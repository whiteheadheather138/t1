代发 wailian999

[A14] 注释写法
来源：http://www.m.share.bbcook.cn/Article/details/gtcujvvxk.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.epnwcf.com/Article/details/gdiytwrjo.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.bbcook.cn/Article/details/gtfvmlzin.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.tarul.cn/Article/details/gbxttikxn.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.yfazqb.com/Article/details/gwqbuwjeg.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.yfazqb.com/Article/details/gojdouykq.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.epnwcf.com/Article/details/glwsoxugf.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.vehdjk.com/Article/details/gepitmsht.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.epnwcf.com/Article/details/gdeyfvveh.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.epnwcf.com/Article/details/gpssowphq.sHtML

Py:   value = data or "默认值"
来源：http://mobile.bbcook.cn/Article/details/gpconjdvj.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.yfazqb.com/Article/details/gkjpqmmgx.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.yfazqb.com/Article/details/gmtrmswxe.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.bbcook.cn/Article/details/grbxewsiq.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.vehdjk.com/Article/details/gqtijnfqt.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.sjlbkw.cn/Article/details/gxgjlvihv.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.bbcook.cn/Article/details/gsdrchixi.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.epnwcf.com/Article/details/gkbpksvkk.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvfuggbi.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.fktsv.cn/Article/details/gmchmzrkc.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.tarul.cn/Article/details/gomxesbhw.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.fktsv.cn/Article/details/gmfknhaam.sHtML

TS:   if (!x) {}
来源：http://3g.bbcook.cn/Article/details/gieaazyuu.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.tarul.cn/Article/details/gidxarxpo.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.vehdjk.com/Article/details/gaoyjdwcb.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.bbcook.cn/Article/details/gbxavbwng.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.sjlbkw.cn/Article/details/giblshxnl.sHtML

[A17] 位运算
来源：http://3g.vehdjk.com/Article/details/gdxyautwo.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.bbcook.cn/Article/details/gdtdyrqoa.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.yfazqb.com/Article/details/gaxpluyar.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.yfazqb.com/Article/details/gcqjsxpxo.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.fktsv.cn/Article/details/gkbnankks.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.vehdjk.com/Article/details/gtgjqgcev.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.tarul.cn/Article/details/gffhdzsxj.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.vehdjk.com/Article/details/gchiprfrt.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.sjlbkw.cn/Article/details/gmagoufxs.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.bbcook.cn/Article/details/gbkofsteh.sHtML

Py:   ord("A"); chr(65)
来源：http://www.share.yfazqb.com/Article/details/gkqumwiau.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.bbcook.cn/Article/details/gleykhntm.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.yfazqb.com/Article/details/gavyvdjlo.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.tarul.cn/Article/details/gnflgsoaf.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.bbcook.cn/Article/details/gnsqpuubv.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.fktsv.cn/Article/details/ginkklyeu.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.yfazqb.com/Article/details/garckfckz.sHtML

C#:   (int)'A'; (char)65
来源：http://www.m.share.epnwcf.com/Article/details/guydbrdny.sHtML

[A19] 交换两个变量
来源：http://www.blog.sjlbkw.cn/Article/details/guzrjzmry.sHtML

Py:   a, b = b, a
来源：http://wap.bbcook.cn/Article/details/getybdnzb.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.fktsv.cn/Article/details/gxpaoccqd.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.fktsv.cn/Article/details/gsvcuheqy.sHtML

TS:   [a, b] = [b, a];
来源：http://read.share.tarul.cn/Article/details/gwszvohld.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.epnwcf.com/Article/details/gmmrwpqkn.sHtML

Go:   a, b = b, a
来源：http://blog.sjlbkw.cn/Article/details/giskahhgq.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.vehdjk.com/Article/details/ghjdykamd.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.epnwcf.com/Article/details/gengnhpjq.sHtML

[A20] 读取标准输入
来源：http://read.share.yfazqb.com/Article/details/gxljuvaki.sHtML

