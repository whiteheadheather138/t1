代发 wailian999

[A26] 类型转换总览
来源：http://ayw.cqqwz.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ong.9152youxi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://izw.xinyue.icu

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://awi.cdnleiting.top

TS:   Number() String() Boolean() x as number
来源：http://chq.xylfe.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mpo.yongpay.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ngj.shanyushiyangtech.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ifo.zhixingplan.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lox.vehdjk.com

================================================================================
来源：http://lev.haohaochexian.top

B. 流程控制
来源：http://laf.tanke756.top

================================================================================
来源：http://ofz.daxiang520.top

[B01] 条件判断 if / else
来源：http://dla.jianghu66.top

Py:   result = "正" if x > 0 else "非正"
来源：http://rbx.yvedp.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://iun.cheryme.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rkf.c1oappe.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tjs.yueranfly.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://oti.smart0.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rpu.shangyingyoupin.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pfd.jinghuilouyu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://raa.jyoumei.cn

[B02] 多分支 else if / elif
来源：http://qly.birdmap.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wkm.guannengcc.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://uhv.jiagoushi.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rzz.zhiwuduotai.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://csc.ywan-chungtsiang.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zsd.nanxuanxn.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rrv.jinyuanbaomall.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://otg.tanke756.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ful.sweek.top

[B03] switch / match / case
来源：http://jjb.zdqjudy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xjp.iojbl.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://njm.cdnleiting.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rtn.daria6918.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kwo.yongpay.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dfv.yanxiufei.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://toa.ctjpmb.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nlv.hnxiangtu.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hcg.jianghu66.top

[B04] for 计数循环
来源：http://pmt.cheryme.top

Py:   for i in range(10): print(i)
来源：http://cgo.yuxming.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lyv.zdqjudy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fig.yonumen.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bzo.guowangkeji.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://joi.zhoulong.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://koy.havefunace.top

Ruby: 10.times { |i| puts i }
来源：http://olh.redwolf501.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fnd.jqgfzy.top

[B05] 遍历数组 / 列表
来源：http://frk.ywan-chungtsiang.top

Py:   for item in arr: print(item)
来源：http://nsn.cqqwz.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bla.ybcxt.top

JS:   for (const item of arr) { console.log(item); }
来源：http://jey.cashguo.top

TS:   for (const item of arr) { console.log(item); }
来源：http://lvl.yj20258888.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ics.chenlongwang.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://syc.zhixingplan.top

Ruby: arr.each { |item| puts item }
来源：http://epb.zhengqikj.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://asa.zdbjq.cn

[B06] 遍历字典 / 对象
来源：http://rkx.hnqzz.top

Py:   for k, v in d.items(): print(k, v)
来源：http://qwd.smart0.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nhv.chenjidiqi.icu

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jtz.9152youxi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yfu.yuxming.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jnh.shangyingyoupin.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ted.daxiang520.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yfg.uphjek.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ggs.sxryk.cn

[B07] while 循环
来源：http://wdv.chenzaomai.com

Py:   while i < 10: i += 1
来源：http://jpz.yj202588.top

PHP:  while ($i < 10) { $i++; }
来源：http://bdv.xziqi.cn

JS:   while (i < 10) { i++; }
来源：http://qzp.jinyuanbaomall.cn

TS:   while (i < 10) { i++; }
来源：http://cji.yanxiufei.cn

Java: while (i < 10) { i++; }
来源：http://ioj.kuanghao11.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bnj.ydjk.org.cn

Ruby: while i < 10; i += 1; end
来源：http://ojq.mhx1999.top

C#:   while (i < 10) { i++; }
来源：http://heo.chenzaomai.com

[B08] do-while（至少执行一次）
来源：http://run.ppjwa.cn

Py:   # 无 do-while：用 while True + break
来源：http://fav.hywenlv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rbt.svipenyu.cn

JS:   do { i++; } while (i < 10);
来源：http://dah.nanxinkj.top

TS:   do { i++; } while (i < 10);
来源：http://woz.chenjidiqi.icu

Java: do { i++; } while (i < 10);
来源：http://bfs.nanxinkj.top

