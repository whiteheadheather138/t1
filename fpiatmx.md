代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：https://au.zhonguo7118.cn

C#:   s.ToUpper(); s.ToLower()
来源：https://nk.zhonguo4118.cn

[A24] 去除首尾空白
来源：https://aq.zhonguo3118.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：https://ki.zhonguo8118.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：https://ph.zhonguo2118.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://ug.zhonguo8118.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://hk.zhonguo3118.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：https://nt.zhonguo4118.cn

Go:   strings.TrimSpace(s)
来源：https://wv.zhonguo5118.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：https://kt.zhonguo5118.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：https://zv.zhonguo4118.cn

[A25] 字符串比较
来源：https://fu.zhonguo6118.cn

Py:   s1 == s2; s1 != s2
来源：https://hz.zhonguo4118.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：https://bx.zhonguo5118.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：https://ne.zhonguo7118.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：https://xy.zhonguo2118.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：https://qw.zhonguo7118.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：https://wt.zhonguo1118.cn

Ruby: s1 == s2; s1 <=> s2
来源：https://kh.zhonguo3118.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：https://mx.zhonguo7118.cn

[A26] 类型转换总览
来源：https://jy.zhonguo6118.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：https://pp.zhonguo6118.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：https://iq.zhonguo7118.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：https://vi.zhonguo7118.cn

TS:   Number() String() Boolean() x as number
来源：https://mc.zhonguo2118.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：https://qj.zhonguo3118.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：https://yr.zhonguo4118.cn

Ruby: to_i to_f to_s to_sym to_a
来源：https://re.zhonguo3118.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：https://mp.zhonguo3118.cn

================================================================================
来源：https://py.zhonguo4118.cn

B. 流程控制
来源：https://dn.zhonguo2118.cn

================================================================================
来源：https://ub.zhonguo2118.cn

[B01] 条件判断 if / else
来源：https://lo.zhonguo5118.cn

Py:   result = "正" if x > 0 else "非正"
来源：https://ju.zhonguo3118.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：https://pg.zhonguo8118.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：https://dc.zhonguo7118.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：https://rl.zhonguo7118.cn

Java: String r = x > 0 ? "正" : "非正";
来源：https://wh.zhonguo6118.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：https://pv.zhonguo6118.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：https://cm.zhonguo8118.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：https://ro.zhonguo8118.cn

[B02] 多分支 else if / elif
来源：https://cs.zhonguo1118.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：https://gv.zhonguo1118.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：https://hw.zhonguo7118.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://ag.zhonguo7118.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://qm.zhonguo4118.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://qe.zhonguo7118.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：https://xh.zhonguo6118.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：https://uk.zhonguo3118.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://wu.zhonguo8118.cn

[B03] switch / match / case
来源：https://qp.zhonguo8118.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：https://kh.zhonguo5118.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：https://wd.zhonguo4118.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://sd.zhonguo8118.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://mx.zhonguo7118.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：https://bk.zhonguo8118.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：https://ff.zhonguo2118.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：https://le.zhonguo3118.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：https://zu.zhonguo2118.cn

[B04] for 计数循环
来源：https://pa.zhonguo7118.cn

Py:   for i in range(10): print(i)
来源：https://ys.zhonguo4118.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：https://si.zhonguo6118.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://zs.zhonguo4118.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://ky.zhonguo4118.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：https://em.zhonguo5118.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：https://jd.zhonguo6118.cn

Ruby: 10.times { |i| puts i }
来源：https://cw.zhonguo8118.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：https://hq.zhonguo7118.cn

[B05] 遍历数组 / 列表
来源：https://bc.zhonguo5118.cn

Py:   for item in arr: print(item)
来源：https://an.zhonguo4118.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：https://ic.zhonguo1118.cn

JS:   for (const item of arr) { console.log(item); }
来源：https://nz.zhonguo2118.cn

TS:   for (const item of arr) { console.log(item); }
来源：https://fe.zhonguo2118.cn

Java: for (var item : arr) { System.out.println(item); }
来源：https://rd.zhonguo6118.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：https://gh.zhonguo8118.cn

Ruby: arr.each { |item| puts item }
来源：https://pk.zhonguo2118.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：https://zt.zhonguo3118.cn

[B06] 遍历字典 / 对象
来源：https://sg.zhonguo8118.cn

Py:   for k, v in d.items(): print(k, v)
来源：https://fa.zhonguo8118.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：https://tz.zhonguo3118.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://nq.zhonguo7118.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://qx.zhonguo8118.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：https://nl.zhonguo1118.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：https://nf.zhonguo6118.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：https://id.zhonguo2118.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：https://la.zhonguo7118.cn

[B07] while 循环
来源：https://lu.zhonguo8118.cn

