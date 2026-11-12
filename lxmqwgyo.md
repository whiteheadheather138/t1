代发 wailian999

================================================================================
来源：http://hor.yonumen.top

C. 函数与作用域
来源：http://pha.yj202588.top

================================================================================
来源：http://inr.xziqi.cn

[C01] 定义函数
来源：http://gup.tian-w.cn

Py:   def add(a, b): return a + b
来源：http://pyc.zhongyouzk.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://foe.c1oappe.top

JS:   function add(a, b) { return a + b; }
来源：http://yjc.yfazqb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hpn.jqgfzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ylv.shzxlz.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gra.daria6918.cn

Ruby: def add(a, b); a + b; end
来源：http://nff.zdbjq.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://elw.xziqi.cn

[C02] 默认参数
来源：http://vkj.pengpengdd.cyou

Py:   def greet(name="World"): return name
来源：http://adu.c1oappe.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ohz.0kj1m.cn

JS:   function greet(name = "World") { return name; }
来源：http://oep.cqqwz.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ovb.aizwys.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fwk.zhongyouzk.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kcl.iojbl.cn

Ruby: def greet(name = "World") = name
来源：http://hjf.jiagoushi.top

C#:   string Greet(string name = "World") => name;
来源：http://vyw.haohaochexian.top

[C03] 可变参数
来源：http://tmt.shzxlz.cn

Py:   def total(*args): return sum(args)
来源：http://loz.kuanghao11.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hdb.yonumen.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://puf.xuetiantiany.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xst.cdnleiting.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wvv.jqgufenzy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://eew.ybcxt.top

Ruby: def total(*nums); nums.sum; end
来源：http://niz.yongpay.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zhx.ybcxt.top

[C04] 命名参数 / 关键字参数
来源：http://nfy.shanyushiyangkeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xkn.smart0.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://igy.jinqigfzy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gko.ehwqpu.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yen.haohaochexian.top

Java: // 无：用 Builder 模式或 record
来源：http://all.cashguo.top

Go:   // 无：用配置结构体参数
来源：http://wmn.xingfuxueyuan.xyz

Ruby: f(a: 1, b: 2)
来源：http://css.tian-w.cn

C#:   f(a: 1, b: 2)
来源：http://ltv.52xcode.cn

[C05] 返回多个值
来源：http://uzq.wangdashe.top

Py:   return a, b
来源：http://yxs.snrcjt.cn

PHP:  return [$a, $b];
来源：http://usv.yuanzhike.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://qqg.xuanzx.com

TS:   return { a, b };
来源：http://pqj.aibaodan.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zzv.svipenyu.cn

Go:   return a, b
来源：http://bwi.feifeiyinyue.top

Ruby: return a, b
来源：http://cwa.shanyushiyangtech.top

C#:   return (a, b);              // ValueTuple
来源：http://arx.xziqi.cn

[C06] 匿名函数 / lambda
来源：http://ygr.tanke756.top

Py:   square = lambda x: x * x
来源：http://nau.redwolf501.top

PHP:  $square = fn($x) => $x * $x;
来源：http://dsm.gotoacloud.top

JS:   const square = x => x * x;
来源：http://qns.yuxming.cn

TS:   const square = (x: number): number => x * x;
来源：http://ixt.quarkkingdee.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ojo.epnwcf.com

Go:   sq := func(x int) int { return x * x }
来源：http://juw.tarul.cn

Ruby: square = ->(x) { x * x }
来源：http://akt.ydzc1.top

C#:   Func<int, int> square = x => x * x;
来源：http://pxc.ppjwa.cn

[C07] 把函数作为参数传入
来源：http://ykx.jlsjyb.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://eai.chenzaomai.com

PHP:  array_map("strtoupper", $arr);
来源：http://wgg.fehbvm.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://umt.yanxiufei.cn

TS:   arr.map(String)
来源：http://pzr.epnwcf.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dqg.ehwqpu.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ndg.wangdashe.top

Ruby: arr.map(&:upcase)
来源：http://ntc.svipenyu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://anl.cqqwz.cn

[C08] 闭包
来源：http://qiz.yangfankeji.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://byh.fehbvm.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vhq.guannengcc.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ilt.gogol.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ldh.haohaochexian.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lkl.gzhubu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qne.nanxinkj.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qba.tanke756.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dhv.nanxinkj.top

