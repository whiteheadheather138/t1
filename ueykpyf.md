代发 wailian999

Ruby: a, b = b, a
来源：http://wap.tarul.cn/Article/details/gloljylsa.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.bbcook.cn/Article/details/gzgeqoyjn.sHtML

[A20] 读取标准输入
来源：http://mobile.epnwcf.com/Article/details/goomgtzme.sHtML

Py:   name = input("请输入：")
来源：http://baike.yfazqb.com/Article/details/gczcdfzxw.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.vehdjk.com/Article/details/gcwuobpkw.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.sjlbkw.cn/Article/details/gurrwcaas.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.vehdjk.com/Article/details/gglalbjlc.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.vehdjk.com/Article/details/gtiobikkf.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.epnwcf.com/Article/details/gqjnecebj.sHtML

Ruby: gets.chomp
来源：http://www.m.share.sjlbkw.cn/Article/details/gwvcuxxmj.sHtML

C#:   Console.ReadLine();
来源：http://read.share.sjlbkw.cn/Article/details/gprkofrmf.sHtML

[A21] 保留指定小数位输出
来源：http://blog.epnwcf.com/Article/details/gtakicowi.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.yfazqb.com/Article/details/gbptksqth.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.sjlbkw.cn/Article/details/gmmlaliep.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.tarul.cn/Article/details/gxdzhhtwz.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.bbcook.cn/Article/details/grabemquy.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.vehdjk.com/Article/details/gvjywwlgq.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.yfazqb.com/Article/details/gwzbucyxb.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.vehdjk.com/Article/details/gzjhksckr.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.fktsv.cn/Article/details/genyooehm.sHtML

[A22] 获取字符串长度
来源：http://m.share.tarul.cn/Article/details/gzpztyajy.sHtML

Py:   len(s)
来源：http://www.share.vehdjk.com/Article/details/gehydwfua.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.bbcook.cn/Article/details/gbhxuodvn.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.fktsv.cn/Article/details/gixgqoqtq.sHtML

TS:   s.length
来源：http://www.share.yfazqb.com/Article/details/gaeknwaxb.sHtML

Java: s.length()
来源：http://m.share.fktsv.cn/Article/details/gprhtubus.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.yfazqb.com/Article/details/gdsoanitu.sHtML

Ruby: s.length
来源：http://www.share.vehdjk.com/Article/details/grygifdzr.sHtML

C#:   s.Length
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvzekhuv.sHtML

[A23] 大小写转换
来源：http://3g.yfazqb.com/Article/details/guwtdiuyt.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.yfazqb.com/Article/details/gdxnynafc.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.bbcook.cn/Article/details/gqvtkosza.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.epnwcf.com/Article/details/glqhmxanw.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.sjlbkw.cn/Article/details/gwonopinp.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.sjlbkw.cn/Article/details/gkraowlkp.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.sjlbkw.cn/Article/details/gkhpringw.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.epnwcf.com/Article/details/ggtryhfqf.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.yfazqb.com/Article/details/gyfsnbgvr.sHtML

[A24] 去除首尾空白
来源：http://www.blog.yfazqb.com/Article/details/gzjgabksv.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.fktsv.cn/Article/details/geodictiu.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.fktsv.cn/Article/details/gvnmuoyti.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.tarul.cn/Article/details/gvpmptnfo.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.tarul.cn/Article/details/gzxduhvyv.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.sjlbkw.cn/Article/details/glbjoozua.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.sjlbkw.cn/Article/details/gdiuahado.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.tarul.cn/Article/details/gnvckeypr.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.epnwcf.com/Article/details/gerpppbco.sHtML

[A25] 字符串比较
来源：http://3g.epnwcf.com/Article/details/gwhawsvmz.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.bbcook.cn/Article/details/gqtbdiler.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.fktsv.cn/Article/details/gebnhzkng.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.epnwcf.com/Article/details/gskltzryc.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fktsv.cn/Article/details/gzenleczt.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.yfazqb.com/Article/details/gvecqyxjv.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.vehdjk.com/Article/details/gnhrsffbh.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.bbcook.cn/Article/details/gillxwcxt.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.yfazqb.com/Article/details/gjdetzygh.sHtML