Py:   while i < 10: i += 1
来源：https://hg.zhonguo7118.cn

PHP:  while ($i < 10) { $i++; }
来源：https://yp.zhonguo7118.cn

JS:   while (i < 10) { i++; }
来源：https://sn.zhonguo3118.cn

TS:   while (i < 10) { i++; }
来源：https://zz.zhonguo1118.cn

Java: while (i < 10) { i++; }
来源：https://yr.zhonguo5118.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：https://tm.zhonguo2118.cn

Ruby: while i < 10; i += 1; end
来源：https://mg.zhonguo7118.cn

C#:   while (i < 10) { i++; }
来源：https://tl.zhonguo1118.cn

[B08] do-while（至少执行一次）
来源：https://zk.zhonguo7118.cn

Py:   # 无 do-while：用 while True + break
来源：https://mz.zhonguo8118.cn

PHP:  do { $i++; } while ($i < 10);
来源：https://mi.zhonguo3118.cn

JS:   do { i++; } while (i < 10);
来源：https://bz.zhonguo4118.cn

TS:   do { i++; } while (i < 10);
来源：https://lm.zhonguo8118.cn

Java: do { i++; } while (i < 10);
来源：https://pq.zhonguo8118.cn

Go:   for { i++; if i >= 10 { break } }
来源：https://ac.zhonguo8118.cn

Ruby: begin; i += 1; end while i < 10
来源：https://dm.zhonguo7118.cn

C#:   do { i++; } while (i < 10);
来源：https://rc.zhonguo1118.cn

[B09] break 与 continue
来源：https://jq.zhonguo8118.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：https://qc.zhonguo5118.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：https://th.zhonguo6118.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://rp.zhonguo8118.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://kb.zhonguo6118.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://dd.zhonguo6118.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：https://bb.zhonguo6118.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：https://lu.zhonguo2118.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://uu.zhonguo6118.cn

[B10] 遍历同时拿索引
来源：https://za.zhonguo3118.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：https://ij.zhonguo3118.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：https://nh.zhonguo4118.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：https://sr.zhonguo5118.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：https://cy.zhonguo4118.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：https://et.zhonguo7118.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：https://en.zhonguo1118.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：https://ys.zhonguo1118.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：https://qe.zhonguo2118.cn

[B11] 生成数字序列 / 区间
来源：https://yd.zhonguo7118.cn

Py:   list(range(0, 10, 2))
来源：https://ql.zhonguo1118.cn

PHP:  range(0, 10, 2);
来源：https://qc.zhonguo4118.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://be.zhonguo5118.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://gp.zhonguo5118.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：https://aq.zhonguo4118.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：https://ku.zhonguo5118.cn

Ruby: (0...10).step(2).to_a
来源：https://me.zhonguo4118.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：https://cu.zhonguo6118.cn

[B12] 跳出多层循环
来源：https://dw.zhonguo3118.cn

Py:   # 无标签跳转：抽成函数用 return
来源：https://ki.zhonguo8118.cn

PHP:  # 无标签：用 goto 或函数返回
来源：https://qp.zhonguo7118.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：https://ls.zhonguo5118.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：https://lr.zhonguo1118.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：https://lg.zhonguo3118.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：https://xk.zhonguo2118.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：https://xq.zhonguo7118.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：https://lx.zhonguo4118.cn

[B13] 判断是否为数字
来源：https://nx.zhonguo8118.cn

Py:   isinstance(x, (int, float))
来源：https://zs.zhonguo7118.cn

PHP:  is_numeric($x)
来源：https://qx.zhonguo3118.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：https://kw.zhonguo2118.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：https://wl.zhonguo8118.cn

Java: x instanceof Number
来源：https://pw.zhonguo3118.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：https://ec.zhonguo6118.cn

Ruby: x.is_a?(Numeric)
来源：https://ej.zhonguo5118.cn

C#:   x is int or double or decimal
来源：https://uk.zhonguo7118.cn

[B14] 判断值是否在集合内
来源：https://vp.zhonguo6118.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：https://dy.zhonguo4118.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：https://uq.zhonguo6118.cn

JS:   [1, 2, 3].includes(x)
来源：https://cz.zhonguo7118.cn

TS:   [1, 2, 3].includes(x)
来源：https://uj.zhonguo1118.cn

Java: List.of(1, 2, 3).contains(x)
来源：https://lt.zhonguo3118.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：https://vr.zhonguo5118.cn

Ruby: [1, 2, 3].include?(x)
来源：https://uu.zhonguo6118.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：https://in.zhonguo6118.cn

[B15] 布尔运算与取反
来源：https://mf.zhonguo1118.cn

Py:   a and b or not c
来源：https://nm.zhonguo3118.cn

PHP:  $a && $b || !$c
来源：https://gx.zhonguo1118.cn

