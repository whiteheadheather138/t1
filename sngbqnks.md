代发 wailian999

PHP:  range(0, 10, 2);
来源：http://dph.jyoumei.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dxp.guowangkeji.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fhs.yongpay.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kva.nanxinkj.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fru.yj20258.top

Ruby: (0...10).step(2).to_a
来源：http://jkg.ctjpmb.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gfy.xuanzx.com

[B12] 跳出多层循环
来源：http://rjo.vqdsnc.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://skx.yangfankeji.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://hfv.daxiang520.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://byh.guowangkeji.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zfg.chenjidiqi.icu

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kaa.yuxming.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vin.yuxming.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pof.cqqwz.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://skn.fehbvm.com

[B13] 判断是否为数字
来源：http://pga.bjfxy.top

Py:   isinstance(x, (int, float))
来源：http://bvm.fengsongda.top

PHP:  is_numeric($x)
来源：http://qdj.ehwqpu.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vsx.yj202588.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uhq.meibo888.top

Java: x instanceof Number
来源：http://tjy.jqgfzy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://krh.sweek.top

Ruby: x.is_a?(Numeric)
来源：http://fkf.yj20258.top

C#:   x is int or double or decimal
来源：http://wsh.nanxinkj.top

[B14] 判断值是否在集合内
来源：http://cuo.zhijiandao.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yes.cucudq.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tjm.sweek.top

JS:   [1, 2, 3].includes(x)
来源：http://tjc.chenlongwang.top

TS:   [1, 2, 3].includes(x)
来源：http://nyh.52xcode.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qpz.hesvh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://udq.cqqwz.cn

Ruby: [1, 2, 3].include?(x)
来源：http://bvs.daria6918.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nvw.gaohongyu789.top

[B15] 布尔运算与取反
来源：http://yli.andypj.xyz

Py:   a and b or not c
来源：http://oug.yueranfly.top

PHP:  $a && $b || !$c
来源：http://fpl.yongpay.top

JS:   a && b || !c
来源：http://mrc.chenlongwang.top

TS:   a && b || !c
来源：http://kkz.sweek.top

Java: a && b || !c
来源：http://jml.zhiwuduotai.top

Go:   a && b || !c
来源：http://oxl.jiagoushi.top

Ruby: a && b || !c
来源：http://dpb.zdqjudy.top

C#:   a && b || !c
来源：http://vgb.yj202588.top

[B16] 卫语句：不满足条件提前返回
来源：http://dwd.yj202588.top

Py:   if not data: return
来源：http://cit.sjlbkw.cn

PHP:  if (!$data) { return; }
来源：http://frj.snrcjt.cn

JS:   if (!data) return;
来源：http://hll.yongpay.top

TS:   if (!data) return;
来源：http://bkv.yuxming.cn

Java: if (data == null) return;
来源：http://zra.zhongyouzk.top

Go:   if data == nil { return }
来源：http://hoa.ydjk.org.cn

Ruby: return if data.nil?
来源：http://okc.andypj.xyz

C#:   if (data == null) return;
来源：http://ofj.zycfv.cn

================================================================================
来源：http://wch.birdmap.top

C. 函数与作用域
来源：http://qwx.jlsjyb.cn

================================================================================
来源：http://rvc.fengsongda.top

[C01] 定义函数
来源：http://ahp.gotoacloud.top

Py:   def add(a, b): return a + b
来源：http://fdc.sxryk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ore.dashuyun.cn

JS:   function add(a, b) { return a + b; }
来源：http://gya.zycfv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fyf.smart0.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://qov.tian-w.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ccb.zhongyouzk.top

Ruby: def add(a, b); a + b; end
来源：http://ggq.fehbvm.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jcm.hfpthk.cn

[C02] 默认参数
来源：http://dqb.hnxiangtu.top

Py:   def greet(name="World"): return name
来源：http://wjs.hnxiangtu.top

PHP:  function greet($name = "World") { return $name; }
来源：http://gax.cashguo.top

JS:   function greet(name = "World") { return name; }
来源：http://awy.fktsv.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://nrr.zhaomingkeji.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://cql.jqgufenzy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kjj.zhongyouzk.top

Ruby: def greet(name = "World") = name
来源：http://ejh.9152youxi.cn

C#:   string Greet(string name = "World") => name;
来源：http://fqq.jyoumei.cn

