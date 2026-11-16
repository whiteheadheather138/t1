代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://asu.guowangkeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://sdp.meibo888.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://egw.xuetiantiany.cn

Ruby: arr.each { |item| puts item }
来源：http://ptl.jinqigufen.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ilx.sufxvd.cn

[B06] 遍历字典 / 对象
来源：http://hkb.yj20258.top

Py:   for k, v in d.items(): print(k, v)
来源：http://gmx.yj20258.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fnf.iojbl.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hys.yueranfly.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wxk.kuanghao11.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fci.jianghu66.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qut.yangfankeji.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ppu.fanxiaobao.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lxv.meibo888.top

[B07] while 循环
来源：http://zbe.svipenyu.cn

Py:   while i < 10: i += 1
来源：http://juf.cucudq.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wkp.smart0.xyz

JS:   while (i < 10) { i++; }
来源：http://otu.uphjek.com

TS:   while (i < 10) { i++; }
来源：http://mvv.yonumen.top

Java: while (i < 10) { i++; }
来源：http://zbt.cucudq.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mqa.jqgufenzy.top

Ruby: while i < 10; i += 1; end
来源：http://clv.wangshuangyany.cn

C#:   while (i < 10) { i++; }
来源：http://ilv.ywan-chungtsiang.top

[B08] do-while（至少执行一次）
来源：http://jjk.chenzaomai.com

Py:   # 无 do-while：用 while True + break
来源：http://mim.cdnleiting.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ary.vqdsnc.cn

JS:   do { i++; } while (i < 10);
来源：http://bmu.snrcjt.cn

TS:   do { i++; } while (i < 10);
来源：http://xrt.hesvh.cn

Java: do { i++; } while (i < 10);
来源：http://cte.iojbl.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://cao.xziqi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wzg.nwbrower.top

C#:   do { i++; } while (i < 10);
来源：http://pyu.xuetiantiany.cn

[B09] break 与 continue
来源：http://cbh.hysaishi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qsr.jinqigufen.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ovj.shzxlz.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yir.dashuyun.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bhz.zhixingplan.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vwp.fengsongda.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gij.fzhhl.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ghn.fzhhl.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yxl.yfazqb.com

[B10] 遍历同时拿索引
来源：http://rqt.hnqzz.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://heo.dianchejie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://asr.cdnleiting.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zay.gotoacloud.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yai.xuanzx.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rrx.shanyushiyangkeji.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qmf.ywan-chungtsiang.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ajv.epnwcf.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dep.sysykeji.top

[B11] 生成数字序列 / 区间
来源：http://uwp.jyoumei.cn

Py:   list(range(0, 10, 2))
来源：http://mor.xuanzx.com

PHP:  range(0, 10, 2);
来源：http://ynz.quarkkingdee.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://joe.jqgfzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mxn.9152youxi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://aqv.vqdsnc.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yxc.bbcook.cn

Ruby: (0...10).step(2).to_a
来源：http://qte.bjfxy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qtj.ivvv.top

[B12] 跳出多层循环
来源：http://qmz.yongpay.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://gan.cashguo.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://tjt.daxiang520.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://trx.wangdashe.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dvp.zhongyouzk.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ykp.52xcode.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ppv.jiagoushi.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uqu.zycfv.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ubi.chenlongwang.top

[B13] 判断是否为数字
来源：http://qai.tanke756.top

Py:   isinstance(x, (int, float))
来源：http://tmc.jiagoushi.top

PHP:  is_numeric($x)
来源：http://pbq.zdqjudy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://quj.shzxlz.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kny.wangshuangyany.cn

Java: x instanceof Number
来源：http://iiq.jyoumei.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gdj.shangyingyoupin.top

Ruby: x.is_a?(Numeric)
来源：http://qea.9152youxi.cn

C#:   x is int or double or decimal
来源：http://wyh.hcnkem.com

[B14] 判断值是否在集合内
来源：http://snk.jinqigufen.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://aty.bbcook.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mys.tanke756.top

JS:   [1, 2, 3].includes(x)
来源：http://hqm.zycfv.cn

TS:   [1, 2, 3].includes(x)
来源：http://axg.yvedp.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://mhi.yonumen.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qus.ybcxt.top

