代发 wailian999

[C02] 默认参数
来源：http://lhg.cdnleiting.top

Py:   def greet(name="World"): return name
来源：http://cdf.52xcode.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mig.jinyuanbaomall.cn

JS:   function greet(name = "World") { return name; }
来源：http://pwl.jianghu66.top

TS:   function greet(name: string = "World") { return name; }
来源：http://iwn.aibaodan.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://foh.yuxming.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blh.redwolf501.top

Ruby: def greet(name = "World") = name
来源：http://yfs.zhongyouzk.top

C#:   string Greet(string name = "World") => name;
来源：http://yqr.cashguo.top

[C03] 可变参数
来源：http://pen.zdqjudy.top

Py:   def total(*args): return sum(args)
来源：http://spt.vqdsnc.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ngb.zdqjudy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gcx.ctjpmb.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ahh.yfazqb.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vmv.haohaochexian.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rxu.hywenlv.cn

Ruby: def total(*nums); nums.sum; end
来源：http://quq.shzxlz.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jqg.yj20258.top

[C04] 命名参数 / 关键字参数
来源：http://xxw.hesvh.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vbk.haohaochexian.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://uoe.hnqzz.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://knm.aibaodan.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://usf.tianlin.xyz

Java: // 无：用 Builder 模式或 record
来源：http://qos.tanke756.top

Go:   // 无：用配置结构体参数
来源：http://brs.hesvh.cn

Ruby: f(a: 1, b: 2)
来源：http://kzz.tarul.cn

C#:   f(a: 1, b: 2)
来源：http://vbk.chenjidiqi.icu

[C05] 返回多个值
来源：http://iye.xingfuxueyuan.xyz

Py:   return a, b
来源：http://yly.jlsjyb.cn

PHP:  return [$a, $b];
来源：http://ins.yanxiufei.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://far.vehdjk.com

TS:   return { a, b };
来源：http://crb.mhx1999.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pca.iojbl.cn

Go:   return a, b
来源：http://hfk.hongshengwenyu.top

Ruby: return a, b
来源：http://fjt.feifeiyinyue.top

C#:   return (a, b);              // ValueTuple
来源：http://taf.jyoumei.cn

[C06] 匿名函数 / lambda
来源：http://grd.shzxlz.cn

Py:   square = lambda x: x * x
来源：http://tfo.chenzaomai.com

PHP:  $square = fn($x) => $x * $x;
来源：http://hyo.hammf.cn

JS:   const square = x => x * x;
来源：http://rtb.hywenlv.cn

TS:   const square = (x: number): number => x * x;
来源：http://edy.shuidangran.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pkh.gotoacloud.top

Go:   sq := func(x int) int { return x * x }
来源：http://ngp.52xcode.cn

Ruby: square = ->(x) { x * x }
来源：http://rcl.svipenyu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jnn.andypj.xyz

[C07] 把函数作为参数传入
来源：http://xyc.jinqigfzy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xzk.ivvv.top

PHP:  array_map("strtoupper", $arr);
来源：http://fxa.redwolf501.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://edu.daria6918.cn

TS:   arr.map(String)
来源：http://cch.yj20258888.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cla.c1oappe.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rng.hnqzz.top

Ruby: arr.map(&:upcase)
来源：http://rwg.yj202588.top

C#:   arr.Select(s => s.ToUpper())
来源：http://vpn.shangyingyoupin.top

[C08] 闭包
来源：http://pmo.nanxinkj.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vnd.yvedp.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blc.xziqi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://irk.zhiwuduotai.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hlf.xuetiantiany.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kgs.zhaomingkeji.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://csz.gotoacloud.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jwk.jinghuilouyu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://knv.iojbl.cn

[C09] 递归
来源：http://afs.jiagoushi.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ptg.daxiang520.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dyh.hcnkem.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aup.yuanzhike.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://urc.svipenyu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ipl.cdnleiting.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tkm.c1oappe.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dag.yuxming.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fem.fktsv.cn

[C10] 变量作用域
来源：http://nhr.hywenlv.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ffj.yangfankeji.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://omx.cucudq.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wqn.cdnleiting.top

TS:   同 JS
来源：http://lom.gaohongyu789.top

Java: 方法内为块级作用域
来源：http://tnh.vqdsnc.cn

Go:   花括号块级作用域
来源：http://jlx.aibaodan.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://foj.cashguo.top

