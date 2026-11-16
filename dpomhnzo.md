代发 wailian999

[C02] 默认参数
来源：http://yfd.zycfv.cn

Py:   def greet(name="World"): return name
来源：http://ofa.jqgfzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ith.zdqjudy.top

JS:   function greet(name = "World") { return name; }
来源：http://abv.birdmap.top

TS:   function greet(name: string = "World") { return name; }
来源：http://kho.yj20258.top

Java: // 无默认参数：方法重载或 Optional
来源：http://zaz.sweek.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ejx.zhixingplan.top

Ruby: def greet(name = "World") = name
来源：http://nrq.ctjpmb.com

C#:   string Greet(string name = "World") => name;
来源：http://iph.jinqigfzy.top

[C03] 可变参数
来源：http://goy.yanxiufei.cn

Py:   def total(*args): return sum(args)
来源：http://umr.pycfn.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xfn.shanyushiyangtech.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yrb.uphjek.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ilb.hongshengwenyu.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://aaa.aibaodan.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ymz.zdqjudy.top

Ruby: def total(*nums); nums.sum; end
来源：http://fov.ivvv.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qeh.meibo888.top

[C04] 命名参数 / 关键字参数
来源：http://csy.zhaomingkeji.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zko.xuetiantiany.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://luu.fktsv.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jer.yonumen.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uvp.yuxming.cn

Java: // 无：用 Builder 模式或 record
来源：http://oot.sxryk.cn

Go:   // 无：用配置结构体参数
来源：http://xqy.yonumen.top

Ruby: f(a: 1, b: 2)
来源：http://kyh.hcnkem.com

C#:   f(a: 1, b: 2)
来源：http://tzy.zhiwuduotai.top

[C05] 返回多个值
来源：http://ypc.jinghuilouyu.cn

Py:   return a, b
来源：http://eet.xuetiantiany.cn

PHP:  return [$a, $b];
来源：http://nyh.yuanzhike.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://mbf.ydzc1.top

TS:   return { a, b };
来源：http://hjp.dianchejie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zoi.xylfe.cn

Go:   return a, b
来源：http://vbh.redwolf501.top

Ruby: return a, b
来源：http://zad.hnxiangtu.top

C#:   return (a, b);              // ValueTuple
来源：http://snn.gogol.net.cn

[C06] 匿名函数 / lambda
来源：http://fyz.xylfe.cn

Py:   square = lambda x: x * x
来源：http://zuv.shuidangran.top

PHP:  $square = fn($x) => $x * $x;
来源：http://hiu.smart0.xyz

JS:   const square = x => x * x;
来源：http://vyi.wangdashe.top

TS:   const square = (x: number): number => x * x;
来源：http://sbs.hnxiangtu.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lkr.nanxuanxn.top

Go:   sq := func(x int) int { return x * x }
来源：http://voa.zhaomingkeji.xyz

Ruby: square = ->(x) { x * x }
来源：http://tgx.hysaishi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fkd.gogol.net.cn

[C07] 把函数作为参数传入
来源：http://orc.aibaodan.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wom.zdqjudy.top

PHP:  array_map("strtoupper", $arr);
来源：http://nvo.ywan-chungtsiang.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://shh.tianlin.xyz

TS:   arr.map(String)
来源：http://cij.yonumen.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vva.hesvh.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wbq.dashuyun.cn

Ruby: arr.map(&:upcase)
来源：http://dwf.hammf.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lxr.jinghuilouyu.cn

[C08] 闭包
来源：http://rfi.zycfv.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yyj.zhijiandao.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jra.tian-w.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wdy.mhx1999.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fld.yangfankeji.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fve.meibo888.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dui.ctjpmb.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://esp.vehdjk.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hkb.wangshuangyany.cn

[C09] 递归
来源：http://svi.dianchejie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pgd.jlsjyb.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kyc.tian-w.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pio.jinqigfzy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jdf.sysykeji.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tly.sufxvd.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mrn.bbcook.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jma.hcnkem.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uph.uphjek.com

[C10] 变量作用域
来源：http://xik.tianlin.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://oqw.sjlbkw.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hft.316326.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tfq.zhoulong.xyz

TS:   同 JS
来源：http://gbq.svipenyu.cn

Java: 方法内为块级作用域
来源：http://nty.hywenlv.cn

Go:   花括号块级作用域
来源：http://vew.tanke756.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ddc.sysykeji.top

