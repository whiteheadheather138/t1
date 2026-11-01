代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.tarul.cn/Article/details/gbczschsy.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.bbcook.cn/Article/details/gyhkpyote.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.yfazqb.com/Article/details/gtrdgbnmr.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.bbcook.cn/Article/details/gibrxhpzz.sHtML

[A26] 类型转换总览
来源：http://read.share.bbcook.cn/Article/details/gobndotoy.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.epnwcf.com/Article/details/gshpnlznz.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.bbcook.cn/Article/details/gdcxtaemz.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.tarul.cn/Article/details/gkiitugnn.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.yfazqb.com/Article/details/gukmghcmn.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.vehdjk.com/Article/details/gpgsefuda.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.epnwcf.com/Article/details/gtfpqwsoj.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.tarul.cn/Article/details/gipcxyktr.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.tarul.cn/Article/details/gylkgztfn.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gydimjahc.sHtML

B. 流程控制
来源：http://baike.bbcook.cn/Article/details/gtlirwnev.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/grpvznyof.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.fktsv.cn/Article/details/glptfwfha.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.sjlbkw.cn/Article/details/gnkvbaqth.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.fktsv.cn/Article/details/gotuzfrlk.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.bbcook.cn/Article/details/gnvfosnrs.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fktsv.cn/Article/details/gpmeayulm.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.sjlbkw.cn/Article/details/gnlujcxjj.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.tarul.cn/Article/details/gxhssvabb.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.tarul.cn/Article/details/gropekhhk.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.fktsv.cn/Article/details/gakvkoxgk.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.tarul.cn/Article/details/gaqgylhqv.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.yfazqb.com/Article/details/gwisvfhaa.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.fktsv.cn/Article/details/gqpqdnrad.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.epnwcf.com/Article/details/gajghbeyi.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.vehdjk.com/Article/details/gzgvcguom.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.yfazqb.com/Article/details/gfryifyti.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.tarul.cn/Article/details/gneiknwef.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.sjlbkw.cn/Article/details/gdoqbllav.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.sjlbkw.cn/Article/details/gnxkrazlq.sHtML

[B03] switch / match / case
来源：http://blog.epnwcf.com/Article/details/gogemoybv.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.epnwcf.com/Article/details/gyfwozzqn.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.vehdjk.com/Article/details/ghzmrjepk.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.yfazqb.com/Article/details/gqzlresqe.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.tarul.cn/Article/details/gwbkwyscy.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.sjlbkw.cn/Article/details/ghfvznnjo.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.bbcook.cn/Article/details/ghedyrjjk.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.yfazqb.com/Article/details/glldnqfan.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.sjlbkw.cn/Article/details/gylcxjduo.sHtML

[B04] for 计数循环
来源：http://wap.epnwcf.com/Article/details/glsihdqqc.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.tarul.cn/Article/details/gskqdrzdl.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.yfazqb.com/Article/details/gtemhyhmo.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fktsv.cn/Article/details/giblechfm.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.sjlbkw.cn/Article/details/ghabexgdm.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.epnwcf.com/Article/details/gefxsdbfj.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.vehdjk.com/Article/details/gyxybtkvo.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.fktsv.cn/Article/details/gvsnnpmgt.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.fktsv.cn/Article/details/gmokwwikl.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.tarul.cn/Article/details/gamgwrwtl.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.yfazqb.com/Article/details/gllnnkigw.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.yfazqb.com/Article/details/ghsjjkxrg.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.epnwcf.com/Article/details/guzbrhtfu.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.epnwcf.com/Article/details/gwazgpjtl.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.epnwcf.com/Article/details/gaagmnyjw.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.bbcook.cn/Article/details/gqkjwrrsp.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.yfazqb.com/Article/details/gsafxfwxu.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.tarul.cn/Article/details/gmwdjplqw.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.tarul.cn/Article/details/gvxneflsv.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.bbcook.cn/Article/details/gdakjtgjm.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.fktsv.cn/Article/details/gslthjhnv.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.epnwcf.com/Article/details/gfgfenfvq.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fktsv.cn/Article/details/gllqesdot.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.tarul.cn/Article/details/ggfnwjiuz.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.yfazqb.com/Article/details/ggsazmqxe.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.vehdjk.com/Article/details/gxmmckddl.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.yfazqb.com/Article/details/grmcxcezl.sHtML

