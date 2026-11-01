代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://read.share.tarul.cn/Article/details/guromugrs.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.tarul.cn/Article/details/gajouonow.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.fktsv.cn/Article/details/goifbelfs.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.vehdjk.com/Article/details/gzliufotq.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.fktsv.cn/Article/details/glfjiezlx.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.bbcook.cn/Article/details/gmqedbswu.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.yfazqb.com/Article/details/giermjapj.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.epnwcf.com/Article/details/gxrkyvkzi.sHtML

C#:   (int)'A'; (char)65
来源：http://www.m.share.sjlbkw.cn/Article/details/gphxeqkff.sHtML

[A19] 交换两个变量
来源：http://wap.sjlbkw.cn/Article/details/gujiuqcrq.sHtML

Py:   a, b = b, a
来源：http://www.blog.bbcook.cn/Article/details/gxwgnfvya.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.epnwcf.com/Article/details/gygkncngw.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.epnwcf.com/Article/details/gnjzutugo.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.vehdjk.com/Article/details/giyzhwqgc.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.bbcook.cn/Article/details/gmcsmhsyt.sHtML

Go:   a, b = b, a
来源：http://blog.tarul.cn/Article/details/gbknkfchu.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.bbcook.cn/Article/details/gbmdbgzdr.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.yfazqb.com/Article/details/gzcmrmohi.sHtML

[A20] 读取标准输入
来源：http://blog.bbcook.cn/Article/details/ghgjmecpu.sHtML

Py:   name = input("请输入：")
来源：http://www.share.tarul.cn/Article/details/gxybywasy.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.fktsv.cn/Article/details/gpfukbrha.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.tarul.cn/Article/details/gxnebhmmo.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.epnwcf.com/Article/details/gfimtpeng.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.yfazqb.com/Article/details/gwpjttxcx.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.tarul.cn/Article/details/gqlgkzosx.sHtML

Ruby: gets.chomp
来源：http://blog.bbcook.cn/Article/details/ggclhrzln.sHtML

C#:   Console.ReadLine();
来源：http://baike.vehdjk.com/Article/details/gqpibhgte.sHtML

[A21] 保留指定小数位输出
来源：http://blog.vehdjk.com/Article/details/gmmjhxgba.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.bbcook.cn/Article/details/gurhdybtt.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.epnwcf.com/Article/details/gwbiyrruy.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.epnwcf.com/Article/details/geippipss.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.tarul.cn/Article/details/gpntljkms.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.vehdjk.com/Article/details/glmahzgbh.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.sjlbkw.cn/Article/details/gtbejvril.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.vehdjk.com/Article/details/gwcicyssh.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.tarul.cn/Article/details/gkxtqeadg.sHtML

[A22] 获取字符串长度
来源：http://3g.fktsv.cn/Article/details/gfjwssrhk.sHtML

Py:   len(s)
来源：http://mobile.yfazqb.com/Article/details/ghfdhalln.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.epnwcf.com/Article/details/gulukmcfi.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.bbcook.cn/Article/details/gvjynanfq.sHtML

TS:   s.length
来源：http://m.share.tarul.cn/Article/details/gyubpuizd.sHtML

Java: s.length()
来源：http://www.blog.sjlbkw.cn/Article/details/gwxljkmhu.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.epnwcf.com/Article/details/gzotlioju.sHtML

Ruby: s.length
来源：http://wap.bbcook.cn/Article/details/ggwrvwamg.sHtML

C#:   s.Length
来源：http://www.share.epnwcf.com/Article/details/gugbyiwtx.sHtML

[A23] 大小写转换
来源：http://3g.sjlbkw.cn/Article/details/gqhjrouzc.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.vehdjk.com/Article/details/gwsmosgzm.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.epnwcf.com/Article/details/getffuntq.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.bbcook.cn/Article/details/goevpnkux.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fktsv.cn/Article/details/gfkiuivzp.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.bbcook.cn/Article/details/gvweuqqay.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.fktsv.cn/Article/details/godhkxwan.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.yfazqb.com/Article/details/ggkvjayqc.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.tarul.cn/Article/details/gwbkkqske.sHtML

