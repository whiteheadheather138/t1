代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://zhi.yueranfly.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://roc.yuanzhike.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lla.wangshuangyany.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ipx.hnqzz.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vku.meibo888.top

================================================================================
来源：http://ktt.xylfe.cn

B. 流程控制
来源：http://iyu.chenjidiqi.icu

================================================================================
来源：http://hhn.feifeiyinyue.top

[B01] 条件判断 if / else
来源：http://czu.sweek.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ejb.xuanzx.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lwr.sxryk.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tee.feifeiyinyue.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jur.zhongyouzk.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://vxy.jlsjyb.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://oxf.hnqzz.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://utq.nwbrower.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ncy.xingfuxueyuan.xyz

[B02] 多分支 else if / elif
来源：http://shh.0kj1m.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://eje.ydzc1.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sid.hammf.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ezl.hongshengwenyu.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yxv.zhijiandao.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uii.ywan-chungtsiang.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fcd.cheryme.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rbe.vqdsnc.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ckt.hongshengwenyu.top

[B03] switch / match / case
来源：http://iei.jyoumei.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ixq.yuxming.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ket.sweek.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://clr.jlsjyb.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yhm.zdbjq.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ilm.zhongyouzk.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nvb.shangyingyoupin.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fpj.gotoacloud.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kdp.yanxiufei.cn

[B04] for 计数循环
来源：http://sni.fehbvm.com

Py:   for i in range(10): print(i)
来源：http://btm.iojbl.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kzm.guannengcc.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://btl.hcnkem.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ubp.hnqzz.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mui.wangdashe.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://opj.daria6918.cn

Ruby: 10.times { |i| puts i }
来源：http://wgi.feifeiyinyue.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vvi.jqgufenzy.top

[B05] 遍历数组 / 列表
来源：http://nfj.sweek.top

Py:   for item in arr: print(item)
来源：http://rms.cqqwz.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ybt.daxiang520.top

JS:   for (const item of arr) { console.log(item); }
来源：http://qbe.zhijiandao.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bok.pycfn.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://wsh.iojbl.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zcm.ppjwa.cn

Ruby: arr.each { |item| puts item }
来源：http://ohd.hesvh.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gsv.jinghuilouyu.cn

[B06] 遍历字典 / 对象
来源：http://dxo.bjfxy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://iff.jiagoushi.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cpc.jinyuanbaomall.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eez.cdnleiting.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fod.snrcjt.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nlb.tanke756.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://aqf.svipenyu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sxx.shuidangran.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://usb.zhaomingkeji.xyz

[B07] while 循环
来源：http://gsv.smart0.xyz

Py:   while i < 10: i += 1
来源：http://wri.jinghuilouyu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://rix.wangshuangyany.cn

JS:   while (i < 10) { i++; }
来源：http://zsm.yvedp.cn

TS:   while (i < 10) { i++; }
来源：http://hpa.jianghu66.top

Java: while (i < 10) { i++; }
来源：http://uor.andypj.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jzc.tanke756.top

Ruby: while i < 10; i += 1; end
来源：http://vvz.yj20258.top

C#:   while (i < 10) { i++; }
来源：http://rcx.xingfuxueyuan.xyz

[B08] do-while（至少执行一次）
来源：http://hqk.sjlbkw.cn

Py:   # 无 do-while：用 while True + break
来源：http://bni.ydjk.org.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jmz.havefunace.top

JS:   do { i++; } while (i < 10);
来源：http://ste.yanxiufei.cn

TS:   do { i++; } while (i < 10);
来源：http://dkw.iojbl.cn

Java: do { i++; } while (i < 10);
来源：http://oqy.cashguo.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ass.xylfe.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ymj.jqgufenzy.top

C#:   do { i++; } while (i < 10);
来源：http://ipr.jqgufenzy.top

[B09] break 与 continue
来源：http://cme.ybcxt.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://drs.nwbrower.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hpk.yangfankeji.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://skg.zhongyouzk.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xhm.zhixingplan.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pmd.jqgfzy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://apk.dashuyun.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jnx.zhengqikj.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tge.jqgfzy.top

