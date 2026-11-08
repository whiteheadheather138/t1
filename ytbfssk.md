代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：https://ql.zhonguo3118.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：https://vy.zhonguo1118.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：https://jv.zhonguo6118.cn

Ruby: "42".to_i; "3.14".to_f
来源：https://py.zhonguo4118.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：https://zg.zhonguo3118.cn

[A07] 数字转字符串
来源：https://hk.zhonguo4118.cn

Py:   str(42)
来源：https://oi.zhonguo8118.cn

PHP:  (string) 42; strval(42)
来源：https://lj.zhonguo6118.cn

JS:   String(42); (42).toString()
来源：https://wp.zhonguo4118.cn

TS:   String(42)
来源：https://rl.zhonguo7118.cn

Java: String.valueOf(42); Integer.toString(42)
来源：https://va.zhonguo7118.cn

Go:   strconv.Itoa(42)
来源：https://wo.zhonguo4118.cn

Ruby: 42.to_s
来源：https://zn.zhonguo8118.cn

C#:   42.ToString()
来源：https://re.zhonguo4118.cn

[A08] 取整与四舍五入
来源：https://ix.zhonguo2118.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：https://wh.zhonguo6118.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：https://po.zhonguo8118.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：https://be.zhonguo3118.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：https://or.zhonguo3118.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：https://ae.zhonguo6118.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：https://cc.zhonguo6118.cn

Ruby: 3.567.round(2); 3.9.floor
来源：https://nq.zhonguo6118.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：https://cg.zhonguo1118.cn

[A09] 绝对值与最大最小值
来源：https://ef.zhonguo2118.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：https://mk.zhonguo5118.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：https://rj.zhonguo1118.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：https://te.zhonguo7118.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：https://fc.zhonguo7118.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：https://xi.zhonguo8118.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：https://rg.zhonguo3118.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：https://km.zhonguo8118.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：https://cr.zhonguo3118.cn

[A10] 生成随机数
来源：https://cr.zhonguo6118.cn

Py:   import random; random.randint(1, 100)
来源：https://ls.zhonguo1118.cn

PHP:  random_int(1, 100);
来源：https://gm.zhonguo8118.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：https://fd.zhonguo5118.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：https://wa.zhonguo5118.cn

Java: new Random().nextInt(100) + 1
来源：https://gn.zhonguo4118.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：https://sy.zhonguo8118.cn

Ruby: rand(1..100)
来源：https://hh.zhonguo5118.cn

C#:   new Random().Next(1, 101)
来源：https://lk.zhonguo3118.cn

[A11] 条件表达式（三元）
来源：https://yt.zhonguo2118.cn

Py:   "yes" if x > 0 else "no"
来源：https://ow.zhonguo5118.cn

PHP:  $x > 0 ? "yes" : "no"
来源：https://wj.zhonguo1118.cn

JS:   x > 0 ? "yes" : "no"
来源：https://zv.zhonguo1118.cn

TS:   x > 0 ? "yes" : "no"
来源：https://uh.zhonguo3118.cn

Java: x > 0 ? "yes" : "no"
来源：https://sb.zhonguo2118.cn

Go:   // 无三元运算符，需用 if 语句
来源：https://cf.zhonguo8118.cn

Ruby: x > 0 ? "yes" : "no"
来源：https://na.zhonguo3118.cn

C#:   x > 0 ? "yes" : "no"
来源：https://du.zhonguo8118.cn

[A12] 字符串插值 / 格式化
来源：https://vd.zhonguo6118.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：https://fx.zhonguo4118.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：https://km.zhonguo5118.cn

JS:   `Hello, ${name}!`
来源：https://ak.zhonguo1118.cn

TS:   `Hello, ${name}!`
来源：https://cj.zhonguo5118.cn

Java: "Hello, %s!".formatted(name)
来源：https://vn.zhonguo4118.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：https://tu.zhonguo1118.cn

Ruby: "Hello, #{name}!"
来源：https://pz.zhonguo1118.cn

C#:   $"Hello, {name}!"
来源：https://am.zhonguo6118.cn

[A13] 多行字符串（练习 \n 转义）
来源：https://lq.zhonguo3118.cn

Py:   "第一行\n第二行"
来源：https://za.zhonguo5118.cn

PHP:  "第一行\n第二行"
来源：https://oy.zhonguo7118.cn

JS:   "第一行\n第二行"
来源：https://ri.zhonguo7118.cn

TS:   "第一行\n第二行"
来源：https://ql.zhonguo5118.cn

Java: "第一行\n第二行"
来源：https://ub.zhonguo8118.cn

Go:   "第一行\n第二行"
来源：https://hp.zhonguo2118.cn

Ruby: "第一行\n第二行"
来源：https://gz.zhonguo7118.cn

