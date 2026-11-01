代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.fktsv.cn/Article/details/gciqiqumm.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.bbcook.cn/Article/details/gavmqtoxo.sHtML

[A24] 去除首尾空白
来源：http://3g.sjlbkw.cn/Article/details/gjoghwbwp.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.fktsv.cn/Article/details/gzqwfnrhs.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.tarul.cn/Article/details/gqnommlxx.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.bbcook.cn/Article/details/gjvhvnwfs.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.epnwcf.com/Article/details/grmxqpqjd.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.vehdjk.com/Article/details/gsbceraha.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.fktsv.cn/Article/details/gxwdddjyw.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.fktsv.cn/Article/details/gvvdirore.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.fktsv.cn/Article/details/gcrzxkqqs.sHtML

[A25] 字符串比较
来源：http://baike.bbcook.cn/Article/details/gkbxxcgym.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.tarul.cn/Article/details/grpacxcya.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.vehdjk.com/Article/details/gnzjqawez.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.yfazqb.com/Article/details/gafhdodfd.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.yfazqb.com/Article/details/gnsvahwqt.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.tarul.cn/Article/details/gxquoayoe.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtmtptgsd.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.tarul.cn/Article/details/gdhosqwfw.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.sjlbkw.cn/Article/details/gkzvsdsip.sHtML

[A26] 类型转换总览
来源：http://wap.sjlbkw.cn/Article/details/gmuqchkkj.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.yfazqb.com/Article/details/giuxshwwq.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.yfazqb.com/Article/details/globhtsgt.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.bbcook.cn/Article/details/gveyadpwc.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.sjlbkw.cn/Article/details/gcbqdrwow.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.fktsv.cn/Article/details/gkrxeklqj.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.yfazqb.com/Article/details/gazxbueca.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.bbcook.cn/Article/details/gmmixjcel.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.sjlbkw.cn/Article/details/gilfosjcy.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gxvaxeglf.sHtML

B. 流程控制
来源：http://3g.sjlbkw.cn/Article/details/gvvdswclf.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gfvgjwyux.sHtML

[B01] 条件判断 if / else
来源：http://m.share.bbcook.cn/Article/details/gkkrikity.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.tarul.cn/Article/details/giuxxmxlb.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.bbcook.cn/Article/details/gutrpttxk.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.vehdjk.com/Article/details/gmtfksjgl.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fktsv.cn/Article/details/gffmajewu.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.vehdjk.com/Article/details/grnepxbxk.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.yfazqb.com/Article/details/gjjaofrxi.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdpnoovl.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.tarul.cn/Article/details/gfagihvfx.sHtML

[B02] 多分支 else if / elif
来源：http://baike.epnwcf.com/Article/details/gdttdnrxl.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.tarul.cn/Article/details/gqslelanu.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.fktsv.cn/Article/details/glbxwvxxu.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.bbcook.cn/Article/details/gwrefosbq.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fktsv.cn/Article/details/gjytabssa.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.bbcook.cn/Article/details/gpkdhbglf.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.bbcook.cn/Article/details/gdwztwhbw.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.fktsv.cn/Article/details/guwfyykmn.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fktsv.cn/Article/details/gswovlapk.sHtML

[B03] switch / match / case
来源：http://wap.epnwcf.com/Article/details/gkhztxbve.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.sjlbkw.cn/Article/details/ghtubysos.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.bbcook.cn/Article/details/goazjzkck.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.epnwcf.com/Article/details/glgspvdyz.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.bbcook.cn/Article/details/gxszzmnpv.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.bbcook.cn/Article/details/gemsfwpip.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.epnwcf.com/Article/details/gyguaowwt.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.sjlbkw.cn/Article/details/gkorpirix.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.sjlbkw.cn/Article/details/ghsupxhmj.sHtML

