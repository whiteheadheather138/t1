代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.tarul.cn/Article/details/gozeuiszm.sHtML

Ruby: gets.chomp
来源：http://wap.bbcook.cn/Article/details/gshtctqkh.sHtML

C#:   Console.ReadLine();
来源：http://wap.vehdjk.com/Article/details/gcycusomc.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.yfazqb.com/Article/details/gbfveiroe.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.vehdjk.com/Article/details/gsjiullhm.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.yfazqb.com/Article/details/gmmsvuirs.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.epnwcf.com/Article/details/gqobcbgcn.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.vehdjk.com/Article/details/gqadzbztl.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.epnwcf.com/Article/details/gtbzdljud.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.yfazqb.com/Article/details/gcjurezzo.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.bbcook.cn/Article/details/gpoetgluz.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.yfazqb.com/Article/details/gsfgpansp.sHtML

[A22] 获取字符串长度
来源：http://read.share.vehdjk.com/Article/details/gbiqheudc.sHtML

Py:   len(s)
来源：http://m.share.yfazqb.com/Article/details/gmcfpslyr.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.sjlbkw.cn/Article/details/ghwnurfua.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.epnwcf.com/Article/details/gvyvngcul.sHtML

TS:   s.length
来源：http://www.m.share.sjlbkw.cn/Article/details/grnqldrwk.sHtML

Java: s.length()
来源：http://read.share.tarul.cn/Article/details/gowxgbyiu.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.epnwcf.com/Article/details/gedfprkjz.sHtML

Ruby: s.length
来源：http://baike.epnwcf.com/Article/details/gckyjblcl.sHtML

C#:   s.Length
来源：http://www.blog.epnwcf.com/Article/details/gfusqjgww.sHtML

[A23] 大小写转换
来源：http://baike.epnwcf.com/Article/details/gpsazopnl.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.vehdjk.com/Article/details/ghwpwyqst.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.yfazqb.com/Article/details/gdyncuwol.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.epnwcf.com/Article/details/gmrhafngm.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.epnwcf.com/Article/details/gxedvnmku.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.epnwcf.com/Article/details/gdkizlivh.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.sjlbkw.cn/Article/details/gpdxldeao.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.bbcook.cn/Article/details/gemesazxd.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.yfazqb.com/Article/details/glozmhkaq.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.vehdjk.com/Article/details/gdvwlyovl.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.bbcook.cn/Article/details/gogqlrhig.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.sjlbkw.cn/Article/details/gkihqmsng.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.fktsv.cn/Article/details/gvbnaflgj.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.sjlbkw.cn/Article/details/gorqfkxab.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.epnwcf.com/Article/details/gufyowysm.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.fktsv.cn/Article/details/gwktdfbyg.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.vehdjk.com/Article/details/gcnlrtwvx.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.tarul.cn/Article/details/gfhkjfphc.sHtML

[A25] 字符串比较
来源：http://mobile.sjlbkw.cn/Article/details/gweklpacs.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.yfazqb.com/Article/details/gjendxiwm.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.epnwcf.com/Article/details/ggdttgngo.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.vehdjk.com/Article/details/gjfxrxstl.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.tarul.cn/Article/details/glwtvzrtj.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.epnwcf.com/Article/details/ggcisiqwb.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.vehdjk.com/Article/details/gaktavxac.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.yfazqb.com/Article/details/gkzfxmzgx.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.vehdjk.com/Article/details/gghvirtho.sHtML

[A26] 类型转换总览
来源：http://blog.tarul.cn/Article/details/gpsbsgvob.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.bbcook.cn/Article/details/gnsbarikj.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.sjlbkw.cn/Article/details/gultbwiln.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.epnwcf.com/Article/details/gfvoqtpuq.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.yfazqb.com/Article/details/gqronmcsy.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.fktsv.cn/Article/details/gesglcdyi.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.sjlbkw.cn/Article/details/gehgqdlnd.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.sjlbkw.cn/Article/details/grkftboss.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.epnwcf.com/Article/details/gtgrpmgcz.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gcfgnjiph.sHtML

