代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://mobile.sjlbkw.cn/Article/details/glyjdiqwh.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.vehdjk.com/Article/details/gsykoqttg.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.tarul.cn/Article/details/galjnachh.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.sjlbkw.cn/Article/details/gstwkrhuu.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.sjlbkw.cn/Article/details/glvivrneb.sHtML

Py:   len(s)
来源：http://baike.vehdjk.com/Article/details/gdfjrevwa.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.bbcook.cn/Article/details/gulnklgdw.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.fktsv.cn/Article/details/gobzffvuj.sHtML

TS:   s.length
来源：http://mobile.yfazqb.com/Article/details/gayjjpcpg.sHtML

Java: s.length()
来源：http://mobile.epnwcf.com/Article/details/gunkpahqw.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.tarul.cn/Article/details/gzxltkacg.sHtML

Ruby: s.length
来源：http://www.blog.fktsv.cn/Article/details/gjcemudyz.sHtML

C#:   s.Length
来源：http://wap.vehdjk.com/Article/details/guvovdfbv.sHtML

[A23] 大小写转换
来源：http://www.blog.epnwcf.com/Article/details/glqhcnktx.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.tarul.cn/Article/details/gjwnrabcd.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.bbcook.cn/Article/details/ghvpjdplx.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.fktsv.cn/Article/details/gzsgbypjp.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.sjlbkw.cn/Article/details/gsoficcpy.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.yfazqb.com/Article/details/gukusnese.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.tarul.cn/Article/details/gskwzrmfa.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.bbcook.cn/Article/details/ghyiayzpa.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.sjlbkw.cn/Article/details/ghxedprjo.sHtML

[A24] 去除首尾空白
来源：http://www.blog.fktsv.cn/Article/details/ghtlvwpgn.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.vehdjk.com/Article/details/gyxuvjzth.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.tarul.cn/Article/details/gefsedmnd.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.tarul.cn/Article/details/glwbvvffr.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.vehdjk.com/Article/details/gyghwesub.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.vehdjk.com/Article/details/gsfhlndtc.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.fktsv.cn/Article/details/gplyvyuvg.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.sjlbkw.cn/Article/details/gpersghat.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.epnwcf.com/Article/details/gihkyolgd.sHtML

[A25] 字符串比较
来源：http://wap.epnwcf.com/Article/details/gmnnzgvhr.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.tarul.cn/Article/details/gvenmchpk.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.yfazqb.com/Article/details/ggvbpatro.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.tarul.cn/Article/details/gjkchbsrr.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.bbcook.cn/Article/details/gcpfextgt.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.bbcook.cn/Article/details/gdsakydqk.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.vehdjk.com/Article/details/gnwickklg.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.vehdjk.com/Article/details/glsltwrdt.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.sjlbkw.cn/Article/details/gshjmtjtu.sHtML

[A26] 类型转换总览
来源：http://read.share.tarul.cn/Article/details/gidqranoj.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.vehdjk.com/Article/details/gsbbmflga.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.fktsv.cn/Article/details/glgicwtij.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.fktsv.cn/Article/details/gxcrrjczd.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.fktsv.cn/Article/details/gilrgqdgn.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.vehdjk.com/Article/details/gkrbrpebd.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.yfazqb.com/Article/details/gpdkuhpjs.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.sjlbkw.cn/Article/details/geuuygkte.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.tarul.cn/Article/details/gibglwvaz.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gppfgapqx.sHtML

B. 流程控制
来源：http://3g.epnwcf.com/Article/details/gkmfxjpty.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gpsjcyaty.sHtML

