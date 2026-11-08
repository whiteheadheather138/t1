代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：https://ot.zhonguo1118.cn

Java: new Random().nextInt(100) + 1
来源：https://hd.zhonguo3118.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：https://aw.zhonguo8118.cn

Ruby: rand(1..100)
来源：https://fh.zhonguo8118.cn

C#:   new Random().Next(1, 101)
来源：https://bn.zhonguo7118.cn

[A11] 条件表达式（三元）
来源：https://xt.zhonguo4118.cn

Py:   "yes" if x > 0 else "no"
来源：https://jc.zhonguo3118.cn

PHP:  $x > 0 ? "yes" : "no"
来源：https://ee.zhonguo1118.cn

JS:   x > 0 ? "yes" : "no"
来源：https://sj.zhonguo3118.cn

TS:   x > 0 ? "yes" : "no"
来源：https://gg.zhonguo2118.cn

Java: x > 0 ? "yes" : "no"
来源：https://cx.zhonguo7118.cn

Go:   // 无三元运算符，需用 if 语句
来源：https://xn.zhonguo4118.cn

Ruby: x > 0 ? "yes" : "no"
来源：https://ub.zhonguo4118.cn

C#:   x > 0 ? "yes" : "no"
来源：https://zt.zhonguo4118.cn

[A12] 字符串插值 / 格式化
来源：https://ps.zhonguo2118.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：https://cd.zhonguo6118.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：https://ux.zhonguo5118.cn

JS:   `Hello, ${name}!`
来源：https://or.zhonguo3118.cn

TS:   `Hello, ${name}!`
来源：https://ex.zhonguo1118.cn

Java: "Hello, %s!".formatted(name)
来源：https://jv.zhonguo2118.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：https://fu.zhonguo3118.cn

Ruby: "Hello, #{name}!"
来源：https://ky.zhonguo7118.cn

C#:   $"Hello, {name}!"
来源：https://ou.zhonguo7118.cn

[A13] 多行字符串（练习 \n 转义）
来源：https://tl.zhonguo1118.cn

Py:   "第一行\n第二行"
来源：https://dn.zhonguo4118.cn

PHP:  "第一行\n第二行"
来源：https://xf.zhonguo1118.cn

JS:   "第一行\n第二行"
来源：https://gp.zhonguo5118.cn

TS:   "第一行\n第二行"
来源：https://cm.zhonguo1118.cn

Java: "第一行\n第二行"
来源：https://gq.zhonguo6118.cn

Go:   "第一行\n第二行"
来源：https://ie.zhonguo3118.cn

Ruby: "第一行\n第二行"
来源：https://ab.zhonguo7118.cn

C#:   "第一行\n第二行"
来源：https://je.zhonguo6118.cn

[A14] 注释写法
来源：https://ao.zhonguo5118.cn

Py:   # 单行；三引号字符串可作多行说明
来源：https://uc.zhonguo4118.cn

PHP:  // 或 # 单行；/* 多行 */
来源：https://bz.zhonguo4118.cn

JS:   // 单行；/* 多行 */
来源：https://go.zhonguo7118.cn

TS:   // 单行；/* 多行 */
来源：https://xy.zhonguo5118.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：https://rk.zhonguo4118.cn

Go:   // 单行；/* 多行 */
来源：https://if.zhonguo6118.cn

Ruby: # 单行；=begin 多行 =end
来源：https://kx.zhonguo4118.cn

C#:   // 单行；/* 多行 */
来源：https://pb.zhonguo2118.cn

[A15] 空值判断与默认值
来源：https://el.zhonguo5118.cn

Py:   value = data or "默认值"
来源：https://he.zhonguo1118.cn

PHP:  $value = $data ?? "默认值";
来源：https://wp.zhonguo8118.cn

JS:   const value = data ?? "默认值";
来源：https://xi.zhonguo4118.cn

TS:   const value = data ?? "默认值";
来源：https://ri.zhonguo6118.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：https://xm.zhonguo5118.cn

