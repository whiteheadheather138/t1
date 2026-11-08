代发 wailian999

Py:   abs(-5); max(1, 2); min(1, 2)
来源：https://db.zhonguo7118.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：https://ca.zhonguo6118.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：https://dg.zhonguo1118.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：https://dp.zhonguo5118.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：https://lv.zhonguo7118.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：https://up.zhonguo8118.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：https://bk.zhonguo3118.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：https://ot.zhonguo4118.cn

[A10] 生成随机数
来源：https://iz.zhonguo3118.cn

Py:   import random; random.randint(1, 100)
来源：https://bz.zhonguo8118.cn

PHP:  random_int(1, 100);
来源：https://ap.zhonguo5118.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：https://pp.zhonguo4118.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：https://zu.zhonguo6118.cn

Java: new Random().nextInt(100) + 1
来源：https://ic.zhonguo8118.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：https://qw.zhonguo1118.cn

Ruby: rand(1..100)
来源：https://hp.zhonguo3118.cn

C#:   new Random().Next(1, 101)
来源：https://fk.zhonguo4118.cn

[A11] 条件表达式（三元）
来源：https://rv.zhonguo7118.cn

Py:   "yes" if x > 0 else "no"
来源：https://yk.zhonguo7118.cn

PHP:  $x > 0 ? "yes" : "no"
来源：https://yg.zhonguo3118.cn

JS:   x > 0 ? "yes" : "no"
来源：https://rg.zhonguo1118.cn

TS:   x > 0 ? "yes" : "no"
来源：https://mm.zhonguo3118.cn

Java: x > 0 ? "yes" : "no"
来源：https://sz.zhonguo6118.cn

Go:   // 无三元运算符，需用 if 语句
来源：https://mh.zhonguo8118.cn

Ruby: x > 0 ? "yes" : "no"
来源：https://qz.zhonguo6118.cn

C#:   x > 0 ? "yes" : "no"
来源：https://vb.zhonguo8118.cn

[A12] 字符串插值 / 格式化
来源：https://wi.zhonguo6118.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：https://ux.zhonguo7118.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：https://vk.zhonguo6118.cn

JS:   `Hello, ${name}!`
来源：https://at.zhonguo1118.cn

TS:   `Hello, ${name}!`
来源：https://iw.zhonguo7118.cn

Java: "Hello, %s!".formatted(name)
来源：https://iv.zhonguo7118.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：https://ul.zhonguo8118.cn

Ruby: "Hello, #{name}!"
来源：https://zu.zhonguo6118.cn

C#:   $"Hello, {name}!"
来源：https://xt.zhonguo5118.cn

[A13] 多行字符串（练习 \n 转义）
来源：https://bh.zhonguo3118.cn

Py:   "第一行\n第二行"
来源：https://ze.zhonguo7118.cn

PHP:  "第一行\n第二行"
来源：https://kw.zhonguo8118.cn

JS:   "第一行\n第二行"
来源：https://ms.zhonguo8118.cn

TS:   "第一行\n第二行"
来源：https://uq.zhonguo3118.cn

Java: "第一行\n第二行"
来源：https://yz.zhonguo2118.cn

Go:   "第一行\n第二行"
来源：https://wq.zhonguo2118.cn

Ruby: "第一行\n第二行"
来源：https://ow.zhonguo2118.cn

C#:   "第一行\n第二行"
来源：https://oa.zhonguo1118.cn

[A14] 注释写法
来源：https://ex.zhonguo2118.cn

Py:   # 单行；三引号字符串可作多行说明
来源：https://gx.zhonguo6118.cn

PHP:  // 或 # 单行；/* 多行 */
来源：https://ip.zhonguo4118.cn

JS:   // 单行；/* 多行 */
来源：https://ft.zhonguo1118.cn

TS:   // 单行；/* 多行 */
来源：https://dg.zhonguo1118.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：https://qg.zhonguo3118.cn

