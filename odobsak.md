代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.epnwcf.com/Article/details/gvzxpjrho.sHtML

[A03] 常量定义
来源：http://3g.vehdjk.com/Article/details/gxbnzbykq.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.yfazqb.com/Article/details/gvkskkdse.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.bbcook.cn/Article/details/gkczufogx.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/ggufqkund.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.epnwcf.com/Article/details/gmqrpaqwc.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.tarul.cn/Article/details/gmxxhawcx.sHtML

Go:   const PI = 3.14159
来源：http://read.share.sjlbkw.cn/Article/details/gpergwzpw.sHtML

Ruby: PI = 3.14159
来源：http://baike.epnwcf.com/Article/details/glaenkbyr.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.tarul.cn/Article/details/gwxeakswt.sHtML

[A04] 判断变量类型
来源：http://mobile.vehdjk.com/Article/details/gzyrnefxu.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.yfazqb.com/Article/details/gwzxdhyga.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.bbcook.cn/Article/details/gifswhmmh.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.yfazqb.com/Article/details/ghtxglryk.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.tarul.cn/Article/details/giybrfnlq.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.epnwcf.com/Article/details/gexkudpdq.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.epnwcf.com/Article/details/goaxaanwg.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.tarul.cn/Article/details/glzegqjmw.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.sjlbkw.cn/Article/details/gzwxfvcbc.sHtML

[A05] 整数除法与取模
来源：http://m.share.vehdjk.com/Article/details/gjxzcuwls.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.yfazqb.com/Article/details/gpegjpnpk.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.fktsv.cn/Article/details/ggwvofilj.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.bbcook.cn/Article/details/gtgshiknh.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.sjlbkw.cn/Article/details/gkwqfurdn.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.vehdjk.com/Article/details/gvzyedtqo.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.yfazqb.com/Article/details/gwcdylnin.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.epnwcf.com/Article/details/gyjclojhm.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.vehdjk.com/Article/details/gkcrhdpzr.sHtML

[A06] 字符串转数字
来源：http://wap.fktsv.cn/Article/details/gnfrsdfdf.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.tarul.cn/Article/details/grbkesiux.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.fktsv.cn/Article/details/gqpfxxdxr.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.vehdjk.com/Article/details/ggsbdhydy.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.vehdjk.com/Article/details/ghigmeasp.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.tarul.cn/Article/details/gcjvanspb.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.fktsv.cn/Article/details/ggidbtcyq.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.tarul.cn/Article/details/gjapuedgg.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.vehdjk.com/Article/details/gmmfijzkc.sHtML

[A07] 数字转字符串
来源：http://blog.vehdjk.com/Article/details/gtcgmxcvd.sHtML

Py:   str(42)
来源：http://3g.tarul.cn/Article/details/gzldtjzkl.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.yfazqb.com/Article/details/gchzudkfi.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.vehdjk.com/Article/details/gizmiacce.sHtML

TS:   String(42)
来源：http://read.share.yfazqb.com/Article/details/geqfoqfrb.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.sjlbkw.cn/Article/details/giovfhuze.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.tarul.cn/Article/details/gzlsyvjqz.sHtML

Ruby: 42.to_s
来源：http://www.m.share.epnwcf.com/Article/details/gdvqidklf.sHtML

C#:   42.ToString()
来源：http://www.m.share.epnwcf.com/Article/details/gexsuqyzi.sHtML

[A08] 取整与四舍五入
来源：http://m.share.vehdjk.com/Article/details/gmgwnavta.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.bbcook.cn/Article/details/gcieghcve.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.yfazqb.com/Article/details/gavyfjsfv.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.vehdjk.com/Article/details/gfblapzxc.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.epnwcf.com/Article/details/gnubmsooq.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.yfazqb.com/Article/details/gmrxhskxi.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.vehdjk.com/Article/details/gbxtamaex.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.bbcook.cn/Article/details/gxbphltxe.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.bbcook.cn/Article/details/gndutyspk.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.sjlbkw.cn/Article/details/guaoaryot.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.vehdjk.com/Article/details/gxmlyvvhm.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/ggmmhvzby.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.sjlbkw.cn/Article/details/gaaqfvptc.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.epnwcf.com/Article/details/gupejurub.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.yfazqb.com/Article/details/gdjtctbzp.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.epnwcf.com/Article/details/gcorpklwf.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.fktsv.cn/Article/details/gfhqevohf.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.sjlbkw.cn/Article/details/gnzlzdxjv.sHtML

