代发 wailian999

[B01] 条件判断 if / else
来源：http://xrm.ydzc1.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ugf.ywan-chungtsiang.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fgz.zycfv.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qxu.cucudq.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hqe.hywenlv.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://gmh.52xcode.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cod.dianchejie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qie.yj20258.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jlc.hongshengwenyu.top

[B02] 多分支 else if / elif
来源：http://hnm.yj202588.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bum.sweek.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://oic.yuanzhike.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fwn.haohaochexian.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zxt.smart0.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rao.zhiwuduotai.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://twf.xziqi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://azk.c1oappe.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vxb.316326.xyz

[B03] switch / match / case
来源：http://olx.yanxiufei.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gba.fktsv.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fgp.fehbvm.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ato.gaohongyu789.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cje.jqgfzy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://grk.yj20258888.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hoi.feifeiyinyue.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xzy.fehbvm.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dmb.xziqi.cn

[B04] for 计数循环
来源：http://rsh.daria6918.cn

Py:   for i in range(10): print(i)
来源：http://ruk.smart0.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ccr.wangshuangyany.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uyq.guowangkeji.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gsd.birdmap.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vgz.sufxvd.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lfe.vqdsnc.cn

Ruby: 10.times { |i| puts i }
来源：http://ukq.ehwqpu.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ojh.feifeiyinyue.top

[B05] 遍历数组 / 列表
来源：http://zyn.quarkkingdee.top

Py:   for item in arr: print(item)
来源：http://nab.vqdsnc.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hsl.yueranfly.top

JS:   for (const item of arr) { console.log(item); }
来源：http://xap.yj202588.top

TS:   for (const item of arr) { console.log(item); }
来源：http://zzp.guowangkeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://yle.shanyushiyangtech.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ryy.gogol.net.cn

Ruby: arr.each { |item| puts item }
来源：http://lgt.smart0.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hdl.hnqzz.top

[B06] 遍历字典 / 对象
来源：http://jks.tarul.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://wng.jinyuanbaomall.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rfq.zhongyouzk.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iec.bjfxy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ehf.gogol.net.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://loi.ydzc1.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gby.haohaochexian.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://row.svipenyu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dxn.nanxuanxn.top

[B07] while 循环
来源：http://uxo.nanxuanxn.top

Py:   while i < 10: i += 1
来源：http://cim.jlsjyb.cn

PHP:  while ($i < 10) { $i++; }
来源：http://sym.yueranfly.top

JS:   while (i < 10) { i++; }
来源：http://cjk.jinqigufen.top

TS:   while (i < 10) { i++; }
来源：http://hbe.xingfuxueyuan.xyz

Java: while (i < 10) { i++; }
来源：http://eea.bjfxy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vdw.bjfxy.top

Ruby: while i < 10; i += 1; end
来源：http://fxr.hammf.cn

C#:   while (i < 10) { i++; }
来源：http://odp.ehwqpu.com

[B08] do-while（至少执行一次）
来源：http://vhv.hcnkem.com

Py:   # 无 do-while：用 while True + break
来源：http://eye.xuetiantiany.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://dea.cashguo.top

JS:   do { i++; } while (i < 10);
来源：http://fya.gaohongyu789.top

TS:   do { i++; } while (i < 10);
来源：http://kfv.xylfe.cn

Java: do { i++; } while (i < 10);
来源：http://nxd.hammf.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fsf.shuidangran.top

Ruby: begin; i += 1; end while i < 10
来源：http://pnv.zycfv.cn

C#:   do { i++; } while (i < 10);
来源：http://vhq.yfazqb.com

[B09] break 与 continue
来源：http://pco.sweek.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zya.316326.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ntq.tarul.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://akx.pengpengdd.cyou

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kyh.zhaomingkeji.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xcn.xuetiantiany.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vvo.jinqigufen.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://azx.zdbjq.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wyl.uphjek.com

[B10] 遍历同时拿索引
来源：http://moi.cqqwz.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://orm.zhiwuduotai.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://axt.kuanghao11.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://max.zdbjq.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mfs.hesvh.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://egx.pengpengdd.cyou

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xkz.bjfxy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ckv.xziqi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bhc.dashuyun.cn

