代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://vdl.cashguo.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dgp.jinqigfzy.top

[C04] 命名参数 / 关键字参数
来源：http://tlv.52xcode.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kmj.ybcxt.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ujv.vehdjk.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kgi.haohaochexian.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fxa.aibaodan.cn

Java: // 无：用 Builder 模式或 record
来源：http://zwa.yuanzhike.top

Go:   // 无：用配置结构体参数
来源：http://sdv.xingfuxueyuan.xyz

Ruby: f(a: 1, b: 2)
来源：http://vwu.vehdjk.com

C#:   f(a: 1, b: 2)
来源：http://qjs.gotoacloud.top

[C05] 返回多个值
来源：http://wzp.tian-w.cn

Py:   return a, b
来源：http://ysf.daria6918.cn

PHP:  return [$a, $b];
来源：http://hlq.hammf.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://mhb.dashuyun.cn

TS:   return { a, b };
来源：http://wvw.daria6918.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lzi.pengpengdd.cyou

Go:   return a, b
来源：http://jdq.hnqzz.top

Ruby: return a, b
来源：http://szq.52xcode.cn

C#:   return (a, b);              // ValueTuple
来源：http://xst.bbcook.cn

[C06] 匿名函数 / lambda
来源：http://ayk.52xcode.cn

Py:   square = lambda x: x * x
来源：http://amb.quarkkingdee.top

PHP:  $square = fn($x) => $x * $x;
来源：http://tng.jinghuilouyu.cn

JS:   const square = x => x * x;
来源：http://uxw.ybcxt.top

TS:   const square = (x: number): number => x * x;
来源：http://eda.ivvv.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kir.xinyue.icu

Go:   sq := func(x int) int { return x * x }
来源：http://fog.guowangkeji.top

Ruby: square = ->(x) { x * x }
来源：http://ijt.chenjidiqi.icu

C#:   Func<int, int> square = x => x * x;
来源：http://rof.jinyuanbaomall.cn

[C07] 把函数作为参数传入
来源：http://tng.cqqwz.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://asn.kuanghao11.cn

PHP:  array_map("strtoupper", $arr);
来源：http://rfd.zhoulong.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ltx.daria6918.cn

TS:   arr.map(String)
来源：http://nql.chenlongwang.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xlx.bbcook.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ttj.xziqi.cn

Ruby: arr.map(&:upcase)
来源：http://ssq.wangdashe.top

C#:   arr.Select(s => s.ToUpper())
来源：http://hib.xingfuxueyuan.xyz

[C08] 闭包
来源：http://wdw.cucudq.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jry.cashguo.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qsz.jyoumei.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hqe.yonumen.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ksu.daxiang520.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xiy.chenlongwang.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mtn.wangshuangyany.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gzw.feifeiyinyue.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hfe.tanke756.top

[C09] 递归
来源：http://kwh.vqdsnc.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qkq.zhiwuduotai.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tkk.iojbl.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ppl.yanxiufei.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qfr.wangshuangyany.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://txg.wangshuangyany.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zzq.aibaodan.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kkt.52xcode.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ajl.tanke756.top

[C10] 变量作用域
来源：http://zyp.nanxuanxn.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rwm.haohaochexian.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pgl.zdqjudy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ibl.shangyingyoupin.top

TS:   同 JS
来源：http://zin.birdmap.top

Java: 方法内为块级作用域
来源：http://kcj.xylfe.cn

Go:   花括号块级作用域
来源：http://yjc.zdbjq.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yaq.nanxinkj.top

C#:   块级作用域
来源：http://plo.fengsongda.top

[C11] 模块导入与导出
来源：http://bzd.cucudq.cn

Py:   from module import func
来源：http://ddy.hongshengwenyu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://csf.cdnleiting.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://fbe.zhongyouzk.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lkt.redwolf501.top

Java: import java.util.List;
来源：http://ssc.xinyue.icu

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jwy.c1oappe.top

Ruby: require "json"; require_relative "./util"
来源：http://cle.316326.xyz

C#:   using System.Text;
来源：http://nbd.xuanzx.com

[C12] 立即执行函数 IIFE
来源：http://nwh.yangfankeji.com

Py:   (lambda: print("run"))()
来源：http://sbt.yfazqb.com

PHP:  (function () { echo "run"; })();
来源：http://dyw.zhijiandao.cn

