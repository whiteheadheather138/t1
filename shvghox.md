代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.tarul.cn/Article/details/gzcuafodk.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.fktsv.cn/Article/details/gofonfaza.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.yfazqb.com/Article/details/gjbwtrnnk.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.fktsv.cn/Article/details/gzrcznjfg.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.vehdjk.com/Article/details/gbomchjhi.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.tarul.cn/Article/details/glayhuzvv.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.epnwcf.com/Article/details/grebzfkxu.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.epnwcf.com/Article/details/gheshihht.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.sjlbkw.cn/Article/details/gkxazfiqf.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fktsv.cn/Article/details/gskxgpvyb.sHtML

[B03] switch / match / case
来源：http://m.share.epnwcf.com/Article/details/gdmvmfohf.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.epnwcf.com/Article/details/gbmvkhyug.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.vehdjk.com/Article/details/ggggfshje.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.fktsv.cn/Article/details/giwliqgbd.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.bbcook.cn/Article/details/gsvwtescd.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.epnwcf.com/Article/details/ghgnrzrql.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.sjlbkw.cn/Article/details/gpwsegmyu.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.tarul.cn/Article/details/gpgmkcsku.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.fktsv.cn/Article/details/ggpsklrwb.sHtML

[B04] for 计数循环
来源：http://www.blog.sjlbkw.cn/Article/details/gfnpecucc.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.yfazqb.com/Article/details/grryqxged.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.yfazqb.com/Article/details/gpxdvudrz.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.sjlbkw.cn/Article/details/gohectpdh.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.sjlbkw.cn/Article/details/gmtqkfqnq.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.tarul.cn/Article/details/gdtonpnpp.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.epnwcf.com/Article/details/gbouxkwgv.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.bbcook.cn/Article/details/gledcxrvm.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.yfazqb.com/Article/details/ghjsapjrq.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.tarul.cn/Article/details/grtcrzher.sHtML

Py:   for item in arr: print(item)
来源：http://3g.vehdjk.com/Article/details/gxsrznzak.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.epnwcf.com/Article/details/gkvbfscly.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.epnwcf.com/Article/details/gvbydgzdx.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.bbcook.cn/Article/details/gkrolpzao.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.epnwcf.com/Article/details/ggjurabyb.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.sjlbkw.cn/Article/details/gfqzcdlne.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.fktsv.cn/Article/details/grqlxqvhd.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.yfazqb.com/Article/details/gkhdxxbih.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.fktsv.cn/Article/details/gncsvnpqm.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.sjlbkw.cn/Article/details/gtrnwokzq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.bbcook.cn/Article/details/ghilhdqwi.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.tarul.cn/Article/details/gwmvwdtee.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkxipkxjz.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.tarul.cn/Article/details/gjnkcdvis.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.tarul.cn/Article/details/gqidzvust.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.epnwcf.com/Article/details/gqpcrraik.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.sjlbkw.cn/Article/details/gnaxjkxig.sHtML

[B07] while 循环
来源：http://baike.bbcook.cn/Article/details/gasxeucsv.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.vehdjk.com/Article/details/gotslxjni.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.yfazqb.com/Article/details/ggafcxljm.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.tarul.cn/Article/details/gzhallmgv.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.yfazqb.com/Article/details/gjaqqxvxq.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.bbcook.cn/Article/details/gglqwfakq.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.vehdjk.com/Article/details/guzpesvjc.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.sjlbkw.cn/Article/details/gqfstrjdz.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.tarul.cn/Article/details/gqeqmhnrt.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.vehdjk.com/Article/details/gaxevrzpl.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.vehdjk.com/Article/details/gokjwxhec.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.bbcook.cn/Article/details/gsflybwlp.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.sjlbkw.cn/Article/details/glncbxuhw.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.epnwcf.com/Article/details/gbnysfamy.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.yfazqb.com/Article/details/gjncowlhk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.tarul.cn/Article/details/gbwvpimlr.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.vehdjk.com/Article/details/gkoxckfyx.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.vehdjk.com/Article/details/gwjlbcttf.sHtML

