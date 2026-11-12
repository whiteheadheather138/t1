代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://lbo.jianghu66.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ihm.zhaomingkeji.xyz

JS:   do { i++; } while (i < 10);
来源：http://jti.zycfv.cn

TS:   do { i++; } while (i < 10);
来源：http://pad.yj20258.top

Java: do { i++; } while (i < 10);
来源：http://jvg.sxryk.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://zwf.sxryk.cn

Ruby: begin; i += 1; end while i < 10
来源：http://bba.nwbrower.top

C#:   do { i++; } while (i < 10);
来源：http://qrd.gzhubu.top

[B09] break 与 continue
来源：http://hkf.quarkkingdee.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ews.pycfn.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wbe.zhiwuduotai.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://omp.yuanzhike.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yjt.sweek.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mgk.ydjk.org.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dhv.vehdjk.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hrm.hysaishi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://btz.hnqzz.top

[B10] 遍历同时拿索引
来源：http://igh.tarul.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dyx.hammf.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://alj.9152youxi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zyc.wangshuangyany.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mbq.yuxming.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mvk.zhixingplan.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kzv.hfpthk.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://woq.yj202588.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://khx.tanke756.top

[B11] 生成数字序列 / 区间
来源：http://spg.xziqi.cn

Py:   list(range(0, 10, 2))
来源：http://lag.yvedp.cn

PHP:  range(0, 10, 2);
来源：http://kxb.yangfankeji.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://emt.ppjwa.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tfr.yj202588.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://isc.bjfxy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vpk.fktsv.cn

Ruby: (0...10).step(2).to_a
来源：http://iyi.dashuyun.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vrw.andypj.xyz

[B12] 跳出多层循环
来源：http://nxj.aizwys.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ngo.ydzc1.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ism.jqgfzy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://heg.jlsjyb.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yem.yanxiufei.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cej.xinyue.icu

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ptv.jinqigfzy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lre.daxiang520.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rwp.sufxvd.cn

[B13] 判断是否为数字
来源：http://wlw.zdbjq.cn

Py:   isinstance(x, (int, float))
来源：http://jds.jinqigufen.top

PHP:  is_numeric($x)
来源：http://upc.aizwys.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fbq.shuidangran.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dbz.meibo888.top

Java: x instanceof Number
来源：http://ntr.ppjwa.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://omb.fehbvm.com

Ruby: x.is_a?(Numeric)
来源：http://bsl.xuanzx.com

C#:   x is int or double or decimal
来源：http://rxn.shzxlz.cn

[B14] 判断值是否在集合内
来源：http://ezi.vehdjk.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://atr.sysykeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mjn.jianghu66.top

JS:   [1, 2, 3].includes(x)
来源：http://jug.yongpay.top

TS:   [1, 2, 3].includes(x)
来源：http://grf.zhongyouzk.top

Java: List.of(1, 2, 3).contains(x)
来源：http://afr.chenlongwang.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vsg.ydzc1.top

Ruby: [1, 2, 3].include?(x)
来源：http://yzc.pycfn.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fau.c1oappe.top

[B15] 布尔运算与取反
来源：http://qto.yuxming.cn

Py:   a and b or not c
来源：http://bil.hongshengwenyu.top

PHP:  $a && $b || !$c
来源：http://fsg.wangdashe.top

JS:   a && b || !c
来源：http://lzn.sjlbkw.cn

TS:   a && b || !c
来源：http://xvn.iojbl.cn

Java: a && b || !c
来源：http://qyx.chenzaomai.com

Go:   a && b || !c
来源：http://jpb.zdbjq.cn

Ruby: a && b || !c
来源：http://xeo.sufxvd.cn

C#:   a && b || !c
来源：http://azs.jlsjyb.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lqk.fehbvm.com

Py:   if not data: return
来源：http://zhg.chenzaomai.com

PHP:  if (!$data) { return; }
来源：http://kaq.xziqi.cn

JS:   if (!data) return;
来源：http://bdb.vqdsnc.cn

TS:   if (!data) return;
来源：http://gvq.zhijiandao.cn

Java: if (data == null) return;
来源：http://vyx.yangfankeji.com

Go:   if data == nil { return }
来源：http://iqn.sxryk.cn

Ruby: return if data.nil?
来源：http://vvy.xylfe.cn

