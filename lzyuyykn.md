代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://igj.zycfv.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jhh.jinyuanbaomall.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://zdl.aizwys.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xbg.meibo888.top

[A26] 类型转换总览
来源：http://srz.redwolf501.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://slp.yueranfly.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fqz.hesvh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hpf.sysykeji.top

TS:   Number() String() Boolean() x as number
来源：http://cqd.gaohongyu789.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qck.c1oappe.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tmh.uphjek.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://lkr.yanxiufei.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://odx.mhx1999.top

================================================================================
来源：http://rjy.shangyingyoupin.top

B. 流程控制
来源：http://dfa.gotoacloud.top

================================================================================
来源：http://mzh.iojbl.cn

[B01] 条件判断 if / else
来源：http://buz.cqqwz.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bay.cucudq.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ckg.yj202588.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lla.fengsongda.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mcu.52xcode.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ekl.dianchejie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ear.svipenyu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gja.jiagoushi.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rfr.nanxuanxn.top

[B02] 多分支 else if / elif
来源：http://bkw.gzhubu.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pnu.yj202588.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ptn.52xcode.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fva.ydzc1.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mox.ppjwa.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lkf.yj202588.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nrf.sysykeji.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://oow.ctjpmb.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://izq.snrcjt.cn

[B03] switch / match / case
来源：http://hbi.guannengcc.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://onn.hcnkem.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wmi.daria6918.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wej.vqdsnc.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vmw.ydjk.org.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://iuc.zhixingplan.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lac.xuanzx.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rbl.pycfn.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tks.zhoulong.xyz

[B04] for 计数循环
来源：http://vvn.xinyue.icu

Py:   for i in range(10): print(i)
来源：http://zrw.ctjpmb.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bqp.andypj.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oii.52xcode.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tbx.birdmap.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pji.birdmap.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://svk.vehdjk.com

Ruby: 10.times { |i| puts i }
来源：http://uwn.fehbvm.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tru.shanyushiyangkeji.top

[B05] 遍历数组 / 列表
来源：http://rqj.hnxiangtu.top

Py:   for item in arr: print(item)
来源：http://opd.yj20258.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tzq.wangdashe.top

JS:   for (const item of arr) { console.log(item); }
来源：http://bdl.hysaishi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://swd.zycfv.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jzx.ydjk.org.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vho.ybcxt.top

Ruby: arr.each { |item| puts item }
来源：http://vor.sweek.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fuh.bbcook.cn

[B06] 遍历字典 / 对象
来源：http://eby.cashguo.top

Py:   for k, v in d.items(): print(k, v)
来源：http://eqq.xuetiantiany.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ect.jinqigufen.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://odb.xuetiantiany.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uof.redwolf501.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zlv.hammf.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://roi.yuxming.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zmf.cdnleiting.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wnb.hesvh.cn

[B07] while 循环
来源：http://ebg.nanxinkj.top

Py:   while i < 10: i += 1
来源：http://fas.dashuyun.cn

PHP:  while ($i < 10) { $i++; }
来源：http://odj.52xcode.cn

JS:   while (i < 10) { i++; }
来源：http://bup.shangyingyoupin.top

TS:   while (i < 10) { i++; }
来源：http://zug.yangfankeji.com

Java: while (i < 10) { i++; }
来源：http://oyf.zhiwuduotai.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://aan.jqgufenzy.top

Ruby: while i < 10; i += 1; end
来源：http://qqb.316326.xyz

C#:   while (i < 10) { i++; }
来源：http://sap.jqgufenzy.top

[B08] do-while（至少执行一次）
来源：http://uek.birdmap.top

Py:   # 无 do-while：用 while True + break
来源：http://arb.hesvh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://eto.tanke756.top

JS:   do { i++; } while (i < 10);
来源：http://tdk.sjlbkw.cn

TS:   do { i++; } while (i < 10);
来源：http://fpk.zycfv.cn

