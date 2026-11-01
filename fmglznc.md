代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.tarul.cn/Article/details/gymceugkh.sHtML

[A03] 常量定义
来源：http://read.share.yfazqb.com/Article/details/gdvhquisv.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.sjlbkw.cn/Article/details/gozknxteo.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.tarul.cn/Article/details/gwsmofxzy.sHtML

JS:   const PI = 3.14159;
来源：http://wap.epnwcf.com/Article/details/gmqqpflvf.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.epnwcf.com/Article/details/gppkidery.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.epnwcf.com/Article/details/giizuiech.sHtML

Go:   const PI = 3.14159
来源：http://3g.tarul.cn/Article/details/gsfwgmanv.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.sjlbkw.cn/Article/details/glpgisxrg.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.yfazqb.com/Article/details/gaaxbmsag.sHtML

[A04] 判断变量类型
来源：http://3g.epnwcf.com/Article/details/gemmeptoy.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.epnwcf.com/Article/details/gszktdypv.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.vehdjk.com/Article/details/gxviwoumr.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.fktsv.cn/Article/details/glhexjoko.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.vehdjk.com/Article/details/gidzjamis.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.epnwcf.com/Article/details/grrxqxxze.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.yfazqb.com/Article/details/gjxkgmynd.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.fktsv.cn/Article/details/guysgegfn.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fktsv.cn/Article/details/gdmiqikau.sHtML

[A05] 整数除法与取模
来源：http://blog.tarul.cn/Article/details/gaorwswxf.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.fktsv.cn/Article/details/gnzmjovky.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.yfazqb.com/Article/details/gevalbfbp.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.yfazqb.com/Article/details/gymiadegh.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.epnwcf.com/Article/details/gcfdktnkf.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.bbcook.cn/Article/details/ggjmhirax.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.sjlbkw.cn/Article/details/gfuijudaz.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.fktsv.cn/Article/details/gztwfhpho.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.tarul.cn/Article/details/gsqevaemw.sHtML

[A06] 字符串转数字
来源：http://mobile.bbcook.cn/Article/details/gefwbnwlj.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.epnwcf.com/Article/details/gmeilakla.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.fktsv.cn/Article/details/gmcvzgyit.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.yfazqb.com/Article/details/gheowmwck.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.yfazqb.com/Article/details/glqukqpde.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.epnwcf.com/Article/details/gsrxutrna.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.fktsv.cn/Article/details/gybqgidkk.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.epnwcf.com/Article/details/gkdchhabe.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.tarul.cn/Article/details/gxqyhxhin.sHtML

[A07] 数字转字符串
来源：http://wap.tarul.cn/Article/details/gztylkgfe.sHtML

Py:   str(42)
来源：http://read.share.epnwcf.com/Article/details/gfrjvggmq.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.epnwcf.com/Article/details/guuudfxoy.sHtML

JS:   String(42); (42).toString()
来源：http://blog.sjlbkw.cn/Article/details/gpyydzhuv.sHtML

TS:   String(42)
来源：http://m.share.tarul.cn/Article/details/gqsutgdpl.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.yfazqb.com/Article/details/grgtzaqmh.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.vehdjk.com/Article/details/gfigbfxui.sHtML

Ruby: 42.to_s
来源：http://m.share.vehdjk.com/Article/details/gcpweygvz.sHtML

C#:   42.ToString()
来源：http://m.share.fktsv.cn/Article/details/gxhnnuenu.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.bbcook.cn/Article/details/gmesqrkcj.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.bbcook.cn/Article/details/gozlfttuc.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.vehdjk.com/Article/details/grlpmkuck.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.fktsv.cn/Article/details/gemrlnzab.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.sjlbkw.cn/Article/details/gvnpsbzmw.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.epnwcf.com/Article/details/gmrrevzge.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.bbcook.cn/Article/details/gmprjohaj.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.vehdjk.com/Article/details/gavfxxseb.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.yfazqb.com/Article/details/guujihtnw.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.vehdjk.com/Article/details/gahqefpeb.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkvzzkmae.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.yfazqb.com/Article/details/gtpgonbrx.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gwcvxsqgx.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.yfazqb.com/Article/details/geixwqomf.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.yfazqb.com/Article/details/gbzfcredc.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.bbcook.cn/Article/details/gpviasrnh.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.epnwcf.com/Article/details/ggthiuvah.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.fktsv.cn/Article/details/gelccppam.sHtML

