代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：https://zy.zhonguo7118.cn

================================================================================
来源：https://nj.zhonguo1118.cn

B. 流程控制
来源：https://gj.zhonguo6118.cn

================================================================================
来源：https://kk.zhonguo6118.cn

[B01] 条件判断 if / else
来源：https://ld.zhonguo2118.cn

Py:   result = "正" if x > 0 else "非正"
来源：https://hh.zhonguo8118.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：https://yz.zhonguo2118.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：https://ev.zhonguo5118.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：https://ju.zhonguo2118.cn

Java: String r = x > 0 ? "正" : "非正";
来源：https://uo.zhonguo6118.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：https://yx.zhonguo2118.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：https://ki.zhonguo8118.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：https://sn.zhonguo1118.cn

[B02] 多分支 else if / elif
来源：https://eo.zhonguo6118.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：https://xo.zhonguo1118.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：https://tt.zhonguo1118.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://xn.zhonguo1118.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://vy.zhonguo7118.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://tj.zhonguo1118.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：https://qu.zhonguo4118.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：https://qi.zhonguo5118.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://hs.zhonguo7118.cn

[B03] switch / match / case
来源：https://tv.zhonguo4118.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：https://xy.zhonguo1118.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：https://gk.zhonguo8118.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://jb.zhonguo5118.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://dz.zhonguo3118.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：https://ij.zhonguo6118.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：https://bp.zhonguo5118.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：https://nm.zhonguo1118.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：https://hh.zhonguo3118.cn

[B04] for 计数循环
来源：https://vz.zhonguo5118.cn

Py:   for i in range(10): print(i)
来源：https://jn.zhonguo8118.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：https://at.zhonguo1118.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://on.zhonguo6118.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://ns.zhonguo8118.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：https://ud.zhonguo3118.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：https://xk.zhonguo2118.cn

Ruby: 10.times { |i| puts i }
来源：https://ay.zhonguo1118.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：https://ks.zhonguo3118.cn

[B05] 遍历数组 / 列表
来源：https://cd.zhonguo1118.cn

Py:   for item in arr: print(item)
来源：https://rr.zhonguo8118.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：https://fm.zhonguo1118.cn

JS:   for (const item of arr) { console.log(item); }
来源：https://vn.zhonguo7118.cn

TS:   for (const item of arr) { console.log(item); }
来源：https://qv.zhonguo3118.cn

Java: for (var item : arr) { System.out.println(item); }
来源：https://aq.zhonguo8118.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：https://qv.zhonguo7118.cn

Ruby: arr.each { |item| puts item }
来源：https://hx.zhonguo8118.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：https://vf.zhonguo1118.cn

[B06] 遍历字典 / 对象
来源：https://pm.zhonguo7118.cn

Py:   for k, v in d.items(): print(k, v)
来源：https://ty.zhonguo8118.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：https://np.zhonguo6118.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://za.zhonguo1118.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://kc.zhonguo1118.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：https://uc.zhonguo7118.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：https://dn.zhonguo6118.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：https://ra.zhonguo2118.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：https://mj.zhonguo6118.cn

[B07] while 循环
来源：https://to.zhonguo7118.cn

Py:   while i < 10: i += 1
来源：https://ph.zhonguo8118.cn

PHP:  while ($i < 10) { $i++; }
来源：https://xs.zhonguo7118.cn

JS:   while (i < 10) { i++; }
来源：https://gi.zhonguo7118.cn

TS:   while (i < 10) { i++; }
来源：https://rq.zhonguo6118.cn

Java: while (i < 10) { i++; }
来源：https://hl.zhonguo5118.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：https://bu.zhonguo8118.cn

Ruby: while i < 10; i += 1; end
来源：https://lm.zhonguo3118.cn

C#:   while (i < 10) { i++; }
来源：https://dq.zhonguo6118.cn

[B08] do-while（至少执行一次）
来源：https://uy.zhonguo7118.cn

