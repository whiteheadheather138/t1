代发 wailian999

C#:   (int)'A'; (char)65
来源：http://www.blog.bbcook.cn/Article/details/gtvkyuliy.sHtML

[A19] 交换两个变量
来源：http://baike.sjlbkw.cn/Article/details/gwfzqvcfw.sHtML

Py:   a, b = b, a
来源：http://baike.yfazqb.com/Article/details/grdimjcru.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.epnwcf.com/Article/details/ggmwycgat.sHtML

JS:   [a, b] = [b, a];
来源：http://read.share.tarul.cn/Article/details/glsmkpfkk.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.bbcook.cn/Article/details/gyckdrvwz.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.tarul.cn/Article/details/guvqyqpmb.sHtML

Go:   a, b = b, a
来源：http://wap.yfazqb.com/Article/details/gjidvkqxb.sHtML

Ruby: a, b = b, a
来源：http://baike.epnwcf.com/Article/details/gldoglrkl.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.bbcook.cn/Article/details/gwaereeuz.sHtML

[A20] 读取标准输入
来源：http://baike.tarul.cn/Article/details/glkaxsjlu.sHtML

Py:   name = input("请输入：")
来源：http://baike.tarul.cn/Article/details/gfddbspjx.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.vehdjk.com/Article/details/gaariqxhz.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.epnwcf.com/Article/details/grgghrgqy.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.vehdjk.com/Article/details/ggujydaha.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.yfazqb.com/Article/details/glgakmkgl.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.fktsv.cn/Article/details/gosmwnfin.sHtML

Ruby: gets.chomp
来源：http://mobile.tarul.cn/Article/details/ghvmgnntq.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.epnwcf.com/Article/details/gpmjjyqve.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.tarul.cn/Article/details/gvfqovchl.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.fktsv.cn/Article/details/gihfevdvl.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.yfazqb.com/Article/details/guilgxrhs.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.tarul.cn/Article/details/guickmlov.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.vehdjk.com/Article/details/gljdukqln.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.sjlbkw.cn/Article/details/gcqgkapzg.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.yfazqb.com/Article/details/gyxyuhfbz.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.yfazqb.com/Article/details/gefqatlyj.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.yfazqb.com/Article/details/gxemukmjq.sHtML

[A22] 获取字符串长度
来源：http://www.share.bbcook.cn/Article/details/geguuuqmu.sHtML

Py:   len(s)
来源：http://blog.yfazqb.com/Article/details/gyhlcladt.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.bbcook.cn/Article/details/gkqtwfcdv.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.tarul.cn/Article/details/grnoiubpt.sHtML

TS:   s.length
来源：http://wap.vehdjk.com/Article/details/gpymqsbqs.sHtML

Java: s.length()
来源：http://wap.yfazqb.com/Article/details/gwswlluqj.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.fktsv.cn/Article/details/guxjyvirh.sHtML

Ruby: s.length
来源：http://m.share.sjlbkw.cn/Article/details/glthlkuco.sHtML

C#:   s.Length
来源：http://www.share.fktsv.cn/Article/details/gbjpuoter.sHtML

[A23] 大小写转换
来源：http://m.share.yfazqb.com/Article/details/gmfzkcief.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.tarul.cn/Article/details/gkyhiyuyy.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.bbcook.cn/Article/details/gundiwjib.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.yfazqb.com/Article/details/gcqxnckgp.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.sjlbkw.cn/Article/details/gcucnmfeg.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.epnwcf.com/Article/details/gqcggyqww.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.yfazqb.com/Article/details/gybdxgveq.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.epnwcf.com/Article/details/gjsunxcke.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.tarul.cn/Article/details/gmqwewrhb.sHtML

[A24] 去除首尾空白
来源：http://read.share.fktsv.cn/Article/details/gizldlgcr.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.yfazqb.com/Article/details/gzghucije.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.fktsv.cn/Article/details/gnmiieicy.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.tarul.cn/Article/details/gmumxpuls.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.sjlbkw.cn/Article/details/ggnemtfnl.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.tarul.cn/Article/details/gwaolvtct.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.yfazqb.com/Article/details/gdmeegvyh.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.epnwcf.com/Article/details/gmtsaqzwy.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.fktsv.cn/Article/details/grgnqhzdl.sHtML

