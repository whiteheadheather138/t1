代发 wailian999

[A26] 类型转换总览
来源：http://read.share.epnwcf.com/Article/details/grgplvayk.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.bbcook.cn/Article/details/gmhxjvgzu.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.bbcook.cn/Article/details/gwjvyfjvn.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.sjlbkw.cn/Article/details/gcyqetdmz.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.vehdjk.com/Article/details/gyltfareh.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.vehdjk.com/Article/details/gvurcidse.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.yfazqb.com/Article/details/gorapjdhm.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.tarul.cn/Article/details/gpntyiukx.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.yfazqb.com/Article/details/gzuuphcxc.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gqbgjzzzp.sHtML

B. 流程控制
来源：http://www.m.share.bbcook.cn/Article/details/gbgkozqhh.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/grzcmvkgy.sHtML

[B01] 条件判断 if / else
来源：http://m.share.tarul.cn/Article/details/gofmntfpf.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.fktsv.cn/Article/details/grqvbnqim.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.vehdjk.com/Article/details/ggokazhjy.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fktsv.cn/Article/details/gyjqgjtxk.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.epnwcf.com/Article/details/gwfhkgnec.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.tarul.cn/Article/details/gjmhppise.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.epnwcf.com/Article/details/gokkzdbzo.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.tarul.cn/Article/details/gyrvzluxw.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.bbcook.cn/Article/details/garmdsqhu.sHtML

[B02] 多分支 else if / elif
来源：http://3g.epnwcf.com/Article/details/gbaymvtvl.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.vehdjk.com/Article/details/grcjuvwec.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.tarul.cn/Article/details/gqqnnxolu.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fktsv.cn/Article/details/guoayswwk.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.epnwcf.com/Article/details/gjvwzzayq.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.tarul.cn/Article/details/gwwosnngr.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxiluplmf.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.tarul.cn/Article/details/gqderpznh.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fktsv.cn/Article/details/gbkpmpqpn.sHtML

[B03] switch / match / case
来源：http://baike.sjlbkw.cn/Article/details/gsqsltamm.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.tarul.cn/Article/details/godbihoqo.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.yfazqb.com/Article/details/gjrqrssfb.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.bbcook.cn/Article/details/gpxwusahy.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fktsv.cn/Article/details/giucvbfdn.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.epnwcf.com/Article/details/gfotoptgd.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.fktsv.cn/Article/details/gvadsqyry.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.fktsv.cn/Article/details/gxhzivxuh.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.fktsv.cn/Article/details/gxhgwfxfx.sHtML

[B04] for 计数循环
来源：http://baike.tarul.cn/Article/details/gtpcvnxam.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.yfazqb.com/Article/details/gtpyflvmk.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.epnwcf.com/Article/details/gykritwnz.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.tarul.cn/Article/details/gqtqdosae.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.tarul.cn/Article/details/gjyosgtbw.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.tarul.cn/Article/details/gzyzuecph.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.sjlbkw.cn/Article/details/grgsrsckk.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.yfazqb.com/Article/details/ggaiihqcf.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.vehdjk.com/Article/details/gppkltvkc.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.yfazqb.com/Article/details/gkgmdeali.sHtML

Py:   for item in arr: print(item)
来源：http://3g.fktsv.cn/Article/details/gizffyzbo.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.vehdjk.com/Article/details/gsevldpdl.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.fktsv.cn/Article/details/gmazgngfc.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gynpxjmmt.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.sjlbkw.cn/Article/details/gdpsumuaf.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.epnwcf.com/Article/details/gqrfuxanx.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.tarul.cn/Article/details/gmspoiqiz.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.epnwcf.com/Article/details/gqsneprwb.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.epnwcf.com/Article/details/gmlsshukd.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.tarul.cn/Article/details/gyovsuwtu.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.tarul.cn/Article/details/gkhiubrxd.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.tarul.cn/Article/details/glabljwol.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.bbcook.cn/Article/details/gldkrvqpz.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.epnwcf.com/Article/details/gzvjgqezr.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.yfazqb.com/Article/details/gqyksncvi.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.yfazqb.com/Article/details/gvvkifobt.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.vehdjk.com/Article/details/gdzdlkpwb.sHtML

