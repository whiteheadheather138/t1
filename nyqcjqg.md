代发 wailian999

[B01] 条件判断 if / else
来源：https://or.zhonguo5118.cn

Py:   result = "正" if x > 0 else "非正"
来源：https://nw.zhonguo1118.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：https://xp.zhonguo5118.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：https://aw.zhonguo7118.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：https://tr.zhonguo7118.cn

Java: String r = x > 0 ? "正" : "非正";
来源：https://nq.zhonguo8118.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：https://sx.zhonguo8118.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：https://tb.zhonguo4118.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：https://wa.zhonguo3118.cn

[B02] 多分支 else if / elif
来源：https://zt.zhonguo3118.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：https://lw.zhonguo4118.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：https://ag.zhonguo6118.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://yv.zhonguo4118.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://tp.zhonguo4118.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://wv.zhonguo8118.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：https://ra.zhonguo8118.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：https://pa.zhonguo4118.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://ty.zhonguo8118.cn

[B03] switch / match / case
来源：https://rc.zhonguo2118.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：https://vs.zhonguo3118.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：https://ao.zhonguo8118.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://gq.zhonguo3118.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://hr.zhonguo2118.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：https://gf.zhonguo2118.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：https://ni.zhonguo2118.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：https://wl.zhonguo7118.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：https://xm.zhonguo4118.cn

[B04] for 计数循环
来源：https://ax.zhonguo1118.cn

Py:   for i in range(10): print(i)
来源：https://ta.zhonguo8118.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：https://dq.zhonguo3118.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://zg.zhonguo2118.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://hq.zhonguo1118.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：https://ze.zhonguo7118.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：https://wa.zhonguo8118.cn

Ruby: 10.times { |i| puts i }
来源：https://ez.zhonguo1118.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：https://zm.zhonguo1118.cn

[B05] 遍历数组 / 列表
来源：https://ov.zhonguo1118.cn

Py:   for item in arr: print(item)
来源：https://og.zhonguo2118.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：https://pk.zhonguo8118.cn

JS:   for (const item of arr) { console.log(item); }
来源：https://vi.zhonguo1118.cn

TS:   for (const item of arr) { console.log(item); }
来源：https://vj.zhonguo2118.cn

Java: for (var item : arr) { System.out.println(item); }
来源：https://kr.zhonguo1118.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：https://ok.zhonguo8118.cn

Ruby: arr.each { |item| puts item }
来源：https://pl.zhonguo3118.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：https://zc.zhonguo5118.cn

[B06] 遍历字典 / 对象
来源：https://kj.zhonguo3118.cn

Py:   for k, v in d.items(): print(k, v)
来源：https://ox.zhonguo8118.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：https://ln.zhonguo4118.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://ds.zhonguo6118.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://jw.zhonguo5118.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：https://mo.zhonguo8118.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：https://bb.zhonguo6118.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：https://rl.zhonguo7118.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：https://at.zhonguo5118.cn

[B07] while 循环
来源：https://cy.zhonguo2118.cn

Py:   while i < 10: i += 1
来源：https://mq.zhonguo6118.cn

PHP:  while ($i < 10) { $i++; }
来源：https://gw.zhonguo6118.cn

JS:   while (i < 10) { i++; }
来源：https://uh.zhonguo6118.cn

TS:   while (i < 10) { i++; }
来源：https://ke.zhonguo3118.cn

Java: while (i < 10) { i++; }
来源：https://uc.zhonguo1118.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：https://tk.zhonguo6118.cn

Ruby: while i < 10; i += 1; end
来源：https://le.zhonguo8118.cn

C#:   while (i < 10) { i++; }
来源：https://cl.zhonguo1118.cn

[B08] do-while（至少执行一次）
来源：https://wc.zhonguo3118.cn

Py:   # 无 do-while：用 while True + break
来源：https://or.zhonguo6118.cn

PHP:  do { $i++; } while ($i < 10);
来源：https://wa.zhonguo2118.cn

