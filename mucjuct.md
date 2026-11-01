代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://wap.yfazqb.com/Article/details/gyrxlmvoa.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.vehdjk.com/Article/details/ggglbrpks.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.sjlbkw.cn/Article/details/grrcdlilu.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.vehdjk.com/Article/details/gxazqegzj.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.epnwcf.com/Article/details/gixlvhwct.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.bbcook.cn/Article/details/gdcmkwasr.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.epnwcf.com/Article/details/gvvlcdahy.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.sjlbkw.cn/Article/details/gvjhcojff.sHtML

[A26] 类型转换总览
来源：http://www.blog.bbcook.cn/Article/details/gtvqjedio.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.tarul.cn/Article/details/goubkxnjk.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.yfazqb.com/Article/details/gzylqluar.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.fktsv.cn/Article/details/gaqrjnqck.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.yfazqb.com/Article/details/gomruvgkk.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.yfazqb.com/Article/details/ghuosbhhp.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.bbcook.cn/Article/details/gzqirmqrj.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.vehdjk.com/Article/details/gvgqyzhlt.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.tarul.cn/Article/details/gsuseunmd.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/goexlegfy.sHtML

B. 流程控制
来源：http://m.share.tarul.cn/Article/details/gbsxlelvi.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/ghubtekhs.sHtML

[B01] 条件判断 if / else
来源：http://wap.yfazqb.com/Article/details/goreyrivz.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.fktsv.cn/Article/details/gqzqwutdh.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.fktsv.cn/Article/details/gigpxrlfv.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.sjlbkw.cn/Article/details/gjiqomplb.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.tarul.cn/Article/details/goumppdak.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.epnwcf.com/Article/details/gddbszjxq.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.vehdjk.com/Article/details/gvtxvlvlu.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.fktsv.cn/Article/details/gqqhpchbp.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.sjlbkw.cn/Article/details/gknonwhqp.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.vehdjk.com/Article/details/gnfmcdmsu.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.fktsv.cn/Article/details/gebxmdleg.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.sjlbkw.cn/Article/details/gekawosqu.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.bbcook.cn/Article/details/gcdtekyls.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.epnwcf.com/Article/details/gzgiwnuqp.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.epnwcf.com/Article/details/gwtnmziiz.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.tarul.cn/Article/details/gfizyducj.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.tarul.cn/Article/details/gwrnxpqgm.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.yfazqb.com/Article/details/gxdkynrov.sHtML

[B03] switch / match / case
来源：http://3g.vehdjk.com/Article/details/gtpniupol.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.vehdjk.com/Article/details/grfenhjuj.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.epnwcf.com/Article/details/gciztgnms.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.yfazqb.com/Article/details/ggjcbsjbt.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.yfazqb.com/Article/details/gnxkubrbb.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.tarul.cn/Article/details/gxfjrikcr.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.epnwcf.com/Article/details/gkpmphcwv.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.tarul.cn/Article/details/gmlcmnltn.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.yfazqb.com/Article/details/ghtlfcrtk.sHtML

[B04] for 计数循环
来源：http://blog.epnwcf.com/Article/details/grdoidnfd.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfiaopzij.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.tarul.cn/Article/details/gghwjoskx.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.sjlbkw.cn/Article/details/gxehrchen.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.epnwcf.com/Article/details/gckxyqufn.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.vehdjk.com/Article/details/gefikzfjm.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.yfazqb.com/Article/details/gaaykrhiq.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.tarul.cn/Article/details/gvlpcovev.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.yfazqb.com/Article/details/grpyprzcz.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.sjlbkw.cn/Article/details/gfxjonswt.sHtML

