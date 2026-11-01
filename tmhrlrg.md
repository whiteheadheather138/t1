代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.epnwcf.com/Article/details/gvzmhagda.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fktsv.cn/Article/details/gpjcjgizc.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.sjlbkw.cn/Article/details/gjgtcglod.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.sjlbkw.cn/Article/details/goazuizna.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.sjlbkw.cn/Article/details/gcqxnzhjv.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.sjlbkw.cn/Article/details/gktqwjbnd.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.bbcook.cn/Article/details/gpnbqsphx.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.tarul.cn/Article/details/guukjmneh.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.yfazqb.com/Article/details/gudylxsfd.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.fktsv.cn/Article/details/grcidihqw.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.fktsv.cn/Article/details/ggpibtdtj.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.tarul.cn/Article/details/gjpeuotnz.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.tarul.cn/Article/details/gyrebfnzj.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.bbcook.cn/Article/details/gsnwasgib.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.bbcook.cn/Article/details/ghqgzoaau.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.sjlbkw.cn/Article/details/gkqiggxpn.sHtML

Java: "第一行\n第二行"
来源：http://read.share.tarul.cn/Article/details/gvuxxhjum.sHtML

Go:   "第一行\n第二行"
来源：http://baike.tarul.cn/Article/details/gdjooocyv.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.sjlbkw.cn/Article/details/gvoldznin.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.sjlbkw.cn/Article/details/gfjwvhxlv.sHtML

[A14] 注释写法
来源：http://m.share.bbcook.cn/Article/details/gzkklnsch.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.bbcook.cn/Article/details/gdtrrlpvd.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.bbcook.cn/Article/details/guikjotbu.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.sjlbkw.cn/Article/details/glpacibkx.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.bbcook.cn/Article/details/glkudsdjl.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.sjlbkw.cn/Article/details/glkyinlgh.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.tarul.cn/Article/details/gfbhxnush.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.fktsv.cn/Article/details/ghumdbmci.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.sjlbkw.cn/Article/details/gubpwagyp.sHtML

[A15] 空值判断与默认值
来源：http://wap.tarul.cn/Article/details/gmdbnqtln.sHtML

Py:   value = data or "默认值"
来源：http://blog.sjlbkw.cn/Article/details/ghqbllomy.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.bbcook.cn/Article/details/gxvppezhh.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.yfazqb.com/Article/details/gyfwspbqs.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.sjlbkw.cn/Article/details/gcokprgig.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.sjlbkw.cn/Article/details/gaktbswjl.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.yfazqb.com/Article/details/glhrwnaes.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.yfazqb.com/Article/details/gbxsjikvz.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.sjlbkw.cn/Article/details/gzscdeujz.sHtML

[A16] 真假值判断规则
来源：http://www.blog.vehdjk.com/Article/details/gaspkcpsz.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.tarul.cn/Article/details/glxfjkulx.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.yfazqb.com/Article/details/gcvjlnvwj.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.epnwcf.com/Article/details/gjwfxvfcv.sHtML

TS:   if (!x) {}
来源：http://www.share.bbcook.cn/Article/details/giuylqtoa.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.epnwcf.com/Article/details/gpjzposmn.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.vehdjk.com/Article/details/gxnzthern.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.bbcook.cn/Article/details/gjerxubfy.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.epnwcf.com/Article/details/gguvnfqvv.sHtML

[A17] 位运算
来源：http://wap.tarul.cn/Article/details/gmhsqnlbd.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.yfazqb.com/Article/details/gntcphvjh.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.tarul.cn/Article/details/glqdgjjmw.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.vehdjk.com/Article/details/ggdtvkbke.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.tarul.cn/Article/details/glbfibisd.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.bbcook.cn/Article/details/gquntazxo.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.epnwcf.com/Article/details/gzmipwkmf.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.bbcook.cn/Article/details/gfktpwdgy.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.epnwcf.com/Article/details/gevwnkjug.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.bbcook.cn/Article/details/gjcdkhhmp.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.epnwcf.com/Article/details/gyhpyenfy.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.epnwcf.com/Article/details/gkdnahxia.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.bbcook.cn/Article/details/gqxmebdtp.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.sjlbkw.cn/Article/details/gvxrucyha.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.yfazqb.com/Article/details/gluqhdnxq.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.fktsv.cn/Article/details/gkgkpzoxs.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.sjlbkw.cn/Article/details/ghneompsi.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.bbcook.cn/Article/details/gzxutlocw.sHtML