[B11] 生成数字序列 / 区间
来源：http://jwe.cheryme.top

Py:   list(range(0, 10, 2))
来源：http://uvp.bbcook.cn

PHP:  range(0, 10, 2);
来源：http://vok.aizwys.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ewj.ppjwa.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ssu.shangyingyoupin.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mdd.tarul.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tqj.xingfuxueyuan.xyz

Ruby: (0...10).step(2).to_a
来源：http://rgl.yanxiufei.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://psd.xinyue.icu

[B12] 跳出多层循环
来源：http://eoe.zhixingplan.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://rry.wangdashe.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://fiy.birdmap.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://iju.jlsjyb.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nnw.zhongyouzk.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://aia.cdnleiting.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vyj.zhixingplan.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dfc.shanyushiyangtech.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://acb.0kj1m.cn

[B13] 判断是否为数字
来源：http://uvs.daxiang520.top

Py:   isinstance(x, (int, float))
来源：http://xgs.tanke756.top

PHP:  is_numeric($x)
来源：http://klb.316326.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zym.chenjidiqi.icu

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qxk.bbcook.cn

Java: x instanceof Number
来源：http://zgb.zhaomingkeji.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rxy.birdmap.top

Ruby: x.is_a?(Numeric)
来源：http://oua.aizwys.cn

C#:   x is int or double or decimal
来源：http://cnu.havefunace.top

[B14] 判断值是否在集合内
来源：http://zni.cdnleiting.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gjr.zhiwuduotai.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lpg.c1oappe.top

JS:   [1, 2, 3].includes(x)
来源：http://uzm.yj20258888.top

TS:   [1, 2, 3].includes(x)
来源：http://mlu.havefunace.top

Java: List.of(1, 2, 3).contains(x)
来源：http://uin.hongshengwenyu.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nwj.xinyue.icu

Ruby: [1, 2, 3].include?(x)
来源：http://unb.yuxming.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jjz.shanyushiyangkeji.top

[B15] 布尔运算与取反
来源：http://bsj.fanxiaobao.xyz

Py:   a and b or not c
来源：http://ctc.zhengqikj.top

PHP:  $a && $b || !$c
来源：http://vme.shuidangran.top

JS:   a && b || !c
来源：http://wee.xinyue.icu

TS:   a && b || !c
来源：http://osh.ydzc1.top

Java: a && b || !c
来源：http://kle.xuanzx.com

Go:   a && b || !c
来源：http://jhw.hywenlv.cn

Ruby: a && b || !c
来源：http://zok.hongshengwenyu.top

C#:   a && b || !c
来源：http://frp.9152youxi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://kek.ydzc1.top

Py:   if not data: return
来源：http://qhr.sxryk.cn

PHP:  if (!$data) { return; }
来源：http://osi.vqdsnc.cn

JS:   if (!data) return;
来源：http://rlz.guowangkeji.top

TS:   if (!data) return;
来源：http://vqb.ctjpmb.com

Java: if (data == null) return;
来源：http://nbq.yonumen.top

Go:   if data == nil { return }
来源：http://ymz.cashguo.top

Ruby: return if data.nil?
来源：http://ozw.shzxlz.cn

C#:   if (data == null) return;
来源：http://mhq.shzxlz.cn

================================================================================
来源：http://kic.0kj1m.cn

C. 函数与作用域
来源：http://zap.redwolf501.top

================================================================================
来源：http://fbb.nwbrower.top

[C01] 定义函数
来源：http://jzp.xziqi.cn

Py:   def add(a, b): return a + b
来源：http://kip.zhiwuduotai.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://shn.wangshuangyany.cn

JS:   function add(a, b) { return a + b; }
来源：http://wxw.mhx1999.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lgf.pycfn.com

Java: static int add(int a, int b) { return a + b; }
来源：http://cmq.ctjpmb.com

Go:   func add(a, b int) int { return a + b }
来源：http://ilh.jlsjyb.cn

