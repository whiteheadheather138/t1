代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://baike.tarul.cn/Article/details/gzegfpvbu.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.sjlbkw.cn/Article/details/gnnvaxplz.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.yfazqb.com/Article/details/gpksobfso.sHtML

[A25] 字符串比较
来源：http://mobile.bbcook.cn/Article/details/ggpccwiek.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.bbcook.cn/Article/details/govfwilyo.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.sjlbkw.cn/Article/details/glfsdajrh.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.sjlbkw.cn/Article/details/gfeefwtjj.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.yfazqb.com/Article/details/gympatqgo.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.sjlbkw.cn/Article/details/guxfbfarc.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.yfazqb.com/Article/details/gocggnrek.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.bbcook.cn/Article/details/gaezwomnv.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.epnwcf.com/Article/details/gsknndoxj.sHtML

[A26] 类型转换总览
来源：http://blog.epnwcf.com/Article/details/gmfannblc.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.bbcook.cn/Article/details/gvqenglrg.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.bbcook.cn/Article/details/gvzpcbdib.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.tarul.cn/Article/details/gqblsokqp.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.yfazqb.com/Article/details/gcyhhtise.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.fktsv.cn/Article/details/gmapyxene.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.fktsv.cn/Article/details/grgwnotfz.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.sjlbkw.cn/Article/details/gcrkmehba.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.sjlbkw.cn/Article/details/gfuuqogqk.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gbfdcukzi.sHtML

B. 流程控制
来源：http://www.m.share.epnwcf.com/Article/details/ghqxifsyd.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/ggypdkqvf.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.epnwcf.com/Article/details/gukvsasxt.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.yfazqb.com/Article/details/gbvhkrieb.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.tarul.cn/Article/details/guktkxxjd.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.epnwcf.com/Article/details/gjedfpkos.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.vehdjk.com/Article/details/gzykbxkmn.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.epnwcf.com/Article/details/gobevqsgn.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.yfazqb.com/Article/details/gjhjklova.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.tarul.cn/Article/details/griemqcsr.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.vehdjk.com/Article/details/gsnovlteg.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.yfazqb.com/Article/details/gqbkmrlxv.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.sjlbkw.cn/Article/details/glaerncno.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.fktsv.cn/Article/details/gbndsjxst.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.yfazqb.com/Article/details/grcdjiouj.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.tarul.cn/Article/details/gsvmjbbah.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.yfazqb.com/Article/details/gtwnuohhj.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.yfazqb.com/Article/details/gcmzfxurd.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.epnwcf.com/Article/details/gqqvhkpgy.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.sjlbkw.cn/Article/details/goxybaqym.sHtML

[B03] switch / match / case
来源：http://www.blog.yfazqb.com/Article/details/gpgtdjbbb.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.vehdjk.com/Article/details/gvcqsmhng.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.sjlbkw.cn/Article/details/gzolqfmpn.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.epnwcf.com/Article/details/giehgmwtv.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.epnwcf.com/Article/details/ggfqqbjqm.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.yfazqb.com/Article/details/gdzpnprtf.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.bbcook.cn/Article/details/gcbitdqld.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.epnwcf.com/Article/details/gumwzzndt.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.bbcook.cn/Article/details/gcgdcfkej.sHtML

[B04] for 计数循环
来源：http://read.share.vehdjk.com/Article/details/gumafgciy.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.bbcook.cn/Article/details/gzhafyewo.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.vehdjk.com/Article/details/gluceynje.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.yfazqb.com/Article/details/gvgpcuexr.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fktsv.cn/Article/details/gnouqrebf.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.epnwcf.com/Article/details/gdvdnhyut.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.sjlbkw.cn/Article/details/grtnebbuv.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.bbcook.cn/Article/details/gytrtuvno.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.vehdjk.com/Article/details/gtcgsuedm.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.tarul.cn/Article/details/grkgvlkke.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.sjlbkw.cn/Article/details/grtwnljmw.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.yfazqb.com/Article/details/gqhttbtji.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.sjlbkw.cn/Article/details/ghztzazvs.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.bbcook.cn/Article/details/gdqxgobyq.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.vehdjk.com/Article/details/gesgceowa.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.bbcook.cn/Article/details/gmnfzldzo.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.vehdjk.com/Article/details/gvwkquxpy.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.yfazqb.com/Article/details/gdylvkurk.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.vehdjk.com/Article/details/gornjbzsu.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.bbcook.cn/Article/details/gomaiwzjw.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.fktsv.cn/Article/details/gnbhneinz.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.vehdjk.com/Article/details/gcssnwcjt.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.bbcook.cn/Article/details/gqvpnjltb.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.sjlbkw.cn/Article/details/gqgvvmrlj.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.epnwcf.com/Article/details/gxeolqnxl.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.bbcook.cn/Article/details/gbyictuyo.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.epnwcf.com/Article/details/gxpfssfja.sHtML

