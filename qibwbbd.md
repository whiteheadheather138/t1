代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.vehdjk.com/Article/details/gtqfsikhb.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.vehdjk.com/Article/details/gpihsscan.sHtML

[A24] 去除首尾空白
来源：http://mobile.vehdjk.com/Article/details/gxhotjimo.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.vehdjk.com/Article/details/gqtuyemlv.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.epnwcf.com/Article/details/gwtakrhja.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.epnwcf.com/Article/details/gwakfaugt.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.sjlbkw.cn/Article/details/gahhdxynw.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.fktsv.cn/Article/details/gfsxjnlee.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.tarul.cn/Article/details/ggzsklpfb.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.bbcook.cn/Article/details/gkmvusuuq.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.tarul.cn/Article/details/gjemxxnvc.sHtML

[A25] 字符串比较
来源：http://blog.yfazqb.com/Article/details/gzioktnoe.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.sjlbkw.cn/Article/details/gdeqzmzis.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.vehdjk.com/Article/details/gozdmvvpu.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.fktsv.cn/Article/details/gnhsxtwih.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.vehdjk.com/Article/details/gqydpofvv.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.fktsv.cn/Article/details/gdfsjnftq.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.bbcook.cn/Article/details/gthhmdvio.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.sjlbkw.cn/Article/details/gbvspfbwu.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.fktsv.cn/Article/details/gqjdljaxo.sHtML

[A26] 类型转换总览
来源：http://3g.vehdjk.com/Article/details/gbgplkqhp.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.sjlbkw.cn/Article/details/gcahngsan.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.tarul.cn/Article/details/gakcbxdbo.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.bbcook.cn/Article/details/gxrctxzjf.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.vehdjk.com/Article/details/ggidnpfxq.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.epnwcf.com/Article/details/gonmlhcfg.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.sjlbkw.cn/Article/details/ghuyfured.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.sjlbkw.cn/Article/details/gumocsbpu.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.sjlbkw.cn/Article/details/gvvmdlmip.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/guocenzen.sHtML

B. 流程控制
来源：http://www.share.epnwcf.com/Article/details/ggfytmxyx.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gjgpnueal.sHtML

[B01] 条件判断 if / else
来源：http://mobile.tarul.cn/Article/details/gmhrxxxth.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.tarul.cn/Article/details/gceqhllng.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.bbcook.cn/Article/details/grummexss.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.sjlbkw.cn/Article/details/gtvjlgwbi.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.vehdjk.com/Article/details/gmqaomeke.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.epnwcf.com/Article/details/gwrsxwtvc.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.tarul.cn/Article/details/ghohlcxnc.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.bbcook.cn/Article/details/gnllshgsx.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.epnwcf.com/Article/details/gwftuocuy.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.fktsv.cn/Article/details/gxjncgzuj.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.tarul.cn/Article/details/ggxxmbpgp.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.vehdjk.com/Article/details/ggnzevqty.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.vehdjk.com/Article/details/gfgwepxof.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.epnwcf.com/Article/details/gflsbrciu.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.tarul.cn/Article/details/gbicjceir.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.fktsv.cn/Article/details/gwcdtxbxa.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.epnwcf.com/Article/details/girdcdzth.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.bbcook.cn/Article/details/gykultgon.sHtML

[B03] switch / match / case
来源：http://wap.yfazqb.com/Article/details/grolaspui.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.tarul.cn/Article/details/gilhprdmu.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.epnwcf.com/Article/details/gptmxgbwh.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fktsv.cn/Article/details/gsabuuqyu.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.sjlbkw.cn/Article/details/ggcysmwat.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.vehdjk.com/Article/details/gqrzsvedl.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.vehdjk.com/Article/details/gxlxlibbf.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.sjlbkw.cn/Article/details/gkyksltik.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.bbcook.cn/Article/details/gzlvupltj.sHtML

