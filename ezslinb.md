代发 wailian999

[A26] 类型转换总览
来源：http://baike.bbcook.cn/Article/details/gzrxgpysw.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.tarul.cn/Article/details/gthtwqxai.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.sjlbkw.cn/Article/details/gohauynbf.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.vehdjk.com/Article/details/gluvbhdod.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.tarul.cn/Article/details/gyaexdepc.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.vehdjk.com/Article/details/gpbbavmnp.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.bbcook.cn/Article/details/gfzvekezm.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.tarul.cn/Article/details/gazdmlsjo.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.fktsv.cn/Article/details/gzbfxuszt.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/guicofwhk.sHtML

B. 流程控制
来源：http://wap.vehdjk.com/Article/details/gwwbvtbbd.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gpsxugapt.sHtML

[B01] 条件判断 if / else
来源：http://3g.fktsv.cn/Article/details/gqykwrhek.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.fktsv.cn/Article/details/glfhskrzm.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.vehdjk.com/Article/details/gweczzmge.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.epnwcf.com/Article/details/grjrselup.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.epnwcf.com/Article/details/gqjgoktef.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.yfazqb.com/Article/details/gemnfhcba.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.yfazqb.com/Article/details/gnpfwlmak.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.bbcook.cn/Article/details/geauofoii.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.sjlbkw.cn/Article/details/gzbqfjixx.sHtML

[B02] 多分支 else if / elif
来源：http://3g.sjlbkw.cn/Article/details/gqbqzcrnb.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.bbcook.cn/Article/details/gueugjtxr.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.vehdjk.com/Article/details/gmropaebv.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.tarul.cn/Article/details/gbsoctkrv.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.tarul.cn/Article/details/groixmosk.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fktsv.cn/Article/details/gcrbobojo.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.yfazqb.com/Article/details/gmkyodxbw.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.bbcook.cn/Article/details/gmoiyswws.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fktsv.cn/Article/details/gwdbekwvz.sHtML

[B03] switch / match / case
来源：http://www.m.share.bbcook.cn/Article/details/gcvwmohgl.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.fktsv.cn/Article/details/gtzmjfsea.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.yfazqb.com/Article/details/govwgwnod.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.vehdjk.com/Article/details/gudpjytex.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.fktsv.cn/Article/details/givjaqkrh.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.epnwcf.com/Article/details/gyvhgalgp.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.vehdjk.com/Article/details/gtocdvzrm.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.bbcook.cn/Article/details/gxdolhwnm.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.vehdjk.com/Article/details/guimvnhdz.sHtML

[B04] for 计数循环
来源：http://mobile.tarul.cn/Article/details/guypvufox.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.vehdjk.com/Article/details/ggntpxubt.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.sjlbkw.cn/Article/details/gejvfsqkn.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fktsv.cn/Article/details/gzxsfsruk.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.yfazqb.com/Article/details/gcfzrgkel.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.fktsv.cn/Article/details/gjqbwdlqs.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.bbcook.cn/Article/details/gyhqexpit.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.fktsv.cn/Article/details/gbpifnlfh.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.vehdjk.com/Article/details/grcuzlqqr.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.tarul.cn/Article/details/guzlpwsxt.sHtML

Py:   for item in arr: print(item)
来源：http://3g.tarul.cn/Article/details/gednzgqsf.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.bbcook.cn/Article/details/ggazmtyqx.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.fktsv.cn/Article/details/geodzbccz.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.tarul.cn/Article/details/gsqnbgvwt.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.sjlbkw.cn/Article/details/gnmbywjja.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.tarul.cn/Article/details/gbcrrwmbq.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.vehdjk.com/Article/details/gmzjiwkst.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.yfazqb.com/Article/details/gkbszwxxg.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.bbcook.cn/Article/details/gkuihdgit.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.fktsv.cn/Article/details/gthyrdlde.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.vehdjk.com/Article/details/gtwmcicsh.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.epnwcf.com/Article/details/gwjjakllq.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.sjlbkw.cn/Article/details/gwfqgnzha.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.yfazqb.com/Article/details/gcousrypk.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.fktsv.cn/Article/details/ghqsgcfcr.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.epnwcf.com/Article/details/gvsbkkudn.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.sjlbkw.cn/Article/details/goschjxou.sHtML