Go:   // 单行；/* 多行 */
来源：https://ep.zhonguo8118.cn

Ruby: # 单行；=begin 多行 =end
来源：https://wo.zhonguo2118.cn

C#:   // 单行；/* 多行 */
来源：https://vp.zhonguo1118.cn

[A15] 空值判断与默认值
来源：https://zv.zhonguo8118.cn

Py:   value = data or "默认值"
来源：https://ps.zhonguo3118.cn

PHP:  $value = $data ?? "默认值";
来源：https://yf.zhonguo5118.cn

JS:   const value = data ?? "默认值";
来源：https://yb.zhonguo5118.cn

TS:   const value = data ?? "默认值";
来源：https://pz.zhonguo5118.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：https://lk.zhonguo2118.cn

Go:   if data == "" { data = "默认值" }
来源：https://bh.zhonguo3118.cn

Ruby: value = data || "默认值"
来源：https://yi.zhonguo7118.cn

C#:   var value = data ?? "默认值";
来源：https://lo.zhonguo8118.cn

[A16] 真假值判断规则
来源：https://co.zhonguo1118.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：https://bj.zhonguo7118.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：https://sp.zhonguo1118.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：https://tf.zhonguo5118.cn

TS:   if (!x) {}
来源：https://iw.zhonguo5118.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：https://yn.zhonguo5118.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：https://dg.zhonguo6118.cn

Ruby: unless x            # nil 与 false 为假
来源：https://ti.zhonguo7118.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：https://dr.zhonguo2118.cn

[A17] 位运算
来源：https://ro.zhonguo8118.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://ar.zhonguo2118.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：https://mi.zhonguo8118.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://fk.zhonguo5118.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：https://qu.zhonguo3118.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://eb.zhonguo8118.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：https://rm.zhonguo6118.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://vj.zhonguo7118.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://rc.zhonguo8118.cn

[A18] 字符与 ASCII 码互转
来源：https://cl.zhonguo5118.cn

Py:   ord("A"); chr(65)
来源：https://nu.zhonguo7118.cn

PHP:  ord("A"); chr(65)
来源：https://yx.zhonguo3118.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://io.zhonguo1118.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://mp.zhonguo6118.cn

Java: (int) 'A'; (char) 65
来源：https://tt.zhonguo2118.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：https://ml.zhonguo5118.cn

Ruby: "A".ord; 65.chr
来源：https://tj.zhonguo7118.cn

C#:   (int)'A'; (char)65
来源：https://jq.zhonguo8118.cn

[A19] 交换两个变量
来源：https://cx.zhonguo8118.cn

Py:   a, b = b, a
来源：https://fm.zhonguo4118.cn

PHP:  [$a, $b] = [$b, $a];
来源：https://st.zhonguo2118.cn

JS:   [a, b] = [b, a];
来源：https://vy.zhonguo3118.cn

TS:   [a, b] = [b, a];
来源：https://qj.zhonguo6118.cn

Java: int t = a; a = b; b = t;
来源：https://rq.zhonguo2118.cn

Go:   a, b = b, a
来源：https://bo.zhonguo3118.cn

Ruby: a, b = b, a
来源：https://ln.zhonguo5118.cn

C#:   (a, b) = (b, a);
来源：https://gy.zhonguo8118.cn

[A20] 读取标准输入
来源：https://hy.zhonguo6118.cn

Py:   name = input("请输入：")
来源：https://wp.zhonguo7118.cn

PHP:  $name = trim(fgets(STDIN));
来源：https://uc.zhonguo3118.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：https://mv.zhonguo5118.cn

TS:   // Node.js：readline 模块
来源：https://tk.zhonguo7118.cn

Java: new Scanner(System.in).nextLine()
来源：https://yy.zhonguo1118.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：https://pa.zhonguo6118.cn

Ruby: gets.chomp
来源：https://ar.zhonguo4118.cn

