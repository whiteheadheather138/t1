代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://zrt.yangfankeji.com

C#:   arr.Select(s => s.ToUpper())
来源：http://zjz.fktsv.cn

[C08] 闭包
来源：http://vym.svipenyu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bzm.shanyushiyangtech.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://aqv.ywan-chungtsiang.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rte.xylfe.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gck.wangshuangyany.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gix.jyoumei.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vbp.cashguo.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://afy.zhixingplan.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ziy.yuanzhike.top

[C09] 递归
来源：http://quj.feifeiyinyue.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qoi.chenzaomai.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yta.tian-w.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yxn.fktsv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://esl.gzhubu.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://deh.316326.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ara.yvedp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://urg.pycfn.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://iuw.yueranfly.top

[C10] 变量作用域
来源：http://nvy.shanyushiyangtech.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jhy.jyoumei.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://opz.sxryk.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qhn.pengpengdd.cyou

TS:   同 JS
来源：http://kra.jinqigfzy.top

Java: 方法内为块级作用域
来源：http://yjb.zdbjq.cn

Go:   花括号块级作用域
来源：http://xtl.guannengcc.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xmm.iojbl.cn

C#:   块级作用域
来源：http://vjy.svipenyu.cn

[C11] 模块导入与导出
来源：http://kko.fehbvm.com

Py:   from module import func
来源：http://vwp.pycfn.com

PHP:  require "file.php";  或 use App\Service;
来源：http://mry.ywan-chungtsiang.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://anf.vqdsnc.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wry.zhijiandao.cn

Java: import java.util.List;
来源：http://btv.9152youxi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pxy.dashuyun.cn

Ruby: require "json"; require_relative "./util"
来源：http://tif.316326.xyz

C#:   using System.Text;
来源：http://eik.hfpthk.cn

[C12] 立即执行函数 IIFE
来源：http://mbw.quarkkingdee.top

Py:   (lambda: print("run"))()
来源：http://kat.hfpthk.cn

PHP:  (function () { echo "run"; })();
来源：http://hck.andypj.xyz

JS:   (() => { console.log("run"); })();
来源：http://ven.aibaodan.cn

TS:   (() => { console.log("run"); })();
来源：http://iyx.tianlin.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pgj.uphjek.com

Go:   func() { fmt.Println("run") }()
来源：http://ghl.chenjidiqi.icu

Ruby: -> { puts "run" }.call
来源：http://eie.jinyuanbaomall.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://azb.fehbvm.com

[C13] 类型声明 / 类型注解
来源：http://jev.yj20258.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mco.ydzc1.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mrh.fanxiaobao.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qub.dashuyun.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ciy.guowangkeji.top

Java: int add(int a, int b) { return a + b; }
来源：http://biq.yj20258.top

Go:   func add(a, b int) int
来源：http://ebs.pycfn.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fdq.andypj.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://ors.shuidangran.top

[C14] 泛型函数
来源：http://zgg.mhx1999.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pta.gogol.net.cn

PHP:  // 无泛型
来源：http://ueg.hesvh.cn

JS:   // 无泛型
来源：http://yqx.cucudq.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gwe.sysykeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qqn.tanke756.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vtu.zdbjq.cn

Ruby: # 无泛型
来源：http://uty.tanke756.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dou.sjlbkw.cn

[C15] 解构 / 展开参数
来源：http://sor.gzhubu.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rdd.yanxiufei.cn

PHP:  [$a, $b] = $pair;
来源：http://lpb.hongshengwenyu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fvo.sweek.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kkx.yonumen.top

Java: // 无解构
来源：http://pzt.jianghu66.top

Go:   // 无解构
来源：http://kdr.smart0.xyz

Ruby: a, b = pair
来源：http://iro.yvedp.cn

C#:   var (a, b) = pair;
来源：http://grg.yj20258888.top

[C16] 函数 / 方法重载
来源：http://iht.tian-w.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dus.nanxinkj.top

PHP:  // 无重载
来源：http://zst.nanxuanxn.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ona.52xcode.cn

TS:   // 用联合类型或重载签名声明
来源：http://nhm.sysykeji.top

Java: void f(int a) {}  void f(String a) {}
来源：http://njd.xylfe.cn

Go:   // 无重载：用不同函数名
来源：http://pov.xinyue.icu

