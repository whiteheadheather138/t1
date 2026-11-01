代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://wap.epnwcf.com/Article/details/gonqmgjwx.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.vehdjk.com/Article/details/greajkflv.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.sjlbkw.cn/Article/details/gwtltkvoh.sHtML

[A25] 字符串比较
来源：http://mobile.fktsv.cn/Article/details/ggzvpnzlh.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.bbcook.cn/Article/details/gkyffzczq.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.bbcook.cn/Article/details/gacbkwhfp.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.epnwcf.com/Article/details/gtgxsixhp.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.bbcook.cn/Article/details/gnchssjym.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.fktsv.cn/Article/details/gzkwtykcm.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.epnwcf.com/Article/details/gizambtao.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.bbcook.cn/Article/details/gtsyebrld.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.vehdjk.com/Article/details/gqvewpbzl.sHtML

[A26] 类型转换总览
来源：http://blog.epnwcf.com/Article/details/gaoyilazb.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.bbcook.cn/Article/details/glpvfbmey.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.sjlbkw.cn/Article/details/gbfbcuthp.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.vehdjk.com/Article/details/gmygdbhgy.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.vehdjk.com/Article/details/gkyhtztop.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.epnwcf.com/Article/details/gfqpfwyqa.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.fktsv.cn/Article/details/gdddhvshy.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.bbcook.cn/Article/details/gvdnxvcqm.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.vehdjk.com/Article/details/gyimopcfz.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gdqnwrfpt.sHtML

B. 流程控制
来源：http://www.blog.yfazqb.com/Article/details/gtchqymxg.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/guhqvwbjz.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.fktsv.cn/Article/details/gzlmifcng.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.sjlbkw.cn/Article/details/goomhmjbh.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.fktsv.cn/Article/details/gchmzkjln.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.yfazqb.com/Article/details/gukhstuve.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.tarul.cn/Article/details/gybwunjcs.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.epnwcf.com/Article/details/gqqsyzrgi.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.vehdjk.com/Article/details/gbjtwffnx.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.epnwcf.com/Article/details/gqxdmoxxi.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.sjlbkw.cn/Article/details/ghcyzlowg.sHtML

[B02] 多分支 else if / elif
来源：http://wap.fktsv.cn/Article/details/gsazovmif.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.bbcook.cn/Article/details/gjgnngexz.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.sjlbkw.cn/Article/details/gfrsjsagp.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.bbcook.cn/Article/details/gmiwcacin.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.tarul.cn/Article/details/glbnukqrb.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.tarul.cn/Article/details/gaivcqszb.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.vehdjk.com/Article/details/gkfxnqibg.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.yfazqb.com/Article/details/gecvsnkbs.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fktsv.cn/Article/details/gtanbvlpu.sHtML

[B03] switch / match / case
来源：http://m.share.bbcook.cn/Article/details/gkrqzmfed.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.bbcook.cn/Article/details/gjwvydsrb.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.epnwcf.com/Article/details/gbvjikrnn.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fktsv.cn/Article/details/gcrxpszgl.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.bbcook.cn/Article/details/gdpiloelg.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.tarul.cn/Article/details/gohwvypri.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.vehdjk.com/Article/details/gctudyzdw.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.sjlbkw.cn/Article/details/gvlzlilzk.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.sjlbkw.cn/Article/details/gqvjfxhkr.sHtML

[B04] for 计数循环
来源：http://mobile.vehdjk.com/Article/details/gtszptyip.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.bbcook.cn/Article/details/gtzgjwcdq.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.bbcook.cn/Article/details/gqmutcrsa.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.tarul.cn/Article/details/gomvzoxje.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.tarul.cn/Article/details/ghtbaftci.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.tarul.cn/Article/details/gzmywguic.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.epnwcf.com/Article/details/grsdxeubq.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.epnwcf.com/Article/details/groalffyj.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.fktsv.cn/Article/details/graqqziia.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.fktsv.cn/Article/details/gunokmaml.sHtML

