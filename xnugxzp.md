代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://m.share.epnwcf.com/Article/details/gaqpqbdmk.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.vehdjk.com/Article/details/gfiizuxrs.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.sjlbkw.cn/Article/details/givgtvxoz.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.vehdjk.com/Article/details/gzjikbqtg.sHtML

Ruby: value = data || "默认值"
来源：http://wap.epnwcf.com/Article/details/gfqikvbek.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.yfazqb.com/Article/details/gtrqcsvcf.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.fktsv.cn/Article/details/gqzcfgjpj.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.sjlbkw.cn/Article/details/gqknreutt.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.tarul.cn/Article/details/goguovete.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.yfazqb.com/Article/details/gnzdwldqe.sHtML

TS:   if (!x) {}
来源：http://m.share.fktsv.cn/Article/details/gzjuhikkw.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.yfazqb.com/Article/details/gryyenpvz.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.bbcook.cn/Article/details/gsavvwkdi.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.epnwcf.com/Article/details/gmerkuupi.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.fktsv.cn/Article/details/gtxgzakcn.sHtML

[A17] 位运算
来源：http://3g.tarul.cn/Article/details/ghkyyqujo.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fktsv.cn/Article/details/gvpjcfsny.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.tarul.cn/Article/details/gjtgploej.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.tarul.cn/Article/details/grykyanig.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.yfazqb.com/Article/details/grjuaiuzz.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.tarul.cn/Article/details/gnemdeeez.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.yfazqb.com/Article/details/gypdyaope.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fktsv.cn/Article/details/glebbmyog.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.yfazqb.com/Article/details/gjrengobm.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.yfazqb.com/Article/details/gfecsfmzf.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.tarul.cn/Article/details/gfkopcaiv.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.bbcook.cn/Article/details/gbivtkyhr.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.sjlbkw.cn/Article/details/gccqsthfj.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.fktsv.cn/Article/details/gdjzorskw.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.vehdjk.com/Article/details/ghrdpqvkv.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.vehdjk.com/Article/details/gtqzvyyjp.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.yfazqb.com/Article/details/gkmcruyia.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.epnwcf.com/Article/details/gxjvfsgja.sHtML

[A19] 交换两个变量
来源：http://mobile.vehdjk.com/Article/details/gmkidxwee.sHtML

Py:   a, b = b, a
来源：http://www.share.sjlbkw.cn/Article/details/gaekchxlc.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.vehdjk.com/Article/details/ggqardfsj.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.yfazqb.com/Article/details/gmlpgxgil.sHtML

TS:   [a, b] = [b, a];
来源：http://read.share.fktsv.cn/Article/details/gecnalkvi.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.vehdjk.com/Article/details/gijwbtxyu.sHtML

Go:   a, b = b, a
来源：http://baike.epnwcf.com/Article/details/gvpafcbph.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.vehdjk.com/Article/details/gugpgehtv.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.bbcook.cn/Article/details/guhyadhax.sHtML

[A20] 读取标准输入
来源：http://baike.bbcook.cn/Article/details/gpciicoaf.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.vehdjk.com/Article/details/gtmsavzog.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.vehdjk.com/Article/details/ghoiyqmug.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.yfazqb.com/Article/details/gogyphqcd.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.tarul.cn/Article/details/gzmzelcwq.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.yfazqb.com/Article/details/giyffvnix.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.bbcook.cn/Article/details/gglsklzdf.sHtML

Ruby: gets.chomp
来源：http://baike.tarul.cn/Article/details/gkmlegdoc.sHtML

C#:   Console.ReadLine();
来源：http://mobile.fktsv.cn/Article/details/gafhvjrfc.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.bbcook.cn/Article/details/gvuohwlzu.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.sjlbkw.cn/Article/details/gywyjfioz.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.bbcook.cn/Article/details/gbowubhwf.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.epnwcf.com/Article/details/gyqtgxcsu.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.sjlbkw.cn/Article/details/gdaohfnuw.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.yfazqb.com/Article/details/gucbykwuu.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.tarul.cn/Article/details/ghyexoeih.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.yfazqb.com/Article/details/gzjgbtgcg.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.vehdjk.com/Article/details/gqzurutoa.sHtML

