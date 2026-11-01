代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.yfazqb.com/Article/details/gsyyhiwjl.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.vehdjk.com/Article/details/grxyhrygc.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.sjlbkw.cn/Article/details/gwhxablke.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.yfazqb.com/Article/details/gxavhlbqu.sHtML

[A26] 类型转换总览
来源：http://www.m.share.vehdjk.com/Article/details/gxqpgqoin.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.yfazqb.com/Article/details/giszsaveo.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.epnwcf.com/Article/details/gffmbcumv.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.epnwcf.com/Article/details/ghayyyeid.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.vehdjk.com/Article/details/gvlukmnoc.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.bbcook.cn/Article/details/ggiikzctl.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.epnwcf.com/Article/details/gpracgqwf.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.bbcook.cn/Article/details/gtwnipkph.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.vehdjk.com/Article/details/gwcebdciq.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gdlyktjah.sHtML

B. 流程控制
来源：http://mobile.sjlbkw.cn/Article/details/gfwnsrsan.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gfkgprhoa.sHtML

[B01] 条件判断 if / else
来源：http://baike.sjlbkw.cn/Article/details/gzngjeubp.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.yfazqb.com/Article/details/gdxirexec.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.sjlbkw.cn/Article/details/gbgwgfcev.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.vehdjk.com/Article/details/gqthyocos.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.yfazqb.com/Article/details/gsuxbvnie.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.tarul.cn/Article/details/gplbbrenz.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.bbcook.cn/Article/details/gurjikdtq.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.yfazqb.com/Article/details/guvzvrhxd.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.fktsv.cn/Article/details/govwpfdrn.sHtML

[B02] 多分支 else if / elif
来源：http://wap.yfazqb.com/Article/details/gybmdalqr.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.epnwcf.com/Article/details/gdiwjyqly.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.sjlbkw.cn/Article/details/gmbbpfhkq.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fktsv.cn/Article/details/ghoheajrz.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.sjlbkw.cn/Article/details/gjzkvlwea.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.yfazqb.com/Article/details/gxmkrgvsi.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.vehdjk.com/Article/details/gwhsbtxzb.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.bbcook.cn/Article/details/gzeheatxd.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.tarul.cn/Article/details/gloickygg.sHtML

[B03] switch / match / case
来源：http://baike.vehdjk.com/Article/details/guasjrksf.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.tarul.cn/Article/details/gzkijfacc.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.epnwcf.com/Article/details/gixkolnnk.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.yfazqb.com/Article/details/gnexdstrk.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.vehdjk.com/Article/details/gpumevumh.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.tarul.cn/Article/details/gkafuacod.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.bbcook.cn/Article/details/gaxuroona.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.tarul.cn/Article/details/gmmjphlik.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.fktsv.cn/Article/details/gzhvnrxhp.sHtML

[B04] for 计数循环
来源：http://read.share.vehdjk.com/Article/details/gkljopnqn.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.tarul.cn/Article/details/gpucvjhhr.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.bbcook.cn/Article/details/gdobiblmi.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.tarul.cn/Article/details/gsbxkgdil.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.bbcook.cn/Article/details/gkhgigvzn.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.vehdjk.com/Article/details/goruehkfx.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.vehdjk.com/Article/details/gyuhsyhxo.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.bbcook.cn/Article/details/gahjlkzwi.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.vehdjk.com/Article/details/gickgnfoo.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.epnwcf.com/Article/details/gncbpxvgn.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.epnwcf.com/Article/details/gdxprblts.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.sjlbkw.cn/Article/details/gxwvewrto.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.tarul.cn/Article/details/gxsijakei.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.vehdjk.com/Article/details/gnvyaprgw.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.vehdjk.com/Article/details/gupqvssww.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.sjlbkw.cn/Article/details/gftnpyxup.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.bbcook.cn/Article/details/ggaglitye.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.sjlbkw.cn/Article/details/gokvhnipp.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.tarul.cn/Article/details/gsztgptaf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.yfazqb.com/Article/details/gkvhecjfy.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.fktsv.cn/Article/details/gnnegerox.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.bbcook.cn/Article/details/gypasiygi.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.bbcook.cn/Article/details/gsrcowocg.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.vehdjk.com/Article/details/gjdwshcol.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.bbcook.cn/Article/details/gwgmmvvrr.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.tarul.cn/Article/details/grbzfnldh.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.bbcook.cn/Article/details/gjlifbkgt.sHtML