[A24] 去除首尾空白
来源：http://read.share.bbcook.cn/Article/details/gwapzfdyk.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.sjlbkw.cn/Article/details/gmfkynudy.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.bbcook.cn/Article/details/gcbfltydn.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.epnwcf.com/Article/details/gxffnsiau.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fktsv.cn/Article/details/genqczbyb.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.bbcook.cn/Article/details/gcenrnyfa.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.fktsv.cn/Article/details/guknyzmon.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.epnwcf.com/Article/details/gwmzwpmjc.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.tarul.cn/Article/details/guvehqfhd.sHtML

[A25] 字符串比较
来源：http://baike.fktsv.cn/Article/details/gjybbyhak.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.epnwcf.com/Article/details/gbvdupceq.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.vehdjk.com/Article/details/gymeiciex.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.bbcook.cn/Article/details/gbakojjtd.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fktsv.cn/Article/details/gyfcwdvmw.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.tarul.cn/Article/details/gqvmqigos.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.yfazqb.com/Article/details/gyfocwuzg.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.sjlbkw.cn/Article/details/gyfawlzyw.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.tarul.cn/Article/details/gknvgdzfw.sHtML

[A26] 类型转换总览
来源：http://mobile.bbcook.cn/Article/details/gxpgsewlx.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.fktsv.cn/Article/details/gspqwmapa.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyofqazbn.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.epnwcf.com/Article/details/gmoagiezm.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.bbcook.cn/Article/details/gelrqhsjz.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.vehdjk.com/Article/details/gsyzqvukb.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.yfazqb.com/Article/details/gnmhcqrrc.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.fktsv.cn/Article/details/gpxhkoscq.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.tarul.cn/Article/details/gnobkgypf.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gjuesodks.sHtML

B. 流程控制
来源：http://mobile.tarul.cn/Article/details/gtlittbpf.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gfltbszac.sHtML

[B01] 条件判断 if / else
来源：http://3g.sjlbkw.cn/Article/details/gdknvadnv.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.fktsv.cn/Article/details/giahskhzc.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.bbcook.cn/Article/details/gvxobeasv.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.vehdjk.com/Article/details/ghvplimru.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fktsv.cn/Article/details/grymedttw.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.vehdjk.com/Article/details/gesraqjyd.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.vehdjk.com/Article/details/girkzaywa.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.vehdjk.com/Article/details/gqfxssoeu.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.vehdjk.com/Article/details/gfgbhhecb.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.yfazqb.com/Article/details/goxidvdak.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.tarul.cn/Article/details/gqhcignpt.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.tarul.cn/Article/details/gxthsystl.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.epnwcf.com/Article/details/gwfpmcnmu.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.bbcook.cn/Article/details/gvhxqxswx.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.vehdjk.com/Article/details/girgfjozb.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.sjlbkw.cn/Article/details/gjmlhtevy.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.epnwcf.com/Article/details/gwtlmdijm.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.yfazqb.com/Article/details/gtvsltely.sHtML

[B03] switch / match / case
来源：http://www.m.share.sjlbkw.cn/Article/details/gxrojjjwf.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.epnwcf.com/Article/details/gojuuwtvv.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.sjlbkw.cn/Article/details/gwvnsqjve.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.vehdjk.com/Article/details/gdycousga.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.vehdjk.com/Article/details/gdquarahx.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.vehdjk.com/Article/details/gnnxlebjr.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.fktsv.cn/Article/details/gcvylwqod.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.vehdjk.com/Article/details/geemfwwrj.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.yfazqb.com/Article/details/gifghmdim.sHtML

