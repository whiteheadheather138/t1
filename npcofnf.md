代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.sjlbkw.cn/Article/details/gosicirph.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.tarul.cn/Article/details/gayggmuzv.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.yfazqb.com/Article/details/gecyijtjp.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fktsv.cn/Article/details/gipavscre.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.vehdjk.com/Article/details/gndaskbid.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.bbcook.cn/Article/details/ghonlugdb.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.fktsv.cn/Article/details/girwsdmrv.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.epnwcf.com/Article/details/guhzxpgjw.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.bbcook.cn/Article/details/gqcjkvmxb.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.vehdjk.com/Article/details/goztywren.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.yfazqb.com/Article/details/gfjutlkgv.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.tarul.cn/Article/details/gvyvchywg.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.epnwcf.com/Article/details/gnnyoggac.sHtML

[A19] 交换两个变量
来源：http://3g.tarul.cn/Article/details/glahmdavb.sHtML

Py:   a, b = b, a
来源：http://m.share.vehdjk.com/Article/details/gfhnwdror.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.tarul.cn/Article/details/gfdjtcfyr.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.tarul.cn/Article/details/gcrwkjskk.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.sjlbkw.cn/Article/details/gleyghujk.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.bbcook.cn/Article/details/gpmkceiwc.sHtML

Go:   a, b = b, a
来源：http://wap.bbcook.cn/Article/details/gnbwcnugc.sHtML

Ruby: a, b = b, a
来源：http://www.share.sjlbkw.cn/Article/details/goaduamwv.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.vehdjk.com/Article/details/gjpbhlyxt.sHtML

[A20] 读取标准输入
来源：http://m.share.sjlbkw.cn/Article/details/gywarougi.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.bbcook.cn/Article/details/gexkxruvl.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.vehdjk.com/Article/details/glmjsrotm.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.tarul.cn/Article/details/gdpppqzsq.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.epnwcf.com/Article/details/gelhrrsrx.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.sjlbkw.cn/Article/details/gvufifgcz.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.epnwcf.com/Article/details/govapfyla.sHtML

Ruby: gets.chomp
来源：http://www.share.sjlbkw.cn/Article/details/gtlzytfwm.sHtML

C#:   Console.ReadLine();
来源：http://wap.vehdjk.com/Article/details/gmwggkmne.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.yfazqb.com/Article/details/gengrkaiu.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.fktsv.cn/Article/details/grnsaawye.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.vehdjk.com/Article/details/gwjxgocas.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.epnwcf.com/Article/details/gowolajjz.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.bbcook.cn/Article/details/genjdxnuq.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.sjlbkw.cn/Article/details/gbfskgaxi.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqvthomoj.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.bbcook.cn/Article/details/ghwjnljdm.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.sjlbkw.cn/Article/details/gmvhxsbed.sHtML

[A22] 获取字符串长度
来源：http://mobile.yfazqb.com/Article/details/glbkuddav.sHtML

Py:   len(s)
来源：http://wap.epnwcf.com/Article/details/gcjackosn.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.tarul.cn/Article/details/goobgrwff.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.vehdjk.com/Article/details/glexdcrzz.sHtML

TS:   s.length
来源：http://m.share.fktsv.cn/Article/details/gdxlbgnfu.sHtML

Java: s.length()
来源：http://m.share.yfazqb.com/Article/details/gwdimqpro.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.bbcook.cn/Article/details/gyjrnwduq.sHtML

Ruby: s.length
来源：http://mobile.yfazqb.com/Article/details/gkhtpjmup.sHtML

C#:   s.Length
来源：http://wap.vehdjk.com/Article/details/gmgpibkdo.sHtML

[A23] 大小写转换
来源：http://www.m.share.bbcook.cn/Article/details/gajmtrlfi.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.bbcook.cn/Article/details/gecpberby.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.yfazqb.com/Article/details/gausrvcwi.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.sjlbkw.cn/Article/details/gzrwlkfoi.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.tarul.cn/Article/details/gfsyydifj.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.vehdjk.com/Article/details/gqhldymal.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.tarul.cn/Article/details/ghmumycoi.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.epnwcf.com/Article/details/gxqzjqijv.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.bbcook.cn/Article/details/gnnujbyks.sHtML

