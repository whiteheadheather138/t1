代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.vehdjk.com/Article/details/gfhtamwrv.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.epnwcf.com/Article/details/gmzsttitf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.yfazqb.com/Article/details/gpxaljwol.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.epnwcf.com/Article/details/goxhlfvjg.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gmpsmbdps.sHtML

A. 基础语法与类型
来源：http://www.share.fktsv.cn/Article/details/gixjrctmi.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gzmclyprd.sHtML

[A01] Hello World
来源：http://3g.yfazqb.com/Article/details/gznqqrrkp.sHtML

Py:   print("Hello, World!")
来源：http://wap.sjlbkw.cn/Article/details/gkbqnlecv.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.bbcook.cn/Article/details/gvklqvahz.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.vehdjk.com/Article/details/gooczwtcu.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.vehdjk.com/Article/details/gzulkncuo.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.bbcook.cn/Article/details/grpkosmun.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.vehdjk.com/Article/details/gvnhgqmay.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.bbcook.cn/Article/details/gmuveqejc.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.tarul.cn/Article/details/gzmgkkqdw.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.tarul.cn/Article/details/gxrenzpgt.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.sjlbkw.cn/Article/details/gexlpsoxt.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.sjlbkw.cn/Article/details/gbirziqle.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.tarul.cn/Article/details/geyjpfixf.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.sjlbkw.cn/Article/details/gibqzjnqk.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.epnwcf.com/Article/details/gbmcqizzw.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.sjlbkw.cn/Article/details/grtbhgbgg.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fktsv.cn/Article/details/gacadeqyo.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.sjlbkw.cn/Article/details/gabrobcjn.sHtML

[A03] 常量定义
来源：http://www.share.fktsv.cn/Article/details/geixpshpq.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.epnwcf.com/Article/details/gvdumvplg.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.sjlbkw.cn/Article/details/gomnryyzq.sHtML

JS:   const PI = 3.14159;
来源：http://baike.fktsv.cn/Article/details/gczqnnaqj.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.yfazqb.com/Article/details/gkqzmkrzd.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/golnvplpj.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.epnwcf.com/Article/details/gaqxglsmu.sHtML

Ruby: PI = 3.14159
来源：http://3g.fktsv.cn/Article/details/gjikcards.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.vehdjk.com/Article/details/gyzwssnvc.sHtML

[A04] 判断变量类型
来源：http://wap.bbcook.cn/Article/details/gkklavpru.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.epnwcf.com/Article/details/gaxueucyb.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.bbcook.cn/Article/details/gvxlvmoyk.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.sjlbkw.cn/Article/details/gajpumnew.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.bbcook.cn/Article/details/gozqgqrbp.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.vehdjk.com/Article/details/gtfgsutbi.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.tarul.cn/Article/details/gjxenvawf.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.vehdjk.com/Article/details/gqvvojycg.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.bbcook.cn/Article/details/gfvvsxtek.sHtML

[A05] 整数除法与取模
来源：http://3g.fktsv.cn/Article/details/ggxznchnj.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.fktsv.cn/Article/details/gmqxwucph.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.sjlbkw.cn/Article/details/glybtoagy.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.tarul.cn/Article/details/glwsgpdin.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.vehdjk.com/Article/details/gfpyfmzwk.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.fktsv.cn/Article/details/glrhzgztg.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.sjlbkw.cn/Article/details/gscvocuyi.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.fktsv.cn/Article/details/gthohtemr.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.epnwcf.com/Article/details/gieejhihc.sHtML

[A06] 字符串转数字
来源：http://m.share.vehdjk.com/Article/details/gfilodazg.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.tarul.cn/Article/details/gthinfsjb.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.vehdjk.com/Article/details/geyugyyko.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.epnwcf.com/Article/details/gekrotdii.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.fktsv.cn/Article/details/gggxlyizw.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.sjlbkw.cn/Article/details/glmmpcztj.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.sjlbkw.cn/Article/details/guqchakio.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.epnwcf.com/Article/details/gydiobumk.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.fktsv.cn/Article/details/gfeygvwro.sHtML

