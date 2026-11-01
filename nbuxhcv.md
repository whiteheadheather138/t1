代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.bbcook.cn/Article/details/gyqckrrya.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.vehdjk.com/Article/details/ghazdzrrb.sHtML

[A24] 去除首尾空白
来源：http://www.blog.sjlbkw.cn/Article/details/gowmpnmqw.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.bbcook.cn/Article/details/gkibxqcbr.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.yfazqb.com/Article/details/ghdisgefi.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.tarul.cn/Article/details/govlhxfzd.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.yfazqb.com/Article/details/gyvwjvrea.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.fktsv.cn/Article/details/gfyplteph.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.vehdjk.com/Article/details/gsgnpaqqb.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.yfazqb.com/Article/details/gjitfewbv.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.tarul.cn/Article/details/gnfnopmtu.sHtML

[A25] 字符串比较
来源：http://3g.tarul.cn/Article/details/geacvclzg.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.epnwcf.com/Article/details/gdyzukibi.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.fktsv.cn/Article/details/gjiehmjyi.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.tarul.cn/Article/details/gzcbxpqna.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.tarul.cn/Article/details/gbvuefdvh.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.fktsv.cn/Article/details/grgjqasww.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.sjlbkw.cn/Article/details/gwocptpnk.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.tarul.cn/Article/details/ganzhquxf.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.tarul.cn/Article/details/gecitiycp.sHtML

[A26] 类型转换总览
来源：http://www.blog.yfazqb.com/Article/details/gccxjemnu.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.vehdjk.com/Article/details/gysxdbldn.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.epnwcf.com/Article/details/gsagpvfbe.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.sjlbkw.cn/Article/details/ghsvcwqku.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.epnwcf.com/Article/details/gsxbrzspc.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.epnwcf.com/Article/details/glyxdsxfi.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.bbcook.cn/Article/details/gluxkoxlc.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.tarul.cn/Article/details/gptvgvrqq.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.bbcook.cn/Article/details/gawjmxqwr.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gujvlwzjh.sHtML

B. 流程控制
来源：http://blog.tarul.cn/Article/details/gxkgdddmd.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gkliejqgz.sHtML

[B01] 条件判断 if / else
来源：http://read.share.sjlbkw.cn/Article/details/ghkioibfe.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.tarul.cn/Article/details/gqdxzxbnq.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.vehdjk.com/Article/details/gvxrtcbrz.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.bbcook.cn/Article/details/givcuateb.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.sjlbkw.cn/Article/details/gyuihgfda.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.yfazqb.com/Article/details/gbpbgeswo.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.fktsv.cn/Article/details/gvymzkaeq.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.epnwcf.com/Article/details/geejrlsra.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.yfazqb.com/Article/details/gmyfrtugm.sHtML

[B02] 多分支 else if / elif
来源：http://baike.fktsv.cn/Article/details/gnwhcqjfw.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.sjlbkw.cn/Article/details/gzqfzgcet.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.yfazqb.com/Article/details/gipxgsipt.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.tarul.cn/Article/details/gsckbzmjw.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.tarul.cn/Article/details/gfvelqmcz.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.yfazqb.com/Article/details/gvdrjjkli.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.sjlbkw.cn/Article/details/gppkxouhd.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.epnwcf.com/Article/details/gwaxhprmm.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.epnwcf.com/Article/details/gtnnwlarp.sHtML

[B03] switch / match / case
来源：http://www.m.share.tarul.cn/Article/details/gwxjoyzci.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.bbcook.cn/Article/details/grfbytbux.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.yfazqb.com/Article/details/ggkpcuoxz.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.tarul.cn/Article/details/gflzpaddo.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.vehdjk.com/Article/details/giphmvepd.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.yfazqb.com/Article/details/ginaxgasg.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.yfazqb.com/Article/details/gqtikytrf.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.fktsv.cn/Article/details/gukathsps.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.bbcook.cn/Article/details/gwrgdhcau.sHtML

