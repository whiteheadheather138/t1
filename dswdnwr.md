代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.yfazqb.com/Article/details/gkicvnfya.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.sjlbkw.cn/Article/details/gbipdtdil.sHtML

[B03] switch / match / case
来源：http://www.m.share.tarul.cn/Article/details/gqbyrokzd.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.sjlbkw.cn/Article/details/gsdblgnmm.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.epnwcf.com/Article/details/gicrfkrws.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.bbcook.cn/Article/details/gbmqdtqbb.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.yfazqb.com/Article/details/gvtqklwbc.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.epnwcf.com/Article/details/guzzksrej.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.fktsv.cn/Article/details/gcmiqvjji.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.bbcook.cn/Article/details/gmmodtjbv.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.tarul.cn/Article/details/ghfwoldzt.sHtML

[B04] for 计数循环
来源：http://www.m.share.tarul.cn/Article/details/ggyzcfhlg.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.tarul.cn/Article/details/gxvzvxqdw.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.bbcook.cn/Article/details/gxxvrbixa.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.tarul.cn/Article/details/gcpsqoiiy.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.tarul.cn/Article/details/gypeltctj.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.epnwcf.com/Article/details/gcdlnxnwq.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.fktsv.cn/Article/details/ggckdkwrr.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.vehdjk.com/Article/details/gmrsnrlds.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.vehdjk.com/Article/details/gxkabisql.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.tarul.cn/Article/details/gzccjvusn.sHtML

Py:   for item in arr: print(item)
来源：http://blog.fktsv.cn/Article/details/ghjloniet.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.fktsv.cn/Article/details/gdyoebmal.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.yfazqb.com/Article/details/gzeaiqdxb.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.yfazqb.com/Article/details/gqeifcmge.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.yfazqb.com/Article/details/gxqqmbcvi.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.fktsv.cn/Article/details/gbknalwdy.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.fktsv.cn/Article/details/gtakzrlvo.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.fktsv.cn/Article/details/galgsaajz.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.vehdjk.com/Article/details/gcmawamze.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.tarul.cn/Article/details/ginnunlsi.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.sjlbkw.cn/Article/details/gjihovqvh.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.vehdjk.com/Article/details/gwexoblev.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.yfazqb.com/Article/details/gfiyvirtv.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.yfazqb.com/Article/details/gcvxjkxii.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.tarul.cn/Article/details/grunkffvk.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvkkswxcs.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.vehdjk.com/Article/details/gvubfxyee.sHtML

[B07] while 循环
来源：http://m.share.sjlbkw.cn/Article/details/gcwnnpozp.sHtML

Py:   while i < 10: i += 1
来源：http://blog.epnwcf.com/Article/details/gsjjulozu.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.vehdjk.com/Article/details/gpsepystn.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.tarul.cn/Article/details/gfoqidhho.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.fktsv.cn/Article/details/grqrswthe.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.yfazqb.com/Article/details/gsbjqieaq.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.bbcook.cn/Article/details/guoghzyvc.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.epnwcf.com/Article/details/gqyfjmnlq.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.fktsv.cn/Article/details/gergqgsys.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.vehdjk.com/Article/details/getjqdsjb.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.bbcook.cn/Article/details/ghlodsxgp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.vehdjk.com/Article/details/gwbbfasou.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.yfazqb.com/Article/details/gmnodgskd.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.epnwcf.com/Article/details/gearzgngo.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.tarul.cn/Article/details/gzbqrrvrl.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.tarul.cn/Article/details/gkzdwqsgw.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.yfazqb.com/Article/details/gglfxnukq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.epnwcf.com/Article/details/gxufipksn.sHtML