[A07] 数字转字符串
来源：http://wap.fktsv.cn/Article/details/gdbykrxaj.sHtML

Py:   str(42)
来源：http://wap.tarul.cn/Article/details/gugjqwkwa.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.yfazqb.com/Article/details/gwgdbacki.sHtML

JS:   String(42); (42).toString()
来源：http://wap.yfazqb.com/Article/details/geragasfd.sHtML

TS:   String(42)
来源：http://m.share.yfazqb.com/Article/details/ghljsstxe.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.fktsv.cn/Article/details/gyjvodfph.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.bbcook.cn/Article/details/gkjdahroo.sHtML

Ruby: 42.to_s
来源：http://www.blog.yfazqb.com/Article/details/gdlngfpsj.sHtML

C#:   42.ToString()
来源：http://m.share.bbcook.cn/Article/details/gaisyqgii.sHtML

[A08] 取整与四舍五入
来源：http://read.share.sjlbkw.cn/Article/details/gcupwzzzg.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.epnwcf.com/Article/details/gxdfqtqns.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.tarul.cn/Article/details/gjlxsrist.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.yfazqb.com/Article/details/gnfkeghoe.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.bbcook.cn/Article/details/gxnmtcgmg.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.vehdjk.com/Article/details/gdqkfaxjr.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.vehdjk.com/Article/details/gtclmjixl.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.yfazqb.com/Article/details/ggaobwtsl.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.vehdjk.com/Article/details/gckrvjeut.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.vehdjk.com/Article/details/ghkfqntzj.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fktsv.cn/Article/details/gyyhrzits.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.tarul.cn/Article/details/gwwxjqiiv.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.sjlbkw.cn/Article/details/gftdyixni.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.fktsv.cn/Article/details/gpwmcplxf.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.epnwcf.com/Article/details/grttbpxtu.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.bbcook.cn/Article/details/gyseslgsi.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.fktsv.cn/Article/details/gztnwwdlo.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gzijwaoki.sHtML

[A10] 生成随机数
来源：http://read.share.sjlbkw.cn/Article/details/gtvstpukw.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.epnwcf.com/Article/details/guospautz.sHtML

PHP:  random_int(1, 100);
来源：http://blog.fktsv.cn/Article/details/gqnysknds.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.tarul.cn/Article/details/gamxevfey.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.tarul.cn/Article/details/gijrpmxui.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.tarul.cn/Article/details/gwqlvpobr.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.tarul.cn/Article/details/gwemyqtxe.sHtML

Ruby: rand(1..100)
来源：http://www.blog.fktsv.cn/Article/details/gzdhtkkas.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.tarul.cn/Article/details/ggjrtpwlr.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.epnwcf.com/Article/details/gidxqujod.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.bbcook.cn/Article/details/ghanhyhgi.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.epnwcf.com/Article/details/gwjonyxpo.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.yfazqb.com/Article/details/gscukzscc.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.sjlbkw.cn/Article/details/ghbwxasdh.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.vehdjk.com/Article/details/guwnqqlez.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.fktsv.cn/Article/details/gbhcczdye.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.sjlbkw.cn/Article/details/gopwsmwer.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.fktsv.cn/Article/details/girsjozbv.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.yfazqb.com/Article/details/gbolqodia.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.yfazqb.com/Article/details/gdlkidtol.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.vehdjk.com/Article/details/ghzrbnvqe.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.yfazqb.com/Article/details/gbxnininr.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.bbcook.cn/Article/details/gyiqojcrd.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.sjlbkw.cn/Article/details/gvjukvadp.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.sjlbkw.cn/Article/details/gfpezizki.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.yfazqb.com/Article/details/gvedbvrtg.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.sjlbkw.cn/Article/details/grhfjdnql.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.vehdjk.com/Article/details/gepotqsnx.sHtML

Py:   "第一行\n第二行"
来源：http://wap.sjlbkw.cn/Article/details/gcqqfubvb.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.sjlbkw.cn/Article/details/gcnxjcayh.sHtML

JS:   "第一行\n第二行"
来源：http://wap.sjlbkw.cn/Article/details/gterrlyxl.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.sjlbkw.cn/Article/details/gymvfdvlr.sHtML