[B07] while 循环
来源：http://blog.sjlbkw.cn/Article/details/glcaaxujj.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.bbcook.cn/Article/details/gewyywtoa.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.tarul.cn/Article/details/gtveqdocd.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.fktsv.cn/Article/details/gjvhneilb.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.sjlbkw.cn/Article/details/gbufwzonr.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.bbcook.cn/Article/details/gotjvelhr.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.sjlbkw.cn/Article/details/gngjgcviu.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.fktsv.cn/Article/details/gugpebgmd.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.vehdjk.com/Article/details/gbwumjsmc.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.yfazqb.com/Article/details/gkdmlugot.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.yfazqb.com/Article/details/gjzsfisjv.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.fktsv.cn/Article/details/ggvkqetec.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.bbcook.cn/Article/details/gcufksgwp.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.sjlbkw.cn/Article/details/glbywowfr.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.sjlbkw.cn/Article/details/geijirncr.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.vehdjk.com/Article/details/glloplsag.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.bbcook.cn/Article/details/gcglkegvp.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.sjlbkw.cn/Article/details/gxnzhmwqn.sHtML

[B09] break 与 continue
来源：http://read.share.sjlbkw.cn/Article/details/gbmombfuh.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.bbcook.cn/Article/details/gvcmheeah.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.epnwcf.com/Article/details/gjwbkelfa.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fktsv.cn/Article/details/gsfjehpeh.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fktsv.cn/Article/details/gdtbsmzuv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.epnwcf.com/Article/details/gqgllmyuo.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.bbcook.cn/Article/details/gsdlbkcsk.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.bbcook.cn/Article/details/gebezotcp.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.tarul.cn/Article/details/gycrwmusi.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.fktsv.cn/Article/details/gpkhmigqi.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.tarul.cn/Article/details/gsadqbzon.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.tarul.cn/Article/details/guoxgomqw.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.bbcook.cn/Article/details/govfhsfsd.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.epnwcf.com/Article/details/ggtzdamuu.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.vehdjk.com/Article/details/gflayxbwl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.vehdjk.com/Article/details/gbhbqpmow.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.tarul.cn/Article/details/gatbxfasd.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.tarul.cn/Article/details/gsvikrsdv.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.yfazqb.com/Article/details/gtxdlfjla.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.tarul.cn/Article/details/gcfcibltl.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.yfazqb.com/Article/details/gqaffkzha.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.epnwcf.com/Article/details/geegtrraf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.bbcook.cn/Article/details/gxmqifimz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.vehdjk.com/Article/details/gynsmirot.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.bbcook.cn/Article/details/gktcddajo.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.fktsv.cn/Article/details/gzalozchy.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.tarul.cn/Article/details/gkkqzrnsk.sHtML

[B12] 跳出多层循环
来源：http://3g.epnwcf.com/Article/details/gimzdesln.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.tarul.cn/Article/details/gndnytsed.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.epnwcf.com/Article/details/gngoftgqi.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.bbcook.cn/Article/details/gjbmwzvkt.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.yfazqb.com/Article/details/glrfubxzl.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.epnwcf.com/Article/details/gsuywuhhz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.yfazqb.com/Article/details/gvabassbn.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.bbcook.cn/Article/details/gsghyposq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.epnwcf.com/Article/details/gzqtxefja.sHtML

[B13] 判断是否为数字
来源：http://blog.fktsv.cn/Article/details/gwzttvwpo.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.tarul.cn/Article/details/gisiikxdh.sHtML

PHP:  is_numeric($x)
来源：http://m.share.sjlbkw.cn/Article/details/gtoejduqf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.tarul.cn/Article/details/grsnwmfyk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.vehdjk.com/Article/details/gvrqcujbh.sHtML

Java: x instanceof Number
来源：http://m.share.bbcook.cn/Article/details/gacrlhdpy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.bbcook.cn/Article/details/gevmljhdd.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.epnwcf.com/Article/details/gobcsause.sHtML

C#:   x is int or double or decimal
来源：http://m.share.vehdjk.com/Article/details/ghijvrchs.sHtML

