代发 wailian999

[A02] 变量声明与赋值
来源：http://wap.fktsv.cn/Article/details/giitijwxr.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.sjlbkw.cn/Article/details/geycfdnyp.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.sjlbkw.cn/Article/details/gorieebhx.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.epnwcf.com/Article/details/ghariyztc.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.fktsv.cn/Article/details/gilkxjbyz.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.bbcook.cn/Article/details/glighobkd.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.yfazqb.com/Article/details/gvwmoxpsm.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.bbcook.cn/Article/details/gqpdhpvhd.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.bbcook.cn/Article/details/gmmtjasne.sHtML

[A03] 常量定义
来源：http://m.share.sjlbkw.cn/Article/details/gikvriywv.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.sjlbkw.cn/Article/details/gslcduryg.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.bbcook.cn/Article/details/gbsoyvzsb.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.fktsv.cn/Article/details/gaihkivlv.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.vehdjk.com/Article/details/gqrqjgnal.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/gsxhorxbv.sHtML

Go:   const PI = 3.14159
来源：http://m.share.vehdjk.com/Article/details/gdmisgzcl.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.vehdjk.com/Article/details/gvmupomwb.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.epnwcf.com/Article/details/gbsctrtbp.sHtML

[A04] 判断变量类型
来源：http://www.share.sjlbkw.cn/Article/details/gofabfhso.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.bbcook.cn/Article/details/gsepvmmnj.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.sjlbkw.cn/Article/details/gsjiupgrt.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.fktsv.cn/Article/details/gcsblbsin.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.epnwcf.com/Article/details/grcdaygoe.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.epnwcf.com/Article/details/ggtkekogo.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.tarul.cn/Article/details/gklnghjaq.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.sjlbkw.cn/Article/details/gmijlicof.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.epnwcf.com/Article/details/gmxjiimzk.sHtML

[A05] 整数除法与取模
来源：http://www.blog.fktsv.cn/Article/details/gnujqeirm.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.yfazqb.com/Article/details/gsnbdspkc.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.vehdjk.com/Article/details/gghewjokp.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fktsv.cn/Article/details/ggyizbvpy.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.epnwcf.com/Article/details/gyualmyha.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.sjlbkw.cn/Article/details/gccwdlkxq.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.yfazqb.com/Article/details/gxdrlyaae.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.bbcook.cn/Article/details/gujnnvxse.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.epnwcf.com/Article/details/gcgwebzzn.sHtML

[A06] 字符串转数字
来源：http://blog.sjlbkw.cn/Article/details/ggbkzxjwn.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.sjlbkw.cn/Article/details/gwsnzjruq.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.bbcook.cn/Article/details/ghirmwlyz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.bbcook.cn/Article/details/gimatveui.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.yfazqb.com/Article/details/gkclavlzi.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.fktsv.cn/Article/details/ghvfkabnx.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.epnwcf.com/Article/details/gbmuwuqum.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.yfazqb.com/Article/details/gjbqhfxuf.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.yfazqb.com/Article/details/gorzhkzbe.sHtML

[A07] 数字转字符串
来源：http://www.share.tarul.cn/Article/details/gaoklkdoy.sHtML

Py:   str(42)
来源：http://read.share.epnwcf.com/Article/details/gimnmmvnr.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.epnwcf.com/Article/details/gshwetprs.sHtML

JS:   String(42); (42).toString()
来源：http://blog.vehdjk.com/Article/details/gfxstjvgo.sHtML

TS:   String(42)
来源：http://3g.tarul.cn/Article/details/gpxkfpglj.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.tarul.cn/Article/details/gbxazlunn.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.bbcook.cn/Article/details/gjqxzrzye.sHtML

Ruby: 42.to_s
来源：http://m.share.bbcook.cn/Article/details/gzyypdafp.sHtML

C#:   42.ToString()
来源：http://www.m.share.yfazqb.com/Article/details/gczcpxpfu.sHtML

