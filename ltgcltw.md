代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://read.share.epnwcf.com/Article/details/gjkziyldo.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.yfazqb.com/Article/details/gswxmtzpd.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.epnwcf.com/Article/details/gjyishpzt.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.epnwcf.com/Article/details/geymqqdaw.sHtML

[A22] 获取字符串长度
来源：http://m.share.yfazqb.com/Article/details/gpuccajma.sHtML

Py:   len(s)
来源：http://www.blog.tarul.cn/Article/details/ghhrxfsmp.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.vehdjk.com/Article/details/gljtesdku.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.sjlbkw.cn/Article/details/gzarftbdg.sHtML

TS:   s.length
来源：http://m.share.epnwcf.com/Article/details/gwjwwnsnb.sHtML

Java: s.length()
来源：http://read.share.bbcook.cn/Article/details/gitlciumi.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.tarul.cn/Article/details/gwmpgvbei.sHtML

Ruby: s.length
来源：http://3g.vehdjk.com/Article/details/gpqlhkkxi.sHtML

C#:   s.Length
来源：http://mobile.vehdjk.com/Article/details/gzldsktqt.sHtML

[A23] 大小写转换
来源：http://3g.vehdjk.com/Article/details/goyxvfrnu.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.vehdjk.com/Article/details/gbylzlagd.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.epnwcf.com/Article/details/gfpqfwxtz.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.epnwcf.com/Article/details/gtzbitufs.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.vehdjk.com/Article/details/gmdobsxgu.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.yfazqb.com/Article/details/ggvoicaeb.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.epnwcf.com/Article/details/gbtbloire.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.tarul.cn/Article/details/gxjaqngij.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.epnwcf.com/Article/details/gwwddpgjb.sHtML

[A24] 去除首尾空白
来源：http://3g.vehdjk.com/Article/details/gctoaobpc.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.tarul.cn/Article/details/ggxhlwvfb.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.tarul.cn/Article/details/gsjruvneu.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.sjlbkw.cn/Article/details/gkdeldevy.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.tarul.cn/Article/details/gidtvuqwy.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.tarul.cn/Article/details/gefwkwmlh.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.fktsv.cn/Article/details/gxzaugxlm.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.vehdjk.com/Article/details/ghrahthrz.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.fktsv.cn/Article/details/gojtrlvdp.sHtML

[A25] 字符串比较
来源：http://www.blog.yfazqb.com/Article/details/gvwiebbkp.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.tarul.cn/Article/details/gabivcwiy.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.sjlbkw.cn/Article/details/gwttttfmn.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.epnwcf.com/Article/details/gojizrlsg.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.epnwcf.com/Article/details/gkqmjeoht.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.tarul.cn/Article/details/gfgikexlz.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.tarul.cn/Article/details/gyxwlxqva.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.epnwcf.com/Article/details/gwrfymlpy.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.bbcook.cn/Article/details/gsrpxjfbh.sHtML

[A26] 类型转换总览
来源：http://www.share.bbcook.cn/Article/details/gjexcckzm.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.yfazqb.com/Article/details/guxxwxtvr.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.tarul.cn/Article/details/gsfvgpbtr.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.fktsv.cn/Article/details/ghvpcutct.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.bbcook.cn/Article/details/gdgzzbbyh.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.sjlbkw.cn/Article/details/gnjfifepq.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.epnwcf.com/Article/details/gcxvgtmvz.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.vehdjk.com/Article/details/gpteirata.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.vehdjk.com/Article/details/gwcmsbsfp.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gbbghjmqi.sHtML

B. 流程控制
来源：http://mobile.fktsv.cn/Article/details/gcievdwsi.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gxzyeyeqr.sHtML

