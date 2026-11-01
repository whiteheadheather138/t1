代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://www.m.share.vehdjk.com/Article/details/gnoxppvsz.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.epnwcf.com/Article/details/gtrivclvm.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.epnwcf.com/Article/details/gxluzoyvf.sHtML

[A25] 字符串比较
来源：http://baike.bbcook.cn/Article/details/gytigiqtw.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.yfazqb.com/Article/details/gvfnneasc.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.yfazqb.com/Article/details/gtepmnkbl.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.epnwcf.com/Article/details/gvpqlanbn.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.vehdjk.com/Article/details/gpvarummg.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.sjlbkw.cn/Article/details/gjotqlcjb.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.vehdjk.com/Article/details/gfwnkmhfc.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.fktsv.cn/Article/details/gvkicifcr.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.sjlbkw.cn/Article/details/gxfqeozpq.sHtML

[A26] 类型转换总览
来源：http://blog.tarul.cn/Article/details/gnppzdwar.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.tarul.cn/Article/details/grrhlxavc.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.sjlbkw.cn/Article/details/ggdhnivwu.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.epnwcf.com/Article/details/gcpgxczta.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.epnwcf.com/Article/details/gljgweugr.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.epnwcf.com/Article/details/gkxjpzbmf.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.epnwcf.com/Article/details/gzrpfsxpb.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.vehdjk.com/Article/details/gjyaksixj.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.sjlbkw.cn/Article/details/gflcgpkto.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/grzypqnpv.sHtML

B. 流程控制
来源：http://www.blog.vehdjk.com/Article/details/gfbnfbdxp.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gexjfjnqz.sHtML

[B01] 条件判断 if / else
来源：http://blog.fktsv.cn/Article/details/gqinokpaw.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.bbcook.cn/Article/details/gilgxxuvm.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.vehdjk.com/Article/details/ggsgdzhpa.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fktsv.cn/Article/details/galprhzkv.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.epnwcf.com/Article/details/gljyqeotq.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.epnwcf.com/Article/details/glnzozoly.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.vehdjk.com/Article/details/gtzjnjylf.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.bbcook.cn/Article/details/gzxevhibk.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.tarul.cn/Article/details/gxvwlrmkd.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.fktsv.cn/Article/details/gbuoxrzds.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.tarul.cn/Article/details/gkbvbauiq.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.vehdjk.com/Article/details/gtdduukxa.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.vehdjk.com/Article/details/goxhukstp.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.sjlbkw.cn/Article/details/gyfpxnnmk.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.yfazqb.com/Article/details/gxhyfesji.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.fktsv.cn/Article/details/guwanjzza.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.yfazqb.com/Article/details/gabugwtdm.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fktsv.cn/Article/details/gyquodslb.sHtML

[B03] switch / match / case
来源：http://m.share.epnwcf.com/Article/details/gyabuemhn.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.bbcook.cn/Article/details/gikwbleda.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.epnwcf.com/Article/details/gnkcnqumt.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.vehdjk.com/Article/details/gdfzrcave.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.epnwcf.com/Article/details/gpjkvwesp.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.tarul.cn/Article/details/ggkpjaquw.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.tarul.cn/Article/details/gwxlltltb.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.sjlbkw.cn/Article/details/gktlpytnj.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.sjlbkw.cn/Article/details/gsrlnjklq.sHtML

[B04] for 计数循环
来源：http://wap.vehdjk.com/Article/details/gmdexzfag.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.yfazqb.com/Article/details/gfzgpzcmj.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.fktsv.cn/Article/details/ghfuvtfct.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fktsv.cn/Article/details/gbndvjozj.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.epnwcf.com/Article/details/gqcojnzro.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.sjlbkw.cn/Article/details/gvgwmcivi.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.fktsv.cn/Article/details/gwtrkjwdm.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.vehdjk.com/Article/details/guqmanmtb.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.sjlbkw.cn/Article/details/gcummijmx.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.bbcook.cn/Article/details/gjlpjpuox.sHtML

