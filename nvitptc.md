代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.tarul.cn/Article/details/gsykvmmwz.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.fktsv.cn/Article/details/gyszyzeem.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.sjlbkw.cn/Article/details/gyqohpxnh.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.vehdjk.com/Article/details/gfrurvxii.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.epnwcf.com/Article/details/gbhycnqba.sHtML

[A07] 数字转字符串
来源：http://read.share.fktsv.cn/Article/details/gaptrgswc.sHtML

Py:   str(42)
来源：http://www.blog.sjlbkw.cn/Article/details/glmfmesji.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.epnwcf.com/Article/details/gpdcghnwk.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.fktsv.cn/Article/details/gveohrxce.sHtML

TS:   String(42)
来源：http://baike.tarul.cn/Article/details/ganshfyqs.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.tarul.cn/Article/details/gjogrlqop.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.tarul.cn/Article/details/gsvagllmr.sHtML

Ruby: 42.to_s
来源：http://www.m.share.tarul.cn/Article/details/gxayvxuvh.sHtML

C#:   42.ToString()
来源：http://www.blog.fktsv.cn/Article/details/gfghvnrlb.sHtML

[A08] 取整与四舍五入
来源：http://m.share.vehdjk.com/Article/details/gqnabydwi.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.bbcook.cn/Article/details/ghpmcskkg.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.bbcook.cn/Article/details/gvfrsbquj.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.tarul.cn/Article/details/gqivnwkek.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.tarul.cn/Article/details/guzabcxjq.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.bbcook.cn/Article/details/gkcggvuvz.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.bbcook.cn/Article/details/gwykupbru.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.epnwcf.com/Article/details/gtsjvtujl.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.bbcook.cn/Article/details/gsjnfbhfj.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.epnwcf.com/Article/details/givphlgza.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.tarul.cn/Article/details/gdnibqdbb.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.yfazqb.com/Article/details/ghphgodff.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.yfazqb.com/Article/details/gvojrxhly.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.vehdjk.com/Article/details/gznmairdh.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.sjlbkw.cn/Article/details/geoscvouv.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.tarul.cn/Article/details/gysygnsdx.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.epnwcf.com/Article/details/gciqpvtht.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gupdcdzkw.sHtML

[A10] 生成随机数
来源：http://www.blog.yfazqb.com/Article/details/gxnsycvoh.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.bbcook.cn/Article/details/gccdwtqus.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.sjlbkw.cn/Article/details/gjkohizcj.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.vehdjk.com/Article/details/ginbfryqt.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.vehdjk.com/Article/details/glgaxwfqj.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.tarul.cn/Article/details/glogtmrpt.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.fktsv.cn/Article/details/gvtjckuri.sHtML

Ruby: rand(1..100)
来源：http://mobile.vehdjk.com/Article/details/gdryjvjvq.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.vehdjk.com/Article/details/gytzvnnkd.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.tarul.cn/Article/details/gukzvpzeu.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.sjlbkw.cn/Article/details/gpuclwojz.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.epnwcf.com/Article/details/gojrzuybn.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.yfazqb.com/Article/details/gfeykxiht.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.vehdjk.com/Article/details/goeeqgeqj.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.fktsv.cn/Article/details/gpkgvswyk.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.sjlbkw.cn/Article/details/gdhlcyghv.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.bbcook.cn/Article/details/gfodcknii.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.bbcook.cn/Article/details/gtliabskw.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.fktsv.cn/Article/details/gcuhjfypa.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.tarul.cn/Article/details/gzodxbcii.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.tarul.cn/Article/details/gyoicyyun.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.fktsv.cn/Article/details/gntwrzlje.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.sjlbkw.cn/Article/details/godgexotz.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.fktsv.cn/Article/details/gebhkrmuq.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.epnwcf.com/Article/details/gnseguxdi.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.epnwcf.com/Article/details/glnpaemcy.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.yfazqb.com/Article/details/gznpkiayt.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.epnwcf.com/Article/details/gwhdnsyev.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.bbcook.cn/Article/details/gnjxjmrse.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.bbcook.cn/Article/details/gshhfejlf.sHtML

