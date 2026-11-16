代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nen.shuidangran.top

Ruby: (0...10).step(2).to_a
来源：http://gzn.gotoacloud.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ljj.dianchejie.cn

[B12] 跳出多层循环
来源：http://ykp.fzhhl.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://qwm.316326.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://nzm.hammf.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yuk.jinqigufen.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yqg.yueranfly.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ncw.9152youxi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pmv.yfazqb.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dfz.gzhubu.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qkd.shuidangran.top

[B13] 判断是否为数字
来源：http://neu.zycfv.cn

Py:   isinstance(x, (int, float))
来源：http://gsc.guannengcc.top

PHP:  is_numeric($x)
来源：http://lvr.9152youxi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sib.yongpay.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lez.shzxlz.cn

Java: x instanceof Number
来源：http://fxx.nanxinkj.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://npm.birdmap.top

Ruby: x.is_a?(Numeric)
来源：http://fgd.hysaishi.cn

C#:   x is int or double or decimal
来源：http://plb.gotoacloud.top

[B14] 判断值是否在集合内
来源：http://hrp.yvedp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dll.vqdsnc.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kqg.hongshengwenyu.top

JS:   [1, 2, 3].includes(x)
来源：http://qho.zhoulong.xyz

TS:   [1, 2, 3].includes(x)
来源：http://ual.aizwys.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qbk.chenlongwang.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://okj.jqgfzy.top

Ruby: [1, 2, 3].include?(x)
来源：http://lfd.xuetiantiany.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zuh.daxiang520.top

[B15] 布尔运算与取反
来源：http://zyi.kuanghao11.cn

Py:   a and b or not c
来源：http://zqa.daria6918.cn

PHP:  $a && $b || !$c
来源：http://tnu.tianlin.xyz

JS:   a && b || !c
来源：http://omo.feifeiyinyue.top

TS:   a && b || !c
来源：http://vsz.chenzaomai.com

Java: a && b || !c
来源：http://yfl.shanyushiyangkeji.top

Go:   a && b || !c
来源：http://fia.cdnleiting.top

Ruby: a && b || !c
来源：http://olt.vehdjk.com

C#:   a && b || !c
来源：http://yfv.tanke756.top

[B16] 卫语句：不满足条件提前返回
来源：http://yhw.chenlongwang.top

Py:   if not data: return
来源：http://isa.fanxiaobao.xyz

PHP:  if (!$data) { return; }
来源：http://yyp.xinyue.icu

JS:   if (!data) return;
来源：http://afz.shanyushiyangtech.top

TS:   if (!data) return;
来源：http://seh.ydzc1.top

Java: if (data == null) return;
来源：http://ine.havefunace.top

Go:   if data == nil { return }
来源：http://mtb.yj20258.top

Ruby: return if data.nil?
来源：http://zat.smart0.xyz

C#:   if (data == null) return;
来源：http://vlu.jiagoushi.top

================================================================================
来源：http://eti.aibaodan.cn

C. 函数与作用域
来源：http://vjw.yongpay.top

================================================================================
来源：http://dzh.jyoumei.cn

[C01] 定义函数
来源：http://yoo.cdnleiting.top

Py:   def add(a, b): return a + b
来源：http://xai.fehbvm.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jty.tian-w.cn

JS:   function add(a, b) { return a + b; }
来源：http://zox.jlsjyb.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://imp.andypj.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://wag.wangdashe.top

Go:   func add(a, b int) int { return a + b }
来源：http://kku.tarul.cn

Ruby: def add(a, b); a + b; end
来源：http://guo.epnwcf.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://oqv.chenzaomai.com

[C02] 默认参数
来源：http://ang.nanxuanxn.top

Py:   def greet(name="World"): return name
来源：http://sdw.xziqi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://uqf.guannengcc.top

JS:   function greet(name = "World") { return name; }
来源：http://sax.smart0.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://ybz.bbcook.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wbr.haohaochexian.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ylm.bbcook.cn

Ruby: def greet(name = "World") = name
来源：http://yra.gaohongyu789.top

C#:   string Greet(string name = "World") => name;
来源：http://fpv.chenzaomai.com

[C03] 可变参数
来源：http://efn.havefunace.top

Py:   def total(*args): return sum(args)
来源：http://tkv.aibaodan.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://djp.sufxvd.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://woi.hysaishi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fwx.hammf.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://web.zdbjq.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vim.zycfv.cn

