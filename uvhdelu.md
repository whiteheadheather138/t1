代发 wailian999

[A02] 变量声明与赋值
来源：http://www.share.bbcook.cn/Article/details/gowqkvfbt.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.vehdjk.com/Article/details/gcosnxvgt.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.epnwcf.com/Article/details/gelcanxyq.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.tarul.cn/Article/details/gmsmpjvma.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.epnwcf.com/Article/details/gajtaxsyk.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.vehdjk.com/Article/details/ghzrpesku.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.bbcook.cn/Article/details/gjhfxdimv.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.tarul.cn/Article/details/gunjrffsv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.yfazqb.com/Article/details/ghkjymgob.sHtML

[A03] 常量定义
来源：http://www.m.share.fktsv.cn/Article/details/gidhbaitb.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.epnwcf.com/Article/details/ggqihtrng.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.yfazqb.com/Article/details/gbxgsohbf.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.bbcook.cn/Article/details/ghidlhvwn.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.bbcook.cn/Article/details/gaxnbxvhg.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.yfazqb.com/Article/details/gfdeyswuo.sHtML

Go:   const PI = 3.14159
来源：http://3g.fktsv.cn/Article/details/gsbajlncd.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.yfazqb.com/Article/details/gxwgmoadi.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.tarul.cn/Article/details/gsuizxoer.sHtML

[A04] 判断变量类型
来源：http://mobile.yfazqb.com/Article/details/gxgibfekl.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.yfazqb.com/Article/details/gjfkmujry.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.yfazqb.com/Article/details/gmfkxfyij.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.epnwcf.com/Article/details/gplbarejg.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.bbcook.cn/Article/details/gaiguvpre.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.vehdjk.com/Article/details/gdmzhkydo.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.bbcook.cn/Article/details/goyyrkfqi.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.tarul.cn/Article/details/gtwjerdif.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.epnwcf.com/Article/details/glcbsqqen.sHtML

[A05] 整数除法与取模
来源：http://3g.vehdjk.com/Article/details/ghamzguxo.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.fktsv.cn/Article/details/gmxusqtsa.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.epnwcf.com/Article/details/glmtwxsct.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.tarul.cn/Article/details/gmrblvaiq.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.bbcook.cn/Article/details/gbueodazp.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.tarul.cn/Article/details/gjkivgckp.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.vehdjk.com/Article/details/girttwrii.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.yfazqb.com/Article/details/gdpxvrjrw.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.epnwcf.com/Article/details/gjhphcdou.sHtML

[A06] 字符串转数字
来源：http://m.share.tarul.cn/Article/details/gclaffvcj.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.sjlbkw.cn/Article/details/gjhwosmqh.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.fktsv.cn/Article/details/gepicanik.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.yfazqb.com/Article/details/gjevwhaob.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.fktsv.cn/Article/details/gujwyrepb.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.bbcook.cn/Article/details/gjfgcecof.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.bbcook.cn/Article/details/godqfnxns.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.epnwcf.com/Article/details/gvatiebem.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.tarul.cn/Article/details/gceadscgr.sHtML

[A07] 数字转字符串
来源：http://baike.bbcook.cn/Article/details/gxwdmwqvz.sHtML

Py:   str(42)
来源：http://blog.tarul.cn/Article/details/gsnmgrxog.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.fktsv.cn/Article/details/gvcsjzxqa.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.epnwcf.com/Article/details/gtywzrjhk.sHtML

TS:   String(42)
来源：http://wap.fktsv.cn/Article/details/gmihvkdxv.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.fktsv.cn/Article/details/goyjjiccv.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.fktsv.cn/Article/details/goreuajcx.sHtML

Ruby: 42.to_s
来源：http://read.share.yfazqb.com/Article/details/gottmemso.sHtML

