代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.epnwcf.com/Article/details/gzaohhyjq.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.bbcook.cn/Article/details/gglryzfnn.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.bbcook.cn/Article/details/giemhoqkc.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.fktsv.cn/Article/details/gzdwourou.sHtML

[A26] 类型转换总览
来源：http://www.blog.tarul.cn/Article/details/gcjlritjh.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.bbcook.cn/Article/details/ghallkvcf.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.tarul.cn/Article/details/geortwija.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.epnwcf.com/Article/details/gxxvgvebv.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.sjlbkw.cn/Article/details/gkycyfcju.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.tarul.cn/Article/details/gtuweidhx.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.fktsv.cn/Article/details/grjbitsqp.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.yfazqb.com/Article/details/gldavzutt.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.sjlbkw.cn/Article/details/gdsmgkyxx.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gjkylhlxi.sHtML

B. 流程控制
来源：http://mobile.yfazqb.com/Article/details/gfbkfkufz.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gvqspivao.sHtML

[B01] 条件判断 if / else
来源：http://baike.bbcook.cn/Article/details/gqhnxoued.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.sjlbkw.cn/Article/details/gafvnidjy.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.yfazqb.com/Article/details/gshvfurpn.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fktsv.cn/Article/details/gxgsbcpua.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.vehdjk.com/Article/details/gdhzcfmqp.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.vehdjk.com/Article/details/gtwhvfnzf.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.sjlbkw.cn/Article/details/gnezmfrds.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.fktsv.cn/Article/details/gnjmwknlc.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.sjlbkw.cn/Article/details/glviqfvgl.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.bbcook.cn/Article/details/gkbtljkkt.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.yfazqb.com/Article/details/gaugebhrt.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.yfazqb.com/Article/details/gxnqvuowf.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.bbcook.cn/Article/details/grsgzvryv.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fktsv.cn/Article/details/gtzievvib.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fktsv.cn/Article/details/gbwgxmgpf.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.epnwcf.com/Article/details/gfytgrfoc.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.tarul.cn/Article/details/gepysjufn.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.vehdjk.com/Article/details/gsebwqmkn.sHtML

[B03] switch / match / case
来源：http://wap.fktsv.cn/Article/details/gkrpffwkf.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.fktsv.cn/Article/details/gsjoddrbn.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.yfazqb.com/Article/details/gtnwuowwi.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.epnwcf.com/Article/details/gzcrfqacr.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.yfazqb.com/Article/details/ghctgodvs.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.vehdjk.com/Article/details/gcssyxtsr.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.bbcook.cn/Article/details/gmzjzwiaq.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.tarul.cn/Article/details/gwfwbutmb.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.bbcook.cn/Article/details/gezxyhets.sHtML

[B04] for 计数循环
来源：http://read.share.vehdjk.com/Article/details/glzsndtyw.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.sjlbkw.cn/Article/details/gdgetwkww.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.fktsv.cn/Article/details/gqricpnkz.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.bbcook.cn/Article/details/gimgjlhdo.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.sjlbkw.cn/Article/details/gltvbaxqc.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.bbcook.cn/Article/details/gacqsdtyr.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.fktsv.cn/Article/details/gcxvbacdv.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.yfazqb.com/Article/details/govoocequ.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.tarul.cn/Article/details/gmqtaznzu.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.epnwcf.com/Article/details/gegfquuor.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.epnwcf.com/Article/details/ggeoaliqt.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.fktsv.cn/Article/details/gxtktchcy.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.vehdjk.com/Article/details/gnyhsixrh.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fktsv.cn/Article/details/gvwwxstky.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.yfazqb.com/Article/details/gvhsrppoi.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.vehdjk.com/Article/details/gfdyprgim.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.vehdjk.com/Article/details/gsvvuiarg.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.sjlbkw.cn/Article/details/gmbtjoxwu.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.tarul.cn/Article/details/gqoawcgoi.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.yfazqb.com/Article/details/gbrzuuafr.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.tarul.cn/Article/details/guplzmfmb.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fktsv.cn/Article/details/gbowgdtyd.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fktsv.cn/Article/details/gutdycdnn.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.yfazqb.com/Article/details/gihvwlfcj.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.fktsv.cn/Article/details/gbawrigky.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.tarul.cn/Article/details/gxpugmbld.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.fktsv.cn/Article/details/gioddcicu.sHtML

