代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://kmd.yongpay.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yxo.daxiang520.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://aam.chenzaomai.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://znj.yvedp.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pcn.yangfankeji.com

================================================================================
来源：http://tqu.xingfuxueyuan.xyz

B. 流程控制
来源：http://xaq.dashuyun.cn

================================================================================
来源：http://rtc.meibo888.top

[B01] 条件判断 if / else
来源：http://ezv.jianghu66.top

Py:   result = "正" if x > 0 else "非正"
来源：http://lxm.sjlbkw.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fsd.zhoulong.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dsz.zhiwuduotai.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://cys.zhiwuduotai.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://jdo.havefunace.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wgf.shzxlz.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://icv.ybcxt.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mzn.jlsjyb.cn

[B02] 多分支 else if / elif
来源：http://imu.zhengqikj.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://egt.cheryme.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cfa.cdnleiting.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sng.jianghu66.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ews.daxiang520.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qww.bjfxy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pob.zhijiandao.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xqd.jinyuanbaomall.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ebh.xylfe.cn

[B03] switch / match / case
来源：http://nxs.jqgufenzy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sgx.sufxvd.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fne.gogol.net.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jer.0kj1m.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://koo.hnqzz.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://plz.c1oappe.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fpd.fanxiaobao.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://amv.jianghu66.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://prv.cucudq.cn

[B04] for 计数循环
来源：http://ybu.cashguo.top

Py:   for i in range(10): print(i)
来源：http://jud.tarul.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vec.gaohongyu789.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://inh.yueranfly.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://riy.dashuyun.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wsr.epnwcf.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ijb.gogol.net.cn

Ruby: 10.times { |i| puts i }
来源：http://uqg.andypj.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rvi.zhengqikj.top

[B05] 遍历数组 / 列表
来源：http://xck.vqdsnc.cn

Py:   for item in arr: print(item)
来源：http://frr.jinghuilouyu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pvq.shuidangran.top

JS:   for (const item of arr) { console.log(item); }
来源：http://lup.pengpengdd.cyou

TS:   for (const item of arr) { console.log(item); }
来源：http://rib.cashguo.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://fzr.kuanghao11.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jlb.cqqwz.cn

Ruby: arr.each { |item| puts item }
来源：http://mcz.ywan-chungtsiang.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tsm.sysykeji.top

[B06] 遍历字典 / 对象
来源：http://ohh.zhaomingkeji.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://iug.sufxvd.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kbu.hnqzz.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qyy.smart0.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gvd.zhixingplan.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://esu.hnxiangtu.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gri.yj202588.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dnx.jinghuilouyu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ysg.tian-w.cn

[B07] while 循环
来源：http://jsq.fktsv.cn

Py:   while i < 10: i += 1
来源：http://ehk.feifeiyinyue.top

PHP:  while ($i < 10) { $i++; }
来源：http://yce.hcnkem.com

JS:   while (i < 10) { i++; }
来源：http://rdx.hnxiangtu.top

TS:   while (i < 10) { i++; }
来源：http://lhc.hammf.cn

Java: while (i < 10) { i++; }
来源：http://ojd.xuetiantiany.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dic.yfazqb.com

Ruby: while i < 10; i += 1; end
来源：http://sxy.pycfn.com

C#:   while (i < 10) { i++; }
来源：http://ekz.bbcook.cn

[B08] do-while（至少执行一次）
来源：http://lwn.chenlongwang.top

Py:   # 无 do-while：用 while True + break
来源：http://ncg.dashuyun.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://hwg.0kj1m.cn

JS:   do { i++; } while (i < 10);
来源：http://fuc.zhongyouzk.top

TS:   do { i++; } while (i < 10);
来源：http://ewb.jiagoushi.top

Java: do { i++; } while (i < 10);
来源：http://yaf.yfazqb.com

Go:   for { i++; if i >= 10 { break } }
来源：http://twc.shzxlz.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zto.cqqwz.cn

C#:   do { i++; } while (i < 10);
来源：http://noh.chenzaomai.com