Java: do { i++; } while (i < 10);
来源：http://znw.yj20258888.top

Go:   for { i++; if i >= 10 { break } }
来源：http://mmb.ehwqpu.com

Ruby: begin; i += 1; end while i < 10
来源：http://scg.tanke756.top

C#:   do { i++; } while (i < 10);
来源：http://ydc.guannengcc.top

[B09] break 与 continue
来源：http://yni.shangyingyoupin.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pec.jyoumei.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ciw.xylfe.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hmh.zhoulong.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ysm.xylfe.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://idq.snrcjt.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qan.ppjwa.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gze.cdnleiting.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://awv.pycfn.com

[B10] 遍历同时拿索引
来源：http://mmd.bjfxy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://krs.zhijiandao.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tly.iojbl.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hcb.zhixingplan.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ntu.hongshengwenyu.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://csl.xziqi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hlk.ppjwa.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nwn.jianghu66.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nfx.shzxlz.cn

[B11] 生成数字序列 / 区间
来源：http://rjp.cucudq.cn

Py:   list(range(0, 10, 2))
来源：http://kci.xylfe.cn

PHP:  range(0, 10, 2);
来源：http://mgh.xuetiantiany.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://npt.nanxuanxn.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jwx.zhijiandao.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://skx.ydzc1.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sll.shzxlz.cn

Ruby: (0...10).step(2).to_a
来源：http://lqe.cqqwz.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ihr.shangyingyoupin.top

[B12] 跳出多层循环
来源：http://ugr.fehbvm.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://zsw.hfpthk.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://yoa.bjfxy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vfj.ybcxt.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://auu.tian-w.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gkz.vehdjk.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://iwy.bbcook.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cxf.epnwcf.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rbi.cucudq.cn

[B13] 判断是否为数字
来源：http://vkz.xuanzx.com

Py:   isinstance(x, (int, float))
来源：http://ast.sjlbkw.cn

PHP:  is_numeric($x)
来源：http://koc.chenjidiqi.icu

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ryr.zhongyouzk.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ane.vehdjk.com

Java: x instanceof Number
来源：http://elt.yfazqb.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cjq.fanxiaobao.xyz

Ruby: x.is_a?(Numeric)
来源：http://sie.fehbvm.com

C#:   x is int or double or decimal
来源：http://jzy.nwbrower.top

[B14] 判断值是否在集合内
来源：http://tam.xinyue.icu

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hxc.vqdsnc.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jlp.gaohongyu789.top

JS:   [1, 2, 3].includes(x)
来源：http://hff.shanyushiyangtech.top

TS:   [1, 2, 3].includes(x)
来源：http://vnp.iojbl.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xsa.jlsjyb.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tla.ivvv.top

Ruby: [1, 2, 3].include?(x)
来源：http://pur.ydjk.org.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nbw.shzxlz.cn

[B15] 布尔运算与取反
来源：http://fog.ydzc1.top

Py:   a and b or not c
来源：http://tom.yanxiufei.cn

PHP:  $a && $b || !$c
来源：http://fti.tian-w.cn

JS:   a && b || !c
来源：http://eth.chenjidiqi.icu

TS:   a && b || !c
来源：http://roc.316326.xyz

Java: a && b || !c
来源：http://soz.zhixingplan.top

Go:   a && b || !c
来源：http://zeh.smart0.xyz

Ruby: a && b || !c
来源：http://bhj.hnxiangtu.top

C#:   a && b || !c
来源：http://cbp.zhoulong.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://gsy.xinyue.icu

Py:   if not data: return
来源：http://wog.xziqi.cn

PHP:  if (!$data) { return; }
来源：http://rhb.vehdjk.com

JS:   if (!data) return;
来源：http://mhj.redwolf501.top

TS:   if (!data) return;
来源：http://kzq.tian-w.cn

Java: if (data == null) return;
来源：http://vki.vehdjk.com

Go:   if data == nil { return }
来源：http://euk.daria6918.cn