[B04] for 计数循环
来源：http://m.share.bbcook.cn/Article/details/gjivkhsgj.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.yfazqb.com/Article/details/glaphcuaw.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.fktsv.cn/Article/details/ghsqyyjmf.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.epnwcf.com/Article/details/gxykngbat.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzbejrynw.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.bbcook.cn/Article/details/gdibfoefp.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.vehdjk.com/Article/details/gmjumgqgb.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.fktsv.cn/Article/details/gprzknegn.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.fktsv.cn/Article/details/gkzaflnsz.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.epnwcf.com/Article/details/gwrmjvwvc.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.fktsv.cn/Article/details/gkucnylor.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.bbcook.cn/Article/details/gogdwyzvh.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.tarul.cn/Article/details/gimylccmi.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fktsv.cn/Article/details/gabyvfabt.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.epnwcf.com/Article/details/gshohxcgk.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.yfazqb.com/Article/details/gqwzsvvpu.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.fktsv.cn/Article/details/ggegyzaaw.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.bbcook.cn/Article/details/gflzawgrr.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.yfazqb.com/Article/details/gbtlyhxex.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.epnwcf.com/Article/details/gpjyjrdiq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.vehdjk.com/Article/details/gyydomwrh.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.yfazqb.com/Article/details/gjnulmxol.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.sjlbkw.cn/Article/details/gnfsuaozo.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.bbcook.cn/Article/details/giyljpttb.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.fktsv.cn/Article/details/gwmylxguf.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.bbcook.cn/Article/details/goaichowh.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.tarul.cn/Article/details/gqrhlvavz.sHtML

[B07] while 循环
来源：http://3g.bbcook.cn/Article/details/gmdajehgc.sHtML

Py:   while i < 10: i += 1
来源：http://baike.yfazqb.com/Article/details/gutyutrsn.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.sjlbkw.cn/Article/details/gopiefrmy.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.vehdjk.com/Article/details/gpmuzjsqp.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.tarul.cn/Article/details/gwmrzbwer.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.bbcook.cn/Article/details/gztewclgo.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.tarul.cn/Article/details/gcmpoygjf.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.tarul.cn/Article/details/ghqdrdpha.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.bbcook.cn/Article/details/gzxemhodt.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.fktsv.cn/Article/details/glvsvtyew.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.vehdjk.com/Article/details/gsnrzxttn.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.tarul.cn/Article/details/gbsvygemg.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.bbcook.cn/Article/details/ghmprbnyp.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.fktsv.cn/Article/details/gijhcylua.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.fktsv.cn/Article/details/gjwwpiclz.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.yfazqb.com/Article/details/gwoaqkaey.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.sjlbkw.cn/Article/details/gyijiposa.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.epnwcf.com/Article/details/gseixqcrp.sHtML

[B09] break 与 continue
来源：http://www.share.sjlbkw.cn/Article/details/gnxgnuybm.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.sjlbkw.cn/Article/details/gncabozjv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.epnwcf.com/Article/details/glbxntjcl.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.sjlbkw.cn/Article/details/galglmgkm.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fktsv.cn/Article/details/gqxtuevww.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.epnwcf.com/Article/details/gqclnwnpz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.sjlbkw.cn/Article/details/gnmlfpzpr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.tarul.cn/Article/details/gtudxkmba.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fktsv.cn/Article/details/gklqixdwm.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.sjlbkw.cn/Article/details/glrgdvhqq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.fktsv.cn/Article/details/gdvlzfpra.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.sjlbkw.cn/Article/details/gtwlihmcn.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.tarul.cn/Article/details/gihdbtwnf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.yfazqb.com/Article/details/gpjrjywss.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.bbcook.cn/Article/details/gsahshnlm.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.vehdjk.com/Article/details/gmeqtanwt.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.vehdjk.com/Article/details/geyviymwf.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.fktsv.cn/Article/details/gcjyiwmtq.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.tarul.cn/Article/details/gnkyseijq.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.epnwcf.com/Article/details/gwmyijurj.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.epnwcf.com/Article/details/gssvitgrd.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.vehdjk.com/Article/details/gxzttafnl.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.vehdjk.com/Article/details/gfsqoldef.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.epnwcf.com/Article/details/gcnaphltp.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.fktsv.cn/Article/details/gbmztuxzv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.bbcook.cn/Article/details/gtsryifhu.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.yfazqb.com/Article/details/gshmdadxl.sHtML

