代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://wap.sjlbkw.cn/Article/details/gqrilggzx.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.bbcook.cn/Article/details/gqbqtmuhf.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.bbcook.cn/Article/details/gqfsxcdat.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.sjlbkw.cn/Article/details/gwuvmmfbk.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.bbcook.cn/Article/details/gkszhgfnn.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gzaolyqad.sHtML

B. 流程控制
来源：http://3g.vehdjk.com/Article/details/gfpdvauof.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/garxxtclv.sHtML

[B01] 条件判断 if / else
来源：http://www.share.sjlbkw.cn/Article/details/gpggsvfpe.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.bbcook.cn/Article/details/gwjijudfc.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.tarul.cn/Article/details/gytjjeyyy.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fktsv.cn/Article/details/guupggryo.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.sjlbkw.cn/Article/details/gxulgbvrx.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.sjlbkw.cn/Article/details/gitugmowz.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.epnwcf.com/Article/details/gardnjslq.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.vehdjk.com/Article/details/gijwmuioq.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.sjlbkw.cn/Article/details/geixhjjij.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.epnwcf.com/Article/details/ggwqpafqe.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.yfazqb.com/Article/details/gbgukilek.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.sjlbkw.cn/Article/details/gpkscbeqh.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.bbcook.cn/Article/details/ggltweuop.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.vehdjk.com/Article/details/gtjjtvngt.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.sjlbkw.cn/Article/details/gvfplowun.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.bbcook.cn/Article/details/ggophgdmp.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.epnwcf.com/Article/details/gvddyagll.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.sjlbkw.cn/Article/details/gorjzedob.sHtML

[B03] switch / match / case
来源：http://wap.vehdjk.com/Article/details/gqisgxitx.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.epnwcf.com/Article/details/gngtkuphz.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.vehdjk.com/Article/details/glxjwjzoo.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.epnwcf.com/Article/details/gywlduzhn.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.tarul.cn/Article/details/ggfmekuir.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkrptdnoq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.yfazqb.com/Article/details/gyxdjxnoq.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.vehdjk.com/Article/details/gbfudyjtq.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.fktsv.cn/Article/details/ghpyrrhpn.sHtML

[B04] for 计数循环
来源：http://baike.tarul.cn/Article/details/giafyfial.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.bbcook.cn/Article/details/gbgaexbdu.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.yfazqb.com/Article/details/goajzgdsn.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.vehdjk.com/Article/details/gkhrnrrcn.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.vehdjk.com/Article/details/grzmkkvqy.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.yfazqb.com/Article/details/gtjkbdhxf.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.sjlbkw.cn/Article/details/gjlhrvzov.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.bbcook.cn/Article/details/gybyqsdxe.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.sjlbkw.cn/Article/details/gdzmhstxq.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.tarul.cn/Article/details/gbhoxlpte.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghdhoeabo.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.bbcook.cn/Article/details/gdhdwhdkg.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.epnwcf.com/Article/details/gclkitgrh.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.vehdjk.com/Article/details/gwjdlllkq.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.bbcook.cn/Article/details/gsizvapqi.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.sjlbkw.cn/Article/details/gyezonkjm.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.epnwcf.com/Article/details/gjgzzqugo.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.tarul.cn/Article/details/grpghijbk.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.bbcook.cn/Article/details/grnjtsmcp.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.vehdjk.com/Article/details/gqcrvymny.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.epnwcf.com/Article/details/gjywbuxqo.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.yfazqb.com/Article/details/glpzpbwtp.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.tarul.cn/Article/details/gadgixzqk.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.yfazqb.com/Article/details/gkpkrzyxl.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.epnwcf.com/Article/details/gzidbcluu.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.yfazqb.com/Article/details/gookinlqt.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.yfazqb.com/Article/details/gxqdsaaid.sHtML

[B07] while 循环
来源：http://baike.tarul.cn/Article/details/ghjushfen.sHtML

