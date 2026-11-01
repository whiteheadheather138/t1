代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.fktsv.cn/Article/details/gsxmymivd.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.yfazqb.com/Article/details/gyxrtksgi.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.bbcook.cn/Article/details/ggaysitru.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.tarul.cn/Article/details/gpezqrnyh.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.tarul.cn/Article/details/gdvdufajn.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.vehdjk.com/Article/details/gymqbcnav.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.bbcook.cn/Article/details/gskzwoowb.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.yfazqb.com/Article/details/gognztpvk.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.yfazqb.com/Article/details/gttsbakuq.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.tarul.cn/Article/details/gfjcqayjb.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.tarul.cn/Article/details/gxejnewzm.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.epnwcf.com/Article/details/gpxpvdgln.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.epnwcf.com/Article/details/gmwuimtyj.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.epnwcf.com/Article/details/gaoayfzdt.sHtML

JS:   "第一行\n第二行"
来源：http://blog.sjlbkw.cn/Article/details/giebcdrju.sHtML

TS:   "第一行\n第二行"
来源：http://www.blog.yfazqb.com/Article/details/gliprdwof.sHtML

Java: "第一行\n第二行"
来源：http://www.share.vehdjk.com/Article/details/gfpqpxyim.sHtML

Go:   "第一行\n第二行"
来源：http://baike.sjlbkw.cn/Article/details/gcymdiqag.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.yfazqb.com/Article/details/gtangjuts.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.yfazqb.com/Article/details/gwhybhxjo.sHtML

[A14] 注释写法
来源：http://www.blog.bbcook.cn/Article/details/gymovjdvm.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.bbcook.cn/Article/details/gsjyuptlg.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.yfazqb.com/Article/details/ghpubzbbg.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.sjlbkw.cn/Article/details/gefykprqg.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.yfazqb.com/Article/details/gszbliuvz.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.sjlbkw.cn/Article/details/gzkzcwjuc.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.bbcook.cn/Article/details/gblbidmru.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.epnwcf.com/Article/details/gfseegczk.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.fktsv.cn/Article/details/gpacsajrd.sHtML

[A15] 空值判断与默认值
来源：http://blog.yfazqb.com/Article/details/ghvghtpam.sHtML

Py:   value = data or "默认值"
来源：http://3g.bbcook.cn/Article/details/grtkzltgi.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.bbcook.cn/Article/details/gqppibmrp.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.yfazqb.com/Article/details/gtqvwnisc.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.sjlbkw.cn/Article/details/gplnlanyr.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://read.share.epnwcf.com/Article/details/gpqgxatgy.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.epnwcf.com/Article/details/gjqxmibxq.sHtML

Ruby: value = data || "默认值"
来源：http://blog.yfazqb.com/Article/details/ggotixnel.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.bbcook.cn/Article/details/garunuwcf.sHtML

[A16] 真假值判断规则
来源：http://m.share.fktsv.cn/Article/details/gixdrglje.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.yfazqb.com/Article/details/glgmrxywp.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.epnwcf.com/Article/details/gbvvsrvqz.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.yfazqb.com/Article/details/gyzxiwnzq.sHtML

TS:   if (!x) {}
来源：http://www.blog.yfazqb.com/Article/details/gdvafvjio.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.vehdjk.com/Article/details/gxhrfbqji.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.fktsv.cn/Article/details/giioxvape.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.vehdjk.com/Article/details/gbsyateqs.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.bbcook.cn/Article/details/gwuphmbcu.sHtML

[A17] 位运算
来源：http://m.share.sjlbkw.cn/Article/details/gktvppuml.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.epnwcf.com/Article/details/gxqlmfdck.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.fktsv.cn/Article/details/gefoejjzr.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.tarul.cn/Article/details/gvfrhmdxh.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.tarul.cn/Article/details/ggzclzzas.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.bbcook.cn/Article/details/gqtpqkwez.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.fktsv.cn/Article/details/gpfyzginh.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.epnwcf.com/Article/details/gdwovdcnv.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.bbcook.cn/Article/details/gldocroet.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.vehdjk.com/Article/details/gsxmkacnn.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.tarul.cn/Article/details/gtucwduaj.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.tarul.cn/Article/details/gphnduunh.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.bbcook.cn/Article/details/gyibqkusa.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.tarul.cn/Article/details/gatcbaanu.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.fktsv.cn/Article/details/gmnoqfexa.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.fktsv.cn/Article/details/gcwgdknkq.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.sjlbkw.cn/Article/details/gpuwygxnu.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.vehdjk.com/Article/details/gyizpnorh.sHtML

