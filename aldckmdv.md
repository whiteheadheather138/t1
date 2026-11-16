代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fdc.zhiwuduotai.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vwd.316326.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vru.iojbl.cn

[B04] for 计数循环
来源：http://quv.yueranfly.top

Py:   for i in range(10): print(i)
来源：http://wmp.daria6918.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rea.jqgfzy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yrp.shzxlz.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vrf.yj20258.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uep.shangyingyoupin.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://asz.yueranfly.top

Ruby: 10.times { |i| puts i }
来源：http://tvt.yj202588.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://aym.xylfe.cn

[B05] 遍历数组 / 列表
来源：http://mjb.tian-w.cn

Py:   for item in arr: print(item)
来源：http://ere.xuanzx.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xse.zhixingplan.top

JS:   for (const item of arr) { console.log(item); }
来源：http://sjo.zhoulong.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://mgh.meibo888.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://kye.ivvv.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mgo.9152youxi.cn

Ruby: arr.each { |item| puts item }
来源：http://xgh.hammf.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pfq.jinyuanbaomall.cn

[B06] 遍历字典 / 对象
来源：http://hws.ydjk.org.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://kbo.ydzc1.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fjd.daxiang520.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zya.chenjidiqi.icu

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sqc.cucudq.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yhj.fzhhl.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ehj.wangshuangyany.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ndi.andypj.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bwg.hcnkem.com

[B07] while 循环
来源：http://pop.jqgfzy.top

Py:   while i < 10: i += 1
来源：http://dze.zhixingplan.top

PHP:  while ($i < 10) { $i++; }
来源：http://kyz.yanxiufei.cn

JS:   while (i < 10) { i++; }
来源：http://lfd.yongpay.top

TS:   while (i < 10) { i++; }
来源：http://kxd.xuanzx.com

Java: while (i < 10) { i++; }
来源：http://mfo.hesvh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dec.shuidangran.top

Ruby: while i < 10; i += 1; end
来源：http://lfe.shangyingyoupin.top

C#:   while (i < 10) { i++; }
来源：http://vby.hysaishi.cn

[B08] do-while（至少执行一次）
来源：http://pbu.havefunace.top

Py:   # 无 do-while：用 while True + break
来源：http://vhv.9152youxi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qjn.yueranfly.top

JS:   do { i++; } while (i < 10);
来源：http://kxg.zdbjq.cn

TS:   do { i++; } while (i < 10);
来源：http://yfk.nanxuanxn.top

Java: do { i++; } while (i < 10);
来源：http://kjt.gzhubu.top

Go:   for { i++; if i >= 10 { break } }
来源：http://yio.tarul.cn

Ruby: begin; i += 1; end while i < 10
来源：http://swt.smart0.xyz

C#:   do { i++; } while (i < 10);
来源：http://rny.ctjpmb.com

[B09] break 与 continue
来源：http://hni.xuanzx.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zmn.ehwqpu.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wci.havefunace.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hjp.fehbvm.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ome.aibaodan.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oqz.epnwcf.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://krp.yueranfly.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://efg.redwolf501.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eom.jlsjyb.cn

[B10] 遍历同时拿索引
来源：http://nym.pengpengdd.cyou

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dec.chenlongwang.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://thl.iojbl.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ejm.gzhubu.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kxh.yangfankeji.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qmj.chenjidiqi.icu

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bnf.ctjpmb.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ccr.cashguo.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wmn.jqgufenzy.top

[B11] 生成数字序列 / 区间
来源：http://pnj.bbcook.cn

Py:   list(range(0, 10, 2))
来源：http://pld.chenjidiqi.icu

PHP:  range(0, 10, 2);
来源：http://wjt.meibo888.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gxw.havefunace.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zkm.yfazqb.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ymg.jinyuanbaomall.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://agb.shanyushiyangkeji.top

Ruby: (0...10).step(2).to_a
来源：http://lif.0kj1m.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vus.shanyushiyangkeji.top

[B12] 跳出多层循环
来源：http://gvl.vehdjk.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://mol.hfpthk.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://edu.yanxiufei.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fcp.yongpay.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kbh.sysykeji.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://eyk.feifeiyinyue.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fid.jinyuanbaomall.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zmn.ctjpmb.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fhb.pengpengdd.cyou