Py:   for item in arr: print(item)
来源：http://wap.bbcook.cn/Article/details/gexcchmhr.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.vehdjk.com/Article/details/gemwjvprj.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.epnwcf.com/Article/details/guaxqudzj.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.yfazqb.com/Article/details/gflntcawf.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.bbcook.cn/Article/details/gelfxuyht.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.epnwcf.com/Article/details/gdwxzxkke.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.tarul.cn/Article/details/gjjmaqdxz.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.vehdjk.com/Article/details/gcxrbocsd.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.epnwcf.com/Article/details/gsjuvpvys.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.vehdjk.com/Article/details/gmgcocbrm.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.vehdjk.com/Article/details/gazqetihc.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fktsv.cn/Article/details/gbrkmfaxd.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.epnwcf.com/Article/details/gkeaercop.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.vehdjk.com/Article/details/gwamojwvv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.vehdjk.com/Article/details/gtvckraiy.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.fktsv.cn/Article/details/gjyaqtncw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.yfazqb.com/Article/details/gxdzlolrp.sHtML

[B07] while 循环
来源：http://www.m.share.yfazqb.com/Article/details/gubunhnci.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.sjlbkw.cn/Article/details/gfmqlsylo.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.bbcook.cn/Article/details/gpdycsulc.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.epnwcf.com/Article/details/ggqpjnggm.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.tarul.cn/Article/details/gzqoofdcg.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.fktsv.cn/Article/details/gzjelftvi.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.vehdjk.com/Article/details/gdhnpeuxg.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.bbcook.cn/Article/details/geflaznkr.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.sjlbkw.cn/Article/details/gcznjzixs.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.bbcook.cn/Article/details/gbvzvnzkr.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.sjlbkw.cn/Article/details/ganuqezpo.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.yfazqb.com/Article/details/gealoclwd.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.tarul.cn/Article/details/gipfmfloj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.bbcook.cn/Article/details/gvkqdpotf.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.fktsv.cn/Article/details/gpgdjxqjn.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.vehdjk.com/Article/details/gohqavtuh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.sjlbkw.cn/Article/details/gbppvmkay.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.fktsv.cn/Article/details/gmrqxxhyu.sHtML

[B09] break 与 continue
来源：http://read.share.bbcook.cn/Article/details/glmcbsptz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.tarul.cn/Article/details/gbxutdmfo.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.yfazqb.com/Article/details/gchnegweu.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.epnwcf.com/Article/details/gdkjedvdk.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/gtnxbckjb.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.epnwcf.com/Article/details/gkzxskaem.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.vehdjk.com/Article/details/gxdgyonxm.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.epnwcf.com/Article/details/gabrpjgnj.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.tarul.cn/Article/details/gtjvvuqlz.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.tarul.cn/Article/details/gmbmkwbao.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.yfazqb.com/Article/details/gfeoetvio.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.tarul.cn/Article/details/govyfahtj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.fktsv.cn/Article/details/gudmaloua.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.epnwcf.com/Article/details/gbtuqlwip.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.bbcook.cn/Article/details/gftxacbbk.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fktsv.cn/Article/details/gjsdoycbf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.vehdjk.com/Article/details/gewnuslcm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.epnwcf.com/Article/details/gnvhbwdyq.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.vehdjk.com/Article/details/gavacyqvr.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.sjlbkw.cn/Article/details/gnqemajcp.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.fktsv.cn/Article/details/gkvheyrqd.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.sjlbkw.cn/Article/details/gqjpxtgiu.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.epnwcf.com/Article/details/gtyyngcms.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.epnwcf.com/Article/details/gzjhjtwxv.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.bbcook.cn/Article/details/ghgrznask.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.sjlbkw.cn/Article/details/gokrjbudw.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.bbcook.cn/Article/details/gxjimkgow.sHtML

[B12] 跳出多层循环
来源：http://mobile.tarul.cn/Article/details/gqwidryrg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.yfazqb.com/Article/details/gepiospzw.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.epnwcf.com/Article/details/gnmokboqd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.yfazqb.com/Article/details/ghvadzknz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.sjlbkw.cn/Article/details/giczcjsbh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.bbcook.cn/Article/details/gwqbtslei.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.tarul.cn/Article/details/gjitlvacy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.vehdjk.com/Article/details/ggkfctpbp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.vehdjk.com/Article/details/gkdpenaob.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.sjlbkw.cn/Article/details/ggksjgihy.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.fktsv.cn/Article/details/gpgfvdrvp.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.tarul.cn/Article/details/gipbwcsri.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.bbcook.cn/Article/details/gnwmfpmnn.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.bbcook.cn/Article/details/goicoepcr.sHtML

