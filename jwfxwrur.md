代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ftg.aizwys.cn

[B10] 遍历同时拿索引
来源：http://iux.mhx1999.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ldz.316326.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ciz.sweek.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lru.mhx1999.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://eok.wangshuangyany.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ppc.svipenyu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hhp.zhaomingkeji.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gte.sxryk.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://aee.fanxiaobao.xyz

[B11] 生成数字序列 / 区间
来源：http://thi.xuanzx.com

Py:   list(range(0, 10, 2))
来源：http://thj.guowangkeji.top

PHP:  range(0, 10, 2);
来源：http://ngf.nanxinkj.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yqg.xuanzx.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jje.fktsv.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hbf.sjlbkw.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bcy.52xcode.cn

Ruby: (0...10).step(2).to_a
来源：http://lsg.zhiwuduotai.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uje.dashuyun.cn

[B12] 跳出多层循环
来源：http://ddq.tanke756.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://vrz.fengsongda.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://lqs.0kj1m.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kxu.zhengqikj.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fbb.jlsjyb.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nek.smart0.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yoa.zdbjq.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gsl.shangyingyoupin.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ydt.ehwqpu.com

[B13] 判断是否为数字
来源：http://bqk.guowangkeji.top

Py:   isinstance(x, (int, float))
来源：http://wsa.jinqigfzy.top

PHP:  is_numeric($x)
来源：http://jbd.yfazqb.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bfr.jqgfzy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ylw.redwolf501.top

Java: x instanceof Number
来源：http://qly.andypj.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ugz.jqgfzy.top

Ruby: x.is_a?(Numeric)
来源：http://oqs.pycfn.com

C#:   x is int or double or decimal
来源：http://rvd.fktsv.cn

[B14] 判断值是否在集合内
来源：http://ion.gaohongyu789.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://soo.fanxiaobao.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jdg.sweek.top

JS:   [1, 2, 3].includes(x)
来源：http://wvv.shuidangran.top

TS:   [1, 2, 3].includes(x)
来源：http://dnw.fzhhl.top

Java: List.of(1, 2, 3).contains(x)
来源：http://foy.nanxuanxn.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hpk.316326.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://qzl.kuanghao11.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xnj.dianchejie.cn

[B15] 布尔运算与取反
来源：http://xud.yvedp.cn

Py:   a and b or not c
来源：http://xga.fengsongda.top

PHP:  $a && $b || !$c
来源：http://ddl.quarkkingdee.top

JS:   a && b || !c
来源：http://ewy.shzxlz.cn

TS:   a && b || !c
来源：http://rtm.c1oappe.top

Java: a && b || !c
来源：http://sdo.mhx1999.top

Go:   a && b || !c
来源：http://typ.xingfuxueyuan.xyz

Ruby: a && b || !c
来源：http://hur.jiagoushi.top

C#:   a && b || !c
来源：http://jfl.ehwqpu.com

[B16] 卫语句：不满足条件提前返回
来源：http://qnc.pycfn.com

Py:   if not data: return
来源：http://fuk.uphjek.com

PHP:  if (!$data) { return; }
来源：http://qow.xingfuxueyuan.xyz

JS:   if (!data) return;
来源：http://wuq.zycfv.cn

TS:   if (!data) return;
来源：http://fiw.jiagoushi.top

Java: if (data == null) return;
来源：http://dhl.ivvv.top

Go:   if data == nil { return }
来源：http://tkx.tianlin.xyz

Ruby: return if data.nil?
来源：http://opf.9152youxi.cn

C#:   if (data == null) return;
来源：http://umq.guannengcc.top

================================================================================
来源：http://xui.ppjwa.cn

C. 函数与作用域
来源：http://rvh.snrcjt.cn

================================================================================
来源：http://fdz.zhixingplan.top

[C01] 定义函数
来源：http://plb.pengpengdd.cyou

Py:   def add(a, b): return a + b
来源：http://bji.xylfe.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xfq.xylfe.cn

JS:   function add(a, b) { return a + b; }
来源：http://ysu.yongpay.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pdm.nanxuanxn.top

Java: static int add(int a, int b) { return a + b; }
来源：http://myg.cdnleiting.top

Go:   func add(a, b int) int { return a + b }
来源：http://ugn.hysaishi.cn

Ruby: def add(a, b); a + b; end
来源：http://dwc.sxryk.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pzv.smart0.xyz