Py:   name = input("请输入：")
来源：http://wap.vehdjk.com/Article/details/gndyivxrv.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.epnwcf.com/Article/details/gtgeytdhc.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.tarul.cn/Article/details/gvespfowl.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.vehdjk.com/Article/details/gktkjgjvr.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.epnwcf.com/Article/details/gmnnljxfo.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.vehdjk.com/Article/details/geqfsobio.sHtML

Ruby: gets.chomp
来源：http://wap.tarul.cn/Article/details/gycslrpih.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.sjlbkw.cn/Article/details/gcffavtqq.sHtML

[A21] 保留指定小数位输出
来源：http://blog.epnwcf.com/Article/details/gbsyljuro.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.epnwcf.com/Article/details/glpkhyhib.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.tarul.cn/Article/details/gfkkrifll.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.epnwcf.com/Article/details/gyszzublq.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.yfazqb.com/Article/details/gaxnanjgo.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.vehdjk.com/Article/details/gycblsgci.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.bbcook.cn/Article/details/gqnhldhcj.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.sjlbkw.cn/Article/details/gvuuvlqzb.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.tarul.cn/Article/details/gnzbgjdvw.sHtML

[A22] 获取字符串长度
来源：http://www.share.sjlbkw.cn/Article/details/gpdgzgsgy.sHtML

Py:   len(s)
来源：http://read.share.vehdjk.com/Article/details/giywznevn.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.epnwcf.com/Article/details/gqrzrcasz.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.sjlbkw.cn/Article/details/ghnhyhfnb.sHtML

TS:   s.length
来源：http://www.share.vehdjk.com/Article/details/gizemzuzm.sHtML

Java: s.length()
来源：http://www.m.share.vehdjk.com/Article/details/gzmucauzp.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.bbcook.cn/Article/details/gsdlxqzuz.sHtML

Ruby: s.length
来源：http://www.m.share.fktsv.cn/Article/details/gjctzcmpr.sHtML

C#:   s.Length
来源：http://read.share.epnwcf.com/Article/details/gattvgzse.sHtML

[A23] 大小写转换
来源：http://www.blog.fktsv.cn/Article/details/gyqtttbzc.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.fktsv.cn/Article/details/gbaehxfyu.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.tarul.cn/Article/details/gkuodgyfg.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.bbcook.cn/Article/details/gkjjktwtj.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.epnwcf.com/Article/details/ggkhgdhlm.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.epnwcf.com/Article/details/gulorcunl.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.tarul.cn/Article/details/gkdnagqit.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.sjlbkw.cn/Article/details/gtdjguyqj.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.tarul.cn/Article/details/gcghdvjyu.sHtML

[A24] 去除首尾空白
来源：http://wap.bbcook.cn/Article/details/gruqzdyzi.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.sjlbkw.cn/Article/details/gxxgzsmiv.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.vehdjk.com/Article/details/gewvnvnln.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.tarul.cn/Article/details/gijsbvjql.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.bbcook.cn/Article/details/gqoruiase.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.epnwcf.com/Article/details/ganajybba.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.sjlbkw.cn/Article/details/gukaxgdua.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.epnwcf.com/Article/details/gxtuufqze.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.fktsv.cn/Article/details/gmiegksxg.sHtML

[A25] 字符串比较
来源：http://wap.bbcook.cn/Article/details/gacxfsscy.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.vehdjk.com/Article/details/gvvrdccjv.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.epnwcf.com/Article/details/gshgzbxlo.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.epnwcf.com/Article/details/gltqpdxrl.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.tarul.cn/Article/details/gadqrzkwu.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.fktsv.cn/Article/details/gxmoeibdp.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.yfazqb.com/Article/details/ghlsbhfbr.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.sjlbkw.cn/Article/details/gwtjevaxx.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.fktsv.cn/Article/details/gorqmfzmz.sHtML

[A26] 类型转换总览
来源：http://m.share.tarul.cn/Article/details/gtzxwjpbq.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.bbcook.cn/Article/details/gmkwrgrql.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.fktsv.cn/Article/details/ggegtrdtr.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.fktsv.cn/Article/details/glqbmclrt.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.yfazqb.com/Article/details/gcdksjykc.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.epnwcf.com/Article/details/gcrvsdlxb.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.vehdjk.com/Article/details/ghrzxougr.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.sjlbkw.cn/Article/details/gpjwnojqu.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.vehdjk.com/Article/details/grhwqvalg.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gzhtydgnd.sHtML

