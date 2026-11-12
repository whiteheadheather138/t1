代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://gew.wangshuangyany.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://iiu.shangyingyoupin.top

[C04] 命名参数 / 关键字参数
来源：http://hwz.bjfxy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kfi.jyoumei.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pms.epnwcf.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://trc.gzhubu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nkd.xingfuxueyuan.xyz

Java: // 无：用 Builder 模式或 record
来源：http://gqe.jlsjyb.cn

Go:   // 无：用配置结构体参数
来源：http://gjy.shanyushiyangkeji.top

Ruby: f(a: 1, b: 2)
来源：http://czu.nanxuanxn.top

C#:   f(a: 1, b: 2)
来源：http://qit.yuxming.cn

[C05] 返回多个值
来源：http://ejc.xylfe.cn

Py:   return a, b
来源：http://lud.zhongyouzk.top

PHP:  return [$a, $b];
来源：http://gph.9152youxi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xnn.chenzaomai.com

TS:   return { a, b };
来源：http://pdj.hongshengwenyu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://uoo.tarul.cn

Go:   return a, b
来源：http://ccv.jqgufenzy.top

Ruby: return a, b
来源：http://dyt.svipenyu.cn

C#:   return (a, b);              // ValueTuple
来源：http://svf.cdnleiting.top

[C06] 匿名函数 / lambda
来源：http://ynf.chenlongwang.top

Py:   square = lambda x: x * x
来源：http://psr.haohaochexian.top

PHP:  $square = fn($x) => $x * $x;
来源：http://rst.sxryk.cn

JS:   const square = x => x * x;
来源：http://ogz.tianlin.xyz

TS:   const square = (x: number): number => x * x;
来源：http://otf.zdqjudy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://khm.hnxiangtu.top

Go:   sq := func(x int) int { return x * x }
来源：http://pou.uphjek.com

Ruby: square = ->(x) { x * x }
来源：http://oze.cheryme.top

C#:   Func<int, int> square = x => x * x;
来源：http://cxo.ctjpmb.com

[C07] 把函数作为参数传入
来源：http://tqt.tanke756.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jqi.yj20258.top

PHP:  array_map("strtoupper", $arr);
来源：http://mne.guowangkeji.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ewj.ivvv.top

TS:   arr.map(String)
来源：http://uig.fktsv.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://smr.guowangkeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://res.nanxuanxn.top

Ruby: arr.map(&:upcase)
来源：http://yww.bjfxy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://gbc.yuxming.cn

[C08] 闭包
来源：http://nhy.xylfe.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://deb.havefunace.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rrj.cqqwz.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://isx.epnwcf.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pyx.fzhhl.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://amt.hfpthk.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ywr.cheryme.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tal.ybcxt.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mzj.zdqjudy.top

[C09] 递归
来源：http://dwh.52xcode.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cgz.birdmap.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lwn.hongshengwenyu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zmj.bbcook.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eta.fehbvm.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gjr.fktsv.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://quf.xingfuxueyuan.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zhm.xylfe.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dro.daxiang520.top

[C10] 变量作用域
来源：http://iez.ivvv.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vrk.dianchejie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ksw.iojbl.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tai.shzxlz.cn

TS:   同 JS
来源：http://ref.dashuyun.cn

Java: 方法内为块级作用域
来源：http://lpt.sysykeji.top

Go:   花括号块级作用域
来源：http://bgk.zdbjq.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yki.smart0.xyz

C#:   块级作用域
来源：http://zcv.zhoulong.xyz

[C11] 模块导入与导出
来源：http://cdy.ehwqpu.com

Py:   from module import func
来源：http://nar.cashguo.top

PHP:  require "file.php";  或 use App\Service;
来源：http://zrp.aibaodan.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://enr.tianlin.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ges.birdmap.top

Java: import java.util.List;
来源：http://hht.uphjek.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vsg.yj20258.top

Ruby: require "json"; require_relative "./util"
来源：http://clq.yfazqb.com

C#:   using System.Text;
来源：http://tlk.cqqwz.cn

[C12] 立即执行函数 IIFE
来源：http://wgk.shuidangran.top

Py:   (lambda: print("run"))()
来源：http://rey.ctjpmb.com

PHP:  (function () { echo "run"; })();
来源：http://zch.ybcxt.top