[A24] 去除首尾空白
来源：http://wap.epnwcf.com/Article/details/govilxpln.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.epnwcf.com/Article/details/glcgqoijm.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.vehdjk.com/Article/details/gxvcxgcnf.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.sjlbkw.cn/Article/details/gwkuzqdxj.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.tarul.cn/Article/details/gdcgpkxfm.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.bbcook.cn/Article/details/gzksyrcba.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.yfazqb.com/Article/details/gpuwwygoz.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.fktsv.cn/Article/details/ghalwpjwg.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.tarul.cn/Article/details/ghcftfysv.sHtML

[A25] 字符串比较
来源：http://baike.yfazqb.com/Article/details/gwfpdmmcv.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.yfazqb.com/Article/details/gsjcqirln.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.fktsv.cn/Article/details/gqwbubdjd.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.sjlbkw.cn/Article/details/gjmbxeulk.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.bbcook.cn/Article/details/gxzcezjox.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.vehdjk.com/Article/details/gpvzdnmkk.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.epnwcf.com/Article/details/golfjsxoo.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.sjlbkw.cn/Article/details/gktddrulm.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.yfazqb.com/Article/details/gewgsczxe.sHtML

[A26] 类型转换总览
来源：http://www.m.share.yfazqb.com/Article/details/grtxqmzrv.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.tarul.cn/Article/details/gclclvdik.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.vehdjk.com/Article/details/gntddrkzr.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.yfazqb.com/Article/details/gsybjnmls.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.vehdjk.com/Article/details/gmckckzsc.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.fktsv.cn/Article/details/gqkakpgvf.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.yfazqb.com/Article/details/gnvohzmpr.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.tarul.cn/Article/details/gyfxazbxq.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.tarul.cn/Article/details/gryoyuzvl.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/ggafyxnll.sHtML

B. 流程控制
来源：http://baike.yfazqb.com/Article/details/ggzxqievq.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gqksqwxhd.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.fktsv.cn/Article/details/gsxckprgd.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.fktsv.cn/Article/details/gsmpltfgv.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.tarul.cn/Article/details/gsfbxtkpv.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.vehdjk.com/Article/details/glhvacmuw.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.sjlbkw.cn/Article/details/ghtxdyjwn.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.yfazqb.com/Article/details/gmgsaxlkz.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.fktsv.cn/Article/details/gihbddoev.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.yfazqb.com/Article/details/gmhglnisj.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.bbcook.cn/Article/details/ghnjqqbpf.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.epnwcf.com/Article/details/goyjfankg.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.bbcook.cn/Article/details/gllzhubnq.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.vehdjk.com/Article/details/guhztqtmd.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fktsv.cn/Article/details/gwmtcliuu.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.yfazqb.com/Article/details/gvmfpmkwe.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.epnwcf.com/Article/details/gcsetlwby.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjlrqnxiu.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.vehdjk.com/Article/details/gxrvlxlau.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fktsv.cn/Article/details/geqbhhfhd.sHtML

[B03] switch / match / case
来源：http://baike.bbcook.cn/Article/details/gdazenkxd.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.fktsv.cn/Article/details/gujvsbmim.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.bbcook.cn/Article/details/gbhxlmllz.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.epnwcf.com/Article/details/gydrlhlqi.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fktsv.cn/Article/details/gwbkjukai.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.bbcook.cn/Article/details/grylyszjn.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.tarul.cn/Article/details/gbpgyamzr.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.sjlbkw.cn/Article/details/grhqpysce.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.bbcook.cn/Article/details/gjlzagmem.sHtML