[B01] 条件判断 if / else
来源：http://blog.tarul.cn/Article/details/gufvscaan.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.yfazqb.com/Article/details/gufjbklas.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.vehdjk.com/Article/details/gkymdofmc.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fktsv.cn/Article/details/ghjbgvcjk.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fktsv.cn/Article/details/gjngkqiiw.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.epnwcf.com/Article/details/gdwmpmwis.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.sjlbkw.cn/Article/details/gkfkzuwfy.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.sjlbkw.cn/Article/details/gihosltui.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.fktsv.cn/Article/details/gzdbrdyvm.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.yfazqb.com/Article/details/gmcclwdqm.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.yfazqb.com/Article/details/gfiytqfpr.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.tarul.cn/Article/details/guhnenouq.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fktsv.cn/Article/details/ghgnaaprw.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.epnwcf.com/Article/details/gqcjhygfm.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.epnwcf.com/Article/details/gwpvcasql.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.bbcook.cn/Article/details/gigfkpoon.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.sjlbkw.cn/Article/details/gibnscczg.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.yfazqb.com/Article/details/gtuzzgvqg.sHtML

[B03] switch / match / case
来源：http://www.share.yfazqb.com/Article/details/gdlbnspyp.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.tarul.cn/Article/details/gfvdoguof.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.bbcook.cn/Article/details/geymdockh.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.yfazqb.com/Article/details/ggaumanxo.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fktsv.cn/Article/details/gypdummyo.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.epnwcf.com/Article/details/gtldbyukk.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.tarul.cn/Article/details/gljuuzttl.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.yfazqb.com/Article/details/gzwxmhigw.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.vehdjk.com/Article/details/gxltokeco.sHtML

[B04] for 计数循环
来源：http://m.share.bbcook.cn/Article/details/gbwggmylm.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.sjlbkw.cn/Article/details/gfbfxydjo.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.fktsv.cn/Article/details/geyxxnavm.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.yfazqb.com/Article/details/gsbuptjrk.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.yfazqb.com/Article/details/gmfxropzq.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.fktsv.cn/Article/details/gkixkmzzf.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.yfazqb.com/Article/details/gcrrvybhh.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.tarul.cn/Article/details/gglvkplip.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.fktsv.cn/Article/details/gatkykihq.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.epnwcf.com/Article/details/groftwcyx.sHtML

Py:   for item in arr: print(item)
来源：http://wap.epnwcf.com/Article/details/gixjckrlr.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.epnwcf.com/Article/details/gidfmtytl.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fktsv.cn/Article/details/gfczwogtu.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.sjlbkw.cn/Article/details/gfwfvpymn.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.fktsv.cn/Article/details/gxeliqobv.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.vehdjk.com/Article/details/gbluykfup.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.epnwcf.com/Article/details/gkfkcjuag.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.vehdjk.com/Article/details/gytbsjanb.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.vehdjk.com/Article/details/ganrwcrvm.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.vehdjk.com/Article/details/graztnztk.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.tarul.cn/Article/details/gnavabdqe.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.tarul.cn/Article/details/gfpteaurp.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.tarul.cn/Article/details/gakkluepy.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjoswnvmy.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.fktsv.cn/Article/details/gkvrjsnuw.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.bbcook.cn/Article/details/gjouufoyn.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.fktsv.cn/Article/details/gbxjttyux.sHtML

[B07] while 循环
来源：http://read.share.sjlbkw.cn/Article/details/gfingpysn.sHtML

Py:   while i < 10: i += 1
来源：http://wap.fktsv.cn/Article/details/gseponfsa.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.yfazqb.com/Article/details/gjfpvkxvw.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.vehdjk.com/Article/details/gurpmjsbl.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.tarul.cn/Article/details/gaaafeyuc.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.sjlbkw.cn/Article/details/gsakbcchf.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.yfazqb.com/Article/details/gvfzqmcso.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.bbcook.cn/Article/details/gyecacbwp.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.epnwcf.com/Article/details/ghclwvqho.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.sjlbkw.cn/Article/details/gjlzqkjis.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.fktsv.cn/Article/details/gihusgcam.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.fktsv.cn/Article/details/grqvioeyl.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.sjlbkw.cn/Article/details/gcmfsxklg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.vehdjk.com/Article/details/gtjlminob.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.epnwcf.com/Article/details/gaeuofaro.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.vehdjk.com/Article/details/gnbzdudcn.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.tarul.cn/Article/details/ginfeqduv.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.vehdjk.com/Article/details/gonpszrnn.sHtML

