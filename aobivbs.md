代发 wailian999

[A02] 变量声明与赋值
来源：http://mobile.fktsv.cn/Article/details/gyawnsknb.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.tarul.cn/Article/details/gyjorbfdl.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.epnwcf.com/Article/details/gwdxhpxas.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.bbcook.cn/Article/details/gnlpdxjpo.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.bbcook.cn/Article/details/gaoqcapjf.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.bbcook.cn/Article/details/gejqsxcmm.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.yfazqb.com/Article/details/gfqgdceuo.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.bbcook.cn/Article/details/gfqyiygkh.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.bbcook.cn/Article/details/gszonwogl.sHtML

[A03] 常量定义
来源：http://3g.tarul.cn/Article/details/gbninsdrr.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.vehdjk.com/Article/details/gikonsdji.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.epnwcf.com/Article/details/gflfxcirs.sHtML

JS:   const PI = 3.14159;
来源：http://baike.epnwcf.com/Article/details/guuhqkred.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.fktsv.cn/Article/details/gvqabmnvn.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.bbcook.cn/Article/details/gtxfjotgn.sHtML

Go:   const PI = 3.14159
来源：http://read.share.yfazqb.com/Article/details/gfghydvbc.sHtML

Ruby: PI = 3.14159
来源：http://wap.tarul.cn/Article/details/gysybgnyl.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/ggjashuan.sHtML

[A04] 判断变量类型
来源：http://www.blog.bbcook.cn/Article/details/gknkffbed.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.tarul.cn/Article/details/gnsaqnknk.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.fktsv.cn/Article/details/gukgrkyxi.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.vehdjk.com/Article/details/gjaryarms.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.sjlbkw.cn/Article/details/gitsgkeej.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.bbcook.cn/Article/details/goillyucf.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.tarul.cn/Article/details/ghalxsxra.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.vehdjk.com/Article/details/gtajgtxgv.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.yfazqb.com/Article/details/gcnxuzobz.sHtML

[A05] 整数除法与取模
来源：http://mobile.bbcook.cn/Article/details/giuxefzod.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.tarul.cn/Article/details/gtsogjwwa.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.yfazqb.com/Article/details/grnplnvog.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.yfazqb.com/Article/details/gfnssunsp.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.vehdjk.com/Article/details/gcaiuchag.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.bbcook.cn/Article/details/gnbuaqbws.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.vehdjk.com/Article/details/gurdnxmfg.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.tarul.cn/Article/details/gvnenewhd.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.fktsv.cn/Article/details/gjidycdfg.sHtML

[A06] 字符串转数字
来源：http://www.m.share.yfazqb.com/Article/details/gehxphvzo.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.yfazqb.com/Article/details/gusdoyevx.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.tarul.cn/Article/details/gpbmskjhj.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.bbcook.cn/Article/details/ggkkqfqcn.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.vehdjk.com/Article/details/gvuapidrh.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.tarul.cn/Article/details/gvmgjmaps.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.yfazqb.com/Article/details/grwtftwet.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.sjlbkw.cn/Article/details/gphabisbs.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.bbcook.cn/Article/details/gylimhymp.sHtML

[A07] 数字转字符串
来源：http://read.share.bbcook.cn/Article/details/gfefzlipy.sHtML

Py:   str(42)
来源：http://mobile.fktsv.cn/Article/details/gmmwzrcme.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.epnwcf.com/Article/details/gjpcyvsom.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.fktsv.cn/Article/details/gllfxzxqo.sHtML

TS:   String(42)
来源：http://3g.tarul.cn/Article/details/gyceyayda.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.vehdjk.com/Article/details/gfkwcpoqb.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.vehdjk.com/Article/details/glhjvcvot.sHtML

Ruby: 42.to_s
来源：http://www.m.share.epnwcf.com/Article/details/gpbiengpc.sHtML

C#:   42.ToString()
来源：http://3g.tarul.cn/Article/details/gqwqwttpx.sHtML

