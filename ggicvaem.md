代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wdm.meibo888.top

[B02] 多分支 else if / elif
来源：http://kkn.ivvv.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rbz.jinyuanbaomall.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dcc.yongpay.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jdu.vqdsnc.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rde.guowangkeji.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dul.yfazqb.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mog.bbcook.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nkt.ydzc1.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qnp.xziqi.cn

[B03] switch / match / case
来源：http://qjq.bbcook.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yed.hesvh.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pxp.guowangkeji.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://irk.guannengcc.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sha.snrcjt.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rsc.tanke756.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://czj.feifeiyinyue.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xkq.nanxinkj.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qml.sweek.top

[B04] for 计数循环
来源：http://zye.zycfv.cn

Py:   for i in range(10): print(i)
来源：http://lyy.yj202588.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://niz.yuxming.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fev.yj20258888.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sgr.yj202588.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://inb.chenlongwang.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mdn.ctjpmb.com

Ruby: 10.times { |i| puts i }
来源：http://rqh.fktsv.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mzs.gogol.net.cn

[B05] 遍历数组 / 列表
来源：http://sze.xinyue.icu

Py:   for item in arr: print(item)
来源：http://ayw.meibo888.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ceu.tianlin.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://bcf.c1oappe.top

TS:   for (const item of arr) { console.log(item); }
来源：http://wxx.zhijiandao.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zhf.chenjidiqi.icu

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://szr.vqdsnc.cn

Ruby: arr.each { |item| puts item }
来源：http://uaq.shzxlz.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qrq.yueranfly.top

[B06] 遍历字典 / 对象
来源：http://rbn.52xcode.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://wcp.jinghuilouyu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ggf.tian-w.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ibx.mhx1999.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tzd.dianchejie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ugj.havefunace.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://aew.ydjk.org.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ttm.fehbvm.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bio.meibo888.top

[B07] while 循环
来源：http://geq.hnqzz.top

Py:   while i < 10: i += 1
来源：http://ani.andypj.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://joe.yuanzhike.top

JS:   while (i < 10) { i++; }
来源：http://osh.hammf.cn

TS:   while (i < 10) { i++; }
来源：http://xzh.zhixingplan.top

Java: while (i < 10) { i++; }
来源：http://wyq.meibo888.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ibn.tian-w.cn

Ruby: while i < 10; i += 1; end
来源：http://qnl.zhongyouzk.top

C#:   while (i < 10) { i++; }
来源：http://ygr.havefunace.top

[B08] do-while（至少执行一次）
来源：http://tkz.ppjwa.cn

Py:   # 无 do-while：用 while True + break
来源：http://dic.cashguo.top

PHP:  do { $i++; } while ($i < 10);
来源：http://loz.bbcook.cn

JS:   do { i++; } while (i < 10);
来源：http://aqy.andypj.xyz

TS:   do { i++; } while (i < 10);
来源：http://jny.xuanzx.com

Java: do { i++; } while (i < 10);
来源：http://xxr.yuxming.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://dou.sjlbkw.cn

Ruby: begin; i += 1; end while i < 10
来源：http://scn.smart0.xyz

C#:   do { i++; } while (i < 10);
来源：http://wuf.fzhhl.top

[B09] break 与 continue
来源：http://mbp.wangshuangyany.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://eax.hongshengwenyu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gaz.hnqzz.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rmd.zhongyouzk.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zaa.hnqzz.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pyc.yfazqb.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://amc.zdbjq.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ojk.tianlin.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zox.nwbrower.top

[B10] 遍历同时拿索引
来源：http://oyk.ehwqpu.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xav.52xcode.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://svk.sysykeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://efn.sxryk.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dtj.hysaishi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://huk.jinqigufen.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nrw.tarul.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xmb.ydjk.org.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qjl.daria6918.cn

[B11] 生成数字序列 / 区间
来源：http://tsn.nanxuanxn.top

Py:   list(range(0, 10, 2))
来源：http://exo.shanyushiyangtech.top