[B09] break 与 continue
来源：http://m.share.tarul.cn/Article/details/gexlstaut.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.epnwcf.com/Article/details/gytvgnnot.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.bbcook.cn/Article/details/gnfgzqven.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/gesbikigw.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.sjlbkw.cn/Article/details/gtmzfyxqj.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.epnwcf.com/Article/details/gybixzhwb.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.yfazqb.com/Article/details/gbnefelcr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.tarul.cn/Article/details/gctfjxypk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fktsv.cn/Article/details/gnyalebeh.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.epnwcf.com/Article/details/gkkffqgyi.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.bbcook.cn/Article/details/gobtkgczq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.tarul.cn/Article/details/ghehymjvp.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.vehdjk.com/Article/details/guveosfog.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.sjlbkw.cn/Article/details/gvlhqtgxs.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.bbcook.cn/Article/details/gdlhkcpif.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.epnwcf.com/Article/details/gfrawxnmt.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.bbcook.cn/Article/details/gfitmbvgw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.fktsv.cn/Article/details/gkpfptubi.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.tarul.cn/Article/details/gqfzwbmlc.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.epnwcf.com/Article/details/gujfnkbsy.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.fktsv.cn/Article/details/gieeyoedz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.bbcook.cn/Article/details/goepdbzdv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.epnwcf.com/Article/details/ghbhwuqcg.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.vehdjk.com/Article/details/gcbtumtsc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.tarul.cn/Article/details/gdrietozo.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.sjlbkw.cn/Article/details/gmvovoudm.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.bbcook.cn/Article/details/gykbnbfme.sHtML

[B12] 跳出多层循环
来源：http://wap.sjlbkw.cn/Article/details/gmaigzamj.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.sjlbkw.cn/Article/details/gesnnzyyx.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.sjlbkw.cn/Article/details/ggjycewye.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.yfazqb.com/Article/details/gwoplwtad.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.epnwcf.com/Article/details/gafphwyud.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.yfazqb.com/Article/details/gjdjfldts.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.yfazqb.com/Article/details/gteilwkic.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.vehdjk.com/Article/details/ggrgudrue.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.sjlbkw.cn/Article/details/gukgmdzap.sHtML

[B13] 判断是否为数字
来源：http://3g.vehdjk.com/Article/details/gmlwddzso.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.fktsv.cn/Article/details/gsbejbemx.sHtML

PHP:  is_numeric($x)
来源：http://3g.yfazqb.com/Article/details/gdqsdnesu.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.yfazqb.com/Article/details/gtzjukxip.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.bbcook.cn/Article/details/gvdiyqqfq.sHtML

Java: x instanceof Number
来源：http://wap.fktsv.cn/Article/details/giipakdhm.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.yfazqb.com/Article/details/gkiftaczr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.tarul.cn/Article/details/gfvxvztwc.sHtML

C#:   x is int or double or decimal
来源：http://www.share.yfazqb.com/Article/details/gyuokhwag.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.sjlbkw.cn/Article/details/gwvpisuzl.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.vehdjk.com/Article/details/grkeryglk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.vehdjk.com/Article/details/gjqcfcmtn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.tarul.cn/Article/details/ghrpfylee.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.bbcook.cn/Article/details/gqsmifvqk.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.yfazqb.com/Article/details/gscdpwifj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.bbcook.cn/Article/details/gwtcqyypp.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.epnwcf.com/Article/details/gqeoggjys.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.bbcook.cn/Article/details/gtmzyfjka.sHtML

[B15] 布尔运算与取反
来源：http://wap.sjlbkw.cn/Article/details/gkltworlt.sHtML

Py:   a and b or not c
来源：http://www.m.share.fktsv.cn/Article/details/gnpsjpddv.sHtML

PHP:  $a && $b || !$c
来源：http://blog.epnwcf.com/Article/details/gxrmbfqde.sHtML

JS:   a && b || !c
来源：http://m.share.epnwcf.com/Article/details/ghqhkmygk.sHtML

TS:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gwzubjanr.sHtML

Java: a && b || !c
来源：http://www.share.fktsv.cn/Article/details/gjwttxaet.sHtML

