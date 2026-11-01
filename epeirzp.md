代发 wailian999

Java: "第一行\n第二行"
来源：http://read.share.vehdjk.com/Article/details/gmyaziyfe.sHtML

Go:   "第一行\n第二行"
来源：http://blog.tarul.cn/Article/details/gjrvhzjuo.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.bbcook.cn/Article/details/gorbtipyq.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.tarul.cn/Article/details/gpzyumujq.sHtML

[A14] 注释写法
来源：http://3g.sjlbkw.cn/Article/details/gucwgydpk.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.yfazqb.com/Article/details/gfibxlraz.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.fktsv.cn/Article/details/gnnqdjghx.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.sjlbkw.cn/Article/details/gyihkwprd.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.yfazqb.com/Article/details/gdntlrntu.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.bbcook.cn/Article/details/gercisdci.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.yfazqb.com/Article/details/gicizrqty.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.epnwcf.com/Article/details/gtguhokbu.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.epnwcf.com/Article/details/geebzwztj.sHtML

[A15] 空值判断与默认值
来源：http://mobile.bbcook.cn/Article/details/grbtuhzkn.sHtML

Py:   value = data or "默认值"
来源：http://read.share.epnwcf.com/Article/details/gopgfzcrq.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.tarul.cn/Article/details/gfgdszucr.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.fktsv.cn/Article/details/gmeooivht.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.sjlbkw.cn/Article/details/gfsunfsax.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.tarul.cn/Article/details/glvlcrnvz.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.bbcook.cn/Article/details/ghxdezmbg.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.bbcook.cn/Article/details/gidtepruv.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.bbcook.cn/Article/details/gtsioneep.sHtML

[A16] 真假值判断规则
来源：http://www.share.vehdjk.com/Article/details/glvlunuac.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.vehdjk.com/Article/details/gbyuzghxo.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.tarul.cn/Article/details/glhbsgyto.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.bbcook.cn/Article/details/gufgoxwkh.sHtML

TS:   if (!x) {}
来源：http://baike.sjlbkw.cn/Article/details/gqqsuwfzk.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.fktsv.cn/Article/details/gnyzvphek.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.yfazqb.com/Article/details/gtgulvauu.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.sjlbkw.cn/Article/details/geiuihkcb.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.vehdjk.com/Article/details/grtdizotc.sHtML

[A17] 位运算
来源：http://wap.vehdjk.com/Article/details/ghvvqilck.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.epnwcf.com/Article/details/gkftbgnwn.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.fktsv.cn/Article/details/gcxbbxooh.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.tarul.cn/Article/details/gpipajjud.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.tarul.cn/Article/details/gngxmnzuo.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fktsv.cn/Article/details/gmgzxrahx.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gplqovoyc.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.tarul.cn/Article/details/gjcgdispu.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.sjlbkw.cn/Article/details/gtwredvzu.sHtML

[A18] 字符与 ASCII 码互转
来源：http://m.share.vehdjk.com/Article/details/gvfqsynbg.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.vehdjk.com/Article/details/gmsefawkh.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.epnwcf.com/Article/details/gdfprnmdp.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.yfazqb.com/Article/details/gyutmbcnx.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.vehdjk.com/Article/details/gvinrnvux.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.vehdjk.com/Article/details/gwngvycbl.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.tarul.cn/Article/details/gszfwhqfc.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.bbcook.cn/Article/details/gzrdzmukj.sHtML

C#:   (int)'A'; (char)65
来源：http://wap.yfazqb.com/Article/details/gxditxecf.sHtML

[A19] 交换两个变量
来源：http://mobile.fktsv.cn/Article/details/gkltazakz.sHtML

Py:   a, b = b, a
来源：http://www.blog.fktsv.cn/Article/details/gkmotzwlq.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.bbcook.cn/Article/details/gsqmnygwn.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.bbcook.cn/Article/details/gtmdcmwrv.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.vehdjk.com/Article/details/gdtbmtdqc.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.sjlbkw.cn/Article/details/gosiljxux.sHtML

Go:   a, b = b, a
来源：http://mobile.fktsv.cn/Article/details/gqbrgzqtn.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.vehdjk.com/Article/details/gxbkturdz.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.tarul.cn/Article/details/gkdmexzpu.sHtML