JS:   (() => { console.log("run"); })();
来源：http://tcf.zdbjq.cn

TS:   (() => { console.log("run"); })();
来源：http://rdg.andypj.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://eey.iojbl.cn

Go:   func() { fmt.Println("run") }()
来源：http://cvh.zdqjudy.top

Ruby: -> { puts "run" }.call
来源：http://xld.guannengcc.top

C#:   // 无 IIFE：用静态构造函数
来源：http://cue.zhixingplan.top

[C13] 类型声明 / 类型注解
来源：http://kyv.vqdsnc.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dkc.xziqi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qcd.zhiwuduotai.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xkd.yonumen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://aml.smart0.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://tme.ivvv.top

Go:   func add(a, b int) int
来源：http://qzn.pengpengdd.cyou

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ijs.nwbrower.top

C#:   int Add(int a, int b) => a + b;
来源：http://yzd.chenlongwang.top

[C14] 泛型函数
来源：http://sxg.zhaomingkeji.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://itv.tianlin.xyz

PHP:  // 无泛型
来源：http://ewq.kuanghao11.cn

JS:   // 无泛型
来源：http://rcz.wangshuangyany.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://oeu.nanxuanxn.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://asr.epnwcf.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://uxx.zhijiandao.cn

Ruby: # 无泛型
来源：http://tnr.hnxiangtu.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gsk.hywenlv.cn

[C15] 解构 / 展开参数
来源：http://pla.zhongyouzk.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://uxf.ydzc1.top

PHP:  [$a, $b] = $pair;
来源：http://ymy.tian-w.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://eud.pengpengdd.cyou

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ryr.vehdjk.com

Java: // 无解构
来源：http://pdq.hcnkem.com

Go:   // 无解构
来源：http://iyh.zhiwuduotai.top

Ruby: a, b = pair
来源：http://mcw.nanxuanxn.top

C#:   var (a, b) = pair;
来源：http://jfy.yonumen.top

[C16] 函数 / 方法重载
来源：http://cfh.chenzaomai.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bgv.feifeiyinyue.top

PHP:  // 无重载
来源：http://lys.gotoacloud.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://nnq.tian-w.cn

TS:   // 用联合类型或重载签名声明
来源：http://gya.guowangkeji.top

Java: void f(int a) {}  void f(String a) {}
来源：http://npe.iojbl.cn

Go:   // 无重载：用不同函数名
来源：http://qwq.bbcook.cn

Ruby: # 无重载：靠动态参数
来源：http://dti.tarul.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hwh.jianghu66.top

================================================================================
来源：http://ydb.hongshengwenyu.top

D. 数组 / 列表 / 集合
来源：http://irt.birdmap.top

================================================================================
来源：http://eyr.iojbl.cn

[D01] 创建数组 / 列表
来源：http://zol.zhixingplan.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://yfq.pengpengdd.cyou

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uka.xziqi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pkp.jiagoushi.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://opg.jiagoushi.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zay.pycfn.com

Go:   arr := []int{1, 2, 3}
来源：http://vbw.chenjidiqi.icu

Ruby: arr = [1, 2, 3]
来源：http://tna.shanyushiyangtech.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sbu.wangdashe.top

[D02] 追加元素到末尾
来源：http://fnk.epnwcf.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hyn.yangfankeji.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tlh.feifeiyinyue.top

JS:   arr.push(4);
来源：http://oza.yvedp.cn

TS:   arr.push(4);
来源：http://kgs.pycfn.com

Java: list.add(4);
来源：http://klr.sweek.top

Go:   arr = append(arr, 4)
来源：http://gdj.gotoacloud.top

Ruby: arr << 4; arr.push(5)
来源：http://yqn.sysykeji.top

C#:   list.Add(4);
来源：http://qit.fktsv.cn

[D03] 在指定位置插入元素
来源：http://rly.havefunace.top

Py:   arr.insert(0, 0)
来源：http://isc.yueranfly.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ukn.aibaodan.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tnk.sweek.top

TS:   arr.splice(0, 0, 0);
来源：http://sgh.c1oappe.top

Java: list.add(0, 0);
来源：http://dwq.yongpay.top

Go:   arr = append([]int{0}, arr...)
来源：http://nzl.gzhubu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://asj.chenlongwang.top

C#:   list.Insert(0, 0);
来源：http://mie.ydzc1.top

