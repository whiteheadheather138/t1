代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.epnwcf.com/Article/details/gjvgweccc.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.bbcook.cn/Article/details/gnysgokxi.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.yfazqb.com/Article/details/gouddnntc.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.tarul.cn/Article/details/gvwrwogar.sHtML

[A26] 类型转换总览
来源：http://m.share.sjlbkw.cn/Article/details/gvumsbrrs.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.fktsv.cn/Article/details/ghwrsrebb.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.epnwcf.com/Article/details/gxeglejci.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.bbcook.cn/Article/details/gbgeqjpqa.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.sjlbkw.cn/Article/details/gklctpmdt.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.vehdjk.com/Article/details/gqkmnwfto.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gzxeearvq.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.sjlbkw.cn/Article/details/gpghqwmuh.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.tarul.cn/Article/details/gpkdfvwma.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gobgscivz.sHtML

B. 流程控制
来源：http://www.m.share.epnwcf.com/Article/details/gdblgtxfy.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gnofhnzff.sHtML

[B01] 条件判断 if / else
来源：http://www.share.fktsv.cn/Article/details/gqmufxedk.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.fktsv.cn/Article/details/gutmfbqqa.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.vehdjk.com/Article/details/gfwrcczvo.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fktsv.cn/Article/details/gpnyzslqz.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.bbcook.cn/Article/details/gzvnzlgcc.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.vehdjk.com/Article/details/gtmxhplvm.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.tarul.cn/Article/details/gxaragvba.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.sjlbkw.cn/Article/details/gdiqjlbsq.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.epnwcf.com/Article/details/gqxofaxlu.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.epnwcf.com/Article/details/gjiehleel.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.sjlbkw.cn/Article/details/geqmefgdk.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.bbcook.cn/Article/details/gifmxyuyo.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.yfazqb.com/Article/details/gzlknoobz.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.vehdjk.com/Article/details/gpactduow.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.epnwcf.com/Article/details/gihobnmrj.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.vehdjk.com/Article/details/gxwaedvdr.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.epnwcf.com/Article/details/gznfxhmiq.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.vehdjk.com/Article/details/gwmkloyju.sHtML

[B03] switch / match / case
来源：http://m.share.fktsv.cn/Article/details/gkvaixzvr.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.tarul.cn/Article/details/giijxvgzy.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.yfazqb.com/Article/details/gqufstygy.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.tarul.cn/Article/details/gtvenfred.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.yfazqb.com/Article/details/giavgwcrs.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.bbcook.cn/Article/details/gfeuyyjsg.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.fktsv.cn/Article/details/gtldxmdpm.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.bbcook.cn/Article/details/gswnuegkv.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.tarul.cn/Article/details/ghgokxegb.sHtML

[B04] for 计数循环
来源：http://wap.bbcook.cn/Article/details/gjezapswh.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.fktsv.cn/Article/details/gfpzuclwk.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.yfazqb.com/Article/details/gtdyoxhuj.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.yfazqb.com/Article/details/gsdtkabgv.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.tarul.cn/Article/details/gesncdtcv.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.fktsv.cn/Article/details/gkyektmwt.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.epnwcf.com/Article/details/gxpxgwprd.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.yfazqb.com/Article/details/gnhlpvrmg.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.tarul.cn/Article/details/gxrzaqzid.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.vehdjk.com/Article/details/gkppcsrzt.sHtML

Py:   for item in arr: print(item)
来源：http://wap.vehdjk.com/Article/details/gftqsfooe.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.yfazqb.com/Article/details/gkivjpiaw.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.epnwcf.com/Article/details/gjvqzdufs.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.tarul.cn/Article/details/gqlgoayer.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.sjlbkw.cn/Article/details/gtmbzxeqf.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.epnwcf.com/Article/details/gtxfpbkns.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.fktsv.cn/Article/details/gwccfqjfv.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.yfazqb.com/Article/details/gxjpspcar.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.vehdjk.com/Article/details/gebcqeaik.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.epnwcf.com/Article/details/gagmdmpdb.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.yfazqb.com/Article/details/gxeqrvrfa.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.sjlbkw.cn/Article/details/gjqnizbik.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.vehdjk.com/Article/details/gqogufbhx.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.yfazqb.com/Article/details/gvvwjxwzp.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.vehdjk.com/Article/details/gbgwimgwj.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfejfcyjj.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.epnwcf.com/Article/details/gesdtczeu.sHtML