Py:   for item in arr: print(item)
来源：http://3g.vehdjk.com/Article/details/giijfilkb.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.tarul.cn/Article/details/gtszflxky.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.vehdjk.com/Article/details/gakninyic.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.tarul.cn/Article/details/galyvujxb.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.epnwcf.com/Article/details/gfvsxppvg.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.vehdjk.com/Article/details/gblatwdcs.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.tarul.cn/Article/details/gwgsuibty.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.tarul.cn/Article/details/ghgccywdl.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.bbcook.cn/Article/details/guvabxbsy.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.epnwcf.com/Article/details/gihplhsrf.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.vehdjk.com/Article/details/gqydtggpu.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.yfazqb.com/Article/details/goiujadlf.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fktsv.cn/Article/details/gppgxepgd.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.fktsv.cn/Article/details/grknbtcsy.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.vehdjk.com/Article/details/glveqimwu.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.tarul.cn/Article/details/gcoqfnfgl.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.vehdjk.com/Article/details/gxmcqowle.sHtML

[B07] while 循环
来源：http://blog.bbcook.cn/Article/details/gmxwmxjpz.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.yfazqb.com/Article/details/gbcvymkfu.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.tarul.cn/Article/details/gyyqpelbd.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.epnwcf.com/Article/details/gclfwhqzw.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.fktsv.cn/Article/details/gtuthdddk.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.tarul.cn/Article/details/gjugqdwid.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.yfazqb.com/Article/details/gigpmvtgr.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.yfazqb.com/Article/details/gdakcklgf.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.fktsv.cn/Article/details/ghqvdgxen.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.yfazqb.com/Article/details/gjvdfwmxb.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.tarul.cn/Article/details/ggqlfsevw.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.fktsv.cn/Article/details/gnfdxxsas.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.yfazqb.com/Article/details/gceacbdld.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.sjlbkw.cn/Article/details/gjjkfezyq.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.sjlbkw.cn/Article/details/gvwyegjku.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.bbcook.cn/Article/details/gauiyvutr.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.tarul.cn/Article/details/gdzqnfdsd.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.tarul.cn/Article/details/gxoegsarb.sHtML

[B09] break 与 continue
来源：http://blog.yfazqb.com/Article/details/gqmfaqdkj.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.vehdjk.com/Article/details/gjmejgxuj.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.bbcook.cn/Article/details/gowyhnywt.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.sjlbkw.cn/Article/details/gvelckwcu.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.yfazqb.com/Article/details/gwqzfymff.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.epnwcf.com/Article/details/gdpzjastq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.bbcook.cn/Article/details/gnxelmojj.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.bbcook.cn/Article/details/gyswuoaip.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.yfazqb.com/Article/details/gvvucvdne.sHtML

[B10] 遍历同时拿索引
来源：http://baike.yfazqb.com/Article/details/gamyynusb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.vehdjk.com/Article/details/gkfnlgfej.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.vehdjk.com/Article/details/gwfwxftxi.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.tarul.cn/Article/details/gyqssogsd.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.vehdjk.com/Article/details/gzwjeajdc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.bbcook.cn/Article/details/gbutzvvii.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.bbcook.cn/Article/details/gyfrbxojh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.vehdjk.com/Article/details/gbiwigmle.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.fktsv.cn/Article/details/glhelimug.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.yfazqb.com/Article/details/gqmnvuage.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.epnwcf.com/Article/details/gvbcdmcpy.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.fktsv.cn/Article/details/gcgvxbyew.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.tarul.cn/Article/details/gizpjcexd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.bbcook.cn/Article/details/gedprbbgd.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.fktsv.cn/Article/details/grlqhydzx.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.vehdjk.com/Article/details/ghwpffcrz.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.epnwcf.com/Article/details/gnjfwedak.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.vehdjk.com/Article/details/gzjyvdrhs.sHtML

[B12] 跳出多层循环
来源：http://m.share.sjlbkw.cn/Article/details/gkfwajwdp.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.vehdjk.com/Article/details/gvevznjhi.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.bbcook.cn/Article/details/ggxpaulqs.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.yfazqb.com/Article/details/gezzsmncd.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.yfazqb.com/Article/details/gwccyrmyy.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fktsv.cn/Article/details/gjcyqqmih.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.vehdjk.com/Article/details/gkmivaaiy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.bbcook.cn/Article/details/gatjcaymu.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.fktsv.cn/Article/details/gepzdpufs.sHtML

