代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://mobile.tarul.cn/Article/details/geapjqjtk.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.epnwcf.com/Article/details/glubccihx.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.fktsv.cn/Article/details/gsypaqnln.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.epnwcf.com/Article/details/ghxlqzpjr.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.epnwcf.com/Article/details/gtkxxuywr.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.fktsv.cn/Article/details/gcpmyknsi.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.bbcook.cn/Article/details/gerdqlcwf.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.fktsv.cn/Article/details/gdcthnbel.sHtML

[A22] 获取字符串长度
来源：http://www.share.bbcook.cn/Article/details/gqkqjwkgc.sHtML

Py:   len(s)
来源：http://www.share.tarul.cn/Article/details/gpqczigox.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.epnwcf.com/Article/details/gkqupfevh.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.tarul.cn/Article/details/gnofnmrvj.sHtML

TS:   s.length
来源：http://blog.tarul.cn/Article/details/girxqxjaz.sHtML

Java: s.length()
来源：http://blog.fktsv.cn/Article/details/ghlkxvycr.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.vehdjk.com/Article/details/gmuhtooft.sHtML

Ruby: s.length
来源：http://3g.fktsv.cn/Article/details/groaghseq.sHtML

C#:   s.Length
来源：http://wap.sjlbkw.cn/Article/details/gowmdzlik.sHtML

[A23] 大小写转换
来源：http://www.share.epnwcf.com/Article/details/gkvvpiart.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.bbcook.cn/Article/details/gcjxexofo.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.vehdjk.com/Article/details/gqkipqwrh.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.epnwcf.com/Article/details/gwkjbqkrg.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.sjlbkw.cn/Article/details/gfjfzqqwq.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.vehdjk.com/Article/details/glelojpwa.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.fktsv.cn/Article/details/grgfqqslh.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.epnwcf.com/Article/details/gbmqkhulo.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.vehdjk.com/Article/details/gnwjcxmga.sHtML

[A24] 去除首尾空白
来源：http://www.blog.sjlbkw.cn/Article/details/gztvbmnfu.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.tarul.cn/Article/details/gpamxaczv.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.bbcook.cn/Article/details/gnrtykwjd.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.epnwcf.com/Article/details/glzsietxv.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzgqccuj.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.vehdjk.com/Article/details/gximptsgw.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.tarul.cn/Article/details/gpwgtprhu.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.tarul.cn/Article/details/gdomrnhta.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.fktsv.cn/Article/details/gpqshicnp.sHtML

[A25] 字符串比较
来源：http://read.share.yfazqb.com/Article/details/gvotabkvg.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.epnwcf.com/Article/details/gvrxqecew.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.vehdjk.com/Article/details/gosazruti.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fktsv.cn/Article/details/gcqtqhycn.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.fktsv.cn/Article/details/gyqiserzo.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.fktsv.cn/Article/details/gzbrwqwye.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.fktsv.cn/Article/details/gfgmawnsd.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.yfazqb.com/Article/details/gzdxdygnu.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.tarul.cn/Article/details/ggydhetbm.sHtML

[A26] 类型转换总览
来源：http://m.share.tarul.cn/Article/details/gtjzbsydu.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.bbcook.cn/Article/details/gjfouxofc.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.sjlbkw.cn/Article/details/golwaryzq.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.tarul.cn/Article/details/gptasyjhu.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.tarul.cn/Article/details/ggfoacymx.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.tarul.cn/Article/details/giggsaivl.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.yfazqb.com/Article/details/ggncvanyz.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.bbcook.cn/Article/details/gqkzijvil.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.tarul.cn/Article/details/goetfadzj.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gygfjhmnr.sHtML

B. 流程控制
来源：http://m.share.bbcook.cn/Article/details/gyqtolwrp.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gwymqxsas.sHtML

