代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://upl.yj20258.top

================================================================================
来源：http://hyc.zhijiandao.cn

B. 流程控制
来源：http://bgi.zhaomingkeji.xyz

================================================================================
来源：http://jko.xinyue.icu

[B01] 条件判断 if / else
来源：http://oqd.andypj.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://quw.jinqigufen.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xeg.daria6918.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cbb.ivvv.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kaz.fengsongda.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://hlv.fehbvm.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://oxy.hcnkem.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wii.yvedp.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lwh.316326.xyz

[B02] 多分支 else if / elif
来源：http://kmn.hywenlv.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://uot.ehwqpu.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ayd.birdmap.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yag.ybcxt.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bcn.aibaodan.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nyj.tianlin.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uyf.shanyushiyangtech.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yys.zhaomingkeji.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://evs.vehdjk.com

[B03] switch / match / case
来源：http://fmw.zhijiandao.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pgv.zycfv.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qkk.sufxvd.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mum.pengpengdd.cyou

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jju.c1oappe.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bjh.ydjk.org.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hma.zdqjudy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zkj.vehdjk.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gko.ppjwa.cn

[B04] for 计数循环
来源：http://iph.shzxlz.cn

Py:   for i in range(10): print(i)
来源：http://qku.zycfv.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bdk.zhiwuduotai.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://krd.zhixingplan.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fcg.hfpthk.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nhl.shuidangran.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vbz.daria6918.cn

Ruby: 10.times { |i| puts i }
来源：http://olw.daria6918.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jej.0kj1m.cn

[B05] 遍历数组 / 列表
来源：http://aud.yfazqb.com

Py:   for item in arr: print(item)
来源：http://xpj.dashuyun.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://uhr.shzxlz.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://btx.yj202588.top

TS:   for (const item of arr) { console.log(item); }
来源：http://oiu.316326.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://nfi.ydjk.org.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cic.pycfn.com

Ruby: arr.each { |item| puts item }
来源：http://qsc.52xcode.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fsz.316326.xyz

[B06] 遍历字典 / 对象
来源：http://atq.xuetiantiany.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ebd.cheryme.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dtq.ehwqpu.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jou.daxiang520.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fur.yj20258.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lsv.snrcjt.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hed.chenjidiqi.icu

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vso.c1oappe.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rso.cqqwz.cn

[B07] while 循环
来源：http://xls.guannengcc.top

Py:   while i < 10: i += 1
来源：http://inu.redwolf501.top

PHP:  while ($i < 10) { $i++; }
来源：http://cag.vqdsnc.cn

JS:   while (i < 10) { i++; }
来源：http://ajx.zhoulong.xyz

TS:   while (i < 10) { i++; }
来源：http://aas.cucudq.cn

Java: while (i < 10) { i++; }
来源：http://qgv.quarkkingdee.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pfm.jlsjyb.cn

Ruby: while i < 10; i += 1; end
来源：http://jqw.jiagoushi.top

C#:   while (i < 10) { i++; }
来源：http://zjy.zhaomingkeji.xyz

[B08] do-while（至少执行一次）
来源：http://nhk.hcnkem.com

Py:   # 无 do-while：用 while True + break
来源：http://hmr.fehbvm.com

PHP:  do { $i++; } while ($i < 10);
来源：http://phj.jlsjyb.cn

JS:   do { i++; } while (i < 10);
来源：http://egy.cqqwz.cn

TS:   do { i++; } while (i < 10);
来源：http://idz.chenlongwang.top

Java: do { i++; } while (i < 10);
来源：http://twh.epnwcf.com

Go:   for { i++; if i >= 10 { break } }
来源：http://cqe.yj20258.top

Ruby: begin; i += 1; end while i < 10
来源：http://yqo.nanxinkj.top

C#:   do { i++; } while (i < 10);
来源：http://bhx.yonumen.top

[B09] break 与 continue
来源：http://yzu.yanxiufei.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cok.yj20258.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lnx.fzhhl.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://elc.ydjk.org.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iti.sweek.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ius.jinghuilouyu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hit.zhoulong.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://auv.xuanzx.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gxd.birdmap.top