JS:   do { i++; } while (i < 10);
来源：https://rk.zhonguo5118.cn

TS:   do { i++; } while (i < 10);
来源：https://xv.zhonguo6118.cn

Java: do { i++; } while (i < 10);
来源：https://gi.zhonguo4118.cn

Go:   for { i++; if i >= 10 { break } }
来源：https://fd.zhonguo6118.cn

Ruby: begin; i += 1; end while i < 10
来源：https://dc.zhonguo3118.cn

C#:   do { i++; } while (i < 10);
来源：https://dd.zhonguo1118.cn

[B09] break 与 continue
来源：https://ld.zhonguo4118.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：https://hm.zhonguo2118.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：https://cl.zhonguo3118.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://eg.zhonguo7118.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://mp.zhonguo6118.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://dm.zhonguo8118.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：https://po.zhonguo6118.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：https://vz.zhonguo8118.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://qq.zhonguo4118.cn

[B10] 遍历同时拿索引
来源：https://gt.zhonguo8118.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：https://bx.zhonguo7118.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：https://tq.zhonguo7118.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：https://rk.zhonguo7118.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：https://xz.zhonguo8118.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：https://lk.zhonguo7118.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：https://re.zhonguo8118.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：https://uw.zhonguo5118.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：https://cd.zhonguo6118.cn

[B11] 生成数字序列 / 区间
来源：https://yu.zhonguo1118.cn

Py:   list(range(0, 10, 2))
来源：https://wb.zhonguo4118.cn

PHP:  range(0, 10, 2);
来源：https://bb.zhonguo6118.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://cc.zhonguo5118.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://at.zhonguo8118.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：https://bl.zhonguo7118.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：https://yc.zhonguo7118.cn

Ruby: (0...10).step(2).to_a
来源：https://oc.zhonguo5118.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：https://mu.zhonguo1118.cn

[B12] 跳出多层循环
来源：https://bp.zhonguo5118.cn

Py:   # 无标签跳转：抽成函数用 return
来源：https://bs.zhonguo8118.cn

PHP:  # 无标签：用 goto 或函数返回
来源：https://hl.zhonguo5118.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：https://kq.zhonguo1118.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：https://bo.zhonguo7118.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：https://dn.zhonguo5118.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：https://xf.zhonguo6118.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：https://pv.zhonguo2118.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：https://qu.zhonguo7118.cn

[B13] 判断是否为数字
来源：https://he.zhonguo6118.cn

Py:   isinstance(x, (int, float))
来源：https://ro.zhonguo8118.cn

PHP:  is_numeric($x)
来源：https://ih.zhonguo7118.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：https://zw.zhonguo5118.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：https://ae.zhonguo8118.cn

Java: x instanceof Number
来源：https://fq.zhonguo7118.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：https://lp.zhonguo4118.cn

Ruby: x.is_a?(Numeric)
来源：https://jr.zhonguo8118.cn

C#:   x is int or double or decimal
来源：https://ae.zhonguo4118.cn

[B14] 判断值是否在集合内
来源：https://qv.zhonguo3118.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：https://qa.zhonguo6118.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：https://tp.zhonguo4118.cn

JS:   [1, 2, 3].includes(x)
来源：https://nf.zhonguo1118.cn

TS:   [1, 2, 3].includes(x)
来源：https://be.zhonguo2118.cn

Java: List.of(1, 2, 3).contains(x)
来源：https://lh.zhonguo7118.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：https://vz.zhonguo7118.cn

Ruby: [1, 2, 3].include?(x)
来源：https://uq.zhonguo5118.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：https://av.zhonguo4118.cn

[B15] 布尔运算与取反
来源：https://kc.zhonguo1118.cn

Py:   a and b or not c
来源：https://yh.zhonguo5118.cn

PHP:  $a && $b || !$c
来源：https://hl.zhonguo5118.cn

