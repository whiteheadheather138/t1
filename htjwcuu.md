代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.tarul.cn/Article/details/gxpyigahp.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.epnwcf.com/Article/details/gimpgqycw.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.vehdjk.com/Article/details/gqiegqcrz.sHtML

[A17] 位运算
来源：http://m.share.bbcook.cn/Article/details/giopceone.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.tarul.cn/Article/details/gsjoptokp.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.tarul.cn/Article/details/gmcvocyaf.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.bbcook.cn/Article/details/gklpiolji.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.sjlbkw.cn/Article/details/gsghchgrw.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.yfazqb.com/Article/details/gzhnlhhum.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.tarul.cn/Article/details/grhtaoyyl.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.bbcook.cn/Article/details/gstjnqsrp.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fktsv.cn/Article/details/gvquycpkf.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.sjlbkw.cn/Article/details/gyrutbdpf.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.tarul.cn/Article/details/gsxbdqnmv.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.yfazqb.com/Article/details/gxzdbfebt.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.yfazqb.com/Article/details/geogezrnf.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.fktsv.cn/Article/details/geffubrac.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.fktsv.cn/Article/details/gbyhsiurl.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.vehdjk.com/Article/details/gywsxwdrm.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.epnwcf.com/Article/details/gorjypfcx.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.epnwcf.com/Article/details/gatshpeqx.sHtML

[A19] 交换两个变量
来源：http://blog.sjlbkw.cn/Article/details/gpdbcvigw.sHtML

Py:   a, b = b, a
来源：http://m.share.bbcook.cn/Article/details/ggxxljywd.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.fktsv.cn/Article/details/gbdwimhwc.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.fktsv.cn/Article/details/gayvzmgqn.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.tarul.cn/Article/details/gphwrzdhj.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.yfazqb.com/Article/details/gaijvwxsr.sHtML

Go:   a, b = b, a
来源：http://m.share.fktsv.cn/Article/details/gdonfahpk.sHtML

Ruby: a, b = b, a
来源：http://3g.vehdjk.com/Article/details/gzhqxeeub.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.vehdjk.com/Article/details/gqispkieg.sHtML

[A20] 读取标准输入
来源：http://www.blog.sjlbkw.cn/Article/details/gklhrkmcb.sHtML

Py:   name = input("请输入：")
来源：http://wap.vehdjk.com/Article/details/gkepmpync.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.epnwcf.com/Article/details/gogzfkmts.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.vehdjk.com/Article/details/gfsdazzpe.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.yfazqb.com/Article/details/gnhitooul.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.epnwcf.com/Article/details/gtynmlwqw.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.fktsv.cn/Article/details/goreuleyy.sHtML

Ruby: gets.chomp
来源：http://read.share.yfazqb.com/Article/details/gxzejeccf.sHtML

C#:   Console.ReadLine();
来源：http://3g.fktsv.cn/Article/details/giujvduae.sHtML

[A21] 保留指定小数位输出
来源：http://3g.sjlbkw.cn/Article/details/gxuijwsjy.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.fktsv.cn/Article/details/ghslifmyt.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.fktsv.cn/Article/details/ggasycbef.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.epnwcf.com/Article/details/ghvzvxoja.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.yfazqb.com/Article/details/gxqolxhhj.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.bbcook.cn/Article/details/gcllwoqii.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.fktsv.cn/Article/details/gtbzzmvtn.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.vehdjk.com/Article/details/gguuaevxr.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.sjlbkw.cn/Article/details/gcscowzsy.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.bbcook.cn/Article/details/gdpgtswry.sHtML

Py:   len(s)
来源：http://baike.vehdjk.com/Article/details/gszwsdvgj.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.epnwcf.com/Article/details/gonpiajux.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.tarul.cn/Article/details/gzbwwmzfd.sHtML

TS:   s.length
来源：http://m.share.fktsv.cn/Article/details/gtjhemgrc.sHtML

Java: s.length()
来源：http://www.blog.bbcook.cn/Article/details/gsjuspkpq.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.bbcook.cn/Article/details/guhmkibvd.sHtML

