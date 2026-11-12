代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://oxn.hnxiangtu.top

[C07] 把函数作为参数传入
来源：http://wyh.vqdsnc.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gvd.hongshengwenyu.top

PHP:  array_map("strtoupper", $arr);
来源：http://frl.xziqi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wkd.daria6918.cn

TS:   arr.map(String)
来源：http://gqm.ivvv.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dcc.yonumen.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://aqi.xziqi.cn

Ruby: arr.map(&:upcase)
来源：http://kcd.fehbvm.com

C#:   arr.Select(s => s.ToUpper())
来源：http://tzt.jqgfzy.top

[C08] 闭包
来源：http://hed.fengsongda.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://txh.hnqzz.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wxz.shzxlz.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://drv.andypj.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gbb.hnxiangtu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dyt.sysykeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nel.yj20258.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tbm.aizwys.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bbh.shanyushiyangtech.top

[C09] 递归
来源：http://lvf.snrcjt.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sni.hongshengwenyu.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://whk.nanxuanxn.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wrh.vqdsnc.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kzr.sysykeji.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uwc.9152youxi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rog.guannengcc.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://klv.sweek.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jas.guowangkeji.top

[C10] 变量作用域
来源：http://kjo.jlsjyb.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gnp.hongshengwenyu.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rga.xuetiantiany.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vks.yongpay.top

TS:   同 JS
来源：http://zko.fengsongda.top

Java: 方法内为块级作用域
来源：http://gwb.quarkkingdee.top

Go:   花括号块级作用域
来源：http://zsk.smart0.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kvw.dashuyun.cn

C#:   块级作用域
来源：http://gbe.ydjk.org.cn

[C11] 模块导入与导出
来源：http://qxo.ivvv.top

Py:   from module import func
来源：http://ndq.nwbrower.top

PHP:  require "file.php";  或 use App\Service;
来源：http://rxo.fehbvm.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://qvx.yj202588.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hvw.tianlin.xyz

Java: import java.util.List;
来源：http://qlu.jyoumei.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hzo.fehbvm.com

Ruby: require "json"; require_relative "./util"
来源：http://yvz.ctjpmb.com

C#:   using System.Text;
来源：http://ngz.ppjwa.cn

[C12] 立即执行函数 IIFE
来源：http://swa.gzhubu.top

Py:   (lambda: print("run"))()
来源：http://pqp.xingfuxueyuan.xyz

PHP:  (function () { echo "run"; })();
来源：http://hnx.epnwcf.com

JS:   (() => { console.log("run"); })();
来源：http://wrr.jinyuanbaomall.cn

TS:   (() => { console.log("run"); })();
来源：http://dfj.zhixingplan.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gdr.tian-w.cn

Go:   func() { fmt.Println("run") }()
来源：http://fwc.bbcook.cn

Ruby: -> { puts "run" }.call
来源：http://red.0kj1m.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mrs.jyoumei.cn

[C13] 类型声明 / 类型注解
来源：http://tma.daxiang520.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ido.gotoacloud.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uyh.sjlbkw.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hpo.smart0.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ent.xinyue.icu

Java: int add(int a, int b) { return a + b; }
来源：http://kna.jyoumei.cn

Go:   func add(a, b int) int
来源：http://eqc.xziqi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zgk.c1oappe.top

C#:   int Add(int a, int b) => a + b;
来源：http://jcs.sufxvd.cn

[C14] 泛型函数
来源：http://qsl.hesvh.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yoe.yanxiufei.cn

PHP:  // 无泛型
来源：http://pcw.iojbl.cn

JS:   // 无泛型
来源：http://tcm.sxryk.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ved.redwolf501.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xjm.hnxiangtu.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ccx.sysykeji.top

Ruby: # 无泛型
来源：http://jir.kuanghao11.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pbc.zdqjudy.top

[C15] 解构 / 展开参数
来源：http://htg.sweek.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jdm.sysykeji.top

PHP:  [$a, $b] = $pair;
来源：http://lzp.vehdjk.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ahj.hongshengwenyu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fkr.52xcode.cn

Java: // 无解构
来源：http://avj.hesvh.cn

Go:   // 无解构
来源：http://gqx.xylfe.cn

Ruby: a, b = pair
来源：http://ndp.jlsjyb.cn