C#:   "第一行\n第二行"
来源：https://ip.zhonguo3118.cn

[A14] 注释写法
来源：https://iq.zhonguo3118.cn

Py:   # 单行；三引号字符串可作多行说明
来源：https://bn.zhonguo5118.cn

PHP:  // 或 # 单行；/* 多行 */
来源：https://ur.zhonguo1118.cn

JS:   // 单行；/* 多行 */
来源：https://sr.zhonguo6118.cn

TS:   // 单行；/* 多行 */
来源：https://hz.zhonguo7118.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：https://se.zhonguo7118.cn

Go:   // 单行；/* 多行 */
来源：https://wg.zhonguo8118.cn

Ruby: # 单行；=begin 多行 =end
来源：https://km.zhonguo7118.cn

C#:   // 单行；/* 多行 */
来源：https://tg.zhonguo4118.cn

[A15] 空值判断与默认值
来源：https://ne.zhonguo8118.cn

Py:   value = data or "默认值"
来源：https://xu.zhonguo3118.cn

PHP:  $value = $data ?? "默认值";
来源：https://uz.zhonguo6118.cn

JS:   const value = data ?? "默认值";
来源：https://pi.zhonguo8118.cn

TS:   const value = data ?? "默认值";
来源：https://si.zhonguo5118.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：https://wv.zhonguo8118.cn

Go:   if data == "" { data = "默认值" }
来源：https://ma.zhonguo2118.cn

Ruby: value = data || "默认值"
来源：https://pg.zhonguo4118.cn

C#:   var value = data ?? "默认值";
来源：https://pq.zhonguo7118.cn

[A16] 真假值判断规则
来源：https://va.zhonguo4118.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：https://qh.zhonguo1118.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：https://uv.zhonguo2118.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：https://kq.zhonguo8118.cn

TS:   if (!x) {}
来源：https://xl.zhonguo2118.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：https://ip.zhonguo1118.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：https://tq.zhonguo8118.cn

Ruby: unless x            # nil 与 false 为假
来源：https://tz.zhonguo2118.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：https://ha.zhonguo3118.cn

[A17] 位运算
来源：https://fb.zhonguo7118.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://ut.zhonguo7118.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：https://kh.zhonguo5118.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://ha.zhonguo7118.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：https://qw.zhonguo4118.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://lk.zhonguo7118.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：https://np.zhonguo5118.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://um.zhonguo8118.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://jw.zhonguo1118.cn

[A18] 字符与 ASCII 码互转
来源：https://zr.zhonguo2118.cn

Py:   ord("A"); chr(65)
来源：https://yt.zhonguo2118.cn

PHP:  ord("A"); chr(65)
来源：https://wu.zhonguo5118.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://ul.zhonguo4118.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://np.zhonguo5118.cn

Java: (int) 'A'; (char) 65
来源：https://ql.zhonguo8118.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：https://la.zhonguo1118.cn

Ruby: "A".ord; 65.chr
来源：https://wm.zhonguo8118.cn

C#:   (int)'A'; (char)65
来源：https://xa.zhonguo7118.cn

[A19] 交换两个变量
来源：https://bn.zhonguo3118.cn

Py:   a, b = b, a
来源：https://id.zhonguo1118.cn

PHP:  [$a, $b] = [$b, $a];
来源：https://lf.zhonguo3118.cn

JS:   [a, b] = [b, a];
来源：https://lr.zhonguo7118.cn

TS:   [a, b] = [b, a];
来源：https://ei.zhonguo2118.cn

Java: int t = a; a = b; b = t;
来源：https://er.zhonguo2118.cn

Go:   a, b = b, a
来源：https://mt.zhonguo5118.cn

Ruby: a, b = b, a
来源：https://vq.zhonguo5118.cn

C#:   (a, b) = (b, a);
来源：https://hv.zhonguo2118.cn

[A20] 读取标准输入
来源：https://bp.zhonguo3118.cn

Py:   name = input("请输入：")
来源：https://ts.zhonguo1118.cn

PHP:  $name = trim(fgets(STDIN));
来源：https://up.zhonguo1118.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：https://lp.zhonguo7118.cn

TS:   // Node.js：readline 模块
来源：https://sj.zhonguo1118.cn

Java: new Scanner(System.in).nextLine()
来源：https://dn.zhonguo1118.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：https://jk.zhonguo6118.cn

Ruby: gets.chomp
来源：https://hr.zhonguo4118.cn

C#:   Console.ReadLine();
来源：https://sc.zhonguo7118.cn

[A21] 保留指定小数位输出
来源：https://jr.zhonguo2118.cn

Py:   f"{3.14159:.2f}"
来源：https://vg.zhonguo4118.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：https://kh.zhonguo3118.cn

JS:   (3.14159).toFixed(2)
来源：https://ko.zhonguo1118.cn

