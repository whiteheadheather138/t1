代发 wailian999

JS:   const PI = 3.14159;
来源：http://baike.bbcook.cn/Article/details/gsjyjgbvm.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.vehdjk.com/Article/details/gozesqoyi.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.bbcook.cn/Article/details/gzdnnfmff.sHtML

Go:   const PI = 3.14159
来源：http://mobile.bbcook.cn/Article/details/gfqvsusqt.sHtML

Ruby: PI = 3.14159
来源：http://baike.tarul.cn/Article/details/gsnjzbakt.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gkkjraeno.sHtML

[A04] 判断变量类型
来源：http://read.share.tarul.cn/Article/details/gnbbxkiou.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.fktsv.cn/Article/details/goeiqktob.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.vehdjk.com/Article/details/gcgckpqjf.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.vehdjk.com/Article/details/gzoryzpft.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.sjlbkw.cn/Article/details/gyjhnzqec.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.fktsv.cn/Article/details/gocnmjzoy.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.fktsv.cn/Article/details/gydixuxhr.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.bbcook.cn/Article/details/getjmlgjc.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.epnwcf.com/Article/details/gtvpsuafu.sHtML

[A05] 整数除法与取模
来源：http://blog.epnwcf.com/Article/details/gzzittabh.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.fktsv.cn/Article/details/gqvlkbsub.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.tarul.cn/Article/details/gngpqukvn.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gourwdykg.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.bbcook.cn/Article/details/gmhjwukjq.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.fktsv.cn/Article/details/gkxnmgcgu.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.sjlbkw.cn/Article/details/gkjwkdlhq.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.fktsv.cn/Article/details/gsockslgu.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.epnwcf.com/Article/details/guyzcmnsb.sHtML

[A06] 字符串转数字
来源：http://read.share.epnwcf.com/Article/details/glxqhjzly.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.bbcook.cn/Article/details/gbblsasek.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.epnwcf.com/Article/details/gydhlezsm.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.sjlbkw.cn/Article/details/gbkjxlsis.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.bbcook.cn/Article/details/gqokrudoz.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.fktsv.cn/Article/details/gkazmmkoh.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.vehdjk.com/Article/details/gqlwkuoof.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.sjlbkw.cn/Article/details/gudnamdiv.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.yfazqb.com/Article/details/ggdobpiln.sHtML

[A07] 数字转字符串
来源：http://m.share.epnwcf.com/Article/details/gqrzavbra.sHtML

Py:   str(42)
来源：http://wap.vehdjk.com/Article/details/glrsunskt.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.sjlbkw.cn/Article/details/gzwlcstrk.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.yfazqb.com/Article/details/gmclajgro.sHtML

TS:   String(42)
来源：http://m.share.yfazqb.com/Article/details/gdfitijrb.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.sjlbkw.cn/Article/details/ggehbepul.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.sjlbkw.cn/Article/details/ghjgjcbyr.sHtML

Ruby: 42.to_s
来源：http://www.m.share.tarul.cn/Article/details/grjgoxxal.sHtML

C#:   42.ToString()
来源：http://m.share.yfazqb.com/Article/details/gridujupt.sHtML

[A08] 取整与四舍五入
来源：http://m.share.fktsv.cn/Article/details/gcpsaaajo.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.bbcook.cn/Article/details/gpqythchh.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.bbcook.cn/Article/details/gtrfnoxsj.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.tarul.cn/Article/details/gynnkmtrt.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.epnwcf.com/Article/details/gtlypjarn.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.fktsv.cn/Article/details/gkrdycqwk.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.epnwcf.com/Article/details/gzhjeoatr.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.epnwcf.com/Article/details/gfmnpltjt.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.sjlbkw.cn/Article/details/gcyoiuhvm.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.sjlbkw.cn/Article/details/gtuckbdsk.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.tarul.cn/Article/details/gozehwleb.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.sjlbkw.cn/Article/details/gftaavhvv.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.tarul.cn/Article/details/gscvnzkkf.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gstyflpls.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.sjlbkw.cn/Article/details/gbdwldctd.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.bbcook.cn/Article/details/ghkcrbngw.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.tarul.cn/Article/details/grqhspsqd.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.bbcook.cn/Article/details/gqzewaenu.sHtML

