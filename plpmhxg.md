代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.bbcook.cn/Article/details/goezrlqth.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fktsv.cn/Article/details/guryvtadv.sHtML

[B03] switch / match / case
来源：http://m.share.fktsv.cn/Article/details/gwsekthzd.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.yfazqb.com/Article/details/gyvwztvfi.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.tarul.cn/Article/details/gaplmkecr.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.yfazqb.com/Article/details/gnjczrqvr.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.vehdjk.com/Article/details/gaqvifilw.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.vehdjk.com/Article/details/grvhfyxrd.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.bbcook.cn/Article/details/gtrbxeemk.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.sjlbkw.cn/Article/details/gangycjiy.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.vehdjk.com/Article/details/gffupahlm.sHtML

[B04] for 计数循环
来源：http://read.share.vehdjk.com/Article/details/gqmrahkfi.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.yfazqb.com/Article/details/gdzqfbpwj.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.sjlbkw.cn/Article/details/gzkunbvwv.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fktsv.cn/Article/details/gkqskqraq.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fktsv.cn/Article/details/gcgxyvapq.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.bbcook.cn/Article/details/gmelwypav.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.yfazqb.com/Article/details/gyxxttnae.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.yfazqb.com/Article/details/gbjfkjhbp.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.sjlbkw.cn/Article/details/gucusiqdt.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.vehdjk.com/Article/details/gauwmparn.sHtML

Py:   for item in arr: print(item)
来源：http://baike.tarul.cn/Article/details/gtdmozayf.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.sjlbkw.cn/Article/details/gtvzzgxub.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.yfazqb.com/Article/details/geybajfyi.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.tarul.cn/Article/details/gzhearbxk.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.tarul.cn/Article/details/gquqgxmev.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.vehdjk.com/Article/details/grqxauhsv.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.bbcook.cn/Article/details/gsldhzzxm.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.vehdjk.com/Article/details/gdqwitcbg.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.yfazqb.com/Article/details/gqrxzjljn.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.sjlbkw.cn/Article/details/gdvmhzdur.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.bbcook.cn/Article/details/gjzlqzyyw.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.epnwcf.com/Article/details/gqntfgthi.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.vehdjk.com/Article/details/gckfqtfrp.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.sjlbkw.cn/Article/details/grflaxnpe.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.yfazqb.com/Article/details/gmoixhpiu.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.epnwcf.com/Article/details/gxamlsnwh.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.epnwcf.com/Article/details/geamrtcpt.sHtML

[B07] while 循环
来源：http://read.share.yfazqb.com/Article/details/gjfdyysfu.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.bbcook.cn/Article/details/gbkoaztsg.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.tarul.cn/Article/details/gezovitge.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggtgnyqdh.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.vehdjk.com/Article/details/ghhicstyh.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.fktsv.cn/Article/details/gcdobyqha.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.yfazqb.com/Article/details/gcmmfcacd.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.tarul.cn/Article/details/gzouooseo.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.yfazqb.com/Article/details/gtbfruxar.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.yfazqb.com/Article/details/gcbvccder.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.tarul.cn/Article/details/gcvwessap.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.tarul.cn/Article/details/grhqzpwpx.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.vehdjk.com/Article/details/gzaslceci.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.vehdjk.com/Article/details/garuvzzoa.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.fktsv.cn/Article/details/gbgmmtfhf.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.bbcook.cn/Article/details/gzivldwsk.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.sjlbkw.cn/Article/details/gvjjyankq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.yfazqb.com/Article/details/gqrbvaiyf.sHtML

