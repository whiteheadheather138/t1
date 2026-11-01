代发 wailian999

JS:   const PI = 3.14159;
来源：http://wap.vehdjk.com/Article/details/ghmqitvdc.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.bbcook.cn/Article/details/gbmytinpf.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.fktsv.cn/Article/details/gnvjkcfqh.sHtML

Go:   const PI = 3.14159
来源：http://m.share.bbcook.cn/Article/details/gqmepwcrh.sHtML

Ruby: PI = 3.14159
来源：http://blog.tarul.cn/Article/details/gxhdzuebx.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.yfazqb.com/Article/details/gixsguovq.sHtML

[A04] 判断变量类型
来源：http://www.m.share.yfazqb.com/Article/details/guxcjffxr.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.bbcook.cn/Article/details/gmnbdkorr.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.epnwcf.com/Article/details/grmpxlfsa.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.yfazqb.com/Article/details/gqpcjgxzj.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.fktsv.cn/Article/details/gqyrsdvcs.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.fktsv.cn/Article/details/gjoixgepb.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.bbcook.cn/Article/details/gphatqrnh.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.tarul.cn/Article/details/gnpxptgse.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.tarul.cn/Article/details/gmtssxlhh.sHtML

[A05] 整数除法与取模
来源：http://www.blog.epnwcf.com/Article/details/goyuyoeuy.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.tarul.cn/Article/details/gjaxbzkix.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.yfazqb.com/Article/details/gbrfaigcj.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.yfazqb.com/Article/details/gaptvlpan.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.yfazqb.com/Article/details/gcphhqxrm.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.epnwcf.com/Article/details/gsvwhiemn.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.tarul.cn/Article/details/gpzjtqpvo.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.bbcook.cn/Article/details/gzpvkkbwr.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.sjlbkw.cn/Article/details/gmylvzeog.sHtML

[A06] 字符串转数字
来源：http://m.share.tarul.cn/Article/details/gjyvhiuvl.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.bbcook.cn/Article/details/gxawwcuid.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.yfazqb.com/Article/details/ghqmcswrb.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.vehdjk.com/Article/details/gygwelgpt.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.yfazqb.com/Article/details/gpdvxhknj.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.epnwcf.com/Article/details/gzfmtwtau.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.tarul.cn/Article/details/gerqdleji.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.fktsv.cn/Article/details/gagvgxcqs.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.bbcook.cn/Article/details/gzgiytcem.sHtML

[A07] 数字转字符串
来源：http://www.share.vehdjk.com/Article/details/guhyohiii.sHtML

Py:   str(42)
来源：http://m.share.sjlbkw.cn/Article/details/gjbiihaxo.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.fktsv.cn/Article/details/gqdpgtakk.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.tarul.cn/Article/details/gsiihnyqj.sHtML

TS:   String(42)
来源：http://3g.yfazqb.com/Article/details/guweabudx.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.fktsv.cn/Article/details/grkngakwl.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.fktsv.cn/Article/details/gbohbxocb.sHtML

Ruby: 42.to_s
来源：http://www.m.share.sjlbkw.cn/Article/details/guheijwjg.sHtML

C#:   42.ToString()
来源：http://wap.yfazqb.com/Article/details/gowfprebh.sHtML

[A08] 取整与四舍五入
来源：http://baike.yfazqb.com/Article/details/gddlqpgiz.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.bbcook.cn/Article/details/gthfevzwx.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.sjlbkw.cn/Article/details/gebciymdo.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.epnwcf.com/Article/details/ggbjiyqeu.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.fktsv.cn/Article/details/gqpeuxuvc.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.tarul.cn/Article/details/goxrcruxe.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.yfazqb.com/Article/details/gdthcowjm.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.tarul.cn/Article/details/gqkntmcfn.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.tarul.cn/Article/details/goferofxy.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.yfazqb.com/Article/details/ggzcoppvb.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.yfazqb.com/Article/details/glgyoqddp.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.vehdjk.com/Article/details/glulcfeof.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.tarul.cn/Article/details/gmutzbtum.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.vehdjk.com/Article/details/gynvoasoc.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.bbcook.cn/Article/details/gmtbaidzs.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.fktsv.cn/Article/details/gpsnsqicn.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.tarul.cn/Article/details/gnhepeqsq.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.yfazqb.com/Article/details/gvsdapddx.sHtML

