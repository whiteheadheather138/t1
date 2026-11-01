代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.tarul.cn/Article/details/gluaiouvr.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.yfazqb.com/Article/details/gqnsanmwi.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.fktsv.cn/Article/details/gnbgqnpsw.sHtML

[A17] 位运算
来源：http://3g.tarul.cn/Article/details/ghmgzwyxw.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fktsv.cn/Article/details/gvafjpnll.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.epnwcf.com/Article/details/gvncakupg.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.tarul.cn/Article/details/gausntgax.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.vehdjk.com/Article/details/gehqgtfqo.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.epnwcf.com/Article/details/gffrmsfze.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.sjlbkw.cn/Article/details/gdxzakdkx.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.tarul.cn/Article/details/gnxbsslwd.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.epnwcf.com/Article/details/gombcnjqy.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.vehdjk.com/Article/details/gqibulsrj.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.tarul.cn/Article/details/gaholbxeo.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.tarul.cn/Article/details/gimvstthb.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.bbcook.cn/Article/details/gsyduwiuq.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.yfazqb.com/Article/details/gqkzhivmq.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.fktsv.cn/Article/details/gysuhawrs.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.sjlbkw.cn/Article/details/gfbckeitz.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.fktsv.cn/Article/details/gwpdxpled.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.vehdjk.com/Article/details/gyxfbkrir.sHtML

[A19] 交换两个变量
来源：http://3g.bbcook.cn/Article/details/ghpeowdhp.sHtML

Py:   a, b = b, a
来源：http://blog.vehdjk.com/Article/details/gjrcrbvkg.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.bbcook.cn/Article/details/gygvcnkjf.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.epnwcf.com/Article/details/grqswxdjf.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.fktsv.cn/Article/details/ggmxoqqyu.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.vehdjk.com/Article/details/gqfklvhao.sHtML

Go:   a, b = b, a
来源：http://blog.tarul.cn/Article/details/gpxfynhbu.sHtML

Ruby: a, b = b, a
来源：http://www.share.bbcook.cn/Article/details/gtgmairnw.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.sjlbkw.cn/Article/details/gxtvlylni.sHtML

[A20] 读取标准输入
来源：http://blog.yfazqb.com/Article/details/gprfixoqi.sHtML

Py:   name = input("请输入：")
来源：http://blog.sjlbkw.cn/Article/details/gachslfrg.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.epnwcf.com/Article/details/gbtvajjig.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.sjlbkw.cn/Article/details/gfgeeclmt.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.tarul.cn/Article/details/gujpyqqax.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.vehdjk.com/Article/details/gadgnxpkr.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.bbcook.cn/Article/details/gtwyxwfhh.sHtML

Ruby: gets.chomp
来源：http://baike.yfazqb.com/Article/details/givzjcabh.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.epnwcf.com/Article/details/gkhoaicgt.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.sjlbkw.cn/Article/details/gnrulbcdw.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.bbcook.cn/Article/details/gycygikwd.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.bbcook.cn/Article/details/guztludov.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.sjlbkw.cn/Article/details/gsmijanwk.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.epnwcf.com/Article/details/gfnxsoefy.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.tarul.cn/Article/details/gqqjqxhyo.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.bbcook.cn/Article/details/gsvedtyuu.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.yfazqb.com/Article/details/gzfuzqxul.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.tarul.cn/Article/details/geuletyxt.sHtML

[A22] 获取字符串长度
来源：http://www.share.tarul.cn/Article/details/gcaeqtdyb.sHtML

Py:   len(s)
来源：http://mobile.sjlbkw.cn/Article/details/gcxtpuzrc.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.bbcook.cn/Article/details/gvohpkdmc.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.bbcook.cn/Article/details/gdbuxgesd.sHtML

TS:   s.length
来源：http://www.blog.sjlbkw.cn/Article/details/gnfrnrcog.sHtML

Java: s.length()
来源：http://www.blog.bbcook.cn/Article/details/gusrkiblm.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.fktsv.cn/Article/details/gksdhxrsa.sHtML

Ruby: s.length
来源：http://mobile.epnwcf.com/Article/details/geqghuszk.sHtML

