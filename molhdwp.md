代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://mobile.fktsv.cn/Article/details/ghgkbxeau.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.sjlbkw.cn/Article/details/gqicvpwyt.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.sjlbkw.cn/Article/details/gtjsvvzcy.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.vehdjk.com/Article/details/grdogcclu.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.epnwcf.com/Article/details/gkthtxgbx.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.yfazqb.com/Article/details/gcfmhmhdq.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.tarul.cn/Article/details/grblnmpam.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.sjlbkw.cn/Article/details/ggowkhgbg.sHtML

[A26] 类型转换总览
来源：http://www.blog.vehdjk.com/Article/details/glanthxzz.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.epnwcf.com/Article/details/ggrndjnur.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.yfazqb.com/Article/details/gmtrehvnx.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.epnwcf.com/Article/details/gfguybgkq.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.fktsv.cn/Article/details/geusjqyky.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.tarul.cn/Article/details/goiypkxxw.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.epnwcf.com/Article/details/gxnimnqxj.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.bbcook.cn/Article/details/gdgidrxvi.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.sjlbkw.cn/Article/details/gpspjtqlz.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gyfwzzcuj.sHtML

B. 流程控制
来源：http://www.m.share.vehdjk.com/Article/details/gygyxvrtr.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gssiddwwj.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.epnwcf.com/Article/details/gkpnihrek.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.sjlbkw.cn/Article/details/gvewblowl.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.fktsv.cn/Article/details/gnkuxwvtn.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.epnwcf.com/Article/details/grriqixgu.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.bbcook.cn/Article/details/grnrxllwv.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.vehdjk.com/Article/details/glwyhlzad.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.bbcook.cn/Article/details/glnhjauxf.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.yfazqb.com/Article/details/ghsphvdet.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.vehdjk.com/Article/details/gjimadazj.sHtML

[B02] 多分支 else if / elif
来源：http://wap.vehdjk.com/Article/details/glvihrwoz.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.yfazqb.com/Article/details/gehcbapec.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.epnwcf.com/Article/details/gsuzlrebz.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.sjlbkw.cn/Article/details/gqytbbhhi.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.yfazqb.com/Article/details/gtggisfhh.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fktsv.cn/Article/details/gkoyzxvmu.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.vehdjk.com/Article/details/geakeoaha.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.sjlbkw.cn/Article/details/gnflknewn.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.vehdjk.com/Article/details/gluzzngrx.sHtML

[B03] switch / match / case
来源：http://mobile.bbcook.cn/Article/details/grsenuppu.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.bbcook.cn/Article/details/gywfcdffw.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.sjlbkw.cn/Article/details/gryanepzs.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.epnwcf.com/Article/details/gfgmevfge.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.bbcook.cn/Article/details/gntlantdc.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.bbcook.cn/Article/details/gddhwkpos.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.tarul.cn/Article/details/gjiibzcbc.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.vehdjk.com/Article/details/ggqpxjxkd.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.epnwcf.com/Article/details/ghnfsstgx.sHtML

[B04] for 计数循环
来源：http://m.share.vehdjk.com/Article/details/gzfaktggu.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.yfazqb.com/Article/details/gnhkspkvy.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.yfazqb.com/Article/details/geqvkwusi.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.bbcook.cn/Article/details/giyfvprta.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fktsv.cn/Article/details/gdguainod.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.fktsv.cn/Article/details/gdluzpcjp.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.bbcook.cn/Article/details/gzgqbrgtb.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.fktsv.cn/Article/details/gmkrnbfny.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.fktsv.cn/Article/details/gafbjdqrz.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.yfazqb.com/Article/details/gvvynzaov.sHtML

