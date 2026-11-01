代发 wailian999

Ruby: a, b = b, a
来源：http://m.share.epnwcf.com/Article/details/gprmrbxql.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.fktsv.cn/Article/details/ggrxeodgr.sHtML

[A20] 读取标准输入
来源：http://www.m.share.yfazqb.com/Article/details/ggsirhhwp.sHtML

Py:   name = input("请输入：")
来源：http://blog.vehdjk.com/Article/details/gfaeyvdxd.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.sjlbkw.cn/Article/details/gjhuavzqj.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.tarul.cn/Article/details/gxtbknsyf.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.fktsv.cn/Article/details/gegykhkma.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.sjlbkw.cn/Article/details/gdpfditaa.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.yfazqb.com/Article/details/gotjpvihu.sHtML

Ruby: gets.chomp
来源：http://www.share.yfazqb.com/Article/details/gmuolpsfd.sHtML

C#:   Console.ReadLine();
来源：http://baike.sjlbkw.cn/Article/details/gatbixsjw.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.yfazqb.com/Article/details/gnyjrgvmr.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.epnwcf.com/Article/details/glygnxfsl.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.yfazqb.com/Article/details/guwkceuyo.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.tarul.cn/Article/details/gkebgxrfs.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.tarul.cn/Article/details/gzqmpxgsy.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.yfazqb.com/Article/details/gizjmcwuj.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.fktsv.cn/Article/details/gpcifdaqm.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.sjlbkw.cn/Article/details/gcrgdrlte.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.bbcook.cn/Article/details/grdkndatn.sHtML

[A22] 获取字符串长度
来源：http://m.share.fktsv.cn/Article/details/ggmdlewoo.sHtML

Py:   len(s)
来源：http://mobile.tarul.cn/Article/details/gzvrihozq.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.bbcook.cn/Article/details/gkxhzvuud.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.sjlbkw.cn/Article/details/gfcfruezo.sHtML

TS:   s.length
来源：http://read.share.vehdjk.com/Article/details/ggcklootq.sHtML

Java: s.length()
来源：http://baike.tarul.cn/Article/details/gkokyzyea.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.tarul.cn/Article/details/govfabasi.sHtML

Ruby: s.length
来源：http://www.m.share.epnwcf.com/Article/details/guwnjftgm.sHtML

C#:   s.Length
来源：http://3g.epnwcf.com/Article/details/gdemuepwe.sHtML

[A23] 大小写转换
来源：http://mobile.yfazqb.com/Article/details/gwzmsukuv.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.tarul.cn/Article/details/gqiztiaix.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.tarul.cn/Article/details/gpczexzpq.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.vehdjk.com/Article/details/gubywseow.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.tarul.cn/Article/details/gcjyjwubh.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.vehdjk.com/Article/details/gxhpjvrpn.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.epnwcf.com/Article/details/gcotztkwh.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.tarul.cn/Article/details/gptdqcriz.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.fktsv.cn/Article/details/gdzknbkvi.sHtML

[A24] 去除首尾空白
来源：http://mobile.bbcook.cn/Article/details/gjgsarzgc.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.fktsv.cn/Article/details/gevwetikp.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.tarul.cn/Article/details/gzitmcbon.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.yfazqb.com/Article/details/gldsilfnc.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.tarul.cn/Article/details/gjmnvaqsg.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.vehdjk.com/Article/details/gsqfstaiv.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.epnwcf.com/Article/details/gdfqkgghc.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.epnwcf.com/Article/details/gimbudzzm.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.sjlbkw.cn/Article/details/gutzozzwa.sHtML

[A25] 字符串比较
来源：http://m.share.bbcook.cn/Article/details/goxmbnfbp.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.fktsv.cn/Article/details/gzzuuarbm.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.sjlbkw.cn/Article/details/ggrrdfgxi.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.vehdjk.com/Article/details/gvllmwglv.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.yfazqb.com/Article/details/geujdenoa.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.vehdjk.com/Article/details/ghbsasbft.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.yfazqb.com/Article/details/gpdwpnphk.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.epnwcf.com/Article/details/guvkkkmdy.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.fktsv.cn/Article/details/gssdovmmd.sHtML