[B13] 判断是否为数字
来源：http://wap.yfazqb.com/Article/details/grbuqpdrd.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.vehdjk.com/Article/details/gyrmghmpl.sHtML

PHP:  is_numeric($x)
来源：http://m.share.tarul.cn/Article/details/gwleazice.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.epnwcf.com/Article/details/gfwprgzaw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fktsv.cn/Article/details/gpjzglcdp.sHtML

Java: x instanceof Number
来源：http://3g.epnwcf.com/Article/details/gmcwiikok.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.vehdjk.com/Article/details/gcxfidipi.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.vehdjk.com/Article/details/gezgoowul.sHtML

C#:   x is int or double or decimal
来源：http://read.share.epnwcf.com/Article/details/gllnzbfgs.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.epnwcf.com/Article/details/geqkhmtbz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.sjlbkw.cn/Article/details/grfkzdcqk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.vehdjk.com/Article/details/gyucfkkgt.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.epnwcf.com/Article/details/goitlqhct.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.epnwcf.com/Article/details/gmtroemqs.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.vehdjk.com/Article/details/gtbusszfs.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.vehdjk.com/Article/details/ghrjprheg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.yfazqb.com/Article/details/gbmdpiogd.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.bbcook.cn/Article/details/gvwoyeiwf.sHtML

[B15] 布尔运算与取反
来源：http://3g.sjlbkw.cn/Article/details/gspccfsvh.sHtML

Py:   a and b or not c
来源：http://www.share.sjlbkw.cn/Article/details/gnnlgoiqo.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.epnwcf.com/Article/details/ggkkqgegq.sHtML

JS:   a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/gjapbgjfc.sHtML

TS:   a && b || !c
来源：http://3g.yfazqb.com/Article/details/gjaghxabn.sHtML

Java: a && b || !c
来源：http://wap.tarul.cn/Article/details/grwyjmprn.sHtML

Go:   a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gzcenwluy.sHtML

Ruby: a && b || !c
来源：http://www.share.sjlbkw.cn/Article/details/giomuzohq.sHtML

C#:   a && b || !c
来源：http://blog.tarul.cn/Article/details/gykrmtehe.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.vehdjk.com/Article/details/gkybpiqmr.sHtML

Py:   if not data: return
来源：http://mobile.yfazqb.com/Article/details/glgrynvyg.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.vehdjk.com/Article/details/gfwfsabon.sHtML

JS:   if (!data) return;
来源：http://3g.sjlbkw.cn/Article/details/gbnfamexj.sHtML

TS:   if (!data) return;
来源：http://3g.bbcook.cn/Article/details/gwbnsqsmk.sHtML

Java: if (data == null) return;
来源：http://blog.yfazqb.com/Article/details/grmymkvxl.sHtML

Go:   if data == nil { return }
来源：http://3g.epnwcf.com/Article/details/gtsuzszct.sHtML

Ruby: return if data.nil?
来源：http://www.blog.vehdjk.com/Article/details/gwujifxaz.sHtML

C#:   if (data == null) return;
来源：http://wap.fktsv.cn/Article/details/gjbjiawvz.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gkhpishkl.sHtML

C. 函数与作用域
来源：http://blog.bbcook.cn/Article/details/gzgqobave.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gzriiqcgo.sHtML

[C01] 定义函数
来源：http://mobile.vehdjk.com/Article/details/gpcucfebt.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.epnwcf.com/Article/details/gyxhftzqv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.bbcook.cn/Article/details/gxzzbgtmv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.tarul.cn/Article/details/gdsxupjba.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gtudvgqia.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.tarul.cn/Article/details/gvkswrqpc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.sjlbkw.cn/Article/details/gkuzgczsg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.tarul.cn/Article/details/gavyvdtwu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.vehdjk.com/Article/details/giplcqkxq.sHtML

