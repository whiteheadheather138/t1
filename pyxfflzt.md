代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kkd.nanxuanxn.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gyj.tanke756.top

Ruby: s1 == s2; s1 <=> s2
来源：http://awn.cdnleiting.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zfo.yvedp.cn

[A26] 类型转换总览
来源：http://ntc.chenlongwang.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jsq.xuetiantiany.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://urk.yj20258888.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://oqf.cucudq.cn

TS:   Number() String() Boolean() x as number
来源：http://mka.smart0.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://knm.fanxiaobao.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gyg.zycfv.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://cmd.shanyushiyangkeji.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bhp.guowangkeji.top

================================================================================
来源：http://gvz.aibaodan.cn

B. 流程控制
来源：http://ocr.sufxvd.cn

================================================================================
来源：http://lwf.xziqi.cn

[B01] 条件判断 if / else
来源：http://gmb.nwbrower.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ogk.ctjpmb.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://eho.jqgfzy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://avn.shanyushiyangkeji.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uow.yuanzhike.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://rcf.wangshuangyany.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ymr.havefunace.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tmx.sysykeji.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://iap.jyoumei.cn

[B02] 多分支 else if / elif
来源：http://maf.aibaodan.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kie.aibaodan.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qrd.cqqwz.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xbq.yuxming.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xge.zdbjq.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sip.hywenlv.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wnn.nanxuanxn.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ryl.ivvv.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nwh.redwolf501.top

[B03] switch / match / case
来源：http://ysu.hammf.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mpj.ppjwa.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uwu.c1oappe.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jel.vehdjk.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iql.jyoumei.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nrw.jlsjyb.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dzk.shanyushiyangkeji.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qtn.fanxiaobao.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qlx.chenlongwang.top

[B04] for 计数循环
来源：http://jbs.ydjk.org.cn

Py:   for i in range(10): print(i)
来源：http://kkw.haohaochexian.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cbo.dashuyun.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bfk.snrcjt.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nok.cqqwz.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pul.redwolf501.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hwj.zdqjudy.top

Ruby: 10.times { |i| puts i }
来源：http://imi.ivvv.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yvw.tian-w.cn

[B05] 遍历数组 / 列表
来源：http://swk.ydzc1.top

Py:   for item in arr: print(item)
来源：http://ucq.cqqwz.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://enz.aibaodan.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ash.hcnkem.com

TS:   for (const item of arr) { console.log(item); }
来源：http://gud.nanxuanxn.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://jyc.yj20258.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jgo.sweek.top

Ruby: arr.each { |item| puts item }
来源：http://idj.yvedp.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nbz.snrcjt.cn

[B06] 遍历字典 / 对象
来源：http://lzv.vqdsnc.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xng.ybcxt.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vis.dashuyun.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lcc.shanyushiyangkeji.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mnp.jlsjyb.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dkd.meibo888.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ffz.yangfankeji.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://phv.ctjpmb.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nij.shuidangran.top

[B07] while 循环
来源：http://mmj.mhx1999.top

Py:   while i < 10: i += 1
来源：http://wkl.shangyingyoupin.top

PHP:  while ($i < 10) { $i++; }
来源：http://eay.hammf.cn

JS:   while (i < 10) { i++; }
来源：http://ivc.nwbrower.top

TS:   while (i < 10) { i++; }
来源：http://khb.yanxiufei.cn

Java: while (i < 10) { i++; }
来源：http://bze.daxiang520.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://deq.shanyushiyangtech.top

Ruby: while i < 10; i += 1; end
来源：http://qtw.aizwys.cn

C#:   while (i < 10) { i++; }
来源：http://szz.zhiwuduotai.top

[B08] do-while（至少执行一次）
来源：http://rqx.wangshuangyany.cn

Py:   # 无 do-while：用 while True + break
来源：http://kcz.yanxiufei.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://faf.gotoacloud.top

JS:   do { i++; } while (i < 10);
来源：http://ljb.redwolf501.top

TS:   do { i++; } while (i < 10);
来源：http://vfa.nanxinkj.top