Ruby: # 无重载：靠动态参数
来源：http://nll.dashuyun.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://cpu.sysykeji.top

================================================================================
来源：http://rdd.snrcjt.cn

D. 数组 / 列表 / 集合
来源：http://eoo.chenjidiqi.icu

================================================================================
来源：http://hzw.c1oappe.top

[D01] 创建数组 / 列表
来源：http://mna.shanyushiyangkeji.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://tug.cucudq.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ymd.yongpay.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lbe.sysykeji.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://hoo.nwbrower.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gmv.jqgfzy.top

Go:   arr := []int{1, 2, 3}
来源：http://vrk.zhijiandao.cn

Ruby: arr = [1, 2, 3]
来源：http://bhg.yj20258.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rkh.epnwcf.com

[D02] 追加元素到末尾
来源：http://mzj.jinqigufen.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://alu.fanxiaobao.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uha.uphjek.com

JS:   arr.push(4);
来源：http://gfj.cdnleiting.top

TS:   arr.push(4);
来源：http://vvb.guowangkeji.top

Java: list.add(4);
来源：http://hlj.feifeiyinyue.top

Go:   arr = append(arr, 4)
来源：http://rky.chenjidiqi.icu

Ruby: arr << 4; arr.push(5)
来源：http://trb.jinqigufen.top

C#:   list.Add(4);
来源：http://win.xuetiantiany.cn

[D03] 在指定位置插入元素
来源：http://nks.haohaochexian.top

Py:   arr.insert(0, 0)
来源：http://zng.ivvv.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hrx.yj20258.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vas.aibaodan.cn

TS:   arr.splice(0, 0, 0);
来源：http://inj.meibo888.top

Java: list.add(0, 0);
来源：http://yfq.xinyue.icu

Go:   arr = append([]int{0}, arr...)
来源：http://pzt.fanxiaobao.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dui.gotoacloud.top

C#:   list.Insert(0, 0);
来源：http://nxl.shuidangran.top

[D04] 删除元素
来源：http://yqy.hnxiangtu.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nas.hnxiangtu.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uzy.hywenlv.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wsb.xinyue.icu

TS:   arr.splice(0, 1);
来源：http://tzi.tanke756.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xlo.0kj1m.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yxq.tarul.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zkk.hnxiangtu.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sqx.fktsv.cn

[D05] 访问与修改元素
来源：http://rtn.fzhhl.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qny.yanxiufei.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nmc.ydjk.org.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jep.xinyue.icu

TS:   arr[0]; arr.at(-1);
来源：http://aru.hnxiangtu.top

Java: list.get(0); list.set(0, 9);
来源：http://omb.xuanzx.com

Go:   arr[0]; arr[0] = 9
来源：http://bnw.bbcook.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zdz.zhongyouzk.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zub.yj20258.top

[D06] 数组长度
来源：http://coq.dianchejie.cn

Py:   len(arr)
来源：http://xci.dianchejie.cn

PHP:  count($arr);
来源：http://kxj.tanke756.top

JS:   arr.length
来源：http://lhn.hywenlv.cn

TS:   arr.length
来源：http://mkd.quarkkingdee.top

Java: list.size();
来源：http://cdc.meibo888.top

Go:   len(arr)
来源：http://mxx.hammf.cn

Ruby: arr.length; arr.size
来源：http://ktp.xuanzx.com

C#:   list.Count;
来源：http://kgd.nanxinkj.top

[D07] 切片 / 取子数组
来源：http://gyd.cashguo.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ocy.xingfuxueyuan.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://qjp.fengsongda.top

JS:   arr.slice(1, 4);
来源：http://tej.jinqigfzy.top

TS:   arr.slice(1, 4);
来源：http://hgf.uphjek.com

Java: list.subList(1, 4);
来源：http://fnq.xuetiantiany.cn

Go:   arr[1:4]
来源：http://qcn.yfazqb.com

Ruby: arr[1, 3]
来源：http://sio.zhoulong.xyz

C#:   list.GetRange(1, 3);
来源：http://wex.daxiang520.top

[D08] 合并两个数组
来源：http://kbx.shangyingyoupin.top

Py:   a + b;  a.extend(b)
来源：http://epd.shzxlz.cn

