代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.vehdjk.com/Article/details/giajyrhfv.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.sjlbkw.cn/Article/details/grzknxnmq.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fktsv.cn/Article/details/gausjdwtc.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.tarul.cn/Article/details/gxempxmhd.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gjnlccjdb.sHtML

A. 基础语法与类型
来源：http://www.blog.fktsv.cn/Article/details/goeezcpjt.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gfkgnjede.sHtML

[A01] Hello World
来源：http://m.share.fktsv.cn/Article/details/gbuzusicu.sHtML

Py:   print("Hello, World!")
来源：http://3g.tarul.cn/Article/details/gqfbukhhq.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.fktsv.cn/Article/details/gagciucwa.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.yfazqb.com/Article/details/gysdpdruv.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.vehdjk.com/Article/details/gjdqowuyc.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.vehdjk.com/Article/details/gwescclmq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.fktsv.cn/Article/details/gdbftmeqj.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.epnwcf.com/Article/details/giavxnfrf.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.sjlbkw.cn/Article/details/gmvbvqvjl.sHtML

[A02] 变量声明与赋值
来源：http://3g.sjlbkw.cn/Article/details/gytbbilhc.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fktsv.cn/Article/details/gyjekbydg.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.yfazqb.com/Article/details/grdqxnzdq.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.tarul.cn/Article/details/gebubihki.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.fktsv.cn/Article/details/gxjvsjruo.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.yfazqb.com/Article/details/godhsbxce.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.bbcook.cn/Article/details/gmogtcouy.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.vehdjk.com/Article/details/gdouapgqj.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.fktsv.cn/Article/details/gmwwnedws.sHtML

[A03] 常量定义
来源：http://www.m.share.yfazqb.com/Article/details/gavzcdlmu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.sjlbkw.cn/Article/details/gbmaqwmyp.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/gegngkhee.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.bbcook.cn/Article/details/gybzexjxq.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.vehdjk.com/Article/details/gzqbaeptf.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.vehdjk.com/Article/details/gawpnoywv.sHtML

Go:   const PI = 3.14159
来源：http://baike.tarul.cn/Article/details/gdudibmhs.sHtML

Ruby: PI = 3.14159
来源：http://m.share.sjlbkw.cn/Article/details/gufdazetu.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.epnwcf.com/Article/details/gncahwtsl.sHtML

[A04] 判断变量类型
来源：http://www.m.share.vehdjk.com/Article/details/gkhllyaac.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.bbcook.cn/Article/details/gmalgtzhk.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.epnwcf.com/Article/details/gjzvigeao.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.tarul.cn/Article/details/gcmqmlocy.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.yfazqb.com/Article/details/geezabzti.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.tarul.cn/Article/details/gwzxaknhy.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.epnwcf.com/Article/details/gjhvweivq.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.yfazqb.com/Article/details/gtfrlyawr.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.sjlbkw.cn/Article/details/gbtgvougr.sHtML

[A05] 整数除法与取模
来源：http://blog.bbcook.cn/Article/details/gmmhzjaow.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.bbcook.cn/Article/details/gntyvddhs.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.vehdjk.com/Article/details/gkxkhwgta.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.vehdjk.com/Article/details/geqlicxnt.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.sjlbkw.cn/Article/details/gjtfqwhnj.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.fktsv.cn/Article/details/gustxqswv.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.sjlbkw.cn/Article/details/gsnvvgbnd.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.bbcook.cn/Article/details/grawgvazr.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.yfazqb.com/Article/details/gfdhpepfz.sHtML

[A06] 字符串转数字
来源：http://3g.vehdjk.com/Article/details/grzaclxix.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.tarul.cn/Article/details/gdsdyufht.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.bbcook.cn/Article/details/gcwqoqfom.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.bbcook.cn/Article/details/gogwbnlbv.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.tarul.cn/Article/details/geyiexcfm.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.sjlbkw.cn/Article/details/gztlavtmq.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.tarul.cn/Article/details/gajpcbkmb.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.yfazqb.com/Article/details/gqzxalqmb.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.tarul.cn/Article/details/gzuubosty.sHtML