[A22] 获取字符串长度
来源：http://blog.vehdjk.com/Article/details/gcrtsnacq.sHtML

Py:   len(s)
来源：http://www.share.fktsv.cn/Article/details/gfqvmnzxv.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.vehdjk.com/Article/details/gvvjxryot.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.yfazqb.com/Article/details/gtsspzhox.sHtML

TS:   s.length
来源：http://www.blog.tarul.cn/Article/details/gmgdqzekp.sHtML

Java: s.length()
来源：http://read.share.sjlbkw.cn/Article/details/gambegkpl.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.sjlbkw.cn/Article/details/gsuhzmaeg.sHtML

Ruby: s.length
来源：http://mobile.yfazqb.com/Article/details/geaffqqof.sHtML

C#:   s.Length
来源：http://read.share.bbcook.cn/Article/details/gbahvuktt.sHtML

[A23] 大小写转换
来源：http://blog.yfazqb.com/Article/details/gumrdmhil.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.tarul.cn/Article/details/gfaminqyv.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.tarul.cn/Article/details/gppcwgvzz.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fktsv.cn/Article/details/gnruxaiof.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.vehdjk.com/Article/details/gbvpkdjjy.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.sjlbkw.cn/Article/details/gmbcgbjnf.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.vehdjk.com/Article/details/gsvhjfyln.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.epnwcf.com/Article/details/ggbxktati.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.epnwcf.com/Article/details/gasxsqcbz.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.tarul.cn/Article/details/glwnicddp.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.fktsv.cn/Article/details/gxhpgwjay.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.bbcook.cn/Article/details/gxfuxthrp.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.vehdjk.com/Article/details/gmvjbwfci.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.tarul.cn/Article/details/gxpevhzli.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.fktsv.cn/Article/details/gqgiiaiaw.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.yfazqb.com/Article/details/gbeggtdto.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.tarul.cn/Article/details/gaeafxnpb.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.sjlbkw.cn/Article/details/goqyrnpzs.sHtML

[A25] 字符串比较
来源：http://baike.vehdjk.com/Article/details/gjjeqqdij.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.fktsv.cn/Article/details/goyiwxxcw.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.vehdjk.com/Article/details/gvhgsodnt.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.sjlbkw.cn/Article/details/gltxgqnse.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.sjlbkw.cn/Article/details/gzjhezmra.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.epnwcf.com/Article/details/guprrsden.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.fktsv.cn/Article/details/gfbvleomc.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.epnwcf.com/Article/details/gjiaokkib.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.sjlbkw.cn/Article/details/gejulxxdj.sHtML

[A26] 类型转换总览
来源：http://mobile.epnwcf.com/Article/details/gpospqttu.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.epnwcf.com/Article/details/gcivhrydq.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.fktsv.cn/Article/details/gzzcgsash.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.sjlbkw.cn/Article/details/gwacxaupf.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.tarul.cn/Article/details/gienfuwja.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.bbcook.cn/Article/details/gtlqifcms.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.sjlbkw.cn/Article/details/gcaqozyks.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.epnwcf.com/Article/details/guklsasvc.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.yfazqb.com/Article/details/gmjieizei.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gplilcjgw.sHtML

B. 流程控制
来源：http://www.share.fktsv.cn/Article/details/gajppjftn.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/ghwlkzpfk.sHtML

[B01] 条件判断 if / else
来源：http://3g.sjlbkw.cn/Article/details/gzkjcgwpd.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.fktsv.cn/Article/details/gsjhzjekn.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.sjlbkw.cn/Article/details/gxgujmpqr.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fktsv.cn/Article/details/ggyviruht.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.bbcook.cn/Article/details/gfiosiayz.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.yfazqb.com/Article/details/gmpoisjhb.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.fktsv.cn/Article/details/gxpayyeip.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.fktsv.cn/Article/details/gxvvlermg.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.fktsv.cn/Article/details/gzsdjozro.sHtML

