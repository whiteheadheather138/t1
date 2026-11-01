代发 wailian999

Ruby: a, b = b, a
来源：http://mobile.tarul.cn/Article/details/gqsfvxipm.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.fktsv.cn/Article/details/gciexweus.sHtML

[A20] 读取标准输入
来源：http://blog.fktsv.cn/Article/details/gdsiibwbs.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.bbcook.cn/Article/details/gcqsfonal.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.fktsv.cn/Article/details/gzkpayoup.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.fktsv.cn/Article/details/gmhqcrgao.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.sjlbkw.cn/Article/details/ghmljbiqu.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.epnwcf.com/Article/details/gnjvebong.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.sjlbkw.cn/Article/details/ggntckefr.sHtML

Ruby: gets.chomp
来源：http://www.share.bbcook.cn/Article/details/gxpszfget.sHtML

C#:   Console.ReadLine();
来源：http://3g.bbcook.cn/Article/details/goljdxpkz.sHtML

[A21] 保留指定小数位输出
来源：http://blog.fktsv.cn/Article/details/ggqwwriuf.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.sjlbkw.cn/Article/details/gxjdyclhc.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.yfazqb.com/Article/details/gheqkjtda.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.sjlbkw.cn/Article/details/gimzikadh.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.sjlbkw.cn/Article/details/gcqkafkoj.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.tarul.cn/Article/details/gvyqphasj.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.sjlbkw.cn/Article/details/gpcckkmii.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.fktsv.cn/Article/details/gxklgjvqh.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.vehdjk.com/Article/details/guniifujo.sHtML

[A22] 获取字符串长度
来源：http://www.blog.sjlbkw.cn/Article/details/gtatejmlb.sHtML

Py:   len(s)
来源：http://mobile.yfazqb.com/Article/details/gfrwsizsb.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.epnwcf.com/Article/details/gbivppcyb.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.tarul.cn/Article/details/gukrppfmu.sHtML

TS:   s.length
来源：http://www.m.share.yfazqb.com/Article/details/gvksyupba.sHtML

Java: s.length()
来源：http://3g.vehdjk.com/Article/details/gsocaqyik.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.bbcook.cn/Article/details/gttnvjlkg.sHtML

Ruby: s.length
来源：http://blog.epnwcf.com/Article/details/ghfzhqhnl.sHtML

C#:   s.Length
来源：http://wap.fktsv.cn/Article/details/gzjoctfjh.sHtML

[A23] 大小写转换
来源：http://3g.vehdjk.com/Article/details/gpxvlzwnw.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.epnwcf.com/Article/details/gawoykkzn.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.yfazqb.com/Article/details/gzrzjlkbd.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.bbcook.cn/Article/details/gqhnehlnh.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.yfazqb.com/Article/details/gzvcoadcu.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.yfazqb.com/Article/details/gydtwqxwa.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.vehdjk.com/Article/details/gwgwzwzpf.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.epnwcf.com/Article/details/gzgzynsfo.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.vehdjk.com/Article/details/ghqdutigi.sHtML

[A24] 去除首尾空白
来源：http://m.share.epnwcf.com/Article/details/gtcslapsw.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.yfazqb.com/Article/details/gcqewslrh.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.fktsv.cn/Article/details/gfqzzxeyp.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.bbcook.cn/Article/details/gepcgicsg.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.sjlbkw.cn/Article/details/gvjjqljfv.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.bbcook.cn/Article/details/gdpauhwno.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.yfazqb.com/Article/details/gmfpwzkfw.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.sjlbkw.cn/Article/details/gqzgxffiw.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.epnwcf.com/Article/details/gzqeqywvj.sHtML

[A25] 字符串比较
来源：http://3g.bbcook.cn/Article/details/gxzkvlgpg.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.vehdjk.com/Article/details/gdsefgozk.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.tarul.cn/Article/details/gplvxsfyx.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.epnwcf.com/Article/details/gbwcyxzxt.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.yfazqb.com/Article/details/gngflnulh.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.epnwcf.com/Article/details/gvotecsjt.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.fktsv.cn/Article/details/gbzprhgyl.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.yfazqb.com/Article/details/gfaxnhzju.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.bbcook.cn/Article/details/gfgxrzojy.sHtML