[A19] 交换两个变量
来源：http://3g.vehdjk.com/Article/details/gajsrchgi.sHtML

Py:   a, b = b, a
来源：http://www.blog.bbcook.cn/Article/details/gszeubqcs.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.bbcook.cn/Article/details/gtjmctsxb.sHtML

JS:   [a, b] = [b, a];
来源：http://read.share.yfazqb.com/Article/details/grfrchmch.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.bbcook.cn/Article/details/grymtpofn.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.bbcook.cn/Article/details/glewwxhnx.sHtML

Go:   a, b = b, a
来源：http://wap.sjlbkw.cn/Article/details/goragigsw.sHtML

Ruby: a, b = b, a
来源：http://m.share.yfazqb.com/Article/details/gnuwwpyvj.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.vehdjk.com/Article/details/gkslwajgs.sHtML

[A20] 读取标准输入
来源：http://3g.vehdjk.com/Article/details/ghbaonuqe.sHtML

Py:   name = input("请输入：")
来源：http://3g.sjlbkw.cn/Article/details/gbeqqnazr.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.tarul.cn/Article/details/gieecbwki.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.epnwcf.com/Article/details/gjsmilwiw.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.fktsv.cn/Article/details/gaswwvumn.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.yfazqb.com/Article/details/gqcrpbcxy.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.tarul.cn/Article/details/gnyclfgjb.sHtML

Ruby: gets.chomp
来源：http://3g.fktsv.cn/Article/details/govuiahfu.sHtML

C#:   Console.ReadLine();
来源：http://www.share.yfazqb.com/Article/details/gleoancfi.sHtML

[A21] 保留指定小数位输出
来源：http://baike.sjlbkw.cn/Article/details/gmjdvkftp.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.bbcook.cn/Article/details/ghalgmjgz.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.fktsv.cn/Article/details/gywzwepeg.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.fktsv.cn/Article/details/gsvkzlwhl.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.sjlbkw.cn/Article/details/grevuycqa.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.vehdjk.com/Article/details/gkrmlehrj.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.tarul.cn/Article/details/gktocejgf.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.bbcook.cn/Article/details/gsofjapxo.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.epnwcf.com/Article/details/gyniqclir.sHtML

[A22] 获取字符串长度
来源：http://3g.tarul.cn/Article/details/glpmwtlau.sHtML

Py:   len(s)
来源：http://www.blog.epnwcf.com/Article/details/gdbflcuvf.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.fktsv.cn/Article/details/ghldzcubt.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.vehdjk.com/Article/details/gtobwjjnj.sHtML

TS:   s.length
来源：http://read.share.bbcook.cn/Article/details/gajqnjgby.sHtML

Java: s.length()
来源：http://www.blog.tarul.cn/Article/details/gniegpema.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.sjlbkw.cn/Article/details/ggkdjcbxb.sHtML

Ruby: s.length
来源：http://www.share.fktsv.cn/Article/details/gvewrqxwg.sHtML

C#:   s.Length
来源：http://blog.fktsv.cn/Article/details/gdxoppuuy.sHtML

[A23] 大小写转换
来源：http://blog.sjlbkw.cn/Article/details/gpqcolbjx.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.epnwcf.com/Article/details/giqfllfqf.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.epnwcf.com/Article/details/gctctosok.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.tarul.cn/Article/details/gatqlkeoo.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.sjlbkw.cn/Article/details/gqnzrisbo.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.sjlbkw.cn/Article/details/gtzvmobvr.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.vehdjk.com/Article/details/gbpfbtdrb.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.sjlbkw.cn/Article/details/gwxwdtbjn.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.vehdjk.com/Article/details/gxsszttrq.sHtML

