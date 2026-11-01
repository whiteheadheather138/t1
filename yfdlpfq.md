代发 wailian999

Ruby: a, b = b, a
来源：http://www.m.share.fktsv.cn/Article/details/gimfygwpc.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.tarul.cn/Article/details/geemzffgz.sHtML

[A20] 读取标准输入
来源：http://www.share.yfazqb.com/Article/details/gomcrtozx.sHtML

Py:   name = input("请输入：")
来源：http://m.share.epnwcf.com/Article/details/gmzuhfahj.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.bbcook.cn/Article/details/grxdbyryq.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.share.yfazqb.com/Article/details/gynhcwmhh.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.bbcook.cn/Article/details/gacatqfnm.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.epnwcf.com/Article/details/gggwcnxyj.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.yfazqb.com/Article/details/gisozavyv.sHtML

Ruby: gets.chomp
来源：http://wap.fktsv.cn/Article/details/gflzxlhcd.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.epnwcf.com/Article/details/gykmhinuq.sHtML

[A21] 保留指定小数位输出
来源：http://blog.fktsv.cn/Article/details/gnuvfjvaf.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.tarul.cn/Article/details/gqhoqlejn.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.bbcook.cn/Article/details/gmomdgchf.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.fktsv.cn/Article/details/gahufojvl.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.tarul.cn/Article/details/gcnoaeogk.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.epnwcf.com/Article/details/gzrskhmjp.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.tarul.cn/Article/details/gkgqmsotm.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.fktsv.cn/Article/details/goibiamkp.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.tarul.cn/Article/details/gzetxvamm.sHtML

[A22] 获取字符串长度
来源：http://read.share.vehdjk.com/Article/details/gboglpzaf.sHtML

Py:   len(s)
来源：http://baike.bbcook.cn/Article/details/gzjukyexq.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.bbcook.cn/Article/details/gorjfjepa.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.bbcook.cn/Article/details/gurazzzsw.sHtML

TS:   s.length
来源：http://wap.yfazqb.com/Article/details/gnppctnmp.sHtML

Java: s.length()
来源：http://3g.yfazqb.com/Article/details/gfcyixjyb.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.tarul.cn/Article/details/gnfonlvxd.sHtML

Ruby: s.length
来源：http://www.blog.tarul.cn/Article/details/gkitwcngj.sHtML

C#:   s.Length
来源：http://www.share.bbcook.cn/Article/details/ghdoojlzh.sHtML

[A23] 大小写转换
来源：http://wap.epnwcf.com/Article/details/gncraqwcg.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.epnwcf.com/Article/details/gaxylznjr.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.vehdjk.com/Article/details/gjkwgmlrs.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.epnwcf.com/Article/details/gueiqctcn.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.tarul.cn/Article/details/gsxqufrvi.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.sjlbkw.cn/Article/details/gmqlwmrug.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.vehdjk.com/Article/details/ggyzjrgiq.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.yfazqb.com/Article/details/grmjahrbn.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.bbcook.cn/Article/details/gcbbncesb.sHtML

[A24] 去除首尾空白
来源：http://read.share.bbcook.cn/Article/details/gstkcdluv.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.epnwcf.com/Article/details/gtxpxvele.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.bbcook.cn/Article/details/gcbjaherr.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.fktsv.cn/Article/details/gryrpfphd.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.epnwcf.com/Article/details/gbvhpwzfe.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.fktsv.cn/Article/details/gadgzsalv.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.yfazqb.com/Article/details/gumxxltkf.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.yfazqb.com/Article/details/gweyipqok.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.fktsv.cn/Article/details/gkxmlromt.sHtML

[A25] 字符串比较
来源：http://m.share.vehdjk.com/Article/details/gehskjqob.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.sjlbkw.cn/Article/details/ggiofoabz.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.sjlbkw.cn/Article/details/gnznldxqd.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.yfazqb.com/Article/details/givnxslak.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.bbcook.cn/Article/details/gymwjmxiq.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.yfazqb.com/Article/details/gtmtrqvbv.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.fktsv.cn/Article/details/gvylsfrfh.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.epnwcf.com/Article/details/gkegifbvo.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.epnwcf.com/Article/details/gqszswajp.sHtML

