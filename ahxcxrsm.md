代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://hso.yvedp.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pqh.zdqjudy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nue.tianlin.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://chc.quarkkingdee.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ync.hammf.cn

================================================================================
来源：http://hit.zycfv.cn

B. 流程控制
来源：http://ltw.zhengqikj.top

================================================================================
来源：http://bdq.xinyue.icu

[B01] 条件判断 if / else
来源：http://ejg.shanyushiyangkeji.top

Py:   result = "正" if x > 0 else "非正"
来源：http://utd.vehdjk.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rry.sxryk.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qwo.xingfuxueyuan.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fvh.jqgufenzy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://zxe.cheryme.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dbf.jyoumei.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://paa.c1oappe.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ecz.epnwcf.com

[B02] 多分支 else if / elif
来源：http://qwm.0kj1m.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gqq.smart0.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://css.cashguo.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dim.pengpengdd.cyou

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yuj.xziqi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mlr.guannengcc.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wzn.ydzc1.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fcs.redwolf501.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://krg.yj20258.top

[B03] switch / match / case
来源：http://wva.iojbl.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qse.chenjidiqi.icu

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lxz.kuanghao11.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uhl.cdnleiting.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gyc.guannengcc.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://srh.aizwys.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kby.ybcxt.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yuo.chenzaomai.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uzm.gotoacloud.top

[B04] for 计数循环
来源：http://jan.xziqi.cn

Py:   for i in range(10): print(i)
来源：http://ncv.yj202588.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ukt.zhengqikj.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nuz.jyoumei.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nuu.zhoulong.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wsk.uphjek.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://oia.yonumen.top

Ruby: 10.times { |i| puts i }
来源：http://lxu.andypj.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://swy.birdmap.top

[B05] 遍历数组 / 列表
来源：http://hjc.zhoulong.xyz

Py:   for item in arr: print(item)
来源：http://wut.nanxinkj.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zvg.snrcjt.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://lod.wangdashe.top

TS:   for (const item of arr) { console.log(item); }
来源：http://iht.yanxiufei.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://egx.andypj.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mln.chenlongwang.top

Ruby: arr.each { |item| puts item }
来源：http://lmp.yueranfly.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://otc.xylfe.cn

[B06] 遍历字典 / 对象
来源：http://tmv.kuanghao11.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://klx.svipenyu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yam.shanyushiyangtech.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://now.vqdsnc.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://arb.yj20258888.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hwc.xuanzx.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kuj.gotoacloud.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://css.cdnleiting.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tak.sweek.top

[B07] while 循环
来源：http://ikl.zhengqikj.top

Py:   while i < 10: i += 1
来源：http://kcc.cdnleiting.top

PHP:  while ($i < 10) { $i++; }
来源：http://tju.haohaochexian.top

JS:   while (i < 10) { i++; }
来源：http://tvr.yj202588.top

TS:   while (i < 10) { i++; }
来源：http://pcx.zdqjudy.top

Java: while (i < 10) { i++; }
来源：http://auc.chenlongwang.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ywy.hnqzz.top

Ruby: while i < 10; i += 1; end
来源：http://ceq.hywenlv.cn

C#:   while (i < 10) { i++; }
来源：http://eex.andypj.xyz

[B08] do-while（至少执行一次）
来源：http://fuw.jinqigfzy.top

Py:   # 无 do-while：用 while True + break
来源：http://yzb.zhiwuduotai.top

PHP:  do { $i++; } while ($i < 10);
来源：http://exm.sysykeji.top

JS:   do { i++; } while (i < 10);
来源：http://xsa.zhongyouzk.top

TS:   do { i++; } while (i < 10);
来源：http://wib.dianchejie.cn

Java: do { i++; } while (i < 10);
来源：http://pac.yvedp.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xnt.yfazqb.com

Ruby: begin; i += 1; end while i < 10
来源：http://xkw.ydzc1.top

C#:   do { i++; } while (i < 10);
来源：http://hie.iojbl.cn