JS:   a && b || !c
来源：https://av.zhonguo4118.cn

TS:   a && b || !c
来源：https://or.zhonguo1118.cn

Java: a && b || !c
来源：https://gz.zhonguo4118.cn

Go:   a && b || !c
来源：https://tu.zhonguo6118.cn

Ruby: a && b || !c
来源：https://hm.zhonguo1118.cn

C#:   a && b || !c
来源：https://zh.zhonguo4118.cn

[B16] 卫语句：不满足条件提前返回
来源：https://lb.zhonguo1118.cn

Py:   if not data: return
来源：https://lu.zhonguo1118.cn

PHP:  if (!$data) { return; }
来源：https://ix.zhonguo1118.cn

JS:   if (!data) return;
来源：https://df.zhonguo4118.cn

TS:   if (!data) return;
来源：https://pv.zhonguo7118.cn

Java: if (data == null) return;
来源：https://zd.zhonguo6118.cn

Go:   if data == nil { return }
来源：https://mi.zhonguo7118.cn

Ruby: return if data.nil?
来源：https://kw.zhonguo8118.cn

C#:   if (data == null) return;
来源：https://jd.zhonguo4118.cn

================================================================================
来源：https://rj.zhonguo5118.cn

C. 函数与作用域
来源：https://gl.zhonguo1118.cn

================================================================================
来源：https://if.zhonguo8118.cn

[C01] 定义函数
来源：https://pc.zhonguo6118.cn

Py:   def add(a, b): return a + b
来源：https://xe.zhonguo4118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://li.zhonguo7118.cn

JS:   function add(a, b) { return a + b; }
来源：https://gk.zhonguo7118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://vz.zhonguo4118.cn

Java: static int add(int a, int b) { return a + b; }
来源：https://cf.zhonguo6118.cn

Go:   func add(a, b int) int { return a + b }
来源：https://mu.zhonguo3118.cn

Ruby: def add(a, b); a + b; end
来源：https://rl.zhonguo5118.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：https://hu.zhonguo5118.cn

[C02] 默认参数
来源：https://nt.zhonguo4118.cn

Py:   def greet(name="World"): return name
来源：https://ey.zhonguo7118.cn

PHP:  function greet($name = "World") { return $name; }
来源：https://bc.zhonguo3118.cn

JS:   function greet(name = "World") { return name; }
来源：https://uw.zhonguo3118.cn

TS:   function greet(name: string = "World") { return name; }
来源：https://xa.zhonguo3118.cn

Java: // 无默认参数：方法重载或 Optional
来源：https://aa.zhonguo7118.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：https://ox.zhonguo2118.cn

Ruby: def greet(name = "World") = name
来源：https://xj.zhonguo3118.cn

C#:   string Greet(string name = "World") => name;
来源：https://uu.zhonguo8118.cn

[C03] 可变参数
来源：https://gp.zhonguo7118.cn

Py:   def total(*args): return sum(args)
来源：https://st.zhonguo6118.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：https://oy.zhonguo8118.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：https://gq.zhonguo5118.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：https://yx.zhonguo5118.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：https://rx.zhonguo6118.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：https://hv.zhonguo8118.cn

Ruby: def total(*nums); nums.sum; end
来源：https://cs.zhonguo4118.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：https://it.zhonguo6118.cn

[C04] 命名参数 / 关键字参数
来源：https://hu.zhonguo8118.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：https://wm.zhonguo2118.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：https://tz.zhonguo4118.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：https://yp.zhonguo6118.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：https://ij.zhonguo7118.cn

Java: // 无：用 Builder 模式或 record
来源：https://ys.zhonguo6118.cn

Go:   // 无：用配置结构体参数
来源：https://hc.zhonguo3118.cn

Ruby: f(a: 1, b: 2)
来源：https://zw.zhonguo1118.cn

C#:   f(a: 1, b: 2)
来源：https://bm.zhonguo3118.cn

