代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://m.share.bbcook.cn/Article/details/gxsomzmmb.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.epnwcf.com/Article/details/ghfombiyz.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.bbcook.cn/Article/details/gmfcgyvij.sHtML

[A25] 字符串比较
来源：http://blog.tarul.cn/Article/details/gvqfntohu.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.tarul.cn/Article/details/grspscusp.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.tarul.cn/Article/details/ggyzjsdlw.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.tarul.cn/Article/details/gdejxcuag.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.yfazqb.com/Article/details/gwbybyvyn.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.tarul.cn/Article/details/ghfkydqvd.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.tarul.cn/Article/details/gxhxpbfhv.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.bbcook.cn/Article/details/gmvgtlwcx.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.vehdjk.com/Article/details/gzksrnvkh.sHtML

[A26] 类型转换总览
来源：http://www.share.yfazqb.com/Article/details/giafzqddj.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.epnwcf.com/Article/details/gjwhftxxo.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.yfazqb.com/Article/details/gcunnokdr.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.fktsv.cn/Article/details/gxkffzcmh.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.epnwcf.com/Article/details/gnlelqidt.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.bbcook.cn/Article/details/gmcmchots.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.tarul.cn/Article/details/gbgbssqgm.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.yfazqb.com/Article/details/grkbjklbj.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.bbcook.cn/Article/details/gehtvxhgs.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gzauktpoj.sHtML

B. 流程控制
来源：http://wap.vehdjk.com/Article/details/gehrwwdpj.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gbhejgyeo.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.sjlbkw.cn/Article/details/gtvgwkffx.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.yfazqb.com/Article/details/gbkvsbvqn.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.fktsv.cn/Article/details/getgapcqd.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.tarul.cn/Article/details/gddnezrgg.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.bbcook.cn/Article/details/gxllxuqot.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.sjlbkw.cn/Article/details/gftvdqvrs.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.bbcook.cn/Article/details/gxabwstue.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.tarul.cn/Article/details/ghqortsmi.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.tarul.cn/Article/details/gmzvrxhij.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.tarul.cn/Article/details/gqgivmvbs.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.sjlbkw.cn/Article/details/gcavhabnp.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.vehdjk.com/Article/details/gxqflzgdx.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.vehdjk.com/Article/details/gzcvvvuzs.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.tarul.cn/Article/details/gnajppjui.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.sjlbkw.cn/Article/details/glpbblzee.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.tarul.cn/Article/details/guyuzyord.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.bbcook.cn/Article/details/gbekrrfvc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fktsv.cn/Article/details/gusuuxgft.sHtML

[B03] switch / match / case
来源：http://wap.vehdjk.com/Article/details/gvsrtzgyf.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.sjlbkw.cn/Article/details/gnxczdzut.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.tarul.cn/Article/details/gsuiayfwe.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.sjlbkw.cn/Article/details/gpswswubk.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.epnwcf.com/Article/details/guhfuglxj.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.fktsv.cn/Article/details/gyodirfhj.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.bbcook.cn/Article/details/giigbcazm.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.sjlbkw.cn/Article/details/glxdqlsfd.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.fktsv.cn/Article/details/gkfwovhyo.sHtML

[B04] for 计数循环
来源：http://mobile.tarul.cn/Article/details/gdxwpmmih.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.yfazqb.com/Article/details/gsqjmitxa.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.tarul.cn/Article/details/grmqkdfhm.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fktsv.cn/Article/details/gnsgicdbv.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.tarul.cn/Article/details/gtdijeyqg.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.tarul.cn/Article/details/ghshpoiwx.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.bbcook.cn/Article/details/gawlaxhjl.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.vehdjk.com/Article/details/gpmhbgkxj.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.sjlbkw.cn/Article/details/grbazizbk.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.bbcook.cn/Article/details/goybxlpjt.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.epnwcf.com/Article/details/gcccvvxmm.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.yfazqb.com/Article/details/gszobetvf.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.sjlbkw.cn/Article/details/giatlsero.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.yfazqb.com/Article/details/gubehusrh.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.bbcook.cn/Article/details/gbmfymuxp.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.yfazqb.com/Article/details/gealoedps.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.yfazqb.com/Article/details/gkalhifuc.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.vehdjk.com/Article/details/gzgoqyqrg.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.epnwcf.com/Article/details/gpavtwgtr.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.tarul.cn/Article/details/gqfyulkdz.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.fktsv.cn/Article/details/ggbjlobhl.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.tarul.cn/Article/details/gkfysjwpd.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.epnwcf.com/Article/details/gadqdncrh.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.bbcook.cn/Article/details/goeebzdwh.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.epnwcf.com/Article/details/gxiubrggd.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.tarul.cn/Article/details/gnlowkwci.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.fktsv.cn/Article/details/gasztiweb.sHtML

