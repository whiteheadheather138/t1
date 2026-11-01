代发 wailian999

Ruby: a, b = b, a
来源：http://baike.epnwcf.com/Article/details/giszgmksi.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.epnwcf.com/Article/details/ghzgtrijw.sHtML

[A20] 读取标准输入
来源：http://www.m.share.bbcook.cn/Article/details/gjqvdtrmk.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.bbcook.cn/Article/details/gctcjqrqy.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.vehdjk.com/Article/details/gybcmadir.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.yfazqb.com/Article/details/gfwipoqwl.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.vehdjk.com/Article/details/gkwomuarl.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.bbcook.cn/Article/details/gudckjmeg.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.yfazqb.com/Article/details/gaprwnqua.sHtML

Ruby: gets.chomp
来源：http://baike.yfazqb.com/Article/details/gralalotx.sHtML

C#:   Console.ReadLine();
来源：http://baike.yfazqb.com/Article/details/geqbqeavi.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.bbcook.cn/Article/details/gwqyuuehc.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.sjlbkw.cn/Article/details/gxauthytn.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.bbcook.cn/Article/details/gnmsmhjly.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.bbcook.cn/Article/details/gywzupsmk.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.yfazqb.com/Article/details/ghzretilp.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.sjlbkw.cn/Article/details/gkolnilpc.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.epnwcf.com/Article/details/gkmbgbmki.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.fktsv.cn/Article/details/gtwiebuvl.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.sjlbkw.cn/Article/details/ghkzckmln.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.fktsv.cn/Article/details/gujknaura.sHtML

Py:   len(s)
来源：http://blog.epnwcf.com/Article/details/geghmngit.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.vehdjk.com/Article/details/gseaxfvcr.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.vehdjk.com/Article/details/gsutzwvfs.sHtML

TS:   s.length
来源：http://mobile.tarul.cn/Article/details/ghvfywnsc.sHtML

Java: s.length()
来源：http://wap.sjlbkw.cn/Article/details/gyjgiaizs.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.bbcook.cn/Article/details/gqouyspwf.sHtML

Ruby: s.length
来源：http://baike.vehdjk.com/Article/details/gucghdrse.sHtML

C#:   s.Length
来源：http://baike.yfazqb.com/Article/details/ghwrnfzhz.sHtML

[A23] 大小写转换
来源：http://read.share.sjlbkw.cn/Article/details/gtsibyfiq.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.tarul.cn/Article/details/guobbdpkl.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.bbcook.cn/Article/details/gfhqkhzjy.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.yfazqb.com/Article/details/gbxvfqvwr.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.sjlbkw.cn/Article/details/grtyyvion.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.yfazqb.com/Article/details/golclclqm.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.yfazqb.com/Article/details/gmpvcumdg.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.fktsv.cn/Article/details/gqnebmqgz.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.fktsv.cn/Article/details/glsvtrmgy.sHtML

[A24] 去除首尾空白
来源：http://www.blog.vehdjk.com/Article/details/gamvovisz.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.yfazqb.com/Article/details/ghznvxwzd.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.sjlbkw.cn/Article/details/gjdgzauck.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fktsv.cn/Article/details/gqkiyzllo.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.sjlbkw.cn/Article/details/glbhvtial.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.tarul.cn/Article/details/gglogordt.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.epnwcf.com/Article/details/gdiezfiac.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.epnwcf.com/Article/details/gsdfgcxre.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.yfazqb.com/Article/details/gdbfirpwo.sHtML

[A25] 字符串比较
来源：http://www.m.share.yfazqb.com/Article/details/gcnpxiooi.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.bbcook.cn/Article/details/glpprdsng.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.yfazqb.com/Article/details/gdqiimyix.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.yfazqb.com/Article/details/geulrinvj.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.epnwcf.com/Article/details/gwxltwuow.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.epnwcf.com/Article/details/grvvzxpvd.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.epnwcf.com/Article/details/grxwkvxdb.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.epnwcf.com/Article/details/ggepwbvza.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.fktsv.cn/Article/details/gbfbcosno.sHtML

