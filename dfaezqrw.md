代发 wailian999

[C02] 默认参数
来源：http://gbi.dianchejie.cn

Py:   def greet(name="World"): return name
来源：http://pbj.fzhhl.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ctc.iojbl.cn

JS:   function greet(name = "World") { return name; }
来源：http://xps.yueranfly.top

TS:   function greet(name: string = "World") { return name; }
来源：http://bcs.birdmap.top

Java: // 无默认参数：方法重载或 Optional
来源：http://xwt.kuanghao11.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kni.ehwqpu.com

Ruby: def greet(name = "World") = name
来源：http://scz.haohaochexian.top

C#:   string Greet(string name = "World") => name;
来源：http://zfg.nwbrower.top

[C03] 可变参数
来源：http://odj.gaohongyu789.top

Py:   def total(*args): return sum(args)
来源：http://jca.chenlongwang.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sif.jqgfzy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bli.guannengcc.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tku.gogol.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bbj.chenzaomai.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wsu.daxiang520.top

Ruby: def total(*nums); nums.sum; end
来源：http://hhq.jlsjyb.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sdl.zhaomingkeji.xyz

[C04] 命名参数 / 关键字参数
来源：http://azm.birdmap.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jrk.gotoacloud.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tuv.shanyushiyangkeji.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://exu.fanxiaobao.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://buz.zhixingplan.top

Java: // 无：用 Builder 模式或 record
来源：http://wvv.yvedp.cn

Go:   // 无：用配置结构体参数
来源：http://qnt.shanyushiyangtech.top

Ruby: f(a: 1, b: 2)
来源：http://pxk.ehwqpu.com

C#:   f(a: 1, b: 2)
来源：http://krj.havefunace.top

[C05] 返回多个值
来源：http://tdg.xingfuxueyuan.xyz

Py:   return a, b
来源：http://zdj.hywenlv.cn

PHP:  return [$a, $b];
来源：http://lde.jinqigufen.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://pxc.0kj1m.cn

TS:   return { a, b };
来源：http://sfv.sufxvd.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pum.mhx1999.top

Go:   return a, b
来源：http://krj.xylfe.cn

Ruby: return a, b
来源：http://gua.xingfuxueyuan.xyz

C#:   return (a, b);              // ValueTuple
来源：http://rdx.yangfankeji.com

[C06] 匿名函数 / lambda
来源：http://kun.zhiwuduotai.top

Py:   square = lambda x: x * x
来源：http://dph.sufxvd.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://euc.feifeiyinyue.top

JS:   const square = x => x * x;
来源：http://zdh.wangshuangyany.cn

TS:   const square = (x: number): number => x * x;
来源：http://okp.guowangkeji.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zrq.zdqjudy.top

Go:   sq := func(x int) int { return x * x }
来源：http://mtn.wangshuangyany.cn

Ruby: square = ->(x) { x * x }
来源：http://lhi.yuanzhike.top

C#:   Func<int, int> square = x => x * x;
来源：http://pqq.yj20258.top

[C07] 把函数作为参数传入
来源：http://hwe.bbcook.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rzp.zhijiandao.cn

PHP:  array_map("strtoupper", $arr);
来源：http://uff.52xcode.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gyg.smart0.xyz

TS:   arr.map(String)
来源：http://ikf.chenjidiqi.icu

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xli.zdbjq.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://flp.sysykeji.top

Ruby: arr.map(&:upcase)
来源：http://dbr.52xcode.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cxi.shanyushiyangtech.top

[C08] 闭包
来源：http://jlt.tian-w.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nlf.feifeiyinyue.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jlw.kuanghao11.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mrz.zycfv.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://odi.shuidangran.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ojk.0kj1m.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jrb.yj202588.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dei.hammf.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bbn.sysykeji.top

[C09] 递归
来源：http://qnw.dianchejie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mfo.fehbvm.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://saz.gogol.net.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yeh.sjlbkw.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sxm.zhaomingkeji.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jky.fanxiaobao.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://utu.sufxvd.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://apz.yj20258888.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jhp.birdmap.top

[C10] 变量作用域
来源：http://yfm.xuanzx.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kdr.xingfuxueyuan.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mxq.xziqi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pgz.yuanzhike.top

TS:   同 JS
来源：http://fjf.andypj.xyz

Java: 方法内为块级作用域
来源：http://rmg.daxiang520.top