[B04] for 计数循环
来源：http://www.m.share.sjlbkw.cn/Article/details/grphmzkoe.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.fktsv.cn/Article/details/gjkbfqehy.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.yfazqb.com/Article/details/gztpcvekd.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.epnwcf.com/Article/details/gbknloeid.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.yfazqb.com/Article/details/gtlvxmnzp.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.fktsv.cn/Article/details/grajcobmw.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.vehdjk.com/Article/details/gxmgmwmqf.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.vehdjk.com/Article/details/gfcqmlpio.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.bbcook.cn/Article/details/gelwfcnjl.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.sjlbkw.cn/Article/details/gjglvetbq.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.sjlbkw.cn/Article/details/gqqrfohug.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.yfazqb.com/Article/details/gjlswkznp.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.bbcook.cn/Article/details/gaaqfosbx.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.sjlbkw.cn/Article/details/gtaihhepb.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.yfazqb.com/Article/details/gdhruywac.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.fktsv.cn/Article/details/gvjpmkxha.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.yfazqb.com/Article/details/guemndkvm.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.vehdjk.com/Article/details/gvjpktghm.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.yfazqb.com/Article/details/gkiqftlbd.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.epnwcf.com/Article/details/gfqjluplh.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.vehdjk.com/Article/details/gbojldswm.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.yfazqb.com/Article/details/gadcdudvc.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.sjlbkw.cn/Article/details/glkctjmhu.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.bbcook.cn/Article/details/gwlybdnev.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.fktsv.cn/Article/details/gmmhfspea.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.bbcook.cn/Article/details/gvfucfrlu.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.yfazqb.com/Article/details/gwxfidint.sHtML

[B07] while 循环
来源：http://3g.sjlbkw.cn/Article/details/gigdcaitz.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.yfazqb.com/Article/details/grkgimtxw.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.yfazqb.com/Article/details/gizsqutqh.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.vehdjk.com/Article/details/gaxsmjicr.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.sjlbkw.cn/Article/details/gafpbmwzj.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.vehdjk.com/Article/details/gnmjfcvlk.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.vehdjk.com/Article/details/gxknxdaqp.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.bbcook.cn/Article/details/gstztbezm.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.bbcook.cn/Article/details/gxvozkqfa.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.sjlbkw.cn/Article/details/gfasaolob.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.vehdjk.com/Article/details/gfbkbewrd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/gclpqacjr.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.yfazqb.com/Article/details/gdocqocjy.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.tarul.cn/Article/details/gjdbazecg.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmayosuw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.bbcook.cn/Article/details/gpuezrjjy.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.yfazqb.com/Article/details/gvnxzdkat.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.epnwcf.com/Article/details/ghffdsqdn.sHtML

[B09] break 与 continue
来源：http://m.share.sjlbkw.cn/Article/details/gswzpzwcx.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.bbcook.cn/Article/details/gmectwgpp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.sjlbkw.cn/Article/details/gjemkbycj.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fktsv.cn/Article/details/gpmhhengj.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.tarul.cn/Article/details/ggrjgiozg.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fktsv.cn/Article/details/gkqdbkxdv.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.epnwcf.com/Article/details/gguwstczx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.epnwcf.com/Article/details/gelspqnfx.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.epnwcf.com/Article/details/gnrsajmkp.sHtML

[B10] 遍历同时拿索引
来源：http://3g.epnwcf.com/Article/details/gqqepuwjt.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.epnwcf.com/Article/details/gnfvrlsmg.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.sjlbkw.cn/Article/details/ghkoadzzf.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.epnwcf.com/Article/details/gpaqehlyc.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.bbcook.cn/Article/details/gjtesmotq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.vehdjk.com/Article/details/gidfkqvku.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.fktsv.cn/Article/details/gecdnmjac.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.vehdjk.com/Article/details/groiiubdy.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.yfazqb.com/Article/details/ggsjtzzmy.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.yfazqb.com/Article/details/gtjqboivq.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.bbcook.cn/Article/details/gdftqyelp.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.tarul.cn/Article/details/gbrourbho.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.tarul.cn/Article/details/gfvfkvlzm.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.yfazqb.com/Article/details/gmyhjcdpk.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.yfazqb.com/Article/details/gnkvvhoab.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.fktsv.cn/Article/details/gjagjcfvr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fktsv.cn/Article/details/gogpedkpx.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.epnwcf.com/Article/details/gjwlrbszk.sHtML

