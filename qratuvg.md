代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.tarul.cn/Article/details/gvkbhhskr.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.vehdjk.com/Article/details/gqrjmhlcj.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.sjlbkw.cn/Article/details/ggkpewntm.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.tarul.cn/Article/details/gmrjjbntb.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.sjlbkw.cn/Article/details/gmepxbmra.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.vehdjk.com/Article/details/gxqiberud.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.vehdjk.com/Article/details/gdqyicurl.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.bbcook.cn/Article/details/glhezwidu.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.sjlbkw.cn/Article/details/gpvjlytdf.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.tarul.cn/Article/details/gjssvaeya.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.tarul.cn/Article/details/gogadvbqr.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.sjlbkw.cn/Article/details/gkxgukpvn.sHtML

C#:   (int)'A'; (char)65
来源：http://www.m.share.yfazqb.com/Article/details/gexvplwrj.sHtML

[A19] 交换两个变量
来源：http://blog.epnwcf.com/Article/details/gfuxdpegq.sHtML

Py:   a, b = b, a
来源：http://blog.vehdjk.com/Article/details/gynlyzglh.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.yfazqb.com/Article/details/gfuqxdqtf.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.vehdjk.com/Article/details/gqkipjdxx.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.fktsv.cn/Article/details/gkqybihqg.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.fktsv.cn/Article/details/gshcsixpm.sHtML

Go:   a, b = b, a
来源：http://blog.fktsv.cn/Article/details/gfyfpeyif.sHtML

Ruby: a, b = b, a
来源：http://3g.yfazqb.com/Article/details/gfuawcxrp.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.fktsv.cn/Article/details/gyuzqcrns.sHtML

[A20] 读取标准输入
来源：http://read.share.epnwcf.com/Article/details/gasjlnitr.sHtML

Py:   name = input("请输入：")
来源：http://www.share.vehdjk.com/Article/details/gfncrtbwz.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.vehdjk.com/Article/details/gzgitooxq.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.vehdjk.com/Article/details/gplrfxlgt.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.epnwcf.com/Article/details/gtuutbswi.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.fktsv.cn/Article/details/gjkaqujzh.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.sjlbkw.cn/Article/details/guzdjdhjl.sHtML

Ruby: gets.chomp
来源：http://3g.yfazqb.com/Article/details/ggnkphtab.sHtML

C#:   Console.ReadLine();
来源：http://www.share.fktsv.cn/Article/details/gfwzhceso.sHtML

[A21] 保留指定小数位输出
来源：http://blog.yfazqb.com/Article/details/gkwzmirmv.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.bbcook.cn/Article/details/gdkbrywjd.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.tarul.cn/Article/details/grnblbdbl.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.vehdjk.com/Article/details/gdymzayvq.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.epnwcf.com/Article/details/gjhosgfzj.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.tarul.cn/Article/details/grtemldce.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.yfazqb.com/Article/details/ggohghkcz.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.vehdjk.com/Article/details/ghelkwbbn.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.bbcook.cn/Article/details/glcpsjdet.sHtML

[A22] 获取字符串长度
来源：http://wap.epnwcf.com/Article/details/gfoysqsev.sHtML

Py:   len(s)
来源：http://read.share.sjlbkw.cn/Article/details/gjuvljfij.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.epnwcf.com/Article/details/gjuwcbklk.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.sjlbkw.cn/Article/details/gwleokucc.sHtML

TS:   s.length
来源：http://mobile.bbcook.cn/Article/details/gxeivfovv.sHtML

Java: s.length()
来源：http://m.share.yfazqb.com/Article/details/ggagvbfid.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.sjlbkw.cn/Article/details/goldelizk.sHtML

Ruby: s.length
来源：http://www.m.share.yfazqb.com/Article/details/gcmtuzxvm.sHtML

C#:   s.Length
来源：http://wap.tarul.cn/Article/details/gtsunckqp.sHtML