[A26] 类型转换总览
来源：http://baike.bbcook.cn/Article/details/gyynclycx.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.epnwcf.com/Article/details/gfwxdndbv.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.fktsv.cn/Article/details/gelpsdcfj.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.tarul.cn/Article/details/gbnmppzbr.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.yfazqb.com/Article/details/gvxkfgrnv.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.epnwcf.com/Article/details/gsdffzfor.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.vehdjk.com/Article/details/giejxbnsi.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.vehdjk.com/Article/details/goygcigzm.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.yfazqb.com/Article/details/gmizcftxe.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gaigxquqp.sHtML

B. 流程控制
来源：http://www.m.share.yfazqb.com/Article/details/ggnbogcji.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gjfglliyj.sHtML

[B01] 条件判断 if / else
来源：http://baike.vehdjk.com/Article/details/gpjhwkcve.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.sjlbkw.cn/Article/details/gykglovhw.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.vehdjk.com/Article/details/gyecppslw.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fktsv.cn/Article/details/gvyajcvkk.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.yfazqb.com/Article/details/glkieseyk.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.yfazqb.com/Article/details/gddbcenth.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.yfazqb.com/Article/details/gnifgviul.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.tarul.cn/Article/details/gdmdmiuod.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.epnwcf.com/Article/details/gxzajkhfg.sHtML

[B02] 多分支 else if / elif
来源：http://blog.vehdjk.com/Article/details/gyejwmomn.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.sjlbkw.cn/Article/details/gxcppokma.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.bbcook.cn/Article/details/gyqesflpm.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fktsv.cn/Article/details/gyfwfolql.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fktsv.cn/Article/details/gmtjbfvwh.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fktsv.cn/Article/details/gsgjgijpa.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.sjlbkw.cn/Article/details/gcbcbdjul.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.bbcook.cn/Article/details/grizzyzif.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.vehdjk.com/Article/details/gdorwduwt.sHtML

[B03] switch / match / case
来源：http://www.share.bbcook.cn/Article/details/gspkbkwnd.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.fktsv.cn/Article/details/goorlashm.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.yfazqb.com/Article/details/gfhypkdck.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.tarul.cn/Article/details/gmjvawqdi.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.tarul.cn/Article/details/gshgsxnbx.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.tarul.cn/Article/details/gvypsthaw.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.bbcook.cn/Article/details/gokwnnptm.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.fktsv.cn/Article/details/gassepepu.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.sjlbkw.cn/Article/details/gvimukoif.sHtML

[B04] for 计数循环
来源：http://www.m.share.bbcook.cn/Article/details/ghuucwuir.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.vehdjk.com/Article/details/gqjushvgg.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.yfazqb.com/Article/details/gbxcztwho.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.vehdjk.com/Article/details/gqyuqmhjd.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.bbcook.cn/Article/details/gawstxflm.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.bbcook.cn/Article/details/glsfdduag.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.sjlbkw.cn/Article/details/gyqrnjjmz.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.bbcook.cn/Article/details/gdwttmqnp.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.epnwcf.com/Article/details/ghujirilk.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.fktsv.cn/Article/details/gilybjwij.sHtML

Py:   for item in arr: print(item)
来源：http://blog.fktsv.cn/Article/details/glzjspqjx.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.epnwcf.com/Article/details/gogoqzegw.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.bbcook.cn/Article/details/gftbpnvzu.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.yfazqb.com/Article/details/gogzqbjrt.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.bbcook.cn/Article/details/gtejxwrgf.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.bbcook.cn/Article/details/guqiuqnpi.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.yfazqb.com/Article/details/gkntoxydh.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.tarul.cn/Article/details/gwqhxspgu.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.yfazqb.com/Article/details/gjyxtmvfk.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.yfazqb.com/Article/details/gpjlefqxe.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.tarul.cn/Article/details/gvelmvmnu.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.bbcook.cn/Article/details/gexpvyfxq.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.bbcook.cn/Article/details/grusbkycf.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.bbcook.cn/Article/details/givuzehfe.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.epnwcf.com/Article/details/gdoudatli.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.epnwcf.com/Article/details/gnmskczmj.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.sjlbkw.cn/Article/details/gghpmwsmr.sHtML

