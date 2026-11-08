代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：https://gn.zhonguo5118.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：https://dk.zhonguo8118.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：https://yq.zhonguo6118.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：https://sp.zhonguo6118.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：https://xb.zhonguo4118.cn

C#:   s.ToUpper(); s.ToLower()
来源：https://wz.zhonguo1118.cn

[A24] 去除首尾空白
来源：https://cp.zhonguo1118.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：https://sh.zhonguo3118.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：https://ka.zhonguo8118.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://by.zhonguo7118.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://qa.zhonguo8118.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：https://wr.zhonguo7118.cn

Go:   strings.TrimSpace(s)
来源：https://fd.zhonguo1118.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：https://hk.zhonguo5118.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：https://if.zhonguo6118.cn

[A25] 字符串比较
来源：https://ug.zhonguo7118.cn

Py:   s1 == s2; s1 != s2
来源：https://ej.zhonguo1118.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：https://zc.zhonguo4118.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：https://va.zhonguo7118.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：https://yk.zhonguo8118.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：https://ed.zhonguo5118.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：https://zh.zhonguo8118.cn

Ruby: s1 == s2; s1 <=> s2
来源：https://gl.zhonguo3118.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：https://il.zhonguo7118.cn

[A26] 类型转换总览
来源：https://xr.zhonguo6118.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：https://pa.zhonguo2118.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：https://pe.zhonguo2118.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：https://wv.zhonguo8118.cn

TS:   Number() String() Boolean() x as number
来源：https://ae.zhonguo6118.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：https://bf.zhonguo6118.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：https://so.zhonguo7118.cn

Ruby: to_i to_f to_s to_sym to_a
来源：https://ho.zhonguo1118.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：https://lt.zhonguo6118.cn

================================================================================
来源：https://go.zhonguo2118.cn

B. 流程控制
来源：https://fj.zhonguo6118.cn

================================================================================
来源：https://au.zhonguo7118.cn

[B01] 条件判断 if / else
来源：https://vy.zhonguo5118.cn

Py:   result = "正" if x > 0 else "非正"
来源：https://ac.zhonguo8118.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：https://lj.zhonguo7118.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：https://we.zhonguo3118.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：https://vf.zhonguo4118.cn

Java: String r = x > 0 ? "正" : "非正";
来源：https://lg.zhonguo1118.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：https://ek.zhonguo8118.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：https://lq.zhonguo7118.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：https://qy.zhonguo2118.cn

[B02] 多分支 else if / elif
来源：https://ra.zhonguo6118.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：https://cj.zhonguo4118.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：https://qs.zhonguo6118.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://db.zhonguo5118.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://ao.zhonguo1118.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://nw.zhonguo8118.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：https://ab.zhonguo7118.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：https://iv.zhonguo6118.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://jk.zhonguo2118.cn

[B03] switch / match / case
来源：https://gw.zhonguo7118.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：https://hp.zhonguo4118.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：https://mf.zhonguo7118.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://po.zhonguo4118.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://aq.zhonguo4118.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：https://ip.zhonguo4118.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：https://hq.zhonguo8118.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：https://st.zhonguo2118.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：https://vy.zhonguo7118.cn

[B04] for 计数循环
来源：https://yo.zhonguo1118.cn

Py:   for i in range(10): print(i)
来源：https://uo.zhonguo8118.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：https://qj.zhonguo3118.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://xf.zhonguo8118.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://gc.zhonguo3118.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：https://dq.zhonguo4118.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：https://bb.zhonguo3118.cn

Ruby: 10.times { |i| puts i }
来源：https://bt.zhonguo6118.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：https://wn.zhonguo3118.cn

[B05] 遍历数组 / 列表
来源：https://dw.zhonguo1118.cn

Py:   for item in arr: print(item)
来源：https://dj.zhonguo4118.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：https://sz.zhonguo1118.cn

JS:   for (const item of arr) { console.log(item); }
来源：https://vx.zhonguo7118.cn

TS:   for (const item of arr) { console.log(item); }
来源：https://xs.zhonguo4118.cn

Java: for (var item : arr) { System.out.println(item); }
来源：https://be.zhonguo1118.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：https://fb.zhonguo5118.cn

Ruby: arr.each { |item| puts item }
来源：https://va.zhonguo8118.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：https://uo.zhonguo1118.cn

[B06] 遍历字典 / 对象
来源：https://xl.zhonguo2118.cn

Py:   for k, v in d.items(): print(k, v)
来源：https://ed.zhonguo2118.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：https://qq.zhonguo3118.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://kn.zhonguo8118.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://qn.zhonguo5118.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：https://er.zhonguo1118.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：https://fx.zhonguo3118.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：https://dz.zhonguo5118.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：https://ub.zhonguo5118.cn

