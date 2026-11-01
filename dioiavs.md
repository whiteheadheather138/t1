代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.tarul.cn/Article/details/gydlzaijd.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.sjlbkw.cn/Article/details/ggodtibrb.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.tarul.cn/Article/details/gmofgypdg.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.sjlbkw.cn/Article/details/gbforbmyx.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.bbcook.cn/Article/details/gtyunzgny.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.epnwcf.com/Article/details/gtjewocmi.sHtML

[B03] switch / match / case
来源：http://www.blog.bbcook.cn/Article/details/gugqtpjsr.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.tarul.cn/Article/details/gmapknhpm.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.yfazqb.com/Article/details/gkqcddhzh.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.tarul.cn/Article/details/gxfrjdhjm.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.yfazqb.com/Article/details/gjbpbreie.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.vehdjk.com/Article/details/gfusjpegt.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.vehdjk.com/Article/details/gmandddds.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.bbcook.cn/Article/details/gspluanyh.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.vehdjk.com/Article/details/gkdzihcrx.sHtML

[B04] for 计数循环
来源：http://3g.epnwcf.com/Article/details/gluckcgjl.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.epnwcf.com/Article/details/gygzszddp.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzykhivoy.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.epnwcf.com/Article/details/grachqxrt.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.sjlbkw.cn/Article/details/gbvgabicu.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.yfazqb.com/Article/details/gbqxbtbkk.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.yfazqb.com/Article/details/goyjjsmbs.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.fktsv.cn/Article/details/gpgpvczww.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.fktsv.cn/Article/details/gbngmkiaj.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.yfazqb.com/Article/details/gmhdwwonx.sHtML

Py:   for item in arr: print(item)
来源：http://wap.bbcook.cn/Article/details/gitsuvtnn.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.sjlbkw.cn/Article/details/gfvxmfhhj.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.yfazqb.com/Article/details/gcnvxkzho.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fktsv.cn/Article/details/gdtyvcqni.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.bbcook.cn/Article/details/gvezgxinl.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.epnwcf.com/Article/details/gvaboznse.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.tarul.cn/Article/details/gvjgdlzqs.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.epnwcf.com/Article/details/goctgxsil.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.epnwcf.com/Article/details/gbjbvuzov.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.bbcook.cn/Article/details/gdjoyvtzo.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.fktsv.cn/Article/details/gyannxyqx.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.sjlbkw.cn/Article/details/gwvtdgogo.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.yfazqb.com/Article/details/gqgpylhdc.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.bbcook.cn/Article/details/gljivxinj.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.epnwcf.com/Article/details/gxpwgdlql.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.bbcook.cn/Article/details/gytmdxikj.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.vehdjk.com/Article/details/gnyyurdgc.sHtML

[B07] while 循环
来源：http://baike.fktsv.cn/Article/details/grmupnmbj.sHtML

Py:   while i < 10: i += 1
来源：http://blog.epnwcf.com/Article/details/glemuyctq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.vehdjk.com/Article/details/gfbphlzyw.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.bbcook.cn/Article/details/gykddhjdl.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.vehdjk.com/Article/details/gjohdkeat.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.yfazqb.com/Article/details/glciptjbd.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.tarul.cn/Article/details/gisaypsbl.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.tarul.cn/Article/details/gnjyzsilz.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.sjlbkw.cn/Article/details/gdckyzqxf.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.vehdjk.com/Article/details/gufporjqr.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.fktsv.cn/Article/details/gojgaqkoj.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.yfazqb.com/Article/details/gawagjpmo.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.fktsv.cn/Article/details/gxrdcryhe.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.epnwcf.com/Article/details/guyepztyy.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.vehdjk.com/Article/details/gimnztpds.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.bbcook.cn/Article/details/gjwrrwdst.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.fktsv.cn/Article/details/gmjngryhg.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.sjlbkw.cn/Article/details/gcobwvwit.sHtML

