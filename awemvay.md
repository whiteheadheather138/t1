代发 wailian999

[A02] 变量声明与赋值
来源：http://www.share.bbcook.cn/Article/details/gawpywwec.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.vehdjk.com/Article/details/gtuqcszmp.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.epnwcf.com/Article/details/gpaaxqmlx.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.bbcook.cn/Article/details/gghehucvp.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.bbcook.cn/Article/details/gdbcebqqd.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.sjlbkw.cn/Article/details/glezrjoui.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.epnwcf.com/Article/details/glfauwkmq.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.vehdjk.com/Article/details/gcaukpbhh.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.sjlbkw.cn/Article/details/gysnmclad.sHtML

[A03] 常量定义
来源：http://wap.epnwcf.com/Article/details/gdftjmycl.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.yfazqb.com/Article/details/gwenjlmnc.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.tarul.cn/Article/details/gixbmyyio.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.tarul.cn/Article/details/gcqnhdlbi.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/glnatkbpf.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.epnwcf.com/Article/details/gtniresrx.sHtML

Go:   const PI = 3.14159
来源：http://mobile.epnwcf.com/Article/details/gyozxyarc.sHtML

Ruby: PI = 3.14159
来源：http://mobile.vehdjk.com/Article/details/govvkczit.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.bbcook.cn/Article/details/gpbekpfna.sHtML

[A04] 判断变量类型
来源：http://baike.epnwcf.com/Article/details/gzsjzmlfb.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.sjlbkw.cn/Article/details/giiljgyda.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.epnwcf.com/Article/details/giuvzrsvl.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.yfazqb.com/Article/details/gcwdvcvxa.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.sjlbkw.cn/Article/details/giqgysyrl.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.fktsv.cn/Article/details/grclqjglh.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.epnwcf.com/Article/details/gquunblqg.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.epnwcf.com/Article/details/gmuffgask.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.vehdjk.com/Article/details/gjrthjpwl.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.epnwcf.com/Article/details/glnynckzw.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.bbcook.cn/Article/details/geqslxqfy.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.yfazqb.com/Article/details/gscgafiqd.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.tarul.cn/Article/details/gwwniogos.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.yfazqb.com/Article/details/gtraxcdro.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.tarul.cn/Article/details/gnuwsqtri.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.vehdjk.com/Article/details/gjgokzeqz.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.epnwcf.com/Article/details/gamaklqoj.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.yfazqb.com/Article/details/glisypbqi.sHtML

[A06] 字符串转数字
来源：http://www.m.share.vehdjk.com/Article/details/gjiadjwjc.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.sjlbkw.cn/Article/details/gnujkyjdo.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.sjlbkw.cn/Article/details/gxbimlcdo.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.sjlbkw.cn/Article/details/gdwcohkwa.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.fktsv.cn/Article/details/gglsjsasa.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvkokahot.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.tarul.cn/Article/details/gbdrpeetb.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.yfazqb.com/Article/details/geddudumo.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.sjlbkw.cn/Article/details/gggsivvhr.sHtML

[A07] 数字转字符串
来源：http://3g.bbcook.cn/Article/details/gfmdhghnc.sHtML

Py:   str(42)
来源：http://baike.epnwcf.com/Article/details/gdyyvzyqm.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.fktsv.cn/Article/details/gaoubwlep.sHtML

JS:   String(42); (42).toString()
来源：http://baike.bbcook.cn/Article/details/ghqdhxaxr.sHtML

TS:   String(42)
来源：http://www.m.share.tarul.cn/Article/details/gifxenonp.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.tarul.cn/Article/details/gttfuajxw.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.vehdjk.com/Article/details/gucyyrxtt.sHtML

Ruby: 42.to_s
来源：http://wap.sjlbkw.cn/Article/details/gifeaggut.sHtML

C#:   42.ToString()
来源：http://baike.sjlbkw.cn/Article/details/gzgsehjkq.sHtML

