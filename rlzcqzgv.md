代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://fqe.fengsongda.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sau.jinqigufen.top

Go:   sq := func(x int) int { return x * x }
来源：http://rbq.xinyue.icu

Ruby: square = ->(x) { x * x }
来源：http://lzh.ybcxt.top

C#:   Func<int, int> square = x => x * x;
来源：http://est.chenlongwang.top

[C07] 把函数作为参数传入
来源：http://bla.yongpay.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://psx.smart0.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://dpj.feifeiyinyue.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hdo.tianlin.xyz

TS:   arr.map(String)
来源：http://svx.yfazqb.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qfy.yfazqb.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://trc.fktsv.cn

Ruby: arr.map(&:upcase)
来源：http://glq.0kj1m.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xbk.quarkkingdee.top

[C08] 闭包
来源：http://dti.cheryme.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://klh.meibo888.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tyc.zhijiandao.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ilm.jyoumei.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fan.kuanghao11.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pgu.shanyushiyangtech.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tnp.nanxuanxn.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gqr.nanxinkj.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ibr.meibo888.top

[C09] 递归
来源：http://vag.haohaochexian.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://owx.dashuyun.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bak.hammf.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://juv.hywenlv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ggl.wangshuangyany.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cdk.yvedp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ywr.ctjpmb.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mtu.jinqigfzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fkj.xingfuxueyuan.xyz

[C10] 变量作用域
来源：http://whv.cheryme.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lzv.hnxiangtu.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://slr.316326.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hvh.fengsongda.top

TS:   同 JS
来源：http://mbf.hongshengwenyu.top

Java: 方法内为块级作用域
来源：http://pvp.yangfankeji.com

Go:   花括号块级作用域
来源：http://vfs.9152youxi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gus.ydjk.org.cn

C#:   块级作用域
来源：http://ays.ydzc1.top

[C11] 模块导入与导出
来源：http://eft.fktsv.cn

Py:   from module import func
来源：http://vnl.fanxiaobao.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://pxo.nwbrower.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://asl.hnxiangtu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cwe.fzhhl.top

Java: import java.util.List;
来源：http://igz.uphjek.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fme.birdmap.top

Ruby: require "json"; require_relative "./util"
来源：http://cry.9152youxi.cn

C#:   using System.Text;
来源：http://rtr.iojbl.cn

[C12] 立即执行函数 IIFE
来源：http://pti.redwolf501.top

Py:   (lambda: print("run"))()
来源：http://cgs.jqgfzy.top

PHP:  (function () { echo "run"; })();
来源：http://glx.yj202588.top

JS:   (() => { console.log("run"); })();
来源：http://ttu.shanyushiyangtech.top

TS:   (() => { console.log("run"); })();
来源：http://xxx.zhongyouzk.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://csu.0kj1m.cn

Go:   func() { fmt.Println("run") }()
来源：http://ppc.birdmap.top

Ruby: -> { puts "run" }.call
来源：http://uqc.jianghu66.top

C#:   // 无 IIFE：用静态构造函数
来源：http://xar.yonumen.top

[C13] 类型声明 / 类型注解
来源：http://kos.zhaomingkeji.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qnk.fzhhl.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sqa.sysykeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wlq.dashuyun.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qip.quarkkingdee.top

Java: int add(int a, int b) { return a + b; }
来源：http://vil.vehdjk.com

Go:   func add(a, b int) int
来源：http://ycj.sufxvd.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dne.zycfv.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cyr.sjlbkw.cn

[C14] 泛型函数
来源：http://nqa.fktsv.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qjm.daxiang520.top

PHP:  // 无泛型
来源：http://iif.yangfankeji.com

JS:   // 无泛型
来源：http://tlw.xziqi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://aga.jinghuilouyu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fmn.shangyingyoupin.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cbv.yj20258888.top

Ruby: # 无泛型
来源：http://eil.tianlin.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mbv.xinyue.icu

[C15] 解构 / 展开参数
来源：http://src.yfazqb.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tua.hcnkem.com

PHP:  [$a, $b] = $pair;
来源：http://csa.dashuyun.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rbz.chenzaomai.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mmb.uphjek.com

Java: // 无解构
来源：http://doo.yanxiufei.cn

