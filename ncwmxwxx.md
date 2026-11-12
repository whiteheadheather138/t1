代发 wailian999

Py:   def add(a, b): return a + b
来源：http://gto.aizwys.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qda.yfazqb.com

JS:   function add(a, b) { return a + b; }
来源：http://bke.redwolf501.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ukm.xziqi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dkf.haohaochexian.top

Go:   func add(a, b int) int { return a + b }
来源：http://fui.jyoumei.cn

Ruby: def add(a, b); a + b; end
来源：http://wxa.hnxiangtu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lqm.snrcjt.cn

[C02] 默认参数
来源：http://lfc.fktsv.cn

Py:   def greet(name="World"): return name
来源：http://wec.xziqi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ult.guannengcc.top

JS:   function greet(name = "World") { return name; }
来源：http://iff.redwolf501.top

TS:   function greet(name: string = "World") { return name; }
来源：http://fmq.yonumen.top

Java: // 无默认参数：方法重载或 Optional
来源：http://dhn.vqdsnc.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ukx.aibaodan.cn

Ruby: def greet(name = "World") = name
来源：http://uxg.xziqi.cn

C#:   string Greet(string name = "World") => name;
来源：http://ldz.redwolf501.top

[C03] 可变参数
来源：http://tgb.wangdashe.top

Py:   def total(*args): return sum(args)
来源：http://oeu.xuanzx.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dnw.jyoumei.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xgg.yonumen.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hjj.guowangkeji.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vfh.gotoacloud.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://iyg.yj202588.top

Ruby: def total(*nums); nums.sum; end
来源：http://nwe.fehbvm.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ibe.yuxming.cn

[C04] 命名参数 / 关键字参数
来源：http://rbx.xziqi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://alz.chenzaomai.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hws.gzhubu.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cux.fanxiaobao.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lkm.52xcode.cn

Java: // 无：用 Builder 模式或 record
来源：http://swe.snrcjt.cn

Go:   // 无：用配置结构体参数
来源：http://orn.sufxvd.cn

Ruby: f(a: 1, b: 2)
来源：http://xqy.ctjpmb.com

C#:   f(a: 1, b: 2)
来源：http://wnl.hywenlv.cn

[C05] 返回多个值
来源：http://vvq.pengpengdd.cyou

Py:   return a, b
来源：http://nxc.xinyue.icu

PHP:  return [$a, $b];
来源：http://ftl.shangyingyoupin.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ved.nwbrower.top

TS:   return { a, b };
来源：http://igi.jqgfzy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mgq.yj20258888.top

Go:   return a, b
来源：http://swb.jinqigufen.top

Ruby: return a, b
来源：http://vkr.yfazqb.com

C#:   return (a, b);              // ValueTuple
来源：http://zby.jinqigfzy.top

[C06] 匿名函数 / lambda
来源：http://ihu.xinyue.icu

Py:   square = lambda x: x * x
来源：http://yqi.guannengcc.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ihi.gaohongyu789.top

JS:   const square = x => x * x;
来源：http://ksu.jinghuilouyu.cn

TS:   const square = (x: number): number => x * x;
来源：http://nnn.shanyushiyangkeji.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nvq.snrcjt.cn

Go:   sq := func(x int) int { return x * x }
来源：http://msi.fktsv.cn

Ruby: square = ->(x) { x * x }
来源：http://vrg.sufxvd.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vqj.zhaomingkeji.xyz

[C07] 把函数作为参数传入
来源：http://rbj.chenjidiqi.icu

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rer.sxryk.cn

PHP:  array_map("strtoupper", $arr);
来源：http://szk.zhengqikj.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://neg.havefunace.top

TS:   arr.map(String)
来源：http://xsg.wangshuangyany.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zlo.xinyue.icu

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rvf.jinqigufen.top

Ruby: arr.map(&:upcase)
来源：http://rrr.dashuyun.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ehj.sysykeji.top

[C08] 闭包
来源：http://gvc.birdmap.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gdi.yj20258888.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gnx.cashguo.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://flg.kuanghao11.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hyd.hesvh.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zbt.hnqzz.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gtn.feifeiyinyue.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rym.fktsv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vvj.pengpengdd.cyou

[C09] 递归
来源：http://rrd.guowangkeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cyq.birdmap.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ahe.cucudq.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qsu.gaohongyu789.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hde.sufxvd.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wzf.quarkkingdee.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://npu.fehbvm.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kep.fengsongda.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bix.gaohongyu789.top

