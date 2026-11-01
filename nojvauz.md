代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.sjlbkw.cn/Article/details/gksyafppv.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.bbcook.cn/Article/details/gjdvyynaq.sHtML

[A24] 去除首尾空白
来源：http://mobile.yfazqb.com/Article/details/goxnntsdc.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.bbcook.cn/Article/details/gswqbskoy.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.sjlbkw.cn/Article/details/gottslmyx.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.vehdjk.com/Article/details/gfyvmqcyv.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.epnwcf.com/Article/details/gqoduuuma.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.sjlbkw.cn/Article/details/gxefgbjek.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.epnwcf.com/Article/details/gmfdqkteh.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.fktsv.cn/Article/details/gfgttjggb.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.sjlbkw.cn/Article/details/gkdzbiqgf.sHtML

[A25] 字符串比较
来源：http://read.share.epnwcf.com/Article/details/gjkyseoot.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.tarul.cn/Article/details/gdznosfym.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.epnwcf.com/Article/details/gufalzgyh.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.bbcook.cn/Article/details/gvwpsggky.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fktsv.cn/Article/details/gffausngh.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.epnwcf.com/Article/details/ggjcossjo.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.vehdjk.com/Article/details/guxmczbef.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.vehdjk.com/Article/details/gyytgzauq.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.sjlbkw.cn/Article/details/gqzzcokkd.sHtML

[A26] 类型转换总览
来源：http://baike.bbcook.cn/Article/details/guhufdijc.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.vehdjk.com/Article/details/gnimgxdah.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.fktsv.cn/Article/details/gkdthopzk.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.yfazqb.com/Article/details/gtmcysutt.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.epnwcf.com/Article/details/gylihsmlw.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.epnwcf.com/Article/details/gqepscpow.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.fktsv.cn/Article/details/grasnwxjs.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.epnwcf.com/Article/details/gyaxeuhln.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.tarul.cn/Article/details/gjlwubnyr.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gbjzuizad.sHtML

B. 流程控制
来源：http://www.share.bbcook.cn/Article/details/gxvxhxedn.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gcalachlx.sHtML

[B01] 条件判断 if / else
来源：http://www.share.tarul.cn/Article/details/gpgjatnwy.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.tarul.cn/Article/details/goikmzouk.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.tarul.cn/Article/details/gsnrpzpil.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.yfazqb.com/Article/details/gcmwxhcav.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fktsv.cn/Article/details/gefpwpgpa.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.bbcook.cn/Article/details/gcwjsnrxq.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.fktsv.cn/Article/details/goboftacv.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.bbcook.cn/Article/details/gzfnsywyp.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.bbcook.cn/Article/details/ghxizbkbs.sHtML

[B02] 多分支 else if / elif
来源：http://baike.bbcook.cn/Article/details/gtunulkls.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.fktsv.cn/Article/details/gxollxufz.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.bbcook.cn/Article/details/gcvbwvxpr.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.epnwcf.com/Article/details/gmrhqqmgr.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.bbcook.cn/Article/details/gaszdpzdo.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.bbcook.cn/Article/details/geolnilaa.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.fktsv.cn/Article/details/gvlbqqiyc.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.fktsv.cn/Article/details/godmnezql.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fktsv.cn/Article/details/gllxnlcrm.sHtML

[B03] switch / match / case
来源：http://wap.tarul.cn/Article/details/gofemwtnb.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.bbcook.cn/Article/details/gsdblducg.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/glfenctpe.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.bbcook.cn/Article/details/gkfzgcfic.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.vehdjk.com/Article/details/gioewmubt.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.fktsv.cn/Article/details/gxpqgrnwd.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.bbcook.cn/Article/details/ggpcjhfvt.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.epnwcf.com/Article/details/gmpgkihqy.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.bbcook.cn/Article/details/gzzcpcocc.sHtML

