代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：https://dj.zhonguo1118.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：https://pr.zhonguo4118.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：https://ik.zhonguo5118.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：https://zl.zhonguo1118.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：https://xc.zhonguo5118.cn

C#:   s.ToUpper(); s.ToLower()
来源：https://qx.zhonguo8118.cn

[A24] 去除首尾空白
来源：https://ri.zhonguo1118.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：https://hy.zhonguo5118.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：https://da.zhonguo2118.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://sy.zhonguo6118.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://bd.zhonguo6118.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：https://pc.zhonguo8118.cn

Go:   strings.TrimSpace(s)
来源：https://ca.zhonguo1118.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：https://id.zhonguo4118.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：https://lq.zhonguo5118.cn

[A25] 字符串比较
来源：https://rw.zhonguo1118.cn

Py:   s1 == s2; s1 != s2
来源：https://xd.zhonguo8118.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：https://kd.zhonguo4118.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：https://fh.zhonguo2118.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：https://cp.zhonguo6118.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：https://sa.zhonguo3118.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：https://ez.zhonguo3118.cn

Ruby: s1 == s2; s1 <=> s2
来源：https://oj.zhonguo2118.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：https://is.zhonguo6118.cn

[A26] 类型转换总览
来源：https://ts.zhonguo7118.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：https://de.zhonguo2118.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：https://pn.zhonguo3118.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：https://pc.zhonguo7118.cn

TS:   Number() String() Boolean() x as number
来源：https://ei.zhonguo5118.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：https://mj.zhonguo3118.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：https://ox.zhonguo1118.cn

Ruby: to_i to_f to_s to_sym to_a
来源：https://ma.zhonguo1118.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：https://ou.zhonguo6118.cn

================================================================================
来源：https://xv.zhonguo1118.cn

B. 流程控制
来源：https://lm.zhonguo5118.cn

================================================================================
来源：https://jg.zhonguo3118.cn

[B01] 条件判断 if / else
来源：https://tx.zhonguo2118.cn

Py:   result = "正" if x > 0 else "非正"
来源：https://kh.zhonguo7118.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：https://vm.zhonguo2118.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：https://oq.zhonguo1118.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：https://tw.zhonguo6118.cn

Java: String r = x > 0 ? "正" : "非正";
来源：https://ia.zhonguo2118.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：https://bc.zhonguo3118.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：https://db.zhonguo8118.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：https://ii.zhonguo4118.cn

[B02] 多分支 else if / elif
来源：https://af.zhonguo7118.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：https://qv.zhonguo2118.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：https://ju.zhonguo2118.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://mf.zhonguo6118.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://mg.zhonguo3118.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://vb.zhonguo5118.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：https://qj.zhonguo2118.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：https://vu.zhonguo7118.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://oc.zhonguo1118.cn

[B03] switch / match / case
来源：https://jl.zhonguo6118.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：https://an.zhonguo8118.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：https://yp.zhonguo1118.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://dr.zhonguo4118.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://uf.zhonguo7118.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：https://ce.zhonguo6118.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：https://cb.zhonguo6118.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：https://tp.zhonguo3118.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：https://ig.zhonguo8118.cn

[B04] for 计数循环
来源：https://my.zhonguo5118.cn

Py:   for i in range(10): print(i)
来源：https://fo.zhonguo3118.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：https://ix.zhonguo6118.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://uf.zhonguo5118.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://al.zhonguo7118.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：https://ew.zhonguo1118.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：https://jz.zhonguo6118.cn

Ruby: 10.times { |i| puts i }
来源：https://ix.zhonguo7118.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：https://fl.zhonguo1118.cn

[B05] 遍历数组 / 列表
来源：https://oj.zhonguo1118.cn

Py:   for item in arr: print(item)
来源：https://ff.zhonguo2118.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：https://fc.zhonguo1118.cn

JS:   for (const item of arr) { console.log(item); }
来源：https://jk.zhonguo5118.cn

TS:   for (const item of arr) { console.log(item); }
来源：https://il.zhonguo5118.cn

Java: for (var item : arr) { System.out.println(item); }
来源：https://pv.zhonguo5118.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：https://cw.zhonguo7118.cn

Ruby: arr.each { |item| puts item }
来源：https://pq.zhonguo7118.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：https://zb.zhonguo8118.cn

[B06] 遍历字典 / 对象
来源：https://wa.zhonguo7118.cn

Py:   for k, v in d.items(): print(k, v)
来源：https://rk.zhonguo3118.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：https://ir.zhonguo6118.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://sf.zhonguo6118.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://vc.zhonguo3118.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：https://oo.zhonguo1118.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：https://nq.zhonguo5118.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：https://qy.zhonguo5118.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：https://xa.zhonguo5118.cn