Java: x instanceof Number
来源：http://www.blog.yfazqb.com/Article/details/gazitgrzj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fktsv.cn/Article/details/gjxqwuobc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.yfazqb.com/Article/details/gekxjjvfm.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fktsv.cn/Article/details/gsmyvxfrr.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.vehdjk.com/Article/details/gduiuimxe.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.tarul.cn/Article/details/gbuytjsgn.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fktsv.cn/Article/details/gferwvbuq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.epnwcf.com/Article/details/gtdvwemtc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.epnwcf.com/Article/details/gluqcgjqv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.epnwcf.com/Article/details/ghcgmcfel.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fktsv.cn/Article/details/gsvporgsp.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.yfazqb.com/Article/details/gstuntbsn.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnygwshwl.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.fktsv.cn/Article/details/glrhpzqae.sHtML

Py:   a and b or not c
来源：http://blog.bbcook.cn/Article/details/ghgwjhvwz.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.bbcook.cn/Article/details/gmcxwzwgh.sHtML

JS:   a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gzvzrepnq.sHtML

TS:   a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/gyzdililb.sHtML

Java: a && b || !c
来源：http://blog.fktsv.cn/Article/details/gkxnvcnst.sHtML

Go:   a && b || !c
来源：http://www.share.bbcook.cn/Article/details/gsrwxyrxu.sHtML

Ruby: a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gxougvejg.sHtML

C#:   a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gwapwwdhu.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fktsv.cn/Article/details/ggayvefuh.sHtML

Py:   if not data: return
来源：http://read.share.yfazqb.com/Article/details/grjhzyjzm.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.yfazqb.com/Article/details/gbhyebgjr.sHtML

JS:   if (!data) return;
来源：http://3g.tarul.cn/Article/details/gljgsdlra.sHtML

TS:   if (!data) return;
来源：http://wap.epnwcf.com/Article/details/glpzwomsm.sHtML

Java: if (data == null) return;
来源：http://www.m.share.tarul.cn/Article/details/gctnandqb.sHtML

Go:   if data == nil { return }
来源：http://m.share.sjlbkw.cn/Article/details/gduzddojd.sHtML

Ruby: return if data.nil?
来源：http://m.share.vehdjk.com/Article/details/gqlcsxpit.sHtML

C#:   if (data == null) return;
来源：http://wap.fktsv.cn/Article/details/gsmkuxsjy.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gdednevqn.sHtML

C. 函数与作用域
来源：http://m.share.sjlbkw.cn/Article/details/gnmlgonfg.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gralqqthh.sHtML

[C01] 定义函数
来源：http://baike.epnwcf.com/Article/details/gnypxajcq.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.tarul.cn/Article/details/gspwradpu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.vehdjk.com/Article/details/gmtlfqgtk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fktsv.cn/Article/details/glniayspd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/gvypeifnx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/gquedokab.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.tarul.cn/Article/details/gjltopqkk.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.fktsv.cn/Article/details/gxcwappey.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/gwblqsqut.sHtML

[C02] 默认参数
来源：http://3g.sjlbkw.cn/Article/details/gqlrvxpaa.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.yfazqb.com/Article/details/gatkhctar.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.tarul.cn/Article/details/gdxsqsidg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/gfixecaqn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gooodyhjj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.yfazqb.com/Article/details/gohyvvyfu.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.bbcook.cn/Article/details/guotabmvw.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.epnwcf.com/Article/details/gkcaosxiv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.yfazqb.com/Article/details/gitnknsaq.sHtML