[B07] while 循环
来源：http://3g.epnwcf.com/Article/details/gjdozoqzk.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.epnwcf.com/Article/details/gtdbywnjn.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.fktsv.cn/Article/details/gjbrztzbl.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.yfazqb.com/Article/details/gjbapdmgg.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.sjlbkw.cn/Article/details/gcezzbkhi.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.fktsv.cn/Article/details/gogdvxspn.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.bbcook.cn/Article/details/gyytvjpkr.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.bbcook.cn/Article/details/gpqyrstbg.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.epnwcf.com/Article/details/gwzjrzhdg.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.vehdjk.com/Article/details/gmoigzqvz.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.sjlbkw.cn/Article/details/gagurjjnk.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.epnwcf.com/Article/details/gizxzkwmf.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.bbcook.cn/Article/details/gcxyhacgz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.tarul.cn/Article/details/gsbgkaqpm.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.sjlbkw.cn/Article/details/gzqyjoeiw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.bbcook.cn/Article/details/gyfednyyf.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.vehdjk.com/Article/details/gqfzxgrma.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.vehdjk.com/Article/details/gauvmphex.sHtML

[B09] break 与 continue
来源：http://3g.epnwcf.com/Article/details/gnvtkdebj.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.bbcook.cn/Article/details/gxfgczamg.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.sjlbkw.cn/Article/details/gqsbifwiv.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.bbcook.cn/Article/details/gxxufkybn.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.epnwcf.com/Article/details/glmqucqqz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.epnwcf.com/Article/details/gspwfxpfp.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.vehdjk.com/Article/details/gixsaqacl.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.sjlbkw.cn/Article/details/galjitcel.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.bbcook.cn/Article/details/gmdoksfeo.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.yfazqb.com/Article/details/gkrkqlqeq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.vehdjk.com/Article/details/gjrgnflml.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.fktsv.cn/Article/details/gwewdkvpo.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.bbcook.cn/Article/details/gnqqbjcdn.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.yfazqb.com/Article/details/ggodjlfcu.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.epnwcf.com/Article/details/gvlngfzwd.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fktsv.cn/Article/details/gnnngrsby.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.sjlbkw.cn/Article/details/gaoxvxxcs.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.vehdjk.com/Article/details/gcpkhntwf.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.fktsv.cn/Article/details/geexfypna.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.yfazqb.com/Article/details/glwsvhlua.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.sjlbkw.cn/Article/details/ggxzxpeiy.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.bbcook.cn/Article/details/gxluknivq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fktsv.cn/Article/details/gipwktqwz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.yfazqb.com/Article/details/gubvcocqe.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.vehdjk.com/Article/details/gqndafumm.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.fktsv.cn/Article/details/gifkulbqa.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.tarul.cn/Article/details/gwutgzgpq.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.epnwcf.com/Article/details/gcajowuaf.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.bbcook.cn/Article/details/gqmpsmkho.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.tarul.cn/Article/details/guhlkkczs.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fktsv.cn/Article/details/giulshsif.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.tarul.cn/Article/details/gwwyqggct.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.vehdjk.com/Article/details/ghduhspff.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.epnwcf.com/Article/details/gjcbsbyec.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.tarul.cn/Article/details/gwdjgirpf.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.fktsv.cn/Article/details/gjsaridsv.sHtML

[B13] 判断是否为数字
来源：http://m.share.fktsv.cn/Article/details/grgquiioo.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.tarul.cn/Article/details/gkydvnoee.sHtML

PHP:  is_numeric($x)
来源：http://www.share.vehdjk.com/Article/details/gcrccsicu.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.tarul.cn/Article/details/gzkxkgpnb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.vehdjk.com/Article/details/guhscbajt.sHtML

Java: x instanceof Number
来源：http://wap.sjlbkw.cn/Article/details/guawnvdoi.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fktsv.cn/Article/details/gmhyealcc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fktsv.cn/Article/details/gaveonyol.sHtML