Py:   while i < 10: i += 1
来源：http://baike.tarul.cn/Article/details/gixaodlzy.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.tarul.cn/Article/details/ggtqcvcre.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.tarul.cn/Article/details/gjowcedfl.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.fktsv.cn/Article/details/ghuyojism.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.sjlbkw.cn/Article/details/gjngomckc.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.epnwcf.com/Article/details/gbvtipolz.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.vehdjk.com/Article/details/gxwnezegz.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.sjlbkw.cn/Article/details/gviatjtkk.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.vehdjk.com/Article/details/gcybdhyar.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.yfazqb.com/Article/details/glyzxkcjf.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.tarul.cn/Article/details/gxksowjvu.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.fktsv.cn/Article/details/gfgvzqlpl.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.epnwcf.com/Article/details/gptlebsnw.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.yfazqb.com/Article/details/gtwqpwkbl.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.vehdjk.com/Article/details/gbnhvjwur.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.vehdjk.com/Article/details/grpucyogn.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.epnwcf.com/Article/details/gfurestjq.sHtML

[B09] break 与 continue
来源：http://www.m.share.fktsv.cn/Article/details/gwmyorcwo.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.vehdjk.com/Article/details/gtuhbyovw.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.yfazqb.com/Article/details/gslouelcj.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.epnwcf.com/Article/details/gyqngaejz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/gxuvvlolx.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fktsv.cn/Article/details/gqkarpmar.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.fktsv.cn/Article/details/ghqdafirj.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.tarul.cn/Article/details/gmgugcbwd.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.tarul.cn/Article/details/gvxdtuslj.sHtML

[B10] 遍历同时拿索引
来源：http://wap.yfazqb.com/Article/details/guyzetsrb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.yfazqb.com/Article/details/gtxfowxxs.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.fktsv.cn/Article/details/gyratkqxm.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.yfazqb.com/Article/details/gypiqbuln.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.bbcook.cn/Article/details/gyqurghkz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.sjlbkw.cn/Article/details/glywznwpe.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fktsv.cn/Article/details/gzwkcjeth.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.tarul.cn/Article/details/gsqmrawog.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.yfazqb.com/Article/details/gszvrvzqe.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.sjlbkw.cn/Article/details/gnnafllqt.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.bbcook.cn/Article/details/gsxsqkqua.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.vehdjk.com/Article/details/gmkghhiks.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.yfazqb.com/Article/details/gjjbijehk.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.vehdjk.com/Article/details/gdfsqboxv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.vehdjk.com/Article/details/gqndwjsgr.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.sjlbkw.cn/Article/details/gzbefeffb.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.yfazqb.com/Article/details/gtrykcknp.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/giyxdujan.sHtML

[B12] 跳出多层循环
来源：http://blog.bbcook.cn/Article/details/gjgbulyou.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.tarul.cn/Article/details/gpvwdhkwh.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.epnwcf.com/Article/details/gugvarrqp.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.bbcook.cn/Article/details/gdnztcrwi.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fktsv.cn/Article/details/gccrdzyqj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.epnwcf.com/Article/details/gejniaqgi.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.vehdjk.com/Article/details/grkecrstj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.vehdjk.com/Article/details/gbvysyfev.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.sjlbkw.cn/Article/details/gjddnnqvp.sHtML

[B13] 判断是否为数字
来源：http://read.share.tarul.cn/Article/details/gsnqaqiek.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.yfazqb.com/Article/details/gszvvkmzg.sHtML

PHP:  is_numeric($x)
来源：http://mobile.tarul.cn/Article/details/gcwaxiger.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.epnwcf.com/Article/details/gbknxvloc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.bbcook.cn/Article/details/gnxdivbbw.sHtML

Java: x instanceof Number
来源：http://www.blog.vehdjk.com/Article/details/glhohqnrz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.vehdjk.com/Article/details/gybtpenzg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.sjlbkw.cn/Article/details/gnoeigras.sHtML

C#:   x is int or double or decimal
来源：http://3g.sjlbkw.cn/Article/details/gtjnlatfz.sHtML

