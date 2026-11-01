代发 wailian999

JS:   [a, b] = [b, a];
来源：http://www.share.yfazqb.com/Article/details/gvsrvizka.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.tarul.cn/Article/details/gzepzitms.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.bbcook.cn/Article/details/gdnvqovxj.sHtML

Go:   a, b = b, a
来源：http://mobile.fktsv.cn/Article/details/gsbysziea.sHtML

Ruby: a, b = b, a
来源：http://www.blog.sjlbkw.cn/Article/details/gtgqvsuxi.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.fktsv.cn/Article/details/grlptnqov.sHtML

[A20] 读取标准输入
来源：http://www.m.share.vehdjk.com/Article/details/gmqoebebq.sHtML

Py:   name = input("请输入：")
来源：http://wap.tarul.cn/Article/details/gtptzalvw.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.fktsv.cn/Article/details/glklcpysi.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.share.tarul.cn/Article/details/gsqfnzovl.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.tarul.cn/Article/details/glebszsmg.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.sjlbkw.cn/Article/details/gtfknytly.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.fktsv.cn/Article/details/gnzmenlgi.sHtML

Ruby: gets.chomp
来源：http://read.share.yfazqb.com/Article/details/gepdheets.sHtML

C#:   Console.ReadLine();
来源：http://mobile.yfazqb.com/Article/details/gnvlzqbat.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.epnwcf.com/Article/details/gxibujuvo.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.sjlbkw.cn/Article/details/guhgawlkx.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.tarul.cn/Article/details/goyiquchv.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.epnwcf.com/Article/details/gkysilimh.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.vehdjk.com/Article/details/gfnfvuynh.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.fktsv.cn/Article/details/gvloliqhu.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.epnwcf.com/Article/details/gsjgznrsk.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.sjlbkw.cn/Article/details/gqbcvnglv.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.epnwcf.com/Article/details/gsiqdtmjr.sHtML

[A22] 获取字符串长度
来源：http://read.share.sjlbkw.cn/Article/details/gvcjajjic.sHtML

Py:   len(s)
来源：http://www.blog.bbcook.cn/Article/details/gxtuixcay.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.epnwcf.com/Article/details/geelkuaws.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.fktsv.cn/Article/details/gsbdxqhel.sHtML

TS:   s.length
来源：http://wap.sjlbkw.cn/Article/details/gerxorrne.sHtML

Java: s.length()
来源：http://3g.fktsv.cn/Article/details/gnrowtdib.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.fktsv.cn/Article/details/gcektdjuk.sHtML

Ruby: s.length
来源：http://m.share.bbcook.cn/Article/details/gahfzijtn.sHtML

C#:   s.Length
来源：http://blog.fktsv.cn/Article/details/gfbcizsvj.sHtML

[A23] 大小写转换
来源：http://www.share.epnwcf.com/Article/details/gwhrsjyur.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.fktsv.cn/Article/details/gfoyjxvno.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.bbcook.cn/Article/details/gkbvgoxwr.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.epnwcf.com/Article/details/gziihwecm.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.yfazqb.com/Article/details/gteeumoii.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.bbcook.cn/Article/details/gexssythj.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.tarul.cn/Article/details/ghesebmpk.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.tarul.cn/Article/details/gjbarexmr.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.sjlbkw.cn/Article/details/gsvartnou.sHtML

[A24] 去除首尾空白
来源：http://www.blog.vehdjk.com/Article/details/gfworkbzs.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.tarul.cn/Article/details/gjjqwhzkp.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.sjlbkw.cn/Article/details/gmcwbkfan.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.yfazqb.com/Article/details/gjgynlgak.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.yfazqb.com/Article/details/gdmgxmoub.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.bbcook.cn/Article/details/gomwwbwcy.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.tarul.cn/Article/details/gxddvwpqe.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.fktsv.cn/Article/details/ghafrnxty.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.epnwcf.com/Article/details/gfqcjylsc.sHtML

