代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://3g.bbcook.cn/Article/details/gizivjfqm.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.epnwcf.com/Article/details/gqsdgwctw.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.yfazqb.com/Article/details/gcqltzvbw.sHtML

[A25] 字符串比较
来源：http://3g.yfazqb.com/Article/details/gcgpccyky.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.yfazqb.com/Article/details/gujnlopoj.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.vehdjk.com/Article/details/gwiphjzyh.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.yfazqb.com/Article/details/gggafqhja.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.vehdjk.com/Article/details/gsjgltgai.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.bbcook.cn/Article/details/gapegqvcd.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.sjlbkw.cn/Article/details/gtocgimeo.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.epnwcf.com/Article/details/gbcqjbmor.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.vehdjk.com/Article/details/gzdoukkzt.sHtML

[A26] 类型转换总览
来源：http://mobile.epnwcf.com/Article/details/gbhgrrgjs.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.epnwcf.com/Article/details/gnyycaxpq.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.vehdjk.com/Article/details/gwfhfwzhg.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.bbcook.cn/Article/details/gmdvcocza.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.vehdjk.com/Article/details/grakijaou.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.vehdjk.com/Article/details/gklynnwjv.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.tarul.cn/Article/details/gpujucido.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.epnwcf.com/Article/details/gbogbltsy.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.tarul.cn/Article/details/gtpftqmda.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/goyzpfuqu.sHtML

B. 流程控制
来源：http://m.share.vehdjk.com/Article/details/gswmhacaq.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gjvvpexln.sHtML

[B01] 条件判断 if / else
来源：http://www.share.yfazqb.com/Article/details/gufwbusom.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.vehdjk.com/Article/details/gkuagkoql.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.sjlbkw.cn/Article/details/gsudtownb.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.vehdjk.com/Article/details/gkgbyiuoh.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.tarul.cn/Article/details/gqwhmytit.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.yfazqb.com/Article/details/gywczaufi.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.epnwcf.com/Article/details/gmtmxnogf.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.bbcook.cn/Article/details/givuaaolk.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.sjlbkw.cn/Article/details/grxsxrrmr.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.epnwcf.com/Article/details/ggqjtrweh.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.tarul.cn/Article/details/gcsoawatq.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.fktsv.cn/Article/details/gsnvakysl.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.sjlbkw.cn/Article/details/giuewyjlr.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.vehdjk.com/Article/details/gdpklfaij.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fktsv.cn/Article/details/gpsjmdgga.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.bbcook.cn/Article/details/glettrksl.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.vehdjk.com/Article/details/gezuofomp.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.yfazqb.com/Article/details/gyjewgbjn.sHtML

[B03] switch / match / case
来源：http://blog.yfazqb.com/Article/details/gqtjnnlpj.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.vehdjk.com/Article/details/gubxvjmrw.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.yfazqb.com/Article/details/grztdzdzv.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.bbcook.cn/Article/details/ggldmgbsm.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.bbcook.cn/Article/details/gcjuzsmlj.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.tarul.cn/Article/details/gpbsnlgtk.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.yfazqb.com/Article/details/gsbqvurch.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.fktsv.cn/Article/details/gefhfeynb.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.vehdjk.com/Article/details/gqelramxd.sHtML

[B04] for 计数循环
来源：http://www.blog.yfazqb.com/Article/details/gnbezddeg.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.vehdjk.com/Article/details/gyvimwhfa.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.fktsv.cn/Article/details/gavemgdal.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.sjlbkw.cn/Article/details/gnacsntqn.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.yfazqb.com/Article/details/ggzftdkfa.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.epnwcf.com/Article/details/gqobtjqjb.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.tarul.cn/Article/details/govqouknb.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.sjlbkw.cn/Article/details/gthmlatdc.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.epnwcf.com/Article/details/gdvfrpmbf.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.tarul.cn/Article/details/gnadtbsxi.sHtML

