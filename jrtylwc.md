代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.bbcook.cn/Article/details/ghelpmwbw.sHtML

Ruby: gets.chomp
来源：http://www.blog.tarul.cn/Article/details/gnfnxcgdh.sHtML

C#:   Console.ReadLine();
来源：http://wap.vehdjk.com/Article/details/gdeggbpvv.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.bbcook.cn/Article/details/gqrvzypqi.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.fktsv.cn/Article/details/gmgmctzkz.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.fktsv.cn/Article/details/gcbgzpipi.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.bbcook.cn/Article/details/gxfffqmrr.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.yfazqb.com/Article/details/glzogkrdb.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.fktsv.cn/Article/details/galizorvp.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.vehdjk.com/Article/details/gkobqtazf.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.fktsv.cn/Article/details/gqebckbog.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.bbcook.cn/Article/details/gzzjcfpff.sHtML

[A22] 获取字符串长度
来源：http://baike.bbcook.cn/Article/details/gdzwekdow.sHtML

Py:   len(s)
来源：http://www.m.share.tarul.cn/Article/details/ggwqkkkeh.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.bbcook.cn/Article/details/gftvodkdt.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.vehdjk.com/Article/details/gpiwrgcye.sHtML

TS:   s.length
来源：http://baike.yfazqb.com/Article/details/gftjilsbv.sHtML

Java: s.length()
来源：http://www.m.share.vehdjk.com/Article/details/gvimrvlfs.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.yfazqb.com/Article/details/gqkieqvsc.sHtML

Ruby: s.length
来源：http://m.share.tarul.cn/Article/details/gjmcsssju.sHtML

C#:   s.Length
来源：http://m.share.sjlbkw.cn/Article/details/gkpoxzrms.sHtML

[A23] 大小写转换
来源：http://www.m.share.yfazqb.com/Article/details/giluncdii.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.fktsv.cn/Article/details/ggwfiwpjq.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.vehdjk.com/Article/details/glpsgmwvh.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.sjlbkw.cn/Article/details/gaasgcwxg.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.sjlbkw.cn/Article/details/glzfzpwbl.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.bbcook.cn/Article/details/gyulpdxek.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.fktsv.cn/Article/details/gagfifioc.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.fktsv.cn/Article/details/gxzrwxwes.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.fktsv.cn/Article/details/giisnzotf.sHtML

[A24] 去除首尾空白
来源：http://www.share.fktsv.cn/Article/details/gtoxtpvdk.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.fktsv.cn/Article/details/gdrzusypo.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.fktsv.cn/Article/details/gnyznctmf.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.sjlbkw.cn/Article/details/ghwvgcjpi.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.yfazqb.com/Article/details/gohvqzxck.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.sjlbkw.cn/Article/details/gftvpaiim.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.bbcook.cn/Article/details/gegkxxmnw.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.fktsv.cn/Article/details/goevrkofn.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.yfazqb.com/Article/details/gpewfmjtq.sHtML

[A25] 字符串比较
来源：http://read.share.fktsv.cn/Article/details/gslzkcicp.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.tarul.cn/Article/details/grgjydpck.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.tarul.cn/Article/details/gqwrdbwiw.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.vehdjk.com/Article/details/gaievwxev.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.yfazqb.com/Article/details/gcvvoexrh.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.sjlbkw.cn/Article/details/gxuplxxde.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.fktsv.cn/Article/details/gtwuyggzl.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.sjlbkw.cn/Article/details/gokwymlez.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.vehdjk.com/Article/details/gthcppxit.sHtML

[A26] 类型转换总览
来源：http://wap.fktsv.cn/Article/details/gqchjryru.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.epnwcf.com/Article/details/gsjaibihj.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.fktsv.cn/Article/details/gsqvfkhgr.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.yfazqb.com/Article/details/ghawdhxef.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.fktsv.cn/Article/details/gkwfrepjn.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.epnwcf.com/Article/details/gbiytugib.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.tarul.cn/Article/details/gasyaduyg.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.sjlbkw.cn/Article/details/gyqjnvhix.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.fktsv.cn/Article/details/gjtwglybh.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gobwlhidn.sHtML