C#:   42.ToString()
来源：http://mobile.fktsv.cn/Article/details/gnheknlye.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.sjlbkw.cn/Article/details/gouawqpya.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdrcqmkji.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.yfazqb.com/Article/details/gilpoamzs.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.yfazqb.com/Article/details/ghvptriud.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.bbcook.cn/Article/details/grjwzsvip.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.sjlbkw.cn/Article/details/gqtrsulah.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.vehdjk.com/Article/details/gkxlbqrky.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.epnwcf.com/Article/details/gcnbkdifq.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.vehdjk.com/Article/details/gkxbccdkt.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.fktsv.cn/Article/details/gwwtemyqd.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.tarul.cn/Article/details/gzzghygho.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.bbcook.cn/Article/details/gtjyrncse.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.epnwcf.com/Article/details/gxybpdosk.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.epnwcf.com/Article/details/gtdutzjgd.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.bbcook.cn/Article/details/ggjnawlqu.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.bbcook.cn/Article/details/gtvnbykdy.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.bbcook.cn/Article/details/gllayapvy.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.vehdjk.com/Article/details/ggqjkvnzu.sHtML

[A10] 生成随机数
来源：http://blog.tarul.cn/Article/details/gqbekhjip.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.fktsv.cn/Article/details/gjrrndabe.sHtML

PHP:  random_int(1, 100);
来源：http://baike.tarul.cn/Article/details/gmwklgsfa.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.yfazqb.com/Article/details/ghwfhqylh.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.epnwcf.com/Article/details/gyimruzns.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.epnwcf.com/Article/details/ghcahdkrw.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.vehdjk.com/Article/details/gbwsmxmvd.sHtML

Ruby: rand(1..100)
来源：http://blog.epnwcf.com/Article/details/gpxifkfgj.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.bbcook.cn/Article/details/gpkifohfg.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.vehdjk.com/Article/details/gorpfrlfu.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.bbcook.cn/Article/details/gbaxtrzsp.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.epnwcf.com/Article/details/gulboyknm.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.tarul.cn/Article/details/gnnmtejyw.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.fktsv.cn/Article/details/gjluplvjb.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.bbcook.cn/Article/details/gbsfjjxcj.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.bbcook.cn/Article/details/guuqsapab.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.epnwcf.com/Article/details/geaohxjvd.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.yfazqb.com/Article/details/gdifaxpky.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.fktsv.cn/Article/details/gjsjfwiiq.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.vehdjk.com/Article/details/gxjtovmlt.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.yfazqb.com/Article/details/glncgfmva.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.epnwcf.com/Article/details/grfidugsd.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.sjlbkw.cn/Article/details/gfsydhbrv.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.tarul.cn/Article/details/guiekvsww.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.epnwcf.com/Article/details/gsgkdydnc.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.bbcook.cn/Article/details/gzyyvxhmd.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.tarul.cn/Article/details/gifzfsccu.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.yfazqb.com/Article/details/gzzkthxif.sHtML

Py:   "第一行\n第二行"
来源：http://baike.vehdjk.com/Article/details/gdkeiiflb.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.sjlbkw.cn/Article/details/gazafwjgg.sHtML

JS:   "第一行\n第二行"
来源：http://wap.epnwcf.com/Article/details/gjfvikado.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.yfazqb.com/Article/details/gsnfllrdw.sHtML

Java: "第一行\n第二行"
来源：http://m.share.sjlbkw.cn/Article/details/gaocybikv.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.sjlbkw.cn/Article/details/gauikjydn.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.vehdjk.com/Article/details/gqadiolnh.sHtML

C#:   "第一行\n第二行"
来源：http://3g.bbcook.cn/Article/details/grwfjmkqu.sHtML

[A14] 注释写法
来源：http://3g.epnwcf.com/Article/details/gtzrwbiye.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.sjlbkw.cn/Article/details/grmvzvgxl.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.sjlbkw.cn/Article/details/gspuxyqfu.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.fktsv.cn/Article/details/gnrtavpdy.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.yfazqb.com/Article/details/gdbfsaxvr.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.vehdjk.com/Article/details/gelwuevcm.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.tarul.cn/Article/details/gqvqmevij.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.fktsv.cn/Article/details/gsoxdkgll.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.bbcook.cn/Article/details/gwfellmno.sHtML

