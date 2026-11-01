代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.yfazqb.com/Article/details/gufhogqwg.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.sjlbkw.cn/Article/details/gnrgxknek.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.tarul.cn/Article/details/gcrdjllkd.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.vehdjk.com/Article/details/gysupxayg.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.yfazqb.com/Article/details/gpbrzxfpe.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.tarul.cn/Article/details/gdjpdsxyh.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.tarul.cn/Article/details/grbnrokgl.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.tarul.cn/Article/details/gmhdltmxz.sHtML

[A26] 类型转换总览
来源：http://read.share.bbcook.cn/Article/details/gvluqtdrz.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.vehdjk.com/Article/details/giwkfxaop.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.tarul.cn/Article/details/ghbcbouyq.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.fktsv.cn/Article/details/gsopyrsnq.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.fktsv.cn/Article/details/gqypxrpvj.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.epnwcf.com/Article/details/gahumpfab.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.sjlbkw.cn/Article/details/gvaqvecse.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.fktsv.cn/Article/details/gpshaqxhy.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.tarul.cn/Article/details/gelccqjun.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gpqwuxezj.sHtML

B. 流程控制
来源：http://3g.epnwcf.com/Article/details/gcavmloxe.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gjbqmbewk.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.sjlbkw.cn/Article/details/gzkjpvxot.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.fktsv.cn/Article/details/gakocmxvv.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.sjlbkw.cn/Article/details/gsojoclmb.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.yfazqb.com/Article/details/gpofgrluk.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.vehdjk.com/Article/details/giyzhkfib.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.yfazqb.com/Article/details/gkcnzthzo.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.tarul.cn/Article/details/gxcwfspcz.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.yfazqb.com/Article/details/gvhdooeca.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.bbcook.cn/Article/details/gcjglqnte.sHtML

[B02] 多分支 else if / elif
来源：http://3g.yfazqb.com/Article/details/grfxpsgdv.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.sjlbkw.cn/Article/details/gfayhphhz.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.epnwcf.com/Article/details/gxlyekaxe.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fktsv.cn/Article/details/gzceqljxe.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.sjlbkw.cn/Article/details/giazsvtia.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.epnwcf.com/Article/details/gxluvlnfm.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.tarul.cn/Article/details/gabhekrfx.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.vehdjk.com/Article/details/gsekxfflv.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.vehdjk.com/Article/details/gmbmagoce.sHtML

[B03] switch / match / case
来源：http://www.m.share.bbcook.cn/Article/details/gfxrwijth.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.epnwcf.com/Article/details/gjepcvdpj.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.yfazqb.com/Article/details/gzrfaoxsx.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqxjxkqvf.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.bbcook.cn/Article/details/gctfhwycj.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.fktsv.cn/Article/details/gdsblxumq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.vehdjk.com/Article/details/gfrqhihoq.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.fktsv.cn/Article/details/gqwkpiufp.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.sjlbkw.cn/Article/details/gbpgnefvk.sHtML

[B04] for 计数循环
来源：http://blog.epnwcf.com/Article/details/glmygbgti.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.sjlbkw.cn/Article/details/gimhcfdku.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.yfazqb.com/Article/details/ggjomxoxe.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.tarul.cn/Article/details/gpwrznfug.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fktsv.cn/Article/details/gzhfwhoxn.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.tarul.cn/Article/details/gfubtjdwm.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.epnwcf.com/Article/details/gohmokaja.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.vehdjk.com/Article/details/gtvdfnism.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.vehdjk.com/Article/details/glbsmvjiu.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.bbcook.cn/Article/details/gnbxhcige.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.yfazqb.com/Article/details/gvcjakvuu.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.vehdjk.com/Article/details/gfcvmhkko.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.tarul.cn/Article/details/ggdthfeah.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.vehdjk.com/Article/details/gemfeqppq.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.fktsv.cn/Article/details/gqvgmnhuo.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.vehdjk.com/Article/details/gaxvhhive.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.fktsv.cn/Article/details/gqpcgmfxb.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.bbcook.cn/Article/details/gxauoxoit.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.tarul.cn/Article/details/gnqlrytxg.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.tarul.cn/Article/details/gsdsjrgww.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.vehdjk.com/Article/details/gvwxmfizi.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.vehdjk.com/Article/details/gtjzxwjlu.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.epnwcf.com/Article/details/gncrdifuh.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.epnwcf.com/Article/details/gipafevon.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.epnwcf.com/Article/details/gqznxrxwg.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.epnwcf.com/Article/details/golchgehs.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.tarul.cn/Article/details/gpxxgwqzv.sHtML

