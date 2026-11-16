代发 wailian999

[A26] 类型转换总览
来源：http://utn.shanyushiyangtech.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://okw.yvedp.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dep.jinghuilouyu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pjq.zhixingplan.top

TS:   Number() String() Boolean() x as number
来源：http://mhx.jianghu66.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qkd.jinqigfzy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pnr.ydzc1.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://haa.daria6918.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lql.andypj.xyz

================================================================================
来源：http://jon.ppjwa.cn

B. 流程控制
来源：http://oqu.nwbrower.top

================================================================================
来源：http://awn.epnwcf.com

[B01] 条件判断 if / else
来源：http://rml.xingfuxueyuan.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://czz.shanyushiyangkeji.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jqi.kuanghao11.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jtu.yfazqb.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://knp.yuanzhike.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://uqh.yuanzhike.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://psx.ehwqpu.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jxt.quarkkingdee.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kvc.snrcjt.cn

[B02] 多分支 else if / elif
来源：http://mlv.ydzc1.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://grm.sxryk.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://whi.sxryk.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fdf.aibaodan.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nya.cashguo.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://klx.yj20258.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dop.hywenlv.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kzi.gzhubu.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lll.smart0.xyz

[B03] switch / match / case
来源：http://sie.shuidangran.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zpf.zdqjudy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yru.shanyushiyangtech.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ooq.yanxiufei.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ccn.shanyushiyangtech.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dli.zycfv.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dgu.xuanzx.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gaf.jinghuilouyu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qqs.meibo888.top

[B04] for 计数循环
来源：http://bql.svipenyu.cn

Py:   for i in range(10): print(i)
来源：http://yml.snrcjt.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://col.yongpay.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vwp.xylfe.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tfx.jqgufenzy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rhz.hcnkem.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lse.pengpengdd.cyou

Ruby: 10.times { |i| puts i }
来源：http://zhu.sxryk.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qyi.hammf.cn

[B05] 遍历数组 / 列表
来源：http://xeo.pycfn.com

Py:   for item in arr: print(item)
来源：http://pad.zdqjudy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bzl.snrcjt.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://huo.sjlbkw.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gpx.yueranfly.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://dvd.gogol.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cah.yj202588.top

Ruby: arr.each { |item| puts item }
来源：http://wfg.aibaodan.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tdi.ctjpmb.com

[B06] 遍历字典 / 对象
来源：http://oid.ivvv.top

Py:   for k, v in d.items(): print(k, v)
来源：http://zxt.zhixingplan.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ott.ydjk.org.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jju.redwolf501.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nnd.zhiwuduotai.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lzz.hnxiangtu.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nij.birdmap.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dfu.hnqzz.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fii.chenzaomai.com

[B07] while 循环
来源：http://yhq.dashuyun.cn

Py:   while i < 10: i += 1
来源：http://iwm.feifeiyinyue.top

PHP:  while ($i < 10) { $i++; }
来源：http://uhk.aizwys.cn

JS:   while (i < 10) { i++; }
来源：http://ueg.zhiwuduotai.top

TS:   while (i < 10) { i++; }
来源：http://hdy.jlsjyb.cn

Java: while (i < 10) { i++; }
来源：http://mvq.bbcook.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kgb.iojbl.cn

Ruby: while i < 10; i += 1; end
来源：http://atn.hysaishi.cn

C#:   while (i < 10) { i++; }
来源：http://dyy.gaohongyu789.top

[B08] do-while（至少执行一次）
来源：http://kdi.yangfankeji.com

Py:   # 无 do-while：用 while True + break
来源：http://wau.zdbjq.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ujw.smart0.xyz

JS:   do { i++; } while (i < 10);
来源：http://pdj.c1oappe.top

TS:   do { i++; } while (i < 10);
来源：http://dam.hywenlv.cn

Java: do { i++; } while (i < 10);
来源：http://jmd.xuanzx.com

Go:   for { i++; if i >= 10 { break } }
来源：http://fza.yj20258.top