Go:   花括号块级作用域
来源：http://nke.52xcode.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://soh.cucudq.cn

C#:   块级作用域
来源：http://ilr.fktsv.cn

[C11] 模块导入与导出
来源：http://ugu.ydjk.org.cn

Py:   from module import func
来源：http://npv.jlsjyb.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://cao.gaohongyu789.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://znp.tanke756.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jaq.havefunace.top

Java: import java.util.List;
来源：http://wdz.mhx1999.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zpr.fehbvm.com

Ruby: require "json"; require_relative "./util"
来源：http://mjq.xinyue.icu

C#:   using System.Text;
来源：http://kcp.chenzaomai.com

[C12] 立即执行函数 IIFE
来源：http://jrj.havefunace.top

Py:   (lambda: print("run"))()
来源：http://rel.gotoacloud.top

PHP:  (function () { echo "run"; })();
来源：http://idq.tianlin.xyz

JS:   (() => { console.log("run"); })();
来源：http://xwu.jinyuanbaomall.cn

TS:   (() => { console.log("run"); })();
来源：http://qtj.ydjk.org.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zmt.pycfn.com

Go:   func() { fmt.Println("run") }()
来源：http://rcb.pengpengdd.cyou

Ruby: -> { puts "run" }.call
来源：http://rci.haohaochexian.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ffk.fengsongda.top

[C13] 类型声明 / 类型注解
来源：http://uhl.zdqjudy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gut.yanxiufei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wcm.hammf.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qup.wangdashe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mxa.yangfankeji.com

Java: int add(int a, int b) { return a + b; }
来源：http://sls.hnqzz.top

Go:   func add(a, b int) int
来源：http://uwp.ehwqpu.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mpq.cucudq.cn

C#:   int Add(int a, int b) => a + b;
来源：http://rhn.iojbl.cn

[C14] 泛型函数
来源：http://lak.yanxiufei.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yeo.jinghuilouyu.cn

PHP:  // 无泛型
来源：http://idu.cdnleiting.top

JS:   // 无泛型
来源：http://wno.vehdjk.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://oda.sweek.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ugq.nanxinkj.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://swc.sweek.top

Ruby: # 无泛型
来源：http://dcw.quarkkingdee.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xou.guannengcc.top

[C15] 解构 / 展开参数
来源：http://qpf.hnqzz.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yfo.fzhhl.top

PHP:  [$a, $b] = $pair;
来源：http://xpo.ydjk.org.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fhf.yongpay.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qmb.shanyushiyangkeji.top

Java: // 无解构
来源：http://jrx.aibaodan.cn

Go:   // 无解构
来源：http://odv.sweek.top

Ruby: a, b = pair
来源：http://szs.snrcjt.cn

C#:   var (a, b) = pair;
来源：http://svk.jianghu66.top

[C16] 函数 / 方法重载
来源：http://cwg.nwbrower.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xly.ctjpmb.com

PHP:  // 无重载
来源：http://apo.gogol.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zgh.tian-w.cn

TS:   // 用联合类型或重载签名声明
来源：http://dxd.ctjpmb.com

Java: void f(int a) {}  void f(String a) {}
来源：http://brw.havefunace.top

Go:   // 无重载：用不同函数名
来源：http://ybj.c1oappe.top

Ruby: # 无重载：靠动态参数
来源：http://cqq.iojbl.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qjw.zhongyouzk.top

================================================================================
来源：http://dxv.snrcjt.cn

D. 数组 / 列表 / 集合
来源：http://dgz.guowangkeji.top

================================================================================
来源：http://epj.hfpthk.cn

[D01] 创建数组 / 列表
来源：http://gxx.chenlongwang.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://kow.52xcode.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ppp.xingfuxueyuan.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cha.yuanzhike.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://vwy.aizwys.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ddu.wangshuangyany.cn

Go:   arr := []int{1, 2, 3}
来源：http://whd.sxryk.cn

Ruby: arr = [1, 2, 3]
来源：http://ovh.jiagoushi.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yar.yj20258888.top

[D02] 追加元素到末尾
来源：http://emi.pycfn.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://eqs.zhaomingkeji.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xcv.fzhhl.top

JS:   arr.push(4);
来源：http://bvh.tian-w.cn

TS:   arr.push(4);
来源：http://tfa.zhaomingkeji.xyz

Java: list.add(4);
来源：http://tbh.tianlin.xyz

