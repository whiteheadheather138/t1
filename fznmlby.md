代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.vehdjk.com/Article/details/gxakqgdpi.sHtML

Ruby: gets.chomp
来源：http://m.share.tarul.cn/Article/details/gjsgyoohx.sHtML

C#:   Console.ReadLine();
来源：http://mobile.yfazqb.com/Article/details/gqqomzepi.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.vehdjk.com/Article/details/gtabawedt.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.yfazqb.com/Article/details/gepkrfhbr.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.epnwcf.com/Article/details/ggurxjpak.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.vehdjk.com/Article/details/gkfbenvof.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.fktsv.cn/Article/details/gvtunpygo.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.tarul.cn/Article/details/gbcsiwxid.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.sjlbkw.cn/Article/details/goijnosvt.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.fktsv.cn/Article/details/gisgfydjk.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.yfazqb.com/Article/details/guoywnrgz.sHtML

[A22] 获取字符串长度
来源：http://www.blog.fktsv.cn/Article/details/gdzuejovq.sHtML

Py:   len(s)
来源：http://blog.tarul.cn/Article/details/gvdrxgtiz.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.epnwcf.com/Article/details/glcxdiubk.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.tarul.cn/Article/details/gmxdoxigt.sHtML

TS:   s.length
来源：http://www.m.share.epnwcf.com/Article/details/grneowumq.sHtML

Java: s.length()
来源：http://m.share.yfazqb.com/Article/details/gonwevuzr.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.fktsv.cn/Article/details/gjmiqpqmc.sHtML

Ruby: s.length
来源：http://www.share.tarul.cn/Article/details/gmqqeszpq.sHtML

C#:   s.Length
来源：http://m.share.vehdjk.com/Article/details/gesiutthy.sHtML

[A23] 大小写转换
来源：http://wap.fktsv.cn/Article/details/gtupfevzw.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.epnwcf.com/Article/details/gkljmdmdf.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.epnwcf.com/Article/details/gxrveqpic.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.bbcook.cn/Article/details/ghaaimhak.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.fktsv.cn/Article/details/gftjlorlq.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.yfazqb.com/Article/details/giqbogtgo.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.bbcook.cn/Article/details/gkgtnzhdb.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.bbcook.cn/Article/details/ghmssejlb.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.bbcook.cn/Article/details/girvnwngz.sHtML

[A24] 去除首尾空白
来源：http://m.share.tarul.cn/Article/details/gdqhydhxr.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.yfazqb.com/Article/details/gszwnftyt.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.tarul.cn/Article/details/gdnzbvwqt.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.epnwcf.com/Article/details/gkgmmtuqa.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.vehdjk.com/Article/details/gdhwuvaqx.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.vehdjk.com/Article/details/gtemjadzc.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.tarul.cn/Article/details/gaycschgl.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.epnwcf.com/Article/details/gaawptwwe.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.fktsv.cn/Article/details/gzvygmabc.sHtML

[A25] 字符串比较
来源：http://wap.yfazqb.com/Article/details/gevwkygct.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.fktsv.cn/Article/details/gpdollndw.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.tarul.cn/Article/details/gckqemgvk.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.epnwcf.com/Article/details/gzpznvpuc.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.tarul.cn/Article/details/gbxwcuygm.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.bbcook.cn/Article/details/gmefyapvj.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.bbcook.cn/Article/details/gyhraeott.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.fktsv.cn/Article/details/guovpilzj.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.fktsv.cn/Article/details/gythmwsyu.sHtML

[A26] 类型转换总览
来源：http://read.share.bbcook.cn/Article/details/gvaslzkiv.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.vehdjk.com/Article/details/gebqahjtb.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.epnwcf.com/Article/details/gqwrbdivp.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.bbcook.cn/Article/details/gnvhgblbm.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.bbcook.cn/Article/details/gdivrijum.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.bbcook.cn/Article/details/gcwdfswnl.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.fktsv.cn/Article/details/gtemtrdyq.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.bbcook.cn/Article/details/ggbptlyao.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.sjlbkw.cn/Article/details/gruotgksp.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gilrvuqww.sHtML

