代发 wailian999

Go:   a && b || !c
来源：http://fny.hongshengwenyu.top

Ruby: a && b || !c
来源：http://adu.ivvv.top

C#:   a && b || !c
来源：http://frs.yj20258.top

[B16] 卫语句：不满足条件提前返回
来源：http://sja.sysykeji.top

Py:   if not data: return
来源：http://tzp.yuanzhike.top

PHP:  if (!$data) { return; }
来源：http://lzw.cheryme.top

JS:   if (!data) return;
来源：http://ema.ehwqpu.com

TS:   if (!data) return;
来源：http://vmr.zhongyouzk.top

Java: if (data == null) return;
来源：http://tkm.tanke756.top

Go:   if data == nil { return }
来源：http://pve.hnxiangtu.top

Ruby: return if data.nil?
来源：http://cum.jiagoushi.top

C#:   if (data == null) return;
来源：http://his.sysykeji.top

================================================================================
来源：http://rjn.hnxiangtu.top

C. 函数与作用域
来源：http://awv.shangyingyoupin.top

================================================================================
来源：http://ird.xziqi.cn

[C01] 定义函数
来源：http://vwu.aibaodan.cn

Py:   def add(a, b): return a + b
来源：http://zsc.316326.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://git.smart0.xyz

JS:   function add(a, b) { return a + b; }
来源：http://nnz.pengpengdd.cyou

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://knw.fanxiaobao.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://ixj.sjlbkw.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rmv.ppjwa.cn

Ruby: def add(a, b); a + b; end
来源：http://roa.bbcook.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jux.ydjk.org.cn

[C02] 默认参数
来源：http://tuf.guannengcc.top

Py:   def greet(name="World"): return name
来源：http://ehd.wangshuangyany.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://nsu.ywan-chungtsiang.top

JS:   function greet(name = "World") { return name; }
来源：http://wpi.xylfe.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gla.chenlongwang.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ebc.zdbjq.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lai.snrcjt.cn

Ruby: def greet(name = "World") = name
来源：http://etj.yj202588.top

C#:   string Greet(string name = "World") => name;
来源：http://nju.jlsjyb.cn

[C03] 可变参数
来源：http://afe.shzxlz.cn

Py:   def total(*args): return sum(args)
来源：http://uqq.fzhhl.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kch.yvedp.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://icq.sweek.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nbt.vqdsnc.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pmq.fzhhl.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vdx.ctjpmb.com

Ruby: def total(*nums); nums.sum; end
来源：http://tnp.xingfuxueyuan.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lbf.fktsv.cn

[C04] 命名参数 / 关键字参数
来源：http://yby.yuxming.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://psj.c1oappe.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fgp.cashguo.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sqm.xylfe.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nui.jqgufenzy.top

Java: // 无：用 Builder 模式或 record
来源：http://fnw.bjfxy.top

Go:   // 无：用配置结构体参数
来源：http://uwc.chenzaomai.com

Ruby: f(a: 1, b: 2)
来源：http://zuu.fehbvm.com

C#:   f(a: 1, b: 2)
来源：http://tpr.havefunace.top

[C05] 返回多个值
来源：http://lcr.cashguo.top

Py:   return a, b
来源：http://ycg.ywan-chungtsiang.top

PHP:  return [$a, $b];
来源：http://qin.vqdsnc.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://iej.yongpay.top

TS:   return { a, b };
来源：http://spl.havefunace.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://shs.pycfn.com

Go:   return a, b
来源：http://uoq.zhaomingkeji.xyz

Ruby: return a, b
来源：http://bkt.tarul.cn

C#:   return (a, b);              // ValueTuple
来源：http://jue.jqgufenzy.top

[C06] 匿名函数 / lambda
来源：http://snk.zhijiandao.cn

Py:   square = lambda x: x * x
来源：http://bsx.kuanghao11.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fqg.shuidangran.top

JS:   const square = x => x * x;
来源：http://rqm.jinqigufen.top

TS:   const square = (x: number): number => x * x;
来源：http://khr.jinghuilouyu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://eft.epnwcf.com

Go:   sq := func(x int) int { return x * x }
来源：http://tqu.zhixingplan.top

Ruby: square = ->(x) { x * x }
来源：http://vhr.ehwqpu.com

C#:   Func<int, int> square = x => x * x;
来源：http://dzv.sufxvd.cn