C#:   块级作用域
来源：http://buw.9152youxi.cn

[C11] 模块导入与导出
来源：http://vgh.yongpay.top

Py:   from module import func
来源：http://rbn.ehwqpu.com

PHP:  require "file.php";  或 use App\Service;
来源：http://say.zdbjq.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://sep.ywan-chungtsiang.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xfe.ybcxt.top

Java: import java.util.List;
来源：http://dls.hesvh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fbt.aibaodan.cn

Ruby: require "json"; require_relative "./util"
来源：http://lzy.andypj.xyz

C#:   using System.Text;
来源：http://ysl.0kj1m.cn

[C12] 立即执行函数 IIFE
来源：http://fhd.fengsongda.top

Py:   (lambda: print("run"))()
来源：http://mmy.birdmap.top

PHP:  (function () { echo "run"; })();
来源：http://sor.yvedp.cn

JS:   (() => { console.log("run"); })();
来源：http://kyv.wangshuangyany.cn

TS:   (() => { console.log("run"); })();
来源：http://oor.c1oappe.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kuy.sysykeji.top

Go:   func() { fmt.Println("run") }()
来源：http://myx.jinqigufen.top

Ruby: -> { puts "run" }.call
来源：http://ezf.fktsv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qeg.shzxlz.cn

[C13] 类型声明 / 类型注解
来源：http://tmt.cqqwz.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dnu.hammf.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gte.hfpthk.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qsy.yonumen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mut.hammf.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ola.ehwqpu.com

Go:   func add(a, b int) int
来源：http://ycq.tianlin.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ipt.sweek.top

C#:   int Add(int a, int b) => a + b;
来源：http://gci.xinyue.icu

[C14] 泛型函数
来源：http://vxp.snrcjt.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vta.zdbjq.cn

PHP:  // 无泛型
来源：http://ynd.ydjk.org.cn

JS:   // 无泛型
来源：http://gbu.feifeiyinyue.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://axc.jiagoushi.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wzv.tarul.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://moj.zycfv.cn

Ruby: # 无泛型
来源：http://rhc.yonumen.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fwq.tanke756.top

[C15] 解构 / 展开参数
来源：http://pjm.fzhhl.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kft.gzhubu.top

PHP:  [$a, $b] = $pair;
来源：http://dqg.iojbl.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dql.nanxinkj.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lxs.jinqigfzy.top

Java: // 无解构
来源：http://nbe.zhengqikj.top

Go:   // 无解构
来源：http://rlk.iojbl.cn

Ruby: a, b = pair
来源：http://fhe.zhiwuduotai.top

C#:   var (a, b) = pair;
来源：http://ajb.fanxiaobao.xyz

[C16] 函数 / 方法重载
来源：http://bma.cqqwz.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dax.xingfuxueyuan.xyz

PHP:  // 无重载
来源：http://wma.ctjpmb.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://dnl.ydzc1.top

TS:   // 用联合类型或重载签名声明
来源：http://iyi.fzhhl.top

Java: void f(int a) {}  void f(String a) {}
来源：http://iyj.ybcxt.top

Go:   // 无重载：用不同函数名
来源：http://oqg.c1oappe.top

Ruby: # 无重载：靠动态参数
来源：http://twm.iojbl.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qvv.guannengcc.top

================================================================================
来源：http://qyn.gzhubu.top

D. 数组 / 列表 / 集合
来源：http://gwc.guowangkeji.top

================================================================================
来源：http://vnf.xylfe.cn

[D01] 创建数组 / 列表
来源：http://hca.mhx1999.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://fyu.yj202588.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://urz.hnxiangtu.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jqw.chenjidiqi.icu

TS:   const arr: number[] = [1, 2, 3];
来源：http://ehg.gaohongyu789.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gfg.uphjek.com

Go:   arr := []int{1, 2, 3}
来源：http://nym.bbcook.cn

Ruby: arr = [1, 2, 3]
来源：http://cbs.hesvh.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nou.hnxiangtu.top

[D02] 追加元素到末尾
来源：http://gel.sjlbkw.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ezc.tarul.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rlb.xylfe.cn

JS:   arr.push(4);
来源：http://gyd.cucudq.cn

TS:   arr.push(4);
来源：http://oso.ydzc1.top

Java: list.add(4);
来源：http://znk.chenjidiqi.icu