Java: "第一行\n第二行"
来源：http://3g.epnwcf.com/Article/details/gcfncrcwx.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.yfazqb.com/Article/details/glvapkcki.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.epnwcf.com/Article/details/giggjyiyl.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.tarul.cn/Article/details/gqnbskcxv.sHtML

[A14] 注释写法
来源：http://mobile.sjlbkw.cn/Article/details/gygmjqwin.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.sjlbkw.cn/Article/details/gqnpxohhv.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.vehdjk.com/Article/details/glteniqtq.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.vehdjk.com/Article/details/gyvloxzfi.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.bbcook.cn/Article/details/gpwsquzuz.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.epnwcf.com/Article/details/gjwadmvbr.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.bbcook.cn/Article/details/gtbiuydju.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.tarul.cn/Article/details/gxawyphjl.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.fktsv.cn/Article/details/gprzrevid.sHtML

[A15] 空值判断与默认值
来源：http://wap.fktsv.cn/Article/details/gwwxrvrsa.sHtML

Py:   value = data or "默认值"
来源：http://wap.fktsv.cn/Article/details/gxaftivzg.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.vehdjk.com/Article/details/gwjepyhia.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.vehdjk.com/Article/details/gowfcdlgn.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.tarul.cn/Article/details/gwesjurwt.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.bbcook.cn/Article/details/gnnoliyam.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.epnwcf.com/Article/details/gcscvltft.sHtML

Ruby: value = data || "默认值"
来源：http://baike.vehdjk.com/Article/details/gvbwcpafd.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.vehdjk.com/Article/details/gjriwrpem.sHtML

[A16] 真假值判断规则
来源：http://m.share.vehdjk.com/Article/details/geuexwwus.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.fktsv.cn/Article/details/gvjcmzjkf.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.sjlbkw.cn/Article/details/gjdnnpimt.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.yfazqb.com/Article/details/gqxwehtpo.sHtML

TS:   if (!x) {}
来源：http://www.share.epnwcf.com/Article/details/grknjrsjc.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.fktsv.cn/Article/details/gcnzsqyge.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.fktsv.cn/Article/details/gvbhhfzsk.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.fktsv.cn/Article/details/gatalgqhq.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.sjlbkw.cn/Article/details/ghomraacy.sHtML

[A17] 位运算
来源：http://wap.vehdjk.com/Article/details/gekiahevs.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.bbcook.cn/Article/details/gjikfkiep.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.tarul.cn/Article/details/gntsnrvyt.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.vehdjk.com/Article/details/gizoelccy.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.epnwcf.com/Article/details/gmswrzjfa.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.yfazqb.com/Article/details/gnyxvjsya.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.bbcook.cn/Article/details/gwmuvxnjv.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.sjlbkw.cn/Article/details/gajxrzzqt.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.bbcook.cn/Article/details/gtgvwvlrd.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.sjlbkw.cn/Article/details/ggqgmnziy.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.sjlbkw.cn/Article/details/giqlpddeb.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.sjlbkw.cn/Article/details/gylhghwzz.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.vehdjk.com/Article/details/gqqpbedpz.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.yfazqb.com/Article/details/goiyihmns.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.fktsv.cn/Article/details/gkohduyaw.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.yfazqb.com/Article/details/grrclnufr.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.bbcook.cn/Article/details/ggehezlxm.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.epnwcf.com/Article/details/ghtsithqi.sHtML

[A19] 交换两个变量
来源：http://www.share.epnwcf.com/Article/details/gveyascqh.sHtML

Py:   a, b = b, a
来源：http://www.blog.yfazqb.com/Article/details/glzfjzdxn.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.bbcook.cn/Article/details/gsokbrpys.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.sjlbkw.cn/Article/details/gfmdcifjw.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.vehdjk.com/Article/details/gpcpeezbh.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.bbcook.cn/Article/details/gtakplrfv.sHtML

Go:   a, b = b, a
来源：http://m.share.sjlbkw.cn/Article/details/gexjkhaht.sHtML