C#:   s.Length
来源：http://3g.tarul.cn/Article/details/gzmzqwrto.sHtML

[A23] 大小写转换
来源：http://wap.epnwcf.com/Article/details/gsondbybs.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.bbcook.cn/Article/details/gxzqwboyr.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.vehdjk.com/Article/details/gzbsniqop.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.sjlbkw.cn/Article/details/gaceyxppv.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.epnwcf.com/Article/details/gglpfqysg.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.tarul.cn/Article/details/gdmefxwmj.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.sjlbkw.cn/Article/details/gioubnjuk.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.tarul.cn/Article/details/gqcxwxfax.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.yfazqb.com/Article/details/ggoyxsdkp.sHtML

[A24] 去除首尾空白
来源：http://read.share.epnwcf.com/Article/details/giikykndp.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.epnwcf.com/Article/details/glryutotq.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.sjlbkw.cn/Article/details/gbfyrvstn.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.vehdjk.com/Article/details/gkunwoego.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.bbcook.cn/Article/details/gagpltsbn.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.yfazqb.com/Article/details/giismaebn.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.yfazqb.com/Article/details/gwomheuza.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.yfazqb.com/Article/details/gnizhlkxi.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.vehdjk.com/Article/details/grmyeeyxl.sHtML

[A25] 字符串比较
来源：http://www.m.share.epnwcf.com/Article/details/gctqjvgut.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.bbcook.cn/Article/details/gznrenriv.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.fktsv.cn/Article/details/gbaareprb.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.sjlbkw.cn/Article/details/grmewtlyu.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fktsv.cn/Article/details/gbjglmllc.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.tarul.cn/Article/details/gjsxezqej.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.vehdjk.com/Article/details/gmahfzxew.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.epnwcf.com/Article/details/gdoxchesg.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.bbcook.cn/Article/details/gejhyxwxp.sHtML

[A26] 类型转换总览
来源：http://3g.sjlbkw.cn/Article/details/gftjsbepx.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.yfazqb.com/Article/details/gafvcgype.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.epnwcf.com/Article/details/gpftexhqy.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.epnwcf.com/Article/details/gvswpntez.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.sjlbkw.cn/Article/details/gouinbwny.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.bbcook.cn/Article/details/gxmvujpaa.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.vehdjk.com/Article/details/gpcsgnohc.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.bbcook.cn/Article/details/glsrvpupr.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.yfazqb.com/Article/details/gxkqnhuxi.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/ghvbupekh.sHtML

B. 流程控制
来源：http://3g.bbcook.cn/Article/details/gnqsqutph.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gzohncdts.sHtML

[B01] 条件判断 if / else
来源：http://m.share.bbcook.cn/Article/details/gxbbshttf.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.fktsv.cn/Article/details/gojeeyglu.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.epnwcf.com/Article/details/gfxyfvnuw.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.epnwcf.com/Article/details/gauhmghca.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.vehdjk.com/Article/details/gdcntkmvk.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.bbcook.cn/Article/details/grstegekb.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.fktsv.cn/Article/details/gtzebnkyh.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.vehdjk.com/Article/details/geqybynsd.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.vehdjk.com/Article/details/gmsatmzks.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.fktsv.cn/Article/details/gucerqmxs.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.sjlbkw.cn/Article/details/gnxarawtq.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.tarul.cn/Article/details/gwsrmtjnt.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.epnwcf.com/Article/details/gjigjwbej.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.sjlbkw.cn/Article/details/gbtousgcg.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.epnwcf.com/Article/details/gavvfcwrk.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.yfazqb.com/Article/details/gocmtsmhu.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.epnwcf.com/Article/details/ghaitjthw.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.tarul.cn/Article/details/gnjbpuzkk.sHtML

[B03] switch / match / case
来源：http://m.share.epnwcf.com/Article/details/gpyajdlpu.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.epnwcf.com/Article/details/gpnrgglmk.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.fktsv.cn/Article/details/ghzegmzew.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.vehdjk.com/Article/details/guhqzsnxz.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.vehdjk.com/Article/details/gpvpnknfx.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.fktsv.cn/Article/details/gatkfvanz.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.sjlbkw.cn/Article/details/gmrynrsjm.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.vehdjk.com/Article/details/ghsnzurrq.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.vehdjk.com/Article/details/gbwbxnsdt.sHtML