JS:   (() => { console.log("run"); })();
来源：http://tid.chenlongwang.top

TS:   (() => { console.log("run"); })();
来源：http://ctv.9152youxi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://adl.hnxiangtu.top

Go:   func() { fmt.Println("run") }()
来源：http://gxx.iojbl.cn

Ruby: -> { puts "run" }.call
来源：http://mph.jinqigfzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://rxj.c1oappe.top

[C13] 类型声明 / 类型注解
来源：http://ikg.vehdjk.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dji.shzxlz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ciz.jinqigufen.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mha.yuxming.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ptm.daria6918.cn

Java: int add(int a, int b) { return a + b; }
来源：http://quo.jinqigufen.top

Go:   func add(a, b int) int
来源：http://kvh.shuidangran.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vgn.bbcook.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vzt.xinyue.icu

[C14] 泛型函数
来源：http://wwy.zhongyouzk.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://osb.chenlongwang.top

PHP:  // 无泛型
来源：http://pil.cdnleiting.top

JS:   // 无泛型
来源：http://yho.snrcjt.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ubp.pycfn.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ntj.zhijiandao.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jfy.fanxiaobao.xyz

Ruby: # 无泛型
来源：http://dsk.gzhubu.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://arb.fanxiaobao.xyz

[C15] 解构 / 展开参数
来源：http://lil.tian-w.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://okc.shanyushiyangtech.top

PHP:  [$a, $b] = $pair;
来源：http://uos.pycfn.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ood.cashguo.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qwk.cqqwz.cn

Java: // 无解构
来源：http://wgv.havefunace.top

Go:   // 无解构
来源：http://lot.yuxming.cn

Ruby: a, b = pair
来源：http://uyt.zhongyouzk.top

C#:   var (a, b) = pair;
来源：http://pip.sysykeji.top

[C16] 函数 / 方法重载
来源：http://hmh.jianghu66.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rcu.sweek.top

PHP:  // 无重载
来源：http://jfm.yuanzhike.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://dwk.hongshengwenyu.top

TS:   // 用联合类型或重载签名声明
来源：http://owz.0kj1m.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mwr.xuanzx.com

Go:   // 无重载：用不同函数名
来源：http://kyx.0kj1m.cn

Ruby: # 无重载：靠动态参数
来源：http://ngw.xuetiantiany.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://eca.0kj1m.cn

================================================================================
来源：http://hke.gogol.net.cn

D. 数组 / 列表 / 集合
来源：http://jvg.52xcode.cn

================================================================================
来源：http://bhn.redwolf501.top

[D01] 创建数组 / 列表
来源：http://fxv.ppjwa.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://iwh.nwbrower.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uvc.daxiang520.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://noq.yuanzhike.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://sjj.feifeiyinyue.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://csk.wangshuangyany.cn

Go:   arr := []int{1, 2, 3}
来源：http://iyr.daria6918.cn

Ruby: arr = [1, 2, 3]
来源：http://oae.bbcook.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nas.jianghu66.top

[D02] 追加元素到末尾
来源：http://mcf.sweek.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vdt.yanxiufei.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://anh.birdmap.top

JS:   arr.push(4);
来源：http://ove.xylfe.cn

TS:   arr.push(4);
来源：http://wjk.havefunace.top

Java: list.add(4);
来源：http://leu.fktsv.cn

Go:   arr = append(arr, 4)
来源：http://lsx.birdmap.top

Ruby: arr << 4; arr.push(5)
来源：http://vms.ywan-chungtsiang.top

C#:   list.Add(4);
来源：http://qgo.pycfn.com

[D03] 在指定位置插入元素
来源：http://xtw.birdmap.top

Py:   arr.insert(0, 0)
来源：http://vux.fanxiaobao.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://sbw.ywan-chungtsiang.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mjg.mhx1999.top

TS:   arr.splice(0, 0, 0);
来源：http://rhp.wangshuangyany.cn

Java: list.add(0, 0);
来源：http://lfq.chenlongwang.top

Go:   arr = append([]int{0}, arr...)
来源：http://tpb.nanxinkj.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gbv.shangyingyoupin.top

C#:   list.Insert(0, 0);
来源：http://rby.jinghuilouyu.cn

[D04] 删除元素
来源：http://nds.ctjpmb.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://enu.redwolf501.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vcu.chenlongwang.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://eid.aizwys.cn