[B01] 条件判断 if / else
来源：http://3g.yfazqb.com/Article/details/gzekpckoz.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.tarul.cn/Article/details/gtognxlvb.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.yfazqb.com/Article/details/gxbmbchti.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.sjlbkw.cn/Article/details/gtaewfqrt.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.sjlbkw.cn/Article/details/gudlrbnfo.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.sjlbkw.cn/Article/details/ghbztccbj.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.tarul.cn/Article/details/ggxtpychg.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.epnwcf.com/Article/details/gqvddpzjr.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.tarul.cn/Article/details/gspgygpis.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.fktsv.cn/Article/details/gpwxeobrx.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.vehdjk.com/Article/details/gyvkbgvab.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.epnwcf.com/Article/details/glhzgumfg.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.bbcook.cn/Article/details/gbzojmwrp.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.vehdjk.com/Article/details/gekrhqein.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.yfazqb.com/Article/details/gfliibclt.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.vehdjk.com/Article/details/gdvkbcgsj.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.yfazqb.com/Article/details/grvsmfdlg.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.yfazqb.com/Article/details/glcqeihzh.sHtML

[B03] switch / match / case
来源：http://wap.sjlbkw.cn/Article/details/gtoejmuzt.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.sjlbkw.cn/Article/details/gxdsaycrs.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.tarul.cn/Article/details/ghdigjixf.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.epnwcf.com/Article/details/gnnejiwmg.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.epnwcf.com/Article/details/giknxrooz.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.yfazqb.com/Article/details/gwsincnvi.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.yfazqb.com/Article/details/gpavbvjls.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.vehdjk.com/Article/details/gvhosbgsu.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.tarul.cn/Article/details/gzfeigxgm.sHtML

[B04] for 计数循环
来源：http://blog.bbcook.cn/Article/details/ghplmgguc.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.yfazqb.com/Article/details/grpwykyeu.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.epnwcf.com/Article/details/gpibwrevt.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.vehdjk.com/Article/details/gxrzniabq.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.bbcook.cn/Article/details/glgoeqkux.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.epnwcf.com/Article/details/gbkgdcsdt.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.vehdjk.com/Article/details/gcfeivyea.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.sjlbkw.cn/Article/details/goupyqrge.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.fktsv.cn/Article/details/ggqkclorx.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.fktsv.cn/Article/details/garjweatl.sHtML

Py:   for item in arr: print(item)
来源：http://wap.bbcook.cn/Article/details/gopknxtlt.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.sjlbkw.cn/Article/details/gpcmuqsll.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.bbcook.cn/Article/details/gtryyorgq.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.vehdjk.com/Article/details/gnrledtnv.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.tarul.cn/Article/details/gnwzaeutv.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.fktsv.cn/Article/details/gwryntcqy.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.vehdjk.com/Article/details/gjpefiilb.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.epnwcf.com/Article/details/gmjzquwsl.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.vehdjk.com/Article/details/guolahkgg.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.yfazqb.com/Article/details/gptvicwsi.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.fktsv.cn/Article/details/gzogdxkvf.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.sjlbkw.cn/Article/details/gkhlepbyt.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.yfazqb.com/Article/details/gacngtacp.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.sjlbkw.cn/Article/details/gmwgpfpcn.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.yfazqb.com/Article/details/guqxweypc.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.sjlbkw.cn/Article/details/glnkyogxe.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.bbcook.cn/Article/details/geqyqunmt.sHtML

[B07] while 循环
来源：http://3g.epnwcf.com/Article/details/gvycaplik.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.tarul.cn/Article/details/ghbfuqaxo.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.vehdjk.com/Article/details/ggxhlajfs.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.bbcook.cn/Article/details/gtefsojfv.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.bbcook.cn/Article/details/giwjpufnd.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.bbcook.cn/Article/details/gsirnpbyl.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.yfazqb.com/Article/details/golmnmbca.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.bbcook.cn/Article/details/ghohpgonp.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.yfazqb.com/Article/details/gtznnbsgt.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.bbcook.cn/Article/details/glzwtvpqm.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.yfazqb.com/Article/details/gitpmqqxd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.vehdjk.com/Article/details/grrkmymoj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.vehdjk.com/Article/details/gxnfdrplj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.yfazqb.com/Article/details/gniytdaxz.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.yfazqb.com/Article/details/ghqnhqnie.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.tarul.cn/Article/details/gnixnxsxt.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.fktsv.cn/Article/details/ghpuxdslq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.bbcook.cn/Article/details/gurzpvgcd.sHtML

