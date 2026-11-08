代发 wailian999

JS:   [a, b] = [b, a];
来源：https://ko.zhonguo5118.cn

TS:   [a, b] = [b, a];
来源：https://oj.zhonguo5118.cn

Java: int t = a; a = b; b = t;
来源：https://gi.zhonguo7118.cn

Go:   a, b = b, a
来源：https://ee.zhonguo5118.cn

Ruby: a, b = b, a
来源：https://tb.zhonguo8118.cn

C#:   (a, b) = (b, a);
来源：https://hg.zhonguo6118.cn

[A20] 读取标准输入
来源：https://rz.zhonguo4118.cn

Py:   name = input("请输入：")
来源：https://si.zhonguo3118.cn

PHP:  $name = trim(fgets(STDIN));
来源：https://tm.zhonguo5118.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：https://qa.zhonguo2118.cn

TS:   // Node.js：readline 模块
来源：https://an.zhonguo4118.cn

Java: new Scanner(System.in).nextLine()
来源：https://sp.zhonguo8118.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：https://pu.zhonguo4118.cn

Ruby: gets.chomp
来源：https://bl.zhonguo1118.cn

C#:   Console.ReadLine();
来源：https://so.zhonguo4118.cn

[A21] 保留指定小数位输出
来源：https://hw.zhonguo5118.cn

Py:   f"{3.14159:.2f}"
来源：https://xu.zhonguo2118.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：https://ds.zhonguo5118.cn

JS:   (3.14159).toFixed(2)
来源：https://cd.zhonguo4118.cn

TS:   (3.14159).toFixed(2)
来源：https://ol.zhonguo4118.cn

Java: String.format("%.2f", 3.14159)
来源：https://id.zhonguo3118.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：https://fg.zhonguo1118.cn

Ruby: format("%.2f", 3.14159)
来源：https://ze.zhonguo3118.cn

C#:   3.14159.ToString("F2")
来源：https://qb.zhonguo7118.cn

[A22] 获取字符串长度
来源：https://sp.zhonguo3118.cn

Py:   len(s)
来源：https://xq.zhonguo5118.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：https://lq.zhonguo7118.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：https://xn.zhonguo1118.cn

TS:   s.length
来源：https://pt.zhonguo5118.cn

Java: s.length()
来源：https://wt.zhonguo2118.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：https://wr.zhonguo6118.cn

Ruby: s.length
来源：https://yf.zhonguo3118.cn

C#:   s.Length
来源：https://ow.zhonguo8118.cn

[A23] 大小写转换
来源：https://yk.zhonguo7118.cn

Py:   s.upper(); s.lower(); s.title()
来源：https://rd.zhonguo2118.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：https://sb.zhonguo7118.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：https://ha.zhonguo3118.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：https://yd.zhonguo3118.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：https://qe.zhonguo5118.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：https://wn.zhonguo7118.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：https://cl.zhonguo5118.cn

C#:   s.ToUpper(); s.ToLower()
来源：https://fl.zhonguo1118.cn

[A24] 去除首尾空白
来源：https://at.zhonguo3118.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：https://vv.zhonguo6118.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：https://vp.zhonguo3118.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://fv.zhonguo4118.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://ct.zhonguo8118.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：https://pi.zhonguo2118.cn

Go:   strings.TrimSpace(s)
来源：https://qt.zhonguo1118.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：https://cr.zhonguo7118.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：https://wf.zhonguo1118.cn

[A25] 字符串比较
来源：https://yt.zhonguo5118.cn

Py:   s1 == s2; s1 != s2
来源：https://nc.zhonguo2118.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：https://mi.zhonguo5118.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：https://gy.zhonguo6118.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：https://pa.zhonguo2118.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：https://rd.zhonguo5118.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：https://fi.zhonguo1118.cn

Ruby: s1 == s2; s1 <=> s2
来源：https://hw.zhonguo1118.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：https://wb.zhonguo4118.cn

[A26] 类型转换总览
来源：https://nu.zhonguo6118.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：https://bd.zhonguo7118.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：https://az.zhonguo6118.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：https://sc.zhonguo5118.cn

TS:   Number() String() Boolean() x as number
来源：https://xh.zhonguo7118.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：https://zv.zhonguo5118.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：https://mj.zhonguo4118.cn

Ruby: to_i to_f to_s to_sym to_a
来源：https://bb.zhonguo3118.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：https://kd.zhonguo8118.cn

================================================================================
来源：https://ib.zhonguo4118.cn

B. 流程控制
来源：https://af.zhonguo1118.cn

================================================================================
来源：https://rh.zhonguo8118.cn

[B01] 条件判断 if / else
来源：https://uo.zhonguo6118.cn