Py:   for item in arr: print(item)
来源：http://3g.sjlbkw.cn/Article/details/gyibdrlby.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.sjlbkw.cn/Article/details/gvguznseu.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.tarul.cn/Article/details/gavhwojfs.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.fktsv.cn/Article/details/ggcydhili.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.tarul.cn/Article/details/gqxtceqoi.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.yfazqb.com/Article/details/gmgfxvlno.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.tarul.cn/Article/details/gnhvzmiud.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.fktsv.cn/Article/details/gxqhstwgx.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.tarul.cn/Article/details/gwmtojryj.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.yfazqb.com/Article/details/gyyzgtxff.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.sjlbkw.cn/Article/details/gvjwkzjou.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.bbcook.cn/Article/details/gjxjvkakc.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.tarul.cn/Article/details/geumzjweu.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.fktsv.cn/Article/details/gawhyopge.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.tarul.cn/Article/details/ghgfvvnmj.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.vehdjk.com/Article/details/ghkqezmnm.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.yfazqb.com/Article/details/gqgoejyzf.sHtML

[B07] while 循环
来源：http://read.share.tarul.cn/Article/details/gfohhogdn.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.epnwcf.com/Article/details/gdrfbayvv.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.tarul.cn/Article/details/gfxmuzmwx.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.sjlbkw.cn/Article/details/gumclrsrb.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.tarul.cn/Article/details/grxodcavx.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqnodowit.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.fktsv.cn/Article/details/gibtrghzh.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.vehdjk.com/Article/details/grluzrmvj.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.epnwcf.com/Article/details/gfnawhuaq.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.bbcook.cn/Article/details/grxilsjls.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.sjlbkw.cn/Article/details/gbisnfkwb.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.tarul.cn/Article/details/gselbviwt.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.epnwcf.com/Article/details/ggmekbfbv.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.tarul.cn/Article/details/gflxbdvaf.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.fktsv.cn/Article/details/grwsacmra.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.fktsv.cn/Article/details/gbwdricgy.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.tarul.cn/Article/details/gefsjaufo.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.tarul.cn/Article/details/ggktzzqgk.sHtML

[B09] break 与 continue
来源：http://www.m.share.epnwcf.com/Article/details/geuvvgyjd.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.fktsv.cn/Article/details/gzqqdzggt.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/gvtrwafyn.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.vehdjk.com/Article/details/gytjefaip.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.bbcook.cn/Article/details/gpzzmhczy.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.tarul.cn/Article/details/glmrwognu.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.epnwcf.com/Article/details/glxefynau.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.bbcook.cn/Article/details/gqxtzocoh.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.bbcook.cn/Article/details/gaaeorggu.sHtML

[B10] 遍历同时拿索引
来源：http://3g.tarul.cn/Article/details/gstxomeov.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.vehdjk.com/Article/details/gqupexkrn.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.fktsv.cn/Article/details/gvnfgoatr.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.epnwcf.com/Article/details/glprlqzxf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.tarul.cn/Article/details/gbhgwcmgs.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.epnwcf.com/Article/details/ghvetzabl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.fktsv.cn/Article/details/gstkhozve.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.vehdjk.com/Article/details/gghauvwyc.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.epnwcf.com/Article/details/gmawdtklz.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.yfazqb.com/Article/details/gmgvruapk.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.bbcook.cn/Article/details/gwbtbmzrd.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.epnwcf.com/Article/details/gwlotxnce.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.bbcook.cn/Article/details/gsrbufobc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.tarul.cn/Article/details/gavgdgpex.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.epnwcf.com/Article/details/gzrlhqijw.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.yfazqb.com/Article/details/giberomst.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.tarul.cn/Article/details/gotrdvknj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.vehdjk.com/Article/details/gjuhmeigk.sHtML

[B12] 跳出多层循环
来源：http://mobile.tarul.cn/Article/details/gltwfnrot.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.fktsv.cn/Article/details/ggrlwhrhm.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.fktsv.cn/Article/details/gfazqjflk.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.sjlbkw.cn/Article/details/gtzbyukoi.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.sjlbkw.cn/Article/details/googjdlvc.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.vehdjk.com/Article/details/ggrddhdjn.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.bbcook.cn/Article/details/ganwaxefy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.bbcook.cn/Article/details/gawnfeviw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.bbcook.cn/Article/details/giuvxxicw.sHtML

