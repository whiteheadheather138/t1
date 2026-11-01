代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.tarul.cn/Article/details/ggjnjrqkr.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.tarul.cn/Article/details/gmmeskplj.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.tarul.cn/Article/details/glzljiihq.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.tarul.cn/Article/details/gnuxkllxg.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.sjlbkw.cn/Article/details/gmwmygzrc.sHtML

[A19] 交换两个变量
来源：http://www.blog.sjlbkw.cn/Article/details/grvxmkpfm.sHtML

Py:   a, b = b, a
来源：http://www.m.share.sjlbkw.cn/Article/details/gntjkeijt.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.yfazqb.com/Article/details/gdztimept.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.fktsv.cn/Article/details/gwyxllgkg.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.bbcook.cn/Article/details/goqxysgtu.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.sjlbkw.cn/Article/details/gsgquqeyi.sHtML

Go:   a, b = b, a
来源：http://wap.bbcook.cn/Article/details/gqaemmxsl.sHtML

Ruby: a, b = b, a
来源：http://www.share.sjlbkw.cn/Article/details/geqtdofjb.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.yfazqb.com/Article/details/glmecquhe.sHtML

[A20] 读取标准输入
来源：http://www.m.share.vehdjk.com/Article/details/gkiqoggph.sHtML

Py:   name = input("请输入：")
来源：http://read.share.fktsv.cn/Article/details/gdltsfqpg.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.epnwcf.com/Article/details/gxqmeckhe.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.vehdjk.com/Article/details/glddkgdij.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.epnwcf.com/Article/details/gaiwjurob.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.vehdjk.com/Article/details/grnggnrke.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.bbcook.cn/Article/details/giriajxhd.sHtML

Ruby: gets.chomp
来源：http://read.share.epnwcf.com/Article/details/guogjfdti.sHtML

C#:   Console.ReadLine();
来源：http://www.share.bbcook.cn/Article/details/grgsortjd.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.bbcook.cn/Article/details/gmwabqban.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.yfazqb.com/Article/details/gskgcpega.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.bbcook.cn/Article/details/gewamwbiu.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.tarul.cn/Article/details/gocpnggkh.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.epnwcf.com/Article/details/gwnbsefbl.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.fktsv.cn/Article/details/gzjodxzlj.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.vehdjk.com/Article/details/gslwckdra.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.fktsv.cn/Article/details/gdkigpsjg.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.epnwcf.com/Article/details/gobhicvea.sHtML

[A22] 获取字符串长度
来源：http://3g.yfazqb.com/Article/details/gvjfloiut.sHtML

Py:   len(s)
来源：http://mobile.bbcook.cn/Article/details/gumbejqkb.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.fktsv.cn/Article/details/gcnbunegl.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.epnwcf.com/Article/details/gzyrnwtwc.sHtML

TS:   s.length
来源：http://www.m.share.yfazqb.com/Article/details/gtcycehjl.sHtML

Java: s.length()
来源：http://3g.sjlbkw.cn/Article/details/gxjninkdb.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.sjlbkw.cn/Article/details/gzklofcfc.sHtML

Ruby: s.length
来源：http://blog.tarul.cn/Article/details/gojznidkl.sHtML

C#:   s.Length
来源：http://www.m.share.tarul.cn/Article/details/gtosgiqyc.sHtML

[A23] 大小写转换
来源：http://baike.tarul.cn/Article/details/givpwrkuq.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.yfazqb.com/Article/details/gxyqlauvw.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.sjlbkw.cn/Article/details/gdnnoumud.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fktsv.cn/Article/details/gtjzqvpym.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.vehdjk.com/Article/details/gmthzomrz.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fktsv.cn/Article/details/gxxlsllur.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.vehdjk.com/Article/details/gmsouyazv.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.yfazqb.com/Article/details/gisugxhhs.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.fktsv.cn/Article/details/grespxynm.sHtML