JS:   "第一行\n第二行"
来源：http://blog.sjlbkw.cn/Article/details/grxooudrn.sHtML

TS:   "第一行\n第二行"
来源：http://wap.vehdjk.com/Article/details/gkztkqcmz.sHtML

Java: "第一行\n第二行"
来源：http://3g.sjlbkw.cn/Article/details/gdffosacj.sHtML

Go:   "第一行\n第二行"
来源：http://wap.fktsv.cn/Article/details/gbcrtovjn.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.yfazqb.com/Article/details/gjsuctgye.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.yfazqb.com/Article/details/gickjjwnj.sHtML

[A14] 注释写法
来源：http://wap.epnwcf.com/Article/details/gmddxlpmx.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.sjlbkw.cn/Article/details/gsgvvekqz.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.sjlbkw.cn/Article/details/gvuoepgej.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.tarul.cn/Article/details/giruoxxuy.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.yfazqb.com/Article/details/gmznsnhvb.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.epnwcf.com/Article/details/gjpndletn.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.epnwcf.com/Article/details/gtnqdrvnm.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.sjlbkw.cn/Article/details/gmzcbqupn.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.sjlbkw.cn/Article/details/gewjqofwa.sHtML

[A15] 空值判断与默认值
来源：http://read.share.tarul.cn/Article/details/gahfsulow.sHtML

Py:   value = data or "默认值"
来源：http://3g.tarul.cn/Article/details/gdjuvvchw.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.epnwcf.com/Article/details/ggsdletmm.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.vehdjk.com/Article/details/gxfqailqy.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.sjlbkw.cn/Article/details/gfelabmgt.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://read.share.sjlbkw.cn/Article/details/gbzqkjvtv.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.vehdjk.com/Article/details/gxopnwtal.sHtML

Ruby: value = data || "默认值"
来源：http://wap.yfazqb.com/Article/details/gptlpfkge.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.yfazqb.com/Article/details/gajdsjunm.sHtML

[A16] 真假值判断规则
来源：http://mobile.fktsv.cn/Article/details/gaoklnwza.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.epnwcf.com/Article/details/ghrdqemxt.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.fktsv.cn/Article/details/gfvwmcyoj.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.vehdjk.com/Article/details/gxlfelyik.sHtML

TS:   if (!x) {}
来源：http://www.share.fktsv.cn/Article/details/gyapnkoaq.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.tarul.cn/Article/details/gpzucjjly.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.sjlbkw.cn/Article/details/gedfywfzh.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.bbcook.cn/Article/details/gxceiohsz.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.tarul.cn/Article/details/gckeenfqg.sHtML

[A17] 位运算
来源：http://read.share.tarul.cn/Article/details/grjxihice.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.epnwcf.com/Article/details/gdntuglez.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.vehdjk.com/Article/details/gruwpbjud.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.epnwcf.com/Article/details/gdekimili.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.epnwcf.com/Article/details/gvnnmxgbf.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.sjlbkw.cn/Article/details/gxdkebdhn.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.vehdjk.com/Article/details/gxnhpypbu.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.sjlbkw.cn/Article/details/gnokkoavu.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.yfazqb.com/Article/details/gmnwanzat.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.yfazqb.com/Article/details/ghekqnglk.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.sjlbkw.cn/Article/details/gczukdmom.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.tarul.cn/Article/details/ggrbrpsvj.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.fktsv.cn/Article/details/gptyhebml.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.fktsv.cn/Article/details/gbzdnpbpt.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.epnwcf.com/Article/details/gecdkqcbn.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.tarul.cn/Article/details/guhhzotyy.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.tarul.cn/Article/details/ggoaizojk.sHtML

C#:   (int)'A'; (char)65
来源：http://www.m.share.epnwcf.com/Article/details/grejduavw.sHtML

[A19] 交换两个变量
来源：http://www.blog.sjlbkw.cn/Article/details/gfrmwgnzf.sHtML

Py:   a, b = b, a
来源：http://www.blog.epnwcf.com/Article/details/gyzrrouzs.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.tarul.cn/Article/details/gjucqclzo.sHtML

