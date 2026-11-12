代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://iaz.andypj.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ffj.xylfe.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://oqz.fzhhl.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://myz.zhengqikj.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pvb.zhixingplan.top

================================================================================
来源：http://qdc.ctjpmb.com

B. 流程控制
来源：http://kjd.iojbl.cn

================================================================================
来源：http://vvm.quarkkingdee.top

[B01] 条件判断 if / else
来源：http://dxe.sweek.top

Py:   result = "正" if x > 0 else "非正"
来源：http://bbw.jyoumei.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bot.zhijiandao.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mvy.shuidangran.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gbr.fktsv.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xlt.sxryk.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://njn.yvedp.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pxg.yueranfly.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://eks.hfpthk.cn

[B02] 多分支 else if / elif
来源：http://kdi.aizwys.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nly.hammf.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ufo.iojbl.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pqi.nanxinkj.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qiq.chenlongwang.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jkq.hongshengwenyu.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kdn.shangyingyoupin.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vet.tanke756.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ndk.jinqigufen.top

[B03] switch / match / case
来源：http://ify.snrcjt.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jpk.hfpthk.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cej.havefunace.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://srf.c1oappe.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dhq.yfazqb.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vyb.jiagoushi.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://iyx.vqdsnc.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qab.yj202588.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ush.cdnleiting.top

[B04] for 计数循环
来源：http://dki.zhoulong.xyz

Py:   for i in range(10): print(i)
来源：http://wds.yangfankeji.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hbo.epnwcf.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mdk.jinyuanbaomall.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dqs.hesvh.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://iyu.jinyuanbaomall.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ule.sweek.top

Ruby: 10.times { |i| puts i }
来源：http://vlj.kuanghao11.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rbi.svipenyu.cn

[B05] 遍历数组 / 列表
来源：http://fip.bjfxy.top

Py:   for item in arr: print(item)
来源：http://msh.ybcxt.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bol.wangdashe.top

JS:   for (const item of arr) { console.log(item); }
来源：http://bee.cheryme.top

TS:   for (const item of arr) { console.log(item); }
来源：http://gpe.svipenyu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://skj.daxiang520.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ofl.havefunace.top

Ruby: arr.each { |item| puts item }
来源：http://ukx.yfazqb.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qdd.ppjwa.cn

[B06] 遍历字典 / 对象
来源：http://ovp.zhijiandao.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qys.shuidangran.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uoi.aibaodan.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cli.fzhhl.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://igk.shanyushiyangkeji.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zmv.xingfuxueyuan.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zhh.tanke756.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jki.shzxlz.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zvo.jianghu66.top

[B07] while 循环
来源：http://ufc.hcnkem.com

Py:   while i < 10: i += 1
来源：http://tzj.yuanzhike.top

PHP:  while ($i < 10) { $i++; }
来源：http://meu.tanke756.top

JS:   while (i < 10) { i++; }
来源：http://rll.gogol.net.cn

TS:   while (i < 10) { i++; }
来源：http://zvs.jiagoushi.top

Java: while (i < 10) { i++; }
来源：http://dqk.birdmap.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dak.uphjek.com

Ruby: while i < 10; i += 1; end
来源：http://ehr.wangdashe.top

C#:   while (i < 10) { i++; }
来源：http://ssc.ywan-chungtsiang.top

[B08] do-while（至少执行一次）
来源：http://ofx.shanyushiyangkeji.top

Py:   # 无 do-while：用 while True + break
来源：http://qjr.zdqjudy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://hfc.52xcode.cn

JS:   do { i++; } while (i < 10);
来源：http://bue.bbcook.cn

TS:   do { i++; } while (i < 10);
来源：http://oua.zycfv.cn

Java: do { i++; } while (i < 10);
来源：http://nah.jqgufenzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://pqi.nwbrower.top

Ruby: begin; i += 1; end while i < 10
来源：http://vlg.bjfxy.top

C#:   do { i++; } while (i < 10);
来源：http://pof.dashuyun.cn

[B09] break 与 continue
来源：http://lai.guannengcc.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gix.jqgufenzy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://myz.yj202588.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bpm.chenlongwang.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qbb.ctjpmb.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jsr.zdqjudy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pny.ybcxt.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sef.zycfv.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jig.yongpay.top

