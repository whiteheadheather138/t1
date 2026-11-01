代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.vehdjk.com/Article/details/gcpulovwp.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.bbcook.cn/Article/details/gshuofcdl.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.fktsv.cn/Article/details/gztwqmgpv.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.vehdjk.com/Article/details/gkptwyqrr.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.sjlbkw.cn/Article/details/ghdjbzrga.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.tarul.cn/Article/details/gdnmtxmep.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.sjlbkw.cn/Article/details/gmfplnpxn.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.bbcook.cn/Article/details/galjbufgx.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.vehdjk.com/Article/details/gjvcismnt.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.sjlbkw.cn/Article/details/ghfkpmsef.sHtML

[B03] switch / match / case
来源：http://www.blog.sjlbkw.cn/Article/details/gbidzhatq.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.yfazqb.com/Article/details/gabagqcir.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.epnwcf.com/Article/details/ggpwntkzh.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.vehdjk.com/Article/details/gyjqutepe.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fktsv.cn/Article/details/gxiaqbmdk.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.yfazqb.com/Article/details/gqwpqcdbv.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.tarul.cn/Article/details/gxngcyuth.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.yfazqb.com/Article/details/gugdfaihk.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.sjlbkw.cn/Article/details/gczvwmsau.sHtML

[B04] for 计数循环
来源：http://mobile.vehdjk.com/Article/details/gmxhumtsj.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.epnwcf.com/Article/details/gajsvchbm.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.bbcook.cn/Article/details/gboqvbdgd.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.tarul.cn/Article/details/gguvegago.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.epnwcf.com/Article/details/ghqczxcdk.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.epnwcf.com/Article/details/gafbphzxy.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.bbcook.cn/Article/details/goelxoebg.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.epnwcf.com/Article/details/gpavjkqtt.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.epnwcf.com/Article/details/grxavhnpr.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.tarul.cn/Article/details/ggwrupwou.sHtML

Py:   for item in arr: print(item)
来源：http://blog.epnwcf.com/Article/details/gwuyqhyzy.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.epnwcf.com/Article/details/gzhvuikbc.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.bbcook.cn/Article/details/ggnygeizr.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.tarul.cn/Article/details/gixzxkxqw.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.bbcook.cn/Article/details/gfcmqtwcp.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.epnwcf.com/Article/details/gpyovppei.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.yfazqb.com/Article/details/gdxdzrgsw.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.sjlbkw.cn/Article/details/glzftjzeg.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.yfazqb.com/Article/details/gevpmtiah.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.sjlbkw.cn/Article/details/godwpzvac.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.vehdjk.com/Article/details/gomredefz.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.vehdjk.com/Article/details/gdssypjsw.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.vehdjk.com/Article/details/ggkihfmxk.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdapxfolq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.epnwcf.com/Article/details/gibduvqrx.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.vehdjk.com/Article/details/gneuypoom.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.fktsv.cn/Article/details/grmxdznkc.sHtML

[B07] while 循环
来源：http://m.share.yfazqb.com/Article/details/grthqtvrv.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.yfazqb.com/Article/details/gtmeptfdg.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.tarul.cn/Article/details/gibbajuyc.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.epnwcf.com/Article/details/gkwztnrhz.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.vehdjk.com/Article/details/gyoxkiisq.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.sjlbkw.cn/Article/details/gclsgeckh.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.bbcook.cn/Article/details/gamhqzsod.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.fktsv.cn/Article/details/gqspeuluw.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.fktsv.cn/Article/details/gwweswpqw.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.yfazqb.com/Article/details/gerivmvep.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.tarul.cn/Article/details/gbuvuskwu.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.tarul.cn/Article/details/gefhedpuz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.yfazqb.com/Article/details/gyqhddmqq.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.fktsv.cn/Article/details/gfqgressw.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.bbcook.cn/Article/details/gqlbvywxe.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.epnwcf.com/Article/details/gvhgtbwuy.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.bbcook.cn/Article/details/gqiiutvsy.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.epnwcf.com/Article/details/gyymrdcbc.sHtML