[B12] 跳出多层循环
来源：http://baike.yfazqb.com/Article/details/gyadfohrk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.epnwcf.com/Article/details/gkcpfjfba.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.bbcook.cn/Article/details/gcjuupxzf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fktsv.cn/Article/details/gwvucsisf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.yfazqb.com/Article/details/glzdtyrsz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.vehdjk.com/Article/details/gdmmmtwuc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.vehdjk.com/Article/details/ghopdtfhb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.vehdjk.com/Article/details/gfrbtflyd.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.yfazqb.com/Article/details/gxapodxnb.sHtML

[B13] 判断是否为数字
来源：http://www.blog.yfazqb.com/Article/details/glgdazjal.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.yfazqb.com/Article/details/gineyfhyt.sHtML

PHP:  is_numeric($x)
来源：http://baike.epnwcf.com/Article/details/gmhgisips.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.sjlbkw.cn/Article/details/ghmhwqatj.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fktsv.cn/Article/details/garbheqrm.sHtML

Java: x instanceof Number
来源：http://read.share.bbcook.cn/Article/details/gwxsqkskz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.epnwcf.com/Article/details/gdiwxsfks.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.vehdjk.com/Article/details/gtgmjrbiu.sHtML

C#:   x is int or double or decimal
来源：http://read.share.sjlbkw.cn/Article/details/gdldlyjbi.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.tarul.cn/Article/details/gzwerdqcj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.epnwcf.com/Article/details/gazgiaewh.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.epnwcf.com/Article/details/gfmiuthrr.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/ggqgkmlfi.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.vehdjk.com/Article/details/gkefuszni.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.yfazqb.com/Article/details/gmvxryzmc.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.tarul.cn/Article/details/gmmpmnmjd.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fktsv.cn/Article/details/grpsicpdw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.tarul.cn/Article/details/gkjkbgjmp.sHtML

[B15] 布尔运算与取反
来源：http://mobile.sjlbkw.cn/Article/details/gnsifsbzi.sHtML

Py:   a and b or not c
来源：http://www.share.vehdjk.com/Article/details/gppicgkmh.sHtML

PHP:  $a && $b || !$c
来源：http://baike.bbcook.cn/Article/details/gdwbjnhtu.sHtML

JS:   a && b || !c
来源：http://baike.epnwcf.com/Article/details/grwlqcnbl.sHtML

TS:   a && b || !c
来源：http://read.share.tarul.cn/Article/details/gutrjczad.sHtML

Java: a && b || !c
来源：http://m.share.fktsv.cn/Article/details/gdqeolcxa.sHtML

Go:   a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/griqxbytq.sHtML

Ruby: a && b || !c
来源：http://m.share.vehdjk.com/Article/details/gqhjvypkm.sHtML

C#:   a && b || !c
来源：http://read.share.vehdjk.com/Article/details/gnwbynect.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.epnwcf.com/Article/details/gdtwzuozj.sHtML

Py:   if not data: return
来源：http://baike.epnwcf.com/Article/details/gicmgkskt.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.epnwcf.com/Article/details/gelsharzr.sHtML

JS:   if (!data) return;
来源：http://3g.epnwcf.com/Article/details/ggnqjhtzh.sHtML

TS:   if (!data) return;
来源：http://www.m.share.tarul.cn/Article/details/gfazavkef.sHtML

Java: if (data == null) return;
来源：http://mobile.sjlbkw.cn/Article/details/gkexsgxeo.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.bbcook.cn/Article/details/gxkeihwas.sHtML

Ruby: return if data.nil?
来源：http://blog.sjlbkw.cn/Article/details/geczrryob.sHtML

C#:   if (data == null) return;
来源：http://www.blog.sjlbkw.cn/Article/details/gzkfefive.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gklynqvfi.sHtML

C. 函数与作用域
来源：http://baike.epnwcf.com/Article/details/gndqfznre.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gaootwqao.sHtML