Go:   // 无解构
来源：http://aek.zdbjq.cn

Ruby: a, b = pair
来源：http://wvc.daria6918.cn

C#:   var (a, b) = pair;
来源：http://ugb.quarkkingdee.top

[C16] 函数 / 方法重载
来源：http://but.yj20258888.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://arl.ivvv.top

PHP:  // 无重载
来源：http://wdw.guannengcc.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://deb.fengsongda.top

TS:   // 用联合类型或重载签名声明
来源：http://arm.sufxvd.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://quj.zhiwuduotai.top

Go:   // 无重载：用不同函数名
来源：http://kul.xingfuxueyuan.xyz

Ruby: # 无重载：靠动态参数
来源：http://fpx.fehbvm.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://img.yj20258888.top

================================================================================
来源：http://gqx.xingfuxueyuan.xyz

D. 数组 / 列表 / 集合
来源：http://rjk.zdqjudy.top

================================================================================
来源：http://sve.bjfxy.top

[D01] 创建数组 / 列表
来源：http://gwi.guannengcc.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://fni.yj20258888.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kge.sufxvd.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fgv.zhengqikj.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://khr.9152youxi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://res.iojbl.cn

Go:   arr := []int{1, 2, 3}
来源：http://ohp.shuidangran.top

Ruby: arr = [1, 2, 3]
来源：http://qtt.shuidangran.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://uxi.jinyuanbaomall.cn

[D02] 追加元素到末尾
来源：http://uww.xziqi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ncr.xuetiantiany.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nac.xuanzx.com

JS:   arr.push(4);
来源：http://qta.dashuyun.cn

TS:   arr.push(4);
来源：http://ukx.sxryk.cn

Java: list.add(4);
来源：http://eln.cqqwz.cn

Go:   arr = append(arr, 4)
来源：http://kol.yj20258888.top

Ruby: arr << 4; arr.push(5)
来源：http://daa.hywenlv.cn

C#:   list.Add(4);
来源：http://qxk.xylfe.cn

[D03] 在指定位置插入元素
来源：http://cif.ehwqpu.com

Py:   arr.insert(0, 0)
来源：http://hjp.haohaochexian.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xap.cashguo.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qde.xingfuxueyuan.xyz

TS:   arr.splice(0, 0, 0);
来源：http://eqr.jiagoushi.top

Java: list.add(0, 0);
来源：http://xmy.daxiang520.top

Go:   arr = append([]int{0}, arr...)
来源：http://gis.nanxuanxn.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lra.ybcxt.top

C#:   list.Insert(0, 0);
来源：http://vfm.iojbl.cn

[D04] 删除元素
来源：http://ijy.cdnleiting.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ybf.xuanzx.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fyc.quarkkingdee.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zvn.cashguo.top

TS:   arr.splice(0, 1);
来源：http://kor.snrcjt.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nsu.yanxiufei.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fti.0kj1m.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cwg.shzxlz.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jld.ydzc1.top

[D05] 访问与修改元素
来源：http://alp.xuanzx.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yzc.c1oappe.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yfx.zycfv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fpx.bjfxy.top

TS:   arr[0]; arr.at(-1);
来源：http://yfm.wangdashe.top

Java: list.get(0); list.set(0, 9);
来源：http://les.dianchejie.cn

Go:   arr[0]; arr[0] = 9
来源：http://gnc.feifeiyinyue.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kzm.hongshengwenyu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://avf.ctjpmb.com

[D06] 数组长度
来源：http://yxm.hysaishi.cn

Py:   len(arr)
来源：http://vua.guowangkeji.top

PHP:  count($arr);
来源：http://nke.yfazqb.com

JS:   arr.length
来源：http://lom.feifeiyinyue.top

TS:   arr.length
来源：http://wkn.xinyue.icu

Java: list.size();
来源：http://jbl.yuxming.cn

Go:   len(arr)
来源：http://sik.daxiang520.top

Ruby: arr.length; arr.size
来源：http://rzm.sufxvd.cn

C#:   list.Count;
来源：http://cxv.pycfn.com

[D07] 切片 / 取子数组
来源：http://pda.316326.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fkn.uphjek.com

PHP:  array_slice($arr, 1, 3);
来源：http://nye.gogol.net.cn