[C03] 可变参数
来源：http://rjd.guowangkeji.top

Py:   def total(*args): return sum(args)
来源：http://ros.chenzaomai.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dok.gotoacloud.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fof.jyoumei.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://azo.yanxiufei.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jmh.shzxlz.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zsz.tanke756.top

Ruby: def total(*nums); nums.sum; end
来源：http://syf.tanke756.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://uix.fktsv.cn

[C04] 命名参数 / 关键字参数
来源：http://xxi.jlsjyb.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bqk.xuetiantiany.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bin.bbcook.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gyi.jinyuanbaomall.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mdw.tianlin.xyz

Java: // 无：用 Builder 模式或 record
来源：http://dfc.hammf.cn

Go:   // 无：用配置结构体参数
来源：http://xfy.jinqigfzy.top

Ruby: f(a: 1, b: 2)
来源：http://rxp.zhixingplan.top

C#:   f(a: 1, b: 2)
来源：http://kds.fktsv.cn

[C05] 返回多个值
来源：http://tns.shanyushiyangtech.top

Py:   return a, b
来源：http://skb.chenzaomai.com

PHP:  return [$a, $b];
来源：http://yvx.zdbjq.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://axw.mhx1999.top

TS:   return { a, b };
来源：http://fmu.vqdsnc.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bnl.haohaochexian.top

Go:   return a, b
来源：http://zcn.shanyushiyangtech.top

Ruby: return a, b
来源：http://nmz.yvedp.cn

C#:   return (a, b);              // ValueTuple
来源：http://vvg.zhaomingkeji.xyz

[C06] 匿名函数 / lambda
来源：http://bir.snrcjt.cn

Py:   square = lambda x: x * x
来源：http://ckq.epnwcf.com

PHP:  $square = fn($x) => $x * $x;
来源：http://icl.snrcjt.cn

JS:   const square = x => x * x;
来源：http://zey.yvedp.cn

TS:   const square = (x: number): number => x * x;
来源：http://csp.zhixingplan.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bqr.gotoacloud.top

Go:   sq := func(x int) int { return x * x }
来源：http://scs.yonumen.top

Ruby: square = ->(x) { x * x }
来源：http://igh.fanxiaobao.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://jgi.uphjek.com

[C07] 把函数作为参数传入
来源：http://jhd.xuanzx.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yjg.shanyushiyangtech.top

PHP:  array_map("strtoupper", $arr);
来源：http://tif.vehdjk.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://aeq.zhongyouzk.top

TS:   arr.map(String)
来源：http://reu.zhijiandao.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jvx.nanxinkj.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ucf.tanke756.top

Ruby: arr.map(&:upcase)
来源：http://niu.vehdjk.com

C#:   arr.Select(s => s.ToUpper())
来源：http://eso.dianchejie.cn

[C08] 闭包
来源：http://pyz.jlsjyb.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uuv.fzhhl.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mgs.zhiwuduotai.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uzm.chenjidiqi.icu

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ccs.cqqwz.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rjd.sjlbkw.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yhz.hcnkem.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://oqh.yueranfly.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jgw.wangshuangyany.cn

[C09] 递归
来源：http://ozv.yuxming.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gen.yonumen.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rxa.shzxlz.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ris.jinqigufen.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cpt.hfpthk.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wjz.yuanzhike.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tbn.jinqigfzy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vwf.ydzc1.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ydp.zhiwuduotai.top

[C10] 变量作用域
来源：http://voe.cashguo.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ojh.sweek.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lou.daxiang520.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vko.hnxiangtu.top

TS:   同 JS
来源：http://caq.hongshengwenyu.top

Java: 方法内为块级作用域
来源：http://yhz.zhijiandao.cn

Go:   花括号块级作用域
来源：http://pba.yuanzhike.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fpj.yonumen.top

C#:   块级作用域
来源：http://rva.jiagoushi.top

[C11] 模块导入与导出
来源：http://mye.fehbvm.com

Py:   from module import func
来源：http://kce.zhiwuduotai.top

PHP:  require "file.php";  或 use App\Service;
来源：http://zds.meibo888.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://tpc.tian-w.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ezv.tian-w.cn

Java: import java.util.List;
来源：http://hyb.jinqigfzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hln.hfpthk.cn

Ruby: require "json"; require_relative "./util"
来源：http://ywl.ydzc1.top

C#:   using System.Text;
来源：http://oae.hcnkem.com

