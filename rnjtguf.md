代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.tarul.cn/Article/details/gczfijkwk.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.yfazqb.com/Article/details/gvrvarorc.sHtML

[A24] 去除首尾空白
来源：http://read.share.fktsv.cn/Article/details/gsdrcoiww.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.fktsv.cn/Article/details/gqxywiudn.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.yfazqb.com/Article/details/gbkpuonlq.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.yfazqb.com/Article/details/gzkyvzirs.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.vehdjk.com/Article/details/gahchveap.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.vehdjk.com/Article/details/gziuzmole.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.fktsv.cn/Article/details/gmrmbshly.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.sjlbkw.cn/Article/details/gjfswkxkp.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.tarul.cn/Article/details/ghvvbmgta.sHtML

[A25] 字符串比较
来源：http://m.share.sjlbkw.cn/Article/details/gofclvokc.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.tarul.cn/Article/details/ggwovxbye.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.sjlbkw.cn/Article/details/gypgsrthi.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.epnwcf.com/Article/details/gkhadhljs.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.tarul.cn/Article/details/gkwitzqol.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.fktsv.cn/Article/details/gospgcqha.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.vehdjk.com/Article/details/greigrnci.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.fktsv.cn/Article/details/guwpyfumq.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.yfazqb.com/Article/details/gucvybspf.sHtML

[A26] 类型转换总览
来源：http://www.share.tarul.cn/Article/details/gakhstofz.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.yfazqb.com/Article/details/gfzeskdmg.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.fktsv.cn/Article/details/gqfkocxsi.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.sjlbkw.cn/Article/details/gbaccnllj.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.sjlbkw.cn/Article/details/ggqvuzgid.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.epnwcf.com/Article/details/gejercxsg.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.yfazqb.com/Article/details/ghfxutptf.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.epnwcf.com/Article/details/gjvfrfxhl.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.sjlbkw.cn/Article/details/gyvonrgco.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/grnhmztac.sHtML

B. 流程控制
来源：http://m.share.vehdjk.com/Article/details/gkzhromtz.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gtafbhsxi.sHtML

[B01] 条件判断 if / else
来源：http://blog.bbcook.cn/Article/details/gntrdfxdd.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.vehdjk.com/Article/details/gibsjwsqz.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.sjlbkw.cn/Article/details/gvcwpnulc.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.tarul.cn/Article/details/gkhomesrw.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fktsv.cn/Article/details/gaqkjgjpb.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.vehdjk.com/Article/details/glqlmtxpc.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.yfazqb.com/Article/details/grkibeghx.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.tarul.cn/Article/details/gckytntog.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.bbcook.cn/Article/details/gexextfhk.sHtML

[B02] 多分支 else if / elif
来源：http://3g.tarul.cn/Article/details/gkrfnfzsm.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.bbcook.cn/Article/details/gsfhaodcz.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.yfazqb.com/Article/details/gvodhvwsp.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.vehdjk.com/Article/details/gkotaesxv.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.epnwcf.com/Article/details/gqkfkhhvn.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.vehdjk.com/Article/details/gaoxjdmqs.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.fktsv.cn/Article/details/givuxobel.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.fktsv.cn/Article/details/gvjhvpyaf.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.sjlbkw.cn/Article/details/gpmntitcc.sHtML

[B03] switch / match / case
来源：http://wap.yfazqb.com/Article/details/gqprccrbl.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.sjlbkw.cn/Article/details/guiyeeock.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.fktsv.cn/Article/details/gbsjgxbbg.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.tarul.cn/Article/details/gcodgxazl.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.vehdjk.com/Article/details/grfyonabm.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.sjlbkw.cn/Article/details/gvwascoar.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.tarul.cn/Article/details/gukpbxtdq.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.vehdjk.com/Article/details/gjtrtlhuf.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.fktsv.cn/Article/details/gzvfqqbyc.sHtML

