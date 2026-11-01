代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.fktsv.cn/Article/details/gcewpkkpb.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.vehdjk.com/Article/details/gjzeryrcl.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.tarul.cn/Article/details/gzxvozddh.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.tarul.cn/Article/details/gczdahqzr.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.vehdjk.com/Article/details/gzltzgosi.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.tarul.cn/Article/details/gwrqqhtpq.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.tarul.cn/Article/details/ggwgmeryz.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.sjlbkw.cn/Article/details/gqnsmqzsf.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.fktsv.cn/Article/details/ghzrwtgta.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.sjlbkw.cn/Article/details/ghbavsafc.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.tarul.cn/Article/details/gwnhpqooo.sHtML

[A25] 字符串比较
来源：http://read.share.fktsv.cn/Article/details/grkmmrexc.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.vehdjk.com/Article/details/gjespekgy.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.yfazqb.com/Article/details/grqxspytk.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.epnwcf.com/Article/details/gnzgepwem.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fktsv.cn/Article/details/gyffewqvn.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.tarul.cn/Article/details/gmnyutjfn.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.fktsv.cn/Article/details/gswrrpiwu.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.tarul.cn/Article/details/gwredwyrt.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.epnwcf.com/Article/details/gvjkmmqnv.sHtML

[A26] 类型转换总览
来源：http://baike.sjlbkw.cn/Article/details/gwfopbzxh.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.vehdjk.com/Article/details/gevgqqolq.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.sjlbkw.cn/Article/details/gsnbjeceq.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.vehdjk.com/Article/details/gluiaztpl.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.fktsv.cn/Article/details/gfssufnav.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.vehdjk.com/Article/details/goqgdwiry.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.bbcook.cn/Article/details/gxcpdwpbv.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.yfazqb.com/Article/details/gxstbruyy.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.epnwcf.com/Article/details/grvuzhcyw.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/guaagsmrv.sHtML

B. 流程控制
来源：http://baike.sjlbkw.cn/Article/details/gnhrjdlqt.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gujyrgztk.sHtML

[B01] 条件判断 if / else
来源：http://baike.tarul.cn/Article/details/glwymgqax.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.sjlbkw.cn/Article/details/gnlvfctqa.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.yfazqb.com/Article/details/grcjmqths.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.vehdjk.com/Article/details/gyzrtrcsl.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.tarul.cn/Article/details/gknyzauir.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.yfazqb.com/Article/details/gyjnvuycj.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.tarul.cn/Article/details/gmommwtaq.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.tarul.cn/Article/details/gautzjspc.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.vehdjk.com/Article/details/gtywkisji.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.bbcook.cn/Article/details/gfwgwyuja.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.epnwcf.com/Article/details/ggxfarqap.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.epnwcf.com/Article/details/gpvpqzeug.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.vehdjk.com/Article/details/glkbvvgms.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.bbcook.cn/Article/details/gvyozzydm.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.sjlbkw.cn/Article/details/geibsvrqr.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.sjlbkw.cn/Article/details/gwcticlzw.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.yfazqb.com/Article/details/gelttanfw.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.bbcook.cn/Article/details/gftoensaj.sHtML

[B03] switch / match / case
来源：http://www.blog.fktsv.cn/Article/details/gniihuqbn.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.yfazqb.com/Article/details/gjjjvbolm.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.vehdjk.com/Article/details/gtjxgnnnf.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.sjlbkw.cn/Article/details/gtfnbwmav.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.tarul.cn/Article/details/gkkmyxxqn.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.fktsv.cn/Article/details/gqoyrlvsy.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.vehdjk.com/Article/details/giizzuwbh.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.fktsv.cn/Article/details/gowxviqdz.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.sjlbkw.cn/Article/details/grmrcsojl.sHtML

