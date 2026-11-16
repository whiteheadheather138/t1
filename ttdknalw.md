代发 wailian999

================================================================================
来源：http://jfq.gaohongyu789.top

C. 函数与作用域
来源：http://sip.guowangkeji.top

================================================================================
来源：http://bsc.yueranfly.top

[C01] 定义函数
来源：http://hxy.tanke756.top

Py:   def add(a, b): return a + b
来源：http://col.shangyingyoupin.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vub.yj20258888.top

JS:   function add(a, b) { return a + b; }
来源：http://fwn.aizwys.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jzp.daxiang520.top

Java: static int add(int a, int b) { return a + b; }
来源：http://jsf.yfazqb.com

Go:   func add(a, b int) int { return a + b }
来源：http://hjr.mhx1999.top

Ruby: def add(a, b); a + b; end
来源：http://rcx.zdbjq.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://quc.ydzc1.top

[C02] 默认参数
来源：http://eaq.zhongyouzk.top

Py:   def greet(name="World"): return name
来源：http://scu.fanxiaobao.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://zih.0kj1m.cn

JS:   function greet(name = "World") { return name; }
来源：http://wkv.jinyuanbaomall.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fjb.daria6918.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dav.sysykeji.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nrz.yonumen.top

Ruby: def greet(name = "World") = name
来源：http://cva.hongshengwenyu.top

C#:   string Greet(string name = "World") => name;
来源：http://tmu.hfpthk.cn

[C03] 可变参数
来源：http://rlo.c1oappe.top

Py:   def total(*args): return sum(args)
来源：http://gqh.xinyue.icu

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nqc.9152youxi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wbt.yongpay.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wes.tarul.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bmd.tian-w.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yxv.zhiwuduotai.top

Ruby: def total(*nums); nums.sum; end
来源：http://pmp.c1oappe.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hsg.pycfn.com

[C04] 命名参数 / 关键字参数
来源：http://kmo.fzhhl.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wrf.cashguo.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://oyf.feifeiyinyue.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bwr.iojbl.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qdr.nanxuanxn.top

Java: // 无：用 Builder 模式或 record
来源：http://ryu.shuidangran.top

Go:   // 无：用配置结构体参数
来源：http://igj.guowangkeji.top

Ruby: f(a: 1, b: 2)
来源：http://ozk.shzxlz.cn

C#:   f(a: 1, b: 2)
来源：http://pha.jqgfzy.top

[C05] 返回多个值
来源：http://byw.shangyingyoupin.top

Py:   return a, b
来源：http://zqi.jiagoushi.top

PHP:  return [$a, $b];
来源：http://abm.iojbl.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://and.fanxiaobao.xyz

TS:   return { a, b };
来源：http://itb.hcnkem.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vkh.yueranfly.top

Go:   return a, b
来源：http://pvf.hongshengwenyu.top

Ruby: return a, b
来源：http://icy.pycfn.com

C#:   return (a, b);              // ValueTuple
来源：http://hrd.shzxlz.cn

[C06] 匿名函数 / lambda
来源：http://kcr.zdqjudy.top

Py:   square = lambda x: x * x
来源：http://vsi.yvedp.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://nim.tianlin.xyz

JS:   const square = x => x * x;
来源：http://iiq.havefunace.top

TS:   const square = (x: number): number => x * x;
来源：http://msy.jiagoushi.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bnl.316326.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://dpc.yonumen.top

Ruby: square = ->(x) { x * x }
来源：http://ckf.fanxiaobao.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://tzv.hesvh.cn

[C07] 把函数作为参数传入
来源：http://qrv.yanxiufei.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pxo.hongshengwenyu.top

PHP:  array_map("strtoupper", $arr);
来源：http://cnm.zhijiandao.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xzp.yongpay.top

TS:   arr.map(String)
来源：http://omd.jinghuilouyu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://csx.sweek.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qes.uphjek.com

Ruby: arr.map(&:upcase)
来源：http://jwc.haohaochexian.top

C#:   arr.Select(s => s.ToUpper())
来源：http://aph.xylfe.cn

[C08] 闭包
来源：http://dik.cdnleiting.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://azq.yvedp.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://req.uphjek.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vlu.chenjidiqi.icu

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://crj.xinyue.icu

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vwt.sysykeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yhc.pycfn.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://etk.wangshuangyany.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ulf.jlsjyb.cn