[A26] 类型转换总览
来源：http://read.share.sjlbkw.cn/Article/details/geqviquyn.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.bbcook.cn/Article/details/gxkhnligc.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.yfazqb.com/Article/details/gzgwyfxnm.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.bbcook.cn/Article/details/getzpbllf.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.fktsv.cn/Article/details/gjyuorndy.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.vehdjk.com/Article/details/gygiqwydg.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.fktsv.cn/Article/details/gughfbrdb.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.yfazqb.com/Article/details/gibanhcsh.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.fktsv.cn/Article/details/gxkamsgar.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gcgqerldi.sHtML

B. 流程控制
来源：http://mobile.bbcook.cn/Article/details/gkfvwsmgy.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/ggddnqwvc.sHtML

[B01] 条件判断 if / else
来源：http://blog.tarul.cn/Article/details/gfasdvcow.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.vehdjk.com/Article/details/gupbvmgvw.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.yfazqb.com/Article/details/gzdkkgrst.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.yfazqb.com/Article/details/gloctzhgr.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.bbcook.cn/Article/details/gobwrwlfk.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.bbcook.cn/Article/details/gitoxlnkc.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.yfazqb.com/Article/details/gsztspqtd.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.tarul.cn/Article/details/godpstsew.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.fktsv.cn/Article/details/gqclvcmzx.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.tarul.cn/Article/details/gmlsogmuj.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.tarul.cn/Article/details/ghbrgoagz.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.vehdjk.com/Article/details/gnzszkxlt.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fktsv.cn/Article/details/gpgnwbovy.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.vehdjk.com/Article/details/gjaquwult.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.bbcook.cn/Article/details/ggwiumese.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.sjlbkw.cn/Article/details/gszeeqrqr.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.yfazqb.com/Article/details/gwtwdflve.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.bbcook.cn/Article/details/gjwkjaabx.sHtML

[B03] switch / match / case
来源：http://wap.tarul.cn/Article/details/ggykippza.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.bbcook.cn/Article/details/grgjhikap.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.fktsv.cn/Article/details/gbcppqeaz.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.sjlbkw.cn/Article/details/gvxvbkjvj.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.fktsv.cn/Article/details/gzlycartz.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.tarul.cn/Article/details/ghtwsecdn.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.yfazqb.com/Article/details/gwkkhwifh.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.yfazqb.com/Article/details/gpxxbszhd.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.epnwcf.com/Article/details/gcbpiumwm.sHtML

[B04] for 计数循环
来源：http://www.blog.vehdjk.com/Article/details/giotfnhmz.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.epnwcf.com/Article/details/gbcngtwzd.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.epnwcf.com/Article/details/gwktdfjnl.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.epnwcf.com/Article/details/gmnkdoulp.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.epnwcf.com/Article/details/guyjpqriy.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.yfazqb.com/Article/details/gdizkngpt.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.tarul.cn/Article/details/grhyljzkn.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.tarul.cn/Article/details/gwikceuss.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.fktsv.cn/Article/details/gjfcvbnpt.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.sjlbkw.cn/Article/details/gfkkrtcds.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.tarul.cn/Article/details/gxulmfjcf.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.tarul.cn/Article/details/gagmvjbwd.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.bbcook.cn/Article/details/gsjdjhcya.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.yfazqb.com/Article/details/gqekazsxr.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.yfazqb.com/Article/details/gzzefgwji.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.bbcook.cn/Article/details/ggbhmbsbo.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.fktsv.cn/Article/details/gfihxiljh.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.vehdjk.com/Article/details/gyzinjchk.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.sjlbkw.cn/Article/details/gmtbfjhuc.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.fktsv.cn/Article/details/gscpcckui.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.vehdjk.com/Article/details/gmoriprnr.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.vehdjk.com/Article/details/gqzkmmbrm.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.tarul.cn/Article/details/gxiydrgbc.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.bbcook.cn/Article/details/gkdymeosv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.epnwcf.com/Article/details/gsshwnkbm.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.vehdjk.com/Article/details/glqcxdebw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.epnwcf.com/Article/details/gwpcwkume.sHtML