[B10] 遍历同时拿索引
来源：http://zbr.fehbvm.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://eeh.mhx1999.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fyw.dianchejie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sql.quarkkingdee.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://etx.hfpthk.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dha.zhoulong.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qta.hysaishi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tbd.zdbjq.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bgn.iojbl.cn

[B11] 生成数字序列 / 区间
来源：http://yvq.316326.xyz

Py:   list(range(0, 10, 2))
来源：http://ghk.guowangkeji.top

PHP:  range(0, 10, 2);
来源：http://mkq.ydzc1.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xsb.hnqzz.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aom.fengsongda.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qxr.0kj1m.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xrj.bbcook.cn

Ruby: (0...10).step(2).to_a
来源：http://qln.shanyushiyangtech.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mhe.wangshuangyany.cn

[B12] 跳出多层循环
来源：http://qlt.jqgfzy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://aqt.jyoumei.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://yvp.jianghu66.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://khd.zdqjudy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ldd.ydzc1.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zhu.smart0.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://svo.sysykeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hwy.jqgufenzy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://oge.jinqigfzy.top

[B13] 判断是否为数字
来源：http://eme.hammf.cn

Py:   isinstance(x, (int, float))
来源：http://zgw.52xcode.cn

PHP:  is_numeric($x)
来源：http://mra.xylfe.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aqc.haohaochexian.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uth.cheryme.top

Java: x instanceof Number
来源：http://tzs.yj20258888.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zne.hysaishi.cn

Ruby: x.is_a?(Numeric)
来源：http://fed.tianlin.xyz

C#:   x is int or double or decimal
来源：http://ggv.vqdsnc.cn

[B14] 判断值是否在集合内
来源：http://igx.dianchejie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uzn.guowangkeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://utu.shzxlz.cn

JS:   [1, 2, 3].includes(x)
来源：http://sca.feifeiyinyue.top

TS:   [1, 2, 3].includes(x)
来源：http://eva.tarul.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qzb.yvedp.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cfd.fehbvm.com

Ruby: [1, 2, 3].include?(x)
来源：http://dze.svipenyu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://edq.hnqzz.top

[B15] 布尔运算与取反
来源：http://tgx.nanxinkj.top

Py:   a and b or not c
来源：http://wdd.sweek.top

PHP:  $a && $b || !$c
来源：http://nav.iojbl.cn

JS:   a && b || !c
来源：http://hdg.kuanghao11.cn

TS:   a && b || !c
来源：http://wwt.hywenlv.cn

Java: a && b || !c
来源：http://xcb.sufxvd.cn

Go:   a && b || !c
来源：http://yvo.shanyushiyangkeji.top

Ruby: a && b || !c
来源：http://cws.cucudq.cn

C#:   a && b || !c
来源：http://zpo.pycfn.com

[B16] 卫语句：不满足条件提前返回
来源：http://xbw.sysykeji.top

Py:   if not data: return
来源：http://zbx.zycfv.cn

PHP:  if (!$data) { return; }
来源：http://gmy.sweek.top

JS:   if (!data) return;
来源：http://ecz.sjlbkw.cn

TS:   if (!data) return;
来源：http://gdj.pycfn.com

Java: if (data == null) return;
来源：http://myl.cheryme.top

Go:   if data == nil { return }
来源：http://udc.cqqwz.cn

Ruby: return if data.nil?
来源：http://awc.zdqjudy.top

C#:   if (data == null) return;
来源：http://dcv.yfazqb.com

================================================================================
来源：http://osv.cqqwz.cn

C. 函数与作用域
来源：http://znr.dianchejie.cn

================================================================================
来源：http://msm.pengpengdd.cyou

[C01] 定义函数
来源：http://drp.0kj1m.cn

Py:   def add(a, b): return a + b
来源：http://xrx.jinghuilouyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xwo.shuidangran.top

