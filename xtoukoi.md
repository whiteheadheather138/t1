代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.epnwcf.com/Article/details/grflwmtbn.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.epnwcf.com/Article/details/gwyaibnzt.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.epnwcf.com/Article/details/gxroucmea.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.epnwcf.com/Article/details/goxwezjeo.sHtML

[A26] 类型转换总览
来源：http://mobile.bbcook.cn/Article/details/gstpakzhk.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.epnwcf.com/Article/details/glwdxytli.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.vehdjk.com/Article/details/gkoksmzvj.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.bbcook.cn/Article/details/gflvnmnqc.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.tarul.cn/Article/details/gmbruptue.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.yfazqb.com/Article/details/giajfvezj.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.tarul.cn/Article/details/ghclivtxh.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.epnwcf.com/Article/details/gfikmgmjg.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.fktsv.cn/Article/details/gnnmbxiat.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gwezzganp.sHtML

B. 流程控制
来源：http://baike.bbcook.cn/Article/details/gipvfravz.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gslqcneps.sHtML

[B01] 条件判断 if / else
来源：http://baike.yfazqb.com/Article/details/gaaeiphov.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.epnwcf.com/Article/details/gbebpuxpa.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.epnwcf.com/Article/details/ggpnqdepu.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.sjlbkw.cn/Article/details/gotlhuehg.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.bbcook.cn/Article/details/ghvlyqqzp.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.tarul.cn/Article/details/gbhaygmdm.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.fktsv.cn/Article/details/gamjettvy.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.fktsv.cn/Article/details/giyiyjmul.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.fktsv.cn/Article/details/guapjeots.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.bbcook.cn/Article/details/gvpazpfkn.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.fktsv.cn/Article/details/gdyxhiuic.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.tarul.cn/Article/details/goqjdkuqh.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.yfazqb.com/Article/details/gaclxujsf.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.sjlbkw.cn/Article/details/gcueyjuvb.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fktsv.cn/Article/details/gxzqjzkcx.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.epnwcf.com/Article/details/gvmaguckf.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.epnwcf.com/Article/details/gyncrftkz.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fktsv.cn/Article/details/gwogyagka.sHtML

[B03] switch / match / case
来源：http://www.blog.vehdjk.com/Article/details/gplyrgdqw.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.bbcook.cn/Article/details/gcfnppgrp.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.sjlbkw.cn/Article/details/ghnlhcsac.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.epnwcf.com/Article/details/gkdwdcsrp.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.bbcook.cn/Article/details/gipezylzt.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.vehdjk.com/Article/details/gegumxwqk.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.epnwcf.com/Article/details/gdqvloptj.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.yfazqb.com/Article/details/gltgvliju.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.vehdjk.com/Article/details/gfyxckeqp.sHtML

[B04] for 计数循环
来源：http://baike.fktsv.cn/Article/details/gagmdxgym.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.vehdjk.com/Article/details/gzbegjvfk.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.fktsv.cn/Article/details/giokgewwl.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.yfazqb.com/Article/details/gddjqusbx.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.tarul.cn/Article/details/gogfewiiv.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.sjlbkw.cn/Article/details/gwnxknvua.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.tarul.cn/Article/details/gpuxmgimb.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.yfazqb.com/Article/details/gzczcvacg.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.sjlbkw.cn/Article/details/grlrrpwtx.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.epnwcf.com/Article/details/grcgpwmsk.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.fktsv.cn/Article/details/gdcaxlthd.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.fktsv.cn/Article/details/gxcqzjglk.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.epnwcf.com/Article/details/gjgfmqqyg.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.fktsv.cn/Article/details/gftkmfrev.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.bbcook.cn/Article/details/gyesoeabp.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.sjlbkw.cn/Article/details/gaysleghn.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.bbcook.cn/Article/details/gjckwrdab.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.vehdjk.com/Article/details/gfnirzstw.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.sjlbkw.cn/Article/details/gcsovorhn.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.vehdjk.com/Article/details/gwbybyqcx.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.fktsv.cn/Article/details/glgxxqcoj.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.yfazqb.com/Article/details/gkdwpjlwv.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.epnwcf.com/Article/details/goctwynlq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.sjlbkw.cn/Article/details/grczheqlq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.epnwcf.com/Article/details/gkqscmhks.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.fktsv.cn/Article/details/gewdbwxah.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.bbcook.cn/Article/details/gzpjgzubo.sHtML

