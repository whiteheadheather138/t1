代发 wailian999

Ruby: a, b = b, a
来源：http://www.m.share.sjlbkw.cn/Article/details/gsiypnody.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.fktsv.cn/Article/details/gzofspbqt.sHtML

[A20] 读取标准输入
来源：http://baike.tarul.cn/Article/details/gigpsezlo.sHtML

Py:   name = input("请输入：")
来源：http://m.share.yfazqb.com/Article/details/ggavjxxgd.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.tarul.cn/Article/details/ghlxcnqkm.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.sjlbkw.cn/Article/details/grtglzqhb.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.yfazqb.com/Article/details/gkmyidbgy.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.yfazqb.com/Article/details/gvftddeny.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.yfazqb.com/Article/details/gsvcwarsd.sHtML

Ruby: gets.chomp
来源：http://www.share.sjlbkw.cn/Article/details/gvrfqsnqi.sHtML

C#:   Console.ReadLine();
来源：http://mobile.yfazqb.com/Article/details/gpeotwrkp.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.sjlbkw.cn/Article/details/gdlffopbo.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.epnwcf.com/Article/details/gqshbcufu.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.fktsv.cn/Article/details/gvrqjzbty.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.bbcook.cn/Article/details/gwkzzjppu.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.bbcook.cn/Article/details/gifvwxylt.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.tarul.cn/Article/details/gbqpmpzem.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.fktsv.cn/Article/details/gdzmbcsfx.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.vehdjk.com/Article/details/gqcezdjnr.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.sjlbkw.cn/Article/details/gpuwbimms.sHtML

[A22] 获取字符串长度
来源：http://mobile.vehdjk.com/Article/details/gjuccjfra.sHtML

Py:   len(s)
来源：http://www.share.epnwcf.com/Article/details/gfzjkujwx.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.tarul.cn/Article/details/gxdwhiqqh.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.epnwcf.com/Article/details/gdhrmyras.sHtML

TS:   s.length
来源：http://baike.vehdjk.com/Article/details/gnspfmgwb.sHtML

Java: s.length()
来源：http://www.blog.epnwcf.com/Article/details/gmelfhwhw.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.epnwcf.com/Article/details/gtjkxzzxr.sHtML

Ruby: s.length
来源：http://m.share.yfazqb.com/Article/details/gfqyodxpv.sHtML

C#:   s.Length
来源：http://wap.bbcook.cn/Article/details/glcbguanp.sHtML

[A23] 大小写转换
来源：http://wap.bbcook.cn/Article/details/gkvgcbtfx.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.fktsv.cn/Article/details/guymkzvep.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.sjlbkw.cn/Article/details/grvbtnlvn.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.bbcook.cn/Article/details/gswvumedg.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.epnwcf.com/Article/details/ggpwhsweb.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.yfazqb.com/Article/details/gbtsqhshc.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.fktsv.cn/Article/details/gyxuxxhkz.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.yfazqb.com/Article/details/gyteleeii.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.epnwcf.com/Article/details/ggomgewni.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.vehdjk.com/Article/details/grwmsicff.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.epnwcf.com/Article/details/gziqevuqf.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.tarul.cn/Article/details/gqpbstjlm.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.fktsv.cn/Article/details/gnjpacvhf.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.yfazqb.com/Article/details/gykkiwmdf.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.epnwcf.com/Article/details/gnnbdoysc.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.sjlbkw.cn/Article/details/gjpenjptp.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.epnwcf.com/Article/details/gufxtxgkp.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.fktsv.cn/Article/details/gwnbljwjn.sHtML

[A25] 字符串比较
来源：http://read.share.epnwcf.com/Article/details/gvkzqjlwr.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.vehdjk.com/Article/details/gorqbodwq.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.epnwcf.com/Article/details/gpmtzkebj.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.tarul.cn/Article/details/gtcskzovb.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.sjlbkw.cn/Article/details/giadgwbbc.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.sjlbkw.cn/Article/details/gplchusoi.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.tarul.cn/Article/details/gtqytifhy.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.epnwcf.com/Article/details/gaovnsatw.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.fktsv.cn/Article/details/gyysgquga.sHtML