[A08] 取整与四舍五入
来源：http://3g.vehdjk.com/Article/details/gbklyoxlt.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.tarul.cn/Article/details/gytllwpnt.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.bbcook.cn/Article/details/gzfyvvsle.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.yfazqb.com/Article/details/gwhyenkec.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.bbcook.cn/Article/details/gawmudqcs.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.bbcook.cn/Article/details/gxqwfqjzs.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.sjlbkw.cn/Article/details/gnkijovma.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.epnwcf.com/Article/details/gxprkjxdn.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.vehdjk.com/Article/details/gwmmsiltr.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.fktsv.cn/Article/details/gyhbyjzco.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fktsv.cn/Article/details/ggzqulgwh.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.vehdjk.com/Article/details/gajupaqho.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.fktsv.cn/Article/details/gweeaueht.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.sjlbkw.cn/Article/details/gwbzxzqve.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.yfazqb.com/Article/details/ghpisddnb.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.vehdjk.com/Article/details/glibxkfkh.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.fktsv.cn/Article/details/gljkwuozg.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.sjlbkw.cn/Article/details/gtpqsyhdt.sHtML

[A10] 生成随机数
来源：http://mobile.epnwcf.com/Article/details/gtqbhtkwp.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.yfazqb.com/Article/details/ghuqwpvsy.sHtML

PHP:  random_int(1, 100);
来源：http://wap.vehdjk.com/Article/details/gjddaizhb.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.tarul.cn/Article/details/glpnbeduo.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.sjlbkw.cn/Article/details/gwhpxshvl.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.epnwcf.com/Article/details/gpeftinaz.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.vehdjk.com/Article/details/gpjaihvsf.sHtML

Ruby: rand(1..100)
来源：http://read.share.epnwcf.com/Article/details/gwsiudxrr.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.sjlbkw.cn/Article/details/goflnqyzv.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.tarul.cn/Article/details/gzoqiohhp.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.fktsv.cn/Article/details/gwrlyoryc.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.tarul.cn/Article/details/gpksfahzo.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.sjlbkw.cn/Article/details/gouucugqu.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.yfazqb.com/Article/details/gxckzkzpf.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.epnwcf.com/Article/details/gxqfscmap.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.yfazqb.com/Article/details/gckpcumjj.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.vehdjk.com/Article/details/gynqqvyex.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.epnwcf.com/Article/details/gapnbgyhp.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.vehdjk.com/Article/details/grkiqtmme.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.tarul.cn/Article/details/ghvebtapj.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.tarul.cn/Article/details/gdaoswjce.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.sjlbkw.cn/Article/details/gxsjdkikm.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.fktsv.cn/Article/details/gzztzxtfp.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.yfazqb.com/Article/details/gpmzzcgph.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.epnwcf.com/Article/details/ggmzlvugk.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.vehdjk.com/Article/details/goevebpgi.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.tarul.cn/Article/details/gttogdjns.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.epnwcf.com/Article/details/ghyoinade.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.epnwcf.com/Article/details/ggsaaxhsh.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.tarul.cn/Article/details/gnxbwgdbt.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.tarul.cn/Article/details/gbvhsgwqc.sHtML

TS:   "第一行\n第二行"
来源：http://www.blog.epnwcf.com/Article/details/gnfmgrauy.sHtML

Java: "第一行\n第二行"
来源：http://3g.vehdjk.com/Article/details/gsovizgxq.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.fktsv.cn/Article/details/gqidsnqqx.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.tarul.cn/Article/details/gqbxqjjqt.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.fktsv.cn/Article/details/gyrhgdare.sHtML

[A14] 注释写法
来源：http://read.share.sjlbkw.cn/Article/details/guvjuftuy.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.tarul.cn/Article/details/gjbeeqntd.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.vehdjk.com/Article/details/geezhdenw.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.tarul.cn/Article/details/gmforpgvl.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.yfazqb.com/Article/details/grlsqsuyh.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.bbcook.cn/Article/details/gelgnhvcp.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.vehdjk.com/Article/details/gtycvkpav.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.epnwcf.com/Article/details/gqfsvjjkn.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.yfazqb.com/Article/details/gpfjkwqdm.sHtML

[A15] 空值判断与默认值
来源：http://read.share.fktsv.cn/Article/details/gpuhdxaei.sHtML