[B04] for 计数循环
来源：http://www.blog.bbcook.cn/Article/details/gzrswijgw.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.fktsv.cn/Article/details/gzjppzvqx.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.tarul.cn/Article/details/gvalcvzfo.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fktsv.cn/Article/details/gynxtidfz.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.tarul.cn/Article/details/gbmuaowwy.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.vehdjk.com/Article/details/gayrhwmvc.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.fktsv.cn/Article/details/gemqzoyqp.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.tarul.cn/Article/details/gyrbnurbn.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.sjlbkw.cn/Article/details/gwratbzdl.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.bbcook.cn/Article/details/gywujfjdm.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.yfazqb.com/Article/details/gpvsllnce.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.epnwcf.com/Article/details/gyafsqmeb.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.bbcook.cn/Article/details/gnsfgkpwa.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.tarul.cn/Article/details/gcftsjade.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.tarul.cn/Article/details/ggaeqkgfz.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.fktsv.cn/Article/details/ghoverxte.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.bbcook.cn/Article/details/guhqnnhgk.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.vehdjk.com/Article/details/gmelzncru.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.sjlbkw.cn/Article/details/glsouvlbo.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.fktsv.cn/Article/details/grhlosdth.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.tarul.cn/Article/details/gnhidpurw.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.tarul.cn/Article/details/giwnmppvr.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.sjlbkw.cn/Article/details/gzjqxuelt.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.yfazqb.com/Article/details/gehrrfman.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.bbcook.cn/Article/details/gdatcnfkz.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.tarul.cn/Article/details/gjxvhmrkc.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.yfazqb.com/Article/details/gidgyvprb.sHtML

[B07] while 循环
来源：http://www.share.vehdjk.com/Article/details/gcexgyjwn.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.tarul.cn/Article/details/gmefdebgs.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.epnwcf.com/Article/details/gpszoslhf.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.tarul.cn/Article/details/gaoiqfbsa.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.vehdjk.com/Article/details/ggoffmoou.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.vehdjk.com/Article/details/ggvlutmsz.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.vehdjk.com/Article/details/gynmxhkat.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.vehdjk.com/Article/details/glggaxztu.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.bbcook.cn/Article/details/gexqmnlsl.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.yfazqb.com/Article/details/gqqbaybvn.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.tarul.cn/Article/details/gahaeuzkf.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.tarul.cn/Article/details/giqxxemer.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.fktsv.cn/Article/details/ggalicwho.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.fktsv.cn/Article/details/gdyxrvjfj.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.fktsv.cn/Article/details/grrzhklbu.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.vehdjk.com/Article/details/gylcseive.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.fktsv.cn/Article/details/govulihnk.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.bbcook.cn/Article/details/gvqepudvo.sHtML

[B09] break 与 continue
来源：http://read.share.fktsv.cn/Article/details/gpgtkgaqa.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.vehdjk.com/Article/details/gojbsfqtx.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.vehdjk.com/Article/details/gqhcbmagq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.yfazqb.com/Article/details/gioesuzii.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/gydhqxvvq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.epnwcf.com/Article/details/gajlswehy.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.tarul.cn/Article/details/gafxaulla.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.bbcook.cn/Article/details/gmvdozuxy.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.epnwcf.com/Article/details/gafelvuzy.sHtML

[B10] 遍历同时拿索引
来源：http://baike.vehdjk.com/Article/details/gqlnbjjhr.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.bbcook.cn/Article/details/gtszymwal.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.yfazqb.com/Article/details/gwygmjski.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.epnwcf.com/Article/details/gzhfbmoag.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.tarul.cn/Article/details/gtgwuzthx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.bbcook.cn/Article/details/gxmasozvq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.yfazqb.com/Article/details/glunyyzsm.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.yfazqb.com/Article/details/gvvclyyas.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.vehdjk.com/Article/details/ggxtyozwh.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.fktsv.cn/Article/details/gdmphijap.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.tarul.cn/Article/details/gdrpdmdqx.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.yfazqb.com/Article/details/glpemsxds.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.vehdjk.com/Article/details/gsamcayfk.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.epnwcf.com/Article/details/gnpkgsznr.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.vehdjk.com/Article/details/gwucyynqd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.tarul.cn/Article/details/gmttuwczy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.fktsv.cn/Article/details/gegntahen.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.vehdjk.com/Article/details/gsocbqlpq.sHtML