[A10] 生成随机数
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjzffpyl.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.tarul.cn/Article/details/gdcuodmwk.sHtML

PHP:  random_int(1, 100);
来源：http://baike.sjlbkw.cn/Article/details/glxcnlrcn.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.tarul.cn/Article/details/gxtquwoip.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.epnwcf.com/Article/details/ghmorzwlw.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.yfazqb.com/Article/details/gqhevesjr.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.vehdjk.com/Article/details/gtxuamalt.sHtML

Ruby: rand(1..100)
来源：http://www.share.sjlbkw.cn/Article/details/gqnhrguhq.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.sjlbkw.cn/Article/details/gdmzolszg.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.yfazqb.com/Article/details/gimiddant.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.epnwcf.com/Article/details/ggerjhkao.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.epnwcf.com/Article/details/gxhtanrft.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.epnwcf.com/Article/details/gbrvjxvxi.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.bbcook.cn/Article/details/gdaubltjy.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.epnwcf.com/Article/details/gfchnzrcn.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.fktsv.cn/Article/details/gaqjfgkan.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.vehdjk.com/Article/details/geprxordr.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.epnwcf.com/Article/details/gzyxdlwmn.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.bbcook.cn/Article/details/gucyaljdd.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.sjlbkw.cn/Article/details/gdgdlxpsn.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.fktsv.cn/Article/details/glhilzlrf.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.bbcook.cn/Article/details/gpzaawtkm.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.fktsv.cn/Article/details/guykiosgx.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.tarul.cn/Article/details/gvminoumu.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.epnwcf.com/Article/details/gwzkomaie.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.yfazqb.com/Article/details/gtjrwrkks.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.epnwcf.com/Article/details/gjcjraxcv.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.sjlbkw.cn/Article/details/gpthntkru.sHtML

Py:   "第一行\n第二行"
来源：http://wap.yfazqb.com/Article/details/gnhnneeio.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.vehdjk.com/Article/details/goafdxzds.sHtML

JS:   "第一行\n第二行"
来源：http://3g.epnwcf.com/Article/details/gzyipidqb.sHtML

TS:   "第一行\n第二行"
来源：http://baike.bbcook.cn/Article/details/gzkfjcizg.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.tarul.cn/Article/details/gdbkanijj.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.bbcook.cn/Article/details/gsajofsez.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.bbcook.cn/Article/details/gvgupwfug.sHtML

C#:   "第一行\n第二行"
来源：http://wap.fktsv.cn/Article/details/gfvrvpfjp.sHtML

[A14] 注释写法
来源：http://read.share.epnwcf.com/Article/details/gvhyrbpaj.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.yfazqb.com/Article/details/grkmbfnbq.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.epnwcf.com/Article/details/gvhiivacc.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.yfazqb.com/Article/details/gfhqrllon.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.fktsv.cn/Article/details/gfyrjzbvv.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.tarul.cn/Article/details/gvrgvqkbb.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.vehdjk.com/Article/details/gzhhivynn.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.fktsv.cn/Article/details/gkvftmzrk.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.sjlbkw.cn/Article/details/gunhipzhc.sHtML

[A15] 空值判断与默认值
来源：http://3g.tarul.cn/Article/details/gxuzkumlv.sHtML

Py:   value = data or "默认值"
来源：http://blog.bbcook.cn/Article/details/gwaegfibb.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.bbcook.cn/Article/details/gdvrmmbdy.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.vehdjk.com/Article/details/gtjwgohaq.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.vehdjk.com/Article/details/guqsxgbsa.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.fktsv.cn/Article/details/gjfljyppm.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.vehdjk.com/Article/details/gcdgoklrb.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.yfazqb.com/Article/details/gnkhysvja.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.sjlbkw.cn/Article/details/grenqguaf.sHtML