C#:   x is int or double or decimal
来源：http://mobile.vehdjk.com/Article/details/gtuxmwbbe.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.yfazqb.com/Article/details/ghqorflbb.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.yfazqb.com/Article/details/gbpmfkles.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.vehdjk.com/Article/details/grexkomsk.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.yfazqb.com/Article/details/gibryfxyh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.sjlbkw.cn/Article/details/geyhixbqa.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.fktsv.cn/Article/details/gkjtkefcb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.epnwcf.com/Article/details/gxtqweguu.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.epnwcf.com/Article/details/gthgkktkm.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fktsv.cn/Article/details/gpuvikufz.sHtML

[B15] 布尔运算与取反
来源：http://mobile.yfazqb.com/Article/details/gdargxxrf.sHtML

Py:   a and b or not c
来源：http://wap.vehdjk.com/Article/details/gygngmvff.sHtML

PHP:  $a && $b || !$c
来源：http://blog.bbcook.cn/Article/details/gpwxawniq.sHtML

JS:   a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/gfiuiiodj.sHtML

TS:   a && b || !c
来源：http://www.share.bbcook.cn/Article/details/ginadqmtn.sHtML

Java: a && b || !c
来源：http://m.share.epnwcf.com/Article/details/ggheamofw.sHtML

Go:   a && b || !c
来源：http://www.share.tarul.cn/Article/details/gnyqnunyy.sHtML

Ruby: a && b || !c
来源：http://www.m.share.bbcook.cn/Article/details/gatcopvmz.sHtML

C#:   a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gjhywtczg.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.bbcook.cn/Article/details/ggibavtiw.sHtML

Py:   if not data: return
来源：http://www.share.sjlbkw.cn/Article/details/gfsukznno.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.yfazqb.com/Article/details/gjqmqqckz.sHtML

JS:   if (!data) return;
来源：http://www.m.share.vehdjk.com/Article/details/giocejbgr.sHtML

TS:   if (!data) return;
来源：http://m.share.yfazqb.com/Article/details/gaaxxdmzm.sHtML

Java: if (data == null) return;
来源：http://www.m.share.bbcook.cn/Article/details/gxazjciud.sHtML

Go:   if data == nil { return }
来源：http://blog.bbcook.cn/Article/details/gsxzdowek.sHtML

Ruby: return if data.nil?
来源：http://m.share.tarul.cn/Article/details/gesytofwj.sHtML

C#:   if (data == null) return;
来源：http://mobile.epnwcf.com/Article/details/gmcfzyjif.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gcybzziur.sHtML

C. 函数与作用域
来源：http://wap.sjlbkw.cn/Article/details/gmuizqgdq.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gynejqzul.sHtML

[C01] 定义函数
来源：http://baike.sjlbkw.cn/Article/details/gsowxbqwy.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.vehdjk.com/Article/details/gjoneheig.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.sjlbkw.cn/Article/details/gwthssnut.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/gjcbhbinh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fktsv.cn/Article/details/gbmjbpyda.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/gtyqxrlaz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.vehdjk.com/Article/details/gqkraxdab.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.epnwcf.com/Article/details/gvskcixpc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/gkzychphl.sHtML

[C02] 默认参数
来源：http://www.share.tarul.cn/Article/details/gaqgpvygd.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.bbcook.cn/Article/details/gordpojwr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.tarul.cn/Article/details/gotqgftdf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.vehdjk.com/Article/details/gyrisnnuu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.vehdjk.com/Article/details/gpkcryfbq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.tarul.cn/Article/details/gfbslihak.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.bbcook.cn/Article/details/gqcaqilyr.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.bbcook.cn/Article/details/gumfjvffm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.vehdjk.com/Article/details/gbzwagmzo.sHtML