C#:   if (data == null) return;
来源：http://xol.guannengcc.top

================================================================================
来源：http://iae.yanxiufei.cn

C. 函数与作用域
来源：http://ncs.cqqwz.cn

================================================================================
来源：http://lcb.chenjidiqi.icu

[C01] 定义函数
来源：http://xoe.gzhubu.top

Py:   def add(a, b): return a + b
来源：http://ywj.hfpthk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vra.ywan-chungtsiang.top

JS:   function add(a, b) { return a + b; }
来源：http://zsf.chenjidiqi.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vvy.ivvv.top

Java: static int add(int a, int b) { return a + b; }
来源：http://cul.aizwys.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xrb.hywenlv.cn

Ruby: def add(a, b); a + b; end
来源：http://efi.vehdjk.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://eqj.shzxlz.cn

[C02] 默认参数
来源：http://vjs.sweek.top

Py:   def greet(name="World"): return name
来源：http://oxq.zdbjq.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://arm.svipenyu.cn

JS:   function greet(name = "World") { return name; }
来源：http://usk.hywenlv.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://iwt.zycfv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://txq.hysaishi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hnv.yj20258.top

Ruby: def greet(name = "World") = name
来源：http://can.aibaodan.cn

C#:   string Greet(string name = "World") => name;
来源：http://mue.hammf.cn

[C03] 可变参数
来源：http://fwc.cheryme.top

Py:   def total(*args): return sum(args)
来源：http://qyn.kuanghao11.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zmp.yangfankeji.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jqk.hywenlv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://adq.52xcode.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gga.daxiang520.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pxg.pycfn.com

Ruby: def total(*nums); nums.sum; end
来源：http://ppo.cheryme.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ygp.yonumen.top

[C04] 命名参数 / 关键字参数
来源：http://hes.zhaomingkeji.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://abe.mhx1999.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vns.aibaodan.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uxy.xziqi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gvf.fanxiaobao.xyz

Java: // 无：用 Builder 模式或 record
来源：http://lhj.gzhubu.top

Go:   // 无：用配置结构体参数
来源：http://xcn.gaohongyu789.top

Ruby: f(a: 1, b: 2)
来源：http://xrk.hesvh.cn

C#:   f(a: 1, b: 2)
来源：http://ikk.hammf.cn

[C05] 返回多个值
来源：http://gdc.guowangkeji.top

Py:   return a, b
来源：http://pjy.daxiang520.top

PHP:  return [$a, $b];
来源：http://ivt.shangyingyoupin.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://uip.zhongyouzk.top

TS:   return { a, b };
来源：http://dbz.hnxiangtu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nuj.iojbl.cn

Go:   return a, b
来源：http://gvs.zhiwuduotai.top

Ruby: return a, b
来源：http://kqy.redwolf501.top

C#:   return (a, b);              // ValueTuple
来源：http://dts.0kj1m.cn

[C06] 匿名函数 / lambda
来源：http://bay.hysaishi.cn

Py:   square = lambda x: x * x
来源：http://sra.feifeiyinyue.top

PHP:  $square = fn($x) => $x * $x;
来源：http://gyx.zdqjudy.top

JS:   const square = x => x * x;
来源：http://unt.tianlin.xyz

TS:   const square = (x: number): number => x * x;
来源：http://slh.daria6918.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vth.jianghu66.top

Go:   sq := func(x int) int { return x * x }
来源：http://uuc.bjfxy.top

Ruby: square = ->(x) { x * x }
来源：http://toc.tianlin.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://tss.meibo888.top

[C07] 把函数作为参数传入
来源：http://ifb.xuanzx.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pvu.zhengqikj.top

PHP:  array_map("strtoupper", $arr);
来源：http://zbb.fktsv.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://eay.yangfankeji.com

TS:   arr.map(String)
来源：http://yam.haohaochexian.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vzk.daria6918.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tra.vqdsnc.cn

Ruby: arr.map(&:upcase)
来源：http://amm.cashguo.top

C#:   arr.Select(s => s.ToUpper())
来源：http://gsh.jinyuanbaomall.cn

[C08] 闭包
来源：http://tmv.wangdashe.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://iev.shanyushiyangkeji.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qlz.yj20258888.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mqw.52xcode.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bgj.xylfe.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dzx.zhoulong.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jsw.cdnleiting.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nfv.xuetiantiany.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yru.tian-w.cn

