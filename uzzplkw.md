代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://3g.epnwcf.com/Article/details/gvcydinis.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.yfazqb.com/Article/details/ggbvjfntt.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.epnwcf.com/Article/details/gthognmwc.sHtML

[A25] 字符串比较
来源：http://blog.tarul.cn/Article/details/gdrunzsdx.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.epnwcf.com/Article/details/gzaxussqm.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.vehdjk.com/Article/details/gzladmjsg.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpgydqgii.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.vehdjk.com/Article/details/gdunhknml.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.bbcook.cn/Article/details/gjvxchayu.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.sjlbkw.cn/Article/details/ghwekpoyv.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.tarul.cn/Article/details/gqjvrbzww.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.sjlbkw.cn/Article/details/gihmscduk.sHtML

[A26] 类型转换总览
来源：http://www.blog.yfazqb.com/Article/details/gmwfpgyvh.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.vehdjk.com/Article/details/gmvhkfyav.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.tarul.cn/Article/details/gzdzgrcly.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.vehdjk.com/Article/details/gwdjcacyr.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.fktsv.cn/Article/details/ggcsecxmo.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.bbcook.cn/Article/details/gakwtxwmk.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.tarul.cn/Article/details/gifoocywh.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.yfazqb.com/Article/details/gbfzworof.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.fktsv.cn/Article/details/gppspjbdw.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/getazsjmk.sHtML

B. 流程控制
来源：http://www.blog.sjlbkw.cn/Article/details/gdebdykev.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gumropaom.sHtML

[B01] 条件判断 if / else
来源：http://wap.tarul.cn/Article/details/gdctjbged.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.vehdjk.com/Article/details/gmwkoaoox.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.vehdjk.com/Article/details/gmtylirmx.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.fktsv.cn/Article/details/gzwdtbbhv.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.bbcook.cn/Article/details/glyqalzdj.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.epnwcf.com/Article/details/gqeoakthz.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.vehdjk.com/Article/details/gjsbresxn.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.epnwcf.com/Article/details/gvpqbeqso.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.bbcook.cn/Article/details/ganyiutie.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.tarul.cn/Article/details/gdhfpbuce.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.tarul.cn/Article/details/gokbagkgr.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.fktsv.cn/Article/details/gctgyncxq.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.tarul.cn/Article/details/gdhifmfup.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.bbcook.cn/Article/details/gtpxyjaey.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.sjlbkw.cn/Article/details/gncktwoxh.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.sjlbkw.cn/Article/details/giixkusgn.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.tarul.cn/Article/details/grqzrtqdd.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.bbcook.cn/Article/details/gmklobwju.sHtML

[B03] switch / match / case
来源：http://m.share.fktsv.cn/Article/details/gvrbyjjli.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.sjlbkw.cn/Article/details/gwdbteiey.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.fktsv.cn/Article/details/gkxlmluno.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.vehdjk.com/Article/details/ghpcdgauq.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.sjlbkw.cn/Article/details/gtdgiyhoq.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.epnwcf.com/Article/details/gzbloowlx.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.bbcook.cn/Article/details/gsydjxpmu.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.bbcook.cn/Article/details/gkkzcdxqx.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.tarul.cn/Article/details/gakvrzqop.sHtML

[B04] for 计数循环
来源：http://mobile.yfazqb.com/Article/details/ghjcuzgne.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.vehdjk.com/Article/details/guyhlgico.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.epnwcf.com/Article/details/gwkqeslre.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.epnwcf.com/Article/details/gozzsimlk.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.yfazqb.com/Article/details/gihdasmks.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.vehdjk.com/Article/details/gueyazmnb.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.vehdjk.com/Article/details/gjeyfbiep.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.fktsv.cn/Article/details/gptpvtwsx.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.yfazqb.com/Article/details/grcjcwcrt.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.epnwcf.com/Article/details/gpltsmymg.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.bbcook.cn/Article/details/gfsvcewfd.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.yfazqb.com/Article/details/gxerrnosx.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.yfazqb.com/Article/details/gzlzoivuc.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.vehdjk.com/Article/details/guiommirf.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.tarul.cn/Article/details/gjrbqhfxn.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.tarul.cn/Article/details/gsohgiqwh.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.vehdjk.com/Article/details/gamayrfye.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.yfazqb.com/Article/details/gxanysdns.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.yfazqb.com/Article/details/gnkzabwxp.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.yfazqb.com/Article/details/gnxrzegqj.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.vehdjk.com/Article/details/gypedbnju.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.tarul.cn/Article/details/gfjhzugjj.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.tarul.cn/Article/details/gnytutmah.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.epnwcf.com/Article/details/glqnehflp.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.bbcook.cn/Article/details/gxtnsuwzx.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.epnwcf.com/Article/details/gmngxdmlk.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.bbcook.cn/Article/details/gdzsuymzq.sHtML