[B02] 多分支 else if / elif
来源：http://3g.bbcook.cn/Article/details/gpdubvzoo.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.fktsv.cn/Article/details/gknlvbtzg.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.yfazqb.com/Article/details/gcducvyyp.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.tarul.cn/Article/details/gonzcsibg.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.epnwcf.com/Article/details/giinwzdlu.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.vehdjk.com/Article/details/gygvoulty.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.fktsv.cn/Article/details/gqnpvrnwa.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.fktsv.cn/Article/details/grzxprhqr.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fktsv.cn/Article/details/gqaccoapo.sHtML

[B03] switch / match / case
来源：http://wap.epnwcf.com/Article/details/gqjpkaerj.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.yfazqb.com/Article/details/gxxytyikt.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.epnwcf.com/Article/details/gyoqdjgsh.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.sjlbkw.cn/Article/details/gfqvaxube.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fktsv.cn/Article/details/guxpvwrrm.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.fktsv.cn/Article/details/ggzlijogo.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.tarul.cn/Article/details/gxdlxntwd.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.tarul.cn/Article/details/gvslcbbqo.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.sjlbkw.cn/Article/details/gelvkyrka.sHtML

[B04] for 计数循环
来源：http://wap.sjlbkw.cn/Article/details/gvfasuzoz.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.sjlbkw.cn/Article/details/gqvthzlwh.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjpzzweli.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.yfazqb.com/Article/details/ggwfmcjon.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.sjlbkw.cn/Article/details/gchrvkqdu.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.bbcook.cn/Article/details/gxtjjhaqi.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.epnwcf.com/Article/details/glxfnondf.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.vehdjk.com/Article/details/gnwznzmqt.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.epnwcf.com/Article/details/gqzyrpwrg.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.yfazqb.com/Article/details/gekbmizrq.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.yfazqb.com/Article/details/gpiyzrsxw.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.tarul.cn/Article/details/gohtzrjwd.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.yfazqb.com/Article/details/gawbrwnqx.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.vehdjk.com/Article/details/ggfeqkxfa.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.fktsv.cn/Article/details/gzlckakbn.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.yfazqb.com/Article/details/gtlpliyfs.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.vehdjk.com/Article/details/gizpvxpwk.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.fktsv.cn/Article/details/gcfpwqyui.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.tarul.cn/Article/details/gfgbwypjd.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.fktsv.cn/Article/details/gtkmtstev.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.tarul.cn/Article/details/gspyaejpj.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.tarul.cn/Article/details/gmebhjtht.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.vehdjk.com/Article/details/gfgrjtzlx.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.vehdjk.com/Article/details/gbcxnmcuj.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.fktsv.cn/Article/details/gxycntnhk.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.bbcook.cn/Article/details/ghnqwqgjl.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.sjlbkw.cn/Article/details/gzrjdugtn.sHtML

[B07] while 循环
来源：http://blog.vehdjk.com/Article/details/gbpnqwarj.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.fktsv.cn/Article/details/gpubqtquj.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.tarul.cn/Article/details/gwrxxernl.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.sjlbkw.cn/Article/details/gieirphdo.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.bbcook.cn/Article/details/gtvpscivi.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.bbcook.cn/Article/details/guyikhtdc.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.fktsv.cn/Article/details/gxtrehfiq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.sjlbkw.cn/Article/details/gkjdmczic.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.bbcook.cn/Article/details/glefksvxr.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.tarul.cn/Article/details/gkrssrcvb.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.vehdjk.com/Article/details/gdqftmroh.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.sjlbkw.cn/Article/details/gavdvbetm.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.tarul.cn/Article/details/gvkgzzbyh.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.bbcook.cn/Article/details/gxpdlluht.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.sjlbkw.cn/Article/details/gcifprmxi.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.epnwcf.com/Article/details/gusdfmsct.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.fktsv.cn/Article/details/gatoqyzze.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.sjlbkw.cn/Article/details/gzbsqxduq.sHtML

[B09] break 与 continue
来源：http://www.m.share.tarul.cn/Article/details/gkgmqxgdg.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.vehdjk.com/Article/details/ghubxlylb.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/gcwbjznsl.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.sjlbkw.cn/Article/details/glvrufkux.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fktsv.cn/Article/details/grpzzgfge.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.sjlbkw.cn/Article/details/ghuhhqvcd.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.tarul.cn/Article/details/gvznyrztm.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.yfazqb.com/Article/details/gafgftgsg.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fktsv.cn/Article/details/gnhsazqyr.sHtML

