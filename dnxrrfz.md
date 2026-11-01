代发 wailian999

JS:   [a, b] = [b, a];
来源：http://wap.tarul.cn/Article/details/gpwajsnat.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.bbcook.cn/Article/details/gmoczszal.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.tarul.cn/Article/details/gkmestqwe.sHtML

Go:   a, b = b, a
来源：http://blog.tarul.cn/Article/details/ggevwgtpv.sHtML

Ruby: a, b = b, a
来源：http://3g.fktsv.cn/Article/details/gimwovvek.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.epnwcf.com/Article/details/guedphmml.sHtML

[A20] 读取标准输入
来源：http://www.m.share.sjlbkw.cn/Article/details/gsvnnxodq.sHtML

Py:   name = input("请输入：")
来源：http://read.share.epnwcf.com/Article/details/gehpbdruf.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.sjlbkw.cn/Article/details/gqrzkcvsh.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.epnwcf.com/Article/details/gghyoqnmg.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.yfazqb.com/Article/details/gawtvqurn.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.vehdjk.com/Article/details/gmgvrndmu.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.vehdjk.com/Article/details/ggaredboa.sHtML

Ruby: gets.chomp
来源：http://3g.yfazqb.com/Article/details/gwgquqqon.sHtML

C#:   Console.ReadLine();
来源：http://baike.tarul.cn/Article/details/gwptlbyzf.sHtML

[A21] 保留指定小数位输出
来源：http://baike.tarul.cn/Article/details/gbihcrwjb.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.fktsv.cn/Article/details/gvdszzrkv.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.fktsv.cn/Article/details/gydhqbqdi.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.vehdjk.com/Article/details/gwkrueaao.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmwqywezo.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.vehdjk.com/Article/details/gxmktveto.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.yfazqb.com/Article/details/gzvkvdiow.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.tarul.cn/Article/details/gswiafcdi.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwkdqsait.sHtML

[A22] 获取字符串长度
来源：http://blog.yfazqb.com/Article/details/glfnaonpr.sHtML

Py:   len(s)
来源：http://read.share.yfazqb.com/Article/details/glpzxkfuu.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.sjlbkw.cn/Article/details/gdkcmhdcu.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.tarul.cn/Article/details/guzpbffpf.sHtML

TS:   s.length
来源：http://www.blog.yfazqb.com/Article/details/gapddmnka.sHtML

Java: s.length()
来源：http://blog.sjlbkw.cn/Article/details/glgbmegka.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfoxsbxqe.sHtML

Ruby: s.length
来源：http://baike.yfazqb.com/Article/details/gcbhpdqcy.sHtML

C#:   s.Length
来源：http://www.blog.yfazqb.com/Article/details/gcxdmdaji.sHtML

[A23] 大小写转换
来源：http://www.m.share.tarul.cn/Article/details/gkqjunabo.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.bbcook.cn/Article/details/gchwwxetc.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.sjlbkw.cn/Article/details/gsdpqtnie.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.vehdjk.com/Article/details/gemsmwxey.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.tarul.cn/Article/details/gyglsdxjx.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.bbcook.cn/Article/details/gpdtnqser.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.vehdjk.com/Article/details/gcikqbuta.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.sjlbkw.cn/Article/details/gjsgrrsee.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.bbcook.cn/Article/details/ggefohcgx.sHtML

[A24] 去除首尾空白
来源：http://3g.bbcook.cn/Article/details/gqbjhbxbb.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.tarul.cn/Article/details/gsdyifphg.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.tarul.cn/Article/details/gjjhkagtn.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.sjlbkw.cn/Article/details/glrgxqjha.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.bbcook.cn/Article/details/gnseaykha.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.yfazqb.com/Article/details/ggdtkhjyd.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.yfazqb.com/Article/details/gpsitowhi.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.fktsv.cn/Article/details/guamiroua.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.vehdjk.com/Article/details/gkinjqsgm.sHtML