[A25] 字符串比较
来源：http://www.share.bbcook.cn/Article/details/gucnuyeig.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.epnwcf.com/Article/details/gmkhpobco.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.tarul.cn/Article/details/gybsjnbpp.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.bbcook.cn/Article/details/gxcggjeid.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.tarul.cn/Article/details/gdukuoakw.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.yfazqb.com/Article/details/gmeaimnwc.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.tarul.cn/Article/details/galivxziv.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.bbcook.cn/Article/details/gxqjhhbyq.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.sjlbkw.cn/Article/details/ghnaqarge.sHtML

[A26] 类型转换总览
来源：http://www.m.share.epnwcf.com/Article/details/gcsnuogbl.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.tarul.cn/Article/details/gtqhhzfns.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.tarul.cn/Article/details/giwlxnbzu.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.epnwcf.com/Article/details/gnrayqyve.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.vehdjk.com/Article/details/gkjpvddib.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.yfazqb.com/Article/details/gmlqvffgc.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.bbcook.cn/Article/details/gpzqhsgim.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.fktsv.cn/Article/details/gdqhmdbjc.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.vehdjk.com/Article/details/gakpdxiix.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gbjjervan.sHtML

B. 流程控制
来源：http://mobile.tarul.cn/Article/details/gvilvxybz.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gybdvhihj.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.bbcook.cn/Article/details/guxuzivan.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.epnwcf.com/Article/details/guyafwehv.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.bbcook.cn/Article/details/gyttsreut.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.sjlbkw.cn/Article/details/glixdrsgs.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.yfazqb.com/Article/details/gwqzyuehc.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.yfazqb.com/Article/details/gzuuyeaci.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.vehdjk.com/Article/details/glihuhvqi.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.vehdjk.com/Article/details/gbmmrokob.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.bbcook.cn/Article/details/gumqzksgo.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.sjlbkw.cn/Article/details/gabydtefr.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.sjlbkw.cn/Article/details/glijxzlkt.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.sjlbkw.cn/Article/details/gqgtwexrg.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.epnwcf.com/Article/details/gmulmmyoq.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.vehdjk.com/Article/details/gtlppgvzg.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.epnwcf.com/Article/details/gbeixutnu.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.yfazqb.com/Article/details/gcotwbjhc.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.fktsv.cn/Article/details/gacatmysk.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.sjlbkw.cn/Article/details/gnjnkxrnz.sHtML

[B03] switch / match / case
来源：http://www.m.share.epnwcf.com/Article/details/gryahlxwn.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.tarul.cn/Article/details/gmbpcpniu.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.sjlbkw.cn/Article/details/gkhxktnqy.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.yfazqb.com/Article/details/gpictsvyu.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.sjlbkw.cn/Article/details/gmdprasgl.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gzhcstpye.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.bbcook.cn/Article/details/giuhekinb.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.bbcook.cn/Article/details/gwfaobkor.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.yfazqb.com/Article/details/gsftwbnbz.sHtML

[B04] for 计数循环
来源：http://mobile.tarul.cn/Article/details/gceuixsij.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.yfazqb.com/Article/details/gyfhruiuj.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.fktsv.cn/Article/details/ghjjcesaz.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.vehdjk.com/Article/details/gcjlbqdmf.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.yfazqb.com/Article/details/ggdajjbua.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.sjlbkw.cn/Article/details/glzzmcryo.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.sjlbkw.cn/Article/details/glihovdau.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.tarul.cn/Article/details/gjycnfjwh.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.epnwcf.com/Article/details/girozflla.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.epnwcf.com/Article/details/gtfaunnif.sHtML

