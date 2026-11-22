One <name>.anim.json per animation, same folder layout as the source.
  fps, keys, length_s   timing (keys = number of key frames; a looping clip repeats its first key at the end)
  meta                  additive type, root-motion flags and similar, when the asset has them
  bones.<bone>.p        position per key  [x,y,z]      local to the parent bone, centimetres
  bones.<bone>.r        rotation per key  [x,y,z,w]    local to the parent bone (quaternion)
  bones.<bone>.s        scale per key, only written when it is not 1
Unreal axes: X forward, Y right, Z up (left-handed). index.json lists everything and the assumed bone parents.
debug/ appears only when a file could not be read: send those files back so the reader can be fixed.