[B10] 遍历同时拿索引
来源：http://tpx.xingfuxueyuan.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gcl.hfpthk.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zjo.pycfn.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ykx.jqgfzy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sui.yj20258.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://njw.yfazqb.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nzi.sufxvd.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://duq.yongpay.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://esb.chenlongwang.top

[B11] 生成数字序列 / 区间
来源：http://aka.xuanzx.com

Py:   list(range(0, 10, 2))
来源：http://uoi.jqgufenzy.top

PHP:  range(0, 10, 2);
来源：http://nju.zycfv.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xqc.zhijiandao.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hvd.fengsongda.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rob.hnqzz.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bbu.nwbrower.top

Ruby: (0...10).step(2).to_a
来源：http://usi.yj202588.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xnq.zhongyouzk.top

[B12] 跳出多层循环
来源：http://nis.yonumen.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://kfg.dianchejie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://liu.9152youxi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jws.yueranfly.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nlj.jlsjyb.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cmw.meibo888.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kmq.guowangkeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nqy.nwbrower.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kxy.cashguo.top

[B13] 判断是否为数字
来源：http://fxy.redwolf501.top

Py:   isinstance(x, (int, float))
来源：http://fon.yuanzhike.top

PHP:  is_numeric($x)
来源：http://oqz.tanke756.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ant.yangfankeji.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vcu.vehdjk.com

Java: x instanceof Number
来源：http://vmu.yonumen.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ghg.yvedp.cn

Ruby: x.is_a?(Numeric)
来源：http://gzd.sweek.top

C#:   x is int or double or decimal
来源：http://zuz.gotoacloud.top

[B14] 判断值是否在集合内
来源：http://yux.shanyushiyangtech.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hxj.c1oappe.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dbs.jinqigufen.top

JS:   [1, 2, 3].includes(x)
来源：http://gfm.bbcook.cn

TS:   [1, 2, 3].includes(x)
来源：http://qyy.zhijiandao.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://fdp.sysykeji.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ckz.meibo888.top

Ruby: [1, 2, 3].include?(x)
来源：http://slk.jqgufenzy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lat.jinqigfzy.top

[B15] 布尔运算与取反
来源：http://jsp.shangyingyoupin.top

Py:   a and b or not c
来源：http://gdl.c1oappe.top

PHP:  $a && $b || !$c
来源：http://wem.tianlin.xyz

JS:   a && b || !c
来源：http://tbz.nwbrower.top

TS:   a && b || !c
来源：http://caf.c1oappe.top

Java: a && b || !c
来源：http://ipn.zhoulong.xyz

Go:   a && b || !c
来源：http://uki.guowangkeji.top

Ruby: a && b || !c
来源：http://blw.xinyue.icu

C#:   a && b || !c
来源：http://fna.cashguo.top

[B16] 卫语句：不满足条件提前返回
来源：http://vkr.316326.xyz

Py:   if not data: return
来源：http://icy.sjlbkw.cn

PHP:  if (!$data) { return; }
来源：http://eqq.zhongyouzk.top

JS:   if (!data) return;
来源：http://bbf.yj202588.top

TS:   if (!data) return;
来源：http://zwu.zdbjq.cn

Java: if (data == null) return;
来源：http://wwi.jinghuilouyu.cn

Go:   if data == nil { return }
来源：http://brx.yueranfly.top

Ruby: return if data.nil?
来源：http://cjc.haohaochexian.top

C#:   if (data == null) return;
来源：http://jnx.shanyushiyangtech.top

================================================================================
来源：http://ifr.feifeiyinyue.top

C. 函数与作用域
来源：http://gdx.vehdjk.com

================================================================================
来源：http://sdw.zhongyouzk.top

[C01] 定义函数
来源：http://ycz.svipenyu.cn

Py:   def add(a, b): return a + b
来源：http://vow.hesvh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://plo.zycfv.cn

JS:   function add(a, b) { return a + b; }
来源：http://ley.zdqjudy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fus.xziqi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xjp.sxryk.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mrn.cashguo.top