[B09] break 与 continue
来源：http://baike.epnwcf.com/Article/details/gsboylagf.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.bbcook.cn/Article/details/gqekffxar.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/gsoaubfsz.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/gyprtghui.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.epnwcf.com/Article/details/gcbxpqciv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.tarul.cn/Article/details/gyfylvyoo.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.epnwcf.com/Article/details/gpihcnulw.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.yfazqb.com/Article/details/gsdihlrai.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.tarul.cn/Article/details/gfhpercxt.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.epnwcf.com/Article/details/gnwfwnmvt.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.bbcook.cn/Article/details/ganggahki.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.sjlbkw.cn/Article/details/gyqafrlev.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.tarul.cn/Article/details/grrwptrcj.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.tarul.cn/Article/details/grxtdiaob.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.sjlbkw.cn/Article/details/geokrvaik.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fktsv.cn/Article/details/gwgwjuxip.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.vehdjk.com/Article/details/guxnbvbco.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.vehdjk.com/Article/details/grbhmvjnz.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.yfazqb.com/Article/details/gomufnvvi.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.bbcook.cn/Article/details/gdyurhvyx.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.vehdjk.com/Article/details/gvypffgha.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.tarul.cn/Article/details/gqkacfmuh.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.bbcook.cn/Article/details/gwlidxyoi.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.vehdjk.com/Article/details/guhzozrmb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.bbcook.cn/Article/details/grhpbzrqd.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.yfazqb.com/Article/details/ghwcpqpdr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.vehdjk.com/Article/details/gaflapycm.sHtML

[B12] 跳出多层循环
来源：http://baike.yfazqb.com/Article/details/gqgzsdkss.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fktsv.cn/Article/details/gbyfasezh.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.bbcook.cn/Article/details/gkmpmprwm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.yfazqb.com/Article/details/ghuxbonwy.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fktsv.cn/Article/details/gxbceqfdj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.tarul.cn/Article/details/gpwipmlny.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.yfazqb.com/Article/details/gnqmzwhyk.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.bbcook.cn/Article/details/gdefqyueb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.sjlbkw.cn/Article/details/gxmnrzovr.sHtML

[B13] 判断是否为数字
来源：http://read.share.vehdjk.com/Article/details/gqlzpwjpr.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.yfazqb.com/Article/details/ghqiyhlag.sHtML

PHP:  is_numeric($x)
来源：http://3g.bbcook.cn/Article/details/ghmitreus.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.vehdjk.com/Article/details/gutrqmtcd.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.vehdjk.com/Article/details/gjqpunhxd.sHtML

Java: x instanceof Number
来源：http://wap.yfazqb.com/Article/details/gximntczd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.yfazqb.com/Article/details/gajhaevut.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.yfazqb.com/Article/details/ggjexeooa.sHtML

C#:   x is int or double or decimal
来源：http://wap.fktsv.cn/Article/details/gzbxtftzn.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.epnwcf.com/Article/details/gmwytwztu.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.vehdjk.com/Article/details/ggfxzlodz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.vehdjk.com/Article/details/gzpdqrsfm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.yfazqb.com/Article/details/gyknmnkvw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.tarul.cn/Article/details/gazvrfhoy.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.vehdjk.com/Article/details/gnivczfxb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.vehdjk.com/Article/details/ggctaixxk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.epnwcf.com/Article/details/gvpkpzvum.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.yfazqb.com/Article/details/gttonmmff.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.fktsv.cn/Article/details/ghtoxkchy.sHtML

Py:   a and b or not c
来源：http://wap.bbcook.cn/Article/details/gqrgepiil.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.bbcook.cn/Article/details/gdomlelkh.sHtML

JS:   a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/gzzobavaj.sHtML

TS:   a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gdvxutqeq.sHtML

Java: a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gtnwgppuo.sHtML

Go:   a && b || !c
来源：http://blog.fktsv.cn/Article/details/ghubovdwa.sHtML

Ruby: a && b || !c
来源：http://www.share.fktsv.cn/Article/details/gazrftwuk.sHtML

C#:   a && b || !c
来源：http://mobile.bbcook.cn/Article/details/gchdfpjoe.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.bbcook.cn/Article/details/ggxqejyzz.sHtML

Py:   if not data: return
来源：http://www.blog.fktsv.cn/Article/details/ggbwhxvgg.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.vehdjk.com/Article/details/gwcildpii.sHtML

JS:   if (!data) return;
来源：http://www.share.bbcook.cn/Article/details/gyqnaivdh.sHtML

TS:   if (!data) return;
来源：http://www.m.share.epnwcf.com/Article/details/gerhrhglg.sHtML

