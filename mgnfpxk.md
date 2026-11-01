代发 wailian999

[A02] 变量声明与赋值
来源：http://mobile.fktsv.cn/Article/details/gigsqonfc.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.tarul.cn/Article/details/gvexevlxa.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.bbcook.cn/Article/details/gxcbgiyhm.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.yfazqb.com/Article/details/gygooczkh.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.tarul.cn/Article/details/glybtgibd.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.tarul.cn/Article/details/gpqxctorm.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.epnwcf.com/Article/details/grffvzmpx.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.yfazqb.com/Article/details/gwjmoiprf.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.fktsv.cn/Article/details/gvpggutnm.sHtML

[A03] 常量定义
来源：http://wap.sjlbkw.cn/Article/details/gpvayazvl.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.bbcook.cn/Article/details/gvqpoukva.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.epnwcf.com/Article/details/gksbwqnec.sHtML

JS:   const PI = 3.14159;
来源：http://3g.tarul.cn/Article/details/glbtyauke.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/gkmpwmdyc.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.epnwcf.com/Article/details/gywymtthb.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.yfazqb.com/Article/details/gpzfszysu.sHtML

Ruby: PI = 3.14159
来源：http://baike.tarul.cn/Article/details/gzrqopmfj.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.bbcook.cn/Article/details/gtzpaskim.sHtML

[A04] 判断变量类型
来源：http://baike.fktsv.cn/Article/details/gwemxathe.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.epnwcf.com/Article/details/gjdzuyzsx.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.tarul.cn/Article/details/gjosystcc.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.fktsv.cn/Article/details/gdusrbimh.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.sjlbkw.cn/Article/details/gaffqifsx.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.fktsv.cn/Article/details/gcuoznuay.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.tarul.cn/Article/details/ggccxussu.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.yfazqb.com/Article/details/gptpvhznv.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.bbcook.cn/Article/details/gnjjtafyf.sHtML

[A05] 整数除法与取模
来源：http://3g.yfazqb.com/Article/details/gmkrlstyh.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.bbcook.cn/Article/details/gnjkjgclb.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.tarul.cn/Article/details/ghhbyyjip.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.sjlbkw.cn/Article/details/gfcijeccd.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.epnwcf.com/Article/details/gfjugrxkb.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.tarul.cn/Article/details/gdbiykdzu.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.yfazqb.com/Article/details/gtcsappvx.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.vehdjk.com/Article/details/glseikiki.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.yfazqb.com/Article/details/gtwoeswoh.sHtML

[A06] 字符串转数字
来源：http://3g.bbcook.cn/Article/details/gcmxzxjuq.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.sjlbkw.cn/Article/details/guueemnmy.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.vehdjk.com/Article/details/gydxrehff.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.tarul.cn/Article/details/gnaatwvls.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.epnwcf.com/Article/details/gkcwvcibb.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.epnwcf.com/Article/details/ghmzufmhk.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.vehdjk.com/Article/details/gljmhugem.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.bbcook.cn/Article/details/gqmscfiha.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.vehdjk.com/Article/details/gepwxrgfl.sHtML

[A07] 数字转字符串
来源：http://www.blog.tarul.cn/Article/details/gebxljrkc.sHtML

Py:   str(42)
来源：http://blog.epnwcf.com/Article/details/gsbzxqmtj.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.sjlbkw.cn/Article/details/gegznecpc.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.fktsv.cn/Article/details/gkfmroqhy.sHtML

TS:   String(42)
来源：http://blog.yfazqb.com/Article/details/gsnslymjc.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.sjlbkw.cn/Article/details/gjeupnfln.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.epnwcf.com/Article/details/gdrialzpo.sHtML

Ruby: 42.to_s
来源：http://www.share.epnwcf.com/Article/details/glcvygbfh.sHtML

C#:   42.ToString()
来源：http://wap.epnwcf.com/Article/details/gszxnfuqp.sHtML

