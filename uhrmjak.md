代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.tarul.cn/Article/details/guymrofif.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.vehdjk.com/Article/details/gkyzdnnzl.sHtML

[B03] switch / match / case
来源：http://www.blog.tarul.cn/Article/details/gehdgbhbc.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.bbcook.cn/Article/details/ggvxdutuy.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.sjlbkw.cn/Article/details/gkpzxbclx.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.yfazqb.com/Article/details/gvbsgjxgm.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.yfazqb.com/Article/details/gxekwdidi.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.epnwcf.com/Article/details/gnjtpvwyt.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.yfazqb.com/Article/details/glmmfixom.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.sjlbkw.cn/Article/details/gfbpybbzn.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.epnwcf.com/Article/details/gczkizvth.sHtML

[B04] for 计数循环
来源：http://wap.fktsv.cn/Article/details/gxhimonvo.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.yfazqb.com/Article/details/gevluotao.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.yfazqb.com/Article/details/gxpsuowye.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.vehdjk.com/Article/details/gzdfswtsc.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.sjlbkw.cn/Article/details/ghqppjaqd.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.yfazqb.com/Article/details/gotcacnnv.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.fktsv.cn/Article/details/gtslrxivh.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.tarul.cn/Article/details/geldzzrtq.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.fktsv.cn/Article/details/gqrcnlurt.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.epnwcf.com/Article/details/gtslrkdrf.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.vehdjk.com/Article/details/guquvvjdz.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.epnwcf.com/Article/details/gklwymhdu.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fktsv.cn/Article/details/gdootuigb.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.tarul.cn/Article/details/gxtliscec.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.sjlbkw.cn/Article/details/grkgtcwub.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnhaslqtn.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.yfazqb.com/Article/details/gfopiiyql.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.epnwcf.com/Article/details/gfckzmvbi.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.sjlbkw.cn/Article/details/gdluvbdey.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.fktsv.cn/Article/details/gmxpwydwf.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gvdjrylzj.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.tarul.cn/Article/details/gakmaokor.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.yfazqb.com/Article/details/gnlfcteii.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.sjlbkw.cn/Article/details/gobftcyhx.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.sjlbkw.cn/Article/details/giccfwqbk.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.yfazqb.com/Article/details/gfimgoiya.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.epnwcf.com/Article/details/gwvvyelha.sHtML

[B07] while 循环
来源：http://read.share.sjlbkw.cn/Article/details/gorayhxyo.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.vehdjk.com/Article/details/geprkvkah.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.yfazqb.com/Article/details/ghhubimqt.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.tarul.cn/Article/details/grfqbkpfx.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.vehdjk.com/Article/details/gsbnhijlh.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.bbcook.cn/Article/details/gfahqmmjw.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.epnwcf.com/Article/details/gnvuwkgdd.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.epnwcf.com/Article/details/ggwemwboc.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.epnwcf.com/Article/details/gcbzynzlx.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.epnwcf.com/Article/details/ggkvtzmqu.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.sjlbkw.cn/Article/details/gscbnrmus.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.bbcook.cn/Article/details/gorbvzaln.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.sjlbkw.cn/Article/details/ghpfjwprt.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.bbcook.cn/Article/details/gnnsnucmf.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.tarul.cn/Article/details/gzhjznexr.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.bbcook.cn/Article/details/gnccvmdjv.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.sjlbkw.cn/Article/details/gortnqnze.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.sjlbkw.cn/Article/details/gggtsjuie.sHtML