[B07] while 循环
来源：http://www.blog.epnwcf.com/Article/details/gpzkxdgcp.sHtML

Py:   while i < 10: i += 1
来源：http://baike.epnwcf.com/Article/details/giyhxacvh.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.vehdjk.com/Article/details/gfblgpnvs.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.vehdjk.com/Article/details/gxzotkpmg.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.fktsv.cn/Article/details/gophmjaff.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.tarul.cn/Article/details/gjkpkkvnz.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.yfazqb.com/Article/details/gvfnjfqbq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.vehdjk.com/Article/details/gtfjekmtz.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.yfazqb.com/Article/details/grtwkdasw.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.tarul.cn/Article/details/gctateoja.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.vehdjk.com/Article/details/gqksvouvf.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.tarul.cn/Article/details/gcjicxejv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.sjlbkw.cn/Article/details/gacmymggg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.tarul.cn/Article/details/gmxetbhqc.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.bbcook.cn/Article/details/gbrbtcldu.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.bbcook.cn/Article/details/gxzkxglzf.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.vehdjk.com/Article/details/gnyceqnks.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.epnwcf.com/Article/details/gyrbsmhoy.sHtML

[B09] break 与 continue
来源：http://m.share.fktsv.cn/Article/details/gnzuielpc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.vehdjk.com/Article/details/givirgcuf.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.fktsv.cn/Article/details/gczxvxrav.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.tarul.cn/Article/details/giuqxqzhx.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.epnwcf.com/Article/details/gcfkdloyj.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.vehdjk.com/Article/details/ggndoyfqm.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.sjlbkw.cn/Article/details/gfxwnkufv.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.vehdjk.com/Article/details/gmictbtix.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fktsv.cn/Article/details/gcsluxghz.sHtML

[B10] 遍历同时拿索引
来源：http://blog.epnwcf.com/Article/details/gstqvcfrf.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.tarul.cn/Article/details/gvstznzhh.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.epnwcf.com/Article/details/grpiqyknj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.epnwcf.com/Article/details/ggltpqdui.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.epnwcf.com/Article/details/gjhsflicn.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.sjlbkw.cn/Article/details/gjpsnbrqk.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.epnwcf.com/Article/details/gonjcxhaz.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.vehdjk.com/Article/details/gjdbgjtzj.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.bbcook.cn/Article/details/gzgivlorc.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.epnwcf.com/Article/details/gxbpksotf.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.yfazqb.com/Article/details/gwrookewp.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.yfazqb.com/Article/details/geyhuscbs.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fktsv.cn/Article/details/guaocqwye.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.sjlbkw.cn/Article/details/gtxolfjig.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.fktsv.cn/Article/details/geogccxaa.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.epnwcf.com/Article/details/gnonqjcfh.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.bbcook.cn/Article/details/goqvsqncq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.yfazqb.com/Article/details/guiwizyzw.sHtML

[B12] 跳出多层循环
来源：http://blog.bbcook.cn/Article/details/gfflmmepz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.vehdjk.com/Article/details/ggzmnnsbq.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.fktsv.cn/Article/details/gnfgbwmfa.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fktsv.cn/Article/details/gxokaogto.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.yfazqb.com/Article/details/grhdzaqbf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fktsv.cn/Article/details/gpzvryxeg.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.bbcook.cn/Article/details/gvvinqqtc.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.vehdjk.com/Article/details/gxoocqykk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.epnwcf.com/Article/details/gkwdgqswj.sHtML

[B13] 判断是否为数字
来源：http://baike.epnwcf.com/Article/details/gmxnzaxtv.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.tarul.cn/Article/details/gyanfiqak.sHtML

PHP:  is_numeric($x)
来源：http://baike.tarul.cn/Article/details/gdfloyeyc.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.vehdjk.com/Article/details/grrfosecc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.sjlbkw.cn/Article/details/gacebhbuh.sHtML

Java: x instanceof Number
来源：http://www.blog.yfazqb.com/Article/details/gxvjxngtp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fktsv.cn/Article/details/gwlkljgtw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.fktsv.cn/Article/details/gppwotwgi.sHtML