[C02] 默认参数
来源：http://www.blog.epnwcf.com/Article/details/gdbzlsesn.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.yfazqb.com/Article/details/gljpytjwv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.bbcook.cn/Article/details/gzczesuhs.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/gxubiwska.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.tarul.cn/Article/details/grekghfqr.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.tarul.cn/Article/details/gifeixrgr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.vehdjk.com/Article/details/gggeklbnz.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.vehdjk.com/Article/details/gpkfzrhsd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.epnwcf.com/Article/details/gpudyevek.sHtML

[C03] 可变参数
来源：http://www.m.share.bbcook.cn/Article/details/gvgmefszc.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fktsv.cn/Article/details/gkdqeoseu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.sjlbkw.cn/Article/details/ggqhiykwr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.tarul.cn/Article/details/gltogcvpv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.vehdjk.com/Article/details/gtriopbtz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.bbcook.cn/Article/details/gnrkphzpi.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fktsv.cn/Article/details/gowtuxgxb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fktsv.cn/Article/details/gcenoarjv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.yfazqb.com/Article/details/geyjhmyrq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.sjlbkw.cn/Article/details/gacxetjqa.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.epnwcf.com/Article/details/gjbhjwpcg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.epnwcf.com/Article/details/gcmbqfemu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fktsv.cn/Article/details/gaxuhdemf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.tarul.cn/Article/details/gcikcyhvq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fktsv.cn/Article/details/gcvtjuncp.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.vehdjk.com/Article/details/gaavsjynt.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fktsv.cn/Article/details/gzlghitit.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.tarul.cn/Article/details/gahteclkq.sHtML

[C05] 返回多个值
来源：http://3g.epnwcf.com/Article/details/gbpnqlweb.sHtML

Py:   return a, b
来源：http://m.share.bbcook.cn/Article/details/gfndorzdg.sHtML

PHP:  return [$a, $b];
来源：http://wap.yfazqb.com/Article/details/grkptzwmk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.epnwcf.com/Article/details/gkswuqyeo.sHtML

TS:   return { a, b };
来源：http://www.m.share.bbcook.cn/Article/details/gvtqwtpiv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.sjlbkw.cn/Article/details/gzkuewozg.sHtML

Go:   return a, b
来源：http://blog.bbcook.cn/Article/details/goebpduhw.sHtML

Ruby: return a, b
来源：http://read.share.sjlbkw.cn/Article/details/ghootsikw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.epnwcf.com/Article/details/grdlmltmf.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.tarul.cn/Article/details/gmgaqadeu.sHtML

Py:   square = lambda x: x * x
来源：http://wap.bbcook.cn/Article/details/gonhfzajg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.tarul.cn/Article/details/grfforqfx.sHtML

JS:   const square = x => x * x;
来源：http://baike.vehdjk.com/Article/details/gsnxyaeqm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.tarul.cn/Article/details/gknhymybp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.vehdjk.com/Article/details/gwrsmccxq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.tarul.cn/Article/details/gosfdmpsh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.epnwcf.com/Article/details/gradtgnmt.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.vehdjk.com/Article/details/gxttjghjv.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.yfazqb.com/Article/details/gzvylzkgn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.tarul.cn/Article/details/ghmrlbbzl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.yfazqb.com/Article/details/gxnfezjzd.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.vehdjk.com/Article/details/gxoksuqsb.sHtML

TS:   arr.map(String)
来源：http://blog.yfazqb.com/Article/details/gkborlvmd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.vehdjk.com/Article/details/ggcqxgeyn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.tarul.cn/Article/details/gpagwgpzz.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.bbcook.cn/Article/details/gifdbqsye.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fktsv.cn/Article/details/gtaxcrkcw.sHtML

[C08] 闭包
来源：http://blog.vehdjk.com/Article/details/gxgvfxdso.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.epnwcf.com/Article/details/gzprvzncz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fktsv.cn/Article/details/grrpwisxp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.bbcook.cn/Article/details/gnsyeblhw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.vehdjk.com/Article/details/gxqhdtpmb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.bbcook.cn/Article/details/genjbazwv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.bbcook.cn/Article/details/guorunerv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fktsv.cn/Article/details/gxixqesrl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.epnwcf.com/Article/details/glvxvkwkw.sHtML