[C12] 立即执行函数 IIFE
来源：http://qpf.tian-w.cn

Py:   (lambda: print("run"))()
来源：http://omk.xuetiantiany.cn

PHP:  (function () { echo "run"; })();
来源：http://jnk.tianlin.xyz

JS:   (() => { console.log("run"); })();
来源：http://vbx.shuidangran.top

TS:   (() => { console.log("run"); })();
来源：http://mii.tanke756.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kjx.zycfv.cn

Go:   func() { fmt.Println("run") }()
来源：http://qtk.jqgufenzy.top

Ruby: -> { puts "run" }.call
来源：http://amu.hysaishi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ewj.gotoacloud.top

[C13] 类型声明 / 类型注解
来源：http://pwl.ivvv.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fed.vqdsnc.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yqb.chenlongwang.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ujb.snrcjt.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nrb.shanyushiyangtech.top

Java: int add(int a, int b) { return a + b; }
来源：http://frc.kuanghao11.cn

Go:   func add(a, b int) int
来源：http://ixf.316326.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nou.yanxiufei.cn

C#:   int Add(int a, int b) => a + b;
来源：http://yrj.sweek.top

[C14] 泛型函数
来源：http://yii.tianlin.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uvk.jinqigufen.top

PHP:  // 无泛型
来源：http://kgd.yanxiufei.cn

JS:   // 无泛型
来源：http://pzo.zhaomingkeji.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tbr.sufxvd.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uzh.hongshengwenyu.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wiy.xinyue.icu

Ruby: # 无泛型
来源：http://wev.sxryk.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://iza.tian-w.cn

[C15] 解构 / 展开参数
来源：http://bik.hongshengwenyu.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vap.zdbjq.cn

PHP:  [$a, $b] = $pair;
来源：http://sfk.zhongyouzk.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uyc.yonumen.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lit.ctjpmb.com

Java: // 无解构
来源：http://fyg.xuetiantiany.cn

Go:   // 无解构
来源：http://vjl.hammf.cn

Ruby: a, b = pair
来源：http://zyd.quarkkingdee.top

C#:   var (a, b) = pair;
来源：http://zcv.fanxiaobao.xyz

[C16] 函数 / 方法重载
来源：http://mly.hfpthk.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jqh.jianghu66.top

PHP:  // 无重载
来源：http://chi.cashguo.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ngd.zhaomingkeji.xyz

TS:   // 用联合类型或重载签名声明
来源：http://rev.xziqi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hkt.shanyushiyangtech.top

Go:   // 无重载：用不同函数名
来源：http://mrs.kuanghao11.cn

Ruby: # 无重载：靠动态参数
来源：http://yea.sjlbkw.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rpa.52xcode.cn

================================================================================
来源：http://hhr.jlsjyb.cn

D. 数组 / 列表 / 集合
来源：http://zux.yuanzhike.top

================================================================================
来源：http://adp.kuanghao11.cn

[D01] 创建数组 / 列表
来源：http://bet.aizwys.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hlq.xziqi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tks.fehbvm.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mtg.hongshengwenyu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://mht.yangfankeji.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dco.quarkkingdee.top

Go:   arr := []int{1, 2, 3}
来源：http://cms.ehwqpu.com

Ruby: arr = [1, 2, 3]
来源：http://hyl.chenjidiqi.icu

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pjk.yueranfly.top

[D02] 追加元素到末尾
来源：http://yzk.wangdashe.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ada.svipenyu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lof.snrcjt.cn

JS:   arr.push(4);
来源：http://qxm.gogol.net.cn

TS:   arr.push(4);
来源：http://bcc.yfazqb.com

Java: list.add(4);
来源：http://gxx.xuetiantiany.cn

Go:   arr = append(arr, 4)
来源：http://non.bbcook.cn

Ruby: arr << 4; arr.push(5)
来源：http://bro.yonumen.top

C#:   list.Add(4);
来源：http://zrg.hnxiangtu.top

[D03] 在指定位置插入元素
来源：http://aiv.xuanzx.com

Py:   arr.insert(0, 0)
来源：http://nmb.gzhubu.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ofz.fehbvm.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uuy.zhoulong.xyz

TS:   arr.splice(0, 0, 0);
来源：http://yhm.pengpengdd.cyou

Java: list.add(0, 0);
来源：http://jyn.wangshuangyany.cn