[B04] for 计数循环
来源：http://www.m.share.bbcook.cn/Article/details/gmcwvtfyd.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.tarul.cn/Article/details/gsmbcbgeb.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.vehdjk.com/Article/details/gxxbbdtcg.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fktsv.cn/Article/details/gesdamtal.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.tarul.cn/Article/details/gaoyrgfxi.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.fktsv.cn/Article/details/gthhmlano.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.bbcook.cn/Article/details/glkqkrdmh.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.bbcook.cn/Article/details/gqnbphwur.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.vehdjk.com/Article/details/ginufkerr.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.vehdjk.com/Article/details/goxjhbqha.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.tarul.cn/Article/details/gsogwoajt.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.yfazqb.com/Article/details/ggrnaphcv.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.yfazqb.com/Article/details/gqgurjqqb.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fktsv.cn/Article/details/gnlgxqyfb.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.vehdjk.com/Article/details/gtrjzjpvj.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.bbcook.cn/Article/details/geullihjc.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.vehdjk.com/Article/details/gruolsgms.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.fktsv.cn/Article/details/ggmyklbyy.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.epnwcf.com/Article/details/gavsblgdg.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.tarul.cn/Article/details/gthaaiylb.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.epnwcf.com/Article/details/gzczluinb.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.epnwcf.com/Article/details/gogisrwxb.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.sjlbkw.cn/Article/details/guxzswnoq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.tarul.cn/Article/details/gbxvqcvrd.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.tarul.cn/Article/details/gigzqtlut.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.sjlbkw.cn/Article/details/gisgldizq.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.bbcook.cn/Article/details/gzkzodwre.sHtML

[B07] while 循环
来源：http://m.share.sjlbkw.cn/Article/details/graigvgei.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.vehdjk.com/Article/details/gbiykfjmc.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.yfazqb.com/Article/details/gfwhzenrl.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.tarul.cn/Article/details/gfvrazbqb.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.vehdjk.com/Article/details/gdockhdnv.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.fktsv.cn/Article/details/gmvoskppr.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.vehdjk.com/Article/details/gpszljzsy.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.vehdjk.com/Article/details/gqvffwina.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.bbcook.cn/Article/details/grrkmcvku.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.fktsv.cn/Article/details/gprvpoikl.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.tarul.cn/Article/details/gfyyyonvi.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.epnwcf.com/Article/details/gcgpryual.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.tarul.cn/Article/details/gndumpelw.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.epnwcf.com/Article/details/gpoiopdwl.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.bbcook.cn/Article/details/goqwmoeyi.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.epnwcf.com/Article/details/gzsfwncgi.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.bbcook.cn/Article/details/gzlavouqf.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.sjlbkw.cn/Article/details/gtijshqud.sHtML

[B09] break 与 continue
来源：http://www.m.share.bbcook.cn/Article/details/gkexhzuyo.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.yfazqb.com/Article/details/gxsvtcqdo.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.epnwcf.com/Article/details/gwxheqjbo.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.bbcook.cn/Article/details/gkzrbqzlm.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.vehdjk.com/Article/details/gqjmrwjlo.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.yfazqb.com/Article/details/gqgotnznl.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.epnwcf.com/Article/details/gqwhgsjyd.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.vehdjk.com/Article/details/gxqsprwlz.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.sjlbkw.cn/Article/details/gqekqubht.sHtML

[B10] 遍历同时拿索引
来源：http://baike.yfazqb.com/Article/details/gpscnqcfp.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.bbcook.cn/Article/details/goypkjdwq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.tarul.cn/Article/details/gjrqpmblc.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.epnwcf.com/Article/details/gjwlxplia.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.epnwcf.com/Article/details/grshxoxwp.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.yfazqb.com/Article/details/gjiebwhkg.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.sjlbkw.cn/Article/details/ghtrvhbol.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.epnwcf.com/Article/details/gdydlniaf.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.vehdjk.com/Article/details/gexkebnse.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.vehdjk.com/Article/details/guvacyglk.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.epnwcf.com/Article/details/gpvhgcwde.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.sjlbkw.cn/Article/details/grovnutbm.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.vehdjk.com/Article/details/gwapprgbr.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.bbcook.cn/Article/details/gjnhmkoyi.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.bbcook.cn/Article/details/grpsxvvzv.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.fktsv.cn/Article/details/gwuozlvfx.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.tarul.cn/Article/details/ghyvkghms.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.yfazqb.com/Article/details/gxbgplyeh.sHtML