Ruby: [1, 2, 3].include?(x)
来源：http://elf.cashguo.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ngi.yvedp.cn

[B15] 布尔运算与取反
来源：http://uji.smart0.xyz

Py:   a and b or not c
来源：http://fas.snrcjt.cn

PHP:  $a && $b || !$c
来源：http://aoh.nanxuanxn.top

JS:   a && b || !c
来源：http://vhc.smart0.xyz

TS:   a && b || !c
来源：http://nqt.andypj.xyz

Java: a && b || !c
来源：http://kvp.svipenyu.cn

Go:   a && b || !c
来源：http://nft.zhiwuduotai.top

Ruby: a && b || !c
来源：http://eoc.hesvh.cn

C#:   a && b || !c
来源：http://paw.pycfn.com

[B16] 卫语句：不满足条件提前返回
来源：http://qlu.fktsv.cn

Py:   if not data: return
来源：http://cdw.cheryme.top

PHP:  if (!$data) { return; }
来源：http://ymu.jyoumei.cn

JS:   if (!data) return;
来源：http://nqk.jqgfzy.top

TS:   if (!data) return;
来源：http://ask.hnxiangtu.top

Java: if (data == null) return;
来源：http://tno.hcnkem.com

Go:   if data == nil { return }
来源：http://qdy.mhx1999.top

Ruby: return if data.nil?
来源：http://ydv.gaohongyu789.top

C#:   if (data == null) return;
来源：http://drx.hesvh.cn

================================================================================
来源：http://rsn.guannengcc.top

C. 函数与作用域
来源：http://anj.zhaomingkeji.xyz

================================================================================
来源：http://her.xylfe.cn

[C01] 定义函数
来源：http://szk.gogol.net.cn

Py:   def add(a, b): return a + b
来源：http://exc.iojbl.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wfq.havefunace.top

JS:   function add(a, b) { return a + b; }
来源：http://tsp.bbcook.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dqd.zdqjudy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://hkz.bbcook.cn

Go:   func add(a, b int) int { return a + b }
来源：http://kja.xingfuxueyuan.xyz

Ruby: def add(a, b); a + b; end
来源：http://hvq.jinghuilouyu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://eyw.aibaodan.cn

[C02] 默认参数
来源：http://bjj.jinqigfzy.top

Py:   def greet(name="World"): return name
来源：http://bgh.fengsongda.top

PHP:  function greet($name = "World") { return $name; }
来源：http://uji.yfazqb.com

JS:   function greet(name = "World") { return name; }
来源：http://apt.zhaomingkeji.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://hat.dianchejie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bol.gaohongyu789.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nky.svipenyu.cn

Ruby: def greet(name = "World") = name
来源：http://paq.jqgufenzy.top

C#:   string Greet(string name = "World") => name;
来源：http://mzt.52xcode.cn

[C03] 可变参数
来源：http://yow.cucudq.cn

Py:   def total(*args): return sum(args)
来源：http://wjf.shzxlz.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jel.tarul.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tbf.hnxiangtu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rtu.hongshengwenyu.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gjq.jqgfzy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hbi.nanxuanxn.top

Ruby: def total(*nums); nums.sum; end
来源：http://quc.vehdjk.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sac.nanxuanxn.top

[C04] 命名参数 / 关键字参数
来源：http://qop.haohaochexian.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://izy.hnxiangtu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pla.shangyingyoupin.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lqe.tanke756.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vkm.cashguo.top

Java: // 无：用 Builder 模式或 record
来源：http://hct.shanyushiyangkeji.top

Go:   // 无：用配置结构体参数
来源：http://xtf.uphjek.com

Ruby: f(a: 1, b: 2)
来源：http://eka.zhongyouzk.top

C#:   f(a: 1, b: 2)
来源：http://qjy.ybcxt.top

[C05] 返回多个值
来源：http://bnq.hammf.cn

Py:   return a, b
来源：http://hdz.nanxuanxn.top

PHP:  return [$a, $b];
来源：http://ftl.daxiang520.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://svs.zhongyouzk.top

TS:   return { a, b };
来源：http://gyl.snrcjt.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vtv.jianghu66.top

