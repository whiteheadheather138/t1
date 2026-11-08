代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：https://gm.zhonguo7118.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：https://ks.zhonguo7118.cn

Ruby: format("%.2f", 3.14159)
来源：https://hk.zhonguo5118.cn

C#:   3.14159.ToString("F2")
来源：https://al.zhonguo2118.cn

[A22] 获取字符串长度
来源：https://wa.zhonguo3118.cn

Py:   len(s)
来源：https://dp.zhonguo1118.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：https://gg.zhonguo4118.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：https://te.zhonguo7118.cn

TS:   s.length
来源：https://md.zhonguo1118.cn

Java: s.length()
来源：https://hb.zhonguo4118.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：https://an.zhonguo6118.cn

Ruby: s.length
来源：https://ru.zhonguo5118.cn

C#:   s.Length
来源：https://fi.zhonguo4118.cn

[A23] 大小写转换
来源：https://cw.zhonguo5118.cn

Py:   s.upper(); s.lower(); s.title()
来源：https://zz.zhonguo8118.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：https://px.zhonguo2118.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：https://av.zhonguo8118.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：https://kb.zhonguo3118.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：https://ba.zhonguo6118.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：https://zy.zhonguo7118.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：https://sc.zhonguo5118.cn

C#:   s.ToUpper(); s.ToLower()
来源：https://tk.zhonguo6118.cn

[A24] 去除首尾空白
来源：https://rk.zhonguo3118.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：https://qe.zhonguo3118.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：https://na.zhonguo2118.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://qi.zhonguo1118.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://bc.zhonguo2118.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：https://xa.zhonguo2118.cn

Go:   strings.TrimSpace(s)
来源：https://hy.zhonguo5118.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：https://ku.zhonguo4118.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：https://wd.zhonguo7118.cn

[A25] 字符串比较
来源：https://tf.zhonguo5118.cn

Py:   s1 == s2; s1 != s2
来源：https://yx.zhonguo2118.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：https://qd.zhonguo7118.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：https://zi.zhonguo4118.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：https://jq.zhonguo6118.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：https://yy.zhonguo7118.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：https://ci.zhonguo8118.cn

Ruby: s1 == s2; s1 <=> s2
来源：https://vr.zhonguo3118.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：https://dk.zhonguo1118.cn

[A26] 类型转换总览
来源：https://ea.zhonguo2118.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：https://aq.zhonguo6118.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：https://aq.zhonguo5118.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：https://mi.zhonguo1118.cn

TS:   Number() String() Boolean() x as number
来源：https://fo.zhonguo2118.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：https://lw.zhonguo8118.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：https://go.zhonguo1118.cn

Ruby: to_i to_f to_s to_sym to_a
来源：https://wo.zhonguo2118.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：https://qv.zhonguo8118.cn

================================================================================
来源：https://cz.zhonguo4118.cn

B. 流程控制
来源：https://ju.zhonguo8118.cn

================================================================================
来源：https://ul.zhonguo2118.cn

[B01] 条件判断 if / else
来源：https://vm.zhonguo6118.cn

Py:   result = "正" if x > 0 else "非正"
来源：https://ex.zhonguo1118.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：https://ro.zhonguo1118.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：https://yu.zhonguo2118.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：https://hd.zhonguo4118.cn

Java: String r = x > 0 ? "正" : "非正";
来源：https://tz.zhonguo1118.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：https://xw.zhonguo7118.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：https://ty.zhonguo1118.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：https://za.zhonguo1118.cn

[B02] 多分支 else if / elif
来源：https://tx.zhonguo3118.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：https://sy.zhonguo5118.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：https://jt.zhonguo3118.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://us.zhonguo3118.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://iy.zhonguo6118.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://aj.zhonguo6118.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：https://kz.zhonguo5118.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：https://yg.zhonguo3118.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://gd.zhonguo3118.cn

[B03] switch / match / case
来源：https://mh.zhonguo4118.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：https://rj.zhonguo4118.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：https://uu.zhonguo6118.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://cr.zhonguo5118.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://cg.zhonguo5118.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：https://ls.zhonguo1118.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：https://yo.zhonguo8118.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：https://bp.zhonguo7118.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：https://hm.zhonguo1118.cn

[B04] for 计数循环
来源：https://fy.zhonguo6118.cn

Py:   for i in range(10): print(i)
来源：https://si.zhonguo3118.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：https://vh.zhonguo6118.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://lt.zhonguo7118.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://ph.zhonguo3118.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：https://on.zhonguo7118.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：https://zh.zhonguo4118.cn

Ruby: 10.times { |i| puts i }
来源：https://cq.zhonguo3118.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：https://ee.zhonguo4118.cn