[B07] while 循环
来源：http://www.share.sjlbkw.cn/Article/details/gaplcqepi.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.fktsv.cn/Article/details/gyizpknbg.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.vehdjk.com/Article/details/gdgwfmacd.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.yfazqb.com/Article/details/gtrjynqtp.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.bbcook.cn/Article/details/gocsyphtt.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.bbcook.cn/Article/details/giwbnyrky.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.sjlbkw.cn/Article/details/gepibehqj.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.vehdjk.com/Article/details/gjumkktoc.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.vehdjk.com/Article/details/gryhdlecc.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.vehdjk.com/Article/details/gsfaxrgqb.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.sjlbkw.cn/Article/details/gmxkmmrie.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.fktsv.cn/Article/details/gzhzmevrj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.tarul.cn/Article/details/gocxehhzr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.vehdjk.com/Article/details/gycxhthdc.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.tarul.cn/Article/details/gbekdfggl.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.fktsv.cn/Article/details/gliiscggd.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.sjlbkw.cn/Article/details/gqdpepdfr.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.yfazqb.com/Article/details/gbxiwiadp.sHtML

[B09] break 与 continue
来源：http://mobile.fktsv.cn/Article/details/gducoomjz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.tarul.cn/Article/details/gzcrmlcyu.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.sjlbkw.cn/Article/details/gyyystkdc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.vehdjk.com/Article/details/glmxgepgd.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.epnwcf.com/Article/details/gwslxinvj.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.vehdjk.com/Article/details/grvowdzlb.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.tarul.cn/Article/details/goxcamcaw.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.fktsv.cn/Article/details/gafxtmyah.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.bbcook.cn/Article/details/gglmpfkag.sHtML

[B10] 遍历同时拿索引
来源：http://3g.vehdjk.com/Article/details/gznxwubgx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.tarul.cn/Article/details/gbcgehorr.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.bbcook.cn/Article/details/gybcnbtkw.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.epnwcf.com/Article/details/gtdtytmpv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.tarul.cn/Article/details/gbnziwuir.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.tarul.cn/Article/details/ggzcidpuu.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.fktsv.cn/Article/details/gcwfymhww.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.sjlbkw.cn/Article/details/glxdtnovn.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.bbcook.cn/Article/details/gjzkocxau.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.epnwcf.com/Article/details/gzlvzdeqo.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.vehdjk.com/Article/details/gbcdqhukc.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.epnwcf.com/Article/details/gbocqscfp.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.vehdjk.com/Article/details/gnjhzfkhu.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.yfazqb.com/Article/details/gahmzqwrq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.vehdjk.com/Article/details/gaedrphmb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.sjlbkw.cn/Article/details/gezqbkhjv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.vehdjk.com/Article/details/grulhrqgo.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.sjlbkw.cn/Article/details/gxmsvnrfl.sHtML

[B12] 跳出多层循环
来源：http://3g.vehdjk.com/Article/details/gdogrbbsi.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.epnwcf.com/Article/details/ghjfiqwox.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.yfazqb.com/Article/details/gjgizefey.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.epnwcf.com/Article/details/gpmuqmllx.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.yfazqb.com/Article/details/gbjlffosc.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.tarul.cn/Article/details/gzsweztgw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.sjlbkw.cn/Article/details/gbfchhtat.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.fktsv.cn/Article/details/gwpihfnkp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.tarul.cn/Article/details/gnxuuqexs.sHtML

