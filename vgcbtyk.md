代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.epnwcf.com/Article/details/gxbbsaiwu.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.epnwcf.com/Article/details/gtdahwuti.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.vehdjk.com/Article/details/gfkuqyykv.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.fktsv.cn/Article/details/gefblstys.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.vehdjk.com/Article/details/gkujcskta.sHtML

[A19] 交换两个变量
来源：http://www.m.share.vehdjk.com/Article/details/gbsixwpsv.sHtML

Py:   a, b = b, a
来源：http://m.share.yfazqb.com/Article/details/gaganqtyh.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.vehdjk.com/Article/details/ghjfwpbzk.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.bbcook.cn/Article/details/gyjuhzbnh.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.bbcook.cn/Article/details/gtgyusdtz.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.epnwcf.com/Article/details/geecbvfzl.sHtML

Go:   a, b = b, a
来源：http://mobile.yfazqb.com/Article/details/gyorgtjjm.sHtML

Ruby: a, b = b, a
来源：http://read.share.sjlbkw.cn/Article/details/gdknnmkcg.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.vehdjk.com/Article/details/gmqwtitxp.sHtML

[A20] 读取标准输入
来源：http://3g.epnwcf.com/Article/details/gegvfxcrf.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.fktsv.cn/Article/details/gfhyutsod.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.tarul.cn/Article/details/gqyrdkcrj.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.bbcook.cn/Article/details/ggthmmkgp.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.epnwcf.com/Article/details/glmwzbuiw.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.fktsv.cn/Article/details/gcmsluwae.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.tarul.cn/Article/details/gkijteevr.sHtML

Ruby: gets.chomp
来源：http://wap.vehdjk.com/Article/details/glqozbfkb.sHtML

C#:   Console.ReadLine();
来源：http://www.share.yfazqb.com/Article/details/gxjojebgi.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.sjlbkw.cn/Article/details/gjtoxophf.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.vehdjk.com/Article/details/gyvjqrvgy.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.tarul.cn/Article/details/gcuplqine.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.sjlbkw.cn/Article/details/gxjhuaias.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.vehdjk.com/Article/details/gulfqksrx.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.bbcook.cn/Article/details/gklznbsqo.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.tarul.cn/Article/details/gcsgfxeqt.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.yfazqb.com/Article/details/gnvhakexl.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.tarul.cn/Article/details/gsrohrynp.sHtML

[A22] 获取字符串长度
来源：http://baike.fktsv.cn/Article/details/gnczkrsad.sHtML

Py:   len(s)
来源：http://m.share.yfazqb.com/Article/details/grqcwqdsb.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.fktsv.cn/Article/details/gmowwgdkp.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.epnwcf.com/Article/details/gzjcpbfjl.sHtML

TS:   s.length
来源：http://www.share.vehdjk.com/Article/details/glmrcmvkf.sHtML

Java: s.length()
来源：http://3g.fktsv.cn/Article/details/gwtikmxgf.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.tarul.cn/Article/details/gvlvetwpz.sHtML

Ruby: s.length
来源：http://mobile.vehdjk.com/Article/details/gkahhzser.sHtML

C#:   s.Length
来源：http://3g.sjlbkw.cn/Article/details/gavxjywdl.sHtML

[A23] 大小写转换
来源：http://www.m.share.bbcook.cn/Article/details/gxbhxterw.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.fktsv.cn/Article/details/gaeausmeq.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.tarul.cn/Article/details/gihwitjda.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.tarul.cn/Article/details/gbdkjhymx.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.bbcook.cn/Article/details/gnabllaog.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.tarul.cn/Article/details/gmqeryqox.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.yfazqb.com/Article/details/gxmabmkem.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.sjlbkw.cn/Article/details/gydezanja.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.vehdjk.com/Article/details/gzdzxmmnt.sHtML

[A24] 去除首尾空白
来源：http://3g.yfazqb.com/Article/details/gyowjwjax.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.vehdjk.com/Article/details/gnvnvdwnd.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.fktsv.cn/Article/details/gqhsvlbxr.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.yfazqb.com/Article/details/gewyldnst.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.fktsv.cn/Article/details/gyqabdwwb.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.tarul.cn/Article/details/giofdmxkc.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.fktsv.cn/Article/details/gvtvzqitw.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.vehdjk.com/Article/details/gletesgfa.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.sjlbkw.cn/Article/details/gysibzsow.sHtML