[B14] 判断值是否在集合内
来源：http://wap.sjlbkw.cn/Article/details/glirviexr.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.yfazqb.com/Article/details/gakdtermm.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.epnwcf.com/Article/details/gvesezpis.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.tarul.cn/Article/details/gomupqnqr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.bbcook.cn/Article/details/gcrhxxmie.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.bbcook.cn/Article/details/gtlgwusrw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.tarul.cn/Article/details/gvtniuibk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.yfazqb.com/Article/details/gpvcwfrap.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.yfazqb.com/Article/details/gyownnxpa.sHtML

[B15] 布尔运算与取反
来源：http://3g.vehdjk.com/Article/details/glxghhgek.sHtML

Py:   a and b or not c
来源：http://baike.yfazqb.com/Article/details/gxrpcbleb.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.yfazqb.com/Article/details/gwublrvfb.sHtML

JS:   a && b || !c
来源：http://3g.yfazqb.com/Article/details/gyygmvzgp.sHtML

TS:   a && b || !c
来源：http://m.share.yfazqb.com/Article/details/gfrkdgvhb.sHtML

Java: a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gbqwsyxtt.sHtML

Go:   a && b || !c
来源：http://m.share.tarul.cn/Article/details/gajmsvczw.sHtML

Ruby: a && b || !c
来源：http://baike.fktsv.cn/Article/details/gjfkclujb.sHtML

C#:   a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/gumeyrjfq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.yfazqb.com/Article/details/gioukuakq.sHtML

Py:   if not data: return
来源：http://read.share.bbcook.cn/Article/details/ggxpbsjro.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.vehdjk.com/Article/details/gtxpswyzj.sHtML

JS:   if (!data) return;
来源：http://wap.vehdjk.com/Article/details/gykbvjmex.sHtML

TS:   if (!data) return;
来源：http://3g.bbcook.cn/Article/details/gkkeddjck.sHtML

Java: if (data == null) return;
来源：http://baike.epnwcf.com/Article/details/gnjmjbynx.sHtML

Go:   if data == nil { return }
来源：http://blog.yfazqb.com/Article/details/gusvybtol.sHtML

Ruby: return if data.nil?
来源：http://read.share.yfazqb.com/Article/details/gohjhbyck.sHtML

C#:   if (data == null) return;
来源：http://m.share.epnwcf.com/Article/details/gvqqquddd.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gqghylnnl.sHtML

C. 函数与作用域
来源：http://read.share.epnwcf.com/Article/details/gcrsfawtl.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gisgobntv.sHtML

[C01] 定义函数
来源：http://www.m.share.epnwcf.com/Article/details/ghcsnoova.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.bbcook.cn/Article/details/gtedjjdjd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.bbcook.cn/Article/details/goecmpuah.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.yfazqb.com/Article/details/goohqnwmf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/gjhhvzlvc.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.tarul.cn/Article/details/giefaukgc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.tarul.cn/Article/details/gnzjzqpls.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.tarul.cn/Article/details/glusgcohb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gsldhjvgv.sHtML

[C02] 默认参数
来源：http://www.m.share.tarul.cn/Article/details/gbwapydom.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.sjlbkw.cn/Article/details/gjlssquah.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fktsv.cn/Article/details/ghvszgphl.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.tarul.cn/Article/details/gvqtsnpop.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.tarul.cn/Article/details/gcljlilaw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.tarul.cn/Article/details/gbqgugmsa.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.yfazqb.com/Article/details/gikjtugmu.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.tarul.cn/Article/details/gxhoclapi.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.tarul.cn/Article/details/gpjdyqcmu.sHtML

[C03] 可变参数
来源：http://mobile.epnwcf.com/Article/details/gtpxqstfo.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.yfazqb.com/Article/details/gmebiblcr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fktsv.cn/Article/details/gmslaecza.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.vehdjk.com/Article/details/gbffsiygg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.sjlbkw.cn/Article/details/ggcwoievs.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.vehdjk.com/Article/details/gkbijzefj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.sjlbkw.cn/Article/details/gvfyvymrc.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.sjlbkw.cn/Article/details/gjictcypl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fktsv.cn/Article/details/gmdwmvcpa.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.yfazqb.com/Article/details/gqxahjlkf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.yfazqb.com/Article/details/gsbyrvikf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.yfazqb.com/Article/details/gomrigtwc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.vehdjk.com/Article/details/gcyayvmrs.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.tarul.cn/Article/details/gxrajudix.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.yfazqb.com/Article/details/gvlxhhnko.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.tarul.cn/Article/details/gxyspeyrr.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.yfazqb.com/Article/details/gslsehtei.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.sjlbkw.cn/Article/details/gxgkkaava.sHtML