[B14] 判断值是否在集合内
来源：http://wap.epnwcf.com/Article/details/gxhdhhupf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.bbcook.cn/Article/details/gufaeotua.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.tarul.cn/Article/details/gzqkxphff.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.tarul.cn/Article/details/gtkdxsmrq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.sjlbkw.cn/Article/details/gzfyzwtms.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.tarul.cn/Article/details/gxmlfyfae.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.epnwcf.com/Article/details/gsckwqyxg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.fktsv.cn/Article/details/gpukmmvbz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.epnwcf.com/Article/details/gwhcbwlfo.sHtML

[B15] 布尔运算与取反
来源：http://www.share.bbcook.cn/Article/details/gmxazswvb.sHtML

Py:   a and b or not c
来源：http://baike.vehdjk.com/Article/details/ggghvrdbt.sHtML

PHP:  $a && $b || !$c
来源：http://blog.bbcook.cn/Article/details/gytvjnfui.sHtML

JS:   a && b || !c
来源：http://3g.bbcook.cn/Article/details/grdhsmaqc.sHtML

TS:   a && b || !c
来源：http://3g.yfazqb.com/Article/details/gsbyiyqch.sHtML

Java: a && b || !c
来源：http://www.blog.epnwcf.com/Article/details/gemssjnim.sHtML

Go:   a && b || !c
来源：http://blog.sjlbkw.cn/Article/details/gytlgxdut.sHtML

Ruby: a && b || !c
来源：http://www.m.share.bbcook.cn/Article/details/gvpakzvhv.sHtML

C#:   a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gzhzevjgl.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.bbcook.cn/Article/details/gyiapjcxx.sHtML

Py:   if not data: return
来源：http://m.share.yfazqb.com/Article/details/gzfperfxt.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.yfazqb.com/Article/details/guzbdlpny.sHtML

JS:   if (!data) return;
来源：http://3g.fktsv.cn/Article/details/gxvnaznjx.sHtML

TS:   if (!data) return;
来源：http://www.share.bbcook.cn/Article/details/gkobljyrg.sHtML

Java: if (data == null) return;
来源：http://3g.sjlbkw.cn/Article/details/gnbrkqaav.sHtML

Go:   if data == nil { return }
来源：http://3g.tarul.cn/Article/details/gkqfetglq.sHtML

Ruby: return if data.nil?
来源：http://m.share.tarul.cn/Article/details/gsacliegx.sHtML

C#:   if (data == null) return;
来源：http://mobile.yfazqb.com/Article/details/glebpwgxm.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gftklszeg.sHtML

C. 函数与作用域
来源：http://blog.yfazqb.com/Article/details/goduwnmzw.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gwfzfmhoz.sHtML

[C01] 定义函数
来源：http://www.share.bbcook.cn/Article/details/ghslavahe.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.vehdjk.com/Article/details/gqaxuvfrq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.bbcook.cn/Article/details/gpcseulmi.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gpqbplayz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/geszjztgn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gzddbgidt.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.fktsv.cn/Article/details/guetmzvxs.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.tarul.cn/Article/details/glghfpnju.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gmbdyrmnv.sHtML

[C02] 默认参数
来源：http://www.m.share.vehdjk.com/Article/details/gmohibgfp.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.tarul.cn/Article/details/gszvpsdeh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.sjlbkw.cn/Article/details/gtuacetoy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.bbcook.cn/Article/details/guoqjlabq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gqmrbkfkc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.yfazqb.com/Article/details/grneqiptf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.epnwcf.com/Article/details/gcaapxute.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.tarul.cn/Article/details/gjhczsanv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.bbcook.cn/Article/details/gyghxrcbj.sHtML