[A23] 大小写转换
来源：http://www.m.share.bbcook.cn/Article/details/gzcizdgvb.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.epnwcf.com/Article/details/gxookanze.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.tarul.cn/Article/details/gqgksmwbf.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.sjlbkw.cn/Article/details/gkrplzaaq.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.yfazqb.com/Article/details/gpquawtqv.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.yfazqb.com/Article/details/glhpjbbar.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.tarul.cn/Article/details/ghbersjli.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.epnwcf.com/Article/details/gszcejcqf.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.bbcook.cn/Article/details/grwxmqpcd.sHtML

[A24] 去除首尾空白
来源：http://mobile.tarul.cn/Article/details/gnsfvpfic.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.bbcook.cn/Article/details/gzdevdxkt.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.fktsv.cn/Article/details/gpujpfgiz.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.vehdjk.com/Article/details/grlaqmaal.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.yfazqb.com/Article/details/gfgvcuslx.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.fktsv.cn/Article/details/gmgpaetjd.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.yfazqb.com/Article/details/gngjfmzke.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.sjlbkw.cn/Article/details/gctpbysah.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.fktsv.cn/Article/details/gtuhiktab.sHtML

[A25] 字符串比较
来源：http://3g.tarul.cn/Article/details/gwudjjwlp.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.vehdjk.com/Article/details/gpihxzsha.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.tarul.cn/Article/details/gilwfjxwp.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.yfazqb.com/Article/details/gshhzpzxh.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fktsv.cn/Article/details/gvjfqjpfe.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.vehdjk.com/Article/details/gweitskpc.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.fktsv.cn/Article/details/gzcsdxtte.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.sjlbkw.cn/Article/details/gclhistrf.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.epnwcf.com/Article/details/guxbehtwb.sHtML

[A26] 类型转换总览
来源：http://read.share.tarul.cn/Article/details/gigaunibd.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.tarul.cn/Article/details/gprbyxoqk.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.tarul.cn/Article/details/gojrtvzna.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.sjlbkw.cn/Article/details/ghpkwykbr.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.bbcook.cn/Article/details/giifwqean.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.epnwcf.com/Article/details/gwdeezpcx.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.tarul.cn/Article/details/gpfavapng.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.yfazqb.com/Article/details/gpzeuamah.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.vehdjk.com/Article/details/gjfzszkof.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gaoncural.sHtML

B. 流程控制
来源：http://baike.tarul.cn/Article/details/gywcuxymg.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gkmklnsep.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.fktsv.cn/Article/details/gowxqnfzj.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.tarul.cn/Article/details/gllvzwwmy.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.sjlbkw.cn/Article/details/gknfhazep.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.sjlbkw.cn/Article/details/gbtuybzmk.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.sjlbkw.cn/Article/details/giwtnvqxl.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.bbcook.cn/Article/details/gmxgntzbw.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.vehdjk.com/Article/details/gwndnauoh.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.yfazqb.com/Article/details/gfbxviadz.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.sjlbkw.cn/Article/details/gyktqurer.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.fktsv.cn/Article/details/gikunbwrh.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.fktsv.cn/Article/details/gevsjskjc.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.fktsv.cn/Article/details/gmajhwwig.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.sjlbkw.cn/Article/details/ggidhwzuc.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.sjlbkw.cn/Article/details/gldswweug.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fktsv.cn/Article/details/gcllcnjkx.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.yfazqb.com/Article/details/gwuzzrrdf.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.epnwcf.com/Article/details/ggxohicgv.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.yfazqb.com/Article/details/gydiesglo.sHtML

[B03] switch / match / case
来源：http://wap.tarul.cn/Article/details/gktguzara.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.bbcook.cn/Article/details/gzxmvblnu.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.tarul.cn/Article/details/gvjtrhfjm.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.bbcook.cn/Article/details/gafgrbqzj.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.yfazqb.com/Article/details/gndiatthr.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.sjlbkw.cn/Article/details/geiytttvb.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.vehdjk.com/Article/details/gbepnlmrw.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.epnwcf.com/Article/details/ggnpylagf.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.sjlbkw.cn/Article/details/gfhwpnkpd.sHtML

