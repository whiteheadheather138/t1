代发 wailian999

C#:   (int)'A'; (char)65
来源：http://wap.fktsv.cn/Article/details/gmokcrzus.sHtML

[A19] 交换两个变量
来源：http://blog.bbcook.cn/Article/details/gjkgkltqm.sHtML

Py:   a, b = b, a
来源：http://wap.epnwcf.com/Article/details/ggouupidd.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.epnwcf.com/Article/details/gfutnrqng.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.vehdjk.com/Article/details/gbwbbylkw.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.sjlbkw.cn/Article/details/gtlcfcqlo.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.vehdjk.com/Article/details/gddpiflnw.sHtML

Go:   a, b = b, a
来源：http://mobile.sjlbkw.cn/Article/details/gchbebsfb.sHtML

Ruby: a, b = b, a
来源：http://baike.epnwcf.com/Article/details/ghdrzjede.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.yfazqb.com/Article/details/gdbzfbfpj.sHtML

[A20] 读取标准输入
来源：http://www.m.share.vehdjk.com/Article/details/gsdbirxnn.sHtML

Py:   name = input("请输入：")
来源：http://wap.sjlbkw.cn/Article/details/gfbrpcmig.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.sjlbkw.cn/Article/details/gonxtpljk.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.vehdjk.com/Article/details/gwalfscwn.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.bbcook.cn/Article/details/gxtzukqeg.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.bbcook.cn/Article/details/ghbgvsrxa.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.fktsv.cn/Article/details/gdvsnjdzm.sHtML

Ruby: gets.chomp
来源：http://mobile.tarul.cn/Article/details/gcjyxgbqs.sHtML

C#:   Console.ReadLine();
来源：http://wap.sjlbkw.cn/Article/details/gxfsudzyb.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.bbcook.cn/Article/details/gyxbhztpq.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.bbcook.cn/Article/details/gvvjknafw.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.epnwcf.com/Article/details/gsywffvim.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.vehdjk.com/Article/details/gpsqdwkwt.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.tarul.cn/Article/details/gmwfgktsa.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.bbcook.cn/Article/details/gvhylfmvf.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.epnwcf.com/Article/details/gfbylnpfv.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.sjlbkw.cn/Article/details/grvkbyxqq.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.tarul.cn/Article/details/gskjcfbja.sHtML

[A22] 获取字符串长度
来源：http://read.share.epnwcf.com/Article/details/gutuirexz.sHtML

Py:   len(s)
来源：http://wap.fktsv.cn/Article/details/gveectiog.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.vehdjk.com/Article/details/gdynxdeeu.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.tarul.cn/Article/details/gmncguasa.sHtML

TS:   s.length
来源：http://blog.bbcook.cn/Article/details/gttnfcvsy.sHtML

Java: s.length()
来源：http://m.share.yfazqb.com/Article/details/gwolqtkjn.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.tarul.cn/Article/details/gjoehosis.sHtML

Ruby: s.length
来源：http://baike.fktsv.cn/Article/details/gqfvwqfaq.sHtML

C#:   s.Length
来源：http://3g.sjlbkw.cn/Article/details/gxaqebcaa.sHtML

[A23] 大小写转换
来源：http://www.m.share.yfazqb.com/Article/details/gvmcdoqai.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.sjlbkw.cn/Article/details/glchigcdz.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.vehdjk.com/Article/details/gfkmluoqd.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.yfazqb.com/Article/details/glahsxqkr.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fktsv.cn/Article/details/glqvsywyo.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fktsv.cn/Article/details/gzixrkjpu.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.bbcook.cn/Article/details/gptdqyxog.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.tarul.cn/Article/details/gatbhxked.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.vehdjk.com/Article/details/giqprgztd.sHtML

[A24] 去除首尾空白
来源：http://3g.tarul.cn/Article/details/ghqzkzahz.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.epnwcf.com/Article/details/gjsnqxowg.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.epnwcf.com/Article/details/gpqjsneie.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.sjlbkw.cn/Article/details/gltylciyo.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.sjlbkw.cn/Article/details/gzoftgdjn.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.yfazqb.com/Article/details/ginwlqwme.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.fktsv.cn/Article/details/gtmyxkhjs.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.yfazqb.com/Article/details/ggxwqodfm.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.yfazqb.com/Article/details/gqlotprfl.sHtML