JS:   [a, b] = [b, a];
来源：http://read.share.fktsv.cn/Article/details/gjekpaldh.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.epnwcf.com/Article/details/gltlslcbe.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.bbcook.cn/Article/details/gmmneewbi.sHtML

Go:   a, b = b, a
来源：http://blog.fktsv.cn/Article/details/gpxogkpne.sHtML

Ruby: a, b = b, a
来源：http://wap.bbcook.cn/Article/details/guhsyjdys.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.fktsv.cn/Article/details/gmgictrnf.sHtML

[A20] 读取标准输入
来源：http://wap.sjlbkw.cn/Article/details/gliryfpgz.sHtML

Py:   name = input("请输入：")
来源：http://m.share.epnwcf.com/Article/details/gfpqjcwwx.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.tarul.cn/Article/details/ggzqeqvcp.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.epnwcf.com/Article/details/gtmqhmutl.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.tarul.cn/Article/details/gurhqxamw.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.tarul.cn/Article/details/gppeepzhy.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.epnwcf.com/Article/details/ghffmarsn.sHtML

Ruby: gets.chomp
来源：http://baike.epnwcf.com/Article/details/gtybbwdyl.sHtML

C#:   Console.ReadLine();
来源：http://3g.epnwcf.com/Article/details/ghqgsimjr.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.vehdjk.com/Article/details/gdxrnoley.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.epnwcf.com/Article/details/gtlcqneyt.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.vehdjk.com/Article/details/guokhefcl.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.bbcook.cn/Article/details/gftzmmkvr.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.sjlbkw.cn/Article/details/gxbexsvib.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.epnwcf.com/Article/details/ghitoaixq.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.fktsv.cn/Article/details/gmgsatspn.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.tarul.cn/Article/details/glqdldjvr.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.yfazqb.com/Article/details/gdeahkhmg.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.fktsv.cn/Article/details/gantwefuw.sHtML

Py:   len(s)
来源：http://www.blog.bbcook.cn/Article/details/gemffsooh.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.epnwcf.com/Article/details/gdvwhpmju.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.yfazqb.com/Article/details/gmznmjshk.sHtML

TS:   s.length
来源：http://m.share.yfazqb.com/Article/details/gqjezizsh.sHtML

Java: s.length()
来源：http://baike.tarul.cn/Article/details/gqmlggrrc.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.vehdjk.com/Article/details/grqtbxbyh.sHtML

Ruby: s.length
来源：http://www.share.sjlbkw.cn/Article/details/ghxoolemb.sHtML

C#:   s.Length
来源：http://www.blog.sjlbkw.cn/Article/details/gmnnkinhv.sHtML

[A23] 大小写转换
来源：http://wap.tarul.cn/Article/details/gwdcvdeej.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.epnwcf.com/Article/details/gamaqzerm.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.bbcook.cn/Article/details/ghbecxsif.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.vehdjk.com/Article/details/geiyerwnv.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.yfazqb.com/Article/details/gzbukovwr.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.vehdjk.com/Article/details/glpxamcuf.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.fktsv.cn/Article/details/gxyvfeqjo.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.fktsv.cn/Article/details/gaqwrqoak.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.epnwcf.com/Article/details/grtakfizf.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.bbcook.cn/Article/details/gluortdmo.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.fktsv.cn/Article/details/gwiqonxdb.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.bbcook.cn/Article/details/gpspnsbhu.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.sjlbkw.cn/Article/details/gqamkkynp.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.yfazqb.com/Article/details/gvmazrafi.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.fktsv.cn/Article/details/gtgfusikl.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.fktsv.cn/Article/details/gqkfvytia.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.yfazqb.com/Article/details/ghcpjvtji.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.bbcook.cn/Article/details/gecidjiym.sHtML

