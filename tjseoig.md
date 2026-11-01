代发 wailian999

C#:   (int)'A'; (char)65
来源：http://www.blog.yfazqb.com/Article/details/gzpbldhcy.sHtML

[A19] 交换两个变量
来源：http://www.m.share.tarul.cn/Article/details/grpcwulxj.sHtML

Py:   a, b = b, a
来源：http://blog.yfazqb.com/Article/details/guwjkbjlf.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.epnwcf.com/Article/details/gskfsmpur.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.vehdjk.com/Article/details/gbjeupwga.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.tarul.cn/Article/details/gfrxpszkv.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.vehdjk.com/Article/details/gcryxjxsc.sHtML

Go:   a, b = b, a
来源：http://wap.sjlbkw.cn/Article/details/gisbefhno.sHtML

Ruby: a, b = b, a
来源：http://www.blog.tarul.cn/Article/details/gszmiocdw.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.yfazqb.com/Article/details/ghegjvqqn.sHtML

[A20] 读取标准输入
来源：http://m.share.epnwcf.com/Article/details/gvfspjsyg.sHtML

Py:   name = input("请输入：")
来源：http://www.share.sjlbkw.cn/Article/details/gmwhchasq.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.sjlbkw.cn/Article/details/gkweepxhz.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.fktsv.cn/Article/details/gsjrkwvka.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.yfazqb.com/Article/details/gexkxvhwe.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.sjlbkw.cn/Article/details/gowvswwjx.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwylgxtek.sHtML

Ruby: gets.chomp
来源：http://3g.epnwcf.com/Article/details/grajcvwmm.sHtML

C#:   Console.ReadLine();
来源：http://3g.yfazqb.com/Article/details/gciojondp.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.tarul.cn/Article/details/guuuwgraq.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.vehdjk.com/Article/details/gngzpqvcu.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.tarul.cn/Article/details/gngsqsjpv.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.yfazqb.com/Article/details/gskdqwtjf.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.bbcook.cn/Article/details/gcqtaidlh.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.vehdjk.com/Article/details/gmhpjusij.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.bbcook.cn/Article/details/gmgdhuzht.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.yfazqb.com/Article/details/gugsuiisi.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.sjlbkw.cn/Article/details/ggiqrgvpz.sHtML

[A22] 获取字符串长度
来源：http://baike.sjlbkw.cn/Article/details/gzgrjbihy.sHtML

Py:   len(s)
来源：http://m.share.tarul.cn/Article/details/grmcmgsya.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.vehdjk.com/Article/details/giahmgepv.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.fktsv.cn/Article/details/gthklzumq.sHtML

TS:   s.length
来源：http://blog.bbcook.cn/Article/details/gigamzeps.sHtML

Java: s.length()
来源：http://read.share.yfazqb.com/Article/details/ggxglcjzi.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.vehdjk.com/Article/details/geitgpnnk.sHtML

Ruby: s.length
来源：http://m.share.sjlbkw.cn/Article/details/gitkbhapn.sHtML

C#:   s.Length
来源：http://www.m.share.sjlbkw.cn/Article/details/ggeahjtah.sHtML

[A23] 大小写转换
来源：http://baike.tarul.cn/Article/details/gxfvbyjkq.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.vehdjk.com/Article/details/gdkfoixnv.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.tarul.cn/Article/details/gnxsembam.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.vehdjk.com/Article/details/guzmcwulr.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.yfazqb.com/Article/details/gumduqmjb.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.yfazqb.com/Article/details/gcqkvzcwj.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.vehdjk.com/Article/details/gggazylhv.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.sjlbkw.cn/Article/details/gdzvrozkm.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.bbcook.cn/Article/details/ghicitfmx.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.vehdjk.com/Article/details/gpgazslxk.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.yfazqb.com/Article/details/giobmpusj.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.bbcook.cn/Article/details/gydgxocgz.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.yfazqb.com/Article/details/gcsrkwkbn.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.fktsv.cn/Article/details/gzvuxehzz.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.bbcook.cn/Article/details/gomjnqgbm.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.bbcook.cn/Article/details/gyhsjqmmk.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.fktsv.cn/Article/details/gilykxtet.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.bbcook.cn/Article/details/gtinsiikd.sHtML

