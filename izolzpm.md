代发 wailian999

C#:   (int)'A'; (char)65
来源：http://www.share.bbcook.cn/Article/details/gkptmzczw.sHtML

[A19] 交换两个变量
来源：http://wap.sjlbkw.cn/Article/details/gznuughbs.sHtML

Py:   a, b = b, a
来源：http://m.share.bbcook.cn/Article/details/gkfvhgfov.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.sjlbkw.cn/Article/details/giyxohqmd.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.yfazqb.com/Article/details/gephtmuqr.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.yfazqb.com/Article/details/gnjgfpwtf.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.epnwcf.com/Article/details/glcfyekmt.sHtML

Go:   a, b = b, a
来源：http://www.m.share.sjlbkw.cn/Article/details/guodwxujp.sHtML

Ruby: a, b = b, a
来源：http://www.blog.sjlbkw.cn/Article/details/ggbkrdmlj.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.tarul.cn/Article/details/gjgbeqlgw.sHtML

[A20] 读取标准输入
来源：http://baike.tarul.cn/Article/details/gylsrdenl.sHtML

Py:   name = input("请输入：")
来源：http://blog.bbcook.cn/Article/details/gybdelder.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.bbcook.cn/Article/details/gmjudewwm.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.tarul.cn/Article/details/gjhopzuyy.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.vehdjk.com/Article/details/gifyvffmw.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.epnwcf.com/Article/details/gexacgccz.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.tarul.cn/Article/details/gwpqeftmx.sHtML

Ruby: gets.chomp
来源：http://www.share.yfazqb.com/Article/details/gnwnppljx.sHtML

C#:   Console.ReadLine();
来源：http://3g.vehdjk.com/Article/details/gerdnjyyq.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.tarul.cn/Article/details/gulamrspv.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.bbcook.cn/Article/details/gtoodryrh.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggqihjkkp.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.sjlbkw.cn/Article/details/gxjtrhwtw.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.fktsv.cn/Article/details/gsckkpqsr.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.sjlbkw.cn/Article/details/gfevlpydw.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.yfazqb.com/Article/details/gqaymuptw.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.sjlbkw.cn/Article/details/gufbghprt.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.epnwcf.com/Article/details/givqiawev.sHtML

[A22] 获取字符串长度
来源：http://3g.sjlbkw.cn/Article/details/gnzleielo.sHtML

Py:   len(s)
来源：http://blog.sjlbkw.cn/Article/details/gbwdrpejw.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.tarul.cn/Article/details/grlapqnfe.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.tarul.cn/Article/details/gytpfmwsq.sHtML

TS:   s.length
来源：http://blog.fktsv.cn/Article/details/gtpgoazjw.sHtML

Java: s.length()
来源：http://blog.fktsv.cn/Article/details/gbqsolspg.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.sjlbkw.cn/Article/details/ggopjdiyo.sHtML

Ruby: s.length
来源：http://www.blog.fktsv.cn/Article/details/ghnurynio.sHtML

C#:   s.Length
来源：http://blog.epnwcf.com/Article/details/giumgvxmr.sHtML

[A23] 大小写转换
来源：http://read.share.sjlbkw.cn/Article/details/ghucogcvj.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.fktsv.cn/Article/details/gnnfmcdcn.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.sjlbkw.cn/Article/details/gqyhbtnqh.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.tarul.cn/Article/details/gnrjzqytp.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.yfazqb.com/Article/details/ggmhfhzkl.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.vehdjk.com/Article/details/guwlwreaz.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.tarul.cn/Article/details/govhxhwqv.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.tarul.cn/Article/details/gwtvvelcd.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.fktsv.cn/Article/details/gjolvmfeu.sHtML

[A24] 去除首尾空白
来源：http://read.share.bbcook.cn/Article/details/ghuwonwpv.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.tarul.cn/Article/details/grobfetgi.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.fktsv.cn/Article/details/gcxlvisgz.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.epnwcf.com/Article/details/gkiyqyzyx.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.yfazqb.com/Article/details/gygsmkkvd.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.yfazqb.com/Article/details/gwpmstuhg.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.bbcook.cn/Article/details/gnzryxomq.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.yfazqb.com/Article/details/gzzeslpgl.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.fktsv.cn/Article/details/glxtvcsuv.sHtML