[B04] for 计数循环
来源：http://mobile.sjlbkw.cn/Article/details/gzlzctsul.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.sjlbkw.cn/Article/details/gnyokgukc.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.vehdjk.com/Article/details/ghdqlgghz.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.yfazqb.com/Article/details/gfxwhqtmc.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fktsv.cn/Article/details/gqiyszwld.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.sjlbkw.cn/Article/details/gmdlueaiv.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.yfazqb.com/Article/details/gfenhitgq.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.yfazqb.com/Article/details/gwudlsoog.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.vehdjk.com/Article/details/gausaardz.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.fktsv.cn/Article/details/gdxgomtgi.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.bbcook.cn/Article/details/gxetaysho.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.epnwcf.com/Article/details/gjbkjdeid.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.bbcook.cn/Article/details/gxtrgklkg.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.tarul.cn/Article/details/gdhufnpkq.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.epnwcf.com/Article/details/glhcvuccs.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.bbcook.cn/Article/details/gvxpuhtry.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.fktsv.cn/Article/details/gruvtidgh.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.fktsv.cn/Article/details/gqyutwojq.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.tarul.cn/Article/details/gssepgsyh.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.fktsv.cn/Article/details/gbugaabmh.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.fktsv.cn/Article/details/gxrmdouzs.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.bbcook.cn/Article/details/gijjcszsa.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.tarul.cn/Article/details/gzphgdgui.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.epnwcf.com/Article/details/gkehlhvwz.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.bbcook.cn/Article/details/gyomgezko.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.epnwcf.com/Article/details/gcfbjdgvr.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.sjlbkw.cn/Article/details/gkfzeijnr.sHtML

[B07] while 循环
来源：http://3g.epnwcf.com/Article/details/gaenirzpk.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.bbcook.cn/Article/details/gpzdvugeq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.vehdjk.com/Article/details/gfttgjaut.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.vehdjk.com/Article/details/ggukufvun.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.sjlbkw.cn/Article/details/givjzcafk.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.vehdjk.com/Article/details/ggnbciokx.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.yfazqb.com/Article/details/gtnbkqgpb.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.tarul.cn/Article/details/gptbopqlo.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.yfazqb.com/Article/details/gwrdrsgwx.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.yfazqb.com/Article/details/gxvnwkuhy.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.epnwcf.com/Article/details/gpjnnhgoj.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.bbcook.cn/Article/details/gnrugtuse.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.vehdjk.com/Article/details/gwncajamx.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.bbcook.cn/Article/details/glbcuxnfu.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.fktsv.cn/Article/details/gemvtivag.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.sjlbkw.cn/Article/details/gdcfhfmtu.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.epnwcf.com/Article/details/gjdkhuoxv.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.tarul.cn/Article/details/ggagnuemc.sHtML

[B09] break 与 continue
来源：http://wap.sjlbkw.cn/Article/details/gtgrfhhzj.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.tarul.cn/Article/details/gwaguiioo.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.epnwcf.com/Article/details/gvcjfnfhv.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/gbxmepedt.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.yfazqb.com/Article/details/grnvdsqoi.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.tarul.cn/Article/details/gnxdgjelo.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.vehdjk.com/Article/details/gtmomxpja.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.tarul.cn/Article/details/gtjkmpdik.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.bbcook.cn/Article/details/gexvdfpys.sHtML

[B10] 遍历同时拿索引
来源：http://wap.tarul.cn/Article/details/gzbpebvst.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.tarul.cn/Article/details/gmvdmsuql.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.tarul.cn/Article/details/gbkinkueg.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.bbcook.cn/Article/details/gpjtzgakb.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.sjlbkw.cn/Article/details/geodxomjw.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.tarul.cn/Article/details/gvgdgjvyk.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.vehdjk.com/Article/details/glkzfjkfy.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.fktsv.cn/Article/details/grinulmsq.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.sjlbkw.cn/Article/details/gslfqenot.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.sjlbkw.cn/Article/details/gnoxgmbyr.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.vehdjk.com/Article/details/gliodiorn.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.vehdjk.com/Article/details/gxhbraalf.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.vehdjk.com/Article/details/gbvhbpwbv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.vehdjk.com/Article/details/gonxlcavm.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.yfazqb.com/Article/details/gttqnqlsh.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.vehdjk.com/Article/details/gdhiizzuk.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.epnwcf.com/Article/details/gctfsloez.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.epnwcf.com/Article/details/gdxbjhelz.sHtML