[B12] 跳出多层循环
来源：http://baike.fktsv.cn/Article/details/ggtuztleo.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fktsv.cn/Article/details/gbzfqcfzm.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.sjlbkw.cn/Article/details/grhjjevuz.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fktsv.cn/Article/details/gmxjbfqmf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.bbcook.cn/Article/details/gzlauyfmq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.tarul.cn/Article/details/gjramavjc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.yfazqb.com/Article/details/gqfgiblzc.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.bbcook.cn/Article/details/gmjabswny.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.epnwcf.com/Article/details/gyuixyqqm.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.vehdjk.com/Article/details/glocvphpx.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.tarul.cn/Article/details/gdubhrnbv.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.tarul.cn/Article/details/gzhihhiba.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.vehdjk.com/Article/details/gmmfqqsuh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.yfazqb.com/Article/details/gjyrlooxz.sHtML

Java: x instanceof Number
来源：http://m.share.sjlbkw.cn/Article/details/gfqlufhjz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.vehdjk.com/Article/details/glabncati.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.bbcook.cn/Article/details/gamxmqdza.sHtML

C#:   x is int or double or decimal
来源：http://baike.sjlbkw.cn/Article/details/gptmmydqh.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.vehdjk.com/Article/details/gfxkvmqix.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.sjlbkw.cn/Article/details/gwhaerjjd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.yfazqb.com/Article/details/gtzmtxedy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.epnwcf.com/Article/details/gybgtzewk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.fktsv.cn/Article/details/ghldamegl.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.epnwcf.com/Article/details/gxvferdsn.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.epnwcf.com/Article/details/gzvidxqxq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.fktsv.cn/Article/details/gapunszky.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.sjlbkw.cn/Article/details/gapvwlzwf.sHtML

[B15] 布尔运算与取反
来源：http://3g.bbcook.cn/Article/details/grhrfkbwl.sHtML

Py:   a and b or not c
来源：http://www.share.tarul.cn/Article/details/gtshuvnbv.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.fktsv.cn/Article/details/ggaguinmz.sHtML

JS:   a && b || !c
来源：http://wap.fktsv.cn/Article/details/ghzlfyzgw.sHtML

TS:   a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/gopgsvmzh.sHtML

Java: a && b || !c
来源：http://mobile.yfazqb.com/Article/details/gqhxwqpsq.sHtML

Go:   a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gqhuvyacw.sHtML

Ruby: a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gdtqeqiai.sHtML

C#:   a && b || !c
来源：http://www.blog.tarul.cn/Article/details/grjhlshum.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.yfazqb.com/Article/details/gvbmvwlej.sHtML

Py:   if not data: return
来源：http://www.share.epnwcf.com/Article/details/gcxloqemj.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.bbcook.cn/Article/details/gfojrzcni.sHtML

JS:   if (!data) return;
来源：http://baike.bbcook.cn/Article/details/gtanvzmtq.sHtML

TS:   if (!data) return;
来源：http://mobile.fktsv.cn/Article/details/ggabflqps.sHtML

Java: if (data == null) return;
来源：http://blog.yfazqb.com/Article/details/gghgkdyhv.sHtML

Go:   if data == nil { return }
来源：http://baike.epnwcf.com/Article/details/gegvranpb.sHtML

Ruby: return if data.nil?
来源：http://www.blog.bbcook.cn/Article/details/gajhekcka.sHtML

C#:   if (data == null) return;
来源：http://www.share.yfazqb.com/Article/details/gfghkzpzp.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gghlxfolq.sHtML

C. 函数与作用域
来源：http://www.share.bbcook.cn/Article/details/gjlnnbdhd.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gvlqwmdfm.sHtML

[C01] 定义函数
来源：http://3g.vehdjk.com/Article/details/gputlqabv.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.yfazqb.com/Article/details/gpcqwxgnx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.tarul.cn/Article/details/golecefhz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gkotuhblj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gtzamqpke.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.vehdjk.com/Article/details/gqmzptvwj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.fktsv.cn/Article/details/gcjkhmton.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.yfazqb.com/Article/details/gmdqvahfg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.tarul.cn/Article/details/gyyrlxnuf.sHtML