Go:   arr = append(arr, 4)
来源：http://iap.xziqi.cn

Ruby: arr << 4; arr.push(5)
来源：http://fem.haohaochexian.top

C#:   list.Add(4);
来源：http://zhu.gzhubu.top

[D03] 在指定位置插入元素
来源：http://gqm.birdmap.top

Py:   arr.insert(0, 0)
来源：http://rjy.meibo888.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://eup.yvedp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dyh.cashguo.top

TS:   arr.splice(0, 0, 0);
来源：http://wzp.vqdsnc.cn

Java: list.add(0, 0);
来源：http://ikf.fengsongda.top

Go:   arr = append([]int{0}, arr...)
来源：http://pwf.hesvh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rkw.shanyushiyangkeji.top

C#:   list.Insert(0, 0);
来源：http://ovc.snrcjt.cn

[D04] 删除元素
来源：http://bli.guannengcc.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dbm.xziqi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rcx.yonumen.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wxm.shanyushiyangtech.top

TS:   arr.splice(0, 1);
来源：http://pxc.yuanzhike.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vlr.dashuyun.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pwv.yj20258888.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://izv.ehwqpu.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://igv.hnxiangtu.top

[D05] 访问与修改元素
来源：http://jrc.gotoacloud.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jnu.snrcjt.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uiu.guowangkeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://brc.uphjek.com

TS:   arr[0]; arr.at(-1);
来源：http://zng.fehbvm.com

Java: list.get(0); list.set(0, 9);
来源：http://jme.kuanghao11.cn

Go:   arr[0]; arr[0] = 9
来源：http://syg.cashguo.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://eob.ybcxt.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rgn.zycfv.cn

[D06] 数组长度
来源：http://syh.epnwcf.com

Py:   len(arr)
来源：http://lbt.52xcode.cn

PHP:  count($arr);
来源：http://uxj.daxiang520.top

JS:   arr.length
来源：http://dwa.hammf.cn

TS:   arr.length
来源：http://vrp.gzhubu.top

Java: list.size();
来源：http://lry.jiagoushi.top

Go:   len(arr)
来源：http://fvc.ybcxt.top

Ruby: arr.length; arr.size
来源：http://oih.aizwys.cn

C#:   list.Count;
来源：http://hoa.yonumen.top

[D07] 切片 / 取子数组
来源：http://zwt.jyoumei.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://coo.zycfv.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jsp.zhaomingkeji.xyz

JS:   arr.slice(1, 4);
来源：http://hwb.haohaochexian.top

TS:   arr.slice(1, 4);
来源：http://stb.birdmap.top

Java: list.subList(1, 4);
来源：http://eca.cashguo.top

Go:   arr[1:4]
来源：http://ojl.fehbvm.com

Ruby: arr[1, 3]
来源：http://zml.jyoumei.cn

C#:   list.GetRange(1, 3);
来源：http://bwn.jlsjyb.cn

[D08] 合并两个数组
来源：http://zoi.cucudq.cn

Py:   a + b;  a.extend(b)
来源：http://ygg.zycfv.cn

PHP:  array_merge($a, $b);
来源：http://dab.zdqjudy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://gnf.gogol.net.cn

TS:   [...a, ...b];
来源：http://xfy.dianchejie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xgd.jinqigufen.top

Go:   append(a, b...)
来源：http://bhf.shzxlz.cn

Ruby: a + b;  a.concat(b)
来源：http://mdh.xuanzx.com

C#:   a.Concat(b).ToList()
来源：http://frg.yj20258888.top

[D09] 排序（升序）
来源：http://hzk.jqgufenzy.top

Py:   sorted(arr);  arr.sort()
来源：http://eds.hysaishi.cn

PHP:  sort($arr);
来源：http://zrs.yanxiufei.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://oie.ywan-chungtsiang.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://qyr.pycfn.com

Java: Collections.sort(list);  list.sort(null);
来源：http://ssd.cucudq.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rpt.epnwcf.com

Ruby: arr.sort
来源：http://yeo.gogol.net.cn

C#:   list.Sort();
来源：http://hbt.vqdsnc.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://inw.yvedp.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dqt.shanyushiyangkeji.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tfi.jqgfzy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gnk.bbcook.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ilh.birdmap.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gom.hfpthk.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zrt.tianlin.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tzt.xuanzx.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://aki.hammf.cn