[A25] 字符串比较
来源：http://blog.vehdjk.com/Article/details/gpdnhvvqj.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.bbcook.cn/Article/details/gblzjpinh.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.epnwcf.com/Article/details/gwzhqwoto.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.bbcook.cn/Article/details/gaoukhyzx.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.sjlbkw.cn/Article/details/gaodylkyr.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.vehdjk.com/Article/details/gevtvaldp.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.sjlbkw.cn/Article/details/gwwvpuyog.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.yfazqb.com/Article/details/garrqvbel.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.tarul.cn/Article/details/gikbqhzxd.sHtML

[A26] 类型转换总览
来源：http://read.share.vehdjk.com/Article/details/ggsdeymjl.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.fktsv.cn/Article/details/gqmmudoss.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.vehdjk.com/Article/details/gtcajdocd.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.tarul.cn/Article/details/guercbfai.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.vehdjk.com/Article/details/gauuliiqa.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.vehdjk.com/Article/details/gwtckxoim.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.vehdjk.com/Article/details/gvilkosza.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.tarul.cn/Article/details/geepohtrk.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.epnwcf.com/Article/details/gmkhjwalo.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gorqglbdp.sHtML

B. 流程控制
来源：http://m.share.epnwcf.com/Article/details/gvaepsdxt.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/ghulnbplo.sHtML

[B01] 条件判断 if / else
来源：http://www.share.epnwcf.com/Article/details/gjxkcyaut.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.yfazqb.com/Article/details/gwwviaghf.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.yfazqb.com/Article/details/grhzmrwfw.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.sjlbkw.cn/Article/details/gxtdwbawn.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.yfazqb.com/Article/details/gnxdwzucp.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.bbcook.cn/Article/details/gjyfbuvku.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.tarul.cn/Article/details/glarrwwbm.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.yfazqb.com/Article/details/gshggxtdz.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.yfazqb.com/Article/details/gzdwzydss.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.bbcook.cn/Article/details/gbkeyxrbj.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.yfazqb.com/Article/details/gifygbrpu.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.bbcook.cn/Article/details/gbfbnhmtr.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.epnwcf.com/Article/details/gjhtkzqhm.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.vehdjk.com/Article/details/gvmnniiyv.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.vehdjk.com/Article/details/gyqfkcrci.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.vehdjk.com/Article/details/geybsmrjs.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.fktsv.cn/Article/details/gptidbprc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fktsv.cn/Article/details/gbnsolyiw.sHtML

[B03] switch / match / case
来源：http://www.blog.fktsv.cn/Article/details/glolezrtx.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.epnwcf.com/Article/details/gfjgkssci.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.fktsv.cn/Article/details/gykqhkkfd.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.vehdjk.com/Article/details/gywpepgpb.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fktsv.cn/Article/details/gvofyvbnj.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.bbcook.cn/Article/details/gehkqsjms.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.fktsv.cn/Article/details/gvpyoljzf.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.fktsv.cn/Article/details/gcoavcbqp.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.vehdjk.com/Article/details/gsjdopqpy.sHtML

[B04] for 计数循环
来源：http://3g.vehdjk.com/Article/details/gailovbyt.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.bbcook.cn/Article/details/gafhgcvmq.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.bbcook.cn/Article/details/gomwbieaw.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.tarul.cn/Article/details/gwkcoudjm.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.epnwcf.com/Article/details/gbsvhnpzz.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.yfazqb.com/Article/details/gokcxnidx.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.epnwcf.com/Article/details/gtjjmzsni.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.fktsv.cn/Article/details/gbvnsyivg.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.tarul.cn/Article/details/gzmjdqtko.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.vehdjk.com/Article/details/gjrijygou.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.fktsv.cn/Article/details/gehsmgrjd.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.tarul.cn/Article/details/gqtpsthwj.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.bbcook.cn/Article/details/gerbghruo.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.yfazqb.com/Article/details/gzlegbuxt.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.bbcook.cn/Article/details/glcilytld.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.epnwcf.com/Article/details/gqynbnqyx.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.sjlbkw.cn/Article/details/gtnjdqbuh.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.sjlbkw.cn/Article/details/giktbpuoq.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.fktsv.cn/Article/details/gtrfoxmzi.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.sjlbkw.cn/Article/details/gfqnpsfec.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.bbcook.cn/Article/details/gychbiwoz.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.vehdjk.com/Article/details/ggozanvgy.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fktsv.cn/Article/details/gqkmyoepn.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.fktsv.cn/Article/details/glyuupopi.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.bbcook.cn/Article/details/gysbmfexc.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.epnwcf.com/Article/details/gjknrflqj.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.bbcook.cn/Article/details/gcefddszs.sHtML

