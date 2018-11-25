# timestamp runtime libary module

## understand the kv store logic


1. runtime_io::with_externaalities

2. BlockBuilder for RunTime
   
   apply_extrinsic
   
   finalise_block
   
   inherent_extrinsics
   
   check_inherents
   
   random_seed
   

3. apply_extrinsic_no_note_with_len

  f.disptch(s.into())
  
4. **step into Now::put(now)**

4.1. U::put(val, borrow(), &RuntimeStorage)

4.2. StorageValue storage.put(Self::key(), val)

4.3. GenericStorage for RuntimeStorage

4.4 super::storage::put

  value.using_encoded(|slice| runtime_io::set_storage(&twox_128(key)[..], slice));
  
4.5 set_storage sr-io

4.6. set_storage state-machine

4.7 overlayed_changes.rs set_storage


# ::runtime_io::with_externalities

## state-machine is the place where db get updated

