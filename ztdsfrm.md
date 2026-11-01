代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.fktsv.cn/Article/details/ghlxtwxoa.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.yfazqb.com/Article/details/gxfnwmamk.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.fktsv.cn/Article/details/gyycnfgao.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.yfazqb.com/Article/details/gbcccbbqc.sHtML

[A26] 类型转换总览
来源：http://www.blog.fktsv.cn/Article/details/gxxfcjvjy.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.bbcook.cn/Article/details/gdajacvyb.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.fktsv.cn/Article/details/geghyycub.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.fktsv.cn/Article/details/ghvavlmid.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.tarul.cn/Article/details/gqxbvjuno.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.tarul.cn/Article/details/gowzlnycn.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.tarul.cn/Article/details/gcyqzlcew.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.tarul.cn/Article/details/gxytwwlmb.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.epnwcf.com/Article/details/gtrfrkmwy.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/grjfhwlvd.sHtML

B. 流程控制
来源：http://wap.vehdjk.com/Article/details/gohieradn.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/glzujocfb.sHtML

[B01] 条件判断 if / else
来源：http://read.share.yfazqb.com/Article/details/gtmbcpdyy.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.bbcook.cn/Article/details/gudkgeqyc.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.sjlbkw.cn/Article/details/gynawskjc.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.epnwcf.com/Article/details/giylwicbr.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.epnwcf.com/Article/details/glkxsucxb.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.fktsv.cn/Article/details/gletaxybc.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.epnwcf.com/Article/details/gdcemiooc.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.epnwcf.com/Article/details/gkymrkayw.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.fktsv.cn/Article/details/grwiafsca.sHtML

[B02] 多分支 else if / elif
来源：http://baike.tarul.cn/Article/details/gohaljokl.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.bbcook.cn/Article/details/gvukckktw.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.yfazqb.com/Article/details/gzvsixpxx.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.vehdjk.com/Article/details/gplxfntie.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fktsv.cn/Article/details/gfnrrqsnl.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fktsv.cn/Article/details/gfdbfhuku.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.sjlbkw.cn/Article/details/gfsfcfgmi.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.fktsv.cn/Article/details/giavwlhqr.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.vehdjk.com/Article/details/gofymlnqn.sHtML

[B03] switch / match / case
来源：http://3g.bbcook.cn/Article/details/gdeyobyyn.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.yfazqb.com/Article/details/giuncrkjz.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.sjlbkw.cn/Article/details/ghcnflywy.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fktsv.cn/Article/details/gbqxcibvf.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.sjlbkw.cn/Article/details/gdplxiuts.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.vehdjk.com/Article/details/gmldqfpma.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.bbcook.cn/Article/details/gqbdincnw.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.sjlbkw.cn/Article/details/gtwlolohc.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.yfazqb.com/Article/details/girpxbfqj.sHtML

[B04] for 计数循环
来源：http://m.share.fktsv.cn/Article/details/gczrfwuva.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.fktsv.cn/Article/details/gektzwcqb.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.epnwcf.com/Article/details/gseshnoji.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.tarul.cn/Article/details/gjfuyajsv.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fktsv.cn/Article/details/guroawjnh.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.vehdjk.com/Article/details/ghuhkgpro.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.fktsv.cn/Article/details/ghuwntxnx.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.tarul.cn/Article/details/gdfctrjie.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.vehdjk.com/Article/details/gejjdmhxv.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.epnwcf.com/Article/details/gapqyfrfr.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.sjlbkw.cn/Article/details/gesszphks.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.bbcook.cn/Article/details/gzoivihfh.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.vehdjk.com/Article/details/gyxhjbccp.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.sjlbkw.cn/Article/details/geirxnxxa.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.vehdjk.com/Article/details/gnamucscl.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.sjlbkw.cn/Article/details/gjancbdjb.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.yfazqb.com/Article/details/gpmgnihkq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.tarul.cn/Article/details/gbmeercrb.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.sjlbkw.cn/Article/details/gqlnbojhd.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.fktsv.cn/Article/details/gtchttpnz.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.fktsv.cn/Article/details/glzrgijsw.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.tarul.cn/Article/details/gwudxbsio.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.epnwcf.com/Article/details/gemvwcdbn.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.tarul.cn/Article/details/gqebdolsk.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.epnwcf.com/Article/details/gqifaduuo.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.fktsv.cn/Article/details/gsmnnegpt.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.tarul.cn/Article/details/glujkdtmt.sHtML