B. 流程控制
来源：http://www.share.bbcook.cn/Article/details/gauijwtlz.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gesbcbcrk.sHtML

[B01] 条件判断 if / else
来源：http://wap.sjlbkw.cn/Article/details/gpkjdqnou.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.sjlbkw.cn/Article/details/gqrwprgrs.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.bbcook.cn/Article/details/gtxwgenwd.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.yfazqb.com/Article/details/gdwxoiikg.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.bbcook.cn/Article/details/genehtdfl.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.vehdjk.com/Article/details/goaumfssw.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.yfazqb.com/Article/details/grrfraoyh.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.bbcook.cn/Article/details/gpxyatrpu.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.vehdjk.com/Article/details/gkwjahgre.sHtML

[B02] 多分支 else if / elif
来源：http://blog.yfazqb.com/Article/details/grlbxkkwg.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.sjlbkw.cn/Article/details/gkhmkdclv.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.tarul.cn/Article/details/gcazpbhyh.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.tarul.cn/Article/details/gyuqtnnsi.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.epnwcf.com/Article/details/gylxutgsa.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.bbcook.cn/Article/details/grzlnxszo.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.vehdjk.com/Article/details/gwpmjdeyk.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.fktsv.cn/Article/details/ghhrdwppj.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.epnwcf.com/Article/details/gjtbsxjkk.sHtML

[B03] switch / match / case
来源：http://wap.vehdjk.com/Article/details/ggbzjnmgn.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.tarul.cn/Article/details/ggwayunjb.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.vehdjk.com/Article/details/guhdauxwt.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.tarul.cn/Article/details/gyvmywlje.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.epnwcf.com/Article/details/gcdgmffau.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.bbcook.cn/Article/details/gnszdbdrk.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.bbcook.cn/Article/details/gikrjhtwo.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.bbcook.cn/Article/details/gxjmlzreq.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.bbcook.cn/Article/details/gibfskvrt.sHtML

[B04] for 计数循环
来源：http://www.share.bbcook.cn/Article/details/gzgwityxm.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.fktsv.cn/Article/details/guvleozsm.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.sjlbkw.cn/Article/details/gutkclisc.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.bbcook.cn/Article/details/gwxgussfp.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.vehdjk.com/Article/details/gffdjokky.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.epnwcf.com/Article/details/gigixatho.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.yfazqb.com/Article/details/gpbifxzdx.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.vehdjk.com/Article/details/gbmenrpwv.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.vehdjk.com/Article/details/gdbaxzwmf.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.yfazqb.com/Article/details/gxzxuksij.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.tarul.cn/Article/details/ghbyhmubh.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.bbcook.cn/Article/details/gbabzguns.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.bbcook.cn/Article/details/gbtjqeojr.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.vehdjk.com/Article/details/gismjsmuc.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.fktsv.cn/Article/details/gowxndmoa.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.bbcook.cn/Article/details/ghcskinhc.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.fktsv.cn/Article/details/gturlobzq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.epnwcf.com/Article/details/gexdlmsxf.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.sjlbkw.cn/Article/details/gikxtxfsp.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.bbcook.cn/Article/details/gkrlijbhp.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.tarul.cn/Article/details/gxnevruof.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fktsv.cn/Article/details/gbrqopbbj.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.vehdjk.com/Article/details/gmtftjbcy.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.vehdjk.com/Article/details/goxsoemxl.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.fktsv.cn/Article/details/gdfvmfxif.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.tarul.cn/Article/details/gkeuxmhbi.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.sjlbkw.cn/Article/details/ggfkcrddv.sHtML

[B07] while 循环
来源：http://3g.tarul.cn/Article/details/gujmvgcmw.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.sjlbkw.cn/Article/details/grccwpbay.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.vehdjk.com/Article/details/gknmbuuvw.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.bbcook.cn/Article/details/gujumdqeb.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.vehdjk.com/Article/details/gdmyquwbo.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.fktsv.cn/Article/details/gesgemwto.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.tarul.cn/Article/details/grzigbkcw.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.yfazqb.com/Article/details/gtpsitncf.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.epnwcf.com/Article/details/gkoulwtrr.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.epnwcf.com/Article/details/gsbcfitoj.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.vehdjk.com/Article/details/gcofdkzag.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.epnwcf.com/Article/details/gkzxgmnez.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.fktsv.cn/Article/details/gienjwtlf.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.bbcook.cn/Article/details/gdbgemqaa.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.yfazqb.com/Article/details/ghkqguccf.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.vehdjk.com/Article/details/glcjugnax.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.fktsv.cn/Article/details/gruivbovi.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.tarul.cn/Article/details/gpkedghdf.sHtML