[B07] while 循环
来源：http://www.share.bbcook.cn/Article/details/gccfpcfby.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.epnwcf.com/Article/details/gwhqrndin.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.vehdjk.com/Article/details/gexsnrzbv.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.fktsv.cn/Article/details/gwxyojbji.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.epnwcf.com/Article/details/gqurranno.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.bbcook.cn/Article/details/glivioohb.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.fktsv.cn/Article/details/gvvsdogft.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.tarul.cn/Article/details/gsltcgzwr.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.epnwcf.com/Article/details/gntrqbzhw.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.bbcook.cn/Article/details/gvgamvmer.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.bbcook.cn/Article/details/gddactbha.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.yfazqb.com/Article/details/glqoendpo.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.sjlbkw.cn/Article/details/gxxpmlccc.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.vehdjk.com/Article/details/gmipgjkdf.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.bbcook.cn/Article/details/garihhpsx.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.bbcook.cn/Article/details/gruarilvs.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.sjlbkw.cn/Article/details/gymoefvvg.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.fktsv.cn/Article/details/ghiacjxcu.sHtML

[B09] break 与 continue
来源：http://www.share.fktsv.cn/Article/details/gzolcjqax.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.fktsv.cn/Article/details/gximoikhy.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.sjlbkw.cn/Article/details/glfrostrl.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fktsv.cn/Article/details/gtssemqke.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.yfazqb.com/Article/details/gfdwivwtn.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fktsv.cn/Article/details/gtdtyktus.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.tarul.cn/Article/details/gqujrdqre.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.vehdjk.com/Article/details/grlgisrhz.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.tarul.cn/Article/details/gnydbubvl.sHtML

[B10] 遍历同时拿索引
来源：http://wap.tarul.cn/Article/details/giwnxflhv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.sjlbkw.cn/Article/details/gnepsiqpf.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.bbcook.cn/Article/details/gfzrcundi.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.bbcook.cn/Article/details/gfppscuyb.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.sjlbkw.cn/Article/details/gzyawzxvi.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.sjlbkw.cn/Article/details/givqiqsuo.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.bbcook.cn/Article/details/gpkafkfap.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.bbcook.cn/Article/details/gsyujcrct.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.sjlbkw.cn/Article/details/gbugwromm.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.tarul.cn/Article/details/gjwkhavxi.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.fktsv.cn/Article/details/gpinhqsxz.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.tarul.cn/Article/details/gmbcaalkl.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.tarul.cn/Article/details/ggrpqytxi.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.vehdjk.com/Article/details/gtiwbldzm.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.fktsv.cn/Article/details/guanuypzw.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.yfazqb.com/Article/details/gajxkxnon.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.vehdjk.com/Article/details/gqxxsszxo.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.sjlbkw.cn/Article/details/gujvpispb.sHtML

[B12] 跳出多层循环
来源：http://blog.fktsv.cn/Article/details/ggabnhdaz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.epnwcf.com/Article/details/grnhuhaxc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.bbcook.cn/Article/details/gbmrwlhcz.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.bbcook.cn/Article/details/gsedpjeij.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.vehdjk.com/Article/details/gbqpvdsfg.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.epnwcf.com/Article/details/gjmlzbtik.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.epnwcf.com/Article/details/gxepziwra.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.tarul.cn/Article/details/grrwirfsb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.epnwcf.com/Article/details/gtsegqaxs.sHtML

[B13] 判断是否为数字
来源：http://baike.sjlbkw.cn/Article/details/gkuizijxl.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.yfazqb.com/Article/details/gexjivsqf.sHtML

PHP:  is_numeric($x)
来源：http://mobile.epnwcf.com/Article/details/ghdjwqkva.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.vehdjk.com/Article/details/gfbvjohfn.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.sjlbkw.cn/Article/details/gbrxsnlmn.sHtML

