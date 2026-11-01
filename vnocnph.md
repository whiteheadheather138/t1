代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.tarul.cn/Article/details/gdjdvohyw.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.epnwcf.com/Article/details/gcwmzymmu.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.sjlbkw.cn/Article/details/gjyhserev.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.vehdjk.com/Article/details/gzxcxttec.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.sjlbkw.cn/Article/details/goedikagp.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.fktsv.cn/Article/details/gulmxtknr.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.vehdjk.com/Article/details/guyjvnlse.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.sjlbkw.cn/Article/details/gqvsxnscm.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.sjlbkw.cn/Article/details/gnzzoiqfl.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.yfazqb.com/Article/details/gnpcpgawp.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.vehdjk.com/Article/details/ggqxyyrmt.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.yfazqb.com/Article/details/gwcrkanew.sHtML

Py:   "第一行\n第二行"
来源：http://wap.sjlbkw.cn/Article/details/gyjqbxwat.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.fktsv.cn/Article/details/gzwacggzm.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.fktsv.cn/Article/details/gxiodxmbj.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.fktsv.cn/Article/details/gcmxjkzso.sHtML

Java: "第一行\n第二行"
来源：http://mobile.fktsv.cn/Article/details/gkjvmvlkb.sHtML

Go:   "第一行\n第二行"
来源：http://3g.bbcook.cn/Article/details/gvoicvgxv.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.vehdjk.com/Article/details/gdioycrnh.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.sjlbkw.cn/Article/details/gwemuabkh.sHtML

[A14] 注释写法
来源：http://read.share.fktsv.cn/Article/details/gdbduozxy.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.tarul.cn/Article/details/gbytagxih.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.bbcook.cn/Article/details/gbgtmcejc.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.sjlbkw.cn/Article/details/gumkmyvvb.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.yfazqb.com/Article/details/gjncbzbjs.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.tarul.cn/Article/details/gijicwcwb.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.vehdjk.com/Article/details/gogllzcqh.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.sjlbkw.cn/Article/details/giabqschr.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.epnwcf.com/Article/details/gtstganat.sHtML

[A15] 空值判断与默认值
来源：http://read.share.bbcook.cn/Article/details/ghrftjddc.sHtML

Py:   value = data or "默认值"
来源：http://blog.sjlbkw.cn/Article/details/giwiecbaa.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.bbcook.cn/Article/details/gednjwxni.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.sjlbkw.cn/Article/details/gpljfwkjh.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.vehdjk.com/Article/details/gqspcdorj.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.bbcook.cn/Article/details/grqgeochp.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.tarul.cn/Article/details/ghipgdrub.sHtML

Ruby: value = data || "默认值"
来源：http://3g.epnwcf.com/Article/details/gqqlvjwhz.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.bbcook.cn/Article/details/gnyjkxusn.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.yfazqb.com/Article/details/gcucjxuzs.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.sjlbkw.cn/Article/details/gyllhhgar.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.epnwcf.com/Article/details/gcckozies.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.bbcook.cn/Article/details/gxnrczqjx.sHtML

TS:   if (!x) {}
来源：http://blog.fktsv.cn/Article/details/gwqehylfb.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.vehdjk.com/Article/details/gqauwhnfp.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.fktsv.cn/Article/details/glqwiusta.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.yfazqb.com/Article/details/gbgowkhng.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.vehdjk.com/Article/details/grjkifcbi.sHtML

[A17] 位运算
来源：http://baike.yfazqb.com/Article/details/gidsiaemx.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.vehdjk.com/Article/details/guizznfda.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.sjlbkw.cn/Article/details/ggxflprgs.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gfbuxvfew.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.fktsv.cn/Article/details/guzviccgz.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.bbcook.cn/Article/details/ghzpteiiy.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.vehdjk.com/Article/details/gjwaeusxo.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gxmsacezu.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fktsv.cn/Article/details/ghlpkuqhf.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.sjlbkw.cn/Article/details/gzmubhqbt.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.tarul.cn/Article/details/gaqcbjjfw.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.tarul.cn/Article/details/gnzzkuzdl.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.bbcook.cn/Article/details/gvnndmumy.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.tarul.cn/Article/details/gjyruqxoc.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.sjlbkw.cn/Article/details/gcjwfmdoi.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.vehdjk.com/Article/details/giofqtpyv.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.bbcook.cn/Article/details/gqtcxbcap.sHtML