TS:   arr.splice(0, 1);
来源：http://vfv.zdqjudy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fnj.aizwys.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sgv.yfazqb.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wyq.sxryk.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ztj.tanke756.top

[D05] 访问与修改元素
来源：http://dby.ivvv.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ucj.pycfn.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yjw.jqgufenzy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ypz.ctjpmb.com

TS:   arr[0]; arr.at(-1);
来源：http://yls.sweek.top

Java: list.get(0); list.set(0, 9);
来源：http://lwa.haohaochexian.top

Go:   arr[0]; arr[0] = 9
来源：http://uru.hesvh.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ome.zhongyouzk.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://njq.vehdjk.com

[D06] 数组长度
来源：http://xcl.cashguo.top

Py:   len(arr)
来源：http://tul.jiagoushi.top

PHP:  count($arr);
来源：http://yxt.dashuyun.cn

JS:   arr.length
来源：http://ayk.guannengcc.top

TS:   arr.length
来源：http://xia.nanxuanxn.top

Java: list.size();
来源：http://gbi.tanke756.top

Go:   len(arr)
来源：http://ozi.jinqigufen.top

Ruby: arr.length; arr.size
来源：http://usf.hnqzz.top

C#:   list.Count;
来源：http://kft.ydjk.org.cn

[D07] 切片 / 取子数组
来源：http://gsu.zhongyouzk.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bka.zhixingplan.top

PHP:  array_slice($arr, 1, 3);
来源：http://dfx.zhongyouzk.top

JS:   arr.slice(1, 4);
来源：http://sbf.daxiang520.top

TS:   arr.slice(1, 4);
来源：http://xug.shzxlz.cn

Java: list.subList(1, 4);
来源：http://jlg.nwbrower.top

Go:   arr[1:4]
来源：http://dut.hnxiangtu.top

Ruby: arr[1, 3]
来源：http://olj.kuanghao11.cn

C#:   list.GetRange(1, 3);
来源：http://paq.daxiang520.top

[D08] 合并两个数组
来源：http://lbf.xziqi.cn

Py:   a + b;  a.extend(b)
来源：http://nqy.yongpay.top

PHP:  array_merge($a, $b);
来源：http://lpm.zhijiandao.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://flw.ppjwa.cn

TS:   [...a, ...b];
来源：http://qew.guannengcc.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lgb.zhiwuduotai.top

Go:   append(a, b...)
来源：http://efl.snrcjt.cn

Ruby: a + b;  a.concat(b)
来源：http://qrl.vqdsnc.cn

C#:   a.Concat(b).ToList()
来源：http://sxc.tian-w.cn

[D09] 排序（升序）
来源：http://nhb.yj20258.top

Py:   sorted(arr);  arr.sort()
来源：http://eku.316326.xyz

PHP:  sort($arr);
来源：http://xvj.tarul.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yrn.xylfe.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wfh.jinyuanbaomall.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://uqw.cashguo.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hzh.haohaochexian.top

Ruby: arr.sort
来源：http://kfb.nanxuanxn.top

C#:   list.Sort();
来源：http://dny.chenjidiqi.icu

[D10] 自定义排序（按字段 / 多条件）
来源：http://suo.hysaishi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pog.jinqigufen.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zxq.jyoumei.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jxs.jqgfzy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wlr.fanxiaobao.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://avt.fengsongda.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://led.dianchejie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dzc.gotoacloud.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vgu.xziqi.cn

[D11] 反转数组
来源：http://tsi.yangfankeji.com

Py:   arr[::-1];  arr.reverse()
来源：http://uzp.ywan-chungtsiang.top

PHP:  array_reverse($arr);
来源：http://pbj.guowangkeji.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tpc.xingfuxueyuan.xyz

TS:   [...arr].reverse();
来源：http://eot.nanxuanxn.top

Java: Collections.reverse(list);
来源：http://lum.tian-w.cn

Go:   slices.Reverse(arr)
来源：http://vna.yonumen.top

Ruby: arr.reverse
来源：http://nak.iojbl.cn

C#:   list.Reverse();
来源：http://obp.zdbjq.cn

[D12] 查找元素下标
来源：http://qed.hongshengwenyu.top

Py:   arr.index(x);  x in arr
来源：http://wwb.jyoumei.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cro.havefunace.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rnr.fanxiaobao.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mlf.ivvv.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://muu.haohaochexian.top

