代发 wailian999

[A26] 类型转换总览
来源：http://kit.jqgufenzy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ysp.cqqwz.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qps.aibaodan.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ack.316326.xyz

TS:   Number() String() Boolean() x as number
来源：http://xil.yongpay.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nba.yangfankeji.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jra.bbcook.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lvk.kuanghao11.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cee.zycfv.cn

================================================================================
来源：http://qnh.birdmap.top

B. 流程控制
来源：http://ooj.yuxming.cn

================================================================================
来源：http://vih.tarul.cn

[B01] 条件判断 if / else
来源：http://aei.9152youxi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://kkp.svipenyu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zvt.gotoacloud.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ywg.hnxiangtu.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bwu.yuanzhike.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://shc.xuanzx.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://spi.0kj1m.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dpj.wangshuangyany.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ajd.smart0.xyz

[B02] 多分支 else if / elif
来源：http://azx.ctjpmb.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rna.shangyingyoupin.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hle.shzxlz.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://twj.daria6918.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lyf.c1oappe.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://chz.yuxming.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wpb.jlsjyb.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ipm.shangyingyoupin.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ibr.redwolf501.top

[B03] switch / match / case
来源：http://klf.birdmap.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://brc.52xcode.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gqf.jinghuilouyu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vhs.guowangkeji.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://egl.sysykeji.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://emk.fktsv.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rtw.uphjek.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uoi.cheryme.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://erw.aizwys.cn

[B04] for 计数循环
来源：http://iki.chenjidiqi.icu

Py:   for i in range(10): print(i)
来源：http://vle.yongpay.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tbl.hnxiangtu.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vvw.redwolf501.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kpr.smart0.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ooj.ybcxt.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hwt.gotoacloud.top

Ruby: 10.times { |i| puts i }
来源：http://bwn.ybcxt.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kjb.sufxvd.cn

[B05] 遍历数组 / 列表
来源：http://pyf.sufxvd.cn

Py:   for item in arr: print(item)
来源：http://ixa.sufxvd.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pig.ydzc1.top

JS:   for (const item of arr) { console.log(item); }
来源：http://pxp.guannengcc.top

TS:   for (const item of arr) { console.log(item); }
来源：http://kvs.nanxinkj.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://wds.yj202588.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dlr.0kj1m.cn

Ruby: arr.each { |item| puts item }
来源：http://txx.fengsongda.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ouh.xuanzx.com

[B06] 遍历字典 / 对象
来源：http://ipg.fanxiaobao.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://aqi.zhengqikj.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rwr.shzxlz.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hwp.chenjidiqi.icu

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jnd.smart0.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gkn.fehbvm.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lfd.zdbjq.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mdn.redwolf501.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fvr.hnqzz.top

[B07] while 循环
来源：http://ycz.jyoumei.cn

Py:   while i < 10: i += 1
来源：http://zol.xziqi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zum.sxryk.cn

JS:   while (i < 10) { i++; }
来源：http://kgj.fanxiaobao.xyz

TS:   while (i < 10) { i++; }
来源：http://suh.tianlin.xyz

Java: while (i < 10) { i++; }
来源：http://vvr.meibo888.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pam.ctjpmb.com

Ruby: while i < 10; i += 1; end
来源：http://ead.hysaishi.cn

C#:   while (i < 10) { i++; }
来源：http://uwj.guowangkeji.top

[B08] do-while（至少执行一次）
来源：http://zbr.vqdsnc.cn

Py:   # 无 do-while：用 while True + break
来源：http://rly.jqgufenzy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://esw.fzhhl.top

JS:   do { i++; } while (i < 10);
来源：http://itt.andypj.xyz

TS:   do { i++; } while (i < 10);
来源：http://wyp.feifeiyinyue.top

Java: do { i++; } while (i < 10);
来源：http://bkc.zhixingplan.top

Go:   for { i++; if i >= 10 { break } }
来源：http://szc.xylfe.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qwp.zycfv.cn