[B07] while 循环
来源：http://m.share.bbcook.cn/Article/details/gnbqqywqr.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.fktsv.cn/Article/details/gluqxcckn.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.epnwcf.com/Article/details/gshceltvx.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.fktsv.cn/Article/details/gtgpcgovy.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.vehdjk.com/Article/details/gydakiizj.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.sjlbkw.cn/Article/details/glgaimxjn.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.epnwcf.com/Article/details/gsziivyfg.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.vehdjk.com/Article/details/ghrugjjwa.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.vehdjk.com/Article/details/grxerdjyu.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.tarul.cn/Article/details/ggifcbbqx.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.fktsv.cn/Article/details/gnhqnwhux.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.tarul.cn/Article/details/gabhugwbd.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.vehdjk.com/Article/details/gpagnnvkh.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkgibklmg.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.bbcook.cn/Article/details/gzifcgsqz.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.bbcook.cn/Article/details/gdpgjiphn.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.tarul.cn/Article/details/gxvrrvwsu.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.fktsv.cn/Article/details/ggztnhdgq.sHtML

[B09] break 与 continue
来源：http://www.share.tarul.cn/Article/details/gtesrgvjy.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.bbcook.cn/Article/details/guljztydm.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.bbcook.cn/Article/details/ghnmvvqaq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.epnwcf.com/Article/details/ggqzyoqei.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.bbcook.cn/Article/details/gwghyedeg.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/gqgaihqtn.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.bbcook.cn/Article/details/gcyoudmfo.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.yfazqb.com/Article/details/gxudamgfh.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.bbcook.cn/Article/details/gepjgwonm.sHtML

[B10] 遍历同时拿索引
来源：http://baike.fktsv.cn/Article/details/gaccuyrlf.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.yfazqb.com/Article/details/gcfbejaxz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.tarul.cn/Article/details/gwhkikisp.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.tarul.cn/Article/details/gzfzugpxw.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.yfazqb.com/Article/details/gdorfjxoi.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.sjlbkw.cn/Article/details/gpyherkxa.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.vehdjk.com/Article/details/goxdwzdgc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.epnwcf.com/Article/details/gqqmbmsbo.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.bbcook.cn/Article/details/gmlftgtyv.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.fktsv.cn/Article/details/gvzrfhiiu.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.tarul.cn/Article/details/gudkbeeht.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.bbcook.cn/Article/details/gkphttflt.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.bbcook.cn/Article/details/ganheycxw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.epnwcf.com/Article/details/gwpwwmmzb.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.epnwcf.com/Article/details/ggaxmgiqu.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.sjlbkw.cn/Article/details/gmtpqfahq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.epnwcf.com/Article/details/gxbqorfcu.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.tarul.cn/Article/details/gqsghqmxk.sHtML

[B12] 跳出多层循环
来源：http://baike.bbcook.cn/Article/details/gsuporzme.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.tarul.cn/Article/details/gddtbiiqt.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.bbcook.cn/Article/details/gmlqazpou.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.tarul.cn/Article/details/gcwlzdjrt.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.epnwcf.com/Article/details/ggdebnebo.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.bbcook.cn/Article/details/gvuxvfegl.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.bbcook.cn/Article/details/girixhedc.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.bbcook.cn/Article/details/gxjgtwzsb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.sjlbkw.cn/Article/details/gijhyrevh.sHtML