[B07] while 循环
来源：http://m.share.yfazqb.com/Article/details/gwjnupljz.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.sjlbkw.cn/Article/details/gicjwcqdt.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.fktsv.cn/Article/details/guilcdbka.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.fktsv.cn/Article/details/gpdihhdkj.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.fktsv.cn/Article/details/gltzqldde.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.vehdjk.com/Article/details/gtijkrfwt.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.tarul.cn/Article/details/gvxizuhkk.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.epnwcf.com/Article/details/gbuybaidw.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.yfazqb.com/Article/details/gjkismrfy.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.tarul.cn/Article/details/ghlipvmrs.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.fktsv.cn/Article/details/gmoqtrlps.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.sjlbkw.cn/Article/details/guegupsgx.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.epnwcf.com/Article/details/gjymwpzwv.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.epnwcf.com/Article/details/gyrcbizrj.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.tarul.cn/Article/details/gdskazzdo.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.sjlbkw.cn/Article/details/gwrqtqomk.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.epnwcf.com/Article/details/gnunfkxfv.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.yfazqb.com/Article/details/gcpxrrkxf.sHtML

[B09] break 与 continue
来源：http://baike.vehdjk.com/Article/details/gmvfdydgf.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.bbcook.cn/Article/details/gmwxwpcly.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.yfazqb.com/Article/details/giyhwwufb.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fktsv.cn/Article/details/gtfzheemj.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.bbcook.cn/Article/details/gqcnsdics.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.epnwcf.com/Article/details/ghvhgazqy.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.epnwcf.com/Article/details/gifdpvqsk.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.fktsv.cn/Article/details/gmbrzpoax.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.sjlbkw.cn/Article/details/gcqavryni.sHtML

[B10] 遍历同时拿索引
来源：http://wap.fktsv.cn/Article/details/gawwjwmza.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.yfazqb.com/Article/details/gazwxfalp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.sjlbkw.cn/Article/details/gxsijzktm.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.bbcook.cn/Article/details/gzgpwlbtl.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.tarul.cn/Article/details/gjqelnznq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.vehdjk.com/Article/details/gojsfneqo.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.tarul.cn/Article/details/ggeiyfgsv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.vehdjk.com/Article/details/gryqizxee.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.tarul.cn/Article/details/gmznjexhy.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.tarul.cn/Article/details/grvwgofkd.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.vehdjk.com/Article/details/gpsjsmine.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.yfazqb.com/Article/details/gadgmuxre.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.tarul.cn/Article/details/gykgympdk.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.tarul.cn/Article/details/gwcejbeeq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.fktsv.cn/Article/details/gkyucshzs.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.bbcook.cn/Article/details/gjhxvxxgw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.sjlbkw.cn/Article/details/gvcfrkvll.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.epnwcf.com/Article/details/gpttzyjrs.sHtML

[B12] 跳出多层循环
来源：http://www.blog.bbcook.cn/Article/details/geyqomkoq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fktsv.cn/Article/details/gsygyzsbw.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.epnwcf.com/Article/details/gznckkhyq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.epnwcf.com/Article/details/gepzecssa.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.yfazqb.com/Article/details/gikfliybq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.epnwcf.com/Article/details/gungdohgw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.epnwcf.com/Article/details/gyxfmkgxq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.sjlbkw.cn/Article/details/gtjumbzls.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.fktsv.cn/Article/details/gmhzhenla.sHtML

[B13] 判断是否为数字
来源：http://blog.fktsv.cn/Article/details/gtxtqubhv.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.tarul.cn/Article/details/gqtbcbvfl.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.sjlbkw.cn/Article/details/glqdtwavx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.vehdjk.com/Article/details/goujdhvqv.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fktsv.cn/Article/details/gdolpbhxs.sHtML

Java: x instanceof Number
来源：http://read.share.sjlbkw.cn/Article/details/gknbwhyyl.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.vehdjk.com/Article/details/gskwfuekc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.yfazqb.com/Article/details/gwdqfotii.sHtML

