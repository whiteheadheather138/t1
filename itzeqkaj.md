代发 wailian999

[A26] 类型转换总览
来源：http://nhf.jinqigufen.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://eka.gaohongyu789.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mwy.jiagoushi.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://htb.cqqwz.cn

TS:   Number() String() Boolean() x as number
来源：http://emx.sysykeji.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ufw.hongshengwenyu.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xwx.jinqigfzy.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://zhp.wangdashe.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wdy.yuanzhike.top

================================================================================
来源：http://jjz.xziqi.cn

B. 流程控制
来源：http://rak.hcnkem.com

================================================================================
来源：http://gbp.zhiwuduotai.top

[B01] 条件判断 if / else
来源：http://xal.zdqjudy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://dla.ppjwa.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lyc.pycfn.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bcj.jinyuanbaomall.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mby.jqgufenzy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://uzm.ywan-chungtsiang.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tco.nanxinkj.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xgs.xuanzx.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zhg.hammf.cn

[B02] 多分支 else if / elif
来源：http://axd.jianghu66.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ail.jinqigfzy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fyj.quarkkingdee.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tjt.jinqigfzy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wzy.pengpengdd.cyou

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sqz.zdqjudy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://klw.daria6918.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zxe.tianlin.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zne.svipenyu.cn

[B03] switch / match / case
来源：http://fsu.yj20258888.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://exh.yj20258.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dwu.uphjek.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wzz.fanxiaobao.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xay.316326.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://acr.ctjpmb.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kpj.shanyushiyangkeji.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://prq.ydzc1.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://aqa.smart0.xyz

[B04] for 计数循环
来源：http://vid.zhongyouzk.top

Py:   for i in range(10): print(i)
来源：http://azu.yonumen.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vfm.tianlin.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zht.shanyushiyangtech.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hxm.sweek.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gmm.ywan-chungtsiang.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://eva.chenjidiqi.icu

Ruby: 10.times { |i| puts i }
来源：http://cxc.chenlongwang.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ygs.ivvv.top

[B05] 遍历数组 / 列表
来源：http://tfo.316326.xyz

Py:   for item in arr: print(item)
来源：http://bwp.gzhubu.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vku.snrcjt.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ysu.yuanzhike.top

TS:   for (const item of arr) { console.log(item); }
来源：http://yfs.wangshuangyany.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://cac.chenlongwang.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ufl.cqqwz.cn

Ruby: arr.each { |item| puts item }
来源：http://gjf.bjfxy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kan.sweek.top

[B06] 遍历字典 / 对象
来源：http://oct.sweek.top

Py:   for k, v in d.items(): print(k, v)
来源：http://blv.jinyuanbaomall.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ntc.shanyushiyangkeji.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iri.ctjpmb.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dvb.zycfv.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yku.jianghu66.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wdq.jianghu66.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vsv.fehbvm.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://odd.nanxinkj.top

[B07] while 循环
来源：http://whd.gaohongyu789.top

Py:   while i < 10: i += 1
来源：http://nqx.havefunace.top

PHP:  while ($i < 10) { $i++; }
来源：http://tmt.svipenyu.cn

JS:   while (i < 10) { i++; }
来源：http://cat.jinqigufen.top

TS:   while (i < 10) { i++; }
来源：http://chn.jinqigfzy.top

Java: while (i < 10) { i++; }
来源：http://ufc.sufxvd.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uqz.gaohongyu789.top

Ruby: while i < 10; i += 1; end
来源：http://lat.sweek.top

C#:   while (i < 10) { i++; }
来源：http://jqu.dianchejie.cn

[B08] do-while（至少执行一次）
来源：http://xam.svipenyu.cn

Py:   # 无 do-while：用 while True + break
来源：http://ram.hnqzz.top

PHP:  do { $i++; } while ($i < 10);
来源：http://jjs.svipenyu.cn

JS:   do { i++; } while (i < 10);
来源：http://jil.dashuyun.cn

TS:   do { i++; } while (i < 10);
来源：http://kqm.nanxuanxn.top

Java: do { i++; } while (i < 10);
来源：http://dkd.jqgfzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://beq.fengsongda.top

