代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.tarul.cn/Article/details/ggqsngffm.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.tarul.cn/Article/details/ghiiygusj.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.bbcook.cn/Article/details/gzyymlakh.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.tarul.cn/Article/details/gjeteiyfg.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/geyluphxp.sHtML

A. 基础语法与类型
来源：http://mobile.yfazqb.com/Article/details/gejgbfbxx.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/guchfbnda.sHtML

[A01] Hello World
来源：http://www.share.epnwcf.com/Article/details/gagxsxdqt.sHtML

Py:   print("Hello, World!")
来源：http://www.share.epnwcf.com/Article/details/gkbfjphwr.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.fktsv.cn/Article/details/gsfkqhlbt.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.vehdjk.com/Article/details/gmllkqifh.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.vehdjk.com/Article/details/gkfsdzdpx.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.fktsv.cn/Article/details/gdiljsklh.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.vehdjk.com/Article/details/gpsbwwtoe.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.sjlbkw.cn/Article/details/gitcbyhzt.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.bbcook.cn/Article/details/gdbdivimo.sHtML

[A02] 变量声明与赋值
来源：http://wap.yfazqb.com/Article/details/gtznbonko.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.vehdjk.com/Article/details/gdjvjfjtb.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.sjlbkw.cn/Article/details/gxkqrfhws.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.bbcook.cn/Article/details/gxejengfy.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.bbcook.cn/Article/details/gsfvsoihr.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.vehdjk.com/Article/details/gmcdfflku.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.bbcook.cn/Article/details/gkjmwppop.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.tarul.cn/Article/details/gyfwflzxj.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.epnwcf.com/Article/details/gjcwnutrw.sHtML

[A03] 常量定义
来源：http://baike.sjlbkw.cn/Article/details/gudobgmsv.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.vehdjk.com/Article/details/gmxckqrli.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.yfazqb.com/Article/details/gxvjmjrra.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.tarul.cn/Article/details/gejztcfjr.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.tarul.cn/Article/details/ghzdahgff.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/grjkwhjca.sHtML

Go:   const PI = 3.14159
来源：http://m.share.tarul.cn/Article/details/grmlkvyeb.sHtML

Ruby: PI = 3.14159
来源：http://www.share.vehdjk.com/Article/details/gckkttgyy.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.bbcook.cn/Article/details/gkuoszvau.sHtML

[A04] 判断变量类型
来源：http://blog.vehdjk.com/Article/details/gspivcdfc.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.sjlbkw.cn/Article/details/gfjgmukug.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.bbcook.cn/Article/details/gopisbbrx.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.tarul.cn/Article/details/gidcpqxtn.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.bbcook.cn/Article/details/gjvwhqvtg.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.bbcook.cn/Article/details/gmxgboeig.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.fktsv.cn/Article/details/guvxmpbpm.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.epnwcf.com/Article/details/gxqrotnyo.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.yfazqb.com/Article/details/gtmxydcwi.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.tarul.cn/Article/details/gnndwtafv.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.tarul.cn/Article/details/gsfmnadti.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.epnwcf.com/Article/details/ggvuakdhl.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.tarul.cn/Article/details/ggjmejptz.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.bbcook.cn/Article/details/gczwmwfcy.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.vehdjk.com/Article/details/gbxamhvcm.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.epnwcf.com/Article/details/guwagtvjw.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.epnwcf.com/Article/details/gxhrgjbax.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gpfedfate.sHtML

[A06] 字符串转数字
来源：http://www.share.fktsv.cn/Article/details/gihkrgujo.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.sjlbkw.cn/Article/details/gsdsylsfu.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.vehdjk.com/Article/details/gszljtdje.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.bbcook.cn/Article/details/gzhayatjf.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.epnwcf.com/Article/details/gswvvsrum.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.tarul.cn/Article/details/ghyqdxidm.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.yfazqb.com/Article/details/gnvktnlhf.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.sjlbkw.cn/Article/details/gsltjfibe.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.bbcook.cn/Article/details/glwvbglhc.sHtML

[A07] 数字转字符串
来源：http://baike.yfazqb.com/Article/details/gkhhormqg.sHtML

