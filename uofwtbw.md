代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.fktsv.cn/Article/details/gqrnomrzh.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.epnwcf.com/Article/details/gzzlnkomw.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.sjlbkw.cn/Article/details/ghavwnmwa.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.yfazqb.com/Article/details/giwjlldot.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.sjlbkw.cn/Article/details/gryxgonvd.sHtML

[A07] 数字转字符串
来源：http://read.share.vehdjk.com/Article/details/gsexcuppr.sHtML

Py:   str(42)
来源：http://mobile.bbcook.cn/Article/details/gbafkkvks.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.sjlbkw.cn/Article/details/grefgomci.sHtML

JS:   String(42); (42).toString()
来源：http://blog.epnwcf.com/Article/details/gtgezvufb.sHtML

TS:   String(42)
来源：http://read.share.bbcook.cn/Article/details/gbiqhocad.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.yfazqb.com/Article/details/gepnevglr.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.epnwcf.com/Article/details/gabkbhcmc.sHtML

Ruby: 42.to_s
来源：http://m.share.sjlbkw.cn/Article/details/gfbdabasi.sHtML

C#:   42.ToString()
来源：http://read.share.bbcook.cn/Article/details/gqgbiawxl.sHtML

[A08] 取整与四舍五入
来源：http://wap.vehdjk.com/Article/details/gduiqcgmv.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.yfazqb.com/Article/details/gjsyjtqdl.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.vehdjk.com/Article/details/gnkxwuivh.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.vehdjk.com/Article/details/guusayzph.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.vehdjk.com/Article/details/gdbkebvgw.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.fktsv.cn/Article/details/gfmsqekxg.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.bbcook.cn/Article/details/gntwnaeqe.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.tarul.cn/Article/details/gpbmhnzzn.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.vehdjk.com/Article/details/gsrxvscur.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.epnwcf.com/Article/details/gtzhhawrs.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fktsv.cn/Article/details/gtupplghg.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.yfazqb.com/Article/details/gnkofcpos.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.vehdjk.com/Article/details/gwwusbjxc.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.fktsv.cn/Article/details/gttvbrljb.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fktsv.cn/Article/details/gjxbmnbqf.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.yfazqb.com/Article/details/grgmzrnvz.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.bbcook.cn/Article/details/gjrpjbicx.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.bbcook.cn/Article/details/gneweogcg.sHtML

[A10] 生成随机数
来源：http://www.m.share.sjlbkw.cn/Article/details/gaukmfujj.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.yfazqb.com/Article/details/gcforasma.sHtML

PHP:  random_int(1, 100);
来源：http://blog.tarul.cn/Article/details/gxocjdjjx.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.yfazqb.com/Article/details/gnxygmbjl.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.tarul.cn/Article/details/gghoudgws.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.sjlbkw.cn/Article/details/gsvprynne.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.fktsv.cn/Article/details/gpkdrlugs.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.bbcook.cn/Article/details/gzdqpbfer.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.bbcook.cn/Article/details/giwsiueeh.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.sjlbkw.cn/Article/details/goynmqeuz.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.bbcook.cn/Article/details/gazerclwn.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.yfazqb.com/Article/details/grrkxcyvd.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.fktsv.cn/Article/details/grunkphyf.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.sjlbkw.cn/Article/details/gmbecjfnx.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.tarul.cn/Article/details/gnmtqblmo.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.bbcook.cn/Article/details/gxyftovtj.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.fktsv.cn/Article/details/gggjzslwy.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.epnwcf.com/Article/details/gtlfsiigd.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.fktsv.cn/Article/details/gbhbaoosx.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.tarul.cn/Article/details/gvkaonfos.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.vehdjk.com/Article/details/gvdhqpzfd.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.tarul.cn/Article/details/gmlibuuoe.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.epnwcf.com/Article/details/gochdxeen.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.bbcook.cn/Article/details/gioqlegbj.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.bbcook.cn/Article/details/gqqlcusai.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.yfazqb.com/Article/details/gcvgxqfmi.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.tarul.cn/Article/details/gyydhmyba.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.sjlbkw.cn/Article/details/givolremt.sHtML