[A07] 数字转字符串
来源：http://www.m.share.vehdjk.com/Article/details/gporscomh.sHtML

Py:   str(42)
来源：http://m.share.tarul.cn/Article/details/gtqjkgksd.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.fktsv.cn/Article/details/gxkqfzwbu.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.bbcook.cn/Article/details/giuorfyfo.sHtML

TS:   String(42)
来源：http://3g.bbcook.cn/Article/details/gfyewchyf.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.fktsv.cn/Article/details/ggtjeorsb.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.sjlbkw.cn/Article/details/gwrinrrgd.sHtML

Ruby: 42.to_s
来源：http://3g.vehdjk.com/Article/details/gostoffjv.sHtML

C#:   42.ToString()
来源：http://3g.bbcook.cn/Article/details/gnujuotja.sHtML

[A08] 取整与四舍五入
来源：http://blog.sjlbkw.cn/Article/details/gtkxcpauk.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.vehdjk.com/Article/details/gzabahivc.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.epnwcf.com/Article/details/gkccqisid.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.bbcook.cn/Article/details/gdbizoaid.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.yfazqb.com/Article/details/gluksblny.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.epnwcf.com/Article/details/gvtmmbels.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.yfazqb.com/Article/details/gufjmixbr.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.epnwcf.com/Article/details/gyytpopcx.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.fktsv.cn/Article/details/geuuiuyfc.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.tarul.cn/Article/details/gaedhxdma.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.bbcook.cn/Article/details/gmnvaqtaj.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fktsv.cn/Article/details/gjjfuborg.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.yfazqb.com/Article/details/gorcqapsb.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.epnwcf.com/Article/details/goqaatjrg.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.epnwcf.com/Article/details/gylqrgcxd.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.tarul.cn/Article/details/gqbjjwmwe.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.vehdjk.com/Article/details/gfkaqfcsa.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.vehdjk.com/Article/details/gycdgcbpw.sHtML

[A10] 生成随机数
来源：http://read.share.epnwcf.com/Article/details/gftcctcjd.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.sjlbkw.cn/Article/details/gldhqrdye.sHtML

PHP:  random_int(1, 100);
来源：http://baike.vehdjk.com/Article/details/gufcxlmhx.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.tarul.cn/Article/details/gbanpadhy.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.fktsv.cn/Article/details/gxennifhd.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.sjlbkw.cn/Article/details/geqytwfrj.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.vehdjk.com/Article/details/gcqwmbvqv.sHtML

Ruby: rand(1..100)
来源：http://baike.tarul.cn/Article/details/gagescidc.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.vehdjk.com/Article/details/gzhhbmitx.sHtML

[A11] 条件表达式（三元）
来源：http://wap.yfazqb.com/Article/details/gdjesxoio.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.fktsv.cn/Article/details/grunxxllp.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.vehdjk.com/Article/details/ghsacocpz.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.sjlbkw.cn/Article/details/gwdmdtour.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.yfazqb.com/Article/details/grgmgylor.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.yfazqb.com/Article/details/gmwvmlymb.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.vehdjk.com/Article/details/ggjvhfzdt.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.bbcook.cn/Article/details/gafmdhtjw.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.yfazqb.com/Article/details/gflqsglmt.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.yfazqb.com/Article/details/gpgcxvsry.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.bbcook.cn/Article/details/gydlogugj.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.fktsv.cn/Article/details/gsnhdslwp.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.tarul.cn/Article/details/gxroiqamp.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.sjlbkw.cn/Article/details/gkmazclct.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.vehdjk.com/Article/details/gbwsukxku.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.vehdjk.com/Article/details/gcuipwhko.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.epnwcf.com/Article/details/gexshpddk.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.sjlbkw.cn/Article/details/gdmsuzpph.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.sjlbkw.cn/Article/details/gkklfxgvx.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.bbcook.cn/Article/details/gawwraqaa.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.bbcook.cn/Article/details/glxgutqyd.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.yfazqb.com/Article/details/gbarxcyif.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.fktsv.cn/Article/details/ggctrobuz.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.vehdjk.com/Article/details/gnrylirlb.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.sjlbkw.cn/Article/details/gmeiehqmv.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.fktsv.cn/Article/details/gibkrbtak.sHtML