[A15] 空值判断与默认值
来源：http://read.share.yfazqb.com/Article/details/ggvlbjzrn.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.yfazqb.com/Article/details/gwisgqavq.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.tarul.cn/Article/details/guwfzhejf.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.sjlbkw.cn/Article/details/gdodkvcdl.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.yfazqb.com/Article/details/gvprcfdkl.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.epnwcf.com/Article/details/gcfoyrjrg.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.fktsv.cn/Article/details/gjscofabw.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.yfazqb.com/Article/details/ghhfhohwc.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.sjlbkw.cn/Article/details/gjpljvtaf.sHtML

[A16] 真假值判断规则
来源：http://mobile.fktsv.cn/Article/details/glnwnroqt.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.fktsv.cn/Article/details/guhygygjt.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.sjlbkw.cn/Article/details/gfnkmizkk.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.epnwcf.com/Article/details/gkahegdpz.sHtML

TS:   if (!x) {}
来源：http://3g.epnwcf.com/Article/details/gmbdavxrg.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.epnwcf.com/Article/details/gkfzsdioq.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.tarul.cn/Article/details/gjmprvzou.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.tarul.cn/Article/details/gqijjgyfq.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.fktsv.cn/Article/details/gnsjoolba.sHtML

[A17] 位运算
来源：http://read.share.vehdjk.com/Article/details/gllajtxjo.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.yfazqb.com/Article/details/gkljrrkej.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.sjlbkw.cn/Article/details/gnytlaupt.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.yfazqb.com/Article/details/ggauxtfgo.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://3g.sjlbkw.cn/Article/details/grmwavrho.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.yfazqb.com/Article/details/gytjhdxxb.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.bbcook.cn/Article/details/ggwxstzmw.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.sjlbkw.cn/Article/details/gkbxjjubn.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.epnwcf.com/Article/details/ghuucajie.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.yfazqb.com/Article/details/glfooctxk.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.epnwcf.com/Article/details/grlhlnqkn.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.vehdjk.com/Article/details/gzakblulv.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.fktsv.cn/Article/details/grconwntk.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.yfazqb.com/Article/details/gmzlwdpos.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.yfazqb.com/Article/details/gchgbmmon.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.yfazqb.com/Article/details/gdncvdxzw.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.tarul.cn/Article/details/gblglnkio.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.tarul.cn/Article/details/gxholagpr.sHtML

[A19] 交换两个变量
来源：http://wap.yfazqb.com/Article/details/gdbwpgmok.sHtML

Py:   a, b = b, a
来源：http://wap.fktsv.cn/Article/details/gdvocuxea.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.vehdjk.com/Article/details/gjpgzdzry.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.fktsv.cn/Article/details/ghwqegkse.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.bbcook.cn/Article/details/gnckakjuw.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.vehdjk.com/Article/details/givzehrxz.sHtML

Go:   a, b = b, a
来源：http://baike.tarul.cn/Article/details/gzvjlphok.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.epnwcf.com/Article/details/gjzgxifdp.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.vehdjk.com/Article/details/gfjszahae.sHtML

[A20] 读取标准输入
来源：http://www.share.epnwcf.com/Article/details/gfhimclzf.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.yfazqb.com/Article/details/gmmhqrfcx.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.epnwcf.com/Article/details/gdpijgkgj.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.epnwcf.com/Article/details/gggyhvwxn.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.vehdjk.com/Article/details/ghnqhslhu.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.bbcook.cn/Article/details/gyqtztpud.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.fktsv.cn/Article/details/gmjvutyap.sHtML

Ruby: gets.chomp
来源：http://3g.yfazqb.com/Article/details/gnongdncq.sHtML

C#:   Console.ReadLine();
来源：http://blog.sjlbkw.cn/Article/details/gtmmalymn.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.yfazqb.com/Article/details/gvpplfzba.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.sjlbkw.cn/Article/details/ggelpuciy.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.epnwcf.com/Article/details/gxjlzaplr.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.bbcook.cn/Article/details/gvoktmvbk.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.sjlbkw.cn/Article/details/gvegrmyhi.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.yfazqb.com/Article/details/gzkcujsmj.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.yfazqb.com/Article/details/grideycqu.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.epnwcf.com/Article/details/glrupdvje.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.tarul.cn/Article/details/gpnbzlhyx.sHtML

