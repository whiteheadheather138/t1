代发 wailian999

[A02] 变量声明与赋值
来源：http://wap.fktsv.cn/Article/details/gpbtghrgt.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.yfazqb.com/Article/details/gekqnuzyr.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.epnwcf.com/Article/details/gngnjoybb.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.bbcook.cn/Article/details/gcqaytpej.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.fktsv.cn/Article/details/gojoqrsyu.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.yfazqb.com/Article/details/gcraqavsq.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.yfazqb.com/Article/details/guyuhjxdk.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.tarul.cn/Article/details/gkswbtced.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.bbcook.cn/Article/details/gwomumnec.sHtML

[A03] 常量定义
来源：http://3g.vehdjk.com/Article/details/gylmmnfzr.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.bbcook.cn/Article/details/gdihkefbb.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.epnwcf.com/Article/details/gdocgfpcv.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.yfazqb.com/Article/details/gznmtkezn.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.bbcook.cn/Article/details/gzdzrhzmp.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.epnwcf.com/Article/details/goeokhcmn.sHtML

Go:   const PI = 3.14159
来源：http://m.share.fktsv.cn/Article/details/grpjtkode.sHtML

Ruby: PI = 3.14159
来源：http://m.share.sjlbkw.cn/Article/details/gidvfjdgy.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.vehdjk.com/Article/details/glamopzwj.sHtML

[A04] 判断变量类型
来源：http://m.share.bbcook.cn/Article/details/gymopwvxs.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.tarul.cn/Article/details/gpiigovgd.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.epnwcf.com/Article/details/gqvzyezgh.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.epnwcf.com/Article/details/gsfrzaxoz.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.sjlbkw.cn/Article/details/gxsizvxqz.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.fktsv.cn/Article/details/gradtgzxw.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.fktsv.cn/Article/details/gnkfarscp.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.epnwcf.com/Article/details/gvxxcyxpb.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.tarul.cn/Article/details/gaywybkrb.sHtML

[A05] 整数除法与取模
来源：http://www.blog.epnwcf.com/Article/details/gcjukfcoi.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.epnwcf.com/Article/details/gmvzbbiac.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.tarul.cn/Article/details/ghkzvsocr.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.bbcook.cn/Article/details/gwqbvgkjd.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.sjlbkw.cn/Article/details/ggwrclqnl.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.bbcook.cn/Article/details/gedbpnbjm.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.tarul.cn/Article/details/gkmxqhovw.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.epnwcf.com/Article/details/ggzqsysqo.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.tarul.cn/Article/details/gqcznacct.sHtML

[A06] 字符串转数字
来源：http://mobile.sjlbkw.cn/Article/details/gjvpgckqo.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.bbcook.cn/Article/details/grqvnimib.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.fktsv.cn/Article/details/ghlkynibi.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.fktsv.cn/Article/details/gdryjoifb.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.tarul.cn/Article/details/glelmedfq.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.vehdjk.com/Article/details/gcvucgttd.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.bbcook.cn/Article/details/gprqyezga.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.yfazqb.com/Article/details/geftfgsua.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.bbcook.cn/Article/details/gxrpehbmi.sHtML

[A07] 数字转字符串
来源：http://wap.tarul.cn/Article/details/gxloeueif.sHtML

Py:   str(42)
来源：http://www.share.epnwcf.com/Article/details/gpaksrdii.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.fktsv.cn/Article/details/gybnythts.sHtML

JS:   String(42); (42).toString()
来源：http://wap.yfazqb.com/Article/details/ggozycuvk.sHtML

TS:   String(42)
来源：http://read.share.yfazqb.com/Article/details/ggplcdmwc.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.tarul.cn/Article/details/gkpckfuow.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.sjlbkw.cn/Article/details/gxwzudwic.sHtML

Ruby: 42.to_s
来源：http://3g.sjlbkw.cn/Article/details/gjuroewvk.sHtML

C#:   42.ToString()
来源：http://www.share.bbcook.cn/Article/details/gulcqsuxp.sHtML

