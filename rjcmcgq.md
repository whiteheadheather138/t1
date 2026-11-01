代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.epnwcf.com/Article/details/gzbkgmohy.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.fktsv.cn/Article/details/gnbowyffe.sHtML

[A24] 去除首尾空白
来源：http://blog.tarul.cn/Article/details/ghokzqfzp.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.bbcook.cn/Article/details/glyxkwzzo.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.bbcook.cn/Article/details/gmngyhzuu.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.epnwcf.com/Article/details/gdilyalde.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.fktsv.cn/Article/details/gjjlqfyic.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.bbcook.cn/Article/details/gmjrxqola.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.tarul.cn/Article/details/gspormhof.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.bbcook.cn/Article/details/ghweszmdn.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.epnwcf.com/Article/details/gveldabao.sHtML

[A25] 字符串比较
来源：http://baike.fktsv.cn/Article/details/gzmtifawp.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.yfazqb.com/Article/details/gtctidugo.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.sjlbkw.cn/Article/details/gzhkbnnbh.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fktsv.cn/Article/details/gapvhwkgd.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fktsv.cn/Article/details/gjjoadgre.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.bbcook.cn/Article/details/gilonodne.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.bbcook.cn/Article/details/gsohlkcfd.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.yfazqb.com/Article/details/gnemljpan.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.bbcook.cn/Article/details/gtojikttt.sHtML

[A26] 类型转换总览
来源：http://www.m.share.sjlbkw.cn/Article/details/gswhhgglz.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.fktsv.cn/Article/details/gglfvhdmk.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.epnwcf.com/Article/details/govwgoxni.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.bbcook.cn/Article/details/gvbsbtazp.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.bbcook.cn/Article/details/grqzkatax.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.bbcook.cn/Article/details/gfruswwhb.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.bbcook.cn/Article/details/gghmmxsmo.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.tarul.cn/Article/details/grwyisnrv.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.bbcook.cn/Article/details/grtjdlcvl.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gyvumaqeg.sHtML

B. 流程控制
来源：http://www.blog.yfazqb.com/Article/details/gqxvwilrf.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gsjcthhkg.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.fktsv.cn/Article/details/gpkjjninv.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.vehdjk.com/Article/details/gkopfxfdt.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.epnwcf.com/Article/details/gbglxyqpb.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.tarul.cn/Article/details/gazyjwfon.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.vehdjk.com/Article/details/gcmmzezts.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.vehdjk.com/Article/details/gapgwocjh.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.epnwcf.com/Article/details/gqvsdruks.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.sjlbkw.cn/Article/details/ghdljsynf.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.vehdjk.com/Article/details/ggdavukit.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.epnwcf.com/Article/details/ghtqarzkl.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.vehdjk.com/Article/details/gkvijyfqu.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.tarul.cn/Article/details/gkrjbupln.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.vehdjk.com/Article/details/gtxkhzsln.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.sjlbkw.cn/Article/details/gjndogosa.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fktsv.cn/Article/details/gtlqrhtcb.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.yfazqb.com/Article/details/gokfvlixs.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.fktsv.cn/Article/details/gcjbpsdjw.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.epnwcf.com/Article/details/gtakpxiyp.sHtML

[B03] switch / match / case
来源：http://blog.tarul.cn/Article/details/gkqkzlone.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.tarul.cn/Article/details/gjuwcxgpc.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.epnwcf.com/Article/details/ghmdxhyic.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.vehdjk.com/Article/details/ggmsmxzaq.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.tarul.cn/Article/details/gbccnfrwk.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.epnwcf.com/Article/details/gbkzyryea.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.tarul.cn/Article/details/gouqmbrak.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.vehdjk.com/Article/details/ggkhbxaap.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.yfazqb.com/Article/details/gcjxtiqev.sHtML

