代发 wailian999

Py:   s1 == s2; s1 != s2
来源：https://di.zhonguo5118.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：https://qo.zhonguo8118.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：https://ob.zhonguo6118.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：https://ty.zhonguo8118.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：https://zd.zhonguo7118.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：https://fn.zhonguo3118.cn

Ruby: s1 == s2; s1 <=> s2
来源：https://ns.zhonguo6118.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：https://sm.zhonguo5118.cn

[A26] 类型转换总览
来源：https://bh.zhonguo7118.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：https://fg.zhonguo7118.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：https://dh.zhonguo2118.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：https://xf.zhonguo5118.cn

TS:   Number() String() Boolean() x as number
来源：https://qu.zhonguo1118.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：https://wo.zhonguo3118.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：https://vi.zhonguo1118.cn

Ruby: to_i to_f to_s to_sym to_a
来源：https://mq.zhonguo3118.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：https://qz.zhonguo1118.cn

================================================================================
来源：https://hd.zhonguo8118.cn

B. 流程控制
来源：https://qd.zhonguo6118.cn

================================================================================
来源：https://yl.zhonguo2118.cn

[B01] 条件判断 if / else
来源：https://bn.zhonguo2118.cn

Py:   result = "正" if x > 0 else "非正"
来源：https://ov.zhonguo1118.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：https://xo.zhonguo2118.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：https://so.zhonguo1118.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：https://ff.zhonguo3118.cn

Java: String r = x > 0 ? "正" : "非正";
来源：https://nr.zhonguo5118.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：https://tr.zhonguo2118.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：https://fk.zhonguo8118.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：https://rv.zhonguo8118.cn

[B02] 多分支 else if / elif
来源：https://jq.zhonguo7118.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：https://cm.zhonguo6118.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：https://lf.zhonguo8118.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://ad.zhonguo7118.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://wo.zhonguo6118.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://ab.zhonguo7118.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：https://tr.zhonguo5118.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：https://wg.zhonguo1118.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://wg.zhonguo1118.cn

[B03] switch / match / case
来源：https://pa.zhonguo7118.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：https://sm.zhonguo2118.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：https://ar.zhonguo7118.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://kb.zhonguo7118.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://ej.zhonguo5118.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：https://yv.zhonguo4118.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：https://ii.zhonguo4118.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：https://xr.zhonguo7118.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：https://nz.zhonguo4118.cn

[B04] for 计数循环
来源：https://mb.zhonguo6118.cn

Py:   for i in range(10): print(i)
来源：https://hg.zhonguo8118.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：https://an.zhonguo3118.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://up.zhonguo7118.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://em.zhonguo7118.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：https://rq.zhonguo7118.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：https://aq.zhonguo7118.cn

Ruby: 10.times { |i| puts i }
来源：https://ee.zhonguo5118.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：https://xl.zhonguo4118.cn

[B05] 遍历数组 / 列表
来源：https://wq.zhonguo4118.cn

Py:   for item in arr: print(item)
来源：https://zc.zhonguo8118.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：https://pe.zhonguo6118.cn

JS:   for (const item of arr) { console.log(item); }
来源：https://np.zhonguo3118.cn

TS:   for (const item of arr) { console.log(item); }
来源：https://rn.zhonguo7118.cn

Java: for (var item : arr) { System.out.println(item); }
来源：https://xn.zhonguo3118.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：https://gw.zhonguo3118.cn

Ruby: arr.each { |item| puts item }
来源：https://rq.zhonguo2118.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：https://gv.zhonguo5118.cn

[B06] 遍历字典 / 对象
来源：https://sr.zhonguo8118.cn

Py:   for k, v in d.items(): print(k, v)
来源：https://eo.zhonguo6118.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：https://dd.zhonguo7118.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://kb.zhonguo7118.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://cp.zhonguo5118.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：https://mm.zhonguo8118.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：https://un.zhonguo5118.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：https://yp.zhonguo4118.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：https://mh.zhonguo4118.cn

[B07] while 循环
来源：https://mc.zhonguo8118.cn

Py:   while i < 10: i += 1
来源：https://gh.zhonguo3118.cn

PHP:  while ($i < 10) { $i++; }
来源：https://bf.zhonguo3118.cn

JS:   while (i < 10) { i++; }
来源：https://vc.zhonguo5118.cn

TS:   while (i < 10) { i++; }
来源：https://dl.zhonguo2118.cn

Java: while (i < 10) { i++; }
来源：https://vf.zhonguo2118.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：https://pn.zhonguo4118.cn

Ruby: while i < 10; i += 1; end
来源：https://py.zhonguo4118.cn

C#:   while (i < 10) { i++; }
来源：https://kn.zhonguo6118.cn