C#:   块级作用域
来源：http://ohx.tanke756.top

[C11] 模块导入与导出
来源：http://rkm.fanxiaobao.xyz

Py:   from module import func
来源：http://xrj.sufxvd.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://nxg.tanke756.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ghw.tarul.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tdq.guowangkeji.top

Java: import java.util.List;
来源：http://igk.yanxiufei.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qsu.birdmap.top

Ruby: require "json"; require_relative "./util"
来源：http://quz.ydzc1.top

C#:   using System.Text;
来源：http://mmn.mhx1999.top

[C12] 立即执行函数 IIFE
来源：http://uoj.sweek.top

Py:   (lambda: print("run"))()
来源：http://umd.xinyue.icu

PHP:  (function () { echo "run"; })();
来源：http://cco.jlsjyb.cn

JS:   (() => { console.log("run"); })();
来源：http://hdq.ybcxt.top

TS:   (() => { console.log("run"); })();
来源：http://gse.cheryme.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dlr.svipenyu.cn

Go:   func() { fmt.Println("run") }()
来源：http://ehf.shuidangran.top

Ruby: -> { puts "run" }.call
来源：http://qtr.cqqwz.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://eda.hysaishi.cn

[C13] 类型声明 / 类型注解
来源：http://nac.guowangkeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fph.yueranfly.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rfv.0kj1m.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tlq.feifeiyinyue.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://erg.0kj1m.cn

Java: int add(int a, int b) { return a + b; }
来源：http://pxt.daria6918.cn

Go:   func add(a, b int) int
来源：http://thx.dianchejie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kqx.ydjk.org.cn

C#:   int Add(int a, int b) => a + b;
来源：http://zoa.cqqwz.cn

[C14] 泛型函数
来源：http://nrq.shanyushiyangtech.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lvp.svipenyu.cn

PHP:  // 无泛型
来源：http://vwz.cashguo.top

JS:   // 无泛型
来源：http://hrm.uphjek.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ocf.dianchejie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zti.shanyushiyangkeji.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kyu.fanxiaobao.xyz

Ruby: # 无泛型
来源：http://mxg.hongshengwenyu.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pmv.shuidangran.top

[C15] 解构 / 展开参数
来源：http://mgy.daria6918.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://swi.gogol.net.cn

PHP:  [$a, $b] = $pair;
来源：http://ddg.zhoulong.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sta.jianghu66.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://asm.chenjidiqi.icu

Java: // 无解构
来源：http://mwk.gogol.net.cn

Go:   // 无解构
来源：http://djn.cqqwz.cn

Ruby: a, b = pair
来源：http://bcs.52xcode.cn

C#:   var (a, b) = pair;
来源：http://cli.redwolf501.top

[C16] 函数 / 方法重载
来源：http://wxq.shangyingyoupin.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gqf.shanyushiyangkeji.top

PHP:  // 无重载
来源：http://zzd.316326.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://mdm.xuanzx.com

TS:   // 用联合类型或重载签名声明
来源：http://dnf.sxryk.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xkf.hongshengwenyu.top

Go:   // 无重载：用不同函数名
来源：http://oti.shanyushiyangkeji.top

Ruby: # 无重载：靠动态参数
来源：http://neq.redwolf501.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://tyu.nanxinkj.top

================================================================================
来源：http://yre.zhengqikj.top

D. 数组 / 列表 / 集合
来源：http://cko.hammf.cn

================================================================================
来源：http://fsx.tarul.cn

[D01] 创建数组 / 列表
来源：http://xgv.gzhubu.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://xzt.cashguo.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gfo.yanxiufei.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rmr.haohaochexian.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://yez.snrcjt.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mjy.vehdjk.com

Go:   arr := []int{1, 2, 3}
来源：http://tal.nanxuanxn.top

Ruby: arr = [1, 2, 3]
来源：http://qtq.ctjpmb.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dfa.xingfuxueyuan.xyz

[D02] 追加元素到末尾
来源：http://hjs.ehwqpu.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ryx.zdbjq.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vdn.cqqwz.cn

JS:   arr.push(4);
来源：http://cmk.cdnleiting.top

TS:   arr.push(4);
来源：http://vta.xylfe.cn

Java: list.add(4);
来源：http://djn.zycfv.cn

Go:   arr = append(arr, 4)
来源：http://gde.sweek.top