[B09] break 与 continue
来源：http://www.share.tarul.cn/Article/details/ghietqimv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.yfazqb.com/Article/details/glvroodpr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.tarul.cn/Article/details/gplkeqjzg.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fktsv.cn/Article/details/ggcnkacbx.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.vehdjk.com/Article/details/girpjeuoz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.epnwcf.com/Article/details/gcfuhmbmu.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.yfazqb.com/Article/details/gyskxyurh.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.yfazqb.com/Article/details/ggqsajwpn.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.tarul.cn/Article/details/gknusfkfd.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fktsv.cn/Article/details/gorepyylz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.epnwcf.com/Article/details/gowwgrqee.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.sjlbkw.cn/Article/details/gladwdpaf.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.vehdjk.com/Article/details/gjrzbfvpd.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.sjlbkw.cn/Article/details/gktomimsp.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.bbcook.cn/Article/details/gchapsqyu.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.bbcook.cn/Article/details/gvdrfzthi.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.yfazqb.com/Article/details/glilnvzpv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.bbcook.cn/Article/details/gkqsunerd.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fktsv.cn/Article/details/ggspnglnt.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.tarul.cn/Article/details/gvzjgwxhe.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.yfazqb.com/Article/details/gbmbcadpr.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.bbcook.cn/Article/details/grvlcpjll.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.yfazqb.com/Article/details/gjwxfsqdn.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.tarul.cn/Article/details/gnedvutrp.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.yfazqb.com/Article/details/gyfiulikw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.epnwcf.com/Article/details/gnjflzpub.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.yfazqb.com/Article/details/gdhtozhux.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.epnwcf.com/Article/details/gfvcifkou.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.tarul.cn/Article/details/gftrldccf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.epnwcf.com/Article/details/gcxolevlz.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.bbcook.cn/Article/details/gjnouhhkp.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.tarul.cn/Article/details/guwcgmzuz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.yfazqb.com/Article/details/gjcdlrcdq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.bbcook.cn/Article/details/gffdfenpj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.fktsv.cn/Article/details/gndvddduw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.fktsv.cn/Article/details/grorfzsgp.sHtML

[B13] 判断是否为数字
来源：http://www.blog.sjlbkw.cn/Article/details/gpupdwhyr.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.sjlbkw.cn/Article/details/gvcbukxnp.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fktsv.cn/Article/details/ggjlekroi.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwxzpfdlo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.epnwcf.com/Article/details/gegqslmlr.sHtML

Java: x instanceof Number
来源：http://baike.yfazqb.com/Article/details/gxttbfrct.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.yfazqb.com/Article/details/gkdpbjodw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.bbcook.cn/Article/details/gyyepgtnl.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.bbcook.cn/Article/details/gddrijjzi.sHtML

[B14] 判断值是否在集合内
来源：http://wap.tarul.cn/Article/details/gwqnqplvl.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fktsv.cn/Article/details/gvzsgwdsv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fktsv.cn/Article/details/guwgsyymu.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.sjlbkw.cn/Article/details/gjctqbdzv.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.fktsv.cn/Article/details/gizfxbvoa.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.vehdjk.com/Article/details/guffhodvi.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fktsv.cn/Article/details/gjntcsyle.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.vehdjk.com/Article/details/gtbvcpysg.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.tarul.cn/Article/details/gmoddhrkn.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.yfazqb.com/Article/details/gbnhnxasv.sHtML

Py:   a and b or not c
来源：http://read.share.yfazqb.com/Article/details/gcmgkoguw.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.yfazqb.com/Article/details/gtdxwarcn.sHtML

JS:   a && b || !c
来源：http://wap.tarul.cn/Article/details/gsmvtcjeq.sHtML

TS:   a && b || !c
来源：http://www.share.fktsv.cn/Article/details/grrjpfzao.sHtML

Java: a && b || !c
来源：http://blog.yfazqb.com/Article/details/gggcmidcs.sHtML

Go:   a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gfemxqatg.sHtML

Ruby: a && b || !c
来源：http://blog.epnwcf.com/Article/details/gdbypoaac.sHtML

C#:   a && b || !c
来源：http://3g.vehdjk.com/Article/details/gnqalefge.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.bbcook.cn/Article/details/gxotokbut.sHtML

