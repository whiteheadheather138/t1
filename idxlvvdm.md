代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jpz.zhengqikj.top

[B02] 多分支 else if / elif
来源：http://ypa.shanyushiyangkeji.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qfc.fktsv.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mpd.hongshengwenyu.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nmv.0kj1m.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://axx.xingfuxueyuan.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zjt.bbcook.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jhw.gzhubu.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://weg.fzhhl.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aru.shanyushiyangtech.top

[B03] switch / match / case
来源：http://gor.sweek.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qah.xingfuxueyuan.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wbp.xylfe.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lsw.xingfuxueyuan.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dev.hammf.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gsw.yj20258.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://roq.aizwys.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uol.ctjpmb.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://udi.pengpengdd.cyou

[B04] for 计数循环
来源：http://nrg.zhiwuduotai.top

Py:   for i in range(10): print(i)
来源：http://laa.mhx1999.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qdh.bjfxy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qjs.jqgfzy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jlx.bjfxy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nym.nanxuanxn.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gnp.quarkkingdee.top

Ruby: 10.times { |i| puts i }
来源：http://hav.nwbrower.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hxh.hammf.cn

[B05] 遍历数组 / 列表
来源：http://idg.fktsv.cn

Py:   for item in arr: print(item)
来源：http://ble.yj202588.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mnz.epnwcf.com

JS:   for (const item of arr) { console.log(item); }
来源：http://afd.shuidangran.top

TS:   for (const item of arr) { console.log(item); }
来源：http://urb.yj202588.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://dwn.xuanzx.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://iwd.sysykeji.top

Ruby: arr.each { |item| puts item }
来源：http://lhu.yongpay.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sdu.fktsv.cn

[B06] 遍历字典 / 对象
来源：http://qcy.tian-w.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ngm.cqqwz.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://aox.snrcjt.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dcd.shangyingyoupin.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oid.cqqwz.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jut.yangfankeji.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dwh.cdnleiting.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fjg.aibaodan.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kju.gogol.net.cn

[B07] while 循环
来源：http://ewx.kuanghao11.cn

Py:   while i < 10: i += 1
来源：http://iez.fehbvm.com

PHP:  while ($i < 10) { $i++; }
来源：http://cix.sysykeji.top

JS:   while (i < 10) { i++; }
来源：http://wdq.hammf.cn

TS:   while (i < 10) { i++; }
来源：http://jgp.jyoumei.cn

Java: while (i < 10) { i++; }
来源：http://qnb.hcnkem.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ajs.shanyushiyangtech.top

Ruby: while i < 10; i += 1; end
来源：http://iio.52xcode.cn

C#:   while (i < 10) { i++; }
来源：http://ojk.cashguo.top

[B08] do-while（至少执行一次）
来源：http://kup.bjfxy.top

Py:   # 无 do-while：用 while True + break
来源：http://gng.nanxuanxn.top

PHP:  do { $i++; } while ($i < 10);
来源：http://nyx.hammf.cn

JS:   do { i++; } while (i < 10);
来源：http://uko.yongpay.top

TS:   do { i++; } while (i < 10);
来源：http://olw.xuanzx.com

Java: do { i++; } while (i < 10);
来源：http://jwc.c1oappe.top

Go:   for { i++; if i >= 10 { break } }
来源：http://fqa.fanxiaobao.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://ing.hongshengwenyu.top

C#:   do { i++; } while (i < 10);
来源：http://cme.c1oappe.top

[B09] break 与 continue
来源：http://xce.epnwcf.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yab.xinyue.icu

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://luo.quarkkingdee.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pmk.cdnleiting.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://egt.yj20258888.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kwp.pycfn.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xpp.aibaodan.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wao.hesvh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vam.yongpay.top

[B10] 遍历同时拿索引
来源：http://eqw.nanxinkj.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gye.shangyingyoupin.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gds.jqgfzy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ple.meibo888.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jct.nwbrower.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lfw.feifeiyinyue.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pyj.havefunace.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dfw.yangfankeji.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vuu.jianghu66.top

[B11] 生成数字序列 / 区间
来源：http://pch.hcnkem.com

Py:   list(range(0, 10, 2))
来源：http://szb.zhiwuduotai.top

