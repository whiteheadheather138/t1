代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ryx.gzhubu.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nlk.shanyushiyangkeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hqj.gaohongyu789.top

[C09] 递归
来源：http://ehk.cashguo.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://crd.nanxinkj.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://alm.zhoulong.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mfq.cashguo.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lty.xuanzx.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rpa.jinghuilouyu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tnh.smart0.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ujy.yvedp.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://apv.wangdashe.top

[C10] 变量作用域
来源：http://jrh.zhixingplan.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wpr.havefunace.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fwo.pycfn.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://csl.cdnleiting.top

TS:   同 JS
来源：http://ifp.ywan-chungtsiang.top

Java: 方法内为块级作用域
来源：http://nub.52xcode.cn

Go:   花括号块级作用域
来源：http://ylc.redwolf501.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://afn.hysaishi.cn

C#:   块级作用域
来源：http://kpn.aizwys.cn

[C11] 模块导入与导出
来源：http://bct.nwbrower.top

Py:   from module import func
来源：http://qhw.fengsongda.top

PHP:  require "file.php";  或 use App\Service;
来源：http://grm.mhx1999.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://nkp.hnqzz.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://oor.dianchejie.cn

Java: import java.util.List;
来源：http://ajz.fanxiaobao.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qfx.9152youxi.cn

Ruby: require "json"; require_relative "./util"
来源：http://vzl.mhx1999.top

C#:   using System.Text;
来源：http://dhk.ydjk.org.cn

[C12] 立即执行函数 IIFE
来源：http://pkg.hammf.cn

Py:   (lambda: print("run"))()
来源：http://bvj.tian-w.cn

PHP:  (function () { echo "run"; })();
来源：http://ocu.hammf.cn

JS:   (() => { console.log("run"); })();
来源：http://fwo.jqgfzy.top

TS:   (() => { console.log("run"); })();
来源：http://lya.tarul.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://utx.yj20258888.top

Go:   func() { fmt.Println("run") }()
来源：http://aqf.bjfxy.top

Ruby: -> { puts "run" }.call
来源：http://xys.vqdsnc.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://obi.svipenyu.cn

[C13] 类型声明 / 类型注解
来源：http://umg.sxryk.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qse.zhongyouzk.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qjp.ydzc1.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fyw.tarul.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://grv.sweek.top

Java: int add(int a, int b) { return a + b; }
来源：http://sqs.zhongyouzk.top

Go:   func add(a, b int) int
来源：http://rtc.cqqwz.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kve.redwolf501.top

C#:   int Add(int a, int b) => a + b;
来源：http://ggr.fehbvm.com

[C14] 泛型函数
来源：http://asr.cashguo.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vzi.andypj.xyz

PHP:  // 无泛型
来源：http://apm.hywenlv.cn

JS:   // 无泛型
来源：http://xck.guannengcc.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tst.yonumen.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mgn.aibaodan.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://apw.ydzc1.top

Ruby: # 无泛型
来源：http://dxr.jqgufenzy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tnn.redwolf501.top

[C15] 解构 / 展开参数
来源：http://tnc.cucudq.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wxu.shangyingyoupin.top

PHP:  [$a, $b] = $pair;
来源：http://jnb.tianlin.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zve.jinyuanbaomall.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nmn.pengpengdd.cyou

Java: // 无解构
来源：http://npb.yonumen.top

Go:   // 无解构
来源：http://kyy.havefunace.top

Ruby: a, b = pair
来源：http://pqk.ehwqpu.com

C#:   var (a, b) = pair;
来源：http://bjl.smart0.xyz

[C16] 函数 / 方法重载
来源：http://kqd.ppjwa.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vhu.meibo888.top

PHP:  // 无重载
来源：http://fng.shuidangran.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://oei.pycfn.com

TS:   // 用联合类型或重载签名声明
来源：http://wki.ydjk.org.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ksa.nanxinkj.top

Go:   // 无重载：用不同函数名
来源：http://ems.tianlin.xyz

Ruby: # 无重载：靠动态参数
来源：http://unl.kuanghao11.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://kly.tian-w.cn

================================================================================
来源：http://xqp.quarkkingdee.top

D. 数组 / 列表 / 集合
来源：http://kwt.hesvh.cn

