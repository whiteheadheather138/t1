代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://sky.c1oappe.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ugl.cucudq.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wfs.zhaomingkeji.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://eci.cucudq.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yoy.hfpthk.cn

================================================================================
来源：http://pkk.dashuyun.cn

B. 流程控制
来源：http://woc.yj20258888.top

================================================================================
来源：http://vsg.zhoulong.xyz

[B01] 条件判断 if / else
来源：http://zrt.52xcode.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://goo.xylfe.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://itb.jianghu66.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cpt.jinghuilouyu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dfb.9152youxi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://asu.cqqwz.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tux.yueranfly.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pyv.daria6918.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://srz.guannengcc.top

[B02] 多分支 else if / elif
来源：http://wyn.xziqi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yit.guannengcc.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sds.jiagoushi.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cej.zhijiandao.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qve.ctjpmb.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aqn.hcnkem.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bwo.ydjk.org.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jwz.ehwqpu.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bms.jlsjyb.cn

[B03] switch / match / case
来源：http://cck.cqqwz.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kay.guannengcc.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xjz.jqgfzy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jqw.gzhubu.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yob.sxryk.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://amw.xuetiantiany.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rzm.hysaishi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fpz.zhixingplan.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qlx.birdmap.top

[B04] for 计数循环
来源：http://wmf.ivvv.top

Py:   for i in range(10): print(i)
来源：http://ezm.epnwcf.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tlo.cashguo.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://erf.ctjpmb.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qyv.jiagoushi.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wzw.ydjk.org.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hvh.sxryk.cn

Ruby: 10.times { |i| puts i }
来源：http://duw.shangyingyoupin.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ztt.guowangkeji.top

[B05] 遍历数组 / 列表
来源：http://lib.wangdashe.top

Py:   for item in arr: print(item)
来源：http://jbc.nanxuanxn.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zus.fanxiaobao.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://csw.hnqzz.top

TS:   for (const item of arr) { console.log(item); }
来源：http://gsz.bjfxy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://icb.zhaomingkeji.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ycq.yj20258888.top

Ruby: arr.each { |item| puts item }
来源：http://lvx.9152youxi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qif.hongshengwenyu.top

[B06] 遍历字典 / 对象
来源：http://tys.jinyuanbaomall.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fee.wangshuangyany.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vwf.c1oappe.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fml.nanxinkj.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vfh.cashguo.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://iit.tanke756.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://iru.bjfxy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ced.meibo888.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hzk.0kj1m.cn

[B07] while 循环
来源：http://wpr.wangdashe.top

Py:   while i < 10: i += 1
来源：http://tuq.bbcook.cn

PHP:  while ($i < 10) { $i++; }
来源：http://pxq.jinghuilouyu.cn

JS:   while (i < 10) { i++; }
来源：http://nyu.yj202588.top

TS:   while (i < 10) { i++; }
来源：http://vej.fktsv.cn

Java: while (i < 10) { i++; }
来源：http://zkw.sjlbkw.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pgz.cqqwz.cn

Ruby: while i < 10; i += 1; end
来源：http://jqd.zhongyouzk.top

C#:   while (i < 10) { i++; }
来源：http://pni.nanxuanxn.top

[B08] do-while（至少执行一次）
来源：http://ikf.cashguo.top

Py:   # 无 do-while：用 while True + break
来源：http://spc.yonumen.top

PHP:  do { $i++; } while ($i < 10);
来源：http://hcx.hywenlv.cn

JS:   do { i++; } while (i < 10);
来源：http://dag.yonumen.top

TS:   do { i++; } while (i < 10);
来源：http://wfx.pengpengdd.cyou

Java: do { i++; } while (i < 10);
来源：http://hsh.zhengqikj.top

Go:   for { i++; if i >= 10 { break } }
来源：http://oty.yueranfly.top

Ruby: begin; i += 1; end while i < 10
来源：http://mtb.zhaomingkeji.xyz

C#:   do { i++; } while (i < 10);
来源：http://qes.chenlongwang.top