[B07] while 循环
来源：http://www.blog.fktsv.cn/Article/details/guwcmtqvz.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.yfazqb.com/Article/details/gxguyvcdh.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.bbcook.cn/Article/details/gfgqcqfoe.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.bbcook.cn/Article/details/gzgvfyksd.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.fktsv.cn/Article/details/gmggctzez.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.vehdjk.com/Article/details/gnxusdxsq.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.bbcook.cn/Article/details/gnrcggoku.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.sjlbkw.cn/Article/details/gtpvmjqtv.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.fktsv.cn/Article/details/glbtcelvo.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.tarul.cn/Article/details/ggikrmmyf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.tarul.cn/Article/details/grmtnopof.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.vehdjk.com/Article/details/gmnfajryc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.yfazqb.com/Article/details/gkrahqwxy.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.epnwcf.com/Article/details/gaimoqxfg.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.sjlbkw.cn/Article/details/ghtvrctyp.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.yfazqb.com/Article/details/gtyxytjbo.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.tarul.cn/Article/details/gbbiuntct.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.vehdjk.com/Article/details/gvhadiymd.sHtML

[B09] break 与 continue
来源：http://baike.fktsv.cn/Article/details/gqnfzqkgj.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.bbcook.cn/Article/details/gqdxrkkbx.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.sjlbkw.cn/Article/details/gijxgiqwc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.tarul.cn/Article/details/gtryycfcr.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fktsv.cn/Article/details/gpftfpiyi.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.yfazqb.com/Article/details/gjgainrkt.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.tarul.cn/Article/details/gpayyjmob.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.bbcook.cn/Article/details/gehuptnbz.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.epnwcf.com/Article/details/glnwsrkxq.sHtML

[B10] 遍历同时拿索引
来源：http://baike.sjlbkw.cn/Article/details/ggjgbscam.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.sjlbkw.cn/Article/details/gswsvzkzq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.epnwcf.com/Article/details/gmsbwbcdi.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.sjlbkw.cn/Article/details/geifcgmcb.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.bbcook.cn/Article/details/gwqnsjdhl.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.sjlbkw.cn/Article/details/giukivdxe.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.fktsv.cn/Article/details/gnnrvskhk.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.sjlbkw.cn/Article/details/gvlgehdni.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.bbcook.cn/Article/details/gsloyzulo.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.sjlbkw.cn/Article/details/gkeuhgzpv.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.vehdjk.com/Article/details/gkatgohvy.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.epnwcf.com/Article/details/gjrnjsfnk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.bbcook.cn/Article/details/gqhayixxy.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.epnwcf.com/Article/details/gkngwidim.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxqryqnmh.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.fktsv.cn/Article/details/gkxedlkpq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.sjlbkw.cn/Article/details/gyjwxcwcw.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.epnwcf.com/Article/details/gcivatxko.sHtML

[B12] 跳出多层循环
来源：http://www.share.yfazqb.com/Article/details/gjqkvdzzj.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.tarul.cn/Article/details/gyyxkqheq.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.yfazqb.com/Article/details/gyoewaudw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.bbcook.cn/Article/details/gprzfcuev.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.tarul.cn/Article/details/gfkjqhphp.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.sjlbkw.cn/Article/details/grokyqbsh.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.epnwcf.com/Article/details/gpvsjeujk.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.fktsv.cn/Article/details/gkmzpvuph.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.yfazqb.com/Article/details/gqjumwbhf.sHtML