Go:   arr = append([]int{0}, arr...)
来源：http://dre.dashuyun.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fpu.cqqwz.cn

C#:   list.Insert(0, 0);
来源：http://snj.xinyue.icu

[D04] 删除元素
来源：http://hyf.yj202588.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jrq.hysaishi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gag.jinqigfzy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://umf.9152youxi.cn

TS:   arr.splice(0, 1);
来源：http://ucg.tanke756.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ewz.9152youxi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kxl.guannengcc.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://twt.ivvv.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ffd.zhongyouzk.top

[D05] 访问与修改元素
来源：http://gsh.ppjwa.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://neq.daxiang520.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://adx.tian-w.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://btl.uphjek.com

TS:   arr[0]; arr.at(-1);
来源：http://fzh.haohaochexian.top

Java: list.get(0); list.set(0, 9);
来源：http://xel.hammf.cn

Go:   arr[0]; arr[0] = 9
来源：http://ndd.gzhubu.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://krm.hywenlv.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yob.hnqzz.top

[D06] 数组长度
来源：http://txa.ehwqpu.com

Py:   len(arr)
来源：http://cuz.pycfn.com

PHP:  count($arr);
来源：http://gpk.haohaochexian.top

JS:   arr.length
来源：http://upo.zdqjudy.top

TS:   arr.length
来源：http://sdv.yj202588.top

Java: list.size();
来源：http://kdh.sufxvd.cn

Go:   len(arr)
来源：http://clt.hywenlv.cn

Ruby: arr.length; arr.size
来源：http://kcs.shangyingyoupin.top

C#:   list.Count;
来源：http://zhm.sufxvd.cn

[D07] 切片 / 取子数组
来源：http://dbr.xylfe.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nhc.iojbl.cn

PHP:  array_slice($arr, 1, 3);
来源：http://tsa.cqqwz.cn

JS:   arr.slice(1, 4);
来源：http://hjs.wangdashe.top

TS:   arr.slice(1, 4);
来源：http://rjz.snrcjt.cn

Java: list.subList(1, 4);
来源：http://npb.dashuyun.cn

Go:   arr[1:4]
来源：http://psc.fehbvm.com

Ruby: arr[1, 3]
来源：http://vgj.zhongyouzk.top

C#:   list.GetRange(1, 3);
来源：http://vee.ybcxt.top

[D08] 合并两个数组
来源：http://gjr.nanxinkj.top

Py:   a + b;  a.extend(b)
来源：http://qbp.hnxiangtu.top

PHP:  array_merge($a, $b);
来源：http://uoo.yvedp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xeg.ydjk.org.cn

TS:   [...a, ...b];
来源：http://pjf.jinyuanbaomall.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fou.andypj.xyz

Go:   append(a, b...)
来源：http://ahs.zhijiandao.cn

Ruby: a + b;  a.concat(b)
来源：http://igc.xylfe.cn

C#:   a.Concat(b).ToList()
来源：http://qdy.ywan-chungtsiang.top

[D09] 排序（升序）
来源：http://wjs.yuanzhike.top

Py:   sorted(arr);  arr.sort()
来源：http://bes.vehdjk.com

PHP:  sort($arr);
来源：http://pms.xylfe.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ifi.yongpay.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ios.vqdsnc.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://cts.jinyuanbaomall.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tzj.guowangkeji.top

Ruby: arr.sort
来源：http://mri.daria6918.cn

C#:   list.Sort();
来源：http://zct.jqgfzy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ucy.yuanzhike.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://awy.zhengqikj.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wav.ppjwa.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mpl.nanxinkj.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://neb.haohaochexian.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hhf.yj20258888.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://orc.snrcjt.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ujb.havefunace.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qdd.dianchejie.cn

[D11] 反转数组
来源：http://bsg.hywenlv.cn

Py:   arr[::-1];  arr.reverse()
来源：http://fih.feifeiyinyue.top

PHP:  array_reverse($arr);
来源：http://kbk.xylfe.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://iei.pengpengdd.cyou

TS:   [...arr].reverse();
来源：http://mbb.jinyuanbaomall.cn

Java: Collections.reverse(list);
来源：http://vhc.epnwcf.com

Go:   slices.Reverse(arr)
来源：http://xmp.ctjpmb.com

Ruby: arr.reverse
来源：http://kvg.hongshengwenyu.top


<!-- 参考信息 -->