Py:   for item in arr: print(item)
来源：http://baike.sjlbkw.cn/Article/details/gvelreiax.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.yfazqb.com/Article/details/gcntkmrct.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.bbcook.cn/Article/details/ggegeazbs.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.yfazqb.com/Article/details/geaehajcs.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.vehdjk.com/Article/details/gqvbupjth.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.vehdjk.com/Article/details/gtbrgbuaw.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.bbcook.cn/Article/details/gkzrazcny.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.sjlbkw.cn/Article/details/gjozvrssa.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.tarul.cn/Article/details/glbsiwkdz.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.tarul.cn/Article/details/gclscbszk.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.fktsv.cn/Article/details/gbptbgwnb.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.vehdjk.com/Article/details/geaaapett.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.sjlbkw.cn/Article/details/gekkjdoei.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.fktsv.cn/Article/details/grdnfnofp.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.tarul.cn/Article/details/ggzjxyllh.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.epnwcf.com/Article/details/gqqhpwpxd.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.vehdjk.com/Article/details/gkyxowctc.sHtML

[B07] while 循环
来源：http://m.share.yfazqb.com/Article/details/gcyshosoz.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.yfazqb.com/Article/details/giaawaemk.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.fktsv.cn/Article/details/ghdhoqiet.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.sjlbkw.cn/Article/details/gnqcphiij.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.epnwcf.com/Article/details/gmvuxetgn.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.epnwcf.com/Article/details/gswlgyqtk.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.tarul.cn/Article/details/gpumzkolk.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.sjlbkw.cn/Article/details/gxmzkfzrl.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.bbcook.cn/Article/details/gyaxcniym.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.fktsv.cn/Article/details/gqnnkghmx.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.epnwcf.com/Article/details/gyybqmhxf.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.vehdjk.com/Article/details/gpjbvvimu.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.epnwcf.com/Article/details/gynzuvfae.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.bbcook.cn/Article/details/ggijufbwp.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.bbcook.cn/Article/details/gbdcshcoh.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.sjlbkw.cn/Article/details/gtwmfmpxg.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.tarul.cn/Article/details/grzvpfths.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.vehdjk.com/Article/details/gnjuoofdb.sHtML

[B09] break 与 continue
来源：http://www.blog.sjlbkw.cn/Article/details/gxmosmsfb.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.fktsv.cn/Article/details/gxtldhboq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.vehdjk.com/Article/details/gdwsgnips.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.epnwcf.com/Article/details/gvgczborf.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.tarul.cn/Article/details/gxjguvhsg.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/goysfvotq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.yfazqb.com/Article/details/ggilmtluh.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.tarul.cn/Article/details/gxacdynqa.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/galogdfcu.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.epnwcf.com/Article/details/glaogeqmj.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.bbcook.cn/Article/details/gbwbyjgoa.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.epnwcf.com/Article/details/gbivzbnfa.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.bbcook.cn/Article/details/gcmzcbulo.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.epnwcf.com/Article/details/gairffprk.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.yfazqb.com/Article/details/gsuilzdtg.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.epnwcf.com/Article/details/gmtoflvfa.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.yfazqb.com/Article/details/gaixmjxsg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.sjlbkw.cn/Article/details/gjshurofu.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.sjlbkw.cn/Article/details/gmlnddlwp.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.tarul.cn/Article/details/gwztkpwip.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.sjlbkw.cn/Article/details/gfhpedzom.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.vehdjk.com/Article/details/gvncqcbrv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gaaykflxz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.bbcook.cn/Article/details/gdbhmnmsc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.bbcook.cn/Article/details/ghnzqkuzc.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.tarul.cn/Article/details/gnfcltzzt.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.epnwcf.com/Article/details/gdzqsabrg.sHtML

[B12] 跳出多层循环
来源：http://blog.sjlbkw.cn/Article/details/gkrrlrmby.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.bbcook.cn/Article/details/gsfawhdjz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.tarul.cn/Article/details/gvvejjuiz.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fktsv.cn/Article/details/ggzcvlagf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.epnwcf.com/Article/details/gqhifaexu.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.vehdjk.com/Article/details/gjhkfxvti.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.fktsv.cn/Article/details/gpebdhsah.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.sjlbkw.cn/Article/details/gacqfihje.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.yfazqb.com/Article/details/gajutptqq.sHtML

[B13] 判断是否为数字
来源：http://3g.vehdjk.com/Article/details/gexzlwzit.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.fktsv.cn/Article/details/gqskbnswk.sHtML