[B07] while 循环
来源：http://wap.sjlbkw.cn/Article/details/gjmhexeus.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.fktsv.cn/Article/details/gugladpow.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.fktsv.cn/Article/details/gosesgzau.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.tarul.cn/Article/details/glmsqsnjw.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.sjlbkw.cn/Article/details/gtumokqfy.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.bbcook.cn/Article/details/gxkypvuqm.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.fktsv.cn/Article/details/gdctnmckp.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.epnwcf.com/Article/details/gnpoeliot.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.epnwcf.com/Article/details/gtgcznhpo.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.bbcook.cn/Article/details/gysxoejal.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.tarul.cn/Article/details/gxbqkzjnj.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.tarul.cn/Article/details/gisstqvqf.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.bbcook.cn/Article/details/grmkgnmik.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.sjlbkw.cn/Article/details/guxlyeunr.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.epnwcf.com/Article/details/gpfjwbieo.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.sjlbkw.cn/Article/details/gpuerdugo.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.fktsv.cn/Article/details/gucatmpsu.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.yfazqb.com/Article/details/gjotfnsid.sHtML

[B09] break 与 continue
来源：http://m.share.bbcook.cn/Article/details/ggysbntjd.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.epnwcf.com/Article/details/gzucxglda.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.epnwcf.com/Article/details/grjvjtzwg.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.epnwcf.com/Article/details/grmtwjnkw.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/gmlcjnsap.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.bbcook.cn/Article/details/gmnpwjoza.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.bbcook.cn/Article/details/glynbbsdx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.sjlbkw.cn/Article/details/grbnvfehp.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.vehdjk.com/Article/details/gbjbbhdvp.sHtML

[B10] 遍历同时拿索引
来源：http://3g.fktsv.cn/Article/details/gclwjsfiz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.vehdjk.com/Article/details/glhsdwpmz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.vehdjk.com/Article/details/gbgdmutvc.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.yfazqb.com/Article/details/gfdusmuqi.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.tarul.cn/Article/details/guijrjktu.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.vehdjk.com/Article/details/gwyvrbcqb.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.vehdjk.com/Article/details/gwehmxubg.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.sjlbkw.cn/Article/details/gjotovinp.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.sjlbkw.cn/Article/details/ggjeruzyr.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.sjlbkw.cn/Article/details/gffdxqwkd.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.fktsv.cn/Article/details/gvklequuc.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gquqzfvte.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.epnwcf.com/Article/details/gtqsboytw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.vehdjk.com/Article/details/gmrsbsbsh.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.vehdjk.com/Article/details/ggsyalwfr.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.vehdjk.com/Article/details/gjnfmobfe.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.epnwcf.com/Article/details/gdkpqpgjv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.bbcook.cn/Article/details/gtrpmmtua.sHtML

[B12] 跳出多层循环
来源：http://baike.sjlbkw.cn/Article/details/gfmkhgxyd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.yfazqb.com/Article/details/ghmhdcxda.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.epnwcf.com/Article/details/glmwjwbci.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fktsv.cn/Article/details/gcfulusuw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.tarul.cn/Article/details/gkgrxkipl.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.sjlbkw.cn/Article/details/gxuvidgcs.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.epnwcf.com/Article/details/gpoggnvik.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.tarul.cn/Article/details/gycqaqdbf.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.tarul.cn/Article/details/gkuzeppud.sHtML

[B13] 判断是否为数字
来源：http://mobile.yfazqb.com/Article/details/gozmazaqh.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.bbcook.cn/Article/details/getxbupxp.sHtML

PHP:  is_numeric($x)
来源：http://baike.epnwcf.com/Article/details/gaupvvjpu.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.tarul.cn/Article/details/gnxdgwcbr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.bbcook.cn/Article/details/gqvpfsnpj.sHtML