Py:   # 无 do-while：用 while True + break
来源：https://yu.zhonguo3118.cn

PHP:  do { $i++; } while ($i < 10);
来源：https://qc.zhonguo7118.cn

JS:   do { i++; } while (i < 10);
来源：https://jk.zhonguo2118.cn

TS:   do { i++; } while (i < 10);
来源：https://nk.zhonguo6118.cn

Java: do { i++; } while (i < 10);
来源：https://cp.zhonguo2118.cn

Go:   for { i++; if i >= 10 { break } }
来源：https://wg.zhonguo7118.cn

Ruby: begin; i += 1; end while i < 10
来源：https://us.zhonguo3118.cn

C#:   do { i++; } while (i < 10);
来源：https://ok.zhonguo1118.cn

[B09] break 与 continue
来源：https://vv.zhonguo4118.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：https://nd.zhonguo6118.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：https://vx.zhonguo6118.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://yr.zhonguo4118.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://ck.zhonguo8118.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://oe.zhonguo2118.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：https://ze.zhonguo4118.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：https://ib.zhonguo8118.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://tv.zhonguo8118.cn

[B10] 遍历同时拿索引
来源：https://ue.zhonguo8118.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：https://yx.zhonguo4118.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：https://dt.zhonguo6118.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：https://tp.zhonguo1118.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：https://sz.zhonguo3118.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：https://vi.zhonguo7118.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：https://qs.zhonguo5118.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：https://ku.zhonguo7118.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：https://nz.zhonguo8118.cn

[B11] 生成数字序列 / 区间
来源：https://uk.zhonguo8118.cn

Py:   list(range(0, 10, 2))
来源：https://gv.zhonguo8118.cn

PHP:  range(0, 10, 2);
来源：https://th.zhonguo8118.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://rd.zhonguo4118.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://ic.zhonguo5118.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：https://wh.zhonguo8118.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：https://ze.zhonguo7118.cn

Ruby: (0...10).step(2).to_a
来源：https://ll.zhonguo2118.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：https://rx.zhonguo1118.cn

[B12] 跳出多层循环
来源：https://zr.zhonguo2118.cn

Py:   # 无标签跳转：抽成函数用 return
来源：https://kj.zhonguo6118.cn

PHP:  # 无标签：用 goto 或函数返回
来源：https://go.zhonguo6118.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：https://nm.zhonguo7118.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：https://yc.zhonguo6118.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：https://xb.zhonguo6118.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：https://oy.zhonguo5118.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：https://uz.zhonguo4118.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：https://se.zhonguo8118.cn

[B13] 判断是否为数字
来源：https://sp.zhonguo8118.cn

Py:   isinstance(x, (int, float))
来源：https://jw.zhonguo5118.cn

PHP:  is_numeric($x)
来源：https://sv.zhonguo8118.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：https://fk.zhonguo7118.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：https://kc.zhonguo4118.cn

Java: x instanceof Number
来源：https://ay.zhonguo7118.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：https://qn.zhonguo2118.cn

Ruby: x.is_a?(Numeric)
来源：https://vn.zhonguo5118.cn

C#:   x is int or double or decimal
来源：https://vt.zhonguo5118.cn

[B14] 判断值是否在集合内
来源：https://ml.zhonguo2118.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：https://fx.zhonguo4118.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：https://be.zhonguo6118.cn

JS:   [1, 2, 3].includes(x)
来源：https://cc.zhonguo5118.cn

TS:   [1, 2, 3].includes(x)
来源：https://si.zhonguo3118.cn

Java: List.of(1, 2, 3).contains(x)
来源：https://wd.zhonguo8118.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：https://nd.zhonguo7118.cn

Ruby: [1, 2, 3].include?(x)
来源：https://se.zhonguo2118.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：https://am.zhonguo4118.cn

[B15] 布尔运算与取反
来源：https://da.zhonguo4118.cn