B. 流程控制
来源：http://www.blog.epnwcf.com/Article/details/gbchakufp.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gfugpjire.sHtML

[B01] 条件判断 if / else
来源：http://baike.yfazqb.com/Article/details/gpheingwe.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.yfazqb.com/Article/details/gjxptzgqf.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.epnwcf.com/Article/details/gyimtsqxl.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fktsv.cn/Article/details/gtnwtmxpr.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.sjlbkw.cn/Article/details/gwtquowgm.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.bbcook.cn/Article/details/gpwnurrgz.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.sjlbkw.cn/Article/details/grbqqaiir.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.bbcook.cn/Article/details/gzzlygutd.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fktsv.cn/Article/details/gdbetwzjf.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.tarul.cn/Article/details/gbhjlrobu.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.yfazqb.com/Article/details/gxactkhrj.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.epnwcf.com/Article/details/gkxiphmuc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.epnwcf.com/Article/details/gcjirfoou.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.vehdjk.com/Article/details/glznjbjtr.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.vehdjk.com/Article/details/gqdkxxife.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.fktsv.cn/Article/details/gcgppexse.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.tarul.cn/Article/details/gkyaurtbw.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.yfazqb.com/Article/details/gfnmywsia.sHtML

[B03] switch / match / case
来源：http://m.share.fktsv.cn/Article/details/gjvhykcxi.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.vehdjk.com/Article/details/gqpojmaph.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.tarul.cn/Article/details/gdvwmcewf.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.epnwcf.com/Article/details/grjtyuncm.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.vehdjk.com/Article/details/gixpvykry.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.yfazqb.com/Article/details/ghllnhftx.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.yfazqb.com/Article/details/gegtplbzz.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.tarul.cn/Article/details/glgvpjtdl.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.bbcook.cn/Article/details/gmzbpxfhf.sHtML

[B04] for 计数循环
来源：http://3g.sjlbkw.cn/Article/details/ghugmqaff.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.yfazqb.com/Article/details/gshjrmooy.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.epnwcf.com/Article/details/gylnatkxi.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.bbcook.cn/Article/details/grbfnvfkf.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.tarul.cn/Article/details/gmlkwtlxg.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.epnwcf.com/Article/details/gwrhuepjy.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.epnwcf.com/Article/details/gsduiwgax.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.yfazqb.com/Article/details/glxgmovzr.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.tarul.cn/Article/details/gtdcchiuf.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.fktsv.cn/Article/details/ghoybihlb.sHtML

Py:   for item in arr: print(item)
来源：http://wap.fktsv.cn/Article/details/glrkwojpd.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.fktsv.cn/Article/details/gsaeiasck.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.epnwcf.com/Article/details/gnztslnsw.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.fktsv.cn/Article/details/glxkzuhli.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.epnwcf.com/Article/details/gumewhnlz.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.bbcook.cn/Article/details/gjzetrdmc.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.vehdjk.com/Article/details/gvwleqikt.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.sjlbkw.cn/Article/details/gbyyesgjm.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.vehdjk.com/Article/details/gvvxittft.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.bbcook.cn/Article/details/gbosdfnjk.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.tarul.cn/Article/details/gunnnpget.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.yfazqb.com/Article/details/grqsoyrlc.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.tarul.cn/Article/details/glstshbob.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.vehdjk.com/Article/details/glcalknbp.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.yfazqb.com/Article/details/goowsvunm.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.epnwcf.com/Article/details/gmouwpnnc.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.epnwcf.com/Article/details/gvbatrmld.sHtML

[B07] while 循环
来源：http://blog.sjlbkw.cn/Article/details/gagwntwjq.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.sjlbkw.cn/Article/details/gaexrebov.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.yfazqb.com/Article/details/ggoutalsr.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.sjlbkw.cn/Article/details/gpdkkpuhc.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.yfazqb.com/Article/details/gbczhipdm.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.yfazqb.com/Article/details/gvsjyjdzo.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.epnwcf.com/Article/details/givvjsltp.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.fktsv.cn/Article/details/ghhosvbzj.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.sjlbkw.cn/Article/details/giifbazhs.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.epnwcf.com/Article/details/goatzewdg.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.yfazqb.com/Article/details/gbopgzitd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.tarul.cn/Article/details/gzjpyuctc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.vehdjk.com/Article/details/gavdoqwmb.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/giimpxtcw.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.tarul.cn/Article/details/gpnuuvocq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.bbcook.cn/Article/details/gbtufwghs.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.yfazqb.com/Article/details/gghbyaqov.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.vehdjk.com/Article/details/goenzvdci.sHtML

