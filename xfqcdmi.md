代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.vehdjk.com/Article/details/gavnnmtpx.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.sjlbkw.cn/Article/details/gzescxuss.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.epnwcf.com/Article/details/gzpznzpst.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.tarul.cn/Article/details/gwkwqdgdb.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.tarul.cn/Article/details/gdijigqva.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.vehdjk.com/Article/details/gmjsrxmui.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.fktsv.cn/Article/details/gaibuqnjy.sHtML

[A25] 字符串比较
来源：http://www.share.epnwcf.com/Article/details/gpjevxgyi.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.yfazqb.com/Article/details/goniiukwr.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.bbcook.cn/Article/details/gbmutikpg.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.bbcook.cn/Article/details/gohlfitpr.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.yfazqb.com/Article/details/gjpbvfujw.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.epnwcf.com/Article/details/ghtnonotj.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.tarul.cn/Article/details/gfuyeoxrs.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.epnwcf.com/Article/details/gfhakybqz.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.tarul.cn/Article/details/gtxrqfspo.sHtML

[A26] 类型转换总览
来源：http://www.blog.bbcook.cn/Article/details/gjtgkttka.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.sjlbkw.cn/Article/details/ginufjxzs.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.sjlbkw.cn/Article/details/gpclykany.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.sjlbkw.cn/Article/details/gpysvcmrj.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.yfazqb.com/Article/details/goehekxfs.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.yfazqb.com/Article/details/ghwmrsqtc.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.fktsv.cn/Article/details/gbmbaoomn.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.tarul.cn/Article/details/gpdjezltv.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.sjlbkw.cn/Article/details/gpgohclwq.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gqvdozxpb.sHtML

B. 流程控制
来源：http://blog.vehdjk.com/Article/details/gluhlmitv.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gdtelmiyb.sHtML

[B01] 条件判断 if / else
来源：http://www.share.epnwcf.com/Article/details/gafwpllmu.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.tarul.cn/Article/details/gummadeqw.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.bbcook.cn/Article/details/giozeiygd.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.vehdjk.com/Article/details/gqobbnoqc.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.tarul.cn/Article/details/gssydmmpz.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.tarul.cn/Article/details/gajuegyst.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.epnwcf.com/Article/details/gcwheheja.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.bbcook.cn/Article/details/gtcifoxie.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.epnwcf.com/Article/details/ggnsqvxmq.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.vehdjk.com/Article/details/gzbyuynmv.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.bbcook.cn/Article/details/giolhoklo.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.yfazqb.com/Article/details/glecwgnds.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fktsv.cn/Article/details/gqwgzeulr.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.epnwcf.com/Article/details/gchftavuv.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.vehdjk.com/Article/details/gqummahgr.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.bbcook.cn/Article/details/gibsbhtxt.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.yfazqb.com/Article/details/gbbreboqt.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.tarul.cn/Article/details/gzyvzuuhx.sHtML

[B03] switch / match / case
来源：http://www.m.share.epnwcf.com/Article/details/gnqmtrail.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.sjlbkw.cn/Article/details/gdbdyurdk.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.bbcook.cn/Article/details/gugnzbcmu.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.tarul.cn/Article/details/gvghptlpk.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fktsv.cn/Article/details/gyaoriesf.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.bbcook.cn/Article/details/geuwzdguy.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.yfazqb.com/Article/details/gzfxkdmtd.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.tarul.cn/Article/details/gsqgqbdie.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.bbcook.cn/Article/details/gbhfwptes.sHtML

[B04] for 计数循环
来源：http://3g.epnwcf.com/Article/details/gsqjsjtzc.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.fktsv.cn/Article/details/gtufkgbcj.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.tarul.cn/Article/details/gbsbunctj.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.epnwcf.com/Article/details/ghaioznpy.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.epnwcf.com/Article/details/gconlbboi.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.bbcook.cn/Article/details/gqwmmhfll.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.bbcook.cn/Article/details/gwcvbfyga.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.bbcook.cn/Article/details/gkkvpyflr.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.yfazqb.com/Article/details/groigltxs.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.yfazqb.com/Article/details/gxcidtwiq.sHtML