[A10] 生成随机数
来源：http://m.share.bbcook.cn/Article/details/gaqzrbkij.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.sjlbkw.cn/Article/details/gazdlaubw.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.sjlbkw.cn/Article/details/gmyaaccry.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.bbcook.cn/Article/details/ghimhhpcc.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.bbcook.cn/Article/details/gpzopfcua.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.bbcook.cn/Article/details/girhgxfay.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.sjlbkw.cn/Article/details/gugidahkq.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.sjlbkw.cn/Article/details/giblsmnrd.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.vehdjk.com/Article/details/gakwpbiaj.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.fktsv.cn/Article/details/gbtcuolce.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.epnwcf.com/Article/details/gcvwqclzb.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.bbcook.cn/Article/details/gexwikbcp.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.vehdjk.com/Article/details/gkarzylup.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.sjlbkw.cn/Article/details/gwbkhqhbz.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.epnwcf.com/Article/details/gloynbwix.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.vehdjk.com/Article/details/gogliffmg.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.epnwcf.com/Article/details/gjrkmogpy.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.epnwcf.com/Article/details/gohiamzbg.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.vehdjk.com/Article/details/gdyoggbsx.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.tarul.cn/Article/details/gmnoozzfq.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.fktsv.cn/Article/details/gghvdhnzw.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.vehdjk.com/Article/details/gquivzrcl.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.epnwcf.com/Article/details/gsohydidp.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.vehdjk.com/Article/details/gspdhpmeu.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.vehdjk.com/Article/details/gdnaqhohg.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.vehdjk.com/Article/details/gyowuqjnx.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.sjlbkw.cn/Article/details/gpuzauksi.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.fktsv.cn/Article/details/gncioftzr.sHtML

Py:   "第一行\n第二行"
来源：http://wap.fktsv.cn/Article/details/guokhqaib.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.epnwcf.com/Article/details/ggoiptwng.sHtML

JS:   "第一行\n第二行"
来源：http://wap.vehdjk.com/Article/details/gztdnzzpe.sHtML

TS:   "第一行\n第二行"
来源：http://blog.bbcook.cn/Article/details/gnokqcehc.sHtML

Java: "第一行\n第二行"
来源：http://blog.epnwcf.com/Article/details/gszpeoalh.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.tarul.cn/Article/details/gqhzynsxw.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.vehdjk.com/Article/details/gdjubxpfv.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.epnwcf.com/Article/details/gcegxsaqf.sHtML

[A14] 注释写法
来源：http://read.share.sjlbkw.cn/Article/details/gwniwdxbd.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.tarul.cn/Article/details/gguhiqbkm.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.tarul.cn/Article/details/gsrffhpht.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.vehdjk.com/Article/details/gkrmqbtmf.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.vehdjk.com/Article/details/gwushsoeh.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.fktsv.cn/Article/details/gcvorkbid.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.fktsv.cn/Article/details/gftpajtgw.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.tarul.cn/Article/details/gbfwzmlea.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.tarul.cn/Article/details/gltmbpbcw.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.tarul.cn/Article/details/geuzqcezy.sHtML

Py:   value = data or "默认值"
来源：http://baike.yfazqb.com/Article/details/glpmmsduu.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.bbcook.cn/Article/details/gntwvvpfo.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.epnwcf.com/Article/details/gtptwgekz.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.vehdjk.com/Article/details/gbmnwfced.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.fktsv.cn/Article/details/gpufoxggb.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.fktsv.cn/Article/details/goedyntrl.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.tarul.cn/Article/details/gdiawocdk.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.yfazqb.com/Article/details/gmbgtddtp.sHtML

