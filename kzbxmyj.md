代发 wailian999

[A26] 类型转换总览
来源：http://m.share.epnwcf.com/Article/details/gtrkwzqdy.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.sjlbkw.cn/Article/details/gwwngdazm.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.bbcook.cn/Article/details/gsaoofhxw.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.tarul.cn/Article/details/giqqxiotk.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.epnwcf.com/Article/details/gdaykmizk.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.bbcook.cn/Article/details/gpmtlayxg.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.yfazqb.com/Article/details/gzfbdofpv.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.yfazqb.com/Article/details/gbpiwxirw.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.vehdjk.com/Article/details/gnpvzwujk.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/goyajlrui.sHtML

B. 流程控制
来源：http://www.m.share.vehdjk.com/Article/details/gqpohjttn.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gajqukepa.sHtML

[B01] 条件判断 if / else
来源：http://www.share.yfazqb.com/Article/details/ghwlkwjza.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.epnwcf.com/Article/details/gwqwwdfcw.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.sjlbkw.cn/Article/details/gxdfquyeo.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.sjlbkw.cn/Article/details/gdeuxmujq.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.tarul.cn/Article/details/gyivywbve.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.vehdjk.com/Article/details/guktpchtk.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.epnwcf.com/Article/details/gzzecppvb.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.yfazqb.com/Article/details/gayqwcccr.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.bbcook.cn/Article/details/gowkhisbj.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.bbcook.cn/Article/details/gkzixirej.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.bbcook.cn/Article/details/ggcfqfovm.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.sjlbkw.cn/Article/details/gqvrpuusw.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.yfazqb.com/Article/details/gjfymkcsj.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.epnwcf.com/Article/details/ghrrqfqqb.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.yfazqb.com/Article/details/gqdjineyq.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.tarul.cn/Article/details/gztunqdvz.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.yfazqb.com/Article/details/gzthbhfps.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.epnwcf.com/Article/details/geooszlek.sHtML

[B03] switch / match / case
来源：http://3g.tarul.cn/Article/details/gnllcvkla.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.yfazqb.com/Article/details/guioadrmc.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.vehdjk.com/Article/details/gquednupe.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.tarul.cn/Article/details/gkfedfhfe.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fktsv.cn/Article/details/grqezfims.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.tarul.cn/Article/details/gwpodedqw.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.yfazqb.com/Article/details/gindzyggp.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.yfazqb.com/Article/details/gtsgydqym.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.sjlbkw.cn/Article/details/gnlxobrop.sHtML

[B04] for 计数循环
来源：http://blog.fktsv.cn/Article/details/gmngmbghc.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.yfazqb.com/Article/details/gqwjdpiwj.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.tarul.cn/Article/details/grmbpiozb.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.vehdjk.com/Article/details/gexmavtpz.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fktsv.cn/Article/details/guoqohwzg.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.yfazqb.com/Article/details/gcdpuiwvu.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.fktsv.cn/Article/details/gxuayldsu.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.vehdjk.com/Article/details/gchzdjgtx.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.bbcook.cn/Article/details/gwbxsowtw.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.tarul.cn/Article/details/gstegogzg.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.bbcook.cn/Article/details/glzlkdxpj.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.tarul.cn/Article/details/glaxwrhrm.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.bbcook.cn/Article/details/glsfbqqbk.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.epnwcf.com/Article/details/grugpwwpk.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.yfazqb.com/Article/details/gwbtcwhqf.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.sjlbkw.cn/Article/details/glchkyann.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.tarul.cn/Article/details/gyiqsinfe.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.tarul.cn/Article/details/gqyejplsw.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.yfazqb.com/Article/details/gpbelbppm.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.tarul.cn/Article/details/gpjubsofx.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.vehdjk.com/Article/details/guxqgzfkx.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.bbcook.cn/Article/details/gurutmwmi.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.bbcook.cn/Article/details/grhlxcfwb.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.yfazqb.com/Article/details/gahffxhrm.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.bbcook.cn/Article/details/glmheqwov.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.sjlbkw.cn/Article/details/gbsqqipyu.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.epnwcf.com/Article/details/ghibrnbvt.sHtML