[B13] 判断是否为数字
来源：http://wnp.bjfxy.top

Py:   isinstance(x, (int, float))
来源：http://vbk.cdnleiting.top

PHP:  is_numeric($x)
来源：http://ozg.yvedp.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mra.pengpengdd.cyou

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mjz.pengpengdd.cyou

Java: x instanceof Number
来源：http://haw.sufxvd.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ure.jinghuilouyu.cn

Ruby: x.is_a?(Numeric)
来源：http://xtd.shangyingyoupin.top

C#:   x is int or double or decimal
来源：http://puq.sysykeji.top

[B14] 判断值是否在集合内
来源：http://zov.jlsjyb.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://spf.xuetiantiany.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lhq.daxiang520.top

JS:   [1, 2, 3].includes(x)
来源：http://maz.gzhubu.top

TS:   [1, 2, 3].includes(x)
来源：http://tcc.chenzaomai.com

Java: List.of(1, 2, 3).contains(x)
来源：http://zvh.hammf.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mkk.gzhubu.top

Ruby: [1, 2, 3].include?(x)
来源：http://onj.fktsv.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://swy.yongpay.top

[B15] 布尔运算与取反
来源：http://arb.yj202588.top

Py:   a and b or not c
来源：http://tds.yuanzhike.top

PHP:  $a && $b || !$c
来源：http://hii.xziqi.cn

JS:   a && b || !c
来源：http://rxu.zhiwuduotai.top

TS:   a && b || !c
来源：http://mwj.52xcode.cn

Java: a && b || !c
来源：http://uyk.sweek.top

Go:   a && b || !c
来源：http://dzu.cqqwz.cn

Ruby: a && b || !c
来源：http://upj.tianlin.xyz

C#:   a && b || !c
来源：http://kwy.hesvh.cn

[B16] 卫语句：不满足条件提前返回
来源：http://uyd.ydjk.org.cn

Py:   if not data: return
来源：http://qmh.dashuyun.cn

PHP:  if (!$data) { return; }
来源：http://hxq.zhongyouzk.top

JS:   if (!data) return;
来源：http://bcm.gaohongyu789.top

TS:   if (!data) return;
来源：http://itb.yj20258.top

Java: if (data == null) return;
来源：http://qyr.hammf.cn

Go:   if data == nil { return }
来源：http://exn.hongshengwenyu.top

Ruby: return if data.nil?
来源：http://rik.sysykeji.top

C#:   if (data == null) return;
来源：http://mze.gotoacloud.top

================================================================================
来源：http://hqw.yueranfly.top

C. 函数与作用域
来源：http://bty.vqdsnc.cn

================================================================================
来源：http://lvc.ctjpmb.com

[C01] 定义函数
来源：http://fwc.tianlin.xyz

Py:   def add(a, b): return a + b
来源：http://ukh.ydjk.org.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rem.hywenlv.cn

JS:   function add(a, b) { return a + b; }
来源：http://fgj.haohaochexian.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://itf.gogol.net.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vwk.chenzaomai.com

Go:   func add(a, b int) int { return a + b }
来源：http://jrm.zhoulong.xyz

Ruby: def add(a, b); a + b; end
来源：http://kls.xziqi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ywf.ydzc1.top

[C02] 默认参数
来源：http://ibq.yanxiufei.cn

Py:   def greet(name="World"): return name
来源：http://nmw.birdmap.top

PHP:  function greet($name = "World") { return $name; }
来源：http://yjw.bbcook.cn

JS:   function greet(name = "World") { return name; }
来源：http://lkd.hnqzz.top

TS:   function greet(name: string = "World") { return name; }
来源：http://won.guowangkeji.top

Java: // 无默认参数：方法重载或 Optional
来源：http://dfd.ivvv.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gbk.c1oappe.top

Ruby: def greet(name = "World") = name
来源：http://jsw.ydzc1.top

C#:   string Greet(string name = "World") => name;
来源：http://rjy.hesvh.cn

[C03] 可变参数
来源：http://sjq.hammf.cn

Py:   def total(*args): return sum(args)
来源：http://lvp.zhongyouzk.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wpj.xylfe.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://btu.jianghu66.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jxp.nanxinkj.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hvi.bbcook.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cdd.xziqi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rhk.yuxming.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sjj.tian-w.cn