[B05] 遍历数组 / 列表
来源：https://tr.zhonguo4118.cn

Py:   for item in arr: print(item)
来源：https://pp.zhonguo4118.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：https://nd.zhonguo4118.cn

JS:   for (const item of arr) { console.log(item); }
来源：https://qr.zhonguo2118.cn

TS:   for (const item of arr) { console.log(item); }
来源：https://xg.zhonguo5118.cn

Java: for (var item : arr) { System.out.println(item); }
来源：https://wz.zhonguo8118.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：https://oo.zhonguo1118.cn

Ruby: arr.each { |item| puts item }
来源：https://uy.zhonguo7118.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：https://yb.zhonguo1118.cn

[B06] 遍历字典 / 对象
来源：https://dt.zhonguo6118.cn

Py:   for k, v in d.items(): print(k, v)
来源：https://yk.zhonguo3118.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：https://da.zhonguo6118.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://wp.zhonguo5118.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://we.zhonguo7118.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：https://zl.zhonguo3118.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：https://dw.zhonguo6118.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：https://ax.zhonguo3118.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：https://xv.zhonguo6118.cn

[B07] while 循环
来源：https://oo.zhonguo1118.cn

Py:   while i < 10: i += 1
来源：https://th.zhonguo2118.cn

PHP:  while ($i < 10) { $i++; }
来源：https://nd.zhonguo3118.cn

JS:   while (i < 10) { i++; }
来源：https://qm.zhonguo1118.cn

TS:   while (i < 10) { i++; }
来源：https://bd.zhonguo2118.cn

Java: while (i < 10) { i++; }
来源：https://fj.zhonguo6118.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：https://kt.zhonguo5118.cn

Ruby: while i < 10; i += 1; end
来源：https://yi.zhonguo6118.cn

C#:   while (i < 10) { i++; }
来源：https://fo.zhonguo5118.cn

[B08] do-while（至少执行一次）
来源：https://dd.zhonguo6118.cn

Py:   # 无 do-while：用 while True + break
来源：https://xk.zhonguo5118.cn

PHP:  do { $i++; } while ($i < 10);
来源：https://jb.zhonguo7118.cn

JS:   do { i++; } while (i < 10);
来源：https://xc.zhonguo3118.cn

TS:   do { i++; } while (i < 10);
来源：https://zf.zhonguo2118.cn

Java: do { i++; } while (i < 10);
来源：https://re.zhonguo4118.cn

Go:   for { i++; if i >= 10 { break } }
来源：https://iz.zhonguo7118.cn

Ruby: begin; i += 1; end while i < 10
来源：https://ge.zhonguo2118.cn

C#:   do { i++; } while (i < 10);
来源：https://ls.zhonguo1118.cn

[B09] break 与 continue
来源：https://nc.zhonguo6118.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：https://ws.zhonguo3118.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：https://pt.zhonguo7118.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://ol.zhonguo7118.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://bd.zhonguo6118.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://nw.zhonguo8118.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：https://oc.zhonguo5118.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：https://ki.zhonguo3118.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://be.zhonguo6118.cn

[B10] 遍历同时拿索引
来源：https://pf.zhonguo3118.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：https://cd.zhonguo7118.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：https://xv.zhonguo5118.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：https://li.zhonguo1118.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：https://lk.zhonguo8118.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：https://ta.zhonguo6118.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：https://co.zhonguo1118.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：https://qm.zhonguo5118.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：https://mx.zhonguo3118.cn

[B11] 生成数字序列 / 区间
来源：https://lf.zhonguo4118.cn

Py:   list(range(0, 10, 2))
来源：https://bo.zhonguo4118.cn

PHP:  range(0, 10, 2);
来源：https://uo.zhonguo5118.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://tp.zhonguo3118.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://ui.zhonguo6118.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：https://eg.zhonguo2118.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：https://pe.zhonguo7118.cn

Ruby: (0...10).step(2).to_a
来源：https://kf.zhonguo2118.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：https://uu.zhonguo7118.cn

[B12] 跳出多层循环
来源：https://gp.zhonguo5118.cn

Py:   # 无标签跳转：抽成函数用 return
来源：https://pv.zhonguo7118.cn

PHP:  # 无标签：用 goto 或函数返回
来源：https://ra.zhonguo7118.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：https://hf.zhonguo3118.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：https://pk.zhonguo7118.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：https://uz.zhonguo1118.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：https://ia.zhonguo2118.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：https://tx.zhonguo2118.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：https://ul.zhonguo7118.cn

[B13] 判断是否为数字
来源：https://si.zhonguo5118.cn

Py:   isinstance(x, (int, float))
来源：https://xs.zhonguo8118.cn