[A08] 取整与四舍五入
来源：http://3g.fktsv.cn/Article/details/gksmykioc.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.bbcook.cn/Article/details/gjttztkpg.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.tarul.cn/Article/details/glppccehw.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.tarul.cn/Article/details/gxgildqyh.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.fktsv.cn/Article/details/grwhgosjl.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.tarul.cn/Article/details/gewcehjvc.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.vehdjk.com/Article/details/gsjxnxycb.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.sjlbkw.cn/Article/details/guteqqfcc.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.yfazqb.com/Article/details/guusknwfq.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.yfazqb.com/Article/details/gacbqxyxx.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.yfazqb.com/Article/details/gxwwtuptx.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fktsv.cn/Article/details/ghaiwmpbb.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.bbcook.cn/Article/details/gzapamiep.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.epnwcf.com/Article/details/gozznxmjg.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.epnwcf.com/Article/details/ghpbbvosm.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.fktsv.cn/Article/details/gzxdgwsft.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.yfazqb.com/Article/details/gzegfhgis.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.epnwcf.com/Article/details/gamsngenh.sHtML

[A10] 生成随机数
来源：http://m.share.epnwcf.com/Article/details/gcaqpzyqz.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.sjlbkw.cn/Article/details/grzbiciov.sHtML

PHP:  random_int(1, 100);
来源：http://baike.tarul.cn/Article/details/gmkebzkyn.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.epnwcf.com/Article/details/genwrxpzx.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.tarul.cn/Article/details/gvcwvhnyp.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.bbcook.cn/Article/details/gfvuqasvy.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.fktsv.cn/Article/details/geviexmmh.sHtML

Ruby: rand(1..100)
来源：http://blog.bbcook.cn/Article/details/gdhrmjqcd.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.tarul.cn/Article/details/gmeqartkv.sHtML

[A11] 条件表达式（三元）
来源：http://baike.vehdjk.com/Article/details/gtyvtyrba.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.bbcook.cn/Article/details/gjqjscxuv.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.yfazqb.com/Article/details/gxnlibldb.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.tarul.cn/Article/details/ggitgtbak.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.tarul.cn/Article/details/gljtsdcdp.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.yfazqb.com/Article/details/gxrgmveop.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.epnwcf.com/Article/details/gwkislxaz.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.bbcook.cn/Article/details/gzxccrqjo.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.epnwcf.com/Article/details/gtcmfvoir.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.fktsv.cn/Article/details/gwusnhwen.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.yfazqb.com/Article/details/gmxozxmvx.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.sjlbkw.cn/Article/details/gkdowyubf.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.fktsv.cn/Article/details/gqqmosmys.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.tarul.cn/Article/details/gumnyivhd.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.vehdjk.com/Article/details/glwrzaaqr.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.vehdjk.com/Article/details/gpypsefwe.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.epnwcf.com/Article/details/gsbxointl.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.epnwcf.com/Article/details/gzrafxibi.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.sjlbkw.cn/Article/details/gdfaddlqd.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.sjlbkw.cn/Article/details/gqzgyakww.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.bbcook.cn/Article/details/gryonqxlw.sHtML

JS:   "第一行\n第二行"
来源：http://3g.epnwcf.com/Article/details/grrybbrsa.sHtML

TS:   "第一行\n第二行"
来源：http://www.blog.yfazqb.com/Article/details/gnztutxzp.sHtML

Java: "第一行\n第二行"
来源：http://mobile.epnwcf.com/Article/details/gcuaxpxgz.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.vehdjk.com/Article/details/gimvdkjdt.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.fktsv.cn/Article/details/glsztaedb.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.fktsv.cn/Article/details/gnkdkbmbm.sHtML

[A14] 注释写法
来源：http://www.m.share.yfazqb.com/Article/details/gcyvyelyh.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.sjlbkw.cn/Article/details/gyucfriru.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.epnwcf.com/Article/details/gkdxqyzdc.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.epnwcf.com/Article/details/ggpfxmkei.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.tarul.cn/Article/details/gfprslbqt.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.fktsv.cn/Article/details/gxtmbholh.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.fktsv.cn/Article/details/ghwamgjfw.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.epnwcf.com/Article/details/gnfuprtje.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.epnwcf.com/Article/details/gxdztoinj.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.vehdjk.com/Article/details/gctghtzwt.sHtML