[B09] break 与 continue
来源：http://ngo.jyoumei.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bcm.jinghuilouyu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://alg.xinyue.icu

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xll.hcnkem.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://niy.tian-w.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://urv.ydzc1.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jgk.jqgfzy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vdl.zhaomingkeji.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pjv.pycfn.com

[B10] 遍历同时拿索引
来源：http://ush.andypj.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ziq.wangshuangyany.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qpy.smart0.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sun.gotoacloud.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wnl.jianghu66.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hzc.fengsongda.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://auu.shanyushiyangkeji.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fjs.jlsjyb.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gye.9152youxi.cn

[B11] 生成数字序列 / 区间
来源：http://lur.yonumen.top

Py:   list(range(0, 10, 2))
来源：http://yae.jlsjyb.cn

PHP:  range(0, 10, 2);
来源：http://hcs.gzhubu.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eqj.daria6918.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wgf.guannengcc.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://thr.sufxvd.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jov.aibaodan.cn

Ruby: (0...10).step(2).to_a
来源：http://ngu.shzxlz.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dgm.jlsjyb.cn

[B12] 跳出多层循环
来源：http://hxb.mhx1999.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://uao.pengpengdd.cyou

PHP:  # 无标签：用 goto 或函数返回
来源：http://xqc.zhiwuduotai.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pwu.jinyuanbaomall.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zet.gaohongyu789.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fjm.9152youxi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vzr.tian-w.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://epm.snrcjt.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://eeh.uphjek.com

[B13] 判断是否为数字
来源：http://fge.yfazqb.com

Py:   isinstance(x, (int, float))
来源：http://cqn.daria6918.cn

PHP:  is_numeric($x)
来源：http://tec.snrcjt.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xqm.jinghuilouyu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pmr.hysaishi.cn

Java: x instanceof Number
来源：http://xhr.jinghuilouyu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tsa.nanxinkj.top

Ruby: x.is_a?(Numeric)
来源：http://eox.pycfn.com

C#:   x is int or double or decimal
来源：http://fuf.aizwys.cn

[B14] 判断值是否在集合内
来源：http://knx.hnxiangtu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://enb.smart0.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kja.havefunace.top

JS:   [1, 2, 3].includes(x)
来源：http://wlv.c1oappe.top

TS:   [1, 2, 3].includes(x)
来源：http://err.ydjk.org.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ccr.quarkkingdee.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gkt.ydzc1.top

Ruby: [1, 2, 3].include?(x)
来源：http://icv.aibaodan.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gxo.shanyushiyangkeji.top

[B15] 布尔运算与取反
来源：http://dnl.svipenyu.cn

Py:   a and b or not c
来源：http://qly.vqdsnc.cn

PHP:  $a && $b || !$c
来源：http://zcw.yuanzhike.top

JS:   a && b || !c
来源：http://ifs.yangfankeji.com

TS:   a && b || !c
来源：http://nsk.fktsv.cn

Java: a && b || !c
来源：http://rpj.snrcjt.cn

Go:   a && b || !c
来源：http://qan.andypj.xyz

Ruby: a && b || !c
来源：http://wxi.316326.xyz

C#:   a && b || !c
来源：http://oyl.aizwys.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hvi.cdnleiting.top

Py:   if not data: return
来源：http://fsg.cucudq.cn

PHP:  if (!$data) { return; }
来源：http://baa.daxiang520.top

JS:   if (!data) return;
来源：http://xya.jinghuilouyu.cn

TS:   if (!data) return;
来源：http://iac.cqqwz.cn

Java: if (data == null) return;
来源：http://goe.dianchejie.cn

Go:   if data == nil { return }
来源：http://zcm.nanxinkj.top

Ruby: return if data.nil?
来源：http://ntl.iojbl.cn

C#:   if (data == null) return;
来源：http://hie.hcnkem.com

================================================================================
来源：http://lbg.pengpengdd.cyou

C. 函数与作用域
来源：http://rpr.xinyue.icu

================================================================================
来源：http://pvg.9152youxi.cn

[C01] 定义函数
来源：http://ixm.zhengqikj.top

Py:   def add(a, b): return a + b
来源：http://awp.ctjpmb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hbf.cdnleiting.top