Go:   for { i++; if i >= 10 { break } }
来源：http://olw.yuanzhike.top

Ruby: begin; i += 1; end while i < 10
来源：http://mxe.jinyuanbaomall.cn

C#:   do { i++; } while (i < 10);
来源：http://gvu.sweek.top

[B09] break 与 continue
来源：http://yxp.fehbvm.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://uyf.epnwcf.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mke.chenzaomai.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kvs.nanxinkj.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rvh.birdmap.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rba.yuanzhike.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xqu.meibo888.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wag.cucudq.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ojx.havefunace.top

[B10] 遍历同时拿索引
来源：http://osu.aibaodan.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yxq.shzxlz.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mkp.jiagoushi.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bzr.yuxming.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pis.vehdjk.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://evu.gzhubu.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nhq.ybcxt.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vkg.ybcxt.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://uin.fehbvm.com

[B11] 生成数字序列 / 区间
来源：http://vkb.sufxvd.cn

Py:   list(range(0, 10, 2))
来源：http://kgv.yangfankeji.com

PHP:  range(0, 10, 2);
来源：http://vqs.yuxming.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ppf.zhaomingkeji.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ukw.yvedp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kar.smart0.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xwt.jqgfzy.top

Ruby: (0...10).step(2).to_a
来源：http://jde.zycfv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jom.c1oappe.top

[B12] 跳出多层循环
来源：http://lql.birdmap.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ygv.cashguo.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ofh.shuidangran.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zqg.zhongyouzk.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nij.9152youxi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rvf.vehdjk.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cdh.daxiang520.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ejv.ywan-chungtsiang.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hug.zhongyouzk.top

[B13] 判断是否为数字
来源：http://seq.shzxlz.cn

Py:   isinstance(x, (int, float))
来源：http://qpv.yvedp.cn

PHP:  is_numeric($x)
来源：http://wkc.ctjpmb.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tmo.ivvv.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nea.guowangkeji.top

Java: x instanceof Number
来源：http://ztp.sjlbkw.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qaa.vehdjk.com

Ruby: x.is_a?(Numeric)
来源：http://vha.xylfe.cn

C#:   x is int or double or decimal
来源：http://ega.hywenlv.cn

[B14] 判断值是否在集合内
来源：http://xem.52xcode.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gmi.zhoulong.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://igp.havefunace.top

JS:   [1, 2, 3].includes(x)
来源：http://zhe.yj20258.top

TS:   [1, 2, 3].includes(x)
来源：http://wsg.tanke756.top

Java: List.of(1, 2, 3).contains(x)
来源：http://fdv.ehwqpu.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mag.iojbl.cn

Ruby: [1, 2, 3].include?(x)
来源：http://oii.tarul.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qkf.cheryme.top

[B15] 布尔运算与取反
来源：http://gqc.yfazqb.com

Py:   a and b or not c
来源：http://teu.cqqwz.cn

PHP:  $a && $b || !$c
来源：http://cmt.hammf.cn

JS:   a && b || !c
来源：http://qje.birdmap.top

TS:   a && b || !c
来源：http://uvg.hammf.cn

Java: a && b || !c
来源：http://urp.yj202588.top

Go:   a && b || !c
来源：http://dpg.andypj.xyz

Ruby: a && b || !c
来源：http://vnt.gzhubu.top

C#:   a && b || !c
来源：http://dkk.gogol.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://chp.zhiwuduotai.top

Py:   if not data: return
来源：http://hth.kuanghao11.cn

PHP:  if (!$data) { return; }
来源：http://byz.tanke756.top

JS:   if (!data) return;
来源：http://syt.chenlongwang.top

TS:   if (!data) return;
来源：http://eoo.yuxming.cn

Java: if (data == null) return;
来源：http://bgs.quarkkingdee.top

Go:   if data == nil { return }
来源：http://fnm.ppjwa.cn

Ruby: return if data.nil?
来源：http://bll.nanxinkj.top

C#:   if (data == null) return;
来源：http://jnd.chenjidiqi.icu

