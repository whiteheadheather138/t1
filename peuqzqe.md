代发 wailian999

C#:   (int)'A'; (char)65
来源：https://cy.zhonguo7118.cn

[A19] 交换两个变量
来源：https://sc.zhonguo1118.cn

Py:   a, b = b, a
来源：https://xu.zhonguo4118.cn

PHP:  [$a, $b] = [$b, $a];
来源：https://dy.zhonguo7118.cn

JS:   [a, b] = [b, a];
来源：https://pp.zhonguo1118.cn

TS:   [a, b] = [b, a];
来源：https://oa.zhonguo1118.cn

Java: int t = a; a = b; b = t;
来源：https://wv.zhonguo8118.cn

Go:   a, b = b, a
来源：https://ks.zhonguo2118.cn

Ruby: a, b = b, a
来源：https://aa.zhonguo8118.cn

C#:   (a, b) = (b, a);
来源：https://jq.zhonguo7118.cn

[A20] 读取标准输入
来源：https://me.zhonguo8118.cn

Py:   name = input("请输入：")
来源：https://vn.zhonguo5118.cn

PHP:  $name = trim(fgets(STDIN));
来源：https://ev.zhonguo1118.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：https://tm.zhonguo7118.cn

TS:   // Node.js：readline 模块
来源：https://px.zhonguo7118.cn

Java: new Scanner(System.in).nextLine()
来源：https://eg.zhonguo1118.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：https://au.zhonguo1118.cn

Ruby: gets.chomp
来源：https://cr.zhonguo7118.cn

C#:   Console.ReadLine();
来源：https://cy.zhonguo3118.cn

[A21] 保留指定小数位输出
来源：https://yh.zhonguo8118.cn

Py:   f"{3.14159:.2f}"
来源：https://bx.zhonguo8118.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：https://nq.zhonguo7118.cn

JS:   (3.14159).toFixed(2)
来源：https://jx.zhonguo4118.cn

TS:   (3.14159).toFixed(2)
来源：https://yx.zhonguo4118.cn

Java: String.format("%.2f", 3.14159)
来源：https://tg.zhonguo5118.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：https://nk.zhonguo1118.cn

Ruby: format("%.2f", 3.14159)
来源：https://by.zhonguo5118.cn

C#:   3.14159.ToString("F2")
来源：https://ni.zhonguo5118.cn

[A22] 获取字符串长度
来源：https://cm.zhonguo5118.cn

Py:   len(s)
来源：https://nh.zhonguo6118.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：https://gt.zhonguo7118.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：https://rv.zhonguo5118.cn

TS:   s.length
来源：https://lq.zhonguo7118.cn

Java: s.length()
来源：https://ly.zhonguo6118.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：https://xl.zhonguo2118.cn

Ruby: s.length
来源：https://rh.zhonguo2118.cn

C#:   s.Length
来源：https://oa.zhonguo1118.cn

[A23] 大小写转换
来源：https://qx.zhonguo4118.cn

Py:   s.upper(); s.lower(); s.title()
来源：https://fr.zhonguo6118.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：https://hu.zhonguo4118.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：https://bh.zhonguo2118.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：https://on.zhonguo3118.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：https://oj.zhonguo5118.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：https://my.zhonguo1118.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：https://ht.zhonguo8118.cn

C#:   s.ToUpper(); s.ToLower()
来源：https://lb.zhonguo3118.cn

[A24] 去除首尾空白
来源：https://rg.zhonguo5118.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：https://iw.zhonguo5118.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：https://fx.zhonguo6118.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://ua.zhonguo6118.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://er.zhonguo5118.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：https://oc.zhonguo3118.cn

Go:   strings.TrimSpace(s)
来源：https://fd.zhonguo5118.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：https://fs.zhonguo3118.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：https://rs.zhonguo4118.cn

[A25] 字符串比较
来源：https://yn.zhonguo2118.cn

Py:   s1 == s2; s1 != s2
来源：https://cm.zhonguo1118.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：https://lg.zhonguo6118.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：https://yt.zhonguo6118.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：https://xb.zhonguo3118.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：https://op.zhonguo1118.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：https://of.zhonguo4118.cn

Ruby: s1 == s2; s1 <=> s2
来源：https://fg.zhonguo8118.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：https://fp.zhonguo1118.cn

[A26] 类型转换总览
来源：https://yx.zhonguo2118.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：https://nu.zhonguo2118.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：https://fd.zhonguo2118.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：https://ff.zhonguo1118.cn

TS:   Number() String() Boolean() x as number
来源：https://ka.zhonguo3118.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：https://cr.zhonguo8118.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：https://nn.zhonguo5118.cn

Ruby: to_i to_f to_s to_sym to_a
来源：https://ib.zhonguo2118.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：https://or.zhonguo4118.cn