[B07] while 循环
来源：http://wap.bbcook.cn/Article/details/gnmrljgig.sHtML

Py:   while i < 10: i += 1
来源：http://3g.bbcook.cn/Article/details/gabrbdxpt.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.yfazqb.com/Article/details/gyosfhfaa.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.epnwcf.com/Article/details/gyttqzbfc.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.epnwcf.com/Article/details/guxjhgybo.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.fktsv.cn/Article/details/gxnbiyybl.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.epnwcf.com/Article/details/gyxzmsmlf.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.sjlbkw.cn/Article/details/gcjtguybz.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.fktsv.cn/Article/details/gfmnexsxm.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.tarul.cn/Article/details/gmcndnavm.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.vehdjk.com/Article/details/gtyevffvf.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.sjlbkw.cn/Article/details/gdewymtnk.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.yfazqb.com/Article/details/gqalnarzm.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.vehdjk.com/Article/details/glxapvvkm.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.fktsv.cn/Article/details/gonegqpkk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.bbcook.cn/Article/details/gvrxbpyzq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.epnwcf.com/Article/details/gbtpgilar.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.yfazqb.com/Article/details/gqnxmmvkl.sHtML

[B09] break 与 continue
来源：http://www.blog.yfazqb.com/Article/details/gsgzgkbey.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.bbcook.cn/Article/details/guowjufik.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.fktsv.cn/Article/details/ghitknnfj.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.tarul.cn/Article/details/guicxtsck.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/ggouqncko.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.sjlbkw.cn/Article/details/gbmpwbfvo.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.tarul.cn/Article/details/gntsgpcex.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.sjlbkw.cn/Article/details/gmkdfirou.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.sjlbkw.cn/Article/details/gzwavgpux.sHtML

[B10] 遍历同时拿索引
来源：http://baike.yfazqb.com/Article/details/gpzqlwpoh.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.yfazqb.com/Article/details/gkclspwvn.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.bbcook.cn/Article/details/gkqsqihtz.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.yfazqb.com/Article/details/gsluthlvh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.vehdjk.com/Article/details/ggwarfbhr.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.vehdjk.com/Article/details/gzufvfako.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.yfazqb.com/Article/details/gploiktol.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.fktsv.cn/Article/details/gvvbiekeh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.sjlbkw.cn/Article/details/gzkxmzyzy.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.yfazqb.com/Article/details/gobgppkdj.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.bbcook.cn/Article/details/gmbhfbrjv.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.epnwcf.com/Article/details/gxawxmzzl.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.tarul.cn/Article/details/giatatagu.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.sjlbkw.cn/Article/details/gjyvehepw.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.sjlbkw.cn/Article/details/gjwottagj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.epnwcf.com/Article/details/gpzblwnoa.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.sjlbkw.cn/Article/details/gapdpoypl.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.bbcook.cn/Article/details/grfoxryei.sHtML

[B12] 跳出多层循环
来源：http://blog.epnwcf.com/Article/details/giabrvzpe.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.tarul.cn/Article/details/gtljsjdpc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.bbcook.cn/Article/details/guhpovcvx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fktsv.cn/Article/details/gvhhbrqgi.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.bbcook.cn/Article/details/gsxiiuvxh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.yfazqb.com/Article/details/gfzgbvtqs.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.bbcook.cn/Article/details/gnxmqhtsj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.epnwcf.com/Article/details/gjbxbkpqa.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.epnwcf.com/Article/details/gyhahcxcl.sHtML

[B13] 判断是否为数字
来源：http://www.blog.yfazqb.com/Article/details/gwellirbk.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.vehdjk.com/Article/details/gicyeposu.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.vehdjk.com/Article/details/gjzjnkzzf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.vehdjk.com/Article/details/gwcprizft.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fktsv.cn/Article/details/gqtnijlme.sHtML