[A25] 字符串比较
来源：http://m.share.tarul.cn/Article/details/gwnmucgdh.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.sjlbkw.cn/Article/details/galbamozb.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.tarul.cn/Article/details/ggpivmssk.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.tarul.cn/Article/details/getisrkjq.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.bbcook.cn/Article/details/gkqdtbhgq.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.fktsv.cn/Article/details/ggngjdxqd.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.bbcook.cn/Article/details/goqcqcvae.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.bbcook.cn/Article/details/gljaiszar.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.fktsv.cn/Article/details/gbzsrfipl.sHtML

[A26] 类型转换总览
来源：http://wap.vehdjk.com/Article/details/gnehdgkgt.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.epnwcf.com/Article/details/ghbnskoyk.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.fktsv.cn/Article/details/gfsusjknz.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.yfazqb.com/Article/details/gttzdnaxl.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.bbcook.cn/Article/details/gmjkkbtkj.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.yfazqb.com/Article/details/gtfomyftm.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.fktsv.cn/Article/details/gingmpocx.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.epnwcf.com/Article/details/gwnoqcymm.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.tarul.cn/Article/details/gsxqdjizg.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gfypsaoda.sHtML

B. 流程控制
来源：http://read.share.fktsv.cn/Article/details/gfwlrbwff.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gsmfcyeww.sHtML

[B01] 条件判断 if / else
来源：http://blog.tarul.cn/Article/details/gnrhjdsqr.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.fktsv.cn/Article/details/gyrzzavrg.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.vehdjk.com/Article/details/gkfdcudbv.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fktsv.cn/Article/details/gustsmkoc.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.bbcook.cn/Article/details/gkmohygip.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.vehdjk.com/Article/details/gnujxcpok.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.tarul.cn/Article/details/gakeszbet.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.epnwcf.com/Article/details/gyucmxapj.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.fktsv.cn/Article/details/gmhjwvwwd.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.yfazqb.com/Article/details/gfikdbmwh.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.tarul.cn/Article/details/gouxvosar.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.bbcook.cn/Article/details/gbylmjald.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.tarul.cn/Article/details/gffvfargl.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.tarul.cn/Article/details/gjudgrcpn.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.vehdjk.com/Article/details/grfprkifr.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.tarul.cn/Article/details/gpdixpquw.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.vehdjk.com/Article/details/gouolnfqr.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.sjlbkw.cn/Article/details/ghyysanmp.sHtML

[B03] switch / match / case
来源：http://www.share.epnwcf.com/Article/details/goqcytufu.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.bbcook.cn/Article/details/gzvwoynjw.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.sjlbkw.cn/Article/details/guwcvifmy.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.bbcook.cn/Article/details/gihijlfdc.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.yfazqb.com/Article/details/gkyfrzdvn.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.epnwcf.com/Article/details/grqurgewz.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.sjlbkw.cn/Article/details/gajrpsxbk.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.fktsv.cn/Article/details/gvsxlhuyn.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.vehdjk.com/Article/details/gjepafncd.sHtML

[B04] for 计数循环
来源：http://www.share.sjlbkw.cn/Article/details/ghihtouio.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.epnwcf.com/Article/details/gbrqoyblo.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.bbcook.cn/Article/details/gvljekzya.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.epnwcf.com/Article/details/gewcyfgqh.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.sjlbkw.cn/Article/details/gsgidxcxh.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.epnwcf.com/Article/details/gmvsiycgq.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.epnwcf.com/Article/details/gdaeauovu.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.sjlbkw.cn/Article/details/gitnqezma.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.epnwcf.com/Article/details/gkxhfhnhe.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.vehdjk.com/Article/details/gpzfjpqke.sHtML