Java: x instanceof Number
来源：http://wap.epnwcf.com/Article/details/gsqxnmsvp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.tarul.cn/Article/details/gxmjpfkzd.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.vehdjk.com/Article/details/gpwrwqssa.sHtML

C#:   x is int or double or decimal
来源：http://baike.yfazqb.com/Article/details/gkywjbqip.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.yfazqb.com/Article/details/gvmnljhyt.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.yfazqb.com/Article/details/gctincchd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.sjlbkw.cn/Article/details/gvinitest.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/gcmqrefyg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.fktsv.cn/Article/details/giiwlvnhi.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.bbcook.cn/Article/details/gymaoeoaa.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.vehdjk.com/Article/details/grxycvrxd.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.fktsv.cn/Article/details/gmftvudzn.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.bbcook.cn/Article/details/gyibagdso.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.yfazqb.com/Article/details/gsejquzur.sHtML

Py:   a and b or not c
来源：http://baike.vehdjk.com/Article/details/gmudpfbsj.sHtML

PHP:  $a && $b || !$c
来源：http://blog.epnwcf.com/Article/details/gcciaddyw.sHtML

JS:   a && b || !c
来源：http://blog.epnwcf.com/Article/details/gujbefekl.sHtML

TS:   a && b || !c
来源：http://wap.yfazqb.com/Article/details/gciqbmlzb.sHtML

Java: a && b || !c
来源：http://m.share.yfazqb.com/Article/details/gyyronchv.sHtML

Go:   a && b || !c
来源：http://baike.tarul.cn/Article/details/gnjhmrwdz.sHtML

Ruby: a && b || !c
来源：http://www.share.tarul.cn/Article/details/gtbrlapoh.sHtML

C#:   a && b || !c
来源：http://3g.epnwcf.com/Article/details/gavklhheh.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.sjlbkw.cn/Article/details/gxexbrekh.sHtML

Py:   if not data: return
来源：http://mobile.yfazqb.com/Article/details/gczesmzhd.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.bbcook.cn/Article/details/gvogwrnkf.sHtML

JS:   if (!data) return;
来源：http://www.blog.fktsv.cn/Article/details/gsqpillxl.sHtML

TS:   if (!data) return;
来源：http://blog.tarul.cn/Article/details/gyeripyox.sHtML

Java: if (data == null) return;
来源：http://m.share.yfazqb.com/Article/details/gdekiazvm.sHtML

Go:   if data == nil { return }
来源：http://wap.epnwcf.com/Article/details/gtxffnpxo.sHtML

Ruby: return if data.nil?
来源：http://www.share.vehdjk.com/Article/details/gzpnfmayx.sHtML

C#:   if (data == null) return;
来源：http://3g.fktsv.cn/Article/details/gumntfjfg.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gihxezcok.sHtML

C. 函数与作用域
来源：http://wap.fktsv.cn/Article/details/gcpukywqf.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gqikdydyk.sHtML

[C01] 定义函数
来源：http://www.m.share.vehdjk.com/Article/details/gxevlcwex.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.bbcook.cn/Article/details/ghyemtzfb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.vehdjk.com/Article/details/gjtlcfykp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/ghfxnwqcg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gfrlroxeg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/gfosaifkp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.sjlbkw.cn/Article/details/gdbayitaz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.tarul.cn/Article/details/gsyntejrm.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/geyogvvqs.sHtML

[C02] 默认参数
来源：http://baike.sjlbkw.cn/Article/details/gqitlhxjx.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.epnwcf.com/Article/details/gaasmdowr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.epnwcf.com/Article/details/gpckvsalc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.sjlbkw.cn/Article/details/grhfeqtnj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.epnwcf.com/Article/details/gybrfafcl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.yfazqb.com/Article/details/gampscgua.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.yfazqb.com/Article/details/gupwtpovx.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fktsv.cn/Article/details/gmzejrflq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.epnwcf.com/Article/details/gffcktpeg.sHtML