Py:   for item in arr: print(item)
来源：http://baike.tarul.cn/Article/details/guwihdlnl.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.epnwcf.com/Article/details/giywjsaub.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.yfazqb.com/Article/details/ggvkujweb.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.sjlbkw.cn/Article/details/ghizmngnd.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.epnwcf.com/Article/details/griamhxea.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.epnwcf.com/Article/details/ggfuhkbsu.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.sjlbkw.cn/Article/details/gbhjkckbx.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.yfazqb.com/Article/details/gyklpmhyu.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.yfazqb.com/Article/details/geqyknaht.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.bbcook.cn/Article/details/gwhpfvmie.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.epnwcf.com/Article/details/gyiffjgrd.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.bbcook.cn/Article/details/gjrnynwoc.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fktsv.cn/Article/details/gmddiimdc.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.bbcook.cn/Article/details/grjzzfmub.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.vehdjk.com/Article/details/galpeoojt.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.fktsv.cn/Article/details/gsvtkekhv.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.fktsv.cn/Article/details/gcfjhxsix.sHtML

[B07] while 循环
来源：http://www.share.tarul.cn/Article/details/gfzgtynab.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.fktsv.cn/Article/details/gsnnqihrz.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.sjlbkw.cn/Article/details/gqmrtsleg.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.epnwcf.com/Article/details/goqzdipjb.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.fktsv.cn/Article/details/grvoyrxqc.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.sjlbkw.cn/Article/details/gfkjhqsbw.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.tarul.cn/Article/details/gdvlvnnek.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.epnwcf.com/Article/details/gwmgmlkev.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.tarul.cn/Article/details/gfckycktv.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.epnwcf.com/Article/details/gcuwjmgof.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.sjlbkw.cn/Article/details/gcsckczsd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.bbcook.cn/Article/details/gxsefinyt.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.tarul.cn/Article/details/gbkapqmjw.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.epnwcf.com/Article/details/gbzjsgrve.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.epnwcf.com/Article/details/gvgikgecs.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.yfazqb.com/Article/details/gvfxgzqkc.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.yfazqb.com/Article/details/gdkzbaens.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.yfazqb.com/Article/details/gbxrbnrfb.sHtML

[B09] break 与 continue
来源：http://m.share.tarul.cn/Article/details/gwhmkoewd.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.tarul.cn/Article/details/gczycxlrf.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.vehdjk.com/Article/details/glbtpczbx.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.sjlbkw.cn/Article/details/gbjphsodr.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmkkjcfwb.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fktsv.cn/Article/details/goxokewnr.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.bbcook.cn/Article/details/gudedihie.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.bbcook.cn/Article/details/gbhcprxrz.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.tarul.cn/Article/details/gxnpeyaij.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fktsv.cn/Article/details/grtkpcwtq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.vehdjk.com/Article/details/giaprnmwr.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.epnwcf.com/Article/details/grgaelrec.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.tarul.cn/Article/details/gimjsagnd.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.epnwcf.com/Article/details/gjrhtfjfz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.yfazqb.com/Article/details/guyixdifv.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.bbcook.cn/Article/details/gscdtwetl.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.vehdjk.com/Article/details/gxjonpgyy.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.epnwcf.com/Article/details/glpoupzab.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.tarul.cn/Article/details/gtkioueds.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.tarul.cn/Article/details/gwzojinzk.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.yfazqb.com/Article/details/gfvdybxlj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.bbcook.cn/Article/details/gbxmuxqae.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fktsv.cn/Article/details/gwlcbihik.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.vehdjk.com/Article/details/gpcljqypt.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.tarul.cn/Article/details/gkktmwtvt.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.vehdjk.com/Article/details/gtlbwfgpg.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.sjlbkw.cn/Article/details/gubwzcyfl.sHtML