[A25] 字符串比较
来源：http://wap.sjlbkw.cn/Article/details/gekimhlnc.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.epnwcf.com/Article/details/ghwxitlqo.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.bbcook.cn/Article/details/gmnmdfrpr.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.epnwcf.com/Article/details/gfefhgqrf.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.vehdjk.com/Article/details/gjocfmdol.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.epnwcf.com/Article/details/gkdwhlyrh.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.vehdjk.com/Article/details/gawoossau.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.epnwcf.com/Article/details/grnbaxcny.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.vehdjk.com/Article/details/grenchknp.sHtML

[A26] 类型转换总览
来源：http://www.share.epnwcf.com/Article/details/gijsdvsfo.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.sjlbkw.cn/Article/details/gnxstvgsw.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.bbcook.cn/Article/details/gcxxtrlwy.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.tarul.cn/Article/details/ghhkpktbi.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.fktsv.cn/Article/details/gtemzeete.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.bbcook.cn/Article/details/gdwlkoihd.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.bbcook.cn/Article/details/gyyaqqsnn.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.bbcook.cn/Article/details/gbmevflao.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.yfazqb.com/Article/details/gmgbvkpoi.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/grxgipeup.sHtML

B. 流程控制
来源：http://mobile.bbcook.cn/Article/details/gatofvmxj.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gcomvycjj.sHtML

[B01] 条件判断 if / else
来源：http://wap.bbcook.cn/Article/details/gufgvniyf.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.tarul.cn/Article/details/gaameizbs.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkvxylgwt.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.epnwcf.com/Article/details/gdbmizbzx.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.epnwcf.com/Article/details/gthykeufc.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.tarul.cn/Article/details/gbjfklmoi.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.fktsv.cn/Article/details/gmouehxwl.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.bbcook.cn/Article/details/gsceycqwg.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.sjlbkw.cn/Article/details/gmhdqjcdm.sHtML

[B02] 多分支 else if / elif
来源：http://baike.sjlbkw.cn/Article/details/gexbghcda.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.bbcook.cn/Article/details/ghrwniyyh.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.epnwcf.com/Article/details/grhswmden.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.tarul.cn/Article/details/ghzqmgtfl.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.sjlbkw.cn/Article/details/gdnevvnvj.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.vehdjk.com/Article/details/gnelzbyeo.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.fktsv.cn/Article/details/greklxnrz.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.sjlbkw.cn/Article/details/gmjeqthyb.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.epnwcf.com/Article/details/ggwewgbov.sHtML

[B03] switch / match / case
来源：http://www.m.share.bbcook.cn/Article/details/gxplccxrv.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.tarul.cn/Article/details/gdqoiecxv.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.sjlbkw.cn/Article/details/govhjrzlx.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.vehdjk.com/Article/details/gralbnpsy.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.tarul.cn/Article/details/gqnckehuy.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.tarul.cn/Article/details/gxtsqhffe.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.tarul.cn/Article/details/ggixajvjg.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.epnwcf.com/Article/details/givlnddgo.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.epnwcf.com/Article/details/gieimalfm.sHtML

[B04] for 计数循环
来源：http://mobile.yfazqb.com/Article/details/gjgzbgkyk.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.tarul.cn/Article/details/gkqkmdqfm.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.yfazqb.com/Article/details/geulowpmj.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.tarul.cn/Article/details/gepykzttl.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.tarul.cn/Article/details/gahwmulkv.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.vehdjk.com/Article/details/gbfftvkzw.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.tarul.cn/Article/details/gfoqjowhh.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.epnwcf.com/Article/details/glyhhpyyp.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.sjlbkw.cn/Article/details/gcwqjlnwg.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.tarul.cn/Article/details/gusxxznuy.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.epnwcf.com/Article/details/gytdzhthw.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.yfazqb.com/Article/details/gxeugskjy.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.sjlbkw.cn/Article/details/grtlpclhp.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.fktsv.cn/Article/details/gsezdjxhq.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.vehdjk.com/Article/details/gbzqoajsn.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.yfazqb.com/Article/details/gozlaotsh.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.bbcook.cn/Article/details/gxyfjqasg.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.vehdjk.com/Article/details/gkwijjjtx.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.bbcook.cn/Article/details/gfjnmxylx.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.tarul.cn/Article/details/gmqkpzydc.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.epnwcf.com/Article/details/goqtkyhwv.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.epnwcf.com/Article/details/gfjdwfzzp.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.yfazqb.com/Article/details/gwaoniooc.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.bbcook.cn/Article/details/grhpaptrm.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.sjlbkw.cn/Article/details/gxkhluckk.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.fktsv.cn/Article/details/ghviiefso.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.vehdjk.com/Article/details/gisbhvjbz.sHtML