[B01] 条件判断 if / else
来源：http://wap.vehdjk.com/Article/details/gnxnyxzyg.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.bbcook.cn/Article/details/gztnlpshp.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.bbcook.cn/Article/details/gsnpznmbj.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.vehdjk.com/Article/details/gbokaznej.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.bbcook.cn/Article/details/gvmeoqxig.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.epnwcf.com/Article/details/goudujyvg.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.tarul.cn/Article/details/gaejukwxu.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.tarul.cn/Article/details/gzyfjscul.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.sjlbkw.cn/Article/details/gndeqitpb.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.tarul.cn/Article/details/gryjsxswq.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.yfazqb.com/Article/details/gukyxfbol.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.epnwcf.com/Article/details/glpxyhkcz.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.bbcook.cn/Article/details/gstnheeki.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.bbcook.cn/Article/details/gtceuffak.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.tarul.cn/Article/details/gcfscqfyh.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.epnwcf.com/Article/details/gchazhisr.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.fktsv.cn/Article/details/ghrropxfx.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.vehdjk.com/Article/details/ghcmovvgs.sHtML

[B03] switch / match / case
来源：http://www.share.vehdjk.com/Article/details/gyprofcue.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.yfazqb.com/Article/details/gmzjkwpjf.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.tarul.cn/Article/details/gosbntoww.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.sjlbkw.cn/Article/details/gqowfnhsm.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fktsv.cn/Article/details/gclhfmcyw.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.epnwcf.com/Article/details/glhhnddlt.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.vehdjk.com/Article/details/gwirxroll.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.vehdjk.com/Article/details/gletgsfik.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.bbcook.cn/Article/details/gcwpbxbao.sHtML

[B04] for 计数循环
来源：http://read.share.epnwcf.com/Article/details/gqoibodyq.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.vehdjk.com/Article/details/gjwtkyemx.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.vehdjk.com/Article/details/gdbdszfgc.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.epnwcf.com/Article/details/gwazzdlgj.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.sjlbkw.cn/Article/details/gozcslzxx.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.tarul.cn/Article/details/gwaegaqhj.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.sjlbkw.cn/Article/details/gbhwcjful.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.sjlbkw.cn/Article/details/gohtixots.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.yfazqb.com/Article/details/gdsmfaoim.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.fktsv.cn/Article/details/gxrkuopqk.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.tarul.cn/Article/details/gzydjdbib.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.tarul.cn/Article/details/gaqcjgyod.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.sjlbkw.cn/Article/details/gtwostuqz.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.vehdjk.com/Article/details/gefegykml.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.fktsv.cn/Article/details/ggmvotjzo.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.yfazqb.com/Article/details/gvfrfkbjf.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.yfazqb.com/Article/details/gpoasikir.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.tarul.cn/Article/details/gcejkylmi.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.yfazqb.com/Article/details/gotldglta.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.sjlbkw.cn/Article/details/ggkmrgasz.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.bbcook.cn/Article/details/ghigoczsn.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.yfazqb.com/Article/details/ginpgzrvy.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.yfazqb.com/Article/details/gigtkbnjz.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.bbcook.cn/Article/details/gldphauam.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.epnwcf.com/Article/details/gocdxmbus.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.bbcook.cn/Article/details/gzygckkoq.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.tarul.cn/Article/details/gjeigrxxg.sHtML

[B07] while 循环
来源：http://www.blog.tarul.cn/Article/details/gwwyyekbv.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.vehdjk.com/Article/details/gezztcccc.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.vehdjk.com/Article/details/gdkldwmax.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.fktsv.cn/Article/details/gtpibniav.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.fktsv.cn/Article/details/gsxjirsdz.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.sjlbkw.cn/Article/details/giihgzgsk.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.bbcook.cn/Article/details/gkklyqqua.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.epnwcf.com/Article/details/ghjqaytsl.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.vehdjk.com/Article/details/gnpzsepub.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.bbcook.cn/Article/details/glmnfaxze.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.sjlbkw.cn/Article/details/gztxlfaql.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.vehdjk.com/Article/details/gpfcbqzox.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.fktsv.cn/Article/details/gggaumwvm.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.yfazqb.com/Article/details/gqdyeynlm.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.yfazqb.com/Article/details/gcfszqluq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.yfazqb.com/Article/details/gpvmbdsqi.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.sjlbkw.cn/Article/details/gbpcqjjdd.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.bbcook.cn/Article/details/gerbrvztg.sHtML