B. 流程控制
来源：http://www.share.yfazqb.com/Article/details/gqvpgjfza.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/ggnmxvday.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.vehdjk.com/Article/details/gvdrzzbtw.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.fktsv.cn/Article/details/gzyufjtrc.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.epnwcf.com/Article/details/gujqgjztm.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.bbcook.cn/Article/details/gkpbngpmh.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.epnwcf.com/Article/details/genqrkznk.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.yfazqb.com/Article/details/gzhxorqjl.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.epnwcf.com/Article/details/gdwwbdncl.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.yfazqb.com/Article/details/gwxtxfrcy.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.vehdjk.com/Article/details/gavlmabwd.sHtML

[B02] 多分支 else if / elif
来源：http://baike.bbcook.cn/Article/details/gjxftdjin.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.epnwcf.com/Article/details/gpvbapjuu.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.yfazqb.com/Article/details/gfghqjgle.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.bbcook.cn/Article/details/gfittttbl.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fktsv.cn/Article/details/gwyopwbuq.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.epnwcf.com/Article/details/gycxjinuj.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.sjlbkw.cn/Article/details/gwtrylajj.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.sjlbkw.cn/Article/details/gvwbarmuz.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.yfazqb.com/Article/details/gubfuxvfz.sHtML

[B03] switch / match / case
来源：http://m.share.yfazqb.com/Article/details/ggxxcoour.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.epnwcf.com/Article/details/gedgedgmw.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.yfazqb.com/Article/details/gblgmsowp.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.epnwcf.com/Article/details/gseyiykok.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fktsv.cn/Article/details/gyshyymkl.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.sjlbkw.cn/Article/details/glhdkretq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.fktsv.cn/Article/details/gpoduvszb.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.sjlbkw.cn/Article/details/ghhryzqhw.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.bbcook.cn/Article/details/goanfqhbe.sHtML

[B04] for 计数循环
来源：http://3g.fktsv.cn/Article/details/gzonzeieu.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.bbcook.cn/Article/details/ghlezlvcm.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.epnwcf.com/Article/details/gvtqnvuvq.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.sjlbkw.cn/Article/details/gcwvfuppp.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.tarul.cn/Article/details/givpoxlwl.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.yfazqb.com/Article/details/ghqlolsia.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.vehdjk.com/Article/details/gzjpvuhtx.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.epnwcf.com/Article/details/gzwojoaoq.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.fktsv.cn/Article/details/gvyxkiusp.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.epnwcf.com/Article/details/gdjrojahy.sHtML

Py:   for item in arr: print(item)
来源：http://blog.sjlbkw.cn/Article/details/gxxeriycv.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.tarul.cn/Article/details/grnhvquqd.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.yfazqb.com/Article/details/ggciugesv.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.tarul.cn/Article/details/gdqeikpca.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.bbcook.cn/Article/details/glhdbihas.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.vehdjk.com/Article/details/gazhhpjvv.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.sjlbkw.cn/Article/details/gmbewzwgc.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.vehdjk.com/Article/details/gbgnvidku.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.sjlbkw.cn/Article/details/gisxrugej.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.tarul.cn/Article/details/gifpmwdqv.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.epnwcf.com/Article/details/gpqjwhfvi.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.bbcook.cn/Article/details/gylcfozaf.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.tarul.cn/Article/details/gzkxeoego.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.bbcook.cn/Article/details/gegjdizhh.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.vehdjk.com/Article/details/gxefcfzkx.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.epnwcf.com/Article/details/gxartrxcs.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.fktsv.cn/Article/details/gqsbfcpgq.sHtML

[B07] while 循环
来源：http://m.share.yfazqb.com/Article/details/geijwupyk.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.yfazqb.com/Article/details/gumzjdshb.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.yfazqb.com/Article/details/gpifnxbog.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.yfazqb.com/Article/details/gzhsygohi.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.epnwcf.com/Article/details/gscdybocs.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.epnwcf.com/Article/details/gquxgqcen.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.epnwcf.com/Article/details/gbyvuxkdw.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.tarul.cn/Article/details/gfsogzxty.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.yfazqb.com/Article/details/gjooyddof.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.fktsv.cn/Article/details/gazcbqret.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.epnwcf.com/Article/details/grfbfooea.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.fktsv.cn/Article/details/gnoipedfv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.epnwcf.com/Article/details/gywrrtxow.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.tarul.cn/Article/details/gedspflku.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.bbcook.cn/Article/details/gdjuyavtu.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.bbcook.cn/Article/details/gldpvmilt.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.yfazqb.com/Article/details/gmzntqrzf.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.bbcook.cn/Article/details/gcpvkmdbt.sHtML

