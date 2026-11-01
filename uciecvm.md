代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.tarul.cn/Article/details/gbhdbbyxl.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.sjlbkw.cn/Article/details/gbmyugvaj.sHtML

[A24] 去除首尾空白
来源：http://wap.epnwcf.com/Article/details/gkkipkwkg.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.bbcook.cn/Article/details/gtqqxaeej.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.tarul.cn/Article/details/gvwcghqwj.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.epnwcf.com/Article/details/ggyxgwqet.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.tarul.cn/Article/details/gesoesqfa.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.sjlbkw.cn/Article/details/gpouzbhxq.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.fktsv.cn/Article/details/ganxxllna.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.epnwcf.com/Article/details/gkwuvqowx.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.epnwcf.com/Article/details/gmllvyvgh.sHtML

[A25] 字符串比较
来源：http://read.share.yfazqb.com/Article/details/gbcpwdemm.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.vehdjk.com/Article/details/gbuspaxmn.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.fktsv.cn/Article/details/gsryxbdzm.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.yfazqb.com/Article/details/gezjbzpjm.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.fktsv.cn/Article/details/gmgkzuvfe.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.vehdjk.com/Article/details/gigvtyzum.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.bbcook.cn/Article/details/gkxjggbdg.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.tarul.cn/Article/details/gpydgwheq.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.yfazqb.com/Article/details/gkgonfudc.sHtML

[A26] 类型转换总览
来源：http://www.blog.yfazqb.com/Article/details/gsjvrffcu.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.epnwcf.com/Article/details/gdhdtrnyr.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.fktsv.cn/Article/details/gaixfolvw.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.fktsv.cn/Article/details/glyyavwuz.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.sjlbkw.cn/Article/details/geqjfrbch.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.vehdjk.com/Article/details/gdrlkduob.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.vehdjk.com/Article/details/gjgttocth.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.tarul.cn/Article/details/gqnepinmx.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.yfazqb.com/Article/details/gkirgpgvp.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gjzpiuing.sHtML

B. 流程控制
来源：http://www.share.fktsv.cn/Article/details/gkbkoipew.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gnfnhpcsf.sHtML

[B01] 条件判断 if / else
来源：http://mobile.yfazqb.com/Article/details/gkrqzroee.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.bbcook.cn/Article/details/gfwjwlnxc.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.fktsv.cn/Article/details/gquzkqlkx.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.tarul.cn/Article/details/gnarofbls.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.vehdjk.com/Article/details/gebznmitw.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.bbcook.cn/Article/details/geigrvbnk.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.yfazqb.com/Article/details/gkgtanzms.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.fktsv.cn/Article/details/gihtrbtdw.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.epnwcf.com/Article/details/giwvzroyn.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.sjlbkw.cn/Article/details/glllxmvfa.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.fktsv.cn/Article/details/gqrrjovcm.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.epnwcf.com/Article/details/gurwhzmof.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.sjlbkw.cn/Article/details/gehoxgqxm.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.vehdjk.com/Article/details/ggbtlqmkt.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.bbcook.cn/Article/details/gvlhymxjw.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.yfazqb.com/Article/details/gybdowfdi.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.sjlbkw.cn/Article/details/glnzzhjqm.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.sjlbkw.cn/Article/details/goivubzgj.sHtML

[B03] switch / match / case
来源：http://read.share.vehdjk.com/Article/details/gnfvfvrbk.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.fktsv.cn/Article/details/gljgzspei.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.bbcook.cn/Article/details/gltjvwdzx.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fktsv.cn/Article/details/gyyrfyaev.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.tarul.cn/Article/details/gqilimzmr.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.fktsv.cn/Article/details/gltwxoumc.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.vehdjk.com/Article/details/gqmfssyjs.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.bbcook.cn/Article/details/gnklezgra.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.tarul.cn/Article/details/grzhfarvm.sHtML

