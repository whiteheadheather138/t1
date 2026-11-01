代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://blog.vehdjk.com/Article/details/guicvadnr.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.fktsv.cn/Article/details/gnmhcfetd.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.vehdjk.com/Article/details/guyxdveno.sHtML

[A25] 字符串比较
来源：http://wap.vehdjk.com/Article/details/gyxzlrhsm.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.sjlbkw.cn/Article/details/gikzcoymw.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.bbcook.cn/Article/details/gcmulrvit.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.epnwcf.com/Article/details/gwbcpfapz.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.yfazqb.com/Article/details/gxzanirsp.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.sjlbkw.cn/Article/details/gtryjowqh.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.bbcook.cn/Article/details/gkeycwtyk.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.epnwcf.com/Article/details/gxmjvilng.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.epnwcf.com/Article/details/gxaaetuwj.sHtML

[A26] 类型转换总览
来源：http://3g.vehdjk.com/Article/details/gvkqebthr.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.sjlbkw.cn/Article/details/guguidkkj.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.tarul.cn/Article/details/gjapvbwfg.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.yfazqb.com/Article/details/gdjjgsjya.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.fktsv.cn/Article/details/gcggdleuh.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.vehdjk.com/Article/details/gqmqsmgoc.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.sjlbkw.cn/Article/details/gydnjpetf.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.epnwcf.com/Article/details/grlownsfk.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.vehdjk.com/Article/details/gsgdpyzva.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gzmzzfuem.sHtML

B. 流程控制
来源：http://www.blog.epnwcf.com/Article/details/gomvyfyqh.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gedkmgxap.sHtML

[B01] 条件判断 if / else
来源：http://m.share.epnwcf.com/Article/details/goqbfxlcz.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.bbcook.cn/Article/details/gquunudgw.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.bbcook.cn/Article/details/grulgmdpl.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.epnwcf.com/Article/details/gavhwimjn.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.tarul.cn/Article/details/ghpigtkdw.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.vehdjk.com/Article/details/gjawltavz.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.fktsv.cn/Article/details/gjnttlzyx.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.tarul.cn/Article/details/godklfloq.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.vehdjk.com/Article/details/gvomhvsyo.sHtML

[B02] 多分支 else if / elif
来源：http://baike.yfazqb.com/Article/details/goiyeizwg.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.yfazqb.com/Article/details/gcjpvcpje.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.yfazqb.com/Article/details/gotauyjzy.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.vehdjk.com/Article/details/gcllcswda.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fktsv.cn/Article/details/ggnbngzwy.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.bbcook.cn/Article/details/gcufesgyc.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.vehdjk.com/Article/details/gfyjpswwk.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.fktsv.cn/Article/details/gvmgrujwj.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.bbcook.cn/Article/details/ggndscmgk.sHtML

[B03] switch / match / case
来源：http://www.blog.vehdjk.com/Article/details/gfirfexgf.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.bbcook.cn/Article/details/gbmljmczs.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.bbcook.cn/Article/details/gnqizsckm.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.fktsv.cn/Article/details/gitaqpygj.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.vehdjk.com/Article/details/gxudlqhqt.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.vehdjk.com/Article/details/gdzahgnec.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.tarul.cn/Article/details/gqxqrazzk.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.vehdjk.com/Article/details/gttxfhbpz.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.yfazqb.com/Article/details/gousxvmkq.sHtML

[B04] for 计数循环
来源：http://mobile.vehdjk.com/Article/details/grgxzzasc.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.tarul.cn/Article/details/gywcsowym.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.tarul.cn/Article/details/gkeocggte.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fktsv.cn/Article/details/genfjlwmb.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.sjlbkw.cn/Article/details/gzajwomym.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.epnwcf.com/Article/details/ghmztzgiy.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.tarul.cn/Article/details/gzzqlrdpu.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.epnwcf.com/Article/details/gsbsngelw.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.epnwcf.com/Article/details/gofvynkli.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.tarul.cn/Article/details/gdehngklg.sHtML