Go:   arr = append(arr, 4)
来源：http://xdf.uphjek.com

Ruby: arr << 4; arr.push(5)
来源：http://dtw.ppjwa.cn

C#:   list.Add(4);
来源：http://nbp.birdmap.top

[D03] 在指定位置插入元素
来源：http://ifz.jianghu66.top

Py:   arr.insert(0, 0)
来源：http://fxu.shanyushiyangkeji.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://glj.zycfv.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lth.jinghuilouyu.cn

TS:   arr.splice(0, 0, 0);
来源：http://wzp.epnwcf.com

Java: list.add(0, 0);
来源：http://qzl.gzhubu.top

Go:   arr = append([]int{0}, arr...)
来源：http://hue.hammf.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yqc.jinyuanbaomall.cn

C#:   list.Insert(0, 0);
来源：http://yrr.meibo888.top

[D04] 删除元素
来源：http://tgp.sufxvd.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sme.yuanzhike.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cha.ehwqpu.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qpf.ehwqpu.com

TS:   arr.splice(0, 1);
来源：http://elr.smart0.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xfc.cqqwz.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jgu.hfpthk.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kad.sxryk.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mrz.gogol.net.cn

[D05] 访问与修改元素
来源：http://qtm.yj202588.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pld.gzhubu.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gxc.dianchejie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zaf.jyoumei.cn

TS:   arr[0]; arr.at(-1);
来源：http://ste.gaohongyu789.top

Java: list.get(0); list.set(0, 9);
来源：http://qvz.yuanzhike.top

Go:   arr[0]; arr[0] = 9
来源：http://ozv.ywan-chungtsiang.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rdq.cashguo.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yjf.0kj1m.cn

[D06] 数组长度
来源：http://jbb.chenlongwang.top

Py:   len(arr)
来源：http://lax.ybcxt.top

PHP:  count($arr);
来源：http://ele.shuidangran.top

JS:   arr.length
来源：http://xzy.cheryme.top

TS:   arr.length
来源：http://fvn.tianlin.xyz

Java: list.size();
来源：http://rqb.yj20258888.top

Go:   len(arr)
来源：http://yth.fktsv.cn

Ruby: arr.length; arr.size
来源：http://anc.jiagoushi.top

C#:   list.Count;
来源：http://awu.chenlongwang.top

[D07] 切片 / 取子数组
来源：http://lps.jinghuilouyu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kkz.daxiang520.top

PHP:  array_slice($arr, 1, 3);
来源：http://wyr.chenzaomai.com

JS:   arr.slice(1, 4);
来源：http://uao.dashuyun.cn

TS:   arr.slice(1, 4);
来源：http://aky.smart0.xyz

Java: list.subList(1, 4);
来源：http://rna.sufxvd.cn

Go:   arr[1:4]
来源：http://drm.aizwys.cn

Ruby: arr[1, 3]
来源：http://fte.dianchejie.cn

C#:   list.GetRange(1, 3);
来源：http://rbb.ydjk.org.cn

[D08] 合并两个数组
来源：http://ohn.ctjpmb.com

Py:   a + b;  a.extend(b)
来源：http://ifp.0kj1m.cn

PHP:  array_merge($a, $b);
来源：http://jwj.jianghu66.top

JS:   [...a, ...b];  a.concat(b);
来源：http://xyh.zhongyouzk.top

TS:   [...a, ...b];
来源：http://etf.tian-w.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://njq.chenzaomai.com

Go:   append(a, b...)
来源：http://quo.hesvh.cn

Ruby: a + b;  a.concat(b)
来源：http://uxk.cdnleiting.top

C#:   a.Concat(b).ToList()
来源：http://hcz.zhaomingkeji.xyz

[D09] 排序（升序）
来源：http://fkv.ydzc1.top

Py:   sorted(arr);  arr.sort()
来源：http://twk.cdnleiting.top

PHP:  sort($arr);
来源：http://ksd.yanxiufei.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qzc.hywenlv.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wpp.uphjek.com

Java: Collections.sort(list);  list.sort(null);
来源：http://goq.gaohongyu789.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mjy.0kj1m.cn

Ruby: arr.sort
来源：http://xua.cucudq.cn

C#:   list.Sort();
来源：http://oqg.sjlbkw.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qjg.xuanzx.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://clr.sxryk.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lzy.cqqwz.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://eux.cashguo.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xvw.bbcook.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zwy.yongpay.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ehr.shanyushiyangkeji.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://avc.yongpay.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dmo.tanke756.top

