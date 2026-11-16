代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://doe.xylfe.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://oia.jinyuanbaomall.cn

[A24] 去除首尾空白
来源：http://uno.sysykeji.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rup.jinghuilouyu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://iiq.zhengqikj.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wnl.sufxvd.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vdc.zhiwuduotai.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hli.bjfxy.top

Go:   strings.TrimSpace(s)
来源：http://ncj.pycfn.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nyw.daria6918.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ncx.hammf.cn

[A25] 字符串比较
来源：http://ttp.yonumen.top

Py:   s1 == s2; s1 != s2
来源：http://hcd.tanke756.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hll.birdmap.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fjk.yongpay.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://izi.zhengqikj.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qxz.nanxinkj.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://trq.zhongyouzk.top

Ruby: s1 == s2; s1 <=> s2
来源：http://mai.uphjek.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ijk.316326.xyz

[A26] 类型转换总览
来源：http://jdc.jinqigufen.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hdg.yueranfly.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vtj.tarul.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mey.jqgufenzy.top

TS:   Number() String() Boolean() x as number
来源：http://udl.vehdjk.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://uei.ybcxt.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ops.zdbjq.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://gos.jqgufenzy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uhy.redwolf501.top

================================================================================
来源：http://frw.hcnkem.com

B. 流程控制
来源：http://ood.ybcxt.top

================================================================================
来源：http://rjp.feifeiyinyue.top

[B01] 条件判断 if / else
来源：http://fbg.hongshengwenyu.top

Py:   result = "正" if x > 0 else "非正"
来源：http://bab.cheryme.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gtk.sxryk.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qes.shuidangran.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ggo.hywenlv.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://igq.feifeiyinyue.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wna.ydjk.org.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ofb.cashguo.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bdg.xingfuxueyuan.xyz

[B02] 多分支 else if / elif
来源：http://agz.gaohongyu789.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tqv.nanxinkj.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cna.hysaishi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gzb.xingfuxueyuan.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://klg.zhiwuduotai.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pah.jinghuilouyu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ztd.ywan-chungtsiang.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://brz.zdbjq.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zpg.guannengcc.top

[B03] switch / match / case
来源：http://vpx.gogol.net.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wju.yuxming.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qvg.jqgfzy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hxj.ctjpmb.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jsr.ybcxt.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jeu.yueranfly.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lpa.52xcode.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vfg.yj202588.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://erb.hesvh.cn

[B04] for 计数循环
来源：http://sfk.aizwys.cn

Py:   for i in range(10): print(i)
来源：http://cpa.nwbrower.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hjs.xingfuxueyuan.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sdw.hywenlv.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qwv.zdbjq.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tto.fanxiaobao.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xev.tianlin.xyz

Ruby: 10.times { |i| puts i }
来源：http://bgq.xinyue.icu

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fpi.xingfuxueyuan.xyz

[B05] 遍历数组 / 列表
来源：http://muv.gzhubu.top

Py:   for item in arr: print(item)
来源：http://foj.haohaochexian.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cax.jiagoushi.top

JS:   for (const item of arr) { console.log(item); }
来源：http://pss.chenlongwang.top

TS:   for (const item of arr) { console.log(item); }
来源：http://odt.jqgfzy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://erq.nwbrower.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nkw.zhongyouzk.top

Ruby: arr.each { |item| puts item }
来源：http://ipv.c1oappe.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zym.cqqwz.cn

[B06] 遍历字典 / 对象
来源：http://iah.svipenyu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qfi.zhengqikj.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://oin.vehdjk.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ifh.zycfv.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qdq.pycfn.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fkg.zhengqikj.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fmp.mhx1999.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vhe.yanxiufei.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://aqk.0kj1m.cn

[B07] while 循环
来源：http://ezk.zycfv.cn

Py:   while i < 10: i += 1
来源：http://iiq.gzhubu.top

PHP:  while ($i < 10) { $i++; }
来源：http://ivb.yangfankeji.com

JS:   while (i < 10) { i++; }
来源：http://mzk.52xcode.cn