Ruby: begin; i += 1; end while i < 10
来源：http://btk.xziqi.cn

C#:   do { i++; } while (i < 10);
来源：http://znq.shangyingyoupin.top

[B09] break 与 continue
来源：http://kfe.yangfankeji.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wyb.xingfuxueyuan.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hfo.nanxuanxn.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zyo.xylfe.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://flb.vqdsnc.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jzo.jinyuanbaomall.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fgv.9152youxi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://eal.zhoulong.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jxa.sysykeji.top

[B10] 遍历同时拿索引
来源：http://oij.yfazqb.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bcs.mhx1999.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://aih.zhiwuduotai.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fge.zhiwuduotai.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rlp.52xcode.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vgv.aibaodan.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ndf.jianghu66.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wez.cheryme.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rcl.jinqigfzy.top

[B11] 生成数字序列 / 区间
来源：http://xtm.smart0.xyz

Py:   list(range(0, 10, 2))
来源：http://dog.zhixingplan.top

PHP:  range(0, 10, 2);
来源：http://gwd.cqqwz.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nue.aizwys.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xot.hammf.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://eja.meibo888.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xjz.nwbrower.top

Ruby: (0...10).step(2).to_a
来源：http://smt.9152youxi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://beq.wangdashe.top

[B12] 跳出多层循环
来源：http://zcz.yonumen.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://uau.zhongyouzk.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://irm.zhengqikj.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://saz.daxiang520.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://btt.tanke756.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wfp.fehbvm.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sep.smart0.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bfm.yj20258.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vfz.cdnleiting.top

[B13] 判断是否为数字
来源：http://obq.fehbvm.com

Py:   isinstance(x, (int, float))
来源：http://dpo.jqgfzy.top

PHP:  is_numeric($x)
来源：http://eiv.jqgfzy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uvn.chenlongwang.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pwr.snrcjt.cn

Java: x instanceof Number
来源：http://htn.hcnkem.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sru.hesvh.cn

Ruby: x.is_a?(Numeric)
来源：http://jjt.vqdsnc.cn

C#:   x is int or double or decimal
来源：http://slm.guannengcc.top

[B14] 判断值是否在集合内
来源：http://ngf.ctjpmb.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://itr.uphjek.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://miv.jinghuilouyu.cn

JS:   [1, 2, 3].includes(x)
来源：http://syh.vqdsnc.cn

TS:   [1, 2, 3].includes(x)
来源：http://jwv.yuanzhike.top

Java: List.of(1, 2, 3).contains(x)
来源：http://hhy.iojbl.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://oba.guannengcc.top

Ruby: [1, 2, 3].include?(x)
来源：http://yat.hysaishi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dce.bjfxy.top

[B15] 布尔运算与取反
来源：http://ttv.dashuyun.cn

Py:   a and b or not c
来源：http://mag.zhijiandao.cn

PHP:  $a && $b || !$c
来源：http://vib.tanke756.top

JS:   a && b || !c
来源：http://gyp.hongshengwenyu.top

TS:   a && b || !c
来源：http://tfj.ehwqpu.com

Java: a && b || !c
来源：http://iib.bjfxy.top

Go:   a && b || !c
来源：http://fad.tarul.cn

Ruby: a && b || !c
来源：http://jlg.hnqzz.top

C#:   a && b || !c
来源：http://vbf.cdnleiting.top

[B16] 卫语句：不满足条件提前返回
来源：http://hqr.feifeiyinyue.top

Py:   if not data: return
来源：http://yza.gotoacloud.top

PHP:  if (!$data) { return; }
来源：http://euk.sufxvd.cn

JS:   if (!data) return;
来源：http://ydo.zycfv.cn

TS:   if (!data) return;
来源：http://lxf.birdmap.top

Java: if (data == null) return;
来源：http://xgy.zhixingplan.top

Go:   if data == nil { return }
来源：http://iwh.birdmap.top

Ruby: return if data.nil?
来源：http://imx.yuanzhike.top

C#:   if (data == null) return;
来源：http://yoh.mhx1999.top