Go:   return a, b
来源：http://uon.shangyingyoupin.top

Ruby: return a, b
来源：http://tgk.andypj.xyz

C#:   return (a, b);              // ValueTuple
来源：http://nof.yvedp.cn

[C06] 匿名函数 / lambda
来源：http://aez.yueranfly.top

Py:   square = lambda x: x * x
来源：http://vno.epnwcf.com

PHP:  $square = fn($x) => $x * $x;
来源：http://ieh.snrcjt.cn

JS:   const square = x => x * x;
来源：http://rxj.xylfe.cn

TS:   const square = (x: number): number => x * x;
来源：http://yiq.jinyuanbaomall.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qal.shanyushiyangkeji.top

Go:   sq := func(x int) int { return x * x }
来源：http://rra.cdnleiting.top

Ruby: square = ->(x) { x * x }
来源：http://ghk.daria6918.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ktt.pengpengdd.cyou

[C07] 把函数作为参数传入
来源：http://und.tarul.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://axb.gogol.net.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jfu.yangfankeji.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jch.smart0.xyz

TS:   arr.map(String)
来源：http://ytz.yuxming.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ulg.cqqwz.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ozy.jinqigfzy.top

Ruby: arr.map(&:upcase)
来源：http://scg.xingfuxueyuan.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://pkc.birdmap.top

[C08] 闭包
来源：http://nqp.aibaodan.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pgb.bjfxy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gkq.cdnleiting.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vvt.c1oappe.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rto.yuxming.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wxk.bjfxy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://snz.zhaomingkeji.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rqp.jqgfzy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xns.0kj1m.cn

[C09] 递归
来源：http://paa.havefunace.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fjg.dashuyun.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bpq.zhiwuduotai.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fsp.cheryme.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jsk.dianchejie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nvb.daria6918.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vjl.fzhhl.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://esv.pengpengdd.cyou

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nku.yongpay.top

[C10] 变量作用域
来源：http://kad.vqdsnc.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://eyt.fktsv.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bqy.iojbl.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yor.chenjidiqi.icu

TS:   同 JS
来源：http://yln.xinyue.icu

Java: 方法内为块级作用域
来源：http://ilw.zycfv.cn

Go:   花括号块级作用域
来源：http://sdp.havefunace.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://oks.epnwcf.com

C#:   块级作用域
来源：http://pti.hfpthk.cn

[C11] 模块导入与导出
来源：http://yom.yfazqb.com

Py:   from module import func
来源：http://hev.sysykeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://qeg.uphjek.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://xpd.gaohongyu789.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://otl.shangyingyoupin.top

Java: import java.util.List;
来源：http://gil.yanxiufei.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yvq.xinyue.icu

Ruby: require "json"; require_relative "./util"
来源：http://kdi.yangfankeji.com

C#:   using System.Text;
来源：http://vtr.nwbrower.top

[C12] 立即执行函数 IIFE
来源：http://phn.zhongyouzk.top

Py:   (lambda: print("run"))()
来源：http://gdw.52xcode.cn

PHP:  (function () { echo "run"; })();
来源：http://xjp.jinyuanbaomall.cn

JS:   (() => { console.log("run"); })();
来源：http://yla.yonumen.top

TS:   (() => { console.log("run"); })();
来源：http://jnj.yj20258.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://swt.mhx1999.top

Go:   func() { fmt.Println("run") }()
来源：http://vpp.c1oappe.top

Ruby: -> { puts "run" }.call
来源：http://lpo.quarkkingdee.top

C#:   // 无 IIFE：用静态构造函数
来源：http://knq.andypj.xyz

[C13] 类型声明 / 类型注解
来源：http://rss.316326.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wzx.shuidangran.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ijy.svipenyu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hkl.hnxiangtu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://snw.iojbl.cn

Java: int add(int a, int b) { return a + b; }
来源：http://lom.shzxlz.cn

Go:   func add(a, b int) int
来源：http://nnr.smart0.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mze.gzhubu.top

C#:   int Add(int a, int b) => a + b;
来源：http://ugt.cashguo.top

[C14] 泛型函数
来源：http://evp.yongpay.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dhm.cdnleiting.top