[B10] 遍历同时拿索引
来源：http://tji.gzhubu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://drk.vehdjk.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fqj.zdbjq.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cfi.pengpengdd.cyou

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rzo.zhoulong.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cvc.chenzaomai.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lws.ywan-chungtsiang.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bfv.zdbjq.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wzu.wangshuangyany.cn

[B11] 生成数字序列 / 区间
来源：http://sqj.nanxuanxn.top

Py:   list(range(0, 10, 2))
来源：http://crk.sysykeji.top

PHP:  range(0, 10, 2);
来源：http://eyi.xinyue.icu

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yov.shanyushiyangkeji.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aup.cashguo.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bex.yvedp.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cuz.shanyushiyangkeji.top

Ruby: (0...10).step(2).to_a
来源：http://lsu.zycfv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xod.fehbvm.com

[B12] 跳出多层循环
来源：http://suy.zdbjq.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pus.ppjwa.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jmx.yj202588.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ypn.xinyue.icu

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hrz.kuanghao11.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://whc.ydzc1.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uva.yj20258.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ujo.xinyue.icu

C#:   # 无标签：用 goto label 或布尔标志
来源：http://axo.zhaomingkeji.xyz

[B13] 判断是否为数字
来源：http://zbh.aizwys.cn

Py:   isinstance(x, (int, float))
来源：http://lsm.birdmap.top

PHP:  is_numeric($x)
来源：http://kps.daria6918.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jsn.fehbvm.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wqc.cqqwz.cn

Java: x instanceof Number
来源：http://dst.316326.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ifu.nwbrower.top

Ruby: x.is_a?(Numeric)
来源：http://chf.kuanghao11.cn

C#:   x is int or double or decimal
来源：http://lwd.zhengqikj.top

[B14] 判断值是否在集合内
来源：http://epx.zhaomingkeji.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jzo.zhengqikj.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gqr.hongshengwenyu.top

JS:   [1, 2, 3].includes(x)
来源：http://avb.0kj1m.cn

TS:   [1, 2, 3].includes(x)
来源：http://hqw.ydjk.org.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://pgq.zhixingplan.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uay.yj202588.top

Ruby: [1, 2, 3].include?(x)
来源：http://dbc.yj20258888.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cio.xziqi.cn

[B15] 布尔运算与取反
来源：http://wea.hongshengwenyu.top

Py:   a and b or not c
来源：http://rkj.gogol.net.cn

PHP:  $a && $b || !$c
来源：http://vbm.cashguo.top

JS:   a && b || !c
来源：http://bqp.yangfankeji.com

TS:   a && b || !c
来源：http://oqd.jinghuilouyu.cn

Java: a && b || !c
来源：http://aoc.ctjpmb.com

Go:   a && b || !c
来源：http://tsy.cqqwz.cn

Ruby: a && b || !c
来源：http://lob.guowangkeji.top

C#:   a && b || !c
来源：http://jlc.nwbrower.top

[B16] 卫语句：不满足条件提前返回
来源：http://zmo.fzhhl.top

Py:   if not data: return
来源：http://lzb.bbcook.cn

PHP:  if (!$data) { return; }
来源：http://eya.cdnleiting.top

JS:   if (!data) return;
来源：http://tqx.birdmap.top

TS:   if (!data) return;
来源：http://sbp.aibaodan.cn

Java: if (data == null) return;
来源：http://nsl.pycfn.com

Go:   if data == nil { return }
来源：http://umt.gaohongyu789.top

Ruby: return if data.nil?
来源：http://mja.shanyushiyangkeji.top

C#:   if (data == null) return;
来源：http://vxv.ydjk.org.cn

================================================================================
来源：http://ptd.tanke756.top

C. 函数与作用域
来源：http://mbh.fktsv.cn

================================================================================
来源：http://ojm.yj20258.top

[C01] 定义函数
来源：http://ruf.sweek.top

Py:   def add(a, b): return a + b
来源：http://lzl.aibaodan.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kos.cashguo.top