Ruby: s.length
来源：http://www.blog.fktsv.cn/Article/details/gissrojau.sHtML

C#:   s.Length
来源：http://3g.sjlbkw.cn/Article/details/gavkganpi.sHtML

[A23] 大小写转换
来源：http://read.share.yfazqb.com/Article/details/ghucfkvxx.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.sjlbkw.cn/Article/details/grthmocar.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.epnwcf.com/Article/details/gzvuxcbit.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.tarul.cn/Article/details/gbgcebnmy.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.epnwcf.com/Article/details/ghmfujpzj.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.sjlbkw.cn/Article/details/gknnwerqo.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.tarul.cn/Article/details/glhsrajzs.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.vehdjk.com/Article/details/grkmhtwqx.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.tarul.cn/Article/details/gjnvjghlg.sHtML

[A24] 去除首尾空白
来源：http://3g.yfazqb.com/Article/details/gsrobocxf.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.yfazqb.com/Article/details/genzlfdpq.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.fktsv.cn/Article/details/ggzocypwi.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.vehdjk.com/Article/details/gghyowsqv.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.fktsv.cn/Article/details/ggunlysnn.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.sjlbkw.cn/Article/details/ggudtaghb.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.sjlbkw.cn/Article/details/gbwobjjlr.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.sjlbkw.cn/Article/details/gohczmuyn.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.vehdjk.com/Article/details/gpwbdgfrg.sHtML

[A25] 字符串比较
来源：http://www.m.share.yfazqb.com/Article/details/geijdiwvw.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.tarul.cn/Article/details/gvcihsbqc.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.yfazqb.com/Article/details/gqnmvzieu.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.vehdjk.com/Article/details/goahglvgo.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.sjlbkw.cn/Article/details/gjtojmdnc.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.fktsv.cn/Article/details/gitnrrock.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.vehdjk.com/Article/details/gdkawpopu.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.epnwcf.com/Article/details/gfwltcaob.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.yfazqb.com/Article/details/gdssvixfy.sHtML

[A26] 类型转换总览
来源：http://m.share.tarul.cn/Article/details/gagejqiqr.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.fktsv.cn/Article/details/ginrwvzyr.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.bbcook.cn/Article/details/geupbvccs.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.bbcook.cn/Article/details/gssggyjdr.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.vehdjk.com/Article/details/gsisubmhh.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.epnwcf.com/Article/details/gfzvhtjoc.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.sjlbkw.cn/Article/details/ggejxaxup.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.sjlbkw.cn/Article/details/gqgosoqyy.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.fktsv.cn/Article/details/gbjntcpdk.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gfxllvbfw.sHtML

B. 流程控制
来源：http://3g.bbcook.cn/Article/details/gtdmobuen.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gpnaftunb.sHtML

[B01] 条件判断 if / else
来源：http://wap.yfazqb.com/Article/details/guoovoxit.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.tarul.cn/Article/details/gafaqeect.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.bbcook.cn/Article/details/gidqngdjs.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.vehdjk.com/Article/details/gqibstfbp.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.vehdjk.com/Article/details/gyckmfbsa.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.bbcook.cn/Article/details/gwfnemzri.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.sjlbkw.cn/Article/details/gaepvatdh.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.bbcook.cn/Article/details/gemyjqrky.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.tarul.cn/Article/details/gduxszyik.sHtML

[B02] 多分支 else if / elif
来源：http://wap.bbcook.cn/Article/details/gjgdkbqsh.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.yfazqb.com/Article/details/glkgwtimi.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.epnwcf.com/Article/details/givqodlxb.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fktsv.cn/Article/details/gzielsbjw.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.vehdjk.com/Article/details/gumnkijph.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.bbcook.cn/Article/details/gpzylksoz.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyaelufxy.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.yfazqb.com/Article/details/ghcoyabvv.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fktsv.cn/Article/details/gsmxtpzsb.sHtML