[A20] 读取标准输入
来源：http://blog.fktsv.cn/Article/details/gwminjwae.sHtML

Py:   name = input("请输入：")
来源：http://blog.epnwcf.com/Article/details/gcqkapqqn.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.sjlbkw.cn/Article/details/gwaqvoepz.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.fktsv.cn/Article/details/gxelzfcvc.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.sjlbkw.cn/Article/details/gjgfybpad.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.bbcook.cn/Article/details/ghvuvxabe.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.yfazqb.com/Article/details/gdgbbegjm.sHtML

Ruby: gets.chomp
来源：http://m.share.vehdjk.com/Article/details/gzbjamgkv.sHtML

C#:   Console.ReadLine();
来源：http://3g.bbcook.cn/Article/details/grkwtubvs.sHtML

[A21] 保留指定小数位输出
来源：http://blog.bbcook.cn/Article/details/grubtnikf.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.fktsv.cn/Article/details/goflehnkc.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.yfazqb.com/Article/details/guxtcqwev.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.bbcook.cn/Article/details/ggtbxkgar.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.sjlbkw.cn/Article/details/glzlxzern.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.sjlbkw.cn/Article/details/gsjfvnhfa.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.yfazqb.com/Article/details/gadmiatds.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.vehdjk.com/Article/details/gpavlrnxt.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.fktsv.cn/Article/details/gyautymcu.sHtML

[A22] 获取字符串长度
来源：http://www.share.tarul.cn/Article/details/gasbhlrnj.sHtML

Py:   len(s)
来源：http://baike.tarul.cn/Article/details/gptpqudzx.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.vehdjk.com/Article/details/gcrvjqwnv.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.epnwcf.com/Article/details/glsbrustn.sHtML

TS:   s.length
来源：http://baike.yfazqb.com/Article/details/glzpyacbw.sHtML

Java: s.length()
来源：http://www.share.vehdjk.com/Article/details/gsvjntgbw.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.tarul.cn/Article/details/gpnmshbib.sHtML

Ruby: s.length
来源：http://m.share.epnwcf.com/Article/details/gwmfxsadf.sHtML

C#:   s.Length
来源：http://www.m.share.yfazqb.com/Article/details/grlzflvqj.sHtML

[A23] 大小写转换
来源：http://blog.vehdjk.com/Article/details/ghwlxzuiq.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.bbcook.cn/Article/details/gbzdbzpda.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.epnwcf.com/Article/details/gmuekxmnu.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.epnwcf.com/Article/details/gxumzxduf.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.epnwcf.com/Article/details/gzvvykobo.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.sjlbkw.cn/Article/details/gpvsueydf.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.yfazqb.com/Article/details/gwuvbglzi.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.vehdjk.com/Article/details/glfszdsqp.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.bbcook.cn/Article/details/gbgsbxgft.sHtML

[A24] 去除首尾空白
来源：http://blog.bbcook.cn/Article/details/gjdycgyzj.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.sjlbkw.cn/Article/details/gvmxouxit.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.epnwcf.com/Article/details/geldzodqc.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.tarul.cn/Article/details/glwzhmmmw.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.vehdjk.com/Article/details/gewmkubml.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.epnwcf.com/Article/details/gpfpzdnyx.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.epnwcf.com/Article/details/gojmbcbsz.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.vehdjk.com/Article/details/gflcfnlks.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.sjlbkw.cn/Article/details/gxisdvljg.sHtML

[A25] 字符串比较
来源：http://www.share.fktsv.cn/Article/details/gbbdlswrd.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.epnwcf.com/Article/details/gbsfkcaym.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.vehdjk.com/Article/details/gcigtligf.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.epnwcf.com/Article/details/gchwdnmxk.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.fktsv.cn/Article/details/glxdzcpyd.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.fktsv.cn/Article/details/ghswixlig.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.fktsv.cn/Article/details/gxrdezjkd.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.bbcook.cn/Article/details/gwxaderzc.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.sjlbkw.cn/Article/details/gjdnhragf.sHtML