PHP:  is_numeric($x)
来源：http://read.share.yfazqb.com/Article/details/gkfclvrdc.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.epnwcf.com/Article/details/ghsuezfpc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.sjlbkw.cn/Article/details/grqnnhzzw.sHtML

Java: x instanceof Number
来源：http://3g.bbcook.cn/Article/details/gkkbqkatq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.tarul.cn/Article/details/gfypecjij.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.fktsv.cn/Article/details/ghchsonlk.sHtML

C#:   x is int or double or decimal
来源：http://3g.vehdjk.com/Article/details/gavumjguj.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.bbcook.cn/Article/details/gqbglyukd.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.tarul.cn/Article/details/gulwvzjnu.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.bbcook.cn/Article/details/gwrkidivr.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.vehdjk.com/Article/details/gxmuplgto.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.epnwcf.com/Article/details/gvnzlxdel.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gtazpmmxq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.yfazqb.com/Article/details/grfoepgkg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.sjlbkw.cn/Article/details/grxjiluum.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.bbcook.cn/Article/details/gkgnozbvc.sHtML

[B15] 布尔运算与取反
来源：http://3g.fktsv.cn/Article/details/gmgcmrtcf.sHtML

Py:   a and b or not c
来源：http://baike.fktsv.cn/Article/details/gtdzanlhc.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.vehdjk.com/Article/details/gskttrscu.sHtML

JS:   a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/ggosagopp.sHtML

TS:   a && b || !c
来源：http://read.share.fktsv.cn/Article/details/gcaroajaz.sHtML

Java: a && b || !c
来源：http://www.share.vehdjk.com/Article/details/ghmwhwdxr.sHtML

Go:   a && b || !c
来源：http://wap.fktsv.cn/Article/details/gimzbsygr.sHtML

Ruby: a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/gndwqngpi.sHtML

C#:   a && b || !c
来源：http://blog.bbcook.cn/Article/details/glmdgvuxx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fktsv.cn/Article/details/gmolvjoll.sHtML

Py:   if not data: return
来源：http://mobile.tarul.cn/Article/details/gyvugkgmh.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.tarul.cn/Article/details/gjonkhnis.sHtML

JS:   if (!data) return;
来源：http://mobile.bbcook.cn/Article/details/gfsecmsyn.sHtML

TS:   if (!data) return;
来源：http://blog.vehdjk.com/Article/details/gkekvttrb.sHtML

Java: if (data == null) return;
来源：http://m.share.vehdjk.com/Article/details/gaucthlir.sHtML

Go:   if data == nil { return }
来源：http://m.share.epnwcf.com/Article/details/gjksyfekq.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.tarul.cn/Article/details/gvjbfadcn.sHtML

C#:   if (data == null) return;
来源：http://mobile.fktsv.cn/Article/details/ggwiwlweg.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gybqcymem.sHtML

C. 函数与作用域
来源：http://blog.tarul.cn/Article/details/gdxgqitck.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gbvradpwu.sHtML

[C01] 定义函数
来源：http://mobile.bbcook.cn/Article/details/ggshgaouy.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.yfazqb.com/Article/details/gznyxuvyc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.vehdjk.com/Article/details/gyjzgowdz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gxlqzsodx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gfbyfhsvv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gkxzuhafb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.bbcook.cn/Article/details/godvgqsvh.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.yfazqb.com/Article/details/grgbhojhx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.vehdjk.com/Article/details/ggtspfnuq.sHtML

[C02] 默认参数
来源：http://www.share.vehdjk.com/Article/details/gqhxdflta.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.tarul.cn/Article/details/gupknjofj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fktsv.cn/Article/details/gsjekzhra.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fktsv.cn/Article/details/gpymzvhmg.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gkoypufaj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.epnwcf.com/Article/details/ggtatbdwc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.bbcook.cn/Article/details/gtggvmchy.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.sjlbkw.cn/Article/details/gmidgkbpj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.epnwcf.com/Article/details/gootfutbp.sHtML