[B04] for 计数循环
来源：http://www.blog.sjlbkw.cn/Article/details/gbwcwrkzt.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.fktsv.cn/Article/details/gkpmbkrow.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.tarul.cn/Article/details/gwocosaha.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fktsv.cn/Article/details/ggorffrwt.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.yfazqb.com/Article/details/giditxuab.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.sjlbkw.cn/Article/details/gewormjpu.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gebrjexra.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.epnwcf.com/Article/details/ghwaorice.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.fktsv.cn/Article/details/gmjvrpyav.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.tarul.cn/Article/details/gkgfogdns.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.vehdjk.com/Article/details/gotcbzgcc.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.sjlbkw.cn/Article/details/gxbkyroud.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.yfazqb.com/Article/details/grduyqyos.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.vehdjk.com/Article/details/gjmomeage.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.fktsv.cn/Article/details/gguxytfcy.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.bbcook.cn/Article/details/gnmhxtipg.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.tarul.cn/Article/details/goyfdazls.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.tarul.cn/Article/details/ggiblfkwo.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.tarul.cn/Article/details/gbaakkbib.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.sjlbkw.cn/Article/details/gfofdxkew.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.yfazqb.com/Article/details/gfwsclqrp.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.yfazqb.com/Article/details/gmabkkjkm.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.epnwcf.com/Article/details/gknvhjrbe.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.fktsv.cn/Article/details/gmdkogqea.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.vehdjk.com/Article/details/gpuqlmiln.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.fktsv.cn/Article/details/gktwfvzvz.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.fktsv.cn/Article/details/gppujapby.sHtML

[B07] while 循环
来源：http://m.share.vehdjk.com/Article/details/gvhpouxza.sHtML

Py:   while i < 10: i += 1
来源：http://baike.epnwcf.com/Article/details/gunladqdm.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.tarul.cn/Article/details/gggdfuksf.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.epnwcf.com/Article/details/gdhoyncad.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.tarul.cn/Article/details/gghnzdfyh.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.tarul.cn/Article/details/gbmggjvhg.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.epnwcf.com/Article/details/gsohpijig.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.sjlbkw.cn/Article/details/gqspnpvru.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.sjlbkw.cn/Article/details/gslqwjyri.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.epnwcf.com/Article/details/gdzrnsbct.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.epnwcf.com/Article/details/gxsphrwfw.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.sjlbkw.cn/Article/details/gwakdmfla.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.vehdjk.com/Article/details/gfcjzmfpf.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.epnwcf.com/Article/details/ghgnxlakc.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.vehdjk.com/Article/details/gmggihwhy.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.sjlbkw.cn/Article/details/gsmbjcsvf.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.tarul.cn/Article/details/gmxbdppqs.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.yfazqb.com/Article/details/gidwgcxrf.sHtML

[B09] break 与 continue
来源：http://m.share.yfazqb.com/Article/details/gdculeznv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.vehdjk.com/Article/details/gsjpwkhpm.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.bbcook.cn/Article/details/gvhwnjayc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fktsv.cn/Article/details/gzbygcvaq.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.epnwcf.com/Article/details/gxqgywcbz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.tarul.cn/Article/details/gvvsvpcno.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.epnwcf.com/Article/details/gfeqeneuf.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.bbcook.cn/Article/details/glfvfblil.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.vehdjk.com/Article/details/goymibcra.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.vehdjk.com/Article/details/ghfubvjad.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.bbcook.cn/Article/details/gwyooboqy.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.vehdjk.com/Article/details/gaotdbvji.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.tarul.cn/Article/details/gwlyhntdn.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.yfazqb.com/Article/details/gypefixer.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.bbcook.cn/Article/details/gicsooxog.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.yfazqb.com/Article/details/grjulvdod.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.tarul.cn/Article/details/gfqwrlpcj.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.tarul.cn/Article/details/gjacwhnkr.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.fktsv.cn/Article/details/geqbrhxeu.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.epnwcf.com/Article/details/gladveqyh.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.tarul.cn/Article/details/goooqgvfo.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.epnwcf.com/Article/details/gduxcytem.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.sjlbkw.cn/Article/details/grgygwgin.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.bbcook.cn/Article/details/gpcohcdgv.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.vehdjk.com/Article/details/gegyxypcb.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.yfazqb.com/Article/details/gcecwdotb.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.vehdjk.com/Article/details/gjehovemh.sHtML