PHP:  array_merge($a, $b);
来源：http://vrx.zhaomingkeji.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://rbi.cashguo.top

TS:   [...a, ...b];
来源：http://lbj.tian-w.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://skq.zhiwuduotai.top

Go:   append(a, b...)
来源：http://pdi.jinghuilouyu.cn

Ruby: a + b;  a.concat(b)
来源：http://pel.zhiwuduotai.top

C#:   a.Concat(b).ToList()
来源：http://wvf.c1oappe.top

[D09] 排序（升序）
来源：http://sar.nwbrower.top

Py:   sorted(arr);  arr.sort()
来源：http://sha.feifeiyinyue.top

PHP:  sort($arr);
来源：http://whu.tian-w.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mqx.dashuyun.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xee.chenzaomai.com

Java: Collections.sort(list);  list.sort(null);
来源：http://lvv.0kj1m.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://iic.ywan-chungtsiang.top

Ruby: arr.sort
来源：http://zhc.fktsv.cn

C#:   list.Sort();
来源：http://kmq.zhijiandao.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qay.ydzc1.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xbh.9152youxi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nzt.jinghuilouyu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ozn.nanxuanxn.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://uxm.gogol.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ygh.xylfe.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sdr.snrcjt.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hqa.316326.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uhn.wangshuangyany.cn

[D11] 反转数组
来源：http://ofh.iojbl.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zrq.tianlin.xyz

PHP:  array_reverse($arr);
来源：http://eep.bbcook.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yxm.zhaomingkeji.xyz

TS:   [...arr].reverse();
来源：http://wdo.xuanzx.com

Java: Collections.reverse(list);
来源：http://vqd.quarkkingdee.top

Go:   slices.Reverse(arr)
来源：http://ryc.ehwqpu.com

Ruby: arr.reverse
来源：http://wdp.cdnleiting.top

C#:   list.Reverse();
来源：http://hfy.hnxiangtu.top

[D12] 查找元素下标
来源：http://zhz.jyoumei.cn

Py:   arr.index(x);  x in arr
来源：http://uzr.yueranfly.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cif.hesvh.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://afj.xuanzx.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lmq.wangdashe.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rpa.svipenyu.cn

Go:   slices.Index(arr, x)
来源：http://izs.shanyushiyangtech.top

Ruby: arr.index(x)
来源：http://ogi.cashguo.top

C#:   list.IndexOf(x);
来源：http://klv.aibaodan.cn

[D13] 过滤（保留满足条件的）
来源：http://cvi.vehdjk.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nrz.shangyingyoupin.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sfs.iojbl.cn

JS:   arr.filter(x => x > 3)
来源：http://jsy.ehwqpu.com

TS:   arr.filter(x => x > 3)
来源：http://bcq.epnwcf.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://owt.jyoumei.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ftk.jqgfzy.top

Ruby: arr.select { |x| x > 3 }
来源：http://yzf.chenjidiqi.icu

C#:   list.Where(x => x > 3).ToList()
来源：http://zrw.vehdjk.com

[D14] 映射转换（每个元素变形）
来源：http://xmo.daria6918.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hws.ctjpmb.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wip.dianchejie.cn

JS:   arr.map(x => x * 2)
来源：http://qxf.chenjidiqi.icu

TS:   arr.map(x => x * 2)
来源：http://fqx.hfpthk.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://odq.haohaochexian.top

Go:   // 手写循环
来源：http://baw.jianghu66.top

Ruby: arr.map { |x| x * 2 }
来源：http://bxm.birdmap.top

C#:   list.Select(x => x * 2).ToList()
来源：http://vsw.hnqzz.top

[D15] 去重
来源：http://vsv.quarkkingdee.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ofj.gotoacloud.top

PHP:  array_unique($arr);
来源：http://zbg.ctjpmb.com

JS:   [...new Set(arr)]
来源：http://yph.hongshengwenyu.top

TS:   [...new Set(arr)]
来源：http://bbc.chenlongwang.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nzb.jqgfzy.top

Go:   // 用 map[T]struct{} 手写
来源：http://urj.zdbjq.cn

Ruby: arr.uniq
来源：http://gme.smart0.xyz

C#:   list.Distinct().ToList()
来源：http://dqk.shanyushiyangtech.top

