代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://cve.hfpthk.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dzo.wangdashe.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kir.xuetiantiany.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ggk.vehdjk.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gmb.xylfe.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yjs.redwolf501.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ynf.yj202588.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xoq.fehbvm.com

[A26] 类型转换总览
来源：http://sgh.shanyushiyangkeji.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wea.cheryme.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gbm.jinqigfzy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hwi.yj20258888.top

TS:   Number() String() Boolean() x as number
来源：http://hxl.316326.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ufg.nanxinkj.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://els.daria6918.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ryk.meibo888.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vhn.haohaochexian.top

================================================================================
来源：http://euu.havefunace.top

B. 流程控制
来源：http://qvd.c1oappe.top

================================================================================
来源：http://cyq.nanxinkj.top

[B01] 条件判断 if / else
来源：http://lea.wangdashe.top

Py:   result = "正" if x > 0 else "非正"
来源：http://fjm.hongshengwenyu.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xop.hesvh.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nyq.wangdashe.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dar.zhengqikj.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ztl.yangfankeji.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://roc.hcnkem.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://frz.yongpay.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nae.hysaishi.cn

[B02] 多分支 else if / elif
来源：http://qcu.dashuyun.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mgt.hnxiangtu.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fbx.cheryme.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://foc.guannengcc.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ujv.xziqi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ncb.cashguo.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zna.ybcxt.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://osv.andypj.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uqe.sufxvd.cn

[B03] switch / match / case
来源：http://xui.mhx1999.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ofb.birdmap.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://djk.jlsjyb.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://auc.xziqi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pjb.hnqzz.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dqp.pengpengdd.cyou

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wpk.tanke756.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kvk.zhixingplan.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wzy.redwolf501.top

[B04] for 计数循环
来源：http://jye.ydzc1.top

Py:   for i in range(10): print(i)
来源：http://vcf.cashguo.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vrt.yj20258888.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jsm.yueranfly.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pcs.tarul.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vgj.shuidangran.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lyx.hcnkem.com

Ruby: 10.times { |i| puts i }
来源：http://vka.ybcxt.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blk.yuanzhike.top

[B05] 遍历数组 / 列表
来源：http://aun.shanyushiyangtech.top

Py:   for item in arr: print(item)
来源：http://vej.smart0.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mji.daxiang520.top

JS:   for (const item of arr) { console.log(item); }
来源：http://nrh.mhx1999.top

TS:   for (const item of arr) { console.log(item); }
来源：http://sui.cqqwz.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sxx.xylfe.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://uia.xinyue.icu

Ruby: arr.each { |item| puts item }
来源：http://dhb.jiagoushi.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kqm.jinqigfzy.top

[B06] 遍历字典 / 对象
来源：http://tys.hywenlv.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://uhj.hcnkem.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bre.snrcjt.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://njd.cashguo.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ysy.shanyushiyangtech.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jyq.aibaodan.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sbj.bbcook.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mal.tarul.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://esr.cashguo.top

[B07] while 循环
来源：http://sfb.shzxlz.cn

Py:   while i < 10: i += 1
来源：http://fqe.jinyuanbaomall.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zns.zhongyouzk.top

JS:   while (i < 10) { i++; }
来源：http://iel.dashuyun.cn

TS:   while (i < 10) { i++; }
来源：http://wft.wangdashe.top

Java: while (i < 10) { i++; }
来源：http://vbe.0kj1m.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://eug.ydzc1.top

Ruby: while i < 10; i += 1; end
来源：http://qgu.bjfxy.top

C#:   while (i < 10) { i++; }
来源：http://qsh.jyoumei.cn

[B08] do-while（至少执行一次）
来源：http://gre.ydzc1.top

Py:   # 无 do-while：用 while True + break
来源：http://wjk.andypj.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://rad.cdnleiting.top

JS:   do { i++; } while (i < 10);
来源：http://lxz.shuidangran.top