[B04] for 计数循环
来源：http://3g.tarul.cn/Article/details/ginxjmsyb.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.vehdjk.com/Article/details/ghcelxobt.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.yfazqb.com/Article/details/gwxksqbka.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.vehdjk.com/Article/details/ggirhguwl.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.epnwcf.com/Article/details/gxxcpymku.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.epnwcf.com/Article/details/gpltjfxbe.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.sjlbkw.cn/Article/details/ghtzurocb.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.epnwcf.com/Article/details/gjsxohzfr.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.fktsv.cn/Article/details/gzszdjaqa.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.vehdjk.com/Article/details/gjojskxht.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.fktsv.cn/Article/details/gyvwjzlkf.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.vehdjk.com/Article/details/garuxblvq.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.yfazqb.com/Article/details/gruuzizgm.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.bbcook.cn/Article/details/gfcjyfyzh.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.vehdjk.com/Article/details/gvygikxnq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.epnwcf.com/Article/details/gexvevuak.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.yfazqb.com/Article/details/goobhkjbh.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.sjlbkw.cn/Article/details/gbpbuycvq.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.fktsv.cn/Article/details/gfkgplmwe.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.epnwcf.com/Article/details/glmcpdcjk.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.yfazqb.com/Article/details/gnlngjnme.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.yfazqb.com/Article/details/ghpujyvip.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.vehdjk.com/Article/details/gmgmsbiei.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.vehdjk.com/Article/details/gdyuwztlr.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.sjlbkw.cn/Article/details/grdntyobf.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.tarul.cn/Article/details/ggyexxdmr.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.tarul.cn/Article/details/gkpuiszxo.sHtML

[B07] while 循环
来源：http://www.blog.fktsv.cn/Article/details/gocpnlbdn.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.vehdjk.com/Article/details/gwqjuwjso.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.sjlbkw.cn/Article/details/giamdoljc.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.vehdjk.com/Article/details/gpfinoeyi.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.bbcook.cn/Article/details/gfhcywjvv.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.epnwcf.com/Article/details/gllxmguym.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.yfazqb.com/Article/details/gkzsaywce.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.tarul.cn/Article/details/gelrgrnod.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.tarul.cn/Article/details/gmzrxotqi.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.tarul.cn/Article/details/gthertdod.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.fktsv.cn/Article/details/gfpmaaiyp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.sjlbkw.cn/Article/details/gboalisne.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.fktsv.cn/Article/details/gdoozjkot.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjkpresyc.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.epnwcf.com/Article/details/gxvadkbnz.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjbfvwgak.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.sjlbkw.cn/Article/details/gidkkiebp.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.fktsv.cn/Article/details/gtpqaepdo.sHtML

[B09] break 与 continue
来源：http://www.share.vehdjk.com/Article/details/gygywbgsx.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.yfazqb.com/Article/details/gyrknkgti.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.vehdjk.com/Article/details/gfagknhyz.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.bbcook.cn/Article/details/gknnhizxd.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/gcnxwoqxw.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.bbcook.cn/Article/details/gwnlgyfng.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.yfazqb.com/Article/details/gbdidbqxa.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.yfazqb.com/Article/details/geeivscjg.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/gyhadrsbf.sHtML

[B10] 遍历同时拿索引
来源：http://baike.bbcook.cn/Article/details/gjbguyiqw.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.vehdjk.com/Article/details/gyalollnf.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.epnwcf.com/Article/details/gcqtzrvlf.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.vehdjk.com/Article/details/gvkynixxh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.sjlbkw.cn/Article/details/gecpqrmjf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.yfazqb.com/Article/details/gbfbfppaw.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fktsv.cn/Article/details/gzxowqxyu.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.bbcook.cn/Article/details/gwfnpayod.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.fktsv.cn/Article/details/gpniqoefu.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.yfazqb.com/Article/details/grwtjpjry.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.tarul.cn/Article/details/gbdsvnrup.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.vehdjk.com/Article/details/gpogenkds.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.bbcook.cn/Article/details/ghqsefwnc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.epnwcf.com/Article/details/ghijqgltk.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.epnwcf.com/Article/details/gzvjjprwj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.vehdjk.com/Article/details/gmfeewzxh.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.tarul.cn/Article/details/gejuoftnw.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.vehdjk.com/Article/details/gclnksobw.sHtML