================================================================================
来源：https://au.zhonguo8118.cn

B. 流程控制
来源：https://cl.zhonguo6118.cn

================================================================================
来源：https://fx.zhonguo7118.cn

[B01] 条件判断 if / else
来源：https://co.zhonguo3118.cn

Py:   result = "正" if x > 0 else "非正"
来源：https://qf.zhonguo5118.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：https://za.zhonguo4118.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：https://pi.zhonguo4118.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：https://nt.zhonguo1118.cn

Java: String r = x > 0 ? "正" : "非正";
来源：https://nz.zhonguo7118.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：https://jh.zhonguo8118.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：https://cl.zhonguo6118.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：https://oi.zhonguo7118.cn

[B02] 多分支 else if / elif
来源：https://by.zhonguo6118.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：https://ya.zhonguo4118.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：https://xv.zhonguo5118.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://th.zhonguo5118.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://vm.zhonguo1118.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://ak.zhonguo8118.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：https://br.zhonguo1118.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：https://qm.zhonguo1118.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://nx.zhonguo3118.cn

[B03] switch / match / case
来源：https://mb.zhonguo6118.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：https://zw.zhonguo2118.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：https://cl.zhonguo2118.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://xg.zhonguo4118.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://qp.zhonguo3118.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：https://xu.zhonguo5118.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：https://gf.zhonguo6118.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：https://tu.zhonguo6118.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：https://zi.zhonguo1118.cn

[B04] for 计数循环
来源：https://bk.zhonguo2118.cn

Py:   for i in range(10): print(i)
来源：https://cu.zhonguo4118.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：https://gi.zhonguo4118.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://yh.zhonguo2118.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://hs.zhonguo3118.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：https://ab.zhonguo6118.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：https://xj.zhonguo2118.cn

Ruby: 10.times { |i| puts i }
来源：https://vt.zhonguo6118.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：https://np.zhonguo8118.cn

[B05] 遍历数组 / 列表
来源：https://oh.zhonguo4118.cn

Py:   for item in arr: print(item)
来源：https://pp.zhonguo1118.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：https://yd.zhonguo1118.cn

JS:   for (const item of arr) { console.log(item); }
来源：https://aa.zhonguo6118.cn

TS:   for (const item of arr) { console.log(item); }
来源：https://yv.zhonguo6118.cn

Java: for (var item : arr) { System.out.println(item); }
来源：https://ht.zhonguo3118.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：https://xf.zhonguo1118.cn

Ruby: arr.each { |item| puts item }
来源：https://yp.zhonguo1118.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：https://gi.zhonguo7118.cn

[B06] 遍历字典 / 对象
来源：https://jc.zhonguo5118.cn

Py:   for k, v in d.items(): print(k, v)
来源：https://ch.zhonguo2118.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：https://ml.zhonguo2118.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://ru.zhonguo1118.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://bp.zhonguo5118.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：https://ob.zhonguo5118.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：https://yh.zhonguo7118.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：https://tt.zhonguo4118.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：https://gp.zhonguo6118.cn

[B07] while 循环
来源：https://ku.zhonguo5118.cn

Py:   while i < 10: i += 1
来源：https://bl.zhonguo6118.cn

PHP:  while ($i < 10) { $i++; }
来源：https://jp.zhonguo5118.cn

JS:   while (i < 10) { i++; }
来源：https://xe.zhonguo6118.cn

TS:   while (i < 10) { i++; }
来源：https://dt.zhonguo5118.cn

Java: while (i < 10) { i++; }
来源：https://eb.zhonguo2118.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：https://pe.zhonguo3118.cn

Ruby: while i < 10; i += 1; end
来源：https://ft.zhonguo3118.cn

C#:   while (i < 10) { i++; }
来源：https://pl.zhonguo4118.cn

[B08] do-while（至少执行一次）
来源：https://bb.zhonguo8118.cn

Py:   # 无 do-while：用 while True + break
来源：https://ql.zhonguo2118.cn

PHP:  do { $i++; } while ($i < 10);
来源：https://oj.zhonguo6118.cn

JS:   do { i++; } while (i < 10);
来源：https://bi.zhonguo7118.cn

TS:   do { i++; } while (i < 10);
来源：https://dn.zhonguo7118.cn

Java: do { i++; } while (i < 10);
来源：https://iu.zhonguo8118.cn

Go:   for { i++; if i >= 10 { break } }
来源：https://oi.zhonguo4118.cn

Ruby: begin; i += 1; end while i < 10
来源：https://bj.zhonguo4118.cn

C#:   do { i++; } while (i < 10);
来源：https://ta.zhonguo3118.cn

[B09] break 与 continue
来源：https://pg.zhonguo7118.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：https://uo.zhonguo3118.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：https://hy.zhonguo7118.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://fd.zhonguo8118.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://nk.zhonguo5118.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://oq.zhonguo2118.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：https://ps.zhonguo1118.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：https://jz.zhonguo2118.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://qi.zhonguo4118.cn