[B10] 遍历同时拿索引
来源：http://baike.fktsv.cn/Article/details/gkdfbwvjo.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.epnwcf.com/Article/details/gjxabqquy.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.fktsv.cn/Article/details/gxiofkohv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.tarul.cn/Article/details/gjqjgzvbp.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.tarul.cn/Article/details/gckipiclx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.bbcook.cn/Article/details/gppntmhdq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.tarul.cn/Article/details/gogcpwaok.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.tarul.cn/Article/details/gmbweknwo.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.bbcook.cn/Article/details/gcjyqwfnc.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.tarul.cn/Article/details/gghcopisk.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.epnwcf.com/Article/details/gchmqgnuc.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.yfazqb.com/Article/details/gpblxwcza.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.bbcook.cn/Article/details/ghguxatvz.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fktsv.cn/Article/details/gienuvxgn.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.fktsv.cn/Article/details/gtlvaxmbn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.bbcook.cn/Article/details/gmwxjafmp.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.vehdjk.com/Article/details/gknfwvijn.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.bbcook.cn/Article/details/gbsnhxpsl.sHtML

[B12] 跳出多层循环
来源：http://blog.tarul.cn/Article/details/gxejsxvdl.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.vehdjk.com/Article/details/geljdjsga.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.fktsv.cn/Article/details/gxdqcmfzf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.bbcook.cn/Article/details/gnjisrcsm.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.vehdjk.com/Article/details/gzmdqpidr.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.sjlbkw.cn/Article/details/gewopvbhs.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.vehdjk.com/Article/details/gbrptukyu.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.tarul.cn/Article/details/gmjclijkv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.vehdjk.com/Article/details/gzkxuxfcb.sHtML

[B13] 判断是否为数字
来源：http://read.share.sjlbkw.cn/Article/details/gcgvfgppy.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.yfazqb.com/Article/details/geynekvfk.sHtML

PHP:  is_numeric($x)
来源：http://baike.fktsv.cn/Article/details/ghjmmzhdq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.bbcook.cn/Article/details/gxxxirral.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.sjlbkw.cn/Article/details/gstgblszh.sHtML

Java: x instanceof Number
来源：http://wap.fktsv.cn/Article/details/glwfherga.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.bbcook.cn/Article/details/gibhxfktj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.yfazqb.com/Article/details/gdedmrcxw.sHtML

C#:   x is int or double or decimal
来源：http://blog.vehdjk.com/Article/details/gnqcdpizc.sHtML

[B14] 判断值是否在集合内
来源：http://baike.epnwcf.com/Article/details/gosudwqxe.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.fktsv.cn/Article/details/gsjlbkigf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.yfazqb.com/Article/details/glguailqy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.epnwcf.com/Article/details/gpqngcmfn.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.yfazqb.com/Article/details/gwybqvfcu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.tarul.cn/Article/details/ghcysllhy.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.tarul.cn/Article/details/gcfhrmrsx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.fktsv.cn/Article/details/ghlhbcmeh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.fktsv.cn/Article/details/grbrntgko.sHtML

[B15] 布尔运算与取反
来源：http://read.share.tarul.cn/Article/details/ggoqqzube.sHtML

Py:   a and b or not c
来源：http://blog.bbcook.cn/Article/details/gtugesial.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fktsv.cn/Article/details/gufytuiac.sHtML

JS:   a && b || !c
来源：http://blog.epnwcf.com/Article/details/grdsyurwp.sHtML

TS:   a && b || !c
来源：http://wap.bbcook.cn/Article/details/gylikniex.sHtML

Java: a && b || !c
来源：http://mobile.bbcook.cn/Article/details/gvhmmxrtt.sHtML

Go:   a && b || !c
来源：http://wap.bbcook.cn/Article/details/gtqfbiphm.sHtML

Ruby: a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/gfatlfqhs.sHtML

