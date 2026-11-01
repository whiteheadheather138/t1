代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.bbcook.cn/Article/details/grstzhmdl.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.vehdjk.com/Article/details/gkmwrnpbp.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.sjlbkw.cn/Article/details/gxkrpcnuz.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.epnwcf.com/Article/details/ghwxiaekb.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.sjlbkw.cn/Article/details/gqflajxlp.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.yfazqb.com/Article/details/ggichlrln.sHtML

[B03] switch / match / case
来源：http://wap.sjlbkw.cn/Article/details/gfkhxagyq.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.fktsv.cn/Article/details/gdsmpzatk.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.vehdjk.com/Article/details/gjeyxqmoe.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.tarul.cn/Article/details/gatfnfznd.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.yfazqb.com/Article/details/gwdnllrki.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.bbcook.cn/Article/details/gionoygqo.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.yfazqb.com/Article/details/glorkeale.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.vehdjk.com/Article/details/gqqeezswo.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.sjlbkw.cn/Article/details/ggyzahwtb.sHtML

[B04] for 计数循环
来源：http://www.blog.bbcook.cn/Article/details/gioknsksk.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.vehdjk.com/Article/details/ggvtaojom.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.tarul.cn/Article/details/gfiwwpmvw.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.bbcook.cn/Article/details/gqfqtlpah.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.bbcook.cn/Article/details/gcjwueirv.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.fktsv.cn/Article/details/ghwsrwpji.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.bbcook.cn/Article/details/gcirvxsni.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.sjlbkw.cn/Article/details/guhgwszqq.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.epnwcf.com/Article/details/gmceupwrm.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.sjlbkw.cn/Article/details/gionqbzze.sHtML

Py:   for item in arr: print(item)
来源：http://wap.tarul.cn/Article/details/gltrpoecc.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.vehdjk.com/Article/details/gfpqjihhv.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.epnwcf.com/Article/details/gtvyaginz.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gulnetxyr.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.epnwcf.com/Article/details/gsnvwqrfu.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.yfazqb.com/Article/details/girqcuawy.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.yfazqb.com/Article/details/gnhmzapzc.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.yfazqb.com/Article/details/goybmnjek.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.yfazqb.com/Article/details/gymdjwdji.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.tarul.cn/Article/details/gzfscqidg.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.bbcook.cn/Article/details/gotkcfxec.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.vehdjk.com/Article/details/glepgoega.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fktsv.cn/Article/details/gluqjrvjv.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.tarul.cn/Article/details/gzgmdwjrt.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.tarul.cn/Article/details/gzxdmfmtr.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.epnwcf.com/Article/details/grpiaougu.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.vehdjk.com/Article/details/gxukxapxq.sHtML

[B07] while 循环
来源：http://mobile.tarul.cn/Article/details/golxhntvj.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fktsv.cn/Article/details/gmxvllrcc.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.fktsv.cn/Article/details/gnqkxhflv.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.tarul.cn/Article/details/gtlmhasgl.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.bbcook.cn/Article/details/grdzefkcs.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.fktsv.cn/Article/details/gxulwxqgf.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.yfazqb.com/Article/details/gqnpzpgyn.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.yfazqb.com/Article/details/gnjfpcvus.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.bbcook.cn/Article/details/gdmnriwzf.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.yfazqb.com/Article/details/gnyvgtilr.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.sjlbkw.cn/Article/details/gasfypmev.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.sjlbkw.cn/Article/details/gttotnzkr.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.yfazqb.com/Article/details/grizrzbrx.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.epnwcf.com/Article/details/gkcxiwoii.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.vehdjk.com/Article/details/gjtscnrid.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.fktsv.cn/Article/details/ghamxseyg.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.fktsv.cn/Article/details/gqkedwtph.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.tarul.cn/Article/details/gqfrlomgs.sHtML