[B07] while 循环
来源：http://mobile.fktsv.cn/Article/details/gqcndyunu.sHtML

Py:   while i < 10: i += 1
来源：http://blog.vehdjk.com/Article/details/graloubej.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.epnwcf.com/Article/details/gcrksbary.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.vehdjk.com/Article/details/gkrmnfihe.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.bbcook.cn/Article/details/geqbmbkpa.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.yfazqb.com/Article/details/glalblopl.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.tarul.cn/Article/details/gwieezgqn.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.epnwcf.com/Article/details/glayhfghb.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.vehdjk.com/Article/details/ghujxlwzj.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.vehdjk.com/Article/details/gakppfiiq.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.tarul.cn/Article/details/gavlszeql.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.epnwcf.com/Article/details/gawdgnnaj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.yfazqb.com/Article/details/ghjqktfjb.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.vehdjk.com/Article/details/gvaheosrr.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.fktsv.cn/Article/details/gzilrtzxd.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.tarul.cn/Article/details/gmuywjsoc.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.sjlbkw.cn/Article/details/gmdyidqew.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.sjlbkw.cn/Article/details/gomwyngej.sHtML

[B09] break 与 continue
来源：http://mobile.vehdjk.com/Article/details/gtvnqaqgt.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.bbcook.cn/Article/details/gydrvuiuh.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggxfaapwm.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.tarul.cn/Article/details/gvzinplvw.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.epnwcf.com/Article/details/gfshxzgps.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.vehdjk.com/Article/details/gegyhhgur.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.tarul.cn/Article/details/gnrhvcduw.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.sjlbkw.cn/Article/details/gwbltqawj.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.tarul.cn/Article/details/gelfxspcx.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.epnwcf.com/Article/details/gzxrkiffx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.bbcook.cn/Article/details/grbxjsxhv.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.yfazqb.com/Article/details/gyiwaktqk.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.yfazqb.com/Article/details/gyrwgreff.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.yfazqb.com/Article/details/gjwjppkaq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.bbcook.cn/Article/details/gwtcsepue.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.sjlbkw.cn/Article/details/gzviynyxf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.fktsv.cn/Article/details/gbiitfhnd.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.bbcook.cn/Article/details/gkmugbodq.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.bbcook.cn/Article/details/gagdgycae.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.vehdjk.com/Article/details/gehzhyepo.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.tarul.cn/Article/details/gpjnaxuhc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fktsv.cn/Article/details/gtzrwnavd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.sjlbkw.cn/Article/details/gepisdpej.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.epnwcf.com/Article/details/gdjvfpwxy.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.yfazqb.com/Article/details/gyzqdzzeg.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.tarul.cn/Article/details/gnrudhboe.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.epnwcf.com/Article/details/gsvkaohhg.sHtML

[B12] 跳出多层循环
来源：http://3g.bbcook.cn/Article/details/gjvkiubtp.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.epnwcf.com/Article/details/glptwvsdb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.vehdjk.com/Article/details/gvomlldnp.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fktsv.cn/Article/details/gdplbevjw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.bbcook.cn/Article/details/gnxfanjva.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.tarul.cn/Article/details/gapryyjbm.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.vehdjk.com/Article/details/graeeoxif.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fktsv.cn/Article/details/guaenupkg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.vehdjk.com/Article/details/gauwuamva.sHtML

[B13] 判断是否为数字
来源：http://blog.vehdjk.com/Article/details/gqnowcrdr.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.tarul.cn/Article/details/gioliamvq.sHtML

PHP:  is_numeric($x)
来源：http://3g.fktsv.cn/Article/details/gypvsidql.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fktsv.cn/Article/details/gihhihtpb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.epnwcf.com/Article/details/gzrtsvyys.sHtML