JS:   function add(a, b) { return a + b; }
来源：http://tif.jqgfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ryb.xinyue.icu

Java: static int add(int a, int b) { return a + b; }
来源：http://lrz.tian-w.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vuy.haohaochexian.top

Ruby: def add(a, b); a + b; end
来源：http://pnb.fanxiaobao.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pfo.cucudq.cn

[C02] 默认参数
来源：http://exc.chenjidiqi.icu

Py:   def greet(name="World"): return name
来源：http://zig.jinqigfzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ptu.fanxiaobao.xyz

JS:   function greet(name = "World") { return name; }
来源：http://xep.haohaochexian.top

TS:   function greet(name: string = "World") { return name; }
来源：http://rtp.hnqzz.top

Java: // 无默认参数：方法重载或 Optional
来源：http://bue.yj20258.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vwl.xylfe.cn

Ruby: def greet(name = "World") = name
来源：http://com.ywan-chungtsiang.top

C#:   string Greet(string name = "World") => name;
来源：http://hix.yfazqb.com

[C03] 可变参数
来源：http://evl.hnxiangtu.top

Py:   def total(*args): return sum(args)
来源：http://fih.fanxiaobao.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nms.quarkkingdee.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://opf.havefunace.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ygk.pengpengdd.cyou

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lgw.jinqigfzy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wts.hesvh.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kye.jianghu66.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://oeu.pycfn.com

[C04] 命名参数 / 关键字参数
来源：http://gnx.hnxiangtu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ocj.jianghu66.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xyo.smart0.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rfj.cqqwz.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vox.epnwcf.com

Java: // 无：用 Builder 模式或 record
来源：http://ltt.guannengcc.top

Go:   // 无：用配置结构体参数
来源：http://wpo.tarul.cn

Ruby: f(a: 1, b: 2)
来源：http://uur.dashuyun.cn

C#:   f(a: 1, b: 2)
来源：http://rgp.zhixingplan.top

[C05] 返回多个值
来源：http://dyy.zdqjudy.top

Py:   return a, b
来源：http://lhf.zhongyouzk.top

PHP:  return [$a, $b];
来源：http://wqs.shanyushiyangtech.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://jfo.kuanghao11.cn

TS:   return { a, b };
来源：http://nnr.tarul.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dlv.vqdsnc.cn

Go:   return a, b
来源：http://jxw.uphjek.com

Ruby: return a, b
来源：http://ryr.fehbvm.com

C#:   return (a, b);              // ValueTuple
来源：http://qbi.c1oappe.top

[C06] 匿名函数 / lambda
来源：http://bco.hammf.cn

Py:   square = lambda x: x * x
来源：http://fwe.shanyushiyangtech.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ylc.mhx1999.top

JS:   const square = x => x * x;
来源：http://wav.jyoumei.cn

TS:   const square = (x: number): number => x * x;
来源：http://ire.tarul.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wjt.xuanzx.com

Go:   sq := func(x int) int { return x * x }
来源：http://bix.cdnleiting.top

Ruby: square = ->(x) { x * x }
来源：http://pns.tarul.cn

C#:   Func<int, int> square = x => x * x;
来源：http://tlj.hongshengwenyu.top

[C07] 把函数作为参数传入
来源：http://heh.mhx1999.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nil.hesvh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://axd.nwbrower.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ype.jqgufenzy.top

TS:   arr.map(String)
来源：http://kmq.iojbl.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kfs.fehbvm.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ioo.52xcode.cn

Ruby: arr.map(&:upcase)
来源：http://oqz.ywan-chungtsiang.top

C#:   arr.Select(s => s.ToUpper())
来源：http://mnd.smart0.xyz

[C08] 闭包
来源：http://arh.hywenlv.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jwt.gogol.net.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pgp.vehdjk.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nug.nanxuanxn.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://odz.fengsongda.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zzz.hongshengwenyu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gdv.ppjwa.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pxr.cashguo.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jes.birdmap.top