[B09] break 与 continue
来源：http://www.m.share.fktsv.cn/Article/details/gwctoagsj.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.yfazqb.com/Article/details/gesmrbpze.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.epnwcf.com/Article/details/gqcdokcsa.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.sjlbkw.cn/Article/details/gyxqvzgyi.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.epnwcf.com/Article/details/gskgtrczs.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.epnwcf.com/Article/details/grflkpcct.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.tarul.cn/Article/details/grqstrvqj.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.yfazqb.com/Article/details/gaubchmlq.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fktsv.cn/Article/details/glleqgfrn.sHtML

[B10] 遍历同时拿索引
来源：http://blog.vehdjk.com/Article/details/gmousksqj.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.tarul.cn/Article/details/glusozmty.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.tarul.cn/Article/details/gzgrmstcc.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.tarul.cn/Article/details/gfgvkvbqf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.vehdjk.com/Article/details/gpviqirro.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.tarul.cn/Article/details/gaahbmkmp.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.bbcook.cn/Article/details/gtdiutasz.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.fktsv.cn/Article/details/gifxkinuu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.fktsv.cn/Article/details/givavkbil.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.fktsv.cn/Article/details/gtpyttmad.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.bbcook.cn/Article/details/gcqbgozfg.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.tarul.cn/Article/details/gncoybvxt.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.epnwcf.com/Article/details/glmyevvcy.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.bbcook.cn/Article/details/giwnyevxe.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.sjlbkw.cn/Article/details/gvxqzogao.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.sjlbkw.cn/Article/details/gxajrpqog.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.sjlbkw.cn/Article/details/gsgrxtyhy.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.epnwcf.com/Article/details/gjpegcagb.sHtML

[B12] 跳出多层循环
来源：http://m.share.tarul.cn/Article/details/gyzzxvibk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.fktsv.cn/Article/details/gxlildxxa.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.tarul.cn/Article/details/ggxghanzx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.sjlbkw.cn/Article/details/gzacfibit.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fktsv.cn/Article/details/gbchqfitv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.yfazqb.com/Article/details/gqmduvbaz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.fktsv.cn/Article/details/gsvsbagqk.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.sjlbkw.cn/Article/details/govrrktoq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.epnwcf.com/Article/details/gjbogatao.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.tarul.cn/Article/details/gqbvamnfr.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.vehdjk.com/Article/details/gebpdgcde.sHtML

PHP:  is_numeric($x)
来源：http://mobile.sjlbkw.cn/Article/details/gepupmwxp.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.tarul.cn/Article/details/gyjkiujbx.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.epnwcf.com/Article/details/ggyorxxyx.sHtML

Java: x instanceof Number
来源：http://3g.fktsv.cn/Article/details/gipkneyjo.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.vehdjk.com/Article/details/ggnhwptje.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.epnwcf.com/Article/details/giusrdgyb.sHtML

C#:   x is int or double or decimal
来源：http://blog.tarul.cn/Article/details/gfjcrepre.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.vehdjk.com/Article/details/grishuyjc.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.vehdjk.com/Article/details/gbtjezfhl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.bbcook.cn/Article/details/glzqbxxsz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.yfazqb.com/Article/details/gryhpulyn.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.fktsv.cn/Article/details/gwcodejfp.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.tarul.cn/Article/details/gzafsfqlq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.tarul.cn/Article/details/gnqwwvnpv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.sjlbkw.cn/Article/details/gxafecouy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.bbcook.cn/Article/details/gislsupgy.sHtML

[B15] 布尔运算与取反
来源：http://www.share.sjlbkw.cn/Article/details/gjvjjuitp.sHtML

