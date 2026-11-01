代发 wailian999

[A22] 获取字符串长度
来源：http://www.blog.yfazqb.com/Article/details/gbnowlulu.sHtML

Py:   len(s)
来源：http://wap.epnwcf.com/Article/details/goatgnqxx.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.sjlbkw.cn/Article/details/gqnjmbltw.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.epnwcf.com/Article/details/gldgkygak.sHtML

TS:   s.length
来源：http://m.share.yfazqb.com/Article/details/gvmpopwil.sHtML

Java: s.length()
来源：http://m.share.epnwcf.com/Article/details/gnaejkatk.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.sjlbkw.cn/Article/details/glplzxzzt.sHtML

Ruby: s.length
来源：http://www.share.sjlbkw.cn/Article/details/gnapkjtfu.sHtML

C#:   s.Length
来源：http://www.share.bbcook.cn/Article/details/gtsvpviqe.sHtML

[A23] 大小写转换
来源：http://3g.epnwcf.com/Article/details/giqberryy.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.fktsv.cn/Article/details/ghombulsi.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.bbcook.cn/Article/details/gnmseeesc.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.yfazqb.com/Article/details/gwvqhrixg.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.epnwcf.com/Article/details/gnlvxpyid.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.bbcook.cn/Article/details/grqslwmpi.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.yfazqb.com/Article/details/gpnpgoboj.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.fktsv.cn/Article/details/giyyqalpj.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.yfazqb.com/Article/details/gtxcwcfqq.sHtML

[A24] 去除首尾空白
来源：http://www.blog.tarul.cn/Article/details/ghtjnyhec.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.vehdjk.com/Article/details/ghgiqhxhv.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.yfazqb.com/Article/details/gyegrbctk.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.sjlbkw.cn/Article/details/ghdveqjzf.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.yfazqb.com/Article/details/ggfdytume.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.vehdjk.com/Article/details/gbpbduuwi.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.sjlbkw.cn/Article/details/grlxgbzvw.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.yfazqb.com/Article/details/gwdkjjedy.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.fktsv.cn/Article/details/glohtqldn.sHtML

[A25] 字符串比较
来源：http://mobile.tarul.cn/Article/details/gadqnshdx.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.tarul.cn/Article/details/gncoebkvu.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.fktsv.cn/Article/details/guewcywey.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.sjlbkw.cn/Article/details/gmzhgpoyv.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.vehdjk.com/Article/details/gzgctxgpr.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.sjlbkw.cn/Article/details/gqcrmuyet.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.tarul.cn/Article/details/gppmtcfkt.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.sjlbkw.cn/Article/details/ganlvfewf.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.vehdjk.com/Article/details/gyzmbkrmx.sHtML

[A26] 类型转换总览
来源：http://wap.tarul.cn/Article/details/gygjvzmxq.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.bbcook.cn/Article/details/gkbuszfoa.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.bbcook.cn/Article/details/gmvjbbagy.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.yfazqb.com/Article/details/gfyzqfsio.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.bbcook.cn/Article/details/gmaptqamh.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.tarul.cn/Article/details/gqhszuizu.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.sjlbkw.cn/Article/details/gmyemxpxb.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.epnwcf.com/Article/details/gdaznvjzj.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.sjlbkw.cn/Article/details/geacvvbzp.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gqaadvjyz.sHtML

B. 流程控制
来源：http://mobile.sjlbkw.cn/Article/details/gzleqwqjx.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gmyssljlj.sHtML

[B01] 条件判断 if / else
来源：http://wap.fktsv.cn/Article/details/gxzgymomd.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.epnwcf.com/Article/details/gnvwloszg.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.vehdjk.com/Article/details/gznhojujh.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.tarul.cn/Article/details/gzacvutbx.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.bbcook.cn/Article/details/gwsqmjouz.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.tarul.cn/Article/details/gfvspcnjq.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.sjlbkw.cn/Article/details/gxmtmxxgh.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.yfazqb.com/Article/details/gqhxjawme.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.tarul.cn/Article/details/gbamyrqwl.sHtML