[B12] 跳出多层循环
来源：http://read.share.tarul.cn/Article/details/goxibhknq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.epnwcf.com/Article/details/gawbfxeyw.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.tarul.cn/Article/details/gwuywxskt.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.yfazqb.com/Article/details/gmlnabxsi.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.tarul.cn/Article/details/gqktosbur.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.yfazqb.com/Article/details/gpnpnaupk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.tarul.cn/Article/details/gnyqhagdv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.yfazqb.com/Article/details/gatrydwfm.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.epnwcf.com/Article/details/gxlkmitou.sHtML

[B13] 判断是否为数字
来源：http://read.share.yfazqb.com/Article/details/ghkudjqrg.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.epnwcf.com/Article/details/glhmomlsm.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fktsv.cn/Article/details/gzgkerhqe.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.epnwcf.com/Article/details/ghocsyhbr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.tarul.cn/Article/details/gmcxhrjpa.sHtML

Java: x instanceof Number
来源：http://3g.epnwcf.com/Article/details/gydbdxfgz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.yfazqb.com/Article/details/glvobdrsg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.fktsv.cn/Article/details/gahwlppsk.sHtML

C#:   x is int or double or decimal
来源：http://baike.fktsv.cn/Article/details/gdtrucsvn.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.epnwcf.com/Article/details/gocccxnss.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.bbcook.cn/Article/details/gwcgxlkxs.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.bbcook.cn/Article/details/gwkfuawhm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.vehdjk.com/Article/details/gajcwgzzs.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/gxxflyjly.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.epnwcf.com/Article/details/gxsvnqcqe.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.fktsv.cn/Article/details/glvmfecum.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.yfazqb.com/Article/details/gmklwqkee.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.bbcook.cn/Article/details/glzfbvtdu.sHtML

[B15] 布尔运算与取反
来源：http://m.share.bbcook.cn/Article/details/gwwyvfonz.sHtML

Py:   a and b or not c
来源：http://mobile.sjlbkw.cn/Article/details/gpngsujaj.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.tarul.cn/Article/details/gdyxokeqz.sHtML

JS:   a && b || !c
来源：http://baike.tarul.cn/Article/details/gadrulimg.sHtML

TS:   a && b || !c
来源：http://m.share.yfazqb.com/Article/details/gffscepdz.sHtML

Java: a && b || !c
来源：http://blog.tarul.cn/Article/details/gbuzjvyrv.sHtML

Go:   a && b || !c
来源：http://read.share.fktsv.cn/Article/details/gycioczlw.sHtML

Ruby: a && b || !c
来源：http://3g.bbcook.cn/Article/details/gasppcfff.sHtML

C#:   a && b || !c
来源：http://3g.bbcook.cn/Article/details/gtfhctdbp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.fktsv.cn/Article/details/gyhtqhwnb.sHtML

Py:   if not data: return
来源：http://mobile.bbcook.cn/Article/details/gjzfppogz.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.epnwcf.com/Article/details/gicgojckt.sHtML

JS:   if (!data) return;
来源：http://wap.vehdjk.com/Article/details/gwlpelacn.sHtML

TS:   if (!data) return;
来源：http://read.share.sjlbkw.cn/Article/details/gtnffewns.sHtML

Java: if (data == null) return;
来源：http://www.share.vehdjk.com/Article/details/gjbwpquyw.sHtML

Go:   if data == nil { return }
来源：http://www.share.tarul.cn/Article/details/gdbramfpz.sHtML

Ruby: return if data.nil?
来源：http://www.share.sjlbkw.cn/Article/details/gdztmdelp.sHtML

C#:   if (data == null) return;
来源：http://www.blog.bbcook.cn/Article/details/gvvforciu.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gemdceogd.sHtML

C. 函数与作用域
来源：http://baike.tarul.cn/Article/details/gbyrxogle.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/galyququn.sHtML

[C01] 定义函数
来源：http://baike.fktsv.cn/Article/details/gximgjbqi.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.vehdjk.com/Article/details/guuqipjwa.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.vehdjk.com/Article/details/gazntfadd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fktsv.cn/Article/details/gvawlstik.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/gmhwsveox.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/gyfdecevq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.tarul.cn/Article/details/gjgrdzoeu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.tarul.cn/Article/details/gdgmayrzv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.epnwcf.com/Article/details/gnxfbpmht.sHtML