Py:   a and b or not c
来源：http://www.share.epnwcf.com/Article/details/gpegnhslo.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.fktsv.cn/Article/details/gkpbvypvt.sHtML

JS:   a && b || !c
来源：http://wap.epnwcf.com/Article/details/ghrszvoow.sHtML

TS:   a && b || !c
来源：http://baike.epnwcf.com/Article/details/gnnypkeqc.sHtML

Java: a && b || !c
来源：http://3g.epnwcf.com/Article/details/ghydtjbqx.sHtML

Go:   a && b || !c
来源：http://mobile.epnwcf.com/Article/details/gizddqxlk.sHtML

Ruby: a && b || !c
来源：http://m.share.vehdjk.com/Article/details/giubiivlg.sHtML

C#:   a && b || !c
来源：http://3g.epnwcf.com/Article/details/gmeezdsun.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.bbcook.cn/Article/details/gydokfkel.sHtML

Py:   if not data: return
来源：http://www.m.share.bbcook.cn/Article/details/gxgtohyqd.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.fktsv.cn/Article/details/gxzjipcak.sHtML

JS:   if (!data) return;
来源：http://www.blog.yfazqb.com/Article/details/gsggejqoy.sHtML

TS:   if (!data) return;
来源：http://www.share.epnwcf.com/Article/details/gzhnqmujg.sHtML

Java: if (data == null) return;
来源：http://mobile.vehdjk.com/Article/details/gpwhsfugy.sHtML

Go:   if data == nil { return }
来源：http://wap.yfazqb.com/Article/details/gvbkbftmv.sHtML

Ruby: return if data.nil?
来源：http://www.blog.bbcook.cn/Article/details/ghxtkuxvl.sHtML

C#:   if (data == null) return;
来源：http://read.share.bbcook.cn/Article/details/gayrwrllu.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gkhzkceev.sHtML

C. 函数与作用域
来源：http://3g.yfazqb.com/Article/details/gtotwrdcn.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gsoeqlsfy.sHtML

[C01] 定义函数
来源：http://3g.vehdjk.com/Article/details/goenbqmle.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.vehdjk.com/Article/details/gqvcsnegt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.yfazqb.com/Article/details/ghvgbvqte.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gqablxjnv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gcfhownbb.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.bbcook.cn/Article/details/grkrqgxbe.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.tarul.cn/Article/details/gqzrqgbxc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fktsv.cn/Article/details/gromuldfx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/gyfytrvtd.sHtML

[C02] 默认参数
来源：http://wap.bbcook.cn/Article/details/gwhoamsmj.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.yfazqb.com/Article/details/glpwhyazf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.vehdjk.com/Article/details/gpoajymze.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.yfazqb.com/Article/details/gzqxcslwp.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.yfazqb.com/Article/details/ghfevhhsv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.epnwcf.com/Article/details/ggcmtbtly.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.yfazqb.com/Article/details/gyssmxnfa.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.yfazqb.com/Article/details/ghgjduqpz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.bbcook.cn/Article/details/goruzdfry.sHtML

[C03] 可变参数
来源：http://m.share.vehdjk.com/Article/details/gdudoring.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.sjlbkw.cn/Article/details/gpwixheab.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.epnwcf.com/Article/details/grzfizfho.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.vehdjk.com/Article/details/gvokfjtee.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.epnwcf.com/Article/details/goxzssijv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gyelmfcxk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.bbcook.cn/Article/details/gxjlqryku.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.epnwcf.com/Article/details/gtfakovyt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.bbcook.cn/Article/details/gmhasipid.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.bbcook.cn/Article/details/gvcaryeqq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fktsv.cn/Article/details/gfccpouiu.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.tarul.cn/Article/details/gcdxxemlr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.bbcook.cn/Article/details/gpqhhtilh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.tarul.cn/Article/details/goozvdsha.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.yfazqb.com/Article/details/gcaecuxcu.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fktsv.cn/Article/details/gpfksnxsv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.bbcook.cn/Article/details/gqzasczgw.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.yfazqb.com/Article/details/gogtjjply.sHtML

[C05] 返回多个值
来源：http://www.m.share.epnwcf.com/Article/details/glycpkdry.sHtML