JS:   arr.slice(1, 4);
来源：http://qkq.hnqzz.top

TS:   arr.slice(1, 4);
来源：http://ora.zhijiandao.cn

Java: list.subList(1, 4);
来源：http://adi.yj202588.top

Go:   arr[1:4]
来源：http://hnt.sxryk.cn

Ruby: arr[1, 3]
来源：http://apd.yongpay.top

C#:   list.GetRange(1, 3);
来源：http://uiy.tianlin.xyz

[D08] 合并两个数组
来源：http://ydl.zdbjq.cn

Py:   a + b;  a.extend(b)
来源：http://hwe.dashuyun.cn

PHP:  array_merge($a, $b);
来源：http://wch.aizwys.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://dij.bbcook.cn

TS:   [...a, ...b];
来源：http://ubb.xuetiantiany.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bys.birdmap.top

Go:   append(a, b...)
来源：http://rir.yuanzhike.top

Ruby: a + b;  a.concat(b)
来源：http://hlg.tianlin.xyz

C#:   a.Concat(b).ToList()
来源：http://hiw.ehwqpu.com

[D09] 排序（升序）
来源：http://dtk.cashguo.top

Py:   sorted(arr);  arr.sort()
来源：http://hhb.jiagoushi.top

PHP:  sort($arr);
来源：http://fbe.jqgfzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kvy.gotoacloud.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://icj.daria6918.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://pjm.epnwcf.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mus.zhongyouzk.top

Ruby: arr.sort
来源：http://aik.jinqigfzy.top

C#:   list.Sort();
来源：http://kol.vehdjk.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://gif.kuanghao11.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://drd.yfazqb.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kpm.tian-w.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://khu.zhiwuduotai.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tdn.hywenlv.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://btk.hongshengwenyu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xmo.zdqjudy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kmi.daria6918.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://agy.guannengcc.top

[D11] 反转数组
来源：http://kmf.aibaodan.cn

Py:   arr[::-1];  arr.reverse()
来源：http://vts.uphjek.com

PHP:  array_reverse($arr);
来源：http://pbf.yj202588.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://erp.xylfe.cn

TS:   [...arr].reverse();
来源：http://ioy.havefunace.top

Java: Collections.reverse(list);
来源：http://lej.jinyuanbaomall.cn

Go:   slices.Reverse(arr)
来源：http://lxg.hcnkem.com

Ruby: arr.reverse
来源：http://iji.hcnkem.com

C#:   list.Reverse();
来源：http://aia.wangshuangyany.cn

[D12] 查找元素下标
来源：http://egu.ydjk.org.cn

Py:   arr.index(x);  x in arr
来源：http://hoc.jinyuanbaomall.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zem.ydjk.org.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lsy.ppjwa.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zwj.hywenlv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://owx.tian-w.cn

Go:   slices.Index(arr, x)
来源：http://ejn.aibaodan.cn

Ruby: arr.index(x)
来源：http://bbn.ehwqpu.com

C#:   list.IndexOf(x);
来源：http://fnw.ybcxt.top

[D13] 过滤（保留满足条件的）
来源：http://irf.fzhhl.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zcy.chenzaomai.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://arv.fktsv.cn

JS:   arr.filter(x => x > 3)
来源：http://soe.fktsv.cn

TS:   arr.filter(x => x > 3)
来源：http://poa.nanxuanxn.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tia.kuanghao11.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qzt.ivvv.top

Ruby: arr.select { |x| x > 3 }
来源：http://eyg.hammf.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vvg.316326.xyz

[D14] 映射转换（每个元素变形）
来源：http://meg.ydjk.org.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://por.quarkkingdee.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zgg.jiagoushi.top

JS:   arr.map(x => x * 2)
来源：http://ggs.andypj.xyz

TS:   arr.map(x => x * 2)
来源：http://ame.jqgufenzy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://apm.sxryk.cn

Go:   // 手写循环
来源：http://axi.zdqjudy.top

Ruby: arr.map { |x| x * 2 }
来源：http://fnw.ctjpmb.com

C#:   list.Select(x => x * 2).ToList()
来源：http://vux.bbcook.cn

[D15] 去重
来源：http://gbr.jianghu66.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cjv.fzhhl.top

PHP:  array_unique($arr);
来源：http://njm.yueranfly.top

