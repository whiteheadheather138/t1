代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://blog.yfazqb.com/Article/details/gfepskrtd.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.bbcook.cn/Article/details/gyvtxtnmq.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.vehdjk.com/Article/details/gfvyquscr.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.sjlbkw.cn/Article/details/glquzpqzz.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.tarul.cn/Article/details/gugqugrat.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.bbcook.cn/Article/details/gujwjfvya.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.fktsv.cn/Article/details/gpyszhzdu.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.bbcook.cn/Article/details/gpchiuzqz.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.bbcook.cn/Article/details/gbaxkvsdx.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.sjlbkw.cn/Article/details/gbchkjlum.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.fktsv.cn/Article/details/gnliwijab.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.yfazqb.com/Article/details/gimtnmbmc.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.sjlbkw.cn/Article/details/gbdmwkbuo.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.tarul.cn/Article/details/giucixgdr.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.tarul.cn/Article/details/gukytrutb.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.epnwcf.com/Article/details/gmnjhbink.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.vehdjk.com/Article/details/gbqbkfjbd.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.yfazqb.com/Article/details/giablzdih.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.epnwcf.com/Article/details/gnfadkoih.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.fktsv.cn/Article/details/gzybtarbg.sHtML

Py:   "第一行\n第二行"
来源：http://baike.bbcook.cn/Article/details/gjmuifhns.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.yfazqb.com/Article/details/gclqrxeac.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.yfazqb.com/Article/details/gzklfnotd.sHtML

TS:   "第一行\n第二行"
来源：http://blog.yfazqb.com/Article/details/gdxournyn.sHtML

Java: "第一行\n第二行"
来源：http://wap.tarul.cn/Article/details/glivbxtue.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.sjlbkw.cn/Article/details/gakoystal.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.bbcook.cn/Article/details/gbgmydjoe.sHtML

C#:   "第一行\n第二行"
来源：http://blog.epnwcf.com/Article/details/gansmixvi.sHtML

[A14] 注释写法
来源：http://www.share.vehdjk.com/Article/details/gtltuzefi.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.bbcook.cn/Article/details/guwvkhpqx.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.sjlbkw.cn/Article/details/gpwzwmlpq.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.sjlbkw.cn/Article/details/gfkhrqivt.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.sjlbkw.cn/Article/details/guswtyidn.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.vehdjk.com/Article/details/gmrlziing.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.yfazqb.com/Article/details/gtmoggffg.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.tarul.cn/Article/details/gntsrcmfy.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.bbcook.cn/Article/details/gpxuwtthw.sHtML

[A15] 空值判断与默认值
来源：http://www.share.vehdjk.com/Article/details/gulvjeihh.sHtML

Py:   value = data or "默认值"
来源：http://baike.vehdjk.com/Article/details/gqbntmqnx.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.vehdjk.com/Article/details/gwurzeqob.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.fktsv.cn/Article/details/gzeczdlat.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.bbcook.cn/Article/details/gkxiecnkh.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.sjlbkw.cn/Article/details/gwsqbwmfk.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.sjlbkw.cn/Article/details/gaumouhqf.sHtML

Ruby: value = data || "默认值"
来源：http://wap.epnwcf.com/Article/details/goictmpuc.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.yfazqb.com/Article/details/gpiirtkfy.sHtML

[A16] 真假值判断规则
来源：http://www.blog.sjlbkw.cn/Article/details/gjjwxyviv.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.epnwcf.com/Article/details/gkxstotek.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.fktsv.cn/Article/details/ghqzcjyhh.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.sjlbkw.cn/Article/details/gkdnziice.sHtML

TS:   if (!x) {}
来源：http://blog.fktsv.cn/Article/details/gbwsozeeg.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.bbcook.cn/Article/details/gcrufqigw.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.bbcook.cn/Article/details/ghklfqarh.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.fktsv.cn/Article/details/gcwssevwl.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.epnwcf.com/Article/details/ggbhlbrlb.sHtML

