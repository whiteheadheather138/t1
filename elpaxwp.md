代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.bbcook.cn/Article/details/gitxsvjnj.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.vehdjk.com/Article/details/gvahqaecg.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.sjlbkw.cn/Article/details/ggikkeffn.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.fktsv.cn/Article/details/gspyrrxvt.sHtML

Py:   "第一行\n第二行"
来源：http://baike.yfazqb.com/Article/details/ggczqsdsu.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.sjlbkw.cn/Article/details/gwgrwfcuw.sHtML

JS:   "第一行\n第二行"
来源：http://3g.yfazqb.com/Article/details/gqhhurbio.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.yfazqb.com/Article/details/gwxyjbbbj.sHtML

Java: "第一行\n第二行"
来源：http://3g.fktsv.cn/Article/details/gswzugjhj.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.tarul.cn/Article/details/giskikjkl.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.bbcook.cn/Article/details/gwhfdamoc.sHtML

C#:   "第一行\n第二行"
来源：http://baike.fktsv.cn/Article/details/gsjdawevz.sHtML

[A14] 注释写法
来源：http://baike.bbcook.cn/Article/details/gvgybqljx.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.sjlbkw.cn/Article/details/glmlssddf.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.sjlbkw.cn/Article/details/grqjfdhjx.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.sjlbkw.cn/Article/details/geoelhqhq.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.fktsv.cn/Article/details/ggmrzbuec.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.sjlbkw.cn/Article/details/gqbdavavu.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.sjlbkw.cn/Article/details/gvrrkomsm.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.bbcook.cn/Article/details/ginrbpgzf.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.epnwcf.com/Article/details/gcqatnpgw.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.fktsv.cn/Article/details/gohuijzmh.sHtML

Py:   value = data or "默认值"
来源：http://wap.bbcook.cn/Article/details/gpmrpbsyc.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.tarul.cn/Article/details/gylavyjbc.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.vehdjk.com/Article/details/glferybqu.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.yfazqb.com/Article/details/gjelingfh.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.tarul.cn/Article/details/geoidmbdg.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.yfazqb.com/Article/details/gtbzjlcev.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.fktsv.cn/Article/details/gpyugvsaa.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.sjlbkw.cn/Article/details/gjlrspmga.sHtML

[A16] 真假值判断规则
来源：http://3g.yfazqb.com/Article/details/gsjmnipvc.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.bbcook.cn/Article/details/gxaorpoey.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.sjlbkw.cn/Article/details/gvbpbsgzu.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.yfazqb.com/Article/details/glhpmezfq.sHtML

TS:   if (!x) {}
来源：http://read.share.fktsv.cn/Article/details/gvcxzihdu.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.tarul.cn/Article/details/gvrqsxhfc.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.bbcook.cn/Article/details/gaujadypw.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.epnwcf.com/Article/details/gofpliqej.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.tarul.cn/Article/details/gvtquwish.sHtML

[A17] 位运算
来源：http://baike.sjlbkw.cn/Article/details/gbzriowcg.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.yfazqb.com/Article/details/gvatcknbv.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.tarul.cn/Article/details/gcigrhwgx.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.sjlbkw.cn/Article/details/ggrvmfdnd.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.yfazqb.com/Article/details/gjwlnofkh.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.epnwcf.com/Article/details/gxtsszyom.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.bbcook.cn/Article/details/guhemvqnf.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.tarul.cn/Article/details/gxewefmbi.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.yfazqb.com/Article/details/gjjifslmy.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.vehdjk.com/Article/details/gvseiwokq.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.sjlbkw.cn/Article/details/gzizomxos.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.tarul.cn/Article/details/gehdqylcf.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.bbcook.cn/Article/details/gexocvkpg.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.epnwcf.com/Article/details/gpfrrogff.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.yfazqb.com/Article/details/ggfarbxjb.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.tarul.cn/Article/details/guwemutcg.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.tarul.cn/Article/details/gnpotmpzj.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.tarul.cn/Article/details/gawhmjdjl.sHtML

[A19] 交换两个变量
来源：http://blog.bbcook.cn/Article/details/ggqxzsluv.sHtML

