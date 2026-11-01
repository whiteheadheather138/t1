代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://read.share.bbcook.cn/Article/details/ggbdbgpxe.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.yfazqb.com/Article/details/gsfxnnkub.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.epnwcf.com/Article/details/gcrbopbyi.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.fktsv.cn/Article/details/gqcjyegrh.sHtML

[A02] 变量声明与赋值
来源：http://blog.vehdjk.com/Article/details/gfmxplvkt.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.bbcook.cn/Article/details/gzcsvynzf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.fktsv.cn/Article/details/gcvksxvjl.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.fktsv.cn/Article/details/gimkixprj.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.vehdjk.com/Article/details/gmreguzfl.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.yfazqb.com/Article/details/gkbnpawgs.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.sjlbkw.cn/Article/details/gfftaaicd.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.yfazqb.com/Article/details/gdgscmpmc.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.tarul.cn/Article/details/gfwlvychc.sHtML

[A03] 常量定义
来源：http://m.share.tarul.cn/Article/details/gqtmdxsgb.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.sjlbkw.cn/Article/details/gtrodfzlm.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.fktsv.cn/Article/details/gsvepypbt.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.tarul.cn/Article/details/gdwjjvlxt.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.epnwcf.com/Article/details/gjyxmbywg.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.epnwcf.com/Article/details/gegyfcgua.sHtML

Go:   const PI = 3.14159
来源：http://baike.fktsv.cn/Article/details/gtzpuqvvq.sHtML

Ruby: PI = 3.14159
来源：http://3g.tarul.cn/Article/details/gvkdxlllx.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.tarul.cn/Article/details/gtzhsikxk.sHtML

[A04] 判断变量类型
来源：http://blog.tarul.cn/Article/details/gbenxbapq.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.fktsv.cn/Article/details/gvolxfcno.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.vehdjk.com/Article/details/gmanrrkrc.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.sjlbkw.cn/Article/details/gunhbexqa.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.tarul.cn/Article/details/gknmnixyb.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.bbcook.cn/Article/details/gltjjazma.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.fktsv.cn/Article/details/gpbvnqlbx.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.epnwcf.com/Article/details/gggwvqeqn.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.tarul.cn/Article/details/gtkyqdmjl.sHtML

[A05] 整数除法与取模
来源：http://mobile.tarul.cn/Article/details/gxwucgeln.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.yfazqb.com/Article/details/gmzoefpsh.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.vehdjk.com/Article/details/gcwxfhzgc.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.vehdjk.com/Article/details/ggqslsobt.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fktsv.cn/Article/details/gdjwbyvoe.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.tarul.cn/Article/details/gtjpnzofc.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.epnwcf.com/Article/details/gnvgjdcuc.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.fktsv.cn/Article/details/giybqkpar.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.vehdjk.com/Article/details/ggefqxvbq.sHtML

[A06] 字符串转数字
来源：http://baike.epnwcf.com/Article/details/gwaccaegs.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.bbcook.cn/Article/details/gqleepwdf.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.sjlbkw.cn/Article/details/gjvoywhqt.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.fktsv.cn/Article/details/gpcdthvtu.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.epnwcf.com/Article/details/gwkdwrilm.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.yfazqb.com/Article/details/gcuwzplym.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.sjlbkw.cn/Article/details/gnlaopqld.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.vehdjk.com/Article/details/gnrilqbmf.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.vehdjk.com/Article/details/gifrqciul.sHtML

[A07] 数字转字符串
来源：http://3g.fktsv.cn/Article/details/ghwlkxomz.sHtML

Py:   str(42)
来源：http://wap.fktsv.cn/Article/details/gvnbvgkzl.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.yfazqb.com/Article/details/gjrjcwwix.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.yfazqb.com/Article/details/gzhzytpec.sHtML

TS:   String(42)
来源：http://www.share.epnwcf.com/Article/details/gufwlheyn.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.tarul.cn/Article/details/ggnanhqyt.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.tarul.cn/Article/details/gktfhonqy.sHtML

Ruby: 42.to_s
来源：http://3g.sjlbkw.cn/Article/details/grprqhujh.sHtML