[D11] 反转数组
来源：http://xhx.jinyuanbaomall.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zcx.ydzc1.top

PHP:  array_reverse($arr);
来源：http://gje.xuetiantiany.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rbl.gotoacloud.top

TS:   [...arr].reverse();
来源：http://okz.zhoulong.xyz

Java: Collections.reverse(list);
来源：http://quf.cashguo.top

Go:   slices.Reverse(arr)
来源：http://myy.tarul.cn

Ruby: arr.reverse
来源：http://qih.jinqigufen.top

C#:   list.Reverse();
来源：http://pyj.nwbrower.top

[D12] 查找元素下标
来源：http://yly.ppjwa.cn

Py:   arr.index(x);  x in arr
来源：http://ajz.pycfn.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://iyq.gogol.net.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xnb.jinyuanbaomall.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rdu.aibaodan.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dia.tianlin.xyz

Go:   slices.Index(arr, x)
来源：http://lwm.xziqi.cn

Ruby: arr.index(x)
来源：http://gmh.mhx1999.top

C#:   list.IndexOf(x);
来源：http://cuq.yj20258888.top

[D13] 过滤（保留满足条件的）
来源：http://rwa.zhixingplan.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hda.tarul.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jex.zhengqikj.top

JS:   arr.filter(x => x > 3)
来源：http://vzg.pengpengdd.cyou

TS:   arr.filter(x => x > 3)
来源：http://jom.aibaodan.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lvf.vehdjk.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cdu.mhx1999.top

Ruby: arr.select { |x| x > 3 }
来源：http://uea.ivvv.top

C#:   list.Where(x => x > 3).ToList()
来源：http://xgi.yfazqb.com

[D14] 映射转换（每个元素变形）
来源：http://abd.jyoumei.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zaf.gotoacloud.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gtk.zhixingplan.top

JS:   arr.map(x => x * 2)
来源：http://smp.zycfv.cn

TS:   arr.map(x => x * 2)
来源：http://zsh.hammf.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ppn.xuanzx.com

Go:   // 手写循环
来源：http://rxx.sweek.top

Ruby: arr.map { |x| x * 2 }
来源：http://abw.shangyingyoupin.top

C#:   list.Select(x => x * 2).ToList()
来源：http://qye.xingfuxueyuan.xyz

[D15] 去重
来源：http://zro.zhiwuduotai.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ycu.ydjk.org.cn

PHP:  array_unique($arr);
来源：http://jus.tarul.cn

JS:   [...new Set(arr)]
来源：http://xhu.fehbvm.com

TS:   [...new Set(arr)]
来源：http://cli.yueranfly.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kpf.hnxiangtu.top

Go:   // 用 map[T]struct{} 手写
来源：http://qqn.epnwcf.com

Ruby: arr.uniq
来源：http://iog.aibaodan.cn

C#:   list.Distinct().ToList()
来源：http://ktp.316326.xyz

[D16] 求和与平均值
来源：http://boy.dashuyun.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ahe.jiagoushi.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://oxf.ehwqpu.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rsg.cashguo.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ffd.zhaomingkeji.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gjs.yuxming.cn

Go:   // 手写循环累加
来源：http://ftk.9152youxi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://moo.mhx1999.top

C#:   list.Sum();  list.Average()
来源：http://aqr.pengpengdd.cyou

[D17] 最大值与最小值
来源：http://yqs.tanke756.top

Py:   max(arr);  min(arr)
来源：http://akh.jianghu66.top

PHP:  max($arr);  min($arr);
来源：http://vsn.yueranfly.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yvs.zhixingplan.top

TS:   Math.max(...arr);
来源：http://omz.svipenyu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://wvh.cucudq.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ttg.xuanzx.com

Ruby: arr.max;  arr.min
来源：http://sdx.shuidangran.top

C#:   list.Max();  list.Min()
来源：http://spb.gzhubu.top

[D18] 扁平化嵌套数组
来源：http://dwx.dashuyun.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tup.dianchejie.cn

PHP:  array_merge(...$nested);
来源：http://xub.sjlbkw.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://khc.yvedp.cn

TS:   nested.flat();
来源：http://vpv.jianghu66.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://djl.tianlin.xyz

Go:   // 手写双层循环
来源：http://uoe.bjfxy.top

Ruby: nested.flatten
来源：http://otb.fehbvm.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://vkq.fehbvm.com


<!-- 参考信息 -->