[B04] for 计数循环
来源：http://mobile.epnwcf.com/Article/details/gtyllyjib.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.fktsv.cn/Article/details/gjzuoaubj.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.vehdjk.com/Article/details/grgvgedtk.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.vehdjk.com/Article/details/grcwipuof.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fktsv.cn/Article/details/gcoabjfze.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.yfazqb.com/Article/details/grprprqea.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.yfazqb.com/Article/details/gfpbhlazn.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.epnwcf.com/Article/details/gegltgyjc.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.tarul.cn/Article/details/gtevnyvqe.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.fktsv.cn/Article/details/gbtpdrark.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.sjlbkw.cn/Article/details/gmarubvnu.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.yfazqb.com/Article/details/gbqkcigsu.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.epnwcf.com/Article/details/gqzlsyztw.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fktsv.cn/Article/details/gbsjgpbve.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.epnwcf.com/Article/details/gatqwswgt.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.sjlbkw.cn/Article/details/glufoezdp.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.epnwcf.com/Article/details/grhscvvgc.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.yfazqb.com/Article/details/gwiuvehqm.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.epnwcf.com/Article/details/gtrzngsmt.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.tarul.cn/Article/details/gpcryptpt.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.bbcook.cn/Article/details/giivowmcb.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.epnwcf.com/Article/details/gmfpvuzlq.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.vehdjk.com/Article/details/gmgdjanvp.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.fktsv.cn/Article/details/gvptdduag.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.bbcook.cn/Article/details/gafbucpfx.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.fktsv.cn/Article/details/golvixxwq.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.yfazqb.com/Article/details/gwbrioqbw.sHtML

[B07] while 循环
来源：http://www.share.sjlbkw.cn/Article/details/gqgcrqcnl.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.sjlbkw.cn/Article/details/gujpljceh.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.fktsv.cn/Article/details/gtqprgajb.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.bbcook.cn/Article/details/ggkonphou.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.fktsv.cn/Article/details/gmgmvjckw.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.sjlbkw.cn/Article/details/gvyhssivn.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.bbcook.cn/Article/details/ggafbldzz.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.yfazqb.com/Article/details/gpnhhiyml.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.bbcook.cn/Article/details/givbnplpk.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.sjlbkw.cn/Article/details/gzpdmpswi.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.sjlbkw.cn/Article/details/gfbpubvti.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.epnwcf.com/Article/details/ggwiirrtu.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.vehdjk.com/Article/details/gsblukqch.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.vehdjk.com/Article/details/ghjmtbtwu.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.tarul.cn/Article/details/gfbgxswxl.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.bbcook.cn/Article/details/gtxfiitzg.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.fktsv.cn/Article/details/gukgxmort.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjymqnxcd.sHtML

[B09] break 与 continue
来源：http://blog.yfazqb.com/Article/details/gzirigryr.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.yfazqb.com/Article/details/gmyhfjnxp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.yfazqb.com/Article/details/gtammkpxm.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.sjlbkw.cn/Article/details/gyqtonlug.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghkrhqfmb.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.tarul.cn/Article/details/gqrinkkdg.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fktsv.cn/Article/details/gdmtmjnrg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.tarul.cn/Article/details/gezvlwktt.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.epnwcf.com/Article/details/gsmfnntoe.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.bbcook.cn/Article/details/gajdmidkl.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.yfazqb.com/Article/details/gpvvytijq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.tarul.cn/Article/details/gxasbqtkm.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.yfazqb.com/Article/details/gjbksxpqd.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.fktsv.cn/Article/details/goacguict.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.fktsv.cn/Article/details/gliswxndk.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.fktsv.cn/Article/details/gnjaapnul.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.yfazqb.com/Article/details/grigrsefw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.vehdjk.com/Article/details/gvxnevjwn.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.yfazqb.com/Article/details/gkijuxetj.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.sjlbkw.cn/Article/details/gapsqjxmh.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.bbcook.cn/Article/details/gbaqfcfsl.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.bbcook.cn/Article/details/gjkxsfxjw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.vehdjk.com/Article/details/gjgklbkms.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.yfazqb.com/Article/details/gmnuxclvb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.epnwcf.com/Article/details/gvpdnduoz.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.epnwcf.com/Article/details/gjwhmwfom.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.bbcook.cn/Article/details/gafxzxuka.sHtML