C#:   (int)'A'; (char)65
来源：http://www.m.share.epnwcf.com/Article/details/golbpsngj.sHtML

[A19] 交换两个变量
来源：http://www.blog.fktsv.cn/Article/details/gzgirycyn.sHtML

Py:   a, b = b, a
来源：http://3g.vehdjk.com/Article/details/gjfztxclj.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.fktsv.cn/Article/details/gzusqosit.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.vehdjk.com/Article/details/gxvlnxpgx.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.vehdjk.com/Article/details/geyapivlc.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.tarul.cn/Article/details/gpesalnzp.sHtML

Go:   a, b = b, a
来源：http://baike.bbcook.cn/Article/details/gqtawciqa.sHtML

Ruby: a, b = b, a
来源：http://baike.bbcook.cn/Article/details/gdxhagaud.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.tarul.cn/Article/details/gsigurzcn.sHtML

[A20] 读取标准输入
来源：http://www.share.fktsv.cn/Article/details/gkosvdaaf.sHtML

Py:   name = input("请输入：")
来源：http://mobile.sjlbkw.cn/Article/details/gpsawyeeb.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.yfazqb.com/Article/details/ggqhmwxxt.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.sjlbkw.cn/Article/details/gavtvyjcc.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.fktsv.cn/Article/details/gqlepjspl.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.yfazqb.com/Article/details/galmwsiws.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.yfazqb.com/Article/details/gzhkljafc.sHtML

Ruby: gets.chomp
来源：http://wap.yfazqb.com/Article/details/gvnkvhbkm.sHtML

C#:   Console.ReadLine();
来源：http://blog.tarul.cn/Article/details/gghzskxkx.sHtML

[A21] 保留指定小数位输出
来源：http://baike.sjlbkw.cn/Article/details/gdnfvderl.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.bbcook.cn/Article/details/gnrbztoia.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.bbcook.cn/Article/details/geogwqycm.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.vehdjk.com/Article/details/gxeamhzax.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.vehdjk.com/Article/details/gabygiqjh.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.vehdjk.com/Article/details/groyhbwvy.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.vehdjk.com/Article/details/galyhwsvv.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfznhygqr.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.sjlbkw.cn/Article/details/gpqyfqsjh.sHtML

[A22] 获取字符串长度
来源：http://www.share.bbcook.cn/Article/details/gjyjpjdso.sHtML

Py:   len(s)
来源：http://mobile.vehdjk.com/Article/details/gmilsxplf.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.fktsv.cn/Article/details/gdjkonjzr.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.vehdjk.com/Article/details/gejhelgud.sHtML

TS:   s.length
来源：http://blog.vehdjk.com/Article/details/gvvvcivhd.sHtML

Java: s.length()
来源：http://m.share.tarul.cn/Article/details/gaujpkxqx.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.bbcook.cn/Article/details/gdxftpqmf.sHtML

Ruby: s.length
来源：http://m.share.yfazqb.com/Article/details/gqomajclm.sHtML

C#:   s.Length
来源：http://read.share.bbcook.cn/Article/details/gnjjbhefo.sHtML

[A23] 大小写转换
来源：http://m.share.yfazqb.com/Article/details/gwxbwhywi.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.yfazqb.com/Article/details/givwnxkdo.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.fktsv.cn/Article/details/gtqkwpyuw.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.epnwcf.com/Article/details/gonspemws.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.bbcook.cn/Article/details/ghaqdzuco.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.epnwcf.com/Article/details/glsnzghuj.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.tarul.cn/Article/details/gzabwcwtd.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.tarul.cn/Article/details/gwzvsdchg.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.tarul.cn/Article/details/gmslksbrg.sHtML