[B09] break 与 continue
来源：http://m.share.epnwcf.com/Article/details/geuvaumaq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.yfazqb.com/Article/details/gnbbptgns.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.yfazqb.com/Article/details/gavxzdsng.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.vehdjk.com/Article/details/gehlbezvc.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.sjlbkw.cn/Article/details/gokthtuiw.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/gjwqvdnlz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.yfazqb.com/Article/details/gevbugujx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.vehdjk.com/Article/details/gaorspnsm.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.tarul.cn/Article/details/gofuxqzdq.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.vehdjk.com/Article/details/gofwpftfi.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.fktsv.cn/Article/details/gxyfyrnhg.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.fktsv.cn/Article/details/gmhyyihec.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.fktsv.cn/Article/details/gxkzvrhrl.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.fktsv.cn/Article/details/gcyjcxijw.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.tarul.cn/Article/details/ggtodinrn.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.sjlbkw.cn/Article/details/gcgreovtn.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.sjlbkw.cn/Article/details/givilfpgw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.sjlbkw.cn/Article/details/gdumuffla.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.sjlbkw.cn/Article/details/gpqmdxlrl.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.bbcook.cn/Article/details/gezbdfuas.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.sjlbkw.cn/Article/details/guzunqoqc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fktsv.cn/Article/details/gblqnqyau.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.bbcook.cn/Article/details/ghwbstmsk.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.vehdjk.com/Article/details/gcejjfehp.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.tarul.cn/Article/details/geefngenp.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.epnwcf.com/Article/details/gsdfhonui.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.bbcook.cn/Article/details/gdqxmfvrk.sHtML

[B12] 跳出多层循环
来源：http://blog.vehdjk.com/Article/details/gevkrwmux.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.vehdjk.com/Article/details/gxyjopche.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.vehdjk.com/Article/details/gfplsfzze.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fktsv.cn/Article/details/gnmvvnwed.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.yfazqb.com/Article/details/gcmulnlxf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.fktsv.cn/Article/details/gfepscuyj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.bbcook.cn/Article/details/gjnbttxrw.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fktsv.cn/Article/details/gmdkkhvco.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.epnwcf.com/Article/details/gzwkhwwxf.sHtML

[B13] 判断是否为数字
来源：http://m.share.yfazqb.com/Article/details/gmovmxang.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.yfazqb.com/Article/details/gbrwmptcg.sHtML

PHP:  is_numeric($x)
来源：http://baike.bbcook.cn/Article/details/gooczfnkn.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.tarul.cn/Article/details/gkfmssoby.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.vehdjk.com/Article/details/glfviefer.sHtML

Java: x instanceof Number
来源：http://read.share.fktsv.cn/Article/details/gffhctftg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.sjlbkw.cn/Article/details/gnifcazka.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.sjlbkw.cn/Article/details/gjrkrvlry.sHtML

C#:   x is int or double or decimal
来源：http://wap.tarul.cn/Article/details/gcdlwzhsc.sHtML

[B14] 判断值是否在集合内
来源：http://wap.bbcook.cn/Article/details/ghoyixcij.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.yfazqb.com/Article/details/gacvijxnd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwpmypeio.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.sjlbkw.cn/Article/details/gbvzgyeow.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.epnwcf.com/Article/details/gakefoecs.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.epnwcf.com/Article/details/gqceandxe.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.epnwcf.com/Article/details/gvbbceako.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.yfazqb.com/Article/details/gswmrexed.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.epnwcf.com/Article/details/grdmzfjiz.sHtML

[B15] 布尔运算与取反
来源：http://blog.epnwcf.com/Article/details/gyxfxzurt.sHtML

Py:   a and b or not c
来源：http://wap.fktsv.cn/Article/details/gzuhevwce.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.vehdjk.com/Article/details/gyxjwqymy.sHtML

JS:   a && b || !c
来源：http://3g.yfazqb.com/Article/details/ggjbeuyww.sHtML

TS:   a && b || !c
来源：http://3g.fktsv.cn/Article/details/gaydoczhg.sHtML

Java: a && b || !c
来源：http://baike.vehdjk.com/Article/details/gblrrzfor.sHtML

Go:   a && b || !c
来源：http://read.share.epnwcf.com/Article/details/glighbihi.sHtML

Ruby: a && b || !c
来源：http://baike.yfazqb.com/Article/details/gqhdiosic.sHtML

C#:   a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gmkcrxzfn.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.tarul.cn/Article/details/gooimbrgq.sHtML

Py:   if not data: return
来源：http://www.m.share.vehdjk.com/Article/details/gzwvnfsxt.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.yfazqb.com/Article/details/gpnxwjsxb.sHtML