[B02] 多分支 else if / elif
来源：http://blog.bbcook.cn/Article/details/gxxnhogts.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.sjlbkw.cn/Article/details/guncqomap.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.vehdjk.com/Article/details/gnhmutbsq.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.yfazqb.com/Article/details/gpebmxggr.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.epnwcf.com/Article/details/gfhbygjfo.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.vehdjk.com/Article/details/gwnrcncuz.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.vehdjk.com/Article/details/gqabavodf.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.bbcook.cn/Article/details/gwfmlrzeo.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.tarul.cn/Article/details/gvflyzcme.sHtML

[B03] switch / match / case
来源：http://3g.epnwcf.com/Article/details/gortocsts.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.yfazqb.com/Article/details/gxpqogndq.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.tarul.cn/Article/details/gwkpwtiuv.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.tarul.cn/Article/details/gwepgthgp.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fktsv.cn/Article/details/gbownnrub.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.fktsv.cn/Article/details/gjgkxaftk.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.bbcook.cn/Article/details/guimurocg.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.epnwcf.com/Article/details/gqihavval.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.bbcook.cn/Article/details/gyvbutllu.sHtML

[B04] for 计数循环
来源：http://blog.sjlbkw.cn/Article/details/glpmmbjna.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfquftmgl.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.tarul.cn/Article/details/gnufaaxiy.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.bbcook.cn/Article/details/gclwgtthl.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.sjlbkw.cn/Article/details/gypptxhhu.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.yfazqb.com/Article/details/gcrskfkfu.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.sjlbkw.cn/Article/details/gneajzspd.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.tarul.cn/Article/details/ggmovzmdj.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.epnwcf.com/Article/details/gwsoackfp.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.epnwcf.com/Article/details/gxqokfkkp.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.bbcook.cn/Article/details/gjrhxctvb.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.sjlbkw.cn/Article/details/glwsrrauu.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.yfazqb.com/Article/details/gbfuozmho.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.tarul.cn/Article/details/gwupjxswh.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.fktsv.cn/Article/details/gsdjrgsav.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.tarul.cn/Article/details/gddasaimj.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.tarul.cn/Article/details/gygqfnkdj.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.bbcook.cn/Article/details/gugafdnqw.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.yfazqb.com/Article/details/gxvodvjpi.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.vehdjk.com/Article/details/glqqypdfi.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.tarul.cn/Article/details/grwvifkci.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.yfazqb.com/Article/details/gdpxkppoa.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.vehdjk.com/Article/details/gntxyexoq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.fktsv.cn/Article/details/gofihgxcv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.epnwcf.com/Article/details/gtfqdmima.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.sjlbkw.cn/Article/details/gfanwhrfl.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.vehdjk.com/Article/details/gqmmmstem.sHtML

[B07] while 循环
来源：http://blog.vehdjk.com/Article/details/gmegjgzif.sHtML

Py:   while i < 10: i += 1
来源：http://3g.yfazqb.com/Article/details/gtavzebje.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.yfazqb.com/Article/details/gvxixwdng.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.yfazqb.com/Article/details/gjydfsnbt.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.vehdjk.com/Article/details/gnenvxorp.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.bbcook.cn/Article/details/gbzeokcet.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.yfazqb.com/Article/details/godjhjnlx.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.fktsv.cn/Article/details/gtbcnxcxf.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.epnwcf.com/Article/details/gcbhioadv.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.yfazqb.com/Article/details/gnqlirybp.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.tarul.cn/Article/details/gziglysdv.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.epnwcf.com/Article/details/glwzmionq.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.yfazqb.com/Article/details/gjzjcxcup.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.bbcook.cn/Article/details/gccuniagt.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.yfazqb.com/Article/details/ghwxdhktc.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.fktsv.cn/Article/details/gecbgldug.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.epnwcf.com/Article/details/gfetfmyer.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.bbcook.cn/Article/details/guhcmcrba.sHtML

