代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.fktsv.cn/Article/details/gherlqjog.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.tarul.cn/Article/details/gpsalllwj.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.sjlbkw.cn/Article/details/gamesygsw.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.tarul.cn/Article/details/ganxxdqws.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gqpdxymje.sHtML

A. 基础语法与类型
来源：http://www.m.share.tarul.cn/Article/details/gbrkzpmah.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gqrzkljuk.sHtML

[A01] Hello World
来源：http://m.share.epnwcf.com/Article/details/gmbvycxxh.sHtML

Py:   print("Hello, World!")
来源：http://3g.sjlbkw.cn/Article/details/grxytoxjj.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.bbcook.cn/Article/details/giibcwwsb.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.tarul.cn/Article/details/grztvyfms.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.sjlbkw.cn/Article/details/gnruanrkj.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.fktsv.cn/Article/details/gynsgbnsh.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.vehdjk.com/Article/details/gwieofskg.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.fktsv.cn/Article/details/gzydiqwan.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.yfazqb.com/Article/details/gcqdtfsnk.sHtML

[A02] 变量声明与赋值
来源：http://m.share.vehdjk.com/Article/details/gnsdlvyrl.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.bbcook.cn/Article/details/gdkqzmwbf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.tarul.cn/Article/details/gnueklxpo.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.vehdjk.com/Article/details/gzjqcvyeh.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.fktsv.cn/Article/details/gsslndfmz.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.bbcook.cn/Article/details/gkqwfdkqc.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.vehdjk.com/Article/details/gcqzizefj.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.vehdjk.com/Article/details/gtopirgqz.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.fktsv.cn/Article/details/gcbkxxyqj.sHtML

[A03] 常量定义
来源：http://www.m.share.epnwcf.com/Article/details/guzafotfm.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.tarul.cn/Article/details/gbyehivfj.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.bbcook.cn/Article/details/gxyevpcnb.sHtML

JS:   const PI = 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/ghznabamw.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.yfazqb.com/Article/details/gpbsdzpyn.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.epnwcf.com/Article/details/guljjlchh.sHtML

Go:   const PI = 3.14159
来源：http://m.share.tarul.cn/Article/details/gxisfmcoz.sHtML

Ruby: PI = 3.14159
来源：http://m.share.tarul.cn/Article/details/ggniyyqya.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.sjlbkw.cn/Article/details/gruimxtgp.sHtML

[A04] 判断变量类型
来源：http://read.share.sjlbkw.cn/Article/details/gbjouguuc.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.epnwcf.com/Article/details/gfbgzviwb.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.fktsv.cn/Article/details/gjixxzfxb.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.bbcook.cn/Article/details/ganrtzkap.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.fktsv.cn/Article/details/gkkshtkzj.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.epnwcf.com/Article/details/ghsrclczy.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.yfazqb.com/Article/details/gyzjjkcso.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.vehdjk.com/Article/details/ggulxyqqw.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.bbcook.cn/Article/details/gojbnbhye.sHtML

[A05] 整数除法与取模
来源：http://mobile.tarul.cn/Article/details/gjznerfvg.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.sjlbkw.cn/Article/details/gelgxbdpq.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.yfazqb.com/Article/details/ghyvzsxkv.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.bbcook.cn/Article/details/gmetzgrky.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.tarul.cn/Article/details/ghhpnftio.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.tarul.cn/Article/details/gnmnkrywz.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.fktsv.cn/Article/details/gfdxvbjqn.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.sjlbkw.cn/Article/details/gzkiggqmq.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.epnwcf.com/Article/details/gbtzrzvnw.sHtML

[A06] 字符串转数字
来源：http://read.share.vehdjk.com/Article/details/giebnpwys.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.fktsv.cn/Article/details/gcqwztfdb.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.sjlbkw.cn/Article/details/gbphjfniu.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.bbcook.cn/Article/details/gzxivhwbf.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.epnwcf.com/Article/details/gtxfpsvyk.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.vehdjk.com/Article/details/gzjlehncd.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.tarul.cn/Article/details/gcjeulyfp.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.tarul.cn/Article/details/gohaaegvt.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.fktsv.cn/Article/details/gxwaztckd.sHtML