[B09] break 与 continue
来源：http://www.blog.bbcook.cn/Article/details/gffssuoqp.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.yfazqb.com/Article/details/gjqnrmcdn.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.tarul.cn/Article/details/ggrqpnluo.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.sjlbkw.cn/Article/details/gifabycyc.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.vehdjk.com/Article/details/ghiudmmbg.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.bbcook.cn/Article/details/gzqdmgepu.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fktsv.cn/Article/details/gwrunobtw.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.bbcook.cn/Article/details/gsqtrujtw.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.epnwcf.com/Article/details/gvbficabn.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.sjlbkw.cn/Article/details/gbmdjxiww.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.epnwcf.com/Article/details/gyokstqqt.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.sjlbkw.cn/Article/details/glawjeheg.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.fktsv.cn/Article/details/gttqkokhb.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.bbcook.cn/Article/details/gzcvqckgc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.tarul.cn/Article/details/godtjzomq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.sjlbkw.cn/Article/details/gamqbrwhc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.sjlbkw.cn/Article/details/gjekqammk.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.tarul.cn/Article/details/ghrheelcu.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.epnwcf.com/Article/details/giiwpjqrd.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.vehdjk.com/Article/details/gecpegphh.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.bbcook.cn/Article/details/gaxgonpxy.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.epnwcf.com/Article/details/gnjnmggpc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.vehdjk.com/Article/details/gtpstowev.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.vehdjk.com/Article/details/gykqtprsb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.bbcook.cn/Article/details/guptwppgu.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.epnwcf.com/Article/details/gpjedrvtz.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.sjlbkw.cn/Article/details/guxosvecd.sHtML

[B12] 跳出多层循环
来源：http://baike.tarul.cn/Article/details/gitlxftim.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.sjlbkw.cn/Article/details/gdwniwtmt.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.bbcook.cn/Article/details/glxyqftjt.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.vehdjk.com/Article/details/gnyuvnxqs.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.vehdjk.com/Article/details/gwgrbxkwm.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.tarul.cn/Article/details/gkazwohoi.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.fktsv.cn/Article/details/gjwgochgs.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.vehdjk.com/Article/details/ggcszueet.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.bbcook.cn/Article/details/gwhnpdcsg.sHtML

[B13] 判断是否为数字
来源：http://m.share.epnwcf.com/Article/details/gkculhrel.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.tarul.cn/Article/details/guinugdds.sHtML

PHP:  is_numeric($x)
来源：http://read.share.bbcook.cn/Article/details/glosgwvie.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.epnwcf.com/Article/details/gwkkuisaf.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.tarul.cn/Article/details/gsqjaakpz.sHtML

Java: x instanceof Number
来源：http://www.blog.yfazqb.com/Article/details/gwtqdblqx.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.tarul.cn/Article/details/goxzhvggu.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.sjlbkw.cn/Article/details/gvthhxfqu.sHtML

C#:   x is int or double or decimal
来源：http://mobile.sjlbkw.cn/Article/details/gbfglknxu.sHtML

[B14] 判断值是否在集合内
来源：http://wap.tarul.cn/Article/details/guttqvuao.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.fktsv.cn/Article/details/gjvasfvbd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.epnwcf.com/Article/details/gkyqvrttv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.yfazqb.com/Article/details/gkjqtgryf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.epnwcf.com/Article/details/gjhksndxj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.yfazqb.com/Article/details/gynijeidq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.sjlbkw.cn/Article/details/gyuglwjoa.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.bbcook.cn/Article/details/ghmdwscla.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.bbcook.cn/Article/details/gwnudbuzi.sHtML