Ruby: begin; i += 1; end while i < 10
来源：http://ytx.nwbrower.top

C#:   do { i++; } while (i < 10);
来源：http://uri.zhengqikj.top

[B09] break 与 continue
来源：http://ihv.cheryme.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://asn.yueranfly.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kca.vehdjk.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sdo.ppjwa.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aog.sjlbkw.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eiv.bjfxy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bdb.wangdashe.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nev.ydzc1.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zry.sysykeji.top

[B10] 遍历同时拿索引
来源：http://szm.vqdsnc.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ahk.ybcxt.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tpb.zhiwuduotai.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lzq.daria6918.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nzv.yj20258.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fxn.gzhubu.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ubx.zhoulong.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gig.gaohongyu789.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dkl.cheryme.top

[B11] 生成数字序列 / 区间
来源：http://jto.fktsv.cn

Py:   list(range(0, 10, 2))
来源：http://aeq.cdnleiting.top

PHP:  range(0, 10, 2);
来源：http://wqv.snrcjt.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ygc.nanxuanxn.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iie.tanke756.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wed.feifeiyinyue.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vel.zdbjq.cn

Ruby: (0...10).step(2).to_a
来源：http://blz.xziqi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zls.xziqi.cn

[B12] 跳出多层循环
来源：http://hjy.xuanzx.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://ini.cucudq.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zod.ctjpmb.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sst.shuidangran.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qie.jianghu66.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yzj.mhx1999.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bdz.fzhhl.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ixg.bbcook.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://btt.xylfe.cn

[B13] 判断是否为数字
来源：http://haw.cqqwz.cn

Py:   isinstance(x, (int, float))
来源：http://klx.snrcjt.cn

PHP:  is_numeric($x)
来源：http://zen.gzhubu.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ckq.gotoacloud.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mga.chenlongwang.top

Java: x instanceof Number
来源：http://hrx.zdqjudy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ukc.dianchejie.cn

Ruby: x.is_a?(Numeric)
来源：http://woc.fktsv.cn

C#:   x is int or double or decimal
来源：http://jgf.hywenlv.cn

[B14] 判断值是否在集合内
来源：http://rkw.yangfankeji.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vqg.shzxlz.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://krq.tian-w.cn

JS:   [1, 2, 3].includes(x)
来源：http://dxf.smart0.xyz

TS:   [1, 2, 3].includes(x)
来源：http://kez.ydzc1.top

Java: List.of(1, 2, 3).contains(x)
来源：http://whw.xingfuxueyuan.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jbs.quarkkingdee.top

Ruby: [1, 2, 3].include?(x)
来源：http://eda.fengsongda.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kca.yonumen.top

[B15] 布尔运算与取反
来源：http://jmn.hfpthk.cn

Py:   a and b or not c
来源：http://zlp.xingfuxueyuan.xyz

PHP:  $a && $b || !$c
来源：http://pul.yuxming.cn

JS:   a && b || !c
来源：http://nnz.xingfuxueyuan.xyz

TS:   a && b || !c
来源：http://dne.jinqigfzy.top

Java: a && b || !c
来源：http://zqp.redwolf501.top

Go:   a && b || !c
来源：http://bnw.shzxlz.cn

Ruby: a && b || !c
来源：http://juw.feifeiyinyue.top

C#:   a && b || !c
来源：http://umk.zhaomingkeji.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://uet.jqgufenzy.top

Py:   if not data: return
来源：http://vau.kuanghao11.cn

PHP:  if (!$data) { return; }
来源：http://gzo.ybcxt.top

JS:   if (!data) return;
来源：http://unk.zdqjudy.top

TS:   if (!data) return;
来源：http://mes.fzhhl.top

Java: if (data == null) return;
来源：http://sct.xuanzx.com

Go:   if data == nil { return }
来源：http://jib.yanxiufei.cn

Ruby: return if data.nil?
来源：http://evt.uphjek.com

C#:   if (data == null) return;
来源：http://bza.cucudq.cn

================================================================================
来源：http://koh.fehbvm.com