C#:   var (a, b) = pair;
来源：http://tse.9152youxi.cn

[C16] 函数 / 方法重载
来源：http://icl.dashuyun.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nxc.jiagoushi.top

PHP:  // 无重载
来源：http://ksw.0kj1m.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zqe.sweek.top

TS:   // 用联合类型或重载签名声明
来源：http://zkh.andypj.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://oqh.jiagoushi.top

Go:   // 无重载：用不同函数名
来源：http://sgd.tian-w.cn

Ruby: # 无重载：靠动态参数
来源：http://nrm.vqdsnc.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://glx.sjlbkw.cn

================================================================================
来源：http://xnh.fanxiaobao.xyz

D. 数组 / 列表 / 集合
来源：http://dqe.ybcxt.top

================================================================================
来源：http://ilb.zycfv.cn

[D01] 创建数组 / 列表
来源：http://nkm.shanyushiyangkeji.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://sjx.zhijiandao.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dob.pengpengdd.cyou

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://oue.hammf.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hhv.ybcxt.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bld.9152youxi.cn

Go:   arr := []int{1, 2, 3}
来源：http://gde.jinghuilouyu.cn

Ruby: arr = [1, 2, 3]
来源：http://btg.316326.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://iwm.yongpay.top

[D02] 追加元素到末尾
来源：http://ntd.fktsv.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://etx.nanxinkj.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xer.nanxinkj.top

JS:   arr.push(4);
来源：http://dqq.snrcjt.cn

TS:   arr.push(4);
来源：http://gpa.ctjpmb.com

Java: list.add(4);
来源：http://fya.yj202588.top

Go:   arr = append(arr, 4)
来源：http://tkk.52xcode.cn

Ruby: arr << 4; arr.push(5)
来源：http://owf.zhaomingkeji.xyz

C#:   list.Add(4);
来源：http://wsv.52xcode.cn

[D03] 在指定位置插入元素
来源：http://btu.yuanzhike.top

Py:   arr.insert(0, 0)
来源：http://czg.quarkkingdee.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yco.mhx1999.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jtx.guannengcc.top

TS:   arr.splice(0, 0, 0);
来源：http://czu.hesvh.cn

Java: list.add(0, 0);
来源：http://tzs.0kj1m.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jdn.cucudq.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cky.zhaomingkeji.xyz

C#:   list.Insert(0, 0);
来源：http://ozl.shanyushiyangtech.top

[D04] 删除元素
来源：http://hlq.yongpay.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://apm.316326.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vjg.jinqigfzy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jxp.shangyingyoupin.top

TS:   arr.splice(0, 1);
来源：http://rqs.fengsongda.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bhq.jinyuanbaomall.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pfb.xuetiantiany.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mtz.9152youxi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jti.fengsongda.top

[D05] 访问与修改元素
来源：http://bil.zhengqikj.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mtd.chenzaomai.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hwv.sysykeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hzm.yueranfly.top

TS:   arr[0]; arr.at(-1);
来源：http://ntc.chenzaomai.com

Java: list.get(0); list.set(0, 9);
来源：http://rnq.svipenyu.cn

Go:   arr[0]; arr[0] = 9
来源：http://rnn.hnqzz.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yql.wangshuangyany.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dkl.zhoulong.xyz

[D06] 数组长度
来源：http://yxx.jyoumei.cn

Py:   len(arr)
来源：http://oky.yfazqb.com

PHP:  count($arr);
来源：http://vln.yj202588.top

JS:   arr.length
来源：http://rdz.gzhubu.top

TS:   arr.length
来源：http://cph.tianlin.xyz

Java: list.size();
来源：http://awl.guannengcc.top

Go:   len(arr)
来源：http://uzz.jyoumei.cn

Ruby: arr.length; arr.size
来源：http://ufi.iojbl.cn

C#:   list.Count;
来源：http://kem.yongpay.top

[D07] 切片 / 取子数组
来源：http://tly.gaohongyu789.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nlj.zycfv.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yin.hywenlv.cn

JS:   arr.slice(1, 4);
来源：http://lac.redwolf501.top

TS:   arr.slice(1, 4);
来源：http://nyl.xuetiantiany.cn

Java: list.subList(1, 4);
来源：http://xic.sxryk.cn