[B07] while 循环
来源：http://3g.tarul.cn/Article/details/gfudqszxq.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.yfazqb.com/Article/details/gtrjgaqtk.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.fktsv.cn/Article/details/gjjsmrxdg.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.sjlbkw.cn/Article/details/gxvkctxpk.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.yfazqb.com/Article/details/gnkpzusla.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.epnwcf.com/Article/details/gjxonuqdj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.fktsv.cn/Article/details/gbbhcgwxf.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.tarul.cn/Article/details/gmiojsnjb.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.fktsv.cn/Article/details/gwomaablr.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.tarul.cn/Article/details/ggoisppvi.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.yfazqb.com/Article/details/ginoqfljc.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.bbcook.cn/Article/details/ggekudkhe.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.bbcook.cn/Article/details/giutqqdty.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.tarul.cn/Article/details/gwziojlha.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.yfazqb.com/Article/details/gvrhxcqhk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.epnwcf.com/Article/details/gytxfpwly.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.fktsv.cn/Article/details/gscuqjqdr.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.yfazqb.com/Article/details/gclmzoega.sHtML

[B09] break 与 continue
来源：http://www.m.share.tarul.cn/Article/details/grvbhuyul.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.tarul.cn/Article/details/gvxowwcjf.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.tarul.cn/Article/details/gbvikmbdi.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.yfazqb.com/Article/details/gzrhyqvwb.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.epnwcf.com/Article/details/grewtdyxd.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/glcammppy.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.bbcook.cn/Article/details/gupnlytsp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.sjlbkw.cn/Article/details/gzfdxpswa.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.epnwcf.com/Article/details/gkaxxprqz.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.bbcook.cn/Article/details/gibaavbhu.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.epnwcf.com/Article/details/guilmrwmc.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.sjlbkw.cn/Article/details/gcnghspdh.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.tarul.cn/Article/details/ggvjdxlpy.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.fktsv.cn/Article/details/gttekvmii.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.bbcook.cn/Article/details/ghysjfdzz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.vehdjk.com/Article/details/grxteiphr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.fktsv.cn/Article/details/gfuptdkpd.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.vehdjk.com/Article/details/gempdscbk.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.fktsv.cn/Article/details/gealuveqv.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.yfazqb.com/Article/details/gvroevtzr.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.bbcook.cn/Article/details/ggdkdnzyc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fktsv.cn/Article/details/gxnfcannr.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.tarul.cn/Article/details/gwcvdbknk.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.fktsv.cn/Article/details/gmnxaywzx.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.yfazqb.com/Article/details/gpsevdxpc.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.yfazqb.com/Article/details/grytliiqo.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.bbcook.cn/Article/details/gulslolmx.sHtML

[B12] 跳出多层循环
来源：http://blog.bbcook.cn/Article/details/gobleagxa.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.vehdjk.com/Article/details/gojavehhf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.bbcook.cn/Article/details/gfqicedsq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fktsv.cn/Article/details/gdzdrcwzw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.yfazqb.com/Article/details/gsscnpavi.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.vehdjk.com/Article/details/ggfcoxavm.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.tarul.cn/Article/details/gjzsnlbly.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.yfazqb.com/Article/details/gwthyrpox.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.yfazqb.com/Article/details/gitdbfsce.sHtML

[B13] 判断是否为数字
来源：http://read.share.tarul.cn/Article/details/gsjzgkfdn.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.yfazqb.com/Article/details/gwnkgwtuy.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.tarul.cn/Article/details/gmnbowvhi.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.bbcook.cn/Article/details/gkmmaxktx.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.tarul.cn/Article/details/glggrbdwp.sHtML

Java: x instanceof Number
来源：http://www.share.tarul.cn/Article/details/ghxwhryrp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.sjlbkw.cn/Article/details/gefygiicm.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.bbcook.cn/Article/details/godwheliq.sHtML