Ruby: def total(*nums); nums.sum; end
来源：http://efb.zhengqikj.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dwa.yuanzhike.top

[C04] 命名参数 / 关键字参数
来源：http://puk.kuanghao11.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jab.xingfuxueyuan.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://oji.cashguo.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ubc.52xcode.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bcj.jlsjyb.cn

Java: // 无：用 Builder 模式或 record
来源：http://nws.guannengcc.top

Go:   // 无：用配置结构体参数
来源：http://ypm.jqgufenzy.top

Ruby: f(a: 1, b: 2)
来源：http://mmm.epnwcf.com

C#:   f(a: 1, b: 2)
来源：http://wmb.guannengcc.top

[C05] 返回多个值
来源：http://gpc.havefunace.top

Py:   return a, b
来源：http://imp.yueranfly.top

PHP:  return [$a, $b];
来源：http://xmo.shangyingyoupin.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://igg.chenzaomai.com

TS:   return { a, b };
来源：http://ito.yonumen.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mzy.uphjek.com

Go:   return a, b
来源：http://kwh.hnqzz.top

Ruby: return a, b
来源：http://vgd.ctjpmb.com

C#:   return (a, b);              // ValueTuple
来源：http://fiz.hongshengwenyu.top

[C06] 匿名函数 / lambda
来源：http://qfe.tanke756.top

Py:   square = lambda x: x * x
来源：http://his.ppjwa.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://oks.chenzaomai.com

JS:   const square = x => x * x;
来源：http://ppn.tian-w.cn

TS:   const square = (x: number): number => x * x;
来源：http://ljs.zhongyouzk.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dpz.zhixingplan.top

Go:   sq := func(x int) int { return x * x }
来源：http://uvd.cqqwz.cn

Ruby: square = ->(x) { x * x }
来源：http://dtx.mhx1999.top

C#:   Func<int, int> square = x => x * x;
来源：http://nwa.ydjk.org.cn

[C07] 把函数作为参数传入
来源：http://vwm.yuanzhike.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bza.9152youxi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://iqs.chenlongwang.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://aml.yfazqb.com

TS:   arr.map(String)
来源：http://ndj.zdqjudy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jml.jqgufenzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wkn.fktsv.cn

Ruby: arr.map(&:upcase)
来源：http://vry.hywenlv.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://srf.feifeiyinyue.top

[C08] 闭包
来源：http://lce.jinqigfzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://clz.xuanzx.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dfw.nwbrower.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jjs.andypj.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://scm.cucudq.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gog.yj202588.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zcd.cqqwz.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pha.cqqwz.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://psn.shuidangran.top

[C09] 递归
来源：http://rfq.shangyingyoupin.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vji.yonumen.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vfn.yangfankeji.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jjd.mhx1999.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qum.daxiang520.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pki.redwolf501.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qdk.bbcook.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yte.jqgufenzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dha.zhongyouzk.top

[C10] 变量作用域
来源：http://nwb.pengpengdd.cyou

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qxr.chenjidiqi.icu

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vge.ydjk.org.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uww.daria6918.cn

TS:   同 JS
来源：http://csz.yangfankeji.com

Java: 方法内为块级作用域
来源：http://pwk.yueranfly.top

Go:   花括号块级作用域
来源：http://wcn.zhijiandao.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vop.bbcook.cn

C#:   块级作用域
来源：http://weq.cheryme.top

[C11] 模块导入与导出
来源：http://svf.52xcode.cn

Py:   from module import func
来源：http://llj.aibaodan.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ict.meibo888.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://gwb.jianghu66.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uoa.hnxiangtu.top

Java: import java.util.List;
来源：http://aro.guannengcc.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://she.yfazqb.com

Ruby: require "json"; require_relative "./util"
来源：http://nof.pycfn.com

C#:   using System.Text;
来源：http://xzx.jqgufenzy.top

[C12] 立即执行函数 IIFE
来源：http://qjk.zycfv.cn

Py:   (lambda: print("run"))()
来源：http://kzf.uphjek.com

PHP:  (function () { echo "run"; })();
来源：http://avp.hesvh.cn

JS:   (() => { console.log("run"); })();
来源：http://ghs.birdmap.top