Py:   result = "正" if x > 0 else "非正"
来源：https://ou.zhonguo4118.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：https://nw.zhonguo6118.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：https://qg.zhonguo6118.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：https://lp.zhonguo6118.cn

Java: String r = x > 0 ? "正" : "非正";
来源：https://hy.zhonguo8118.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：https://oc.zhonguo7118.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：https://oo.zhonguo4118.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：https://ew.zhonguo1118.cn

[B02] 多分支 else if / elif
来源：https://my.zhonguo7118.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：https://tn.zhonguo1118.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：https://ih.zhonguo8118.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://ny.zhonguo4118.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://gj.zhonguo6118.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://qp.zhonguo2118.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：https://pg.zhonguo7118.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：https://cz.zhonguo7118.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://iz.zhonguo5118.cn

[B03] switch / match / case
来源：https://vl.zhonguo5118.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：https://bj.zhonguo6118.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：https://nx.zhonguo5118.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://dt.zhonguo5118.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://gi.zhonguo4118.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：https://nz.zhonguo8118.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：https://zx.zhonguo8118.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：https://wj.zhonguo6118.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：https://ox.zhonguo3118.cn

[B04] for 计数循环
来源：https://hy.zhonguo6118.cn

Py:   for i in range(10): print(i)
来源：https://ba.zhonguo7118.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：https://sf.zhonguo3118.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://su.zhonguo6118.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://im.zhonguo7118.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：https://xq.zhonguo3118.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：https://gb.zhonguo2118.cn

Ruby: 10.times { |i| puts i }
来源：https://yb.zhonguo7118.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：https://xl.zhonguo7118.cn

[B05] 遍历数组 / 列表
来源：https://wl.zhonguo8118.cn

Py:   for item in arr: print(item)
来源：https://vx.zhonguo8118.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：https://nt.zhonguo6118.cn

JS:   for (const item of arr) { console.log(item); }
来源：https://gf.zhonguo4118.cn

TS:   for (const item of arr) { console.log(item); }
来源：https://jj.zhonguo4118.cn

Java: for (var item : arr) { System.out.println(item); }
来源：https://hm.zhonguo3118.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：https://kd.zhonguo5118.cn

Ruby: arr.each { |item| puts item }
来源：https://kj.zhonguo7118.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：https://ui.zhonguo8118.cn

[B06] 遍历字典 / 对象
来源：https://ps.zhonguo5118.cn

Py:   for k, v in d.items(): print(k, v)
来源：https://ze.zhonguo7118.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：https://aa.zhonguo2118.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://xk.zhonguo5118.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://ui.zhonguo5118.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：https://ou.zhonguo7118.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：https://dn.zhonguo2118.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：https://tj.zhonguo2118.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：https://fv.zhonguo5118.cn

[B07] while 循环
来源：https://kr.zhonguo5118.cn

Py:   while i < 10: i += 1
来源：https://cd.zhonguo6118.cn

PHP:  while ($i < 10) { $i++; }
来源：https://sh.zhonguo1118.cn

JS:   while (i < 10) { i++; }
来源：https://jd.zhonguo2118.cn

TS:   while (i < 10) { i++; }
来源：https://xw.zhonguo3118.cn

Java: while (i < 10) { i++; }
来源：https://jk.zhonguo7118.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：https://mo.zhonguo7118.cn

Ruby: while i < 10; i += 1; end
来源：https://be.zhonguo8118.cn

C#:   while (i < 10) { i++; }
来源：https://qq.zhonguo1118.cn

[B08] do-while（至少执行一次）
来源：https://ym.zhonguo5118.cn

Py:   # 无 do-while：用 while True + break
来源：https://xh.zhonguo8118.cn

PHP:  do { $i++; } while ($i < 10);
来源：https://qr.zhonguo5118.cn

JS:   do { i++; } while (i < 10);
来源：https://xj.zhonguo6118.cn

TS:   do { i++; } while (i < 10);
来源：https://sq.zhonguo7118.cn

Java: do { i++; } while (i < 10);
来源：https://gq.zhonguo7118.cn

Go:   for { i++; if i >= 10 { break } }
来源：https://sb.zhonguo2118.cn

Ruby: begin; i += 1; end while i < 10
来源：https://ll.zhonguo8118.cn

C#:   do { i++; } while (i < 10);
来源：https://xk.zhonguo5118.cn

[B09] break 与 continue
来源：https://vm.zhonguo2118.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：https://rb.zhonguo1118.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：https://iu.zhonguo7118.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://cr.zhonguo5118.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://qo.zhonguo2118.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://sc.zhonguo3118.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：https://pm.zhonguo3118.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：https://nb.zhonguo7118.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://ib.zhonguo7118.cn