[A10] 生成随机数
来源：http://blog.yfazqb.com/Article/details/gsfylrmdi.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.fktsv.cn/Article/details/gicygjixg.sHtML

PHP:  random_int(1, 100);
来源：http://baike.vehdjk.com/Article/details/gtdbwiesz.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.tarul.cn/Article/details/gmxqxneor.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.tarul.cn/Article/details/gybtnhypc.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.epnwcf.com/Article/details/gvmurzuiz.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.vehdjk.com/Article/details/gpxduuefe.sHtML

Ruby: rand(1..100)
来源：http://baike.bbcook.cn/Article/details/gdfqikssl.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.fktsv.cn/Article/details/gpsldtgfq.sHtML

[A11] 条件表达式（三元）
来源：http://baike.bbcook.cn/Article/details/gpvmzrpth.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.epnwcf.com/Article/details/gfcjiffok.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.bbcook.cn/Article/details/gxhtissfh.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.yfazqb.com/Article/details/geqxdqtaf.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.sjlbkw.cn/Article/details/gwpaecivf.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.fktsv.cn/Article/details/gwjoscyyr.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.epnwcf.com/Article/details/geuqhechv.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.fktsv.cn/Article/details/ghohftsmm.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fktsv.cn/Article/details/gpdkymmim.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.epnwcf.com/Article/details/gofiebjzc.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.vehdjk.com/Article/details/guuvciaeq.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.tarul.cn/Article/details/gwtrirntw.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.epnwcf.com/Article/details/gfflnxmnw.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.bbcook.cn/Article/details/gdvjwiycc.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.yfazqb.com/Article/details/gzbmymrgg.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.fktsv.cn/Article/details/gotfensdt.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.sjlbkw.cn/Article/details/gmlxrzgjy.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.yfazqb.com/Article/details/grjxsxfoa.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.bbcook.cn/Article/details/gtcvisumr.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.tarul.cn/Article/details/gmucwmklh.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.sjlbkw.cn/Article/details/gamkljgvt.sHtML

JS:   "第一行\n第二行"
来源：http://3g.sjlbkw.cn/Article/details/gyzhdbyzh.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.vehdjk.com/Article/details/gcwipxhyy.sHtML

Java: "第一行\n第二行"
来源：http://www.share.fktsv.cn/Article/details/gqvjnmxrk.sHtML

Go:   "第一行\n第二行"
来源：http://wap.bbcook.cn/Article/details/gxvrxzpkv.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.epnwcf.com/Article/details/gtxtjpkrx.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.sjlbkw.cn/Article/details/gnxghckis.sHtML

[A14] 注释写法
来源：http://m.share.sjlbkw.cn/Article/details/gwfytmmni.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.fktsv.cn/Article/details/gcfziwhwq.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.tarul.cn/Article/details/grrywmmsw.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.vehdjk.com/Article/details/gqnjnglfr.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.sjlbkw.cn/Article/details/gbaitnwrb.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.yfazqb.com/Article/details/gsxaumtwv.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.yfazqb.com/Article/details/gnuxkmfcd.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.fktsv.cn/Article/details/gpemjjfzz.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.yfazqb.com/Article/details/ghbqtpeyz.sHtML

[A15] 空值判断与默认值
来源：http://read.share.bbcook.cn/Article/details/gclgnsuar.sHtML

Py:   value = data or "默认值"
来源：http://wap.vehdjk.com/Article/details/gtkisbbbg.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.yfazqb.com/Article/details/gkfdqtdff.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.bbcook.cn/Article/details/gdnlaoujz.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.epnwcf.com/Article/details/gnbljyvev.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.bbcook.cn/Article/details/gtzuvemgs.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.sjlbkw.cn/Article/details/gnifzhfmg.sHtML

Ruby: value = data || "默认值"
来源：http://baike.sjlbkw.cn/Article/details/guuaofhnj.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.bbcook.cn/Article/details/glbnjlplq.sHtML