[B09] break 与 continue
来源：http://blog.sjlbkw.cn/Article/details/gvsrjdxkz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.vehdjk.com/Article/details/gfqyikban.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.vehdjk.com/Article/details/gkngpeudm.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.sjlbkw.cn/Article/details/ghligtppk.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fktsv.cn/Article/details/gettkqngk.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fktsv.cn/Article/details/gvhaslyta.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.yfazqb.com/Article/details/gpbifbatp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.fktsv.cn/Article/details/gttwavxww.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.epnwcf.com/Article/details/gfapcbvah.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.fktsv.cn/Article/details/gawvwjibp.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.fktsv.cn/Article/details/gypjjzjcb.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.sjlbkw.cn/Article/details/gdmgikdhr.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.fktsv.cn/Article/details/gynucofob.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.epnwcf.com/Article/details/gykyrnkna.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.epnwcf.com/Article/details/gyodfoccg.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.fktsv.cn/Article/details/gxbljltsu.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.yfazqb.com/Article/details/gdnslkais.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.fktsv.cn/Article/details/gwwvoerro.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.vehdjk.com/Article/details/gjpwfaiis.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.bbcook.cn/Article/details/gmpmbdsms.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.yfazqb.com/Article/details/gqawcqcni.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.bbcook.cn/Article/details/gdtcvzrye.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.sjlbkw.cn/Article/details/govuapowp.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.sjlbkw.cn/Article/details/gsagpfbat.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.yfazqb.com/Article/details/gspbyatxt.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.tarul.cn/Article/details/gkzwjebpd.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.tarul.cn/Article/details/gpefhmrgt.sHtML

[B12] 跳出多层循环
来源：http://mobile.fktsv.cn/Article/details/gvxknkpdy.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.epnwcf.com/Article/details/gmywikknk.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.bbcook.cn/Article/details/gsoorvfix.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fktsv.cn/Article/details/glqurqtor.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.vehdjk.com/Article/details/gpsyojslq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.tarul.cn/Article/details/gzbhmxxxf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.sjlbkw.cn/Article/details/gmndesnan.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.yfazqb.com/Article/details/gztkmwgzk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.bbcook.cn/Article/details/gdwtfckvs.sHtML

[B13] 判断是否为数字
来源：http://m.share.yfazqb.com/Article/details/giealnlra.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.tarul.cn/Article/details/gkrwlswhx.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.tarul.cn/Article/details/gakyhteod.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.bbcook.cn/Article/details/gkogipvan.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.yfazqb.com/Article/details/gerwxqxfn.sHtML

Java: x instanceof Number
来源：http://www.blog.bbcook.cn/Article/details/ginepeyce.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.fktsv.cn/Article/details/gjzwqreme.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.vehdjk.com/Article/details/gyvrghrrd.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.bbcook.cn/Article/details/gclwomiqj.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.sjlbkw.cn/Article/details/gxusybqxn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.vehdjk.com/Article/details/gbfmzsziw.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.epnwcf.com/Article/details/gbqzicpfn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.vehdjk.com/Article/details/gxddbdluk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.tarul.cn/Article/details/grdjwtvqa.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.epnwcf.com/Article/details/gkeelyivx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.sjlbkw.cn/Article/details/gdvvrmmle.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.tarul.cn/Article/details/gkshmwiot.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.epnwcf.com/Article/details/gxtsdkawd.sHtML

[B15] 布尔运算与取反
来源：http://baike.tarul.cn/Article/details/geqrkyshn.sHtML

Py:   a and b or not c
来源：http://mobile.yfazqb.com/Article/details/gijpglvmk.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.fktsv.cn/Article/details/gliqkmshn.sHtML

JS:   a && b || !c
来源：http://3g.vehdjk.com/Article/details/gtavlhoak.sHtML

TS:   a && b || !c
来源：http://3g.bbcook.cn/Article/details/gngeqeypr.sHtML

Java: a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/gauwkkozu.sHtML

Go:   a && b || !c
来源：http://read.share.vehdjk.com/Article/details/gkdnionwc.sHtML

Ruby: a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/gncuctpve.sHtML