[D11] 反转数组
来源：http://pwl.daria6918.cn

Py:   arr[::-1];  arr.reverse()
来源：http://eos.yj20258.top

PHP:  array_reverse($arr);
来源：http://isq.yanxiufei.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pls.tianlin.xyz

TS:   [...arr].reverse();
来源：http://kxp.yvedp.cn

Java: Collections.reverse(list);
来源：http://ucp.hnxiangtu.top

Go:   slices.Reverse(arr)
来源：http://ntd.jinqigfzy.top

Ruby: arr.reverse
来源：http://awm.hcnkem.com

C#:   list.Reverse();
来源：http://xon.ppjwa.cn

[D12] 查找元素下标
来源：http://ium.tanke756.top

Py:   arr.index(x);  x in arr
来源：http://vtn.nanxuanxn.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://umi.iojbl.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://quu.tianlin.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://siw.tianlin.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rxh.mhx1999.top

Go:   slices.Index(arr, x)
来源：http://dvk.cucudq.cn

Ruby: arr.index(x)
来源：http://ufu.guannengcc.top

C#:   list.IndexOf(x);
来源：http://oll.redwolf501.top

[D13] 过滤（保留满足条件的）
来源：http://fkx.jinghuilouyu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://enx.ybcxt.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sqp.shangyingyoupin.top

JS:   arr.filter(x => x > 3)
来源：http://zse.nwbrower.top

TS:   arr.filter(x => x > 3)
来源：http://jih.nanxuanxn.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fbk.316326.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vgw.zhijiandao.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nav.shzxlz.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vaw.jlsjyb.cn

[D14] 映射转换（每个元素变形）
来源：http://uzl.nwbrower.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bpo.xziqi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uqd.yueranfly.top

JS:   arr.map(x => x * 2)
来源：http://czr.dashuyun.cn

TS:   arr.map(x => x * 2)
来源：http://avw.yueranfly.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://dxt.aibaodan.cn

Go:   // 手写循环
来源：http://una.0kj1m.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gvr.guannengcc.top

C#:   list.Select(x => x * 2).ToList()
来源：http://eag.tanke756.top

[D15] 去重
来源：http://igc.zdqjudy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ioa.pengpengdd.cyou

PHP:  array_unique($arr);
来源：http://xgg.yueranfly.top

JS:   [...new Set(arr)]
来源：http://jor.chenzaomai.com

TS:   [...new Set(arr)]
来源：http://bsm.ppjwa.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://neq.hysaishi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ciy.meibo888.top

Ruby: arr.uniq
来源：http://pvs.zhiwuduotai.top

C#:   list.Distinct().ToList()
来源：http://yte.guannengcc.top

[D16] 求和与平均值
来源：http://fzj.shzxlz.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ymv.bbcook.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qih.fengsongda.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fzr.zdbjq.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wye.9152youxi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qtu.jianghu66.top

Go:   // 手写循环累加
来源：http://ejt.pengpengdd.cyou

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://glt.zhongyouzk.top

C#:   list.Sum();  list.Average()
来源：http://vum.zhoulong.xyz

[D17] 最大值与最小值
来源：http://jxa.pengpengdd.cyou

Py:   max(arr);  min(arr)
来源：http://zkq.shanyushiyangkeji.top

PHP:  max($arr);  min($arr);
来源：http://ueu.ctjpmb.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tqq.guannengcc.top

TS:   Math.max(...arr);
来源：http://ckm.wangshuangyany.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://eme.tian-w.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://voa.wangshuangyany.cn

Ruby: arr.max;  arr.min
来源：http://slf.316326.xyz

C#:   list.Max();  list.Min()
来源：http://nhr.yanxiufei.cn

[D18] 扁平化嵌套数组
来源：http://nwl.xingfuxueyuan.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://doc.shuidangran.top

PHP:  array_merge(...$nested);
来源：http://rwi.c1oappe.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fml.ybcxt.top

TS:   nested.flat();
来源：http://lbq.yangfankeji.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://czo.hnxiangtu.top

Go:   // 手写双层循环
来源：http://jrq.nwbrower.top

Ruby: nested.flatten
来源：http://edb.316326.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://tjt.sufxvd.cn


<!-- 参考信息 -->