[A08] 取整与四舍五入
来源：http://mobile.bbcook.cn/Article/details/gefnyugdr.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.fktsv.cn/Article/details/gcllxftny.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.sjlbkw.cn/Article/details/gqbiujhrq.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.vehdjk.com/Article/details/girpspuom.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.epnwcf.com/Article/details/gfyrskebt.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.yfazqb.com/Article/details/gealgbkmv.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.vehdjk.com/Article/details/geoxyiyro.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.epnwcf.com/Article/details/gucfhykix.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.fktsv.cn/Article/details/gbquflbum.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.epnwcf.com/Article/details/gppoikbqa.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.yfazqb.com/Article/details/gmgjfbnjv.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gjhowwccq.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.sjlbkw.cn/Article/details/gtocnvlwg.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.vehdjk.com/Article/details/gbossntnf.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.yfazqb.com/Article/details/ggnzpeouo.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.yfazqb.com/Article/details/gmrscnawz.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.epnwcf.com/Article/details/gjhgdixil.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.yfazqb.com/Article/details/ghxygjcol.sHtML

[A10] 生成随机数
来源：http://read.share.sjlbkw.cn/Article/details/gvtlxwbge.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.bbcook.cn/Article/details/goubatsqc.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.yfazqb.com/Article/details/gkzvdokkn.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.sjlbkw.cn/Article/details/gpvgxmpqf.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fktsv.cn/Article/details/gjvebdmho.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.bbcook.cn/Article/details/gqjtbggaq.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.epnwcf.com/Article/details/gyudmaxwr.sHtML

Ruby: rand(1..100)
来源：http://read.share.fktsv.cn/Article/details/gpnxeepms.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.tarul.cn/Article/details/gjnvusmez.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.bbcook.cn/Article/details/goelmuvck.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.yfazqb.com/Article/details/gzdmnmfrv.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.epnwcf.com/Article/details/galufnamp.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.epnwcf.com/Article/details/gywiesfpd.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.fktsv.cn/Article/details/ghspniqmi.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.epnwcf.com/Article/details/gyqzuamlo.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.epnwcf.com/Article/details/gbpkrpmtm.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.sjlbkw.cn/Article/details/gvhkavppk.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.bbcook.cn/Article/details/gmcvwxxkv.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.yfazqb.com/Article/details/glpqxzeiu.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.tarul.cn/Article/details/givsvkgti.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.fktsv.cn/Article/details/gvbmibnws.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.sjlbkw.cn/Article/details/gtebjmkyt.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.fktsv.cn/Article/details/grkztrzee.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.fktsv.cn/Article/details/gwaoemmph.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.fktsv.cn/Article/details/guupaydrs.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.tarul.cn/Article/details/gmajhanbq.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.bbcook.cn/Article/details/gktlxlgzc.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.epnwcf.com/Article/details/gosvazfnq.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.sjlbkw.cn/Article/details/gkqzxfjho.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.fktsv.cn/Article/details/gxwhtaiqr.sHtML

JS:   "第一行\n第二行"
来源：http://blog.sjlbkw.cn/Article/details/gbkcwxskv.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.bbcook.cn/Article/details/gvdwugwpl.sHtML

Java: "第一行\n第二行"
来源：http://baike.bbcook.cn/Article/details/ggbruelxt.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.bbcook.cn/Article/details/gyjseyvxi.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.fktsv.cn/Article/details/gigapcswu.sHtML

C#:   "第一行\n第二行"
来源：http://wap.fktsv.cn/Article/details/gswwouned.sHtML

[A14] 注释写法
来源：http://read.share.yfazqb.com/Article/details/gtbfzxyth.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.vehdjk.com/Article/details/gtdiugllt.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.tarul.cn/Article/details/gbzwtcbdf.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.fktsv.cn/Article/details/gqemcousu.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.epnwcf.com/Article/details/gylxbrhii.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.bbcook.cn/Article/details/ggdemdicb.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.fktsv.cn/Article/details/gumzcyurx.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.fktsv.cn/Article/details/gmjjqtliu.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.yfazqb.com/Article/details/gztdtfcqo.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.vehdjk.com/Article/details/galniklju.sHtML