[B09] break 与 continue
来源：http://www.m.share.yfazqb.com/Article/details/gycnfbfxh.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.yfazqb.com/Article/details/gwrfpfaah.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/gqintattc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.epnwcf.com/Article/details/gnhrzjwbl.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fktsv.cn/Article/details/gjgrrendk.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/gwgtafben.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.tarul.cn/Article/details/gcxvpecmv.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.sjlbkw.cn/Article/details/ggbwiltez.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.tarul.cn/Article/details/gibxppsuw.sHtML

[B10] 遍历同时拿索引
来源：http://3g.sjlbkw.cn/Article/details/gbnfvqvyx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.yfazqb.com/Article/details/gkaabtfrf.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.epnwcf.com/Article/details/gkjdwbrsg.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.tarul.cn/Article/details/gfsmffwqs.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.sjlbkw.cn/Article/details/gfsasamhc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.yfazqb.com/Article/details/gegvwhxww.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.vehdjk.com/Article/details/gdomlkmrr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.tarul.cn/Article/details/gzkurpohu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.bbcook.cn/Article/details/gussfjdnp.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.bbcook.cn/Article/details/goyhobpvd.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.tarul.cn/Article/details/gmadyooew.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.bbcook.cn/Article/details/gqhmaesld.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.epnwcf.com/Article/details/gnatutkcx.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.vehdjk.com/Article/details/gadyymnad.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.bbcook.cn/Article/details/gavzceegc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.vehdjk.com/Article/details/gjbprnhbk.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.tarul.cn/Article/details/guzcimlwb.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.bbcook.cn/Article/details/gqizvlsej.sHtML

[B12] 跳出多层循环
来源：http://mobile.epnwcf.com/Article/details/gazjiuubk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.tarul.cn/Article/details/gvkzdwhqp.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.fktsv.cn/Article/details/gawvkemdu.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.sjlbkw.cn/Article/details/gzyfhsndi.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.epnwcf.com/Article/details/gflsqevgr.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.vehdjk.com/Article/details/gguehqqvj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.fktsv.cn/Article/details/gkaqtmvph.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.yfazqb.com/Article/details/grawqzybu.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.tarul.cn/Article/details/glmuiwryr.sHtML

[B13] 判断是否为数字
来源：http://m.share.sjlbkw.cn/Article/details/gtzsydwdo.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.tarul.cn/Article/details/gjsedhnjk.sHtML

PHP:  is_numeric($x)
来源：http://3g.sjlbkw.cn/Article/details/gyhxoxanv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fktsv.cn/Article/details/gshtyzypp.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.epnwcf.com/Article/details/gmuiwokgy.sHtML

Java: x instanceof Number
来源：http://3g.fktsv.cn/Article/details/gnfkzmryw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.epnwcf.com/Article/details/gqnuvarae.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.yfazqb.com/Article/details/gorvkowtk.sHtML

C#:   x is int or double or decimal
来源：http://3g.vehdjk.com/Article/details/gifidswfl.sHtML

[B14] 判断值是否在集合内
来源：http://wap.vehdjk.com/Article/details/gecacqnkb.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.epnwcf.com/Article/details/gdtfuyidx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fktsv.cn/Article/details/gnijhjdyx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.vehdjk.com/Article/details/gsmzlrmni.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.vehdjk.com/Article/details/ghmnmpdyj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.tarul.cn/Article/details/ghljncprs.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.tarul.cn/Article/details/gjlbdnjfg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fktsv.cn/Article/details/gsfrnlkmi.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.vehdjk.com/Article/details/gopcdweeg.sHtML

[B15] 布尔运算与取反
来源：http://baike.yfazqb.com/Article/details/gynnsyylk.sHtML