[D04] 删除元素
来源：http://gmh.jinghuilouyu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://aqh.ywan-chungtsiang.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wye.snrcjt.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ncy.yfazqb.com

TS:   arr.splice(0, 1);
来源：http://srn.birdmap.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://aht.aibaodan.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://akt.pengpengdd.cyou

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dko.daria6918.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://csg.aibaodan.cn

[D05] 访问与修改元素
来源：http://rqd.bjfxy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kjn.zhongyouzk.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://suj.mhx1999.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kqe.dianchejie.cn

TS:   arr[0]; arr.at(-1);
来源：http://kkl.kuanghao11.cn

Java: list.get(0); list.set(0, 9);
来源：http://lth.sjlbkw.cn

Go:   arr[0]; arr[0] = 9
来源：http://krh.havefunace.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://quy.yanxiufei.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dcu.xuanzx.com

[D06] 数组长度
来源：http://lpf.andypj.xyz

Py:   len(arr)
来源：http://kgz.guannengcc.top

PHP:  count($arr);
来源：http://plm.tian-w.cn

JS:   arr.length
来源：http://mdb.birdmap.top

TS:   arr.length
来源：http://dxz.hfpthk.cn

Java: list.size();
来源：http://aci.vqdsnc.cn

Go:   len(arr)
来源：http://nsj.sufxvd.cn

Ruby: arr.length; arr.size
来源：http://eyk.nwbrower.top

C#:   list.Count;
来源：http://lpl.52xcode.cn

[D07] 切片 / 取子数组
来源：http://mgo.yanxiufei.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fzk.jlsjyb.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xje.hnxiangtu.top

JS:   arr.slice(1, 4);
来源：http://zib.cqqwz.cn

TS:   arr.slice(1, 4);
来源：http://slf.cdnleiting.top

Java: list.subList(1, 4);
来源：http://fzh.ydjk.org.cn

Go:   arr[1:4]
来源：http://kpa.yj202588.top

Ruby: arr[1, 3]
来源：http://ppf.shanyushiyangtech.top

C#:   list.GetRange(1, 3);
来源：http://cvp.jlsjyb.cn

[D08] 合并两个数组
来源：http://lxz.yj20258888.top

Py:   a + b;  a.extend(b)
来源：http://inm.gogol.net.cn

PHP:  array_merge($a, $b);
来源：http://uio.jinqigfzy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://yen.cqqwz.cn

TS:   [...a, ...b];
来源：http://irb.52xcode.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jxl.vehdjk.com

Go:   append(a, b...)
来源：http://rnq.jinqigfzy.top

Ruby: a + b;  a.concat(b)
来源：http://kcx.9152youxi.cn

C#:   a.Concat(b).ToList()
来源：http://xad.gzhubu.top

[D09] 排序（升序）
来源：http://cjz.tanke756.top

Py:   sorted(arr);  arr.sort()
来源：http://wvb.yanxiufei.cn

PHP:  sort($arr);
来源：http://lfl.zhixingplan.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lcw.ydjk.org.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://pce.zhijiandao.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://iyd.xuetiantiany.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cps.feifeiyinyue.top

Ruby: arr.sort
来源：http://ccy.zhijiandao.cn

C#:   list.Sort();
来源：http://dbf.hywenlv.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://eqm.sysykeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yba.sweek.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://efn.svipenyu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dfb.hywenlv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ogd.hcnkem.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yfj.jinghuilouyu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pqv.pycfn.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://auh.xingfuxueyuan.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hid.yj20258.top

[D11] 反转数组
来源：http://cup.smart0.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://ccu.gogol.net.cn

PHP:  array_reverse($arr);
来源：http://xis.yongpay.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yrn.shuidangran.top

TS:   [...arr].reverse();
来源：http://osz.shangyingyoupin.top

Java: Collections.reverse(list);
来源：http://ycb.sweek.top

Go:   slices.Reverse(arr)
来源：http://czz.mhx1999.top

Ruby: arr.reverse
来源：http://sed.jinyuanbaomall.cn

C#:   list.Reverse();
来源：http://pbo.shzxlz.cn

[D12] 查找元素下标
来源：http://njq.zhijiandao.cn

Py:   arr.index(x);  x in arr
来源：http://wef.sufxvd.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://iit.shuidangran.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cqx.52xcode.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dso.meibo888.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://liu.shangyingyoupin.top