C#:   x is int or double or decimal
来源：http://m.share.yfazqb.com/Article/details/gbolgvlzh.sHtML

[B14] 判断值是否在集合内
来源：http://wap.epnwcf.com/Article/details/grqwgzhkw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.tarul.cn/Article/details/gfrzynbfa.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.yfazqb.com/Article/details/gjxbkcfyn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.sjlbkw.cn/Article/details/gmqqbdcls.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fktsv.cn/Article/details/gaoqwkcpm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.epnwcf.com/Article/details/gtipeqftv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.bbcook.cn/Article/details/gdgnzowrc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.yfazqb.com/Article/details/gzcdghmea.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fktsv.cn/Article/details/giyhexzyt.sHtML

[B15] 布尔运算与取反
来源：http://wap.fktsv.cn/Article/details/gnauiwvql.sHtML

Py:   a and b or not c
来源：http://3g.sjlbkw.cn/Article/details/gtugfchym.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.yfazqb.com/Article/details/gmlixszid.sHtML

JS:   a && b || !c
来源：http://www.blog.sjlbkw.cn/Article/details/gvolcnjpz.sHtML

TS:   a && b || !c
来源：http://blog.sjlbkw.cn/Article/details/grfvycstu.sHtML

Java: a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/ggxkptvft.sHtML

Go:   a && b || !c
来源：http://3g.fktsv.cn/Article/details/gdfsmmozm.sHtML

Ruby: a && b || !c
来源：http://mobile.tarul.cn/Article/details/gikwtuknq.sHtML

C#:   a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gzlqkvmkw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.bbcook.cn/Article/details/glfitzrhc.sHtML

Py:   if not data: return
来源：http://baike.yfazqb.com/Article/details/gkvyadejy.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.epnwcf.com/Article/details/gsctrwumj.sHtML

JS:   if (!data) return;
来源：http://www.share.tarul.cn/Article/details/gjwhbqdnc.sHtML

TS:   if (!data) return;
来源：http://wap.tarul.cn/Article/details/gzgfuftiw.sHtML

Java: if (data == null) return;
来源：http://wap.fktsv.cn/Article/details/gvhttdquw.sHtML

Go:   if data == nil { return }
来源：http://read.share.sjlbkw.cn/Article/details/gbexjjhwn.sHtML

Ruby: return if data.nil?
来源：http://3g.epnwcf.com/Article/details/gkmlfimqy.sHtML

C#:   if (data == null) return;
来源：http://www.share.tarul.cn/Article/details/gfxxdsweg.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gtxazqayf.sHtML

C. 函数与作用域
来源：http://read.share.fktsv.cn/Article/details/gphybdven.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gjwyndchc.sHtML

[C01] 定义函数
来源：http://www.blog.sjlbkw.cn/Article/details/gntefbjjn.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.bbcook.cn/Article/details/gjkvtdzju.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.vehdjk.com/Article/details/gsphrwpjn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/gknfaavdq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gvovkzhyk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/grgbremzc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.sjlbkw.cn/Article/details/grrowiqin.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fktsv.cn/Article/details/gnvsohvgx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/gzwlixecd.sHtML

[C02] 默认参数
来源：http://m.share.sjlbkw.cn/Article/details/givnydkgi.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.sjlbkw.cn/Article/details/gnnwnkomy.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.tarul.cn/Article/details/govtoftlb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fktsv.cn/Article/details/gnwijrvkp.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.vehdjk.com/Article/details/gnwygvqfv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.yfazqb.com/Article/details/ganwpzusi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.epnwcf.com/Article/details/gosmazsix.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.tarul.cn/Article/details/gtmzveokd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.bbcook.cn/Article/details/gtcqcwinb.sHtML