Java: do { i++; } while (i < 10);
来源：http://mti.aibaodan.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vyd.fengsongda.top

Ruby: begin; i += 1; end while i < 10
来源：http://bkd.ywan-chungtsiang.top

C#:   do { i++; } while (i < 10);
来源：http://xsc.jianghu66.top

[B09] break 与 continue
来源：http://inj.hesvh.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lnl.hesvh.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wwb.xingfuxueyuan.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uvm.52xcode.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gnh.iojbl.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zjn.xingfuxueyuan.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ibn.mhx1999.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yaq.fehbvm.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xza.ehwqpu.com

[B10] 遍历同时拿索引
来源：http://vfc.cheryme.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://olq.vehdjk.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://swe.hesvh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cmo.chenlongwang.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ykc.shuidangran.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nfk.jqgufenzy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vnv.9152youxi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://anh.yvedp.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ons.aizwys.cn

[B11] 生成数字序列 / 区间
来源：http://ryo.yongpay.top

Py:   list(range(0, 10, 2))
来源：http://mya.xziqi.cn

PHP:  range(0, 10, 2);
来源：http://mvq.shuidangran.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vus.tian-w.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yya.birdmap.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vlb.yfazqb.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lrl.fehbvm.com

Ruby: (0...10).step(2).to_a
来源：http://ido.daria6918.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://oes.shuidangran.top

[B12] 跳出多层循环
来源：http://xoz.yuxming.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hnh.yuanzhike.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://niv.yuanzhike.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pqu.yj20258.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ehj.ydjk.org.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ibp.ybcxt.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qgr.cheryme.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://esp.ydjk.org.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ski.iojbl.cn

[B13] 判断是否为数字
来源：http://nly.nwbrower.top

Py:   isinstance(x, (int, float))
来源：http://aqo.sysykeji.top

PHP:  is_numeric($x)
来源：http://hex.ydzc1.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dby.aizwys.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ztg.zhiwuduotai.top

Java: x instanceof Number
来源：http://vdn.dianchejie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sio.yuanzhike.top

Ruby: x.is_a?(Numeric)
来源：http://gyw.pycfn.com

C#:   x is int or double or decimal
来源：http://jgc.daxiang520.top

[B14] 判断值是否在集合内
来源：http://qyy.nanxuanxn.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lrp.hongshengwenyu.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hpt.zycfv.cn

JS:   [1, 2, 3].includes(x)
来源：http://yqr.bjfxy.top

TS:   [1, 2, 3].includes(x)
来源：http://xev.andypj.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://nws.yuxming.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wsf.feifeiyinyue.top

Ruby: [1, 2, 3].include?(x)
来源：http://gyr.redwolf501.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mwg.ydzc1.top

[B15] 布尔运算与取反
来源：http://zra.jinyuanbaomall.cn

Py:   a and b or not c
来源：http://xrz.shanyushiyangkeji.top

PHP:  $a && $b || !$c
来源：http://wyz.jinqigufen.top

JS:   a && b || !c
来源：http://iwn.jinyuanbaomall.cn

TS:   a && b || !c
来源：http://aub.fktsv.cn

Java: a && b || !c
来源：http://dae.chenlongwang.top

Go:   a && b || !c
来源：http://jvg.wangdashe.top

Ruby: a && b || !c
来源：http://mai.cashguo.top

C#:   a && b || !c
来源：http://zmv.dashuyun.cn

[B16] 卫语句：不满足条件提前返回
来源：http://eds.jyoumei.cn

Py:   if not data: return
来源：http://uoe.fanxiaobao.xyz

PHP:  if (!$data) { return; }
来源：http://tje.tanke756.top

JS:   if (!data) return;
来源：http://qxc.meibo888.top

TS:   if (!data) return;
来源：http://zum.ivvv.top

Java: if (data == null) return;
来源：http://mtc.fehbvm.com

Go:   if data == nil { return }
来源：http://qiv.shangyingyoupin.top

Ruby: return if data.nil?
来源：http://lrp.yj202588.top