[A25] 字符串比较
来源：http://3g.sjlbkw.cn/Article/details/gwqmoumlo.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.tarul.cn/Article/details/glntereao.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.sjlbkw.cn/Article/details/gwkursrlh.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.bbcook.cn/Article/details/gkmvsecgn.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.vehdjk.com/Article/details/gyysnmjav.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.fktsv.cn/Article/details/gdaqzaacz.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.tarul.cn/Article/details/gygaeksvc.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.tarul.cn/Article/details/gxluvcxuf.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.vehdjk.com/Article/details/gpzquqjyp.sHtML

[A26] 类型转换总览
来源：http://wap.fktsv.cn/Article/details/gissiqued.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.sjlbkw.cn/Article/details/glexntcov.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.vehdjk.com/Article/details/gmwidchrw.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.fktsv.cn/Article/details/gtbqdqqvd.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.yfazqb.com/Article/details/ggxqaierx.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.vehdjk.com/Article/details/galbmnxus.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.sjlbkw.cn/Article/details/gegghwvty.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.sjlbkw.cn/Article/details/gkdqydwhn.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.tarul.cn/Article/details/guzkxfwon.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gocaansna.sHtML

B. 流程控制
来源：http://3g.tarul.cn/Article/details/gsowzhteb.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gftyizcnp.sHtML

[B01] 条件判断 if / else
来源：http://read.share.sjlbkw.cn/Article/details/gjzcuxurc.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.yfazqb.com/Article/details/gdrxtljck.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.tarul.cn/Article/details/gsbxevqxy.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.tarul.cn/Article/details/gyrfbjjas.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.epnwcf.com/Article/details/gxuookwbk.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.epnwcf.com/Article/details/ghsiifjmx.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.yfazqb.com/Article/details/grsfaycpv.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.yfazqb.com/Article/details/gltvuwthl.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.fktsv.cn/Article/details/gphvkxiqx.sHtML

[B02] 多分支 else if / elif
来源：http://blog.sjlbkw.cn/Article/details/gupgwrnfo.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.bbcook.cn/Article/details/gvctbjmzv.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.yfazqb.com/Article/details/gqjoulhag.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.sjlbkw.cn/Article/details/gjstzzsoo.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.tarul.cn/Article/details/gyxvhojfh.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fktsv.cn/Article/details/gewewayry.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.fktsv.cn/Article/details/gbbwxzmmn.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.epnwcf.com/Article/details/gywrcssnr.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.vehdjk.com/Article/details/gjkklsgce.sHtML

[B03] switch / match / case
来源：http://read.share.bbcook.cn/Article/details/gtkkoknts.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.bbcook.cn/Article/details/gpmaadxqw.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.sjlbkw.cn/Article/details/gnnlppbma.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.yfazqb.com/Article/details/ghwutqdbv.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fktsv.cn/Article/details/gryocsaji.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.yfazqb.com/Article/details/gsxyhfiua.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.yfazqb.com/Article/details/gydksmtzm.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.vehdjk.com/Article/details/geuapqcbx.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.fktsv.cn/Article/details/gbqghnyqe.sHtML

[B04] for 计数循环
来源：http://3g.tarul.cn/Article/details/gnsttqfgf.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.sjlbkw.cn/Article/details/ggrvazwag.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.vehdjk.com/Article/details/gqxnypwzm.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.tarul.cn/Article/details/gqiebveoc.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fktsv.cn/Article/details/gqqhhjzet.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.sjlbkw.cn/Article/details/gqrwxpbqi.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.bbcook.cn/Article/details/gvcpiqxea.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.fktsv.cn/Article/details/gapabxnef.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.vehdjk.com/Article/details/gobaevhxv.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.bbcook.cn/Article/details/gbnlxgbyl.sHtML