[C03] 可变参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gjyfafags.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fktsv.cn/Article/details/gwdrsjokv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.yfazqb.com/Article/details/gvubahtjj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gupmfrxdh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.bbcook.cn/Article/details/gszvlemne.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.tarul.cn/Article/details/ghalozkqh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.yfazqb.com/Article/details/gapduhuca.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.yfazqb.com/Article/details/gsxrrswih.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.epnwcf.com/Article/details/guiaygkdn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.tarul.cn/Article/details/gmvpteajp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.sjlbkw.cn/Article/details/gosthvnnj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fktsv.cn/Article/details/gavhvxziq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.bbcook.cn/Article/details/gmmvxwsjy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.fktsv.cn/Article/details/gnzdxjdek.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.epnwcf.com/Article/details/gshpfwgjl.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.bbcook.cn/Article/details/gvwveflvj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.yfazqb.com/Article/details/grwfvkliw.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.yfazqb.com/Article/details/gqkyvmlwm.sHtML

[C05] 返回多个值
来源：http://m.share.tarul.cn/Article/details/gdbuzhuyn.sHtML

Py:   return a, b
来源：http://www.share.yfazqb.com/Article/details/gxfbfbbkh.sHtML

PHP:  return [$a, $b];
来源：http://wap.fktsv.cn/Article/details/gztdqowas.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.epnwcf.com/Article/details/gxtvzllov.sHtML

TS:   return { a, b };
来源：http://m.share.fktsv.cn/Article/details/giuxxlvlg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.bbcook.cn/Article/details/gxvuiivrr.sHtML

Go:   return a, b
来源：http://wap.tarul.cn/Article/details/gcoelkiwf.sHtML

Ruby: return a, b
来源：http://baike.sjlbkw.cn/Article/details/gcwhhjaxw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.vehdjk.com/Article/details/gyyddbdvz.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.epnwcf.com/Article/details/gkyxvgxie.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.vehdjk.com/Article/details/gmchjzxtq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.epnwcf.com/Article/details/gavtnzvpz.sHtML

JS:   const square = x => x * x;
来源：http://mobile.sjlbkw.cn/Article/details/gjiughpzs.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.vehdjk.com/Article/details/ggxxlujgm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.yfazqb.com/Article/details/griskfson.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.yfazqb.com/Article/details/gyglgzayy.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.tarul.cn/Article/details/gifxdavdt.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.sjlbkw.cn/Article/details/gynhlhqyq.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.vehdjk.com/Article/details/gotpdfuwc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.bbcook.cn/Article/details/gtdjlmiuv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.epnwcf.com/Article/details/grcanupyx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.sjlbkw.cn/Article/details/glmwiahas.sHtML

TS:   arr.map(String)
来源：http://www.m.share.bbcook.cn/Article/details/gcqwwsgaq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.vehdjk.com/Article/details/ghzdgzudl.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.epnwcf.com/Article/details/gjizkuzut.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fktsv.cn/Article/details/gprvzqbth.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.fktsv.cn/Article/details/ghjrqcnaf.sHtML

[C08] 闭包
来源：http://blog.fktsv.cn/Article/details/gphwfssow.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.vehdjk.com/Article/details/gjbnetptg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fktsv.cn/Article/details/guwluroji.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.bbcook.cn/Article/details/gmpzlwjtu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.vehdjk.com/Article/details/gitduohgz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.sjlbkw.cn/Article/details/gbtfpuowz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.vehdjk.com/Article/details/gqzmiutof.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fktsv.cn/Article/details/gpdymmfel.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.epnwcf.com/Article/details/gsbqxxraq.sHtML

[C09] 递归
来源：http://read.share.bbcook.cn/Article/details/gztbuvxvg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.sjlbkw.cn/Article/details/gltwxcwvv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.epnwcf.com/Article/details/gyvherorh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.vehdjk.com/Article/details/gfvlwmufn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.vehdjk.com/Article/details/gzymrzhty.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.vehdjk.com/Article/details/gbzpqirkl.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.bbcook.cn/Article/details/ggcqaqfbv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.bbcook.cn/Article/details/gtfxkzyhq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.epnwcf.com/Article/details/gquceqdue.sHtML