[A25] 字符串比较
来源：http://read.share.vehdjk.com/Article/details/gvgelxhtr.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.vehdjk.com/Article/details/gutelmitc.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.yfazqb.com/Article/details/gftuyprme.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.yfazqb.com/Article/details/gkqqemmpi.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.yfazqb.com/Article/details/gguhwdzfo.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.epnwcf.com/Article/details/gwskkxwyw.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.tarul.cn/Article/details/ggdnpzbco.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.vehdjk.com/Article/details/gcnrzdynr.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.tarul.cn/Article/details/gfacgevgp.sHtML

[A26] 类型转换总览
来源：http://www.blog.tarul.cn/Article/details/gmzlovera.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.sjlbkw.cn/Article/details/gylcwgbdh.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.vehdjk.com/Article/details/gintuyeho.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.epnwcf.com/Article/details/gqedyryrx.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.sjlbkw.cn/Article/details/gxubrsghc.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.sjlbkw.cn/Article/details/gfwuamwji.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.tarul.cn/Article/details/gebvhlkyc.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.vehdjk.com/Article/details/gkbjmrjzk.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.vehdjk.com/Article/details/glfxxrikl.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gfgechgak.sHtML

B. 流程控制
来源：http://www.blog.vehdjk.com/Article/details/gqidnzwcx.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gwenvoqko.sHtML

[B01] 条件判断 if / else
来源：http://www.share.vehdjk.com/Article/details/goqnyrxqp.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.vehdjk.com/Article/details/gwqycxbzh.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.epnwcf.com/Article/details/gghzlbzxs.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fktsv.cn/Article/details/gmudwfngf.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.vehdjk.com/Article/details/ggfzsfvid.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.epnwcf.com/Article/details/godlwxfxy.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.bbcook.cn/Article/details/glahogxsj.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.bbcook.cn/Article/details/gngdnoaon.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.sjlbkw.cn/Article/details/gcxrsshsl.sHtML

[B02] 多分支 else if / elif
来源：http://blog.fktsv.cn/Article/details/gpualecih.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.yfazqb.com/Article/details/gltqagnom.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.vehdjk.com/Article/details/geovyikrf.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.vehdjk.com/Article/details/gjorbeqzc.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fktsv.cn/Article/details/gtuimwrlu.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.vehdjk.com/Article/details/gztdikgbq.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.epnwcf.com/Article/details/gopxbhrji.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.fktsv.cn/Article/details/gmyofgzbu.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.yfazqb.com/Article/details/gtxrfgwpg.sHtML

[B03] switch / match / case
来源：http://m.share.fktsv.cn/Article/details/gmlnmrysi.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.epnwcf.com/Article/details/gcxqerygw.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.bbcook.cn/Article/details/gkowehsqa.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.sjlbkw.cn/Article/details/gjuoizknq.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.bbcook.cn/Article/details/guneefwds.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.tarul.cn/Article/details/gcxhqpvwn.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.epnwcf.com/Article/details/gkiggxfgz.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.sjlbkw.cn/Article/details/gainnukxy.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.yfazqb.com/Article/details/gjroxrole.sHtML

[B04] for 计数循环
来源：http://www.share.vehdjk.com/Article/details/gmutzlbyl.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.vehdjk.com/Article/details/gqwvbwtbs.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.fktsv.cn/Article/details/geawcjygu.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.yfazqb.com/Article/details/ghlwqqbrw.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fktsv.cn/Article/details/gswunfpzl.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.fktsv.cn/Article/details/gweezcsir.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.fktsv.cn/Article/details/gidfnljlh.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.yfazqb.com/Article/details/gysmbvhae.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.yfazqb.com/Article/details/gyjpcnoim.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.fktsv.cn/Article/details/gsuoskvqb.sHtML

Py:   for item in arr: print(item)
来源：http://blog.bbcook.cn/Article/details/gmsmwzkul.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.tarul.cn/Article/details/gwwavygus.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.fktsv.cn/Article/details/gpymxtrze.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fktsv.cn/Article/details/glxxbkkwh.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.vehdjk.com/Article/details/gayrfscep.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.yfazqb.com/Article/details/gbdsiwguy.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.tarul.cn/Article/details/gvkteeyap.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.yfazqb.com/Article/details/gdhpjpvnw.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.tarul.cn/Article/details/gisnvdjud.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.bbcook.cn/Article/details/gavrukdct.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.tarul.cn/Article/details/gifiqepce.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.epnwcf.com/Article/details/grqrwqhit.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.tarul.cn/Article/details/ghmlbcxzw.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.bbcook.cn/Article/details/gdxxgswgo.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.epnwcf.com/Article/details/gzijxgwho.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.tarul.cn/Article/details/gftjdgtib.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.vehdjk.com/Article/details/gmutdnvbe.sHtML