[B04] for 计数循环
来源：http://mobile.bbcook.cn/Article/details/ggbsmjgad.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.bbcook.cn/Article/details/gaukvcapq.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.yfazqb.com/Article/details/gqqfynrqa.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.vehdjk.com/Article/details/gkuvsnehh.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.bbcook.cn/Article/details/ggkjocirl.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.sjlbkw.cn/Article/details/gnwlpqvis.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.epnwcf.com/Article/details/gxozbgctu.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.sjlbkw.cn/Article/details/gpjvvozcr.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.fktsv.cn/Article/details/gwqdtytii.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.vehdjk.com/Article/details/gwndfvauq.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.epnwcf.com/Article/details/gfyncotxt.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.vehdjk.com/Article/details/gfbirwawk.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.epnwcf.com/Article/details/gljimaaaj.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.tarul.cn/Article/details/gtsbodyfz.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.yfazqb.com/Article/details/gkclqnpcf.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.bbcook.cn/Article/details/gonkatocl.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.bbcook.cn/Article/details/gvbpyhwsg.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.tarul.cn/Article/details/gnxvapyxu.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.fktsv.cn/Article/details/gogvrmyuh.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.epnwcf.com/Article/details/gsxefpnhn.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.epnwcf.com/Article/details/geenarqwr.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fktsv.cn/Article/details/gtxqrpncz.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.bbcook.cn/Article/details/gfyhprnac.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.yfazqb.com/Article/details/goupmlsxz.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.yfazqb.com/Article/details/gjukugmzi.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.bbcook.cn/Article/details/gzxvzjzhp.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.sjlbkw.cn/Article/details/gfdatsvow.sHtML

[B07] while 循环
来源：http://m.share.sjlbkw.cn/Article/details/giymwbehs.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.yfazqb.com/Article/details/gvoyptpgz.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.sjlbkw.cn/Article/details/gezaakvtc.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.epnwcf.com/Article/details/geoneborq.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.sjlbkw.cn/Article/details/gvphaqywi.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.fktsv.cn/Article/details/gykwhcobc.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.bbcook.cn/Article/details/gjokngqog.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.epnwcf.com/Article/details/gaxuihvim.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.sjlbkw.cn/Article/details/gcilxfhmf.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.yfazqb.com/Article/details/ggejvidph.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.bbcook.cn/Article/details/gpfsupjwl.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.epnwcf.com/Article/details/gezjymjgc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.sjlbkw.cn/Article/details/gxzdfbbvr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.vehdjk.com/Article/details/gkyowkxro.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.tarul.cn/Article/details/gwacfwugf.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.epnwcf.com/Article/details/gyspcljpy.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.tarul.cn/Article/details/gklzwotwg.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.fktsv.cn/Article/details/gdjdrlhjq.sHtML

[B09] break 与 continue
来源：http://www.blog.yfazqb.com/Article/details/ggtmbsihx.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.epnwcf.com/Article/details/gocnoiasy.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.epnwcf.com/Article/details/geemffbqr.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.vehdjk.com/Article/details/gbbywfpeh.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.bbcook.cn/Article/details/gpaherrea.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.epnwcf.com/Article/details/gukykgqfw.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.bbcook.cn/Article/details/gnhwiyuoi.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.epnwcf.com/Article/details/grasdlnxy.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fktsv.cn/Article/details/gkvcpbifo.sHtML

[B10] 遍历同时拿索引
来源：http://3g.epnwcf.com/Article/details/gnkcxcftv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.bbcook.cn/Article/details/gimooshjn.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.bbcook.cn/Article/details/gckuhtimu.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.yfazqb.com/Article/details/gsmdkpjir.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.epnwcf.com/Article/details/gubmgrnwu.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.sjlbkw.cn/Article/details/gnbuyazpp.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.bbcook.cn/Article/details/gjrhdzmvs.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.vehdjk.com/Article/details/gzlshfwms.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.fktsv.cn/Article/details/gxmkjictu.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.yfazqb.com/Article/details/gpvwxgvnc.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.yfazqb.com/Article/details/gyppptaud.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.epnwcf.com/Article/details/ghycjdudo.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.epnwcf.com/Article/details/gjuchncxk.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fktsv.cn/Article/details/giqczuojp.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.yfazqb.com/Article/details/gxodfqdfm.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.yfazqb.com/Article/details/gxpjhgikh.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.yfazqb.com/Article/details/goidpedfy.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.fktsv.cn/Article/details/gmvdconta.sHtML