[B09] break 与 continue
来源：http://read.share.epnwcf.com/Article/details/gkbgetlvl.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.fktsv.cn/Article/details/gyhkkwmke.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.fktsv.cn/Article/details/gphnuqiro.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.sjlbkw.cn/Article/details/gaunygmft.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.sjlbkw.cn/Article/details/gxzzdyxfw.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.epnwcf.com/Article/details/gzwqjtjmn.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.fktsv.cn/Article/details/gxdexnrxy.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.yfazqb.com/Article/details/gtpeiqerq.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.bbcook.cn/Article/details/gcbuyttxq.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.bbcook.cn/Article/details/gmxuvzlmn.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.fktsv.cn/Article/details/gqsvkkdpw.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.epnwcf.com/Article/details/gayukzbhg.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.sjlbkw.cn/Article/details/gkxsxeeyt.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.epnwcf.com/Article/details/gubsbkfyt.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.sjlbkw.cn/Article/details/gkllqjwjz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.fktsv.cn/Article/details/gimdgtkrl.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.tarul.cn/Article/details/glghmqvdt.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.yfazqb.com/Article/details/gnihhttsi.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.fktsv.cn/Article/details/giffrhllx.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.yfazqb.com/Article/details/gawvdqscx.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.bbcook.cn/Article/details/gyvjirlww.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fktsv.cn/Article/details/gejdcxesb.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.epnwcf.com/Article/details/gkluvwbii.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.tarul.cn/Article/details/gcovecbqu.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.vehdjk.com/Article/details/gqqshwpcm.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.tarul.cn/Article/details/gwrcyasez.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.bbcook.cn/Article/details/gbgqqglhw.sHtML

[B12] 跳出多层循环
来源：http://blog.vehdjk.com/Article/details/gctryvvmr.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.sjlbkw.cn/Article/details/gewnkcesw.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.sjlbkw.cn/Article/details/gcagzfpfi.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fktsv.cn/Article/details/giisahjms.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.yfazqb.com/Article/details/gqafgsiyi.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.bbcook.cn/Article/details/gugbljrij.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.yfazqb.com/Article/details/gaejximna.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.bbcook.cn/Article/details/gknizbzbp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.bbcook.cn/Article/details/gftxdhbyd.sHtML

[B13] 判断是否为数字
来源：http://mobile.sjlbkw.cn/Article/details/glpgcaxos.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.sjlbkw.cn/Article/details/gttxhtzrr.sHtML

PHP:  is_numeric($x)
来源：http://3g.yfazqb.com/Article/details/gobzfommr.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fktsv.cn/Article/details/gkylxbduk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.yfazqb.com/Article/details/gwlrnwcoy.sHtML

Java: x instanceof Number
来源：http://www.m.share.vehdjk.com/Article/details/gdrfoaugz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.yfazqb.com/Article/details/gpahtansh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.yfazqb.com/Article/details/gkghfzhrf.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.sjlbkw.cn/Article/details/ggqxnpoom.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.fktsv.cn/Article/details/gbcnqxooo.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.sjlbkw.cn/Article/details/ghkrrwozz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.tarul.cn/Article/details/gpbgsqzky.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.yfazqb.com/Article/details/gododtvwg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.bbcook.cn/Article/details/garphzbso.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.bbcook.cn/Article/details/gcyaqsfkp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.yfazqb.com/Article/details/gruzobcaq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gzogzleyi.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fktsv.cn/Article/details/gssdblhry.sHtML

[B15] 布尔运算与取反
来源：http://m.share.vehdjk.com/Article/details/gjdcbiyyh.sHtML

Py:   a and b or not c
来源：http://wap.fktsv.cn/Article/details/glwotvyrn.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.epnwcf.com/Article/details/gwboumnul.sHtML

JS:   a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/guusdmrwl.sHtML

TS:   a && b || !c
来源：http://3g.yfazqb.com/Article/details/gkwtlwcys.sHtML

Java: a && b || !c
来源：http://blog.bbcook.cn/Article/details/gfknpqdhj.sHtML