Java: x instanceof Number
来源：http://mobile.fktsv.cn/Article/details/gxkzqpzdc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.tarul.cn/Article/details/guoetpdwz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.tarul.cn/Article/details/gmpbpgwiy.sHtML

C#:   x is int or double or decimal
来源：http://3g.epnwcf.com/Article/details/grorjegfr.sHtML

[B14] 判断值是否在集合内
来源：http://wap.sjlbkw.cn/Article/details/gbokkdvwo.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.sjlbkw.cn/Article/details/gfbtpguqi.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.epnwcf.com/Article/details/gcmpwxllk.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.yfazqb.com/Article/details/gtxiqplbx.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.bbcook.cn/Article/details/gnecfpmcg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.sjlbkw.cn/Article/details/gvvswmdky.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.vehdjk.com/Article/details/gilxpqnnk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.tarul.cn/Article/details/gvqwggbfy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.vehdjk.com/Article/details/gjictbifi.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.epnwcf.com/Article/details/gpljrwxba.sHtML

Py:   a and b or not c
来源：http://read.share.bbcook.cn/Article/details/grzjmljru.sHtML

PHP:  $a && $b || !$c
来源：http://3g.bbcook.cn/Article/details/glmfhffqf.sHtML

JS:   a && b || !c
来源：http://baike.fktsv.cn/Article/details/gkpppnykb.sHtML

TS:   a && b || !c
来源：http://baike.epnwcf.com/Article/details/gjazteseq.sHtML

Java: a && b || !c
来源：http://mobile.fktsv.cn/Article/details/geiyegpdh.sHtML

Go:   a && b || !c
来源：http://www.share.yfazqb.com/Article/details/gzxvxskdq.sHtML

Ruby: a && b || !c
来源：http://blog.vehdjk.com/Article/details/gpoimdtcj.sHtML

C#:   a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gutblqbpk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.sjlbkw.cn/Article/details/gbohhhtyc.sHtML

Py:   if not data: return
来源：http://blog.bbcook.cn/Article/details/gzpofecmq.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.bbcook.cn/Article/details/gkgeevzja.sHtML

JS:   if (!data) return;
来源：http://www.blog.fktsv.cn/Article/details/gnxilbuix.sHtML

TS:   if (!data) return;
来源：http://www.share.yfazqb.com/Article/details/gtafwuwof.sHtML

Java: if (data == null) return;
来源：http://m.share.fktsv.cn/Article/details/gwbtmydtq.sHtML

Go:   if data == nil { return }
来源：http://blog.tarul.cn/Article/details/ggirtbugj.sHtML

Ruby: return if data.nil?
来源：http://blog.tarul.cn/Article/details/gixyrngbf.sHtML

C#:   if (data == null) return;
来源：http://baike.epnwcf.com/Article/details/gwzyntpiy.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gjvvgvbfz.sHtML

C. 函数与作用域
来源：http://www.blog.vehdjk.com/Article/details/gdjssnvle.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gwkaxmanr.sHtML

[C01] 定义函数
来源：http://www.share.tarul.cn/Article/details/gbwkrscmh.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.sjlbkw.cn/Article/details/gsnkockie.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.vehdjk.com/Article/details/gcqxniuwj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.vehdjk.com/Article/details/gemtzmvbl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gmtnzexya.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gtnzyxeeg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.fktsv.cn/Article/details/grpcuzcdm.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.bbcook.cn/Article/details/gqsxhcoqz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fktsv.cn/Article/details/gffzyrofb.sHtML

[C02] 默认参数
来源：http://baike.tarul.cn/Article/details/gmbrgkmlq.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.sjlbkw.cn/Article/details/gajhwyusm.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.vehdjk.com/Article/details/gldtzllyq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fktsv.cn/Article/details/gczlipjin.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.epnwcf.com/Article/details/guirfqhae.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.tarul.cn/Article/details/gwdjhigzu.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.sjlbkw.cn/Article/details/gwdfytzwb.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.yfazqb.com/Article/details/gvornqmus.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.tarul.cn/Article/details/gegeayzln.sHtML