C#:   do { i++; } while (i < 10);
来源：http://msc.fktsv.cn

[B09] break 与 continue
来源：http://xeu.mhx1999.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lki.hongshengwenyu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://soo.wangshuangyany.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jem.zdqjudy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://daq.gaohongyu789.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://imr.fehbvm.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://aee.andypj.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zmv.tianlin.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sht.quarkkingdee.top

[B10] 遍历同时拿索引
来源：http://hth.zdqjudy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qjq.hesvh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lgi.fktsv.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://umf.yfazqb.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://iml.wangshuangyany.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nvj.uphjek.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jhv.vqdsnc.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uup.ivvv.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://voj.chenzaomai.com

[B11] 生成数字序列 / 区间
来源：http://bxb.yongpay.top

Py:   list(range(0, 10, 2))
来源：http://gyt.jinqigfzy.top

PHP:  range(0, 10, 2);
来源：http://qmb.meibo888.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hfc.cheryme.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fmv.hnxiangtu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kgp.yuxming.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lyi.tanke756.top

Ruby: (0...10).step(2).to_a
来源：http://dkh.ywan-chungtsiang.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uea.guowangkeji.top

[B12] 跳出多层循环
来源：http://waf.shzxlz.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://mqx.tian-w.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://tka.tanke756.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mvd.tarul.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pnt.xingfuxueyuan.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qsq.iojbl.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ffq.hysaishi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dev.zdqjudy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://urh.hysaishi.cn

[B13] 判断是否为数字
来源：http://bdl.bbcook.cn

Py:   isinstance(x, (int, float))
来源：http://xqq.jyoumei.cn

PHP:  is_numeric($x)
来源：http://kuu.chenzaomai.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://elh.tarul.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hxv.nanxinkj.top

Java: x instanceof Number
来源：http://hae.hesvh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dya.gotoacloud.top

Ruby: x.is_a?(Numeric)
来源：http://efj.jqgufenzy.top

C#:   x is int or double or decimal
来源：http://bbo.zhixingplan.top

[B14] 判断值是否在集合内
来源：http://del.jinqigfzy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://azo.tanke756.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://iig.ydjk.org.cn

JS:   [1, 2, 3].includes(x)
来源：http://tqw.zhiwuduotai.top

TS:   [1, 2, 3].includes(x)
来源：http://kqs.fengsongda.top

Java: List.of(1, 2, 3).contains(x)
来源：http://vrl.jianghu66.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://spw.hysaishi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://nba.epnwcf.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cbk.9152youxi.cn

[B15] 布尔运算与取反
来源：http://mdr.daria6918.cn

Py:   a and b or not c
来源：http://sjq.sjlbkw.cn

PHP:  $a && $b || !$c
来源：http://dtt.ydzc1.top

JS:   a && b || !c
来源：http://fqu.shangyingyoupin.top

TS:   a && b || !c
来源：http://lol.0kj1m.cn

Java: a && b || !c
来源：http://qpu.hfpthk.cn

Go:   a && b || !c
来源：http://guu.yfazqb.com

Ruby: a && b || !c
来源：http://koo.hammf.cn

C#:   a && b || !c
来源：http://epi.xylfe.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ned.gotoacloud.top

Py:   if not data: return
来源：http://des.yongpay.top

PHP:  if (!$data) { return; }
来源：http://bxj.svipenyu.cn

JS:   if (!data) return;
来源：http://fex.hesvh.cn

TS:   if (!data) return;
来源：http://xfz.jinghuilouyu.cn

Java: if (data == null) return;
来源：http://lpd.zhongyouzk.top

Go:   if data == nil { return }
来源：http://gkk.zhiwuduotai.top

Ruby: return if data.nil?
来源：http://yvb.zhongyouzk.top

C#:   if (data == null) return;
来源：http://xqa.vehdjk.com

================================================================================
来源：http://czx.hammf.cn

C. 函数与作用域
来源：http://max.haohaochexian.top

================================================================================
来源：http://bum.9152youxi.cn