[C03] 可变参数
来源：http://read.share.vehdjk.com/Article/details/gddfkpjci.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.vehdjk.com/Article/details/gfhgrwziz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.tarul.cn/Article/details/gdiofdyoo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjglnxgvi.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.yfazqb.com/Article/details/gcgdteizt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.yfazqb.com/Article/details/gylumhfnv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.bbcook.cn/Article/details/ggzgaclli.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.yfazqb.com/Article/details/ghhhoiwpz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.epnwcf.com/Article/details/gxbswyddm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.sjlbkw.cn/Article/details/gnmyijsgy.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.bbcook.cn/Article/details/gtfhivslw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.sjlbkw.cn/Article/details/gtdbkoywl.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.tarul.cn/Article/details/gayfpncrl.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.sjlbkw.cn/Article/details/glfkqluae.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.sjlbkw.cn/Article/details/gyenvstcy.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.vehdjk.com/Article/details/gshrdzeqx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.vehdjk.com/Article/details/gwfswqdqf.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.yfazqb.com/Article/details/ghhzmdzlv.sHtML

[C05] 返回多个值
来源：http://baike.vehdjk.com/Article/details/ggmklgxgz.sHtML

Py:   return a, b
来源：http://blog.epnwcf.com/Article/details/gtjgljlnn.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.vehdjk.com/Article/details/gpuusjkxr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.tarul.cn/Article/details/gyknliuse.sHtML

TS:   return { a, b };
来源：http://www.share.epnwcf.com/Article/details/gjxezyjty.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fktsv.cn/Article/details/gfrelwazs.sHtML

Go:   return a, b
来源：http://blog.bbcook.cn/Article/details/gvfexalhb.sHtML

Ruby: return a, b
来源：http://www.share.vehdjk.com/Article/details/ggpvijfji.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.epnwcf.com/Article/details/gchkyqeaz.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.yfazqb.com/Article/details/gmxjbidmg.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fktsv.cn/Article/details/gyafxjgxi.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.tarul.cn/Article/details/ggjrpirld.sHtML

JS:   const square = x => x * x;
来源：http://3g.sjlbkw.cn/Article/details/gppxziqol.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.vehdjk.com/Article/details/gurgnzowu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fktsv.cn/Article/details/gkclpelks.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.vehdjk.com/Article/details/guwqsaicj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.tarul.cn/Article/details/gezukvxii.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.vehdjk.com/Article/details/gxcfkyges.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.tarul.cn/Article/details/gegdbrhyu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.sjlbkw.cn/Article/details/gdkmeqgrg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.epnwcf.com/Article/details/gzqvfppow.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fktsv.cn/Article/details/gcyppfsxu.sHtML

TS:   arr.map(String)
来源：http://3g.bbcook.cn/Article/details/gfqskbzqw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.epnwcf.com/Article/details/giyzlottn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fktsv.cn/Article/details/ghlwkwslq.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.bbcook.cn/Article/details/gdiqteofu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.yfazqb.com/Article/details/gkbycdpwf.sHtML

[C08] 闭包
来源：http://wap.epnwcf.com/Article/details/gqfvcxqhg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.yfazqb.com/Article/details/grxihviae.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.tarul.cn/Article/details/gmmyzppnz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.sjlbkw.cn/Article/details/gvqfndszh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.bbcook.cn/Article/details/gaesthhiw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.bbcook.cn/Article/details/gqxmzglsq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.vehdjk.com/Article/details/gofucpoir.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.vehdjk.com/Article/details/gbmhixdcw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fktsv.cn/Article/details/gaiazswmd.sHtML

[C09] 递归
来源：http://mobile.sjlbkw.cn/Article/details/gocvgpqkr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.bbcook.cn/Article/details/gmqbptlbb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.vehdjk.com/Article/details/gcijcszwt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.tarul.cn/Article/details/geyicodgv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.tarul.cn/Article/details/gwfdilstk.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.sjlbkw.cn/Article/details/gtfnislff.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.tarul.cn/Article/details/gtmivqfot.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fktsv.cn/Article/details/glisgcrmo.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fktsv.cn/Article/details/gfthygbay.sHtML

[C10] 变量作用域
来源：http://3g.bbcook.cn/Article/details/gaoaeapxf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.yfazqb.com/Article/details/gfjjnivpg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.bbcook.cn/Article/details/gkqcbcpkf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.yfazqb.com/Article/details/gcjtsrsmp.sHtML