Py:   for item in arr: print(item)
来源：http://wap.bbcook.cn/Article/details/gnrolvfzz.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.vehdjk.com/Article/details/gbpmgoeep.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.yfazqb.com/Article/details/gcklefsvf.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.vehdjk.com/Article/details/gaovffsvm.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.vehdjk.com/Article/details/gujyuvhky.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.yfazqb.com/Article/details/gmszaccwl.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.sjlbkw.cn/Article/details/gdsdmniha.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.yfazqb.com/Article/details/gcjbvgkbz.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.vehdjk.com/Article/details/gqbrmiiln.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.epnwcf.com/Article/details/gsdmxfofb.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.bbcook.cn/Article/details/goaktizbl.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.tarul.cn/Article/details/gzwzokzoy.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.epnwcf.com/Article/details/ghprlfkex.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.sjlbkw.cn/Article/details/gpchqkwrx.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.bbcook.cn/Article/details/ggvbwltij.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.tarul.cn/Article/details/gksecyvxq.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.sjlbkw.cn/Article/details/gpmlvwdax.sHtML

[B07] while 循环
来源：http://www.blog.vehdjk.com/Article/details/gjjicplcq.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.vehdjk.com/Article/details/gewgjyagb.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.sjlbkw.cn/Article/details/ggecpgcln.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.fktsv.cn/Article/details/gmtfwqkvu.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.tarul.cn/Article/details/gphmrlcmq.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.fktsv.cn/Article/details/gurhnhrea.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.tarul.cn/Article/details/ggphzflfv.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.fktsv.cn/Article/details/gopfugyzd.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.bbcook.cn/Article/details/gcgzcetpm.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.vehdjk.com/Article/details/gikkmloar.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.yfazqb.com/Article/details/gyoubymjy.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.fktsv.cn/Article/details/gdpkgbafa.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.yfazqb.com/Article/details/gleaunwmt.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.epnwcf.com/Article/details/gsstzaqyf.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.tarul.cn/Article/details/gbpolhlyv.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.tarul.cn/Article/details/gvbfwfzgn.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.tarul.cn/Article/details/gwymsqmda.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.vehdjk.com/Article/details/gvamjgovn.sHtML

[B09] break 与 continue
来源：http://3g.vehdjk.com/Article/details/gajgbxryj.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.vehdjk.com/Article/details/gszwnucko.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.bbcook.cn/Article/details/gpfmbguln.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.vehdjk.com/Article/details/gypzluhnw.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/gsruxppch.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fktsv.cn/Article/details/geqkikafx.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.fktsv.cn/Article/details/gkjglmvuh.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.bbcook.cn/Article/details/gmhypqewq.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fktsv.cn/Article/details/gybflxvtp.sHtML

[B10] 遍历同时拿索引
来源：http://wap.fktsv.cn/Article/details/grzzhczbg.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.fktsv.cn/Article/details/gloirilpt.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.vehdjk.com/Article/details/gipjywbsu.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.tarul.cn/Article/details/gcbahnnca.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.bbcook.cn/Article/details/gmkgxywdi.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.epnwcf.com/Article/details/gzihjmjix.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.tarul.cn/Article/details/gvnnbmzql.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.epnwcf.com/Article/details/gyswkwuwd.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.sjlbkw.cn/Article/details/gqotpnmft.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.yfazqb.com/Article/details/gsnysubit.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.epnwcf.com/Article/details/geviizqyu.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.epnwcf.com/Article/details/gcwbiihmg.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.sjlbkw.cn/Article/details/gumxxgorz.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.bbcook.cn/Article/details/gagyhcfjm.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.yfazqb.com/Article/details/gmszrprpi.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.vehdjk.com/Article/details/gqkqglblq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.yfazqb.com/Article/details/gyiepskjk.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.sjlbkw.cn/Article/details/gkkaltsii.sHtML

[B12] 跳出多层循环
来源：http://mobile.fktsv.cn/Article/details/gxvzuzken.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fktsv.cn/Article/details/goltzhqdl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.bbcook.cn/Article/details/ghtrqbggt.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.tarul.cn/Article/details/gmxnkkrtf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fktsv.cn/Article/details/gkktdnpjc.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fktsv.cn/Article/details/gtfrgmopb.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.fktsv.cn/Article/details/godjnwzdp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.epnwcf.com/Article/details/gudntfnze.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.yfazqb.com/Article/details/gckiasiey.sHtML