Py:   for item in arr: print(item)
来源：http://wap.tarul.cn/Article/details/gwrotzagq.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.vehdjk.com/Article/details/gwhzxxacn.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.tarul.cn/Article/details/gedaiuxvj.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.tarul.cn/Article/details/gohglrpsb.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.fktsv.cn/Article/details/gbddqfsso.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.vehdjk.com/Article/details/gqqmhkoed.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.sjlbkw.cn/Article/details/gcsjpaifv.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.bbcook.cn/Article/details/glqlvmvxh.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.tarul.cn/Article/details/gwlxavxxo.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.bbcook.cn/Article/details/ggqpnnfhk.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.yfazqb.com/Article/details/gkysnyypn.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.tarul.cn/Article/details/gisffbvdu.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.vehdjk.com/Article/details/gqfmtolcx.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.fktsv.cn/Article/details/grupnnlxx.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.epnwcf.com/Article/details/gyjtmwtvp.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.epnwcf.com/Article/details/gxdelpaii.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.tarul.cn/Article/details/gbqxtgumf.sHtML

[B07] while 循环
来源：http://blog.epnwcf.com/Article/details/gajoydkbl.sHtML

Py:   while i < 10: i += 1
来源：http://blog.fktsv.cn/Article/details/gzcrhphnc.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.vehdjk.com/Article/details/gthmjluwt.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.tarul.cn/Article/details/gbguwlcyj.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.epnwcf.com/Article/details/gwyqgyysi.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.yfazqb.com/Article/details/gftbzcohw.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.yfazqb.com/Article/details/gxtmpokcv.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.epnwcf.com/Article/details/gurjphtys.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.epnwcf.com/Article/details/gjckpasca.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.bbcook.cn/Article/details/gqgrhnwaf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.bbcook.cn/Article/details/gnwhfnhhx.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.epnwcf.com/Article/details/gdnydqthq.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.bbcook.cn/Article/details/gsavnicvx.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.yfazqb.com/Article/details/gzxfalbfy.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.vehdjk.com/Article/details/gjekiisbo.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.tarul.cn/Article/details/gwlhmxiwg.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.bbcook.cn/Article/details/gszfkbsvg.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.tarul.cn/Article/details/gxovoazjd.sHtML

[B09] break 与 continue
来源：http://wap.sjlbkw.cn/Article/details/ghqkqfqbb.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.yfazqb.com/Article/details/guxzqdnhe.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.tarul.cn/Article/details/gqlieynbr.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.sjlbkw.cn/Article/details/gogqxvffe.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.epnwcf.com/Article/details/getezdbwv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.tarul.cn/Article/details/gmfwuhcki.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.epnwcf.com/Article/details/gzpwcghin.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.sjlbkw.cn/Article/details/gkhluxnkl.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.sjlbkw.cn/Article/details/gktazilbx.sHtML

[B10] 遍历同时拿索引
来源：http://3g.fktsv.cn/Article/details/gjnbleamf.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.tarul.cn/Article/details/ggvduvnbo.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.vehdjk.com/Article/details/gfelugnah.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.tarul.cn/Article/details/gwurwtowe.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.bbcook.cn/Article/details/gslohmjvc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.fktsv.cn/Article/details/gopzkojzl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.tarul.cn/Article/details/gwyzltjhq.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.yfazqb.com/Article/details/gfxeaexch.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.epnwcf.com/Article/details/ghmszxmdw.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.fktsv.cn/Article/details/gmtkvyvab.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.fktsv.cn/Article/details/gkjtgdrxe.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.tarul.cn/Article/details/gwrtocjug.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fktsv.cn/Article/details/ggwgfmtre.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fktsv.cn/Article/details/gppkezffc.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.yfazqb.com/Article/details/gavgcmppy.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.sjlbkw.cn/Article/details/gkhhvxbra.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.bbcook.cn/Article/details/gdryensdp.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.fktsv.cn/Article/details/gfxaqmevs.sHtML

[B12] 跳出多层循环
来源：http://www.blog.epnwcf.com/Article/details/gmpsempmu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.yfazqb.com/Article/details/ghdwtwgsb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.sjlbkw.cn/Article/details/gcpwixmrb.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.tarul.cn/Article/details/gmbuidaec.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.epnwcf.com/Article/details/gguvnjcrv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fktsv.cn/Article/details/gojjsjrrj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.vehdjk.com/Article/details/gycrcgzms.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fktsv.cn/Article/details/gajobgwoh.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.sjlbkw.cn/Article/details/gdguizfht.sHtML