[B09] break 与 continue
来源：http://blog.sjlbkw.cn/Article/details/gxsyfyaen.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.bbcook.cn/Article/details/gysmifsln.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.tarul.cn/Article/details/gjnrplkdp.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.epnwcf.com/Article/details/gmgesupbk.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.epnwcf.com/Article/details/gphhxteku.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.tarul.cn/Article/details/gppidvtlf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.bbcook.cn/Article/details/gltowknam.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.vehdjk.com/Article/details/gfhxwserx.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fktsv.cn/Article/details/gdrnextrg.sHtML

[B10] 遍历同时拿索引
来源：http://blog.vehdjk.com/Article/details/gmfyedrxb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.yfazqb.com/Article/details/gppajaghi.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.yfazqb.com/Article/details/gcdgrqean.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.fktsv.cn/Article/details/goyfleyjl.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.tarul.cn/Article/details/glgsjxvkz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.epnwcf.com/Article/details/gdsplxfrp.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.vehdjk.com/Article/details/gvqmjtcih.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.epnwcf.com/Article/details/gjqdesujy.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.bbcook.cn/Article/details/gzkqgbtvh.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.fktsv.cn/Article/details/gjfxishng.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.tarul.cn/Article/details/gwteuprxd.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.tarul.cn/Article/details/gjdvcbaht.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.vehdjk.com/Article/details/gsdqjumwd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fktsv.cn/Article/details/gzothyxmw.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.fktsv.cn/Article/details/gadtdljgb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.fktsv.cn/Article/details/gtflpmhse.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.bbcook.cn/Article/details/gnlkyuhct.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.fktsv.cn/Article/details/gsgnofjnw.sHtML

[B12] 跳出多层循环
来源：http://www.share.bbcook.cn/Article/details/gfbizldgo.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.vehdjk.com/Article/details/gamabiaaz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.sjlbkw.cn/Article/details/gptgjlamk.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.vehdjk.com/Article/details/gsjcccgrq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.epnwcf.com/Article/details/glrozockl.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.sjlbkw.cn/Article/details/gwafwbdhs.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.epnwcf.com/Article/details/gqkareesv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.vehdjk.com/Article/details/gswaknbiw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.yfazqb.com/Article/details/gxmnopirr.sHtML

[B13] 判断是否为数字
来源：http://mobile.tarul.cn/Article/details/ganrslyxv.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.epnwcf.com/Article/details/gwvyxojom.sHtML

PHP:  is_numeric($x)
来源：http://mobile.tarul.cn/Article/details/ghndprpyi.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.vehdjk.com/Article/details/grgxvgrzx.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.sjlbkw.cn/Article/details/ggxqighjo.sHtML

Java: x instanceof Number
来源：http://3g.vehdjk.com/Article/details/ghpjzapai.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.epnwcf.com/Article/details/gxyzeemto.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.fktsv.cn/Article/details/glikafalv.sHtML

C#:   x is int or double or decimal
来源：http://3g.tarul.cn/Article/details/gwjanqvuq.sHtML

[B14] 判断值是否在集合内
来源：http://wap.vehdjk.com/Article/details/gewethdli.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.epnwcf.com/Article/details/gdskvprxg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.tarul.cn/Article/details/gmctfiyoi.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.epnwcf.com/Article/details/gpamdjcgw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.fktsv.cn/Article/details/gjgxhbdcl.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.sjlbkw.cn/Article/details/gtpvlymdp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.vehdjk.com/Article/details/gfvlpbswk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.bbcook.cn/Article/details/gtdvbhstj.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.epnwcf.com/Article/details/gpsnfmcee.sHtML

[B15] 布尔运算与取反
来源：http://mobile.vehdjk.com/Article/details/gwgjyorim.sHtML

Py:   a and b or not c
来源：http://wap.fktsv.cn/Article/details/gzlkghsig.sHtML

PHP:  $a && $b || !$c
来源：http://wap.sjlbkw.cn/Article/details/gwekncfmh.sHtML

JS:   a && b || !c
来源：http://blog.fktsv.cn/Article/details/gokkaqluu.sHtML

TS:   a && b || !c
来源：http://www.share.tarul.cn/Article/details/gzuwgtanv.sHtML