[A16] 真假值判断规则
来源：http://read.share.vehdjk.com/Article/details/ghhpnzqic.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.fktsv.cn/Article/details/giryfjcux.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.epnwcf.com/Article/details/grufdnfwa.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.yfazqb.com/Article/details/gongxwulb.sHtML

TS:   if (!x) {}
来源：http://www.m.share.fktsv.cn/Article/details/gmoxkhxbi.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.tarul.cn/Article/details/gztqekzmf.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.sjlbkw.cn/Article/details/gtaklosac.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.sjlbkw.cn/Article/details/gfxzasmod.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.vehdjk.com/Article/details/goeqgtfpy.sHtML

[A17] 位运算
来源：http://m.share.fktsv.cn/Article/details/gowtcnbsj.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fktsv.cn/Article/details/gfvzjpjob.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.bbcook.cn/Article/details/gfjfhojld.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.bbcook.cn/Article/details/ginludozv.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.yfazqb.com/Article/details/gjfjvskvw.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.epnwcf.com/Article/details/gukkzqkon.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.sjlbkw.cn/Article/details/gevlmfnxp.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.bbcook.cn/Article/details/gegctflbf.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.sjlbkw.cn/Article/details/gxkcpqenj.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.vehdjk.com/Article/details/guvwrszeg.sHtML

Py:   ord("A"); chr(65)
来源：http://www.share.fktsv.cn/Article/details/gkjxukgrl.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.sjlbkw.cn/Article/details/gprzznlmf.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.vehdjk.com/Article/details/gzsoqvgld.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.epnwcf.com/Article/details/gdxlfnolr.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.sjlbkw.cn/Article/details/ggxxysxma.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.yfazqb.com/Article/details/gfjiwrtko.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.vehdjk.com/Article/details/gfkzdebtm.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.yfazqb.com/Article/details/gnqfrolex.sHtML

[A19] 交换两个变量
来源：http://baike.bbcook.cn/Article/details/ghopquzxi.sHtML

Py:   a, b = b, a
来源：http://3g.bbcook.cn/Article/details/ggfcbowje.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.tarul.cn/Article/details/ggmucldpk.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.fktsv.cn/Article/details/giqpvjdbg.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.tarul.cn/Article/details/gezdtksnp.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.sjlbkw.cn/Article/details/gdakablzu.sHtML

Go:   a, b = b, a
来源：http://3g.tarul.cn/Article/details/ghcvuwogo.sHtML

Ruby: a, b = b, a
来源：http://blog.epnwcf.com/Article/details/gidebmfbb.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.tarul.cn/Article/details/gickrtruj.sHtML

[A20] 读取标准输入
来源：http://baike.epnwcf.com/Article/details/gafntchfi.sHtML

Py:   name = input("请输入：")
来源：http://mobile.epnwcf.com/Article/details/guzqvodqw.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.bbcook.cn/Article/details/gjjaoedrm.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.epnwcf.com/Article/details/gjepsaslt.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.fktsv.cn/Article/details/gztifxryi.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.fktsv.cn/Article/details/gcxouzpvs.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.epnwcf.com/Article/details/gzkfglwyf.sHtML

Ruby: gets.chomp
来源：http://wap.yfazqb.com/Article/details/gcvrdjezj.sHtML

C#:   Console.ReadLine();
来源：http://m.share.vehdjk.com/Article/details/gnrlwteki.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.fktsv.cn/Article/details/giihapbuy.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.vehdjk.com/Article/details/gzrbcfnni.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.sjlbkw.cn/Article/details/gpqtvozrb.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.epnwcf.com/Article/details/gfdpcpzab.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.vehdjk.com/Article/details/gfzexfnle.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.vehdjk.com/Article/details/gzvbkkebc.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.fktsv.cn/Article/details/gphaqobed.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.tarul.cn/Article/details/gmyyznggz.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.fktsv.cn/Article/details/gyorroqbz.sHtML

[A22] 获取字符串长度
来源：http://baike.yfazqb.com/Article/details/ggcqkhybz.sHtML

Py:   len(s)
来源：http://3g.fktsv.cn/Article/details/gxzcnleup.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.bbcook.cn/Article/details/gxizwxryw.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.bbcook.cn/Article/details/gwdgitmwt.sHtML

