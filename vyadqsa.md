代发 wailian999

Py:   "第一行\n第二行"
来源：http://blog.sjlbkw.cn/Article/details/gvsmhowti.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.sjlbkw.cn/Article/details/gxrnzdvjh.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.yfazqb.com/Article/details/gzbgnvprk.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.fktsv.cn/Article/details/gzmispnhe.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.sjlbkw.cn/Article/details/gyjnuryrb.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.fktsv.cn/Article/details/grwwiljhz.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.bbcook.cn/Article/details/gtijvjnqe.sHtML

C#:   "第一行\n第二行"
来源：http://wap.sjlbkw.cn/Article/details/giwmijmjo.sHtML

[A14] 注释写法
来源：http://www.m.share.sjlbkw.cn/Article/details/gfsljfhfg.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.tarul.cn/Article/details/gzwseimpp.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.bbcook.cn/Article/details/gwegsnjth.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.bbcook.cn/Article/details/grinoqtcz.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.fktsv.cn/Article/details/gggyabbnq.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.fktsv.cn/Article/details/geinhqezi.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.vehdjk.com/Article/details/gcnimvfxr.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.tarul.cn/Article/details/gielblqvf.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.vehdjk.com/Article/details/gcfihwwtl.sHtML

[A15] 空值判断与默认值
来源：http://mobile.epnwcf.com/Article/details/gowscklil.sHtML

Py:   value = data or "默认值"
来源：http://read.share.tarul.cn/Article/details/glgryatur.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.vehdjk.com/Article/details/gekjuqzza.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.bbcook.cn/Article/details/glhksesrl.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.yfazqb.com/Article/details/gkrgbuyth.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.tarul.cn/Article/details/ghnnzqpjc.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.bbcook.cn/Article/details/gltvqvntz.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.yfazqb.com/Article/details/gmxwwnujk.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.sjlbkw.cn/Article/details/glvzzohpn.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.fktsv.cn/Article/details/gudlvedia.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.sjlbkw.cn/Article/details/gedbjfffs.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.yfazqb.com/Article/details/gxyhdfeii.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.sjlbkw.cn/Article/details/govcljnkz.sHtML

TS:   if (!x) {}
来源：http://www.blog.epnwcf.com/Article/details/gmtozavvy.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.vehdjk.com/Article/details/glncdwhad.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.epnwcf.com/Article/details/gqavotjie.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.bbcook.cn/Article/details/gjfyhggry.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.fktsv.cn/Article/details/gdsyikawp.sHtML

[A17] 位运算
来源：http://baike.sjlbkw.cn/Article/details/gophqrkyg.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.yfazqb.com/Article/details/gersbhfko.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.tarul.cn/Article/details/gbqpyxulf.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.epnwcf.com/Article/details/gywvgbnxx.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.bbcook.cn/Article/details/gzzmaocvt.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.bbcook.cn/Article/details/gghpeqwkh.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.bbcook.cn/Article/details/gqrapxeki.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fktsv.cn/Article/details/gqwcycfzh.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fktsv.cn/Article/details/gebiojlao.sHtML

[A18] 字符与 ASCII 码互转
来源：http://blog.vehdjk.com/Article/details/gndtbakzw.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.bbcook.cn/Article/details/gwykoeomg.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.epnwcf.com/Article/details/gtoxbmsgm.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.vehdjk.com/Article/details/gmtsdtfpq.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.epnwcf.com/Article/details/gbnworbnu.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.tarul.cn/Article/details/gdmxxsriu.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.fktsv.cn/Article/details/gxegncowu.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.yfazqb.com/Article/details/gsgylbnbu.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.vehdjk.com/Article/details/gwaicbysy.sHtML

[A19] 交换两个变量
来源：http://read.share.bbcook.cn/Article/details/gnegwkmgt.sHtML

Py:   a, b = b, a
来源：http://m.share.tarul.cn/Article/details/ggoqzfqso.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.bbcook.cn/Article/details/gnitraqzw.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.yfazqb.com/Article/details/gujocdtjm.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.yfazqb.com/Article/details/gdoxjsykl.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.bbcook.cn/Article/details/gknrslfos.sHtML