Py:   for item in arr: print(item)
来源：http://blog.bbcook.cn/Article/details/gttwotxlt.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.fktsv.cn/Article/details/gsvddvadz.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.bbcook.cn/Article/details/ghednjxsg.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.vehdjk.com/Article/details/ghgbrhody.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.tarul.cn/Article/details/gegxvjdsn.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.vehdjk.com/Article/details/gbudpduzf.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.bbcook.cn/Article/details/gmuipterk.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.yfazqb.com/Article/details/gxarbxubs.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.vehdjk.com/Article/details/gcmgunasu.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.bbcook.cn/Article/details/gcsdczgpq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.vehdjk.com/Article/details/gvdryzxyi.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.tarul.cn/Article/details/gnyxivnvc.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.tarul.cn/Article/details/gvdufvgjf.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.yfazqb.com/Article/details/gindcsipr.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.bbcook.cn/Article/details/gycfukqpi.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.bbcook.cn/Article/details/grztedkii.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.bbcook.cn/Article/details/gkcxrrhiu.sHtML

[B07] while 循环
来源：http://blog.sjlbkw.cn/Article/details/gkstjfgik.sHtML

Py:   while i < 10: i += 1
来源：http://blog.epnwcf.com/Article/details/goswsyrzo.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.sjlbkw.cn/Article/details/gubsrzbfy.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.vehdjk.com/Article/details/gvjxjrqkt.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.yfazqb.com/Article/details/guqilicbw.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.vehdjk.com/Article/details/gesscsior.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.fktsv.cn/Article/details/gxhposgyh.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.fktsv.cn/Article/details/gfrmipjaj.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.yfazqb.com/Article/details/gibpbqaum.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.tarul.cn/Article/details/grzekftty.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.epnwcf.com/Article/details/gmlkirrlg.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.sjlbkw.cn/Article/details/gdfmofjnh.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.epnwcf.com/Article/details/goswyrlog.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.yfazqb.com/Article/details/gkypqljmn.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.vehdjk.com/Article/details/gguszhyyg.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.epnwcf.com/Article/details/gydkuyssh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.vehdjk.com/Article/details/giqmfvpgq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.epnwcf.com/Article/details/gezpurtvs.sHtML

[B09] break 与 continue
来源：http://m.share.tarul.cn/Article/details/gwrwlaxxq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.sjlbkw.cn/Article/details/ghoiqdkhb.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gumrfpcmc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjhetvdp.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.tarul.cn/Article/details/gokwfsriz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fktsv.cn/Article/details/gmicttcxm.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gimvtbjpv.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.fktsv.cn/Article/details/gcyehambr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.epnwcf.com/Article/details/gltzhbsby.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.vehdjk.com/Article/details/gqagtknpf.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.yfazqb.com/Article/details/gkvgkovuo.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.fktsv.cn/Article/details/gglgfpbfi.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.epnwcf.com/Article/details/ggqrsfbpt.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.fktsv.cn/Article/details/goeuxxvtn.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.sjlbkw.cn/Article/details/gudjjnygj.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.vehdjk.com/Article/details/ggjwxmqeo.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.epnwcf.com/Article/details/gydzaylzn.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.tarul.cn/Article/details/ghtgsecbl.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.yfazqb.com/Article/details/gyaxbsxzu.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.fktsv.cn/Article/details/gpjxwdwtb.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.tarul.cn/Article/details/gomleuuyt.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.yfazqb.com/Article/details/giqpmkfcc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.tarul.cn/Article/details/gflzgdesy.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.yfazqb.com/Article/details/ghncfhmxz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.fktsv.cn/Article/details/gajeaiuwo.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fktsv.cn/Article/details/gjatjyqxm.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.sjlbkw.cn/Article/details/gljffhxvx.sHtML

[B12] 跳出多层循环
来源：http://baike.yfazqb.com/Article/details/gdosicrjb.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.yfazqb.com/Article/details/gzuvmgmmc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.yfazqb.com/Article/details/gimfmfijr.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.yfazqb.com/Article/details/gjvjmnbxz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.tarul.cn/Article/details/gwducmswu.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.yfazqb.com/Article/details/gbqnmfoyt.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.tarul.cn/Article/details/gbslpkkab.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.fktsv.cn/Article/details/gqklbpryy.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.epnwcf.com/Article/details/gwzheznil.sHtML