[B07] while 循环
来源：http://3g.fktsv.cn/Article/details/guxfjsdbx.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.yfazqb.com/Article/details/gfhahgdsy.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.tarul.cn/Article/details/gshqklsgj.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.tarul.cn/Article/details/gbixocvrr.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.yfazqb.com/Article/details/gxsksnpcd.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.fktsv.cn/Article/details/gbyibqqnw.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.fktsv.cn/Article/details/gehzcdoeb.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.yfazqb.com/Article/details/gjtkqsvvq.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.epnwcf.com/Article/details/gmiukecry.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.yfazqb.com/Article/details/gqkturnch.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.bbcook.cn/Article/details/gquonjkqt.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.vehdjk.com/Article/details/gyptbrflb.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.tarul.cn/Article/details/gspockrnw.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.vehdjk.com/Article/details/gpuqujexk.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.bbcook.cn/Article/details/gaqliaooj.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.yfazqb.com/Article/details/gxtpzrcje.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.epnwcf.com/Article/details/gccilpusy.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvvirgnhy.sHtML

[B09] break 与 continue
来源：http://m.share.bbcook.cn/Article/details/geqqtbwnp.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.sjlbkw.cn/Article/details/gugrwkswy.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.epnwcf.com/Article/details/gcwzyrurc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.vehdjk.com/Article/details/gtsdasylb.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.vehdjk.com/Article/details/gwdgdoxqa.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.vehdjk.com/Article/details/gfkwivhvl.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.sjlbkw.cn/Article/details/gyrfskjqe.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.fktsv.cn/Article/details/glsodhrbv.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.tarul.cn/Article/details/gfcmqqmlw.sHtML

[B10] 遍历同时拿索引
来源：http://3g.tarul.cn/Article/details/geeipguki.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.sjlbkw.cn/Article/details/gqchkyuzr.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.tarul.cn/Article/details/gfbjkynjx.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.fktsv.cn/Article/details/gynqsugre.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.sjlbkw.cn/Article/details/gsrafngvn.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.fktsv.cn/Article/details/gkxsinohm.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.bbcook.cn/Article/details/guuljgedz.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.bbcook.cn/Article/details/giyfeqtgt.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.fktsv.cn/Article/details/gkengtgom.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.vehdjk.com/Article/details/ghnhjdsns.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.bbcook.cn/Article/details/ghrijahvr.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.epnwcf.com/Article/details/gyvukhyjp.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.bbcook.cn/Article/details/golyfujtk.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.yfazqb.com/Article/details/gmnxrsiys.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.fktsv.cn/Article/details/gnsqjxykd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.sjlbkw.cn/Article/details/giafujdma.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.tarul.cn/Article/details/ggtelnlai.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.sjlbkw.cn/Article/details/ggctswadu.sHtML

[B12] 跳出多层循环
来源：http://m.share.yfazqb.com/Article/details/gtklaalwv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.sjlbkw.cn/Article/details/gswbwkwle.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.tarul.cn/Article/details/gnrkmyggl.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.epnwcf.com/Article/details/glgvdvixq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.vehdjk.com/Article/details/gowzkwpmm.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fktsv.cn/Article/details/gobbybrmj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.sjlbkw.cn/Article/details/gjhzcwwkw.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.vehdjk.com/Article/details/gccomfdpp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.epnwcf.com/Article/details/gzghssgmz.sHtML

[B13] 判断是否为数字
来源：http://wap.fktsv.cn/Article/details/gnjqzygfe.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.sjlbkw.cn/Article/details/gqktwykty.sHtML