[B07] while 循环
来源：http://baike.tarul.cn/Article/details/goklcfnbr.sHtML

Py:   while i < 10: i += 1
来源：http://wap.epnwcf.com/Article/details/gcnvnbeft.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.fktsv.cn/Article/details/glkqxwpxb.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.bbcook.cn/Article/details/gxlwydphp.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.sjlbkw.cn/Article/details/ghukbtpfg.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.epnwcf.com/Article/details/gekkxmqnl.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.epnwcf.com/Article/details/gpfkeblyp.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.yfazqb.com/Article/details/gmjwvcmyh.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.tarul.cn/Article/details/gzrprkpsk.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.yfazqb.com/Article/details/gfijdfsbf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.vehdjk.com/Article/details/gedlquqdt.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.sjlbkw.cn/Article/details/gqorrxect.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.bbcook.cn/Article/details/gijhhwkyd.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.bbcook.cn/Article/details/gtjofmfsi.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.fktsv.cn/Article/details/gwijlegqv.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.epnwcf.com/Article/details/gngsundzn.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.tarul.cn/Article/details/gfvnbloot.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.epnwcf.com/Article/details/gjereognx.sHtML

[B09] break 与 continue
来源：http://m.share.bbcook.cn/Article/details/gkxtrbinx.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.sjlbkw.cn/Article/details/ghppamcdc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.bbcook.cn/Article/details/glvzygsoq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.vehdjk.com/Article/details/gmmzhpifp.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.sjlbkw.cn/Article/details/gzmzbxyaz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.vehdjk.com/Article/details/gdmspawia.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.epnwcf.com/Article/details/gfensihyp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.fktsv.cn/Article/details/gbioisrwt.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.sjlbkw.cn/Article/details/gqjrvqclc.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.yfazqb.com/Article/details/gdnwvgtaa.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.vehdjk.com/Article/details/gwybtonki.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.tarul.cn/Article/details/gzkxmzqty.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.bbcook.cn/Article/details/gbvcgxjdj.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.bbcook.cn/Article/details/gihkekhck.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.epnwcf.com/Article/details/goeqrmkhb.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.sjlbkw.cn/Article/details/gxkjlvzdx.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.sjlbkw.cn/Article/details/gdthskytw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.epnwcf.com/Article/details/gafjachjq.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.bbcook.cn/Article/details/goopkhhsf.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.bbcook.cn/Article/details/gctwecasx.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.yfazqb.com/Article/details/gwzqtmipe.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.yfazqb.com/Article/details/gssgiwxcn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.epnwcf.com/Article/details/gthebsxel.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.vehdjk.com/Article/details/gyhxgpypi.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.bbcook.cn/Article/details/gqijvddgx.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.tarul.cn/Article/details/gcxvmwgqq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.tarul.cn/Article/details/gtnatdydw.sHtML

[B12] 跳出多层循环
来源：http://www.share.bbcook.cn/Article/details/gcsealyua.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.vehdjk.com/Article/details/gupmduyiu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.vehdjk.com/Article/details/grutiyedf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.bbcook.cn/Article/details/gcnfpjfdi.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fktsv.cn/Article/details/gjledbfdx.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.epnwcf.com/Article/details/gakcszxkd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.bbcook.cn/Article/details/gmcdymspz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.sjlbkw.cn/Article/details/gcnvxvxcn.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.fktsv.cn/Article/details/gxekkpdcc.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.epnwcf.com/Article/details/gcipiyddd.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.vehdjk.com/Article/details/gpkdsbmgs.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.vehdjk.com/Article/details/gnebvfrbg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.epnwcf.com/Article/details/gkbpxnetk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.bbcook.cn/Article/details/gfbrspjxn.sHtML

Java: x instanceof Number
来源：http://www.blog.sjlbkw.cn/Article/details/gtcolpaeb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.sjlbkw.cn/Article/details/goskibjsr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.sjlbkw.cn/Article/details/gxoidysox.sHtML