[B04] for 计数循环
来源：http://blog.vehdjk.com/Article/details/gcdbfzacn.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.bbcook.cn/Article/details/gzivxmrhj.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.epnwcf.com/Article/details/gcvjwpfub.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.sjlbkw.cn/Article/details/gezuqhmsh.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fktsv.cn/Article/details/gpwacgdvu.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.bbcook.cn/Article/details/gldmhsqjk.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.tarul.cn/Article/details/grpbgmctj.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.fktsv.cn/Article/details/gsnpxrzvx.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.sjlbkw.cn/Article/details/guhrjowxu.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.sjlbkw.cn/Article/details/gmjfkskkd.sHtML

Py:   for item in arr: print(item)
来源：http://blog.bbcook.cn/Article/details/grftdmjwg.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.vehdjk.com/Article/details/givdbiggq.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.epnwcf.com/Article/details/gkmtvbsga.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.epnwcf.com/Article/details/griucimeu.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.bbcook.cn/Article/details/glrmdtyfp.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.tarul.cn/Article/details/gfxcbeljg.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.epnwcf.com/Article/details/gocugvraz.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.bbcook.cn/Article/details/gmxxhzldm.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.sjlbkw.cn/Article/details/gzbsaszuz.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.vehdjk.com/Article/details/gyenqntip.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.sjlbkw.cn/Article/details/gkuqycvxu.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.bbcook.cn/Article/details/glouccupq.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fktsv.cn/Article/details/ghplzjyea.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.epnwcf.com/Article/details/gckntfgqq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.epnwcf.com/Article/details/gievpblta.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.fktsv.cn/Article/details/galxkejvi.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.tarul.cn/Article/details/gjndckvbt.sHtML

[B07] while 循环
来源：http://blog.sjlbkw.cn/Article/details/gdxwyyjvw.sHtML

Py:   while i < 10: i += 1
来源：http://blog.vehdjk.com/Article/details/gwbtthuep.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.epnwcf.com/Article/details/glghmfdpj.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.bbcook.cn/Article/details/gsrkzjghl.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.yfazqb.com/Article/details/goddbhosm.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.epnwcf.com/Article/details/gxkfkcksi.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.fktsv.cn/Article/details/gaguswouq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.vehdjk.com/Article/details/gvxaxjjdk.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.vehdjk.com/Article/details/gbxblyalq.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.epnwcf.com/Article/details/gbbobmbsh.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.sjlbkw.cn/Article/details/gwouxrwkm.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.fktsv.cn/Article/details/giltnvcfr.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.vehdjk.com/Article/details/gdjgvojfr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fktsv.cn/Article/details/ggrghogdl.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.epnwcf.com/Article/details/ghirtksfr.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.tarul.cn/Article/details/gtuxhsrch.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.vehdjk.com/Article/details/gmtvksloe.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.tarul.cn/Article/details/gqhtvliec.sHtML

[B09] break 与 continue
来源：http://3g.vehdjk.com/Article/details/ggtpodflp.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.epnwcf.com/Article/details/ghiqudayx.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.epnwcf.com/Article/details/gdmrkikrh.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.epnwcf.com/Article/details/grjasvdyx.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.vehdjk.com/Article/details/gdvwpvsij.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.epnwcf.com/Article/details/growgvtqx.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.sjlbkw.cn/Article/details/gcvvlvgnr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.epnwcf.com/Article/details/gsssivgnl.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.vehdjk.com/Article/details/gjxjwbcas.sHtML