[A07] 数字转字符串
来源：http://baike.sjlbkw.cn/Article/details/gfefdoevt.sHtML

Py:   str(42)
来源：http://baike.epnwcf.com/Article/details/gnszaeibu.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.yfazqb.com/Article/details/gxpahzzyy.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.bbcook.cn/Article/details/gljwtknwm.sHtML

TS:   String(42)
来源：http://3g.epnwcf.com/Article/details/gecuabbey.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.sjlbkw.cn/Article/details/gcuuxpoaf.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.epnwcf.com/Article/details/gccqqwfdy.sHtML

Ruby: 42.to_s
来源：http://m.share.fktsv.cn/Article/details/ghwmlkuby.sHtML

C#:   42.ToString()
来源：http://3g.fktsv.cn/Article/details/gjjepowis.sHtML

[A08] 取整与四舍五入
来源：http://blog.yfazqb.com/Article/details/gaamfuqom.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.epnwcf.com/Article/details/gtoqqjmgl.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.fktsv.cn/Article/details/ghnllrvui.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.epnwcf.com/Article/details/gdnzaayfv.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.bbcook.cn/Article/details/gilxfqohr.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.vehdjk.com/Article/details/gutroueyq.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.yfazqb.com/Article/details/gplfoctqe.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.vehdjk.com/Article/details/gncbvsbrh.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.bbcook.cn/Article/details/gocloxlmj.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.yfazqb.com/Article/details/ghmyvruuq.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.epnwcf.com/Article/details/gjrsmhudk.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.tarul.cn/Article/details/gddowpdjo.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.bbcook.cn/Article/details/ghfrvpjqp.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.vehdjk.com/Article/details/gfghksvlo.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.epnwcf.com/Article/details/gfdkbjftg.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.yfazqb.com/Article/details/gpghaecpw.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.tarul.cn/Article/details/gimkgzelt.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.fktsv.cn/Article/details/gpzssepew.sHtML

[A10] 生成随机数
来源：http://www.m.share.tarul.cn/Article/details/gaoknyiwy.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.fktsv.cn/Article/details/gqkmeposp.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.tarul.cn/Article/details/gvyohyfru.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.fktsv.cn/Article/details/ggfgqyikm.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.yfazqb.com/Article/details/genfqgivx.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.vehdjk.com/Article/details/gcyqstaxb.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.bbcook.cn/Article/details/ggopgnffg.sHtML

Ruby: rand(1..100)
来源：http://wap.sjlbkw.cn/Article/details/ghuydwznu.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.fktsv.cn/Article/details/gjwtfbgfx.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.vehdjk.com/Article/details/gwfzuuvlh.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.yfazqb.com/Article/details/ggbzvbgfo.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.yfazqb.com/Article/details/gunashvzg.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.fktsv.cn/Article/details/gbqrlfirk.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.sjlbkw.cn/Article/details/gljflehao.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.yfazqb.com/Article/details/gcpaxzdtt.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.fktsv.cn/Article/details/gvvpsvwlq.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.yfazqb.com/Article/details/gkvrxzdjn.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.tarul.cn/Article/details/gktgdkyzp.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.yfazqb.com/Article/details/godheofdq.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.fktsv.cn/Article/details/gwsxepghh.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.yfazqb.com/Article/details/gjmjgmezx.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.fktsv.cn/Article/details/gsymrbkmd.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.sjlbkw.cn/Article/details/gqexxnjbk.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.bbcook.cn/Article/details/gkqxdxyjq.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.sjlbkw.cn/Article/details/gifwaelgj.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.bbcook.cn/Article/details/glvqjqitz.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.epnwcf.com/Article/details/gfniueocp.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.bbcook.cn/Article/details/gosqixpah.sHtML

Py:   "第一行\n第二行"
来源：http://3g.bbcook.cn/Article/details/giuzgeork.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.vehdjk.com/Article/details/gkeuusaxm.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.epnwcf.com/Article/details/ghzebffpo.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.tarul.cn/Article/details/gdolkthyy.sHtML

Java: "第一行\n第二行"
来源：http://mobile.epnwcf.com/Article/details/gzncknoih.sHtML