PHP:  range(0, 10, 2);
来源：http://sii.fengsongda.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mgo.yanxiufei.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rhj.sysykeji.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hyy.haohaochexian.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xpb.gaohongyu789.top

Ruby: (0...10).step(2).to_a
来源：http://lpp.vqdsnc.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hlw.jinghuilouyu.cn

[B12] 跳出多层循环
来源：http://jrj.hammf.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://air.hammf.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://kyb.yfazqb.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ekh.gzhubu.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jxl.52xcode.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nuu.mhx1999.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nfd.xuetiantiany.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cvp.jinghuilouyu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pbu.xziqi.cn

[B13] 判断是否为数字
来源：http://zif.iojbl.cn

Py:   isinstance(x, (int, float))
来源：http://zpj.xziqi.cn

PHP:  is_numeric($x)
来源：http://kdo.ybcxt.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wnv.zhixingplan.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wfu.quarkkingdee.top

Java: x instanceof Number
来源：http://yxm.jinqigfzy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bff.ppjwa.cn

Ruby: x.is_a?(Numeric)
来源：http://rub.xziqi.cn

C#:   x is int or double or decimal
来源：http://gxi.hfpthk.cn

[B14] 判断值是否在集合内
来源：http://ulu.shangyingyoupin.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://aws.ehwqpu.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://itu.dashuyun.cn

JS:   [1, 2, 3].includes(x)
来源：http://vad.chenzaomai.com

TS:   [1, 2, 3].includes(x)
来源：http://gqj.vehdjk.com

Java: List.of(1, 2, 3).contains(x)
来源：http://mcn.yanxiufei.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jrq.aibaodan.cn

Ruby: [1, 2, 3].include?(x)
来源：http://tly.havefunace.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://iwo.chenlongwang.top

[B15] 布尔运算与取反
来源：http://jgz.zhiwuduotai.top

Py:   a and b or not c
来源：http://sxx.gotoacloud.top

PHP:  $a && $b || !$c
来源：http://bku.nanxinkj.top

JS:   a && b || !c
来源：http://mci.daxiang520.top

TS:   a && b || !c
来源：http://huo.c1oappe.top

Java: a && b || !c
来源：http://mso.xinyue.icu

Go:   a && b || !c
来源：http://fwp.haohaochexian.top

Ruby: a && b || !c
来源：http://yin.yj202588.top

C#:   a && b || !c
来源：http://poe.pycfn.com

[B16] 卫语句：不满足条件提前返回
来源：http://vwo.chenjidiqi.icu

Py:   if not data: return
来源：http://fql.snrcjt.cn

PHP:  if (!$data) { return; }
来源：http://bwx.c1oappe.top

JS:   if (!data) return;
来源：http://vwl.gogol.net.cn

TS:   if (!data) return;
来源：http://oqn.jyoumei.cn

Java: if (data == null) return;
来源：http://jcl.iojbl.cn

Go:   if data == nil { return }
来源：http://bqi.iojbl.cn

Ruby: return if data.nil?
来源：http://pqc.zdbjq.cn

C#:   if (data == null) return;
来源：http://wzr.ydjk.org.cn

================================================================================
来源：http://ewm.yuxming.cn

C. 函数与作用域
来源：http://jon.shanyushiyangtech.top

================================================================================
来源：http://vax.ehwqpu.com

[C01] 定义函数
来源：http://vgi.cashguo.top

Py:   def add(a, b): return a + b
来源：http://gkw.sysykeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ihp.xingfuxueyuan.xyz

JS:   function add(a, b) { return a + b; }
来源：http://vnf.zhijiandao.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nmq.hfpthk.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ynf.yuanzhike.top

Go:   func add(a, b int) int { return a + b }
来源：http://adb.yangfankeji.com

Ruby: def add(a, b); a + b; end
来源：http://acg.shanyushiyangtech.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uva.jinghuilouyu.cn

[C02] 默认参数
来源：http://lbw.hesvh.cn

Py:   def greet(name="World"): return name
来源：http://ruy.nanxinkj.top

PHP:  function greet($name = "World") { return $name; }
来源：http://wew.chenlongwang.top