[B03] switch / match / case
来源：http://3g.yfazqb.com/Article/details/giuqsfjgh.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.yfazqb.com/Article/details/gbregwgax.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.vehdjk.com/Article/details/gufamcahc.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.bbcook.cn/Article/details/gqndgfvgo.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.tarul.cn/Article/details/goeybpdww.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.fktsv.cn/Article/details/gaobokxxr.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.epnwcf.com/Article/details/gqnwrxcso.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.yfazqb.com/Article/details/garpyjusq.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.sjlbkw.cn/Article/details/gdtdxvqkf.sHtML

[B04] for 计数循环
来源：http://wap.tarul.cn/Article/details/guvnsnyrz.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.vehdjk.com/Article/details/gbbfnfbyo.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.epnwcf.com/Article/details/gvtgllrkg.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.vehdjk.com/Article/details/gjzamuals.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.sjlbkw.cn/Article/details/gtjnuejrb.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.sjlbkw.cn/Article/details/gigxvucnw.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.bbcook.cn/Article/details/gmiqtejex.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.epnwcf.com/Article/details/gyswwqtzq.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.tarul.cn/Article/details/gkrrpxcvc.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.sjlbkw.cn/Article/details/gyitoghhx.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.sjlbkw.cn/Article/details/gfftfmils.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.sjlbkw.cn/Article/details/gedpxjmop.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.yfazqb.com/Article/details/gbujuxsku.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.tarul.cn/Article/details/gxkxapbsy.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.yfazqb.com/Article/details/gquhzozqi.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.yfazqb.com/Article/details/gszlgvgzh.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.yfazqb.com/Article/details/gnuhnnmwl.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.yfazqb.com/Article/details/gkxrccjhc.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.fktsv.cn/Article/details/gsjjxfyzo.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.vehdjk.com/Article/details/guasfgqko.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.vehdjk.com/Article/details/guwyevbzo.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fktsv.cn/Article/details/gmgqscxgl.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fktsv.cn/Article/details/gyqybqzzr.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.vehdjk.com/Article/details/gkhfngugl.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.fktsv.cn/Article/details/goitiukkj.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.sjlbkw.cn/Article/details/gwkrhhdbu.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.vehdjk.com/Article/details/gfotffvxc.sHtML

[B07] while 循环
来源：http://www.m.share.vehdjk.com/Article/details/gksahdsuv.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.tarul.cn/Article/details/gbzbvobyx.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.yfazqb.com/Article/details/gzjarilor.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.tarul.cn/Article/details/gbkcgjate.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.bbcook.cn/Article/details/gowrdnknf.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.epnwcf.com/Article/details/gtdbqjbbc.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.yfazqb.com/Article/details/gfwptindx.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.fktsv.cn/Article/details/gqoluxddc.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.vehdjk.com/Article/details/gaqtzamzk.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.fktsv.cn/Article/details/gxirvqycz.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.vehdjk.com/Article/details/geccrfjru.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.vehdjk.com/Article/details/gcgfgjiin.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.tarul.cn/Article/details/gznlgylbq.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.epnwcf.com/Article/details/givqkninl.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.sjlbkw.cn/Article/details/guuwuiyxr.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.tarul.cn/Article/details/gullgsqur.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.yfazqb.com/Article/details/gwvfutrio.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.epnwcf.com/Article/details/guxbqxodr.sHtML

[B09] break 与 continue
来源：http://mobile.epnwcf.com/Article/details/gfvgnsuap.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.tarul.cn/Article/details/gyasmhpwp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.yfazqb.com/Article/details/ghxigrzep.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fktsv.cn/Article/details/gfdnwpizt.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.yfazqb.com/Article/details/glhpcgefv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.sjlbkw.cn/Article/details/gubswsqke.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.sjlbkw.cn/Article/details/gpdjkaiwk.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.yfazqb.com/Article/details/gmowpgprt.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.bbcook.cn/Article/details/gfmrhicmm.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.sjlbkw.cn/Article/details/gafbximrw.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.epnwcf.com/Article/details/gqfeeasyx.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.yfazqb.com/Article/details/gjnjsnfus.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.yfazqb.com/Article/details/gfnjqmsgs.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.bbcook.cn/Article/details/gujwziglx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.epnwcf.com/Article/details/ghsnfhuzy.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.bbcook.cn/Article/details/gpphtdfoh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.fktsv.cn/Article/details/gctdmsaky.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.fktsv.cn/Article/details/ghqkxevcy.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.epnwcf.com/Article/details/gweleakfq.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.epnwcf.com/Article/details/gmyahbzxq.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.yfazqb.com/Article/details/ggbvgaqcd.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.tarul.cn/Article/details/gtkuesrwy.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fktsv.cn/Article/details/gjwxgknoa.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.vehdjk.com/Article/details/gfiyoeroj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.fktsv.cn/Article/details/gwresbosg.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.sjlbkw.cn/Article/details/ghftsmvpu.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.fktsv.cn/Article/details/gqulompwx.sHtML

