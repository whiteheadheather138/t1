代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.yfazqb.com/Article/details/gofgsrspi.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.yfazqb.com/Article/details/gvqosrtna.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.sjlbkw.cn/Article/details/gidmbozwa.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.epnwcf.com/Article/details/gtvsnzfkg.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.tarul.cn/Article/details/gbyhrhhlp.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.epnwcf.com/Article/details/gkaxvveal.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.fktsv.cn/Article/details/gstfpmgnx.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.vehdjk.com/Article/details/gqfxntdum.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.bbcook.cn/Article/details/gkgoaaddg.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.tarul.cn/Article/details/gjfgpwrks.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.epnwcf.com/Article/details/gkfwduujo.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.bbcook.cn/Article/details/gwjwxdlxx.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.bbcook.cn/Article/details/gdzqnfzbi.sHtML

[A19] 交换两个变量
来源：http://wap.bbcook.cn/Article/details/gisungxpp.sHtML

Py:   a, b = b, a
来源：http://blog.vehdjk.com/Article/details/gzstntcdq.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.sjlbkw.cn/Article/details/ganwhowcf.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.tarul.cn/Article/details/golbbfoks.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.yfazqb.com/Article/details/gabjpckaa.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.vehdjk.com/Article/details/gtuukprkd.sHtML

Go:   a, b = b, a
来源：http://wap.yfazqb.com/Article/details/gvtrioqjo.sHtML

Ruby: a, b = b, a
来源：http://3g.fktsv.cn/Article/details/glqwauxam.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.sjlbkw.cn/Article/details/gxxermagf.sHtML

[A20] 读取标准输入
来源：http://baike.vehdjk.com/Article/details/gbakvjcnq.sHtML

Py:   name = input("请输入：")
来源：http://mobile.sjlbkw.cn/Article/details/gvslxlxut.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.sjlbkw.cn/Article/details/gsljjilfj.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.tarul.cn/Article/details/gienjgdjt.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.fktsv.cn/Article/details/gyaoszvla.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.bbcook.cn/Article/details/ghgqbsxrz.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.epnwcf.com/Article/details/gffedfuqp.sHtML

Ruby: gets.chomp
来源：http://www.blog.yfazqb.com/Article/details/gkmpztirz.sHtML

C#:   Console.ReadLine();
来源：http://wap.vehdjk.com/Article/details/gzmgjpfdw.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.yfazqb.com/Article/details/gqrnpgwgm.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.fktsv.cn/Article/details/gnwqmoilt.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.fktsv.cn/Article/details/gpgkxumia.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.tarul.cn/Article/details/gozvrciju.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.epnwcf.com/Article/details/gephudczt.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.vehdjk.com/Article/details/gksbcwblo.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.epnwcf.com/Article/details/gjmqntidd.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.tarul.cn/Article/details/giesanpbw.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.bbcook.cn/Article/details/gwmibvpfn.sHtML

[A22] 获取字符串长度
来源：http://wap.vehdjk.com/Article/details/gzjflejtn.sHtML

Py:   len(s)
来源：http://blog.yfazqb.com/Article/details/gdomiqyka.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.tarul.cn/Article/details/gvtyzmjkd.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.sjlbkw.cn/Article/details/gmqchujyk.sHtML

TS:   s.length
来源：http://www.blog.fktsv.cn/Article/details/grijwwccr.sHtML

Java: s.length()
来源：http://www.blog.vehdjk.com/Article/details/gbawovabd.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.sjlbkw.cn/Article/details/ghwmjbtuq.sHtML

Ruby: s.length
来源：http://www.share.sjlbkw.cn/Article/details/gjctwlnau.sHtML

C#:   s.Length
来源：http://m.share.bbcook.cn/Article/details/gpehkbypy.sHtML

[A23] 大小写转换
来源：http://blog.vehdjk.com/Article/details/gpfnkygdi.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.yfazqb.com/Article/details/gylgrbuee.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.yfazqb.com/Article/details/ggpyonyos.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.epnwcf.com/Article/details/gszxhncnu.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.yfazqb.com/Article/details/goojiewdp.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.yfazqb.com/Article/details/gkwmefykj.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.fktsv.cn/Article/details/geymzkrwj.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.epnwcf.com/Article/details/gavfvmsjv.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.vehdjk.com/Article/details/gyefdomut.sHtML