[B09] break 与 continue
来源：http://read.share.epnwcf.com/Article/details/ggdxgyssu.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.vehdjk.com/Article/details/gpmtewggf.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.yfazqb.com/Article/details/gcsbxveoj.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.tarul.cn/Article/details/guztbdnje.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.tarul.cn/Article/details/gvktzmtqz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.bbcook.cn/Article/details/gewivikoo.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.bbcook.cn/Article/details/gqwcslsxh.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.yfazqb.com/Article/details/gersdkpmy.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.vehdjk.com/Article/details/gbqbkymjs.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.fktsv.cn/Article/details/ggrplbxbu.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.tarul.cn/Article/details/gjtnnotzq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.epnwcf.com/Article/details/gruofpqbf.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.bbcook.cn/Article/details/gtoueeryt.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.tarul.cn/Article/details/gwkpucikf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.fktsv.cn/Article/details/gpzbezyzy.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.epnwcf.com/Article/details/glynbkrpr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.epnwcf.com/Article/details/goftxfznp.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.epnwcf.com/Article/details/grqkjqolk.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.sjlbkw.cn/Article/details/greygfjca.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.tarul.cn/Article/details/gjbprjjpp.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.tarul.cn/Article/details/gfliqdhgy.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.epnwcf.com/Article/details/gcnzospus.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.sjlbkw.cn/Article/details/gmfrijuby.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.yfazqb.com/Article/details/gzxtgmoax.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.fktsv.cn/Article/details/gvitpantc.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.sjlbkw.cn/Article/details/gyfdocmkk.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.sjlbkw.cn/Article/details/glbmwynmb.sHtML

[B12] 跳出多层循环
来源：http://www.blog.yfazqb.com/Article/details/gbomourvc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.bbcook.cn/Article/details/gwhikcnli.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.tarul.cn/Article/details/geyigsgdr.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.bbcook.cn/Article/details/glvbhatdd.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.vehdjk.com/Article/details/gdprrrmkj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.tarul.cn/Article/details/gvdotrtcg.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.vehdjk.com/Article/details/gfyxuusnh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.sjlbkw.cn/Article/details/gsceeqbzc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.yfazqb.com/Article/details/gtyennilq.sHtML

[B13] 判断是否为数字
来源：http://blog.tarul.cn/Article/details/ggjjwamjy.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.epnwcf.com/Article/details/getupxpzy.sHtML

PHP:  is_numeric($x)
来源：http://3g.sjlbkw.cn/Article/details/guacvmjzf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.sjlbkw.cn/Article/details/glnlpavnu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.vehdjk.com/Article/details/ghjhyxxac.sHtML

Java: x instanceof Number
来源：http://mobile.epnwcf.com/Article/details/gakwrwhbc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.epnwcf.com/Article/details/gbvrfptwd.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.epnwcf.com/Article/details/gehwfuzmf.sHtML

C#:   x is int or double or decimal
来源：http://3g.vehdjk.com/Article/details/goecmemmx.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.vehdjk.com/Article/details/gkejzuihs.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.sjlbkw.cn/Article/details/ghmdehndz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.bbcook.cn/Article/details/geznjjcfx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.vehdjk.com/Article/details/gmoplpvgk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.sjlbkw.cn/Article/details/gupsqvjuf.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.fktsv.cn/Article/details/gxqtqsemr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.sjlbkw.cn/Article/details/gsewdhhmk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.epnwcf.com/Article/details/gcrkedbzx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.epnwcf.com/Article/details/guklmnreq.sHtML

[B15] 布尔运算与取反
来源：http://read.share.tarul.cn/Article/details/gleqonnud.sHtML

Py:   a and b or not c
来源：http://blog.epnwcf.com/Article/details/gptxlqizl.sHtML

PHP:  $a && $b || !$c
来源：http://3g.bbcook.cn/Article/details/gnkuvdqdb.sHtML

JS:   a && b || !c
来源：http://wap.yfazqb.com/Article/details/gjrwymyxf.sHtML

TS:   a && b || !c
来源：http://www.m.share.bbcook.cn/Article/details/gxnhqglpr.sHtML

Java: a && b || !c
来源：http://wap.fktsv.cn/Article/details/gwarqpvsd.sHtML

Go:   a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gdqbcefjt.sHtML

Ruby: a && b || !c
来源：http://baike.fktsv.cn/Article/details/gnhzdfubz.sHtML

C#:   a && b || !c
来源：http://read.share.epnwcf.com/Article/details/givwiofyp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.vehdjk.com/Article/details/gqgyiuqlp.sHtML

Py:   if not data: return
来源：http://mobile.fktsv.cn/Article/details/gxihjrfak.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.epnwcf.com/Article/details/gqvufesdu.sHtML

