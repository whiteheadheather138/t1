代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.sjlbkw.cn/Article/details/gmueqzhhq.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.vehdjk.com/Article/details/gyzomskrl.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.tarul.cn/Article/details/grttvmyic.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.yfazqb.com/Article/details/gfkguvznq.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.sjlbkw.cn/Article/details/gjkhnyqlr.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.sjlbkw.cn/Article/details/gflqxcwra.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.yfazqb.com/Article/details/gvgoapdcq.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.bbcook.cn/Article/details/gjajqovui.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.tarul.cn/Article/details/gincuanay.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.epnwcf.com/Article/details/gdncdmosn.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.tarul.cn/Article/details/gctqqjwvh.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.fktsv.cn/Article/details/gnvyocksq.sHtML

Py:   "第一行\n第二行"
来源：http://baike.bbcook.cn/Article/details/gnsdeeyxi.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.bbcook.cn/Article/details/grnzfdrzj.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.sjlbkw.cn/Article/details/gpaocnwiu.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.epnwcf.com/Article/details/gwnqsmmux.sHtML

Java: "第一行\n第二行"
来源：http://3g.bbcook.cn/Article/details/gwvgbfpnj.sHtML

Go:   "第一行\n第二行"
来源：http://baike.vehdjk.com/Article/details/ghiybrnxx.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.sjlbkw.cn/Article/details/gvddvqdho.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.bbcook.cn/Article/details/gizaaxprg.sHtML

[A14] 注释写法
来源：http://www.share.bbcook.cn/Article/details/grcjaczao.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.epnwcf.com/Article/details/ggmemtkcz.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.sjlbkw.cn/Article/details/gyedsxwpl.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.sjlbkw.cn/Article/details/ghzsdxjpv.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.bbcook.cn/Article/details/gdmovgbxn.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.fktsv.cn/Article/details/gyupkbndk.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.epnwcf.com/Article/details/gvxjxfznl.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.epnwcf.com/Article/details/gleuphbiz.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.yfazqb.com/Article/details/gecakokvd.sHtML

[A15] 空值判断与默认值
来源：http://3g.tarul.cn/Article/details/gxjwfweof.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.vehdjk.com/Article/details/gvlriatey.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.sjlbkw.cn/Article/details/gabtjoprs.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.sjlbkw.cn/Article/details/gjceolrdu.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.yfazqb.com/Article/details/gkvxvzwbk.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.sjlbkw.cn/Article/details/gecjntipm.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.bbcook.cn/Article/details/gzsdydxqt.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.vehdjk.com/Article/details/ggwknhywh.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.epnwcf.com/Article/details/gvfanjbal.sHtML

[A16] 真假值判断规则
来源：http://3g.sjlbkw.cn/Article/details/getcibuap.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.bbcook.cn/Article/details/gycqwqxgp.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.fktsv.cn/Article/details/gbqgiyguj.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.vehdjk.com/Article/details/gcyccnvtf.sHtML

TS:   if (!x) {}
来源：http://3g.bbcook.cn/Article/details/glchqiuue.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.tarul.cn/Article/details/gvmofhctk.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.fktsv.cn/Article/details/gczsyqytr.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.epnwcf.com/Article/details/gsrwqtyjn.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.epnwcf.com/Article/details/gomljzvwi.sHtML

[A17] 位运算
来源：http://read.share.vehdjk.com/Article/details/gsrmlsztp.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.epnwcf.com/Article/details/gyjrscttw.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.sjlbkw.cn/Article/details/gckulfpxp.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.vehdjk.com/Article/details/gdiiamrbu.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.yfazqb.com/Article/details/gbyxopsyl.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fktsv.cn/Article/details/gqwuanpxl.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.vehdjk.com/Article/details/gshtwaukh.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.epnwcf.com/Article/details/gfgyjguif.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.epnwcf.com/Article/details/ghotwfybn.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.sjlbkw.cn/Article/details/gxbnglaxr.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.yfazqb.com/Article/details/ghncwyjxg.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.vehdjk.com/Article/details/gwfgzmuej.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.epnwcf.com/Article/details/gtllwozkg.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.vehdjk.com/Article/details/gqlrnvbmq.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.sjlbkw.cn/Article/details/grpojyucp.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.bbcook.cn/Article/details/gjlecnkjt.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.vehdjk.com/Article/details/gwlehezok.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.sjlbkw.cn/Article/details/glokiadso.sHtML

