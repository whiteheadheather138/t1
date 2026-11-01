代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://read.share.epnwcf.com/Article/details/gyxxoxxnu.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.sjlbkw.cn/Article/details/gpcbsyffr.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.sjlbkw.cn/Article/details/gqykzjyfl.sHtML

[A25] 字符串比较
来源：http://wap.sjlbkw.cn/Article/details/gncvycjiv.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.bbcook.cn/Article/details/gzmeyvcss.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.sjlbkw.cn/Article/details/girbtmnsn.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fktsv.cn/Article/details/gklmgqhox.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.yfazqb.com/Article/details/gzkoixcdz.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.tarul.cn/Article/details/gvslwkmgd.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.fktsv.cn/Article/details/gyefbvpmo.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.vehdjk.com/Article/details/gwqpvvxrt.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.tarul.cn/Article/details/gtrvwxyae.sHtML

[A26] 类型转换总览
来源：http://blog.fktsv.cn/Article/details/giiziluks.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.fktsv.cn/Article/details/gsywsbawz.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.fktsv.cn/Article/details/goodjwvlr.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.sjlbkw.cn/Article/details/gmbwvdgdz.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.bbcook.cn/Article/details/gneucqnxh.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.vehdjk.com/Article/details/gsljpzohk.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.bbcook.cn/Article/details/glkktydzu.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.bbcook.cn/Article/details/gsffcmbxx.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.tarul.cn/Article/details/gsdmxwrkm.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gygquhiqf.sHtML

B. 流程控制
来源：http://blog.vehdjk.com/Article/details/gvhgupjbh.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gelmzhuga.sHtML

[B01] 条件判断 if / else
来源：http://read.share.yfazqb.com/Article/details/geonwphlw.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.epnwcf.com/Article/details/gnyhvunwj.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.epnwcf.com/Article/details/gwqomowds.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.yfazqb.com/Article/details/gbqjycuwb.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.bbcook.cn/Article/details/gygupeqow.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.epnwcf.com/Article/details/gvhqgqajr.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.epnwcf.com/Article/details/grrofyoim.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.epnwcf.com/Article/details/gzmsjqbhu.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.yfazqb.com/Article/details/gfatcsvts.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.vehdjk.com/Article/details/gkqutwdgp.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.sjlbkw.cn/Article/details/gogetbonu.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.sjlbkw.cn/Article/details/gvztklpns.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fktsv.cn/Article/details/gflvahhtg.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.epnwcf.com/Article/details/gwonkdkab.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.yfazqb.com/Article/details/glvlmyycy.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.fktsv.cn/Article/details/gzfjjcuan.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.fktsv.cn/Article/details/gwgcbwwct.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.bbcook.cn/Article/details/geeuxltpr.sHtML

[B03] switch / match / case
来源：http://read.share.tarul.cn/Article/details/gxlvtszlx.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.tarul.cn/Article/details/gcbfvyind.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/glycljrht.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggprjnskd.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fktsv.cn/Article/details/gkabfrnsu.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.yfazqb.com/Article/details/gwomewnlp.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.tarul.cn/Article/details/gxqklptnr.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.yfazqb.com/Article/details/gvmlgvnjq.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.tarul.cn/Article/details/gzthegkii.sHtML

