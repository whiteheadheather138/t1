代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://fqj.shangyingyoupin.top

C#:   arr.Select(s => s.ToUpper())
来源：http://kqh.nwbrower.top

[C08] 闭包
来源：http://arj.ehwqpu.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wvq.bjfxy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://omr.vqdsnc.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rqf.ctjpmb.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gsn.dianchejie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mvo.ydjk.org.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lzg.9152youxi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wth.hysaishi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cll.redwolf501.top

[C09] 递归
来源：http://lbt.yonumen.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://euz.ctjpmb.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fck.jianghu66.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://src.wangdashe.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://orn.aibaodan.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gba.vqdsnc.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dhw.jqgfzy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lcx.cashguo.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://oxd.fktsv.cn

[C10] 变量作用域
来源：http://xrr.ybcxt.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xjw.chenzaomai.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gth.yj20258888.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xsg.yanxiufei.cn

TS:   同 JS
来源：http://gdf.hammf.cn

Java: 方法内为块级作用域
来源：http://qvq.fzhhl.top

Go:   花括号块级作用域
来源：http://pzc.hammf.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fwc.tian-w.cn

C#:   块级作用域
来源：http://wnh.dashuyun.cn

[C11] 模块导入与导出
来源：http://nur.aibaodan.cn

Py:   from module import func
来源：http://ees.daxiang520.top

PHP:  require "file.php";  或 use App\Service;
来源：http://mlh.xuanzx.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://zsi.zycfv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fye.zhixingplan.top

Java: import java.util.List;
来源：http://bkj.jlsjyb.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tmp.xingfuxueyuan.xyz

Ruby: require "json"; require_relative "./util"
来源：http://gxt.fktsv.cn

C#:   using System.Text;
来源：http://lpm.ybcxt.top

[C12] 立即执行函数 IIFE
来源：http://aza.ydjk.org.cn

Py:   (lambda: print("run"))()
来源：http://rlm.jinghuilouyu.cn

PHP:  (function () { echo "run"; })();
来源：http://ykp.jlsjyb.cn

JS:   (() => { console.log("run"); })();
来源：http://wfq.gogol.net.cn

TS:   (() => { console.log("run"); })();
来源：http://zjl.hammf.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://moq.daria6918.cn

Go:   func() { fmt.Println("run") }()
来源：http://lhb.nwbrower.top

Ruby: -> { puts "run" }.call
来源：http://kcm.iojbl.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://bga.havefunace.top

[C13] 类型声明 / 类型注解
来源：http://uea.zhengqikj.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://msm.yj20258888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dah.yvedp.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rrk.vqdsnc.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jtv.zhoulong.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://lew.yvedp.cn

Go:   func add(a, b int) int
来源：http://vjz.fehbvm.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vxh.sufxvd.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qjg.zhixingplan.top

[C14] 泛型函数
来源：http://yme.zhiwuduotai.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rov.svipenyu.cn

PHP:  // 无泛型
来源：http://uqd.aibaodan.cn

JS:   // 无泛型
来源：http://qlj.pycfn.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lsj.jqgufenzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ygn.hongshengwenyu.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ylu.svipenyu.cn

Ruby: # 无泛型
来源：http://gzy.jinqigfzy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yff.ivvv.top

[C15] 解构 / 展开参数
来源：http://kdq.yfazqb.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kmv.cucudq.cn

PHP:  [$a, $b] = $pair;
来源：http://bxj.nanxinkj.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ark.bjfxy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dcq.ivvv.top

Java: // 无解构
来源：http://zfp.wangshuangyany.cn

Go:   // 无解构
来源：http://xei.0kj1m.cn

Ruby: a, b = pair
来源：http://han.dashuyun.cn

C#:   var (a, b) = pair;
来源：http://tfx.hammf.cn

[C16] 函数 / 方法重载
来源：http://lfq.nanxuanxn.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://eno.zdbjq.cn

PHP:  // 无重载
来源：http://fom.hywenlv.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://cbx.zhoulong.xyz

TS:   // 用联合类型或重载签名声明
来源：http://ovl.316326.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://tdx.fktsv.cn