[B10] 遍历同时拿索引
来源：https://qi.zhonguo3118.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：https://cw.zhonguo6118.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：https://qv.zhonguo8118.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：https://gb.zhonguo2118.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：https://tj.zhonguo5118.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：https://im.zhonguo8118.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：https://vv.zhonguo7118.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：https://oc.zhonguo7118.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：https://fw.zhonguo2118.cn

[B11] 生成数字序列 / 区间
来源：https://km.zhonguo1118.cn

Py:   list(range(0, 10, 2))
来源：https://ob.zhonguo7118.cn

PHP:  range(0, 10, 2);
来源：https://lk.zhonguo7118.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://jt.zhonguo8118.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://rh.zhonguo8118.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：https://pv.zhonguo5118.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：https://bi.zhonguo8118.cn

Ruby: (0...10).step(2).to_a
来源：https://xd.zhonguo8118.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：https://ya.zhonguo6118.cn

[B12] 跳出多层循环
来源：https://ef.zhonguo5118.cn

Py:   # 无标签跳转：抽成函数用 return
来源：https://fo.zhonguo7118.cn

PHP:  # 无标签：用 goto 或函数返回
来源：https://tp.zhonguo5118.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：https://tz.zhonguo7118.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：https://mi.zhonguo7118.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：https://zw.zhonguo6118.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：https://md.zhonguo3118.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：https://oo.zhonguo6118.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：https://jw.zhonguo4118.cn

[B13] 判断是否为数字
来源：https://aa.zhonguo3118.cn

Py:   isinstance(x, (int, float))
来源：https://jc.zhonguo6118.cn

PHP:  is_numeric($x)
来源：https://kj.zhonguo7118.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：https://jn.zhonguo3118.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：https://oa.zhonguo5118.cn

Java: x instanceof Number
来源：https://hq.zhonguo3118.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：https://ur.zhonguo1118.cn

Ruby: x.is_a?(Numeric)
来源：https://dy.zhonguo2118.cn

C#:   x is int or double or decimal
来源：https://pv.zhonguo1118.cn

[B14] 判断值是否在集合内
来源：https://xi.zhonguo3118.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：https://ng.zhonguo8118.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：https://hb.zhonguo8118.cn

JS:   [1, 2, 3].includes(x)
来源：https://ke.zhonguo8118.cn

TS:   [1, 2, 3].includes(x)
来源：https://tx.zhonguo7118.cn

Java: List.of(1, 2, 3).contains(x)
来源：https://jh.zhonguo4118.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：https://qq.zhonguo5118.cn

Ruby: [1, 2, 3].include?(x)
来源：https://ku.zhonguo6118.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：https://ke.zhonguo8118.cn

[B15] 布尔运算与取反
来源：https://qe.zhonguo8118.cn

Py:   a and b or not c
来源：https://jc.zhonguo5118.cn

PHP:  $a && $b || !$c
来源：https://vs.zhonguo1118.cn

JS:   a && b || !c
来源：https://sw.zhonguo4118.cn

TS:   a && b || !c
来源：https://ps.zhonguo3118.cn

Java: a && b || !c
来源：https://bs.zhonguo8118.cn

Go:   a && b || !c
来源：https://bn.zhonguo4118.cn

Ruby: a && b || !c
来源：https://zw.zhonguo7118.cn

C#:   a && b || !c
来源：https://fk.zhonguo4118.cn

[B16] 卫语句：不满足条件提前返回
来源：https://rp.zhonguo2118.cn

Py:   if not data: return
来源：https://qf.zhonguo7118.cn

PHP:  if (!$data) { return; }
来源：https://dv.zhonguo2118.cn

JS:   if (!data) return;
来源：https://hr.zhonguo1118.cn

TS:   if (!data) return;
来源：https://oq.zhonguo3118.cn

Java: if (data == null) return;
来源：https://qt.zhonguo5118.cn

Go:   if data == nil { return }
来源：https://qk.zhonguo4118.cn

Ruby: return if data.nil?
来源：https://qz.zhonguo7118.cn

C#:   if (data == null) return;
来源：https://ou.zhonguo4118.cn

================================================================================
来源：https://gg.zhonguo5118.cn

C. 函数与作用域
来源：https://qr.zhonguo5118.cn

================================================================================
来源：https://ts.zhonguo2118.cn

[C01] 定义函数
来源：https://cv.zhonguo7118.cn

Py:   def add(a, b): return a + b
来源：https://lf.zhonguo4118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://gt.zhonguo1118.cn

JS:   function add(a, b) { return a + b; }
来源：https://aq.zhonguo2118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://jl.zhonguo6118.cn

Java: static int add(int a, int b) { return a + b; }
来源：https://dm.zhonguo6118.cn

Go:   func add(a, b int) int { return a + b }
来源：https://uf.zhonguo1118.cn

Ruby: def add(a, b); a + b; end
来源：https://jv.zhonguo6118.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：https://uy.zhonguo5118.cn