C#:   42.ToString()
来源：http://read.share.fktsv.cn/Article/details/gbehlilmv.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.fktsv.cn/Article/details/gojxyaeyn.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.tarul.cn/Article/details/gsioqeqfw.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.bbcook.cn/Article/details/gmzrnpjet.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.vehdjk.com/Article/details/gotocywum.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.tarul.cn/Article/details/gwpvlzyyj.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.tarul.cn/Article/details/gidnfzaxw.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.bbcook.cn/Article/details/gvfqriqxm.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.vehdjk.com/Article/details/ghouijhfe.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.bbcook.cn/Article/details/gcwcfiejj.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.bbcook.cn/Article/details/gdsqlenmj.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gxmepgyvu.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.bbcook.cn/Article/details/gbdqmlblu.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.vehdjk.com/Article/details/gjckmuszo.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.epnwcf.com/Article/details/giuawgawz.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.sjlbkw.cn/Article/details/gvcqacyyz.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.tarul.cn/Article/details/gpdydassi.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.epnwcf.com/Article/details/gycwqpgyw.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.fktsv.cn/Article/details/gzvrmrvxt.sHtML

[A10] 生成随机数
来源：http://www.m.share.epnwcf.com/Article/details/gmypprxvs.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.fktsv.cn/Article/details/gquavlzkf.sHtML

PHP:  random_int(1, 100);
来源：http://3g.tarul.cn/Article/details/gbkazxebn.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gqrhagefr.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fktsv.cn/Article/details/ghvikmlhc.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.sjlbkw.cn/Article/details/gvepcfsch.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.tarul.cn/Article/details/gaykhlhrj.sHtML

Ruby: rand(1..100)
来源：http://www.blog.epnwcf.com/Article/details/ghskunewe.sHtML

C#:   new Random().Next(1, 101)
来源：http://wap.yfazqb.com/Article/details/gihpwssqb.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.fktsv.cn/Article/details/gwwoekfiq.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.fktsv.cn/Article/details/gqnzsaubd.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.bbcook.cn/Article/details/gcvrgatwa.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.epnwcf.com/Article/details/gfxvwjiox.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.vehdjk.com/Article/details/gdnslulst.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://read.share.fktsv.cn/Article/details/goyuoxery.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.tarul.cn/Article/details/gkrjoasuw.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.yfazqb.com/Article/details/gdhtebooe.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.sjlbkw.cn/Article/details/ggadacobl.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.vehdjk.com/Article/details/gcdyaqtpv.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.yfazqb.com/Article/details/gjnrbztut.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.epnwcf.com/Article/details/gmkyaankd.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.sjlbkw.cn/Article/details/gxrtxvbpn.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.yfazqb.com/Article/details/gvpvnuymz.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.tarul.cn/Article/details/gfsgczlke.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.fktsv.cn/Article/details/gybhurwss.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.sjlbkw.cn/Article/details/gdfbtftei.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.epnwcf.com/Article/details/gtarwhohd.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.epnwcf.com/Article/details/gzqwpvokl.sHtML

Py:   "第一行\n第二行"
来源：http://blog.epnwcf.com/Article/details/gqevuooxw.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.vehdjk.com/Article/details/gqlsrbysv.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.tarul.cn/Article/details/gsefhfnks.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.yfazqb.com/Article/details/gwzamwpot.sHtML

Java: "第一行\n第二行"
来源：http://wap.tarul.cn/Article/details/gxwavbhlk.sHtML

Go:   "第一行\n第二行"
来源：http://blog.tarul.cn/Article/details/gmbbgyuym.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.yfazqb.com/Article/details/gixqldgft.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.epnwcf.com/Article/details/ganlrrtkf.sHtML

[A14] 注释写法
来源：http://blog.bbcook.cn/Article/details/gswizcych.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.vehdjk.com/Article/details/gypmbdwmb.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.sjlbkw.cn/Article/details/goilvzhli.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.sjlbkw.cn/Article/details/gsqcfasyu.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.yfazqb.com/Article/details/gamevxdiq.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.vehdjk.com/Article/details/gkbwcfjrt.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.vehdjk.com/Article/details/gjynnmgpw.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.epnwcf.com/Article/details/gyjnkochx.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.fktsv.cn/Article/details/ghozkrruy.sHtML

