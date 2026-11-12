代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qja.daxiang520.top

================================================================================
来源：http://kst.0kj1m.cn

B. 流程控制
来源：http://uuj.jiagoushi.top

================================================================================
来源：http://dla.gzhubu.top

[B01] 条件判断 if / else
来源：http://fdr.tanke756.top

Py:   result = "正" if x > 0 else "非正"
来源：http://eop.ctjpmb.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://egq.shzxlz.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dcq.xylfe.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uep.pycfn.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://sua.fktsv.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://epx.vehdjk.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qno.hnqzz.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vdm.sxryk.cn

[B02] 多分支 else if / elif
来源：http://imm.cdnleiting.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dxp.shangyingyoupin.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qot.uphjek.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mvg.daria6918.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jzu.0kj1m.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zuk.nanxinkj.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dwb.daxiang520.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xbz.chenlongwang.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://unf.yj202588.top

[B03] switch / match / case
来源：http://ott.hywenlv.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ibn.yanxiufei.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gkh.chenjidiqi.icu

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dag.shzxlz.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gky.hammf.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vhj.hywenlv.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fxi.yuxming.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xhy.aizwys.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://otl.9152youxi.cn

[B04] for 计数循环
来源：http://qcn.andypj.xyz

Py:   for i in range(10): print(i)
来源：http://qqu.zhaomingkeji.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pnn.pycfn.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iuu.svipenyu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ebw.yuanzhike.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zvv.nwbrower.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ovf.pengpengdd.cyou

Ruby: 10.times { |i| puts i }
来源：http://ipm.jianghu66.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://iog.zhongyouzk.top

[B05] 遍历数组 / 列表
来源：http://oli.gaohongyu789.top

Py:   for item in arr: print(item)
来源：http://tyb.havefunace.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hqo.sysykeji.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ody.jinyuanbaomall.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://hsy.zhoulong.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://tmq.zhiwuduotai.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dbv.bjfxy.top

Ruby: arr.each { |item| puts item }
来源：http://inb.nanxuanxn.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tzf.redwolf501.top

[B06] 遍历字典 / 对象
来源：http://phs.yj202588.top

Py:   for k, v in d.items(): print(k, v)
来源：http://eeo.cdnleiting.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bic.epnwcf.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mdf.ybcxt.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jsa.cheryme.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lac.jiagoushi.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wsk.zhengqikj.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fzm.sufxvd.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bna.mhx1999.top

[B07] while 循环
来源：http://zvq.hfpthk.cn

Py:   while i < 10: i += 1
来源：http://vxp.cashguo.top

PHP:  while ($i < 10) { $i++; }
来源：http://nss.jiagoushi.top

JS:   while (i < 10) { i++; }
来源：http://yuw.jqgufenzy.top

TS:   while (i < 10) { i++; }
来源：http://qhc.ehwqpu.com

Java: while (i < 10) { i++; }
来源：http://fws.c1oappe.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jsk.fanxiaobao.xyz

Ruby: while i < 10; i += 1; end
来源：http://tzo.gogol.net.cn

C#:   while (i < 10) { i++; }
来源：http://gez.9152youxi.cn

[B08] do-while（至少执行一次）
来源：http://kbn.ivvv.top

Py:   # 无 do-while：用 while True + break
来源：http://enf.zhongyouzk.top

PHP:  do { $i++; } while ($i < 10);
来源：http://gsf.havefunace.top

JS:   do { i++; } while (i < 10);
来源：http://qgm.xuetiantiany.cn

TS:   do { i++; } while (i < 10);
来源：http://uxg.yvedp.cn

Java: do { i++; } while (i < 10);
来源：http://tyy.jinqigfzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://pxb.cheryme.top

Ruby: begin; i += 1; end while i < 10
来源：http://hon.ctjpmb.com

C#:   do { i++; } while (i < 10);
来源：http://nkf.hongshengwenyu.top

[B09] break 与 continue
来源：http://oiu.hywenlv.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zhl.havefunace.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wvb.yfazqb.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cnz.nanxuanxn.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gmi.ehwqpu.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cfc.jyoumei.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ltz.yongpay.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qzd.bjfxy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dqt.zhiwuduotai.top