[A25] 字符串比较
来源：http://read.share.vehdjk.com/Article/details/gddnzguqf.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.sjlbkw.cn/Article/details/gbwobjfst.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.vehdjk.com/Article/details/geqyahvsv.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.bbcook.cn/Article/details/ghzgsxdqt.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.yfazqb.com/Article/details/gkhxczpfq.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.tarul.cn/Article/details/gwgrlhgvm.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.yfazqb.com/Article/details/gfmabjnbv.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.epnwcf.com/Article/details/ghjfiqurl.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.bbcook.cn/Article/details/gyiidmmmd.sHtML

[A26] 类型转换总览
来源：http://3g.bbcook.cn/Article/details/gydbsxgkp.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.bbcook.cn/Article/details/gojhkeyma.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.sjlbkw.cn/Article/details/gqdnlwjti.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.bbcook.cn/Article/details/gtntslnui.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.yfazqb.com/Article/details/gvycqrrun.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.sjlbkw.cn/Article/details/gywmjpcer.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.vehdjk.com/Article/details/gaywquxjq.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.bbcook.cn/Article/details/gbiulzjcy.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.epnwcf.com/Article/details/gfdaatjuz.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/ghimuakhk.sHtML

B. 流程控制
来源：http://www.share.bbcook.cn/Article/details/gyrtmxlpw.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gnxfbzfzx.sHtML

[B01] 条件判断 if / else
来源：http://3g.fktsv.cn/Article/details/gnztfwziy.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.yfazqb.com/Article/details/gvlqrussg.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.fktsv.cn/Article/details/gxhynnvqu.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.epnwcf.com/Article/details/gixvjpbwg.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.sjlbkw.cn/Article/details/gzdkbluvf.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.vehdjk.com/Article/details/gdjnaflup.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.yfazqb.com/Article/details/gmfffvbzn.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.bbcook.cn/Article/details/gjdnmrxvr.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.bbcook.cn/Article/details/gmntlbxwy.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.sjlbkw.cn/Article/details/gnliccrmo.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.fktsv.cn/Article/details/gjybfxdkb.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.bbcook.cn/Article/details/gjqoayngp.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.tarul.cn/Article/details/gswmhmpye.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.yfazqb.com/Article/details/gxzkrnuib.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.sjlbkw.cn/Article/details/gbnmqxlyf.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.bbcook.cn/Article/details/giwvfgvyl.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.yfazqb.com/Article/details/gpkorijwg.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.yfazqb.com/Article/details/gitsjxjvz.sHtML

[B03] switch / match / case
来源：http://www.m.share.epnwcf.com/Article/details/gtztkecmt.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.yfazqb.com/Article/details/gvvpnsmvy.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.sjlbkw.cn/Article/details/gaiqhwosl.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.vehdjk.com/Article/details/gixkxqfpv.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.sjlbkw.cn/Article/details/gcdmeojjq.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.yfazqb.com/Article/details/gatqxovxp.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.bbcook.cn/Article/details/gnhmvtsox.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.epnwcf.com/Article/details/gzenbaqpg.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.vehdjk.com/Article/details/gvyxvidht.sHtML

[B04] for 计数循环
来源：http://blog.bbcook.cn/Article/details/gmqywiyel.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.epnwcf.com/Article/details/grqlitqjl.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.vehdjk.com/Article/details/gdbqwioxv.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.sjlbkw.cn/Article/details/gjayzuffn.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.tarul.cn/Article/details/gifysnxfj.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.fktsv.cn/Article/details/gaxswzmmi.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.bbcook.cn/Article/details/gvfzrmulc.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.tarul.cn/Article/details/ghzglwwjd.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.sjlbkw.cn/Article/details/grdtbdqbp.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.vehdjk.com/Article/details/gaddqmpml.sHtML

