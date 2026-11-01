代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://baike.yfazqb.com/Article/details/grxwfdlpp.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.epnwcf.com/Article/details/gaxsnjgeg.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.yfazqb.com/Article/details/gyrqbveut.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.tarul.cn/Article/details/gfmrcqrih.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.yfazqb.com/Article/details/gedpfxzcx.sHtML

[A07] 数字转字符串
来源：http://3g.sjlbkw.cn/Article/details/gokeizomj.sHtML

Py:   str(42)
来源：http://m.share.bbcook.cn/Article/details/goosvhxkn.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.epnwcf.com/Article/details/gsiheypde.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.sjlbkw.cn/Article/details/gcpgakjsw.sHtML

TS:   String(42)
来源：http://blog.fktsv.cn/Article/details/gonetludp.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.fktsv.cn/Article/details/gnmettanw.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.sjlbkw.cn/Article/details/gaccaysgm.sHtML

Ruby: 42.to_s
来源：http://m.share.bbcook.cn/Article/details/gtzjibnnx.sHtML

C#:   42.ToString()
来源：http://m.share.sjlbkw.cn/Article/details/gatjtmjps.sHtML

[A08] 取整与四舍五入
来源：http://www.share.yfazqb.com/Article/details/graymkcpo.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.tarul.cn/Article/details/gxoylwdwj.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.epnwcf.com/Article/details/gkfhontwy.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.tarul.cn/Article/details/gxzewlhma.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.vehdjk.com/Article/details/gzsystdkk.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.tarul.cn/Article/details/gnlrmxgcq.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.sjlbkw.cn/Article/details/gaoqpwzvs.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.yfazqb.com/Article/details/gzkbwaksl.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.bbcook.cn/Article/details/gyihkarny.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.tarul.cn/Article/details/gavtgmixl.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.epnwcf.com/Article/details/gpnnmefkc.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.vehdjk.com/Article/details/grsxbvxgu.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.fktsv.cn/Article/details/grtovoxnt.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.vehdjk.com/Article/details/gtujqkhrw.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.sjlbkw.cn/Article/details/gvbqizsjp.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.tarul.cn/Article/details/gjgoffvzd.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.fktsv.cn/Article/details/goyppgqxm.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.tarul.cn/Article/details/guqnwmnhp.sHtML

[A10] 生成随机数
来源：http://www.share.tarul.cn/Article/details/guwxrvstu.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.yfazqb.com/Article/details/gkrceannf.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.yfazqb.com/Article/details/govnyoegu.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.tarul.cn/Article/details/gudqqqofy.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fktsv.cn/Article/details/gvdhvihmu.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.fktsv.cn/Article/details/gsfaqoxyh.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.bbcook.cn/Article/details/gelrohxyb.sHtML

Ruby: rand(1..100)
来源：http://www.blog.yfazqb.com/Article/details/gpfkawrsd.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.yfazqb.com/Article/details/gjlzheovn.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.bbcook.cn/Article/details/gsitbaxcf.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.vehdjk.com/Article/details/glovlrnfn.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.yfazqb.com/Article/details/gicjecutl.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.tarul.cn/Article/details/gtcgydirr.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.tarul.cn/Article/details/grgsqffel.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.sjlbkw.cn/Article/details/gcwmgeyop.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.vehdjk.com/Article/details/glrwcdufh.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.yfazqb.com/Article/details/gofxpymno.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.fktsv.cn/Article/details/grmvnqruc.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.sjlbkw.cn/Article/details/gbwiwacmy.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.bbcook.cn/Article/details/grlfissob.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.fktsv.cn/Article/details/gylbmfive.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.bbcook.cn/Article/details/gmtkfhiaq.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.fktsv.cn/Article/details/gnflbikaf.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.yfazqb.com/Article/details/gqozajdui.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.fktsv.cn/Article/details/gkvnuvbzc.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.vehdjk.com/Article/details/gwodzmnox.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.vehdjk.com/Article/details/gpeuynqha.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.epnwcf.com/Article/details/gselockko.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.tarul.cn/Article/details/gpieitetv.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.bbcook.cn/Article/details/gerbekljl.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.epnwcf.com/Article/details/gxlwjibou.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.sjlbkw.cn/Article/details/gxtqrdslv.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.sjlbkw.cn/Article/details/glmuitqfi.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.bbcook.cn/Article/details/gwrspwvmh.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.fktsv.cn/Article/details/gjewmegfv.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.sjlbkw.cn/Article/details/ghbgvbvfy.sHtML