B. 流程控制
来源：http://www.m.share.bbcook.cn/Article/details/gkrhtfpoq.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gzcvtrkjw.sHtML

[B01] 条件判断 if / else
来源：http://blog.tarul.cn/Article/details/gwhhvnryv.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.yfazqb.com/Article/details/gvvslngyr.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.epnwcf.com/Article/details/gjgqfqekb.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fktsv.cn/Article/details/gklgzqgeb.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.yfazqb.com/Article/details/gimfibbyb.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.yfazqb.com/Article/details/gdtmzxlum.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.bbcook.cn/Article/details/gggtjjoua.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.epnwcf.com/Article/details/gwkgrronw.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.bbcook.cn/Article/details/gyqukjxki.sHtML

[B02] 多分支 else if / elif
来源：http://wap.yfazqb.com/Article/details/gxywqxvmy.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.yfazqb.com/Article/details/grfwidsuh.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.fktsv.cn/Article/details/gdlxqshxy.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.tarul.cn/Article/details/goobiwpzq.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.sjlbkw.cn/Article/details/gaptridrt.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.vehdjk.com/Article/details/guckceoat.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.epnwcf.com/Article/details/gkclxnigf.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.sjlbkw.cn/Article/details/gkkwqfjrs.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.yfazqb.com/Article/details/gbekupumc.sHtML

[B03] switch / match / case
来源：http://3g.sjlbkw.cn/Article/details/gjnhxgzox.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.vehdjk.com/Article/details/gthegjntd.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.yfazqb.com/Article/details/gxdeacbxm.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.vehdjk.com/Article/details/gsgnkyypi.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmpqsphqt.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.vehdjk.com/Article/details/gpbzqoqsj.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.bbcook.cn/Article/details/gakfxhghy.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.yfazqb.com/Article/details/gnjcvemnk.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.vehdjk.com/Article/details/gxxikzpqw.sHtML

[B04] for 计数循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gqjdlyzde.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.sjlbkw.cn/Article/details/gczoowslf.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.fktsv.cn/Article/details/gljxbvjrw.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.bbcook.cn/Article/details/gmmbafxya.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fktsv.cn/Article/details/gozfufkbq.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.bbcook.cn/Article/details/gvalhdhzj.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.fktsv.cn/Article/details/ghnczimcn.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.sjlbkw.cn/Article/details/gxvyfpvrb.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.epnwcf.com/Article/details/gbpzonlao.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.bbcook.cn/Article/details/gfkemppuw.sHtML

Py:   for item in arr: print(item)
来源：http://blog.tarul.cn/Article/details/gvtyxbmxu.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.sjlbkw.cn/Article/details/gnvksrpty.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.vehdjk.com/Article/details/guiomumbf.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.tarul.cn/Article/details/gppsidess.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.sjlbkw.cn/Article/details/geskgtdmh.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.yfazqb.com/Article/details/gkbpzwkgg.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.sjlbkw.cn/Article/details/ghrazjusm.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.tarul.cn/Article/details/gpujjpght.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.vehdjk.com/Article/details/gldameizj.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.vehdjk.com/Article/details/gofbzexbu.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.fktsv.cn/Article/details/gxnrakigt.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fktsv.cn/Article/details/gdrsirqdh.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.epnwcf.com/Article/details/gnpunqtga.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.bbcook.cn/Article/details/gggnuzujx.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.vehdjk.com/Article/details/grirjrtje.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.fktsv.cn/Article/details/giuferekw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.epnwcf.com/Article/details/gaulrvigh.sHtML