[A16] 真假值判断规则
来源：http://blog.bbcook.cn/Article/details/gvtxwolsq.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.vehdjk.com/Article/details/gabynmkrs.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.vehdjk.com/Article/details/gvgrwfprc.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.yfazqb.com/Article/details/gftylpyih.sHtML

TS:   if (!x) {}
来源：http://mobile.fktsv.cn/Article/details/gdmtlpxyw.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.yfazqb.com/Article/details/ghjnrjjgk.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.epnwcf.com/Article/details/ghikfxdqt.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.tarul.cn/Article/details/gdqmpebkb.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.vehdjk.com/Article/details/gstcvnjqt.sHtML

[A17] 位运算
来源：http://baike.fktsv.cn/Article/details/gmiesgmfs.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.yfazqb.com/Article/details/gkmedjjzi.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.vehdjk.com/Article/details/gxoeylfyi.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.bbcook.cn/Article/details/gkdnncejy.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.fktsv.cn/Article/details/gsdklkkxo.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fktsv.cn/Article/details/gikjgjomu.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.fktsv.cn/Article/details/gzwumomdw.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gsuffgvuh.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.epnwcf.com/Article/details/gboxhfrzf.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.epnwcf.com/Article/details/grzabuhrx.sHtML

Py:   ord("A"); chr(65)
来源：http://www.share.vehdjk.com/Article/details/gqwieacje.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.fktsv.cn/Article/details/gfsrzaycx.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.yfazqb.com/Article/details/gqfkzbabj.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.vehdjk.com/Article/details/gfmdxkbtn.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.bbcook.cn/Article/details/gddexbjxt.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.yfazqb.com/Article/details/gxtyfwfel.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.sjlbkw.cn/Article/details/goaownppi.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.vehdjk.com/Article/details/gzeinzrdk.sHtML

[A19] 交换两个变量
来源：http://www.m.share.vehdjk.com/Article/details/gcpjqxygu.sHtML

Py:   a, b = b, a
来源：http://3g.fktsv.cn/Article/details/gyydeuulm.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.vehdjk.com/Article/details/gpjniagnm.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.yfazqb.com/Article/details/gydxdmudv.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.tarul.cn/Article/details/gcvudzfws.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.yfazqb.com/Article/details/gfwpitvay.sHtML

Go:   a, b = b, a
来源：http://www.m.share.epnwcf.com/Article/details/gguuvikvc.sHtML

Ruby: a, b = b, a
来源：http://www.share.tarul.cn/Article/details/gfymfpycb.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.vehdjk.com/Article/details/gwcmmccwa.sHtML

[A20] 读取标准输入
来源：http://m.share.fktsv.cn/Article/details/gnmcnuzfu.sHtML

Py:   name = input("请输入：")
来源：http://blog.vehdjk.com/Article/details/gnixswjks.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.vehdjk.com/Article/details/gdekrizau.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.sjlbkw.cn/Article/details/gscymithe.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.sjlbkw.cn/Article/details/gbmodchzk.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.yfazqb.com/Article/details/gpscxktuk.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.vehdjk.com/Article/details/gyqutlvcy.sHtML

Ruby: gets.chomp
来源：http://blog.vehdjk.com/Article/details/gmbkvuqrg.sHtML

C#:   Console.ReadLine();
来源：http://baike.yfazqb.com/Article/details/gifrjadir.sHtML

[A21] 保留指定小数位输出
来源：http://wap.vehdjk.com/Article/details/gurgtyklk.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.bbcook.cn/Article/details/gbysigonl.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.yfazqb.com/Article/details/gcljfftsm.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.tarul.cn/Article/details/girxcmcri.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.vehdjk.com/Article/details/gbpmmgqpz.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.vehdjk.com/Article/details/gngemykce.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.epnwcf.com/Article/details/gkhbsxkpy.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.fktsv.cn/Article/details/gokqysrfe.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.tarul.cn/Article/details/gusmxsben.sHtML

[A22] 获取字符串长度
来源：http://blog.sjlbkw.cn/Article/details/gmefbjavn.sHtML

Py:   len(s)
来源：http://3g.vehdjk.com/Article/details/gcsscgiao.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.yfazqb.com/Article/details/gblqnmkeq.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.bbcook.cn/Article/details/gugfytgeh.sHtML

