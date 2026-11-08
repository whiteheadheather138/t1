代发 wailian999

Py:   print("Hello, World!")
来源：https://le.zhonguo2118.cn

PHP:  echo "Hello, World!";
来源：https://lp.zhonguo1118.cn

JS:   console.log("Hello, World!");
来源：https://ej.zhonguo2118.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：https://lc.zhonguo1118.cn

Java: System.out.println("Hello, World!");
来源：https://at.zhonguo5118.cn

Go:   fmt.Println("Hello, World!")
来源：https://il.zhonguo4118.cn

Ruby: puts "Hello, World!"
来源：https://lp.zhonguo8118.cn

C#:   Console.WriteLine("Hello, World!");
来源：https://bp.zhonguo1118.cn

[A02] 变量声明与赋值
来源：https://yn.zhonguo2118.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：https://mo.zhonguo2118.cn

PHP:  $name = "Alex"; $age = 20;
来源：https://vx.zhonguo5118.cn

JS:   let name = "Alex"; const age = 20;
来源：https://jk.zhonguo5118.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：https://lj.zhonguo8118.cn

Java: String name = "Alex"; int age = 20;
来源：https://va.zhonguo6118.cn

Go:   name := "Alex"; age := 20
来源：https://xz.zhonguo8118.cn

Ruby: name = "Alex"; age = 20
来源：https://hq.zhonguo2118.cn

C#:   string name = "Alex"; int age = 20;
来源：https://gp.zhonguo5118.cn

[A03] 常量定义
来源：https://rz.zhonguo1118.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：https://cj.zhonguo8118.cn

PHP:  const PI = 3.14159;
来源：https://jx.zhonguo5118.cn

JS:   const PI = 3.14159;
来源：https://em.zhonguo4118.cn

TS:   const PI: number = 3.14159;
来源：https://qf.zhonguo8118.cn

Java: static final double PI = 3.14159;
来源：https://rt.zhonguo2118.cn

Go:   const PI = 3.14159
来源：https://xy.zhonguo7118.cn

Ruby: PI = 3.14159
来源：https://re.zhonguo8118.cn

C#:   const double PI = 3.14159;
来源：https://mr.zhonguo3118.cn

[A04] 判断变量类型
来源：https://pd.zhonguo8118.cn

Py:   type(x).__name__; isinstance(x, int)
来源：https://cm.zhonguo3118.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：https://fg.zhonguo6118.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：https://zm.zhonguo1118.cn

TS:   typeof x; x instanceof Date
来源：https://dq.zhonguo7118.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：https://fn.zhonguo1118.cn

Go:   reflect.TypeOf(x).Name()
来源：https://qb.zhonguo2118.cn

Ruby: x.class; x.is_a?(Integer)
来源：https://jh.zhonguo2118.cn

C#:   x.GetType().Name; x is int
来源：https://dw.zhonguo2118.cn

[A05] 整数除法与取模
来源：https://ry.zhonguo3118.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：https://eu.zhonguo6118.cn

PHP:  intdiv(7, 2); 7 % 2
来源：https://wf.zhonguo3118.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：https://hv.zhonguo6118.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：https://it.zhonguo3118.cn

Java: 7 / 2; 7 % 2
来源：https://mm.zhonguo1118.cn

Go:   7 / 2; 7 % 2
来源：https://qq.zhonguo8118.cn

Ruby: 7 / 2; 7 % 2
来源：https://mr.zhonguo5118.cn

C#:   7 / 2; 7 % 2
来源：https://bp.zhonguo6118.cn

[A06] 字符串转数字
来源：https://db.zhonguo3118.cn

Py:   int("42"); float("3.14")
来源：https://ub.zhonguo4118.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：https://us.zhonguo8118.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：https://wj.zhonguo5118.cn

TS:   parseInt("42", 10); Number("42")
来源：https://fr.zhonguo6118.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：https://hn.zhonguo3118.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：https://yy.zhonguo4118.cn

Ruby: "42".to_i; "3.14".to_f
来源：https://vz.zhonguo1118.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：https://gk.zhonguo6118.cn