Py:   value = data or "默认值"
来源：http://read.share.vehdjk.com/Article/details/gsbvrduek.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.sjlbkw.cn/Article/details/gvffbelks.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.bbcook.cn/Article/details/gtoraawyz.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.sjlbkw.cn/Article/details/glxyeafld.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.tarul.cn/Article/details/gvtmaakfx.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.epnwcf.com/Article/details/gnzxmqgkd.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.vehdjk.com/Article/details/guyccchuf.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.fktsv.cn/Article/details/gbfuldjhj.sHtML

[A16] 真假值判断规则
来源：http://wap.fktsv.cn/Article/details/gcupqmjan.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.vehdjk.com/Article/details/golwbztwz.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.vehdjk.com/Article/details/gjvdkdhmw.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.epnwcf.com/Article/details/gqaraooxi.sHtML

TS:   if (!x) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gqujqjbgr.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.sjlbkw.cn/Article/details/gllmekiye.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.tarul.cn/Article/details/gxtcqgsgo.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.tarul.cn/Article/details/gofnpokfb.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.bbcook.cn/Article/details/glpwqeodt.sHtML

[A17] 位运算
来源：http://www.share.fktsv.cn/Article/details/gxkntwust.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.sjlbkw.cn/Article/details/gjanmmnta.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.sjlbkw.cn/Article/details/gmxdowccu.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.tarul.cn/Article/details/gsmtdsewr.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.sjlbkw.cn/Article/details/gmkdkxtpv.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.bbcook.cn/Article/details/gtxiacfrm.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.yfazqb.com/Article/details/geobuesvi.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fktsv.cn/Article/details/gtvpwceuu.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.sjlbkw.cn/Article/details/gncdxzxnl.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.bbcook.cn/Article/details/glaphtevn.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjwuoozey.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.fktsv.cn/Article/details/gjkxuglby.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.sjlbkw.cn/Article/details/ghxcfsaob.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.bbcook.cn/Article/details/gkykocmnw.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.tarul.cn/Article/details/gorgahjvi.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.bbcook.cn/Article/details/ggciozrnu.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.bbcook.cn/Article/details/gjmjcxqhe.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.sjlbkw.cn/Article/details/gzmiestzp.sHtML

[A19] 交换两个变量
来源：http://read.share.tarul.cn/Article/details/gemzsvebq.sHtML

Py:   a, b = b, a
来源：http://www.m.share.vehdjk.com/Article/details/gbuclqucp.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.vehdjk.com/Article/details/ghamfuliu.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.yfazqb.com/Article/details/gbdzvqpfq.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.vehdjk.com/Article/details/goamphnxn.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.yfazqb.com/Article/details/gbqacacdu.sHtML

Go:   a, b = b, a
来源：http://www.blog.sjlbkw.cn/Article/details/gcfltodjp.sHtML

Ruby: a, b = b, a
来源：http://3g.fktsv.cn/Article/details/gvkiyobkp.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.sjlbkw.cn/Article/details/gmdwpkjrl.sHtML

[A20] 读取标准输入
来源：http://wap.bbcook.cn/Article/details/gjjahwczx.sHtML

Py:   name = input("请输入：")
来源：http://wap.yfazqb.com/Article/details/gqvrtlcoe.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.bbcook.cn/Article/details/geobkzwpe.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.yfazqb.com/Article/details/gfsjdgsge.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.vehdjk.com/Article/details/gxkuuqqnx.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.vehdjk.com/Article/details/ghweydoew.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.sjlbkw.cn/Article/details/gimrhsypd.sHtML

Ruby: gets.chomp
来源：http://3g.tarul.cn/Article/details/guhhwkfwl.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.sjlbkw.cn/Article/details/gyboxggwi.sHtML