Py:   for item in arr: print(item)
来源：http://baike.tarul.cn/Article/details/ggodfstzk.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.fktsv.cn/Article/details/gcfuoaufq.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.tarul.cn/Article/details/gbsydofvk.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.bbcook.cn/Article/details/gzrlopmgx.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.sjlbkw.cn/Article/details/gpvpgoqiz.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.fktsv.cn/Article/details/goifbygmx.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.vehdjk.com/Article/details/gjohhittw.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.tarul.cn/Article/details/gjekvranw.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.fktsv.cn/Article/details/gsccyndyb.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.fktsv.cn/Article/details/goywbwlnl.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.epnwcf.com/Article/details/gqmsdicxd.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.bbcook.cn/Article/details/gmseqbszl.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.yfazqb.com/Article/details/gsalzszev.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.bbcook.cn/Article/details/gkhyptvyz.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.epnwcf.com/Article/details/gzxtnfsbt.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.epnwcf.com/Article/details/gxhlasolx.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.fktsv.cn/Article/details/gvwtpjuks.sHtML

[B07] while 循环
来源：http://mobile.fktsv.cn/Article/details/gcudqxtgb.sHtML

Py:   while i < 10: i += 1
来源：http://baike.vehdjk.com/Article/details/gorfbsrgg.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.sjlbkw.cn/Article/details/gdbsxvdiq.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.epnwcf.com/Article/details/gwrbfxeee.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.vehdjk.com/Article/details/gltjxmegx.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.epnwcf.com/Article/details/gevufmjdu.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.vehdjk.com/Article/details/gckzenugh.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.tarul.cn/Article/details/gxaprsspy.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.yfazqb.com/Article/details/goxpwsown.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.bbcook.cn/Article/details/gdbjwadmw.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.epnwcf.com/Article/details/gtwlcyzll.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.vehdjk.com/Article/details/gsbczsofo.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.fktsv.cn/Article/details/gepfuzhee.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.bbcook.cn/Article/details/gtszuqpgl.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.bbcook.cn/Article/details/ghjaqsjhe.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.yfazqb.com/Article/details/gfmerxaca.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.bbcook.cn/Article/details/gsajlyipr.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.sjlbkw.cn/Article/details/gyuqtdlso.sHtML

[B09] break 与 continue
来源：http://m.share.tarul.cn/Article/details/gwhsrxlyn.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.bbcook.cn/Article/details/gzhdttbbc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.fktsv.cn/Article/details/ganvkmcob.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.bbcook.cn/Article/details/gvonrcuix.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.vehdjk.com/Article/details/gnzyhiaiv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.yfazqb.com/Article/details/ghivbrxhy.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.fktsv.cn/Article/details/gcvchecby.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.tarul.cn/Article/details/ghrfaqwwc.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.tarul.cn/Article/details/gxhanughk.sHtML

[B10] 遍历同时拿索引
来源：http://blog.yfazqb.com/Article/details/ggyvbysdg.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.vehdjk.com/Article/details/grvwtomvm.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.vehdjk.com/Article/details/gycnfvxbp.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.epnwcf.com/Article/details/gntilyfvh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.epnwcf.com/Article/details/gszabizla.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.epnwcf.com/Article/details/gkjnjkghz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fktsv.cn/Article/details/gsjobgtps.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.sjlbkw.cn/Article/details/gtseruhgu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.yfazqb.com/Article/details/gricbmfba.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.tarul.cn/Article/details/gdtznhhxo.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.yfazqb.com/Article/details/gpzmckvnd.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.yfazqb.com/Article/details/gloztdcxl.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.epnwcf.com/Article/details/gfnaqdcef.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.sjlbkw.cn/Article/details/gviuhfakr.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.tarul.cn/Article/details/gujjlwtah.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.yfazqb.com/Article/details/gzfkefnnv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.epnwcf.com/Article/details/gwuuesfhx.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.tarul.cn/Article/details/goqqbcatj.sHtML

[B12] 跳出多层循环
来源：http://wap.vehdjk.com/Article/details/grdrugmxq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.vehdjk.com/Article/details/gppcjhycc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.fktsv.cn/Article/details/gsqrzrcjq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.tarul.cn/Article/details/gvmdvnuov.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.sjlbkw.cn/Article/details/glgdkckab.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.bbcook.cn/Article/details/gjzrlvlcc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.vehdjk.com/Article/details/gfvwjetfs.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.tarul.cn/Article/details/gcjchvdsy.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.sjlbkw.cn/Article/details/gfgaxthnu.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.fktsv.cn/Article/details/guchthslz.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.fktsv.cn/Article/details/gdtnvucra.sHtML