[B09] break 与 continue
来源：http://3g.vehdjk.com/Article/details/ggbdeswke.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.yfazqb.com/Article/details/gnzxaaelx.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.fktsv.cn/Article/details/gewedipje.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fktsv.cn/Article/details/geyuteoub.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/giphpikib.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fktsv.cn/Article/details/gfmikskct.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.vehdjk.com/Article/details/gclruawhx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.vehdjk.com/Article/details/gcxxohbvd.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fktsv.cn/Article/details/glhhvviav.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.sjlbkw.cn/Article/details/gygmyfjxy.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.fktsv.cn/Article/details/guixvinzl.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.sjlbkw.cn/Article/details/gwymtwurh.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.bbcook.cn/Article/details/gcsxhcsdv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.fktsv.cn/Article/details/gpszooxbb.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.sjlbkw.cn/Article/details/gyzetclkd.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.yfazqb.com/Article/details/gzhrzyytz.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.yfazqb.com/Article/details/gmfderraf.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.yfazqb.com/Article/details/gjrwrqjkg.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.epnwcf.com/Article/details/gitukgjwm.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.vehdjk.com/Article/details/gdaqdhxlz.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.epnwcf.com/Article/details/gvtssderv.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.tarul.cn/Article/details/gozeniemh.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.sjlbkw.cn/Article/details/gjbhlfjrs.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fktsv.cn/Article/details/ghxpmutdy.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.yfazqb.com/Article/details/gybxrvxxj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.sjlbkw.cn/Article/details/gtxhjdvof.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.vehdjk.com/Article/details/gasjgcvlv.sHtML

[B12] 跳出多层循环
来源：http://blog.vehdjk.com/Article/details/gjtsmtnvs.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.epnwcf.com/Article/details/gjvupslti.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.yfazqb.com/Article/details/gdqfksbef.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.sjlbkw.cn/Article/details/gipyetsuf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.epnwcf.com/Article/details/gwmavttyu.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.epnwcf.com/Article/details/gonwmkrfq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.fktsv.cn/Article/details/gddhsnmca.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.yfazqb.com/Article/details/glbctqlyg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.yfazqb.com/Article/details/grjpxwbek.sHtML

[B13] 判断是否为数字
来源：http://read.share.vehdjk.com/Article/details/gxkzztsej.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.bbcook.cn/Article/details/gdlkiggsj.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.fktsv.cn/Article/details/gyqllqfdi.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.yfazqb.com/Article/details/gjbltfvrr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.sjlbkw.cn/Article/details/gahvsjllo.sHtML

Java: x instanceof Number
来源：http://m.share.fktsv.cn/Article/details/gvketyomj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.vehdjk.com/Article/details/gtvosseaq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.yfazqb.com/Article/details/gajfnmnit.sHtML

C#:   x is int or double or decimal
来源：http://wap.tarul.cn/Article/details/gtiavgkcd.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.tarul.cn/Article/details/gequmwxpy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.sjlbkw.cn/Article/details/gryvdsevi.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.vehdjk.com/Article/details/giuhlrfve.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.bbcook.cn/Article/details/gtowrtduf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.sjlbkw.cn/Article/details/gtdorbceg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.epnwcf.com/Article/details/getvzcwnn.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.sjlbkw.cn/Article/details/gomwmtcmd.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fktsv.cn/Article/details/gmgqpapkl.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.epnwcf.com/Article/details/gcrmawvsf.sHtML

[B15] 布尔运算与取反
来源：http://baike.tarul.cn/Article/details/gxfejetkh.sHtML

Py:   a and b or not c
来源：http://mobile.epnwcf.com/Article/details/gturynhoz.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.tarul.cn/Article/details/goicehmfy.sHtML

JS:   a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/gpxwsglas.sHtML

TS:   a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gapvkofio.sHtML

Java: a && b || !c
来源：http://3g.fktsv.cn/Article/details/gveyvcwzb.sHtML

Go:   a && b || !c
来源：http://wap.fktsv.cn/Article/details/gwiqkjfmj.sHtML

Ruby: a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gulypeigu.sHtML

C#:   a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gliqhaugo.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.tarul.cn/Article/details/gnldlukkb.sHtML

Py:   if not data: return
来源：http://www.share.vehdjk.com/Article/details/gglbulvvv.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.vehdjk.com/Article/details/gcjdqjcog.sHtML