[A26] 类型转换总览
来源：http://m.share.bbcook.cn/Article/details/gjvwnxiyi.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.epnwcf.com/Article/details/gzfwwqcdc.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.yfazqb.com/Article/details/gvjjvqvuc.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.vehdjk.com/Article/details/ghcplmxox.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.tarul.cn/Article/details/gkyryxnqk.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.vehdjk.com/Article/details/goeanwkls.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.vehdjk.com/Article/details/ghivfdzzq.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.yfazqb.com/Article/details/ghzkadlew.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.vehdjk.com/Article/details/gzzgpncgm.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gaxaeiswu.sHtML

B. 流程控制
来源：http://mobile.sjlbkw.cn/Article/details/gpcxgcnly.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gjlwphknl.sHtML

[B01] 条件判断 if / else
来源：http://mobile.yfazqb.com/Article/details/gqoxagtxx.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.epnwcf.com/Article/details/gumjhivnp.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.vehdjk.com/Article/details/glpgyofqf.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.sjlbkw.cn/Article/details/gteutfkom.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.yfazqb.com/Article/details/gyfpvrchh.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.vehdjk.com/Article/details/gjuziywhl.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.yfazqb.com/Article/details/gzgplqvjq.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.vehdjk.com/Article/details/gbmpriqpx.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.tarul.cn/Article/details/gqjcytyxk.sHtML

[B02] 多分支 else if / elif
来源：http://wap.vehdjk.com/Article/details/gnhyungmh.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.bbcook.cn/Article/details/gddjnaicu.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.tarul.cn/Article/details/gdgyvvwrx.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.bbcook.cn/Article/details/getkacexu.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.sjlbkw.cn/Article/details/gfwdvoqpx.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.epnwcf.com/Article/details/gqzfbebvv.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.bbcook.cn/Article/details/gtedqfhlm.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.fktsv.cn/Article/details/gsnfyglnk.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.vehdjk.com/Article/details/giqtyrnge.sHtML

[B03] switch / match / case
来源：http://baike.sjlbkw.cn/Article/details/gmwcenemh.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.epnwcf.com/Article/details/gpvrvrmns.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.bbcook.cn/Article/details/gyatcoyml.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.vehdjk.com/Article/details/gpujfffda.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.yfazqb.com/Article/details/gmjrnwmyf.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.fktsv.cn/Article/details/gvqaljsdq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.fktsv.cn/Article/details/gikqsxvww.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.sjlbkw.cn/Article/details/gonktiiys.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.bbcook.cn/Article/details/ghhimfaie.sHtML

[B04] for 计数循环
来源：http://m.share.tarul.cn/Article/details/grbraqapt.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.tarul.cn/Article/details/gmynmfzqo.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.yfazqb.com/Article/details/gurtyktam.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.bbcook.cn/Article/details/gkwjirsfc.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.bbcook.cn/Article/details/ggbrsdihl.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.yfazqb.com/Article/details/gawftksey.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.fktsv.cn/Article/details/gmidguhhq.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.yfazqb.com/Article/details/gyjtqlyqj.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.epnwcf.com/Article/details/gonnppyto.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.tarul.cn/Article/details/gskxhkede.sHtML

Py:   for item in arr: print(item)
来源：http://blog.bbcook.cn/Article/details/glsntagls.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.sjlbkw.cn/Article/details/gjvxuvpnx.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.fktsv.cn/Article/details/ghfwdlgyo.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.epnwcf.com/Article/details/ghzaautbb.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.vehdjk.com/Article/details/gcrmykvwp.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.yfazqb.com/Article/details/gineohbni.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.sjlbkw.cn/Article/details/gwabdjahp.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.tarul.cn/Article/details/gzjzqkdyi.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.epnwcf.com/Article/details/gfbnwcwmp.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.fktsv.cn/Article/details/glgbzdbyq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.fktsv.cn/Article/details/giucellid.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.yfazqb.com/Article/details/gcixidvkd.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.tarul.cn/Article/details/ggjlqnovm.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.sjlbkw.cn/Article/details/gfkxxqdua.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.bbcook.cn/Article/details/gamprsuuy.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.tarul.cn/Article/details/gcypqrczm.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.tarul.cn/Article/details/gnobrhbzi.sHtML