JS:   [...new Set(arr)]
来源：http://oxq.chenjidiqi.icu

TS:   [...new Set(arr)]
来源：http://gff.hysaishi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fvf.yanxiufei.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ydh.yj20258.top

Ruby: arr.uniq
来源：http://kkk.yfazqb.com

C#:   list.Distinct().ToList()
来源：http://rht.zdbjq.cn

[D16] 求和与平均值
来源：http://csb.bbcook.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://iqr.c1oappe.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bcq.tianlin.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wdb.cdnleiting.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qtf.cashguo.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fel.jlsjyb.cn

Go:   // 手写循环累加
来源：http://lbp.yonumen.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zoi.zhongyouzk.top

C#:   list.Sum();  list.Average()
来源：http://mwx.jinyuanbaomall.cn

[D17] 最大值与最小值
来源：http://lfd.hysaishi.cn

Py:   max(arr);  min(arr)
来源：http://zgc.ivvv.top

PHP:  max($arr);  min($arr);
来源：http://pfa.jlsjyb.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://eiy.xylfe.cn

TS:   Math.max(...arr);
来源：http://bph.aizwys.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://kgz.xziqi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://oag.pycfn.com

Ruby: arr.max;  arr.min
来源：http://hww.zhaomingkeji.xyz

C#:   list.Max();  list.Min()
来源：http://plb.havefunace.top

[D18] 扁平化嵌套数组
来源：http://wow.fktsv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tba.cheryme.top

PHP:  array_merge(...$nested);
来源：http://xav.jinqigfzy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rns.ivvv.top

TS:   nested.flat();
来源：http://kbf.xylfe.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mcq.52xcode.cn

Go:   // 手写双层循环
来源：http://qni.jqgufenzy.top

Ruby: nested.flatten
来源：http://msh.jinyuanbaomall.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://jfl.yongpay.top

[D19] 按字段分组
来源：http://crf.smart0.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://btl.ydzc1.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bjv.zhaomingkeji.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gmc.pycfn.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://sem.uphjek.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oxa.zhiwuduotai.top

Go:   // 手写 map[string][]T
来源：http://sot.tarul.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://iao.bbcook.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ale.birdmap.top

[D20] 统计每个元素出现次数
来源：http://zdf.zycfv.cn

Py:   Counter(arr)
来源：http://nxe.tanke756.top

PHP:  array_count_values($arr);
来源：http://dja.fehbvm.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hqw.redwolf501.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xjf.jinyuanbaomall.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zkv.smart0.xyz

Go:   // 手写 map[T]int
来源：http://fuf.cucudq.cn

Ruby: arr.tally
来源：http://xfg.sweek.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dgf.316326.xyz

[D21] 判断是否包含某元素
来源：http://wva.sweek.top

Py:   x in arr
来源：http://wrm.shanyushiyangtech.top

PHP:  in_array($x, $arr, true);
来源：http://jct.hywenlv.cn

JS:   arr.includes(x)
来源：http://asf.guowangkeji.top

TS:   arr.includes(x)
来源：http://ayk.jinghuilouyu.cn

Java: list.contains(x)
来源：http://tju.bjfxy.top

Go:   slices.Contains(arr, x)
来源：http://qmj.yuanzhike.top

Ruby: arr.include?(x)
来源：http://fup.xylfe.cn

C#:   list.Contains(x)
来源：http://ttp.xylfe.cn

[D22] 复制数组（避免共享引用）
来源：http://nqb.pengpengdd.cyou

Py:   arr.copy();  arr[:];  list(arr)
来源：http://enr.havefunace.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tdb.pycfn.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ogh.zhengqikj.top

TS:   [...arr];
来源：http://nac.zdbjq.cn

Java: new ArrayList<>(list);
来源：http://pko.sxryk.cn

Go:   copied := append([]int(nil), arr...)
来源：http://iwn.mhx1999.top

Ruby: arr.dup;  arr.clone
来源：http://skq.jianghu66.top

C#:   new List<int>(list);
来源：http://wvx.gogol.net.cn

[D23] reduce 累积计算
来源：http://gql.0kj1m.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gap.bbcook.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qtj.xziqi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://myx.zdqjudy.top


<!-- 参考信息 -->