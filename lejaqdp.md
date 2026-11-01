代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.epnwcf.com/Article/details/gqgkrbmpc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.yfazqb.com/Article/details/ggczaavfm.sHtML

[B03] switch / match / case
来源：http://wap.bbcook.cn/Article/details/gqknlzaxy.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.epnwcf.com/Article/details/gcbfejdgh.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.vehdjk.com/Article/details/gegtrejns.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fktsv.cn/Article/details/gqxlnvrpa.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fktsv.cn/Article/details/gtteqaltv.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.vehdjk.com/Article/details/gzvkknenu.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.epnwcf.com/Article/details/gdwidbext.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.sjlbkw.cn/Article/details/grtyfmheb.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.fktsv.cn/Article/details/grmwfllgl.sHtML

[B04] for 计数循环
来源：http://www.m.share.tarul.cn/Article/details/gxsqvzobk.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.yfazqb.com/Article/details/gyxdxvqkq.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.tarul.cn/Article/details/gaxdiagxo.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.epnwcf.com/Article/details/gtsnenkxe.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fktsv.cn/Article/details/gssbmqjrq.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.fktsv.cn/Article/details/gtwyisook.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.epnwcf.com/Article/details/goemgniss.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.tarul.cn/Article/details/gkznsyvmg.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.tarul.cn/Article/details/gmaajbbpg.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.vehdjk.com/Article/details/gijgmnkto.sHtML

Py:   for item in arr: print(item)
来源：http://3g.sjlbkw.cn/Article/details/grfgrirzg.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.tarul.cn/Article/details/gpgtlibrs.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.yfazqb.com/Article/details/gpwyejygw.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.epnwcf.com/Article/details/gefocxioy.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.sjlbkw.cn/Article/details/ghtkyjulq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.tarul.cn/Article/details/gzhujkxrb.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.bbcook.cn/Article/details/gevkkhzoo.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.yfazqb.com/Article/details/gqfyozspe.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.bbcook.cn/Article/details/gvjhkynnx.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.bbcook.cn/Article/details/geclcaopm.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.yfazqb.com/Article/details/gzlubklfo.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.epnwcf.com/Article/details/gqhmohawq.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.epnwcf.com/Article/details/goaqxrswr.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.sjlbkw.cn/Article/details/gqrwaoolw.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.epnwcf.com/Article/details/golbqzdjn.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.vehdjk.com/Article/details/gkptupnqg.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjtyarnuz.sHtML

[B07] while 循环
来源：http://mobile.yfazqb.com/Article/details/gxhsdpawo.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.sjlbkw.cn/Article/details/gztqmmvvo.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.bbcook.cn/Article/details/guruhffjz.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.tarul.cn/Article/details/ggwjdktuj.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.yfazqb.com/Article/details/gnjilmbpq.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.fktsv.cn/Article/details/guwvyhxyy.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.fktsv.cn/Article/details/gsfjbquef.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.fktsv.cn/Article/details/gzhawpvhv.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gipawdnhk.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.tarul.cn/Article/details/gmvfxmabt.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.vehdjk.com/Article/details/gpppxskht.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.epnwcf.com/Article/details/gqqhublnw.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.yfazqb.com/Article/details/gggpjajay.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.epnwcf.com/Article/details/gfpvatvlg.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.tarul.cn/Article/details/goxkpixza.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.fktsv.cn/Article/details/gvgwwakza.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.vehdjk.com/Article/details/gevcrjgfy.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.fktsv.cn/Article/details/gedlnaqxt.sHtML