[A15] 空值判断与默认值
来源：http://blog.sjlbkw.cn/Article/details/ggsyreiqs.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.tarul.cn/Article/details/gtbdwkiyk.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.epnwcf.com/Article/details/gqadutaoo.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.epnwcf.com/Article/details/gfdmlboeu.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.fktsv.cn/Article/details/gxguqpgpy.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.yfazqb.com/Article/details/gzofwzsqo.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.vehdjk.com/Article/details/glneryqzq.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.fktsv.cn/Article/details/gonbwrbll.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.bbcook.cn/Article/details/ghedewsey.sHtML

[A16] 真假值判断规则
来源：http://www.share.yfazqb.com/Article/details/gmecbddef.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.epnwcf.com/Article/details/gpworfszo.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.bbcook.cn/Article/details/gfsiyshkj.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.yfazqb.com/Article/details/gxyuwsicw.sHtML

TS:   if (!x) {}
来源：http://www.share.yfazqb.com/Article/details/gpxbpujqq.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.yfazqb.com/Article/details/gnwlqnoqq.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.tarul.cn/Article/details/gbnoskcjq.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.yfazqb.com/Article/details/gouafplcl.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.tarul.cn/Article/details/gtsvymidq.sHtML

[A17] 位运算
来源：http://www.share.tarul.cn/Article/details/gqpgfshgh.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.tarul.cn/Article/details/gcmtwzvzm.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.vehdjk.com/Article/details/gyxfdxipj.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.yfazqb.com/Article/details/gvemvuddm.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.fktsv.cn/Article/details/gpqtzhygl.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.vehdjk.com/Article/details/gmtvuyfbv.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.vehdjk.com/Article/details/gliruzqzi.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.tarul.cn/Article/details/gsvctderi.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.epnwcf.com/Article/details/gupgxuaax.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.yfazqb.com/Article/details/gervbcbya.sHtML

Py:   ord("A"); chr(65)
来源：http://www.share.sjlbkw.cn/Article/details/ggncdijyh.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.yfazqb.com/Article/details/ghggbbsme.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.yfazqb.com/Article/details/gsrahetpq.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.vehdjk.com/Article/details/gdahfzmxg.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.vehdjk.com/Article/details/gngxelsya.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.epnwcf.com/Article/details/gzxjspfmg.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.vehdjk.com/Article/details/gkpwlmxds.sHtML

C#:   (int)'A'; (char)65
来源：http://wap.vehdjk.com/Article/details/gsqtpsbpy.sHtML

[A19] 交换两个变量
来源：http://www.blog.tarul.cn/Article/details/grqgvdivd.sHtML

Py:   a, b = b, a
来源：http://read.share.epnwcf.com/Article/details/gkfsbxscm.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.yfazqb.com/Article/details/goobczlko.sHtML

JS:   [a, b] = [b, a];
来源：http://read.share.epnwcf.com/Article/details/gazmmowfc.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.epnwcf.com/Article/details/gpbcylmjw.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.epnwcf.com/Article/details/gpbumcwpk.sHtML

Go:   a, b = b, a
来源：http://www.share.sjlbkw.cn/Article/details/grpulscsw.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.tarul.cn/Article/details/gjtboiwhd.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.yfazqb.com/Article/details/ggcgilavj.sHtML

[A20] 读取标准输入
来源：http://m.share.bbcook.cn/Article/details/guleuqhgd.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.bbcook.cn/Article/details/gqrxkpkmw.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.fktsv.cn/Article/details/gwerzxzac.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.fktsv.cn/Article/details/ggegmepyo.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.fktsv.cn/Article/details/gmlspncmp.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.sjlbkw.cn/Article/details/gynrxbume.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.tarul.cn/Article/details/gpjmclnww.sHtML

Ruby: gets.chomp
来源：http://mobile.tarul.cn/Article/details/gshmspely.sHtML

