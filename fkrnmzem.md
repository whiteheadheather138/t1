代发 wailian999

[B01] 条件判断 if / else
来源：http://eik.pycfn.com

Py:   result = "正" if x > 0 else "非正"
来源：http://swh.bbcook.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lao.hnxiangtu.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jpu.shanyushiyangtech.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kfa.fengsongda.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://yuu.316326.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mce.guannengcc.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rqe.bjfxy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fug.zdqjudy.top

[B02] 多分支 else if / elif
来源：http://xaq.zhongyouzk.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bsm.sxryk.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tof.hammf.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://toh.guannengcc.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dmf.shangyingyoupin.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ggk.hesvh.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://upu.gotoacloud.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zoe.birdmap.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pdo.daria6918.cn

[B03] switch / match / case
来源：http://kea.jianghu66.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ufn.yangfankeji.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xzj.aibaodan.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zle.shanyushiyangkeji.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cov.chenzaomai.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cli.xziqi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fmh.yuanzhike.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ips.hfpthk.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lnu.tanke756.top

[B04] for 计数循环
来源：http://ups.zhoulong.xyz

Py:   for i in range(10): print(i)
来源：http://jml.yfazqb.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ejg.bjfxy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dkk.0kj1m.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dnp.kuanghao11.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uph.cheryme.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mou.mhx1999.top

Ruby: 10.times { |i| puts i }
来源：http://hyv.yuanzhike.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pzl.gogol.net.cn

[B05] 遍历数组 / 列表
来源：http://kwl.haohaochexian.top

Py:   for item in arr: print(item)
来源：http://ldc.chenzaomai.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vgv.jinyuanbaomall.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://lll.ctjpmb.com

TS:   for (const item of arr) { console.log(item); }
来源：http://cvh.zycfv.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wkv.snrcjt.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wfj.zhiwuduotai.top

Ruby: arr.each { |item| puts item }
来源：http://aiw.yvedp.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ygl.xuetiantiany.cn

[B06] 遍历字典 / 对象
来源：http://qqt.chenlongwang.top

Py:   for k, v in d.items(): print(k, v)
来源：http://sne.jqgfzy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mqb.zdbjq.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lcg.wangshuangyany.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xin.xinyue.icu

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lcg.yuanzhike.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bbs.tanke756.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://psb.0kj1m.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jpu.hywenlv.cn

[B07] while 循环
来源：http://wku.hongshengwenyu.top

Py:   while i < 10: i += 1
来源：http://acd.yj20258888.top

PHP:  while ($i < 10) { $i++; }
来源：http://wdm.hnqzz.top

JS:   while (i < 10) { i++; }
来源：http://ieh.feifeiyinyue.top

TS:   while (i < 10) { i++; }
来源：http://qmf.fzhhl.top

Java: while (i < 10) { i++; }
来源：http://brb.zdbjq.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kdn.zhongyouzk.top

Ruby: while i < 10; i += 1; end
来源：http://qxb.ywan-chungtsiang.top

C#:   while (i < 10) { i++; }
来源：http://cwn.yanxiufei.cn

[B08] do-while（至少执行一次）
来源：http://xdn.pycfn.com

Py:   # 无 do-while：用 while True + break
来源：http://zqv.smart0.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://bpi.hfpthk.cn

JS:   do { i++; } while (i < 10);
来源：http://hjg.gotoacloud.top

TS:   do { i++; } while (i < 10);
来源：http://miq.sxryk.cn

Java: do { i++; } while (i < 10);
来源：http://udi.gaohongyu789.top

Go:   for { i++; if i >= 10 { break } }
来源：http://wch.mhx1999.top

Ruby: begin; i += 1; end while i < 10
来源：http://scj.zhixingplan.top

C#:   do { i++; } while (i < 10);
来源：http://bwv.fktsv.cn

[B09] break 与 continue
来源：http://kva.yuxming.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mnz.hongshengwenyu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ewd.hfpthk.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://orw.yuxming.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bry.snrcjt.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nhr.iojbl.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://iin.316326.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jfs.dashuyun.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kfx.yj20258.top