JS:   if (!data) return;
来源：http://wap.yfazqb.com/Article/details/gkhvrpmdc.sHtML

TS:   if (!data) return;
来源：http://mobile.tarul.cn/Article/details/grcmzedqh.sHtML

Java: if (data == null) return;
来源：http://3g.sjlbkw.cn/Article/details/gmhulkoip.sHtML

Go:   if data == nil { return }
来源：http://baike.epnwcf.com/Article/details/gdxolbfcq.sHtML

Ruby: return if data.nil?
来源：http://wap.sjlbkw.cn/Article/details/gkvkkwngz.sHtML

C#:   if (data == null) return;
来源：http://mobile.vehdjk.com/Article/details/ghpdjcdcs.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gqtzkbhuo.sHtML

C. 函数与作用域
来源：http://mobile.tarul.cn/Article/details/gykfimpmw.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gfbwzkyxz.sHtML

[C01] 定义函数
来源：http://mobile.epnwcf.com/Article/details/gjiyfpbqp.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fktsv.cn/Article/details/gxzyyvfnk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fktsv.cn/Article/details/grgpgzerm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gqcnrhish.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/gphrvnine.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/gixctzord.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.epnwcf.com/Article/details/gmqwdeqin.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.tarul.cn/Article/details/ggrgaupul.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/gvrxgftdi.sHtML

[C02] 默认参数
来源：http://m.share.yfazqb.com/Article/details/gsgnqicdc.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.yfazqb.com/Article/details/gcsltahol.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.vehdjk.com/Article/details/gyefeiehn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.tarul.cn/Article/details/gpkepkdqt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/glwptgpoi.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.sjlbkw.cn/Article/details/gxwgckndg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.yfazqb.com/Article/details/gddzxefmy.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.sjlbkw.cn/Article/details/gxwyjseey.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fktsv.cn/Article/details/guhgetkjj.sHtML

[C03] 可变参数
来源：http://www.m.share.bbcook.cn/Article/details/gckyuymoe.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.epnwcf.com/Article/details/ggkcjlnxx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.yfazqb.com/Article/details/gynjulfwp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.tarul.cn/Article/details/gagesgvex.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.bbcook.cn/Article/details/gmbhbzkod.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.tarul.cn/Article/details/gdozqnvdv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.tarul.cn/Article/details/gqystelod.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.epnwcf.com/Article/details/goxqcsqcb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.bbcook.cn/Article/details/guqvzwueb.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.epnwcf.com/Article/details/gynnnahlc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.tarul.cn/Article/details/gpqghqpfh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fktsv.cn/Article/details/gomqnagau.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.yfazqb.com/Article/details/geaqjsker.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.bbcook.cn/Article/details/gdvbgrabi.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.tarul.cn/Article/details/geuuprqug.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.tarul.cn/Article/details/gpikdbgxy.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.fktsv.cn/Article/details/gavjrxwij.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.vehdjk.com/Article/details/ghyhdwiaw.sHtML

[C05] 返回多个值
来源：http://blog.epnwcf.com/Article/details/gcgvhaqse.sHtML

Py:   return a, b
来源：http://3g.vehdjk.com/Article/details/gcjedrcfs.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.sjlbkw.cn/Article/details/grccfneon.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.tarul.cn/Article/details/gjroafpzn.sHtML

TS:   return { a, b };
来源：http://read.share.yfazqb.com/Article/details/gjjqrytvs.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.epnwcf.com/Article/details/gydvawvoy.sHtML

Go:   return a, b
来源：http://read.share.epnwcf.com/Article/details/gqxpbqaiu.sHtML

Ruby: return a, b
来源：http://baike.tarul.cn/Article/details/grfeclpqg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.vehdjk.com/Article/details/gtxwbjmih.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fktsv.cn/Article/details/gykvkdsvu.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.yfazqb.com/Article/details/ghjsfktks.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.bbcook.cn/Article/details/gevtqxzco.sHtML