Go:   slices.Index(arr, x)
来源：http://qbx.jianghu66.top

Ruby: arr.index(x)
来源：http://wed.hysaishi.cn

C#:   list.IndexOf(x);
来源：http://bjz.yangfankeji.com

[D13] 过滤（保留满足条件的）
来源：http://vxr.bbcook.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fje.chenzaomai.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qyz.yonumen.top

JS:   arr.filter(x => x > 3)
来源：http://kih.cucudq.cn

TS:   arr.filter(x => x > 3)
来源：http://jvc.sufxvd.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jmg.quarkkingdee.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zji.fktsv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hqx.vehdjk.com

C#:   list.Where(x => x > 3).ToList()
来源：http://wmt.redwolf501.top

[D14] 映射转换（每个元素变形）
来源：http://jnt.havefunace.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://igx.ywan-chungtsiang.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://btr.hnqzz.top

JS:   arr.map(x => x * 2)
来源：http://jni.wangdashe.top

TS:   arr.map(x => x * 2)
来源：http://ota.sxryk.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qtq.daria6918.cn

Go:   // 手写循环
来源：http://une.feifeiyinyue.top

Ruby: arr.map { |x| x * 2 }
来源：http://efd.yj202588.top

C#:   list.Select(x => x * 2).ToList()
来源：http://kvz.xingfuxueyuan.xyz

[D15] 去重
来源：http://vuo.redwolf501.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://apq.mhx1999.top

PHP:  array_unique($arr);
来源：http://qtz.zycfv.cn

JS:   [...new Set(arr)]
来源：http://nva.pengpengdd.cyou

TS:   [...new Set(arr)]
来源：http://nrc.yuanzhike.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dax.yvedp.cn

Go:   // 用 map[T]struct{} 手写
来源：http://azv.52xcode.cn

Ruby: arr.uniq
来源：http://lam.jianghu66.top

C#:   list.Distinct().ToList()
来源：http://qod.ctjpmb.com

[D16] 求和与平均值
来源：http://wug.shzxlz.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ixc.nwbrower.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jtd.yvedp.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kbc.ywan-chungtsiang.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://brx.zhixingplan.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zte.bjfxy.top

Go:   // 手写循环累加
来源：http://fxc.yj20258.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://imt.ydjk.org.cn

C#:   list.Sum();  list.Average()
来源：http://kcc.aibaodan.cn

[D17] 最大值与最小值
来源：http://chi.yuanzhike.top

Py:   max(arr);  min(arr)
来源：http://eba.cqqwz.cn

PHP:  max($arr);  min($arr);
来源：http://zhg.ydjk.org.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qqh.yuxming.cn

TS:   Math.max(...arr);
来源：http://ilb.svipenyu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://dyt.pycfn.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ffb.xingfuxueyuan.xyz

Ruby: arr.max;  arr.min
来源：http://pfr.fzhhl.top

C#:   list.Max();  list.Min()
来源：http://tlq.hcnkem.com

[D18] 扁平化嵌套数组
来源：http://ylw.svipenyu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wpx.yfazqb.com

PHP:  array_merge(...$nested);
来源：http://day.uphjek.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://oxn.zhaomingkeji.xyz

TS:   nested.flat();
来源：http://jhz.vehdjk.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tir.nanxuanxn.top

Go:   // 手写双层循环
来源：http://vtv.aizwys.cn

Ruby: nested.flatten
来源：http://ivo.tianlin.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://dcz.fehbvm.com

[D19] 按字段分组
来源：http://gfz.yangfankeji.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jlx.hysaishi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fqg.cqqwz.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://eik.daria6918.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fmk.sufxvd.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sjo.guannengcc.top

Go:   // 手写 map[string][]T
来源：http://ghw.zhijiandao.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://yhy.zdqjudy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rcs.chenzaomai.com

[D20] 统计每个元素出现次数
来源：http://wri.ybcxt.top

Py:   Counter(arr)
来源：http://qik.zycfv.cn

PHP:  array_count_values($arr);
来源：http://arj.andypj.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://anw.zhixingplan.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lcy.hongshengwenyu.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://alv.zdqjudy.top

Go:   // 手写 map[T]int
来源：http://bwm.jinyuanbaomall.cn


<!-- 参考信息 -->