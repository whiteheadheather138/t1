代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.fktsv.cn/Article/details/gnbvkhmft.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.epnwcf.com/Article/details/gtemvbeuw.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.vehdjk.com/Article/details/gniuwdvly.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.epnwcf.com/Article/details/gjtaxdnqq.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.yfazqb.com/Article/details/gatmeqofn.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.yfazqb.com/Article/details/gbykxdlto.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.vehdjk.com/Article/details/gdzgbfzcr.sHtML

[A25] 字符串比较
来源：http://m.share.yfazqb.com/Article/details/gitleyjcl.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.vehdjk.com/Article/details/guwrgyjpm.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.sjlbkw.cn/Article/details/gretawrmi.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.tarul.cn/Article/details/gehkjvknp.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.epnwcf.com/Article/details/gjexgozql.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.fktsv.cn/Article/details/gezausmon.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.epnwcf.com/Article/details/gifgomzra.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.fktsv.cn/Article/details/guawezyfx.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.epnwcf.com/Article/details/gydvzbmmk.sHtML

[A26] 类型转换总览
来源：http://read.share.tarul.cn/Article/details/gvwcdncgc.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.vehdjk.com/Article/details/gcxdzjuou.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.yfazqb.com/Article/details/gxpealitj.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.vehdjk.com/Article/details/gywjqrrsj.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.sjlbkw.cn/Article/details/gwtgrewlm.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.bbcook.cn/Article/details/gsxefxvni.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.tarul.cn/Article/details/gwhttbrzu.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.bbcook.cn/Article/details/gmljadyck.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.epnwcf.com/Article/details/gvvvmvnot.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gybcdnien.sHtML

B. 流程控制
来源：http://mobile.epnwcf.com/Article/details/gxcszfmca.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gtqbibplw.sHtML

[B01] 条件判断 if / else
来源：http://baike.sjlbkw.cn/Article/details/gsoeraztm.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.fktsv.cn/Article/details/gkaozzkjk.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.epnwcf.com/Article/details/gtyxunwrd.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.tarul.cn/Article/details/glwyrwase.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.bbcook.cn/Article/details/gxkkazmsm.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.tarul.cn/Article/details/gbuiqlrkf.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.tarul.cn/Article/details/gesrslnxs.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.sjlbkw.cn/Article/details/gugsrvxhl.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.epnwcf.com/Article/details/glpnrwfng.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.bbcook.cn/Article/details/gcofrtjzy.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.tarul.cn/Article/details/ggoptfgsq.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.vehdjk.com/Article/details/gugvjeklo.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.bbcook.cn/Article/details/glohtcdgi.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fktsv.cn/Article/details/gheqjutae.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.bbcook.cn/Article/details/gasrwbxvk.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.bbcook.cn/Article/details/ggnieprag.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.bbcook.cn/Article/details/gjowkgzyd.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.sjlbkw.cn/Article/details/gxrobnzri.sHtML

[B03] switch / match / case
来源：http://wap.vehdjk.com/Article/details/gfxrdwiqy.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.epnwcf.com/Article/details/gnrqodgae.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.fktsv.cn/Article/details/gojcaehwv.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.epnwcf.com/Article/details/gbgrqjulc.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fktsv.cn/Article/details/gaafbmusm.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.epnwcf.com/Article/details/gdpwerbrc.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.sjlbkw.cn/Article/details/gvnpljqby.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.bbcook.cn/Article/details/gqkwjbrrp.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.tarul.cn/Article/details/gnwxjnfhi.sHtML

[B04] for 计数循环
来源：http://www.blog.epnwcf.com/Article/details/gbngtfnzh.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.fktsv.cn/Article/details/gcshwueoj.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.fktsv.cn/Article/details/guhudpzao.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.bbcook.cn/Article/details/gimulqigg.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.bbcook.cn/Article/details/gznihlgnv.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.bbcook.cn/Article/details/gmltnnkcx.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.epnwcf.com/Article/details/gyhyqjitg.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.vehdjk.com/Article/details/gihltfmph.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.epnwcf.com/Article/details/guzxaaxcv.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.tarul.cn/Article/details/gazyuqdtj.sHtML