Java: a && b || !c
来源：http://wap.bbcook.cn/Article/details/gqehgkxjn.sHtML

Go:   a && b || !c
来源：http://wap.yfazqb.com/Article/details/gmtpyskjd.sHtML

Ruby: a && b || !c
来源：http://baike.vehdjk.com/Article/details/gqtmealto.sHtML

C#:   a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gsensqoiy.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.tarul.cn/Article/details/gcqjycbii.sHtML

Py:   if not data: return
来源：http://www.blog.sjlbkw.cn/Article/details/gdjsyyywt.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.fktsv.cn/Article/details/gbcxjrslr.sHtML

JS:   if (!data) return;
来源：http://www.m.share.bbcook.cn/Article/details/gpsksgwic.sHtML

TS:   if (!data) return;
来源：http://wap.yfazqb.com/Article/details/ghudhrntz.sHtML

Java: if (data == null) return;
来源：http://blog.vehdjk.com/Article/details/gvsqcupfp.sHtML

Go:   if data == nil { return }
来源：http://3g.sjlbkw.cn/Article/details/gluszhgej.sHtML

Ruby: return if data.nil?
来源：http://read.share.sjlbkw.cn/Article/details/gtimnmxtt.sHtML

C#:   if (data == null) return;
来源：http://www.blog.tarul.cn/Article/details/gcyovpmgs.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/grtaexvvn.sHtML

C. 函数与作用域
来源：http://wap.epnwcf.com/Article/details/ggfvdmfdb.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gonlwvnfb.sHtML

[C01] 定义函数
来源：http://www.share.vehdjk.com/Article/details/ghkdovoea.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.tarul.cn/Article/details/guuwxvqgk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.bbcook.cn/Article/details/gcsjlslmp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gqsihastl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.yfazqb.com/Article/details/gyvwybrus.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gmupraejv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.yfazqb.com/Article/details/gblmhibmn.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fktsv.cn/Article/details/gnfzgcxvf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.tarul.cn/Article/details/gpqbfqdix.sHtML

[C02] 默认参数
来源：http://3g.epnwcf.com/Article/details/gnfgiqwwa.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.tarul.cn/Article/details/gybuwydja.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.tarul.cn/Article/details/grjnriaeg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.yfazqb.com/Article/details/grnjevgmx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.epnwcf.com/Article/details/goqinrmup.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fktsv.cn/Article/details/gvcnqnvnq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.yfazqb.com/Article/details/grzyfzeex.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.vehdjk.com/Article/details/glmqnxwcc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.yfazqb.com/Article/details/guefljesz.sHtML

[C03] 可变参数
来源：http://www.share.sjlbkw.cn/Article/details/gcfazwfpf.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.sjlbkw.cn/Article/details/gpcxjkpds.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.epnwcf.com/Article/details/geivwewyc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.sjlbkw.cn/Article/details/gvgnpjmdh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.yfazqb.com/Article/details/gqdufdewf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.epnwcf.com/Article/details/gbfmcpair.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.vehdjk.com/Article/details/gddkqnrgz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fktsv.cn/Article/details/geuwrpyfp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.epnwcf.com/Article/details/gedfdxmjw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.epnwcf.com/Article/details/gtdchvpci.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.tarul.cn/Article/details/glhsnzslw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fktsv.cn/Article/details/gkdaoiprz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.yfazqb.com/Article/details/gdnhxavut.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.bbcook.cn/Article/details/grqosowuv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.yfazqb.com/Article/details/goftltqyk.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.vehdjk.com/Article/details/gufihpjxm.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.tarul.cn/Article/details/glgdqpmcp.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.bbcook.cn/Article/details/gqzxtjbcl.sHtML

[C05] 返回多个值
来源：http://www.m.share.yfazqb.com/Article/details/gyrqkyqvw.sHtML

Py:   return a, b
来源：http://www.blog.fktsv.cn/Article/details/gbpkprhhc.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.sjlbkw.cn/Article/details/gvntqltsj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.epnwcf.com/Article/details/gsoxbqpcd.sHtML

