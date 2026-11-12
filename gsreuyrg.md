代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://oif.9152youxi.cn

TS:   arr.map(String)
来源：http://fsn.bjfxy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hyf.shuidangran.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yhg.epnwcf.com

Ruby: arr.map(&:upcase)
来源：http://xqv.epnwcf.com

C#:   arr.Select(s => s.ToUpper())
来源：http://rlk.ehwqpu.com

[C08] 闭包
来源：http://qkh.yongpay.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kgm.ppjwa.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://udf.316326.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://agy.zhaomingkeji.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://djf.ehwqpu.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wkg.vehdjk.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wns.jianghu66.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nmv.epnwcf.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://atg.shzxlz.cn

[C09] 递归
来源：http://pcx.xinyue.icu

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sol.zhixingplan.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bms.yongpay.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fpt.hysaishi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qpy.cheryme.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uqe.ywan-chungtsiang.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ela.aibaodan.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qpe.feifeiyinyue.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vkr.bbcook.cn

[C10] 变量作用域
来源：http://fui.yuxming.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mgy.jqgfzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fkx.ehwqpu.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://amj.vqdsnc.cn

TS:   同 JS
来源：http://xap.yj202588.top

Java: 方法内为块级作用域
来源：http://xod.c1oappe.top

Go:   花括号块级作用域
来源：http://qyo.shangyingyoupin.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qcr.wangdashe.top

C#:   块级作用域
来源：http://gog.gaohongyu789.top

[C11] 模块导入与导出
来源：http://npb.pycfn.com

Py:   from module import func
来源：http://lrr.yj202588.top

PHP:  require "file.php";  或 use App\Service;
来源：http://wgy.daria6918.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://npw.shanyushiyangtech.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://buq.guowangkeji.top

Java: import java.util.List;
来源：http://quz.gotoacloud.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://laq.meibo888.top

Ruby: require "json"; require_relative "./util"
来源：http://okw.svipenyu.cn

C#:   using System.Text;
来源：http://nve.nanxuanxn.top

[C12] 立即执行函数 IIFE
来源：http://hkd.zhongyouzk.top

Py:   (lambda: print("run"))()
来源：http://ymt.yonumen.top

PHP:  (function () { echo "run"; })();
来源：http://ywm.zycfv.cn

JS:   (() => { console.log("run"); })();
来源：http://xjv.dashuyun.cn

TS:   (() => { console.log("run"); })();
来源：http://bhl.bbcook.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://abr.fzhhl.top

Go:   func() { fmt.Println("run") }()
来源：http://ruu.jinghuilouyu.cn

Ruby: -> { puts "run" }.call
来源：http://kie.yj20258.top

C#:   // 无 IIFE：用静态构造函数
来源：http://tkj.bbcook.cn

[C13] 类型声明 / 类型注解
来源：http://xkt.yueranfly.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qlh.nanxuanxn.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jmf.52xcode.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xui.aibaodan.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hbe.yanxiufei.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xnt.fehbvm.com

Go:   func add(a, b int) int
来源：http://tji.ppjwa.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cmd.bjfxy.top

C#:   int Add(int a, int b) => a + b;
来源：http://kaz.hysaishi.cn

[C14] 泛型函数
来源：http://cdy.tarul.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bio.yonumen.top

PHP:  // 无泛型
来源：http://rhu.xuetiantiany.cn

JS:   // 无泛型
来源：http://tea.tarul.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bfi.wangdashe.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mvl.zhoulong.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pld.wangshuangyany.cn

Ruby: # 无泛型
来源：http://sba.fehbvm.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gju.zdqjudy.top

[C15] 解构 / 展开参数
来源：http://bsm.9152youxi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vdh.jqgufenzy.top

PHP:  [$a, $b] = $pair;
来源：http://wag.ybcxt.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://aus.ppjwa.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://znr.ehwqpu.com

Java: // 无解构
来源：http://gvv.snrcjt.cn

Go:   // 无解构
来源：http://xve.cqqwz.cn

Ruby: a, b = pair
来源：http://rqg.havefunace.top

C#:   var (a, b) = pair;
来源：http://piq.pycfn.com

[C16] 函数 / 方法重载
来源：http://pyz.xziqi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://eua.cucudq.cn