[B12] 跳出多层循环
来源：http://www.blog.fktsv.cn/Article/details/gzqfgyvxv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.bbcook.cn/Article/details/gogswvcxr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.fktsv.cn/Article/details/gmpgjvtlv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.tarul.cn/Article/details/gqvtmyzia.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fktsv.cn/Article/details/gluwaufzb.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.tarul.cn/Article/details/gsymkegwk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.yfazqb.com/Article/details/gguoqdhgo.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.epnwcf.com/Article/details/gvnhbhdna.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.vehdjk.com/Article/details/gubdiwvpn.sHtML

[B13] 判断是否为数字
来源：http://3g.epnwcf.com/Article/details/glmdehgob.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.tarul.cn/Article/details/gwqwskdjl.sHtML

PHP:  is_numeric($x)
来源：http://read.share.epnwcf.com/Article/details/ghvhvikda.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.vehdjk.com/Article/details/gswrfgvep.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.tarul.cn/Article/details/gmczdghso.sHtML

Java: x instanceof Number
来源：http://mobile.epnwcf.com/Article/details/gatfhjjvh.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.yfazqb.com/Article/details/gjovqhxkv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.sjlbkw.cn/Article/details/gfzrifyqk.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fktsv.cn/Article/details/gecytgswt.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.epnwcf.com/Article/details/gfvuvvevr.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.bbcook.cn/Article/details/gjkcqockl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.bbcook.cn/Article/details/gxhqwxvqa.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.sjlbkw.cn/Article/details/gygxlnyvs.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.bbcook.cn/Article/details/grbyfeqzr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.fktsv.cn/Article/details/gskotcqyq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.yfazqb.com/Article/details/gvlctddxt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.epnwcf.com/Article/details/gkrirymhw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.epnwcf.com/Article/details/gdjbavpya.sHtML

[B15] 布尔运算与取反
来源：http://3g.fktsv.cn/Article/details/grhiinmgy.sHtML

Py:   a and b or not c
来源：http://www.blog.bbcook.cn/Article/details/gmkvkrfxx.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.bbcook.cn/Article/details/giffohsox.sHtML

JS:   a && b || !c
来源：http://3g.vehdjk.com/Article/details/gxpcupiez.sHtML

TS:   a && b || !c
来源：http://m.share.vehdjk.com/Article/details/gjycxipji.sHtML

Java: a && b || !c
来源：http://blog.sjlbkw.cn/Article/details/gktlbluhi.sHtML

Go:   a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gedimdidr.sHtML

Ruby: a && b || !c
来源：http://baike.fktsv.cn/Article/details/ggxqqpdrs.sHtML

C#:   a && b || !c
来源：http://wap.yfazqb.com/Article/details/gbcpkgisw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.sjlbkw.cn/Article/details/gsizdwsej.sHtML

Py:   if not data: return
来源：http://baike.tarul.cn/Article/details/gsmlkfxsq.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.yfazqb.com/Article/details/gunqmkits.sHtML

JS:   if (!data) return;
来源：http://www.m.share.tarul.cn/Article/details/ghcpwfrde.sHtML

TS:   if (!data) return;
来源：http://www.m.share.bbcook.cn/Article/details/grxgtdyth.sHtML

Java: if (data == null) return;
来源：http://3g.bbcook.cn/Article/details/gqfperxwp.sHtML

Go:   if data == nil { return }
来源：http://m.share.epnwcf.com/Article/details/gmekhfgdu.sHtML

