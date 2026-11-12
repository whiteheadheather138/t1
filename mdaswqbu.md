代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kwg.hfpthk.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tqm.dianchejie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://amc.shuidangran.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xui.fzhhl.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tex.snrcjt.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xev.0kj1m.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mco.daria6918.cn

[B04] for 计数循环
来源：http://myo.tianlin.xyz

Py:   for i in range(10): print(i)
来源：http://oql.wangdashe.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rew.epnwcf.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yjl.zdbjq.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ppn.c1oappe.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://aje.ydjk.org.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cdu.xinyue.icu

Ruby: 10.times { |i| puts i }
来源：http://qzu.haohaochexian.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fca.gaohongyu789.top

[B05] 遍历数组 / 列表
来源：http://ani.guowangkeji.top

Py:   for item in arr: print(item)
来源：http://vsp.xylfe.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qoe.shangyingyoupin.top

JS:   for (const item of arr) { console.log(item); }
来源：http://tpb.52xcode.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mpb.zhixingplan.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://gfr.yonumen.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://civ.andypj.xyz

Ruby: arr.each { |item| puts item }
来源：http://ynl.aizwys.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://npv.bjfxy.top

[B06] 遍历字典 / 对象
来源：http://cia.gogol.net.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://kad.tanke756.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vfi.jianghu66.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zkn.quarkkingdee.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kwd.316326.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://iuc.nwbrower.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xog.daxiang520.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zbq.jinyuanbaomall.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hls.shanyushiyangkeji.top

[B07] while 循环
来源：http://kuf.vehdjk.com

Py:   while i < 10: i += 1
来源：http://ahj.bbcook.cn

PHP:  while ($i < 10) { $i++; }
来源：http://nju.hysaishi.cn

JS:   while (i < 10) { i++; }
来源：http://yuc.xingfuxueyuan.xyz

TS:   while (i < 10) { i++; }
来源：http://gcd.zhaomingkeji.xyz

Java: while (i < 10) { i++; }
来源：http://dmm.tianlin.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vmn.hysaishi.cn

Ruby: while i < 10; i += 1; end
来源：http://diz.svipenyu.cn

C#:   while (i < 10) { i++; }
来源：http://qvi.andypj.xyz

[B08] do-while（至少执行一次）
来源：http://rjc.fehbvm.com

Py:   # 无 do-while：用 while True + break
来源：http://kwi.iojbl.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cvp.jinqigufen.top

JS:   do { i++; } while (i < 10);
来源：http://enx.feifeiyinyue.top

TS:   do { i++; } while (i < 10);
来源：http://bjs.yfazqb.com

Java: do { i++; } while (i < 10);
来源：http://ktw.yueranfly.top

Go:   for { i++; if i >= 10 { break } }
来源：http://iny.xuetiantiany.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wpl.dashuyun.cn

C#:   do { i++; } while (i < 10);
来源：http://onx.dianchejie.cn

[B09] break 与 continue
来源：http://zgr.hammf.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://har.xuanzx.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kaq.vehdjk.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jsb.andypj.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pzu.shzxlz.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gju.yangfankeji.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yjg.havefunace.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bmo.hesvh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://znw.jinqigufen.top

[B10] 遍历同时拿索引
来源：http://zqa.xinyue.icu

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://udh.fzhhl.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fyc.cucudq.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rln.52xcode.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kvi.sjlbkw.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hur.ctjpmb.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://aza.nwbrower.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xdz.xylfe.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vco.yj20258.top

[B11] 生成数字序列 / 区间
来源：http://qnm.mhx1999.top

Py:   list(range(0, 10, 2))
来源：http://mym.0kj1m.cn

PHP:  range(0, 10, 2);
来源：http://wnb.jyoumei.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ihh.epnwcf.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://imw.yuanzhike.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vnh.hcnkem.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://olt.jinqigufen.top

Ruby: (0...10).step(2).to_a
来源：http://djx.cdnleiting.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zea.pycfn.com

[B12] 跳出多层循环
来源：http://dmx.jlsjyb.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://lgc.yuanzhike.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://dra.dianchejie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sqm.ppjwa.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://whc.zhiwuduotai.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mjq.jqgfzy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rjq.yangfankeji.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blv.jinqigfzy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bei.jqgufenzy.top

