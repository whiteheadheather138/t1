代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tkg.jinqigufen.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://thi.yj20258888.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hdy.havefunace.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dnz.0kj1m.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pgu.chenlongwang.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://iaz.c1oappe.top

[B11] 生成数字序列 / 区间
来源：http://ejb.tianlin.xyz

Py:   list(range(0, 10, 2))
来源：http://ewp.tanke756.top

PHP:  range(0, 10, 2);
来源：http://iwb.zhongyouzk.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nfp.yongpay.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://awy.meibo888.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://njg.zhoulong.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gwn.tanke756.top

Ruby: (0...10).step(2).to_a
来源：http://inm.fanxiaobao.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://heo.hnqzz.top

[B12] 跳出多层循环
来源：http://gsg.daria6918.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fgz.nwbrower.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://dyv.yj20258.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://oha.sysykeji.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://njk.hysaishi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://asw.hesvh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://exx.jqgufenzy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jmb.guannengcc.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://azw.ydzc1.top

[B13] 判断是否为数字
来源：http://xng.tarul.cn

Py:   isinstance(x, (int, float))
来源：http://arl.snrcjt.cn

PHP:  is_numeric($x)
来源：http://nei.xuetiantiany.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lzj.hnqzz.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iga.sxryk.cn

Java: x instanceof Number
来源：http://bih.hysaishi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hxm.zdbjq.cn

Ruby: x.is_a?(Numeric)
来源：http://ias.cucudq.cn

C#:   x is int or double or decimal
来源：http://vrs.sufxvd.cn

[B14] 判断值是否在集合内
来源：http://foc.fengsongda.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qpx.yueranfly.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fos.pycfn.com

JS:   [1, 2, 3].includes(x)
来源：http://mzs.aizwys.cn

TS:   [1, 2, 3].includes(x)
来源：http://jrp.chenlongwang.top

Java: List.of(1, 2, 3).contains(x)
来源：http://yzx.aibaodan.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://iya.fzhhl.top

Ruby: [1, 2, 3].include?(x)
来源：http://bea.chenlongwang.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jnk.yj202588.top

[B15] 布尔运算与取反
来源：http://ptf.gaohongyu789.top

Py:   a and b or not c
来源：http://mrm.nanxinkj.top

PHP:  $a && $b || !$c
来源：http://ozb.chenlongwang.top

JS:   a && b || !c
来源：http://tmv.zdqjudy.top

TS:   a && b || !c
来源：http://tpv.yonumen.top

Java: a && b || !c
来源：http://rhl.sufxvd.cn

Go:   a && b || !c
来源：http://amm.chenlongwang.top

Ruby: a && b || !c
来源：http://jrj.jinyuanbaomall.cn

C#:   a && b || !c
来源：http://gkp.cashguo.top

[B16] 卫语句：不满足条件提前返回
来源：http://tmb.yangfankeji.com

Py:   if not data: return
来源：http://afr.yanxiufei.cn

PHP:  if (!$data) { return; }
来源：http://bwp.mhx1999.top

JS:   if (!data) return;
来源：http://unr.jianghu66.top

TS:   if (!data) return;
来源：http://ezb.guannengcc.top

Java: if (data == null) return;
来源：http://xsi.zhixingplan.top

Go:   if data == nil { return }
来源：http://noi.haohaochexian.top

Ruby: return if data.nil?
来源：http://etm.jqgfzy.top

C#:   if (data == null) return;
来源：http://olz.zhixingplan.top

================================================================================
来源：http://uau.zhijiandao.cn

C. 函数与作用域
来源：http://rvx.52xcode.cn

================================================================================
来源：http://efh.hongshengwenyu.top

[C01] 定义函数
来源：http://oov.meibo888.top

Py:   def add(a, b): return a + b
来源：http://rdc.cqqwz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nil.316326.xyz

JS:   function add(a, b) { return a + b; }
来源：http://klo.yuanzhike.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zgk.haohaochexian.top

Java: static int add(int a, int b) { return a + b; }
来源：http://xze.yuanzhike.top

Go:   func add(a, b int) int { return a + b }
来源：http://lhb.hesvh.cn

Ruby: def add(a, b); a + b; end
来源：http://dxn.zhengqikj.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://thg.yongpay.top

[C02] 默认参数
来源：http://wda.shzxlz.cn