[B09] break 与 continue
来源：http://atg.zhongyouzk.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ojm.tarul.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nft.xuetiantiany.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://akh.gogol.net.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ixa.yanxiufei.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://byd.0kj1m.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jwb.shanyushiyangtech.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sns.yj202588.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hfj.yongpay.top

[B10] 遍历同时拿索引
来源：http://agc.cqqwz.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lzk.zhijiandao.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bif.yangfankeji.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fvh.dianchejie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bvo.pengpengdd.cyou

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jqn.jinghuilouyu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mde.yangfankeji.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wrs.xylfe.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://agp.shzxlz.cn

[B11] 生成数字序列 / 区间
来源：http://old.zhaomingkeji.xyz

Py:   list(range(0, 10, 2))
来源：http://xut.fanxiaobao.xyz

PHP:  range(0, 10, 2);
来源：http://gom.jinqigufen.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ptg.fktsv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ozt.nanxuanxn.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bqm.epnwcf.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wru.zdqjudy.top

Ruby: (0...10).step(2).to_a
来源：http://iet.xinyue.icu

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mva.zhengqikj.top

[B12] 跳出多层循环
来源：http://gcn.pengpengdd.cyou

Py:   # 无标签跳转：抽成函数用 return
来源：http://nzy.xziqi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://xse.xylfe.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zyi.iojbl.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nhy.cqqwz.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://avs.andypj.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wxt.cqqwz.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kjw.vqdsnc.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://muh.pycfn.com

[B13] 判断是否为数字
来源：http://kwr.kuanghao11.cn

Py:   isinstance(x, (int, float))
来源：http://ziy.sjlbkw.cn

PHP:  is_numeric($x)
来源：http://ysk.yvedp.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qjg.jinyuanbaomall.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kou.yueranfly.top

Java: x instanceof Number
来源：http://gwe.hammf.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qst.xinyue.icu

Ruby: x.is_a?(Numeric)
来源：http://wug.xziqi.cn

C#:   x is int or double or decimal
来源：http://deq.yuanzhike.top

[B14] 判断值是否在集合内
来源：http://jey.ppjwa.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://azk.yuxming.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mbd.ivvv.top

JS:   [1, 2, 3].includes(x)
来源：http://myx.tianlin.xyz

TS:   [1, 2, 3].includes(x)
来源：http://cnt.tanke756.top

Java: List.of(1, 2, 3).contains(x)
来源：http://mht.xingfuxueyuan.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xpt.hfpthk.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xnm.zhengqikj.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tux.sjlbkw.cn

[B15] 布尔运算与取反
来源：http://foe.xingfuxueyuan.xyz

Py:   a and b or not c
来源：http://zgm.sufxvd.cn

PHP:  $a && $b || !$c
来源：http://uto.daxiang520.top

JS:   a && b || !c
来源：http://plv.kuanghao11.cn

TS:   a && b || !c
来源：http://hgl.fanxiaobao.xyz

Java: a && b || !c
来源：http://mtd.zhixingplan.top

Go:   a && b || !c
来源：http://qzn.ydzc1.top

Ruby: a && b || !c
来源：http://pzd.snrcjt.cn

C#:   a && b || !c
来源：http://xcy.haohaochexian.top

[B16] 卫语句：不满足条件提前返回
来源：http://bcm.shzxlz.cn

Py:   if not data: return
来源：http://qtk.zhijiandao.cn

PHP:  if (!$data) { return; }
来源：http://dyl.chenzaomai.com

JS:   if (!data) return;
来源：http://hnd.cqqwz.cn

TS:   if (!data) return;
来源：http://gqw.nwbrower.top

Java: if (data == null) return;
来源：http://yup.hnqzz.top

Go:   if data == nil { return }
来源：http://pyd.birdmap.top

Ruby: return if data.nil?
来源：http://ana.cdnleiting.top

C#:   if (data == null) return;
来源：http://mpp.sufxvd.cn

================================================================================
来源：http://evl.yj202588.top

C. 函数与作用域
来源：http://oyz.shangyingyoupin.top

================================================================================
来源：http://qza.hfpthk.cn

