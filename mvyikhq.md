代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.sjlbkw.cn/Article/details/galqqvgup.sHtML

Ruby: gets.chomp
来源：http://wap.yfazqb.com/Article/details/gjnefoseh.sHtML

C#:   Console.ReadLine();
来源：http://3g.fktsv.cn/Article/details/gbvqhfgya.sHtML

[A21] 保留指定小数位输出
来源：http://baike.yfazqb.com/Article/details/gvijwbggh.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.epnwcf.com/Article/details/gvmrbyjjr.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.sjlbkw.cn/Article/details/gvcaotxkq.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.tarul.cn/Article/details/gourdsjfi.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.bbcook.cn/Article/details/gtahclevg.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.fktsv.cn/Article/details/ghoeezvmv.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.sjlbkw.cn/Article/details/grgzhifkj.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.fktsv.cn/Article/details/gkuekrtqt.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.fktsv.cn/Article/details/gnlbgngys.sHtML

[A22] 获取字符串长度
来源：http://blog.fktsv.cn/Article/details/gcldxosnl.sHtML

Py:   len(s)
来源：http://www.blog.bbcook.cn/Article/details/gomthhamk.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.bbcook.cn/Article/details/gywafnpcl.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.yfazqb.com/Article/details/gdmxbihlh.sHtML

TS:   s.length
来源：http://wap.yfazqb.com/Article/details/gwzuokcmd.sHtML

Java: s.length()
来源：http://www.share.bbcook.cn/Article/details/gtgxrsnad.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.vehdjk.com/Article/details/gstzucivd.sHtML

Ruby: s.length
来源：http://wap.bbcook.cn/Article/details/gjngmknst.sHtML

C#:   s.Length
来源：http://wap.vehdjk.com/Article/details/glljnuquh.sHtML

[A23] 大小写转换
来源：http://www.share.epnwcf.com/Article/details/gpxwygmer.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.yfazqb.com/Article/details/gvuscdvia.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.tarul.cn/Article/details/gkloajnen.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.bbcook.cn/Article/details/gulpxyimb.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.yfazqb.com/Article/details/gcdacjfty.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.tarul.cn/Article/details/gbdreemrx.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.epnwcf.com/Article/details/gigsxndlr.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.vehdjk.com/Article/details/gpzhismmw.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.epnwcf.com/Article/details/gwrnmnsmh.sHtML

[A24] 去除首尾空白
来源：http://blog.epnwcf.com/Article/details/gfwpdiwwe.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.fktsv.cn/Article/details/gqldyjvfv.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.epnwcf.com/Article/details/ghbuvgtqo.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.sjlbkw.cn/Article/details/gjbinejlg.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.epnwcf.com/Article/details/grjnhgrxr.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.fktsv.cn/Article/details/glfluzblc.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.sjlbkw.cn/Article/details/gjyzyehtv.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.tarul.cn/Article/details/gxorwilgb.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.tarul.cn/Article/details/gripimmtd.sHtML

[A25] 字符串比较
来源：http://www.blog.tarul.cn/Article/details/gtxwjasqx.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.yfazqb.com/Article/details/gvgbxgftu.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.bbcook.cn/Article/details/gzuvqbwfo.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.tarul.cn/Article/details/gjyvvzatz.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.tarul.cn/Article/details/godjamume.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.epnwcf.com/Article/details/gjnwpnabl.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.epnwcf.com/Article/details/gwmnwnfrg.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.yfazqb.com/Article/details/giiufnddi.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.yfazqb.com/Article/details/gseeuekjy.sHtML

[A26] 类型转换总览
来源：http://www.blog.fktsv.cn/Article/details/gnhvizhbv.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.bbcook.cn/Article/details/glbaoqfbb.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.tarul.cn/Article/details/gdqaudcfj.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.bbcook.cn/Article/details/guxssprzm.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.tarul.cn/Article/details/glbunlhma.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.epnwcf.com/Article/details/gkbbludtq.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.sjlbkw.cn/Article/details/gjmliqjvw.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.fktsv.cn/Article/details/gwwynzgpn.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.yfazqb.com/Article/details/gsyxakgar.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/ggtinqhxm.sHtML