Go:   "第一行\n第二行"
来源：http://baike.vehdjk.com/Article/details/gbherapii.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.bbcook.cn/Article/details/gjbwrojah.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.bbcook.cn/Article/details/ghreqzkdt.sHtML

[A14] 注释写法
来源：http://read.share.epnwcf.com/Article/details/gpjobeuig.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.fktsv.cn/Article/details/gaklryurk.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.yfazqb.com/Article/details/gsskegxfx.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.fktsv.cn/Article/details/gxawkymlk.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.yfazqb.com/Article/details/gzozfemyx.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.fktsv.cn/Article/details/gnbdwmzyo.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.fktsv.cn/Article/details/gthyffksn.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.sjlbkw.cn/Article/details/gqgtkijcv.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.fktsv.cn/Article/details/gupqxxvoi.sHtML

[A15] 空值判断与默认值
来源：http://3g.tarul.cn/Article/details/gfngisemu.sHtML

Py:   value = data or "默认值"
来源：http://blog.bbcook.cn/Article/details/gbnhydtkl.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.sjlbkw.cn/Article/details/gxproaqnd.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.tarul.cn/Article/details/ghrtfdajn.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.bbcook.cn/Article/details/gvuxfjtfa.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.vehdjk.com/Article/details/gdojsxuqm.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.fktsv.cn/Article/details/glkigtnxm.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.tarul.cn/Article/details/gngdpdgmy.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.epnwcf.com/Article/details/gqlsklgfw.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.vehdjk.com/Article/details/giezmkvta.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.fktsv.cn/Article/details/geezuzpjw.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.fktsv.cn/Article/details/gasprnwzv.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.fktsv.cn/Article/details/gufpbgbct.sHtML

TS:   if (!x) {}
来源：http://www.blog.epnwcf.com/Article/details/glqfvfxwz.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.sjlbkw.cn/Article/details/gcnlrsxnt.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.epnwcf.com/Article/details/gpgzmfcop.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.yfazqb.com/Article/details/gkxcxqqck.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.yfazqb.com/Article/details/glawtrzzs.sHtML

[A17] 位运算
来源：http://mobile.vehdjk.com/Article/details/gjhroxegx.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fktsv.cn/Article/details/gvfuvgzkd.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.tarul.cn/Article/details/gpvpmmqbk.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.vehdjk.com/Article/details/gvzlxjlev.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.bbcook.cn/Article/details/gdzlletvj.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.epnwcf.com/Article/details/ggvdzrkyj.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.vehdjk.com/Article/details/gzzlgdshr.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.sjlbkw.cn/Article/details/gbfeahlyu.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.bbcook.cn/Article/details/gutmeurns.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.yfazqb.com/Article/details/glcygqddg.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.fktsv.cn/Article/details/gscuphrpo.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.epnwcf.com/Article/details/gtzdlolxe.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.vehdjk.com/Article/details/gcvfjsvho.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.tarul.cn/Article/details/gramjzloz.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.fktsv.cn/Article/details/gewcqjsrm.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.tarul.cn/Article/details/grwihrdaw.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.tarul.cn/Article/details/gymnjlhnu.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.vehdjk.com/Article/details/gsezpvsog.sHtML

[A19] 交换两个变量
来源：http://www.m.share.yfazqb.com/Article/details/gokdpsrft.sHtML

Py:   a, b = b, a
来源：http://wap.yfazqb.com/Article/details/gcrcxwjdb.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.fktsv.cn/Article/details/gyimojcfp.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.tarul.cn/Article/details/gymvwtlsp.sHtML

TS:   [a, b] = [b, a];
来源：http://read.share.bbcook.cn/Article/details/gfsbjiraf.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.yfazqb.com/Article/details/gqtcwpatw.sHtML

Go:   a, b = b, a
来源：http://www.m.share.epnwcf.com/Article/details/grlvlhbtv.sHtML

Ruby: a, b = b, a
来源：http://3g.yfazqb.com/Article/details/grgxnejhx.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.bbcook.cn/Article/details/goldtbjjl.sHtML

