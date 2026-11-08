代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：https://fs.zhonguo8118.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：https://rk.zhonguo4118.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：https://dc.zhonguo5118.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：https://bh.zhonguo4118.cn

================================================================================
来源：https://cl.zhonguo5118.cn

A. 基础语法与类型
来源：https://mx.zhonguo8118.cn

================================================================================
来源：https://wb.zhonguo5118.cn

[A01] Hello World
来源：https://cl.zhonguo6118.cn

Py:   print("Hello, World!")
来源：https://ma.zhonguo7118.cn

PHP:  echo "Hello, World!";
来源：https://lp.zhonguo4118.cn

JS:   console.log("Hello, World!");
来源：https://op.zhonguo8118.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：https://wx.zhonguo6118.cn

Java: System.out.println("Hello, World!");
来源：https://wm.zhonguo3118.cn

Go:   fmt.Println("Hello, World!")
来源：https://rj.zhonguo8118.cn

Ruby: puts "Hello, World!"
来源：https://nt.zhonguo1118.cn

C#:   Console.WriteLine("Hello, World!");
来源：https://ro.zhonguo6118.cn

[A02] 变量声明与赋值
来源：https://qm.zhonguo2118.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：https://bd.zhonguo5118.cn

PHP:  $name = "Alex"; $age = 20;
来源：https://ah.zhonguo2118.cn

JS:   let name = "Alex"; const age = 20;
来源：https://ur.zhonguo4118.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：https://ab.zhonguo7118.cn

Java: String name = "Alex"; int age = 20;
来源：https://bm.zhonguo3118.cn

Go:   name := "Alex"; age := 20
来源：https://mt.zhonguo3118.cn

Ruby: name = "Alex"; age = 20
来源：https://yf.zhonguo8118.cn

C#:   string name = "Alex"; int age = 20;
来源：https://ns.zhonguo7118.cn

[A03] 常量定义
来源：https://wm.zhonguo7118.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：https://ig.zhonguo6118.cn

PHP:  const PI = 3.14159;
来源：https://zd.zhonguo3118.cn

JS:   const PI = 3.14159;
来源：https://pd.zhonguo8118.cn

TS:   const PI: number = 3.14159;
来源：https://vd.zhonguo6118.cn

Java: static final double PI = 3.14159;
来源：https://ao.zhonguo2118.cn

Go:   const PI = 3.14159
来源：https://sn.zhonguo7118.cn

Ruby: PI = 3.14159
来源：https://ib.zhonguo6118.cn

C#:   const double PI = 3.14159;
来源：https://gx.zhonguo1118.cn

[A04] 判断变量类型
来源：https://kr.zhonguo6118.cn

Py:   type(x).__name__; isinstance(x, int)
来源：https://oz.zhonguo1118.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：https://hv.zhonguo5118.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：https://zo.zhonguo2118.cn

TS:   typeof x; x instanceof Date
来源：https://er.zhonguo5118.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：https://xj.zhonguo2118.cn

Go:   reflect.TypeOf(x).Name()
来源：https://ex.zhonguo5118.cn

Ruby: x.class; x.is_a?(Integer)
来源：https://tj.zhonguo3118.cn

C#:   x.GetType().Name; x is int
来源：https://ru.zhonguo1118.cn

[A05] 整数除法与取模
来源：https://pj.zhonguo5118.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：https://oz.zhonguo3118.cn

PHP:  intdiv(7, 2); 7 % 2
来源：https://kt.zhonguo4118.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：https://en.zhonguo3118.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：https://lb.zhonguo2118.cn

Java: 7 / 2; 7 % 2
来源：https://ba.zhonguo4118.cn

Go:   7 / 2; 7 % 2
来源：https://ma.zhonguo7118.cn

Ruby: 7 / 2; 7 % 2
来源：https://dr.zhonguo7118.cn

C#:   7 / 2; 7 % 2
来源：https://uj.zhonguo8118.cn

[A06] 字符串转数字
来源：https://bb.zhonguo3118.cn