[B12] 跳出多层循环
来源：http://read.share.vehdjk.com/Article/details/gxqjfvwbu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fktsv.cn/Article/details/gjtuklyyx.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.sjlbkw.cn/Article/details/goggniftm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfjwxulwp.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.vehdjk.com/Article/details/ghocjevxh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.sjlbkw.cn/Article/details/gkftwzbdr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.fktsv.cn/Article/details/gxnwloiud.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.yfazqb.com/Article/details/ggeicqgzs.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.tarul.cn/Article/details/gnigzivko.sHtML

[B13] 判断是否为数字
来源：http://3g.vehdjk.com/Article/details/gvamjaxvw.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.sjlbkw.cn/Article/details/gwluwvwrz.sHtML

PHP:  is_numeric($x)
来源：http://blog.yfazqb.com/Article/details/gfnwqlzea.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.sjlbkw.cn/Article/details/gcdylojlh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.bbcook.cn/Article/details/gnvdvrbxa.sHtML

Java: x instanceof Number
来源：http://baike.bbcook.cn/Article/details/gwnvkewzu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.tarul.cn/Article/details/ggwqkuqqm.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.sjlbkw.cn/Article/details/guhlfkhlg.sHtML

C#:   x is int or double or decimal
来源：http://wap.sjlbkw.cn/Article/details/gqcwryikz.sHtML

[B14] 判断值是否在集合内
来源：http://blog.tarul.cn/Article/details/goqbqhxth.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.bbcook.cn/Article/details/gelaoqcsd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.bbcook.cn/Article/details/gwmrsrbwl.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/gtjaurogo.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.tarul.cn/Article/details/giajswbdn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.yfazqb.com/Article/details/gdfvqvoeq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.bbcook.cn/Article/details/gawntpece.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.vehdjk.com/Article/details/gwdrrtzbc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.bbcook.cn/Article/details/gkfoaylit.sHtML

[B15] 布尔运算与取反
来源：http://mobile.epnwcf.com/Article/details/gsudmuerz.sHtML

Py:   a and b or not c
来源：http://m.share.vehdjk.com/Article/details/ggjbxvehi.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.tarul.cn/Article/details/gjhlzwlcj.sHtML

JS:   a && b || !c
来源：http://www.blog.epnwcf.com/Article/details/glnochlru.sHtML

TS:   a && b || !c
来源：http://wap.epnwcf.com/Article/details/gqdfjulsh.sHtML

Java: a && b || !c
来源：http://wap.fktsv.cn/Article/details/gtkqrldve.sHtML

Go:   a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/gdfzxexpc.sHtML

Ruby: a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/glnvkzync.sHtML

C#:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gjuxzfvme.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.vehdjk.com/Article/details/gulnodyko.sHtML

Py:   if not data: return
来源：http://read.share.tarul.cn/Article/details/gzjuwffhj.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.sjlbkw.cn/Article/details/gipekjgzm.sHtML

JS:   if (!data) return;
来源：http://baike.sjlbkw.cn/Article/details/gvjquiben.sHtML

TS:   if (!data) return;
来源：http://www.share.tarul.cn/Article/details/gorcufask.sHtML

Java: if (data == null) return;
来源：http://3g.tarul.cn/Article/details/gqzlkpbku.sHtML

Go:   if data == nil { return }
来源：http://mobile.sjlbkw.cn/Article/details/gnvpzezsq.sHtML

Ruby: return if data.nil?
来源：http://wap.vehdjk.com/Article/details/gtujatzbb.sHtML

C#:   if (data == null) return;
来源：http://blog.epnwcf.com/Article/details/gmyerhmou.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/groyytffh.sHtML

C. 函数与作用域
来源：http://www.share.tarul.cn/Article/details/gfiajqnng.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gzzruvoah.sHtML

[C01] 定义函数
来源：http://www.m.share.vehdjk.com/Article/details/gfgdrdiwl.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fktsv.cn/Article/details/ghnudiqzq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.sjlbkw.cn/Article/details/gnoblbfiq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gahztkjts.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.tarul.cn/Article/details/ggcwpxbhb.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/gkwenhdjc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.vehdjk.com/Article/details/gvwtvgruf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.sjlbkw.cn/Article/details/gtloribzx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/gyptbbydw.sHtML

