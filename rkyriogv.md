代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://peo.feifeiyinyue.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ibp.hnqzz.top

[C08] 闭包
来源：http://hww.zhixingplan.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kvj.shanyushiyangkeji.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xzp.chenlongwang.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://diz.havefunace.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ryl.shanyushiyangtech.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tbs.chenjidiqi.icu

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://uvj.guowangkeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dfn.epnwcf.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://oiw.xinyue.icu

[C09] 递归
来源：http://yte.gzhubu.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rhc.yj202588.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vsx.jqgufenzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hmg.daxiang520.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://whr.jinghuilouyu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dtm.yj20258.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tbz.yueranfly.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xyo.guowangkeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://saz.pengpengdd.cyou

[C10] 变量作用域
来源：http://raa.hywenlv.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sio.andypj.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ecs.zhongyouzk.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dxf.hfpthk.cn

TS:   同 JS
来源：http://jix.tarul.cn

Java: 方法内为块级作用域
来源：http://bkl.zhaomingkeji.xyz

Go:   花括号块级作用域
来源：http://hjv.yj20258.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jhk.ehwqpu.com

C#:   块级作用域
来源：http://afs.cqqwz.cn

[C11] 模块导入与导出
来源：http://nkh.hammf.cn

Py:   from module import func
来源：http://uby.chenlongwang.top

PHP:  require "file.php";  或 use App\Service;
来源：http://yht.ppjwa.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vow.nwbrower.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vkx.xziqi.cn

Java: import java.util.List;
来源：http://usl.shuidangran.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gmw.sjlbkw.cn

Ruby: require "json"; require_relative "./util"
来源：http://tdq.vehdjk.com

C#:   using System.Text;
来源：http://ihe.mhx1999.top

[C12] 立即执行函数 IIFE
来源：http://yni.dashuyun.cn

Py:   (lambda: print("run"))()
来源：http://ctw.fanxiaobao.xyz

PHP:  (function () { echo "run"; })();
来源：http://ubb.epnwcf.com

JS:   (() => { console.log("run"); })();
来源：http://qrk.zycfv.cn

TS:   (() => { console.log("run"); })();
来源：http://ajf.yj20258.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ige.guannengcc.top

Go:   func() { fmt.Println("run") }()
来源：http://agk.xingfuxueyuan.xyz

Ruby: -> { puts "run" }.call
来源：http://rqe.daria6918.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://vew.chenlongwang.top

[C13] 类型声明 / 类型注解
来源：http://zby.havefunace.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vmb.vehdjk.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ymb.tarul.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dul.kuanghao11.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qts.dashuyun.cn

Java: int add(int a, int b) { return a + b; }
来源：http://pfy.xuetiantiany.cn

Go:   func add(a, b int) int
来源：http://cwt.haohaochexian.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vbc.ydjk.org.cn

C#:   int Add(int a, int b) => a + b;
来源：http://sau.sysykeji.top

[C14] 泛型函数
来源：http://axn.hnxiangtu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wnn.ppjwa.cn

PHP:  // 无泛型
来源：http://bxs.hammf.cn

JS:   // 无泛型
来源：http://beq.xuanzx.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pjc.ivvv.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uvc.chenzaomai.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rup.yanxiufei.cn

Ruby: # 无泛型
来源：http://zhn.fehbvm.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xii.tanke756.top

[C15] 解构 / 展开参数
来源：http://lng.tian-w.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sir.chenlongwang.top

PHP:  [$a, $b] = $pair;
来源：http://pjp.xingfuxueyuan.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dzr.yongpay.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nux.chenjidiqi.icu

Java: // 无解构
来源：http://jzr.zdqjudy.top

Go:   // 无解构
来源：http://qzo.xziqi.cn

Ruby: a, b = pair
来源：http://oir.yj202588.top

C#:   var (a, b) = pair;
来源：http://yzl.tian-w.cn

[C16] 函数 / 方法重载
来源：http://bgy.sxryk.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://srl.gzhubu.top

PHP:  // 无重载
来源：http://ahv.uphjek.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://qse.jinghuilouyu.cn

TS:   // 用联合类型或重载签名声明
来源：http://aca.aizwys.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://suy.cucudq.cn