[B07] while 循环
来源：https://py.zhonguo5118.cn

Py:   while i < 10: i += 1
来源：https://cf.zhonguo2118.cn

PHP:  while ($i < 10) { $i++; }
来源：https://ft.zhonguo1118.cn

JS:   while (i < 10) { i++; }
来源：https://mz.zhonguo4118.cn

TS:   while (i < 10) { i++; }
来源：https://kz.zhonguo7118.cn

Java: while (i < 10) { i++; }
来源：https://vu.zhonguo6118.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：https://yu.zhonguo1118.cn

Ruby: while i < 10; i += 1; end
来源：https://hg.zhonguo2118.cn

C#:   while (i < 10) { i++; }
来源：https://cy.zhonguo1118.cn

[B08] do-while（至少执行一次）
来源：https://aq.zhonguo8118.cn

Py:   # 无 do-while：用 while True + break
来源：https://vg.zhonguo3118.cn

PHP:  do { $i++; } while ($i < 10);
来源：https://bi.zhonguo6118.cn

JS:   do { i++; } while (i < 10);
来源：https://my.zhonguo6118.cn

TS:   do { i++; } while (i < 10);
来源：https://to.zhonguo3118.cn

Java: do { i++; } while (i < 10);
来源：https://ps.zhonguo7118.cn

Go:   for { i++; if i >= 10 { break } }
来源：https://wj.zhonguo8118.cn

Ruby: begin; i += 1; end while i < 10
来源：https://mt.zhonguo6118.cn

C#:   do { i++; } while (i < 10);
来源：https://pn.zhonguo7118.cn

[B09] break 与 continue
来源：https://cp.zhonguo4118.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：https://eu.zhonguo4118.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：https://xs.zhonguo1118.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://rp.zhonguo7118.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://oq.zhonguo6118.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://va.zhonguo8118.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：https://xh.zhonguo7118.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：https://mh.zhonguo5118.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://zs.zhonguo5118.cn

[B10] 遍历同时拿索引
来源：https://gn.zhonguo7118.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：https://ys.zhonguo7118.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：https://ya.zhonguo6118.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：https://ei.zhonguo2118.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：https://ih.zhonguo7118.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：https://uf.zhonguo6118.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：https://kq.zhonguo3118.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：https://db.zhonguo8118.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：https://wq.zhonguo2118.cn

[B11] 生成数字序列 / 区间
来源：https://dh.zhonguo7118.cn

Py:   list(range(0, 10, 2))
来源：https://zw.zhonguo5118.cn

PHP:  range(0, 10, 2);
来源：https://rm.zhonguo6118.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://dk.zhonguo4118.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://mg.zhonguo4118.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：https://dp.zhonguo2118.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：https://av.zhonguo8118.cn

Ruby: (0...10).step(2).to_a
来源：https://pr.zhonguo2118.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：https://pk.zhonguo4118.cn

[B12] 跳出多层循环
来源：https://ne.zhonguo5118.cn

Py:   # 无标签跳转：抽成函数用 return
来源：https://xp.zhonguo7118.cn

PHP:  # 无标签：用 goto 或函数返回
来源：https://vy.zhonguo5118.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：https://qf.zhonguo6118.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：https://qq.zhonguo8118.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：https://wm.zhonguo1118.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：https://pk.zhonguo3118.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：https://hn.zhonguo5118.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：https://wg.zhonguo3118.cn

[B13] 判断是否为数字
来源：https://fm.zhonguo3118.cn

Py:   isinstance(x, (int, float))
来源：https://hm.zhonguo4118.cn

PHP:  is_numeric($x)
来源：https://jb.zhonguo2118.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：https://jx.zhonguo4118.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：https://qd.zhonguo8118.cn

Java: x instanceof Number
来源：https://kb.zhonguo1118.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：https://jc.zhonguo1118.cn

Ruby: x.is_a?(Numeric)
来源：https://zs.zhonguo2118.cn

C#:   x is int or double or decimal
来源：https://ru.zhonguo1118.cn

[B14] 判断值是否在集合内
来源：https://hj.zhonguo4118.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：https://as.zhonguo1118.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：https://mp.zhonguo4118.cn

JS:   [1, 2, 3].includes(x)
来源：https://sk.zhonguo5118.cn

TS:   [1, 2, 3].includes(x)
来源：https://sb.zhonguo7118.cn

Java: List.of(1, 2, 3).contains(x)
来源：https://jn.zhonguo5118.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：https://ri.zhonguo3118.cn

Ruby: [1, 2, 3].include?(x)
来源：https://ha.zhonguo5118.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：https://cd.zhonguo8118.cn

[B15] 布尔运算与取反
来源：https://dv.zhonguo6118.cn