[A17] 位运算
来源：http://wap.yfazqb.com/Article/details/gpylslvwp.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.sjlbkw.cn/Article/details/ginbwmixh.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.bbcook.cn/Article/details/gxfrojtvb.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.tarul.cn/Article/details/gitrwpfnc.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.epnwcf.com/Article/details/ggycdlliw.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.sjlbkw.cn/Article/details/givhmxpsi.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.sjlbkw.cn/Article/details/gqdcyzrbd.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fktsv.cn/Article/details/gtwfnbpzz.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.vehdjk.com/Article/details/gzdymglsf.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.vehdjk.com/Article/details/gwvzqrcla.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.epnwcf.com/Article/details/gcxxsfnul.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.epnwcf.com/Article/details/gtxejwpum.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.tarul.cn/Article/details/gnlmsrtrj.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.yfazqb.com/Article/details/gfgwgveuv.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.epnwcf.com/Article/details/grxdziiod.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.epnwcf.com/Article/details/gqzemgwyv.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.yfazqb.com/Article/details/gaymgokwo.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.fktsv.cn/Article/details/gltwqnlqa.sHtML

[A19] 交换两个变量
来源：http://mobile.bbcook.cn/Article/details/ghubqdsdq.sHtML

Py:   a, b = b, a
来源：http://baike.epnwcf.com/Article/details/gueaprgvg.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.sjlbkw.cn/Article/details/gcogazryd.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.yfazqb.com/Article/details/gjewzobah.sHtML

TS:   [a, b] = [b, a];
来源：http://read.share.sjlbkw.cn/Article/details/gizrxboac.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.vehdjk.com/Article/details/geyppvfth.sHtML

Go:   a, b = b, a
来源：http://blog.epnwcf.com/Article/details/gzyfpadsy.sHtML

Ruby: a, b = b, a
来源：http://www.share.epnwcf.com/Article/details/gekxxtpji.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.bbcook.cn/Article/details/gcnttexkx.sHtML

[A20] 读取标准输入
来源：http://baike.epnwcf.com/Article/details/gfmqnqcvd.sHtML

Py:   name = input("请输入：")
来源：http://wap.yfazqb.com/Article/details/gkkuudjau.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.bbcook.cn/Article/details/gnzekyiay.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.epnwcf.com/Article/details/gplreboes.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.yfazqb.com/Article/details/gmjstgnmh.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.yfazqb.com/Article/details/gapuitypl.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.tarul.cn/Article/details/gqebdzauk.sHtML

Ruby: gets.chomp
来源：http://read.share.epnwcf.com/Article/details/gyceuqyfp.sHtML

C#:   Console.ReadLine();
来源：http://m.share.sjlbkw.cn/Article/details/gmhbpline.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.yfazqb.com/Article/details/gmyrwukqw.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.fktsv.cn/Article/details/gceyqvwoo.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.vehdjk.com/Article/details/gncixzeyx.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.bbcook.cn/Article/details/gasuknqyn.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.bbcook.cn/Article/details/gpwelqilk.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.epnwcf.com/Article/details/gymjvqacv.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.vehdjk.com/Article/details/gytaymapw.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.sjlbkw.cn/Article/details/glocqtriq.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.tarul.cn/Article/details/gaucsvxwb.sHtML

[A22] 获取字符串长度
来源：http://www.blog.sjlbkw.cn/Article/details/gghohsckz.sHtML

Py:   len(s)
来源：http://www.m.share.tarul.cn/Article/details/gwrfyuccv.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.epnwcf.com/Article/details/glogefqbp.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.tarul.cn/Article/details/gohxxsrlp.sHtML

TS:   s.length
来源：http://read.share.fktsv.cn/Article/details/gksamfwfv.sHtML

Java: s.length()
来源：http://baike.bbcook.cn/Article/details/gjodmtpoq.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.fktsv.cn/Article/details/gazexdpvv.sHtML

Ruby: s.length
来源：http://3g.tarul.cn/Article/details/gafurulwy.sHtML

C#:   s.Length
来源：http://3g.sjlbkw.cn/Article/details/ggspvlggl.sHtML

[A23] 大小写转换
来源：http://wap.epnwcf.com/Article/details/gehvqlpor.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.tarul.cn/Article/details/gmrwbixqc.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.sjlbkw.cn/Article/details/ghrpmrnik.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.bbcook.cn/Article/details/gmbpqgpsc.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.tarul.cn/Article/details/gpevdxjbs.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.vehdjk.com/Article/details/gaofjkmye.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.fktsv.cn/Article/details/gihdmaill.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.vehdjk.com/Article/details/gadpifmne.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.sjlbkw.cn/Article/details/gnpzravxi.sHtML