Ruby: arr << 4; arr.push(5)
来源：http://izv.pengpengdd.cyou

C#:   list.Add(4);
来源：http://lqr.shanyushiyangkeji.top

[D03] 在指定位置插入元素
来源：http://wxf.tanke756.top

Py:   arr.insert(0, 0)
来源：http://ddt.quarkkingdee.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://doc.zhijiandao.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kib.tianlin.xyz

TS:   arr.splice(0, 0, 0);
来源：http://jgj.fehbvm.com

Java: list.add(0, 0);
来源：http://tkp.shanyushiyangtech.top

Go:   arr = append([]int{0}, arr...)
来源：http://hwj.zhoulong.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zus.hesvh.cn

C#:   list.Insert(0, 0);
来源：http://vgg.yuxming.cn

[D04] 删除元素
来源：http://bpw.uphjek.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nqf.hesvh.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nda.hnxiangtu.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rtr.daria6918.cn

TS:   arr.splice(0, 1);
来源：http://llv.yueranfly.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://iwb.xingfuxueyuan.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://amr.andypj.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ubp.gotoacloud.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yzu.vehdjk.com

[D05] 访问与修改元素
来源：http://ngb.yongpay.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tdn.zhengqikj.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://atl.jianghu66.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hrz.xingfuxueyuan.xyz

TS:   arr[0]; arr.at(-1);
来源：http://xqw.yueranfly.top

Java: list.get(0); list.set(0, 9);
来源：http://pxc.yuanzhike.top

Go:   arr[0]; arr[0] = 9
来源：http://bjg.aizwys.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://grx.sxryk.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kle.sjlbkw.cn

[D06] 数组长度
来源：http://ttq.xziqi.cn

Py:   len(arr)
来源：http://ixh.bbcook.cn

PHP:  count($arr);
来源：http://puk.daria6918.cn

JS:   arr.length
来源：http://stm.shangyingyoupin.top

TS:   arr.length
来源：http://rmb.yangfankeji.com

Java: list.size();
来源：http://are.daria6918.cn

Go:   len(arr)
来源：http://nqj.9152youxi.cn

Ruby: arr.length; arr.size
来源：http://jui.jianghu66.top

C#:   list.Count;
来源：http://dzu.ehwqpu.com

[D07] 切片 / 取子数组
来源：http://vat.fanxiaobao.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tzg.sweek.top

PHP:  array_slice($arr, 1, 3);
来源：http://oia.jiagoushi.top

JS:   arr.slice(1, 4);
来源：http://eva.fzhhl.top

TS:   arr.slice(1, 4);
来源：http://wtp.daxiang520.top

Java: list.subList(1, 4);
来源：http://exz.iojbl.cn

Go:   arr[1:4]
来源：http://rlz.jlsjyb.cn

Ruby: arr[1, 3]
来源：http://qzw.dianchejie.cn

C#:   list.GetRange(1, 3);
来源：http://yrj.kuanghao11.cn

[D08] 合并两个数组
来源：http://bzx.sweek.top

Py:   a + b;  a.extend(b)
来源：http://pfm.ywan-chungtsiang.top

PHP:  array_merge($a, $b);
来源：http://wuf.zhoulong.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://edh.sysykeji.top

TS:   [...a, ...b];
来源：http://ppn.zhixingplan.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dci.ywan-chungtsiang.top

Go:   append(a, b...)
来源：http://qbn.gaohongyu789.top

Ruby: a + b;  a.concat(b)
来源：http://ecm.52xcode.cn

C#:   a.Concat(b).ToList()
来源：http://flp.nwbrower.top

[D09] 排序（升序）
来源：http://jrg.bjfxy.top

Py:   sorted(arr);  arr.sort()
来源：http://dww.ctjpmb.com

PHP:  sort($arr);
来源：http://rpl.ppjwa.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hzr.cashguo.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://hgp.quarkkingdee.top

Java: Collections.sort(list);  list.sort(null);
来源：http://waf.chenzaomai.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://aah.yuxming.cn

Ruby: arr.sort
来源：http://cwk.ppjwa.cn

C#:   list.Sort();
来源：http://hoi.hongshengwenyu.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://xsy.yj20258.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sfz.yj20258.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://epe.zhoulong.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nlm.sysykeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oal.9152youxi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://upj.ivvv.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://oqj.hesvh.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yoy.52xcode.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://igh.zhengqikj.top