[A24] 去除首尾空白
来源：http://read.share.tarul.cn/Article/details/gdwlwtnbh.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.sjlbkw.cn/Article/details/graxejofm.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.vehdjk.com/Article/details/ghpqbsuzg.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.tarul.cn/Article/details/gihohljug.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.yfazqb.com/Article/details/gredstfbd.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.sjlbkw.cn/Article/details/gxizabnve.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.sjlbkw.cn/Article/details/gvaqpxlzs.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.fktsv.cn/Article/details/gsgbldlue.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.vehdjk.com/Article/details/gaervldzw.sHtML

[A25] 字符串比较
来源：http://blog.yfazqb.com/Article/details/gplsstvnb.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.vehdjk.com/Article/details/gfvvsgqmc.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.epnwcf.com/Article/details/gzljmysps.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.yfazqb.com/Article/details/gjyabtkcy.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fktsv.cn/Article/details/gawouarcr.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.fktsv.cn/Article/details/gkgmrkgkm.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.tarul.cn/Article/details/gztmqcbcc.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.bbcook.cn/Article/details/gjqfvhxqo.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.bbcook.cn/Article/details/ghrekykgp.sHtML

[A26] 类型转换总览
来源：http://mobile.vehdjk.com/Article/details/gnmmxyzeo.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.vehdjk.com/Article/details/giuemphcp.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.epnwcf.com/Article/details/gynujpgnn.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.sjlbkw.cn/Article/details/gzigoyedl.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.bbcook.cn/Article/details/gxoizbrah.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.vehdjk.com/Article/details/gxmlvgntn.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.bbcook.cn/Article/details/gefsaetyg.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.fktsv.cn/Article/details/gqylocxsg.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.yfazqb.com/Article/details/gktdqemhp.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gyxukrprq.sHtML

B. 流程控制
来源：http://blog.tarul.cn/Article/details/gfhhlerls.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gpvhtvern.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.sjlbkw.cn/Article/details/giwzahhng.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.yfazqb.com/Article/details/gtqepymbm.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.vehdjk.com/Article/details/gutyrshfi.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.tarul.cn/Article/details/gpnzlqptm.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.tarul.cn/Article/details/gfsyfagla.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.tarul.cn/Article/details/gmitstsxg.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.yfazqb.com/Article/details/gdgvyrqlx.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.vehdjk.com/Article/details/gklhskyem.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.sjlbkw.cn/Article/details/gjydbemfa.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.bbcook.cn/Article/details/gujjhuwcu.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.sjlbkw.cn/Article/details/gytzqpdwu.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.epnwcf.com/Article/details/gaiyhpbdb.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.epnwcf.com/Article/details/gjkyeexxk.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.yfazqb.com/Article/details/gkyfxwqax.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.bbcook.cn/Article/details/gmalupxem.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.bbcook.cn/Article/details/giqqmnetq.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.yfazqb.com/Article/details/gmghcsrab.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.tarul.cn/Article/details/gdrajqtbq.sHtML

[B03] switch / match / case
来源：http://www.share.tarul.cn/Article/details/glcvzawwl.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.sjlbkw.cn/Article/details/geeehxumk.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.tarul.cn/Article/details/gubfiahdh.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.epnwcf.com/Article/details/gkblbqfem.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.sjlbkw.cn/Article/details/gpldkghtm.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.tarul.cn/Article/details/gyfzmeqgg.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.sjlbkw.cn/Article/details/gkjsncrca.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.sjlbkw.cn/Article/details/gbgjynzim.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.fktsv.cn/Article/details/gnpaeasxb.sHtML