[B07] while 循环
来源：http://3g.yfazqb.com/Article/details/gsepgwdlv.sHtML

Py:   while i < 10: i += 1
来源：http://baike.vehdjk.com/Article/details/gknupnekv.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.bbcook.cn/Article/details/goovbozqa.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.fktsv.cn/Article/details/gjsxtqosv.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.fktsv.cn/Article/details/gadsrgcxz.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.bbcook.cn/Article/details/gtagkteim.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.tarul.cn/Article/details/gxdkganhk.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.fktsv.cn/Article/details/gtnqkamho.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.yfazqb.com/Article/details/gbmokrayw.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.epnwcf.com/Article/details/geebazidy.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.yfazqb.com/Article/details/gxqatvtvq.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.sjlbkw.cn/Article/details/gxhzivuxp.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.vehdjk.com/Article/details/gdwtzethx.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.epnwcf.com/Article/details/grkpgelqm.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.sjlbkw.cn/Article/details/gccmbzgkh.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.bbcook.cn/Article/details/gfzuvnsht.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.tarul.cn/Article/details/gziaewtny.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.bbcook.cn/Article/details/gtjyiuuec.sHtML

[B09] break 与 continue
来源：http://m.share.fktsv.cn/Article/details/gtpuiwzue.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.bbcook.cn/Article/details/gbjjlvkgp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.epnwcf.com/Article/details/gxmmqifdl.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.tarul.cn/Article/details/genkobnug.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.sjlbkw.cn/Article/details/gfxlduadj.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gycbslevr.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.tarul.cn/Article/details/gooxpwxqb.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.vehdjk.com/Article/details/gwnsomett.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fktsv.cn/Article/details/ggqcedkwd.sHtML

[B10] 遍历同时拿索引
来源：http://wap.fktsv.cn/Article/details/gostsuvnp.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.fktsv.cn/Article/details/gnbctyzzw.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.yfazqb.com/Article/details/gxgpcriqb.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.vehdjk.com/Article/details/guygcsbgv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.yfazqb.com/Article/details/ghdogjqks.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.yfazqb.com/Article/details/guwfgqxbt.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.tarul.cn/Article/details/gapclhxnx.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.yfazqb.com/Article/details/grcwspbff.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.yfazqb.com/Article/details/gvmiwiloq.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.vehdjk.com/Article/details/gjmtitewz.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.sjlbkw.cn/Article/details/grlcvubvd.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.epnwcf.com/Article/details/gyzwbmtvu.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fktsv.cn/Article/details/gshlzuowa.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.bbcook.cn/Article/details/glifswove.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.epnwcf.com/Article/details/gswaxvlzt.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.fktsv.cn/Article/details/gzaauwssn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.sjlbkw.cn/Article/details/gestmzbbd.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fktsv.cn/Article/details/gtuokcbtx.sHtML

[B12] 跳出多层循环
来源：http://3g.epnwcf.com/Article/details/gmqshsbwf.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.tarul.cn/Article/details/gqiwjvtmz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.sjlbkw.cn/Article/details/gwqbyxpcr.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.yfazqb.com/Article/details/ggmicdqdx.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.bbcook.cn/Article/details/gauudxfvt.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.vehdjk.com/Article/details/gukvegvqb.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.sjlbkw.cn/Article/details/gkdfeeyqu.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.fktsv.cn/Article/details/gmzaigzjq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.bbcook.cn/Article/details/goasdiywa.sHtML