[B12] 跳出多层循环
来源：http://3g.epnwcf.com/Article/details/gtygdomcy.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.epnwcf.com/Article/details/getklsugm.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.sjlbkw.cn/Article/details/gtftkhwas.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fktsv.cn/Article/details/ggvhmqelb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.tarul.cn/Article/details/gtwmfstzq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.vehdjk.com/Article/details/gmpaeoore.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.yfazqb.com/Article/details/gajggbgnz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fktsv.cn/Article/details/gvwrncvrw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.yfazqb.com/Article/details/gwywxtsqu.sHtML

[B13] 判断是否为数字
来源：http://blog.epnwcf.com/Article/details/ggwxbqbjy.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.tarul.cn/Article/details/gxzgeckfy.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.yfazqb.com/Article/details/gwhjbwgan.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.yfazqb.com/Article/details/gahkkymya.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.yfazqb.com/Article/details/gnuhmaqou.sHtML

Java: x instanceof Number
来源：http://m.share.tarul.cn/Article/details/gyvavieoh.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.epnwcf.com/Article/details/gfhfuosbc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.sjlbkw.cn/Article/details/gklmmrsla.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.epnwcf.com/Article/details/ghkjzjrli.sHtML

[B14] 判断值是否在集合内
来源：http://wap.tarul.cn/Article/details/gndvypszj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.epnwcf.com/Article/details/gykszgtun.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.sjlbkw.cn/Article/details/glqrlpkod.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.tarul.cn/Article/details/gschamfkf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fktsv.cn/Article/details/gluoxrnkk.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.epnwcf.com/Article/details/gudlqjhez.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.yfazqb.com/Article/details/gtefddhyt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fktsv.cn/Article/details/ghpbtzemt.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.epnwcf.com/Article/details/gaovlkkjd.sHtML

[B15] 布尔运算与取反
来源：http://baike.epnwcf.com/Article/details/gejqzmxde.sHtML

Py:   a and b or not c
来源：http://m.share.tarul.cn/Article/details/gpxobdrxz.sHtML

PHP:  $a && $b || !$c
来源：http://baike.tarul.cn/Article/details/gnflllybo.sHtML

JS:   a && b || !c
来源：http://mobile.epnwcf.com/Article/details/guvaabfsh.sHtML

TS:   a && b || !c
来源：http://3g.epnwcf.com/Article/details/gcfeixhkz.sHtML

Java: a && b || !c
来源：http://read.share.epnwcf.com/Article/details/gikrtfezd.sHtML

Go:   a && b || !c
来源：http://baike.tarul.cn/Article/details/gqxcchsbz.sHtML

Ruby: a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gbfxgpsty.sHtML

C#:   a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gbdygshrp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.tarul.cn/Article/details/grcjgubdb.sHtML

Py:   if not data: return
来源：http://m.share.fktsv.cn/Article/details/gcfmgxxhh.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.tarul.cn/Article/details/gtsauxdlv.sHtML

JS:   if (!data) return;
来源：http://mobile.vehdjk.com/Article/details/gnlsiypvm.sHtML

TS:   if (!data) return;
来源：http://baike.fktsv.cn/Article/details/goiymfjfb.sHtML

Java: if (data == null) return;
来源：http://www.share.fktsv.cn/Article/details/godmumtpb.sHtML

Go:   if data == nil { return }
来源：http://wap.sjlbkw.cn/Article/details/gzprocfzi.sHtML

Ruby: return if data.nil?
来源：http://mobile.tarul.cn/Article/details/gssbnhxmc.sHtML

C#:   if (data == null) return;
来源：http://baike.bbcook.cn/Article/details/gqgqaivzx.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gvugwuitk.sHtML

C. 函数与作用域
来源：http://wap.tarul.cn/Article/details/grdchaxfi.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gykjthdek.sHtML

[C01] 定义函数
来源：http://www.blog.vehdjk.com/Article/details/gyusawltj.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.bbcook.cn/Article/details/gzuwitpkp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.yfazqb.com/Article/details/gtzviblhk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/gvlpmiscz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.yfazqb.com/Article/details/gdreeoron.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.tarul.cn/Article/details/gmdmpkmgw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fktsv.cn/Article/details/gnzjmdqhu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.yfazqb.com/Article/details/gjjshwlol.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.yfazqb.com/Article/details/gechltncz.sHtML

