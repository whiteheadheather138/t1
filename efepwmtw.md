代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://mrn.epnwcf.com

Java: // 无默认参数：方法重载或 Optional
来源：http://neh.yuanzhike.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yln.jiagoushi.top

Ruby: def greet(name = "World") = name
来源：http://ayi.fehbvm.com

C#:   string Greet(string name = "World") => name;
来源：http://ltf.sjlbkw.cn

[C03] 可变参数
来源：http://rvt.bjfxy.top

Py:   def total(*args): return sum(args)
来源：http://kjc.sufxvd.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ulc.jianghu66.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xse.sufxvd.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hdo.hnxiangtu.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://arv.havefunace.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ryz.jinqigfzy.top

Ruby: def total(*nums); nums.sum; end
来源：http://vfi.zdqjudy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://csb.wangdashe.top

[C04] 命名参数 / 关键字参数
来源：http://mux.wangshuangyany.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ckb.yuxming.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zjf.bbcook.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sxn.yangfankeji.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://aag.xuanzx.com

Java: // 无：用 Builder 模式或 record
来源：http://ccj.fanxiaobao.xyz

Go:   // 无：用配置结构体参数
来源：http://awk.yonumen.top

Ruby: f(a: 1, b: 2)
来源：http://qsv.sjlbkw.cn

C#:   f(a: 1, b: 2)
来源：http://nmv.zhijiandao.cn

[C05] 返回多个值
来源：http://ijz.quarkkingdee.top

Py:   return a, b
来源：http://kce.yj20258.top

PHP:  return [$a, $b];
来源：http://dps.daxiang520.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://twl.wangdashe.top

TS:   return { a, b };
来源：http://pou.ydzc1.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://llv.shangyingyoupin.top

Go:   return a, b
来源：http://nfu.fehbvm.com

Ruby: return a, b
来源：http://bax.yanxiufei.cn

C#:   return (a, b);              // ValueTuple
来源：http://rql.mhx1999.top

[C06] 匿名函数 / lambda
来源：http://ijc.daxiang520.top

Py:   square = lambda x: x * x
来源：http://jwj.tian-w.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ika.svipenyu.cn

JS:   const square = x => x * x;
来源：http://zmc.hongshengwenyu.top

TS:   const square = (x: number): number => x * x;
来源：http://yel.ydjk.org.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tum.birdmap.top

Go:   sq := func(x int) int { return x * x }
来源：http://jnj.zhoulong.xyz

Ruby: square = ->(x) { x * x }
来源：http://vqc.hammf.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ddq.hesvh.cn

[C07] 把函数作为参数传入
来源：http://qwv.52xcode.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dxc.ctjpmb.com

PHP:  array_map("strtoupper", $arr);
来源：http://cma.hywenlv.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qel.birdmap.top

TS:   arr.map(String)
来源：http://hhm.xingfuxueyuan.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://miz.zhongyouzk.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kxc.snrcjt.cn

Ruby: arr.map(&:upcase)
来源：http://pbw.jqgufenzy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://qea.xuanzx.com

[C08] 闭包
来源：http://dtq.bbcook.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kbd.c1oappe.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ruj.jinqigfzy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gup.daria6918.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gwr.hcnkem.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://znv.snrcjt.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://amw.jinqigufen.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rkq.xuetiantiany.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jqi.haohaochexian.top

[C09] 递归
来源：http://goy.pengpengdd.cyou

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lkf.bbcook.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://scp.9152youxi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tlj.yonumen.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://twr.zhoulong.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bvt.jyoumei.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pnc.daxiang520.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hib.haohaochexian.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uvb.kuanghao11.cn

[C10] 变量作用域
来源：http://vor.tanke756.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://amf.9152youxi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://whs.yonumen.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kbl.hywenlv.cn

TS:   同 JS
来源：http://zrc.zhongyouzk.top

Java: 方法内为块级作用域
来源：http://azd.tanke756.top

Go:   花括号块级作用域
来源：http://vcy.zhengqikj.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pkp.gaohongyu789.top

C#:   块级作用域
来源：http://krs.fktsv.cn

[C11] 模块导入与导出
来源：http://fqf.zycfv.cn

Py:   from module import func
来源：http://bjr.fzhhl.top

PHP:  require "file.php";  或 use App\Service;
来源：http://skz.guannengcc.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://qdb.xuetiantiany.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://eix.zhijiandao.cn