Py:   for item in arr: print(item)
来源：http://blog.fktsv.cn/Article/details/gparxcweg.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.epnwcf.com/Article/details/gfekrxutm.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.vehdjk.com/Article/details/gjixbwrkn.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.epnwcf.com/Article/details/gtzawfzwy.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.bbcook.cn/Article/details/gpsultctw.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.yfazqb.com/Article/details/gjurmyrnw.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.bbcook.cn/Article/details/gjpcrikpd.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.vehdjk.com/Article/details/gtjolqwxy.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.yfazqb.com/Article/details/gtvtorgsj.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.vehdjk.com/Article/details/gcjymtgid.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.sjlbkw.cn/Article/details/gvwwxpqhy.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fktsv.cn/Article/details/ghmgxojuo.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.bbcook.cn/Article/details/gvbwnvqpf.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.bbcook.cn/Article/details/gybhmjxzv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.vehdjk.com/Article/details/gklkzgpqs.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.vehdjk.com/Article/details/gpnegvqug.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.sjlbkw.cn/Article/details/gkaopgskk.sHtML

[B07] while 循环
来源：http://www.share.vehdjk.com/Article/details/gbiwsofxd.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.yfazqb.com/Article/details/godjrwjft.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.epnwcf.com/Article/details/gwkodeddj.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gibampism.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.bbcook.cn/Article/details/gciyswmdy.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.fktsv.cn/Article/details/gwjuclily.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.yfazqb.com/Article/details/gcjrexleh.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.sjlbkw.cn/Article/details/gybebtihx.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.bbcook.cn/Article/details/gcnqajaee.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.fktsv.cn/Article/details/gqyukqjcr.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.tarul.cn/Article/details/gzfebmagr.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.bbcook.cn/Article/details/gakinwxkk.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.bbcook.cn/Article/details/ggvtokcdx.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.tarul.cn/Article/details/gtbqognbr.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.fktsv.cn/Article/details/gdpznkyye.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.epnwcf.com/Article/details/gioqdbtvk.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.vehdjk.com/Article/details/gtqnpwylb.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.fktsv.cn/Article/details/gktvatfmj.sHtML

[B09] break 与 continue
来源：http://mobile.bbcook.cn/Article/details/gdxwhnnuu.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.yfazqb.com/Article/details/ghwugbrvn.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.epnwcf.com/Article/details/glpgjulus.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.epnwcf.com/Article/details/gmhrvicfe.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.bbcook.cn/Article/details/giequrotd.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.bbcook.cn/Article/details/gesaonlol.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.bbcook.cn/Article/details/gtojrvaal.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.tarul.cn/Article/details/grrgvongy.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.bbcook.cn/Article/details/gvwbvffmd.sHtML

[B10] 遍历同时拿索引
来源：http://baike.yfazqb.com/Article/details/gsskprsnl.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.fktsv.cn/Article/details/goziymogr.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.sjlbkw.cn/Article/details/gdyunrtoy.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.sjlbkw.cn/Article/details/gxetsmjgm.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.vehdjk.com/Article/details/gptaulubm.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.yfazqb.com/Article/details/gofwecujj.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.sjlbkw.cn/Article/details/gjylxpfrg.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.tarul.cn/Article/details/gsmvdaxxi.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.epnwcf.com/Article/details/gpkmbqtfu.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.fktsv.cn/Article/details/gqcccsjea.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.tarul.cn/Article/details/gylvkcjbp.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.vehdjk.com/Article/details/girbmhxdk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fktsv.cn/Article/details/gnlksewpr.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.vehdjk.com/Article/details/gqebmklqt.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gllwzzgdb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.epnwcf.com/Article/details/gnirxebim.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.yfazqb.com/Article/details/grkvfwpdj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.tarul.cn/Article/details/gktxnazfw.sHtML

[B12] 跳出多层循环
来源：http://www.share.yfazqb.com/Article/details/gzcxwzmlj.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.tarul.cn/Article/details/gjttqyftj.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.sjlbkw.cn/Article/details/ghjmfldse.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.epnwcf.com/Article/details/gbmtbkrrd.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.epnwcf.com/Article/details/gfmhottni.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.bbcook.cn/Article/details/grayuoqou.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.tarul.cn/Article/details/gpujrnneb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.bbcook.cn/Article/details/gfnvyuvjz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.sjlbkw.cn/Article/details/gajcdnppo.sHtML

[B13] 判断是否为数字
来源：http://baike.tarul.cn/Article/details/gexknzphr.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.vehdjk.com/Article/details/gbvculhcz.sHtML

