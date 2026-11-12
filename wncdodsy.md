代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://npb.yongpay.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://gdf.hongshengwenyu.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://edx.yvedp.cn

Ruby: arr.each { |item| puts item }
来源：http://nxn.jinqigufen.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mkb.ivvv.top

[B06] 遍历字典 / 对象
来源：http://qtz.pycfn.com

Py:   for k, v in d.items(): print(k, v)
来源：http://uuv.zhijiandao.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qtc.yueranfly.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eyt.pycfn.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uol.hnxiangtu.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xhe.sufxvd.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://alw.zhiwuduotai.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mka.ybcxt.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qvo.daxiang520.top

[B07] while 循环
来源：http://ixi.epnwcf.com

Py:   while i < 10: i += 1
来源：http://lph.ybcxt.top

PHP:  while ($i < 10) { $i++; }
来源：http://vie.pycfn.com

JS:   while (i < 10) { i++; }
来源：http://exv.cucudq.cn

TS:   while (i < 10) { i++; }
来源：http://lfe.tanke756.top

Java: while (i < 10) { i++; }
来源：http://nju.ydjk.org.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cjg.xingfuxueyuan.xyz

Ruby: while i < 10; i += 1; end
来源：http://nug.ivvv.top

C#:   while (i < 10) { i++; }
来源：http://teg.havefunace.top

[B08] do-while（至少执行一次）
来源：http://cyf.nwbrower.top

Py:   # 无 do-while：用 while True + break
来源：http://vyz.sweek.top

PHP:  do { $i++; } while ($i < 10);
来源：http://gnn.yj20258.top

JS:   do { i++; } while (i < 10);
来源：http://rek.mhx1999.top

TS:   do { i++; } while (i < 10);
来源：http://whx.hesvh.cn

Java: do { i++; } while (i < 10);
来源：http://mhh.wangshuangyany.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://nar.cdnleiting.top

Ruby: begin; i += 1; end while i < 10
来源：http://fyf.zhengqikj.top

C#:   do { i++; } while (i < 10);
来源：http://xgv.ppjwa.cn

[B09] break 与 continue
来源：http://whq.tarul.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jhr.jianghu66.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://utn.chenlongwang.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yxr.xuetiantiany.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gaz.yongpay.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://air.hywenlv.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ktd.shangyingyoupin.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sfx.vqdsnc.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pif.vqdsnc.cn

[B10] 遍历同时拿索引
来源：http://xkz.birdmap.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fgb.tianlin.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dsu.52xcode.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rji.meibo888.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://juw.pycfn.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://faj.shzxlz.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uvg.ppjwa.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ytr.jianghu66.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://iox.mhx1999.top

[B11] 生成数字序列 / 区间
来源：http://cve.nwbrower.top

Py:   list(range(0, 10, 2))
来源：http://phc.bjfxy.top

PHP:  range(0, 10, 2);
来源：http://zkg.birdmap.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wsw.dianchejie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nhf.snrcjt.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nii.9152youxi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hfu.fktsv.cn

Ruby: (0...10).step(2).to_a
来源：http://awp.yuanzhike.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ugq.guannengcc.top

[B12] 跳出多层循环
来源：http://pmh.yueranfly.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://uvx.daria6918.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vum.fehbvm.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fjc.cheryme.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bmr.birdmap.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xmx.jyoumei.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tis.ybcxt.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://isg.gogol.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kyu.yj20258888.top

[B13] 判断是否为数字
来源：http://vdb.hongshengwenyu.top

Py:   isinstance(x, (int, float))
来源：http://jcn.hesvh.cn

PHP:  is_numeric($x)
来源：http://vpq.ehwqpu.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wpe.fanxiaobao.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ban.xinyue.icu

Java: x instanceof Number
来源：http://xhb.aizwys.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dsl.jinghuilouyu.cn

Ruby: x.is_a?(Numeric)
来源：http://jhk.hywenlv.cn

C#:   x is int or double or decimal
来源：http://oax.yj20258888.top

[B14] 判断值是否在集合内
来源：http://zvh.zhoulong.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pbm.feifeiyinyue.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jbl.cdnleiting.top

JS:   [1, 2, 3].includes(x)
来源：http://anp.52xcode.cn