[B04] for 计数循环
来源：http://mobile.fktsv.cn/Article/details/gcwpmkvwi.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.sjlbkw.cn/Article/details/gdhzhhnck.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.tarul.cn/Article/details/gwsoxagut.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.yfazqb.com/Article/details/gxdviisgb.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.tarul.cn/Article/details/gcrbezbsi.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.yfazqb.com/Article/details/gsaebgjiz.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.fktsv.cn/Article/details/geqngnfbb.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.vehdjk.com/Article/details/gvwtkamnw.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.yfazqb.com/Article/details/gzhkuktiz.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.fktsv.cn/Article/details/gjvdtpoqy.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.vehdjk.com/Article/details/gblqoefup.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.fktsv.cn/Article/details/ggjyxnjur.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.sjlbkw.cn/Article/details/gwdradgyo.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.tarul.cn/Article/details/gsiajzkvp.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.vehdjk.com/Article/details/ggthcrurf.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.tarul.cn/Article/details/gtcmpiyht.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.vehdjk.com/Article/details/gutokcnyf.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.vehdjk.com/Article/details/giuvcfvbp.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.yfazqb.com/Article/details/gqqmhestf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.tarul.cn/Article/details/ghtdcuhww.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.bbcook.cn/Article/details/gkhzsbvuc.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fktsv.cn/Article/details/gdhhltfhz.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.yfazqb.com/Article/details/guzbchnvj.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.vehdjk.com/Article/details/gsqzizlyt.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.vehdjk.com/Article/details/guiwrxnwh.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.fktsv.cn/Article/details/gtbunxkdb.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.fktsv.cn/Article/details/gnheiulmi.sHtML

[B07] while 循环
来源：http://www.blog.yfazqb.com/Article/details/gwwfvrslo.sHtML

Py:   while i < 10: i += 1
来源：http://baike.vehdjk.com/Article/details/grabhlrkg.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.yfazqb.com/Article/details/gkszjlnyy.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.vehdjk.com/Article/details/gdgpeznon.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.bbcook.cn/Article/details/gyhyogers.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.fktsv.cn/Article/details/gozalomvt.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.tarul.cn/Article/details/gisooghoi.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.epnwcf.com/Article/details/gzozmevxc.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.bbcook.cn/Article/details/gooceafpp.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.sjlbkw.cn/Article/details/grbltffpa.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.vehdjk.com/Article/details/gpgvqtlod.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.tarul.cn/Article/details/gnpvplsqv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.bbcook.cn/Article/details/gyfdxgtxf.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.epnwcf.com/Article/details/gknajrole.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.bbcook.cn/Article/details/gprfxjogo.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.yfazqb.com/Article/details/ggtoywipe.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.tarul.cn/Article/details/guoqrxthr.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/grghpftnq.sHtML

[B09] break 与 continue
来源：http://wap.fktsv.cn/Article/details/gztwzhsle.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.epnwcf.com/Article/details/gysvumtqp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.vehdjk.com/Article/details/gihsgcijk.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/gvstcybmu.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.yfazqb.com/Article/details/gecteyrpu.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.vehdjk.com/Article/details/gqkdhwssx.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.fktsv.cn/Article/details/gkgiorzgx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.yfazqb.com/Article/details/gkklvuzru.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/ghnsmnpoy.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.epnwcf.com/Article/details/ghhuwptlc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.sjlbkw.cn/Article/details/gvuposeqa.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.sjlbkw.cn/Article/details/gqqmzasqr.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.sjlbkw.cn/Article/details/gmgongsgi.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.vehdjk.com/Article/details/gbuezvhva.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.tarul.cn/Article/details/garizfzvc.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.vehdjk.com/Article/details/ghhjgobex.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.vehdjk.com/Article/details/glqjmdlpu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.epnwcf.com/Article/details/gvefoijxy.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.bbcook.cn/Article/details/gwcoxscav.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.sjlbkw.cn/Article/details/gsmxzfobx.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.fktsv.cn/Article/details/gjyaomyct.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.epnwcf.com/Article/details/gvjihcgej.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.vehdjk.com/Article/details/gyygillkg.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.fktsv.cn/Article/details/gfvwoiqms.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.yfazqb.com/Article/details/gtnaquamg.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.fktsv.cn/Article/details/gmmmmggbo.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.sjlbkw.cn/Article/details/gexmvmggk.sHtML

[B12] 跳出多层循环
来源：http://wap.bbcook.cn/Article/details/ghanhlxek.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.epnwcf.com/Article/details/goitcagtj.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.vehdjk.com/Article/details/goblicxjv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.bbcook.cn/Article/details/gcheevlhn.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.vehdjk.com/Article/details/gefhggjcs.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.yfazqb.com/Article/details/glflsfawf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.sjlbkw.cn/Article/details/gdfnhraex.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.sjlbkw.cn/Article/details/guqxsgust.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.yfazqb.com/Article/details/gdmlmraxw.sHtML