[A07] 数字转字符串
来源：https://lc.zhonguo4118.cn

Py:   str(42)
来源：https://ru.zhonguo7118.cn

PHP:  (string) 42; strval(42)
来源：https://uh.zhonguo5118.cn

JS:   String(42); (42).toString()
来源：https://yy.zhonguo5118.cn

TS:   String(42)
来源：https://qj.zhonguo3118.cn

Java: String.valueOf(42); Integer.toString(42)
来源：https://fu.zhonguo3118.cn

Go:   strconv.Itoa(42)
来源：https://ej.zhonguo1118.cn

Ruby: 42.to_s
来源：https://wf.zhonguo3118.cn

C#:   42.ToString()
来源：https://ff.zhonguo5118.cn

[A08] 取整与四舍五入
来源：https://yv.zhonguo2118.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：https://zt.zhonguo1118.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：https://ww.zhonguo1118.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：https://vy.zhonguo5118.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：https://nn.zhonguo3118.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：https://ha.zhonguo1118.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：https://du.zhonguo4118.cn

Ruby: 3.567.round(2); 3.9.floor
来源：https://hl.zhonguo3118.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：https://wz.zhonguo6118.cn

[A09] 绝对值与最大最小值
来源：https://rr.zhonguo5118.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：https://dh.zhonguo3118.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：https://ja.zhonguo5118.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：https://qh.zhonguo7118.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：https://hs.zhonguo8118.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：https://kk.zhonguo3118.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：https://nv.zhonguo1118.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：https://cx.zhonguo7118.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：https://bm.zhonguo3118.cn

[A10] 生成随机数
来源：https://gz.zhonguo4118.cn

Py:   import random; random.randint(1, 100)
来源：https://xb.zhonguo7118.cn

PHP:  random_int(1, 100);
来源：https://st.zhonguo2118.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：https://nx.zhonguo7118.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：https://ta.zhonguo1118.cn

Java: new Random().nextInt(100) + 1
来源：https://yj.zhonguo1118.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：https://pe.zhonguo7118.cn

Ruby: rand(1..100)
来源：https://px.zhonguo8118.cn

C#:   new Random().Next(1, 101)
来源：https://fk.zhonguo3118.cn

[A11] 条件表达式（三元）
来源：https://kn.zhonguo8118.cn

Py:   "yes" if x > 0 else "no"
来源：https://cd.zhonguo5118.cn

PHP:  $x > 0 ? "yes" : "no"
来源：https://bu.zhonguo7118.cn

JS:   x > 0 ? "yes" : "no"
来源：https://za.zhonguo6118.cn

TS:   x > 0 ? "yes" : "no"
来源：https://xf.zhonguo2118.cn

Java: x > 0 ? "yes" : "no"
来源：https://wh.zhonguo4118.cn

Go:   // 无三元运算符，需用 if 语句
来源：https://fp.zhonguo4118.cn

Ruby: x > 0 ? "yes" : "no"
来源：https://eb.zhonguo8118.cn

C#:   x > 0 ? "yes" : "no"
来源：https://jk.zhonguo5118.cn

[A12] 字符串插值 / 格式化
来源：https://ny.zhonguo3118.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：https://qx.zhonguo6118.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：https://mt.zhonguo4118.cn

JS:   `Hello, ${name}!`
来源：https://ps.zhonguo6118.cn

TS:   `Hello, ${name}!`
来源：https://xd.zhonguo1118.cn

Java: "Hello, %s!".formatted(name)
来源：https://wr.zhonguo6118.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：https://fv.zhonguo6118.cn

Ruby: "Hello, #{name}!"
来源：https://tw.zhonguo8118.cn

C#:   $"Hello, {name}!"
来源：https://xf.zhonguo5118.cn

[A13] 多行字符串（练习 \n 转义）
来源：https://ha.zhonguo5118.cn

Py:   "第一行\n第二行"
来源：https://sx.zhonguo3118.cn