[D11] 反转数组
来源：http://trr.andypj.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://qrk.andypj.xyz

PHP:  array_reverse($arr);
来源：http://jae.quarkkingdee.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nye.svipenyu.cn

TS:   [...arr].reverse();
来源：http://kij.kuanghao11.cn

Java: Collections.reverse(list);
来源：http://qny.hesvh.cn

Go:   slices.Reverse(arr)
来源：http://csx.shzxlz.cn

Ruby: arr.reverse
来源：http://gwi.hesvh.cn

C#:   list.Reverse();
来源：http://uji.andypj.xyz

[D12] 查找元素下标
来源：http://vdg.dianchejie.cn

Py:   arr.index(x);  x in arr
来源：http://oyk.zhongyouzk.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jmx.yonumen.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aja.redwolf501.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://crk.shanyushiyangkeji.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xre.chenlongwang.top

Go:   slices.Index(arr, x)
来源：http://aeh.ywan-chungtsiang.top

Ruby: arr.index(x)
来源：http://wis.jianghu66.top

C#:   list.IndexOf(x);
来源：http://krf.zdbjq.cn

[D13] 过滤（保留满足条件的）
来源：http://ljs.sxryk.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gdo.hammf.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://uav.hcnkem.com

JS:   arr.filter(x => x > 3)
来源：http://wpd.yuxming.cn

TS:   arr.filter(x => x > 3)
来源：http://cwk.ydzc1.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bxi.zhengqikj.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vrt.yangfankeji.com

Ruby: arr.select { |x| x > 3 }
来源：http://pwy.kuanghao11.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ngf.aibaodan.cn

[D14] 映射转换（每个元素变形）
来源：http://lpq.yonumen.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://szl.vehdjk.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uap.wangdashe.top

JS:   arr.map(x => x * 2)
来源：http://mdx.fzhhl.top

TS:   arr.map(x => x * 2)
来源：http://lno.chenzaomai.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://zwm.c1oappe.top

Go:   // 手写循环
来源：http://vnh.xziqi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://eds.chenjidiqi.icu

C#:   list.Select(x => x * 2).ToList()
来源：http://hnu.9152youxi.cn

[D15] 去重
来源：http://sux.pycfn.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pdl.shangyingyoupin.top

PHP:  array_unique($arr);
来源：http://lxo.tianlin.xyz

JS:   [...new Set(arr)]
来源：http://eon.ctjpmb.com

TS:   [...new Set(arr)]
来源：http://pyc.shangyingyoupin.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ppy.tian-w.cn

Go:   // 用 map[T]struct{} 手写
来源：http://pjs.zhaomingkeji.xyz

Ruby: arr.uniq
来源：http://uyn.yanxiufei.cn

C#:   list.Distinct().ToList()
来源：http://acr.jqgufenzy.top

[D16] 求和与平均值
来源：http://hln.yangfankeji.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ohu.yfazqb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xrw.dianchejie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mis.guowangkeji.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gyz.yongpay.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bht.quarkkingdee.top

Go:   // 手写循环累加
来源：http://pvd.hywenlv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://miq.yonumen.top

C#:   list.Sum();  list.Average()
来源：http://meo.vehdjk.com

[D17] 最大值与最小值
来源：http://ens.sxryk.cn

Py:   max(arr);  min(arr)
来源：http://dgq.yj20258888.top

PHP:  max($arr);  min($arr);
来源：http://ewa.cashguo.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uhe.ehwqpu.com

TS:   Math.max(...arr);
来源：http://mno.cucudq.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zqt.zhoulong.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://orr.chenlongwang.top

Ruby: arr.max;  arr.min
来源：http://xwx.0kj1m.cn

C#:   list.Max();  list.Min()
来源：http://eyy.vehdjk.com

[D18] 扁平化嵌套数组
来源：http://vbv.cucudq.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://olu.pycfn.com

PHP:  array_merge(...$nested);
来源：http://rhh.jqgfzy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tgb.shanyushiyangtech.top

TS:   nested.flat();
来源：http://kew.guannengcc.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nce.smart0.xyz

Go:   // 手写双层循环
来源：http://wal.snrcjt.cn

Ruby: nested.flatten
来源：http://fay.xylfe.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yed.jlsjyb.cn


<!-- 参考信息 -->