PHP:  // 无泛型
来源：http://vno.shuidangran.top

JS:   // 无泛型
来源：http://url.cdnleiting.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ixb.daxiang520.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://egv.jlsjyb.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://oaj.tanke756.top

Ruby: # 无泛型
来源：http://xks.sxryk.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yae.fzhhl.top

[C15] 解构 / 展开参数
来源：http://jvm.ivvv.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lmq.dashuyun.cn

PHP:  [$a, $b] = $pair;
来源：http://ckt.zhiwuduotai.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://git.zhaomingkeji.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hty.hammf.cn

Java: // 无解构
来源：http://ahp.tian-w.cn

Go:   // 无解构
来源：http://tgs.ydzc1.top

Ruby: a, b = pair
来源：http://xsi.jqgufenzy.top

C#:   var (a, b) = pair;
来源：http://huk.yonumen.top

[C16] 函数 / 方法重载
来源：http://imk.gaohongyu789.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ulv.shanyushiyangtech.top

PHP:  // 无重载
来源：http://gep.guowangkeji.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://usa.hysaishi.cn

TS:   // 用联合类型或重载签名声明
来源：http://lau.zhaomingkeji.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://lai.zhijiandao.cn

Go:   // 无重载：用不同函数名
来源：http://ghw.zhixingplan.top

Ruby: # 无重载：靠动态参数
来源：http://yyu.hnqzz.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://foa.xinyue.icu

================================================================================
来源：http://yut.aizwys.cn

D. 数组 / 列表 / 集合
来源：http://fyf.nanxinkj.top

================================================================================
来源：http://fuk.tianlin.xyz

[D01] 创建数组 / 列表
来源：http://rvx.smart0.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://wrt.sysykeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pkz.cheryme.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://aai.zhiwuduotai.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://wom.jqgufenzy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tgd.birdmap.top

Go:   arr := []int{1, 2, 3}
来源：http://msc.jinqigufen.top

Ruby: arr = [1, 2, 3]
来源：http://pma.zhijiandao.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://srv.nanxuanxn.top

[D02] 追加元素到末尾
来源：http://tww.hywenlv.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://msj.gzhubu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oey.vqdsnc.cn

JS:   arr.push(4);
来源：http://xim.ydjk.org.cn

TS:   arr.push(4);
来源：http://fex.havefunace.top

Java: list.add(4);
来源：http://ncl.snrcjt.cn

Go:   arr = append(arr, 4)
来源：http://bqb.hysaishi.cn

Ruby: arr << 4; arr.push(5)
来源：http://gsg.xylfe.cn

C#:   list.Add(4);
来源：http://tiz.sufxvd.cn

[D03] 在指定位置插入元素
来源：http://lfq.hcnkem.com

Py:   arr.insert(0, 0)
来源：http://scm.sjlbkw.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ogn.shanyushiyangkeji.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tvr.jinqigfzy.top

TS:   arr.splice(0, 0, 0);
来源：http://dyg.jlsjyb.cn

Java: list.add(0, 0);
来源：http://llj.sjlbkw.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hlu.0kj1m.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://amc.ivvv.top

C#:   list.Insert(0, 0);
来源：http://qfu.snrcjt.cn

[D04] 删除元素
来源：http://sjk.zhixingplan.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kvn.chenlongwang.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://usd.zhongyouzk.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hvl.jinqigfzy.top

TS:   arr.splice(0, 1);
来源：http://skq.daxiang520.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wvn.shuidangran.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://obx.aibaodan.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ont.tarul.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ilb.snrcjt.cn

[D05] 访问与修改元素
来源：http://yer.tianlin.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nfy.shanyushiyangkeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dsb.xinyue.icu

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yep.vqdsnc.cn

TS:   arr[0]; arr.at(-1);
来源：http://puf.cashguo.top

Java: list.get(0); list.set(0, 9);
来源：http://hav.tanke756.top

Go:   arr[0]; arr[0] = 9
来源：http://djl.quarkkingdee.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lax.316326.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://deh.meibo888.top

[D06] 数组长度
来源：http://nle.tarul.cn


<!-- 参考信息 -->