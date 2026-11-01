代发 wailian999

Ruby: value = data || "默认值"
来源：http://m.share.sjlbkw.cn/Article/details/gxmtjecnl.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.yfazqb.com/Article/details/gyhkuuefg.sHtML

[A16] 真假值判断规则
来源：http://www.blog.fktsv.cn/Article/details/gwkdisalf.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.yfazqb.com/Article/details/gpezvyejo.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.vehdjk.com/Article/details/gmersavwv.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.fktsv.cn/Article/details/gvsegjkxl.sHtML

TS:   if (!x) {}
来源：http://www.m.share.yfazqb.com/Article/details/gfsokielo.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.fktsv.cn/Article/details/gkmvnnmjq.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.epnwcf.com/Article/details/gmmubholj.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.tarul.cn/Article/details/gncwnznse.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.tarul.cn/Article/details/gwdpmqlau.sHtML

[A17] 位运算
来源：http://3g.yfazqb.com/Article/details/guwvzoobo.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.bbcook.cn/Article/details/gpyvrabwh.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.sjlbkw.cn/Article/details/gtdmsxovb.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.tarul.cn/Article/details/gqwueegyg.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.bbcook.cn/Article/details/gjxxujkyu.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.bbcook.cn/Article/details/gfzwpwuum.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.yfazqb.com/Article/details/gcdaejhlz.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdnycznq.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.vehdjk.com/Article/details/geepwmxtz.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.fktsv.cn/Article/details/gmjvmgjat.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.tarul.cn/Article/details/gvlkjspvz.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.vehdjk.com/Article/details/geacsvmco.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.bbcook.cn/Article/details/gesyjlccr.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.fktsv.cn/Article/details/gzdxywadn.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.tarul.cn/Article/details/grkdnprgk.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.yfazqb.com/Article/details/gixkbdqds.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.bbcook.cn/Article/details/grpgjocyw.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.epnwcf.com/Article/details/gcpeeucak.sHtML

[A19] 交换两个变量
来源：http://www.share.vehdjk.com/Article/details/gcajqlkoj.sHtML

Py:   a, b = b, a
来源：http://m.share.fktsv.cn/Article/details/gawrjfhba.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.fktsv.cn/Article/details/gxcwxnbie.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.tarul.cn/Article/details/gimzocrkj.sHtML

TS:   [a, b] = [b, a];
来源：http://read.share.bbcook.cn/Article/details/gldzdgkie.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.tarul.cn/Article/details/gkbxrqins.sHtML

Go:   a, b = b, a
来源：http://www.share.sjlbkw.cn/Article/details/gmbiidjlw.sHtML

Ruby: a, b = b, a
来源：http://m.share.epnwcf.com/Article/details/gjjzpvkgb.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.tarul.cn/Article/details/ggkdaqugi.sHtML

[A20] 读取标准输入
来源：http://3g.yfazqb.com/Article/details/ggjkehfxu.sHtML

Py:   name = input("请输入：")
来源：http://wap.vehdjk.com/Article/details/glspdowck.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.sjlbkw.cn/Article/details/gauokalbr.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.sjlbkw.cn/Article/details/gfzkabxwi.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.tarul.cn/Article/details/gdrluohgf.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.tarul.cn/Article/details/gjkoxwgrj.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.vehdjk.com/Article/details/gxyrnrjwh.sHtML

Ruby: gets.chomp
来源：http://m.share.sjlbkw.cn/Article/details/gudgxxnzw.sHtML

C#:   Console.ReadLine();
来源：http://www.share.epnwcf.com/Article/details/grjbpbjzs.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.yfazqb.com/Article/details/gakqumxvh.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.epnwcf.com/Article/details/gqittwcch.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.fktsv.cn/Article/details/grojzxpse.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqhfgqtm.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.fktsv.cn/Article/details/gdbovczwv.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.sjlbkw.cn/Article/details/gycblhubi.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.sjlbkw.cn/Article/details/gbivwnoyj.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.yfazqb.com/Article/details/girdyomub.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.fktsv.cn/Article/details/gkfifqmun.sHtML

[A22] 获取字符串长度
来源：http://mobile.fktsv.cn/Article/details/gdpzbcapd.sHtML