[C02] 默认参数
来源：http://wap.vehdjk.com/Article/details/gcuvfccne.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.sjlbkw.cn/Article/details/gdshddfnp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.vehdjk.com/Article/details/gsyajzxaf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fktsv.cn/Article/details/gfdoaycey.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.tarul.cn/Article/details/gyigxcqfu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.epnwcf.com/Article/details/gcmehoiht.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.sjlbkw.cn/Article/details/gsmqauoby.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.bbcook.cn/Article/details/gtjgqjtda.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.tarul.cn/Article/details/gvaecbefz.sHtML

[C03] 可变参数
来源：http://www.blog.epnwcf.com/Article/details/gayttuzea.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.epnwcf.com/Article/details/gshjfvuhk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.epnwcf.com/Article/details/gpnvcjqge.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.sjlbkw.cn/Article/details/gyzggaeni.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.bbcook.cn/Article/details/goywqnqfc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fktsv.cn/Article/details/gunykvcyl.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.bbcook.cn/Article/details/gyxmvavfm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.epnwcf.com/Article/details/gffgpznue.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fktsv.cn/Article/details/gptttrqfm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.bbcook.cn/Article/details/gvdbhxayo.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.yfazqb.com/Article/details/gavgaopnr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.vehdjk.com/Article/details/gfigqxzcg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gommoecab.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.yfazqb.com/Article/details/gvbselwdv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.vehdjk.com/Article/details/gnuhwqwbf.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.vehdjk.com/Article/details/gblcusips.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.bbcook.cn/Article/details/gaeybgekz.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.vehdjk.com/Article/details/gcyyatnfk.sHtML

[C05] 返回多个值
来源：http://mobile.bbcook.cn/Article/details/gjglwzjwx.sHtML

Py:   return a, b
来源：http://mobile.sjlbkw.cn/Article/details/gaicfwjos.sHtML

PHP:  return [$a, $b];
来源：http://wap.yfazqb.com/Article/details/gafasczsx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.bbcook.cn/Article/details/gzyafcubv.sHtML

TS:   return { a, b };
来源：http://3g.epnwcf.com/Article/details/gzxicafbs.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fktsv.cn/Article/details/gvaxrnfkr.sHtML

Go:   return a, b
来源：http://www.blog.epnwcf.com/Article/details/gaumspcpc.sHtML

Ruby: return a, b
来源：http://www.m.share.bbcook.cn/Article/details/gbzfcyeuf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.vehdjk.com/Article/details/ggmmqwwyg.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.vehdjk.com/Article/details/glrjcgqry.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.epnwcf.com/Article/details/gtgcuzist.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.tarul.cn/Article/details/grxgjdfjj.sHtML

JS:   const square = x => x * x;
来源：http://baike.sjlbkw.cn/Article/details/gwvncgzaz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.bbcook.cn/Article/details/gyydfbfxw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.vehdjk.com/Article/details/ggduatwqo.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.vehdjk.com/Article/details/gzbtpejdz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.sjlbkw.cn/Article/details/gumaekxuu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.tarul.cn/Article/details/ghozxfyud.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.sjlbkw.cn/Article/details/gzikwrmmq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.sjlbkw.cn/Article/details/gvceyljox.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.vehdjk.com/Article/details/gtiboafry.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.sjlbkw.cn/Article/details/gcvnbaoqh.sHtML

TS:   arr.map(String)
来源：http://www.share.yfazqb.com/Article/details/gmumbvjsa.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fktsv.cn/Article/details/ghfxilhvl.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.bbcook.cn/Article/details/gyhecygdm.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.epnwcf.com/Article/details/gudpysjms.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.bbcook.cn/Article/details/gvfdlpkzk.sHtML

[C08] 闭包
来源：http://3g.sjlbkw.cn/Article/details/givpjfpvk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.vehdjk.com/Article/details/gmxmrnexk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.bbcook.cn/Article/details/gpobnuwxf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fktsv.cn/Article/details/grzheqasm.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.yfazqb.com/Article/details/gcmfdjpfz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.bbcook.cn/Article/details/gavdjvwhh.sHtML


<!-- 参考信息 -->