C#:   Console.ReadLine();
来源：https://qo.zhonguo3118.cn

[A21] 保留指定小数位输出
来源：https://xh.zhonguo4118.cn

Py:   f"{3.14159:.2f}"
来源：https://ub.zhonguo2118.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：https://cl.zhonguo8118.cn

JS:   (3.14159).toFixed(2)
来源：https://ab.zhonguo6118.cn

TS:   (3.14159).toFixed(2)
来源：https://he.zhonguo8118.cn

Java: String.format("%.2f", 3.14159)
来源：https://ua.zhonguo7118.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：https://zr.zhonguo3118.cn

Ruby: format("%.2f", 3.14159)
来源：https://ry.zhonguo1118.cn

C#:   3.14159.ToString("F2")
来源：https://dw.zhonguo1118.cn

[A22] 获取字符串长度
来源：https://xk.zhonguo3118.cn

Py:   len(s)
来源：https://jt.zhonguo6118.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：https://rf.zhonguo5118.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：https://cb.zhonguo3118.cn

TS:   s.length
来源：https://nt.zhonguo5118.cn

Java: s.length()
来源：https://ym.zhonguo8118.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：https://ic.zhonguo7118.cn

Ruby: s.length
来源：https://cg.zhonguo3118.cn

C#:   s.Length
来源：https://ag.zhonguo8118.cn

[A23] 大小写转换
来源：https://dq.zhonguo3118.cn

Py:   s.upper(); s.lower(); s.title()
来源：https://mn.zhonguo4118.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：https://zx.zhonguo3118.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：https://qf.zhonguo2118.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：https://rz.zhonguo7118.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：https://tg.zhonguo8118.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：https://wy.zhonguo1118.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：https://cw.zhonguo5118.cn

C#:   s.ToUpper(); s.ToLower()
来源：https://ul.zhonguo6118.cn

[A24] 去除首尾空白
来源：https://ar.zhonguo5118.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：https://wt.zhonguo4118.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：https://hv.zhonguo4118.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://fq.zhonguo7118.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://gv.zhonguo8118.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：https://qp.zhonguo4118.cn

Go:   strings.TrimSpace(s)
来源：https://iu.zhonguo7118.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：https://gc.zhonguo1118.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：https://ig.zhonguo6118.cn

[A25] 字符串比较
来源：https://ho.zhonguo4118.cn

Py:   s1 == s2; s1 != s2
来源：https://si.zhonguo1118.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：https://zi.zhonguo1118.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：https://jo.zhonguo5118.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：https://kt.zhonguo3118.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：https://un.zhonguo4118.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：https://yz.zhonguo4118.cn

Ruby: s1 == s2; s1 <=> s2
来源：https://ij.zhonguo3118.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：https://eg.zhonguo7118.cn

[A26] 类型转换总览
来源：https://gh.zhonguo1118.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：https://ec.zhonguo3118.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：https://kr.zhonguo2118.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：https://nv.zhonguo7118.cn

TS:   Number() String() Boolean() x as number
来源：https://hj.zhonguo5118.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：https://pk.zhonguo8118.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：https://jc.zhonguo4118.cn

Ruby: to_i to_f to_s to_sym to_a
来源：https://hz.zhonguo1118.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：https://yt.zhonguo4118.cn

================================================================================
来源：https://ct.zhonguo1118.cn

B. 流程控制
来源：https://kp.zhonguo1118.cn

================================================================================
来源：https://ld.zhonguo4118.cn

[B01] 条件判断 if / else
来源：https://um.zhonguo1118.cn

Py:   result = "正" if x > 0 else "非正"
来源：https://ce.zhonguo8118.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：https://if.zhonguo7118.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：https://mx.zhonguo2118.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：https://pb.zhonguo7118.cn

Java: String r = x > 0 ? "正" : "非正";
来源：https://sn.zhonguo7118.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：https://tc.zhonguo7118.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：https://po.zhonguo4118.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：https://pl.zhonguo7118.cn