[B08] do-while（至少执行一次）
来源：https://ql.zhonguo3118.cn

Py:   # 无 do-while：用 while True + break
来源：https://rb.zhonguo3118.cn

PHP:  do { $i++; } while ($i < 10);
来源：https://ja.zhonguo6118.cn

JS:   do { i++; } while (i < 10);
来源：https://sm.zhonguo4118.cn

TS:   do { i++; } while (i < 10);
来源：https://it.zhonguo8118.cn

Java: do { i++; } while (i < 10);
来源：https://hj.zhonguo8118.cn

Go:   for { i++; if i >= 10 { break } }
来源：https://jz.zhonguo8118.cn

Ruby: begin; i += 1; end while i < 10
来源：https://cq.zhonguo3118.cn

C#:   do { i++; } while (i < 10);
来源：https://be.zhonguo3118.cn

[B09] break 与 continue
来源：https://fo.zhonguo7118.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：https://wu.zhonguo7118.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：https://kh.zhonguo4118.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://jm.zhonguo7118.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://dr.zhonguo6118.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://qz.zhonguo2118.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：https://nk.zhonguo5118.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：https://oa.zhonguo4118.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://kv.zhonguo4118.cn

[B10] 遍历同时拿索引
来源：https://eu.zhonguo2118.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：https://ug.zhonguo5118.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：https://fq.zhonguo4118.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：https://vg.zhonguo2118.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：https://fe.zhonguo4118.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：https://nc.zhonguo7118.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：https://mb.zhonguo1118.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：https://ic.zhonguo5118.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：https://ag.zhonguo7118.cn

[B11] 生成数字序列 / 区间
来源：https://ei.zhonguo1118.cn

Py:   list(range(0, 10, 2))
来源：https://zi.zhonguo5118.cn

PHP:  range(0, 10, 2);
来源：https://gl.zhonguo6118.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://kb.zhonguo1118.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://xf.zhonguo3118.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：https://fk.zhonguo2118.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：https://xq.zhonguo3118.cn

Ruby: (0...10).step(2).to_a
来源：https://pi.zhonguo4118.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：https://so.zhonguo4118.cn

[B12] 跳出多层循环
来源：https://qd.zhonguo5118.cn

Py:   # 无标签跳转：抽成函数用 return
来源：https://bx.zhonguo4118.cn

PHP:  # 无标签：用 goto 或函数返回
来源：https://kg.zhonguo5118.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：https://zw.zhonguo7118.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：https://lr.zhonguo4118.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：https://xh.zhonguo2118.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：https://xn.zhonguo3118.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：https://el.zhonguo1118.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：https://kv.zhonguo4118.cn

[B13] 判断是否为数字
来源：https://ws.zhonguo8118.cn

Py:   isinstance(x, (int, float))
来源：https://br.zhonguo4118.cn

PHP:  is_numeric($x)
来源：https://pt.zhonguo3118.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：https://kh.zhonguo5118.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：https://wr.zhonguo3118.cn

Java: x instanceof Number
来源：https://vo.zhonguo8118.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：https://th.zhonguo4118.cn

Ruby: x.is_a?(Numeric)
来源：https://mr.zhonguo6118.cn

C#:   x is int or double or decimal
来源：https://rj.zhonguo6118.cn

[B14] 判断值是否在集合内
来源：https://kh.zhonguo4118.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：https://on.zhonguo6118.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：https://th.zhonguo2118.cn

JS:   [1, 2, 3].includes(x)
来源：https://wg.zhonguo2118.cn

TS:   [1, 2, 3].includes(x)
来源：https://en.zhonguo1118.cn

Java: List.of(1, 2, 3).contains(x)
来源：https://tl.zhonguo3118.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：https://cm.zhonguo5118.cn

Ruby: [1, 2, 3].include?(x)
来源：https://at.zhonguo1118.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：https://qr.zhonguo1118.cn

[B15] 布尔运算与取反
来源：https://tc.zhonguo4118.cn

Py:   a and b or not c
来源：https://mf.zhonguo3118.cn

PHP:  $a && $b || !$c
来源：https://gc.zhonguo8118.cn

JS:   a && b || !c
来源：https://hu.zhonguo2118.cn

TS:   a && b || !c
来源：https://ry.zhonguo3118.cn

Java: a && b || !c
来源：https://si.zhonguo1118.cn

Go:   a && b || !c
来源：https://ge.zhonguo8118.cn

Ruby: a && b || !c
来源：https://ok.zhonguo2118.cn

C#:   a && b || !c
来源：https://lj.zhonguo7118.cn

[B16] 卫语句：不满足条件提前返回
来源：https://hk.zhonguo6118.cn

Py:   if not data: return
来源：https://gr.zhonguo5118.cn

PHP:  if (!$data) { return; }
来源：https://hh.zhonguo5118.cn