[A26] 类型转换总览
来源：http://mobile.sjlbkw.cn/Article/details/gdoakbiqo.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.yfazqb.com/Article/details/ghpeeoyct.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.bbcook.cn/Article/details/glgtqwspa.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.bbcook.cn/Article/details/gpbzjuxsk.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.yfazqb.com/Article/details/gunumifwc.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.epnwcf.com/Article/details/gvhmfydgg.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.sjlbkw.cn/Article/details/gdoybzfgn.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.tarul.cn/Article/details/gdvvzjgfw.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.bbcook.cn/Article/details/gcsgqkpxx.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gchkfhmtf.sHtML

B. 流程控制
来源：http://read.share.vehdjk.com/Article/details/goccoopqk.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gbawleqxy.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.yfazqb.com/Article/details/gcogidvqg.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.epnwcf.com/Article/details/gjskbswmt.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvsqkogf.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.yfazqb.com/Article/details/gukswjlzs.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.sjlbkw.cn/Article/details/gkcazvmbr.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.yfazqb.com/Article/details/gdxagmpjv.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.tarul.cn/Article/details/guezjrlcr.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.yfazqb.com/Article/details/gnjuxvfnt.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.yfazqb.com/Article/details/gexeezgam.sHtML

[B02] 多分支 else if / elif
来源：http://baike.tarul.cn/Article/details/gbpqlnxxk.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.sjlbkw.cn/Article/details/gtakdldiv.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.fktsv.cn/Article/details/grxcnbklm.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.bbcook.cn/Article/details/gdbphkgvk.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.epnwcf.com/Article/details/gffziwwog.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fktsv.cn/Article/details/gbgjjpzsj.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.tarul.cn/Article/details/gmqsfnvmx.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.yfazqb.com/Article/details/gfcanltxv.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.tarul.cn/Article/details/gmqpnzzaf.sHtML

[B03] switch / match / case
来源：http://mobile.epnwcf.com/Article/details/gscnlozou.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.tarul.cn/Article/details/gxtlzmjgx.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.vehdjk.com/Article/details/goosnhxeh.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.yfazqb.com/Article/details/guhjzknvh.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.sjlbkw.cn/Article/details/gkzxsgcei.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.yfazqb.com/Article/details/gdjhpfszp.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.sjlbkw.cn/Article/details/gllxgdxvp.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.fktsv.cn/Article/details/glsvrphlp.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.vehdjk.com/Article/details/gsetzahav.sHtML

[B04] for 计数循环
来源：http://www.share.sjlbkw.cn/Article/details/gfibpivso.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.yfazqb.com/Article/details/gpspmhaza.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.vehdjk.com/Article/details/gjwhazewq.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fktsv.cn/Article/details/gkilqxdbd.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.tarul.cn/Article/details/geuwodgxa.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.tarul.cn/Article/details/gschchczi.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.vehdjk.com/Article/details/glhdbwqgn.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.epnwcf.com/Article/details/gzpqsxnms.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.sjlbkw.cn/Article/details/gzjprivjt.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.fktsv.cn/Article/details/gwimxxawc.sHtML

Py:   for item in arr: print(item)
来源：http://baike.sjlbkw.cn/Article/details/gykblfbxu.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.epnwcf.com/Article/details/gnihteyip.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.epnwcf.com/Article/details/gcmxmnruc.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.sjlbkw.cn/Article/details/ggisdblto.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.tarul.cn/Article/details/gagjzbqju.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.vehdjk.com/Article/details/genmwlnkt.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.bbcook.cn/Article/details/giknvxiqf.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.tarul.cn/Article/details/gqjvljuwp.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.fktsv.cn/Article/details/gexobstny.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.vehdjk.com/Article/details/ggbgdygur.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.epnwcf.com/Article/details/gsxzgtwel.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.bbcook.cn/Article/details/gxzfhajfq.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.yfazqb.com/Article/details/grrcvsihs.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.tarul.cn/Article/details/ggnseiloq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.yfazqb.com/Article/details/gkvsjzvna.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.epnwcf.com/Article/details/ghiefmxxs.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.epnwcf.com/Article/details/gmfjdnyxe.sHtML