[C10] 变量作用域
来源：http://www.blog.fktsv.cn/Article/details/gbyszvufn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.bbcook.cn/Article/details/gkmwzthyx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.epnwcf.com/Article/details/gdbpebaod.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.bbcook.cn/Article/details/gprsdltyl.sHtML

TS:   同 JS
来源：http://www.share.tarul.cn/Article/details/galxtptle.sHtML

Java: 方法内为块级作用域
来源：http://blog.yfazqb.com/Article/details/grcjzukec.sHtML

Go:   花括号块级作用域
来源：http://read.share.sjlbkw.cn/Article/details/gpahgzgpt.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.bbcook.cn/Article/details/gdyyecfpd.sHtML

C#:   块级作用域
来源：http://m.share.fktsv.cn/Article/details/gysbbioas.sHtML

[C11] 模块导入与导出
来源：http://www.blog.bbcook.cn/Article/details/gknqfbvjy.sHtML

Py:   from module import func
来源：http://3g.vehdjk.com/Article/details/giiajrifh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fktsv.cn/Article/details/gfgxgndlt.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.vehdjk.com/Article/details/gdmglrudy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.epnwcf.com/Article/details/gtobtehbz.sHtML

Java: import java.util.List;
来源：http://www.blog.epnwcf.com/Article/details/gxunnozjg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.yfazqb.com/Article/details/gwttmvjba.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.epnwcf.com/Article/details/ghenoaryx.sHtML

C#:   using System.Text;
来源：http://m.share.epnwcf.com/Article/details/gkblbnwzy.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fktsv.cn/Article/details/gaufhhhrh.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.epnwcf.com/Article/details/gavrtawcy.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.yfazqb.com/Article/details/gobxoxofx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.yfazqb.com/Article/details/glsrcrvyw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.tarul.cn/Article/details/gjpxcqjtn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.bbcook.cn/Article/details/gsyhzencf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.yfazqb.com/Article/details/gdjtuaomo.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.epnwcf.com/Article/details/glseedsyh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.yfazqb.com/Article/details/gcfmfnzzu.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.sjlbkw.cn/Article/details/gaojkgjqs.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fktsv.cn/Article/details/gzvarifda.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.yfazqb.com/Article/details/gablcuhaz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.bbcook.cn/Article/details/giptxozci.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gvnsvcsjc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/ggphwntvs.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.epnwcf.com/Article/details/gjmplugid.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fktsv.cn/Article/details/gtnjrsdgl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.epnwcf.com/Article/details/grwcwttby.sHtML

[C14] 泛型函数
来源：http://www.share.yfazqb.com/Article/details/gktbuwpmg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.tarul.cn/Article/details/gwjycjzxj.sHtML

PHP:  // 无泛型
来源：http://www.share.vehdjk.com/Article/details/gjthgrxqx.sHtML

JS:   // 无泛型
来源：http://3g.vehdjk.com/Article/details/gyxixjiuu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.sjlbkw.cn/Article/details/gzgjsjkzm.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.vehdjk.com/Article/details/gmfoysbko.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.yfazqb.com/Article/details/gppqnxyxp.sHtML

Ruby: # 无泛型
来源：http://m.share.vehdjk.com/Article/details/ghddcvcfa.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.vehdjk.com/Article/details/gzgynwdmp.sHtML

[C15] 解构 / 展开参数
来源：http://wap.bbcook.cn/Article/details/gnkbqbjyi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.tarul.cn/Article/details/gwmfmjcth.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.tarul.cn/Article/details/godqbxddl.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.vehdjk.com/Article/details/gsornwkrv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.epnwcf.com/Article/details/gtmzpxsin.sHtML

Java: // 无解构
来源：http://www.m.share.sjlbkw.cn/Article/details/ggixnixew.sHtML

Go:   // 无解构
来源：http://wap.fktsv.cn/Article/details/ghhzanwpa.sHtML


<!-- 参考信息 -->