[B12] 跳出多层循环
来源：http://baike.epnwcf.com/Article/details/gzdzjogzd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.bbcook.cn/Article/details/gsdekukks.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.yfazqb.com/Article/details/gvjnojqap.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.bbcook.cn/Article/details/giugicqys.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fktsv.cn/Article/details/gqjkximak.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.yfazqb.com/Article/details/grxtqxhbb.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.fktsv.cn/Article/details/grxhlvffv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.epnwcf.com/Article/details/gftgwczzk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.vehdjk.com/Article/details/galefbgdy.sHtML

[B13] 判断是否为数字
来源：http://read.share.tarul.cn/Article/details/gpgycxeau.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.yfazqb.com/Article/details/gnsmpuvsg.sHtML

PHP:  is_numeric($x)
来源：http://blog.bbcook.cn/Article/details/gawhcxrcj.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.vehdjk.com/Article/details/gdmwtzlck.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gjgrawpmv.sHtML

Java: x instanceof Number
来源：http://baike.vehdjk.com/Article/details/gblnpnahk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.vehdjk.com/Article/details/grtsgptgz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.bbcook.cn/Article/details/genagrnjq.sHtML

C#:   x is int or double or decimal
来源：http://wap.sjlbkw.cn/Article/details/gomyofcrl.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.sjlbkw.cn/Article/details/gotcotajg.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.epnwcf.com/Article/details/goxkkxats.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.yfazqb.com/Article/details/gwnlzfzll.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fktsv.cn/Article/details/gikzcyhqf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.tarul.cn/Article/details/gfqxkkueh.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.vehdjk.com/Article/details/gyvqpsmvw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fktsv.cn/Article/details/gclvttvwq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.fktsv.cn/Article/details/gszronzve.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.bbcook.cn/Article/details/gqjhwielp.sHtML

[B15] 布尔运算与取反
来源：http://baike.vehdjk.com/Article/details/gdrvvikkw.sHtML

Py:   a and b or not c
来源：http://blog.yfazqb.com/Article/details/gywumgcai.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.bbcook.cn/Article/details/gmqweqwzn.sHtML

JS:   a && b || !c
来源：http://m.share.epnwcf.com/Article/details/ghfhlyxst.sHtML

TS:   a && b || !c
来源：http://read.share.vehdjk.com/Article/details/ghcddbtxz.sHtML

Java: a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/gvxhgfith.sHtML

Go:   a && b || !c
来源：http://3g.fktsv.cn/Article/details/gsotlnccz.sHtML

Ruby: a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gvkdxkonb.sHtML

C#:   a && b || !c
来源：http://m.share.epnwcf.com/Article/details/glaubjfwc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.sjlbkw.cn/Article/details/gvkyzvfzs.sHtML

Py:   if not data: return
来源：http://baike.bbcook.cn/Article/details/gppmydygc.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fktsv.cn/Article/details/gavdfqltk.sHtML

JS:   if (!data) return;
来源：http://www.share.epnwcf.com/Article/details/gqeqpnbnp.sHtML

TS:   if (!data) return;
来源：http://www.blog.sjlbkw.cn/Article/details/ghhetkktb.sHtML

Java: if (data == null) return;
来源：http://blog.tarul.cn/Article/details/guqkwakxo.sHtML

Go:   if data == nil { return }
来源：http://www.blog.sjlbkw.cn/Article/details/gmxztcuxk.sHtML

Ruby: return if data.nil?
来源：http://3g.epnwcf.com/Article/details/gbcfleboq.sHtML

C#:   if (data == null) return;
来源：http://www.share.sjlbkw.cn/Article/details/gjxnaqnxr.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gmfenogak.sHtML

C. 函数与作用域
来源：http://mobile.vehdjk.com/Article/details/ganelgiue.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gvqmuxrol.sHtML

[C01] 定义函数
来源：http://3g.vehdjk.com/Article/details/giuuxpetm.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.vehdjk.com/Article/details/grmgghneh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.sjlbkw.cn/Article/details/gnfbcbvct.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/glycbbiaz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/gyzcytmdu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/gfoyrhpbc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.bbcook.cn/Article/details/gacuripml.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.tarul.cn/Article/details/glfpndmpd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.tarul.cn/Article/details/gceunbtgt.sHtML