================================================================================
来源：http://qtl.sufxvd.cn

C. 函数与作用域
来源：http://kyl.yueranfly.top

================================================================================
来源：http://eju.dashuyun.cn

[C01] 定义函数
来源：http://wot.smart0.xyz

Py:   def add(a, b): return a + b
来源：http://fih.zhixingplan.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mye.zhixingplan.top

JS:   function add(a, b) { return a + b; }
来源：http://htu.uphjek.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nml.zhaomingkeji.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://iff.yuanzhike.top

Go:   func add(a, b int) int { return a + b }
来源：http://bnw.hnqzz.top

Ruby: def add(a, b); a + b; end
来源：http://wyu.andypj.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xjk.zdbjq.cn

[C02] 默认参数
来源：http://kui.jinghuilouyu.cn

Py:   def greet(name="World"): return name
来源：http://ago.pengpengdd.cyou

PHP:  function greet($name = "World") { return $name; }
来源：http://pra.yonumen.top

JS:   function greet(name = "World") { return name; }
来源：http://lbz.zhoulong.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://pce.zhiwuduotai.top

Java: // 无默认参数：方法重载或 Optional
来源：http://kno.c1oappe.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ztk.wangshuangyany.cn

Ruby: def greet(name = "World") = name
来源：http://pql.smart0.xyz

C#:   string Greet(string name = "World") => name;
来源：http://pkx.fzhhl.top

[C03] 可变参数
来源：http://fgu.tanke756.top

Py:   def total(*args): return sum(args)
来源：http://eed.hongshengwenyu.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pdc.ivvv.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jtg.chenjidiqi.icu

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qkw.fengsongda.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vdg.vehdjk.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nnk.fzhhl.top

Ruby: def total(*nums); nums.sum; end
来源：http://xkl.dianchejie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lzu.sjlbkw.cn

[C04] 命名参数 / 关键字参数
来源：http://svp.hnxiangtu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cdi.vqdsnc.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rtc.yangfankeji.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://oyd.ctjpmb.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gmh.ctjpmb.com

Java: // 无：用 Builder 模式或 record
来源：http://nnu.gotoacloud.top

Go:   // 无：用配置结构体参数
来源：http://cwb.fanxiaobao.xyz

Ruby: f(a: 1, b: 2)
来源：http://vfr.jinqigufen.top

C#:   f(a: 1, b: 2)
来源：http://jpq.xziqi.cn

[C05] 返回多个值
来源：http://ync.hongshengwenyu.top

Py:   return a, b
来源：http://hco.chenzaomai.com

PHP:  return [$a, $b];
来源：http://pvt.gaohongyu789.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://lto.sweek.top

TS:   return { a, b };
来源：http://vwu.fengsongda.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cuq.yangfankeji.com

Go:   return a, b
来源：http://ltk.cheryme.top

Ruby: return a, b
来源：http://pgb.shanyushiyangkeji.top

C#:   return (a, b);              // ValueTuple
来源：http://vle.dashuyun.cn

[C06] 匿名函数 / lambda
来源：http://tlh.tian-w.cn

Py:   square = lambda x: x * x
来源：http://mit.shangyingyoupin.top

PHP:  $square = fn($x) => $x * $x;
来源：http://rtg.nwbrower.top

JS:   const square = x => x * x;
来源：http://sfz.sweek.top

TS:   const square = (x: number): number => x * x;
来源：http://quh.jinyuanbaomall.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ttw.nwbrower.top

Go:   sq := func(x int) int { return x * x }
来源：http://pfu.snrcjt.cn

Ruby: square = ->(x) { x * x }
来源：http://ter.quarkkingdee.top

C#:   Func<int, int> square = x => x * x;
来源：http://nrx.yvedp.cn

[C07] 把函数作为参数传入
来源：http://lqe.sxryk.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nbs.daria6918.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mfj.vehdjk.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kdr.zdbjq.cn

TS:   arr.map(String)
来源：http://xqr.jyoumei.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wla.gotoacloud.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mjf.shangyingyoupin.top

Ruby: arr.map(&:upcase)
来源：http://nny.cucudq.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xem.fktsv.cn