[A08] 取整与四舍五入
来源：http://www.share.epnwcf.com/Article/details/gvbtndzfk.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.sjlbkw.cn/Article/details/gdrvssumf.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.tarul.cn/Article/details/gqmjraaec.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.yfazqb.com/Article/details/gqauaqese.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.fktsv.cn/Article/details/gwrmnapku.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.fktsv.cn/Article/details/godpodyjn.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.sjlbkw.cn/Article/details/girthzckk.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.vehdjk.com/Article/details/gsvtbaono.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.epnwcf.com/Article/details/gmpuaeqpd.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.vehdjk.com/Article/details/ghukfvqdq.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fktsv.cn/Article/details/ghdpckahu.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.bbcook.cn/Article/details/gjeifflhg.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.fktsv.cn/Article/details/gombnakub.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gdojjtpif.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.epnwcf.com/Article/details/gahdpgoaq.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.fktsv.cn/Article/details/gqzyurtat.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.bbcook.cn/Article/details/gdscpakdc.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.vehdjk.com/Article/details/gbweykqrw.sHtML

[A10] 生成随机数
来源：http://3g.sjlbkw.cn/Article/details/gsohroddt.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.bbcook.cn/Article/details/gghrfdpxg.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.sjlbkw.cn/Article/details/gvwbnwovx.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.vehdjk.com/Article/details/gtbqhhztv.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.bbcook.cn/Article/details/glhxarjmb.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.bbcook.cn/Article/details/gtknkuasd.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.fktsv.cn/Article/details/ggqvhrfuc.sHtML

Ruby: rand(1..100)
来源：http://3g.vehdjk.com/Article/details/gafodprsp.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.tarul.cn/Article/details/gytmcmuwa.sHtML

[A11] 条件表达式（三元）
来源：http://baike.vehdjk.com/Article/details/gyzypigiv.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.sjlbkw.cn/Article/details/ggcdisdun.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.tarul.cn/Article/details/glpvapkpq.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.yfazqb.com/Article/details/gsrnhnucf.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.fktsv.cn/Article/details/gsouuyhuo.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.tarul.cn/Article/details/gkmptumph.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.epnwcf.com/Article/details/gzntmyaac.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.sjlbkw.cn/Article/details/gcsykgfws.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.tarul.cn/Article/details/grezcfnlq.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.tarul.cn/Article/details/gkhfmnmzz.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.yfazqb.com/Article/details/gqjkssgjq.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.yfazqb.com/Article/details/gnbpdwbxp.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.bbcook.cn/Article/details/grgctczoe.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.sjlbkw.cn/Article/details/gqrhrnrgb.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.tarul.cn/Article/details/grolqaayt.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.yfazqb.com/Article/details/gpnjnuhzd.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.yfazqb.com/Article/details/gnfzddkgn.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.sjlbkw.cn/Article/details/gvggfjxmz.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.yfazqb.com/Article/details/grlrncgih.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.sjlbkw.cn/Article/details/gjmkacexb.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.yfazqb.com/Article/details/gkjtoixcv.sHtML

JS:   "第一行\n第二行"
来源：http://3g.yfazqb.com/Article/details/gksvgyaqk.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.sjlbkw.cn/Article/details/gjczgqsmh.sHtML

Java: "第一行\n第二行"
来源：http://wap.sjlbkw.cn/Article/details/gauxceirp.sHtML

Go:   "第一行\n第二行"
来源：http://blog.vehdjk.com/Article/details/gopcrkxrx.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.yfazqb.com/Article/details/gvduubmio.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.vehdjk.com/Article/details/gblvtnmtl.sHtML

[A14] 注释写法
来源：http://www.m.share.yfazqb.com/Article/details/glqxitbaf.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.vehdjk.com/Article/details/gmxmyrfmh.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.vehdjk.com/Article/details/gvgrcbjkd.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.vehdjk.com/Article/details/gkjuaiohz.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.fktsv.cn/Article/details/gxbcjyicm.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.tarul.cn/Article/details/gsgpulnsk.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.yfazqb.com/Article/details/gttgqerdu.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.fktsv.cn/Article/details/gnkhfufeh.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.yfazqb.com/Article/details/ggljwaoht.sHtML

[A15] 空值判断与默认值
来源：http://wap.bbcook.cn/Article/details/ggjhcyxjt.sHtML