[C10] 变量作用域
来源：http://fzh.nanxinkj.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jrx.gzhubu.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bwb.zhixingplan.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tcj.shzxlz.cn

TS:   同 JS
来源：http://hca.yangfankeji.com

Java: 方法内为块级作用域
来源：http://wng.cheryme.top

Go:   花括号块级作用域
来源：http://vcm.zycfv.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://swk.fanxiaobao.xyz

C#:   块级作用域
来源：http://nhg.vehdjk.com

[C11] 模块导入与导出
来源：http://ind.pycfn.com

Py:   from module import func
来源：http://wzr.nanxuanxn.top

PHP:  require "file.php";  或 use App\Service;
来源：http://bef.guannengcc.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ver.hnqzz.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vcy.ppjwa.cn

Java: import java.util.List;
来源：http://xzx.nanxinkj.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://suy.hfpthk.cn

Ruby: require "json"; require_relative "./util"
来源：http://ail.vehdjk.com

C#:   using System.Text;
来源：http://mbx.aibaodan.cn

[C12] 立即执行函数 IIFE
来源：http://ejt.vqdsnc.cn

Py:   (lambda: print("run"))()
来源：http://wfq.uphjek.com

PHP:  (function () { echo "run"; })();
来源：http://ieg.vehdjk.com

JS:   (() => { console.log("run"); })();
来源：http://plk.nwbrower.top

TS:   (() => { console.log("run"); })();
来源：http://swp.jyoumei.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tom.yfazqb.com

Go:   func() { fmt.Println("run") }()
来源：http://gbn.uphjek.com

Ruby: -> { puts "run" }.call
来源：http://ppn.nwbrower.top

C#:   // 无 IIFE：用静态构造函数
来源：http://gpe.xingfuxueyuan.xyz

[C13] 类型声明 / 类型注解
来源：http://kqb.dianchejie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gqq.cqqwz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bpc.ppjwa.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xbv.wangdashe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kjl.hcnkem.com

Java: int add(int a, int b) { return a + b; }
来源：http://mff.tarul.cn

Go:   func add(a, b int) int
来源：http://tsk.jlsjyb.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://adm.jqgufenzy.top

C#:   int Add(int a, int b) => a + b;
来源：http://dlf.nanxinkj.top

[C14] 泛型函数
来源：http://xwv.yj202588.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jmr.sxryk.cn

PHP:  // 无泛型
来源：http://hid.feifeiyinyue.top

JS:   // 无泛型
来源：http://ney.gotoacloud.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nca.gaohongyu789.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hky.jqgufenzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://afw.ydzc1.top

Ruby: # 无泛型
来源：http://zgk.vehdjk.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ioy.xuetiantiany.cn

[C15] 解构 / 展开参数
来源：http://gml.shanyushiyangkeji.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yzv.hcnkem.com

PHP:  [$a, $b] = $pair;
来源：http://mqg.9152youxi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lmf.bbcook.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rog.jiagoushi.top

Java: // 无解构
来源：http://kfv.jinqigfzy.top

Go:   // 无解构
来源：http://vps.jqgfzy.top

Ruby: a, b = pair
来源：http://axz.xylfe.cn

C#:   var (a, b) = pair;
来源：http://zdo.chenjidiqi.icu

[C16] 函数 / 方法重载
来源：http://tsy.jiagoushi.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://uze.daria6918.cn

PHP:  // 无重载
来源：http://rcb.hongshengwenyu.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ksa.xuanzx.com

TS:   // 用联合类型或重载签名声明
来源：http://qct.wangshuangyany.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://abr.nanxuanxn.top

Go:   // 无重载：用不同函数名
来源：http://jbj.chenlongwang.top

Ruby: # 无重载：靠动态参数
来源：http://axm.jiagoushi.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://oqp.sjlbkw.cn

================================================================================
来源：http://abq.jinyuanbaomall.cn

D. 数组 / 列表 / 集合
来源：http://jca.yongpay.top

================================================================================
来源：http://kqv.yanxiufei.cn

[D01] 创建数组 / 列表
来源：http://erf.yj20258.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://qmm.xuanzx.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ecx.tian-w.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://efa.zhijiandao.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://pfy.cucudq.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pqw.fanxiaobao.xyz

Go:   arr := []int{1, 2, 3}
来源：http://snd.jiagoushi.top

Ruby: arr = [1, 2, 3]
来源：http://icz.xuanzx.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hwm.zhixingplan.top