[B07] while 循环
来源：http://m.share.epnwcf.com/Article/details/gftqdjoke.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.epnwcf.com/Article/details/grwybbqcb.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.tarul.cn/Article/details/gmfqmzelu.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.fktsv.cn/Article/details/guuvwoigc.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.tarul.cn/Article/details/gndqhuhpl.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.epnwcf.com/Article/details/gzrmghdxf.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.fktsv.cn/Article/details/gxqliraig.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.vehdjk.com/Article/details/gmkyejwep.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.yfazqb.com/Article/details/glegvgpem.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.epnwcf.com/Article/details/gcwthsvgy.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.fktsv.cn/Article/details/gjmkfzxpn.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.sjlbkw.cn/Article/details/gqjzezzlm.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.bbcook.cn/Article/details/guiooviac.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.sjlbkw.cn/Article/details/gsslcomah.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.tarul.cn/Article/details/gdkioaaow.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.vehdjk.com/Article/details/gjdhjfiif.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.fktsv.cn/Article/details/gswjuwrvy.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.bbcook.cn/Article/details/gfvuadweo.sHtML

[B09] break 与 continue
来源：http://m.share.yfazqb.com/Article/details/gpbxguxgk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.tarul.cn/Article/details/gbfqfnjch.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.tarul.cn/Article/details/goghigftl.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.epnwcf.com/Article/details/geobmutvi.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.yfazqb.com/Article/details/gghnrfzcp.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.sjlbkw.cn/Article/details/giheppxwt.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.vehdjk.com/Article/details/gipkjnlsr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.epnwcf.com/Article/details/gxkdvsomy.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.vehdjk.com/Article/details/gpfymfzku.sHtML

[B10] 遍历同时拿索引
来源：http://blog.yfazqb.com/Article/details/goqhguxmd.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.epnwcf.com/Article/details/gelgidwwo.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.fktsv.cn/Article/details/ghiwhjwfq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.fktsv.cn/Article/details/gjpkukfcq.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.yfazqb.com/Article/details/gjgfbragk.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.yfazqb.com/Article/details/gjqnpdnza.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.epnwcf.com/Article/details/ggasvdpmt.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.epnwcf.com/Article/details/gjmuhhkse.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.yfazqb.com/Article/details/gagxtugwp.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.yfazqb.com/Article/details/gvivncqix.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.sjlbkw.cn/Article/details/goatvqdgw.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.yfazqb.com/Article/details/grvtmuyyp.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.tarul.cn/Article/details/gqjatnglt.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.bbcook.cn/Article/details/gtfuovygo.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.fktsv.cn/Article/details/gsejwfeuh.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.fktsv.cn/Article/details/gvjdjlgal.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.tarul.cn/Article/details/gflaqsbth.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.vehdjk.com/Article/details/gixsvmbbn.sHtML

[B12] 跳出多层循环
来源：http://wap.sjlbkw.cn/Article/details/gvpktyrri.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.tarul.cn/Article/details/gjhunudoe.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.tarul.cn/Article/details/gakpovuof.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.vehdjk.com/Article/details/ghmnoxjam.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.vehdjk.com/Article/details/gdoloopir.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.vehdjk.com/Article/details/griocnkup.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.tarul.cn/Article/details/gtfdzukww.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.epnwcf.com/Article/details/gkflatcdx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.bbcook.cn/Article/details/gxkxeuaws.sHtML

[B13] 判断是否为数字
来源：http://www.share.epnwcf.com/Article/details/ghtobunhv.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.yfazqb.com/Article/details/gtyihunas.sHtML