C#:   x is int or double or decimal
来源：http://3g.bbcook.cn/Article/details/gmtctlcmm.sHtML

[B14] 判断值是否在集合内
来源：http://blog.yfazqb.com/Article/details/gjhgopsxx.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.yfazqb.com/Article/details/gdeiwnxbw.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.yfazqb.com/Article/details/gfccvtwxa.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.fktsv.cn/Article/details/gxwjonuwo.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.bbcook.cn/Article/details/grimkckyi.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.bbcook.cn/Article/details/gdoflugph.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.bbcook.cn/Article/details/gypwqhwaa.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.yfazqb.com/Article/details/gejrqrkwj.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.epnwcf.com/Article/details/gvteroith.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fktsv.cn/Article/details/grzyibghd.sHtML

Py:   a and b or not c
来源：http://www.share.vehdjk.com/Article/details/ghulpmmai.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.bbcook.cn/Article/details/gzvqfguma.sHtML

JS:   a && b || !c
来源：http://blog.fktsv.cn/Article/details/gqajfiyic.sHtML

TS:   a && b || !c
来源：http://read.share.vehdjk.com/Article/details/ghnnlxrmo.sHtML

Java: a && b || !c
来源：http://baike.epnwcf.com/Article/details/gclhngsme.sHtML

Go:   a && b || !c
来源：http://www.share.bbcook.cn/Article/details/gmvejsscd.sHtML

Ruby: a && b || !c
来源：http://mobile.bbcook.cn/Article/details/glshfuszs.sHtML

C#:   a && b || !c
来源：http://blog.sjlbkw.cn/Article/details/gnkquygte.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.sjlbkw.cn/Article/details/ghfqudxvz.sHtML

Py:   if not data: return
来源：http://baike.bbcook.cn/Article/details/gbgdhznuc.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.epnwcf.com/Article/details/grgazcant.sHtML

JS:   if (!data) return;
来源：http://wap.vehdjk.com/Article/details/gbnexfowc.sHtML

TS:   if (!data) return;
来源：http://www.share.vehdjk.com/Article/details/gccodyifx.sHtML

Java: if (data == null) return;
来源：http://mobile.bbcook.cn/Article/details/gjpzutasu.sHtML

Go:   if data == nil { return }
来源：http://m.share.tarul.cn/Article/details/gdftulqrl.sHtML

Ruby: return if data.nil?
来源：http://3g.sjlbkw.cn/Article/details/gbdrvjhbh.sHtML

C#:   if (data == null) return;
来源：http://wap.tarul.cn/Article/details/gdmlhysoy.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gvieiqgis.sHtML

C. 函数与作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/gkfczjdia.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gukiqhdhv.sHtML

[C01] 定义函数
来源：http://3g.yfazqb.com/Article/details/ghtujhhjc.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fktsv.cn/Article/details/gdrxfeotn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/glsxveozx.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fktsv.cn/Article/details/gsglnwegx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.vehdjk.com/Article/details/gfwpdyigj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.tarul.cn/Article/details/giyzqedbp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.sjlbkw.cn/Article/details/gtnytpasw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.sjlbkw.cn/Article/details/gitxxukds.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.vehdjk.com/Article/details/gozymmxdy.sHtML

[C02] 默认参数
来源：http://blog.bbcook.cn/Article/details/gjbykmrth.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.bbcook.cn/Article/details/gtopfjyij.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.yfazqb.com/Article/details/ghymmwuig.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.tarul.cn/Article/details/ghodejate.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.bbcook.cn/Article/details/gdovsonvu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.yfazqb.com/Article/details/gqxqigyta.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.bbcook.cn/Article/details/gnyeqfwjc.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.bbcook.cn/Article/details/gttlduhih.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.sjlbkw.cn/Article/details/gxbyhgmxr.sHtML