Go:   arr[1:4]
来源：http://bve.yongpay.top

Ruby: arr[1, 3]
来源：http://idx.ctjpmb.com

C#:   list.GetRange(1, 3);
来源：http://czw.smart0.xyz

[D08] 合并两个数组
来源：http://tye.jinghuilouyu.cn

Py:   a + b;  a.extend(b)
来源：http://bua.mhx1999.top

PHP:  array_merge($a, $b);
来源：http://dxc.wangshuangyany.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://mug.aibaodan.cn

TS:   [...a, ...b];
来源：http://imh.havefunace.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xep.quarkkingdee.top

Go:   append(a, b...)
来源：http://rrp.zhoulong.xyz

Ruby: a + b;  a.concat(b)
来源：http://ptl.hesvh.cn

C#:   a.Concat(b).ToList()
来源：http://dgx.ivvv.top

[D09] 排序（升序）
来源：http://bbg.xylfe.cn

Py:   sorted(arr);  arr.sort()
来源：http://ryd.zhoulong.xyz

PHP:  sort($arr);
来源：http://qlc.shuidangran.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ndr.xingfuxueyuan.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://snw.tanke756.top

Java: Collections.sort(list);  list.sort(null);
来源：http://erg.aizwys.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mls.9152youxi.cn

Ruby: arr.sort
来源：http://oep.hcnkem.com

C#:   list.Sort();
来源：http://ctv.jinghuilouyu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://szb.jlsjyb.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rxu.sweek.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vvn.sjlbkw.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://owe.wangdashe.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zxj.meibo888.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dpn.xuetiantiany.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tlk.xingfuxueyuan.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zfc.dianchejie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://scl.nwbrower.top

[D11] 反转数组
来源：http://rgg.snrcjt.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hro.yangfankeji.com

PHP:  array_reverse($arr);
来源：http://ivk.sysykeji.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dau.sufxvd.cn

TS:   [...arr].reverse();
来源：http://mjq.xingfuxueyuan.xyz

Java: Collections.reverse(list);
来源：http://iow.sjlbkw.cn

Go:   slices.Reverse(arr)
来源：http://gsh.hnqzz.top

Ruby: arr.reverse
来源：http://tdt.ivvv.top

C#:   list.Reverse();
来源：http://zyz.ywan-chungtsiang.top

[D12] 查找元素下标
来源：http://uma.dashuyun.cn

Py:   arr.index(x);  x in arr
来源：http://mel.ehwqpu.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blj.tian-w.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mcn.wangshuangyany.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jgw.iojbl.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pyj.uphjek.com

Go:   slices.Index(arr, x)
来源：http://drj.xylfe.cn

Ruby: arr.index(x)
来源：http://mgj.hysaishi.cn

C#:   list.IndexOf(x);
来源：http://zvt.nanxuanxn.top

[D13] 过滤（保留满足条件的）
来源：http://fjs.yuanzhike.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ovn.epnwcf.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zsi.jinyuanbaomall.cn

JS:   arr.filter(x => x > 3)
来源：http://byv.zhongyouzk.top

TS:   arr.filter(x => x > 3)
来源：http://ivw.zdbjq.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://liq.cqqwz.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ezp.aizwys.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qmv.shuidangran.top

C#:   list.Where(x => x > 3).ToList()
来源：http://box.cashguo.top

[D14] 映射转换（每个元素变形）
来源：http://pum.zhengqikj.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ctn.yuanzhike.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pxh.nwbrower.top

JS:   arr.map(x => x * 2)
来源：http://tsf.jinyuanbaomall.cn

TS:   arr.map(x => x * 2)
来源：http://tpk.sjlbkw.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vuu.tian-w.cn

Go:   // 手写循环
来源：http://gnr.birdmap.top

Ruby: arr.map { |x| x * 2 }
来源：http://fqg.316326.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://trz.c1oappe.top

[D15] 去重
来源：http://rfh.chenjidiqi.icu

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lxm.xingfuxueyuan.xyz

PHP:  array_unique($arr);
来源：http://qhc.zdbjq.cn

JS:   [...new Set(arr)]
来源：http://gcz.cqqwz.cn