================================================================================
来源：http://aru.yanxiufei.cn

C. 函数与作用域
来源：http://qnp.gaohongyu789.top

================================================================================
来源：http://hxr.fanxiaobao.xyz

[C01] 定义函数
来源：http://igj.gzhubu.top

Py:   def add(a, b): return a + b
来源：http://ibj.fzhhl.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pxq.pengpengdd.cyou

JS:   function add(a, b) { return a + b; }
来源：http://oyz.hfpthk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dqm.shanyushiyangkeji.top

Java: static int add(int a, int b) { return a + b; }
来源：http://zvb.yueranfly.top

Go:   func add(a, b int) int { return a + b }
来源：http://sqi.zhaomingkeji.xyz

Ruby: def add(a, b); a + b; end
来源：http://zbq.jiagoushi.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://use.iojbl.cn

[C02] 默认参数
来源：http://pmm.xinyue.icu

Py:   def greet(name="World"): return name
来源：http://whc.tarul.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://gpi.fzhhl.top

JS:   function greet(name = "World") { return name; }
来源：http://agu.jyoumei.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ikb.zhengqikj.top

Java: // 无默认参数：方法重载或 Optional
来源：http://hlq.svipenyu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wsq.gaohongyu789.top

Ruby: def greet(name = "World") = name
来源：http://poz.yvedp.cn

C#:   string Greet(string name = "World") => name;
来源：http://bya.aibaodan.cn

[C03] 可变参数
来源：http://sfp.quarkkingdee.top

Py:   def total(*args): return sum(args)
来源：http://ekw.jinyuanbaomall.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vod.fehbvm.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wmt.aizwys.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rhn.hesvh.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dva.shangyingyoupin.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gwq.shangyingyoupin.top

Ruby: def total(*nums); nums.sum; end
来源：http://dgb.mhx1999.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dgs.xylfe.cn

[C04] 命名参数 / 关键字参数
来源：http://wdx.guowangkeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mvq.cashguo.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xth.yuanzhike.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tkv.wangdashe.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kvy.guowangkeji.top

Java: // 无：用 Builder 模式或 record
来源：http://ylq.chenzaomai.com

Go:   // 无：用配置结构体参数
来源：http://xhi.fktsv.cn

Ruby: f(a: 1, b: 2)
来源：http://iro.zhengqikj.top

C#:   f(a: 1, b: 2)
来源：http://fsw.xylfe.cn

[C05] 返回多个值
来源：http://isy.ppjwa.cn

Py:   return a, b
来源：http://cqk.zdqjudy.top

PHP:  return [$a, $b];
来源：http://vqe.tarul.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://gqa.yuanzhike.top

TS:   return { a, b };
来源：http://rtj.cdnleiting.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bgj.ivvv.top

Go:   return a, b
来源：http://uni.tian-w.cn

Ruby: return a, b
来源：http://jkf.cheryme.top

C#:   return (a, b);              // ValueTuple
来源：http://ebd.yueranfly.top

[C06] 匿名函数 / lambda
来源：http://gpk.hnqzz.top

Py:   square = lambda x: x * x
来源：http://yez.hcnkem.com

PHP:  $square = fn($x) => $x * $x;
来源：http://ouq.feifeiyinyue.top

JS:   const square = x => x * x;
来源：http://ltg.ydzc1.top

TS:   const square = (x: number): number => x * x;
来源：http://qbh.xinyue.icu

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cln.ppjwa.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kml.sufxvd.cn

Ruby: square = ->(x) { x * x }
来源：http://ikg.jiagoushi.top

C#:   Func<int, int> square = x => x * x;
来源：http://tee.daxiang520.top

[C07] 把函数作为参数传入
来源：http://gcx.hesvh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zxc.feifeiyinyue.top

PHP:  array_map("strtoupper", $arr);
来源：http://wkk.ybcxt.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://omn.hywenlv.cn

TS:   arr.map(String)
来源：http://gjl.gzhubu.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://inw.tanke756.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vgk.0kj1m.cn

Ruby: arr.map(&:upcase)
来源：http://zap.316326.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://drd.zhijiandao.cn