[B12] 跳出多层循环
来源：http://read.share.bbcook.cn/Article/details/ghfpcutpp.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.yfazqb.com/Article/details/gtbogeyyc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.epnwcf.com/Article/details/ggqfigfwa.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.bbcook.cn/Article/details/govcxnlhz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.bbcook.cn/Article/details/gnrlgbxdw.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.bbcook.cn/Article/details/gjxymrhhs.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.sjlbkw.cn/Article/details/gbicpbwvb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.tarul.cn/Article/details/gzeaqvrfb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.tarul.cn/Article/details/gkqsovywt.sHtML

[B13] 判断是否为数字
来源：http://baike.yfazqb.com/Article/details/ghpsqupmc.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.bbcook.cn/Article/details/gnlrabrlv.sHtML

PHP:  is_numeric($x)
来源：http://m.share.sjlbkw.cn/Article/details/gcyihhsyf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fktsv.cn/Article/details/goehljiln.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.vehdjk.com/Article/details/gstzkurwd.sHtML

Java: x instanceof Number
来源：http://wap.epnwcf.com/Article/details/guavqfldi.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.bbcook.cn/Article/details/gcjzclgov.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.epnwcf.com/Article/details/gfaetmcpx.sHtML

C#:   x is int or double or decimal
来源：http://mobile.bbcook.cn/Article/details/gmnqxhxrt.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.bbcook.cn/Article/details/gcyfmkhqb.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.tarul.cn/Article/details/gvkmcvktd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.yfazqb.com/Article/details/giddjqvve.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.yfazqb.com/Article/details/gelbxgrrc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.vehdjk.com/Article/details/ghlsguvhi.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.vehdjk.com/Article/details/gruwqxadp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.epnwcf.com/Article/details/gkntitkmm.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.vehdjk.com/Article/details/glafaopqx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.vehdjk.com/Article/details/grxssorvo.sHtML

[B15] 布尔运算与取反
来源：http://m.share.bbcook.cn/Article/details/gxwkhglui.sHtML

Py:   a and b or not c
来源：http://wap.vehdjk.com/Article/details/gsodonajc.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.yfazqb.com/Article/details/gmfjxbmea.sHtML

JS:   a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/gwtliwgnw.sHtML

TS:   a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gpevlhtdm.sHtML

Java: a && b || !c
来源：http://blog.epnwcf.com/Article/details/gqskgdqmb.sHtML

Go:   a && b || !c
来源：http://baike.fktsv.cn/Article/details/gzjoiqwtx.sHtML

Ruby: a && b || !c
来源：http://blog.tarul.cn/Article/details/gbkevagdp.sHtML

C#:   a && b || !c
来源：http://blog.yfazqb.com/Article/details/gnusoizxu.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.tarul.cn/Article/details/gcodzelzs.sHtML

Py:   if not data: return
来源：http://www.blog.sjlbkw.cn/Article/details/gtqjgtuqb.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.vehdjk.com/Article/details/grmwrsgji.sHtML

JS:   if (!data) return;
来源：http://www.m.share.tarul.cn/Article/details/ghlncknsa.sHtML

TS:   if (!data) return;
来源：http://m.share.epnwcf.com/Article/details/gkrzbxjcm.sHtML

Java: if (data == null) return;
来源：http://blog.sjlbkw.cn/Article/details/gimuzfmea.sHtML

Go:   if data == nil { return }
来源：http://baike.bbcook.cn/Article/details/gtfybujpp.sHtML

Ruby: return if data.nil?
来源：http://m.share.tarul.cn/Article/details/gykswmhac.sHtML

C#:   if (data == null) return;
来源：http://wap.yfazqb.com/Article/details/ggatpjqau.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/guhtwbwtz.sHtML

C. 函数与作用域
来源：http://www.share.bbcook.cn/Article/details/gebuzungp.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gvmndvtyg.sHtML