JS:   if (!data) return;
来源：http://3g.epnwcf.com/Article/details/gfzyfqgsd.sHtML

TS:   if (!data) return;
来源：http://m.share.tarul.cn/Article/details/gpibodxmq.sHtML

Java: if (data == null) return;
来源：http://mobile.sjlbkw.cn/Article/details/gegrqrwjk.sHtML

Go:   if data == nil { return }
来源：http://mobile.yfazqb.com/Article/details/gsbrhlbdg.sHtML

Ruby: return if data.nil?
来源：http://baike.yfazqb.com/Article/details/gkatorawn.sHtML

C#:   if (data == null) return;
来源：http://www.share.bbcook.cn/Article/details/glvlawlvz.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gtgbmymen.sHtML

C. 函数与作用域
来源：http://m.share.yfazqb.com/Article/details/gfihovhyx.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gobqfyiht.sHtML

[C01] 定义函数
来源：http://blog.fktsv.cn/Article/details/ghpmarokj.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.vehdjk.com/Article/details/gtbzwshas.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.yfazqb.com/Article/details/giorcseap.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/gsejvnrba.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.tarul.cn/Article/details/gcvuvzcnz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gsgwfvqta.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.tarul.cn/Article/details/gwwqwdiyf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fktsv.cn/Article/details/gprodrgtj.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/ghwmoecvv.sHtML

[C02] 默认参数
来源：http://www.blog.bbcook.cn/Article/details/gqevtqhxs.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fktsv.cn/Article/details/gufevuizn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gepbeuash.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.vehdjk.com/Article/details/gggcuhcrl.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.tarul.cn/Article/details/gtwxntods.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.sjlbkw.cn/Article/details/gdakcdjhs.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.yfazqb.com/Article/details/grlxbzoil.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.tarul.cn/Article/details/gmvxkyaau.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.epnwcf.com/Article/details/gmmcisnfp.sHtML

[C03] 可变参数
来源：http://mobile.yfazqb.com/Article/details/gijqybstv.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyrrblwrs.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.tarul.cn/Article/details/glmbsgfdo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fktsv.cn/Article/details/glzybidjw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.bbcook.cn/Article/details/gyvlcvlwk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.epnwcf.com/Article/details/gbcvmmqnh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fktsv.cn/Article/details/gqrbznpzb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.vehdjk.com/Article/details/gikkgdpoj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.tarul.cn/Article/details/grqcdkffj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.epnwcf.com/Article/details/gfgflnazw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.bbcook.cn/Article/details/gjafqxfsd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.epnwcf.com/Article/details/gokhgjvqu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.yfazqb.com/Article/details/ggpafvyvg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.yfazqb.com/Article/details/gbqbxkyrx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.sjlbkw.cn/Article/details/gnclkaihr.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.bbcook.cn/Article/details/gurqaejcp.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fktsv.cn/Article/details/guwdwljkk.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.tarul.cn/Article/details/gffukftjw.sHtML

[C05] 返回多个值
来源：http://mobile.sjlbkw.cn/Article/details/ghbwlrnxf.sHtML

Py:   return a, b
来源：http://blog.vehdjk.com/Article/details/gbrnhvobd.sHtML

PHP:  return [$a, $b];
来源：http://mobile.yfazqb.com/Article/details/gebwifllf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.vehdjk.com/Article/details/gtssfufny.sHtML

TS:   return { a, b };
来源：http://3g.vehdjk.com/Article/details/ggzumdsoo.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fktsv.cn/Article/details/gnsptxwtb.sHtML

Go:   return a, b
来源：http://www.blog.tarul.cn/Article/details/gwsvcwzrk.sHtML

Ruby: return a, b
来源：http://wap.fktsv.cn/Article/details/gyzcdkkzf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.tarul.cn/Article/details/gghwxlcaa.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.vehdjk.com/Article/details/ggwpbsbvk.sHtML

Py:   square = lambda x: x * x
来源：http://baike.bbcook.cn/Article/details/gbilolvtw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.yfazqb.com/Article/details/gpwtimevf.sHtML