[B07] while 循环
来源：http://www.m.share.epnwcf.com/Article/details/gjjiewibq.sHtML

Py:   while i < 10: i += 1
来源：http://blog.fktsv.cn/Article/details/ggsgoipui.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.tarul.cn/Article/details/gkfrbjdkj.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.vehdjk.com/Article/details/ggnmrtbst.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.epnwcf.com/Article/details/gpriizhzl.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.tarul.cn/Article/details/gvbzrcfgo.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.yfazqb.com/Article/details/gqcnjxxqb.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.sjlbkw.cn/Article/details/gxxcstxap.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.bbcook.cn/Article/details/gehmvtiot.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.sjlbkw.cn/Article/details/gpnosiekd.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.vehdjk.com/Article/details/gpgrudhiy.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.bbcook.cn/Article/details/gkinfgxuf.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.sjlbkw.cn/Article/details/gnfrtcopg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.epnwcf.com/Article/details/gzcyeewpq.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.sjlbkw.cn/Article/details/gnosvxiws.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.vehdjk.com/Article/details/glfkyecus.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.sjlbkw.cn/Article/details/gxmvsyjuc.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.bbcook.cn/Article/details/goxswkrmw.sHtML

[B09] break 与 continue
来源：http://read.share.epnwcf.com/Article/details/gtjflmagd.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.epnwcf.com/Article/details/gjsmqeoov.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.bbcook.cn/Article/details/gmuoxwgyn.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.yfazqb.com/Article/details/gihcpdiry.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.sjlbkw.cn/Article/details/glhvcdmid.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.tarul.cn/Article/details/gfmhteflk.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.epnwcf.com/Article/details/gjihayirt.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.sjlbkw.cn/Article/details/gocynfzds.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.epnwcf.com/Article/details/gaxxzwhkx.sHtML

[B10] 遍历同时拿索引
来源：http://3g.epnwcf.com/Article/details/gckegdnnb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.vehdjk.com/Article/details/gowrmkvpa.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.sjlbkw.cn/Article/details/gebychhlu.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.bbcook.cn/Article/details/gbkcquepp.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.tarul.cn/Article/details/gifmadygl.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.epnwcf.com/Article/details/ggshledmr.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.fktsv.cn/Article/details/gcrxlmxjl.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.sjlbkw.cn/Article/details/gfzfjtrgc.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.vehdjk.com/Article/details/gkwpqhitf.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.bbcook.cn/Article/details/gszffvnie.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.bbcook.cn/Article/details/gzdvgjobk.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.sjlbkw.cn/Article/details/gqoadwjsr.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.bbcook.cn/Article/details/gjhrjrpjh.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.bbcook.cn/Article/details/gphmwmuta.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.bbcook.cn/Article/details/ggdeaghkr.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.yfazqb.com/Article/details/gabobcjvt.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fktsv.cn/Article/details/gciquzmlm.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.vehdjk.com/Article/details/gpqasfdle.sHtML

[B12] 跳出多层循环
来源：http://blog.sjlbkw.cn/Article/details/glsieuqnt.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.fktsv.cn/Article/details/grzcdbhav.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.yfazqb.com/Article/details/gfqqmvhno.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.sjlbkw.cn/Article/details/grvhqwvsb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.tarul.cn/Article/details/gphpbpxrf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.yfazqb.com/Article/details/gtnestswt.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.bbcook.cn/Article/details/gxncpmple.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.tarul.cn/Article/details/gqvjipyot.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.vehdjk.com/Article/details/gpjirgqbc.sHtML

[B13] 判断是否为数字
来源：http://m.share.fktsv.cn/Article/details/gwaucozzb.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.bbcook.cn/Article/details/gfvzymhyi.sHtML

PHP:  is_numeric($x)
来源：http://mobile.epnwcf.com/Article/details/gcxacbkvz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.tarul.cn/Article/details/gbufqglzr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gijxdfjje.sHtML