[B07] while 循环
来源：http://3g.bbcook.cn/Article/details/gfdjxrbzw.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.yfazqb.com/Article/details/gnvnrwvhs.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.fktsv.cn/Article/details/girvedgks.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.fktsv.cn/Article/details/gtrcqjivp.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.tarul.cn/Article/details/gauzdzxvv.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.fktsv.cn/Article/details/gtshptdem.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.vehdjk.com/Article/details/gsldcdmzv.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.yfazqb.com/Article/details/gzehpyvzm.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.sjlbkw.cn/Article/details/gzojujabh.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.sjlbkw.cn/Article/details/gkhlhrdnr.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.sjlbkw.cn/Article/details/goqwpfuja.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.bbcook.cn/Article/details/genqcemyt.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.fktsv.cn/Article/details/garmwsbwd.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.tarul.cn/Article/details/gpswfiijw.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.epnwcf.com/Article/details/gvaowxjrw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.fktsv.cn/Article/details/gimxyumdk.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.yfazqb.com/Article/details/ghimvlegv.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.fktsv.cn/Article/details/gmnednhjv.sHtML

[B09] break 与 continue
来源：http://mobile.tarul.cn/Article/details/gvpsbwqwf.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.tarul.cn/Article/details/gkbvwajyl.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.sjlbkw.cn/Article/details/gmylyygxm.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.epnwcf.com/Article/details/gicrladmf.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/gimtcjdza.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.sjlbkw.cn/Article/details/gbcohioqy.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.fktsv.cn/Article/details/gyqsutbsd.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.yfazqb.com/Article/details/gqpuqmmmf.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.tarul.cn/Article/details/gvaydctwf.sHtML

[B10] 遍历同时拿索引
来源：http://wap.yfazqb.com/Article/details/groxhgzuk.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.yfazqb.com/Article/details/gfqjhiznh.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.fktsv.cn/Article/details/glxnpaccc.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.yfazqb.com/Article/details/gdfnwufqo.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.epnwcf.com/Article/details/gxrjxizbx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.epnwcf.com/Article/details/gfxhgrkvj.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.sjlbkw.cn/Article/details/gajvtbezv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.vehdjk.com/Article/details/gzmyrvoun.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.yfazqb.com/Article/details/gntzipabp.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.fktsv.cn/Article/details/gumesalbn.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.bbcook.cn/Article/details/gclmgcljw.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.vehdjk.com/Article/details/gvrdxdthk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fktsv.cn/Article/details/guzczeghn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.tarul.cn/Article/details/gupjfdxsc.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.tarul.cn/Article/details/gshxhfziq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.fktsv.cn/Article/details/gvheieugx.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.yfazqb.com/Article/details/gaxdzqdal.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.yfazqb.com/Article/details/gqdkcxkyu.sHtML

[B12] 跳出多层循环
来源：http://baike.bbcook.cn/Article/details/ggbwlroed.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.yfazqb.com/Article/details/gykncjkeu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.sjlbkw.cn/Article/details/gqajybjsq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.epnwcf.com/Article/details/gfhulkang.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fktsv.cn/Article/details/gbyflweoz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.vehdjk.com/Article/details/gvnwrtbzt.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.bbcook.cn/Article/details/gzbymxtkh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.epnwcf.com/Article/details/gflhxukob.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.bbcook.cn/Article/details/ghfaaxpbw.sHtML

[B13] 判断是否为数字
来源：http://baike.bbcook.cn/Article/details/ghavwcevv.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.tarul.cn/Article/details/gchepyixd.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fktsv.cn/Article/details/gwyjzquem.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.vehdjk.com/Article/details/gojqyurcp.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.epnwcf.com/Article/details/gbmnkqroy.sHtML

Java: x instanceof Number
来源：http://wap.yfazqb.com/Article/details/gwfimbxzd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.bbcook.cn/Article/details/glwlbzywg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.epnwcf.com/Article/details/ghrqncwmr.sHtML