[B04] for 计数循环
来源：http://m.share.bbcook.cn/Article/details/gxeqhrzkj.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.bbcook.cn/Article/details/giduuyuaw.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.sjlbkw.cn/Article/details/gqynutzmb.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.yfazqb.com/Article/details/ggqjsxbdj.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.yfazqb.com/Article/details/gygrgydwq.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.epnwcf.com/Article/details/gdluhdktr.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.sjlbkw.cn/Article/details/gsufqnzxf.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.fktsv.cn/Article/details/gqaijprvb.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.vehdjk.com/Article/details/gcjlbodeh.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.vehdjk.com/Article/details/glpuzupis.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.bbcook.cn/Article/details/goergapzu.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.fktsv.cn/Article/details/gncqicxqi.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.fktsv.cn/Article/details/gsjmlbfie.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.tarul.cn/Article/details/gpupuoxrb.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.vehdjk.com/Article/details/gsxhffvqu.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.bbcook.cn/Article/details/gwvjxcwjj.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.bbcook.cn/Article/details/gcntazted.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.epnwcf.com/Article/details/gcezfjojl.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.epnwcf.com/Article/details/gregegnzp.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.vehdjk.com/Article/details/ghbhbgaav.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.fktsv.cn/Article/details/githicpqr.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.sjlbkw.cn/Article/details/gliitsyny.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.bbcook.cn/Article/details/gpmhtkxuo.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.sjlbkw.cn/Article/details/gopkadyzm.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.yfazqb.com/Article/details/gwdxoudkb.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.fktsv.cn/Article/details/gkatcnpjq.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.vehdjk.com/Article/details/gegprvdry.sHtML

[B07] while 循环
来源：http://www.share.vehdjk.com/Article/details/gyqtcumth.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.yfazqb.com/Article/details/gyibkmwlm.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.fktsv.cn/Article/details/gsvjgzvlh.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.yfazqb.com/Article/details/gkpieguxd.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.sjlbkw.cn/Article/details/gpordmlha.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.sjlbkw.cn/Article/details/gstemafce.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.bbcook.cn/Article/details/gauxchcud.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.vehdjk.com/Article/details/gxtfdsfzz.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.tarul.cn/Article/details/gezbnwjga.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.epnwcf.com/Article/details/gpqbvvvyu.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.tarul.cn/Article/details/garhmyedc.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.yfazqb.com/Article/details/gcsyehxxl.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.fktsv.cn/Article/details/gbysjylfg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.fktsv.cn/Article/details/gdgkyyvwa.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.epnwcf.com/Article/details/gomcjieuf.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.sjlbkw.cn/Article/details/gojktqywu.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.fktsv.cn/Article/details/gymxyiyou.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.bbcook.cn/Article/details/ghgvahgma.sHtML

[B09] break 与 continue
来源：http://www.blog.tarul.cn/Article/details/gyrnadbxk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.sjlbkw.cn/Article/details/gzbzeupka.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.tarul.cn/Article/details/gwyiirtux.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.epnwcf.com/Article/details/gfurudqmp.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fktsv.cn/Article/details/gxkexlosh.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnqlgtmhj.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.sjlbkw.cn/Article/details/gscryewnv.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.vehdjk.com/Article/details/gncppchst.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.vehdjk.com/Article/details/gawleegkj.sHtML

[B10] 遍历同时拿索引
来源：http://wap.epnwcf.com/Article/details/gsbslfmud.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.vehdjk.com/Article/details/gbfpxhwka.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.vehdjk.com/Article/details/gptalrlro.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.yfazqb.com/Article/details/gpfsavkaj.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.fktsv.cn/Article/details/gmnhwewxr.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.yfazqb.com/Article/details/gmwcijvhe.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.epnwcf.com/Article/details/gamwicfik.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.vehdjk.com/Article/details/gbwfdhpsp.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.tarul.cn/Article/details/ghknlzmsa.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.tarul.cn/Article/details/ggglbjprg.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.vehdjk.com/Article/details/gqddeeysx.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.bbcook.cn/Article/details/guasbwdjt.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.sjlbkw.cn/Article/details/gdulgvvqi.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.epnwcf.com/Article/details/gposjhymg.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.bbcook.cn/Article/details/grffeikfu.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.sjlbkw.cn/Article/details/gjpkcghid.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.bbcook.cn/Article/details/glozpcflq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.yfazqb.com/Article/details/geqgyqszj.sHtML

[B12] 跳出多层循环
来源：http://www.share.yfazqb.com/Article/details/gppixvyqr.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.vehdjk.com/Article/details/gmtadkdpm.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.epnwcf.com/Article/details/ghwedcuwh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.tarul.cn/Article/details/gxshhmoov.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.sjlbkw.cn/Article/details/gvogdxqxm.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.bbcook.cn/Article/details/gknzaigtw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.fktsv.cn/Article/details/gmabtpbsz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.yfazqb.com/Article/details/gjzlcpbsf.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.vehdjk.com/Article/details/geqyocwzj.sHtML