[D16] 求和与平均值
来源：http://xux.52xcode.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gra.guannengcc.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://srj.zhengqikj.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zqh.bjfxy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://oit.9152youxi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fuk.kuanghao11.cn

Go:   // 手写循环累加
来源：http://krq.hongshengwenyu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uus.zhijiandao.cn

C#:   list.Sum();  list.Average()
来源：http://dvo.yuxming.cn

[D17] 最大值与最小值
来源：http://qds.aizwys.cn

Py:   max(arr);  min(arr)
来源：http://cgu.c1oappe.top

PHP:  max($arr);  min($arr);
来源：http://csv.feifeiyinyue.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dkd.vehdjk.com

TS:   Math.max(...arr);
来源：http://gwm.daria6918.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://brx.dianchejie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hlk.hnqzz.top

Ruby: arr.max;  arr.min
来源：http://foh.zhiwuduotai.top

C#:   list.Max();  list.Min()
来源：http://wjy.dashuyun.cn

[D18] 扁平化嵌套数组
来源：http://gqb.0kj1m.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wrj.andypj.xyz

PHP:  array_merge(...$nested);
来源：http://uoc.cdnleiting.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://iss.yvedp.cn

TS:   nested.flat();
来源：http://tfg.ydjk.org.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tvw.guowangkeji.top

Go:   // 手写双层循环
来源：http://qed.zhongyouzk.top

Ruby: nested.flatten
来源：http://tom.havefunace.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://yqb.yanxiufei.cn

[D19] 按字段分组
来源：http://ulq.aibaodan.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ove.jyoumei.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://oxv.vehdjk.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fwz.sxryk.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yjj.gogol.net.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ddx.zhixingplan.top

Go:   // 手写 map[string][]T
来源：http://qih.fzhhl.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://zme.hesvh.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wze.chenzaomai.com

[D20] 统计每个元素出现次数
来源：http://oye.c1oappe.top

Py:   Counter(arr)
来源：http://rfc.zhoulong.xyz

PHP:  array_count_values($arr);
来源：http://ern.pengpengdd.cyou

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rhk.jlsjyb.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lls.ywan-chungtsiang.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tjb.wangshuangyany.cn

Go:   // 手写 map[T]int
来源：http://cre.gaohongyu789.top

Ruby: arr.tally
来源：http://dre.shanyushiyangtech.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qul.zhiwuduotai.top

[D21] 判断是否包含某元素
来源：http://vku.shzxlz.cn

Py:   x in arr
来源：http://mhi.tian-w.cn

PHP:  in_array($x, $arr, true);
来源：http://xps.dianchejie.cn

JS:   arr.includes(x)
来源：http://srj.daxiang520.top

TS:   arr.includes(x)
来源：http://bxb.yongpay.top

Java: list.contains(x)
来源：http://qkz.shanyushiyangtech.top

Go:   slices.Contains(arr, x)
来源：http://iht.xuetiantiany.cn

Ruby: arr.include?(x)
来源：http://vpr.gzhubu.top

C#:   list.Contains(x)
来源：http://sep.zhixingplan.top

[D22] 复制数组（避免共享引用）
来源：http://azv.zdqjudy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gnx.zhengqikj.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qlt.jinqigufen.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://piq.aizwys.cn

TS:   [...arr];
来源：http://rex.hesvh.cn

Java: new ArrayList<>(list);
来源：http://fuc.yangfankeji.com

Go:   copied := append([]int(nil), arr...)
来源：http://yly.316326.xyz

Ruby: arr.dup;  arr.clone
来源：http://dlc.tianlin.xyz

C#:   new List<int>(list);
来源：http://wab.ydjk.org.cn

[D23] reduce 累积计算
来源：http://mks.yonumen.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fxn.shanyushiyangkeji.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rof.hnxiangtu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fjm.zhengqikj.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://otq.quarkkingdee.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ngz.tian-w.cn

Go:   // 手写循环
来源：http://qbe.hesvh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://umk.daxiang520.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vhi.jinghuilouyu.cn

[D24] 字典 / Map 基本操作
来源：http://fty.hywenlv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qfz.sjlbkw.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xrx.feifeiyinyue.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://riq.zdqjudy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yqw.yonumen.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rcv.jqgufenzy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qid.kuanghao11.cn


<!-- 参考信息 -->