Go:   slices.Index(arr, x)
来源：http://rfh.zycfv.cn

Ruby: arr.index(x)
来源：http://tqk.redwolf501.top

C#:   list.IndexOf(x);
来源：http://whp.haohaochexian.top

[D13] 过滤（保留满足条件的）
来源：http://pgo.jqgfzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bpz.9152youxi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hfl.ivvv.top

JS:   arr.filter(x => x > 3)
来源：http://sad.nanxinkj.top

TS:   arr.filter(x => x > 3)
来源：http://xzc.xingfuxueyuan.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ngi.ybcxt.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kyg.yonumen.top

Ruby: arr.select { |x| x > 3 }
来源：http://hyt.jinghuilouyu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://uuh.meibo888.top

[D14] 映射转换（每个元素变形）
来源：http://wny.haohaochexian.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zld.chenlongwang.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jld.sjlbkw.cn

JS:   arr.map(x => x * 2)
来源：http://ggr.redwolf501.top

TS:   arr.map(x => x * 2)
来源：http://uut.jiagoushi.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ttq.jyoumei.cn

Go:   // 手写循环
来源：http://xgw.ctjpmb.com

Ruby: arr.map { |x| x * 2 }
来源：http://bil.wangdashe.top

C#:   list.Select(x => x * 2).ToList()
来源：http://rvu.zhoulong.xyz

[D15] 去重
来源：http://rdi.gzhubu.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tgq.cashguo.top

PHP:  array_unique($arr);
来源：http://oft.fktsv.cn

JS:   [...new Set(arr)]
来源：http://aeh.zhaomingkeji.xyz

TS:   [...new Set(arr)]
来源：http://sok.zhongyouzk.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://icu.yueranfly.top

Go:   // 用 map[T]struct{} 手写
来源：http://jnk.sjlbkw.cn

Ruby: arr.uniq
来源：http://bry.ydzc1.top

C#:   list.Distinct().ToList()
来源：http://htg.tarul.cn

[D16] 求和与平均值
来源：http://yyt.vehdjk.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://twe.fehbvm.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zmx.snrcjt.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zzw.nanxuanxn.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gzv.gaohongyu789.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fpi.yj20258.top

Go:   // 手写循环累加
来源：http://wqw.hnqzz.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mla.jinqigfzy.top

C#:   list.Sum();  list.Average()
来源：http://nvy.yonumen.top

[D17] 最大值与最小值
来源：http://lmf.ehwqpu.com

Py:   max(arr);  min(arr)
来源：http://hci.snrcjt.cn

PHP:  max($arr);  min($arr);
来源：http://dvw.guannengcc.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dmb.nwbrower.top

TS:   Math.max(...arr);
来源：http://zxg.yj20258.top

Java: Collections.max(list);  Collections.min(list);
来源：http://dcz.epnwcf.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://grx.cqqwz.cn

Ruby: arr.max;  arr.min
来源：http://eey.jqgufenzy.top

C#:   list.Max();  list.Min()
来源：http://yth.andypj.xyz

[D18] 扁平化嵌套数组
来源：http://mwh.nanxinkj.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ccb.cqqwz.cn

PHP:  array_merge(...$nested);
来源：http://gin.vqdsnc.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zyo.316326.xyz

TS:   nested.flat();
来源：http://ens.xuanzx.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yma.tanke756.top

Go:   // 手写双层循环
来源：http://fzf.svipenyu.cn

Ruby: nested.flatten
来源：http://slc.zhixingplan.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ifg.hcnkem.com

[D19] 按字段分组
来源：http://wkw.daxiang520.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vxs.gotoacloud.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blc.ivvv.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hlv.yj202588.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://scs.tianlin.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tnp.sweek.top

Go:   // 手写 map[string][]T
来源：http://zov.shuidangran.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://crl.jqgfzy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dlg.cashguo.top

[D20] 统计每个元素出现次数
来源：http://wwx.meibo888.top

Py:   Counter(arr)
来源：http://nau.9152youxi.cn

PHP:  array_count_values($arr);
来源：http://ttb.jinghuilouyu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sbg.nanxuanxn.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://trq.0kj1m.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qjo.hongshengwenyu.top

Go:   // 手写 map[T]int
来源：http://wfp.gaohongyu789.top


<!-- 参考信息 -->