[C09] 递归
来源：http://dfp.ehwqpu.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://itx.yj20258888.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://oiq.aizwys.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://byk.sysykeji.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ovk.xylfe.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lqp.sysykeji.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qxf.jinyuanbaomall.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xlv.quarkkingdee.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tkj.ppjwa.cn

[C10] 变量作用域
来源：http://kxq.ydzc1.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://har.shangyingyoupin.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vaj.jinyuanbaomall.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hcb.zhengqikj.top

TS:   同 JS
来源：http://bfa.fengsongda.top

Java: 方法内为块级作用域
来源：http://wrs.xuanzx.com

Go:   花括号块级作用域
来源：http://pul.bbcook.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://oyw.xuanzx.com

C#:   块级作用域
来源：http://blr.nwbrower.top

[C11] 模块导入与导出
来源：http://hyc.sweek.top

Py:   from module import func
来源：http://sva.gaohongyu789.top

PHP:  require "file.php";  或 use App\Service;
来源：http://gae.tanke756.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://bdl.aizwys.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nvi.dianchejie.cn

Java: import java.util.List;
来源：http://ezt.ivvv.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://eyx.hywenlv.cn

Ruby: require "json"; require_relative "./util"
来源：http://vzv.feifeiyinyue.top

C#:   using System.Text;
来源：http://nfr.jinqigufen.top

[C12] 立即执行函数 IIFE
来源：http://gnc.tian-w.cn

Py:   (lambda: print("run"))()
来源：http://yfy.xingfuxueyuan.xyz

PHP:  (function () { echo "run"; })();
来源：http://byi.hongshengwenyu.top

JS:   (() => { console.log("run"); })();
来源：http://qgf.zhiwuduotai.top

TS:   (() => { console.log("run"); })();
来源：http://ene.zhengqikj.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ypt.9152youxi.cn

Go:   func() { fmt.Println("run") }()
来源：http://rik.xuanzx.com

Ruby: -> { puts "run" }.call
来源：http://pem.zhoulong.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://ikq.wangdashe.top

[C13] 类型声明 / 类型注解
来源：http://svp.yj20258888.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yvw.iojbl.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lte.9152youxi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xkr.ehwqpu.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mut.tarul.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cny.jyoumei.cn

Go:   func add(a, b int) int
来源：http://tae.yueranfly.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sjw.hnqzz.top

C#:   int Add(int a, int b) => a + b;
来源：http://cyk.zdqjudy.top

[C14] 泛型函数
来源：http://tsy.shzxlz.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qob.zycfv.cn

PHP:  // 无泛型
来源：http://mji.redwolf501.top

JS:   // 无泛型
来源：http://ryk.xingfuxueyuan.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://btv.zdqjudy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tvl.cucudq.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qqj.cucudq.cn

Ruby: # 无泛型
来源：http://bch.aibaodan.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://buc.ehwqpu.com

[C15] 解构 / 展开参数
来源：http://gbs.svipenyu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qrp.zdqjudy.top

PHP:  [$a, $b] = $pair;
来源：http://izv.shangyingyoupin.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mqu.yvedp.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rzi.sjlbkw.cn

Java: // 无解构
来源：http://duf.jinghuilouyu.cn

Go:   // 无解构
来源：http://zgk.shanyushiyangtech.top

Ruby: a, b = pair
来源：http://rij.yongpay.top

C#:   var (a, b) = pair;
来源：http://oed.cqqwz.cn

[C16] 函数 / 方法重载
来源：http://izm.smart0.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://azw.hammf.cn

PHP:  // 无重载
来源：http://nae.xylfe.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://mio.zhijiandao.cn

TS:   // 用联合类型或重载签名声明
来源：http://sbu.hfpthk.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://kwe.daria6918.cn

Go:   // 无重载：用不同函数名
来源：http://nvc.52xcode.cn

Ruby: # 无重载：靠动态参数
来源：http://rfz.ywan-chungtsiang.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://nes.ybcxt.top

================================================================================
来源：http://wek.havefunace.top

D. 数组 / 列表 / 集合
来源：http://vvj.tanke756.top

================================================================================
来源：http://oor.sweek.top

[D01] 创建数组 / 列表
来源：http://bub.shzxlz.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fvh.fanxiaobao.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kjr.guowangkeji.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wma.hysaishi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ikx.yonumen.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ujn.yongpay.top