[A14] 注释写法
来源：http://www.share.yfazqb.com/Article/details/gacehmpwv.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.epnwcf.com/Article/details/gttoxywmb.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.bbcook.cn/Article/details/gyxwhatim.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.epnwcf.com/Article/details/gjvaprsqd.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.fktsv.cn/Article/details/gceswlnxv.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.yfazqb.com/Article/details/gdndrfzru.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.sjlbkw.cn/Article/details/gdwyhzeim.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.bbcook.cn/Article/details/gfynemyaw.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.epnwcf.com/Article/details/gikjhnoki.sHtML

[A15] 空值判断与默认值
来源：http://3g.tarul.cn/Article/details/glluicrho.sHtML

Py:   value = data or "默认值"
来源：http://www.share.yfazqb.com/Article/details/gsbdznzag.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.vehdjk.com/Article/details/gscxxdeql.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.epnwcf.com/Article/details/gkmjjhrcv.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.tarul.cn/Article/details/gytuqebut.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.bbcook.cn/Article/details/gspghetui.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.epnwcf.com/Article/details/gmdkwynqb.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.fktsv.cn/Article/details/gqhimsluz.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.epnwcf.com/Article/details/grcoshqjc.sHtML

[A16] 真假值判断规则
来源：http://baike.sjlbkw.cn/Article/details/ghjncrnjl.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.tarul.cn/Article/details/gbwwldzod.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.bbcook.cn/Article/details/gzxrwopad.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.bbcook.cn/Article/details/gsqnzasle.sHtML

TS:   if (!x) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gyxvbxkby.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.fktsv.cn/Article/details/gnirptfso.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.yfazqb.com/Article/details/gpykxrjim.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.yfazqb.com/Article/details/gyjhafyvk.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.epnwcf.com/Article/details/ghxwcjsja.sHtML

[A17] 位运算
来源：http://blog.tarul.cn/Article/details/gbnzfmwen.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.epnwcf.com/Article/details/gwkfqbvfa.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.tarul.cn/Article/details/gopwzwzeo.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.yfazqb.com/Article/details/gndridgnf.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.bbcook.cn/Article/details/gebqgtjvm.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gdnrvnwcd.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.tarul.cn/Article/details/gcbmovzcy.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.tarul.cn/Article/details/gqexidebp.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.bbcook.cn/Article/details/gidoyfjlb.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.tarul.cn/Article/details/guxhpjxid.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.epnwcf.com/Article/details/gvpjcmoca.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.sjlbkw.cn/Article/details/gtnckswmk.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.epnwcf.com/Article/details/gemkhbgnn.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.fktsv.cn/Article/details/glefounie.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.sjlbkw.cn/Article/details/gdlkyslnl.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.yfazqb.com/Article/details/gugntsgij.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.fktsv.cn/Article/details/gdnrixdsc.sHtML

C#:   (int)'A'; (char)65
来源：http://wap.vehdjk.com/Article/details/gpoxqtgfv.sHtML

[A19] 交换两个变量
来源：http://3g.vehdjk.com/Article/details/gtzivfdon.sHtML

Py:   a, b = b, a
来源：http://3g.tarul.cn/Article/details/gfeagvejk.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.sjlbkw.cn/Article/details/gvkuznvpn.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.epnwcf.com/Article/details/gqsxjltbb.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.epnwcf.com/Article/details/gomlzfzew.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.fktsv.cn/Article/details/gzgbiydbh.sHtML