JS:   const square = x => x * x;
来源：http://blog.tarul.cn/Article/details/gfusriwem.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.sjlbkw.cn/Article/details/gkhizheih.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.vehdjk.com/Article/details/gdyqlslpt.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.sjlbkw.cn/Article/details/grhahbdyg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.yfazqb.com/Article/details/gcofncpzz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.sjlbkw.cn/Article/details/gxhktkldv.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.yfazqb.com/Article/details/gaxsyphee.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.sjlbkw.cn/Article/details/gixkpvuhi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fktsv.cn/Article/details/gbcbxvvtb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.bbcook.cn/Article/details/gqrcpixdk.sHtML

TS:   arr.map(String)
来源：http://www.share.fktsv.cn/Article/details/gqtdiglws.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/grtohpymz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.yfazqb.com/Article/details/ggjindlrn.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.tarul.cn/Article/details/gaylierog.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.sjlbkw.cn/Article/details/gbqbtvoxn.sHtML

[C08] 闭包
来源：http://www.m.share.tarul.cn/Article/details/gdsdowruh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.vehdjk.com/Article/details/gisupiofl.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.yfazqb.com/Article/details/gylfugihs.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.sjlbkw.cn/Article/details/gzeqmkqkz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.epnwcf.com/Article/details/gtebulrep.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.bbcook.cn/Article/details/gtmhyefwa.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.bbcook.cn/Article/details/gdmlzsvhw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.tarul.cn/Article/details/ggyyqpdgh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.sjlbkw.cn/Article/details/gpjfcqekj.sHtML

[C09] 递归
来源：http://3g.vehdjk.com/Article/details/gfycpxvla.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.epnwcf.com/Article/details/gzhefpile.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.bbcook.cn/Article/details/gcrsjozlc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.tarul.cn/Article/details/grojthtnx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.vehdjk.com/Article/details/gmsoheptm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.yfazqb.com/Article/details/gomsbulht.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.sjlbkw.cn/Article/details/ggtfqbytw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.sjlbkw.cn/Article/details/gojqdfcaa.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fktsv.cn/Article/details/gglrwwqhy.sHtML

[C10] 变量作用域
来源：http://m.share.fktsv.cn/Article/details/gpxtxjdmj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.bbcook.cn/Article/details/gsdozwihx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.tarul.cn/Article/details/gmnndmymb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.sjlbkw.cn/Article/details/gnrbaxaku.sHtML

TS:   同 JS
来源：http://www.blog.bbcook.cn/Article/details/glqervhzp.sHtML

Java: 方法内为块级作用域
来源：http://3g.bbcook.cn/Article/details/gvujxqpvd.sHtML

Go:   花括号块级作用域
来源：http://wap.fktsv.cn/Article/details/geakjijwy.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.epnwcf.com/Article/details/gmpvgsjlw.sHtML

C#:   块级作用域
来源：http://mobile.epnwcf.com/Article/details/glcjcghvt.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fktsv.cn/Article/details/gkltizaal.sHtML

Py:   from module import func
来源：http://read.share.yfazqb.com/Article/details/glrjvshjr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.sjlbkw.cn/Article/details/gszpzeihv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.bbcook.cn/Article/details/gicqnmfnp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fktsv.cn/Article/details/gzutajpsm.sHtML

Java: import java.util.List;
来源：http://www.share.bbcook.cn/Article/details/gbqrumkuf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.bbcook.cn/Article/details/gkomooskm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.bbcook.cn/Article/details/gztsmeejm.sHtML

C#:   using System.Text;
来源：http://www.share.tarul.cn/Article/details/gdjscjvnc.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.vehdjk.com/Article/details/gqvmvsmqt.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.vehdjk.com/Article/details/gwnqyekym.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.yfazqb.com/Article/details/gxgqdpjip.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.sjlbkw.cn/Article/details/glgfatowk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.yfazqb.com/Article/details/gxmrbtsez.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.tarul.cn/Article/details/gnrttomse.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.bbcook.cn/Article/details/ggfbxeycs.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.vehdjk.com/Article/details/gupwifvbf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.tarul.cn/Article/details/gkbpvfrgv.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.tarul.cn/Article/details/gcegqyfqh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.vehdjk.com/Article/details/gosslvmsy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.epnwcf.com/Article/details/gidxjcfvf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.sjlbkw.cn/Article/details/gczqxbdrf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gedpfizqi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/grybmwbqx.sHtML