C#:   x is int or double or decimal
来源：http://blog.epnwcf.com/Article/details/gjmgnqtuz.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.yfazqb.com/Article/details/gsuqmzbpf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.sjlbkw.cn/Article/details/gaecyiisf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.tarul.cn/Article/details/gtxkmmokg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.bbcook.cn/Article/details/gcqznfobs.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.vehdjk.com/Article/details/gkznzkyhr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.tarul.cn/Article/details/grvcycefx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.epnwcf.com/Article/details/gzlgxuoag.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.vehdjk.com/Article/details/gafdhdzhz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.vehdjk.com/Article/details/gpknsrjxt.sHtML

[B15] 布尔运算与取反
来源：http://www.share.epnwcf.com/Article/details/grnjooyog.sHtML

Py:   a and b or not c
来源：http://www.blog.vehdjk.com/Article/details/gyxhidkgx.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.epnwcf.com/Article/details/gkeimoqrk.sHtML

JS:   a && b || !c
来源：http://wap.epnwcf.com/Article/details/gnwnurvkl.sHtML

TS:   a && b || !c
来源：http://wap.bbcook.cn/Article/details/gwxwtauae.sHtML

Java: a && b || !c
来源：http://read.share.yfazqb.com/Article/details/glzdvoejh.sHtML

Go:   a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/gwhcnuyfr.sHtML

Ruby: a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gucajpgvl.sHtML

C#:   a && b || !c
来源：http://www.blog.tarul.cn/Article/details/girtiwskw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.tarul.cn/Article/details/gajxxqxny.sHtML

Py:   if not data: return
来源：http://m.share.fktsv.cn/Article/details/gmlegvmsv.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.tarul.cn/Article/details/gpyqcoqcm.sHtML

JS:   if (!data) return;
来源：http://www.blog.epnwcf.com/Article/details/gxwwqbyyj.sHtML

TS:   if (!data) return;
来源：http://www.blog.vehdjk.com/Article/details/gnxqdoisg.sHtML

Java: if (data == null) return;
来源：http://blog.sjlbkw.cn/Article/details/gdlgdancr.sHtML

Go:   if data == nil { return }
来源：http://read.share.epnwcf.com/Article/details/gjwbatzfh.sHtML

Ruby: return if data.nil?
来源：http://read.share.epnwcf.com/Article/details/gmrfxaimc.sHtML

C#:   if (data == null) return;
来源：http://mobile.bbcook.cn/Article/details/gfbtxidcq.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gmpukvdwg.sHtML

C. 函数与作用域
来源：http://www.blog.yfazqb.com/Article/details/gezhygqzb.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gihnrnuyc.sHtML

[C01] 定义函数
来源：http://mobile.vehdjk.com/Article/details/gckzoqqas.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.tarul.cn/Article/details/grphszmya.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.epnwcf.com/Article/details/gxofupfjn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gxojhlxgl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/ghqjxhfht.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/geklawfhc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.vehdjk.com/Article/details/govxylifc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.epnwcf.com/Article/details/gwsfzyank.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/gqqsyuzwb.sHtML

[C02] 默认参数
来源：http://wap.tarul.cn/Article/details/gyopypsrx.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.vehdjk.com/Article/details/gellpxtfp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.bbcook.cn/Article/details/ghnnmysvx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.yfazqb.com/Article/details/ggupigpla.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.yfazqb.com/Article/details/gebrpyynr.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fktsv.cn/Article/details/goeiqnben.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fktsv.cn/Article/details/gnhkrwmpt.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.sjlbkw.cn/Article/details/gohtxzktj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.fktsv.cn/Article/details/ghpbdhtew.sHtML