Py:   a and b or not c
来源：https://po.zhonguo4118.cn

PHP:  $a && $b || !$c
来源：https://tf.zhonguo6118.cn

JS:   a && b || !c
来源：https://tq.zhonguo3118.cn

TS:   a && b || !c
来源：https://qh.zhonguo3118.cn

Java: a && b || !c
来源：https://dl.zhonguo5118.cn

Go:   a && b || !c
来源：https://hr.zhonguo8118.cn

Ruby: a && b || !c
来源：https://mi.zhonguo4118.cn

C#:   a && b || !c
来源：https://cn.zhonguo1118.cn

[B16] 卫语句：不满足条件提前返回
来源：https://pp.zhonguo5118.cn

Py:   if not data: return
来源：https://dt.zhonguo5118.cn

PHP:  if (!$data) { return; }
来源：https://ui.zhonguo1118.cn

JS:   if (!data) return;
来源：https://fq.zhonguo5118.cn

TS:   if (!data) return;
来源：https://ud.zhonguo7118.cn

Java: if (data == null) return;
来源：https://tf.zhonguo8118.cn

Go:   if data == nil { return }
来源：https://wb.zhonguo6118.cn

Ruby: return if data.nil?
来源：https://mg.zhonguo1118.cn

C#:   if (data == null) return;
来源：https://ng.zhonguo6118.cn

================================================================================
来源：https://ot.zhonguo8118.cn

C. 函数与作用域
来源：https://cv.zhonguo5118.cn

================================================================================
来源：https://rj.zhonguo4118.cn

[C01] 定义函数
来源：https://kf.zhonguo2118.cn

Py:   def add(a, b): return a + b
来源：https://lr.zhonguo3118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://wn.zhonguo3118.cn

JS:   function add(a, b) { return a + b; }
来源：https://vj.zhonguo7118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://rk.zhonguo4118.cn

Java: static int add(int a, int b) { return a + b; }
来源：https://bi.zhonguo8118.cn

Go:   func add(a, b int) int { return a + b }
来源：https://vm.zhonguo2118.cn

Ruby: def add(a, b); a + b; end
来源：https://si.zhonguo7118.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：https://fg.zhonguo3118.cn

[C02] 默认参数
来源：https://za.zhonguo5118.cn

Py:   def greet(name="World"): return name
来源：https://th.zhonguo2118.cn

PHP:  function greet($name = "World") { return $name; }
来源：https://mx.zhonguo5118.cn

JS:   function greet(name = "World") { return name; }
来源：https://ny.zhonguo7118.cn

TS:   function greet(name: string = "World") { return name; }
来源：https://rd.zhonguo7118.cn

Java: // 无默认参数：方法重载或 Optional
来源：https://if.zhonguo1118.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：https://hm.zhonguo5118.cn

Ruby: def greet(name = "World") = name
来源：https://eh.zhonguo8118.cn

C#:   string Greet(string name = "World") => name;
来源：https://op.zhonguo1118.cn

[C03] 可变参数
来源：https://ei.zhonguo7118.cn

Py:   def total(*args): return sum(args)
来源：https://ao.zhonguo4118.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：https://cz.zhonguo2118.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：https://do.zhonguo6118.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：https://hf.zhonguo6118.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：https://ia.zhonguo6118.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：https://cf.zhonguo7118.cn

Ruby: def total(*nums); nums.sum; end
来源：https://ct.zhonguo3118.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：https://bs.zhonguo2118.cn

[C04] 命名参数 / 关键字参数
来源：https://el.zhonguo5118.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：https://lv.zhonguo5118.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：https://ln.zhonguo3118.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：https://jy.zhonguo4118.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：https://nu.zhonguo8118.cn

Java: // 无：用 Builder 模式或 record
来源：https://eu.zhonguo1118.cn

Go:   // 无：用配置结构体参数
来源：https://en.zhonguo7118.cn