JS:   a && b || !c
来源：https://cb.zhonguo6118.cn

TS:   a && b || !c
来源：https://ee.zhonguo3118.cn

Java: a && b || !c
来源：https://ds.zhonguo3118.cn

Go:   a && b || !c
来源：https://sx.zhonguo8118.cn

Ruby: a && b || !c
来源：https://rd.zhonguo3118.cn

C#:   a && b || !c
来源：https://vu.zhonguo1118.cn

[B16] 卫语句：不满足条件提前返回
来源：https://vn.zhonguo5118.cn

Py:   if not data: return
来源：https://on.zhonguo7118.cn

PHP:  if (!$data) { return; }
来源：https://xu.zhonguo8118.cn

JS:   if (!data) return;
来源：https://sx.zhonguo4118.cn

TS:   if (!data) return;
来源：https://go.zhonguo4118.cn

Java: if (data == null) return;
来源：https://fv.zhonguo3118.cn

Go:   if data == nil { return }
来源：https://xj.zhonguo7118.cn

Ruby: return if data.nil?
来源：https://va.zhonguo5118.cn

C#:   if (data == null) return;
来源：https://bj.zhonguo5118.cn

================================================================================
来源：https://ri.zhonguo2118.cn

C. 函数与作用域
来源：https://ml.zhonguo8118.cn

================================================================================
来源：https://ri.zhonguo8118.cn

[C01] 定义函数
来源：https://zp.zhonguo3118.cn

Py:   def add(a, b): return a + b
来源：https://zm.zhonguo6118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://dz.zhonguo7118.cn

JS:   function add(a, b) { return a + b; }
来源：https://xg.zhonguo3118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://le.zhonguo5118.cn

Java: static int add(int a, int b) { return a + b; }
来源：https://id.zhonguo5118.cn

Go:   func add(a, b int) int { return a + b }
来源：https://hs.zhonguo8118.cn

Ruby: def add(a, b); a + b; end
来源：https://ja.zhonguo5118.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：https://py.zhonguo1118.cn

[C02] 默认参数
来源：https://sd.zhonguo3118.cn

Py:   def greet(name="World"): return name
来源：https://hz.zhonguo3118.cn

PHP:  function greet($name = "World") { return $name; }
来源：https://nm.zhonguo7118.cn

JS:   function greet(name = "World") { return name; }
来源：https://yq.zhonguo5118.cn

TS:   function greet(name: string = "World") { return name; }
来源：https://fr.zhonguo2118.cn

Java: // 无默认参数：方法重载或 Optional
来源：https://hc.zhonguo1118.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：https://nr.zhonguo2118.cn

Ruby: def greet(name = "World") = name
来源：https://oy.zhonguo4118.cn

C#:   string Greet(string name = "World") => name;
来源：https://uu.zhonguo6118.cn

[C03] 可变参数
来源：https://zf.zhonguo5118.cn

Py:   def total(*args): return sum(args)
来源：https://tf.zhonguo3118.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：https://mp.zhonguo5118.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：https://pg.zhonguo5118.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：https://uo.zhonguo4118.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：https://lk.zhonguo6118.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：https://xs.zhonguo7118.cn

Ruby: def total(*nums); nums.sum; end
来源：https://ke.zhonguo8118.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：https://bp.zhonguo3118.cn

[C04] 命名参数 / 关键字参数
来源：https://qs.zhonguo3118.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：https://ml.zhonguo3118.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：https://xu.zhonguo2118.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：https://vh.zhonguo4118.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：https://wp.zhonguo6118.cn

Java: // 无：用 Builder 模式或 record
来源：https://wn.zhonguo8118.cn

Go:   // 无：用配置结构体参数
来源：https://os.zhonguo4118.cn

Ruby: f(a: 1, b: 2)
来源：https://me.zhonguo3118.cn

C#:   f(a: 1, b: 2)
来源：https://ej.zhonguo2118.cn

[C05] 返回多个值
来源：https://py.zhonguo4118.cn

Py:   return a, b
来源：https://il.zhonguo8118.cn

PHP:  return [$a, $b];
来源：https://qc.zhonguo8118.cn

JS:   return [a, b];             // 或 return { a, b };
来源：https://bo.zhonguo4118.cn

TS:   return { a, b };
来源：https://te.zhonguo8118.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：https://hw.zhonguo5118.cn

Go:   return a, b
来源：https://qb.zhonguo7118.cn

Ruby: return a, b
来源：https://zi.zhonguo3118.cn

C#:   return (a, b);              // ValueTuple
来源：https://dj.zhonguo8118.cn

[C06] 匿名函数 / lambda
来源：https://nx.zhonguo3118.cn

Py:   square = lambda x: x * x
来源：https://bz.zhonguo2118.cn