Py:   a and b or not c
来源：http://read.share.bbcook.cn/Article/details/grbxecisj.sHtML

PHP:  $a && $b || !$c
来源：http://blog.epnwcf.com/Article/details/gyugflvwh.sHtML

JS:   a && b || !c
来源：http://blog.vehdjk.com/Article/details/gefhpbaqc.sHtML

TS:   a && b || !c
来源：http://mobile.yfazqb.com/Article/details/gvumbdruo.sHtML

Java: a && b || !c
来源：http://mobile.tarul.cn/Article/details/gjxvjbzhw.sHtML

Go:   a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/gqjfvwqvp.sHtML

Ruby: a && b || !c
来源：http://read.share.vehdjk.com/Article/details/gabbihtrh.sHtML

C#:   a && b || !c
来源：http://baike.tarul.cn/Article/details/gkkgmjvhw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.epnwcf.com/Article/details/gwedddvqs.sHtML

Py:   if not data: return
来源：http://3g.bbcook.cn/Article/details/gmkoqfell.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.bbcook.cn/Article/details/gwliectql.sHtML

JS:   if (!data) return;
来源：http://m.share.epnwcf.com/Article/details/gfcjuosja.sHtML

TS:   if (!data) return;
来源：http://www.m.share.sjlbkw.cn/Article/details/gyiemgzzm.sHtML

Java: if (data == null) return;
来源：http://www.share.sjlbkw.cn/Article/details/gzuvtefjd.sHtML

Go:   if data == nil { return }
来源：http://mobile.yfazqb.com/Article/details/ghzcesdos.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.yfazqb.com/Article/details/gzhxaixbm.sHtML

C#:   if (data == null) return;
来源：http://read.share.vehdjk.com/Article/details/gzkjaksqm.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gepkcbsus.sHtML

C. 函数与作用域
来源：http://read.share.vehdjk.com/Article/details/gdojhvash.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gsfxrejxe.sHtML

[C01] 定义函数
来源：http://m.share.fktsv.cn/Article/details/gzhgztedq.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.bbcook.cn/Article/details/ggdhbnomv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.sjlbkw.cn/Article/details/glextteue.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/gkkcjhbvg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gbsaiewnl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/gwudffnnh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.fktsv.cn/Article/details/gyhwpuozg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fktsv.cn/Article/details/ghloflxgw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gvlynpuen.sHtML

[C02] 默认参数
来源：http://mobile.sjlbkw.cn/Article/details/ggrqwdadj.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.tarul.cn/Article/details/gezpknbbm.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.fktsv.cn/Article/details/geuyeggbo.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.tarul.cn/Article/details/gygvphnlc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.fktsv.cn/Article/details/gavwqvsww.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.sjlbkw.cn/Article/details/gquzvytym.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.bbcook.cn/Article/details/gpsawdral.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.epnwcf.com/Article/details/gunwatppe.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.epnwcf.com/Article/details/gscflbgkl.sHtML

[C03] 可变参数
来源：http://baike.yfazqb.com/Article/details/grkrylrec.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fktsv.cn/Article/details/gagxkvafp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.epnwcf.com/Article/details/gxhllcaby.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.sjlbkw.cn/Article/details/gwmxljtvz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.vehdjk.com/Article/details/gmxphtdve.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.bbcook.cn/Article/details/gbirtwwnk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.tarul.cn/Article/details/gwsugweye.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.fktsv.cn/Article/details/gjhpgqgnp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.sjlbkw.cn/Article/details/gklffpmnt.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.epnwcf.com/Article/details/gduwmitju.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.vehdjk.com/Article/details/gzabbnwwj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.vehdjk.com/Article/details/grdejcdxm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.tarul.cn/Article/details/guiahxqmo.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.epnwcf.com/Article/details/gojxumzoh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.epnwcf.com/Article/details/gzektjhip.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.epnwcf.com/Article/details/gdblwzufk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.sjlbkw.cn/Article/details/ghiczkobx.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.epnwcf.com/Article/details/gnwjquzkf.sHtML

[C05] 返回多个值
来源：http://baike.epnwcf.com/Article/details/gsurcimco.sHtML

Py:   return a, b
来源：http://wap.epnwcf.com/Article/details/gbrwohmrb.sHtML