[B07] while 循环
来源：https://vp.zhonguo4118.cn

Py:   while i < 10: i += 1
来源：https://za.zhonguo8118.cn

PHP:  while ($i < 10) { $i++; }
来源：https://yi.zhonguo5118.cn

JS:   while (i < 10) { i++; }
来源：https://yf.zhonguo6118.cn

TS:   while (i < 10) { i++; }
来源：https://qm.zhonguo3118.cn

Java: while (i < 10) { i++; }
来源：https://nk.zhonguo8118.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：https://ks.zhonguo8118.cn

Ruby: while i < 10; i += 1; end
来源：https://lt.zhonguo1118.cn

C#:   while (i < 10) { i++; }
来源：https://wb.zhonguo2118.cn

[B08] do-while（至少执行一次）
来源：https://kz.zhonguo4118.cn

Py:   # 无 do-while：用 while True + break
来源：https://ip.zhonguo7118.cn

PHP:  do { $i++; } while ($i < 10);
来源：https://wl.zhonguo2118.cn

JS:   do { i++; } while (i < 10);
来源：https://gm.zhonguo4118.cn

TS:   do { i++; } while (i < 10);
来源：https://iv.zhonguo5118.cn

Java: do { i++; } while (i < 10);
来源：https://cj.zhonguo8118.cn

Go:   for { i++; if i >= 10 { break } }
来源：https://mq.zhonguo7118.cn

Ruby: begin; i += 1; end while i < 10
来源：https://rs.zhonguo7118.cn

C#:   do { i++; } while (i < 10);
来源：https://ej.zhonguo3118.cn

[B09] break 与 continue
来源：https://gv.zhonguo5118.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：https://vj.zhonguo8118.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：https://uv.zhonguo4118.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://rh.zhonguo5118.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://kb.zhonguo8118.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://me.zhonguo4118.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：https://pz.zhonguo6118.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：https://nq.zhonguo6118.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://rk.zhonguo1118.cn

[B10] 遍历同时拿索引
来源：https://do.zhonguo5118.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：https://xr.zhonguo3118.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：https://wd.zhonguo5118.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：https://qp.zhonguo3118.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：https://qw.zhonguo1118.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：https://iy.zhonguo4118.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：https://xt.zhonguo7118.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：https://qf.zhonguo5118.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：https://xi.zhonguo8118.cn

[B11] 生成数字序列 / 区间
来源：https://gj.zhonguo5118.cn

Py:   list(range(0, 10, 2))
来源：https://xo.zhonguo4118.cn

PHP:  range(0, 10, 2);
来源：https://cl.zhonguo4118.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://tu.zhonguo2118.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://jd.zhonguo3118.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：https://ke.zhonguo3118.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：https://oj.zhonguo7118.cn

Ruby: (0...10).step(2).to_a
来源：https://se.zhonguo1118.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：https://jx.zhonguo3118.cn

[B12] 跳出多层循环
来源：https://ha.zhonguo4118.cn

Py:   # 无标签跳转：抽成函数用 return
来源：https://ti.zhonguo2118.cn

PHP:  # 无标签：用 goto 或函数返回
来源：https://tx.zhonguo7118.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：https://yt.zhonguo6118.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：https://ym.zhonguo1118.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：https://xr.zhonguo2118.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：https://ue.zhonguo3118.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：https://vr.zhonguo1118.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：https://tw.zhonguo4118.cn

[B13] 判断是否为数字
来源：https://hf.zhonguo2118.cn

Py:   isinstance(x, (int, float))
来源：https://kg.zhonguo3118.cn

PHP:  is_numeric($x)
来源：https://wg.zhonguo3118.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：https://st.zhonguo3118.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：https://yb.zhonguo1118.cn

Java: x instanceof Number
来源：https://jn.zhonguo3118.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：https://ib.zhonguo7118.cn

Ruby: x.is_a?(Numeric)
来源：https://ab.zhonguo4118.cn

C#:   x is int or double or decimal
来源：https://mv.zhonguo1118.cn

[B14] 判断值是否在集合内
来源：https://lf.zhonguo8118.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：https://uw.zhonguo3118.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：https://lm.zhonguo5118.cn

JS:   [1, 2, 3].includes(x)
来源：https://ic.zhonguo1118.cn

TS:   [1, 2, 3].includes(x)
来源：https://kt.zhonguo6118.cn

Java: List.of(1, 2, 3).contains(x)
来源：https://cx.zhonguo6118.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：https://le.zhonguo3118.cn

Ruby: [1, 2, 3].include?(x)
来源：https://xl.zhonguo6118.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：https://mv.zhonguo4118.cn

[B15] 布尔运算与取反
来源：https://xy.zhonguo3118.cn