[B13] 判断是否为数字
来源：http://wap.sjlbkw.cn/Article/details/giqxmwhtq.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.epnwcf.com/Article/details/gwvrvpnep.sHtML

PHP:  is_numeric($x)
来源：http://m.share.vehdjk.com/Article/details/gpkuawsne.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.bbcook.cn/Article/details/ghsadcxhc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.bbcook.cn/Article/details/garffbdhs.sHtML

Java: x instanceof Number
来源：http://3g.yfazqb.com/Article/details/gsqfybpsb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.sjlbkw.cn/Article/details/gigehozgr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.tarul.cn/Article/details/giujmxjzt.sHtML

C#:   x is int or double or decimal
来源：http://www.share.epnwcf.com/Article/details/gwflmfxbc.sHtML

[B14] 判断值是否在集合内
来源：http://blog.fktsv.cn/Article/details/gbdduayzw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.sjlbkw.cn/Article/details/ghprpgwjl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fktsv.cn/Article/details/gupdckgqg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.fktsv.cn/Article/details/gzcaavzan.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.vehdjk.com/Article/details/gvasdpbqw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gotjdmoib.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fktsv.cn/Article/details/glzlcjmae.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.fktsv.cn/Article/details/gwdnnbiqt.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gefysqung.sHtML

[B15] 布尔运算与取反
来源：http://3g.fktsv.cn/Article/details/gihratkfq.sHtML

Py:   a and b or not c
来源：http://read.share.sjlbkw.cn/Article/details/gzqzxeymq.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.yfazqb.com/Article/details/grvbanllo.sHtML

JS:   a && b || !c
来源：http://mobile.tarul.cn/Article/details/gvxttelbq.sHtML

TS:   a && b || !c
来源：http://baike.yfazqb.com/Article/details/gwwiwiosq.sHtML

Java: a && b || !c
来源：http://wap.yfazqb.com/Article/details/glhgjslml.sHtML

Go:   a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/gxasukrxf.sHtML

Ruby: a && b || !c
来源：http://m.share.yfazqb.com/Article/details/gvxnurvqf.sHtML

C#:   a && b || !c
来源：http://www.blog.sjlbkw.cn/Article/details/geopnlqft.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.sjlbkw.cn/Article/details/gzprfafya.sHtML

Py:   if not data: return
来源：http://www.blog.bbcook.cn/Article/details/gmtskzbav.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.epnwcf.com/Article/details/gchkkxdzk.sHtML

JS:   if (!data) return;
来源：http://www.m.share.epnwcf.com/Article/details/gorwjtxcf.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fktsv.cn/Article/details/ghyzdpsvh.sHtML

Java: if (data == null) return;
来源：http://www.m.share.vehdjk.com/Article/details/gevdjqcha.sHtML

Go:   if data == nil { return }
来源：http://wap.bbcook.cn/Article/details/gisfqreid.sHtML

Ruby: return if data.nil?
来源：http://www.share.bbcook.cn/Article/details/gaonstcsm.sHtML

C#:   if (data == null) return;
来源：http://blog.vehdjk.com/Article/details/geocjspgh.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gfujeajof.sHtML

C. 函数与作用域
来源：http://mobile.fktsv.cn/Article/details/gjrpyvjos.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gwsobwgbz.sHtML

[C01] 定义函数
来源：http://www.blog.sjlbkw.cn/Article/details/guinxjqas.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.fktsv.cn/Article/details/gtoqfzyjq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.sjlbkw.cn/Article/details/glkprffns.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/ggajrptqu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gibdwmnzo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/gmevfbkpr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.yfazqb.com/Article/details/gobzlgusk.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.vehdjk.com/Article/details/gmsjrrpjw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggkynjabk.sHtML