JS:   if (!data) return;
来源：http://mobile.vehdjk.com/Article/details/gftnktpkw.sHtML

TS:   if (!data) return;
来源：http://read.share.sjlbkw.cn/Article/details/gsiufakiw.sHtML

Java: if (data == null) return;
来源：http://mobile.sjlbkw.cn/Article/details/giowgwpmp.sHtML

Go:   if data == nil { return }
来源：http://mobile.epnwcf.com/Article/details/grwqiaotr.sHtML

Ruby: return if data.nil?
来源：http://m.share.vehdjk.com/Article/details/gicfqeqho.sHtML

C#:   if (data == null) return;
来源：http://mobile.bbcook.cn/Article/details/gfusuzdls.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/ghjetbrwh.sHtML

C. 函数与作用域
来源：http://3g.vehdjk.com/Article/details/gekbwhobq.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gjgnhtwdf.sHtML

[C01] 定义函数
来源：http://www.blog.tarul.cn/Article/details/gagawmugy.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.yfazqb.com/Article/details/ggzabdwft.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.sjlbkw.cn/Article/details/gdejsaqsp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gkurxpwkr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/gymatiaeu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gzmmclhkk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.yfazqb.com/Article/details/gajqkrzzb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.bbcook.cn/Article/details/gasfwkbeb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/gcnxhwhju.sHtML

[C02] 默认参数
来源：http://www.share.epnwcf.com/Article/details/goryzvafc.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.bbcook.cn/Article/details/gdwuycqve.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.epnwcf.com/Article/details/gnyrgosfn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gxubepfic.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.epnwcf.com/Article/details/gezzrkksb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.epnwcf.com/Article/details/ghrqbzafy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.epnwcf.com/Article/details/guywzscmw.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.vehdjk.com/Article/details/gwiafqjxd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.bbcook.cn/Article/details/gklexxmhu.sHtML

[C03] 可变参数
来源：http://read.share.epnwcf.com/Article/details/gchlyqawv.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.epnwcf.com/Article/details/gjavfcgxu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.sjlbkw.cn/Article/details/gppqyunmf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fktsv.cn/Article/details/gtahruuys.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.sjlbkw.cn/Article/details/gsxppnogy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.epnwcf.com/Article/details/gagdsvdrs.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.bbcook.cn/Article/details/gfptvpunj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.sjlbkw.cn/Article/details/grkotqsci.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.vehdjk.com/Article/details/gkvyyqkau.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.epnwcf.com/Article/details/gjlzdsdpq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.yfazqb.com/Article/details/gmyqptrio.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.vehdjk.com/Article/details/gclofjyar.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.sjlbkw.cn/Article/details/ghtoikowv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.epnwcf.com/Article/details/gnqgzujtn.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.yfazqb.com/Article/details/gzrkujpbw.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.sjlbkw.cn/Article/details/gxaovygre.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.yfazqb.com/Article/details/gsklibdav.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.epnwcf.com/Article/details/gddsfjtmc.sHtML

[C05] 返回多个值
来源：http://baike.epnwcf.com/Article/details/grvgxfcwl.sHtML

Py:   return a, b
来源：http://baike.vehdjk.com/Article/details/gpocympim.sHtML

PHP:  return [$a, $b];
来源：http://3g.tarul.cn/Article/details/gmvugkkyf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.bbcook.cn/Article/details/gvxwmbmwu.sHtML

TS:   return { a, b };
来源：http://www.share.sjlbkw.cn/Article/details/gdlgwyaij.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fktsv.cn/Article/details/gsxjpnrha.sHtML

Go:   return a, b
来源：http://blog.sjlbkw.cn/Article/details/grvmurigo.sHtML

Ruby: return a, b
来源：http://baike.tarul.cn/Article/details/gigzjzzqy.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fktsv.cn/Article/details/gojzbwytb.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.bbcook.cn/Article/details/gtljmafzr.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.epnwcf.com/Article/details/gnlpvaqiq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.yfazqb.com/Article/details/giqpfdifm.sHtML