PHP:  "第一行\n第二行"
来源：https://ly.zhonguo4118.cn

JS:   "第一行\n第二行"
来源：https://hi.zhonguo6118.cn

TS:   "第一行\n第二行"
来源：https://pm.zhonguo1118.cn

Java: "第一行\n第二行"
来源：https://yj.zhonguo4118.cn

Go:   "第一行\n第二行"
来源：https://dy.zhonguo2118.cn

Ruby: "第一行\n第二行"
来源：https://vi.zhonguo4118.cn

C#:   "第一行\n第二行"
来源：https://iz.zhonguo2118.cn

[A14] 注释写法
来源：https://xz.zhonguo1118.cn

Py:   # 单行；三引号字符串可作多行说明
来源：https://ss.zhonguo2118.cn

PHP:  // 或 # 单行；/* 多行 */
来源：https://ht.zhonguo1118.cn

JS:   // 单行；/* 多行 */
来源：https://ks.zhonguo6118.cn

TS:   // 单行；/* 多行 */
来源：https://jb.zhonguo3118.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：https://ud.zhonguo7118.cn

Go:   // 单行；/* 多行 */
来源：https://dr.zhonguo2118.cn

Ruby: # 单行；=begin 多行 =end
来源：https://tl.zhonguo7118.cn

C#:   // 单行；/* 多行 */
来源：https://qx.zhonguo1118.cn

[A15] 空值判断与默认值
来源：https://hw.zhonguo5118.cn

Py:   value = data or "默认值"
来源：https://tf.zhonguo1118.cn

PHP:  $value = $data ?? "默认值";
来源：https://jt.zhonguo1118.cn

JS:   const value = data ?? "默认值";
来源：https://ih.zhonguo3118.cn

TS:   const value = data ?? "默认值";
来源：https://di.zhonguo3118.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：https://le.zhonguo4118.cn

Go:   if data == "" { data = "默认值" }
来源：https://xo.zhonguo2118.cn

Ruby: value = data || "默认值"
来源：https://nl.zhonguo2118.cn

C#:   var value = data ?? "默认值";
来源：https://ad.zhonguo6118.cn

[A16] 真假值判断规则
来源：https://ue.zhonguo6118.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：https://gu.zhonguo7118.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：https://fs.zhonguo5118.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：https://cb.zhonguo1118.cn

TS:   if (!x) {}
来源：https://ni.zhonguo1118.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：https://gw.zhonguo1118.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：https://zt.zhonguo8118.cn

Ruby: unless x            # nil 与 false 为假
来源：https://fi.zhonguo6118.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：https://qh.zhonguo4118.cn

[A17] 位运算
来源：https://tr.zhonguo6118.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://ij.zhonguo2118.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：https://yi.zhonguo2118.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://ry.zhonguo2118.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：https://bs.zhonguo8118.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://ta.zhonguo3118.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：https://et.zhonguo1118.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://fg.zhonguo8118.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://qo.zhonguo1118.cn

[A18] 字符与 ASCII 码互转
来源：https://mq.zhonguo2118.cn

Py:   ord("A"); chr(65)
来源：https://kq.zhonguo7118.cn

PHP:  ord("A"); chr(65)
来源：https://px.zhonguo6118.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://su.zhonguo6118.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://kb.zhonguo8118.cn

Java: (int) 'A'; (char) 65
来源：https://nq.zhonguo6118.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：https://hv.zhonguo7118.cn

Ruby: "A".ord; 65.chr
来源：https://ov.zhonguo7118.cn

C#:   (int)'A'; (char)65
来源：https://dn.zhonguo4118.cn

[A19] 交换两个变量
来源：https://vu.zhonguo2118.cn

Py:   a, b = b, a
来源：https://uz.zhonguo1118.cn

PHP:  [$a, $b] = [$b, $a];
来源：https://yz.zhonguo3118.cn

JS:   [a, b] = [b, a];
来源：https://tx.zhonguo8118.cn

TS:   [a, b] = [b, a];
来源：https://ap.zhonguo8118.cn