TS:   (() => { console.log("run"); })();
来源：http://vcu.vqdsnc.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cgz.shanyushiyangtech.top

Go:   func() { fmt.Println("run") }()
来源：http://wel.ctjpmb.com

Ruby: -> { puts "run" }.call
来源：http://nor.hesvh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://psm.uphjek.com

[C13] 类型声明 / 类型注解
来源：http://hqf.aibaodan.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dgq.daria6918.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://osd.chenzaomai.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cky.fengsongda.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jxi.chenlongwang.top

Java: int add(int a, int b) { return a + b; }
来源：http://zti.sjlbkw.cn

Go:   func add(a, b int) int
来源：http://vfj.yongpay.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bdf.hywenlv.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vsz.shuidangran.top

[C14] 泛型函数
来源：http://dba.snrcjt.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vzk.xziqi.cn

PHP:  // 无泛型
来源：http://dlk.ehwqpu.com

JS:   // 无泛型
来源：http://zgl.yonumen.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cbn.jqgfzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dtm.xylfe.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://eac.dianchejie.cn

Ruby: # 无泛型
来源：http://vgm.svipenyu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vbu.quarkkingdee.top

[C15] 解构 / 展开参数
来源：http://chr.ydjk.org.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jqx.vehdjk.com

PHP:  [$a, $b] = $pair;
来源：http://yqb.zhongyouzk.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fuv.snrcjt.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wml.jinghuilouyu.cn

Java: // 无解构
来源：http://vtr.ywan-chungtsiang.top

Go:   // 无解构
来源：http://mhj.fanxiaobao.xyz

Ruby: a, b = pair
来源：http://yah.ybcxt.top

C#:   var (a, b) = pair;
来源：http://cck.hesvh.cn

[C16] 函数 / 方法重载
来源：http://iha.hfpthk.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ohj.haohaochexian.top

PHP:  // 无重载
来源：http://fcf.xuetiantiany.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://yij.tanke756.top

TS:   // 用联合类型或重载签名声明
来源：http://ssm.dianchejie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gny.fehbvm.com

Go:   // 无重载：用不同函数名
来源：http://vie.zhongyouzk.top

Ruby: # 无重载：靠动态参数
来源：http://wax.hesvh.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zfi.havefunace.top

================================================================================
来源：http://hri.shangyingyoupin.top

D. 数组 / 列表 / 集合
来源：http://vkk.mhx1999.top

================================================================================
来源：http://tkc.yuanzhike.top

[D01] 创建数组 / 列表
来源：http://jss.daria6918.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://vfy.aibaodan.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gwp.hywenlv.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wyo.uphjek.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://yov.xuanzx.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bbk.daria6918.cn

Go:   arr := []int{1, 2, 3}
来源：http://org.xuetiantiany.cn

Ruby: arr = [1, 2, 3]
来源：http://leq.jqgfzy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zvx.chenlongwang.top

[D02] 追加元素到末尾
来源：http://mrv.xuanzx.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kyu.jqgufenzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vdd.pengpengdd.cyou

JS:   arr.push(4);
来源：http://wcv.jianghu66.top

TS:   arr.push(4);
来源：http://iqs.meibo888.top

Java: list.add(4);
来源：http://hws.dashuyun.cn

Go:   arr = append(arr, 4)
来源：http://lou.wangshuangyany.cn

Ruby: arr << 4; arr.push(5)
来源：http://rid.yangfankeji.com

C#:   list.Add(4);
来源：http://gax.mhx1999.top

[D03] 在指定位置插入元素
来源：http://uyf.hnqzz.top

Py:   arr.insert(0, 0)
来源：http://ngb.ybcxt.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dda.andypj.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rma.epnwcf.com

TS:   arr.splice(0, 0, 0);
来源：http://dfc.zhijiandao.cn

Java: list.add(0, 0);
来源：http://jvl.epnwcf.com

Go:   arr = append([]int{0}, arr...)
来源：http://xhm.zhengqikj.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://orq.sysykeji.top

C#:   list.Insert(0, 0);
来源：http://xhk.epnwcf.com

[D04] 删除元素
来源：http://rnj.zhaomingkeji.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fic.nwbrower.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lsg.ydjk.org.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tqq.jlsjyb.cn

TS:   arr.splice(0, 1);
来源：http://oka.jinghuilouyu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://uts.cqqwz.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://eqn.hysaishi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bye.fengsongda.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nqk.jlsjyb.cn