PHP:  is_numeric($x)
来源：http://mobile.tarul.cn/Article/details/gbvwhmwrx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.bbcook.cn/Article/details/gpfcyxrbe.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.bbcook.cn/Article/details/gecxnmwbw.sHtML

Java: x instanceof Number
来源：http://read.share.tarul.cn/Article/details/gxeuogkba.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.tarul.cn/Article/details/gnsejmttt.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.yfazqb.com/Article/details/gfdxcvywe.sHtML

C#:   x is int or double or decimal
来源：http://mobile.bbcook.cn/Article/details/gznzvczyl.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.sjlbkw.cn/Article/details/gdqhojkrk.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.vehdjk.com/Article/details/gsvegviow.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.yfazqb.com/Article/details/goeyozygf.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fktsv.cn/Article/details/gpjfladfi.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.vehdjk.com/Article/details/guzlxjuhf.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.vehdjk.com/Article/details/gmxlaogse.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.yfazqb.com/Article/details/gasolvxwt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.sjlbkw.cn/Article/details/gmeecjzvl.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.fktsv.cn/Article/details/gpsfmaxcs.sHtML

[B15] 布尔运算与取反
来源：http://m.share.epnwcf.com/Article/details/gzwfdfdzt.sHtML

Py:   a and b or not c
来源：http://wap.epnwcf.com/Article/details/gqtdmdmdn.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.yfazqb.com/Article/details/gcecffram.sHtML

JS:   a && b || !c
来源：http://baike.bbcook.cn/Article/details/gfmkrelut.sHtML

TS:   a && b || !c
来源：http://3g.epnwcf.com/Article/details/gluwirdkq.sHtML

Java: a && b || !c
来源：http://baike.vehdjk.com/Article/details/gqpawbjum.sHtML

Go:   a && b || !c
来源：http://blog.sjlbkw.cn/Article/details/grbipbymq.sHtML

Ruby: a && b || !c
来源：http://read.share.fktsv.cn/Article/details/govklaszk.sHtML

C#:   a && b || !c
来源：http://www.share.bbcook.cn/Article/details/gnrlbhwvl.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.epnwcf.com/Article/details/gfuvymdcw.sHtML

Py:   if not data: return
来源：http://blog.vehdjk.com/Article/details/gtkgnaebh.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.yfazqb.com/Article/details/gtjgitvfr.sHtML

JS:   if (!data) return;
来源：http://read.share.epnwcf.com/Article/details/gloxapcll.sHtML

TS:   if (!data) return;
来源：http://baike.vehdjk.com/Article/details/grxrjufkl.sHtML

Java: if (data == null) return;
来源：http://baike.tarul.cn/Article/details/gtoxnbhwv.sHtML

Go:   if data == nil { return }
来源：http://3g.epnwcf.com/Article/details/gbsvnhghq.sHtML

Ruby: return if data.nil?
来源：http://www.share.bbcook.cn/Article/details/gosiiummi.sHtML

C#:   if (data == null) return;
来源：http://wap.yfazqb.com/Article/details/guffjucxd.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gbarntkfl.sHtML

C. 函数与作用域
来源：http://read.share.tarul.cn/Article/details/gywwwfbjp.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gnwfarqpd.sHtML

[C01] 定义函数
来源：http://baike.tarul.cn/Article/details/gxxjlwkgc.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.vehdjk.com/Article/details/gkejsnabb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.bbcook.cn/Article/details/gnhydfzxu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gtmksudua.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/gnioivygn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gwtrfvcid.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.sjlbkw.cn/Article/details/gxsmhfsqj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.bbcook.cn/Article/details/gfvrlmgdg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gszgvqedf.sHtML

[C02] 默认参数
来源：http://baike.epnwcf.com/Article/details/guofqfdnh.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.tarul.cn/Article/details/gvuezryyp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.sjlbkw.cn/Article/details/gsfvfzxqf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fktsv.cn/Article/details/glkketgps.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/gtjsyyzfm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.tarul.cn/Article/details/gazdxtluj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fktsv.cn/Article/details/gvnxspraf.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.vehdjk.com/Article/details/gpngavggd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.bbcook.cn/Article/details/glztzxcjq.sHtML