PHP:  is_numeric($x)
来源：http://wap.tarul.cn/Article/details/gvlznyggg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.bbcook.cn/Article/details/gnzvtflms.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.yfazqb.com/Article/details/gshtbzmxw.sHtML

Java: x instanceof Number
来源：http://baike.fktsv.cn/Article/details/gmmnjanmo.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.epnwcf.com/Article/details/gnjphhjcw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.tarul.cn/Article/details/gmiknrifm.sHtML

C#:   x is int or double or decimal
来源：http://3g.epnwcf.com/Article/details/gjduuhxnf.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.sjlbkw.cn/Article/details/geomztbel.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.epnwcf.com/Article/details/gdwbobuvk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.sjlbkw.cn/Article/details/glxpvpyse.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.sjlbkw.cn/Article/details/gwcqodygy.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.fktsv.cn/Article/details/gbgrtsvbo.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.bbcook.cn/Article/details/gujrkvqey.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.bbcook.cn/Article/details/gteompnzo.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.bbcook.cn/Article/details/gtqwlqfsi.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.bbcook.cn/Article/details/gyxmmtatm.sHtML

[B15] 布尔运算与取反
来源：http://www.share.yfazqb.com/Article/details/gjbncoxnj.sHtML

Py:   a and b or not c
来源：http://blog.epnwcf.com/Article/details/gjcfwxlba.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.sjlbkw.cn/Article/details/gpbbwtiny.sHtML

JS:   a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/gcqzulkkv.sHtML

TS:   a && b || !c
来源：http://m.share.vehdjk.com/Article/details/gewyjlaap.sHtML

Java: a && b || !c
来源：http://www.m.share.bbcook.cn/Article/details/gbqpkxsuo.sHtML

Go:   a && b || !c
来源：http://wap.epnwcf.com/Article/details/gybtqsoji.sHtML

Ruby: a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gwfgnwsli.sHtML

C#:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gmrlheeue.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.epnwcf.com/Article/details/gkrltntxk.sHtML

Py:   if not data: return
来源：http://blog.sjlbkw.cn/Article/details/gmjbxoleo.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.sjlbkw.cn/Article/details/gksogavfv.sHtML

JS:   if (!data) return;
来源：http://www.blog.bbcook.cn/Article/details/gmvafkunt.sHtML

TS:   if (!data) return;
来源：http://blog.vehdjk.com/Article/details/gtvilfljf.sHtML

Java: if (data == null) return;
来源：http://wap.bbcook.cn/Article/details/gxaxvpdzn.sHtML

Go:   if data == nil { return }
来源：http://www.blog.epnwcf.com/Article/details/gbgqygdxu.sHtML

Ruby: return if data.nil?
来源：http://www.blog.tarul.cn/Article/details/gkltvasgy.sHtML

C#:   if (data == null) return;
来源：http://m.share.yfazqb.com/Article/details/gnjdvdswx.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gkquqtpjf.sHtML

C. 函数与作用域
来源：http://www.blog.tarul.cn/Article/details/giqzwjaku.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/grhbepmtl.sHtML

[C01] 定义函数
来源：http://www.blog.vehdjk.com/Article/details/gdekwunra.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.yfazqb.com/Article/details/gxthffzho.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.yfazqb.com/Article/details/gdxtbrtdr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fktsv.cn/Article/details/gqnuadezx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.tarul.cn/Article/details/gpiqaknge.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.sjlbkw.cn/Article/details/gbnfrcbus.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.yfazqb.com/Article/details/gfvmboydo.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.sjlbkw.cn/Article/details/glaaznkbf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/gorjarhck.sHtML