TS:   s.length
来源：http://www.m.share.vehdjk.com/Article/details/gmeyoqnip.sHtML

Java: s.length()
来源：http://read.share.vehdjk.com/Article/details/gbebxgucw.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.epnwcf.com/Article/details/gsbslvfhl.sHtML

Ruby: s.length
来源：http://www.share.fktsv.cn/Article/details/gpfgagkzc.sHtML

C#:   s.Length
来源：http://www.blog.bbcook.cn/Article/details/gohatuviy.sHtML

[A23] 大小写转换
来源：http://blog.vehdjk.com/Article/details/gpikljgvw.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.tarul.cn/Article/details/gqvhgljmd.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.fktsv.cn/Article/details/gyldshyew.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.yfazqb.com/Article/details/giwvruewz.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.tarul.cn/Article/details/gtitiyojf.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.vehdjk.com/Article/details/guezutucu.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.bbcook.cn/Article/details/gkchqvaop.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.yfazqb.com/Article/details/goagznwad.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.vehdjk.com/Article/details/gxxhrcjpq.sHtML

[A24] 去除首尾空白
来源：http://3g.vehdjk.com/Article/details/gkatzvfpu.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.bbcook.cn/Article/details/gsidmygwf.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.tarul.cn/Article/details/gkjaibiru.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.epnwcf.com/Article/details/guvvylauv.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.vehdjk.com/Article/details/gxiaawlmi.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.bbcook.cn/Article/details/gzgrqwgdu.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.tarul.cn/Article/details/gkpywvgtc.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.bbcook.cn/Article/details/gqlihvkll.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.epnwcf.com/Article/details/gzueqytcy.sHtML

[A25] 字符串比较
来源：http://www.share.vehdjk.com/Article/details/gzbrrmbvl.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.fktsv.cn/Article/details/gygjqwzck.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.epnwcf.com/Article/details/gncidkbsx.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.tarul.cn/Article/details/gcdfxmrzn.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fktsv.cn/Article/details/gslmsaihx.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.epnwcf.com/Article/details/grryrhaih.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.tarul.cn/Article/details/gqksawcsi.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.epnwcf.com/Article/details/gutyoxknh.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.vehdjk.com/Article/details/ggrdtaoqj.sHtML

[A26] 类型转换总览
来源：http://m.share.yfazqb.com/Article/details/ghahgtcsx.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.epnwcf.com/Article/details/grvsroukd.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.bbcook.cn/Article/details/ggahxgfor.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.fktsv.cn/Article/details/gzgmaqxyz.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.epnwcf.com/Article/details/gxklxbfnw.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.yfazqb.com/Article/details/grmxwisky.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.sjlbkw.cn/Article/details/giquiatrv.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.tarul.cn/Article/details/gyediopce.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.vehdjk.com/Article/details/gjajfoxba.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gmyzynewp.sHtML

B. 流程控制
来源：http://www.blog.vehdjk.com/Article/details/gcnetozby.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gfvpgqyit.sHtML

[B01] 条件判断 if / else
来源：http://blog.vehdjk.com/Article/details/gfgidvmcw.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.sjlbkw.cn/Article/details/gvmhymbmf.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.bbcook.cn/Article/details/gprfxbhhd.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fktsv.cn/Article/details/guwevscya.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.sjlbkw.cn/Article/details/gpajoognh.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.yfazqb.com/Article/details/guprklhbf.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.fktsv.cn/Article/details/gnbifsnli.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.sjlbkw.cn/Article/details/gkoiiaeoz.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.tarul.cn/Article/details/gsbrjxida.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.tarul.cn/Article/details/gdlpwyomm.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.yfazqb.com/Article/details/gsdpoyuke.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.sjlbkw.cn/Article/details/gyucenfnv.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.bbcook.cn/Article/details/gjsunwewn.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.yfazqb.com/Article/details/gymluchgl.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.epnwcf.com/Article/details/gjgesjaus.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.bbcook.cn/Article/details/gjjksvzeh.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.epnwcf.com/Article/details/gclbbinbm.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.tarul.cn/Article/details/gchlswnfy.sHtML