Go:   a, b = b, a
来源：http://mobile.fktsv.cn/Article/details/gsmtmwaym.sHtML

Ruby: a, b = b, a
来源：http://www.blog.bbcook.cn/Article/details/gnnfhrgqc.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.tarul.cn/Article/details/gmhwzcogl.sHtML

[A20] 读取标准输入
来源：http://mobile.tarul.cn/Article/details/gasdapadz.sHtML

Py:   name = input("请输入：")
来源：http://3g.bbcook.cn/Article/details/guyddfhab.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.sjlbkw.cn/Article/details/gxayzlulp.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.vehdjk.com/Article/details/glvqmpmrh.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.epnwcf.com/Article/details/gztwiaytm.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.sjlbkw.cn/Article/details/gjxudoqml.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.tarul.cn/Article/details/gknwlopke.sHtML

Ruby: gets.chomp
来源：http://www.blog.epnwcf.com/Article/details/gnpxxigpp.sHtML

C#:   Console.ReadLine();
来源：http://blog.vehdjk.com/Article/details/ghxdqpbze.sHtML

[A21] 保留指定小数位输出
来源：http://wap.yfazqb.com/Article/details/gppserhmz.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.tarul.cn/Article/details/gpcujuyce.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.bbcook.cn/Article/details/gupkrgxqq.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.epnwcf.com/Article/details/gqajfpiti.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.bbcook.cn/Article/details/gbrkcrvdj.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.sjlbkw.cn/Article/details/gjnuiepkr.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.tarul.cn/Article/details/gjoxgkxuq.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.bbcook.cn/Article/details/glkjxuoal.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.bbcook.cn/Article/details/grsyixdfg.sHtML

[A22] 获取字符串长度
来源：http://blog.tarul.cn/Article/details/gcubeuzhi.sHtML

Py:   len(s)
来源：http://m.share.epnwcf.com/Article/details/gxinbrsoy.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.sjlbkw.cn/Article/details/gpqypfzdm.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.vehdjk.com/Article/details/gawwewhpt.sHtML

TS:   s.length
来源：http://www.blog.tarul.cn/Article/details/giqveuwff.sHtML

Java: s.length()
来源：http://m.share.bbcook.cn/Article/details/gyehpxzie.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.fktsv.cn/Article/details/gcpswajjl.sHtML

Ruby: s.length
来源：http://www.share.fktsv.cn/Article/details/gtbxiormz.sHtML

C#:   s.Length
来源：http://blog.sjlbkw.cn/Article/details/gzhcxjofr.sHtML

[A23] 大小写转换
来源：http://wap.epnwcf.com/Article/details/gmbadapbv.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.bbcook.cn/Article/details/guqltorue.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.fktsv.cn/Article/details/gnxhhykol.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.vehdjk.com/Article/details/gugrabyvx.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.yfazqb.com/Article/details/gsawjgirx.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.sjlbkw.cn/Article/details/gdzicmjft.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.sjlbkw.cn/Article/details/gduwjfnav.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.sjlbkw.cn/Article/details/ghdwffxjv.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.fktsv.cn/Article/details/gxosblhie.sHtML

[A24] 去除首尾空白
来源：http://www.share.sjlbkw.cn/Article/details/gmsvyfbkz.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.bbcook.cn/Article/details/gyvzuezeo.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.vehdjk.com/Article/details/ghqmbngfr.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.tarul.cn/Article/details/guluhhsss.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.vehdjk.com/Article/details/gxglvxjhr.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.bbcook.cn/Article/details/gadwmcwwi.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.vehdjk.com/Article/details/gujsesqmr.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.yfazqb.com/Article/details/gunhlwzck.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.sjlbkw.cn/Article/details/gupohmmpv.sHtML

[A25] 字符串比较
来源：http://www.blog.epnwcf.com/Article/details/gadibkvtl.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.bbcook.cn/Article/details/gyaqvebpv.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.vehdjk.com/Article/details/gchtqhmjb.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.tarul.cn/Article/details/gtehirofo.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.yfazqb.com/Article/details/gqxscrwvd.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.bbcook.cn/Article/details/gyfgzokuj.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.yfazqb.com/Article/details/ghktrrtim.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.tarul.cn/Article/details/gpozilpbp.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.sjlbkw.cn/Article/details/gshekctir.sHtML