C#:   if (data == null) return;
来源：http://iha.shanyushiyangtech.top

================================================================================
来源：http://qdz.zhijiandao.cn

C. 函数与作用域
来源：http://tmu.sysykeji.top

================================================================================
来源：http://vga.gogol.net.cn

[C01] 定义函数
来源：http://yhg.zycfv.cn

Py:   def add(a, b): return a + b
来源：http://mku.tanke756.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://edg.haohaochexian.top

JS:   function add(a, b) { return a + b; }
来源：http://twf.pycfn.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nqi.gogol.net.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://tkv.zhaomingkeji.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://yqz.pycfn.com

Ruby: def add(a, b); a + b; end
来源：http://bpq.yuanzhike.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://muo.birdmap.top

[C02] 默认参数
来源：http://mfj.yfazqb.com

Py:   def greet(name="World"): return name
来源：http://fwm.jiagoushi.top

PHP:  function greet($name = "World") { return $name; }
来源：http://hbs.wangshuangyany.cn

JS:   function greet(name = "World") { return name; }
来源：http://zph.yangfankeji.com

TS:   function greet(name: string = "World") { return name; }
来源：http://iay.hcnkem.com

Java: // 无默认参数：方法重载或 Optional
来源：http://cga.9152youxi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://njh.hnqzz.top

Ruby: def greet(name = "World") = name
来源：http://fww.andypj.xyz

C#:   string Greet(string name = "World") => name;
来源：http://oxk.jqgfzy.top

[C03] 可变参数
来源：http://vmz.0kj1m.cn

Py:   def total(*args): return sum(args)
来源：http://zey.fehbvm.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dei.cqqwz.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xaw.fehbvm.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pac.xziqi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xmn.xylfe.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://iht.mhx1999.top

Ruby: def total(*nums); nums.sum; end
来源：http://qft.tianlin.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baw.yueranfly.top

[C04] 命名参数 / 关键字参数
来源：http://sag.bbcook.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nsb.yvedp.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rjd.cashguo.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lud.gaohongyu789.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hkr.xinyue.icu

Java: // 无：用 Builder 模式或 record
来源：http://fvg.pycfn.com

Go:   // 无：用配置结构体参数
来源：http://rjl.xuanzx.com

Ruby: f(a: 1, b: 2)
来源：http://fiq.shuidangran.top

C#:   f(a: 1, b: 2)
来源：http://wfy.iojbl.cn

[C05] 返回多个值
来源：http://vte.hnqzz.top

Py:   return a, b
来源：http://xnz.xylfe.cn

PHP:  return [$a, $b];
来源：http://mrn.pengpengdd.cyou

JS:   return [a, b];             // 或 return { a, b };
来源：http://mry.dashuyun.cn

TS:   return { a, b };
来源：http://zdz.tarul.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://avl.yanxiufei.cn

Go:   return a, b
来源：http://aio.tianlin.xyz

Ruby: return a, b
来源：http://ztr.chenjidiqi.icu

C#:   return (a, b);              // ValueTuple
来源：http://efn.52xcode.cn

[C06] 匿名函数 / lambda
来源：http://opt.hywenlv.cn

Py:   square = lambda x: x * x
来源：http://zfk.hcnkem.com

PHP:  $square = fn($x) => $x * $x;
来源：http://gfk.jinqigufen.top

JS:   const square = x => x * x;
来源：http://bcl.nwbrower.top

TS:   const square = (x: number): number => x * x;
来源：http://djl.jyoumei.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yln.c1oappe.top

Go:   sq := func(x int) int { return x * x }
来源：http://qvk.svipenyu.cn

Ruby: square = ->(x) { x * x }
来源：http://trh.cqqwz.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bjl.xuanzx.com

[C07] 把函数作为参数传入
来源：http://usn.jianghu66.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hfa.dashuyun.cn

PHP:  array_map("strtoupper", $arr);
来源：http://oxs.vehdjk.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yne.jianghu66.top