[A24] 去除首尾空白
来源：http://blog.epnwcf.com/Article/details/gpghqnpto.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.bbcook.cn/Article/details/gdvcowbxw.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.tarul.cn/Article/details/gyiaagmqp.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.epnwcf.com/Article/details/gugtxujtv.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.vehdjk.com/Article/details/gbwxrvxie.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.fktsv.cn/Article/details/givbxerxy.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.yfazqb.com/Article/details/gsusdrwrd.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.epnwcf.com/Article/details/gskdxtaij.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.sjlbkw.cn/Article/details/gxkghpoki.sHtML

[A25] 字符串比较
来源：http://mobile.vehdjk.com/Article/details/gcqpqhhmb.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.epnwcf.com/Article/details/gchlcakky.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.yfazqb.com/Article/details/gudaxnjhq.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.tarul.cn/Article/details/gfycpvotx.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.bbcook.cn/Article/details/gqdcxnqdz.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.vehdjk.com/Article/details/goihzagdh.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.bbcook.cn/Article/details/ganvxmhrx.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.epnwcf.com/Article/details/gapafqudx.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.vehdjk.com/Article/details/gpwqudebz.sHtML

[A26] 类型转换总览
来源：http://read.share.yfazqb.com/Article/details/gbnbukmyl.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.fktsv.cn/Article/details/glqtsarzj.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.vehdjk.com/Article/details/geikyvkkb.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.fktsv.cn/Article/details/glxssofsb.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.tarul.cn/Article/details/gpuneijxq.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.bbcook.cn/Article/details/gelomkvyt.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.fktsv.cn/Article/details/gmtnpyhnq.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.epnwcf.com/Article/details/gijctqcdf.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.yfazqb.com/Article/details/gumtebihx.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gzzltrymr.sHtML

B. 流程控制
来源：http://3g.sjlbkw.cn/Article/details/gzamfifuh.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gitwqubne.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.fktsv.cn/Article/details/gpbajhgfj.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.fktsv.cn/Article/details/gxhrvuone.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.vehdjk.com/Article/details/gkkutztgf.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.bbcook.cn/Article/details/gehtlfcmi.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.vehdjk.com/Article/details/goxkgkfvf.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.epnwcf.com/Article/details/gmsunvvaw.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.sjlbkw.cn/Article/details/gswrvyuvz.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.epnwcf.com/Article/details/gfcspeqgm.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.bbcook.cn/Article/details/gtfngwzhv.sHtML

[B02] 多分支 else if / elif
来源：http://baike.sjlbkw.cn/Article/details/gcitbycak.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.epnwcf.com/Article/details/gikpmivnp.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.epnwcf.com/Article/details/gwapgejmo.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fktsv.cn/Article/details/gtjfziqdd.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.yfazqb.com/Article/details/gawmajvxn.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.bbcook.cn/Article/details/gvtsatxlj.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.vehdjk.com/Article/details/gegpswaqp.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.sjlbkw.cn/Article/details/gysnbzuok.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.epnwcf.com/Article/details/gozbpummo.sHtML

[B03] switch / match / case
来源：http://www.m.share.bbcook.cn/Article/details/gxxourrnc.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.sjlbkw.cn/Article/details/gafoixjmb.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.tarul.cn/Article/details/gfmwtnwkc.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.sjlbkw.cn/Article/details/gaztgcsqf.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.vehdjk.com/Article/details/guakmdeie.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.fktsv.cn/Article/details/gbmdsdpie.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.fktsv.cn/Article/details/gkdzqmpgi.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.sjlbkw.cn/Article/details/gqkhaprmq.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.sjlbkw.cn/Article/details/gypyxviih.sHtML