Py:   int("42"); float("3.14")
来源：https://bn.zhonguo4118.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：https://ep.zhonguo5118.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：https://cy.zhonguo2118.cn

TS:   parseInt("42", 10); Number("42")
来源：https://jm.zhonguo6118.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：https://yc.zhonguo2118.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：https://ru.zhonguo5118.cn

Ruby: "42".to_i; "3.14".to_f
来源：https://kr.zhonguo4118.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：https://ue.zhonguo7118.cn

[A07] 数字转字符串
来源：https://oo.zhonguo2118.cn

Py:   str(42)
来源：https://js.zhonguo3118.cn

PHP:  (string) 42; strval(42)
来源：https://ow.zhonguo4118.cn

JS:   String(42); (42).toString()
来源：https://xk.zhonguo4118.cn

TS:   String(42)
来源：https://cd.zhonguo3118.cn

Java: String.valueOf(42); Integer.toString(42)
来源：https://bb.zhonguo1118.cn

Go:   strconv.Itoa(42)
来源：https://uh.zhonguo6118.cn

Ruby: 42.to_s
来源：https://ne.zhonguo7118.cn

C#:   42.ToString()
来源：https://xg.zhonguo2118.cn

[A08] 取整与四舍五入
来源：https://ab.zhonguo2118.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：https://bi.zhonguo5118.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：https://fu.zhonguo3118.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：https://ho.zhonguo8118.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：https://cm.zhonguo4118.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：https://ia.zhonguo8118.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：https://gh.zhonguo8118.cn

Ruby: 3.567.round(2); 3.9.floor
来源：https://st.zhonguo2118.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：https://if.zhonguo2118.cn

[A09] 绝对值与最大最小值
来源：https://zs.zhonguo1118.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：https://ru.zhonguo8118.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：https://bs.zhonguo4118.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：https://ka.zhonguo1118.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：https://he.zhonguo7118.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：https://rg.zhonguo5118.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：https://tc.zhonguo3118.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：https://lo.zhonguo6118.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：https://dg.zhonguo7118.cn

[A10] 生成随机数
来源：https://df.zhonguo8118.cn

Py:   import random; random.randint(1, 100)
来源：https://qo.zhonguo6118.cn

PHP:  random_int(1, 100);
来源：https://mw.zhonguo8118.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：https://ko.zhonguo3118.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：https://bk.zhonguo5118.cn

Java: new Random().nextInt(100) + 1
来源：https://tu.zhonguo1118.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：https://nh.zhonguo3118.cn

Ruby: rand(1..100)
来源：https://oi.zhonguo8118.cn

C#:   new Random().Next(1, 101)
来源：https://ux.zhonguo2118.cn

[A11] 条件表达式（三元）
来源：https://yl.zhonguo6118.cn

Py:   "yes" if x > 0 else "no"
来源：https://nl.zhonguo6118.cn

PHP:  $x > 0 ? "yes" : "no"
来源：https://tl.zhonguo5118.cn

JS:   x > 0 ? "yes" : "no"
来源：https://en.zhonguo3118.cn

TS:   x > 0 ? "yes" : "no"
来源：https://np.zhonguo3118.cn

Java: x > 0 ? "yes" : "no"
来源：https://tn.zhonguo7118.cn

Go:   // 无三元运算符，需用 if 语句
来源：https://lp.zhonguo5118.cn

Ruby: x > 0 ? "yes" : "no"
来源：https://tq.zhonguo1118.cn

C#:   x > 0 ? "yes" : "no"
来源：https://eg.zhonguo8118.cn

[A12] 字符串插值 / 格式化
来源：https://ld.zhonguo4118.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：https://vs.zhonguo6118.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：https://ql.zhonguo1118.cn

JS:   `Hello, ${name}!`
来源：https://wa.zhonguo3118.cn

TS:   `Hello, ${name}!`
来源：https://ie.zhonguo6118.cn