Java: int t = a; a = b; b = t;
来源：https://wi.zhonguo4118.cn

Go:   a, b = b, a
来源：https://ip.zhonguo4118.cn

Ruby: a, b = b, a
来源：https://lg.zhonguo4118.cn

C#:   (a, b) = (b, a);
来源：https://pa.zhonguo8118.cn

[A20] 读取标准输入
来源：https://sr.zhonguo6118.cn

Py:   name = input("请输入：")
来源：https://uu.zhonguo3118.cn

PHP:  $name = trim(fgets(STDIN));
来源：https://pj.zhonguo3118.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：https://zf.zhonguo6118.cn

TS:   // Node.js：readline 模块
来源：https://zc.zhonguo5118.cn

Java: new Scanner(System.in).nextLine()
来源：https://ke.zhonguo5118.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：https://qa.zhonguo8118.cn

Ruby: gets.chomp
来源：https://ar.zhonguo8118.cn

C#:   Console.ReadLine();
来源：https://xx.zhonguo8118.cn

[A21] 保留指定小数位输出
来源：https://hj.zhonguo4118.cn

Py:   f"{3.14159:.2f}"
来源：https://ym.zhonguo7118.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：https://ww.zhonguo7118.cn

JS:   (3.14159).toFixed(2)
来源：https://rp.zhonguo4118.cn

TS:   (3.14159).toFixed(2)
来源：https://ty.zhonguo8118.cn

Java: String.format("%.2f", 3.14159)
来源：https://yn.zhonguo7118.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：https://xq.zhonguo2118.cn

Ruby: format("%.2f", 3.14159)
来源：https://qr.zhonguo4118.cn

C#:   3.14159.ToString("F2")
来源：https://yp.zhonguo3118.cn

[A22] 获取字符串长度
来源：https://xj.zhonguo5118.cn

Py:   len(s)
来源：https://tc.zhonguo7118.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：https://kg.zhonguo4118.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：https://jj.zhonguo7118.cn

TS:   s.length
来源：https://en.zhonguo3118.cn

Java: s.length()
来源：https://hm.zhonguo7118.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：https://sl.zhonguo6118.cn

Ruby: s.length
来源：https://mw.zhonguo8118.cn

C#:   s.Length
来源：https://zz.zhonguo7118.cn

[A23] 大小写转换
来源：https://xo.zhonguo7118.cn

Py:   s.upper(); s.lower(); s.title()
来源：https://yn.zhonguo4118.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：https://ni.zhonguo4118.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：https://me.zhonguo2118.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：https://ws.zhonguo4118.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：https://cd.zhonguo1118.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：https://ie.zhonguo2118.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：https://ge.zhonguo5118.cn

C#:   s.ToUpper(); s.ToLower()
来源：https://dw.zhonguo2118.cn

[A24] 去除首尾空白
来源：https://zd.zhonguo6118.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：https://kh.zhonguo6118.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：https://xd.zhonguo4118.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://re.zhonguo5118.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://lt.zhonguo4118.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：https://ft.zhonguo4118.cn

Go:   strings.TrimSpace(s)
来源：https://br.zhonguo4118.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：https://as.zhonguo4118.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：https://js.zhonguo2118.cn

[A25] 字符串比较
来源：https://yx.zhonguo3118.cn

Py:   s1 == s2; s1 != s2
来源：https://ph.zhonguo6118.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：https://px.zhonguo5118.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：https://ey.zhonguo8118.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：https://pw.zhonguo2118.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：https://gu.zhonguo1118.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：https://pi.zhonguo2118.cn

Ruby: s1 == s2; s1 <=> s2
来源：https://dz.zhonguo7118.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：https://ry.zhonguo3118.cn

[A26] 类型转换总览
来源：https://vh.zhonguo6118.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：https://nd.zhonguo1118.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：https://vu.zhonguo8118.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：https://pu.zhonguo2118.cn

TS:   Number() String() Boolean() x as number
来源：https://ib.zhonguo3118.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：https://sg.zhonguo1118.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：https://fg.zhonguo1118.cn