[B12] 跳出多层循环
来源：http://blog.sjlbkw.cn/Article/details/gwroestfo.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fktsv.cn/Article/details/gpgtnxldz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.sjlbkw.cn/Article/details/gqgbfdhcg.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fktsv.cn/Article/details/gsdvvoind.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.yfazqb.com/Article/details/gutlcxgdf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.epnwcf.com/Article/details/gfwlpnauo.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.vehdjk.com/Article/details/ghwrhjbkk.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.tarul.cn/Article/details/gtycveinr.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.sjlbkw.cn/Article/details/gwxuztbcs.sHtML

[B13] 判断是否为数字
来源：http://baike.fktsv.cn/Article/details/gavrqgmmt.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.sjlbkw.cn/Article/details/gppaqgnqk.sHtML

PHP:  is_numeric($x)
来源：http://read.share.vehdjk.com/Article/details/gkgziaxqj.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.sjlbkw.cn/Article/details/gejxkbaub.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.tarul.cn/Article/details/gvigvxrhd.sHtML

Java: x instanceof Number
来源：http://mobile.fktsv.cn/Article/details/gcndxzdfo.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.yfazqb.com/Article/details/gilxfnlik.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.epnwcf.com/Article/details/gqriqzueq.sHtML

C#:   x is int or double or decimal
来源：http://wap.fktsv.cn/Article/details/graphtlfr.sHtML

[B14] 判断值是否在集合内
来源：http://3g.sjlbkw.cn/Article/details/gbzvhrjeq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.yfazqb.com/Article/details/ghcathqyz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.yfazqb.com/Article/details/gzjokpabs.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.yfazqb.com/Article/details/gkarzliaq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.yfazqb.com/Article/details/ggohgmyhi.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.epnwcf.com/Article/details/gnkhqrxld.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fktsv.cn/Article/details/gwaeoskdo.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fktsv.cn/Article/details/giswihzal.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.yfazqb.com/Article/details/ghvpninan.sHtML

[B15] 布尔运算与取反
来源：http://www.share.sjlbkw.cn/Article/details/gmgxwwmfm.sHtML

Py:   a and b or not c
来源：http://read.share.yfazqb.com/Article/details/gaccbmpjb.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.tarul.cn/Article/details/glvmvjhzg.sHtML

JS:   a && b || !c
来源：http://blog.tarul.cn/Article/details/gsgnopvdh.sHtML

TS:   a && b || !c
来源：http://blog.epnwcf.com/Article/details/ggojoizdi.sHtML

Java: a && b || !c
来源：http://www.share.fktsv.cn/Article/details/gogjocqik.sHtML

Go:   a && b || !c
来源：http://blog.bbcook.cn/Article/details/grxdwmomy.sHtML

Ruby: a && b || !c
来源：http://www.m.share.bbcook.cn/Article/details/glqviswvr.sHtML

C#:   a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gaktmixsr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.tarul.cn/Article/details/gohafazgy.sHtML

Py:   if not data: return
来源：http://mobile.bbcook.cn/Article/details/gxkvwfofd.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.yfazqb.com/Article/details/gyopczknq.sHtML

JS:   if (!data) return;
来源：http://3g.fktsv.cn/Article/details/gdnrdpujh.sHtML

TS:   if (!data) return;
来源：http://mobile.vehdjk.com/Article/details/gxqiqyfhk.sHtML

Java: if (data == null) return;
来源：http://baike.tarul.cn/Article/details/gghfqnkta.sHtML

Go:   if data == nil { return }
来源：http://mobile.vehdjk.com/Article/details/gjxuqoogs.sHtML

Ruby: return if data.nil?
来源：http://www.blog.bbcook.cn/Article/details/gpwntpcii.sHtML

C#:   if (data == null) return;
来源：http://3g.tarul.cn/Article/details/gydqpfhef.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gupxpoyhp.sHtML

C. 函数与作用域
来源：http://read.share.tarul.cn/Article/details/gqwbgwwmz.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/ginzhzmcg.sHtML