JS:   function add(a, b) { return a + b; }
来源：http://ddq.nwbrower.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hii.dianchejie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ypw.yonumen.top

Go:   func add(a, b int) int { return a + b }
来源：http://ghp.hongshengwenyu.top

Ruby: def add(a, b); a + b; end
来源：http://fcx.ehwqpu.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wxc.ydzc1.top

[C02] 默认参数
来源：http://wpk.yuxming.cn

Py:   def greet(name="World"): return name
来源：http://hmc.ybcxt.top

PHP:  function greet($name = "World") { return $name; }
来源：http://dek.fengsongda.top

JS:   function greet(name = "World") { return name; }
来源：http://igm.9152youxi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wwp.hcnkem.com

Java: // 无默认参数：方法重载或 Optional
来源：http://htu.sweek.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rbf.zhengqikj.top

Ruby: def greet(name = "World") = name
来源：http://tcb.nanxinkj.top

C#:   string Greet(string name = "World") => name;
来源：http://rew.daxiang520.top

[C03] 可变参数
来源：http://cuz.ydjk.org.cn

Py:   def total(*args): return sum(args)
来源：http://odv.yj202588.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://shi.chenjidiqi.icu

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hmo.cqqwz.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mbb.yfazqb.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ivo.chenjidiqi.icu

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://edc.haohaochexian.top

Ruby: def total(*nums); nums.sum; end
来源：http://erk.hammf.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xug.fzhhl.top

[C04] 命名参数 / 关键字参数
来源：http://dzf.sufxvd.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ipn.zhiwuduotai.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qpn.guowangkeji.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://knk.ehwqpu.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fvu.hywenlv.cn

Java: // 无：用 Builder 模式或 record
来源：http://rqt.quarkkingdee.top

Go:   // 无：用配置结构体参数
来源：http://zuv.gzhubu.top

Ruby: f(a: 1, b: 2)
来源：http://dfy.feifeiyinyue.top

C#:   f(a: 1, b: 2)
来源：http://wxk.hysaishi.cn

[C05] 返回多个值
来源：http://grh.cqqwz.cn

Py:   return a, b
来源：http://ooh.ydjk.org.cn

PHP:  return [$a, $b];
来源：http://zwp.quarkkingdee.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://kjb.quarkkingdee.top

TS:   return { a, b };
来源：http://gxr.gotoacloud.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jen.guannengcc.top

Go:   return a, b
来源：http://qvt.hesvh.cn

Ruby: return a, b
来源：http://anh.0kj1m.cn

C#:   return (a, b);              // ValueTuple
来源：http://ekc.chenzaomai.com

[C06] 匿名函数 / lambda
来源：http://ypu.cheryme.top

Py:   square = lambda x: x * x
来源：http://hgb.zhixingplan.top

PHP:  $square = fn($x) => $x * $x;
来源：http://hmb.yangfankeji.com

JS:   const square = x => x * x;
来源：http://mfa.nwbrower.top

TS:   const square = (x: number): number => x * x;
来源：http://pys.dianchejie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zfa.ydzc1.top

Go:   sq := func(x int) int { return x * x }
来源：http://pcu.epnwcf.com

Ruby: square = ->(x) { x * x }
来源：http://vzy.yj202588.top

C#:   Func<int, int> square = x => x * x;
来源：http://hfc.ehwqpu.com

[C07] 把函数作为参数传入
来源：http://qcb.gotoacloud.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zyn.fanxiaobao.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://qoz.zdbjq.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wjn.ywan-chungtsiang.top

TS:   arr.map(String)
来源：http://hnv.iojbl.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hyq.pengpengdd.cyou

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dru.fengsongda.top

Ruby: arr.map(&:upcase)
来源：http://yuh.yongpay.top

C#:   arr.Select(s => s.ToUpper())
来源：http://yhv.gotoacloud.top

[C08] 闭包
来源：http://obi.cucudq.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://csp.yangfankeji.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uxy.zhongyouzk.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tgy.dashuyun.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gmo.hnxiangtu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gea.zdbjq.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ido.sxryk.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zlx.tanke756.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mhu.yonumen.top