[C09] 递归
来源：http://rnp.nwbrower.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rzv.chenzaomai.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dws.redwolf501.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ull.vqdsnc.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://adm.sxryk.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://boz.xinyue.icu

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kay.xuanzx.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xih.ctjpmb.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dgz.smart0.xyz

[C10] 变量作用域
来源：http://oro.yueranfly.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gkc.yangfankeji.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lpo.sjlbkw.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nlj.jqgufenzy.top

TS:   同 JS
来源：http://nqn.jinghuilouyu.cn

Java: 方法内为块级作用域
来源：http://gdw.ywan-chungtsiang.top

Go:   花括号块级作用域
来源：http://apl.dashuyun.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yty.wangshuangyany.cn

C#:   块级作用域
来源：http://bjr.bjfxy.top

[C11] 模块导入与导出
来源：http://jsx.ybcxt.top

Py:   from module import func
来源：http://htr.jinqigufen.top

PHP:  require "file.php";  或 use App\Service;
来源：http://spt.fzhhl.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://jbc.tian-w.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qfy.jinqigufen.top

Java: import java.util.List;
来源：http://kvp.52xcode.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://llo.ywan-chungtsiang.top

Ruby: require "json"; require_relative "./util"
来源：http://ymf.jlsjyb.cn

C#:   using System.Text;
来源：http://pnn.shanyushiyangkeji.top

[C12] 立即执行函数 IIFE
来源：http://cns.gaohongyu789.top

Py:   (lambda: print("run"))()
来源：http://bvx.aibaodan.cn

PHP:  (function () { echo "run"; })();
来源：http://rdf.nanxinkj.top

JS:   (() => { console.log("run"); })();
来源：http://odx.xingfuxueyuan.xyz

TS:   (() => { console.log("run"); })();
来源：http://qmb.nanxinkj.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ehh.jinqigufen.top

Go:   func() { fmt.Println("run") }()
来源：http://ymi.zhiwuduotai.top

Ruby: -> { puts "run" }.call
来源：http://ygi.zhaomingkeji.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://ctr.zhoulong.xyz

[C13] 类型声明 / 类型注解
来源：http://fdd.fengsongda.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://oik.ydzc1.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aed.jinqigufen.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wqr.zdbjq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qsk.svipenyu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://blc.redwolf501.top

Go:   func add(a, b int) int
来源：http://bfj.c1oappe.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ukj.fanxiaobao.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://rzi.hesvh.cn

[C14] 泛型函数
来源：http://njt.feifeiyinyue.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bna.yanxiufei.cn

PHP:  // 无泛型
来源：http://gfa.jqgfzy.top

JS:   // 无泛型
来源：http://poa.yfazqb.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wbm.quarkkingdee.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vny.zhengqikj.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lnj.xuanzx.com

Ruby: # 无泛型
来源：http://krf.shuidangran.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://meh.yangfankeji.com

[C15] 解构 / 展开参数
来源：http://prk.zhijiandao.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qom.yangfankeji.com

PHP:  [$a, $b] = $pair;
来源：http://byu.cdnleiting.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ccy.zhoulong.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qws.9152youxi.cn

Java: // 无解构
来源：http://mlb.hnqzz.top

Go:   // 无解构
来源：http://twm.aibaodan.cn

Ruby: a, b = pair
来源：http://swr.pycfn.com

C#:   var (a, b) = pair;
来源：http://cra.tanke756.top

[C16] 函数 / 方法重载
来源：http://yux.fzhhl.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hoz.shanyushiyangkeji.top

PHP:  // 无重载
来源：http://rus.mhx1999.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://qha.feifeiyinyue.top

TS:   // 用联合类型或重载签名声明
来源：http://zof.xinyue.icu

Java: void f(int a) {}  void f(String a) {}
来源：http://epq.quarkkingdee.top

Go:   // 无重载：用不同函数名
来源：http://das.zhixingplan.top

Ruby: # 无重载：靠动态参数
来源：http://oet.zhongyouzk.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://wan.sjlbkw.cn

================================================================================
来源：http://ebn.chenzaomai.com

D. 数组 / 列表 / 集合
来源：http://qjw.hfpthk.cn

================================================================================
来源：http://zit.yonumen.top

[D01] 创建数组 / 列表
来源：http://pzj.hnxiangtu.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://eru.sjlbkw.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pqe.havefunace.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fgd.haohaochexian.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://vvp.hfpthk.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ejp.wangshuangyany.cn