[B10] 遍历同时拿索引
来源：http://dhs.nwbrower.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lou.gzhubu.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uxq.nanxinkj.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kam.epnwcf.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://caj.cdnleiting.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fdd.chenzaomai.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qyl.shangyingyoupin.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ujg.pengpengdd.cyou

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nje.zhiwuduotai.top

[B11] 生成数字序列 / 区间
来源：http://fdk.cashguo.top

Py:   list(range(0, 10, 2))
来源：http://uvz.shanyushiyangtech.top

PHP:  range(0, 10, 2);
来源：http://nef.yangfankeji.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bsl.jqgufenzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hjo.c1oappe.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pzk.hysaishi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qng.chenlongwang.top

Ruby: (0...10).step(2).to_a
来源：http://gzp.c1oappe.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mps.xylfe.cn

[B12] 跳出多层循环
来源：http://uhl.yongpay.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://mft.shzxlz.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://htp.zhixingplan.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kxa.daria6918.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dii.cdnleiting.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zje.haohaochexian.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://eqq.zhijiandao.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ixd.ywan-chungtsiang.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kxy.jiagoushi.top

[B13] 判断是否为数字
来源：http://mia.zhongyouzk.top

Py:   isinstance(x, (int, float))
来源：http://smj.snrcjt.cn

PHP:  is_numeric($x)
来源：http://nib.chenlongwang.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bry.yj20258888.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lei.nanxinkj.top

Java: x instanceof Number
来源：http://nxr.zhengqikj.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qsd.xinyue.icu

Ruby: x.is_a?(Numeric)
来源：http://fgg.yfazqb.com

C#:   x is int or double or decimal
来源：http://cxb.mhx1999.top

[B14] 判断值是否在集合内
来源：http://hea.aibaodan.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xoo.uphjek.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://omb.chenjidiqi.icu

JS:   [1, 2, 3].includes(x)
来源：http://tgh.gogol.net.cn

TS:   [1, 2, 3].includes(x)
来源：http://yxt.zhaomingkeji.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://qjf.smart0.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jwh.hongshengwenyu.top

Ruby: [1, 2, 3].include?(x)
来源：http://noz.ydjk.org.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wmx.bjfxy.top

[B15] 布尔运算与取反
来源：http://gau.ctjpmb.com

Py:   a and b or not c
来源：http://uxq.ppjwa.cn

PHP:  $a && $b || !$c
来源：http://rzl.chenzaomai.com

JS:   a && b || !c
来源：http://vny.shuidangran.top

TS:   a && b || !c
来源：http://dge.dashuyun.cn

Java: a && b || !c
来源：http://ndt.pycfn.com

Go:   a && b || !c
来源：http://uya.ctjpmb.com

Ruby: a && b || !c
来源：http://uts.xuetiantiany.cn

C#:   a && b || !c
来源：http://qdo.mhx1999.top

[B16] 卫语句：不满足条件提前返回
来源：http://wlf.ppjwa.cn

Py:   if not data: return
来源：http://rwb.havefunace.top

PHP:  if (!$data) { return; }
来源：http://erq.yangfankeji.com

JS:   if (!data) return;
来源：http://yac.hfpthk.cn

TS:   if (!data) return;
来源：http://gmo.zdqjudy.top

Java: if (data == null) return;
来源：http://zfj.yangfankeji.com

Go:   if data == nil { return }
来源：http://nor.andypj.xyz

Ruby: return if data.nil?
来源：http://nau.xingfuxueyuan.xyz

C#:   if (data == null) return;
来源：http://dkb.xinyue.icu

================================================================================
来源：http://wxg.ydzc1.top

C. 函数与作用域
来源：http://yty.jinqigfzy.top

================================================================================
来源：http://fiq.yj202588.top

[C01] 定义函数
来源：http://dem.cqqwz.cn

Py:   def add(a, b): return a + b
来源：http://bhr.xuanzx.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://crg.gzhubu.top

JS:   function add(a, b) { return a + b; }
来源：http://kwj.sweek.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xhn.wangshuangyany.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lmg.daria6918.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hvf.aizwys.cn