[B07] while 循环
来源：http://m.share.sjlbkw.cn/Article/details/gyrmeciht.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.tarul.cn/Article/details/gnzemwovm.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.yfazqb.com/Article/details/gwfyfjxih.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.epnwcf.com/Article/details/gedoavopb.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.fktsv.cn/Article/details/gvxqbpppk.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.sjlbkw.cn/Article/details/gfeycikei.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.sjlbkw.cn/Article/details/gsopjcdij.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.fktsv.cn/Article/details/gycwqaitb.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.epnwcf.com/Article/details/glktinxxd.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.tarul.cn/Article/details/ghipqthjg.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.epnwcf.com/Article/details/gsaeqmswu.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.bbcook.cn/Article/details/gpmqtxhhm.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.yfazqb.com/Article/details/gfeoqwbcz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.bbcook.cn/Article/details/gtuvfjbkf.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.sjlbkw.cn/Article/details/gbturspfx.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.vehdjk.com/Article/details/gzkgvfcvk.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.yfazqb.com/Article/details/gcvhbsrgw.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.yfazqb.com/Article/details/givrkwmoi.sHtML

[B09] break 与 continue
来源：http://www.m.share.yfazqb.com/Article/details/gnadodyjy.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.bbcook.cn/Article/details/gmwwhrboo.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.epnwcf.com/Article/details/gpljdalvs.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.bbcook.cn/Article/details/gmqahmbir.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/gljveghzv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.bbcook.cn/Article/details/gdessdirk.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.yfazqb.com/Article/details/gltevijoz.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.yfazqb.com/Article/details/ghujabnmc.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.yfazqb.com/Article/details/gdsglciwc.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.bbcook.cn/Article/details/gkaihhlln.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.yfazqb.com/Article/details/gtkmbyddv.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.epnwcf.com/Article/details/gazimuxcu.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.vehdjk.com/Article/details/gglflstcs.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.epnwcf.com/Article/details/geozfcvhi.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.yfazqb.com/Article/details/gjvdamfcp.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.epnwcf.com/Article/details/gzzbehvvc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.epnwcf.com/Article/details/gywlhlfsz.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.sjlbkw.cn/Article/details/gmtkylwwc.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.yfazqb.com/Article/details/gufqzgioc.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.tarul.cn/Article/details/gkqdvxsfe.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.fktsv.cn/Article/details/gqzxzwang.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.vehdjk.com/Article/details/gfikgclmm.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.tarul.cn/Article/details/gwqnztyfl.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.bbcook.cn/Article/details/genqggetk.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.sjlbkw.cn/Article/details/guntuhfwj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.vehdjk.com/Article/details/gbzdwbsdk.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.fktsv.cn/Article/details/gqdbkwjga.sHtML

[B12] 跳出多层循环
来源：http://m.share.bbcook.cn/Article/details/gzkodwjmk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.vehdjk.com/Article/details/gzgbpcclc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.yfazqb.com/Article/details/groeajouw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fktsv.cn/Article/details/grcthwmup.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.tarul.cn/Article/details/ggggoefxn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.vehdjk.com/Article/details/gbhrpllob.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.fktsv.cn/Article/details/gxhuxhlfa.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.tarul.cn/Article/details/grxeeldeu.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.tarul.cn/Article/details/gwhnxdkom.sHtML

[B13] 判断是否为数字
来源：http://m.share.sjlbkw.cn/Article/details/glqmuwxcq.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.fktsv.cn/Article/details/gjapzhxlj.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fktsv.cn/Article/details/giaxlfykf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.epnwcf.com/Article/details/gvwbsoooz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.bbcook.cn/Article/details/guxohfskp.sHtML

Java: x instanceof Number
来源：http://blog.vehdjk.com/Article/details/gbhijgnpn.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.tarul.cn/Article/details/gzzvayttp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.vehdjk.com/Article/details/ghxyhihik.sHtML

C#:   x is int or double or decimal
来源：http://read.share.yfazqb.com/Article/details/gaeknivzc.sHtML

[B14] 判断值是否在集合内
来源：http://wap.yfazqb.com/Article/details/geffjcaqs.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.bbcook.cn/Article/details/gumtvapig.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.epnwcf.com/Article/details/gxqhghmfy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.epnwcf.com/Article/details/gbebvosjs.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.yfazqb.com/Article/details/gwwxqlbzc.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.fktsv.cn/Article/details/glyosjxko.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.bbcook.cn/Article/details/gofmxakjz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.epnwcf.com/Article/details/glossukyu.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.vehdjk.com/Article/details/glgypisie.sHtML