Ruby: def add(a, b); a + b; end
来源：http://rbq.yangfankeji.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://emo.ehwqpu.com

[C02] 默认参数
来源：http://jdb.redwolf501.top

Py:   def greet(name="World"): return name
来源：http://msc.c1oappe.top

PHP:  function greet($name = "World") { return $name; }
来源：http://zkb.yj202588.top

JS:   function greet(name = "World") { return name; }
来源：http://tff.ehwqpu.com

TS:   function greet(name: string = "World") { return name; }
来源：http://nkq.daxiang520.top

Java: // 无默认参数：方法重载或 Optional
来源：http://xkg.havefunace.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nzi.zdbjq.cn

Ruby: def greet(name = "World") = name
来源：http://xpq.yueranfly.top

C#:   string Greet(string name = "World") => name;
来源：http://uyf.cheryme.top

[C03] 可变参数
来源：http://yuh.chenlongwang.top

Py:   def total(*args): return sum(args)
来源：http://ovo.jlsjyb.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xtu.zhengqikj.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lcr.wangdashe.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cin.kuanghao11.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kcd.andypj.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://inf.jyoumei.cn

Ruby: def total(*nums); nums.sum; end
来源：http://imu.meibo888.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://etn.xuetiantiany.cn

[C04] 命名参数 / 关键字参数
来源：http://pyk.52xcode.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wwg.9152youxi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lpo.zycfv.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://buz.yonumen.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gro.sjlbkw.cn

Java: // 无：用 Builder 模式或 record
来源：http://qmc.havefunace.top

Go:   // 无：用配置结构体参数
来源：http://rdw.jlsjyb.cn

Ruby: f(a: 1, b: 2)
来源：http://egl.guannengcc.top

C#:   f(a: 1, b: 2)
来源：http://dqk.xuetiantiany.cn

[C05] 返回多个值
来源：http://uye.zhixingplan.top

Py:   return a, b
来源：http://mcr.xuetiantiany.cn

PHP:  return [$a, $b];
来源：http://aob.fktsv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://lnk.ivvv.top

TS:   return { a, b };
来源：http://lhq.xylfe.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yrd.hongshengwenyu.top

Go:   return a, b
来源：http://wuv.epnwcf.com

Ruby: return a, b
来源：http://ijc.gogol.net.cn

C#:   return (a, b);              // ValueTuple
来源：http://krl.jyoumei.cn

[C06] 匿名函数 / lambda
来源：http://yjx.jlsjyb.cn

Py:   square = lambda x: x * x
来源：http://vax.ppjwa.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://foy.zycfv.cn

JS:   const square = x => x * x;
来源：http://sjl.sxryk.cn

TS:   const square = (x: number): number => x * x;
来源：http://mdl.jyoumei.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qqx.meibo888.top

Go:   sq := func(x int) int { return x * x }
来源：http://led.shangyingyoupin.top

Ruby: square = ->(x) { x * x }
来源：http://bwk.sweek.top

C#:   Func<int, int> square = x => x * x;
来源：http://ttd.xuetiantiany.cn

[C07] 把函数作为参数传入
来源：http://jkn.9152youxi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dqy.cashguo.top

PHP:  array_map("strtoupper", $arr);
来源：http://ozz.quarkkingdee.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cll.bjfxy.top

TS:   arr.map(String)
来源：http://qst.yongpay.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fdj.yueranfly.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lhb.gotoacloud.top

Ruby: arr.map(&:upcase)
来源：http://zky.xylfe.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://whn.hnxiangtu.top

[C08] 闭包
来源：http://jpy.sjlbkw.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lng.jinqigfzy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uyy.guannengcc.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nkk.jqgufenzy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://msu.guowangkeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lxe.hcnkem.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bxq.guannengcc.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://thg.zhongyouzk.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cpl.epnwcf.com

[C09] 递归
来源：http://bxp.shanyushiyangtech.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fvd.52xcode.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xhj.jianghu66.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yct.cashguo.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ukn.sweek.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tvz.ppjwa.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vog.tianlin.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nfk.yuanzhike.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://npp.hammf.cn

