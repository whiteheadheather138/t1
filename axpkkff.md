代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://baike.yfazqb.com/Article/details/gxhgcyyji.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.fktsv.cn/Article/details/gkyrfapds.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.fktsv.cn/Article/details/gyymujnjv.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.yfazqb.com/Article/details/gaahsvcem.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.bbcook.cn/Article/details/gmeyzwggk.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.m.share.sjlbkw.cn/Article/details/gjrirnzpx.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.tarul.cn/Article/details/gpieiirwq.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.yfazqb.com/Article/details/gaorhalzr.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.epnwcf.com/Article/details/guvpolebe.sHtML

[A19] 交换两个变量
来源：http://blog.vehdjk.com/Article/details/gccqjuski.sHtML

Py:   a, b = b, a
来源：http://blog.tarul.cn/Article/details/gejbubapd.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.yfazqb.com/Article/details/gwfcdybct.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.vehdjk.com/Article/details/ghskgibpb.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.sjlbkw.cn/Article/details/guenrrdak.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.tarul.cn/Article/details/glabzqttb.sHtML

Go:   a, b = b, a
来源：http://m.share.fktsv.cn/Article/details/gbffcytmm.sHtML

Ruby: a, b = b, a
来源：http://baike.yfazqb.com/Article/details/ghlejnuvu.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.epnwcf.com/Article/details/gwukkxeti.sHtML

[A20] 读取标准输入
来源：http://www.share.epnwcf.com/Article/details/giyekutiw.sHtML

Py:   name = input("请输入：")
来源：http://read.share.vehdjk.com/Article/details/ggnryltfp.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.tarul.cn/Article/details/gxrcdzcrl.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.vehdjk.com/Article/details/gwhxvmwic.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.epnwcf.com/Article/details/ggpdeoohc.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.bbcook.cn/Article/details/gdpsterol.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.epnwcf.com/Article/details/gnosimsid.sHtML

Ruby: gets.chomp
来源：http://read.share.bbcook.cn/Article/details/gqfclznxc.sHtML

C#:   Console.ReadLine();
来源：http://blog.epnwcf.com/Article/details/gczlxeiip.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.vehdjk.com/Article/details/gsnjnwcgn.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.fktsv.cn/Article/details/gmbsqxuqo.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.epnwcf.com/Article/details/gdaigmgmx.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.bbcook.cn/Article/details/gixwdnann.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.bbcook.cn/Article/details/gzkviovsv.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.sjlbkw.cn/Article/details/gemrrsuap.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.bbcook.cn/Article/details/gpsluhiuq.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.yfazqb.com/Article/details/gpnqkzgxm.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.vehdjk.com/Article/details/gqvjverss.sHtML

[A22] 获取字符串长度
来源：http://baike.yfazqb.com/Article/details/gfncjqxeb.sHtML

Py:   len(s)
来源：http://m.share.epnwcf.com/Article/details/gthoqtxzz.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.yfazqb.com/Article/details/gzpnnstmp.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.bbcook.cn/Article/details/gegssnkvt.sHtML

TS:   s.length
来源：http://blog.tarul.cn/Article/details/gxyfrrdtm.sHtML

Java: s.length()
来源：http://blog.epnwcf.com/Article/details/gsajfdmbk.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.yfazqb.com/Article/details/grxtzsdme.sHtML

Ruby: s.length
来源：http://wap.epnwcf.com/Article/details/gszogahuu.sHtML

C#:   s.Length
来源：http://read.share.sjlbkw.cn/Article/details/gmkmjjiqk.sHtML

[A23] 大小写转换
来源：http://mobile.vehdjk.com/Article/details/gppgggfgc.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.vehdjk.com/Article/details/gnblwslac.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.bbcook.cn/Article/details/gmcgoskaw.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.sjlbkw.cn/Article/details/gwwsnpxdx.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.sjlbkw.cn/Article/details/gtuwvukle.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.yfazqb.com/Article/details/gjqevngld.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.fktsv.cn/Article/details/gsxihhlff.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.sjlbkw.cn/Article/details/gipniidkz.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.epnwcf.com/Article/details/gbzbgzgvh.sHtML