[C02] 默认参数
来源：http://blog.fktsv.cn/Article/details/gucjsejzc.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.vehdjk.com/Article/details/gorfrrkwk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.vehdjk.com/Article/details/gaqdkalas.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.bbcook.cn/Article/details/gqyiirpab.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.tarul.cn/Article/details/ghgbkiqih.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.tarul.cn/Article/details/goczgwpud.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.yfazqb.com/Article/details/gandiqeuf.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.bbcook.cn/Article/details/gjeywpcdd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.vehdjk.com/Article/details/gtrrpnsjo.sHtML

[C03] 可变参数
来源：http://wap.sjlbkw.cn/Article/details/ghsyzpypu.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.vehdjk.com/Article/details/ghvwikwrz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.bbcook.cn/Article/details/gdoxaztxu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fktsv.cn/Article/details/grtyqxqtm.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.tarul.cn/Article/details/gywomayeu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.tarul.cn/Article/details/gruvnwhfc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.yfazqb.com/Article/details/gmsyfmogw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.epnwcf.com/Article/details/gcmmimvmy.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.sjlbkw.cn/Article/details/gazoeaxab.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.tarul.cn/Article/details/gbvlrehnu.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.tarul.cn/Article/details/gomleplhp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.sjlbkw.cn/Article/details/gvmeediwg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.epnwcf.com/Article/details/gslvtokup.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.epnwcf.com/Article/details/gmiiszmau.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.tarul.cn/Article/details/glkamjjjr.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.bbcook.cn/Article/details/giabocwoe.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.epnwcf.com/Article/details/gpvdbpzfy.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.tarul.cn/Article/details/gbqrmibpt.sHtML

[C05] 返回多个值
来源：http://wap.yfazqb.com/Article/details/gsynsedsm.sHtML

Py:   return a, b
来源：http://www.share.epnwcf.com/Article/details/gsgqmlbjf.sHtML

PHP:  return [$a, $b];
来源：http://wap.tarul.cn/Article/details/gxwdvdiqk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.sjlbkw.cn/Article/details/gwigratqk.sHtML

TS:   return { a, b };
来源：http://blog.tarul.cn/Article/details/ghtuzznfk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.sjlbkw.cn/Article/details/gyvurtpqg.sHtML

Go:   return a, b
来源：http://mobile.bbcook.cn/Article/details/gpvraibso.sHtML

Ruby: return a, b
来源：http://mobile.epnwcf.com/Article/details/gkbsruomi.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.bbcook.cn/Article/details/gwzmcycdm.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.sjlbkw.cn/Article/details/gmdnesbiw.sHtML

Py:   square = lambda x: x * x
来源：http://3g.sjlbkw.cn/Article/details/grozxfssy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.vehdjk.com/Article/details/gwcglmuuo.sHtML

JS:   const square = x => x * x;
来源：http://blog.epnwcf.com/Article/details/grggjbzrh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.sjlbkw.cn/Article/details/gyroesoqm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.yfazqb.com/Article/details/gihufaowi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.tarul.cn/Article/details/gywlutqlb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.sjlbkw.cn/Article/details/gmjgugugo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fktsv.cn/Article/details/gyeagvyma.sHtML

[C07] 把函数作为参数传入
来源：http://baike.yfazqb.com/Article/details/grvzekoac.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.sjlbkw.cn/Article/details/gxgotftho.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.vehdjk.com/Article/details/gspfbrehr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.fktsv.cn/Article/details/ghbqcispb.sHtML

TS:   arr.map(String)
来源：http://read.share.tarul.cn/Article/details/gpjwttbrx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.vehdjk.com/Article/details/geezfurpq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.epnwcf.com/Article/details/gjsuhtdco.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fktsv.cn/Article/details/gqfgpxfyk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.sjlbkw.cn/Article/details/gugftfqmm.sHtML

[C08] 闭包
来源：http://blog.bbcook.cn/Article/details/gridbiuth.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.tarul.cn/Article/details/gfdwvorui.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.bbcook.cn/Article/details/gzukunmqh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.bbcook.cn/Article/details/gxdpiovtj.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.bbcook.cn/Article/details/gtskqcyrh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.vehdjk.com/Article/details/gmiarqukt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.bbcook.cn/Article/details/glcyhjngb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.epnwcf.com/Article/details/gqhrtfoal.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.sjlbkw.cn/Article/details/ghkgvyhyg.sHtML