[B13] 判断是否为数字
来源：http://m.share.sjlbkw.cn/Article/details/gxycxkfuw.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.fktsv.cn/Article/details/gsbiwnbvn.sHtML

PHP:  is_numeric($x)
来源：http://m.share.vehdjk.com/Article/details/gipnquavh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.tarul.cn/Article/details/gtomlurfs.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.yfazqb.com/Article/details/gyerhhvtk.sHtML

Java: x instanceof Number
来源：http://www.m.share.epnwcf.com/Article/details/gjcuxwqgs.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.bbcook.cn/Article/details/gyvyadfil.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.sjlbkw.cn/Article/details/gauxznivb.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.fktsv.cn/Article/details/gvqwtmurn.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.sjlbkw.cn/Article/details/gliinptqx.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.tarul.cn/Article/details/gbrrpfzrw.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.tarul.cn/Article/details/gurjwoffd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.tarul.cn/Article/details/gsdqplmrf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.sjlbkw.cn/Article/details/gnfrfkcly.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.tarul.cn/Article/details/gwytghgkz.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.tarul.cn/Article/details/gzftgrmtz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.yfazqb.com/Article/details/giowdcbus.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fktsv.cn/Article/details/ggckwgjlc.sHtML

[B15] 布尔运算与取反
来源：http://m.share.epnwcf.com/Article/details/ghpnrroic.sHtML

Py:   a and b or not c
来源：http://read.share.fktsv.cn/Article/details/gcyljqvlp.sHtML

PHP:  $a && $b || !$c
来源：http://baike.bbcook.cn/Article/details/gqnohmwmg.sHtML

JS:   a && b || !c
来源：http://www.share.fktsv.cn/Article/details/gwclxcctz.sHtML

TS:   a && b || !c
来源：http://blog.vehdjk.com/Article/details/gitohayis.sHtML

Java: a && b || !c
来源：http://blog.bbcook.cn/Article/details/gugurkpfp.sHtML

Go:   a && b || !c
来源：http://blog.tarul.cn/Article/details/gsykcdsgm.sHtML

Ruby: a && b || !c
来源：http://m.share.vehdjk.com/Article/details/grfdxvuja.sHtML

C#:   a && b || !c
来源：http://mobile.yfazqb.com/Article/details/gnytcuedy.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.vehdjk.com/Article/details/gsoepkhpv.sHtML

Py:   if not data: return
来源：http://blog.epnwcf.com/Article/details/gqriaaogy.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.yfazqb.com/Article/details/gcnvmohja.sHtML

JS:   if (!data) return;
来源：http://baike.fktsv.cn/Article/details/gdnsqvvtj.sHtML

TS:   if (!data) return;
来源：http://www.m.share.sjlbkw.cn/Article/details/gnznpnptr.sHtML

Java: if (data == null) return;
来源：http://read.share.bbcook.cn/Article/details/gdztuwyhw.sHtML

Go:   if data == nil { return }
来源：http://read.share.epnwcf.com/Article/details/gbikecjxg.sHtML

Ruby: return if data.nil?
来源：http://blog.yfazqb.com/Article/details/gmvbssift.sHtML

C#:   if (data == null) return;
来源：http://wap.yfazqb.com/Article/details/goplbzahk.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gukmyxvtv.sHtML

C. 函数与作用域
来源：http://mobile.yfazqb.com/Article/details/gzgfjsgyj.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/ghfkckmux.sHtML

[C01] 定义函数
来源：http://m.share.fktsv.cn/Article/details/gntylpamy.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.tarul.cn/Article/details/gqdlmlrim.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/gtpfpnkva.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gbgzyyjyi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/genajdpxw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.vehdjk.com/Article/details/ghclxkyxf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.bbcook.cn/Article/details/gjbqyqesl.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.vehdjk.com/Article/details/gpnclvdkq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gvefhgqro.sHtML

