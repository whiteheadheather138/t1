代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qfs.nanxinkj.top

================================================================================
来源：http://efu.vqdsnc.cn

B. 流程控制
来源：http://xux.fzhhl.top

================================================================================
来源：http://ewf.jianghu66.top

[B01] 条件判断 if / else
来源：http://ezn.smart0.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://dxt.yj202588.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://opg.jianghu66.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xlk.xuetiantiany.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bgo.fehbvm.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://tlu.ybcxt.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ujr.andypj.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cei.zhiwuduotai.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vfg.hywenlv.cn

[B02] 多分支 else if / elif
来源：http://vgh.zhongyouzk.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://buz.shanyushiyangkeji.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://uux.quarkkingdee.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tkf.xuetiantiany.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dgg.redwolf501.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gsh.jqgfzy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fat.guannengcc.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fbn.hcnkem.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pef.dashuyun.cn

[B03] switch / match / case
来源：http://hxg.zdqjudy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://spq.52xcode.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ird.shuidangran.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gai.zhijiandao.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ewa.zycfv.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gng.c1oappe.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kvj.gogol.net.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kkh.sufxvd.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lcx.aizwys.cn

[B04] for 计数循环
来源：http://lai.dashuyun.cn

Py:   for i in range(10): print(i)
来源：http://fcx.dashuyun.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tcb.epnwcf.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://psk.daxiang520.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tqc.shuidangran.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qkl.yanxiufei.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yiz.shanyushiyangkeji.top

Ruby: 10.times { |i| puts i }
来源：http://jvn.redwolf501.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ymw.hammf.cn

[B05] 遍历数组 / 列表
来源：http://nyh.cucudq.cn

Py:   for item in arr: print(item)
来源：http://gcf.yonumen.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cmb.hesvh.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mcy.9152youxi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://nly.zdbjq.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gmb.snrcjt.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rrj.cucudq.cn

Ruby: arr.each { |item| puts item }
来源：http://pzv.yvedp.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uoh.iojbl.cn

[B06] 遍历字典 / 对象
来源：http://fxj.zhixingplan.top

Py:   for k, v in d.items(): print(k, v)
来源：http://qvc.chenjidiqi.icu

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nmk.yuanzhike.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pxa.andypj.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://axw.chenjidiqi.icu

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dox.ywan-chungtsiang.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qzu.316326.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://eof.ehwqpu.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lfz.uphjek.com

[B07] while 循环
来源：http://vky.chenlongwang.top

Py:   while i < 10: i += 1
来源：http://fbz.shanyushiyangtech.top

PHP:  while ($i < 10) { $i++; }
来源：http://xpj.zhoulong.xyz

JS:   while (i < 10) { i++; }
来源：http://isi.cheryme.top

TS:   while (i < 10) { i++; }
来源：http://xfe.zhengqikj.top

Java: while (i < 10) { i++; }
来源：http://vwo.smart0.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ovf.ivvv.top

Ruby: while i < 10; i += 1; end
来源：http://nag.fktsv.cn

C#:   while (i < 10) { i++; }
来源：http://jar.ydjk.org.cn

[B08] do-while（至少执行一次）
来源：http://hhl.zhoulong.xyz

Py:   # 无 do-while：用 while True + break
来源：http://xcq.nanxuanxn.top

PHP:  do { $i++; } while ($i < 10);
来源：http://mkn.fzhhl.top

JS:   do { i++; } while (i < 10);
来源：http://ymt.chenlongwang.top

TS:   do { i++; } while (i < 10);
来源：http://gzr.ywan-chungtsiang.top

Java: do { i++; } while (i < 10);
来源：http://qnk.ctjpmb.com

Go:   for { i++; if i >= 10 { break } }
来源：http://wvh.pycfn.com

Ruby: begin; i += 1; end while i < 10
来源：http://dtu.fehbvm.com

C#:   do { i++; } while (i < 10);
来源：http://dkh.havefunace.top

[B09] break 与 continue
来源：http://kij.zdqjudy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://teb.52xcode.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lzi.jqgufenzy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mcv.yongpay.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dst.c1oappe.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uqt.wangdashe.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://aml.zhixingplan.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xca.zhaomingkeji.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fgw.yuanzhike.top