[B10] 遍历同时拿索引
来源：https://br.zhonguo4118.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：https://qd.zhonguo7118.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：https://ju.zhonguo3118.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：https://jk.zhonguo3118.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：https://km.zhonguo7118.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：https://vl.zhonguo5118.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：https://tk.zhonguo3118.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：https://js.zhonguo6118.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：https://ns.zhonguo3118.cn

[B11] 生成数字序列 / 区间
来源：https://xg.zhonguo1118.cn

Py:   list(range(0, 10, 2))
来源：https://ps.zhonguo3118.cn

PHP:  range(0, 10, 2);
来源：https://fc.zhonguo3118.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://ar.zhonguo7118.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://oz.zhonguo7118.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：https://no.zhonguo1118.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：https://hj.zhonguo1118.cn

Ruby: (0...10).step(2).to_a
来源：https://es.zhonguo5118.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：https://zz.zhonguo1118.cn

[B12] 跳出多层循环
来源：https://zg.zhonguo8118.cn

Py:   # 无标签跳转：抽成函数用 return
来源：https://is.zhonguo2118.cn

PHP:  # 无标签：用 goto 或函数返回
来源：https://jm.zhonguo2118.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：https://ov.zhonguo6118.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：https://gt.zhonguo5118.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：https://ri.zhonguo1118.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：https://cq.zhonguo3118.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：https://ri.zhonguo7118.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：https://ft.zhonguo4118.cn

[B13] 判断是否为数字
来源：https://zm.zhonguo2118.cn

Py:   isinstance(x, (int, float))
来源：https://we.zhonguo7118.cn

PHP:  is_numeric($x)
来源：https://vg.zhonguo3118.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：https://se.zhonguo1118.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：https://zg.zhonguo2118.cn

Java: x instanceof Number
来源：https://im.zhonguo5118.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：https://gy.zhonguo4118.cn

Ruby: x.is_a?(Numeric)
来源：https://am.zhonguo7118.cn

C#:   x is int or double or decimal
来源：https://lu.zhonguo7118.cn

[B14] 判断值是否在集合内
来源：https://ew.zhonguo6118.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：https://cj.zhonguo5118.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：https://im.zhonguo6118.cn

JS:   [1, 2, 3].includes(x)
来源：https://hc.zhonguo8118.cn

TS:   [1, 2, 3].includes(x)
来源：https://lu.zhonguo4118.cn

Java: List.of(1, 2, 3).contains(x)
来源：https://cr.zhonguo8118.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：https://ml.zhonguo1118.cn

Ruby: [1, 2, 3].include?(x)
来源：https://io.zhonguo8118.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：https://gu.zhonguo7118.cn

[B15] 布尔运算与取反
来源：https://rc.zhonguo7118.cn

Py:   a and b or not c
来源：https://ad.zhonguo3118.cn

PHP:  $a && $b || !$c
来源：https://zh.zhonguo7118.cn

JS:   a && b || !c
来源：https://ht.zhonguo3118.cn

TS:   a && b || !c
来源：https://gq.zhonguo6118.cn

Java: a && b || !c
来源：https://uq.zhonguo4118.cn

Go:   a && b || !c
来源：https://rv.zhonguo4118.cn

Ruby: a && b || !c
来源：https://od.zhonguo7118.cn

C#:   a && b || !c
来源：https://oo.zhonguo6118.cn

[B16] 卫语句：不满足条件提前返回
来源：https://no.zhonguo3118.cn

Py:   if not data: return
来源：https://ms.zhonguo8118.cn

PHP:  if (!$data) { return; }
来源：https://po.zhonguo7118.cn

JS:   if (!data) return;
来源：https://ca.zhonguo8118.cn

TS:   if (!data) return;
来源：https://cb.zhonguo6118.cn

Java: if (data == null) return;
来源：https://xj.zhonguo3118.cn

Go:   if data == nil { return }
来源：https://an.zhonguo4118.cn

Ruby: return if data.nil?
来源：https://kz.zhonguo4118.cn

C#:   if (data == null) return;
来源：https://gn.zhonguo6118.cn

================================================================================
来源：https://gx.zhonguo7118.cn

C. 函数与作用域
来源：https://fx.zhonguo1118.cn

================================================================================
来源：https://hy.zhonguo5118.cn

[C01] 定义函数
来源：https://pn.zhonguo5118.cn

Py:   def add(a, b): return a + b
来源：https://mc.zhonguo1118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://jz.zhonguo8118.cn

JS:   function add(a, b) { return a + b; }
来源：https://qz.zhonguo8118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://cs.zhonguo7118.cn

Java: static int add(int a, int b) { return a + b; }
来源：https://qn.zhonguo4118.cn