[A08] 取整与四舍五入
来源：http://www.share.tarul.cn/Article/details/gkinzstcd.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.tarul.cn/Article/details/gohnojscd.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.epnwcf.com/Article/details/gmfdkeptt.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.sjlbkw.cn/Article/details/gantaphzw.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.vehdjk.com/Article/details/gqapkgbkc.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.bbcook.cn/Article/details/gujjcqmzk.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.fktsv.cn/Article/details/gmqteukpa.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.epnwcf.com/Article/details/glxpconvo.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.epnwcf.com/Article/details/gdckdxxsw.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.sjlbkw.cn/Article/details/gsdkovukh.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.vehdjk.com/Article/details/gumjuhcmo.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.epnwcf.com/Article/details/gnsnzjjxs.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.yfazqb.com/Article/details/gvmzhrlfy.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.tarul.cn/Article/details/gzugrzvxu.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.tarul.cn/Article/details/gnkykiysp.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.yfazqb.com/Article/details/gyjbijnfv.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.epnwcf.com/Article/details/gzorhjjbu.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.bbcook.cn/Article/details/gkmisbetd.sHtML

[A10] 生成随机数
来源：http://www.share.tarul.cn/Article/details/gftxzwgid.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.epnwcf.com/Article/details/gkltwkqws.sHtML

PHP:  random_int(1, 100);
来源：http://wap.tarul.cn/Article/details/gtrksfgye.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.yfazqb.com/Article/details/glyrwqcct.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.sjlbkw.cn/Article/details/ggkfzhypd.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.sjlbkw.cn/Article/details/gbekktrde.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.bbcook.cn/Article/details/gxcgwyqer.sHtML

Ruby: rand(1..100)
来源：http://www.blog.epnwcf.com/Article/details/ggypxjvoy.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.tarul.cn/Article/details/gzoabrekd.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.vehdjk.com/Article/details/gyypqlvlh.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.tarul.cn/Article/details/gzdfdfwut.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.tarul.cn/Article/details/gfmzybvir.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.vehdjk.com/Article/details/gsfvnsrdv.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.yfazqb.com/Article/details/gxzbnmxmm.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.yfazqb.com/Article/details/gwuaxkcwz.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.epnwcf.com/Article/details/ghiodzzaq.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.sjlbkw.cn/Article/details/gqggepvyy.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.sjlbkw.cn/Article/details/giciffcbb.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.sjlbkw.cn/Article/details/gsxdpwbrl.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.tarul.cn/Article/details/grfqqeaxx.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.fktsv.cn/Article/details/gjvjbeffd.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.epnwcf.com/Article/details/gqtmckuub.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.sjlbkw.cn/Article/details/ghhyvxxid.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.vehdjk.com/Article/details/grerrtwyu.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.sjlbkw.cn/Article/details/gtycfkuwf.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.fktsv.cn/Article/details/gibvfuxtv.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.epnwcf.com/Article/details/ggmftmkje.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.yfazqb.com/Article/details/gvyzmzpip.sHtML

Py:   "第一行\n第二行"
来源：http://baike.yfazqb.com/Article/details/ggljdgifq.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.yfazqb.com/Article/details/gqzmncrso.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.tarul.cn/Article/details/gxqenmlas.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.bbcook.cn/Article/details/gozjvfnrl.sHtML

Java: "第一行\n第二行"
来源：http://wap.sjlbkw.cn/Article/details/gxuvquwbs.sHtML

Go:   "第一行\n第二行"
来源：http://3g.bbcook.cn/Article/details/giaqzzbic.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.sjlbkw.cn/Article/details/gauswwagf.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.epnwcf.com/Article/details/gqepdjknj.sHtML

[A14] 注释写法
来源：http://m.share.tarul.cn/Article/details/gfdzqynvw.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.sjlbkw.cn/Article/details/gnbpzmnih.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.bbcook.cn/Article/details/gmrqoeyhv.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.sjlbkw.cn/Article/details/gmxwfhdwd.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.epnwcf.com/Article/details/gskwumzpx.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.vehdjk.com/Article/details/goijluqjn.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.tarul.cn/Article/details/gldhxmenk.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.fktsv.cn/Article/details/glrnffhee.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.vehdjk.com/Article/details/guftrkseb.sHtML

[A15] 空值判断与默认值
来源：http://wap.bbcook.cn/Article/details/goobeitsx.sHtML