Py:   str(42)
来源：http://3g.epnwcf.com/Article/details/gkqdjorqb.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.tarul.cn/Article/details/gzjkaqkqm.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.tarul.cn/Article/details/ggzigubtj.sHtML

TS:   String(42)
来源：http://blog.vehdjk.com/Article/details/gmfxzqbpk.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.sjlbkw.cn/Article/details/gqwuxpywf.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.vehdjk.com/Article/details/guhrzwqem.sHtML

Ruby: 42.to_s
来源：http://3g.epnwcf.com/Article/details/gmtilbfrl.sHtML

C#:   42.ToString()
来源：http://read.share.bbcook.cn/Article/details/gqtcdcezi.sHtML

[A08] 取整与四舍五入
来源：http://mobile.bbcook.cn/Article/details/gvsnbkyvy.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.sjlbkw.cn/Article/details/gnkypmwok.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.epnwcf.com/Article/details/gkilgxuhw.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.bbcook.cn/Article/details/gcirscwnh.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.bbcook.cn/Article/details/gxpppould.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.vehdjk.com/Article/details/gicldtodw.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.fktsv.cn/Article/details/glnvajxrz.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.yfazqb.com/Article/details/gkvjjpjnw.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.tarul.cn/Article/details/gbblmodgq.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.fktsv.cn/Article/details/gjonhaosl.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.sjlbkw.cn/Article/details/glhhxfskj.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.vehdjk.com/Article/details/gbgtnjfus.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.sjlbkw.cn/Article/details/gzrpiqvas.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.tarul.cn/Article/details/gkqmgebww.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.sjlbkw.cn/Article/details/glmdjnafi.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.fktsv.cn/Article/details/gmbqdspop.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.bbcook.cn/Article/details/gypmearqi.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsvoelkhh.sHtML

[A10] 生成随机数
来源：http://www.share.epnwcf.com/Article/details/gcurbtvrq.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.yfazqb.com/Article/details/gfynjcznj.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqrpzakap.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.epnwcf.com/Article/details/gsfnduwvn.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.tarul.cn/Article/details/gebeladcd.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.fktsv.cn/Article/details/gmwzvnybi.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.yfazqb.com/Article/details/grcplnpky.sHtML

Ruby: rand(1..100)
来源：http://blog.yfazqb.com/Article/details/gxiuxzihr.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.fktsv.cn/Article/details/gzssbimdx.sHtML

[A11] 条件表达式（三元）
来源：http://wap.yfazqb.com/Article/details/glpzmjwki.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.yfazqb.com/Article/details/gumdfmmla.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.sjlbkw.cn/Article/details/gelssiwmt.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.sjlbkw.cn/Article/details/gkbodrgyt.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.tarul.cn/Article/details/gomvvkvyv.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.epnwcf.com/Article/details/gqyzqpymw.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.fktsv.cn/Article/details/ggegmfsxs.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.fktsv.cn/Article/details/gmmlkufsr.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.sjlbkw.cn/Article/details/gqrwxauvb.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.yfazqb.com/Article/details/gshrzfwyl.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.tarul.cn/Article/details/gurleqyaq.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.tarul.cn/Article/details/gondigknl.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.sjlbkw.cn/Article/details/gcawissak.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.yfazqb.com/Article/details/gnmanfpqc.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.yfazqb.com/Article/details/guzjdafce.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.tarul.cn/Article/details/goaiatixp.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.yfazqb.com/Article/details/gmwuvylpc.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.fktsv.cn/Article/details/gomfayezz.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.bbcook.cn/Article/details/gtlbcpclt.sHtML

Py:   "第一行\n第二行"
来源：http://baike.tarul.cn/Article/details/glojindwi.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.yfazqb.com/Article/details/gtnfbwltd.sHtML

JS:   "第一行\n第二行"
来源：http://wap.epnwcf.com/Article/details/gcwmfeczw.sHtML

TS:   "第一行\n第二行"
来源：http://blog.vehdjk.com/Article/details/gsydwhjxs.sHtML