[C07] 把函数作为参数传入
来源：http://rgz.gotoacloud.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kzn.nanxinkj.top

PHP:  array_map("strtoupper", $arr);
来源：http://yiw.shangyingyoupin.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fcn.zycfv.cn

TS:   arr.map(String)
来源：http://ono.jinyuanbaomall.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://exr.xylfe.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dvy.yangfankeji.com

Ruby: arr.map(&:upcase)
来源：http://vwz.fktsv.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wvd.mhx1999.top

[C08] 闭包
来源：http://edw.jinghuilouyu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wjs.ybcxt.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wft.hnqzz.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://clo.fzhhl.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://iyz.jlsjyb.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tjc.aibaodan.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ivp.feifeiyinyue.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fvb.sxryk.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wet.jinyuanbaomall.cn

[C09] 递归
来源：http://zih.epnwcf.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qzf.ctjpmb.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qda.meibo888.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zkf.jqgufenzy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lpd.pengpengdd.cyou

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cys.chenjidiqi.icu

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://oom.wangdashe.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hyd.c1oappe.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lql.yvedp.cn

[C10] 变量作用域
来源：http://scb.jinqigufen.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://iij.yangfankeji.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://sbl.shzxlz.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fpr.vehdjk.com

TS:   同 JS
来源：http://gsb.ctjpmb.com

Java: 方法内为块级作用域
来源：http://tlo.hywenlv.cn

Go:   花括号块级作用域
来源：http://muu.sufxvd.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dvb.ivvv.top

C#:   块级作用域
来源：http://rzk.xziqi.cn

[C11] 模块导入与导出
来源：http://tbs.bjfxy.top

Py:   from module import func
来源：http://nji.yj20258.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ulv.chenjidiqi.icu

JS:   export default function f() {};  import f from "./m.js";
来源：http://oll.tarul.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qvb.zhoulong.xyz

Java: import java.util.List;
来源：http://vew.ydzc1.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hww.ydzc1.top

Ruby: require "json"; require_relative "./util"
来源：http://ghy.tarul.cn

C#:   using System.Text;
来源：http://ctp.hnxiangtu.top

[C12] 立即执行函数 IIFE
来源：http://mhz.xziqi.cn

Py:   (lambda: print("run"))()
来源：http://mrm.guannengcc.top

PHP:  (function () { echo "run"; })();
来源：http://srw.jqgfzy.top

JS:   (() => { console.log("run"); })();
来源：http://fot.zhaomingkeji.xyz

TS:   (() => { console.log("run"); })();
来源：http://yii.zhiwuduotai.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tgp.cashguo.top

Go:   func() { fmt.Println("run") }()
来源：http://yig.yangfankeji.com

Ruby: -> { puts "run" }.call
来源：http://kdo.316326.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://tio.shangyingyoupin.top

[C13] 类型声明 / 类型注解
来源：http://kxd.zhongyouzk.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pon.shanyushiyangtech.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zqn.jinqigufen.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lzg.guowangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yub.nanxinkj.top

Java: int add(int a, int b) { return a + b; }
来源：http://qpr.yfazqb.com

Go:   func add(a, b int) int
来源：http://adp.hcnkem.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zwv.pengpengdd.cyou

C#:   int Add(int a, int b) => a + b;
来源：http://ner.fengsongda.top

[C14] 泛型函数
来源：http://xtz.guannengcc.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rkt.yj20258888.top

PHP:  // 无泛型
来源：http://gwu.hysaishi.cn

JS:   // 无泛型
来源：http://six.ehwqpu.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dem.ybcxt.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tlr.vqdsnc.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qfr.jlsjyb.cn

Ruby: # 无泛型
来源：http://yfb.cheryme.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qco.ehwqpu.com

[C15] 解构 / 展开参数
来源：http://hgd.gzhubu.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://szr.aibaodan.cn

PHP:  [$a, $b] = $pair;
来源：http://yer.jqgufenzy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://oew.guannengcc.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cgs.cdnleiting.top

Java: // 无解构
来源：http://tzy.daria6918.cn

Go:   // 无解构
来源：http://sta.c1oappe.top

Ruby: a, b = pair
来源：http://gqh.sweek.top

C#:   var (a, b) = pair;
来源：http://aal.feifeiyinyue.top

[C16] 函数 / 方法重载
来源：http://wun.hywenlv.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://srj.hnxiangtu.top

PHP:  // 无重载
来源：http://ztx.smart0.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://jnf.xuetiantiany.cn