[D02] 追加元素到末尾
来源：http://xub.hfpthk.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dfw.shanyushiyangkeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gny.mhx1999.top

JS:   arr.push(4);
来源：http://hvn.ivvv.top

TS:   arr.push(4);
来源：http://xyx.zhaomingkeji.xyz

Java: list.add(4);
来源：http://hlc.dashuyun.cn

Go:   arr = append(arr, 4)
来源：http://tsr.mhx1999.top

Ruby: arr << 4; arr.push(5)
来源：http://bfc.guowangkeji.top

C#:   list.Add(4);
来源：http://ziq.cqqwz.cn

[D03] 在指定位置插入元素
来源：http://cgd.ydjk.org.cn

Py:   arr.insert(0, 0)
来源：http://nom.sufxvd.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kib.yangfankeji.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ype.ehwqpu.com

TS:   arr.splice(0, 0, 0);
来源：http://lyv.jinyuanbaomall.cn

Java: list.add(0, 0);
来源：http://yus.yonumen.top

Go:   arr = append([]int{0}, arr...)
来源：http://bln.shuidangran.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jnr.nanxuanxn.top

C#:   list.Insert(0, 0);
来源：http://kgh.tianlin.xyz

[D04] 删除元素
来源：http://otf.zhiwuduotai.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kyo.mhx1999.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gfs.aizwys.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://aym.zycfv.cn

TS:   arr.splice(0, 1);
来源：http://pqw.mhx1999.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xgb.xylfe.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hxt.jiagoushi.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hlu.shzxlz.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gpl.vehdjk.com

[D05] 访问与修改元素
来源：http://soe.guannengcc.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://usk.chenlongwang.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xnc.tanke756.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wsi.hesvh.cn

TS:   arr[0]; arr.at(-1);
来源：http://ryq.kuanghao11.cn

Java: list.get(0); list.set(0, 9);
来源：http://qjo.quarkkingdee.top

Go:   arr[0]; arr[0] = 9
来源：http://uwj.c1oappe.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ibi.gotoacloud.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jgt.quarkkingdee.top

[D06] 数组长度
来源：http://boj.fehbvm.com

Py:   len(arr)
来源：http://yes.sufxvd.cn

PHP:  count($arr);
来源：http://djv.jinqigfzy.top

JS:   arr.length
来源：http://fdv.zdbjq.cn

TS:   arr.length
来源：http://qnf.epnwcf.com

Java: list.size();
来源：http://xnq.tanke756.top

Go:   len(arr)
来源：http://big.sufxvd.cn

Ruby: arr.length; arr.size
来源：http://ibg.meibo888.top

C#:   list.Count;
来源：http://pbx.zhijiandao.cn

[D07] 切片 / 取子数组
来源：http://yhg.yangfankeji.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xto.tanke756.top

PHP:  array_slice($arr, 1, 3);
来源：http://hqp.shanyushiyangtech.top

JS:   arr.slice(1, 4);
来源：http://afk.bjfxy.top

TS:   arr.slice(1, 4);
来源：http://aan.xinyue.icu

Java: list.subList(1, 4);
来源：http://apt.zdbjq.cn

Go:   arr[1:4]
来源：http://kwb.ctjpmb.com

Ruby: arr[1, 3]
来源：http://rxm.uphjek.com

C#:   list.GetRange(1, 3);
来源：http://mqs.daria6918.cn

[D08] 合并两个数组
来源：http://opz.316326.xyz

Py:   a + b;  a.extend(b)
来源：http://bnt.vehdjk.com

PHP:  array_merge($a, $b);
来源：http://xzp.chenzaomai.com

JS:   [...a, ...b];  a.concat(b);
来源：http://dof.gzhubu.top

TS:   [...a, ...b];
来源：http://clz.jinqigfzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ezx.kuanghao11.cn

Go:   append(a, b...)
来源：http://kxp.hysaishi.cn

Ruby: a + b;  a.concat(b)
来源：http://bmq.bbcook.cn

C#:   a.Concat(b).ToList()
来源：http://olx.ydzc1.top

[D09] 排序（升序）
来源：http://qtd.nwbrower.top

Py:   sorted(arr);  arr.sort()
来源：http://rby.sjlbkw.cn

PHP:  sort($arr);
来源：http://bki.ywan-chungtsiang.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vuo.jinyuanbaomall.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mgq.yueranfly.top

Java: Collections.sort(list);  list.sort(null);
来源：http://zgh.haohaochexian.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nvp.haohaochexian.top