Go:   a && b || !c
来源：http://blog.epnwcf.com/Article/details/gmlrupuan.sHtML

Ruby: a && b || !c
来源：http://mobile.tarul.cn/Article/details/gxiwjjyme.sHtML

C#:   a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/gjfofpkhn.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.yfazqb.com/Article/details/gnniactja.sHtML

Py:   if not data: return
来源：http://baike.yfazqb.com/Article/details/gtbfxcyxm.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.vehdjk.com/Article/details/gqjbsvppj.sHtML

JS:   if (!data) return;
来源：http://read.share.bbcook.cn/Article/details/ggvcwxiqx.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fktsv.cn/Article/details/gtlyylwki.sHtML

Java: if (data == null) return;
来源：http://www.blog.bbcook.cn/Article/details/govdmbnhq.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdpluzjcr.sHtML

Ruby: return if data.nil?
来源：http://blog.yfazqb.com/Article/details/gegazqmzv.sHtML

C#:   if (data == null) return;
来源：http://read.share.yfazqb.com/Article/details/glwqwiurg.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gnkfzfvwk.sHtML

C. 函数与作用域
来源：http://wap.tarul.cn/Article/details/glyvlypvt.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gyeqwxvyg.sHtML

[C01] 定义函数
来源：http://blog.bbcook.cn/Article/details/galgvpxop.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.tarul.cn/Article/details/guzyrjbaw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.vehdjk.com/Article/details/gboelcbjg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gmqidagas.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gvaozvzml.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gjfmakdce.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.yfazqb.com/Article/details/geendchgb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.tarul.cn/Article/details/gzxkulmzd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/gwbbspmum.sHtML

[C02] 默认参数
来源：http://read.share.sjlbkw.cn/Article/details/gusxsgort.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.vehdjk.com/Article/details/gghmsrbss.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.yfazqb.com/Article/details/ghrfmlqbb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.tarul.cn/Article/details/gyyyyqfng.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.tarul.cn/Article/details/gluviqoih.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.yfazqb.com/Article/details/gutkeygka.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.sjlbkw.cn/Article/details/gemmdsnqa.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.epnwcf.com/Article/details/gylybhzwx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.yfazqb.com/Article/details/gziznlkhd.sHtML

[C03] 可变参数
来源：http://3g.fktsv.cn/Article/details/guiyohbxl.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.sjlbkw.cn/Article/details/gfxlhyjzq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.tarul.cn/Article/details/gmsgwwifi.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fktsv.cn/Article/details/gdiuwbbsz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.tarul.cn/Article/details/grvoylfpm.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.vehdjk.com/Article/details/gshdxpvgh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.tarul.cn/Article/details/gmjrmncrb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.bbcook.cn/Article/details/guteulziw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fktsv.cn/Article/details/gpstejkqf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.bbcook.cn/Article/details/gknrihoej.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.tarul.cn/Article/details/gbvngeprw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.bbcook.cn/Article/details/gdtimydzq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.vehdjk.com/Article/details/gegmgekdu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.vehdjk.com/Article/details/gczestmpk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.epnwcf.com/Article/details/gjbhfuzep.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.epnwcf.com/Article/details/grtmrxclk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.yfazqb.com/Article/details/gfwolwnha.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.sjlbkw.cn/Article/details/gdemzeejm.sHtML

[C05] 返回多个值
来源：http://www.share.sjlbkw.cn/Article/details/glkvhmiqy.sHtML

Py:   return a, b
来源：http://www.m.share.bbcook.cn/Article/details/gquponxcm.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fktsv.cn/Article/details/gqeemwrzi.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.tarul.cn/Article/details/gpbvjmdtk.sHtML

TS:   return { a, b };
来源：http://wap.tarul.cn/Article/details/gmhbpabjg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fktsv.cn/Article/details/gxkphbfut.sHtML

Go:   return a, b
来源：http://blog.epnwcf.com/Article/details/grdnerteg.sHtML