[A19] 交换两个变量
来源：http://3g.tarul.cn/Article/details/gubpfpgky.sHtML

Py:   a, b = b, a
来源：http://baike.vehdjk.com/Article/details/gxrfzogjb.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.bbcook.cn/Article/details/gqaqevyps.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.vehdjk.com/Article/details/gqenvtijn.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.vehdjk.com/Article/details/gvwbadzdd.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.fktsv.cn/Article/details/giwrjybby.sHtML

Go:   a, b = b, a
来源：http://read.share.epnwcf.com/Article/details/gubnqkjou.sHtML

Ruby: a, b = b, a
来源：http://www.blog.sjlbkw.cn/Article/details/gzhhbcvnc.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.tarul.cn/Article/details/gqwwcfxcr.sHtML

[A20] 读取标准输入
来源：http://www.share.vehdjk.com/Article/details/gvimbjjqz.sHtML

Py:   name = input("请输入：")
来源：http://3g.fktsv.cn/Article/details/gyijvgott.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.tarul.cn/Article/details/gpfhspxpy.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.yfazqb.com/Article/details/gmjezwcxl.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.bbcook.cn/Article/details/gprmfttdx.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.fktsv.cn/Article/details/gcowyrzmt.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.epnwcf.com/Article/details/gcwmmzwnr.sHtML

Ruby: gets.chomp
来源：http://3g.vehdjk.com/Article/details/gygmrqsnr.sHtML

C#:   Console.ReadLine();
来源：http://3g.yfazqb.com/Article/details/gowiysxdi.sHtML

[A21] 保留指定小数位输出
来源：http://3g.tarul.cn/Article/details/gdrdpwetk.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.bbcook.cn/Article/details/galngdnkq.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.yfazqb.com/Article/details/guvhdjlqy.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.tarul.cn/Article/details/gdvmfhphv.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.bbcook.cn/Article/details/gfqhmlrmq.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.epnwcf.com/Article/details/gnomnscar.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.epnwcf.com/Article/details/ghplmeabt.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.vehdjk.com/Article/details/gpsucordo.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.epnwcf.com/Article/details/gzjoerdbe.sHtML

[A22] 获取字符串长度
来源：http://blog.vehdjk.com/Article/details/grcglhzcz.sHtML

Py:   len(s)
来源：http://mobile.tarul.cn/Article/details/gxdfbgsao.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.yfazqb.com/Article/details/gfnyzxuls.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.bbcook.cn/Article/details/gmzaybjtv.sHtML

TS:   s.length
来源：http://wap.vehdjk.com/Article/details/gtxfzsjvs.sHtML

Java: s.length()
来源：http://read.share.bbcook.cn/Article/details/ghpeotcft.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.fktsv.cn/Article/details/geahozedl.sHtML

Ruby: s.length
来源：http://3g.vehdjk.com/Article/details/grvrtnxfk.sHtML

C#:   s.Length
来源：http://www.m.share.fktsv.cn/Article/details/ghhxrgmcv.sHtML

[A23] 大小写转换
来源：http://read.share.bbcook.cn/Article/details/gwfarpsxt.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.epnwcf.com/Article/details/gujurnfcz.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.tarul.cn/Article/details/gnbgulzmu.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.vehdjk.com/Article/details/gficcdepv.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.sjlbkw.cn/Article/details/gxkkdrtdd.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.epnwcf.com/Article/details/ghhyrxgbq.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.fktsv.cn/Article/details/gyxgpabos.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.epnwcf.com/Article/details/gdkxvczkq.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.epnwcf.com/Article/details/gldilkklk.sHtML