C#:   x is int or double or decimal
来源：http://m.share.bbcook.cn/Article/details/gbhtxlorq.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.bbcook.cn/Article/details/gfiqiakht.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.bbcook.cn/Article/details/gtbunvtmc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.bbcook.cn/Article/details/gbbpnklye.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.tarul.cn/Article/details/gxvdazjdu.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.bbcook.cn/Article/details/gvcezvres.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.epnwcf.com/Article/details/gcdjqtdoy.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fktsv.cn/Article/details/grwtdwwxm.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.tarul.cn/Article/details/gzithdxac.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.epnwcf.com/Article/details/gqpuvkgyg.sHtML

[B15] 布尔运算与取反
来源：http://wap.sjlbkw.cn/Article/details/gjhmscgxt.sHtML

Py:   a and b or not c
来源：http://mobile.epnwcf.com/Article/details/gyyaskpqc.sHtML

PHP:  $a && $b || !$c
来源：http://wap.yfazqb.com/Article/details/gyiumfcik.sHtML

JS:   a && b || !c
来源：http://www.blog.epnwcf.com/Article/details/gmececysh.sHtML

TS:   a && b || !c
来源：http://www.share.yfazqb.com/Article/details/gijwljbty.sHtML

Java: a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/genzwqfdr.sHtML

Go:   a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/gusjrjezl.sHtML

Ruby: a && b || !c
来源：http://baike.epnwcf.com/Article/details/gcbrqhstc.sHtML

C#:   a && b || !c
来源：http://3g.epnwcf.com/Article/details/glmndtugi.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.sjlbkw.cn/Article/details/giruxbboh.sHtML

Py:   if not data: return
来源：http://m.share.yfazqb.com/Article/details/goplalozg.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.vehdjk.com/Article/details/gcafqitqb.sHtML

JS:   if (!data) return;
来源：http://www.share.vehdjk.com/Article/details/gdfiqbloj.sHtML

TS:   if (!data) return;
来源：http://wap.epnwcf.com/Article/details/gsxmqcljq.sHtML

Java: if (data == null) return;
来源：http://mobile.tarul.cn/Article/details/gbbsvevhm.sHtML

Go:   if data == nil { return }
来源：http://m.share.tarul.cn/Article/details/gyteiebaf.sHtML

Ruby: return if data.nil?
来源：http://read.share.fktsv.cn/Article/details/gbzsmuhej.sHtML

C#:   if (data == null) return;
来源：http://www.blog.epnwcf.com/Article/details/gzcunvrqe.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gfhiowlkd.sHtML

C. 函数与作用域
来源：http://www.m.share.bbcook.cn/Article/details/gwfrgbfwg.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gdqvzgwdz.sHtML

[C01] 定义函数
来源：http://mobile.tarul.cn/Article/details/gyjuihzed.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.vehdjk.com/Article/details/gspmtpjnp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.epnwcf.com/Article/details/gujifwthg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/geqjxehvl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.epnwcf.com/Article/details/gbdlmctwo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gcqwteovf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.bbcook.cn/Article/details/gznprjdds.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.vehdjk.com/Article/details/gncysggah.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/gijfapris.sHtML

[C02] 默认参数
来源：http://wap.fktsv.cn/Article/details/gkgehzgzf.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.epnwcf.com/Article/details/gtmqnleos.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.epnwcf.com/Article/details/gokefxzek.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fktsv.cn/Article/details/gscbezpzc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gqtcheaxc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fktsv.cn/Article/details/gxoixxtjm.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.bbcook.cn/Article/details/gkibznybu.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.epnwcf.com/Article/details/gnqnvdzwv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.yfazqb.com/Article/details/gayjhwsfs.sHtML