TS:   (3.14159).toFixed(2)
来源：https://dz.zhonguo5118.cn

Java: String.format("%.2f", 3.14159)
来源：https://jw.zhonguo1118.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：https://vz.zhonguo5118.cn

Ruby: format("%.2f", 3.14159)
来源：https://xe.zhonguo4118.cn

C#:   3.14159.ToString("F2")
来源：https://cr.zhonguo5118.cn

[A22] 获取字符串长度
来源：https://ri.zhonguo3118.cn

Py:   len(s)
来源：https://uc.zhonguo4118.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：https://yi.zhonguo6118.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：https://hw.zhonguo6118.cn

TS:   s.length
来源：https://nt.zhonguo2118.cn

Java: s.length()
来源：https://sm.zhonguo1118.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：https://fl.zhonguo3118.cn

Ruby: s.length
来源：https://jo.zhonguo5118.cn

C#:   s.Length
来源：https://zq.zhonguo7118.cn

[A23] 大小写转换
来源：https://dm.zhonguo1118.cn

Py:   s.upper(); s.lower(); s.title()
来源：https://pt.zhonguo4118.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：https://wb.zhonguo7118.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：https://sl.zhonguo2118.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：https://zo.zhonguo1118.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：https://id.zhonguo7118.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：https://xs.zhonguo2118.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：https://lw.zhonguo1118.cn

C#:   s.ToUpper(); s.ToLower()
来源：https://jk.zhonguo5118.cn

[A24] 去除首尾空白
来源：https://nz.zhonguo2118.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：https://ft.zhonguo7118.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：https://wo.zhonguo3118.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://ca.zhonguo6118.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://hi.zhonguo3118.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：https://om.zhonguo3118.cn

Go:   strings.TrimSpace(s)
来源：https://cp.zhonguo2118.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：https://mp.zhonguo3118.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：https://xz.zhonguo6118.cn

[A25] 字符串比较
来源：https://jv.zhonguo8118.cn

Py:   s1 == s2; s1 != s2
来源：https://sw.zhonguo5118.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：https://cc.zhonguo3118.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：https://ms.zhonguo5118.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：https://wb.zhonguo4118.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：https://mt.zhonguo7118.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：https://ca.zhonguo5118.cn

Ruby: s1 == s2; s1 <=> s2
来源：https://xz.zhonguo4118.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：https://zk.zhonguo5118.cn

[A26] 类型转换总览
来源：https://wy.zhonguo3118.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：https://ga.zhonguo1118.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：https://jk.zhonguo4118.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：https://ej.zhonguo1118.cn

TS:   Number() String() Boolean() x as number
来源：https://hz.zhonguo3118.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：https://df.zhonguo4118.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：https://hk.zhonguo1118.cn

Ruby: to_i to_f to_s to_sym to_a
来源：https://wx.zhonguo2118.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：https://ht.zhonguo7118.cn

================================================================================
来源：https://ik.zhonguo4118.cn

B. 流程控制
来源：https://nm.zhonguo2118.cn

================================================================================
来源：https://mp.zhonguo7118.cn

[B01] 条件判断 if / else
来源：https://tc.zhonguo6118.cn

Py:   result = "正" if x > 0 else "非正"
来源：https://gp.zhonguo4118.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：https://eq.zhonguo3118.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：https://kv.zhonguo7118.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：https://gv.zhonguo8118.cn

Java: String r = x > 0 ? "正" : "非正";
来源：https://ji.zhonguo2118.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：https://wk.zhonguo7118.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：https://oi.zhonguo1118.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：https://ch.zhonguo2118.cn

[B02] 多分支 else if / elif
来源：https://il.zhonguo2118.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：https://bg.zhonguo8118.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：https://rb.zhonguo3118.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://ev.zhonguo1118.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://aa.zhonguo2118.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://wn.zhonguo3118.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：https://xk.zhonguo3118.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：https://ib.zhonguo6118.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://ut.zhonguo5118.cn

[B03] switch / match / case
来源：https://vl.zhonguo2118.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：https://ni.zhonguo1118.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：https://mk.zhonguo1118.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://io.zhonguo7118.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://wg.zhonguo7118.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：https://yb.zhonguo4118.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：https://ah.zhonguo5118.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：https://rm.zhonguo8118.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：https://ax.zhonguo8118.cn

[B04] for 计数循环
来源：https://wz.zhonguo2118.cn

Py:   for i in range(10): print(i)
来源：https://er.zhonguo4118.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：https://yc.zhonguo3118.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://oe.zhonguo6118.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://fu.zhonguo8118.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：https://wc.zhonguo5118.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：https://vo.zhonguo1118.cn

Ruby: 10.times { |i| puts i }
来源：https://nk.zhonguo8118.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：https://ne.zhonguo2118.cn