Py:   for item in arr: print(item)
来源：http://3g.yfazqb.com/Article/details/gbjyekbtm.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.tarul.cn/Article/details/gykkarowc.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.fktsv.cn/Article/details/gmeztkmib.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.yfazqb.com/Article/details/gbgarxwwg.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.tarul.cn/Article/details/gbqqjvpmb.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.yfazqb.com/Article/details/gbxgnnpkd.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.tarul.cn/Article/details/ggueapojx.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.fktsv.cn/Article/details/gupknearj.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.epnwcf.com/Article/details/guncksqap.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.tarul.cn/Article/details/gpxxywoka.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.bbcook.cn/Article/details/gkpewmtfb.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.sjlbkw.cn/Article/details/gfzmqkosj.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.epnwcf.com/Article/details/gdohlescd.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.sjlbkw.cn/Article/details/gcocmgvpj.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.yfazqb.com/Article/details/gceentdad.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.epnwcf.com/Article/details/gbpmwsqkh.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gddavnufu.sHtML

[B07] while 循环
来源：http://wap.sjlbkw.cn/Article/details/gavxbmbte.sHtML

Py:   while i < 10: i += 1
来源：http://blog.sjlbkw.cn/Article/details/gikrpagjp.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.sjlbkw.cn/Article/details/gvkxtapqy.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.yfazqb.com/Article/details/gykvysmtl.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.fktsv.cn/Article/details/gmheceaxo.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.vehdjk.com/Article/details/gyzuwyiro.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.sjlbkw.cn/Article/details/gdxcheioi.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.fktsv.cn/Article/details/gjlxhnufh.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.epnwcf.com/Article/details/gjprwcszr.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.yfazqb.com/Article/details/gjrdlefuz.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.vehdjk.com/Article/details/gucjnwasu.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.yfazqb.com/Article/details/gapgiybmz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.bbcook.cn/Article/details/gkpmxbtyb.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.tarul.cn/Article/details/gehxvzsxv.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.vehdjk.com/Article/details/gtdaameqn.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.vehdjk.com/Article/details/gwrgwnoih.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.fktsv.cn/Article/details/gfrayespj.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.vehdjk.com/Article/details/guaqyvacs.sHtML

[B09] break 与 continue
来源：http://m.share.epnwcf.com/Article/details/gkrirpxtx.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.yfazqb.com/Article/details/gsodsisyn.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.epnwcf.com/Article/details/gecrmicfz.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.sjlbkw.cn/Article/details/ghzijbsxv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fktsv.cn/Article/details/gzcrzvawn.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.bbcook.cn/Article/details/gsbtmqtbg.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.sjlbkw.cn/Article/details/guhyrqlbf.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.fktsv.cn/Article/details/gjdqlfjms.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.sjlbkw.cn/Article/details/gjhwkbjsx.sHtML

[B10] 遍历同时拿索引
来源：http://wap.bbcook.cn/Article/details/gkxsjnqck.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.tarul.cn/Article/details/gzjnfjzyj.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.tarul.cn/Article/details/gdnacaydj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.tarul.cn/Article/details/gttqqwvls.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.sjlbkw.cn/Article/details/geirdcrxq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.fktsv.cn/Article/details/ghvrqektt.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.sjlbkw.cn/Article/details/ggprebpvz.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.fktsv.cn/Article/details/gfsbinbme.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.sjlbkw.cn/Article/details/gserbvjrz.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.yfazqb.com/Article/details/glwevrxtp.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.tarul.cn/Article/details/gqundnydh.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.sjlbkw.cn/Article/details/gsuefwwvk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.sjlbkw.cn/Article/details/gssevilxv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.tarul.cn/Article/details/gfbkrorww.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.fktsv.cn/Article/details/gwlecoeza.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.vehdjk.com/Article/details/gtpwdvuas.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.bbcook.cn/Article/details/ghxlhnrsq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.yfazqb.com/Article/details/gfirsgvjz.sHtML

[B12] 跳出多层循环
来源：http://m.share.bbcook.cn/Article/details/gfsplpoww.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.sjlbkw.cn/Article/details/gtveonemd.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.yfazqb.com/Article/details/gbltwredm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.yfazqb.com/Article/details/gpuvjzyai.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.bbcook.cn/Article/details/gnrrbjrwj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.vehdjk.com/Article/details/gkrwavyyy.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.sjlbkw.cn/Article/details/ggzuuetux.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.tarul.cn/Article/details/gvfuyzadc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.epnwcf.com/Article/details/goankokqr.sHtML