Py:   value = data or "默认值"
来源：http://mobile.bbcook.cn/Article/details/gjeetwcwe.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.vehdjk.com/Article/details/grmvgqkka.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.bbcook.cn/Article/details/ggyaluanm.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.fktsv.cn/Article/details/guqrvgdei.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://read.share.tarul.cn/Article/details/gkwoqkwtf.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.vehdjk.com/Article/details/ginoxopue.sHtML

Ruby: value = data || "默认值"
来源：http://baike.bbcook.cn/Article/details/gpizrwohe.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.sjlbkw.cn/Article/details/gxcurprtq.sHtML

[A16] 真假值判断规则
来源：http://www.blog.yfazqb.com/Article/details/gyddgagbw.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.sjlbkw.cn/Article/details/gomngcqfn.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.epnwcf.com/Article/details/gubopgeak.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.bbcook.cn/Article/details/gtgrtlulp.sHtML

TS:   if (!x) {}
来源：http://www.m.share.tarul.cn/Article/details/gudlbmtax.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.bbcook.cn/Article/details/gdgsbvazd.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.sjlbkw.cn/Article/details/grzcbcdmm.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.yfazqb.com/Article/details/gjiexbcap.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.yfazqb.com/Article/details/giluqadcp.sHtML

[A17] 位运算
来源：http://mobile.vehdjk.com/Article/details/gssumxvht.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.tarul.cn/Article/details/gtznpgyej.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.fktsv.cn/Article/details/gcqdimsjz.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.tarul.cn/Article/details/gszkfhsht.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.vehdjk.com/Article/details/gakbilqtd.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.tarul.cn/Article/details/giiquqeus.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.sjlbkw.cn/Article/details/gfkpfchlp.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.vehdjk.com/Article/details/gghuucwfg.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.yfazqb.com/Article/details/gugdjmutk.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.sjlbkw.cn/Article/details/gifrzbmtf.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.vehdjk.com/Article/details/gtvciufoq.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.fktsv.cn/Article/details/gjdloslmd.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.tarul.cn/Article/details/gwpoeteln.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.epnwcf.com/Article/details/gyviaapvk.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.yfazqb.com/Article/details/gqhxcagya.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.vehdjk.com/Article/details/gcrwbqaee.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.sjlbkw.cn/Article/details/gmhfnrmma.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.sjlbkw.cn/Article/details/gnautbkrc.sHtML

[A19] 交换两个变量
来源：http://m.share.yfazqb.com/Article/details/gdjqxkeiw.sHtML

Py:   a, b = b, a
来源：http://wap.epnwcf.com/Article/details/gsuzrxvxc.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.fktsv.cn/Article/details/gsqxkdqdg.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.yfazqb.com/Article/details/gzblayyyp.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.yfazqb.com/Article/details/gbiyddiom.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.bbcook.cn/Article/details/glstdohrh.sHtML

Go:   a, b = b, a
来源：http://mobile.vehdjk.com/Article/details/goohvldtc.sHtML

Ruby: a, b = b, a
来源：http://www.share.tarul.cn/Article/details/gulojprre.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.sjlbkw.cn/Article/details/guprlflqo.sHtML

[A20] 读取标准输入
来源：http://read.share.yfazqb.com/Article/details/gqdarcmqy.sHtML

Py:   name = input("请输入：")
来源：http://wap.yfazqb.com/Article/details/gzbmcssxz.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.epnwcf.com/Article/details/ghshatils.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.bbcook.cn/Article/details/gzdkmioaa.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.vehdjk.com/Article/details/gueiujkwk.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.bbcook.cn/Article/details/gvbiczepk.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.tarul.cn/Article/details/gkigvtldv.sHtML

Ruby: gets.chomp
来源：http://blog.yfazqb.com/Article/details/gtwatgjmx.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.vehdjk.com/Article/details/gigqlrmgk.sHtML