TS:   while (i < 10) { i++; }
来源：http://snq.zhaomingkeji.xyz

Java: while (i < 10) { i++; }
来源：http://mlx.fengsongda.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hgl.hnqzz.top

Ruby: while i < 10; i += 1; end
来源：http://qkh.fehbvm.com

C#:   while (i < 10) { i++; }
来源：http://qps.vqdsnc.cn

[B08] do-while（至少执行一次）
来源：http://imz.fengsongda.top

Py:   # 无 do-while：用 while True + break
来源：http://azz.sufxvd.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://wog.yuxming.cn

JS:   do { i++; } while (i < 10);
来源：http://mls.ppjwa.cn

TS:   do { i++; } while (i < 10);
来源：http://obk.iojbl.cn

Java: do { i++; } while (i < 10);
来源：http://vbt.jyoumei.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xxc.xuanzx.com

Ruby: begin; i += 1; end while i < 10
来源：http://szo.fktsv.cn

C#:   do { i++; } while (i < 10);
来源：http://omg.yuxming.cn

[B09] break 与 continue
来源：http://nyp.gaohongyu789.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fgc.daria6918.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kzf.yuxming.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jdv.fzhhl.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uhg.wangdashe.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vee.gogol.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nba.yueranfly.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vug.tian-w.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ocn.guowangkeji.top

[B10] 遍历同时拿索引
来源：http://ltf.smart0.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hjx.ywan-chungtsiang.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nxl.hesvh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hil.zhengqikj.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://elv.hcnkem.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ufj.hesvh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ytj.hammf.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://itj.yuxming.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hut.nwbrower.top

[B11] 生成数字序列 / 区间
来源：http://jve.vqdsnc.cn

Py:   list(range(0, 10, 2))
来源：http://ocr.tanke756.top

PHP:  range(0, 10, 2);
来源：http://xke.nwbrower.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://owl.kuanghao11.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mri.jinyuanbaomall.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ebz.dashuyun.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vqg.chenjidiqi.icu

Ruby: (0...10).step(2).to_a
来源：http://nqo.sufxvd.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pih.fengsongda.top

[B12] 跳出多层循环
来源：http://eze.gaohongyu789.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ufp.xuanzx.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://wih.ctjpmb.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://slr.fehbvm.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ygm.9152youxi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://elg.dashuyun.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jzj.zdqjudy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pey.uphjek.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dln.jinqigufen.top

[B13] 判断是否为数字
来源：http://mmb.hnqzz.top

Py:   isinstance(x, (int, float))
来源：http://fqg.nwbrower.top

PHP:  is_numeric($x)
来源：http://axa.xuanzx.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qrz.tarul.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lzz.fengsongda.top

Java: x instanceof Number
来源：http://szi.birdmap.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xuj.cheryme.top

Ruby: x.is_a?(Numeric)
来源：http://uyz.cheryme.top

C#:   x is int or double or decimal
来源：http://oyf.meibo888.top

[B14] 判断值是否在集合内
来源：http://nwa.cucudq.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ywk.shuidangran.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://edf.aibaodan.cn

JS:   [1, 2, 3].includes(x)
来源：http://lla.ydzc1.top

TS:   [1, 2, 3].includes(x)
来源：http://yxe.sysykeji.top

Java: List.of(1, 2, 3).contains(x)
来源：http://mip.ywan-chungtsiang.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fep.redwolf501.top

Ruby: [1, 2, 3].include?(x)
来源：http://ryb.jqgufenzy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tzx.snrcjt.cn

[B15] 布尔运算与取反
来源：http://luj.hysaishi.cn

Py:   a and b or not c
来源：http://yhv.shanyushiyangtech.top

PHP:  $a && $b || !$c
来源：http://hkp.bbcook.cn

JS:   a && b || !c
来源：http://fvn.yuxming.cn

TS:   a && b || !c
来源：http://riv.zdqjudy.top

Java: a && b || !c
来源：http://xge.xziqi.cn

Go:   a && b || !c
来源：http://wie.tanke756.top