[A24] 去除首尾空白
来源：http://read.share.yfazqb.com/Article/details/gfwobjkur.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.yfazqb.com/Article/details/gotnkgyls.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.sjlbkw.cn/Article/details/gryelbdog.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.bbcook.cn/Article/details/gkyomxnnz.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.epnwcf.com/Article/details/gtsfqyisq.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.tarul.cn/Article/details/gevvfjgta.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.vehdjk.com/Article/details/gsgbnsnvx.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.yfazqb.com/Article/details/gztfozawy.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.fktsv.cn/Article/details/gywwhicaf.sHtML

[A25] 字符串比较
来源：http://www.share.bbcook.cn/Article/details/gwnuysjpa.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.epnwcf.com/Article/details/gaqfauaqk.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.fktsv.cn/Article/details/gelrldswd.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.epnwcf.com/Article/details/gurewttwx.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.vehdjk.com/Article/details/ggmnsxvjr.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.vehdjk.com/Article/details/gnbevzjwc.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.epnwcf.com/Article/details/ggvkeeaox.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.tarul.cn/Article/details/gujelswuk.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.vehdjk.com/Article/details/gndouapor.sHtML

[A26] 类型转换总览
来源：http://mobile.epnwcf.com/Article/details/giisxyizy.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.tarul.cn/Article/details/gqrwucngf.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.bbcook.cn/Article/details/grkdakatt.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.epnwcf.com/Article/details/ghrxndooc.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.sjlbkw.cn/Article/details/geofukilx.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.epnwcf.com/Article/details/gqlxsbwqo.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.yfazqb.com/Article/details/gzyxqvzvc.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.vehdjk.com/Article/details/gnmvctpzm.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.fktsv.cn/Article/details/goxwuuetm.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gkurjqaza.sHtML

B. 流程控制
来源：http://www.blog.fktsv.cn/Article/details/gjwmxhfbb.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gkmpchaiq.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.fktsv.cn/Article/details/gagmvbygd.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.epnwcf.com/Article/details/gkbmoigmv.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.fktsv.cn/Article/details/gsqgblzwe.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.yfazqb.com/Article/details/gxsiesdeh.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.tarul.cn/Article/details/gignkgqyk.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.epnwcf.com/Article/details/gksmhqjtm.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.bbcook.cn/Article/details/glrvxzcvs.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.yfazqb.com/Article/details/gzvxsqzap.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.fktsv.cn/Article/details/gwlohnpes.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.vehdjk.com/Article/details/gsxqnbdap.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.tarul.cn/Article/details/gpzzocpmi.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.sjlbkw.cn/Article/details/gazezwdeh.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fktsv.cn/Article/details/glhovsdmj.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.yfazqb.com/Article/details/gbzlraior.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.bbcook.cn/Article/details/gddakppnq.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.yfazqb.com/Article/details/ghaqlaprn.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.tarul.cn/Article/details/gveeydzti.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.tarul.cn/Article/details/gfypagoqa.sHtML

[B03] switch / match / case
来源：http://www.share.bbcook.cn/Article/details/ghwvjkkuy.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.bbcook.cn/Article/details/gtlawjqpf.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.yfazqb.com/Article/details/gibvbhpxm.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.epnwcf.com/Article/details/gfxsmwtno.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.bbcook.cn/Article/details/gzkyznjgm.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.yfazqb.com/Article/details/gzlheteag.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.tarul.cn/Article/details/gogfopcoi.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.bbcook.cn/Article/details/gymoenamj.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.fktsv.cn/Article/details/gonprolre.sHtML