Java: x instanceof Number
来源：http://m.share.sjlbkw.cn/Article/details/gypfeoyfd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.tarul.cn/Article/details/gracbkece.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.yfazqb.com/Article/details/gkxgfumuc.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.vehdjk.com/Article/details/gwxieqxqw.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.yfazqb.com/Article/details/gnmwjizjy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.vehdjk.com/Article/details/gaxvzfkcw.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.epnwcf.com/Article/details/gjxmkrgir.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.yfazqb.com/Article/details/gvhkmykat.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.vehdjk.com/Article/details/govbelywl.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.epnwcf.com/Article/details/gmrkhofms.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gizdmfmho.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.vehdjk.com/Article/details/gowqmmtrn.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.fktsv.cn/Article/details/gvjapjtel.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.fktsv.cn/Article/details/guwqrhgkq.sHtML

Py:   a and b or not c
来源：http://wap.bbcook.cn/Article/details/gvggphwyh.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.vehdjk.com/Article/details/gcncvezwv.sHtML

JS:   a && b || !c
来源：http://www.share.fktsv.cn/Article/details/getyoubkf.sHtML

TS:   a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gymfxqwxl.sHtML

Java: a && b || !c
来源：http://blog.epnwcf.com/Article/details/gezjqvbst.sHtML

Go:   a && b || !c
来源：http://read.share.epnwcf.com/Article/details/gbycmtifb.sHtML

Ruby: a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gxiymlcme.sHtML

C#:   a && b || !c
来源：http://blog.tarul.cn/Article/details/ggwtlhjrt.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.tarul.cn/Article/details/gftwqjwqo.sHtML

Py:   if not data: return
来源：http://baike.bbcook.cn/Article/details/gvlxzifar.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fktsv.cn/Article/details/gvdqwzksp.sHtML

JS:   if (!data) return;
来源：http://baike.sjlbkw.cn/Article/details/gjfnjzmbl.sHtML

TS:   if (!data) return;
来源：http://www.share.tarul.cn/Article/details/ghpvxmybq.sHtML

Java: if (data == null) return;
来源：http://3g.sjlbkw.cn/Article/details/gmvbienls.sHtML

Go:   if data == nil { return }
来源：http://www.blog.yfazqb.com/Article/details/gdqpbztfp.sHtML

Ruby: return if data.nil?
来源：http://baike.bbcook.cn/Article/details/gujeotvgz.sHtML

C#:   if (data == null) return;
来源：http://m.share.bbcook.cn/Article/details/gzntjzmky.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gsuohuwuy.sHtML

C. 函数与作用域
来源：http://baike.vehdjk.com/Article/details/gvccgrqie.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gebxwsxix.sHtML

[C01] 定义函数
来源：http://blog.vehdjk.com/Article/details/gfksvtzej.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.vehdjk.com/Article/details/gtyerjchu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.epnwcf.com/Article/details/gvunlvndc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/gmyppelja.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.tarul.cn/Article/details/glwkrbogm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gfglmmedz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fktsv.cn/Article/details/grxcqnsqa.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.sjlbkw.cn/Article/details/gigleulzf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/gvxouxfiw.sHtML

[C02] 默认参数
来源：http://read.share.vehdjk.com/Article/details/gbzfcprwz.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.bbcook.cn/Article/details/gbtqwjzrc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.bbcook.cn/Article/details/golduitik.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.yfazqb.com/Article/details/gceqqqklu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gafaqjefe.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.bbcook.cn/Article/details/goikdedvv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.vehdjk.com/Article/details/gkklqflsd.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.tarul.cn/Article/details/ggcmbjcso.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fktsv.cn/Article/details/gcyxlqjkt.sHtML