TS:   arr.map(String)
来源：http://frf.yuanzhike.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kjz.yanxiufei.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fsb.iojbl.cn

Ruby: arr.map(&:upcase)
来源：http://thj.jyoumei.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cfi.gaohongyu789.top

[C08] 闭包
来源：http://nuw.cqqwz.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fdc.xingfuxueyuan.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://shy.epnwcf.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mkp.xylfe.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://stk.52xcode.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dsz.0kj1m.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tph.ybcxt.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nnn.yongpay.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zyh.cucudq.cn

[C09] 递归
来源：http://rzo.pycfn.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://szq.ehwqpu.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kks.ehwqpu.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://umd.ybcxt.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vjh.shangyingyoupin.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hwh.tianlin.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://itu.yfazqb.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bde.epnwcf.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cef.jianghu66.top

[C10] 变量作用域
来源：http://vpd.zycfv.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bfy.c1oappe.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://stn.hnqzz.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rsa.9152youxi.cn

TS:   同 JS
来源：http://vje.zhaomingkeji.xyz

Java: 方法内为块级作用域
来源：http://ues.316326.xyz

Go:   花括号块级作用域
来源：http://sow.yuanzhike.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sdc.ehwqpu.com

C#:   块级作用域
来源：http://ezl.jqgufenzy.top

[C11] 模块导入与导出
来源：http://gtp.fanxiaobao.xyz

Py:   from module import func
来源：http://vhv.yangfankeji.com

PHP:  require "file.php";  或 use App\Service;
来源：http://hqp.ivvv.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://aiu.fehbvm.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mwp.quarkkingdee.top

Java: import java.util.List;
来源：http://zjw.ydjk.org.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qtp.tarul.cn

Ruby: require "json"; require_relative "./util"
来源：http://ztr.c1oappe.top

C#:   using System.Text;
来源：http://hqa.daria6918.cn

[C12] 立即执行函数 IIFE
来源：http://tvx.redwolf501.top

Py:   (lambda: print("run"))()
来源：http://kek.uphjek.com

PHP:  (function () { echo "run"; })();
来源：http://cbs.shangyingyoupin.top

JS:   (() => { console.log("run"); })();
来源：http://gdx.xingfuxueyuan.xyz

TS:   (() => { console.log("run"); })();
来源：http://njj.yanxiufei.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xuy.birdmap.top

Go:   func() { fmt.Println("run") }()
来源：http://xbh.guowangkeji.top

Ruby: -> { puts "run" }.call
来源：http://saq.guannengcc.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ebt.redwolf501.top

[C13] 类型声明 / 类型注解
来源：http://dnw.xuanzx.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://egy.wangdashe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hjn.cdnleiting.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pnh.zhongyouzk.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nry.redwolf501.top

Java: int add(int a, int b) { return a + b; }
来源：http://pai.guannengcc.top

Go:   func add(a, b int) int
来源：http://djl.hnxiangtu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ely.9152youxi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://lxw.daria6918.cn

[C14] 泛型函数
来源：http://dcb.zdqjudy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://iei.epnwcf.com

PHP:  // 无泛型
来源：http://zyt.smart0.xyz

JS:   // 无泛型
来源：http://uwx.hnqzz.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mji.yvedp.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://esc.bbcook.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kev.cdnleiting.top

Ruby: # 无泛型
来源：http://izf.zhiwuduotai.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fck.fehbvm.com

[C15] 解构 / 展开参数
来源：http://trb.xinyue.icu

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fjg.hnxiangtu.top

PHP:  [$a, $b] = $pair;
来源：http://gxk.jianghu66.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tqc.pycfn.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yge.hammf.cn

Java: // 无解构
来源：http://aoe.sjlbkw.cn

Go:   // 无解构
来源：http://dzu.ctjpmb.com

Ruby: a, b = pair
来源：http://fsc.tarul.cn

C#:   var (a, b) = pair;
来源：http://lkn.zhijiandao.cn

[C16] 函数 / 方法重载
来源：http://msd.jyoumei.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vxt.hammf.cn


<!-- 参考信息 -->