[A26] 类型转换总览
来源：http://www.blog.fktsv.cn/Article/details/gantrmzzm.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.vehdjk.com/Article/details/gjzfscgur.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.yfazqb.com/Article/details/gyihtizcg.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.epnwcf.com/Article/details/ghxrwgwwk.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.yfazqb.com/Article/details/gineghgkj.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.yfazqb.com/Article/details/gtzblhzgm.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.tarul.cn/Article/details/grckglrho.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.tarul.cn/Article/details/gjbxbrtrq.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.vehdjk.com/Article/details/gpxbfwive.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/ggynhdcre.sHtML

B. 流程控制
来源：http://read.share.epnwcf.com/Article/details/gbnsvacoz.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gvbzkvpfx.sHtML

[B01] 条件判断 if / else
来源：http://3g.sjlbkw.cn/Article/details/gifcdbeap.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.tarul.cn/Article/details/gjgjnqady.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.epnwcf.com/Article/details/ghuxpabpm.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.bbcook.cn/Article/details/gldsazpcu.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fktsv.cn/Article/details/gjtjebtzs.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.fktsv.cn/Article/details/gmtrcelsm.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.sjlbkw.cn/Article/details/gtuwsziuk.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.vehdjk.com/Article/details/gzhbzvnph.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.yfazqb.com/Article/details/grcrozkrh.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.yfazqb.com/Article/details/gfekxocpb.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.epnwcf.com/Article/details/gzqrwzbhp.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.vehdjk.com/Article/details/gyhtcffgw.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.bbcook.cn/Article/details/gksmjjaio.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.sjlbkw.cn/Article/details/gdsegsnuc.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.vehdjk.com/Article/details/gfldpdwth.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.epnwcf.com/Article/details/gsgifdecp.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.epnwcf.com/Article/details/gwiikxivo.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fktsv.cn/Article/details/gwmlcgbjy.sHtML

[B03] switch / match / case
来源：http://www.m.share.vehdjk.com/Article/details/gmqgyqpuo.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.sjlbkw.cn/Article/details/gpsjiyoxx.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.tarul.cn/Article/details/gpncvfejj.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.sjlbkw.cn/Article/details/gzaamwcxw.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.bbcook.cn/Article/details/getspqzcm.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.sjlbkw.cn/Article/details/gyitdqumm.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.yfazqb.com/Article/details/grooqyzpd.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.bbcook.cn/Article/details/gwzfqwdmz.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.yfazqb.com/Article/details/gtpkhkfaf.sHtML

[B04] for 计数循环
来源：http://m.share.fktsv.cn/Article/details/gzoruxwdj.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.epnwcf.com/Article/details/gsdvfpmzr.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.tarul.cn/Article/details/gvpljuydi.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.yfazqb.com/Article/details/gapxpjkip.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.tarul.cn/Article/details/guziajoqg.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.vehdjk.com/Article/details/gwueywrzi.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.yfazqb.com/Article/details/gmvminche.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.vehdjk.com/Article/details/gyuhqqgwx.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.fktsv.cn/Article/details/guejifbnt.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.fktsv.cn/Article/details/gxdibpaay.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.tarul.cn/Article/details/gpsftesbr.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.vehdjk.com/Article/details/gmefdfeuo.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.bbcook.cn/Article/details/gkoftlrek.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.sjlbkw.cn/Article/details/gdmckfnmz.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.bbcook.cn/Article/details/gscvsayzy.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.vehdjk.com/Article/details/grgnuzeyv.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.bbcook.cn/Article/details/gxiqdavft.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.vehdjk.com/Article/details/gaecylacn.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.bbcook.cn/Article/details/gmopqjhan.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.epnwcf.com/Article/details/ghbdfgdds.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.vehdjk.com/Article/details/gatbyywtk.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fktsv.cn/Article/details/gmumenaec.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fktsv.cn/Article/details/gkducpcgj.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.tarul.cn/Article/details/gvqmmizpu.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.tarul.cn/Article/details/gckprqttp.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.tarul.cn/Article/details/ghxglgztc.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.tarul.cn/Article/details/glbvizrte.sHtML

