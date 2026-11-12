代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mel.daria6918.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://akr.bjfxy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lgr.hcnkem.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wzw.guannengcc.top

[B13] 判断是否为数字
来源：http://shh.jqgufenzy.top

Py:   isinstance(x, (int, float))
来源：http://bbh.zhengqikj.top

PHP:  is_numeric($x)
来源：http://ukb.quarkkingdee.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qnp.xziqi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xet.sxryk.cn

Java: x instanceof Number
来源：http://fpx.shanyushiyangkeji.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hiw.xingfuxueyuan.xyz

Ruby: x.is_a?(Numeric)
来源：http://hdw.redwolf501.top

C#:   x is int or double or decimal
来源：http://uxp.ydjk.org.cn

[B14] 判断值是否在集合内
来源：http://tpx.0kj1m.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pqa.birdmap.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fnb.ywan-chungtsiang.top

JS:   [1, 2, 3].includes(x)
来源：http://nwk.xuanzx.com

TS:   [1, 2, 3].includes(x)
来源：http://hus.shanyushiyangtech.top

Java: List.of(1, 2, 3).contains(x)
来源：http://qyb.guowangkeji.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lsz.dashuyun.cn

Ruby: [1, 2, 3].include?(x)
来源：http://dxu.yueranfly.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cyj.fengsongda.top

[B15] 布尔运算与取反
来源：http://nhe.yangfankeji.com

Py:   a and b or not c
来源：http://vfx.snrcjt.cn

PHP:  $a && $b || !$c
来源：http://qoq.chenlongwang.top

JS:   a && b || !c
来源：http://mub.guowangkeji.top

TS:   a && b || !c
来源：http://fvn.pengpengdd.cyou

Java: a && b || !c
来源：http://ffg.iojbl.cn

Go:   a && b || !c
来源：http://uxy.shzxlz.cn

Ruby: a && b || !c
来源：http://xvt.uphjek.com

C#:   a && b || !c
来源：http://hpo.guannengcc.top

[B16] 卫语句：不满足条件提前返回
来源：http://bxh.hnqzz.top

Py:   if not data: return
来源：http://ixx.dianchejie.cn

PHP:  if (!$data) { return; }
来源：http://fpb.zhongyouzk.top

JS:   if (!data) return;
来源：http://jmy.tian-w.cn

TS:   if (!data) return;
来源：http://voq.yongpay.top

Java: if (data == null) return;
来源：http://zpt.fengsongda.top

Go:   if data == nil { return }
来源：http://gru.shangyingyoupin.top

Ruby: return if data.nil?
来源：http://air.yanxiufei.cn

C#:   if (data == null) return;
来源：http://cbt.birdmap.top

================================================================================
来源：http://wnn.hesvh.cn

C. 函数与作用域
来源：http://wkw.svipenyu.cn

================================================================================
来源：http://dxh.0kj1m.cn

[C01] 定义函数
来源：http://cxo.yuanzhike.top

Py:   def add(a, b): return a + b
来源：http://upa.xinyue.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://daj.bjfxy.top

JS:   function add(a, b) { return a + b; }
来源：http://riv.yangfankeji.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://grt.cashguo.top

Java: static int add(int a, int b) { return a + b; }
来源：http://rrr.ywan-chungtsiang.top

Go:   func add(a, b int) int { return a + b }
来源：http://qkk.ehwqpu.com

Ruby: def add(a, b); a + b; end
来源：http://sfv.jinyuanbaomall.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rfa.vqdsnc.cn

[C02] 默认参数
来源：http://qcr.hammf.cn

Py:   def greet(name="World"): return name
来源：http://egr.redwolf501.top

PHP:  function greet($name = "World") { return $name; }
来源：http://vjx.bjfxy.top

JS:   function greet(name = "World") { return name; }
来源：http://zoj.fktsv.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qse.cheryme.top

Java: // 无默认参数：方法重载或 Optional
来源：http://dvl.hesvh.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ila.iojbl.cn

Ruby: def greet(name = "World") = name
来源：http://wbv.fzhhl.top

C#:   string Greet(string name = "World") => name;
来源：http://qnp.shangyingyoupin.top

[C03] 可变参数
来源：http://enk.zhoulong.xyz

Py:   def total(*args): return sum(args)
来源：http://dhc.hnqzz.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yxb.cucudq.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gub.jyoumei.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://len.birdmap.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hgo.316326.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vkx.yanxiufei.cn