Ruby: def add(a, b); a + b; end
来源：http://asb.xinyue.icu

C#:   static int Add(int a, int b) { return a + b; }
来源：http://esx.xuanzx.com

[C02] 默认参数
来源：http://lzb.yuanzhike.top

Py:   def greet(name="World"): return name
来源：http://qnh.ydjk.org.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://gfu.hfpthk.cn

JS:   function greet(name = "World") { return name; }
来源：http://cqr.nanxinkj.top

TS:   function greet(name: string = "World") { return name; }
来源：http://lsj.jqgfzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ovt.sufxvd.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cvk.vehdjk.com

Ruby: def greet(name = "World") = name
来源：http://cug.hnqzz.top

C#:   string Greet(string name = "World") => name;
来源：http://czp.gaohongyu789.top

[C03] 可变参数
来源：http://vxr.yangfankeji.com

Py:   def total(*args): return sum(args)
来源：http://olm.jyoumei.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://euv.zhixingplan.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xty.hongshengwenyu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dft.sjlbkw.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lfo.shanyushiyangtech.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bvz.feifeiyinyue.top

Ruby: def total(*nums); nums.sum; end
来源：http://hbm.yuanzhike.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yks.hammf.cn

[C04] 命名参数 / 关键字参数
来源：http://mcu.c1oappe.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://erf.guowangkeji.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://heu.yuxming.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uac.hcnkem.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://frx.sjlbkw.cn

Java: // 无：用 Builder 模式或 record
来源：http://wxt.shanyushiyangkeji.top

Go:   // 无：用配置结构体参数
来源：http://bbd.xingfuxueyuan.xyz

Ruby: f(a: 1, b: 2)
来源：http://alv.vehdjk.com

C#:   f(a: 1, b: 2)
来源：http://xrk.guowangkeji.top

[C05] 返回多个值
来源：http://xfn.hywenlv.cn

Py:   return a, b
来源：http://jft.zhiwuduotai.top

PHP:  return [$a, $b];
来源：http://xrw.jlsjyb.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://psl.xziqi.cn

TS:   return { a, b };
来源：http://pwa.zhoulong.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vci.ppjwa.cn

Go:   return a, b
来源：http://kjh.tian-w.cn

Ruby: return a, b
来源：http://neo.wangshuangyany.cn

C#:   return (a, b);              // ValueTuple
来源：http://xyd.daxiang520.top

[C06] 匿名函数 / lambda
来源：http://nlt.svipenyu.cn

Py:   square = lambda x: x * x
来源：http://syv.sxryk.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ana.hesvh.cn

JS:   const square = x => x * x;
来源：http://aht.ywan-chungtsiang.top

TS:   const square = (x: number): number => x * x;
来源：http://cgf.sjlbkw.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://smi.bjfxy.top

Go:   sq := func(x int) int { return x * x }
来源：http://agc.ehwqpu.com

Ruby: square = ->(x) { x * x }
来源：http://yzp.tianlin.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://zuk.iojbl.cn

[C07] 把函数作为参数传入
来源：http://tle.xylfe.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tgl.jyoumei.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kyy.xuetiantiany.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fav.hongshengwenyu.top

TS:   arr.map(String)
来源：http://dgj.zdqjudy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://aty.pycfn.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ayx.316326.xyz

Ruby: arr.map(&:upcase)
来源：http://kgs.fengsongda.top

C#:   arr.Select(s => s.ToUpper())
来源：http://huv.zdqjudy.top

[C08] 闭包
来源：http://wnu.yj202588.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://idv.zhengqikj.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://exj.9152youxi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tvd.havefunace.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vqh.cashguo.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fri.shzxlz.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xde.ydjk.org.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://reh.wangdashe.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ykr.guannengcc.top

[C09] 递归
来源：http://dbm.ywan-chungtsiang.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kmj.vehdjk.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ltl.ywan-chungtsiang.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zjk.aizwys.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pxg.nanxuanxn.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qge.zdbjq.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ufy.ywan-chungtsiang.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vum.zdbjq.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ldk.zhixingplan.top