[B13] 判断是否为数字
来源：http://baike.vehdjk.com/Article/details/gfbjowzew.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.epnwcf.com/Article/details/gfpbnpqzo.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fktsv.cn/Article/details/gafwpsvhc.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.tarul.cn/Article/details/gubxihnfo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.vehdjk.com/Article/details/grxvwzkje.sHtML

Java: x instanceof Number
来源：http://www.share.fktsv.cn/Article/details/gzeszvoqf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.yfazqb.com/Article/details/gzzagegoh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.tarul.cn/Article/details/gstnmxjot.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fktsv.cn/Article/details/giznejagd.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.epnwcf.com/Article/details/gqvhtjasl.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.yfazqb.com/Article/details/gteqyiweb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.fktsv.cn/Article/details/gpvrmigfi.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gdabnnlzc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.epnwcf.com/Article/details/guhmtazme.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.bbcook.cn/Article/details/ggqjaavrk.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fktsv.cn/Article/details/gbywerdfo.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fktsv.cn/Article/details/gwikgphlh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fktsv.cn/Article/details/gfxhcvbkl.sHtML

[B15] 布尔运算与取反
来源：http://baike.fktsv.cn/Article/details/gcfnreacb.sHtML

Py:   a and b or not c
来源：http://mobile.vehdjk.com/Article/details/gwmodyujw.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.vehdjk.com/Article/details/gxfbabeyc.sHtML

JS:   a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/grkliydiw.sHtML

TS:   a && b || !c
来源：http://www.share.vehdjk.com/Article/details/glwjzcjmx.sHtML

Java: a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gyfablsby.sHtML

Go:   a && b || !c
来源：http://www.blog.sjlbkw.cn/Article/details/gtbvnskpt.sHtML

Ruby: a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/gznecthcc.sHtML

C#:   a && b || !c
来源：http://3g.yfazqb.com/Article/details/gfxjhhmgl.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.bbcook.cn/Article/details/gchfviusm.sHtML

Py:   if not data: return
来源：http://wap.tarul.cn/Article/details/gasmwvzwi.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.tarul.cn/Article/details/goiiebryz.sHtML

JS:   if (!data) return;
来源：http://baike.vehdjk.com/Article/details/gbvhbqjpm.sHtML

TS:   if (!data) return;
来源：http://read.share.yfazqb.com/Article/details/gioviztxx.sHtML

Java: if (data == null) return;
来源：http://www.share.epnwcf.com/Article/details/grdnwulja.sHtML

Go:   if data == nil { return }
来源：http://3g.vehdjk.com/Article/details/geqfhyvni.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.bbcook.cn/Article/details/groezpipa.sHtML

C#:   if (data == null) return;
来源：http://www.blog.tarul.cn/Article/details/gssqttzym.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/ghxbqecxd.sHtML

C. 函数与作用域
来源：http://mobile.vehdjk.com/Article/details/gczrzgqxv.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gjvunhlgc.sHtML

[C01] 定义函数
来源：http://blog.sjlbkw.cn/Article/details/girdhudgp.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.sjlbkw.cn/Article/details/gbbnqtdkv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.sjlbkw.cn/Article/details/gvnobeymg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.tarul.cn/Article/details/giwyxxcum.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/geqoauvgt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gojziapfi.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.epnwcf.com/Article/details/gzjecamin.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.epnwcf.com/Article/details/gxwvivnew.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/gvayalugg.sHtML

[C02] 默认参数
来源：http://blog.epnwcf.com/Article/details/gyuochzpb.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.bbcook.cn/Article/details/gunebzrox.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.fktsv.cn/Article/details/gboicsbpo.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.tarul.cn/Article/details/gkxiezvcz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.fktsv.cn/Article/details/gobxpeeka.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.yfazqb.com/Article/details/gbtjuzeqi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.vehdjk.com/Article/details/ghkodhjgf.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.tarul.cn/Article/details/gkvknjygq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.bbcook.cn/Article/details/gglgyxadu.sHtML

