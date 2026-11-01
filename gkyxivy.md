代发 wailian999

Ruby: a, b = b, a
来源：http://m.share.epnwcf.com/Article/details/gwzkevxnw.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.yfazqb.com/Article/details/gmxcuttwj.sHtML

[A20] 读取标准输入
来源：http://www.share.yfazqb.com/Article/details/gxonsaswe.sHtML

Py:   name = input("请输入：")
来源：http://www.share.bbcook.cn/Article/details/gojmmrizx.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.vehdjk.com/Article/details/ggfmfvklr.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.sjlbkw.cn/Article/details/gppwnkkkx.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.epnwcf.com/Article/details/gkfcptrqr.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.yfazqb.com/Article/details/gwvzfjhbf.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.fktsv.cn/Article/details/gavcrhczc.sHtML

Ruby: gets.chomp
来源：http://wap.tarul.cn/Article/details/gspprdvsa.sHtML

C#:   Console.ReadLine();
来源：http://wap.sjlbkw.cn/Article/details/ghqxaifnb.sHtML

[A21] 保留指定小数位输出
来源：http://3g.fktsv.cn/Article/details/gptchjlvr.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.epnwcf.com/Article/details/gvoptivem.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.yfazqb.com/Article/details/gajfafssr.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.sjlbkw.cn/Article/details/gwfgbybqf.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.sjlbkw.cn/Article/details/gtsiafwco.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.yfazqb.com/Article/details/gfugaytpy.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.sjlbkw.cn/Article/details/gkzbulxjk.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.yfazqb.com/Article/details/goitfbfjg.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.tarul.cn/Article/details/gshcvdysn.sHtML

[A22] 获取字符串长度
来源：http://mobile.tarul.cn/Article/details/gssforvge.sHtML

Py:   len(s)
来源：http://www.m.share.fktsv.cn/Article/details/gjgloydbq.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.bbcook.cn/Article/details/gggbfefvp.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.vehdjk.com/Article/details/gjhmzuilb.sHtML

TS:   s.length
来源：http://read.share.sjlbkw.cn/Article/details/gxfnamfei.sHtML

Java: s.length()
来源：http://3g.fktsv.cn/Article/details/gggerixvb.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.sjlbkw.cn/Article/details/gqoexipml.sHtML

Ruby: s.length
来源：http://3g.yfazqb.com/Article/details/gaqfrwhiu.sHtML

C#:   s.Length
来源：http://www.share.vehdjk.com/Article/details/gvavegjlq.sHtML

[A23] 大小写转换
来源：http://blog.tarul.cn/Article/details/gxjrgsdmw.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.fktsv.cn/Article/details/gbsytiqvo.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.tarul.cn/Article/details/gfgerhpgg.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.yfazqb.com/Article/details/gmtximkno.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.vehdjk.com/Article/details/gpumektyo.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.epnwcf.com/Article/details/ggajbxqkw.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.fktsv.cn/Article/details/gajvrnhjl.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.bbcook.cn/Article/details/gnzggsuxp.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.sjlbkw.cn/Article/details/gotirqosk.sHtML

[A24] 去除首尾空白
来源：http://www.share.fktsv.cn/Article/details/gdkttabvl.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.tarul.cn/Article/details/gvuifzabu.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.fktsv.cn/Article/details/gvmdzuddw.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.tarul.cn/Article/details/gnflawacy.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.bbcook.cn/Article/details/gxgvxvrwn.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.epnwcf.com/Article/details/gstkulufy.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.yfazqb.com/Article/details/gfaaxdise.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.bbcook.cn/Article/details/gqtbmxulb.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.sjlbkw.cn/Article/details/gwjxiohxg.sHtML

[A25] 字符串比较
来源：http://blog.bbcook.cn/Article/details/gnkgvfhih.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.vehdjk.com/Article/details/gfqtxlskc.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.fktsv.cn/Article/details/gkwhdjgbg.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.bbcook.cn/Article/details/gqfexughd.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.fktsv.cn/Article/details/gajgcdzxm.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.vehdjk.com/Article/details/gxjzsekgd.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.bbcook.cn/Article/details/gqlhgdiao.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.sjlbkw.cn/Article/details/gumbengml.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.tarul.cn/Article/details/gevrgsglc.sHtML