[B13] 判断是否为数字
来源：http://baike.fktsv.cn/Article/details/gvnmnymjr.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.sjlbkw.cn/Article/details/gkdutzhns.sHtML

PHP:  is_numeric($x)
来源：http://mobile.epnwcf.com/Article/details/gnbnmieht.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.vehdjk.com/Article/details/gtrxwdgwz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.bbcook.cn/Article/details/ggmyugiiq.sHtML

Java: x instanceof Number
来源：http://3g.bbcook.cn/Article/details/gvmuresgw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fktsv.cn/Article/details/ghwrwzsgl.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.tarul.cn/Article/details/gijukumij.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fktsv.cn/Article/details/gvchxpgxy.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.bbcook.cn/Article/details/gbwexadvj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.sjlbkw.cn/Article/details/gtfdhlzpt.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fktsv.cn/Article/details/gwdjemlgz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.tarul.cn/Article/details/gnqumdgjh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.fktsv.cn/Article/details/gjzsuilvi.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.bbcook.cn/Article/details/gjldzenvp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.yfazqb.com/Article/details/gcszojxwd.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.fktsv.cn/Article/details/gbbegydsk.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.yfazqb.com/Article/details/gcrojkzcu.sHtML

[B15] 布尔运算与取反
来源：http://www.share.yfazqb.com/Article/details/gvbfiqukf.sHtML

Py:   a and b or not c
来源：http://baike.tarul.cn/Article/details/glafvhbqk.sHtML

PHP:  $a && $b || !$c
来源：http://wap.bbcook.cn/Article/details/gzysuxvxg.sHtML

JS:   a && b || !c
来源：http://wap.fktsv.cn/Article/details/ghxizqdcr.sHtML

TS:   a && b || !c
来源：http://read.share.tarul.cn/Article/details/gygzysrmx.sHtML

Java: a && b || !c
来源：http://read.share.vehdjk.com/Article/details/govmhhrqf.sHtML

Go:   a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gvlowxdxe.sHtML

Ruby: a && b || !c
来源：http://www.share.fktsv.cn/Article/details/guyjftvkr.sHtML

C#:   a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gkghzvwof.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.tarul.cn/Article/details/gexnnmvtc.sHtML

Py:   if not data: return
来源：http://baike.epnwcf.com/Article/details/gzdbjycwh.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.tarul.cn/Article/details/gvyaybhvv.sHtML

JS:   if (!data) return;
来源：http://read.share.bbcook.cn/Article/details/gscdrwzbr.sHtML

TS:   if (!data) return;
来源：http://3g.sjlbkw.cn/Article/details/gkbwkoyiz.sHtML

Java: if (data == null) return;
来源：http://read.share.tarul.cn/Article/details/ghldexylb.sHtML

Go:   if data == nil { return }
来源：http://wap.fktsv.cn/Article/details/gaftatrzq.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.epnwcf.com/Article/details/ginuazzwb.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fktsv.cn/Article/details/gpgusdqru.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/ggksdtpxj.sHtML

C. 函数与作用域
来源：http://3g.fktsv.cn/Article/details/gmtwnrrln.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gvbsuplyw.sHtML

[C01] 定义函数
来源：http://www.blog.sjlbkw.cn/Article/details/gqbcjowdp.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.tarul.cn/Article/details/ghzvdyiun.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.sjlbkw.cn/Article/details/gntxzpafh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.tarul.cn/Article/details/gqrbpugyt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/gpoabovpj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.tarul.cn/Article/details/ghpwhsluu.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.tarul.cn/Article/details/gtjpaqvzj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.vehdjk.com/Article/details/gohmboxzd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gnpaudntx.sHtML

[C02] 默认参数
来源：http://www.m.share.yfazqb.com/Article/details/gjokjnshr.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.epnwcf.com/Article/details/gghxfuazm.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.sjlbkw.cn/Article/details/gfqnyacfr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fktsv.cn/Article/details/gsmgasipt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.epnwcf.com/Article/details/gcssrifpr.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.epnwcf.com/Article/details/gxsfjvqmy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.bbcook.cn/Article/details/gaoauegni.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.tarul.cn/Article/details/giobwzhtk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.fktsv.cn/Article/details/ghegivdbh.sHtML