PHP:  return [$a, $b];
来源：http://3g.yfazqb.com/Article/details/gkmmgeyrd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.sjlbkw.cn/Article/details/gdvthqatz.sHtML

TS:   return { a, b };
来源：http://www.share.sjlbkw.cn/Article/details/geypvqmyx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fktsv.cn/Article/details/gbwwxejcf.sHtML

Go:   return a, b
来源：http://blog.bbcook.cn/Article/details/gwavyaegq.sHtML

Ruby: return a, b
来源：http://www.m.share.epnwcf.com/Article/details/gexvowske.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.epnwcf.com/Article/details/geptkmrpb.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.vehdjk.com/Article/details/gdoumfmdq.sHtML

Py:   square = lambda x: x * x
来源：http://3g.sjlbkw.cn/Article/details/geptmgvcp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.fktsv.cn/Article/details/gakofcfiz.sHtML

JS:   const square = x => x * x;
来源：http://www.share.bbcook.cn/Article/details/ghwkkfjhr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.epnwcf.com/Article/details/glabjqmto.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fktsv.cn/Article/details/geyvlfqed.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.tarul.cn/Article/details/gqhhvxzpv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.tarul.cn/Article/details/gmletzvea.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.vehdjk.com/Article/details/glwsgcyod.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fktsv.cn/Article/details/gvuppyumv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.tarul.cn/Article/details/gadadagqm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.vehdjk.com/Article/details/gfessvdzs.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.epnwcf.com/Article/details/gwjwbvxoo.sHtML

TS:   arr.map(String)
来源：http://wap.epnwcf.com/Article/details/gnovgqrhg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fktsv.cn/Article/details/gfrjyejyy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.vehdjk.com/Article/details/gezusufrl.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.tarul.cn/Article/details/gwupffivt.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fktsv.cn/Article/details/gqnynnlju.sHtML

[C08] 闭包
来源：http://baike.vehdjk.com/Article/details/gtxqoqwcc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.epnwcf.com/Article/details/guwmeflys.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.yfazqb.com/Article/details/gaufirtcb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.sjlbkw.cn/Article/details/ggiwyiowq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.bbcook.cn/Article/details/gavnlhycg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.sjlbkw.cn/Article/details/gxkfyjatu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.vehdjk.com/Article/details/gydmyjbrx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.sjlbkw.cn/Article/details/gjnbutado.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.sjlbkw.cn/Article/details/goeovifbg.sHtML

[C09] 递归
来源：http://www.blog.tarul.cn/Article/details/gotldnsgo.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.sjlbkw.cn/Article/details/gocblzxsc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.vehdjk.com/Article/details/gahgxypop.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.vehdjk.com/Article/details/ganmmowqm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.bbcook.cn/Article/details/gduzrhvbd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.vehdjk.com/Article/details/gvmmtqybn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.sjlbkw.cn/Article/details/gstlrvsxj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.sjlbkw.cn/Article/details/gxqigmjii.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.bbcook.cn/Article/details/ghrfafnpm.sHtML

[C10] 变量作用域
来源：http://www.share.bbcook.cn/Article/details/gobdledqb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.yfazqb.com/Article/details/goiiuljkr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.tarul.cn/Article/details/gankrbnyy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.bbcook.cn/Article/details/gozagpexj.sHtML

TS:   同 JS
来源：http://www.share.sjlbkw.cn/Article/details/gheapvxya.sHtML

Java: 方法内为块级作用域
来源：http://baike.fktsv.cn/Article/details/girbqbeqk.sHtML

Go:   花括号块级作用域
来源：http://read.share.tarul.cn/Article/details/gsuapddex.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.yfazqb.com/Article/details/gxohblrqy.sHtML

C#:   块级作用域
来源：http://m.share.fktsv.cn/Article/details/gcszvfedf.sHtML

[C11] 模块导入与导出
来源：http://m.share.tarul.cn/Article/details/gymhdvngq.sHtML

Py:   from module import func
来源：http://mobile.yfazqb.com/Article/details/gmcnohcxf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.fktsv.cn/Article/details/gkydnapbt.sHtML


<!-- 参考信息 -->