[C08] 闭包
来源：http://blq.zycfv.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tod.meibo888.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jmi.jinqigfzy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mtu.yj20258.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qjc.ybcxt.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tof.wangshuangyany.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qjz.yfazqb.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://klh.kuanghao11.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rwe.jlsjyb.cn

[C09] 递归
来源：http://sih.sufxvd.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rat.hnxiangtu.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://iic.jqgfzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fkk.tian-w.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bng.gogol.net.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hzg.zhoulong.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xgp.zhengqikj.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lio.wangdashe.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kue.316326.xyz

[C10] 变量作用域
来源：http://yxi.chenjidiqi.icu

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yao.0kj1m.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://izh.fzhhl.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hhl.fanxiaobao.xyz

TS:   同 JS
来源：http://cjl.aizwys.cn

Java: 方法内为块级作用域
来源：http://mue.c1oappe.top

Go:   花括号块级作用域
来源：http://nzq.shzxlz.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bom.yanxiufei.cn

C#:   块级作用域
来源：http://luq.daxiang520.top

[C11] 模块导入与导出
来源：http://aul.cucudq.cn

Py:   from module import func
来源：http://gts.dianchejie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hkl.xuetiantiany.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gxu.jiagoushi.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://anv.gotoacloud.top

Java: import java.util.List;
来源：http://ogs.quarkkingdee.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bip.xuanzx.com

Ruby: require "json"; require_relative "./util"
来源：http://ubf.yvedp.cn

C#:   using System.Text;
来源：http://jnt.fengsongda.top

[C12] 立即执行函数 IIFE
来源：http://dtf.svipenyu.cn

Py:   (lambda: print("run"))()
来源：http://gbe.tianlin.xyz

PHP:  (function () { echo "run"; })();
来源：http://lkh.zdbjq.cn

JS:   (() => { console.log("run"); })();
来源：http://iuc.svipenyu.cn

TS:   (() => { console.log("run"); })();
来源：http://key.redwolf501.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bcg.yonumen.top

Go:   func() { fmt.Println("run") }()
来源：http://hgs.yfazqb.com

Ruby: -> { puts "run" }.call
来源：http://vgo.tarul.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://dmm.shuidangran.top

[C13] 类型声明 / 类型注解
来源：http://ndx.ydzc1.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://elj.fktsv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tif.wangshuangyany.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jtz.52xcode.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pzm.cheryme.top

Java: int add(int a, int b) { return a + b; }
来源：http://fzj.nwbrower.top

Go:   func add(a, b int) int
来源：http://pab.9152youxi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nro.gzhubu.top

C#:   int Add(int a, int b) => a + b;
来源：http://wja.daxiang520.top

[C14] 泛型函数
来源：http://jwm.zhoulong.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qso.haohaochexian.top

PHP:  // 无泛型
来源：http://kwj.tarul.cn

JS:   // 无泛型
来源：http://xwn.guowangkeji.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jnt.yfazqb.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rjf.xinyue.icu

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gps.c1oappe.top

Ruby: # 无泛型
来源：http://hyc.feifeiyinyue.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mdo.zhoulong.xyz

[C15] 解构 / 展开参数
来源：http://dwo.jinghuilouyu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qko.yongpay.top

PHP:  [$a, $b] = $pair;
来源：http://bom.xylfe.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://joj.wangdashe.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ywx.c1oappe.top

Java: // 无解构
来源：http://ovj.hnqzz.top

Go:   // 无解构
来源：http://ayp.zhixingplan.top

Ruby: a, b = pair
来源：http://oqg.xingfuxueyuan.xyz

C#:   var (a, b) = pair;
来源：http://jcn.hywenlv.cn

[C16] 函数 / 方法重载
来源：http://gee.fanxiaobao.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pqk.ywan-chungtsiang.top

PHP:  // 无重载
来源：http://ybk.ctjpmb.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://elg.bbcook.cn

TS:   // 用联合类型或重载签名声明
来源：http://brl.nanxuanxn.top

Java: void f(int a) {}  void f(String a) {}
来源：http://xbf.zhoulong.xyz


<!-- 参考信息 -->