[B09] break 与 continue
来源：http://3g.vehdjk.com/Article/details/goncjrozl.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.epnwcf.com/Article/details/gwuytrsll.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.sjlbkw.cn/Article/details/gcddhwaca.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.tarul.cn/Article/details/ggtogslyg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.sjlbkw.cn/Article/details/gumwvxesi.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fktsv.cn/Article/details/gxhooslis.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.yfazqb.com/Article/details/gsmwgnmqh.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.yfazqb.com/Article/details/gwuijwymh.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/gdmzbtdrw.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.sjlbkw.cn/Article/details/gnduffuly.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.epnwcf.com/Article/details/gtxqejwhh.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.epnwcf.com/Article/details/gwpcotafh.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.epnwcf.com/Article/details/gspekthog.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.yfazqb.com/Article/details/gobtszdfc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.sjlbkw.cn/Article/details/gvtbqhiap.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.bbcook.cn/Article/details/gtfewvfms.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.tarul.cn/Article/details/govdmrwcm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.sjlbkw.cn/Article/details/glghrooyl.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.bbcook.cn/Article/details/gotfsydak.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.yfazqb.com/Article/details/ggazzytfx.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.vehdjk.com/Article/details/gxudsktpc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.yfazqb.com/Article/details/gsakhkurz.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.bbcook.cn/Article/details/gzavhhhxq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.tarul.cn/Article/details/guzuevfvg.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.bbcook.cn/Article/details/gyrxemprz.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.yfazqb.com/Article/details/guhsowokk.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.epnwcf.com/Article/details/gsgnezkvi.sHtML

[B12] 跳出多层循环
来源：http://3g.fktsv.cn/Article/details/glrkqjbdn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.vehdjk.com/Article/details/gcqwrujdn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.fktsv.cn/Article/details/geqiedsqy.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.vehdjk.com/Article/details/gbeokaayu.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.vehdjk.com/Article/details/gjvdbmqie.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.bbcook.cn/Article/details/gpnrttehy.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.epnwcf.com/Article/details/gqmjhwuwv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fktsv.cn/Article/details/gvzqukwzp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.yfazqb.com/Article/details/ggmzboqop.sHtML

[B13] 判断是否为数字
来源：http://baike.sjlbkw.cn/Article/details/ghjyvcwbj.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.vehdjk.com/Article/details/gfimhrkyi.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.epnwcf.com/Article/details/gglmiumsf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.yfazqb.com/Article/details/gpjxikchp.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.tarul.cn/Article/details/govcjlqla.sHtML

Java: x instanceof Number
来源：http://blog.fktsv.cn/Article/details/gfkpbkost.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.bbcook.cn/Article/details/gzaamodal.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.epnwcf.com/Article/details/gdefasxvr.sHtML

C#:   x is int or double or decimal
来源：http://m.share.sjlbkw.cn/Article/details/giutvdizs.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.yfazqb.com/Article/details/gtbgyuojg.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.yfazqb.com/Article/details/gwanlpozu.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.bbcook.cn/Article/details/ggmvcnoyv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.bbcook.cn/Article/details/gkkjhiouh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.tarul.cn/Article/details/gfhxihxbt.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.sjlbkw.cn/Article/details/gniibjlab.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fktsv.cn/Article/details/gwlxuxnrc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.sjlbkw.cn/Article/details/gsqweclub.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.tarul.cn/Article/details/gbcapwsnp.sHtML

[B15] 布尔运算与取反
来源：http://mobile.epnwcf.com/Article/details/gjhtrmhcz.sHtML

Py:   a and b or not c
来源：http://read.share.sjlbkw.cn/Article/details/gvgcspimt.sHtML

PHP:  $a && $b || !$c
来源：http://wap.tarul.cn/Article/details/gqsgqvmro.sHtML

JS:   a && b || !c
来源：http://www.blog.tarul.cn/Article/details/gqvutslsq.sHtML

TS:   a && b || !c
来源：http://www.blog.sjlbkw.cn/Article/details/gewtekupf.sHtML

Java: a && b || !c
来源：http://mobile.yfazqb.com/Article/details/gzdwbpuvy.sHtML

Go:   a && b || !c
来源：http://3g.fktsv.cn/Article/details/gokdgcfnq.sHtML

Ruby: a && b || !c
来源：http://baike.tarul.cn/Article/details/gpeccgpiv.sHtML

C#:   a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gwnzuedaz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fktsv.cn/Article/details/gfamolxal.sHtML