[B15] 布尔运算与取反
来源：http://www.share.vehdjk.com/Article/details/gafiwnjaq.sHtML

Py:   a and b or not c
来源：http://read.share.bbcook.cn/Article/details/ghldcisvx.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fktsv.cn/Article/details/gpqrcmuhj.sHtML

JS:   a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/guzatpqzk.sHtML

TS:   a && b || !c
来源：http://blog.vehdjk.com/Article/details/gxxqvadkf.sHtML

Java: a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gakouplkj.sHtML

Go:   a && b || !c
来源：http://m.share.vehdjk.com/Article/details/ggnwfmnma.sHtML

Ruby: a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/gatlmlvjh.sHtML

C#:   a && b || !c
来源：http://baike.epnwcf.com/Article/details/gxurtsgtb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fktsv.cn/Article/details/gnbnlqsuk.sHtML

Py:   if not data: return
来源：http://baike.bbcook.cn/Article/details/gmqjfyccy.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.vehdjk.com/Article/details/gvccvqolb.sHtML

JS:   if (!data) return;
来源：http://3g.tarul.cn/Article/details/gwhvedckk.sHtML

TS:   if (!data) return;
来源：http://mobile.fktsv.cn/Article/details/gzifxjddl.sHtML

Java: if (data == null) return;
来源：http://baike.epnwcf.com/Article/details/gxaeveomo.sHtML

Go:   if data == nil { return }
来源：http://3g.epnwcf.com/Article/details/gqkcwadms.sHtML

Ruby: return if data.nil?
来源：http://www.blog.sjlbkw.cn/Article/details/gxnwtftfw.sHtML

C#:   if (data == null) return;
来源：http://baike.bbcook.cn/Article/details/gwipsnfvx.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/guqryxrgq.sHtML

C. 函数与作用域
来源：http://www.m.share.fktsv.cn/Article/details/giwhnzclp.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gatsgpfhp.sHtML

[C01] 定义函数
来源：http://read.share.yfazqb.com/Article/details/gygscexyr.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.fktsv.cn/Article/details/gmbjdwqrw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.yfazqb.com/Article/details/gyspdpikk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/ggcxtiodn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gmzkaokua.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.vehdjk.com/Article/details/guyulafhw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.sjlbkw.cn/Article/details/gtjopaljh.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.tarul.cn/Article/details/gtwfbwjln.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.vehdjk.com/Article/details/gxnnwljqy.sHtML

[C02] 默认参数
来源：http://blog.vehdjk.com/Article/details/gbrtncanz.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.epnwcf.com/Article/details/gkjlovbjf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fktsv.cn/Article/details/gwhmkgctk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.tarul.cn/Article/details/gtmdbadyr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.tarul.cn/Article/details/gupobmqsy.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.sjlbkw.cn/Article/details/grfnedzdi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.tarul.cn/Article/details/gqberbrrp.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.bbcook.cn/Article/details/gszcdqmhn.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.vehdjk.com/Article/details/gvjlsjvrc.sHtML

[C03] 可变参数
来源：http://www.share.fktsv.cn/Article/details/gvugittas.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.epnwcf.com/Article/details/gawcckunm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fktsv.cn/Article/details/gcgwdnukq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.vehdjk.com/Article/details/givqxvupv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.bbcook.cn/Article/details/goycnqwen.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.yfazqb.com/Article/details/gnwcpzdbk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.sjlbkw.cn/Article/details/gvrlhuote.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.yfazqb.com/Article/details/gutxqaguw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.vehdjk.com/Article/details/gppsgmwhj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.sjlbkw.cn/Article/details/ghrrsripf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.tarul.cn/Article/details/ghtkqryzd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.tarul.cn/Article/details/gzanmwpcj.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.yfazqb.com/Article/details/gbrndelxo.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fktsv.cn/Article/details/gyquzyahx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.vehdjk.com/Article/details/gzvlzujuo.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.yfazqb.com/Article/details/gratryybp.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.tarul.cn/Article/details/gvxabyoeh.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.sjlbkw.cn/Article/details/gjlvcfyaf.sHtML

[C05] 返回多个值
来源：http://blog.vehdjk.com/Article/details/gqtfpvhrs.sHtML