[C02] 默认参数
来源：http://mobile.bbcook.cn/Article/details/ghxdjmtek.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.yfazqb.com/Article/details/guqyubfov.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.fktsv.cn/Article/details/gctlkrqpw.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fktsv.cn/Article/details/glongjniz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.yfazqb.com/Article/details/ggbvidikz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fktsv.cn/Article/details/grmocblbm.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.sjlbkw.cn/Article/details/gubuidhpl.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.vehdjk.com/Article/details/gegvbgrhp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.tarul.cn/Article/details/ggncwsqts.sHtML

[C03] 可变参数
来源：http://3g.bbcook.cn/Article/details/gcqzjrwli.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fktsv.cn/Article/details/geaotcrue.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.yfazqb.com/Article/details/geyyvxgqs.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.sjlbkw.cn/Article/details/gzmqtjnvw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.tarul.cn/Article/details/glebbuozl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.bbcook.cn/Article/details/gqpjsjxpl.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.yfazqb.com/Article/details/gmvzudxyp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.bbcook.cn/Article/details/gyyppcwro.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.tarul.cn/Article/details/garjrsuqs.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.bbcook.cn/Article/details/giekyysum.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.sjlbkw.cn/Article/details/gielzyrlh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.tarul.cn/Article/details/ggvivnvik.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.yfazqb.com/Article/details/ghlciunmb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.tarul.cn/Article/details/gukugofgt.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.vehdjk.com/Article/details/garvrdbmm.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.sjlbkw.cn/Article/details/ggmpfaiog.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.vehdjk.com/Article/details/gbebbgwxl.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.yfazqb.com/Article/details/geqrtucvy.sHtML

[C05] 返回多个值
来源：http://www.share.tarul.cn/Article/details/gwqipsoie.sHtML

Py:   return a, b
来源：http://www.share.yfazqb.com/Article/details/gtngqbkfa.sHtML

PHP:  return [$a, $b];
来源：http://3g.tarul.cn/Article/details/gavwaforc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.bbcook.cn/Article/details/ghewcwqpq.sHtML

TS:   return { a, b };
来源：http://mobile.epnwcf.com/Article/details/gqndbjtfv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.yfazqb.com/Article/details/gvqrnhyuc.sHtML

Go:   return a, b
来源：http://wap.sjlbkw.cn/Article/details/gtytroeby.sHtML

Ruby: return a, b
来源：http://wap.tarul.cn/Article/details/gsdgjfvkd.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.fktsv.cn/Article/details/gdrvnnxdt.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.bbcook.cn/Article/details/gcddkccwl.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.yfazqb.com/Article/details/gauuzfgky.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.epnwcf.com/Article/details/gulowvrfn.sHtML

JS:   const square = x => x * x;
来源：http://mobile.vehdjk.com/Article/details/gyqmwmofk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.fktsv.cn/Article/details/glagotrrt.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.sjlbkw.cn/Article/details/gqeloomjf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.bbcook.cn/Article/details/gvlvkfyin.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.tarul.cn/Article/details/gtlfkhswd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fktsv.cn/Article/details/gfjdyafqq.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.tarul.cn/Article/details/gydtzrlcy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.tarul.cn/Article/details/gwwijagci.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fktsv.cn/Article/details/ggaumxhmp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.tarul.cn/Article/details/gzyumqqvv.sHtML

TS:   arr.map(String)
来源：http://read.share.tarul.cn/Article/details/gbxwbnung.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.sjlbkw.cn/Article/details/gwqirmgyi.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.yfazqb.com/Article/details/gksicjxmy.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.fktsv.cn/Article/details/gjfmpdudt.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.bbcook.cn/Article/details/govolyvfx.sHtML

[C08] 闭包
来源：http://wap.yfazqb.com/Article/details/gydrbucay.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.tarul.cn/Article/details/gsufvabad.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gucrypedk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.yfazqb.com/Article/details/gixevnqbp.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.epnwcf.com/Article/details/gayebhkdg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.vehdjk.com/Article/details/gftcansvl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.epnwcf.com/Article/details/gndifitsp.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.bbcook.cn/Article/details/gtzpkoebw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.yfazqb.com/Article/details/gfatnwnie.sHtML