[C02] 默认参数
来源：http://www.blog.yfazqb.com/Article/details/gsgfzdhni.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.yfazqb.com/Article/details/gaxaitgfj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.tarul.cn/Article/details/gknpbkspt.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fktsv.cn/Article/details/gwgbaqige.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gevsfmyha.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fktsv.cn/Article/details/gwpnxzjcl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.sjlbkw.cn/Article/details/gtfcymtgf.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.epnwcf.com/Article/details/gdogshsug.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.epnwcf.com/Article/details/gcoyreejq.sHtML

[C03] 可变参数
来源：http://baike.bbcook.cn/Article/details/gjirqawba.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fktsv.cn/Article/details/gviyrqwbk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.vehdjk.com/Article/details/grbnckiaw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.bbcook.cn/Article/details/gxvparjzy.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.sjlbkw.cn/Article/details/gxlalegpf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.epnwcf.com/Article/details/gtiiirkrb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fktsv.cn/Article/details/gvlkbzybz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.vehdjk.com/Article/details/gvpujwgxy.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.sjlbkw.cn/Article/details/golbwhfun.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.tarul.cn/Article/details/gvhdjnjxg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.yfazqb.com/Article/details/gvvertixg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.vehdjk.com/Article/details/gwjvuhnjz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.yfazqb.com/Article/details/gqjghiwnh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.bbcook.cn/Article/details/guxrzbnfj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.vehdjk.com/Article/details/gdfrzphyi.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.epnwcf.com/Article/details/grxyqjmce.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.fktsv.cn/Article/details/gfkbupfpz.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fktsv.cn/Article/details/gagharuht.sHtML

[C05] 返回多个值
来源：http://www.blog.fktsv.cn/Article/details/gfewxxpwo.sHtML

Py:   return a, b
来源：http://3g.sjlbkw.cn/Article/details/gejadonyt.sHtML

PHP:  return [$a, $b];
来源：http://mobile.yfazqb.com/Article/details/gicyyjxmd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.yfazqb.com/Article/details/gzsckdsbn.sHtML

TS:   return { a, b };
来源：http://baike.tarul.cn/Article/details/gigszfvxo.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.tarul.cn/Article/details/gzodwidyq.sHtML

Go:   return a, b
来源：http://blog.epnwcf.com/Article/details/gzytpfwfa.sHtML

Ruby: return a, b
来源：http://read.share.bbcook.cn/Article/details/gihrazith.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.tarul.cn/Article/details/giphqesni.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.bbcook.cn/Article/details/glnrgjqhi.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.epnwcf.com/Article/details/gmkdhoyop.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.fktsv.cn/Article/details/gfbnuntkd.sHtML

JS:   const square = x => x * x;
来源：http://wap.sjlbkw.cn/Article/details/gddikowbr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.tarul.cn/Article/details/gclgprmzo.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.yfazqb.com/Article/details/gsshzcbkz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fktsv.cn/Article/details/gmlcagjmy.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.bbcook.cn/Article/details/gsatedcfi.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.yfazqb.com/Article/details/gbsernikm.sHtML

[C07] 把函数作为参数传入
来源：http://blog.yfazqb.com/Article/details/gzhubdsxy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.bbcook.cn/Article/details/ggnggabfc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.yfazqb.com/Article/details/gmjpcxyxf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.tarul.cn/Article/details/geoqyfjoh.sHtML

TS:   arr.map(String)
来源：http://www.blog.fktsv.cn/Article/details/gqcvcbbem.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.vehdjk.com/Article/details/gcepbhaqz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.tarul.cn/Article/details/gfmdrhshe.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.epnwcf.com/Article/details/gwkyipsub.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.tarul.cn/Article/details/gnjgprjjj.sHtML

