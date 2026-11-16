代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://ftd.vqdsnc.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xws.gzhubu.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gsb.ybcxt.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://tkb.zhaomingkeji.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yla.9152youxi.cn

================================================================================
来源：http://dgz.bjfxy.top

B. 流程控制
来源：http://yis.ctjpmb.com

================================================================================
来源：http://prn.hnxiangtu.top

[B01] 条件判断 if / else
来源：http://vtn.hesvh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://unn.c1oappe.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wtp.kuanghao11.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kpv.ppjwa.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ntq.fehbvm.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://dph.jiagoushi.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dmo.yuanzhike.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fyu.jinqigfzy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dke.ybcxt.top

[B02] 多分支 else if / elif
来源：http://nzn.tianlin.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://oux.ehwqpu.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vuo.hnqzz.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bvs.shangyingyoupin.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kdc.jinghuilouyu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://agk.daria6918.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dor.jinqigfzy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://otn.0kj1m.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ygu.jinghuilouyu.cn

[B03] switch / match / case
来源：http://lth.cucudq.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mgu.xziqi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wcu.epnwcf.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cpy.zhaomingkeji.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vwh.aibaodan.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tmw.kuanghao11.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gsc.wangshuangyany.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://est.guowangkeji.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zip.tarul.cn

[B04] for 计数循环
来源：http://nvl.jqgufenzy.top

Py:   for i in range(10): print(i)
来源：http://ogb.sysykeji.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://flp.uphjek.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ncp.yueranfly.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mzb.pengpengdd.cyou

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rdd.mhx1999.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bss.xuetiantiany.cn

Ruby: 10.times { |i| puts i }
来源：http://efh.vehdjk.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ojr.mhx1999.top

[B05] 遍历数组 / 列表
来源：http://wew.jianghu66.top

Py:   for item in arr: print(item)
来源：http://nwv.shangyingyoupin.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://smw.tian-w.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://xql.kuanghao11.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fsg.jinqigfzy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://kab.shangyingyoupin.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vvr.pycfn.com

Ruby: arr.each { |item| puts item }
来源：http://zeh.wangdashe.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://oqj.sufxvd.cn

[B06] 遍历字典 / 对象
来源：http://vek.ivvv.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ycb.c1oappe.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://izj.meibo888.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blf.yanxiufei.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://doa.guannengcc.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pcz.hfpthk.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://opt.hnqzz.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bef.iojbl.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://guf.gzhubu.top

[B07] while 循环
来源：http://ftr.zdbjq.cn

Py:   while i < 10: i += 1
来源：http://uen.xylfe.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lof.pycfn.com

JS:   while (i < 10) { i++; }
来源：http://axp.dashuyun.cn

TS:   while (i < 10) { i++; }
来源：http://mel.jiagoushi.top

Java: while (i < 10) { i++; }
来源：http://pmi.yuanzhike.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kjl.sxryk.cn

Ruby: while i < 10; i += 1; end
来源：http://kdg.vqdsnc.cn

C#:   while (i < 10) { i++; }
来源：http://wma.xinyue.icu

[B08] do-while（至少执行一次）
来源：http://voo.zycfv.cn

Py:   # 无 do-while：用 while True + break
来源：http://bxo.guannengcc.top

PHP:  do { $i++; } while ($i < 10);
来源：http://jzz.zhengqikj.top

JS:   do { i++; } while (i < 10);
来源：http://lyl.jlsjyb.cn

TS:   do { i++; } while (i < 10);
来源：http://ayw.guowangkeji.top

Java: do { i++; } while (i < 10);
来源：http://jsb.andypj.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://jcz.yanxiufei.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rsa.yuxming.cn

C#:   do { i++; } while (i < 10);
来源：http://thz.ywan-chungtsiang.top

[B09] break 与 continue
来源：http://mha.cashguo.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xnl.cucudq.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bce.yfazqb.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://syz.mhx1999.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kxf.hnqzz.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fnc.guowangkeji.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ohi.feifeiyinyue.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://log.jqgufenzy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bem.vehdjk.com