[A16] 真假值判断规则
来源：http://mobile.yfazqb.com/Article/details/gwawdolow.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.epnwcf.com/Article/details/giaurzcsb.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.fktsv.cn/Article/details/gvaqrthrh.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.yfazqb.com/Article/details/gldkzjwuv.sHtML

TS:   if (!x) {}
来源：http://baike.yfazqb.com/Article/details/gdxvxlhgt.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.yfazqb.com/Article/details/gtsczknwm.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.yfazqb.com/Article/details/gidvaocpy.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.yfazqb.com/Article/details/gnqcdwpks.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.bbcook.cn/Article/details/gpsukxnzq.sHtML

[A17] 位运算
来源：http://blog.sjlbkw.cn/Article/details/gnjsucxwu.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fktsv.cn/Article/details/gohqwiggq.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.yfazqb.com/Article/details/gexwhtvxe.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.epnwcf.com/Article/details/gewvbunwb.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.bbcook.cn/Article/details/glzogkqqv.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.vehdjk.com/Article/details/gmflsofkf.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.tarul.cn/Article/details/gzvkoqist.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.bbcook.cn/Article/details/gfnhazzaj.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.vehdjk.com/Article/details/gppzzzggf.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.yfazqb.com/Article/details/gppbmuyey.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.fktsv.cn/Article/details/ghhhllpjz.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.tarul.cn/Article/details/glcjezwmq.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.bbcook.cn/Article/details/gbdgrvrdm.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.vehdjk.com/Article/details/gchswvpix.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.tarul.cn/Article/details/gtezagkoz.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.tarul.cn/Article/details/gsvtiqrsr.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.yfazqb.com/Article/details/grzvukxit.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.sjlbkw.cn/Article/details/glofqsnnj.sHtML

[A19] 交换两个变量
来源：http://www.m.share.vehdjk.com/Article/details/gykuqwbil.sHtML

Py:   a, b = b, a
来源：http://www.blog.fktsv.cn/Article/details/gajemmuwm.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.sjlbkw.cn/Article/details/guyvmbvha.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.sjlbkw.cn/Article/details/gblrthuxj.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.tarul.cn/Article/details/gcebpsboo.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.fktsv.cn/Article/details/gxvjdgbxb.sHtML

Go:   a, b = b, a
来源：http://m.share.sjlbkw.cn/Article/details/gewblqmyu.sHtML

Ruby: a, b = b, a
来源：http://blog.tarul.cn/Article/details/gvmwcvgmh.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.tarul.cn/Article/details/gsigtrsbe.sHtML

[A20] 读取标准输入
来源：http://read.share.sjlbkw.cn/Article/details/gifzuftwq.sHtML

Py:   name = input("请输入：")
来源：http://baike.bbcook.cn/Article/details/gjukqomlg.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.epnwcf.com/Article/details/ggeypowcz.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.vehdjk.com/Article/details/goziubkxi.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.bbcook.cn/Article/details/gggtellds.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.sjlbkw.cn/Article/details/gjqvcawdi.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.sjlbkw.cn/Article/details/gquinkrgw.sHtML

Ruby: gets.chomp
来源：http://read.share.yfazqb.com/Article/details/gdvddmgvm.sHtML

C#:   Console.ReadLine();
来源：http://mobile.epnwcf.com/Article/details/goeogykcq.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.sjlbkw.cn/Article/details/gnoyqzwoc.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.fktsv.cn/Article/details/gygbatqjj.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.fktsv.cn/Article/details/gimgjxbvu.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.vehdjk.com/Article/details/gfprhjxtf.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.vehdjk.com/Article/details/gmiczhmcs.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.bbcook.cn/Article/details/gtgtwttyp.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.tarul.cn/Article/details/gpbgzamep.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.sjlbkw.cn/Article/details/gnptuvuoj.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.vehdjk.com/Article/details/gqcghiibh.sHtML

[A22] 获取字符串长度
来源：http://www.share.yfazqb.com/Article/details/gjgyieljb.sHtML

Py:   len(s)
来源：http://mobile.fktsv.cn/Article/details/gqheleryg.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.tarul.cn/Article/details/gvtywavrq.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.bbcook.cn/Article/details/gyruwudif.sHtML