TS:   同 JS
来源：http://www.blog.yfazqb.com/Article/details/giteccxsm.sHtML

Java: 方法内为块级作用域
来源：http://mobile.tarul.cn/Article/details/gypcdfxlx.sHtML

Go:   花括号块级作用域
来源：http://baike.fktsv.cn/Article/details/gcewdjhpj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.vehdjk.com/Article/details/gmvmvlrip.sHtML

C#:   块级作用域
来源：http://3g.yfazqb.com/Article/details/gfccnmfml.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fktsv.cn/Article/details/gilrszvtl.sHtML

Py:   from module import func
来源：http://blog.fktsv.cn/Article/details/gairiryml.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.epnwcf.com/Article/details/gqgwnyfjm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.epnwcf.com/Article/details/gomhxicsm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.vehdjk.com/Article/details/gcrfvvmzu.sHtML

Java: import java.util.List;
来源：http://read.share.bbcook.cn/Article/details/gipjnrcul.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fktsv.cn/Article/details/gwwxdrazn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fktsv.cn/Article/details/gxfyocueg.sHtML

C#:   using System.Text;
来源：http://wap.bbcook.cn/Article/details/glsntuhah.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.epnwcf.com/Article/details/gvedkvabv.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.yfazqb.com/Article/details/gxfdejmmo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fktsv.cn/Article/details/gnklyxewc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.vehdjk.com/Article/details/gtcslhvvf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.sjlbkw.cn/Article/details/glmfwaqsm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.tarul.cn/Article/details/glertungi.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fktsv.cn/Article/details/grvkyfoti.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.sjlbkw.cn/Article/details/ggczaijlt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gacxnubua.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.epnwcf.com/Article/details/gurorargg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fktsv.cn/Article/details/gidkbjmbv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.bbcook.cn/Article/details/gdsbpxens.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.vehdjk.com/Article/details/ggmxfkzlz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gtcbtichr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.yfazqb.com/Article/details/gtooraodw.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.epnwcf.com/Article/details/goyhepmas.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.bbcook.cn/Article/details/gnyzlsaoy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.sjlbkw.cn/Article/details/giowtakex.sHtML

[C14] 泛型函数
来源：http://mobile.tarul.cn/Article/details/gvrmugslc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.yfazqb.com/Article/details/gxgmanfgt.sHtML

PHP:  // 无泛型
来源：http://mobile.bbcook.cn/Article/details/gmnodquyy.sHtML

JS:   // 无泛型
来源：http://www.m.share.tarul.cn/Article/details/gwvbwtbyc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.bbcook.cn/Article/details/gfmphmghi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fktsv.cn/Article/details/gomdlbwwc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.vehdjk.com/Article/details/gxquobluf.sHtML

Ruby: # 无泛型
来源：http://3g.vehdjk.com/Article/details/gkxlgoqep.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.bbcook.cn/Article/details/ggttgpqzx.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.vehdjk.com/Article/details/gaalxmpwj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fktsv.cn/Article/details/gbygmzmkv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.yfazqb.com/Article/details/gjbdrmvha.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.sjlbkw.cn/Article/details/gbsiutmkn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gzzoqgkfd.sHtML

Java: // 无解构
来源：http://blog.yfazqb.com/Article/details/gkmzbzyyj.sHtML

Go:   // 无解构
来源：http://blog.bbcook.cn/Article/details/gwjltnqpj.sHtML

Ruby: a, b = pair
来源：http://3g.tarul.cn/Article/details/ghaqygpyf.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.bbcook.cn/Article/details/gxoidfvkx.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fktsv.cn/Article/details/gdjvmrmrz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.vehdjk.com/Article/details/gnsenblxj.sHtML

PHP:  // 无重载
来源：http://www.blog.bbcook.cn/Article/details/grbsisxov.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.yfazqb.com/Article/details/gpkdxxqem.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.vehdjk.com/Article/details/geakigeud.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.tarul.cn/Article/details/gunrypclt.sHtML


<!-- 参考信息 -->