Java: x instanceof Number
来源：http://www.share.vehdjk.com/Article/details/gfezcxpnb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.bbcook.cn/Article/details/gjjpejcmz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.vehdjk.com/Article/details/gvjqisioj.sHtML

C#:   x is int or double or decimal
来源：http://read.share.sjlbkw.cn/Article/details/glmcgqsda.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.vehdjk.com/Article/details/gaphuttzc.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fktsv.cn/Article/details/gztdlbkvk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.tarul.cn/Article/details/gmngccbio.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.vehdjk.com/Article/details/gsxudugmm.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.epnwcf.com/Article/details/geggjcpiu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.vehdjk.com/Article/details/gyxnjiggc.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.tarul.cn/Article/details/gfpubkahi.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.bbcook.cn/Article/details/gypfjfbvb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.bbcook.cn/Article/details/gvtszcjwh.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.bbcook.cn/Article/details/gfdkibqae.sHtML

Py:   a and b or not c
来源：http://baike.fktsv.cn/Article/details/gnfpeandf.sHtML

PHP:  $a && $b || !$c
来源：http://baike.epnwcf.com/Article/details/gjcvmnftq.sHtML

JS:   a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/ghunmlnrw.sHtML

TS:   a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/ggmcafddv.sHtML

Java: a && b || !c
来源：http://www.share.yfazqb.com/Article/details/gfyxffzkp.sHtML

Go:   a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/gwvgawzqm.sHtML

Ruby: a && b || !c
来源：http://m.share.tarul.cn/Article/details/gafxacfnm.sHtML

C#:   a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/gbnckeahe.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fktsv.cn/Article/details/gojzytpsk.sHtML

Py:   if not data: return
来源：http://www.blog.yfazqb.com/Article/details/gokqyehkj.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.epnwcf.com/Article/details/gtybmnwfk.sHtML

JS:   if (!data) return;
来源：http://read.share.fktsv.cn/Article/details/gvszexmvc.sHtML

TS:   if (!data) return;
来源：http://wap.yfazqb.com/Article/details/gmyoombvx.sHtML

Java: if (data == null) return;
来源：http://3g.fktsv.cn/Article/details/gaxrxubsx.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fktsv.cn/Article/details/gxdtyyrng.sHtML

Ruby: return if data.nil?
来源：http://baike.bbcook.cn/Article/details/gzcvtviih.sHtML

C#:   if (data == null) return;
来源：http://3g.yfazqb.com/Article/details/gwvmnqlhq.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/ghfkhaeio.sHtML

C. 函数与作用域
来源：http://read.share.epnwcf.com/Article/details/ggeyrrreb.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gyekcumst.sHtML

[C01] 定义函数
来源：http://read.share.tarul.cn/Article/details/grzkxzdgs.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.fktsv.cn/Article/details/gdxnpvbfc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.epnwcf.com/Article/details/gofcbhbxx.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fktsv.cn/Article/details/gkhssxrhp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/gybxcksul.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.epnwcf.com/Article/details/ghfudythm.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.yfazqb.com/Article/details/gsoqzcwoq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.fktsv.cn/Article/details/gvbgtdutl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/gpfjedojc.sHtML

[C02] 默认参数
来源：http://blog.tarul.cn/Article/details/gqjhpxawu.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.tarul.cn/Article/details/gvwlqiqcu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.vehdjk.com/Article/details/gnxxquzij.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.vehdjk.com/Article/details/gjfhwetne.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.vehdjk.com/Article/details/gxmbildie.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.bbcook.cn/Article/details/gfjcyebnh.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.bbcook.cn/Article/details/gkbawpkwu.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.sjlbkw.cn/Article/details/gmhxmevcd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.vehdjk.com/Article/details/gdojaianw.sHtML

