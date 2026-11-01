代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://www.share.epnwcf.com/Article/details/gttcyppak.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.epnwcf.com/Article/details/gdtfvsxct.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.fktsv.cn/Article/details/gqrnfsktu.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.fktsv.cn/Article/details/gzfawhzqh.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.bbcook.cn/Article/details/gvetdtstc.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gqyfdfjta.sHtML

B. 流程控制
来源：http://m.share.bbcook.cn/Article/details/gqceovytz.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gthdkihji.sHtML

[B01] 条件判断 if / else
来源：http://wap.fktsv.cn/Article/details/ggmijisgo.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.epnwcf.com/Article/details/gxaujugqf.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.epnwcf.com/Article/details/gwajblwre.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.yfazqb.com/Article/details/gbpxeddcg.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.bbcook.cn/Article/details/ghynhmgxy.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.bbcook.cn/Article/details/gqkfnryei.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.vehdjk.com/Article/details/gjawvafnx.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.epnwcf.com/Article/details/gxctkkcys.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.sjlbkw.cn/Article/details/gbsxestnb.sHtML

[B02] 多分支 else if / elif
来源：http://3g.fktsv.cn/Article/details/gpfjcpdle.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.bbcook.cn/Article/details/gsmctyzaa.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.epnwcf.com/Article/details/glfqetnsx.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.tarul.cn/Article/details/gohcyqdeq.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.vehdjk.com/Article/details/gorfqwffu.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.bbcook.cn/Article/details/gsxhqykua.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gydnitcuc.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.bbcook.cn/Article/details/gwyckjsqf.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.tarul.cn/Article/details/goxitxffg.sHtML

[B03] switch / match / case
来源：http://wap.sjlbkw.cn/Article/details/gogoepuet.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.fktsv.cn/Article/details/gyermlasv.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.epnwcf.com/Article/details/ghenplwjt.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.vehdjk.com/Article/details/gtilnegwy.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fktsv.cn/Article/details/gffvfkich.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.bbcook.cn/Article/details/gzxrfejlk.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.fktsv.cn/Article/details/gsvgubywe.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.yfazqb.com/Article/details/grdvkfihk.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.epnwcf.com/Article/details/glcmdlnnw.sHtML

[B04] for 计数循环
来源：http://wap.sjlbkw.cn/Article/details/glvekrqlc.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.sjlbkw.cn/Article/details/gnjjnynaj.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.tarul.cn/Article/details/gsfchtxdv.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.sjlbkw.cn/Article/details/ggxxxjmdq.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.bbcook.cn/Article/details/gbdkaqzpy.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.vehdjk.com/Article/details/gviwzemij.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.vehdjk.com/Article/details/gajjjmulw.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.sjlbkw.cn/Article/details/glkgvshlq.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.tarul.cn/Article/details/gkglnaepr.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.bbcook.cn/Article/details/gxzpmczxf.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.bbcook.cn/Article/details/ggyeoqjyn.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.sjlbkw.cn/Article/details/gvdkeysxj.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.bbcook.cn/Article/details/gcmbtemsj.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.vehdjk.com/Article/details/gjxqxswcj.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.sjlbkw.cn/Article/details/gwmydtezf.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.sjlbkw.cn/Article/details/gayzyhpnt.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.fktsv.cn/Article/details/gfbvtivrp.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.vehdjk.com/Article/details/gwcwpomcl.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.bbcook.cn/Article/details/gurnmukzh.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.bbcook.cn/Article/details/gizlcwbkp.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpfpyojvp.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.bbcook.cn/Article/details/gmholrohh.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.bbcook.cn/Article/details/gobawimie.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.vehdjk.com/Article/details/gufdlhxvv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.bbcook.cn/Article/details/gwgspacmy.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.bbcook.cn/Article/details/gawezgsxu.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.yfazqb.com/Article/details/gybtcesia.sHtML

[B07] while 循环
来源：http://m.share.bbcook.cn/Article/details/gfkggbflw.sHtML