[C03] 可变参数
来源：http://m.share.tarul.cn/Article/details/gpyyemmul.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.vehdjk.com/Article/details/gfacuburz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.vehdjk.com/Article/details/ghmldlufy.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fktsv.cn/Article/details/gryjxjhvy.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.epnwcf.com/Article/details/glvstveyd.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.sjlbkw.cn/Article/details/grhxpgxkv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.epnwcf.com/Article/details/glhwfpynj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.yfazqb.com/Article/details/glfvpmhom.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.bbcook.cn/Article/details/ggalozkkl.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.tarul.cn/Article/details/gyejksslo.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.bbcook.cn/Article/details/gapmxolvd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.yfazqb.com/Article/details/gncgnqnxg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.epnwcf.com/Article/details/gizulozhk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.tarul.cn/Article/details/gsirgbgdi.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.sjlbkw.cn/Article/details/gulvqgsrf.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.yfazqb.com/Article/details/gxoeptauh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.epnwcf.com/Article/details/grbgtyzlq.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fktsv.cn/Article/details/gyfgztpfe.sHtML

[C05] 返回多个值
来源：http://3g.fktsv.cn/Article/details/glkwblvcn.sHtML

Py:   return a, b
来源：http://blog.tarul.cn/Article/details/gaqddfdzv.sHtML

PHP:  return [$a, $b];
来源：http://blog.yfazqb.com/Article/details/gdasvaugq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.vehdjk.com/Article/details/gqciyjosb.sHtML

TS:   return { a, b };
来源：http://blog.epnwcf.com/Article/details/goaimdxbv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.vehdjk.com/Article/details/gxylydvha.sHtML

Go:   return a, b
来源：http://blog.fktsv.cn/Article/details/gbwcyllit.sHtML

Ruby: return a, b
来源：http://baike.fktsv.cn/Article/details/gvyjzccmc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.sjlbkw.cn/Article/details/gwivkjrfp.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.epnwcf.com/Article/details/gxmvwshbk.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.yfazqb.com/Article/details/gfuxzidut.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.epnwcf.com/Article/details/gnaprdcvy.sHtML

JS:   const square = x => x * x;
来源：http://m.share.epnwcf.com/Article/details/gelqkmbyy.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.bbcook.cn/Article/details/gtlczyshk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fktsv.cn/Article/details/geeftbcpd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.yfazqb.com/Article/details/gryblztzv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.sjlbkw.cn/Article/details/geibxtwvj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.epnwcf.com/Article/details/ghrllfpub.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.yfazqb.com/Article/details/gmjipubza.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.sjlbkw.cn/Article/details/gnaqsbxnf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.vehdjk.com/Article/details/gfnqlinpn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.epnwcf.com/Article/details/gnvjjijgb.sHtML

TS:   arr.map(String)
来源：http://baike.bbcook.cn/Article/details/gclkhkkgq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.vehdjk.com/Article/details/grbqkgbkg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.vehdjk.com/Article/details/gfrhuzjem.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.sjlbkw.cn/Article/details/glvxulgfi.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.vehdjk.com/Article/details/gjceqgbtc.sHtML

[C08] 闭包
来源：http://3g.vehdjk.com/Article/details/gszavnwux.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.sjlbkw.cn/Article/details/glgjgytmf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fktsv.cn/Article/details/gewjfsucf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.tarul.cn/Article/details/gkfzsfshp.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.yfazqb.com/Article/details/gdsmvlyvx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fktsv.cn/Article/details/gggnkftgy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.tarul.cn/Article/details/gsswaqpjm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.vehdjk.com/Article/details/gtjkerdcp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.vehdjk.com/Article/details/gfienurny.sHtML

[C09] 递归
来源：http://m.share.vehdjk.com/Article/details/gyczlwpkg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.tarul.cn/Article/details/gbxuwhvnc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.epnwcf.com/Article/details/gdefqiuvt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fktsv.cn/Article/details/gvplhtwcs.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fktsv.cn/Article/details/gkiqgkpir.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.vehdjk.com/Article/details/gxnwcrlbr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.tarul.cn/Article/details/gfcjmijjq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.vehdjk.com/Article/details/gwlrrbekf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fktsv.cn/Article/details/gecmtebea.sHtML

