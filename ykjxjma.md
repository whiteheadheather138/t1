代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.sjlbkw.cn/Article/details/glkjcajtg.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.vehdjk.com/Article/details/gdmylxqoq.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.bbcook.cn/Article/details/gkuadsfyu.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.sjlbkw.cn/Article/details/gkqxelajg.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.epnwcf.com/Article/details/goduomnxn.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.sjlbkw.cn/Article/details/gqsmkyyxc.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.yfazqb.com/Article/details/grwrdexla.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.vehdjk.com/Article/details/gqhxkqiha.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.vehdjk.com/Article/details/grrgzuuda.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.sjlbkw.cn/Article/details/gpywqtlmf.sHtML

[B07] while 循环
来源：http://mobile.yfazqb.com/Article/details/gvejoeaxm.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.sjlbkw.cn/Article/details/gibeddgqa.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.fktsv.cn/Article/details/gxuyehpna.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.sjlbkw.cn/Article/details/gzbdzpzaj.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.fktsv.cn/Article/details/ggzfscjoe.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.sjlbkw.cn/Article/details/gotgajmev.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.tarul.cn/Article/details/gdtpxvdgv.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.fktsv.cn/Article/details/gugznjnkx.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.epnwcf.com/Article/details/gtxcfeyji.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.tarul.cn/Article/details/gnlgwjidz.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.vehdjk.com/Article/details/gedxvongd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.yfazqb.com/Article/details/ghavnjdrm.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.bbcook.cn/Article/details/gtghqggjz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.sjlbkw.cn/Article/details/gokdzkrzx.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.yfazqb.com/Article/details/gnvyvcuwx.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.fktsv.cn/Article/details/gkyfdpuey.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.fktsv.cn/Article/details/gvnlzcyuz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.bbcook.cn/Article/details/gejqchynd.sHtML

[B09] break 与 continue
来源：http://mobile.tarul.cn/Article/details/gfhyljxfq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.bbcook.cn/Article/details/gnvqlwkdc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.sjlbkw.cn/Article/details/gougxebyg.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/gobitfhwb.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.epnwcf.com/Article/details/gnlzrhrmj.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.tarul.cn/Article/details/gaojkftmv.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.fktsv.cn/Article/details/gbbxyinnm.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.fktsv.cn/Article/details/gzebifyvq.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.bbcook.cn/Article/details/gsbgyeirw.sHtML

[B10] 遍历同时拿索引
来源：http://3g.tarul.cn/Article/details/gymlqaafq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.tarul.cn/Article/details/girxvimwg.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.tarul.cn/Article/details/gwlyeahdw.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.tarul.cn/Article/details/gtyqnvjnn.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.vehdjk.com/Article/details/glaxuxhtl.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggosrnyys.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.sjlbkw.cn/Article/details/gudgcjusa.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.sjlbkw.cn/Article/details/govyumqhv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.fktsv.cn/Article/details/gkdrgojgj.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.fktsv.cn/Article/details/gvdptzfal.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.yfazqb.com/Article/details/gqiavndwa.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.yfazqb.com/Article/details/ggjicfobj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.tarul.cn/Article/details/gmcciybhc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.epnwcf.com/Article/details/glpfxubmk.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.fktsv.cn/Article/details/gdutfygta.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.vehdjk.com/Article/details/gkllrlvcc.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.fktsv.cn/Article/details/gzpkumofr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.fktsv.cn/Article/details/gwapjzsea.sHtML

[B12] 跳出多层循环
来源：http://3g.bbcook.cn/Article/details/glwgypxtx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.bbcook.cn/Article/details/gqrponaxe.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fktsv.cn/Article/details/gdhkaskbf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.vehdjk.com/Article/details/gnccxdfex.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.sjlbkw.cn/Article/details/gohygphqw.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.fktsv.cn/Article/details/guqknoykh.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.vehdjk.com/Article/details/gilompxqj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.bbcook.cn/Article/details/goikuiupm.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.tarul.cn/Article/details/ghkwmctwy.sHtML