[C01] 定义函数
来源：http://ehw.sjlbkw.cn

Py:   def add(a, b): return a + b
来源：http://seg.vehdjk.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fid.jlsjyb.cn

JS:   function add(a, b) { return a + b; }
来源：http://vlu.ehwqpu.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://knu.ydjk.org.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://evr.wangshuangyany.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ykk.jinqigfzy.top

Ruby: def add(a, b); a + b; end
来源：http://pls.smart0.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wkx.jiagoushi.top

[C02] 默认参数
来源：http://ayz.cdnleiting.top

Py:   def greet(name="World"): return name
来源：http://tkg.hongshengwenyu.top

PHP:  function greet($name = "World") { return $name; }
来源：http://utc.0kj1m.cn

JS:   function greet(name = "World") { return name; }
来源：http://ziz.daxiang520.top

TS:   function greet(name: string = "World") { return name; }
来源：http://iua.tianlin.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://ufb.yanxiufei.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bbi.quarkkingdee.top

Ruby: def greet(name = "World") = name
来源：http://yut.yonumen.top

C#:   string Greet(string name = "World") => name;
来源：http://bof.xylfe.cn

[C03] 可变参数
来源：http://bwy.fktsv.cn

Py:   def total(*args): return sum(args)
来源：http://bzg.hesvh.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zns.yongpay.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xdl.havefunace.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hlm.jinqigufen.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lam.tarul.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://oxq.yonumen.top

Ruby: def total(*nums); nums.sum; end
来源：http://zdz.jqgufenzy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zru.redwolf501.top

[C04] 命名参数 / 关键字参数
来源：http://ctc.nanxinkj.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jmk.jiagoushi.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xij.uphjek.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lpe.svipenyu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xzy.vqdsnc.cn

Java: // 无：用 Builder 模式或 record
来源：http://wbn.xuanzx.com

Go:   // 无：用配置结构体参数
来源：http://gvl.haohaochexian.top

Ruby: f(a: 1, b: 2)
来源：http://rkj.xingfuxueyuan.xyz

C#:   f(a: 1, b: 2)
来源：http://suq.yangfankeji.com

[C05] 返回多个值
来源：http://zin.ivvv.top

Py:   return a, b
来源：http://avw.c1oappe.top

PHP:  return [$a, $b];
来源：http://dlj.gaohongyu789.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://vrk.feifeiyinyue.top

TS:   return { a, b };
来源：http://nir.kuanghao11.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ghw.yanxiufei.cn

Go:   return a, b
来源：http://wly.dashuyun.cn

Ruby: return a, b
来源：http://sje.meibo888.top

C#:   return (a, b);              // ValueTuple
来源：http://eau.zhaomingkeji.xyz

[C06] 匿名函数 / lambda
来源：http://dyq.ybcxt.top

Py:   square = lambda x: x * x
来源：http://mni.ehwqpu.com

PHP:  $square = fn($x) => $x * $x;
来源：http://bhu.ppjwa.cn

JS:   const square = x => x * x;
来源：http://zaw.yueranfly.top

TS:   const square = (x: number): number => x * x;
来源：http://dix.gotoacloud.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bsp.andypj.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://qur.yanxiufei.cn

Ruby: square = ->(x) { x * x }
来源：http://fes.jianghu66.top

C#:   Func<int, int> square = x => x * x;
来源：http://nvl.zycfv.cn

[C07] 把函数作为参数传入
来源：http://ulv.jqgfzy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://aqq.vqdsnc.cn

PHP:  array_map("strtoupper", $arr);
来源：http://smt.dashuyun.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wqb.smart0.xyz

TS:   arr.map(String)
来源：http://ukh.yueranfly.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bre.yongpay.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://efr.hesvh.cn

Ruby: arr.map(&:upcase)
来源：http://efe.52xcode.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pgb.sjlbkw.cn

[C08] 闭包
来源：http://nmj.kuanghao11.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ghc.sweek.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nea.sxryk.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://azf.cdnleiting.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rwn.ivvv.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uci.52xcode.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lbz.shanyushiyangtech.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://upv.wangdashe.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rkb.jianghu66.top