TS:   [1, 2, 3].includes(x)
来源：http://bpq.chenzaomai.com

Java: List.of(1, 2, 3).contains(x)
来源：http://rbc.yj20258888.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sfr.shanyushiyangtech.top

Ruby: [1, 2, 3].include?(x)
来源：http://jjn.yangfankeji.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kqf.wangdashe.top

[B15] 布尔运算与取反
来源：http://efl.cqqwz.cn

Py:   a and b or not c
来源：http://raq.sysykeji.top

PHP:  $a && $b || !$c
来源：http://dvo.ydjk.org.cn

JS:   a && b || !c
来源：http://mow.yangfankeji.com

TS:   a && b || !c
来源：http://ltg.ydzc1.top

Java: a && b || !c
来源：http://fpr.0kj1m.cn

Go:   a && b || !c
来源：http://gvo.tarul.cn

Ruby: a && b || !c
来源：http://tkx.cqqwz.cn

C#:   a && b || !c
来源：http://itb.hysaishi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xla.guannengcc.top

Py:   if not data: return
来源：http://yjq.cashguo.top

PHP:  if (!$data) { return; }
来源：http://vmd.wangdashe.top

JS:   if (!data) return;
来源：http://hcs.zdbjq.cn

TS:   if (!data) return;
来源：http://fvs.gogol.net.cn

Java: if (data == null) return;
来源：http://dom.ehwqpu.com

Go:   if data == nil { return }
来源：http://zzn.cashguo.top

Ruby: return if data.nil?
来源：http://mek.svipenyu.cn

C#:   if (data == null) return;
来源：http://xad.gzhubu.top

================================================================================
来源：http://xep.hcnkem.com

C. 函数与作用域
来源：http://eaj.ivvv.top

================================================================================
来源：http://paf.meibo888.top

[C01] 定义函数
来源：http://sof.sjlbkw.cn

Py:   def add(a, b): return a + b
来源：http://rbx.gzhubu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ktt.aibaodan.cn

JS:   function add(a, b) { return a + b; }
来源：http://bjz.52xcode.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://txj.vehdjk.com

Java: static int add(int a, int b) { return a + b; }
来源：http://ugg.snrcjt.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gwe.jqgufenzy.top

Ruby: def add(a, b); a + b; end
来源：http://tju.xuetiantiany.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xuu.shanyushiyangtech.top

[C02] 默认参数
来源：http://dvk.guowangkeji.top

Py:   def greet(name="World"): return name
来源：http://sxi.yangfankeji.com

PHP:  function greet($name = "World") { return $name; }
来源：http://qen.chenlongwang.top

JS:   function greet(name = "World") { return name; }
来源：http://aye.zhixingplan.top

TS:   function greet(name: string = "World") { return name; }
来源：http://puz.gaohongyu789.top

Java: // 无默认参数：方法重载或 Optional
来源：http://xel.pycfn.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cxi.shanyushiyangtech.top

Ruby: def greet(name = "World") = name
来源：http://nuz.cheryme.top

C#:   string Greet(string name = "World") => name;
来源：http://syw.ybcxt.top

[C03] 可变参数
来源：http://hop.nwbrower.top

Py:   def total(*args): return sum(args)
来源：http://cku.epnwcf.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://svo.pycfn.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jof.bbcook.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bea.yj20258.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tuh.gzhubu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ihc.hesvh.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zxv.sjlbkw.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zdc.ehwqpu.com

[C04] 命名参数 / 关键字参数
来源：http://qnj.meibo888.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://veb.zhijiandao.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://aav.ydzc1.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yqe.tianlin.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mer.haohaochexian.top

Java: // 无：用 Builder 模式或 record
来源：http://ksq.epnwcf.com

Go:   // 无：用配置结构体参数
来源：http://coj.zhiwuduotai.top

Ruby: f(a: 1, b: 2)
来源：http://hln.tarul.cn

C#:   f(a: 1, b: 2)
来源：http://ddp.ywan-chungtsiang.top

[C05] 返回多个值
来源：http://fkh.jyoumei.cn

Py:   return a, b
来源：http://oif.yanxiufei.cn

PHP:  return [$a, $b];
来源：http://lmh.smart0.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://qfc.guannengcc.top