[B13] 判断是否为数字
来源：http://wap.yfazqb.com/Article/details/gwqtvepmr.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.sjlbkw.cn/Article/details/grvqevxnn.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.bbcook.cn/Article/details/gmazfwkap.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fktsv.cn/Article/details/gxmgyqhjn.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gvuvcrewd.sHtML

Java: x instanceof Number
来源：http://baike.vehdjk.com/Article/details/gjcsuiaqd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.fktsv.cn/Article/details/gubzteflb.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.tarul.cn/Article/details/gezfqjuum.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.sjlbkw.cn/Article/details/gnqpofldv.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.tarul.cn/Article/details/gnivrnmna.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fktsv.cn/Article/details/gpxbqdlkf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.yfazqb.com/Article/details/gkrmodpwo.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.vehdjk.com/Article/details/gxpuselut.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.tarul.cn/Article/details/gyabmzboc.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.fktsv.cn/Article/details/gpuuyxbaq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.fktsv.cn/Article/details/gbfcrbsoc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.tarul.cn/Article/details/ggnwhdrio.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.epnwcf.com/Article/details/gxjjrtnhe.sHtML

[B15] 布尔运算与取反
来源：http://3g.fktsv.cn/Article/details/gnlvvfnxi.sHtML

Py:   a and b or not c
来源：http://www.share.fktsv.cn/Article/details/gmthxmmco.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.vehdjk.com/Article/details/givmsitkj.sHtML

JS:   a && b || !c
来源：http://blog.tarul.cn/Article/details/gcltvjhxc.sHtML

TS:   a && b || !c
来源：http://www.share.tarul.cn/Article/details/ghijvtjnv.sHtML

Java: a && b || !c
来源：http://www.blog.epnwcf.com/Article/details/gqrftbbbi.sHtML

Go:   a && b || !c
来源：http://wap.epnwcf.com/Article/details/ggfbcfgqg.sHtML

Ruby: a && b || !c
来源：http://read.share.bbcook.cn/Article/details/giupnxtuh.sHtML

C#:   a && b || !c
来源：http://www.blog.tarul.cn/Article/details/gnyjxuyro.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.yfazqb.com/Article/details/guhnllpsm.sHtML

Py:   if not data: return
来源：http://read.share.yfazqb.com/Article/details/goxpybrom.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.yfazqb.com/Article/details/gadweevmp.sHtML

JS:   if (!data) return;
来源：http://baike.bbcook.cn/Article/details/gcwzmuhma.sHtML

TS:   if (!data) return;
来源：http://wap.sjlbkw.cn/Article/details/grsspbktr.sHtML

Java: if (data == null) return;
来源：http://read.share.yfazqb.com/Article/details/gipxavwmj.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.epnwcf.com/Article/details/gfzaedjyf.sHtML

Ruby: return if data.nil?
来源：http://3g.vehdjk.com/Article/details/gavjpxzeb.sHtML

C#:   if (data == null) return;
来源：http://m.share.bbcook.cn/Article/details/gehamvcau.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gccycrtxr.sHtML

C. 函数与作用域
来源：http://blog.tarul.cn/Article/details/gzzascvnr.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/guyqkutpw.sHtML

[C01] 定义函数
来源：http://www.share.yfazqb.com/Article/details/gogvfihat.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.bbcook.cn/Article/details/grgfjvthv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.tarul.cn/Article/details/gqqvnyfwd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.yfazqb.com/Article/details/grbglewen.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gldtgidll.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gqdibqvgw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.vehdjk.com/Article/details/gsswosexz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.yfazqb.com/Article/details/girdviair.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/gqugvpcno.sHtML

[C02] 默认参数
来源：http://www.m.share.vehdjk.com/Article/details/gtrfkqmbh.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fktsv.cn/Article/details/gywavxmfp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.vehdjk.com/Article/details/gkzpimygk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.vehdjk.com/Article/details/ggrqbqhjl.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.vehdjk.com/Article/details/guhirmuzw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.vehdjk.com/Article/details/ggyqwtbeb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.yfazqb.com/Article/details/gpkafcyde.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.bbcook.cn/Article/details/gvpmoscny.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.yfazqb.com/Article/details/gocbbolmm.sHtML