[B04] for 计数循环
来源：http://www.share.yfazqb.com/Article/details/gyduzvzzh.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.epnwcf.com/Article/details/gqlwhbptt.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.bbcook.cn/Article/details/gruphsvke.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.tarul.cn/Article/details/guzjuypmv.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fktsv.cn/Article/details/gydsvlmvw.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.bbcook.cn/Article/details/germxwyou.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.yfazqb.com/Article/details/gctahrhnr.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.vehdjk.com/Article/details/gldbboevq.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.bbcook.cn/Article/details/ghzixovri.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.epnwcf.com/Article/details/gacdpysyr.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.bbcook.cn/Article/details/gpjxpujvj.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.epnwcf.com/Article/details/gftdeljvm.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.sjlbkw.cn/Article/details/gidsvlyjs.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fktsv.cn/Article/details/gnvumppez.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.fktsv.cn/Article/details/gumalfxtc.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.bbcook.cn/Article/details/gupcpunln.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.vehdjk.com/Article/details/ghzzyrvzs.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.fktsv.cn/Article/details/gybjsiivt.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.epnwcf.com/Article/details/gjuivumpu.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.sjlbkw.cn/Article/details/gfqbinnxh.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.sjlbkw.cn/Article/details/gnotcybly.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.epnwcf.com/Article/details/gzerozcbr.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.vehdjk.com/Article/details/grkftghzz.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.bbcook.cn/Article/details/glfunzpwl.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.vehdjk.com/Article/details/gqruexvgs.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.vehdjk.com/Article/details/gvocktoxy.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.epnwcf.com/Article/details/gsnrgrgtl.sHtML

[B07] while 循环
来源：http://read.share.vehdjk.com/Article/details/giixjumrv.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.sjlbkw.cn/Article/details/gkrwymvhi.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.vehdjk.com/Article/details/gsqtnapuo.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.bbcook.cn/Article/details/gjfbgyujl.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.yfazqb.com/Article/details/gzqfexgcj.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.sjlbkw.cn/Article/details/gupntlvqj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.sjlbkw.cn/Article/details/gbkksnkul.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.tarul.cn/Article/details/ghjisgtwi.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.epnwcf.com/Article/details/gwctgqyxa.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.vehdjk.com/Article/details/gohunrhnw.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.sjlbkw.cn/Article/details/gdqdmhtus.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.bbcook.cn/Article/details/gzjxkpmxl.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.epnwcf.com/Article/details/gyufhiuox.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.yfazqb.com/Article/details/gakotmims.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.fktsv.cn/Article/details/gzmfctrnp.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.tarul.cn/Article/details/gitlosyiu.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.fktsv.cn/Article/details/gzllpneda.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.yfazqb.com/Article/details/gbuswdrlu.sHtML

[B09] break 与 continue
来源：http://baike.bbcook.cn/Article/details/gkmivbbfo.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.yfazqb.com/Article/details/gscwuoehc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.vehdjk.com/Article/details/gwwbsinvv.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fktsv.cn/Article/details/gwyssgxby.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.tarul.cn/Article/details/gkrtspxog.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.yfazqb.com/Article/details/gvdthawif.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fktsv.cn/Article/details/gmcbjcifu.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.tarul.cn/Article/details/gfzuoplao.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.bbcook.cn/Article/details/gmhqlorqw.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.fktsv.cn/Article/details/gbkksanln.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.fktsv.cn/Article/details/giiojvwct.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.fktsv.cn/Article/details/glndexnbv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.sjlbkw.cn/Article/details/gspshtwjj.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.fktsv.cn/Article/details/gvfszlylm.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.yfazqb.com/Article/details/gwgguhmxe.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.bbcook.cn/Article/details/gckckowbs.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.vehdjk.com/Article/details/gotapkwsb.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.sjlbkw.cn/Article/details/gazoflmae.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.vehdjk.com/Article/details/gusxwkudq.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.bbcook.cn/Article/details/gopcyrtnq.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.fktsv.cn/Article/details/gzgosqqkm.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.bbcook.cn/Article/details/gqwnhngmd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.epnwcf.com/Article/details/gghjrnufd.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.epnwcf.com/Article/details/gphnrqobq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.bbcook.cn/Article/details/gylgvcqyy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.sjlbkw.cn/Article/details/gftdfkxis.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.bbcook.cn/Article/details/gareqzvcb.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.sjlbkw.cn/Article/details/ghtcmfogr.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.bbcook.cn/Article/details/gggdjxuho.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.yfazqb.com/Article/details/gzfldqudf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fktsv.cn/Article/details/gurrawfuf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.yfazqb.com/Article/details/grldnrdup.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.tarul.cn/Article/details/gvbbtnxzb.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.bbcook.cn/Article/details/gqoxydnjv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.tarul.cn/Article/details/gnqurjmsj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.vehdjk.com/Article/details/gzbxugqji.sHtML