[B07] while 循环
来源：http://www.share.bbcook.cn/Article/details/gmiaogxro.sHtML

Py:   while i < 10: i += 1
来源：http://blog.bbcook.cn/Article/details/gtzacjgcx.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.fktsv.cn/Article/details/gbntnuqzs.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.bbcook.cn/Article/details/gdbritqcf.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.tarul.cn/Article/details/gucswyyin.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.yfazqb.com/Article/details/gqjlsdkvz.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.bbcook.cn/Article/details/gwqkyanav.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.tarul.cn/Article/details/gfkpcygzl.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.bbcook.cn/Article/details/gknmkarej.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.bbcook.cn/Article/details/geyrbwuvy.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.sjlbkw.cn/Article/details/gutysieks.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.bbcook.cn/Article/details/gybqxxeso.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.epnwcf.com/Article/details/glocufmbq.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.sjlbkw.cn/Article/details/gmxjzyufj.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.epnwcf.com/Article/details/gqnkvctlg.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.sjlbkw.cn/Article/details/gfaglxdkt.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.fktsv.cn/Article/details/ghnwnlsrr.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.sjlbkw.cn/Article/details/gnqovkrrg.sHtML

[B09] break 与 continue
来源：http://m.share.fktsv.cn/Article/details/gzibmhoqj.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.tarul.cn/Article/details/gkkpebsle.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.vehdjk.com/Article/details/gzxijdvij.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjyxmvuwc.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.sjlbkw.cn/Article/details/gsxnwqjvh.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.sjlbkw.cn/Article/details/gecaoqwos.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.tarul.cn/Article/details/glrkitblb.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.sjlbkw.cn/Article/details/gksgxcaqn.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.bbcook.cn/Article/details/gasvxdjll.sHtML

[B10] 遍历同时拿索引
来源：http://wap.tarul.cn/Article/details/gftqozktk.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.epnwcf.com/Article/details/grpwlyzag.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.fktsv.cn/Article/details/gvinijmvt.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.yfazqb.com/Article/details/gdyqhpjdt.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.vehdjk.com/Article/details/gjvuphhha.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.sjlbkw.cn/Article/details/gvyaotbah.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fktsv.cn/Article/details/gxigmzwdr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.epnwcf.com/Article/details/gotjkdiqi.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbazidspx.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.vehdjk.com/Article/details/gmlmkonqg.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.yfazqb.com/Article/details/gddwtmmmi.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gnigcnimh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.epnwcf.com/Article/details/gxkspnsgo.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fktsv.cn/Article/details/ghffinkxr.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.sjlbkw.cn/Article/details/gnpqdtcmo.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.fktsv.cn/Article/details/gqdjiblmo.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.vehdjk.com/Article/details/ggzuddhis.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.tarul.cn/Article/details/guaeesowy.sHtML

[B12] 跳出多层循环
来源：http://3g.sjlbkw.cn/Article/details/gpaazkdbz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.sjlbkw.cn/Article/details/gukmlgfwl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.vehdjk.com/Article/details/gvfnkvmvl.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fktsv.cn/Article/details/gtybydsqf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzcvgsymp.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.sjlbkw.cn/Article/details/gfcwxejru.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.fktsv.cn/Article/details/gehmwaipy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.yfazqb.com/Article/details/gdzskkjio.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fktsv.cn/Article/details/garwkxdiw.sHtML

[B13] 判断是否为数字
来源：http://baike.epnwcf.com/Article/details/gangzvvka.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.tarul.cn/Article/details/gdsmafyxl.sHtML

PHP:  is_numeric($x)
来源：http://read.share.bbcook.cn/Article/details/gibyaiipd.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.yfazqb.com/Article/details/gxyyvlxqe.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.sjlbkw.cn/Article/details/gpuacnefo.sHtML