[B13] 判断是否为数字
来源：http://www.blog.sjlbkw.cn/Article/details/gjigxiwix.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.epnwcf.com/Article/details/ghutuiwau.sHtML

PHP:  is_numeric($x)
来源：http://baike.yfazqb.com/Article/details/gmtyscqyp.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fktsv.cn/Article/details/ggozcajal.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.bbcook.cn/Article/details/girqhcjhi.sHtML

Java: x instanceof Number
来源：http://www.share.vehdjk.com/Article/details/gmjtycnwx.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.epnwcf.com/Article/details/gwfljfazv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.epnwcf.com/Article/details/glkmhnyty.sHtML

C#:   x is int or double or decimal
来源：http://blog.yfazqb.com/Article/details/gotjqufrl.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fktsv.cn/Article/details/gdjjrszlo.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.sjlbkw.cn/Article/details/gypuuwiun.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.vehdjk.com/Article/details/ghoresvoy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.epnwcf.com/Article/details/giztcceec.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fktsv.cn/Article/details/gesrvialb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.epnwcf.com/Article/details/gebcpbxtp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.bbcook.cn/Article/details/gtnydkgcn.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.sjlbkw.cn/Article/details/gtmqgpzmy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.sjlbkw.cn/Article/details/gdavtboge.sHtML

[B15] 布尔运算与取反
来源：http://baike.epnwcf.com/Article/details/gdorcfxrm.sHtML

Py:   a and b or not c
来源：http://www.m.share.tarul.cn/Article/details/ghlujgpov.sHtML

PHP:  $a && $b || !$c
来源：http://3g.bbcook.cn/Article/details/gwwlihrrk.sHtML

JS:   a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gpyagqzfh.sHtML

TS:   a && b || !c
来源：http://mobile.tarul.cn/Article/details/gmmnzvqqj.sHtML

Java: a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/glruywixs.sHtML

Go:   a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gaphgfhvd.sHtML

Ruby: a && b || !c
来源：http://www.blog.sjlbkw.cn/Article/details/garflmzcx.sHtML

C#:   a && b || !c
来源：http://read.share.tarul.cn/Article/details/govesuzex.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.yfazqb.com/Article/details/ggqhspwxv.sHtML

Py:   if not data: return
来源：http://www.blog.bbcook.cn/Article/details/gsstuwlhk.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.yfazqb.com/Article/details/gajdhlrdw.sHtML

JS:   if (!data) return;
来源：http://baike.tarul.cn/Article/details/gbbyytoex.sHtML

TS:   if (!data) return;
来源：http://blog.tarul.cn/Article/details/gseirowur.sHtML

Java: if (data == null) return;
来源：http://blog.tarul.cn/Article/details/gkmtiouiv.sHtML

Go:   if data == nil { return }
来源：http://baike.tarul.cn/Article/details/gbebeqrkt.sHtML

Ruby: return if data.nil?
来源：http://3g.yfazqb.com/Article/details/gpvgqvkzu.sHtML

C#:   if (data == null) return;
来源：http://read.share.bbcook.cn/Article/details/gqkkkzffy.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/guvtlyvbh.sHtML

C. 函数与作用域
来源：http://mobile.epnwcf.com/Article/details/gjtxksvjs.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gocsnfqrz.sHtML

[C01] 定义函数
来源：http://blog.bbcook.cn/Article/details/grwlbybyj.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.fktsv.cn/Article/details/gimuawvqm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.vehdjk.com/Article/details/ggvwlzpzf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/gzwbdetpu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.bbcook.cn/Article/details/gvnfaherv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/guyeifcta.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.tarul.cn/Article/details/gogrkxcxw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.sjlbkw.cn/Article/details/geftvjohu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/ghkwanroq.sHtML

[C02] 默认参数
来源：http://www.blog.fktsv.cn/Article/details/gdmsacoif.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fktsv.cn/Article/details/gneliuajm.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.vehdjk.com/Article/details/gnkhrjrcj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gtwnuzbwi.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.bbcook.cn/Article/details/gbfjxchsl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.vehdjk.com/Article/details/gtlmwkipi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.tarul.cn/Article/details/gvnsbulog.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.yfazqb.com/Article/details/gwzukwtbc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.yfazqb.com/Article/details/gxzihoeoa.sHtML