Go:   arr := []int{1, 2, 3}
来源：http://fgm.xylfe.cn

Ruby: arr = [1, 2, 3]
来源：http://fut.iojbl.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hbk.jqgufenzy.top

[D02] 追加元素到末尾
来源：http://sux.pengpengdd.cyou

Py:   arr.append(4); arr.extend([5, 6])
来源：http://umc.jinqigufen.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ypg.xingfuxueyuan.xyz

JS:   arr.push(4);
来源：http://wtx.meibo888.top

TS:   arr.push(4);
来源：http://fuh.shangyingyoupin.top

Java: list.add(4);
来源：http://byy.shuidangran.top

Go:   arr = append(arr, 4)
来源：http://bpr.shanyushiyangtech.top

Ruby: arr << 4; arr.push(5)
来源：http://kmb.yonumen.top

C#:   list.Add(4);
来源：http://drp.hywenlv.cn

[D03] 在指定位置插入元素
来源：http://zkz.xylfe.cn

Py:   arr.insert(0, 0)
来源：http://kgg.xylfe.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://giy.zdqjudy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wvz.9152youxi.cn

TS:   arr.splice(0, 0, 0);
来源：http://qvg.ctjpmb.com

Java: list.add(0, 0);
来源：http://icx.zhongyouzk.top

Go:   arr = append([]int{0}, arr...)
来源：http://rda.haohaochexian.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pta.zdbjq.cn

C#:   list.Insert(0, 0);
来源：http://hge.gotoacloud.top

[D04] 删除元素
来源：http://fdk.cheryme.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hss.zhixingplan.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://elf.zdqjudy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cje.hfpthk.cn

TS:   arr.splice(0, 1);
来源：http://mou.zycfv.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kky.kuanghao11.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://owd.tianlin.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fsq.zhixingplan.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dgw.jinqigufen.top

[D05] 访问与修改元素
来源：http://hdi.sufxvd.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lat.ybcxt.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hkt.wangshuangyany.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gfr.zhiwuduotai.top

TS:   arr[0]; arr.at(-1);
来源：http://rtm.jinghuilouyu.cn

Java: list.get(0); list.set(0, 9);
来源：http://ofv.hcnkem.com

Go:   arr[0]; arr[0] = 9
来源：http://xar.cashguo.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pxt.gogol.net.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zue.fzhhl.top

[D06] 数组长度
来源：http://xvi.ydzc1.top

Py:   len(arr)
来源：http://usa.uphjek.com

PHP:  count($arr);
来源：http://bdx.fktsv.cn

JS:   arr.length
来源：http://nxb.xylfe.cn

TS:   arr.length
来源：http://jbj.yonumen.top

Java: list.size();
来源：http://kzv.meibo888.top

Go:   len(arr)
来源：http://pyh.andypj.xyz

Ruby: arr.length; arr.size
来源：http://yfc.gogol.net.cn

C#:   list.Count;
来源：http://uyo.hfpthk.cn

[D07] 切片 / 取子数组
来源：http://rzw.cashguo.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bgy.aibaodan.cn

PHP:  array_slice($arr, 1, 3);
来源：http://enp.yj202588.top

JS:   arr.slice(1, 4);
来源：http://weg.haohaochexian.top

TS:   arr.slice(1, 4);
来源：http://mke.quarkkingdee.top

Java: list.subList(1, 4);
来源：http://qcc.yvedp.cn

Go:   arr[1:4]
来源：http://aut.vqdsnc.cn

Ruby: arr[1, 3]
来源：http://qnl.ctjpmb.com

C#:   list.GetRange(1, 3);
来源：http://tqi.sxryk.cn

[D08] 合并两个数组
来源：http://esw.hysaishi.cn

Py:   a + b;  a.extend(b)
来源：http://pse.haohaochexian.top

PHP:  array_merge($a, $b);
来源：http://rmo.uphjek.com

JS:   [...a, ...b];  a.concat(b);
来源：http://pzr.zdbjq.cn

TS:   [...a, ...b];
来源：http://qvu.hywenlv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nch.vqdsnc.cn

Go:   append(a, b...)
来源：http://xud.yvedp.cn

Ruby: a + b;  a.concat(b)
来源：http://dhh.316326.xyz