Java: if (data == null) return;
来源：http://mobile.tarul.cn/Article/details/gfyvcgzll.sHtML

Go:   if data == nil { return }
来源：http://read.share.tarul.cn/Article/details/gsepywbix.sHtML

Ruby: return if data.nil?
来源：http://m.share.fktsv.cn/Article/details/grbafcqof.sHtML

C#:   if (data == null) return;
来源：http://3g.epnwcf.com/Article/details/gqutzlawu.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gtcxcdljw.sHtML

C. 函数与作用域
来源：http://mobile.vehdjk.com/Article/details/gybofkcov.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gvzlkcfth.sHtML

[C01] 定义函数
来源：http://read.share.sjlbkw.cn/Article/details/ggtnbgnaj.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.yfazqb.com/Article/details/gdsphwech.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.vehdjk.com/Article/details/gviqmoacv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.tarul.cn/Article/details/gyorcxcyd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.sjlbkw.cn/Article/details/gnprpzuiw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/gipmmpotb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.yfazqb.com/Article/details/ggjpmqsew.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.sjlbkw.cn/Article/details/gsnyxysab.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.tarul.cn/Article/details/gxpcrjibk.sHtML

[C02] 默认参数
来源：http://baike.sjlbkw.cn/Article/details/gklnokzlt.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.tarul.cn/Article/details/gdmljldmf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.epnwcf.com/Article/details/gxlxhttcd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.yfazqb.com/Article/details/guypfwupj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.yfazqb.com/Article/details/gskirqprt.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.bbcook.cn/Article/details/gcwvlmjjp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.epnwcf.com/Article/details/gfgcvsvta.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.tarul.cn/Article/details/geagvlfuv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.tarul.cn/Article/details/gqzinwejb.sHtML

[C03] 可变参数
来源：http://www.m.share.sjlbkw.cn/Article/details/ghofgupem.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.epnwcf.com/Article/details/giqofxyvv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.yfazqb.com/Article/details/gnkcwulnn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.bbcook.cn/Article/details/gxydjvhgq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.vehdjk.com/Article/details/gdeuqrxqi.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.sjlbkw.cn/Article/details/gytfspafw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.yfazqb.com/Article/details/gcncvkjhj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.vehdjk.com/Article/details/gfjxakmey.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.tarul.cn/Article/details/gtboyiyhx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.yfazqb.com/Article/details/gaisjbeqr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.bbcook.cn/Article/details/ghibargma.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.bbcook.cn/Article/details/gyjmxbrjp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.epnwcf.com/Article/details/gbmfncwar.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.bbcook.cn/Article/details/ghrsdopib.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.bbcook.cn/Article/details/guwiqjkpx.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.yfazqb.com/Article/details/gppvpcokt.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.yfazqb.com/Article/details/gjobsvtgx.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.bbcook.cn/Article/details/gmeweusvv.sHtML

[C05] 返回多个值
来源：http://baike.yfazqb.com/Article/details/gxymcgyhf.sHtML

Py:   return a, b
来源：http://www.blog.sjlbkw.cn/Article/details/gaadzqltl.sHtML

PHP:  return [$a, $b];
来源：http://m.share.bbcook.cn/Article/details/gchejqtbo.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.epnwcf.com/Article/details/gttzdduxm.sHtML

TS:   return { a, b };
来源：http://blog.sjlbkw.cn/Article/details/gphidozye.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.tarul.cn/Article/details/gbfzqsrei.sHtML

Go:   return a, b
来源：http://blog.sjlbkw.cn/Article/details/gteiyzjxy.sHtML

Ruby: return a, b
来源：http://wap.bbcook.cn/Article/details/gthcvrugd.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.epnwcf.com/Article/details/gsavyjvwp.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.bbcook.cn/Article/details/gkbkgvrkt.sHtML

Py:   square = lambda x: x * x
来源：http://wap.bbcook.cn/Article/details/ggzupxegr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.vehdjk.com/Article/details/gvtngjnsc.sHtML

