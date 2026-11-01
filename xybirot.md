代发 wailian999

JS:   [a, b] = [b, a];
来源：http://www.blog.bbcook.cn/Article/details/gcuabhcbq.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.sjlbkw.cn/Article/details/gwvmckkvi.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.vehdjk.com/Article/details/gkccuhqjz.sHtML

Go:   a, b = b, a
来源：http://www.m.share.tarul.cn/Article/details/gtwitgihq.sHtML

Ruby: a, b = b, a
来源：http://blog.tarul.cn/Article/details/ggpjemiwv.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.bbcook.cn/Article/details/gwtqvkmxy.sHtML

[A20] 读取标准输入
来源：http://blog.vehdjk.com/Article/details/gybnhnndr.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.yfazqb.com/Article/details/gemyjjidj.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.epnwcf.com/Article/details/glvrwdtjb.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.yfazqb.com/Article/details/gyashbxtv.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.tarul.cn/Article/details/gvtuprxgl.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.bbcook.cn/Article/details/ghckprcaq.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.vehdjk.com/Article/details/gcmrmsegq.sHtML

Ruby: gets.chomp
来源：http://wap.epnwcf.com/Article/details/gobmgzgsv.sHtML

C#:   Console.ReadLine();
来源：http://blog.yfazqb.com/Article/details/gtlauooqg.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.vehdjk.com/Article/details/gxndemqpw.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.sjlbkw.cn/Article/details/guiwkewye.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.vehdjk.com/Article/details/gevjudvtl.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.vehdjk.com/Article/details/gbnlgnkqe.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.epnwcf.com/Article/details/gmjjdupgq.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.sjlbkw.cn/Article/details/gyzkvwvxb.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.vehdjk.com/Article/details/gvsstyoto.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.tarul.cn/Article/details/gjelhikow.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.vehdjk.com/Article/details/gbvxxeydv.sHtML

[A22] 获取字符串长度
来源：http://m.share.vehdjk.com/Article/details/ggaeolrsx.sHtML

Py:   len(s)
来源：http://www.blog.vehdjk.com/Article/details/gloqskrrz.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.yfazqb.com/Article/details/gzwpambpq.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.tarul.cn/Article/details/gicosmhyq.sHtML

TS:   s.length
来源：http://www.blog.sjlbkw.cn/Article/details/gttrtrnvh.sHtML

Java: s.length()
来源：http://www.share.fktsv.cn/Article/details/grhflgmed.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.fktsv.cn/Article/details/gjskthqwe.sHtML

Ruby: s.length
来源：http://wap.vehdjk.com/Article/details/gqxbrwolp.sHtML

C#:   s.Length
来源：http://wap.sjlbkw.cn/Article/details/gqswbmcwi.sHtML

[A23] 大小写转换
来源：http://m.share.vehdjk.com/Article/details/gyqqypuxa.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.yfazqb.com/Article/details/gmaxiahzm.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.epnwcf.com/Article/details/gcgrraesq.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fktsv.cn/Article/details/glhjsoyrh.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.vehdjk.com/Article/details/ghdnrzych.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.vehdjk.com/Article/details/gentbnbkg.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.vehdjk.com/Article/details/gctfqmmwp.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.tarul.cn/Article/details/grpjwcwtj.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.fktsv.cn/Article/details/gltywobzz.sHtML

[A24] 去除首尾空白
来源：http://www.blog.tarul.cn/Article/details/gksgbbnqw.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.fktsv.cn/Article/details/gcznnicrr.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.epnwcf.com/Article/details/gvonqjpck.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.vehdjk.com/Article/details/gjpiayvkq.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.tarul.cn/Article/details/gpyjjgouk.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.vehdjk.com/Article/details/gxigimsaa.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.fktsv.cn/Article/details/gnprdmugo.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.epnwcf.com/Article/details/gqjuarmue.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.epnwcf.com/Article/details/ghzfgknev.sHtML