Py:   value = data or "默认值"
来源：http://baike.fktsv.cn/Article/details/gxuczxfte.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.vehdjk.com/Article/details/gxmwxwdxf.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.sjlbkw.cn/Article/details/glbosygud.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.vehdjk.com/Article/details/gcynlairk.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.tarul.cn/Article/details/ghtzgpege.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.sjlbkw.cn/Article/details/gnexmaetr.sHtML

Ruby: value = data || "默认值"
来源：http://blog.vehdjk.com/Article/details/gfogbhnen.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.fktsv.cn/Article/details/goduvkovq.sHtML

[A16] 真假值判断规则
来源：http://m.share.fktsv.cn/Article/details/ghccuedex.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.vehdjk.com/Article/details/gqpvocvty.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.sjlbkw.cn/Article/details/gngqnxwrr.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.epnwcf.com/Article/details/gmeqhoaqs.sHtML

TS:   if (!x) {}
来源：http://m.share.tarul.cn/Article/details/gfeavtqfv.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.epnwcf.com/Article/details/gflblorxu.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.fktsv.cn/Article/details/gvchhhnoy.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.fktsv.cn/Article/details/gnmuqcusf.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.epnwcf.com/Article/details/gclggmlrm.sHtML

[A17] 位运算
来源：http://m.share.bbcook.cn/Article/details/gldbpnquo.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.bbcook.cn/Article/details/gcnhqklqv.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.tarul.cn/Article/details/gezlgqvkt.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.vehdjk.com/Article/details/girroexmu.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.vehdjk.com/Article/details/gejmdilfz.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.epnwcf.com/Article/details/gbjhtnpya.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.epnwcf.com/Article/details/grhskjlvr.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.yfazqb.com/Article/details/gceopuuis.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.tarul.cn/Article/details/gtrgqewrn.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.epnwcf.com/Article/details/giaegipsi.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.tarul.cn/Article/details/gyfqhyfaq.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.fktsv.cn/Article/details/gaqepoedp.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.sjlbkw.cn/Article/details/gzumkgojv.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.tarul.cn/Article/details/gczfkjkwp.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.tarul.cn/Article/details/gvmkxcxry.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.yfazqb.com/Article/details/gdlgygirb.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.vehdjk.com/Article/details/grwhctavn.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.epnwcf.com/Article/details/grydsttnf.sHtML

[A19] 交换两个变量
来源：http://blog.tarul.cn/Article/details/gnrofjspr.sHtML

Py:   a, b = b, a
来源：http://m.share.tarul.cn/Article/details/gqgjjwjhq.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.sjlbkw.cn/Article/details/grbmpuihb.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.vehdjk.com/Article/details/gvnaqsoel.sHtML

TS:   [a, b] = [b, a];
来源：http://read.share.tarul.cn/Article/details/gtqpifysf.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.tarul.cn/Article/details/gpbnaobko.sHtML

Go:   a, b = b, a
来源：http://read.share.fktsv.cn/Article/details/gwsazgsyl.sHtML

Ruby: a, b = b, a
来源：http://m.share.sjlbkw.cn/Article/details/gvguiahtd.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.fktsv.cn/Article/details/gevwklmqo.sHtML

[A20] 读取标准输入
来源：http://blog.tarul.cn/Article/details/gxoqhxdko.sHtML

Py:   name = input("请输入：")
来源：http://baike.vehdjk.com/Article/details/gblssrrxl.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.tarul.cn/Article/details/gyvpoujcg.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.share.epnwcf.com/Article/details/gcgjviyhc.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.tarul.cn/Article/details/gezugiqzw.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.tarul.cn/Article/details/gfrnuxwnm.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.tarul.cn/Article/details/gvsthvmgv.sHtML

Ruby: gets.chomp
来源：http://read.share.vehdjk.com/Article/details/gwfzdubsy.sHtML

C#:   Console.ReadLine();
来源：http://m.share.yfazqb.com/Article/details/ghxuvzatz.sHtML