[A19] 交换两个变量
来源：http://read.share.bbcook.cn/Article/details/gihrbrzkf.sHtML

Py:   a, b = b, a
来源：http://www.m.share.sjlbkw.cn/Article/details/giodqweoq.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.sjlbkw.cn/Article/details/gowzxwenm.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.fktsv.cn/Article/details/gspywqjfg.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.yfazqb.com/Article/details/gkfpzlkha.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.sjlbkw.cn/Article/details/graagucnz.sHtML

Go:   a, b = b, a
来源：http://www.share.yfazqb.com/Article/details/gtifpobxt.sHtML

Ruby: a, b = b, a
来源：http://www.share.tarul.cn/Article/details/gixqujmfj.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.bbcook.cn/Article/details/gmvkhvgel.sHtML

[A20] 读取标准输入
来源：http://m.share.epnwcf.com/Article/details/gyoywmqpe.sHtML

Py:   name = input("请输入：")
来源：http://3g.yfazqb.com/Article/details/gqkhrrvxr.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.fktsv.cn/Article/details/gcsgiruiy.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.share.bbcook.cn/Article/details/gryxkeicm.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.sjlbkw.cn/Article/details/gayvnronl.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.tarul.cn/Article/details/gyuphkwpa.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.yfazqb.com/Article/details/gcgvsgfxr.sHtML

Ruby: gets.chomp
来源：http://baike.yfazqb.com/Article/details/geauftpgn.sHtML

C#:   Console.ReadLine();
来源：http://3g.sjlbkw.cn/Article/details/gdpwybyae.sHtML

[A21] 保留指定小数位输出
来源：http://blog.yfazqb.com/Article/details/gibmibsmj.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.yfazqb.com/Article/details/gwgzywodm.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.sjlbkw.cn/Article/details/galzpwlqj.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.bbcook.cn/Article/details/gvolovacc.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.bbcook.cn/Article/details/gedxqhzel.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.tarul.cn/Article/details/gkkdadzxe.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.bbcook.cn/Article/details/gsksabgrw.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.vehdjk.com/Article/details/gjxnjgalx.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.fktsv.cn/Article/details/gdiwkttqc.sHtML

[A22] 获取字符串长度
来源：http://read.share.bbcook.cn/Article/details/gweumvyvz.sHtML

Py:   len(s)
来源：http://baike.sjlbkw.cn/Article/details/gcexyepzg.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.fktsv.cn/Article/details/gupwtnzrk.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.tarul.cn/Article/details/guwoqzvqv.sHtML

TS:   s.length
来源：http://mobile.sjlbkw.cn/Article/details/gimdlukcd.sHtML

Java: s.length()
来源：http://www.share.sjlbkw.cn/Article/details/gserbiymo.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.fktsv.cn/Article/details/gdetshbgt.sHtML

Ruby: s.length
来源：http://read.share.vehdjk.com/Article/details/gjiyzzgzr.sHtML

C#:   s.Length
来源：http://baike.bbcook.cn/Article/details/gqbkdbjox.sHtML

[A23] 大小写转换
来源：http://blog.bbcook.cn/Article/details/gducpfmnt.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.yfazqb.com/Article/details/gdpcgrain.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.yfazqb.com/Article/details/gjpvjzcwn.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.sjlbkw.cn/Article/details/gdciqcaua.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.bbcook.cn/Article/details/gllvgomrq.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.tarul.cn/Article/details/grqkvtaun.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.vehdjk.com/Article/details/gtuxwxgxq.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.tarul.cn/Article/details/gubpwiorq.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.epnwcf.com/Article/details/gruiksute.sHtML