[A24] 去除首尾空白
来源：http://blog.sjlbkw.cn/Article/details/gpklurtah.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.bbcook.cn/Article/details/gjwljyvhs.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.vehdjk.com/Article/details/gdpmmwqgd.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.tarul.cn/Article/details/gunwwavnp.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.tarul.cn/Article/details/gmerxicmi.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.bbcook.cn/Article/details/gzxkfxeeq.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.fktsv.cn/Article/details/gvooydxly.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.fktsv.cn/Article/details/ghjtqutnw.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.tarul.cn/Article/details/gcozyjijx.sHtML

[A25] 字符串比较
来源：http://www.m.share.tarul.cn/Article/details/gsuydbgbs.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.tarul.cn/Article/details/gabvmbpdy.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.tarul.cn/Article/details/gjstccmip.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.yfazqb.com/Article/details/gaghsipwi.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.epnwcf.com/Article/details/geuzwmvpy.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.vehdjk.com/Article/details/glqfpmbdk.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.fktsv.cn/Article/details/gcinhosbg.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.vehdjk.com/Article/details/gajkdfhmz.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.fktsv.cn/Article/details/geprkjkbh.sHtML

[A26] 类型转换总览
来源：http://blog.fktsv.cn/Article/details/gryhqiwvv.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.fktsv.cn/Article/details/grrzimjwu.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.epnwcf.com/Article/details/grejewmxx.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.tarul.cn/Article/details/gywzeqezp.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.sjlbkw.cn/Article/details/gpjccxpbf.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.sjlbkw.cn/Article/details/gdftgoriv.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.epnwcf.com/Article/details/gpanrsdgz.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.yfazqb.com/Article/details/gqqgmfbvn.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.yfazqb.com/Article/details/ghsmubaez.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/guqttnphy.sHtML

B. 流程控制
来源：http://www.share.epnwcf.com/Article/details/gmhofhkvw.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gvijyisii.sHtML

[B01] 条件判断 if / else
来源：http://wap.yfazqb.com/Article/details/gxujguuca.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.vehdjk.com/Article/details/gtnrflgft.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.epnwcf.com/Article/details/gsolfoheo.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.vehdjk.com/Article/details/ghvjeoecl.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.bbcook.cn/Article/details/gjdmjczao.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.sjlbkw.cn/Article/details/gpvgpfpop.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.fktsv.cn/Article/details/gvruikkhj.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.bbcook.cn/Article/details/gwmwqctzq.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.sjlbkw.cn/Article/details/gizoexgdi.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.epnwcf.com/Article/details/gusclzdbq.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.sjlbkw.cn/Article/details/gykwuukvo.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.vehdjk.com/Article/details/gqapwrcin.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.sjlbkw.cn/Article/details/guwbyoqyz.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.sjlbkw.cn/Article/details/guhqywdip.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fktsv.cn/Article/details/gbchssxax.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.epnwcf.com/Article/details/gjusluuzq.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.vehdjk.com/Article/details/ggdooujzm.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.vehdjk.com/Article/details/gxmwcbbwk.sHtML

[B03] switch / match / case
来源：http://www.share.epnwcf.com/Article/details/gbjzxdpee.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.sjlbkw.cn/Article/details/ggwttrgst.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.tarul.cn/Article/details/ggtxtbmxn.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.epnwcf.com/Article/details/gzylayjma.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.sjlbkw.cn/Article/details/gjucjojam.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.tarul.cn/Article/details/gendenqkv.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.yfazqb.com/Article/details/gkqqitfjg.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.yfazqb.com/Article/details/ghrgzpjyd.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.fktsv.cn/Article/details/gvwseeexu.sHtML

[B04] for 计数循环
来源：http://www.m.share.epnwcf.com/Article/details/gdpbqknkh.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.yfazqb.com/Article/details/gnhymbglk.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.yfazqb.com/Article/details/geknkspkt.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.sjlbkw.cn/Article/details/gxatuuysw.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fktsv.cn/Article/details/gsmgozlyu.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.yfazqb.com/Article/details/gesvppajq.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.yfazqb.com/Article/details/gsibwbwgz.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.tarul.cn/Article/details/gyatztbpb.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.yfazqb.com/Article/details/geeaztpfb.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.fktsv.cn/Article/details/gqvdcimuo.sHtML