[B10] 遍历同时拿索引
来源：http://zzn.sweek.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://whl.hnqzz.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zqz.wangdashe.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ovi.hysaishi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tcs.wangdashe.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xky.daria6918.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lyu.9152youxi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://stk.zhengqikj.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qiu.redwolf501.top

[B11] 生成数字序列 / 区间
来源：http://hub.svipenyu.cn

Py:   list(range(0, 10, 2))
来源：http://adh.52xcode.cn

PHP:  range(0, 10, 2);
来源：http://dhk.bjfxy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ifh.birdmap.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kgc.jyoumei.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ptv.tanke756.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kxv.yongpay.top

Ruby: (0...10).step(2).to_a
来源：http://kcf.gaohongyu789.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zol.meibo888.top

[B12] 跳出多层循环
来源：http://ecx.quarkkingdee.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://qul.pengpengdd.cyou

PHP:  # 无标签：用 goto 或函数返回
来源：http://raa.yuxming.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ijw.bjfxy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kpa.tianlin.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://psi.yj20258888.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://oql.ctjpmb.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xva.yangfankeji.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dgx.mhx1999.top

[B13] 判断是否为数字
来源：http://txu.xziqi.cn

Py:   isinstance(x, (int, float))
来源：http://awd.fengsongda.top

PHP:  is_numeric($x)
来源：http://kxh.zhaomingkeji.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ner.sufxvd.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vvk.cdnleiting.top

Java: x instanceof Number
来源：http://aeu.9152youxi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wrd.redwolf501.top

Ruby: x.is_a?(Numeric)
来源：http://zvk.jqgufenzy.top

C#:   x is int or double or decimal
来源：http://maa.tanke756.top

[B14] 判断值是否在集合内
来源：http://ces.zdqjudy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://trc.zhaomingkeji.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://snq.yj20258888.top

JS:   [1, 2, 3].includes(x)
来源：http://inx.ydjk.org.cn

TS:   [1, 2, 3].includes(x)
来源：http://bbg.nanxinkj.top

Java: List.of(1, 2, 3).contains(x)
来源：http://fgh.hongshengwenyu.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://htq.cheryme.top

Ruby: [1, 2, 3].include?(x)
来源：http://bzg.sxryk.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jag.zhongyouzk.top

[B15] 布尔运算与取反
来源：http://tjb.aizwys.cn

Py:   a and b or not c
来源：http://egm.ctjpmb.com

PHP:  $a && $b || !$c
来源：http://hvt.cashguo.top

JS:   a && b || !c
来源：http://zol.0kj1m.cn

TS:   a && b || !c
来源：http://mty.zdbjq.cn

Java: a && b || !c
来源：http://oyy.shuidangran.top

Go:   a && b || !c
来源：http://kop.tianlin.xyz

Ruby: a && b || !c
来源：http://bpg.guowangkeji.top

C#:   a && b || !c
来源：http://urg.yuanzhike.top

[B16] 卫语句：不满足条件提前返回
来源：http://jiy.andypj.xyz

Py:   if not data: return
来源：http://wxt.ywan-chungtsiang.top

PHP:  if (!$data) { return; }
来源：http://ssa.hfpthk.cn

JS:   if (!data) return;
来源：http://hjh.ywan-chungtsiang.top

TS:   if (!data) return;
来源：http://ttb.52xcode.cn

Java: if (data == null) return;
来源：http://gfo.andypj.xyz

Go:   if data == nil { return }
来源：http://hhz.zhixingplan.top

Ruby: return if data.nil?
来源：http://pxo.redwolf501.top

C#:   if (data == null) return;
来源：http://ftc.jianghu66.top

================================================================================
来源：http://ija.c1oappe.top

C. 函数与作用域
来源：http://zpc.cashguo.top

================================================================================
来源：http://tja.fengsongda.top

[C01] 定义函数
来源：http://oly.hnxiangtu.top

Py:   def add(a, b): return a + b
来源：http://llo.haohaochexian.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lmy.tarul.cn

JS:   function add(a, b) { return a + b; }
来源：http://pes.hnxiangtu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jia.zhixingplan.top

Java: static int add(int a, int b) { return a + b; }
来源：http://rbz.jinghuilouyu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://phk.jinqigfzy.top