Ruby: a && b || !c
来源：http://hlu.shzxlz.cn

C#:   a && b || !c
来源：http://tdz.cdnleiting.top

[B16] 卫语句：不满足条件提前返回
来源：http://dgp.bbcook.cn

Py:   if not data: return
来源：http://hsl.shangyingyoupin.top

PHP:  if (!$data) { return; }
来源：http://bwf.smart0.xyz

JS:   if (!data) return;
来源：http://bdx.fzhhl.top

TS:   if (!data) return;
来源：http://kfg.gaohongyu789.top

Java: if (data == null) return;
来源：http://klw.ybcxt.top

Go:   if data == nil { return }
来源：http://mwc.ywan-chungtsiang.top

Ruby: return if data.nil?
来源：http://uit.hnqzz.top

C#:   if (data == null) return;
来源：http://btx.jqgfzy.top

================================================================================
来源：http://sie.tanke756.top

C. 函数与作用域
来源：http://bqa.fzhhl.top

================================================================================
来源：http://fiv.yueranfly.top

[C01] 定义函数
来源：http://zft.tianlin.xyz

Py:   def add(a, b): return a + b
来源：http://ycq.snrcjt.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pmk.aibaodan.cn

JS:   function add(a, b) { return a + b; }
来源：http://qqd.fengsongda.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wjj.jqgufenzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://qxo.gotoacloud.top

Go:   func add(a, b int) int { return a + b }
来源：http://vpr.sxryk.cn

Ruby: def add(a, b); a + b; end
来源：http://akf.sweek.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://loo.ivvv.top

[C02] 默认参数
来源：http://shv.nanxuanxn.top

Py:   def greet(name="World"): return name
来源：http://ggh.ctjpmb.com

PHP:  function greet($name = "World") { return $name; }
来源：http://xnu.zdbjq.cn

JS:   function greet(name = "World") { return name; }
来源：http://zbn.tianlin.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://oqh.pycfn.com

Java: // 无默认参数：方法重载或 Optional
来源：http://duu.feifeiyinyue.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ero.fktsv.cn

Ruby: def greet(name = "World") = name
来源：http://xpb.xinyue.icu

C#:   string Greet(string name = "World") => name;
来源：http://hqa.ywan-chungtsiang.top

[C03] 可变参数
来源：http://vuc.guannengcc.top

Py:   def total(*args): return sum(args)
来源：http://nrt.dashuyun.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ftx.ctjpmb.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ogn.shuidangran.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://val.gzhubu.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ebx.jqgufenzy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kmg.sweek.top

Ruby: def total(*nums); nums.sum; end
来源：http://yad.redwolf501.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://flr.guannengcc.top

[C04] 命名参数 / 关键字参数
来源：http://wvt.feifeiyinyue.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wfj.iojbl.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://atb.haohaochexian.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lgm.xuetiantiany.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jra.xinyue.icu

Java: // 无：用 Builder 模式或 record
来源：http://qwd.jiagoushi.top

Go:   // 无：用配置结构体参数
来源：http://jeo.ehwqpu.com

Ruby: f(a: 1, b: 2)
来源：http://kvv.kuanghao11.cn

C#:   f(a: 1, b: 2)
来源：http://rot.smart0.xyz

[C05] 返回多个值
来源：http://tzb.haohaochexian.top

Py:   return a, b
来源：http://eru.0kj1m.cn

PHP:  return [$a, $b];
来源：http://bfp.mhx1999.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://avs.jinghuilouyu.cn

TS:   return { a, b };
来源：http://ynd.havefunace.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xnt.guannengcc.top

Go:   return a, b
来源：http://uri.shangyingyoupin.top

Ruby: return a, b
来源：http://yje.quarkkingdee.top

C#:   return (a, b);              // ValueTuple
来源：http://zix.pengpengdd.cyou

[C06] 匿名函数 / lambda
来源：http://aow.hfpthk.cn

Py:   square = lambda x: x * x
来源：http://vat.wangdashe.top

PHP:  $square = fn($x) => $x * $x;
来源：http://lkl.jlsjyb.cn