[C05] 返回多个值
来源：https://jg.zhonguo5118.cn

Py:   return a, b
来源：https://fg.zhonguo7118.cn

PHP:  return [$a, $b];
来源：https://gz.zhonguo2118.cn

JS:   return [a, b];             // 或 return { a, b };
来源：https://zg.zhonguo1118.cn

TS:   return { a, b };
来源：https://xl.zhonguo1118.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：https://gz.zhonguo4118.cn

Go:   return a, b
来源：https://hb.zhonguo6118.cn

Ruby: return a, b
来源：https://ev.zhonguo8118.cn

C#:   return (a, b);              // ValueTuple
来源：https://eb.zhonguo6118.cn

[C06] 匿名函数 / lambda
来源：https://si.zhonguo8118.cn

Py:   square = lambda x: x * x
来源：https://fq.zhonguo2118.cn

PHP:  $square = fn($x) => $x * $x;
来源：https://dl.zhonguo8118.cn

JS:   const square = x => x * x;
来源：https://hf.zhonguo8118.cn

TS:   const square = (x: number): number => x * x;
来源：https://wn.zhonguo1118.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：https://ff.zhonguo2118.cn

Go:   sq := func(x int) int { return x * x }
来源：https://oz.zhonguo8118.cn

Ruby: square = ->(x) { x * x }
来源：https://sj.zhonguo1118.cn

C#:   Func<int, int> square = x => x * x;
来源：https://uc.zhonguo1118.cn

[C07] 把函数作为参数传入
来源：https://ci.zhonguo4118.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：https://md.zhonguo5118.cn

PHP:  array_map("strtoupper", $arr);
来源：https://kq.zhonguo6118.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：https://kl.zhonguo5118.cn

TS:   arr.map(String)
来源：https://vo.zhonguo8118.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：https://qk.zhonguo5118.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：https://zj.zhonguo6118.cn

Ruby: arr.map(&:upcase)
来源：https://wj.zhonguo2118.cn

C#:   arr.Select(s => s.ToUpper())
来源：https://xa.zhonguo6118.cn

[C08] 闭包
来源：https://nz.zhonguo6118.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：https://ky.zhonguo8118.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：https://ff.zhonguo5118.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：https://lt.zhonguo8118.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：https://io.zhonguo4118.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：https://jf.zhonguo7118.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：https://qc.zhonguo1118.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：https://xn.zhonguo1118.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：https://mu.zhonguo3118.cn

[C09] 递归
来源：https://gg.zhonguo1118.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：https://my.zhonguo5118.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：https://bh.zhonguo7118.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://cy.zhonguo8118.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://ex.zhonguo8118.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：https://tn.zhonguo2118.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：https://ft.zhonguo5118.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：https://na.zhonguo3118.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：https://ct.zhonguo8118.cn

[C10] 变量作用域
来源：https://cn.zhonguo5118.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：https://ao.zhonguo8118.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：https://px.zhonguo7118.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：https://gf.zhonguo8118.cn

TS:   同 JS
来源：https://vf.zhonguo3118.cn

Java: 方法内为块级作用域
来源：https://hf.zhonguo3118.cn

Go:   花括号块级作用域
来源：https://kc.zhonguo3118.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：https://jw.zhonguo4118.cn

C#:   块级作用域
来源：https://zd.zhonguo3118.cn

[C11] 模块导入与导出
来源：https://oc.zhonguo3118.cn

Py:   from module import func
来源：https://eo.zhonguo8118.cn

PHP:  require "file.php";  或 use App\Service;
来源：https://io.zhonguo5118.cn

JS:   export default function f() {};  import f from "./m.js";
来源：https://cq.zhonguo1118.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：https://vv.zhonguo7118.cn

Java: import java.util.List;
来源：https://gk.zhonguo1118.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：https://gp.zhonguo8118.cn

Ruby: require "json"; require_relative "./util"
来源：https://td.zhonguo6118.cn

