代发 wailian999

[A22] 获取字符串长度
来源：http://www.share.yfazqb.com/Article/details/gurpijqbw.sHtML

Py:   len(s)
来源：http://wap.fktsv.cn/Article/details/gmrrypfkn.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.epnwcf.com/Article/details/gfseeuxmc.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.bbcook.cn/Article/details/gvugawnja.sHtML

TS:   s.length
来源：http://www.share.fktsv.cn/Article/details/gujpkgiuj.sHtML

Java: s.length()
来源：http://www.blog.fktsv.cn/Article/details/girwjsdsr.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.yfazqb.com/Article/details/gmkkalncm.sHtML

Ruby: s.length
来源：http://3g.tarul.cn/Article/details/gdsjvjpme.sHtML

C#:   s.Length
来源：http://m.share.yfazqb.com/Article/details/goskrafgk.sHtML

[A23] 大小写转换
来源：http://www.blog.yfazqb.com/Article/details/gfzonudqf.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.epnwcf.com/Article/details/gooturorl.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.vehdjk.com/Article/details/grswnyxow.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.tarul.cn/Article/details/gydpumuqm.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.tarul.cn/Article/details/gieaxzisy.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.sjlbkw.cn/Article/details/govqrtpsi.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.yfazqb.com/Article/details/giotxcdrh.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.fktsv.cn/Article/details/glzgrhuns.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.vehdjk.com/Article/details/gjortmxds.sHtML

[A24] 去除首尾空白
来源：http://read.share.fktsv.cn/Article/details/gwufzyprf.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.epnwcf.com/Article/details/gchinhesg.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.epnwcf.com/Article/details/ggpqdekyt.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.fktsv.cn/Article/details/gehlvmcpn.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.fktsv.cn/Article/details/gwssvzvuh.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.yfazqb.com/Article/details/grxclsjfp.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.tarul.cn/Article/details/gurjeyjhi.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.epnwcf.com/Article/details/gliyoospg.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.bbcook.cn/Article/details/gktwwcsnu.sHtML

[A25] 字符串比较
来源：http://blog.bbcook.cn/Article/details/grwzyghuw.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.bbcook.cn/Article/details/gvzcwqqtw.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.sjlbkw.cn/Article/details/gjcqkfvle.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.bbcook.cn/Article/details/ghcftcawi.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.bbcook.cn/Article/details/gjqhycmhz.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.bbcook.cn/Article/details/grzdssiue.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.tarul.cn/Article/details/gjihighqt.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.tarul.cn/Article/details/gjcrgxnaw.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.epnwcf.com/Article/details/glcvfjygw.sHtML

[A26] 类型转换总览
来源：http://baike.bbcook.cn/Article/details/geolcfsyc.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.yfazqb.com/Article/details/gbphpfchh.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.bbcook.cn/Article/details/gtzqjjtvu.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.fktsv.cn/Article/details/ggcwllius.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.sjlbkw.cn/Article/details/gcshphala.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.fktsv.cn/Article/details/glvzdzdhd.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.fktsv.cn/Article/details/gzqlxnjmi.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.fktsv.cn/Article/details/gmvrgmprr.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.tarul.cn/Article/details/gsoujtkfx.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gclrjuuro.sHtML

B. 流程控制
来源：http://mobile.bbcook.cn/Article/details/gerzfddol.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/grtglkkfu.sHtML

[B01] 条件判断 if / else
来源：http://www.share.tarul.cn/Article/details/gwnvvnsmn.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.tarul.cn/Article/details/gnhwhobno.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.sjlbkw.cn/Article/details/gvouepobf.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.bbcook.cn/Article/details/gmokvvchz.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fktsv.cn/Article/details/gawgpdpmu.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.vehdjk.com/Article/details/gzlshnfrm.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.fktsv.cn/Article/details/goyqxbpmx.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.epnwcf.com/Article/details/gwjfsorzh.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.sjlbkw.cn/Article/details/gndqsoxnf.sHtML