Ruby: f(a: 1, b: 2)
来源：https://tg.zhonguo2118.cn

C#:   f(a: 1, b: 2)
来源：https://zu.zhonguo2118.cn

[C05] 返回多个值
来源：https://df.zhonguo2118.cn

Py:   return a, b
来源：https://vm.zhonguo1118.cn

PHP:  return [$a, $b];
来源：https://la.zhonguo2118.cn

JS:   return [a, b];             // 或 return { a, b };
来源：https://kk.zhonguo1118.cn

TS:   return { a, b };
来源：https://rf.zhonguo2118.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：https://ii.zhonguo6118.cn

Go:   return a, b
来源：https://nw.zhonguo6118.cn

Ruby: return a, b
来源：https://uk.zhonguo2118.cn

C#:   return (a, b);              // ValueTuple
来源：https://oe.zhonguo2118.cn

[C06] 匿名函数 / lambda
来源：https://ci.zhonguo6118.cn

Py:   square = lambda x: x * x
来源：https://fa.zhonguo5118.cn

PHP:  $square = fn($x) => $x * $x;
来源：https://dv.zhonguo2118.cn

JS:   const square = x => x * x;
来源：https://ih.zhonguo8118.cn

TS:   const square = (x: number): number => x * x;
来源：https://ng.zhonguo5118.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：https://zm.zhonguo8118.cn

Go:   sq := func(x int) int { return x * x }
来源：https://ul.zhonguo4118.cn

Ruby: square = ->(x) { x * x }
来源：https://nl.zhonguo6118.cn

C#:   Func<int, int> square = x => x * x;
来源：https://lj.zhonguo7118.cn

[C07] 把函数作为参数传入
来源：https://ls.zhonguo8118.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：https://lb.zhonguo3118.cn

PHP:  array_map("strtoupper", $arr);
来源：https://uj.zhonguo4118.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：https://uu.zhonguo2118.cn

TS:   arr.map(String)
来源：https://tz.zhonguo5118.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：https://ip.zhonguo8118.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：https://kp.zhonguo7118.cn

Ruby: arr.map(&:upcase)
来源：https://xp.zhonguo7118.cn

C#:   arr.Select(s => s.ToUpper())
来源：https://np.zhonguo1118.cn

[C08] 闭包
来源：https://hg.zhonguo7118.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：https://eg.zhonguo1118.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：https://zd.zhonguo3118.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：https://xs.zhonguo4118.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：https://sf.zhonguo8118.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：https://xb.zhonguo4118.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：https://zz.zhonguo7118.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：https://pw.zhonguo7118.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：https://ss.zhonguo6118.cn

[C09] 递归
来源：https://bf.zhonguo4118.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：https://qy.zhonguo6118.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：https://az.zhonguo2118.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://lp.zhonguo6118.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://bd.zhonguo7118.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：https://cp.zhonguo3118.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：https://fo.zhonguo1118.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：https://hl.zhonguo8118.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：https://fc.zhonguo2118.cn

[C10] 变量作用域
来源：https://yr.zhonguo5118.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：https://fl.zhonguo7118.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：https://qk.zhonguo6118.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：https://vh.zhonguo6118.cn

TS:   同 JS
来源：https://tv.zhonguo2118.cn

Java: 方法内为块级作用域
来源：https://ab.zhonguo1118.cn

Go:   花括号块级作用域
来源：https://nw.zhonguo2118.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：https://tb.zhonguo2118.cn

C#:   块级作用域
来源：https://ip.zhonguo6118.cn

[C11] 模块导入与导出
来源：https://il.zhonguo3118.cn

Py:   from module import func
来源：https://ft.zhonguo8118.cn

PHP:  require "file.php";  或 use App\Service;
来源：https://yi.zhonguo7118.cn

JS:   export default function f() {};  import f from "./m.js";
来源：https://hz.zhonguo1118.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：https://tx.zhonguo8118.cn