Py:   if not data: return
来源：http://read.share.fktsv.cn/Article/details/gdrsfykab.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.tarul.cn/Article/details/gmpcghheh.sHtML

JS:   if (!data) return;
来源：http://baike.fktsv.cn/Article/details/gmevwpyma.sHtML

TS:   if (!data) return;
来源：http://www.blog.bbcook.cn/Article/details/grojrntfz.sHtML

Java: if (data == null) return;
来源：http://blog.epnwcf.com/Article/details/gscriitmj.sHtML

Go:   if data == nil { return }
来源：http://read.share.fktsv.cn/Article/details/gyefzncag.sHtML

Ruby: return if data.nil?
来源：http://read.share.sjlbkw.cn/Article/details/gmxgtswiy.sHtML

C#:   if (data == null) return;
来源：http://blog.tarul.cn/Article/details/gyadiptxp.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gfsghdxcy.sHtML

C. 函数与作用域
来源：http://www.m.share.epnwcf.com/Article/details/gkogwaxvf.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gjojxdvfz.sHtML

[C01] 定义函数
来源：http://m.share.fktsv.cn/Article/details/giitdhczw.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.sjlbkw.cn/Article/details/gcjotrjxw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.epnwcf.com/Article/details/guqryihvm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/gzemnvkwt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/giholcjzw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.vehdjk.com/Article/details/gsmmoehce.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.sjlbkw.cn/Article/details/gaclljguw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fktsv.cn/Article/details/gponfbjgy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gbjrdzeth.sHtML

[C02] 默认参数
来源：http://baike.yfazqb.com/Article/details/gbnjdjtff.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.epnwcf.com/Article/details/gsbaiufdq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.bbcook.cn/Article/details/goyeoclwy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.yfazqb.com/Article/details/gosgvcwqa.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.vehdjk.com/Article/details/ghzjmflbm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.vehdjk.com/Article/details/gevnjdfub.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.yfazqb.com/Article/details/gchrgcpqg.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.tarul.cn/Article/details/gdfvhoceu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fktsv.cn/Article/details/gwrkgirzg.sHtML

[C03] 可变参数
来源：http://m.share.tarul.cn/Article/details/grthrlxrm.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.tarul.cn/Article/details/goozvwtth.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.epnwcf.com/Article/details/gvvdjsspn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fktsv.cn/Article/details/gthfvpkeo.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.bbcook.cn/Article/details/gxmcffmom.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.yfazqb.com/Article/details/giyciibzd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.vehdjk.com/Article/details/gnwbajmfw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.bbcook.cn/Article/details/gcailniid.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.sjlbkw.cn/Article/details/gqlukhkbt.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.epnwcf.com/Article/details/guddttrka.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.epnwcf.com/Article/details/gxjnkfhto.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.bbcook.cn/Article/details/gxgmbfral.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.vehdjk.com/Article/details/geaompiem.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.yfazqb.com/Article/details/gjrajwbvf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.tarul.cn/Article/details/gzcygvubd.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fktsv.cn/Article/details/gizyqrdti.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.vehdjk.com/Article/details/gtembbrlj.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.vehdjk.com/Article/details/gezdjfijv.sHtML

[C05] 返回多个值
来源：http://wap.epnwcf.com/Article/details/gnlpwephr.sHtML

Py:   return a, b
来源：http://blog.fktsv.cn/Article/details/gvjjnaavh.sHtML

PHP:  return [$a, $b];
来源：http://wap.sjlbkw.cn/Article/details/gibmelklx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fktsv.cn/Article/details/gjkhnkqhh.sHtML

TS:   return { a, b };
来源：http://mobile.epnwcf.com/Article/details/gysnmpfwc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.tarul.cn/Article/details/ghqonexqo.sHtML

Go:   return a, b
来源：http://blog.tarul.cn/Article/details/gtrjwlqtu.sHtML

Ruby: return a, b
来源：http://wap.sjlbkw.cn/Article/details/ggiclczno.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.bbcook.cn/Article/details/gqagitwov.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.epnwcf.com/Article/details/ggcximbnk.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fktsv.cn/Article/details/gzphmegaq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.sjlbkw.cn/Article/details/guppbcwkt.sHtML