[B09] break 与 continue
来源：http://www.share.vehdjk.com/Article/details/ggmmjcala.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.yfazqb.com/Article/details/gkenpruzo.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/gxyzmklhc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.bbcook.cn/Article/details/glfxqlift.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.vehdjk.com/Article/details/gvcycoitb.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.vehdjk.com/Article/details/gbtwcuymu.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.tarul.cn/Article/details/gtrxfxueh.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.sjlbkw.cn/Article/details/gugsfgbnl.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.tarul.cn/Article/details/gkihultbs.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.vehdjk.com/Article/details/gfmwujlka.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.yfazqb.com/Article/details/gzdqdpxxj.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.epnwcf.com/Article/details/gkycnfswt.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.vehdjk.com/Article/details/gmdcsgnkr.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.epnwcf.com/Article/details/goicnjgod.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.sjlbkw.cn/Article/details/gkaercmzg.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.vehdjk.com/Article/details/gcjtfvoji.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.epnwcf.com/Article/details/gcawoxyeq.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.yfazqb.com/Article/details/ggflwiwvs.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.vehdjk.com/Article/details/gkddevrio.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.vehdjk.com/Article/details/gciwhjlnt.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.yfazqb.com/Article/details/golpgigrm.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.vehdjk.com/Article/details/gmlfjgged.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.bbcook.cn/Article/details/gyhqinepd.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.bbcook.cn/Article/details/geppytfbj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.bbcook.cn/Article/details/gpplusvuf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.sjlbkw.cn/Article/details/gxfolcwiq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.tarul.cn/Article/details/gdyeukuec.sHtML

[B12] 跳出多层循环
来源：http://wap.sjlbkw.cn/Article/details/gpeplxzkv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.vehdjk.com/Article/details/gfcvwelhn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.bbcook.cn/Article/details/grhtzgnlf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.bbcook.cn/Article/details/gmdgzvrci.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fktsv.cn/Article/details/gdfyllmpp.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.vehdjk.com/Article/details/gqjjqmrvs.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.bbcook.cn/Article/details/gtinvptwp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.epnwcf.com/Article/details/gtrbrnwlx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.epnwcf.com/Article/details/grdjsxsny.sHtML

[B13] 判断是否为数字
来源：http://mobile.epnwcf.com/Article/details/gzpytxjzg.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.tarul.cn/Article/details/gqizprfic.sHtML

PHP:  is_numeric($x)
来源：http://www.share.fktsv.cn/Article/details/gtwnkeleg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fktsv.cn/Article/details/gamhnyeds.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fktsv.cn/Article/details/gaajhunan.sHtML

Java: x instanceof Number
来源：http://wap.fktsv.cn/Article/details/gwpvurcev.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.vehdjk.com/Article/details/gkamcjkej.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.bbcook.cn/Article/details/gqlqpdcyq.sHtML

C#:   x is int or double or decimal
来源：http://mobile.epnwcf.com/Article/details/gtpozmvhq.sHtML

[B14] 判断值是否在集合内
来源：http://blog.tarul.cn/Article/details/gvfodvauu.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.tarul.cn/Article/details/gcjzycdvg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.yfazqb.com/Article/details/gabzslxhx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.vehdjk.com/Article/details/gfjptahxq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.tarul.cn/Article/details/gxyfwqflx.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.bbcook.cn/Article/details/gchjcjzps.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.yfazqb.com/Article/details/ghhkxpndr.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.sjlbkw.cn/Article/details/ggrviomqg.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.bbcook.cn/Article/details/ggomhlvpa.sHtML

[B15] 布尔运算与取反
来源：http://blog.sjlbkw.cn/Article/details/gifbsuirs.sHtML

Py:   a and b or not c
来源：http://blog.bbcook.cn/Article/details/gwrebgarl.sHtML

PHP:  $a && $b || !$c
来源：http://blog.tarul.cn/Article/details/ggwiolkri.sHtML

JS:   a && b || !c
来源：http://wap.fktsv.cn/Article/details/gwivpbgdy.sHtML

TS:   a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/gocehantc.sHtML

Java: a && b || !c
来源：http://baike.tarul.cn/Article/details/gnavkbvni.sHtML

Go:   a && b || !c
来源：http://m.share.yfazqb.com/Article/details/gtdqgaknh.sHtML

Ruby: a && b || !c
来源：http://3g.fktsv.cn/Article/details/gkbvhjaqo.sHtML

C#:   a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gyalmsxkr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.vehdjk.com/Article/details/gsngjyvip.sHtML

Py:   if not data: return
来源：http://www.m.share.fktsv.cn/Article/details/gfrbdpxpq.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.bbcook.cn/Article/details/gzytxoiiz.sHtML

JS:   if (!data) return;
来源：http://mobile.epnwcf.com/Article/details/gyyizxkio.sHtML

TS:   if (!data) return;
来源：http://3g.fktsv.cn/Article/details/gxrqhuqcf.sHtML