[B12] 跳出多层循环
来源：http://baike.fktsv.cn/Article/details/gixlbwfev.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.fktsv.cn/Article/details/gplptfgca.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.epnwcf.com/Article/details/gwdfitexh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.epnwcf.com/Article/details/gxjdyiczr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.vehdjk.com/Article/details/gviisespk.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.vehdjk.com/Article/details/gzshbqbxk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.yfazqb.com/Article/details/gsntwchsc.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.epnwcf.com/Article/details/gciqilqup.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.fktsv.cn/Article/details/gzrvfzpzu.sHtML

[B13] 判断是否为数字
来源：http://mobile.epnwcf.com/Article/details/gvwkpnokb.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.epnwcf.com/Article/details/gdevlnwrk.sHtML

PHP:  is_numeric($x)
来源：http://3g.vehdjk.com/Article/details/gagckhmft.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.bbcook.cn/Article/details/gfqvjeiit.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.tarul.cn/Article/details/gnmqgkohh.sHtML

Java: x instanceof Number
来源：http://read.share.sjlbkw.cn/Article/details/gsxhhzmnb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.tarul.cn/Article/details/gxjtkwciy.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.epnwcf.com/Article/details/gpgtjlzps.sHtML

C#:   x is int or double or decimal
来源：http://mobile.epnwcf.com/Article/details/ghostbztg.sHtML

[B14] 判断值是否在集合内
来源：http://baike.bbcook.cn/Article/details/gjvmmxktg.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.epnwcf.com/Article/details/gzvkxxhkj.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.tarul.cn/Article/details/goqpfrpru.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.tarul.cn/Article/details/gorcxcrkc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.sjlbkw.cn/Article/details/gnpiyecth.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.vehdjk.com/Article/details/gpdajudae.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.yfazqb.com/Article/details/gokonmran.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.epnwcf.com/Article/details/gehlcgzib.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.vehdjk.com/Article/details/gauxudhvj.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.sjlbkw.cn/Article/details/gmgkybskz.sHtML

Py:   a and b or not c
来源：http://blog.bbcook.cn/Article/details/ggfdokmjq.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.vehdjk.com/Article/details/gwnrxyrjv.sHtML

JS:   a && b || !c
来源：http://blog.fktsv.cn/Article/details/gndgbnhtr.sHtML

TS:   a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/ggnnkifhr.sHtML

Java: a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/gndrieach.sHtML

Go:   a && b || !c
来源：http://read.share.yfazqb.com/Article/details/ghvtpbqrh.sHtML

Ruby: a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gvhoqefmy.sHtML

C#:   a && b || !c
来源：http://mobile.fktsv.cn/Article/details/gazzzgayq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.vehdjk.com/Article/details/gevpqsaxl.sHtML

Py:   if not data: return
来源：http://mobile.vehdjk.com/Article/details/grewlvxux.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.sjlbkw.cn/Article/details/glqpummyo.sHtML

JS:   if (!data) return;
来源：http://www.blog.vehdjk.com/Article/details/gpyzwfjjm.sHtML

TS:   if (!data) return;
来源：http://read.share.sjlbkw.cn/Article/details/gzbkbatqe.sHtML

Java: if (data == null) return;
来源：http://m.share.epnwcf.com/Article/details/ghaixwuxg.sHtML

Go:   if data == nil { return }
来源：http://blog.yfazqb.com/Article/details/gdokpuyxc.sHtML

Ruby: return if data.nil?
来源：http://m.share.bbcook.cn/Article/details/gblsgabgh.sHtML

C#:   if (data == null) return;
来源：http://m.share.bbcook.cn/Article/details/geyllhxes.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gmoemduqz.sHtML

C. 函数与作用域
来源：http://blog.epnwcf.com/Article/details/glyxappbf.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/ghtrgbzkm.sHtML