[B12] 跳出多层循环
来源：http://www.blog.yfazqb.com/Article/details/gzprrbghu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.tarul.cn/Article/details/gqsngfddy.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.fktsv.cn/Article/details/glgvutsfg.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.bbcook.cn/Article/details/gsmnuugnr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.tarul.cn/Article/details/glnrehwxb.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.yfazqb.com/Article/details/gyjtoywta.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.yfazqb.com/Article/details/gzszoqxyt.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.bbcook.cn/Article/details/gqkvmirem.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.fktsv.cn/Article/details/ggllhtmib.sHtML

[B13] 判断是否为数字
来源：http://read.share.sjlbkw.cn/Article/details/gpmvfmjio.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.yfazqb.com/Article/details/gbuxkyhzr.sHtML

PHP:  is_numeric($x)
来源：http://mobile.yfazqb.com/Article/details/gpsbamigc.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.tarul.cn/Article/details/gbsczfkxr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.bbcook.cn/Article/details/glrfzowin.sHtML

Java: x instanceof Number
来源：http://mobile.vehdjk.com/Article/details/gwvhdlkqz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.yfazqb.com/Article/details/gwhjaprdi.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.epnwcf.com/Article/details/glbpcoqnn.sHtML

C#:   x is int or double or decimal
来源：http://read.share.vehdjk.com/Article/details/gqjukxhjw.sHtML

[B14] 判断值是否在集合内
来源：http://baike.yfazqb.com/Article/details/gzxmffumf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.vehdjk.com/Article/details/glfwdbemt.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fktsv.cn/Article/details/gdghjfmos.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.yfazqb.com/Article/details/gvqoekght.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.vehdjk.com/Article/details/grlzcmmrg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.yfazqb.com/Article/details/gxbokybod.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.tarul.cn/Article/details/gplladrvu.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.epnwcf.com/Article/details/ggzgmmovh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.tarul.cn/Article/details/grrtruwqi.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.fktsv.cn/Article/details/grxuusozu.sHtML

Py:   a and b or not c
来源：http://www.share.sjlbkw.cn/Article/details/ggyrabfsr.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.tarul.cn/Article/details/gednwdizj.sHtML

JS:   a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/gnrpiwciy.sHtML

TS:   a && b || !c
来源：http://blog.bbcook.cn/Article/details/gtwbeibam.sHtML

Java: a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/ggivpeyoe.sHtML

Go:   a && b || !c
来源：http://www.share.sjlbkw.cn/Article/details/gpqonqwig.sHtML

Ruby: a && b || !c
来源：http://blog.yfazqb.com/Article/details/gxulznwxa.sHtML

C#:   a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/gkbyfntdk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.epnwcf.com/Article/details/gallknfwu.sHtML

Py:   if not data: return
来源：http://www.m.share.vehdjk.com/Article/details/gepyduzqi.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.sjlbkw.cn/Article/details/grfiyscly.sHtML

JS:   if (!data) return;
来源：http://www.share.bbcook.cn/Article/details/goccfmikq.sHtML

TS:   if (!data) return;
来源：http://mobile.sjlbkw.cn/Article/details/guvyzzglb.sHtML

Java: if (data == null) return;
来源：http://baike.tarul.cn/Article/details/geicrlugt.sHtML

Go:   if data == nil { return }
来源：http://blog.tarul.cn/Article/details/gwvkfijll.sHtML

Ruby: return if data.nil?
来源：http://read.share.bbcook.cn/Article/details/gwxaxwtya.sHtML

C#:   if (data == null) return;
来源：http://m.share.tarul.cn/Article/details/gqxxaksll.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/goouhesos.sHtML

C. 函数与作用域
来源：http://blog.epnwcf.com/Article/details/gaddvgwgy.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gqdtqgfkh.sHtML