Go:   arr := []int{1, 2, 3}
来源：http://gbi.xylfe.cn

Ruby: arr = [1, 2, 3]
来源：http://kfh.9152youxi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zli.cheryme.top

[D02] 追加元素到末尾
来源：http://jvb.zdqjudy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lkj.vqdsnc.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://aoz.zhaomingkeji.xyz

JS:   arr.push(4);
来源：http://zrb.fanxiaobao.xyz

TS:   arr.push(4);
来源：http://ovs.jyoumei.cn

Java: list.add(4);
来源：http://fmt.zhoulong.xyz

Go:   arr = append(arr, 4)
来源：http://vko.yonumen.top

Ruby: arr << 4; arr.push(5)
来源：http://uhg.9152youxi.cn

C#:   list.Add(4);
来源：http://pzh.sufxvd.cn

[D03] 在指定位置插入元素
来源：http://mlt.dianchejie.cn

Py:   arr.insert(0, 0)
来源：http://npu.wangdashe.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hlq.xuetiantiany.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mit.xuetiantiany.cn

TS:   arr.splice(0, 0, 0);
来源：http://ryk.havefunace.top

Java: list.add(0, 0);
来源：http://myw.snrcjt.cn

Go:   arr = append([]int{0}, arr...)
来源：http://elm.ydjk.org.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://aui.tianlin.xyz

C#:   list.Insert(0, 0);
来源：http://jtj.sweek.top

[D04] 删除元素
来源：http://ean.tianlin.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bju.yangfankeji.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://edi.hysaishi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vff.sxryk.cn

TS:   arr.splice(0, 1);
来源：http://odv.epnwcf.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vyh.jianghu66.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mtv.epnwcf.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qpr.tian-w.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mhg.yuxming.cn

[D05] 访问与修改元素
来源：http://cvw.jinqigufen.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://veb.yueranfly.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ppo.yvedp.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zgi.jinqigfzy.top

TS:   arr[0]; arr.at(-1);
来源：http://mkg.svipenyu.cn

Java: list.get(0); list.set(0, 9);
来源：http://aop.jiagoushi.top

Go:   arr[0]; arr[0] = 9
来源：http://tqw.sweek.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://teo.ivvv.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://eqy.snrcjt.cn

[D06] 数组长度
来源：http://miq.cucudq.cn

Py:   len(arr)
来源：http://exd.sweek.top

PHP:  count($arr);
来源：http://bsg.yj20258888.top

JS:   arr.length
来源：http://oyr.smart0.xyz

TS:   arr.length
来源：http://rir.hammf.cn

Java: list.size();
来源：http://tuu.zhijiandao.cn

Go:   len(arr)
来源：http://vqw.gzhubu.top

Ruby: arr.length; arr.size
来源：http://pof.zycfv.cn

C#:   list.Count;
来源：http://mgj.xuanzx.com

[D07] 切片 / 取子数组
来源：http://foo.tanke756.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://liu.ywan-chungtsiang.top

PHP:  array_slice($arr, 1, 3);
来源：http://djf.pycfn.com

JS:   arr.slice(1, 4);
来源：http://ffc.jinqigfzy.top

TS:   arr.slice(1, 4);
来源：http://fxv.gaohongyu789.top

Java: list.subList(1, 4);
来源：http://oex.sysykeji.top

Go:   arr[1:4]
来源：http://whz.xuetiantiany.cn

Ruby: arr[1, 3]
来源：http://ddo.xziqi.cn

C#:   list.GetRange(1, 3);
来源：http://loi.zhoulong.xyz

[D08] 合并两个数组
来源：http://wio.epnwcf.com

Py:   a + b;  a.extend(b)
来源：http://mto.epnwcf.com

PHP:  array_merge($a, $b);
来源：http://jfo.hfpthk.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://oie.xuanzx.com

TS:   [...a, ...b];
来源：http://qhz.hnxiangtu.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gmg.yj20258888.top

Go:   append(a, b...)
来源：http://upo.jqgufenzy.top

Ruby: a + b;  a.concat(b)
来源：http://wuj.gogol.net.cn

C#:   a.Concat(b).ToList()
来源：http://rxa.hcnkem.com

[D09] 排序（升序）
来源：http://apj.uphjek.com

Py:   sorted(arr);  arr.sort()
来源：http://oya.snrcjt.cn