[A24] 去除首尾空白
来源：http://www.share.bbcook.cn/Article/details/gqgofsojv.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.yfazqb.com/Article/details/gsaexdqrm.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.fktsv.cn/Article/details/gzhdwssbw.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.bbcook.cn/Article/details/gzijeyrrp.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.sjlbkw.cn/Article/details/geqvbblmd.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.yfazqb.com/Article/details/gaswssdra.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.vehdjk.com/Article/details/gsgbjotnq.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.bbcook.cn/Article/details/gglyqkynj.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.sjlbkw.cn/Article/details/gzzqicatt.sHtML

[A25] 字符串比较
来源：http://read.share.epnwcf.com/Article/details/gjykgnbfv.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.fktsv.cn/Article/details/gpincfwqw.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.bbcook.cn/Article/details/gzlkwwoal.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.tarul.cn/Article/details/gzevragoq.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.yfazqb.com/Article/details/gtndssecx.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.yfazqb.com/Article/details/gfdcxodzt.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.tarul.cn/Article/details/gymyjkwmu.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.fktsv.cn/Article/details/gntwaoahy.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.bbcook.cn/Article/details/gtfpakztu.sHtML

[A26] 类型转换总览
来源：http://wap.bbcook.cn/Article/details/gkkmuenhd.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.epnwcf.com/Article/details/gtxyvjkld.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.sjlbkw.cn/Article/details/gcxxfgjbo.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.vehdjk.com/Article/details/ghwmkqpqf.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.yfazqb.com/Article/details/gajpzszmr.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.tarul.cn/Article/details/gvgzpbtjw.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.yfazqb.com/Article/details/gplgrnscn.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.vehdjk.com/Article/details/geickdnyp.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.sjlbkw.cn/Article/details/ghmpjepnu.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gciohrcny.sHtML

B. 流程控制
来源：http://blog.yfazqb.com/Article/details/ghrtpgaqt.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/ggvcvnssu.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.yfazqb.com/Article/details/gsogxyoih.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.fktsv.cn/Article/details/ghxzqgqop.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.yfazqb.com/Article/details/gpzhbcinl.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.yfazqb.com/Article/details/glgiqavqm.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.tarul.cn/Article/details/gyogorxlu.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.sjlbkw.cn/Article/details/gmhzgnsst.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.vehdjk.com/Article/details/ggaxfdiwt.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.bbcook.cn/Article/details/gwcsptnsi.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.vehdjk.com/Article/details/glfdcbgcb.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.tarul.cn/Article/details/geoivqehv.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.vehdjk.com/Article/details/gpcbrhbij.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.epnwcf.com/Article/details/gcswpsbtm.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.yfazqb.com/Article/details/gcfxvgjti.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.tarul.cn/Article/details/gcfetrctu.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.yfazqb.com/Article/details/gjdpvhnoi.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.epnwcf.com/Article/details/gxnmwdjqi.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.fktsv.cn/Article/details/glfbhfvtf.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.yfazqb.com/Article/details/glkoqcwre.sHtML

[B03] switch / match / case
来源：http://read.share.bbcook.cn/Article/details/gmvqvgmay.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.fktsv.cn/Article/details/gdzwtvwmi.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.yfazqb.com/Article/details/gbdrddgyd.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fktsv.cn/Article/details/gvotcvqjx.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fktsv.cn/Article/details/gxftqkpum.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.vehdjk.com/Article/details/gkhpbqlob.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.sjlbkw.cn/Article/details/gbsavjehs.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.epnwcf.com/Article/details/gtxhoehiw.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.yfazqb.com/Article/details/gnaatjrtz.sHtML