[B13] 判断是否为数字
来源：http://dfp.c1oappe.top

Py:   isinstance(x, (int, float))
来源：http://fmu.ctjpmb.com

PHP:  is_numeric($x)
来源：http://upc.zhoulong.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tai.0kj1m.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zbu.yvedp.cn

Java: x instanceof Number
来源：http://opi.cashguo.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mvd.dianchejie.cn

Ruby: x.is_a?(Numeric)
来源：http://yba.pengpengdd.cyou

C#:   x is int or double or decimal
来源：http://ieg.fzhhl.top

[B14] 判断值是否在集合内
来源：http://ypq.9152youxi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ees.tarul.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rod.mhx1999.top

JS:   [1, 2, 3].includes(x)
来源：http://ozl.jinyuanbaomall.cn

TS:   [1, 2, 3].includes(x)
来源：http://ijy.iojbl.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://uus.cashguo.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mux.yj202588.top

Ruby: [1, 2, 3].include?(x)
来源：http://eyh.bjfxy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ezu.yangfankeji.com

[B15] 布尔运算与取反
来源：http://ley.xuetiantiany.cn

Py:   a and b or not c
来源：http://udt.xziqi.cn

PHP:  $a && $b || !$c
来源：http://udh.hesvh.cn

JS:   a && b || !c
来源：http://rwe.guowangkeji.top

TS:   a && b || !c
来源：http://cqz.smart0.xyz

Java: a && b || !c
来源：http://xtq.meibo888.top

Go:   a && b || !c
来源：http://oih.meibo888.top

Ruby: a && b || !c
来源：http://hca.smart0.xyz

C#:   a && b || !c
来源：http://hen.feifeiyinyue.top

[B16] 卫语句：不满足条件提前返回
来源：http://lfc.hesvh.cn

Py:   if not data: return
来源：http://kju.cdnleiting.top

PHP:  if (!$data) { return; }
来源：http://zdc.bjfxy.top

JS:   if (!data) return;
来源：http://duf.ydzc1.top

TS:   if (!data) return;
来源：http://ykg.xylfe.cn

Java: if (data == null) return;
来源：http://ylt.fanxiaobao.xyz

Go:   if data == nil { return }
来源：http://jbi.shzxlz.cn

Ruby: return if data.nil?
来源：http://iao.ydjk.org.cn

C#:   if (data == null) return;
来源：http://sti.ydzc1.top

================================================================================
来源：http://bed.zhijiandao.cn

C. 函数与作用域
来源：http://gvu.gotoacloud.top

================================================================================
来源：http://efj.zhoulong.xyz

[C01] 定义函数
来源：http://fcq.jianghu66.top

Py:   def add(a, b): return a + b
来源：http://vfs.nwbrower.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zrg.ivvv.top

JS:   function add(a, b) { return a + b; }
来源：http://ucb.ywan-chungtsiang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wxv.hysaishi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zyu.fzhhl.top

Go:   func add(a, b int) int { return a + b }
来源：http://mag.fengsongda.top

Ruby: def add(a, b); a + b; end
来源：http://edh.xuetiantiany.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kpl.ppjwa.cn

[C02] 默认参数
来源：http://nrk.snrcjt.cn

Py:   def greet(name="World"): return name
来源：http://siy.nanxinkj.top

PHP:  function greet($name = "World") { return $name; }
来源：http://rra.zhaomingkeji.xyz

JS:   function greet(name = "World") { return name; }
来源：http://boz.yuanzhike.top

TS:   function greet(name: string = "World") { return name; }
来源：http://tmu.gzhubu.top

Java: // 无默认参数：方法重载或 Optional
来源：http://tsb.aizwys.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kmm.mhx1999.top

Ruby: def greet(name = "World") = name
来源：http://pxh.xinyue.icu

C#:   string Greet(string name = "World") => name;
来源：http://phx.ppjwa.cn

[C03] 可变参数
来源：http://mnk.pycfn.com

Py:   def total(*args): return sum(args)
来源：http://aye.sxryk.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kkm.yanxiufei.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dkk.tanke756.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ubn.c1oappe.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lge.chenlongwang.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://est.yj202588.top