C#:   using System.Text;
来源：https://gf.zhonguo5118.cn

[C12] 立即执行函数 IIFE
来源：https://kx.zhonguo8118.cn

Py:   (lambda: print("run"))()
来源：https://yq.zhonguo6118.cn

PHP:  (function () { echo "run"; })();
来源：https://qh.zhonguo3118.cn

JS:   (() => { console.log("run"); })();
来源：https://dm.zhonguo8118.cn

TS:   (() => { console.log("run"); })();
来源：https://my.zhonguo5118.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：https://qe.zhonguo1118.cn

Go:   func() { fmt.Println("run") }()
来源：https://lv.zhonguo2118.cn

Ruby: -> { puts "run" }.call
来源：https://vx.zhonguo8118.cn

C#:   // 无 IIFE：用静态构造函数
来源：https://qa.zhonguo1118.cn

[C13] 类型声明 / 类型注解
来源：https://rr.zhonguo1118.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：https://gx.zhonguo3118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://nw.zhonguo4118.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：https://vs.zhonguo2118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://sm.zhonguo2118.cn

Java: int add(int a, int b) { return a + b; }
来源：https://pp.zhonguo4118.cn

Go:   func add(a, b int) int
来源：https://oq.zhonguo1118.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：https://bj.zhonguo2118.cn

C#:   int Add(int a, int b) => a + b;
来源：https://bf.zhonguo8118.cn

[C14] 泛型函数
来源：https://gb.zhonguo1118.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：https://qi.zhonguo1118.cn

PHP:  // 无泛型
来源：https://om.zhonguo3118.cn

JS:   // 无泛型
来源：https://gn.zhonguo4118.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：https://zs.zhonguo3118.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：https://yw.zhonguo5118.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：https://vf.zhonguo2118.cn

Ruby: # 无泛型
来源：https://pu.zhonguo2118.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：https://fo.zhonguo6118.cn

[C15] 解构 / 展开参数
来源：https://en.zhonguo4118.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：https://lg.zhonguo7118.cn

PHP:  [$a, $b] = $pair;
来源：https://kv.zhonguo6118.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：https://eh.zhonguo6118.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：https://uz.zhonguo5118.cn

Java: // 无解构
来源：https://bn.zhonguo6118.cn

Go:   // 无解构
来源：https://sl.zhonguo5118.cn

Ruby: a, b = pair
来源：https://un.zhonguo4118.cn

C#:   var (a, b) = pair;
来源：https://im.zhonguo2118.cn

[C16] 函数 / 方法重载
来源：https://ej.zhonguo8118.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：https://od.zhonguo6118.cn

PHP:  // 无重载
来源：https://rn.zhonguo6118.cn

JS:   // 无重载：靠 arguments.length 分支
来源：https://iy.zhonguo6118.cn

TS:   // 用联合类型或重载签名声明
来源：https://df.zhonguo5118.cn

Java: void f(int a) {}  void f(String a) {}
来源：https://ti.zhonguo4118.cn

Go:   // 无重载：用不同函数名
来源：https://lv.zhonguo5118.cn

Ruby: # 无重载：靠动态参数
来源：https://ot.zhonguo1118.cn

C#:   void F(int a) {}  void F(string a) {}
来源：https://wv.zhonguo5118.cn

================================================================================
来源：https://xx.zhonguo5118.cn

D. 数组 / 列表 / 集合
来源：https://nn.zhonguo8118.cn

================================================================================
来源：https://ec.zhonguo1118.cn

[D01] 创建数组 / 列表
来源：https://zo.zhonguo2118.cn

Py:   arr = [1, 2, 3];  empty = []
来源：https://bx.zhonguo1118.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：https://dh.zhonguo5118.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：https://js.zhonguo8118.cn

TS:   const arr: number[] = [1, 2, 3];
来源：https://za.zhonguo1118.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：https://ld.zhonguo4118.cn


<!-- 参考信息 -->