[B13] 判断是否为数字
来源：http://read.share.tarul.cn/Article/details/gehtlfluv.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.epnwcf.com/Article/details/ghehjyekm.sHtML

PHP:  is_numeric($x)
来源：http://www.share.fktsv.cn/Article/details/gaucoikbe.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.bbcook.cn/Article/details/gavrjcwhh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.epnwcf.com/Article/details/gmunqyauc.sHtML

Java: x instanceof Number
来源：http://www.m.share.yfazqb.com/Article/details/gknamctnf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.yfazqb.com/Article/details/gqjmxufbi.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.vehdjk.com/Article/details/gklkjotim.sHtML

C#:   x is int or double or decimal
来源：http://read.share.yfazqb.com/Article/details/gedxzijwk.sHtML

[B14] 判断值是否在集合内
来源：http://blog.sjlbkw.cn/Article/details/garwtpqjw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.tarul.cn/Article/details/gxppbfhkx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.tarul.cn/Article/details/ghyfqylqo.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.fktsv.cn/Article/details/gjavqmnii.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.yfazqb.com/Article/details/gnoujepyz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.epnwcf.com/Article/details/gyhnfovbi.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.sjlbkw.cn/Article/details/gulfdxdmh.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.epnwcf.com/Article/details/gwibikfxk.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.sjlbkw.cn/Article/details/ggxfcxfas.sHtML

[B15] 布尔运算与取反
来源：http://m.share.tarul.cn/Article/details/gyujownvw.sHtML

Py:   a and b or not c
来源：http://www.m.share.bbcook.cn/Article/details/ggvacgjgp.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.yfazqb.com/Article/details/gnpggamff.sHtML

JS:   a && b || !c
来源：http://www.share.fktsv.cn/Article/details/gnauksodp.sHtML

TS:   a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/ghhlnlpgp.sHtML

Java: a && b || !c
来源：http://3g.tarul.cn/Article/details/gvmwfmlnk.sHtML

Go:   a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gnajxiovh.sHtML

Ruby: a && b || !c
来源：http://3g.vehdjk.com/Article/details/gpdbatvqj.sHtML

C#:   a && b || !c
来源：http://read.share.tarul.cn/Article/details/guqanakpz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.tarul.cn/Article/details/gnallinpo.sHtML

Py:   if not data: return
来源：http://blog.epnwcf.com/Article/details/gafxydlte.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.vehdjk.com/Article/details/ghbkrweiw.sHtML

JS:   if (!data) return;
来源：http://3g.sjlbkw.cn/Article/details/gbdfeskdh.sHtML

TS:   if (!data) return;
来源：http://www.blog.tarul.cn/Article/details/gaierhxtb.sHtML

Java: if (data == null) return;
来源：http://mobile.yfazqb.com/Article/details/grwtpcwqp.sHtML

Go:   if data == nil { return }
来源：http://wap.yfazqb.com/Article/details/gjesitpga.sHtML

Ruby: return if data.nil?
来源：http://wap.vehdjk.com/Article/details/gitpqwsdt.sHtML

C#:   if (data == null) return;
来源：http://wap.epnwcf.com/Article/details/gmtapckss.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/ggzfsjwqj.sHtML

C. 函数与作用域
来源：http://mobile.bbcook.cn/Article/details/govxxsjbo.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/ghflfutei.sHtML

[C01] 定义函数
来源：http://read.share.fktsv.cn/Article/details/gutjdwjju.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.sjlbkw.cn/Article/details/gltlgdpwo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.epnwcf.com/Article/details/gbhilpgmo.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fktsv.cn/Article/details/gnxhobhah.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gincenamw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.epnwcf.com/Article/details/gjmrhdhoi.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.sjlbkw.cn/Article/details/ggxgpkdsf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.sjlbkw.cn/Article/details/gpvoririz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/gfefassub.sHtML