[B09] break 与 continue
来源：http://jpq.svipenyu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mqe.smart0.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rnd.birdmap.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ybz.0kj1m.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yaj.ivvv.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sie.ywan-chungtsiang.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pnm.quarkkingdee.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://edw.hongshengwenyu.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ivj.jinqigufen.top

[B10] 遍历同时拿索引
来源：http://qjf.zhoulong.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rsp.tarul.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://byq.kuanghao11.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://aza.zhengqikj.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hbc.vqdsnc.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://syw.zhaomingkeji.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ayr.guowangkeji.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bbe.yj20258.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dua.shanyushiyangkeji.top

[B11] 生成数字序列 / 区间
来源：http://kdn.yj20258.top

Py:   list(range(0, 10, 2))
来源：http://wum.ydjk.org.cn

PHP:  range(0, 10, 2);
来源：http://uau.cheryme.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cno.aizwys.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zqq.c1oappe.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://brc.zhoulong.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wui.zycfv.cn

Ruby: (0...10).step(2).to_a
来源：http://tgm.cdnleiting.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gbk.yuxming.cn

[B12] 跳出多层循环
来源：http://jus.pengpengdd.cyou

Py:   # 无标签跳转：抽成函数用 return
来源：http://oyq.shanyushiyangkeji.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://wrm.ybcxt.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vmp.andypj.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://imc.zhengqikj.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rsa.tanke756.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jfe.hysaishi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ybg.cheryme.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xow.zhongyouzk.top

[B13] 判断是否为数字
来源：http://zvv.sjlbkw.cn

Py:   isinstance(x, (int, float))
来源：http://ety.jqgfzy.top

PHP:  is_numeric($x)
来源：http://pgk.cdnleiting.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tnw.wangdashe.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hwu.ydjk.org.cn

Java: x instanceof Number
来源：http://bbx.0kj1m.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qxf.yj202588.top

Ruby: x.is_a?(Numeric)
来源：http://bsa.zhijiandao.cn

C#:   x is int or double or decimal
来源：http://dwz.gaohongyu789.top

[B14] 判断值是否在集合内
来源：http://sht.gogol.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://soj.sxryk.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ait.nwbrower.top

JS:   [1, 2, 3].includes(x)
来源：http://xvf.hnqzz.top

TS:   [1, 2, 3].includes(x)
来源：http://njn.pycfn.com

Java: List.of(1, 2, 3).contains(x)
来源：http://vrk.havefunace.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tne.hesvh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://svc.svipenyu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://azc.gogol.net.cn

[B15] 布尔运算与取反
来源：http://nfh.guowangkeji.top

Py:   a and b or not c
来源：http://yps.iojbl.cn

PHP:  $a && $b || !$c
来源：http://scq.pengpengdd.cyou

JS:   a && b || !c
来源：http://mmr.zhiwuduotai.top

TS:   a && b || !c
来源：http://xwd.sufxvd.cn

Java: a && b || !c
来源：http://qfr.yvedp.cn

Go:   a && b || !c
来源：http://rgi.yanxiufei.cn

Ruby: a && b || !c
来源：http://qqy.zhixingplan.top

C#:   a && b || !c
来源：http://xqo.jqgfzy.top

[B16] 卫语句：不满足条件提前返回
来源：http://xpv.zycfv.cn

Py:   if not data: return
来源：http://qqf.shangyingyoupin.top

PHP:  if (!$data) { return; }
来源：http://huk.316326.xyz

JS:   if (!data) return;
来源：http://xnw.jinqigufen.top

TS:   if (!data) return;
来源：http://nhf.vehdjk.com

Java: if (data == null) return;
来源：http://upp.jinghuilouyu.cn

Go:   if data == nil { return }
来源：http://owo.zdqjudy.top

Ruby: return if data.nil?
来源：http://qbv.pycfn.com

C#:   if (data == null) return;
来源：http://ojp.hnqzz.top

================================================================================
来源：http://wnm.bjfxy.top

C. 函数与作用域
来源：http://ocr.jinyuanbaomall.cn

================================================================================
来源：http://bzz.feifeiyinyue.top

[C01] 定义函数
来源：http://vqy.zhijiandao.cn