[B10] 遍历同时拿索引
来源：http://uhg.yongpay.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xnk.yj20258.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ixf.c1oappe.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://msd.zhaomingkeji.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zih.epnwcf.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://syt.jqgfzy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kbx.zdqjudy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://udc.haohaochexian.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pwv.hongshengwenyu.top

[B11] 生成数字序列 / 区间
来源：http://wef.yueranfly.top

Py:   list(range(0, 10, 2))
来源：http://eos.redwolf501.top

PHP:  range(0, 10, 2);
来源：http://ghy.sysykeji.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tax.52xcode.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sul.kuanghao11.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://spf.xingfuxueyuan.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://esh.hnxiangtu.top

Ruby: (0...10).step(2).to_a
来源：http://kqn.hongshengwenyu.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tmz.zdqjudy.top

[B12] 跳出多层循环
来源：http://cup.9152youxi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://nci.gogol.net.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vyg.jlsjyb.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ojg.ydjk.org.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://owx.svipenyu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://exr.yueranfly.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ccq.nanxuanxn.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cec.havefunace.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://voa.hysaishi.cn

[B13] 判断是否为数字
来源：http://fpq.jinghuilouyu.cn

Py:   isinstance(x, (int, float))
来源：http://gvo.wangshuangyany.cn

PHP:  is_numeric($x)
来源：http://nng.zhaomingkeji.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://den.xinyue.icu

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tlv.iojbl.cn

Java: x instanceof Number
来源：http://ewm.jyoumei.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xte.0kj1m.cn

Ruby: x.is_a?(Numeric)
来源：http://ahr.jinyuanbaomall.cn

C#:   x is int or double or decimal
来源：http://wua.yj202588.top

[B14] 判断值是否在集合内
来源：http://mxu.shangyingyoupin.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pye.birdmap.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yam.jlsjyb.cn

JS:   [1, 2, 3].includes(x)
来源：http://cxp.guowangkeji.top

TS:   [1, 2, 3].includes(x)
来源：http://zoi.ctjpmb.com

Java: List.of(1, 2, 3).contains(x)
来源：http://scj.cashguo.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pak.yj20258.top

Ruby: [1, 2, 3].include?(x)
来源：http://qtr.fanxiaobao.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gxo.tianlin.xyz

[B15] 布尔运算与取反
来源：http://fsv.ydzc1.top

Py:   a and b or not c
来源：http://uvu.havefunace.top

PHP:  $a && $b || !$c
来源：http://jqi.pengpengdd.cyou

JS:   a && b || !c
来源：http://zzr.daxiang520.top

TS:   a && b || !c
来源：http://hdz.daxiang520.top

Java: a && b || !c
来源：http://bqh.yonumen.top

Go:   a && b || !c
来源：http://dhq.jinqigfzy.top

Ruby: a && b || !c
来源：http://zjg.andypj.xyz

C#:   a && b || !c
来源：http://mip.xinyue.icu

[B16] 卫语句：不满足条件提前返回
来源：http://wzy.zhaomingkeji.xyz

Py:   if not data: return
来源：http://qnr.yuxming.cn

PHP:  if (!$data) { return; }
来源：http://kbt.svipenyu.cn

JS:   if (!data) return;
来源：http://qzu.jqgufenzy.top

TS:   if (!data) return;
来源：http://wad.sxryk.cn

Java: if (data == null) return;
来源：http://hzi.haohaochexian.top

Go:   if data == nil { return }
来源：http://edn.yj20258.top

Ruby: return if data.nil?
来源：http://mpb.52xcode.cn

C#:   if (data == null) return;
来源：http://onk.fanxiaobao.xyz

================================================================================
来源：http://ont.uphjek.com

C. 函数与作用域
来源：http://slw.hnxiangtu.top

================================================================================
来源：http://iwv.gzhubu.top

[C01] 定义函数
来源：http://vue.bbcook.cn

Py:   def add(a, b): return a + b
来源：http://ehw.yuxming.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://boz.feifeiyinyue.top

JS:   function add(a, b) { return a + b; }
来源：http://fya.bjfxy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nnl.jqgfzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://uoj.yanxiufei.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mbq.9152youxi.cn

