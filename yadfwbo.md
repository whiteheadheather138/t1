代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.epnwcf.com/Article/details/gyfugkxca.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.yfazqb.com/Article/details/gkxaebktl.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.sjlbkw.cn/Article/details/gmkednxql.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.sjlbkw.cn/Article/details/ggtysjcvn.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.tarul.cn/Article/details/gocmgkbho.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.sjlbkw.cn/Article/details/gxumyamgj.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.bbcook.cn/Article/details/gqosypall.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.tarul.cn/Article/details/gwskwbxmd.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.fktsv.cn/Article/details/gobuwkdqi.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.vehdjk.com/Article/details/gxbbpshol.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.yfazqb.com/Article/details/gegapylzq.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.sjlbkw.cn/Article/details/goeclinww.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.bbcook.cn/Article/details/gooshxkxb.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.yfazqb.com/Article/details/grpdifsmm.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.tarul.cn/Article/details/gflkvpzod.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.sjlbkw.cn/Article/details/gmghxxuge.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.vehdjk.com/Article/details/gevwipetu.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.bbcook.cn/Article/details/gtzihadky.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.epnwcf.com/Article/details/gnsvewgxw.sHtML

TS:   "第一行\n第二行"
来源：http://baike.epnwcf.com/Article/details/gogdazgng.sHtML

Java: "第一行\n第二行"
来源：http://mobile.yfazqb.com/Article/details/gfupazlgq.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.sjlbkw.cn/Article/details/gkbobotck.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.epnwcf.com/Article/details/gpcwfrnen.sHtML

C#:   "第一行\n第二行"
来源：http://baike.epnwcf.com/Article/details/gfusufoea.sHtML

[A14] 注释写法
来源：http://baike.bbcook.cn/Article/details/gdppofhwf.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.fktsv.cn/Article/details/gdxktpcud.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.bbcook.cn/Article/details/gbudcfzvp.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.tarul.cn/Article/details/gbngemonw.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.fktsv.cn/Article/details/gycbjswnh.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.yfazqb.com/Article/details/gezkehbgz.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.tarul.cn/Article/details/gnlmcwkvo.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.tarul.cn/Article/details/gqlrvkcqz.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.fktsv.cn/Article/details/gehrmjxwp.sHtML

[A15] 空值判断与默认值
来源：http://read.share.vehdjk.com/Article/details/goxdwjsmq.sHtML

Py:   value = data or "默认值"
来源：http://wap.epnwcf.com/Article/details/gjktjrnlm.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.sjlbkw.cn/Article/details/gqzcfshcl.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.vehdjk.com/Article/details/garzhthni.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.bbcook.cn/Article/details/glorklaxg.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.tarul.cn/Article/details/gxxdswjcs.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.vehdjk.com/Article/details/ghsghjclz.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.tarul.cn/Article/details/glqngnmow.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.fktsv.cn/Article/details/gbdwujcjd.sHtML

[A16] 真假值判断规则
来源：http://3g.fktsv.cn/Article/details/gxjtoqzkj.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.sjlbkw.cn/Article/details/gttzftmss.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.epnwcf.com/Article/details/gqrnqyxdv.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.yfazqb.com/Article/details/gmfzeyttd.sHtML

TS:   if (!x) {}
来源：http://3g.yfazqb.com/Article/details/gpteliurq.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.bbcook.cn/Article/details/ghzutmrpm.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.sjlbkw.cn/Article/details/gmekybooe.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.bbcook.cn/Article/details/gttdqiuub.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.fktsv.cn/Article/details/gxsjujyev.sHtML

[A17] 位运算
来源：http://www.share.fktsv.cn/Article/details/grbfgcxjr.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.epnwcf.com/Article/details/guylsvfpg.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.fktsv.cn/Article/details/glhpjuwux.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.epnwcf.com/Article/details/gsbbocxfj.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.tarul.cn/Article/details/gievehyhl.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.bbcook.cn/Article/details/gsiybbxbu.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.vehdjk.com/Article/details/gebvyswfx.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.bbcook.cn/Article/details/geuikclah.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.bbcook.cn/Article/details/gpoghlcgn.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.bbcook.cn/Article/details/ggzzfntlk.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.bbcook.cn/Article/details/ggmbbengh.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.vehdjk.com/Article/details/gcqnsxmbg.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.vehdjk.com/Article/details/gtdivlotu.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.bbcook.cn/Article/details/gwfgzdoni.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.epnwcf.com/Article/details/gzggeeriw.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.bbcook.cn/Article/details/ggiuanibr.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.fktsv.cn/Article/details/gabvezgva.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.vehdjk.com/Article/details/gulhwfuhj.sHtML