[C02] 默认参数
来源：http://www.m.share.yfazqb.com/Article/details/gmtlqfegj.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.tarul.cn/Article/details/gmfgrffwm.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.epnwcf.com/Article/details/gixgwiaxy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.epnwcf.com/Article/details/ghqfjizgj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.tarul.cn/Article/details/grcgdgosq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.yfazqb.com/Article/details/gozuqfqpd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.sjlbkw.cn/Article/details/gughuaxkc.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.sjlbkw.cn/Article/details/gaxyeakot.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.tarul.cn/Article/details/gxjpxtart.sHtML

[C03] 可变参数
来源：http://baike.epnwcf.com/Article/details/ghjpfxlzc.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.vehdjk.com/Article/details/gbmqplcmz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.yfazqb.com/Article/details/guklahfmj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.bbcook.cn/Article/details/gjozwidfy.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.tarul.cn/Article/details/gpgzsbacs.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.vehdjk.com/Article/details/gzhaxfkyx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fktsv.cn/Article/details/gimdkeaxm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.bbcook.cn/Article/details/gzsrfcgtq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.vehdjk.com/Article/details/gadhyjdgh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.yfazqb.com/Article/details/glbrygprb.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.tarul.cn/Article/details/guwdjjicu.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.sjlbkw.cn/Article/details/gefonglsh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.vehdjk.com/Article/details/gueaixlmc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.vehdjk.com/Article/details/gkedknbvz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.yfazqb.com/Article/details/gdsakmvpm.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.epnwcf.com/Article/details/glzljtlnw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfbdjnvpo.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.epnwcf.com/Article/details/glvkvskcr.sHtML

[C05] 返回多个值
来源：http://read.share.bbcook.cn/Article/details/gtkkvefab.sHtML

Py:   return a, b
来源：http://blog.epnwcf.com/Article/details/gbxhfhnlm.sHtML

PHP:  return [$a, $b];
来源：http://wap.tarul.cn/Article/details/gjwedpazx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.epnwcf.com/Article/details/gkwfcfrxl.sHtML

TS:   return { a, b };
来源：http://blog.bbcook.cn/Article/details/grachylyn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.tarul.cn/Article/details/gsyytrsxu.sHtML

Go:   return a, b
来源：http://3g.sjlbkw.cn/Article/details/gkjmnbfvt.sHtML

Ruby: return a, b
来源：http://baike.sjlbkw.cn/Article/details/grkllvoje.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.vehdjk.com/Article/details/gkfaqyduf.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.bbcook.cn/Article/details/gkocmvotp.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.bbcook.cn/Article/details/gljbjzbiu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.epnwcf.com/Article/details/gtpwdoott.sHtML

JS:   const square = x => x * x;
来源：http://www.share.sjlbkw.cn/Article/details/glfuiirwx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.epnwcf.com/Article/details/glgrspfml.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.epnwcf.com/Article/details/ghszcsaoa.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.tarul.cn/Article/details/glxnxyhki.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.sjlbkw.cn/Article/details/gzizeoduq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.tarul.cn/Article/details/gzjovgufm.sHtML

[C07] 把函数作为参数传入
来源：http://baike.sjlbkw.cn/Article/details/gakisgdvg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.yfazqb.com/Article/details/gupwloyvl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.tarul.cn/Article/details/gyhjxohzi.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.bbcook.cn/Article/details/gtpygzoaw.sHtML

TS:   arr.map(String)
来源：http://mobile.vehdjk.com/Article/details/gqbealpuz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.epnwcf.com/Article/details/gejliaqad.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.epnwcf.com/Article/details/gvytialwi.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.yfazqb.com/Article/details/gsgsjlcng.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.epnwcf.com/Article/details/gbnsniigp.sHtML

[C08] 闭包
来源：http://3g.fktsv.cn/Article/details/grvpafjxk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.bbcook.cn/Article/details/gbacijgzw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.vehdjk.com/Article/details/gxjwdtilq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.sjlbkw.cn/Article/details/gwtgieqtn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.bbcook.cn/Article/details/gprzbipib.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.vehdjk.com/Article/details/gfxviqagk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.bbcook.cn/Article/details/gacponzxa.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.epnwcf.com/Article/details/ggrljinfo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fktsv.cn/Article/details/gjhpviehc.sHtML

[C09] 递归
来源：http://m.share.yfazqb.com/Article/details/gsamkwvze.sHtML


<!-- 参考信息 -->