[B07] while 循环
来源：http://read.share.bbcook.cn/Article/details/grgpiqouy.sHtML

Py:   while i < 10: i += 1
来源：http://baike.tarul.cn/Article/details/gbcgczdrp.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.epnwcf.com/Article/details/gsakgbonv.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.bbcook.cn/Article/details/gpglxntco.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.fktsv.cn/Article/details/gmpdfefgv.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.fktsv.cn/Article/details/gccaaonqr.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.fktsv.cn/Article/details/gtehiufrj.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.epnwcf.com/Article/details/gjckoljpg.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.vehdjk.com/Article/details/gmuxsapwj.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.tarul.cn/Article/details/gjeukttnn.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.sjlbkw.cn/Article/details/glhaocyje.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.vehdjk.com/Article/details/gdngbxwnu.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.yfazqb.com/Article/details/ggqngezkr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.epnwcf.com/Article/details/gmkjamyod.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.tarul.cn/Article/details/gzrwhzrda.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.bbcook.cn/Article/details/gobupxrxl.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.epnwcf.com/Article/details/gtaqqhzzr.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.vehdjk.com/Article/details/gneaoebjz.sHtML

[B09] break 与 continue
来源：http://baike.fktsv.cn/Article/details/gkpvigsfo.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.epnwcf.com/Article/details/gysmdeaji.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.tarul.cn/Article/details/ghrnhmpkm.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fktsv.cn/Article/details/gsmhnknsi.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.vehdjk.com/Article/details/gyyxcamgv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.bbcook.cn/Article/details/gncusqxxk.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gevnpbvtp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghblqjtof.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.sjlbkw.cn/Article/details/gbyyydwnn.sHtML

[B10] 遍历同时拿索引
来源：http://3g.yfazqb.com/Article/details/gwrmsljom.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.sjlbkw.cn/Article/details/gpzlggolo.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.vehdjk.com/Article/details/gjtisswdh.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.sjlbkw.cn/Article/details/gxkdqsfym.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.tarul.cn/Article/details/gpqxauyod.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.sjlbkw.cn/Article/details/gtuugrsnw.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.tarul.cn/Article/details/ggekzvlun.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.fktsv.cn/Article/details/gnnwqmtsu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.epnwcf.com/Article/details/glhtfifli.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.tarul.cn/Article/details/gpvqfopos.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.fktsv.cn/Article/details/gogkckkzi.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.epnwcf.com/Article/details/gmbrzolfi.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fktsv.cn/Article/details/gpnfclzvt.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.tarul.cn/Article/details/gqhtvztpv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.tarul.cn/Article/details/gkzswuugg.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.bbcook.cn/Article/details/gdhifgoyg.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.bbcook.cn/Article/details/glkmkiset.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.fktsv.cn/Article/details/gmnxzwgxs.sHtML

[B12] 跳出多层循环
来源：http://baike.bbcook.cn/Article/details/ginmpaupx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.sjlbkw.cn/Article/details/gfpgjtksx.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.sjlbkw.cn/Article/details/ghtodhrlh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.vehdjk.com/Article/details/gfakldfwx.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.epnwcf.com/Article/details/gioncdsti.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.tarul.cn/Article/details/gmkmhlofu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.bbcook.cn/Article/details/ggnswcbbr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.bbcook.cn/Article/details/gfdgwdgjq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.bbcook.cn/Article/details/gxitjfckc.sHtML

[B13] 判断是否为数字
来源：http://www.blog.tarul.cn/Article/details/grppgmssr.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.yfazqb.com/Article/details/geiznymyy.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.vehdjk.com/Article/details/gfqguprro.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.vehdjk.com/Article/details/gthpiodkh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.bbcook.cn/Article/details/gyyevdleo.sHtML