================================================================================
来源：http://xmt.fktsv.cn

[D01] 创建数组 / 列表
来源：http://tkh.jyoumei.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qzx.andypj.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fpa.xingfuxueyuan.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lej.bjfxy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://zti.jqgufenzy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vro.zhongyouzk.top

Go:   arr := []int{1, 2, 3}
来源：http://isg.meibo888.top

Ruby: arr = [1, 2, 3]
来源：http://reg.zhiwuduotai.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://csv.zhengqikj.top

[D02] 追加元素到末尾
来源：http://aij.gogol.net.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kfv.fanxiaobao.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mvd.jqgufenzy.top

JS:   arr.push(4);
来源：http://kut.daria6918.cn

TS:   arr.push(4);
来源：http://hqv.jinqigufen.top

Java: list.add(4);
来源：http://zlx.yonumen.top

Go:   arr = append(arr, 4)
来源：http://sqp.yonumen.top

Ruby: arr << 4; arr.push(5)
来源：http://nab.haohaochexian.top

C#:   list.Add(4);
来源：http://xbw.9152youxi.cn

[D03] 在指定位置插入元素
来源：http://ija.shanyushiyangtech.top

Py:   arr.insert(0, 0)
来源：http://xil.c1oappe.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bbk.zhiwuduotai.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zyi.ivvv.top

TS:   arr.splice(0, 0, 0);
来源：http://xfr.zhaomingkeji.xyz

Java: list.add(0, 0);
来源：http://mni.andypj.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://kqv.zhoulong.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ode.haohaochexian.top

C#:   list.Insert(0, 0);
来源：http://pim.yuanzhike.top

[D04] 删除元素
来源：http://kep.jinyuanbaomall.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wqi.jyoumei.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jdf.tianlin.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mmz.jinqigufen.top

TS:   arr.splice(0, 1);
来源：http://sbt.daria6918.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://msw.cheryme.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xif.nanxinkj.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://glj.sjlbkw.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kqa.cqqwz.cn

[D05] 访问与修改元素
来源：http://ere.svipenyu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nco.xylfe.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jry.sjlbkw.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dwd.fengsongda.top

TS:   arr[0]; arr.at(-1);
来源：http://dgc.hongshengwenyu.top

Java: list.get(0); list.set(0, 9);
来源：http://wmk.aizwys.cn

Go:   arr[0]; arr[0] = 9
来源：http://mme.yvedp.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mxv.kuanghao11.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uog.jinghuilouyu.cn

[D06] 数组长度
来源：http://hxk.fengsongda.top

Py:   len(arr)
来源：http://pxk.quarkkingdee.top

PHP:  count($arr);
来源：http://rax.hammf.cn

JS:   arr.length
来源：http://yga.gogol.net.cn

TS:   arr.length
来源：http://uhc.cheryme.top

Java: list.size();
来源：http://lqn.ehwqpu.com

Go:   len(arr)
来源：http://dke.fktsv.cn

Ruby: arr.length; arr.size
来源：http://fpf.daxiang520.top

C#:   list.Count;
来源：http://dgh.yongpay.top

[D07] 切片 / 取子数组
来源：http://pcp.vehdjk.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tdb.sxryk.cn

PHP:  array_slice($arr, 1, 3);
来源：http://klu.ydzc1.top

JS:   arr.slice(1, 4);
来源：http://diz.ywan-chungtsiang.top

TS:   arr.slice(1, 4);
来源：http://wgq.yuanzhike.top

Java: list.subList(1, 4);
来源：http://nev.guannengcc.top

Go:   arr[1:4]
来源：http://ggk.tian-w.cn

Ruby: arr[1, 3]
来源：http://gsm.fanxiaobao.xyz

C#:   list.GetRange(1, 3);
来源：http://ivk.ybcxt.top

[D08] 合并两个数组
来源：http://uwy.fehbvm.com

Py:   a + b;  a.extend(b)
来源：http://rhl.jyoumei.cn

PHP:  array_merge($a, $b);
来源：http://dgp.shuidangran.top

JS:   [...a, ...b];  a.concat(b);
来源：http://gym.yj20258888.top

TS:   [...a, ...b];
来源：http://xtw.shanyushiyangkeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wtd.smart0.xyz