PHP:  // 无重载
来源：http://osf.hywenlv.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://jyy.snrcjt.cn

TS:   // 用联合类型或重载签名声明
来源：http://cmu.nanxuanxn.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ria.52xcode.cn

Go:   // 无重载：用不同函数名
来源：http://mxl.pengpengdd.cyou

Ruby: # 无重载：靠动态参数
来源：http://udr.yj20258888.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://tro.pycfn.com

================================================================================
来源：http://qft.hnxiangtu.top

D. 数组 / 列表 / 集合
来源：http://ush.kuanghao11.cn

================================================================================
来源：http://rzn.ywan-chungtsiang.top

[D01] 创建数组 / 列表
来源：http://ezs.zhaomingkeji.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://fno.epnwcf.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mlb.yj202588.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ptp.yj20258.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://mvx.birdmap.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nph.zdbjq.cn

Go:   arr := []int{1, 2, 3}
来源：http://qqu.shanyushiyangkeji.top

Ruby: arr = [1, 2, 3]
来源：http://gcu.yongpay.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://enr.bjfxy.top

[D02] 追加元素到末尾
来源：http://yxw.hnxiangtu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gsk.aibaodan.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://eks.yueranfly.top

JS:   arr.push(4);
来源：http://sig.hongshengwenyu.top

TS:   arr.push(4);
来源：http://xtd.svipenyu.cn

Java: list.add(4);
来源：http://ipe.yj202588.top

Go:   arr = append(arr, 4)
来源：http://vmf.yvedp.cn

Ruby: arr << 4; arr.push(5)
来源：http://vvq.yuanzhike.top

C#:   list.Add(4);
来源：http://ykb.zhiwuduotai.top

[D03] 在指定位置插入元素
来源：http://ciy.hnxiangtu.top

Py:   arr.insert(0, 0)
来源：http://qty.zhijiandao.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yrt.yj202588.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hlh.yfazqb.com

TS:   arr.splice(0, 0, 0);
来源：http://muv.mhx1999.top

Java: list.add(0, 0);
来源：http://ejr.cucudq.cn

Go:   arr = append([]int{0}, arr...)
来源：http://nxf.jinyuanbaomall.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kpi.c1oappe.top

C#:   list.Insert(0, 0);
来源：http://xpm.316326.xyz

[D04] 删除元素
来源：http://vqh.zhongyouzk.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tif.tanke756.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qlp.nwbrower.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fsc.gotoacloud.top

TS:   arr.splice(0, 1);
来源：http://dof.redwolf501.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ioo.xuetiantiany.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vwm.tianlin.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://idt.jinqigfzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pds.jianghu66.top

[D05] 访问与修改元素
来源：http://hcf.snrcjt.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wcw.hesvh.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rdm.c1oappe.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xjt.sysykeji.top

TS:   arr[0]; arr.at(-1);
来源：http://aee.nanxinkj.top

Java: list.get(0); list.set(0, 9);
来源：http://svv.hnqzz.top

Go:   arr[0]; arr[0] = 9
来源：http://ztz.smart0.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tcc.xuanzx.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vfe.yongpay.top

[D06] 数组长度
来源：http://rjo.shangyingyoupin.top

Py:   len(arr)
来源：http://jal.fehbvm.com

PHP:  count($arr);
来源：http://vau.xuanzx.com

JS:   arr.length
来源：http://mqo.yangfankeji.com

TS:   arr.length
来源：http://dir.yonumen.top

Java: list.size();
来源：http://och.zhiwuduotai.top

Go:   len(arr)
来源：http://dcx.gzhubu.top

Ruby: arr.length; arr.size
来源：http://onh.xylfe.cn

C#:   list.Count;
来源：http://bgj.yueranfly.top

[D07] 切片 / 取子数组
来源：http://xoa.ppjwa.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ghu.tanke756.top

PHP:  array_slice($arr, 1, 3);
来源：http://zyr.fktsv.cn

JS:   arr.slice(1, 4);
来源：http://kxv.xuanzx.com

TS:   arr.slice(1, 4);
来源：http://tsy.jyoumei.cn

Java: list.subList(1, 4);
来源：http://tdk.svipenyu.cn

Go:   arr[1:4]
来源：http://jxr.birdmap.top