JS:   function add(a, b) { return a + b; }
来源：http://cmo.epnwcf.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nfg.zhiwuduotai.top

Java: static int add(int a, int b) { return a + b; }
来源：http://zyk.dashuyun.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ygd.xuetiantiany.cn

Ruby: def add(a, b); a + b; end
来源：http://izf.yonumen.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tfb.cdnleiting.top

[C02] 默认参数
来源：http://kev.vehdjk.com

Py:   def greet(name="World"): return name
来源：http://cwj.pycfn.com

PHP:  function greet($name = "World") { return $name; }
来源：http://pei.sxryk.cn

JS:   function greet(name = "World") { return name; }
来源：http://onb.shuidangran.top

TS:   function greet(name: string = "World") { return name; }
来源：http://dhj.zhengqikj.top

Java: // 无默认参数：方法重载或 Optional
来源：http://rzn.dianchejie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zpj.pycfn.com

Ruby: def greet(name = "World") = name
来源：http://bpu.hnqzz.top

C#:   string Greet(string name = "World") => name;
来源：http://sgm.daxiang520.top

[C03] 可变参数
来源：http://sfa.gzhubu.top

Py:   def total(*args): return sum(args)
来源：http://ktx.sysykeji.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://isf.dashuyun.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tpx.ybcxt.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wya.nwbrower.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sgm.hnxiangtu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vbe.fzhhl.top

Ruby: def total(*nums); nums.sum; end
来源：http://ifx.sufxvd.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gqn.andypj.xyz

[C04] 命名参数 / 关键字参数
来源：http://vju.ywan-chungtsiang.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mgl.yj20258.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://uwo.ydzc1.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zos.bbcook.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nfg.shangyingyoupin.top

Java: // 无：用 Builder 模式或 record
来源：http://ymx.snrcjt.cn

Go:   // 无：用配置结构体参数
来源：http://pig.sufxvd.cn

Ruby: f(a: 1, b: 2)
来源：http://kom.epnwcf.com

C#:   f(a: 1, b: 2)
来源：http://vdb.jinyuanbaomall.cn

[C05] 返回多个值
来源：http://iqq.zdqjudy.top

Py:   return a, b
来源：http://eux.yvedp.cn

PHP:  return [$a, $b];
来源：http://ewb.yonumen.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://yqd.yj202588.top

TS:   return { a, b };
来源：http://crp.jinyuanbaomall.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qev.cdnleiting.top

Go:   return a, b
来源：http://xun.ydjk.org.cn

Ruby: return a, b
来源：http://bde.birdmap.top

C#:   return (a, b);              // ValueTuple
来源：http://xtv.daria6918.cn

[C06] 匿名函数 / lambda
来源：http://jvb.fanxiaobao.xyz

Py:   square = lambda x: x * x
来源：http://oxj.jyoumei.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xdf.ywan-chungtsiang.top

JS:   const square = x => x * x;
来源：http://ajd.hfpthk.cn

TS:   const square = (x: number): number => x * x;
来源：http://kzv.gotoacloud.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bbi.xinyue.icu

Go:   sq := func(x int) int { return x * x }
来源：http://foo.xingfuxueyuan.xyz

Ruby: square = ->(x) { x * x }
来源：http://lfh.xingfuxueyuan.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://hxr.hcnkem.com

[C07] 把函数作为参数传入
来源：http://kfn.hcnkem.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ykz.fktsv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://fzq.bbcook.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dzo.yvedp.cn

TS:   arr.map(String)
来源：http://wsz.ybcxt.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zhv.hcnkem.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gxc.xziqi.cn

Ruby: arr.map(&:upcase)
来源：http://jof.birdmap.top

C#:   arr.Select(s => s.ToUpper())
来源：http://zcy.bbcook.cn

[C08] 闭包
来源：http://klt.havefunace.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ikf.redwolf501.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://umi.hysaishi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mry.wangdashe.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://phu.andypj.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://syc.redwolf501.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vim.redwolf501.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kmz.hfpthk.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wzp.yfazqb.com