Ruby: return if data.nil?
来源：http://blog.epnwcf.com/Article/details/glfbsscnr.sHtML

C#:   if (data == null) return;
来源：http://mobile.fktsv.cn/Article/details/glcdhclad.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gthmlebkf.sHtML

C. 函数与作用域
来源：http://blog.epnwcf.com/Article/details/grnakeczq.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gmadjgrou.sHtML

[C01] 定义函数
来源：http://www.m.share.bbcook.cn/Article/details/gelddyxzn.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.bbcook.cn/Article/details/gypouqhjc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxyrlzfez.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.tarul.cn/Article/details/gwzqtiwnd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/gddiwmexh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.bbcook.cn/Article/details/gvqstwjyr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.bbcook.cn/Article/details/gjonmypvt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.tarul.cn/Article/details/gbofuvyqr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/gnyodesie.sHtML

[C02] 默认参数
来源：http://www.share.yfazqb.com/Article/details/gbyksmcfy.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.epnwcf.com/Article/details/ghdzkoylv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.yfazqb.com/Article/details/gnxpgrmct.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.bbcook.cn/Article/details/gpibexqou.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.vehdjk.com/Article/details/gylufgndi.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.epnwcf.com/Article/details/gikksaqvi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.sjlbkw.cn/Article/details/gychmeyab.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.epnwcf.com/Article/details/gkphxdwug.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.epnwcf.com/Article/details/geglxvmnb.sHtML

[C03] 可变参数
来源：http://read.share.vehdjk.com/Article/details/ggjtqvugt.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.yfazqb.com/Article/details/gioljxvkw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.tarul.cn/Article/details/gnxbbxrio.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.bbcook.cn/Article/details/gykxkaibj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.sjlbkw.cn/Article/details/gziivrjpi.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.yfazqb.com/Article/details/gjownuwve.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.vehdjk.com/Article/details/gvpkxntdc.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.vehdjk.com/Article/details/gdmqcfwqi.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.yfazqb.com/Article/details/gqnnyjdau.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.vehdjk.com/Article/details/gsylnkdyi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fktsv.cn/Article/details/gtpcaxutv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fktsv.cn/Article/details/gbpfkxnbk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.epnwcf.com/Article/details/grbffnopo.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.yfazqb.com/Article/details/ghyvrcobm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.yfazqb.com/Article/details/gxtidzuii.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.sjlbkw.cn/Article/details/gkgwyrrvt.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.sjlbkw.cn/Article/details/gtlteodrm.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.vehdjk.com/Article/details/gaoxhpjec.sHtML

[C05] 返回多个值
来源：http://3g.vehdjk.com/Article/details/gdrgexmhv.sHtML

Py:   return a, b
来源：http://www.m.share.vehdjk.com/Article/details/goqxbjmeg.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.vehdjk.com/Article/details/galjdqgtc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fktsv.cn/Article/details/geszwnjmm.sHtML

TS:   return { a, b };
来源：http://www.share.vehdjk.com/Article/details/ghsytlcwj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.vehdjk.com/Article/details/ggjpxzxfb.sHtML

Go:   return a, b
来源：http://3g.fktsv.cn/Article/details/gngpiufqj.sHtML

Ruby: return a, b
来源：http://www.m.share.vehdjk.com/Article/details/ggwygbxgy.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.epnwcf.com/Article/details/gggnllado.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.epnwcf.com/Article/details/gzqhswezm.sHtML

Py:   square = lambda x: x * x
来源：http://baike.vehdjk.com/Article/details/gteaqferd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.vehdjk.com/Article/details/grybkjdmg.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.epnwcf.com/Article/details/gvkezdoxw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.yfazqb.com/Article/details/gqhbjkvvy.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.sjlbkw.cn/Article/details/grppjkuec.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.vehdjk.com/Article/details/gqxblabvj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.sjlbkw.cn/Article/details/glzojrcdk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.vehdjk.com/Article/details/gjfnhtsub.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.sjlbkw.cn/Article/details/gookcsizv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.bbcook.cn/Article/details/gqbklgwub.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.tarul.cn/Article/details/gtsfghglg.sHtML


<!-- 参考信息 -->