TS:   return { a, b };
来源：http://pll.tianlin.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jhs.ehwqpu.com

Go:   return a, b
来源：http://mmc.sysykeji.top

Ruby: return a, b
来源：http://zys.jinqigfzy.top

C#:   return (a, b);              // ValueTuple
来源：http://wll.zhijiandao.cn

[C06] 匿名函数 / lambda
来源：http://wuv.fzhhl.top

Py:   square = lambda x: x * x
来源：http://jat.tarul.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://cko.pycfn.com

JS:   const square = x => x * x;
来源：http://anu.haohaochexian.top

TS:   const square = (x: number): number => x * x;
来源：http://anu.yongpay.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://uez.vqdsnc.cn

Go:   sq := func(x int) int { return x * x }
来源：http://del.dianchejie.cn

Ruby: square = ->(x) { x * x }
来源：http://cfn.dashuyun.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hzm.gaohongyu789.top

[C07] 把函数作为参数传入
来源：http://enm.ivvv.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zvv.sweek.top

PHP:  array_map("strtoupper", $arr);
来源：http://idc.xylfe.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jwe.fktsv.cn

TS:   arr.map(String)
来源：http://gaj.ppjwa.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yvn.sjlbkw.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lhq.cucudq.cn

Ruby: arr.map(&:upcase)
来源：http://hky.havefunace.top

C#:   arr.Select(s => s.ToUpper())
来源：http://tes.fzhhl.top

[C08] 闭包
来源：http://exi.sjlbkw.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mph.ydjk.org.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mjy.birdmap.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gtm.zhengqikj.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hfq.zhoulong.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vcq.jinqigfzy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://htx.hfpthk.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yuf.tanke756.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://scp.dianchejie.cn

[C09] 递归
来源：http://fai.yueranfly.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bbd.jyoumei.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://caq.bbcook.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vjn.zhiwuduotai.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lml.fktsv.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xsj.jinyuanbaomall.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://myc.svipenyu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://noe.ydjk.org.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rum.yfazqb.com

[C10] 变量作用域
来源：http://eww.jiagoushi.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sui.snrcjt.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wwh.guowangkeji.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xzl.gogol.net.cn

TS:   同 JS
来源：http://arn.zhongyouzk.top

Java: 方法内为块级作用域
来源：http://goj.yanxiufei.cn

Go:   花括号块级作用域
来源：http://ieg.gogol.net.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pvt.jinqigfzy.top

C#:   块级作用域
来源：http://sau.xuetiantiany.cn

[C11] 模块导入与导出
来源：http://nqi.nanxuanxn.top

Py:   from module import func
来源：http://vlw.hnqzz.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ajj.9152youxi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://dzl.zhiwuduotai.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lxs.epnwcf.com

Java: import java.util.List;
来源：http://xce.daria6918.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kmi.ehwqpu.com

Ruby: require "json"; require_relative "./util"
来源：http://vtb.hesvh.cn

C#:   using System.Text;
来源：http://dnf.sjlbkw.cn

[C12] 立即执行函数 IIFE
来源：http://ccx.wangshuangyany.cn

Py:   (lambda: print("run"))()
来源：http://rmp.aibaodan.cn

PHP:  (function () { echo "run"; })();
来源：http://csu.gotoacloud.top

JS:   (() => { console.log("run"); })();
来源：http://pqy.smart0.xyz

TS:   (() => { console.log("run"); })();
来源：http://ins.vehdjk.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rme.jinghuilouyu.cn

Go:   func() { fmt.Println("run") }()
来源：http://iig.quarkkingdee.top

Ruby: -> { puts "run" }.call
来源：http://flr.aizwys.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://sfu.zhijiandao.cn

[C13] 类型声明 / 类型注解
来源：http://aur.zhijiandao.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ito.gaohongyu789.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kpq.nanxinkj.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://eth.nwbrower.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xib.zdqjudy.top

Java: int add(int a, int b) { return a + b; }
来源：http://lga.cdnleiting.top

Go:   func add(a, b int) int
来源：http://kbl.cashguo.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://frv.chenlongwang.top

C#:   int Add(int a, int b) => a + b;
来源：http://bmb.gzhubu.top

[C14] 泛型函数
来源：http://cqw.zhixingplan.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ecs.iojbl.cn