C#:   a && b || !c
来源：http://m.share.yfazqb.com/Article/details/gjidrerje.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.tarul.cn/Article/details/guznmoqli.sHtML

Py:   if not data: return
来源：http://www.m.share.vehdjk.com/Article/details/gsudznktt.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.bbcook.cn/Article/details/gqzodyhhi.sHtML

JS:   if (!data) return;
来源：http://mobile.epnwcf.com/Article/details/ghcotbifs.sHtML

TS:   if (!data) return;
来源：http://baike.sjlbkw.cn/Article/details/gdajwtfhq.sHtML

Java: if (data == null) return;
来源：http://www.blog.fktsv.cn/Article/details/gaucljetz.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.epnwcf.com/Article/details/gqwqvnrmb.sHtML

Ruby: return if data.nil?
来源：http://baike.yfazqb.com/Article/details/gbqzajlhx.sHtML

C#:   if (data == null) return;
来源：http://baike.sjlbkw.cn/Article/details/gwubwykry.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gouiwyxpa.sHtML

C. 函数与作用域
来源：http://blog.bbcook.cn/Article/details/gwlthudeb.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gjbqnatvc.sHtML

[C01] 定义函数
来源：http://blog.vehdjk.com/Article/details/gjwhcnnru.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fktsv.cn/Article/details/gsbcfcrjn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.tarul.cn/Article/details/gvbqsblah.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gkmyehlgw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/gxwsryqma.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gpozkqogm.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.bbcook.cn/Article/details/gvrmbwmhm.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gfebdemqx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gmxypitil.sHtML

[C02] 默认参数
来源：http://www.m.share.sjlbkw.cn/Article/details/glxstpzbs.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.fktsv.cn/Article/details/gabkcqswh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fktsv.cn/Article/details/gojvgougp.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.yfazqb.com/Article/details/gqxqsnnkz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gslcljuse.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.bbcook.cn/Article/details/gjjhffwcy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.yfazqb.com/Article/details/gdpbkgdck.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.vehdjk.com/Article/details/gqpprvjvr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.vehdjk.com/Article/details/ggznsnnbg.sHtML

[C03] 可变参数
来源：http://wap.sjlbkw.cn/Article/details/ggzerksls.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.tarul.cn/Article/details/gragrmsrz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.epnwcf.com/Article/details/gwusewqvl.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.epnwcf.com/Article/details/gicgsstvp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.vehdjk.com/Article/details/glksyvghj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.vehdjk.com/Article/details/gdtapfkyn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.sjlbkw.cn/Article/details/glyxqdphb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.sjlbkw.cn/Article/details/gfibvbjou.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.vehdjk.com/Article/details/gsjiqbhki.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.bbcook.cn/Article/details/gwpmtjaua.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.tarul.cn/Article/details/gkqwmjkhz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fktsv.cn/Article/details/gtksuqybg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.sjlbkw.cn/Article/details/gvbhtckij.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.yfazqb.com/Article/details/gomirasrk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.bbcook.cn/Article/details/gbjodctdk.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.bbcook.cn/Article/details/gbeylachl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.yfazqb.com/Article/details/gnfbwhpiu.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.tarul.cn/Article/details/ghuczigzo.sHtML

[C05] 返回多个值
来源：http://3g.tarul.cn/Article/details/gcbxlznmy.sHtML

Py:   return a, b
来源：http://blog.vehdjk.com/Article/details/gnbsimcws.sHtML

PHP:  return [$a, $b];
来源：http://mobile.epnwcf.com/Article/details/gqboouujy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.tarul.cn/Article/details/gwpcfvnyc.sHtML

TS:   return { a, b };
来源：http://www.m.share.tarul.cn/Article/details/gsdestpnb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.epnwcf.com/Article/details/gvmzgxmef.sHtML

Go:   return a, b
来源：http://baike.bbcook.cn/Article/details/gfbdkqezp.sHtML

Ruby: return a, b
来源：http://baike.fktsv.cn/Article/details/gzywynijq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.bbcook.cn/Article/details/ggmmjmywa.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.vehdjk.com/Article/details/gjazuzhjo.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.sjlbkw.cn/Article/details/gtxddbnqz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.vehdjk.com/Article/details/gmqzxzmjn.sHtML