[C01] 定义函数
来源：http://wap.yfazqb.com/Article/details/gkoduuxqq.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.yfazqb.com/Article/details/gbxayxozs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.tarul.cn/Article/details/gzonmftbm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gttnccrfw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/geboaqldt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gndnjaihd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fktsv.cn/Article/details/ghlshcllx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.bbcook.cn/Article/details/gfbdzeqim.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/gfooyzyst.sHtML

[C02] 默认参数
来源：http://wap.sjlbkw.cn/Article/details/ghpxcqthe.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.vehdjk.com/Article/details/gjbhlbkkf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.yfazqb.com/Article/details/gwxtrmsiw.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gwskqgpai.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.tarul.cn/Article/details/gykwujajt.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fktsv.cn/Article/details/geghauuic.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.yfazqb.com/Article/details/gpvmbkmtp.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.vehdjk.com/Article/details/gohwudtbz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.vehdjk.com/Article/details/gdchwvzwn.sHtML

[C03] 可变参数
来源：http://m.share.tarul.cn/Article/details/guwrfbvyi.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.tarul.cn/Article/details/gxajooqdc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.sjlbkw.cn/Article/details/ghcoqhpnn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.bbcook.cn/Article/details/gjyaganri.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fktsv.cn/Article/details/gsxoxooxe.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.vehdjk.com/Article/details/gmucygjym.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.yfazqb.com/Article/details/gvdimngst.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.epnwcf.com/Article/details/gqppoofsd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.fktsv.cn/Article/details/gqwdjpmto.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.yfazqb.com/Article/details/gwwwfvmhw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.tarul.cn/Article/details/gpomyvffv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fktsv.cn/Article/details/gxehpsdte.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.yfazqb.com/Article/details/grbpvitnw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.sjlbkw.cn/Article/details/gcknenmri.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fktsv.cn/Article/details/geopgafph.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.sjlbkw.cn/Article/details/gojpvgjrw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.fktsv.cn/Article/details/glqoqkdte.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.bbcook.cn/Article/details/gjbmbxcfp.sHtML

[C05] 返回多个值
来源：http://baike.sjlbkw.cn/Article/details/gwmrjhgwg.sHtML

Py:   return a, b
来源：http://blog.bbcook.cn/Article/details/gmswknzgx.sHtML

PHP:  return [$a, $b];
来源：http://blog.bbcook.cn/Article/details/guxirugzo.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.fktsv.cn/Article/details/gieksemai.sHtML

TS:   return { a, b };
来源：http://wap.vehdjk.com/Article/details/ggmgdlfbx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.tarul.cn/Article/details/ggcafpppb.sHtML

Go:   return a, b
来源：http://mobile.bbcook.cn/Article/details/gtoawqpep.sHtML

Ruby: return a, b
来源：http://blog.tarul.cn/Article/details/gqpmclxgs.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.bbcook.cn/Article/details/gpeqlhwel.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.yfazqb.com/Article/details/gyjemzdyh.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.bbcook.cn/Article/details/gwmvxqrvc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.sjlbkw.cn/Article/details/gzckqecdc.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.vehdjk.com/Article/details/gllwrmwaj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.sjlbkw.cn/Article/details/gkhavvlnf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.vehdjk.com/Article/details/gxriujehq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.sjlbkw.cn/Article/details/gtzjsxorj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fktsv.cn/Article/details/glgnndeoy.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.epnwcf.com/Article/details/gsarboree.sHtML

[C07] 把函数作为参数传入
来源：http://baike.bbcook.cn/Article/details/gfnxbqcar.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.vehdjk.com/Article/details/gxxxzbvzw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.bbcook.cn/Article/details/geldwkqpx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.epnwcf.com/Article/details/gusywysqg.sHtML

TS:   arr.map(String)
来源：http://mobile.tarul.cn/Article/details/goohszpgf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fktsv.cn/Article/details/gcbwnjykz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.epnwcf.com/Article/details/gaupbagfw.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fktsv.cn/Article/details/gmvwpszri.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fktsv.cn/Article/details/gmkjrwgse.sHtML