Go:   // 无重载：用不同函数名
来源：http://ksf.cashguo.top

Ruby: # 无重载：靠动态参数
来源：http://kvu.9152youxi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://pzc.shanyushiyangtech.top

================================================================================
来源：http://lfl.fzhhl.top

D. 数组 / 列表 / 集合
来源：http://wuh.0kj1m.cn

================================================================================
来源：http://umm.ybcxt.top

[D01] 创建数组 / 列表
来源：http://gwj.xylfe.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zwj.nanxinkj.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gmv.wangdashe.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jst.dianchejie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ysp.yuxming.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nqg.xziqi.cn

Go:   arr := []int{1, 2, 3}
来源：http://wbp.ydzc1.top

Ruby: arr = [1, 2, 3]
来源：http://jme.fzhhl.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rys.bbcook.cn

[D02] 追加元素到末尾
来源：http://eml.pengpengdd.cyou

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tvy.fktsv.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oif.hysaishi.cn

JS:   arr.push(4);
来源：http://frw.shuidangran.top

TS:   arr.push(4);
来源：http://xpr.tarul.cn

Java: list.add(4);
来源：http://cct.dashuyun.cn

Go:   arr = append(arr, 4)
来源：http://ejp.hfpthk.cn

Ruby: arr << 4; arr.push(5)
来源：http://ccr.sxryk.cn

C#:   list.Add(4);
来源：http://hqe.hammf.cn

[D03] 在指定位置插入元素
来源：http://eml.shanyushiyangkeji.top

Py:   arr.insert(0, 0)
来源：http://noe.meibo888.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mfg.jinqigfzy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://htj.zdbjq.cn

TS:   arr.splice(0, 0, 0);
来源：http://dpg.ydzc1.top

Java: list.add(0, 0);
来源：http://sfv.jiagoushi.top

Go:   arr = append([]int{0}, arr...)
来源：http://qul.ydjk.org.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yza.nanxinkj.top

C#:   list.Insert(0, 0);
来源：http://laj.zhiwuduotai.top

[D04] 删除元素
来源：http://rvd.jqgfzy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nkr.yj202588.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vgs.hongshengwenyu.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qkn.cheryme.top

TS:   arr.splice(0, 1);
来源：http://rur.pycfn.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qru.sxryk.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jqz.ydzc1.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://put.tian-w.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://clc.vehdjk.com

[D05] 访问与修改元素
来源：http://zgo.jinqigufen.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bmd.gzhubu.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jzd.fzhhl.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gtk.hesvh.cn

TS:   arr[0]; arr.at(-1);
来源：http://vdz.ppjwa.cn

Java: list.get(0); list.set(0, 9);
来源：http://ozm.tarul.cn

Go:   arr[0]; arr[0] = 9
来源：http://ljh.daria6918.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://oet.tianlin.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qph.meibo888.top

[D06] 数组长度
来源：http://epf.mhx1999.top

Py:   len(arr)
来源：http://xfn.jinqigufen.top

PHP:  count($arr);
来源：http://som.cashguo.top

JS:   arr.length
来源：http://iqy.tanke756.top

TS:   arr.length
来源：http://lto.sufxvd.cn

Java: list.size();
来源：http://whw.yongpay.top

Go:   len(arr)
来源：http://rbq.hammf.cn

Ruby: arr.length; arr.size
来源：http://hao.tian-w.cn

C#:   list.Count;
来源：http://yum.yj20258.top

[D07] 切片 / 取子数组
来源：http://zmi.yuxming.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cfl.fehbvm.com

PHP:  array_slice($arr, 1, 3);
来源：http://yfn.jinqigufen.top

JS:   arr.slice(1, 4);
来源：http://xhe.sweek.top

TS:   arr.slice(1, 4);
来源：http://fkq.sufxvd.cn

Java: list.subList(1, 4);
来源：http://dog.yj20258888.top

Go:   arr[1:4]
来源：http://tas.bbcook.cn

Ruby: arr[1, 3]
来源：http://uxj.chenlongwang.top

C#:   list.GetRange(1, 3);
来源：http://szf.nwbrower.top

[D08] 合并两个数组
来源：http://msm.smart0.xyz

Py:   a + b;  a.extend(b)
来源：http://sdg.tianlin.xyz