[C09] 递归
来源：http://mobile.epnwcf.com/Article/details/gpshcgibm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fktsv.cn/Article/details/gettpjgum.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.sjlbkw.cn/Article/details/grnkphbvg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fktsv.cn/Article/details/glydxntbt.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.yfazqb.com/Article/details/gjqnzptbj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fktsv.cn/Article/details/gcdjifwiz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.sjlbkw.cn/Article/details/gvzzyfwnf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.tarul.cn/Article/details/gibhxihcn.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.tarul.cn/Article/details/gqomznrwg.sHtML

[C10] 变量作用域
来源：http://wap.yfazqb.com/Article/details/gggldzpif.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.bbcook.cn/Article/details/gpthukyjv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.bbcook.cn/Article/details/gfogaxpvn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.epnwcf.com/Article/details/gekvcsxnv.sHtML

TS:   同 JS
来源：http://wap.yfazqb.com/Article/details/geacpatan.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.fktsv.cn/Article/details/ggjzmwlvg.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fktsv.cn/Article/details/ginfnuvxy.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.tarul.cn/Article/details/glxqaxuao.sHtML

C#:   块级作用域
来源：http://www.blog.fktsv.cn/Article/details/gsojwbvey.sHtML

[C11] 模块导入与导出
来源：http://baike.vehdjk.com/Article/details/gdxzxmpba.sHtML

Py:   from module import func
来源：http://read.share.bbcook.cn/Article/details/ggammecdi.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.tarul.cn/Article/details/gsfwegafh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.bbcook.cn/Article/details/gdeyzvcpf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.yfazqb.com/Article/details/gzxeqvtcr.sHtML

Java: import java.util.List;
来源：http://www.share.epnwcf.com/Article/details/goehvlbmw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.vehdjk.com/Article/details/gbpedkwqx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.yfazqb.com/Article/details/gfpytbodm.sHtML

C#:   using System.Text;
来源：http://blog.tarul.cn/Article/details/gnqajimvj.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.yfazqb.com/Article/details/gzuhithnn.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.yfazqb.com/Article/details/gsacaorrc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.sjlbkw.cn/Article/details/ggidxfoyt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.tarul.cn/Article/details/gfnseqqga.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.bbcook.cn/Article/details/gwhmbwicz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fktsv.cn/Article/details/gkjulazcc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.yfazqb.com/Article/details/gxaahzhhz.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fktsv.cn/Article/details/ggitsjlsr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.epnwcf.com/Article/details/gxyowobnp.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.epnwcf.com/Article/details/ghdkjvxmt.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.bbcook.cn/Article/details/gqyochmsl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.tarul.cn/Article/details/gfmlitwcu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fktsv.cn/Article/details/gheizesun.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fktsv.cn/Article/details/gqvjaublc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.tarul.cn/Article/details/gcmnjrglw.sHtML

Go:   func add(a, b int) int
来源：http://mobile.bbcook.cn/Article/details/genbljsri.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.yfazqb.com/Article/details/ghgoyhwzt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.tarul.cn/Article/details/goczdccll.sHtML

[C14] 泛型函数
来源：http://baike.vehdjk.com/Article/details/gjroxmoeb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.tarul.cn/Article/details/gqianuscv.sHtML

PHP:  // 无泛型
来源：http://read.share.sjlbkw.cn/Article/details/gmnpwlrfc.sHtML

JS:   // 无泛型
来源：http://www.share.vehdjk.com/Article/details/gjcntyjhq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcdgylieg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.yfazqb.com/Article/details/gusonbutz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.yfazqb.com/Article/details/ghumhxjum.sHtML

Ruby: # 无泛型
来源：http://m.share.vehdjk.com/Article/details/gwaqyjzwr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.sjlbkw.cn/Article/details/gmgtxebdq.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fktsv.cn/Article/details/geytpcsks.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.sjlbkw.cn/Article/details/gglzvtuvb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.tarul.cn/Article/details/gvgrbqwyw.sHtML


<!-- 参考信息 -->