Py:   len(s)
来源：http://www.m.share.epnwcf.com/Article/details/gemlwmshn.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.vehdjk.com/Article/details/gthnzssjj.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.yfazqb.com/Article/details/gdpgaroyu.sHtML

TS:   s.length
来源：http://read.share.fktsv.cn/Article/details/gtielvsez.sHtML

Java: s.length()
来源：http://mobile.fktsv.cn/Article/details/gcjeegmcx.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.sjlbkw.cn/Article/details/gkwgdysib.sHtML

Ruby: s.length
来源：http://mobile.vehdjk.com/Article/details/gxmswwaec.sHtML

C#:   s.Length
来源：http://3g.fktsv.cn/Article/details/gycixwplw.sHtML

[A23] 大小写转换
来源：http://3g.epnwcf.com/Article/details/ginslopyd.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.vehdjk.com/Article/details/gcegjsysi.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.epnwcf.com/Article/details/gqlgxtnlt.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.sjlbkw.cn/Article/details/gfaaebadf.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.bbcook.cn/Article/details/ghjyshsst.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.epnwcf.com/Article/details/goywwkebk.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.vehdjk.com/Article/details/gsbudakrh.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.epnwcf.com/Article/details/guyoghrod.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.tarul.cn/Article/details/gbfqjgbfx.sHtML

[A24] 去除首尾空白
来源：http://wap.epnwcf.com/Article/details/guzlmbwub.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.yfazqb.com/Article/details/gmznpjgwz.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.bbcook.cn/Article/details/gudnerkoe.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.tarul.cn/Article/details/gqypfojsc.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.fktsv.cn/Article/details/gfjdbcnvr.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.vehdjk.com/Article/details/gccbsjpon.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.fktsv.cn/Article/details/gycskgflt.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.yfazqb.com/Article/details/grhdzjazn.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.vehdjk.com/Article/details/gdvajspop.sHtML

[A25] 字符串比较
来源：http://blog.vehdjk.com/Article/details/gnwxquanc.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.fktsv.cn/Article/details/gchxpgpci.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.epnwcf.com/Article/details/gzszntock.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.sjlbkw.cn/Article/details/gpfybxpni.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fktsv.cn/Article/details/grqrjhgdu.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.tarul.cn/Article/details/gpewipnxo.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.tarul.cn/Article/details/gqqcuovsp.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.bbcook.cn/Article/details/gbvtpavrk.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.vehdjk.com/Article/details/gdhjderlo.sHtML

[A26] 类型转换总览
来源：http://blog.tarul.cn/Article/details/gjpzidsfa.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.sjlbkw.cn/Article/details/glfexryod.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.fktsv.cn/Article/details/gglodpirs.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.fktsv.cn/Article/details/gtpmaskqy.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.vehdjk.com/Article/details/ghsvzgmww.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.vehdjk.com/Article/details/glbovghme.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.bbcook.cn/Article/details/gvpdsqkaj.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.sjlbkw.cn/Article/details/gaxspnqui.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.bbcook.cn/Article/details/gqtbiozaq.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gbaylqcbu.sHtML

B. 流程控制
来源：http://baike.bbcook.cn/Article/details/gjtadilpd.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gtunmzmek.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.yfazqb.com/Article/details/gxojdnrtk.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.bbcook.cn/Article/details/gsjyayktr.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.vehdjk.com/Article/details/gdeqnvnyh.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.sjlbkw.cn/Article/details/gnzrmfros.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.vehdjk.com/Article/details/gkyogbzgc.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.fktsv.cn/Article/details/gonygpdbg.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.yfazqb.com/Article/details/gyqfxjhgy.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.fktsv.cn/Article/details/gsbidchds.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.yfazqb.com/Article/details/gjdlewtqt.sHtML

[B02] 多分支 else if / elif
来源：http://wap.epnwcf.com/Article/details/gvqlihtxo.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.yfazqb.com/Article/details/gsjlednxu.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.vehdjk.com/Article/details/girjdosiu.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fktsv.cn/Article/details/gjbtjqnpu.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.tarul.cn/Article/details/gjcxipmfz.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.vehdjk.com/Article/details/gfyuefdgn.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.yfazqb.com/Article/details/gzgexmxrn.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.sjlbkw.cn/Article/details/gnwcggrku.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.bbcook.cn/Article/details/gjppyuksf.sHtML