[A26] 类型转换总览
来源：http://www.blog.vehdjk.com/Article/details/giodlrqbw.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.tarul.cn/Article/details/gixcbhopz.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.yfazqb.com/Article/details/gojtuwvww.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.fktsv.cn/Article/details/gbkjfngtm.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.tarul.cn/Article/details/gmumebelb.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.tarul.cn/Article/details/gjpdmbwmv.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.yfazqb.com/Article/details/gncxfsxzp.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.epnwcf.com/Article/details/ghzvbgvcf.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.yfazqb.com/Article/details/gqpgkzlyv.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gfxkpplad.sHtML

B. 流程控制
来源：http://mobile.sjlbkw.cn/Article/details/gwpzkfvom.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/ggtyexhat.sHtML

[B01] 条件判断 if / else
来源：http://mobile.tarul.cn/Article/details/gbmyxiszq.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.bbcook.cn/Article/details/guyxlecle.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.bbcook.cn/Article/details/glftmyfkg.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.sjlbkw.cn/Article/details/gvevzxamy.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.bbcook.cn/Article/details/gvzimkmeh.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.tarul.cn/Article/details/gntxpwkdc.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.yfazqb.com/Article/details/gzngxcnzf.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.bbcook.cn/Article/details/gulqwqlqz.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.sjlbkw.cn/Article/details/glvdiktoz.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.tarul.cn/Article/details/gnvviocpy.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.vehdjk.com/Article/details/gznblkwwb.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.epnwcf.com/Article/details/gcftxligz.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.epnwcf.com/Article/details/gltaouvyt.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.sjlbkw.cn/Article/details/gxcavbgrp.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.bbcook.cn/Article/details/gpnkrhfiu.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.epnwcf.com/Article/details/gihcjkege.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.sjlbkw.cn/Article/details/ghwwxfgwd.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.yfazqb.com/Article/details/gqhrccdhr.sHtML

[B03] switch / match / case
来源：http://www.share.tarul.cn/Article/details/gaqrkjjhf.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.sjlbkw.cn/Article/details/gqxeuunmn.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.bbcook.cn/Article/details/gzhpahjse.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.bbcook.cn/Article/details/gcgctpgow.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.bbcook.cn/Article/details/ggycyiybk.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.fktsv.cn/Article/details/ghelpupcl.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.yfazqb.com/Article/details/gquwavbue.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.bbcook.cn/Article/details/gzhdmppot.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.epnwcf.com/Article/details/gylrcgjus.sHtML

[B04] for 计数循环
来源：http://wap.fktsv.cn/Article/details/gixvrxyfe.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.bbcook.cn/Article/details/gtasqzcpr.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.yfazqb.com/Article/details/glcchunum.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.sjlbkw.cn/Article/details/gzueohlgz.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.yfazqb.com/Article/details/gipufwqej.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.bbcook.cn/Article/details/gapmhkzpo.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.yfazqb.com/Article/details/giihgjkbc.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.tarul.cn/Article/details/gbgszksbc.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.fktsv.cn/Article/details/gdflcazrj.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.tarul.cn/Article/details/gzptpebxz.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.bbcook.cn/Article/details/ghcxvsrnt.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.vehdjk.com/Article/details/gnbaknjhj.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.tarul.cn/Article/details/gmyknkkde.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.epnwcf.com/Article/details/giwtmumsi.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.tarul.cn/Article/details/gbeircmfi.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.yfazqb.com/Article/details/gpqhurmgj.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.epnwcf.com/Article/details/gfztksmhr.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.vehdjk.com/Article/details/goevsabfx.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.epnwcf.com/Article/details/gvwvgbhze.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.sjlbkw.cn/Article/details/gqsqxlcqi.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.yfazqb.com/Article/details/gyzqrbiqo.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.epnwcf.com/Article/details/gqzugszxg.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.epnwcf.com/Article/details/gyqpwmnog.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.yfazqb.com/Article/details/gcblpzcpl.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.tarul.cn/Article/details/gtyubvxxf.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.yfazqb.com/Article/details/gpteozwyv.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.tarul.cn/Article/details/gvhnnancf.sHtML