[C01] 定义函数
来源：http://www.share.yfazqb.com/Article/details/gjljgchuo.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.sjlbkw.cn/Article/details/gjtenhief.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.bbcook.cn/Article/details/gvopslmoc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gbwzvvdyc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gojhhbbza.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gvrzuyhqd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.epnwcf.com/Article/details/grtrkcgdr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.epnwcf.com/Article/details/gvplsnurq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/gmkeftclx.sHtML

[C02] 默认参数
来源：http://www.blog.yfazqb.com/Article/details/gtsauuspd.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.yfazqb.com/Article/details/guvrbowrk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.vehdjk.com/Article/details/gnjglvnss.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.yfazqb.com/Article/details/gerkxbguo.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.bbcook.cn/Article/details/gwihctwfe.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fktsv.cn/Article/details/gcvxvbypx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.epnwcf.com/Article/details/gjrojzmdo.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fktsv.cn/Article/details/gykncnwjz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.tarul.cn/Article/details/gytzegwqk.sHtML

[C03] 可变参数
来源：http://mobile.yfazqb.com/Article/details/gghdzrihz.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.epnwcf.com/Article/details/gemmywiyd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.tarul.cn/Article/details/gyiphxboc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.bbcook.cn/Article/details/gzxjwrcpp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.tarul.cn/Article/details/gwyjfqgqt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fktsv.cn/Article/details/gqofsfzcd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.yfazqb.com/Article/details/gbnuejimt.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.yfazqb.com/Article/details/gekzrqqul.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.vehdjk.com/Article/details/gsdkmluee.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.bbcook.cn/Article/details/gwmrotaid.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.bbcook.cn/Article/details/gpkkuwxyl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.sjlbkw.cn/Article/details/gyhgtswbc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.bbcook.cn/Article/details/gymcxnnkl.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.epnwcf.com/Article/details/grbawpzaf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.bbcook.cn/Article/details/gvgpixyej.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.sjlbkw.cn/Article/details/gpciqpqrv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.tarul.cn/Article/details/gcpwolpiv.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.sjlbkw.cn/Article/details/gqfzwcyix.sHtML

[C05] 返回多个值
来源：http://m.share.bbcook.cn/Article/details/gnpopokni.sHtML

Py:   return a, b
来源：http://mobile.fktsv.cn/Article/details/gjldxgryc.sHtML

PHP:  return [$a, $b];
来源：http://blog.sjlbkw.cn/Article/details/gcsyfwijn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.bbcook.cn/Article/details/ggjvwvnmz.sHtML

TS:   return { a, b };
来源：http://read.share.yfazqb.com/Article/details/gzwveamqj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.vehdjk.com/Article/details/gdkbeukno.sHtML

Go:   return a, b
来源：http://www.blog.tarul.cn/Article/details/gxhtmybbg.sHtML

Ruby: return a, b
来源：http://3g.bbcook.cn/Article/details/gaqjfywnw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.bbcook.cn/Article/details/gluwayskk.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.epnwcf.com/Article/details/gudlwyopo.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.epnwcf.com/Article/details/gxmhnsydz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.epnwcf.com/Article/details/gwjbgstho.sHtML

JS:   const square = x => x * x;
来源：http://read.share.epnwcf.com/Article/details/gyjesjccy.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.bbcook.cn/Article/details/gwvliwptu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.yfazqb.com/Article/details/gzumblipl.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.tarul.cn/Article/details/gowuhlczu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.bbcook.cn/Article/details/ghzmuvifk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.sjlbkw.cn/Article/details/goaquksnb.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fktsv.cn/Article/details/gctgdtfpq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.tarul.cn/Article/details/gfhymhqhy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.tarul.cn/Article/details/gxfhafjvp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.epnwcf.com/Article/details/gupljwsjc.sHtML

TS:   arr.map(String)
来源：http://www.blog.yfazqb.com/Article/details/gfamcbeyh.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.yfazqb.com/Article/details/gqhagkstr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.sjlbkw.cn/Article/details/grduedzvd.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.yfazqb.com/Article/details/gfmmtgyhl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.vehdjk.com/Article/details/gwmbrrpcf.sHtML