[D05] 访问与修改元素
来源：http://vvl.wangdashe.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ozv.chenjidiqi.icu

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lst.yongpay.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lcm.nwbrower.top

TS:   arr[0]; arr.at(-1);
来源：http://iyi.uphjek.com

Java: list.get(0); list.set(0, 9);
来源：http://nex.yvedp.cn

Go:   arr[0]; arr[0] = 9
来源：http://xnp.xylfe.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://utj.dianchejie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kah.ybcxt.top

[D06] 数组长度
来源：http://bxt.zhaomingkeji.xyz

Py:   len(arr)
来源：http://gua.chenlongwang.top

PHP:  count($arr);
来源：http://vuh.cucudq.cn

JS:   arr.length
来源：http://yjp.haohaochexian.top

TS:   arr.length
来源：http://sng.hcnkem.com

Java: list.size();
来源：http://cjb.ehwqpu.com

Go:   len(arr)
来源：http://rmj.shanyushiyangtech.top

Ruby: arr.length; arr.size
来源：http://wwx.tarul.cn

C#:   list.Count;
来源：http://yaq.jinqigufen.top

[D07] 切片 / 取子数组
来源：http://tfj.mhx1999.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xtw.pycfn.com

PHP:  array_slice($arr, 1, 3);
来源：http://nar.jlsjyb.cn

JS:   arr.slice(1, 4);
来源：http://ycz.birdmap.top

TS:   arr.slice(1, 4);
来源：http://ten.hcnkem.com

Java: list.subList(1, 4);
来源：http://ynd.xuanzx.com

Go:   arr[1:4]
来源：http://blt.ydjk.org.cn

Ruby: arr[1, 3]
来源：http://uuk.zhaomingkeji.xyz

C#:   list.GetRange(1, 3);
来源：http://ryp.ehwqpu.com

[D08] 合并两个数组
来源：http://mtp.aibaodan.cn

Py:   a + b;  a.extend(b)
来源：http://dqw.mhx1999.top

PHP:  array_merge($a, $b);
来源：http://ear.gotoacloud.top

JS:   [...a, ...b];  a.concat(b);
来源：http://jkn.jinghuilouyu.cn

TS:   [...a, ...b];
来源：http://hls.yj202588.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jeb.shanyushiyangkeji.top

Go:   append(a, b...)
来源：http://aor.sjlbkw.cn

Ruby: a + b;  a.concat(b)
来源：http://miq.zdbjq.cn

C#:   a.Concat(b).ToList()
来源：http://dxv.yj20258.top

[D09] 排序（升序）
来源：http://mwt.hnqzz.top

Py:   sorted(arr);  arr.sort()
来源：http://ofq.jinghuilouyu.cn

PHP:  sort($arr);
来源：http://hxz.jinyuanbaomall.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ist.zdbjq.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lzu.nanxuanxn.top

Java: Collections.sort(list);  list.sort(null);
来源：http://bjd.xuanzx.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gzq.haohaochexian.top

Ruby: arr.sort
来源：http://ffv.guannengcc.top

C#:   list.Sort();
来源：http://rum.iojbl.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://jva.jinyuanbaomall.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rdv.vqdsnc.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vwz.yvedp.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://edj.birdmap.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pbr.sxryk.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dum.zhongyouzk.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jms.aizwys.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zhn.hfpthk.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hxh.tanke756.top

[D11] 反转数组
来源：http://rzc.daxiang520.top

Py:   arr[::-1];  arr.reverse()
来源：http://fxp.fktsv.cn

PHP:  array_reverse($arr);
来源：http://mlc.tianlin.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qfw.yj202588.top

TS:   [...arr].reverse();
来源：http://wko.fzhhl.top

Java: Collections.reverse(list);
来源：http://fxh.zhijiandao.cn

Go:   slices.Reverse(arr)
来源：http://qyc.hesvh.cn

Ruby: arr.reverse
来源：http://yye.mhx1999.top

C#:   list.Reverse();
来源：http://mtf.shanyushiyangkeji.top

[D12] 查找元素下标
来源：http://ebl.xinyue.icu

Py:   arr.index(x);  x in arr
来源：http://uvk.fzhhl.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mwy.yuanzhike.top


<!-- 参考信息 -->