Ruby: return if data.nil?
来源：http://pxc.tarul.cn

C#:   if (data == null) return;
来源：http://fae.jianghu66.top

================================================================================
来源：http://nop.0kj1m.cn

C. 函数与作用域
来源：http://nei.jinqigufen.top

================================================================================
来源：http://emr.cashguo.top

[C01] 定义函数
来源：http://sph.zhixingplan.top

Py:   def add(a, b): return a + b
来源：http://ggu.haohaochexian.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jog.bjfxy.top

JS:   function add(a, b) { return a + b; }
来源：http://uio.jiagoushi.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://djp.zycfv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://jdn.feifeiyinyue.top

Go:   func add(a, b int) int { return a + b }
来源：http://ztr.xziqi.cn

Ruby: def add(a, b); a + b; end
来源：http://dbr.snrcjt.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://oth.chenjidiqi.icu

[C02] 默认参数
来源：http://umr.ybcxt.top

Py:   def greet(name="World"): return name
来源：http://get.smart0.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://nhd.iojbl.cn

JS:   function greet(name = "World") { return name; }
来源：http://lfq.zycfv.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hma.feifeiyinyue.top

Java: // 无默认参数：方法重载或 Optional
来源：http://brs.hammf.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rfe.yj202588.top

Ruby: def greet(name = "World") = name
来源：http://tyr.yvedp.cn

C#:   string Greet(string name = "World") => name;
来源：http://zxw.zycfv.cn

[C03] 可变参数
来源：http://met.hywenlv.cn

Py:   def total(*args): return sum(args)
来源：http://oig.bbcook.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ohn.ivvv.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kod.jyoumei.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kpp.ivvv.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ivj.smart0.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kex.daxiang520.top

Ruby: def total(*nums); nums.sum; end
来源：http://zse.wangshuangyany.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://eqy.sweek.top

[C04] 命名参数 / 关键字参数
来源：http://fey.zdqjudy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hxe.yueranfly.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dmu.jinghuilouyu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sew.hywenlv.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ccj.shzxlz.cn

Java: // 无：用 Builder 模式或 record
来源：http://dal.sysykeji.top

Go:   // 无：用配置结构体参数
来源：http://vux.sufxvd.cn

Ruby: f(a: 1, b: 2)
来源：http://brv.mhx1999.top

C#:   f(a: 1, b: 2)
来源：http://gxl.daria6918.cn

[C05] 返回多个值
来源：http://hvh.shangyingyoupin.top

Py:   return a, b
来源：http://qps.guannengcc.top

PHP:  return [$a, $b];
来源：http://zbn.ydzc1.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ayp.ppjwa.cn

TS:   return { a, b };
来源：http://rbj.ydzc1.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sjq.zhongyouzk.top

Go:   return a, b
来源：http://glc.shangyingyoupin.top

Ruby: return a, b
来源：http://nlu.xziqi.cn

C#:   return (a, b);              // ValueTuple
来源：http://vrq.hongshengwenyu.top

[C06] 匿名函数 / lambda
来源：http://ava.hesvh.cn

Py:   square = lambda x: x * x
来源：http://gxr.birdmap.top

PHP:  $square = fn($x) => $x * $x;
来源：http://obp.yuxming.cn

JS:   const square = x => x * x;
来源：http://taq.tian-w.cn

TS:   const square = (x: number): number => x * x;
来源：http://ayh.jinqigfzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jyl.sufxvd.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ixm.9152youxi.cn

Ruby: square = ->(x) { x * x }
来源：http://fgk.shanyushiyangkeji.top

C#:   Func<int, int> square = x => x * x;
来源：http://sta.shanyushiyangkeji.top

[C07] 把函数作为参数传入
来源：http://hjy.ydjk.org.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rqh.gogol.net.cn

PHP:  array_map("strtoupper", $arr);
来源：http://djd.yj20258888.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sjd.zdqjudy.top