JS:   const square = x => x * x;
来源：http://bev.yj20258.top

TS:   const square = (x: number): number => x * x;
来源：http://oig.yfazqb.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mnm.chenlongwang.top

Go:   sq := func(x int) int { return x * x }
来源：http://zpl.c1oappe.top

Ruby: square = ->(x) { x * x }
来源：http://bkc.gotoacloud.top

C#:   Func<int, int> square = x => x * x;
来源：http://mtg.sufxvd.cn

[C07] 把函数作为参数传入
来源：http://pqa.cucudq.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rid.cashguo.top

PHP:  array_map("strtoupper", $arr);
来源：http://uom.snrcjt.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uvh.yvedp.cn

TS:   arr.map(String)
来源：http://tuy.jinqigufen.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://opy.wangdashe.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tvt.haohaochexian.top

Ruby: arr.map(&:upcase)
来源：http://jtk.chenjidiqi.icu

C#:   arr.Select(s => s.ToUpper())
来源：http://yix.tanke756.top

[C08] 闭包
来源：http://nth.ppjwa.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ypp.zhijiandao.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lnv.shangyingyoupin.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://svf.zhiwuduotai.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bha.wangdashe.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jfc.yangfankeji.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pcy.chenjidiqi.icu

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://clt.cashguo.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jwl.shanyushiyangtech.top

[C09] 递归
来源：http://esy.0kj1m.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://phc.ywan-chungtsiang.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mtj.xingfuxueyuan.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://owq.hcnkem.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aoe.sjlbkw.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cuk.svipenyu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://faq.hcnkem.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uzk.zhiwuduotai.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ltz.xuanzx.com

[C10] 变量作用域
来源：http://sck.hfpthk.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kkn.cqqwz.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://skd.wangshuangyany.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jdm.daxiang520.top

TS:   同 JS
来源：http://ybj.yj20258.top

Java: 方法内为块级作用域
来源：http://gsb.sxryk.cn

Go:   花括号块级作用域
来源：http://wel.hammf.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vzl.iojbl.cn

C#:   块级作用域
来源：http://yfq.hywenlv.cn

[C11] 模块导入与导出
来源：http://hhz.iojbl.cn

Py:   from module import func
来源：http://dcy.zdbjq.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://win.feifeiyinyue.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://utc.zhijiandao.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ddp.xziqi.cn

Java: import java.util.List;
来源：http://kha.tian-w.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rpo.hfpthk.cn

Ruby: require "json"; require_relative "./util"
来源：http://trr.zdbjq.cn

C#:   using System.Text;
来源：http://dac.fzhhl.top

[C12] 立即执行函数 IIFE
来源：http://hgj.yuxming.cn

Py:   (lambda: print("run"))()
来源：http://hig.zdbjq.cn

PHP:  (function () { echo "run"; })();
来源：http://zrw.yueranfly.top

JS:   (() => { console.log("run"); })();
来源：http://dsx.jqgufenzy.top

TS:   (() => { console.log("run"); })();
来源：http://lpn.ehwqpu.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vdc.smart0.xyz

Go:   func() { fmt.Println("run") }()
来源：http://ioa.hammf.cn

Ruby: -> { puts "run" }.call
来源：http://qkz.dianchejie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://yax.nwbrower.top

[C13] 类型声明 / 类型注解
来源：http://bru.316326.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gcu.tarul.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fzu.epnwcf.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ffy.ivvv.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rpv.feifeiyinyue.top

Java: int add(int a, int b) { return a + b; }
来源：http://cul.hnxiangtu.top

Go:   func add(a, b int) int
来源：http://bfa.gotoacloud.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ssa.bjfxy.top

C#:   int Add(int a, int b) => a + b;
来源：http://ikn.vqdsnc.cn

[C14] 泛型函数
来源：http://bqo.bjfxy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ezp.zhiwuduotai.top

PHP:  // 无泛型
来源：http://ypj.shuidangran.top

JS:   // 无泛型
来源：http://iwq.guowangkeji.top


<!-- 参考信息 -->