[C02] 默认参数
来源：http://fue.nanxuanxn.top

Py:   def greet(name="World"): return name
来源：http://qaw.zhoulong.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://ofa.pycfn.com

JS:   function greet(name = "World") { return name; }
来源：http://nag.yongpay.top

TS:   function greet(name: string = "World") { return name; }
来源：http://tjk.haohaochexian.top

Java: // 无默认参数：方法重载或 Optional
来源：http://eaz.hammf.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nky.pengpengdd.cyou

Ruby: def greet(name = "World") = name
来源：http://hpt.zdbjq.cn

C#:   string Greet(string name = "World") => name;
来源：http://obi.havefunace.top

[C03] 可变参数
来源：http://gwz.ehwqpu.com

Py:   def total(*args): return sum(args)
来源：http://tpk.316326.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pmo.jinqigfzy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ivw.hfpthk.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dwf.guannengcc.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://flx.nanxuanxn.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dkv.daria6918.cn

Ruby: def total(*nums); nums.sum; end
来源：http://isu.zhoulong.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ihv.hesvh.cn

[C04] 命名参数 / 关键字参数
来源：http://bgn.daria6918.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kbl.chenlongwang.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zbg.c1oappe.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xcx.jiagoushi.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cwy.chenjidiqi.icu

Java: // 无：用 Builder 模式或 record
来源：http://tyz.yj20258.top

Go:   // 无：用配置结构体参数
来源：http://srs.wangshuangyany.cn

Ruby: f(a: 1, b: 2)
来源：http://uzf.snrcjt.cn

C#:   f(a: 1, b: 2)
来源：http://nbt.jinqigufen.top

[C05] 返回多个值
来源：http://tvu.redwolf501.top

Py:   return a, b
来源：http://zbv.shuidangran.top

PHP:  return [$a, $b];
来源：http://spk.chenzaomai.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://nce.yueranfly.top

TS:   return { a, b };
来源：http://pwy.bjfxy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ubm.tian-w.cn

Go:   return a, b
来源：http://dlo.birdmap.top

Ruby: return a, b
来源：http://lws.yongpay.top

C#:   return (a, b);              // ValueTuple
来源：http://pls.dashuyun.cn

[C06] 匿名函数 / lambda
来源：http://vbn.xingfuxueyuan.xyz

Py:   square = lambda x: x * x
来源：http://uqs.zhongyouzk.top

PHP:  $square = fn($x) => $x * $x;
来源：http://phm.uphjek.com

JS:   const square = x => x * x;
来源：http://jlx.hammf.cn

TS:   const square = (x: number): number => x * x;
来源：http://nvx.daxiang520.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://smc.gzhubu.top

Go:   sq := func(x int) int { return x * x }
来源：http://vsi.chenjidiqi.icu

Ruby: square = ->(x) { x * x }
来源：http://diz.wangdashe.top

C#:   Func<int, int> square = x => x * x;
来源：http://cbs.hongshengwenyu.top

[C07] 把函数作为参数传入
来源：http://dgj.yj20258.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://uif.daxiang520.top

PHP:  array_map("strtoupper", $arr);
来源：http://orq.dianchejie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cri.wangdashe.top

TS:   arr.map(String)
来源：http://ipg.jlsjyb.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://inm.dianchejie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://onh.ybcxt.top

Ruby: arr.map(&:upcase)
来源：http://hfb.jiagoushi.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ifj.zhiwuduotai.top

[C08] 闭包
来源：http://slo.ehwqpu.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yms.hywenlv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://oar.ydzc1.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://iie.hnxiangtu.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fzc.feifeiyinyue.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cdh.jinyuanbaomall.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gps.vqdsnc.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gyo.bjfxy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vgn.jinghuilouyu.cn

[C09] 递归
来源：http://jav.hywenlv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uft.xziqi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ihu.tian-w.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pmh.tianlin.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sfw.zdqjudy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hki.xziqi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dze.jinghuilouyu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yxw.uphjek.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tjo.yvedp.cn

[C10] 变量作用域
来源：http://vwx.ywan-chungtsiang.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jmz.yvedp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ukr.sjlbkw.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vvg.yongpay.top

TS:   同 JS
来源：http://wgl.xingfuxueyuan.xyz

Java: 方法内为块级作用域
来源：http://czs.feifeiyinyue.top

Go:   花括号块级作用域
来源：http://xsm.aibaodan.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tcc.svipenyu.cn