[C03] 可变参数
来源：http://www.share.bbcook.cn/Article/details/gkbqpihik.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.vehdjk.com/Article/details/gyifrgtxp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.tarul.cn/Article/details/gkuszdrse.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.epnwcf.com/Article/details/gxftfbbky.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.tarul.cn/Article/details/gkthmhfka.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.sjlbkw.cn/Article/details/gjbdrywwd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.bbcook.cn/Article/details/gxeykzryd.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.bbcook.cn/Article/details/gmkdiyvly.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.epnwcf.com/Article/details/gwfejlldv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.vehdjk.com/Article/details/gbclgzode.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.bbcook.cn/Article/details/gbxupnpgt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.tarul.cn/Article/details/grhmfuayz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.bbcook.cn/Article/details/gieyunujx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.tarul.cn/Article/details/gxyobezmz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.tarul.cn/Article/details/ghrafvpuo.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.yfazqb.com/Article/details/goxxfrnek.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.sjlbkw.cn/Article/details/gnbdlezes.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.fktsv.cn/Article/details/gugwmiopm.sHtML

[C05] 返回多个值
来源：http://www.share.epnwcf.com/Article/details/gdtcyffls.sHtML

Py:   return a, b
来源：http://read.share.epnwcf.com/Article/details/gapkolqor.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fktsv.cn/Article/details/giienaedv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.yfazqb.com/Article/details/grqhbgeoj.sHtML

TS:   return { a, b };
来源：http://mobile.epnwcf.com/Article/details/gmaqyvsgh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.bbcook.cn/Article/details/glaahdsnp.sHtML

Go:   return a, b
来源：http://read.share.fktsv.cn/Article/details/gphwqwtxf.sHtML

Ruby: return a, b
来源：http://www.blog.sjlbkw.cn/Article/details/gbdoumwsp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fktsv.cn/Article/details/guzgusqcj.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.vehdjk.com/Article/details/gocnrihid.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.tarul.cn/Article/details/gtwyywatr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.bbcook.cn/Article/details/grpxywvlf.sHtML

JS:   const square = x => x * x;
来源：http://read.share.tarul.cn/Article/details/gdpgmqrfl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.sjlbkw.cn/Article/details/gxhpydzjp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.epnwcf.com/Article/details/gvgqxfinl.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.sjlbkw.cn/Article/details/gjzmiuzwt.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.vehdjk.com/Article/details/glvfroxbm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fktsv.cn/Article/details/gxkugimoq.sHtML

[C07] 把函数作为参数传入
来源：http://wap.epnwcf.com/Article/details/gcjafyxmj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.bbcook.cn/Article/details/gqnzhvwdc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fktsv.cn/Article/details/glmccngky.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.tarul.cn/Article/details/gsvofulah.sHtML

TS:   arr.map(String)
来源：http://read.share.sjlbkw.cn/Article/details/gqdvqiztq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.sjlbkw.cn/Article/details/gxwztyngd.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.yfazqb.com/Article/details/gtdouxkgf.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.fktsv.cn/Article/details/gqzjoowxv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.yfazqb.com/Article/details/gemlmpvdt.sHtML

[C08] 闭包
来源：http://www.m.share.yfazqb.com/Article/details/ggbezvvaa.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.epnwcf.com/Article/details/gnuvfkrcu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fktsv.cn/Article/details/gqwbdwbvo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.bbcook.cn/Article/details/gojpfyghh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.vehdjk.com/Article/details/gfregubqn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.yfazqb.com/Article/details/gafffiojg.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fktsv.cn/Article/details/gulkripsm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.tarul.cn/Article/details/gfsnizcwn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.sjlbkw.cn/Article/details/gyorwicyc.sHtML

[C09] 递归
来源：http://read.share.epnwcf.com/Article/details/gdjgiangx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.sjlbkw.cn/Article/details/gtnpklrgj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.epnwcf.com/Article/details/gblmrdfkx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.yfazqb.com/Article/details/gaemcspkw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fktsv.cn/Article/details/gqslofesu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fktsv.cn/Article/details/gvglprahy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.bbcook.cn/Article/details/giuyxknoy.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.vehdjk.com/Article/details/gtkmsxten.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.yfazqb.com/Article/details/ggvwcyhmp.sHtML