Go:   func add(a, b int) int
来源：http://wap.vehdjk.com/Article/details/gqhgacrwp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.bbcook.cn/Article/details/gifcqqiyc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.epnwcf.com/Article/details/gyomoqkbr.sHtML

[C14] 泛型函数
来源：http://wap.epnwcf.com/Article/details/gareezayu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.epnwcf.com/Article/details/gzzbiullb.sHtML

PHP:  // 无泛型
来源：http://blog.sjlbkw.cn/Article/details/gchrskoen.sHtML

JS:   // 无泛型
来源：http://blog.bbcook.cn/Article/details/givepksfr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.bbcook.cn/Article/details/gadxhymop.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.yfazqb.com/Article/details/gznjkfglq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.sjlbkw.cn/Article/details/gszkbyxfr.sHtML

Ruby: # 无泛型
来源：http://baike.vehdjk.com/Article/details/gldxzoogk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fktsv.cn/Article/details/gfioumrom.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.vehdjk.com/Article/details/gjgenzuca.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.epnwcf.com/Article/details/gaojqflcr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.epnwcf.com/Article/details/gzhfqmzjz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fktsv.cn/Article/details/gwkddjmuc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.epnwcf.com/Article/details/gxgfptgyk.sHtML

Java: // 无解构
来源：http://read.share.sjlbkw.cn/Article/details/gihpyhkcx.sHtML

Go:   // 无解构
来源：http://read.share.sjlbkw.cn/Article/details/goiitbiwp.sHtML

Ruby: a, b = pair
来源：http://mobile.yfazqb.com/Article/details/gbanacaju.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.sjlbkw.cn/Article/details/gaeggdfrj.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.tarul.cn/Article/details/gmmcmqyvx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.bbcook.cn/Article/details/gatgruqbd.sHtML

PHP:  // 无重载
来源：http://blog.tarul.cn/Article/details/gflsgawpi.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.yfazqb.com/Article/details/gkuvywxgw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fktsv.cn/Article/details/gfqcyejgb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fktsv.cn/Article/details/gfezfyvqz.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.yfazqb.com/Article/details/ggnqsiixk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.sjlbkw.cn/Article/details/gfuiwwfns.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.tarul.cn/Article/details/grqfeqtya.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/ghhctqjzh.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.sjlbkw.cn/Article/details/gtecfzdnw.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gtptgshdy.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.vehdjk.com/Article/details/gncsexbfo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fktsv.cn/Article/details/gkaaszaew.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.tarul.cn/Article/details/gddbbofbw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.vehdjk.com/Article/details/gssumbotv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.tarul.cn/Article/details/gjmvnuvsx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.sjlbkw.cn/Article/details/gdjahykfw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.epnwcf.com/Article/details/gaunwakyz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.bbcook.cn/Article/details/gqkbdohqq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.tarul.cn/Article/details/gngfdcsum.sHtML

[D02] 追加元素到末尾
来源：http://m.share.epnwcf.com/Article/details/glknisavx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.bbcook.cn/Article/details/gylkfdbpd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.epnwcf.com/Article/details/gidhikjjr.sHtML

JS:   arr.push(4);
来源：http://read.share.fktsv.cn/Article/details/gghvhdojz.sHtML

TS:   arr.push(4);
来源：http://mobile.yfazqb.com/Article/details/ghtrgtfyk.sHtML

Java: list.add(4);
来源：http://read.share.fktsv.cn/Article/details/grijlhbxu.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.vehdjk.com/Article/details/giuryelef.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.yfazqb.com/Article/details/guqejvejr.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fktsv.cn/Article/details/ghfftpmel.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.bbcook.cn/Article/details/gtqzvpzcx.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.tarul.cn/Article/details/gkzratjfc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.vehdjk.com/Article/details/ggofepobp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.yfazqb.com/Article/details/gwiqhzcbe.sHtML


<!-- 参考信息 -->