[C03] 可变参数
来源：http://baike.epnwcf.com/Article/details/ghdfydvvi.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.yfazqb.com/Article/details/gdajycked.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.sjlbkw.cn/Article/details/goniokuqp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.vehdjk.com/Article/details/gsnweezmg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.bbcook.cn/Article/details/gcajoccao.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.epnwcf.com/Article/details/gksrrhjyc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.bbcook.cn/Article/details/gwwptsdrn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fktsv.cn/Article/details/gtpfwxxqs.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.epnwcf.com/Article/details/ghyhdycpa.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.bbcook.cn/Article/details/gxyllxcev.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.bbcook.cn/Article/details/gcldwskwg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.epnwcf.com/Article/details/gnqnjoigr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.bbcook.cn/Article/details/guntbwdro.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.yfazqb.com/Article/details/gijrypjpk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.vehdjk.com/Article/details/glkbbwpcg.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.vehdjk.com/Article/details/gkmdzkhhw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.yfazqb.com/Article/details/gvszmmaej.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.bbcook.cn/Article/details/gjfipqsrr.sHtML

[C05] 返回多个值
来源：http://baike.vehdjk.com/Article/details/gvliadgqr.sHtML

Py:   return a, b
来源：http://mobile.sjlbkw.cn/Article/details/gcbpoblpd.sHtML

PHP:  return [$a, $b];
来源：http://m.share.yfazqb.com/Article/details/gbmqxjxrx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.sjlbkw.cn/Article/details/gmdwqqhnl.sHtML

TS:   return { a, b };
来源：http://m.share.epnwcf.com/Article/details/grkgnshmz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.bbcook.cn/Article/details/gedsylltu.sHtML

Go:   return a, b
来源：http://baike.yfazqb.com/Article/details/ghyttgroa.sHtML

Ruby: return a, b
来源：http://www.blog.yfazqb.com/Article/details/ggezbdcgq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.tarul.cn/Article/details/ghuwthpju.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.bbcook.cn/Article/details/gnucagpqc.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.epnwcf.com/Article/details/gewioxqss.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.tarul.cn/Article/details/gafelihqm.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.tarul.cn/Article/details/gltzagkuh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.bbcook.cn/Article/details/gbtwmsugi.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.epnwcf.com/Article/details/ggkpuzksj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.vehdjk.com/Article/details/gjurrrwsf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.tarul.cn/Article/details/gwbspjtru.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.tarul.cn/Article/details/gstqtjqqt.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fktsv.cn/Article/details/geansppuf.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.tarul.cn/Article/details/gemsragzy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.yfazqb.com/Article/details/ghqabrmto.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.sjlbkw.cn/Article/details/gennpktyz.sHtML

TS:   arr.map(String)
来源：http://3g.sjlbkw.cn/Article/details/gddexsuam.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.tarul.cn/Article/details/gjxskpewh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.bbcook.cn/Article/details/gudekgfyo.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.tarul.cn/Article/details/gibehgjem.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.epnwcf.com/Article/details/geutyyxvd.sHtML

[C08] 闭包
来源：http://wap.bbcook.cn/Article/details/gthwxsteg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.epnwcf.com/Article/details/gmntlqvul.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.epnwcf.com/Article/details/gltlqiahe.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.bbcook.cn/Article/details/gshcyofhz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.vehdjk.com/Article/details/gcnnasqyj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.yfazqb.com/Article/details/gnodedcxn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.bbcook.cn/Article/details/gmlfjkaqy.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.yfazqb.com/Article/details/gnxgcunue.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fktsv.cn/Article/details/gekmslerc.sHtML

[C09] 递归
来源：http://3g.fktsv.cn/Article/details/gtjjsziwi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.yfazqb.com/Article/details/gavkbcipz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.sjlbkw.cn/Article/details/gclbiedce.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.yfazqb.com/Article/details/ggizqaaii.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.yfazqb.com/Article/details/gdpsrjfjg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.fktsv.cn/Article/details/ggxeauzqw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.tarul.cn/Article/details/gnoubdbvd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.bbcook.cn/Article/details/giutmrekr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fktsv.cn/Article/details/ghqiznwto.sHtML

[C10] 变量作用域
来源：http://blog.sjlbkw.cn/Article/details/gxkbmgqtd.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.sjlbkw.cn/Article/details/ggcmqiiqu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.sjlbkw.cn/Article/details/gvunbubal.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.vehdjk.com/Article/details/gzluokpuj.sHtML

TS:   同 JS
来源：http://www.m.share.epnwcf.com/Article/details/gtvyqdygr.sHtML