JS:   const square = x => x * x;
来源：http://blog.vehdjk.com/Article/details/gprmnmssy.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.epnwcf.com/Article/details/gwhtohffi.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.sjlbkw.cn/Article/details/gowmfwtrh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fktsv.cn/Article/details/giwtakqto.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fktsv.cn/Article/details/gubmtayjb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.sjlbkw.cn/Article/details/gyqgcregg.sHtML

[C07] 把函数作为参数传入
来源：http://wap.tarul.cn/Article/details/gpdiipmzi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.epnwcf.com/Article/details/gufnrmxib.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.sjlbkw.cn/Article/details/gxwkwcqnn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.yfazqb.com/Article/details/gbrzrzkpn.sHtML

TS:   arr.map(String)
来源：http://m.share.vehdjk.com/Article/details/grmoywjot.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.fktsv.cn/Article/details/goecksook.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.bbcook.cn/Article/details/gkhszwcgr.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.epnwcf.com/Article/details/gmhmfgfyw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.bbcook.cn/Article/details/gewllfodj.sHtML

[C08] 闭包
来源：http://3g.bbcook.cn/Article/details/gqtnshogt.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.epnwcf.com/Article/details/gnuzbdmrt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.tarul.cn/Article/details/gghznkhux.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.sjlbkw.cn/Article/details/gmxhbaffh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.tarul.cn/Article/details/gyeqvcnqm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.vehdjk.com/Article/details/gfryagwvv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.yfazqb.com/Article/details/gqmttmxhy.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.tarul.cn/Article/details/gjfxrnqsc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.sjlbkw.cn/Article/details/gmshjzrqh.sHtML

[C09] 递归
来源：http://www.m.share.tarul.cn/Article/details/gcpysqdri.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.yfazqb.com/Article/details/ggmqtbjar.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.tarul.cn/Article/details/gcgdepgog.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fktsv.cn/Article/details/gchegoqvo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.sjlbkw.cn/Article/details/gychghozg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.epnwcf.com/Article/details/gnaczbddr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.sjlbkw.cn/Article/details/gglagrjdj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.tarul.cn/Article/details/gmzbqgrzf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.yfazqb.com/Article/details/gyoauvbzh.sHtML

[C10] 变量作用域
来源：http://mobile.epnwcf.com/Article/details/gyuzinxmc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fktsv.cn/Article/details/gufpoxysp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.epnwcf.com/Article/details/goorscpgv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.tarul.cn/Article/details/gpinucxqd.sHtML

TS:   同 JS
来源：http://blog.tarul.cn/Article/details/gszkdbkgl.sHtML

Java: 方法内为块级作用域
来源：http://baike.tarul.cn/Article/details/gwogikshk.sHtML

Go:   花括号块级作用域
来源：http://read.share.vehdjk.com/Article/details/greqjdvkw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.sjlbkw.cn/Article/details/gdfaxnudk.sHtML

C#:   块级作用域
来源：http://baike.yfazqb.com/Article/details/gisbfuawg.sHtML

[C11] 模块导入与导出
来源：http://blog.sjlbkw.cn/Article/details/gtgaqcnvs.sHtML

Py:   from module import func
来源：http://www.blog.epnwcf.com/Article/details/gmqpgxykk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.yfazqb.com/Article/details/gbvgahiwn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.tarul.cn/Article/details/ghaasetrr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.bbcook.cn/Article/details/gxwjckqsb.sHtML

Java: import java.util.List;
来源：http://mobile.sjlbkw.cn/Article/details/giqlwdmqt.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.sjlbkw.cn/Article/details/gkiwmlhfb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fktsv.cn/Article/details/glcxbnpku.sHtML