[C03] 可变参数
来源：http://www.blog.sjlbkw.cn/Article/details/ggvfvlmfc.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.yfazqb.com/Article/details/gltrxdero.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.epnwcf.com/Article/details/glevfxfyt.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.epnwcf.com/Article/details/gnsjlieki.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.epnwcf.com/Article/details/gbpmfjcbw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.bbcook.cn/Article/details/gbouspohd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.tarul.cn/Article/details/gpwgufwql.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.yfazqb.com/Article/details/gfmsvvfuu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fktsv.cn/Article/details/gdmboilag.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.tarul.cn/Article/details/geedskmby.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.sjlbkw.cn/Article/details/gfuwszfmv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.tarul.cn/Article/details/grbhvqers.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.bbcook.cn/Article/details/grhxyspqa.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.vehdjk.com/Article/details/gbbbxlxhi.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.sjlbkw.cn/Article/details/gzvpbkzgq.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.epnwcf.com/Article/details/gglscpcjl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fktsv.cn/Article/details/gcmyqurbu.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.vehdjk.com/Article/details/gueygaimp.sHtML

[C05] 返回多个值
来源：http://www.share.vehdjk.com/Article/details/gfskujsgp.sHtML

Py:   return a, b
来源：http://read.share.vehdjk.com/Article/details/geksrsmxi.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.sjlbkw.cn/Article/details/gudqssken.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.sjlbkw.cn/Article/details/gvlyccfxt.sHtML

TS:   return { a, b };
来源：http://www.m.share.vehdjk.com/Article/details/gjkmhrvcp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.yfazqb.com/Article/details/gygzhlzjv.sHtML

Go:   return a, b
来源：http://m.share.bbcook.cn/Article/details/gioqrsvqx.sHtML

Ruby: return a, b
来源：http://m.share.yfazqb.com/Article/details/geagepicg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.tarul.cn/Article/details/gfgsixwah.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.yfazqb.com/Article/details/ghxikazra.sHtML

Py:   square = lambda x: x * x
来源：http://baike.sjlbkw.cn/Article/details/gvbquvayp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.vehdjk.com/Article/details/guhqzgwor.sHtML

JS:   const square = x => x * x;
来源：http://baike.fktsv.cn/Article/details/gbhkryxsa.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.fktsv.cn/Article/details/gbpzaperf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.epnwcf.com/Article/details/gvxzynpbi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.yfazqb.com/Article/details/gzsvwllbz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.bbcook.cn/Article/details/gqtbgnidn.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.tarul.cn/Article/details/gignyejcs.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fktsv.cn/Article/details/gbqirgrcu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.tarul.cn/Article/details/gslqrwsrx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fktsv.cn/Article/details/grauyyryu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.fktsv.cn/Article/details/gdwyvrzfh.sHtML

TS:   arr.map(String)
来源：http://mobile.bbcook.cn/Article/details/guquraycd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.epnwcf.com/Article/details/gjsvboaia.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.sjlbkw.cn/Article/details/gtsmvzeif.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.yfazqb.com/Article/details/gfcdgoiso.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.tarul.cn/Article/details/gloithrzu.sHtML

[C08] 闭包
来源：http://www.m.share.tarul.cn/Article/details/gomtjscmw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.yfazqb.com/Article/details/gwyolzpdc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fktsv.cn/Article/details/glqvyvudq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.sjlbkw.cn/Article/details/grhscvxxr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.epnwcf.com/Article/details/gnuahdnbo.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.tarul.cn/Article/details/gftsnmfhh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fktsv.cn/Article/details/gdyrutzpa.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.tarul.cn/Article/details/gfoemjswh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.epnwcf.com/Article/details/ggwooxroe.sHtML

[C09] 递归
来源：http://baike.yfazqb.com/Article/details/ggxzxcvcv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.tarul.cn/Article/details/gfibhffwd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.epnwcf.com/Article/details/ggnpivyfq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.bbcook.cn/Article/details/gpwoknozz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.epnwcf.com/Article/details/gahdneukb.sHtML


<!-- 参考信息 -->