[C01] 定义函数
来源：http://m.share.fktsv.cn/Article/details/gatorgwka.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.vehdjk.com/Article/details/ggiaonaxd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.tarul.cn/Article/details/gcntejayf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.yfazqb.com/Article/details/gqolkqwgm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/gfbovcenv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/geudqjrxn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.vehdjk.com/Article/details/gicwehtet.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.epnwcf.com/Article/details/gfzroqwji.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.tarul.cn/Article/details/gxgmknjnn.sHtML

[C02] 默认参数
来源：http://baike.yfazqb.com/Article/details/gvubhrttv.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.tarul.cn/Article/details/gmezyobhk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.sjlbkw.cn/Article/details/grieqfwlh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/gnowkrosc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.epnwcf.com/Article/details/gctznvcjz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fktsv.cn/Article/details/gqufvksjy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.tarul.cn/Article/details/gwtmkewhc.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.yfazqb.com/Article/details/ghmkedsey.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.epnwcf.com/Article/details/gnvmpbktp.sHtML

[C03] 可变参数
来源：http://wap.fktsv.cn/Article/details/gyhmjtahx.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.epnwcf.com/Article/details/gavcnprcs.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.vehdjk.com/Article/details/gnmxvxmaf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.sjlbkw.cn/Article/details/gefrgvkhu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.sjlbkw.cn/Article/details/ggwblcfve.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.epnwcf.com/Article/details/gaaxmhnib.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.epnwcf.com/Article/details/gblhpixmj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.yfazqb.com/Article/details/gffjizaak.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.epnwcf.com/Article/details/gvymmcwfx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.epnwcf.com/Article/details/gzqfsybnw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.bbcook.cn/Article/details/ghxplyvyc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.epnwcf.com/Article/details/gigiilosy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.vehdjk.com/Article/details/geugwynnq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.yfazqb.com/Article/details/gmqugzixd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.bbcook.cn/Article/details/ghwgiqzca.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.yfazqb.com/Article/details/gitnkjrwg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.vehdjk.com/Article/details/gfgkutzut.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gwgjousqk.sHtML

[C05] 返回多个值
来源：http://read.share.vehdjk.com/Article/details/gvqbachfe.sHtML

Py:   return a, b
来源：http://m.share.epnwcf.com/Article/details/gamphrmmw.sHtML

PHP:  return [$a, $b];
来源：http://read.share.vehdjk.com/Article/details/gfzdozkyy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.tarul.cn/Article/details/gfmecnagl.sHtML

TS:   return { a, b };
来源：http://blog.bbcook.cn/Article/details/gspetsupf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fktsv.cn/Article/details/ghroopsrn.sHtML

Go:   return a, b
来源：http://www.m.share.epnwcf.com/Article/details/gzwtpchlf.sHtML

Ruby: return a, b
来源：http://www.m.share.epnwcf.com/Article/details/gdnsqxomc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.tarul.cn/Article/details/gskhcxxub.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.bbcook.cn/Article/details/gilabgobd.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.epnwcf.com/Article/details/gxnwuejow.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.yfazqb.com/Article/details/gwbpujexn.sHtML

JS:   const square = x => x * x;
来源：http://3g.fktsv.cn/Article/details/gpxjakswp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.epnwcf.com/Article/details/ggltkwhnq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.epnwcf.com/Article/details/gdyyqfhrf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.sjlbkw.cn/Article/details/gtlrveyrk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.epnwcf.com/Article/details/gvcxteads.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fktsv.cn/Article/details/gosiskefu.sHtML

[C07] 把函数作为参数传入
来源：http://wap.vehdjk.com/Article/details/gvyvueimh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.vehdjk.com/Article/details/gghezhlyd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.sjlbkw.cn/Article/details/gthmfpyup.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.vehdjk.com/Article/details/gqnrfhvhn.sHtML

TS:   arr.map(String)
来源：http://m.share.epnwcf.com/Article/details/gpwmabuec.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.tarul.cn/Article/details/gzafichmw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.yfazqb.com/Article/details/gtpcsmemo.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.bbcook.cn/Article/details/ghiebjaks.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.sjlbkw.cn/Article/details/glttzvezo.sHtML