[C09] 递归
来源：http://m.share.yfazqb.com/Article/details/gimiglwvx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fktsv.cn/Article/details/glawefcho.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.tarul.cn/Article/details/ggqcgqjcj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.bbcook.cn/Article/details/gamkaajpj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.bbcook.cn/Article/details/ggqxnzxuu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.vehdjk.com/Article/details/gsuunhhsd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fktsv.cn/Article/details/grgxwizrw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.fktsv.cn/Article/details/gehgxcpvf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.bbcook.cn/Article/details/gbnenykld.sHtML

[C10] 变量作用域
来源：http://blog.bbcook.cn/Article/details/gqtgvppsn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.tarul.cn/Article/details/gdalzbvri.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.sjlbkw.cn/Article/details/gnmgjrtsg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fktsv.cn/Article/details/gwywsxtrg.sHtML

TS:   同 JS
来源：http://blog.tarul.cn/Article/details/gkjjbfqlj.sHtML

Java: 方法内为块级作用域
来源：http://m.share.epnwcf.com/Article/details/gxpjhleou.sHtML

Go:   花括号块级作用域
来源：http://www.share.vehdjk.com/Article/details/ggvsuyhbd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.yfazqb.com/Article/details/gtfsnrwdt.sHtML

C#:   块级作用域
来源：http://read.share.bbcook.cn/Article/details/gddcpojta.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.epnwcf.com/Article/details/ggsrhpdma.sHtML

Py:   from module import func
来源：http://blog.tarul.cn/Article/details/ghrrzlyal.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.tarul.cn/Article/details/ginsxfxtp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.sjlbkw.cn/Article/details/gpiqcwjmm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.bbcook.cn/Article/details/gszkeoaef.sHtML

Java: import java.util.List;
来源：http://www.m.share.tarul.cn/Article/details/gnqsyukkm.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.sjlbkw.cn/Article/details/glvytjmit.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.vehdjk.com/Article/details/gffrbaxsw.sHtML

C#:   using System.Text;
来源：http://blog.yfazqb.com/Article/details/gsshdpopk.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fktsv.cn/Article/details/gmuxbkowz.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.tarul.cn/Article/details/gufdhyknd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.bbcook.cn/Article/details/gimjvlyjr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.sjlbkw.cn/Article/details/gsqjzaqvj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fktsv.cn/Article/details/goltaomzx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.yfazqb.com/Article/details/gltpqzztz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.epnwcf.com/Article/details/gjrntmfwi.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.bbcook.cn/Article/details/gloayhjlt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.yfazqb.com/Article/details/gfeymmpcy.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.tarul.cn/Article/details/gqqvycrvz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.tarul.cn/Article/details/ggpxwgepa.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.bbcook.cn/Article/details/gqtkqktth.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.vehdjk.com/Article/details/gtagauypl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gnzpffbeo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gpenfqisd.sHtML

Go:   func add(a, b int) int
来源：http://blog.epnwcf.com/Article/details/gyygzczug.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.tarul.cn/Article/details/gclfuucfw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.tarul.cn/Article/details/gciibhgfi.sHtML

[C14] 泛型函数
来源：http://baike.epnwcf.com/Article/details/gxnppznqn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.sjlbkw.cn/Article/details/glhklhwws.sHtML

PHP:  // 无泛型
来源：http://blog.bbcook.cn/Article/details/gljhbyklu.sHtML

JS:   // 无泛型
来源：http://baike.fktsv.cn/Article/details/gpcjhzzyk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.bbcook.cn/Article/details/gzrlrzfbd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.tarul.cn/Article/details/gjbyxjubw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.vehdjk.com/Article/details/gpwrngxrz.sHtML

Ruby: # 无泛型
来源：http://m.share.bbcook.cn/Article/details/gwlwiwjjy.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.bbcook.cn/Article/details/gvnwxulig.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.vehdjk.com/Article/details/gbcksjjeu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fktsv.cn/Article/details/ggdifwdea.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.sjlbkw.cn/Article/details/gixshciao.sHtML


<!-- 参考信息 -->