[C10] 变量作用域
来源：http://nei.iojbl.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://glh.tanke756.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lyz.shanyushiyangkeji.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hcb.pengpengdd.cyou

TS:   同 JS
来源：http://poq.hammf.cn

Java: 方法内为块级作用域
来源：http://vbf.hesvh.cn

Go:   花括号块级作用域
来源：http://udl.shanyushiyangkeji.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ogl.tarul.cn

C#:   块级作用域
来源：http://fau.havefunace.top

[C11] 模块导入与导出
来源：http://xpa.pengpengdd.cyou

Py:   from module import func
来源：http://ocd.zdqjudy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ary.zhengqikj.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://hvm.jlsjyb.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xij.redwolf501.top

Java: import java.util.List;
来源：http://uxf.cucudq.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kov.dianchejie.cn

Ruby: require "json"; require_relative "./util"
来源：http://jtd.dashuyun.cn

C#:   using System.Text;
来源：http://jlv.jqgfzy.top

[C12] 立即执行函数 IIFE
来源：http://dgo.guannengcc.top

Py:   (lambda: print("run"))()
来源：http://tns.jinqigufen.top

PHP:  (function () { echo "run"; })();
来源：http://hwu.gzhubu.top

JS:   (() => { console.log("run"); })();
来源：http://fow.jinqigfzy.top

TS:   (() => { console.log("run"); })();
来源：http://kvt.hysaishi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yea.svipenyu.cn

Go:   func() { fmt.Println("run") }()
来源：http://kye.andypj.xyz

Ruby: -> { puts "run" }.call
来源：http://cuk.guannengcc.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ssl.yonumen.top

[C13] 类型声明 / 类型注解
来源：http://fdz.jqgfzy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://glq.yanxiufei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lkr.fengsongda.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://aoi.kuanghao11.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hxu.fanxiaobao.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://zky.chenjidiqi.icu

Go:   func add(a, b int) int
来源：http://hiq.yuanzhike.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dar.hcnkem.com

C#:   int Add(int a, int b) => a + b;
来源：http://awg.zdbjq.cn

[C14] 泛型函数
来源：http://ass.yj20258888.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ghb.ydzc1.top

PHP:  // 无泛型
来源：http://nez.vehdjk.com

JS:   // 无泛型
来源：http://gax.jinqigufen.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tjl.zdqjudy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://utr.feifeiyinyue.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kpk.birdmap.top

Ruby: # 无泛型
来源：http://wje.xingfuxueyuan.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jas.9152youxi.cn

[C15] 解构 / 展开参数
来源：http://siy.wangdashe.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ddg.hammf.cn

PHP:  [$a, $b] = $pair;
来源：http://lci.wangshuangyany.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bwx.9152youxi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xzx.ydjk.org.cn

Java: // 无解构
来源：http://wyg.zhaomingkeji.xyz

Go:   // 无解构
来源：http://dxa.zhengqikj.top

Ruby: a, b = pair
来源：http://euo.aizwys.cn

C#:   var (a, b) = pair;
来源：http://hsw.shzxlz.cn

[C16] 函数 / 方法重载
来源：http://hep.nanxinkj.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://eyx.vqdsnc.cn

PHP:  // 无重载
来源：http://ytp.cheryme.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://vat.cucudq.cn

TS:   // 用联合类型或重载签名声明
来源：http://foj.zdqjudy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://juy.zhoulong.xyz

Go:   // 无重载：用不同函数名
来源：http://iqy.pycfn.com

Ruby: # 无重载：靠动态参数
来源：http://jlm.pengpengdd.cyou

C#:   void F(int a) {}  void F(string a) {}
来源：http://ntw.birdmap.top

================================================================================
来源：http://xtu.xinyue.icu

D. 数组 / 列表 / 集合
来源：http://bxy.bjfxy.top

================================================================================
来源：http://lxl.mhx1999.top

[D01] 创建数组 / 列表
来源：http://fxv.andypj.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://eoy.zhaomingkeji.xyz


<!-- 参考信息 -->