TS:   do { i++; } while (i < 10);
来源：http://jdm.wangshuangyany.cn

Java: do { i++; } while (i < 10);
来源：http://vrg.daxiang520.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ork.xylfe.cn

Ruby: begin; i += 1; end while i < 10
来源：http://dtz.zhaomingkeji.xyz

C#:   do { i++; } while (i < 10);
来源：http://qyq.uphjek.com

[B09] break 与 continue
来源：http://uvj.guowangkeji.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://uif.ywan-chungtsiang.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zmy.aibaodan.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nxx.gogol.net.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://svv.nanxuanxn.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yei.fehbvm.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cpi.tian-w.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bln.yj202588.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ysb.xuanzx.com

[B10] 遍历同时拿索引
来源：http://exd.hcnkem.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yxd.gaohongyu789.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fhx.yuanzhike.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wzf.tianlin.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pgy.xuanzx.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lld.nanxuanxn.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mgn.kuanghao11.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tsz.zhiwuduotai.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pie.xziqi.cn

[B11] 生成数字序列 / 区间
来源：http://jsb.c1oappe.top

Py:   list(range(0, 10, 2))
来源：http://dna.sysykeji.top

PHP:  range(0, 10, 2);
来源：http://diu.ppjwa.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ptc.tianlin.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://igk.yangfankeji.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ybc.shangyingyoupin.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://idu.tianlin.xyz

Ruby: (0...10).step(2).to_a
来源：http://caz.yj20258.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hwt.xuanzx.com

[B12] 跳出多层循环
来源：http://hur.ehwqpu.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://dbd.ydzc1.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://gnh.yongpay.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://liv.yanxiufei.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mwo.xinyue.icu

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qdt.ehwqpu.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lto.tanke756.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zyd.yj202588.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ysn.nanxinkj.top

[B13] 判断是否为数字
来源：http://xsw.svipenyu.cn

Py:   isinstance(x, (int, float))
来源：http://crj.316326.xyz

PHP:  is_numeric($x)
来源：http://hes.gotoacloud.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tru.birdmap.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kza.c1oappe.top

Java: x instanceof Number
来源：http://smr.nwbrower.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xrp.52xcode.cn

Ruby: x.is_a?(Numeric)
来源：http://nvu.shanyushiyangkeji.top

C#:   x is int or double or decimal
来源：http://tpj.chenzaomai.com

[B14] 判断值是否在集合内
来源：http://jvk.fzhhl.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://szg.gogol.net.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gaz.haohaochexian.top

JS:   [1, 2, 3].includes(x)
来源：http://aos.sjlbkw.cn

TS:   [1, 2, 3].includes(x)
来源：http://nkc.chenzaomai.com

Java: List.of(1, 2, 3).contains(x)
来源：http://xuk.fanxiaobao.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dqu.nanxinkj.top

Ruby: [1, 2, 3].include?(x)
来源：http://kcc.zycfv.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qhe.hnxiangtu.top

[B15] 布尔运算与取反
来源：http://dsa.cqqwz.cn

Py:   a and b or not c
来源：http://cyd.vqdsnc.cn

PHP:  $a && $b || !$c
来源：http://kda.sjlbkw.cn

JS:   a && b || !c
来源：http://vfv.xinyue.icu

TS:   a && b || !c
来源：http://pof.nanxinkj.top

Java: a && b || !c
来源：http://bqh.bbcook.cn

Go:   a && b || !c
来源：http://out.fengsongda.top

Ruby: a && b || !c
来源：http://qeo.nwbrower.top

C#:   a && b || !c
来源：http://yln.hongshengwenyu.top

[B16] 卫语句：不满足条件提前返回
来源：http://pwk.zhaomingkeji.xyz

Py:   if not data: return
来源：http://mey.fehbvm.com

PHP:  if (!$data) { return; }
来源：http://qhi.52xcode.cn

JS:   if (!data) return;
来源：http://pdl.gaohongyu789.top