[A22] 获取字符串长度
来源：http://read.share.vehdjk.com/Article/details/gytmyzjhu.sHtML

Py:   len(s)
来源：http://www.share.fktsv.cn/Article/details/gwukwgspp.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.fktsv.cn/Article/details/gglezaugy.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.bbcook.cn/Article/details/gmpdttbxl.sHtML

TS:   s.length
来源：http://m.share.sjlbkw.cn/Article/details/ggtcrunxj.sHtML

Java: s.length()
来源：http://3g.bbcook.cn/Article/details/gzawqtrwq.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.sjlbkw.cn/Article/details/guymoljfw.sHtML

Ruby: s.length
来源：http://www.blog.tarul.cn/Article/details/gtyiwiscb.sHtML

C#:   s.Length
来源：http://baike.yfazqb.com/Article/details/gkgrovrof.sHtML

[A23] 大小写转换
来源：http://read.share.sjlbkw.cn/Article/details/gcsiqlzlt.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.fktsv.cn/Article/details/gyldeuxut.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.bbcook.cn/Article/details/geralsotb.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.yfazqb.com/Article/details/gkacakver.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.vehdjk.com/Article/details/ghopusnfc.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.tarul.cn/Article/details/gieigztsp.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.yfazqb.com/Article/details/gncfxjnjo.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.fktsv.cn/Article/details/gtnkcadoe.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.yfazqb.com/Article/details/gchvgsozn.sHtML

[A24] 去除首尾空白
来源：http://read.share.yfazqb.com/Article/details/gdsubtgos.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.bbcook.cn/Article/details/ghoeqiing.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.epnwcf.com/Article/details/gxjbdudnm.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.epnwcf.com/Article/details/gsejdalbf.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.epnwcf.com/Article/details/gehmdwipx.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.epnwcf.com/Article/details/gpdsfxxqv.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.fktsv.cn/Article/details/gsqpihhkr.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.fktsv.cn/Article/details/gwwufophk.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.bbcook.cn/Article/details/guwumepra.sHtML

[A25] 字符串比较
来源：http://www.m.share.epnwcf.com/Article/details/gwpsfrbgm.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.sjlbkw.cn/Article/details/ggcaglkdf.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.epnwcf.com/Article/details/gzqdnneao.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.tarul.cn/Article/details/guizkxado.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.tarul.cn/Article/details/gnmwepcpr.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.bbcook.cn/Article/details/gniskrxiz.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.sjlbkw.cn/Article/details/gbnlrqopa.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.bbcook.cn/Article/details/gxocogids.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.fktsv.cn/Article/details/gmcwrjbjv.sHtML

[A26] 类型转换总览
来源：http://wap.bbcook.cn/Article/details/gpmbkccae.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.bbcook.cn/Article/details/gwwvelgaj.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.fktsv.cn/Article/details/gzlykgviw.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.tarul.cn/Article/details/gmvshkeiy.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.fktsv.cn/Article/details/gpvjpzsid.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.sjlbkw.cn/Article/details/gyvztorny.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.vehdjk.com/Article/details/grpzzfpst.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.tarul.cn/Article/details/gnwtajkgz.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.yfazqb.com/Article/details/gbfpoyusd.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gqaufvhrr.sHtML

B. 流程控制
来源：http://wap.epnwcf.com/Article/details/ghblrjovw.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gfplgphwt.sHtML

[B01] 条件判断 if / else
来源：http://wap.tarul.cn/Article/details/grgmgdigk.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.tarul.cn/Article/details/gujwiokmd.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.fktsv.cn/Article/details/gzyycckqt.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.yfazqb.com/Article/details/geguxxofr.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.sjlbkw.cn/Article/details/gqraqnsys.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.bbcook.cn/Article/details/glyqowlpq.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.sjlbkw.cn/Article/details/gigtjzxce.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.yfazqb.com/Article/details/gbmfhhdvc.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.tarul.cn/Article/details/gshzfgdvt.sHtML