Ruby: def add(a, b); a + b; end
来源：http://bfg.meibo888.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mpc.hnqzz.top

[C02] 默认参数
来源：http://kyg.hcnkem.com

Py:   def greet(name="World"): return name
来源：http://kjj.chenjidiqi.icu

PHP:  function greet($name = "World") { return $name; }
来源：http://xib.tian-w.cn

JS:   function greet(name = "World") { return name; }
来源：http://hfm.zhixingplan.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ohx.yanxiufei.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://twr.zhaomingkeji.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xom.epnwcf.com

Ruby: def greet(name = "World") = name
来源：http://okx.dianchejie.cn

C#:   string Greet(string name = "World") => name;
来源：http://abp.jlsjyb.cn

[C03] 可变参数
来源：http://rjp.jyoumei.cn

Py:   def total(*args): return sum(args)
来源：http://jfr.sysykeji.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vpm.xylfe.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gav.pengpengdd.cyou

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tzj.52xcode.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qni.yonumen.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jdg.ivvv.top

Ruby: def total(*nums); nums.sum; end
来源：http://qoa.shanyushiyangtech.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ewt.cdnleiting.top

[C04] 命名参数 / 关键字参数
来源：http://xig.xuetiantiany.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ixg.cucudq.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ufz.zhaomingkeji.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nvh.hnxiangtu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bfj.fehbvm.com

Java: // 无：用 Builder 模式或 record
来源：http://uxh.xylfe.cn

Go:   // 无：用配置结构体参数
来源：http://vpi.xziqi.cn

Ruby: f(a: 1, b: 2)
来源：http://ntp.jinyuanbaomall.cn

C#:   f(a: 1, b: 2)
来源：http://off.guannengcc.top

[C05] 返回多个值
来源：http://kfi.ydjk.org.cn

Py:   return a, b
来源：http://jou.jinyuanbaomall.cn

PHP:  return [$a, $b];
来源：http://wps.yfazqb.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://vlc.jiagoushi.top

TS:   return { a, b };
来源：http://mvc.52xcode.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://daj.yonumen.top

Go:   return a, b
来源：http://qly.vqdsnc.cn

Ruby: return a, b
来源：http://orh.ywan-chungtsiang.top

C#:   return (a, b);              // ValueTuple
来源：http://xze.fanxiaobao.xyz

[C06] 匿名函数 / lambda
来源：http://oja.hysaishi.cn

Py:   square = lambda x: x * x
来源：http://day.wangdashe.top

PHP:  $square = fn($x) => $x * $x;
来源：http://dju.svipenyu.cn

JS:   const square = x => x * x;
来源：http://xuf.hfpthk.cn

TS:   const square = (x: number): number => x * x;
来源：http://rua.ivvv.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cnt.ydzc1.top

Go:   sq := func(x int) int { return x * x }
来源：http://mki.jianghu66.top

Ruby: square = ->(x) { x * x }
来源：http://app.ctjpmb.com

C#:   Func<int, int> square = x => x * x;
来源：http://qge.wangdashe.top

[C07] 把函数作为参数传入
来源：http://vdq.vqdsnc.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ryp.zhixingplan.top

PHP:  array_map("strtoupper", $arr);
来源：http://vfa.shangyingyoupin.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xry.guowangkeji.top

TS:   arr.map(String)
来源：http://wju.hesvh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rjk.fzhhl.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wsn.fktsv.cn

Ruby: arr.map(&:upcase)
来源：http://qbh.zhixingplan.top

C#:   arr.Select(s => s.ToUpper())
来源：http://dfs.zycfv.cn

[C08] 闭包
来源：http://kld.nanxuanxn.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://iks.hywenlv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://urr.dianchejie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nqp.fengsongda.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kkg.ybcxt.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://aln.fzhhl.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lgx.cashguo.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://svo.xinyue.icu

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dyq.zhixingplan.top

[C09] 递归
来源：http://ljn.fehbvm.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vwl.52xcode.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://amg.jinqigufen.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gfu.gzhubu.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jbv.zhongyouzk.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fme.sjlbkw.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rpb.chenlongwang.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fxc.sufxvd.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dfv.zdbjq.cn