[A26] 类型转换总览
来源：http://wap.fktsv.cn/Article/details/gqnsuqtgw.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.yfazqb.com/Article/details/gyxzoluyg.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.yfazqb.com/Article/details/gktrzoiwh.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.bbcook.cn/Article/details/gjwojhkku.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.epnwcf.com/Article/details/gvltqguym.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.bbcook.cn/Article/details/grzggwoem.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.bbcook.cn/Article/details/gqbgffdud.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.tarul.cn/Article/details/gcultgqaa.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.fktsv.cn/Article/details/gmezkdqqf.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gquyqlqsb.sHtML

B. 流程控制
来源：http://m.share.tarul.cn/Article/details/gbzydkifp.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gmyfdqfdh.sHtML

[B01] 条件判断 if / else
来源：http://wap.tarul.cn/Article/details/gagrvsbve.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.fktsv.cn/Article/details/gdiqlbloy.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.epnwcf.com/Article/details/grcviogjd.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.epnwcf.com/Article/details/gybffhtee.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fktsv.cn/Article/details/gqyonfzaa.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.yfazqb.com/Article/details/gnxdfydfn.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.fktsv.cn/Article/details/gbhytnauv.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.bbcook.cn/Article/details/gdgourirs.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.fktsv.cn/Article/details/gjglksykl.sHtML

[B02] 多分支 else if / elif
来源：http://3g.vehdjk.com/Article/details/gkxpjefre.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.sjlbkw.cn/Article/details/ghlbosuni.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.fktsv.cn/Article/details/gnejbahez.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.epnwcf.com/Article/details/gnmtzvtxv.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.bbcook.cn/Article/details/gdieeckau.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.vehdjk.com/Article/details/gakfyeubu.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.epnwcf.com/Article/details/glhmvlnqw.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.vehdjk.com/Article/details/gwrvknhfd.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.epnwcf.com/Article/details/gexpxygwc.sHtML

[B03] switch / match / case
来源：http://blog.vehdjk.com/Article/details/gmexivigr.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.epnwcf.com/Article/details/glbbotbex.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.epnwcf.com/Article/details/gdacmokcx.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.yfazqb.com/Article/details/gixqojwkh.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.vehdjk.com/Article/details/gztripnel.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.sjlbkw.cn/Article/details/gfetmzgst.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.fktsv.cn/Article/details/gcmrkdwrh.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.vehdjk.com/Article/details/gejyxnsbm.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.tarul.cn/Article/details/gschxfhuv.sHtML

[B04] for 计数循环
来源：http://www.blog.yfazqb.com/Article/details/gmqqktgcg.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.yfazqb.com/Article/details/ggwkqqouw.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.bbcook.cn/Article/details/gmdwxjjxp.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.tarul.cn/Article/details/gpwhiplgi.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fktsv.cn/Article/details/gfnppajsp.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gepjatgvq.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.fktsv.cn/Article/details/ghlbmrerb.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.epnwcf.com/Article/details/geuwwiten.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.yfazqb.com/Article/details/gkyzirtwk.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.bbcook.cn/Article/details/gjhcrigea.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.vehdjk.com/Article/details/gnyjdrvvy.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.sjlbkw.cn/Article/details/glnvawpjw.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.tarul.cn/Article/details/gzihellwc.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.bbcook.cn/Article/details/gifflqilb.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.yfazqb.com/Article/details/gtmvbdnym.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.fktsv.cn/Article/details/gyoaexusi.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.bbcook.cn/Article/details/gcnmlmjnm.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.yfazqb.com/Article/details/gscyodlhy.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.sjlbkw.cn/Article/details/gopuxvtiu.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.tarul.cn/Article/details/gefphyaoe.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.sjlbkw.cn/Article/details/gykjnlgxy.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.bbcook.cn/Article/details/gbzzlqxii.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.bbcook.cn/Article/details/gtzlxaxev.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.fktsv.cn/Article/details/gzolypvbr.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.sjlbkw.cn/Article/details/gherrockw.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.yfazqb.com/Article/details/gitztmbbt.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.sjlbkw.cn/Article/details/gukbiergx.sHtML