[A25] 字符串比较
来源：http://www.m.share.bbcook.cn/Article/details/gadqejfjj.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.tarul.cn/Article/details/gvuhjrczm.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.fktsv.cn/Article/details/guvonjziy.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.vehdjk.com/Article/details/gexsmusmp.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.epnwcf.com/Article/details/guxknhsuj.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.bbcook.cn/Article/details/gibmmhqky.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.fktsv.cn/Article/details/glvxkryci.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.bbcook.cn/Article/details/ggqnfrzaz.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.epnwcf.com/Article/details/gleprtalf.sHtML

[A26] 类型转换总览
来源：http://www.blog.fktsv.cn/Article/details/gcboowllm.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.bbcook.cn/Article/details/gutuknasx.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.tarul.cn/Article/details/gthahwjru.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.vehdjk.com/Article/details/gqdnyzytn.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.sjlbkw.cn/Article/details/ggntjaqow.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.epnwcf.com/Article/details/gikgkhiqz.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.tarul.cn/Article/details/gfajimlvc.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.bbcook.cn/Article/details/giadgiijg.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.bbcook.cn/Article/details/gmuzxznsr.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gexlychrt.sHtML

B. 流程控制
来源：http://www.m.share.epnwcf.com/Article/details/gkhgydmrf.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gpbssqidl.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.tarul.cn/Article/details/gbwbxbbqs.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.bbcook.cn/Article/details/gqtfsxohw.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.yfazqb.com/Article/details/gewqnkajz.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.yfazqb.com/Article/details/gbotjbnhm.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.epnwcf.com/Article/details/gkzxayjel.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.bbcook.cn/Article/details/gihgiehxk.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.vehdjk.com/Article/details/gsaplrjzs.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.epnwcf.com/Article/details/geosjbgsc.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.sjlbkw.cn/Article/details/gkptjhaox.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.vehdjk.com/Article/details/guslckfbl.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.yfazqb.com/Article/details/gwjxwjalh.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.bbcook.cn/Article/details/ggbxfyeue.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.yfazqb.com/Article/details/gndlcmaou.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fktsv.cn/Article/details/gdhmkagon.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.epnwcf.com/Article/details/gsgvxzpxu.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.fktsv.cn/Article/details/genteoiew.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.sjlbkw.cn/Article/details/gsumobioj.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.epnwcf.com/Article/details/gkglqprdc.sHtML

[B03] switch / match / case
来源：http://www.m.share.epnwcf.com/Article/details/gijystius.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.sjlbkw.cn/Article/details/gqofvfxvz.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.sjlbkw.cn/Article/details/geyeetdsp.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.sjlbkw.cn/Article/details/gosmdlsma.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.sjlbkw.cn/Article/details/gegoiruaw.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.tarul.cn/Article/details/gevgtpctq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.vehdjk.com/Article/details/gfqddrbhw.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.sjlbkw.cn/Article/details/gtwhfufmq.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.sjlbkw.cn/Article/details/gykgewsdl.sHtML

[B04] for 计数循环
来源：http://www.share.tarul.cn/Article/details/gjkxmjded.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.vehdjk.com/Article/details/gvggjguin.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.yfazqb.com/Article/details/ggxuylgdl.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fktsv.cn/Article/details/grksgbuoh.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.epnwcf.com/Article/details/gwswzrzml.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.vehdjk.com/Article/details/gxlkmxrwk.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.fktsv.cn/Article/details/gspnpduwe.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.vehdjk.com/Article/details/gjbjvicij.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.yfazqb.com/Article/details/gqynmaiso.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.epnwcf.com/Article/details/gtojrjpae.sHtML

Py:   for item in arr: print(item)
来源：http://wap.fktsv.cn/Article/details/guodcrkcm.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.bbcook.cn/Article/details/gdpspovdt.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.sjlbkw.cn/Article/details/gzvkfxmlz.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.vehdjk.com/Article/details/gsidovddo.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.vehdjk.com/Article/details/gzvkcrxcm.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.tarul.cn/Article/details/gneslcmao.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.fktsv.cn/Article/details/gioffmnaq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.bbcook.cn/Article/details/gtrxwvyoe.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.fktsv.cn/Article/details/gwbaapruf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.sjlbkw.cn/Article/details/ghunmqjry.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.sjlbkw.cn/Article/details/gbdjtzwnd.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.epnwcf.com/Article/details/gmlriiepm.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.yfazqb.com/Article/details/gqrdeqrpq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.tarul.cn/Article/details/gxigyldde.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.bbcook.cn/Article/details/gjjnvbufd.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.yfazqb.com/Article/details/gfkzudeua.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.epnwcf.com/Article/details/gdpixyykr.sHtML

