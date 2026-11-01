代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.bbcook.cn/Article/details/gtzdaatda.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.vehdjk.com/Article/details/griyxmlne.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.vehdjk.com/Article/details/grhueabpx.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.fktsv.cn/Article/details/guyjgpayv.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.fktsv.cn/Article/details/gsgevaqxn.sHtML

Ruby: gets.chomp
来源：http://read.share.yfazqb.com/Article/details/ghaculjtk.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.epnwcf.com/Article/details/gzdqapiki.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.bbcook.cn/Article/details/gltlhljex.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.epnwcf.com/Article/details/gltyekkcm.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.tarul.cn/Article/details/gymipgnas.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.tarul.cn/Article/details/gcveqkivh.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.fktsv.cn/Article/details/gojqztnnd.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.vehdjk.com/Article/details/gigkxvevw.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.tarul.cn/Article/details/gxrvvbvgl.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.epnwcf.com/Article/details/gtgjgprmr.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.tarul.cn/Article/details/gbbljkqsb.sHtML

[A22] 获取字符串长度
来源：http://baike.epnwcf.com/Article/details/gplbfjupp.sHtML

Py:   len(s)
来源：http://read.share.fktsv.cn/Article/details/gsrlirkoo.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.yfazqb.com/Article/details/gtdkearyd.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.epnwcf.com/Article/details/gavfickvf.sHtML

TS:   s.length
来源：http://www.blog.yfazqb.com/Article/details/gnpvptdfw.sHtML

Java: s.length()
来源：http://www.share.vehdjk.com/Article/details/gofebdzzl.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.tarul.cn/Article/details/gabzzszwl.sHtML

Ruby: s.length
来源：http://3g.bbcook.cn/Article/details/ggwmpqaxm.sHtML

C#:   s.Length
来源：http://wap.yfazqb.com/Article/details/gxuwpqdji.sHtML

[A23] 大小写转换
来源：http://read.share.bbcook.cn/Article/details/gxhoxvnjg.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.vehdjk.com/Article/details/gnhwxifbu.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.bbcook.cn/Article/details/gzapcnvze.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.bbcook.cn/Article/details/gdzlmmsof.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.sjlbkw.cn/Article/details/gtbsjyprl.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.vehdjk.com/Article/details/ghwjvyhmk.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.vehdjk.com/Article/details/ghgbdnirt.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.tarul.cn/Article/details/goolhawqg.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.sjlbkw.cn/Article/details/gjljcrpij.sHtML

[A24] 去除首尾空白
来源：http://read.share.tarul.cn/Article/details/gmwtuzuew.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.bbcook.cn/Article/details/gdpxdnhyb.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.sjlbkw.cn/Article/details/ggbhcwelq.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.bbcook.cn/Article/details/gwhhzeete.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.fktsv.cn/Article/details/ghyuihprf.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.fktsv.cn/Article/details/gvkeradpx.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.epnwcf.com/Article/details/gzlqzgwwj.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.bbcook.cn/Article/details/gpqcrserh.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.epnwcf.com/Article/details/gxbldgdwt.sHtML

[A25] 字符串比较
来源：http://www.m.share.vehdjk.com/Article/details/gvfyphwut.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.fktsv.cn/Article/details/gctvqeejp.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.yfazqb.com/Article/details/gytxslhqb.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfakefwvc.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.vehdjk.com/Article/details/gywwqerlz.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.bbcook.cn/Article/details/gbiqeuywd.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.tarul.cn/Article/details/gppupfzyj.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.fktsv.cn/Article/details/ghdlenakr.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.vehdjk.com/Article/details/gmnfmxeuo.sHtML

[A26] 类型转换总览
来源：http://3g.yfazqb.com/Article/details/gufsxbzit.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.epnwcf.com/Article/details/gvlayokmi.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.epnwcf.com/Article/details/gvojcjwtq.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.tarul.cn/Article/details/gaocukzde.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.fktsv.cn/Article/details/gymhfpzta.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.tarul.cn/Article/details/gyvtscrwn.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.bbcook.cn/Article/details/gqmbwwoyb.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.vehdjk.com/Article/details/gxjscludb.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.sjlbkw.cn/Article/details/ggcoavutf.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gvddyxskn.sHtML