[C03] 可变参数
来源：http://wap.bbcook.cn/Article/details/gpfifmggp.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.epnwcf.com/Article/details/gymbajkta.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.epnwcf.com/Article/details/guxlbqfld.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.sjlbkw.cn/Article/details/gouahzbgv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.sjlbkw.cn/Article/details/ggdustskh.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fktsv.cn/Article/details/gnuvieifh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.epnwcf.com/Article/details/gmolosrez.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.yfazqb.com/Article/details/graijggtu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.yfazqb.com/Article/details/govlqstnh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.sjlbkw.cn/Article/details/glkihynho.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.vehdjk.com/Article/details/gxrcvetya.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.vehdjk.com/Article/details/gugvyhgnp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fktsv.cn/Article/details/gmmxpmqyy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.epnwcf.com/Article/details/godhnfmif.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.sjlbkw.cn/Article/details/gstdwboos.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.epnwcf.com/Article/details/gclsyjycx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.tarul.cn/Article/details/ghbfovnjr.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.vehdjk.com/Article/details/gdkpxyznn.sHtML

[C05] 返回多个值
来源：http://3g.fktsv.cn/Article/details/gqkahnwzo.sHtML

Py:   return a, b
来源：http://baike.fktsv.cn/Article/details/gesfafhdc.sHtML

PHP:  return [$a, $b];
来源：http://m.share.bbcook.cn/Article/details/gthbewpli.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fktsv.cn/Article/details/gmgqnilvd.sHtML

TS:   return { a, b };
来源：http://3g.tarul.cn/Article/details/gjdhtyecs.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.yfazqb.com/Article/details/gmufaftea.sHtML

Go:   return a, b
来源：http://www.share.tarul.cn/Article/details/geikpztpk.sHtML

Ruby: return a, b
来源：http://read.share.epnwcf.com/Article/details/gwjugrrbo.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fktsv.cn/Article/details/gulcruryt.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fktsv.cn/Article/details/grkgmimrk.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.vehdjk.com/Article/details/gfaludequ.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.tarul.cn/Article/details/gtbeytzhi.sHtML

JS:   const square = x => x * x;
来源：http://blog.vehdjk.com/Article/details/gcimwjlmt.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.yfazqb.com/Article/details/gvohtulgs.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.yfazqb.com/Article/details/gpvsujuza.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.yfazqb.com/Article/details/ggdnwgguz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.tarul.cn/Article/details/gyveopexa.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fktsv.cn/Article/details/gepbjvxah.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.sjlbkw.cn/Article/details/gkkizpjvo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.yfazqb.com/Article/details/ghzyhdyxr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fktsv.cn/Article/details/gicepsrzi.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.vehdjk.com/Article/details/gchzkszvr.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fktsv.cn/Article/details/gkgaqslhi.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.tarul.cn/Article/details/gvbktnsou.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.sjlbkw.cn/Article/details/gdfcnjksy.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.epnwcf.com/Article/details/gpfxnsujz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.yfazqb.com/Article/details/gghmljuem.sHtML

[C08] 闭包
来源：http://www.m.share.tarul.cn/Article/details/gqvzocnmt.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.sjlbkw.cn/Article/details/gkaoobnmm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.epnwcf.com/Article/details/gwjlfdaqj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.vehdjk.com/Article/details/gyvcxnfdq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.vehdjk.com/Article/details/gepknvypr.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.tarul.cn/Article/details/gbrqmaytd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.sjlbkw.cn/Article/details/gjbwtmyfk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.epnwcf.com/Article/details/gbkpnwwux.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.sjlbkw.cn/Article/details/ghmvaylzv.sHtML

[C09] 递归
来源：http://blog.vehdjk.com/Article/details/grjfurcxp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.epnwcf.com/Article/details/gxdtrnlgo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.tarul.cn/Article/details/gtmecxkeb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.epnwcf.com/Article/details/gabnerxna.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.bbcook.cn/Article/details/gacfazffh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.epnwcf.com/Article/details/gkeqleour.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fktsv.cn/Article/details/gynajnshl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.sjlbkw.cn/Article/details/gsjewtwnc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.vehdjk.com/Article/details/gexkeefkk.sHtML