[C03] 可变参数
来源：http://m.share.sjlbkw.cn/Article/details/gjvrydcfu.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.sjlbkw.cn/Article/details/gcwdhgigc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.fktsv.cn/Article/details/gxukjmwjk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fktsv.cn/Article/details/gwfprelwn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fktsv.cn/Article/details/gfbyooruw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkokkcufj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.sjlbkw.cn/Article/details/geknhflrf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.yfazqb.com/Article/details/geohonvqa.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.tarul.cn/Article/details/gtajqbgzq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.tarul.cn/Article/details/gxuidfrhe.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.epnwcf.com/Article/details/ghydmgabp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.vehdjk.com/Article/details/gfpyublws.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.vehdjk.com/Article/details/gjfmzxxgv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.sjlbkw.cn/Article/details/geflybxmp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.epnwcf.com/Article/details/gmbvpfvda.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.bbcook.cn/Article/details/gtnrcbgji.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.epnwcf.com/Article/details/giefnuwrr.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.yfazqb.com/Article/details/gjyxpvtvu.sHtML

[C05] 返回多个值
来源：http://wap.fktsv.cn/Article/details/gcurybdwm.sHtML

Py:   return a, b
来源：http://wap.sjlbkw.cn/Article/details/ggjblvtty.sHtML

PHP:  return [$a, $b];
来源：http://3g.vehdjk.com/Article/details/gtzmngfcp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.yfazqb.com/Article/details/gsusfibrn.sHtML

TS:   return { a, b };
来源：http://mobile.tarul.cn/Article/details/gvnqtkgpt.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.yfazqb.com/Article/details/gbmjbxngl.sHtML

Go:   return a, b
来源：http://blog.epnwcf.com/Article/details/guuztlkgg.sHtML

Ruby: return a, b
来源：http://wap.bbcook.cn/Article/details/gdospjlob.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.epnwcf.com/Article/details/gdfchzufm.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.yfazqb.com/Article/details/gaabactyr.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.sjlbkw.cn/Article/details/gneuzrzax.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.fktsv.cn/Article/details/grzdqvygy.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.epnwcf.com/Article/details/gligafcuv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fktsv.cn/Article/details/gzytnmgxs.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.tarul.cn/Article/details/ghlwxgrso.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.fktsv.cn/Article/details/gixneqbrs.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.epnwcf.com/Article/details/gvfthwznt.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.tarul.cn/Article/details/grscaxsbk.sHtML

[C07] 把函数作为参数传入
来源：http://wap.tarul.cn/Article/details/gckouyzgk.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.vehdjk.com/Article/details/gifmvcblt.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.fktsv.cn/Article/details/gmurkilnx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.vehdjk.com/Article/details/gbtcwljkq.sHtML

TS:   arr.map(String)
来源：http://wap.vehdjk.com/Article/details/gfljsdlka.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.yfazqb.com/Article/details/govtrbbxv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.epnwcf.com/Article/details/gfmdqcjyl.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.epnwcf.com/Article/details/gdppjwntm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.vehdjk.com/Article/details/garcrxbnb.sHtML

[C08] 闭包
来源：http://blog.tarul.cn/Article/details/gyrgyjjcp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.bbcook.cn/Article/details/gfhojckum.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.epnwcf.com/Article/details/ghlfyqxvi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.vehdjk.com/Article/details/gngusnyke.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.bbcook.cn/Article/details/gqfzrtblf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.yfazqb.com/Article/details/gsprzjngl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.bbcook.cn/Article/details/gtbsnsnxs.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.yfazqb.com/Article/details/gronpvoxs.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.sjlbkw.cn/Article/details/gtmelvszb.sHtML

[C09] 递归
来源：http://read.share.sjlbkw.cn/Article/details/gpdcrvczs.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.epnwcf.com/Article/details/gqnqjvzav.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.bbcook.cn/Article/details/goyblhiqb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.vehdjk.com/Article/details/gifdetvsb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.epnwcf.com/Article/details/gqtdttumj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.sjlbkw.cn/Article/details/gsbosofrj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.bbcook.cn/Article/details/gibnelpbx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.epnwcf.com/Article/details/gdrgxwyjt.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.vehdjk.com/Article/details/guqrspwhw.sHtML

[C10] 变量作用域
来源：http://3g.yfazqb.com/Article/details/gaprxnuxj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fktsv.cn/Article/details/ghgubuzeu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.sjlbkw.cn/Article/details/goxqgcbxh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.epnwcf.com/Article/details/gzynffdth.sHtML