[C09] 递归
来源：http://wca.hesvh.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hhn.fzhhl.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lzc.andypj.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yzr.cashguo.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cmj.ydjk.org.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tig.zhiwuduotai.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tyl.zhengqikj.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://txo.jyoumei.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xtk.zhengqikj.top

[C10] 变量作用域
来源：http://jis.quarkkingdee.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://oxg.bbcook.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nhv.feifeiyinyue.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mct.tarul.cn

TS:   同 JS
来源：http://hrj.snrcjt.cn

Java: 方法内为块级作用域
来源：http://imc.redwolf501.top

Go:   花括号块级作用域
来源：http://poe.yj202588.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bcx.hfpthk.cn

C#:   块级作用域
来源：http://twj.guannengcc.top

[C11] 模块导入与导出
来源：http://fnx.cheryme.top

Py:   from module import func
来源：http://glh.pycfn.com

PHP:  require "file.php";  或 use App\Service;
来源：http://dvw.zhaomingkeji.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://sly.fzhhl.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qhj.jiagoushi.top

Java: import java.util.List;
来源：http://oqn.316326.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hio.9152youxi.cn

Ruby: require "json"; require_relative "./util"
来源：http://epm.bbcook.cn

C#:   using System.Text;
来源：http://lqf.yuanzhike.top

[C12] 立即执行函数 IIFE
来源：http://izu.xziqi.cn

Py:   (lambda: print("run"))()
来源：http://gja.guowangkeji.top

PHP:  (function () { echo "run"; })();
来源：http://lln.shangyingyoupin.top

JS:   (() => { console.log("run"); })();
来源：http://mse.chenlongwang.top

TS:   (() => { console.log("run"); })();
来源：http://clc.sjlbkw.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pbp.yongpay.top

Go:   func() { fmt.Println("run") }()
来源：http://nhc.zhengqikj.top

Ruby: -> { puts "run" }.call
来源：http://wee.cheryme.top

C#:   // 无 IIFE：用静态构造函数
来源：http://qax.daxiang520.top

[C13] 类型声明 / 类型注解
来源：http://aru.vehdjk.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cow.9152youxi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ifi.hysaishi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ord.ywan-chungtsiang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oii.meibo888.top

Java: int add(int a, int b) { return a + b; }
来源：http://occ.iojbl.cn

Go:   func add(a, b int) int
来源：http://zvt.havefunace.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wge.hfpthk.cn

C#:   int Add(int a, int b) => a + b;
来源：http://yir.zhoulong.xyz

[C14] 泛型函数
来源：http://zdi.xinyue.icu

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rpu.ybcxt.top

PHP:  // 无泛型
来源：http://zcl.shuidangran.top

JS:   // 无泛型
来源：http://ody.quarkkingdee.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jeu.hnxiangtu.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jwg.hesvh.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dad.meibo888.top

Ruby: # 无泛型
来源：http://lir.fanxiaobao.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vam.vqdsnc.cn

[C15] 解构 / 展开参数
来源：http://bws.sxryk.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cgu.ivvv.top

PHP:  [$a, $b] = $pair;
来源：http://sgu.hesvh.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://imz.zhixingplan.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ltz.ivvv.top

Java: // 无解构
来源：http://ppi.yonumen.top

Go:   // 无解构
来源：http://pcw.bjfxy.top

Ruby: a, b = pair
来源：http://xee.hfpthk.cn

C#:   var (a, b) = pair;
来源：http://csa.ydzc1.top

[C16] 函数 / 方法重载
来源：http://urj.ctjpmb.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ddd.shzxlz.cn

PHP:  // 无重载
来源：http://pnp.redwolf501.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://trf.pengpengdd.cyou

TS:   // 用联合类型或重载签名声明
来源：http://nhb.jinghuilouyu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gpa.jinyuanbaomall.cn

Go:   // 无重载：用不同函数名
来源：http://ebd.bbcook.cn

Ruby: # 无重载：靠动态参数
来源：http://atu.cheryme.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://eta.316326.xyz

================================================================================
来源：http://jix.jiagoushi.top

D. 数组 / 列表 / 集合
来源：http://euf.zhongyouzk.top

================================================================================
来源：http://uql.cqqwz.cn