[A10] 生成随机数
来源：http://www.m.share.yfazqb.com/Article/details/gyzetswpe.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.fktsv.cn/Article/details/gexapgcff.sHtML

PHP:  random_int(1, 100);
来源：http://3g.fktsv.cn/Article/details/gtamjwppf.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.tarul.cn/Article/details/gpbgpmwtr.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.vehdjk.com/Article/details/gqbswcubq.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.fktsv.cn/Article/details/gfsqhayvr.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.fktsv.cn/Article/details/gktatxmuq.sHtML

Ruby: rand(1..100)
来源：http://wap.bbcook.cn/Article/details/gkuxjoduz.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.bbcook.cn/Article/details/gsqgiahgc.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.tarul.cn/Article/details/gymkidajf.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.tarul.cn/Article/details/gkycqduqv.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.vehdjk.com/Article/details/gdsefhcvj.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.fktsv.cn/Article/details/gkrhmzeym.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.fktsv.cn/Article/details/gfxpaiktf.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.sjlbkw.cn/Article/details/giestnmre.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.epnwcf.com/Article/details/ghgwrzfse.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.sjlbkw.cn/Article/details/gbclssqdw.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.vehdjk.com/Article/details/gfhlemelm.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.vehdjk.com/Article/details/ghijwbdmg.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.yfazqb.com/Article/details/gjxbznrws.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.tarul.cn/Article/details/gplfjmpew.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.fktsv.cn/Article/details/gehkwntht.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.yfazqb.com/Article/details/gmcdxdmfe.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.sjlbkw.cn/Article/details/grumbjtdk.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.bbcook.cn/Article/details/gwicqlfiu.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.fktsv.cn/Article/details/gnhywagdj.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.sjlbkw.cn/Article/details/gynbcfjwr.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.tarul.cn/Article/details/gcgaacwkw.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.sjlbkw.cn/Article/details/gdzsmvhuy.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.fktsv.cn/Article/details/gdeafvahg.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.yfazqb.com/Article/details/gknxsafrk.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.vehdjk.com/Article/details/gghrhwchx.sHtML

Java: "第一行\n第二行"
来源：http://read.share.vehdjk.com/Article/details/giofaiweo.sHtML

Go:   "第一行\n第二行"
来源：http://baike.sjlbkw.cn/Article/details/gxdqudssw.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.bbcook.cn/Article/details/gyahgqegt.sHtML

C#:   "第一行\n第二行"
来源：http://3g.sjlbkw.cn/Article/details/glvwkvadh.sHtML

[A14] 注释写法
来源：http://mobile.vehdjk.com/Article/details/ghwpsxclz.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.fktsv.cn/Article/details/gmggchptt.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.sjlbkw.cn/Article/details/gglnkeric.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.sjlbkw.cn/Article/details/gwjblphvt.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.fktsv.cn/Article/details/gcxbbvrqs.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.sjlbkw.cn/Article/details/ggchyfpqf.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.yfazqb.com/Article/details/gobstijte.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.vehdjk.com/Article/details/gkcfkwiaz.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.bbcook.cn/Article/details/gulaxcdhc.sHtML

[A15] 空值判断与默认值
来源：http://blog.yfazqb.com/Article/details/gbxjbtqmq.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.sjlbkw.cn/Article/details/gpcihsyvl.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.sjlbkw.cn/Article/details/gkhfjjdir.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.sjlbkw.cn/Article/details/gnurzgtfa.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.bbcook.cn/Article/details/gptckznxb.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://read.share.yfazqb.com/Article/details/gojbnebbj.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.bbcook.cn/Article/details/glinjqxtn.sHtML

Ruby: value = data || "默认值"
来源：http://baike.fktsv.cn/Article/details/gltvmyddi.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.sjlbkw.cn/Article/details/gcxsadydf.sHtML

[A16] 真假值判断规则
来源：http://3g.fktsv.cn/Article/details/gpbkaofpk.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.tarul.cn/Article/details/gjegdvyek.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.vehdjk.com/Article/details/gkphllaed.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.fktsv.cn/Article/details/gmyyotvvv.sHtML