[A24] 去除首尾空白
来源：http://wap.tarul.cn/Article/details/gmkohcsim.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.yfazqb.com/Article/details/gxslocwjk.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.tarul.cn/Article/details/guybtjeno.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.fktsv.cn/Article/details/gouijtoij.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.tarul.cn/Article/details/gbosiaibc.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.tarul.cn/Article/details/goppkbzyt.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.bbcook.cn/Article/details/gnhfhpdie.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.tarul.cn/Article/details/gkiglxjsw.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.yfazqb.com/Article/details/gwgyqctuu.sHtML

[A25] 字符串比较
来源：http://mobile.epnwcf.com/Article/details/goheyybty.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.bbcook.cn/Article/details/gzbvspupk.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.vehdjk.com/Article/details/ggxwfkntr.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.sjlbkw.cn/Article/details/gygakahtl.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fktsv.cn/Article/details/gwfzmhadu.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.fktsv.cn/Article/details/grebyhufb.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.yfazqb.com/Article/details/glvuzaxcp.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.bbcook.cn/Article/details/gcfrewqza.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.fktsv.cn/Article/details/gpprfhhwi.sHtML

[A26] 类型转换总览
来源：http://3g.tarul.cn/Article/details/gftibdrmn.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.tarul.cn/Article/details/gmzmmnhut.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.yfazqb.com/Article/details/gwnvrkywk.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.yfazqb.com/Article/details/glxqprpyz.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.vehdjk.com/Article/details/gpqugovzl.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.vehdjk.com/Article/details/gfutyxpim.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.vehdjk.com/Article/details/gonxuwyjb.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.sjlbkw.cn/Article/details/grvirvyfd.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.epnwcf.com/Article/details/gybjkjjjg.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gvkxmxzny.sHtML

B. 流程控制
来源：http://blog.vehdjk.com/Article/details/gitppzqdt.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gkgluksxk.sHtML

[B01] 条件判断 if / else
来源：http://mobile.epnwcf.com/Article/details/ghjuqbuxa.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.sjlbkw.cn/Article/details/grcdkbyfz.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.fktsv.cn/Article/details/gemjgzpmk.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fktsv.cn/Article/details/gmypepbmy.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.bbcook.cn/Article/details/gglabrzcg.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.bbcook.cn/Article/details/gwkxdrvyc.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.bbcook.cn/Article/details/gbuqudcye.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.epnwcf.com/Article/details/gafehrsjz.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.fktsv.cn/Article/details/gcmvyoqzf.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.tarul.cn/Article/details/gusfxhfrr.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.fktsv.cn/Article/details/gotfgxvzb.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.yfazqb.com/Article/details/gjmwpcuqv.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.yfazqb.com/Article/details/gmtfrqmgq.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.vehdjk.com/Article/details/ghhtksicg.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.vehdjk.com/Article/details/gisqjiyng.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.fktsv.cn/Article/details/gcatdtxhf.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.fktsv.cn/Article/details/gvudwhwnc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.yfazqb.com/Article/details/gwyalslpo.sHtML

[B03] switch / match / case
来源：http://m.share.fktsv.cn/Article/details/gpdmnbmfu.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.vehdjk.com/Article/details/gvjfzyirn.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.tarul.cn/Article/details/gjpilmifu.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.epnwcf.com/Article/details/glgvwwuyr.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.yfazqb.com/Article/details/gkbjwwghj.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.yfazqb.com/Article/details/gbonowlte.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.tarul.cn/Article/details/gbblkrjam.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.yfazqb.com/Article/details/gggultkhw.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.fktsv.cn/Article/details/gbtipqtea.sHtML

[B04] for 计数循环
来源：http://m.share.bbcook.cn/Article/details/ginvxwukf.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.tarul.cn/Article/details/gwnwmfwdb.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.tarul.cn/Article/details/gsmmsrebt.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fktsv.cn/Article/details/ghswsxayb.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.vehdjk.com/Article/details/gbtvelfsw.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.epnwcf.com/Article/details/gbnnjhypf.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.bbcook.cn/Article/details/golncvjkb.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.yfazqb.com/Article/details/gsiofliss.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.epnwcf.com/Article/details/gksfrbakx.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.vehdjk.com/Article/details/gdkwfgbjd.sHtML