Py:   a and b or not c
来源：https://vy.zhonguo8118.cn

PHP:  $a && $b || !$c
来源：https://sd.zhonguo1118.cn

JS:   a && b || !c
来源：https://sl.zhonguo2118.cn

TS:   a && b || !c
来源：https://vk.zhonguo6118.cn

Java: a && b || !c
来源：https://cr.zhonguo8118.cn

Go:   a && b || !c
来源：https://mi.zhonguo3118.cn

Ruby: a && b || !c
来源：https://ht.zhonguo7118.cn

C#:   a && b || !c
来源：https://fe.zhonguo6118.cn

[B16] 卫语句：不满足条件提前返回
来源：https://zr.zhonguo1118.cn

Py:   if not data: return
来源：https://fr.zhonguo5118.cn

PHP:  if (!$data) { return; }
来源：https://fk.zhonguo5118.cn

JS:   if (!data) return;
来源：https://ra.zhonguo3118.cn

TS:   if (!data) return;
来源：https://zd.zhonguo4118.cn

Java: if (data == null) return;
来源：https://eh.zhonguo8118.cn

Go:   if data == nil { return }
来源：https://ty.zhonguo4118.cn

Ruby: return if data.nil?
来源：https://vl.zhonguo8118.cn

C#:   if (data == null) return;
来源：https://gm.zhonguo5118.cn

================================================================================
来源：https://no.zhonguo2118.cn

C. 函数与作用域
来源：https://tf.zhonguo2118.cn

================================================================================
来源：https://mh.zhonguo3118.cn

[C01] 定义函数
来源：https://il.zhonguo7118.cn

Py:   def add(a, b): return a + b
来源：https://fh.zhonguo3118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://ks.zhonguo8118.cn

JS:   function add(a, b) { return a + b; }
来源：https://dy.zhonguo5118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://wy.zhonguo3118.cn

Java: static int add(int a, int b) { return a + b; }
来源：https://qq.zhonguo5118.cn

Go:   func add(a, b int) int { return a + b }
来源：https://qt.zhonguo4118.cn

Ruby: def add(a, b); a + b; end
来源：https://ql.zhonguo7118.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：https://zh.zhonguo8118.cn

[C02] 默认参数
来源：https://ji.zhonguo2118.cn

Py:   def greet(name="World"): return name
来源：https://mv.zhonguo6118.cn

PHP:  function greet($name = "World") { return $name; }
来源：https://sv.zhonguo7118.cn

JS:   function greet(name = "World") { return name; }
来源：https://sl.zhonguo3118.cn

TS:   function greet(name: string = "World") { return name; }
来源：https://lj.zhonguo1118.cn

Java: // 无默认参数：方法重载或 Optional
来源：https://ed.zhonguo3118.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：https://bb.zhonguo3118.cn

Ruby: def greet(name = "World") = name
来源：https://gt.zhonguo4118.cn

C#:   string Greet(string name = "World") => name;
来源：https://eb.zhonguo7118.cn

[C03] 可变参数
来源：https://gq.zhonguo1118.cn

Py:   def total(*args): return sum(args)
来源：https://vz.zhonguo5118.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：https://af.zhonguo3118.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：https://ij.zhonguo3118.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：https://kl.zhonguo4118.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：https://vp.zhonguo5118.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：https://le.zhonguo4118.cn

Ruby: def total(*nums); nums.sum; end
来源：https://ds.zhonguo8118.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：https://pm.zhonguo2118.cn

[C04] 命名参数 / 关键字参数
来源：https://gh.zhonguo4118.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：https://vi.zhonguo2118.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：https://yd.zhonguo5118.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：https://bu.zhonguo7118.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：https://qi.zhonguo7118.cn

Java: // 无：用 Builder 模式或 record
来源：https://wt.zhonguo3118.cn

Go:   // 无：用配置结构体参数
来源：https://dv.zhonguo7118.cn

Ruby: f(a: 1, b: 2)
来源：https://rp.zhonguo4118.cn

C#:   f(a: 1, b: 2)
来源：https://vd.zhonguo2118.cn

[C05] 返回多个值
来源：https://qh.zhonguo1118.cn

Py:   return a, b
来源：https://wa.zhonguo4118.cn

PHP:  return [$a, $b];
来源：https://yn.zhonguo2118.cn

JS:   return [a, b];             // 或 return { a, b };
来源：https://xx.zhonguo6118.cn

TS:   return { a, b };
来源：https://tn.zhonguo2118.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：https://cl.zhonguo5118.cn

Go:   return a, b
来源：https://pm.zhonguo2118.cn

Ruby: return a, b
来源：https://ho.zhonguo3118.cn