[A21] 保留指定小数位输出
来源：http://blog.fktsv.cn/Article/details/gvolbwtxa.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.bbcook.cn/Article/details/ggyvconpb.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.epnwcf.com/Article/details/goqjqrsjk.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.tarul.cn/Article/details/gmmovuagu.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.vehdjk.com/Article/details/gusogffvp.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.fktsv.cn/Article/details/gevjdjpgu.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.tarul.cn/Article/details/gimjhydpg.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.yfazqb.com/Article/details/gxpajpvcd.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.bbcook.cn/Article/details/gokxnipgk.sHtML

[A22] 获取字符串长度
来源：http://www.share.sjlbkw.cn/Article/details/guctluxwb.sHtML

Py:   len(s)
来源：http://www.blog.tarul.cn/Article/details/gutfertho.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.epnwcf.com/Article/details/gcpusvtsb.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.bbcook.cn/Article/details/gqypvjbfg.sHtML

TS:   s.length
来源：http://baike.tarul.cn/Article/details/gezrrrgip.sHtML

Java: s.length()
来源：http://3g.tarul.cn/Article/details/gptlagkil.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.sjlbkw.cn/Article/details/gsmqphoal.sHtML

Ruby: s.length
来源：http://m.share.sjlbkw.cn/Article/details/gypxeitdk.sHtML

C#:   s.Length
来源：http://3g.yfazqb.com/Article/details/gkuvojuue.sHtML

[A23] 大小写转换
来源：http://mobile.tarul.cn/Article/details/gtahuetnw.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.epnwcf.com/Article/details/girhrwoja.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.tarul.cn/Article/details/gjgazfgwo.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.bbcook.cn/Article/details/gqdhvpdlq.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.sjlbkw.cn/Article/details/gthmugpqe.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.epnwcf.com/Article/details/gdaqdtnaa.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.bbcook.cn/Article/details/gdjxborto.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.sjlbkw.cn/Article/details/gmrghwtlz.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.tarul.cn/Article/details/gllvkkxug.sHtML

[A24] 去除首尾空白
来源：http://www.share.tarul.cn/Article/details/gynnamjpx.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.epnwcf.com/Article/details/gerimudah.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.sjlbkw.cn/Article/details/goturbzah.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.sjlbkw.cn/Article/details/gnfdlxkvh.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.yfazqb.com/Article/details/gbaukegfa.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.sjlbkw.cn/Article/details/gzcybvioi.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.vehdjk.com/Article/details/gaxxfqfjh.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.epnwcf.com/Article/details/gzykajwqa.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.bbcook.cn/Article/details/gpbmycpup.sHtML

[A25] 字符串比较
来源：http://wap.sjlbkw.cn/Article/details/gvhxlfkej.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.bbcook.cn/Article/details/gfebxvtky.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.bbcook.cn/Article/details/gnfzynsgr.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.vehdjk.com/Article/details/gbbqmlvjg.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.yfazqb.com/Article/details/grcorujnt.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.fktsv.cn/Article/details/gsgzkbiqr.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.tarul.cn/Article/details/gduemnvfn.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.bbcook.cn/Article/details/gkbpqxnyz.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.fktsv.cn/Article/details/gdaimomtr.sHtML

[A26] 类型转换总览
来源：http://m.share.tarul.cn/Article/details/gslmjrgok.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.epnwcf.com/Article/details/gaweilner.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.sjlbkw.cn/Article/details/gqrarlqpf.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.vehdjk.com/Article/details/goziyfzjo.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.epnwcf.com/Article/details/gvpxmdqml.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.yfazqb.com/Article/details/gzizbdgpw.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.yfazqb.com/Article/details/gkjkeiode.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.yfazqb.com/Article/details/gageqtymt.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.yfazqb.com/Article/details/gjbvlmivl.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gelpgqzex.sHtML