JS:   if (!data) return;
来源：https://gf.zhonguo1118.cn

TS:   if (!data) return;
来源：https://mb.zhonguo4118.cn

Java: if (data == null) return;
来源：https://kv.zhonguo4118.cn

Go:   if data == nil { return }
来源：https://ws.zhonguo3118.cn

Ruby: return if data.nil?
来源：https://sr.zhonguo8118.cn

C#:   if (data == null) return;
来源：https://tx.zhonguo2118.cn

================================================================================
来源：https://hn.zhonguo7118.cn

C. 函数与作用域
来源：https://re.zhonguo2118.cn

================================================================================
来源：https://re.zhonguo5118.cn

[C01] 定义函数
来源：https://qv.zhonguo8118.cn

Py:   def add(a, b): return a + b
来源：https://se.zhonguo5118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://kz.zhonguo5118.cn

JS:   function add(a, b) { return a + b; }
来源：https://wa.zhonguo7118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://za.zhonguo3118.cn

Java: static int add(int a, int b) { return a + b; }
来源：https://la.zhonguo8118.cn

Go:   func add(a, b int) int { return a + b }
来源：https://rz.zhonguo2118.cn

Ruby: def add(a, b); a + b; end
来源：https://zv.zhonguo4118.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：https://xx.zhonguo8118.cn

[C02] 默认参数
来源：https://jp.zhonguo3118.cn

Py:   def greet(name="World"): return name
来源：https://pp.zhonguo2118.cn

PHP:  function greet($name = "World") { return $name; }
来源：https://rt.zhonguo2118.cn

JS:   function greet(name = "World") { return name; }
来源：https://fy.zhonguo2118.cn

TS:   function greet(name: string = "World") { return name; }
来源：https://bc.zhonguo4118.cn

Java: // 无默认参数：方法重载或 Optional
来源：https://ew.zhonguo3118.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：https://bd.zhonguo5118.cn

Ruby: def greet(name = "World") = name
来源：https://zt.zhonguo1118.cn

C#:   string Greet(string name = "World") => name;
来源：https://we.zhonguo8118.cn

[C03] 可变参数
来源：https://ae.zhonguo6118.cn

Py:   def total(*args): return sum(args)
来源：https://ty.zhonguo6118.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：https://uo.zhonguo4118.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：https://dq.zhonguo2118.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：https://yc.zhonguo3118.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：https://ak.zhonguo7118.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：https://dd.zhonguo6118.cn

Ruby: def total(*nums); nums.sum; end
来源：https://oe.zhonguo2118.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：https://hh.zhonguo6118.cn

[C04] 命名参数 / 关键字参数
来源：https://er.zhonguo5118.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：https://vx.zhonguo1118.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：https://wm.zhonguo1118.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：https://nb.zhonguo1118.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：https://vd.zhonguo4118.cn

Java: // 无：用 Builder 模式或 record
来源：https://wh.zhonguo4118.cn

Go:   // 无：用配置结构体参数
来源：https://xd.zhonguo7118.cn

Ruby: f(a: 1, b: 2)
来源：https://ws.zhonguo6118.cn

C#:   f(a: 1, b: 2)
来源：https://cx.zhonguo5118.cn

[C05] 返回多个值
来源：https://hr.zhonguo5118.cn

Py:   return a, b
来源：https://yo.zhonguo1118.cn

PHP:  return [$a, $b];
来源：https://cl.zhonguo6118.cn

JS:   return [a, b];             // 或 return { a, b };
来源：https://uo.zhonguo7118.cn

TS:   return { a, b };
来源：https://od.zhonguo3118.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：https://vd.zhonguo4118.cn

Go:   return a, b
来源：https://ug.zhonguo7118.cn

Ruby: return a, b
来源：https://ap.zhonguo4118.cn

C#:   return (a, b);              // ValueTuple
来源：https://yt.zhonguo7118.cn

[C06] 匿名函数 / lambda
来源：https://rx.zhonguo8118.cn

Py:   square = lambda x: x * x
来源：https://ks.zhonguo3118.cn

PHP:  $square = fn($x) => $x * $x;
来源：https://wq.zhonguo4118.cn

JS:   const square = x => x * x;
来源：https://xx.zhonguo7118.cn

TS:   const square = (x: number): number => x * x;
来源：https://ay.zhonguo4118.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：https://jl.zhonguo4118.cn

Go:   sq := func(x int) int { return x * x }
来源：https://qt.zhonguo6118.cn

Ruby: square = ->(x) { x * x }
来源：https://jt.zhonguo8118.cn

C#:   Func<int, int> square = x => x * x;
来源：https://ay.zhonguo7118.cn

[C07] 把函数作为参数传入
来源：https://lq.zhonguo5118.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：https://uc.zhonguo3118.cn