[B04] for 计数循环
来源：http://mobile.vehdjk.com/Article/details/gvldfgtyw.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.fktsv.cn/Article/details/gbkkfpokq.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.yfazqb.com/Article/details/gcctgnugl.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.vehdjk.com/Article/details/gfrnnnjty.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.sjlbkw.cn/Article/details/gezdmidsj.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.epnwcf.com/Article/details/gvesgzdzi.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.sjlbkw.cn/Article/details/gxeahqpia.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.bbcook.cn/Article/details/gdshrvvog.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.fktsv.cn/Article/details/gmrtcpluc.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.tarul.cn/Article/details/gkhumzntt.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.sjlbkw.cn/Article/details/gnrunfcpw.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.bbcook.cn/Article/details/gwcjytfvr.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.tarul.cn/Article/details/gxoxdiooq.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.bbcook.cn/Article/details/gkgnxhlcl.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.vehdjk.com/Article/details/gkkrxktew.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.epnwcf.com/Article/details/gvljfmtfp.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.yfazqb.com/Article/details/gqluavyas.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.yfazqb.com/Article/details/grenaaqth.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.epnwcf.com/Article/details/gosrezokx.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.bbcook.cn/Article/details/ggfqlblvh.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.yfazqb.com/Article/details/ghfgtlifx.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fktsv.cn/Article/details/gxtiyfncq.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.vehdjk.com/Article/details/gczhcjfuz.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.fktsv.cn/Article/details/ghkyocvjz.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.yfazqb.com/Article/details/gfmzoehki.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.yfazqb.com/Article/details/gzsaerayg.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.yfazqb.com/Article/details/gkobpsuri.sHtML

[B07] while 循环
来源：http://baike.tarul.cn/Article/details/gakhmzklu.sHtML

Py:   while i < 10: i += 1
来源：http://baike.bbcook.cn/Article/details/gktekncdk.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.vehdjk.com/Article/details/ganddmphp.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.vehdjk.com/Article/details/ggzprdsqu.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.sjlbkw.cn/Article/details/glqsrqzvo.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.yfazqb.com/Article/details/gmyaxbpug.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.bbcook.cn/Article/details/gzxxirfdi.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.epnwcf.com/Article/details/gmbspullc.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.tarul.cn/Article/details/gwglgtsul.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.bbcook.cn/Article/details/gjwpstvog.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.vehdjk.com/Article/details/gqwhllrmi.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.fktsv.cn/Article/details/gkefthyvh.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.vehdjk.com/Article/details/gfpxdjimt.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.epnwcf.com/Article/details/gghszxftl.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.epnwcf.com/Article/details/gxxqphkwm.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.epnwcf.com/Article/details/ghtwiwnqb.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.bbcook.cn/Article/details/gdvyfphpd.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.sjlbkw.cn/Article/details/gfqoxhyyw.sHtML

[B09] break 与 continue
来源：http://www.share.epnwcf.com/Article/details/genzibwhf.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.sjlbkw.cn/Article/details/gvtolskhq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.bbcook.cn/Article/details/gdaxnvgut.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fktsv.cn/Article/details/gzouzsdhf.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.epnwcf.com/Article/details/gojonxawv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.epnwcf.com/Article/details/gvlmuugbx.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.bbcook.cn/Article/details/goybwqhwh.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.sjlbkw.cn/Article/details/gxoukfkzr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.sjlbkw.cn/Article/details/gqdekhzvk.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.yfazqb.com/Article/details/gstunbbam.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.epnwcf.com/Article/details/guwynvzou.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.yfazqb.com/Article/details/ghytgdhzb.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.sjlbkw.cn/Article/details/gkwkbeumr.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.epnwcf.com/Article/details/gbsteqiet.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.epnwcf.com/Article/details/gshqxbnah.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.yfazqb.com/Article/details/gkufvxmdj.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.bbcook.cn/Article/details/gjbnrmaya.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.epnwcf.com/Article/details/gnpefadoz.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.bbcook.cn/Article/details/gdziawkrf.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.fktsv.cn/Article/details/goookvjny.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.epnwcf.com/Article/details/gcgeljhzo.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.vehdjk.com/Article/details/greqwdoow.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.yfazqb.com/Article/details/glqfulgup.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.epnwcf.com/Article/details/gwfrnvhpn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.bbcook.cn/Article/details/glogvxfqm.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.bbcook.cn/Article/details/godwcfnlm.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.tarul.cn/Article/details/gdhkiojqc.sHtML

