# import

  ```
  (u1, u4, u8, u16, u32, u64, u128) = ... @ types
  (i1, i4, i8, i16, i32, i64, i128) = ... @ types
  (true, false, bool, text) = ... @ types
  ```

# declare

  ```
  value  : u32          = 1000
  tuple  : (str,i8,i32) = ('a', 1, 100)
  array  : [u32]        = [1, 2, 3, 4]
  dict   : {str:int}    = {a:1, b:2, c:3}
  string : text         = "hello"
  ```

# assign

  ```
  value   = 2000
  tuple   = ('b', 2, 200)
  array  += [5] + [6, 7]
  dict   += {d:4}
  string += " " + "world"
  ```

# conditional

  ```
  true ? (
    stdout.print("true!"),
    stderr.print("false!"),
  )
  ```

  ```
  case = 100
  case ? {
    0..100  : stdout.print("match!"),
    'a'..'b': stderr.print("miss!"),
  }
  ```

# loop

  ```
  while | (
    stmt,
  )

  for | (
  )