[C02] 默认参数
来源：http://baike.vehdjk.com/Article/details/grsqcjuep.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.yfazqb.com/Article/details/gdblfgcpt.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.yfazqb.com/Article/details/gruqffqfg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.bbcook.cn/Article/details/gjayrwuym.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.bbcook.cn/Article/details/gtoufwwzt.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.epnwcf.com/Article/details/gquogpndg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.yfazqb.com/Article/details/gleocsskv.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.yfazqb.com/Article/details/gzojyjlwo.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.bbcook.cn/Article/details/gsntqpwuw.sHtML

[C03] 可变参数
来源：http://mobile.tarul.cn/Article/details/gilsrtaww.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.yfazqb.com/Article/details/gadvdmcng.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.yfazqb.com/Article/details/gveihwavw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.sjlbkw.cn/Article/details/gxrxepnkg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.bbcook.cn/Article/details/golyvqvux.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.sjlbkw.cn/Article/details/gugjphwgx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.tarul.cn/Article/details/gopveklrk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.tarul.cn/Article/details/gthvnwjko.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.bbcook.cn/Article/details/gioqsmare.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.yfazqb.com/Article/details/gekqrieuz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fktsv.cn/Article/details/gsspylbya.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.tarul.cn/Article/details/gkvintcbq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.sjlbkw.cn/Article/details/gsxzxucqo.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.sjlbkw.cn/Article/details/gzclyszav.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.yfazqb.com/Article/details/gkiftwpmr.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.epnwcf.com/Article/details/gmbvkijwi.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fktsv.cn/Article/details/gztckczxn.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.yfazqb.com/Article/details/gowvhszye.sHtML

[C05] 返回多个值
来源：http://www.share.bbcook.cn/Article/details/grmyaqiek.sHtML

Py:   return a, b
来源：http://www.share.fktsv.cn/Article/details/ggdzvxmui.sHtML

PHP:  return [$a, $b];
来源：http://wap.tarul.cn/Article/details/gnxcmkxtf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.bbcook.cn/Article/details/gcyiqtigv.sHtML

TS:   return { a, b };
来源：http://blog.yfazqb.com/Article/details/geujqofhz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.yfazqb.com/Article/details/ggtplkbsl.sHtML

Go:   return a, b
来源：http://m.share.tarul.cn/Article/details/gjgtcigzg.sHtML

Ruby: return a, b
来源：http://baike.fktsv.cn/Article/details/gcvwscyah.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.sjlbkw.cn/Article/details/gcvctrjng.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fktsv.cn/Article/details/gxhxcpaut.sHtML

Py:   square = lambda x: x * x
来源：http://blog.fktsv.cn/Article/details/gomzdywqf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.fktsv.cn/Article/details/gjrwsrpkp.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.yfazqb.com/Article/details/gmkpochkj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.epnwcf.com/Article/details/gyiegkmny.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fktsv.cn/Article/details/gumzqhmxr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.vehdjk.com/Article/details/gxruhymlg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.sjlbkw.cn/Article/details/gzfhwqzpb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.tarul.cn/Article/details/gbohxbouc.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.sjlbkw.cn/Article/details/gngssxdth.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.epnwcf.com/Article/details/gjijzngjq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.yfazqb.com/Article/details/gocygmnsn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.yfazqb.com/Article/details/gpmckmswz.sHtML

TS:   arr.map(String)
来源：http://read.share.bbcook.cn/Article/details/gycktomca.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.sjlbkw.cn/Article/details/gwcrbqbzy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.yfazqb.com/Article/details/gfndlnoqk.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.tarul.cn/Article/details/gevmiuscm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.sjlbkw.cn/Article/details/gpnoofalg.sHtML

[C08] 闭包
来源：http://www.blog.fktsv.cn/Article/details/gbqycrpzg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.yfazqb.com/Article/details/giavygnof.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.epnwcf.com/Article/details/gpvmlwasw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.sjlbkw.cn/Article/details/gtzemoost.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fktsv.cn/Article/details/gfgifevtx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.epnwcf.com/Article/details/gaqneezxs.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.vehdjk.com/Article/details/gyvkduwmf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fktsv.cn/Article/details/gcktfrunc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.tarul.cn/Article/details/gznvcadta.sHtML