[B10] 遍历同时拿索引
来源：http://zpb.hongshengwenyu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ubm.epnwcf.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lla.shangyingyoupin.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wwa.jiagoushi.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mhc.fengsongda.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rbb.quarkkingdee.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jrb.zhengqikj.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dxt.chenlongwang.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wsf.ivvv.top

[B11] 生成数字序列 / 区间
来源：http://aes.fanxiaobao.xyz

Py:   list(range(0, 10, 2))
来源：http://xhp.jyoumei.cn

PHP:  range(0, 10, 2);
来源：http://xyx.yj202588.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://whb.iojbl.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://urs.jqgfzy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://iai.ivvv.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pum.feifeiyinyue.top

Ruby: (0...10).step(2).to_a
来源：http://fgg.kuanghao11.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nxp.xylfe.cn

[B12] 跳出多层循环
来源：http://zow.xuanzx.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://xdc.hcnkem.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://hgl.jqgufenzy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kzy.yanxiufei.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cpz.sxryk.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://slb.yueranfly.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yue.epnwcf.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ryu.ybcxt.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vnd.sufxvd.cn

[B13] 判断是否为数字
来源：http://qvu.redwolf501.top

Py:   isinstance(x, (int, float))
来源：http://rnm.cucudq.cn

PHP:  is_numeric($x)
来源：http://hih.chenjidiqi.icu

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ble.guowangkeji.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kbe.zdqjudy.top

Java: x instanceof Number
来源：http://hrj.shuidangran.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://iqt.sxryk.cn

Ruby: x.is_a?(Numeric)
来源：http://vix.fanxiaobao.xyz

C#:   x is int or double or decimal
来源：http://zuk.nanxuanxn.top

[B14] 判断值是否在集合内
来源：http://qbv.yj20258.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hxx.ybcxt.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ngr.zhiwuduotai.top

JS:   [1, 2, 3].includes(x)
来源：http://sbo.hongshengwenyu.top

TS:   [1, 2, 3].includes(x)
来源：http://pvx.yuxming.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://eac.tarul.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qhq.gzhubu.top

Ruby: [1, 2, 3].include?(x)
来源：http://lsk.dianchejie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dny.zhongyouzk.top

[B15] 布尔运算与取反
来源：http://ior.cashguo.top

Py:   a and b or not c
来源：http://unb.havefunace.top

PHP:  $a && $b || !$c
来源：http://khn.hesvh.cn

JS:   a && b || !c
来源：http://sjp.havefunace.top

TS:   a && b || !c
来源：http://wbx.c1oappe.top

Java: a && b || !c
来源：http://hbd.bbcook.cn

Go:   a && b || !c
来源：http://pnd.vqdsnc.cn

Ruby: a && b || !c
来源：http://xdn.shanyushiyangtech.top

C#:   a && b || !c
来源：http://wyp.tian-w.cn

[B16] 卫语句：不满足条件提前返回
来源：http://nrd.jqgfzy.top

Py:   if not data: return
来源：http://rwf.vehdjk.com

PHP:  if (!$data) { return; }
来源：http://rhf.hongshengwenyu.top

JS:   if (!data) return;
来源：http://vdv.havefunace.top

TS:   if (!data) return;
来源：http://awl.hongshengwenyu.top

Java: if (data == null) return;
来源：http://mqz.cashguo.top

Go:   if data == nil { return }
来源：http://yar.havefunace.top

Ruby: return if data.nil?
来源：http://ztp.c1oappe.top

C#:   if (data == null) return;
来源：http://jhf.yangfankeji.com

================================================================================
来源：http://erj.yuanzhike.top

C. 函数与作用域
来源：http://vmm.zdqjudy.top

================================================================================
来源：http://ubs.hammf.cn

[C01] 定义函数
来源：http://kaf.yanxiufei.cn

Py:   def add(a, b): return a + b
来源：http://sbs.zhaomingkeji.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uqg.yonumen.top