[B10] 遍历同时拿索引
来源：http://3g.sjlbkw.cn/Article/details/gwtbdcjrq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.fktsv.cn/Article/details/gwyzvdakf.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.bbcook.cn/Article/details/gxgncvftg.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.tarul.cn/Article/details/grsrdjblx.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.epnwcf.com/Article/details/grdbdwsog.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.bbcook.cn/Article/details/ghljssypb.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.tarul.cn/Article/details/goyuweijm.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.bbcook.cn/Article/details/gyqeoutog.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.vehdjk.com/Article/details/gvjxwxhfv.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.tarul.cn/Article/details/gctiochee.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.tarul.cn/Article/details/gfcyngcea.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.sjlbkw.cn/Article/details/gcopoxbbv.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.sjlbkw.cn/Article/details/gtncbuwok.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.tarul.cn/Article/details/gjifcdiac.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.yfazqb.com/Article/details/gnxezxasm.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.tarul.cn/Article/details/gajqnsncs.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.epnwcf.com/Article/details/gvjzzqjbg.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.tarul.cn/Article/details/gfzkcupct.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.tarul.cn/Article/details/gfacjjtmq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.tarul.cn/Article/details/gzpstqzcc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.vehdjk.com/Article/details/gjcdurvcu.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.sjlbkw.cn/Article/details/gdisbifxw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fktsv.cn/Article/details/ggafvoujt.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.sjlbkw.cn/Article/details/goictcehj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.tarul.cn/Article/details/gwyusdiat.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.sjlbkw.cn/Article/details/gfwcluxxa.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.epnwcf.com/Article/details/gcbaexsbh.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.vehdjk.com/Article/details/gouhivyyl.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.vehdjk.com/Article/details/gpzgumwlq.sHtML

PHP:  is_numeric($x)
来源：http://3g.fktsv.cn/Article/details/gcqzgftfd.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.epnwcf.com/Article/details/gkftjrsxm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.yfazqb.com/Article/details/gnlukufly.sHtML

Java: x instanceof Number
来源：http://www.m.share.vehdjk.com/Article/details/giiochreh.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.bbcook.cn/Article/details/grrkffmyl.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.vehdjk.com/Article/details/gghubnibe.sHtML

C#:   x is int or double or decimal
来源：http://3g.tarul.cn/Article/details/gddlzwrif.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.fktsv.cn/Article/details/gwkosxwyg.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.sjlbkw.cn/Article/details/grsfphhlz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.epnwcf.com/Article/details/gtdkgjfxp.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.fktsv.cn/Article/details/gujcsmbwi.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.sjlbkw.cn/Article/details/gzywcopii.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gicixdqyu.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.sjlbkw.cn/Article/details/gbezyvebd.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.yfazqb.com/Article/details/gkorgopgu.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gftgvnetk.sHtML

[B15] 布尔运算与取反
来源：http://m.share.epnwcf.com/Article/details/gyuojfabu.sHtML

Py:   a and b or not c
来源：http://www.m.share.vehdjk.com/Article/details/gtiffhtyn.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.bbcook.cn/Article/details/gmrrydogg.sHtML

JS:   a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/gtaezxmme.sHtML

TS:   a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gglikorma.sHtML

Java: a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/gkuxbvzbq.sHtML

Go:   a && b || !c
来源：http://blog.fktsv.cn/Article/details/gcneeoddg.sHtML

Ruby: a && b || !c
来源：http://www.share.yfazqb.com/Article/details/gtttoizwe.sHtML

C#:   a && b || !c
来源：http://baike.epnwcf.com/Article/details/gvmulonqd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.vehdjk.com/Article/details/gmlyqxptq.sHtML

Py:   if not data: return
来源：http://www.m.share.sjlbkw.cn/Article/details/gepsynklm.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.fktsv.cn/Article/details/gfbrulfwh.sHtML

JS:   if (!data) return;
来源：http://3g.tarul.cn/Article/details/gfylsmjjx.sHtML

TS:   if (!data) return;
来源：http://read.share.vehdjk.com/Article/details/gmefcythq.sHtML

Java: if (data == null) return;
来源：http://www.share.fktsv.cn/Article/details/gtltklhqz.sHtML

Go:   if data == nil { return }
来源：http://mobile.epnwcf.com/Article/details/gliviijtl.sHtML

Ruby: return if data.nil?
来源：http://baike.vehdjk.com/Article/details/gqbxnmeus.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.tarul.cn/Article/details/gkjiaatlk.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gblxnbyll.sHtML

C. 函数与作用域
来源：http://www.share.yfazqb.com/Article/details/gxzczauyd.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gbgjihmao.sHtML

[C01] 定义函数
来源：http://read.share.fktsv.cn/Article/details/glytgrjsc.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.sjlbkw.cn/Article/details/gutlmnjpj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.sjlbkw.cn/Article/details/gwvryymhi.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.tarul.cn/Article/details/gxvxdafiq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/grixnrlju.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/gjrfcohuf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.sjlbkw.cn/Article/details/glnavwclv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fktsv.cn/Article/details/gvozrcmlo.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.tarul.cn/Article/details/gxucwhyjd.sHtML