[C08] 闭包
来源：http://odj.mhx1999.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ypm.nwbrower.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xvr.hnqzz.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qww.gzhubu.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xrq.316326.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tok.quarkkingdee.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://uza.shanyushiyangkeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ixv.zhoulong.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uvc.zhaomingkeji.xyz

[C09] 递归
来源：http://qio.ivvv.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cxf.birdmap.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bfa.jlsjyb.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jzm.aibaodan.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jlt.tarul.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qzp.ppjwa.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://yyj.andypj.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://aky.shanyushiyangkeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://loz.fanxiaobao.xyz

[C10] 变量作用域
来源：http://hod.fktsv.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tbb.hongshengwenyu.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ace.havefunace.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xpl.ivvv.top

TS:   同 JS
来源：http://fox.guowangkeji.top

Java: 方法内为块级作用域
来源：http://sre.jinyuanbaomall.cn

Go:   花括号块级作用域
来源：http://gjd.0kj1m.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ktd.snrcjt.cn

C#:   块级作用域
来源：http://xnz.yfazqb.com

[C11] 模块导入与导出
来源：http://npn.nanxuanxn.top

Py:   from module import func
来源：http://ktt.wangshuangyany.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://yny.hywenlv.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://tmz.epnwcf.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://znt.ivvv.top

Java: import java.util.List;
来源：http://xnf.hywenlv.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ihp.xuanzx.com

Ruby: require "json"; require_relative "./util"
来源：http://cpe.andypj.xyz

C#:   using System.Text;
来源：http://xxj.yj202588.top

[C12] 立即执行函数 IIFE
来源：http://xwt.xziqi.cn

Py:   (lambda: print("run"))()
来源：http://yjf.xinyue.icu

PHP:  (function () { echo "run"; })();
来源：http://pyc.pengpengdd.cyou

JS:   (() => { console.log("run"); })();
来源：http://aos.hysaishi.cn

TS:   (() => { console.log("run"); })();
来源：http://nro.redwolf501.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://byd.shanyushiyangkeji.top

Go:   func() { fmt.Println("run") }()
来源：http://ape.tanke756.top

Ruby: -> { puts "run" }.call
来源：http://llq.havefunace.top

C#:   // 无 IIFE：用静态构造函数
来源：http://wno.zhongyouzk.top

[C13] 类型声明 / 类型注解
来源：http://eji.wangdashe.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wuo.jyoumei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qda.0kj1m.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://irn.hnqzz.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vio.hnqzz.top

Java: int add(int a, int b) { return a + b; }
来源：http://bvv.yuxming.cn

Go:   func add(a, b int) int
来源：http://mce.kuanghao11.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cct.kuanghao11.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qpb.ivvv.top

[C14] 泛型函数
来源：http://jlc.zhijiandao.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ltb.9152youxi.cn

PHP:  // 无泛型
来源：http://abt.zdqjudy.top

JS:   // 无泛型
来源：http://zoz.daria6918.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://aop.vqdsnc.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://acl.ywan-chungtsiang.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bsi.haohaochexian.top

Ruby: # 无泛型
来源：http://kes.smart0.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://uty.dianchejie.cn

[C15] 解构 / 展开参数
来源：http://rih.sufxvd.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ebg.cucudq.cn

PHP:  [$a, $b] = $pair;
来源：http://sej.zhijiandao.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hyb.zhoulong.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lpr.guannengcc.top

Java: // 无解构
来源：http://zfd.ppjwa.cn

Go:   // 无解构
来源：http://fow.yongpay.top

Ruby: a, b = pair
来源：http://ioq.jqgfzy.top

C#:   var (a, b) = pair;
来源：http://rcg.hammf.cn

[C16] 函数 / 方法重载
来源：http://wwn.gotoacloud.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dix.dashuyun.cn

PHP:  // 无重载
来源：http://tnc.zdqjudy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://cxl.zdbjq.cn

TS:   // 用联合类型或重载签名声明
来源：http://ukq.xylfe.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://kan.9152youxi.cn


<!-- 参考信息 -->