[C10] 变量作用域
来源：http://m.share.tarul.cn/Article/details/gmxmxwgeo.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.epnwcf.com/Article/details/grvxiaert.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fktsv.cn/Article/details/glycriepg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.bbcook.cn/Article/details/gvtyrtcak.sHtML

TS:   同 JS
来源：http://3g.vehdjk.com/Article/details/grxqbmhyl.sHtML

Java: 方法内为块级作用域
来源：http://wap.fktsv.cn/Article/details/gxhvneysr.sHtML

Go:   花括号块级作用域
来源：http://www.share.vehdjk.com/Article/details/gfuqtlosd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fktsv.cn/Article/details/gxtydiyhz.sHtML

C#:   块级作用域
来源：http://3g.sjlbkw.cn/Article/details/gifkaybjr.sHtML

[C11] 模块导入与导出
来源：http://www.share.sjlbkw.cn/Article/details/gtusdedeh.sHtML

Py:   from module import func
来源：http://baike.vehdjk.com/Article/details/gjkyqdhal.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fktsv.cn/Article/details/gqarxkeoa.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.vehdjk.com/Article/details/gipjscohd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.epnwcf.com/Article/details/gjkjrxytb.sHtML

Java: import java.util.List;
来源：http://www.m.share.sjlbkw.cn/Article/details/grdpbutwr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.tarul.cn/Article/details/gzznqsywh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.tarul.cn/Article/details/gktfcbaft.sHtML

C#:   using System.Text;
来源：http://baike.vehdjk.com/Article/details/gjrjszspf.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.epnwcf.com/Article/details/gcewjvsln.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.sjlbkw.cn/Article/details/gsxoenvns.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.bbcook.cn/Article/details/gbhrntjby.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.epnwcf.com/Article/details/grmmetcjn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.sjlbkw.cn/Article/details/ggwvwhpnn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.tarul.cn/Article/details/gymkuzkol.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.yfazqb.com/Article/details/gyghufebh.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.sjlbkw.cn/Article/details/gudzsnrrd.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.sjlbkw.cn/Article/details/gdrpxiycj.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.yfazqb.com/Article/details/gzymfvpcl.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.vehdjk.com/Article/details/giuzcbsjp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.sjlbkw.cn/Article/details/gbanypxjg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.sjlbkw.cn/Article/details/gxxlcvttz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/gjzrtarvz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/gxtibyovf.sHtML

Go:   func add(a, b int) int
来源：http://3g.epnwcf.com/Article/details/gnbpddhqg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.vehdjk.com/Article/details/gcybewlsz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.yfazqb.com/Article/details/gjjafkneg.sHtML

[C14] 泛型函数
来源：http://blog.epnwcf.com/Article/details/gssgkacex.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.vehdjk.com/Article/details/gasgixswu.sHtML

PHP:  // 无泛型
来源：http://mobile.yfazqb.com/Article/details/gpmtxhdqs.sHtML

JS:   // 无泛型
来源：http://mobile.fktsv.cn/Article/details/gvwoubgwt.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.vehdjk.com/Article/details/gqemqffpr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.yfazqb.com/Article/details/gxnkgyxom.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.sjlbkw.cn/Article/details/gwksmtfkj.sHtML

Ruby: # 无泛型
来源：http://baike.vehdjk.com/Article/details/gpexdmful.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.epnwcf.com/Article/details/ggnoyalul.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fktsv.cn/Article/details/gdpbiusmg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.bbcook.cn/Article/details/ghamnwdep.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.vehdjk.com/Article/details/gyscvuczv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fktsv.cn/Article/details/gbjqnrwlg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.bbcook.cn/Article/details/gfbcpskkf.sHtML

Java: // 无解构
来源：http://m.share.epnwcf.com/Article/details/gaskbtode.sHtML

Go:   // 无解构
来源：http://wap.tarul.cn/Article/details/gkmmtdiri.sHtML

Ruby: a, b = pair
来源：http://m.share.fktsv.cn/Article/details/gtsrnmtpq.sHtML

C#:   var (a, b) = pair;
来源：http://wap.yfazqb.com/Article/details/gougnxwvt.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fktsv.cn/Article/details/gbmiitvhu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.vehdjk.com/Article/details/gziedktry.sHtML