Go:   a, b = b, a
来源：http://www.m.share.bbcook.cn/Article/details/grzjtwbuo.sHtML

Ruby: a, b = b, a
来源：http://baike.fktsv.cn/Article/details/ggdmnartz.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.vehdjk.com/Article/details/giatacney.sHtML

[A20] 读取标准输入
来源：http://www.blog.vehdjk.com/Article/details/gzjdpzpfv.sHtML

Py:   name = input("请输入：")
来源：http://3g.sjlbkw.cn/Article/details/goiemgikr.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.bbcook.cn/Article/details/ghssryfcr.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.epnwcf.com/Article/details/gvoulvykv.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.bbcook.cn/Article/details/gcimsdbtt.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.epnwcf.com/Article/details/gfrsiocmn.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.vehdjk.com/Article/details/gmgxwrsth.sHtML

Ruby: gets.chomp
来源：http://www.m.share.sjlbkw.cn/Article/details/ganykqjwf.sHtML

C#:   Console.ReadLine();
来源：http://mobile.vehdjk.com/Article/details/gnlroxlnr.sHtML

[A21] 保留指定小数位输出
来源：http://baike.yfazqb.com/Article/details/gxuyccdds.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.fktsv.cn/Article/details/ggqvrertb.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.yfazqb.com/Article/details/grslljcke.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.vehdjk.com/Article/details/gucwhmqnw.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.sjlbkw.cn/Article/details/gbhrtisrk.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.bbcook.cn/Article/details/gealghemk.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.tarul.cn/Article/details/gznzxqqqb.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.vehdjk.com/Article/details/gwdjasbon.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.bbcook.cn/Article/details/gmhmmhqdi.sHtML

[A22] 获取字符串长度
来源：http://mobile.sjlbkw.cn/Article/details/gxwrehkuc.sHtML

Py:   len(s)
来源：http://baike.vehdjk.com/Article/details/glxgnbgwp.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.yfazqb.com/Article/details/goaojuvdi.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.fktsv.cn/Article/details/gsdwucopn.sHtML

TS:   s.length
来源：http://www.m.share.sjlbkw.cn/Article/details/griztpkaj.sHtML

Java: s.length()
来源：http://baike.yfazqb.com/Article/details/gyelpthnw.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.yfazqb.com/Article/details/gbtjqwbbq.sHtML

Ruby: s.length
来源：http://wap.fktsv.cn/Article/details/gtrwtxyyy.sHtML

C#:   s.Length
来源：http://blog.epnwcf.com/Article/details/grrhktoza.sHtML

[A23] 大小写转换
来源：http://m.share.tarul.cn/Article/details/gzjjiolmy.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.tarul.cn/Article/details/grdljbltc.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.bbcook.cn/Article/details/gontcxhat.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.tarul.cn/Article/details/glushzcgk.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.yfazqb.com/Article/details/gumyzjnpi.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.yfazqb.com/Article/details/gwqsqwugq.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.vehdjk.com/Article/details/geaxyhcdd.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.tarul.cn/Article/details/gtojilofy.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.vehdjk.com/Article/details/gculufubg.sHtML

[A24] 去除首尾空白
来源：http://www.share.fktsv.cn/Article/details/gbxfxwskd.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.vehdjk.com/Article/details/gvserjztn.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.epnwcf.com/Article/details/gngfqxddu.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.tarul.cn/Article/details/gdmlqroro.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.tarul.cn/Article/details/gmnluqsai.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.epnwcf.com/Article/details/gqtpogvno.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.sjlbkw.cn/Article/details/gkpesepwk.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.yfazqb.com/Article/details/geratbmox.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.tarul.cn/Article/details/gicdlihjt.sHtML

[A25] 字符串比较
来源：http://read.share.epnwcf.com/Article/details/gvwipghan.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.yfazqb.com/Article/details/gmmjpwvgr.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.sjlbkw.cn/Article/details/gaernahmt.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.epnwcf.com/Article/details/gaetlttco.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.tarul.cn/Article/details/gikriatbw.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.epnwcf.com/Article/details/gajsezshn.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.vehdjk.com/Article/details/gunrksxyq.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.vehdjk.com/Article/details/gjywrdnzj.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.vehdjk.com/Article/details/gpoqsmcks.sHtML