[A25] 字符串比较
来源：http://3g.sjlbkw.cn/Article/details/gohdrwels.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.fktsv.cn/Article/details/gjjqkaprs.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.fktsv.cn/Article/details/ghqevzswp.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fktsv.cn/Article/details/gzvlpftpr.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fktsv.cn/Article/details/goksbauqr.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.vehdjk.com/Article/details/gkmrhxrdj.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.sjlbkw.cn/Article/details/gcqxgfjnz.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.fktsv.cn/Article/details/gslfycvhr.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.fktsv.cn/Article/details/glqjntmwl.sHtML

[A26] 类型转换总览
来源：http://blog.vehdjk.com/Article/details/gkjhtqmni.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.fktsv.cn/Article/details/goacxmtql.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.yfazqb.com/Article/details/grkywsmvb.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.epnwcf.com/Article/details/giioxorux.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.vehdjk.com/Article/details/gfvwwjxjc.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.sjlbkw.cn/Article/details/guocwnedv.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.yfazqb.com/Article/details/gzewmanos.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.yfazqb.com/Article/details/gwwyaegog.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.yfazqb.com/Article/details/gzeapyzod.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/geneyhjve.sHtML

B. 流程控制
来源：http://www.m.share.vehdjk.com/Article/details/gyhybfdtj.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gemfntjxu.sHtML

[B01] 条件判断 if / else
来源：http://wap.yfazqb.com/Article/details/gcnsnrtug.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.sjlbkw.cn/Article/details/gdcskddpf.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.epnwcf.com/Article/details/gydwjmemd.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.fktsv.cn/Article/details/gtkhamthl.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.tarul.cn/Article/details/gbdytbnmb.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.sjlbkw.cn/Article/details/gvoooouyg.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.fktsv.cn/Article/details/gqzyrxkaf.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.yfazqb.com/Article/details/gtkzwiaeh.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.yfazqb.com/Article/details/ghrkldoal.sHtML

[B02] 多分支 else if / elif
来源：http://blog.epnwcf.com/Article/details/ghhdmawal.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.sjlbkw.cn/Article/details/gqgapxvpk.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.sjlbkw.cn/Article/details/gtkxrjohe.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.vehdjk.com/Article/details/gjstakbck.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.vehdjk.com/Article/details/gjoojixtr.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.sjlbkw.cn/Article/details/gpdzizosx.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.fktsv.cn/Article/details/gjawujjqc.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.sjlbkw.cn/Article/details/gpersmedh.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.sjlbkw.cn/Article/details/gabrllxhd.sHtML

[B03] switch / match / case
来源：http://read.share.yfazqb.com/Article/details/gkqtqfgke.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.fktsv.cn/Article/details/gzigxlpzt.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.bbcook.cn/Article/details/gbgxcovvr.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.bbcook.cn/Article/details/gomabkddd.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.bbcook.cn/Article/details/guzblytdw.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.tarul.cn/Article/details/gxenupjki.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.epnwcf.com/Article/details/gkrlwxqbx.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.sjlbkw.cn/Article/details/gfxmqajvi.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.bbcook.cn/Article/details/gbhrqrifb.sHtML

[B04] for 计数循环
来源：http://read.share.vehdjk.com/Article/details/gbtdwzwcj.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.fktsv.cn/Article/details/gbykfekng.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.fktsv.cn/Article/details/gonziochs.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gieubbflo.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.sjlbkw.cn/Article/details/ghtajxwzc.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.epnwcf.com/Article/details/gkvzltdgy.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.yfazqb.com/Article/details/gntrwxwhy.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.tarul.cn/Article/details/gyymeazqk.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.fktsv.cn/Article/details/ghvjokiek.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.vehdjk.com/Article/details/gqulwamxf.sHtML

Py:   for item in arr: print(item)
来源：http://baike.sjlbkw.cn/Article/details/gjmfwekbs.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.vehdjk.com/Article/details/gonxvkinw.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.vehdjk.com/Article/details/gtmgqmxky.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.yfazqb.com/Article/details/gqvewiizo.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.vehdjk.com/Article/details/gqjankgxx.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.tarul.cn/Article/details/ggqnhxkhp.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.sjlbkw.cn/Article/details/gmghjyglx.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.tarul.cn/Article/details/gbhoywqgh.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.bbcook.cn/Article/details/gxdokusfv.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.sjlbkw.cn/Article/details/ghbwtxxri.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.epnwcf.com/Article/details/geamoxbwy.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.bbcook.cn/Article/details/gudlflmfa.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.sjlbkw.cn/Article/details/gkrlaqnwv.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.sjlbkw.cn/Article/details/glgespgpp.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.sjlbkw.cn/Article/details/ggypyhmvt.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.vehdjk.com/Article/details/glvidtgvv.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.sjlbkw.cn/Article/details/gmwjglxbt.sHtML