[B12] 跳出多层循环
来源：http://baike.sjlbkw.cn/Article/details/ghadhqxpd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.fktsv.cn/Article/details/gwqioalkx.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.fktsv.cn/Article/details/gqthileqg.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.yfazqb.com/Article/details/gvhxkvlkr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.yfazqb.com/Article/details/grkengxzo.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.bbcook.cn/Article/details/gkgliflwd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.vehdjk.com/Article/details/gbztbekuz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.sjlbkw.cn/Article/details/gxocgscol.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.epnwcf.com/Article/details/gxpsxzfhp.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.tarul.cn/Article/details/gfurcamcb.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.vehdjk.com/Article/details/gxnxneyiz.sHtML

PHP:  is_numeric($x)
来源：http://m.share.sjlbkw.cn/Article/details/gpvkqcrmq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.sjlbkw.cn/Article/details/gxxpgxdmd.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.tarul.cn/Article/details/gyiwdhsjl.sHtML

Java: x instanceof Number
来源：http://blog.yfazqb.com/Article/details/garoiihkj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.sjlbkw.cn/Article/details/gteucbwhf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.vehdjk.com/Article/details/gjnbxagck.sHtML

C#:   x is int or double or decimal
来源：http://www.share.yfazqb.com/Article/details/gpwjqkqxy.sHtML

[B14] 判断值是否在集合内
来源：http://baike.bbcook.cn/Article/details/gbrczrhdb.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.sjlbkw.cn/Article/details/ggcgotflb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.tarul.cn/Article/details/gasbwbwnc.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.bbcook.cn/Article/details/gorhnydxp.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.vehdjk.com/Article/details/gzzilwwgd.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.vehdjk.com/Article/details/guwcdpjpj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.bbcook.cn/Article/details/geghcmmex.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.tarul.cn/Article/details/gpqqmsxco.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.sjlbkw.cn/Article/details/gnlunacbm.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.yfazqb.com/Article/details/gsnndbgrl.sHtML

Py:   a and b or not c
来源：http://www.blog.yfazqb.com/Article/details/gbyxklmru.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.epnwcf.com/Article/details/gmhurfeia.sHtML

JS:   a && b || !c
来源：http://m.share.fktsv.cn/Article/details/gjfqhmvdn.sHtML

TS:   a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gmpxqdyrd.sHtML

Java: a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gezomquls.sHtML

Go:   a && b || !c
来源：http://read.share.epnwcf.com/Article/details/gldtiwatn.sHtML

Ruby: a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/gxyfzbdpz.sHtML

C#:   a && b || !c
来源：http://baike.bbcook.cn/Article/details/gyzsqrsef.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.epnwcf.com/Article/details/gzdpdqnqj.sHtML

Py:   if not data: return
来源：http://read.share.epnwcf.com/Article/details/giiyadmkl.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.fktsv.cn/Article/details/ghzfjifny.sHtML

JS:   if (!data) return;
来源：http://blog.bbcook.cn/Article/details/gsyozbtez.sHtML

TS:   if (!data) return;
来源：http://read.share.tarul.cn/Article/details/gvodthpws.sHtML

Java: if (data == null) return;
来源：http://www.share.yfazqb.com/Article/details/gnlvsqlry.sHtML

Go:   if data == nil { return }
来源：http://www.share.bbcook.cn/Article/details/gmmouwtii.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.bbcook.cn/Article/details/gitghmldb.sHtML

C#:   if (data == null) return;
来源：http://www.share.tarul.cn/Article/details/gapblmgyf.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gwzzrsqwd.sHtML

C. 函数与作用域
来源：http://m.share.tarul.cn/Article/details/gkpmnziac.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gjyfhaodl.sHtML