[B02] 多分支 else if / elif
来源：https://tl.zhonguo7118.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：https://bf.zhonguo6118.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：https://zm.zhonguo4118.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://zn.zhonguo6118.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://zo.zhonguo2118.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://fk.zhonguo3118.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：https://sb.zhonguo4118.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：https://yx.zhonguo2118.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://dt.zhonguo7118.cn

[B03] switch / match / case
来源：https://xs.zhonguo6118.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：https://gt.zhonguo4118.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：https://ft.zhonguo4118.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://dc.zhonguo6118.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://rk.zhonguo4118.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：https://ay.zhonguo5118.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：https://oj.zhonguo4118.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：https://uy.zhonguo4118.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：https://ic.zhonguo8118.cn

[B04] for 计数循环
来源：https://ff.zhonguo6118.cn

Py:   for i in range(10): print(i)
来源：https://jv.zhonguo1118.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：https://co.zhonguo5118.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://gx.zhonguo3118.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://qo.zhonguo2118.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：https://ns.zhonguo3118.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：https://fi.zhonguo5118.cn

Ruby: 10.times { |i| puts i }
来源：https://wf.zhonguo8118.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：https://kn.zhonguo3118.cn

[B05] 遍历数组 / 列表
来源：https://sc.zhonguo2118.cn

Py:   for item in arr: print(item)
来源：https://nk.zhonguo4118.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：https://dd.zhonguo1118.cn

JS:   for (const item of arr) { console.log(item); }
来源：https://xe.zhonguo2118.cn

TS:   for (const item of arr) { console.log(item); }
来源：https://tq.zhonguo6118.cn

Java: for (var item : arr) { System.out.println(item); }
来源：https://jk.zhonguo6118.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：https://mv.zhonguo2118.cn

Ruby: arr.each { |item| puts item }
来源：https://wq.zhonguo2118.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：https://nh.zhonguo8118.cn

[B06] 遍历字典 / 对象
来源：https://fi.zhonguo4118.cn

Py:   for k, v in d.items(): print(k, v)
来源：https://ge.zhonguo5118.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：https://vv.zhonguo1118.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://pa.zhonguo7118.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://wn.zhonguo2118.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：https://av.zhonguo3118.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：https://mz.zhonguo5118.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：https://ux.zhonguo8118.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：https://ux.zhonguo8118.cn

[B07] while 循环
来源：https://if.zhonguo1118.cn

Py:   while i < 10: i += 1
来源：https://yu.zhonguo7118.cn

PHP:  while ($i < 10) { $i++; }
来源：https://ie.zhonguo8118.cn

JS:   while (i < 10) { i++; }
来源：https://gl.zhonguo3118.cn

TS:   while (i < 10) { i++; }
来源：https://rd.zhonguo4118.cn

Java: while (i < 10) { i++; }
来源：https://ik.zhonguo2118.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：https://on.zhonguo7118.cn

Ruby: while i < 10; i += 1; end
来源：https://kn.zhonguo1118.cn

C#:   while (i < 10) { i++; }
来源：https://du.zhonguo2118.cn

[B08] do-while（至少执行一次）
来源：https://ug.zhonguo8118.cn

Py:   # 无 do-while：用 while True + break
来源：https://tm.zhonguo4118.cn

PHP:  do { $i++; } while ($i < 10);
来源：https://rd.zhonguo7118.cn

JS:   do { i++; } while (i < 10);
来源：https://nv.zhonguo3118.cn

TS:   do { i++; } while (i < 10);
来源：https://xd.zhonguo7118.cn

Java: do { i++; } while (i < 10);
来源：https://vy.zhonguo2118.cn

Go:   for { i++; if i >= 10 { break } }
来源：https://lj.zhonguo6118.cn

Ruby: begin; i += 1; end while i < 10
来源：https://en.zhonguo6118.cn

C#:   do { i++; } while (i < 10);
来源：https://wg.zhonguo3118.cn