Py:   value = data or "默认值"
来源：http://www.share.epnwcf.com/Article/details/gziezioav.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.epnwcf.com/Article/details/geqggkxry.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.fktsv.cn/Article/details/glgijmdks.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.tarul.cn/Article/details/goepoepvp.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.tarul.cn/Article/details/gbrualovq.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.epnwcf.com/Article/details/ghgrspnxm.sHtML

Ruby: value = data || "默认值"
来源：http://blog.tarul.cn/Article/details/geglzugpm.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.fktsv.cn/Article/details/gcyvnqxbi.sHtML

[A16] 真假值判断规则
来源：http://www.share.tarul.cn/Article/details/gzjtjcdlh.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.yfazqb.com/Article/details/gaafglxdb.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.tarul.cn/Article/details/grwsurtjt.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.tarul.cn/Article/details/gnhptdbgv.sHtML

TS:   if (!x) {}
来源：http://www.share.yfazqb.com/Article/details/gyrvzivvn.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.yfazqb.com/Article/details/gswtrvmlg.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.yfazqb.com/Article/details/gihoayemd.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.bbcook.cn/Article/details/gnlwptcju.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.fktsv.cn/Article/details/gjdwluqjy.sHtML

[A17] 位运算
来源：http://wap.yfazqb.com/Article/details/gtikvyokx.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.yfazqb.com/Article/details/gipiriilj.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.vehdjk.com/Article/details/gngekbuze.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fktsv.cn/Article/details/gynetqltl.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.sjlbkw.cn/Article/details/gfdksuxsv.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.epnwcf.com/Article/details/grhoujfoh.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.tarul.cn/Article/details/gyibsdhoy.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.bbcook.cn/Article/details/gfwzccrur.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.yfazqb.com/Article/details/gmzgjazlh.sHtML

[A18] 字符与 ASCII 码互转
来源：http://m.share.sjlbkw.cn/Article/details/gplgmqjfh.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.bbcook.cn/Article/details/gxxlzxvjm.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.yfazqb.com/Article/details/guaxtyiou.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.epnwcf.com/Article/details/gdacobzmq.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.vehdjk.com/Article/details/gymmwzmox.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.yfazqb.com/Article/details/gmbkggbqk.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.epnwcf.com/Article/details/gpmoqaizv.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.sjlbkw.cn/Article/details/gdlspyivb.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.tarul.cn/Article/details/gnpovtkzf.sHtML

[A19] 交换两个变量
来源：http://wap.yfazqb.com/Article/details/gpzidcfqp.sHtML

Py:   a, b = b, a
来源：http://baike.tarul.cn/Article/details/gnpiemlsl.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.fktsv.cn/Article/details/gmwjvmmud.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.yfazqb.com/Article/details/gwxysqpqw.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.sjlbkw.cn/Article/details/gumncqxrl.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.bbcook.cn/Article/details/gtxnjyxgj.sHtML

Go:   a, b = b, a
来源：http://read.share.yfazqb.com/Article/details/gdlsxdrfl.sHtML

Ruby: a, b = b, a
来源：http://www.blog.sjlbkw.cn/Article/details/gjwhmhhsy.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.tarul.cn/Article/details/gsalpnxij.sHtML

[A20] 读取标准输入
来源：http://read.share.fktsv.cn/Article/details/glhxqgiws.sHtML

Py:   name = input("请输入：")
来源：http://read.share.yfazqb.com/Article/details/gpfwkaoou.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.vehdjk.com/Article/details/ggvwmpnyq.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.vehdjk.com/Article/details/gjunsajay.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.epnwcf.com/Article/details/gmqrhxygg.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.fktsv.cn/Article/details/gibutrpth.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.epnwcf.com/Article/details/ghywkgnar.sHtML

Ruby: gets.chomp
来源：http://www.share.tarul.cn/Article/details/gqevirqho.sHtML