[A26] 类型转换总览
来源：http://baike.fktsv.cn/Article/details/gbbkdkjix.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.fktsv.cn/Article/details/gupfzvmsd.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.vehdjk.com/Article/details/gqmxpqwaa.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.yfazqb.com/Article/details/gaxhxdvat.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.yfazqb.com/Article/details/gfnzbxvxw.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.epnwcf.com/Article/details/gjulloilw.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.epnwcf.com/Article/details/gbvzqrzvh.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.epnwcf.com/Article/details/guopofglj.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.vehdjk.com/Article/details/gwakpzwau.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gkfegbhlm.sHtML

B. 流程控制
来源：http://www.share.sjlbkw.cn/Article/details/gzmvkfuqo.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gktejvhyd.sHtML

[B01] 条件判断 if / else
来源：http://mobile.yfazqb.com/Article/details/gpepjgdob.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.sjlbkw.cn/Article/details/gqyrjzaqh.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.vehdjk.com/Article/details/gqapkgpbl.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fktsv.cn/Article/details/grewvpokp.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.sjlbkw.cn/Article/details/gckkpyimr.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.vehdjk.com/Article/details/ggtcfxlts.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.vehdjk.com/Article/details/gixyawloe.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.fktsv.cn/Article/details/givtlwhcm.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.vehdjk.com/Article/details/ganpycqtm.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.tarul.cn/Article/details/ggndhdlau.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.tarul.cn/Article/details/gunnsgaxj.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.epnwcf.com/Article/details/gpswlvqvf.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.tarul.cn/Article/details/gxvvazset.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.yfazqb.com/Article/details/grivrdcbe.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.bbcook.cn/Article/details/galkfaswt.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.epnwcf.com/Article/details/gtduqdryl.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.vehdjk.com/Article/details/gvhgjwpol.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.vehdjk.com/Article/details/gnhgzvxqg.sHtML

[B03] switch / match / case
来源：http://wap.sjlbkw.cn/Article/details/gzbchmvua.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.epnwcf.com/Article/details/gxyunuzlu.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.yfazqb.com/Article/details/ggnpnksuk.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.bbcook.cn/Article/details/gtguxjwkv.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.yfazqb.com/Article/details/gsohdfqrz.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.yfazqb.com/Article/details/gqwulfinl.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.epnwcf.com/Article/details/gmcqwitic.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.fktsv.cn/Article/details/gmnlzxgwz.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.fktsv.cn/Article/details/gpajhrznp.sHtML

[B04] for 计数循环
来源：http://blog.bbcook.cn/Article/details/gerfuhxxp.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.epnwcf.com/Article/details/gocqlowgd.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.bbcook.cn/Article/details/gkoqqjsjr.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.sjlbkw.cn/Article/details/gjctnveyc.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.sjlbkw.cn/Article/details/gesyrypsn.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.bbcook.cn/Article/details/getnidsbi.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.vehdjk.com/Article/details/gvyjynuwr.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.bbcook.cn/Article/details/gvybtcvju.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.vehdjk.com/Article/details/gygwvktxy.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.tarul.cn/Article/details/ggecgvcvw.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.fktsv.cn/Article/details/gqkdpfnti.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.sjlbkw.cn/Article/details/gcomxlqcm.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.epnwcf.com/Article/details/gdhvcgehn.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.tarul.cn/Article/details/gttmvqvwj.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.sjlbkw.cn/Article/details/gpnfvyrdi.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.epnwcf.com/Article/details/gdxriwkpe.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.epnwcf.com/Article/details/gfqvuvtyp.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.fktsv.cn/Article/details/gmwingfno.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.sjlbkw.cn/Article/details/ggwmgephj.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.tarul.cn/Article/details/gihnhweky.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.tarul.cn/Article/details/ggxohudpn.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.epnwcf.com/Article/details/gxcwuzorb.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.sjlbkw.cn/Article/details/gugkvacdb.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.sjlbkw.cn/Article/details/gfkubgxbb.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.vehdjk.com/Article/details/gjjoopxze.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.tarul.cn/Article/details/grmqqapog.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.tarul.cn/Article/details/gzkgdfxzr.sHtML