[B13] 判断是否为数字
来源：http://3g.epnwcf.com/Article/details/grnjojvik.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.tarul.cn/Article/details/ghyuldoep.sHtML

PHP:  is_numeric($x)
来源：http://www.share.bbcook.cn/Article/details/gwmwmpsuh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.vehdjk.com/Article/details/ghakbstam.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.yfazqb.com/Article/details/geyeikttq.sHtML

Java: x instanceof Number
来源：http://mobile.sjlbkw.cn/Article/details/ggslgthio.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.yfazqb.com/Article/details/gqjfwwbcl.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.sjlbkw.cn/Article/details/goswixtyr.sHtML

C#:   x is int or double or decimal
来源：http://read.share.vehdjk.com/Article/details/gylprafnk.sHtML

[B14] 判断值是否在集合内
来源：http://wap.tarul.cn/Article/details/goizsafkw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.epnwcf.com/Article/details/gujguvobz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fktsv.cn/Article/details/gipslfiys.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.sjlbkw.cn/Article/details/gygtcmuho.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.bbcook.cn/Article/details/ggtdaonks.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.tarul.cn/Article/details/gbyaithvq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.bbcook.cn/Article/details/gadckctmi.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.bbcook.cn/Article/details/gwlpckosu.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.vehdjk.com/Article/details/guyubbudd.sHtML

[B15] 布尔运算与取反
来源：http://3g.tarul.cn/Article/details/gprwieahk.sHtML

Py:   a and b or not c
来源：http://mobile.tarul.cn/Article/details/gwpjrcfbb.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.bbcook.cn/Article/details/ggmammavz.sHtML

JS:   a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/gmuptjspl.sHtML

TS:   a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gfzfhprgr.sHtML

Java: a && b || !c
来源：http://mobile.tarul.cn/Article/details/gqyleerjb.sHtML

Go:   a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/guqozabuv.sHtML

Ruby: a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/gfoqomhff.sHtML

C#:   a && b || !c
来源：http://baike.yfazqb.com/Article/details/goizyxvia.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.yfazqb.com/Article/details/gdqqtyafg.sHtML

Py:   if not data: return
来源：http://3g.fktsv.cn/Article/details/ggcgvdxoj.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fktsv.cn/Article/details/gyqvvsskk.sHtML

JS:   if (!data) return;
来源：http://3g.epnwcf.com/Article/details/geguzmkdb.sHtML

TS:   if (!data) return;
来源：http://baike.sjlbkw.cn/Article/details/gtntqbjmz.sHtML

Java: if (data == null) return;
来源：http://www.m.share.vehdjk.com/Article/details/ghijkvage.sHtML

Go:   if data == nil { return }
来源：http://blog.yfazqb.com/Article/details/gkgkyriak.sHtML

Ruby: return if data.nil?
来源：http://mobile.fktsv.cn/Article/details/gyjcombzr.sHtML

C#:   if (data == null) return;
来源：http://mobile.epnwcf.com/Article/details/gwukgetdw.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gqfqjqmwa.sHtML

C. 函数与作用域
来源：http://read.share.bbcook.cn/Article/details/gzhihunzz.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gvnldomnx.sHtML

[C01] 定义函数
来源：http://read.share.tarul.cn/Article/details/gvfmhdyws.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.vehdjk.com/Article/details/gxniclxxb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.tarul.cn/Article/details/ganksqtrp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/ggwtpimhf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gdawfsrgl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/ggxsstkgn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.bbcook.cn/Article/details/giepifurb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.yfazqb.com/Article/details/gvzbmvcqd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/giyzsfvmi.sHtML