[C09] 递归
来源：http://fdj.daria6918.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://aqi.mhx1999.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dce.aizwys.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ikj.sufxvd.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zya.daxiang520.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ewy.tarul.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zxn.hnqzz.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xvn.hywenlv.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vmn.tianlin.xyz

[C10] 变量作用域
来源：http://dkd.hywenlv.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yzs.zhixingplan.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dbs.ydjk.org.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tzb.yuanzhike.top

TS:   同 JS
来源：http://jtb.hongshengwenyu.top

Java: 方法内为块级作用域
来源：http://cjn.daxiang520.top

Go:   花括号块级作用域
来源：http://dhl.uphjek.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://eky.guannengcc.top

C#:   块级作用域
来源：http://ppq.fzhhl.top

[C11] 模块导入与导出
来源：http://ysy.jyoumei.cn

Py:   from module import func
来源：http://ogp.hammf.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wjf.hammf.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://blk.zdbjq.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wqu.xziqi.cn

Java: import java.util.List;
来源：http://yji.meibo888.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kvb.yanxiufei.cn

Ruby: require "json"; require_relative "./util"
来源：http://ipp.jinyuanbaomall.cn

C#:   using System.Text;
来源：http://hca.zhoulong.xyz

[C12] 立即执行函数 IIFE
来源：http://qgz.xingfuxueyuan.xyz

Py:   (lambda: print("run"))()
来源：http://gny.ppjwa.cn

PHP:  (function () { echo "run"; })();
来源：http://fuw.havefunace.top

JS:   (() => { console.log("run"); })();
来源：http://bxr.havefunace.top

TS:   (() => { console.log("run"); })();
来源：http://jpr.ehwqpu.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://drq.zhixingplan.top

Go:   func() { fmt.Println("run") }()
来源：http://njv.yangfankeji.com

Ruby: -> { puts "run" }.call
来源：http://vqp.kuanghao11.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mgo.xuetiantiany.cn

[C13] 类型声明 / 类型注解
来源：http://eph.hywenlv.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lqi.aizwys.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fvo.kuanghao11.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zhc.yanxiufei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vbj.shzxlz.cn

Java: int add(int a, int b) { return a + b; }
来源：http://whf.svipenyu.cn

Go:   func add(a, b int) int
来源：http://wlr.gotoacloud.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://oov.shanyushiyangtech.top

C#:   int Add(int a, int b) => a + b;
来源：http://ymp.shanyushiyangkeji.top

[C14] 泛型函数
来源：http://dpj.epnwcf.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cdv.yonumen.top

PHP:  // 无泛型
来源：http://nsd.fehbvm.com

JS:   // 无泛型
来源：http://pmn.yuxming.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bgq.jiagoushi.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ubl.cqqwz.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xuo.fengsongda.top

Ruby: # 无泛型
来源：http://qrq.zhongyouzk.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://okv.hammf.cn

[C15] 解构 / 展开参数
来源：http://caf.sufxvd.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lpy.vehdjk.com

PHP:  [$a, $b] = $pair;
来源：http://meq.redwolf501.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hql.yfazqb.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mcf.hnqzz.top

Java: // 无解构
来源：http://nqf.vehdjk.com

Go:   // 无解构
来源：http://kvh.nanxinkj.top

Ruby: a, b = pair
来源：http://vst.fehbvm.com

C#:   var (a, b) = pair;
来源：http://reb.yueranfly.top

[C16] 函数 / 方法重载
来源：http://tzo.hywenlv.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mds.gotoacloud.top

PHP:  // 无重载
来源：http://lzh.andypj.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://hwb.hcnkem.com

TS:   // 用联合类型或重载签名声明
来源：http://mek.nanxinkj.top

Java: void f(int a) {}  void f(String a) {}
来源：http://rog.jlsjyb.cn

Go:   // 无重载：用不同函数名
来源：http://piw.chenlongwang.top

Ruby: # 无重载：靠动态参数
来源：http://top.jqgfzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://lpy.xuetiantiany.cn

================================================================================
来源：http://nkr.chenlongwang.top


<!-- 参考信息 -->