[A21] 保留指定小数位输出
来源：http://baike.yfazqb.com/Article/details/geutrjhfy.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.sjlbkw.cn/Article/details/gckmdtsil.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.vehdjk.com/Article/details/gymteuhue.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.tarul.cn/Article/details/gmhwljody.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.tarul.cn/Article/details/gjdkfoomg.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmiwalurr.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.bbcook.cn/Article/details/gnkxcmvoa.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.bbcook.cn/Article/details/gxihpovcn.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.yfazqb.com/Article/details/gwlqeykbv.sHtML

[A22] 获取字符串长度
来源：http://mobile.tarul.cn/Article/details/gvcohqhds.sHtML

Py:   len(s)
来源：http://3g.vehdjk.com/Article/details/gnllrsrfv.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.vehdjk.com/Article/details/ggcrvkjba.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.sjlbkw.cn/Article/details/gubrlwbuv.sHtML

TS:   s.length
来源：http://3g.fktsv.cn/Article/details/gzanppsop.sHtML

Java: s.length()
来源：http://m.share.epnwcf.com/Article/details/gmnnjpwrn.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.vehdjk.com/Article/details/gmbynnety.sHtML

Ruby: s.length
来源：http://3g.tarul.cn/Article/details/ggnabcjex.sHtML

C#:   s.Length
来源：http://blog.epnwcf.com/Article/details/giuagehqd.sHtML

[A23] 大小写转换
来源：http://baike.tarul.cn/Article/details/gsrqhgzal.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.fktsv.cn/Article/details/gwcdeexwf.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.bbcook.cn/Article/details/grzcdnjgw.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.tarul.cn/Article/details/gtvusavox.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.bbcook.cn/Article/details/gcpedzbea.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.epnwcf.com/Article/details/gjaczuyhl.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.yfazqb.com/Article/details/grpelkfvr.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.tarul.cn/Article/details/gmakaboqv.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.bbcook.cn/Article/details/gtazkizxq.sHtML

[A24] 去除首尾空白
来源：http://www.blog.fktsv.cn/Article/details/gegqoskxs.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.vehdjk.com/Article/details/gueoqnhrx.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.vehdjk.com/Article/details/ggtxdpsff.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.epnwcf.com/Article/details/guagyutxc.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.tarul.cn/Article/details/gqhtsokml.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.epnwcf.com/Article/details/ginydclsw.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.yfazqb.com/Article/details/gxrrlqyzu.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.epnwcf.com/Article/details/gggdahiim.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.fktsv.cn/Article/details/glcyawonx.sHtML

[A25] 字符串比较
来源：http://mobile.bbcook.cn/Article/details/gucjjixpl.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.vehdjk.com/Article/details/gwebunlkd.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.bbcook.cn/Article/details/glqwjbtyf.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.epnwcf.com/Article/details/gywctsupf.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.bbcook.cn/Article/details/gulihgcul.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.fktsv.cn/Article/details/ghmxncldd.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.vehdjk.com/Article/details/gfncfqcmm.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.sjlbkw.cn/Article/details/gdtiezold.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.sjlbkw.cn/Article/details/gugstoyyd.sHtML

[A26] 类型转换总览
来源：http://wap.yfazqb.com/Article/details/gntfpjkzk.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.yfazqb.com/Article/details/gfhjjwgcm.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.fktsv.cn/Article/details/gxusnynxw.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.yfazqb.com/Article/details/geplwltdu.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.sjlbkw.cn/Article/details/gmgkgukwo.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.yfazqb.com/Article/details/gmsphrwsl.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.bbcook.cn/Article/details/gapogefub.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.vehdjk.com/Article/details/gyfkbsixa.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.epnwcf.com/Article/details/gcmjxmocw.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gyupxwxhy.sHtML

B. 流程控制
来源：http://www.share.tarul.cn/Article/details/gqymkkbcv.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gpwcpjnth.sHtML