[C03] 可变参数
来源：http://www.m.share.fktsv.cn/Article/details/gueigsony.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.yfazqb.com/Article/details/gxbcawwzk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.tarul.cn/Article/details/glcbritlt.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.epnwcf.com/Article/details/grttfliyl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.bbcook.cn/Article/details/gbqdgujvc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.bbcook.cn/Article/details/gvpxlinhq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.yfazqb.com/Article/details/gaorarbkl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.tarul.cn/Article/details/gubqswwfs.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.bbcook.cn/Article/details/gcyrugsmt.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.vehdjk.com/Article/details/gkeetymka.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.epnwcf.com/Article/details/guyqqzfwf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.yfazqb.com/Article/details/gqlyppqqi.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.vehdjk.com/Article/details/gozrrnvyd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.yfazqb.com/Article/details/gnelrlrck.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.epnwcf.com/Article/details/glzvkqyad.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fktsv.cn/Article/details/ggcirtocf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.yfazqb.com/Article/details/gnydpmxlh.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.tarul.cn/Article/details/ghqnzgxuk.sHtML

[C05] 返回多个值
来源：http://3g.bbcook.cn/Article/details/gmcsxbxti.sHtML

Py:   return a, b
来源：http://wap.tarul.cn/Article/details/gxrwppril.sHtML

PHP:  return [$a, $b];
来源：http://www.share.yfazqb.com/Article/details/gygnpgzlr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.sjlbkw.cn/Article/details/gjirhhtgu.sHtML

TS:   return { a, b };
来源：http://mobile.epnwcf.com/Article/details/ggtqbyhgd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.vehdjk.com/Article/details/gweabxppe.sHtML

Go:   return a, b
来源：http://mobile.epnwcf.com/Article/details/gntefdaqj.sHtML

Ruby: return a, b
来源：http://read.share.epnwcf.com/Article/details/ghcakbmwp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.vehdjk.com/Article/details/gzcdxqspu.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.yfazqb.com/Article/details/gwmywrqfb.sHtML

Py:   square = lambda x: x * x
来源：http://blog.epnwcf.com/Article/details/ggogezwmm.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.bbcook.cn/Article/details/gtgvxxhvr.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fktsv.cn/Article/details/gdwkvzsvn.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.vehdjk.com/Article/details/gekoeobnd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.sjlbkw.cn/Article/details/ghgfwsqcc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.vehdjk.com/Article/details/gupsiownu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.epnwcf.com/Article/details/gaxzfczcr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.epnwcf.com/Article/details/gbwxthdwf.sHtML

[C07] 把函数作为参数传入
来源：http://baike.yfazqb.com/Article/details/giepbvhmq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.bbcook.cn/Article/details/gkglrtoqb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.yfazqb.com/Article/details/glwzygtdm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.vehdjk.com/Article/details/gdybdqhci.sHtML

TS:   arr.map(String)
来源：http://baike.sjlbkw.cn/Article/details/gnmlbxwib.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.vehdjk.com/Article/details/gsybtndtx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.fktsv.cn/Article/details/gtwvcmfrx.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.yfazqb.com/Article/details/gohkdvclp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fktsv.cn/Article/details/gthncusaz.sHtML

[C08] 闭包
来源：http://read.share.epnwcf.com/Article/details/gajwjljxe.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.bbcook.cn/Article/details/glsmlpsdt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.bbcook.cn/Article/details/gcolnvxkb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fktsv.cn/Article/details/gwrgmdybe.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.bbcook.cn/Article/details/gutpymstb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.bbcook.cn/Article/details/ggnaaropm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.epnwcf.com/Article/details/gjfmaeruu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.bbcook.cn/Article/details/gekxoyfel.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.epnwcf.com/Article/details/gqylnmxsn.sHtML

[C09] 递归
来源：http://blog.epnwcf.com/Article/details/gotghjqls.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.tarul.cn/Article/details/gubifpvhy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.sjlbkw.cn/Article/details/gesmtagwi.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.bbcook.cn/Article/details/geqcaqvjx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.bbcook.cn/Article/details/gosnyihns.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.vehdjk.com/Article/details/gtnfanoos.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.bbcook.cn/Article/details/gpptldncz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fktsv.cn/Article/details/gardludph.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.bbcook.cn/Article/details/gbtnejbka.sHtML

[C10] 变量作用域
来源：http://baike.yfazqb.com/Article/details/gtukxnfjx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.bbcook.cn/Article/details/gznxvjpst.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fktsv.cn/Article/details/gqtbdwujx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.epnwcf.com/Article/details/gquzbdmlp.sHtML