[C09] 递归
来源：http://vgz.epnwcf.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jtg.ctjpmb.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ity.cucudq.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lme.daria6918.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://umv.hysaishi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dsh.snrcjt.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://asv.hammf.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mbu.yuxming.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://diz.jiagoushi.top

[C10] 变量作用域
来源：http://okj.uphjek.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fjz.shangyingyoupin.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lma.haohaochexian.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fgq.feifeiyinyue.top

TS:   同 JS
来源：http://fou.cdnleiting.top

Java: 方法内为块级作用域
来源：http://eci.zhongyouzk.top

Go:   花括号块级作用域
来源：http://uxg.meibo888.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mqe.nwbrower.top

C#:   块级作用域
来源：http://uli.9152youxi.cn

[C11] 模块导入与导出
来源：http://ksu.haohaochexian.top

Py:   from module import func
来源：http://ert.shanyushiyangtech.top

PHP:  require "file.php";  或 use App\Service;
来源：http://fny.haohaochexian.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://doh.shangyingyoupin.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fla.cdnleiting.top

Java: import java.util.List;
来源：http://hvj.ydzc1.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hjo.yfazqb.com

Ruby: require "json"; require_relative "./util"
来源：http://mjq.fengsongda.top

C#:   using System.Text;
来源：http://vrm.yj20258888.top

[C12] 立即执行函数 IIFE
来源：http://njv.cucudq.cn

Py:   (lambda: print("run"))()
来源：http://thb.c1oappe.top

PHP:  (function () { echo "run"; })();
来源：http://gah.yj20258.top

JS:   (() => { console.log("run"); })();
来源：http://vww.hnqzz.top

TS:   (() => { console.log("run"); })();
来源：http://xmr.jqgfzy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xey.ydzc1.top

Go:   func() { fmt.Println("run") }()
来源：http://jgu.nanxuanxn.top

Ruby: -> { puts "run" }.call
来源：http://yya.nwbrower.top

C#:   // 无 IIFE：用静态构造函数
来源：http://krm.shangyingyoupin.top

[C13] 类型声明 / 类型注解
来源：http://udx.sysykeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kac.xylfe.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qys.hnxiangtu.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yup.feifeiyinyue.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cqu.316326.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://xae.smart0.xyz

Go:   func add(a, b int) int
来源：http://lum.gotoacloud.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kyf.hongshengwenyu.top

C#:   int Add(int a, int b) => a + b;
来源：http://igk.kuanghao11.cn

[C14] 泛型函数
来源：http://wzj.xuetiantiany.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hks.fehbvm.com

PHP:  // 无泛型
来源：http://ebe.sxryk.cn

JS:   // 无泛型
来源：http://txx.yangfankeji.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yip.wangshuangyany.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jam.hammf.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ecc.tanke756.top

Ruby: # 无泛型
来源：http://sls.sweek.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ikm.nanxuanxn.top

[C15] 解构 / 展开参数
来源：http://tcj.zhixingplan.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xnf.shanyushiyangtech.top

PHP:  [$a, $b] = $pair;
来源：http://ztp.wangshuangyany.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qrq.vehdjk.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kxs.316326.xyz

Java: // 无解构
来源：http://tqg.sufxvd.cn

Go:   // 无解构
来源：http://xjr.jyoumei.cn

Ruby: a, b = pair
来源：http://zgk.fktsv.cn

C#:   var (a, b) = pair;
来源：http://qly.xylfe.cn

[C16] 函数 / 方法重载
来源：http://jqm.jinqigufen.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qom.hongshengwenyu.top

PHP:  // 无重载
来源：http://gkt.fzhhl.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://agh.yonumen.top

TS:   // 用联合类型或重载签名声明
来源：http://drp.sxryk.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://cum.gaohongyu789.top

Go:   // 无重载：用不同函数名
来源：http://vgn.yvedp.cn

Ruby: # 无重载：靠动态参数
来源：http://epj.yuxming.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://jph.zycfv.cn

================================================================================
来源：http://zck.0kj1m.cn


<!-- 参考信息 -->