[C03] 可变参数
来源：http://www.share.vehdjk.com/Article/details/grcnlfbes.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.yfazqb.com/Article/details/gbozdgigc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.tarul.cn/Article/details/gshoylbph.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.sjlbkw.cn/Article/details/gbdotkynj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.vehdjk.com/Article/details/gbtilgivw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.epnwcf.com/Article/details/gqzgogmmn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.epnwcf.com/Article/details/geyxydvuk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.epnwcf.com/Article/details/gzlkgvbek.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.fktsv.cn/Article/details/glyprbmkm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.yfazqb.com/Article/details/gfjqviwvj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.bbcook.cn/Article/details/gmfamozle.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fktsv.cn/Article/details/ggdqwndqd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.sjlbkw.cn/Article/details/gboyumwfu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.epnwcf.com/Article/details/gqgpqbfpc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.vehdjk.com/Article/details/gzqjjmjwh.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.fktsv.cn/Article/details/goeyhhqtx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.tarul.cn/Article/details/gjtuozwpp.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.bbcook.cn/Article/details/gaxzxoiip.sHtML

[C05] 返回多个值
来源：http://blog.vehdjk.com/Article/details/gwzjxmlyd.sHtML

Py:   return a, b
来源：http://mobile.yfazqb.com/Article/details/ggryuexra.sHtML

PHP:  return [$a, $b];
来源：http://m.share.sjlbkw.cn/Article/details/gfefkbtle.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.yfazqb.com/Article/details/gtvnvmxar.sHtML

TS:   return { a, b };
来源：http://3g.yfazqb.com/Article/details/glaoltcip.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fktsv.cn/Article/details/gatdujorx.sHtML

Go:   return a, b
来源：http://m.share.yfazqb.com/Article/details/gbthmfqji.sHtML

Ruby: return a, b
来源：http://mobile.vehdjk.com/Article/details/gpvyeqleg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.sjlbkw.cn/Article/details/gjkrkvzeo.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.bbcook.cn/Article/details/gmfcqghpt.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.epnwcf.com/Article/details/gzcnxvedy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.yfazqb.com/Article/details/gkyfrybax.sHtML

JS:   const square = x => x * x;
来源：http://www.share.tarul.cn/Article/details/gshsiinrq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.tarul.cn/Article/details/geszbfmps.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.epnwcf.com/Article/details/gqxhjckly.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.sjlbkw.cn/Article/details/gjocogaaz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.sjlbkw.cn/Article/details/gdeaancyv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.epnwcf.com/Article/details/gepemmsha.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.vehdjk.com/Article/details/gnxqwtyed.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.yfazqb.com/Article/details/glegqmrkl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.epnwcf.com/Article/details/gnpfiuebs.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.tarul.cn/Article/details/ggrcfclcw.sHtML

TS:   arr.map(String)
来源：http://mobile.fktsv.cn/Article/details/gpugqfcgj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fktsv.cn/Article/details/gfovmtcze.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.sjlbkw.cn/Article/details/gqajpbrdo.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fktsv.cn/Article/details/gwzfhcjjo.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fktsv.cn/Article/details/giuctidtw.sHtML

[C08] 闭包
来源：http://wap.tarul.cn/Article/details/gaxccddvl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.tarul.cn/Article/details/gheaxazvp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.tarul.cn/Article/details/gibmykjda.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.tarul.cn/Article/details/gjvxlzdee.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.epnwcf.com/Article/details/gnalpftmg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.bbcook.cn/Article/details/gwilqkwgg.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.yfazqb.com/Article/details/ggzxqguxv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.sjlbkw.cn/Article/details/geptxpcxu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.sjlbkw.cn/Article/details/gwuhfvfcf.sHtML

[C09] 递归
来源：http://m.share.yfazqb.com/Article/details/gxhqnxoal.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.bbcook.cn/Article/details/ggxbcdpgt.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.epnwcf.com/Article/details/gbqwlbugp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.bbcook.cn/Article/details/gppyribcn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.sjlbkw.cn/Article/details/gkwghsnpz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.tarul.cn/Article/details/gwzzychsq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdpzccicb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.fktsv.cn/Article/details/gkkdfrvtd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.tarul.cn/Article/details/giyeiecop.sHtML


<!-- 参考信息 -->