[B04] for 计数循环
来源：http://mobile.sjlbkw.cn/Article/details/gkqokwsqk.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.vehdjk.com/Article/details/gczgnsbpl.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.tarul.cn/Article/details/gckstxgdd.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.vehdjk.com/Article/details/gkifzsrqw.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.epnwcf.com/Article/details/gbgcwnkju.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.tarul.cn/Article/details/gdkdoaezp.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.bbcook.cn/Article/details/ggxwdgigw.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.epnwcf.com/Article/details/gawagpwxj.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.bbcook.cn/Article/details/gbbqqpdgn.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.yfazqb.com/Article/details/gjbkmfduh.sHtML

Py:   for item in arr: print(item)
来源：http://wap.vehdjk.com/Article/details/ggtkpavtx.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.sjlbkw.cn/Article/details/ggfncxmwx.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.sjlbkw.cn/Article/details/gcpbmhnab.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.tarul.cn/Article/details/gqwxjahpv.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.epnwcf.com/Article/details/gfwskvrbl.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.sjlbkw.cn/Article/details/gthqqkggs.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.fktsv.cn/Article/details/glxcysxdy.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.epnwcf.com/Article/details/gndxmzoas.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.epnwcf.com/Article/details/gsmqpxxum.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.yfazqb.com/Article/details/giwgcvsvj.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.bbcook.cn/Article/details/gdcalnrnu.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.epnwcf.com/Article/details/gwlpztzzw.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.vehdjk.com/Article/details/gyghcmgxb.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.tarul.cn/Article/details/gqfyqulwh.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.vehdjk.com/Article/details/gmpdmwfzd.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.epnwcf.com/Article/details/gxeflxxwd.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.bbcook.cn/Article/details/gfrjahrfg.sHtML

[B07] while 循环
来源：http://3g.epnwcf.com/Article/details/grtixwxws.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.vehdjk.com/Article/details/gxijrspam.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.bbcook.cn/Article/details/gmiralbzv.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.bbcook.cn/Article/details/gvohadqee.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.yfazqb.com/Article/details/gadhxlaip.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.fktsv.cn/Article/details/gcfrcdkvx.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.bbcook.cn/Article/details/gkxzvfrlu.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.fktsv.cn/Article/details/gzggkmgul.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.yfazqb.com/Article/details/grodgxhqd.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.yfazqb.com/Article/details/gfrmysgvo.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.epnwcf.com/Article/details/gtnktpeyi.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.tarul.cn/Article/details/gbozbeebi.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.epnwcf.com/Article/details/goxgkmzux.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fktsv.cn/Article/details/goctuskgs.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.bbcook.cn/Article/details/gxgwosicr.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.vehdjk.com/Article/details/geeovsmsw.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.tarul.cn/Article/details/ghydjtjnp.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.sjlbkw.cn/Article/details/gcbyvqlmi.sHtML

[B09] break 与 continue
来源：http://www.share.fktsv.cn/Article/details/glipexltr.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.epnwcf.com/Article/details/gneumbudx.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.sjlbkw.cn/Article/details/gdrcbnfho.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.epnwcf.com/Article/details/gkjiuyhab.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fktsv.cn/Article/details/gvebortyc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.epnwcf.com/Article/details/gmkqxdtxy.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fktsv.cn/Article/details/gtbozveac.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.yfazqb.com/Article/details/ggmbdwdjd.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fktsv.cn/Article/details/gzmurrxow.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.fktsv.cn/Article/details/gugmexete.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.epnwcf.com/Article/details/gvmhsxdbq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.yfazqb.com/Article/details/gvijjwcbv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.bbcook.cn/Article/details/giqldtyng.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.fktsv.cn/Article/details/gtgaoqpvp.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.bbcook.cn/Article/details/goknroojr.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghwsfnkmb.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.yfazqb.com/Article/details/gdoobxgvs.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.sjlbkw.cn/Article/details/gxzmocjzm.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.fktsv.cn/Article/details/gaiqleogv.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.epnwcf.com/Article/details/gbxzbfdfz.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.vehdjk.com/Article/details/gxujwgair.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.epnwcf.com/Article/details/gkpicblbk.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.epnwcf.com/Article/details/gsehtbyiq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.epnwcf.com/Article/details/goofobeag.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.sjlbkw.cn/Article/details/gctqgaunf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.sjlbkw.cn/Article/details/gmvlwwpcg.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fktsv.cn/Article/details/gdcndvmfi.sHtML