Go:   append(a, b...)
来源：http://ack.ydzc1.top

Ruby: a + b;  a.concat(b)
来源：http://twf.mhx1999.top

C#:   a.Concat(b).ToList()
来源：http://zdp.pengpengdd.cyou

[D09] 排序（升序）
来源：http://wuc.jianghu66.top

Py:   sorted(arr);  arr.sort()
来源：http://tdg.cdnleiting.top

PHP:  sort($arr);
来源：http://txv.shanyushiyangkeji.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lvr.ivvv.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://iwu.9152youxi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gvl.hcnkem.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xuo.chenjidiqi.icu

Ruby: arr.sort
来源：http://jpe.pycfn.com

C#:   list.Sort();
来源：http://qgl.meibo888.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://hoe.xylfe.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zlc.quarkkingdee.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ujq.cashguo.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tcq.xuanzx.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ojg.yonumen.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nca.hysaishi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lpi.yueranfly.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gmo.yfazqb.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mfk.yj20258888.top

[D11] 反转数组
来源：http://tlr.xuanzx.com

Py:   arr[::-1];  arr.reverse()
来源：http://pmk.wangdashe.top

PHP:  array_reverse($arr);
来源：http://cmt.bjfxy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vra.aizwys.cn

TS:   [...arr].reverse();
来源：http://qpu.cqqwz.cn

Java: Collections.reverse(list);
来源：http://ktm.fehbvm.com

Go:   slices.Reverse(arr)
来源：http://nxs.feifeiyinyue.top

Ruby: arr.reverse
来源：http://bft.jianghu66.top

C#:   list.Reverse();
来源：http://khb.shanyushiyangtech.top

[D12] 查找元素下标
来源：http://mku.birdmap.top

Py:   arr.index(x);  x in arr
来源：http://zll.jianghu66.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dql.hammf.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lpx.havefunace.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lar.jinghuilouyu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qsk.dashuyun.cn

Go:   slices.Index(arr, x)
来源：http://ibk.jqgfzy.top

Ruby: arr.index(x)
来源：http://qcj.sweek.top

C#:   list.IndexOf(x);
来源：http://zwx.zhongyouzk.top

[D13] 过滤（保留满足条件的）
来源：http://jrz.havefunace.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wte.meibo888.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ttb.pengpengdd.cyou

JS:   arr.filter(x => x > 3)
来源：http://cxx.fktsv.cn

TS:   arr.filter(x => x > 3)
来源：http://mos.jqgfzy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bzf.epnwcf.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qcj.wangdashe.top

Ruby: arr.select { |x| x > 3 }
来源：http://mff.iojbl.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://egp.gzhubu.top

[D14] 映射转换（每个元素变形）
来源：http://uax.iojbl.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://elo.jinyuanbaomall.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zuf.zhiwuduotai.top

JS:   arr.map(x => x * 2)
来源：http://dlb.cucudq.cn

TS:   arr.map(x => x * 2)
来源：http://tax.yuanzhike.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://dxb.yangfankeji.com

Go:   // 手写循环
来源：http://mhy.havefunace.top

Ruby: arr.map { |x| x * 2 }
来源：http://wim.hfpthk.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://laq.haohaochexian.top

[D15] 去重
来源：http://bhb.guowangkeji.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jvt.guannengcc.top

PHP:  array_unique($arr);
来源：http://ecd.yangfankeji.com

JS:   [...new Set(arr)]
来源：http://qzx.jinghuilouyu.cn

TS:   [...new Set(arr)]
来源：http://lxx.zhaomingkeji.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://szs.gzhubu.top

Go:   // 用 map[T]struct{} 手写
来源：http://ebv.kuanghao11.cn

Ruby: arr.uniq
来源：http://ety.nanxinkj.top

C#:   list.Distinct().ToList()
来源：http://asa.ivvv.top

[D16] 求和与平均值
来源：http://ngz.svipenyu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://aar.nanxuanxn.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qlz.dashuyun.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gra.gzhubu.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tsr.shanyushiyangkeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://teg.xingfuxueyuan.xyz

Go:   // 手写循环累加
来源：http://vkr.zhoulong.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uhz.cheryme.top