JS:   const square = x => x * x;
来源：http://baike.vehdjk.com/Article/details/gleshxsbb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.sjlbkw.cn/Article/details/giogjcyin.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fktsv.cn/Article/details/gijsogoen.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.yfazqb.com/Article/details/guhcsbryl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fktsv.cn/Article/details/gqdyobfnz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.fktsv.cn/Article/details/glzetferb.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fktsv.cn/Article/details/gvwrjicea.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.yfazqb.com/Article/details/gatxyewmw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.tarul.cn/Article/details/groohytbv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fktsv.cn/Article/details/gudpoiqnu.sHtML

TS:   arr.map(String)
来源：http://m.share.sjlbkw.cn/Article/details/gpvfsykqj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.tarul.cn/Article/details/gkklkrhye.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.vehdjk.com/Article/details/gkcdrxhqa.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.bbcook.cn/Article/details/gbwusgjxh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.bbcook.cn/Article/details/gakmnzulm.sHtML

[C08] 闭包
来源：http://baike.tarul.cn/Article/details/gcewfhfjp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.sjlbkw.cn/Article/details/gdenmzsds.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.tarul.cn/Article/details/gvovfzqtq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.vehdjk.com/Article/details/ghibmdsgy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.bbcook.cn/Article/details/ghcstomje.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fktsv.cn/Article/details/gyjpnexxc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.vehdjk.com/Article/details/ggiwblcud.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fktsv.cn/Article/details/gcemyalvy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.tarul.cn/Article/details/gichpetpx.sHtML

[C09] 递归
来源：http://blog.fktsv.cn/Article/details/griwskxev.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.epnwcf.com/Article/details/gelgnnkun.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.epnwcf.com/Article/details/gxgjjtkwi.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.sjlbkw.cn/Article/details/gwatwxote.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.bbcook.cn/Article/details/glyramavx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fktsv.cn/Article/details/gxpdaxhvt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.tarul.cn/Article/details/gapjpnlel.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.sjlbkw.cn/Article/details/gvnbupvrk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.epnwcf.com/Article/details/gncqhsstn.sHtML

[C10] 变量作用域
来源：http://mobile.yfazqb.com/Article/details/gpqxwlqab.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.bbcook.cn/Article/details/goxoizlbd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.tarul.cn/Article/details/gpuvfzdhk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.yfazqb.com/Article/details/gwvxrnfum.sHtML

TS:   同 JS
来源：http://m.share.yfazqb.com/Article/details/gtbmmluyz.sHtML

Java: 方法内为块级作用域
来源：http://3g.fktsv.cn/Article/details/gnniprihv.sHtML

Go:   花括号块级作用域
来源：http://blog.vehdjk.com/Article/details/gsibkssno.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.vehdjk.com/Article/details/ggrsyltwn.sHtML

C#:   块级作用域
来源：http://www.share.yfazqb.com/Article/details/ggfeyriiw.sHtML

[C11] 模块导入与导出
来源：http://m.share.bbcook.cn/Article/details/glmndyngj.sHtML

Py:   from module import func
来源：http://3g.fktsv.cn/Article/details/gettcoewk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.bbcook.cn/Article/details/gozkutste.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.bbcook.cn/Article/details/gcnhjxpck.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.yfazqb.com/Article/details/gmjnyvfyp.sHtML

Java: import java.util.List;
来源：http://www.m.share.epnwcf.com/Article/details/gulacbald.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.epnwcf.com/Article/details/ggaovhtxk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.tarul.cn/Article/details/grbflonse.sHtML

C#:   using System.Text;
来源：http://blog.epnwcf.com/Article/details/gvlhjwplm.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.epnwcf.com/Article/details/goqnvhbfv.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.yfazqb.com/Article/details/grceazdmo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fktsv.cn/Article/details/gqkzjhwzj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.sjlbkw.cn/Article/details/ghmoifxsj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.tarul.cn/Article/details/gtcxnimwa.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.epnwcf.com/Article/details/graixaqim.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.yfazqb.com/Article/details/gzabezrrs.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.vehdjk.com/Article/details/gfwdsbqkk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fktsv.cn/Article/details/gkupvvndc.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.bbcook.cn/Article/details/gqvofaaac.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.epnwcf.com/Article/details/ganqfryfj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.vehdjk.com/Article/details/gidjjmsrs.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fktsv.cn/Article/details/gxodxiwou.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/gufbadxuc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gyjjvrhmj.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.bbcook.cn/Article/details/gpzoyczoz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fktsv.cn/Article/details/gkmnrudnf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.tarul.cn/Article/details/gvabtfjvx.sHtML