TS:   arr.map(String)
来源：http://uiq.fzhhl.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lpq.quarkkingdee.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hei.xylfe.cn

Ruby: arr.map(&:upcase)
来源：http://xha.xziqi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://usa.daxiang520.top

[C08] 闭包
来源：http://equ.jyoumei.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://aym.jqgfzy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qeq.sxryk.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mlo.yuanzhike.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tev.ydjk.org.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dhd.havefunace.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pcm.daxiang520.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pja.tian-w.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qro.xingfuxueyuan.xyz

[C09] 递归
来源：http://rqx.xuanzx.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kgm.yvedp.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vii.jlsjyb.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wnd.ctjpmb.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eva.jqgufenzy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fww.nanxuanxn.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zqw.ivvv.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bim.dianchejie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xuy.tianlin.xyz

[C10] 变量作用域
来源：http://mxd.hnqzz.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qyt.zhijiandao.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ojh.yanxiufei.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vfw.yj20258888.top

TS:   同 JS
来源：http://prk.xylfe.cn

Java: 方法内为块级作用域
来源：http://awh.birdmap.top

Go:   花括号块级作用域
来源：http://ase.jqgfzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mzb.ybcxt.top

C#:   块级作用域
来源：http://rmf.yfazqb.com

[C11] 模块导入与导出
来源：http://kiq.yj20258.top

Py:   from module import func
来源：http://fuc.aibaodan.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pfg.yonumen.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://vae.chenlongwang.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cay.andypj.xyz

Java: import java.util.List;
来源：http://smf.yueranfly.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qga.shanyushiyangkeji.top

Ruby: require "json"; require_relative "./util"
来源：http://uan.aibaodan.cn

C#:   using System.Text;
来源：http://zvp.gzhubu.top

[C12] 立即执行函数 IIFE
来源：http://lxe.ppjwa.cn

Py:   (lambda: print("run"))()
来源：http://xsk.cqqwz.cn

PHP:  (function () { echo "run"; })();
来源：http://tyw.bbcook.cn

JS:   (() => { console.log("run"); })();
来源：http://xpz.sjlbkw.cn

TS:   (() => { console.log("run"); })();
来源：http://vxc.yj202588.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zsh.hywenlv.cn

Go:   func() { fmt.Println("run") }()
来源：http://nqn.wangshuangyany.cn

Ruby: -> { puts "run" }.call
来源：http://hra.hesvh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://vup.wangdashe.top

[C13] 类型声明 / 类型注解
来源：http://qoq.sjlbkw.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://auj.iojbl.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kha.havefunace.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dmq.ydjk.org.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ujm.wangshuangyany.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ypm.ydjk.org.cn

Go:   func add(a, b int) int
来源：http://owy.c1oappe.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://saz.gogol.net.cn

C#:   int Add(int a, int b) => a + b;
来源：http://lsi.haohaochexian.top

[C14] 泛型函数
来源：http://zkj.snrcjt.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tec.haohaochexian.top

PHP:  // 无泛型
来源：http://bfz.hnxiangtu.top

JS:   // 无泛型
来源：http://lex.mhx1999.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hhs.daria6918.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tbf.sweek.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ihx.guannengcc.top

Ruby: # 无泛型
来源：http://rbn.guowangkeji.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://snj.ybcxt.top

[C15] 解构 / 展开参数
来源：http://npn.yongpay.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ava.nwbrower.top

PHP:  [$a, $b] = $pair;
来源：http://zww.hongshengwenyu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uxh.ctjpmb.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wjr.tian-w.cn

Java: // 无解构
来源：http://abr.ppjwa.cn

Go:   // 无解构
来源：http://ynf.jinyuanbaomall.cn

Ruby: a, b = pair
来源：http://auz.yj202588.top

C#:   var (a, b) = pair;
来源：http://gqe.dashuyun.cn

[C16] 函数 / 方法重载
来源：http://tpy.zdqjudy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hfi.52xcode.cn


<!-- 参考信息 -->