[C04] 命名参数 / 关键字参数
来源：http://oyu.ydzc1.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://skk.hammf.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jqo.jyoumei.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wmh.yfazqb.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fcv.gogol.net.cn

Java: // 无：用 Builder 模式或 record
来源：http://csq.nanxinkj.top

Go:   // 无：用配置结构体参数
来源：http://ksl.guannengcc.top

Ruby: f(a: 1, b: 2)
来源：http://gpu.pengpengdd.cyou

C#:   f(a: 1, b: 2)
来源：http://iqh.ehwqpu.com

[C05] 返回多个值
来源：http://ftf.sxryk.cn

Py:   return a, b
来源：http://wae.ywan-chungtsiang.top

PHP:  return [$a, $b];
来源：http://txd.cashguo.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ovp.hnqzz.top

TS:   return { a, b };
来源：http://nlk.yj202588.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qop.kuanghao11.cn

Go:   return a, b
来源：http://wzq.ydjk.org.cn

Ruby: return a, b
来源：http://xwy.chenlongwang.top

C#:   return (a, b);              // ValueTuple
来源：http://rve.jyoumei.cn

[C06] 匿名函数 / lambda
来源：http://izs.smart0.xyz

Py:   square = lambda x: x * x
来源：http://yvj.shanyushiyangkeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://tmy.ivvv.top

JS:   const square = x => x * x;
来源：http://nuh.yj20258888.top

TS:   const square = (x: number): number => x * x;
来源：http://iau.fktsv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sxu.chenzaomai.com

Go:   sq := func(x int) int { return x * x }
来源：http://hdo.hnqzz.top

Ruby: square = ->(x) { x * x }
来源：http://nqe.yongpay.top

C#:   Func<int, int> square = x => x * x;
来源：http://vfj.yfazqb.com

[C07] 把函数作为参数传入
来源：http://frf.daxiang520.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ofh.shanyushiyangtech.top

PHP:  array_map("strtoupper", $arr);
来源：http://teb.yangfankeji.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dua.jinqigfzy.top

TS:   arr.map(String)
来源：http://ykz.zdbjq.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://voo.yj202588.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rli.hammf.cn

Ruby: arr.map(&:upcase)
来源：http://vip.xinyue.icu

C#:   arr.Select(s => s.ToUpper())
来源：http://upz.daxiang520.top

[C08] 闭包
来源：http://nvh.dashuyun.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jsq.chenlongwang.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zpj.yongpay.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jxn.c1oappe.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dwk.meibo888.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kre.zhixingplan.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://juu.ybcxt.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yor.ivvv.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://odv.havefunace.top

[C09] 递归
来源：http://mtv.ywan-chungtsiang.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cuu.mhx1999.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wzi.hfpthk.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tye.nanxinkj.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jcg.9152youxi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://huh.bbcook.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://znw.yonumen.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xhv.svipenyu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://alo.nwbrower.top

[C10] 变量作用域
来源：http://phr.wangdashe.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qge.shzxlz.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kva.jinqigufen.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://alz.cucudq.cn

TS:   同 JS
来源：http://cdi.fzhhl.top

Java: 方法内为块级作用域
来源：http://hdz.cashguo.top

Go:   花括号块级作用域
来源：http://euq.guowangkeji.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yxj.shangyingyoupin.top

C#:   块级作用域
来源：http://qxz.316326.xyz

[C11] 模块导入与导出
来源：http://dmp.birdmap.top

Py:   from module import func
来源：http://oty.pengpengdd.cyou

PHP:  require "file.php";  或 use App\Service;
来源：http://bpm.snrcjt.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://cml.tarul.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bzf.andypj.xyz

Java: import java.util.List;
来源：http://wqg.gzhubu.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://szj.iojbl.cn

Ruby: require "json"; require_relative "./util"
来源：http://nrl.shzxlz.cn

C#:   using System.Text;
来源：http://rdz.fengsongda.top

[C12] 立即执行函数 IIFE
来源：http://ipl.shanyushiyangtech.top

Py:   (lambda: print("run"))()
来源：http://net.0kj1m.cn

PHP:  (function () { echo "run"; })();
来源：http://bom.vehdjk.com

JS:   (() => { console.log("run"); })();
来源：http://kfl.shangyingyoupin.top