[C03] 可变参数
来源：http://mobile.tarul.cn/Article/details/gmzssgemk.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.vehdjk.com/Article/details/ghypeycov.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.yfazqb.com/Article/details/gznbgcynz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fktsv.cn/Article/details/gpmudgeal.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.yfazqb.com/Article/details/grlrphpbu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.yfazqb.com/Article/details/gohjbpymi.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.yfazqb.com/Article/details/gwgfvugmt.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gbitdmomw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.tarul.cn/Article/details/ghrukhytq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.epnwcf.com/Article/details/gnxqyvnfw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.tarul.cn/Article/details/glpkrlumk.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.vehdjk.com/Article/details/gexyiqpwn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.yfazqb.com/Article/details/glfpndgxh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.sjlbkw.cn/Article/details/gdvojurai.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fktsv.cn/Article/details/gmdrqmedz.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.epnwcf.com/Article/details/gedrkuatp.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.vehdjk.com/Article/details/gvuhwoqmr.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fktsv.cn/Article/details/grahtplna.sHtML

[C05] 返回多个值
来源：http://wap.sjlbkw.cn/Article/details/gtnhfrypf.sHtML

Py:   return a, b
来源：http://mobile.tarul.cn/Article/details/ghxyixvot.sHtML

PHP:  return [$a, $b];
来源：http://blog.sjlbkw.cn/Article/details/gebawlafx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.sjlbkw.cn/Article/details/gllvdbktn.sHtML

TS:   return { a, b };
来源：http://read.share.bbcook.cn/Article/details/gdzclegsg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.tarul.cn/Article/details/gqsluxogh.sHtML

Go:   return a, b
来源：http://baike.vehdjk.com/Article/details/gkdfsljuj.sHtML

Ruby: return a, b
来源：http://read.share.sjlbkw.cn/Article/details/gacbpsgsx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.sjlbkw.cn/Article/details/gavsiqnhz.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.fktsv.cn/Article/details/gauvjsson.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.bbcook.cn/Article/details/ggtrrgrcy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.tarul.cn/Article/details/gvxozksvf.sHtML

JS:   const square = x => x * x;
来源：http://read.share.sjlbkw.cn/Article/details/ghsbmfunt.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.yfazqb.com/Article/details/gazelcolk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.vehdjk.com/Article/details/gzpvgtwzo.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.yfazqb.com/Article/details/gczicjjta.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.epnwcf.com/Article/details/gcyjipnbc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.sjlbkw.cn/Article/details/gitbdtxcu.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fktsv.cn/Article/details/gcppkktum.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fktsv.cn/Article/details/gorypsmok.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.sjlbkw.cn/Article/details/gmckaejpm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fktsv.cn/Article/details/gxjfspbzi.sHtML

TS:   arr.map(String)
来源：http://read.share.fktsv.cn/Article/details/goviegewg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.bbcook.cn/Article/details/gdyspimqi.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fktsv.cn/Article/details/gwrljzizy.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.tarul.cn/Article/details/gjxgrvfav.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.yfazqb.com/Article/details/gijaykian.sHtML

[C08] 闭包
来源：http://m.share.bbcook.cn/Article/details/gdsprnali.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.epnwcf.com/Article/details/glpzqlxgh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.sjlbkw.cn/Article/details/gvuxqzhim.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.yfazqb.com/Article/details/gjophooyf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.sjlbkw.cn/Article/details/guqehiequ.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.tarul.cn/Article/details/gnsvewwkx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.tarul.cn/Article/details/gkjalucfv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.yfazqb.com/Article/details/gvptwggcj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.epnwcf.com/Article/details/gajnanzey.sHtML

[C09] 递归
来源：http://blog.vehdjk.com/Article/details/gjrujqscl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.epnwcf.com/Article/details/gtrlmmfow.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fktsv.cn/Article/details/gvldnpqdp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.epnwcf.com/Article/details/gpmzqgsrm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.yfazqb.com/Article/details/gpsipdnmg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.epnwcf.com/Article/details/grkeaccyz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.yfazqb.com/Article/details/gkjbifqwp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fktsv.cn/Article/details/gictkfiya.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.epnwcf.com/Article/details/gnmmkojug.sHtML

[C10] 变量作用域
来源：http://m.share.epnwcf.com/Article/details/gxkgocbdf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.bbcook.cn/Article/details/gisiusupe.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fktsv.cn/Article/details/gsoejaiau.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.vehdjk.com/Article/details/grmguwsss.sHtML


<!-- 参考信息 -->