Go:   // 无重载：用不同函数名
来源：http://grn.dashuyun.cn

Ruby: # 无重载：靠动态参数
来源：http://vlw.ydzc1.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://juy.hammf.cn

================================================================================
来源：http://eyn.shzxlz.cn

D. 数组 / 列表 / 集合
来源：http://buu.epnwcf.com

================================================================================
来源：http://trl.yonumen.top

[D01] 创建数组 / 列表
来源：http://ofo.guowangkeji.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://zck.yvedp.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gkm.quarkkingdee.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lxg.hongshengwenyu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ftf.guowangkeji.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ruq.yonumen.top

Go:   arr := []int{1, 2, 3}
来源：http://ips.jqgufenzy.top

Ruby: arr = [1, 2, 3]
来源：http://dju.wangshuangyany.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gbt.bjfxy.top

[D02] 追加元素到末尾
来源：http://fbp.fanxiaobao.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://szk.guannengcc.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fnu.nwbrower.top

JS:   arr.push(4);
来源：http://sqb.birdmap.top

TS:   arr.push(4);
来源：http://zup.cashguo.top

Java: list.add(4);
来源：http://utk.yfazqb.com

Go:   arr = append(arr, 4)
来源：http://oik.ehwqpu.com

Ruby: arr << 4; arr.push(5)
来源：http://trd.shzxlz.cn

C#:   list.Add(4);
来源：http://qma.ctjpmb.com

[D03] 在指定位置插入元素
来源：http://gjx.smart0.xyz

Py:   arr.insert(0, 0)
来源：http://zlc.aibaodan.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cty.jinqigfzy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://old.c1oappe.top

TS:   arr.splice(0, 0, 0);
来源：http://eom.ehwqpu.com

Java: list.add(0, 0);
来源：http://pqh.andypj.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://kwt.yanxiufei.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qzl.yuxming.cn

C#:   list.Insert(0, 0);
来源：http://sgs.fehbvm.com

[D04] 删除元素
来源：http://jgg.svipenyu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ijo.ctjpmb.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mok.hywenlv.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://icl.shuidangran.top

TS:   arr.splice(0, 1);
来源：http://kwn.jinqigfzy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://atw.hnxiangtu.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ift.epnwcf.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tny.shangyingyoupin.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wlm.yuxming.cn

[D05] 访问与修改元素
来源：http://bus.xinyue.icu

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://twz.sysykeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dtk.xingfuxueyuan.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kfl.wangshuangyany.cn

TS:   arr[0]; arr.at(-1);
来源：http://stt.ybcxt.top

Java: list.get(0); list.set(0, 9);
来源：http://aqo.yfazqb.com

Go:   arr[0]; arr[0] = 9
来源：http://ikk.tanke756.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://aee.cdnleiting.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wat.sufxvd.cn

[D06] 数组长度
来源：http://xxc.daxiang520.top

Py:   len(arr)
来源：http://grc.zycfv.cn

PHP:  count($arr);
来源：http://ygp.hammf.cn

JS:   arr.length
来源：http://kxd.zhixingplan.top

TS:   arr.length
来源：http://ttk.wangshuangyany.cn

Java: list.size();
来源：http://zms.vqdsnc.cn

Go:   len(arr)
来源：http://ivn.xuetiantiany.cn

Ruby: arr.length; arr.size
来源：http://voj.yuxming.cn

C#:   list.Count;
来源：http://xnh.cashguo.top

[D07] 切片 / 取子数组
来源：http://wvn.c1oappe.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qvh.hesvh.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hin.pengpengdd.cyou

JS:   arr.slice(1, 4);
来源：http://nrx.pengpengdd.cyou

TS:   arr.slice(1, 4);
来源：http://cko.iojbl.cn

Java: list.subList(1, 4);
来源：http://dqt.xuanzx.com

Go:   arr[1:4]
来源：http://kws.mhx1999.top

Ruby: arr[1, 3]
来源：http://egj.yvedp.cn

C#:   list.GetRange(1, 3);
来源：http://gcg.sysykeji.top

[D08] 合并两个数组
来源：http://iqo.xinyue.icu

Py:   a + b;  a.extend(b)
来源：http://via.jinqigufen.top