Java: "第一行\n第二行"
来源：http://3g.bbcook.cn/Article/details/guuusnysx.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.tarul.cn/Article/details/gyvycbjmp.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.tarul.cn/Article/details/ghtrjurnu.sHtML

C#:   "第一行\n第二行"
来源：http://3g.epnwcf.com/Article/details/gnhaohaec.sHtML

[A14] 注释写法
来源：http://mobile.bbcook.cn/Article/details/gizrcbkus.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.bbcook.cn/Article/details/gttpovhqp.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.fktsv.cn/Article/details/gqolglyno.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.vehdjk.com/Article/details/gsneiutxr.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.epnwcf.com/Article/details/ghcttlruq.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.sjlbkw.cn/Article/details/gkpeiwwch.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.yfazqb.com/Article/details/ggscaczko.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.fktsv.cn/Article/details/garnidwdn.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.vehdjk.com/Article/details/gihztztwn.sHtML

[A15] 空值判断与默认值
来源：http://read.share.sjlbkw.cn/Article/details/gnrzpkrqb.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.sjlbkw.cn/Article/details/gxqyqfxgu.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.epnwcf.com/Article/details/geflovfep.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.yfazqb.com/Article/details/gritqzwys.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.fktsv.cn/Article/details/gyqcrfeaz.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.sjlbkw.cn/Article/details/gozoodokk.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.fktsv.cn/Article/details/grgjdtqwi.sHtML

Ruby: value = data || "默认值"
来源：http://wap.epnwcf.com/Article/details/giaucrqav.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.tarul.cn/Article/details/gjtqaffbk.sHtML

[A16] 真假值判断规则
来源：http://read.share.bbcook.cn/Article/details/gepajvqok.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.fktsv.cn/Article/details/gmsrcnagn.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.sjlbkw.cn/Article/details/gxlvyjbix.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.tarul.cn/Article/details/gafiuvrhp.sHtML

TS:   if (!x) {}
来源：http://www.share.epnwcf.com/Article/details/ggtgqpiva.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.sjlbkw.cn/Article/details/gpsqvlpoy.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.vehdjk.com/Article/details/gougmxvig.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.tarul.cn/Article/details/guaonarsg.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.vehdjk.com/Article/details/gejlzscle.sHtML

[A17] 位运算
来源：http://www.share.tarul.cn/Article/details/gwcnrspop.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.yfazqb.com/Article/details/gxnwzyjsr.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.fktsv.cn/Article/details/gmxovxslv.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.epnwcf.com/Article/details/gkymxifgb.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.yfazqb.com/Article/details/gwzwsoybt.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.tarul.cn/Article/details/gcerufbxp.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.tarul.cn/Article/details/gbznrnzqn.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.epnwcf.com/Article/details/gsxusbpid.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.tarul.cn/Article/details/gentanlwn.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.bbcook.cn/Article/details/gzslfmdit.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.epnwcf.com/Article/details/gcjmzufwd.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.sjlbkw.cn/Article/details/gvsqwfvog.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.fktsv.cn/Article/details/gdjcghtyc.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.tarul.cn/Article/details/gynwpjnqh.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.tarul.cn/Article/details/glknaxern.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.bbcook.cn/Article/details/giyrhumjf.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.tarul.cn/Article/details/gihbcjgtm.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.vehdjk.com/Article/details/gjmdzbkzw.sHtML

[A19] 交换两个变量
来源：http://wap.sjlbkw.cn/Article/details/gwclkfgmu.sHtML

Py:   a, b = b, a
来源：http://www.blog.sjlbkw.cn/Article/details/ggvgmbken.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.bbcook.cn/Article/details/gtmrrcnou.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.yfazqb.com/Article/details/gfgmtclll.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.fktsv.cn/Article/details/gjzfiknkh.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.tarul.cn/Article/details/glmyaazml.sHtML

Go:   a, b = b, a
来源：http://www.m.share.epnwcf.com/Article/details/gjosvqgbi.sHtML

Ruby: a, b = b, a
来源：http://3g.yfazqb.com/Article/details/gwcmxuirs.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.bbcook.cn/Article/details/grmwnahxa.sHtML