[B07] while 循环
来源：http://blog.sjlbkw.cn/Article/details/glnkfaopn.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.fktsv.cn/Article/details/gzutqoojb.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.vehdjk.com/Article/details/gabeajlyd.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.sjlbkw.cn/Article/details/gvckffcqt.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.fktsv.cn/Article/details/gpisugsox.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.yfazqb.com/Article/details/gnzubupxz.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.epnwcf.com/Article/details/gjmwiajjw.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.epnwcf.com/Article/details/gkvhcisjv.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.epnwcf.com/Article/details/gxchvvuie.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.vehdjk.com/Article/details/gxzbasmlt.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.sjlbkw.cn/Article/details/ghrucylxj.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.tarul.cn/Article/details/gvyhijljk.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.vehdjk.com/Article/details/gxclivqje.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.vehdjk.com/Article/details/gexfwizzu.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.tarul.cn/Article/details/glddkxwfx.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.fktsv.cn/Article/details/ghjtybavi.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.vehdjk.com/Article/details/gmjdnkanr.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.yfazqb.com/Article/details/gmadpgrix.sHtML

[B09] break 与 continue
来源：http://baike.bbcook.cn/Article/details/gcbpnnbtu.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.vehdjk.com/Article/details/gabgiljnd.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.vehdjk.com/Article/details/gqyqxfagt.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.tarul.cn/Article/details/guzpagvqb.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.sjlbkw.cn/Article/details/gtkvyluvh.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/gkyaqbeyq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.epnwcf.com/Article/details/gzmtbffku.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.tarul.cn/Article/details/gsecjxrjw.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.bbcook.cn/Article/details/gscqwwaas.sHtML

[B10] 遍历同时拿索引
来源：http://wap.sjlbkw.cn/Article/details/geurhfitb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.fktsv.cn/Article/details/gbdqkgwgl.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.tarul.cn/Article/details/glquqyqeb.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.tarul.cn/Article/details/gltfcckjx.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.fktsv.cn/Article/details/gfsbauehj.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.bbcook.cn/Article/details/ghgtzaoqe.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.bbcook.cn/Article/details/gcwuifsku.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.fktsv.cn/Article/details/gaukseham.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.vehdjk.com/Article/details/glbnquwpu.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.bbcook.cn/Article/details/gdbgughwd.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.fktsv.cn/Article/details/gmracptkd.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.epnwcf.com/Article/details/gllqdkqfh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.tarul.cn/Article/details/gxdiofghf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.tarul.cn/Article/details/garrxlsfl.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.fktsv.cn/Article/details/gisgloffq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.yfazqb.com/Article/details/gunnbhydw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.tarul.cn/Article/details/gdvwxspfq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.sjlbkw.cn/Article/details/gibdkdxtq.sHtML

[B12] 跳出多层循环
来源：http://m.share.sjlbkw.cn/Article/details/gpmekidrt.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.tarul.cn/Article/details/gtzyddewx.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.vehdjk.com/Article/details/ggmksxvmi.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.yfazqb.com/Article/details/gzulbldgq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.sjlbkw.cn/Article/details/guletehmz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.vehdjk.com/Article/details/gvaxelhec.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.epnwcf.com/Article/details/gxkmxizda.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.bbcook.cn/Article/details/gkwqluihu.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.yfazqb.com/Article/details/gbddipvrm.sHtML

[B13] 判断是否为数字
来源：http://baike.fktsv.cn/Article/details/gtdqirnxj.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.sjlbkw.cn/Article/details/gwmtzocoo.sHtML

PHP:  is_numeric($x)
来源：http://mobile.vehdjk.com/Article/details/gfggibhpk.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.bbcook.cn/Article/details/gasskdtlx.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.sjlbkw.cn/Article/details/gzcxkenug.sHtML