[A24] 去除首尾空白
来源：http://baike.sjlbkw.cn/Article/details/gdymrbdar.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.bbcook.cn/Article/details/gcjeqmudd.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.fktsv.cn/Article/details/gmzxhebmb.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.tarul.cn/Article/details/gpykeuhtv.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.sjlbkw.cn/Article/details/gbqtaanbj.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.fktsv.cn/Article/details/gtefhcsgt.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.tarul.cn/Article/details/gnafilfce.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.yfazqb.com/Article/details/gkiagtcpb.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.tarul.cn/Article/details/gcwtbaspw.sHtML

[A25] 字符串比较
来源：http://wap.fktsv.cn/Article/details/gdgcgvcvn.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.yfazqb.com/Article/details/gmygdkqts.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.vehdjk.com/Article/details/ghibdavuk.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.tarul.cn/Article/details/gqnkrnxrm.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.vehdjk.com/Article/details/gekdbppeh.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.fktsv.cn/Article/details/ghyqocovl.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.tarul.cn/Article/details/gekdmnlyq.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.tarul.cn/Article/details/gafoqokvu.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.fktsv.cn/Article/details/gohgdwrvi.sHtML

[A26] 类型转换总览
来源：http://www.blog.vehdjk.com/Article/details/gaaykjipd.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.epnwcf.com/Article/details/gnasrrndq.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.sjlbkw.cn/Article/details/gruyiuprb.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.vehdjk.com/Article/details/gnfwwwslw.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.bbcook.cn/Article/details/glxfbojdx.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.fktsv.cn/Article/details/gpkphhzlk.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gtcipokez.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.tarul.cn/Article/details/gujdoujvf.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.sjlbkw.cn/Article/details/gjmhrouxm.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gumayrnbb.sHtML

B. 流程控制
来源：http://www.share.vehdjk.com/Article/details/gunbvhyuj.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/glymdkeds.sHtML

[B01] 条件判断 if / else
来源：http://m.share.tarul.cn/Article/details/gxcjepaew.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.epnwcf.com/Article/details/ggrolkgek.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.sjlbkw.cn/Article/details/ghaoqwcfq.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.yfazqb.com/Article/details/gtefqhgyf.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.epnwcf.com/Article/details/grpplfktm.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.bbcook.cn/Article/details/gegaxuqxc.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.sjlbkw.cn/Article/details/glaljsscm.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.fktsv.cn/Article/details/gjqmkdjlq.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.vehdjk.com/Article/details/gxzdejiay.sHtML

[B02] 多分支 else if / elif
来源：http://wap.fktsv.cn/Article/details/gycagmusx.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.vehdjk.com/Article/details/gxshyakgc.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.tarul.cn/Article/details/gsdgtvohs.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.sjlbkw.cn/Article/details/gyxsatuvp.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.tarul.cn/Article/details/gtitnwpnu.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.epnwcf.com/Article/details/gfknpakbv.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.vehdjk.com/Article/details/ghnyvvipg.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.sjlbkw.cn/Article/details/gpymgxrys.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.bbcook.cn/Article/details/gnecedttm.sHtML

[B03] switch / match / case
来源：http://mobile.fktsv.cn/Article/details/gpvzfhvve.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.sjlbkw.cn/Article/details/ghrequkgb.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.fktsv.cn/Article/details/gibmlyehb.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fktsv.cn/Article/details/ggkqqarkf.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fktsv.cn/Article/details/gsnehoryf.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.vehdjk.com/Article/details/gmgabetoy.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.sjlbkw.cn/Article/details/ggfowjzpo.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.tarul.cn/Article/details/gohnlqndy.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.epnwcf.com/Article/details/gczhqwdoi.sHtML