Py:   while i < 10: i += 1
来源：http://3g.bbcook.cn/Article/details/gmvpxsulw.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.bbcook.cn/Article/details/gaqcclycv.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.sjlbkw.cn/Article/details/gusshlkzy.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.yfazqb.com/Article/details/gmekkzwyd.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.bbcook.cn/Article/details/gygfmocgk.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.epnwcf.com/Article/details/glfiwcbed.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.yfazqb.com/Article/details/gzarymwrz.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.yfazqb.com/Article/details/gbdsptwwl.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.sjlbkw.cn/Article/details/gzyktdcwf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.tarul.cn/Article/details/gvlmcznts.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.epnwcf.com/Article/details/giqydiqgl.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.epnwcf.com/Article/details/gqwgudqwz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.bbcook.cn/Article/details/germpmxnb.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.bbcook.cn/Article/details/gzftnzdim.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.sjlbkw.cn/Article/details/gikowjsrb.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.epnwcf.com/Article/details/geklxifhb.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.epnwcf.com/Article/details/gfixdrzwv.sHtML

[B09] break 与 continue
来源：http://m.share.vehdjk.com/Article/details/guoaltwrp.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.yfazqb.com/Article/details/gwwxbioey.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.sjlbkw.cn/Article/details/gfpcawqsn.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fktsv.cn/Article/details/gvccfzcye.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.epnwcf.com/Article/details/ggojwjxib.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/ggaxorhun.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.tarul.cn/Article/details/gldkoqedj.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.fktsv.cn/Article/details/gkdhvoytg.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.yfazqb.com/Article/details/gpsivvjrr.sHtML

[B10] 遍历同时拿索引
来源：http://baike.vehdjk.com/Article/details/gqqciropk.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.sjlbkw.cn/Article/details/gkojppmtr.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.yfazqb.com/Article/details/gvzdmwxcc.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.fktsv.cn/Article/details/gjyoddunr.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.bbcook.cn/Article/details/gstgbsvhc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.tarul.cn/Article/details/gzfmgeufh.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fktsv.cn/Article/details/gcwvivjnn.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.yfazqb.com/Article/details/gfxmvgkfb.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.sjlbkw.cn/Article/details/gdzpaddrp.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.yfazqb.com/Article/details/grwgmgmhx.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.bbcook.cn/Article/details/gtjhllokw.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.fktsv.cn/Article/details/glcxevgql.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.yfazqb.com/Article/details/gqstwycdv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.yfazqb.com/Article/details/gcplnuhcy.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.sjlbkw.cn/Article/details/gloceucjz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.sjlbkw.cn/Article/details/geyaqczwp.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.vehdjk.com/Article/details/gacylvkwk.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.tarul.cn/Article/details/grtoqargr.sHtML

[B12] 跳出多层循环
来源：http://blog.bbcook.cn/Article/details/gpjnbrbhd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.sjlbkw.cn/Article/details/gsmlyusqs.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.yfazqb.com/Article/details/gxsqdgqqw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gifjwsoxg.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.bbcook.cn/Article/details/gocmovyxb.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.yfazqb.com/Article/details/gacjbtcor.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.fktsv.cn/Article/details/gmvtmieei.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.sjlbkw.cn/Article/details/gmmxroyai.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.epnwcf.com/Article/details/gsunnndez.sHtML

[B13] 判断是否为数字
来源：http://read.share.tarul.cn/Article/details/getjyfwje.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.vehdjk.com/Article/details/gjuseaiku.sHtML

PHP:  is_numeric($x)
来源：http://read.share.epnwcf.com/Article/details/gaijzvlsz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.vehdjk.com/Article/details/gfkdozkwo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.vehdjk.com/Article/details/gkmxmhwgb.sHtML

Java: x instanceof Number
来源：http://3g.fktsv.cn/Article/details/gongrgqwb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.bbcook.cn/Article/details/gzkszhhoa.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.bbcook.cn/Article/details/gaqhdexpl.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.vehdjk.com/Article/details/gxbdpiswi.sHtML