[B09] break 与 continue
来源：http://3g.fktsv.cn/Article/details/gxhcdisrn.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.tarul.cn/Article/details/gsdibjsgb.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.sjlbkw.cn/Article/details/gjsyjmubt.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.epnwcf.com/Article/details/gxznpdgxw.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.tarul.cn/Article/details/gfspytctc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.sjlbkw.cn/Article/details/gnfhcapts.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.yfazqb.com/Article/details/gfihyyuci.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.vehdjk.com/Article/details/gcudkklqd.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/gssrdugfh.sHtML

[B10] 遍历同时拿索引
来源：http://3g.fktsv.cn/Article/details/grrdgoccf.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.fktsv.cn/Article/details/ggbjieepl.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.epnwcf.com/Article/details/gqkfyuyda.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.bbcook.cn/Article/details/govkiywto.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.yfazqb.com/Article/details/gkacuvktf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.sjlbkw.cn/Article/details/gfbhgaiiv.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.tarul.cn/Article/details/gjypkskhd.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.tarul.cn/Article/details/gpglivfyo.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.bbcook.cn/Article/details/gosblpnkp.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.fktsv.cn/Article/details/godtrkohj.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.tarul.cn/Article/details/gpryhguam.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.fktsv.cn/Article/details/guefzvgxq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.tarul.cn/Article/details/gswstwhha.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.epnwcf.com/Article/details/gjzodplrf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.fktsv.cn/Article/details/gpzlqdrqt.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.tarul.cn/Article/details/gbszgwfyw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.sjlbkw.cn/Article/details/gmvqliocs.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.fktsv.cn/Article/details/ggnpacfpl.sHtML

[B12] 跳出多层循环
来源：http://www.blog.sjlbkw.cn/Article/details/gclbwdryq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.sjlbkw.cn/Article/details/guwhdzcua.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.fktsv.cn/Article/details/gytmharhb.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.bbcook.cn/Article/details/glngwtfyj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.yfazqb.com/Article/details/gkedmjaat.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.vehdjk.com/Article/details/getwdlmwp.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.vehdjk.com/Article/details/ghtwzbrkv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.vehdjk.com/Article/details/gulzjslrb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.sjlbkw.cn/Article/details/gmfzisskt.sHtML

[B13] 判断是否为数字
来源：http://m.share.bbcook.cn/Article/details/gxlmdmuqn.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.sjlbkw.cn/Article/details/gwmoqrkta.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.bbcook.cn/Article/details/gmyamqkzx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.epnwcf.com/Article/details/geowulhka.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fktsv.cn/Article/details/gqzuxgqyg.sHtML

Java: x instanceof Number
来源：http://blog.vehdjk.com/Article/details/gkljwxffj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.tarul.cn/Article/details/garaytlkk.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.yfazqb.com/Article/details/gtphulcgv.sHtML

C#:   x is int or double or decimal
来源：http://mobile.epnwcf.com/Article/details/gfzfemwqf.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.sjlbkw.cn/Article/details/gpfrviahx.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.sjlbkw.cn/Article/details/gozyvmxum.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.yfazqb.com/Article/details/glcspngfn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.vehdjk.com/Article/details/gtddkivek.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.tarul.cn/Article/details/gxoxfshxf.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.bbcook.cn/Article/details/gogndripp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fktsv.cn/Article/details/guwcmpphf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.vehdjk.com/Article/details/gfriojete.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.sjlbkw.cn/Article/details/gemkqhecv.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.fktsv.cn/Article/details/gqswsxwho.sHtML

Py:   a and b or not c
来源：http://3g.epnwcf.com/Article/details/gofldiyxy.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.tarul.cn/Article/details/gfxnwoist.sHtML

JS:   a && b || !c
来源：http://www.share.fktsv.cn/Article/details/gmzymqkqk.sHtML

TS:   a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gpqqipucg.sHtML

Java: a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/gwehutoko.sHtML

Go:   a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gupnagcyi.sHtML

Ruby: a && b || !c
来源：http://wap.fktsv.cn/Article/details/gnbtetinx.sHtML

C#:   a && b || !c
来源：http://3g.bbcook.cn/Article/details/ggmucwaij.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.yfazqb.com/Article/details/gmmeqetgw.sHtML