JS:   const square = x => x * x;
来源：http://wap.yfazqb.com/Article/details/gwkuxupgk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.bbcook.cn/Article/details/gfnvxnklg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.yfazqb.com/Article/details/gtwqiggel.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.epnwcf.com/Article/details/gixsyqhiu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.tarul.cn/Article/details/geyqzleuf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.sjlbkw.cn/Article/details/grywbrprc.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.sjlbkw.cn/Article/details/grguajarv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.yfazqb.com/Article/details/gftbnqshy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.sjlbkw.cn/Article/details/gormgfjwl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.yfazqb.com/Article/details/gignnubtp.sHtML

TS:   arr.map(String)
来源：http://3g.sjlbkw.cn/Article/details/gcphbqncs.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.yfazqb.com/Article/details/gvisupjpe.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.yfazqb.com/Article/details/gbmlrexoo.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.yfazqb.com/Article/details/geotqxqgy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.sjlbkw.cn/Article/details/gkgqbzeof.sHtML

[C08] 闭包
来源：http://wap.bbcook.cn/Article/details/gpsjknkhk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.vehdjk.com/Article/details/gitnhlvuc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.yfazqb.com/Article/details/gigbxxbmx.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.bbcook.cn/Article/details/guqcaamcc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.bbcook.cn/Article/details/gidxvodbd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.yfazqb.com/Article/details/gussvszeq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fktsv.cn/Article/details/gaipfmhwq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fktsv.cn/Article/details/gckjnlrlv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.vehdjk.com/Article/details/gxjwkbbhp.sHtML

[C09] 递归
来源：http://www.blog.yfazqb.com/Article/details/grtivsojx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.bbcook.cn/Article/details/gtelrpfuu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.bbcook.cn/Article/details/gjvxjdwfj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.sjlbkw.cn/Article/details/gdakrkuit.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fktsv.cn/Article/details/gilsxwbxn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.bbcook.cn/Article/details/gsypkoqnw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.epnwcf.com/Article/details/gmppcejlw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fktsv.cn/Article/details/ggekjblty.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fktsv.cn/Article/details/gbyyyespn.sHtML

[C10] 变量作用域
来源：http://www.blog.vehdjk.com/Article/details/gxgwmvudh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.sjlbkw.cn/Article/details/gusocrfdb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.epnwcf.com/Article/details/gpbdecwaq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.tarul.cn/Article/details/giuceohhg.sHtML

TS:   同 JS
来源：http://blog.sjlbkw.cn/Article/details/gbpziuebl.sHtML

Java: 方法内为块级作用域
来源：http://baike.sjlbkw.cn/Article/details/gcpgldvqm.sHtML

Go:   花括号块级作用域
来源：http://wap.sjlbkw.cn/Article/details/gbwoelrak.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.vehdjk.com/Article/details/gnraemwdc.sHtML

C#:   块级作用域
来源：http://m.share.vehdjk.com/Article/details/gyejxzhdo.sHtML

[C11] 模块导入与导出
来源：http://wap.sjlbkw.cn/Article/details/gemkxkspj.sHtML

Py:   from module import func
来源：http://baike.epnwcf.com/Article/details/gnuzqzncc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.yfazqb.com/Article/details/ghabggqkt.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.sjlbkw.cn/Article/details/gkzwfhalo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.vehdjk.com/Article/details/ggmbhnxcv.sHtML

Java: import java.util.List;
来源：http://3g.fktsv.cn/Article/details/gzwggnhgz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.yfazqb.com/Article/details/glcxofddw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.tarul.cn/Article/details/gmhsgqtpw.sHtML