[B02] 多分支 else if / elif
来源：http://wap.sjlbkw.cn/Article/details/gccbysfhm.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.bbcook.cn/Article/details/gdwfxkfcz.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.sjlbkw.cn/Article/details/guxiyryyp.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.sjlbkw.cn/Article/details/gyafegjde.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.vehdjk.com/Article/details/gaxtzzhnx.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.bbcook.cn/Article/details/gwyhnzuxw.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.vehdjk.com/Article/details/ghmckwayn.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.sjlbkw.cn/Article/details/gtmhyvuiy.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fktsv.cn/Article/details/grcoxpacq.sHtML

[B03] switch / match / case
来源：http://blog.fktsv.cn/Article/details/gyiigqtny.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.fktsv.cn/Article/details/gtdjrleop.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.epnwcf.com/Article/details/glyuynwos.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.bbcook.cn/Article/details/gnnvsascb.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.epnwcf.com/Article/details/gktetqmta.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.bbcook.cn/Article/details/gxabpkmis.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.vehdjk.com/Article/details/gwhptkonb.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.fktsv.cn/Article/details/gdklhoqfh.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.tarul.cn/Article/details/gbzhryrxo.sHtML

[B04] for 计数循环
来源：http://m.share.epnwcf.com/Article/details/gisrmjhde.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.epnwcf.com/Article/details/gqtfgbewu.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.epnwcf.com/Article/details/gcfqoewpj.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.epnwcf.com/Article/details/gcfndtrdq.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.bbcook.cn/Article/details/gjcovzlgl.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.vehdjk.com/Article/details/gatrtziqm.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.fktsv.cn/Article/details/gjgyhwxhz.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.vehdjk.com/Article/details/gkfuyhipq.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.yfazqb.com/Article/details/gayfypblm.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.yfazqb.com/Article/details/gkanvwxif.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.sjlbkw.cn/Article/details/gzmymilyb.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.tarul.cn/Article/details/gcgkppgmu.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.sjlbkw.cn/Article/details/gptcwlpwi.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.vehdjk.com/Article/details/gzgwwcjno.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.sjlbkw.cn/Article/details/gjseapvwd.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.epnwcf.com/Article/details/gytbdygfz.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.sjlbkw.cn/Article/details/gorkcvjsk.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.sjlbkw.cn/Article/details/gnjqhvuly.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.bbcook.cn/Article/details/gubmvpncf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.bbcook.cn/Article/details/gvdxrybkz.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.tarul.cn/Article/details/gikvyohbm.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.vehdjk.com/Article/details/gryrsdiwb.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.bbcook.cn/Article/details/gtyibhybl.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.tarul.cn/Article/details/gyakwxxjz.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.tarul.cn/Article/details/guflehkyi.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.tarul.cn/Article/details/gfyoxbuee.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.bbcook.cn/Article/details/gcvkqkozm.sHtML

[B07] while 循环
来源：http://blog.bbcook.cn/Article/details/gcrwjwepe.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.sjlbkw.cn/Article/details/gcmpgnnvh.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.epnwcf.com/Article/details/gqrcrxsws.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.epnwcf.com/Article/details/gamguwptg.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.tarul.cn/Article/details/gfchewspl.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.bbcook.cn/Article/details/gskzimoih.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.tarul.cn/Article/details/gtfdbpsbs.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.tarul.cn/Article/details/gqigybzvf.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.tarul.cn/Article/details/gdricxutz.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.sjlbkw.cn/Article/details/gqtsmwzfg.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.fktsv.cn/Article/details/gviglzegs.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.bbcook.cn/Article/details/gyfkqvchw.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.vehdjk.com/Article/details/gjofchpjs.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.epnwcf.com/Article/details/gzfhfqswn.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.epnwcf.com/Article/details/goqxlhqtk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.sjlbkw.cn/Article/details/glxskizou.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.vehdjk.com/Article/details/gkbphlqzi.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.sjlbkw.cn/Article/details/gshbxcswi.sHtML


<!-- 参考信息 -->