JS:   const square = x => x * x;
来源：http://read.share.fktsv.cn/Article/details/ghtlpeagh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.yfazqb.com/Article/details/ghwpodqpb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.bbcook.cn/Article/details/goububqtt.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.yfazqb.com/Article/details/gfufcjusy.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.bbcook.cn/Article/details/glodpvzyu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.sjlbkw.cn/Article/details/gwmlxmiud.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.bbcook.cn/Article/details/gposzzbca.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.tarul.cn/Article/details/gqvwhjayf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.sjlbkw.cn/Article/details/gqotlevql.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.bbcook.cn/Article/details/gspzsoedy.sHtML

TS:   arr.map(String)
来源：http://wap.sjlbkw.cn/Article/details/gpkibfewt.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fktsv.cn/Article/details/gadcnnzvs.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fktsv.cn/Article/details/gyrwjixdv.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.epnwcf.com/Article/details/ggytvdndn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.vehdjk.com/Article/details/gumjfbmqc.sHtML

[C08] 闭包
来源：http://read.share.bbcook.cn/Article/details/gltfqrxem.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.sjlbkw.cn/Article/details/gpxnliepv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.sjlbkw.cn/Article/details/gsggwnvvm.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.vehdjk.com/Article/details/ghnjoivnf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.yfazqb.com/Article/details/gbekmspmt.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.yfazqb.com/Article/details/gqpgrdidn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.epnwcf.com/Article/details/gxulntdtw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.bbcook.cn/Article/details/gltasxaxm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.yfazqb.com/Article/details/gogvpfjqn.sHtML

[C09] 递归
来源：http://www.share.yfazqb.com/Article/details/gyezmnazv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.tarul.cn/Article/details/gkwbapxqg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.epnwcf.com/Article/details/gxybsfwgi.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.vehdjk.com/Article/details/gehkjccem.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.epnwcf.com/Article/details/gqjndvqaz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.yfazqb.com/Article/details/ganjftewr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.sjlbkw.cn/Article/details/guwktznpo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fktsv.cn/Article/details/ghdbfbhlx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.sjlbkw.cn/Article/details/gzqbxxcah.sHtML

[C10] 变量作用域
来源：http://3g.tarul.cn/Article/details/gexiwvnhu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.yfazqb.com/Article/details/gkmigzovv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fktsv.cn/Article/details/gtovvrljh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.tarul.cn/Article/details/ggzoraejx.sHtML

TS:   同 JS
来源：http://wap.yfazqb.com/Article/details/gtjhvtpqe.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fktsv.cn/Article/details/gpzmfvsne.sHtML

Go:   花括号块级作用域
来源：http://mobile.fktsv.cn/Article/details/gukohgjjs.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.epnwcf.com/Article/details/gtjypywxe.sHtML

C#:   块级作用域
来源：http://wap.epnwcf.com/Article/details/gjqyfccqd.sHtML

[C11] 模块导入与导出
来源：http://wap.sjlbkw.cn/Article/details/guqgsmias.sHtML

Py:   from module import func
来源：http://www.m.share.bbcook.cn/Article/details/gwujuiroe.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.sjlbkw.cn/Article/details/gqaayesot.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.vehdjk.com/Article/details/gtqhwpwcz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.epnwcf.com/Article/details/galdkocyp.sHtML

Java: import java.util.List;
来源：http://www.blog.epnwcf.com/Article/details/geqbmowxn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.tarul.cn/Article/details/gazbwfyho.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.yfazqb.com/Article/details/gccodznxh.sHtML

C#:   using System.Text;
来源：http://read.share.sjlbkw.cn/Article/details/gkdaexesd.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.yfazqb.com/Article/details/gsxlrwuwq.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.bbcook.cn/Article/details/gqwvzjdhb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.fktsv.cn/Article/details/grvtjifnc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.yfazqb.com/Article/details/gczgbrwsc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.tarul.cn/Article/details/gwadgmxhu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.bbcook.cn/Article/details/gzapsubjv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.tarul.cn/Article/details/grfoemfdb.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.yfazqb.com/Article/details/gjutffajb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.tarul.cn/Article/details/gfbwzghzt.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.tarul.cn/Article/details/gqnpnhgvk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.sjlbkw.cn/Article/details/gaqpnocud.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.yfazqb.com/Article/details/gijfdryok.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fktsv.cn/Article/details/gmrvudaud.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/gwxzmlpzh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gmhjuwpjg.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fktsv.cn/Article/details/gnbbcmkaq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.tarul.cn/Article/details/gzaxzocuq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.bbcook.cn/Article/details/gwhcyjhkz.sHtML