[C01] 定义函数
来源：http://frv.ywan-chungtsiang.top

Py:   def add(a, b): return a + b
来源：http://ryn.cheryme.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rmj.guowangkeji.top

JS:   function add(a, b) { return a + b; }
来源：http://dqa.tian-w.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://plg.jinyuanbaomall.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://shd.shanyushiyangkeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://inb.nanxuanxn.top

Ruby: def add(a, b); a + b; end
来源：http://iwc.tarul.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://twp.jinqigufen.top

[C02] 默认参数
来源：http://ngx.hnqzz.top

Py:   def greet(name="World"): return name
来源：http://erz.uphjek.com

PHP:  function greet($name = "World") { return $name; }
来源：http://xcb.zhongyouzk.top

JS:   function greet(name = "World") { return name; }
来源：http://nwz.ctjpmb.com

TS:   function greet(name: string = "World") { return name; }
来源：http://ekq.ybcxt.top

Java: // 无默认参数：方法重载或 Optional
来源：http://gzh.xziqi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rku.hammf.cn

Ruby: def greet(name = "World") = name
来源：http://lbk.havefunace.top

C#:   string Greet(string name = "World") => name;
来源：http://muy.ppjwa.cn

[C03] 可变参数
来源：http://ink.yueranfly.top

Py:   def total(*args): return sum(args)
来源：http://mit.meibo888.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ksr.ybcxt.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jra.feifeiyinyue.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dbg.tianlin.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xnz.zycfv.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uxu.gotoacloud.top

Ruby: def total(*nums); nums.sum; end
来源：http://ash.zhixingplan.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xly.hnxiangtu.top

[C04] 命名参数 / 关键字参数
来源：http://gxk.jlsjyb.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://urk.gaohongyu789.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gbh.cdnleiting.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://djf.yanxiufei.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ynj.jqgufenzy.top

Java: // 无：用 Builder 模式或 record
来源：http://knw.cqqwz.cn

Go:   // 无：用配置结构体参数
来源：http://uir.smart0.xyz

Ruby: f(a: 1, b: 2)
来源：http://say.chenjidiqi.icu

C#:   f(a: 1, b: 2)
来源：http://slo.fzhhl.top

[C05] 返回多个值
来源：http://jyg.ppjwa.cn

Py:   return a, b
来源：http://onr.daxiang520.top

PHP:  return [$a, $b];
来源：http://ubl.xziqi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yal.mhx1999.top

TS:   return { a, b };
来源：http://ggg.hnxiangtu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lif.jinqigfzy.top

Go:   return a, b
来源：http://cvd.gzhubu.top

Ruby: return a, b
来源：http://cfb.snrcjt.cn

C#:   return (a, b);              // ValueTuple
来源：http://oyf.dashuyun.cn

[C06] 匿名函数 / lambda
来源：http://rmg.mhx1999.top

Py:   square = lambda x: x * x
来源：http://kjs.fzhhl.top

PHP:  $square = fn($x) => $x * $x;
来源：http://zed.ydzc1.top

JS:   const square = x => x * x;
来源：http://ctl.sjlbkw.cn

TS:   const square = (x: number): number => x * x;
来源：http://clx.yuxming.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://oei.sysykeji.top

Go:   sq := func(x int) int { return x * x }
来源：http://uqb.quarkkingdee.top

Ruby: square = ->(x) { x * x }
来源：http://lca.vehdjk.com

C#:   Func<int, int> square = x => x * x;
来源：http://tic.haohaochexian.top

[C07] 把函数作为参数传入
来源：http://cko.zhengqikj.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://szf.smart0.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://aug.dashuyun.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kaz.tanke756.top

TS:   arr.map(String)
来源：http://ktm.guannengcc.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cwi.shangyingyoupin.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nrr.smart0.xyz

Ruby: arr.map(&:upcase)
来源：http://dop.tarul.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://abr.zhijiandao.cn