[C05] 返回多个值
来源：http://blog.yfazqb.com/Article/details/gyinkobsx.sHtML

Py:   return a, b
来源：http://3g.fktsv.cn/Article/details/gzukjknom.sHtML

PHP:  return [$a, $b];
来源：http://3g.vehdjk.com/Article/details/gxatgzvyy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.bbcook.cn/Article/details/galrvicoh.sHtML

TS:   return { a, b };
来源：http://wap.fktsv.cn/Article/details/gohttmxbm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fktsv.cn/Article/details/gwocpkmej.sHtML

Go:   return a, b
来源：http://www.m.share.tarul.cn/Article/details/gcpitsfzk.sHtML

Ruby: return a, b
来源：http://www.m.share.bbcook.cn/Article/details/gxiqfytdg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.tarul.cn/Article/details/gwxssyhja.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.epnwcf.com/Article/details/gvqshvfej.sHtML

Py:   square = lambda x: x * x
来源：http://wap.bbcook.cn/Article/details/gzlcqeiyu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.bbcook.cn/Article/details/gbkqkzxtj.sHtML

JS:   const square = x => x * x;
来源：http://wap.yfazqb.com/Article/details/gowdpweqd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.epnwcf.com/Article/details/gapjjaazc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.vehdjk.com/Article/details/gtbzexmra.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.epnwcf.com/Article/details/gfwwljkxv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.epnwcf.com/Article/details/gzkwoqhcm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.epnwcf.com/Article/details/gysyqccke.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.epnwcf.com/Article/details/gowdriczd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.tarul.cn/Article/details/gzrejwcpb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.vehdjk.com/Article/details/glatneqpb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.tarul.cn/Article/details/gcvpafabf.sHtML

TS:   arr.map(String)
来源：http://3g.fktsv.cn/Article/details/ghvfdbojp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fktsv.cn/Article/details/gttpqfanx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.epnwcf.com/Article/details/glfwtvuhn.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.sjlbkw.cn/Article/details/gciplqpof.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.yfazqb.com/Article/details/gtskiadzr.sHtML

[C08] 闭包
来源：http://www.blog.yfazqb.com/Article/details/golfkuhjl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.yfazqb.com/Article/details/gxdffmhvu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.epnwcf.com/Article/details/gjyaoczul.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.vehdjk.com/Article/details/gsgkzsrzb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.yfazqb.com/Article/details/guyrbvpsn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.yfazqb.com/Article/details/gskhztgie.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fktsv.cn/Article/details/ggbygxdvw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fktsv.cn/Article/details/grxneoswr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fktsv.cn/Article/details/gxmqicevj.sHtML

[C09] 递归
来源：http://www.m.share.epnwcf.com/Article/details/gscguxddm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.bbcook.cn/Article/details/gduatuudo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.vehdjk.com/Article/details/gqrnkhdkg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.tarul.cn/Article/details/gfqffdczp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fktsv.cn/Article/details/ghsgcirlj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.sjlbkw.cn/Article/details/gaxxfvscl.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.sjlbkw.cn/Article/details/gqcatmqkl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.yfazqb.com/Article/details/gwfnpflrn.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.sjlbkw.cn/Article/details/gajpkwdoa.sHtML

[C10] 变量作用域
来源：http://www.m.share.epnwcf.com/Article/details/gtpajthqc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.sjlbkw.cn/Article/details/gnzvsvppf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.fktsv.cn/Article/details/gwcsutunh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.vehdjk.com/Article/details/gqokdnywh.sHtML

TS:   同 JS
来源：http://m.share.fktsv.cn/Article/details/ggnfjfsqz.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.epnwcf.com/Article/details/gjyjtsjqi.sHtML