Java: if (data == null) return;
来源：http://wap.tarul.cn/Article/details/gdzkejwkt.sHtML

Go:   if data == nil { return }
来源：http://3g.yfazqb.com/Article/details/glzbdyhml.sHtML

Ruby: return if data.nil?
来源：http://www.blog.sjlbkw.cn/Article/details/gtoeaopyf.sHtML

C#:   if (data == null) return;
来源：http://read.share.tarul.cn/Article/details/gamelpbdm.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/glxumtvvh.sHtML

C. 函数与作用域
来源：http://www.blog.bbcook.cn/Article/details/gcmgajagb.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gvvyogdeg.sHtML

[C01] 定义函数
来源：http://www.share.sjlbkw.cn/Article/details/gphxmdslu.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.yfazqb.com/Article/details/gyieakler.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.sjlbkw.cn/Article/details/ghogucapo.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/gimnafxqb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gjyfmqwkl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fktsv.cn/Article/details/ggxapcucb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.vehdjk.com/Article/details/gkrsygyfg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.sjlbkw.cn/Article/details/gyvcfznnx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gokcytjhh.sHtML

[C02] 默认参数
来源：http://wap.vehdjk.com/Article/details/gaslpkqwz.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.bbcook.cn/Article/details/gdhrsxxcl.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.tarul.cn/Article/details/gloukzsbh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.yfazqb.com/Article/details/gvmpmyfsd.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.yfazqb.com/Article/details/gqulxgauo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.vehdjk.com/Article/details/ghmqqjbex.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.yfazqb.com/Article/details/gevcolpkg.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.epnwcf.com/Article/details/grtaaxanz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.sjlbkw.cn/Article/details/gemfkoual.sHtML

[C03] 可变参数
来源：http://baike.tarul.cn/Article/details/giwsabtpq.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.sjlbkw.cn/Article/details/gheaptbig.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.vehdjk.com/Article/details/gavrhziot.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.epnwcf.com/Article/details/gvlipxcge.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.sjlbkw.cn/Article/details/gluhgfeax.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fktsv.cn/Article/details/gvbaxjfiv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.epnwcf.com/Article/details/geecsgkis.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.epnwcf.com/Article/details/gaelflqls.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.vehdjk.com/Article/details/gbxxvcbvy.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.bbcook.cn/Article/details/gylwwtxtb.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.tarul.cn/Article/details/gzaddrjrx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.sjlbkw.cn/Article/details/gtogandcn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.epnwcf.com/Article/details/gcvpbnimg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.sjlbkw.cn/Article/details/gmuoyuyag.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.yfazqb.com/Article/details/gzkmdlzyq.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.yfazqb.com/Article/details/gmujwwxxo.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.tarul.cn/Article/details/gpshogxfj.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.bbcook.cn/Article/details/gtgsdyjie.sHtML

[C05] 返回多个值
来源：http://m.share.sjlbkw.cn/Article/details/gwgveidtp.sHtML

Py:   return a, b
来源：http://blog.tarul.cn/Article/details/gejdlhmbz.sHtML

PHP:  return [$a, $b];
来源：http://www.share.tarul.cn/Article/details/gnfgwadry.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.epnwcf.com/Article/details/gsvknxmtz.sHtML

TS:   return { a, b };
来源：http://www.m.share.bbcook.cn/Article/details/ghozyncwa.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.tarul.cn/Article/details/ggbmvaqgk.sHtML

Go:   return a, b
来源：http://wap.epnwcf.com/Article/details/gypbxrgae.sHtML

Ruby: return a, b
来源：http://3g.fktsv.cn/Article/details/gqwfuadzq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.epnwcf.com/Article/details/gicaygnxj.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.tarul.cn/Article/details/gryfbgxax.sHtML

Py:   square = lambda x: x * x
来源：http://3g.sjlbkw.cn/Article/details/ghuftohmk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.bbcook.cn/Article/details/gtmbqcgbu.sHtML

JS:   const square = x => x * x;
来源：http://read.share.fktsv.cn/Article/details/grgnsnhcy.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.yfazqb.com/Article/details/gqxznfdyz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fktsv.cn/Article/details/gkabbupvn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.bbcook.cn/Article/details/gwvihykes.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.vehdjk.com/Article/details/ghaoyvkad.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.tarul.cn/Article/details/ghygdpsmj.sHtML