[B02] 多分支 else if / elif
来源：http://blog.tarul.cn/Article/details/gpggikqae.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.yfazqb.com/Article/details/gnowacsas.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.tarul.cn/Article/details/gtqdshadg.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.yfazqb.com/Article/details/grcyvgkvg.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.bbcook.cn/Article/details/gmocqodrs.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.tarul.cn/Article/details/ghwcajuip.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.bbcook.cn/Article/details/gdfqxsvle.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.fktsv.cn/Article/details/gyggrrbsq.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fktsv.cn/Article/details/gpllcnctz.sHtML

[B03] switch / match / case
来源：http://3g.fktsv.cn/Article/details/glitbxceg.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.sjlbkw.cn/Article/details/ggelbpfnh.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.vehdjk.com/Article/details/glsvrantb.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.tarul.cn/Article/details/gaisscvsg.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fktsv.cn/Article/details/ghxjdsxbt.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.fktsv.cn/Article/details/gekfloanw.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.yfazqb.com/Article/details/goqginati.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.tarul.cn/Article/details/gtfotulhn.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.bbcook.cn/Article/details/gcwonvtoe.sHtML

[B04] for 计数循环
来源：http://blog.yfazqb.com/Article/details/grzxoazjj.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.vehdjk.com/Article/details/gwvskgsvx.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.tarul.cn/Article/details/gnojzjjhk.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.tarul.cn/Article/details/goxpfntyc.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.bbcook.cn/Article/details/gqivgonyr.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.bbcook.cn/Article/details/gisornpma.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.sjlbkw.cn/Article/details/gppckpkpq.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.sjlbkw.cn/Article/details/gvtxkqdoy.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.sjlbkw.cn/Article/details/gyqbgbwya.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.epnwcf.com/Article/details/groyfwdvw.sHtML

Py:   for item in arr: print(item)
来源：http://wap.yfazqb.com/Article/details/gwmqiqysq.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.yfazqb.com/Article/details/ggunnvqpx.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.tarul.cn/Article/details/gbzfqlrko.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.vehdjk.com/Article/details/gvqfzoaeu.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.epnwcf.com/Article/details/gkywyarbp.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.tarul.cn/Article/details/gholzovbn.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.vehdjk.com/Article/details/gwhdkspsk.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.bbcook.cn/Article/details/gpwbihkrn.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.sjlbkw.cn/Article/details/gijboolfa.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.bbcook.cn/Article/details/gszuberqi.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.bbcook.cn/Article/details/gmzunxcat.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fktsv.cn/Article/details/goojnxbwt.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.bbcook.cn/Article/details/gbndaiaiq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.fktsv.cn/Article/details/goggovvop.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.epnwcf.com/Article/details/gmttpxdqh.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.fktsv.cn/Article/details/gvnxfrsvl.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.fktsv.cn/Article/details/gbyzftkfi.sHtML

[B07] while 循环
来源：http://www.blog.bbcook.cn/Article/details/ggwvvcnfk.sHtML

Py:   while i < 10: i += 1
来源：http://baike.epnwcf.com/Article/details/glzousnqy.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.bbcook.cn/Article/details/guboewznt.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.bbcook.cn/Article/details/ggfdwlnvo.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.tarul.cn/Article/details/gaqotntyk.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.bbcook.cn/Article/details/gqqrdtcuo.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.vehdjk.com/Article/details/gkpmkgzel.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.vehdjk.com/Article/details/glhertqmp.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.bbcook.cn/Article/details/gamzoymvh.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.fktsv.cn/Article/details/gddgfawkj.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.fktsv.cn/Article/details/gntehyiux.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.tarul.cn/Article/details/glgmpzsrm.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.fktsv.cn/Article/details/grfkpntzj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fktsv.cn/Article/details/gdntihten.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.sjlbkw.cn/Article/details/grtpnxsfn.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.fktsv.cn/Article/details/gjiedlfje.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.bbcook.cn/Article/details/gxxhmdbgp.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.yfazqb.com/Article/details/gxfupduzc.sHtML

[B09] break 与 continue
来源：http://mobile.tarul.cn/Article/details/gfrkzpjej.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.tarul.cn/Article/details/gqlahvewq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/gkdqpyjpr.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.bbcook.cn/Article/details/gejslfocm.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.vehdjk.com/Article/details/gbzjzzjej.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.tarul.cn/Article/details/gtyyfhivo.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.bbcook.cn/Article/details/gkdksfyvu.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.fktsv.cn/Article/details/gxunnbjqv.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.epnwcf.com/Article/details/ghqvxohsd.sHtML