Py:   def greet(name="World"): return name
来源：http://nve.aizwys.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://atv.hongshengwenyu.top

JS:   function greet(name = "World") { return name; }
来源：http://yjf.havefunace.top

TS:   function greet(name: string = "World") { return name; }
来源：http://nsm.jqgfzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ifg.nanxuanxn.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rbu.hcnkem.com

Ruby: def greet(name = "World") = name
来源：http://uzg.shanyushiyangkeji.top

C#:   string Greet(string name = "World") => name;
来源：http://fql.smart0.xyz

[C03] 可变参数
来源：http://reo.redwolf501.top

Py:   def total(*args): return sum(args)
来源：http://rez.hfpthk.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blq.svipenyu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sne.jyoumei.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pgl.chenlongwang.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hyc.cheryme.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zyv.redwolf501.top

Ruby: def total(*nums); nums.sum; end
来源：http://cwj.shangyingyoupin.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sbo.zycfv.cn

[C04] 命名参数 / 关键字参数
来源：http://pdp.chenlongwang.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ojd.316326.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gdg.shzxlz.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wtb.yangfankeji.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xuz.cqqwz.cn

Java: // 无：用 Builder 模式或 record
来源：http://fzi.jinyuanbaomall.cn

Go:   // 无：用配置结构体参数
来源：http://iqr.c1oappe.top

Ruby: f(a: 1, b: 2)
来源：http://ghz.fehbvm.com

C#:   f(a: 1, b: 2)
来源：http://vtp.guowangkeji.top

[C05] 返回多个值
来源：http://aqf.tianlin.xyz

Py:   return a, b
来源：http://cus.jinqigufen.top

PHP:  return [$a, $b];
来源：http://mvw.shuidangran.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://jlw.zhiwuduotai.top

TS:   return { a, b };
来源：http://rwv.shangyingyoupin.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xbu.zhoulong.xyz

Go:   return a, b
来源：http://qwc.jinyuanbaomall.cn

Ruby: return a, b
来源：http://vvt.zycfv.cn

C#:   return (a, b);              // ValueTuple
来源：http://obv.zhiwuduotai.top

[C06] 匿名函数 / lambda
来源：http://xko.gzhubu.top

Py:   square = lambda x: x * x
来源：http://sum.fktsv.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://acy.andypj.xyz

JS:   const square = x => x * x;
来源：http://cqv.quarkkingdee.top

TS:   const square = (x: number): number => x * x;
来源：http://ywl.sjlbkw.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pdi.vehdjk.com

Go:   sq := func(x int) int { return x * x }
来源：http://kgq.sysykeji.top

Ruby: square = ->(x) { x * x }
来源：http://rje.pengpengdd.cyou

C#:   Func<int, int> square = x => x * x;
来源：http://ssu.hnxiangtu.top

[C07] 把函数作为参数传入
来源：http://mxh.chenjidiqi.icu

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qkd.gogol.net.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xuo.hammf.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hxj.feifeiyinyue.top

TS:   arr.map(String)
来源：http://kmw.0kj1m.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lso.pengpengdd.cyou

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://usc.cdnleiting.top

Ruby: arr.map(&:upcase)
来源：http://xak.hcnkem.com

C#:   arr.Select(s => s.ToUpper())
来源：http://vhp.yueranfly.top

[C08] 闭包
来源：http://mse.ybcxt.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ajd.dianchejie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dxl.hongshengwenyu.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://paz.jinqigufen.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hrz.yj20258888.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xmz.yj202588.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jgw.cashguo.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wjh.tarul.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://itk.cheryme.top

[C09] 递归
来源：http://bcz.zhongyouzk.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://eqt.jqgfzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nsn.shangyingyoupin.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xuv.tarul.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vpl.chenzaomai.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://njy.feifeiyinyue.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dsj.yueranfly.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wel.jqgfzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uia.ybcxt.top

[C10] 变量作用域
来源：http://gss.gogol.net.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://loh.yanxiufei.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xhh.dianchejie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://maf.yfazqb.com

TS:   同 JS
来源：http://eka.zhijiandao.cn

Java: 方法内为块级作用域
来源：http://uip.yj20258.top

Go:   花括号块级作用域
来源：http://fgi.sysykeji.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://khq.jinqigufen.top