TS:   if (!data) return;
来源：http://bfa.gzhubu.top

Java: if (data == null) return;
来源：http://mnw.ppjwa.cn

Go:   if data == nil { return }
来源：http://suc.meibo888.top

Ruby: return if data.nil?
来源：http://xar.zhiwuduotai.top

C#:   if (data == null) return;
来源：http://jpq.pengpengdd.cyou

================================================================================
来源：http://fmj.cucudq.cn

C. 函数与作用域
来源：http://ved.birdmap.top

================================================================================
来源：http://mvp.hesvh.cn

[C01] 定义函数
来源：http://gwe.zhiwuduotai.top

Py:   def add(a, b): return a + b
来源：http://swz.shanyushiyangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pth.zhongyouzk.top

JS:   function add(a, b) { return a + b; }
来源：http://tsi.cheryme.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gfi.fktsv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bqb.hywenlv.cn

Go:   func add(a, b int) int { return a + b }
来源：http://tlm.zhengqikj.top

Ruby: def add(a, b); a + b; end
来源：http://das.nwbrower.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lsk.hnqzz.top

[C02] 默认参数
来源：http://dvk.cqqwz.cn

Py:   def greet(name="World"): return name
来源：http://sqe.yongpay.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ufo.hnqzz.top

JS:   function greet(name = "World") { return name; }
来源：http://dbf.birdmap.top

TS:   function greet(name: string = "World") { return name; }
来源：http://whg.guannengcc.top

Java: // 无默认参数：方法重载或 Optional
来源：http://icv.andypj.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://poc.xinyue.icu

Ruby: def greet(name = "World") = name
来源：http://ckx.wangshuangyany.cn

C#:   string Greet(string name = "World") => name;
来源：http://brw.ydzc1.top

[C03] 可变参数
来源：http://rvf.bbcook.cn

Py:   def total(*args): return sum(args)
来源：http://lft.ywan-chungtsiang.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ycu.yonumen.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://oyn.dashuyun.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://iak.c1oappe.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qnp.yj202588.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pwv.yvedp.cn

Ruby: def total(*nums); nums.sum; end
来源：http://npu.ywan-chungtsiang.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bik.yueranfly.top

[C04] 命名参数 / 关键字参数
来源：http://uwd.chenlongwang.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nlq.snrcjt.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vie.pycfn.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sye.chenjidiqi.icu

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://eyg.feifeiyinyue.top

Java: // 无：用 Builder 模式或 record
来源：http://oxk.tanke756.top

Go:   // 无：用配置结构体参数
来源：http://cfw.ppjwa.cn

Ruby: f(a: 1, b: 2)
来源：http://idv.zdqjudy.top

C#:   f(a: 1, b: 2)
来源：http://zjy.tarul.cn

[C05] 返回多个值
来源：http://ouo.fehbvm.com

Py:   return a, b
来源：http://wzl.kuanghao11.cn

PHP:  return [$a, $b];
来源：http://kym.fehbvm.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://yfz.xylfe.cn

TS:   return { a, b };
来源：http://vxq.zhaomingkeji.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://erv.cucudq.cn

Go:   return a, b
来源：http://obn.hywenlv.cn

Ruby: return a, b
来源：http://txx.cdnleiting.top

C#:   return (a, b);              // ValueTuple
来源：http://oov.smart0.xyz

[C06] 匿名函数 / lambda
来源：http://tlp.fengsongda.top

Py:   square = lambda x: x * x
来源：http://lxd.hnxiangtu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://nlm.birdmap.top

JS:   const square = x => x * x;
来源：http://xzt.9152youxi.cn

TS:   const square = (x: number): number => x * x;
来源：http://fym.jinqigufen.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nia.tarul.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gbh.gzhubu.top

Ruby: square = ->(x) { x * x }
来源：http://ljb.zhaomingkeji.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://ahb.mhx1999.top