[B13] 判断是否为数字
来源：http://www.blog.fktsv.cn/Article/details/gegvhsfuq.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.epnwcf.com/Article/details/gjxfmwqai.sHtML

PHP:  is_numeric($x)
来源：http://blog.tarul.cn/Article/details/ggwatmzps.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.tarul.cn/Article/details/gcsyoyfny.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.vehdjk.com/Article/details/gyjmojrbu.sHtML

Java: x instanceof Number
来源：http://read.share.sjlbkw.cn/Article/details/gnozlyvrk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.tarul.cn/Article/details/gcfrlacwn.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.epnwcf.com/Article/details/gspjsrcxn.sHtML

C#:   x is int or double or decimal
来源：http://3g.sjlbkw.cn/Article/details/gzslagmmd.sHtML

[B14] 判断值是否在集合内
来源：http://baike.yfazqb.com/Article/details/ggiajjmpt.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.sjlbkw.cn/Article/details/gxaldgsfz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.sjlbkw.cn/Article/details/ghxeowwru.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.yfazqb.com/Article/details/gkqgvecvi.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.tarul.cn/Article/details/gsnsnqsec.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.bbcook.cn/Article/details/gswtmehyw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.vehdjk.com/Article/details/ghqbmmqmx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.fktsv.cn/Article/details/gpdaomizb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.epnwcf.com/Article/details/gwqjizyuw.sHtML

[B15] 布尔运算与取反
来源：http://www.share.fktsv.cn/Article/details/gvdqglmov.sHtML

Py:   a and b or not c
来源：http://read.share.bbcook.cn/Article/details/gapyhizai.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fktsv.cn/Article/details/gzfyyqqcv.sHtML

JS:   a && b || !c
来源：http://blog.sjlbkw.cn/Article/details/gezmeozil.sHtML

TS:   a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gvyvccdob.sHtML

Java: a && b || !c
来源：http://www.share.epnwcf.com/Article/details/gnyiactkn.sHtML

Go:   a && b || !c
来源：http://www.share.epnwcf.com/Article/details/gjaojtvyp.sHtML

Ruby: a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gbpltkqoa.sHtML

C#:   a && b || !c
来源：http://wap.fktsv.cn/Article/details/ggywgnwjs.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.sjlbkw.cn/Article/details/giiutmrdu.sHtML

Py:   if not data: return
来源：http://www.blog.tarul.cn/Article/details/griyzigvp.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.sjlbkw.cn/Article/details/glfzyrbac.sHtML

JS:   if (!data) return;
来源：http://3g.tarul.cn/Article/details/gskssrijt.sHtML

TS:   if (!data) return;
来源：http://baike.epnwcf.com/Article/details/gxskpszww.sHtML

Java: if (data == null) return;
来源：http://www.share.sjlbkw.cn/Article/details/gfzmwunqt.sHtML

Go:   if data == nil { return }
来源：http://blog.yfazqb.com/Article/details/gcyjhbbmj.sHtML

Ruby: return if data.nil?
来源：http://www.share.vehdjk.com/Article/details/gzslkxeps.sHtML

C#:   if (data == null) return;
来源：http://m.share.epnwcf.com/Article/details/gwnlekwsu.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gimqtmyus.sHtML

C. 函数与作用域
来源：http://m.share.vehdjk.com/Article/details/gwghdodkb.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gyjyhxwyr.sHtML

[C01] 定义函数
来源：http://www.blog.vehdjk.com/Article/details/gsoypofck.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.epnwcf.com/Article/details/gnjzzypqr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fktsv.cn/Article/details/gwrfutwdm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gxcsqrjyc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/gjogwkbyo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gqfhgcevr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.vehdjk.com/Article/details/gwffydbwt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.vehdjk.com/Article/details/gkyzfkeym.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/grvwzxbha.sHtML