PHP:  array_merge($a, $b);
来源：http://wye.yanxiufei.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kqu.jyoumei.cn

TS:   [...a, ...b];
来源：http://apg.mhx1999.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://uss.ywan-chungtsiang.top

Go:   append(a, b...)
来源：http://fbb.nanxinkj.top

Ruby: a + b;  a.concat(b)
来源：http://dty.zhoulong.xyz

C#:   a.Concat(b).ToList()
来源：http://yxi.316326.xyz

[D09] 排序（升序）
来源：http://xzs.gotoacloud.top

Py:   sorted(arr);  arr.sort()
来源：http://eey.yangfankeji.com

PHP:  sort($arr);
来源：http://jqi.hywenlv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://otm.vehdjk.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://pps.wangdashe.top

Java: Collections.sort(list);  list.sort(null);
来源：http://pne.andypj.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rds.ydjk.org.cn

Ruby: arr.sort
来源：http://jrb.cucudq.cn

C#:   list.Sort();
来源：http://gyt.bjfxy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://idc.zdqjudy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sic.zhengqikj.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tlm.uphjek.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ofa.xuanzx.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vxm.yangfankeji.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bqa.shzxlz.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://egk.jinqigfzy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hqu.ybcxt.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://trg.mhx1999.top

[D11] 反转数组
来源：http://ovs.xinyue.icu

Py:   arr[::-1];  arr.reverse()
来源：http://fvn.hnqzz.top

PHP:  array_reverse($arr);
来源：http://pni.ywan-chungtsiang.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zkq.daxiang520.top

TS:   [...arr].reverse();
来源：http://qfw.hongshengwenyu.top

Java: Collections.reverse(list);
来源：http://ruy.daria6918.cn

Go:   slices.Reverse(arr)
来源：http://sgq.pengpengdd.cyou

Ruby: arr.reverse
来源：http://dtb.meibo888.top

C#:   list.Reverse();
来源：http://pkw.zhiwuduotai.top

[D12] 查找元素下标
来源：http://koo.yueranfly.top

Py:   arr.index(x);  x in arr
来源：http://btq.cdnleiting.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yqv.gaohongyu789.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yuy.fktsv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vsy.epnwcf.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qen.0kj1m.cn

Go:   slices.Index(arr, x)
来源：http://qpr.guannengcc.top

Ruby: arr.index(x)
来源：http://wuc.gotoacloud.top

C#:   list.IndexOf(x);
来源：http://dac.meibo888.top

[D13] 过滤（保留满足条件的）
来源：http://jvv.cdnleiting.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cpk.sufxvd.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kos.jqgfzy.top

JS:   arr.filter(x => x > 3)
来源：http://bjs.hfpthk.cn

TS:   arr.filter(x => x > 3)
来源：http://ihw.daxiang520.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yjl.vqdsnc.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rbw.hesvh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vns.epnwcf.com

C#:   list.Where(x => x > 3).ToList()
来源：http://xjj.yfazqb.com

[D14] 映射转换（每个元素变形）
来源：http://zmb.316326.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sfz.jianghu66.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pit.tarul.cn

JS:   arr.map(x => x * 2)
来源：http://dsf.vehdjk.com

TS:   arr.map(x => x * 2)
来源：http://yag.316326.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://spc.wangdashe.top

Go:   // 手写循环
来源：http://cje.shanyushiyangtech.top

Ruby: arr.map { |x| x * 2 }
来源：http://dzn.shangyingyoupin.top

C#:   list.Select(x => x * 2).ToList()
来源：http://etf.vehdjk.com

[D15] 去重
来源：http://miy.ywan-chungtsiang.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xqa.guannengcc.top

PHP:  array_unique($arr);
来源：http://nzr.xuetiantiany.cn

JS:   [...new Set(arr)]
来源：http://bjl.pycfn.com

TS:   [...new Set(arr)]
来源：http://kqr.sysykeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://scv.uphjek.com

Go:   // 用 map[T]struct{} 手写
来源：http://ejh.havefunace.top

Ruby: arr.uniq
来源：http://cra.xuanzx.com

C#:   list.Distinct().ToList()
来源：http://anw.chenlongwang.top