[B09] break 与 continue
来源：https://dn.zhonguo2118.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：https://hn.zhonguo6118.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：https://fj.zhonguo2118.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://ko.zhonguo4118.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://vy.zhonguo1118.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://co.zhonguo2118.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：https://gc.zhonguo4118.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：https://do.zhonguo8118.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://cd.zhonguo6118.cn

[B10] 遍历同时拿索引
来源：https://xl.zhonguo4118.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：https://as.zhonguo8118.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：https://wg.zhonguo4118.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：https://xz.zhonguo2118.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：https://yd.zhonguo2118.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：https://jn.zhonguo7118.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：https://qq.zhonguo7118.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：https://vl.zhonguo5118.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：https://rr.zhonguo5118.cn

[B11] 生成数字序列 / 区间
来源：https://cy.zhonguo7118.cn

Py:   list(range(0, 10, 2))
来源：https://ej.zhonguo2118.cn

PHP:  range(0, 10, 2);
来源：https://gv.zhonguo3118.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://ya.zhonguo2118.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://fz.zhonguo2118.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：https://hf.zhonguo1118.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：https://ak.zhonguo2118.cn

Ruby: (0...10).step(2).to_a
来源：https://po.zhonguo3118.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：https://ru.zhonguo8118.cn

[B12] 跳出多层循环
来源：https://ro.zhonguo4118.cn

Py:   # 无标签跳转：抽成函数用 return
来源：https://cb.zhonguo4118.cn

PHP:  # 无标签：用 goto 或函数返回
来源：https://lf.zhonguo8118.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：https://ue.zhonguo8118.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：https://mk.zhonguo3118.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：https://cq.zhonguo7118.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：https://eb.zhonguo6118.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：https://oi.zhonguo8118.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：https://cc.zhonguo3118.cn

[B13] 判断是否为数字
来源：https://tt.zhonguo1118.cn

Py:   isinstance(x, (int, float))
来源：https://xe.zhonguo2118.cn

PHP:  is_numeric($x)
来源：https://cl.zhonguo7118.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：https://gy.zhonguo3118.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：https://hj.zhonguo1118.cn

Java: x instanceof Number
来源：https://zj.zhonguo5118.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：https://xw.zhonguo6118.cn

Ruby: x.is_a?(Numeric)
来源：https://jq.zhonguo4118.cn

C#:   x is int or double or decimal
来源：https://yy.zhonguo3118.cn

[B14] 判断值是否在集合内
来源：https://gr.zhonguo3118.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：https://gv.zhonguo1118.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：https://ro.zhonguo1118.cn

JS:   [1, 2, 3].includes(x)
来源：https://ka.zhonguo7118.cn

TS:   [1, 2, 3].includes(x)
来源：https://pe.zhonguo7118.cn

Java: List.of(1, 2, 3).contains(x)
来源：https://pv.zhonguo1118.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：https://dz.zhonguo4118.cn

Ruby: [1, 2, 3].include?(x)
来源：https://go.zhonguo8118.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：https://aw.zhonguo8118.cn

[B15] 布尔运算与取反
来源：https://pk.zhonguo8118.cn

Py:   a and b or not c
来源：https://sn.zhonguo4118.cn

PHP:  $a && $b || !$c
来源：https://mj.zhonguo5118.cn

JS:   a && b || !c
来源：https://tf.zhonguo4118.cn

TS:   a && b || !c
来源：https://ex.zhonguo4118.cn

Java: a && b || !c
来源：https://nz.zhonguo6118.cn

Go:   a && b || !c
来源：https://ls.zhonguo6118.cn

Ruby: a && b || !c
来源：https://fq.zhonguo2118.cn

C#:   a && b || !c
来源：https://kx.zhonguo5118.cn

[B16] 卫语句：不满足条件提前返回
来源：https://is.zhonguo4118.cn


<!-- 参考信息 -->