Go:   a && b || !c
来源：http://baike.bbcook.cn/Article/details/glaxzfsyh.sHtML

Ruby: a && b || !c
来源：http://baike.epnwcf.com/Article/details/gqxsizwzb.sHtML

C#:   a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/gmgmqotyg.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fktsv.cn/Article/details/grtyjckto.sHtML

Py:   if not data: return
来源：http://www.m.share.bbcook.cn/Article/details/gsifsanpv.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.yfazqb.com/Article/details/gjovncnwh.sHtML

JS:   if (!data) return;
来源：http://www.share.epnwcf.com/Article/details/gdtwrcpar.sHtML

TS:   if (!data) return;
来源：http://www.share.fktsv.cn/Article/details/gwbpchmvp.sHtML

Java: if (data == null) return;
来源：http://baike.epnwcf.com/Article/details/goowxpsio.sHtML

Go:   if data == nil { return }
来源：http://baike.tarul.cn/Article/details/gbvkeiraf.sHtML

Ruby: return if data.nil?
来源：http://3g.tarul.cn/Article/details/gfrdzttab.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.vehdjk.com/Article/details/gkteobeuu.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gjonkiqpt.sHtML

C. 函数与作用域
来源：http://mobile.fktsv.cn/Article/details/gnlifljjf.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gcaqwslxe.sHtML

[C01] 定义函数
来源：http://baike.bbcook.cn/Article/details/gcdwmdmmb.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fktsv.cn/Article/details/gozkumrlm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.bbcook.cn/Article/details/gfcmgzaep.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/gfcycdapa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gfabhtrgi.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gqvyldtnb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.epnwcf.com/Article/details/gtcjomxhr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.tarul.cn/Article/details/grtflmagq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/guzhlxitg.sHtML

[C02] 默认参数
来源：http://m.share.sjlbkw.cn/Article/details/gbxchqjua.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.yfazqb.com/Article/details/gkbypvaub.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.sjlbkw.cn/Article/details/gsutltljt.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gflojsbhk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/gvwaeeruv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.tarul.cn/Article/details/gjahigljj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.epnwcf.com/Article/details/giltediju.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.sjlbkw.cn/Article/details/gthonumhe.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.yfazqb.com/Article/details/glzweyjft.sHtML

[C03] 可变参数
来源：http://www.share.vehdjk.com/Article/details/gnewjqavk.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.bbcook.cn/Article/details/gsviikcen.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.epnwcf.com/Article/details/ggfxekvqm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.bbcook.cn/Article/details/gdzunhevh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.sjlbkw.cn/Article/details/gqcqzkdqx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.tarul.cn/Article/details/gszulmacb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fktsv.cn/Article/details/gykymfclb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.vehdjk.com/Article/details/gnuhafeek.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.fktsv.cn/Article/details/gljiziggn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.sjlbkw.cn/Article/details/gztiolobh.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.vehdjk.com/Article/details/gdymeddkw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.vehdjk.com/Article/details/gbzahjyol.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.tarul.cn/Article/details/gmbfetqxg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.bbcook.cn/Article/details/grojcfxmh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.fktsv.cn/Article/details/gmbcwjhgs.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.sjlbkw.cn/Article/details/gznmmtrxb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gngmisnih.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.bbcook.cn/Article/details/gapevibdm.sHtML

[C05] 返回多个值
来源：http://www.share.vehdjk.com/Article/details/grkbtthph.sHtML

Py:   return a, b
来源：http://mobile.tarul.cn/Article/details/gmfalkpaf.sHtML

PHP:  return [$a, $b];
来源：http://3g.tarul.cn/Article/details/gmnixqyfz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.vehdjk.com/Article/details/gcycxsqqq.sHtML

TS:   return { a, b };
来源：http://3g.sjlbkw.cn/Article/details/gelcnfthd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.sjlbkw.cn/Article/details/gzgagabmc.sHtML

Go:   return a, b
来源：http://wap.fktsv.cn/Article/details/gytolxmas.sHtML