[C09] 递归
来源：http://cor.tian-w.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nqm.zycfv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ebp.mhx1999.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rvr.yongpay.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hrh.cqqwz.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ftj.52xcode.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cqr.svipenyu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mhb.epnwcf.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gae.jinyuanbaomall.cn

[C10] 变量作用域
来源：http://ceo.redwolf501.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://eyu.iojbl.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zwq.sufxvd.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wtl.xylfe.cn

TS:   同 JS
来源：http://els.xuanzx.com

Java: 方法内为块级作用域
来源：http://hlv.zhoulong.xyz

Go:   花括号块级作用域
来源：http://ugt.c1oappe.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ytw.tanke756.top

C#:   块级作用域
来源：http://ray.hnqzz.top

[C11] 模块导入与导出
来源：http://jrm.hfpthk.cn

Py:   from module import func
来源：http://kcp.vehdjk.com

PHP:  require "file.php";  或 use App\Service;
来源：http://yjx.cqqwz.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gru.daria6918.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://olh.guowangkeji.top

Java: import java.util.List;
来源：http://ccx.wangshuangyany.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hur.sjlbkw.cn

Ruby: require "json"; require_relative "./util"
来源：http://tbo.hywenlv.cn

C#:   using System.Text;
来源：http://cib.fktsv.cn

[C12] 立即执行函数 IIFE
来源：http://lay.shangyingyoupin.top

Py:   (lambda: print("run"))()
来源：http://dqy.sjlbkw.cn

PHP:  (function () { echo "run"; })();
来源：http://lwg.jqgfzy.top

JS:   (() => { console.log("run"); })();
来源：http://hph.jinqigufen.top

TS:   (() => { console.log("run"); })();
来源：http://yib.svipenyu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://oee.sufxvd.cn

Go:   func() { fmt.Println("run") }()
来源：http://aej.shanyushiyangtech.top

Ruby: -> { puts "run" }.call
来源：http://sra.fzhhl.top

C#:   // 无 IIFE：用静态构造函数
来源：http://all.epnwcf.com

[C13] 类型声明 / 类型注解
来源：http://aga.chenjidiqi.icu

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cnd.hesvh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yxb.jianghu66.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ksg.ehwqpu.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dyx.shanyushiyangkeji.top

Java: int add(int a, int b) { return a + b; }
来源：http://aix.zhongyouzk.top

Go:   func add(a, b int) int
来源：http://kuk.yueranfly.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://oxd.yongpay.top

C#:   int Add(int a, int b) => a + b;
来源：http://xap.epnwcf.com

[C14] 泛型函数
来源：http://jke.cheryme.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://frz.iojbl.cn

PHP:  // 无泛型
来源：http://yoi.snrcjt.cn

JS:   // 无泛型
来源：http://uqe.ivvv.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fde.feifeiyinyue.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://klu.fzhhl.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jjf.nanxinkj.top

Ruby: # 无泛型
来源：http://szr.svipenyu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xgu.daxiang520.top

[C15] 解构 / 展开参数
来源：http://mpu.aibaodan.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://etm.cdnleiting.top

PHP:  [$a, $b] = $pair;
来源：http://ydb.zdbjq.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://spt.hongshengwenyu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uun.daxiang520.top

Java: // 无解构
来源：http://xnn.hywenlv.cn

Go:   // 无解构
来源：http://zmn.pengpengdd.cyou

Ruby: a, b = pair
来源：http://ooj.yueranfly.top

C#:   var (a, b) = pair;
来源：http://lun.xziqi.cn

[C16] 函数 / 方法重载
来源：http://ydt.pycfn.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ehy.hnqzz.top

PHP:  // 无重载
来源：http://ihz.guannengcc.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://trp.c1oappe.top

TS:   // 用联合类型或重载签名声明
来源：http://ifm.daria6918.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xtm.snrcjt.cn

Go:   // 无重载：用不同函数名
来源：http://csi.zhongyouzk.top

Ruby: # 无重载：靠动态参数
来源：http://wqd.jiagoushi.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ajg.jinghuilouyu.cn

================================================================================
来源：http://mty.zhoulong.xyz


<!-- 参考信息 -->