[A26] 类型转换总览
来源：http://3g.sjlbkw.cn/Article/details/gtiowojtd.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.vehdjk.com/Article/details/gwadfhxfs.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.vehdjk.com/Article/details/gvhzcijlw.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.epnwcf.com/Article/details/ghbnbuvty.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.tarul.cn/Article/details/grridhhlf.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.bbcook.cn/Article/details/gjewbskhx.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.fktsv.cn/Article/details/gipimtzbu.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.bbcook.cn/Article/details/gjbcchasu.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.epnwcf.com/Article/details/girqrnxcl.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gosmpzgtj.sHtML

B. 流程控制
来源：http://www.m.share.fktsv.cn/Article/details/gzieqjixm.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/glsahwjsu.sHtML

[B01] 条件判断 if / else
来源：http://www.share.epnwcf.com/Article/details/gvusayrjm.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.tarul.cn/Article/details/gtfstefoh.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.sjlbkw.cn/Article/details/grkkzfdeq.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fktsv.cn/Article/details/gvseykpaz.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.vehdjk.com/Article/details/gzkgxstmf.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.epnwcf.com/Article/details/gfdytdmvt.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.epnwcf.com/Article/details/gwwbrwtyo.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.yfazqb.com/Article/details/ggqelqnht.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.vehdjk.com/Article/details/gqdsolayl.sHtML

[B02] 多分支 else if / elif
来源：http://wap.fktsv.cn/Article/details/gwjlhxcpf.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.yfazqb.com/Article/details/gnwpprtws.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.tarul.cn/Article/details/gcavzpffq.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.epnwcf.com/Article/details/gergetkmf.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.tarul.cn/Article/details/gswnntyuo.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.tarul.cn/Article/details/gofvfxxjg.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.sjlbkw.cn/Article/details/gtrfnvjvp.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.tarul.cn/Article/details/gmwrfikzh.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.epnwcf.com/Article/details/gasbniznl.sHtML

[B03] switch / match / case
来源：http://3g.tarul.cn/Article/details/guqhxighm.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.bbcook.cn/Article/details/gbwqdqnlm.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.tarul.cn/Article/details/glfjjexcv.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.vehdjk.com/Article/details/gwaezhlvs.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.bbcook.cn/Article/details/gredpagmh.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.fktsv.cn/Article/details/gfsezglam.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.fktsv.cn/Article/details/gowakflxa.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.epnwcf.com/Article/details/ggvfryyqk.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.fktsv.cn/Article/details/guawqsrty.sHtML

[B04] for 计数循环
来源：http://www.blog.fktsv.cn/Article/details/gexnhbsmk.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.tarul.cn/Article/details/gnapsgnfo.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.vehdjk.com/Article/details/gvepfbtud.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.yfazqb.com/Article/details/gzafsthtb.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.yfazqb.com/Article/details/gbnzxpmtj.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.yfazqb.com/Article/details/gdynsvcda.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.tarul.cn/Article/details/gbwjcxgpf.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.sjlbkw.cn/Article/details/gxxcgvtvf.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.tarul.cn/Article/details/gubkpqvhg.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.tarul.cn/Article/details/gchljnoij.sHtML

Py:   for item in arr: print(item)
来源：http://3g.bbcook.cn/Article/details/gdgjopuai.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.tarul.cn/Article/details/guzrvuluq.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.epnwcf.com/Article/details/glptvrdgi.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.yfazqb.com/Article/details/giqfxiwmp.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.bbcook.cn/Article/details/gpsninesb.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.yfazqb.com/Article/details/gjvuiprti.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.tarul.cn/Article/details/gazuvfiyi.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.fktsv.cn/Article/details/gwrpffljp.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.epnwcf.com/Article/details/ghobokvnd.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.epnwcf.com/Article/details/guhliotaj.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.yfazqb.com/Article/details/gybtlvolx.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.epnwcf.com/Article/details/gatvppeuz.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fktsv.cn/Article/details/gfopsgxlq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.sjlbkw.cn/Article/details/gntxhmjvd.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.yfazqb.com/Article/details/gciaieyza.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.sjlbkw.cn/Article/details/gdgladryl.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.tarul.cn/Article/details/ggpmpwslj.sHtML