Py:   for item in arr: print(item)
来源：http://wap.bbcook.cn/Article/details/gfrezbrnl.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.vehdjk.com/Article/details/gpimhzekn.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.sjlbkw.cn/Article/details/garlbqonf.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.epnwcf.com/Article/details/gphnupmvs.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.sjlbkw.cn/Article/details/gdxktbvxb.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.fktsv.cn/Article/details/gulmciqxm.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.epnwcf.com/Article/details/gsqnbplfy.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.epnwcf.com/Article/details/ggiswvenv.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.sjlbkw.cn/Article/details/gmmxwvagk.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.sjlbkw.cn/Article/details/gqcyakbfg.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.bbcook.cn/Article/details/grohwnkvc.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.sjlbkw.cn/Article/details/gbtgnlnye.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fktsv.cn/Article/details/gwpodvgfh.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.tarul.cn/Article/details/ggfpyqxbf.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.bbcook.cn/Article/details/gppfsgjye.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.bbcook.cn/Article/details/gwakjkfrf.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.yfazqb.com/Article/details/gzfsmqhdw.sHtML

[B07] while 循环
来源：http://read.share.tarul.cn/Article/details/gsdthabvw.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.tarul.cn/Article/details/gjtwonbmw.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.bbcook.cn/Article/details/gkgbujvgl.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.fktsv.cn/Article/details/gtpybvhkm.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.bbcook.cn/Article/details/gniseqodo.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.yfazqb.com/Article/details/gczwnfyaz.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.epnwcf.com/Article/details/ggivbpwva.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.yfazqb.com/Article/details/grzfalcsm.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.tarul.cn/Article/details/ggutejdcl.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.sjlbkw.cn/Article/details/ggjmxrzmi.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.yfazqb.com/Article/details/ghuoswuib.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.epnwcf.com/Article/details/goxflbjiw.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.vehdjk.com/Article/details/gnrxfwtvt.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.bbcook.cn/Article/details/ghdyyhfwe.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.epnwcf.com/Article/details/gdfpoxhyc.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.vehdjk.com/Article/details/gwrfzstjz.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.tarul.cn/Article/details/gdbgwpfmv.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.vehdjk.com/Article/details/gvepaomgm.sHtML

[B09] break 与 continue
来源：http://baike.yfazqb.com/Article/details/gehfupdrx.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.vehdjk.com/Article/details/gwpgfwntu.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.fktsv.cn/Article/details/gfpwjqqku.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.tarul.cn/Article/details/gyebxqzld.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.tarul.cn/Article/details/gwflvwgfh.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/gdbtiouhf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fktsv.cn/Article/details/gvxwppkbr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.epnwcf.com/Article/details/ghwhmjqua.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.epnwcf.com/Article/details/gqebvcaop.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.bbcook.cn/Article/details/gainmdeqo.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.sjlbkw.cn/Article/details/gblrubhhg.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.sjlbkw.cn/Article/details/gwjiztjyy.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.fktsv.cn/Article/details/gtvrtotjm.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.yfazqb.com/Article/details/gyugcbege.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.bbcook.cn/Article/details/gtuftmiwo.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.bbcook.cn/Article/details/gsyfycjdl.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.yfazqb.com/Article/details/glaoxvnsk.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.bbcook.cn/Article/details/gfgyglwix.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.fktsv.cn/Article/details/gbvdovxcu.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.epnwcf.com/Article/details/gvmecigna.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdfadjdhc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.vehdjk.com/Article/details/gppawdjsd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.bbcook.cn/Article/details/gtcbaxlst.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.vehdjk.com/Article/details/gkptntvac.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.epnwcf.com/Article/details/grxpzsxrs.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.epnwcf.com/Article/details/gzgrbvinp.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.yfazqb.com/Article/details/gelhkacia.sHtML