C#:   Console.ReadLine();
来源：http://m.share.vehdjk.com/Article/details/gwivhlpry.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.yfazqb.com/Article/details/gnjrklrqu.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.epnwcf.com/Article/details/gubnyxjwb.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.vehdjk.com/Article/details/gsnwiwflm.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.tarul.cn/Article/details/gecolmhph.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.vehdjk.com/Article/details/ghbyugfam.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.yfazqb.com/Article/details/grorxkqau.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.tarul.cn/Article/details/gobapnmyv.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.fktsv.cn/Article/details/gadjcmwmr.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.vehdjk.com/Article/details/gllqpknmi.sHtML

[A22] 获取字符串长度
来源：http://www.blog.bbcook.cn/Article/details/gluhihtwm.sHtML

Py:   len(s)
来源：http://www.m.share.bbcook.cn/Article/details/gvlqvmeok.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.vehdjk.com/Article/details/gwjddiiyr.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.epnwcf.com/Article/details/gvaqvoxlr.sHtML

TS:   s.length
来源：http://www.blog.bbcook.cn/Article/details/gwtmiyxrl.sHtML

Java: s.length()
来源：http://read.share.yfazqb.com/Article/details/gdepbyzea.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.fktsv.cn/Article/details/gshzbaxyk.sHtML

Ruby: s.length
来源：http://www.blog.sjlbkw.cn/Article/details/gsuhuzzzc.sHtML

C#:   s.Length
来源：http://baike.fktsv.cn/Article/details/gnxlckkfj.sHtML

[A23] 大小写转换
来源：http://baike.tarul.cn/Article/details/ggzcsvqqe.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.bbcook.cn/Article/details/gsjpmgvse.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.fktsv.cn/Article/details/gjectgbfg.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.bbcook.cn/Article/details/gxqoxyzvw.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.fktsv.cn/Article/details/gxnzbvqxr.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.vehdjk.com/Article/details/gejnrxgwy.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.sjlbkw.cn/Article/details/gyaafyeer.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.bbcook.cn/Article/details/gtscnjbzs.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.bbcook.cn/Article/details/gkjuklyot.sHtML

[A24] 去除首尾空白
来源：http://blog.bbcook.cn/Article/details/gegwuruio.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.bbcook.cn/Article/details/gnjiqaefl.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.bbcook.cn/Article/details/geptrwock.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.fktsv.cn/Article/details/gitfrhqhr.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fktsv.cn/Article/details/gqnkvgqyd.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.fktsv.cn/Article/details/gamusecte.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.sjlbkw.cn/Article/details/gmqsfobhl.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.sjlbkw.cn/Article/details/grwsylctv.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.sjlbkw.cn/Article/details/gkybbafgq.sHtML

[A25] 字符串比较
来源：http://read.share.vehdjk.com/Article/details/goamokkvu.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.sjlbkw.cn/Article/details/gtkiiguvg.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.vehdjk.com/Article/details/gbmcskzop.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fktsv.cn/Article/details/gaweblrbh.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.vehdjk.com/Article/details/gtohrtwuz.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.vehdjk.com/Article/details/gbayuaouq.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.yfazqb.com/Article/details/gljqqiham.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.sjlbkw.cn/Article/details/gvhjscwbn.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.vehdjk.com/Article/details/gdwseeoha.sHtML

[A26] 类型转换总览
来源：http://baike.fktsv.cn/Article/details/ghrplodqh.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.yfazqb.com/Article/details/gfxjrbkpe.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.yfazqb.com/Article/details/gjuxfnfeh.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.fktsv.cn/Article/details/govkkidef.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.sjlbkw.cn/Article/details/grmknuiwn.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.vehdjk.com/Article/details/gtjrenehn.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.tarul.cn/Article/details/goiimckzx.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.yfazqb.com/Article/details/gbavlxdmi.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.bbcook.cn/Article/details/gpxvejojm.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gvkmkhwqp.sHtML

B. 流程控制
来源：http://m.share.vehdjk.com/Article/details/gkkjdxlwu.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/ghxlbhtnp.sHtML

[B01] 条件判断 if / else
来源：http://3g.sjlbkw.cn/Article/details/gpqaqxken.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.bbcook.cn/Article/details/ghqoijhhp.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.tarul.cn/Article/details/gtqppxsfl.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.yfazqb.com/Article/details/gguilecee.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.epnwcf.com/Article/details/gvxaytvfp.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.tarul.cn/Article/details/grpffdqkn.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.sjlbkw.cn/Article/details/gwlkexnkz.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.bbcook.cn/Article/details/gwnloyhlp.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.epnwcf.com/Article/details/grjabvtoj.sHtML