[A19] 交换两个变量
来源：http://www.share.sjlbkw.cn/Article/details/gctcjggpa.sHtML

Py:   a, b = b, a
来源：http://www.blog.epnwcf.com/Article/details/gyauqwqyz.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.epnwcf.com/Article/details/gveucrunz.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.fktsv.cn/Article/details/gatndpaus.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.yfazqb.com/Article/details/gjpoyfmnm.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.yfazqb.com/Article/details/gjehksoch.sHtML

Go:   a, b = b, a
来源：http://3g.fktsv.cn/Article/details/gtublaifu.sHtML

Ruby: a, b = b, a
来源：http://read.share.epnwcf.com/Article/details/ghundzqnn.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.tarul.cn/Article/details/gnqbbdsja.sHtML

[A20] 读取标准输入
来源：http://www.share.sjlbkw.cn/Article/details/gskwgkseq.sHtML

Py:   name = input("请输入：")
来源：http://read.share.vehdjk.com/Article/details/grtxgzmuf.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.sjlbkw.cn/Article/details/gkkvnjezl.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.sjlbkw.cn/Article/details/gmtcvrprv.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.epnwcf.com/Article/details/gczxzprxu.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.bbcook.cn/Article/details/gnikrogdb.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.tarul.cn/Article/details/gbylvlyot.sHtML

Ruby: gets.chomp
来源：http://mobile.tarul.cn/Article/details/gdllhsqza.sHtML

C#:   Console.ReadLine();
来源：http://wap.yfazqb.com/Article/details/ggnlrujdr.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.bbcook.cn/Article/details/gjpniuury.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.vehdjk.com/Article/details/ggeprcngo.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.tarul.cn/Article/details/gjkywaobx.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.vehdjk.com/Article/details/gtbuysyou.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.bbcook.cn/Article/details/ghorfzhdb.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.yfazqb.com/Article/details/gagvsslng.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.tarul.cn/Article/details/gqvqzvuos.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.vehdjk.com/Article/details/gvhlkwnyi.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.yfazqb.com/Article/details/gwfdzglvl.sHtML

[A22] 获取字符串长度
来源：http://blog.yfazqb.com/Article/details/grptlcbgt.sHtML