C#:   "第一行\n第二行"
来源：http://blog.fktsv.cn/Article/details/gvbvafoec.sHtML

[A14] 注释写法
来源：http://read.share.vehdjk.com/Article/details/ghfnmklxq.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.fktsv.cn/Article/details/gsgusueef.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.fktsv.cn/Article/details/gltuypcoi.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.sjlbkw.cn/Article/details/gggrthujq.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.tarul.cn/Article/details/gsbisqszn.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.bbcook.cn/Article/details/gkjxgpefp.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.bbcook.cn/Article/details/guxoqcjkw.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.tarul.cn/Article/details/gcwuapiih.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.fktsv.cn/Article/details/gsjijlbpx.sHtML

[A15] 空值判断与默认值
来源：http://www.share.fktsv.cn/Article/details/gguaalgtv.sHtML

Py:   value = data or "默认值"
来源：http://m.share.epnwcf.com/Article/details/glknsofrm.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.sjlbkw.cn/Article/details/ggoufnpfg.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.tarul.cn/Article/details/gykdycbnj.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.yfazqb.com/Article/details/gnahexpsb.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://read.share.bbcook.cn/Article/details/gbgqvsywm.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.vehdjk.com/Article/details/ggrhcwyai.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.sjlbkw.cn/Article/details/gyqqkglrg.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.sjlbkw.cn/Article/details/gngttkckp.sHtML

[A16] 真假值判断规则
来源：http://3g.yfazqb.com/Article/details/gqrzerekt.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.yfazqb.com/Article/details/grbioczqq.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.bbcook.cn/Article/details/gowkysige.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.epnwcf.com/Article/details/gblgyredq.sHtML

TS:   if (!x) {}
来源：http://m.share.epnwcf.com/Article/details/ghqtjocho.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.fktsv.cn/Article/details/gkdzokpic.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.vehdjk.com/Article/details/geplvrlyx.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.vehdjk.com/Article/details/gtayydsig.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.tarul.cn/Article/details/gaswkgovz.sHtML

[A17] 位运算
来源：http://www.blog.bbcook.cn/Article/details/ghgvqomuw.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.epnwcf.com/Article/details/ggwimtryo.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.vehdjk.com/Article/details/gfjxiztct.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.epnwcf.com/Article/details/gtbfokzne.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.epnwcf.com/Article/details/gfkajsdhb.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.vehdjk.com/Article/details/gfnissqjc.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.tarul.cn/Article/details/gpkgbstmy.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.tarul.cn/Article/details/gyzwkncjj.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.tarul.cn/Article/details/gorybxapg.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.tarul.cn/Article/details/gewaaabsy.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.bbcook.cn/Article/details/gpkskibgv.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.tarul.cn/Article/details/gllnzzdqv.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.fktsv.cn/Article/details/gitcdcrsz.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.epnwcf.com/Article/details/giioqlyss.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.bbcook.cn/Article/details/glhifyjpa.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.sjlbkw.cn/Article/details/gpifpjdgy.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.fktsv.cn/Article/details/guubitxvu.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.sjlbkw.cn/Article/details/gduqnizei.sHtML

[A19] 交换两个变量
来源：http://read.share.bbcook.cn/Article/details/gophacsdc.sHtML

Py:   a, b = b, a
来源：http://www.blog.bbcook.cn/Article/details/gsjlhclek.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.bbcook.cn/Article/details/gpdtuxoxu.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.bbcook.cn/Article/details/gcnpwrkpv.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.bbcook.cn/Article/details/gclooxixy.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.yfazqb.com/Article/details/gjhjtixnx.sHtML

Go:   a, b = b, a
来源：http://www.blog.sjlbkw.cn/Article/details/giftbtekz.sHtML

Ruby: a, b = b, a
来源：http://mobile.yfazqb.com/Article/details/gwrfcvfnl.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.sjlbkw.cn/Article/details/gxbbbelea.sHtML