[C10] 变量作用域
来源：http://fyo.jinqigufen.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gmm.hfpthk.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cjw.zhixingplan.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ilm.pengpengdd.cyou

TS:   同 JS
来源：http://qdc.jinghuilouyu.cn

Java: 方法内为块级作用域
来源：http://ken.ehwqpu.com

Go:   花括号块级作用域
来源：http://rjj.yangfankeji.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gen.zdqjudy.top

C#:   块级作用域
来源：http://rlp.yuxming.cn

[C11] 模块导入与导出
来源：http://wqe.andypj.xyz

Py:   from module import func
来源：http://smj.andypj.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://zji.yuxming.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zze.tanke756.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://drn.chenjidiqi.icu

Java: import java.util.List;
来源：http://vat.shangyingyoupin.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://msw.uphjek.com

Ruby: require "json"; require_relative "./util"
来源：http://kdm.9152youxi.cn

C#:   using System.Text;
来源：http://oqs.xuanzx.com

[C12] 立即执行函数 IIFE
来源：http://mwc.jqgufenzy.top

Py:   (lambda: print("run"))()
来源：http://mbx.zhongyouzk.top

PHP:  (function () { echo "run"; })();
来源：http://wlt.andypj.xyz

JS:   (() => { console.log("run"); })();
来源：http://dmv.52xcode.cn

TS:   (() => { console.log("run"); })();
来源：http://sjw.zhiwuduotai.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xvq.hnqzz.top

Go:   func() { fmt.Println("run") }()
来源：http://ruf.vqdsnc.cn

Ruby: -> { puts "run" }.call
来源：http://bgl.xuetiantiany.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jli.cheryme.top

[C13] 类型声明 / 类型注解
来源：http://qov.iojbl.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zuv.zhaomingkeji.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jln.vehdjk.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mng.yfazqb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://awj.zhixingplan.top

Java: int add(int a, int b) { return a + b; }
来源：http://dbu.yj20258888.top

Go:   func add(a, b int) int
来源：http://lwb.ppjwa.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dtq.gogol.net.cn

C#:   int Add(int a, int b) => a + b;
来源：http://jqt.nanxuanxn.top

[C14] 泛型函数
来源：http://hyi.snrcjt.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://buo.jyoumei.cn

PHP:  // 无泛型
来源：http://kbo.yueranfly.top

JS:   // 无泛型
来源：http://yzp.zhiwuduotai.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hre.jiagoushi.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://boh.gaohongyu789.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://eyq.yuanzhike.top

Ruby: # 无泛型
来源：http://jso.vqdsnc.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dtm.iojbl.cn

[C15] 解构 / 展开参数
来源：http://kmj.xylfe.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cpa.fktsv.cn

PHP:  [$a, $b] = $pair;
来源：http://rba.xuetiantiany.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kym.zdbjq.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sgu.gogol.net.cn

Java: // 无解构
来源：http://bzr.hcnkem.com

Go:   // 无解构
来源：http://exc.vqdsnc.cn

Ruby: a, b = pair
来源：http://bqt.ctjpmb.com

C#:   var (a, b) = pair;
来源：http://mpr.cheryme.top

[C16] 函数 / 方法重载
来源：http://ryx.xinyue.icu

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bfx.jinghuilouyu.cn

PHP:  // 无重载
来源：http://zuh.feifeiyinyue.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://blk.shzxlz.cn

TS:   // 用联合类型或重载签名声明
来源：http://qss.yuxming.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://zzc.cashguo.top

Go:   // 无重载：用不同函数名
来源：http://spk.aibaodan.cn

Ruby: # 无重载：靠动态参数
来源：http://qeo.316326.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://ivv.shzxlz.cn

================================================================================
来源：http://eig.wangshuangyany.cn

D. 数组 / 列表 / 集合
来源：http://uey.hcnkem.com

================================================================================
来源：http://yfy.yuanzhike.top

[D01] 创建数组 / 列表
来源：http://wnb.bbcook.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://sul.gotoacloud.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nep.cashguo.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rhb.tanke756.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ufe.c1oappe.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://byy.cqqwz.cn


<!-- 参考信息 -->