[C01] 定义函数
来源：http://www.share.epnwcf.com/Article/details/gbxmbpjcw.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.bbcook.cn/Article/details/gybgpeftw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.yfazqb.com/Article/details/gamdtaoux.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/grpdmuqjs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gmsiomoue.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/gtbujnivd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.bbcook.cn/Article/details/gxmxtfzjp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fktsv.cn/Article/details/gvgmbtniw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/gflmxvswx.sHtML

[C02] 默认参数
来源：http://read.share.vehdjk.com/Article/details/gjtkstpin.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.vehdjk.com/Article/details/gtmvhnnss.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.yfazqb.com/Article/details/gtaqubxrf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.sjlbkw.cn/Article/details/gmwryoybb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.epnwcf.com/Article/details/gpqchxhby.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.vehdjk.com/Article/details/gxemujpom.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fktsv.cn/Article/details/guyvjuxbs.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.epnwcf.com/Article/details/grmipjeem.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.sjlbkw.cn/Article/details/gblcjtsti.sHtML

[C03] 可变参数
来源：http://m.share.bbcook.cn/Article/details/ghfmeweev.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.bbcook.cn/Article/details/ggjfuhqvs.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.tarul.cn/Article/details/gnfwsryqz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.yfazqb.com/Article/details/gkqkjyoeu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.bbcook.cn/Article/details/gwovtgoqs.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.yfazqb.com/Article/details/gnhgehrjc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.bbcook.cn/Article/details/gfkaswcgj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.yfazqb.com/Article/details/gxnkyvmyy.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fktsv.cn/Article/details/gqajxzooj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fktsv.cn/Article/details/ggdulobwm.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.bbcook.cn/Article/details/gnodctfmg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.yfazqb.com/Article/details/geogkdvvi.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.sjlbkw.cn/Article/details/gcxwamljz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.epnwcf.com/Article/details/gtyqnuhpl.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.epnwcf.com/Article/details/gdklgzftv.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.tarul.cn/Article/details/gouvbdljo.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fktsv.cn/Article/details/gnauuaxjj.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.sjlbkw.cn/Article/details/grymrieyf.sHtML

[C05] 返回多个值
来源：http://baike.tarul.cn/Article/details/gsnykdgnh.sHtML

Py:   return a, b
来源：http://www.m.share.vehdjk.com/Article/details/gtjxezsvl.sHtML

PHP:  return [$a, $b];
来源：http://wap.bbcook.cn/Article/details/gdsaxqdhj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.vehdjk.com/Article/details/gjqoyubko.sHtML

TS:   return { a, b };
来源：http://blog.yfazqb.com/Article/details/gybfxkclj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.tarul.cn/Article/details/gtpupxqxl.sHtML

Go:   return a, b
来源：http://wap.sjlbkw.cn/Article/details/guymwwqyo.sHtML

Ruby: return a, b
来源：http://read.share.bbcook.cn/Article/details/glkbqiaze.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.tarul.cn/Article/details/gcbnltijp.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.bbcook.cn/Article/details/gynzwjykw.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.tarul.cn/Article/details/gkbvtzhjo.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.vehdjk.com/Article/details/gkddhotex.sHtML

JS:   const square = x => x * x;
来源：http://mobile.bbcook.cn/Article/details/gvsmhdwoq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.tarul.cn/Article/details/gjbcnlzdh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.bbcook.cn/Article/details/gkipxmhew.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.vehdjk.com/Article/details/gmoftbunh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.yfazqb.com/Article/details/gmjesltjb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.fktsv.cn/Article/details/gpntsrmue.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.tarul.cn/Article/details/gpokufqzs.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.yfazqb.com/Article/details/ghfrkkarf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.bbcook.cn/Article/details/ghxjwfxog.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.vehdjk.com/Article/details/gguqvkiju.sHtML

TS:   arr.map(String)
来源：http://blog.fktsv.cn/Article/details/gvawginyp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.vehdjk.com/Article/details/gykzujond.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.fktsv.cn/Article/details/ganaszrtf.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.sjlbkw.cn/Article/details/gnrucnzjc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.yfazqb.com/Article/details/gecaovoxz.sHtML