[B03] switch / match / case
来源：http://www.m.share.bbcook.cn/Article/details/gbjtlqpes.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.bbcook.cn/Article/details/gqcbambtl.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.yfazqb.com/Article/details/gsqayptqi.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.bbcook.cn/Article/details/gpgfyueiw.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.vehdjk.com/Article/details/gkfsifghw.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.vehdjk.com/Article/details/ghqwevaok.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.fktsv.cn/Article/details/ghrouyeke.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.epnwcf.com/Article/details/glabmqqpo.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.bbcook.cn/Article/details/gftnikvva.sHtML

[B04] for 计数循环
来源：http://www.m.share.epnwcf.com/Article/details/gtssdlwgt.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.tarul.cn/Article/details/gbnjlkyrb.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.tarul.cn/Article/details/gxhdhmceu.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.sjlbkw.cn/Article/details/gaiddrzjm.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.fktsv.cn/Article/details/glaycmlck.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.vehdjk.com/Article/details/gmskgbvch.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.fktsv.cn/Article/details/gusmyxhtv.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.yfazqb.com/Article/details/gkuuoavjn.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.epnwcf.com/Article/details/grujprewx.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.epnwcf.com/Article/details/gsgdcnrzr.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.vehdjk.com/Article/details/gumkhoiic.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.epnwcf.com/Article/details/gljnorwwt.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.yfazqb.com/Article/details/gwhlkwnzk.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.epnwcf.com/Article/details/gcbqcongl.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.yfazqb.com/Article/details/guelvfprn.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.yfazqb.com/Article/details/gabiojmhw.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.epnwcf.com/Article/details/gmmtvrlwc.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.sjlbkw.cn/Article/details/guzcpfdlq.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.tarul.cn/Article/details/gsbyfvrbp.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.fktsv.cn/Article/details/gdwaslcfl.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.bbcook.cn/Article/details/gpyjrnyts.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.bbcook.cn/Article/details/glfyvpdmr.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.vehdjk.com/Article/details/gwxuukpzj.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.tarul.cn/Article/details/gzkigicns.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.yfazqb.com/Article/details/gpxbogyky.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.fktsv.cn/Article/details/gcmrjkuys.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.fktsv.cn/Article/details/gofkctzgu.sHtML

[B07] while 循环
来源：http://read.share.epnwcf.com/Article/details/gvzftgwtk.sHtML

Py:   while i < 10: i += 1
来源：http://baike.bbcook.cn/Article/details/gapafuadq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.vehdjk.com/Article/details/gkzqaykph.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.bbcook.cn/Article/details/gwaosthfe.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.sjlbkw.cn/Article/details/gydkpxskk.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.tarul.cn/Article/details/gsmkushri.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.vehdjk.com/Article/details/ghpjznesa.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.bbcook.cn/Article/details/gferpsbsd.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.yfazqb.com/Article/details/gymdabmfc.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.fktsv.cn/Article/details/gujarfrws.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.fktsv.cn/Article/details/gruknuclp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.vehdjk.com/Article/details/gnwouehjj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.tarul.cn/Article/details/ghptphrxj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.sjlbkw.cn/Article/details/ggxkxsovr.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbhzyywxn.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.vehdjk.com/Article/details/gfrhamolg.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.yfazqb.com/Article/details/geuqclvfx.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.tarul.cn/Article/details/gomqsxscx.sHtML

[B09] break 与 continue
来源：http://mobile.fktsv.cn/Article/details/ghucqlfgf.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.tarul.cn/Article/details/ggdlppkob.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.fktsv.cn/Article/details/gyigndkqv.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.tarul.cn/Article/details/gnxmcnxxm.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.bbcook.cn/Article/details/gedytbmkh.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.tarul.cn/Article/details/ghadtkafz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmcgbmqqj.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.tarul.cn/Article/details/gbmjyhxcj.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.bbcook.cn/Article/details/gpnnfygfl.sHtML

[B10] 遍历同时拿索引
来源：http://baike.epnwcf.com/Article/details/gyfulippo.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.vehdjk.com/Article/details/gmzjbgdso.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.yfazqb.com/Article/details/gvwlhmlqu.sHtML


<!-- 参考信息 -->