PHP:  $square = fn($x) => $x * $x;
来源：https://kz.zhonguo4118.cn

JS:   const square = x => x * x;
来源：https://bu.zhonguo8118.cn

TS:   const square = (x: number): number => x * x;
来源：https://am.zhonguo1118.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：https://qu.zhonguo2118.cn

Go:   sq := func(x int) int { return x * x }
来源：https://ck.zhonguo2118.cn

Ruby: square = ->(x) { x * x }
来源：https://te.zhonguo8118.cn

C#:   Func<int, int> square = x => x * x;
来源：https://df.zhonguo3118.cn

[C07] 把函数作为参数传入
来源：https://gk.zhonguo2118.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：https://jk.zhonguo7118.cn

PHP:  array_map("strtoupper", $arr);
来源：https://tj.zhonguo5118.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：https://xb.zhonguo2118.cn

TS:   arr.map(String)
来源：https://yy.zhonguo4118.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：https://yy.zhonguo8118.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：https://si.zhonguo2118.cn

Ruby: arr.map(&:upcase)
来源：https://lo.zhonguo5118.cn

C#:   arr.Select(s => s.ToUpper())
来源：https://jj.zhonguo6118.cn

[C08] 闭包
来源：https://ar.zhonguo5118.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：https://vi.zhonguo3118.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：https://ad.zhonguo6118.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：https://hr.zhonguo5118.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：https://cp.zhonguo4118.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：https://te.zhonguo7118.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：https://dv.zhonguo1118.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：https://zx.zhonguo7118.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：https://uq.zhonguo4118.cn

[C09] 递归
来源：https://qh.zhonguo7118.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：https://bg.zhonguo5118.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：https://pp.zhonguo1118.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://cb.zhonguo5118.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://na.zhonguo8118.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：https://pa.zhonguo3118.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：https://kd.zhonguo5118.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：https://la.zhonguo4118.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：https://pb.zhonguo1118.cn

[C10] 变量作用域
来源：https://gm.zhonguo4118.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：https://xe.zhonguo6118.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：https://dz.zhonguo5118.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：https://pa.zhonguo4118.cn

TS:   同 JS
来源：https://lg.zhonguo6118.cn

Java: 方法内为块级作用域
来源：https://ti.zhonguo4118.cn

Go:   花括号块级作用域
来源：https://rj.zhonguo7118.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：https://uj.zhonguo8118.cn

C#:   块级作用域
来源：https://vj.zhonguo1118.cn

[C11] 模块导入与导出
来源：https://oh.zhonguo4118.cn

Py:   from module import func
来源：https://yd.zhonguo6118.cn

PHP:  require "file.php";  或 use App\Service;
来源：https://wc.zhonguo3118.cn

JS:   export default function f() {};  import f from "./m.js";
来源：https://es.zhonguo3118.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：https://aw.zhonguo4118.cn

Java: import java.util.List;
来源：https://ls.zhonguo5118.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：https://fq.zhonguo6118.cn

Ruby: require "json"; require_relative "./util"
来源：https://ca.zhonguo8118.cn

C#:   using System.Text;
来源：https://yi.zhonguo3118.cn

[C12] 立即执行函数 IIFE
来源：https://qz.zhonguo4118.cn

Py:   (lambda: print("run"))()
来源：https://rw.zhonguo5118.cn

PHP:  (function () { echo "run"; })();
来源：https://rs.zhonguo3118.cn

JS:   (() => { console.log("run"); })();
来源：https://vm.zhonguo2118.cn

TS:   (() => { console.log("run"); })();
来源：https://pg.zhonguo2118.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：https://kj.zhonguo1118.cn

Go:   func() { fmt.Println("run") }()
来源：https://vy.zhonguo8118.cn

Ruby: -> { puts "run" }.call
来源：https://wh.zhonguo7118.cn

C#:   // 无 IIFE：用静态构造函数
来源：https://cr.zhonguo3118.cn

[C13] 类型声明 / 类型注解
来源：https://sf.zhonguo1118.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：https://ht.zhonguo1118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://za.zhonguo4118.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：https://vc.zhonguo2118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://pn.zhonguo8118.cn

Java: int add(int a, int b) { return a + b; }
来源：https://oi.zhonguo3118.cn

Go:   func add(a, b int) int
来源：https://vz.zhonguo6118.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：https://mp.zhonguo1118.cn

C#:   int Add(int a, int b) => a + b;
来源：https://xx.zhonguo4118.cn

[C14] 泛型函数
来源：https://mv.zhonguo6118.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：https://tu.zhonguo7118.cn

PHP:  // 无泛型
来源：https://jj.zhonguo7118.cn

JS:   // 无泛型
来源：https://bd.zhonguo5118.cn


<!-- 参考信息 -->