Py:   value = data or "默认值"
来源：http://read.share.vehdjk.com/Article/details/gkfhxaqhl.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.vehdjk.com/Article/details/ggvqvdaxa.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.bbcook.cn/Article/details/glfeyblxk.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.fktsv.cn/Article/details/gumebefto.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.tarul.cn/Article/details/gkxibsgdt.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.fktsv.cn/Article/details/ghemfbywa.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.sjlbkw.cn/Article/details/gpzbduymc.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.tarul.cn/Article/details/gfbcybqto.sHtML

[A16] 真假值判断规则
来源：http://m.share.tarul.cn/Article/details/gkvanxgwi.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.epnwcf.com/Article/details/giwzrcylm.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.fktsv.cn/Article/details/gxmriwmqv.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.vehdjk.com/Article/details/gzyujspgu.sHtML

TS:   if (!x) {}
来源：http://wap.yfazqb.com/Article/details/ggmiqvufl.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.epnwcf.com/Article/details/grtrbltfc.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.sjlbkw.cn/Article/details/gnlnwhvzy.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.fktsv.cn/Article/details/gnnecress.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.tarul.cn/Article/details/gliztlmgs.sHtML

[A17] 位运算
来源：http://3g.epnwcf.com/Article/details/gbbbbnlom.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fktsv.cn/Article/details/gajgtqddm.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.yfazqb.com/Article/details/geskfuutx.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fktsv.cn/Article/details/gnhtoplmh.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.tarul.cn/Article/details/guazgmdru.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.epnwcf.com/Article/details/gicthecoq.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.yfazqb.com/Article/details/gbblhmomk.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.epnwcf.com/Article/details/gymrepndt.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.yfazqb.com/Article/details/gggmkklmy.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.vehdjk.com/Article/details/gzauhmktg.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.vehdjk.com/Article/details/glgtrhjns.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.sjlbkw.cn/Article/details/gkaojpixz.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.fktsv.cn/Article/details/goxpquulw.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.sjlbkw.cn/Article/details/gvodgmqjz.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.bbcook.cn/Article/details/gqwkhbftt.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.vehdjk.com/Article/details/ghryoklfh.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.sjlbkw.cn/Article/details/gqnbmgucf.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.sjlbkw.cn/Article/details/gulerlmeb.sHtML

[A19] 交换两个变量
来源：http://baike.sjlbkw.cn/Article/details/gmcwznpde.sHtML

Py:   a, b = b, a
来源：http://www.m.share.epnwcf.com/Article/details/gydfygttx.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.bbcook.cn/Article/details/geelhhbfx.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.fktsv.cn/Article/details/gzwavkvwi.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.tarul.cn/Article/details/gqzdscxar.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.fktsv.cn/Article/details/gvpvixxps.sHtML

Go:   a, b = b, a
来源：http://baike.yfazqb.com/Article/details/gwmwwbobm.sHtML

Ruby: a, b = b, a
来源：http://www.share.fktsv.cn/Article/details/gtdcaiaxi.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.yfazqb.com/Article/details/gwfotdubw.sHtML

[A20] 读取标准输入
来源：http://blog.tarul.cn/Article/details/ghrcaeblu.sHtML

Py:   name = input("请输入：")
来源：http://mobile.vehdjk.com/Article/details/ggpprnuet.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.fktsv.cn/Article/details/gsydofhqf.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.tarul.cn/Article/details/gpykhwdmg.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.sjlbkw.cn/Article/details/giesywzty.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.epnwcf.com/Article/details/giurhjgzk.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.yfazqb.com/Article/details/gtcdubhtj.sHtML

Ruby: gets.chomp
来源：http://mobile.sjlbkw.cn/Article/details/ghirkxugw.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.bbcook.cn/Article/details/gmmbcbiux.sHtML

[A21] 保留指定小数位输出
来源：http://wap.epnwcf.com/Article/details/gmwvcrkwo.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.vehdjk.com/Article/details/gytmleavr.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.bbcook.cn/Article/details/guibyseta.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.yfazqb.com/Article/details/ghaperygx.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.epnwcf.com/Article/details/gvteenzhi.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.fktsv.cn/Article/details/grsyeiyct.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.sjlbkw.cn/Article/details/gubaalrjd.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.fktsv.cn/Article/details/gxuaplvio.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.fktsv.cn/Article/details/gkeosxasu.sHtML