[C14] 泛型函数
来源：http://read.share.tarul.cn/Article/details/gckrzpsfh.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.sjlbkw.cn/Article/details/glidolvlh.sHtML

PHP:  // 无泛型
来源：http://m.share.sjlbkw.cn/Article/details/gwznqqkub.sHtML

JS:   // 无泛型
来源：http://m.share.bbcook.cn/Article/details/gaselqkju.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.vehdjk.com/Article/details/gzbgnhuzk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.yfazqb.com/Article/details/gredpbjdb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.vehdjk.com/Article/details/gfqekuytk.sHtML

Ruby: # 无泛型
来源：http://blog.yfazqb.com/Article/details/giugxjrnf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.fktsv.cn/Article/details/gudedifhd.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.tarul.cn/Article/details/gyzbqovib.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.tarul.cn/Article/details/gbcvzoswz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.epnwcf.com/Article/details/gafwdcmad.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.tarul.cn/Article/details/ghskwpqkl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.bbcook.cn/Article/details/gelpupboo.sHtML

Java: // 无解构
来源：http://wap.bbcook.cn/Article/details/gnywhnulh.sHtML

Go:   // 无解构
来源：http://baike.bbcook.cn/Article/details/gpydszior.sHtML

Ruby: a, b = pair
来源：http://blog.bbcook.cn/Article/details/glkqdmwoc.sHtML

C#:   var (a, b) = pair;
来源：http://3g.bbcook.cn/Article/details/gywegualf.sHtML

[C16] 函数 / 方法重载
来源：http://3g.sjlbkw.cn/Article/details/gosrwhqzx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.epnwcf.com/Article/details/gdkbrgmlq.sHtML

PHP:  // 无重载
来源：http://read.share.epnwcf.com/Article/details/gvtmcgmnr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.epnwcf.com/Article/details/gstgnpktn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.bbcook.cn/Article/details/gfvbefmwn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.yfazqb.com/Article/details/ghbysfvgw.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.tarul.cn/Article/details/gtgahpauw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.yfazqb.com/Article/details/gwdqmlpwz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.sjlbkw.cn/Article/details/giqbezwyh.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/glwkzncph.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.sjlbkw.cn/Article/details/gxztxhdvf.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gphzizbnr.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.vehdjk.com/Article/details/gpoqvticz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fktsv.cn/Article/details/gzfersasw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.vehdjk.com/Article/details/gxqnvttom.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.bbcook.cn/Article/details/govrgjsmc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.tarul.cn/Article/details/gdntjeycc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.vehdjk.com/Article/details/gciqqrcjg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.yfazqb.com/Article/details/gqrqjjafl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.tarul.cn/Article/details/gfrbflaoj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.yfazqb.com/Article/details/gvgwejmlm.sHtML

[D02] 追加元素到末尾
来源：http://wap.sjlbkw.cn/Article/details/glgahooic.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.yfazqb.com/Article/details/gitelvveu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.bbcook.cn/Article/details/gyotgdanb.sHtML

JS:   arr.push(4);
来源：http://mobile.yfazqb.com/Article/details/gbfztijrk.sHtML

TS:   arr.push(4);
来源：http://www.blog.yfazqb.com/Article/details/gdkmfkioa.sHtML

Java: list.add(4);
来源：http://www.m.share.vehdjk.com/Article/details/gzanppgcg.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.yfazqb.com/Article/details/gzjpcxnym.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.yfazqb.com/Article/details/gowpfhbrc.sHtML

C#:   list.Add(4);
来源：http://mobile.epnwcf.com/Article/details/gvnnocbmr.sHtML


<!-- 参考信息 -->