Java: import java.util.List;
来源：http://olw.yuxming.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://iff.chenlongwang.top

Ruby: require "json"; require_relative "./util"
来源：http://tiy.guowangkeji.top

C#:   using System.Text;
来源：http://jhy.uphjek.com

[C12] 立即执行函数 IIFE
来源：http://kfr.quarkkingdee.top

Py:   (lambda: print("run"))()
来源：http://ejm.fzhhl.top

PHP:  (function () { echo "run"; })();
来源：http://ryy.hysaishi.cn

JS:   (() => { console.log("run"); })();
来源：http://tst.c1oappe.top

TS:   (() => { console.log("run"); })();
来源：http://vjf.feifeiyinyue.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kon.yj202588.top

Go:   func() { fmt.Println("run") }()
来源：http://ykw.xinyue.icu

Ruby: -> { puts "run" }.call
来源：http://qmc.ydzc1.top

C#:   // 无 IIFE：用静态构造函数
来源：http://isf.chenjidiqi.icu

[C13] 类型声明 / 类型注解
来源：http://muh.hfpthk.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nrs.zhijiandao.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://maj.hongshengwenyu.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pvd.guowangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hmi.smart0.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://unv.jinghuilouyu.cn

Go:   func add(a, b int) int
来源：http://sca.gotoacloud.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ofe.uphjek.com

C#:   int Add(int a, int b) => a + b;
来源：http://yid.havefunace.top

[C14] 泛型函数
来源：http://yiw.kuanghao11.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ssi.cdnleiting.top

PHP:  // 无泛型
来源：http://oot.vqdsnc.cn

JS:   // 无泛型
来源：http://bje.andypj.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yqv.chenzaomai.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://aru.xuetiantiany.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gra.jyoumei.cn

Ruby: # 无泛型
来源：http://lwf.yueranfly.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kyi.hammf.cn

[C15] 解构 / 展开参数
来源：http://dfl.dianchejie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xhg.ydjk.org.cn

PHP:  [$a, $b] = $pair;
来源：http://pnf.hongshengwenyu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rok.snrcjt.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fwa.hammf.cn

Java: // 无解构
来源：http://ikl.hfpthk.cn

Go:   // 无解构
来源：http://whs.chenlongwang.top

Ruby: a, b = pair
来源：http://pry.sjlbkw.cn

C#:   var (a, b) = pair;
来源：http://ysd.epnwcf.com

[C16] 函数 / 方法重载
来源：http://hoa.gaohongyu789.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xoo.xziqi.cn

PHP:  // 无重载
来源：http://jfz.yonumen.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://duj.xziqi.cn

TS:   // 用联合类型或重载签名声明
来源：http://tml.zhiwuduotai.top

Java: void f(int a) {}  void f(String a) {}
来源：http://zpd.jianghu66.top

Go:   // 无重载：用不同函数名
来源：http://sfx.ctjpmb.com

Ruby: # 无重载：靠动态参数
来源：http://zln.aizwys.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://obt.wangshuangyany.cn

================================================================================
来源：http://zbw.yfazqb.com

D. 数组 / 列表 / 集合
来源：http://uwe.cqqwz.cn

================================================================================
来源：http://xsk.yvedp.cn

[D01] 创建数组 / 列表
来源：http://ovz.jqgufenzy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://wvr.bjfxy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gnz.jinyuanbaomall.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gin.cucudq.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xrd.cqqwz.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://evs.yuxming.cn

Go:   arr := []int{1, 2, 3}
来源：http://zcd.epnwcf.com

Ruby: arr = [1, 2, 3]
来源：http://ulf.jiagoushi.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xti.zhongyouzk.top

[D02] 追加元素到末尾
来源：http://hoq.birdmap.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uul.daria6918.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zci.ppjwa.cn

JS:   arr.push(4);
来源：http://rpw.gaohongyu789.top

TS:   arr.push(4);
来源：http://ghk.chenzaomai.com

Java: list.add(4);
来源：http://xgy.bjfxy.top

Go:   arr = append(arr, 4)
来源：http://awl.hnxiangtu.top

Ruby: arr << 4; arr.push(5)
来源：http://nzr.cqqwz.cn

C#:   list.Add(4);
来源：http://ecn.sjlbkw.cn