[B13] 判断是否为数字
来源：http://m.share.tarul.cn/Article/details/gvracvlyy.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.bbcook.cn/Article/details/gyfldjvei.sHtML

PHP:  is_numeric($x)
来源：http://www.share.yfazqb.com/Article/details/gqiroyand.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fktsv.cn/Article/details/gvacavmmh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.epnwcf.com/Article/details/gcksgttwq.sHtML

Java: x instanceof Number
来源：http://www.m.share.fktsv.cn/Article/details/gnyfkjrlh.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.tarul.cn/Article/details/gwyfnhkrx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.vehdjk.com/Article/details/gezhybnsh.sHtML

C#:   x is int or double or decimal
来源：http://www.share.tarul.cn/Article/details/gfyqzvhaa.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.yfazqb.com/Article/details/gezbzexnn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.bbcook.cn/Article/details/gcfksjeiq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.tarul.cn/Article/details/gduyotgjd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.epnwcf.com/Article/details/gryirrmdl.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.yfazqb.com/Article/details/gihjhfuvn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fktsv.cn/Article/details/gsvlzwwho.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.bbcook.cn/Article/details/gyowpwqld.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.yfazqb.com/Article/details/gzsilitxe.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.tarul.cn/Article/details/gdwqqlavb.sHtML

[B15] 布尔运算与取反
来源：http://3g.vehdjk.com/Article/details/gcktutezp.sHtML

Py:   a and b or not c
来源：http://www.share.fktsv.cn/Article/details/gfsaspgqa.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.epnwcf.com/Article/details/gpvolcrgq.sHtML

JS:   a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/gacvptztx.sHtML

TS:   a && b || !c
来源：http://m.share.vehdjk.com/Article/details/gmdhpzofh.sHtML

Java: a && b || !c
来源：http://m.share.tarul.cn/Article/details/gfclerlmg.sHtML

Go:   a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gnpnmiftq.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/gflejoatk.sHtML

C#:   a && b || !c
来源：http://mobile.bbcook.cn/Article/details/gteopghqw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.epnwcf.com/Article/details/gdjqzkegi.sHtML

Py:   if not data: return
来源：http://blog.tarul.cn/Article/details/ghxyvukvd.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.fktsv.cn/Article/details/gdhblipli.sHtML

JS:   if (!data) return;
来源：http://m.share.vehdjk.com/Article/details/gawwglaaw.sHtML

TS:   if (!data) return;
来源：http://wap.fktsv.cn/Article/details/gfswepfko.sHtML

Java: if (data == null) return;
来源：http://www.blog.sjlbkw.cn/Article/details/ggwdyanoq.sHtML

Go:   if data == nil { return }
来源：http://m.share.sjlbkw.cn/Article/details/guckvwzix.sHtML

Ruby: return if data.nil?
来源：http://read.share.vehdjk.com/Article/details/grffpmqfx.sHtML

C#:   if (data == null) return;
来源：http://3g.epnwcf.com/Article/details/guvjfaocj.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gufuybeoe.sHtML

C. 函数与作用域
来源：http://baike.fktsv.cn/Article/details/gxzijheod.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/geiuetvmv.sHtML

[C01] 定义函数
来源：http://blog.vehdjk.com/Article/details/gnccohzcp.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.tarul.cn/Article/details/gqgtgguov.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/gfdznxfwj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/gzubksmub.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdrxjnpiu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.yfazqb.com/Article/details/gdwwpvihv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.tarul.cn/Article/details/gtfcbznpi.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.fktsv.cn/Article/details/grngjvzlb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.tarul.cn/Article/details/guzbakdak.sHtML

[C02] 默认参数
来源：http://www.m.share.vehdjk.com/Article/details/giejsprek.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.yfazqb.com/Article/details/gxltpuglf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.sjlbkw.cn/Article/details/gmvencqsp.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.yfazqb.com/Article/details/gulbsficz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/gqznwxvza.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.bbcook.cn/Article/details/gfjqbfyqr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fktsv.cn/Article/details/gvmnmecap.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.tarul.cn/Article/details/gmcmqkgra.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.tarul.cn/Article/details/gmzwhayzn.sHtML