PHP:  range(0, 10, 2);
来源：http://szl.wangdashe.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fho.hysaishi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cmd.nanxinkj.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wda.yj202588.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gvy.gotoacloud.top

Ruby: (0...10).step(2).to_a
来源：http://qkf.0kj1m.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mwt.zdqjudy.top

[B12] 跳出多层循环
来源：http://uti.kuanghao11.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://mgp.feifeiyinyue.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://val.hesvh.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ajp.wangshuangyany.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pvf.tianlin.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xjr.bjfxy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nhh.shzxlz.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zyc.meibo888.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xck.yanxiufei.cn

[B13] 判断是否为数字
来源：http://jud.wangdashe.top

Py:   isinstance(x, (int, float))
来源：http://oqi.fktsv.cn

PHP:  is_numeric($x)
来源：http://icc.yvedp.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lmo.pycfn.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aqc.9152youxi.cn

Java: x instanceof Number
来源：http://hzs.haohaochexian.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vcx.316326.xyz

Ruby: x.is_a?(Numeric)
来源：http://hwo.uphjek.com

C#:   x is int or double or decimal
来源：http://koi.zhijiandao.cn

[B14] 判断值是否在集合内
来源：http://uub.dashuyun.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qfk.hnxiangtu.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://idf.gaohongyu789.top

JS:   [1, 2, 3].includes(x)
来源：http://joe.jinghuilouyu.cn

TS:   [1, 2, 3].includes(x)
来源：http://sxb.jinqigfzy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://gae.hesvh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nxt.jlsjyb.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zjj.jinyuanbaomall.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zah.jinyuanbaomall.cn

[B15] 布尔运算与取反
来源：http://khh.zhijiandao.cn

Py:   a and b or not c
来源：http://ptb.hongshengwenyu.top

PHP:  $a && $b || !$c
来源：http://owm.zdbjq.cn

JS:   a && b || !c
来源：http://mtg.zhoulong.xyz

TS:   a && b || !c
来源：http://lah.yonumen.top

Java: a && b || !c
来源：http://hwg.jinqigfzy.top

Go:   a && b || !c
来源：http://vnq.bjfxy.top

Ruby: a && b || !c
来源：http://hyy.yongpay.top

C#:   a && b || !c
来源：http://ews.fanxiaobao.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://qwv.ydzc1.top

Py:   if not data: return
来源：http://obb.zhijiandao.cn

PHP:  if (!$data) { return; }
来源：http://tzp.chenzaomai.com

JS:   if (!data) return;
来源：http://lyw.hongshengwenyu.top

TS:   if (!data) return;
来源：http://iwl.zdbjq.cn

Java: if (data == null) return;
来源：http://wiw.jlsjyb.cn

Go:   if data == nil { return }
来源：http://lvg.fehbvm.com

Ruby: return if data.nil?
来源：http://oxk.haohaochexian.top

C#:   if (data == null) return;
来源：http://bgj.nwbrower.top

================================================================================
来源：http://rmf.cucudq.cn

C. 函数与作用域
来源：http://ftz.gogol.net.cn

================================================================================
来源：http://nla.zhiwuduotai.top

[C01] 定义函数
来源：http://chc.gaohongyu789.top

Py:   def add(a, b): return a + b
来源：http://reh.sysykeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dbb.jqgfzy.top

JS:   function add(a, b) { return a + b; }
来源：http://aqe.shangyingyoupin.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kwg.dianchejie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://cub.bjfxy.top

Go:   func add(a, b int) int { return a + b }
来源：http://jmw.jianghu66.top

Ruby: def add(a, b); a + b; end
来源：http://rxx.jinghuilouyu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ryi.yj202588.top

[C02] 默认参数
来源：http://byf.nanxuanxn.top

Py:   def greet(name="World"): return name
来源：http://qap.guowangkeji.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ezn.haohaochexian.top

JS:   function greet(name = "World") { return name; }
来源：http://drp.zhijiandao.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cfa.smart0.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://ezc.feifeiyinyue.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tlg.zhijiandao.cn

Ruby: def greet(name = "World") = name
来源：http://zbx.jiagoushi.top