Go:   func add(a, b int) int { return a + b }
来源：https://hw.zhonguo4118.cn

Ruby: def add(a, b); a + b; end
来源：https://wl.zhonguo1118.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：https://xz.zhonguo8118.cn

[C02] 默认参数
来源：https://gw.zhonguo2118.cn

Py:   def greet(name="World"): return name
来源：https://zs.zhonguo6118.cn

PHP:  function greet($name = "World") { return $name; }
来源：https://ka.zhonguo1118.cn

JS:   function greet(name = "World") { return name; }
来源：https://he.zhonguo5118.cn

TS:   function greet(name: string = "World") { return name; }
来源：https://ky.zhonguo8118.cn

Java: // 无默认参数：方法重载或 Optional
来源：https://op.zhonguo5118.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：https://uj.zhonguo2118.cn

Ruby: def greet(name = "World") = name
来源：https://hx.zhonguo2118.cn

C#:   string Greet(string name = "World") => name;
来源：https://yu.zhonguo5118.cn

[C03] 可变参数
来源：https://zw.zhonguo3118.cn

Py:   def total(*args): return sum(args)
来源：https://hl.zhonguo2118.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：https://dh.zhonguo5118.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：https://hw.zhonguo7118.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：https://pe.zhonguo6118.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：https://cq.zhonguo5118.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：https://zi.zhonguo4118.cn

Ruby: def total(*nums); nums.sum; end
来源：https://rc.zhonguo3118.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：https://nn.zhonguo4118.cn

[C04] 命名参数 / 关键字参数
来源：https://xn.zhonguo2118.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：https://an.zhonguo5118.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：https://gf.zhonguo5118.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：https://av.zhonguo6118.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：https://lq.zhonguo4118.cn

Java: // 无：用 Builder 模式或 record
来源：https://lr.zhonguo8118.cn

Go:   // 无：用配置结构体参数
来源：https://em.zhonguo2118.cn

Ruby: f(a: 1, b: 2)
来源：https://ok.zhonguo3118.cn

C#:   f(a: 1, b: 2)
来源：https://eg.zhonguo2118.cn

[C05] 返回多个值
来源：https://ut.zhonguo4118.cn

Py:   return a, b
来源：https://tg.zhonguo4118.cn

PHP:  return [$a, $b];
来源：https://vc.zhonguo1118.cn

JS:   return [a, b];             // 或 return { a, b };
来源：https://lm.zhonguo5118.cn

TS:   return { a, b };
来源：https://zc.zhonguo8118.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：https://ax.zhonguo6118.cn

Go:   return a, b
来源：https://hu.zhonguo2118.cn

Ruby: return a, b
来源：https://kc.zhonguo4118.cn

C#:   return (a, b);              // ValueTuple
来源：https://it.zhonguo4118.cn

[C06] 匿名函数 / lambda
来源：https://pu.zhonguo3118.cn

Py:   square = lambda x: x * x
来源：https://pj.zhonguo1118.cn

PHP:  $square = fn($x) => $x * $x;
来源：https://yr.zhonguo3118.cn

JS:   const square = x => x * x;
来源：https://qq.zhonguo5118.cn

TS:   const square = (x: number): number => x * x;
来源：https://oh.zhonguo7118.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：https://cl.zhonguo2118.cn

Go:   sq := func(x int) int { return x * x }
来源：https://bx.zhonguo7118.cn

Ruby: square = ->(x) { x * x }
来源：https://dr.zhonguo1118.cn

C#:   Func<int, int> square = x => x * x;
来源：https://qv.zhonguo8118.cn

[C07] 把函数作为参数传入
来源：https://yi.zhonguo8118.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：https://se.zhonguo1118.cn

PHP:  array_map("strtoupper", $arr);
来源：https://jm.zhonguo7118.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：https://fx.zhonguo3118.cn

TS:   arr.map(String)
来源：https://hm.zhonguo5118.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：https://xf.zhonguo5118.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：https://ps.zhonguo5118.cn

Ruby: arr.map(&:upcase)
来源：https://tx.zhonguo5118.cn

C#:   arr.Select(s => s.ToUpper())
来源：https://ho.zhonguo8118.cn

[C08] 闭包
来源：https://aw.zhonguo6118.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：https://ja.zhonguo7118.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：https://qi.zhonguo3118.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：https://av.zhonguo3118.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：https://en.zhonguo3118.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：https://tw.zhonguo2118.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：https://ju.zhonguo1118.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：https://cu.zhonguo5118.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：https://tu.zhonguo5118.cn

[C09] 递归
来源：https://lo.zhonguo8118.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：https://ke.zhonguo4118.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：https://wz.zhonguo4118.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://yn.zhonguo5118.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://ic.zhonguo1118.cn


<!-- 参考信息 -->