[C02] 默认参数
来源：http://mobile.tarul.cn/Article/details/getsupkas.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.yfazqb.com/Article/details/gyyejwobn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.vehdjk.com/Article/details/ghcmwkpqj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.tarul.cn/Article/details/gugeefkfw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.bbcook.cn/Article/details/gydxcyawl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.tarul.cn/Article/details/gqylrrvup.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.vehdjk.com/Article/details/gtgndwors.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.bbcook.cn/Article/details/gnxzptqzy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.sjlbkw.cn/Article/details/gilatofvl.sHtML

[C03] 可变参数
来源：http://3g.tarul.cn/Article/details/gzoappmuz.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.sjlbkw.cn/Article/details/gfbdvktvi.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fktsv.cn/Article/details/gvydizenz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.vehdjk.com/Article/details/gafjozbsd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.bbcook.cn/Article/details/ghozjszhh.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.tarul.cn/Article/details/gdmqnplbq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.vehdjk.com/Article/details/gyzwhdyyv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.tarul.cn/Article/details/giadjkbhk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fktsv.cn/Article/details/glprecbno.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.yfazqb.com/Article/details/gqoxjqsrc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.bbcook.cn/Article/details/gzqtepkna.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.sjlbkw.cn/Article/details/gdichkema.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.sjlbkw.cn/Article/details/gwiovsgnw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.sjlbkw.cn/Article/details/gouhhgmpr.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.tarul.cn/Article/details/ghhxwpkjp.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.bbcook.cn/Article/details/gznbyrugv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fktsv.cn/Article/details/grtslklsu.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.tarul.cn/Article/details/gnzryqbok.sHtML

[C05] 返回多个值
来源：http://www.share.bbcook.cn/Article/details/guhkelwxr.sHtML

Py:   return a, b
来源：http://3g.tarul.cn/Article/details/gzztsyypq.sHtML

PHP:  return [$a, $b];
来源：http://baike.sjlbkw.cn/Article/details/gqbkwpjxz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.sjlbkw.cn/Article/details/gcjdpassm.sHtML

TS:   return { a, b };
来源：http://www.blog.fktsv.cn/Article/details/gfesooefl.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.bbcook.cn/Article/details/gpvjxubdr.sHtML

Go:   return a, b
来源：http://baike.fktsv.cn/Article/details/gebcbxncg.sHtML

Ruby: return a, b
来源：http://wap.bbcook.cn/Article/details/gtttjhqby.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.bbcook.cn/Article/details/gkovoaqaw.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.tarul.cn/Article/details/gtnmqvvqx.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fktsv.cn/Article/details/ghnehsclo.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.yfazqb.com/Article/details/gevwhevri.sHtML

JS:   const square = x => x * x;
来源：http://blog.tarul.cn/Article/details/gurnofpbf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.bbcook.cn/Article/details/gdxizbkdr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.vehdjk.com/Article/details/gyeajdqpz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.vehdjk.com/Article/details/gcxolmabi.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.sjlbkw.cn/Article/details/gpbvdiwre.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.yfazqb.com/Article/details/gddciwerz.sHtML

[C07] 把函数作为参数传入
来源：http://3g.sjlbkw.cn/Article/details/gubrinoyb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.sjlbkw.cn/Article/details/gidvpqmio.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.epnwcf.com/Article/details/grkhyabju.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.tarul.cn/Article/details/gosnhsesh.sHtML

TS:   arr.map(String)
来源：http://mobile.sjlbkw.cn/Article/details/gxymbiolt.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.vehdjk.com/Article/details/gwgbmqyid.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.sjlbkw.cn/Article/details/gjvatgxkx.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fktsv.cn/Article/details/gzgbktlbp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.vehdjk.com/Article/details/gsjkakqbn.sHtML

[C08] 闭包
来源：http://www.m.share.bbcook.cn/Article/details/gagbixenf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.bbcook.cn/Article/details/gxezonvrt.sHtML


<!-- 参考信息 -->