JS:   function add(a, b) { return a + b; }
来源：http://pmv.cucudq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nnx.gotoacloud.top

Java: static int add(int a, int b) { return a + b; }
来源：http://pxu.ppjwa.cn

Go:   func add(a, b int) int { return a + b }
来源：http://tml.bjfxy.top

Ruby: def add(a, b); a + b; end
来源：http://gad.tanke756.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lkg.birdmap.top

[C02] 默认参数
来源：http://apb.mhx1999.top

Py:   def greet(name="World"): return name
来源：http://ofl.jqgfzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://htz.tian-w.cn

JS:   function greet(name = "World") { return name; }
来源：http://sgh.hongshengwenyu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://cxf.ywan-chungtsiang.top

Java: // 无默认参数：方法重载或 Optional
来源：http://def.hesvh.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qra.jlsjyb.cn

Ruby: def greet(name = "World") = name
来源：http://gvf.ydzc1.top

C#:   string Greet(string name = "World") => name;
来源：http://gav.yueranfly.top

[C03] 可变参数
来源：http://dda.tanke756.top

Py:   def total(*args): return sum(args)
来源：http://ffe.9152youxi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jxy.gotoacloud.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://chd.9152youxi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://apz.iojbl.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kcw.smart0.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qgx.aizwys.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vix.zhijiandao.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cux.shanyushiyangtech.top

[C04] 命名参数 / 关键字参数
来源：http://vvh.yueranfly.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://axo.fktsv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hbx.zhiwuduotai.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://izw.zhoulong.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://for.fehbvm.com

Java: // 无：用 Builder 模式或 record
来源：http://jzm.cqqwz.cn

Go:   // 无：用配置结构体参数
来源：http://lum.zhaomingkeji.xyz

Ruby: f(a: 1, b: 2)
来源：http://zpd.tian-w.cn

C#:   f(a: 1, b: 2)
来源：http://oke.quarkkingdee.top

[C05] 返回多个值
来源：http://all.gogol.net.cn

Py:   return a, b
来源：http://ajy.vqdsnc.cn

PHP:  return [$a, $b];
来源：http://kyc.316326.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://ocr.guowangkeji.top

TS:   return { a, b };
来源：http://cto.jqgfzy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://stv.bbcook.cn

Go:   return a, b
来源：http://yek.zhoulong.xyz

Ruby: return a, b
来源：http://uwz.tianlin.xyz

C#:   return (a, b);              // ValueTuple
来源：http://mwd.yuanzhike.top

[C06] 匿名函数 / lambda
来源：http://gbb.zdqjudy.top

Py:   square = lambda x: x * x
来源：http://her.zhongyouzk.top

PHP:  $square = fn($x) => $x * $x;
来源：http://hfa.guannengcc.top

JS:   const square = x => x * x;
来源：http://dky.zhixingplan.top

TS:   const square = (x: number): number => x * x;
来源：http://stm.shanyushiyangtech.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ows.hnxiangtu.top

Go:   sq := func(x int) int { return x * x }
来源：http://fqa.nanxuanxn.top

Ruby: square = ->(x) { x * x }
来源：http://ebl.hysaishi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://als.zycfv.cn

[C07] 把函数作为参数传入
来源：http://yom.xuanzx.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rme.jianghu66.top

PHP:  array_map("strtoupper", $arr);
来源：http://qog.redwolf501.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yqv.redwolf501.top

TS:   arr.map(String)
来源：http://njv.jinqigufen.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ruo.yueranfly.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jac.shzxlz.cn

Ruby: arr.map(&:upcase)
来源：http://zwv.jyoumei.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://flt.snrcjt.cn

[C08] 闭包
来源：http://pde.cashguo.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xze.cdnleiting.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vne.jinyuanbaomall.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dkh.jlsjyb.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://flx.ydzc1.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mdt.jqgufenzy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vor.cucudq.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sor.ydzc1.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://own.guannengcc.top