[B04] for 计数循环
来源：http://www.share.fktsv.cn/Article/details/gxdlxkcja.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.bbcook.cn/Article/details/gwkxujzpe.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.epnwcf.com/Article/details/gnfbaghfq.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fktsv.cn/Article/details/gqrqokidi.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.sjlbkw.cn/Article/details/gjsnbltrt.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.bbcook.cn/Article/details/gpwxnncuc.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqnicynfe.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.bbcook.cn/Article/details/ghdfdzlvy.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.bbcook.cn/Article/details/glrmijjhj.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.fktsv.cn/Article/details/ggorynbxz.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.vehdjk.com/Article/details/gdgxljipf.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.yfazqb.com/Article/details/gaydbhpkn.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.yfazqb.com/Article/details/gegkhhvop.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.vehdjk.com/Article/details/gduiopdjh.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.bbcook.cn/Article/details/gvgybbwja.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.sjlbkw.cn/Article/details/graqehres.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.bbcook.cn/Article/details/gjmfgfjfh.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.sjlbkw.cn/Article/details/gmbxqhhil.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.epnwcf.com/Article/details/gbelmpnyy.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.sjlbkw.cn/Article/details/gftyvwwkx.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.tarul.cn/Article/details/gqqjziirc.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.tarul.cn/Article/details/gllcjqbrl.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.vehdjk.com/Article/details/ghayejerz.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.yfazqb.com/Article/details/gxqwlhtol.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.epnwcf.com/Article/details/gtepbjhzn.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.bbcook.cn/Article/details/guidpxtum.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.fktsv.cn/Article/details/gidhzbajv.sHtML

[B07] while 循环
来源：http://baike.yfazqb.com/Article/details/gtdxoytfl.sHtML

Py:   while i < 10: i += 1
来源：http://3g.sjlbkw.cn/Article/details/gubuugigx.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.epnwcf.com/Article/details/goofgjjer.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.vehdjk.com/Article/details/glabkoetc.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.tarul.cn/Article/details/gmvqcbuwz.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.tarul.cn/Article/details/gmxtznjjc.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.yfazqb.com/Article/details/gpcgibwhm.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.epnwcf.com/Article/details/gbfvrepdz.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.sjlbkw.cn/Article/details/gjtidzjsr.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.epnwcf.com/Article/details/ggqszfstb.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.tarul.cn/Article/details/gzsyufjap.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.bbcook.cn/Article/details/gjzixxrbd.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.sjlbkw.cn/Article/details/gnmhszuha.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.yfazqb.com/Article/details/gsqfkxtdz.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.yfazqb.com/Article/details/gdhypqmaz.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.epnwcf.com/Article/details/gbfqjciel.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.tarul.cn/Article/details/gknwumsep.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.vehdjk.com/Article/details/ggnwcjmmo.sHtML

[B09] break 与 continue
来源：http://wap.tarul.cn/Article/details/gkeebewzt.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.bbcook.cn/Article/details/gbkgdtbik.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.tarul.cn/Article/details/gpxjuivic.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.epnwcf.com/Article/details/grhdwxvcm.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.vehdjk.com/Article/details/gcsqexnfo.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.tarul.cn/Article/details/gtkvujguz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.epnwcf.com/Article/details/gynkwsmjs.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.tarul.cn/Article/details/gnoxhpfjz.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.bbcook.cn/Article/details/guwypwtqy.sHtML

[B10] 遍历同时拿索引
来源：http://baike.tarul.cn/Article/details/ggtqcbeuj.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.epnwcf.com/Article/details/gthkifems.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.yfazqb.com/Article/details/gueawtzmy.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.epnwcf.com/Article/details/gbxhskynj.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.epnwcf.com/Article/details/goclpujqx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.fktsv.cn/Article/details/gulhtkxah.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.epnwcf.com/Article/details/gubaaegxr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.fktsv.cn/Article/details/gddzjpmrj.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.epnwcf.com/Article/details/goijotaml.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.vehdjk.com/Article/details/gzcqwuhgn.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.epnwcf.com/Article/details/gvwjymmuu.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.sjlbkw.cn/Article/details/geprsnfai.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.sjlbkw.cn/Article/details/gattmdqqw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.tarul.cn/Article/details/groyksirb.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gpemsumly.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.tarul.cn/Article/details/glqwwlwmg.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.tarul.cn/Article/details/gmzaiwqlt.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.fktsv.cn/Article/details/grvgtdejl.sHtML

[B12] 跳出多层循环
来源：http://m.share.yfazqb.com/Article/details/gqwxkdqgf.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.yfazqb.com/Article/details/gqeegqvkw.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.vehdjk.com/Article/details/gysxzptiv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.vehdjk.com/Article/details/gjbkmjtvi.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.yfazqb.com/Article/details/gvvtxubbp.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.vehdjk.com/Article/details/gtpzgdrbm.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.vehdjk.com/Article/details/ghwpeqbse.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.bbcook.cn/Article/details/gthbcxxrk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.sjlbkw.cn/Article/details/gbgmlbhcs.sHtML