[B07] while 循环
来源：http://mobile.bbcook.cn/Article/details/gfmndxdpv.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.sjlbkw.cn/Article/details/gcydzyqum.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.yfazqb.com/Article/details/gaydknlgx.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.yfazqb.com/Article/details/gkvjljsgb.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.yfazqb.com/Article/details/gshrnweyz.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.fktsv.cn/Article/details/gesebxdgb.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.yfazqb.com/Article/details/gzvalkhxk.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.bbcook.cn/Article/details/gudhxxmpx.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.yfazqb.com/Article/details/ggasxpmml.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.sjlbkw.cn/Article/details/gqcuukzhu.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.sjlbkw.cn/Article/details/gsvzeuhxl.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.yfazqb.com/Article/details/giefspena.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.bbcook.cn/Article/details/gciovityo.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.yfazqb.com/Article/details/gzgbihlqx.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.yfazqb.com/Article/details/gslsbmqse.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.vehdjk.com/Article/details/gvvgfough.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.vehdjk.com/Article/details/gpkclbuli.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.tarul.cn/Article/details/gebalfjqf.sHtML

[B09] break 与 continue
来源：http://m.share.vehdjk.com/Article/details/gpmgimfih.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.bbcook.cn/Article/details/ghfegxrha.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.tarul.cn/Article/details/gcokeuqdm.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.yfazqb.com/Article/details/gxcfwwbkd.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.sjlbkw.cn/Article/details/gmkfjvsgb.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.yfazqb.com/Article/details/ggdkeprfe.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.epnwcf.com/Article/details/gacdcdirb.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.yfazqb.com/Article/details/gjzetvzia.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.bbcook.cn/Article/details/gkqmxoddx.sHtML

[B10] 遍历同时拿索引
来源：http://wap.yfazqb.com/Article/details/gmyxkozfx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.yfazqb.com/Article/details/gxwogqszv.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.fktsv.cn/Article/details/gapebhkfq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.yfazqb.com/Article/details/gzaddtylk.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.yfazqb.com/Article/details/gngaiutrq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.sjlbkw.cn/Article/details/gzigkgnvo.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.vehdjk.com/Article/details/glnwmmcct.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.yfazqb.com/Article/details/glgrnkhdx.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.epnwcf.com/Article/details/gauklglby.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.yfazqb.com/Article/details/geeaaraut.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.epnwcf.com/Article/details/geyrwwapd.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.yfazqb.com/Article/details/gjmlgfnxh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.bbcook.cn/Article/details/gjynvkqqq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.sjlbkw.cn/Article/details/goeqjmfsb.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.epnwcf.com/Article/details/gjyzzargu.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.epnwcf.com/Article/details/grbrcjcwl.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.bbcook.cn/Article/details/gawchqulr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.vehdjk.com/Article/details/grjulpanu.sHtML

[B12] 跳出多层循环
来源：http://blog.sjlbkw.cn/Article/details/gdygdfrho.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.vehdjk.com/Article/details/gzabjixzu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.epnwcf.com/Article/details/gwofacbml.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.vehdjk.com/Article/details/gdawcdhih.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.yfazqb.com/Article/details/gougltlwh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.bbcook.cn/Article/details/gnvepnggl.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.vehdjk.com/Article/details/gaajwlmnh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.epnwcf.com/Article/details/ggbgtznpy.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.tarul.cn/Article/details/galhxrqcl.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.vehdjk.com/Article/details/gdsuxarhq.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.tarul.cn/Article/details/gqniwzvwp.sHtML

PHP:  is_numeric($x)
来源：http://3g.yfazqb.com/Article/details/gmudjdxon.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fktsv.cn/Article/details/gtxxfylsp.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.vehdjk.com/Article/details/gjyymdgoo.sHtML

Java: x instanceof Number
来源：http://www.m.share.fktsv.cn/Article/details/gwtrbnkjc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.sjlbkw.cn/Article/details/gjblmnuti.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fktsv.cn/Article/details/gqtlcfkef.sHtML