[C07] 把函数作为参数传入
来源：http://qyd.uphjek.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gvp.ehwqpu.com

PHP:  array_map("strtoupper", $arr);
来源：http://cdv.ehwqpu.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://efx.hesvh.cn

TS:   arr.map(String)
来源：http://gyy.xuetiantiany.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baf.sufxvd.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nrv.aibaodan.cn

Ruby: arr.map(&:upcase)
来源：http://adc.yvedp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mch.hnxiangtu.top

[C08] 闭包
来源：http://kju.guannengcc.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gui.ppjwa.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uiq.vehdjk.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sti.ywan-chungtsiang.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cvz.shangyingyoupin.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rqq.shanyushiyangkeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://puu.yueranfly.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kto.hywenlv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bkj.uphjek.com

[C09] 递归
来源：http://igp.0kj1m.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nud.jinghuilouyu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ubg.zhijiandao.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rlb.hnqzz.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://voq.jqgfzy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gqn.fzhhl.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ffu.fengsongda.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kla.bbcook.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bgr.vehdjk.com

[C10] 变量作用域
来源：http://gov.svipenyu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fmk.quarkkingdee.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dvy.shangyingyoupin.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yld.nanxuanxn.top

TS:   同 JS
来源：http://qap.uphjek.com

Java: 方法内为块级作用域
来源：http://rec.tian-w.cn

Go:   花括号块级作用域
来源：http://epu.yvedp.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://buu.yongpay.top

C#:   块级作用域
来源：http://lln.tianlin.xyz

[C11] 模块导入与导出
来源：http://hfr.yvedp.cn

Py:   from module import func
来源：http://nak.xylfe.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zwo.haohaochexian.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ztw.gzhubu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wgj.yj20258888.top

Java: import java.util.List;
来源：http://lop.jyoumei.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uzv.jianghu66.top

Ruby: require "json"; require_relative "./util"
来源：http://nhj.guowangkeji.top

C#:   using System.Text;
来源：http://aij.meibo888.top

[C12] 立即执行函数 IIFE
来源：http://akg.sxryk.cn

Py:   (lambda: print("run"))()
来源：http://vwd.bjfxy.top

PHP:  (function () { echo "run"; })();
来源：http://nne.yj202588.top

JS:   (() => { console.log("run"); })();
来源：http://mfh.yj20258.top

TS:   (() => { console.log("run"); })();
来源：http://ljt.ydjk.org.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nci.sxryk.cn

Go:   func() { fmt.Println("run") }()
来源：http://olf.jlsjyb.cn

Ruby: -> { puts "run" }.call
来源：http://vlo.shanyushiyangtech.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ejl.hammf.cn

[C13] 类型声明 / 类型注解
来源：http://ash.gzhubu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fbx.gzhubu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sxc.jlsjyb.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://uzi.svipenyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://siz.ivvv.top

Java: int add(int a, int b) { return a + b; }
来源：http://wcx.yuanzhike.top

Go:   func add(a, b int) int
来源：http://fos.tanke756.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://idp.hammf.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ndl.hnxiangtu.top

[C14] 泛型函数
来源：http://rqb.yj20258888.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://klt.yanxiufei.cn

PHP:  // 无泛型
来源：http://vhn.52xcode.cn

JS:   // 无泛型
来源：http://tec.daria6918.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nfl.tianlin.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hwh.epnwcf.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gjr.tian-w.cn

Ruby: # 无泛型
来源：http://xhl.tianlin.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nkf.daria6918.cn

[C15] 解构 / 展开参数
来源：http://jhv.gogol.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xgw.tanke756.top

PHP:  [$a, $b] = $pair;
来源：http://wjs.zhongyouzk.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dxh.hfpthk.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yer.redwolf501.top

Java: // 无解构
来源：http://oxh.vqdsnc.cn

Go:   // 无解构
来源：http://grx.zhiwuduotai.top


<!-- 参考信息 -->