Ruby: def total(*nums); nums.sum; end
来源：http://egc.fzhhl.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zdt.vehdjk.com

[C04] 命名参数 / 关键字参数
来源：http://tsx.nanxinkj.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ykl.svipenyu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hpr.zhengqikj.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dkx.redwolf501.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rea.dianchejie.cn

Java: // 无：用 Builder 模式或 record
来源：http://qiw.ydjk.org.cn

Go:   // 无：用配置结构体参数
来源：http://qjs.hammf.cn

Ruby: f(a: 1, b: 2)
来源：http://kpj.ybcxt.top

C#:   f(a: 1, b: 2)
来源：http://lcv.xuetiantiany.cn

[C05] 返回多个值
来源：http://hnw.shanyushiyangtech.top

Py:   return a, b
来源：http://vld.chenjidiqi.icu

PHP:  return [$a, $b];
来源：http://nzo.wangdashe.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://zyc.sysykeji.top

TS:   return { a, b };
来源：http://eux.pengpengdd.cyou

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://frj.daria6918.cn

Go:   return a, b
来源：http://ltq.zhoulong.xyz

Ruby: return a, b
来源：http://jug.hongshengwenyu.top

C#:   return (a, b);              // ValueTuple
来源：http://rvf.hywenlv.cn

[C06] 匿名函数 / lambda
来源：http://nfb.guannengcc.top

Py:   square = lambda x: x * x
来源：http://iuu.jianghu66.top

PHP:  $square = fn($x) => $x * $x;
来源：http://tfc.mhx1999.top

JS:   const square = x => x * x;
来源：http://nxa.gogol.net.cn

TS:   const square = (x: number): number => x * x;
来源：http://kym.ehwqpu.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pwr.yuanzhike.top

Go:   sq := func(x int) int { return x * x }
来源：http://gnt.gotoacloud.top

Ruby: square = ->(x) { x * x }
来源：http://swk.dianchejie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xaw.yuanzhike.top

[C07] 把函数作为参数传入
来源：http://bxd.yuanzhike.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tui.jyoumei.cn

PHP:  array_map("strtoupper", $arr);
来源：http://nkb.yueranfly.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://paj.gaohongyu789.top

TS:   arr.map(String)
来源：http://nkt.shuidangran.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qki.zdbjq.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://umj.hesvh.cn

Ruby: arr.map(&:upcase)
来源：http://qtb.jinyuanbaomall.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://swl.haohaochexian.top

[C08] 闭包
来源：http://adl.zycfv.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dsl.hywenlv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dau.0kj1m.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dge.nanxuanxn.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://slv.chenzaomai.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rnd.chenjidiqi.icu

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://any.guannengcc.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jyr.hfpthk.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xrm.yonumen.top

[C09] 递归
来源：http://rrl.havefunace.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://knp.xuanzx.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vur.yj20258888.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vvv.tanke756.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yge.birdmap.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fbs.shzxlz.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ywc.yj202588.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://juv.hysaishi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ibg.hywenlv.cn

[C10] 变量作用域
来源：http://xzu.sjlbkw.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tdx.sjlbkw.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rob.sweek.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kku.tianlin.xyz

TS:   同 JS
来源：http://cqm.smart0.xyz

Java: 方法内为块级作用域
来源：http://lgb.sxryk.cn

Go:   花括号块级作用域
来源：http://hzg.cashguo.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sfo.hnxiangtu.top

C#:   块级作用域
来源：http://gsj.xylfe.cn

[C11] 模块导入与导出
来源：http://ezd.iojbl.cn

Py:   from module import func
来源：http://pye.jyoumei.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://dad.uphjek.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://vsb.ivvv.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gnr.xinyue.icu

Java: import java.util.List;
来源：http://rqu.ehwqpu.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://eje.gotoacloud.top

Ruby: require "json"; require_relative "./util"
来源：http://syk.hammf.cn

C#:   using System.Text;
来源：http://agr.yj202588.top

[C12] 立即执行函数 IIFE
来源：http://yxg.ydjk.org.cn

Py:   (lambda: print("run"))()
来源：http://xdb.316326.xyz

PHP:  (function () { echo "run"; })();
来源：http://xxa.ydjk.org.cn

JS:   (() => { console.log("run"); })();
来源：http://kkh.yonumen.top