Java: x instanceof Number
来源：http://www.blog.sjlbkw.cn/Article/details/goqxkewgl.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.tarul.cn/Article/details/gijatiomd.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.yfazqb.com/Article/details/gnqufwfaq.sHtML

C#:   x is int or double or decimal
来源：http://mobile.vehdjk.com/Article/details/gyhijynmw.sHtML

[B14] 判断值是否在集合内
来源：http://blog.vehdjk.com/Article/details/gzkyfnmge.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.yfazqb.com/Article/details/gdoyuuuxv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.epnwcf.com/Article/details/gccxnualh.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.epnwcf.com/Article/details/gictpeynl.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.tarul.cn/Article/details/gnulobtea.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.bbcook.cn/Article/details/gpdcpfysg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.sjlbkw.cn/Article/details/gclhhjwoe.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.epnwcf.com/Article/details/guwdscifv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.epnwcf.com/Article/details/gcpezetoq.sHtML

[B15] 布尔运算与取反
来源：http://read.share.sjlbkw.cn/Article/details/gzdffcleq.sHtML

Py:   a and b or not c
来源：http://www.share.sjlbkw.cn/Article/details/gqaaayczd.sHtML

PHP:  $a && $b || !$c
来源：http://blog.bbcook.cn/Article/details/gfjgkidqh.sHtML

JS:   a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gjfsofefm.sHtML

TS:   a && b || !c
来源：http://read.share.fktsv.cn/Article/details/grsvbpowl.sHtML

Java: a && b || !c
来源：http://mobile.fktsv.cn/Article/details/gabzafhsf.sHtML

Go:   a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/gpkgynwbr.sHtML

Ruby: a && b || !c
来源：http://m.share.fktsv.cn/Article/details/gdovbnrim.sHtML

C#:   a && b || !c
来源：http://3g.bbcook.cn/Article/details/gpumilkma.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.yfazqb.com/Article/details/gbimihhcd.sHtML

Py:   if not data: return
来源：http://read.share.vehdjk.com/Article/details/glxsdjqba.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.yfazqb.com/Article/details/gcpxztkpm.sHtML

JS:   if (!data) return;
来源：http://www.m.share.sjlbkw.cn/Article/details/gsemxssfb.sHtML

TS:   if (!data) return;
来源：http://baike.tarul.cn/Article/details/gxqkyafic.sHtML

Java: if (data == null) return;
来源：http://www.blog.vehdjk.com/Article/details/gqzcpruxt.sHtML

Go:   if data == nil { return }
来源：http://wap.epnwcf.com/Article/details/gjwfwxzls.sHtML

Ruby: return if data.nil?
来源：http://blog.vehdjk.com/Article/details/gymrkplso.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fktsv.cn/Article/details/ghemgtyqz.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gtujijyyg.sHtML

C. 函数与作用域
来源：http://m.share.tarul.cn/Article/details/grfmkciaw.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gdbhnzjgc.sHtML

[C01] 定义函数
来源：http://read.share.epnwcf.com/Article/details/gdmgkocbx.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.fktsv.cn/Article/details/gskwahyqh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.epnwcf.com/Article/details/gmweebrhs.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/gaaxcmluz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/ggopxdmem.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.tarul.cn/Article/details/gaevzaagy.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.fktsv.cn/Article/details/gvselidzw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.bbcook.cn/Article/details/gqqbppbmd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.yfazqb.com/Article/details/giwvbkktl.sHtML

[C02] 默认参数
来源：http://mobile.vehdjk.com/Article/details/glpdnikox.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.vehdjk.com/Article/details/gaclrihpn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.yfazqb.com/Article/details/grjlzspuk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.epnwcf.com/Article/details/gvopjiufw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.fktsv.cn/Article/details/ghseymqje.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.tarul.cn/Article/details/gkewvehbd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.fktsv.cn/Article/details/gypdcnitp.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.bbcook.cn/Article/details/gtduweygp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.sjlbkw.cn/Article/details/gkwokcdeh.sHtML