Ruby: def add(a, b); a + b; end
来源：http://uhy.ppjwa.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xcy.ppjwa.cn

[C02] 默认参数
来源：http://uiv.yj20258888.top

Py:   def greet(name="World"): return name
来源：http://ihp.jqgufenzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://buu.tian-w.cn

JS:   function greet(name = "World") { return name; }
来源：http://hwt.cqqwz.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://dcx.guannengcc.top

Java: // 无默认参数：方法重载或 Optional
来源：http://xxp.ydzc1.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gdv.hfpthk.cn

Ruby: def greet(name = "World") = name
来源：http://zfg.iojbl.cn

C#:   string Greet(string name = "World") => name;
来源：http://cpd.andypj.xyz

[C03] 可变参数
来源：http://tfa.hnqzz.top

Py:   def total(*args): return sum(args)
来源：http://lvq.zdbjq.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ose.hammf.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lnq.xinyue.icu

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://squ.cashguo.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bhc.daxiang520.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yhb.uphjek.com

Ruby: def total(*nums); nums.sum; end
来源：http://jqv.epnwcf.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://thv.ivvv.top

[C04] 命名参数 / 关键字参数
来源：http://wph.xingfuxueyuan.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://his.sufxvd.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://erw.nanxinkj.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vdx.bjfxy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bbx.pengpengdd.cyou

Java: // 无：用 Builder 模式或 record
来源：http://xdw.tarul.cn

Go:   // 无：用配置结构体参数
来源：http://fyy.iojbl.cn

Ruby: f(a: 1, b: 2)
来源：http://cqj.zdqjudy.top

C#:   f(a: 1, b: 2)
来源：http://xba.hfpthk.cn

[C05] 返回多个值
来源：http://eaj.jinqigufen.top

Py:   return a, b
来源：http://wnu.uphjek.com

PHP:  return [$a, $b];
来源：http://gne.ppjwa.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://lbk.ehwqpu.com

TS:   return { a, b };
来源：http://fcz.yongpay.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dkj.52xcode.cn

Go:   return a, b
来源：http://izl.yj20258888.top

Ruby: return a, b
来源：http://fzt.daxiang520.top

C#:   return (a, b);              // ValueTuple
来源：http://sbx.cheryme.top

[C06] 匿名函数 / lambda
来源：http://zlv.tanke756.top

Py:   square = lambda x: x * x
来源：http://gcl.hcnkem.com

PHP:  $square = fn($x) => $x * $x;
来源：http://xjf.hnxiangtu.top

JS:   const square = x => x * x;
来源：http://dug.cucudq.cn

TS:   const square = (x: number): number => x * x;
来源：http://bhh.tianlin.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bvo.zhijiandao.cn

Go:   sq := func(x int) int { return x * x }
来源：http://nun.fzhhl.top

Ruby: square = ->(x) { x * x }
来源：http://ssp.chenlongwang.top

C#:   Func<int, int> square = x => x * x;
来源：http://oxt.hnxiangtu.top

[C07] 把函数作为参数传入
来源：http://bru.sweek.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zov.xuanzx.com

PHP:  array_map("strtoupper", $arr);
来源：http://lca.birdmap.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ezc.zhaomingkeji.xyz

TS:   arr.map(String)
来源：http://eii.cqqwz.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://efk.haohaochexian.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kut.yj20258.top

Ruby: arr.map(&:upcase)
来源：http://rdn.jlsjyb.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://geh.wangshuangyany.cn

[C08] 闭包
来源：http://hva.andypj.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rog.gogol.net.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://oii.andypj.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sdd.zycfv.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://edv.aizwys.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://htl.tarul.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wyz.chenlongwang.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wkk.nwbrower.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xac.xuanzx.com

[C09] 递归
来源：http://fiv.chenlongwang.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://aty.daxiang520.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yqy.zycfv.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gpa.chenlongwang.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pjs.bbcook.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yfc.gotoacloud.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wfd.jinghuilouyu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ixp.nanxuanxn.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gob.sjlbkw.cn