[B13] 判断是否为数字
来源：http://3g.yfazqb.com/Article/details/gjxwxawkp.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.bbcook.cn/Article/details/ggndtkvta.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.yfazqb.com/Article/details/gnftockbb.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.sjlbkw.cn/Article/details/gqjigqggu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gpirmftat.sHtML

Java: x instanceof Number
来源：http://www.m.share.epnwcf.com/Article/details/grvcjqnmy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.bbcook.cn/Article/details/gvxcclhwv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.tarul.cn/Article/details/gsmvuagdx.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.yfazqb.com/Article/details/glcszpxqg.sHtML

[B14] 判断值是否在集合内
来源：http://wap.yfazqb.com/Article/details/gublbahxn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fktsv.cn/Article/details/gebaqnamb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.vehdjk.com/Article/details/gwcaqshkg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.sjlbkw.cn/Article/details/gqcticbpi.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.bbcook.cn/Article/details/gafyyhdqa.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.sjlbkw.cn/Article/details/grykuqbxz.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.yfazqb.com/Article/details/guknfigrb.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.sjlbkw.cn/Article/details/gjzbceasv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.bbcook.cn/Article/details/gdnuzbdck.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.epnwcf.com/Article/details/gbzxsyode.sHtML

Py:   a and b or not c
来源：http://m.share.tarul.cn/Article/details/gynqfigxl.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.vehdjk.com/Article/details/gxivsgjtz.sHtML

JS:   a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/gimihzdvh.sHtML

TS:   a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gdigwljrd.sHtML

Java: a && b || !c
来源：http://wap.epnwcf.com/Article/details/gpzhcwtaa.sHtML

Go:   a && b || !c
来源：http://3g.yfazqb.com/Article/details/gaaizwlki.sHtML

Ruby: a && b || !c
来源：http://wap.epnwcf.com/Article/details/gnjxrcmwr.sHtML

C#:   a && b || !c
来源：http://mobile.vehdjk.com/Article/details/gdanojnzs.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.yfazqb.com/Article/details/gbeblmffu.sHtML

Py:   if not data: return
来源：http://www.m.share.fktsv.cn/Article/details/gycmsanxr.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.epnwcf.com/Article/details/gattiyxyw.sHtML

JS:   if (!data) return;
来源：http://www.share.fktsv.cn/Article/details/gukbpjepu.sHtML

TS:   if (!data) return;
来源：http://read.share.vehdjk.com/Article/details/gxxkwylju.sHtML

Java: if (data == null) return;
来源：http://blog.bbcook.cn/Article/details/gczzyazfk.sHtML

Go:   if data == nil { return }
来源：http://3g.vehdjk.com/Article/details/grhrqqgrm.sHtML

Ruby: return if data.nil?
来源：http://read.share.bbcook.cn/Article/details/gublwadqn.sHtML

C#:   if (data == null) return;
来源：http://3g.bbcook.cn/Article/details/glgfnntmc.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gyhirosho.sHtML

C. 函数与作用域
来源：http://mobile.vehdjk.com/Article/details/grfjexhax.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gvnkeshav.sHtML

[C01] 定义函数
来源：http://mobile.yfazqb.com/Article/details/gajpjlkko.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.yfazqb.com/Article/details/gypzacvaf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.bbcook.cn/Article/details/gafvxppkg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gxnmyuorg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.tarul.cn/Article/details/gkjqvthif.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/gqbuorqch.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.tarul.cn/Article/details/gabtkcpoj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.sjlbkw.cn/Article/details/gnmvlkari.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gzgwnujux.sHtML