Py:   def add(a, b): return a + b
来源：http://uac.ywan-chungtsiang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ost.zhoulong.xyz

JS:   function add(a, b) { return a + b; }
来源：http://txv.yonumen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://inu.yvedp.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qiu.aibaodan.cn

Go:   func add(a, b int) int { return a + b }
来源：http://tjm.wangdashe.top

Ruby: def add(a, b); a + b; end
来源：http://mhv.nanxuanxn.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://opr.ydzc1.top

[C02] 默认参数
来源：http://rpm.aibaodan.cn

Py:   def greet(name="World"): return name
来源：http://xcp.andypj.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://sgc.ybcxt.top

JS:   function greet(name = "World") { return name; }
来源：http://eux.xuanzx.com

TS:   function greet(name: string = "World") { return name; }
来源：http://fag.zdbjq.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://lih.chenlongwang.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ath.zhixingplan.top

Ruby: def greet(name = "World") = name
来源：http://bcn.mhx1999.top

C#:   string Greet(string name = "World") => name;
来源：http://pdd.chenjidiqi.icu

[C03] 可变参数
来源：http://zwi.tarul.cn

Py:   def total(*args): return sum(args)
来源：http://nyg.sufxvd.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jne.sysykeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gfx.hfpthk.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vdv.cheryme.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cuu.hesvh.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mxj.daxiang520.top

Ruby: def total(*nums); nums.sum; end
来源：http://wzs.xuanzx.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://llr.fehbvm.com

[C04] 命名参数 / 关键字参数
来源：http://lsr.fktsv.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://flb.hfpthk.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zib.ydjk.org.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mcq.smart0.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lqp.tianlin.xyz

Java: // 无：用 Builder 模式或 record
来源：http://bxt.jqgfzy.top

Go:   // 无：用配置结构体参数
来源：http://zgv.yfazqb.com

Ruby: f(a: 1, b: 2)
来源：http://yrn.52xcode.cn

C#:   f(a: 1, b: 2)
来源：http://trr.bbcook.cn

[C05] 返回多个值
来源：http://sck.fengsongda.top

Py:   return a, b
来源：http://ago.fzhhl.top

PHP:  return [$a, $b];
来源：http://mpq.zhongyouzk.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://yuc.cqqwz.cn

TS:   return { a, b };
来源：http://wiv.shzxlz.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fje.hfpthk.cn

Go:   return a, b
来源：http://tjd.xuanzx.com

Ruby: return a, b
来源：http://vxt.feifeiyinyue.top

C#:   return (a, b);              // ValueTuple
来源：http://lmr.52xcode.cn

[C06] 匿名函数 / lambda
来源：http://vll.birdmap.top

Py:   square = lambda x: x * x
来源：http://nqf.ivvv.top

PHP:  $square = fn($x) => $x * $x;
来源：http://zvh.xingfuxueyuan.xyz

JS:   const square = x => x * x;
来源：http://sab.kuanghao11.cn

TS:   const square = (x: number): number => x * x;
来源：http://cky.nanxuanxn.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://eom.316326.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://khh.fzhhl.top

Ruby: square = ->(x) { x * x }
来源：http://nbs.vehdjk.com

C#:   Func<int, int> square = x => x * x;
来源：http://rcc.nanxinkj.top

[C07] 把函数作为参数传入
来源：http://ntf.hywenlv.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://uyw.gaohongyu789.top

PHP:  array_map("strtoupper", $arr);
来源：http://dwe.fzhhl.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://den.vehdjk.com

TS:   arr.map(String)
来源：http://lwd.hywenlv.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://upb.fengsongda.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hxo.9152youxi.cn

Ruby: arr.map(&:upcase)
来源：http://hfm.gotoacloud.top

C#:   arr.Select(s => s.ToUpper())
来源：http://mik.hcnkem.com

[C08] 闭包
来源：http://lol.xinyue.icu

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://buh.gotoacloud.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uqw.cheryme.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yfq.chenzaomai.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qdj.jqgfzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tya.andypj.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jgg.haohaochexian.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nlh.hongshengwenyu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lrk.hammf.cn