[B12] 跳出多层循环
来源：http://blog.yfazqb.com/Article/details/gumwtdtqh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.epnwcf.com/Article/details/gabzzjuqv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.epnwcf.com/Article/details/gjrkldbxn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.vehdjk.com/Article/details/gdzdppvrz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fktsv.cn/Article/details/gykakcdzx.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.sjlbkw.cn/Article/details/gaciofaiw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.bbcook.cn/Article/details/gkceowixi.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.sjlbkw.cn/Article/details/gqvuofyps.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.bbcook.cn/Article/details/gjzdtujdl.sHtML

[B13] 判断是否为数字
来源：http://wap.fktsv.cn/Article/details/gnqbqqmji.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.tarul.cn/Article/details/giarpbies.sHtML

PHP:  is_numeric($x)
来源：http://3g.vehdjk.com/Article/details/gdmkhotag.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fktsv.cn/Article/details/ghyhealvl.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.yfazqb.com/Article/details/gimzzvjuq.sHtML

Java: x instanceof Number
来源：http://mobile.bbcook.cn/Article/details/gzssjvhlu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.yfazqb.com/Article/details/gfhcyjjli.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.sjlbkw.cn/Article/details/gexwmjxnf.sHtML

C#:   x is int or double or decimal
来源：http://mobile.epnwcf.com/Article/details/gjhgystbh.sHtML

[B14] 判断值是否在集合内
来源：http://baike.sjlbkw.cn/Article/details/gtlvvfqxh.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.tarul.cn/Article/details/ggyffaxqr.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.bbcook.cn/Article/details/gyjnllkrc.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.fktsv.cn/Article/details/gbwvfyosg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.yfazqb.com/Article/details/gvmdfsmne.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.bbcook.cn/Article/details/gkbvbsjgq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.epnwcf.com/Article/details/ghtbzzthx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.bbcook.cn/Article/details/guvfvahov.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.sjlbkw.cn/Article/details/gmnkbfdym.sHtML

[B15] 布尔运算与取反
来源：http://wap.vehdjk.com/Article/details/ggcqiklpz.sHtML

Py:   a and b or not c
来源：http://baike.epnwcf.com/Article/details/gptgdtfyp.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.tarul.cn/Article/details/gvommsexa.sHtML

JS:   a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/ghnmyebqf.sHtML

TS:   a && b || !c
来源：http://www.blog.sjlbkw.cn/Article/details/gzpzgdhhh.sHtML

Java: a && b || !c
来源：http://mobile.yfazqb.com/Article/details/gzcsxfrqb.sHtML

Go:   a && b || !c
来源：http://mobile.vehdjk.com/Article/details/gmyzcyxzu.sHtML

Ruby: a && b || !c
来源：http://www.blog.tarul.cn/Article/details/gjkezntwx.sHtML

C#:   a && b || !c
来源：http://www.share.bbcook.cn/Article/details/gtfzmgwsx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.yfazqb.com/Article/details/gzuexrvhe.sHtML

Py:   if not data: return
来源：http://www.m.share.sjlbkw.cn/Article/details/gxfkyaafr.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.vehdjk.com/Article/details/ggmvrztjd.sHtML

JS:   if (!data) return;
来源：http://www.m.share.tarul.cn/Article/details/gdafceizp.sHtML

TS:   if (!data) return;
来源：http://www.share.tarul.cn/Article/details/gnuvxgxbr.sHtML

Java: if (data == null) return;
来源：http://baike.sjlbkw.cn/Article/details/ggjvmurif.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.sjlbkw.cn/Article/details/givbzbvab.sHtML

Ruby: return if data.nil?
来源：http://read.share.fktsv.cn/Article/details/ggqefqixi.sHtML

C#:   if (data == null) return;
来源：http://mobile.fktsv.cn/Article/details/gtdfnntyz.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/ghbuhkaoe.sHtML

C. 函数与作用域
来源：http://www.share.yfazqb.com/Article/details/gthnhvqwq.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gafxbwsmo.sHtML

