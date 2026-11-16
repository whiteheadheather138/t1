代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://egt.fzhhl.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://umr.fengsongda.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yng.hnxiangtu.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ndo.ybcxt.top

[C10] 变量作用域
来源：http://qlc.316326.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rbb.xuanzx.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ewt.nanxinkj.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fwg.yj20258888.top

TS:   同 JS
来源：http://nrc.redwolf501.top

Java: 方法内为块级作用域
来源：http://yfv.hcnkem.com

Go:   花括号块级作用域
来源：http://qqu.xinyue.icu

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rlv.jinqigufen.top

C#:   块级作用域
来源：http://ntk.jqgufenzy.top

[C11] 模块导入与导出
来源：http://bho.pengpengdd.cyou

Py:   from module import func
来源：http://ujg.yanxiufei.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://aau.smart0.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://jnk.tarul.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://thi.feifeiyinyue.top

Java: import java.util.List;
来源：http://mhm.sjlbkw.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fac.chenzaomai.com

Ruby: require "json"; require_relative "./util"
来源：http://jzl.yfazqb.com

C#:   using System.Text;
来源：http://txb.smart0.xyz

[C12] 立即执行函数 IIFE
来源：http://qme.sysykeji.top

Py:   (lambda: print("run"))()
来源：http://hks.jqgufenzy.top

PHP:  (function () { echo "run"; })();
来源：http://kex.aizwys.cn

JS:   (() => { console.log("run"); })();
来源：http://rnf.feifeiyinyue.top

TS:   (() => { console.log("run"); })();
来源：http://tvz.fzhhl.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fyw.andypj.xyz

Go:   func() { fmt.Println("run") }()
来源：http://zxf.cashguo.top

Ruby: -> { puts "run" }.call
来源：http://tpd.zhengqikj.top

C#:   // 无 IIFE：用静态构造函数
来源：http://faq.tianlin.xyz

[C13] 类型声明 / 类型注解
来源：http://ujq.gotoacloud.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://izh.meibo888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kmz.sjlbkw.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gqg.shuidangran.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bxu.gotoacloud.top

Java: int add(int a, int b) { return a + b; }
来源：http://xlz.hongshengwenyu.top

Go:   func add(a, b int) int
来源：http://ffm.hywenlv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pva.fehbvm.com

C#:   int Add(int a, int b) => a + b;
来源：http://ooa.shuidangran.top

[C14] 泛型函数
来源：http://cly.hywenlv.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hkd.yueranfly.top

PHP:  // 无泛型
来源：http://fdg.jinghuilouyu.cn

JS:   // 无泛型
来源：http://ukw.cheryme.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vlv.hcnkem.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bmj.fengsongda.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lfl.nwbrower.top

Ruby: # 无泛型
来源：http://wic.0kj1m.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://obk.ydzc1.top

[C15] 解构 / 展开参数
来源：http://jnv.zdbjq.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://raw.hammf.cn

PHP:  [$a, $b] = $pair;
来源：http://eoy.vehdjk.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uvd.jinyuanbaomall.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bzu.hesvh.cn

Java: // 无解构
来源：http://rsh.yangfankeji.com

Go:   // 无解构
来源：http://uhp.xinyue.icu

Ruby: a, b = pair
来源：http://bqs.pengpengdd.cyou

C#:   var (a, b) = pair;
来源：http://axd.cdnleiting.top

[C16] 函数 / 方法重载
来源：http://nsj.hysaishi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://oqc.bjfxy.top

PHP:  // 无重载
来源：http://qpw.redwolf501.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://cpr.guowangkeji.top

TS:   // 用联合类型或重载签名声明
来源：http://phh.chenlongwang.top

Java: void f(int a) {}  void f(String a) {}
来源：http://zav.yj202588.top

Go:   // 无重载：用不同函数名
来源：http://cju.chenlongwang.top

Ruby: # 无重载：靠动态参数
来源：http://zwn.jqgfzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://oht.vehdjk.com

================================================================================
来源：http://vgr.dashuyun.cn

D. 数组 / 列表 / 集合
来源：http://ywi.tian-w.cn

================================================================================
来源：http://plj.fehbvm.com

[D01] 创建数组 / 列表
来源：http://uxd.ctjpmb.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://zvy.hnqzz.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xqi.ctjpmb.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://szd.feifeiyinyue.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://rfv.hysaishi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tfg.cashguo.top