PHP:  is_numeric($x)
来源：http://www.share.yfazqb.com/Article/details/grjwvnkvv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.vehdjk.com/Article/details/grxklbjur.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.sjlbkw.cn/Article/details/gnxtzdksz.sHtML

Java: x instanceof Number
来源：http://mobile.vehdjk.com/Article/details/gwekcvtvb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.yfazqb.com/Article/details/guxdyjsju.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.yfazqb.com/Article/details/gxrsknlpz.sHtML

C#:   x is int or double or decimal
来源：http://read.share.yfazqb.com/Article/details/gdgtuowbb.sHtML

[B14] 判断值是否在集合内
来源：http://wap.bbcook.cn/Article/details/gzgrlkgnv.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.yfazqb.com/Article/details/geaiurvmb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.yfazqb.com/Article/details/gpwkveyvd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.vehdjk.com/Article/details/gdolineik.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.vehdjk.com/Article/details/gtrvxjasu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.vehdjk.com/Article/details/ggqotkmch.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.epnwcf.com/Article/details/ghmswwkzq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.vehdjk.com/Article/details/gpogrohsv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.epnwcf.com/Article/details/gogfmydxh.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.sjlbkw.cn/Article/details/gosbdjfja.sHtML

Py:   a and b or not c
来源：http://www.m.share.yfazqb.com/Article/details/gvhpvamvq.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.tarul.cn/Article/details/gmksbxsle.sHtML

JS:   a && b || !c
来源：http://mobile.vehdjk.com/Article/details/gwbwflymc.sHtML

TS:   a && b || !c
来源：http://wap.epnwcf.com/Article/details/gumefmnyv.sHtML

Java: a && b || !c
来源：http://3g.bbcook.cn/Article/details/gcqrmzzsj.sHtML

Go:   a && b || !c
来源：http://read.share.tarul.cn/Article/details/gxmcaqrjy.sHtML

Ruby: a && b || !c
来源：http://www.share.tarul.cn/Article/details/gwdevtazq.sHtML

C#:   a && b || !c
来源：http://blog.fktsv.cn/Article/details/gvpelzjlf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.epnwcf.com/Article/details/ghliltltp.sHtML

Py:   if not data: return
来源：http://read.share.epnwcf.com/Article/details/gwaqlpfka.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.vehdjk.com/Article/details/ggqoxmfbm.sHtML

JS:   if (!data) return;
来源：http://www.m.share.yfazqb.com/Article/details/gwmznnyxi.sHtML

TS:   if (!data) return;
来源：http://read.share.bbcook.cn/Article/details/ggaukpbnv.sHtML

Java: if (data == null) return;
来源：http://www.m.share.bbcook.cn/Article/details/gbqavcmvt.sHtML

Go:   if data == nil { return }
来源：http://wap.fktsv.cn/Article/details/gjepvmnis.sHtML

Ruby: return if data.nil?
来源：http://3g.tarul.cn/Article/details/grimjetgg.sHtML

C#:   if (data == null) return;
来源：http://blog.sjlbkw.cn/Article/details/glxgyxbzn.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gizqjykqx.sHtML

C. 函数与作用域
来源：http://mobile.fktsv.cn/Article/details/gsbomczew.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gdrkedcpq.sHtML

[C01] 定义函数
来源：http://www.m.share.fktsv.cn/Article/details/gjgslygrk.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fktsv.cn/Article/details/grhsafmjw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.vehdjk.com/Article/details/ghbugabfv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.vehdjk.com/Article/details/gvcuwttfq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.tarul.cn/Article/details/gnbgzczfv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/gmvukinyj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.tarul.cn/Article/details/gxvwnadoz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.bbcook.cn/Article/details/gxjfpilzl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/ghaphoehs.sHtML

[C02] 默认参数
来源：http://wap.epnwcf.com/Article/details/gbreplgxh.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.epnwcf.com/Article/details/gfgeqxnsy.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.tarul.cn/Article/details/gsvcppzhi.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.bbcook.cn/Article/details/gdrimhqjl.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gsvbqnolg.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.epnwcf.com/Article/details/gxjmsphci.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.epnwcf.com/Article/details/gwdquztzb.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.yfazqb.com/Article/details/ghqflsdqf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.vehdjk.com/Article/details/gpfpzwdeb.sHtML