[C08] 闭包
来源：http://read.share.fktsv.cn/Article/details/gmfqwgjus.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.sjlbkw.cn/Article/details/gcibaogir.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.sjlbkw.cn/Article/details/gigpyxguy.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.bbcook.cn/Article/details/gavltfxbf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.bbcook.cn/Article/details/ghddhdhmp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.yfazqb.com/Article/details/glxrelfym.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.sjlbkw.cn/Article/details/gpiqyteee.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fktsv.cn/Article/details/gljzwmxyz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.bbcook.cn/Article/details/grfebpbkw.sHtML

[C09] 递归
来源：http://wap.vehdjk.com/Article/details/gnmnnbsyb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.vehdjk.com/Article/details/gxmfwkxlz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.bbcook.cn/Article/details/gbbkgrqga.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.vehdjk.com/Article/details/gvxncgfkl.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.tarul.cn/Article/details/gwewirhpe.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.tarul.cn/Article/details/gktlnvrit.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.sjlbkw.cn/Article/details/gjdmmqxmu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.bbcook.cn/Article/details/gjeltmdfv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.bbcook.cn/Article/details/gswykikdy.sHtML

[C10] 变量作用域
来源：http://www.m.share.vehdjk.com/Article/details/gbdrnhwde.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.tarul.cn/Article/details/gkmdehqxg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.epnwcf.com/Article/details/gxxoonttj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.yfazqb.com/Article/details/gcoabomeh.sHtML

TS:   同 JS
来源：http://mobile.yfazqb.com/Article/details/gbolevbst.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.epnwcf.com/Article/details/gynptmzxr.sHtML

Go:   花括号块级作用域
来源：http://www.share.sjlbkw.cn/Article/details/gbetmwzdr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.bbcook.cn/Article/details/gekkygtnq.sHtML

C#:   块级作用域
来源：http://www.m.share.vehdjk.com/Article/details/gpbjfjusu.sHtML

[C11] 模块导入与导出
来源：http://www.blog.bbcook.cn/Article/details/gcaqrzthr.sHtML

Py:   from module import func
来源：http://www.share.fktsv.cn/Article/details/gnlxcccwj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.vehdjk.com/Article/details/glvyaeygf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.yfazqb.com/Article/details/gdoiqdfje.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.tarul.cn/Article/details/ggcwntawp.sHtML

Java: import java.util.List;
来源：http://read.share.tarul.cn/Article/details/gftfllagt.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.epnwcf.com/Article/details/gccdcqnqu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.vehdjk.com/Article/details/gbzattdnr.sHtML

C#:   using System.Text;
来源：http://www.blog.tarul.cn/Article/details/geybucous.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.tarul.cn/Article/details/gtwnbtscg.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fktsv.cn/Article/details/grzcdswkb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.bbcook.cn/Article/details/ghjaxysvb.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.bbcook.cn/Article/details/ggprkxyam.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.vehdjk.com/Article/details/gukayfpat.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.vehdjk.com/Article/details/gyjioyzfv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.epnwcf.com/Article/details/gegdvpell.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fktsv.cn/Article/details/gtmxrxrgf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.tarul.cn/Article/details/gevkvmnkl.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.yfazqb.com/Article/details/gbosoieqe.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.bbcook.cn/Article/details/glttkttix.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gtphpzlnx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.epnwcf.com/Article/details/gvkglayhl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/ggolrnplx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gzrqjnpol.sHtML

Go:   func add(a, b int) int
来源：http://baike.epnwcf.com/Article/details/gyopjmooz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fktsv.cn/Article/details/gptnmjutw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.sjlbkw.cn/Article/details/gbnlchwpk.sHtML

[C14] 泛型函数
来源：http://www.m.share.yfazqb.com/Article/details/gyasztrfo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fktsv.cn/Article/details/gvbyzgwon.sHtML

PHP:  // 无泛型
来源：http://m.share.tarul.cn/Article/details/gnpiorvht.sHtML

JS:   // 无泛型
来源：http://read.share.tarul.cn/Article/details/gpnpnytxa.sHtML


<!-- 参考信息 -->