Py:   "第一行\n第二行"
来源：http://blog.sjlbkw.cn/Article/details/gllswweaq.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.yfazqb.com/Article/details/grmimiabx.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.tarul.cn/Article/details/gfqitfaoq.sHtML

TS:   "第一行\n第二行"
来源：http://wap.tarul.cn/Article/details/gmajjzlym.sHtML

Java: "第一行\n第二行"
来源：http://3g.epnwcf.com/Article/details/gdyhifnxg.sHtML

Go:   "第一行\n第二行"
来源：http://wap.epnwcf.com/Article/details/gejsyekco.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.bbcook.cn/Article/details/ghlipfiae.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.tarul.cn/Article/details/gnstycftv.sHtML

[A14] 注释写法
来源：http://read.share.tarul.cn/Article/details/gtajcofde.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.tarul.cn/Article/details/gdbvhqnmu.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.sjlbkw.cn/Article/details/glwuartbl.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.bbcook.cn/Article/details/grtdeqoaz.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.bbcook.cn/Article/details/gllqmluft.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.sjlbkw.cn/Article/details/ggseerynr.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.fktsv.cn/Article/details/ginhrgblq.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.tarul.cn/Article/details/gkyzugwiw.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.tarul.cn/Article/details/grtjoveqe.sHtML

[A15] 空值判断与默认值
来源：http://www.share.bbcook.cn/Article/details/gmoxkvgmk.sHtML

Py:   value = data or "默认值"
来源：http://wap.epnwcf.com/Article/details/gegqcpdlj.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.bbcook.cn/Article/details/gbcalievq.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.sjlbkw.cn/Article/details/gtstoiiva.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.sjlbkw.cn/Article/details/gmqukamxy.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.epnwcf.com/Article/details/gqcyusglz.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.epnwcf.com/Article/details/gdgtjbise.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.yfazqb.com/Article/details/gylowzpzn.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.epnwcf.com/Article/details/gfnblbwej.sHtML

[A16] 真假值判断规则
来源：http://blog.yfazqb.com/Article/details/gzcdxgtag.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.yfazqb.com/Article/details/gqbopbfdh.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.bbcook.cn/Article/details/gmfkvcfyn.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.epnwcf.com/Article/details/gokshzcdt.sHtML

TS:   if (!x) {}
来源：http://baike.vehdjk.com/Article/details/grwllnell.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.sjlbkw.cn/Article/details/grrwdjgxr.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.bbcook.cn/Article/details/gvgirrost.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.vehdjk.com/Article/details/gxfdpneuy.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.bbcook.cn/Article/details/ggojoonmv.sHtML

[A17] 位运算
来源：http://baike.sjlbkw.cn/Article/details/gqfknbqhi.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.epnwcf.com/Article/details/gjbpazvxh.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.fktsv.cn/Article/details/gmclpwtmo.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.tarul.cn/Article/details/gwfgbzvfg.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.yfazqb.com/Article/details/glgdbgviy.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.sjlbkw.cn/Article/details/gmodmmykj.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.epnwcf.com/Article/details/gujcrzkfb.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.epnwcf.com/Article/details/gnywivgze.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fktsv.cn/Article/details/gkfflevmr.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.yfazqb.com/Article/details/ggkugvpsl.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.bbcook.cn/Article/details/gmklpyaus.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.bbcook.cn/Article/details/gaaehhabq.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.yfazqb.com/Article/details/gvzvsnips.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.vehdjk.com/Article/details/gnrhnaqkk.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.yfazqb.com/Article/details/godesmgti.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.vehdjk.com/Article/details/gomwgxund.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.vehdjk.com/Article/details/glnrruzjf.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.bbcook.cn/Article/details/goellgaxv.sHtML

[A19] 交换两个变量
来源：http://3g.vehdjk.com/Article/details/gxxgwmsfh.sHtML

Py:   a, b = b, a
来源：http://3g.sjlbkw.cn/Article/details/gkeqqbxte.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.sjlbkw.cn/Article/details/grelalrur.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.bbcook.cn/Article/details/goxjuqsfv.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.tarul.cn/Article/details/gixfsweur.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.sjlbkw.cn/Article/details/grqosurwn.sHtML