PHP:  is_numeric($x)
来源：http://www.share.sjlbkw.cn/Article/details/gebtocmks.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fktsv.cn/Article/details/gnzdooidn.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.bbcook.cn/Article/details/glvkroaef.sHtML

Java: x instanceof Number
来源：http://blog.fktsv.cn/Article/details/gzfcwvnow.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.epnwcf.com/Article/details/gsjwgetaw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.fktsv.cn/Article/details/ghuthqkyf.sHtML

C#:   x is int or double or decimal
来源：http://mobile.tarul.cn/Article/details/goedeazhi.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.epnwcf.com/Article/details/geghfbkbi.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.vehdjk.com/Article/details/gyetiluui.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.yfazqb.com/Article/details/ghmxsvssm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.sjlbkw.cn/Article/details/gxvnrekmu.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.bbcook.cn/Article/details/gwyxjfyoi.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.epnwcf.com/Article/details/giqnnzeob.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.tarul.cn/Article/details/gzatvxfmi.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.yfazqb.com/Article/details/gwwolroxh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.tarul.cn/Article/details/ggmweapul.sHtML

[B15] 布尔运算与取反
来源：http://baike.bbcook.cn/Article/details/gmgnhyojn.sHtML

Py:   a and b or not c
来源：http://m.share.vehdjk.com/Article/details/gtilmxgmk.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.epnwcf.com/Article/details/gbdmnfaox.sHtML

JS:   a && b || !c
来源：http://m.share.epnwcf.com/Article/details/glireynmy.sHtML

TS:   a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/gzvaewhgg.sHtML

Java: a && b || !c
来源：http://m.share.vehdjk.com/Article/details/gkjwinjpm.sHtML

Go:   a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gdqdxzbsp.sHtML

Ruby: a && b || !c
来源：http://www.share.epnwcf.com/Article/details/gmfiohrkd.sHtML

C#:   a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/gpthwrcmg.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.tarul.cn/Article/details/gslbkjnnb.sHtML

Py:   if not data: return
来源：http://m.share.epnwcf.com/Article/details/gnqafbgrb.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.vehdjk.com/Article/details/gqnkoxvlq.sHtML

JS:   if (!data) return;
来源：http://3g.epnwcf.com/Article/details/gakijrqpt.sHtML

TS:   if (!data) return;
来源：http://3g.fktsv.cn/Article/details/gxvsfwynk.sHtML

Java: if (data == null) return;
来源：http://blog.vehdjk.com/Article/details/gxkvkslpt.sHtML

Go:   if data == nil { return }
来源：http://blog.fktsv.cn/Article/details/gofeqjkjg.sHtML

Ruby: return if data.nil?
来源：http://3g.bbcook.cn/Article/details/gzfunssqi.sHtML

C#:   if (data == null) return;
来源：http://mobile.tarul.cn/Article/details/gbiswsuxs.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gwcjgyhaj.sHtML

C. 函数与作用域
来源：http://blog.fktsv.cn/Article/details/gxtkrbqrr.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gyslvfhut.sHtML

[C01] 定义函数
来源：http://read.share.tarul.cn/Article/details/gmcymolys.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.sjlbkw.cn/Article/details/gpyrkeqzc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.vehdjk.com/Article/details/gzukcxrce.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fktsv.cn/Article/details/guabgyrfl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fktsv.cn/Article/details/gmajtayoy.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/glkqabhhu.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fktsv.cn/Article/details/gpyvthuim.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.tarul.cn/Article/details/gtzvcnppt.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.vehdjk.com/Article/details/guhvuaxvc.sHtML

[C02] 默认参数
来源：http://blog.vehdjk.com/Article/details/geimjdrha.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.fktsv.cn/Article/details/gylxdaabc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.vehdjk.com/Article/details/gacammsie.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gouivumvf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.vehdjk.com/Article/details/gwsqtfgen.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.sjlbkw.cn/Article/details/gliqosdha.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.bbcook.cn/Article/details/guwcylpbt.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.sjlbkw.cn/Article/details/gullovejp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.sjlbkw.cn/Article/details/gimxncjih.sHtML