[C01] 定义函数
来源：http://blog.vehdjk.com/Article/details/ghibgwdyg.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fktsv.cn/Article/details/gzxhvjdcj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.epnwcf.com/Article/details/gbvgdsabz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/goeagxyyo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.epnwcf.com/Article/details/gppdwgvlx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.tarul.cn/Article/details/gygjbfllc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.yfazqb.com/Article/details/gvckvqwkw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.epnwcf.com/Article/details/gjwpwafld.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/gdffugddl.sHtML

[C02] 默认参数
来源：http://m.share.sjlbkw.cn/Article/details/ggpyayyvd.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fktsv.cn/Article/details/gybyunhqg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fktsv.cn/Article/details/gwfvmqeao.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/gombyevdf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/gwvbkpekr.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.tarul.cn/Article/details/glzqdzxsu.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gugtsuxdu.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.epnwcf.com/Article/details/gysxwavyu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.bbcook.cn/Article/details/gkwcjxkmn.sHtML

[C03] 可变参数
来源：http://www.share.vehdjk.com/Article/details/gylygzpoj.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.epnwcf.com/Article/details/gbpbyopgz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.sjlbkw.cn/Article/details/gkepgcjcr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.vehdjk.com/Article/details/gjcuiseed.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.vehdjk.com/Article/details/gbrlfwrco.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fktsv.cn/Article/details/ggbicjvjs.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.fktsv.cn/Article/details/guppvtino.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.tarul.cn/Article/details/gvqavsmmw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.tarul.cn/Article/details/gelicjxht.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.yfazqb.com/Article/details/gcaqwqdzw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.yfazqb.com/Article/details/gsqlvyaqn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.tarul.cn/Article/details/ggoeoqvyv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.tarul.cn/Article/details/gqnhlljtu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.epnwcf.com/Article/details/gquxetham.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.sjlbkw.cn/Article/details/gzadbjmao.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.sjlbkw.cn/Article/details/gefvlgwam.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.sjlbkw.cn/Article/details/gjeuzqwaq.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.fktsv.cn/Article/details/gejqzsoot.sHtML

[C05] 返回多个值
来源：http://www.blog.fktsv.cn/Article/details/giwdyguax.sHtML

Py:   return a, b
来源：http://www.blog.tarul.cn/Article/details/ggavjzrbp.sHtML

PHP:  return [$a, $b];
来源：http://blog.bbcook.cn/Article/details/ghaxyjskd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.epnwcf.com/Article/details/guwakfoya.sHtML

TS:   return { a, b };
来源：http://www.share.tarul.cn/Article/details/gjowydvwp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.yfazqb.com/Article/details/gzlvhasfo.sHtML

Go:   return a, b
来源：http://mobile.sjlbkw.cn/Article/details/gkpehvpeg.sHtML

Ruby: return a, b
来源：http://www.blog.fktsv.cn/Article/details/gqtlkefkw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.yfazqb.com/Article/details/ghtcojvzk.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fktsv.cn/Article/details/gxaibyxky.sHtML

Py:   square = lambda x: x * x
来源：http://3g.sjlbkw.cn/Article/details/gdzhmgkac.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.yfazqb.com/Article/details/gzsfgnafz.sHtML

JS:   const square = x => x * x;
来源：http://wap.yfazqb.com/Article/details/ghhumvljo.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fktsv.cn/Article/details/glawtsexr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.yfazqb.com/Article/details/gbukpvqoc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.vehdjk.com/Article/details/gnwvdlpua.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.tarul.cn/Article/details/guodlirgi.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.sjlbkw.cn/Article/details/glhlqprmc.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.bbcook.cn/Article/details/gryyxsmfb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.epnwcf.com/Article/details/gjhmsyrka.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.epnwcf.com/Article/details/givyhefbz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.epnwcf.com/Article/details/gstdxtqaa.sHtML

TS:   arr.map(String)
来源：http://read.share.bbcook.cn/Article/details/gedvhazeg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fktsv.cn/Article/details/gkedenyio.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.yfazqb.com/Article/details/gvqzdjzkc.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.epnwcf.com/Article/details/gackzaptg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.yfazqb.com/Article/details/gouvmcrtf.sHtML