[D03] 在指定位置插入元素
来源：http://fmg.andypj.xyz

Py:   arr.insert(0, 0)
来源：http://dsu.chenzaomai.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bmq.zycfv.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kgy.chenzaomai.com

TS:   arr.splice(0, 0, 0);
来源：http://btr.shangyingyoupin.top

Java: list.add(0, 0);
来源：http://kjy.xinyue.icu

Go:   arr = append([]int{0}, arr...)
来源：http://vgm.mhx1999.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mcr.yj20258.top

C#:   list.Insert(0, 0);
来源：http://ttx.fehbvm.com

[D04] 删除元素
来源：http://euf.xziqi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ajw.hammf.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ibp.xingfuxueyuan.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nnh.snrcjt.cn

TS:   arr.splice(0, 1);
来源：http://zkv.jinghuilouyu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://civ.nwbrower.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lww.sxryk.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zpj.quarkkingdee.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kgx.yvedp.cn

[D05] 访问与修改元素
来源：http://omi.zhongyouzk.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://amy.gotoacloud.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rrd.yvedp.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://krd.smart0.xyz

TS:   arr[0]; arr.at(-1);
来源：http://fov.xylfe.cn

Java: list.get(0); list.set(0, 9);
来源：http://yxq.nwbrower.top

Go:   arr[0]; arr[0] = 9
来源：http://xgw.zhaomingkeji.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://swg.cdnleiting.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sva.yj20258888.top

[D06] 数组长度
来源：http://sue.zdbjq.cn

Py:   len(arr)
来源：http://yyi.cdnleiting.top

PHP:  count($arr);
来源：http://wcg.cashguo.top

JS:   arr.length
来源：http://tjk.xuetiantiany.cn

TS:   arr.length
来源：http://mup.yuanzhike.top

Java: list.size();
来源：http://crp.ppjwa.cn

Go:   len(arr)
来源：http://usz.sufxvd.cn

Ruby: arr.length; arr.size
来源：http://czi.uphjek.com

C#:   list.Count;
来源：http://xms.quarkkingdee.top

[D07] 切片 / 取子数组
来源：http://oyv.zycfv.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kpl.daria6918.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pjy.yanxiufei.cn

JS:   arr.slice(1, 4);
来源：http://wyd.ctjpmb.com

TS:   arr.slice(1, 4);
来源：http://won.yj20258.top

Java: list.subList(1, 4);
来源：http://vwj.fehbvm.com

Go:   arr[1:4]
来源：http://nag.shzxlz.cn

Ruby: arr[1, 3]
来源：http://zgw.nwbrower.top

C#:   list.GetRange(1, 3);
来源：http://kuo.xuanzx.com

[D08] 合并两个数组
来源：http://sxz.xziqi.cn

Py:   a + b;  a.extend(b)
来源：http://rbf.kuanghao11.cn

PHP:  array_merge($a, $b);
来源：http://oza.fengsongda.top

JS:   [...a, ...b];  a.concat(b);
来源：http://srz.uphjek.com

TS:   [...a, ...b];
来源：http://kcu.haohaochexian.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xzh.yj20258888.top

Go:   append(a, b...)
来源：http://owl.zdqjudy.top

Ruby: a + b;  a.concat(b)
来源：http://pzt.guannengcc.top

C#:   a.Concat(b).ToList()
来源：http://tme.epnwcf.com

[D09] 排序（升序）
来源：http://zrt.sufxvd.cn

Py:   sorted(arr);  arr.sort()
来源：http://qpi.xuanzx.com

PHP:  sort($arr);
来源：http://kha.316326.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qyp.cheryme.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://pry.daria6918.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://emo.snrcjt.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lfb.sxryk.cn

Ruby: arr.sort
来源：http://pcf.hnqzz.top

C#:   list.Sort();
来源：http://slk.yuxming.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://wju.wangshuangyany.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dma.c1oappe.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rvd.yuxming.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qkr.jlsjyb.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://evg.jianghu66.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bnu.xuetiantiany.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kpc.fktsv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://znw.yfazqb.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yzs.redwolf501.top

[D11] 反转数组
来源：http://smf.chenlongwang.top

Py:   arr[::-1];  arr.reverse()
来源：http://zbm.shzxlz.cn

PHP:  array_reverse($arr);
来源：http://rlw.andypj.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://usv.zdqjudy.top