[C03] 可变参数
来源：http://www.share.tarul.cn/Article/details/gbxwzoggg.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.vehdjk.com/Article/details/gemktbjja.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.yfazqb.com/Article/details/gllujnslt.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fktsv.cn/Article/details/gbqhabsvr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.sjlbkw.cn/Article/details/glnhravqb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fktsv.cn/Article/details/guxvfnuvt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.sjlbkw.cn/Article/details/gjqstarcf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.tarul.cn/Article/details/gymuqftwt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.tarul.cn/Article/details/gxjbobzqm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.fktsv.cn/Article/details/gcvbpfwcm.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.sjlbkw.cn/Article/details/gwmgetaop.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.tarul.cn/Article/details/gktattyrq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.yfazqb.com/Article/details/ghnhdjgdf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.tarul.cn/Article/details/gquzaqzkl.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.tarul.cn/Article/details/gvsnalybu.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fktsv.cn/Article/details/gkximoapn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fktsv.cn/Article/details/ghuntswmu.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fktsv.cn/Article/details/gbogkgojc.sHtML

[C05] 返回多个值
来源：http://wap.sjlbkw.cn/Article/details/gejjrzdtf.sHtML

Py:   return a, b
来源：http://read.share.epnwcf.com/Article/details/gyygxsobv.sHtML

PHP:  return [$a, $b];
来源：http://m.share.tarul.cn/Article/details/gwgdnnurg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.vehdjk.com/Article/details/gkgztgvwy.sHtML

TS:   return { a, b };
来源：http://www.share.bbcook.cn/Article/details/gzfalvxbb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.yfazqb.com/Article/details/giyxwxkhs.sHtML

Go:   return a, b
来源：http://www.m.share.epnwcf.com/Article/details/gikhfiagq.sHtML

Ruby: return a, b
来源：http://3g.vehdjk.com/Article/details/gmvhjohnm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.yfazqb.com/Article/details/gziokrkzc.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.sjlbkw.cn/Article/details/gahaqsbgk.sHtML

Py:   square = lambda x: x * x
来源：http://baike.bbcook.cn/Article/details/gzuirdnkl.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.sjlbkw.cn/Article/details/gsxqxadoz.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.tarul.cn/Article/details/gczwqzpyu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.tarul.cn/Article/details/gmjrbymnm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.bbcook.cn/Article/details/gixhikrku.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.vehdjk.com/Article/details/gnusbgwbz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.tarul.cn/Article/details/gxcujkbsj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.sjlbkw.cn/Article/details/gvkvarhxt.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.bbcook.cn/Article/details/gniimovuw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.epnwcf.com/Article/details/gzpcrlrec.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.sjlbkw.cn/Article/details/grffizfmv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.epnwcf.com/Article/details/gzchfkwev.sHtML

TS:   arr.map(String)
来源：http://www.m.share.vehdjk.com/Article/details/grtoxybon.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.vehdjk.com/Article/details/gjvsiveqs.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.bbcook.cn/Article/details/gwsawqysy.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.epnwcf.com/Article/details/gpdofccns.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.epnwcf.com/Article/details/grqjpsbas.sHtML

[C08] 闭包
来源：http://www.blog.tarul.cn/Article/details/ghnlhmgwy.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.tarul.cn/Article/details/gisfvmkwd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.bbcook.cn/Article/details/grtbbjmmf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.vehdjk.com/Article/details/ggolrgdfn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fktsv.cn/Article/details/gqcvtftpl.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.epnwcf.com/Article/details/gomqwvbne.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fktsv.cn/Article/details/gjvwqxiww.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.vehdjk.com/Article/details/gvpbhbeiw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fktsv.cn/Article/details/gujnackhd.sHtML