Go:   if data == "" { data = "默认值" }
来源：https://if.zhonguo4118.cn

Ruby: value = data || "默认值"
来源：https://pb.zhonguo5118.cn

C#:   var value = data ?? "默认值";
来源：https://ta.zhonguo1118.cn

[A16] 真假值判断规则
来源：https://bz.zhonguo1118.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：https://ca.zhonguo4118.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：https://ji.zhonguo8118.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：https://wd.zhonguo8118.cn

TS:   if (!x) {}
来源：https://xo.zhonguo3118.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：https://sf.zhonguo2118.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：https://dc.zhonguo8118.cn

Ruby: unless x            # nil 与 false 为假
来源：https://ct.zhonguo4118.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：https://nu.zhonguo1118.cn

[A17] 位运算
来源：https://km.zhonguo4118.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://cz.zhonguo4118.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：https://fj.zhonguo4118.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://qx.zhonguo4118.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：https://al.zhonguo4118.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://rk.zhonguo1118.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：https://ji.zhonguo7118.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://ur.zhonguo8118.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://nl.zhonguo6118.cn

[A18] 字符与 ASCII 码互转
来源：https://rc.zhonguo3118.cn

Py:   ord("A"); chr(65)
来源：https://fo.zhonguo8118.cn

PHP:  ord("A"); chr(65)
来源：https://lr.zhonguo3118.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://lx.zhonguo5118.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://vm.zhonguo4118.cn

Java: (int) 'A'; (char) 65
来源：https://hr.zhonguo7118.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：https://yn.zhonguo2118.cn

Ruby: "A".ord; 65.chr
来源：https://gh.zhonguo7118.cn

C#:   (int)'A'; (char)65
来源：https://gy.zhonguo3118.cn

[A19] 交换两个变量
来源：https://id.zhonguo5118.cn

Py:   a, b = b, a
来源：https://sm.zhonguo3118.cn

PHP:  [$a, $b] = [$b, $a];
来源：https://iq.zhonguo5118.cn

JS:   [a, b] = [b, a];
来源：https://ry.zhonguo6118.cn

TS:   [a, b] = [b, a];
来源：https://ly.zhonguo8118.cn

Java: int t = a; a = b; b = t;
来源：https://nk.zhonguo6118.cn

Go:   a, b = b, a
来源：https://uu.zhonguo2118.cn

Ruby: a, b = b, a
来源：https://tw.zhonguo7118.cn

C#:   (a, b) = (b, a);
来源：https://uf.zhonguo3118.cn

[A20] 读取标准输入
来源：https://uf.zhonguo1118.cn

Py:   name = input("请输入：")
来源：https://hz.zhonguo7118.cn

PHP:  $name = trim(fgets(STDIN));
来源：https://pa.zhonguo8118.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：https://px.zhonguo7118.cn

TS:   // Node.js：readline 模块
来源：https://qk.zhonguo6118.cn

Java: new Scanner(System.in).nextLine()
来源：https://ij.zhonguo4118.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：https://fx.zhonguo6118.cn

Ruby: gets.chomp
来源：https://ku.zhonguo3118.cn

C#:   Console.ReadLine();
来源：https://wq.zhonguo5118.cn

[A21] 保留指定小数位输出
来源：https://nr.zhonguo6118.cn

Py:   f"{3.14159:.2f}"
来源：https://ge.zhonguo4118.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：https://yf.zhonguo5118.cn

JS:   (3.14159).toFixed(2)
来源：https://ao.zhonguo5118.cn

TS:   (3.14159).toFixed(2)
来源：https://mw.zhonguo1118.cn

Java: String.format("%.2f", 3.14159)
来源：https://od.zhonguo5118.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：https://uu.zhonguo7118.cn

Ruby: format("%.2f", 3.14159)
来源：https://xu.zhonguo5118.cn

C#:   3.14159.ToString("F2")
来源：https://oo.zhonguo4118.cn