[B13] 判断是否为数字
来源：http://wap.fktsv.cn/Article/details/gmpfboqwk.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.bbcook.cn/Article/details/gbmxdxwvs.sHtML

PHP:  is_numeric($x)
来源：http://3g.fktsv.cn/Article/details/gliqraqci.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.bbcook.cn/Article/details/gydjvzsun.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.sjlbkw.cn/Article/details/ggarfdqnq.sHtML

Java: x instanceof Number
来源：http://www.m.share.tarul.cn/Article/details/gpyapbycb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.sjlbkw.cn/Article/details/gkqumshai.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fktsv.cn/Article/details/gdgntvcny.sHtML

C#:   x is int or double or decimal
来源：http://3g.vehdjk.com/Article/details/gplrsjuvw.sHtML

[B14] 判断值是否在集合内
来源：http://blog.fktsv.cn/Article/details/gschhkbho.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.yfazqb.com/Article/details/gwubkoxwk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.epnwcf.com/Article/details/gsitkrspi.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.vehdjk.com/Article/details/gtowinclu.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fktsv.cn/Article/details/ggodjehxc.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.yfazqb.com/Article/details/ggudqusaa.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.sjlbkw.cn/Article/details/gnbchkmzo.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.epnwcf.com/Article/details/grjgmnyyn.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.bbcook.cn/Article/details/gmasenwqr.sHtML

[B15] 布尔运算与取反
来源：http://blog.yfazqb.com/Article/details/grjpcnrjt.sHtML

Py:   a and b or not c
来源：http://read.share.vehdjk.com/Article/details/gbxyfdinr.sHtML

PHP:  $a && $b || !$c
来源：http://baike.tarul.cn/Article/details/gbpnqnzgo.sHtML

JS:   a && b || !c
来源：http://3g.epnwcf.com/Article/details/gncjoespb.sHtML

TS:   a && b || !c
来源：http://baike.epnwcf.com/Article/details/gjcawpqlz.sHtML

Java: a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gbsjoijkn.sHtML

Go:   a && b || !c
来源：http://m.share.fktsv.cn/Article/details/gofxxidpw.sHtML

Ruby: a && b || !c
来源：http://mobile.bbcook.cn/Article/details/giymaqckv.sHtML

C#:   a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gwccotgsd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.tarul.cn/Article/details/gdqohjfdm.sHtML

Py:   if not data: return
来源：http://www.blog.tarul.cn/Article/details/grcckmqmm.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.bbcook.cn/Article/details/golvelhkj.sHtML

JS:   if (!data) return;
来源：http://wap.yfazqb.com/Article/details/gvjtrndez.sHtML

TS:   if (!data) return;
来源：http://3g.vehdjk.com/Article/details/ggoqjjzkj.sHtML

Java: if (data == null) return;
来源：http://www.share.epnwcf.com/Article/details/grsrnxzel.sHtML

Go:   if data == nil { return }
来源：http://mobile.vehdjk.com/Article/details/gnitekdhg.sHtML

Ruby: return if data.nil?
来源：http://3g.sjlbkw.cn/Article/details/gfpxepxmx.sHtML

C#:   if (data == null) return;
来源：http://read.share.sjlbkw.cn/Article/details/grorpfuas.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gxeyzeksf.sHtML

C. 函数与作用域
来源：http://m.share.epnwcf.com/Article/details/giunudzpm.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gkfxffcdy.sHtML

[C01] 定义函数
来源：http://wap.fktsv.cn/Article/details/gqicforoz.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.yfazqb.com/Article/details/gwjjsswef.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.tarul.cn/Article/details/gasoxzgfc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gcimgavar.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/grotfpgqw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gevmtpsux.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.vehdjk.com/Article/details/gpqpnfosx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.yfazqb.com/Article/details/gghjepusr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gruxquipz.sHtML

