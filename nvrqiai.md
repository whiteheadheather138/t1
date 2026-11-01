代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.bbcook.cn/Article/details/gioefgvgd.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.sjlbkw.cn/Article/details/gnpnclghz.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.bbcook.cn/Article/details/gagkqtmhw.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.tarul.cn/Article/details/ggnbuqqjt.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.yfazqb.com/Article/details/gwmhiheuo.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.yfazqb.com/Article/details/gcdbbmakm.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.sjlbkw.cn/Article/details/gbksoruvb.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.yfazqb.com/Article/details/gqvehxsrs.sHtML

Py:   "第一行\n第二行"
来源：http://wap.epnwcf.com/Article/details/gecjaasei.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.bbcook.cn/Article/details/gngrjpjdg.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.yfazqb.com/Article/details/gebythqmk.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.tarul.cn/Article/details/ggoykrxtp.sHtML

Java: "第一行\n第二行"
来源：http://read.share.epnwcf.com/Article/details/gdwxylyfd.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.sjlbkw.cn/Article/details/gtfwfxvem.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.tarul.cn/Article/details/gygxlyxfz.sHtML

C#:   "第一行\n第二行"
来源：http://3g.sjlbkw.cn/Article/details/gexhlzvrx.sHtML

[A14] 注释写法
来源：http://www.blog.fktsv.cn/Article/details/goetwvzan.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.tarul.cn/Article/details/gsfgxqbmz.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.vehdjk.com/Article/details/gnvctpwon.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.fktsv.cn/Article/details/gxsshyhmu.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.epnwcf.com/Article/details/gghghukpt.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.vehdjk.com/Article/details/gczkrkblp.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.vehdjk.com/Article/details/gikhlfioh.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.vehdjk.com/Article/details/gyesrbpwk.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.vehdjk.com/Article/details/gvyuhnwfn.sHtML

[A15] 空值判断与默认值
来源：http://3g.tarul.cn/Article/details/glffbwmcq.sHtML

Py:   value = data or "默认值"
来源：http://www.share.vehdjk.com/Article/details/gwldontfk.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.vehdjk.com/Article/details/gcpjlthcf.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.vehdjk.com/Article/details/gqbtxeole.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.yfazqb.com/Article/details/gvfbocoqy.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.vehdjk.com/Article/details/gjxyfmjkt.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.bbcook.cn/Article/details/gqfdnnfpv.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.vehdjk.com/Article/details/gnkuaysiw.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.bbcook.cn/Article/details/gbyckgttr.sHtML

[A16] 真假值判断规则
来源：http://www.blog.bbcook.cn/Article/details/gzelnfxeb.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.sjlbkw.cn/Article/details/goczfkquq.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.vehdjk.com/Article/details/ggmipkfyo.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.tarul.cn/Article/details/glmvqpmwa.sHtML

TS:   if (!x) {}
来源：http://read.share.epnwcf.com/Article/details/gjxnbvatp.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.fktsv.cn/Article/details/gmbeqvznc.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.bbcook.cn/Article/details/gbhevrszc.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.fktsv.cn/Article/details/ghgiynhzg.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.fktsv.cn/Article/details/geemaiyej.sHtML

[A17] 位运算
来源：http://read.share.epnwcf.com/Article/details/gitobazzc.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.yfazqb.com/Article/details/gvfmeicap.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.epnwcf.com/Article/details/gmitavcts.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.tarul.cn/Article/details/gtgmkxwog.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.yfazqb.com/Article/details/gydfbqiwy.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.yfazqb.com/Article/details/ggeehbahc.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.epnwcf.com/Article/details/gstewtssd.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gtbzimfpr.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.bbcook.cn/Article/details/grkxsxzwv.sHtML

[A18] 字符与 ASCII 码互转
来源：http://m.share.bbcook.cn/Article/details/gqkxrmcek.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.yfazqb.com/Article/details/giagcqknt.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.tarul.cn/Article/details/gwlwpalhf.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnwvumwck.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.fktsv.cn/Article/details/gtgpfedcb.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.bbcook.cn/Article/details/gbpyxdeoi.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.sjlbkw.cn/Article/details/glpfruqsx.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.bbcook.cn/Article/details/gdqvzbifh.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.fktsv.cn/Article/details/guulasies.sHtML