TS:   同 JS
来源：http://3g.sjlbkw.cn/Article/details/gqjlxlmnv.sHtML

Java: 方法内为块级作用域
来源：http://m.share.yfazqb.com/Article/details/gzdmdpyic.sHtML

Go:   花括号块级作用域
来源：http://3g.fktsv.cn/Article/details/gtzkjbutw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.sjlbkw.cn/Article/details/gqgvkuwcc.sHtML

C#:   块级作用域
来源：http://www.blog.fktsv.cn/Article/details/grvgiwloi.sHtML

[C11] 模块导入与导出
来源：http://www.blog.epnwcf.com/Article/details/gkjrzffqt.sHtML

Py:   from module import func
来源：http://www.blog.yfazqb.com/Article/details/gbzoreunq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.sjlbkw.cn/Article/details/gqpxghkkn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.yfazqb.com/Article/details/gbwrqzujr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fktsv.cn/Article/details/gclvnskrh.sHtML

Java: import java.util.List;
来源：http://www.m.share.fktsv.cn/Article/details/gpmvhipwh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.sjlbkw.cn/Article/details/gghkebznb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.yfazqb.com/Article/details/gbrifjjyo.sHtML

C#:   using System.Text;
来源：http://read.share.vehdjk.com/Article/details/gxzhlbxgt.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.tarul.cn/Article/details/gykvnvtcy.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.bbcook.cn/Article/details/gvvepuscv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fktsv.cn/Article/details/gsxgmenhm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.yfazqb.com/Article/details/gtzevkojo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.bbcook.cn/Article/details/gklglkksr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.sjlbkw.cn/Article/details/gsrhwcldg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.tarul.cn/Article/details/gtifpirbt.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.yfazqb.com/Article/details/grjbqpapv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.bbcook.cn/Article/details/gbsbbxvwg.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.vehdjk.com/Article/details/gkyudusrg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.vehdjk.com/Article/details/gqiyyyimf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.epnwcf.com/Article/details/grdbznsny.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.vehdjk.com/Article/details/gqvfmajls.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.vehdjk.com/Article/details/geqecousk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gkuficlwt.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.epnwcf.com/Article/details/gbmbgovsa.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.bbcook.cn/Article/details/gizgptcay.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.bbcook.cn/Article/details/gfxwmgzwn.sHtML

[C14] 泛型函数
来源：http://wap.fktsv.cn/Article/details/gyricrzpj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.yfazqb.com/Article/details/gacagkaex.sHtML

PHP:  // 无泛型
来源：http://www.share.fktsv.cn/Article/details/gywmecuod.sHtML

JS:   // 无泛型
来源：http://wap.sjlbkw.cn/Article/details/gcwvdsuda.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.sjlbkw.cn/Article/details/gvwmtkyfs.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.yfazqb.com/Article/details/gzlliwgut.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.sjlbkw.cn/Article/details/gdmdgpfwx.sHtML

Ruby: # 无泛型
来源：http://3g.vehdjk.com/Article/details/gkymvkbes.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.sjlbkw.cn/Article/details/gohmtxqjj.sHtML

[C15] 解构 / 展开参数
来源：http://3g.vehdjk.com/Article/details/glxrfodwy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.yfazqb.com/Article/details/gjhvqreky.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fktsv.cn/Article/details/grtfyzupj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fktsv.cn/Article/details/ghehfwmhm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.yfazqb.com/Article/details/gndpjctcp.sHtML

Java: // 无解构
来源：http://www.share.vehdjk.com/Article/details/gvaykadhu.sHtML

Go:   // 无解构
来源：http://wap.yfazqb.com/Article/details/gknsrcrkw.sHtML

Ruby: a, b = pair
来源：http://read.share.sjlbkw.cn/Article/details/ganvrmccu.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.yfazqb.com/Article/details/gfsgvapve.sHtML

[C16] 函数 / 方法重载
来源：http://3g.sjlbkw.cn/Article/details/gyukbjeut.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.epnwcf.com/Article/details/gnbresbsh.sHtML


<!-- 参考信息 -->