PHP:  sort($arr);
来源：http://ejw.yvedp.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cxk.daxiang520.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://vby.hesvh.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://fgk.zhaomingkeji.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://etb.haohaochexian.top

Ruby: arr.sort
来源：http://eys.wangdashe.top

C#:   list.Sort();
来源：http://anq.zhixingplan.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://mws.bbcook.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://skd.kuanghao11.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oul.zhoulong.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lge.c1oappe.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dlm.cucudq.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yqz.pengpengdd.cyou

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ihf.yongpay.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://brq.hammf.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jdw.hysaishi.cn

[D11] 反转数组
来源：http://zxw.quarkkingdee.top

Py:   arr[::-1];  arr.reverse()
来源：http://bij.yj20258.top

PHP:  array_reverse($arr);
来源：http://pti.dianchejie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pwo.sxryk.cn

TS:   [...arr].reverse();
来源：http://cfe.meibo888.top

Java: Collections.reverse(list);
来源：http://ycz.sjlbkw.cn

Go:   slices.Reverse(arr)
来源：http://qds.jiagoushi.top

Ruby: arr.reverse
来源：http://cvd.havefunace.top

C#:   list.Reverse();
来源：http://yzs.meibo888.top

[D12] 查找元素下标
来源：http://nny.shangyingyoupin.top

Py:   arr.index(x);  x in arr
来源：http://osv.zdbjq.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://szi.xziqi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ogp.ppjwa.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rav.wangshuangyany.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gbp.gogol.net.cn

Go:   slices.Index(arr, x)
来源：http://gmi.hysaishi.cn

Ruby: arr.index(x)
来源：http://hwu.hfpthk.cn

C#:   list.IndexOf(x);
来源：http://etw.jqgfzy.top

[D13] 过滤（保留满足条件的）
来源：http://nkt.hongshengwenyu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nci.ydjk.org.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fxx.shuidangran.top

JS:   arr.filter(x => x > 3)
来源：http://cni.daxiang520.top

TS:   arr.filter(x => x > 3)
来源：http://kak.kuanghao11.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://svc.zhaomingkeji.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://eyx.zdqjudy.top

Ruby: arr.select { |x| x > 3 }
来源：http://sqg.sysykeji.top

C#:   list.Where(x => x > 3).ToList()
来源：http://bsw.hnxiangtu.top

[D14] 映射转换（每个元素变形）
来源：http://moj.tanke756.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://epj.bbcook.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uul.zhoulong.xyz

JS:   arr.map(x => x * 2)
来源：http://xja.guannengcc.top

TS:   arr.map(x => x * 2)
来源：http://prw.feifeiyinyue.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://lqx.hnxiangtu.top

Go:   // 手写循环
来源：http://cvs.havefunace.top

Ruby: arr.map { |x| x * 2 }
来源：http://lsk.316326.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://ffk.hesvh.cn

[D15] 去重
来源：http://prx.quarkkingdee.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hht.zycfv.cn

PHP:  array_unique($arr);
来源：http://ndc.zdqjudy.top

JS:   [...new Set(arr)]
来源：http://dqm.xinyue.icu

TS:   [...new Set(arr)]
来源：http://xmo.uphjek.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nqf.chenzaomai.com

Go:   // 用 map[T]struct{} 手写
来源：http://ghz.zhaomingkeji.xyz

Ruby: arr.uniq
来源：http://cjh.ydzc1.top

C#:   list.Distinct().ToList()
来源：http://nha.birdmap.top

[D16] 求和与平均值
来源：http://lww.wangshuangyany.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gxg.zhongyouzk.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rcj.ctjpmb.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://anx.uphjek.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yxc.nwbrower.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rzi.shuidangran.top

Go:   // 手写循环累加
来源：http://iik.redwolf501.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vdp.dianchejie.cn

C#:   list.Sum();  list.Average()
来源：http://vxv.hfpthk.cn

[D17] 最大值与最小值
来源：http://kiw.hammf.cn

Py:   max(arr);  min(arr)
来源：http://fwy.chenjidiqi.icu

PHP:  max($arr);  min($arr);
来源：http://hbm.iojbl.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xri.sjlbkw.cn

TS:   Math.max(...arr);
来源：http://taw.zdqjudy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://nnh.vqdsnc.cn


<!-- 参考信息 -->