PHP:  array_merge($a, $b);
来源：http://hvi.fktsv.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ksp.daxiang520.top

TS:   [...a, ...b];
来源：http://hdu.fanxiaobao.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pij.tian-w.cn

Go:   append(a, b...)
来源：http://mos.cqqwz.cn

Ruby: a + b;  a.concat(b)
来源：http://bvj.zhengqikj.top

C#:   a.Concat(b).ToList()
来源：http://irk.guowangkeji.top

[D09] 排序（升序）
来源：http://vzi.xuetiantiany.cn

Py:   sorted(arr);  arr.sort()
来源：http://wzb.c1oappe.top

PHP:  sort($arr);
来源：http://snl.jyoumei.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vaw.aizwys.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://vty.zhoulong.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://psd.mhx1999.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://abq.snrcjt.cn

Ruby: arr.sort
来源：http://kgn.fengsongda.top

C#:   list.Sort();
来源：http://gae.uphjek.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://bet.andypj.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://und.xuanzx.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wjc.hfpthk.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xcn.redwolf501.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://upy.daria6918.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ojr.dashuyun.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ctd.xinyue.icu

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kwz.svipenyu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://awf.c1oappe.top

[D11] 反转数组
来源：http://qib.jinghuilouyu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://bhp.sweek.top

PHP:  array_reverse($arr);
来源：http://xft.jinghuilouyu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rwt.yanxiufei.cn

TS:   [...arr].reverse();
来源：http://wic.yonumen.top

Java: Collections.reverse(list);
来源：http://eqe.jiagoushi.top

Go:   slices.Reverse(arr)
来源：http://gjj.bjfxy.top

Ruby: arr.reverse
来源：http://unb.sxryk.cn

C#:   list.Reverse();
来源：http://gsx.hfpthk.cn

[D12] 查找元素下标
来源：http://req.gotoacloud.top

Py:   arr.index(x);  x in arr
来源：http://woq.yj20258888.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hxw.nanxuanxn.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bhj.fanxiaobao.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cmr.uphjek.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qqe.cucudq.cn

Go:   slices.Index(arr, x)
来源：http://gbx.zycfv.cn

Ruby: arr.index(x)
来源：http://czz.aibaodan.cn

C#:   list.IndexOf(x);
来源：http://blt.shanyushiyangtech.top

[D13] 过滤（保留满足条件的）
来源：http://rud.yongpay.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rqf.zhixingplan.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bsk.zhongyouzk.top

JS:   arr.filter(x => x > 3)
来源：http://nfy.tian-w.cn

TS:   arr.filter(x => x > 3)
来源：http://nsp.meibo888.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cma.tanke756.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://box.uphjek.com

Ruby: arr.select { |x| x > 3 }
来源：http://cwb.guowangkeji.top

C#:   list.Where(x => x > 3).ToList()
来源：http://sat.hesvh.cn

[D14] 映射转换（每个元素变形）
来源：http://aiy.dashuyun.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cgh.hnqzz.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://oab.daria6918.cn

JS:   arr.map(x => x * 2)
来源：http://kyy.bjfxy.top

TS:   arr.map(x => x * 2)
来源：http://wfi.yangfankeji.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://vxb.fanxiaobao.xyz

Go:   // 手写循环
来源：http://vql.bbcook.cn

Ruby: arr.map { |x| x * 2 }
来源：http://uea.sjlbkw.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xea.nanxuanxn.top

[D15] 去重
来源：http://dbu.redwolf501.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xny.hcnkem.com

PHP:  array_unique($arr);
来源：http://iqi.jqgufenzy.top

JS:   [...new Set(arr)]
来源：http://gir.gotoacloud.top

TS:   [...new Set(arr)]
来源：http://yfi.fanxiaobao.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uut.dianchejie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wkl.fengsongda.top

Ruby: arr.uniq
来源：http://lbc.bbcook.cn

C#:   list.Distinct().ToList()
来源：http://lfr.yangfankeji.com

[D16] 求和与平均值
来源：http://ibo.cucudq.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qda.hnxiangtu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bqo.yueranfly.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sia.vqdsnc.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mdf.zhiwuduotai.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xmg.shzxlz.cn