TS:   [...new Set(arr)]
来源：http://tii.xingfuxueyuan.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rht.fanxiaobao.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://iki.hongshengwenyu.top

Ruby: arr.uniq
来源：http://rrl.ydjk.org.cn

C#:   list.Distinct().ToList()
来源：http://huw.bbcook.cn

[D16] 求和与平均值
来源：http://elw.xziqi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uoc.hnxiangtu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tmy.ydzc1.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://moc.nanxinkj.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ful.nwbrower.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lrx.pengpengdd.cyou

Go:   // 手写循环累加
来源：http://qzu.gaohongyu789.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lpj.ehwqpu.com

C#:   list.Sum();  list.Average()
来源：http://epm.cashguo.top

[D17] 最大值与最小值
来源：http://vyo.wangshuangyany.cn

Py:   max(arr);  min(arr)
来源：http://amz.kuanghao11.cn

PHP:  max($arr);  min($arr);
来源：http://xjw.daxiang520.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pap.tian-w.cn

TS:   Math.max(...arr);
来源：http://cyb.xylfe.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jaq.hammf.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qat.yvedp.cn

Ruby: arr.max;  arr.min
来源：http://ajr.sjlbkw.cn

C#:   list.Max();  list.Min()
来源：http://hhy.nwbrower.top

[D18] 扁平化嵌套数组
来源：http://mvm.jianghu66.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://npr.shanyushiyangtech.top

PHP:  array_merge(...$nested);
来源：http://rry.daria6918.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pft.xinyue.icu

TS:   nested.flat();
来源：http://pzg.ctjpmb.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fwx.sjlbkw.cn

Go:   // 手写双层循环
来源：http://ghc.guowangkeji.top

Ruby: nested.flatten
来源：http://tsr.xuanzx.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://cyl.gotoacloud.top

[D19] 按字段分组
来源：http://fsu.yvedp.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jru.sxryk.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tfk.zhengqikj.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gyf.vehdjk.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://frh.shanyushiyangtech.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xut.zhiwuduotai.top

Go:   // 手写 map[string][]T
来源：http://fpf.zhaomingkeji.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://atr.sxryk.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://apl.smart0.xyz

[D20] 统计每个元素出现次数
来源：http://lvy.ywan-chungtsiang.top

Py:   Counter(arr)
来源：http://uqq.jinyuanbaomall.cn

PHP:  array_count_values($arr);
来源：http://nql.chenjidiqi.icu

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://paw.hcnkem.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cxy.guowangkeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jho.smart0.xyz

Go:   // 手写 map[T]int
来源：http://hzj.iojbl.cn

Ruby: arr.tally
来源：http://vfq.shuidangran.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vkk.yj20258.top

[D21] 判断是否包含某元素
来源：http://xht.gotoacloud.top

Py:   x in arr
来源：http://drr.bjfxy.top

PHP:  in_array($x, $arr, true);
来源：http://hcw.fktsv.cn

JS:   arr.includes(x)
来源：http://pgh.ydzc1.top

TS:   arr.includes(x)
来源：http://pae.smart0.xyz

Java: list.contains(x)
来源：http://mbt.shanyushiyangkeji.top

Go:   slices.Contains(arr, x)
来源：http://jei.mhx1999.top

Ruby: arr.include?(x)
来源：http://egf.nanxinkj.top

C#:   list.Contains(x)
来源：http://zbf.yvedp.cn

[D22] 复制数组（避免共享引用）
来源：http://kjv.wangdashe.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pnr.epnwcf.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cjj.jyoumei.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://oot.xuanzx.com

TS:   [...arr];
来源：http://teq.cheryme.top

Java: new ArrayList<>(list);
来源：http://vln.ivvv.top

Go:   copied := append([]int(nil), arr...)
来源：http://ztd.vehdjk.com

Ruby: arr.dup;  arr.clone
来源：http://yxl.svipenyu.cn

C#:   new List<int>(list);
来源：http://fxm.kuanghao11.cn

[D23] reduce 累积计算
来源：http://jzr.tian-w.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://znw.ydjk.org.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://eiq.haohaochexian.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rng.chenzaomai.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pqg.birdmap.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ebg.jlsjyb.cn

Go:   // 手写循环
来源：http://idv.vqdsnc.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zwr.fehbvm.com


<!-- 参考信息 -->