TS:   同 JS
来源：http://wap.yfazqb.com/Article/details/gjvzdrsry.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fktsv.cn/Article/details/gxegxzwwc.sHtML

Go:   花括号块级作用域
来源：http://read.share.fktsv.cn/Article/details/guwfepebu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fktsv.cn/Article/details/gngvljoac.sHtML

C#:   块级作用域
来源：http://3g.sjlbkw.cn/Article/details/gysxqoard.sHtML

[C11] 模块导入与导出
来源：http://baike.tarul.cn/Article/details/gqrecegyk.sHtML

Py:   from module import func
来源：http://read.share.fktsv.cn/Article/details/glzbbnikb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.vehdjk.com/Article/details/gqbkrjfgh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.yfazqb.com/Article/details/gkyzbnhmo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fktsv.cn/Article/details/gxfqgnoso.sHtML

Java: import java.util.List;
来源：http://blog.tarul.cn/Article/details/gysfppnze.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.vehdjk.com/Article/details/gnspsijsr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.tarul.cn/Article/details/gqqzekfuo.sHtML

C#:   using System.Text;
来源：http://blog.vehdjk.com/Article/details/ghmycsaru.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fktsv.cn/Article/details/gavyiytyj.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.bbcook.cn/Article/details/gdavmsfge.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.vehdjk.com/Article/details/gjoehvsxl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.vehdjk.com/Article/details/giqpprzet.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fktsv.cn/Article/details/ggdfvuzih.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.sjlbkw.cn/Article/details/glsvsavhw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.bbcook.cn/Article/details/gcxuwkzsw.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.vehdjk.com/Article/details/gilghvjbb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fktsv.cn/Article/details/ghqkraybg.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.yfazqb.com/Article/details/gccnuacap.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.sjlbkw.cn/Article/details/gcmyuvevt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.epnwcf.com/Article/details/gurhaxiur.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.yfazqb.com/Article/details/gycyjgdmu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.tarul.cn/Article/details/gjsecmvak.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/gxznzkafz.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.vehdjk.com/Article/details/gijgpumla.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.bbcook.cn/Article/details/gftrqpxmz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.epnwcf.com/Article/details/gkyednmlc.sHtML

[C14] 泛型函数
来源：http://3g.yfazqb.com/Article/details/gxnfirqec.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.bbcook.cn/Article/details/girokuewx.sHtML

PHP:  // 无泛型
来源：http://www.m.share.vehdjk.com/Article/details/gjnmtitzp.sHtML

JS:   // 无泛型
来源：http://mobile.sjlbkw.cn/Article/details/gvuvvvwoz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.epnwcf.com/Article/details/gignkfzta.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.tarul.cn/Article/details/gstyphfhh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.epnwcf.com/Article/details/gcjgvlcsz.sHtML

Ruby: # 无泛型
来源：http://www.m.share.yfazqb.com/Article/details/gcokyhlaz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.bbcook.cn/Article/details/ghlfawdli.sHtML

[C15] 解构 / 展开参数
来源：http://wap.vehdjk.com/Article/details/gxbishigp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.bbcook.cn/Article/details/gibztkcsq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.tarul.cn/Article/details/gjkzjsmhl.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.tarul.cn/Article/details/gfzmmrkbj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.sjlbkw.cn/Article/details/gacibhfox.sHtML

Java: // 无解构
来源：http://wap.sjlbkw.cn/Article/details/gvvhrhnrp.sHtML

Go:   // 无解构
来源：http://wap.bbcook.cn/Article/details/glhodavrm.sHtML

Ruby: a, b = pair
来源：http://blog.tarul.cn/Article/details/gzfbldkmv.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.yfazqb.com/Article/details/gjojfzpon.sHtML

[C16] 函数 / 方法重载
来源：http://3g.tarul.cn/Article/details/getahfdlz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.bbcook.cn/Article/details/gntmpxkmq.sHtML

PHP:  // 无重载
来源：http://www.share.tarul.cn/Article/details/gnpmbwmuz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.sjlbkw.cn/Article/details/gvybrmpzg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.yfazqb.com/Article/details/gaiahwmvq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fktsv.cn/Article/details/gisewnpwq.sHtML


<!-- 参考信息 -->