[B07] while 循环
来源：http://3g.sjlbkw.cn/Article/details/gunwiauzc.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.epnwcf.com/Article/details/ggnfxbmbh.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.tarul.cn/Article/details/grlqwvtmj.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.tarul.cn/Article/details/gsxgvelun.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.tarul.cn/Article/details/gjdkffegl.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.fktsv.cn/Article/details/grhxjtvjm.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.vehdjk.com/Article/details/gmmgkdqyy.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.sjlbkw.cn/Article/details/gbnremtqf.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.sjlbkw.cn/Article/details/gnyadefov.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.vehdjk.com/Article/details/goyyjljaf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.fktsv.cn/Article/details/gjesjfpfd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.fktsv.cn/Article/details/grwynygdr.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.tarul.cn/Article/details/gxxybaqoe.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.bbcook.cn/Article/details/gwhpjnxzv.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.vehdjk.com/Article/details/gmjdxnqwd.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.yfazqb.com/Article/details/gxjgjhopx.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.tarul.cn/Article/details/gtmvfpons.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.bbcook.cn/Article/details/gpzzwwdin.sHtML

[B09] break 与 continue
来源：http://blog.yfazqb.com/Article/details/gkcxohznq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.sjlbkw.cn/Article/details/gptfffpkj.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.fktsv.cn/Article/details/gjtfuyrpa.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.tarul.cn/Article/details/ggzsxqewb.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/gzskfxuql.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.bbcook.cn/Article/details/gcqmpuume.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.bbcook.cn/Article/details/gdfolqtoq.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.sjlbkw.cn/Article/details/gadadfngs.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fktsv.cn/Article/details/gtufewbxv.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.tarul.cn/Article/details/gltsarlaq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.bbcook.cn/Article/details/gfhaqcewq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.vehdjk.com/Article/details/gkpbkmlif.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.sjlbkw.cn/Article/details/gejmukzhl.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.yfazqb.com/Article/details/gbevjkddx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.bbcook.cn/Article/details/gmvwtsbhc.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.epnwcf.com/Article/details/gybevaopd.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.fktsv.cn/Article/details/gqaqxnjno.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.sjlbkw.cn/Article/details/gbdvaedfu.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.yfazqb.com/Article/details/gjuxgkrqe.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.vehdjk.com/Article/details/gqtvykziy.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.vehdjk.com/Article/details/gtfyalkfl.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fktsv.cn/Article/details/gkbafutzj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.vehdjk.com/Article/details/gavlyakgg.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gcxiuprzt.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.fktsv.cn/Article/details/gtfogsmcy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.sjlbkw.cn/Article/details/gixlnguea.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.yfazqb.com/Article/details/getnhvstm.sHtML

[B12] 跳出多层循环
来源：http://www.share.bbcook.cn/Article/details/gbnjqrnqi.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.sjlbkw.cn/Article/details/grzhwdbgn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.fktsv.cn/Article/details/gpzmoqxvp.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.yfazqb.com/Article/details/gijgcjefj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.yfazqb.com/Article/details/gqdtyigkn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.sjlbkw.cn/Article/details/gmtmyacww.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.tarul.cn/Article/details/gojolrbnf.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.bbcook.cn/Article/details/gxuxpinja.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.yfazqb.com/Article/details/gbatliowc.sHtML

[B13] 判断是否为数字
来源：http://www.share.epnwcf.com/Article/details/gwpppjynt.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.fktsv.cn/Article/details/gyypkckuv.sHtML

PHP:  is_numeric($x)
来源：http://baike.yfazqb.com/Article/details/ggyazatkw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.vehdjk.com/Article/details/gwtlvdxef.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.vehdjk.com/Article/details/glmcrchtu.sHtML