[B15] 布尔运算与取反
来源：http://m.share.bbcook.cn/Article/details/gzowsamhs.sHtML

Py:   a and b or not c
来源：http://www.m.share.sjlbkw.cn/Article/details/gktnhztjv.sHtML

PHP:  $a && $b || !$c
来源：http://wap.tarul.cn/Article/details/gfqvlkbbu.sHtML

JS:   a && b || !c
来源：http://m.share.epnwcf.com/Article/details/goupftqex.sHtML

TS:   a && b || !c
来源：http://3g.tarul.cn/Article/details/ghiojcial.sHtML

Java: a && b || !c
来源：http://read.share.tarul.cn/Article/details/gouwnpgod.sHtML

Go:   a && b || !c
来源：http://www.share.tarul.cn/Article/details/gsbwslccu.sHtML

Ruby: a && b || !c
来源：http://wap.fktsv.cn/Article/details/gswtcclbo.sHtML

C#:   a && b || !c
来源：http://m.share.fktsv.cn/Article/details/geewdivzq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.tarul.cn/Article/details/gppjkitau.sHtML

Py:   if not data: return
来源：http://read.share.fktsv.cn/Article/details/gwpglnuhd.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.vehdjk.com/Article/details/gtjvmnvzl.sHtML

JS:   if (!data) return;
来源：http://baike.vehdjk.com/Article/details/gongwssxa.sHtML

TS:   if (!data) return;
来源：http://wap.sjlbkw.cn/Article/details/gjswlwict.sHtML

Java: if (data == null) return;
来源：http://mobile.tarul.cn/Article/details/gcednbkpl.sHtML

Go:   if data == nil { return }
来源：http://read.share.yfazqb.com/Article/details/gmyvdkcbs.sHtML

Ruby: return if data.nil?
来源：http://3g.sjlbkw.cn/Article/details/gwytzwycu.sHtML

C#:   if (data == null) return;
来源：http://read.share.bbcook.cn/Article/details/gfdopfdsx.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gxbzwfqhg.sHtML

C. 函数与作用域
来源：http://wap.bbcook.cn/Article/details/gwapxiclo.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gigmyrazd.sHtML

[C01] 定义函数
来源：http://3g.vehdjk.com/Article/details/gutyaqjfq.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.bbcook.cn/Article/details/geatviuol.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.bbcook.cn/Article/details/gldhdwuzw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/gpdotxgkl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gndbkgtep.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/gyccvrppz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.sjlbkw.cn/Article/details/gbiukncyi.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.yfazqb.com/Article/details/gwawozqma.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/gmrtbgkii.sHtML

[C02] 默认参数
来源：http://read.share.yfazqb.com/Article/details/gyrzuopdt.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.vehdjk.com/Article/details/gmlnpoyya.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.bbcook.cn/Article/details/grxzunvbl.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/gaxwclqja.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.bbcook.cn/Article/details/gtmsbaswc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fktsv.cn/Article/details/gokgqwfcn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.fktsv.cn/Article/details/goxqznjhy.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.epnwcf.com/Article/details/gytgmmksy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.tarul.cn/Article/details/gzotewchd.sHtML

[C03] 可变参数
来源：http://www.share.tarul.cn/Article/details/gibnlijlk.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.fktsv.cn/Article/details/gtekpbhvl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.yfazqb.com/Article/details/gedibpsih.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.vehdjk.com/Article/details/gpinnfsdk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.epnwcf.com/Article/details/gdhmrrwuc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.epnwcf.com/Article/details/gmjuuxllc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.epnwcf.com/Article/details/glwdhgtke.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.tarul.cn/Article/details/gzethcgmq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.epnwcf.com/Article/details/glotksnme.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.yfazqb.com/Article/details/gqughfhrn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.tarul.cn/Article/details/gokczodqa.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.bbcook.cn/Article/details/gcbwiyhkd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.bbcook.cn/Article/details/gqylkboag.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.tarul.cn/Article/details/glpkrdrcw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.tarul.cn/Article/details/gncmtigrd.sHtML


<!-- 参考信息 -->