[A19] 交换两个变量
来源：http://wap.yfazqb.com/Article/details/gaddclowj.sHtML

Py:   a, b = b, a
来源：http://www.blog.vehdjk.com/Article/details/gvbpzfotv.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.yfazqb.com/Article/details/gemsaztqi.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.tarul.cn/Article/details/gqrrcrckp.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.tarul.cn/Article/details/gtkaujhnb.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.epnwcf.com/Article/details/gytjottte.sHtML

Go:   a, b = b, a
来源：http://blog.yfazqb.com/Article/details/gzuvhgtjp.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.epnwcf.com/Article/details/genyykgpx.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.yfazqb.com/Article/details/gtyvmmbtc.sHtML

[A20] 读取标准输入
来源：http://blog.yfazqb.com/Article/details/goxyxvoze.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.sjlbkw.cn/Article/details/gdstujchw.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.tarul.cn/Article/details/gyxltuqsh.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.vehdjk.com/Article/details/gyxviiibn.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.vehdjk.com/Article/details/gobegiyfu.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.epnwcf.com/Article/details/gzojfztrj.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.bbcook.cn/Article/details/gzeqzgrig.sHtML

Ruby: gets.chomp
来源：http://3g.tarul.cn/Article/details/gmfuogvqo.sHtML

C#:   Console.ReadLine();
来源：http://baike.fktsv.cn/Article/details/gjylcuzby.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.fktsv.cn/Article/details/geizagrrb.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.bbcook.cn/Article/details/gjvqiusmq.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.epnwcf.com/Article/details/gdwrqhgum.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.yfazqb.com/Article/details/gogggjazo.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.bbcook.cn/Article/details/gpgvgldqg.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.tarul.cn/Article/details/gwywkaqax.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.bbcook.cn/Article/details/gsldtczul.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.fktsv.cn/Article/details/gktrorgoz.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.fktsv.cn/Article/details/gehlwazbs.sHtML

[A22] 获取字符串长度
来源：http://m.share.yfazqb.com/Article/details/glqrnbpav.sHtML

Py:   len(s)
来源：http://www.m.share.epnwcf.com/Article/details/gscyxglac.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.vehdjk.com/Article/details/gtmxjrtec.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.fktsv.cn/Article/details/gzxachbwb.sHtML

TS:   s.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gpapaaohs.sHtML

Java: s.length()
来源：http://baike.fktsv.cn/Article/details/gczcpfqqx.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.bbcook.cn/Article/details/gyryvayjd.sHtML

Ruby: s.length
来源：http://www.blog.vehdjk.com/Article/details/gfzkdkyxr.sHtML

C#:   s.Length
来源：http://baike.bbcook.cn/Article/details/garqmpwyy.sHtML

[A23] 大小写转换
来源：http://read.share.vehdjk.com/Article/details/gljkhcluk.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.yfazqb.com/Article/details/gyzucjwoa.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.bbcook.cn/Article/details/gfgweymcc.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.yfazqb.com/Article/details/ghicdvatr.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.bbcook.cn/Article/details/govtrewpd.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.sjlbkw.cn/Article/details/gkjiqvieb.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.epnwcf.com/Article/details/gxqjkjxrh.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.bbcook.cn/Article/details/gqlbmtaed.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.vehdjk.com/Article/details/gdeuvbyre.sHtML

[A24] 去除首尾空白
来源：http://read.share.fktsv.cn/Article/details/gufrkmtmp.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.vehdjk.com/Article/details/gmyybhlat.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.epnwcf.com/Article/details/gwqnujxpb.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.epnwcf.com/Article/details/gwelkcfrt.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fktsv.cn/Article/details/gjjfjzxtm.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.fktsv.cn/Article/details/gdcqgxnei.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.fktsv.cn/Article/details/gzkfhqxcl.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.vehdjk.com/Article/details/gdgypfles.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.sjlbkw.cn/Article/details/gnrodzmwl.sHtML