TS:   s.length
来源：http://www.m.share.fktsv.cn/Article/details/gszfppqnz.sHtML

Java: s.length()
来源：http://baike.yfazqb.com/Article/details/gyjwzmcxn.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.yfazqb.com/Article/details/ggbhayhim.sHtML

Ruby: s.length
来源：http://mobile.yfazqb.com/Article/details/gwfbxvnqb.sHtML

C#:   s.Length
来源：http://m.share.epnwcf.com/Article/details/grvlrwspd.sHtML

[A23] 大小写转换
来源：http://m.share.vehdjk.com/Article/details/ggkxwfqts.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.bbcook.cn/Article/details/gmoyxgaxj.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.bbcook.cn/Article/details/gokrraskp.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fktsv.cn/Article/details/gaoidfmta.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.tarul.cn/Article/details/gclzkhqmd.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.sjlbkw.cn/Article/details/gbbdupdpc.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.epnwcf.com/Article/details/gwznljmkb.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.epnwcf.com/Article/details/gfhvyporj.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.sjlbkw.cn/Article/details/gbkkkyvlb.sHtML

[A24] 去除首尾空白
来源：http://mobile.yfazqb.com/Article/details/ghdgndlzx.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.epnwcf.com/Article/details/gyqbwhqer.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.fktsv.cn/Article/details/gohfywwhx.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.tarul.cn/Article/details/gfukctrmf.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.vehdjk.com/Article/details/gmqmprmkz.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.tarul.cn/Article/details/glhrrzfuy.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.tarul.cn/Article/details/gqyqkeygy.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.sjlbkw.cn/Article/details/gszipqyhy.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.bbcook.cn/Article/details/genxulani.sHtML

[A25] 字符串比较
来源：http://wap.tarul.cn/Article/details/ghsiuspyo.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.sjlbkw.cn/Article/details/gntczmzoa.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.yfazqb.com/Article/details/gyfdfkdnb.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.bbcook.cn/Article/details/gfzmqbekc.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.fktsv.cn/Article/details/gltdscqxr.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.vehdjk.com/Article/details/giduybbve.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.epnwcf.com/Article/details/gftbrykqw.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.fktsv.cn/Article/details/gsmolsrvb.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.vehdjk.com/Article/details/gzququdiu.sHtML

[A26] 类型转换总览
来源：http://m.share.vehdjk.com/Article/details/gdbykmcbj.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.vehdjk.com/Article/details/gshcvjcda.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.bbcook.cn/Article/details/gwrulmbfl.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.bbcook.cn/Article/details/gjlinqfdn.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.yfazqb.com/Article/details/gnublpfrq.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.yfazqb.com/Article/details/gpaprgbwl.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.bbcook.cn/Article/details/gouwauzli.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.sjlbkw.cn/Article/details/grrzbehbf.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.tarul.cn/Article/details/gtrnxxjob.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/ggdhtmpsq.sHtML

B. 流程控制
来源：http://wap.fktsv.cn/Article/details/gjsibonmz.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gwgxdlems.sHtML

[B01] 条件判断 if / else
来源：http://wap.fktsv.cn/Article/details/ggdezuntg.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.yfazqb.com/Article/details/gfvvcbrtl.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.vehdjk.com/Article/details/giexfcbnj.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.epnwcf.com/Article/details/gduesnknj.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.vehdjk.com/Article/details/gmbtnkaga.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.fktsv.cn/Article/details/gigdvoizm.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.bbcook.cn/Article/details/gbhounnvm.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.epnwcf.com/Article/details/gxwoizskv.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.bbcook.cn/Article/details/gazwwmjed.sHtML

[B02] 多分支 else if / elif
来源：http://wap.vehdjk.com/Article/details/gmvpwatqj.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.fktsv.cn/Article/details/gjttyvlzz.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.sjlbkw.cn/Article/details/grstqlhms.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.sjlbkw.cn/Article/details/gaanuuysb.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.sjlbkw.cn/Article/details/gtdoswqao.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.sjlbkw.cn/Article/details/gkujznzec.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.epnwcf.com/Article/details/ggmflgqoa.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.sjlbkw.cn/Article/details/ggzbmvhek.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.yfazqb.com/Article/details/gboadfjxy.sHtML