PHP:  is_numeric($x)
来源：https://ik.zhonguo6118.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：https://yc.zhonguo5118.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：https://te.zhonguo2118.cn

Java: x instanceof Number
来源：https://rn.zhonguo3118.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：https://pj.zhonguo5118.cn

Ruby: x.is_a?(Numeric)
来源：https://ys.zhonguo8118.cn

C#:   x is int or double or decimal
来源：https://vf.zhonguo2118.cn

[B14] 判断值是否在集合内
来源：https://vn.zhonguo3118.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：https://pr.zhonguo6118.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：https://rg.zhonguo5118.cn

JS:   [1, 2, 3].includes(x)
来源：https://na.zhonguo8118.cn

TS:   [1, 2, 3].includes(x)
来源：https://pm.zhonguo2118.cn

Java: List.of(1, 2, 3).contains(x)
来源：https://zu.zhonguo2118.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：https://ov.zhonguo8118.cn

Ruby: [1, 2, 3].include?(x)
来源：https://nr.zhonguo7118.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：https://uj.zhonguo3118.cn

[B15] 布尔运算与取反
来源：https://zv.zhonguo8118.cn

Py:   a and b or not c
来源：https://pt.zhonguo2118.cn

PHP:  $a && $b || !$c
来源：https://de.zhonguo2118.cn

JS:   a && b || !c
来源：https://ru.zhonguo1118.cn

TS:   a && b || !c
来源：https://mv.zhonguo7118.cn

Java: a && b || !c
来源：https://fw.zhonguo5118.cn

Go:   a && b || !c
来源：https://yr.zhonguo8118.cn

Ruby: a && b || !c
来源：https://wq.zhonguo3118.cn

C#:   a && b || !c
来源：https://ws.zhonguo2118.cn

[B16] 卫语句：不满足条件提前返回
来源：https://bn.zhonguo8118.cn

Py:   if not data: return
来源：https://iy.zhonguo2118.cn

PHP:  if (!$data) { return; }
来源：https://uu.zhonguo1118.cn

JS:   if (!data) return;
来源：https://rw.zhonguo1118.cn

TS:   if (!data) return;
来源：https://us.zhonguo4118.cn

Java: if (data == null) return;
来源：https://up.zhonguo3118.cn

Go:   if data == nil { return }
来源：https://uh.zhonguo1118.cn

Ruby: return if data.nil?
来源：https://km.zhonguo6118.cn

C#:   if (data == null) return;
来源：https://dt.zhonguo3118.cn

================================================================================
来源：https://ks.zhonguo3118.cn

C. 函数与作用域
来源：https://kh.zhonguo3118.cn

================================================================================
来源：https://ic.zhonguo6118.cn

[C01] 定义函数
来源：https://fq.zhonguo5118.cn

Py:   def add(a, b): return a + b
来源：https://nj.zhonguo6118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://ry.zhonguo7118.cn

JS:   function add(a, b) { return a + b; }
来源：https://kh.zhonguo2118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://qp.zhonguo1118.cn

Java: static int add(int a, int b) { return a + b; }
来源：https://op.zhonguo3118.cn

Go:   func add(a, b int) int { return a + b }
来源：https://eu.zhonguo1118.cn

Ruby: def add(a, b); a + b; end
来源：https://oo.zhonguo8118.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：https://le.zhonguo8118.cn

[C02] 默认参数
来源：https://ae.zhonguo4118.cn

Py:   def greet(name="World"): return name
来源：https://jb.zhonguo8118.cn

PHP:  function greet($name = "World") { return $name; }
来源：https://pu.zhonguo1118.cn

JS:   function greet(name = "World") { return name; }
来源：https://dp.zhonguo3118.cn

TS:   function greet(name: string = "World") { return name; }
来源：https://ih.zhonguo3118.cn

Java: // 无默认参数：方法重载或 Optional
来源：https://br.zhonguo6118.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：https://ib.zhonguo4118.cn

Ruby: def greet(name = "World") = name
来源：https://df.zhonguo7118.cn

C#:   string Greet(string name = "World") => name;
来源：https://vc.zhonguo1118.cn

[C03] 可变参数
来源：https://uv.zhonguo2118.cn

Py:   def total(*args): return sum(args)
来源：https://wu.zhonguo8118.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：https://ug.zhonguo2118.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：https://ni.zhonguo4118.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：https://jx.zhonguo8118.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：https://nr.zhonguo6118.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：https://ei.zhonguo7118.cn

Ruby: def total(*nums); nums.sum; end
来源：https://ac.zhonguo4118.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：https://tl.zhonguo7118.cn

[C04] 命名参数 / 关键字参数
来源：https://ba.zhonguo6118.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：https://js.zhonguo7118.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：https://rb.zhonguo6118.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：https://mv.zhonguo5118.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：https://yb.zhonguo1118.cn