Java: "Hello, %s!".formatted(name)
来源：https://vo.zhonguo7118.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：https://eo.zhonguo7118.cn

Ruby: "Hello, #{name}!"
来源：https://kd.zhonguo8118.cn

C#:   $"Hello, {name}!"
来源：https://sb.zhonguo2118.cn

[A13] 多行字符串（练习 \n 转义）
来源：https://bd.zhonguo6118.cn

Py:   "第一行\n第二行"
来源：https://bj.zhonguo2118.cn

PHP:  "第一行\n第二行"
来源：https://un.zhonguo7118.cn

JS:   "第一行\n第二行"
来源：https://ka.zhonguo3118.cn

TS:   "第一行\n第二行"
来源：https://gr.zhonguo6118.cn

Java: "第一行\n第二行"
来源：https://vc.zhonguo3118.cn

Go:   "第一行\n第二行"
来源：https://kc.zhonguo4118.cn

Ruby: "第一行\n第二行"
来源：https://ee.zhonguo1118.cn

C#:   "第一行\n第二行"
来源：https://pv.zhonguo2118.cn

[A14] 注释写法
来源：https://mi.zhonguo8118.cn

Py:   # 单行；三引号字符串可作多行说明
来源：https://rb.zhonguo2118.cn

PHP:  // 或 # 单行；/* 多行 */
来源：https://xs.zhonguo6118.cn

JS:   // 单行；/* 多行 */
来源：https://pb.zhonguo3118.cn

TS:   // 单行；/* 多行 */
来源：https://ab.zhonguo2118.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：https://ip.zhonguo1118.cn

Go:   // 单行；/* 多行 */
来源：https://fd.zhonguo4118.cn

Ruby: # 单行；=begin 多行 =end
来源：https://bp.zhonguo5118.cn

C#:   // 单行；/* 多行 */
来源：https://nq.zhonguo1118.cn

[A15] 空值判断与默认值
来源：https://se.zhonguo1118.cn

Py:   value = data or "默认值"
来源：https://uc.zhonguo2118.cn

PHP:  $value = $data ?? "默认值";
来源：https://zb.zhonguo3118.cn

JS:   const value = data ?? "默认值";
来源：https://je.zhonguo1118.cn

TS:   const value = data ?? "默认值";
来源：https://xr.zhonguo3118.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：https://dw.zhonguo2118.cn

Go:   if data == "" { data = "默认值" }
来源：https://it.zhonguo8118.cn

Ruby: value = data || "默认值"
来源：https://ya.zhonguo5118.cn

C#:   var value = data ?? "默认值";
来源：https://lq.zhonguo8118.cn

[A16] 真假值判断规则
来源：https://ns.zhonguo6118.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：https://ry.zhonguo3118.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：https://qu.zhonguo1118.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：https://fm.zhonguo3118.cn

TS:   if (!x) {}
来源：https://do.zhonguo5118.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：https://jt.zhonguo3118.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：https://ez.zhonguo6118.cn

Ruby: unless x            # nil 与 false 为假
来源：https://hc.zhonguo4118.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：https://ry.zhonguo4118.cn

[A17] 位运算
来源：https://jm.zhonguo7118.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://au.zhonguo2118.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：https://is.zhonguo8118.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://ub.zhonguo6118.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：https://uj.zhonguo4118.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://ly.zhonguo2118.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：https://gh.zhonguo6118.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://am.zhonguo2118.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://qg.zhonguo3118.cn

[A18] 字符与 ASCII 码互转
来源：https://zm.zhonguo1118.cn

Py:   ord("A"); chr(65)
来源：https://lw.zhonguo1118.cn

PHP:  ord("A"); chr(65)
来源：https://pb.zhonguo6118.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://zb.zhonguo7118.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://al.zhonguo8118.cn

Java: (int) 'A'; (char) 65
来源：https://uj.zhonguo2118.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：https://tr.zhonguo7118.cn

Ruby: "A".ord; 65.chr
来源：https://ze.zhonguo8118.cn