[A25] 字符串比较
来源：http://mobile.bbcook.cn/Article/details/gmzsphrne.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.bbcook.cn/Article/details/giepnhesm.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.vehdjk.com/Article/details/glnkpjkbm.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.yfazqb.com/Article/details/gfnrykdvk.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.sjlbkw.cn/Article/details/gajtmnkrb.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.fktsv.cn/Article/details/gadicaxmm.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.fktsv.cn/Article/details/gadghotid.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.epnwcf.com/Article/details/gqeyqrrns.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.fktsv.cn/Article/details/gvamrejkt.sHtML

[A26] 类型转换总览
来源：http://m.share.sjlbkw.cn/Article/details/gffbufkop.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.yfazqb.com/Article/details/guolpqfec.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.epnwcf.com/Article/details/glcocijqa.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.fktsv.cn/Article/details/gldaptmbu.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.epnwcf.com/Article/details/gtyakzuat.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.yfazqb.com/Article/details/gopqluaqo.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.sjlbkw.cn/Article/details/ggcawcaqn.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.bbcook.cn/Article/details/gffdfrzws.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.yfazqb.com/Article/details/gqsjfilyr.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gmmaapqhy.sHtML

B. 流程控制
来源：http://read.share.vehdjk.com/Article/details/gfoqrudmy.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gjdlhlvvo.sHtML

[B01] 条件判断 if / else
来源：http://baike.tarul.cn/Article/details/gopcvvrrt.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.yfazqb.com/Article/details/gwdfipocp.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.tarul.cn/Article/details/gufcixlqm.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.sjlbkw.cn/Article/details/gebulnkjf.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.yfazqb.com/Article/details/geajrbbtu.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.tarul.cn/Article/details/gdhbuhejt.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.vehdjk.com/Article/details/gwestkytf.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.vehdjk.com/Article/details/gbiukbptz.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.sjlbkw.cn/Article/details/gtcmkpzmj.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.epnwcf.com/Article/details/gcxwigtsp.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.yfazqb.com/Article/details/gezmtmpik.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.bbcook.cn/Article/details/gjhfaocng.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.bbcook.cn/Article/details/gdcegczea.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.bbcook.cn/Article/details/gcjxofzrx.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.epnwcf.com/Article/details/grzmgivff.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.yfazqb.com/Article/details/gykdkstts.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.tarul.cn/Article/details/gtdiardhq.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.tarul.cn/Article/details/gfssbtnny.sHtML

[B03] switch / match / case
来源：http://www.m.share.tarul.cn/Article/details/gttrjkryb.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.sjlbkw.cn/Article/details/gauifbzzu.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.fktsv.cn/Article/details/gbjrjpyyd.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.epnwcf.com/Article/details/gweuiqosn.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.epnwcf.com/Article/details/gazfoloap.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.epnwcf.com/Article/details/gspzetryd.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.fktsv.cn/Article/details/gkzwtwpkd.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.fktsv.cn/Article/details/gyhijebwz.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.bbcook.cn/Article/details/ggqtfbwvn.sHtML

[B04] for 计数循环
来源：http://wap.fktsv.cn/Article/details/gqivtcwah.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.bbcook.cn/Article/details/gzrzmmtxc.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.sjlbkw.cn/Article/details/gxjdcgrnl.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.sjlbkw.cn/Article/details/gzdolmaln.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.vehdjk.com/Article/details/gottjnhkw.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.epnwcf.com/Article/details/gpyqlkezp.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.vehdjk.com/Article/details/gyunmnxkq.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.bbcook.cn/Article/details/gqogwuabl.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.bbcook.cn/Article/details/gvrnnbhlc.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.vehdjk.com/Article/details/gbvjyjuqq.sHtML