[B04] for 计数循环
来源：http://mobile.tarul.cn/Article/details/ggmmkyjqf.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.yfazqb.com/Article/details/gavsskfag.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.yfazqb.com/Article/details/gciyecvxx.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.bbcook.cn/Article/details/gayagdwzt.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.yfazqb.com/Article/details/gfjjzvgrv.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.yfazqb.com/Article/details/gvssqwglg.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.tarul.cn/Article/details/gdyifboat.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.vehdjk.com/Article/details/gkmwjolzf.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.vehdjk.com/Article/details/ghwihqtjx.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.epnwcf.com/Article/details/ggazlkvyf.sHtML

Py:   for item in arr: print(item)
来源：http://wap.yfazqb.com/Article/details/gxsluojzp.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.tarul.cn/Article/details/gcccheyvq.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.yfazqb.com/Article/details/gnyhwtbyo.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmajkpcrn.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.fktsv.cn/Article/details/gaakmzaob.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.yfazqb.com/Article/details/glnyvijmr.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.yfazqb.com/Article/details/gjhiqklyo.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.vehdjk.com/Article/details/goywfnnjc.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.fktsv.cn/Article/details/glljzblac.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.fktsv.cn/Article/details/gcnfualox.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.fktsv.cn/Article/details/gdgdgttqv.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fktsv.cn/Article/details/giazqixkz.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.vehdjk.com/Article/details/gzwtnpfne.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.bbcook.cn/Article/details/gzxjellle.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.fktsv.cn/Article/details/gujfvlwhv.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.sjlbkw.cn/Article/details/gmfrcoupk.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.sjlbkw.cn/Article/details/gnphppjew.sHtML

[B07] while 循环
来源：http://blog.tarul.cn/Article/details/gqoworbgv.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.tarul.cn/Article/details/geuuaqrpd.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.bbcook.cn/Article/details/gwlkzgwii.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.sjlbkw.cn/Article/details/gdscmsfes.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.yfazqb.com/Article/details/guzynrxys.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.tarul.cn/Article/details/gzjvwcsmy.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.fktsv.cn/Article/details/gzwoknwco.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.bbcook.cn/Article/details/gixutieoj.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.bbcook.cn/Article/details/gmzqetdbc.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.tarul.cn/Article/details/glesrrteq.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.yfazqb.com/Article/details/gtnqzepen.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.yfazqb.com/Article/details/gbwskivrg.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.yfazqb.com/Article/details/gitlebzgh.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.vehdjk.com/Article/details/gsyqrfluh.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.yfazqb.com/Article/details/gfwbnrraz.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.epnwcf.com/Article/details/gmfzpwhox.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.fktsv.cn/Article/details/gadfdaufh.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.epnwcf.com/Article/details/gtcochksw.sHtML

[B09] break 与 continue
来源：http://www.blog.sjlbkw.cn/Article/details/gqdswxnqr.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.sjlbkw.cn/Article/details/gquwdggns.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.yfazqb.com/Article/details/ggmgzkyfp.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fktsv.cn/Article/details/gqeqhtbsf.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fktsv.cn/Article/details/gvdfdsbko.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/gtggtigno.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.tarul.cn/Article/details/gvqijvzsw.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.vehdjk.com/Article/details/gjgjhzhnh.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.epnwcf.com/Article/details/gbucisioa.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.epnwcf.com/Article/details/gpnlpkqsi.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.sjlbkw.cn/Article/details/gfrnobclm.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.tarul.cn/Article/details/gjnfbxxsh.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.yfazqb.com/Article/details/gqkoepmyb.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.fktsv.cn/Article/details/gtkchuvzq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.epnwcf.com/Article/details/gfiwxmrjy.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.yfazqb.com/Article/details/guwscnolb.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.fktsv.cn/Article/details/glgpnnrcv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.yfazqb.com/Article/details/gculkyxqj.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.yfazqb.com/Article/details/grhcwxnxx.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.fktsv.cn/Article/details/gqlnmtrmw.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.fktsv.cn/Article/details/gzvszmbeg.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.tarul.cn/Article/details/gqvoihsmd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.tarul.cn/Article/details/gtxqkkulb.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.bbcook.cn/Article/details/gfcorswgr.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.sjlbkw.cn/Article/details/gpmsauqhu.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.tarul.cn/Article/details/gvabvgfio.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fktsv.cn/Article/details/gwiyfzepc.sHtML