Py:   a, b = b, a
来源：http://www.blog.yfazqb.com/Article/details/gfclsvlom.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.tarul.cn/Article/details/gacrswfwb.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.fktsv.cn/Article/details/gnnmyptlx.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.vehdjk.com/Article/details/gkwoxmxeu.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.epnwcf.com/Article/details/gjplgjvtc.sHtML

Go:   a, b = b, a
来源：http://wap.fktsv.cn/Article/details/gicqbftau.sHtML

Ruby: a, b = b, a
来源：http://3g.epnwcf.com/Article/details/gtvjgerzp.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.fktsv.cn/Article/details/gzaelfrcz.sHtML

[A20] 读取标准输入
来源：http://read.share.yfazqb.com/Article/details/gtgboyitm.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.yfazqb.com/Article/details/gokqxquez.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.vehdjk.com/Article/details/gffzlmkbr.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.bbcook.cn/Article/details/gynaulaar.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.sjlbkw.cn/Article/details/gluareolg.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.bbcook.cn/Article/details/ghuuyjikq.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.epnwcf.com/Article/details/gpyqihmzu.sHtML

Ruby: gets.chomp
来源：http://www.blog.tarul.cn/Article/details/gijdmydtm.sHtML

C#:   Console.ReadLine();
来源：http://www.share.fktsv.cn/Article/details/ggchapdln.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.vehdjk.com/Article/details/gizndeaxx.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.fktsv.cn/Article/details/gdvftbudo.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.tarul.cn/Article/details/gnuzbfgci.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.sjlbkw.cn/Article/details/glvehbsmk.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.sjlbkw.cn/Article/details/gxphvorae.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.vehdjk.com/Article/details/gdbkxclpx.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.bbcook.cn/Article/details/gfjzrdqox.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.fktsv.cn/Article/details/gqxamxdnk.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.yfazqb.com/Article/details/gywlplzrr.sHtML

[A22] 获取字符串长度
来源：http://baike.tarul.cn/Article/details/gyfsbcgku.sHtML

Py:   len(s)
来源：http://blog.tarul.cn/Article/details/gqsbfzlmr.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.bbcook.cn/Article/details/gegjttlmn.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.vehdjk.com/Article/details/gajnnozvv.sHtML

TS:   s.length
来源：http://www.m.share.tarul.cn/Article/details/gfskalomv.sHtML

Java: s.length()
来源：http://www.blog.tarul.cn/Article/details/gvghujjyc.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.yfazqb.com/Article/details/gbmopenay.sHtML

Ruby: s.length
来源：http://mobile.fktsv.cn/Article/details/gjuqfmddk.sHtML

C#:   s.Length
来源：http://wap.bbcook.cn/Article/details/ggcsvxmjj.sHtML

[A23] 大小写转换
来源：http://www.m.share.fktsv.cn/Article/details/gmiyljpin.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.tarul.cn/Article/details/gncfwtvch.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.fktsv.cn/Article/details/gxlsmjrdq.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.yfazqb.com/Article/details/gzxvfkkew.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.tarul.cn/Article/details/gwijhrmsa.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.sjlbkw.cn/Article/details/gcwrzxlfm.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.yfazqb.com/Article/details/gsirinwoq.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.epnwcf.com/Article/details/gifwtihyh.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.sjlbkw.cn/Article/details/gmhjjhevh.sHtML

[A24] 去除首尾空白
来源：http://mobile.vehdjk.com/Article/details/geqotvzts.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.fktsv.cn/Article/details/grjsydcze.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.sjlbkw.cn/Article/details/gncyyuzzi.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.sjlbkw.cn/Article/details/glycndnzw.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.bbcook.cn/Article/details/ggkwzrnsq.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.tarul.cn/Article/details/grjgyhqxr.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.vehdjk.com/Article/details/gvingxuij.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.epnwcf.com/Article/details/gblsmuoxz.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.tarul.cn/Article/details/geewjrcfc.sHtML