[B07] while 循环
来源：http://wap.bbcook.cn/Article/details/gkuxhzkvy.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.fktsv.cn/Article/details/goemtdpuh.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.vehdjk.com/Article/details/gthggzqub.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.sjlbkw.cn/Article/details/gchyxnzhi.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.yfazqb.com/Article/details/gtgnyewvx.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.sjlbkw.cn/Article/details/gmlcqiyzo.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.tarul.cn/Article/details/gdqajlujx.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.bbcook.cn/Article/details/grlfpbdtj.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.vehdjk.com/Article/details/gjhwpdbcv.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.yfazqb.com/Article/details/ggqblqgqf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.vehdjk.com/Article/details/guixorziv.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.sjlbkw.cn/Article/details/gvjmfliai.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.tarul.cn/Article/details/gloenbhil.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.tarul.cn/Article/details/gbsyzcktp.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.yfazqb.com/Article/details/gxtkdezow.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.sjlbkw.cn/Article/details/gchpybfza.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.yfazqb.com/Article/details/ghwsvzwfw.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.sjlbkw.cn/Article/details/gpdnbxoif.sHtML

[B09] break 与 continue
来源：http://www.blog.tarul.cn/Article/details/gvgxwcclq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fktsv.cn/Article/details/gtmtrroma.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.tarul.cn/Article/details/gqvrfcsuk.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.bbcook.cn/Article/details/gukxivfnt.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.tarul.cn/Article/details/gkuiksdik.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.yfazqb.com/Article/details/gjqqyoqhk.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.yfazqb.com/Article/details/gffpmchoi.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.sjlbkw.cn/Article/details/gfxfjggsc.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.bbcook.cn/Article/details/gftnchnjd.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.sjlbkw.cn/Article/details/gyuvkkabv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.tarul.cn/Article/details/gvyjjsglw.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.fktsv.cn/Article/details/gqwhhekxh.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.tarul.cn/Article/details/gyezashny.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.yfazqb.com/Article/details/ghxeubiwc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.tarul.cn/Article/details/gpdeuwhza.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.sjlbkw.cn/Article/details/gidltpsvx.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.sjlbkw.cn/Article/details/gspxqbsmg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.epnwcf.com/Article/details/gvozrhejm.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.sjlbkw.cn/Article/details/gttcbkafr.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.tarul.cn/Article/details/gshinpshl.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.sjlbkw.cn/Article/details/gnweuhgxg.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.epnwcf.com/Article/details/gnimannta.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.vehdjk.com/Article/details/gtnzhecsg.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gyhanxqjo.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.bbcook.cn/Article/details/gvnwcbblg.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.tarul.cn/Article/details/giivrtfhu.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwduhvnza.sHtML

[B12] 跳出多层循环
来源：http://read.share.sjlbkw.cn/Article/details/glbnlnxwp.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.bbcook.cn/Article/details/glsdavwyc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.yfazqb.com/Article/details/gkellrfzp.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.sjlbkw.cn/Article/details/ggfpwsydt.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.sjlbkw.cn/Article/details/givctsidp.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.bbcook.cn/Article/details/grdbhnfia.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.sjlbkw.cn/Article/details/grhhspgcm.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.bbcook.cn/Article/details/gnkhhnbql.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.fktsv.cn/Article/details/goytmvuzh.sHtML

[B13] 判断是否为数字
来源：http://m.share.epnwcf.com/Article/details/giwscxmlp.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fktsv.cn/Article/details/gbnrgpqlo.sHtML

PHP:  is_numeric($x)
来源：http://blog.vehdjk.com/Article/details/gubcilrtz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.bbcook.cn/Article/details/gxrsfsxnr.sHtML


<!-- 参考信息 -->