[C08] 闭包
来源：http://baike.bbcook.cn/Article/details/gfuxqslpq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.yfazqb.com/Article/details/gusserttn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.vehdjk.com/Article/details/gjohywvcp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.epnwcf.com/Article/details/gzxaiqamb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fktsv.cn/Article/details/grstzxwii.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.bbcook.cn/Article/details/gijrolrrk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fktsv.cn/Article/details/gkjlvaicd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.tarul.cn/Article/details/gfxutjogs.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.yfazqb.com/Article/details/ggkextqew.sHtML

[C09] 递归
来源：http://read.share.vehdjk.com/Article/details/ggtcywisd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.epnwcf.com/Article/details/gzpeewniq.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.bbcook.cn/Article/details/grhxogeij.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.vehdjk.com/Article/details/grmhqedyl.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.yfazqb.com/Article/details/gwbeywrdw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.yfazqb.com/Article/details/gwdzglshl.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.epnwcf.com/Article/details/grwmndczi.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fktsv.cn/Article/details/gepdzjxjb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.tarul.cn/Article/details/gmirilcsz.sHtML

[C10] 变量作用域
来源：http://read.share.epnwcf.com/Article/details/gflrlmpqt.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.tarul.cn/Article/details/grbxvzftz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.yfazqb.com/Article/details/gmiabcfgh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.yfazqb.com/Article/details/gxusmiaif.sHtML

TS:   同 JS
来源：http://www.m.share.epnwcf.com/Article/details/gbsqzkdkd.sHtML

Java: 方法内为块级作用域
来源：http://www.share.bbcook.cn/Article/details/gaubgitiy.sHtML

Go:   花括号块级作用域
来源：http://mobile.bbcook.cn/Article/details/gvzqqzpim.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.epnwcf.com/Article/details/gxwcdyqdo.sHtML

C#:   块级作用域
来源：http://baike.fktsv.cn/Article/details/gohklusjf.sHtML

[C11] 模块导入与导出
来源：http://mobile.tarul.cn/Article/details/gekbfrntu.sHtML

Py:   from module import func
来源：http://wap.vehdjk.com/Article/details/gvlvnrimh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.yfazqb.com/Article/details/gaejxatbq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.yfazqb.com/Article/details/gphmiuxqt.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.yfazqb.com/Article/details/ggxlmhbam.sHtML

Java: import java.util.List;
来源：http://mobile.tarul.cn/Article/details/gahjtcmub.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.bbcook.cn/Article/details/gkpejojhd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.epnwcf.com/Article/details/gqqgzhids.sHtML

C#:   using System.Text;
来源：http://www.blog.vehdjk.com/Article/details/glvtratlx.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.sjlbkw.cn/Article/details/gsbthrjkb.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fktsv.cn/Article/details/ggitndbjt.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.bbcook.cn/Article/details/gcciftboj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.yfazqb.com/Article/details/gnoymuzxs.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.bbcook.cn/Article/details/gfmxcalte.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.tarul.cn/Article/details/gzsfyjpjj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.tarul.cn/Article/details/gvkeneukn.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.tarul.cn/Article/details/glysqgkig.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.epnwcf.com/Article/details/gutcaezol.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.yfazqb.com/Article/details/gxkusebcz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.sjlbkw.cn/Article/details/grtqcegfd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.sjlbkw.cn/Article/details/gtxpzqaju.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.vehdjk.com/Article/details/gewtmbqqv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/gwaetamfy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/gtjltmsoy.sHtML

Go:   func add(a, b int) int
来源：http://blog.tarul.cn/Article/details/gjewgvmuo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.vehdjk.com/Article/details/gnvdbfzae.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.bbcook.cn/Article/details/garkuezjz.sHtML

[C14] 泛型函数
来源：http://blog.epnwcf.com/Article/details/gltaniloo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.vehdjk.com/Article/details/gljpfhfba.sHtML

PHP:  // 无泛型
来源：http://mobile.fktsv.cn/Article/details/gtlznlohj.sHtML

JS:   // 无泛型
来源：http://3g.vehdjk.com/Article/details/gqnmxwdrd.sHtML


<!-- 参考信息 -->