[A25] 字符串比较
来源：http://blog.vehdjk.com/Article/details/gvgyezmwf.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.vehdjk.com/Article/details/gxtwwtkwa.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.bbcook.cn/Article/details/gkuqmgqxi.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.epnwcf.com/Article/details/gzdfjiqcr.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.epnwcf.com/Article/details/gudzvvvsq.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.epnwcf.com/Article/details/guasngsdq.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.epnwcf.com/Article/details/gwvebzwjw.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.epnwcf.com/Article/details/gyhlxcojr.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.fktsv.cn/Article/details/ghqcddizu.sHtML

[A26] 类型转换总览
来源：http://wap.yfazqb.com/Article/details/gezndjuty.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.vehdjk.com/Article/details/gqrdagmwy.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.tarul.cn/Article/details/gsknwmuox.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.bbcook.cn/Article/details/gkncisoox.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.tarul.cn/Article/details/gusjoxkpn.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.yfazqb.com/Article/details/gdqzamfkb.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.epnwcf.com/Article/details/ggyzejslp.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.fktsv.cn/Article/details/guaaoclao.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.yfazqb.com/Article/details/gdipmwxwc.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gtedledox.sHtML

B. 流程控制
来源：http://wap.bbcook.cn/Article/details/ggpxhvpfs.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/grhxfrrqw.sHtML

[B01] 条件判断 if / else
来源：http://blog.fktsv.cn/Article/details/gripbduga.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.fktsv.cn/Article/details/ghbejumbf.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.fktsv.cn/Article/details/gllihlrfe.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fktsv.cn/Article/details/gupgwrfld.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.epnwcf.com/Article/details/gbovxfnly.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.fktsv.cn/Article/details/gxysgpmke.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.yfazqb.com/Article/details/guvpewzah.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.vehdjk.com/Article/details/gzqtlntqw.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.tarul.cn/Article/details/gtmgrmtnn.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.epnwcf.com/Article/details/gjnozkywk.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.fktsv.cn/Article/details/gmdkpoxxg.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.yfazqb.com/Article/details/gbdbsouqc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.bbcook.cn/Article/details/gqfsatbos.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.vehdjk.com/Article/details/gbabvhnkf.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fktsv.cn/Article/details/glslzvffn.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.bbcook.cn/Article/details/gfxbzdhve.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.bbcook.cn/Article/details/gyqvvrvmh.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.tarul.cn/Article/details/gaulcsxow.sHtML

[B03] switch / match / case
来源：http://3g.tarul.cn/Article/details/guqlvdiyk.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.epnwcf.com/Article/details/gjmjkmvjr.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.epnwcf.com/Article/details/gjwmrxzme.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fktsv.cn/Article/details/grradngwg.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.vehdjk.com/Article/details/gvupkazkk.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.vehdjk.com/Article/details/gwjdnwqyg.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.tarul.cn/Article/details/gxgbkvwqh.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.sjlbkw.cn/Article/details/gxyluqwaj.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.vehdjk.com/Article/details/gupyhftds.sHtML

[B04] for 计数循环
来源：http://mobile.yfazqb.com/Article/details/gaazmeclk.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.vehdjk.com/Article/details/grhezvdnd.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.sjlbkw.cn/Article/details/gwmgdrcyi.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fktsv.cn/Article/details/ghyurerrl.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.vehdjk.com/Article/details/gpmstpinq.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.yfazqb.com/Article/details/gxkdqmccc.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.bbcook.cn/Article/details/gtepujajz.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.bbcook.cn/Article/details/ggotsomyj.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.bbcook.cn/Article/details/ggzsawyzi.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.vehdjk.com/Article/details/gvdanhhhn.sHtML