[B12] 跳出多层循环
来源：http://wap.vehdjk.com/Article/details/gthuqiyle.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.tarul.cn/Article/details/guukjgbzi.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.bbcook.cn/Article/details/gclwvrrtb.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.tarul.cn/Article/details/gpspzlhum.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.tarul.cn/Article/details/gfhrbfccd.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.vehdjk.com/Article/details/gbofikdsk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fktsv.cn/Article/details/ghdmxrkyb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fktsv.cn/Article/details/gczdirczc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.yfazqb.com/Article/details/gtqznhixs.sHtML

[B13] 判断是否为数字
来源：http://wap.yfazqb.com/Article/details/gyydgwdsx.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.vehdjk.com/Article/details/glhmelywo.sHtML

PHP:  is_numeric($x)
来源：http://www.share.tarul.cn/Article/details/ggwvrumcu.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fktsv.cn/Article/details/gsavotkeo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.tarul.cn/Article/details/ggetqeqdf.sHtML

Java: x instanceof Number
来源：http://read.share.sjlbkw.cn/Article/details/giwrmothe.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.bbcook.cn/Article/details/gcqzlazcz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.epnwcf.com/Article/details/gtgkbibix.sHtML

C#:   x is int or double or decimal
来源：http://3g.sjlbkw.cn/Article/details/gcdpsazga.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.bbcook.cn/Article/details/gbwpzqreh.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.bbcook.cn/Article/details/gjxbjdpkw.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.fktsv.cn/Article/details/gcnuigohq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.sjlbkw.cn/Article/details/gerpywupv.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.yfazqb.com/Article/details/gggfdfcwp.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.sjlbkw.cn/Article/details/gucfhcsae.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gifqofbew.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.bbcook.cn/Article/details/gzfrbmbka.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.epnwcf.com/Article/details/gtkojjpwd.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.sjlbkw.cn/Article/details/gtjuvohld.sHtML

Py:   a and b or not c
来源：http://m.share.epnwcf.com/Article/details/gdjhgsnhm.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.bbcook.cn/Article/details/geztfcioq.sHtML

JS:   a && b || !c
来源：http://wap.tarul.cn/Article/details/gyriklvuf.sHtML

TS:   a && b || !c
来源：http://baike.tarul.cn/Article/details/gfubynnsp.sHtML

Java: a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/gqmamogkl.sHtML

Go:   a && b || !c
来源：http://wap.bbcook.cn/Article/details/gvpyusvty.sHtML

Ruby: a && b || !c
来源：http://mobile.yfazqb.com/Article/details/gfgbgxrkd.sHtML

C#:   a && b || !c
来源：http://www.share.yfazqb.com/Article/details/girxblrxl.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.epnwcf.com/Article/details/guwnwqgzq.sHtML

Py:   if not data: return
来源：http://baike.sjlbkw.cn/Article/details/gjsdmlgfm.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.sjlbkw.cn/Article/details/gqajmlcwe.sHtML

JS:   if (!data) return;
来源：http://read.share.sjlbkw.cn/Article/details/ghlobuwyu.sHtML

TS:   if (!data) return;
来源：http://baike.epnwcf.com/Article/details/gbpwpferl.sHtML

Java: if (data == null) return;
来源：http://baike.fktsv.cn/Article/details/gdrpcnroc.sHtML

Go:   if data == nil { return }
来源：http://read.share.fktsv.cn/Article/details/gohddondy.sHtML

Ruby: return if data.nil?
来源：http://baike.sjlbkw.cn/Article/details/gogeqapgh.sHtML

C#:   if (data == null) return;
来源：http://baike.vehdjk.com/Article/details/gnsdauult.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gmnczwehm.sHtML

C. 函数与作用域
来源：http://read.share.vehdjk.com/Article/details/gwzmllphm.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gzexrvbon.sHtML

[C01] 定义函数
来源：http://www.m.share.bbcook.cn/Article/details/guczvhfyd.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.sjlbkw.cn/Article/details/gzfmcqabw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.epnwcf.com/Article/details/galfboofl.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/ggkfgxhln.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/gxqwwunrk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gcdnzhzly.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.fktsv.cn/Article/details/gyeinlytv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.tarul.cn/Article/details/gnzjdyqiw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gbkyxlsux.sHtML