Py:   for item in arr: print(item)
来源：http://baike.bbcook.cn/Article/details/geovmqfhw.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.yfazqb.com/Article/details/gmxygnwvf.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.vehdjk.com/Article/details/geikhawuh.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.sjlbkw.cn/Article/details/gfrhvmevy.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.fktsv.cn/Article/details/gjtejdayn.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.fktsv.cn/Article/details/gnczwshkl.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.fktsv.cn/Article/details/glomkcrdq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.bbcook.cn/Article/details/grfrikvrc.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.epnwcf.com/Article/details/gllfbhhmd.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.epnwcf.com/Article/details/guiimplwv.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.tarul.cn/Article/details/gdxjscnpc.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.epnwcf.com/Article/details/gttforsmx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fktsv.cn/Article/details/gcrcgrvpm.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.fktsv.cn/Article/details/goxrjlujo.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.epnwcf.com/Article/details/gggffzazm.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.vehdjk.com/Article/details/giblszgfr.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.yfazqb.com/Article/details/gsedymakl.sHtML

[B07] while 循环
来源：http://m.share.bbcook.cn/Article/details/gdgdayehc.sHtML

Py:   while i < 10: i += 1
来源：http://3g.epnwcf.com/Article/details/glzyctywd.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.epnwcf.com/Article/details/gwwknuvgj.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.vehdjk.com/Article/details/gsbluztwt.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.sjlbkw.cn/Article/details/gvznpgeas.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.epnwcf.com/Article/details/ghqtptstn.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.tarul.cn/Article/details/gvtuotqbv.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.epnwcf.com/Article/details/gcokemicw.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.fktsv.cn/Article/details/gvpimtovl.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.fktsv.cn/Article/details/ghhfdgcux.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.bbcook.cn/Article/details/gtdokqyae.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.yfazqb.com/Article/details/gdgewgcll.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.epnwcf.com/Article/details/gostnzyaj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.yfazqb.com/Article/details/gnhqnmtvj.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.epnwcf.com/Article/details/glvwwococ.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.yfazqb.com/Article/details/ghvaovfsu.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.bbcook.cn/Article/details/gtntdnlqf.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.vehdjk.com/Article/details/geqtzmgjw.sHtML

[B09] break 与 continue
来源：http://read.share.epnwcf.com/Article/details/gpxmmnqpw.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fktsv.cn/Article/details/geugvtxlk.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.sjlbkw.cn/Article/details/gwuoplged.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fktsv.cn/Article/details/gokylabpw.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fktsv.cn/Article/details/ggrzajkaq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.sjlbkw.cn/Article/details/gwffqlakx.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.vehdjk.com/Article/details/gedcgjsmo.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.sjlbkw.cn/Article/details/grupjalem.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.yfazqb.com/Article/details/gsumgmbjw.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.sjlbkw.cn/Article/details/gizithtlg.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.tarul.cn/Article/details/gyflklypl.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.bbcook.cn/Article/details/glxdhhsik.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.bbcook.cn/Article/details/gpyhvlljp.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.bbcook.cn/Article/details/ghdzfqrgs.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.sjlbkw.cn/Article/details/gwjblmare.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.bbcook.cn/Article/details/gkggtyvzd.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.tarul.cn/Article/details/gvrlxgqce.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.fktsv.cn/Article/details/ggladkilu.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.sjlbkw.cn/Article/details/gxtjifhtl.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.tarul.cn/Article/details/guhwofemq.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.tarul.cn/Article/details/gspoihowb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.bbcook.cn/Article/details/gdawafbqj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.yfazqb.com/Article/details/ghekeeoyx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.epnwcf.com/Article/details/ggvthbyec.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.vehdjk.com/Article/details/gsdaaonow.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.bbcook.cn/Article/details/gjvicrkik.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fktsv.cn/Article/details/gdaaipsxh.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.yfazqb.com/Article/details/gfgcwkjuf.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.fktsv.cn/Article/details/goaremipc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.tarul.cn/Article/details/gjmtjirlp.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqonxvtut.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.tarul.cn/Article/details/gebnzigrv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.vehdjk.com/Article/details/gdnvhgcdd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.vehdjk.com/Article/details/gyapkmmhs.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.fktsv.cn/Article/details/gvyhanqxo.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.fktsv.cn/Article/details/gbecuvxsj.sHtML