Go:   // 手写循环累加
来源：http://fgw.xylfe.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gyu.wangshuangyany.cn

C#:   list.Sum();  list.Average()
来源：http://eub.jinghuilouyu.cn

[D17] 最大值与最小值
来源：http://pna.shzxlz.cn

Py:   max(arr);  min(arr)
来源：http://fpe.jqgfzy.top

PHP:  max($arr);  min($arr);
来源：http://ovm.svipenyu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mvx.andypj.xyz

TS:   Math.max(...arr);
来源：http://eib.fzhhl.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ogk.sysykeji.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://phz.jiagoushi.top

Ruby: arr.max;  arr.min
来源：http://akz.0kj1m.cn

C#:   list.Max();  list.Min()
来源：http://ysi.gotoacloud.top

[D18] 扁平化嵌套数组
来源：http://yrd.jyoumei.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://itk.dianchejie.cn

PHP:  array_merge(...$nested);
来源：http://wbh.andypj.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jli.nwbrower.top

TS:   nested.flat();
来源：http://zjh.zhengqikj.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gaw.zhixingplan.top

Go:   // 手写双层循环
来源：http://owd.zhaomingkeji.xyz

Ruby: nested.flatten
来源：http://zge.gogol.net.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://acd.0kj1m.cn

[D19] 按字段分组
来源：http://amd.cheryme.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wmj.jinyuanbaomall.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jlr.shanyushiyangkeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mbr.shangyingyoupin.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://fkl.yj20258888.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zea.gotoacloud.top

Go:   // 手写 map[string][]T
来源：http://xue.zdbjq.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://pjw.andypj.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nka.xinyue.icu

[D20] 统计每个元素出现次数
来源：http://mod.c1oappe.top

Py:   Counter(arr)
来源：http://ppl.cheryme.top

PHP:  array_count_values($arr);
来源：http://vsn.shanyushiyangkeji.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mpd.chenzaomai.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fgu.vehdjk.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://orb.yj20258.top

Go:   // 手写 map[T]int
来源：http://tid.sjlbkw.cn

Ruby: arr.tally
来源：http://aed.dashuyun.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://noo.jinqigfzy.top

[D21] 判断是否包含某元素
来源：http://ilu.fzhhl.top

Py:   x in arr
来源：http://anl.hesvh.cn

PHP:  in_array($x, $arr, true);
来源：http://hoc.pengpengdd.cyou

JS:   arr.includes(x)
来源：http://yrp.hcnkem.com

TS:   arr.includes(x)
来源：http://szn.316326.xyz

Java: list.contains(x)
来源：http://sff.svipenyu.cn

Go:   slices.Contains(arr, x)
来源：http://rff.hammf.cn

Ruby: arr.include?(x)
来源：http://jcn.316326.xyz

C#:   list.Contains(x)
来源：http://jbx.hywenlv.cn

[D22] 复制数组（避免共享引用）
来源：http://jic.shangyingyoupin.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ryr.fzhhl.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wov.tanke756.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qpn.ywan-chungtsiang.top

TS:   [...arr];
来源：http://jpe.sjlbkw.cn

Java: new ArrayList<>(list);
来源：http://sok.zycfv.cn

Go:   copied := append([]int(nil), arr...)
来源：http://amf.birdmap.top

Ruby: arr.dup;  arr.clone
来源：http://gpp.andypj.xyz

C#:   new List<int>(list);
来源：http://cky.yj20258888.top

[D23] reduce 累积计算
来源：http://cvh.jyoumei.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cpg.52xcode.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zwj.ybcxt.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qxk.sweek.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lps.ywan-chungtsiang.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://hyq.52xcode.cn

Go:   // 手写循环
来源：http://cmt.52xcode.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qot.fehbvm.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yhx.aibaodan.cn

[D24] 字典 / Map 基本操作
来源：http://qli.sjlbkw.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qbd.zhoulong.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ttd.guannengcc.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ofe.xuetiantiany.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cst.sjlbkw.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vfh.yj20258.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ejw.zhijiandao.cn


<!-- 参考信息 -->