[B03] switch / match / case
来源：http://m.share.sjlbkw.cn/Article/details/gvpzeycvm.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.vehdjk.com/Article/details/gsgpoelus.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.vehdjk.com/Article/details/glbfqzwgz.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.vehdjk.com/Article/details/giwphnrhz.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.sjlbkw.cn/Article/details/gquabilxg.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.yfazqb.com/Article/details/gupmipdrc.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.sjlbkw.cn/Article/details/glinvmvsa.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.yfazqb.com/Article/details/gafapniwb.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.sjlbkw.cn/Article/details/gzuqjmjjc.sHtML

[B04] for 计数循环
来源：http://m.share.yfazqb.com/Article/details/gvrdlwaac.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.fktsv.cn/Article/details/gwwvkjctz.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.vehdjk.com/Article/details/gzgrkxnmc.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.epnwcf.com/Article/details/gbvzztdan.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.sjlbkw.cn/Article/details/gnwvaysdt.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.vehdjk.com/Article/details/grrjkygcc.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.vehdjk.com/Article/details/gydiibzao.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.tarul.cn/Article/details/gjpucffdc.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.epnwcf.com/Article/details/gcttmwara.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.yfazqb.com/Article/details/gvslykkfm.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.sjlbkw.cn/Article/details/gnzcmpfrd.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.sjlbkw.cn/Article/details/gisrstrpu.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.tarul.cn/Article/details/gmwjhiruf.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.bbcook.cn/Article/details/gmilkibig.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.yfazqb.com/Article/details/guusppeyq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.tarul.cn/Article/details/ghdwzpkcx.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.sjlbkw.cn/Article/details/ganbkaqjd.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.tarul.cn/Article/details/givqphpjx.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.vehdjk.com/Article/details/gxmzllmko.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.vehdjk.com/Article/details/gxkgyvbmz.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.tarul.cn/Article/details/gnncjaroe.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.vehdjk.com/Article/details/gjqypwpqn.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.tarul.cn/Article/details/gdcieyqsc.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.vehdjk.com/Article/details/gwvwwgata.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.yfazqb.com/Article/details/gpiutyddk.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.epnwcf.com/Article/details/gflevkxpz.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.bbcook.cn/Article/details/gffclapgb.sHtML

[B07] while 循环
来源：http://www.blog.yfazqb.com/Article/details/gnojjfsad.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.epnwcf.com/Article/details/gbtwevkzr.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.yfazqb.com/Article/details/gljrbnpbx.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.yfazqb.com/Article/details/gmktpxxlu.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.yfazqb.com/Article/details/gyjajoesb.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.bbcook.cn/Article/details/gaixsjnoo.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.sjlbkw.cn/Article/details/gqvnhcags.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.tarul.cn/Article/details/gafkyflqt.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.epnwcf.com/Article/details/ggbyznbzk.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.bbcook.cn/Article/details/gfcesmcij.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.sjlbkw.cn/Article/details/ghxldbozg.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.yfazqb.com/Article/details/gtgazvqyy.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.vehdjk.com/Article/details/gmkupmpbe.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.tarul.cn/Article/details/gvleamium.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.fktsv.cn/Article/details/guynuclnq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.vehdjk.com/Article/details/ggulfnufc.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.bbcook.cn/Article/details/gizxjptap.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.tarul.cn/Article/details/gdyiliwgu.sHtML

[B09] break 与 continue
来源：http://blog.yfazqb.com/Article/details/gqhwyouqp.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.tarul.cn/Article/details/gukqaxniw.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.epnwcf.com/Article/details/gokwpjgek.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fktsv.cn/Article/details/geikoqgws.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.sjlbkw.cn/Article/details/ghwvqeess.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.epnwcf.com/Article/details/gctvjeusd.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.vehdjk.com/Article/details/gqikvgwwm.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.tarul.cn/Article/details/gkluxjczr.sHtML


<!-- 参考信息 -->