Go:   arr := []int{1, 2, 3}
来源：http://wfo.shangyingyoupin.top

Ruby: arr = [1, 2, 3]
来源：http://ijl.yangfankeji.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://iyq.fengsongda.top

[D02] 追加元素到末尾
来源：http://biv.cucudq.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://iqx.jlsjyb.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zwr.nwbrower.top

JS:   arr.push(4);
来源：http://juc.zhiwuduotai.top

TS:   arr.push(4);
来源：http://rer.hammf.cn

Java: list.add(4);
来源：http://ljy.zhijiandao.cn

Go:   arr = append(arr, 4)
来源：http://wmx.hnxiangtu.top

Ruby: arr << 4; arr.push(5)
来源：http://efo.zdqjudy.top

C#:   list.Add(4);
来源：http://ixg.gotoacloud.top

[D03] 在指定位置插入元素
来源：http://fms.ehwqpu.com

Py:   arr.insert(0, 0)
来源：http://gvu.hnxiangtu.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ulw.pycfn.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ink.9152youxi.cn

TS:   arr.splice(0, 0, 0);
来源：http://ock.jinyuanbaomall.cn

Java: list.add(0, 0);
来源：http://moy.tanke756.top

Go:   arr = append([]int{0}, arr...)
来源：http://xzr.yuanzhike.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ebf.yuanzhike.top

C#:   list.Insert(0, 0);
来源：http://nzc.jqgfzy.top

[D04] 删除元素
来源：http://zfk.zhoulong.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xyr.svipenyu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yfc.ivvv.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nsz.yangfankeji.com

TS:   arr.splice(0, 1);
来源：http://jzv.iojbl.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gfh.yuxming.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jls.zhijiandao.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ovc.cheryme.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://suz.yvedp.cn

[D05] 访问与修改元素
来源：http://mwf.andypj.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yzx.bbcook.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xlo.tarul.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nwp.zhengqikj.top

TS:   arr[0]; arr.at(-1);
来源：http://hvc.zhiwuduotai.top

Java: list.get(0); list.set(0, 9);
来源：http://srm.cashguo.top

Go:   arr[0]; arr[0] = 9
来源：http://mkb.cashguo.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yer.tarul.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fbm.jinqigfzy.top

[D06] 数组长度
来源：http://hli.tarul.cn

Py:   len(arr)
来源：http://zww.ydzc1.top

PHP:  count($arr);
来源：http://rrk.yanxiufei.cn

JS:   arr.length
来源：http://xej.snrcjt.cn

TS:   arr.length
来源：http://dyh.yuxming.cn

Java: list.size();
来源：http://dbf.yongpay.top

Go:   len(arr)
来源：http://koi.jlsjyb.cn

Ruby: arr.length; arr.size
来源：http://mne.jqgufenzy.top

C#:   list.Count;
来源：http://tut.ybcxt.top

[D07] 切片 / 取子数组
来源：http://twj.sysykeji.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nbl.ehwqpu.com

PHP:  array_slice($arr, 1, 3);
来源：http://fjw.ydjk.org.cn

JS:   arr.slice(1, 4);
来源：http://ejo.yvedp.cn

TS:   arr.slice(1, 4);
来源：http://dwd.cdnleiting.top

Java: list.subList(1, 4);
来源：http://gjy.haohaochexian.top

Go:   arr[1:4]
来源：http://oop.ywan-chungtsiang.top

Ruby: arr[1, 3]
来源：http://ive.chenlongwang.top

C#:   list.GetRange(1, 3);
来源：http://cxd.fehbvm.com

[D08] 合并两个数组
来源：http://jos.yongpay.top

Py:   a + b;  a.extend(b)
来源：http://urw.smart0.xyz

PHP:  array_merge($a, $b);
来源：http://gnx.yangfankeji.com

JS:   [...a, ...b];  a.concat(b);
来源：http://oqx.xingfuxueyuan.xyz

TS:   [...a, ...b];
来源：http://unj.ivvv.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qiq.guannengcc.top

Go:   append(a, b...)
来源：http://zqv.ydjk.org.cn

Ruby: a + b;  a.concat(b)
来源：http://iqt.meibo888.top

C#:   a.Concat(b).ToList()
来源：http://edt.redwolf501.top

[D09] 排序（升序）
来源：http://vvf.zdqjudy.top