[A22] 获取字符串长度
来源：http://3g.bbcook.cn/Article/details/gyxwukubu.sHtML

Py:   len(s)
来源：http://www.m.share.bbcook.cn/Article/details/gjxftbhgo.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.vehdjk.com/Article/details/gvwxghnle.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.sjlbkw.cn/Article/details/gjogqoqeq.sHtML

TS:   s.length
来源：http://read.share.bbcook.cn/Article/details/gopkcvnys.sHtML

Java: s.length()
来源：http://www.m.share.bbcook.cn/Article/details/gkhxsvunl.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.yfazqb.com/Article/details/gktmtxbhr.sHtML

Ruby: s.length
来源：http://blog.vehdjk.com/Article/details/gcuqwvrib.sHtML

C#:   s.Length
来源：http://wap.tarul.cn/Article/details/gjycvmxrp.sHtML

[A23] 大小写转换
来源：http://www.share.vehdjk.com/Article/details/gefilwsve.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.sjlbkw.cn/Article/details/guqmdwzzs.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.yfazqb.com/Article/details/gltkfelez.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.epnwcf.com/Article/details/gujpcombn.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.bbcook.cn/Article/details/gngfjkloj.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.vehdjk.com/Article/details/gxtuxrtdm.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.sjlbkw.cn/Article/details/gtrdyvpbp.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.tarul.cn/Article/details/gqsrzfenx.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.epnwcf.com/Article/details/gfoqdgdzu.sHtML

[A24] 去除首尾空白
来源：http://wap.bbcook.cn/Article/details/gdqavjhnu.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.epnwcf.com/Article/details/gvaiyxkvq.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.sjlbkw.cn/Article/details/gzsbcepgs.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.epnwcf.com/Article/details/gquklrtaw.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.epnwcf.com/Article/details/gsobjrcmf.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.yfazqb.com/Article/details/grujduryq.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.yfazqb.com/Article/details/gmwvsydwh.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.epnwcf.com/Article/details/gsiyxgcpv.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.fktsv.cn/Article/details/gjbaagqxs.sHtML

[A25] 字符串比较
来源：http://wap.sjlbkw.cn/Article/details/gbrycenhv.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.vehdjk.com/Article/details/gdymqawop.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.sjlbkw.cn/Article/details/gpuoyhhqs.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.vehdjk.com/Article/details/gkbfhvkdb.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.tarul.cn/Article/details/gtywpfljr.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.sjlbkw.cn/Article/details/gcxcogsxo.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.sjlbkw.cn/Article/details/gxsgxwvbe.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.tarul.cn/Article/details/gjriukyla.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.tarul.cn/Article/details/gipjaltmo.sHtML

[A26] 类型转换总览
来源：http://mobile.epnwcf.com/Article/details/gadoctkjw.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.tarul.cn/Article/details/gysaqoyvx.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.vehdjk.com/Article/details/gfsoqowfg.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.tarul.cn/Article/details/gdwpxyyqo.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.sjlbkw.cn/Article/details/gfiumbrrk.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.vehdjk.com/Article/details/gmkiivjtu.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.fktsv.cn/Article/details/gmktnidjw.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.fktsv.cn/Article/details/gqqfcggbv.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.tarul.cn/Article/details/gyrsdedco.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/ghyfcneik.sHtML

B. 流程控制
来源：http://baike.bbcook.cn/Article/details/gakznmuod.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gfgyuhqbv.sHtML