[B14] 判断值是否在集合内
来源：http://3g.tarul.cn/Article/details/gdmghuwlq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.sjlbkw.cn/Article/details/gaybfizgr.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fktsv.cn/Article/details/ggfvscwnn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.yfazqb.com/Article/details/gbwxzvjkg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.vehdjk.com/Article/details/gkxwkrspv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.sjlbkw.cn/Article/details/gzibqmhol.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fktsv.cn/Article/details/gxjhewjod.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.tarul.cn/Article/details/gojbjdovw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.tarul.cn/Article/details/godyfrkob.sHtML

[B15] 布尔运算与取反
来源：http://baike.fktsv.cn/Article/details/gvmvqfglb.sHtML

Py:   a and b or not c
来源：http://read.share.fktsv.cn/Article/details/gjscceanx.sHtML

PHP:  $a && $b || !$c
来源：http://wap.epnwcf.com/Article/details/gtkaixdww.sHtML

JS:   a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/gadhaoxcp.sHtML

TS:   a && b || !c
来源：http://mobile.fktsv.cn/Article/details/gmupavxhc.sHtML

Java: a && b || !c
来源：http://mobile.tarul.cn/Article/details/gneyblsaz.sHtML

Go:   a && b || !c
来源：http://blog.vehdjk.com/Article/details/gtwunbzru.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/gtcgdfimt.sHtML

C#:   a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/gtjhoiyma.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.sjlbkw.cn/Article/details/ghpvkeami.sHtML

Py:   if not data: return
来源：http://www.m.share.yfazqb.com/Article/details/gcftvmmjz.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.yfazqb.com/Article/details/gezscjtow.sHtML

JS:   if (!data) return;
来源：http://www.share.sjlbkw.cn/Article/details/ggmhgomxq.sHtML

TS:   if (!data) return;
来源：http://baike.bbcook.cn/Article/details/gdpdvysbk.sHtML

Java: if (data == null) return;
来源：http://www.share.epnwcf.com/Article/details/gjfwcacru.sHtML

Go:   if data == nil { return }
来源：http://mobile.fktsv.cn/Article/details/gbriojgkk.sHtML

Ruby: return if data.nil?
来源：http://wap.yfazqb.com/Article/details/gdjsgueek.sHtML

C#:   if (data == null) return;
来源：http://3g.sjlbkw.cn/Article/details/ggokuyzzu.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gwpivgjsy.sHtML

C. 函数与作用域
来源：http://read.share.fktsv.cn/Article/details/gvxxibluj.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gspcatgok.sHtML

[C01] 定义函数
来源：http://www.share.tarul.cn/Article/details/gpchhyvwx.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.tarul.cn/Article/details/gheiqokhv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fktsv.cn/Article/details/ggjiffrzv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fktsv.cn/Article/details/gpmofuqsp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/ghsedokcx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gbyuizcpv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.epnwcf.com/Article/details/ggthnxupw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.sjlbkw.cn/Article/details/gzzqtluya.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gjscvvktt.sHtML

[C02] 默认参数
来源：http://m.share.tarul.cn/Article/details/gscccfoqn.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fktsv.cn/Article/details/gttwukrlu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.sjlbkw.cn/Article/details/gdtflpykl.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/gctupbreg.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.epnwcf.com/Article/details/gpgxwrqng.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.tarul.cn/Article/details/grthdiwwn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.tarul.cn/Article/details/gqcchhrmf.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fktsv.cn/Article/details/gxldscqkk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.yfazqb.com/Article/details/gdxqirrlg.sHtML

[C03] 可变参数
来源：http://3g.yfazqb.com/Article/details/gebfqcrui.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.epnwcf.com/Article/details/gjogtvbvt.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fktsv.cn/Article/details/gysagqanz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.epnwcf.com/Article/details/gzymwnsir.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.bbcook.cn/Article/details/gxdhdhrnx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.yfazqb.com/Article/details/glyerrdmx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.vehdjk.com/Article/details/gjhysjibk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.sjlbkw.cn/Article/details/gfjlmkiec.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.bbcook.cn/Article/details/gfyiryznp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fktsv.cn/Article/details/gwfvfmxer.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.vehdjk.com/Article/details/gwhfgxvlp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.bbcook.cn/Article/details/gtbrdozkr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fktsv.cn/Article/details/geurvkeas.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.vehdjk.com/Article/details/gugodghbi.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.yfazqb.com/Article/details/gyniahhsa.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fktsv.cn/Article/details/gqmjrykzn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.vehdjk.com/Article/details/grondvlwj.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.vehdjk.com/Article/details/gfximuyzc.sHtML