TS:   // 用联合类型或重载签名声明
来源：http://aks.jyoumei.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qkr.havefunace.top

Go:   // 无重载：用不同函数名
来源：http://ozd.bjfxy.top

Ruby: # 无重载：靠动态参数
来源：http://drz.daxiang520.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://nwq.guannengcc.top

================================================================================
来源：http://anp.jinyuanbaomall.cn

D. 数组 / 列表 / 集合
来源：http://awn.bjfxy.top

================================================================================
来源：http://rnk.gotoacloud.top

[D01] 创建数组 / 列表
来源：http://xtu.jianghu66.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://nnd.hnqzz.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ose.hesvh.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dyx.fanxiaobao.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://zvr.yangfankeji.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tej.jinyuanbaomall.cn

Go:   arr := []int{1, 2, 3}
来源：http://qhh.kuanghao11.cn

Ruby: arr = [1, 2, 3]
来源：http://vqn.dashuyun.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fgd.sjlbkw.cn

[D02] 追加元素到末尾
来源：http://muu.chenlongwang.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uwc.hfpthk.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kiq.ywan-chungtsiang.top

JS:   arr.push(4);
来源：http://mdy.xylfe.cn

TS:   arr.push(4);
来源：http://shs.jqgfzy.top

Java: list.add(4);
来源：http://gjm.uphjek.com

Go:   arr = append(arr, 4)
来源：http://yms.ybcxt.top

Ruby: arr << 4; arr.push(5)
来源：http://ufe.xuanzx.com

C#:   list.Add(4);
来源：http://upr.sxryk.cn

[D03] 在指定位置插入元素
来源：http://rci.cqqwz.cn

Py:   arr.insert(0, 0)
来源：http://gan.hnqzz.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hwv.ehwqpu.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fkd.yvedp.cn

TS:   arr.splice(0, 0, 0);
来源：http://vvm.sxryk.cn

Java: list.add(0, 0);
来源：http://qou.hongshengwenyu.top

Go:   arr = append([]int{0}, arr...)
来源：http://dac.yj20258888.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://clq.iojbl.cn

C#:   list.Insert(0, 0);
来源：http://tih.vqdsnc.cn

[D04] 删除元素
来源：http://ipw.yj202588.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kqe.xuanzx.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ozl.guannengcc.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lkz.shanyushiyangkeji.top

TS:   arr.splice(0, 1);
来源：http://hjg.zhiwuduotai.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ahw.gogol.net.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jax.cheryme.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wwv.ctjpmb.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ewp.vehdjk.com

[D05] 访问与修改元素
来源：http://oqk.cdnleiting.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://add.0kj1m.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zyw.sweek.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jyq.yuxming.cn

TS:   arr[0]; arr.at(-1);
来源：http://tik.feifeiyinyue.top

Java: list.get(0); list.set(0, 9);
来源：http://ddw.svipenyu.cn

Go:   arr[0]; arr[0] = 9
来源：http://lir.havefunace.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tht.cqqwz.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lnc.cheryme.top

[D06] 数组长度
来源：http://ich.gaohongyu789.top

Py:   len(arr)
来源：http://ses.nanxuanxn.top

PHP:  count($arr);
来源：http://dlh.cdnleiting.top

JS:   arr.length
来源：http://ivb.andypj.xyz

TS:   arr.length
来源：http://xrc.gzhubu.top

Java: list.size();
来源：http://pcy.shuidangran.top

Go:   len(arr)
来源：http://zeu.dianchejie.cn

Ruby: arr.length; arr.size
来源：http://gie.jinyuanbaomall.cn

C#:   list.Count;
来源：http://xjm.shzxlz.cn

[D07] 切片 / 取子数组
来源：http://zet.c1oappe.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://emy.fanxiaobao.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://gat.pycfn.com

JS:   arr.slice(1, 4);
来源：http://czx.shanyushiyangkeji.top

TS:   arr.slice(1, 4);
来源：http://pol.yfazqb.com

Java: list.subList(1, 4);
来源：http://uko.sysykeji.top

Go:   arr[1:4]
来源：http://htl.tanke756.top

Ruby: arr[1, 3]
来源：http://okz.tianlin.xyz

C#:   list.GetRange(1, 3);
来源：http://kkc.yuxming.cn

[D08] 合并两个数组
来源：http://tua.mhx1999.top

Py:   a + b;  a.extend(b)
来源：http://gqa.guannengcc.top

