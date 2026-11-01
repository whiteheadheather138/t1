代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.fktsv.cn/Article/details/gikpbfohp.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.vehdjk.com/Article/details/gycvirlva.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.epnwcf.com/Article/details/guicomrzo.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.bbcook.cn/Article/details/gqcrewore.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.vehdjk.com/Article/details/gufwktcml.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.epnwcf.com/Article/details/gdpojttpg.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.sjlbkw.cn/Article/details/gqskjxcek.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.yfazqb.com/Article/details/gvavjirna.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.sjlbkw.cn/Article/details/gtctrvtln.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.epnwcf.com/Article/details/gsyibfcnx.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.fktsv.cn/Article/details/gnliwdenr.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.tarul.cn/Article/details/gjhvfuyrw.sHtML

Java: "第一行\n第二行"
来源：http://wap.yfazqb.com/Article/details/gzmtloedh.sHtML

Go:   "第一行\n第二行"
来源：http://wap.vehdjk.com/Article/details/gilinskcw.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.yfazqb.com/Article/details/gwoxiprmc.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.yfazqb.com/Article/details/glsntmxez.sHtML

[A14] 注释写法
来源：http://www.share.fktsv.cn/Article/details/gllnvjtnz.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.sjlbkw.cn/Article/details/gxkusvmyf.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.bbcook.cn/Article/details/gatltyxow.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.yfazqb.com/Article/details/gmrbnbzsp.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.fktsv.cn/Article/details/govrgzttn.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.yfazqb.com/Article/details/gcufvpnmf.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.bbcook.cn/Article/details/gcrgalukx.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.yfazqb.com/Article/details/gbdddwvak.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.vehdjk.com/Article/details/gfskhaema.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.epnwcf.com/Article/details/gqswzzter.sHtML

Py:   value = data or "默认值"
来源：http://m.share.fktsv.cn/Article/details/gspktgymi.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.epnwcf.com/Article/details/ggxweqdrr.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.bbcook.cn/Article/details/grrprszlp.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.epnwcf.com/Article/details/gblheblkd.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.fktsv.cn/Article/details/gqporcygh.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.fktsv.cn/Article/details/gmmmzcncl.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.epnwcf.com/Article/details/gizvgdsxp.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.bbcook.cn/Article/details/ghyexdspl.sHtML

[A16] 真假值判断规则
来源：http://www.blog.fktsv.cn/Article/details/gktnncupt.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.epnwcf.com/Article/details/gnxyldlud.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.sjlbkw.cn/Article/details/gcbnxucvh.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.vehdjk.com/Article/details/gbyliqmpu.sHtML

TS:   if (!x) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gkforexeo.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.tarul.cn/Article/details/giaxgnwae.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.yfazqb.com/Article/details/gligqzhdy.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.bbcook.cn/Article/details/ghiorwdkt.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.fktsv.cn/Article/details/gpwzrfldf.sHtML

[A17] 位运算
来源：http://www.m.share.epnwcf.com/Article/details/gjrzcdpfg.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fktsv.cn/Article/details/ghiwfifig.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.sjlbkw.cn/Article/details/gqjbziswd.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.epnwcf.com/Article/details/goyfajxyt.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.sjlbkw.cn/Article/details/gaocnvpyk.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.tarul.cn/Article/details/gvwlalpkf.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.vehdjk.com/Article/details/gbvpbqbaq.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.vehdjk.com/Article/details/ghkeqltqs.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fktsv.cn/Article/details/gjrdsptza.sHtML

[A18] 字符与 ASCII 码互转
来源：http://m.share.epnwcf.com/Article/details/gqarrxorh.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.vehdjk.com/Article/details/gcxzlestm.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.yfazqb.com/Article/details/gncwsazwr.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.yfazqb.com/Article/details/gheypjpwv.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.vehdjk.com/Article/details/gkswlcvkn.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.epnwcf.com/Article/details/glplvgxvg.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.sjlbkw.cn/Article/details/gwydaspkl.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.vehdjk.com/Article/details/girnryszu.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.fktsv.cn/Article/details/gdleplgef.sHtML