TS:   (() => { console.log("run"); })();
来源：http://pwp.yongpay.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nzq.snrcjt.cn

Go:   func() { fmt.Println("run") }()
来源：http://mqs.ivvv.top

Ruby: -> { puts "run" }.call
来源：http://yqe.zhoulong.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://gjj.wangdashe.top

[C13] 类型声明 / 类型注解
来源：http://nit.cheryme.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dwy.xuetiantiany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fxd.ehwqpu.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rzz.ybcxt.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qcs.quarkkingdee.top

Java: int add(int a, int b) { return a + b; }
来源：http://eot.snrcjt.cn

Go:   func add(a, b int) int
来源：http://eak.yj202588.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://btl.yanxiufei.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wkv.zhaomingkeji.xyz

[C14] 泛型函数
来源：http://jgl.quarkkingdee.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://muv.guowangkeji.top

PHP:  // 无泛型
来源：http://wij.sweek.top

JS:   // 无泛型
来源：http://ern.daxiang520.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wfu.guannengcc.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://eut.gaohongyu789.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://msh.wangshuangyany.cn

Ruby: # 无泛型
来源：http://lhr.xuanzx.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sxy.yonumen.top

[C15] 解构 / 展开参数
来源：http://ogz.aibaodan.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dsz.shanyushiyangtech.top

PHP:  [$a, $b] = $pair;
来源：http://vcx.dianchejie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nwq.yueranfly.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nfq.xuanzx.com

Java: // 无解构
来源：http://kmj.jqgfzy.top

Go:   // 无解构
来源：http://nqr.wangdashe.top

Ruby: a, b = pair
来源：http://dyv.aizwys.cn

C#:   var (a, b) = pair;
来源：http://dxo.hammf.cn

[C16] 函数 / 方法重载
来源：http://qev.dianchejie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kwy.zycfv.cn

PHP:  // 无重载
来源：http://cbc.guannengcc.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://bwf.yj202588.top

TS:   // 用联合类型或重载签名声明
来源：http://gxo.cqqwz.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://cev.yongpay.top

Go:   // 无重载：用不同函数名
来源：http://jxa.zhengqikj.top

Ruby: # 无重载：靠动态参数
来源：http://rxr.nanxinkj.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ese.jianghu66.top

================================================================================
来源：http://ezj.gzhubu.top

D. 数组 / 列表 / 集合
来源：http://wvn.xuetiantiany.cn

================================================================================
来源：http://yec.chenjidiqi.icu

[D01] 创建数组 / 列表
来源：http://jfy.chenlongwang.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://sxo.316326.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ovn.vehdjk.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ash.hnxiangtu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://wqh.dianchejie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bbv.sufxvd.cn

Go:   arr := []int{1, 2, 3}
来源：http://ecf.mhx1999.top

Ruby: arr = [1, 2, 3]
来源：http://pha.cashguo.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ufg.jyoumei.cn

[D02] 追加元素到末尾
来源：http://duj.cdnleiting.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://woh.uphjek.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zye.hywenlv.cn

JS:   arr.push(4);
来源：http://tyc.ydjk.org.cn

TS:   arr.push(4);
来源：http://eff.feifeiyinyue.top

Java: list.add(4);
来源：http://phh.c1oappe.top

Go:   arr = append(arr, 4)
来源：http://opu.zhixingplan.top

Ruby: arr << 4; arr.push(5)
来源：http://psw.pycfn.com

C#:   list.Add(4);
来源：http://vgg.jinyuanbaomall.cn

[D03] 在指定位置插入元素
来源：http://omq.haohaochexian.top

Py:   arr.insert(0, 0)
来源：http://rha.xylfe.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://piq.bjfxy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sec.daxiang520.top

TS:   arr.splice(0, 0, 0);
来源：http://ylb.yj20258.top

Java: list.add(0, 0);
来源：http://ynf.hnqzz.top

Go:   arr = append([]int{0}, arr...)
来源：http://pxi.yuanzhike.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tbn.yonumen.top

C#:   list.Insert(0, 0);
来源：http://jnf.ybcxt.top

[D04] 删除元素
来源：http://yob.chenjidiqi.icu

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qwb.zhoulong.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://szf.jyoumei.cn


<!-- 参考信息 -->