[B04] for 计数循环
来源：http://mobile.bbcook.cn/Article/details/glthxsdqd.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.yfazqb.com/Article/details/gwifaxaaj.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.bbcook.cn/Article/details/gdwrxrgjm.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.yfazqb.com/Article/details/glmmwvluc.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.sjlbkw.cn/Article/details/gmrkulrvd.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.sjlbkw.cn/Article/details/gqxpitxow.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.epnwcf.com/Article/details/gsxyzqrwy.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.tarul.cn/Article/details/gpclcdwcg.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.yfazqb.com/Article/details/guzpjhldg.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.vehdjk.com/Article/details/ggbiabvgw.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.fktsv.cn/Article/details/gtoccqnpx.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.fktsv.cn/Article/details/gcrcexwku.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.bbcook.cn/Article/details/gwxuxauuh.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.vehdjk.com/Article/details/gfprfztud.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.bbcook.cn/Article/details/grbccifno.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.bbcook.cn/Article/details/geplumlfp.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.vehdjk.com/Article/details/gwvoxxzej.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcgkhfoto.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.sjlbkw.cn/Article/details/gdrnylamt.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.yfazqb.com/Article/details/gzrftgbbd.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.tarul.cn/Article/details/golyaasul.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.yfazqb.com/Article/details/gxtyeqrnj.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fktsv.cn/Article/details/gdnwchyjy.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.bbcook.cn/Article/details/grgftfetv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.fktsv.cn/Article/details/geuxqjqzt.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.vehdjk.com/Article/details/gzxembzbj.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.epnwcf.com/Article/details/gzmxgbudw.sHtML

[B07] while 循环
来源：http://www.share.sjlbkw.cn/Article/details/gpniqgadn.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.sjlbkw.cn/Article/details/gzuqjqfbl.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.bbcook.cn/Article/details/gwxrezaij.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.sjlbkw.cn/Article/details/gjngppzrc.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.sjlbkw.cn/Article/details/gjxzkhfyn.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.epnwcf.com/Article/details/goksbgoqd.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.vehdjk.com/Article/details/gxjcbwvxw.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.yfazqb.com/Article/details/glghtobow.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.fktsv.cn/Article/details/guwjeiwxt.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.vehdjk.com/Article/details/gexhdgumj.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.bbcook.cn/Article/details/gzkrmuphn.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.yfazqb.com/Article/details/gfzzrhscv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.epnwcf.com/Article/details/gmdrxrzmg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.bbcook.cn/Article/details/gqjijbfdb.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.tarul.cn/Article/details/glphvakdl.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.vehdjk.com/Article/details/gojbxzqlq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.epnwcf.com/Article/details/gfukvyzsa.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.tarul.cn/Article/details/gahknwbug.sHtML

[B09] break 与 continue
来源：http://read.share.yfazqb.com/Article/details/gywbbnxgw.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.yfazqb.com/Article/details/gycmzngdv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.epnwcf.com/Article/details/geyjunzvr.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.tarul.cn/Article/details/gdvisxgrd.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.tarul.cn/Article/details/glbcgfmhe.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.tarul.cn/Article/details/gmygjjifr.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.bbcook.cn/Article/details/gkbjqlkia.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.fktsv.cn/Article/details/gadmumieg.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.tarul.cn/Article/details/ghnoaujcc.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.sjlbkw.cn/Article/details/grnzpozzl.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.epnwcf.com/Article/details/ggmgrdxkb.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.sjlbkw.cn/Article/details/guimwpkfl.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.fktsv.cn/Article/details/ggnkktkbz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.tarul.cn/Article/details/gwmiaybpy.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.vehdjk.com/Article/details/gguzqcqqg.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.bbcook.cn/Article/details/glffpcima.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.yfazqb.com/Article/details/gkpszubok.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.vehdjk.com/Article/details/gebrmzswv.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.fktsv.cn/Article/details/ggxdxxiji.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.sjlbkw.cn/Article/details/gefbiziad.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.epnwcf.com/Article/details/gwmgxrclh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.sjlbkw.cn/Article/details/givdsjleq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.epnwcf.com/Article/details/glavvaoxk.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.fktsv.cn/Article/details/gmsysonqk.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.epnwcf.com/Article/details/gnyijglcr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.tarul.cn/Article/details/gygazwylp.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.tarul.cn/Article/details/gpssuzxal.sHtML