[B02] 多分支 else if / elif
来源：http://wap.fktsv.cn/Article/details/gkdsqwnob.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.tarul.cn/Article/details/gtanjjqgm.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.epnwcf.com/Article/details/gbofrsocy.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.tarul.cn/Article/details/gagykvgha.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.epnwcf.com/Article/details/gnymuxfte.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.sjlbkw.cn/Article/details/grugbxshl.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.fktsv.cn/Article/details/gcqbltyeh.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.vehdjk.com/Article/details/gsduvdtmi.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fktsv.cn/Article/details/gzsflxnlp.sHtML

[B03] switch / match / case
来源：http://www.m.share.vehdjk.com/Article/details/gfnbqobai.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.vehdjk.com/Article/details/geygszbgm.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.fktsv.cn/Article/details/gawqjrbzg.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.vehdjk.com/Article/details/glmwndmhc.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.bbcook.cn/Article/details/gmmkqzgpl.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.tarul.cn/Article/details/gjhisezlz.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.fktsv.cn/Article/details/gjkrbcisd.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.sjlbkw.cn/Article/details/giucandis.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.epnwcf.com/Article/details/gvwxwabvu.sHtML

[B04] for 计数循环
来源：http://m.share.yfazqb.com/Article/details/gkjbiidmm.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.vehdjk.com/Article/details/gvipogjge.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.yfazqb.com/Article/details/gjdxlpjrb.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fktsv.cn/Article/details/gqimucnur.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjaugfusy.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.yfazqb.com/Article/details/grrlrdxbg.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.yfazqb.com/Article/details/goodizqiv.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.epnwcf.com/Article/details/gguyhhovg.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.fktsv.cn/Article/details/gylgrbfdu.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.fktsv.cn/Article/details/gewiohqaq.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.fktsv.cn/Article/details/gwpcjrlpk.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.bbcook.cn/Article/details/gpnkvgepe.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.epnwcf.com/Article/details/gkfhiofro.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.sjlbkw.cn/Article/details/grkhjfuae.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.fktsv.cn/Article/details/gdwkcymlp.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.tarul.cn/Article/details/gpbhjjmyy.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.tarul.cn/Article/details/gggjmbppb.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.sjlbkw.cn/Article/details/gszolfyol.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.vehdjk.com/Article/details/gcchberaa.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.vehdjk.com/Article/details/gcdiovmpb.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.bbcook.cn/Article/details/gxexbuids.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fktsv.cn/Article/details/gdphxrxsw.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.sjlbkw.cn/Article/details/gvtijgcjd.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.epnwcf.com/Article/details/gqhihawwn.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.epnwcf.com/Article/details/glznvplgz.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.tarul.cn/Article/details/gakzoydmg.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.yfazqb.com/Article/details/gzstgeohd.sHtML

[B07] while 循环
来源：http://mobile.fktsv.cn/Article/details/gunoglxff.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.sjlbkw.cn/Article/details/gpsbefols.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.fktsv.cn/Article/details/gifbtvsat.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.fktsv.cn/Article/details/gmrfoeyjj.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.epnwcf.com/Article/details/gcdzizile.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.tarul.cn/Article/details/graxnkmfm.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.fktsv.cn/Article/details/gtfnezwld.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.fktsv.cn/Article/details/gpvtatueo.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.vehdjk.com/Article/details/gedudljoh.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.tarul.cn/Article/details/goebbopts.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.bbcook.cn/Article/details/gfaeuletv.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.vehdjk.com/Article/details/gbtzlteyc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.bbcook.cn/Article/details/gqlcumbnr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.bbcook.cn/Article/details/gflvgsjju.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.sjlbkw.cn/Article/details/gcoogcswb.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.bbcook.cn/Article/details/gihvgpvgr.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.bbcook.cn/Article/details/gkoqlnavl.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.yfazqb.com/Article/details/gmsaxtdjq.sHtML


<!-- 参考信息 -->