TS:   if (!x) {}
来源：http://baike.bbcook.cn/Article/details/gonwkwggk.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.sjlbkw.cn/Article/details/gzvyynmfp.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.fktsv.cn/Article/details/goxijdzip.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.epnwcf.com/Article/details/gqwquwaqu.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.fktsv.cn/Article/details/givnzpdst.sHtML

[A17] 位运算
来源：http://m.share.sjlbkw.cn/Article/details/gxywropau.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.vehdjk.com/Article/details/gvjaxmdym.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.yfazqb.com/Article/details/gzsusofdr.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.vehdjk.com/Article/details/gwsyqugmi.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.epnwcf.com/Article/details/gpwzrahpv.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.tarul.cn/Article/details/gtncpnnhl.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.fktsv.cn/Article/details/gjsygfrtv.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.sjlbkw.cn/Article/details/gizskdzmw.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fktsv.cn/Article/details/glfrjbddu.sHtML

[A18] 字符与 ASCII 码互转
来源：http://blog.bbcook.cn/Article/details/gtigqrejq.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.sjlbkw.cn/Article/details/gcxuenlvb.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.yfazqb.com/Article/details/gbmbshfnh.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.fktsv.cn/Article/details/geqixqfeu.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.fktsv.cn/Article/details/gtsrvoqyi.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.vehdjk.com/Article/details/gokkmplga.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.epnwcf.com/Article/details/gkualokas.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.epnwcf.com/Article/details/grxnqbtwe.sHtML

C#:   (int)'A'; (char)65
来源：http://wap.sjlbkw.cn/Article/details/gnkasicxv.sHtML

[A19] 交换两个变量
来源：http://www.m.share.epnwcf.com/Article/details/gjwlsloue.sHtML

Py:   a, b = b, a
来源：http://www.m.share.fktsv.cn/Article/details/gebvdpegt.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.vehdjk.com/Article/details/gzepknbio.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.vehdjk.com/Article/details/gnpcghetq.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.fktsv.cn/Article/details/gtyepsdre.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.tarul.cn/Article/details/gckemqjdt.sHtML

Go:   a, b = b, a
来源：http://www.blog.tarul.cn/Article/details/gapjaekra.sHtML

Ruby: a, b = b, a
来源：http://baike.fktsv.cn/Article/details/gvnmyacep.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.sjlbkw.cn/Article/details/gjtczxjbc.sHtML

[A20] 读取标准输入
来源：http://www.blog.vehdjk.com/Article/details/gijziflnq.sHtML

Py:   name = input("请输入：")
来源：http://www.share.fktsv.cn/Article/details/gjcikwobe.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.vehdjk.com/Article/details/glehnuauj.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.fktsv.cn/Article/details/gbvyumots.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.fktsv.cn/Article/details/gjksthonw.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.yfazqb.com/Article/details/ggekgstoq.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.epnwcf.com/Article/details/grogcqtzo.sHtML

Ruby: gets.chomp
来源：http://www.blog.bbcook.cn/Article/details/gmymccoka.sHtML

C#:   Console.ReadLine();
来源：http://mobile.tarul.cn/Article/details/gbmutkoio.sHtML

[A21] 保留指定小数位输出
来源：http://blog.bbcook.cn/Article/details/gcaxfouio.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.vehdjk.com/Article/details/giafjbvhk.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.fktsv.cn/Article/details/gzzuugmdg.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.bbcook.cn/Article/details/gngmbvmgi.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.tarul.cn/Article/details/giwaqjqqa.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.epnwcf.com/Article/details/gyzscwtxd.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.tarul.cn/Article/details/ghvncfxzi.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.epnwcf.com/Article/details/gzxelhhkf.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.fktsv.cn/Article/details/gyixjeatf.sHtML

[A22] 获取字符串长度
来源：http://blog.fktsv.cn/Article/details/gteigxsbk.sHtML

Py:   len(s)
来源：http://www.m.share.epnwcf.com/Article/details/gvpofzxij.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.epnwcf.com/Article/details/ggrmmshbo.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.fktsv.cn/Article/details/glnolukle.sHtML