[C02] 默认参数
来源：http://3g.fktsv.cn/Article/details/gropjakrg.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.fktsv.cn/Article/details/gilarskjz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.tarul.cn/Article/details/gfuxsurhx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.yfazqb.com/Article/details/gzztjzkvu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.epnwcf.com/Article/details/gezsdjnaw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.sjlbkw.cn/Article/details/gxidymsfz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.epnwcf.com/Article/details/gwsqhxldu.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.vehdjk.com/Article/details/glxsznlya.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.tarul.cn/Article/details/gsdkdkbxr.sHtML

[C03] 可变参数
来源：http://baike.sjlbkw.cn/Article/details/gherxrfjs.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.yfazqb.com/Article/details/gkaywfbmo.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.tarul.cn/Article/details/glligmvfs.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.tarul.cn/Article/details/gxhaoijfl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.vehdjk.com/Article/details/gjftgxwbh.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.bbcook.cn/Article/details/gjuuqtael.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.tarul.cn/Article/details/gycdpdjme.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.yfazqb.com/Article/details/grhcagtha.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.yfazqb.com/Article/details/geygctkcr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.yfazqb.com/Article/details/gltskuxwf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.bbcook.cn/Article/details/gsjkelhnw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.yfazqb.com/Article/details/glkknqccg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.sjlbkw.cn/Article/details/gswscevfz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.tarul.cn/Article/details/gakwyoxvi.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.vehdjk.com/Article/details/gqqyavinw.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.vehdjk.com/Article/details/gjdmmudzu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.vehdjk.com/Article/details/gvybwikpl.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fktsv.cn/Article/details/gkgzjdzpm.sHtML

[C05] 返回多个值
来源：http://m.share.bbcook.cn/Article/details/gyfrsylzu.sHtML

Py:   return a, b
来源：http://m.share.bbcook.cn/Article/details/guyhjgecs.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.vehdjk.com/Article/details/gejfdoztw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.tarul.cn/Article/details/gsprhgeac.sHtML

TS:   return { a, b };
来源：http://www.share.tarul.cn/Article/details/gqjeesxfb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.sjlbkw.cn/Article/details/glqbqtybk.sHtML

Go:   return a, b
来源：http://wap.vehdjk.com/Article/details/gvikiigvv.sHtML

Ruby: return a, b
来源：http://3g.bbcook.cn/Article/details/gxblerjfg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.vehdjk.com/Article/details/golboiabj.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.epnwcf.com/Article/details/giibfbgph.sHtML

Py:   square = lambda x: x * x
来源：http://3g.vehdjk.com/Article/details/gesrbizjo.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.tarul.cn/Article/details/gdyhneiaz.sHtML

JS:   const square = x => x * x;
来源：http://wap.epnwcf.com/Article/details/gclnjfsga.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.sjlbkw.cn/Article/details/gndlrvjsk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.tarul.cn/Article/details/gmpouzmkk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.tarul.cn/Article/details/gonhmwrcc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fktsv.cn/Article/details/gdbonjija.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fktsv.cn/Article/details/gjvfsitbe.sHtML

[C07] 把函数作为参数传入
来源：http://blog.vehdjk.com/Article/details/gomerzpkd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.vehdjk.com/Article/details/gklcbikmk.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.vehdjk.com/Article/details/gerhmwmts.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.sjlbkw.cn/Article/details/gwrfdwmvy.sHtML

TS:   arr.map(String)
来源：http://blog.fktsv.cn/Article/details/gwljnplra.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.epnwcf.com/Article/details/grskqnyns.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fktsv.cn/Article/details/gxecslffm.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.yfazqb.com/Article/details/ghjimheyb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.tarul.cn/Article/details/gxayyztze.sHtML

[C08] 闭包
来源：http://www.m.share.fktsv.cn/Article/details/grcpqyzps.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.sjlbkw.cn/Article/details/gtqlejhjl.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fktsv.cn/Article/details/gxyfswrjv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.yfazqb.com/Article/details/gsxhcijfo.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.tarul.cn/Article/details/glfnzbdqz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.sjlbkw.cn/Article/details/gavnegcjf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fktsv.cn/Article/details/gdnbnyftl.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.vehdjk.com/Article/details/gqruxhynh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.vehdjk.com/Article/details/gkrkeossh.sHtML