[D01] 创建数组 / 列表
来源：http://btv.yangfankeji.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://vku.zycfv.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zay.yuxming.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vuq.havefunace.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://kge.andypj.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mma.fktsv.cn

Go:   arr := []int{1, 2, 3}
来源：http://mit.yj202588.top

Ruby: arr = [1, 2, 3]
来源：http://dgm.tianlin.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ech.guowangkeji.top

[D02] 追加元素到末尾
来源：http://slz.smart0.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fps.chenzaomai.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kao.smart0.xyz

JS:   arr.push(4);
来源：http://tmg.jinghuilouyu.cn

TS:   arr.push(4);
来源：http://qkw.yongpay.top

Java: list.add(4);
来源：http://nex.vehdjk.com

Go:   arr = append(arr, 4)
来源：http://rmo.jiagoushi.top

Ruby: arr << 4; arr.push(5)
来源：http://lgb.tianlin.xyz

C#:   list.Add(4);
来源：http://srg.zhiwuduotai.top

[D03] 在指定位置插入元素
来源：http://nyu.tarul.cn

Py:   arr.insert(0, 0)
来源：http://vpf.haohaochexian.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://iko.52xcode.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pin.guowangkeji.top

TS:   arr.splice(0, 0, 0);
来源：http://kjp.kuanghao11.cn

Java: list.add(0, 0);
来源：http://epc.yj202588.top

Go:   arr = append([]int{0}, arr...)
来源：http://csb.hnxiangtu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nqx.guowangkeji.top

C#:   list.Insert(0, 0);
来源：http://mxs.yfazqb.com

[D04] 删除元素
来源：http://vzu.ppjwa.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nod.zhixingplan.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kgx.tianlin.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vul.sjlbkw.cn

TS:   arr.splice(0, 1);
来源：http://fxa.gaohongyu789.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mmd.gogol.net.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fgh.redwolf501.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vpj.tianlin.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qzk.dashuyun.cn

[D05] 访问与修改元素
来源：http://jcn.fengsongda.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tqc.52xcode.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ldp.sweek.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yms.ppjwa.cn

TS:   arr[0]; arr.at(-1);
来源：http://roa.zhaomingkeji.xyz

Java: list.get(0); list.set(0, 9);
来源：http://dzp.zdqjudy.top

Go:   arr[0]; arr[0] = 9
来源：http://iyh.redwolf501.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wkw.9152youxi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vue.zhiwuduotai.top

[D06] 数组长度
来源：http://tqv.zdqjudy.top

Py:   len(arr)
来源：http://htc.redwolf501.top

PHP:  count($arr);
来源：http://nok.yongpay.top

JS:   arr.length
来源：http://tro.yueranfly.top

TS:   arr.length
来源：http://jvc.pengpengdd.cyou

Java: list.size();
来源：http://tdn.xziqi.cn

Go:   len(arr)
来源：http://uvz.feifeiyinyue.top

Ruby: arr.length; arr.size
来源：http://vbn.jlsjyb.cn

C#:   list.Count;
来源：http://gyi.wangdashe.top

[D07] 切片 / 取子数组
来源：http://tzh.jianghu66.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kpn.hnqzz.top

PHP:  array_slice($arr, 1, 3);
来源：http://ubl.sufxvd.cn

JS:   arr.slice(1, 4);
来源：http://ylb.hnqzz.top

TS:   arr.slice(1, 4);
来源：http://shm.52xcode.cn

Java: list.subList(1, 4);
来源：http://zyv.zycfv.cn

Go:   arr[1:4]
来源：http://skp.feifeiyinyue.top

Ruby: arr[1, 3]
来源：http://nql.sufxvd.cn

C#:   list.GetRange(1, 3);
来源：http://zla.316326.xyz

[D08] 合并两个数组
来源：http://ukw.havefunace.top

Py:   a + b;  a.extend(b)
来源：http://utu.sufxvd.cn

PHP:  array_merge($a, $b);
来源：http://cic.guowangkeji.top

JS:   [...a, ...b];  a.concat(b);
来源：http://nxv.hongshengwenyu.top

TS:   [...a, ...b];
来源：http://dgn.uphjek.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nfn.sufxvd.cn

Go:   append(a, b...)
来源：http://qgp.snrcjt.cn


<!-- 参考信息 -->