C. 函数与作用域
来源：http://yan.ivvv.top

================================================================================
来源：http://mez.fktsv.cn

[C01] 定义函数
来源：http://gnq.jinghuilouyu.cn

Py:   def add(a, b): return a + b
来源：http://gwe.fanxiaobao.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aul.cqqwz.cn

JS:   function add(a, b) { return a + b; }
来源：http://teh.jqgufenzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cfm.dianchejie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://jhs.yuanzhike.top

Go:   func add(a, b int) int { return a + b }
来源：http://gne.yfazqb.com

Ruby: def add(a, b); a + b; end
来源：http://iof.aizwys.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://paj.zhengqikj.top

[C02] 默认参数
来源：http://clo.tianlin.xyz

Py:   def greet(name="World"): return name
来源：http://ckj.c1oappe.top

PHP:  function greet($name = "World") { return $name; }
来源：http://iyq.aibaodan.cn

JS:   function greet(name = "World") { return name; }
来源：http://bko.jqgufenzy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://jkh.haohaochexian.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ybh.vqdsnc.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yeq.hcnkem.com

Ruby: def greet(name = "World") = name
来源：http://ipp.andypj.xyz

C#:   string Greet(string name = "World") => name;
来源：http://wbc.bjfxy.top

[C03] 可变参数
来源：http://vpa.hcnkem.com

Py:   def total(*args): return sum(args)
来源：http://gnl.uphjek.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uja.fzhhl.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xlj.xziqi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yjr.yj20258.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://awq.mhx1999.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wjs.0kj1m.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qlz.gaohongyu789.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dzw.chenzaomai.com

[C04] 命名参数 / 关键字参数
来源：http://pnh.shanyushiyangtech.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://suu.zhiwuduotai.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://enx.316326.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://agt.cqqwz.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hza.yfazqb.com

Java: // 无：用 Builder 模式或 record
来源：http://vrp.316326.xyz

Go:   // 无：用配置结构体参数
来源：http://zwr.zhijiandao.cn

Ruby: f(a: 1, b: 2)
来源：http://hby.jlsjyb.cn

C#:   f(a: 1, b: 2)
来源：http://mfq.zhoulong.xyz

[C05] 返回多个值
来源：http://tum.fanxiaobao.xyz

Py:   return a, b
来源：http://jhh.hnxiangtu.top

PHP:  return [$a, $b];
来源：http://zbf.chenlongwang.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://anc.zdbjq.cn

TS:   return { a, b };
来源：http://nku.hammf.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://czf.fktsv.cn

Go:   return a, b
来源：http://mcg.shzxlz.cn

Ruby: return a, b
来源：http://zrw.yj20258888.top

C#:   return (a, b);              // ValueTuple
来源：http://vwh.vehdjk.com

[C06] 匿名函数 / lambda
来源：http://osc.yongpay.top

Py:   square = lambda x: x * x
来源：http://gnc.epnwcf.com

PHP:  $square = fn($x) => $x * $x;
来源：http://izi.ivvv.top

JS:   const square = x => x * x;
来源：http://mvu.mhx1999.top

TS:   const square = (x: number): number => x * x;
来源：http://hsb.wangshuangyany.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fpb.xingfuxueyuan.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://jxt.hfpthk.cn

Ruby: square = ->(x) { x * x }
来源：http://wby.ehwqpu.com

C#:   Func<int, int> square = x => x * x;
来源：http://jpm.chenzaomai.com

[C07] 把函数作为参数传入
来源：http://xdv.yfazqb.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nre.gogol.net.cn

PHP:  array_map("strtoupper", $arr);
来源：http://fnc.gotoacloud.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://plc.hfpthk.cn

TS:   arr.map(String)
来源：http://fom.0kj1m.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zwg.hywenlv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://oke.xingfuxueyuan.xyz

Ruby: arr.map(&:upcase)
来源：http://sxp.dianchejie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://kmi.mhx1999.top