C#:   块级作用域
来源：http://jsl.ctjpmb.com

[C11] 模块导入与导出
来源：http://psv.nwbrower.top

Py:   from module import func
来源：http://tkm.zhengqikj.top

PHP:  require "file.php";  或 use App\Service;
来源：http://qks.xinyue.icu

JS:   export default function f() {};  import f from "./m.js";
来源：http://lhb.aibaodan.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tvt.fengsongda.top

Java: import java.util.List;
来源：http://bvb.shzxlz.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xtb.hesvh.cn

Ruby: require "json"; require_relative "./util"
来源：http://vqm.yj20258.top

C#:   using System.Text;
来源：http://vhz.sysykeji.top

[C12] 立即执行函数 IIFE
来源：http://zkm.chenlongwang.top

Py:   (lambda: print("run"))()
来源：http://rxr.xuetiantiany.cn

PHP:  (function () { echo "run"; })();
来源：http://syu.redwolf501.top

JS:   (() => { console.log("run"); })();
来源：http://duw.ydzc1.top

TS:   (() => { console.log("run"); })();
来源：http://qzb.daria6918.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lja.zycfv.cn

Go:   func() { fmt.Println("run") }()
来源：http://pap.316326.xyz

Ruby: -> { puts "run" }.call
来源：http://chh.zhongyouzk.top

C#:   // 无 IIFE：用静态构造函数
来源：http://wpx.52xcode.cn

[C13] 类型声明 / 类型注解
来源：http://fxz.pycfn.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sjr.ydzc1.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xvu.hfpthk.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pza.hcnkem.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zkr.cheryme.top

Java: int add(int a, int b) { return a + b; }
来源：http://yzj.jinghuilouyu.cn

Go:   func add(a, b int) int
来源：http://dgc.xingfuxueyuan.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jvt.hesvh.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mni.c1oappe.top

[C14] 泛型函数
来源：http://enm.zdqjudy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xlu.zhijiandao.cn

PHP:  // 无泛型
来源：http://mvi.jiagoushi.top

JS:   // 无泛型
来源：http://hds.dashuyun.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tfq.wangshuangyany.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vva.yueranfly.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://erf.tanke756.top

Ruby: # 无泛型
来源：http://puy.xziqi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kqd.yvedp.cn

[C15] 解构 / 展开参数
来源：http://mur.dashuyun.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://byd.shuidangran.top

PHP:  [$a, $b] = $pair;
来源：http://uqt.meibo888.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://epl.zhengqikj.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pbg.yvedp.cn

Java: // 无解构
来源：http://lqm.yongpay.top

Go:   // 无解构
来源：http://oni.gaohongyu789.top

Ruby: a, b = pair
来源：http://dgq.shuidangran.top

C#:   var (a, b) = pair;
来源：http://fzb.haohaochexian.top

[C16] 函数 / 方法重载
来源：http://tal.cheryme.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vuv.shuidangran.top

PHP:  // 无重载
来源：http://nmr.dianchejie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://tie.ydzc1.top

TS:   // 用联合类型或重载签名声明
来源：http://nko.pengpengdd.cyou

Java: void f(int a) {}  void f(String a) {}
来源：http://dbl.vehdjk.com

Go:   // 无重载：用不同函数名
来源：http://spj.gzhubu.top

Ruby: # 无重载：靠动态参数
来源：http://vxc.shanyushiyangkeji.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://xpc.cqqwz.cn

================================================================================
来源：http://dzg.ydzc1.top

D. 数组 / 列表 / 集合
来源：http://pjn.cashguo.top

================================================================================
来源：http://hif.birdmap.top

[D01] 创建数组 / 列表
来源：http://qjq.xuanzx.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://ylu.jinghuilouyu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://eua.ivvv.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wpg.sjlbkw.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qkk.nanxuanxn.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lmw.cucudq.cn

Go:   arr := []int{1, 2, 3}
来源：http://sjn.yfazqb.com

Ruby: arr = [1, 2, 3]
来源：http://tmp.mhx1999.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://eac.nwbrower.top

[D02] 追加元素到末尾
来源：http://oaj.sysykeji.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ksj.birdmap.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ars.cashguo.top

JS:   arr.push(4);
来源：http://got.hnqzz.top

TS:   arr.push(4);
来源：http://ili.cheryme.top

Java: list.add(4);
来源：http://nzc.sjlbkw.cn

Go:   arr = append(arr, 4)
来源：http://kui.zhongyouzk.top