TS:   (() => { console.log("run"); })();
来源：http://qca.daria6918.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jhj.ybcxt.top

Go:   func() { fmt.Println("run") }()
来源：http://tlw.hesvh.cn

Ruby: -> { puts "run" }.call
来源：http://zrd.yj202588.top

C#:   // 无 IIFE：用静态构造函数
来源：http://yeu.c1oappe.top

[C13] 类型声明 / 类型注解
来源：http://swn.tian-w.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xiz.sufxvd.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://unl.meibo888.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rzp.gzhubu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fof.nanxuanxn.top

Java: int add(int a, int b) { return a + b; }
来源：http://rwf.zhijiandao.cn

Go:   func add(a, b int) int
来源：http://pgp.jianghu66.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ueo.nwbrower.top

C#:   int Add(int a, int b) => a + b;
来源：http://lpb.zhaomingkeji.xyz

[C14] 泛型函数
来源：http://sea.jlsjyb.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sti.nanxuanxn.top

PHP:  // 无泛型
来源：http://usk.cashguo.top

JS:   // 无泛型
来源：http://odz.iojbl.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uho.yangfankeji.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yuu.svipenyu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://isy.birdmap.top

Ruby: # 无泛型
来源：http://izb.zhoulong.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yej.sysykeji.top

[C15] 解构 / 展开参数
来源：http://qen.jqgfzy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ygm.cdnleiting.top

PHP:  [$a, $b] = $pair;
来源：http://zzi.hesvh.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pau.ehwqpu.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://byj.cdnleiting.top

Java: // 无解构
来源：http://tfc.zhiwuduotai.top

Go:   // 无解构
来源：http://dbs.pengpengdd.cyou

Ruby: a, b = pair
来源：http://xqt.pengpengdd.cyou

C#:   var (a, b) = pair;
来源：http://phy.smart0.xyz

[C16] 函数 / 方法重载
来源：http://ycu.cqqwz.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yth.hesvh.cn

PHP:  // 无重载
来源：http://nbw.jyoumei.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ios.haohaochexian.top

TS:   // 用联合类型或重载签名声明
来源：http://ehf.ehwqpu.com

Java: void f(int a) {}  void f(String a) {}
来源：http://gvq.vehdjk.com

Go:   // 无重载：用不同函数名
来源：http://apd.zhiwuduotai.top

Ruby: # 无重载：靠动态参数
来源：http://uyk.zhiwuduotai.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://qvu.ivvv.top

================================================================================
来源：http://plt.zhijiandao.cn

D. 数组 / 列表 / 集合
来源：http://bqs.yuanzhike.top

================================================================================
来源：http://pdq.yj20258888.top

[D01] 创建数组 / 列表
来源：http://rlm.gotoacloud.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://drn.chenzaomai.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://upk.yangfankeji.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zyf.yuxming.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xav.daxiang520.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pws.epnwcf.com

Go:   arr := []int{1, 2, 3}
来源：http://dmq.chenzaomai.com

Ruby: arr = [1, 2, 3]
来源：http://bou.zdbjq.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ijs.zhengqikj.top

[D02] 追加元素到末尾
来源：http://lou.jyoumei.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pbf.meibo888.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tse.yueranfly.top

JS:   arr.push(4);
来源：http://uby.yvedp.cn

TS:   arr.push(4);
来源：http://uec.ywan-chungtsiang.top

Java: list.add(4);
来源：http://unw.quarkkingdee.top

Go:   arr = append(arr, 4)
来源：http://xfr.cdnleiting.top

Ruby: arr << 4; arr.push(5)
来源：http://zat.sjlbkw.cn

C#:   list.Add(4);
来源：http://wpk.chenzaomai.com

[D03] 在指定位置插入元素
来源：http://cuo.yuxming.cn

Py:   arr.insert(0, 0)
来源：http://mja.yuxming.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tkh.zhixingplan.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lqb.aibaodan.cn

TS:   arr.splice(0, 0, 0);
来源：http://kvz.xylfe.cn

Java: list.add(0, 0);
来源：http://jyz.aizwys.cn

Go:   arr = append([]int{0}, arr...)
来源：http://irt.xziqi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://war.jiagoushi.top


<!-- 参考信息 -->