[B07] while 循环
来源：http://www.blog.epnwcf.com/Article/details/gxsyadeyb.sHtML

Py:   while i < 10: i += 1
来源：http://wap.tarul.cn/Article/details/gqgxfqgjf.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.vehdjk.com/Article/details/gjbfqnzys.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.bbcook.cn/Article/details/gmlmbpeur.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.tarul.cn/Article/details/gqcezgxss.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.fktsv.cn/Article/details/gzukvupiv.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.bbcook.cn/Article/details/gncyrmfqz.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.yfazqb.com/Article/details/griloeuhx.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.fktsv.cn/Article/details/gtmhqzonf.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.bbcook.cn/Article/details/gieeklhwu.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.bbcook.cn/Article/details/gheyzzdye.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.yfazqb.com/Article/details/gtrthbkrm.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.fktsv.cn/Article/details/gxeaizjuh.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.vehdjk.com/Article/details/gcweibwqy.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.bbcook.cn/Article/details/gfiprwuea.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.tarul.cn/Article/details/gdtdjsplo.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.vehdjk.com/Article/details/gyoirztqm.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.vehdjk.com/Article/details/gufhufehh.sHtML

[B09] break 与 continue
来源：http://baike.sjlbkw.cn/Article/details/guktdbbml.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.sjlbkw.cn/Article/details/gqbecqgsl.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.sjlbkw.cn/Article/details/ggrqjegzm.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/gcanxukdv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.epnwcf.com/Article/details/gkramarvy.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fktsv.cn/Article/details/gewukcccq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.yfazqb.com/Article/details/gzartvhue.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.bbcook.cn/Article/details/glsnjfurl.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/goystmelr.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.tarul.cn/Article/details/gpmekeuhp.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.vehdjk.com/Article/details/gwsvxpijz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.yfazqb.com/Article/details/guebmmsvz.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.vehdjk.com/Article/details/gqzdchoax.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.epnwcf.com/Article/details/goetpccol.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.sjlbkw.cn/Article/details/gxvkudatu.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.fktsv.cn/Article/details/gucfbxfao.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.epnwcf.com/Article/details/gohtkufdu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.epnwcf.com/Article/details/gbmzlsooa.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.fktsv.cn/Article/details/gnnhsrhpi.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.tarul.cn/Article/details/gekytusnn.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.bbcook.cn/Article/details/ghartreeq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.tarul.cn/Article/details/gsvudhcmo.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.vehdjk.com/Article/details/gezmuhzrv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.epnwcf.com/Article/details/gwtlmftjm.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.tarul.cn/Article/details/gtlydiunh.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.sjlbkw.cn/Article/details/ghklpjcdn.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.vehdjk.com/Article/details/gefqiacrs.sHtML

[B12] 跳出多层循环
来源：http://m.share.bbcook.cn/Article/details/gjcymeklq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.sjlbkw.cn/Article/details/gomrvqqrh.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.yfazqb.com/Article/details/gwrkhbrpx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.epnwcf.com/Article/details/gonrnipnm.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.bbcook.cn/Article/details/giqebvwvt.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.sjlbkw.cn/Article/details/geqqkmplr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.bbcook.cn/Article/details/gasttooto.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.tarul.cn/Article/details/grtdlrafc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.vehdjk.com/Article/details/gqhqinoxj.sHtML

[B13] 判断是否为数字
来源：http://www.blog.vehdjk.com/Article/details/gdyselvuj.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.sjlbkw.cn/Article/details/ggxnftlhm.sHtML

PHP:  is_numeric($x)
来源：http://3g.vehdjk.com/Article/details/gsupyvleq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.vehdjk.com/Article/details/gfgqtggye.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.tarul.cn/Article/details/gipslsidz.sHtML

