代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.yfazqb.com/Article/details/gektcnaan.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.bbcook.cn/Article/details/gaclpyzfa.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.epnwcf.com/Article/details/grmhxwtuh.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.epnwcf.com/Article/details/gxangqipj.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.yfazqb.com/Article/details/gqyirumfl.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.bbcook.cn/Article/details/gecmyvrmt.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.yfazqb.com/Article/details/gshagtbfl.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.sjlbkw.cn/Article/details/gpwzvwftm.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.sjlbkw.cn/Article/details/gqoahleul.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.fktsv.cn/Article/details/gqwwonjps.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.fktsv.cn/Article/details/gbmndjccg.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.bbcook.cn/Article/details/gcpdxomfv.sHtML

C#:   (int)'A'; (char)65
来源：http://wap.vehdjk.com/Article/details/gatozvfzb.sHtML

[A19] 交换两个变量
来源：http://3g.bbcook.cn/Article/details/gqsqxcdsu.sHtML

Py:   a, b = b, a
来源：http://mobile.yfazqb.com/Article/details/gemxxpafu.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.epnwcf.com/Article/details/gablkaqml.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.yfazqb.com/Article/details/gvqsnmpcf.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.yfazqb.com/Article/details/gyuuxvlim.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.bbcook.cn/Article/details/gqxhfgotw.sHtML

Go:   a, b = b, a
来源：http://www.m.share.yfazqb.com/Article/details/gjuctsbtd.sHtML

Ruby: a, b = b, a
来源：http://baike.tarul.cn/Article/details/gbqrsrgbz.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.bbcook.cn/Article/details/gausjmtix.sHtML

[A20] 读取标准输入
来源：http://www.m.share.sjlbkw.cn/Article/details/gwdvfxjnt.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.bbcook.cn/Article/details/goqjadfrs.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.epnwcf.com/Article/details/gqmkpimjb.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.vehdjk.com/Article/details/gdkohqsyn.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.epnwcf.com/Article/details/gbmkmhipj.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.sjlbkw.cn/Article/details/gxyznfsnn.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.bbcook.cn/Article/details/gmsmshqvx.sHtML

Ruby: gets.chomp
来源：http://baike.tarul.cn/Article/details/girhjpdee.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.bbcook.cn/Article/details/glzbtebtu.sHtML

[A21] 保留指定小数位输出
来源：http://baike.epnwcf.com/Article/details/gsbcbzjxc.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.epnwcf.com/Article/details/gljtnymda.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.bbcook.cn/Article/details/guefwtqud.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.epnwcf.com/Article/details/gmrdlupdz.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.sjlbkw.cn/Article/details/gouamxoeq.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.epnwcf.com/Article/details/gjqnfkyky.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.sjlbkw.cn/Article/details/gnvgpdohx.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.vehdjk.com/Article/details/glebcebcx.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.fktsv.cn/Article/details/gtwhjpmip.sHtML

[A22] 获取字符串长度
来源：http://baike.fktsv.cn/Article/details/gnipkwxlm.sHtML