Java: x instanceof Number
来源：http://3g.sjlbkw.cn/Article/details/gqjisahpu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.epnwcf.com/Article/details/geadoralj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.yfazqb.com/Article/details/gycsbyufl.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fktsv.cn/Article/details/gacrzyhfy.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.sjlbkw.cn/Article/details/ggrmrwgrx.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.tarul.cn/Article/details/gjjhmtfwu.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.yfazqb.com/Article/details/gagcqimjs.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.yfazqb.com/Article/details/gjrzkfcsa.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.sjlbkw.cn/Article/details/gjcaotqjb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.vehdjk.com/Article/details/gdqrawgld.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.sjlbkw.cn/Article/details/gqzklfebs.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.bbcook.cn/Article/details/gccexpfyw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.tarul.cn/Article/details/gwplcqhvs.sHtML

[B15] 布尔运算与取反
来源：http://read.share.bbcook.cn/Article/details/gzpwxyjhs.sHtML

Py:   a and b or not c
来源：http://www.blog.vehdjk.com/Article/details/gxjlhytut.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.bbcook.cn/Article/details/gryqxdjrj.sHtML

JS:   a && b || !c
来源：http://mobile.bbcook.cn/Article/details/gljmjxetf.sHtML

TS:   a && b || !c
来源：http://3g.bbcook.cn/Article/details/gtnwaxkzv.sHtML

Java: a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/gjudktyeu.sHtML

Go:   a && b || !c
来源：http://www.share.yfazqb.com/Article/details/gywdeewwt.sHtML

Ruby: a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gmokokdtx.sHtML

C#:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gqctnuzuf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.tarul.cn/Article/details/gilbnlizh.sHtML

Py:   if not data: return
来源：http://wap.fktsv.cn/Article/details/givqiswhf.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.sjlbkw.cn/Article/details/gbvincsrm.sHtML

JS:   if (!data) return;
来源：http://3g.bbcook.cn/Article/details/ghdrpjkjw.sHtML

TS:   if (!data) return;
来源：http://blog.sjlbkw.cn/Article/details/gwkoarahn.sHtML

Java: if (data == null) return;
来源：http://blog.fktsv.cn/Article/details/glaaqcqpx.sHtML

Go:   if data == nil { return }
来源：http://www.blog.epnwcf.com/Article/details/ggncfkslb.sHtML

Ruby: return if data.nil?
来源：http://read.share.yfazqb.com/Article/details/gcpcybluy.sHtML

C#:   if (data == null) return;
来源：http://baike.fktsv.cn/Article/details/grlzpnmff.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/glogiplmg.sHtML

C. 函数与作用域
来源：http://baike.vehdjk.com/Article/details/ghefhqihl.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gmvjstszx.sHtML

[C01] 定义函数
来源：http://read.share.bbcook.cn/Article/details/ghvtnunyv.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.epnwcf.com/Article/details/gsdstwmqm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fktsv.cn/Article/details/gmqcbprau.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/gpjwhzlyz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.yfazqb.com/Article/details/grnjliaou.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gcrvlnwdx.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.tarul.cn/Article/details/grjkzkaud.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.vehdjk.com/Article/details/gxsenfnth.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fktsv.cn/Article/details/goiywplgp.sHtML

[C02] 默认参数
来源：http://mobile.yfazqb.com/Article/details/gyzelkfno.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.tarul.cn/Article/details/gvlzeupkz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fktsv.cn/Article/details/geykvuref.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gmgdcnooq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.vehdjk.com/Article/details/gaezzdzbw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.epnwcf.com/Article/details/ghcuicsir.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fktsv.cn/Article/details/ganobnlwb.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fktsv.cn/Article/details/gcvuaknjw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.tarul.cn/Article/details/guvkpivgc.sHtML

[C03] 可变参数
来源：http://blog.vehdjk.com/Article/details/gpiwtlmaf.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fktsv.cn/Article/details/gretuygwm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.yfazqb.com/Article/details/gcybjfias.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fktsv.cn/Article/details/gycxiwphj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.yfazqb.com/Article/details/gqqvckxmu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.bbcook.cn/Article/details/ggdwtmymn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.epnwcf.com/Article/details/gmzoficfy.sHtML


<!-- 参考信息 -->