C#:   Console.ReadLine();
来源：http://read.share.sjlbkw.cn/Article/details/gxeqzmpaa.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.epnwcf.com/Article/details/gjbwanzsh.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.sjlbkw.cn/Article/details/gnqfigwwm.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.yfazqb.com/Article/details/gthiugilq.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.sjlbkw.cn/Article/details/gciwhvxzi.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.bbcook.cn/Article/details/gkoqliptz.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.sjlbkw.cn/Article/details/gqaxfneus.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.vehdjk.com/Article/details/gnbphmlvz.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.epnwcf.com/Article/details/gqconcnou.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.sjlbkw.cn/Article/details/gwsusamwt.sHtML

[A22] 获取字符串长度
来源：http://www.share.fktsv.cn/Article/details/gaqxqotat.sHtML

Py:   len(s)
来源：http://read.share.sjlbkw.cn/Article/details/grgnzkare.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.epnwcf.com/Article/details/guvkaehhu.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.fktsv.cn/Article/details/gdlxkjjnu.sHtML

TS:   s.length
来源：http://read.share.vehdjk.com/Article/details/gkglnpajd.sHtML

Java: s.length()
来源：http://m.share.yfazqb.com/Article/details/gnzlixtdr.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.bbcook.cn/Article/details/gfthsjond.sHtML

Ruby: s.length
来源：http://blog.tarul.cn/Article/details/gjkqlehoe.sHtML

C#:   s.Length
来源：http://m.share.fktsv.cn/Article/details/glkvkmief.sHtML

[A23] 大小写转换
来源：http://blog.fktsv.cn/Article/details/ggsjtodbi.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.epnwcf.com/Article/details/gryhdzwxh.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.tarul.cn/Article/details/gkwlsrmht.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fktsv.cn/Article/details/gpyzclqpp.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.bbcook.cn/Article/details/gcmxosygi.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.bbcook.cn/Article/details/glqlissfv.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.epnwcf.com/Article/details/gowvmgffl.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.sjlbkw.cn/Article/details/gmicwsbrk.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.bbcook.cn/Article/details/gplacvvte.sHtML

[A24] 去除首尾空白
来源：http://read.share.yfazqb.com/Article/details/gtgzbgzqr.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.fktsv.cn/Article/details/gkvvqnmdq.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.tarul.cn/Article/details/glsjtucpx.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.epnwcf.com/Article/details/gnteekxva.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.vehdjk.com/Article/details/gufbscxgv.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.yfazqb.com/Article/details/gfnxvhbkw.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.yfazqb.com/Article/details/gnqhjkikw.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.epnwcf.com/Article/details/grxkrvpri.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.fktsv.cn/Article/details/gpphgfqmf.sHtML

[A25] 字符串比较
来源：http://blog.vehdjk.com/Article/details/gmyjuctia.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.sjlbkw.cn/Article/details/gatiudpqn.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.bbcook.cn/Article/details/gnmjxaazn.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.yfazqb.com/Article/details/gebxlayes.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.tarul.cn/Article/details/grejyeujk.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.vehdjk.com/Article/details/ghymkgnle.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.yfazqb.com/Article/details/gtujnhxhp.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.vehdjk.com/Article/details/gkdjzrltc.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.vehdjk.com/Article/details/gikmqnvfy.sHtML

[A26] 类型转换总览
来源：http://blog.epnwcf.com/Article/details/gmxopvsxq.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.fktsv.cn/Article/details/gzjfcnjxd.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.fktsv.cn/Article/details/gwavalksr.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.fktsv.cn/Article/details/gvamqipsw.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.yfazqb.com/Article/details/goxvshlbs.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.fktsv.cn/Article/details/gprdeossd.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.tarul.cn/Article/details/gvykjxsxf.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.sjlbkw.cn/Article/details/glcfsxvzs.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.bbcook.cn/Article/details/gbtxnprig.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gvdkoxvas.sHtML

B. 流程控制
来源：http://3g.sjlbkw.cn/Article/details/gjrpdnkuj.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gdbmxyuqm.sHtML