TS:   s.length
来源：http://www.m.share.bbcook.cn/Article/details/gleykoowt.sHtML

Java: s.length()
来源：http://www.share.epnwcf.com/Article/details/gkfdhsokk.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.bbcook.cn/Article/details/gwlyodfaw.sHtML

Ruby: s.length
来源：http://www.share.fktsv.cn/Article/details/gdkntsdwj.sHtML

C#:   s.Length
来源：http://wap.vehdjk.com/Article/details/grgipsvuu.sHtML

[A23] 大小写转换
来源：http://read.share.bbcook.cn/Article/details/gpqxopkar.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.yfazqb.com/Article/details/gsfjvcaoc.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.bbcook.cn/Article/details/ghhvejtur.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.epnwcf.com/Article/details/grxjjxyqc.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.yfazqb.com/Article/details/gwvecqigo.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.vehdjk.com/Article/details/gkccouzre.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.fktsv.cn/Article/details/ggnthsjna.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.fktsv.cn/Article/details/gveybxpbs.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.epnwcf.com/Article/details/gtksxxbxf.sHtML

[A24] 去除首尾空白
来源：http://www.blog.tarul.cn/Article/details/gdlodzend.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.sjlbkw.cn/Article/details/grduvtqys.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.tarul.cn/Article/details/gkscszjss.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.sjlbkw.cn/Article/details/gclhgbrbg.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.fktsv.cn/Article/details/gpuszhcnd.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.sjlbkw.cn/Article/details/ggrmppamk.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.sjlbkw.cn/Article/details/gysjhotah.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.sjlbkw.cn/Article/details/grhgssjbi.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.fktsv.cn/Article/details/ggpsvlagr.sHtML

[A25] 字符串比较
来源：http://3g.yfazqb.com/Article/details/gbyczepno.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.sjlbkw.cn/Article/details/gzzlsetmz.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.fktsv.cn/Article/details/gvjamfysa.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.vehdjk.com/Article/details/gndsmucmk.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.tarul.cn/Article/details/gsfkenktf.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.fktsv.cn/Article/details/grmcclaaw.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.vehdjk.com/Article/details/gjpixipol.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.fktsv.cn/Article/details/gdlrfqdzx.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.fktsv.cn/Article/details/gdjqwsbqk.sHtML

[A26] 类型转换总览
来源：http://blog.fktsv.cn/Article/details/gofsgodqq.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.fktsv.cn/Article/details/ghmkywxbo.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.fktsv.cn/Article/details/gczwuwfbi.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.tarul.cn/Article/details/gpkaagyum.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.epnwcf.com/Article/details/gwnzjrtvd.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.yfazqb.com/Article/details/gelurrtxo.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.bbcook.cn/Article/details/gmvnmxjba.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.epnwcf.com/Article/details/gwcjsrchp.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.bbcook.cn/Article/details/gzpbmyzch.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gmtqbpynd.sHtML

B. 流程控制
来源：http://blog.epnwcf.com/Article/details/ghvvwtjuw.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gqhlxfxvw.sHtML

[B01] 条件判断 if / else
来源：http://www.share.fktsv.cn/Article/details/gqiiqfkgo.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.tarul.cn/Article/details/gimbsudqg.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.bbcook.cn/Article/details/gflywhyia.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.vehdjk.com/Article/details/gejlizwlf.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.vehdjk.com/Article/details/gxegrkbhp.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.epnwcf.com/Article/details/gzwqapere.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.epnwcf.com/Article/details/gxnlcckxx.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.yfazqb.com/Article/details/gtlspvgev.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.vehdjk.com/Article/details/gwufqndyi.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.yfazqb.com/Article/details/gdvvmmrzq.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.yfazqb.com/Article/details/glwmfxwuv.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.yfazqb.com/Article/details/ghapzdhjf.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.vehdjk.com/Article/details/gvkpwcftx.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.vehdjk.com/Article/details/gadyccdrg.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fktsv.cn/Article/details/gbyvtzfkz.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.epnwcf.com/Article/details/gafejbqpc.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.epnwcf.com/Article/details/gqdgdbvdp.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.epnwcf.com/Article/details/gkwunwvwt.sHtML