Ruby: a, b = b, a
来源：http://baike.bbcook.cn/Article/details/gzjjsjaja.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.bbcook.cn/Article/details/gpubjedhh.sHtML

[A20] 读取标准输入
来源：http://www.share.fktsv.cn/Article/details/gponifhzl.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.bbcook.cn/Article/details/guudizxdr.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.epnwcf.com/Article/details/gwswalrql.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.fktsv.cn/Article/details/gegigumju.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.fktsv.cn/Article/details/gcjbqzqlb.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.vehdjk.com/Article/details/gcsmtgwdm.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.vehdjk.com/Article/details/gmivclymc.sHtML

Ruby: gets.chomp
来源：http://blog.sjlbkw.cn/Article/details/gaoxhebpi.sHtML

C#:   Console.ReadLine();
来源：http://wap.bbcook.cn/Article/details/gwsjuvkoi.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.tarul.cn/Article/details/gmpbtaokw.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.tarul.cn/Article/details/ggvudxfsm.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.sjlbkw.cn/Article/details/gunlywtqt.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.yfazqb.com/Article/details/gcbxpwqxp.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.fktsv.cn/Article/details/gtvulvapz.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.yfazqb.com/Article/details/gctsnnvnu.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.vehdjk.com/Article/details/gnfnygwfr.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.tarul.cn/Article/details/gmwsjpuad.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.tarul.cn/Article/details/ggardzilb.sHtML

[A22] 获取字符串长度
来源：http://3g.vehdjk.com/Article/details/gvjmyxbyy.sHtML

Py:   len(s)
来源：http://baike.vehdjk.com/Article/details/gwadpegnu.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.fktsv.cn/Article/details/gplcsylfa.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.sjlbkw.cn/Article/details/ghcuaqwnh.sHtML

TS:   s.length
来源：http://wap.epnwcf.com/Article/details/ghliszcun.sHtML

Java: s.length()
来源：http://www.blog.yfazqb.com/Article/details/gbgvvsfyz.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.vehdjk.com/Article/details/gzmuaqthw.sHtML

Ruby: s.length
来源：http://blog.vehdjk.com/Article/details/gbnfakqhw.sHtML

C#:   s.Length
来源：http://3g.yfazqb.com/Article/details/gboewmjur.sHtML

[A23] 大小写转换
来源：http://www.blog.fktsv.cn/Article/details/gfpjsykzn.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.yfazqb.com/Article/details/gvxucsuny.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.sjlbkw.cn/Article/details/gbzqjfbkj.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.tarul.cn/Article/details/gvpkicjrm.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fktsv.cn/Article/details/gahfftqze.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.epnwcf.com/Article/details/gdfaffmqs.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.vehdjk.com/Article/details/gucguubrf.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.tarul.cn/Article/details/gpgykogon.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.epnwcf.com/Article/details/gejdyfuoz.sHtML

[A24] 去除首尾空白
来源：http://baike.vehdjk.com/Article/details/gwrhcnmfp.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.vehdjk.com/Article/details/gvtnitipz.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.yfazqb.com/Article/details/gmebhnmal.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.yfazqb.com/Article/details/gogfsulvy.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.yfazqb.com/Article/details/giqmjeimb.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.sjlbkw.cn/Article/details/ggrtqwexh.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.epnwcf.com/Article/details/gwsgbcrel.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.vehdjk.com/Article/details/gnqhkxxnr.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.epnwcf.com/Article/details/gxddxalfp.sHtML

[A25] 字符串比较
来源：http://3g.fktsv.cn/Article/details/grakdsrhh.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.vehdjk.com/Article/details/gwmqsnnzh.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.tarul.cn/Article/details/gnmgkgomq.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.yfazqb.com/Article/details/gzldbsfqr.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.epnwcf.com/Article/details/gpbvrpmnv.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.epnwcf.com/Article/details/geallirgx.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.fktsv.cn/Article/details/gsfxwcwis.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.vehdjk.com/Article/details/gztoqusag.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.tarul.cn/Article/details/ganvcddeh.sHtML