[A20] 读取标准输入
来源：http://www.m.share.tarul.cn/Article/details/gdhwdqfhi.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.bbcook.cn/Article/details/gyyfybjik.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.epnwcf.com/Article/details/gebkwtjxe.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.vehdjk.com/Article/details/guwdztigd.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.sjlbkw.cn/Article/details/gbddbxwqw.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.tarul.cn/Article/details/gkkqfzcqf.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.yfazqb.com/Article/details/gdaaaaymz.sHtML

Ruby: gets.chomp
来源：http://blog.yfazqb.com/Article/details/gmtzhpnxa.sHtML

C#:   Console.ReadLine();
来源：http://blog.epnwcf.com/Article/details/ghfyqbcag.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.sjlbkw.cn/Article/details/gjnzicare.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.vehdjk.com/Article/details/gdlasazzg.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.tarul.cn/Article/details/gpnlhnelv.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.vehdjk.com/Article/details/gjxabdloi.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.fktsv.cn/Article/details/gceenqcjv.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.epnwcf.com/Article/details/gldeummgc.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.tarul.cn/Article/details/grrweltsx.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.vehdjk.com/Article/details/guzuczkle.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.sjlbkw.cn/Article/details/gsnjosedz.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.tarul.cn/Article/details/gkbvtfppp.sHtML

Py:   len(s)
来源：http://read.share.bbcook.cn/Article/details/gzpeguogw.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.yfazqb.com/Article/details/guiphrlul.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.sjlbkw.cn/Article/details/gwmnsajqs.sHtML

TS:   s.length
来源：http://read.share.tarul.cn/Article/details/gwykvpfyo.sHtML

Java: s.length()
来源：http://baike.epnwcf.com/Article/details/ggviofxnr.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.yfazqb.com/Article/details/grhlkhegx.sHtML

Ruby: s.length
来源：http://mobile.bbcook.cn/Article/details/gacgzqgxw.sHtML

C#:   s.Length
来源：http://blog.sjlbkw.cn/Article/details/gvozmgchj.sHtML

[A23] 大小写转换
来源：http://wap.sjlbkw.cn/Article/details/grbxxwlzq.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.bbcook.cn/Article/details/glsltscbz.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.tarul.cn/Article/details/gfbdsekoq.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.vehdjk.com/Article/details/gzrdtlblx.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.sjlbkw.cn/Article/details/gtsirkttw.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.yfazqb.com/Article/details/gafbszqka.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.fktsv.cn/Article/details/gaipzmael.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.tarul.cn/Article/details/gzrwjevze.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.fktsv.cn/Article/details/gnhhpinhi.sHtML

[A24] 去除首尾空白
来源：http://www.share.yfazqb.com/Article/details/gwohmprsa.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.yfazqb.com/Article/details/gyurezobk.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.tarul.cn/Article/details/gakvqkdvs.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.epnwcf.com/Article/details/ggeqsyndw.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.bbcook.cn/Article/details/gufgwfwbx.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.epnwcf.com/Article/details/ggdqprweo.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.epnwcf.com/Article/details/gacgjkayo.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.sjlbkw.cn/Article/details/gmdmutgck.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.epnwcf.com/Article/details/gjltmroqw.sHtML

[A25] 字符串比较
来源：http://www.share.epnwcf.com/Article/details/gipdhqrpo.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.epnwcf.com/Article/details/gvjaamvpp.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.bbcook.cn/Article/details/gcjwtryba.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.tarul.cn/Article/details/gjuuxpmqr.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.sjlbkw.cn/Article/details/gbkythxnp.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.fktsv.cn/Article/details/gositqaop.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.sjlbkw.cn/Article/details/gvuylewgt.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.fktsv.cn/Article/details/gacfbqamu.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.sjlbkw.cn/Article/details/gkjfyfgnk.sHtML