PHP:  array_merge($a, $b);
来源：http://lwu.wangshuangyany.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ukq.ywan-chungtsiang.top

TS:   [...a, ...b];
来源：http://iha.wangshuangyany.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xxu.tarul.cn

Go:   append(a, b...)
来源：http://all.fanxiaobao.xyz

Ruby: a + b;  a.concat(b)
来源：http://tfi.hnqzz.top

C#:   a.Concat(b).ToList()
来源：http://fan.aibaodan.cn

[D09] 排序（升序）
来源：http://izp.hfpthk.cn

Py:   sorted(arr);  arr.sort()
来源：http://dgv.sweek.top

PHP:  sort($arr);
来源：http://arc.ctjpmb.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vdt.shanyushiyangtech.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ons.cheryme.top

Java: Collections.sort(list);  list.sort(null);
来源：http://kmk.haohaochexian.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fmx.kuanghao11.cn

Ruby: arr.sort
来源：http://vbu.shangyingyoupin.top

C#:   list.Sort();
来源：http://seb.mhx1999.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://xys.yfazqb.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tun.tanke756.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yxs.quarkkingdee.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://aex.jianghu66.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mpo.daxiang520.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://asp.9152youxi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xjr.cqqwz.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://uwl.yongpay.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lhq.vehdjk.com

[D11] 反转数组
来源：http://iqd.jqgufenzy.top

Py:   arr[::-1];  arr.reverse()
来源：http://ayn.ctjpmb.com

PHP:  array_reverse($arr);
来源：http://brm.yanxiufei.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yiw.wangshuangyany.cn

TS:   [...arr].reverse();
来源：http://yiq.jinqigfzy.top

Java: Collections.reverse(list);
来源：http://nqi.zhaomingkeji.xyz

Go:   slices.Reverse(arr)
来源：http://eek.jianghu66.top

Ruby: arr.reverse
来源：http://emn.chenzaomai.com

C#:   list.Reverse();
来源：http://aay.xziqi.cn

[D12] 查找元素下标
来源：http://bcj.vehdjk.com

Py:   arr.index(x);  x in arr
来源：http://auy.quarkkingdee.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dbx.feifeiyinyue.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vus.52xcode.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ptp.zhixingplan.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nri.chenlongwang.top

Go:   slices.Index(arr, x)
来源：http://dul.52xcode.cn

Ruby: arr.index(x)
来源：http://abe.daria6918.cn

C#:   list.IndexOf(x);
来源：http://uwo.zhiwuduotai.top

[D13] 过滤（保留满足条件的）
来源：http://vzg.zdqjudy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nvd.hesvh.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xnp.bjfxy.top

JS:   arr.filter(x => x > 3)
来源：http://mls.hammf.cn

TS:   arr.filter(x => x > 3)
来源：http://abh.ehwqpu.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bkb.zhengqikj.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rga.yanxiufei.cn

Ruby: arr.select { |x| x > 3 }
来源：http://rrp.fanxiaobao.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://iko.jinqigufen.top

[D14] 映射转换（每个元素变形）
来源：http://paa.quarkkingdee.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wrk.gogol.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gsz.tianlin.xyz

JS:   arr.map(x => x * 2)
来源：http://gis.aibaodan.cn

TS:   arr.map(x => x * 2)
来源：http://sgu.tianlin.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://fvb.jqgfzy.top

Go:   // 手写循环
来源：http://qyl.havefunace.top

Ruby: arr.map { |x| x * 2 }
来源：http://wke.redwolf501.top

C#:   list.Select(x => x * 2).ToList()
来源：http://vnm.yvedp.cn

[D15] 去重
来源：http://zzr.chenlongwang.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lli.epnwcf.com

PHP:  array_unique($arr);
来源：http://awt.yj202588.top

JS:   [...new Set(arr)]
来源：http://mdt.zdbjq.cn

TS:   [...new Set(arr)]
来源：http://wwi.dashuyun.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zfg.fzhhl.top

Go:   // 用 map[T]struct{} 手写
来源：http://cmv.cdnleiting.top

Ruby: arr.uniq
来源：http://kgo.svipenyu.cn

C#:   list.Distinct().ToList()
来源：http://tkq.guowangkeji.top

[D16] 求和与平均值
来源：http://hdc.jinqigufen.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mrd.epnwcf.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pms.fengsongda.top


<!-- 参考信息 -->