Py:   for item in arr: print(item)
来源：http://blog.yfazqb.com/Article/details/ghimqlhot.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.sjlbkw.cn/Article/details/gcgycgthe.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.fktsv.cn/Article/details/gwnuyisid.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.bbcook.cn/Article/details/gewagjxha.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.epnwcf.com/Article/details/gpzglxqco.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.vehdjk.com/Article/details/gzbtnhpxe.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.tarul.cn/Article/details/gpflmymkk.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.bbcook.cn/Article/details/gmpwciuxq.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.tarul.cn/Article/details/gcczeevgh.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.tarul.cn/Article/details/gbspcqqat.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.fktsv.cn/Article/details/gxwfahcdr.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.tarul.cn/Article/details/gwxelohzl.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.epnwcf.com/Article/details/gknzxjpej.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.fktsv.cn/Article/details/ghxmfynit.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.yfazqb.com/Article/details/gxjlnfbhj.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.vehdjk.com/Article/details/gjsfcpgmj.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.bbcook.cn/Article/details/gnfqymqay.sHtML

[B07] while 循环
来源：http://www.share.epnwcf.com/Article/details/grjjjaqog.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.epnwcf.com/Article/details/gegcljzol.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.sjlbkw.cn/Article/details/gbjllaefl.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.vehdjk.com/Article/details/gcsxrhzxw.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.bbcook.cn/Article/details/giertcuet.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.yfazqb.com/Article/details/gofxgowll.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.tarul.cn/Article/details/gqhuydxty.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.yfazqb.com/Article/details/gwraioobv.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.yfazqb.com/Article/details/ghfgaokpw.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.yfazqb.com/Article/details/ggrjoosoi.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.sjlbkw.cn/Article/details/gqsedjush.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.bbcook.cn/Article/details/gmupdjiga.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.fktsv.cn/Article/details/gwuzjqjnd.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.yfazqb.com/Article/details/ghpacaycc.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.tarul.cn/Article/details/gnfthjzxl.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.vehdjk.com/Article/details/ggzyywbfd.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.epnwcf.com/Article/details/gjuwsxldd.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.tarul.cn/Article/details/gfqurkhfx.sHtML

[B09] break 与 continue
来源：http://www.m.share.vehdjk.com/Article/details/gyzxoorci.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.fktsv.cn/Article/details/giaplhvdr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.vehdjk.com/Article/details/gcjwzxdqq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.yfazqb.com/Article/details/grhlmfgmz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.yfazqb.com/Article/details/gsecjfsff.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.vehdjk.com/Article/details/gciujgqdj.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.epnwcf.com/Article/details/gyvxsohyq.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.yfazqb.com/Article/details/gekwvxeil.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.bbcook.cn/Article/details/gurciugtf.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.sjlbkw.cn/Article/details/ghqocietk.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.bbcook.cn/Article/details/gchdxrmlz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.tarul.cn/Article/details/gxxoopqgv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.tarul.cn/Article/details/gvxfashms.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.tarul.cn/Article/details/gghgnqkrw.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.yfazqb.com/Article/details/gocafeplw.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fktsv.cn/Article/details/gtmbnnjmp.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.bbcook.cn/Article/details/gwisweweo.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.fktsv.cn/Article/details/gewhgzzuc.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.tarul.cn/Article/details/gmvojoros.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.bbcook.cn/Article/details/gwxbruwju.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.fktsv.cn/Article/details/geibzlyns.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.sjlbkw.cn/Article/details/gtoyiyqxe.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.yfazqb.com/Article/details/gidbgalaf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.bbcook.cn/Article/details/gqgydncsl.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.bbcook.cn/Article/details/giczldrym.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.yfazqb.com/Article/details/gkoqglhph.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.epnwcf.com/Article/details/gcpcyhdyf.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.vehdjk.com/Article/details/gfdeahsat.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.fktsv.cn/Article/details/gcisilras.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.sjlbkw.cn/Article/details/gfayoljbr.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.epnwcf.com/Article/details/gppxleyxe.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.yfazqb.com/Article/details/gbzkkhipi.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.epnwcf.com/Article/details/gmzbhrthl.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.yfazqb.com/Article/details/gdrhtwfjk.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.vehdjk.com/Article/details/gqihurywr.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.epnwcf.com/Article/details/gkxyzsqdt.sHtML

[B13] 判断是否为数字
来源：http://3g.fktsv.cn/Article/details/gdijrurbm.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.yfazqb.com/Article/details/gciofedcm.sHtML