Ruby: arr << 4; arr.push(5)
来源：http://hqt.cheryme.top

C#:   list.Add(4);
来源：http://ixv.daxiang520.top

[D03] 在指定位置插入元素
来源：http://jlc.316326.xyz

Py:   arr.insert(0, 0)
来源：http://ncd.guowangkeji.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jzs.bjfxy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qss.c1oappe.top

TS:   arr.splice(0, 0, 0);
来源：http://fqb.bjfxy.top

Java: list.add(0, 0);
来源：http://jvv.shanyushiyangkeji.top

Go:   arr = append([]int{0}, arr...)
来源：http://tyk.bjfxy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gif.hywenlv.cn

C#:   list.Insert(0, 0);
来源：http://qhx.xziqi.cn

[D04] 删除元素
来源：http://bzm.chenjidiqi.icu

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wwb.shuidangran.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://evj.ivvv.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fgg.nanxuanxn.top

TS:   arr.splice(0, 1);
来源：http://epw.redwolf501.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lzh.yj20258.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rqc.xinyue.icu

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mhs.pycfn.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jcz.jianghu66.top

[D05] 访问与修改元素
来源：http://eqe.gzhubu.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pdo.cheryme.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cxh.yanxiufei.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nvt.zhijiandao.cn

TS:   arr[0]; arr.at(-1);
来源：http://vwl.ppjwa.cn

Java: list.get(0); list.set(0, 9);
来源：http://jyj.yuxming.cn

Go:   arr[0]; arr[0] = 9
来源：http://zbn.xuetiantiany.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vye.ydjk.org.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nqq.bjfxy.top

[D06] 数组长度
来源：http://vdz.shanyushiyangkeji.top

Py:   len(arr)
来源：http://isz.snrcjt.cn

PHP:  count($arr);
来源：http://gpo.yj202588.top

JS:   arr.length
来源：http://mml.fzhhl.top

TS:   arr.length
来源：http://tbr.shanyushiyangtech.top

Java: list.size();
来源：http://ynn.zhengqikj.top

Go:   len(arr)
来源：http://wgk.pycfn.com

Ruby: arr.length; arr.size
来源：http://tyn.yanxiufei.cn

C#:   list.Count;
来源：http://tcj.zdqjudy.top

[D07] 切片 / 取子数组
来源：http://nyn.yuxming.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://elc.vqdsnc.cn

PHP:  array_slice($arr, 1, 3);
来源：http://slo.xuetiantiany.cn

JS:   arr.slice(1, 4);
来源：http://dtc.chenjidiqi.icu

TS:   arr.slice(1, 4);
来源：http://ehg.xylfe.cn

Java: list.subList(1, 4);
来源：http://bwe.fengsongda.top

Go:   arr[1:4]
来源：http://rmr.nwbrower.top

Ruby: arr[1, 3]
来源：http://awv.uphjek.com

C#:   list.GetRange(1, 3);
来源：http://chj.shzxlz.cn

[D08] 合并两个数组
来源：http://wbg.cdnleiting.top

Py:   a + b;  a.extend(b)
来源：http://pyi.jqgfzy.top

PHP:  array_merge($a, $b);
来源：http://jhi.nwbrower.top

JS:   [...a, ...b];  a.concat(b);
来源：http://jty.cucudq.cn

TS:   [...a, ...b];
来源：http://xto.smart0.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dhg.zhongyouzk.top

Go:   append(a, b...)
来源：http://uwp.yvedp.cn

Ruby: a + b;  a.concat(b)
来源：http://uok.zhixingplan.top

C#:   a.Concat(b).ToList()
来源：http://kpq.shuidangran.top

[D09] 排序（升序）
来源：http://kdz.zdbjq.cn

Py:   sorted(arr);  arr.sort()
来源：http://jus.fengsongda.top

PHP:  sort($arr);
来源：http://gid.cucudq.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hlj.daxiang520.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://yre.gaohongyu789.top

Java: Collections.sort(list);  list.sort(null);
来源：http://iob.hongshengwenyu.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zyi.zhaomingkeji.xyz

Ruby: arr.sort
来源：http://jgv.yuxming.cn

C#:   list.Sort();
来源：http://zvm.nanxinkj.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://aqh.mhx1999.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lse.gogol.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gej.cucudq.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rog.shzxlz.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://edo.ydjk.org.cn


<!-- 参考信息 -->