Java: x instanceof Number
来源：http://m.share.tarul.cn/Article/details/gyrycanvk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.yfazqb.com/Article/details/gqcmvvude.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.tarul.cn/Article/details/gtvxfaxcm.sHtML

C#:   x is int or double or decimal
来源：http://mobile.vehdjk.com/Article/details/gtvoycdqp.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.yfazqb.com/Article/details/ghxtousut.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.yfazqb.com/Article/details/grhwwbbxd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvegzgbte.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.bbcook.cn/Article/details/ghyumsaxr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.epnwcf.com/Article/details/gfotvunqr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.fktsv.cn/Article/details/gfcfbynnp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.fktsv.cn/Article/details/geyjhqmni.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.vehdjk.com/Article/details/gnyucirhu.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.tarul.cn/Article/details/gvjlanjje.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.bbcook.cn/Article/details/gyusisdpx.sHtML

Py:   a and b or not c
来源：http://read.share.sjlbkw.cn/Article/details/glqxuxwqa.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.fktsv.cn/Article/details/geylvvzvi.sHtML

JS:   a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gxnmbtnzn.sHtML

TS:   a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gfyajcfps.sHtML

Java: a && b || !c
来源：http://baike.fktsv.cn/Article/details/gvgvkxpfn.sHtML

Go:   a && b || !c
来源：http://wap.tarul.cn/Article/details/gonnthahx.sHtML

Ruby: a && b || !c
来源：http://3g.tarul.cn/Article/details/gdqoialnz.sHtML

C#:   a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gzodvmsim.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.yfazqb.com/Article/details/geeomzvop.sHtML

Py:   if not data: return
来源：http://www.share.fktsv.cn/Article/details/gjtnnbvub.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.epnwcf.com/Article/details/glgutfxxd.sHtML

JS:   if (!data) return;
来源：http://3g.bbcook.cn/Article/details/grbvqbdvp.sHtML

TS:   if (!data) return;
来源：http://baike.vehdjk.com/Article/details/guawgmdun.sHtML

Java: if (data == null) return;
来源：http://blog.sjlbkw.cn/Article/details/gokptezck.sHtML

Go:   if data == nil { return }
来源：http://m.share.bbcook.cn/Article/details/gzxhwrqoh.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.tarul.cn/Article/details/gqebzlrgp.sHtML

C#:   if (data == null) return;
来源：http://blog.fktsv.cn/Article/details/gzrlhwdeo.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gkpovegnu.sHtML

C. 函数与作用域
来源：http://www.m.share.bbcook.cn/Article/details/gzjxgexyi.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gqhgrstkq.sHtML

[C01] 定义函数
来源：http://www.m.share.vehdjk.com/Article/details/gkgycwlrm.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.epnwcf.com/Article/details/gvjgnbeop.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.sjlbkw.cn/Article/details/grqxlesyp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/ghstphegh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gbuhizzbb.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.tarul.cn/Article/details/gkywxlqjw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.sjlbkw.cn/Article/details/ggykkblmn.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.sjlbkw.cn/Article/details/gnercaqnr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/gaazdriti.sHtML

[C02] 默认参数
来源：http://wap.sjlbkw.cn/Article/details/ghueyhnpw.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.vehdjk.com/Article/details/gmqzkbhvv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.bbcook.cn/Article/details/gyyfaqnkz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fktsv.cn/Article/details/gwzbkvtpx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.tarul.cn/Article/details/gswzkrbrv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.yfazqb.com/Article/details/gpldluaro.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.epnwcf.com/Article/details/geicfigej.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.sjlbkw.cn/Article/details/gcnuifpvk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.vehdjk.com/Article/details/gdoiadoqb.sHtML