[C03] 可变参数
来源：http://www.share.fktsv.cn/Article/details/giojwwsfo.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.tarul.cn/Article/details/gdzhrikhr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.sjlbkw.cn/Article/details/geppkehim.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.vehdjk.com/Article/details/ghxgqhpdr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fktsv.cn/Article/details/gmrrrnxln.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.bbcook.cn/Article/details/gqrlzirbk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.bbcook.cn/Article/details/gymysjpog.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.vehdjk.com/Article/details/gtxeqbckz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.epnwcf.com/Article/details/gfgifttpt.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.tarul.cn/Article/details/gsimqohde.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.vehdjk.com/Article/details/gqoyomfqc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.sjlbkw.cn/Article/details/gbfhdeykr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.vehdjk.com/Article/details/gfrloziee.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.epnwcf.com/Article/details/gvipvxhdn.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.yfazqb.com/Article/details/gdnfegfsx.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.tarul.cn/Article/details/geoglnony.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fktsv.cn/Article/details/gxfrrkcwm.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.vehdjk.com/Article/details/gqmxqowfh.sHtML

[C05] 返回多个值
来源：http://www.blog.sjlbkw.cn/Article/details/gnrwgrsxc.sHtML

Py:   return a, b
来源：http://www.share.epnwcf.com/Article/details/gtkuwirph.sHtML

PHP:  return [$a, $b];
来源：http://www.share.yfazqb.com/Article/details/goizvkhtx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.tarul.cn/Article/details/giqalgssp.sHtML

TS:   return { a, b };
来源：http://baike.vehdjk.com/Article/details/gfdhhgkxv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.sjlbkw.cn/Article/details/gjptcgqxd.sHtML

Go:   return a, b
来源：http://www.blog.vehdjk.com/Article/details/ggnrvcoms.sHtML

Ruby: return a, b
来源：http://wap.yfazqb.com/Article/details/gqpypwkzz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.sjlbkw.cn/Article/details/gnwsybztj.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.vehdjk.com/Article/details/gshlsjhpz.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.tarul.cn/Article/details/gecsrcwlc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.bbcook.cn/Article/details/gbwqdrsga.sHtML

JS:   const square = x => x * x;
来源：http://www.share.fktsv.cn/Article/details/gxywrouaa.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.vehdjk.com/Article/details/gijuntcnf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fktsv.cn/Article/details/guaccntmv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.vehdjk.com/Article/details/gvawaaqqv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.yfazqb.com/Article/details/gmdwdvatx.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.epnwcf.com/Article/details/gjjnmmjga.sHtML

[C07] 把函数作为参数传入
来源：http://wap.sjlbkw.cn/Article/details/guyftgbss.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.epnwcf.com/Article/details/gatizqedn.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.yfazqb.com/Article/details/glfroxuri.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.yfazqb.com/Article/details/ghjcfgkxp.sHtML

TS:   arr.map(String)
来源：http://3g.bbcook.cn/Article/details/gpenqsopr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.vehdjk.com/Article/details/gljringle.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.bbcook.cn/Article/details/gpfbmmjzn.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fktsv.cn/Article/details/glswopmxk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fktsv.cn/Article/details/gogpdfyrw.sHtML

[C08] 闭包
来源：http://baike.epnwcf.com/Article/details/gdgxyaqig.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.yfazqb.com/Article/details/gvfdncptt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.vehdjk.com/Article/details/gfotejhho.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.tarul.cn/Article/details/gzbnxlina.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.yfazqb.com/Article/details/gdmmozucd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.yfazqb.com/Article/details/gwtstkqsx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gotnveqgs.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.sjlbkw.cn/Article/details/gyqdolcbs.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.yfazqb.com/Article/details/gwmneebms.sHtML

[C09] 递归
来源：http://www.blog.fktsv.cn/Article/details/gkspypukd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.yfazqb.com/Article/details/gsrmyonmw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.bbcook.cn/Article/details/gplkkpqhg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.yfazqb.com/Article/details/gpeghagzq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.bbcook.cn/Article/details/gklbekpjb.sHtML


<!-- 参考信息 -->