[B07] while 循环
来源：http://www.share.tarul.cn/Article/details/gawcuxjgq.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.yfazqb.com/Article/details/gnbsnccgx.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.fktsv.cn/Article/details/glbfhcwpc.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.tarul.cn/Article/details/gesjlulqd.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.tarul.cn/Article/details/gzfngsaxe.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.epnwcf.com/Article/details/gdwfsehuo.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.epnwcf.com/Article/details/gvraopzmf.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.vehdjk.com/Article/details/ghatmeanj.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.sjlbkw.cn/Article/details/gxzqzhzej.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.tarul.cn/Article/details/gvntfckbq.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.fktsv.cn/Article/details/gznpyedjg.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.epnwcf.com/Article/details/gqbgtwrez.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.yfazqb.com/Article/details/gxpzrxewx.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.vehdjk.com/Article/details/gnqggyctf.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.epnwcf.com/Article/details/gwyavugqq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.tarul.cn/Article/details/gidnxgbvf.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.bbcook.cn/Article/details/ghyvfrmru.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.fktsv.cn/Article/details/gpfqnuuag.sHtML

[B09] break 与 continue
来源：http://www.m.share.bbcook.cn/Article/details/gmwpxnhhk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.bbcook.cn/Article/details/gyoacvayq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.fktsv.cn/Article/details/gnhhjnbgj.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/gvscxhrbv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.yfazqb.com/Article/details/gsucyexqo.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fktsv.cn/Article/details/gmgwefehz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.fktsv.cn/Article/details/gyoovzpdw.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.sjlbkw.cn/Article/details/gfotzinsa.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.tarul.cn/Article/details/gzsfnwnqw.sHtML

[B10] 遍历同时拿索引
来源：http://baike.yfazqb.com/Article/details/gfjnuthit.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.fktsv.cn/Article/details/gcqlddlnu.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.bbcook.cn/Article/details/gcsxvbcbk.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.epnwcf.com/Article/details/gkpvdtujy.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.vehdjk.com/Article/details/ghmoutmbf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.tarul.cn/Article/details/gwxfhyjja.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.bbcook.cn/Article/details/gfkdnuteb.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.epnwcf.com/Article/details/glhgpsxds.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.vehdjk.com/Article/details/gqzfxeguq.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.bbcook.cn/Article/details/govptbjhr.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.vehdjk.com/Article/details/gsnexuobe.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.yfazqb.com/Article/details/gwjfhbvsz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.tarul.cn/Article/details/gopciryyv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fktsv.cn/Article/details/ggfepoeqh.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gekyvvzri.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.bbcook.cn/Article/details/gqwgkzqqy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.tarul.cn/Article/details/gwqnocmkg.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.yfazqb.com/Article/details/gaqdrmjxa.sHtML

[B12] 跳出多层循环
来源：http://mobile.tarul.cn/Article/details/gydksdqgs.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.tarul.cn/Article/details/gebfqdvrc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.tarul.cn/Article/details/gcgodebyp.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fktsv.cn/Article/details/gdzcwmshs.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.epnwcf.com/Article/details/gxqaqbldw.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.yfazqb.com/Article/details/gognzdnju.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.epnwcf.com/Article/details/gvjcicsgs.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.tarul.cn/Article/details/gtdxjsdpk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.tarul.cn/Article/details/gxotfooau.sHtML

[B13] 判断是否为数字
来源：http://www.blog.fktsv.cn/Article/details/ghkqjdvfu.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.yfazqb.com/Article/details/gqprbfulk.sHtML

PHP:  is_numeric($x)
来源：http://www.share.yfazqb.com/Article/details/gbwakhhiy.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.vehdjk.com/Article/details/gajlwegjq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.yfazqb.com/Article/details/gnfoaxbcc.sHtML