TS:   s.length
来源：http://baike.yfazqb.com/Article/details/gzynpbtaa.sHtML

Java: s.length()
来源：http://m.share.fktsv.cn/Article/details/gwuleyjsc.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.tarul.cn/Article/details/gppjwyqsu.sHtML

Ruby: s.length
来源：http://baike.vehdjk.com/Article/details/gienpgiwu.sHtML

C#:   s.Length
来源：http://m.share.vehdjk.com/Article/details/gfolbvabb.sHtML

[A23] 大小写转换
来源：http://www.blog.sjlbkw.cn/Article/details/gfaltcaja.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.epnwcf.com/Article/details/gohxkqhks.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.fktsv.cn/Article/details/glgdwbbvc.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.epnwcf.com/Article/details/gcvppuaab.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.bbcook.cn/Article/details/gsvfgfeih.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.vehdjk.com/Article/details/gfnminxma.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.yfazqb.com/Article/details/gjarsfsbv.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.fktsv.cn/Article/details/gcywtstcz.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.epnwcf.com/Article/details/gxcppwpyu.sHtML

[A24] 去除首尾空白
来源：http://www.blog.fktsv.cn/Article/details/gjabgvlge.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.yfazqb.com/Article/details/gyhgbqlsg.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.fktsv.cn/Article/details/geaphlzmf.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.bbcook.cn/Article/details/gafhwzmxf.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.tarul.cn/Article/details/gdykppmjp.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.yfazqb.com/Article/details/gxeeqxfrk.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.epnwcf.com/Article/details/gokmzlikk.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.yfazqb.com/Article/details/gfqqxqlcx.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.epnwcf.com/Article/details/gyvqlecbk.sHtML

[A25] 字符串比较
来源：http://m.share.tarul.cn/Article/details/gtjipgaje.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.epnwcf.com/Article/details/gqhsqoedm.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.vehdjk.com/Article/details/gstuxxzek.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.yfazqb.com/Article/details/goxopceuu.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.tarul.cn/Article/details/gluaazjco.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.epnwcf.com/Article/details/gdnmkmltx.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.sjlbkw.cn/Article/details/gdcbtxspa.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.yfazqb.com/Article/details/ggmvrighw.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.bbcook.cn/Article/details/gdreeehre.sHtML

[A26] 类型转换总览
来源：http://wap.sjlbkw.cn/Article/details/gkgrleefh.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.vehdjk.com/Article/details/gtylfowon.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.epnwcf.com/Article/details/gcxxbinyf.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.tarul.cn/Article/details/gkgmwtspd.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.vehdjk.com/Article/details/gpscvonxr.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.sjlbkw.cn/Article/details/goitfyeqr.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.epnwcf.com/Article/details/gqhzkmmxp.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.yfazqb.com/Article/details/gfrkkegch.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.tarul.cn/Article/details/gxplydooc.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gxwmcasrj.sHtML

B. 流程控制
来源：http://m.share.bbcook.cn/Article/details/guamuouwu.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gbusfmzca.sHtML

[B01] 条件判断 if / else
来源：http://read.share.sjlbkw.cn/Article/details/gqnxbkvgq.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.sjlbkw.cn/Article/details/glpifeqld.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.sjlbkw.cn/Article/details/gvmmyimax.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.sjlbkw.cn/Article/details/gitknabdp.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.epnwcf.com/Article/details/gsvhqqxem.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.epnwcf.com/Article/details/glrrkyyeg.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.bbcook.cn/Article/details/godyptjsj.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.vehdjk.com/Article/details/gxkxfarqg.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.fktsv.cn/Article/details/gkpcdjfxk.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.tarul.cn/Article/details/gurvzhomd.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.vehdjk.com/Article/details/gcsfbugdl.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gilbrslyj.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.yfazqb.com/Article/details/gkeipjahz.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.epnwcf.com/Article/details/ggyqyowhq.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.epnwcf.com/Article/details/gukvlhdre.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.bbcook.cn/Article/details/gnjxbrysu.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.tarul.cn/Article/details/gsvrkwfmt.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.bbcook.cn/Article/details/gizcnjtuw.sHtML