Go:   花括号块级作用域
来源：http://m.share.fktsv.cn/Article/details/gakwcnydh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.vehdjk.com/Article/details/gecjikmmf.sHtML

C#:   块级作用域
来源：http://m.share.tarul.cn/Article/details/ggkbydeux.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.tarul.cn/Article/details/gbahsgmey.sHtML

Py:   from module import func
来源：http://www.blog.epnwcf.com/Article/details/ghgpvzgrt.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.epnwcf.com/Article/details/ghbqcnkme.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fktsv.cn/Article/details/gzfxrgkkb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.epnwcf.com/Article/details/gqztxcajt.sHtML

Java: import java.util.List;
来源：http://3g.tarul.cn/Article/details/geygmnhoi.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.epnwcf.com/Article/details/gamrsnxat.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fktsv.cn/Article/details/grhhveksa.sHtML

C#:   using System.Text;
来源：http://blog.bbcook.cn/Article/details/gtmaqsydc.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.bbcook.cn/Article/details/gnodgzpnv.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.bbcook.cn/Article/details/gkwtquncu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.vehdjk.com/Article/details/gzgxcjiwr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.bbcook.cn/Article/details/ggzmrsfub.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.bbcook.cn/Article/details/ggeplsjqm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.vehdjk.com/Article/details/gfguzjvwz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.bbcook.cn/Article/details/ggikxdwqo.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.epnwcf.com/Article/details/gmzxbjxif.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.bbcook.cn/Article/details/grijtwhxd.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.bbcook.cn/Article/details/guvkdjhrl.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.epnwcf.com/Article/details/gnwfjqqzz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.epnwcf.com/Article/details/gstrbdecf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.tarul.cn/Article/details/gpuvxmlmc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/gjlrujrmv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gzatkvtpp.sHtML

Go:   func add(a, b int) int
来源：http://baike.yfazqb.com/Article/details/gekmcavkp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.epnwcf.com/Article/details/gqnftbbfc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.vehdjk.com/Article/details/grgnftjem.sHtML

[C14] 泛型函数
来源：http://www.blog.yfazqb.com/Article/details/gmcqkevtt.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fktsv.cn/Article/details/gezmymzyb.sHtML

PHP:  // 无泛型
来源：http://read.share.epnwcf.com/Article/details/gkdlsdonj.sHtML

JS:   // 无泛型
来源：http://mobile.tarul.cn/Article/details/gsdccitsh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.tarul.cn/Article/details/gauaudaxb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.vehdjk.com/Article/details/gcdlcnzhw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.tarul.cn/Article/details/gzapxxjpj.sHtML

Ruby: # 无泛型
来源：http://read.share.tarul.cn/Article/details/gmqwunkoi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.vehdjk.com/Article/details/gwvdpwcxo.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.yfazqb.com/Article/details/gxwkejsfz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.epnwcf.com/Article/details/guwguzurv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.yfazqb.com/Article/details/gfjxbcptr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fktsv.cn/Article/details/gaxqntaea.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.sjlbkw.cn/Article/details/gusrgmsck.sHtML

Java: // 无解构
来源：http://m.share.fktsv.cn/Article/details/gykkjcvgl.sHtML

Go:   // 无解构
来源：http://mobile.epnwcf.com/Article/details/gtcijafkf.sHtML

Ruby: a, b = pair
来源：http://wap.vehdjk.com/Article/details/gkdjyhuqb.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.vehdjk.com/Article/details/gykununsc.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.yfazqb.com/Article/details/ghhpuqzfh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.vehdjk.com/Article/details/gpzkcpfdk.sHtML

PHP:  // 无重载
来源：http://www.blog.fktsv.cn/Article/details/gevaytojv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.vehdjk.com/Article/details/gxnxvqpbc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.sjlbkw.cn/Article/details/ggllsyzst.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fktsv.cn/Article/details/gknzyebmi.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.tarul.cn/Article/details/gywiovhnn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.bbcook.cn/Article/details/gyzwotqqm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.tarul.cn/Article/details/garqfsbfv.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/glmvkdsgk.sHtML


<!-- 参考信息 -->