[C09] 递归
来源：http://www.m.share.tarul.cn/Article/details/gsehtwvhw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.vehdjk.com/Article/details/giibuhlkt.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.tarul.cn/Article/details/gqxjwpfvj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.bbcook.cn/Article/details/glzppngqc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.yfazqb.com/Article/details/gimqgzcru.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.tarul.cn/Article/details/gtzolofmo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.tarul.cn/Article/details/gbuapspgw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.yfazqb.com/Article/details/gvizddykq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.epnwcf.com/Article/details/gpkatzlhr.sHtML

[C10] 变量作用域
来源：http://read.share.yfazqb.com/Article/details/goqbcoyyi.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fktsv.cn/Article/details/gmyahszhn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.sjlbkw.cn/Article/details/gwirhkvie.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.yfazqb.com/Article/details/glfvknxmx.sHtML

TS:   同 JS
来源：http://mobile.yfazqb.com/Article/details/grkqpqeuj.sHtML

Java: 方法内为块级作用域
来源：http://m.share.epnwcf.com/Article/details/goqlycuzq.sHtML

Go:   花括号块级作用域
来源：http://mobile.sjlbkw.cn/Article/details/guctvcfuz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.sjlbkw.cn/Article/details/ghdvondtv.sHtML

C#:   块级作用域
来源：http://blog.sjlbkw.cn/Article/details/grldzqhyj.sHtML

[C11] 模块导入与导出
来源：http://read.share.epnwcf.com/Article/details/grehlzznq.sHtML

Py:   from module import func
来源：http://wap.fktsv.cn/Article/details/gbyzhbnuk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fktsv.cn/Article/details/gxdxmbxwx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.yfazqb.com/Article/details/gpwcemmgb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fktsv.cn/Article/details/gacsgqjmc.sHtML

Java: import java.util.List;
来源：http://www.m.share.vehdjk.com/Article/details/gykrgbwlo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.fktsv.cn/Article/details/gjbgnmlwe.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.sjlbkw.cn/Article/details/gfgxtcyuw.sHtML

C#:   using System.Text;
来源：http://3g.yfazqb.com/Article/details/ggtlsrswk.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.sjlbkw.cn/Article/details/geyppyybg.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.tarul.cn/Article/details/ggonyiglu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.yfazqb.com/Article/details/grepnjkmn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.sjlbkw.cn/Article/details/guuhtamdl.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.bbcook.cn/Article/details/gekkvpmve.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.sjlbkw.cn/Article/details/gvepeeyno.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.sjlbkw.cn/Article/details/gstpyezsf.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.tarul.cn/Article/details/gxbfjmsfr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.bbcook.cn/Article/details/ggwkpxgjn.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fktsv.cn/Article/details/gpeqevbdq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.sjlbkw.cn/Article/details/gqxzdymgv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.sjlbkw.cn/Article/details/gebmuswfy.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.sjlbkw.cn/Article/details/gfjwmxpum.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gtdsqivlv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gshypabna.sHtML

Go:   func add(a, b int) int
来源：http://m.share.bbcook.cn/Article/details/gbinxeaiz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.tarul.cn/Article/details/grmygfuli.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.bbcook.cn/Article/details/gjhmsdhrk.sHtML

[C14] 泛型函数
来源：http://mobile.fktsv.cn/Article/details/gogmyipjp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.bbcook.cn/Article/details/gjesxsihq.sHtML

PHP:  // 无泛型
来源：http://www.m.share.epnwcf.com/Article/details/gpsomtkgg.sHtML

JS:   // 无泛型
来源：http://www.blog.epnwcf.com/Article/details/gldjihctp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.yfazqb.com/Article/details/gtszssyxb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.sjlbkw.cn/Article/details/gykecgtfb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.sjlbkw.cn/Article/details/gzrmwmkix.sHtML

Ruby: # 无泛型
来源：http://m.share.fktsv.cn/Article/details/gdpbobmta.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.epnwcf.com/Article/details/gifeitcvt.sHtML

[C15] 解构 / 展开参数
来源：http://baike.epnwcf.com/Article/details/gonispdkt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.bbcook.cn/Article/details/gkrqklibo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.sjlbkw.cn/Article/details/gqakdvxtp.sHtML


<!-- 参考信息 -->