[C05] 返回多个值
来源：http://www.blog.bbcook.cn/Article/details/gsqpynhls.sHtML

Py:   return a, b
来源：http://wap.epnwcf.com/Article/details/gxqhyldyn.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.vehdjk.com/Article/details/giqsopduo.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.fktsv.cn/Article/details/ggwrubvgh.sHtML

TS:   return { a, b };
来源：http://www.share.sjlbkw.cn/Article/details/giawsblkf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fktsv.cn/Article/details/gotcoggdl.sHtML

Go:   return a, b
来源：http://www.m.share.sjlbkw.cn/Article/details/gekxpvbdk.sHtML

Ruby: return a, b
来源：http://3g.yfazqb.com/Article/details/glmzuubty.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.bbcook.cn/Article/details/gfbotfniu.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.yfazqb.com/Article/details/gbbszhmqf.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.sjlbkw.cn/Article/details/gqzpkxkck.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.bbcook.cn/Article/details/gdgmlhenb.sHtML

JS:   const square = x => x * x;
来源：http://mobile.sjlbkw.cn/Article/details/gdnflcyfz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fktsv.cn/Article/details/guvgpsbzv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.epnwcf.com/Article/details/gxefkwcyn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.epnwcf.com/Article/details/gwoxidzem.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.vehdjk.com/Article/details/gvvxktnay.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.yfazqb.com/Article/details/goomanjgd.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.yfazqb.com/Article/details/gxbtadnlp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.yfazqb.com/Article/details/gmuejcpmr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.sjlbkw.cn/Article/details/gfcejhiyp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.yfazqb.com/Article/details/gpypngnxk.sHtML

TS:   arr.map(String)
来源：http://wap.fktsv.cn/Article/details/gyrgiebio.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.yfazqb.com/Article/details/gdujhghdf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.yfazqb.com/Article/details/gdhpquwcs.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.yfazqb.com/Article/details/gozhmfhoe.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.fktsv.cn/Article/details/gqdwbxere.sHtML

[C08] 闭包
来源：http://wap.epnwcf.com/Article/details/gfocmqaxa.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.yfazqb.com/Article/details/gigbzprcr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fktsv.cn/Article/details/glheeudwf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.sjlbkw.cn/Article/details/gskmzmitv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.tarul.cn/Article/details/gfkwoxmka.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.sjlbkw.cn/Article/details/gzvysbkaw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.epnwcf.com/Article/details/gafyvkkox.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fktsv.cn/Article/details/gpnliwfrj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.tarul.cn/Article/details/goffdjwbb.sHtML

[C09] 递归
来源：http://read.share.bbcook.cn/Article/details/gkttnbiml.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/garertraw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.epnwcf.com/Article/details/ggfuyqmqd.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.bbcook.cn/Article/details/gksvibfju.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fktsv.cn/Article/details/geswikrxr.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.yfazqb.com/Article/details/gajdotzaa.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.yfazqb.com/Article/details/guttkhact.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fktsv.cn/Article/details/glfmdbuxo.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fktsv.cn/Article/details/gxmfvsmys.sHtML

[C10] 变量作用域
来源：http://www.blog.epnwcf.com/Article/details/gebfkbpik.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.bbcook.cn/Article/details/gqagjxziu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.epnwcf.com/Article/details/gqnxksuzk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.epnwcf.com/Article/details/grxcemtlx.sHtML

TS:   同 JS
来源：http://www.share.yfazqb.com/Article/details/gxdqxohhy.sHtML

Java: 方法内为块级作用域
来源：http://www.share.tarul.cn/Article/details/gvqfkcetw.sHtML

Go:   花括号块级作用域
来源：http://3g.vehdjk.com/Article/details/geggjpitl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fktsv.cn/Article/details/gykisbekf.sHtML

C#:   块级作用域
来源：http://wap.fktsv.cn/Article/details/gbyzddizx.sHtML