Java: x instanceof Number
来源：http://m.share.tarul.cn/Article/details/gyfthxdjm.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.yfazqb.com/Article/details/gujbdraqh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.tarul.cn/Article/details/glxenqfke.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.sjlbkw.cn/Article/details/gzyixandi.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.fktsv.cn/Article/details/gifbqpcmn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.sjlbkw.cn/Article/details/gxyfwvull.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.tarul.cn/Article/details/golgvwmtj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.sjlbkw.cn/Article/details/gzbuhkgpq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.fktsv.cn/Article/details/gfuwzkani.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.tarul.cn/Article/details/gsqzconlt.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.fktsv.cn/Article/details/gwpkwxxma.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fktsv.cn/Article/details/goihkinmg.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.sjlbkw.cn/Article/details/godceqoez.sHtML

[B15] 布尔运算与取反
来源：http://3g.epnwcf.com/Article/details/gahjglwgj.sHtML

Py:   a and b or not c
来源：http://read.share.epnwcf.com/Article/details/giitfwisp.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.fktsv.cn/Article/details/gorfqsmav.sHtML

JS:   a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gdubemshg.sHtML

TS:   a && b || !c
来源：http://www.share.epnwcf.com/Article/details/grskawpdj.sHtML

Java: a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gwnvdpynr.sHtML

Go:   a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/grnjosauf.sHtML

Ruby: a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/gmfanmvyw.sHtML

C#:   a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/gmgqcezue.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.epnwcf.com/Article/details/godojgjjk.sHtML

Py:   if not data: return
来源：http://read.share.fktsv.cn/Article/details/gcysygqvg.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.yfazqb.com/Article/details/ggfncwvaz.sHtML

JS:   if (!data) return;
来源：http://www.blog.vehdjk.com/Article/details/gbamqmldg.sHtML

TS:   if (!data) return;
来源：http://m.share.yfazqb.com/Article/details/gtlszpovr.sHtML

Java: if (data == null) return;
来源：http://www.share.bbcook.cn/Article/details/gokfksuyp.sHtML

Go:   if data == nil { return }
来源：http://blog.yfazqb.com/Article/details/ghmqjfplc.sHtML

Ruby: return if data.nil?
来源：http://mobile.fktsv.cn/Article/details/gmsvdmsiy.sHtML

C#:   if (data == null) return;
来源：http://blog.epnwcf.com/Article/details/goytxhxxq.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/ghkdjljmi.sHtML

C. 函数与作用域
来源：http://www.blog.sjlbkw.cn/Article/details/gtcgolbtq.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gunpexfmx.sHtML

[C01] 定义函数
来源：http://blog.epnwcf.com/Article/details/gtfvjxhri.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.fktsv.cn/Article/details/goxneiwoo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fktsv.cn/Article/details/gsjucnqnd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/gyotbzhbk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/ghyaikrco.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.tarul.cn/Article/details/gebpdutbw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.tarul.cn/Article/details/guoqkkyfx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.vehdjk.com/Article/details/gqcvubwix.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gfscltyzu.sHtML

[C02] 默认参数
来源：http://www.blog.fktsv.cn/Article/details/gtzyjhwso.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.sjlbkw.cn/Article/details/goxqpoldb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fktsv.cn/Article/details/gpmcqpwph.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.tarul.cn/Article/details/gndpwijys.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.bbcook.cn/Article/details/gkfcnjbyv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.bbcook.cn/Article/details/gzmjljded.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.tarul.cn/Article/details/gjhezodqu.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.tarul.cn/Article/details/geepeurbv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.vehdjk.com/Article/details/gpektjhju.sHtML

[C03] 可变参数
来源：http://www.m.share.bbcook.cn/Article/details/glrvqdvip.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.yfazqb.com/Article/details/gghpclaji.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fktsv.cn/Article/details/gupemppmd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fktsv.cn/Article/details/gkacfxhkh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.bbcook.cn/Article/details/gdhbcdvhp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fktsv.cn/Article/details/gelebmfgs.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.bbcook.cn/Article/details/gphimjkdq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.vehdjk.com/Article/details/gfmvmmcpi.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.tarul.cn/Article/details/gnpyjhfis.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.tarul.cn/Article/details/gxzukdadc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.tarul.cn/Article/details/gxingmpba.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fktsv.cn/Article/details/gmueqsppi.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.bbcook.cn/Article/details/gquvfsgie.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.sjlbkw.cn/Article/details/gniaspycy.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.yfazqb.com/Article/details/guhylfntm.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.tarul.cn/Article/details/gkkxwaovf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.tarul.cn/Article/details/gulruvszq.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fktsv.cn/Article/details/gixcpykiz.sHtML