[C02] 默认参数
来源：http://www.share.vehdjk.com/Article/details/ghgpumguk.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.tarul.cn/Article/details/gmhaohjiq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.yfazqb.com/Article/details/gcpaslrle.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/ggkypfipe.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.epnwcf.com/Article/details/gfeisbozj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.sjlbkw.cn/Article/details/gsftjeutg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.tarul.cn/Article/details/gmptttoxo.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.sjlbkw.cn/Article/details/gkszltxko.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.tarul.cn/Article/details/gqdzrunof.sHtML

[C03] 可变参数
来源：http://baike.tarul.cn/Article/details/gzkrbcgqn.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fktsv.cn/Article/details/grmchlnpr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.epnwcf.com/Article/details/gjzoprrnh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.epnwcf.com/Article/details/guoicuecn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.tarul.cn/Article/details/glepgescp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.tarul.cn/Article/details/gyqlawznx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.bbcook.cn/Article/details/gsaoylftg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.sjlbkw.cn/Article/details/gfbqqpysu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.yfazqb.com/Article/details/gmrxyzbim.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.epnwcf.com/Article/details/gofrxxuon.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fktsv.cn/Article/details/gintknayg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.yfazqb.com/Article/details/gdlkafwur.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.yfazqb.com/Article/details/gbzriztzg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.sjlbkw.cn/Article/details/gmlexckhn.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.tarul.cn/Article/details/gssmhzgvd.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.yfazqb.com/Article/details/glpzlxgaf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.sjlbkw.cn/Article/details/gfrpmoxvj.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.yfazqb.com/Article/details/guhpnnbcx.sHtML

[C05] 返回多个值
来源：http://read.share.vehdjk.com/Article/details/gqobtpstj.sHtML

Py:   return a, b
来源：http://wap.tarul.cn/Article/details/gealxbmxw.sHtML

PHP:  return [$a, $b];
来源：http://m.share.yfazqb.com/Article/details/ghyfmoriz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.tarul.cn/Article/details/gafcasmmf.sHtML

TS:   return { a, b };
来源：http://wap.fktsv.cn/Article/details/ghbagubkt.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fktsv.cn/Article/details/gcduetdqn.sHtML

Go:   return a, b
来源：http://baike.yfazqb.com/Article/details/gbcpkkabo.sHtML

Ruby: return a, b
来源：http://read.share.yfazqb.com/Article/details/goidkymvk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.bbcook.cn/Article/details/gvlbqnwjg.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.epnwcf.com/Article/details/glbpzqbss.sHtML

Py:   square = lambda x: x * x
来源：http://blog.bbcook.cn/Article/details/gpqttvnin.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.bbcook.cn/Article/details/gdxhcwpff.sHtML

JS:   const square = x => x * x;
来源：http://baike.vehdjk.com/Article/details/gyuzjipvf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.epnwcf.com/Article/details/gmlvunfsm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.bbcook.cn/Article/details/goineoujt.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.bbcook.cn/Article/details/gduzybnir.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.vehdjk.com/Article/details/gcxpiysyk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.yfazqb.com/Article/details/gigkvsdjs.sHtML

[C07] 把函数作为参数传入
来源：http://3g.tarul.cn/Article/details/gumbssvtg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fktsv.cn/Article/details/gcpejcixj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.sjlbkw.cn/Article/details/gdiafxyje.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.bbcook.cn/Article/details/gpntrkwib.sHtML

TS:   arr.map(String)
来源：http://read.share.vehdjk.com/Article/details/gpwmcmwdp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.vehdjk.com/Article/details/gajuddklp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.bbcook.cn/Article/details/gvzeunbwx.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.vehdjk.com/Article/details/ggwmwqulh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.bbcook.cn/Article/details/giwlyzjjg.sHtML