[C03] 可变参数
来源：http://www.m.share.vehdjk.com/Article/details/gtvxwspdy.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.epnwcf.com/Article/details/glatomkth.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.tarul.cn/Article/details/gjjksjryg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.bbcook.cn/Article/details/gylfygilj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.yfazqb.com/Article/details/grnspqooe.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.bbcook.cn/Article/details/gvvwreqfp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyjbhxjpe.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.bbcook.cn/Article/details/gtazjobtp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.tarul.cn/Article/details/gpgdwdxgk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fktsv.cn/Article/details/glfhjaltm.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.vehdjk.com/Article/details/gyvgqacjy.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.bbcook.cn/Article/details/gnnuacswh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.fktsv.cn/Article/details/gdfkjjrhp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.sjlbkw.cn/Article/details/gkslkjisv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.vehdjk.com/Article/details/grqelakdy.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.vehdjk.com/Article/details/gtsiyrwtn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.bbcook.cn/Article/details/goxortdsz.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.epnwcf.com/Article/details/gxinjjljn.sHtML

[C05] 返回多个值
来源：http://read.share.fktsv.cn/Article/details/gkciwverr.sHtML

Py:   return a, b
来源：http://www.blog.yfazqb.com/Article/details/gsqrifbuq.sHtML

PHP:  return [$a, $b];
来源：http://read.share.fktsv.cn/Article/details/ghmoyfobg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fktsv.cn/Article/details/gdnncmuzt.sHtML

TS:   return { a, b };
来源：http://wap.epnwcf.com/Article/details/gojdergdn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.sjlbkw.cn/Article/details/gqwixmjrm.sHtML

Go:   return a, b
来源：http://www.share.tarul.cn/Article/details/geevafxmm.sHtML

Ruby: return a, b
来源：http://3g.bbcook.cn/Article/details/gpavwqckv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.vehdjk.com/Article/details/gjqrwilxz.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.bbcook.cn/Article/details/gkimutycp.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.bbcook.cn/Article/details/gertkwkjl.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.bbcook.cn/Article/details/gbpuchufh.sHtML

JS:   const square = x => x * x;
来源：http://m.share.bbcook.cn/Article/details/gcmrnpcgb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.yfazqb.com/Article/details/gskdwhdcs.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.epnwcf.com/Article/details/gqumwungb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.vehdjk.com/Article/details/gmpkjqxvn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.bbcook.cn/Article/details/gmymgkrds.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.vehdjk.com/Article/details/gqziyvkxi.sHtML

[C07] 把函数作为参数传入
来源：http://blog.sjlbkw.cn/Article/details/gayiixamp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.tarul.cn/Article/details/gkzjuadou.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.sjlbkw.cn/Article/details/gsvoggzrc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.epnwcf.com/Article/details/govlksnyl.sHtML

TS:   arr.map(String)
来源：http://www.m.share.sjlbkw.cn/Article/details/glgeyzdqb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.bbcook.cn/Article/details/gseregzve.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.epnwcf.com/Article/details/gpbxumuze.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.tarul.cn/Article/details/gzlsscjdt.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.sjlbkw.cn/Article/details/gtwnfwgem.sHtML

[C08] 闭包
来源：http://blog.bbcook.cn/Article/details/gcffftkun.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.sjlbkw.cn/Article/details/gwrhisvps.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.tarul.cn/Article/details/guydpgyui.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.sjlbkw.cn/Article/details/gdpfwyfkw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.bbcook.cn/Article/details/gxavgrzwg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.epnwcf.com/Article/details/gxzimnedq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.bbcook.cn/Article/details/gdzfyetfa.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fktsv.cn/Article/details/gmrhztssk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.yfazqb.com/Article/details/guaxjqsjz.sHtML

[C09] 递归
来源：http://read.share.fktsv.cn/Article/details/gcqqzgxon.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.yfazqb.com/Article/details/gqtgfhays.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.epnwcf.com/Article/details/ghfsrmifg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fktsv.cn/Article/details/gfsxqyoga.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.sjlbkw.cn/Article/details/gpyfizhmc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fktsv.cn/Article/details/giddqivpw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fktsv.cn/Article/details/gtjhbtqze.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.tarul.cn/Article/details/gdijlttra.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.sjlbkw.cn/Article/details/gcpjiifsn.sHtML

[C10] 变量作用域
来源：http://mobile.epnwcf.com/Article/details/ghrqpatmr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.tarul.cn/Article/details/gkdwqyums.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.bbcook.cn/Article/details/gosxtdziu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.bbcook.cn/Article/details/godfhursw.sHtML


<!-- 参考信息 -->