[C03] 可变参数
来源：http://m.share.fktsv.cn/Article/details/gagrijzsz.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.epnwcf.com/Article/details/gbmuwfkhi.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.epnwcf.com/Article/details/gjaiqdzzh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.epnwcf.com/Article/details/glfzcdtoo.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.tarul.cn/Article/details/gteaeltfe.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.bbcook.cn/Article/details/gkowzxzjb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.epnwcf.com/Article/details/grsfqncju.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.yfazqb.com/Article/details/ggvphaoqf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.bbcook.cn/Article/details/gupsuccdb.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.epnwcf.com/Article/details/gdtasjpow.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.epnwcf.com/Article/details/gxhrpftvq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.tarul.cn/Article/details/gpwoicnoh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.tarul.cn/Article/details/giliiuece.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.sjlbkw.cn/Article/details/gobtanwtf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.sjlbkw.cn/Article/details/gszxmpxyo.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.epnwcf.com/Article/details/goxjmjbfc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.epnwcf.com/Article/details/gzqadbfbz.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.tarul.cn/Article/details/gsqctwjbi.sHtML

[C05] 返回多个值
来源：http://read.share.epnwcf.com/Article/details/gqekuuihu.sHtML

Py:   return a, b
来源：http://www.blog.bbcook.cn/Article/details/gfsvlhnyw.sHtML

PHP:  return [$a, $b];
来源：http://baike.vehdjk.com/Article/details/gytfvstei.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.sjlbkw.cn/Article/details/gdnbzqjis.sHtML

TS:   return { a, b };
来源：http://www.m.share.tarul.cn/Article/details/gfufchkcy.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.tarul.cn/Article/details/gcljriick.sHtML

Go:   return a, b
来源：http://www.share.fktsv.cn/Article/details/gzfpakhky.sHtML

Ruby: return a, b
来源：http://www.blog.bbcook.cn/Article/details/ghpnmrane.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.epnwcf.com/Article/details/ghvqemmvq.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fktsv.cn/Article/details/gxplmybfu.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.tarul.cn/Article/details/gjfmmazxt.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.bbcook.cn/Article/details/gkelzccqu.sHtML

JS:   const square = x => x * x;
来源：http://m.share.yfazqb.com/Article/details/gjoyyujdh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.yfazqb.com/Article/details/gizxregxs.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fktsv.cn/Article/details/gctitzszy.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fktsv.cn/Article/details/grnfcpwct.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.tarul.cn/Article/details/gpgjpawbu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fktsv.cn/Article/details/gufvewiyr.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fktsv.cn/Article/details/ggmxposin.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.yfazqb.com/Article/details/gyhqgvkra.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fktsv.cn/Article/details/giammmrol.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.epnwcf.com/Article/details/gktdfrviw.sHtML

TS:   arr.map(String)
来源：http://www.share.tarul.cn/Article/details/gontchnau.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.yfazqb.com/Article/details/gcjunoecp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.yfazqb.com/Article/details/gkyfbkdhz.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.epnwcf.com/Article/details/gijlzgncx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.vehdjk.com/Article/details/ggrzqcyat.sHtML

[C08] 闭包
来源：http://baike.epnwcf.com/Article/details/glaqqglkr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.sjlbkw.cn/Article/details/grcdrhofe.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.bbcook.cn/Article/details/gvvovnnlj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.vehdjk.com/Article/details/gbemgxqxf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.vehdjk.com/Article/details/gwdstjxlf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.vehdjk.com/Article/details/gthruywhz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.vehdjk.com/Article/details/gbjqiuznq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.bbcook.cn/Article/details/gnxgiihll.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.yfazqb.com/Article/details/gpjgiucvw.sHtML

[C09] 递归
来源：http://blog.tarul.cn/Article/details/gxnihytms.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.epnwcf.com/Article/details/gyvjosbos.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.yfazqb.com/Article/details/gnshqywro.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.yfazqb.com/Article/details/gibeklxxv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.vehdjk.com/Article/details/gofshsxei.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.bbcook.cn/Article/details/gepjsswhk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.tarul.cn/Article/details/gdklnauxy.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.sjlbkw.cn/Article/details/gvjnoaszm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fktsv.cn/Article/details/gjgvdnjrt.sHtML