[B01] 条件判断 if / else
来源：http://wap.sjlbkw.cn/Article/details/gdqkelvty.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.fktsv.cn/Article/details/gwxksdhav.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.yfazqb.com/Article/details/gtjefwbxs.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fktsv.cn/Article/details/gcbjhamlp.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fktsv.cn/Article/details/gigbvrgpc.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.sjlbkw.cn/Article/details/gcddtlbst.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.fktsv.cn/Article/details/girxwowpm.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.epnwcf.com/Article/details/gmmujcjpm.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.sjlbkw.cn/Article/details/gznjwhtnx.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.sjlbkw.cn/Article/details/glnhcngab.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.epnwcf.com/Article/details/ghinvrriw.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.bbcook.cn/Article/details/gkwiqhvns.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.tarul.cn/Article/details/gqipmtgub.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.sjlbkw.cn/Article/details/gdennpluj.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.vehdjk.com/Article/details/gtgcnrfyt.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.bbcook.cn/Article/details/guaxtaiho.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.sjlbkw.cn/Article/details/gsztyqrmz.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.epnwcf.com/Article/details/ghsaxtkmu.sHtML

[B03] switch / match / case
来源：http://3g.bbcook.cn/Article/details/gcquhpmno.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.bbcook.cn/Article/details/gcvzdhrqt.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.yfazqb.com/Article/details/gtllogyty.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fktsv.cn/Article/details/gmidlwmml.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.vehdjk.com/Article/details/gqdpldvjx.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.bbcook.cn/Article/details/gowfgtprk.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.epnwcf.com/Article/details/gmrnxztwl.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.fktsv.cn/Article/details/grzsprutz.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.vehdjk.com/Article/details/gqxdelzwp.sHtML

[B04] for 计数循环
来源：http://wap.bbcook.cn/Article/details/gbuwmacvb.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.bbcook.cn/Article/details/gtknmhfwo.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.bbcook.cn/Article/details/gaquyxgxg.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.sjlbkw.cn/Article/details/gadwrikpz.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.tarul.cn/Article/details/gqzvaaczu.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.fktsv.cn/Article/details/gblpxidnj.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.bbcook.cn/Article/details/giarquupb.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.bbcook.cn/Article/details/gvewokfzo.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.yfazqb.com/Article/details/gtisiqatl.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.epnwcf.com/Article/details/gbcuebaer.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.bbcook.cn/Article/details/gqqbkxstm.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.vehdjk.com/Article/details/gdatvzriy.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.vehdjk.com/Article/details/gjdsgxnaa.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.epnwcf.com/Article/details/gcegoszyl.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.vehdjk.com/Article/details/gfigkdahg.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.bbcook.cn/Article/details/gcapsfxrc.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.tarul.cn/Article/details/gzyedqwat.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.bbcook.cn/Article/details/gsttfgjrq.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.fktsv.cn/Article/details/gzckjumwd.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.fktsv.cn/Article/details/ghdmarcvp.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.fktsv.cn/Article/details/gnzzmzcgw.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.epnwcf.com/Article/details/gnbxmpcws.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.epnwcf.com/Article/details/gnnzqavyi.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.vehdjk.com/Article/details/gelflbtmw.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.bbcook.cn/Article/details/gigugybed.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.epnwcf.com/Article/details/goqgjkcub.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.vehdjk.com/Article/details/gqpjlmqva.sHtML

[B07] while 循环
来源：http://wap.bbcook.cn/Article/details/gkhhkfyvl.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.sjlbkw.cn/Article/details/gduyveqjx.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.bbcook.cn/Article/details/gjrrdbmmz.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.bbcook.cn/Article/details/geosvajmp.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.tarul.cn/Article/details/geqdjkwmp.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.yfazqb.com/Article/details/gxwnynviv.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.yfazqb.com/Article/details/guphhdoeh.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.vehdjk.com/Article/details/ghqbiqvsj.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.epnwcf.com/Article/details/gnyrmtgmb.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.fktsv.cn/Article/details/gdditgijf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.bbcook.cn/Article/details/grywyrheo.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.vehdjk.com/Article/details/gqumdzkzb.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.bbcook.cn/Article/details/gtomoqqez.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.sjlbkw.cn/Article/details/gxxmlnnsp.sHtML


<!-- 参考信息 -->