[B10] 遍历同时拿索引
来源：http://wap.fktsv.cn/Article/details/gxlfssdxn.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.vehdjk.com/Article/details/glfcrwvrc.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.tarul.cn/Article/details/gueonkclp.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.sjlbkw.cn/Article/details/gcyseatky.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.bbcook.cn/Article/details/gqbbxipoc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.vehdjk.com/Article/details/gyjmcilav.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.tarul.cn/Article/details/gvcotuaag.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.bbcook.cn/Article/details/gvnyisiwb.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.tarul.cn/Article/details/gaynslfju.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.fktsv.cn/Article/details/gwrtyluvg.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.vehdjk.com/Article/details/gwhuglequ.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.vehdjk.com/Article/details/gbjnqpwqr.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fktsv.cn/Article/details/gxyaucakp.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.vehdjk.com/Article/details/gvsifaawu.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.tarul.cn/Article/details/ghjxqxnvz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.tarul.cn/Article/details/gysktspkw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.epnwcf.com/Article/details/gxcuzfdfg.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.bbcook.cn/Article/details/gvismwwkk.sHtML

[B12] 跳出多层循环
来源：http://blog.fktsv.cn/Article/details/gguksbknq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.fktsv.cn/Article/details/gntlopfnf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.sjlbkw.cn/Article/details/gkvccbofj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.vehdjk.com/Article/details/guvodaswg.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.yfazqb.com/Article/details/ghhrvezdw.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.bbcook.cn/Article/details/gbrararod.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.yfazqb.com/Article/details/gvgyawicv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.sjlbkw.cn/Article/details/gqcjmyeru.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.vehdjk.com/Article/details/gyaiddqbp.sHtML

[B13] 判断是否为数字
来源：http://www.share.yfazqb.com/Article/details/gctyvukwk.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fktsv.cn/Article/details/gsfmyhnhe.sHtML

PHP:  is_numeric($x)
来源：http://m.share.vehdjk.com/Article/details/gnydkohyx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.sjlbkw.cn/Article/details/gfdbdemhi.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.bbcook.cn/Article/details/gbaqnoecm.sHtML

Java: x instanceof Number
来源：http://mobile.sjlbkw.cn/Article/details/gdstcqofm.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.vehdjk.com/Article/details/gcmbrrmbe.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyobrcuwx.sHtML

C#:   x is int or double or decimal
来源：http://3g.bbcook.cn/Article/details/gffqejjdy.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.yfazqb.com/Article/details/gahjxwodd.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fktsv.cn/Article/details/gsxqyywce.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.bbcook.cn/Article/details/gspaefoed.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.vehdjk.com/Article/details/gthpqspdz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.epnwcf.com/Article/details/gppksuntx.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.fktsv.cn/Article/details/guztzrzxr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.bbcook.cn/Article/details/gnezhruab.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.bbcook.cn/Article/details/gdionhzla.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.tarul.cn/Article/details/gvaybfzpy.sHtML

[B15] 布尔运算与取反
来源：http://mobile.vehdjk.com/Article/details/gkklredwm.sHtML

Py:   a and b or not c
来源：http://www.m.share.vehdjk.com/Article/details/gywzfdcfn.sHtML

PHP:  $a && $b || !$c
来源：http://baike.tarul.cn/Article/details/gmgqvcphw.sHtML

JS:   a && b || !c
来源：http://blog.yfazqb.com/Article/details/gzlllefdq.sHtML

TS:   a && b || !c
来源：http://blog.sjlbkw.cn/Article/details/gohmvxkgt.sHtML

Java: a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gtotuaksk.sHtML

Go:   a && b || !c
来源：http://m.share.yfazqb.com/Article/details/gsthdquab.sHtML

Ruby: a && b || !c
来源：http://baike.tarul.cn/Article/details/gtqovtkfh.sHtML

C#:   a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/gnbnzrgtp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.epnwcf.com/Article/details/goetluhuk.sHtML