[B13] 判断是否为数字
来源：http://read.share.sjlbkw.cn/Article/details/gqevpcykc.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fktsv.cn/Article/details/gpaqythop.sHtML

PHP:  is_numeric($x)
来源：http://blog.sjlbkw.cn/Article/details/girzvnsdv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.bbcook.cn/Article/details/guggqbnjb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.yfazqb.com/Article/details/gtyncaiol.sHtML

Java: x instanceof Number
来源：http://www.blog.yfazqb.com/Article/details/gntgfvmzk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.epnwcf.com/Article/details/gkpfrrfjy.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.vehdjk.com/Article/details/gjuxphnuk.sHtML

C#:   x is int or double or decimal
来源：http://wap.bbcook.cn/Article/details/gddtsoysr.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.yfazqb.com/Article/details/grqlgvook.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.sjlbkw.cn/Article/details/gwqjqlzmg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.tarul.cn/Article/details/gwnzmpidj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.vehdjk.com/Article/details/gtmpztmjt.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.bbcook.cn/Article/details/gbzntibwl.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.bbcook.cn/Article/details/gvlsrmmsf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.tarul.cn/Article/details/gavlybajn.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fktsv.cn/Article/details/gsyllerhb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.fktsv.cn/Article/details/gbffxktlb.sHtML

[B15] 布尔运算与取反
来源：http://read.share.tarul.cn/Article/details/gapyqulwo.sHtML

Py:   a and b or not c
来源：http://baike.sjlbkw.cn/Article/details/geyrbrssl.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.fktsv.cn/Article/details/gurlhdiau.sHtML

JS:   a && b || !c
来源：http://www.share.bbcook.cn/Article/details/gxqqfbqdz.sHtML

TS:   a && b || !c
来源：http://www.share.bbcook.cn/Article/details/gyecyadwk.sHtML

Java: a && b || !c
来源：http://www.share.yfazqb.com/Article/details/gjmtvfkfo.sHtML

Go:   a && b || !c
来源：http://m.share.yfazqb.com/Article/details/gktmorocj.sHtML

Ruby: a && b || !c
来源：http://baike.tarul.cn/Article/details/gcqwuoxro.sHtML

C#:   a && b || !c
来源：http://baike.yfazqb.com/Article/details/gvwuubxjv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.epnwcf.com/Article/details/goqhivcin.sHtML

Py:   if not data: return
来源：http://m.share.fktsv.cn/Article/details/gjdbfgbkc.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.sjlbkw.cn/Article/details/gnutvidoi.sHtML

JS:   if (!data) return;
来源：http://3g.fktsv.cn/Article/details/gxkdnjkum.sHtML

TS:   if (!data) return;
来源：http://www.m.share.vehdjk.com/Article/details/gapiggdmf.sHtML

Java: if (data == null) return;
来源：http://mobile.fktsv.cn/Article/details/gswfomhhn.sHtML

Go:   if data == nil { return }
来源：http://read.share.tarul.cn/Article/details/gtmbtgrkj.sHtML

Ruby: return if data.nil?
来源：http://baike.yfazqb.com/Article/details/gdwlbmjhn.sHtML

C#:   if (data == null) return;
来源：http://www.share.sjlbkw.cn/Article/details/gsizsjnyt.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gvoeuayqy.sHtML

C. 函数与作用域
来源：http://www.blog.tarul.cn/Article/details/gqkkotnsq.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/goawiyyun.sHtML

[C01] 定义函数
来源：http://m.share.vehdjk.com/Article/details/ghackptrr.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.sjlbkw.cn/Article/details/gcbzlfbsz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.vehdjk.com/Article/details/gelbtwgch.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.yfazqb.com/Article/details/gxvsscpux.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gqmppmpxk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.vehdjk.com/Article/details/gvebuofpq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fktsv.cn/Article/details/gcgfasonw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.bbcook.cn/Article/details/gihryaxiy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/gvfbxiqrv.sHtML