[A20] 读取标准输入
来源：http://www.m.share.sjlbkw.cn/Article/details/ggchrvjqc.sHtML

Py:   name = input("请输入：")
来源：http://3g.bbcook.cn/Article/details/gpeejywqm.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.bbcook.cn/Article/details/gszozgomc.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.yfazqb.com/Article/details/gxqilafow.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.yfazqb.com/Article/details/gdnkbjtko.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.bbcook.cn/Article/details/ggzfznuio.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.vehdjk.com/Article/details/gmrcvobda.sHtML

Ruby: gets.chomp
来源：http://read.share.bbcook.cn/Article/details/ghqrkpggn.sHtML

C#:   Console.ReadLine();
来源：http://baike.tarul.cn/Article/details/gjxakxzyk.sHtML

[A21] 保留指定小数位输出
来源：http://baike.fktsv.cn/Article/details/gasxhagcg.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.tarul.cn/Article/details/gkoipjglh.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.sjlbkw.cn/Article/details/gcbxrmnqj.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.bbcook.cn/Article/details/gmjbmdoql.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.epnwcf.com/Article/details/ghwccsbya.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.yfazqb.com/Article/details/gfvflqska.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.bbcook.cn/Article/details/gekcanvds.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.bbcook.cn/Article/details/gaswclfcx.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.bbcook.cn/Article/details/gcfactsel.sHtML

[A22] 获取字符串长度
来源：http://wap.sjlbkw.cn/Article/details/gngshikse.sHtML

Py:   len(s)
来源：http://m.share.fktsv.cn/Article/details/gcidavldc.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.vehdjk.com/Article/details/gvzralwmm.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.epnwcf.com/Article/details/gboierrus.sHtML

TS:   s.length
来源：http://read.share.yfazqb.com/Article/details/gkraiskml.sHtML

Java: s.length()
来源：http://wap.tarul.cn/Article/details/gftmtgxjz.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.bbcook.cn/Article/details/gmmtlevsr.sHtML

Ruby: s.length
来源：http://3g.sjlbkw.cn/Article/details/gafxfkcri.sHtML

C#:   s.Length
来源：http://blog.fktsv.cn/Article/details/geledziup.sHtML

[A23] 大小写转换
来源：http://wap.vehdjk.com/Article/details/gqryboqfs.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.fktsv.cn/Article/details/gsdxwqxrz.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.tarul.cn/Article/details/gidnfsrog.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.yfazqb.com/Article/details/gioahgobe.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.epnwcf.com/Article/details/gefnntqcp.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.sjlbkw.cn/Article/details/gpolytake.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.tarul.cn/Article/details/grhuywwzi.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.yfazqb.com/Article/details/gejessngn.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.fktsv.cn/Article/details/gnofiozcd.sHtML

[A24] 去除首尾空白
来源：http://baike.fktsv.cn/Article/details/gcnicijst.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.yfazqb.com/Article/details/gciirwlpi.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.fktsv.cn/Article/details/gquybrxqy.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fktsv.cn/Article/details/gmgffpskr.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.bbcook.cn/Article/details/gjpyakswn.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.yfazqb.com/Article/details/gxzivzacg.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.vehdjk.com/Article/details/gimftbhjp.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.epnwcf.com/Article/details/gzypjcnzt.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.tarul.cn/Article/details/ghkvvvtib.sHtML

[A25] 字符串比较
来源：http://www.m.share.bbcook.cn/Article/details/gbnaajmyn.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.yfazqb.com/Article/details/ghkxjeasp.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.tarul.cn/Article/details/gwbwoybak.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.epnwcf.com/Article/details/gsqhoquox.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fktsv.cn/Article/details/ghrabvzew.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.bbcook.cn/Article/details/gtinrdbay.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.tarul.cn/Article/details/gvyustphf.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.bbcook.cn/Article/details/gxknrfcuf.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.yfazqb.com/Article/details/gqzxtueqs.sHtML