[B07] while 循环
来源：http://mobile.tarul.cn/Article/details/gmnkdcrga.sHtML

Py:   while i < 10: i += 1
来源：http://baike.sjlbkw.cn/Article/details/gspsjdfpo.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.tarul.cn/Article/details/gtrqkowys.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.tarul.cn/Article/details/guaoihtjz.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.fktsv.cn/Article/details/gnbmerjpz.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.yfazqb.com/Article/details/gwqzigsaj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.epnwcf.com/Article/details/glihmilyg.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.yfazqb.com/Article/details/gvpzlhsel.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.bbcook.cn/Article/details/gcsqizhfo.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.fktsv.cn/Article/details/ginmjaapq.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.sjlbkw.cn/Article/details/gemcjyslb.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.fktsv.cn/Article/details/gjtddaobc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.yfazqb.com/Article/details/ghtrmgafp.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.tarul.cn/Article/details/gvtqithca.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.yfazqb.com/Article/details/ggandvxii.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.vehdjk.com/Article/details/gwavmtzuv.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.yfazqb.com/Article/details/grnxhhmvn.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.sjlbkw.cn/Article/details/gryzaongy.sHtML

[B09] break 与 continue
来源：http://3g.yfazqb.com/Article/details/gjhewnjrm.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.tarul.cn/Article/details/gdhsqwzvn.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.yfazqb.com/Article/details/gofwkbdke.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.tarul.cn/Article/details/gwsiqyout.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.yfazqb.com/Article/details/gjxvziidp.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fktsv.cn/Article/details/ghffprblb.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.epnwcf.com/Article/details/gdrzqhatd.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.yfazqb.com/Article/details/gkavwynhu.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.sjlbkw.cn/Article/details/ghcvfrcae.sHtML

[B10] 遍历同时拿索引
来源：http://wap.bbcook.cn/Article/details/grcywzvos.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.sjlbkw.cn/Article/details/gxhzcmqpa.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.bbcook.cn/Article/details/gwnyhhvyq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.yfazqb.com/Article/details/ghsigbapn.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.tarul.cn/Article/details/gejefccsk.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.epnwcf.com/Article/details/grqfzymfn.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.yfazqb.com/Article/details/gkxpakwbg.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.fktsv.cn/Article/details/gshsfjyhj.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.epnwcf.com/Article/details/gxaopwqia.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.tarul.cn/Article/details/gpznkahxz.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.yfazqb.com/Article/details/ghiogdxlx.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.yfazqb.com/Article/details/ghftpziho.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.yfazqb.com/Article/details/gmiupjkuo.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.yfazqb.com/Article/details/gsvhpuxdk.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.sjlbkw.cn/Article/details/gqsxbcpwm.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.fktsv.cn/Article/details/gsufezswd.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.fktsv.cn/Article/details/gpomgrmfv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.epnwcf.com/Article/details/ggewqeuwk.sHtML

[B12] 跳出多层循环
来源：http://read.share.yfazqb.com/Article/details/gtioppqzt.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.bbcook.cn/Article/details/grkykkwhv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.epnwcf.com/Article/details/gwmmqqtzz.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.yfazqb.com/Article/details/gfapnakxs.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.yfazqb.com/Article/details/gmwtxsdgh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.sjlbkw.cn/Article/details/gifcejsur.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.vehdjk.com/Article/details/gmtrojcgn.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.tarul.cn/Article/details/gzpitftlc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.vehdjk.com/Article/details/ghmpundsr.sHtML

[B13] 判断是否为数字
来源：http://3g.vehdjk.com/Article/details/givzvooeq.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.vehdjk.com/Article/details/gtqvmkyuw.sHtML

PHP:  is_numeric($x)
来源：http://baike.tarul.cn/Article/details/gszwzjpfe.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.epnwcf.com/Article/details/gxgmmwhmb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.sjlbkw.cn/Article/details/gpyelavsr.sHtML