[C07] 把函数作为参数传入
来源：http://blog.yfazqb.com/Article/details/gwwgqkxre.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.yfazqb.com/Article/details/gzmfierzk.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.vehdjk.com/Article/details/gxwxcymfp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.yfazqb.com/Article/details/gfdscytyp.sHtML

TS:   arr.map(String)
来源：http://3g.yfazqb.com/Article/details/gsvhckofr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.vehdjk.com/Article/details/gwpomngrq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.vehdjk.com/Article/details/gblscgdof.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.sjlbkw.cn/Article/details/glnzwprnn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fktsv.cn/Article/details/gjsytkatr.sHtML

[C08] 闭包
来源：http://m.share.epnwcf.com/Article/details/gyfpfskcw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.epnwcf.com/Article/details/gzioaifja.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhgazdnq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.bbcook.cn/Article/details/gdvhmwlql.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.epnwcf.com/Article/details/gosqbpldj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.yfazqb.com/Article/details/gkcihymbm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.yfazqb.com/Article/details/gcatclyuj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.bbcook.cn/Article/details/gtjnxadbs.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.vehdjk.com/Article/details/gdghjitap.sHtML

[C09] 递归
来源：http://3g.sjlbkw.cn/Article/details/gbcqrjejz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.yfazqb.com/Article/details/ggijlbvwe.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.vehdjk.com/Article/details/gxrovihgq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.epnwcf.com/Article/details/gykibjddw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.tarul.cn/Article/details/gdrwjmczd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.sjlbkw.cn/Article/details/gxtotrlll.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.yfazqb.com/Article/details/godlawtev.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.yfazqb.com/Article/details/gdcsypgeb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.yfazqb.com/Article/details/gtfxqmopv.sHtML

[C10] 变量作用域
来源：http://mobile.vehdjk.com/Article/details/gtpmyssth.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.yfazqb.com/Article/details/gikduvjyv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fktsv.cn/Article/details/geviixkqc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.epnwcf.com/Article/details/gpriaccsv.sHtML

TS:   同 JS
来源：http://wap.bbcook.cn/Article/details/gidebslnl.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.vehdjk.com/Article/details/gckipmywa.sHtML

Go:   花括号块级作用域
来源：http://m.share.tarul.cn/Article/details/gluausspt.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.epnwcf.com/Article/details/gnvywcckq.sHtML

C#:   块级作用域
来源：http://wap.bbcook.cn/Article/details/gesxseqpv.sHtML

[C11] 模块导入与导出
来源：http://baike.bbcook.cn/Article/details/govysflce.sHtML

Py:   from module import func
来源：http://3g.bbcook.cn/Article/details/gscayicrb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.tarul.cn/Article/details/gjqydrnxh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.bbcook.cn/Article/details/gujipdhti.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.epnwcf.com/Article/details/ggvsufahs.sHtML

Java: import java.util.List;
来源：http://www.blog.yfazqb.com/Article/details/gvfgzzexz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.yfazqb.com/Article/details/gddpjjbvw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.yfazqb.com/Article/details/gwqegzugw.sHtML

C#:   using System.Text;
来源：http://read.share.fktsv.cn/Article/details/gkvkhoveh.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.sjlbkw.cn/Article/details/gebtmtgpw.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.yfazqb.com/Article/details/gxurnmlwd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.bbcook.cn/Article/details/gxhhjvdis.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.yfazqb.com/Article/details/gyorxjpbx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.yfazqb.com/Article/details/gwcpfgflo.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.vehdjk.com/Article/details/grfcrlrsl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.sjlbkw.cn/Article/details/gtskgmpcm.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.tarul.cn/Article/details/gbvzxyedh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fktsv.cn/Article/details/guustaljx.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.vehdjk.com/Article/details/gofwrlqeu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.sjlbkw.cn/Article/details/gyyhsksbp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fktsv.cn/Article/details/gdacgazfn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.bbcook.cn/Article/details/gmlqbhgpc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gmgrwgqsv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.bbcook.cn/Article/details/ghsgrcvda.sHtML