Ruby: to_i to_f to_s to_sym to_a
来源：https://bg.zhonguo8118.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：https://be.zhonguo6118.cn

================================================================================
来源：https://ty.zhonguo7118.cn

B. 流程控制
来源：https://ox.zhonguo3118.cn

================================================================================
来源：https://fx.zhonguo5118.cn

[B01] 条件判断 if / else
来源：https://xs.zhonguo6118.cn

Py:   result = "正" if x > 0 else "非正"
来源：https://md.zhonguo1118.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：https://cl.zhonguo7118.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：https://fv.zhonguo6118.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：https://aq.zhonguo4118.cn

Java: String r = x > 0 ? "正" : "非正";
来源：https://lb.zhonguo3118.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：https://gd.zhonguo3118.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：https://zd.zhonguo5118.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：https://cs.zhonguo7118.cn

[B02] 多分支 else if / elif
来源：https://dm.zhonguo6118.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：https://bc.zhonguo7118.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：https://nm.zhonguo7118.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://fh.zhonguo8118.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://wt.zhonguo1118.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://mg.zhonguo7118.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：https://tm.zhonguo5118.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：https://gg.zhonguo7118.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://ad.zhonguo1118.cn

[B03] switch / match / case
来源：https://hw.zhonguo2118.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：https://xp.zhonguo5118.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：https://bj.zhonguo2118.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://lb.zhonguo8118.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://tf.zhonguo1118.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：https://qc.zhonguo2118.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：https://aq.zhonguo5118.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：https://ew.zhonguo8118.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：https://zx.zhonguo4118.cn

[B04] for 计数循环
来源：https://km.zhonguo7118.cn

Py:   for i in range(10): print(i)
来源：https://qw.zhonguo1118.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：https://um.zhonguo5118.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://li.zhonguo7118.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://qz.zhonguo3118.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：https://ih.zhonguo6118.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：https://is.zhonguo5118.cn

Ruby: 10.times { |i| puts i }
来源：https://mb.zhonguo8118.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：https://mc.zhonguo3118.cn

[B05] 遍历数组 / 列表
来源：https://jo.zhonguo4118.cn

Py:   for item in arr: print(item)
来源：https://id.zhonguo5118.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：https://fh.zhonguo1118.cn

JS:   for (const item of arr) { console.log(item); }
来源：https://cx.zhonguo8118.cn

TS:   for (const item of arr) { console.log(item); }
来源：https://cj.zhonguo2118.cn

Java: for (var item : arr) { System.out.println(item); }
来源：https://ob.zhonguo5118.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：https://bk.zhonguo7118.cn

Ruby: arr.each { |item| puts item }
来源：https://fp.zhonguo8118.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：https://kp.zhonguo5118.cn

[B06] 遍历字典 / 对象
来源：https://da.zhonguo2118.cn

Py:   for k, v in d.items(): print(k, v)
来源：https://kg.zhonguo8118.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：https://au.zhonguo5118.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://rc.zhonguo3118.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://js.zhonguo1118.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：https://yd.zhonguo8118.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：https://cr.zhonguo2118.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：https://rd.zhonguo1118.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：https://hb.zhonguo7118.cn

[B07] while 循环
来源：https://bm.zhonguo6118.cn

Py:   while i < 10: i += 1
来源：https://mw.zhonguo1118.cn

PHP:  while ($i < 10) { $i++; }
来源：https://bb.zhonguo5118.cn

JS:   while (i < 10) { i++; }
来源：https://zn.zhonguo3118.cn

TS:   while (i < 10) { i++; }
来源：https://br.zhonguo5118.cn

Java: while (i < 10) { i++; }
来源：https://yt.zhonguo4118.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：https://zt.zhonguo6118.cn

Ruby: while i < 10; i += 1; end
来源：https://hs.zhonguo7118.cn

C#:   while (i < 10) { i++; }
来源：https://ek.zhonguo1118.cn

[B08] do-while（至少执行一次）
来源：https://nd.zhonguo4118.cn


<!-- 参考信息 -->