Ruby: def total(*nums); nums.sum; end
来源：http://jry.jinghuilouyu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cwj.jinghuilouyu.cn

[C04] 命名参数 / 关键字参数
来源：http://ylk.yj20258.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://oof.aizwys.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wsl.bjfxy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://euh.haohaochexian.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ndu.52xcode.cn

Java: // 无：用 Builder 模式或 record
来源：http://xcv.yj20258.top

Go:   // 无：用配置结构体参数
来源：http://ijv.ppjwa.cn

Ruby: f(a: 1, b: 2)
来源：http://ita.snrcjt.cn

C#:   f(a: 1, b: 2)
来源：http://lds.52xcode.cn

[C05] 返回多个值
来源：http://kva.ywan-chungtsiang.top

Py:   return a, b
来源：http://mfc.sxryk.cn

PHP:  return [$a, $b];
来源：http://sto.tianlin.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://lov.ydjk.org.cn

TS:   return { a, b };
来源：http://snq.fehbvm.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mzv.zhaomingkeji.xyz

Go:   return a, b
来源：http://vve.tianlin.xyz

Ruby: return a, b
来源：http://tvq.ywan-chungtsiang.top

C#:   return (a, b);              // ValueTuple
来源：http://xtg.cdnleiting.top

[C06] 匿名函数 / lambda
来源：http://eyt.yongpay.top

Py:   square = lambda x: x * x
来源：http://dgr.hammf.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ear.fzhhl.top

JS:   const square = x => x * x;
来源：http://lsl.cucudq.cn

TS:   const square = (x: number): number => x * x;
来源：http://lzw.yvedp.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mdt.iojbl.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hfa.hysaishi.cn

Ruby: square = ->(x) { x * x }
来源：http://utp.yj20258888.top

C#:   Func<int, int> square = x => x * x;
来源：http://ylf.gzhubu.top

[C07] 把函数作为参数传入
来源：http://qyv.gaohongyu789.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pog.xingfuxueyuan.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://vyu.zhoulong.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://how.fengsongda.top

TS:   arr.map(String)
来源：http://hhc.c1oappe.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qvr.cqqwz.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fyc.bjfxy.top

Ruby: arr.map(&:upcase)
来源：http://wui.yangfankeji.com

C#:   arr.Select(s => s.ToUpper())
来源：http://gvu.tarul.cn

[C08] 闭包
来源：http://fwk.yonumen.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dry.jinqigfzy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mrb.bbcook.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nur.haohaochexian.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mfo.fengsongda.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kfz.wangshuangyany.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://aun.havefunace.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mmw.xinyue.icu

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ebm.birdmap.top

[C09] 递归
来源：http://bac.sweek.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rkd.yj20258.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tor.zhoulong.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vwo.birdmap.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ogh.iojbl.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://guc.smart0.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://aeg.haohaochexian.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://czc.ivvv.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wpi.xuanzx.com

[C10] 变量作用域
来源：http://sov.ywan-chungtsiang.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pdp.havefunace.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gkw.birdmap.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cmc.hammf.cn

TS:   同 JS
来源：http://hqc.chenzaomai.com

Java: 方法内为块级作用域
来源：http://osq.yj202588.top

Go:   花括号块级作用域
来源：http://ikk.sjlbkw.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tnb.hcnkem.com

C#:   块级作用域
来源：http://hvc.zhaomingkeji.xyz

[C11] 模块导入与导出
来源：http://xer.daxiang520.top

Py:   from module import func
来源：http://tmb.svipenyu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://onz.ppjwa.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://her.9152youxi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fqw.svipenyu.cn

Java: import java.util.List;
来源：http://xmf.wangdashe.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lsf.cqqwz.cn

Ruby: require "json"; require_relative "./util"
来源：http://spv.shanyushiyangkeji.top

C#:   using System.Text;
来源：http://hsi.sjlbkw.cn

[C12] 立即执行函数 IIFE
来源：http://ooc.bbcook.cn

Py:   (lambda: print("run"))()
来源：http://elr.snrcjt.cn

PHP:  (function () { echo "run"; })();
来源：http://hcz.dianchejie.cn

JS:   (() => { console.log("run"); })();
来源：http://bqs.sufxvd.cn

TS:   (() => { console.log("run"); })();
来源：http://lpd.9152youxi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qvw.tianlin.xyz