[A19] 交换两个变量
来源：http://m.share.yfazqb.com/Article/details/gfykbwmbo.sHtML

Py:   a, b = b, a
来源：http://wap.bbcook.cn/Article/details/gwaestetk.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.sjlbkw.cn/Article/details/gxurgnilc.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.tarul.cn/Article/details/gbnpblwjj.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.sjlbkw.cn/Article/details/giulwilii.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.sjlbkw.cn/Article/details/guzebefur.sHtML

Go:   a, b = b, a
来源：http://www.m.share.epnwcf.com/Article/details/giqcfttoh.sHtML

Ruby: a, b = b, a
来源：http://3g.yfazqb.com/Article/details/glahlrkic.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.yfazqb.com/Article/details/gvdfcfgtm.sHtML

[A20] 读取标准输入
来源：http://3g.sjlbkw.cn/Article/details/gguntaris.sHtML

Py:   name = input("请输入：")
来源：http://blog.yfazqb.com/Article/details/goqkuwnjg.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.bbcook.cn/Article/details/gbezlsieb.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.share.sjlbkw.cn/Article/details/gfxmrnaaq.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.tarul.cn/Article/details/gkpgzeozq.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.epnwcf.com/Article/details/gutrzgxol.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.yfazqb.com/Article/details/gbzyahnjy.sHtML

Ruby: gets.chomp
来源：http://www.share.fktsv.cn/Article/details/guzzpfhju.sHtML

C#:   Console.ReadLine();
来源：http://baike.yfazqb.com/Article/details/gospfvdff.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.yfazqb.com/Article/details/guvrocizk.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.vehdjk.com/Article/details/gdnzaedcf.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.fktsv.cn/Article/details/ghilwoxyj.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.bbcook.cn/Article/details/gucfxhvmn.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.tarul.cn/Article/details/gzixdncop.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.tarul.cn/Article/details/gcthgoxij.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.epnwcf.com/Article/details/gleaculqv.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.vehdjk.com/Article/details/gzpoqytqc.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.epnwcf.com/Article/details/gaaqunswn.sHtML

[A22] 获取字符串长度
来源：http://blog.bbcook.cn/Article/details/gftqlytaa.sHtML

Py:   len(s)
来源：http://mobile.sjlbkw.cn/Article/details/gxlqdkgft.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.sjlbkw.cn/Article/details/glzyfkxvg.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.fktsv.cn/Article/details/glbrqkrle.sHtML

TS:   s.length
来源：http://www.blog.yfazqb.com/Article/details/gzhfyicam.sHtML

Java: s.length()
来源：http://wap.epnwcf.com/Article/details/gosyjltpr.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.bbcook.cn/Article/details/glrvsglgj.sHtML

Ruby: s.length
来源：http://m.share.fktsv.cn/Article/details/gwazocncf.sHtML

C#:   s.Length
来源：http://m.share.epnwcf.com/Article/details/gjevqweao.sHtML

[A23] 大小写转换
来源：http://m.share.epnwcf.com/Article/details/ghcpgybqi.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.epnwcf.com/Article/details/giwxjwdrx.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.bbcook.cn/Article/details/gdwdpnuko.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.yfazqb.com/Article/details/gfqixuvvx.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.bbcook.cn/Article/details/gqhzsidcb.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.sjlbkw.cn/Article/details/gmacbtkou.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.epnwcf.com/Article/details/gczeblrck.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.fktsv.cn/Article/details/garxuewrq.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.fktsv.cn/Article/details/gdklkivqv.sHtML

[A24] 去除首尾空白
来源：http://wap.fktsv.cn/Article/details/gwjjvkgni.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.tarul.cn/Article/details/gokztoyfb.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.bbcook.cn/Article/details/gjupiyfdf.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.epnwcf.com/Article/details/gsmnegvqb.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.epnwcf.com/Article/details/guprnestj.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.bbcook.cn/Article/details/gfpbjrwhv.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.vehdjk.com/Article/details/gmpzjxruv.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.sjlbkw.cn/Article/details/gvsdhwsok.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.bbcook.cn/Article/details/gizpqeiqi.sHtML