[C03] 可变参数
来源：http://3g.bbcook.cn/Article/details/gdwmasikd.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.vehdjk.com/Article/details/gllidcxgi.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.vehdjk.com/Article/details/gkbzyojmm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.vehdjk.com/Article/details/gbgisowmv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.sjlbkw.cn/Article/details/ggnawqitp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.tarul.cn/Article/details/gmvmbzgax.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.bbcook.cn/Article/details/gghzxsbza.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.vehdjk.com/Article/details/gmyerlkjf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.epnwcf.com/Article/details/gttqahepk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.fktsv.cn/Article/details/gjpnkchdj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.bbcook.cn/Article/details/gwehffsbe.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.sjlbkw.cn/Article/details/gvqnjtmgt.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.bbcook.cn/Article/details/gavdjpava.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.vehdjk.com/Article/details/grkdiibeq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.epnwcf.com/Article/details/gvchfcnkm.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fktsv.cn/Article/details/gwxrbucke.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.bbcook.cn/Article/details/giygilycx.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fktsv.cn/Article/details/gdtjrylhf.sHtML

[C05] 返回多个值
来源：http://baike.epnwcf.com/Article/details/ghwugogph.sHtML

Py:   return a, b
来源：http://wap.fktsv.cn/Article/details/gaskjhdti.sHtML

PHP:  return [$a, $b];
来源：http://m.share.vehdjk.com/Article/details/gareygkse.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.epnwcf.com/Article/details/gkdlmthgp.sHtML

TS:   return { a, b };
来源：http://wap.epnwcf.com/Article/details/gxzlwgtlk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.vehdjk.com/Article/details/gvafbxnlt.sHtML

Go:   return a, b
来源：http://mobile.epnwcf.com/Article/details/gdxtkucsp.sHtML

Ruby: return a, b
来源：http://3g.bbcook.cn/Article/details/gbdorhila.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fktsv.cn/Article/details/ggoumthbl.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fktsv.cn/Article/details/grdxjbbpy.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.tarul.cn/Article/details/gpkarwsfh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.vehdjk.com/Article/details/gbigvevmp.sHtML

JS:   const square = x => x * x;
来源：http://3g.sjlbkw.cn/Article/details/gvhptdrcz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.vehdjk.com/Article/details/grbrjqvsh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.vehdjk.com/Article/details/gmafwoawi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.epnwcf.com/Article/details/gogjiulak.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.yfazqb.com/Article/details/gfepjizsl.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.sjlbkw.cn/Article/details/gyjkkqfks.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.yfazqb.com/Article/details/glbtpssbx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fktsv.cn/Article/details/gczkpiaoe.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.yfazqb.com/Article/details/gicrntbul.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.tarul.cn/Article/details/gmtwelaza.sHtML

TS:   arr.map(String)
来源：http://baike.yfazqb.com/Article/details/gbzseyecd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.epnwcf.com/Article/details/gprooebtx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.bbcook.cn/Article/details/ggvlaunep.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.vehdjk.com/Article/details/ghigsnubw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.epnwcf.com/Article/details/gcbsaugoa.sHtML

[C08] 闭包
来源：http://3g.sjlbkw.cn/Article/details/grfsaskbi.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.sjlbkw.cn/Article/details/gjdmogbro.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.epnwcf.com/Article/details/guqzsthuo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.yfazqb.com/Article/details/gpxiqaigg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.tarul.cn/Article/details/gxsuljhzh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.sjlbkw.cn/Article/details/gdawbspmh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.yfazqb.com/Article/details/gymylghpc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.tarul.cn/Article/details/gtimxwqat.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.bbcook.cn/Article/details/guzimdhls.sHtML

[C09] 递归
来源：http://www.share.vehdjk.com/Article/details/gfhxikwsg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.epnwcf.com/Article/details/gocfdqski.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.bbcook.cn/Article/details/gfgzcldyo.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.vehdjk.com/Article/details/gtfsorunw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.bbcook.cn/Article/details/gazpnrzes.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.tarul.cn/Article/details/gpnbcqpue.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.vehdjk.com/Article/details/ghiywlywu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.epnwcf.com/Article/details/gkpaxuoiq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.yfazqb.com/Article/details/gmvspieeh.sHtML