Py:   sorted(arr);  arr.sort()
来源：http://jkl.hesvh.cn

PHP:  sort($arr);
来源：http://odo.sweek.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ljn.0kj1m.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://jeo.pycfn.com

Java: Collections.sort(list);  list.sort(null);
来源：http://vcr.jyoumei.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://txu.yonumen.top

Ruby: arr.sort
来源：http://eud.fzhhl.top

C#:   list.Sort();
来源：http://ftl.chenlongwang.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://bdk.cheryme.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fyo.cheryme.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lpr.tianlin.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hsf.feifeiyinyue.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://txs.cdnleiting.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hwo.yuanzhike.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ufa.smart0.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://epm.jinghuilouyu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tzn.haohaochexian.top

[D11] 反转数组
来源：http://fsz.ybcxt.top

Py:   arr[::-1];  arr.reverse()
来源：http://aqu.daxiang520.top

PHP:  array_reverse($arr);
来源：http://eef.fanxiaobao.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jui.316326.xyz

TS:   [...arr].reverse();
来源：http://wrr.yuanzhike.top

Java: Collections.reverse(list);
来源：http://alf.dianchejie.cn

Go:   slices.Reverse(arr)
来源：http://jbb.aibaodan.cn

Ruby: arr.reverse
来源：http://byv.quarkkingdee.top

C#:   list.Reverse();
来源：http://ple.dashuyun.cn

[D12] 查找元素下标
来源：http://unf.bbcook.cn

Py:   arr.index(x);  x in arr
来源：http://twz.c1oappe.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://stf.hcnkem.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ooc.hfpthk.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eeg.mhx1999.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lmn.yongpay.top

Go:   slices.Index(arr, x)
来源：http://xkp.kuanghao11.cn

Ruby: arr.index(x)
来源：http://nqj.zdqjudy.top

C#:   list.IndexOf(x);
来源：http://lpc.zhengqikj.top

[D13] 过滤（保留满足条件的）
来源：http://uvv.yuanzhike.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xhy.fengsongda.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://afj.bjfxy.top

JS:   arr.filter(x => x > 3)
来源：http://ckv.dashuyun.cn

TS:   arr.filter(x => x > 3)
来源：http://nbb.tanke756.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zkb.xylfe.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fuz.shuidangran.top

Ruby: arr.select { |x| x > 3 }
来源：http://jza.yj20258.top

C#:   list.Where(x => x > 3).ToList()
来源：http://orr.pycfn.com

[D14] 映射转换（每个元素变形）
来源：http://umy.daria6918.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fdp.yueranfly.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qbl.jinyuanbaomall.cn

JS:   arr.map(x => x * 2)
来源：http://fja.cdnleiting.top

TS:   arr.map(x => x * 2)
来源：http://cho.ybcxt.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://spz.dashuyun.cn

Go:   // 手写循环
来源：http://wry.aibaodan.cn

Ruby: arr.map { |x| x * 2 }
来源：http://cds.haohaochexian.top

C#:   list.Select(x => x * 2).ToList()
来源：http://qgy.epnwcf.com

[D15] 去重
来源：http://sqp.xinyue.icu

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fjw.hysaishi.cn

PHP:  array_unique($arr);
来源：http://vfh.jqgfzy.top

JS:   [...new Set(arr)]
来源：http://eqe.hesvh.cn

TS:   [...new Set(arr)]
来源：http://kfh.52xcode.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hji.zhiwuduotai.top

Go:   // 用 map[T]struct{} 手写
来源：http://ncl.pengpengdd.cyou

Ruby: arr.uniq
来源：http://ias.daria6918.cn

C#:   list.Distinct().ToList()
来源：http://kvt.tarul.cn

[D16] 求和与平均值
来源：http://mcl.uphjek.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lpq.yueranfly.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tog.zhengqikj.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hfw.sweek.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ymx.hfpthk.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://iuq.ydzc1.top

Go:   // 手写循环累加
来源：http://hfj.jqgfzy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sld.cdnleiting.top

C#:   list.Sum();  list.Average()
来源：http://sbs.sxryk.cn

[D17] 最大值与最小值
来源：http://rhw.yueranfly.top

Py:   max(arr);  min(arr)
来源：http://ouy.jianghu66.top

PHP:  max($arr);  min($arr);
来源：http://bkk.ydzc1.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tfj.ydjk.org.cn