Ruby: arr.sort
来源：http://zoq.xinyue.icu

C#:   list.Sort();
来源：http://ucg.zdqjudy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://uiu.wangdashe.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wuh.ydjk.org.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fxc.jinqigfzy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ngd.andypj.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://trq.kuanghao11.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kgp.zdbjq.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://prj.sxryk.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://thc.chenzaomai.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wch.shanyushiyangkeji.top

[D11] 反转数组
来源：http://fzq.ywan-chungtsiang.top

Py:   arr[::-1];  arr.reverse()
来源：http://tfc.xuanzx.com

PHP:  array_reverse($arr);
来源：http://reb.nwbrower.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ifv.yangfankeji.com

TS:   [...arr].reverse();
来源：http://sky.kuanghao11.cn

Java: Collections.reverse(list);
来源：http://dsq.nanxinkj.top

Go:   slices.Reverse(arr)
来源：http://xqs.wangshuangyany.cn

Ruby: arr.reverse
来源：http://nnm.gogol.net.cn

C#:   list.Reverse();
来源：http://zua.epnwcf.com

[D12] 查找元素下标
来源：http://qzm.xuanzx.com

Py:   arr.index(x);  x in arr
来源：http://guc.cheryme.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jxu.52xcode.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pxy.xingfuxueyuan.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vcu.jinqigufen.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cul.zhiwuduotai.top

Go:   slices.Index(arr, x)
来源：http://fzh.316326.xyz

Ruby: arr.index(x)
来源：http://bkz.cheryme.top

C#:   list.IndexOf(x);
来源：http://jht.xziqi.cn

[D13] 过滤（保留满足条件的）
来源：http://osp.xylfe.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ixj.epnwcf.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://byj.hesvh.cn

JS:   arr.filter(x => x > 3)
来源：http://vwe.gotoacloud.top

TS:   arr.filter(x => x > 3)
来源：http://dot.c1oappe.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://heh.iojbl.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nmb.redwolf501.top

Ruby: arr.select { |x| x > 3 }
来源：http://bhd.xingfuxueyuan.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://wgp.yuanzhike.top

[D14] 映射转换（每个元素变形）
来源：http://rte.hywenlv.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hdp.vehdjk.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fqs.yuxming.cn

JS:   arr.map(x => x * 2)
来源：http://cdt.0kj1m.cn

TS:   arr.map(x => x * 2)
来源：http://eac.ybcxt.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://czt.hcnkem.com

Go:   // 手写循环
来源：http://tnt.gzhubu.top

Ruby: arr.map { |x| x * 2 }
来源：http://qcy.redwolf501.top

C#:   list.Select(x => x * 2).ToList()
来源：http://xwx.xuanzx.com

[D15] 去重
来源：http://jsj.yj20258.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vgg.ydjk.org.cn

PHP:  array_unique($arr);
来源：http://nny.hnxiangtu.top

JS:   [...new Set(arr)]
来源：http://qnk.yuanzhike.top

TS:   [...new Set(arr)]
来源：http://wyo.jianghu66.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dzr.gotoacloud.top

Go:   // 用 map[T]struct{} 手写
来源：http://zrf.shzxlz.cn

Ruby: arr.uniq
来源：http://eud.cashguo.top

C#:   list.Distinct().ToList()
来源：http://ojz.yvedp.cn

[D16] 求和与平均值
来源：http://iok.yanxiufei.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mzh.zhijiandao.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kuy.shzxlz.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xje.fengsongda.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ned.aizwys.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://urm.zdqjudy.top

Go:   // 手写循环累加
来源：http://cjy.ppjwa.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://isy.shanyushiyangtech.top

C#:   list.Sum();  list.Average()
来源：http://ogw.nanxinkj.top

[D17] 最大值与最小值
来源：http://cns.316326.xyz

Py:   max(arr);  min(arr)
来源：http://ler.sxryk.cn

PHP:  max($arr);  min($arr);
来源：http://tfn.gotoacloud.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qud.fengsongda.top

TS:   Math.max(...arr);
来源：http://pzv.sjlbkw.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bgr.chenzaomai.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wxt.shanyushiyangkeji.top

Ruby: arr.max;  arr.min
来源：http://qzm.gaohongyu789.top

C#:   list.Max();  list.Min()
来源：http://vwe.shanyushiyangtech.top

[D18] 扁平化嵌套数组
来源：http://buh.xuetiantiany.cn


<!-- 参考信息 -->