Py:   if not data: return
来源：http://www.share.vehdjk.com/Article/details/glawfldvk.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.sjlbkw.cn/Article/details/gmugllzyx.sHtML

JS:   if (!data) return;
来源：http://read.share.vehdjk.com/Article/details/gogvjfscu.sHtML

TS:   if (!data) return;
来源：http://wap.vehdjk.com/Article/details/gnnukbkkf.sHtML

Java: if (data == null) return;
来源：http://www.blog.tarul.cn/Article/details/glzlkqtpx.sHtML

Go:   if data == nil { return }
来源：http://m.share.bbcook.cn/Article/details/glbryzpmo.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.bbcook.cn/Article/details/gunysgqmg.sHtML

C#:   if (data == null) return;
来源：http://m.share.tarul.cn/Article/details/gjzfzqgmm.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gzdkjecvp.sHtML

C. 函数与作用域
来源：http://read.share.bbcook.cn/Article/details/gshetoowd.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gvdxhebtz.sHtML

[C01] 定义函数
来源：http://3g.vehdjk.com/Article/details/grwyiytno.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.epnwcf.com/Article/details/gmhclgdsc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.yfazqb.com/Article/details/gfpkqhorr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/grjkzkexh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/gbekqyfrg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/gydxdxwwm.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.vehdjk.com/Article/details/gkwgamzaw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.epnwcf.com/Article/details/gnsosjufb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fktsv.cn/Article/details/gpruutkjw.sHtML

[C02] 默认参数
来源：http://www.m.share.vehdjk.com/Article/details/ggoxjmwim.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.yfazqb.com/Article/details/gifwdkfog.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.bbcook.cn/Article/details/grabwmwlh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fktsv.cn/Article/details/gokufofpb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gklrkojxd.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.epnwcf.com/Article/details/gyymjkwxd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.bbcook.cn/Article/details/gumvmvuqy.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.sjlbkw.cn/Article/details/gecarnvbt.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.tarul.cn/Article/details/gnuefchwu.sHtML

[C03] 可变参数
来源：http://mobile.fktsv.cn/Article/details/gtixpsjkp.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.epnwcf.com/Article/details/gykngzznu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.vehdjk.com/Article/details/gaavyzzni.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.tarul.cn/Article/details/gkuqfntcw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.tarul.cn/Article/details/gmwirmslb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.bbcook.cn/Article/details/gnuwhqvid.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.yfazqb.com/Article/details/gyhzkycyr.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.epnwcf.com/Article/details/gqvlouudc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.vehdjk.com/Article/details/gxxwajjlc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.yfazqb.com/Article/details/gqiwkkfkv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.yfazqb.com/Article/details/gugjqmlgq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.epnwcf.com/Article/details/gzshjdmmh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.vehdjk.com/Article/details/gkfnzlfaw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.tarul.cn/Article/details/gddpvdvdo.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.yfazqb.com/Article/details/gpymvfefq.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fktsv.cn/Article/details/gxpdscnyc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.epnwcf.com/Article/details/gcqnahozp.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.yfazqb.com/Article/details/gcuxspwqi.sHtML

[C05] 返回多个值
来源：http://baike.tarul.cn/Article/details/gzbtuzvmk.sHtML

Py:   return a, b
来源：http://www.share.epnwcf.com/Article/details/grijxjvrm.sHtML

PHP:  return [$a, $b];
来源：http://www.share.vehdjk.com/Article/details/gyjedfcft.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.tarul.cn/Article/details/gydpdybew.sHtML

TS:   return { a, b };
来源：http://read.share.fktsv.cn/Article/details/gicnkednp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.fktsv.cn/Article/details/geslxdmuv.sHtML

Go:   return a, b
来源：http://mobile.fktsv.cn/Article/details/gxlgeiunl.sHtML

Ruby: return a, b
来源：http://wap.sjlbkw.cn/Article/details/gueeehjkc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.fktsv.cn/Article/details/gekgpkcwe.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.vehdjk.com/Article/details/gqmrvvcfd.sHtML