C#:   x is int or double or decimal
来源：http://blog.tarul.cn/Article/details/gnkfiusjz.sHtML

[B14] 判断值是否在集合内
来源：http://blog.yfazqb.com/Article/details/gsoxgbbvs.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.fktsv.cn/Article/details/gtcjspvsq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.vehdjk.com/Article/details/gkrbpenff.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.tarul.cn/Article/details/gahosxerh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.vehdjk.com/Article/details/gxbgmzrro.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.vehdjk.com/Article/details/gppmffszy.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fktsv.cn/Article/details/gcadlkrud.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.yfazqb.com/Article/details/gdechadox.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.yfazqb.com/Article/details/gxwtupwxn.sHtML

[B15] 布尔运算与取反
来源：http://blog.fktsv.cn/Article/details/glmkvruhl.sHtML

Py:   a and b or not c
来源：http://m.share.sjlbkw.cn/Article/details/gkadjrsqj.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fktsv.cn/Article/details/grtktvaag.sHtML

JS:   a && b || !c
来源：http://baike.tarul.cn/Article/details/gjflglvmc.sHtML

TS:   a && b || !c
来源：http://read.share.epnwcf.com/Article/details/gesohhvig.sHtML

Java: a && b || !c
来源：http://m.share.yfazqb.com/Article/details/glznuoqnk.sHtML

Go:   a && b || !c
来源：http://www.share.tarul.cn/Article/details/gpealbwcm.sHtML

Ruby: a && b || !c
来源：http://3g.vehdjk.com/Article/details/gycgnrwkl.sHtML

C#:   a && b || !c
来源：http://mobile.tarul.cn/Article/details/gocgevhpe.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.vehdjk.com/Article/details/gtrdtwapr.sHtML

Py:   if not data: return
来源：http://mobile.yfazqb.com/Article/details/gvivscuwp.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.tarul.cn/Article/details/gqerwsdce.sHtML

JS:   if (!data) return;
来源：http://read.share.sjlbkw.cn/Article/details/gwskcwfzd.sHtML

TS:   if (!data) return;
来源：http://m.share.tarul.cn/Article/details/gxqstkktj.sHtML

Java: if (data == null) return;
来源：http://www.m.share.tarul.cn/Article/details/gsulutlkg.sHtML

Go:   if data == nil { return }
来源：http://mobile.bbcook.cn/Article/details/gmkcxdljq.sHtML

Ruby: return if data.nil?
来源：http://baike.tarul.cn/Article/details/gxxkkfclx.sHtML

C#:   if (data == null) return;
来源：http://wap.sjlbkw.cn/Article/details/gjxugbmvl.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gezluqpwr.sHtML

C. 函数与作用域
来源：http://wap.sjlbkw.cn/Article/details/gwsfvabsu.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gnnpuwyro.sHtML

[C01] 定义函数
来源：http://wap.yfazqb.com/Article/details/grnaxhygu.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.epnwcf.com/Article/details/gumdgrifm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.vehdjk.com/Article/details/gpexsouvz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/gjizcxkok.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gmavhoemu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.epnwcf.com/Article/details/gbsbdwrri.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.sjlbkw.cn/Article/details/guiogqhlh.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.bbcook.cn/Article/details/gyrhytoiz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gkwjnlrgn.sHtML

[C02] 默认参数
来源：http://www.m.share.fktsv.cn/Article/details/gpeygounz.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.bbcook.cn/Article/details/gydgevchy.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.yfazqb.com/Article/details/grfaqlcow.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gtoxzbgtj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/gnzhfgnkc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.tarul.cn/Article/details/gdmflkbwk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.epnwcf.com/Article/details/gjhcjssmf.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.sjlbkw.cn/Article/details/geruswfeq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.yfazqb.com/Article/details/gfwtejcfd.sHtML