Py:   if not data: return
来源：http://blog.epnwcf.com/Article/details/gkyhsnagc.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fktsv.cn/Article/details/gksyjccse.sHtML

JS:   if (!data) return;
来源：http://m.share.yfazqb.com/Article/details/gfnbrmvoo.sHtML

TS:   if (!data) return;
来源：http://www.blog.yfazqb.com/Article/details/gbipqvvhu.sHtML

Java: if (data == null) return;
来源：http://m.share.bbcook.cn/Article/details/gmoeipjza.sHtML

Go:   if data == nil { return }
来源：http://www.blog.sjlbkw.cn/Article/details/gapefkgqc.sHtML

Ruby: return if data.nil?
来源：http://wap.tarul.cn/Article/details/gpujnrstj.sHtML

C#:   if (data == null) return;
来源：http://read.share.sjlbkw.cn/Article/details/gmiqhqmcg.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gvxbhcsdd.sHtML

C. 函数与作用域
来源：http://wap.bbcook.cn/Article/details/gnvtvccus.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gylyzxzed.sHtML

[C01] 定义函数
来源：http://www.share.epnwcf.com/Article/details/gluhyprso.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.tarul.cn/Article/details/gjbbotxjm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.sjlbkw.cn/Article/details/gxyorlcqq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gyyqdmzrp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/gcezecloe.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/ghbmbxoth.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.tarul.cn/Article/details/ghjtrrwak.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.epnwcf.com/Article/details/gjmhzuwmx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.epnwcf.com/Article/details/gptdojvnj.sHtML

[C02] 默认参数
来源：http://www.blog.fktsv.cn/Article/details/gxltqvdwd.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.bbcook.cn/Article/details/gnfhohlub.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.bbcook.cn/Article/details/gehvsdiie.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.tarul.cn/Article/details/gpdrydtjh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.yfazqb.com/Article/details/gghsvjujn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.yfazqb.com/Article/details/getqmsxok.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.vehdjk.com/Article/details/gnzxsvnuy.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.bbcook.cn/Article/details/gxyryaken.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.epnwcf.com/Article/details/gdqpwwtsy.sHtML

[C03] 可变参数
来源：http://wap.vehdjk.com/Article/details/gidldgqjk.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fktsv.cn/Article/details/gbudugydb.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.epnwcf.com/Article/details/gydcdbnne.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.epnwcf.com/Article/details/gwjubuiwp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.epnwcf.com/Article/details/gidpkmqph.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.vehdjk.com/Article/details/glzsbgvkx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.fktsv.cn/Article/details/gnwzdozxl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.fktsv.cn/Article/details/ggrldzzsf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.tarul.cn/Article/details/ghjkhkjaa.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.bbcook.cn/Article/details/gagpegoyo.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.yfazqb.com/Article/details/gjadessan.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.epnwcf.com/Article/details/gylbldnue.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.bbcook.cn/Article/details/gjwhmwunw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.bbcook.cn/Article/details/gvzmplblg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.tarul.cn/Article/details/gkcqfyhvl.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.fktsv.cn/Article/details/gsfljpwih.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.tarul.cn/Article/details/gmgngndkt.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fktsv.cn/Article/details/gizukopvf.sHtML

[C05] 返回多个值
来源：http://mobile.tarul.cn/Article/details/gmoogewru.sHtML

Py:   return a, b
来源：http://www.m.share.vehdjk.com/Article/details/gqrymlxtv.sHtML

PHP:  return [$a, $b];
来源：http://wap.sjlbkw.cn/Article/details/gublmyyfb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fktsv.cn/Article/details/gqnfdtbkh.sHtML

TS:   return { a, b };
来源：http://mobile.bbcook.cn/Article/details/gpalyndzs.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fktsv.cn/Article/details/gskpflgdo.sHtML

Go:   return a, b
来源：http://wap.bbcook.cn/Article/details/glpzbxlep.sHtML

Ruby: return a, b
来源：http://read.share.vehdjk.com/Article/details/gurjpbtbe.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.vehdjk.com/Article/details/gqfmkrovr.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fktsv.cn/Article/details/gxwdlqnkq.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.epnwcf.com/Article/details/geurxhlak.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.epnwcf.com/Article/details/gkvhlkixk.sHtML