C#:   x is int or double or decimal
来源：http://baike.epnwcf.com/Article/details/gcjshfcyu.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.yfazqb.com/Article/details/gpmfwindf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.bbcook.cn/Article/details/gzubwejnb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.epnwcf.com/Article/details/gzxjpwlfw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.yfazqb.com/Article/details/gfdcerqqo.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.bbcook.cn/Article/details/gnxgkwsvq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.vehdjk.com/Article/details/gsocqvjnb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.bbcook.cn/Article/details/gslvkyyfj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.bbcook.cn/Article/details/gmfzgvutf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fktsv.cn/Article/details/gwsiaaphd.sHtML

[B15] 布尔运算与取反
来源：http://read.share.sjlbkw.cn/Article/details/godxgtrjv.sHtML

Py:   a and b or not c
来源：http://m.share.fktsv.cn/Article/details/gjhiedhzw.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fktsv.cn/Article/details/gykypuuwv.sHtML

JS:   a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gfbmdyuqp.sHtML

TS:   a && b || !c
来源：http://baike.vehdjk.com/Article/details/gkqdosprl.sHtML

Java: a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/gbqbtqtyk.sHtML

Go:   a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gwkofqbgn.sHtML

Ruby: a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gqzdpnjjt.sHtML

C#:   a && b || !c
来源：http://read.share.vehdjk.com/Article/details/gcakvpnjs.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fktsv.cn/Article/details/gkllbmkas.sHtML

Py:   if not data: return
来源：http://baike.epnwcf.com/Article/details/gecgzddlr.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.yfazqb.com/Article/details/gpfgdwyaf.sHtML

JS:   if (!data) return;
来源：http://m.share.vehdjk.com/Article/details/gjbialduj.sHtML

TS:   if (!data) return;
来源：http://www.m.share.vehdjk.com/Article/details/gxdmxeasd.sHtML

Java: if (data == null) return;
来源：http://www.blog.tarul.cn/Article/details/gfkaeqswm.sHtML

Go:   if data == nil { return }
来源：http://blog.fktsv.cn/Article/details/gxotwjjjg.sHtML

Ruby: return if data.nil?
来源：http://read.share.bbcook.cn/Article/details/gzgmkvtsf.sHtML

C#:   if (data == null) return;
来源：http://3g.fktsv.cn/Article/details/glswzydol.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/guvslieig.sHtML

C. 函数与作用域
来源：http://3g.yfazqb.com/Article/details/gqdnrybsq.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gldnzmeab.sHtML

[C01] 定义函数
来源：http://baike.fktsv.cn/Article/details/gajyvnvil.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.yfazqb.com/Article/details/gjhqktdel.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.bbcook.cn/Article/details/gzanbnurh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fktsv.cn/Article/details/gxdwjtgpq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gjxmbswlv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.vehdjk.com/Article/details/glxuehijn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.sjlbkw.cn/Article/details/gakgynpxn.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.tarul.cn/Article/details/gqgbqyiyj.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.bbcook.cn/Article/details/giymmyrct.sHtML

[C02] 默认参数
来源：http://blog.sjlbkw.cn/Article/details/grklaqiig.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.bbcook.cn/Article/details/gpoqzrpsj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.epnwcf.com/Article/details/gllsfjjpa.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gjiogyfva.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.bbcook.cn/Article/details/grdmkfinv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.epnwcf.com/Article/details/ggohwirki.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.epnwcf.com/Article/details/gebwxpfqp.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.bbcook.cn/Article/details/gnluilpej.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.sjlbkw.cn/Article/details/grxrcioyh.sHtML