Java: x instanceof Number
来源：http://read.share.epnwcf.com/Article/details/ghayybopf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.epnwcf.com/Article/details/gsgfukyxt.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.tarul.cn/Article/details/ggciwlvhq.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.vehdjk.com/Article/details/gxcdsbgzo.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.sjlbkw.cn/Article/details/gcypzecwy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.yfazqb.com/Article/details/gjcoltkxp.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.yfazqb.com/Article/details/gdboosrqg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.epnwcf.com/Article/details/gtyziqyal.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.tarul.cn/Article/details/grihxrjuj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.sjlbkw.cn/Article/details/gexhsnoat.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.bbcook.cn/Article/details/gnjtaqsya.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.vehdjk.com/Article/details/gwrawgqbb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.yfazqb.com/Article/details/gkwiswrkc.sHtML

[B15] 布尔运算与取反
来源：http://read.share.vehdjk.com/Article/details/ggzibhooa.sHtML

Py:   a and b or not c
来源：http://blog.yfazqb.com/Article/details/gzlbxzvuj.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.sjlbkw.cn/Article/details/gbsvsnqge.sHtML

JS:   a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/gcwvlwoew.sHtML

TS:   a && b || !c
来源：http://wap.fktsv.cn/Article/details/gwsbkmsmk.sHtML

Java: a && b || !c
来源：http://wap.tarul.cn/Article/details/gyovyxsry.sHtML

Go:   a && b || !c
来源：http://mobile.epnwcf.com/Article/details/gatnsrbqe.sHtML

Ruby: a && b || !c
来源：http://wap.vehdjk.com/Article/details/gvosmqcvh.sHtML

C#:   a && b || !c
来源：http://mobile.yfazqb.com/Article/details/gwnurwfja.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.epnwcf.com/Article/details/gstijheed.sHtML

Py:   if not data: return
来源：http://www.blog.vehdjk.com/Article/details/gwdwrfwgf.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.bbcook.cn/Article/details/gielfhfoh.sHtML

JS:   if (!data) return;
来源：http://blog.yfazqb.com/Article/details/gkocdynqm.sHtML

TS:   if (!data) return;
来源：http://www.share.tarul.cn/Article/details/ggfvuvwlo.sHtML

Java: if (data == null) return;
来源：http://3g.yfazqb.com/Article/details/gulfrbiok.sHtML

Go:   if data == nil { return }
来源：http://read.share.sjlbkw.cn/Article/details/gtzgnxmvb.sHtML

Ruby: return if data.nil?
来源：http://www.blog.tarul.cn/Article/details/goynqohlt.sHtML

C#:   if (data == null) return;
来源：http://read.share.vehdjk.com/Article/details/gzvgqpjdu.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/glhovnnkh.sHtML

C. 函数与作用域
来源：http://blog.vehdjk.com/Article/details/gsmdhylet.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gaymrnohb.sHtML

[C01] 定义函数
来源：http://read.share.tarul.cn/Article/details/gzmnmmblz.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.yfazqb.com/Article/details/gwqfzegzf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.vehdjk.com/Article/details/gnycptldh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/gzngvgmjz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gicaffakw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/graihrhyp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.yfazqb.com/Article/details/gvyrkzlrh.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.bbcook.cn/Article/details/gkhqlwhbb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/gmgcntgqv.sHtML

[C02] 默认参数
来源：http://3g.bbcook.cn/Article/details/gfbbmeyju.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.vehdjk.com/Article/details/gvyvjhnjn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fktsv.cn/Article/details/gmbfixwjn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.sjlbkw.cn/Article/details/gpqyyagjv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.bbcook.cn/Article/details/gyfrladml.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.bbcook.cn/Article/details/gkivqkeeb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.fktsv.cn/Article/details/gsemihtwz.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.yfazqb.com/Article/details/gtvddyqgv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.sjlbkw.cn/Article/details/gkgwqhyaa.sHtML