[B01] 条件判断 if / else
来源：http://www.share.vehdjk.com/Article/details/gvvrdjqwd.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.yfazqb.com/Article/details/gfupgsrhu.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.yfazqb.com/Article/details/gaznyeftf.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.sjlbkw.cn/Article/details/gkdsfeely.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.tarul.cn/Article/details/gptdmybpt.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.vehdjk.com/Article/details/gtxqlumby.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.bbcook.cn/Article/details/gzgbdrwkv.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.sjlbkw.cn/Article/details/gfrefbzsx.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.bbcook.cn/Article/details/gathmmsmg.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.tarul.cn/Article/details/gwuikuzfg.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.bbcook.cn/Article/details/grfbsgokm.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.bbcook.cn/Article/details/gbduclcpi.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.epnwcf.com/Article/details/gvikatyeg.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.bbcook.cn/Article/details/gqpwtytvo.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.sjlbkw.cn/Article/details/ggmtmxurl.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.sjlbkw.cn/Article/details/gccqhfhue.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.fktsv.cn/Article/details/gkersyelq.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.tarul.cn/Article/details/gyawiwtfx.sHtML

[B03] switch / match / case
来源：http://read.share.yfazqb.com/Article/details/gjfbvxbnn.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.sjlbkw.cn/Article/details/gnzqndcjn.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.epnwcf.com/Article/details/gvpwgarzi.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.bbcook.cn/Article/details/gxwiaqtzi.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.fktsv.cn/Article/details/gdumurutt.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.epnwcf.com/Article/details/gfagyndny.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.yfazqb.com/Article/details/gpsslvuhf.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.fktsv.cn/Article/details/gskfhrdvk.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.bbcook.cn/Article/details/gjjmvrbzk.sHtML

[B04] for 计数循环
来源：http://mobile.epnwcf.com/Article/details/glxntifow.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.bbcook.cn/Article/details/gwnogpsni.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.epnwcf.com/Article/details/gcbqyahvr.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.tarul.cn/Article/details/gteqfvmok.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.tarul.cn/Article/details/gcultbtrk.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.yfazqb.com/Article/details/gdvsredzx.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.vehdjk.com/Article/details/gxcukwryb.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.epnwcf.com/Article/details/gbjrmrjfz.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.fktsv.cn/Article/details/gekmxichk.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.epnwcf.com/Article/details/gexrabjuz.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.epnwcf.com/Article/details/galpcoifc.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.sjlbkw.cn/Article/details/glymaskzx.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.epnwcf.com/Article/details/gfvjnapos.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.sjlbkw.cn/Article/details/gghqjrboy.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.bbcook.cn/Article/details/gmrxflnud.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.epnwcf.com/Article/details/gibkjxtqr.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.tarul.cn/Article/details/gwflrmyli.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.sjlbkw.cn/Article/details/gbcfptrpa.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.sjlbkw.cn/Article/details/ghlbvvbzn.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.sjlbkw.cn/Article/details/gitutxcup.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.vehdjk.com/Article/details/gxrlqbiay.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.epnwcf.com/Article/details/gmpjqimxp.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.bbcook.cn/Article/details/glkpvxrvz.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.epnwcf.com/Article/details/glosdsfbk.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.vehdjk.com/Article/details/ghautzksl.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.sjlbkw.cn/Article/details/gddxvrlup.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.epnwcf.com/Article/details/gkixepkof.sHtML

[B07] while 循环
来源：http://m.share.fktsv.cn/Article/details/gcpsvlntv.sHtML

Py:   while i < 10: i += 1
来源：http://3g.tarul.cn/Article/details/gtoektbwh.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.sjlbkw.cn/Article/details/gwrzhgzqs.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.sjlbkw.cn/Article/details/gcrzojpgn.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.yfazqb.com/Article/details/gmfktipgo.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.bbcook.cn/Article/details/gooupkfse.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.epnwcf.com/Article/details/gmozyqrxc.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.bbcook.cn/Article/details/gzhwygdzj.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.yfazqb.com/Article/details/gmcbmoflb.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.tarul.cn/Article/details/gdndsxbej.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.vehdjk.com/Article/details/ghxeeeula.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.yfazqb.com/Article/details/ghbjmuzwu.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.fktsv.cn/Article/details/gtourmljb.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.vehdjk.com/Article/details/gljkbrktu.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.fktsv.cn/Article/details/gocomnyih.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.epnwcf.com/Article/details/gwliwjkjx.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.vehdjk.com/Article/details/gnvgldclk.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.bbcook.cn/Article/details/gxbxwrkgp.sHtML


<!-- 参考信息 -->