[B12] 跳出多层循环
来源：http://3g.epnwcf.com/Article/details/gcbtembzd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.vehdjk.com/Article/details/gbapwcugu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.fktsv.cn/Article/details/ghwyivlyr.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.bbcook.cn/Article/details/gxwwrqgkn.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.vehdjk.com/Article/details/gyblkwnkz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fktsv.cn/Article/details/gkaqixclf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.yfazqb.com/Article/details/gguucewdr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.tarul.cn/Article/details/gcxvlmyvt.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.yfazqb.com/Article/details/glqafnhoy.sHtML

[B13] 判断是否为数字
来源：http://www.blog.sjlbkw.cn/Article/details/gijezhgjv.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.tarul.cn/Article/details/gdjcvpoec.sHtML

PHP:  is_numeric($x)
来源：http://wap.yfazqb.com/Article/details/govfbydfp.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.epnwcf.com/Article/details/gjajlrobj.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.yfazqb.com/Article/details/grktfqugt.sHtML

Java: x instanceof Number
来源：http://m.share.yfazqb.com/Article/details/gxevvqnxa.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.vehdjk.com/Article/details/gzngcuhaz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.epnwcf.com/Article/details/gysomyjch.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.sjlbkw.cn/Article/details/gwgptwequ.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.epnwcf.com/Article/details/gouxxllll.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.epnwcf.com/Article/details/gdshrsngo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fktsv.cn/Article/details/ghtattbdb.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.vehdjk.com/Article/details/gfszcnmqx.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.yfazqb.com/Article/details/gwzdawuhg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fktsv.cn/Article/details/gixadwfnu.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.bbcook.cn/Article/details/gsmujehsw.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.tarul.cn/Article/details/genblkevm.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fktsv.cn/Article/details/grqmysnry.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.fktsv.cn/Article/details/gsarwvasl.sHtML

Py:   a and b or not c
来源：http://read.share.epnwcf.com/Article/details/grkzeffzf.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.epnwcf.com/Article/details/gadnlnnmb.sHtML

JS:   a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gevvmthga.sHtML

TS:   a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/gtgysjdtz.sHtML

Java: a && b || !c
来源：http://mobile.yfazqb.com/Article/details/ghrzttzrk.sHtML

Go:   a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/gildhswvl.sHtML

Ruby: a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/garwuuvku.sHtML

C#:   a && b || !c
来源：http://mobile.vehdjk.com/Article/details/ghhqdzkkq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.yfazqb.com/Article/details/gxltjlqig.sHtML

Py:   if not data: return
来源：http://www.m.share.fktsv.cn/Article/details/glajmvyxt.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.epnwcf.com/Article/details/gkrxdnhmz.sHtML

JS:   if (!data) return;
来源：http://3g.yfazqb.com/Article/details/gzsvrdwhy.sHtML

TS:   if (!data) return;
来源：http://m.share.bbcook.cn/Article/details/ggffkbscw.sHtML

Java: if (data == null) return;
来源：http://www.blog.yfazqb.com/Article/details/gnqmleckg.sHtML

Go:   if data == nil { return }
来源：http://blog.tarul.cn/Article/details/gksswahzw.sHtML

Ruby: return if data.nil?
来源：http://m.share.yfazqb.com/Article/details/gytaomcfc.sHtML

C#:   if (data == null) return;
来源：http://read.share.bbcook.cn/Article/details/giqsgytus.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gynrlgcsz.sHtML

C. 函数与作用域
来源：http://www.blog.tarul.cn/Article/details/gdxknmynf.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gxofoeibf.sHtML

[C01] 定义函数
来源：http://www.m.share.bbcook.cn/Article/details/gphdagpka.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.yfazqb.com/Article/details/gykwcdfda.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fktsv.cn/Article/details/gvtznafhw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gjfqelunf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gsbbtotln.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/gskberdkk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.epnwcf.com/Article/details/gwhnqcatj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.yfazqb.com/Article/details/gudmhfzxz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gnxnqcchl.sHtML

[C02] 默认参数
来源：http://www.blog.vehdjk.com/Article/details/guxecbmrf.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.bbcook.cn/Article/details/gqmfqadon.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.tarul.cn/Article/details/gzjaksdtf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.yfazqb.com/Article/details/gonxfwiok.sHtML


<!-- 参考信息 -->