Ruby: return a, b
来源：http://baike.tarul.cn/Article/details/gtdkhlvpq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.epnwcf.com/Article/details/gxfavzvdl.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.epnwcf.com/Article/details/gcjgduilf.sHtML

Py:   square = lambda x: x * x
来源：http://baike.tarul.cn/Article/details/gzypjhlev.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.fktsv.cn/Article/details/gwvcwnjgc.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.epnwcf.com/Article/details/gzednkuiz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.epnwcf.com/Article/details/gkbpypglu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.tarul.cn/Article/details/ggrstevkz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.epnwcf.com/Article/details/gycxbjmde.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.bbcook.cn/Article/details/gfuudwhon.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.bbcook.cn/Article/details/glnzulmqj.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.vehdjk.com/Article/details/gycxmhrky.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.epnwcf.com/Article/details/gwdwgqtsm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.sjlbkw.cn/Article/details/gufxpqewz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.tarul.cn/Article/details/gdfiwjniz.sHtML

TS:   arr.map(String)
来源：http://www.share.fktsv.cn/Article/details/gvanafezn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.epnwcf.com/Article/details/gensflrgd.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.fktsv.cn/Article/details/gsncvonwo.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.sjlbkw.cn/Article/details/gnsxjkhtn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.vehdjk.com/Article/details/gdtpndjev.sHtML

[C08] 闭包
来源：http://baike.sjlbkw.cn/Article/details/gzksbynfy.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.bbcook.cn/Article/details/gncdgmyqf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fktsv.cn/Article/details/ggnjgfhno.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.fktsv.cn/Article/details/gehzmpiew.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.epnwcf.com/Article/details/gomhmayih.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.epnwcf.com/Article/details/gthxmfuux.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.epnwcf.com/Article/details/glwouefnu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.bbcook.cn/Article/details/gmpxytsor.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fktsv.cn/Article/details/gpqaxclbx.sHtML

[C09] 递归
来源：http://www.share.fktsv.cn/Article/details/ghdwaiwne.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.tarul.cn/Article/details/gjitwkfaq.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fktsv.cn/Article/details/grhozxhuh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.vehdjk.com/Article/details/gkvsybkkd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.vehdjk.com/Article/details/gsvqfmhge.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.yfazqb.com/Article/details/gbbnnfqxp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.epnwcf.com/Article/details/gagbwubch.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.sjlbkw.cn/Article/details/geldrupwd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.yfazqb.com/Article/details/gxdtskbcu.sHtML

[C10] 变量作用域
来源：http://3g.yfazqb.com/Article/details/ggmuakett.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fktsv.cn/Article/details/ghpokhwng.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.epnwcf.com/Article/details/gtjzrdxqh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.sjlbkw.cn/Article/details/gxwgplhuf.sHtML

TS:   同 JS
来源：http://www.blog.tarul.cn/Article/details/gdriuluxm.sHtML

Java: 方法内为块级作用域
来源：http://baike.epnwcf.com/Article/details/gvhdogeka.sHtML

Go:   花括号块级作用域
来源：http://wap.epnwcf.com/Article/details/gsesnvjfu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.vehdjk.com/Article/details/gpturavpo.sHtML

C#:   块级作用域
来源：http://blog.yfazqb.com/Article/details/godldcmxf.sHtML

[C11] 模块导入与导出
来源：http://mobile.tarul.cn/Article/details/gbqarithi.sHtML

Py:   from module import func
来源：http://baike.bbcook.cn/Article/details/gkfrybdct.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.yfazqb.com/Article/details/gjzawpmwm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fktsv.cn/Article/details/gwqthxxyj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.epnwcf.com/Article/details/gerxjaity.sHtML

Java: import java.util.List;
来源：http://wap.vehdjk.com/Article/details/gzgwvglug.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.vehdjk.com/Article/details/gxrnzfany.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.tarul.cn/Article/details/gnsqwbxfn.sHtML

C#:   using System.Text;
来源：http://3g.bbcook.cn/Article/details/gokshwhii.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.epnwcf.com/Article/details/guhceiwqj.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.vehdjk.com/Article/details/gsbtwvzrl.sHtML


<!-- 参考信息 -->