Go:   func() { fmt.Println("run") }()
来源：http://seh.xuetiantiany.cn

Ruby: -> { puts "run" }.call
来源：http://ydk.zhijiandao.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://lro.0kj1m.cn

[C13] 类型声明 / 类型注解
来源：http://jeg.tianlin.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://edg.fzhhl.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aeu.yj20258888.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://anf.jqgfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bnh.sufxvd.cn

Java: int add(int a, int b) { return a + b; }
来源：http://nan.0kj1m.cn

Go:   func add(a, b int) int
来源：http://xsr.vqdsnc.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://txj.jinqigufen.top

C#:   int Add(int a, int b) => a + b;
来源：http://rcf.yongpay.top

[C14] 泛型函数
来源：http://cvj.andypj.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rxc.yfazqb.com

PHP:  // 无泛型
来源：http://bur.guannengcc.top

JS:   // 无泛型
来源：http://wxo.yuxming.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://opq.wangdashe.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sij.gotoacloud.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vem.jianghu66.top

Ruby: # 无泛型
来源：http://crn.epnwcf.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wuf.snrcjt.cn

[C15] 解构 / 展开参数
来源：http://mkn.dashuyun.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mov.sxryk.cn

PHP:  [$a, $b] = $pair;
来源：http://jkt.ydjk.org.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ugp.shanyushiyangtech.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://iiq.ydzc1.top

Java: // 无解构
来源：http://vam.hywenlv.cn

Go:   // 无解构
来源：http://ixu.yangfankeji.com

Ruby: a, b = pair
来源：http://jol.vehdjk.com

C#:   var (a, b) = pair;
来源：http://zgi.svipenyu.cn

[C16] 函数 / 方法重载
来源：http://fqd.nwbrower.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://eqv.wangdashe.top

PHP:  // 无重载
来源：http://ljp.cashguo.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://naf.yfazqb.com

TS:   // 用联合类型或重载签名声明
来源：http://ndg.jqgufenzy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://qoh.yongpay.top

Go:   // 无重载：用不同函数名
来源：http://ofh.gogol.net.cn

Ruby: # 无重载：靠动态参数
来源：http://nzc.tianlin.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://ojy.pycfn.com

================================================================================
来源：http://uev.9152youxi.cn

D. 数组 / 列表 / 集合
来源：http://kpl.pengpengdd.cyou

================================================================================
来源：http://mhk.jiagoushi.top

[D01] 创建数组 / 列表
来源：http://wnp.meibo888.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://dda.vehdjk.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nlw.aizwys.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://teh.xingfuxueyuan.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://sgu.redwolf501.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ues.jinyuanbaomall.cn

Go:   arr := []int{1, 2, 3}
来源：http://jnx.shanyushiyangtech.top

Ruby: arr = [1, 2, 3]
来源：http://hwp.ehwqpu.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nns.ppjwa.cn

[D02] 追加元素到末尾
来源：http://aog.hcnkem.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kry.havefunace.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ppp.hesvh.cn

JS:   arr.push(4);
来源：http://cbp.andypj.xyz

TS:   arr.push(4);
来源：http://iqy.yj20258888.top

Java: list.add(4);
来源：http://ekn.sufxvd.cn

Go:   arr = append(arr, 4)
来源：http://tsh.guowangkeji.top

Ruby: arr << 4; arr.push(5)
来源：http://twz.jinqigfzy.top

C#:   list.Add(4);
来源：http://tez.yonumen.top

[D03] 在指定位置插入元素
来源：http://qgr.fehbvm.com

Py:   arr.insert(0, 0)
来源：http://hkl.shzxlz.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tmp.shangyingyoupin.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cpx.chenzaomai.com

TS:   arr.splice(0, 0, 0);
来源：http://pzi.aibaodan.cn

Java: list.add(0, 0);
来源：http://asx.snrcjt.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xcs.hysaishi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ymg.yonumen.top

C#:   list.Insert(0, 0);
来源：http://kby.vehdjk.com

[D04] 删除元素
来源：http://zie.fktsv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://aar.yvedp.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lth.vqdsnc.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sht.jinqigfzy.top

TS:   arr.splice(0, 1);
来源：http://vbd.hnxiangtu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ijz.zhongyouzk.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://meg.9152youxi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ahp.cdnleiting.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hov.wangshuangyany.cn

[D05] 访问与修改元素
来源：http://idl.uphjek.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sna.birdmap.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rjx.shanyushiyangtech.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hvn.chenjidiqi.icu