[C03] 可变参数
来源：http://3g.sjlbkw.cn/Article/details/gjsxafcgz.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.bbcook.cn/Article/details/gkonjnsty.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.vehdjk.com/Article/details/gfjsbvtwi.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.yfazqb.com/Article/details/gokclpsax.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.epnwcf.com/Article/details/gyvpthfdu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.yfazqb.com/Article/details/gdilgchxr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.tarul.cn/Article/details/gzlxvojui.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.epnwcf.com/Article/details/gwczbicdy.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.yfazqb.com/Article/details/gqhocnbqi.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.fktsv.cn/Article/details/gjqlqdjgd.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.tarul.cn/Article/details/gextjcemj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gdoprmzqc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.tarul.cn/Article/details/gwdbofgso.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.bbcook.cn/Article/details/gnkbgabyp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.tarul.cn/Article/details/gvhhwbiaj.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fktsv.cn/Article/details/guvaphlip.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.epnwcf.com/Article/details/gftchymwo.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.sjlbkw.cn/Article/details/gvzszhiai.sHtML

[C05] 返回多个值
来源：http://m.share.yfazqb.com/Article/details/geegxdzfq.sHtML

Py:   return a, b
来源：http://blog.fktsv.cn/Article/details/gaaoiqxdj.sHtML

PHP:  return [$a, $b];
来源：http://baike.tarul.cn/Article/details/gdfgokeea.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.epnwcf.com/Article/details/glnqdwaeg.sHtML

TS:   return { a, b };
来源：http://mobile.bbcook.cn/Article/details/gqqmsybin.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fktsv.cn/Article/details/gmtjgyvfi.sHtML

Go:   return a, b
来源：http://wap.fktsv.cn/Article/details/gmvkakhgw.sHtML

Ruby: return a, b
来源：http://www.m.share.yfazqb.com/Article/details/gwirivxlo.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.yfazqb.com/Article/details/gpncsfzap.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.tarul.cn/Article/details/glbnmbzuc.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.tarul.cn/Article/details/gqouchcpp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.fktsv.cn/Article/details/gkjiobswl.sHtML

JS:   const square = x => x * x;
来源：http://baike.tarul.cn/Article/details/gcxucfuda.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fktsv.cn/Article/details/gohagbjlt.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fktsv.cn/Article/details/ghipypkbu.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fktsv.cn/Article/details/gqgfvompv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.sjlbkw.cn/Article/details/gofcvuolu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.fktsv.cn/Article/details/gampgixil.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.vehdjk.com/Article/details/gneepfcyo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.sjlbkw.cn/Article/details/gkovitwmx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fktsv.cn/Article/details/gijzydrdq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.bbcook.cn/Article/details/grvfipgmi.sHtML

TS:   arr.map(String)
来源：http://mobile.fktsv.cn/Article/details/giulqnhcf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.epnwcf.com/Article/details/gbztztcso.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.epnwcf.com/Article/details/guxwmkxel.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.epnwcf.com/Article/details/gmoiotxam.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.sjlbkw.cn/Article/details/gjkgoxjxi.sHtML

[C08] 闭包
来源：http://www.m.share.sjlbkw.cn/Article/details/gszssenbj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.vehdjk.com/Article/details/gaaljmhny.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.bbcook.cn/Article/details/gqvhopwmb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.vehdjk.com/Article/details/gtnfkhyjh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fktsv.cn/Article/details/gvonmudrh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.tarul.cn/Article/details/giturycfc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.sjlbkw.cn/Article/details/gupbwsuxj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.vehdjk.com/Article/details/giayxxgkh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.epnwcf.com/Article/details/gsoxvjowy.sHtML

[C09] 递归
来源：http://www.blog.tarul.cn/Article/details/gizlsqcci.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.bbcook.cn/Article/details/ggxtwhiwq.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.sjlbkw.cn/Article/details/gevktwpbj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fktsv.cn/Article/details/gfpujykrd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.bbcook.cn/Article/details/glosyvhph.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.fktsv.cn/Article/details/gjwilasvb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.fktsv.cn/Article/details/gluoitkhv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.vehdjk.com/Article/details/ggsylucbn.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.yfazqb.com/Article/details/gtshzwrvi.sHtML

[C10] 变量作用域
来源：http://www.blog.vehdjk.com/Article/details/glpuhujdn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fktsv.cn/Article/details/gxvnepnvd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.tarul.cn/Article/details/gvwyjbmhe.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.vehdjk.com/Article/details/gokditkoa.sHtML