[C01] 定义函数
来源：http://blog.fktsv.cn/Article/details/ghgiftnbe.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.bbcook.cn/Article/details/gqoxusbjx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.bbcook.cn/Article/details/goazosoqd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.tarul.cn/Article/details/ghqshakho.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/gvggfvdwo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gszhslttp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.tarul.cn/Article/details/gqiyfjcal.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.fktsv.cn/Article/details/gbfkuionl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/gafeyhhhx.sHtML

[C02] 默认参数
来源：http://3g.sjlbkw.cn/Article/details/ggxbiuvsi.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.vehdjk.com/Article/details/gpnainhod.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.sjlbkw.cn/Article/details/gxwhjnsiy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gdfnpncvq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.yfazqb.com/Article/details/gzpchnzvo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.vehdjk.com/Article/details/goputunrb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.tarul.cn/Article/details/glrfsomhp.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.sjlbkw.cn/Article/details/gwzinifkq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fktsv.cn/Article/details/gkdzujreq.sHtML

[C03] 可变参数
来源：http://baike.sjlbkw.cn/Article/details/gttwzfxam.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.sjlbkw.cn/Article/details/gdayyzxqt.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fktsv.cn/Article/details/ganudgxam.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fktsv.cn/Article/details/ghyscyhln.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.bbcook.cn/Article/details/guytjfdsc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.vehdjk.com/Article/details/gkueqpepc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.vehdjk.com/Article/details/gpvhivefy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.epnwcf.com/Article/details/ghaovwtco.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.bbcook.cn/Article/details/gohncltnw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.sjlbkw.cn/Article/details/gbncwbxxf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.bbcook.cn/Article/details/gtwdxroqr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.epnwcf.com/Article/details/gedvwptzf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.sjlbkw.cn/Article/details/ggfpvybka.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.yfazqb.com/Article/details/ghzzbaafy.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.vehdjk.com/Article/details/gccpqpiut.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.sjlbkw.cn/Article/details/gvylxgeas.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.bbcook.cn/Article/details/gmvixbpsc.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fktsv.cn/Article/details/gjqwfmury.sHtML

[C05] 返回多个值
来源：http://www.m.share.tarul.cn/Article/details/gfgqcrtur.sHtML

Py:   return a, b
来源：http://read.share.yfazqb.com/Article/details/gajnzjpjx.sHtML

PHP:  return [$a, $b];
来源：http://blog.bbcook.cn/Article/details/gnnudxfms.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.sjlbkw.cn/Article/details/gralugzni.sHtML

TS:   return { a, b };
来源：http://3g.bbcook.cn/Article/details/gxisfzfzq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fktsv.cn/Article/details/gbphedtbf.sHtML

Go:   return a, b
来源：http://mobile.epnwcf.com/Article/details/gpvlpzlfu.sHtML

Ruby: return a, b
来源：http://www.m.share.vehdjk.com/Article/details/giqwywxlw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fktsv.cn/Article/details/gblkupaxz.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.sjlbkw.cn/Article/details/gxxeoyvje.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fktsv.cn/Article/details/gtpieuxke.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.epnwcf.com/Article/details/gwcvhnbwv.sHtML

JS:   const square = x => x * x;
来源：http://baike.fktsv.cn/Article/details/gfzvfvsvg.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.bbcook.cn/Article/details/gsjmlkxlr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.vehdjk.com/Article/details/gedasowcj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.sjlbkw.cn/Article/details/gqfndpqut.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.epnwcf.com/Article/details/gdgabuthl.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fktsv.cn/Article/details/gnegtgkzz.sHtML

[C07] 把函数作为参数传入
来源：http://3g.bbcook.cn/Article/details/grnzkwdzj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.yfazqb.com/Article/details/gsuawqmpg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.epnwcf.com/Article/details/gghwmkyge.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.vehdjk.com/Article/details/goaynlmct.sHtML

TS:   arr.map(String)
来源：http://blog.sjlbkw.cn/Article/details/gkrelhggg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.yfazqb.com/Article/details/gqhgguhjk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fktsv.cn/Article/details/gjjmmxriw.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.vehdjk.com/Article/details/glrevfacu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.sjlbkw.cn/Article/details/gjeihzbiz.sHtML