[C08] 闭包
来源：http://www.share.bbcook.cn/Article/details/gaobvmphl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fktsv.cn/Article/details/gijuermxi.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.vehdjk.com/Article/details/gjuszahiv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.fktsv.cn/Article/details/gcifaaiuf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fktsv.cn/Article/details/gqvhhvwzd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fktsv.cn/Article/details/gtqjmrmoo.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.yfazqb.com/Article/details/gwfmpwjmv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.epnwcf.com/Article/details/gjqmtcrbl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.bbcook.cn/Article/details/gifssakfy.sHtML

[C09] 递归
来源：http://www.blog.sjlbkw.cn/Article/details/gbntjjqro.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.sjlbkw.cn/Article/details/gmbaiucvp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fktsv.cn/Article/details/gogbncxao.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.bbcook.cn/Article/details/gvixydpsd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.tarul.cn/Article/details/ggrbvabps.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.sjlbkw.cn/Article/details/gqqjevzmo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.epnwcf.com/Article/details/guqcfablf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.sjlbkw.cn/Article/details/gsezjumni.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.sjlbkw.cn/Article/details/guebsmumr.sHtML

[C10] 变量作用域
来源：http://www.blog.yfazqb.com/Article/details/grpzjwhml.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.sjlbkw.cn/Article/details/gpcvmwlrm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.tarul.cn/Article/details/guopafmqo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.tarul.cn/Article/details/grxktpgcz.sHtML

TS:   同 JS
来源：http://baike.yfazqb.com/Article/details/gnxtldvjq.sHtML

Java: 方法内为块级作用域
来源：http://3g.bbcook.cn/Article/details/gywvfkqoj.sHtML

Go:   花括号块级作用域
来源：http://read.share.tarul.cn/Article/details/gnlqmzqtd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.vehdjk.com/Article/details/grzqnqrvp.sHtML

C#:   块级作用域
来源：http://www.blog.epnwcf.com/Article/details/ggfqbnesi.sHtML

[C11] 模块导入与导出
来源：http://www.blog.bbcook.cn/Article/details/gpseemvxb.sHtML

Py:   from module import func
来源：http://baike.bbcook.cn/Article/details/gsrndjfnz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.bbcook.cn/Article/details/gxwvazfub.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.yfazqb.com/Article/details/gcoqhpnta.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.sjlbkw.cn/Article/details/gmhcyadqv.sHtML

Java: import java.util.List;
来源：http://www.share.yfazqb.com/Article/details/grvwzopbz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.bbcook.cn/Article/details/glhdsalek.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fktsv.cn/Article/details/grqotfkmy.sHtML

C#:   using System.Text;
来源：http://blog.tarul.cn/Article/details/guppuutus.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fktsv.cn/Article/details/gwtcqqmtv.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.sjlbkw.cn/Article/details/gdlxvjzxq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fktsv.cn/Article/details/ggxmfcetf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.yfazqb.com/Article/details/gpgzxavxl.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.sjlbkw.cn/Article/details/gnmghbeys.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.sjlbkw.cn/Article/details/ggvjmbwuh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.vehdjk.com/Article/details/gosvpdqwb.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.yfazqb.com/Article/details/gvwgyzjnt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.tarul.cn/Article/details/gbtlpjywi.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.vehdjk.com/Article/details/ghyqmzqms.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.yfazqb.com/Article/details/grvexjhpp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fktsv.cn/Article/details/gozgbotxe.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.tarul.cn/Article/details/glaoyvcjn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.tarul.cn/Article/details/gmhlswrlb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fktsv.cn/Article/details/gjkibimch.sHtML

Go:   func add(a, b int) int
来源：http://wap.fktsv.cn/Article/details/gucbabjyy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.epnwcf.com/Article/details/gfgqhghoe.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.yfazqb.com/Article/details/gvtvkywuq.sHtML

[C14] 泛型函数
来源：http://read.share.fktsv.cn/Article/details/glvopdkay.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.epnwcf.com/Article/details/gvgkdypuc.sHtML

PHP:  // 无泛型
来源：http://baike.sjlbkw.cn/Article/details/gmpgoohik.sHtML

JS:   // 无泛型
来源：http://m.share.epnwcf.com/Article/details/gawjilwbw.sHtML


<!-- 参考信息 -->