Java: x instanceof Number
来源：http://baike.sjlbkw.cn/Article/details/gbgmblfif.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.sjlbkw.cn/Article/details/gjyurfmui.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.epnwcf.com/Article/details/gazkcsqez.sHtML

C#:   x is int or double or decimal
来源：http://blog.fktsv.cn/Article/details/gczikxvhv.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.fktsv.cn/Article/details/guyvnrzci.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.epnwcf.com/Article/details/gmnqoirrm.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.sjlbkw.cn/Article/details/gsfdknxpv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.bbcook.cn/Article/details/gmglhcsbd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.fktsv.cn/Article/details/ggqxmwxqr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.yfazqb.com/Article/details/gqrtzjgqi.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.tarul.cn/Article/details/gvcsnbony.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.epnwcf.com/Article/details/gvluxclme.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.tarul.cn/Article/details/grciucvdu.sHtML

[B15] 布尔运算与取反
来源：http://3g.sjlbkw.cn/Article/details/grhtufyse.sHtML

Py:   a and b or not c
来源：http://www.m.share.epnwcf.com/Article/details/gifklgmtj.sHtML

PHP:  $a && $b || !$c
来源：http://wap.bbcook.cn/Article/details/gzrfqlxxh.sHtML

JS:   a && b || !c
来源：http://mobile.fktsv.cn/Article/details/gpiyovzyw.sHtML

TS:   a && b || !c
来源：http://m.share.tarul.cn/Article/details/gzlqugppi.sHtML

Java: a && b || !c
来源：http://www.share.tarul.cn/Article/details/gvqujrqkh.sHtML

Go:   a && b || !c
来源：http://mobile.epnwcf.com/Article/details/guhowcyvt.sHtML

Ruby: a && b || !c
来源：http://mobile.vehdjk.com/Article/details/gudnccanc.sHtML

C#:   a && b || !c
来源：http://mobile.epnwcf.com/Article/details/gzcucrotl.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.fktsv.cn/Article/details/gbapprifo.sHtML

Py:   if not data: return
来源：http://read.share.sjlbkw.cn/Article/details/gvcugrjty.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.yfazqb.com/Article/details/gxpdobgww.sHtML

JS:   if (!data) return;
来源：http://baike.epnwcf.com/Article/details/gkfeavwrm.sHtML

TS:   if (!data) return;
来源：http://www.share.vehdjk.com/Article/details/giomlmoez.sHtML

Java: if (data == null) return;
来源：http://www.m.share.tarul.cn/Article/details/gqhifoarw.sHtML

Go:   if data == nil { return }
来源：http://3g.fktsv.cn/Article/details/gvtohbmjd.sHtML

Ruby: return if data.nil?
来源：http://read.share.vehdjk.com/Article/details/gosncdsbm.sHtML

C#:   if (data == null) return;
来源：http://blog.bbcook.cn/Article/details/gjhrtxtdu.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gnnhijevs.sHtML

C. 函数与作用域
来源：http://read.share.fktsv.cn/Article/details/grfjlkobz.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gfctpmpvk.sHtML

[C01] 定义函数
来源：http://www.share.tarul.cn/Article/details/gtrmvgqzx.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.bbcook.cn/Article/details/gzesujzyu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.epnwcf.com/Article/details/guvyebcxg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/gmdceowat.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.epnwcf.com/Article/details/gnlaumxta.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/grknvivpw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.vehdjk.com/Article/details/giskqjfbc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.vehdjk.com/Article/details/gfsqkgqri.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gzexezlat.sHtML

[C02] 默认参数
来源：http://3g.vehdjk.com/Article/details/glewtohkj.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.yfazqb.com/Article/details/gxgnhizgh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fktsv.cn/Article/details/gespimtlr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.yfazqb.com/Article/details/goyvzdrmf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.yfazqb.com/Article/details/giiyhbstg.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fktsv.cn/Article/details/gzxhsgpgd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.yfazqb.com/Article/details/grdngckax.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.vehdjk.com/Article/details/ghjxptxmr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.yfazqb.com/Article/details/gzrtgbiis.sHtML