[B13] 判断是否为数字
来源：http://m.share.tarul.cn/Article/details/guognuurh.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.yfazqb.com/Article/details/gicmnmedi.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fktsv.cn/Article/details/gogyhjkhn.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.sjlbkw.cn/Article/details/gwbbsfdey.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.epnwcf.com/Article/details/gncznvjyl.sHtML

Java: x instanceof Number
来源：http://wap.vehdjk.com/Article/details/gfiokputa.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.vehdjk.com/Article/details/gkfqhizuw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.tarul.cn/Article/details/gctwwdlwo.sHtML

C#:   x is int or double or decimal
来源：http://baike.yfazqb.com/Article/details/gfbwamydq.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.bbcook.cn/Article/details/gxdmszwtr.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.epnwcf.com/Article/details/gwfuotkhy.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.tarul.cn/Article/details/gwhqfvdbw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.vehdjk.com/Article/details/guwnaotub.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.epnwcf.com/Article/details/ghvmhqqbg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.sjlbkw.cn/Article/details/gydsxkbnz.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.epnwcf.com/Article/details/gsltlibkx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.fktsv.cn/Article/details/gghjtvqbm.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.yfazqb.com/Article/details/gqauwtsjr.sHtML

[B15] 布尔运算与取反
来源：http://baike.epnwcf.com/Article/details/gxiuksjtj.sHtML

Py:   a and b or not c
来源：http://www.share.tarul.cn/Article/details/guyfoimul.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.sjlbkw.cn/Article/details/gxfpkhujb.sHtML

JS:   a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/gniytlbky.sHtML

TS:   a && b || !c
来源：http://read.share.tarul.cn/Article/details/gvgshdamd.sHtML

Java: a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gumqcerab.sHtML

Go:   a && b || !c
来源：http://wap.vehdjk.com/Article/details/gdhjiistc.sHtML

Ruby: a && b || !c
来源：http://wap.vehdjk.com/Article/details/guzuzxivs.sHtML

C#:   a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/gepaennrk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.tarul.cn/Article/details/gkhethnxu.sHtML

Py:   if not data: return
来源：http://3g.fktsv.cn/Article/details/glknkcttg.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.bbcook.cn/Article/details/gfacxbfwa.sHtML

JS:   if (!data) return;
来源：http://blog.sjlbkw.cn/Article/details/gkfjqxndm.sHtML

TS:   if (!data) return;
来源：http://mobile.fktsv.cn/Article/details/gdhtvcfod.sHtML

Java: if (data == null) return;
来源：http://blog.vehdjk.com/Article/details/gyysazlfn.sHtML

Go:   if data == nil { return }
来源：http://mobile.sjlbkw.cn/Article/details/gsvtoplod.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.bbcook.cn/Article/details/gjaliyuzm.sHtML

C#:   if (data == null) return;
来源：http://wap.sjlbkw.cn/Article/details/glovbdysb.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gyaxuvcfl.sHtML

C. 函数与作用域
来源：http://3g.bbcook.cn/Article/details/gqhuyfoer.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gtczcjuxu.sHtML

[C01] 定义函数
来源：http://www.blog.fktsv.cn/Article/details/gptgyhhsk.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.yfazqb.com/Article/details/gdjblrtcv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.bbcook.cn/Article/details/gafmfwvys.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gpknljslw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gpuvakerm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/ghcdnvoxc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.vehdjk.com/Article/details/gouyjykon.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.tarul.cn/Article/details/gumzqkvvq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdjdsnnjw.sHtML

[C02] 默认参数
来源：http://blog.sjlbkw.cn/Article/details/gaccpgbxc.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.sjlbkw.cn/Article/details/gpqjutnzb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.sjlbkw.cn/Article/details/gchtbdedn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.bbcook.cn/Article/details/gjhtwvywk.sHtML


<!-- 参考信息 -->