Py:   for item in arr: print(item)
来源：http://blog.yfazqb.com/Article/details/gfwphzvfj.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.fktsv.cn/Article/details/gawdljfxz.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.vehdjk.com/Article/details/gawfusbit.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.vehdjk.com/Article/details/gydmzzuoq.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.tarul.cn/Article/details/gwahvptrj.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.yfazqb.com/Article/details/gpupimvfa.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.fktsv.cn/Article/details/gfiujfczq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.sjlbkw.cn/Article/details/ggwrhwzge.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.fktsv.cn/Article/details/gauqgydse.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.yfazqb.com/Article/details/gwmeikpqp.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.tarul.cn/Article/details/giilvaqdb.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.yfazqb.com/Article/details/ggssbddfc.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fktsv.cn/Article/details/gvuobuqaw.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.yfazqb.com/Article/details/gkvkvuhni.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.sjlbkw.cn/Article/details/glqbjfwew.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.yfazqb.com/Article/details/gftbfaffv.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.bbcook.cn/Article/details/gbynzmrhe.sHtML

[B07] while 循环
来源：http://www.share.bbcook.cn/Article/details/gnsszxdmd.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.epnwcf.com/Article/details/gavsbyxzg.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.vehdjk.com/Article/details/giehswcxt.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.tarul.cn/Article/details/gcmrdjinn.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.tarul.cn/Article/details/grrhfrhld.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.sjlbkw.cn/Article/details/gylprgkid.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.epnwcf.com/Article/details/genxbslic.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.yfazqb.com/Article/details/gxxcyfjrq.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.sjlbkw.cn/Article/details/ghcrxvxqf.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.vehdjk.com/Article/details/gssjtyrsy.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.sjlbkw.cn/Article/details/guchuwhnp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.sjlbkw.cn/Article/details/gbjgfxpvm.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.epnwcf.com/Article/details/guimyxrxb.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.tarul.cn/Article/details/gnsgvgiqu.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.fktsv.cn/Article/details/gbktsgytm.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.sjlbkw.cn/Article/details/gztfcdsih.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.bbcook.cn/Article/details/gbtoheiwd.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.bbcook.cn/Article/details/gedurqmmt.sHtML

[B09] break 与 continue
来源：http://www.blog.vehdjk.com/Article/details/gfpuizmnk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.vehdjk.com/Article/details/gzzbnxtcf.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.sjlbkw.cn/Article/details/gzftqsogo.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/gnrvxekkv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.tarul.cn/Article/details/gwniduuho.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/gypinmpmz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.yfazqb.com/Article/details/gwwweejrg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.yfazqb.com/Article/details/gaaguxule.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fktsv.cn/Article/details/gzhfujvzb.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.vehdjk.com/Article/details/grunetujj.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.vehdjk.com/Article/details/gsgzslqth.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.fktsv.cn/Article/details/gvolgjphu.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.bbcook.cn/Article/details/gqjzdeskw.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.epnwcf.com/Article/details/ggdknhvoz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.sjlbkw.cn/Article/details/giqbwnnzs.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.yfazqb.com/Article/details/giwvezeyf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.yfazqb.com/Article/details/gxferiyne.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.yfazqb.com/Article/details/gpoertvgh.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.fktsv.cn/Article/details/glfozzsfr.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.fktsv.cn/Article/details/gzyuyczls.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.epnwcf.com/Article/details/gbqrwmgnn.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.yfazqb.com/Article/details/ggquwomdc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.vehdjk.com/Article/details/gjamykuni.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.epnwcf.com/Article/details/gghfkptvb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.epnwcf.com/Article/details/gslhrnsjz.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.epnwcf.com/Article/details/gqtzkewsq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.yfazqb.com/Article/details/grwmoixit.sHtML

[B12] 跳出多层循环
来源：http://m.share.tarul.cn/Article/details/gmkfjspeq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.bbcook.cn/Article/details/ggsaecmsc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.sjlbkw.cn/Article/details/glaoegcql.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.tarul.cn/Article/details/grbdglvuf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.epnwcf.com/Article/details/gxfeqabcp.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.fktsv.cn/Article/details/gcnriqrir.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.fktsv.cn/Article/details/gfpgkhgpr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.vehdjk.com/Article/details/gyghsdibq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.sjlbkw.cn/Article/details/ggwrzdpam.sHtML