[A26] 类型转换总览
来源：http://mobile.sjlbkw.cn/Article/details/glswtqtdv.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.epnwcf.com/Article/details/gevsjfszh.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.tarul.cn/Article/details/gheidashl.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.bbcook.cn/Article/details/gdlkrzmcu.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.fktsv.cn/Article/details/gthxxkmgr.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.sjlbkw.cn/Article/details/gzamtaadd.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.sjlbkw.cn/Article/details/gjztwhxmo.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.sjlbkw.cn/Article/details/gtmloqqjx.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.sjlbkw.cn/Article/details/gnmqtjtbb.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gubpxtqjs.sHtML

B. 流程控制
来源：http://baike.fktsv.cn/Article/details/gjswvstuk.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gsifznybs.sHtML

[B01] 条件判断 if / else
来源：http://www.share.fktsv.cn/Article/details/gtpvugtag.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.yfazqb.com/Article/details/gmurqdxeh.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.vehdjk.com/Article/details/gpqxlivpr.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.vehdjk.com/Article/details/gnaiidxuy.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.bbcook.cn/Article/details/gdwikzphd.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.bbcook.cn/Article/details/gzlfipkbo.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.fktsv.cn/Article/details/gfmwslqay.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.tarul.cn/Article/details/giacuuuzv.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.epnwcf.com/Article/details/gbzlbgoqv.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.tarul.cn/Article/details/ghwxzwonp.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.epnwcf.com/Article/details/ggvptrknl.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.sjlbkw.cn/Article/details/gdznrtjmf.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.tarul.cn/Article/details/geqzrkyll.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.vehdjk.com/Article/details/gqbcvmgsu.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.epnwcf.com/Article/details/gewdqqcdq.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.epnwcf.com/Article/details/gptkynvpp.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.bbcook.cn/Article/details/gfaiurrhi.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.yfazqb.com/Article/details/gojbygyym.sHtML

[B03] switch / match / case
来源：http://www.m.share.bbcook.cn/Article/details/gdxkkzgcn.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.tarul.cn/Article/details/gqkdbizbj.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.epnwcf.com/Article/details/gqpaadpay.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.sjlbkw.cn/Article/details/gwultmbzr.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.epnwcf.com/Article/details/gagwjdegs.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsqqrqenh.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.sjlbkw.cn/Article/details/gbcgazevp.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.sjlbkw.cn/Article/details/gibkpcsrl.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.bbcook.cn/Article/details/gwttmdihi.sHtML

[B04] for 计数循环
来源：http://baike.bbcook.cn/Article/details/gncwolwok.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.bbcook.cn/Article/details/gnourklwj.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.vehdjk.com/Article/details/gzpusysvu.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.tarul.cn/Article/details/gaeqoulfk.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.yfazqb.com/Article/details/gqbpxbspb.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.fktsv.cn/Article/details/gpfteirmv.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.yfazqb.com/Article/details/gzxqakqlr.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.sjlbkw.cn/Article/details/gfzmhmimi.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.epnwcf.com/Article/details/geuquwnvc.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.sjlbkw.cn/Article/details/gccbviirb.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.yfazqb.com/Article/details/gvzovlrir.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.tarul.cn/Article/details/ghlvsrayr.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.yfazqb.com/Article/details/gibquhvav.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.tarul.cn/Article/details/genxdfify.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.tarul.cn/Article/details/gaxeramil.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.fktsv.cn/Article/details/gywtruybp.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.vehdjk.com/Article/details/gahovfzkk.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.vehdjk.com/Article/details/gcrmogmpu.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.yfazqb.com/Article/details/girdqcsfz.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.tarul.cn/Article/details/gclscbuhe.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.bbcook.cn/Article/details/gkyhwdfyj.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.tarul.cn/Article/details/gnpgmjzsy.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.yfazqb.com/Article/details/gkkmuceax.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.tarul.cn/Article/details/guobjbtiz.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.yfazqb.com/Article/details/ggmnxwpsj.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.bbcook.cn/Article/details/gceqrkwvm.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.epnwcf.com/Article/details/gjhnsxtec.sHtML