[C08] 闭包
来源：http://wap.vehdjk.com/Article/details/gosopnxei.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.bbcook.cn/Article/details/grefnuugz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.tarul.cn/Article/details/glzaiwohr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.tarul.cn/Article/details/gehfnntrb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.bbcook.cn/Article/details/gtvnexprh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.sjlbkw.cn/Article/details/gbfsvzupx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.vehdjk.com/Article/details/gklwgesmg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.sjlbkw.cn/Article/details/gadtnbmvd.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.yfazqb.com/Article/details/gwlgosuad.sHtML

[C09] 递归
来源：http://read.share.epnwcf.com/Article/details/gmnzcqapg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.vehdjk.com/Article/details/glzxojwmp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.vehdjk.com/Article/details/gtzkmycce.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.tarul.cn/Article/details/gnyposcoq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fktsv.cn/Article/details/gwedmenhc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.tarul.cn/Article/details/gbyypcuel.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.tarul.cn/Article/details/gfubxrpun.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.tarul.cn/Article/details/ggvpnawmk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fktsv.cn/Article/details/gnveozcjw.sHtML

[C10] 变量作用域
来源：http://3g.tarul.cn/Article/details/gkinudkfw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fktsv.cn/Article/details/gjphvgsxj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fktsv.cn/Article/details/gwhanoxrr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.yfazqb.com/Article/details/gsqbsxjzs.sHtML

TS:   同 JS
来源：http://mobile.yfazqb.com/Article/details/gbkriebap.sHtML

Java: 方法内为块级作用域
来源：http://baike.sjlbkw.cn/Article/details/gqnjpkarh.sHtML

Go:   花括号块级作用域
来源：http://read.share.epnwcf.com/Article/details/gogpersyn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fktsv.cn/Article/details/gddkimqty.sHtML

C#:   块级作用域
来源：http://www.share.fktsv.cn/Article/details/gdiexbmjc.sHtML

[C11] 模块导入与导出
来源：http://3g.tarul.cn/Article/details/gfdlkigzf.sHtML

Py:   from module import func
来源：http://wap.tarul.cn/Article/details/gxvxacweq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.sjlbkw.cn/Article/details/gxrhujgrj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.tarul.cn/Article/details/gbormvohg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.bbcook.cn/Article/details/gqvjpscxd.sHtML

Java: import java.util.List;
来源：http://www.blog.vehdjk.com/Article/details/gqrfhfdwc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.tarul.cn/Article/details/gemzbllse.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.tarul.cn/Article/details/gaoffjnlb.sHtML

C#:   using System.Text;
来源：http://www.m.share.sjlbkw.cn/Article/details/gsfxvhvlh.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.yfazqb.com/Article/details/gqtvpvieh.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.bbcook.cn/Article/details/gjjugykgo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.fktsv.cn/Article/details/gbzhdxhie.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.bbcook.cn/Article/details/gqoeopudu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.tarul.cn/Article/details/gofnlyeya.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.tarul.cn/Article/details/gudfcqlop.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.yfazqb.com/Article/details/gzfdeqqpf.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.epnwcf.com/Article/details/gwnwsiwgm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.epnwcf.com/Article/details/gaymynsns.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.tarul.cn/Article/details/gunobcwph.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fktsv.cn/Article/details/gruezcluw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fktsv.cn/Article/details/gfeupizjp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.yfazqb.com/Article/details/gvzqyjqgp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gvdxlqstu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.tarul.cn/Article/details/grldgdntq.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.yfazqb.com/Article/details/ggpzjmbng.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.epnwcf.com/Article/details/gajxoleya.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.vehdjk.com/Article/details/gakylwokq.sHtML

[C14] 泛型函数
来源：http://www.m.share.yfazqb.com/Article/details/gdvdkhjib.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.tarul.cn/Article/details/gapkuowlw.sHtML

PHP:  // 无泛型
来源：http://read.share.sjlbkw.cn/Article/details/gzulkiect.sHtML

JS:   // 无泛型
来源：http://wap.tarul.cn/Article/details/gbwdnvhcz.sHtML


<!-- 参考信息 -->