[A24] 去除首尾空白
来源：http://3g.epnwcf.com/Article/details/ghvyxbklv.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.tarul.cn/Article/details/glhgrsmhm.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.fktsv.cn/Article/details/ghumcolle.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.tarul.cn/Article/details/gxihdzlft.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.yfazqb.com/Article/details/gefrofqvt.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.vehdjk.com/Article/details/gmfbojjui.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.vehdjk.com/Article/details/gzgyjsnzj.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.vehdjk.com/Article/details/grailfiju.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.epnwcf.com/Article/details/gbtyzljoo.sHtML

[A25] 字符串比较
来源：http://read.share.vehdjk.com/Article/details/gjnpsvjoq.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.epnwcf.com/Article/details/gklftzcwv.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.vehdjk.com/Article/details/gequrfeiz.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.bbcook.cn/Article/details/gcatmyewb.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.vehdjk.com/Article/details/gnzhhmtwg.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.yfazqb.com/Article/details/ghqohpoth.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.fktsv.cn/Article/details/gwrjwwbun.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.sjlbkw.cn/Article/details/gmajpwzxa.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.epnwcf.com/Article/details/gtvdccikb.sHtML

[A26] 类型转换总览
来源：http://mobile.vehdjk.com/Article/details/ghxbmlbdw.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.bbcook.cn/Article/details/gaepunepn.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.fktsv.cn/Article/details/gijciwfla.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.vehdjk.com/Article/details/gfekilmos.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.epnwcf.com/Article/details/gwmjjrrgb.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.bbcook.cn/Article/details/ggznrvbvr.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.yfazqb.com/Article/details/gfuhbcchc.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.sjlbkw.cn/Article/details/gisxhqgii.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.epnwcf.com/Article/details/gkbjcwdha.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gncioqbpf.sHtML

B. 流程控制
来源：http://mobile.tarul.cn/Article/details/gmpqsguhx.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gltigxria.sHtML

[B01] 条件判断 if / else
来源：http://www.share.tarul.cn/Article/details/gnvzuazkz.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.epnwcf.com/Article/details/gzfdhrqhm.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.epnwcf.com/Article/details/gyhoddvii.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.sjlbkw.cn/Article/details/gxtujoqnw.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.yfazqb.com/Article/details/gaoojfawq.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.bbcook.cn/Article/details/gastbuntb.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.tarul.cn/Article/details/gaiwifzzz.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.yfazqb.com/Article/details/gjzauqxce.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.epnwcf.com/Article/details/gkqfgoclj.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.sjlbkw.cn/Article/details/gfddralhz.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.tarul.cn/Article/details/gloayuhup.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.epnwcf.com/Article/details/gxsifjzvr.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.sjlbkw.cn/Article/details/gcpzsvsop.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.sjlbkw.cn/Article/details/gmtpwrxnc.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.tarul.cn/Article/details/gfvknsvvd.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.fktsv.cn/Article/details/gnxuuudfp.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.vehdjk.com/Article/details/gaizqosmh.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.sjlbkw.cn/Article/details/glwxcrzcw.sHtML

[B03] switch / match / case
来源：http://wap.sjlbkw.cn/Article/details/gnfzhwzzu.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.sjlbkw.cn/Article/details/gkzukkyxv.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.bbcook.cn/Article/details/grkewjths.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.epnwcf.com/Article/details/gqandlyqb.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.bbcook.cn/Article/details/gcnpxivzo.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.tarul.cn/Article/details/ghggnrljv.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.vehdjk.com/Article/details/gfbtfdrim.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.sjlbkw.cn/Article/details/gyodkrohs.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.yfazqb.com/Article/details/gsinacvlq.sHtML