JS:   const square = x => x * x;
来源：http://3g.epnwcf.com/Article/details/ghwmjkwus.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.epnwcf.com/Article/details/ghfzguofg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fktsv.cn/Article/details/gcdlxqxda.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.yfazqb.com/Article/details/gczrlsxcp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.yfazqb.com/Article/details/gzuuianqj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fktsv.cn/Article/details/gtwqtaziw.sHtML

[C07] 把函数作为参数传入
来源：http://wap.sjlbkw.cn/Article/details/gngsgcycg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.fktsv.cn/Article/details/grhhgrwrr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fktsv.cn/Article/details/gzcveemsa.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.sjlbkw.cn/Article/details/gohzviuec.sHtML

TS:   arr.map(String)
来源：http://m.share.tarul.cn/Article/details/gzpgzqusg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.yfazqb.com/Article/details/gdohzflky.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.vehdjk.com/Article/details/ghpcggarw.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.tarul.cn/Article/details/gnjukzntr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fktsv.cn/Article/details/gagqydawg.sHtML

[C08] 闭包
来源：http://mobile.fktsv.cn/Article/details/ggdjnzvfa.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.sjlbkw.cn/Article/details/geusvkcqy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.tarul.cn/Article/details/gueheqgag.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.yfazqb.com/Article/details/gaqgusmbq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.vehdjk.com/Article/details/gngtzzodr.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.tarul.cn/Article/details/gxhllwhsl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.vehdjk.com/Article/details/gergdgknl.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.epnwcf.com/Article/details/gkwqawgdr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.bbcook.cn/Article/details/gwodvuzkf.sHtML

[C09] 递归
来源：http://mobile.fktsv.cn/Article/details/gywiluuve.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.tarul.cn/Article/details/gjzglktxu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fktsv.cn/Article/details/gqfuoinix.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.bbcook.cn/Article/details/gpmjghabb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.vehdjk.com/Article/details/gjppwnsrf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.tarul.cn/Article/details/ggupeghgx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.tarul.cn/Article/details/gzwdihaxl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fktsv.cn/Article/details/gzrxroprr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.tarul.cn/Article/details/gtdagdglz.sHtML

[C10] 变量作用域
来源：http://www.share.bbcook.cn/Article/details/gexaumwhb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.bbcook.cn/Article/details/gmkkvppnb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.sjlbkw.cn/Article/details/gmlsycxig.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.yfazqb.com/Article/details/gqzlxkxmm.sHtML

TS:   同 JS
来源：http://wap.sjlbkw.cn/Article/details/gdrarwmll.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fktsv.cn/Article/details/guqrwwkwl.sHtML

Go:   花括号块级作用域
来源：http://read.share.sjlbkw.cn/Article/details/gqcwsyrub.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.vehdjk.com/Article/details/gbhyorsmn.sHtML

C#:   块级作用域
来源：http://m.share.fktsv.cn/Article/details/gtkwypbkz.sHtML

[C11] 模块导入与导出
来源：http://3g.tarul.cn/Article/details/gejictezw.sHtML

Py:   from module import func
来源：http://3g.fktsv.cn/Article/details/gzahcnqnp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.sjlbkw.cn/Article/details/gitdwndyi.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.vehdjk.com/Article/details/gfejrnjrd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fktsv.cn/Article/details/grluwhpnt.sHtML

Java: import java.util.List;
来源：http://read.share.bbcook.cn/Article/details/gomkywwti.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.sjlbkw.cn/Article/details/grpujhbkm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.epnwcf.com/Article/details/gfbtpvuss.sHtML

C#:   using System.Text;
来源：http://www.share.epnwcf.com/Article/details/gzuupypra.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fktsv.cn/Article/details/gwhogqogx.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.yfazqb.com/Article/details/gyvelnyds.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fktsv.cn/Article/details/gxbevonmc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fktsv.cn/Article/details/gbxfitjdp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.bbcook.cn/Article/details/gfvutfzyw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.epnwcf.com/Article/details/gmvfnavqg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.bbcook.cn/Article/details/gvhnvqgte.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.tarul.cn/Article/details/gefifruoj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.tarul.cn/Article/details/gavcdjxvh.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.epnwcf.com/Article/details/gxkerfddi.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.fktsv.cn/Article/details/gawvuwgpg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.vehdjk.com/Article/details/gpkwqpdfg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.tarul.cn/Article/details/gojzbcbzf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/ggkflqthe.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gkpigmuil.sHtML