Java: // 无：用 Builder 模式或 record
来源：https://je.zhonguo8118.cn

Go:   // 无：用配置结构体参数
来源：https://vd.zhonguo3118.cn

Ruby: f(a: 1, b: 2)
来源：https://me.zhonguo3118.cn

C#:   f(a: 1, b: 2)
来源：https://zs.zhonguo1118.cn

[C05] 返回多个值
来源：https://fs.zhonguo6118.cn

Py:   return a, b
来源：https://fc.zhonguo3118.cn

PHP:  return [$a, $b];
来源：https://jk.zhonguo1118.cn

JS:   return [a, b];             // 或 return { a, b };
来源：https://dt.zhonguo8118.cn

TS:   return { a, b };
来源：https://cd.zhonguo4118.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：https://dq.zhonguo2118.cn

Go:   return a, b
来源：https://uh.zhonguo3118.cn

Ruby: return a, b
来源：https://hk.zhonguo5118.cn

C#:   return (a, b);              // ValueTuple
来源：https://lu.zhonguo8118.cn

[C06] 匿名函数 / lambda
来源：https://iz.zhonguo6118.cn

Py:   square = lambda x: x * x
来源：https://dp.zhonguo7118.cn

PHP:  $square = fn($x) => $x * $x;
来源：https://hb.zhonguo1118.cn

JS:   const square = x => x * x;
来源：https://sx.zhonguo6118.cn

TS:   const square = (x: number): number => x * x;
来源：https://ij.zhonguo3118.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：https://yi.zhonguo6118.cn

Go:   sq := func(x int) int { return x * x }
来源：https://kn.zhonguo5118.cn

Ruby: square = ->(x) { x * x }
来源：https://ct.zhonguo6118.cn

C#:   Func<int, int> square = x => x * x;
来源：https://qp.zhonguo1118.cn

[C07] 把函数作为参数传入
来源：https://fe.zhonguo3118.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：https://jt.zhonguo3118.cn

PHP:  array_map("strtoupper", $arr);
来源：https://qx.zhonguo2118.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：https://fq.zhonguo1118.cn

TS:   arr.map(String)
来源：https://nf.zhonguo1118.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：https://vx.zhonguo3118.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：https://lk.zhonguo1118.cn

Ruby: arr.map(&:upcase)
来源：https://jw.zhonguo4118.cn

C#:   arr.Select(s => s.ToUpper())
来源：https://hv.zhonguo4118.cn

[C08] 闭包
来源：https://us.zhonguo4118.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：https://vm.zhonguo1118.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：https://pt.zhonguo2118.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：https://jd.zhonguo7118.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：https://bs.zhonguo8118.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：https://zj.zhonguo7118.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：https://hd.zhonguo8118.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：https://lu.zhonguo6118.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：https://dn.zhonguo1118.cn

[C09] 递归
来源：https://rd.zhonguo6118.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：https://wg.zhonguo3118.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：https://ws.zhonguo2118.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://kc.zhonguo2118.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://xb.zhonguo7118.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：https://kd.zhonguo4118.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：https://ry.zhonguo1118.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：https://dt.zhonguo8118.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：https://xe.zhonguo8118.cn

[C10] 变量作用域
来源：https://gq.zhonguo4118.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：https://kj.zhonguo1118.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：https://px.zhonguo3118.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：https://jb.zhonguo8118.cn

TS:   同 JS
来源：https://uh.zhonguo3118.cn

Java: 方法内为块级作用域
来源：https://dd.zhonguo2118.cn

Go:   花括号块级作用域
来源：https://zu.zhonguo8118.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：https://bl.zhonguo1118.cn

C#:   块级作用域
来源：https://dn.zhonguo4118.cn

[C11] 模块导入与导出
来源：https://mq.zhonguo2118.cn

Py:   from module import func
来源：https://gr.zhonguo1118.cn

PHP:  require "file.php";  或 use App\Service;
来源：https://vk.zhonguo6118.cn

JS:   export default function f() {};  import f from "./m.js";
来源：https://mr.zhonguo5118.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：https://jy.zhonguo1118.cn

Java: import java.util.List;
来源：https://wi.zhonguo5118.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：https://it.zhonguo2118.cn

Ruby: require "json"; require_relative "./util"
来源：https://gj.zhonguo7118.cn

C#:   using System.Text;
来源：https://ph.zhonguo6118.cn

[C12] 立即执行函数 IIFE
来源：https://tm.zhonguo7118.cn

Py:   (lambda: print("run"))()
来源：https://mr.zhonguo1118.cn


<!-- 参考信息 -->