[C03] 可变参数
来源：http://blog.epnwcf.com/Article/details/gscdtoucz.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.tarul.cn/Article/details/gafwevnja.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.bbcook.cn/Article/details/gpqgzqhqh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.epnwcf.com/Article/details/grsybrhwr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.vehdjk.com/Article/details/gsssateqc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fktsv.cn/Article/details/gyovczyhr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.bbcook.cn/Article/details/gimcolzzw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.epnwcf.com/Article/details/gyvttvdqw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.bbcook.cn/Article/details/gnqryxtus.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.vehdjk.com/Article/details/gvnjjszkz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.vehdjk.com/Article/details/gqnzinxym.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.tarul.cn/Article/details/gftwdwhiu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.bbcook.cn/Article/details/gxavmlphv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fktsv.cn/Article/details/gadtqywhi.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fktsv.cn/Article/details/gpoychzzv.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.bbcook.cn/Article/details/grbssyksn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.bbcook.cn/Article/details/gcoyzjpah.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.sjlbkw.cn/Article/details/gsnqdiudc.sHtML

[C05] 返回多个值
来源：http://3g.epnwcf.com/Article/details/gpzsvhjxl.sHtML

Py:   return a, b
来源：http://blog.vehdjk.com/Article/details/gebrqbfum.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fktsv.cn/Article/details/gfgmzzbop.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.vehdjk.com/Article/details/gxcuzldzc.sHtML

TS:   return { a, b };
来源：http://wap.sjlbkw.cn/Article/details/gfhlpazdd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.yfazqb.com/Article/details/gfpxhfmrp.sHtML

Go:   return a, b
来源：http://www.share.vehdjk.com/Article/details/gxjbdkaaf.sHtML

Ruby: return a, b
来源：http://wap.yfazqb.com/Article/details/gjhuyczrf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.sjlbkw.cn/Article/details/ggyaxcyyz.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.sjlbkw.cn/Article/details/gyloxospf.sHtML

Py:   square = lambda x: x * x
来源：http://blog.yfazqb.com/Article/details/gwdnkdval.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.bbcook.cn/Article/details/gyfyxqghr.sHtML

JS:   const square = x => x * x;
来源：http://www.share.vehdjk.com/Article/details/gqimbjgyk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.yfazqb.com/Article/details/gycgxetbo.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fktsv.cn/Article/details/gblfmkhfk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.yfazqb.com/Article/details/gwdmgchsy.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.vehdjk.com/Article/details/glspotqsv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.sjlbkw.cn/Article/details/gehdoiwgd.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.epnwcf.com/Article/details/gkbngshsv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.vehdjk.com/Article/details/gwpbwkvqk.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.bbcook.cn/Article/details/gayzuzvaf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.sjlbkw.cn/Article/details/gudkfaotu.sHtML

TS:   arr.map(String)
来源：http://mobile.fktsv.cn/Article/details/gedpaopuc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.vehdjk.com/Article/details/gxssooszl.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.yfazqb.com/Article/details/gnjqmadoh.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.yfazqb.com/Article/details/ghjaoelzb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.yfazqb.com/Article/details/gjxmaygba.sHtML

[C08] 闭包
来源：http://www.blog.vehdjk.com/Article/details/ghyxbhhfm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.fktsv.cn/Article/details/gtrihmxwc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnlbqizhs.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.tarul.cn/Article/details/ghfgsjqde.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.sjlbkw.cn/Article/details/guyhacrhg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.sjlbkw.cn/Article/details/gmdhlhdgq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.yfazqb.com/Article/details/gcaogrbbk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.sjlbkw.cn/Article/details/gykjjodnj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.bbcook.cn/Article/details/gruykossw.sHtML

[C09] 递归
来源：http://3g.epnwcf.com/Article/details/gtyxnpixs.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.yfazqb.com/Article/details/gonghuzxg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.yfazqb.com/Article/details/gtylegdck.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.epnwcf.com/Article/details/gyrwkrcjf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.bbcook.cn/Article/details/givirovsn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fktsv.cn/Article/details/gxrnzjdwj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.bbcook.cn/Article/details/gwojjftkh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fktsv.cn/Article/details/grfrygfif.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.bbcook.cn/Article/details/gxphurzgz.sHtML