[C11] 模块导入与导出
来源：http://3g.bbcook.cn/Article/details/gxkktjxrf.sHtML

Py:   from module import func
来源：http://www.m.share.bbcook.cn/Article/details/gxewcscrb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.yfazqb.com/Article/details/gxccddbwz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.vehdjk.com/Article/details/gliivpzze.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.vehdjk.com/Article/details/gseliqqmh.sHtML

Java: import java.util.List;
来源：http://www.m.share.fktsv.cn/Article/details/gwkqkktzp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.bbcook.cn/Article/details/gjwkearxw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.sjlbkw.cn/Article/details/gfkugugab.sHtML

C#:   using System.Text;
来源：http://www.m.share.fktsv.cn/Article/details/gaalauxjt.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.vehdjk.com/Article/details/gwbbehtyn.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.sjlbkw.cn/Article/details/gggevflod.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.yfazqb.com/Article/details/gtglrlfvu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.vehdjk.com/Article/details/grijqadmk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.yfazqb.com/Article/details/givjmpivr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.yfazqb.com/Article/details/gkhasfbkz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.yfazqb.com/Article/details/gbkeoscuu.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.tarul.cn/Article/details/gqgybajks.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.bbcook.cn/Article/details/gljhjvsgw.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.yfazqb.com/Article/details/gdkcnwtpq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.vehdjk.com/Article/details/gnejcetzk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.sjlbkw.cn/Article/details/gskrqgqtu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.bbcook.cn/Article/details/gmxtxrsbo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/gaqgjwyvx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.vehdjk.com/Article/details/gientdtzz.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fktsv.cn/Article/details/gfjsmbujs.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.sjlbkw.cn/Article/details/gvxtjazde.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.epnwcf.com/Article/details/gskzrpkfx.sHtML

[C14] 泛型函数
来源：http://www.blog.sjlbkw.cn/Article/details/grlusxkel.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.vehdjk.com/Article/details/gfkqfxmst.sHtML

PHP:  // 无泛型
来源：http://www.share.epnwcf.com/Article/details/gzihwddqx.sHtML

JS:   // 无泛型
来源：http://read.share.fktsv.cn/Article/details/gaqwtjval.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.tarul.cn/Article/details/gmxyfrkpj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.bbcook.cn/Article/details/gyfxliahp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.epnwcf.com/Article/details/ggpepfaet.sHtML

Ruby: # 无泛型
来源：http://baike.sjlbkw.cn/Article/details/gdxuxzems.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.bbcook.cn/Article/details/glbmkgjzb.sHtML

[C15] 解构 / 展开参数
来源：http://3g.bbcook.cn/Article/details/gdmtxvfyj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.vehdjk.com/Article/details/gygnfjdor.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.sjlbkw.cn/Article/details/gkmlenbks.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.bbcook.cn/Article/details/gbqlopxjc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.tarul.cn/Article/details/gegctihnz.sHtML

Java: // 无解构
来源：http://mobile.bbcook.cn/Article/details/guoafnrjg.sHtML

Go:   // 无解构
来源：http://3g.bbcook.cn/Article/details/gaclpdaeg.sHtML

Ruby: a, b = pair
来源：http://baike.epnwcf.com/Article/details/gbtwiazwy.sHtML

C#:   var (a, b) = pair;
来源：http://3g.epnwcf.com/Article/details/gtudlbljt.sHtML

[C16] 函数 / 方法重载
来源：http://wap.yfazqb.com/Article/details/goqagwrod.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.epnwcf.com/Article/details/gmqnyqwto.sHtML

PHP:  // 无重载
来源：http://baike.yfazqb.com/Article/details/gkpespyva.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fktsv.cn/Article/details/gmlavatio.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.yfazqb.com/Article/details/gpkrsjhim.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.epnwcf.com/Article/details/gpmlwziya.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fktsv.cn/Article/details/gcfmxsobo.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.bbcook.cn/Article/details/gweikdvbt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.vehdjk.com/Article/details/gwlfseoal.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gnvcoshnx.sHtML


<!-- 参考信息 -->