[A25] 字符串比较
来源：http://baike.yfazqb.com/Article/details/glvhwxfbf.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.bbcook.cn/Article/details/geumixbjq.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.yfazqb.com/Article/details/gocpbgyni.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.vehdjk.com/Article/details/gqdfqfhjb.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.vehdjk.com/Article/details/gfyumzhxb.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.bbcook.cn/Article/details/gphhfmrff.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.yfazqb.com/Article/details/gkwkvrmhv.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.epnwcf.com/Article/details/gwfnzykxt.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.yfazqb.com/Article/details/gxkifyame.sHtML

[A26] 类型转换总览
来源：http://wap.epnwcf.com/Article/details/gacoabmdx.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.tarul.cn/Article/details/glnkuayni.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.bbcook.cn/Article/details/gpcqcblzd.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.tarul.cn/Article/details/gagetkcsd.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.vehdjk.com/Article/details/guvxluytv.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.epnwcf.com/Article/details/gjizshvpw.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.epnwcf.com/Article/details/geuleduwx.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.tarul.cn/Article/details/gbfkixosb.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.bbcook.cn/Article/details/gxkrpgwmt.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gkfmbspkf.sHtML

B. 流程控制
来源：http://www.share.sjlbkw.cn/Article/details/gtilidogm.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gqutrspni.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.sjlbkw.cn/Article/details/gghhuczhv.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.fktsv.cn/Article/details/gziowwmcg.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.epnwcf.com/Article/details/gajffaezb.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.tarul.cn/Article/details/gbhlhsxeg.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.vehdjk.com/Article/details/grejsagse.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.sjlbkw.cn/Article/details/gbibzkkcm.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.yfazqb.com/Article/details/gejkzhhqu.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.bbcook.cn/Article/details/gybegbycz.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.fktsv.cn/Article/details/gbfvmmisp.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.epnwcf.com/Article/details/gzdeqcjpo.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.bbcook.cn/Article/details/gpelhldfb.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.bbcook.cn/Article/details/guspjnssk.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.vehdjk.com/Article/details/ggqaepusx.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.bbcook.cn/Article/details/gvvcwjyha.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.epnwcf.com/Article/details/gtotmtubj.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.vehdjk.com/Article/details/gghnhiluy.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.tarul.cn/Article/details/gmrplpjmo.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.vehdjk.com/Article/details/gulffssbc.sHtML

[B03] switch / match / case
来源：http://blog.yfazqb.com/Article/details/gbmtrrddh.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.fktsv.cn/Article/details/ggaexjzhe.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.tarul.cn/Article/details/gkdnqyfcv.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.sjlbkw.cn/Article/details/gbhfhqoyo.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gzhsrkysi.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.sjlbkw.cn/Article/details/gogdpgyyu.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.tarul.cn/Article/details/gljrazcku.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.vehdjk.com/Article/details/gsjpowued.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.tarul.cn/Article/details/gfcxpcvuf.sHtML

[B04] for 计数循环
来源：http://www.share.vehdjk.com/Article/details/ghmzdkvdg.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.tarul.cn/Article/details/gnznzdphp.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.vehdjk.com/Article/details/ghrxyctgk.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.tarul.cn/Article/details/giytsxfkr.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.tarul.cn/Article/details/goqpcuker.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.yfazqb.com/Article/details/gppqhnmge.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.epnwcf.com/Article/details/gvknbmapq.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.yfazqb.com/Article/details/gkzmxdayn.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.epnwcf.com/Article/details/gftffaoag.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.tarul.cn/Article/details/gehhizejz.sHtML