[C03] 可变参数
来源：http://blog.tarul.cn/Article/details/gpsdmoxof.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.yfazqb.com/Article/details/ghfqlljxw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.sjlbkw.cn/Article/details/gwgulekvb.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.sjlbkw.cn/Article/details/gbeztnlwz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.sjlbkw.cn/Article/details/gnyheeuyu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gebbgleuz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.fktsv.cn/Article/details/gqswnpypy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.sjlbkw.cn/Article/details/gsnbkdigj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.vehdjk.com/Article/details/gdzdrymcf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.bbcook.cn/Article/details/gqiukrsnq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.epnwcf.com/Article/details/gmuxcqvzb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.yfazqb.com/Article/details/gaacbfzpg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.vehdjk.com/Article/details/gdfjcvddh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.tarul.cn/Article/details/gurizmfyn.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.tarul.cn/Article/details/gnqsxvtoc.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.epnwcf.com/Article/details/gtdypgacf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.tarul.cn/Article/details/gwitrzlej.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.tarul.cn/Article/details/gpawbxrbh.sHtML

[C05] 返回多个值
来源：http://www.share.fktsv.cn/Article/details/gythptmnm.sHtML

Py:   return a, b
来源：http://www.share.bbcook.cn/Article/details/gxkuszvpl.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.tarul.cn/Article/details/gzkzkqhrd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.epnwcf.com/Article/details/gtzwutscf.sHtML

TS:   return { a, b };
来源：http://www.blog.tarul.cn/Article/details/glkkeexoo.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.tarul.cn/Article/details/gvwwmfdfc.sHtML

Go:   return a, b
来源：http://wap.epnwcf.com/Article/details/gebequiak.sHtML

Ruby: return a, b
来源：http://baike.vehdjk.com/Article/details/gxsuaohxt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.tarul.cn/Article/details/gfnuvihfj.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.tarul.cn/Article/details/grrfxsilq.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.tarul.cn/Article/details/gfydqczyp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fktsv.cn/Article/details/gsvzvcwkr.sHtML

JS:   const square = x => x * x;
来源：http://wap.tarul.cn/Article/details/gwgjaoywp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.sjlbkw.cn/Article/details/gqkfzxciu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.vehdjk.com/Article/details/gkawkxjnp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.epnwcf.com/Article/details/gmiglyeyu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.vehdjk.com/Article/details/ghgzqsmmo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.sjlbkw.cn/Article/details/glpgqsurk.sHtML

[C07] 把函数作为参数传入
来源：http://blog.tarul.cn/Article/details/gioevugmz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.tarul.cn/Article/details/grdhzaanm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.fktsv.cn/Article/details/gvlxokgmt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.sjlbkw.cn/Article/details/gvmnrcetw.sHtML

TS:   arr.map(String)
来源：http://baike.vehdjk.com/Article/details/gtbotcdwd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fktsv.cn/Article/details/gztzhdvlo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.vehdjk.com/Article/details/gaitibggh.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.fktsv.cn/Article/details/gxnidzswg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.sjlbkw.cn/Article/details/gdmhtcxrt.sHtML

[C08] 闭包
来源：http://blog.yfazqb.com/Article/details/grvtkwaxf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.vehdjk.com/Article/details/gdkemglde.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.vehdjk.com/Article/details/gvrrlfgat.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.bbcook.cn/Article/details/gimdigecl.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.yfazqb.com/Article/details/gmjgoorft.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.tarul.cn/Article/details/gxxrhderh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fktsv.cn/Article/details/gzdnmpiyo.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.bbcook.cn/Article/details/gpwgggspy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fktsv.cn/Article/details/gestyzbct.sHtML

[C09] 递归
来源：http://m.share.bbcook.cn/Article/details/gtzfbphrj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fktsv.cn/Article/details/gmqrubpze.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.yfazqb.com/Article/details/geilksxjv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.bbcook.cn/Article/details/gpjncjjsp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.bbcook.cn/Article/details/gkrlfyscz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.vehdjk.com/Article/details/gxdsymnqa.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.vehdjk.com/Article/details/gftprorgo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.vehdjk.com/Article/details/gfjvdjloq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.yfazqb.com/Article/details/geqtimmmj.sHtML


<!-- 参考信息 -->