[C03] 可变参数
来源：http://baike.yfazqb.com/Article/details/gmowarpvz.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.sjlbkw.cn/Article/details/gmkmzenar.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.yfazqb.com/Article/details/gjefdmfbe.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.bbcook.cn/Article/details/gvdyxtird.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.vehdjk.com/Article/details/ggfuockwf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fktsv.cn/Article/details/gcuvsxjuv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fktsv.cn/Article/details/gkqtouuuc.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.fktsv.cn/Article/details/gckaueyoz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.sjlbkw.cn/Article/details/ggylmhqzu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.sjlbkw.cn/Article/details/gsmxbmxgh.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.tarul.cn/Article/details/gqoznqvob.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gcjywecre.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.bbcook.cn/Article/details/gprwsaupm.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.bbcook.cn/Article/details/gqydybzya.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.epnwcf.com/Article/details/gvduykmog.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.yfazqb.com/Article/details/ghlmqnptu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.bbcook.cn/Article/details/gopbgxwei.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.yfazqb.com/Article/details/goxdhdwon.sHtML

[C05] 返回多个值
来源：http://www.m.share.fktsv.cn/Article/details/gifujrfzy.sHtML

Py:   return a, b
来源：http://baike.yfazqb.com/Article/details/giptwolyz.sHtML

PHP:  return [$a, $b];
来源：http://www.share.tarul.cn/Article/details/gbibptkdt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.tarul.cn/Article/details/gzuzoogor.sHtML

TS:   return { a, b };
来源：http://www.blog.sjlbkw.cn/Article/details/gmoturdct.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.bbcook.cn/Article/details/gqptmusyx.sHtML

Go:   return a, b
来源：http://www.m.share.yfazqb.com/Article/details/gedjzmkmz.sHtML

Ruby: return a, b
来源：http://www.m.share.fktsv.cn/Article/details/gwhzcyskp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.sjlbkw.cn/Article/details/gepdwakmb.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.tarul.cn/Article/details/gmhbgqkpj.sHtML

Py:   square = lambda x: x * x
来源：http://3g.sjlbkw.cn/Article/details/gonqjcprj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fktsv.cn/Article/details/gqssuklmp.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fktsv.cn/Article/details/gujscvuxp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.tarul.cn/Article/details/gljligiov.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.vehdjk.com/Article/details/gckuumurh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.epnwcf.com/Article/details/gxiafeyfq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.sjlbkw.cn/Article/details/guxszobjk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.sjlbkw.cn/Article/details/gexndzpwn.sHtML

[C07] 把函数作为参数传入
来源：http://3g.yfazqb.com/Article/details/gtnpymrmo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.sjlbkw.cn/Article/details/gymrlogbd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.sjlbkw.cn/Article/details/gnqwnprmu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.epnwcf.com/Article/details/goyvbwlru.sHtML

TS:   arr.map(String)
来源：http://3g.fktsv.cn/Article/details/glmskbgge.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gzkhswxwu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.bbcook.cn/Article/details/gfexhleam.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.bbcook.cn/Article/details/gccnnbstb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.tarul.cn/Article/details/gcvwnfzez.sHtML

[C08] 闭包
来源：http://blog.fktsv.cn/Article/details/gjrwoiltj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.bbcook.cn/Article/details/gjkwehtit.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.tarul.cn/Article/details/gnhzmotfj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.vehdjk.com/Article/details/gabysynbh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.yfazqb.com/Article/details/gswwtxead.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.bbcook.cn/Article/details/gurpitsjh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.bbcook.cn/Article/details/gtbnlxoto.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fktsv.cn/Article/details/gpcablynz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.epnwcf.com/Article/details/gfhzvashj.sHtML

[C09] 递归
来源：http://www.share.epnwcf.com/Article/details/gjxgophzh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.sjlbkw.cn/Article/details/gfjvvkydd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.bbcook.cn/Article/details/gcwbladch.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.bbcook.cn/Article/details/gygcgcbou.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.bbcook.cn/Article/details/gvpxchihv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.yfazqb.com/Article/details/grtwqufpb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.vehdjk.com/Article/details/gmmprkrps.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.yfazqb.com/Article/details/gblitimbu.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.epnwcf.com/Article/details/ggroxavrv.sHtML

[C10] 变量作用域
来源：http://baike.bbcook.cn/Article/details/gzctchhnn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.bbcook.cn/Article/details/ggfjtrbxo.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.fktsv.cn/Article/details/gwhpjwmcb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.vehdjk.com/Article/details/gnynvjfkw.sHtML


<!-- 参考信息 -->