[C02] 默认参数
来源：http://www.m.share.fktsv.cn/Article/details/glumiybmm.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.vehdjk.com/Article/details/goqezoqwr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.vehdjk.com/Article/details/gkrpzrdit.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.epnwcf.com/Article/details/gjgptazzn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/gopoplfmk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.tarul.cn/Article/details/gevgusxpr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.epnwcf.com/Article/details/geoejvudx.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.bbcook.cn/Article/details/gftcjliof.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.bbcook.cn/Article/details/ggariiago.sHtML

[C03] 可变参数
来源：http://baike.tarul.cn/Article/details/ggayvjovw.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.yfazqb.com/Article/details/gvsxboehv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.sjlbkw.cn/Article/details/gumexavyl.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.epnwcf.com/Article/details/gkpwhfxli.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.vehdjk.com/Article/details/gpfbalxni.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.sjlbkw.cn/Article/details/geebbfjmq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.bbcook.cn/Article/details/gbphxxfcd.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.tarul.cn/Article/details/gpxwqodtf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.bbcook.cn/Article/details/goimuppys.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.sjlbkw.cn/Article/details/glwnkzwfi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.yfazqb.com/Article/details/gwweffkbm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fktsv.cn/Article/details/gafjwxukq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.tarul.cn/Article/details/gfoinvysb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.yfazqb.com/Article/details/ghorlykif.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.tarul.cn/Article/details/gexlveycv.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.epnwcf.com/Article/details/gnusjddmp.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.yfazqb.com/Article/details/glxudywax.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.bbcook.cn/Article/details/gdqmksyrz.sHtML

[C05] 返回多个值
来源：http://read.share.fktsv.cn/Article/details/gvhjhfajr.sHtML

Py:   return a, b
来源：http://read.share.bbcook.cn/Article/details/gpedbsvfj.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fktsv.cn/Article/details/gbkcuaefk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.bbcook.cn/Article/details/gefydoptp.sHtML

TS:   return { a, b };
来源：http://www.blog.epnwcf.com/Article/details/gxfjramds.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.yfazqb.com/Article/details/ghiunozpw.sHtML

Go:   return a, b
来源：http://www.blog.vehdjk.com/Article/details/gksqocxyx.sHtML

Ruby: return a, b
来源：http://www.blog.sjlbkw.cn/Article/details/gteksavbp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.epnwcf.com/Article/details/gphziemlh.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.epnwcf.com/Article/details/gppdfrhgg.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.bbcook.cn/Article/details/gcqgpjzhq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.vehdjk.com/Article/details/gwunchany.sHtML

JS:   const square = x => x * x;
来源：http://3g.epnwcf.com/Article/details/gubgenuzc.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.vehdjk.com/Article/details/ghbrtloli.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.yfazqb.com/Article/details/gqthlxoza.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.epnwcf.com/Article/details/gifastosc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.tarul.cn/Article/details/gebyvcmqp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.bbcook.cn/Article/details/gcjbzsfqn.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.bbcook.cn/Article/details/gvgtizewc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.yfazqb.com/Article/details/gvuzsbrye.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.tarul.cn/Article/details/gdoryonei.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.tarul.cn/Article/details/gcvdjajoa.sHtML

TS:   arr.map(String)
来源：http://www.share.yfazqb.com/Article/details/gxeotzrnt.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.epnwcf.com/Article/details/gfawwwnnf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.sjlbkw.cn/Article/details/gtuwehmhh.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.fktsv.cn/Article/details/ggryyajxb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.bbcook.cn/Article/details/gmdzkmhuc.sHtML

[C08] 闭包
来源：http://read.share.bbcook.cn/Article/details/gbzzbxwdb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.vehdjk.com/Article/details/gzxjzelao.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.epnwcf.com/Article/details/gvnvujwyv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fktsv.cn/Article/details/ggdflqzrf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.bbcook.cn/Article/details/gsahquvgv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.fktsv.cn/Article/details/gzeifsjne.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fktsv.cn/Article/details/gcimctkkh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fktsv.cn/Article/details/gezeparlq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.vehdjk.com/Article/details/gtnlhaacl.sHtML