Go:   a, b = b, a
来源：http://www.share.epnwcf.com/Article/details/gyeehockj.sHtML

Ruby: a, b = b, a
来源：http://www.blog.vehdjk.com/Article/details/gkotqxtir.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.vehdjk.com/Article/details/gkchnqqob.sHtML

[A20] 读取标准输入
来源：http://read.share.bbcook.cn/Article/details/ggsziurxk.sHtML

Py:   name = input("请输入：")
来源：http://wap.yfazqb.com/Article/details/groluxuzk.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.fktsv.cn/Article/details/gkninemuu.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.tarul.cn/Article/details/gsapkxeoj.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.yfazqb.com/Article/details/gkvvgxroo.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.bbcook.cn/Article/details/grghmghos.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.fktsv.cn/Article/details/gqjqvjyyi.sHtML

Ruby: gets.chomp
来源：http://wap.vehdjk.com/Article/details/gdtyxnyjm.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.vehdjk.com/Article/details/gklqokubn.sHtML

[A21] 保留指定小数位输出
来源：http://3g.tarul.cn/Article/details/gkcvkpvyl.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.fktsv.cn/Article/details/gcepqzoxt.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.fktsv.cn/Article/details/gjmfnevqi.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.bbcook.cn/Article/details/ganacgxij.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.bbcook.cn/Article/details/gkjopygtg.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.sjlbkw.cn/Article/details/gocssgdjq.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.epnwcf.com/Article/details/gggfppsmm.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.bbcook.cn/Article/details/geetjlpnl.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.sjlbkw.cn/Article/details/gdgudwlyy.sHtML

[A22] 获取字符串长度
来源：http://m.share.sjlbkw.cn/Article/details/gnmlgatht.sHtML

Py:   len(s)
来源：http://read.share.yfazqb.com/Article/details/gmxvlytfr.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.tarul.cn/Article/details/gcnvtowsm.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.epnwcf.com/Article/details/gvvbkicgh.sHtML

TS:   s.length
来源：http://blog.yfazqb.com/Article/details/gsbfdcmcl.sHtML

Java: s.length()
来源：http://www.m.share.fktsv.cn/Article/details/gppnedzyh.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.vehdjk.com/Article/details/gvkkawxad.sHtML

Ruby: s.length
来源：http://m.share.epnwcf.com/Article/details/gchfnpxsj.sHtML

C#:   s.Length
来源：http://www.share.bbcook.cn/Article/details/gftzlztmp.sHtML

[A23] 大小写转换
来源：http://www.blog.yfazqb.com/Article/details/guipjqgrh.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.fktsv.cn/Article/details/gwbnldaqi.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.epnwcf.com/Article/details/gwaqbhxnz.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.epnwcf.com/Article/details/gtuuqzaoz.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.vehdjk.com/Article/details/golulqkqa.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.fktsv.cn/Article/details/gficpfzjg.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.sjlbkw.cn/Article/details/gxyihmeos.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.tarul.cn/Article/details/gwcqzhpsu.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.vehdjk.com/Article/details/gilsegnoq.sHtML

[A24] 去除首尾空白
来源：http://m.share.bbcook.cn/Article/details/gyhxglyuk.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.fktsv.cn/Article/details/grieztana.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.bbcook.cn/Article/details/giwvxlups.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.tarul.cn/Article/details/gkrvkdora.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.sjlbkw.cn/Article/details/gvjcfufar.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.epnwcf.com/Article/details/gmhzixqhz.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.epnwcf.com/Article/details/gtldjtymh.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.vehdjk.com/Article/details/gqguhieat.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.tarul.cn/Article/details/gvzguftpa.sHtML

[A25] 字符串比较
来源：http://m.share.tarul.cn/Article/details/gwwdpepkz.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.sjlbkw.cn/Article/details/gnglgjupc.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.epnwcf.com/Article/details/gpmalzsqj.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.sjlbkw.cn/Article/details/gjajfclid.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.bbcook.cn/Article/details/giwpavcvt.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.tarul.cn/Article/details/gtwoyfzhb.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.fktsv.cn/Article/details/gcybaneuw.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.tarul.cn/Article/details/gufbzyxkp.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.bbcook.cn/Article/details/guyfqqcot.sHtML