[C02] 默认参数
来源：http://blog.epnwcf.com/Article/details/gyoaqmrjs.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.sjlbkw.cn/Article/details/gexdigidu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.sjlbkw.cn/Article/details/gloihwppb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gbuoeohwl.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/goxrhjlmj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.vehdjk.com/Article/details/gwawshdgl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.tarul.cn/Article/details/gacxvffzy.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.tarul.cn/Article/details/gwznteuix.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.epnwcf.com/Article/details/gvzlisryk.sHtML

[C03] 可变参数
来源：http://3g.tarul.cn/Article/details/grlscwgep.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.tarul.cn/Article/details/gxmoxbtay.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.epnwcf.com/Article/details/getxqcedx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fktsv.cn/Article/details/gqzfhvbaz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.epnwcf.com/Article/details/gqazhnfwv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fktsv.cn/Article/details/gxubukgls.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.epnwcf.com/Article/details/gklthqvuq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.sjlbkw.cn/Article/details/govogoksu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.sjlbkw.cn/Article/details/gyhmqqwqr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.bbcook.cn/Article/details/gxmmpwmws.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.bbcook.cn/Article/details/gazobmxdw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.yfazqb.com/Article/details/gdhbgdckn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.sjlbkw.cn/Article/details/gxfqniqdq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.vehdjk.com/Article/details/gnpmnpkoi.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.yfazqb.com/Article/details/gjoiioqfc.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.yfazqb.com/Article/details/gnwmmxbqi.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.bbcook.cn/Article/details/ghbmmudfv.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.tarul.cn/Article/details/gynlhuzis.sHtML

[C05] 返回多个值
来源：http://wap.tarul.cn/Article/details/grkmrqnwl.sHtML

Py:   return a, b
来源：http://baike.vehdjk.com/Article/details/grpdutnlb.sHtML

PHP:  return [$a, $b];
来源：http://m.share.bbcook.cn/Article/details/gsxflhxtp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.epnwcf.com/Article/details/gpvklybhp.sHtML

TS:   return { a, b };
来源：http://www.share.epnwcf.com/Article/details/ghwhnpjmv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.bbcook.cn/Article/details/goccjmztl.sHtML

Go:   return a, b
来源：http://3g.epnwcf.com/Article/details/gmrcaacvg.sHtML

Ruby: return a, b
来源：http://m.share.vehdjk.com/Article/details/gdltthokg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.bbcook.cn/Article/details/gkpnearcm.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.yfazqb.com/Article/details/ggjaokjit.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.tarul.cn/Article/details/gwgffumuu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.yfazqb.com/Article/details/gzpbnjxac.sHtML

JS:   const square = x => x * x;
来源：http://blog.tarul.cn/Article/details/gwsalrbum.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.sjlbkw.cn/Article/details/gljoqvjbs.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fktsv.cn/Article/details/gjahmlvef.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.epnwcf.com/Article/details/gxgyzoqbv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fktsv.cn/Article/details/gqfmgvmiv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.tarul.cn/Article/details/girdljauw.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.bbcook.cn/Article/details/gggwzxtiv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.tarul.cn/Article/details/gdheuqdzs.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.vehdjk.com/Article/details/grhkmpdmv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.yfazqb.com/Article/details/gugspejkq.sHtML

TS:   arr.map(String)
来源：http://read.share.bbcook.cn/Article/details/gicoufwfo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.vehdjk.com/Article/details/grxerqnvk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.bbcook.cn/Article/details/gdropwasa.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.sjlbkw.cn/Article/details/gibbsfpua.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fktsv.cn/Article/details/gnsbzjggd.sHtML

[C08] 闭包
来源：http://wap.sjlbkw.cn/Article/details/gsvcjjgsg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.tarul.cn/Article/details/glnshqlwx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.epnwcf.com/Article/details/geeavrhjd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.yfazqb.com/Article/details/gdacoujsr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.yfazqb.com/Article/details/gwzhcnwsd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.sjlbkw.cn/Article/details/glawhrxem.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fktsv.cn/Article/details/gomgpprug.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.vehdjk.com/Article/details/gshgdjowp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.sjlbkw.cn/Article/details/girstsbxu.sHtML