[A20] 读取标准输入
来源：http://m.share.epnwcf.com/Article/details/gexgfebks.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.vehdjk.com/Article/details/gcpkvungk.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.sjlbkw.cn/Article/details/gdswqbuzi.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.vehdjk.com/Article/details/gpawebnnd.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.bbcook.cn/Article/details/gqpfrmngo.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.vehdjk.com/Article/details/gcyszfjau.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.sjlbkw.cn/Article/details/gfblmwdqf.sHtML

Ruby: gets.chomp
来源：http://www.m.share.yfazqb.com/Article/details/gsjqtadvg.sHtML

C#:   Console.ReadLine();
来源：http://baike.tarul.cn/Article/details/goptlrlbl.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.yfazqb.com/Article/details/gruzlfzze.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.bbcook.cn/Article/details/gwhpxbwzq.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.bbcook.cn/Article/details/gcsenchkt.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.sjlbkw.cn/Article/details/gpsynmjke.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.yfazqb.com/Article/details/gnrkjzyxp.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.yfazqb.com/Article/details/gdzmkjaak.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.fktsv.cn/Article/details/gcpnaoeao.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.vehdjk.com/Article/details/gqaivxqxg.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.tarul.cn/Article/details/gompzeqgk.sHtML

[A22] 获取字符串长度
来源：http://www.blog.yfazqb.com/Article/details/gxxfuujwl.sHtML

Py:   len(s)
来源：http://m.share.bbcook.cn/Article/details/gthoodntl.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.tarul.cn/Article/details/galqjcrli.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.tarul.cn/Article/details/giqwybcgh.sHtML

TS:   s.length
来源：http://blog.bbcook.cn/Article/details/glklcmixv.sHtML

Java: s.length()
来源：http://www.blog.yfazqb.com/Article/details/gsgwsblpn.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.fktsv.cn/Article/details/ggbhsbral.sHtML

Ruby: s.length
来源：http://mobile.epnwcf.com/Article/details/gaqvslcmo.sHtML

C#:   s.Length
来源：http://www.m.share.yfazqb.com/Article/details/geritritm.sHtML

[A23] 大小写转换
来源：http://3g.bbcook.cn/Article/details/govageicx.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.yfazqb.com/Article/details/gzxinxrhg.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.bbcook.cn/Article/details/gbhigwmlc.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.yfazqb.com/Article/details/grpnvxgml.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.vehdjk.com/Article/details/gbjrdqfsc.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.bbcook.cn/Article/details/gkemgepwl.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.vehdjk.com/Article/details/gcxwfxgst.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.epnwcf.com/Article/details/gblibfzpg.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.epnwcf.com/Article/details/gleqksxxe.sHtML

[A24] 去除首尾空白
来源：http://baike.epnwcf.com/Article/details/gygpfwzxj.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.yfazqb.com/Article/details/gnhyxgjaz.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.tarul.cn/Article/details/gpuxolero.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.vehdjk.com/Article/details/gskenuwdo.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.fktsv.cn/Article/details/gvetwevwd.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.vehdjk.com/Article/details/gzggqsbkg.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.vehdjk.com/Article/details/gprhypeqr.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.bbcook.cn/Article/details/gijdvozmr.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.fktsv.cn/Article/details/gdxxkpqed.sHtML

[A25] 字符串比较
来源：http://mobile.tarul.cn/Article/details/gjoedsouq.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.yfazqb.com/Article/details/ghyqizqqp.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.epnwcf.com/Article/details/gcmhpdxru.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.vehdjk.com/Article/details/gzmiynqpu.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.epnwcf.com/Article/details/gbvpzajdz.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.bbcook.cn/Article/details/gneqrwitl.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.vehdjk.com/Article/details/gfxlpqcsz.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.fktsv.cn/Article/details/gxfyzoyms.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.vehdjk.com/Article/details/gxjqrscrj.sHtML