PHP:  array_map("strtoupper", $arr);
来源：https://so.zhonguo5118.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：https://ad.zhonguo2118.cn

TS:   arr.map(String)
来源：https://ko.zhonguo5118.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：https://uo.zhonguo6118.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：https://zs.zhonguo8118.cn

Ruby: arr.map(&:upcase)
来源：https://tg.zhonguo4118.cn

C#:   arr.Select(s => s.ToUpper())
来源：https://dx.zhonguo1118.cn

[C08] 闭包
来源：https://zx.zhonguo2118.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：https://nl.zhonguo4118.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：https://rg.zhonguo2118.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：https://rm.zhonguo5118.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：https://sq.zhonguo4118.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：https://xs.zhonguo2118.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：https://pa.zhonguo4118.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：https://xy.zhonguo5118.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：https://tn.zhonguo7118.cn

[C09] 递归
来源：https://gy.zhonguo3118.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：https://sc.zhonguo1118.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：https://uc.zhonguo8118.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://wz.zhonguo7118.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://ie.zhonguo8118.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：https://ft.zhonguo1118.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：https://cc.zhonguo2118.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：https://de.zhonguo6118.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：https://zf.zhonguo3118.cn

[C10] 变量作用域
来源：https://vd.zhonguo7118.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：https://ge.zhonguo5118.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：https://xl.zhonguo2118.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：https://xj.zhonguo3118.cn

TS:   同 JS
来源：https://ye.zhonguo5118.cn

Java: 方法内为块级作用域
来源：https://mc.zhonguo7118.cn

Go:   花括号块级作用域
来源：https://pq.zhonguo7118.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：https://jh.zhonguo4118.cn

C#:   块级作用域
来源：https://xz.zhonguo7118.cn

[C11] 模块导入与导出
来源：https://vp.zhonguo4118.cn

Py:   from module import func
来源：https://az.zhonguo3118.cn

PHP:  require "file.php";  或 use App\Service;
来源：https://ha.zhonguo7118.cn

JS:   export default function f() {};  import f from "./m.js";
来源：https://pb.zhonguo3118.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：https://ki.zhonguo7118.cn

Java: import java.util.List;
来源：https://ao.zhonguo1118.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：https://yc.zhonguo2118.cn

Ruby: require "json"; require_relative "./util"
来源：https://at.zhonguo5118.cn

C#:   using System.Text;
来源：https://xg.zhonguo6118.cn

[C12] 立即执行函数 IIFE
来源：https://gs.zhonguo3118.cn

Py:   (lambda: print("run"))()
来源：https://jr.zhonguo8118.cn

PHP:  (function () { echo "run"; })();
来源：https://lh.zhonguo4118.cn

JS:   (() => { console.log("run"); })();
来源：https://io.zhonguo8118.cn

TS:   (() => { console.log("run"); })();
来源：https://ka.zhonguo7118.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：https://gk.zhonguo8118.cn

Go:   func() { fmt.Println("run") }()
来源：https://yt.zhonguo3118.cn

Ruby: -> { puts "run" }.call
来源：https://wi.zhonguo1118.cn

C#:   // 无 IIFE：用静态构造函数
来源：https://kz.zhonguo6118.cn

[C13] 类型声明 / 类型注解
来源：https://ps.zhonguo1118.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：https://rv.zhonguo5118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://ay.zhonguo5118.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：https://sn.zhonguo3118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://uv.zhonguo5118.cn

Java: int add(int a, int b) { return a + b; }
来源：https://yu.zhonguo4118.cn

Go:   func add(a, b int) int
来源：https://yx.zhonguo7118.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：https://xa.zhonguo7118.cn

C#:   int Add(int a, int b) => a + b;
来源：https://et.zhonguo5118.cn

[C14] 泛型函数
来源：https://eg.zhonguo3118.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：https://fn.zhonguo2118.cn

PHP:  // 无泛型
来源：https://fh.zhonguo2118.cn

JS:   // 无泛型
来源：https://qw.zhonguo1118.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：https://db.zhonguo3118.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：https://zx.zhonguo1118.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：https://ax.zhonguo6118.cn

Ruby: # 无泛型
来源：https://uw.zhonguo4118.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：https://qu.zhonguo5118.cn

[C15] 解构 / 展开参数
来源：https://yw.zhonguo5118.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：https://eg.zhonguo8118.cn

PHP:  [$a, $b] = $pair;
来源：https://gd.zhonguo7118.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：https://wa.zhonguo4118.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：https://ap.zhonguo2118.cn

Java: // 无解构
来源：https://mr.zhonguo7118.cn

Go:   // 无解构
来源：https://aq.zhonguo3118.cn


<!-- 参考信息 -->