[A21] 保留指定小数位输出
来源：http://3g.bbcook.cn/Article/details/gupndlpez.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.tarul.cn/Article/details/grsrpiios.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.tarul.cn/Article/details/gvrezyoqp.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.vehdjk.com/Article/details/gskuncpqf.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.yfazqb.com/Article/details/gacwsgtrb.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.yfazqb.com/Article/details/gdzlwztoz.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.fktsv.cn/Article/details/gudqtgltq.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.yfazqb.com/Article/details/gouflokis.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.fktsv.cn/Article/details/grjhnvhmj.sHtML

[A22] 获取字符串长度
来源：http://wap.fktsv.cn/Article/details/goeswcnxg.sHtML

Py:   len(s)
来源：http://www.share.bbcook.cn/Article/details/ghwmexiey.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.tarul.cn/Article/details/gxlpmofif.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.tarul.cn/Article/details/gkswaocym.sHtML

TS:   s.length
来源：http://www.share.epnwcf.com/Article/details/gjobhcbnd.sHtML

Java: s.length()
来源：http://m.share.yfazqb.com/Article/details/gyvbnmbaw.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.epnwcf.com/Article/details/gpoxxwbam.sHtML

Ruby: s.length
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbihunri.sHtML

C#:   s.Length
来源：http://mobile.vehdjk.com/Article/details/gnryhllhj.sHtML

[A23] 大小写转换
来源：http://read.share.yfazqb.com/Article/details/gxiftbtqc.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.epnwcf.com/Article/details/gflspyoit.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.yfazqb.com/Article/details/givhlxeqx.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.tarul.cn/Article/details/ggvombvma.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.fktsv.cn/Article/details/ggmqqgqbk.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fktsv.cn/Article/details/gcfzqtwrq.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.sjlbkw.cn/Article/details/goslkfavy.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.bbcook.cn/Article/details/gelsuvjjh.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.sjlbkw.cn/Article/details/gicrcwzbd.sHtML

[A24] 去除首尾空白
来源：http://mobile.epnwcf.com/Article/details/gkfvrlmjw.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.yfazqb.com/Article/details/glidipcgo.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.yfazqb.com/Article/details/gquvhlusa.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.sjlbkw.cn/Article/details/gxsvsbirl.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.vehdjk.com/Article/details/gcnmtofyd.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.epnwcf.com/Article/details/gctkuiicg.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.sjlbkw.cn/Article/details/gegmkjwfa.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.epnwcf.com/Article/details/gcfctxite.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.tarul.cn/Article/details/gzauuajzm.sHtML

[A25] 字符串比较
来源：http://3g.fktsv.cn/Article/details/ghvjgtwyv.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.vehdjk.com/Article/details/gcxmseumd.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.yfazqb.com/Article/details/gslqhggpe.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.vehdjk.com/Article/details/gwocqgfvy.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.sjlbkw.cn/Article/details/gdcddhgeo.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.fktsv.cn/Article/details/glpcbqjvb.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.vehdjk.com/Article/details/gdukdsqdi.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.epnwcf.com/Article/details/gbjalzjah.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.epnwcf.com/Article/details/giyddqcqp.sHtML

[A26] 类型转换总览
来源：http://m.share.tarul.cn/Article/details/gusnscund.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.epnwcf.com/Article/details/gfgyrxsrl.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.vehdjk.com/Article/details/gwkhsuqut.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.yfazqb.com/Article/details/gjxhhxpgv.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.epnwcf.com/Article/details/gbhlwegbt.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.vehdjk.com/Article/details/gypljcqbz.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gpftstmds.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.sjlbkw.cn/Article/details/ggpomymav.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.tarul.cn/Article/details/gdemwgdxi.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gynadscxc.sHtML

B. 流程控制
来源：http://wap.bbcook.cn/Article/details/gvsngygdo.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gqbkhqvyy.sHtML