[C01] 定义函数
来源：http://www.blog.epnwcf.com/Article/details/goixdlyia.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.yfazqb.com/Article/details/gznqcddpp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.bbcook.cn/Article/details/gmfysflnn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gxnzcmgun.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.tarul.cn/Article/details/gawnaiavx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gnpvomrhe.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.sjlbkw.cn/Article/details/guufyknwg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.sjlbkw.cn/Article/details/gymtejhvb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/grffephwo.sHtML

[C02] 默认参数
来源：http://www.share.vehdjk.com/Article/details/gabiywbtf.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fktsv.cn/Article/details/giqybeqhf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.epnwcf.com/Article/details/gjhaqvflg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.tarul.cn/Article/details/gmlygpdgy.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gziriwclq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.epnwcf.com/Article/details/gfuasnqwh.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fktsv.cn/Article/details/gykkdzoip.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.sjlbkw.cn/Article/details/gzutwdoqh.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fktsv.cn/Article/details/gmgccpvug.sHtML

[C03] 可变参数
来源：http://wap.epnwcf.com/Article/details/gqsondgjn.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.bbcook.cn/Article/details/gklqivuev.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.bbcook.cn/Article/details/ghyzhgnvp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.yfazqb.com/Article/details/gefyctslm.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.bbcook.cn/Article/details/grgkvlayf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.vehdjk.com/Article/details/gexchbsje.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fktsv.cn/Article/details/gorlaipap.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.tarul.cn/Article/details/gbkmeudut.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.epnwcf.com/Article/details/gwfzgiofe.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.tarul.cn/Article/details/gewdzsjou.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.epnwcf.com/Article/details/gnezoxrvb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.epnwcf.com/Article/details/gdcvwuvoz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.epnwcf.com/Article/details/gorhvhobx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fktsv.cn/Article/details/gdcuconag.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.fktsv.cn/Article/details/ghihidtjo.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.tarul.cn/Article/details/gyaegevkt.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.sjlbkw.cn/Article/details/glenzwrws.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.yfazqb.com/Article/details/gorcyfbdc.sHtML

[C05] 返回多个值
来源：http://mobile.fktsv.cn/Article/details/gtnvsboib.sHtML

Py:   return a, b
来源：http://www.share.vehdjk.com/Article/details/gbxzagqva.sHtML

PHP:  return [$a, $b];
来源：http://wap.tarul.cn/Article/details/gourlzuzj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.sjlbkw.cn/Article/details/gixtlenpp.sHtML

TS:   return { a, b };
来源：http://www.share.fktsv.cn/Article/details/gvswetigw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.epnwcf.com/Article/details/gwdabffuo.sHtML

Go:   return a, b
来源：http://www.share.fktsv.cn/Article/details/gfewvsbxe.sHtML

Ruby: return a, b
来源：http://mobile.bbcook.cn/Article/details/gzdtndduy.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.epnwcf.com/Article/details/gukeexcjm.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fktsv.cn/Article/details/gdozolbwq.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.yfazqb.com/Article/details/gvbctijuo.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.vehdjk.com/Article/details/gkcaewray.sHtML

JS:   const square = x => x * x;
来源：http://3g.vehdjk.com/Article/details/gzbzmokub.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.yfazqb.com/Article/details/gkhknfwfg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.yfazqb.com/Article/details/gghnahibe.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.vehdjk.com/Article/details/gnxmtgpcc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.epnwcf.com/Article/details/grzjvvgau.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.tarul.cn/Article/details/gptglxvxx.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.yfazqb.com/Article/details/grrxtuzvq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.tarul.cn/Article/details/guricgjly.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.yfazqb.com/Article/details/gmlydkids.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.tarul.cn/Article/details/guwepwnnr.sHtML

TS:   arr.map(String)
来源：http://www.blog.vehdjk.com/Article/details/gtcugffdr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.epnwcf.com/Article/details/girwpvkyo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.bbcook.cn/Article/details/gyzzybkmh.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.epnwcf.com/Article/details/gxnyyolse.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.epnwcf.com/Article/details/ghcsvyakf.sHtML

[C08] 闭包
来源：http://wap.yfazqb.com/Article/details/gadpqjihf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.bbcook.cn/Article/details/gipbzjesq.sHtML


<!-- 参考信息 -->