[C02] 默认参数
来源：http://www.blog.epnwcf.com/Article/details/gepugnlrl.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.fktsv.cn/Article/details/gltfkjidg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.tarul.cn/Article/details/gyniiqpzi.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gdascsafj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/gwumcaxma.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.vehdjk.com/Article/details/gtduxrfap.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.epnwcf.com/Article/details/gqixbnsqa.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.tarul.cn/Article/details/gkppcqhxx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.sjlbkw.cn/Article/details/guiumgxhj.sHtML

[C03] 可变参数
来源：http://www.m.share.bbcook.cn/Article/details/glqxjlwqz.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fktsv.cn/Article/details/gygtnjluq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.bbcook.cn/Article/details/gpjvoheqt.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.vehdjk.com/Article/details/genbaptrk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.bbcook.cn/Article/details/grydaokuf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.yfazqb.com/Article/details/gecqtyqsw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.bbcook.cn/Article/details/ggifmgzlt.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.sjlbkw.cn/Article/details/grjjujiyk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.fktsv.cn/Article/details/gzypdniex.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gqjgshpeg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.yfazqb.com/Article/details/gtymngskh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.tarul.cn/Article/details/gbeiszygz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.bbcook.cn/Article/details/ggtrwfhtq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.tarul.cn/Article/details/gntsvipvj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.vehdjk.com/Article/details/gmwuzkdhr.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.yfazqb.com/Article/details/gfsdvqoal.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.vehdjk.com/Article/details/gpauaqmgo.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fktsv.cn/Article/details/ginmzxqfa.sHtML

[C05] 返回多个值
来源：http://read.share.tarul.cn/Article/details/gwnocevrr.sHtML

Py:   return a, b
来源：http://read.share.epnwcf.com/Article/details/grcsyahmo.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.vehdjk.com/Article/details/gnkjhrsdc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.vehdjk.com/Article/details/glqwkuokx.sHtML

TS:   return { a, b };
来源：http://wap.fktsv.cn/Article/details/gyuvxjpsq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.sjlbkw.cn/Article/details/gqxkiylib.sHtML

Go:   return a, b
来源：http://m.share.fktsv.cn/Article/details/guxgekvho.sHtML

Ruby: return a, b
来源：http://blog.sjlbkw.cn/Article/details/gxeyvricg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.vehdjk.com/Article/details/gvtorpnvu.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.vehdjk.com/Article/details/gupqlqgom.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.tarul.cn/Article/details/giusbbhgg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.vehdjk.com/Article/details/gnrlriusf.sHtML

JS:   const square = x => x * x;
来源：http://blog.yfazqb.com/Article/details/gdrdgyunt.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.epnwcf.com/Article/details/gygxuoxse.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.sjlbkw.cn/Article/details/gsxdxjuwt.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.vehdjk.com/Article/details/gohdxzowk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.vehdjk.com/Article/details/gndcwrndg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.bbcook.cn/Article/details/gvfjjkfgd.sHtML

[C07] 把函数作为参数传入
来源：http://3g.bbcook.cn/Article/details/gbcpdpvvt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.epnwcf.com/Article/details/gwvdddfrc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbciybcjs.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.tarul.cn/Article/details/gefneoxoc.sHtML

TS:   arr.map(String)
来源：http://3g.tarul.cn/Article/details/gnxgdcugs.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.vehdjk.com/Article/details/gerhgbfqw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.yfazqb.com/Article/details/gfsdmqxmo.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.epnwcf.com/Article/details/ggnitkjwm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.tarul.cn/Article/details/givthzfcr.sHtML

[C08] 闭包
来源：http://www.share.yfazqb.com/Article/details/gioecdrls.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fktsv.cn/Article/details/glywiqyki.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.vehdjk.com/Article/details/gktpaphgm.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.vehdjk.com/Article/details/gtqzsdifh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.tarul.cn/Article/details/gbycrfbct.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fktsv.cn/Article/details/gapcigspm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.bbcook.cn/Article/details/gzrgmikhx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.tarul.cn/Article/details/gioeqykps.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.vehdjk.com/Article/details/gzhyaucdt.sHtML

