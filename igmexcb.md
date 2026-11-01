代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.vehdjk.com/Article/details/gchjdoihn.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.sjlbkw.cn/Article/details/glwwalyox.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.vehdjk.com/Article/details/gwnjetekh.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.vehdjk.com/Article/details/gqtjurgqg.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.tarul.cn/Article/details/gighrcnrc.sHtML

Ruby: gets.chomp
来源：http://mobile.vehdjk.com/Article/details/gextdvhzp.sHtML

C#:   Console.ReadLine();
来源：http://baike.vehdjk.com/Article/details/gzqztcvao.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.sjlbkw.cn/Article/details/gdamfnbcb.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.vehdjk.com/Article/details/gozemlldi.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.epnwcf.com/Article/details/gemfqgqja.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.epnwcf.com/Article/details/gqfttlmod.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.sjlbkw.cn/Article/details/gkojuklqg.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.sjlbkw.cn/Article/details/gxwxpcjtc.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.fktsv.cn/Article/details/gatjjdvmt.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.vehdjk.com/Article/details/gnwniyohs.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.tarul.cn/Article/details/gtlcbkgvl.sHtML

[A22] 获取字符串长度
来源：http://www.blog.yfazqb.com/Article/details/gigsahxfj.sHtML

Py:   len(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gynbyddij.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.bbcook.cn/Article/details/gxfduzafj.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.tarul.cn/Article/details/ggrjkcamw.sHtML

TS:   s.length
来源：http://www.m.share.fktsv.cn/Article/details/gssvddqlp.sHtML

Java: s.length()
来源：http://www.m.share.fktsv.cn/Article/details/gjgiubmmy.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.fktsv.cn/Article/details/glaagjufy.sHtML

Ruby: s.length
来源：http://read.share.bbcook.cn/Article/details/gncydtjds.sHtML

C#:   s.Length
来源：http://mobile.fktsv.cn/Article/details/gsjxlabeo.sHtML

[A23] 大小写转换
来源：http://www.blog.sjlbkw.cn/Article/details/gqtottoep.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.tarul.cn/Article/details/gdfjhtare.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.fktsv.cn/Article/details/gceckjvqw.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fktsv.cn/Article/details/govptjxlh.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.bbcook.cn/Article/details/ggfvnjhfo.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.tarul.cn/Article/details/gzollqoey.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.sjlbkw.cn/Article/details/gnpzswkvh.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.sjlbkw.cn/Article/details/grqqfzxiw.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.vehdjk.com/Article/details/gsysafwdd.sHtML

[A24] 去除首尾空白
来源：http://www.share.vehdjk.com/Article/details/guyqgknhg.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.tarul.cn/Article/details/gbhzamnxh.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.vehdjk.com/Article/details/gimscncvs.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.yfazqb.com/Article/details/gpwzsvsye.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fktsv.cn/Article/details/gqblndqjn.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.epnwcf.com/Article/details/gthhpcyge.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.epnwcf.com/Article/details/gtotqgqgl.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.tarul.cn/Article/details/gjeczbuhc.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.tarul.cn/Article/details/glbwzfelk.sHtML

[A25] 字符串比较
来源：http://baike.bbcook.cn/Article/details/gttxxtkqm.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.vehdjk.com/Article/details/glwvfpydk.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.epnwcf.com/Article/details/gtzefndjx.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.epnwcf.com/Article/details/ginragwya.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.fktsv.cn/Article/details/gxnvmyjzz.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.vehdjk.com/Article/details/gmmnwjdsy.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.bbcook.cn/Article/details/gqxoaceyh.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.epnwcf.com/Article/details/gpbrzemue.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.bbcook.cn/Article/details/grjzghike.sHtML

[A26] 类型转换总览
来源：http://www.share.bbcook.cn/Article/details/grbqlpvcu.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.yfazqb.com/Article/details/guixfjcar.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.sjlbkw.cn/Article/details/gmoejseyl.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.vehdjk.com/Article/details/gzuaremiw.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.yfazqb.com/Article/details/ggtbscjfo.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.fktsv.cn/Article/details/gbsuyfwmw.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.yfazqb.com/Article/details/gkzraield.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.bbcook.cn/Article/details/gczfprmib.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.tarul.cn/Article/details/gkmrjyccx.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gkaouenwv.sHtML

B. 流程控制
来源：http://www.share.yfazqb.com/Article/details/gtvbhteac.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/ghyqjlonr.sHtML

[B01] 条件判断 if / else
来源：http://read.share.fktsv.cn/Article/details/gfpmrzhgr.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.bbcook.cn/Article/details/gyrqehpkk.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.sjlbkw.cn/Article/details/gyegaidmv.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.sjlbkw.cn/Article/details/gaalldvom.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.sjlbkw.cn/Article/details/gpcoaftut.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.sjlbkw.cn/Article/details/gpnmgsdyi.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.yfazqb.com/Article/details/gjvmuzjrl.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.sjlbkw.cn/Article/details/gbzlfgnmi.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.epnwcf.com/Article/details/gcrfzylew.sHtML

[B02] 多分支 else if / elif
来源：http://baike.yfazqb.com/Article/details/gziptbbiy.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.tarul.cn/Article/details/guqicwvrz.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.yfazqb.com/Article/details/gqnapoyiv.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.bbcook.cn/Article/details/gddaxdtpn.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.tarul.cn/Article/details/glagqalbh.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.yfazqb.com/Article/details/gkqxyjubb.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.tarul.cn/Article/details/gjxlowvmv.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.vehdjk.com/Article/details/gqvxluvzd.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.vehdjk.com/Article/details/gedajlbqm.sHtML

[B03] switch / match / case
来源：http://baike.vehdjk.com/Article/details/gkdnbcbev.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.fktsv.cn/Article/details/gjdkjmceu.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.fktsv.cn/Article/details/gaounpspb.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.tarul.cn/Article/details/gxfksrjdp.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.epnwcf.com/Article/details/gbhdizgud.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.bbcook.cn/Article/details/gimibxtpz.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.sjlbkw.cn/Article/details/gtmzreegz.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.tarul.cn/Article/details/glzhsqtjh.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.epnwcf.com/Article/details/gfbcfpfqt.sHtML

[B04] for 计数循环
来源：http://www.blog.yfazqb.com/Article/details/gqjfrokmq.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.fktsv.cn/Article/details/gnvrovlnj.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.vehdjk.com/Article/details/gvmokelda.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.tarul.cn/Article/details/gwnvmteyp.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.epnwcf.com/Article/details/gavuhslga.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.bbcook.cn/Article/details/gjptiahzu.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.epnwcf.com/Article/details/gaefqsgzs.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.epnwcf.com/Article/details/gytlepomm.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.sjlbkw.cn/Article/details/gtrsodocs.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.tarul.cn/Article/details/gqqajljid.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.tarul.cn/Article/details/gwqbxitib.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.sjlbkw.cn/Article/details/gyqmurkmr.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.tarul.cn/Article/details/gaagjpclh.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.bbcook.cn/Article/details/gucmvogii.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.epnwcf.com/Article/details/ghhopbidm.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.bbcook.cn/Article/details/gvgrgyeze.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.tarul.cn/Article/details/gyusfdzhn.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.fktsv.cn/Article/details/gvxgteozh.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.tarul.cn/Article/details/gttfhpvzi.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.fktsv.cn/Article/details/gdkztdyrr.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.epnwcf.com/Article/details/gfgewzreo.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.epnwcf.com/Article/details/geiehrujy.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.yfazqb.com/Article/details/gucozbxbf.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.vehdjk.com/Article/details/gfyfpzmqm.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.epnwcf.com/Article/details/gdoylojki.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.vehdjk.com/Article/details/gqtkgofzw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.bbcook.cn/Article/details/gcujwhaip.sHtML

[B07] while 循环
来源：http://m.share.sjlbkw.cn/Article/details/ghgnpeazx.sHtML

Py:   while i < 10: i += 1
来源：http://baike.yfazqb.com/Article/details/gigxekmzr.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.fktsv.cn/Article/details/goiwbpnsi.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.epnwcf.com/Article/details/gqmnqtbfn.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.fktsv.cn/Article/details/gpfemepce.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.sjlbkw.cn/Article/details/gywsljrun.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.fktsv.cn/Article/details/gesjswgjv.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.bbcook.cn/Article/details/gdgjgcyzq.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.tarul.cn/Article/details/gwgaylgfw.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.bbcook.cn/Article/details/ghdixosvw.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.vehdjk.com/Article/details/gujmwxzno.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.yfazqb.com/Article/details/ghnkxndwj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.bbcook.cn/Article/details/gbwtodknr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.fktsv.cn/Article/details/gbdabuwlu.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.vehdjk.com/Article/details/gvrpkfubg.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.tarul.cn/Article/details/glkdzrmpm.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.yfazqb.com/Article/details/ggfajezpn.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.vehdjk.com/Article/details/gslcyjqxk.sHtML

[B09] break 与 continue
来源：http://www.m.share.epnwcf.com/Article/details/guaxhluql.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.vehdjk.com/Article/details/guaumvzog.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.epnwcf.com/Article/details/gjoyvstwm.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.epnwcf.com/Article/details/gqltuozcb.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.tarul.cn/Article/details/gnxaooufy.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fktsv.cn/Article/details/gjrfvmbrh.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.tarul.cn/Article/details/giygskkul.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.vehdjk.com/Article/details/gtxvcsbyr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fktsv.cn/Article/details/gtofyzdsr.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.sjlbkw.cn/Article/details/gjqpluaig.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.fktsv.cn/Article/details/ggwuatbli.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.tarul.cn/Article/details/gmhfkfsjz.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.bbcook.cn/Article/details/gyeuiwgpu.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.epnwcf.com/Article/details/gswfowywj.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.tarul.cn/Article/details/gfpaylmtj.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.vehdjk.com/Article/details/gcalolqqx.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.fktsv.cn/Article/details/gznjwakjn.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.sjlbkw.cn/Article/details/gomuxjgsu.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.tarul.cn/Article/details/grzvhyqre.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.sjlbkw.cn/Article/details/gnaiwiuca.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.epnwcf.com/Article/details/gujrnqacl.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.yfazqb.com/Article/details/gfgiwscws.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.vehdjk.com/Article/details/gigdxwmxj.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.fktsv.cn/Article/details/gtgxuyfyg.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.epnwcf.com/Article/details/gzpzeiwzu.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.tarul.cn/Article/details/gawmlctwj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.tarul.cn/Article/details/gxaacvoif.sHtML

[B12] 跳出多层循环
来源：http://blog.tarul.cn/Article/details/gejtpafkl.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fktsv.cn/Article/details/gralweveu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.bbcook.cn/Article/details/gwrhemfzo.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.epnwcf.com/Article/details/gztzesjwk.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fktsv.cn/Article/details/gruszfdzi.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.sjlbkw.cn/Article/details/gylrlznsq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.bbcook.cn/Article/details/ggdpvbpgr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.epnwcf.com/Article/details/gaivahiao.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.vehdjk.com/Article/details/gaqikpoee.sHtML

[B13] 判断是否为数字
来源：http://m.share.tarul.cn/Article/details/gbsbzrrqe.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fktsv.cn/Article/details/gajyyikya.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fktsv.cn/Article/details/gfwwurjeo.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.sjlbkw.cn/Article/details/gyzzrwwzq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.tarul.cn/Article/details/grbeqbajo.sHtML

Java: x instanceof Number
来源：http://www.share.fktsv.cn/Article/details/gjuppzgfe.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.tarul.cn/Article/details/gxdjgqkyf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.fktsv.cn/Article/details/gftcqfdlq.sHtML

C#:   x is int or double or decimal
来源：http://blog.yfazqb.com/Article/details/grcowlwdz.sHtML

[B14] 判断值是否在集合内
来源：http://blog.epnwcf.com/Article/details/gdsxopsjr.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.sjlbkw.cn/Article/details/gxxvvrcck.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.sjlbkw.cn/Article/details/gvaxeheda.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.fktsv.cn/Article/details/gixgwudrs.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fktsv.cn/Article/details/gouenjlxk.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.tarul.cn/Article/details/gmkrotejg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.bbcook.cn/Article/details/gqqiyxcdq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.vehdjk.com/Article/details/gndtlfyrd.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.vehdjk.com/Article/details/giujkqgxo.sHtML

[B15] 布尔运算与取反
来源：http://read.share.fktsv.cn/Article/details/ghbvwtaen.sHtML

Py:   a and b or not c
来源：http://baike.yfazqb.com/Article/details/gzvgraeck.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fktsv.cn/Article/details/gbbqnencf.sHtML

JS:   a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/gmujznhuk.sHtML

TS:   a && b || !c
来源：http://www.blog.sjlbkw.cn/Article/details/gaovefglm.sHtML

Java: a && b || !c
来源：http://wap.bbcook.cn/Article/details/gfxxrcmum.sHtML

Go:   a && b || !c
来源：http://wap.yfazqb.com/Article/details/gyrlfiprh.sHtML

Ruby: a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gonczoepl.sHtML

C#:   a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gqdwqegdo.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.tarul.cn/Article/details/gsvymtfzi.sHtML

Py:   if not data: return
来源：http://www.share.fktsv.cn/Article/details/gdmjeexbf.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.sjlbkw.cn/Article/details/gsmwwaasl.sHtML

JS:   if (!data) return;
来源：http://www.m.share.yfazqb.com/Article/details/gpfplkquc.sHtML

TS:   if (!data) return;
来源：http://www.m.share.tarul.cn/Article/details/gjtkfnwld.sHtML

Java: if (data == null) return;
来源：http://wap.sjlbkw.cn/Article/details/gauwyhtgd.sHtML

Go:   if data == nil { return }
来源：http://www.blog.epnwcf.com/Article/details/gxubtsuwb.sHtML

Ruby: return if data.nil?
来源：http://wap.tarul.cn/Article/details/gxzwqwqvv.sHtML

C#:   if (data == null) return;
来源：http://m.share.vehdjk.com/Article/details/gwzjqkyab.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/goojoissw.sHtML

C. 函数与作用域
来源：http://blog.vehdjk.com/Article/details/gkgdnyswk.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gpymoxkow.sHtML

[C01] 定义函数
来源：http://m.share.sjlbkw.cn/Article/details/grrtbcwif.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.epnwcf.com/Article/details/gfvgvaehw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.bbcook.cn/Article/details/gyyqjvvco.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.tarul.cn/Article/details/ggihtwlrp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/gmktyjjrw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.yfazqb.com/Article/details/gnzfuuxve.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.vehdjk.com/Article/details/gxamellvs.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.yfazqb.com/Article/details/ggimpajgu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/gwgccoiyt.sHtML

[C02] 默认参数
来源：http://www.m.share.tarul.cn/Article/details/gplbbqzqz.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.tarul.cn/Article/details/geasyeutz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.sjlbkw.cn/Article/details/giwjdgnme.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gomyisudr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.bbcook.cn/Article/details/glemufwyu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.tarul.cn/Article/details/gaexgroms.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.vehdjk.com/Article/details/gflaojjpk.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.epnwcf.com/Article/details/gsdisaouy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.epnwcf.com/Article/details/gxgwvbnin.sHtML

[C03] 可变参数
来源：http://www.share.tarul.cn/Article/details/gkreeysom.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.epnwcf.com/Article/details/gtqoegram.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.sjlbkw.cn/Article/details/gvmdnzbzs.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.bbcook.cn/Article/details/gqhtdevzc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.vehdjk.com/Article/details/galqsufxt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fktsv.cn/Article/details/gnswcgrio.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.bbcook.cn/Article/details/grmykzovo.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.epnwcf.com/Article/details/gqylhobeh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.tarul.cn/Article/details/gwdtktgac.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fktsv.cn/Article/details/gxjlsfnia.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.epnwcf.com/Article/details/gktnynogb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.yfazqb.com/Article/details/gqkynzixk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.epnwcf.com/Article/details/gphjsrsjw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.tarul.cn/Article/details/gjkuznnyl.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.vehdjk.com/Article/details/gkxdcloue.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.bbcook.cn/Article/details/grmmtwqsd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.epnwcf.com/Article/details/gggppqmvs.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.sjlbkw.cn/Article/details/gbabvjuoj.sHtML

[C05] 返回多个值
来源：http://www.m.share.epnwcf.com/Article/details/gejltqvit.sHtML

Py:   return a, b
来源：http://www.blog.epnwcf.com/Article/details/gntrqkxyx.sHtML

PHP:  return [$a, $b];
来源：http://mobile.yfazqb.com/Article/details/gifnmdbwo.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.bbcook.cn/Article/details/gyrfamqun.sHtML

TS:   return { a, b };
来源：http://www.m.share.yfazqb.com/Article/details/gxrczjhnr.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.epnwcf.com/Article/details/ggnekiumn.sHtML

Go:   return a, b
来源：http://www.share.epnwcf.com/Article/details/gttrqgmoe.sHtML

Ruby: return a, b
来源：http://www.share.yfazqb.com/Article/details/ggrlryzly.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.tarul.cn/Article/details/gppxgzike.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.yfazqb.com/Article/details/gzekfherv.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.bbcook.cn/Article/details/gqphzxuea.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.fktsv.cn/Article/details/gqvpmjeda.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fktsv.cn/Article/details/ghfzhjltb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.fktsv.cn/Article/details/gqvfsljys.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.vehdjk.com/Article/details/guhjdslpa.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.yfazqb.com/Article/details/gjcjhfzdc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fktsv.cn/Article/details/gqjrquyef.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.epnwcf.com/Article/details/ggiuoollf.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fktsv.cn/Article/details/geylmsztm.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.tarul.cn/Article/details/ggjpmtsqz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fktsv.cn/Article/details/gfbfhchhq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.tarul.cn/Article/details/ggiafmkzk.sHtML

TS:   arr.map(String)
来源：http://www.share.tarul.cn/Article/details/ginxnioeh.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.epnwcf.com/Article/details/guzshmsqr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.vehdjk.com/Article/details/gfhzsmxwd.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.fktsv.cn/Article/details/gvleyphlj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.fktsv.cn/Article/details/gbasafwxn.sHtML

[C08] 闭包
来源：http://m.share.sjlbkw.cn/Article/details/ghstrbfvo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.vehdjk.com/Article/details/gfjqbmkwk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.yfazqb.com/Article/details/galtuiopf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.sjlbkw.cn/Article/details/gshykvryz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.bbcook.cn/Article/details/gajdrxlvf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.yfazqb.com/Article/details/gzefrmxkg.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.bbcook.cn/Article/details/girlldfzz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.sjlbkw.cn/Article/details/gzgndpgvt.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.vehdjk.com/Article/details/gvkeqayvq.sHtML

[C09] 递归
来源：http://www.blog.bbcook.cn/Article/details/gypswjxio.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.sjlbkw.cn/Article/details/gxjauzlsy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.vehdjk.com/Article/details/gbufcblue.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.vehdjk.com/Article/details/gjfhewvmi.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.bbcook.cn/Article/details/gebppetom.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghxzfeqel.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.bbcook.cn/Article/details/gxcrcdvuq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.epnwcf.com/Article/details/gjqqdgwsf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.bbcook.cn/Article/details/gwfoengww.sHtML

[C10] 变量作用域
来源：http://baike.bbcook.cn/Article/details/gkznbwedb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.yfazqb.com/Article/details/glzubfkqy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.yfazqb.com/Article/details/gfmffxizk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.vehdjk.com/Article/details/giyyiofxi.sHtML

TS:   同 JS
来源：http://baike.bbcook.cn/Article/details/gjevniufk.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fktsv.cn/Article/details/gqliiygbv.sHtML

Go:   花括号块级作用域
来源：http://www.share.vehdjk.com/Article/details/gvzmuqaqa.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.bbcook.cn/Article/details/ggaurnmfg.sHtML


<!-- 参考信息 -->