Py:   a and b or not c
来源：https://lc.zhonguo2118.cn

PHP:  $a && $b || !$c
来源：https://yz.zhonguo6118.cn

JS:   a && b || !c
来源：https://sp.zhonguo2118.cn

TS:   a && b || !c
来源：https://fe.zhonguo7118.cn

Java: a && b || !c
来源：https://oq.zhonguo1118.cn

Go:   a && b || !c
来源：https://wo.zhonguo4118.cn

Ruby: a && b || !c
来源：https://wn.zhonguo5118.cn

C#:   a && b || !c
来源：https://tf.zhonguo7118.cn

[B16] 卫语句：不满足条件提前返回
来源：https://gs.zhonguo8118.cn

Py:   if not data: return
来源：https://xq.zhonguo2118.cn

PHP:  if (!$data) { return; }
来源：https://yp.zhonguo8118.cn

JS:   if (!data) return;
来源：https://kj.zhonguo7118.cn

TS:   if (!data) return;
来源：https://yk.zhonguo3118.cn

Java: if (data == null) return;
来源：https://ug.zhonguo1118.cn

Go:   if data == nil { return }
来源：https://na.zhonguo2118.cn

Ruby: return if data.nil?
来源：https://be.zhonguo7118.cn

C#:   if (data == null) return;
来源：https://cv.zhonguo4118.cn

================================================================================
来源：https://tp.zhonguo1118.cn

C. 函数与作用域
来源：https://bg.zhonguo7118.cn

================================================================================
来源：https://ys.zhonguo8118.cn

[C01] 定义函数
来源：https://hv.zhonguo1118.cn

Py:   def add(a, b): return a + b
来源：https://uk.zhonguo4118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://tj.zhonguo7118.cn

JS:   function add(a, b) { return a + b; }
来源：https://dg.zhonguo4118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://oj.zhonguo5118.cn

Java: static int add(int a, int b) { return a + b; }
来源：https://gt.zhonguo6118.cn

Go:   func add(a, b int) int { return a + b }
来源：https://gj.zhonguo4118.cn

Ruby: def add(a, b); a + b; end
来源：https://av.zhonguo4118.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：https://jr.zhonguo7118.cn

[C02] 默认参数
来源：https://ar.zhonguo4118.cn

Py:   def greet(name="World"): return name
来源：https://zg.zhonguo8118.cn

PHP:  function greet($name = "World") { return $name; }
来源：https://qz.zhonguo2118.cn

JS:   function greet(name = "World") { return name; }
来源：https://wt.zhonguo7118.cn

TS:   function greet(name: string = "World") { return name; }
来源：https://vf.zhonguo4118.cn

Java: // 无默认参数：方法重载或 Optional
来源：https://vy.zhonguo4118.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：https://uo.zhonguo6118.cn

Ruby: def greet(name = "World") = name
来源：https://wl.zhonguo5118.cn

C#:   string Greet(string name = "World") => name;
来源：https://gw.zhonguo6118.cn

[C03] 可变参数
来源：https://fd.zhonguo5118.cn

Py:   def total(*args): return sum(args)
来源：https://js.zhonguo4118.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：https://vi.zhonguo2118.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：https://yd.zhonguo2118.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：https://vc.zhonguo4118.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：https://sa.zhonguo7118.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：https://ux.zhonguo8118.cn

Ruby: def total(*nums); nums.sum; end
来源：https://eo.zhonguo1118.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：https://hw.zhonguo1118.cn

[C04] 命名参数 / 关键字参数
来源：https://gi.zhonguo1118.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：https://fd.zhonguo7118.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：https://gn.zhonguo3118.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：https://af.zhonguo5118.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：https://ec.zhonguo2118.cn

Java: // 无：用 Builder 模式或 record
来源：https://qb.zhonguo1118.cn

Go:   // 无：用配置结构体参数
来源：https://am.zhonguo7118.cn

Ruby: f(a: 1, b: 2)
来源：https://tz.zhonguo7118.cn

C#:   f(a: 1, b: 2)
来源：https://vg.zhonguo8118.cn

[C05] 返回多个值
来源：https://mj.zhonguo3118.cn

Py:   return a, b
来源：https://ve.zhonguo7118.cn

PHP:  return [$a, $b];
来源：https://qe.zhonguo7118.cn

JS:   return [a, b];             // 或 return { a, b };
来源：https://nc.zhonguo4118.cn

TS:   return { a, b };
来源：https://np.zhonguo6118.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：https://et.zhonguo7118.cn

Go:   return a, b
来源：https://ac.zhonguo6118.cn

Ruby: return a, b
来源：https://ai.zhonguo6118.cn