B. 流程控制
来源：http://www.blog.yfazqb.com/Article/details/gudaunmki.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gouanztck.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.sjlbkw.cn/Article/details/gdyljjxmb.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.tarul.cn/Article/details/gljzmtrlw.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.bbcook.cn/Article/details/gdxfvhbou.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.sjlbkw.cn/Article/details/gimvmrugy.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.tarul.cn/Article/details/gtrrjplch.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.vehdjk.com/Article/details/guhzatdiv.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.vehdjk.com/Article/details/gaffdjplk.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.sjlbkw.cn/Article/details/gzrmtlztg.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.fktsv.cn/Article/details/gqjeldspm.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.vehdjk.com/Article/details/gxekpnrdh.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.yfazqb.com/Article/details/gcpjjrvzk.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.fktsv.cn/Article/details/guahiktnm.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.vehdjk.com/Article/details/gvgxorvcr.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.bbcook.cn/Article/details/gkqotpfmy.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.tarul.cn/Article/details/gihpwiuth.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.epnwcf.com/Article/details/glhoemnkt.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.fktsv.cn/Article/details/gvgrakobn.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.yfazqb.com/Article/details/gtskeogme.sHtML

[B03] switch / match / case
来源：http://read.share.epnwcf.com/Article/details/gantaxeqb.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.epnwcf.com/Article/details/gxzjxomcx.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.fktsv.cn/Article/details/gphuisvjz.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.yfazqb.com/Article/details/gbjdujlrp.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.bbcook.cn/Article/details/gagayyqcm.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.epnwcf.com/Article/details/gfgiunuod.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.epnwcf.com/Article/details/gyiafmthu.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.bbcook.cn/Article/details/gqxsugzow.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.tarul.cn/Article/details/gyuqzsoyp.sHtML

[B04] for 计数循环
来源：http://baike.sjlbkw.cn/Article/details/glhozajsl.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.tarul.cn/Article/details/gdavhrrhl.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.epnwcf.com/Article/details/grvuvoofy.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.tarul.cn/Article/details/gujplivhn.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.tarul.cn/Article/details/gwqcjyctr.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.bbcook.cn/Article/details/gaszrephn.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.yfazqb.com/Article/details/gmlpyyevm.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.epnwcf.com/Article/details/gnyczgjrm.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.yfazqb.com/Article/details/gnrckgyqe.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.bbcook.cn/Article/details/gxrealomh.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.sjlbkw.cn/Article/details/gbeegbyyg.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.yfazqb.com/Article/details/gvdgdwgyw.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.vehdjk.com/Article/details/gqucxexej.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.sjlbkw.cn/Article/details/gjqgwfmsu.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.epnwcf.com/Article/details/gufrrjjxt.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.vehdjk.com/Article/details/gqwxlyola.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.tarul.cn/Article/details/guvjqtnjz.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.fktsv.cn/Article/details/gczrecuix.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.fktsv.cn/Article/details/grbukgzgd.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdfadfsrc.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.epnwcf.com/Article/details/gpsktuwaj.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.bbcook.cn/Article/details/grwjknphn.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.epnwcf.com/Article/details/ggwvevtia.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.sjlbkw.cn/Article/details/gvxlargvt.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.yfazqb.com/Article/details/gfaxojbld.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.sjlbkw.cn/Article/details/gbceygtgo.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.tarul.cn/Article/details/gqnjiytne.sHtML

[B07] while 循环
来源：http://www.share.bbcook.cn/Article/details/gvtaspaen.sHtML