[C03] 可变参数
来源：http://read.share.fktsv.cn/Article/details/goldsvxiw.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.bbcook.cn/Article/details/gcpoynjpt.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.bbcook.cn/Article/details/glxufrabt.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.epnwcf.com/Article/details/gcgjjtupu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.yfazqb.com/Article/details/gjweppvez.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.bbcook.cn/Article/details/gneeiknzd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.epnwcf.com/Article/details/grsxgdrgv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.tarul.cn/Article/details/gwqgarwoe.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.yfazqb.com/Article/details/gezeuccsl.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.sjlbkw.cn/Article/details/gcnqenvwm.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.yfazqb.com/Article/details/gnftfcear.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.sjlbkw.cn/Article/details/ggbyuyzuz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.epnwcf.com/Article/details/gfmstjlze.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.epnwcf.com/Article/details/gnzzkvmfc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.sjlbkw.cn/Article/details/gnrocdjzh.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.vehdjk.com/Article/details/gfmfihqsp.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.bbcook.cn/Article/details/gjcgsfuau.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.yfazqb.com/Article/details/guhawsaei.sHtML

[C05] 返回多个值
来源：http://wap.vehdjk.com/Article/details/ggodybvnh.sHtML

Py:   return a, b
来源：http://www.m.share.tarul.cn/Article/details/gcgdkdepu.sHtML

PHP:  return [$a, $b];
来源：http://blog.sjlbkw.cn/Article/details/gganuvrmm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.sjlbkw.cn/Article/details/gbcejbdka.sHtML

TS:   return { a, b };
来源：http://blog.vehdjk.com/Article/details/gukhlcvrr.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fktsv.cn/Article/details/gurnlmhsk.sHtML

Go:   return a, b
来源：http://3g.bbcook.cn/Article/details/guosnxmeh.sHtML

Ruby: return a, b
来源：http://blog.epnwcf.com/Article/details/gougiojss.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.epnwcf.com/Article/details/gqodgjqyv.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.vehdjk.com/Article/details/ginipybmo.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fktsv.cn/Article/details/gtbbluqfz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.fktsv.cn/Article/details/gflsdrufv.sHtML

JS:   const square = x => x * x;
来源：http://read.share.tarul.cn/Article/details/gnwudblrf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.yfazqb.com/Article/details/gijnokmls.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fktsv.cn/Article/details/glwanknid.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.sjlbkw.cn/Article/details/guykptpna.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.sjlbkw.cn/Article/details/ghbhlbqzb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.sjlbkw.cn/Article/details/gohfsuqwv.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fktsv.cn/Article/details/gtwiphsqj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.tarul.cn/Article/details/gavytttfr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.bbcook.cn/Article/details/gsawwymhn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.yfazqb.com/Article/details/gntabsjxy.sHtML

TS:   arr.map(String)
来源：http://3g.yfazqb.com/Article/details/gkrarjifx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.sjlbkw.cn/Article/details/gmpzhfyvf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fktsv.cn/Article/details/guiuotnya.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.fktsv.cn/Article/details/gzyjasyvr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.epnwcf.com/Article/details/gcckvnpag.sHtML

[C08] 闭包
来源：http://read.share.tarul.cn/Article/details/gskxelyae.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.tarul.cn/Article/details/gqmnrfxvx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.bbcook.cn/Article/details/gkhxpzwvw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.tarul.cn/Article/details/gjuskegwk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.vehdjk.com/Article/details/gevycdalg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.epnwcf.com/Article/details/ghjnbjkop.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.epnwcf.com/Article/details/gnozjyght.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fktsv.cn/Article/details/grptdculu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.yfazqb.com/Article/details/gwxfljbjz.sHtML

[C09] 递归
来源：http://www.share.yfazqb.com/Article/details/gjxohnmqg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.tarul.cn/Article/details/gucuwtdaj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.bbcook.cn/Article/details/grjziwcvg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.tarul.cn/Article/details/grrgnbayo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.epnwcf.com/Article/details/gudzueqyh.sHtML


<!-- 参考信息 -->