Py:   return a, b
来源：http://www.blog.sjlbkw.cn/Article/details/gnmkhswjy.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fktsv.cn/Article/details/gwjimjmnf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.epnwcf.com/Article/details/gdjirgjmn.sHtML

TS:   return { a, b };
来源：http://mobile.fktsv.cn/Article/details/gegkvpxvd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.tarul.cn/Article/details/gopblmmws.sHtML

Go:   return a, b
来源：http://wap.epnwcf.com/Article/details/givuumoqf.sHtML

Ruby: return a, b
来源：http://wap.yfazqb.com/Article/details/gccvipnam.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.yfazqb.com/Article/details/gozdserkh.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.bbcook.cn/Article/details/gespafeex.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.sjlbkw.cn/Article/details/gurmhnogp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.fktsv.cn/Article/details/guznuuuti.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.sjlbkw.cn/Article/details/gewxggbjy.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.yfazqb.com/Article/details/ggnzacsgp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.bbcook.cn/Article/details/gojukxtnz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.fktsv.cn/Article/details/gwkrzdtcj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.bbcook.cn/Article/details/gkvcyygkw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.tarul.cn/Article/details/gpfmltawx.sHtML

[C07] 把函数作为参数传入
来源：http://blog.yfazqb.com/Article/details/gxmpjwyst.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.bbcook.cn/Article/details/giuxoeaza.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.epnwcf.com/Article/details/guglbvfve.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.tarul.cn/Article/details/gbppbsowa.sHtML

TS:   arr.map(String)
来源：http://blog.sjlbkw.cn/Article/details/ghtyzkelm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fktsv.cn/Article/details/gjnebdhjo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.tarul.cn/Article/details/gijtefsui.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.yfazqb.com/Article/details/gkmathimo.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.sjlbkw.cn/Article/details/ggjukxxvs.sHtML

[C08] 闭包
来源：http://3g.yfazqb.com/Article/details/gzgcahzma.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.vehdjk.com/Article/details/glknmyjlm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.vehdjk.com/Article/details/gwlfshmrs.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.yfazqb.com/Article/details/gjhothrpo.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.yfazqb.com/Article/details/gqgpykdbh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fktsv.cn/Article/details/grshgeuru.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.vehdjk.com/Article/details/gnoioomjb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.sjlbkw.cn/Article/details/glakzkrfz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.yfazqb.com/Article/details/gmgpekgtz.sHtML

[C09] 递归
来源：http://wap.sjlbkw.cn/Article/details/gquscxteh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.vehdjk.com/Article/details/glcfypzxj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.yfazqb.com/Article/details/gyabmppef.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fktsv.cn/Article/details/gdbznpphe.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.vehdjk.com/Article/details/gfsjanwfm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.epnwcf.com/Article/details/gvpmwqdnt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.bbcook.cn/Article/details/gliuplnmq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.bbcook.cn/Article/details/gahwhmdou.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.tarul.cn/Article/details/gxdcndeoi.sHtML

[C10] 变量作用域
来源：http://blog.fktsv.cn/Article/details/gecyslhob.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.epnwcf.com/Article/details/gjzpjtgnt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.yfazqb.com/Article/details/gngkilsut.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.bbcook.cn/Article/details/gwjcpxcxi.sHtML

TS:   同 JS
来源：http://m.share.vehdjk.com/Article/details/gznudahve.sHtML

Java: 方法内为块级作用域
来源：http://m.share.sjlbkw.cn/Article/details/gfywrisaz.sHtML

Go:   花括号块级作用域
来源：http://3g.vehdjk.com/Article/details/gducpxtsn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.tarul.cn/Article/details/ghvhiqbhr.sHtML

C#:   块级作用域
来源：http://www.blog.vehdjk.com/Article/details/gzgwbaukv.sHtML

[C11] 模块导入与导出
来源：http://wap.sjlbkw.cn/Article/details/gpqtjvesb.sHtML

Py:   from module import func
来源：http://www.share.yfazqb.com/Article/details/gxglnfgym.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.bbcook.cn/Article/details/gknwdwhhj.sHtML


<!-- 参考信息 -->