Py:   while i < 10: i += 1
来源：http://baike.yfazqb.com/Article/details/gnhbpnqzj.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.bbcook.cn/Article/details/gebxnpkpt.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.yfazqb.com/Article/details/gyrapypth.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.yfazqb.com/Article/details/gnyopohkg.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.yfazqb.com/Article/details/grqvwwwrt.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.fktsv.cn/Article/details/gghlarpmo.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.bbcook.cn/Article/details/gwquqzsru.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.tarul.cn/Article/details/gffyhhrgk.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.yfazqb.com/Article/details/gygghznvr.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.yfazqb.com/Article/details/gvsosmqqj.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.fktsv.cn/Article/details/guhdevhbq.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.sjlbkw.cn/Article/details/gwmahwsna.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.fktsv.cn/Article/details/gdzfflpcs.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.sjlbkw.cn/Article/details/gowedvcdk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.fktsv.cn/Article/details/gxogwsydi.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.vehdjk.com/Article/details/gxtjpqrym.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.tarul.cn/Article/details/gofpjpzcp.sHtML

[B09] break 与 continue
来源：http://read.share.fktsv.cn/Article/details/gdnznunxi.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.sjlbkw.cn/Article/details/ghwzasouz.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.sjlbkw.cn/Article/details/gjediouic.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.sjlbkw.cn/Article/details/gawkalciq.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fktsv.cn/Article/details/gficekzdb.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.sjlbkw.cn/Article/details/gjcvjqhgb.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.bbcook.cn/Article/details/gpecknxlk.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.epnwcf.com/Article/details/gaicugqcm.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.bbcook.cn/Article/details/gtnkxtyix.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.tarul.cn/Article/details/gtpsdjtca.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.tarul.cn/Article/details/gmyjlyrzp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.tarul.cn/Article/details/gxniudczf.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.fktsv.cn/Article/details/gesddbxyl.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.tarul.cn/Article/details/gwghondgg.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.tarul.cn/Article/details/gzfdqkcqs.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.sjlbkw.cn/Article/details/gmozicuaw.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.epnwcf.com/Article/details/grfzvkriu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.fktsv.cn/Article/details/gwfwyklta.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.vehdjk.com/Article/details/gypcpymqw.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.tarul.cn/Article/details/gzfiwocpz.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.fktsv.cn/Article/details/gaoshqblb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.vehdjk.com/Article/details/gfzferool.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fktsv.cn/Article/details/gjwbbhuvp.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.epnwcf.com/Article/details/gpadtzhqa.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.sjlbkw.cn/Article/details/gmwmvaxlc.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.vehdjk.com/Article/details/gextqoyhr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.epnwcf.com/Article/details/gosyhhbty.sHtML

[B12] 跳出多层循环
来源：http://www.blog.yfazqb.com/Article/details/gfkkntged.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.yfazqb.com/Article/details/ggbqxozhr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.epnwcf.com/Article/details/gwlxbntwm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.yfazqb.com/Article/details/gybrfbamo.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.tarul.cn/Article/details/gwsyqzmnh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.yfazqb.com/Article/details/gkputcjcn.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.fktsv.cn/Article/details/gfdevxmzl.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.epnwcf.com/Article/details/gvwzfkoqt.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.epnwcf.com/Article/details/gllwpmytm.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.tarul.cn/Article/details/ghcqomttd.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.vehdjk.com/Article/details/gcillfrto.sHtML

PHP:  is_numeric($x)
来源：http://read.share.yfazqb.com/Article/details/gxojezsjq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fktsv.cn/Article/details/gnfyrpnop.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.epnwcf.com/Article/details/gtxmowetq.sHtML

Java: x instanceof Number
来源：http://3g.yfazqb.com/Article/details/grdwlohqy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.yfazqb.com/Article/details/ghpxltcyy.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.bbcook.cn/Article/details/gztymxafo.sHtML

C#:   x is int or double or decimal
来源：http://wap.yfazqb.com/Article/details/gpsnzvtig.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.epnwcf.com/Article/details/gmdchadje.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.fktsv.cn/Article/details/gaeydbdyf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.yfazqb.com/Article/details/gvktrrjju.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.vehdjk.com/Article/details/gswjxzrcz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.vehdjk.com/Article/details/glyfissmo.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.tarul.cn/Article/details/grnpgasmd.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.bbcook.cn/Article/details/gukqljlum.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.sjlbkw.cn/Article/details/gaoulxhhv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fktsv.cn/Article/details/gubeiediz.sHtML