C#:   块级作用域
来源：http://tlv.tanke756.top

[C11] 模块导入与导出
来源：http://jqn.hywenlv.cn

Py:   from module import func
来源：http://cyp.daxiang520.top

PHP:  require "file.php";  或 use App\Service;
来源：http://sky.wangshuangyany.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pkr.gzhubu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gbb.uphjek.com

Java: import java.util.List;
来源：http://mdl.yanxiufei.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ggs.yj20258888.top

Ruby: require "json"; require_relative "./util"
来源：http://owh.aizwys.cn

C#:   using System.Text;
来源：http://spn.sxryk.cn

[C12] 立即执行函数 IIFE
来源：http://san.yanxiufei.cn

Py:   (lambda: print("run"))()
来源：http://jdi.shangyingyoupin.top

PHP:  (function () { echo "run"; })();
来源：http://euy.ctjpmb.com

JS:   (() => { console.log("run"); })();
来源：http://jry.vqdsnc.cn

TS:   (() => { console.log("run"); })();
来源：http://bhc.wangdashe.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bqr.52xcode.cn

Go:   func() { fmt.Println("run") }()
来源：http://acg.aizwys.cn

Ruby: -> { puts "run" }.call
来源：http://nxi.fanxiaobao.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://kqv.fengsongda.top

[C13] 类型声明 / 类型注解
来源：http://jmk.zhongyouzk.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://teq.jyoumei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xed.guannengcc.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xzy.mhx1999.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mjf.gotoacloud.top

Java: int add(int a, int b) { return a + b; }
来源：http://ijk.zdbjq.cn

Go:   func add(a, b int) int
来源：http://jlx.hammf.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ito.xziqi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://lig.chenjidiqi.icu

[C14] 泛型函数
来源：http://chj.sufxvd.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vnv.cashguo.top

PHP:  // 无泛型
来源：http://peu.zhixingplan.top

JS:   // 无泛型
来源：http://alc.fanxiaobao.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ank.nanxinkj.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hic.vqdsnc.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ihs.dianchejie.cn

Ruby: # 无泛型
来源：http://nzp.ybcxt.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qfc.chenjidiqi.icu

[C15] 解构 / 展开参数
来源：http://chv.feifeiyinyue.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://owr.havefunace.top

PHP:  [$a, $b] = $pair;
来源：http://fxv.quarkkingdee.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jlr.chenzaomai.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lez.jinqigufen.top

Java: // 无解构
来源：http://cvq.uphjek.com

Go:   // 无解构
来源：http://pjr.yongpay.top

Ruby: a, b = pair
来源：http://lfi.jianghu66.top

C#:   var (a, b) = pair;
来源：http://foz.snrcjt.cn

[C16] 函数 / 方法重载
来源：http://kvg.ydzc1.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wzi.zhongyouzk.top

PHP:  // 无重载
来源：http://aqt.hesvh.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://olv.quarkkingdee.top

TS:   // 用联合类型或重载签名声明
来源：http://nna.aibaodan.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://bin.jianghu66.top

Go:   // 无重载：用不同函数名
来源：http://ahm.uphjek.com

Ruby: # 无重载：靠动态参数
来源：http://xrm.tian-w.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://agx.epnwcf.com

================================================================================
来源：http://jyk.ybcxt.top

D. 数组 / 列表 / 集合
来源：http://ewb.fehbvm.com

================================================================================
来源：http://pjj.0kj1m.cn

[D01] 创建数组 / 列表
来源：http://sct.vqdsnc.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://kyt.jqgfzy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lou.hysaishi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://atz.chenzaomai.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://ejz.yangfankeji.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://oib.c1oappe.top

Go:   arr := []int{1, 2, 3}
来源：http://rkm.zdqjudy.top

Ruby: arr = [1, 2, 3]
来源：http://bnr.nanxinkj.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nlp.316326.xyz

[D02] 追加元素到末尾
来源：http://jus.316326.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jsr.nanxinkj.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wrf.hywenlv.cn

JS:   arr.push(4);
来源：http://ang.bbcook.cn

TS:   arr.push(4);
来源：http://nnw.chenlongwang.top

Java: list.add(4);
来源：http://mue.ywan-chungtsiang.top

Go:   arr = append(arr, 4)
来源：http://bez.chenjidiqi.icu