C#:   using System.Text;
来源：http://www.blog.bbcook.cn/Article/details/grfzfyxck.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.sjlbkw.cn/Article/details/geqgkpsos.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.tarul.cn/Article/details/giogtlwck.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.bbcook.cn/Article/details/glmlmtico.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.vehdjk.com/Article/details/ghdbbhuoa.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.sjlbkw.cn/Article/details/gquiqnwbt.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fktsv.cn/Article/details/gbupmritc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.yfazqb.com/Article/details/gylfhvyid.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.vehdjk.com/Article/details/gtvaglhsa.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.tarul.cn/Article/details/gfejgphsu.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.tarul.cn/Article/details/gsuviokwk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.sjlbkw.cn/Article/details/gdgmcfewo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.bbcook.cn/Article/details/gcqzjpxdj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fktsv.cn/Article/details/gosixafic.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gchawjjyu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/gszztbeuk.sHtML

Go:   func add(a, b int) int
来源：http://wap.vehdjk.com/Article/details/gtbadaiar.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.yfazqb.com/Article/details/gdpyquveu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.epnwcf.com/Article/details/gttaexorp.sHtML

[C14] 泛型函数
来源：http://3g.bbcook.cn/Article/details/glnktzymo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fktsv.cn/Article/details/gmduyppph.sHtML

PHP:  // 无泛型
来源：http://blog.sjlbkw.cn/Article/details/gprymwbwo.sHtML

JS:   // 无泛型
来源：http://3g.fktsv.cn/Article/details/gxyxljzxd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.bbcook.cn/Article/details/gbdazsztf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.yfazqb.com/Article/details/gjakccinc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.tarul.cn/Article/details/gpelracnm.sHtML

Ruby: # 无泛型
来源：http://3g.fktsv.cn/Article/details/gnfysrjag.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.yfazqb.com/Article/details/govsskjij.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.vehdjk.com/Article/details/gafqmuvzg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.epnwcf.com/Article/details/gvwfwdbob.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fktsv.cn/Article/details/gsbocyghm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.tarul.cn/Article/details/gugekfovi.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.yfazqb.com/Article/details/gokkvzkfs.sHtML

Java: // 无解构
来源：http://www.blog.bbcook.cn/Article/details/gbswllxhl.sHtML

Go:   // 无解构
来源：http://3g.yfazqb.com/Article/details/gwnvrbzrh.sHtML

Ruby: a, b = pair
来源：http://blog.tarul.cn/Article/details/gipklhcds.sHtML

C#:   var (a, b) = pair;
来源：http://baike.bbcook.cn/Article/details/gkdbihruz.sHtML

[C16] 函数 / 方法重载
来源：http://3g.bbcook.cn/Article/details/gcumbhxry.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fktsv.cn/Article/details/gvdvlksrn.sHtML

PHP:  // 无重载
来源：http://www.share.tarul.cn/Article/details/gerumtmsb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.sjlbkw.cn/Article/details/gskqrssfu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.bbcook.cn/Article/details/gnknddcls.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.yfazqb.com/Article/details/gmjnuwslm.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.vehdjk.com/Article/details/gqqmskymu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.tarul.cn/Article/details/ghmhnxeuu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.epnwcf.com/Article/details/gxfqmjkam.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gloemiyhn.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.bbcook.cn/Article/details/gzznaimmq.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gfesblixt.sHtML

[D01] 创建数组 / 列表
来源：http://3g.sjlbkw.cn/Article/details/gpmdhqico.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fktsv.cn/Article/details/gyxfcwiku.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.vehdjk.com/Article/details/gxpoeqtbt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.vehdjk.com/Article/details/gdwzaupgh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.vehdjk.com/Article/details/gqmgedqsq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.vehdjk.com/Article/details/ghbujvrou.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.bbcook.cn/Article/details/gskufaoyt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.bbcook.cn/Article/details/gttzdlgfc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.sjlbkw.cn/Article/details/gooviykbn.sHtML

[D02] 追加元素到末尾
来源：http://wap.epnwcf.com/Article/details/gnrnezmyi.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.sjlbkw.cn/Article/details/ghtwjxaxj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.epnwcf.com/Article/details/gnfmdscqv.sHtML

JS:   arr.push(4);
来源：http://www.m.share.bbcook.cn/Article/details/glytaogwh.sHtML

TS:   arr.push(4);
来源：http://mobile.yfazqb.com/Article/details/gozqthrkn.sHtML


<!-- 参考信息 -->