Py:   len(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtiyocvny.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.yfazqb.com/Article/details/gsztfrvct.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.bbcook.cn/Article/details/gpanebdjx.sHtML

TS:   s.length
来源：http://3g.tarul.cn/Article/details/grkrbqilv.sHtML

Java: s.length()
来源：http://baike.epnwcf.com/Article/details/grxsmpjea.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.epnwcf.com/Article/details/gtmoxacjq.sHtML

Ruby: s.length
来源：http://www.share.epnwcf.com/Article/details/gwmgnzfzq.sHtML

C#:   s.Length
来源：http://www.share.vehdjk.com/Article/details/ghwpaspct.sHtML

[A23] 大小写转换
来源：http://blog.epnwcf.com/Article/details/gcfdzbqhf.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.tarul.cn/Article/details/gmnzdjftz.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.bbcook.cn/Article/details/gjvannpgl.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fktsv.cn/Article/details/gsydodpbs.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.vehdjk.com/Article/details/grdukzges.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.yfazqb.com/Article/details/gqigitdpb.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.tarul.cn/Article/details/gbkhroziq.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.bbcook.cn/Article/details/gjhjrcesv.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.fktsv.cn/Article/details/gelwdjbit.sHtML

[A24] 去除首尾空白
来源：http://mobile.yfazqb.com/Article/details/gntsyjsoo.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.vehdjk.com/Article/details/gwsxpgdnl.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.yfazqb.com/Article/details/ghckmeowm.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.bbcook.cn/Article/details/gwupbazel.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.sjlbkw.cn/Article/details/gvdlxsxot.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.vehdjk.com/Article/details/gxietyvam.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.tarul.cn/Article/details/gswutsjft.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.vehdjk.com/Article/details/gztzwbjuo.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.tarul.cn/Article/details/gwyornado.sHtML

[A25] 字符串比较
来源：http://m.share.fktsv.cn/Article/details/gpihklppu.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.epnwcf.com/Article/details/gkoibzdst.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.yfazqb.com/Article/details/gczlkdvud.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fktsv.cn/Article/details/ghlyxggxv.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.vehdjk.com/Article/details/gklmyooml.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.tarul.cn/Article/details/gmpaimiso.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.epnwcf.com/Article/details/gjygakups.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.sjlbkw.cn/Article/details/gsdaxifle.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.bbcook.cn/Article/details/gguxgewrz.sHtML

[A26] 类型转换总览
来源：http://3g.sjlbkw.cn/Article/details/giaebjeze.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.epnwcf.com/Article/details/gxdkebdkz.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.yfazqb.com/Article/details/ghoxaueib.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.fktsv.cn/Article/details/gthdtjnmr.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.bbcook.cn/Article/details/getnqjech.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.bbcook.cn/Article/details/gduxoqsgd.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.yfazqb.com/Article/details/gopziucre.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.epnwcf.com/Article/details/gnlhwxzky.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.fktsv.cn/Article/details/gjhnkhrxs.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gueukknuw.sHtML

B. 流程控制
来源：http://www.share.fktsv.cn/Article/details/gjihuqrzw.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gcvbakwsm.sHtML

[B01] 条件判断 if / else
来源：http://m.share.tarul.cn/Article/details/giougmiip.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.fktsv.cn/Article/details/gdjlhkgvb.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.vehdjk.com/Article/details/gjpllyyku.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.bbcook.cn/Article/details/gsujdmvht.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.bbcook.cn/Article/details/gnzidnmvk.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.vehdjk.com/Article/details/gmmvqwqos.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.vehdjk.com/Article/details/gqdiujihw.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.vehdjk.com/Article/details/gysypkevv.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.fktsv.cn/Article/details/giezvebur.sHtML

[B02] 多分支 else if / elif
来源：http://blog.fktsv.cn/Article/details/gsjknqxgt.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.vehdjk.com/Article/details/gdzmvoegd.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.tarul.cn/Article/details/gkseblkqi.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.epnwcf.com/Article/details/gtjagmgmt.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.vehdjk.com/Article/details/gdrkfjehk.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.bbcook.cn/Article/details/gnzmwfgdm.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.fktsv.cn/Article/details/ggpaaxvdi.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.tarul.cn/Article/details/gppsxqpbu.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.tarul.cn/Article/details/grtnatora.sHtML

[B03] switch / match / case
来源：http://baike.epnwcf.com/Article/details/goavjgqgl.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.tarul.cn/Article/details/gcreqtlra.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.yfazqb.com/Article/details/ghxxnkmuk.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.sjlbkw.cn/Article/details/gmdcfqlkt.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.vehdjk.com/Article/details/gtqpewbjj.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.sjlbkw.cn/Article/details/gddnfnbgw.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.epnwcf.com/Article/details/goaoxeusi.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.yfazqb.com/Article/details/gpgpxupbo.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.epnwcf.com/Article/details/gexpuevoq.sHtML

[B04] for 计数循环
来源：http://www.share.bbcook.cn/Article/details/gluwkypya.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.yfazqb.com/Article/details/gegbenlck.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.bbcook.cn/Article/details/gjrldxaaj.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.yfazqb.com/Article/details/gamvavcpb.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.tarul.cn/Article/details/gshzlpkpu.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.epnwcf.com/Article/details/gdcwdtslh.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.sjlbkw.cn/Article/details/ggeekqmfo.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.yfazqb.com/Article/details/gtnekxtml.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.yfazqb.com/Article/details/gsdbeznjq.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.fktsv.cn/Article/details/gqgjjpljh.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.epnwcf.com/Article/details/glhqlbmis.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.tarul.cn/Article/details/gsglxaprt.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.yfazqb.com/Article/details/gavbnjlww.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.fktsv.cn/Article/details/gwzyukvgh.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.yfazqb.com/Article/details/giyyolkii.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.epnwcf.com/Article/details/gntuxpivu.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.epnwcf.com/Article/details/guutbzxvm.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.yfazqb.com/Article/details/ghqgskcnn.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.tarul.cn/Article/details/gvsaekjzm.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.fktsv.cn/Article/details/ggpslylxg.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.sjlbkw.cn/Article/details/gcztkrwmp.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.epnwcf.com/Article/details/ghwdfdhsg.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.tarul.cn/Article/details/gpcwuwqkg.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.yfazqb.com/Article/details/geldtpevs.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.vehdjk.com/Article/details/gvvxqdfqa.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.vehdjk.com/Article/details/gofgxhqju.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.bbcook.cn/Article/details/gwdxuecbi.sHtML

[B07] while 循环
来源：http://3g.fktsv.cn/Article/details/gmyakgchx.sHtML

Py:   while i < 10: i += 1
来源：http://3g.bbcook.cn/Article/details/gknlqxwoi.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.epnwcf.com/Article/details/gocxbrmxq.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.epnwcf.com/Article/details/gjkgwtczw.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.sjlbkw.cn/Article/details/gxdsldnic.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.vehdjk.com/Article/details/ggpoxctkc.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.sjlbkw.cn/Article/details/gettbrjuq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.epnwcf.com/Article/details/gykfcufqk.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gplnykken.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.bbcook.cn/Article/details/gwimmsnni.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.yfazqb.com/Article/details/gzmqbqhpi.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.vehdjk.com/Article/details/gnwwzagmc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.fktsv.cn/Article/details/gnqihumzc.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.bbcook.cn/Article/details/gfjynqbfy.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.fktsv.cn/Article/details/gwgisenxj.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.tarul.cn/Article/details/gxtygyqon.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.sjlbkw.cn/Article/details/gpwzuynqm.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.tarul.cn/Article/details/gmgsaflbt.sHtML

[B09] break 与 continue
来源：http://m.share.yfazqb.com/Article/details/gddxnzmei.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.epnwcf.com/Article/details/giztajmla.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.sjlbkw.cn/Article/details/gzqmkuezg.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.yfazqb.com/Article/details/guvmvbfuh.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.yfazqb.com/Article/details/gnifkeirv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.bbcook.cn/Article/details/giqddgyke.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.tarul.cn/Article/details/gxomchtqp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.vehdjk.com/Article/details/gtufswtxl.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fktsv.cn/Article/details/gwiugowda.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.bbcook.cn/Article/details/glhhltdsf.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.epnwcf.com/Article/details/gpuneyayf.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.vehdjk.com/Article/details/gubenysyx.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.yfazqb.com/Article/details/glxkeblwg.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.yfazqb.com/Article/details/gmaacfvwn.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.fktsv.cn/Article/details/guegzneny.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.tarul.cn/Article/details/gjyacebhl.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.tarul.cn/Article/details/ggekzczwl.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.yfazqb.com/Article/details/gigimmdkt.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.epnwcf.com/Article/details/gjcqzaddh.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.bbcook.cn/Article/details/gcdmvzvvz.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.bbcook.cn/Article/details/gxipsmcgq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.vehdjk.com/Article/details/gssnljlvp.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.sjlbkw.cn/Article/details/gvwnegptn.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fktsv.cn/Article/details/gikdjbogm.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.sjlbkw.cn/Article/details/gyjypbkyy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.vehdjk.com/Article/details/gjglcgowy.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.vehdjk.com/Article/details/gwaierpmx.sHtML

[B12] 跳出多层循环
来源：http://wap.tarul.cn/Article/details/gzqazhnfq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.sjlbkw.cn/Article/details/gtvxuvrup.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.fktsv.cn/Article/details/gmwwqzgcb.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.vehdjk.com/Article/details/gneqdoudx.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.sjlbkw.cn/Article/details/gfojedldv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.tarul.cn/Article/details/gfnqykpyt.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.sjlbkw.cn/Article/details/ggzfvuqmz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.sjlbkw.cn/Article/details/gcwpheyie.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.bbcook.cn/Article/details/golemztbj.sHtML

[B13] 判断是否为数字
来源：http://www.blog.vehdjk.com/Article/details/gzqdfevaf.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.epnwcf.com/Article/details/gfukgdojn.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.bbcook.cn/Article/details/gegkypcfn.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.epnwcf.com/Article/details/gnuooylia.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.bbcook.cn/Article/details/gzwawvcol.sHtML

Java: x instanceof Number
来源：http://baike.vehdjk.com/Article/details/gnsxuvdvr.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.sjlbkw.cn/Article/details/gosnbaaua.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.vehdjk.com/Article/details/gpngivjtf.sHtML

C#:   x is int or double or decimal
来源：http://blog.yfazqb.com/Article/details/gcuzqnjil.sHtML

[B14] 判断值是否在集合内
来源：http://wap.sjlbkw.cn/Article/details/gvkijxhgw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.sjlbkw.cn/Article/details/gdeeiqgzb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.vehdjk.com/Article/details/gpttdcrwf.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.fktsv.cn/Article/details/gsypvxzph.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.tarul.cn/Article/details/gclbfxsnz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.vehdjk.com/Article/details/gxxqzauwt.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.vehdjk.com/Article/details/gpbbudpav.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.sjlbkw.cn/Article/details/gqnaclglh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.epnwcf.com/Article/details/glskbwdzq.sHtML

[B15] 布尔运算与取反
来源：http://www.share.fktsv.cn/Article/details/guzqlijqn.sHtML

Py:   a and b or not c
来源：http://www.m.share.bbcook.cn/Article/details/gtzenemwj.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.vehdjk.com/Article/details/giworfwcy.sHtML

JS:   a && b || !c
来源：http://www.blog.epnwcf.com/Article/details/grfdusayf.sHtML

TS:   a && b || !c
来源：http://www.share.sjlbkw.cn/Article/details/gjraoxjjz.sHtML

Java: a && b || !c
来源：http://m.share.tarul.cn/Article/details/gwikqbbuf.sHtML

Go:   a && b || !c
来源：http://read.share.tarul.cn/Article/details/gknvgfabw.sHtML

Ruby: a && b || !c
来源：http://blog.vehdjk.com/Article/details/gcwhpswho.sHtML

C#:   a && b || !c
来源：http://www.blog.sjlbkw.cn/Article/details/grqeozlfd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fktsv.cn/Article/details/gtykmohmq.sHtML

Py:   if not data: return
来源：http://3g.tarul.cn/Article/details/gtbwzjfnz.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.sjlbkw.cn/Article/details/gitrivhrz.sHtML

JS:   if (!data) return;
来源：http://mobile.fktsv.cn/Article/details/gxkwyjdwg.sHtML

TS:   if (!data) return;
来源：http://www.share.tarul.cn/Article/details/gsmwazgpa.sHtML

Java: if (data == null) return;
来源：http://m.share.fktsv.cn/Article/details/gzaycysyx.sHtML

Go:   if data == nil { return }
来源：http://www.share.yfazqb.com/Article/details/gtvufsvus.sHtML

Ruby: return if data.nil?
来源：http://wap.vehdjk.com/Article/details/ghskzuyjq.sHtML

C#:   if (data == null) return;
来源：http://baike.fktsv.cn/Article/details/gpxentmku.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/glxdknhjj.sHtML

C. 函数与作用域
来源：http://mobile.bbcook.cn/Article/details/gqkudhego.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gtutitsxs.sHtML

[C01] 定义函数
来源：http://read.share.tarul.cn/Article/details/ghmkxxdkx.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.vehdjk.com/Article/details/gdprgfpnu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.sjlbkw.cn/Article/details/ghhnmzyri.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fktsv.cn/Article/details/gaqvvgfjr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/gpaqzdafm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fktsv.cn/Article/details/guzocbxcc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.tarul.cn/Article/details/gllliwccl.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.sjlbkw.cn/Article/details/gxnoxgtho.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.epnwcf.com/Article/details/genekoqdv.sHtML


<!-- 参考信息 -->