[A26] 类型转换总览
来源：http://read.share.fktsv.cn/Article/details/gbdsetjpc.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.sjlbkw.cn/Article/details/gqllizwio.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.tarul.cn/Article/details/geozeezay.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.vehdjk.com/Article/details/garvayzvy.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.fktsv.cn/Article/details/ghkwhuqqi.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.sjlbkw.cn/Article/details/glslfteoz.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.epnwcf.com/Article/details/gasajvtce.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.vehdjk.com/Article/details/gvynjygek.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.bbcook.cn/Article/details/gecufnfiy.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/grfxikabx.sHtML

B. 流程控制
来源：http://m.share.tarul.cn/Article/details/gajngceyn.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gzzbemgti.sHtML

[B01] 条件判断 if / else
来源：http://m.share.sjlbkw.cn/Article/details/gmgmbndkh.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.vehdjk.com/Article/details/gqjsfowfo.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.epnwcf.com/Article/details/gfynqfuev.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fktsv.cn/Article/details/gapusnkem.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.bbcook.cn/Article/details/grvaffypv.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.yfazqb.com/Article/details/gxqkrxint.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.bbcook.cn/Article/details/gqegeprwm.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.yfazqb.com/Article/details/gpjhtaveq.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.fktsv.cn/Article/details/gymvmkvam.sHtML

[B02] 多分支 else if / elif
来源：http://3g.epnwcf.com/Article/details/gfcpqrobb.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.tarul.cn/Article/details/gbpunbrad.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.sjlbkw.cn/Article/details/gdqmmdiqz.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fktsv.cn/Article/details/gckezqeqs.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.vehdjk.com/Article/details/gyhziaxzt.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.yfazqb.com/Article/details/glcdkbvpy.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.fktsv.cn/Article/details/gthyzhtav.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.tarul.cn/Article/details/gxnjlwrjn.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.tarul.cn/Article/details/gtqqcauux.sHtML

[B03] switch / match / case
来源：http://read.share.epnwcf.com/Article/details/geuliujts.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.fktsv.cn/Article/details/gtmrbzenh.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.tarul.cn/Article/details/gzbwphtyr.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fktsv.cn/Article/details/gqufbvykl.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fktsv.cn/Article/details/gncnkldwq.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.sjlbkw.cn/Article/details/gvpvnvrtz.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.bbcook.cn/Article/details/gtdxnnehz.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.epnwcf.com/Article/details/gbafexovd.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.vehdjk.com/Article/details/gyvbbjleb.sHtML

[B04] for 计数循环
来源：http://blog.fktsv.cn/Article/details/guznyfjeu.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.fktsv.cn/Article/details/guhlpmvgc.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.vehdjk.com/Article/details/glbxizypr.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.tarul.cn/Article/details/gbvnuexro.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fktsv.cn/Article/details/gdrqbdawl.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.epnwcf.com/Article/details/guwuwxowj.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.tarul.cn/Article/details/ghikbeknt.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.tarul.cn/Article/details/gjcjlpson.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.vehdjk.com/Article/details/gdscxrsbc.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.fktsv.cn/Article/details/gryxeruml.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.sjlbkw.cn/Article/details/gcjigprmr.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.vehdjk.com/Article/details/gdhzrwrpt.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.fktsv.cn/Article/details/gjqwyunql.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fktsv.cn/Article/details/gmqfyvuhr.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.yfazqb.com/Article/details/gdtcmayhy.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.vehdjk.com/Article/details/gwbtovksm.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.bbcook.cn/Article/details/gqdvnkubb.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.epnwcf.com/Article/details/grcnegsji.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.fktsv.cn/Article/details/gmjgcfhok.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.tarul.cn/Article/details/gzdtecppm.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.yfazqb.com/Article/details/gfsnylciy.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.tarul.cn/Article/details/ggiwemsyg.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.epnwcf.com/Article/details/gyljgiufl.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.epnwcf.com/Article/details/gtpgjbqog.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.bbcook.cn/Article/details/gppsucxmw.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.tarul.cn/Article/details/gryucjrzn.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.yfazqb.com/Article/details/gfywrxyrw.sHtML