[A22] 获取字符串长度
来源：https://gf.zhonguo4118.cn

Py:   len(s)
来源：https://iw.zhonguo5118.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：https://iz.zhonguo8118.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：https://av.zhonguo4118.cn

TS:   s.length
来源：https://rg.zhonguo6118.cn

Java: s.length()
来源：https://nf.zhonguo5118.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：https://yx.zhonguo1118.cn

Ruby: s.length
来源：https://mv.zhonguo5118.cn

C#:   s.Length
来源：https://cl.zhonguo3118.cn

[A23] 大小写转换
来源：https://zm.zhonguo3118.cn

Py:   s.upper(); s.lower(); s.title()
来源：https://ft.zhonguo4118.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：https://ny.zhonguo5118.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：https://wm.zhonguo1118.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：https://yo.zhonguo1118.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：https://ku.zhonguo4118.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：https://oa.zhonguo3118.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：https://pw.zhonguo4118.cn

C#:   s.ToUpper(); s.ToLower()
来源：https://wd.zhonguo7118.cn

[A24] 去除首尾空白
来源：https://nq.zhonguo2118.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：https://ba.zhonguo5118.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：https://pk.zhonguo5118.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://em.zhonguo2118.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://cp.zhonguo8118.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：https://gx.zhonguo2118.cn

Go:   strings.TrimSpace(s)
来源：https://cy.zhonguo1118.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：https://ur.zhonguo6118.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：https://hh.zhonguo3118.cn

[A25] 字符串比较
来源：https://cw.zhonguo4118.cn

Py:   s1 == s2; s1 != s2
来源：https://fp.zhonguo6118.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：https://pg.zhonguo2118.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：https://qu.zhonguo3118.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：https://ys.zhonguo4118.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：https://ww.zhonguo1118.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：https://kv.zhonguo4118.cn

Ruby: s1 == s2; s1 <=> s2
来源：https://fg.zhonguo4118.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：https://dk.zhonguo7118.cn

[A26] 类型转换总览
来源：https://yd.zhonguo3118.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：https://bv.zhonguo2118.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：https://ga.zhonguo2118.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：https://yb.zhonguo8118.cn

TS:   Number() String() Boolean() x as number
来源：https://tu.zhonguo3118.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：https://gb.zhonguo6118.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：https://ty.zhonguo2118.cn

Ruby: to_i to_f to_s to_sym to_a
来源：https://yj.zhonguo6118.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：https://jh.zhonguo3118.cn

================================================================================
来源：https://om.zhonguo4118.cn

B. 流程控制
来源：https://df.zhonguo5118.cn

================================================================================
来源：https://jr.zhonguo5118.cn

[B01] 条件判断 if / else
来源：https://lf.zhonguo7118.cn

Py:   result = "正" if x > 0 else "非正"
来源：https://nw.zhonguo7118.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：https://ka.zhonguo7118.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：https://xi.zhonguo1118.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：https://no.zhonguo1118.cn

Java: String r = x > 0 ? "正" : "非正";
来源：https://jy.zhonguo1118.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：https://ou.zhonguo6118.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：https://aa.zhonguo7118.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：https://bp.zhonguo6118.cn

[B02] 多分支 else if / elif
来源：https://ar.zhonguo2118.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：https://yq.zhonguo1118.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：https://eb.zhonguo4118.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://wz.zhonguo6118.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://uj.zhonguo6118.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://uh.zhonguo1118.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：https://cg.zhonguo7118.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：https://nq.zhonguo4118.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://qh.zhonguo3118.cn

[B03] switch / match / case
来源：https://ix.zhonguo7118.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：https://aj.zhonguo4118.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：https://ry.zhonguo3118.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://vj.zhonguo1118.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://en.zhonguo8118.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：https://jc.zhonguo7118.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：https://ol.zhonguo1118.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：https://eu.zhonguo2118.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：https://uw.zhonguo6118.cn

[B04] for 计数循环
来源：https://hd.zhonguo8118.cn