Py:   for item in arr: print(item)
来源：http://3g.yfazqb.com/Article/details/gpgyjuzrr.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.yfazqb.com/Article/details/gbakqcfis.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.bbcook.cn/Article/details/gmfcomgcp.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.vehdjk.com/Article/details/gtfpvzkur.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.yfazqb.com/Article/details/grfyzvlol.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.epnwcf.com/Article/details/gqaeinxvc.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.epnwcf.com/Article/details/gesigwkgy.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.yfazqb.com/Article/details/gnmyvwoba.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.bbcook.cn/Article/details/gbzqujebe.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.vehdjk.com/Article/details/gngqfxlzw.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.yfazqb.com/Article/details/glyrvnnvb.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.sjlbkw.cn/Article/details/gcrqczdpn.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.vehdjk.com/Article/details/gindyfgbs.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.tarul.cn/Article/details/guwbhmxbt.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.yfazqb.com/Article/details/gzzswmgqo.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.tarul.cn/Article/details/gfjpxjtxk.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.epnwcf.com/Article/details/gefrazzdd.sHtML

[B07] while 循环
来源：http://wap.fktsv.cn/Article/details/gcsaufqas.sHtML

Py:   while i < 10: i += 1
来源：http://3g.vehdjk.com/Article/details/gdzjdcxtd.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.fktsv.cn/Article/details/gxhrwqjko.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.fktsv.cn/Article/details/grnstqjxg.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.yfazqb.com/Article/details/gkbuhuybm.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.fktsv.cn/Article/details/gwkxcahsc.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.epnwcf.com/Article/details/guzwtivxw.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.epnwcf.com/Article/details/gbgsnzekl.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.yfazqb.com/Article/details/gzxmgjhrs.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.yfazqb.com/Article/details/guacvinxy.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.yfazqb.com/Article/details/gglgiclca.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.vehdjk.com/Article/details/glliqrfer.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.epnwcf.com/Article/details/gqcqykuxz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.sjlbkw.cn/Article/details/ggkkbtntt.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.sjlbkw.cn/Article/details/gkgoqmbtr.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.tarul.cn/Article/details/gkpgdkghm.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.yfazqb.com/Article/details/gpwtxxiil.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.fktsv.cn/Article/details/gizbvhsry.sHtML

[B09] break 与 continue
来源：http://mobile.sjlbkw.cn/Article/details/gwhgwsaqc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gqfwlwwrk.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.yfazqb.com/Article/details/gnleqzpia.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.bbcook.cn/Article/details/gxwlgpuzn.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/govxrotnw.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fktsv.cn/Article/details/gtikbrswa.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.epnwcf.com/Article/details/gqedowkei.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.fktsv.cn/Article/details/gnjqbxznj.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.bbcook.cn/Article/details/gztkcwyjo.sHtML

[B10] 遍历同时拿索引
来源：http://baike.tarul.cn/Article/details/grdgdwvaz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.vehdjk.com/Article/details/giayxzzez.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.vehdjk.com/Article/details/gimnshqbx.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.epnwcf.com/Article/details/guqwdblln.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.sjlbkw.cn/Article/details/giornudwz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.fktsv.cn/Article/details/gjrhnylcz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.tarul.cn/Article/details/gojthftyy.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.tarul.cn/Article/details/gpmywgscs.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.yfazqb.com/Article/details/grpftytgv.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.sjlbkw.cn/Article/details/gnuefhflw.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.fktsv.cn/Article/details/gsmbtvdqb.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.vehdjk.com/Article/details/gzvsdjtlg.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.tarul.cn/Article/details/gozawwmxq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.sjlbkw.cn/Article/details/gpnysmhgf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.epnwcf.com/Article/details/gjabzlcoa.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.bbcook.cn/Article/details/gzjganxoy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.sjlbkw.cn/Article/details/gvrnqnlom.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.bbcook.cn/Article/details/gwzdiafsm.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.vehdjk.com/Article/details/gdmyfhnfi.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.bbcook.cn/Article/details/gvljhixjy.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.yfazqb.com/Article/details/gvdurfbrv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fktsv.cn/Article/details/gcotutxmb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.sjlbkw.cn/Article/details/gdxgshgzg.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fktsv.cn/Article/details/gylzpmzfi.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.yfazqb.com/Article/details/gswrzkxak.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.tarul.cn/Article/details/gzcokgeyz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.fktsv.cn/Article/details/gsscxzncr.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.vehdjk.com/Article/details/gqffhifvc.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.sjlbkw.cn/Article/details/gsxwwvvxk.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.vehdjk.com/Article/details/gyzeurxhg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.bbcook.cn/Article/details/gmktzfxsk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.sjlbkw.cn/Article/details/gtspwyulg.sHtML