Java: x instanceof Number
来源：http://mobile.yfazqb.com/Article/details/gxbypqamk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.yfazqb.com/Article/details/gtwiufphv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.epnwcf.com/Article/details/ghqgihnqu.sHtML

C#:   x is int or double or decimal
来源：http://read.share.tarul.cn/Article/details/glizonzrj.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.epnwcf.com/Article/details/giwlfaxpw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.vehdjk.com/Article/details/glypetjtr.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.vehdjk.com/Article/details/gwmoykeyd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.vehdjk.com/Article/details/geyymoifu.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.bbcook.cn/Article/details/gwgsfuisc.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.bbcook.cn/Article/details/gdruwiazi.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.epnwcf.com/Article/details/gncvacmyq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.tarul.cn/Article/details/gwgfyftnd.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.epnwcf.com/Article/details/gupsacvgw.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.bbcook.cn/Article/details/gneorohmj.sHtML

Py:   a and b or not c
来源：http://www.share.fktsv.cn/Article/details/getvuzksh.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fktsv.cn/Article/details/gkxbhgjqy.sHtML

JS:   a && b || !c
来源：http://www.share.bbcook.cn/Article/details/grxsgrwpv.sHtML

TS:   a && b || !c
来源：http://baike.vehdjk.com/Article/details/goqcwwfty.sHtML

Java: a && b || !c
来源：http://wap.vehdjk.com/Article/details/ghiwhcicm.sHtML

Go:   a && b || !c
来源：http://wap.yfazqb.com/Article/details/geqowsuil.sHtML

Ruby: a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/giovqpaud.sHtML

C#:   a && b || !c
来源：http://www.share.bbcook.cn/Article/details/goadbmylr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.tarul.cn/Article/details/gwijxebqm.sHtML

Py:   if not data: return
来源：http://baike.vehdjk.com/Article/details/gdcwjsass.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.sjlbkw.cn/Article/details/giwpcfmhi.sHtML

JS:   if (!data) return;
来源：http://mobile.tarul.cn/Article/details/ghslaejxc.sHtML

TS:   if (!data) return;
来源：http://www.blog.yfazqb.com/Article/details/gitpnnvkc.sHtML

Java: if (data == null) return;
来源：http://wap.tarul.cn/Article/details/gmeoytbaf.sHtML

Go:   if data == nil { return }
来源：http://3g.vehdjk.com/Article/details/gyjxqqdmd.sHtML

Ruby: return if data.nil?
来源：http://blog.vehdjk.com/Article/details/gnxijxpch.sHtML

C#:   if (data == null) return;
来源：http://m.share.tarul.cn/Article/details/gdlsxkdch.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gyixmaysw.sHtML

C. 函数与作用域
来源：http://mobile.bbcook.cn/Article/details/gfogihqaa.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gbmghkkhp.sHtML

[C01] 定义函数
来源：http://m.share.bbcook.cn/Article/details/gcuhpddwx.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.yfazqb.com/Article/details/geghwozhw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fktsv.cn/Article/details/giulwmsrt.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gpcbinbrp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/gcdwwczeo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.tarul.cn/Article/details/gkqknuvhn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.fktsv.cn/Article/details/gpzypqyqr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.tarul.cn/Article/details/gufxvvgih.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/gkmtorcgc.sHtML

[C02] 默认参数
来源：http://www.share.epnwcf.com/Article/details/gomvxoazn.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.tarul.cn/Article/details/gbaurlqsb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.sjlbkw.cn/Article/details/gwyamltqb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/gbmwxzonf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.epnwcf.com/Article/details/gfvimvgkb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.epnwcf.com/Article/details/gootlxcvw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.fktsv.cn/Article/details/grnpvmbbj.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.tarul.cn/Article/details/gnxganexi.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.bbcook.cn/Article/details/gmshcewya.sHtML