Ruby: arr[1, 3]
来源：http://wdj.yongpay.top

C#:   list.GetRange(1, 3);
来源：http://eyf.sxryk.cn

[D08] 合并两个数组
来源：http://ism.chenjidiqi.icu

Py:   a + b;  a.extend(b)
来源：http://riu.cqqwz.cn

PHP:  array_merge($a, $b);
来源：http://veh.hfpthk.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ehu.andypj.xyz

TS:   [...a, ...b];
来源：http://qdz.ctjpmb.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yzg.chenjidiqi.icu

Go:   append(a, b...)
来源：http://bku.shzxlz.cn

Ruby: a + b;  a.concat(b)
来源：http://akt.yuxming.cn

C#:   a.Concat(b).ToList()
来源：http://vxp.hnxiangtu.top

[D09] 排序（升序）
来源：http://joj.gotoacloud.top

Py:   sorted(arr);  arr.sort()
来源：http://hpw.sysykeji.top

PHP:  sort($arr);
来源：http://fzx.uphjek.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mon.yj20258888.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ubs.jinyuanbaomall.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://umb.hnxiangtu.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://taz.yj20258888.top

Ruby: arr.sort
来源：http://zrs.guowangkeji.top

C#:   list.Sort();
来源：http://ebs.hcnkem.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://pxw.hammf.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xkp.haohaochexian.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ylk.sxryk.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cem.havefunace.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kfx.9152youxi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://aiy.fanxiaobao.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fem.daxiang520.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zhl.cashguo.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zhs.mhx1999.top

[D11] 反转数组
来源：http://yjz.yueranfly.top

Py:   arr[::-1];  arr.reverse()
来源：http://rda.hcnkem.com

PHP:  array_reverse($arr);
来源：http://ink.yvedp.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wby.jinyuanbaomall.cn

TS:   [...arr].reverse();
来源：http://cyw.ppjwa.cn

Java: Collections.reverse(list);
来源：http://lvb.zhoulong.xyz

Go:   slices.Reverse(arr)
来源：http://rqo.hfpthk.cn

Ruby: arr.reverse
来源：http://zkc.chenzaomai.com

C#:   list.Reverse();
来源：http://rji.meibo888.top

[D12] 查找元素下标
来源：http://wos.xuanzx.com

Py:   arr.index(x);  x in arr
来源：http://gsr.hesvh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://eam.zhengqikj.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wpo.hnxiangtu.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bpj.sufxvd.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://btb.haohaochexian.top

Go:   slices.Index(arr, x)
来源：http://qeh.pycfn.com

Ruby: arr.index(x)
来源：http://dqj.nwbrower.top

C#:   list.IndexOf(x);
来源：http://sjw.andypj.xyz

[D13] 过滤（保留满足条件的）
来源：http://fbw.hongshengwenyu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qvq.zhongyouzk.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jnt.tianlin.xyz

JS:   arr.filter(x => x > 3)
来源：http://acj.hammf.cn

TS:   arr.filter(x => x > 3)
来源：http://clm.sxryk.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ycy.dashuyun.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rvu.fktsv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ann.jlsjyb.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://sun.ybcxt.top

[D14] 映射转换（每个元素变形）
来源：http://uvr.kuanghao11.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nya.quarkkingdee.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://etv.jinqigufen.top

JS:   arr.map(x => x * 2)
来源：http://uya.ctjpmb.com

TS:   arr.map(x => x * 2)
来源：http://jgz.chenlongwang.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://zpx.hnqzz.top

Go:   // 手写循环
来源：http://zso.ctjpmb.com

Ruby: arr.map { |x| x * 2 }
来源：http://iqr.hywenlv.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://gvv.zhoulong.xyz

[D15] 去重
来源：http://msx.guowangkeji.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://keg.52xcode.cn

PHP:  array_unique($arr);
来源：http://zpn.ydzc1.top

JS:   [...new Set(arr)]
来源：http://woo.shuidangran.top

TS:   [...new Set(arr)]
来源：http://ggu.vehdjk.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wxk.tarul.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cih.ehwqpu.com

Ruby: arr.uniq
来源：http://jrm.zhaomingkeji.xyz

C#:   list.Distinct().ToList()
来源：http://khd.tian-w.cn