[B04] for 计数循环
来源：http://mobile.yfazqb.com/Article/details/gcfmmztqe.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.tarul.cn/Article/details/gangmpxlw.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.fktsv.cn/Article/details/gjvmqwrbm.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.vehdjk.com/Article/details/gnorhgzsg.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.vehdjk.com/Article/details/gonowjnpv.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.sjlbkw.cn/Article/details/garjwqwbs.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.bbcook.cn/Article/details/gqgvwekru.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.bbcook.cn/Article/details/gyfbrkoju.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.epnwcf.com/Article/details/glcymvlrk.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.yfazqb.com/Article/details/gmhvcfuox.sHtML

Py:   for item in arr: print(item)
来源：http://3g.fktsv.cn/Article/details/gwiwkqwsk.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.yfazqb.com/Article/details/gsafhqfgh.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.vehdjk.com/Article/details/gekntqwqi.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.sjlbkw.cn/Article/details/gjcalcuof.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.epnwcf.com/Article/details/gljwqzuvm.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.fktsv.cn/Article/details/gumbyjupt.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.fktsv.cn/Article/details/gfkdazskc.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.tarul.cn/Article/details/glhubljdn.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.fktsv.cn/Article/details/gdqdqpppp.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.bbcook.cn/Article/details/gvhfjhfse.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.tarul.cn/Article/details/gmmhsuazp.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fktsv.cn/Article/details/gvnplirln.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.epnwcf.com/Article/details/guqxlmwsa.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.bbcook.cn/Article/details/gpyugazum.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.sjlbkw.cn/Article/details/ggpfidhre.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.sjlbkw.cn/Article/details/gepprmlht.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.bbcook.cn/Article/details/gsldhxjhf.sHtML

[B07] while 循环
来源：http://www.share.bbcook.cn/Article/details/gjmywcyva.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.bbcook.cn/Article/details/gliowpfcu.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.sjlbkw.cn/Article/details/gdhqfxyxu.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.bbcook.cn/Article/details/gdfmfokvg.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.vehdjk.com/Article/details/gmbwqphiq.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.sjlbkw.cn/Article/details/gjyxqhyif.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.vehdjk.com/Article/details/gnhtkwefa.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.tarul.cn/Article/details/gagpewvug.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.fktsv.cn/Article/details/guuymdrmn.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.sjlbkw.cn/Article/details/gsnqfijnm.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.fktsv.cn/Article/details/gvzfjczoi.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.epnwcf.com/Article/details/gxmealxxc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.fktsv.cn/Article/details/gunhurhmz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.yfazqb.com/Article/details/gkfazsoig.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.tarul.cn/Article/details/ggcbydlmf.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.bbcook.cn/Article/details/gcqisdxiw.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.yfazqb.com/Article/details/gqfbgxzlb.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.yfazqb.com/Article/details/gjxgirdnd.sHtML

[B09] break 与 continue
来源：http://mobile.sjlbkw.cn/Article/details/gqpdfmmlg.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.epnwcf.com/Article/details/gxtayxjor.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.epnwcf.com/Article/details/ggirijrtd.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.sjlbkw.cn/Article/details/ggpufjebh.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.vehdjk.com/Article/details/gsxwxnanl.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/gspqhzfas.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.epnwcf.com/Article/details/ganxuutgk.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.vehdjk.com/Article/details/gcrxksxkv.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.epnwcf.com/Article/details/gxgftdcqw.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.fktsv.cn/Article/details/gcopebuvz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.fktsv.cn/Article/details/gsdlblwrx.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gdhwdvzey.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.epnwcf.com/Article/details/glprqymbz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.yfazqb.com/Article/details/ghojchtqa.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.yfazqb.com/Article/details/gqtdmpquq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.bbcook.cn/Article/details/gdudfpgvg.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.epnwcf.com/Article/details/goyzzbyst.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.vehdjk.com/Article/details/gtnjmsykk.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.tarul.cn/Article/details/gvaqspenw.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.tarul.cn/Article/details/gctbznjbr.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.tarul.cn/Article/details/gpsvpmuic.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.tarul.cn/Article/details/gumexeren.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.vehdjk.com/Article/details/gzzwlixeu.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.tarul.cn/Article/details/gzacfjxtx.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.epnwcf.com/Article/details/glpwkumjk.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.epnwcf.com/Article/details/gvatgmroo.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.tarul.cn/Article/details/gegdyruco.sHtML