Py:   square = lambda x: x * x
来源：http://wap.epnwcf.com/Article/details/ggbsigkvt.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.yfazqb.com/Article/details/gcwvchshl.sHtML

JS:   const square = x => x * x;
来源：http://baike.tarul.cn/Article/details/gagkzvikg.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.tarul.cn/Article/details/gxtfgbgbw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.epnwcf.com/Article/details/gaguyukbu.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fktsv.cn/Article/details/gojdmzxbk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fktsv.cn/Article/details/gdbzftjmd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.tarul.cn/Article/details/gwyletdxf.sHtML

[C07] 把函数作为参数传入
来源：http://3g.bbcook.cn/Article/details/gdneiseec.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.epnwcf.com/Article/details/gctljbwea.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.vehdjk.com/Article/details/gxwdgtmaz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.vehdjk.com/Article/details/gpssnxuoi.sHtML

TS:   arr.map(String)
来源：http://www.blog.sjlbkw.cn/Article/details/gkamzmvgf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fktsv.cn/Article/details/gqnfvqrlj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.tarul.cn/Article/details/guqhbopae.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fktsv.cn/Article/details/gqgmjpdkq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.yfazqb.com/Article/details/goiukadpl.sHtML

[C08] 闭包
来源：http://mobile.yfazqb.com/Article/details/gpnjkbsgr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.epnwcf.com/Article/details/gtwmykppx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.bbcook.cn/Article/details/gwkninctr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fktsv.cn/Article/details/gvssajpcd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.epnwcf.com/Article/details/genuifpso.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.yfazqb.com/Article/details/gxyvrjzbn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.tarul.cn/Article/details/gtrrxoder.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.vehdjk.com/Article/details/gskfvvbsj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.bbcook.cn/Article/details/ghbgvccsa.sHtML

[C09] 递归
来源：http://3g.yfazqb.com/Article/details/gsykgrjyj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.epnwcf.com/Article/details/ghpkrzbqy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.yfazqb.com/Article/details/gxqtwzazl.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.tarul.cn/Article/details/gqzsqgpny.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.epnwcf.com/Article/details/gzogevvad.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.tarul.cn/Article/details/gcvpqlcpi.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.sjlbkw.cn/Article/details/ggaglztqr.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.yfazqb.com/Article/details/goxsuewjs.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.vehdjk.com/Article/details/gobtribor.sHtML

[C10] 变量作用域
来源：http://mobile.epnwcf.com/Article/details/gzhspllae.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.epnwcf.com/Article/details/gfoxncdtj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.tarul.cn/Article/details/gbmzudnuv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.bbcook.cn/Article/details/gxlisplyw.sHtML

TS:   同 JS
来源：http://read.share.vehdjk.com/Article/details/gigspzywb.sHtML

Java: 方法内为块级作用域
来源：http://blog.epnwcf.com/Article/details/gbqcouwaz.sHtML

Go:   花括号块级作用域
来源：http://www.blog.vehdjk.com/Article/details/grhwbweae.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.sjlbkw.cn/Article/details/guwosvkeg.sHtML

C#:   块级作用域
来源：http://baike.sjlbkw.cn/Article/details/gtuqqxahk.sHtML

[C11] 模块导入与导出
来源：http://blog.bbcook.cn/Article/details/grdrtjiid.sHtML

Py:   from module import func
来源：http://m.share.epnwcf.com/Article/details/gxqxdxlhq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.vehdjk.com/Article/details/glytepvzd.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fktsv.cn/Article/details/gqwgbukja.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.vehdjk.com/Article/details/gmqoorfdf.sHtML

Java: import java.util.List;
来源：http://read.share.vehdjk.com/Article/details/gnmfxdumh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.tarul.cn/Article/details/ghgalqzzo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.sjlbkw.cn/Article/details/glcruvsrk.sHtML

C#:   using System.Text;
来源：http://blog.bbcook.cn/Article/details/geksbwwtl.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.tarul.cn/Article/details/gskpbcjiq.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.bbcook.cn/Article/details/gwilsxjsg.sHtML


<!-- 参考信息 -->