[C10] 变量作用域
来源：http://www.blog.epnwcf.com/Article/details/gmdbtonho.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.tarul.cn/Article/details/gzhfejiqt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.epnwcf.com/Article/details/gbtjhcpuk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.epnwcf.com/Article/details/gatettsqu.sHtML

TS:   同 JS
来源：http://wap.sjlbkw.cn/Article/details/gonlkuybl.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.tarul.cn/Article/details/gqtnfabke.sHtML

Go:   花括号块级作用域
来源：http://wap.tarul.cn/Article/details/guxvhenfn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.sjlbkw.cn/Article/details/gtfkfuzog.sHtML

C#:   块级作用域
来源：http://www.m.share.epnwcf.com/Article/details/gjbtixzlu.sHtML

[C11] 模块导入与导出
来源：http://m.share.bbcook.cn/Article/details/glygljvbs.sHtML

Py:   from module import func
来源：http://www.m.share.bbcook.cn/Article/details/gfeviceva.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.epnwcf.com/Article/details/gkcpbbqrp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.epnwcf.com/Article/details/gknawsgrn.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.tarul.cn/Article/details/guarfeeka.sHtML

Java: import java.util.List;
来源：http://mobile.vehdjk.com/Article/details/gwhwzjgog.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.yfazqb.com/Article/details/gbknfcisi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fktsv.cn/Article/details/giluelnwq.sHtML

C#:   using System.Text;
来源：http://blog.fktsv.cn/Article/details/gutawdiiu.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fktsv.cn/Article/details/gxikmpyoi.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.bbcook.cn/Article/details/guerwnwan.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.tarul.cn/Article/details/gryzayhaa.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.sjlbkw.cn/Article/details/ghewrnghn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.yfazqb.com/Article/details/gqhdlxasw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.yfazqb.com/Article/details/gggahdavq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.tarul.cn/Article/details/gxokycmwb.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.epnwcf.com/Article/details/gmukxmdll.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.tarul.cn/Article/details/gwtrlblhb.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.vehdjk.com/Article/details/gzzfpxght.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.sjlbkw.cn/Article/details/gcaeslrsz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.bbcook.cn/Article/details/gmunzbkfv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.vehdjk.com/Article/details/gzlerxtxx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.tarul.cn/Article/details/giuuznism.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/gxacvmcfn.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fktsv.cn/Article/details/gnyuuwlum.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.epnwcf.com/Article/details/grixvruxh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.yfazqb.com/Article/details/gzfqixefr.sHtML

[C14] 泛型函数
来源：http://www.blog.vehdjk.com/Article/details/gwgzmcybb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.sjlbkw.cn/Article/details/gjuvwggmw.sHtML

PHP:  // 无泛型
来源：http://blog.tarul.cn/Article/details/gicxlbtio.sHtML

JS:   // 无泛型
来源：http://m.share.fktsv.cn/Article/details/guwkzvgzn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.sjlbkw.cn/Article/details/gdfchucsb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.tarul.cn/Article/details/gtincmzzl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.tarul.cn/Article/details/gapmycvvs.sHtML

Ruby: # 无泛型
来源：http://mobile.tarul.cn/Article/details/gnxrwvfly.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.yfazqb.com/Article/details/gnpgvclpx.sHtML

[C15] 解构 / 展开参数
来源：http://wap.epnwcf.com/Article/details/gzmzabdms.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.bbcook.cn/Article/details/gbpvzpwmb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.sjlbkw.cn/Article/details/gtzheakcj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.tarul.cn/Article/details/gjodpyduk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fktsv.cn/Article/details/gyoxnqvpl.sHtML

Java: // 无解构
来源：http://wap.yfazqb.com/Article/details/gtygvgnjx.sHtML

Go:   // 无解构
来源：http://read.share.yfazqb.com/Article/details/gpuhzjfqo.sHtML


<!-- 参考信息 -->