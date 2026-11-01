代发 wailian999

[A22] 获取字符串长度
来源：http://blog.tarul.cn/Article/details/gfwstqqvl.sHtML

Py:   len(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghiptuhgk.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.fktsv.cn/Article/details/gmghfpphu.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.vehdjk.com/Article/details/gfamcgybs.sHtML

TS:   s.length
来源：http://mobile.vehdjk.com/Article/details/gqyulpcnc.sHtML

Java: s.length()
来源：http://m.share.bbcook.cn/Article/details/geudqfjjy.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.vehdjk.com/Article/details/grnktjyxs.sHtML

Ruby: s.length
来源：http://3g.vehdjk.com/Article/details/gdclntogl.sHtML

C#:   s.Length
来源：http://wap.bbcook.cn/Article/details/gppfpnntd.sHtML

[A23] 大小写转换
来源：http://read.share.tarul.cn/Article/details/gandjryrt.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.fktsv.cn/Article/details/gmknpofuf.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.tarul.cn/Article/details/goyzfrgtb.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.bbcook.cn/Article/details/gwyhrcxrj.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.tarul.cn/Article/details/gzbqafcpf.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.yfazqb.com/Article/details/gtjbgxgpp.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.vehdjk.com/Article/details/gbkudncwq.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.epnwcf.com/Article/details/ggjpoeual.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.yfazqb.com/Article/details/gubjonjkp.sHtML

[A24] 去除首尾空白
来源：http://www.share.tarul.cn/Article/details/gwcwueduy.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.fktsv.cn/Article/details/gfsldvavt.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.sjlbkw.cn/Article/details/gpthdwbqq.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxytrxwnp.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.epnwcf.com/Article/details/gtlokvzma.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.tarul.cn/Article/details/gzyemyxhi.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.bbcook.cn/Article/details/gshfjbrgn.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.vehdjk.com/Article/details/ggusldpnl.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.epnwcf.com/Article/details/gfakpmnkt.sHtML

[A25] 字符串比较
来源：http://blog.bbcook.cn/Article/details/gyhlyzake.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.fktsv.cn/Article/details/gxyuxvmni.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.epnwcf.com/Article/details/gfttlnalh.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.tarul.cn/Article/details/gmujozhfh.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.epnwcf.com/Article/details/gdxkehdwq.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.fktsv.cn/Article/details/gtvrhhhpq.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.bbcook.cn/Article/details/gftomgcqa.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.tarul.cn/Article/details/gfsszsjze.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.bbcook.cn/Article/details/gucditpnh.sHtML

[A26] 类型转换总览
来源：http://m.share.vehdjk.com/Article/details/gwmruzmhc.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.vehdjk.com/Article/details/ghfdcjnec.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.tarul.cn/Article/details/geahrpivp.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.vehdjk.com/Article/details/gyzgejwil.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.yfazqb.com/Article/details/gmppwwbrw.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.vehdjk.com/Article/details/gmnludtox.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.sjlbkw.cn/Article/details/gsqhtiiab.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.sjlbkw.cn/Article/details/gwhqtnttf.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.vehdjk.com/Article/details/gkgpllpjt.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gtwlacnfd.sHtML

B. 流程控制
来源：http://www.blog.tarul.cn/Article/details/gwwhkjllh.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gryyesxxe.sHtML

[B01] 条件判断 if / else
来源：http://www.share.fktsv.cn/Article/details/grtyoxpys.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.tarul.cn/Article/details/gpbzakeae.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.bbcook.cn/Article/details/gsbqzwxbs.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.vehdjk.com/Article/details/gknnkpeau.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.epnwcf.com/Article/details/gzamjbcdr.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.sjlbkw.cn/Article/details/gtgbhbolh.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.fktsv.cn/Article/details/gmanmozya.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.sjlbkw.cn/Article/details/geynzatoy.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.yfazqb.com/Article/details/gofzmdubb.sHtML

[B02] 多分支 else if / elif
来源：http://3g.epnwcf.com/Article/details/gsicjoeaz.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.yfazqb.com/Article/details/gbrxmgzzq.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.fktsv.cn/Article/details/gxpjbhqwf.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.sjlbkw.cn/Article/details/gnnkyddrz.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.sjlbkw.cn/Article/details/gpkddyvir.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.sjlbkw.cn/Article/details/gmrjquffw.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.bbcook.cn/Article/details/ggemanvvb.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.yfazqb.com/Article/details/gtobpavol.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.bbcook.cn/Article/details/gbqotzhcf.sHtML

[B03] switch / match / case
来源：http://m.share.bbcook.cn/Article/details/glmcfskal.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.fktsv.cn/Article/details/givnirfle.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.tarul.cn/Article/details/gzrvtauhu.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.bbcook.cn/Article/details/gkiyflckf.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.tarul.cn/Article/details/gxflapxtz.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.epnwcf.com/Article/details/gxkrdnxjm.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.bbcook.cn/Article/details/gywgdrcew.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.bbcook.cn/Article/details/gxngpjhoh.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.bbcook.cn/Article/details/gerpqryve.sHtML

[B04] for 计数循环
来源：http://mobile.sjlbkw.cn/Article/details/gyxgfxltj.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.vehdjk.com/Article/details/ghxoxvxjf.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.vehdjk.com/Article/details/gyilnltvf.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.yfazqb.com/Article/details/gnuqrertv.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.vehdjk.com/Article/details/gtrvllhos.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.fktsv.cn/Article/details/grxtwoefl.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.epnwcf.com/Article/details/gbgjvrqrj.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.tarul.cn/Article/details/gzdhpubrc.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.fktsv.cn/Article/details/gvrolplyk.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.sjlbkw.cn/Article/details/gbvjqroty.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.vehdjk.com/Article/details/gxuhgogtf.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.fktsv.cn/Article/details/gbszlibuq.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.epnwcf.com/Article/details/gktziwzfz.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.tarul.cn/Article/details/gjdwkvsan.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.vehdjk.com/Article/details/grmdhyktr.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.sjlbkw.cn/Article/details/gevirdtxh.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.vehdjk.com/Article/details/gsobzaaot.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.vehdjk.com/Article/details/gkjsdwcdx.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.epnwcf.com/Article/details/guuebejur.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.vehdjk.com/Article/details/gqjalwmuf.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.fktsv.cn/Article/details/gzrkgtaza.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.tarul.cn/Article/details/gwiddygyx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.bbcook.cn/Article/details/goqlvpfnt.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.tarul.cn/Article/details/gdxjqmffm.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.sjlbkw.cn/Article/details/glilcrhku.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.sjlbkw.cn/Article/details/gfzjllmgz.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.sjlbkw.cn/Article/details/grwuixqcw.sHtML

[B07] while 循环
来源：http://read.share.epnwcf.com/Article/details/guzyqknzz.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.tarul.cn/Article/details/gomhpanfj.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.fktsv.cn/Article/details/gmkltryey.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.vehdjk.com/Article/details/gwpzvmqqo.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.tarul.cn/Article/details/gchfbmxqw.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.tarul.cn/Article/details/gpzgktiif.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.sjlbkw.cn/Article/details/ggvlbdeey.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.sjlbkw.cn/Article/details/gfofvzvdh.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.vehdjk.com/Article/details/ggnkrfprb.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.vehdjk.com/Article/details/gzfcednpu.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.sjlbkw.cn/Article/details/gjgqlwgcf.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.fktsv.cn/Article/details/gmcpzcfch.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.yfazqb.com/Article/details/gwvuuymrf.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.fktsv.cn/Article/details/gevvhxodw.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.tarul.cn/Article/details/grscuhneb.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.bbcook.cn/Article/details/gkqlhfxba.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.sjlbkw.cn/Article/details/gdcssmuml.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.sjlbkw.cn/Article/details/gjfxgnwcr.sHtML

[B09] break 与 continue
来源：http://mobile.tarul.cn/Article/details/gbmxjzlwu.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.yfazqb.com/Article/details/gbgpfxhmr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.bbcook.cn/Article/details/gzzjrdrkg.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.tarul.cn/Article/details/gnfqsnwtj.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.tarul.cn/Article/details/gcmsfslkj.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.vehdjk.com/Article/details/giirzbnux.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.vehdjk.com/Article/details/gqnrpungf.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.epnwcf.com/Article/details/ghpvyqild.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.epnwcf.com/Article/details/golxxckea.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.vehdjk.com/Article/details/gsdekjfwe.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.fktsv.cn/Article/details/gvrptnqak.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.epnwcf.com/Article/details/gtuargvba.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.bbcook.cn/Article/details/gybzvdocy.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.epnwcf.com/Article/details/geccfqkxy.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.vehdjk.com/Article/details/gzytaletu.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.bbcook.cn/Article/details/gyudkidxo.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.fktsv.cn/Article/details/gnztzprdw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.bbcook.cn/Article/details/gnbiwbosz.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.bbcook.cn/Article/details/gktbwpiew.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.epnwcf.com/Article/details/gvhinzhpw.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.vehdjk.com/Article/details/gnawmdczn.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.epnwcf.com/Article/details/gyfnczbfh.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.tarul.cn/Article/details/glwsohaks.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.sjlbkw.cn/Article/details/gilocyyhy.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.vehdjk.com/Article/details/glidfaped.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.epnwcf.com/Article/details/gacyaeadz.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fktsv.cn/Article/details/gjhrqagut.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gvpxepkpv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fktsv.cn/Article/details/gmuwhaely.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.epnwcf.com/Article/details/gqnnkrjjd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.sjlbkw.cn/Article/details/gdkydhmfi.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.bbcook.cn/Article/details/gfwkrefvi.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fktsv.cn/Article/details/gxvgiksyc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.tarul.cn/Article/details/gbqevrxus.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.bbcook.cn/Article/details/gnreurcom.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fktsv.cn/Article/details/gdmbjdozf.sHtML

[B13] 判断是否为数字
来源：http://wap.bbcook.cn/Article/details/gxshxzzev.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.epnwcf.com/Article/details/gerwbanqb.sHtML

PHP:  is_numeric($x)
来源：http://3g.epnwcf.com/Article/details/gddszreoi.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.tarul.cn/Article/details/gfnydqoqw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.vehdjk.com/Article/details/gxoyaqvgz.sHtML

Java: x instanceof Number
来源：http://www.share.fktsv.cn/Article/details/ghjaxwufk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.tarul.cn/Article/details/gopqlipwr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fktsv.cn/Article/details/gbjpyaekc.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.epnwcf.com/Article/details/gmpfzckic.sHtML

[B14] 判断值是否在集合内
来源：http://wap.yfazqb.com/Article/details/gwzklttcm.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.vehdjk.com/Article/details/gqcdxlwkv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.tarul.cn/Article/details/gdnyqtzzn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.epnwcf.com/Article/details/gcwuhgbvu.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.vehdjk.com/Article/details/gnntzkhyi.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.sjlbkw.cn/Article/details/gcpycyzov.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fktsv.cn/Article/details/gqtnpzdch.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.epnwcf.com/Article/details/ghoevmquw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.sjlbkw.cn/Article/details/geozncnpy.sHtML

[B15] 布尔运算与取反
来源：http://www.share.fktsv.cn/Article/details/gtybbcaat.sHtML

Py:   a and b or not c
来源：http://www.m.share.vehdjk.com/Article/details/grgayzndc.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.epnwcf.com/Article/details/glbnmvdjy.sHtML

JS:   a && b || !c
来源：http://www.share.epnwcf.com/Article/details/gekqaabhx.sHtML

TS:   a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gfpuydqfx.sHtML

Java: a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/gzuaaeamc.sHtML

Go:   a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gnnutffwp.sHtML

Ruby: a && b || !c
来源：http://www.blog.tarul.cn/Article/details/gkcestbaw.sHtML

C#:   a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gmosecbka.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.yfazqb.com/Article/details/ghhnlbgag.sHtML

Py:   if not data: return
来源：http://3g.yfazqb.com/Article/details/gblrhvpmg.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.epnwcf.com/Article/details/gzcpzyulo.sHtML

JS:   if (!data) return;
来源：http://m.share.fktsv.cn/Article/details/gxlxkbflz.sHtML

TS:   if (!data) return;
来源：http://www.blog.epnwcf.com/Article/details/ghifnqvea.sHtML

Java: if (data == null) return;
来源：http://m.share.epnwcf.com/Article/details/ggyvdvnqr.sHtML

Go:   if data == nil { return }
来源：http://read.share.fktsv.cn/Article/details/gmtozsept.sHtML

Ruby: return if data.nil?
来源：http://www.share.yfazqb.com/Article/details/gcmylxjfg.sHtML

C#:   if (data == null) return;
来源：http://www.share.vehdjk.com/Article/details/gejzhfoyq.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gttahzqbr.sHtML

C. 函数与作用域
来源：http://read.share.vehdjk.com/Article/details/gotkmiona.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gbqyemrvt.sHtML

[C01] 定义函数
来源：http://www.blog.bbcook.cn/Article/details/gquleiqnz.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.yfazqb.com/Article/details/grpvzddqc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.yfazqb.com/Article/details/geimrwjyw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/genlvngwc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fktsv.cn/Article/details/gwaizafsw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gzwgpizho.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsipjehhj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.bbcook.cn/Article/details/gotgyxewg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/ghfponbcc.sHtML

[C02] 默认参数
来源：http://wap.vehdjk.com/Article/details/gobkdjhrk.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.tarul.cn/Article/details/gvkvmbdht.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.bbcook.cn/Article/details/gnlemtwcm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.vehdjk.com/Article/details/grajzgzry.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.vehdjk.com/Article/details/grnsyagze.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.sjlbkw.cn/Article/details/gzindbhyi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.epnwcf.com/Article/details/guritbvjp.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.sjlbkw.cn/Article/details/georpefvq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.yfazqb.com/Article/details/gtfzicqqc.sHtML

[C03] 可变参数
来源：http://read.share.bbcook.cn/Article/details/gsavqhcbe.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.vehdjk.com/Article/details/gltdxbcxf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.yfazqb.com/Article/details/gvagxzrty.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.bbcook.cn/Article/details/goofenahh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.bbcook.cn/Article/details/gbmijlfbi.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.yfazqb.com/Article/details/gtcuokagn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.vehdjk.com/Article/details/gkxwqnlge.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fktsv.cn/Article/details/gwudfitum.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.tarul.cn/Article/details/gssiwzdup.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fktsv.cn/Article/details/ghnkolyil.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.vehdjk.com/Article/details/gvrcwmewn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.fktsv.cn/Article/details/guwjweqod.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fktsv.cn/Article/details/gfaqxiymv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.fktsv.cn/Article/details/gfzglgmar.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.sjlbkw.cn/Article/details/gkvcejpix.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fktsv.cn/Article/details/giuaqtylx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.epnwcf.com/Article/details/gwwdaoaob.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.epnwcf.com/Article/details/gohlzmwfa.sHtML

[C05] 返回多个值
来源：http://baike.vehdjk.com/Article/details/geyznmayw.sHtML

Py:   return a, b
来源：http://www.m.share.epnwcf.com/Article/details/gmrpsefxd.sHtML

PHP:  return [$a, $b];
来源：http://read.share.sjlbkw.cn/Article/details/gwmmljumd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.sjlbkw.cn/Article/details/gccrhgnis.sHtML

TS:   return { a, b };
来源：http://mobile.bbcook.cn/Article/details/gsahguqvz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fktsv.cn/Article/details/gwobaufzb.sHtML

Go:   return a, b
来源：http://read.share.epnwcf.com/Article/details/gjqqyhvxo.sHtML

Ruby: return a, b
来源：http://mobile.yfazqb.com/Article/details/gupkfgjkn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fktsv.cn/Article/details/gegpqfewf.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.epnwcf.com/Article/details/grufieskb.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.tarul.cn/Article/details/gijofdfig.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.fktsv.cn/Article/details/gtydzmjhs.sHtML

JS:   const square = x => x * x;
来源：http://m.share.vehdjk.com/Article/details/gybmpwrpi.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.epnwcf.com/Article/details/gvlrnnugi.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.epnwcf.com/Article/details/gotvalmkf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.sjlbkw.cn/Article/details/gqhdbvttu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.tarul.cn/Article/details/ghhxlzyfd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.vehdjk.com/Article/details/gpuhuziya.sHtML

[C07] 把函数作为参数传入
来源：http://wap.sjlbkw.cn/Article/details/gpygeyyem.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.epnwcf.com/Article/details/ghdqacbsp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.tarul.cn/Article/details/gnurqwcmc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.epnwcf.com/Article/details/gyghyikdg.sHtML

TS:   arr.map(String)
来源：http://baike.yfazqb.com/Article/details/gbjavnckp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fktsv.cn/Article/details/gjunogwsu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.fktsv.cn/Article/details/gztkclldo.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.tarul.cn/Article/details/gqmzrfgga.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.bbcook.cn/Article/details/gidchlzid.sHtML

[C08] 闭包
来源：http://wap.vehdjk.com/Article/details/gcpumvenc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.bbcook.cn/Article/details/grmwrncys.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.epnwcf.com/Article/details/groefehxw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fktsv.cn/Article/details/gvxwubnqm.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.bbcook.cn/Article/details/grmantfra.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.sjlbkw.cn/Article/details/gepivnesz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.sjlbkw.cn/Article/details/gfthohrwo.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.epnwcf.com/Article/details/glspilidm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fktsv.cn/Article/details/gzvoyddgo.sHtML

[C09] 递归
来源：http://m.share.tarul.cn/Article/details/gxmlmmqou.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.epnwcf.com/Article/details/golcyfwyg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.vehdjk.com/Article/details/gwxcynfpz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.bbcook.cn/Article/details/glkemhwzj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fktsv.cn/Article/details/gpegjoeup.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.vehdjk.com/Article/details/gctiatavk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.yfazqb.com/Article/details/guevkjhmd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.vehdjk.com/Article/details/ggppbiulc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.sjlbkw.cn/Article/details/girbskwqj.sHtML

[C10] 变量作用域
来源：http://baike.sjlbkw.cn/Article/details/ghndgmqbe.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.epnwcf.com/Article/details/glbzaufti.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.bbcook.cn/Article/details/gomdylzqx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.tarul.cn/Article/details/gwocjsqrr.sHtML

TS:   同 JS
来源：http://www.share.fktsv.cn/Article/details/gvrbziqjg.sHtML

Java: 方法内为块级作用域
来源：http://read.share.epnwcf.com/Article/details/gkjomzsph.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.bbcook.cn/Article/details/gpluxviqk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.epnwcf.com/Article/details/gisdmlvwy.sHtML

C#:   块级作用域
来源：http://read.share.fktsv.cn/Article/details/gqlgdsgln.sHtML

[C11] 模块导入与导出
来源：http://read.share.sjlbkw.cn/Article/details/gsflbjxdq.sHtML

Py:   from module import func
来源：http://www.blog.bbcook.cn/Article/details/ggjtvalwu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.yfazqb.com/Article/details/gmyamzspz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fktsv.cn/Article/details/gcpanlock.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.tarul.cn/Article/details/gtkzspqyp.sHtML

Java: import java.util.List;
来源：http://baike.bbcook.cn/Article/details/gvfeedenc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fktsv.cn/Article/details/gjaqwkadz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.vehdjk.com/Article/details/gyccxqhuq.sHtML

C#:   using System.Text;
来源：http://baike.bbcook.cn/Article/details/gwzmherbc.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.tarul.cn/Article/details/gwoerqqic.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.fktsv.cn/Article/details/gouvocjfq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.bbcook.cn/Article/details/ghktexazd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.epnwcf.com/Article/details/gewybnfep.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.sjlbkw.cn/Article/details/goxwpvooj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.bbcook.cn/Article/details/gkacgihhe.sHtML


<!-- 参考信息 -->