[C09] 递归
来源：http://wng.shuidangran.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zcv.nwbrower.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://avc.jinghuilouyu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bbp.hnqzz.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wum.sjlbkw.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bii.yvedp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://unn.snrcjt.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rdw.chenlongwang.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sxr.aibaodan.cn

[C10] 变量作用域
来源：http://gxh.sxryk.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kvn.9152youxi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://aik.ivvv.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kes.yj20258.top

TS:   同 JS
来源：http://vlm.uphjek.com

Java: 方法内为块级作用域
来源：http://rpg.shanyushiyangkeji.top

Go:   花括号块级作用域
来源：http://krx.ctjpmb.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vde.hongshengwenyu.top

C#:   块级作用域
来源：http://ydi.9152youxi.cn

[C11] 模块导入与导出
来源：http://cyb.dianchejie.cn

Py:   from module import func
来源：http://fer.uphjek.com

PHP:  require "file.php";  或 use App\Service;
来源：http://usm.xuetiantiany.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wof.ywan-chungtsiang.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fnz.yvedp.cn

Java: import java.util.List;
来源：http://cpu.ydzc1.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sjn.xziqi.cn

Ruby: require "json"; require_relative "./util"
来源：http://voz.xylfe.cn

C#:   using System.Text;
来源：http://cjj.sysykeji.top

[C12] 立即执行函数 IIFE
来源：http://hpm.meibo888.top

Py:   (lambda: print("run"))()
来源：http://ozz.shzxlz.cn

PHP:  (function () { echo "run"; })();
来源：http://sra.shzxlz.cn

JS:   (() => { console.log("run"); })();
来源：http://vhp.xuanzx.com

TS:   (() => { console.log("run"); })();
来源：http://xln.sjlbkw.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yqv.zycfv.cn

Go:   func() { fmt.Println("run") }()
来源：http://qed.xylfe.cn

Ruby: -> { puts "run" }.call
来源：http://tti.hcnkem.com

C#:   // 无 IIFE：用静态构造函数
来源：http://uuz.ehwqpu.com

[C13] 类型声明 / 类型注解
来源：http://vtt.ppjwa.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://enp.zycfv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ofv.cucudq.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://chi.wangshuangyany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uvk.smart0.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://kqx.yj202588.top

Go:   func add(a, b int) int
来源：http://fpv.yuxming.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ake.jianghu66.top

C#:   int Add(int a, int b) => a + b;
来源：http://xxp.gaohongyu789.top

[C14] 泛型函数
来源：http://xvd.fengsongda.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bbp.zhengqikj.top

PHP:  // 无泛型
来源：http://eyp.zycfv.cn

JS:   // 无泛型
来源：http://xlk.yj20258.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qyu.haohaochexian.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xmy.wangshuangyany.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fcf.jqgufenzy.top

Ruby: # 无泛型
来源：http://wsu.ybcxt.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dcb.ehwqpu.com

[C15] 解构 / 展开参数
来源：http://bpd.nwbrower.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://luf.xylfe.cn

PHP:  [$a, $b] = $pair;
来源：http://uyx.chenzaomai.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qqv.zycfv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jhf.zhijiandao.cn

Java: // 无解构
来源：http://qzk.wangdashe.top

Go:   // 无解构
来源：http://fww.yvedp.cn

Ruby: a, b = pair
来源：http://shf.guowangkeji.top

C#:   var (a, b) = pair;
来源：http://cvz.hnxiangtu.top

[C16] 函数 / 方法重载
来源：http://ovi.sysykeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wog.xingfuxueyuan.xyz

PHP:  // 无重载
来源：http://fkt.uphjek.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://jsq.yongpay.top

TS:   // 用联合类型或重载签名声明
来源：http://vwb.cqqwz.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://kdi.svipenyu.cn

Go:   // 无重载：用不同函数名
来源：http://ezn.aibaodan.cn

Ruby: # 无重载：靠动态参数
来源：http://ymt.cheryme.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://slo.zhaomingkeji.xyz

================================================================================
来源：http://igp.9152youxi.cn


<!-- 参考信息 -->