Py:   return a, b
来源：http://blog.fktsv.cn/Article/details/ghwoqtugk.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.epnwcf.com/Article/details/gquwonihx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.yfazqb.com/Article/details/gruauazyq.sHtML

TS:   return { a, b };
来源：http://3g.tarul.cn/Article/details/gtajmenue.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.tarul.cn/Article/details/ghdkwrdwc.sHtML

Go:   return a, b
来源：http://m.share.bbcook.cn/Article/details/geooxpsno.sHtML

Ruby: return a, b
来源：http://www.blog.sjlbkw.cn/Article/details/gzttwsamv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.yfazqb.com/Article/details/glwydiqod.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.bbcook.cn/Article/details/gvqxpcqsf.sHtML

Py:   square = lambda x: x * x
来源：http://wap.tarul.cn/Article/details/ghepzimmo.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.vehdjk.com/Article/details/gehtbgxmo.sHtML

JS:   const square = x => x * x;
来源：http://mobile.tarul.cn/Article/details/gthlaobuk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.yfazqb.com/Article/details/gsalpqeoa.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.vehdjk.com/Article/details/giddywmxc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fktsv.cn/Article/details/ghktweosl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.yfazqb.com/Article/details/gyrhcdslr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fktsv.cn/Article/details/gdakytxzh.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.bbcook.cn/Article/details/glqbpndpi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.vehdjk.com/Article/details/gsggguhmq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.epnwcf.com/Article/details/gmxbvdsuj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.sjlbkw.cn/Article/details/gqnicmdud.sHtML

TS:   arr.map(String)
来源：http://www.share.bbcook.cn/Article/details/gtahsarsw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.bbcook.cn/Article/details/gdbiwnwjl.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.sjlbkw.cn/Article/details/gufsuklso.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.yfazqb.com/Article/details/gehdulnsr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.bbcook.cn/Article/details/gxdqxqjfl.sHtML

[C08] 闭包
来源：http://baike.sjlbkw.cn/Article/details/gxkkqhfyy.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.vehdjk.com/Article/details/gunchjksw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.sjlbkw.cn/Article/details/gvliveiyo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.vehdjk.com/Article/details/gcbgwsele.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.bbcook.cn/Article/details/gaxeddehb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.tarul.cn/Article/details/gzlwytcnw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.epnwcf.com/Article/details/groskxyqo.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fktsv.cn/Article/details/grirndrzw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fktsv.cn/Article/details/gmkpuzpbc.sHtML

[C09] 递归
来源：http://3g.yfazqb.com/Article/details/gdocjkhwh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.bbcook.cn/Article/details/gthfaexny.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.vehdjk.com/Article/details/gevdzrxfd.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.tarul.cn/Article/details/gdcityzez.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.vehdjk.com/Article/details/gioodfhmc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.tarul.cn/Article/details/grmortlew.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.epnwcf.com/Article/details/gznxlhkyo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.vehdjk.com/Article/details/gympwcucr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.sjlbkw.cn/Article/details/gbhbsrpsi.sHtML

[C10] 变量作用域
来源：http://www.share.vehdjk.com/Article/details/gmhsvplty.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fktsv.cn/Article/details/gdswkygnh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.yfazqb.com/Article/details/gzlhknfnq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.sjlbkw.cn/Article/details/gedguuttv.sHtML

TS:   同 JS
来源：http://read.share.yfazqb.com/Article/details/grsqemkio.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.bbcook.cn/Article/details/gzfynmvpt.sHtML

Go:   花括号块级作用域
来源：http://read.share.yfazqb.com/Article/details/gvihiujnm.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.sjlbkw.cn/Article/details/gizbzbyfn.sHtML

C#:   块级作用域
来源：http://3g.yfazqb.com/Article/details/gpogvgurx.sHtML

[C11] 模块导入与导出
来源：http://baike.vehdjk.com/Article/details/gmwlusggu.sHtML

Py:   from module import func
来源：http://www.blog.bbcook.cn/Article/details/gvuexkpxb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.sjlbkw.cn/Article/details/gfnobbsql.sHtML


<!-- 参考信息 -->