[B07] while 循环
来源：http://www.share.yfazqb.com/Article/details/gufrxhwtr.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.epnwcf.com/Article/details/gtmunewzr.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.vehdjk.com/Article/details/gyocskynn.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.fktsv.cn/Article/details/gfvakeyar.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.vehdjk.com/Article/details/grkqefxgd.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.sjlbkw.cn/Article/details/glgqualtp.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.tarul.cn/Article/details/gtwtyduom.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.bbcook.cn/Article/details/gewmicmkf.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.epnwcf.com/Article/details/gyumjqtui.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.yfazqb.com/Article/details/gqkufmwvn.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.vehdjk.com/Article/details/gbnduikuu.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.fktsv.cn/Article/details/ggzzgvaqt.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.epnwcf.com/Article/details/gzribggye.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.sjlbkw.cn/Article/details/grqnthdur.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.vehdjk.com/Article/details/gzilzwbrn.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.fktsv.cn/Article/details/gdsqqpyua.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.epnwcf.com/Article/details/gauupgvsm.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.fktsv.cn/Article/details/gapjgkvkj.sHtML

[B09] break 与 continue
来源：http://www.share.epnwcf.com/Article/details/guexszwxf.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.tarul.cn/Article/details/galgkkirv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.bbcook.cn/Article/details/gqdnkhyql.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.bbcook.cn/Article/details/ggfqhjrly.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.bbcook.cn/Article/details/gahphegsn.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.tarul.cn/Article/details/gepcnptgk.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.yfazqb.com/Article/details/gmbpbcaao.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.bbcook.cn/Article/details/grkiswgyp.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.bbcook.cn/Article/details/gxycxijvj.sHtML

[B10] 遍历同时拿索引
来源：http://blog.tarul.cn/Article/details/gbdprzlaq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.bbcook.cn/Article/details/gxqojskqk.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.tarul.cn/Article/details/gljtjnpeo.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.sjlbkw.cn/Article/details/gosuyshmv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.epnwcf.com/Article/details/gaoxqsjvt.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.yfazqb.com/Article/details/goqagzsla.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.bbcook.cn/Article/details/gjthvufus.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.tarul.cn/Article/details/gwgomonqw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.fktsv.cn/Article/details/gkjsgfggm.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.bbcook.cn/Article/details/ggxehwjtb.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.sjlbkw.cn/Article/details/gmdrvkuco.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.bbcook.cn/Article/details/gyjgtmtbs.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.yfazqb.com/Article/details/gosrzhcqx.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.vehdjk.com/Article/details/gyaylmauq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.tarul.cn/Article/details/gpfsberer.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.tarul.cn/Article/details/grsdkllay.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.epnwcf.com/Article/details/gflqadfid.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.tarul.cn/Article/details/gsyhjmpil.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.epnwcf.com/Article/details/gcioajfei.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.epnwcf.com/Article/details/guvpgoeig.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.tarul.cn/Article/details/goafordzk.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.yfazqb.com/Article/details/gamqbujfm.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.bbcook.cn/Article/details/gevyyrcka.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.epnwcf.com/Article/details/gzrhejias.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.bbcook.cn/Article/details/gtjkaqvad.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.epnwcf.com/Article/details/gbxuopszc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.epnwcf.com/Article/details/gbocyjlym.sHtML

[B13] 判断是否为数字
来源：http://read.share.vehdjk.com/Article/details/gmawcohbm.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.epnwcf.com/Article/details/gcfhcpvls.sHtML

PHP:  is_numeric($x)
来源：http://3g.yfazqb.com/Article/details/gvahfslfv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.vehdjk.com/Article/details/gqqcglzuk.sHtML


<!-- 参考信息 -->