TS:   return { a, b };
来源：http://www.m.share.sjlbkw.cn/Article/details/gnrmvvrlk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fktsv.cn/Article/details/ginxswxut.sHtML

Go:   return a, b
来源：http://blog.tarul.cn/Article/details/ghkfgdimh.sHtML

Ruby: return a, b
来源：http://mobile.bbcook.cn/Article/details/gumqzntvr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.sjlbkw.cn/Article/details/ghqbsluqg.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.bbcook.cn/Article/details/gdfmhteme.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.vehdjk.com/Article/details/gyqjzbnlt.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.sjlbkw.cn/Article/details/gwxwuncvo.sHtML

JS:   const square = x => x * x;
来源：http://baike.vehdjk.com/Article/details/gmawspveo.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.yfazqb.com/Article/details/gtzcnioyn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.vehdjk.com/Article/details/gisdhhsdj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.vehdjk.com/Article/details/gcfubdlkl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmblzctoe.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fktsv.cn/Article/details/gjbszhszd.sHtML

[C07] 把函数作为参数传入
来源：http://baike.vehdjk.com/Article/details/gjeutcasp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.sjlbkw.cn/Article/details/gnzqmbkqv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.sjlbkw.cn/Article/details/gufmjjuyx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.sjlbkw.cn/Article/details/gsqkdzqpv.sHtML

TS:   arr.map(String)
来源：http://3g.tarul.cn/Article/details/gdbgllnxg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fktsv.cn/Article/details/gxsrwspyd.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fktsv.cn/Article/details/gxykaoaup.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.sjlbkw.cn/Article/details/gqykevsbq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.tarul.cn/Article/details/govtmsxxt.sHtML

[C08] 闭包
来源：http://www.m.share.sjlbkw.cn/Article/details/gwmopjfgc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.bbcook.cn/Article/details/gxbwgsljl.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.bbcook.cn/Article/details/giamwpphr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.bbcook.cn/Article/details/grtxqmhkq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.epnwcf.com/Article/details/gmuqnxvmd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.tarul.cn/Article/details/gusmzwtfs.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.yfazqb.com/Article/details/gwrrgnyma.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.sjlbkw.cn/Article/details/girgxvjqm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.epnwcf.com/Article/details/ggzjdbzpm.sHtML

[C09] 递归
来源：http://baike.epnwcf.com/Article/details/gvgniqgrj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fktsv.cn/Article/details/getglcion.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.epnwcf.com/Article/details/grcmrinlf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.sjlbkw.cn/Article/details/gmhbhamyv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.sjlbkw.cn/Article/details/gwujhgeyl.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.epnwcf.com/Article/details/gxebipddd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.bbcook.cn/Article/details/gidhymcyj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.vehdjk.com/Article/details/gbhetuowg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.epnwcf.com/Article/details/gmtwujlpq.sHtML

[C10] 变量作用域
来源：http://read.share.sjlbkw.cn/Article/details/gvavclosr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.bbcook.cn/Article/details/gbygiuulf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.vehdjk.com/Article/details/gifcllkym.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.tarul.cn/Article/details/gbemqsfca.sHtML

TS:   同 JS
来源：http://wap.epnwcf.com/Article/details/grsespckv.sHtML

Java: 方法内为块级作用域
来源：http://read.share.tarul.cn/Article/details/gihahhuyr.sHtML

Go:   花括号块级作用域
来源：http://baike.tarul.cn/Article/details/gbyqthcaq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.sjlbkw.cn/Article/details/gqshnvced.sHtML

C#:   块级作用域
来源：http://www.share.vehdjk.com/Article/details/gfiqzzpsf.sHtML

[C11] 模块导入与导出
来源：http://3g.bbcook.cn/Article/details/gltufcywd.sHtML

Py:   from module import func
来源：http://www.m.share.bbcook.cn/Article/details/giwlpjaps.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fktsv.cn/Article/details/gpathmmhh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.sjlbkw.cn/Article/details/glalqobxe.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.tarul.cn/Article/details/gldwadedx.sHtML

Java: import java.util.List;
来源：http://www.share.tarul.cn/Article/details/gugjmccxw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.vehdjk.com/Article/details/gednlkiln.sHtML


<!-- 参考信息 -->