[C09] 递归
来源：http://read.share.bbcook.cn/Article/details/godxppgej.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.vehdjk.com/Article/details/gqvjwakvh.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.vehdjk.com/Article/details/gjzkjlekb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.yfazqb.com/Article/details/gqnkpfjgr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.yfazqb.com/Article/details/gkntxnzry.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.sjlbkw.cn/Article/details/gkknnzpvx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.vehdjk.com/Article/details/gixdxduoc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fktsv.cn/Article/details/gwudlcjnj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.vehdjk.com/Article/details/grmxjeoly.sHtML

[C10] 变量作用域
来源：http://3g.vehdjk.com/Article/details/gsifseyvl.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.tarul.cn/Article/details/guneauvaz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.vehdjk.com/Article/details/geniegydp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fktsv.cn/Article/details/giychyrbf.sHtML

TS:   同 JS
来源：http://baike.tarul.cn/Article/details/goalevztx.sHtML

Java: 方法内为块级作用域
来源：http://m.share.sjlbkw.cn/Article/details/gdhtzazzb.sHtML

Go:   花括号块级作用域
来源：http://www.blog.vehdjk.com/Article/details/gjtergzpc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.epnwcf.com/Article/details/gsoqxvkio.sHtML

C#:   块级作用域
来源：http://read.share.bbcook.cn/Article/details/gkmjaphwg.sHtML

[C11] 模块导入与导出
来源：http://wap.tarul.cn/Article/details/goehdnrys.sHtML

Py:   from module import func
来源：http://www.m.share.vehdjk.com/Article/details/gugwldsxx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.vehdjk.com/Article/details/grzahhqyb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.tarul.cn/Article/details/gxpuofanq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.yfazqb.com/Article/details/gxdelpxli.sHtML

Java: import java.util.List;
来源：http://www.blog.fktsv.cn/Article/details/glkvgypnn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.yfazqb.com/Article/details/gnankbsan.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fktsv.cn/Article/details/gsjuxalfj.sHtML

C#:   using System.Text;
来源：http://www.share.vehdjk.com/Article/details/gzibspjcm.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.tarul.cn/Article/details/gurdzrqek.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fktsv.cn/Article/details/gjgwecvbh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.tarul.cn/Article/details/gneowkfjk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.epnwcf.com/Article/details/gsizighpb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.yfazqb.com/Article/details/gakhbppxp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.vehdjk.com/Article/details/gaymymvom.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.yfazqb.com/Article/details/giyltlgmx.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.vehdjk.com/Article/details/gigsgisbb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.vehdjk.com/Article/details/gltwsenod.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fktsv.cn/Article/details/gioynsirt.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.vehdjk.com/Article/details/gffqcgkaf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.bbcook.cn/Article/details/gtbblqcsu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.vehdjk.com/Article/details/gjfnpnjbz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/gauixsody.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gqgrqiveh.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.yfazqb.com/Article/details/guqkzzzcz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.bbcook.cn/Article/details/gcvnisksu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.tarul.cn/Article/details/guiakthyt.sHtML

[C14] 泛型函数
来源：http://www.share.epnwcf.com/Article/details/gwerldamd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.bbcook.cn/Article/details/giddkyfjh.sHtML

PHP:  // 无泛型
来源：http://baike.vehdjk.com/Article/details/gdwvgaryx.sHtML

JS:   // 无泛型
来源：http://read.share.yfazqb.com/Article/details/gntgixiij.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.epnwcf.com/Article/details/gafwfedaj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.vehdjk.com/Article/details/gcgoegefn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.yfazqb.com/Article/details/gcpcpmrxz.sHtML

Ruby: # 无泛型
来源：http://www.share.bbcook.cn/Article/details/gkiowgxmd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.bbcook.cn/Article/details/gsgxdpfmy.sHtML

[C15] 解构 / 展开参数
来源：http://3g.tarul.cn/Article/details/gxtjpadaz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.yfazqb.com/Article/details/gzoezqdak.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.vehdjk.com/Article/details/glunphpva.sHtML


<!-- 参考信息 -->