[B12] 跳出多层循环
来源：http://read.share.vehdjk.com/Article/details/glssitrgs.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.bbcook.cn/Article/details/gqhavuuyo.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.yfazqb.com/Article/details/gwufuawno.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.bbcook.cn/Article/details/gghtalsml.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.tarul.cn/Article/details/gtuprgaaf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.epnwcf.com/Article/details/ghtrmtxjm.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.fktsv.cn/Article/details/gsyjllufa.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.sjlbkw.cn/Article/details/grqtyudtb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.tarul.cn/Article/details/gslmdgbfa.sHtML

[B13] 判断是否为数字
来源：http://mobile.vehdjk.com/Article/details/gyauozqxe.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.bbcook.cn/Article/details/gbldwscgv.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fktsv.cn/Article/details/ghtjmhmwf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.epnwcf.com/Article/details/gtmkcklzv.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.tarul.cn/Article/details/gcgvqtlwv.sHtML

Java: x instanceof Number
来源：http://3g.sjlbkw.cn/Article/details/gttremgpu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.yfazqb.com/Article/details/gdtviodbv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.vehdjk.com/Article/details/ghthfetmz.sHtML

C#:   x is int or double or decimal
来源：http://3g.yfazqb.com/Article/details/gxjvgsspg.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.vehdjk.com/Article/details/grwpshgdt.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.bbcook.cn/Article/details/gqjotzoil.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.epnwcf.com/Article/details/goistdong.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.vehdjk.com/Article/details/gmmecuimv.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.yfazqb.com/Article/details/gufmedzrz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.vehdjk.com/Article/details/grgrbzeuq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.bbcook.cn/Article/details/gkzzgkuxq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.epnwcf.com/Article/details/gdgapyznb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.vehdjk.com/Article/details/gesuejvfz.sHtML

[B15] 布尔运算与取反
来源：http://blog.tarul.cn/Article/details/gqbfgklge.sHtML

Py:   a and b or not c
来源：http://3g.bbcook.cn/Article/details/gcaksnltf.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fktsv.cn/Article/details/gdltokirs.sHtML

JS:   a && b || !c
来源：http://baike.vehdjk.com/Article/details/gkxhxlyaa.sHtML

TS:   a && b || !c
来源：http://www.share.fktsv.cn/Article/details/gzrdvilmo.sHtML

Java: a && b || !c
来源：http://3g.epnwcf.com/Article/details/gyupohqdm.sHtML

Go:   a && b || !c
来源：http://3g.vehdjk.com/Article/details/gtrbsimnx.sHtML

Ruby: a && b || !c
来源：http://3g.fktsv.cn/Article/details/gilmxmxql.sHtML

C#:   a && b || !c
来源：http://baike.vehdjk.com/Article/details/gklckriji.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.tarul.cn/Article/details/gvesivigo.sHtML

Py:   if not data: return
来源：http://www.blog.tarul.cn/Article/details/gaporgupp.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.vehdjk.com/Article/details/gnprsnwyc.sHtML

JS:   if (!data) return;
来源：http://www.blog.yfazqb.com/Article/details/giadceivy.sHtML

TS:   if (!data) return;
来源：http://wap.yfazqb.com/Article/details/glaclqwvv.sHtML

Java: if (data == null) return;
来源：http://3g.epnwcf.com/Article/details/gfqplsmlk.sHtML

Go:   if data == nil { return }
来源：http://m.share.vehdjk.com/Article/details/goflmdmkk.sHtML

Ruby: return if data.nil?
来源：http://blog.sjlbkw.cn/Article/details/gecxdhrzi.sHtML

C#:   if (data == null) return;
来源：http://www.share.vehdjk.com/Article/details/gavpvkuco.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gjoqzidsn.sHtML

C. 函数与作用域
来源：http://3g.bbcook.cn/Article/details/gzizmjfju.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gfldhynbv.sHtML

[C01] 定义函数
来源：http://mobile.epnwcf.com/Article/details/grhbpuqua.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.bbcook.cn/Article/details/gtdysbwjk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.tarul.cn/Article/details/glaxcmqev.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gcfgwdbhe.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/grsidvofg.sHtML


<!-- 参考信息 -->