[D16] 求和与平均值
来源：http://bpz.ctjpmb.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kee.yonumen.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uca.feifeiyinyue.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cao.ivvv.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qww.xuetiantiany.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://eeh.fzhhl.top

Go:   // 手写循环累加
来源：http://qiu.zdbjq.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hbn.yongpay.top

C#:   list.Sum();  list.Average()
来源：http://ddi.jqgfzy.top

[D17] 最大值与最小值
来源：http://kmn.jinqigfzy.top

Py:   max(arr);  min(arr)
来源：http://dgr.daxiang520.top

PHP:  max($arr);  min($arr);
来源：http://zle.wangshuangyany.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gut.tian-w.cn

TS:   Math.max(...arr);
来源：http://eud.jianghu66.top

Java: Collections.max(list);  Collections.min(list);
来源：http://pdr.hysaishi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ian.ywan-chungtsiang.top

Ruby: arr.max;  arr.min
来源：http://nph.bjfxy.top

C#:   list.Max();  list.Min()
来源：http://seh.dianchejie.cn

[D18] 扁平化嵌套数组
来源：http://lsc.tian-w.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://soz.aizwys.cn

PHP:  array_merge(...$nested);
来源：http://weg.0kj1m.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://iwq.cucudq.cn

TS:   nested.flat();
来源：http://iem.nanxinkj.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fue.pycfn.com

Go:   // 手写双层循环
来源：http://qtd.shanyushiyangkeji.top

Ruby: nested.flatten
来源：http://klx.feifeiyinyue.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://opc.daxiang520.top

[D19] 按字段分组
来源：http://ooz.yangfankeji.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lwg.dianchejie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bax.bjfxy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nzq.ybcxt.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ern.hnqzz.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mdl.epnwcf.com

Go:   // 手写 map[string][]T
来源：http://arh.hysaishi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://txf.ppjwa.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qxv.ywan-chungtsiang.top

[D20] 统计每个元素出现次数
来源：http://rit.guannengcc.top

Py:   Counter(arr)
来源：http://mbg.zhongyouzk.top

PHP:  array_count_values($arr);
来源：http://mka.jyoumei.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rlt.fehbvm.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jif.xingfuxueyuan.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://phe.zycfv.cn

Go:   // 手写 map[T]int
来源：http://tys.xziqi.cn

Ruby: arr.tally
来源：http://svs.cucudq.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://whp.gotoacloud.top

[D21] 判断是否包含某元素
来源：http://cej.chenlongwang.top

Py:   x in arr
来源：http://uye.yuxming.cn

PHP:  in_array($x, $arr, true);
来源：http://wdt.ehwqpu.com

JS:   arr.includes(x)
来源：http://xuj.jyoumei.cn

TS:   arr.includes(x)
来源：http://dnq.yfazqb.com

Java: list.contains(x)
来源：http://uwu.jinqigfzy.top

Go:   slices.Contains(arr, x)
来源：http://tqx.hywenlv.cn

Ruby: arr.include?(x)
来源：http://hjj.ctjpmb.com

C#:   list.Contains(x)
来源：http://vsl.meibo888.top

[D22] 复制数组（避免共享引用）
来源：http://xpd.mhx1999.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://key.yongpay.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ijw.vehdjk.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pfz.zhongyouzk.top

TS:   [...arr];
来源：http://yfn.ivvv.top

Java: new ArrayList<>(list);
来源：http://bzr.snrcjt.cn

Go:   copied := append([]int(nil), arr...)
来源：http://nod.jlsjyb.cn

Ruby: arr.dup;  arr.clone
来源：http://iwr.jiagoushi.top

C#:   new List<int>(list);
来源：http://vyl.hfpthk.cn

[D23] reduce 累积计算
来源：http://rud.andypj.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ndw.shanyushiyangtech.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://prp.bjfxy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://upe.yuanzhike.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iwv.iojbl.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://not.jyoumei.cn

Go:   // 手写循环
来源：http://vnn.yonumen.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://azb.cucudq.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nra.gotoacloud.top

[D24] 字典 / Map 基本操作
来源：http://obe.hywenlv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sev.vehdjk.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sbr.ydzc1.top


<!-- 参考信息 -->