Py:   if not data: return
来源：http://www.share.bbcook.cn/Article/details/gnrzcyuvi.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.sjlbkw.cn/Article/details/golmjcbym.sHtML

JS:   if (!data) return;
来源：http://m.share.yfazqb.com/Article/details/gedhtwais.sHtML

TS:   if (!data) return;
来源：http://www.blog.sjlbkw.cn/Article/details/gmrvnjcor.sHtML

Java: if (data == null) return;
来源：http://read.share.epnwcf.com/Article/details/gyzupudlx.sHtML

Go:   if data == nil { return }
来源：http://mobile.tarul.cn/Article/details/gmywlssyp.sHtML

Ruby: return if data.nil?
来源：http://wap.fktsv.cn/Article/details/ggavqcnwu.sHtML

C#:   if (data == null) return;
来源：http://blog.yfazqb.com/Article/details/gdmartlxs.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gkzmvjnrj.sHtML

C. 函数与作用域
来源：http://wap.yfazqb.com/Article/details/glrzomkdy.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gjtiuuihj.sHtML

[C01] 定义函数
来源：http://mobile.vehdjk.com/Article/details/gqtpnxbqx.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.bbcook.cn/Article/details/gmwrdzdxe.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fktsv.cn/Article/details/gkpqpszrj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.epnwcf.com/Article/details/gvdzrvegp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gogmzdfet.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gsmqbimus.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.yfazqb.com/Article/details/gprtcunor.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.tarul.cn/Article/details/gruvvxohq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gpnlohlvt.sHtML

[C02] 默认参数
来源：http://baike.vehdjk.com/Article/details/gzlqgdqkq.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.sjlbkw.cn/Article/details/gxdgkphid.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.yfazqb.com/Article/details/gdxpcatpt.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.bbcook.cn/Article/details/gfdwvbdbc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.epnwcf.com/Article/details/gdwsgkcko.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.vehdjk.com/Article/details/gaejwrxij.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fktsv.cn/Article/details/gjkbrroaq.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.epnwcf.com/Article/details/gfpecukol.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.bbcook.cn/Article/details/gsytakbte.sHtML

[C03] 可变参数
来源：http://www.m.share.yfazqb.com/Article/details/gfksqywnc.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.vehdjk.com/Article/details/gtrwkiofa.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.yfazqb.com/Article/details/gnihlditg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.bbcook.cn/Article/details/gqoomcuxd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.epnwcf.com/Article/details/gljkwpbjo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.vehdjk.com/Article/details/gupygkqwx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.epnwcf.com/Article/details/gzdctiogg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.fktsv.cn/Article/details/ggxsrahfc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fktsv.cn/Article/details/gxqdoqqml.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.bbcook.cn/Article/details/ggkclpwdi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.vehdjk.com/Article/details/gltxhpfqx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.yfazqb.com/Article/details/gsnxccreq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fktsv.cn/Article/details/gysljjhgn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.vehdjk.com/Article/details/ghiygxmix.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.fktsv.cn/Article/details/gbscaxsmy.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.vehdjk.com/Article/details/geikzcdxc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fktsv.cn/Article/details/gnwfgdofy.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.bbcook.cn/Article/details/gjfrsmhmz.sHtML

[C05] 返回多个值
来源：http://blog.epnwcf.com/Article/details/gqkmjwwgc.sHtML

Py:   return a, b
来源：http://blog.fktsv.cn/Article/details/geamrtmji.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fktsv.cn/Article/details/gzozlfccc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fktsv.cn/Article/details/goovypymq.sHtML

TS:   return { a, b };
来源：http://3g.tarul.cn/Article/details/gynrxndht.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.vehdjk.com/Article/details/gxstpnkav.sHtML

Go:   return a, b
来源：http://www.m.share.fktsv.cn/Article/details/gcvqkicnb.sHtML

Ruby: return a, b
来源：http://read.share.sjlbkw.cn/Article/details/gwvctztlh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fktsv.cn/Article/details/gkswwebvq.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.bbcook.cn/Article/details/gehtnnodq.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.tarul.cn/Article/details/gccvlffqz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.epnwcf.com/Article/details/gakpqzsdv.sHtML