C#:   return (a, b);              // ValueTuple
来源：https://dv.zhonguo8118.cn

[C06] 匿名函数 / lambda
来源：https://mm.zhonguo8118.cn

Py:   square = lambda x: x * x
来源：https://ar.zhonguo5118.cn

PHP:  $square = fn($x) => $x * $x;
来源：https://of.zhonguo2118.cn

JS:   const square = x => x * x;
来源：https://ma.zhonguo5118.cn

TS:   const square = (x: number): number => x * x;
来源：https://em.zhonguo8118.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：https://am.zhonguo4118.cn

Go:   sq := func(x int) int { return x * x }
来源：https://bw.zhonguo5118.cn

Ruby: square = ->(x) { x * x }
来源：https://hr.zhonguo7118.cn

C#:   Func<int, int> square = x => x * x;
来源：https://mq.zhonguo5118.cn

[C07] 把函数作为参数传入
来源：https://xm.zhonguo1118.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：https://oq.zhonguo4118.cn

PHP:  array_map("strtoupper", $arr);
来源：https://wk.zhonguo5118.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：https://td.zhonguo1118.cn

TS:   arr.map(String)
来源：https://ey.zhonguo4118.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：https://zb.zhonguo4118.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：https://fp.zhonguo6118.cn

Ruby: arr.map(&:upcase)
来源：https://ap.zhonguo8118.cn

C#:   arr.Select(s => s.ToUpper())
来源：https://ac.zhonguo3118.cn

[C08] 闭包
来源：https://ze.zhonguo7118.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：https://nw.zhonguo1118.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：https://fl.zhonguo7118.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：https://jq.zhonguo6118.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：https://ko.zhonguo7118.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：https://bt.zhonguo1118.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：https://zx.zhonguo7118.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：https://iq.zhonguo2118.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：https://vu.zhonguo7118.cn

[C09] 递归
来源：https://xg.zhonguo1118.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：https://jd.zhonguo8118.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：https://no.zhonguo3118.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://io.zhonguo1118.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://zx.zhonguo4118.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：https://nw.zhonguo8118.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：https://hz.zhonguo3118.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：https://xv.zhonguo7118.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：https://su.zhonguo4118.cn

[C10] 变量作用域
来源：https://kl.zhonguo8118.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：https://qb.zhonguo5118.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：https://vl.zhonguo6118.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：https://ny.zhonguo1118.cn

TS:   同 JS
来源：https://hn.zhonguo1118.cn

Java: 方法内为块级作用域
来源：https://nw.zhonguo7118.cn

Go:   花括号块级作用域
来源：https://sy.zhonguo8118.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：https://es.zhonguo5118.cn

C#:   块级作用域
来源：https://kw.zhonguo4118.cn

[C11] 模块导入与导出
来源：https://ud.zhonguo8118.cn

Py:   from module import func
来源：https://ed.zhonguo1118.cn

PHP:  require "file.php";  或 use App\Service;
来源：https://pa.zhonguo7118.cn

JS:   export default function f() {};  import f from "./m.js";
来源：https://ly.zhonguo3118.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：https://py.zhonguo8118.cn

Java: import java.util.List;
来源：https://ez.zhonguo8118.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：https://up.zhonguo3118.cn

Ruby: require "json"; require_relative "./util"
来源：https://wx.zhonguo3118.cn

C#:   using System.Text;
来源：https://xu.zhonguo4118.cn

[C12] 立即执行函数 IIFE
来源：https://lr.zhonguo5118.cn

Py:   (lambda: print("run"))()
来源：https://xg.zhonguo5118.cn

PHP:  (function () { echo "run"; })();
来源：https://ru.zhonguo8118.cn

JS:   (() => { console.log("run"); })();
来源：https://gr.zhonguo8118.cn

TS:   (() => { console.log("run"); })();
来源：https://rh.zhonguo7118.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：https://gj.zhonguo5118.cn

Go:   func() { fmt.Println("run") }()
来源：https://vz.zhonguo5118.cn

Ruby: -> { puts "run" }.call
来源：https://ha.zhonguo2118.cn

C#:   // 无 IIFE：用静态构造函数
来源：https://xl.zhonguo7118.cn

[C13] 类型声明 / 类型注解
来源：https://cy.zhonguo7118.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：https://po.zhonguo2118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://ek.zhonguo3118.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：https://zj.zhonguo7118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://ai.zhonguo4118.cn

Java: int add(int a, int b) { return a + b; }
来源：https://tm.zhonguo5118.cn

Go:   func add(a, b int) int
来源：https://lb.zhonguo8118.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：https://lt.zhonguo1118.cn

C#:   int Add(int a, int b) => a + b;
来源：https://el.zhonguo6118.cn


<!-- 参考信息 -->