Py:   for i in range(10): print(i)
来源：https://qd.zhonguo8118.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：https://hk.zhonguo5118.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://ap.zhonguo8118.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://sc.zhonguo1118.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：https://pa.zhonguo5118.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：https://yy.zhonguo5118.cn

Ruby: 10.times { |i| puts i }
来源：https://kf.zhonguo8118.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：https://qh.zhonguo2118.cn

[B05] 遍历数组 / 列表
来源：https://go.zhonguo4118.cn

Py:   for item in arr: print(item)
来源：https://pm.zhonguo4118.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：https://un.zhonguo8118.cn

JS:   for (const item of arr) { console.log(item); }
来源：https://no.zhonguo4118.cn

TS:   for (const item of arr) { console.log(item); }
来源：https://ob.zhonguo8118.cn

Java: for (var item : arr) { System.out.println(item); }
来源：https://zt.zhonguo6118.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：https://gv.zhonguo2118.cn

Ruby: arr.each { |item| puts item }
来源：https://dg.zhonguo4118.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：https://is.zhonguo8118.cn

[B06] 遍历字典 / 对象
来源：https://jv.zhonguo4118.cn

Py:   for k, v in d.items(): print(k, v)
来源：https://af.zhonguo2118.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：https://kh.zhonguo1118.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://qu.zhonguo6118.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://ic.zhonguo1118.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：https://sf.zhonguo8118.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：https://ds.zhonguo5118.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：https://ow.zhonguo5118.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：https://wi.zhonguo3118.cn

[B07] while 循环
来源：https://gi.zhonguo3118.cn

Py:   while i < 10: i += 1
来源：https://be.zhonguo1118.cn

PHP:  while ($i < 10) { $i++; }
来源：https://ur.zhonguo5118.cn

JS:   while (i < 10) { i++; }
来源：https://hr.zhonguo6118.cn

TS:   while (i < 10) { i++; }
来源：https://dp.zhonguo8118.cn

Java: while (i < 10) { i++; }
来源：https://sw.zhonguo2118.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：https://cp.zhonguo7118.cn

Ruby: while i < 10; i += 1; end
来源：https://ps.zhonguo8118.cn

C#:   while (i < 10) { i++; }
来源：https://dv.zhonguo1118.cn

[B08] do-while（至少执行一次）
来源：https://rr.zhonguo7118.cn

Py:   # 无 do-while：用 while True + break
来源：https://or.zhonguo5118.cn

PHP:  do { $i++; } while ($i < 10);
来源：https://sc.zhonguo5118.cn

JS:   do { i++; } while (i < 10);
来源：https://fh.zhonguo1118.cn

TS:   do { i++; } while (i < 10);
来源：https://xd.zhonguo6118.cn

Java: do { i++; } while (i < 10);
来源：https://xb.zhonguo4118.cn

Go:   for { i++; if i >= 10 { break } }
来源：https://uq.zhonguo7118.cn

Ruby: begin; i += 1; end while i < 10
来源：https://px.zhonguo8118.cn

C#:   do { i++; } while (i < 10);
来源：https://me.zhonguo8118.cn

[B09] break 与 continue
来源：https://qr.zhonguo4118.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：https://vn.zhonguo7118.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：https://ij.zhonguo6118.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://rs.zhonguo4118.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://up.zhonguo1118.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://vy.zhonguo7118.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：https://rd.zhonguo3118.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：https://db.zhonguo1118.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://vv.zhonguo7118.cn

[B10] 遍历同时拿索引
来源：https://en.zhonguo1118.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：https://at.zhonguo3118.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：https://ko.zhonguo1118.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：https://ui.zhonguo5118.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：https://rz.zhonguo7118.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：https://qq.zhonguo3118.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：https://vk.zhonguo8118.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：https://nd.zhonguo6118.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：https://se.zhonguo1118.cn

[B11] 生成数字序列 / 区间
来源：https://hv.zhonguo6118.cn