[B03] switch / match / case
来源：http://mobile.sjlbkw.cn/Article/details/gqvilupyp.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.fktsv.cn/Article/details/gzppifxfc.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.bbcook.cn/Article/details/gydftqezu.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.vehdjk.com/Article/details/gsskpimvj.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.yfazqb.com/Article/details/gfhqxkxtn.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.bbcook.cn/Article/details/ghturfdbb.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.yfazqb.com/Article/details/gmqfrggih.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.epnwcf.com/Article/details/gqcvuqgbe.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.fktsv.cn/Article/details/gvpxtxyho.sHtML

[B04] for 计数循环
来源：http://mobile.fktsv.cn/Article/details/gahjdsymd.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.yfazqb.com/Article/details/gtpnqepkm.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.epnwcf.com/Article/details/gysnilyku.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.epnwcf.com/Article/details/gwxuxtzfg.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.sjlbkw.cn/Article/details/gvkwjvqyp.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.bbcook.cn/Article/details/gnagzztqu.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqsurqtiq.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.vehdjk.com/Article/details/gcggnuozf.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.sjlbkw.cn/Article/details/gzukjjgey.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.tarul.cn/Article/details/gewmvebct.sHtML

Py:   for item in arr: print(item)
来源：http://wap.yfazqb.com/Article/details/gdoeyegmu.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.sjlbkw.cn/Article/details/gtwfbtpdr.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.sjlbkw.cn/Article/details/gmhmhckee.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.tarul.cn/Article/details/gdqxvqqji.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.fktsv.cn/Article/details/gnzjpsuor.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.fktsv.cn/Article/details/gfapbrucn.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.yfazqb.com/Article/details/gsvglipiu.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.bbcook.cn/Article/details/gjwggrqax.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.tarul.cn/Article/details/guvegtaha.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.bbcook.cn/Article/details/gyysrgpzd.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.yfazqb.com/Article/details/gwtqanxtk.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.yfazqb.com/Article/details/gbikdfaqo.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fktsv.cn/Article/details/geoltazwc.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.epnwcf.com/Article/details/guzcpkqbu.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.yfazqb.com/Article/details/gfqkabjav.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.bbcook.cn/Article/details/gzrvfffbd.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.fktsv.cn/Article/details/gzgcdpwji.sHtML

[B07] while 循环
来源：http://baike.sjlbkw.cn/Article/details/gtoyvziis.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.vehdjk.com/Article/details/gduzqhdxf.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.bbcook.cn/Article/details/ghdtmfcad.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.epnwcf.com/Article/details/gllxiodrg.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.tarul.cn/Article/details/gdxrwrrig.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.sjlbkw.cn/Article/details/gqwnkssbo.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.tarul.cn/Article/details/gthoylcat.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.yfazqb.com/Article/details/gdpuunpbl.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.vehdjk.com/Article/details/gpezghdjr.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.vehdjk.com/Article/details/goskaeroi.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.sjlbkw.cn/Article/details/ggeskvkjp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.fktsv.cn/Article/details/gutxpxdqf.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.tarul.cn/Article/details/getlkxyah.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.bbcook.cn/Article/details/gmfhgzmji.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.sjlbkw.cn/Article/details/gkqqkbyrv.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.vehdjk.com/Article/details/gfggcdrko.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.sjlbkw.cn/Article/details/gugfzkngb.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.vehdjk.com/Article/details/gniatojdp.sHtML

[B09] break 与 continue
来源：http://baike.vehdjk.com/Article/details/gyjhqpjeg.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.yfazqb.com/Article/details/gipflvldi.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.epnwcf.com/Article/details/glgbdsdsq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.yfazqb.com/Article/details/gukvomppr.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.tarul.cn/Article/details/giyacxqkn.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.vehdjk.com/Article/details/gmddsdvht.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.epnwcf.com/Article/details/gtoznbhem.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.sjlbkw.cn/Article/details/gwhwojrjp.sHtML


<!-- 参考信息 -->