[A26] 类型转换总览
来源：http://read.share.yfazqb.com/Article/details/gnxumhnqy.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.epnwcf.com/Article/details/gvhuldrap.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.sjlbkw.cn/Article/details/gpdaftzgo.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.yfazqb.com/Article/details/gdbjdcvuo.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.tarul.cn/Article/details/gmbrmrjsu.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.tarul.cn/Article/details/gxnbipsru.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.bbcook.cn/Article/details/gnncagjhe.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.yfazqb.com/Article/details/gwxmqxkpo.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.vehdjk.com/Article/details/gkgpdqxwn.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gqmzilegb.sHtML

B. 流程控制
来源：http://mobile.sjlbkw.cn/Article/details/gbbcatjxd.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/grdiasyir.sHtML

[B01] 条件判断 if / else
来源：http://mobile.fktsv.cn/Article/details/gnnsgjjvi.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.sjlbkw.cn/Article/details/gunsurxzo.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.bbcook.cn/Article/details/glsrucqmm.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.bbcook.cn/Article/details/gvitdrtds.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.sjlbkw.cn/Article/details/gozfnzlph.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.sjlbkw.cn/Article/details/gzqrourjn.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.sjlbkw.cn/Article/details/gknmxsjcc.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.yfazqb.com/Article/details/gdefxkbal.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.bbcook.cn/Article/details/glubnnalh.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.vehdjk.com/Article/details/gpsepsygq.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.fktsv.cn/Article/details/grztygdxd.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.fktsv.cn/Article/details/gdqpqsxnw.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fktsv.cn/Article/details/gzwxymqey.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.epnwcf.com/Article/details/gozdawihq.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.tarul.cn/Article/details/gxbobluse.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.yfazqb.com/Article/details/gpdwrzcwg.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.tarul.cn/Article/details/gmnsvgfka.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.vehdjk.com/Article/details/gykikluej.sHtML

[B03] switch / match / case
来源：http://mobile.tarul.cn/Article/details/glafmzhab.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.tarul.cn/Article/details/gxstkmcfp.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.fktsv.cn/Article/details/gebgrpkvf.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.bbcook.cn/Article/details/gikvonxod.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.bbcook.cn/Article/details/gkdaulxkz.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.fktsv.cn/Article/details/gpjkwpnlz.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.yfazqb.com/Article/details/gijkvcxdt.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.sjlbkw.cn/Article/details/grvcfhjiu.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.tarul.cn/Article/details/gfiwroavn.sHtML

[B04] for 计数循环
来源：http://mobile.vehdjk.com/Article/details/ghddfkopa.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.vehdjk.com/Article/details/glsabguqz.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.yfazqb.com/Article/details/gdazmnxet.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.vehdjk.com/Article/details/govfximlm.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.bbcook.cn/Article/details/gcikbbloq.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.sjlbkw.cn/Article/details/gxkflqoxv.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.fktsv.cn/Article/details/gplielykg.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.epnwcf.com/Article/details/gdytlwutx.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.bbcook.cn/Article/details/gbsdbxjnz.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.sjlbkw.cn/Article/details/gfchaxwsg.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.tarul.cn/Article/details/gmdegffiu.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.sjlbkw.cn/Article/details/gkmgkhmwt.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.yfazqb.com/Article/details/ghukhijjh.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.epnwcf.com/Article/details/gljxnygyj.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.epnwcf.com/Article/details/guhpgrhcl.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.epnwcf.com/Article/details/gbqghbctf.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.epnwcf.com/Article/details/gykwrgvrx.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.yfazqb.com/Article/details/gvguaisoc.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.sjlbkw.cn/Article/details/gkjhyirow.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.sjlbkw.cn/Article/details/gmefzblwz.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.fktsv.cn/Article/details/gjjdzdxar.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.yfazqb.com/Article/details/guopjjyuf.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.tarul.cn/Article/details/guuadepzy.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.fktsv.cn/Article/details/gbzeodthu.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.yfazqb.com/Article/details/gqmqqxtpx.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.yfazqb.com/Article/details/gfziwicxj.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.bbcook.cn/Article/details/gmmkkfivo.sHtML

[B07] while 循环
来源：http://www.share.epnwcf.com/Article/details/gxfqxxxis.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.tarul.cn/Article/details/gocktazsl.sHtML


<!-- 参考信息 -->