Py:   list(range(0, 10, 2))
来源：https://tu.zhonguo3118.cn

PHP:  range(0, 10, 2);
来源：https://dx.zhonguo4118.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://jq.zhonguo7118.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://at.zhonguo2118.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：https://yy.zhonguo1118.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：https://in.zhonguo8118.cn

Ruby: (0...10).step(2).to_a
来源：https://gm.zhonguo3118.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：https://wd.zhonguo8118.cn

[B12] 跳出多层循环
来源：https://zz.zhonguo7118.cn

Py:   # 无标签跳转：抽成函数用 return
来源：https://jx.zhonguo5118.cn

PHP:  # 无标签：用 goto 或函数返回
来源：https://kj.zhonguo8118.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：https://kd.zhonguo8118.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：https://sm.zhonguo2118.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：https://fv.zhonguo3118.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：https://wc.zhonguo4118.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：https://he.zhonguo4118.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：https://qt.zhonguo7118.cn

[B13] 判断是否为数字
来源：https://kr.zhonguo2118.cn

Py:   isinstance(x, (int, float))
来源：https://rj.zhonguo7118.cn

PHP:  is_numeric($x)
来源：https://du.zhonguo6118.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：https://vi.zhonguo5118.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：https://ak.zhonguo5118.cn

Java: x instanceof Number
来源：https://pz.zhonguo2118.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：https://mk.zhonguo3118.cn

Ruby: x.is_a?(Numeric)
来源：https://zf.zhonguo7118.cn

C#:   x is int or double or decimal
来源：https://mo.zhonguo2118.cn

[B14] 判断值是否在集合内
来源：https://za.zhonguo7118.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：https://lp.zhonguo3118.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：https://ys.zhonguo4118.cn

JS:   [1, 2, 3].includes(x)
来源：https://xk.zhonguo7118.cn

TS:   [1, 2, 3].includes(x)
来源：https://pl.zhonguo2118.cn

Java: List.of(1, 2, 3).contains(x)
来源：https://vk.zhonguo6118.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：https://nk.zhonguo1118.cn

Ruby: [1, 2, 3].include?(x)
来源：https://wq.zhonguo6118.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：https://ss.zhonguo8118.cn

[B15] 布尔运算与取反
来源：https://kx.zhonguo1118.cn

Py:   a and b or not c
来源：https://vx.zhonguo8118.cn

PHP:  $a && $b || !$c
来源：https://lw.zhonguo2118.cn

JS:   a && b || !c
来源：https://pd.zhonguo4118.cn

TS:   a && b || !c
来源：https://qc.zhonguo3118.cn

Java: a && b || !c
来源：https://kg.zhonguo6118.cn

Go:   a && b || !c
来源：https://le.zhonguo4118.cn

Ruby: a && b || !c
来源：https://ek.zhonguo2118.cn

C#:   a && b || !c
来源：https://mo.zhonguo1118.cn

[B16] 卫语句：不满足条件提前返回
来源：https://tj.zhonguo6118.cn

Py:   if not data: return
来源：https://zz.zhonguo8118.cn

PHP:  if (!$data) { return; }
来源：https://nq.zhonguo3118.cn

JS:   if (!data) return;
来源：https://ne.zhonguo4118.cn

TS:   if (!data) return;
来源：https://jq.zhonguo5118.cn

Java: if (data == null) return;
来源：https://ow.zhonguo1118.cn

Go:   if data == nil { return }
来源：https://bo.zhonguo8118.cn

Ruby: return if data.nil?
来源：https://qn.zhonguo8118.cn

C#:   if (data == null) return;
来源：https://pa.zhonguo6118.cn

================================================================================
来源：https://qi.zhonguo2118.cn

C. 函数与作用域
来源：https://zt.zhonguo8118.cn

================================================================================
来源：https://ty.zhonguo6118.cn

[C01] 定义函数
来源：https://ah.zhonguo8118.cn


<!-- 参考信息 -->