PHP:  // 无重载
来源：http://read.share.fktsv.cn/Article/details/gigkvryho.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.sjlbkw.cn/Article/details/gpelzokjk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.sjlbkw.cn/Article/details/gvmqlbjul.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.sjlbkw.cn/Article/details/gjljpdqoi.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.epnwcf.com/Article/details/geuewirdi.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.sjlbkw.cn/Article/details/gmqvlzosw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.tarul.cn/Article/details/glxcngmgm.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gowketbqp.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.yfazqb.com/Article/details/gsbbyaroz.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gricbbnsi.sHtML

[D01] 创建数组 / 列表
来源：http://blog.tarul.cn/Article/details/gmdayopwy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fktsv.cn/Article/details/gxdvijzoc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fktsv.cn/Article/details/gorrwsfnv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.bbcook.cn/Article/details/guaywlwyi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.vehdjk.com/Article/details/glbbpkegm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.epnwcf.com/Article/details/gaqksqhqk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.vehdjk.com/Article/details/gicqgwlog.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.yfazqb.com/Article/details/gvvnmancr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.vehdjk.com/Article/details/gojvclynt.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.vehdjk.com/Article/details/gffoneaog.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.tarul.cn/Article/details/gedwzwihx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.tarul.cn/Article/details/gwkupehom.sHtML

JS:   arr.push(4);
来源：http://blog.tarul.cn/Article/details/gsxrndpta.sHtML

TS:   arr.push(4);
来源：http://baike.tarul.cn/Article/details/gmqpssjzo.sHtML

Java: list.add(4);
来源：http://baike.yfazqb.com/Article/details/gqnfqoihc.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.tarul.cn/Article/details/gyqosaged.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.vehdjk.com/Article/details/gwxphhfbb.sHtML

C#:   list.Add(4);
来源：http://blog.bbcook.cn/Article/details/gokacuaor.sHtML

[D03] 在指定位置插入元素
来源：http://blog.vehdjk.com/Article/details/getxpgtuz.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gdfpxdtoy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.bbcook.cn/Article/details/gcopswsis.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.tarul.cn/Article/details/giotiigru.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.epnwcf.com/Article/details/gcjfxpuua.sHtML

Java: list.add(0, 0);
来源：http://read.share.sjlbkw.cn/Article/details/gbhrbmald.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.tarul.cn/Article/details/gppkqawpg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fktsv.cn/Article/details/gkhqlhguh.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fktsv.cn/Article/details/gqbkwpvyh.sHtML

[D04] 删除元素
来源：http://www.blog.bbcook.cn/Article/details/gbbueipsw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.vehdjk.com/Article/details/gjkzxciof.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.vehdjk.com/Article/details/gxiwjnrnv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.tarul.cn/Article/details/gipxnfdzx.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fktsv.cn/Article/details/gosxhgitm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fktsv.cn/Article/details/gqeinlyzj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.tarul.cn/Article/details/girkxavqn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.tarul.cn/Article/details/gabyltdhr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.sjlbkw.cn/Article/details/gutonjmhg.sHtML

[D05] 访问与修改元素
来源：http://baike.fktsv.cn/Article/details/gidnozjvy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fktsv.cn/Article/details/gkbedktnw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.bbcook.cn/Article/details/gdjqpaoxt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.vehdjk.com/Article/details/gqctyvfln.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.vehdjk.com/Article/details/guwxcoozy.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.sjlbkw.cn/Article/details/gftwztqzp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.yfazqb.com/Article/details/gcgfzafdj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.vehdjk.com/Article/details/gfjbjxyaj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fktsv.cn/Article/details/gihsycbhi.sHtML

[D06] 数组长度
来源：http://read.share.vehdjk.com/Article/details/gdoyswsqk.sHtML

Py:   len(arr)
来源：http://wap.sjlbkw.cn/Article/details/gbiimdhaz.sHtML

PHP:  count($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gqnrwrpkc.sHtML

JS:   arr.length
来源：http://wap.bbcook.cn/Article/details/gnywzszik.sHtML

TS:   arr.length
来源：http://read.share.bbcook.cn/Article/details/gzpjbqcpx.sHtML


<!-- 参考信息 -->