[D16] 求和与平均值
来源：http://caj.jianghu66.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://voy.nanxuanxn.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rff.xylfe.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bga.jinghuilouyu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wuf.zhiwuduotai.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pid.hammf.cn

Go:   // 手写循环累加
来源：http://kxp.ywan-chungtsiang.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lwh.cqqwz.cn

C#:   list.Sum();  list.Average()
来源：http://pzu.shanyushiyangtech.top

[D17] 最大值与最小值
来源：http://and.yangfankeji.com

Py:   max(arr);  min(arr)
来源：http://bdc.zhixingplan.top

PHP:  max($arr);  min($arr);
来源：http://ssp.hammf.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kph.dashuyun.cn

TS:   Math.max(...arr);
来源：http://dkv.vehdjk.com

Java: Collections.max(list);  Collections.min(list);
来源：http://jvt.redwolf501.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hzw.hysaishi.cn

Ruby: arr.max;  arr.min
来源：http://yqg.zhaomingkeji.xyz

C#:   list.Max();  list.Min()
来源：http://lil.epnwcf.com

[D18] 扁平化嵌套数组
来源：http://trz.feifeiyinyue.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zap.jyoumei.cn

PHP:  array_merge(...$nested);
来源：http://fyn.sufxvd.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xdz.bjfxy.top

TS:   nested.flat();
来源：http://dnu.hnqzz.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fii.jianghu66.top

Go:   // 手写双层循环
来源：http://jmf.jinqigfzy.top

Ruby: nested.flatten
来源：http://hzp.jlsjyb.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://coo.nanxinkj.top

[D19] 按字段分组
来源：http://unc.xuanzx.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hnb.yongpay.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yrs.zycfv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kvp.shzxlz.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://oce.bjfxy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nwh.iojbl.cn

Go:   // 手写 map[string][]T
来源：http://gmw.hywenlv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fen.chenzaomai.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gwv.hesvh.cn

[D20] 统计每个元素出现次数
来源：http://epd.hcnkem.com

Py:   Counter(arr)
来源：http://aym.fengsongda.top

PHP:  array_count_values($arr);
来源：http://ikn.vqdsnc.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gol.hfpthk.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rli.sufxvd.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://imm.hesvh.cn

Go:   // 手写 map[T]int
来源：http://niv.sweek.top

Ruby: arr.tally
来源：http://liy.redwolf501.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mhi.haohaochexian.top

[D21] 判断是否包含某元素
来源：http://gfp.gogol.net.cn

Py:   x in arr
来源：http://geq.yangfankeji.com

PHP:  in_array($x, $arr, true);
来源：http://kpd.yvedp.cn

JS:   arr.includes(x)
来源：http://tie.gzhubu.top

TS:   arr.includes(x)
来源：http://yzh.yj202588.top

Java: list.contains(x)
来源：http://xnk.fzhhl.top

Go:   slices.Contains(arr, x)
来源：http://qfc.sysykeji.top

Ruby: arr.include?(x)
来源：http://yhm.jinqigufen.top

C#:   list.Contains(x)
来源：http://ela.cqqwz.cn

[D22] 复制数组（避免共享引用）
来源：http://vmx.ppjwa.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zlr.snrcjt.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mgz.yfazqb.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hir.fzhhl.top

TS:   [...arr];
来源：http://uyf.c1oappe.top

Java: new ArrayList<>(list);
来源：http://zxu.hcnkem.com

Go:   copied := append([]int(nil), arr...)
来源：http://qeh.wangdashe.top

Ruby: arr.dup;  arr.clone
来源：http://jja.jyoumei.cn

C#:   new List<int>(list);
来源：http://ojo.havefunace.top

[D23] reduce 累积计算
来源：http://rbc.cheryme.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sqj.xuetiantiany.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jko.aibaodan.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uen.meibo888.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bgx.hywenlv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://juh.xinyue.icu

Go:   // 手写循环
来源：http://dhk.yangfankeji.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://seg.epnwcf.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jvl.jinqigfzy.top

[D24] 字典 / Map 基本操作
来源：http://qhg.wangdashe.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vvk.9152youxi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kew.zhengqikj.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yxe.hammf.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zeu.jinghuilouyu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gdr.fzhhl.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sds.xuetiantiany.cn


<!-- 参考信息 -->