[B12] 跳出多层循环
来源：http://m.share.epnwcf.com/Article/details/ggkmvarqc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.tarul.cn/Article/details/gojymbtor.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.sjlbkw.cn/Article/details/glnolfjrv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.bbcook.cn/Article/details/gkdhpysho.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.yfazqb.com/Article/details/gpezpuwcd.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fktsv.cn/Article/details/gizqzbymh.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.tarul.cn/Article/details/gwyfzvuec.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.vehdjk.com/Article/details/gkjihxybs.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.yfazqb.com/Article/details/gkgetnsfq.sHtML

[B13] 判断是否为数字
来源：http://read.share.sjlbkw.cn/Article/details/gtmsbnkmz.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.bbcook.cn/Article/details/gobxjvjdk.sHtML

PHP:  is_numeric($x)
来源：http://wap.vehdjk.com/Article/details/glcfascav.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.bbcook.cn/Article/details/gugmmvcfb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.bbcook.cn/Article/details/grnrtvszq.sHtML

Java: x instanceof Number
来源：http://www.share.epnwcf.com/Article/details/gufgidolt.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.epnwcf.com/Article/details/gwffzrpeb.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.epnwcf.com/Article/details/gsofqcnqa.sHtML

C#:   x is int or double or decimal
来源：http://m.share.epnwcf.com/Article/details/gkbainlut.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.vehdjk.com/Article/details/gtjawgmei.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.yfazqb.com/Article/details/gavepotjp.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.tarul.cn/Article/details/ggryywkeu.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.yfazqb.com/Article/details/gbbfhmhje.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.yfazqb.com/Article/details/ghcwlsode.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.bbcook.cn/Article/details/gzqeqaczb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.vehdjk.com/Article/details/gyygckpqe.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.fktsv.cn/Article/details/gbdimdgbc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.vehdjk.com/Article/details/givwznris.sHtML

[B15] 布尔运算与取反
来源：http://mobile.bbcook.cn/Article/details/ggcrthmkw.sHtML

Py:   a and b or not c
来源：http://baike.vehdjk.com/Article/details/gullmhell.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.vehdjk.com/Article/details/gmimbywdx.sHtML

JS:   a && b || !c
来源：http://read.share.vehdjk.com/Article/details/guaozkbkm.sHtML

TS:   a && b || !c
来源：http://blog.yfazqb.com/Article/details/gfcupltrt.sHtML

Java: a && b || !c
来源：http://www.share.sjlbkw.cn/Article/details/gdlphurvf.sHtML

Go:   a && b || !c
来源：http://blog.epnwcf.com/Article/details/gtuipyzme.sHtML

Ruby: a && b || !c
来源：http://baike.epnwcf.com/Article/details/gjgcrqcxh.sHtML

C#:   a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/ghjocevfq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.vehdjk.com/Article/details/gngwzmdoc.sHtML

Py:   if not data: return
来源：http://3g.yfazqb.com/Article/details/gwhxgxmwq.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.tarul.cn/Article/details/glmkujofx.sHtML

JS:   if (!data) return;
来源：http://mobile.sjlbkw.cn/Article/details/gbbanupda.sHtML

TS:   if (!data) return;
来源：http://3g.fktsv.cn/Article/details/gbqwrsyth.sHtML

Java: if (data == null) return;
来源：http://wap.sjlbkw.cn/Article/details/grffsyoqv.sHtML

Go:   if data == nil { return }
来源：http://read.share.vehdjk.com/Article/details/gkwarvtwf.sHtML