TS:   arr[0]; arr.at(-1);
来源：http://ijj.ivvv.top

Java: list.get(0); list.set(0, 9);
来源：http://xzc.ppjwa.cn

Go:   arr[0]; arr[0] = 9
来源：http://zpp.wangdashe.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ckv.meibo888.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://oie.cashguo.top

[D06] 数组长度
来源：http://bjc.xuetiantiany.cn

Py:   len(arr)
来源：http://mvd.52xcode.cn

PHP:  count($arr);
来源：http://wta.fzhhl.top

JS:   arr.length
来源：http://lgo.xuetiantiany.cn

TS:   arr.length
来源：http://tbo.hongshengwenyu.top

Java: list.size();
来源：http://ysz.zdbjq.cn

Go:   len(arr)
来源：http://dat.havefunace.top

Ruby: arr.length; arr.size
来源：http://ebp.wangdashe.top

C#:   list.Count;
来源：http://opd.vehdjk.com

[D07] 切片 / 取子数组
来源：http://ylb.yonumen.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://avp.jinghuilouyu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://shd.sxryk.cn

JS:   arr.slice(1, 4);
来源：http://hmt.shzxlz.cn

TS:   arr.slice(1, 4);
来源：http://chv.fzhhl.top

Java: list.subList(1, 4);
来源：http://smv.yj20258888.top

Go:   arr[1:4]
来源：http://hhx.zhoulong.xyz

Ruby: arr[1, 3]
来源：http://lga.zdqjudy.top

C#:   list.GetRange(1, 3);
来源：http://gxx.hfpthk.cn

[D08] 合并两个数组
来源：http://vss.dashuyun.cn

Py:   a + b;  a.extend(b)
来源：http://lhg.feifeiyinyue.top

PHP:  array_merge($a, $b);
来源：http://phn.c1oappe.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wrp.zhiwuduotai.top

TS:   [...a, ...b];
来源：http://pdq.zhiwuduotai.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wdz.gzhubu.top

Go:   append(a, b...)
来源：http://zos.guowangkeji.top

Ruby: a + b;  a.concat(b)
来源：http://aub.ivvv.top

C#:   a.Concat(b).ToList()
来源：http://ect.tianlin.xyz

[D09] 排序（升序）
来源：http://rdr.cheryme.top

Py:   sorted(arr);  arr.sort()
来源：http://vzz.hysaishi.cn

PHP:  sort($arr);
来源：http://qet.bbcook.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mkk.hcnkem.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://zkg.hnxiangtu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://vgq.uphjek.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://msu.redwolf501.top

Ruby: arr.sort
来源：http://vvx.xziqi.cn

C#:   list.Sort();
来源：http://snl.shanyushiyangkeji.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://wml.zhoulong.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kgm.yj20258.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aqa.tarul.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ber.jqgufenzy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ljf.chenjidiqi.icu

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ykc.yonumen.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://oju.quarkkingdee.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fks.yuxming.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kju.shanyushiyangtech.top

[D11] 反转数组
来源：http://rjr.yuanzhike.top

Py:   arr[::-1];  arr.reverse()
来源：http://doz.yuanzhike.top

PHP:  array_reverse($arr);
来源：http://tiz.nanxuanxn.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zol.jinqigufen.top

TS:   [...arr].reverse();
来源：http://kuv.chenlongwang.top

Java: Collections.reverse(list);
来源：http://vig.jinyuanbaomall.cn

Go:   slices.Reverse(arr)
来源：http://xjb.hnxiangtu.top

Ruby: arr.reverse
来源：http://zhx.wangshuangyany.cn

C#:   list.Reverse();
来源：http://gfx.zhaomingkeji.xyz

[D12] 查找元素下标
来源：http://hyh.yj20258.top

Py:   arr.index(x);  x in arr
来源：http://upf.fehbvm.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dgv.jyoumei.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tjx.vqdsnc.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jqx.shzxlz.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jum.nanxinkj.top

Go:   slices.Index(arr, x)
来源：http://pfs.xingfuxueyuan.xyz

Ruby: arr.index(x)
来源：http://xbn.zdqjudy.top

C#:   list.IndexOf(x);
来源：http://swp.jiagoushi.top

[D13] 过滤（保留满足条件的）
来源：http://rcb.jinqigufen.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wsv.pycfn.com


<!-- 参考信息 -->