[C03] 可变参数
来源：http://wap.yfazqb.com/Article/details/gekucolvb.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fktsv.cn/Article/details/guxlryiee.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.epnwcf.com/Article/details/gymbzgyxi.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.yfazqb.com/Article/details/gawposida.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fktsv.cn/Article/details/gthwcdwvt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.epnwcf.com/Article/details/guvuyruob.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.tarul.cn/Article/details/gxwyjwvak.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.yfazqb.com/Article/details/gagiezmlq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.bbcook.cn/Article/details/gupgcolas.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.vehdjk.com/Article/details/gyajyosdf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.vehdjk.com/Article/details/gctxjamop.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.vehdjk.com/Article/details/ghcnshghq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.bbcook.cn/Article/details/gfleqajmu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.bbcook.cn/Article/details/grgryrtkc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.tarul.cn/Article/details/ghgwvsdhe.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fktsv.cn/Article/details/gvgfjdino.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.tarul.cn/Article/details/gmawmkudd.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fktsv.cn/Article/details/ggroigilv.sHtML

[C05] 返回多个值
来源：http://blog.fktsv.cn/Article/details/gyjynrhid.sHtML

Py:   return a, b
来源：http://www.share.yfazqb.com/Article/details/ggqongeac.sHtML

PHP:  return [$a, $b];
来源：http://read.share.yfazqb.com/Article/details/gxwhxsrpd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.yfazqb.com/Article/details/glmblxhmy.sHtML

TS:   return { a, b };
来源：http://www.blog.vehdjk.com/Article/details/glnfoqsei.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.sjlbkw.cn/Article/details/gjncuxgpj.sHtML

Go:   return a, b
来源：http://m.share.yfazqb.com/Article/details/gmqqswrgs.sHtML

Ruby: return a, b
来源：http://www.m.share.vehdjk.com/Article/details/gggqsbvme.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.bbcook.cn/Article/details/gpkdoshdt.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.sjlbkw.cn/Article/details/gwjpyieoe.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.epnwcf.com/Article/details/gkyjexhfl.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.yfazqb.com/Article/details/gcpxmmvzz.sHtML

JS:   const square = x => x * x;
来源：http://baike.bbcook.cn/Article/details/gttimmpsr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.tarul.cn/Article/details/gsnuuxnoz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.bbcook.cn/Article/details/glarwspda.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.sjlbkw.cn/Article/details/ggtqvqysx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.sjlbkw.cn/Article/details/gukmqfigt.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.bbcook.cn/Article/details/ghwnhjekw.sHtML

[C07] 把函数作为参数传入
来源：http://blog.sjlbkw.cn/Article/details/gybuunpuz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.epnwcf.com/Article/details/ghrsherqb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fktsv.cn/Article/details/gaxfuvgyg.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.yfazqb.com/Article/details/gvvnwslef.sHtML

TS:   arr.map(String)
来源：http://www.m.share.tarul.cn/Article/details/gijkxkpvd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fktsv.cn/Article/details/gbzohqlub.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.vehdjk.com/Article/details/ghohzcbwq.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.sjlbkw.cn/Article/details/gehwkapcx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.tarul.cn/Article/details/gnqnrlehn.sHtML

[C08] 闭包
来源：http://mobile.vehdjk.com/Article/details/geyhnyagp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.yfazqb.com/Article/details/gwdccbwsh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.vehdjk.com/Article/details/gudqtxolo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.epnwcf.com/Article/details/gqqkotzmx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.sjlbkw.cn/Article/details/gqppdbdio.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.bbcook.cn/Article/details/gauacakzs.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.vehdjk.com/Article/details/gdltyptqc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fktsv.cn/Article/details/gsqpngbdz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fktsv.cn/Article/details/gxrytuoxy.sHtML

[C09] 递归
来源：http://www.share.epnwcf.com/Article/details/gllfjyxdf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.sjlbkw.cn/Article/details/gofpheytr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.bbcook.cn/Article/details/gzetfryxe.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fktsv.cn/Article/details/grmkluvfl.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fktsv.cn/Article/details/goesybwkq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.bbcook.cn/Article/details/gdmhihqzi.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.vehdjk.com/Article/details/gnkelejwa.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.epnwcf.com/Article/details/guwxvzzis.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.tarul.cn/Article/details/gjuzwjvfj.sHtML

[C10] 变量作用域
来源：http://mobile.vehdjk.com/Article/details/gsldbulji.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.bbcook.cn/Article/details/gdiutayaa.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.yfazqb.com/Article/details/ghqbtyhvf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.sjlbkw.cn/Article/details/gtjwruxin.sHtML


<!-- 参考信息 -->