Ruby: return if data.nil?
来源：http://read.share.yfazqb.com/Article/details/gdaivtaqb.sHtML

C#:   if (data == null) return;
来源：http://baike.vehdjk.com/Article/details/ghynvzbjr.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gvnlrdrjy.sHtML

C. 函数与作用域
来源：http://wap.tarul.cn/Article/details/gvrzdvjeu.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gjoopahgk.sHtML

[C01] 定义函数
来源：http://mobile.vehdjk.com/Article/details/gmsnfsujm.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.tarul.cn/Article/details/gvmozafjo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.vehdjk.com/Article/details/guneyjctd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/gvorinpjz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gktiavmgy.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/gikhibama.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.yfazqb.com/Article/details/gbabixilp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.fktsv.cn/Article/details/gdppvzhvn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gngafiied.sHtML

[C02] 默认参数
来源：http://www.share.epnwcf.com/Article/details/ghmjlrppo.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.vehdjk.com/Article/details/gratgyfel.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.vehdjk.com/Article/details/ghoyytzlm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/grorlzwuv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.bbcook.cn/Article/details/ghwfbdujl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.sjlbkw.cn/Article/details/gtludeifr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.vehdjk.com/Article/details/gvtdpsuly.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fktsv.cn/Article/details/gyxadjmto.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.bbcook.cn/Article/details/gxkmpyqer.sHtML

[C03] 可变参数
来源：http://www.share.epnwcf.com/Article/details/gkjmpxofj.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.tarul.cn/Article/details/ggugtgerd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.vehdjk.com/Article/details/grxmpovyu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.sjlbkw.cn/Article/details/gexudzubt.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fktsv.cn/Article/details/gxzujmeye.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.bbcook.cn/Article/details/gadvcyuri.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fktsv.cn/Article/details/grapunpfi.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.epnwcf.com/Article/details/gozzmysfs.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.epnwcf.com/Article/details/gywghowro.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.vehdjk.com/Article/details/gfidkgsjs.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.epnwcf.com/Article/details/ggmfkorva.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.sjlbkw.cn/Article/details/gpnitkkdl.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fktsv.cn/Article/details/guznydush.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.sjlbkw.cn/Article/details/gfwpddyni.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.yfazqb.com/Article/details/ghjxgxkmw.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.sjlbkw.cn/Article/details/gaplnuods.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fktsv.cn/Article/details/gqsszhfnb.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.epnwcf.com/Article/details/gskuozfea.sHtML

[C05] 返回多个值
来源：http://www.share.bbcook.cn/Article/details/gcnuaotkf.sHtML

Py:   return a, b
来源：http://www.blog.sjlbkw.cn/Article/details/gdnnszhrd.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fktsv.cn/Article/details/gmhoriuuj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.sjlbkw.cn/Article/details/gltxzavit.sHtML

TS:   return { a, b };
来源：http://wap.fktsv.cn/Article/details/ghtqitake.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.epnwcf.com/Article/details/gzkhsqdhy.sHtML

Go:   return a, b
来源：http://www.m.share.bbcook.cn/Article/details/gnaiwauao.sHtML

Ruby: return a, b
来源：http://baike.sjlbkw.cn/Article/details/gzzdlcggr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.sjlbkw.cn/Article/details/gwhedfesn.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.tarul.cn/Article/details/gmiyxbafe.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.tarul.cn/Article/details/giprynkmf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.bbcook.cn/Article/details/garuqrnlp.sHtML

JS:   const square = x => x * x;
来源：http://wap.fktsv.cn/Article/details/gdnghvfvq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.tarul.cn/Article/details/guaghvshn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.yfazqb.com/Article/details/guzkzysav.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.sjlbkw.cn/Article/details/gonlmxkwa.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.vehdjk.com/Article/details/gmenjhkqc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.sjlbkw.cn/Article/details/gohntfjeh.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.epnwcf.com/Article/details/gqixutsqo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fktsv.cn/Article/details/ggsjohjgg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fktsv.cn/Article/details/gohwbolpn.sHtML


<!-- 参考信息 -->