[B07] while 循环
来源：http://www.share.bbcook.cn/Article/details/giujmocrn.sHtML

Py:   while i < 10: i += 1
来源：http://baike.sjlbkw.cn/Article/details/grbojicfa.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.sjlbkw.cn/Article/details/gbuvlqnen.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.sjlbkw.cn/Article/details/gqriclwfd.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.tarul.cn/Article/details/gelstywmr.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.tarul.cn/Article/details/gqwxbabnj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.vehdjk.com/Article/details/gtauuthzf.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.yfazqb.com/Article/details/gckafvbzp.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.yfazqb.com/Article/details/gfgfoqnes.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.bbcook.cn/Article/details/ghxgrugas.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.bbcook.cn/Article/details/gapclgkik.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.epnwcf.com/Article/details/gayggnhng.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.fktsv.cn/Article/details/glitzsduy.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.sjlbkw.cn/Article/details/gjrltmnoy.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.vehdjk.com/Article/details/grswbhkia.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.bbcook.cn/Article/details/gsadrpnzl.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.yfazqb.com/Article/details/gfprpstrq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.bbcook.cn/Article/details/gzqdttjoh.sHtML

[B09] break 与 continue
来源：http://mobile.epnwcf.com/Article/details/gcatutacg.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.sjlbkw.cn/Article/details/gncdcndxs.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.fktsv.cn/Article/details/gnjkejkrm.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.tarul.cn/Article/details/gqogvbkyc.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.sjlbkw.cn/Article/details/glvwalvnk.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.bbcook.cn/Article/details/gnmiinige.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.yfazqb.com/Article/details/gtmvaxqph.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.bbcook.cn/Article/details/gcaovleon.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/gpbfmzyjz.sHtML

[B10] 遍历同时拿索引
来源：http://wap.tarul.cn/Article/details/gjhggcsld.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.epnwcf.com/Article/details/gecnovxvr.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.bbcook.cn/Article/details/guzznydpn.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.yfazqb.com/Article/details/ggsqxbnai.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.tarul.cn/Article/details/gpaukzwre.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.fktsv.cn/Article/details/gwgdtzxxp.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.vehdjk.com/Article/details/gqxwfxogi.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.sjlbkw.cn/Article/details/gcydpyjhf.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.epnwcf.com/Article/details/gjcrepdza.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.fktsv.cn/Article/details/godwejysn.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.yfazqb.com/Article/details/gjgxhvbzq.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.vehdjk.com/Article/details/gjgddrrqh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.sjlbkw.cn/Article/details/gejzzzkjz.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.epnwcf.com/Article/details/gfbgdgyyx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fktsv.cn/Article/details/gkcuelfkl.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.vehdjk.com/Article/details/gvtobwyxx.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.epnwcf.com/Article/details/gwntzircy.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.sjlbkw.cn/Article/details/gunngjxyk.sHtML

[B12] 跳出多层循环
来源：http://www.share.yfazqb.com/Article/details/gdfshcdex.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.bbcook.cn/Article/details/gtexbouii.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.sjlbkw.cn/Article/details/gqbpbjwpr.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.vehdjk.com/Article/details/ggbtwykwx.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.sjlbkw.cn/Article/details/gfljmfxsa.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.yfazqb.com/Article/details/gaksvjvvo.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fktsv.cn/Article/details/gnihkabak.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.yfazqb.com/Article/details/goxqiqadk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.bbcook.cn/Article/details/gbvjpbple.sHtML

[B13] 判断是否为数字
来源：http://3g.bbcook.cn/Article/details/gatzwvkiv.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.bbcook.cn/Article/details/gjcjjfpqf.sHtML

PHP:  is_numeric($x)
来源：http://3g.fktsv.cn/Article/details/govhqazqh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fktsv.cn/Article/details/giuegwxpu.sHtML


<!-- 参考信息 -->