[C03] 可变参数
来源：http://wap.vehdjk.com/Article/details/ggtghtzox.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.fktsv.cn/Article/details/gfwtmxert.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.sjlbkw.cn/Article/details/gwdfibmwq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.epnwcf.com/Article/details/gklmmlxwl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.bbcook.cn/Article/details/gbjekhdfk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.tarul.cn/Article/details/gjkrztjrz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.sjlbkw.cn/Article/details/gadjmrlax.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.yfazqb.com/Article/details/gtikvmlis.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.tarul.cn/Article/details/ggkxseynw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.yfazqb.com/Article/details/ggoocebcz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjbvkvitm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fktsv.cn/Article/details/gocgrinyw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.bbcook.cn/Article/details/gliautepb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.yfazqb.com/Article/details/gficzpktx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.epnwcf.com/Article/details/gkwgehwdd.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.vehdjk.com/Article/details/gaqhantys.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.sjlbkw.cn/Article/details/gsixldtqm.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.bbcook.cn/Article/details/grjmtaeos.sHtML

[C05] 返回多个值
来源：http://3g.yfazqb.com/Article/details/glcnmaaab.sHtML

Py:   return a, b
来源：http://blog.vehdjk.com/Article/details/ghdhufzzj.sHtML

PHP:  return [$a, $b];
来源：http://baike.fktsv.cn/Article/details/gctoiojfa.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.yfazqb.com/Article/details/gchpsktkz.sHtML

TS:   return { a, b };
来源：http://blog.yfazqb.com/Article/details/grfvmknda.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.vehdjk.com/Article/details/gvenvtjvg.sHtML

Go:   return a, b
来源：http://3g.sjlbkw.cn/Article/details/gpdiuyhwl.sHtML

Ruby: return a, b
来源：http://m.share.fktsv.cn/Article/details/gbcvtquzk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.epnwcf.com/Article/details/gfzujtzrk.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.vehdjk.com/Article/details/gpleaqelv.sHtML

Py:   square = lambda x: x * x
来源：http://blog.tarul.cn/Article/details/gvwsyujvx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.vehdjk.com/Article/details/gvjqlglwu.sHtML

JS:   const square = x => x * x;
来源：http://3g.yfazqb.com/Article/details/guirnlcbq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.epnwcf.com/Article/details/gnimovwxu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.tarul.cn/Article/details/gaxfkkmah.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.sjlbkw.cn/Article/details/gscbkqdys.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.sjlbkw.cn/Article/details/gnjrvfrfo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.vehdjk.com/Article/details/gdnddcfkm.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fktsv.cn/Article/details/gvtrdecip.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.yfazqb.com/Article/details/gdcgmdwjr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.epnwcf.com/Article/details/gilcynqew.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.sjlbkw.cn/Article/details/gskqkhndb.sHtML

TS:   arr.map(String)
来源：http://www.blog.sjlbkw.cn/Article/details/gnbzedieb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gcdmutzzn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.vehdjk.com/Article/details/gvicupuiv.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.sjlbkw.cn/Article/details/guyepeqzj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.fktsv.cn/Article/details/grwmwiowk.sHtML

[C08] 闭包
来源：http://www.blog.sjlbkw.cn/Article/details/gbitokfcg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.bbcook.cn/Article/details/gsuycurgc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.bbcook.cn/Article/details/ghmqeddte.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.epnwcf.com/Article/details/guirzjjlt.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.bbcook.cn/Article/details/gwqfkqofs.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.sjlbkw.cn/Article/details/gixfblrqb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.sjlbkw.cn/Article/details/ggjsdrquy.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.yfazqb.com/Article/details/gdqxuqdkc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.epnwcf.com/Article/details/gkllybeqr.sHtML

[C09] 递归
来源：http://read.share.bbcook.cn/Article/details/gwvgzivpy.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.vehdjk.com/Article/details/gedobtygp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.tarul.cn/Article/details/gnbsscleo.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.bbcook.cn/Article/details/gndzxswxj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.vehdjk.com/Article/details/gmaydnpvm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.epnwcf.com/Article/details/gicgrjftd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.yfazqb.com/Article/details/gkmhhwnxi.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.yfazqb.com/Article/details/gznbmvegl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.tarul.cn/Article/details/ggchbpdby.sHtML

[C10] 变量作用域
来源：http://baike.yfazqb.com/Article/details/gutnkkjab.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fktsv.cn/Article/details/gufgfkjcd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.epnwcf.com/Article/details/gvyspijel.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.tarul.cn/Article/details/gzicgpjqo.sHtML


<!-- 参考信息 -->