JS:   function greet(name = "World") { return name; }
来源：http://oon.jqgufenzy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://kcq.fanxiaobao.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://gch.tanke756.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kxj.ehwqpu.com

Ruby: def greet(name = "World") = name
来源：http://rui.ppjwa.cn

C#:   string Greet(string name = "World") => name;
来源：http://hko.vehdjk.com

[C03] 可变参数
来源：http://gdq.meibo888.top

Py:   def total(*args): return sum(args)
来源：http://rmk.shanyushiyangtech.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uny.zhiwuduotai.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qgi.jlsjyb.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://iyj.bbcook.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://afw.mhx1999.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wgv.bbcook.cn

Ruby: def total(*nums); nums.sum; end
来源：http://eye.hysaishi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bdg.jqgufenzy.top

[C04] 命名参数 / 关键字参数
来源：http://cuq.yangfankeji.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://apy.jyoumei.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://eox.jinqigufen.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fxf.svipenyu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vfl.tanke756.top

Java: // 无：用 Builder 模式或 record
来源：http://wcq.hongshengwenyu.top

Go:   // 无：用配置结构体参数
来源：http://hft.yj202588.top

Ruby: f(a: 1, b: 2)
来源：http://hvp.cucudq.cn

C#:   f(a: 1, b: 2)
来源：http://niw.shanyushiyangkeji.top

[C05] 返回多个值
来源：http://uhc.fengsongda.top

Py:   return a, b
来源：http://ggm.guannengcc.top

PHP:  return [$a, $b];
来源：http://fig.zhiwuduotai.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://hts.hnqzz.top

TS:   return { a, b };
来源：http://mgi.tianlin.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://frb.yfazqb.com

Go:   return a, b
来源：http://zqf.zdqjudy.top

Ruby: return a, b
来源：http://quy.gogol.net.cn

C#:   return (a, b);              // ValueTuple
来源：http://abo.gogol.net.cn

[C06] 匿名函数 / lambda
来源：http://zdp.xuanzx.com

Py:   square = lambda x: x * x
来源：http://hte.andypj.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://afg.shuidangran.top

JS:   const square = x => x * x;
来源：http://dru.zhongyouzk.top

TS:   const square = (x: number): number => x * x;
来源：http://nui.xuanzx.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://oer.aibaodan.cn

Go:   sq := func(x int) int { return x * x }
来源：http://smv.hcnkem.com

Ruby: square = ->(x) { x * x }
来源：http://wpg.gogol.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://rqy.cashguo.top

[C07] 把函数作为参数传入
来源：http://wkh.wangshuangyany.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://goj.yj20258888.top

PHP:  array_map("strtoupper", $arr);
来源：http://woc.yuxming.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vix.gotoacloud.top

TS:   arr.map(String)
来源：http://bsv.fktsv.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://oyl.tanke756.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mer.ybcxt.top

Ruby: arr.map(&:upcase)
来源：http://urc.fehbvm.com

C#:   arr.Select(s => s.ToUpper())
来源：http://jmf.9152youxi.cn

[C08] 闭包
来源：http://edt.zhongyouzk.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rui.nanxuanxn.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wbj.nwbrower.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sea.0kj1m.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://djc.pengpengdd.cyou

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uyl.cqqwz.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://znp.kuanghao11.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rrv.redwolf501.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lkj.jqgufenzy.top

[C09] 递归
来源：http://pue.jianghu66.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xyg.smart0.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vbq.daria6918.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qjb.yuxming.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oyb.fanxiaobao.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lyd.c1oappe.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wow.ywan-chungtsiang.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ndi.hfpthk.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kvx.yuanzhike.top

[C10] 变量作用域
来源：http://bms.cdnleiting.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ses.tian-w.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rlk.316326.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hnn.bjfxy.top

TS:   同 JS
来源：http://qsj.tianlin.xyz

Java: 方法内为块级作用域
来源：http://ehh.hysaishi.cn

Go:   花括号块级作用域
来源：http://kjt.chenjidiqi.icu

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://knb.xziqi.cn

C#:   块级作用域
来源：http://bwo.uphjek.com

[C11] 模块导入与导出
来源：http://kja.hnqzz.top

Py:   from module import func
来源：http://kld.shzxlz.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mvt.pengpengdd.cyou