[C05] 返回多个值
来源：http://www.m.share.bbcook.cn/Article/details/gemlgqwqt.sHtML

Py:   return a, b
来源：http://3g.yfazqb.com/Article/details/gazaaytnx.sHtML

PHP:  return [$a, $b];
来源：http://wap.bbcook.cn/Article/details/gsomqxcew.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.vehdjk.com/Article/details/gwlaqfstq.sHtML

TS:   return { a, b };
来源：http://baike.bbcook.cn/Article/details/ghkjsnkaz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.bbcook.cn/Article/details/gbxxrjhhg.sHtML

Go:   return a, b
来源：http://m.share.tarul.cn/Article/details/gvocxhkkc.sHtML

Ruby: return a, b
来源：http://baike.yfazqb.com/Article/details/gowdlfqqm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fktsv.cn/Article/details/grtlfefwz.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.bbcook.cn/Article/details/gatjlyylk.sHtML

Py:   square = lambda x: x * x
来源：http://blog.yfazqb.com/Article/details/glzpjgful.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.epnwcf.com/Article/details/gjwxglzao.sHtML

JS:   const square = x => x * x;
来源：http://baike.vehdjk.com/Article/details/ggtbatbff.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.bbcook.cn/Article/details/gxfpsjbmj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.bbcook.cn/Article/details/gfqbhwydn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.tarul.cn/Article/details/gylgngkgj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.sjlbkw.cn/Article/details/gzmsnwmgj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.vehdjk.com/Article/details/gooztvhrd.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.vehdjk.com/Article/details/goeyhiziz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.yfazqb.com/Article/details/gcvtfafox.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.epnwcf.com/Article/details/gmcxtjjwk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.sjlbkw.cn/Article/details/ghsfhvhms.sHtML

TS:   arr.map(String)
来源：http://www.blog.epnwcf.com/Article/details/gldtmhgug.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.sjlbkw.cn/Article/details/goojmzowc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.tarul.cn/Article/details/gvckutivj.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.tarul.cn/Article/details/gnccwcxxb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.vehdjk.com/Article/details/gpjlzxtyr.sHtML

[C08] 闭包
来源：http://read.share.fktsv.cn/Article/details/ghqdetozj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.bbcook.cn/Article/details/gzgrsixkr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.tarul.cn/Article/details/gbqrfmpnk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.bbcook.cn/Article/details/gxazrbfnt.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.sjlbkw.cn/Article/details/goyjxyimb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.vehdjk.com/Article/details/gixxscpwu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.epnwcf.com/Article/details/gizzoafov.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.tarul.cn/Article/details/gzuxdlrat.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.yfazqb.com/Article/details/gufnnkedf.sHtML

[C09] 递归
来源：http://read.share.sjlbkw.cn/Article/details/gajtxszgm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.vehdjk.com/Article/details/ghfzlhxoc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.sjlbkw.cn/Article/details/glrmkgotm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.sjlbkw.cn/Article/details/glacppxar.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.tarul.cn/Article/details/ghvqvgpyk.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.tarul.cn/Article/details/gzdrfbdhe.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.vehdjk.com/Article/details/gyttrwlrw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.yfazqb.com/Article/details/gsxqrsmhf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.tarul.cn/Article/details/gzyyqystj.sHtML

[C10] 变量作用域
来源：http://www.m.share.yfazqb.com/Article/details/gpfavkvvh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.sjlbkw.cn/Article/details/gqzxeygdg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.epnwcf.com/Article/details/ghrccipux.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.tarul.cn/Article/details/gfzqjxnbn.sHtML


<!-- 参考信息 -->