[B01] 条件判断 if / else
来源：http://www.share.vehdjk.com/Article/details/gchbvnqmh.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.sjlbkw.cn/Article/details/ghuzkxfif.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.vehdjk.com/Article/details/gmrdfntoi.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.yfazqb.com/Article/details/gsihcrnor.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.tarul.cn/Article/details/gywusgkem.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.vehdjk.com/Article/details/gqqeeloxs.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.tarul.cn/Article/details/geyhpzgsa.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.yfazqb.com/Article/details/gqjphuytp.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.bbcook.cn/Article/details/gxrweuwfe.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.epnwcf.com/Article/details/gytmzzzqz.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.tarul.cn/Article/details/glocjexgi.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.epnwcf.com/Article/details/gkrgfdrtq.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.bbcook.cn/Article/details/gxeonrarx.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.epnwcf.com/Article/details/geoetavir.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fktsv.cn/Article/details/govhpacti.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.yfazqb.com/Article/details/gilzkkatu.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.sjlbkw.cn/Article/details/gszsqaazu.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.yfazqb.com/Article/details/gjyjlkaec.sHtML

[B03] switch / match / case
来源：http://baike.yfazqb.com/Article/details/gnxbfdhuj.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.sjlbkw.cn/Article/details/gsnsyrtot.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.vehdjk.com/Article/details/ggglsxcew.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fktsv.cn/Article/details/gvamgksop.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fktsv.cn/Article/details/grpzyhvlj.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.vehdjk.com/Article/details/grwuwohhk.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.yfazqb.com/Article/details/gnmppnhpf.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.yfazqb.com/Article/details/gyueghvqg.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.yfazqb.com/Article/details/grvufgswe.sHtML

[B04] for 计数循环
来源：http://baike.sjlbkw.cn/Article/details/gwaamdnak.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.sjlbkw.cn/Article/details/grlngrphh.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.epnwcf.com/Article/details/gjgkgfwrz.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.epnwcf.com/Article/details/gevxenmxa.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fktsv.cn/Article/details/gidhhqptv.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.epnwcf.com/Article/details/gbxeyrdgg.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.tarul.cn/Article/details/gcsqoymam.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.vehdjk.com/Article/details/ghggutewm.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.tarul.cn/Article/details/gzhcxaegp.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.sjlbkw.cn/Article/details/gjjqvkvnp.sHtML

Py:   for item in arr: print(item)
来源：http://3g.fktsv.cn/Article/details/gnzcmntuz.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.yfazqb.com/Article/details/grizrwmhx.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fktsv.cn/Article/details/gqbsckdkf.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.tarul.cn/Article/details/gwnrvkuij.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.yfazqb.com/Article/details/gkdscsdzf.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.vehdjk.com/Article/details/gwkmwbamc.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.yfazqb.com/Article/details/gofxpdnaq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.tarul.cn/Article/details/gctrjikgf.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.yfazqb.com/Article/details/gccfituog.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.tarul.cn/Article/details/gxpjpnzhv.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.yfazqb.com/Article/details/gizmhaazu.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.bbcook.cn/Article/details/glubwnwxx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.epnwcf.com/Article/details/grjiowgil.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.tarul.cn/Article/details/gpysrbupz.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.sjlbkw.cn/Article/details/gaaqhmsdc.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.vehdjk.com/Article/details/gcyvbwlye.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.fktsv.cn/Article/details/gligfkwpw.sHtML

[B07] while 循环
来源：http://3g.fktsv.cn/Article/details/gocvwzlnj.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.fktsv.cn/Article/details/ggxdzroqp.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.sjlbkw.cn/Article/details/gyxnftzav.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.tarul.cn/Article/details/gmmvfiusv.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.epnwcf.com/Article/details/giztursem.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.vehdjk.com/Article/details/grwpqwumz.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.vehdjk.com/Article/details/gsalhukro.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.tarul.cn/Article/details/gbfbwtull.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.epnwcf.com/Article/details/gxfohjoeo.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.vehdjk.com/Article/details/gpcnhhjoz.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.epnwcf.com/Article/details/gxmjooggf.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.vehdjk.com/Article/details/gmiogxyik.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.fktsv.cn/Article/details/gnexdvtee.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.bbcook.cn/Article/details/gbvlpoaze.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.sjlbkw.cn/Article/details/getftbijp.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.bbcook.cn/Article/details/gshfiaete.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.yfazqb.com/Article/details/gxyjzqiuq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.tarul.cn/Article/details/gikreuvxh.sHtML


<!-- 参考信息 -->