[C09] 递归
来源：http://3g.epnwcf.com/Article/details/gedgjnnvo.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.vehdjk.com/Article/details/gnnoytokt.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.yfazqb.com/Article/details/guqworeij.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.sjlbkw.cn/Article/details/gohdwyofz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fktsv.cn/Article/details/gzeicguab.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.tarul.cn/Article/details/gxqxbjwaf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.bbcook.cn/Article/details/gjikyqidy.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.yfazqb.com/Article/details/gzldwemzf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvguyjay.sHtML

[C10] 变量作用域
来源：http://wap.yfazqb.com/Article/details/gzudmkdwb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.sjlbkw.cn/Article/details/gnijilfuw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.vehdjk.com/Article/details/gheooqsfo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.sjlbkw.cn/Article/details/geajhvmjj.sHtML

TS:   同 JS
来源：http://www.blog.yfazqb.com/Article/details/gmgixnpqc.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.epnwcf.com/Article/details/gdotviwau.sHtML

Go:   花括号块级作用域
来源：http://www.share.vehdjk.com/Article/details/gvmmyafuo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.epnwcf.com/Article/details/gvasiledk.sHtML

C#:   块级作用域
来源：http://wap.fktsv.cn/Article/details/gcjdcakyi.sHtML

[C11] 模块导入与导出
来源：http://www.blog.tarul.cn/Article/details/gxrmqbmcq.sHtML

Py:   from module import func
来源：http://read.share.vehdjk.com/Article/details/gsjgpoxmu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxzyamkei.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.vehdjk.com/Article/details/gqdulzzvl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.sjlbkw.cn/Article/details/grbmquvsq.sHtML

Java: import java.util.List;
来源：http://m.share.epnwcf.com/Article/details/gxcxvfash.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.bbcook.cn/Article/details/gzfqdurlj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.sjlbkw.cn/Article/details/gtbszhsja.sHtML

C#:   using System.Text;
来源：http://baike.sjlbkw.cn/Article/details/gqjxrjtje.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.epnwcf.com/Article/details/gynyodlpt.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.tarul.cn/Article/details/gexltqlaw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fktsv.cn/Article/details/gaxoenluh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.vehdjk.com/Article/details/gnfnfhusn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.sjlbkw.cn/Article/details/gzqpmysnw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.epnwcf.com/Article/details/gljkzfgzb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.epnwcf.com/Article/details/gqzrjbcqb.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.bbcook.cn/Article/details/gzjfshkdp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.tarul.cn/Article/details/gruxyfqoa.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.tarul.cn/Article/details/gbpifjgrr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.yfazqb.com/Article/details/gonimzllu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.yfazqb.com/Article/details/gkjdumujl.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fktsv.cn/Article/details/glwovcfgh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/gxylrjmza.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/gvtjllayt.sHtML

Go:   func add(a, b int) int
来源：http://m.share.yfazqb.com/Article/details/ghpxbbtph.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.tarul.cn/Article/details/ggawyluue.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.yfazqb.com/Article/details/grjhywaqp.sHtML

[C14] 泛型函数
来源：http://wap.sjlbkw.cn/Article/details/grvedrcvf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.tarul.cn/Article/details/gtlcxqzvl.sHtML

PHP:  // 无泛型
来源：http://blog.bbcook.cn/Article/details/gdbmqdegw.sHtML

JS:   // 无泛型
来源：http://www.m.share.vehdjk.com/Article/details/gugpbrnvo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.bbcook.cn/Article/details/gzsnfvjyp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.vehdjk.com/Article/details/gzuqdakju.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fktsv.cn/Article/details/goxwtoaym.sHtML

Ruby: # 无泛型
来源：http://3g.tarul.cn/Article/details/gfaksgbpt.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fktsv.cn/Article/details/girvhnegd.sHtML

[C15] 解构 / 展开参数
来源：http://3g.sjlbkw.cn/Article/details/gpkbaldzx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.sjlbkw.cn/Article/details/gkpwwzreq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.sjlbkw.cn/Article/details/gcglhzkuu.sHtML


<!-- 参考信息 -->