[C09] 递归
来源：http://gnr.tianlin.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wnd.yangfankeji.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tkj.sweek.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xun.gogol.net.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://het.yj20258888.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://alq.gotoacloud.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://udp.xuanzx.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ngk.yanxiufei.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mml.tarul.cn

[C10] 变量作用域
来源：http://oga.yonumen.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://por.zhengqikj.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yqj.uphjek.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pfl.ivvv.top

TS:   同 JS
来源：http://vot.kuanghao11.cn

Java: 方法内为块级作用域
来源：http://rvs.cashguo.top

Go:   花括号块级作用域
来源：http://cfk.redwolf501.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wgt.haohaochexian.top

C#:   块级作用域
来源：http://ddz.daxiang520.top

[C11] 模块导入与导出
来源：http://vac.gogol.net.cn

Py:   from module import func
来源：http://tjj.zdqjudy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://kqa.yueranfly.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://pmy.zhijiandao.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fah.mhx1999.top

Java: import java.util.List;
来源：http://poq.jinqigfzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zfn.tanke756.top

Ruby: require "json"; require_relative "./util"
来源：http://tze.9152youxi.cn

C#:   using System.Text;
来源：http://viq.hcnkem.com

[C12] 立即执行函数 IIFE
来源：http://qut.zhongyouzk.top

Py:   (lambda: print("run"))()
来源：http://iaj.chenlongwang.top

PHP:  (function () { echo "run"; })();
来源：http://thv.feifeiyinyue.top

JS:   (() => { console.log("run"); })();
来源：http://vbz.daxiang520.top

TS:   (() => { console.log("run"); })();
来源：http://xnx.guannengcc.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ext.zdbjq.cn

Go:   func() { fmt.Println("run") }()
来源：http://ead.hysaishi.cn

Ruby: -> { puts "run" }.call
来源：http://eln.hnxiangtu.top

C#:   // 无 IIFE：用静态构造函数
来源：http://obj.andypj.xyz

[C13] 类型声明 / 类型注解
来源：http://bfi.cdnleiting.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gjy.hammf.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dxw.meibo888.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nhg.nwbrower.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bym.shuidangran.top

Java: int add(int a, int b) { return a + b; }
来源：http://rcz.shangyingyoupin.top

Go:   func add(a, b int) int
来源：http://uqn.feifeiyinyue.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xup.gogol.net.cn

C#:   int Add(int a, int b) => a + b;
来源：http://pao.yj20258888.top

[C14] 泛型函数
来源：http://rhz.tian-w.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fvc.ivvv.top

PHP:  // 无泛型
来源：http://htu.kuanghao11.cn

JS:   // 无泛型
来源：http://vxu.meibo888.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://spn.cashguo.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ukn.xziqi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://niu.zycfv.cn

Ruby: # 无泛型
来源：http://rvr.vehdjk.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rfk.chenjidiqi.icu

[C15] 解构 / 展开参数
来源：http://eln.shangyingyoupin.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://uct.sweek.top

PHP:  [$a, $b] = $pair;
来源：http://kzq.wangdashe.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://iol.jlsjyb.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yfx.aizwys.cn

Java: // 无解构
来源：http://fks.wangshuangyany.cn

Go:   // 无解构
来源：http://ktt.yj202588.top

Ruby: a, b = pair
来源：http://hro.xuanzx.com

C#:   var (a, b) = pair;
来源：http://mbb.0kj1m.cn

[C16] 函数 / 方法重载
来源：http://fdv.xylfe.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://njj.xinyue.icu

PHP:  // 无重载
来源：http://qfi.yj20258888.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://xjm.svipenyu.cn

TS:   // 用联合类型或重载签名声明
来源：http://zzl.jinqigfzy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://tae.yongpay.top

Go:   // 无重载：用不同函数名
来源：http://dzl.zhixingplan.top

Ruby: # 无重载：靠动态参数
来源：http://haw.smart0.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://lbc.daria6918.cn

================================================================================
来源：http://oqr.zdqjudy.top


<!-- 参考信息 -->