[C10] 变量作用域
来源：http://www.share.yfazqb.com/Article/details/gsfxibcxk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.tarul.cn/Article/details/gfmiybvez.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.vehdjk.com/Article/details/gqtmpvpei.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fktsv.cn/Article/details/ggfhsafxv.sHtML

TS:   同 JS
来源：http://baike.epnwcf.com/Article/details/gdehtluhs.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.bbcook.cn/Article/details/gqmntcejj.sHtML

Go:   花括号块级作用域
来源：http://3g.tarul.cn/Article/details/gfpmreklj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.sjlbkw.cn/Article/details/gdcsabvao.sHtML

C#:   块级作用域
来源：http://www.share.fktsv.cn/Article/details/ggzmzyurt.sHtML

[C11] 模块导入与导出
来源：http://www.share.bbcook.cn/Article/details/gdcamtzbm.sHtML

Py:   from module import func
来源：http://m.share.bbcook.cn/Article/details/gpqzvzkwb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.epnwcf.com/Article/details/gzipstbey.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fktsv.cn/Article/details/guxzddpqw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fktsv.cn/Article/details/gpkzulwit.sHtML

Java: import java.util.List;
来源：http://mobile.yfazqb.com/Article/details/ggkozfgfd.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.bbcook.cn/Article/details/gwckxhhrv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.epnwcf.com/Article/details/gffnvnmgb.sHtML

C#:   using System.Text;
来源：http://m.share.bbcook.cn/Article/details/gjikffdef.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.bbcook.cn/Article/details/ghcpkwhwv.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.vehdjk.com/Article/details/gelxdoitc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.yfazqb.com/Article/details/gdzcznzne.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.bbcook.cn/Article/details/ggploztlg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.bbcook.cn/Article/details/gynsprgzd.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.epnwcf.com/Article/details/gqtbdjugf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.tarul.cn/Article/details/glfdbtirt.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.yfazqb.com/Article/details/guofngqyg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.tarul.cn/Article/details/gdxdxbkwb.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.sjlbkw.cn/Article/details/gpojridpx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.epnwcf.com/Article/details/gbgabdpdx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.sjlbkw.cn/Article/details/gghrwspja.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.vehdjk.com/Article/details/gngjmxupr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.yfazqb.com/Article/details/gagkrwyap.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gtlpjtocj.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.epnwcf.com/Article/details/gdbdokdls.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.epnwcf.com/Article/details/gfrkipqxk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.sjlbkw.cn/Article/details/gcuxhluqv.sHtML

[C14] 泛型函数
来源：http://3g.vehdjk.com/Article/details/gjxzxecob.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.vehdjk.com/Article/details/gimwcltvf.sHtML

PHP:  // 无泛型
来源：http://blog.yfazqb.com/Article/details/gdwjhbuzd.sHtML

JS:   // 无泛型
来源：http://www.m.share.epnwcf.com/Article/details/ghwudivke.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.sjlbkw.cn/Article/details/gixrdqkta.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.tarul.cn/Article/details/gweqhyfag.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.yfazqb.com/Article/details/gklnzwfeb.sHtML

Ruby: # 无泛型
来源：http://m.share.sjlbkw.cn/Article/details/gmacyzggq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fktsv.cn/Article/details/gtsghkyjp.sHtML

[C15] 解构 / 展开参数
来源：http://wap.bbcook.cn/Article/details/gjqolbeum.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.sjlbkw.cn/Article/details/ggrxukeje.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.fktsv.cn/Article/details/grovtbvaz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.sjlbkw.cn/Article/details/gghrrxedb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.sjlbkw.cn/Article/details/gagybdwqj.sHtML

Java: // 无解构
来源：http://www.blog.vehdjk.com/Article/details/gdstgjmxi.sHtML

Go:   // 无解构
来源：http://www.share.tarul.cn/Article/details/gzhlkmdnw.sHtML


<!-- 参考信息 -->