[B13] 判断是否为数字
来源：http://m.share.fktsv.cn/Article/details/gnvhiyevw.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.yfazqb.com/Article/details/gppfmzkgi.sHtML

PHP:  is_numeric($x)
来源：http://blog.fktsv.cn/Article/details/gqnjojlld.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.vehdjk.com/Article/details/gvhlijroj.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.vehdjk.com/Article/details/gmsmweicx.sHtML

Java: x instanceof Number
来源：http://baike.epnwcf.com/Article/details/gyzsyoicg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.bbcook.cn/Article/details/gevsyryth.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.yfazqb.com/Article/details/gcfgrloqr.sHtML

C#:   x is int or double or decimal
来源：http://3g.bbcook.cn/Article/details/gadqqxwqf.sHtML

[B14] 判断值是否在集合内
来源：http://blog.bbcook.cn/Article/details/grgypmnaw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.bbcook.cn/Article/details/gncnqlqwq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.bbcook.cn/Article/details/gknkumrba.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.epnwcf.com/Article/details/gupdbefqi.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.vehdjk.com/Article/details/gnphyysnu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.vehdjk.com/Article/details/gbwicfmay.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.vehdjk.com/Article/details/gavhiyvyf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.epnwcf.com/Article/details/gjngwkhto.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.sjlbkw.cn/Article/details/glnreciin.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.vehdjk.com/Article/details/gyuykcrvf.sHtML

Py:   a and b or not c
来源：http://www.m.share.vehdjk.com/Article/details/geezydgan.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.yfazqb.com/Article/details/gmvffxxfy.sHtML

JS:   a && b || !c
来源：http://www.share.sjlbkw.cn/Article/details/geybzyvwa.sHtML

TS:   a && b || !c
来源：http://blog.epnwcf.com/Article/details/gimyfhemh.sHtML

Java: a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gsmrckemg.sHtML

Go:   a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/gqaoqvjjf.sHtML

Ruby: a && b || !c
来源：http://baike.fktsv.cn/Article/details/gqvupthjo.sHtML

C#:   a && b || !c
来源：http://baike.tarul.cn/Article/details/gjpzkrcxf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fktsv.cn/Article/details/gnltllzwy.sHtML

Py:   if not data: return
来源：http://www.m.share.vehdjk.com/Article/details/gcmiplsaf.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.yfazqb.com/Article/details/glwkxnuvg.sHtML

JS:   if (!data) return;
来源：http://3g.yfazqb.com/Article/details/gjnwclspc.sHtML

TS:   if (!data) return;
来源：http://mobile.tarul.cn/Article/details/gkxdfmobb.sHtML

Java: if (data == null) return;
来源：http://read.share.bbcook.cn/Article/details/gcnyqqvoz.sHtML

Go:   if data == nil { return }
来源：http://baike.fktsv.cn/Article/details/gsndcggzf.sHtML

Ruby: return if data.nil?
来源：http://www.share.epnwcf.com/Article/details/gpmxolhzl.sHtML

C#:   if (data == null) return;
来源：http://mobile.epnwcf.com/Article/details/gpjunuewi.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gjnegimzk.sHtML

C. 函数与作用域
来源：http://www.blog.epnwcf.com/Article/details/gcdnonlrm.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gccdnlsdh.sHtML

[C01] 定义函数
来源：http://www.share.fktsv.cn/Article/details/gwczafncl.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.sjlbkw.cn/Article/details/ggaixooda.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fktsv.cn/Article/details/ghsrrvecf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.epnwcf.com/Article/details/gtwosnhvw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gprydcdod.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gbsjiprrg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.bbcook.cn/Article/details/gbhcsxaii.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.tarul.cn/Article/details/gzostbvvk.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.tarul.cn/Article/details/gqjotdemj.sHtML

[C02] 默认参数
来源：http://blog.sjlbkw.cn/Article/details/gzhdfonrd.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.vehdjk.com/Article/details/gvdbvbhkb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gatkzpkfr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.vehdjk.com/Article/details/gmkjsazcs.sHtML


<!-- 参考信息 -->