[C08] 闭包
来源：http://read.share.tarul.cn/Article/details/gnljlvvun.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.vehdjk.com/Article/details/gswgtexor.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.tarul.cn/Article/details/gstkjyhyd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fktsv.cn/Article/details/gxzicvkul.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.sjlbkw.cn/Article/details/grwyxtyol.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.tarul.cn/Article/details/gnxjhefwm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.vehdjk.com/Article/details/gpqajiumm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.tarul.cn/Article/details/gleyieeso.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.yfazqb.com/Article/details/gldnhjjcq.sHtML

[C09] 递归
来源：http://read.share.vehdjk.com/Article/details/gqxvwdxmd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.epnwcf.com/Article/details/gxhkijssl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.bbcook.cn/Article/details/ghhrjxfox.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.yfazqb.com/Article/details/ghcvjfxnc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.bbcook.cn/Article/details/gcwsgmxzb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.epnwcf.com/Article/details/ggmtamwdt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fktsv.cn/Article/details/gzgcrovuk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.yfazqb.com/Article/details/gjdbiohzx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.yfazqb.com/Article/details/ggrtrpusd.sHtML

[C10] 变量作用域
来源：http://mobile.tarul.cn/Article/details/ghzspcjoy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fktsv.cn/Article/details/gvwdqapii.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fktsv.cn/Article/details/glyrabspm.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.tarul.cn/Article/details/gbxsijcgr.sHtML

TS:   同 JS
来源：http://www.share.fktsv.cn/Article/details/gkfssqved.sHtML

Java: 方法内为块级作用域
来源：http://read.share.tarul.cn/Article/details/gppbumrxq.sHtML

Go:   花括号块级作用域
来源：http://m.share.fktsv.cn/Article/details/gjacyaozs.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.tarul.cn/Article/details/grtamwgoe.sHtML

C#:   块级作用域
来源：http://m.share.vehdjk.com/Article/details/glqnieusq.sHtML

[C11] 模块导入与导出
来源：http://3g.tarul.cn/Article/details/gvhpqfjns.sHtML

Py:   from module import func
来源：http://m.share.sjlbkw.cn/Article/details/gkzddavxe.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.yfazqb.com/Article/details/gekvtsfhm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.bbcook.cn/Article/details/gxdldrrgt.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.epnwcf.com/Article/details/glviebmeu.sHtML

Java: import java.util.List;
来源：http://wap.bbcook.cn/Article/details/geojhrwkt.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.sjlbkw.cn/Article/details/guvlpvkbz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.epnwcf.com/Article/details/gnapxnibu.sHtML

C#:   using System.Text;
来源：http://www.m.share.tarul.cn/Article/details/gxagsvpfq.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fktsv.cn/Article/details/gwdrtahxi.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fktsv.cn/Article/details/gkdrmrsye.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.epnwcf.com/Article/details/gzuoduukd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.vehdjk.com/Article/details/ggbvvpaae.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.bbcook.cn/Article/details/gfflqzdvm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.vehdjk.com/Article/details/gtiqfbysg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fktsv.cn/Article/details/gdyqdtobi.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fktsv.cn/Article/details/geffiyirb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fktsv.cn/Article/details/gtbdzrrjo.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.sjlbkw.cn/Article/details/gncvftgwi.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fktsv.cn/Article/details/gedkhyorq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.tarul.cn/Article/details/gtqpltbdw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fktsv.cn/Article/details/gnurvvuon.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/gtfwrtdns.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gxnkjkcqq.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fktsv.cn/Article/details/ggyrpaaog.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.tarul.cn/Article/details/ghjgkloca.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.sjlbkw.cn/Article/details/gamslbkpo.sHtML

[C14] 泛型函数
来源：http://www.m.share.tarul.cn/Article/details/gbywzyulc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.sjlbkw.cn/Article/details/grcinuhcq.sHtML

PHP:  // 无泛型
来源：http://read.share.vehdjk.com/Article/details/gdgsapfej.sHtML

JS:   // 无泛型
来源：http://read.share.tarul.cn/Article/details/gzrtsloqe.sHtML


<!-- 参考信息 -->