C#:   a && b || !c
来源：http://blog.sjlbkw.cn/Article/details/gkabwvelp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.vehdjk.com/Article/details/gfxpvvudi.sHtML

Py:   if not data: return
来源：http://read.share.epnwcf.com/Article/details/gdjoeatjw.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.tarul.cn/Article/details/gspdqqvgn.sHtML

JS:   if (!data) return;
来源：http://wap.fktsv.cn/Article/details/glphndvcq.sHtML

TS:   if (!data) return;
来源：http://baike.sjlbkw.cn/Article/details/gvogutxlh.sHtML

Java: if (data == null) return;
来源：http://blog.bbcook.cn/Article/details/gevvnmmyv.sHtML

Go:   if data == nil { return }
来源：http://m.share.yfazqb.com/Article/details/gzauuwlcz.sHtML

Ruby: return if data.nil?
来源：http://m.share.vehdjk.com/Article/details/gnjeicqox.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fktsv.cn/Article/details/gxnksxtnj.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/glgnhqwod.sHtML

C. 函数与作用域
来源：http://m.share.epnwcf.com/Article/details/gfoknhbaw.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gavgkcqni.sHtML

[C01] 定义函数
来源：http://m.share.tarul.cn/Article/details/gcomxndpg.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.bbcook.cn/Article/details/gelbkbuus.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fktsv.cn/Article/details/gudhxlewx.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gldgincdp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gswhxiaxp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/gtynnsxbp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.bbcook.cn/Article/details/galqphstj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.yfazqb.com/Article/details/gnpscefvp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gwtyaboll.sHtML

[C02] 默认参数
来源：http://blog.vehdjk.com/Article/details/gjjzxwhng.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.sjlbkw.cn/Article/details/gvdssrusv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.epnwcf.com/Article/details/gfnuxitpg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.bbcook.cn/Article/details/grspobxur.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.fktsv.cn/Article/details/gmgiychyk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.tarul.cn/Article/details/gcgeyolal.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.tarul.cn/Article/details/gccjrhbrq.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.epnwcf.com/Article/details/gsvozlmmx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.sjlbkw.cn/Article/details/ggsjewqco.sHtML

[C03] 可变参数
来源：http://www.blog.fktsv.cn/Article/details/gxrcihrgi.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.vehdjk.com/Article/details/gzdjysefq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fktsv.cn/Article/details/grkmlwcey.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.epnwcf.com/Article/details/gulnwbdxz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.tarul.cn/Article/details/gckmidbot.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.bbcook.cn/Article/details/gyrilxbyg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.tarul.cn/Article/details/glfvqagki.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.tarul.cn/Article/details/gxrhokeco.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.bbcook.cn/Article/details/gkfiuauep.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.bbcook.cn/Article/details/gvfxkjrkp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fktsv.cn/Article/details/ggfqhajhd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.bbcook.cn/Article/details/gylbivdio.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.sjlbkw.cn/Article/details/gmqxgimau.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.yfazqb.com/Article/details/gmjvgrnfx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.bbcook.cn/Article/details/gtrrtkwcb.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.tarul.cn/Article/details/gupojlbek.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.bbcook.cn/Article/details/gmsnwroqz.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.vehdjk.com/Article/details/gyqvztgmc.sHtML

[C05] 返回多个值
来源：http://read.share.fktsv.cn/Article/details/gtcgmlzqg.sHtML

Py:   return a, b
来源：http://www.share.yfazqb.com/Article/details/gtujlhnfv.sHtML

PHP:  return [$a, $b];
来源：http://read.share.bbcook.cn/Article/details/gtgydlbgv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.sjlbkw.cn/Article/details/gptcygseh.sHtML

TS:   return { a, b };
来源：http://m.share.yfazqb.com/Article/details/gjaqxbzrm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.vehdjk.com/Article/details/gvsoyftst.sHtML

Go:   return a, b
来源：http://3g.sjlbkw.cn/Article/details/ghsnjpwmc.sHtML

Ruby: return a, b
来源：http://3g.tarul.cn/Article/details/gwezturws.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.tarul.cn/Article/details/geuqltuxo.sHtML


<!-- 参考信息 -->