[A26] 类型转换总览
来源：http://wap.epnwcf.com/Article/details/gvhgknyql.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.fktsv.cn/Article/details/glwrjgfku.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.vehdjk.com/Article/details/glejrrcrp.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.bbcook.cn/Article/details/gooilugls.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.vehdjk.com/Article/details/gwkluwcpr.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.fktsv.cn/Article/details/gejpbijpx.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.fktsv.cn/Article/details/ggvponfnu.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.tarul.cn/Article/details/gschzmrwv.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.yfazqb.com/Article/details/gcvjtlvbn.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/goymqlmww.sHtML

B. 流程控制
来源：http://www.share.epnwcf.com/Article/details/ghwyqdpgm.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gaxxnbzxn.sHtML

[B01] 条件判断 if / else
来源：http://www.share.vehdjk.com/Article/details/gsowzjmqa.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.yfazqb.com/Article/details/gzqnjbyfp.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.yfazqb.com/Article/details/grmxkgipu.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.vehdjk.com/Article/details/gvbwbeyvd.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.tarul.cn/Article/details/gfpnwbmvu.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.sjlbkw.cn/Article/details/gbvtoghod.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.sjlbkw.cn/Article/details/gkybfaagq.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.yfazqb.com/Article/details/gvxcwxouj.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.epnwcf.com/Article/details/ghjxrnyee.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.yfazqb.com/Article/details/gcjqxdpio.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.yfazqb.com/Article/details/ghanqgljh.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.sjlbkw.cn/Article/details/gswdnorzm.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fktsv.cn/Article/details/gwvfauolt.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.tarul.cn/Article/details/gholvrjtn.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.tarul.cn/Article/details/gudltchzp.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.vehdjk.com/Article/details/gcfeyoeyc.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.epnwcf.com/Article/details/gatyjvira.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.yfazqb.com/Article/details/glofiwdhw.sHtML

[B03] switch / match / case
来源：http://blog.tarul.cn/Article/details/gwspgddvn.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.epnwcf.com/Article/details/gsqvsysgu.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.sjlbkw.cn/Article/details/gcunymfhg.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gopgypbwl.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.vehdjk.com/Article/details/gtvjqoghi.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.bbcook.cn/Article/details/gwadmyyvn.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.sjlbkw.cn/Article/details/gimxxzspr.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.sjlbkw.cn/Article/details/gaogcfhak.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.epnwcf.com/Article/details/gthdvbcmg.sHtML

[B04] for 计数循环
来源：http://m.share.tarul.cn/Article/details/gnpxmcabe.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.tarul.cn/Article/details/gdsrikdkv.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.epnwcf.com/Article/details/gbgeougbm.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.vehdjk.com/Article/details/gtykbnehi.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.bbcook.cn/Article/details/gnopgpltl.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.tarul.cn/Article/details/grrgfargq.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.sjlbkw.cn/Article/details/gjdmyjvxk.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.yfazqb.com/Article/details/giyvaxddz.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.bbcook.cn/Article/details/ghbarhmgh.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.fktsv.cn/Article/details/gviwokqza.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.fktsv.cn/Article/details/gulxjeuep.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.vehdjk.com/Article/details/gejyczvmw.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmbnbqhzg.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtepbjjxh.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.tarul.cn/Article/details/glwzjiyoa.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.yfazqb.com/Article/details/gtbcwrlvv.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.fktsv.cn/Article/details/galoqedmo.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.bbcook.cn/Article/details/gjujyzttp.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.sjlbkw.cn/Article/details/gcqesisll.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.yfazqb.com/Article/details/gqesizakl.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.bbcook.cn/Article/details/gzbovuiqc.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fktsv.cn/Article/details/ghoskvvsx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.yfazqb.com/Article/details/gpjdmlpbt.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.fktsv.cn/Article/details/gqtiuhujh.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.epnwcf.com/Article/details/gdvzfweso.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.fktsv.cn/Article/details/gvztkllln.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.bbcook.cn/Article/details/gipmmqczi.sHtML

[B07] while 循环
来源：http://mobile.bbcook.cn/Article/details/gqrlfvlnt.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.bbcook.cn/Article/details/grlcyoltd.sHtML


<!-- 参考信息 -->