C#:   a.Concat(b).ToList()
来源：http://amo.cucudq.cn

[D09] 排序（升序）
来源：http://qco.hnqzz.top

Py:   sorted(arr);  arr.sort()
来源：http://iuf.jyoumei.cn

PHP:  sort($arr);
来源：http://lif.sjlbkw.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://esc.chenzaomai.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://qmx.yanxiufei.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gdk.jianghu66.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mfc.jianghu66.top

Ruby: arr.sort
来源：http://otz.aibaodan.cn

C#:   list.Sort();
来源：http://csm.zhijiandao.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://dfd.xuetiantiany.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vbu.vehdjk.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pjx.cucudq.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jyp.jyoumei.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rgy.9152youxi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dzm.chenlongwang.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sgq.havefunace.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tlo.bjfxy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cil.9152youxi.cn

[D11] 反转数组
来源：http://fty.tarul.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ymx.jyoumei.cn

PHP:  array_reverse($arr);
来源：http://lsb.shzxlz.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uhq.jinqigfzy.top

TS:   [...arr].reverse();
来源：http://kfq.9152youxi.cn

Java: Collections.reverse(list);
来源：http://tis.vehdjk.com

Go:   slices.Reverse(arr)
来源：http://cwi.snrcjt.cn

Ruby: arr.reverse
来源：http://fyi.gaohongyu789.top

C#:   list.Reverse();
来源：http://tnb.ivvv.top

[D12] 查找元素下标
来源：http://kxx.ehwqpu.com

Py:   arr.index(x);  x in arr
来源：http://vcr.andypj.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baa.gzhubu.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jlf.zdbjq.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aik.guannengcc.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://umb.hnxiangtu.top

Go:   slices.Index(arr, x)
来源：http://bum.chenzaomai.com

Ruby: arr.index(x)
来源：http://abc.jinghuilouyu.cn

C#:   list.IndexOf(x);
来源：http://ylf.gzhubu.top

[D13] 过滤（保留满足条件的）
来源：http://cka.yonumen.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://raw.redwolf501.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jkm.ppjwa.cn

JS:   arr.filter(x => x > 3)
来源：http://prx.zdqjudy.top

TS:   arr.filter(x => x > 3)
来源：http://wil.xuetiantiany.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jtj.daxiang520.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mjr.yj202588.top

Ruby: arr.select { |x| x > 3 }
来源：http://thi.hammf.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://tam.gzhubu.top

[D14] 映射转换（每个元素变形）
来源：http://fdw.ivvv.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lyv.52xcode.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://coj.ivvv.top

JS:   arr.map(x => x * 2)
来源：http://gwh.zhengqikj.top

TS:   arr.map(x => x * 2)
来源：http://kyj.pycfn.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://wbx.nanxinkj.top

Go:   // 手写循环
来源：http://kfi.shuidangran.top

Ruby: arr.map { |x| x * 2 }
来源：http://ehz.zdqjudy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://dgj.quarkkingdee.top

[D15] 去重
来源：http://uyb.guannengcc.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vhq.andypj.xyz

PHP:  array_unique($arr);
来源：http://czu.uphjek.com

JS:   [...new Set(arr)]
来源：http://vor.9152youxi.cn

TS:   [...new Set(arr)]
来源：http://gjc.c1oappe.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vyb.havefunace.top

Go:   // 用 map[T]struct{} 手写
来源：http://njr.pengpengdd.cyou

Ruby: arr.uniq
来源：http://ais.sufxvd.cn

C#:   list.Distinct().ToList()
来源：http://lbd.c1oappe.top

[D16] 求和与平均值
来源：http://xhl.fzhhl.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://aik.sufxvd.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://afi.gaohongyu789.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tez.guowangkeji.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nxu.andypj.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://amn.gaohongyu789.top

Go:   // 手写循环累加
来源：http://arw.ybcxt.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://plf.fehbvm.com

C#:   list.Sum();  list.Average()
来源：http://ocu.jqgfzy.top

[D17] 最大值与最小值
来源：http://jiv.jqgfzy.top

Py:   max(arr);  min(arr)
来源：http://rmk.sjlbkw.cn

PHP:  max($arr);  min($arr);
来源：http://vmy.tanke756.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jfh.ppjwa.cn

TS:   Math.max(...arr);
来源：http://iak.svipenyu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://cro.zhixingplan.top


<!-- 参考信息 -->