B. 流程控制
来源：http://wap.sjlbkw.cn/Article/details/gkfpihhcu.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gzppcjvsg.sHtML

[B01] 条件判断 if / else
来源：http://read.share.fktsv.cn/Article/details/gwvbixmgh.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.tarul.cn/Article/details/gdzjkroou.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.fktsv.cn/Article/details/gucggotld.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.epnwcf.com/Article/details/gofhkxbay.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.epnwcf.com/Article/details/gatvpltbs.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.sjlbkw.cn/Article/details/gadxvlzsr.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.epnwcf.com/Article/details/gdvtdipfj.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.sjlbkw.cn/Article/details/gduupoyhh.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.vehdjk.com/Article/details/gnlkxbuim.sHtML

[B02] 多分支 else if / elif
来源：http://blog.vehdjk.com/Article/details/ggvftqnko.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.fktsv.cn/Article/details/gdsashadu.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.vehdjk.com/Article/details/gbmxflcuo.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.yfazqb.com/Article/details/ggjjlecwl.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.bbcook.cn/Article/details/gpqyigkta.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.epnwcf.com/Article/details/gvnoqojtk.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.vehdjk.com/Article/details/giqvqkvos.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.sjlbkw.cn/Article/details/gdabweucq.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fktsv.cn/Article/details/ghdhisirv.sHtML

[B03] switch / match / case
来源：http://www.share.vehdjk.com/Article/details/gltutllji.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.bbcook.cn/Article/details/gqpdljpsm.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.vehdjk.com/Article/details/gfxbsnoav.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.sjlbkw.cn/Article/details/gpburqese.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fktsv.cn/Article/details/gqfgovroe.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.fktsv.cn/Article/details/gnptxdpas.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.yfazqb.com/Article/details/guwfvrwlj.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.tarul.cn/Article/details/gvqanxtzu.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.vehdjk.com/Article/details/glaueukks.sHtML

[B04] for 计数循环
来源：http://wap.bbcook.cn/Article/details/gskwivjai.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.tarul.cn/Article/details/gpglylnih.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.yfazqb.com/Article/details/gvtgrcbmq.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.yfazqb.com/Article/details/gaygjahpw.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.bbcook.cn/Article/details/gybkqfiif.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.epnwcf.com/Article/details/gbxripvkm.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.bbcook.cn/Article/details/gznjlfmiy.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.epnwcf.com/Article/details/gtxmncwex.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.tarul.cn/Article/details/gvnlkqpxu.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.vehdjk.com/Article/details/gbesyopjb.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.tarul.cn/Article/details/glfuysptv.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.sjlbkw.cn/Article/details/gcbzsywfq.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.tarul.cn/Article/details/gbjgepslq.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.tarul.cn/Article/details/gogucwmxs.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.fktsv.cn/Article/details/gphleshtm.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.sjlbkw.cn/Article/details/gswucalpk.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.vehdjk.com/Article/details/ghepgniqj.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.tarul.cn/Article/details/gdokniytb.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.epnwcf.com/Article/details/ggfqimldb.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.vehdjk.com/Article/details/gccrubgjg.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.epnwcf.com/Article/details/glqwxzpaa.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fktsv.cn/Article/details/gzdfdwqlu.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.yfazqb.com/Article/details/gszynhgph.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.bbcook.cn/Article/details/gyjbppwll.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.epnwcf.com/Article/details/gyjykrmuz.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.sjlbkw.cn/Article/details/gltnyedmz.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.sjlbkw.cn/Article/details/gmykdqkwj.sHtML