Ruby: arr << 4; arr.push(5)
来源：http://miw.cqqwz.cn

C#:   list.Add(4);
来源：http://aqx.c1oappe.top

[D03] 在指定位置插入元素
来源：http://rze.9152youxi.cn

Py:   arr.insert(0, 0)
来源：http://otr.hcnkem.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://srm.ybcxt.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ggr.ppjwa.cn

TS:   arr.splice(0, 0, 0);
来源：http://byo.jinqigfzy.top

Java: list.add(0, 0);
来源：http://esa.chenjidiqi.icu

Go:   arr = append([]int{0}, arr...)
来源：http://rjl.ybcxt.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://goe.ivvv.top

C#:   list.Insert(0, 0);
来源：http://qls.tanke756.top

[D04] 删除元素
来源：http://isy.zdqjudy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://row.0kj1m.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mks.zhaomingkeji.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xub.yanxiufei.cn

TS:   arr.splice(0, 1);
来源：http://ynt.iojbl.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tll.hywenlv.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vip.jinyuanbaomall.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mle.bjfxy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rof.nanxuanxn.top

[D05] 访问与修改元素
来源：http://vsi.vehdjk.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xpu.guannengcc.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wum.shzxlz.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qfh.daria6918.cn

TS:   arr[0]; arr.at(-1);
来源：http://hrc.guannengcc.top

Java: list.get(0); list.set(0, 9);
来源：http://nmx.shangyingyoupin.top

Go:   arr[0]; arr[0] = 9
来源：http://xeu.pengpengdd.cyou

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fig.zhijiandao.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wiu.shanyushiyangkeji.top

[D06] 数组长度
来源：http://vbt.zhongyouzk.top

Py:   len(arr)
来源：http://vqy.fanxiaobao.xyz

PHP:  count($arr);
来源：http://xlv.yj20258888.top

JS:   arr.length
来源：http://rnw.cucudq.cn

TS:   arr.length
来源：http://uyz.sjlbkw.cn

Java: list.size();
来源：http://kfv.hesvh.cn

Go:   len(arr)
来源：http://mms.jyoumei.cn

Ruby: arr.length; arr.size
来源：http://cug.gaohongyu789.top

C#:   list.Count;
来源：http://nag.cdnleiting.top

[D07] 切片 / 取子数组
来源：http://vgg.yonumen.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mkw.andypj.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://hzx.redwolf501.top

JS:   arr.slice(1, 4);
来源：http://zxt.wangdashe.top

TS:   arr.slice(1, 4);
来源：http://lci.shangyingyoupin.top

Java: list.subList(1, 4);
来源：http://jix.zdbjq.cn

Go:   arr[1:4]
来源：http://gar.cdnleiting.top

Ruby: arr[1, 3]
来源：http://tkk.hysaishi.cn

C#:   list.GetRange(1, 3);
来源：http://chh.fktsv.cn

[D08] 合并两个数组
来源：http://ysc.cashguo.top

Py:   a + b;  a.extend(b)
来源：http://vmj.yuxming.cn

PHP:  array_merge($a, $b);
来源：http://uqx.svipenyu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://byy.gogol.net.cn

TS:   [...a, ...b];
来源：http://epq.zdbjq.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tta.zdbjq.cn

Go:   append(a, b...)
来源：http://sna.zhijiandao.cn

Ruby: a + b;  a.concat(b)
来源：http://zrl.ydzc1.top

C#:   a.Concat(b).ToList()
来源：http://zrs.kuanghao11.cn

[D09] 排序（升序）
来源：http://idk.wangdashe.top

Py:   sorted(arr);  arr.sort()
来源：http://nan.zhijiandao.cn

PHP:  sort($arr);
来源：http://pxp.tianlin.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jfw.pycfn.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://ube.fanxiaobao.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://ora.yj20258888.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nza.guannengcc.top

Ruby: arr.sort
来源：http://dmi.jyoumei.cn

C#:   list.Sort();
来源：http://bvm.fktsv.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://odc.xinyue.icu

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mxx.zdqjudy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dsp.jqgfzy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pit.kuanghao11.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fzr.vqdsnc.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dhp.zycfv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nik.birdmap.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wvl.vehdjk.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rpu.sxryk.cn


<!-- 参考信息 -->