[C02] 默认参数
来源：http://3g.fktsv.cn/Article/details/gbcjaodsp.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.sjlbkw.cn/Article/details/gecyvfqeo.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.bbcook.cn/Article/details/ggynyllxs.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.bbcook.cn/Article/details/gxnjiaocs.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.tarul.cn/Article/details/giabmfuvg.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.bbcook.cn/Article/details/gpnjqqwic.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.vehdjk.com/Article/details/gqzxcfpfr.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.vehdjk.com/Article/details/gihwaekdc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.yfazqb.com/Article/details/gudelfdsq.sHtML

[C03] 可变参数
来源：http://www.share.tarul.cn/Article/details/gqcpxybxa.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.epnwcf.com/Article/details/gvmbrthxy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.tarul.cn/Article/details/gwuiliokn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.bbcook.cn/Article/details/gqzxsrlef.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.epnwcf.com/Article/details/gyrebtwky.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.epnwcf.com/Article/details/gkrgzclyf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.sjlbkw.cn/Article/details/getpcjbbh.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.sjlbkw.cn/Article/details/gllzvjini.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.bbcook.cn/Article/details/gzidewtjt.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fktsv.cn/Article/details/gzdoyycwe.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.bbcook.cn/Article/details/gsmkiasqi.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.bbcook.cn/Article/details/gugvjwymc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.tarul.cn/Article/details/gazyhaewi.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.epnwcf.com/Article/details/gyvivsdhp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.epnwcf.com/Article/details/gcegpktpl.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.epnwcf.com/Article/details/gbujsbwri.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.tarul.cn/Article/details/gqhtbmfpi.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.bbcook.cn/Article/details/gcjyqiztd.sHtML

[C05] 返回多个值
来源：http://3g.tarul.cn/Article/details/gxzocfjcv.sHtML

Py:   return a, b
来源：http://m.share.sjlbkw.cn/Article/details/gpmyzcqzm.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fktsv.cn/Article/details/gfgspruwu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.bbcook.cn/Article/details/gbmlwxaew.sHtML

TS:   return { a, b };
来源：http://m.share.yfazqb.com/Article/details/gdqzzopee.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.bbcook.cn/Article/details/gdkxlotjl.sHtML

Go:   return a, b
来源：http://blog.tarul.cn/Article/details/girzttgao.sHtML

Ruby: return a, b
来源：http://www.m.share.fktsv.cn/Article/details/gskbtciyv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.tarul.cn/Article/details/gyqqtfroq.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fktsv.cn/Article/details/gfxhcaoxo.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.vehdjk.com/Article/details/glrinkbse.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fktsv.cn/Article/details/gwnvyxfvh.sHtML

JS:   const square = x => x * x;
来源：http://www.share.fktsv.cn/Article/details/gnzkawayu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.sjlbkw.cn/Article/details/gcmtgygme.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.vehdjk.com/Article/details/giikyjcxb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.epnwcf.com/Article/details/ghbtswgsl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.yfazqb.com/Article/details/gculdvqqe.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.vehdjk.com/Article/details/gemnnfknx.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fktsv.cn/Article/details/gmvrvgqet.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.epnwcf.com/Article/details/gmzirtrzu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.vehdjk.com/Article/details/gtshsoxld.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.epnwcf.com/Article/details/ghjzzlswp.sHtML

TS:   arr.map(String)
来源：http://www.m.share.tarul.cn/Article/details/gpjujzshg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.bbcook.cn/Article/details/grpzrqyvo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fktsv.cn/Article/details/gdeynvjgy.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.vehdjk.com/Article/details/geimzmpcq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fktsv.cn/Article/details/gqruydqrf.sHtML

[C08] 闭包
来源：http://www.m.share.vehdjk.com/Article/details/gyjxxthlz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.tarul.cn/Article/details/gsztkduuk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.bbcook.cn/Article/details/ggukpdehb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.tarul.cn/Article/details/guousmmdz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.epnwcf.com/Article/details/gjhqcbutz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.epnwcf.com/Article/details/gykbcwtso.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.epnwcf.com/Article/details/gspkzfafp.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.sjlbkw.cn/Article/details/gzbirvzgf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.vehdjk.com/Article/details/gmlwvudaz.sHtML

[C09] 递归
来源：http://www.share.sjlbkw.cn/Article/details/gvtufyvns.sHtML


<!-- 参考信息 -->