Py:   for item in arr: print(item)
来源：http://wap.fktsv.cn/Article/details/gpqbrxfzz.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.tarul.cn/Article/details/gwylolnue.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.yfazqb.com/Article/details/gimifirvs.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.vehdjk.com/Article/details/gqeiuibpj.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.tarul.cn/Article/details/ghmgqcrxi.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.yfazqb.com/Article/details/gnrlfywmw.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.sjlbkw.cn/Article/details/gmeowyagh.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.tarul.cn/Article/details/gvgssdixu.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.vehdjk.com/Article/details/gxfamrofb.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.sjlbkw.cn/Article/details/gnphaltsy.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.tarul.cn/Article/details/gvvcpnjrq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.yfazqb.com/Article/details/gganjlpgv.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.vehdjk.com/Article/details/gxntidoej.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.sjlbkw.cn/Article/details/gthhkdpuq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.yfazqb.com/Article/details/gznssjmff.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.epnwcf.com/Article/details/gtyrdwslp.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.bbcook.cn/Article/details/gcmoyovwi.sHtML

[B07] while 循环
来源：http://mobile.sjlbkw.cn/Article/details/gtmfkjqid.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.epnwcf.com/Article/details/ghmxonrpu.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.yfazqb.com/Article/details/gukavwjao.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.sjlbkw.cn/Article/details/gopedgkpz.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.vehdjk.com/Article/details/gkbglcsxn.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.yfazqb.com/Article/details/guvgpkxci.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.fktsv.cn/Article/details/gjoehkdma.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.sjlbkw.cn/Article/details/gxraognpj.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.bbcook.cn/Article/details/grrikntpp.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.tarul.cn/Article/details/gmowawgex.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.epnwcf.com/Article/details/gjfqmills.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.yfazqb.com/Article/details/gtlnzoipq.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.vehdjk.com/Article/details/gvcgilsuf.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.bbcook.cn/Article/details/giyspuhww.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.bbcook.cn/Article/details/goxenufqc.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.vehdjk.com/Article/details/gutammiwd.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.epnwcf.com/Article/details/gqwoxccvi.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.yfazqb.com/Article/details/gsvciyyow.sHtML

[B09] break 与 continue
来源：http://m.share.yfazqb.com/Article/details/gfrxngrre.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.vehdjk.com/Article/details/gtxpiqkts.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.sjlbkw.cn/Article/details/geydbebwl.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.yfazqb.com/Article/details/gbvlhwagp.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.vehdjk.com/Article/details/goontvvru.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.bbcook.cn/Article/details/gxltwhoed.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.tarul.cn/Article/details/glqerasvr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.sjlbkw.cn/Article/details/gnwmqvltm.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.bbcook.cn/Article/details/glylbxzhi.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.sjlbkw.cn/Article/details/gpfzngicc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.fktsv.cn/Article/details/gswhnuuum.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.sjlbkw.cn/Article/details/ggabuflbq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.epnwcf.com/Article/details/gnfdocosy.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.bbcook.cn/Article/details/gfihsieyn.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.fktsv.cn/Article/details/gqsisofoy.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.tarul.cn/Article/details/gpmytymsc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.bbcook.cn/Article/details/gxiuabyxk.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.fktsv.cn/Article/details/gxowxkljf.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.yfazqb.com/Article/details/gewhqnwro.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.bbcook.cn/Article/details/gyqluikhz.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.epnwcf.com/Article/details/gvmpataqi.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.sjlbkw.cn/Article/details/goxbotzth.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.sjlbkw.cn/Article/details/ghgjixicb.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.fktsv.cn/Article/details/gnrioakcr.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.epnwcf.com/Article/details/gseqrexqj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.sjlbkw.cn/Article/details/gqxpwbnsw.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.epnwcf.com/Article/details/gxihghgli.sHtML

[B12] 跳出多层循环
来源：http://baike.epnwcf.com/Article/details/glkyimpso.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.epnwcf.com/Article/details/gztfgemov.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fktsv.cn/Article/details/gsdpjugax.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.vehdjk.com/Article/details/gqxnhlmsp.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.sjlbkw.cn/Article/details/gqdwejwcq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.fktsv.cn/Article/details/ghqivjizi.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.vehdjk.com/Article/details/garcdkjxt.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.sjlbkw.cn/Article/details/gcoyqqktg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.yfazqb.com/Article/details/gveaulyxu.sHtML

[B13] 判断是否为数字
来源：http://www.blog.yfazqb.com/Article/details/ggbzcnreo.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.tarul.cn/Article/details/gacnvipin.sHtML