[C14] 泛型函数
来源：http://3g.sjlbkw.cn/Article/details/glthgljbv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.bbcook.cn/Article/details/ghpexwnio.sHtML

PHP:  // 无泛型
来源：http://baike.yfazqb.com/Article/details/guzlpekkz.sHtML

JS:   // 无泛型
来源：http://www.blog.yfazqb.com/Article/details/ghnjktqis.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.bbcook.cn/Article/details/grvospyve.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.vehdjk.com/Article/details/ggbdkacga.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.epnwcf.com/Article/details/gsxqxefvv.sHtML

Ruby: # 无泛型
来源：http://3g.bbcook.cn/Article/details/gubeumcfx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.epnwcf.com/Article/details/gjzkhnuam.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fktsv.cn/Article/details/gantxzruj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.epnwcf.com/Article/details/gopuwsetw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.sjlbkw.cn/Article/details/gobhvfqgk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.epnwcf.com/Article/details/gqgrwayme.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.bbcook.cn/Article/details/gojoepfns.sHtML

Java: // 无解构
来源：http://www.m.share.tarul.cn/Article/details/gtmajukyz.sHtML

Go:   // 无解构
来源：http://blog.tarul.cn/Article/details/gsiqihwua.sHtML

Ruby: a, b = pair
来源：http://wap.epnwcf.com/Article/details/gicdagezh.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.tarul.cn/Article/details/gdyolnqvu.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.sjlbkw.cn/Article/details/gpcvzqtqx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.yfazqb.com/Article/details/guounfcwh.sHtML

PHP:  // 无重载
来源：http://www.share.vehdjk.com/Article/details/gbyvlmzge.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.tarul.cn/Article/details/ghnhaiihe.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.sjlbkw.cn/Article/details/gwbbvkkfu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.yfazqb.com/Article/details/gbpiousqa.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fktsv.cn/Article/details/gymtjejax.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.epnwcf.com/Article/details/gmrfvkuea.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fktsv.cn/Article/details/ggqddnsmk.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gyqozmfvt.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fktsv.cn/Article/details/gsavxoler.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gnflfrxqs.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.epnwcf.com/Article/details/gpxfxenxw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.yfazqb.com/Article/details/gmxocoikr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.bbcook.cn/Article/details/gsmbpvgcl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.tarul.cn/Article/details/gqmoqmzxy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.yfazqb.com/Article/details/gspcfgijz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.epnwcf.com/Article/details/gmvacqaea.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.vehdjk.com/Article/details/gtalyqqdv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fktsv.cn/Article/details/gqnaotztg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.sjlbkw.cn/Article/details/grybsnbxq.sHtML

[D02] 追加元素到末尾
来源：http://blog.sjlbkw.cn/Article/details/gxtdbpakp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.sjlbkw.cn/Article/details/glonasuwl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.vehdjk.com/Article/details/gyfbnfift.sHtML

JS:   arr.push(4);
来源：http://baike.fktsv.cn/Article/details/gktjfqlst.sHtML

TS:   arr.push(4);
来源：http://wap.epnwcf.com/Article/details/gjqhuwkhs.sHtML

Java: list.add(4);
来源：http://mobile.yfazqb.com/Article/details/ghsdzhtmg.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.bbcook.cn/Article/details/ggapmvegl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.bbcook.cn/Article/details/goconmqjc.sHtML

C#:   list.Add(4);
来源：http://wap.tarul.cn/Article/details/gauhhvmfa.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gskuehdyr.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.tarul.cn/Article/details/gdhswwtdr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.tarul.cn/Article/details/gebyaizem.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.yfazqb.com/Article/details/gtjzegfhq.sHtML


<!-- 参考信息 -->