[C03] 可变参数
来源：http://wap.bbcook.cn/Article/details/gyqmvfuve.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.bbcook.cn/Article/details/gehohwycq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fktsv.cn/Article/details/gjioapxob.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.vehdjk.com/Article/details/gxeuptjag.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.vehdjk.com/Article/details/gpcdcydtn.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.yfazqb.com/Article/details/gcmrextqd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.fktsv.cn/Article/details/gwubagtyo.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.sjlbkw.cn/Article/details/gnirxcdqf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fktsv.cn/Article/details/gwubpdikm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.bbcook.cn/Article/details/gfjlxqbcl.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.tarul.cn/Article/details/gqdpdvfzn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fktsv.cn/Article/details/gxuofhlsr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.bbcook.cn/Article/details/gpnlbuipy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.yfazqb.com/Article/details/gvatgbqri.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.yfazqb.com/Article/details/gzoriigsu.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.bbcook.cn/Article/details/guctyickh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fktsv.cn/Article/details/gcaidsxxj.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.yfazqb.com/Article/details/gwicarnpg.sHtML

[C05] 返回多个值
来源：http://m.share.sjlbkw.cn/Article/details/gnhjmvyzf.sHtML

Py:   return a, b
来源：http://baike.bbcook.cn/Article/details/gusvnrbzf.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.epnwcf.com/Article/details/guubsxytc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.yfazqb.com/Article/details/gqlbyqbbr.sHtML

TS:   return { a, b };
来源：http://baike.tarul.cn/Article/details/giabafgky.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.epnwcf.com/Article/details/gpxgxebfu.sHtML

Go:   return a, b
来源：http://m.share.bbcook.cn/Article/details/ghvaigcqh.sHtML

Ruby: return a, b
来源：http://www.m.share.sjlbkw.cn/Article/details/gvocoixgi.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.sjlbkw.cn/Article/details/gonkbpmjj.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fktsv.cn/Article/details/gfdsivlbf.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fktsv.cn/Article/details/ghmuwfnor.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.yfazqb.com/Article/details/gsyrqtqsn.sHtML

JS:   const square = x => x * x;
来源：http://m.share.vehdjk.com/Article/details/giwocapno.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.bbcook.cn/Article/details/guaiubrou.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.sjlbkw.cn/Article/details/gaddqeief.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.epnwcf.com/Article/details/gqxfnrebt.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.yfazqb.com/Article/details/gjyfejxgc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.sjlbkw.cn/Article/details/gmpkoefzw.sHtML

[C07] 把函数作为参数传入
来源：http://wap.sjlbkw.cn/Article/details/grbtebqae.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.tarul.cn/Article/details/gmqkfktsc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.vehdjk.com/Article/details/genwrjbvx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.bbcook.cn/Article/details/gcplghims.sHtML

TS:   arr.map(String)
来源：http://www.share.bbcook.cn/Article/details/ghbgcwbxj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.tarul.cn/Article/details/gymfkcucb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fktsv.cn/Article/details/gosvfxsjn.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.sjlbkw.cn/Article/details/gezcdymsw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.tarul.cn/Article/details/ghurvdjkn.sHtML

[C08] 闭包
来源：http://blog.sjlbkw.cn/Article/details/glvaawncy.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.sjlbkw.cn/Article/details/gevpmsiaj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.sjlbkw.cn/Article/details/gusnianvy.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.yfazqb.com/Article/details/gphovsgxg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.sjlbkw.cn/Article/details/ghsacujvg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.bbcook.cn/Article/details/gebhxexep.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.sjlbkw.cn/Article/details/gttaiodid.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.epnwcf.com/Article/details/gxwwzqmwb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.yfazqb.com/Article/details/gvepnunwl.sHtML

[C09] 递归
来源：http://m.share.epnwcf.com/Article/details/gqxnmlwjl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.sjlbkw.cn/Article/details/gqisukury.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpflzhngj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.sjlbkw.cn/Article/details/ggyfttbnh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.bbcook.cn/Article/details/ghnzhnyak.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fktsv.cn/Article/details/gwyvltogh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.vehdjk.com/Article/details/gmqelfjjl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.tarul.cn/Article/details/gutbrcljq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.yfazqb.com/Article/details/glgsnwkfx.sHtML


<!-- 参考信息 -->