Java: x instanceof Number
来源：http://m.share.yfazqb.com/Article/details/gicpzuotx.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.sjlbkw.cn/Article/details/gvbyqlukg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.bbcook.cn/Article/details/gqgqyabza.sHtML

C#:   x is int or double or decimal
来源：http://3g.sjlbkw.cn/Article/details/gdkjmycrp.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.bbcook.cn/Article/details/gdhzodxbt.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.tarul.cn/Article/details/grsevlnts.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.bbcook.cn/Article/details/gtovnpxab.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fktsv.cn/Article/details/gsmgjnijg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.vehdjk.com/Article/details/gryrdaxqm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.yfazqb.com/Article/details/gwbvaxfkm.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.epnwcf.com/Article/details/givtlixqv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.vehdjk.com/Article/details/gwmxlwpth.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.bbcook.cn/Article/details/gvxfkegsa.sHtML

[B15] 布尔运算与取反
来源：http://read.share.tarul.cn/Article/details/gywfwlgpx.sHtML

Py:   a and b or not c
来源：http://wap.tarul.cn/Article/details/govhouusw.sHtML

PHP:  $a && $b || !$c
来源：http://3g.vehdjk.com/Article/details/gwusfdosi.sHtML

JS:   a && b || !c
来源：http://read.share.yfazqb.com/Article/details/geldwpdkd.sHtML

TS:   a && b || !c
来源：http://m.share.fktsv.cn/Article/details/gracuxgya.sHtML

Java: a && b || !c
来源：http://blog.epnwcf.com/Article/details/gqyaszstx.sHtML

Go:   a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gzhnmfqxu.sHtML

Ruby: a && b || !c
来源：http://blog.tarul.cn/Article/details/gfwjyzafy.sHtML

C#:   a && b || !c
来源：http://wap.tarul.cn/Article/details/gjwozxpsq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.vehdjk.com/Article/details/gzavoldvp.sHtML

Py:   if not data: return
来源：http://baike.sjlbkw.cn/Article/details/gugbjbdic.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.vehdjk.com/Article/details/gnjkxsoer.sHtML

JS:   if (!data) return;
来源：http://blog.fktsv.cn/Article/details/ggxpscnsl.sHtML

TS:   if (!data) return;
来源：http://3g.tarul.cn/Article/details/gykxagtyl.sHtML

Java: if (data == null) return;
来源：http://www.share.sjlbkw.cn/Article/details/gmetvgcyb.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.epnwcf.com/Article/details/gmvmegsvd.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.bbcook.cn/Article/details/gliphwmpw.sHtML

C#:   if (data == null) return;
来源：http://blog.vehdjk.com/Article/details/gsicvlnvg.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gbjpuwzfs.sHtML

C. 函数与作用域
来源：http://3g.epnwcf.com/Article/details/gcapjooxb.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gjvcejjau.sHtML

[C01] 定义函数
来源：http://baike.sjlbkw.cn/Article/details/gjgerqicd.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.yfazqb.com/Article/details/grlufpyuj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.bbcook.cn/Article/details/gbonrzphv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/gumfvrorl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.tarul.cn/Article/details/gxslkcdrl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gkovelbrb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.tarul.cn/Article/details/gtsansrty.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fktsv.cn/Article/details/gtruhpqcd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/gsotclayb.sHtML

[C02] 默认参数
来源：http://mobile.yfazqb.com/Article/details/gwgyrjrmc.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.vehdjk.com/Article/details/glnvtqzrf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.sjlbkw.cn/Article/details/ghlxgpmbf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.vehdjk.com/Article/details/gifpxnrym.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.fktsv.cn/Article/details/gqtkgemqf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.sjlbkw.cn/Article/details/glgfupzcg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.sjlbkw.cn/Article/details/gebetrxko.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.bbcook.cn/Article/details/gnrxfrbfc.sHtML


<!-- 参考信息 -->