C#:   return (a, b);              // ValueTuple
来源：https://zn.zhonguo3118.cn

[C06] 匿名函数 / lambda
来源：https://st.zhonguo2118.cn

Py:   square = lambda x: x * x
来源：https://kj.zhonguo5118.cn

PHP:  $square = fn($x) => $x * $x;
来源：https://rb.zhonguo7118.cn

JS:   const square = x => x * x;
来源：https://wi.zhonguo5118.cn

TS:   const square = (x: number): number => x * x;
来源：https://pk.zhonguo2118.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：https://vn.zhonguo3118.cn

Go:   sq := func(x int) int { return x * x }
来源：https://jh.zhonguo4118.cn

Ruby: square = ->(x) { x * x }
来源：https://wy.zhonguo8118.cn

C#:   Func<int, int> square = x => x * x;
来源：https://by.zhonguo3118.cn

[C07] 把函数作为参数传入
来源：https://wf.zhonguo3118.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：https://gu.zhonguo3118.cn

PHP:  array_map("strtoupper", $arr);
来源：https://ni.zhonguo6118.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：https://vb.zhonguo4118.cn

TS:   arr.map(String)
来源：https://uf.zhonguo3118.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：https://uv.zhonguo6118.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：https://sy.zhonguo3118.cn

Ruby: arr.map(&:upcase)
来源：https://td.zhonguo5118.cn

C#:   arr.Select(s => s.ToUpper())
来源：https://td.zhonguo1118.cn

[C08] 闭包
来源：https://zu.zhonguo7118.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：https://yv.zhonguo4118.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：https://pv.zhonguo3118.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：https://sq.zhonguo1118.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：https://yv.zhonguo3118.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：https://cg.zhonguo8118.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：https://kv.zhonguo4118.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：https://bi.zhonguo6118.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：https://zd.zhonguo8118.cn

[C09] 递归
来源：https://wv.zhonguo6118.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：https://av.zhonguo8118.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：https://pd.zhonguo4118.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://yt.zhonguo2118.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://uz.zhonguo7118.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：https://mi.zhonguo5118.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：https://ka.zhonguo8118.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：https://sa.zhonguo2118.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：https://dw.zhonguo7118.cn

[C10] 变量作用域
来源：https://al.zhonguo3118.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：https://jf.zhonguo8118.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：https://nd.zhonguo3118.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：https://pa.zhonguo5118.cn

TS:   同 JS
来源：https://zp.zhonguo6118.cn

Java: 方法内为块级作用域
来源：https://sw.zhonguo4118.cn

Go:   花括号块级作用域
来源：https://xn.zhonguo6118.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：https://uu.zhonguo6118.cn

C#:   块级作用域
来源：https://lk.zhonguo3118.cn

[C11] 模块导入与导出
来源：https://yg.zhonguo3118.cn

Py:   from module import func
来源：https://sn.zhonguo4118.cn

PHP:  require "file.php";  或 use App\Service;
来源：https://qm.zhonguo1118.cn

JS:   export default function f() {};  import f from "./m.js";
来源：https://pj.zhonguo5118.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：https://jn.zhonguo3118.cn

Java: import java.util.List;
来源：https://kv.zhonguo3118.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：https://qh.zhonguo7118.cn

Ruby: require "json"; require_relative "./util"
来源：https://hv.zhonguo6118.cn

C#:   using System.Text;
来源：https://rk.zhonguo4118.cn

[C12] 立即执行函数 IIFE
来源：https://bd.zhonguo6118.cn

Py:   (lambda: print("run"))()
来源：https://dx.zhonguo3118.cn

PHP:  (function () { echo "run"; })();
来源：https://gh.zhonguo4118.cn

JS:   (() => { console.log("run"); })();
来源：https://jz.zhonguo4118.cn

TS:   (() => { console.log("run"); })();
来源：https://dq.zhonguo5118.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：https://sy.zhonguo7118.cn

Go:   func() { fmt.Println("run") }()
来源：https://bl.zhonguo1118.cn

Ruby: -> { puts "run" }.call
来源：https://qy.zhonguo7118.cn

C#:   // 无 IIFE：用静态构造函数
来源：https://sg.zhonguo6118.cn

[C13] 类型声明 / 类型注解
来源：https://ze.zhonguo2118.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：https://xp.zhonguo1118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://av.zhonguo2118.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：https://hd.zhonguo5118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://wn.zhonguo3118.cn

Java: int add(int a, int b) { return a + b; }
来源：https://gn.zhonguo8118.cn

Go:   func add(a, b int) int
来源：https://vw.zhonguo7118.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：https://ap.zhonguo3118.cn

C#:   int Add(int a, int b) => a + b;
来源：https://qo.zhonguo7118.cn


<!-- 参考信息 -->