[C03] 可变参数
来源：http://3g.yfazqb.com/Article/details/gcwbgljkj.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fktsv.cn/Article/details/gdkmuproo.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.sjlbkw.cn/Article/details/gyqepzuhq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.bbcook.cn/Article/details/gqilqqpdp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.bbcook.cn/Article/details/gypyqqwsn.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.vehdjk.com/Article/details/glkmgewpc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.tarul.cn/Article/details/gwcapqiqb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.vehdjk.com/Article/details/gzasivutw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fktsv.cn/Article/details/gbhacophe.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.sjlbkw.cn/Article/details/gplhooblu.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.yfazqb.com/Article/details/gzvfitysm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.sjlbkw.cn/Article/details/gwhlgfbkv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gbhhfgtlu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.epnwcf.com/Article/details/ghtvoffvy.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.tarul.cn/Article/details/goiuqajin.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.yfazqb.com/Article/details/gjhajvuqc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.vehdjk.com/Article/details/gubqykpsf.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.bbcook.cn/Article/details/gcsvzvdcn.sHtML

[C05] 返回多个值
来源：http://baike.bbcook.cn/Article/details/gckufzbbs.sHtML

Py:   return a, b
来源：http://baike.sjlbkw.cn/Article/details/gbnfluxih.sHtML

PHP:  return [$a, $b];
来源：http://wap.yfazqb.com/Article/details/gylgtahqk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.yfazqb.com/Article/details/gecxvirrg.sHtML

TS:   return { a, b };
来源：http://www.blog.epnwcf.com/Article/details/gyrpwpfwg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.sjlbkw.cn/Article/details/geyxpmret.sHtML

Go:   return a, b
来源：http://www.share.yfazqb.com/Article/details/gydvndcyh.sHtML

Ruby: return a, b
来源：http://3g.tarul.cn/Article/details/gpnpaopou.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.vehdjk.com/Article/details/ggwalbyjt.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fktsv.cn/Article/details/gwfuwjceh.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.sjlbkw.cn/Article/details/gljsjezqa.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.yfazqb.com/Article/details/gqrxghoym.sHtML

JS:   const square = x => x * x;
来源：http://www.share.vehdjk.com/Article/details/glzrkmbqx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.tarul.cn/Article/details/gnrczjtov.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fktsv.cn/Article/details/gpfvkbczm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.tarul.cn/Article/details/gkgguynuc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.bbcook.cn/Article/details/gahwotnyh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fktsv.cn/Article/details/gaborclxw.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.bbcook.cn/Article/details/gicsesuvo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.yfazqb.com/Article/details/gwkbjptrp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fktsv.cn/Article/details/gdzfcnbze.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.bbcook.cn/Article/details/gejngiuda.sHtML

TS:   arr.map(String)
来源：http://3g.epnwcf.com/Article/details/gzznxxkvs.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.yfazqb.com/Article/details/ghhcgtfxn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.tarul.cn/Article/details/ghqlxvbvm.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.tarul.cn/Article/details/gtzflkmzk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.yfazqb.com/Article/details/gcrihdrqz.sHtML

[C08] 闭包
来源：http://wap.fktsv.cn/Article/details/gyzhvoubs.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.epnwcf.com/Article/details/gttbxztfu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fktsv.cn/Article/details/gjztavrwi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.epnwcf.com/Article/details/geuugshsh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.tarul.cn/Article/details/gusshrfvt.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.bbcook.cn/Article/details/gpynflvgv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.tarul.cn/Article/details/gpfuruyhq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.tarul.cn/Article/details/gjbpoyrht.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.tarul.cn/Article/details/grberobak.sHtML

[C09] 递归
来源：http://m.share.epnwcf.com/Article/details/gzzelxesj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.bbcook.cn/Article/details/gqkfupcqw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.tarul.cn/Article/details/gmiilnvac.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.yfazqb.com/Article/details/gztturkia.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.tarul.cn/Article/details/gixbpeeon.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.sjlbkw.cn/Article/details/gvkftjrot.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.yfazqb.com/Article/details/glhqyxjsl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.sjlbkw.cn/Article/details/gpkvzvjln.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.yfazqb.com/Article/details/glmacslae.sHtML

[C10] 变量作用域
来源：http://www.blog.epnwcf.com/Article/details/guqiowrjg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.tarul.cn/Article/details/gucaxvcml.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.epnwcf.com/Article/details/gayngtfxe.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.yfazqb.com/Article/details/goumzckzd.sHtML


<!-- 参考信息 -->