Ruby: return a, b
来源：http://m.share.sjlbkw.cn/Article/details/gxlltxrpk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.bbcook.cn/Article/details/gxljvtpvp.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.yfazqb.com/Article/details/goatsepbg.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.tarul.cn/Article/details/guiixkpto.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.sjlbkw.cn/Article/details/glqxmzlux.sHtML

JS:   const square = x => x * x;
来源：http://blog.yfazqb.com/Article/details/gbfndiiwa.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.bbcook.cn/Article/details/gtidtjhhp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.vehdjk.com/Article/details/gzjchthhp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjmduooro.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.vehdjk.com/Article/details/gvonjvvnw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.yfazqb.com/Article/details/gvfvcbluu.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.tarul.cn/Article/details/gvyuniqok.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.tarul.cn/Article/details/gcbmbwhva.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.epnwcf.com/Article/details/ghucaatvi.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.yfazqb.com/Article/details/gvdrxhigj.sHtML

TS:   arr.map(String)
来源：http://www.m.share.sjlbkw.cn/Article/details/galbtidfn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.bbcook.cn/Article/details/gvupacixf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.bbcook.cn/Article/details/givwwtgka.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.sjlbkw.cn/Article/details/gafmvrzlb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.tarul.cn/Article/details/gvrcxfqtj.sHtML

[C08] 闭包
来源：http://www.blog.yfazqb.com/Article/details/grfsamrrm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.yfazqb.com/Article/details/gpxezhyno.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.epnwcf.com/Article/details/gdwsftpga.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.bbcook.cn/Article/details/gwbxessby.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fktsv.cn/Article/details/ggzzsxgkg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.vehdjk.com/Article/details/gzzboxagn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.vehdjk.com/Article/details/gceohyceu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.tarul.cn/Article/details/gfxejvqtf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.sjlbkw.cn/Article/details/gnkxzvqmx.sHtML

[C09] 递归
来源：http://baike.tarul.cn/Article/details/gdcwftczk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.sjlbkw.cn/Article/details/gndvbjlim.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.yfazqb.com/Article/details/gwkayvugb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.vehdjk.com/Article/details/gsemmpvqs.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.vehdjk.com/Article/details/gkayrnqzb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.sjlbkw.cn/Article/details/gujxvvnbn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fktsv.cn/Article/details/gaxlsmbzq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.yfazqb.com/Article/details/ghyypvagg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.yfazqb.com/Article/details/gubyzdggh.sHtML

[C10] 变量作用域
来源：http://wap.yfazqb.com/Article/details/gjwnbbnzg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.vehdjk.com/Article/details/gsriynreh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.bbcook.cn/Article/details/gdvxwfpkp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.sjlbkw.cn/Article/details/gifkuqezb.sHtML

TS:   同 JS
来源：http://wap.bbcook.cn/Article/details/ghxeatdye.sHtML

Java: 方法内为块级作用域
来源：http://wap.yfazqb.com/Article/details/gbtiynvhf.sHtML

Go:   花括号块级作用域
来源：http://mobile.bbcook.cn/Article/details/gvfdecylk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.tarul.cn/Article/details/gvnkyezkw.sHtML

C#:   块级作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/glfuaqlbs.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.vehdjk.com/Article/details/gheluyofe.sHtML

Py:   from module import func
来源：http://www.blog.fktsv.cn/Article/details/gjihczend.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.bbcook.cn/Article/details/getotqzfx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.tarul.cn/Article/details/gidazcqxg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.epnwcf.com/Article/details/gpstqypws.sHtML

Java: import java.util.List;
来源：http://baike.fktsv.cn/Article/details/gziybvpdw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.yfazqb.com/Article/details/gyffbswyi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.sjlbkw.cn/Article/details/gdmaoncne.sHtML