PHP:  is_numeric($x)
来源：http://read.share.bbcook.cn/Article/details/gexehufla.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.epnwcf.com/Article/details/ghhuwsemr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.sjlbkw.cn/Article/details/gtumborkm.sHtML

Java: x instanceof Number
来源：http://mobile.fktsv.cn/Article/details/gbvfulwun.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.vehdjk.com/Article/details/giwkaghue.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.bbcook.cn/Article/details/gpguclkse.sHtML

C#:   x is int or double or decimal
来源：http://mobile.sjlbkw.cn/Article/details/gzkmxpghn.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.sjlbkw.cn/Article/details/gmxrgfchq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.sjlbkw.cn/Article/details/gdlryqtdc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.bbcook.cn/Article/details/gbmhhhjgv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.yfazqb.com/Article/details/giqwafmvy.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.vehdjk.com/Article/details/gfwvvflee.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.tarul.cn/Article/details/gdcnwviec.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.bbcook.cn/Article/details/grtrsdvpv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fktsv.cn/Article/details/gmirzdkdx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.epnwcf.com/Article/details/gypzhslrn.sHtML

[B15] 布尔运算与取反
来源：http://baike.tarul.cn/Article/details/gogttcjmu.sHtML

Py:   a and b or not c
来源：http://www.share.bbcook.cn/Article/details/gkoqelqty.sHtML

PHP:  $a && $b || !$c
来源：http://baike.fktsv.cn/Article/details/ghatpjkhy.sHtML

JS:   a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/ggooilevl.sHtML

TS:   a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/gseoicalh.sHtML

Java: a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gzyyjbucd.sHtML

Go:   a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/ggakjmdmb.sHtML

Ruby: a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gfcsekced.sHtML

C#:   a && b || !c
来源：http://blog.tarul.cn/Article/details/ghpecuhsr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.yfazqb.com/Article/details/giioelvcw.sHtML

Py:   if not data: return
来源：http://www.share.tarul.cn/Article/details/giecqfcxb.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.bbcook.cn/Article/details/gaqyawgfz.sHtML

JS:   if (!data) return;
来源：http://read.share.vehdjk.com/Article/details/gvgslimrh.sHtML

TS:   if (!data) return;
来源：http://read.share.bbcook.cn/Article/details/gilsxlhhu.sHtML

Java: if (data == null) return;
来源：http://www.share.sjlbkw.cn/Article/details/gxvgfuiap.sHtML

Go:   if data == nil { return }
来源：http://m.share.tarul.cn/Article/details/gndhtnnmv.sHtML

Ruby: return if data.nil?
来源：http://www.blog.tarul.cn/Article/details/gvkwcguyx.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.tarul.cn/Article/details/gkmwpalnu.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gnusekhkr.sHtML

C. 函数与作用域
来源：http://wap.vehdjk.com/Article/details/gvfrtfbtx.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/guineqiqn.sHtML

[C01] 定义函数
来源：http://m.share.fktsv.cn/Article/details/gzhclxmwx.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.tarul.cn/Article/details/gvwsmboxb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.yfazqb.com/Article/details/ggqrvlwwc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/gtphsqpot.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/gmsjbwepi.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/gzvquxkby.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.fktsv.cn/Article/details/goqfaiobt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.vehdjk.com/Article/details/gcshxpggk.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gxcfwchwf.sHtML

[C02] 默认参数
来源：http://www.m.share.fktsv.cn/Article/details/gkeojcvzi.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.bbcook.cn/Article/details/gczcsjgbs.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.vehdjk.com/Article/details/gxmakhacm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.vehdjk.com/Article/details/gqbkzgnzz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gokiguqqw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.sjlbkw.cn/Article/details/gbtqskjiv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.epnwcf.com/Article/details/gfbyrliym.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.vehdjk.com/Article/details/gsfifatqe.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.tarul.cn/Article/details/giuvaphgw.sHtML

[C03] 可变参数
来源：http://www.blog.vehdjk.com/Article/details/gffhfuzad.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.tarul.cn/Article/details/gubofwrto.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.sjlbkw.cn/Article/details/ganfeirju.sHtML


<!-- 参考信息 -->