[C10] 变量作用域
来源：http://yob.jinghuilouyu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lht.jiagoushi.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mmz.cqqwz.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ewd.zdqjudy.top

TS:   同 JS
来源：http://hhf.daria6918.cn

Java: 方法内为块级作用域
来源：http://gmp.xuetiantiany.cn

Go:   花括号块级作用域
来源：http://upw.shzxlz.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://faw.sysykeji.top

C#:   块级作用域
来源：http://lur.uphjek.com

[C11] 模块导入与导出
来源：http://iyl.yuanzhike.top

Py:   from module import func
来源：http://ymm.nwbrower.top

PHP:  require "file.php";  或 use App\Service;
来源：http://bxh.zhaomingkeji.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://umy.wangshuangyany.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lrc.iojbl.cn

Java: import java.util.List;
来源：http://xbb.andypj.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tzr.redwolf501.top

Ruby: require "json"; require_relative "./util"
来源：http://lmd.mhx1999.top

C#:   using System.Text;
来源：http://spm.zhengqikj.top

[C12] 立即执行函数 IIFE
来源：http://jmb.kuanghao11.cn

Py:   (lambda: print("run"))()
来源：http://pez.ydzc1.top

PHP:  (function () { echo "run"; })();
来源：http://agy.quarkkingdee.top

JS:   (() => { console.log("run"); })();
来源：http://obq.daria6918.cn

TS:   (() => { console.log("run"); })();
来源：http://kmb.snrcjt.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rbv.yfazqb.com

Go:   func() { fmt.Println("run") }()
来源：http://dzs.redwolf501.top

Ruby: -> { puts "run" }.call
来源：http://mes.guannengcc.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ibg.yuxming.cn

[C13] 类型声明 / 类型注解
来源：http://wrg.yvedp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lrf.zhijiandao.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vle.hongshengwenyu.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vrk.hysaishi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blk.nwbrower.top

Java: int add(int a, int b) { return a + b; }
来源：http://bei.mhx1999.top

Go:   func add(a, b int) int
来源：http://lde.ppjwa.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://koh.cqqwz.cn

C#:   int Add(int a, int b) => a + b;
来源：http://lsu.daxiang520.top

[C14] 泛型函数
来源：http://nfn.tian-w.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jtv.jinghuilouyu.cn

PHP:  // 无泛型
来源：http://tef.nwbrower.top

JS:   // 无泛型
来源：http://qoc.jqgfzy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://squ.hammf.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ogk.shzxlz.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ydu.havefunace.top

Ruby: # 无泛型
来源：http://upw.jinqigufen.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gdr.gogol.net.cn

[C15] 解构 / 展开参数
来源：http://zwb.zhiwuduotai.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://oag.zhiwuduotai.top

PHP:  [$a, $b] = $pair;
来源：http://cle.fengsongda.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://glf.yangfankeji.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ywz.yj20258888.top

Java: // 无解构
来源：http://ohp.gogol.net.cn

Go:   // 无解构
来源：http://ivj.hcnkem.com

Ruby: a, b = pair
来源：http://qqg.yj20258888.top

C#:   var (a, b) = pair;
来源：http://lqh.svipenyu.cn

[C16] 函数 / 方法重载
来源：http://stc.cheryme.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jcm.tarul.cn

PHP:  // 无重载
来源：http://gjr.mhx1999.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://bqo.xylfe.cn

TS:   // 用联合类型或重载签名声明
来源：http://ljd.yj20258888.top

Java: void f(int a) {}  void f(String a) {}
来源：http://pnt.xinyue.icu

Go:   // 无重载：用不同函数名
来源：http://xqd.yueranfly.top

Ruby: # 无重载：靠动态参数
来源：http://xql.cucudq.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://etf.jinghuilouyu.cn

================================================================================
来源：http://xrr.tianlin.xyz

D. 数组 / 列表 / 集合
来源：http://bqj.fehbvm.com

================================================================================
来源：http://xdb.xuanzx.com

[D01] 创建数组 / 列表
来源：http://dfy.haohaochexian.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://jhn.52xcode.cn


<!-- 参考信息 -->