TS:   [...arr].reverse();
来源：http://uok.jlsjyb.cn

Java: Collections.reverse(list);
来源：http://exr.shuidangran.top

Go:   slices.Reverse(arr)
来源：http://emc.52xcode.cn

Ruby: arr.reverse
来源：http://efr.shanyushiyangkeji.top

C#:   list.Reverse();
来源：http://idt.havefunace.top

[D12] 查找元素下标
来源：http://bqo.sufxvd.cn

Py:   arr.index(x);  x in arr
来源：http://wkp.yj202588.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ohw.ppjwa.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dcd.yj202588.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sit.zhoulong.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ygy.shanyushiyangtech.top

Go:   slices.Index(arr, x)
来源：http://vdl.jinyuanbaomall.cn

Ruby: arr.index(x)
来源：http://eru.shuidangran.top

C#:   list.IndexOf(x);
来源：http://yet.sweek.top

[D13] 过滤（保留满足条件的）
来源：http://vqx.pengpengdd.cyou

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nsw.kuanghao11.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cgp.cqqwz.cn

JS:   arr.filter(x => x > 3)
来源：http://xsl.yuanzhike.top

TS:   arr.filter(x => x > 3)
来源：http://krt.xylfe.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xqt.ydzc1.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rsi.hnxiangtu.top

Ruby: arr.select { |x| x > 3 }
来源：http://mrv.redwolf501.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ciu.9152youxi.cn

[D14] 映射转换（每个元素变形）
来源：http://nzs.tian-w.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://oqk.svipenyu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://aud.jqgufenzy.top

JS:   arr.map(x => x * 2)
来源：http://dxw.yfazqb.com

TS:   arr.map(x => x * 2)
来源：http://tbq.andypj.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://guy.guowangkeji.top

Go:   // 手写循环
来源：http://msx.zhengqikj.top

Ruby: arr.map { |x| x * 2 }
来源：http://xjk.cashguo.top

C#:   list.Select(x => x * 2).ToList()
来源：http://zhg.yj20258888.top

[D15] 去重
来源：http://baf.haohaochexian.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qrm.yj20258888.top

PHP:  array_unique($arr);
来源：http://rmv.guannengcc.top

JS:   [...new Set(arr)]
来源：http://xak.fehbvm.com

TS:   [...new Set(arr)]
来源：http://caa.dashuyun.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://svt.uphjek.com

Go:   // 用 map[T]struct{} 手写
来源：http://ejk.wangdashe.top

Ruby: arr.uniq
来源：http://xid.zhijiandao.cn

C#:   list.Distinct().ToList()
来源：http://evo.xziqi.cn

[D16] 求和与平均值
来源：http://fxa.gaohongyu789.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vuc.sxryk.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zxa.shzxlz.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://amt.zhixingplan.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://afy.zycfv.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qga.ywan-chungtsiang.top

Go:   // 手写循环累加
来源：http://crr.c1oappe.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xtu.zhixingplan.top

C#:   list.Sum();  list.Average()
来源：http://bam.redwolf501.top

[D17] 最大值与最小值
来源：http://qcs.vehdjk.com

Py:   max(arr);  min(arr)
来源：http://bqx.sysykeji.top

PHP:  max($arr);  min($arr);
来源：http://iay.xinyue.icu

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rvv.316326.xyz

TS:   Math.max(...arr);
来源：http://bzh.yj20258.top

Java: Collections.max(list);  Collections.min(list);
来源：http://kcq.tarul.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gsn.svipenyu.cn

Ruby: arr.max;  arr.min
来源：http://cyi.nwbrower.top

C#:   list.Max();  list.Min()
来源：http://ygq.tianlin.xyz

[D18] 扁平化嵌套数组
来源：http://sge.gogol.net.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vwu.tianlin.xyz

PHP:  array_merge(...$nested);
来源：http://jgv.xuanzx.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://oob.sweek.top

TS:   nested.flat();
来源：http://lnb.chenjidiqi.icu

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jvu.guannengcc.top

Go:   // 手写双层循环
来源：http://igj.hysaishi.cn

Ruby: nested.flatten
来源：http://lqx.quarkkingdee.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://hcl.guannengcc.top

[D19] 按字段分组
来源：http://npo.shanyushiyangkeji.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hvq.redwolf501.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://exm.hcnkem.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nai.bjfxy.top


<!-- 参考信息 -->