C#:   (int)'A'; (char)65
来源：https://gm.zhonguo8118.cn

[A19] 交换两个变量
来源：https://ov.zhonguo6118.cn

Py:   a, b = b, a
来源：https://vh.zhonguo1118.cn

PHP:  [$a, $b] = [$b, $a];
来源：https://fh.zhonguo8118.cn

JS:   [a, b] = [b, a];
来源：https://ko.zhonguo6118.cn

TS:   [a, b] = [b, a];
来源：https://mf.zhonguo7118.cn

Java: int t = a; a = b; b = t;
来源：https://fv.zhonguo7118.cn

Go:   a, b = b, a
来源：https://ca.zhonguo4118.cn

Ruby: a, b = b, a
来源：https://oj.zhonguo6118.cn

C#:   (a, b) = (b, a);
来源：https://ch.zhonguo7118.cn

[A20] 读取标准输入
来源：https://pf.zhonguo5118.cn

Py:   name = input("请输入：")
来源：https://cz.zhonguo8118.cn

PHP:  $name = trim(fgets(STDIN));
来源：https://lb.zhonguo5118.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：https://tt.zhonguo8118.cn

TS:   // Node.js：readline 模块
来源：https://hy.zhonguo2118.cn

Java: new Scanner(System.in).nextLine()
来源：https://ar.zhonguo2118.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：https://fv.zhonguo5118.cn

Ruby: gets.chomp
来源：https://jo.zhonguo6118.cn

C#:   Console.ReadLine();
来源：https://sl.zhonguo6118.cn

[A21] 保留指定小数位输出
来源：https://bu.zhonguo8118.cn

Py:   f"{3.14159:.2f}"
来源：https://oa.zhonguo2118.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：https://lw.zhonguo1118.cn

JS:   (3.14159).toFixed(2)
来源：https://ni.zhonguo6118.cn

TS:   (3.14159).toFixed(2)
来源：https://gg.zhonguo1118.cn

Java: String.format("%.2f", 3.14159)
来源：https://ex.zhonguo5118.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：https://ke.zhonguo2118.cn

Ruby: format("%.2f", 3.14159)
来源：https://qx.zhonguo6118.cn

C#:   3.14159.ToString("F2")
来源：https://mj.zhonguo5118.cn

[A22] 获取字符串长度
来源：https://mt.zhonguo7118.cn

Py:   len(s)
来源：https://lw.zhonguo2118.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：https://em.zhonguo3118.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：https://sg.zhonguo8118.cn

TS:   s.length
来源：https://pv.zhonguo5118.cn

Java: s.length()
来源：https://af.zhonguo1118.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：https://xp.zhonguo8118.cn

Ruby: s.length
来源：https://sr.zhonguo6118.cn

C#:   s.Length
来源：https://za.zhonguo3118.cn

[A23] 大小写转换
来源：https://ri.zhonguo1118.cn

Py:   s.upper(); s.lower(); s.title()
来源：https://io.zhonguo8118.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：https://yf.zhonguo6118.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：https://rw.zhonguo3118.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：https://nq.zhonguo7118.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：https://pc.zhonguo5118.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：https://pz.zhonguo4118.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：https://hd.zhonguo1118.cn

C#:   s.ToUpper(); s.ToLower()
来源：https://my.zhonguo5118.cn

[A24] 去除首尾空白
来源：https://cn.zhonguo5118.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：https://yy.zhonguo2118.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：https://aq.zhonguo4118.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://gj.zhonguo6118.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：https://bk.zhonguo3118.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：https://ln.zhonguo6118.cn

Go:   strings.TrimSpace(s)
来源：https://gq.zhonguo1118.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：https://rh.zhonguo4118.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：https://cy.zhonguo4118.cn

[A25] 字符串比较
来源：https://ux.zhonguo7118.cn

Py:   s1 == s2; s1 != s2
来源：https://wk.zhonguo6118.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：https://ho.zhonguo5118.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：https://xr.zhonguo6118.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：https://xc.zhonguo2118.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：https://qy.zhonguo8118.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：https://lu.zhonguo8118.cn