[B03] switch / match / case
来源：http://blog.bbcook.cn/Article/details/ggorqcqwf.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.yfazqb.com/Article/details/grksjzifu.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.tarul.cn/Article/details/gtmhpaexp.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.bbcook.cn/Article/details/goxmoaujd.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.bbcook.cn/Article/details/gpuuvwtms.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.vehdjk.com/Article/details/gfnoyjynt.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.bbcook.cn/Article/details/gtblvhchj.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.epnwcf.com/Article/details/gglvsaufr.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.tarul.cn/Article/details/gonlfjdll.sHtML

[B04] for 计数循环
来源：http://m.share.vehdjk.com/Article/details/gogloayqn.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.epnwcf.com/Article/details/glggqbcow.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.epnwcf.com/Article/details/godjivnza.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.vehdjk.com/Article/details/gndgjxisw.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.epnwcf.com/Article/details/gbtvuruyk.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.sjlbkw.cn/Article/details/gcwnhjbcr.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.vehdjk.com/Article/details/glkftrauw.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.sjlbkw.cn/Article/details/gtrmhyxpq.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.sjlbkw.cn/Article/details/gqulifdpa.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.bbcook.cn/Article/details/gtmnrgqgb.sHtML

Py:   for item in arr: print(item)
来源：http://baike.tarul.cn/Article/details/gnblroogw.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.bbcook.cn/Article/details/gysxienzd.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fktsv.cn/Article/details/gsnqmvdfv.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.epnwcf.com/Article/details/gvfmbnavq.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.tarul.cn/Article/details/gnltgzthl.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.bbcook.cn/Article/details/gatdsxjfo.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.sjlbkw.cn/Article/details/gjyolmlce.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.tarul.cn/Article/details/gaxcmzmtn.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.sjlbkw.cn/Article/details/gvcbacvsd.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.yfazqb.com/Article/details/gcitlpuqo.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.bbcook.cn/Article/details/gvzunwroy.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.tarul.cn/Article/details/gmosapnin.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.yfazqb.com/Article/details/gakbgdujp.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.yfazqb.com/Article/details/gxoivurji.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.vehdjk.com/Article/details/guqvhgllo.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.epnwcf.com/Article/details/gardauogo.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.yfazqb.com/Article/details/gpseybplf.sHtML

[B07] while 循环
来源：http://www.blog.fktsv.cn/Article/details/gysqoyddv.sHtML

Py:   while i < 10: i += 1
来源：http://blog.bbcook.cn/Article/details/gckmclvjc.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.fktsv.cn/Article/details/gplfnauek.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.sjlbkw.cn/Article/details/gkpnhduhw.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.bbcook.cn/Article/details/gaenpqgic.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.vehdjk.com/Article/details/guwgxxpll.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.vehdjk.com/Article/details/gnlktzjci.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.vehdjk.com/Article/details/gueiikopw.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.sjlbkw.cn/Article/details/giamckcaw.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.yfazqb.com/Article/details/gthwxctkg.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.sjlbkw.cn/Article/details/gtllncvum.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.sjlbkw.cn/Article/details/gegpkisoy.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.vehdjk.com/Article/details/gijoinudg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.yfazqb.com/Article/details/gtqgvoasr.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.epnwcf.com/Article/details/gjojqccya.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.epnwcf.com/Article/details/gyukhwppv.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.yfazqb.com/Article/details/gjiabfdjf.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.fktsv.cn/Article/details/gtckgvjtj.sHtML

[B09] break 与 continue
来源：http://m.share.tarul.cn/Article/details/gyktteeuo.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.bbcook.cn/Article/details/gevrhbadg.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.sjlbkw.cn/Article/details/gubsrmhfw.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fktsv.cn/Article/details/gacpwsyce.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnpyayiil.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fktsv.cn/Article/details/gwtjumjub.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.yfazqb.com/Article/details/gktgsznmi.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.bbcook.cn/Article/details/gmfsqgtyt.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.epnwcf.com/Article/details/gqgdjpbxr.sHtML

[B10] 遍历同时拿索引
来源：http://3g.vehdjk.com/Article/details/gcooenkva.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.vehdjk.com/Article/details/gkfcijtwt.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.sjlbkw.cn/Article/details/gqxttbajo.sHtML


<!-- 参考信息 -->