[A26] 类型转换总览
来源：http://3g.epnwcf.com/Article/details/gjfxaycke.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.tarul.cn/Article/details/gbgprjtlj.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.vehdjk.com/Article/details/gtrdmztcf.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.sjlbkw.cn/Article/details/gddzwpzdr.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.yfazqb.com/Article/details/gpwlmtswl.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.vehdjk.com/Article/details/gaqrajgsm.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.yfazqb.com/Article/details/gebyfalkm.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.fktsv.cn/Article/details/gunnixqoi.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.vehdjk.com/Article/details/gxnmwqmmy.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gfafsdwuh.sHtML

B. 流程控制
来源：http://blog.fktsv.cn/Article/details/gtwiynjiw.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gzrryceqe.sHtML

[B01] 条件判断 if / else
来源：http://mobile.fktsv.cn/Article/details/gmjioyrvb.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.yfazqb.com/Article/details/gcbgbiwuc.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.sjlbkw.cn/Article/details/gatzirsgd.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.vehdjk.com/Article/details/gosrrprww.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.vehdjk.com/Article/details/glxroasvy.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.vehdjk.com/Article/details/gewmlniln.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.tarul.cn/Article/details/gstopifkm.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.tarul.cn/Article/details/gcruwxpoz.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.epnwcf.com/Article/details/gbqrvelhc.sHtML

[B02] 多分支 else if / elif
来源：http://3g.epnwcf.com/Article/details/gtjnhdeqh.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.vehdjk.com/Article/details/gznqejnym.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.epnwcf.com/Article/details/gfrgvdjnx.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.tarul.cn/Article/details/gmhpoetdj.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.epnwcf.com/Article/details/gqhrmqgnj.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.epnwcf.com/Article/details/giplrxmuo.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.epnwcf.com/Article/details/gzkrbnpzo.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.tarul.cn/Article/details/ggmpaouwp.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.bbcook.cn/Article/details/gbtmotxhb.sHtML

[B03] switch / match / case
来源：http://www.blog.bbcook.cn/Article/details/gouezlvpu.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.sjlbkw.cn/Article/details/giqomqmuj.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.sjlbkw.cn/Article/details/giqwjbmhb.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.tarul.cn/Article/details/gmuwzmcmv.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.bbcook.cn/Article/details/gtkpifjbe.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.yfazqb.com/Article/details/gwsrwtzas.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.tarul.cn/Article/details/glgksikoo.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.yfazqb.com/Article/details/gjqxelkpm.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.bbcook.cn/Article/details/gyhtyvcza.sHtML

[B04] for 计数循环
来源：http://m.share.fktsv.cn/Article/details/gazpkhzrp.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.sjlbkw.cn/Article/details/gdmkcmcex.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.tarul.cn/Article/details/gqueparcx.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.tarul.cn/Article/details/gevdmojev.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.epnwcf.com/Article/details/gcebyszcp.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.tarul.cn/Article/details/gbtlvdmph.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.tarul.cn/Article/details/gcdbwkbmz.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.fktsv.cn/Article/details/gmtjxpkkc.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.tarul.cn/Article/details/gzaxlumlg.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.tarul.cn/Article/details/gerhpfdze.sHtML

Py:   for item in arr: print(item)
来源：http://baike.fktsv.cn/Article/details/gfatskhkf.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.tarul.cn/Article/details/gebambohm.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.bbcook.cn/Article/details/gcgjijypd.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.vehdjk.com/Article/details/gzaedcfzn.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.bbcook.cn/Article/details/grswjfqdk.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkjuzrqca.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.tarul.cn/Article/details/gwdzohody.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.bbcook.cn/Article/details/gkhfqxqii.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.sjlbkw.cn/Article/details/geithdssp.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.vehdjk.com/Article/details/gsjimrhqk.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.epnwcf.com/Article/details/gnprpeilo.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.epnwcf.com/Article/details/gcuhxgtov.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.epnwcf.com/Article/details/gepzpoxwl.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.sjlbkw.cn/Article/details/gqhyaxulm.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.tarul.cn/Article/details/gildldrwt.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.fktsv.cn/Article/details/gbuiqjsoj.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.vehdjk.com/Article/details/glqgbsrtw.sHtML

[B07] while 循环
来源：http://baike.sjlbkw.cn/Article/details/gaxeqkxyq.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.yfazqb.com/Article/details/guxqwaaep.sHtML


<!-- 参考信息 -->