[C02] 默认参数
来源：https://uk.zhonguo8118.cn

Py:   def greet(name="World"): return name
来源：https://xg.zhonguo5118.cn

PHP:  function greet($name = "World") { return $name; }
来源：https://vg.zhonguo4118.cn

JS:   function greet(name = "World") { return name; }
来源：https://vn.zhonguo8118.cn

TS:   function greet(name: string = "World") { return name; }
来源：https://os.zhonguo8118.cn

Java: // 无默认参数：方法重载或 Optional
来源：https://ar.zhonguo4118.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：https://dy.zhonguo6118.cn

Ruby: def greet(name = "World") = name
来源：https://qf.zhonguo6118.cn

C#:   string Greet(string name = "World") => name;
来源：https://zc.zhonguo8118.cn

[C03] 可变参数
来源：https://qt.zhonguo4118.cn

Py:   def total(*args): return sum(args)
来源：https://rs.zhonguo1118.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：https://kn.zhonguo7118.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：https://jo.zhonguo1118.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：https://fq.zhonguo8118.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：https://ed.zhonguo5118.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：https://qj.zhonguo3118.cn

Ruby: def total(*nums); nums.sum; end
来源：https://ij.zhonguo3118.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：https://tw.zhonguo1118.cn

[C04] 命名参数 / 关键字参数
来源：https://pj.zhonguo4118.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：https://xc.zhonguo6118.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：https://zv.zhonguo1118.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：https://ay.zhonguo4118.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：https://lf.zhonguo2118.cn

Java: // 无：用 Builder 模式或 record
来源：https://qo.zhonguo3118.cn

Go:   // 无：用配置结构体参数
来源：https://wo.zhonguo3118.cn

Ruby: f(a: 1, b: 2)
来源：https://jm.zhonguo2118.cn

C#:   f(a: 1, b: 2)
来源：https://cm.zhonguo1118.cn

[C05] 返回多个值
来源：https://wa.zhonguo4118.cn

Py:   return a, b
来源：https://ss.zhonguo2118.cn

PHP:  return [$a, $b];
来源：https://hl.zhonguo6118.cn

JS:   return [a, b];             // 或 return { a, b };
来源：https://fz.zhonguo5118.cn

TS:   return { a, b };
来源：https://jm.zhonguo4118.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：https://oi.zhonguo6118.cn

Go:   return a, b
来源：https://yd.zhonguo2118.cn

Ruby: return a, b
来源：https://tx.zhonguo4118.cn

C#:   return (a, b);              // ValueTuple
来源：https://il.zhonguo6118.cn

[C06] 匿名函数 / lambda
来源：https://ap.zhonguo1118.cn

Py:   square = lambda x: x * x
来源：https://fw.zhonguo2118.cn

PHP:  $square = fn($x) => $x * $x;
来源：https://nl.zhonguo8118.cn

JS:   const square = x => x * x;
来源：https://xw.zhonguo4118.cn

TS:   const square = (x: number): number => x * x;
来源：https://gk.zhonguo2118.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：https://hq.zhonguo4118.cn

Go:   sq := func(x int) int { return x * x }
来源：https://gm.zhonguo2118.cn

Ruby: square = ->(x) { x * x }
来源：https://zy.zhonguo4118.cn

C#:   Func<int, int> square = x => x * x;
来源：https://sg.zhonguo7118.cn

[C07] 把函数作为参数传入
来源：https://ze.zhonguo2118.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：https://us.zhonguo8118.cn

PHP:  array_map("strtoupper", $arr);
来源：https://xy.zhonguo7118.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：https://bm.zhonguo8118.cn

TS:   arr.map(String)
来源：https://ks.zhonguo1118.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：https://rc.zhonguo7118.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：https://uj.zhonguo2118.cn

Ruby: arr.map(&:upcase)
来源：https://oo.zhonguo2118.cn

C#:   arr.Select(s => s.ToUpper())
来源：https://wo.zhonguo4118.cn

[C08] 闭包
来源：https://oz.zhonguo6118.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：https://dl.zhonguo3118.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：https://ko.zhonguo6118.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：https://kt.zhonguo7118.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：https://yo.zhonguo7118.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：https://oy.zhonguo5118.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：https://nx.zhonguo1118.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：https://or.zhonguo1118.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：https://qm.zhonguo1118.cn

[C09] 递归
来源：https://my.zhonguo1118.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：https://wb.zhonguo7118.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：https://vy.zhonguo5118.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://ic.zhonguo7118.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://zk.zhonguo5118.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：https://rf.zhonguo8118.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：https://af.zhonguo2118.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：https://ss.zhonguo3118.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：https://ym.zhonguo6118.cn


<!-- 参考信息 -->