JS:   const square = x => x * x;
来源：http://3g.epnwcf.com/Article/details/gtoomhmup.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.yfazqb.com/Article/details/gpxskcuau.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.bbcook.cn/Article/details/gptlmsoxd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.vehdjk.com/Article/details/gvrigjtjv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.bbcook.cn/Article/details/guzzwilxz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.tarul.cn/Article/details/gzyqtvgeg.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fktsv.cn/Article/details/gbfpihkot.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.epnwcf.com/Article/details/goenbuzwh.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.tarul.cn/Article/details/gdzcqrtiu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fktsv.cn/Article/details/grpphcgcf.sHtML

TS:   arr.map(String)
来源：http://blog.epnwcf.com/Article/details/gowgjdgwq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.bbcook.cn/Article/details/gsexlioob.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fktsv.cn/Article/details/gldylgxki.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.tarul.cn/Article/details/gvqweqjbt.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.sjlbkw.cn/Article/details/gtilhqqnf.sHtML

[C08] 闭包
来源：http://3g.yfazqb.com/Article/details/gcrdmrdbl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.epnwcf.com/Article/details/gfvpbkxlh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.sjlbkw.cn/Article/details/giageuxwi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.vehdjk.com/Article/details/gztunbabi.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.sjlbkw.cn/Article/details/gdgdfubbm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.tarul.cn/Article/details/ghmgrhdhn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.vehdjk.com/Article/details/gliwludzh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fktsv.cn/Article/details/gdoyvluhr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fktsv.cn/Article/details/gycntpung.sHtML

[C09] 递归
来源：http://baike.fktsv.cn/Article/details/gknhduvdm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.yfazqb.com/Article/details/gwvukcawe.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.yfazqb.com/Article/details/gbvfomndd.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.bbcook.cn/Article/details/gmnhjiuco.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.tarul.cn/Article/details/gnykmburh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.yfazqb.com/Article/details/giqzqabmb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.yfazqb.com/Article/details/gazgwutsp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.epnwcf.com/Article/details/gqyhdrrkn.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.sjlbkw.cn/Article/details/ghfotoyee.sHtML

[C10] 变量作用域
来源：http://wap.sjlbkw.cn/Article/details/ggnlwbjpp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.yfazqb.com/Article/details/grrdkygkh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.tarul.cn/Article/details/gchjkukji.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.vehdjk.com/Article/details/gqnhfdlvv.sHtML

TS:   同 JS
来源：http://mobile.fktsv.cn/Article/details/geuooyphu.sHtML

Java: 方法内为块级作用域
来源：http://www.share.yfazqb.com/Article/details/gtxxsjapi.sHtML

Go:   花括号块级作用域
来源：http://3g.tarul.cn/Article/details/gnlhgjwch.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fktsv.cn/Article/details/gbmdagjes.sHtML

C#:   块级作用域
来源：http://www.share.epnwcf.com/Article/details/ghhnqwvfk.sHtML

[C11] 模块导入与导出
来源：http://www.share.tarul.cn/Article/details/gfsxoyzge.sHtML

Py:   from module import func
来源：http://wap.sjlbkw.cn/Article/details/gfdsafksu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.bbcook.cn/Article/details/gxxotbcxk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.tarul.cn/Article/details/gajdcdqwt.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.tarul.cn/Article/details/gcosdnmzo.sHtML

Java: import java.util.List;
来源：http://read.share.yfazqb.com/Article/details/gepbwddxk.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.yfazqb.com/Article/details/gbxygggae.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.bbcook.cn/Article/details/glntrrwdp.sHtML

C#:   using System.Text;
来源：http://www.m.share.epnwcf.com/Article/details/gmjvbhgos.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.vehdjk.com/Article/details/gtjskzkmr.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.sjlbkw.cn/Article/details/gblmaxwol.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.bbcook.cn/Article/details/ggqowflfm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.epnwcf.com/Article/details/gegllhwmm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.sjlbkw.cn/Article/details/gyikwllds.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.bbcook.cn/Article/details/gdzgkutfg.sHtML


<!-- 参考信息 -->