Ruby: s1 == s2; s1 <=> s2
来源：https://nb.zhonguo8118.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：https://ox.zhonguo5118.cn

[A26] 类型转换总览
来源：https://cx.zhonguo1118.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：https://qw.zhonguo3118.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：https://iu.zhonguo2118.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：https://ib.zhonguo6118.cn

TS:   Number() String() Boolean() x as number
来源：https://jy.zhonguo6118.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：https://fv.zhonguo5118.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：https://ud.zhonguo5118.cn

Ruby: to_i to_f to_s to_sym to_a
来源：https://jg.zhonguo5118.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：https://fx.zhonguo8118.cn

================================================================================
来源：https://xp.zhonguo3118.cn

B. 流程控制
来源：https://ft.zhonguo5118.cn

================================================================================
来源：https://rh.zhonguo5118.cn

[B01] 条件判断 if / else
来源：https://mw.zhonguo6118.cn

Py:   result = "正" if x > 0 else "非正"
来源：https://sy.zhonguo3118.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：https://kl.zhonguo8118.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：https://mz.zhonguo6118.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：https://cy.zhonguo5118.cn

Java: String r = x > 0 ? "正" : "非正";
来源：https://uc.zhonguo8118.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：https://zj.zhonguo2118.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：https://kc.zhonguo4118.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：https://jr.zhonguo4118.cn

[B02] 多分支 else if / elif
来源：https://mv.zhonguo4118.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：https://zt.zhonguo6118.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：https://bg.zhonguo7118.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://ks.zhonguo4118.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://kg.zhonguo1118.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://qc.zhonguo8118.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：https://sa.zhonguo7118.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：https://ov.zhonguo2118.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：https://lr.zhonguo7118.cn

[B03] switch / match / case
来源：https://ro.zhonguo2118.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：https://mt.zhonguo6118.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：https://is.zhonguo8118.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://es.zhonguo4118.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：https://aw.zhonguo7118.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：https://oy.zhonguo4118.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：https://ha.zhonguo8118.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：https://im.zhonguo2118.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：https://cj.zhonguo5118.cn

[B04] for 计数循环
来源：https://ey.zhonguo7118.cn

Py:   for i in range(10): print(i)
来源：https://fi.zhonguo2118.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：https://dz.zhonguo2118.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://xe.zhonguo2118.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：https://kr.zhonguo7118.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：https://vr.zhonguo5118.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：https://tf.zhonguo7118.cn

Ruby: 10.times { |i| puts i }
来源：https://qr.zhonguo1118.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：https://ze.zhonguo2118.cn

[B05] 遍历数组 / 列表
来源：https://st.zhonguo3118.cn

Py:   for item in arr: print(item)
来源：https://dg.zhonguo4118.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：https://vx.zhonguo6118.cn

JS:   for (const item of arr) { console.log(item); }
来源：https://ji.zhonguo2118.cn

TS:   for (const item of arr) { console.log(item); }
来源：https://lh.zhonguo2118.cn

Java: for (var item : arr) { System.out.println(item); }
来源：https://br.zhonguo5118.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：https://bp.zhonguo5118.cn

Ruby: arr.each { |item| puts item }
来源：https://ku.zhonguo8118.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：https://np.zhonguo7118.cn

[B06] 遍历字典 / 对象
来源：https://nj.zhonguo7118.cn

Py:   for k, v in d.items(): print(k, v)
来源：https://fd.zhonguo1118.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：https://hb.zhonguo1118.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://oh.zhonguo4118.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://rc.zhonguo1118.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：https://fc.zhonguo6118.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：https://xj.zhonguo7118.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：https://km.zhonguo6118.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：https://qy.zhonguo2118.cn

[B07] while 循环
来源：https://fq.zhonguo7118.cn

Py:   while i < 10: i += 1
来源：https://ra.zhonguo7118.cn


<!-- 参考信息 -->