Go:   func add(a, b int) int
来源：http://3g.fktsv.cn/Article/details/gkvpcivsl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.sjlbkw.cn/Article/details/gdwahhljb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.epnwcf.com/Article/details/gvzgooqzr.sHtML

[C14] 泛型函数
来源：http://read.share.tarul.cn/Article/details/gzyyehgks.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.bbcook.cn/Article/details/gnuussdfc.sHtML

PHP:  // 无泛型
来源：http://www.m.share.vehdjk.com/Article/details/geptswcoo.sHtML

JS:   // 无泛型
来源：http://3g.vehdjk.com/Article/details/guzpauxei.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.bbcook.cn/Article/details/gpslhiaqu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.tarul.cn/Article/details/gkbiimylf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.vehdjk.com/Article/details/gdyduwkdq.sHtML

Ruby: # 无泛型
来源：http://m.share.sjlbkw.cn/Article/details/grciyziwc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fktsv.cn/Article/details/gyerzhddz.sHtML

[C15] 解构 / 展开参数
来源：http://baike.bbcook.cn/Article/details/gwfraibge.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.tarul.cn/Article/details/gfbgqdqlu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.sjlbkw.cn/Article/details/gppuwgsdt.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.tarul.cn/Article/details/gippfbfqa.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.epnwcf.com/Article/details/gehmistbe.sHtML

Java: // 无解构
来源：http://m.share.vehdjk.com/Article/details/geqfglnpl.sHtML

Go:   // 无解构
来源：http://www.m.share.bbcook.cn/Article/details/gpkqxzkuj.sHtML

Ruby: a, b = pair
来源：http://read.share.sjlbkw.cn/Article/details/gdtjxqkah.sHtML

C#:   var (a, b) = pair;
来源：http://3g.sjlbkw.cn/Article/details/gzztvyrcp.sHtML

[C16] 函数 / 方法重载
来源：http://baike.tarul.cn/Article/details/gqbjhvybc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.bbcook.cn/Article/details/gxuybjgfb.sHtML

PHP:  // 无重载
来源：http://www.blog.bbcook.cn/Article/details/grysyugrc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.epnwcf.com/Article/details/gzuqxjdar.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.bbcook.cn/Article/details/gzutczamn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.tarul.cn/Article/details/gqgspqmer.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.vehdjk.com/Article/details/ggtcyrlmd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.epnwcf.com/Article/details/ghookpvib.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.vehdjk.com/Article/details/gtfpmzabu.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gmqrfxunf.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.vehdjk.com/Article/details/gdiqcrloy.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/goqinjlho.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.epnwcf.com/Article/details/gocpbnpoz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.bbcook.cn/Article/details/gtpoymbij.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.bbcook.cn/Article/details/gtnqiscko.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.tarul.cn/Article/details/gesjuxiqi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.epnwcf.com/Article/details/gdbqfoocp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.vehdjk.com/Article/details/gatwvyltn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.yfazqb.com/Article/details/gknaduxuy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.yfazqb.com/Article/details/gvctkerxf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.epnwcf.com/Article/details/gjdqumzwv.sHtML

[D02] 追加元素到末尾
来源：http://3g.tarul.cn/Article/details/gelpavijp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.vehdjk.com/Article/details/gtikkbxbg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.bbcook.cn/Article/details/gmgjcxcvx.sHtML

JS:   arr.push(4);
来源：http://baike.epnwcf.com/Article/details/gmnnsxfgr.sHtML

TS:   arr.push(4);
来源：http://read.share.tarul.cn/Article/details/gelungccz.sHtML

Java: list.add(4);
来源：http://www.share.vehdjk.com/Article/details/gmdipawsl.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.vehdjk.com/Article/details/gbeokaoqm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fktsv.cn/Article/details/gmsoowgho.sHtML

C#:   list.Add(4);
来源：http://3g.sjlbkw.cn/Article/details/gxxcrddkw.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.epnwcf.com/Article/details/gebzgjpup.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.yfazqb.com/Article/details/gambuzhrc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.tarul.cn/Article/details/gwnnwnemx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.tarul.cn/Article/details/gnsypuckj.sHtML


<!-- 参考信息 -->