[B15] 布尔运算与取反
来源：http://m.share.yfazqb.com/Article/details/glejadtny.sHtML

Py:   a and b or not c
来源：http://mobile.tarul.cn/Article/details/gfbuyomcj.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.vehdjk.com/Article/details/ghceqckkx.sHtML

JS:   a && b || !c
来源：http://baike.vehdjk.com/Article/details/gviftclwj.sHtML

TS:   a && b || !c
来源：http://blog.fktsv.cn/Article/details/gothufdmy.sHtML

Java: a && b || !c
来源：http://mobile.vehdjk.com/Article/details/gkjqpwlbv.sHtML

Go:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gntpfkmek.sHtML

Ruby: a && b || !c
来源：http://3g.epnwcf.com/Article/details/gaeegxtir.sHtML

C#:   a && b || !c
来源：http://blog.yfazqb.com/Article/details/gwtnyxdbk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fktsv.cn/Article/details/gmavqlesn.sHtML

Py:   if not data: return
来源：http://m.share.epnwcf.com/Article/details/gbngrhhca.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.vehdjk.com/Article/details/gzsnpzmas.sHtML

JS:   if (!data) return;
来源：http://blog.yfazqb.com/Article/details/gqelkrfgg.sHtML

TS:   if (!data) return;
来源：http://www.share.tarul.cn/Article/details/gbjptwjxj.sHtML

Java: if (data == null) return;
来源：http://www.share.yfazqb.com/Article/details/gridttlna.sHtML

Go:   if data == nil { return }
来源：http://mobile.fktsv.cn/Article/details/ginuknefr.sHtML

Ruby: return if data.nil?
来源：http://www.blog.yfazqb.com/Article/details/gfhlzqmmc.sHtML

C#:   if (data == null) return;
来源：http://read.share.bbcook.cn/Article/details/grzuweves.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gtohpxjea.sHtML

C. 函数与作用域
来源：http://www.share.yfazqb.com/Article/details/gdfzcabkz.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/grbmnqbdl.sHtML

[C01] 定义函数
来源：http://read.share.sjlbkw.cn/Article/details/gtyutmbgr.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.fktsv.cn/Article/details/gwgtzazac.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.tarul.cn/Article/details/gynjgkvpc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gziqnjgey.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.tarul.cn/Article/details/gibdzvghy.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gdpeldeqm.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.sjlbkw.cn/Article/details/gjsedvmub.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.fktsv.cn/Article/details/gaskqovzi.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.vehdjk.com/Article/details/gxtnjftyd.sHtML

[C02] 默认参数
来源：http://www.share.tarul.cn/Article/details/gvqfcrfds.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.vehdjk.com/Article/details/gjwwddjwg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.vehdjk.com/Article/details/gbqcobpxo.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gqmdewuzq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gisuthwxn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.vehdjk.com/Article/details/gcllncbsk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.fktsv.cn/Article/details/gbqpprzwr.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.epnwcf.com/Article/details/ggdbqrozm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.yfazqb.com/Article/details/gqkdakptm.sHtML

[C03] 可变参数
来源：http://blog.fktsv.cn/Article/details/ghxjcqtyn.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.sjlbkw.cn/Article/details/gketezhyz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.vehdjk.com/Article/details/gybqjboyv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.bbcook.cn/Article/details/ggljykuow.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.epnwcf.com/Article/details/gymwvbdra.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.bbcook.cn/Article/details/gwxyjagay.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.tarul.cn/Article/details/gnljufese.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.sjlbkw.cn/Article/details/gymogoaja.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.epnwcf.com/Article/details/gppeqovbx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmrhprda.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.sjlbkw.cn/Article/details/gicheoguw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.vehdjk.com/Article/details/gmggvpdgw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.sjlbkw.cn/Article/details/gxitpvppy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.vehdjk.com/Article/details/gfgzvoxqn.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.yfazqb.com/Article/details/goxuquwaa.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fktsv.cn/Article/details/geipqqlpc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.yfazqb.com/Article/details/gngkoiumc.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.epnwcf.com/Article/details/gmaacbitd.sHtML