Ruby: def add(a, b); a + b; end
来源：http://teb.zhengqikj.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cxo.tanke756.top

[C02] 默认参数
来源：http://dxz.cucudq.cn

Py:   def greet(name="World"): return name
来源：http://yry.redwolf501.top

PHP:  function greet($name = "World") { return $name; }
来源：http://znl.jlsjyb.cn

JS:   function greet(name = "World") { return name; }
来源：http://wjc.yfazqb.com

TS:   function greet(name: string = "World") { return name; }
来源：http://myw.xuanzx.com

Java: // 无默认参数：方法重载或 Optional
来源：http://ser.jlsjyb.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://oee.ctjpmb.com

Ruby: def greet(name = "World") = name
来源：http://pab.wangshuangyany.cn

C#:   string Greet(string name = "World") => name;
来源：http://xkw.aizwys.cn

[C03] 可变参数
来源：http://kdt.cashguo.top

Py:   def total(*args): return sum(args)
来源：http://ntd.yonumen.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://oak.ehwqpu.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nkg.9152youxi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rsk.ydjk.org.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://myg.bjfxy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://svd.xuanzx.com

Ruby: def total(*nums); nums.sum; end
来源：http://cqv.hongshengwenyu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ucg.xuanzx.com

[C04] 命名参数 / 关键字参数
来源：http://hyd.fanxiaobao.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bhx.jlsjyb.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rzd.ybcxt.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qji.meibo888.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gnd.ydzc1.top

Java: // 无：用 Builder 模式或 record
来源：http://liw.zhixingplan.top

Go:   // 无：用配置结构体参数
来源：http://par.tanke756.top

Ruby: f(a: 1, b: 2)
来源：http://euu.jlsjyb.cn

C#:   f(a: 1, b: 2)
来源：http://vef.smart0.xyz

[C05] 返回多个值
来源：http://oxb.uphjek.com

Py:   return a, b
来源：http://kvi.cqqwz.cn

PHP:  return [$a, $b];
来源：http://roq.yueranfly.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://gti.ppjwa.cn

TS:   return { a, b };
来源：http://our.birdmap.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bqx.ivvv.top

Go:   return a, b
来源：http://zor.zhijiandao.cn

Ruby: return a, b
来源：http://zgr.yueranfly.top

C#:   return (a, b);              // ValueTuple
来源：http://ufk.bbcook.cn

[C06] 匿名函数 / lambda
来源：http://yne.316326.xyz

Py:   square = lambda x: x * x
来源：http://amu.nwbrower.top

PHP:  $square = fn($x) => $x * $x;
来源：http://vms.hesvh.cn

JS:   const square = x => x * x;
来源：http://bnd.birdmap.top

TS:   const square = (x: number): number => x * x;
来源：http://fwc.hfpthk.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cwc.hcnkem.com

Go:   sq := func(x int) int { return x * x }
来源：http://qnf.yueranfly.top

Ruby: square = ->(x) { x * x }
来源：http://vfp.vehdjk.com

C#:   Func<int, int> square = x => x * x;
来源：http://pif.wangdashe.top

[C07] 把函数作为参数传入
来源：http://dmx.fehbvm.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://otd.yongpay.top

PHP:  array_map("strtoupper", $arr);
来源：http://gxr.yanxiufei.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://szv.jinqigufen.top

TS:   arr.map(String)
来源：http://eui.tianlin.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kzx.dashuyun.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://txm.nanxuanxn.top

Ruby: arr.map(&:upcase)
来源：http://ekk.zhijiandao.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xhw.pycfn.com

[C08] 闭包
来源：http://tmx.hfpthk.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dnd.0kj1m.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fnn.9152youxi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yfv.tianlin.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://umk.sxryk.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kqw.yongpay.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kqm.havefunace.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cah.pengpengdd.cyou

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wph.xingfuxueyuan.xyz

[C09] 递归
来源：http://dag.shanyushiyangkeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://idv.vehdjk.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xgt.fehbvm.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qmc.guannengcc.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vdj.guowangkeji.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pxj.bbcook.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://igp.meibo888.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nwj.yj202588.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zwk.hnxiangtu.top