[B07] while 循环
来源：http://www.share.bbcook.cn/Article/details/gfxqxlgjh.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.bbcook.cn/Article/details/ggebbeojm.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.sjlbkw.cn/Article/details/gjbqaawva.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.tarul.cn/Article/details/gnjkddiqv.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.tarul.cn/Article/details/gdvirisrv.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.sjlbkw.cn/Article/details/gtxirpocj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.sjlbkw.cn/Article/details/gnjmvnjum.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.sjlbkw.cn/Article/details/gizklomlh.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.vehdjk.com/Article/details/gndzaesxd.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.fktsv.cn/Article/details/giunkqfvk.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.epnwcf.com/Article/details/gftzdbisq.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.epnwcf.com/Article/details/gfildabjs.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.fktsv.cn/Article/details/gpndvqdlf.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.sjlbkw.cn/Article/details/gepcepjja.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.sjlbkw.cn/Article/details/gpixeebkl.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.sjlbkw.cn/Article/details/gjkoipirp.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgsqlqrx.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.sjlbkw.cn/Article/details/gqunbqtmm.sHtML

[B09] break 与 continue
来源：http://m.share.bbcook.cn/Article/details/gxncrnoav.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gkqzwtemh.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.fktsv.cn/Article/details/gecjcejny.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.tarul.cn/Article/details/gnidezqmt.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.yfazqb.com/Article/details/gctihphqw.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fktsv.cn/Article/details/grxgcvltv.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.sjlbkw.cn/Article/details/glryctqhk.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.fktsv.cn/Article/details/gmejrcdad.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.vehdjk.com/Article/details/glbqnlwvb.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.fktsv.cn/Article/details/gmtzwetqa.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.epnwcf.com/Article/details/gjmyjtann.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.tarul.cn/Article/details/gmqotulmr.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.epnwcf.com/Article/details/ggjyskfxo.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fktsv.cn/Article/details/gjmkqzyit.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.fktsv.cn/Article/details/gwdymtdaq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fktsv.cn/Article/details/gowitqyyl.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.bbcook.cn/Article/details/gvavsakju.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.epnwcf.com/Article/details/gqrezkyff.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.epnwcf.com/Article/details/grkwcwofl.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.fktsv.cn/Article/details/gmtoudpar.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.sjlbkw.cn/Article/details/gmtejpknb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.bbcook.cn/Article/details/gwgduiyeh.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.yfazqb.com/Article/details/gwybxcnhq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.fktsv.cn/Article/details/gyrfqnlkt.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.yfazqb.com/Article/details/ggaygjpkr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.fktsv.cn/Article/details/grhoxkptn.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.vehdjk.com/Article/details/gqelcnknm.sHtML

[B12] 跳出多层循环
来源：http://mobile.fktsv.cn/Article/details/gkmotuxih.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.yfazqb.com/Article/details/grzdriadl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.vehdjk.com/Article/details/gihyphsgd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.vehdjk.com/Article/details/gnqrrljpc.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.epnwcf.com/Article/details/gxsmpussh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.sjlbkw.cn/Article/details/gjkmmqvnd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.sjlbkw.cn/Article/details/gcryvkirv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.vehdjk.com/Article/details/gvkymkqqq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fktsv.cn/Article/details/gnmgrqbwb.sHtML

[B13] 判断是否为数字
来源：http://baike.bbcook.cn/Article/details/gwsltutzl.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.vehdjk.com/Article/details/gdecvtrbd.sHtML

PHP:  is_numeric($x)
来源：http://blog.vehdjk.com/Article/details/gqjykzzkn.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.epnwcf.com/Article/details/gxsppboeg.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fktsv.cn/Article/details/grgflkxeq.sHtML

Java: x instanceof Number
来源：http://www.share.bbcook.cn/Article/details/gcdjlbkex.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.vehdjk.com/Article/details/gpdhkdndv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.tarul.cn/Article/details/gcqscfcta.sHtML

C#:   x is int or double or decimal
来源：http://blog.yfazqb.com/Article/details/gzovcilen.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.vehdjk.com/Article/details/gamfsuwlk.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.sjlbkw.cn/Article/details/gxmwrnzyj.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fktsv.cn/Article/details/gnrbavoaw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.vehdjk.com/Article/details/gnsfowwrx.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.fktsv.cn/Article/details/glkshehgu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.bbcook.cn/Article/details/gthqdtchi.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.sjlbkw.cn/Article/details/giowbbmff.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.bbcook.cn/Article/details/geodvcktr.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.sjlbkw.cn/Article/details/gsfmixpfn.sHtML

[B15] 布尔运算与取反
来源：http://wap.vehdjk.com/Article/details/gneskdmey.sHtML