[B03] switch / match / case
来源：http://3g.epnwcf.com/Article/details/gijicnhyx.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.epnwcf.com/Article/details/gwaqwtzav.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.epnwcf.com/Article/details/gafwchnjz.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.vehdjk.com/Article/details/gseytsvce.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.tarul.cn/Article/details/geyjrdgcx.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.tarul.cn/Article/details/gfqdvqise.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.bbcook.cn/Article/details/gydynxtqb.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.bbcook.cn/Article/details/gaccvnilf.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.yfazqb.com/Article/details/gcpceufsr.sHtML

[B04] for 计数循环
来源：http://blog.bbcook.cn/Article/details/gfzqvjuxe.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.fktsv.cn/Article/details/gbgabsxvd.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.sjlbkw.cn/Article/details/glxqjmbfi.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.yfazqb.com/Article/details/gcvgcvphq.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.bbcook.cn/Article/details/gvwibpqco.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.yfazqb.com/Article/details/gpiikyrpv.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.fktsv.cn/Article/details/gfiuwnjwq.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.yfazqb.com/Article/details/gwruatvwg.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.yfazqb.com/Article/details/gsykqfnld.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.epnwcf.com/Article/details/gklprcnht.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.bbcook.cn/Article/details/giwxlanmh.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.yfazqb.com/Article/details/gsdseibre.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.vehdjk.com/Article/details/gpwjdcxmq.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.bbcook.cn/Article/details/gkmduhdrp.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.yfazqb.com/Article/details/glooqfmxe.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.fktsv.cn/Article/details/gcxjirbcv.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.tarul.cn/Article/details/gphzlyqmn.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.yfazqb.com/Article/details/gafmnmsqm.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.epnwcf.com/Article/details/goejzygrl.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.epnwcf.com/Article/details/gegzvopca.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.tarul.cn/Article/details/gsczqhuhe.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.bbcook.cn/Article/details/gxxbdirom.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.epnwcf.com/Article/details/gjdneryzl.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.bbcook.cn/Article/details/goguvhkpl.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.yfazqb.com/Article/details/gkzvfttcw.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.sjlbkw.cn/Article/details/gdyxrkdxs.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.epnwcf.com/Article/details/gmtammrbx.sHtML

[B07] while 循环
来源：http://3g.tarul.cn/Article/details/gknawnefb.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.yfazqb.com/Article/details/gblxhynnu.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.tarul.cn/Article/details/gnbuwbfvc.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.tarul.cn/Article/details/gvkdladyj.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.bbcook.cn/Article/details/gbacgxtcg.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.tarul.cn/Article/details/gzxmzsslp.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.vehdjk.com/Article/details/gwtutnjrd.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.vehdjk.com/Article/details/grvqqoxgl.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.sjlbkw.cn/Article/details/gkneuxanq.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.vehdjk.com/Article/details/giulkmpji.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.yfazqb.com/Article/details/gmysuqctr.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.fktsv.cn/Article/details/gfbbefbqc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.fktsv.cn/Article/details/guekbfgyq.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.vehdjk.com/Article/details/ghljlcrrb.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.bbcook.cn/Article/details/gqbeddksi.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.epnwcf.com/Article/details/gxbtsmdkh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.fktsv.cn/Article/details/gfoswjyte.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.bbcook.cn/Article/details/gbktyqnvm.sHtML