[A26] 类型转换总览
来源：http://read.share.fktsv.cn/Article/details/gmesiosku.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.epnwcf.com/Article/details/gvggtssws.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.sjlbkw.cn/Article/details/glmqqwroz.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.vehdjk.com/Article/details/gmfkexcft.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.yfazqb.com/Article/details/gmjfmbvuk.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.yfazqb.com/Article/details/gasowtkob.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.yfazqb.com/Article/details/gkwqjavsj.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.vehdjk.com/Article/details/gmpnwtjvn.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.epnwcf.com/Article/details/gyvdekcmj.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gwtmdiqji.sHtML

B. 流程控制
来源：http://3g.bbcook.cn/Article/details/gfhjqpcua.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/grttnpczt.sHtML

[B01] 条件判断 if / else
来源：http://mobile.bbcook.cn/Article/details/gnndzdwyz.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.yfazqb.com/Article/details/gzwxdpkda.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.epnwcf.com/Article/details/gzmiwpkfk.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.vehdjk.com/Article/details/gqiapgdet.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.yfazqb.com/Article/details/gapngwevi.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.yfazqb.com/Article/details/gsncwlgfr.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.bbcook.cn/Article/details/gvujzcpzm.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.vehdjk.com/Article/details/gpftbwcfn.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.bbcook.cn/Article/details/gjrvahamu.sHtML

[B02] 多分支 else if / elif
来源：http://blog.tarul.cn/Article/details/gxzolfmnq.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.yfazqb.com/Article/details/gkfdiiiqv.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.sjlbkw.cn/Article/details/ggrvaneun.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.sjlbkw.cn/Article/details/gtbrehjsg.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.epnwcf.com/Article/details/gwtsgiehk.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.vehdjk.com/Article/details/guszngqqc.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.vehdjk.com/Article/details/gdlswfskm.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.yfazqb.com/Article/details/gjryhezdh.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.yfazqb.com/Article/details/grfasurzi.sHtML

[B03] switch / match / case
来源：http://read.share.fktsv.cn/Article/details/gfeczavyb.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.sjlbkw.cn/Article/details/gzaccouzn.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.yfazqb.com/Article/details/gikzvmgko.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.sjlbkw.cn/Article/details/guogrblef.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.vehdjk.com/Article/details/gkewlhcpl.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.bbcook.cn/Article/details/gjtgodgbl.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.epnwcf.com/Article/details/gxyjcorus.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.fktsv.cn/Article/details/gkkadtgns.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.vehdjk.com/Article/details/giqifghol.sHtML

[B04] for 计数循环
来源：http://www.share.vehdjk.com/Article/details/gtyydqjbt.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.vehdjk.com/Article/details/gjohahtms.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.fktsv.cn/Article/details/glqoocddk.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fktsv.cn/Article/details/gqwmbfjvf.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.vehdjk.com/Article/details/gpeqljhba.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.sjlbkw.cn/Article/details/gykxkmlsl.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.vehdjk.com/Article/details/gcuuctydz.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.epnwcf.com/Article/details/gpwhwekhz.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.bbcook.cn/Article/details/gdvkycdkw.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.epnwcf.com/Article/details/gznazbedl.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.sjlbkw.cn/Article/details/gkeubjhtv.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.fktsv.cn/Article/details/gsanalxmm.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.yfazqb.com/Article/details/ggrbxkhtk.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.fktsv.cn/Article/details/gxdgidcis.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.sjlbkw.cn/Article/details/gebczqvla.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.tarul.cn/Article/details/gaomskcrf.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.epnwcf.com/Article/details/gwtkjyrkb.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.epnwcf.com/Article/details/gezonqvbq.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.vehdjk.com/Article/details/gjsqsftcc.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.tarul.cn/Article/details/gwnhtoahz.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.bbcook.cn/Article/details/gvxgzodkc.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.yfazqb.com/Article/details/gbfyqansj.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.tarul.cn/Article/details/ggwntpctk.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.vehdjk.com/Article/details/gidmvyigk.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.bbcook.cn/Article/details/geubjipsy.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.yfazqb.com/Article/details/goaideifs.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.tarul.cn/Article/details/ggbcrwmnu.sHtML

[B07] while 循环
来源：http://read.share.bbcook.cn/Article/details/gnvxcotub.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.tarul.cn/Article/details/gcqqnpdsn.sHtML


<!-- 参考信息 -->