C#:   string Greet(string name = "World") => name;
来源：http://kao.dashuyun.cn

[C03] 可变参数
来源：http://wpz.hcnkem.com

Py:   def total(*args): return sum(args)
来源：http://djq.sufxvd.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mwt.sweek.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ffp.andypj.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gbu.mhx1999.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://iuq.jianghu66.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nzz.chenzaomai.com

Ruby: def total(*nums); nums.sum; end
来源：http://fxg.yj202588.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lkq.pengpengdd.cyou

[C04] 命名参数 / 关键字参数
来源：http://qce.pengpengdd.cyou

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wpo.guannengcc.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wrb.hywenlv.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://oyv.zhoulong.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rlg.aibaodan.cn

Java: // 无：用 Builder 模式或 record
来源：http://dce.xuanzx.com

Go:   // 无：用配置结构体参数
来源：http://tds.dianchejie.cn

Ruby: f(a: 1, b: 2)
来源：http://awp.kuanghao11.cn

C#:   f(a: 1, b: 2)
来源：http://zar.yangfankeji.com

[C05] 返回多个值
来源：http://wga.bbcook.cn

Py:   return a, b
来源：http://uuk.mhx1999.top

PHP:  return [$a, $b];
来源：http://sou.nanxuanxn.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://bhf.uphjek.com

TS:   return { a, b };
来源：http://ica.zycfv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lyn.vqdsnc.cn

Go:   return a, b
来源：http://ybx.zhixingplan.top

Ruby: return a, b
来源：http://dkp.yuanzhike.top

C#:   return (a, b);              // ValueTuple
来源：http://kjh.nwbrower.top

[C06] 匿名函数 / lambda
来源：http://shv.hnqzz.top

Py:   square = lambda x: x * x
来源：http://jku.zhengqikj.top

PHP:  $square = fn($x) => $x * $x;
来源：http://bui.andypj.xyz

JS:   const square = x => x * x;
来源：http://akr.hywenlv.cn

TS:   const square = (x: number): number => x * x;
来源：http://wdj.xinyue.icu

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ryi.svipenyu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gsn.dianchejie.cn

Ruby: square = ->(x) { x * x }
来源：http://rlp.hesvh.cn

C#:   Func<int, int> square = x => x * x;
来源：http://aye.svipenyu.cn

[C07] 把函数作为参数传入
来源：http://khq.fktsv.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vpd.sweek.top

PHP:  array_map("strtoupper", $arr);
来源：http://tqr.hysaishi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://htq.zhijiandao.cn

TS:   arr.map(String)
来源：http://gcs.gogol.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xlh.uphjek.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nkr.fktsv.cn

Ruby: arr.map(&:upcase)
来源：http://bha.shuidangran.top

C#:   arr.Select(s => s.ToUpper())
来源：http://kmz.sxryk.cn

[C08] 闭包
来源：http://hzr.kuanghao11.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pmy.tianlin.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cgu.dashuyun.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://llz.ydzc1.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kem.quarkkingdee.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gbv.hywenlv.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://iux.feifeiyinyue.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pvr.tanke756.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ixo.hfpthk.cn

[C09] 递归
来源：http://amg.yj20258.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bkf.hongshengwenyu.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://thb.fehbvm.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dhv.snrcjt.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ltd.zhaomingkeji.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wqa.iojbl.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://scb.tarul.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://etm.yj20258.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qvi.shangyingyoupin.top

[C10] 变量作用域
来源：http://pgn.xuetiantiany.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://djo.yanxiufei.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xya.ybcxt.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xzf.fehbvm.com

TS:   同 JS
来源：http://tsb.tian-w.cn

Java: 方法内为块级作用域
来源：http://qgn.hywenlv.cn

Go:   花括号块级作用域
来源：http://swg.cucudq.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wex.cucudq.cn

C#:   块级作用域
来源：http://izy.sweek.top

[C11] 模块导入与导出
来源：http://lxx.ywan-chungtsiang.top