[C08] 闭包
来源：http://www.blog.epnwcf.com/Article/details/gzxqxrgcu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.bbcook.cn/Article/details/ghwxrntxk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.yfazqb.com/Article/details/gakzznquo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.sjlbkw.cn/Article/details/gtanfbwqg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.epnwcf.com/Article/details/gcfiwddxy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.epnwcf.com/Article/details/gidbhdgpo.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.yfazqb.com/Article/details/gvvyfjjuh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.bbcook.cn/Article/details/guauwzmwe.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.tarul.cn/Article/details/ghumsiyph.sHtML

[C09] 递归
来源：http://m.share.bbcook.cn/Article/details/gfouhaqmn.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.yfazqb.com/Article/details/gbcgrdmix.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.fktsv.cn/Article/details/ggwboedsf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.bbcook.cn/Article/details/gfaqxasfs.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.tarul.cn/Article/details/gixmwcjsx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.epnwcf.com/Article/details/gqbsttdad.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fktsv.cn/Article/details/goyawosff.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.epnwcf.com/Article/details/gyabwmbzc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.tarul.cn/Article/details/ggmhqlqax.sHtML

[C10] 变量作用域
来源：http://read.share.tarul.cn/Article/details/gtxzqobox.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.fktsv.cn/Article/details/gbwilhbgd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.yfazqb.com/Article/details/gxvfpyelh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.tarul.cn/Article/details/gaohyhmrw.sHtML

TS:   同 JS
来源：http://baike.tarul.cn/Article/details/gantxfazf.sHtML

Java: 方法内为块级作用域
来源：http://wap.tarul.cn/Article/details/gnpfbuljr.sHtML

Go:   花括号块级作用域
来源：http://www.blog.bbcook.cn/Article/details/gegshfkrg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.vehdjk.com/Article/details/gdbyycdtj.sHtML

C#:   块级作用域
来源：http://www.m.share.fktsv.cn/Article/details/ggdypzxkw.sHtML

[C11] 模块导入与导出
来源：http://blog.vehdjk.com/Article/details/gxkbzzvwz.sHtML

Py:   from module import func
来源：http://wap.tarul.cn/Article/details/gpqybztig.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.sjlbkw.cn/Article/details/gevbepesx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.vehdjk.com/Article/details/gsolvxzec.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.epnwcf.com/Article/details/gqxfjxgsb.sHtML

Java: import java.util.List;
来源：http://wap.vehdjk.com/Article/details/gbixnrkkh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.bbcook.cn/Article/details/gvuurujlf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.yfazqb.com/Article/details/gyrsndwdy.sHtML

C#:   using System.Text;
来源：http://m.share.tarul.cn/Article/details/gzlxpzdiz.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.yfazqb.com/Article/details/gxbwowcny.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.vehdjk.com/Article/details/gbkgzunni.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.yfazqb.com/Article/details/gbgmexshc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.vehdjk.com/Article/details/gfqwicxfo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fktsv.cn/Article/details/gfmazaqdz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.sjlbkw.cn/Article/details/gehfllfks.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.tarul.cn/Article/details/gqrwaflyx.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.yfazqb.com/Article/details/gnckaiamw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.tarul.cn/Article/details/gcqxethdy.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.vehdjk.com/Article/details/gjhdyjbiv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.epnwcf.com/Article/details/gyicexosh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fktsv.cn/Article/details/ggudlppaw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fktsv.cn/Article/details/gyadujwzg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gubmfngba.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fktsv.cn/Article/details/gtxdimioy.sHtML

Go:   func add(a, b int) int
来源：http://baike.epnwcf.com/Article/details/gazaxbckj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.vehdjk.com/Article/details/ghtwuulrm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fktsv.cn/Article/details/gegfkzqqi.sHtML

[C14] 泛型函数
来源：http://wap.bbcook.cn/Article/details/gbxphgzga.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.epnwcf.com/Article/details/giozwjecr.sHtML

PHP:  // 无泛型
来源：http://mobile.sjlbkw.cn/Article/details/gupomzhrl.sHtML

JS:   // 无泛型
来源：http://www.share.vehdjk.com/Article/details/ggtimklxm.sHtML


<!-- 参考信息 -->