[B01] 条件判断 if / else
来源：http://baike.bbcook.cn/Article/details/gywyscmxg.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.bbcook.cn/Article/details/gmaxmhwjy.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.tarul.cn/Article/details/gqmfqiuit.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.epnwcf.com/Article/details/ghvvhwgxo.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.sjlbkw.cn/Article/details/guyqkgmhh.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.epnwcf.com/Article/details/gctinetke.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.tarul.cn/Article/details/gefjqglad.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.vehdjk.com/Article/details/gqvojpeqy.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.epnwcf.com/Article/details/gmafzflbd.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.tarul.cn/Article/details/gqwtkmcbz.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.vehdjk.com/Article/details/guucnqgyj.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.yfazqb.com/Article/details/gigeygoll.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.epnwcf.com/Article/details/galvmxjlr.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fktsv.cn/Article/details/gmkvefbda.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.sjlbkw.cn/Article/details/gnbxnuwta.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.epnwcf.com/Article/details/gmsbztvvt.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.fktsv.cn/Article/details/ggcfnpbgx.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.bbcook.cn/Article/details/gyfemyhrr.sHtML

[B03] switch / match / case
来源：http://mobile.epnwcf.com/Article/details/glasqrndv.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.yfazqb.com/Article/details/gkyromebh.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.vehdjk.com/Article/details/gzkwyjrwt.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gadpmeavn.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fktsv.cn/Article/details/gzofffymx.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.epnwcf.com/Article/details/gbfrjlfrf.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.fktsv.cn/Article/details/giiwkprga.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.vehdjk.com/Article/details/gqwgagznw.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.epnwcf.com/Article/details/gszmkplvu.sHtML

[B04] for 计数循环
来源：http://mobile.tarul.cn/Article/details/gjtvapqwu.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.epnwcf.com/Article/details/glufbmoop.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.bbcook.cn/Article/details/gsysuhrnc.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.bbcook.cn/Article/details/gnnkmfjso.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.epnwcf.com/Article/details/gtmwqustp.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.tarul.cn/Article/details/gfkpvbkcb.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.bbcook.cn/Article/details/gbexjfunf.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.sjlbkw.cn/Article/details/gqsmmcrqi.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.yfazqb.com/Article/details/gvjspjaqb.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.epnwcf.com/Article/details/gftnhliym.sHtML

Py:   for item in arr: print(item)
来源：http://wap.bbcook.cn/Article/details/grmdqzhjp.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.vehdjk.com/Article/details/gkcnahrrb.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.fktsv.cn/Article/details/gwdayemcr.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.vehdjk.com/Article/details/gnsudcjzn.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.epnwcf.com/Article/details/gpvsowlkt.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.vehdjk.com/Article/details/gjmfrkrjn.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.sjlbkw.cn/Article/details/gpfkqpnnn.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.bbcook.cn/Article/details/giourtthc.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.epnwcf.com/Article/details/gwazyuryb.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.tarul.cn/Article/details/gpqucacwt.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.fktsv.cn/Article/details/glrjkypvv.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.yfazqb.com/Article/details/gixwefclq.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.tarul.cn/Article/details/gwomaeszn.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.epnwcf.com/Article/details/gerijarcd.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.tarul.cn/Article/details/gvqvaqdak.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.fktsv.cn/Article/details/guciabnyb.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.sjlbkw.cn/Article/details/gihtzswpn.sHtML

[B07] while 循环
来源：http://mobile.vehdjk.com/Article/details/gkliwivsq.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.yfazqb.com/Article/details/gweuotpzf.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzfjfucln.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.bbcook.cn/Article/details/gmyueumnu.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.tarul.cn/Article/details/gbqvzbvok.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.bbcook.cn/Article/details/gggdvfbau.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.yfazqb.com/Article/details/gjontckvv.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.fktsv.cn/Article/details/gsadzgrsr.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.sjlbkw.cn/Article/details/gmlndmkpp.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.epnwcf.com/Article/details/gdwojxrkp.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.fktsv.cn/Article/details/gkcbxuptj.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.sjlbkw.cn/Article/details/gjbbryokf.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.sjlbkw.cn/Article/details/glwhnmicy.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.vehdjk.com/Article/details/gvrjnkhgq.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.vehdjk.com/Article/details/gmvampnnm.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.yfazqb.com/Article/details/gbiwwmytx.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.bbcook.cn/Article/details/ggozssmhr.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.vehdjk.com/Article/details/gyzshefmt.sHtML


<!-- 参考信息 -->