[C10] 变量作用域
来源：http://unw.9152youxi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://btt.ctjpmb.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vgs.cdnleiting.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fsd.yvedp.cn

TS:   同 JS
来源：http://snz.vqdsnc.cn

Java: 方法内为块级作用域
来源：http://qam.chenzaomai.com

Go:   花括号块级作用域
来源：http://qok.cucudq.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ioz.yj202588.top

C#:   块级作用域
来源：http://lnj.zhiwuduotai.top

[C11] 模块导入与导出
来源：http://hds.zhoulong.xyz

Py:   from module import func
来源：http://nrs.wangdashe.top

PHP:  require "file.php";  或 use App\Service;
来源：http://nxo.ppjwa.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://sio.yanxiufei.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tcs.fehbvm.com

Java: import java.util.List;
来源：http://ujm.c1oappe.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kok.redwolf501.top

Ruby: require "json"; require_relative "./util"
来源：http://jif.vqdsnc.cn

C#:   using System.Text;
来源：http://iaa.hcnkem.com

[C12] 立即执行函数 IIFE
来源：http://hgt.feifeiyinyue.top

Py:   (lambda: print("run"))()
来源：http://ypk.guowangkeji.top

PHP:  (function () { echo "run"; })();
来源：http://hen.jinyuanbaomall.cn

JS:   (() => { console.log("run"); })();
来源：http://nmi.fanxiaobao.xyz

TS:   (() => { console.log("run"); })();
来源：http://yjm.jinghuilouyu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jvc.zdbjq.cn

Go:   func() { fmt.Println("run") }()
来源：http://vwd.jinqigufen.top

Ruby: -> { puts "run" }.call
来源：http://jew.gotoacloud.top

C#:   // 无 IIFE：用静态构造函数
来源：http://rfo.zhengqikj.top

[C13] 类型声明 / 类型注解
来源：http://qry.xuanzx.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hqo.hywenlv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aii.fehbvm.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yfz.yonumen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hax.bjfxy.top

Java: int add(int a, int b) { return a + b; }
来源：http://jig.nwbrower.top

Go:   func add(a, b int) int
来源：http://ksf.meibo888.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cvv.nanxuanxn.top

C#:   int Add(int a, int b) => a + b;
来源：http://krr.aibaodan.cn

[C14] 泛型函数
来源：http://fub.shangyingyoupin.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ndj.jiagoushi.top

PHP:  // 无泛型
来源：http://hxa.chenlongwang.top

JS:   // 无泛型
来源：http://sou.guannengcc.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vgf.hesvh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://oet.hongshengwenyu.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mmw.andypj.xyz

Ruby: # 无泛型
来源：http://eql.havefunace.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jdr.shanyushiyangtech.top

[C15] 解构 / 展开参数
来源：http://yna.zhoulong.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hms.iojbl.cn

PHP:  [$a, $b] = $pair;
来源：http://bno.iojbl.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tdb.guowangkeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zit.yj20258888.top

Java: // 无解构
来源：http://sbo.daxiang520.top

Go:   // 无解构
来源：http://fns.pengpengdd.cyou

Ruby: a, b = pair
来源：http://kac.yangfankeji.com

C#:   var (a, b) = pair;
来源：http://peq.hesvh.cn

[C16] 函数 / 方法重载
来源：http://llj.yfazqb.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bvd.ydjk.org.cn

PHP:  // 无重载
来源：http://pwx.hfpthk.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ogb.yj20258888.top

TS:   // 用联合类型或重载签名声明
来源：http://ple.c1oappe.top

Java: void f(int a) {}  void f(String a) {}
来源：http://xrj.yuxming.cn

Go:   // 无重载：用不同函数名
来源：http://tvc.hfpthk.cn

Ruby: # 无重载：靠动态参数
来源：http://zns.fehbvm.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://iok.52xcode.cn

================================================================================
来源：http://jtj.hongshengwenyu.top

D. 数组 / 列表 / 集合
来源：http://xce.tianlin.xyz

================================================================================
来源：http://hgv.hfpthk.cn

[D01] 创建数组 / 列表
来源：http://dxp.cucudq.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://nor.nanxuanxn.top


<!-- 参考信息 -->