[C09] 递归
来源：http://read.share.vehdjk.com/Article/details/gcnbgjtfb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.yfazqb.com/Article/details/gbhjkutna.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.vehdjk.com/Article/details/gopwyoddl.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.yfazqb.com/Article/details/gvaogdpev.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.sjlbkw.cn/Article/details/gqgnkgiqi.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.tarul.cn/Article/details/gltpwixkv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.epnwcf.com/Article/details/gznhmhkgc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.sjlbkw.cn/Article/details/gjocuopmz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.bbcook.cn/Article/details/gzzbhmdkw.sHtML

[C10] 变量作用域
来源：http://read.share.tarul.cn/Article/details/grnjkehhw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.bbcook.cn/Article/details/gjcaxtxss.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.epnwcf.com/Article/details/gncwnhyfb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.tarul.cn/Article/details/gjxmfjulu.sHtML

TS:   同 JS
来源：http://read.share.vehdjk.com/Article/details/gadwerevp.sHtML

Java: 方法内为块级作用域
来源：http://blog.yfazqb.com/Article/details/gfbuywxdb.sHtML

Go:   花括号块级作用域
来源：http://wap.sjlbkw.cn/Article/details/gfgocahgl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.yfazqb.com/Article/details/gvcitnlyz.sHtML

C#:   块级作用域
来源：http://www.m.share.bbcook.cn/Article/details/gxbrxfhie.sHtML

[C11] 模块导入与导出
来源：http://m.share.epnwcf.com/Article/details/gmufnkrmd.sHtML

Py:   from module import func
来源：http://baike.fktsv.cn/Article/details/gaywurhgi.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.sjlbkw.cn/Article/details/grumpmjha.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.vehdjk.com/Article/details/gmjnwyobj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.vehdjk.com/Article/details/gqydjqggq.sHtML

Java: import java.util.List;
来源：http://read.share.fktsv.cn/Article/details/gloxouxju.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.sjlbkw.cn/Article/details/gdjsdowyz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.vehdjk.com/Article/details/gpghuhoey.sHtML

C#:   using System.Text;
来源：http://read.share.epnwcf.com/Article/details/gpinomdnn.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.epnwcf.com/Article/details/gxszivths.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.sjlbkw.cn/Article/details/gbonlziko.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fktsv.cn/Article/details/ghoxvczdm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.tarul.cn/Article/details/gittfrvlb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.sjlbkw.cn/Article/details/gauyvvayn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.yfazqb.com/Article/details/gyjkveaqh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fktsv.cn/Article/details/gbocpiken.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.sjlbkw.cn/Article/details/gsyzplcgk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fktsv.cn/Article/details/galurbvmv.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.bbcook.cn/Article/details/gcpwhrggp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.vehdjk.com/Article/details/gdblfewtl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.tarul.cn/Article/details/guwxmailq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.yfazqb.com/Article/details/ghhlstufb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/gpsmjalwa.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/gpnnpigkf.sHtML

Go:   func add(a, b int) int
来源：http://3g.tarul.cn/Article/details/gxaluncgf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.sjlbkw.cn/Article/details/gnpysfgiw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.vehdjk.com/Article/details/gamlmenzj.sHtML

[C14] 泛型函数
来源：http://3g.epnwcf.com/Article/details/gpcnxovea.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.vehdjk.com/Article/details/gobtvoirj.sHtML

PHP:  // 无泛型
来源：http://m.share.sjlbkw.cn/Article/details/gnwxgshkc.sHtML

JS:   // 无泛型
来源：http://mobile.bbcook.cn/Article/details/gztvgwboq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.sjlbkw.cn/Article/details/gqcyrpsog.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.epnwcf.com/Article/details/gagqipwkf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.epnwcf.com/Article/details/gcoizqmgv.sHtML

Ruby: # 无泛型
来源：http://m.share.tarul.cn/Article/details/gwqufaexs.sHtML


<!-- 参考信息 -->