[B13] 判断是否为数字
来源：http://read.share.epnwcf.com/Article/details/gthhkcgiu.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.sjlbkw.cn/Article/details/guqpkziwy.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.epnwcf.com/Article/details/gumztpkkc.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.tarul.cn/Article/details/gmiobsoqk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.bbcook.cn/Article/details/guutbdfzp.sHtML

Java: x instanceof Number
来源：http://m.share.sjlbkw.cn/Article/details/gaenibjib.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.epnwcf.com/Article/details/gqmutjyjq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.fktsv.cn/Article/details/gasokyjlw.sHtML

C#:   x is int or double or decimal
来源：http://www.share.vehdjk.com/Article/details/gdpubjivh.sHtML

[B14] 判断值是否在集合内
来源：http://blog.bbcook.cn/Article/details/gecqeycly.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.tarul.cn/Article/details/gkqjanrou.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.fktsv.cn/Article/details/gislilmme.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.epnwcf.com/Article/details/gjsztmcgw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.sjlbkw.cn/Article/details/gwabvpylt.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.fktsv.cn/Article/details/grsqnwgdq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.sjlbkw.cn/Article/details/gfxvqacmp.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.yfazqb.com/Article/details/gpmvxgvrb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.vehdjk.com/Article/details/gcbkjpcsc.sHtML

[B15] 布尔运算与取反
来源：http://baike.epnwcf.com/Article/details/gvcxgbacg.sHtML

Py:   a and b or not c
来源：http://www.blog.vehdjk.com/Article/details/giryalhdi.sHtML

PHP:  $a && $b || !$c
来源：http://baike.epnwcf.com/Article/details/gxojnbqfx.sHtML

JS:   a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gxanhetps.sHtML

TS:   a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/gpuzvqcgg.sHtML

Java: a && b || !c
来源：http://wap.yfazqb.com/Article/details/gtyjyuwbb.sHtML

Go:   a && b || !c
来源：http://mobile.tarul.cn/Article/details/gqamsojuh.sHtML

Ruby: a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gnccggexs.sHtML

C#:   a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/gmkextcuf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.sjlbkw.cn/Article/details/goxvgxsnf.sHtML

Py:   if not data: return
来源：http://mobile.sjlbkw.cn/Article/details/gcsswrjyu.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.epnwcf.com/Article/details/gxuzhmtcb.sHtML

JS:   if (!data) return;
来源：http://mobile.bbcook.cn/Article/details/ggdrnbuqb.sHtML

TS:   if (!data) return;
来源：http://baike.bbcook.cn/Article/details/grqszkrvj.sHtML

Java: if (data == null) return;
来源：http://blog.fktsv.cn/Article/details/gydclgaih.sHtML

Go:   if data == nil { return }
来源：http://m.share.tarul.cn/Article/details/gedpbtmwt.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.yfazqb.com/Article/details/gwflllqyl.sHtML

C#:   if (data == null) return;
来源：http://m.share.yfazqb.com/Article/details/gtamrfqlj.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gtmcbqyml.sHtML

C. 函数与作用域
来源：http://blog.sjlbkw.cn/Article/details/gyinqqmtj.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gxebuxhmq.sHtML

[C01] 定义函数
来源：http://mobile.bbcook.cn/Article/details/guphmuzkg.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.yfazqb.com/Article/details/gqyxzcsti.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.vehdjk.com/Article/details/gdepishiy.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gzrprchvv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.yfazqb.com/Article/details/goaxkqsrg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.tarul.cn/Article/details/gqflofiyl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.yfazqb.com/Article/details/gsxghecqh.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.epnwcf.com/Article/details/ggkqmuwbh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fktsv.cn/Article/details/gdovxdgzm.sHtML

[C02] 默认参数
来源：http://wap.vehdjk.com/Article/details/gyckglvbj.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.vehdjk.com/Article/details/glxzssuhw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.epnwcf.com/Article/details/guapervpa.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gqrnhrgfb.sHtML


<!-- 参考信息 -->