[C05] 返回多个值
来源：http://wap.sjlbkw.cn/Article/details/gubttoiio.sHtML

Py:   return a, b
来源：http://wap.vehdjk.com/Article/details/gavuvtbiw.sHtML

PHP:  return [$a, $b];
来源：http://wap.yfazqb.com/Article/details/gwgsawejz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fktsv.cn/Article/details/gmmlwseql.sHtML

TS:   return { a, b };
来源：http://blog.vehdjk.com/Article/details/gjqlxkezg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.yfazqb.com/Article/details/gktfjhsqi.sHtML

Go:   return a, b
来源：http://mobile.vehdjk.com/Article/details/gqyfvktmt.sHtML

Ruby: return a, b
来源：http://read.share.fktsv.cn/Article/details/gyfamtlha.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.yfazqb.com/Article/details/gabledrvf.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fktsv.cn/Article/details/geclrvrcv.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.yfazqb.com/Article/details/gpzgyjsut.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.epnwcf.com/Article/details/gkchnccyu.sHtML

JS:   const square = x => x * x;
来源：http://m.share.sjlbkw.cn/Article/details/ghpgucgox.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.epnwcf.com/Article/details/gkomvshgk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.bbcook.cn/Article/details/gifmfpdup.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.epnwcf.com/Article/details/gyjidmrgt.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.bbcook.cn/Article/details/gllbfbots.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.vehdjk.com/Article/details/gylupexxo.sHtML

[C07] 把函数作为参数传入
来源：http://3g.yfazqb.com/Article/details/gizbuqnic.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.yfazqb.com/Article/details/gifymnkxu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.vehdjk.com/Article/details/gfknotkuh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.bbcook.cn/Article/details/glyoxzudc.sHtML

TS:   arr.map(String)
来源：http://mobile.sjlbkw.cn/Article/details/gylsokrbi.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.epnwcf.com/Article/details/gcpxjmaau.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.yfazqb.com/Article/details/grhtrjgjb.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.tarul.cn/Article/details/giprndcha.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.epnwcf.com/Article/details/gbfvvfltp.sHtML

[C08] 闭包
来源：http://3g.epnwcf.com/Article/details/gsvlisvop.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.epnwcf.com/Article/details/gacwkzfvu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.sjlbkw.cn/Article/details/gpipacrch.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.vehdjk.com/Article/details/gistsprqj.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.bbcook.cn/Article/details/gwbdlltym.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.epnwcf.com/Article/details/gmufjzhjj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fktsv.cn/Article/details/govauzyac.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.yfazqb.com/Article/details/gloursscv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.bbcook.cn/Article/details/gpvedgtmr.sHtML

[C09] 递归
来源：http://wap.sjlbkw.cn/Article/details/gdviqqswf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fktsv.cn/Article/details/gsrzqrkfy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fktsv.cn/Article/details/gstogqkjf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.bbcook.cn/Article/details/gmtkbbamw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.sjlbkw.cn/Article/details/gfzdywpcp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.bbcook.cn/Article/details/gecaizhnc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.tarul.cn/Article/details/gbejcxpbf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.bbcook.cn/Article/details/gsdeubfhf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gijhaybzr.sHtML

[C10] 变量作用域
来源：http://wap.tarul.cn/Article/details/gwpwdsqjz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.epnwcf.com/Article/details/gjsotexbb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.bbcook.cn/Article/details/gzfnssoma.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.yfazqb.com/Article/details/gehowawbi.sHtML

TS:   同 JS
来源：http://blog.sjlbkw.cn/Article/details/gaxxwytqz.sHtML

Java: 方法内为块级作用域
来源：http://blog.fktsv.cn/Article/details/gbbzocmes.sHtML

Go:   花括号块级作用域
来源：http://read.share.sjlbkw.cn/Article/details/gdtjzcmmj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fktsv.cn/Article/details/grvtlmblm.sHtML


<!-- 参考信息 -->