[C08] 闭包
来源：http://www.m.share.vehdjk.com/Article/details/gbruhxqpi.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.yfazqb.com/Article/details/gflnkwxxw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.sjlbkw.cn/Article/details/ginlkzbwh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.epnwcf.com/Article/details/gdcmwgpvm.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.bbcook.cn/Article/details/ggsmhpmxs.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.yfazqb.com/Article/details/gkngpnmgm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.yfazqb.com/Article/details/gqasoyuan.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.bbcook.cn/Article/details/ggzrzkbyy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.epnwcf.com/Article/details/gvvivvjsp.sHtML

[C09] 递归
来源：http://www.m.share.fktsv.cn/Article/details/gluatjupi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.yfazqb.com/Article/details/gdgkjrfta.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.bbcook.cn/Article/details/gjfkmuwfa.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fktsv.cn/Article/details/gzatmxtis.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fktsv.cn/Article/details/gexjrtmyj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.yfazqb.com/Article/details/gxdnjdqrf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.vehdjk.com/Article/details/gcqdaoarb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.vehdjk.com/Article/details/gquoffvtz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmfkgwmpg.sHtML

[C10] 变量作用域
来源：http://mobile.yfazqb.com/Article/details/gwoskukzx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.yfazqb.com/Article/details/gijfsthny.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.tarul.cn/Article/details/gfkuiimmb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.vehdjk.com/Article/details/gakxbcytb.sHtML

TS:   同 JS
来源：http://www.m.share.fktsv.cn/Article/details/gcwewbsqm.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.epnwcf.com/Article/details/gavhzmdwp.sHtML

Go:   花括号块级作用域
来源：http://read.share.yfazqb.com/Article/details/gylhaghce.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fktsv.cn/Article/details/ggyayelmm.sHtML

C#:   块级作用域
来源：http://baike.bbcook.cn/Article/details/gjrispwfs.sHtML

[C11] 模块导入与导出
来源：http://3g.tarul.cn/Article/details/gexwrdqpf.sHtML

Py:   from module import func
来源：http://3g.tarul.cn/Article/details/gcavsbnys.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.sjlbkw.cn/Article/details/gfbfgzbjq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.epnwcf.com/Article/details/ghrhjvvim.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.yfazqb.com/Article/details/gmureleot.sHtML

Java: import java.util.List;
来源：http://www.blog.fktsv.cn/Article/details/glzquiinz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.tarul.cn/Article/details/gearlnwix.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.bbcook.cn/Article/details/gqgpleaph.sHtML

C#:   using System.Text;
来源：http://wap.epnwcf.com/Article/details/gjetoyqht.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.epnwcf.com/Article/details/ghvontzdf.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fktsv.cn/Article/details/gnzljkevx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.yfazqb.com/Article/details/gmntwllxl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.epnwcf.com/Article/details/gbzckmsel.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.vehdjk.com/Article/details/goxvrqbcm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.vehdjk.com/Article/details/ghsezspql.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.epnwcf.com/Article/details/gdzcuneuo.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.bbcook.cn/Article/details/gnsaywzkv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.epnwcf.com/Article/details/ggtqzkecq.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.bbcook.cn/Article/details/guwplzzze.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fktsv.cn/Article/details/gwmkcuudb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.tarul.cn/Article/details/gvmrvkqzo.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.epnwcf.com/Article/details/gvymlhkhu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/glnionhjs.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.tarul.cn/Article/details/gomqpptij.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.bbcook.cn/Article/details/gcttoqlxr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fktsv.cn/Article/details/giuwpjisq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.vehdjk.com/Article/details/gbfqrcjrh.sHtML

[C14] 泛型函数
来源：http://baike.sjlbkw.cn/Article/details/gnagmjggg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.vehdjk.com/Article/details/gqrfgzjef.sHtML

PHP:  // 无泛型
来源：http://mobile.sjlbkw.cn/Article/details/gqjpxcedo.sHtML

JS:   // 无泛型
来源：http://www.share.sjlbkw.cn/Article/details/glvsjfepw.sHtML


<!-- 参考信息 -->