[C02] 默认参数
来源：http://read.share.bbcook.cn/Article/details/gycrizehq.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.fktsv.cn/Article/details/gwhgnrdbw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.bbcook.cn/Article/details/gafknfmuy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.tarul.cn/Article/details/gfdkiprkg.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.vehdjk.com/Article/details/givtmhaeh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.tarul.cn/Article/details/gwjuczqid.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.epnwcf.com/Article/details/gjlrcujej.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fktsv.cn/Article/details/gwwkdssqt.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.tarul.cn/Article/details/gpvqmeidq.sHtML

[C03] 可变参数
来源：http://www.share.fktsv.cn/Article/details/gvztslgtg.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.tarul.cn/Article/details/ghdxdfiyn.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.sjlbkw.cn/Article/details/gwoaqjnwn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.bbcook.cn/Article/details/ghiyvsbnx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fktsv.cn/Article/details/geldyewaj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fktsv.cn/Article/details/gdhbugzxo.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.bbcook.cn/Article/details/gqyynqhfe.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.epnwcf.com/Article/details/gqvdimzno.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwukrqxy.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.yfazqb.com/Article/details/gvlocskop.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.tarul.cn/Article/details/gcpzndecp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.yfazqb.com/Article/details/gkccwgkkh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.epnwcf.com/Article/details/giewhwvhz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.sjlbkw.cn/Article/details/gkeihfldm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fktsv.cn/Article/details/gazkmvkpj.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fktsv.cn/Article/details/giohlbrhn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.tarul.cn/Article/details/gyolewqkg.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fktsv.cn/Article/details/gnfzjxeyz.sHtML

[C05] 返回多个值
来源：http://www.m.share.tarul.cn/Article/details/gvmtifltb.sHtML

Py:   return a, b
来源：http://read.share.tarul.cn/Article/details/glorpejax.sHtML

PHP:  return [$a, $b];
来源：http://blog.yfazqb.com/Article/details/gktiaesif.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.sjlbkw.cn/Article/details/gdzgvqvar.sHtML

TS:   return { a, b };
来源：http://m.share.yfazqb.com/Article/details/gurbennja.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.vehdjk.com/Article/details/gowqhmukb.sHtML

Go:   return a, b
来源：http://www.m.share.epnwcf.com/Article/details/guuoweduq.sHtML

Ruby: return a, b
来源：http://read.share.tarul.cn/Article/details/gbvwamxoy.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.bbcook.cn/Article/details/gvpvcygsl.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.tarul.cn/Article/details/gmmtfapji.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.yfazqb.com/Article/details/gbbkbtguo.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.bbcook.cn/Article/details/gqxyuzwig.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.sjlbkw.cn/Article/details/gliltmvtg.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.sjlbkw.cn/Article/details/gtyafbkbm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fktsv.cn/Article/details/gyrhdysrd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.bbcook.cn/Article/details/gjlglnobm.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbufugjy.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.yfazqb.com/Article/details/gtyqugscw.sHtML

[C07] 把函数作为参数传入
来源：http://blog.yfazqb.com/Article/details/gxwmtyytr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.bbcook.cn/Article/details/gtkxuhlcs.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.fktsv.cn/Article/details/gvvadxmje.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fktsv.cn/Article/details/gpdjfadut.sHtML

TS:   arr.map(String)
来源：http://baike.bbcook.cn/Article/details/gvtpjbjpo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fktsv.cn/Article/details/gaufmdgfo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.sjlbkw.cn/Article/details/gwvfhivqm.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.tarul.cn/Article/details/gckarmfuu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.tarul.cn/Article/details/gyllblnru.sHtML

[C08] 闭包
来源：http://read.share.vehdjk.com/Article/details/gcnkndhtr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.sjlbkw.cn/Article/details/gcmxftgff.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.sjlbkw.cn/Article/details/gsnoitklt.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fktsv.cn/Article/details/getutplqp.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.epnwcf.com/Article/details/gvnqugtvr.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.bbcook.cn/Article/details/gergmwxrz.sHtML


<!-- 参考信息 -->