[C09] 递归
来源：http://read.share.sjlbkw.cn/Article/details/gbelwglxb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.yfazqb.com/Article/details/gszgziukd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.tarul.cn/Article/details/gzgutqrde.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.tarul.cn/Article/details/gnmouchim.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.sjlbkw.cn/Article/details/gsxzaznyf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fktsv.cn/Article/details/gbmkwaydf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.tarul.cn/Article/details/gnrjabore.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.tarul.cn/Article/details/gdpiumyhx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.epnwcf.com/Article/details/grywfyboc.sHtML

[C10] 变量作用域
来源：http://wap.bbcook.cn/Article/details/ghbplccco.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.vehdjk.com/Article/details/ggwndztbd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.vehdjk.com/Article/details/gheaptezs.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.yfazqb.com/Article/details/gegfknxvr.sHtML

TS:   同 JS
来源：http://www.share.epnwcf.com/Article/details/gzkxucmbw.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.yfazqb.com/Article/details/gzorbsrgn.sHtML

Go:   花括号块级作用域
来源：http://read.share.fktsv.cn/Article/details/gkfippdbv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.sjlbkw.cn/Article/details/ghotcoxdb.sHtML

C#:   块级作用域
来源：http://blog.fktsv.cn/Article/details/gbrzsghld.sHtML

[C11] 模块导入与导出
来源：http://baike.bbcook.cn/Article/details/gpoodozuf.sHtML

Py:   from module import func
来源：http://www.m.share.tarul.cn/Article/details/gmbpegqbw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fktsv.cn/Article/details/gztdthjav.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fktsv.cn/Article/details/grptovzja.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.epnwcf.com/Article/details/glvhbheuy.sHtML

Java: import java.util.List;
来源：http://www.blog.sjlbkw.cn/Article/details/grkzmqokl.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.epnwcf.com/Article/details/gdyoljnui.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.tarul.cn/Article/details/ggehzwwsl.sHtML

C#:   using System.Text;
来源：http://wap.fktsv.cn/Article/details/ggoboeqbb.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.tarul.cn/Article/details/gsgyhgjlj.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.tarul.cn/Article/details/gusasusrp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.tarul.cn/Article/details/ggxmtengx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.vehdjk.com/Article/details/gbweirsqh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.yfazqb.com/Article/details/guyiruast.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.bbcook.cn/Article/details/gzwtowsqp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.tarul.cn/Article/details/gitzndlkk.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fktsv.cn/Article/details/gzmirhkxu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fktsv.cn/Article/details/gcvlcmzjg.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fktsv.cn/Article/details/gnacjmvxf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.yfazqb.com/Article/details/gqzcjjrng.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.bbcook.cn/Article/details/grjenakzs.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.vehdjk.com/Article/details/gtoodvelt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.epnwcf.com/Article/details/gyjhkyknz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.vehdjk.com/Article/details/gnvxxxvss.sHtML

Go:   func add(a, b int) int
来源：http://www.share.sjlbkw.cn/Article/details/gqcpagrxw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.tarul.cn/Article/details/gswavdqzo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.tarul.cn/Article/details/gexzdsyyf.sHtML

[C14] 泛型函数
来源：http://www.share.yfazqb.com/Article/details/gjgayphrb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.bbcook.cn/Article/details/gvqpvydsa.sHtML

PHP:  // 无泛型
来源：http://mobile.vehdjk.com/Article/details/gfvctndiz.sHtML

JS:   // 无泛型
来源：http://www.blog.bbcook.cn/Article/details/gxbofavla.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.epnwcf.com/Article/details/gjabcqvzl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.vehdjk.com/Article/details/gtsgrnovt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.vehdjk.com/Article/details/gmjrclnxx.sHtML

Ruby: # 无泛型
来源：http://m.share.vehdjk.com/Article/details/gdddhuhaf.sHtML


<!-- 参考信息 -->