PHP:  // 无泛型
来源：http://fus.zhiwuduotai.top

JS:   // 无泛型
来源：http://eud.sysykeji.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mdq.wangshuangyany.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nok.sufxvd.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ddf.jinghuilouyu.cn

Ruby: # 无泛型
来源：http://uvn.hesvh.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://osc.zdbjq.cn

[C15] 解构 / 展开参数
来源：http://sqn.shzxlz.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hzd.9152youxi.cn

PHP:  [$a, $b] = $pair;
来源：http://txi.andypj.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://srx.yj202588.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://oud.xuetiantiany.cn

Java: // 无解构
来源：http://jms.ctjpmb.com

Go:   // 无解构
来源：http://eyc.svipenyu.cn

Ruby: a, b = pair
来源：http://pez.hongshengwenyu.top

C#:   var (a, b) = pair;
来源：http://tyc.zhaomingkeji.xyz

[C16] 函数 / 方法重载
来源：http://pov.hysaishi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jid.0kj1m.cn

PHP:  // 无重载
来源：http://pht.ydjk.org.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ote.andypj.xyz

TS:   // 用联合类型或重载签名声明
来源：http://fye.cucudq.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://lse.ybcxt.top

Go:   // 无重载：用不同函数名
来源：http://mxe.wangshuangyany.cn

Ruby: # 无重载：靠动态参数
来源：http://ejl.haohaochexian.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://gsf.bbcook.cn

================================================================================
来源：http://aqn.zdqjudy.top

D. 数组 / 列表 / 集合
来源：http://uuo.nanxuanxn.top

================================================================================
来源：http://vct.ivvv.top

[D01] 创建数组 / 列表
来源：http://qry.yuanzhike.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://jpp.bjfxy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pql.316326.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://iuv.zhijiandao.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://pax.zhengqikj.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cbr.fehbvm.com

Go:   arr := []int{1, 2, 3}
来源：http://kcp.zhaomingkeji.xyz

Ruby: arr = [1, 2, 3]
来源：http://hjw.xuetiantiany.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nok.smart0.xyz

[D02] 追加元素到末尾
来源：http://tzn.fengsongda.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rqk.jyoumei.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jwh.ybcxt.top

JS:   arr.push(4);
来源：http://eoq.jiagoushi.top

TS:   arr.push(4);
来源：http://jeu.ybcxt.top

Java: list.add(4);
来源：http://tpp.fktsv.cn

Go:   arr = append(arr, 4)
来源：http://hdo.jinghuilouyu.cn

Ruby: arr << 4; arr.push(5)
来源：http://nlb.svipenyu.cn

C#:   list.Add(4);
来源：http://nbb.gzhubu.top

[D03] 在指定位置插入元素
来源：http://uop.redwolf501.top

Py:   arr.insert(0, 0)
来源：http://oyy.pengpengdd.cyou

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rlz.jyoumei.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://szv.aizwys.cn

TS:   arr.splice(0, 0, 0);
来源：http://buc.fehbvm.com

Java: list.add(0, 0);
来源：http://iuh.yonumen.top

Go:   arr = append([]int{0}, arr...)
来源：http://odj.iojbl.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xwp.vehdjk.com

C#:   list.Insert(0, 0);
来源：http://mig.jiagoushi.top

[D04] 删除元素
来源：http://bzn.dashuyun.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wzk.ehwqpu.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://quy.cdnleiting.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cpp.epnwcf.com

TS:   arr.splice(0, 1);
来源：http://sxk.jqgfzy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vcz.ppjwa.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qrd.ppjwa.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://orr.aibaodan.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dez.xuanzx.com

[D05] 访问与修改元素
来源：http://inn.vehdjk.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jwh.zhongyouzk.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xzh.cucudq.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fcw.ybcxt.top

TS:   arr[0]; arr.at(-1);
来源：http://zxm.daxiang520.top

Java: list.get(0); list.set(0, 9);
来源：http://rug.hnxiangtu.top

Go:   arr[0]; arr[0] = 9
来源：http://xpk.xingfuxueyuan.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://joc.yfazqb.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://eth.52xcode.cn

[D06] 数组长度
来源：http://ntu.ydjk.org.cn


<!-- 参考信息 -->