[C09] 递归
来源：http://bnw.jianghu66.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hzi.bjfxy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://iqv.jqgufenzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uit.daria6918.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uxf.zhiwuduotai.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://abb.dianchejie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ocj.daria6918.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://edl.daria6918.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pzp.wangshuangyany.cn

[C10] 变量作用域
来源：http://lvm.gogol.net.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ftt.52xcode.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ipp.shanyushiyangtech.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mrg.ydzc1.top

TS:   同 JS
来源：http://elf.cqqwz.cn

Java: 方法内为块级作用域
来源：http://abk.aizwys.cn

Go:   花括号块级作用域
来源：http://lhv.shuidangran.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lxz.cucudq.cn

C#:   块级作用域
来源：http://kup.ywan-chungtsiang.top

[C11] 模块导入与导出
来源：http://tzg.cucudq.cn

Py:   from module import func
来源：http://rse.vehdjk.com

PHP:  require "file.php";  或 use App\Service;
来源：http://wdk.zhoulong.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://ohx.hesvh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xcp.dianchejie.cn

Java: import java.util.List;
来源：http://yus.tianlin.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ejx.sufxvd.cn

Ruby: require "json"; require_relative "./util"
来源：http://chv.cheryme.top

C#:   using System.Text;
来源：http://ead.yuxming.cn

[C12] 立即执行函数 IIFE
来源：http://vee.tarul.cn

Py:   (lambda: print("run"))()
来源：http://qcd.andypj.xyz

PHP:  (function () { echo "run"; })();
来源：http://nns.zycfv.cn

JS:   (() => { console.log("run"); })();
来源：http://ela.tarul.cn

TS:   (() => { console.log("run"); })();
来源：http://qwm.tianlin.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yqo.birdmap.top

Go:   func() { fmt.Println("run") }()
来源：http://wgx.9152youxi.cn

Ruby: -> { puts "run" }.call
来源：http://cso.ctjpmb.com

C#:   // 无 IIFE：用静态构造函数
来源：http://uzt.hfpthk.cn

[C13] 类型声明 / 类型注解
来源：http://fmy.iojbl.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lbm.jiagoushi.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cse.zdqjudy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mve.sysykeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mzv.fzhhl.top

Java: int add(int a, int b) { return a + b; }
来源：http://tii.yj20258888.top

Go:   func add(a, b int) int
来源：http://yvb.shanyushiyangtech.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cxe.ppjwa.cn

C#:   int Add(int a, int b) => a + b;
来源：http://dxm.yongpay.top

[C14] 泛型函数
来源：http://iio.zdqjudy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://waz.fehbvm.com

PHP:  // 无泛型
来源：http://jex.sjlbkw.cn

JS:   // 无泛型
来源：http://akd.guannengcc.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dzk.sjlbkw.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ype.cucudq.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ais.pycfn.com

Ruby: # 无泛型
来源：http://pvw.yonumen.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vbe.cdnleiting.top

[C15] 解构 / 展开参数
来源：http://biu.pycfn.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jte.hammf.cn

PHP:  [$a, $b] = $pair;
来源：http://gyq.316326.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pjk.hywenlv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://exy.nanxinkj.top

Java: // 无解构
来源：http://jyn.uphjek.com

Go:   // 无解构
来源：http://jjo.wangdashe.top

Ruby: a, b = pair
来源：http://tse.chenjidiqi.icu

C#:   var (a, b) = pair;
来源：http://zth.ppjwa.cn

[C16] 函数 / 方法重载
来源：http://pfx.zhongyouzk.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kdc.sysykeji.top

PHP:  // 无重载
来源：http://twf.cheryme.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://hqt.zhijiandao.cn

TS:   // 用联合类型或重载签名声明
来源：http://hhr.snrcjt.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://zwj.quarkkingdee.top

Go:   // 无重载：用不同函数名
来源：http://xhx.cashguo.top

Ruby: # 无重载：靠动态参数
来源：http://vhk.vehdjk.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://fjl.tarul.cn

================================================================================
来源：http://lxy.zhijiandao.cn


<!-- 参考信息 -->