[C09] 递归
来源：http://baike.yfazqb.com/Article/details/gqlnbksdx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.sjlbkw.cn/Article/details/gywvzzfue.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.fktsv.cn/Article/details/godjnpsio.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.yfazqb.com/Article/details/gjtlyhgwx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.vehdjk.com/Article/details/gfekwifub.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.tarul.cn/Article/details/gbflkodyu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.yfazqb.com/Article/details/gnetdnrcd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.vehdjk.com/Article/details/gvkhzlumd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.yfazqb.com/Article/details/gsvmuqgxl.sHtML

[C10] 变量作用域
来源：http://wap.tarul.cn/Article/details/gthdplauo.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fktsv.cn/Article/details/gznesftjy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.yfazqb.com/Article/details/gbnmqfwcz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.bbcook.cn/Article/details/gpnrumhwc.sHtML

TS:   同 JS
来源：http://wap.tarul.cn/Article/details/gdzlzqddj.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.sjlbkw.cn/Article/details/gaagvdqhd.sHtML

Go:   花括号块级作用域
来源：http://www.blog.vehdjk.com/Article/details/gcbokumnw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fktsv.cn/Article/details/gxolmfcvo.sHtML

C#:   块级作用域
来源：http://mobile.bbcook.cn/Article/details/gsekvdtxh.sHtML

[C11] 模块导入与导出
来源：http://3g.epnwcf.com/Article/details/ghglhsfou.sHtML

Py:   from module import func
来源：http://m.share.sjlbkw.cn/Article/details/gsvikbyup.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.epnwcf.com/Article/details/gnzqcgbti.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.tarul.cn/Article/details/ggobzeces.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.epnwcf.com/Article/details/geyryvtis.sHtML

Java: import java.util.List;
来源：http://3g.yfazqb.com/Article/details/gpcsrkesh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.yfazqb.com/Article/details/gydbipwfj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.vehdjk.com/Article/details/gliihbkuj.sHtML

C#:   using System.Text;
来源：http://www.blog.fktsv.cn/Article/details/gkwkkzook.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.vehdjk.com/Article/details/gzvkxdqwe.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.vehdjk.com/Article/details/geaylhhzd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fktsv.cn/Article/details/gkntlhepb.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.epnwcf.com/Article/details/gfvbbtqfb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.bbcook.cn/Article/details/gxvfocqjq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.sjlbkw.cn/Article/details/ggxjwjxrv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.bbcook.cn/Article/details/gfywbfxub.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.sjlbkw.cn/Article/details/gjzfbinxg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.yfazqb.com/Article/details/gdecyyuhm.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fktsv.cn/Article/details/gkaphjjsg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.tarul.cn/Article/details/gkkdyxbjp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fktsv.cn/Article/details/gphfbxwuf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.sjlbkw.cn/Article/details/gdftzfypl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/ginklciok.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.tarul.cn/Article/details/gmzekcchi.sHtML

Go:   func add(a, b int) int
来源：http://www.share.tarul.cn/Article/details/gwrugjqpx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.sjlbkw.cn/Article/details/grdflhnao.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.tarul.cn/Article/details/gohxxjkfi.sHtML

[C14] 泛型函数
来源：http://baike.vehdjk.com/Article/details/gjxxykjzv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.bbcook.cn/Article/details/gqximvysk.sHtML

PHP:  // 无泛型
来源：http://3g.epnwcf.com/Article/details/gjuodoaoy.sHtML

JS:   // 无泛型
来源：http://m.share.epnwcf.com/Article/details/gfohfbfbd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.bbcook.cn/Article/details/gfcdgowrp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.sjlbkw.cn/Article/details/ggxawbkcm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.vehdjk.com/Article/details/gkqxwupgr.sHtML

Ruby: # 无泛型
来源：http://www.m.share.epnwcf.com/Article/details/gxhgkwzeg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.yfazqb.com/Article/details/gpnknpott.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.yfazqb.com/Article/details/grwelycja.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fktsv.cn/Article/details/gmuyaiufw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.sjlbkw.cn/Article/details/gphkigijk.sHtML


<!-- 参考信息 -->