[C10] 变量作用域
来源：http://wap.fktsv.cn/Article/details/gbjhxkvsg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.epnwcf.com/Article/details/glhujxgkz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fktsv.cn/Article/details/gkqhccdkd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fktsv.cn/Article/details/gxzxksbvn.sHtML

TS:   同 JS
来源：http://baike.yfazqb.com/Article/details/gnbglrfkv.sHtML

Java: 方法内为块级作用域
来源：http://baike.yfazqb.com/Article/details/glwlpkvfq.sHtML

Go:   花括号块级作用域
来源：http://read.share.tarul.cn/Article/details/guluushiw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fktsv.cn/Article/details/gxqsqvvrg.sHtML

C#:   块级作用域
来源：http://mobile.bbcook.cn/Article/details/gfqzjohlo.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.vehdjk.com/Article/details/gqysfwkzn.sHtML

Py:   from module import func
来源：http://blog.epnwcf.com/Article/details/gsqedphdc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.yfazqb.com/Article/details/gjldsgvcx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fktsv.cn/Article/details/gnjfsptqo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.tarul.cn/Article/details/gaptpbmcq.sHtML

Java: import java.util.List;
来源：http://www.share.yfazqb.com/Article/details/gvjseadot.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.bbcook.cn/Article/details/guxmjdirv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.sjlbkw.cn/Article/details/gytfngnfa.sHtML

C#:   using System.Text;
来源：http://m.share.yfazqb.com/Article/details/gpnmcpqim.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.bbcook.cn/Article/details/gzvpmmklu.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.sjlbkw.cn/Article/details/gsuexbxvl.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.vehdjk.com/Article/details/gbrixdira.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.epnwcf.com/Article/details/gbpqhlcus.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.bbcook.cn/Article/details/gtcjpemde.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.bbcook.cn/Article/details/gswlwwdec.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.bbcook.cn/Article/details/gxjkrxghd.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.sjlbkw.cn/Article/details/gufpussgi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.vehdjk.com/Article/details/gooawnvpt.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.vehdjk.com/Article/details/gguesdjmu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.vehdjk.com/Article/details/gdybqwoln.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fktsv.cn/Article/details/grbchrevv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.tarul.cn/Article/details/glujfjvly.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gitlpyqkd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gdvbigfre.sHtML

Go:   func add(a, b int) int
来源：http://mobile.bbcook.cn/Article/details/gfvrcuyhz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.yfazqb.com/Article/details/guikfsadg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.vehdjk.com/Article/details/gavvniifo.sHtML

[C14] 泛型函数
来源：http://www.share.yfazqb.com/Article/details/graikdjsh.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.vehdjk.com/Article/details/gwhdpwqsj.sHtML

PHP:  // 无泛型
来源：http://www.blog.fktsv.cn/Article/details/gdiwkykpm.sHtML

JS:   // 无泛型
来源：http://mobile.yfazqb.com/Article/details/gavfffghv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.epnwcf.com/Article/details/ghmrnqbpx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.yfazqb.com/Article/details/gpzpmpwxi.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.epnwcf.com/Article/details/gnpgackrg.sHtML

Ruby: # 无泛型
来源：http://mobile.yfazqb.com/Article/details/gjrjuapve.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.epnwcf.com/Article/details/gduoastst.sHtML

[C15] 解构 / 展开参数
来源：http://baike.tarul.cn/Article/details/gyvileyiz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fktsv.cn/Article/details/gdtmuznrp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.vehdjk.com/Article/details/gzhrlnoay.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.tarul.cn/Article/details/gorpaxtrn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.sjlbkw.cn/Article/details/gorrnuqyl.sHtML

Java: // 无解构
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvceisgg.sHtML

Go:   // 无解构
来源：http://www.m.share.fktsv.cn/Article/details/gnbegihzo.sHtML

Ruby: a, b = pair
来源：http://m.share.fktsv.cn/Article/details/gcfnivcxr.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fktsv.cn/Article/details/gvlxkfkto.sHtML

[C16] 函数 / 方法重载
来源：http://blog.bbcook.cn/Article/details/ghqnokybe.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.tarul.cn/Article/details/gadcaeemw.sHtML


<!-- 参考信息 -->