[B05] 遍历数组 / 列表
来源：https://in.zhonguo4118.cn

Py:   for item in arr: print(item)
来源：https://xj.zhonguo2118.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：https://fs.zhonguo5118.cn

JS:   for (const item of arr) { console.log(item); }
来源：https://gb.zhonguo8118.cn

TS:   for (const item of arr) { console.log(item); }
来源：https://wi.zhonguo8118.cn

Java: for (var item : arr) { System.out.println(item); }
来源：https://tz.zhonguo7118.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：https://nw.zhonguo5118.cn

Ruby: arr.each { |item| puts item }
来源：https://xh.zhonguo7118.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：https://nk.zhonguo5118.cn

[B06] 遍历字典 / 对象
来源：https://lx.zhonguo4118.cn

Py:   for k, v in d.items(): print(k, v)
来源：https://au.zhonguo2118.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：https://al.zhonguo2118.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://lp.zhonguo5118.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://mq.zhonguo4118.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：https://jg.zhonguo7118.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：https://at.zhonguo4118.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：https://mi.zhonguo2118.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：https://ks.zhonguo2118.cn

[B07] while 循环
来源：https://kp.zhonguo2118.cn

Py:   while i < 10: i += 1
来源：https://gn.zhonguo4118.cn

PHP:  while ($i < 10) { $i++; }
来源：https://oi.zhonguo7118.cn

JS:   while (i < 10) { i++; }
来源：https://xi.zhonguo5118.cn

TS:   while (i < 10) { i++; }
来源：https://ut.zhonguo8118.cn

Java: while (i < 10) { i++; }
来源：https://yk.zhonguo3118.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：https://bo.zhonguo2118.cn

Ruby: while i < 10; i += 1; end
来源：https://kw.zhonguo4118.cn

C#:   while (i < 10) { i++; }
来源：https://dh.zhonguo6118.cn

[B08] do-while（至少执行一次）
来源：https://vk.zhonguo3118.cn

Py:   # 无 do-while：用 while True + break
来源：https://as.zhonguo2118.cn

PHP:  do { $i++; } while ($i < 10);
来源：https://ue.zhonguo1118.cn

JS:   do { i++; } while (i < 10);
来源：https://ab.zhonguo3118.cn

TS:   do { i++; } while (i < 10);
来源：https://ew.zhonguo6118.cn

Java: do { i++; } while (i < 10);
来源：https://rc.zhonguo4118.cn

Go:   for { i++; if i >= 10 { break } }
来源：https://an.zhonguo3118.cn

Ruby: begin; i += 1; end while i < 10
来源：https://vp.zhonguo1118.cn

C#:   do { i++; } while (i < 10);
来源：https://ib.zhonguo2118.cn

[B09] break 与 continue
来源：https://bg.zhonguo8118.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：https://an.zhonguo7118.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：https://uw.zhonguo1118.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://ph.zhonguo7118.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://de.zhonguo1118.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://dc.zhonguo5118.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：https://zi.zhonguo3118.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：https://fv.zhonguo5118.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://wj.zhonguo1118.cn

[B10] 遍历同时拿索引
来源：https://ej.zhonguo3118.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：https://uk.zhonguo2118.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：https://ay.zhonguo4118.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：https://bo.zhonguo5118.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：https://yx.zhonguo5118.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：https://nb.zhonguo2118.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：https://ht.zhonguo5118.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：https://av.zhonguo6118.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：https://fv.zhonguo8118.cn

[B11] 生成数字序列 / 区间
来源：https://je.zhonguo6118.cn

Py:   list(range(0, 10, 2))
来源：https://lg.zhonguo7118.cn

PHP:  range(0, 10, 2);
来源：https://mp.zhonguo1118.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://lv.zhonguo1118.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://ij.zhonguo4118.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：https://gx.zhonguo7118.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：https://vj.zhonguo4118.cn

Ruby: (0...10).step(2).to_a
来源：https://zs.zhonguo8118.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：https://qv.zhonguo5118.cn

[B12] 跳出多层循环
来源：https://rt.zhonguo7118.cn

Py:   # 无标签跳转：抽成函数用 return
来源：https://qk.zhonguo2118.cn

PHP:  # 无标签：用 goto 或函数返回
来源：https://wi.zhonguo5118.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：https://dn.zhonguo8118.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：https://ad.zhonguo7118.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：https://rl.zhonguo4118.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：https://np.zhonguo7118.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：https://rp.zhonguo1118.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：https://ek.zhonguo6118.cn

[B13] 判断是否为数字
来源：https://jn.zhonguo5118.cn

Py:   isinstance(x, (int, float))
来源：https://rw.zhonguo3118.cn

PHP:  is_numeric($x)
来源：https://ou.zhonguo5118.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：https://uw.zhonguo2118.cn


<!-- 参考信息 -->