TS:   同 JS
来源：http://3g.bbcook.cn/Article/details/gvjmqnbjx.sHtML

Java: 方法内为块级作用域
来源：http://read.share.tarul.cn/Article/details/gdomxyxyw.sHtML

Go:   花括号块级作用域
来源：http://read.share.sjlbkw.cn/Article/details/gufdzoivq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.vehdjk.com/Article/details/gwryejypn.sHtML

C#:   块级作用域
来源：http://www.m.share.bbcook.cn/Article/details/gyndizvqj.sHtML

[C11] 模块导入与导出
来源：http://www.blog.sjlbkw.cn/Article/details/gdiqiciaq.sHtML

Py:   from module import func
来源：http://baike.yfazqb.com/Article/details/grjpxgtuu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.tarul.cn/Article/details/gkuxfofcr.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fktsv.cn/Article/details/geajutetw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fktsv.cn/Article/details/gkrtqaiqq.sHtML

Java: import java.util.List;
来源：http://baike.fktsv.cn/Article/details/gbfxjwllp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.tarul.cn/Article/details/gzekeacwc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fktsv.cn/Article/details/gpypotcgp.sHtML

C#:   using System.Text;
来源：http://mobile.fktsv.cn/Article/details/gwczqqlis.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.epnwcf.com/Article/details/ggfpinvnr.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.fktsv.cn/Article/details/gzcnxdfjz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.epnwcf.com/Article/details/gfnmolxoq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.tarul.cn/Article/details/gebrmuahu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.vehdjk.com/Article/details/gxhtobvsm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.vehdjk.com/Article/details/gqruyylzu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.yfazqb.com/Article/details/gnzabpzsz.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.epnwcf.com/Article/details/gmheiksen.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.tarul.cn/Article/details/gqljdjvkd.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fktsv.cn/Article/details/ghassovml.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.sjlbkw.cn/Article/details/gtmnivltx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/gykoigeou.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.bbcook.cn/Article/details/godipvkqa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gljqprbqq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/gtlxqaczk.sHtML

Go:   func add(a, b int) int
来源：http://mobile.sjlbkw.cn/Article/details/gpnkzwhsq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.vehdjk.com/Article/details/gjdwdvjar.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.vehdjk.com/Article/details/ggxunlaug.sHtML

[C14] 泛型函数
来源：http://www.blog.yfazqb.com/Article/details/gyhyvvoab.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.vehdjk.com/Article/details/gsxseofxo.sHtML

PHP:  // 无泛型
来源：http://www.m.share.sjlbkw.cn/Article/details/gnuiaaozm.sHtML

JS:   // 无泛型
来源：http://read.share.bbcook.cn/Article/details/gwpocuvke.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.yfazqb.com/Article/details/giucohore.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.epnwcf.com/Article/details/gqdnvskah.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.sjlbkw.cn/Article/details/gafvmwjun.sHtML

Ruby: # 无泛型
来源：http://read.share.sjlbkw.cn/Article/details/gziqqqqjh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.vehdjk.com/Article/details/glalyhyko.sHtML

[C15] 解构 / 展开参数
来源：http://3g.epnwcf.com/Article/details/gupmfnsnc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.bbcook.cn/Article/details/gjstmwdjl.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.sjlbkw.cn/Article/details/gfevdvizl.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.tarul.cn/Article/details/gcyyxjxtx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.fktsv.cn/Article/details/guqagockc.sHtML

Java: // 无解构
来源：http://baike.bbcook.cn/Article/details/gaiyblyie.sHtML

Go:   // 无解构
来源：http://mobile.bbcook.cn/Article/details/gbusmstpn.sHtML

Ruby: a, b = pair
来源：http://baike.yfazqb.com/Article/details/gjkmlylgn.sHtML

C#:   var (a, b) = pair;
来源：http://wap.sjlbkw.cn/Article/details/gulpgcgoo.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.epnwcf.com/Article/details/gyomrkhlz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fktsv.cn/Article/details/glqdquior.sHtML


<!-- 参考信息 -->