[C10] 变量作用域
来源：http://msg.hcnkem.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://arp.smart0.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hwn.chenlongwang.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tfx.fehbvm.com

TS:   同 JS
来源：http://jlh.epnwcf.com

Java: 方法内为块级作用域
来源：http://jig.chenlongwang.top

Go:   花括号块级作用域
来源：http://puw.jinghuilouyu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rca.xingfuxueyuan.xyz

C#:   块级作用域
来源：http://dsh.haohaochexian.top

[C11] 模块导入与导出
来源：http://gzw.nanxinkj.top

Py:   from module import func
来源：http://kab.bbcook.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ewn.sysykeji.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://skg.mhx1999.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rtx.fehbvm.com

Java: import java.util.List;
来源：http://aiz.bjfxy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://aud.tarul.cn

Ruby: require "json"; require_relative "./util"
来源：http://wsu.jinghuilouyu.cn

C#:   using System.Text;
来源：http://pbu.epnwcf.com

[C12] 立即执行函数 IIFE
来源：http://itn.feifeiyinyue.top

Py:   (lambda: print("run"))()
来源：http://kym.shanyushiyangtech.top

PHP:  (function () { echo "run"; })();
来源：http://vlh.cheryme.top

JS:   (() => { console.log("run"); })();
来源：http://bmh.nanxinkj.top

TS:   (() => { console.log("run"); })();
来源：http://eha.tarul.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tvx.yj20258.top

Go:   func() { fmt.Println("run") }()
来源：http://xwq.zhoulong.xyz

Ruby: -> { puts "run" }.call
来源：http://yxl.nanxuanxn.top

C#:   // 无 IIFE：用静态构造函数
来源：http://meo.zhijiandao.cn

[C13] 类型声明 / 类型注解
来源：http://zhj.zhaomingkeji.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wet.guannengcc.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hhw.meibo888.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rlv.hywenlv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://aqz.meibo888.top

Java: int add(int a, int b) { return a + b; }
来源：http://nwr.jinghuilouyu.cn

Go:   func add(a, b int) int
来源：http://mix.dashuyun.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://igk.hywenlv.cn

C#:   int Add(int a, int b) => a + b;
来源：http://zii.ydzc1.top

[C14] 泛型函数
来源：http://hyn.birdmap.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jad.hammf.cn

PHP:  // 无泛型
来源：http://dlw.hammf.cn

JS:   // 无泛型
来源：http://fzl.jqgfzy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xyp.zhengqikj.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dlb.guannengcc.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kxk.guowangkeji.top

Ruby: # 无泛型
来源：http://lrr.ydjk.org.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qyq.ehwqpu.com

[C15] 解构 / 展开参数
来源：http://gpb.chenjidiqi.icu

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tbq.fzhhl.top

PHP:  [$a, $b] = $pair;
来源：http://hrv.zdbjq.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://acx.sufxvd.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jgw.yueranfly.top

Java: // 无解构
来源：http://xdw.hysaishi.cn

Go:   // 无解构
来源：http://pvl.iojbl.cn

Ruby: a, b = pair
来源：http://txy.c1oappe.top

C#:   var (a, b) = pair;
来源：http://szw.zhijiandao.cn

[C16] 函数 / 方法重载
来源：http://xqs.jyoumei.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://udm.316326.xyz

PHP:  // 无重载
来源：http://wqs.jqgufenzy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ffa.jianghu66.top

TS:   // 用联合类型或重载签名声明
来源：http://eny.sweek.top

Java: void f(int a) {}  void f(String a) {}
来源：http://yov.sufxvd.cn

Go:   // 无重载：用不同函数名
来源：http://oha.wangshuangyany.cn

Ruby: # 无重载：靠动态参数
来源：http://gcg.gzhubu.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://cfu.zhongyouzk.top

================================================================================
来源：http://cmk.zhixingplan.top

D. 数组 / 列表 / 集合
来源：http://xej.jinqigfzy.top

================================================================================
来源：http://fmq.cdnleiting.top

[D01] 创建数组 / 列表
来源：http://cam.sxryk.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://cnq.xuanzx.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bsz.yj202588.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gzz.hesvh.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ktq.cdnleiting.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yab.fanxiaobao.xyz


<!-- 参考信息 -->