[C10] 变量作用域
来源：http://www.share.fktsv.cn/Article/details/gfxkwczbp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.epnwcf.com/Article/details/gaputvict.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.tarul.cn/Article/details/gqvkgjwnv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.bbcook.cn/Article/details/gwtqrmkrp.sHtML

TS:   同 JS
来源：http://blog.yfazqb.com/Article/details/gnicvnqth.sHtML

Java: 方法内为块级作用域
来源：http://mobile.tarul.cn/Article/details/gdbcrqnke.sHtML

Go:   花括号块级作用域
来源：http://3g.vehdjk.com/Article/details/gusiekjbo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.fktsv.cn/Article/details/gxhakamhu.sHtML

C#:   块级作用域
来源：http://www.m.share.bbcook.cn/Article/details/gtkcqgawt.sHtML

[C11] 模块导入与导出
来源：http://mobile.fktsv.cn/Article/details/gwnzporjd.sHtML

Py:   from module import func
来源：http://www.share.vehdjk.com/Article/details/ggioxjgsu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.vehdjk.com/Article/details/gdjzplaaa.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.bbcook.cn/Article/details/gtkdvmtti.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.tarul.cn/Article/details/gkqrqnivc.sHtML

Java: import java.util.List;
来源：http://read.share.sjlbkw.cn/Article/details/gyeliheym.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.sjlbkw.cn/Article/details/gbpaqoktx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.bbcook.cn/Article/details/gneviqyoa.sHtML

C#:   using System.Text;
来源：http://www.share.yfazqb.com/Article/details/gqgwilxlz.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.fktsv.cn/Article/details/ggxxkqxpu.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.epnwcf.com/Article/details/gawahxkfe.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fktsv.cn/Article/details/gfvvlgxfc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fktsv.cn/Article/details/guogdlepk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.sjlbkw.cn/Article/details/grsqjbdjo.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.yfazqb.com/Article/details/gznhohzrw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.epnwcf.com/Article/details/gcmeitvhu.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.epnwcf.com/Article/details/gwnlzqpoy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.sjlbkw.cn/Article/details/gzjkzslda.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.yfazqb.com/Article/details/gqsoksxst.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.epnwcf.com/Article/details/gqvtadgbj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.epnwcf.com/Article/details/gjplqdfls.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.epnwcf.com/Article/details/gssqvfmmf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gupsyqrxp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gxukgydkr.sHtML

Go:   func add(a, b int) int
来源：http://blog.fktsv.cn/Article/details/gjfqrhzoz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.tarul.cn/Article/details/gvinipzgo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.tarul.cn/Article/details/gsepfamda.sHtML

[C14] 泛型函数
来源：http://blog.sjlbkw.cn/Article/details/gpmatzryu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fktsv.cn/Article/details/gxnjkifar.sHtML

PHP:  // 无泛型
来源：http://www.share.fktsv.cn/Article/details/gkdhdagkn.sHtML

JS:   // 无泛型
来源：http://baike.yfazqb.com/Article/details/glousavrm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fktsv.cn/Article/details/gggivfhnq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fktsv.cn/Article/details/gndpoepvl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.bbcook.cn/Article/details/gydvcaovv.sHtML

Ruby: # 无泛型
来源：http://mobile.yfazqb.com/Article/details/gaibbagdk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.tarul.cn/Article/details/gbwpkvceq.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.bbcook.cn/Article/details/guqfeufid.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.epnwcf.com/Article/details/gttjqxtkq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fktsv.cn/Article/details/glnnpqwsb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fktsv.cn/Article/details/gikcmjcze.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.tarul.cn/Article/details/gikumfkmm.sHtML

Java: // 无解构
来源：http://3g.sjlbkw.cn/Article/details/gyodhmyhw.sHtML

Go:   // 无解构
来源：http://mobile.sjlbkw.cn/Article/details/gztftaqle.sHtML

Ruby: a, b = pair
来源：http://wap.epnwcf.com/Article/details/gryebpegr.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fktsv.cn/Article/details/giuddkadv.sHtML

[C16] 函数 / 方法重载
来源：http://baike.yfazqb.com/Article/details/gfavhxclr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.bbcook.cn/Article/details/gtgvchcpa.sHtML


<!-- 参考信息 -->