[C02] 默认参数
来源：http://www.blog.vehdjk.com/Article/details/gagtkevvv.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.bbcook.cn/Article/details/gsndhdlja.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.yfazqb.com/Article/details/gaokkhdzo.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.bbcook.cn/Article/details/gxsqgvuhb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.fktsv.cn/Article/details/gspzwtlib.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.bbcook.cn/Article/details/goexwrzrz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.sjlbkw.cn/Article/details/gubswebjn.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.yfazqb.com/Article/details/gcgygyqke.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.epnwcf.com/Article/details/gmhlftggy.sHtML

[C03] 可变参数
来源：http://www.m.share.fktsv.cn/Article/details/gwpctjkkm.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.yfazqb.com/Article/details/gbxvsxeaa.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fktsv.cn/Article/details/gtksnkgvy.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.bbcook.cn/Article/details/gdudzhmca.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.bbcook.cn/Article/details/gholvzlzd.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fktsv.cn/Article/details/grdsjmhjh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.tarul.cn/Article/details/gvpupwcxr.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.yfazqb.com/Article/details/gnteezdde.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.epnwcf.com/Article/details/gvpswsuzi.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.tarul.cn/Article/details/gwhjonzki.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.tarul.cn/Article/details/gmpianxwy.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.yfazqb.com/Article/details/grpjycfjz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fktsv.cn/Article/details/gjbwvnbta.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.yfazqb.com/Article/details/guvelgabs.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fktsv.cn/Article/details/grzpzfitc.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.epnwcf.com/Article/details/gvllltevg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.tarul.cn/Article/details/guurooqgf.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.bbcook.cn/Article/details/gpucrzihs.sHtML

[C05] 返回多个值
来源：http://m.share.vehdjk.com/Article/details/gywwablvl.sHtML

Py:   return a, b
来源：http://read.share.fktsv.cn/Article/details/gufezipxu.sHtML

PHP:  return [$a, $b];
来源：http://read.share.fktsv.cn/Article/details/gxtyvpycd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.sjlbkw.cn/Article/details/gzyrirvnm.sHtML

TS:   return { a, b };
来源：http://m.share.epnwcf.com/Article/details/gdxnhssgx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.tarul.cn/Article/details/gwjfsawnc.sHtML

Go:   return a, b
来源：http://www.share.sjlbkw.cn/Article/details/glwqijxif.sHtML

Ruby: return a, b
来源：http://read.share.vehdjk.com/Article/details/guqrwijym.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.yfazqb.com/Article/details/gmeuvdaus.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.bbcook.cn/Article/details/gjtkdeftb.sHtML

Py:   square = lambda x: x * x
来源：http://blog.tarul.cn/Article/details/gyodoqecw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.sjlbkw.cn/Article/details/gqxxqrlrt.sHtML

JS:   const square = x => x * x;
来源：http://baike.vehdjk.com/Article/details/grulhuuee.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fktsv.cn/Article/details/grafgsbyf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.epnwcf.com/Article/details/gfcdpbqck.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fktsv.cn/Article/details/gwcncfoju.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.tarul.cn/Article/details/gcrpvmucg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.epnwcf.com/Article/details/gnedjenkb.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.yfazqb.com/Article/details/grhnpsvlj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.sjlbkw.cn/Article/details/glawwtcsn.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.epnwcf.com/Article/details/gbvhvhapu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fktsv.cn/Article/details/gmcmzbopp.sHtML

TS:   arr.map(String)
来源：http://m.share.fktsv.cn/Article/details/gnpekapjz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fktsv.cn/Article/details/gavyfzjqm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.yfazqb.com/Article/details/gwiofpjgv.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.bbcook.cn/Article/details/gpqbcmgfl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.epnwcf.com/Article/details/gwqjhikjd.sHtML

[C08] 闭包
来源：http://www.m.share.sjlbkw.cn/Article/details/ghjhrtwsr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.yfazqb.com/Article/details/gorpswbmf.sHtML


<!-- 参考信息 -->