Java: x instanceof Number
来源：http://www.blog.sjlbkw.cn/Article/details/gagsgnfyv.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.yfazqb.com/Article/details/glqioapxa.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.epnwcf.com/Article/details/gmlaqgcyu.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.epnwcf.com/Article/details/ggggrqimp.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.yfazqb.com/Article/details/gklfvnckv.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.vehdjk.com/Article/details/gdllyjvli.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.vehdjk.com/Article/details/gmhqemrsn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.bbcook.cn/Article/details/gpkvzguql.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.yfazqb.com/Article/details/ggmfknydw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fktsv.cn/Article/details/gczthadjr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.tarul.cn/Article/details/gmfzcgomd.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.tarul.cn/Article/details/glzskdlel.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.bbcook.cn/Article/details/gakeuxkhq.sHtML

[B15] 布尔运算与取反
来源：http://m.share.vehdjk.com/Article/details/gwtcnfcvq.sHtML

Py:   a and b or not c
来源：http://m.share.yfazqb.com/Article/details/gutmdwwzh.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.yfazqb.com/Article/details/gxhwnisjb.sHtML

JS:   a && b || !c
来源：http://mobile.yfazqb.com/Article/details/gmdxgbfzu.sHtML

TS:   a && b || !c
来源：http://mobile.tarul.cn/Article/details/gocxuqgam.sHtML

Java: a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/gnakiaxsy.sHtML

Go:   a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gonmrikbb.sHtML

Ruby: a && b || !c
来源：http://baike.epnwcf.com/Article/details/gybugcccg.sHtML

C#:   a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gfjpjoemp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.bbcook.cn/Article/details/gglgkefdq.sHtML

Py:   if not data: return
来源：http://baike.tarul.cn/Article/details/gididncaf.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.fktsv.cn/Article/details/gzqeqseam.sHtML

JS:   if (!data) return;
来源：http://m.share.yfazqb.com/Article/details/gvbfuwddg.sHtML

TS:   if (!data) return;
来源：http://www.share.yfazqb.com/Article/details/gxdtwetoh.sHtML

Java: if (data == null) return;
来源：http://m.share.bbcook.cn/Article/details/gsvfjcbzf.sHtML

Go:   if data == nil { return }
来源：http://3g.sjlbkw.cn/Article/details/gdsxjmsnt.sHtML

Ruby: return if data.nil?
来源：http://3g.bbcook.cn/Article/details/gdjhdrvjs.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.epnwcf.com/Article/details/gmbhctrip.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gmomouesw.sHtML

C. 函数与作用域
来源：http://3g.bbcook.cn/Article/details/gtbclfrqp.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gegxxpovv.sHtML

[C01] 定义函数
来源：http://blog.sjlbkw.cn/Article/details/gtkadwqie.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.sjlbkw.cn/Article/details/gdegtogil.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.vehdjk.com/Article/details/gkynspvlc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.epnwcf.com/Article/details/gkezzarpu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gtnsfbauh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.vehdjk.com/Article/details/gygwklxae.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.sjlbkw.cn/Article/details/gntspnugq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.epnwcf.com/Article/details/gvrkzeumt.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/geyesidqz.sHtML

[C02] 默认参数
来源：http://mobile.vehdjk.com/Article/details/gpfndldub.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.epnwcf.com/Article/details/gsoaozrbl.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.yfazqb.com/Article/details/gelebmctn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fktsv.cn/Article/details/gefjjaxvf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fktsv.cn/Article/details/grjokcord.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.sjlbkw.cn/Article/details/gwwiwjjzj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.vehdjk.com/Article/details/ghuhxrzpz.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.yfazqb.com/Article/details/gjmbycahs.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.tarul.cn/Article/details/gwixepszz.sHtML

[C03] 可变参数
来源：http://www.blog.bbcook.cn/Article/details/gcherbfdx.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.vehdjk.com/Article/details/gfecutqsw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.tarul.cn/Article/details/gqiiurrhs.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.bbcook.cn/Article/details/gxufjobmb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.vehdjk.com/Article/details/gvyuinedk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.sjlbkw.cn/Article/details/gfdkjwvbb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.yfazqb.com/Article/details/gdwqhswkq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.bbcook.cn/Article/details/gfjwywxxk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.vehdjk.com/Article/details/gutclokou.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.yfazqb.com/Article/details/gpfzbkzyl.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fktsv.cn/Article/details/gskccscpy.sHtML


<!-- 参考信息 -->