Java: import java.util.List;
来源：https://bs.zhonguo4118.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：https://lm.zhonguo8118.cn

Ruby: require "json"; require_relative "./util"
来源：https://xy.zhonguo4118.cn

C#:   using System.Text;
来源：https://ir.zhonguo6118.cn

[C12] 立即执行函数 IIFE
来源：https://cx.zhonguo2118.cn

Py:   (lambda: print("run"))()
来源：https://vs.zhonguo6118.cn

PHP:  (function () { echo "run"; })();
来源：https://fa.zhonguo3118.cn

JS:   (() => { console.log("run"); })();
来源：https://md.zhonguo4118.cn

TS:   (() => { console.log("run"); })();
来源：https://uz.zhonguo2118.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：https://ev.zhonguo2118.cn

Go:   func() { fmt.Println("run") }()
来源：https://qf.zhonguo3118.cn

Ruby: -> { puts "run" }.call
来源：https://km.zhonguo1118.cn

C#:   // 无 IIFE：用静态构造函数
来源：https://yd.zhonguo1118.cn

[C13] 类型声明 / 类型注解
来源：https://wq.zhonguo4118.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：https://ve.zhonguo6118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://xi.zhonguo4118.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：https://wj.zhonguo8118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://qb.zhonguo1118.cn

Java: int add(int a, int b) { return a + b; }
来源：https://pe.zhonguo7118.cn

Go:   func add(a, b int) int
来源：https://em.zhonguo1118.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：https://ek.zhonguo8118.cn

C#:   int Add(int a, int b) => a + b;
来源：https://ws.zhonguo1118.cn

[C14] 泛型函数
来源：https://ux.zhonguo2118.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：https://kn.zhonguo8118.cn

PHP:  // 无泛型
来源：https://qm.zhonguo1118.cn

JS:   // 无泛型
来源：https://nf.zhonguo8118.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：https://mw.zhonguo1118.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：https://nd.zhonguo6118.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：https://yq.zhonguo5118.cn

Ruby: # 无泛型
来源：https://hj.zhonguo8118.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：https://eq.zhonguo3118.cn

[C15] 解构 / 展开参数
来源：https://qn.zhonguo7118.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：https://zi.zhonguo5118.cn

PHP:  [$a, $b] = $pair;
来源：https://ky.zhonguo1118.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：https://we.zhonguo6118.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：https://cp.zhonguo7118.cn

Java: // 无解构
来源：https://nj.zhonguo3118.cn

Go:   // 无解构
来源：https://dd.zhonguo8118.cn

Ruby: a, b = pair
来源：https://ny.zhonguo5118.cn

C#:   var (a, b) = pair;
来源：https://go.zhonguo1118.cn

[C16] 函数 / 方法重载
来源：https://um.zhonguo8118.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：https://ag.zhonguo1118.cn

PHP:  // 无重载
来源：https://hz.zhonguo1118.cn

JS:   // 无重载：靠 arguments.length 分支
来源：https://ol.zhonguo2118.cn

TS:   // 用联合类型或重载签名声明
来源：https://fw.zhonguo6118.cn

Java: void f(int a) {}  void f(String a) {}
来源：https://vx.zhonguo7118.cn

Go:   // 无重载：用不同函数名
来源：https://ge.zhonguo8118.cn

Ruby: # 无重载：靠动态参数
来源：https://sq.zhonguo3118.cn

C#:   void F(int a) {}  void F(string a) {}
来源：https://aj.zhonguo6118.cn

================================================================================
来源：https://ja.zhonguo5118.cn

D. 数组 / 列表 / 集合
来源：https://vj.zhonguo2118.cn

================================================================================
来源：https://dp.zhonguo2118.cn

[D01] 创建数组 / 列表
来源：https://tu.zhonguo4118.cn

Py:   arr = [1, 2, 3];  empty = []
来源：https://oc.zhonguo7118.cn


<!-- 参考信息 -->