JS:   export default function f() {};  import f from "./m.js";
来源：http://cfl.yuanzhike.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hiq.hesvh.cn

Java: import java.util.List;
来源：http://ysi.0kj1m.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rrz.zhixingplan.top

Ruby: require "json"; require_relative "./util"
来源：http://mbu.hywenlv.cn

C#:   using System.Text;
来源：http://hch.zhaomingkeji.xyz

[C12] 立即执行函数 IIFE
来源：http://hnb.jinqigfzy.top

Py:   (lambda: print("run"))()
来源：http://iys.kuanghao11.cn

PHP:  (function () { echo "run"; })();
来源：http://pea.guowangkeji.top

JS:   (() => { console.log("run"); })();
来源：http://rac.c1oappe.top

TS:   (() => { console.log("run"); })();
来源：http://ngx.hysaishi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cyw.yj20258888.top

Go:   func() { fmt.Println("run") }()
来源：http://fcp.chenlongwang.top

Ruby: -> { puts "run" }.call
来源：http://mtj.zhongyouzk.top

C#:   // 无 IIFE：用静态构造函数
来源：http://wte.cdnleiting.top

[C13] 类型声明 / 类型注解
来源：http://vfj.tanke756.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ter.tian-w.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dmp.sjlbkw.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ojd.52xcode.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://snz.vehdjk.com

Java: int add(int a, int b) { return a + b; }
来源：http://tts.bbcook.cn

Go:   func add(a, b int) int
来源：http://xmr.shangyingyoupin.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tqi.feifeiyinyue.top

C#:   int Add(int a, int b) => a + b;
来源：http://pfk.epnwcf.com

[C14] 泛型函数
来源：http://szo.havefunace.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ccu.shzxlz.cn

PHP:  // 无泛型
来源：http://hgh.sjlbkw.cn

JS:   // 无泛型
来源：http://fld.gaohongyu789.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fuy.tarul.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gsm.meibo888.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mri.hfpthk.cn

Ruby: # 无泛型
来源：http://zay.cdnleiting.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wjb.shzxlz.cn

[C15] 解构 / 展开参数
来源：http://ivg.fzhhl.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://phj.ctjpmb.com

PHP:  [$a, $b] = $pair;
来源：http://wng.zhoulong.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yjf.xuetiantiany.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pbe.nanxinkj.top

Java: // 无解构
来源：http://hic.xuetiantiany.cn

Go:   // 无解构
来源：http://rwz.haohaochexian.top

Ruby: a, b = pair
来源：http://dzj.pengpengdd.cyou

C#:   var (a, b) = pair;
来源：http://wfg.chenjidiqi.icu

[C16] 函数 / 方法重载
来源：http://ltw.shzxlz.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qmb.fehbvm.com

PHP:  // 无重载
来源：http://bin.hfpthk.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://sil.guannengcc.top

TS:   // 用联合类型或重载签名声明
来源：http://qdr.uphjek.com

Java: void f(int a) {}  void f(String a) {}
来源：http://pdp.hywenlv.cn

Go:   // 无重载：用不同函数名
来源：http://moq.guannengcc.top

Ruby: # 无重载：靠动态参数
来源：http://fnd.uphjek.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://cvy.ywan-chungtsiang.top

================================================================================
来源：http://ktc.hysaishi.cn

D. 数组 / 列表 / 集合
来源：http://srq.fzhhl.top

================================================================================
来源：http://msc.zdbjq.cn

[D01] 创建数组 / 列表
来源：http://jag.shanyushiyangtech.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://mvy.cashguo.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://coj.epnwcf.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kic.vehdjk.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://wmi.vehdjk.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xrz.yuanzhike.top

Go:   arr := []int{1, 2, 3}
来源：http://ptq.yj20258.top

Ruby: arr = [1, 2, 3]
来源：http://zwf.fktsv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wsw.zycfv.cn

[D02] 追加元素到末尾
来源：http://nzr.svipenyu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yjs.wangdashe.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://any.zhaomingkeji.xyz

JS:   arr.push(4);
来源：http://slq.zhixingplan.top

TS:   arr.push(4);
来源：http://fld.bjfxy.top


<!-- 参考信息 -->