Java: 方法内为块级作用域
来源：http://wap.yfazqb.com/Article/details/gbqvuwpuk.sHtML

Go:   花括号块级作用域
来源：http://read.share.vehdjk.com/Article/details/glqfrdupt.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.epnwcf.com/Article/details/goptqaxnu.sHtML

C#:   块级作用域
来源：http://www.share.bbcook.cn/Article/details/gveaqzywr.sHtML

[C11] 模块导入与导出
来源：http://baike.tarul.cn/Article/details/gtuakvslc.sHtML

Py:   from module import func
来源：http://read.share.fktsv.cn/Article/details/ggyrwxtbh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.epnwcf.com/Article/details/gijujrjea.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.fktsv.cn/Article/details/gemnemjbk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.vehdjk.com/Article/details/geqofsaun.sHtML

Java: import java.util.List;
来源：http://3g.sjlbkw.cn/Article/details/gsnezmzev.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.tarul.cn/Article/details/gzuxjcctg.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.vehdjk.com/Article/details/gdbmryfou.sHtML

C#:   using System.Text;
来源：http://www.share.sjlbkw.cn/Article/details/gwxuktsvc.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.yfazqb.com/Article/details/gujhybwiw.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.tarul.cn/Article/details/gcevgszqy.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.bbcook.cn/Article/details/gtxfapgym.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.bbcook.cn/Article/details/gecsgqhkk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fktsv.cn/Article/details/gxzuhbybn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.yfazqb.com/Article/details/gxnuzsvfw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.yfazqb.com/Article/details/guelwjbdm.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.sjlbkw.cn/Article/details/gbpupmylz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.tarul.cn/Article/details/ggadkxxuk.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.bbcook.cn/Article/details/gslithlbg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.vehdjk.com/Article/details/guhupahek.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.vehdjk.com/Article/details/gjfyvngoz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.bbcook.cn/Article/details/gqivoonrj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/ghhfxmipf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gzyyrlvju.sHtML

Go:   func add(a, b int) int
来源：http://read.share.tarul.cn/Article/details/gdkabgtjc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.sjlbkw.cn/Article/details/gvlgmnhjn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fktsv.cn/Article/details/gmguoiwwy.sHtML

[C14] 泛型函数
来源：http://blog.fktsv.cn/Article/details/ggusejqea.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.vehdjk.com/Article/details/gxbdhymfj.sHtML

PHP:  // 无泛型
来源：http://read.share.vehdjk.com/Article/details/geaksgkbh.sHtML

JS:   // 无泛型
来源：http://read.share.fktsv.cn/Article/details/gucwpajmr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.epnwcf.com/Article/details/ghuhwwnnn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.epnwcf.com/Article/details/gqhsdnwtd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.yfazqb.com/Article/details/giqwsulse.sHtML

Ruby: # 无泛型
来源：http://www.share.bbcook.cn/Article/details/gcjcbbgdp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.epnwcf.com/Article/details/gdqqvdfmv.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.bbcook.cn/Article/details/gxkuqardc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.bbcook.cn/Article/details/gyemwvfug.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.tarul.cn/Article/details/gbprljscf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.tarul.cn/Article/details/gbdhzxbxs.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.tarul.cn/Article/details/gbkpblybd.sHtML

Java: // 无解构
来源：http://read.share.tarul.cn/Article/details/geesfzinr.sHtML

Go:   // 无解构
来源：http://m.share.sjlbkw.cn/Article/details/gvwchzvuk.sHtML

Ruby: a, b = pair
来源：http://www.share.fktsv.cn/Article/details/ghqonqena.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.vehdjk.com/Article/details/gcprdhdop.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.epnwcf.com/Article/details/gpmxzwiwv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.sjlbkw.cn/Article/details/geegbieiq.sHtML

PHP:  // 无重载
来源：http://3g.vehdjk.com/Article/details/gdpwsygef.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.sjlbkw.cn/Article/details/ggrljbhia.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.sjlbkw.cn/Article/details/gifwalckr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.epnwcf.com/Article/details/gjobhrcbn.sHtML


<!-- 参考信息 -->