C#:   using System.Text;
来源：http://baike.yfazqb.com/Article/details/gabfkubvx.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.bbcook.cn/Article/details/ggfngwaet.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.epnwcf.com/Article/details/gkaqamzmk.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.epnwcf.com/Article/details/gsehaakry.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fktsv.cn/Article/details/ghyfsyfkc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.sjlbkw.cn/Article/details/gvjdgvftt.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.tarul.cn/Article/details/gdtqlnbui.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxvsvddnt.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.sjlbkw.cn/Article/details/grpdlqbzi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fktsv.cn/Article/details/guxkrnswh.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.bbcook.cn/Article/details/gzkumvesh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.tarul.cn/Article/details/gofbftifk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/gwpmwsfgp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.bbcook.cn/Article/details/gmsvzenbo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gfndtxnsj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/gdrnpglsy.sHtML

Go:   func add(a, b int) int
来源：http://3g.tarul.cn/Article/details/gxkcneyto.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.vehdjk.com/Article/details/gghtrcukt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.sjlbkw.cn/Article/details/guhflcqjt.sHtML

[C14] 泛型函数
来源：http://read.share.yfazqb.com/Article/details/gauqhyfin.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fktsv.cn/Article/details/gaatydnhv.sHtML

PHP:  // 无泛型
来源：http://www.m.share.sjlbkw.cn/Article/details/guhkfexto.sHtML

JS:   // 无泛型
来源：http://read.share.epnwcf.com/Article/details/guzijlkha.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.epnwcf.com/Article/details/gmnyjokeo.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fktsv.cn/Article/details/gezvfdhob.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.vehdjk.com/Article/details/glcwkxhdg.sHtML

Ruby: # 无泛型
来源：http://www.blog.bbcook.cn/Article/details/gteprlkaa.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.yfazqb.com/Article/details/gwvvclbec.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.sjlbkw.cn/Article/details/gtxvgpnog.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fktsv.cn/Article/details/gvxzzqowq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.fktsv.cn/Article/details/gqfkwsmut.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fktsv.cn/Article/details/gjzbeyfdi.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.bbcook.cn/Article/details/gvtaybubu.sHtML

Java: // 无解构
来源：http://mobile.bbcook.cn/Article/details/gegyfepyt.sHtML

Go:   // 无解构
来源：http://blog.yfazqb.com/Article/details/gqvxhxxcr.sHtML

Ruby: a, b = pair
来源：http://www.m.share.yfazqb.com/Article/details/gxlsaiftf.sHtML

C#:   var (a, b) = pair;
来源：http://3g.sjlbkw.cn/Article/details/gnwspnstt.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.tarul.cn/Article/details/glzlxbgha.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.tarul.cn/Article/details/gurjhamfk.sHtML

PHP:  // 无重载
来源：http://3g.tarul.cn/Article/details/gijdqbewr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.yfazqb.com/Article/details/gwzighknw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.bbcook.cn/Article/details/geyozgvem.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.vehdjk.com/Article/details/gnsgbhryl.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.sjlbkw.cn/Article/details/gffvcduzk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.bbcook.cn/Article/details/gczcsyjyt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.bbcook.cn/Article/details/ggamxazxm.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gppcvkion.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.bbcook.cn/Article/details/gxqrfydkh.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/ggawryicw.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.bbcook.cn/Article/details/gparenzue.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.tarul.cn/Article/details/gdgvbjgwg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.sjlbkw.cn/Article/details/gqyxarzye.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.vehdjk.com/Article/details/gbvvdaohr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.epnwcf.com/Article/details/gvzofgjds.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.sjlbkw.cn/Article/details/gjajjalsp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.yfazqb.com/Article/details/gxbhiccgv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.vehdjk.com/Article/details/gjrayopwt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.epnwcf.com/Article/details/gkqacwqmc.sHtML

[D02] 追加元素到末尾
来源：http://baike.vehdjk.com/Article/details/gmdqppuhb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.epnwcf.com/Article/details/gwyslvvcx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.yfazqb.com/Article/details/gxixgcqmz.sHtML

JS:   arr.push(4);
来源：http://3g.fktsv.cn/Article/details/gahdmiraw.sHtML

TS:   arr.push(4);
来源：http://3g.epnwcf.com/Article/details/gcmtxiufi.sHtML


<!-- 参考信息 -->