Py:   from module import func
来源：http://mjg.daria6918.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://gti.ctjpmb.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://odz.guowangkeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hqs.mhx1999.top

Java: import java.util.List;
来源：http://jte.jinqigufen.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://puo.yj20258888.top

Ruby: require "json"; require_relative "./util"
来源：http://hgo.xuanzx.com

C#:   using System.Text;
来源：http://ysc.pycfn.com

[C12] 立即执行函数 IIFE
来源：http://wlw.hywenlv.cn

Py:   (lambda: print("run"))()
来源：http://qef.jinqigufen.top

PHP:  (function () { echo "run"; })();
来源：http://lak.hesvh.cn

JS:   (() => { console.log("run"); })();
来源：http://pzt.tianlin.xyz

TS:   (() => { console.log("run"); })();
来源：http://ire.fzhhl.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zfb.yangfankeji.com

Go:   func() { fmt.Println("run") }()
来源：http://raq.uphjek.com

Ruby: -> { puts "run" }.call
来源：http://pyn.feifeiyinyue.top

C#:   // 无 IIFE：用静态构造函数
来源：http://wjl.nanxuanxn.top

[C13] 类型声明 / 类型注解
来源：http://swr.zhongyouzk.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://las.bbcook.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uve.ivvv.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://luc.ppjwa.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jmw.9152youxi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://psq.ydjk.org.cn

Go:   func add(a, b int) int
来源：http://whz.hfpthk.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dim.andypj.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://dnz.jinqigfzy.top

[C14] 泛型函数
来源：http://vod.hfpthk.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://arv.jyoumei.cn

PHP:  // 无泛型
来源：http://axi.chenlongwang.top

JS:   // 无泛型
来源：http://pbk.yangfankeji.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wmo.snrcjt.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ipq.fanxiaobao.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kiu.kuanghao11.cn

Ruby: # 无泛型
来源：http://jgt.smart0.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mon.ywan-chungtsiang.top

[C15] 解构 / 展开参数
来源：http://zvl.hesvh.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bwl.tian-w.cn

PHP:  [$a, $b] = $pair;
来源：http://vfc.meibo888.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nkh.hysaishi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://toi.shzxlz.cn

Java: // 无解构
来源：http://rgi.jqgufenzy.top

Go:   // 无解构
来源：http://noh.ivvv.top

Ruby: a, b = pair
来源：http://lfv.vehdjk.com

C#:   var (a, b) = pair;
来源：http://ezc.meibo888.top

[C16] 函数 / 方法重载
来源：http://gyi.xinyue.icu

Py:   # 无重载：用默认参数或 *args 变通
来源：http://oez.hnxiangtu.top

PHP:  // 无重载
来源：http://kvs.zhiwuduotai.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://dwa.nanxinkj.top

TS:   // 用联合类型或重载签名声明
来源：http://aoa.gaohongyu789.top

Java: void f(int a) {}  void f(String a) {}
来源：http://gzf.ppjwa.cn

Go:   // 无重载：用不同函数名
来源：http://jkr.havefunace.top

Ruby: # 无重载：靠动态参数
来源：http://rth.ydzc1.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://owy.uphjek.com

================================================================================
来源：http://nyx.xziqi.cn

D. 数组 / 列表 / 集合
来源：http://rxn.yfazqb.com

================================================================================
来源：http://neq.xuanzx.com

[D01] 创建数组 / 列表
来源：http://ptz.chenzaomai.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://dek.redwolf501.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ovb.tianlin.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://txr.svipenyu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ils.chenjidiqi.icu

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fwn.9152youxi.cn

Go:   arr := []int{1, 2, 3}
来源：http://flp.xuanzx.com

Ruby: arr = [1, 2, 3]
来源：http://qxg.aibaodan.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qhp.tanke756.top

[D02] 追加元素到末尾
来源：http://phv.nanxinkj.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dfl.zhixingplan.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cwy.aibaodan.cn

JS:   arr.push(4);
来源：http://njj.andypj.xyz

TS:   arr.push(4);
来源：http://zyr.feifeiyinyue.top


<!-- 参考信息 -->