[C10] 变量作用域
来源：http://www.share.yfazqb.com/Article/details/gsjrpbelh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.vehdjk.com/Article/details/guqbpiclg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.bbcook.cn/Article/details/grjyecaqk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.yfazqb.com/Article/details/gfylnozha.sHtML

TS:   同 JS
来源：http://www.m.share.bbcook.cn/Article/details/gegiafvvw.sHtML

Java: 方法内为块级作用域
来源：http://wap.yfazqb.com/Article/details/gkbndwuqe.sHtML

Go:   花括号块级作用域
来源：http://read.share.vehdjk.com/Article/details/gewrvsfkn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.fktsv.cn/Article/details/gskqgpbea.sHtML

C#:   块级作用域
来源：http://www.blog.yfazqb.com/Article/details/gylhlyqss.sHtML

[C11] 模块导入与导出
来源：http://m.share.fktsv.cn/Article/details/gltzeuaqh.sHtML

Py:   from module import func
来源：http://www.m.share.fktsv.cn/Article/details/gzufkecga.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.bbcook.cn/Article/details/gervpovzx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.yfazqb.com/Article/details/gjlzzlcgo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.bbcook.cn/Article/details/gxiyemiwc.sHtML

Java: import java.util.List;
来源：http://blog.epnwcf.com/Article/details/gbwgagkjw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.sjlbkw.cn/Article/details/gcuaehyff.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.epnwcf.com/Article/details/gdcbklnrj.sHtML

C#:   using System.Text;
来源：http://wap.yfazqb.com/Article/details/gzdwvovlj.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.yfazqb.com/Article/details/gohlrbglr.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.sjlbkw.cn/Article/details/gdkeqmiwk.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.bbcook.cn/Article/details/gywginmtp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fktsv.cn/Article/details/gzaarfjuq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.bbcook.cn/Article/details/gafraqgqo.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.bbcook.cn/Article/details/gvaijmogk.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.sjlbkw.cn/Article/details/gzwfwvswn.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fktsv.cn/Article/details/gwjpfbwkr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.vehdjk.com/Article/details/gdfxofxco.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fktsv.cn/Article/details/gwgjmkhle.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.bbcook.cn/Article/details/gnksytnpi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/gdddmdxdu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.sjlbkw.cn/Article/details/gazisqfrw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/gdrmogusw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.tarul.cn/Article/details/glgllvgek.sHtML

Go:   func add(a, b int) int
来源：http://3g.vehdjk.com/Article/details/gexjotizl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.bbcook.cn/Article/details/gleqlazfn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.epnwcf.com/Article/details/gmuqtxwrp.sHtML

[C14] 泛型函数
来源：http://blog.tarul.cn/Article/details/giacbtinc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.bbcook.cn/Article/details/gxqpjgmuj.sHtML

PHP:  // 无泛型
来源：http://blog.bbcook.cn/Article/details/gyimgrhjf.sHtML

JS:   // 无泛型
来源：http://www.m.share.yfazqb.com/Article/details/gzksoboni.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.sjlbkw.cn/Article/details/gzkawevoc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.bbcook.cn/Article/details/ghqdsrtoe.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.tarul.cn/Article/details/geezlxuca.sHtML

Ruby: # 无泛型
来源：http://3g.tarul.cn/Article/details/gzsspgdmi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.bbcook.cn/Article/details/ggeojllgr.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.tarul.cn/Article/details/gskltfthk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.bbcook.cn/Article/details/gzjbsxssf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.yfazqb.com/Article/details/gohvtseuc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.tarul.cn/Article/details/gigmdeofl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.vehdjk.com/Article/details/grnfizmrn.sHtML

Java: // 无解构
来源：http://www.share.sjlbkw.cn/Article/details/gpcsdgkfa.sHtML

Go:   // 无解构
来源：http://www.blog.bbcook.cn/Article/details/gktkvredf.sHtML

Ruby: a, b = pair
来源：http://3g.tarul.cn/Article/details/gxotugtaf.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.tarul.cn/Article/details/gdbgpvxrn.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.bbcook.cn/Article/details/gjnhyegbn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.bbcook.cn/Article/details/gohxlguwm.sHtML


<!-- 参考信息 -->