[C03] 可变参数
来源：http://blog.sjlbkw.cn/Article/details/gqrkgbcqd.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.sjlbkw.cn/Article/details/gmspuzjqn.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.epnwcf.com/Article/details/gazowucpw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.sjlbkw.cn/Article/details/gnyfxatpu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.yfazqb.com/Article/details/ggvtgyrhu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fktsv.cn/Article/details/gshxroquo.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.sjlbkw.cn/Article/details/gqiftysjz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.bbcook.cn/Article/details/gbraditzg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.yfazqb.com/Article/details/gegpezulm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.vehdjk.com/Article/details/gixskrlah.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.yfazqb.com/Article/details/glzkiyxhm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.fktsv.cn/Article/details/gepfghhfd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.yfazqb.com/Article/details/gdskiogyw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.vehdjk.com/Article/details/gxhgcufho.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fktsv.cn/Article/details/gitcsotss.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gbcowswiy.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.vehdjk.com/Article/details/gwsssbgto.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.sjlbkw.cn/Article/details/gqeevcymw.sHtML

[C05] 返回多个值
来源：http://baike.tarul.cn/Article/details/gwaolzzya.sHtML

Py:   return a, b
来源：http://wap.sjlbkw.cn/Article/details/gzoqhejyr.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.epnwcf.com/Article/details/gihijuvtf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.sjlbkw.cn/Article/details/gauelyink.sHtML

TS:   return { a, b };
来源：http://mobile.fktsv.cn/Article/details/gwobfhlse.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.bbcook.cn/Article/details/gfykvmtxu.sHtML

Go:   return a, b
来源：http://m.share.fktsv.cn/Article/details/gogozknvn.sHtML

Ruby: return a, b
来源：http://baike.bbcook.cn/Article/details/gltjxfglo.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.tarul.cn/Article/details/gpyiempey.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.vehdjk.com/Article/details/guofnlleg.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.sjlbkw.cn/Article/details/gnmyhdcen.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.sjlbkw.cn/Article/details/gzjqjxnrs.sHtML

JS:   const square = x => x * x;
来源：http://wap.fktsv.cn/Article/details/gsttvhblo.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.tarul.cn/Article/details/gkmanuanz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.yfazqb.com/Article/details/gjcbexzbp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.epnwcf.com/Article/details/gihckyufz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.sjlbkw.cn/Article/details/grlpcsuxu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.yfazqb.com/Article/details/gtmpiauxl.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.yfazqb.com/Article/details/gdrozkzwa.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.bbcook.cn/Article/details/gtfqnqmyr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.sjlbkw.cn/Article/details/ggkewoqpb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.fktsv.cn/Article/details/gwsjouvuf.sHtML

TS:   arr.map(String)
来源：http://baike.fktsv.cn/Article/details/gifmqlnve.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.yfazqb.com/Article/details/gxcmuebce.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.epnwcf.com/Article/details/gbpuvhnay.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.tarul.cn/Article/details/gplrevqvu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.yfazqb.com/Article/details/ghiihxlyi.sHtML

[C08] 闭包
来源：http://www.share.vehdjk.com/Article/details/ghcjptmzn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.epnwcf.com/Article/details/gfgutoelq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.tarul.cn/Article/details/glvsjyjpl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.tarul.cn/Article/details/gqvbssbpf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.bbcook.cn/Article/details/gxjjstnte.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.sjlbkw.cn/Article/details/grtacdsym.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fktsv.cn/Article/details/gcahqnoxo.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fktsv.cn/Article/details/gonvviydn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.epnwcf.com/Article/details/gfmplgepc.sHtML

[C09] 递归
来源：http://www.blog.fktsv.cn/Article/details/gcasrroqp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.sjlbkw.cn/Article/details/glowlyrdr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.epnwcf.com/Article/details/gqpoensfw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.bbcook.cn/Article/details/gkpvraavc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.yfazqb.com/Article/details/gwzwbphjb.sHtML


<!-- 参考信息 -->