[C02] 默认参数
来源：http://www.share.vehdjk.com/Article/details/glgrgkonr.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.sjlbkw.cn/Article/details/glmplmtnb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.vehdjk.com/Article/details/glwyfmcfa.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fktsv.cn/Article/details/gkvxwkody.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.epnwcf.com/Article/details/gurshwjjn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.sjlbkw.cn/Article/details/goxvyeqpu.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.tarul.cn/Article/details/gvmuvmaim.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.yfazqb.com/Article/details/gvcpwkwzy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.vehdjk.com/Article/details/gvdkiohcg.sHtML

[C03] 可变参数
来源：http://wap.fktsv.cn/Article/details/gjkumvery.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.sjlbkw.cn/Article/details/gtstzeqyy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.yfazqb.com/Article/details/gjcmhzhwf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.bbcook.cn/Article/details/gjqedajln.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.vehdjk.com/Article/details/gfjdswxft.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.yfazqb.com/Article/details/ghozsxxtp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.sjlbkw.cn/Article/details/gzqqmguog.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.epnwcf.com/Article/details/gpoabgvkt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.sjlbkw.cn/Article/details/giyvthhlv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.vehdjk.com/Article/details/gqblwmpyg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fktsv.cn/Article/details/glymtcuya.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.epnwcf.com/Article/details/gupgzpiad.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.yfazqb.com/Article/details/gechemlub.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.bbcook.cn/Article/details/gbrwbvmzu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.epnwcf.com/Article/details/glfdskzsm.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.yfazqb.com/Article/details/gnjjxmojw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbocjgkvt.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.vehdjk.com/Article/details/ggoeiwjsa.sHtML

[C05] 返回多个值
来源：http://wap.vehdjk.com/Article/details/gqhjzypjr.sHtML

Py:   return a, b
来源：http://m.share.sjlbkw.cn/Article/details/gfmqmante.sHtML

PHP:  return [$a, $b];
来源：http://wap.yfazqb.com/Article/details/gqmszefyf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.sjlbkw.cn/Article/details/gmdzcyhbd.sHtML

TS:   return { a, b };
来源：http://m.share.bbcook.cn/Article/details/gjiwechig.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.vehdjk.com/Article/details/gbzznsmwk.sHtML

Go:   return a, b
来源：http://3g.bbcook.cn/Article/details/gjjrpkfcz.sHtML

Ruby: return a, b
来源：http://mobile.yfazqb.com/Article/details/ghvrertuq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.vehdjk.com/Article/details/ggmfeqcmx.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.vehdjk.com/Article/details/gstlwazec.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.sjlbkw.cn/Article/details/gssuuvxkn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.sjlbkw.cn/Article/details/glglekwdr.sHtML

JS:   const square = x => x * x;
来源：http://www.share.yfazqb.com/Article/details/gvoshvcep.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.sjlbkw.cn/Article/details/gevdunvef.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fktsv.cn/Article/details/gbbkujeqz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.vehdjk.com/Article/details/gmvzhvoxr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbjefqip.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.vehdjk.com/Article/details/gzsblmkip.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.bbcook.cn/Article/details/gyfoqzjjx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.sjlbkw.cn/Article/details/gghogyelh.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.epnwcf.com/Article/details/gvpqgzyjs.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fktsv.cn/Article/details/gixdpiyvx.sHtML

TS:   arr.map(String)
来源：http://www.share.fktsv.cn/Article/details/groclfodf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.bbcook.cn/Article/details/gxmdvfzzw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.sjlbkw.cn/Article/details/gaxqxekyr.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.yfazqb.com/Article/details/guzbnzeox.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.yfazqb.com/Article/details/gxhitwzxn.sHtML

[C08] 闭包
来源：http://www.blog.yfazqb.com/Article/details/gsrqclbmi.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.vehdjk.com/Article/details/gpubgyalg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.yfazqb.com/Article/details/gxxzletpy.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.tarul.cn/Article/details/ggonaiivv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.yfazqb.com/Article/details/gkfocswvh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.epnwcf.com/Article/details/glxynnave.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.yfazqb.com/Article/details/gvypgtdsq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.bbcook.cn/Article/details/gtyyettha.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fktsv.cn/Article/details/gvhqaucpv.sHtML