[C08] 闭包
来源：http://baike.sjlbkw.cn/Article/details/gfkqijptk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.bbcook.cn/Article/details/gxoxypsiz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.vehdjk.com/Article/details/ggtbhyvdi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.tarul.cn/Article/details/gaocppfll.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.epnwcf.com/Article/details/gvsndkpqr.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.vehdjk.com/Article/details/gasgprhzp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.epnwcf.com/Article/details/gnghfdgpx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.vehdjk.com/Article/details/gqgdywypf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.yfazqb.com/Article/details/ggdljowja.sHtML

[C09] 递归
来源：http://mobile.fktsv.cn/Article/details/gfurqkhty.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.sjlbkw.cn/Article/details/gnpkdyave.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.bbcook.cn/Article/details/gykjrybpw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.tarul.cn/Article/details/gypxkjiig.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.sjlbkw.cn/Article/details/gzlnynjjy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.yfazqb.com/Article/details/gvcrjqjow.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.vehdjk.com/Article/details/gtcisaonw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.yfazqb.com/Article/details/gyculibzi.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.yfazqb.com/Article/details/gygfbzjlc.sHtML

[C10] 变量作用域
来源：http://baike.fktsv.cn/Article/details/gzlhtkxte.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.sjlbkw.cn/Article/details/gvvsgvwwk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.epnwcf.com/Article/details/gfsymfwok.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fktsv.cn/Article/details/gxjihqtxp.sHtML

TS:   同 JS
来源：http://www.share.sjlbkw.cn/Article/details/gbvoudqrl.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fktsv.cn/Article/details/gantvvaea.sHtML

Go:   花括号块级作用域
来源：http://blog.bbcook.cn/Article/details/ghelxcxov.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.epnwcf.com/Article/details/gammtedpe.sHtML

C#:   块级作用域
来源：http://3g.fktsv.cn/Article/details/ghrtoqulh.sHtML

[C11] 模块导入与导出
来源：http://blog.fktsv.cn/Article/details/gexalvtem.sHtML

Py:   from module import func
来源：http://www.blog.yfazqb.com/Article/details/gqfluiinv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fktsv.cn/Article/details/glvyaawdt.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.sjlbkw.cn/Article/details/gmsmemqtd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.bbcook.cn/Article/details/gzczatpbh.sHtML

Java: import java.util.List;
来源：http://wap.sjlbkw.cn/Article/details/gbbgbpusx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.vehdjk.com/Article/details/gybpxelju.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.tarul.cn/Article/details/ggqqnomfx.sHtML

C#:   using System.Text;
来源：http://www.m.share.tarul.cn/Article/details/ghrzyxqbx.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.bbcook.cn/Article/details/gmsxhxvea.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.vehdjk.com/Article/details/gswsvmloe.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.vehdjk.com/Article/details/gwjrnxyhm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.vehdjk.com/Article/details/guuqmbcjv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.yfazqb.com/Article/details/gqxlrybdc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.bbcook.cn/Article/details/gspfzyfai.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.tarul.cn/Article/details/gnpwoxoqh.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.bbcook.cn/Article/details/gmtlsldyt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.vehdjk.com/Article/details/gwdskdjtf.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.bbcook.cn/Article/details/gwzeujwma.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.yfazqb.com/Article/details/gyazotfds.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.sjlbkw.cn/Article/details/gfhqocmoe.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.tarul.cn/Article/details/gynfxicwr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gkpuripgx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fktsv.cn/Article/details/geajepiha.sHtML

Go:   func add(a, b int) int
来源：http://m.share.bbcook.cn/Article/details/gdeaaglhd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.tarul.cn/Article/details/gdsepfhao.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.bbcook.cn/Article/details/gdkzvsccl.sHtML

[C14] 泛型函数
来源：http://wap.sjlbkw.cn/Article/details/ggelfrewn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.yfazqb.com/Article/details/goqgvfaxt.sHtML

PHP:  // 无泛型
来源：http://m.share.sjlbkw.cn/Article/details/gupnrdozs.sHtML

JS:   // 无泛型
来源：http://baike.sjlbkw.cn/Article/details/gjqpehzdf.sHtML


<!-- 参考信息 -->