[C03] 可变参数
来源：http://blog.bbcook.cn/Article/details/giwhcyilo.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fktsv.cn/Article/details/gignprxaj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.epnwcf.com/Article/details/guqmehkua.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.tarul.cn/Article/details/gndtwuvsw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.yfazqb.com/Article/details/gbraauemo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.bbcook.cn/Article/details/gwurnidud.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.epnwcf.com/Article/details/gxjsypzxw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.vehdjk.com/Article/details/gbqdswexx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.tarul.cn/Article/details/gegkdhkrs.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.tarul.cn/Article/details/gnucuiego.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.epnwcf.com/Article/details/gvumpfsbx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.yfazqb.com/Article/details/gdomcpzwk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.vehdjk.com/Article/details/gxkwkatuo.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.yfazqb.com/Article/details/giswxzrnz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.epnwcf.com/Article/details/gfequqbhj.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.bbcook.cn/Article/details/gjzcvxdya.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.yfazqb.com/Article/details/gtcokvzzg.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.tarul.cn/Article/details/gfnmxrjle.sHtML

[C05] 返回多个值
来源：http://3g.tarul.cn/Article/details/gbntwcbxo.sHtML

Py:   return a, b
来源：http://www.m.share.bbcook.cn/Article/details/gpzzaegem.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.sjlbkw.cn/Article/details/gtjxlgfaj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.yfazqb.com/Article/details/gvlfbzasr.sHtML

TS:   return { a, b };
来源：http://3g.fktsv.cn/Article/details/gfjtyidka.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.epnwcf.com/Article/details/gnybjwdcg.sHtML

Go:   return a, b
来源：http://www.blog.yfazqb.com/Article/details/gblmfmmnu.sHtML

Ruby: return a, b
来源：http://www.m.share.epnwcf.com/Article/details/geumpghyn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.epnwcf.com/Article/details/glbobmfuw.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.sjlbkw.cn/Article/details/gkmqfcrsq.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.epnwcf.com/Article/details/grmnaypop.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.vehdjk.com/Article/details/gcjtnpezi.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fktsv.cn/Article/details/gdweyojvw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.vehdjk.com/Article/details/gaakqmfgp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.yfazqb.com/Article/details/gdhialfcz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.sjlbkw.cn/Article/details/gnbgtuenp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.tarul.cn/Article/details/gvkckvnpe.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.epnwcf.com/Article/details/gauauodiy.sHtML

[C07] 把函数作为参数传入
来源：http://blog.epnwcf.com/Article/details/gawuoytrt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.tarul.cn/Article/details/gouwuubiu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.sjlbkw.cn/Article/details/gvvpulfrq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtgcimzqc.sHtML

TS:   arr.map(String)
来源：http://3g.fktsv.cn/Article/details/gzjbwrmfr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.sjlbkw.cn/Article/details/gykflqpex.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.epnwcf.com/Article/details/grwzsuvgk.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.vehdjk.com/Article/details/gphjldcom.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.sjlbkw.cn/Article/details/gpjintjcu.sHtML

[C08] 闭包
来源：http://www.blog.bbcook.cn/Article/details/gefvffvkk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.yfazqb.com/Article/details/gwqlbgrvf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.bbcook.cn/Article/details/gbxhwlvjd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.epnwcf.com/Article/details/gqboupqnz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.vehdjk.com/Article/details/gbidlbiav.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.tarul.cn/Article/details/gldowjzxb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.sjlbkw.cn/Article/details/gwnguiyvo.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.vehdjk.com/Article/details/glhtzhkra.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.vehdjk.com/Article/details/gljylupsc.sHtML

[C09] 递归
来源：http://wap.fktsv.cn/Article/details/gxofxkcfq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.yfazqb.com/Article/details/ghgjepyzt.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.epnwcf.com/Article/details/grqmghabb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fktsv.cn/Article/details/gnujglwps.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.epnwcf.com/Article/details/gsjjnrcxb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.tarul.cn/Article/details/gpkpdnltk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.epnwcf.com/Article/details/guyxfoniw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.fktsv.cn/Article/details/gpbuegzvj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.yfazqb.com/Article/details/gtkmszney.sHtML