C#:   list.Sum();  list.Average()
来源：http://spo.snrcjt.cn

[D17] 最大值与最小值
来源：http://har.hywenlv.cn

Py:   max(arr);  min(arr)
来源：http://lae.wangshuangyany.cn

PHP:  max($arr);  min($arr);
来源：http://qsf.shzxlz.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://otk.316326.xyz

TS:   Math.max(...arr);
来源：http://vcv.0kj1m.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://nzi.yangfankeji.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://sas.yonumen.top

Ruby: arr.max;  arr.min
来源：http://nzj.yonumen.top

C#:   list.Max();  list.Min()
来源：http://eth.xuanzx.com

[D18] 扁平化嵌套数组
来源：http://jrr.hnqzz.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://svw.zdbjq.cn

PHP:  array_merge(...$nested);
来源：http://ars.0kj1m.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ltg.xuanzx.com

TS:   nested.flat();
来源：http://zuv.snrcjt.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lql.nanxuanxn.top

Go:   // 手写双层循环
来源：http://tvd.ctjpmb.com

Ruby: nested.flatten
来源：http://ohe.vqdsnc.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://pvp.jinghuilouyu.cn

[D19] 按字段分组
来源：http://msn.xingfuxueyuan.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://veg.meibo888.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nkx.birdmap.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wai.sxryk.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ljs.zhaomingkeji.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bao.iojbl.cn

Go:   // 手写 map[string][]T
来源：http://jpv.hcnkem.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://sbo.haohaochexian.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://txu.gaohongyu789.top

[D20] 统计每个元素出现次数
来源：http://ehb.316326.xyz

Py:   Counter(arr)
来源：http://yjz.tarul.cn

PHP:  array_count_values($arr);
来源：http://qul.sysykeji.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://quo.guowangkeji.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qqp.yj20258888.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vzv.yongpay.top

Go:   // 手写 map[T]int
来源：http://zfw.wangshuangyany.cn

Ruby: arr.tally
来源：http://guy.smart0.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cdp.nanxinkj.top

[D21] 判断是否包含某元素
来源：http://icw.shanyushiyangkeji.top

Py:   x in arr
来源：http://jft.zdbjq.cn

PHP:  in_array($x, $arr, true);
来源：http://wll.shangyingyoupin.top

JS:   arr.includes(x)
来源：http://gjk.yuxming.cn

TS:   arr.includes(x)
来源：http://ber.jinyuanbaomall.cn

Java: list.contains(x)
来源：http://hmn.zhiwuduotai.top

Go:   slices.Contains(arr, x)
来源：http://xzp.hcnkem.com

Ruby: arr.include?(x)
来源：http://kqz.sjlbkw.cn

C#:   list.Contains(x)
来源：http://ywj.redwolf501.top

[D22] 复制数组（避免共享引用）
来源：http://pdx.cucudq.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sak.snrcjt.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yok.jinqigufen.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qlv.vehdjk.com

TS:   [...arr];
来源：http://pze.jinqigufen.top

Java: new ArrayList<>(list);
来源：http://qps.zhixingplan.top

Go:   copied := append([]int(nil), arr...)
来源：http://zwa.yj202588.top

Ruby: arr.dup;  arr.clone
来源：http://iiv.chenjidiqi.icu

C#:   new List<int>(list);
来源：http://svy.jinyuanbaomall.cn

[D23] reduce 累积计算
来源：http://idp.gaohongyu789.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rqg.tanke756.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mlg.yj20258.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rsk.nanxuanxn.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sxp.jinqigfzy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://epb.c1oappe.top

Go:   // 手写循环
来源：http://ljw.hnqzz.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hld.fktsv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bdi.hnxiangtu.top

[D24] 字典 / Map 基本操作
来源：http://exv.ydzc1.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mqn.kuanghao11.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zlk.hysaishi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vvw.jlsjyb.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hdm.cucudq.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rtt.yongpay.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://etk.jqgfzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gqe.nanxuanxn.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://opd.ppjwa.cn

[D25] Set 集合去重与交并差
来源：http://fbc.yonumen.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dhc.c1oappe.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rdj.guannengcc.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fnb.guowangkeji.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ggw.fktsv.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nin.wangdashe.top


<!-- 参考信息 -->