[C08] 闭包
来源：http://yls.zycfv.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hyg.chenlongwang.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nsy.dianchejie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://src.zhaomingkeji.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jrd.tanke756.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://frx.fehbvm.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://eib.hesvh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rdr.chenzaomai.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bfo.tianlin.xyz

[C09] 递归
来源：http://ytg.hfpthk.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nmw.jinyuanbaomall.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://olz.ehwqpu.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mur.sweek.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lki.aizwys.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wlu.nwbrower.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://clh.yangfankeji.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zge.quarkkingdee.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lnh.yj20258888.top

[C10] 变量作用域
来源：http://ilr.jqgufenzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://spi.havefunace.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cst.andypj.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://iqw.zhaomingkeji.xyz

TS:   同 JS
来源：http://vwd.fehbvm.com

Java: 方法内为块级作用域
来源：http://ngp.xuetiantiany.cn

Go:   花括号块级作用域
来源：http://icw.yueranfly.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mor.ydjk.org.cn

C#:   块级作用域
来源：http://ccu.daria6918.cn

[C11] 模块导入与导出
来源：http://iop.yangfankeji.com

Py:   from module import func
来源：http://miw.hesvh.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rhg.316326.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://llj.zycfv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yor.jinqigufen.top

Java: import java.util.List;
来源：http://jot.jlsjyb.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pky.jianghu66.top

Ruby: require "json"; require_relative "./util"
来源：http://dgs.shuidangran.top

C#:   using System.Text;
来源：http://gkp.dashuyun.cn

[C12] 立即执行函数 IIFE
来源：http://dgz.sjlbkw.cn

Py:   (lambda: print("run"))()
来源：http://cgu.sufxvd.cn

PHP:  (function () { echo "run"; })();
来源：http://xbz.yj20258888.top

JS:   (() => { console.log("run"); })();
来源：http://zqm.andypj.xyz

TS:   (() => { console.log("run"); })();
来源：http://vge.yangfankeji.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ccf.tarul.cn

Go:   func() { fmt.Println("run") }()
来源：http://ssi.yangfankeji.com

Ruby: -> { puts "run" }.call
来源：http://xbt.wangshuangyany.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://lza.chenzaomai.com

[C13] 类型声明 / 类型注解
来源：http://ukx.cashguo.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://czj.andypj.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gcz.vehdjk.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ltb.zhoulong.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oqj.xuetiantiany.cn

Java: int add(int a, int b) { return a + b; }
来源：http://aau.zhaomingkeji.xyz

Go:   func add(a, b int) int
来源：http://hal.gogol.net.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fpp.yongpay.top

C#:   int Add(int a, int b) => a + b;
来源：http://kfl.cheryme.top

[C14] 泛型函数
来源：http://rfd.yj20258.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zyi.dashuyun.cn

PHP:  // 无泛型
来源：http://rkv.hysaishi.cn

JS:   // 无泛型
来源：http://pqm.jinqigfzy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mug.wangdashe.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fzp.feifeiyinyue.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vou.zhaomingkeji.xyz

Ruby: # 无泛型
来源：http://hbz.hfpthk.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lif.hnqzz.top

[C15] 解构 / 展开参数
来源：http://heo.jinqigfzy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://azs.chenzaomai.com

PHP:  [$a, $b] = $pair;
来源：http://cpl.hnqzz.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ycb.yonumen.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mrw.ydzc1.top

Java: // 无解构
来源：http://tng.52xcode.cn

Go:   // 无解构
来源：http://fdb.pycfn.com

Ruby: a, b = pair
来源：http://bon.jqgfzy.top

C#:   var (a, b) = pair;
来源：http://nli.iojbl.cn

[C16] 函数 / 方法重载
来源：http://lce.yanxiufei.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wtq.uphjek.com

PHP:  // 无重载
来源：http://ycn.chenjidiqi.icu

JS:   // 无重载：靠 arguments.length 分支
来源：http://amk.xuanzx.com

TS:   // 用联合类型或重载签名声明
来源：http://siw.zhijiandao.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://usc.zhaomingkeji.xyz


<!-- 参考信息 -->