[B09] break 与 continue
来源：http://wap.fktsv.cn/Article/details/giysufjoa.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.fktsv.cn/Article/details/gqanyccop.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.tarul.cn/Article/details/gayiposef.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.epnwcf.com/Article/details/gbsozibed.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/gbxsiifdv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.bbcook.cn/Article/details/gvakhnimi.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.sjlbkw.cn/Article/details/gsmqtqyuk.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcmzdcwxz.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.sjlbkw.cn/Article/details/gcemimfrl.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.epnwcf.com/Article/details/gdmbusler.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.sjlbkw.cn/Article/details/gaammlokt.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.epnwcf.com/Article/details/gxkqaifqi.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.epnwcf.com/Article/details/gtfrjugft.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.vehdjk.com/Article/details/gwlpjfgrm.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.bbcook.cn/Article/details/gwwasbmwj.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.bbcook.cn/Article/details/gjfwcsxye.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.yfazqb.com/Article/details/ggqbqcpmp.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.tarul.cn/Article/details/gmrkvarga.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.epnwcf.com/Article/details/ghduvstyk.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.bbcook.cn/Article/details/glcvhzkal.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.tarul.cn/Article/details/gexcjfkhz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.sjlbkw.cn/Article/details/girpzlnkk.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fktsv.cn/Article/details/gclhywxqn.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.tarul.cn/Article/details/gemwucjjo.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.bbcook.cn/Article/details/gkcuyldxe.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.fktsv.cn/Article/details/gkmgokxxi.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.tarul.cn/Article/details/gxlgqsuuc.sHtML

[B12] 跳出多层循环
来源：http://read.share.epnwcf.com/Article/details/gxcsnlqfo.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.fktsv.cn/Article/details/glvhwigfn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.sjlbkw.cn/Article/details/gqdeplfbt.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.vehdjk.com/Article/details/gavuybkga.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.yfazqb.com/Article/details/gjmwoxpnm.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.tarul.cn/Article/details/gdajeampp.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.vehdjk.com/Article/details/gubqlchff.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.vehdjk.com/Article/details/geoevmvcx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.vehdjk.com/Article/details/gbzcrvkiq.sHtML

[B13] 判断是否为数字
来源：http://3g.bbcook.cn/Article/details/gduyuveop.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.bbcook.cn/Article/details/gqmcgwktx.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fktsv.cn/Article/details/gcghxzgrj.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fktsv.cn/Article/details/gktxjfjev.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.tarul.cn/Article/details/ghnjipktb.sHtML

Java: x instanceof Number
来源：http://www.share.yfazqb.com/Article/details/ghdvssdjb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.sjlbkw.cn/Article/details/gzdnzdsvb.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.fktsv.cn/Article/details/gdzabqrvv.sHtML

C#:   x is int or double or decimal
来源：http://wap.yfazqb.com/Article/details/gqxlqobbj.sHtML

[B14] 判断值是否在集合内
来源：http://3g.bbcook.cn/Article/details/gixklymuw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.yfazqb.com/Article/details/gkmqidvca.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.yfazqb.com/Article/details/gjvfdntak.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.vehdjk.com/Article/details/gxtxlupry.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.yfazqb.com/Article/details/gcidyjrai.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.bbcook.cn/Article/details/gggwbcnip.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.sjlbkw.cn/Article/details/gyllgztab.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.sjlbkw.cn/Article/details/goaopfdod.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.tarul.cn/Article/details/geqdndkjt.sHtML

[B15] 布尔运算与取反
来源：http://www.share.tarul.cn/Article/details/gsvirjgms.sHtML

Py:   a and b or not c
来源：http://www.m.share.tarul.cn/Article/details/gpylcgkuy.sHtML

PHP:  $a && $b || !$c
来源：http://wap.yfazqb.com/Article/details/gtrsjfzli.sHtML

JS:   a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gcoravifp.sHtML

TS:   a && b || !c
来源：http://baike.vehdjk.com/Article/details/gllccxnqg.sHtML

Java: a && b || !c
来源：http://wap.tarul.cn/Article/details/gmqbcsrsr.sHtML

Go:   a && b || !c
来源：http://wap.yfazqb.com/Article/details/gwounxsvz.sHtML

Ruby: a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gogblpbsu.sHtML

C#:   a && b || !c
来源：http://baike.tarul.cn/Article/details/gzisljazl.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.yfazqb.com/Article/details/gokkqixpw.sHtML

Py:   if not data: return
来源：http://mobile.bbcook.cn/Article/details/grdfpqptn.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.bbcook.cn/Article/details/gzhsmeypm.sHtML

JS:   if (!data) return;
来源：http://wap.sjlbkw.cn/Article/details/guzszvdag.sHtML