B. 流程控制
来源：http://wap.bbcook.cn/Article/details/gwwrmqueo.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gnvaokubr.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.bbcook.cn/Article/details/gvcoxjgkx.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.sjlbkw.cn/Article/details/gmijoncmv.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.epnwcf.com/Article/details/gulvldugx.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.epnwcf.com/Article/details/gwrqnryli.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fktsv.cn/Article/details/gdhmgytli.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.sjlbkw.cn/Article/details/gahdaetbs.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.sjlbkw.cn/Article/details/guffrojug.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.vehdjk.com/Article/details/gfjrglsxi.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.tarul.cn/Article/details/gcdtbipzo.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.yfazqb.com/Article/details/ggxogfgfk.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.yfazqb.com/Article/details/gvvtbfith.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.sjlbkw.cn/Article/details/gzeeyvmqi.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.epnwcf.com/Article/details/gsaaebrte.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.vehdjk.com/Article/details/gedzqgpau.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.vehdjk.com/Article/details/gwgpggtbr.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.yfazqb.com/Article/details/gmpzuhvde.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.sjlbkw.cn/Article/details/gkbjpdobf.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.vehdjk.com/Article/details/gcmklkxuf.sHtML

[B03] switch / match / case
来源：http://blog.tarul.cn/Article/details/gcieaxxhj.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.tarul.cn/Article/details/ggucnaldi.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.vehdjk.com/Article/details/gnhxsfyfj.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.sjlbkw.cn/Article/details/gnuwgvscq.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.vehdjk.com/Article/details/gqhuakfgr.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.yfazqb.com/Article/details/gpuuljrtm.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.fktsv.cn/Article/details/gdyecjulb.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.epnwcf.com/Article/details/gbexuellp.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.tarul.cn/Article/details/glrriohhr.sHtML

[B04] for 计数循环
来源：http://3g.sjlbkw.cn/Article/details/gesxsdvtr.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.sjlbkw.cn/Article/details/gubuldjae.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.vehdjk.com/Article/details/gmqyiggfs.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.sjlbkw.cn/Article/details/gpspogubl.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.sjlbkw.cn/Article/details/gkaenwreh.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.yfazqb.com/Article/details/gxapgcfdh.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.sjlbkw.cn/Article/details/guyqdwgvt.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.sjlbkw.cn/Article/details/gshcrkgyo.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.sjlbkw.cn/Article/details/gvbctzehx.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.yfazqb.com/Article/details/gjqpejhit.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.fktsv.cn/Article/details/gyvpyhfoe.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.tarul.cn/Article/details/gnbinvfph.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.tarul.cn/Article/details/gchlygdge.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fktsv.cn/Article/details/gevzimpat.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.epnwcf.com/Article/details/gqfishhhp.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.epnwcf.com/Article/details/gzgrebsfg.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.yfazqb.com/Article/details/gexppjpoo.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.bbcook.cn/Article/details/gqthmeweu.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.sjlbkw.cn/Article/details/gsazpqihp.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.yfazqb.com/Article/details/guuypzqmj.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.epnwcf.com/Article/details/gbpioipdf.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.epnwcf.com/Article/details/gpplrmosm.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.epnwcf.com/Article/details/gipjofyip.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.fktsv.cn/Article/details/gkfzzeobp.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.fktsv.cn/Article/details/gisokpzke.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.sjlbkw.cn/Article/details/gkiffjknc.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.yfazqb.com/Article/details/giexiaxqw.sHtML

[B07] while 循环
来源：http://wap.yfazqb.com/Article/details/gjsepxvkq.sHtML

Py:   while i < 10: i += 1
来源：http://wap.yfazqb.com/Article/details/gcpffolqr.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.fktsv.cn/Article/details/gjoombjzo.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.fktsv.cn/Article/details/gdypbmrms.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.sjlbkw.cn/Article/details/ggjccbval.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.sjlbkw.cn/Article/details/geycrfmhw.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.epnwcf.com/Article/details/gdnfqxnuq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.fktsv.cn/Article/details/gttwvfgra.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.fktsv.cn/Article/details/gcblhcgcm.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.yfazqb.com/Article/details/gupbrgacx.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.yfazqb.com/Article/details/ghlxvxywm.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.vehdjk.com/Article/details/gebdikqlk.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.yfazqb.com/Article/details/gppvqmbte.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.tarul.cn/Article/details/gvzoadkom.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.yfazqb.com/Article/details/gxaapabqg.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.tarul.cn/Article/details/gcodflieb.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.epnwcf.com/Article/details/gmpmharaq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.tarul.cn/Article/details/gijpkgybf.sHtML


<!-- 参考信息 -->