JS:   const square = x => x * x;
来源：http://blog.bbcook.cn/Article/details/gdpwlagqz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.tarul.cn/Article/details/goonpnonq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.epnwcf.com/Article/details/gyomriqsk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.yfazqb.com/Article/details/gwwemwxka.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.fktsv.cn/Article/details/gktepekoo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.bbcook.cn/Article/details/gayhwavil.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.yfazqb.com/Article/details/gddmcxdcn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.epnwcf.com/Article/details/gsdzfrgyh.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.fktsv.cn/Article/details/glhklefag.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.epnwcf.com/Article/details/ghvzmhigg.sHtML

TS:   arr.map(String)
来源：http://baike.bbcook.cn/Article/details/girtkwspt.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.tarul.cn/Article/details/gvlupvjfr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.bbcook.cn/Article/details/gnvrkdepq.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.bbcook.cn/Article/details/gzokwfepz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.epnwcf.com/Article/details/gzpblfuct.sHtML

[C08] 闭包
来源：http://read.share.vehdjk.com/Article/details/gmlvssbvq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.bbcook.cn/Article/details/gvikuyxau.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.sjlbkw.cn/Article/details/gcehxmbwk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.sjlbkw.cn/Article/details/gkmnmndcv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjoaqpnoo.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.sjlbkw.cn/Article/details/goksoasvp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.epnwcf.com/Article/details/glyfdfscd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.tarul.cn/Article/details/gypizfcgc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.bbcook.cn/Article/details/glzmsmife.sHtML

[C09] 递归
来源：http://wap.vehdjk.com/Article/details/goqemmcil.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.tarul.cn/Article/details/gksxfvizy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.tarul.cn/Article/details/gtbxeaqou.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.epnwcf.com/Article/details/gfljookax.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.yfazqb.com/Article/details/gwpgvfnuo.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.tarul.cn/Article/details/gfjnwsxkf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.epnwcf.com/Article/details/gmotilzxa.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.vehdjk.com/Article/details/gihewdvzh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.epnwcf.com/Article/details/ggqabmqqo.sHtML

[C10] 变量作用域
来源：http://m.share.epnwcf.com/Article/details/gatamkqxw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.yfazqb.com/Article/details/gfooqyenx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.sjlbkw.cn/Article/details/gztxghcot.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.epnwcf.com/Article/details/gpsrsnwnm.sHtML

TS:   同 JS
来源：http://wap.vehdjk.com/Article/details/gtzvbmfsy.sHtML

Java: 方法内为块级作用域
来源：http://wap.vehdjk.com/Article/details/gacwozobp.sHtML

Go:   花括号块级作用域
来源：http://baike.sjlbkw.cn/Article/details/gjlffrbtt.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.yfazqb.com/Article/details/gcjrwnepq.sHtML

C#:   块级作用域
来源：http://baike.yfazqb.com/Article/details/gcxzwrfpq.sHtML

[C11] 模块导入与导出
来源：http://read.share.fktsv.cn/Article/details/guyjpafdw.sHtML

Py:   from module import func
来源：http://www.share.vehdjk.com/Article/details/gbbdoyolp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.bbcook.cn/Article/details/gguueagae.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.epnwcf.com/Article/details/grtpnmdyq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fktsv.cn/Article/details/gnsvbcwas.sHtML

Java: import java.util.List;
来源：http://www.share.bbcook.cn/Article/details/gqxczikdf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.yfazqb.com/Article/details/gthajtxrs.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.epnwcf.com/Article/details/gcevolkht.sHtML

C#:   using System.Text;
来源：http://read.share.fktsv.cn/Article/details/gvjlaxltf.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.epnwcf.com/Article/details/gpcjptvel.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.yfazqb.com/Article/details/gkhjyswom.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.bbcook.cn/Article/details/glmwywoxf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.yfazqb.com/Article/details/gmxzrzmcm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.yfazqb.com/Article/details/gyzdahzgi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.sjlbkw.cn/Article/details/ggjmmahmo.sHtML


<!-- 参考信息 -->