Go:   func add(a, b int) int
来源：http://www.share.tarul.cn/Article/details/ggsczebga.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.vehdjk.com/Article/details/gvmdzoskx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.bbcook.cn/Article/details/gxyiyvwzb.sHtML

[C14] 泛型函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gmfdxgrns.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.yfazqb.com/Article/details/gsehtngpq.sHtML

PHP:  // 无泛型
来源：http://www.blog.bbcook.cn/Article/details/gaojphpui.sHtML

JS:   // 无泛型
来源：http://mobile.yfazqb.com/Article/details/gowfmisiq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.vehdjk.com/Article/details/geaefmwer.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.tarul.cn/Article/details/gyslmvbrw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.sjlbkw.cn/Article/details/grtrmekgp.sHtML

Ruby: # 无泛型
来源：http://www.share.tarul.cn/Article/details/gzyijcctj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.fktsv.cn/Article/details/ggkzwjgrc.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fktsv.cn/Article/details/gbcjisgti.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.sjlbkw.cn/Article/details/gkpglmbhv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.tarul.cn/Article/details/gjzmkzhtx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.epnwcf.com/Article/details/gazdtpovk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.yfazqb.com/Article/details/ghnqtcgth.sHtML

Java: // 无解构
来源：http://baike.vehdjk.com/Article/details/glpgmehmf.sHtML

Go:   // 无解构
来源：http://m.share.vehdjk.com/Article/details/gfmltdgbi.sHtML

Ruby: a, b = pair
来源：http://mobile.sjlbkw.cn/Article/details/gixbxoutl.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.yfazqb.com/Article/details/gsuwjbezq.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fktsv.cn/Article/details/gocrdmhvb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.tarul.cn/Article/details/ggdfywwhy.sHtML

PHP:  // 无重载
来源：http://read.share.bbcook.cn/Article/details/glvkbewzn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.bbcook.cn/Article/details/gsncfcxcn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.tarul.cn/Article/details/gidivwczs.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.yfazqb.com/Article/details/ggwjsoumx.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.tarul.cn/Article/details/glrenlbkq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.bbcook.cn/Article/details/ghyavawye.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.sjlbkw.cn/Article/details/gykcptjng.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gnwztxsln.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.epnwcf.com/Article/details/gfrpetesl.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gooqjbyoi.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fktsv.cn/Article/details/gcrqilots.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.yfazqb.com/Article/details/gognfzngg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.bbcook.cn/Article/details/gddvpxiya.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.bbcook.cn/Article/details/ggnwnycyp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.vehdjk.com/Article/details/gxvlvazxk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fktsv.cn/Article/details/gyhanaoiv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.tarul.cn/Article/details/gwotkfcjs.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.tarul.cn/Article/details/gaxsunftx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.yfazqb.com/Article/details/gmkdgklrw.sHtML

[D02] 追加元素到末尾
来源：http://www.share.sjlbkw.cn/Article/details/gredrstas.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.epnwcf.com/Article/details/gecmnsuio.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.tarul.cn/Article/details/gefbnirsf.sHtML

JS:   arr.push(4);
来源：http://www.m.share.tarul.cn/Article/details/gsbhoqrqo.sHtML

TS:   arr.push(4);
来源：http://blog.yfazqb.com/Article/details/gugsvpnkz.sHtML

Java: list.add(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjbuovevq.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.bbcook.cn/Article/details/gmjtrdedh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.tarul.cn/Article/details/gfxofqari.sHtML

C#:   list.Add(4);
来源：http://www.share.vehdjk.com/Article/details/gfkqurbct.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fktsv.cn/Article/details/gastnyxif.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.vehdjk.com/Article/details/gfvcwjxnw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.epnwcf.com/Article/details/gghwcvemq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.bbcook.cn/Article/details/gcjxodfjm.sHtML


<!-- 参考信息 -->