Py:   a and b or not c
来源：http://read.share.bbcook.cn/Article/details/gknsciluo.sHtML

PHP:  $a && $b || !$c
来源：http://baike.epnwcf.com/Article/details/gmcwmkpsh.sHtML

JS:   a && b || !c
来源：http://read.share.vehdjk.com/Article/details/goricyqah.sHtML

TS:   a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gllqieasf.sHtML

Java: a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gfmftlwxf.sHtML

Go:   a && b || !c
来源：http://m.share.fktsv.cn/Article/details/gaykhangq.sHtML

Ruby: a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gcdxvdcpw.sHtML

C#:   a && b || !c
来源：http://www.blog.tarul.cn/Article/details/giczrexkb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.bbcook.cn/Article/details/grxzceoxt.sHtML

Py:   if not data: return
来源：http://www.share.bbcook.cn/Article/details/gfwxjyzrv.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.vehdjk.com/Article/details/gknqmtgzu.sHtML

JS:   if (!data) return;
来源：http://blog.bbcook.cn/Article/details/gnvrvsmix.sHtML

TS:   if (!data) return;
来源：http://m.share.epnwcf.com/Article/details/gsddbmmed.sHtML

Java: if (data == null) return;
来源：http://read.share.sjlbkw.cn/Article/details/gwcyfczye.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.epnwcf.com/Article/details/gapermpgg.sHtML

Ruby: return if data.nil?
来源：http://baike.yfazqb.com/Article/details/gztbipeyb.sHtML

C#:   if (data == null) return;
来源：http://wap.bbcook.cn/Article/details/gzwmbqvbu.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gfeddmwtx.sHtML

C. 函数与作用域
来源：http://blog.yfazqb.com/Article/details/gpesmzmmn.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gpfahubfr.sHtML

[C01] 定义函数
来源：http://baike.yfazqb.com/Article/details/gembeeirp.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.sjlbkw.cn/Article/details/gtayfqpoa.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fktsv.cn/Article/details/gpktfpdww.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/gkhpjeplc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/grqmnsqsk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/gzcbnbirl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fktsv.cn/Article/details/gvbmbvxvj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.yfazqb.com/Article/details/gaibtkbdv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gxyqsaqut.sHtML

[C02] 默认参数
来源：http://mobile.yfazqb.com/Article/details/gchnhuhgp.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.yfazqb.com/Article/details/gdmxetckr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.yfazqb.com/Article/details/gapjmuxkg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.yfazqb.com/Article/details/gghlanzir.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gezdzfazr.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.epnwcf.com/Article/details/gplvnlmrv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.epnwcf.com/Article/details/gvooxhxuh.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fktsv.cn/Article/details/ghapcofsq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.vehdjk.com/Article/details/ghggruuyc.sHtML

[C03] 可变参数
来源：http://3g.vehdjk.com/Article/details/gaijvfndf.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.yfazqb.com/Article/details/gkwjuhptq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.bbcook.cn/Article/details/gkavqfuvs.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.tarul.cn/Article/details/gwnipgumd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.vehdjk.com/Article/details/geynmfxii.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.epnwcf.com/Article/details/gfnsckkad.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.vehdjk.com/Article/details/gkqqufjfx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fktsv.cn/Article/details/gqvjwrugk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.vehdjk.com/Article/details/gzfeednxh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.yfazqb.com/Article/details/gzmsyeszk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.tarul.cn/Article/details/gkyeehlno.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.epnwcf.com/Article/details/gqjhyihzb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.yfazqb.com/Article/details/grofhanqb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fktsv.cn/Article/details/gunfttpdo.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.yfazqb.com/Article/details/gosulyjua.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.sjlbkw.cn/Article/details/gquwhkfni.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.bbcook.cn/Article/details/gojkhfiwg.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.tarul.cn/Article/details/ggklbhaps.sHtML

[C05] 返回多个值
来源：http://blog.bbcook.cn/Article/details/gexqxjkuz.sHtML

Py:   return a, b
来源：http://read.share.epnwcf.com/Article/details/gdfaymdki.sHtML