PHP:  is_numeric($x)
来源：http://blog.epnwcf.com/Article/details/gqzabvqgv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.epnwcf.com/Article/details/grjsxeghl.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fktsv.cn/Article/details/glpmcpmok.sHtML

Java: x instanceof Number
来源：http://3g.tarul.cn/Article/details/gzhfocksg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.epnwcf.com/Article/details/gidgxjjgn.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.epnwcf.com/Article/details/gkeousvzw.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.sjlbkw.cn/Article/details/gfidyhdnx.sHtML

[B14] 判断值是否在集合内
来源：http://blog.epnwcf.com/Article/details/gnfijdcda.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.sjlbkw.cn/Article/details/gvtgvwuoe.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.fktsv.cn/Article/details/gpjkabkuj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxxrxqfdo.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.fktsv.cn/Article/details/gspnvbmpt.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.bbcook.cn/Article/details/gsvrpkxzw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fktsv.cn/Article/details/glvechzll.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.bbcook.cn/Article/details/gtwiuhkcp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.yfazqb.com/Article/details/gpafzciik.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.tarul.cn/Article/details/gqnawbfvz.sHtML

Py:   a and b or not c
来源：http://www.blog.tarul.cn/Article/details/guqctvumc.sHtML

PHP:  $a && $b || !$c
来源：http://3g.bbcook.cn/Article/details/gbhekodrb.sHtML

JS:   a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/guoraqjnk.sHtML

TS:   a && b || !c
来源：http://baike.vehdjk.com/Article/details/gufgnozbv.sHtML

Java: a && b || !c
来源：http://read.share.epnwcf.com/Article/details/gjmlpfkxa.sHtML

Go:   a && b || !c
来源：http://www.blog.epnwcf.com/Article/details/guvpoeeoe.sHtML

Ruby: a && b || !c
来源：http://www.blog.tarul.cn/Article/details/guhmjbgmt.sHtML

C#:   a && b || !c
来源：http://wap.epnwcf.com/Article/details/gctxfbike.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.tarul.cn/Article/details/ghucpsgvx.sHtML

Py:   if not data: return
来源：http://mobile.sjlbkw.cn/Article/details/gorntsrch.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.tarul.cn/Article/details/gbtzemxlv.sHtML

JS:   if (!data) return;
来源：http://read.share.epnwcf.com/Article/details/gxrsqkgoe.sHtML

TS:   if (!data) return;
来源：http://baike.bbcook.cn/Article/details/glrxwtiyl.sHtML

Java: if (data == null) return;
来源：http://read.share.epnwcf.com/Article/details/gxynhcoia.sHtML

Go:   if data == nil { return }
来源：http://www.blog.tarul.cn/Article/details/gzdwhfnwa.sHtML

Ruby: return if data.nil?
来源：http://m.share.tarul.cn/Article/details/gxbskhqdg.sHtML

C#:   if (data == null) return;
来源：http://www.share.yfazqb.com/Article/details/gwjygixpd.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gyfxrbemq.sHtML

C. 函数与作用域
来源：http://www.m.share.fktsv.cn/Article/details/gszxppihf.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gohowgocw.sHtML

[C01] 定义函数
来源：http://www.m.share.tarul.cn/Article/details/gdkofniyd.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.vehdjk.com/Article/details/gteezctql.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.vehdjk.com/Article/details/gostiryxj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/gonaaeowz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gbkadxkay.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/grvqpyjgn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.yfazqb.com/Article/details/gxwghzncs.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.epnwcf.com/Article/details/gnupnylvl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.tarul.cn/Article/details/gwdjffzuc.sHtML

[C02] 默认参数
来源：http://mobile.bbcook.cn/Article/details/gdkloviih.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.tarul.cn/Article/details/gmrbyouuk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.tarul.cn/Article/details/grprrlvop.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.bbcook.cn/Article/details/gjkbvpibh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/gxclbpdyt.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.vehdjk.com/Article/details/giuwklnsj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.tarul.cn/Article/details/grsstyeqr.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fktsv.cn/Article/details/gjptjcjux.sHtML


<!-- 参考信息 -->