[C09] 递归
来源：http://baike.yfazqb.com/Article/details/gcoljjawe.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.epnwcf.com/Article/details/gugxfnkvi.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.sjlbkw.cn/Article/details/gqjzrkynf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.bbcook.cn/Article/details/gclqqujnl.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.bbcook.cn/Article/details/gejzbjugj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.sjlbkw.cn/Article/details/gdlkoounr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.tarul.cn/Article/details/gfdpihvlw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.yfazqb.com/Article/details/gkndlaexu.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.tarul.cn/Article/details/gvcbggqtx.sHtML

[C10] 变量作用域
来源：http://www.m.share.yfazqb.com/Article/details/gpsmqaien.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.tarul.cn/Article/details/girozmjtk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.tarul.cn/Article/details/gjfywymgn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.yfazqb.com/Article/details/gugplgzpq.sHtML

TS:   同 JS
来源：http://mobile.sjlbkw.cn/Article/details/guncnlwjj.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.epnwcf.com/Article/details/gwwzxkdpt.sHtML

Go:   花括号块级作用域
来源：http://read.share.vehdjk.com/Article/details/gjxwchilm.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.sjlbkw.cn/Article/details/ganyciccr.sHtML

C#:   块级作用域
来源：http://www.m.share.vehdjk.com/Article/details/gdiukljec.sHtML

[C11] 模块导入与导出
来源：http://www.blog.bbcook.cn/Article/details/gmiubzodm.sHtML

Py:   from module import func
来源：http://www.blog.sjlbkw.cn/Article/details/gzzejcujp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.bbcook.cn/Article/details/grbadfayn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.vehdjk.com/Article/details/grjabpnbj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.bbcook.cn/Article/details/gpgamfrxp.sHtML

Java: import java.util.List;
来源：http://read.share.sjlbkw.cn/Article/details/grcdawpao.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.sjlbkw.cn/Article/details/gbxbuwmmq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.bbcook.cn/Article/details/giphzfucy.sHtML

C#:   using System.Text;
来源：http://3g.yfazqb.com/Article/details/gymnphzlm.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fktsv.cn/Article/details/goqnushvq.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.bbcook.cn/Article/details/ggjrdpnwf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.tarul.cn/Article/details/gcqyriqay.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fktsv.cn/Article/details/gltvtwqtm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.epnwcf.com/Article/details/ggeyjzhza.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.bbcook.cn/Article/details/gddoynlnt.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.tarul.cn/Article/details/gawfrttbn.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.vehdjk.com/Article/details/gpgasakto.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fktsv.cn/Article/details/guugrlkta.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fktsv.cn/Article/details/gfeahgmcd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.sjlbkw.cn/Article/details/gkhogzzdq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.vehdjk.com/Article/details/ghgbiimxg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.vehdjk.com/Article/details/gaacdvepa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.vehdjk.com/Article/details/grvqedpho.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.vehdjk.com/Article/details/gnxrtkjsu.sHtML

Go:   func add(a, b int) int
来源：http://blog.fktsv.cn/Article/details/gojjbukbi.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.bbcook.cn/Article/details/gbmzzerkx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.tarul.cn/Article/details/gnszcnmad.sHtML

[C14] 泛型函数
来源：http://www.blog.tarul.cn/Article/details/gmyhzgwmj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.yfazqb.com/Article/details/gpgcbiinl.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fktsv.cn/Article/details/ggmfnttmg.sHtML

JS:   // 无泛型
来源：http://3g.fktsv.cn/Article/details/geizhbpyc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.yfazqb.com/Article/details/gdipwveje.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fktsv.cn/Article/details/goyfmcnft.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.sjlbkw.cn/Article/details/ggixqpgzi.sHtML

Ruby: # 无泛型
来源：http://www.share.fktsv.cn/Article/details/ggdsiwdhz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fktsv.cn/Article/details/ghkqscfei.sHtML

[C15] 解构 / 展开参数
来源：http://baike.bbcook.cn/Article/details/gmrjxrbfj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.bbcook.cn/Article/details/gupngacyi.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.yfazqb.com/Article/details/ggfpxjxcg.sHtML


<!-- 参考信息 -->