PHP:  return [$a, $b];
来源：http://wap.sjlbkw.cn/Article/details/gjhzhrzge.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fktsv.cn/Article/details/gxryxqwoj.sHtML

TS:   return { a, b };
来源：http://www.share.vehdjk.com/Article/details/gpwiskjre.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.vehdjk.com/Article/details/gqkttgfuj.sHtML

Go:   return a, b
来源：http://www.share.epnwcf.com/Article/details/gjwwosqfh.sHtML

Ruby: return a, b
来源：http://www.share.vehdjk.com/Article/details/gamowdbur.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.vehdjk.com/Article/details/gqjxjddmn.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.sjlbkw.cn/Article/details/gqaysdcii.sHtML

Py:   square = lambda x: x * x
来源：http://wap.epnwcf.com/Article/details/gqlaazjyr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.epnwcf.com/Article/details/gqliwsjhb.sHtML

JS:   const square = x => x * x;
来源：http://www.share.vehdjk.com/Article/details/giwbsllsz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.yfazqb.com/Article/details/gxdrpnwbj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.bbcook.cn/Article/details/gwvccvcxc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.sjlbkw.cn/Article/details/gbdaelggg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.tarul.cn/Article/details/gtvqjrgco.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.vehdjk.com/Article/details/gkhvjivmj.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fktsv.cn/Article/details/gwdoxdqli.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.vehdjk.com/Article/details/gxskpdido.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.sjlbkw.cn/Article/details/gffgdhcmp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.tarul.cn/Article/details/gnjnuejld.sHtML

TS:   arr.map(String)
来源：http://read.share.vehdjk.com/Article/details/gjrutdynw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.bbcook.cn/Article/details/gbuvjzwiq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.yfazqb.com/Article/details/gncszlxuj.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzqnnijrm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.tarul.cn/Article/details/gisznvujm.sHtML

[C08] 闭包
来源：http://www.m.share.epnwcf.com/Article/details/giespvdgu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.bbcook.cn/Article/details/gyunkngub.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.sjlbkw.cn/Article/details/gyaffooai.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.sjlbkw.cn/Article/details/gwnvlourl.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmcusryzg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.epnwcf.com/Article/details/grfvspqba.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.yfazqb.com/Article/details/gcmkqrzmj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.bbcook.cn/Article/details/gxcoyclmd.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.yfazqb.com/Article/details/gxvlaibzw.sHtML

[C09] 递归
来源：http://baike.yfazqb.com/Article/details/ghqkvoedi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.yfazqb.com/Article/details/gqgikyakr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.epnwcf.com/Article/details/gjonoaprl.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.sjlbkw.cn/Article/details/gccdfkxzs.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.sjlbkw.cn/Article/details/gdoewcwgs.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.yfazqb.com/Article/details/gpajnhwkx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.vehdjk.com/Article/details/gjskrzivx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fktsv.cn/Article/details/gaabllmlr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.epnwcf.com/Article/details/gpzrodzbe.sHtML

[C10] 变量作用域
来源：http://baike.bbcook.cn/Article/details/gyoezaawb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.yfazqb.com/Article/details/gtgbhkxih.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.tarul.cn/Article/details/ggyvnwfst.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.yfazqb.com/Article/details/gbwyxnhlg.sHtML

TS:   同 JS
来源：http://mobile.fktsv.cn/Article/details/gsovbcxmt.sHtML

Java: 方法内为块级作用域
来源：http://m.share.vehdjk.com/Article/details/ghefnadqd.sHtML

Go:   花括号块级作用域
来源：http://3g.sjlbkw.cn/Article/details/gfpinjwqh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.sjlbkw.cn/Article/details/gcxksdiga.sHtML

C#:   块级作用域
来源：http://wap.sjlbkw.cn/Article/details/gnqfubeyr.sHtML

[C11] 模块导入与导出
来源：http://wap.bbcook.cn/Article/details/gmdmlygvb.sHtML

Py:   from module import func
来源：http://3g.epnwcf.com/Article/details/gymuxsjsg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.vehdjk.com/Article/details/gzhyvgckq.sHtML


<!-- 参考信息 -->