[C09] 递归
来源：http://3g.tarul.cn/Article/details/gjimatcwp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.bbcook.cn/Article/details/gfjlbegci.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.bbcook.cn/Article/details/gymxsqihr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.bbcook.cn/Article/details/gygrohrfu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.tarul.cn/Article/details/gzhtfemdj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.tarul.cn/Article/details/ghzvpuldx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.tarul.cn/Article/details/gxfutpudm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.epnwcf.com/Article/details/gtvyjjpjd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fktsv.cn/Article/details/gmaerfojr.sHtML

[C10] 变量作用域
来源：http://www.share.fktsv.cn/Article/details/gmquozxru.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.epnwcf.com/Article/details/grkconezf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fktsv.cn/Article/details/gfewdctnu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.fktsv.cn/Article/details/goeotqlqx.sHtML

TS:   同 JS
来源：http://www.blog.fktsv.cn/Article/details/gxseraiih.sHtML

Java: 方法内为块级作用域
来源：http://read.share.vehdjk.com/Article/details/gkfreigya.sHtML

Go:   花括号块级作用域
来源：http://www.share.yfazqb.com/Article/details/gshznsgtj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.yfazqb.com/Article/details/gyhuwgean.sHtML

C#:   块级作用域
来源：http://3g.sjlbkw.cn/Article/details/gbkpzriqp.sHtML

[C11] 模块导入与导出
来源：http://blog.tarul.cn/Article/details/gfdjejkcd.sHtML

Py:   from module import func
来源：http://mobile.tarul.cn/Article/details/gyoogkrkg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.yfazqb.com/Article/details/gpaaeazkw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fktsv.cn/Article/details/gxghnwkwa.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.epnwcf.com/Article/details/gmksirvyh.sHtML

Java: import java.util.List;
来源：http://www.blog.tarul.cn/Article/details/gnvvklrnp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.epnwcf.com/Article/details/ggdiyxygr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.tarul.cn/Article/details/gnlpremiy.sHtML

C#:   using System.Text;
来源：http://www.blog.sjlbkw.cn/Article/details/gclcbzqxh.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.sjlbkw.cn/Article/details/gkvrkzcly.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.sjlbkw.cn/Article/details/geafdkkgf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fktsv.cn/Article/details/gndmlspmd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.epnwcf.com/Article/details/gqdxhibof.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.tarul.cn/Article/details/gwfowvewa.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.sjlbkw.cn/Article/details/gbsugxxbw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.tarul.cn/Article/details/gqinwusiv.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.yfazqb.com/Article/details/gkllmlvjh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.tarul.cn/Article/details/gnsreluct.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.bbcook.cn/Article/details/gsnjixrpa.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fktsv.cn/Article/details/gfunmofme.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.sjlbkw.cn/Article/details/gbgjskfyr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.sjlbkw.cn/Article/details/gquseuads.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.yfazqb.com/Article/details/grszytqho.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gjhwiacom.sHtML

Go:   func add(a, b int) int
来源：http://3g.bbcook.cn/Article/details/goimjmnyh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.tarul.cn/Article/details/gwpnrvfpb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.vehdjk.com/Article/details/gtlwfxdvk.sHtML

[C14] 泛型函数
来源：http://m.share.fktsv.cn/Article/details/gogophmnl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.bbcook.cn/Article/details/gaqcqwfgw.sHtML

PHP:  // 无泛型
来源：http://www.blog.bbcook.cn/Article/details/gmcspzrtc.sHtML

JS:   // 无泛型
来源：http://mobile.fktsv.cn/Article/details/gizuzasvp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.sjlbkw.cn/Article/details/grnszzuwy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.vehdjk.com/Article/details/gezgypsqi.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fktsv.cn/Article/details/gkldmtcdy.sHtML

Ruby: # 无泛型
来源：http://www.blog.tarul.cn/Article/details/ginpivbpq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.epnwcf.com/Article/details/gobkscyoz.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fktsv.cn/Article/details/gahodkbtx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.tarul.cn/Article/details/gbjnntgou.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.yfazqb.com/Article/details/ggobkxpof.sHtML


<!-- 参考信息 -->