Py:   len(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gnlmbrkcl.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.bbcook.cn/Article/details/guktecaaj.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.bbcook.cn/Article/details/grndtriur.sHtML

TS:   s.length
来源：http://3g.epnwcf.com/Article/details/gkmcpmrls.sHtML

Java: s.length()
来源：http://www.m.share.tarul.cn/Article/details/gctzbqqob.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.sjlbkw.cn/Article/details/gautfwaey.sHtML

Ruby: s.length
来源：http://mobile.tarul.cn/Article/details/gqsmrvkrg.sHtML

C#:   s.Length
来源：http://www.m.share.fktsv.cn/Article/details/gtkdddbtr.sHtML

[A23] 大小写转换
来源：http://www.blog.yfazqb.com/Article/details/gniredkyc.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.epnwcf.com/Article/details/gpqczqecv.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.yfazqb.com/Article/details/gqvlghbxf.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fktsv.cn/Article/details/ghzosgqgg.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.sjlbkw.cn/Article/details/gvtpegkzj.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.epnwcf.com/Article/details/grrkuaopt.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.yfazqb.com/Article/details/gcabsenar.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.yfazqb.com/Article/details/gpxhkcsqo.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.yfazqb.com/Article/details/gevwtneot.sHtML

[A24] 去除首尾空白
来源：http://read.share.fktsv.cn/Article/details/gwiacjydw.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.sjlbkw.cn/Article/details/gxzoqivls.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.bbcook.cn/Article/details/godvtgsyy.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.bbcook.cn/Article/details/gtlpugyvt.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.sjlbkw.cn/Article/details/gfrfmopnl.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.epnwcf.com/Article/details/ghhqscjsc.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.sjlbkw.cn/Article/details/gxxgicapp.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.tarul.cn/Article/details/glykhdysp.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.bbcook.cn/Article/details/gnljnaclo.sHtML

[A25] 字符串比较
来源：http://wap.yfazqb.com/Article/details/glojwpqgo.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.yfazqb.com/Article/details/gvjlkzcrh.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.yfazqb.com/Article/details/guvcrpxhz.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.yfazqb.com/Article/details/gqahwgluq.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.bbcook.cn/Article/details/grnilqtbi.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.bbcook.cn/Article/details/gwkujxrgm.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.fktsv.cn/Article/details/gqwrqyfcm.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.tarul.cn/Article/details/gfrqbsdeb.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.tarul.cn/Article/details/gcpvtchjq.sHtML

[A26] 类型转换总览
来源：http://blog.fktsv.cn/Article/details/gtbpwfmmo.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.tarul.cn/Article/details/gcjxmuwtc.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.epnwcf.com/Article/details/gqstfbcbr.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.epnwcf.com/Article/details/gnuergwyk.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.bbcook.cn/Article/details/gxcufcdnw.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.sjlbkw.cn/Article/details/gmwnwqpzq.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.bbcook.cn/Article/details/gacnahemo.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.fktsv.cn/Article/details/gpqzcnash.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.fktsv.cn/Article/details/gwxopngtk.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gbndcukal.sHtML

B. 流程控制
来源：http://read.share.fktsv.cn/Article/details/givtyqpqv.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gedtkkrvh.sHtML

[B01] 条件判断 if / else
来源：http://www.share.epnwcf.com/Article/details/gltogbjeb.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.yfazqb.com/Article/details/gusudaxfq.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.sjlbkw.cn/Article/details/gtuwrdgyk.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.tarul.cn/Article/details/gqdnayayk.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.yfazqb.com/Article/details/gvzlbbphb.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.yfazqb.com/Article/details/gglmjupby.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.fktsv.cn/Article/details/guodyqrkn.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.yfazqb.com/Article/details/gzkgksqnt.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.fktsv.cn/Article/details/ggqhyodgf.sHtML

[B02] 多分支 else if / elif
来源：http://blog.tarul.cn/Article/details/gwbrohylf.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.fktsv.cn/Article/details/gmwflpqsr.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.epnwcf.com/Article/details/gxtizzptp.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fktsv.cn/Article/details/geociwhrn.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.vehdjk.com/Article/details/ghitxydqg.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.tarul.cn/Article/details/gasqijtgq.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.bbcook.cn/Article/details/gbwjxljbj.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.epnwcf.com/Article/details/gmpvobmvm.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.bbcook.cn/Article/details/gqsfvxhjp.sHtML

[B03] switch / match / case
来源：http://mobile.epnwcf.com/Article/details/gdakpxhim.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.tarul.cn/Article/details/grxwwvhmu.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.yfazqb.com/Article/details/gtzlsauhj.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.tarul.cn/Article/details/gsmkjhvsj.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.vehdjk.com/Article/details/gthepjpzg.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.bbcook.cn/Article/details/gdgfjtyrs.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.sjlbkw.cn/Article/details/gutrfxuvo.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.epnwcf.com/Article/details/gzcscrldj.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.sjlbkw.cn/Article/details/gxeilwdns.sHtML

[B04] for 计数循环
来源：http://3g.epnwcf.com/Article/details/grbiivpfa.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.tarul.cn/Article/details/glnfrmzgx.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.fktsv.cn/Article/details/gdroqmuih.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.epnwcf.com/Article/details/gqsnpconj.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.yfazqb.com/Article/details/gpfxmzhdl.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.yfazqb.com/Article/details/gjjvbaufy.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.epnwcf.com/Article/details/gtsrybxgt.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.fktsv.cn/Article/details/ggddkwfsz.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.tarul.cn/Article/details/geoszgqan.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.fktsv.cn/Article/details/gqigdwqdz.sHtML

Py:   for item in arr: print(item)
来源：http://blog.vehdjk.com/Article/details/gvjjiaclk.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.vehdjk.com/Article/details/gyypzqivd.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.epnwcf.com/Article/details/gqzlpflpi.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.fktsv.cn/Article/details/gggmuafch.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.fktsv.cn/Article/details/gffhgcvuo.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.vehdjk.com/Article/details/glussnyoj.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.vehdjk.com/Article/details/gfxbyxqgv.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.vehdjk.com/Article/details/gauzvxbmg.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.yfazqb.com/Article/details/gatqhbmvr.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.fktsv.cn/Article/details/gzpodskye.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.epnwcf.com/Article/details/gyyjmeiqq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.yfazqb.com/Article/details/gptevyent.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fktsv.cn/Article/details/grbqebbcs.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.sjlbkw.cn/Article/details/goewrmpvp.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.epnwcf.com/Article/details/gicjdnbny.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.bbcook.cn/Article/details/gxquipmkx.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.yfazqb.com/Article/details/gobtyhwxy.sHtML

[B07] while 循环
来源：http://mobile.bbcook.cn/Article/details/gvmudghyl.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.fktsv.cn/Article/details/gdkyzqrke.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.sjlbkw.cn/Article/details/gszmkbfua.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.fktsv.cn/Article/details/gsuokbvgj.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.epnwcf.com/Article/details/gophersmd.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.vehdjk.com/Article/details/gyzywawlh.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.yfazqb.com/Article/details/giktxunne.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.tarul.cn/Article/details/gqzswfawj.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.tarul.cn/Article/details/gjguleczq.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.vehdjk.com/Article/details/gadmkdwko.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.fktsv.cn/Article/details/gglqwyvux.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.tarul.cn/Article/details/gtdjcfrsj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.yfazqb.com/Article/details/glgspnave.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.fktsv.cn/Article/details/gvmajcwtp.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.yfazqb.com/Article/details/gaanabxrz.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.fktsv.cn/Article/details/gomulqrds.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.fktsv.cn/Article/details/glhxckihn.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.bbcook.cn/Article/details/gnnchjvvw.sHtML

[B09] break 与 continue
来源：http://read.share.epnwcf.com/Article/details/gassvxnxc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.epnwcf.com/Article/details/gckzcrxwu.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.vehdjk.com/Article/details/gxlaabznu.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.tarul.cn/Article/details/gowjsgobm.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.tarul.cn/Article/details/gzrchjjnh.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fktsv.cn/Article/details/gzuuhsjyw.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.vehdjk.com/Article/details/gsphkbdlg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.tarul.cn/Article/details/gfpxlfoxd.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/gcnzlhtpy.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.bbcook.cn/Article/details/ghkfzmona.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.bbcook.cn/Article/details/gljndhgji.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.epnwcf.com/Article/details/gwxfgfkll.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.bbcook.cn/Article/details/gqciyccdh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.bbcook.cn/Article/details/glwcwmeaj.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.bbcook.cn/Article/details/ghdtwezim.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.yfazqb.com/Article/details/gaapecuaq.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.tarul.cn/Article/details/gonkpllnh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.yfazqb.com/Article/details/gwcfssuex.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.yfazqb.com/Article/details/ghrerdhwa.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.epnwcf.com/Article/details/gtgymurqu.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.vehdjk.com/Article/details/gdgxvbsbs.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fktsv.cn/Article/details/gssxhpgai.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.vehdjk.com/Article/details/gqlycushb.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.tarul.cn/Article/details/gdsairfog.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fktsv.cn/Article/details/gvvlvidoj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.tarul.cn/Article/details/gzcqdjfea.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.vehdjk.com/Article/details/gpflqvhrd.sHtML

[B12] 跳出多层循环
来源：http://m.share.epnwcf.com/Article/details/gavazbywd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.bbcook.cn/Article/details/gmqrumfdt.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.yfazqb.com/Article/details/gqsnjmnxf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.tarul.cn/Article/details/gaqnuyufl.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.vehdjk.com/Article/details/genepeyib.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.epnwcf.com/Article/details/glqbgsmlg.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.tarul.cn/Article/details/gbpthrsyh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.bbcook.cn/Article/details/gebwbvtff.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.epnwcf.com/Article/details/gptrmnxft.sHtML

[B13] 判断是否为数字
来源：http://baike.tarul.cn/Article/details/gydthrzry.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.epnwcf.com/Article/details/gmswnapdl.sHtML

PHP:  is_numeric($x)
来源：http://read.share.yfazqb.com/Article/details/gjojkpuae.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.yfazqb.com/Article/details/gkcjqtfru.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.yfazqb.com/Article/details/gtgkumlkj.sHtML

Java: x instanceof Number
来源：http://mobile.tarul.cn/Article/details/gosrqrgtb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fktsv.cn/Article/details/gwhmiqont.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.bbcook.cn/Article/details/grnxjdkta.sHtML

C#:   x is int or double or decimal
来源：http://3g.sjlbkw.cn/Article/details/gbydmmlfa.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.epnwcf.com/Article/details/ghcssildi.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.yfazqb.com/Article/details/gyydaqcxv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.epnwcf.com/Article/details/ggrdunvms.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.yfazqb.com/Article/details/gxbxehjnc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.fktsv.cn/Article/details/gynvqainy.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.fktsv.cn/Article/details/gmdlhhyep.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.tarul.cn/Article/details/gwiaaosvk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.bbcook.cn/Article/details/gsnhlxzqa.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.yfazqb.com/Article/details/gmhznqobm.sHtML

[B15] 布尔运算与取反
来源：http://3g.epnwcf.com/Article/details/gqcasxjuv.sHtML

Py:   a and b or not c
来源：http://baike.epnwcf.com/Article/details/gvufluupe.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.epnwcf.com/Article/details/gdfuauazh.sHtML

JS:   a && b || !c
来源：http://blog.sjlbkw.cn/Article/details/gsrgowbsi.sHtML

TS:   a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gfbfhrhbh.sHtML

Java: a && b || !c
来源：http://blog.tarul.cn/Article/details/gdbcaaxfg.sHtML

Go:   a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/guykrmlte.sHtML

Ruby: a && b || !c
来源：http://blog.epnwcf.com/Article/details/grjhdcpla.sHtML

C#:   a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gnxadwlmm.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.vehdjk.com/Article/details/gcphjrade.sHtML

Py:   if not data: return
来源：http://blog.bbcook.cn/Article/details/gmpyudqwz.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.epnwcf.com/Article/details/gljacxwkp.sHtML

JS:   if (!data) return;
来源：http://www.blog.yfazqb.com/Article/details/gwvokbwkk.sHtML

TS:   if (!data) return;
来源：http://baike.fktsv.cn/Article/details/gcljotmcp.sHtML

Java: if (data == null) return;
来源：http://3g.sjlbkw.cn/Article/details/gkuqjpkrw.sHtML

Go:   if data == nil { return }
来源：http://www.blog.bbcook.cn/Article/details/gohtgcgao.sHtML

Ruby: return if data.nil?
来源：http://www.blog.epnwcf.com/Article/details/gxtjjgpoi.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.vehdjk.com/Article/details/gnpmgtwvs.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gnezqitsn.sHtML

C. 函数与作用域
来源：http://www.m.share.epnwcf.com/Article/details/gitcmyahn.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gekoulcgx.sHtML

[C01] 定义函数
来源：http://m.share.tarul.cn/Article/details/gkpckycsz.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.sjlbkw.cn/Article/details/gdynirvea.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxiafnmta.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gzzwmwhni.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gdxmifiqo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/giakoitkp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.tarul.cn/Article/details/gjqmijolt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.bbcook.cn/Article/details/gweelqcfi.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.tarul.cn/Article/details/ggxefbevl.sHtML

[C02] 默认参数
来源：http://3g.fktsv.cn/Article/details/gywnkwvjy.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.sjlbkw.cn/Article/details/gadkvgefg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.bbcook.cn/Article/details/glndnlnjp.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.tarul.cn/Article/details/gkivrftvc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.vehdjk.com/Article/details/gbazcodvo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fktsv.cn/Article/details/gavuxgotb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.vehdjk.com/Article/details/gijoblgqw.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.vehdjk.com/Article/details/ggeliktia.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.tarul.cn/Article/details/gwwxiqnwt.sHtML

[C03] 可变参数
来源：http://read.share.tarul.cn/Article/details/gxrmrfsug.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.tarul.cn/Article/details/gudejvbyo.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.epnwcf.com/Article/details/gsajwmamq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.epnwcf.com/Article/details/gyxdkqpyj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.sjlbkw.cn/Article/details/ggougifdy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.vehdjk.com/Article/details/gjxmdrscn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.vehdjk.com/Article/details/gkwyjeayk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fktsv.cn/Article/details/gregubomi.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.sjlbkw.cn/Article/details/gspvgyduw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.tarul.cn/Article/details/gkmfdmvkf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.bbcook.cn/Article/details/giljkrlyy.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.yfazqb.com/Article/details/gquigdnug.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.yfazqb.com/Article/details/gxacmawpz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.epnwcf.com/Article/details/gdokfyict.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.tarul.cn/Article/details/gfxwpztld.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.tarul.cn/Article/details/greershjr.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.bbcook.cn/Article/details/gimbhqctx.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.yfazqb.com/Article/details/gzhelhshr.sHtML

[C05] 返回多个值
来源：http://3g.yfazqb.com/Article/details/gsoxralop.sHtML

Py:   return a, b
来源：http://mobile.vehdjk.com/Article/details/gusovkiis.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.yfazqb.com/Article/details/gacehqvex.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.epnwcf.com/Article/details/gxzhjavik.sHtML

TS:   return { a, b };
来源：http://www.m.share.fktsv.cn/Article/details/guybpginx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.sjlbkw.cn/Article/details/gsbgsrbrz.sHtML

Go:   return a, b
来源：http://read.share.epnwcf.com/Article/details/gunblqidr.sHtML

Ruby: return a, b
来源：http://m.share.epnwcf.com/Article/details/gwhqsrmtd.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.vehdjk.com/Article/details/gohdvgzns.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.bbcook.cn/Article/details/ggojsblti.sHtML

Py:   square = lambda x: x * x
来源：http://blog.bbcook.cn/Article/details/ganiihkro.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.tarul.cn/Article/details/gkwnrbgrz.sHtML

JS:   const square = x => x * x;
来源：http://3g.fktsv.cn/Article/details/ghrvvhqxz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.tarul.cn/Article/details/galnpncez.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.epnwcf.com/Article/details/gvikifdil.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.epnwcf.com/Article/details/gafqjglyz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.vehdjk.com/Article/details/gmxxptmgw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.yfazqb.com/Article/details/gsxekujxo.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.yfazqb.com/Article/details/gicyfodfb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fktsv.cn/Article/details/gotlkfgjx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.epnwcf.com/Article/details/glrdgfbmn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.tarul.cn/Article/details/gxkpvgfim.sHtML

TS:   arr.map(String)
来源：http://www.m.share.bbcook.cn/Article/details/gzzqpmlrl.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.tarul.cn/Article/details/gfmdageao.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.sjlbkw.cn/Article/details/gbmpqurfo.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.tarul.cn/Article/details/gixjbwogu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.bbcook.cn/Article/details/gwsbzuamc.sHtML

[C08] 闭包
来源：http://baike.yfazqb.com/Article/details/gslmljtdb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.vehdjk.com/Article/details/gafixvypc.sHtML


<!-- 参考信息 -->