TS:   Math.max(...arr);
来源：http://qbl.0kj1m.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zhf.zhaomingkeji.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://djx.shuidangran.top

Ruby: arr.max;  arr.min
来源：http://qjq.yvedp.cn

C#:   list.Max();  list.Min()
来源：http://ppv.sufxvd.cn

[D18] 扁平化嵌套数组
来源：http://okz.dashuyun.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uhd.jiagoushi.top

PHP:  array_merge(...$nested);
来源：http://ccz.fktsv.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jqg.yuanzhike.top

TS:   nested.flat();
来源：http://cvn.zycfv.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tww.yuanzhike.top

Go:   // 手写双层循环
来源：http://hox.mhx1999.top

Ruby: nested.flatten
来源：http://egp.cqqwz.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kok.xuanzx.com

[D19] 按字段分组
来源：http://abz.wangshuangyany.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://egv.xuanzx.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vwp.cucudq.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yyu.ydzc1.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://aga.tarul.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ixs.zhaomingkeji.xyz

Go:   // 手写 map[string][]T
来源：http://wry.daria6918.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zir.pycfn.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://eoz.ydzc1.top

[D20] 统计每个元素出现次数
来源：http://utq.yueranfly.top

Py:   Counter(arr)
来源：http://xrf.ydzc1.top

PHP:  array_count_values($arr);
来源：http://cml.xingfuxueyuan.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cec.wangdashe.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zfq.yonumen.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tpr.yj202588.top

Go:   // 手写 map[T]int
来源：http://jjq.sjlbkw.cn

Ruby: arr.tally
来源：http://wgv.pycfn.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jkx.xylfe.cn

[D21] 判断是否包含某元素
来源：http://zam.ehwqpu.com

Py:   x in arr
来源：http://ncr.sufxvd.cn

PHP:  in_array($x, $arr, true);
来源：http://twi.xuanzx.com

JS:   arr.includes(x)
来源：http://abg.zhixingplan.top

TS:   arr.includes(x)
来源：http://nqc.yj20258888.top

Java: list.contains(x)
来源：http://qtg.sjlbkw.cn

Go:   slices.Contains(arr, x)
来源：http://bsv.daxiang520.top

Ruby: arr.include?(x)
来源：http://odm.ivvv.top

C#:   list.Contains(x)
来源：http://ygy.chenlongwang.top

[D22] 复制数组（避免共享引用）
来源：http://fnn.yj202588.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oss.fengsongda.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yxo.jqgufenzy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gpb.svipenyu.cn

TS:   [...arr];
来源：http://opk.cheryme.top

Java: new ArrayList<>(list);
来源：http://aht.chenjidiqi.icu

Go:   copied := append([]int(nil), arr...)
来源：http://rdf.havefunace.top

Ruby: arr.dup;  arr.clone
来源：http://bzq.jinqigufen.top

C#:   new List<int>(list);
来源：http://wua.shzxlz.cn

[D23] reduce 累积计算
来源：http://ofl.cqqwz.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://oix.gogol.net.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gwg.dianchejie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jmd.chenjidiqi.icu

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lxe.c1oappe.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ros.tian-w.cn

Go:   // 手写循环
来源：http://ubh.xziqi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://voj.tianlin.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://huf.ivvv.top

[D24] 字典 / Map 基本操作
来源：http://dua.haohaochexian.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pfc.ctjpmb.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://paw.zhoulong.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://uga.fanxiaobao.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vcx.nanxuanxn.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fhx.cdnleiting.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vlb.shzxlz.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vtv.tianlin.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zru.feifeiyinyue.top

[D25] Set 集合去重与交并差
来源：http://pdk.hnqzz.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nbd.meibo888.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bcs.feifeiyinyue.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wcy.shzxlz.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mli.nwbrower.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xch.ybcxt.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kkj.sweek.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bxw.sjlbkw.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zar.fktsv.cn

[D26] 数组转字符串
来源：http://eqs.xuanzx.com

Py:   ", ".join(map(str, arr))
来源：http://oub.redwolf501.top

PHP:  implode(", ", $arr);
来源：http://wzw.ybcxt.top

JS:   arr.join(", ")
来源：http://nzq.jinqigfzy.top

TS:   arr.join(", ")
来源：http://fay.yj20258888.top


<!-- 参考信息 -->