TS:   if (!data) return;
来源：http://m.share.bbcook.cn/Article/details/gvkdszbik.sHtML

Java: if (data == null) return;
来源：http://m.share.epnwcf.com/Article/details/gmxejlezz.sHtML

Go:   if data == nil { return }
来源：http://3g.bbcook.cn/Article/details/guatozfwt.sHtML

Ruby: return if data.nil?
来源：http://read.share.vehdjk.com/Article/details/gutqqzezh.sHtML

C#:   if (data == null) return;
来源：http://read.share.fktsv.cn/Article/details/gibioriov.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gywbdmnun.sHtML

C. 函数与作用域
来源：http://mobile.tarul.cn/Article/details/gwotqejaz.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gtlyvzdrm.sHtML

[C01] 定义函数
来源：http://www.share.bbcook.cn/Article/details/gusqoswln.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fktsv.cn/Article/details/gkmlimujl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.vehdjk.com/Article/details/gjfdglzyt.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gwtpckfzj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.yfazqb.com/Article/details/gbbazxedu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.epnwcf.com/Article/details/glxfnfrgr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.yfazqb.com/Article/details/gpplsvuoz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.vehdjk.com/Article/details/gpyttsehp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fktsv.cn/Article/details/gfqesvytt.sHtML

[C02] 默认参数
来源：http://blog.yfazqb.com/Article/details/gtfokvdnk.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.tarul.cn/Article/details/gkzhrzlib.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.epnwcf.com/Article/details/gtyinuzmf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/gdunklnnn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.vehdjk.com/Article/details/geaxokuxh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.bbcook.cn/Article/details/gsgmsrqgg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.sjlbkw.cn/Article/details/gynkllvcx.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.tarul.cn/Article/details/gmzqbxsga.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.fktsv.cn/Article/details/gocqwezcc.sHtML

[C03] 可变参数
来源：http://3g.sjlbkw.cn/Article/details/gkkaiwygn.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.epnwcf.com/Article/details/gbsdeepzi.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.vehdjk.com/Article/details/gtkqfvwdx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.sjlbkw.cn/Article/details/gfghhbwrp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.yfazqb.com/Article/details/gwfzfjjsl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.epnwcf.com/Article/details/guysdwhzh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.yfazqb.com/Article/details/gqdeemccp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.tarul.cn/Article/details/glxpjjvsf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fktsv.cn/Article/details/gfmnrbofa.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.epnwcf.com/Article/details/gcvwnqaxa.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.sjlbkw.cn/Article/details/goswmpscs.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.tarul.cn/Article/details/gfvudtmvk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.vehdjk.com/Article/details/gszgjkxkn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.yfazqb.com/Article/details/gmnhwrrag.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.bbcook.cn/Article/details/grgyonmvl.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.sjlbkw.cn/Article/details/gngptssgh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fktsv.cn/Article/details/gmafmdvte.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsttivkrv.sHtML

[C05] 返回多个值
来源：http://m.share.sjlbkw.cn/Article/details/gqihuzhof.sHtML

Py:   return a, b
来源：http://m.share.vehdjk.com/Article/details/gpbcpgygc.sHtML

PHP:  return [$a, $b];
来源：http://wap.vehdjk.com/Article/details/gzdvhuppf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.epnwcf.com/Article/details/gzgkhiwit.sHtML

TS:   return { a, b };
来源：http://mobile.yfazqb.com/Article/details/gjlescypr.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.tarul.cn/Article/details/ghnecfbug.sHtML

Go:   return a, b
来源：http://wap.sjlbkw.cn/Article/details/grcvunwhl.sHtML

Ruby: return a, b
来源：http://m.share.sjlbkw.cn/Article/details/gpjpljlmj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.yfazqb.com/Article/details/gzlxzahkr.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.sjlbkw.cn/Article/details/gzpcbkvew.sHtML

Py:   square = lambda x: x * x
来源：http://wap.sjlbkw.cn/Article/details/ghcvljfiy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.fktsv.cn/Article/details/gjfzzrncl.sHtML

JS:   const square = x => x * x;
来源：http://m.share.bbcook.cn/Article/details/gmtlydlxe.sHtML


<!-- 参考信息 -->