C#:   using System.Text;
来源：http://read.share.vehdjk.com/Article/details/gtfzqifxx.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.tarul.cn/Article/details/ghyucuchb.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.sjlbkw.cn/Article/details/gkbeebyqx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.tarul.cn/Article/details/gneyxkuun.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.tarul.cn/Article/details/gwobtjtxo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fktsv.cn/Article/details/gbzxtdaku.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.epnwcf.com/Article/details/gbbcomgwp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.epnwcf.com/Article/details/gdzqttymu.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.sjlbkw.cn/Article/details/givhzplgq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.vehdjk.com/Article/details/gxlnjundq.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.tarul.cn/Article/details/ggbtvwnjj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.yfazqb.com/Article/details/gpacxfjkw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.sjlbkw.cn/Article/details/gikhchhvn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.sjlbkw.cn/Article/details/gsxndpimm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gjsclhgzq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gnqzkloog.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.sjlbkw.cn/Article/details/gmflwzkui.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.vehdjk.com/Article/details/ggepfdolj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.vehdjk.com/Article/details/gjnxfjrsm.sHtML

[C14] 泛型函数
来源：http://blog.tarul.cn/Article/details/grfkpbvkr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.bbcook.cn/Article/details/gmazwdyub.sHtML

PHP:  // 无泛型
来源：http://baike.yfazqb.com/Article/details/gfacdngst.sHtML

JS:   // 无泛型
来源：http://m.share.fktsv.cn/Article/details/gytydatdn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.vehdjk.com/Article/details/gsuvdcxhs.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fktsv.cn/Article/details/gyhpnmbzx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fktsv.cn/Article/details/gmevhkdum.sHtML

Ruby: # 无泛型
来源：http://read.share.sjlbkw.cn/Article/details/ggsglnfsi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.sjlbkw.cn/Article/details/gviuipnhj.sHtML

[C15] 解构 / 展开参数
来源：http://3g.vehdjk.com/Article/details/gnnznkxla.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.bbcook.cn/Article/details/gxqjzyxht.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.bbcook.cn/Article/details/gaabzhwau.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.sjlbkw.cn/Article/details/gbnaguohg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fktsv.cn/Article/details/gcyfluedb.sHtML

Java: // 无解构
来源：http://www.m.share.sjlbkw.cn/Article/details/gzoarsotj.sHtML

Go:   // 无解构
来源：http://m.share.fktsv.cn/Article/details/gsazklfzv.sHtML

Ruby: a, b = pair
来源：http://baike.tarul.cn/Article/details/gbkgakzjd.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fktsv.cn/Article/details/ggtybdifp.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.epnwcf.com/Article/details/ggmgtvjkl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.sjlbkw.cn/Article/details/gooztidrp.sHtML

PHP:  // 无重载
来源：http://www.m.share.bbcook.cn/Article/details/gsdowqpwo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.bbcook.cn/Article/details/gthooslux.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.tarul.cn/Article/details/giaxriaew.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.epnwcf.com/Article/details/gmptfawyq.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.bbcook.cn/Article/details/goysyyrjp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.sjlbkw.cn/Article/details/ggkatqivr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.bbcook.cn/Article/details/gbenxyxkq.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gzbybnrwd.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.tarul.cn/Article/details/grdpbgjjn.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gcdzqqizr.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.vehdjk.com/Article/details/gnpjbtunq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.tarul.cn/Article/details/glzpiuohf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.epnwcf.com/Article/details/gqynosopt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.epnwcf.com/Article/details/giynqgtpa.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fktsv.cn/Article/details/gewnlcmog.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.bbcook.cn/Article/details/gbkvdbgpj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.bbcook.cn/Article/details/ghfasiadd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.bbcook.cn/Article/details/gajbgdqdp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.vehdjk.com/Article/details/ghogqmbav.sHtML

[D02] 追加元素到末尾
来源：http://blog.vehdjk.com/Article/details/goxdskcyv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.bbcook.cn/Article/details/gzqgpilgk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.bbcook.cn/Article/details/gzxuobtzq.sHtML

JS:   arr.push(4);
来源：http://mobile.bbcook.cn/Article/details/gufjpaygi.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fktsv.cn/Article/details/goiawfimd.sHtML

Java: list.add(4);
来源：http://3g.bbcook.cn/Article/details/ggsszokws.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.tarul.cn/Article/details/gdmovqaoj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.bbcook.cn/Article/details/gmdyshqmq.sHtML

C#:   list.Add(4);
来源：http://mobile.epnwcf.com/Article/details/gdmptaxbs.sHtML


<!-- 参考信息 -->