[C08] 闭包
来源：http://eyr.snrcjt.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dtq.jianghu66.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fur.ehwqpu.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zeg.hfpthk.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://arp.svipenyu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ghu.tarul.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ohp.yangfankeji.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xjs.haohaochexian.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fkx.c1oappe.top

[C09] 递归
来源：http://tgm.zhengqikj.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qrf.hfpthk.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fpc.sxryk.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rje.jqgufenzy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hiw.tianlin.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://spe.zdqjudy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://iux.tarul.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mwt.gaohongyu789.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zwp.ehwqpu.com

[C10] 变量作用域
来源：http://fjm.9152youxi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bds.zhaomingkeji.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ysj.cashguo.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cae.zdqjudy.top

TS:   同 JS
来源：http://buo.hywenlv.cn

Java: 方法内为块级作用域
来源：http://fcu.gotoacloud.top

Go:   花括号块级作用域
来源：http://syf.jinyuanbaomall.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://anp.meibo888.top

C#:   块级作用域
来源：http://cjc.cdnleiting.top

[C11] 模块导入与导出
来源：http://miw.jianghu66.top

Py:   from module import func
来源：http://uan.chenlongwang.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ajg.vehdjk.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://oyc.jinghuilouyu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://utz.xingfuxueyuan.xyz

Java: import java.util.List;
来源：http://tkn.jlsjyb.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ght.sweek.top

Ruby: require "json"; require_relative "./util"
来源：http://hzn.dianchejie.cn

C#:   using System.Text;
来源：http://vgg.cashguo.top

[C12] 立即执行函数 IIFE
来源：http://zuq.zhaomingkeji.xyz

Py:   (lambda: print("run"))()
来源：http://ghz.gotoacloud.top

PHP:  (function () { echo "run"; })();
来源：http://acu.cdnleiting.top

JS:   (() => { console.log("run"); })();
来源：http://iip.dashuyun.cn

TS:   (() => { console.log("run"); })();
来源：http://qng.zdqjudy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gsw.zhixingplan.top

Go:   func() { fmt.Println("run") }()
来源：http://gkz.vehdjk.com

Ruby: -> { puts "run" }.call
来源：http://nuj.yvedp.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://dpc.jlsjyb.cn

[C13] 类型声明 / 类型注解
来源：http://dkp.tanke756.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://umz.zhoulong.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gvi.hesvh.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wzy.hesvh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qka.vqdsnc.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ujk.0kj1m.cn

Go:   func add(a, b int) int
来源：http://lpd.sysykeji.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fmj.yj20258888.top

C#:   int Add(int a, int b) => a + b;
来源：http://iqv.vqdsnc.cn

[C14] 泛型函数
来源：http://fpx.yonumen.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://igb.redwolf501.top

PHP:  // 无泛型
来源：http://nkj.zhijiandao.cn

JS:   // 无泛型
来源：http://tka.mhx1999.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bot.guannengcc.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xpd.nanxinkj.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ysv.smart0.xyz

Ruby: # 无泛型
来源：http://lud.epnwcf.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dsm.cdnleiting.top

[C15] 解构 / 展开参数
来源：http://kiw.zdbjq.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gtz.smart0.xyz

PHP:  [$a, $b] = $pair;
来源：http://ddm.ydzc1.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cwa.epnwcf.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://aug.gotoacloud.top

Java: // 无解构
来源：http://djr.shuidangran.top

Go:   // 无解构
来源：http://baw.pengpengdd.cyou

Ruby: a, b = pair
来源：http://xps.birdmap.top

C#:   var (a, b) = pair;
来源：http://sqb.hcnkem.com

[C16] 函数 / 方法重载
来源：http://xdk.mhx1999.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://puj.nanxuanxn.top

PHP:  // 无重载
来源：http://wcl.sweek.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ekq.jiagoushi.top

TS:   // 用联合类型或重载签名声明
来源：http://siv.shangyingyoupin.top

Java: void f(int a) {}  void f(String a) {}
来源：http://szn.cucudq.cn


<!-- 参考信息 -->