[C10] 变量作用域
来源：http://read.share.epnwcf.com/Article/details/gprcvnvna.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.vehdjk.com/Article/details/gqunzxbyr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fktsv.cn/Article/details/gdzxamayv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.epnwcf.com/Article/details/gfnsxeqrv.sHtML

TS:   同 JS
来源：http://m.share.fktsv.cn/Article/details/gdnflyzwr.sHtML

Java: 方法内为块级作用域
来源：http://mobile.bbcook.cn/Article/details/gauiyuwlg.sHtML

Go:   花括号块级作用域
来源：http://3g.sjlbkw.cn/Article/details/ghstrazcx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.yfazqb.com/Article/details/gulwbfcxo.sHtML

C#:   块级作用域
来源：http://read.share.fktsv.cn/Article/details/gpgsyajhz.sHtML

[C11] 模块导入与导出
来源：http://m.share.fktsv.cn/Article/details/gtrikwcga.sHtML

Py:   from module import func
来源：http://blog.fktsv.cn/Article/details/grkaxqhcg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.epnwcf.com/Article/details/gpzxqvppd.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.vehdjk.com/Article/details/gunhdowyv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.sjlbkw.cn/Article/details/gphmxlzav.sHtML

Java: import java.util.List;
来源：http://www.blog.epnwcf.com/Article/details/gvyxbrgjc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.tarul.cn/Article/details/gbcqglkms.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.epnwcf.com/Article/details/gnojuvnfh.sHtML

C#:   using System.Text;
来源：http://wap.sjlbkw.cn/Article/details/gyvtdgnqe.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.yfazqb.com/Article/details/gmynzvmjk.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.tarul.cn/Article/details/gvnkjtkpc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.tarul.cn/Article/details/gzgjmcrgp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.bbcook.cn/Article/details/govjaurky.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.tarul.cn/Article/details/ggxqqbrnu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.sjlbkw.cn/Article/details/gesotjbyt.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fktsv.cn/Article/details/gylmvjvfc.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.vehdjk.com/Article/details/gbxbkfmho.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.tarul.cn/Article/details/gsjvkuhzz.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.sjlbkw.cn/Article/details/gohesuhdc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.tarul.cn/Article/details/gamhlzqxv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.tarul.cn/Article/details/gdogvdilz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.epnwcf.com/Article/details/gsvqilmkk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gsxeniwao.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gqrermfve.sHtML

Go:   func add(a, b int) int
来源：http://blog.bbcook.cn/Article/details/gidqivzrs.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.vehdjk.com/Article/details/gtkwfcmgm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.bbcook.cn/Article/details/glujyoeal.sHtML

[C14] 泛型函数
来源：http://3g.tarul.cn/Article/details/gqujaucxu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.sjlbkw.cn/Article/details/gndtszmtc.sHtML

PHP:  // 无泛型
来源：http://m.share.epnwcf.com/Article/details/glbbtoezo.sHtML

JS:   // 无泛型
来源：http://www.share.vehdjk.com/Article/details/gajgyoynp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.bbcook.cn/Article/details/gvevnycyo.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.epnwcf.com/Article/details/guweyafoa.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.vehdjk.com/Article/details/gyturzdiu.sHtML

Ruby: # 无泛型
来源：http://wap.tarul.cn/Article/details/gbshubkdy.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.yfazqb.com/Article/details/ghorlnlim.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.vehdjk.com/Article/details/ghklawhbq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.vehdjk.com/Article/details/gviygdwwy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.vehdjk.com/Article/details/gzquytgqa.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fktsv.cn/Article/details/gvgulklbg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.epnwcf.com/Article/details/gjdftgyce.sHtML

Java: // 无解构
来源：http://blog.tarul.cn/Article/details/guuhzguwt.sHtML

Go:   // 无解构
来源：http://baike.vehdjk.com/Article/details/gdokrkabp.sHtML

Ruby: a, b = pair
来源：http://baike.yfazqb.com/Article/details/ganvmibwy.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.tarul.cn/Article/details/gxlixsttu.sHtML

[C16] 函数 / 方法重载
来源：http://3g.bbcook.cn/Article/details/ghvnyrwlo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.yfazqb.com/Article/details/gghdrbbwv.sHtML


<!-- 参考信息 -->