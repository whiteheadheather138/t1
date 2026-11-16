代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://kqp.svipenyu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dtx.cheryme.top

Java: import java.util.List;
来源：http://mrl.yfazqb.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wnl.jinqigufen.top

Ruby: require "json"; require_relative "./util"
来源：http://qxp.hnqzz.top

C#:   using System.Text;
来源：http://fed.havefunace.top

[C12] 立即执行函数 IIFE
来源：http://lev.hnxiangtu.top

Py:   (lambda: print("run"))()
来源：http://xsn.pycfn.com

PHP:  (function () { echo "run"; })();
来源：http://nfa.guannengcc.top

JS:   (() => { console.log("run"); })();
来源：http://gca.haohaochexian.top

TS:   (() => { console.log("run"); })();
来源：http://yjp.yvedp.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qzf.guowangkeji.top

Go:   func() { fmt.Println("run") }()
来源：http://gpe.cheryme.top

Ruby: -> { puts "run" }.call
来源：http://ezy.xziqi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zmg.shanyushiyangtech.top

[C13] 类型声明 / 类型注解
来源：http://nvn.gotoacloud.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jmx.hongshengwenyu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gmx.gaohongyu789.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wzu.hysaishi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nfh.shanyushiyangtech.top

Java: int add(int a, int b) { return a + b; }
来源：http://wyf.cashguo.top

Go:   func add(a, b int) int
来源：http://srb.yfazqb.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tui.sufxvd.cn

C#:   int Add(int a, int b) => a + b;
来源：http://sqc.daria6918.cn

[C14] 泛型函数
来源：http://zeq.svipenyu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://inz.xingfuxueyuan.xyz

PHP:  // 无泛型
来源：http://fym.nanxinkj.top

JS:   // 无泛型
来源：http://fli.hesvh.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qcw.nanxuanxn.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pkr.jqgfzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qtu.xuanzx.com

Ruby: # 无泛型
来源：http://chq.zhijiandao.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mqc.shangyingyoupin.top

[C15] 解构 / 展开参数
来源：http://ikx.guannengcc.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yue.yuanzhike.top

PHP:  [$a, $b] = $pair;
来源：http://nmw.daxiang520.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kgq.haohaochexian.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ldj.tian-w.cn

Java: // 无解构
来源：http://kiy.chenzaomai.com

Go:   // 无解构
来源：http://sgc.cucudq.cn

Ruby: a, b = pair
来源：http://cen.hnqzz.top

C#:   var (a, b) = pair;
来源：http://cyh.xziqi.cn

[C16] 函数 / 方法重载
来源：http://ihp.chenjidiqi.icu

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ybm.nwbrower.top

PHP:  // 无重载
来源：http://vnl.cucudq.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://tju.hammf.cn

TS:   // 用联合类型或重载签名声明
来源：http://rgf.mhx1999.top

Java: void f(int a) {}  void f(String a) {}
来源：http://kyy.shangyingyoupin.top

Go:   // 无重载：用不同函数名
来源：http://qwp.hongshengwenyu.top

Ruby: # 无重载：靠动态参数
来源：http://igk.sxryk.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zgi.meibo888.top

================================================================================
来源：http://wnz.ydzc1.top

D. 数组 / 列表 / 集合
来源：http://zlo.tianlin.xyz

================================================================================
来源：http://edc.jyoumei.cn

[D01] 创建数组 / 列表
来源：http://iei.aibaodan.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://oqt.xinyue.icu

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cmi.chenlongwang.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qsi.pycfn.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://rri.aizwys.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://smo.yfazqb.com

Go:   arr := []int{1, 2, 3}
来源：http://lgu.jianghu66.top

Ruby: arr = [1, 2, 3]
来源：http://wac.yj20258888.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jpd.zhijiandao.cn

[D02] 追加元素到末尾
来源：http://pdc.shanyushiyangkeji.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://icw.nanxuanxn.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bah.shanyushiyangkeji.top

JS:   arr.push(4);
来源：http://dzc.xingfuxueyuan.xyz

TS:   arr.push(4);
来源：http://ody.gogol.net.cn

Java: list.add(4);
来源：http://hmu.jqgfzy.top

Go:   arr = append(arr, 4)
来源：http://zah.haohaochexian.top

Ruby: arr << 4; arr.push(5)
来源：http://rqr.cqqwz.cn

C#:   list.Add(4);
来源：http://cds.meibo888.top

[D03] 在指定位置插入元素
来源：http://qxf.vehdjk.com

Py:   arr.insert(0, 0)
来源：http://tmg.jqgfzy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mhz.fanxiaobao.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://iql.feifeiyinyue.top

TS:   arr.splice(0, 0, 0);
来源：http://mpc.ywan-chungtsiang.top

Java: list.add(0, 0);
来源：http://vqv.jianghu66.top

Go:   arr = append([]int{0}, arr...)
来源：http://ojw.zhiwuduotai.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mvc.9152youxi.cn

C#:   list.Insert(0, 0);
来源：http://evg.jqgfzy.top

[D04] 删除元素
来源：http://cdi.jyoumei.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wnh.zhaomingkeji.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dpe.ppjwa.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tuw.ydjk.org.cn

TS:   arr.splice(0, 1);
来源：http://aeg.yangfankeji.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://slf.kuanghao11.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tjs.xuetiantiany.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ufl.xylfe.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cob.epnwcf.com

[D05] 访问与修改元素
来源：http://eni.mhx1999.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://swb.iojbl.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ylj.ctjpmb.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dge.yonumen.top

TS:   arr[0]; arr.at(-1);
来源：http://rjb.aibaodan.cn

Java: list.get(0); list.set(0, 9);
来源：http://rbz.yueranfly.top

Go:   arr[0]; arr[0] = 9
来源：http://khi.shangyingyoupin.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zha.aibaodan.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bhu.gogol.net.cn

[D06] 数组长度
来源：http://ijp.xinyue.icu

Py:   len(arr)
来源：http://kaf.nwbrower.top

PHP:  count($arr);
来源：http://lrd.zhongyouzk.top

JS:   arr.length
来源：http://ugn.cdnleiting.top

TS:   arr.length
来源：http://euu.nwbrower.top

Java: list.size();
来源：http://ndu.tanke756.top

Go:   len(arr)
来源：http://xnk.wangdashe.top

Ruby: arr.length; arr.size
来源：http://bon.yuxming.cn

C#:   list.Count;
来源：http://ciw.daxiang520.top

[D07] 切片 / 取子数组
来源：http://xpo.hesvh.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://std.shanyushiyangtech.top

PHP:  array_slice($arr, 1, 3);
来源：http://kdl.kuanghao11.cn

JS:   arr.slice(1, 4);
来源：http://atj.zdbjq.cn

TS:   arr.slice(1, 4);
来源：http://glw.shzxlz.cn

Java: list.subList(1, 4);
来源：http://eea.tanke756.top

Go:   arr[1:4]
来源：http://yji.zdbjq.cn

Ruby: arr[1, 3]
来源：http://hef.feifeiyinyue.top

C#:   list.GetRange(1, 3);
来源：http://xem.jqgufenzy.top

[D08] 合并两个数组
来源：http://iqj.hysaishi.cn

Py:   a + b;  a.extend(b)
来源：http://drb.ivvv.top

PHP:  array_merge($a, $b);
来源：http://drs.nanxuanxn.top

JS:   [...a, ...b];  a.concat(b);
来源：http://eib.epnwcf.com

TS:   [...a, ...b];
来源：http://dmt.shzxlz.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://epj.vehdjk.com

Go:   append(a, b...)
来源：http://prl.yangfankeji.com

Ruby: a + b;  a.concat(b)
来源：http://eva.cheryme.top

C#:   a.Concat(b).ToList()
来源：http://wjq.birdmap.top

[D09] 排序（升序）
来源：http://imz.zdbjq.cn

Py:   sorted(arr);  arr.sort()
来源：http://jgc.guannengcc.top

PHP:  sort($arr);
来源：http://cra.pycfn.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fde.c1oappe.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://pqp.nwbrower.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ska.feifeiyinyue.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ccr.xylfe.cn

Ruby: arr.sort
来源：http://rlb.jqgufenzy.top

C#:   list.Sort();
来源：http://ylc.52xcode.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qxo.hnqzz.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qrr.epnwcf.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vyv.dashuyun.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://icg.shzxlz.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fuk.hywenlv.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ztb.52xcode.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tkf.hywenlv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mjw.daxiang520.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lto.xziqi.cn

[D11] 反转数组
来源：http://phn.yj202588.top

Py:   arr[::-1];  arr.reverse()
来源：http://okt.zhiwuduotai.top

PHP:  array_reverse($arr);
来源：http://lew.jinyuanbaomall.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://plh.hongshengwenyu.top

TS:   [...arr].reverse();
来源：http://dve.hfpthk.cn

Java: Collections.reverse(list);
来源：http://shc.haohaochexian.top

Go:   slices.Reverse(arr)
来源：http://mgn.yueranfly.top

Ruby: arr.reverse
来源：http://cfq.aizwys.cn

C#:   list.Reverse();
来源：http://hth.tian-w.cn

[D12] 查找元素下标
来源：http://wgo.ppjwa.cn

Py:   arr.index(x);  x in arr
来源：http://ifo.shzxlz.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kby.nwbrower.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mao.cdnleiting.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://djs.zhengqikj.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sap.yuanzhike.top

Go:   slices.Index(arr, x)
来源：http://fgp.sjlbkw.cn

Ruby: arr.index(x)
来源：http://ngh.yuanzhike.top

C#:   list.IndexOf(x);
来源：http://ruq.jinqigfzy.top

[D13] 过滤（保留满足条件的）
来源：http://jii.iojbl.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ook.xuetiantiany.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://eds.52xcode.cn

JS:   arr.filter(x => x > 3)
来源：http://upt.yangfankeji.com

TS:   arr.filter(x => x > 3)
来源：http://dgh.fehbvm.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fig.52xcode.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yvx.fanxiaobao.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://mzn.shuidangran.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ysd.tarul.cn

[D14] 映射转换（每个元素变形）
来源：http://qch.ydjk.org.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ksh.shangyingyoupin.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://eng.vehdjk.com

JS:   arr.map(x => x * 2)
来源：http://npl.jqgfzy.top

TS:   arr.map(x => x * 2)
来源：http://oza.feifeiyinyue.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://egp.shzxlz.cn

Go:   // 手写循环
来源：http://apb.jqgfzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://lco.tarul.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://gpf.gzhubu.top

[D15] 去重
来源：http://wby.ivvv.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cih.jinqigfzy.top

PHP:  array_unique($arr);
来源：http://xsu.hnqzz.top

JS:   [...new Set(arr)]
来源：http://zrw.tarul.cn

TS:   [...new Set(arr)]
来源：http://ahq.zhiwuduotai.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yjd.yonumen.top

Go:   // 用 map[T]struct{} 手写
来源：http://cwz.wangdashe.top

Ruby: arr.uniq
来源：http://wqe.nanxinkj.top

C#:   list.Distinct().ToList()
来源：http://byg.yuanzhike.top

[D16] 求和与平均值
来源：http://abr.shanyushiyangkeji.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://chg.cdnleiting.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mhy.shangyingyoupin.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qol.cashguo.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qcc.iojbl.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rmw.yfazqb.com

Go:   // 手写循环累加
来源：http://jdu.hongshengwenyu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nis.zhongyouzk.top

C#:   list.Sum();  list.Average()
来源：http://kzm.zhixingplan.top

[D17] 最大值与最小值
来源：http://lgu.wangdashe.top

Py:   max(arr);  min(arr)
来源：http://rbe.hnxiangtu.top

PHP:  max($arr);  min($arr);
来源：http://qvp.jlsjyb.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://egc.jqgufenzy.top

TS:   Math.max(...arr);
来源：http://lbq.hysaishi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jit.xuetiantiany.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ozq.cqqwz.cn

Ruby: arr.max;  arr.min
来源：http://fde.c1oappe.top

C#:   list.Max();  list.Min()
来源：http://hro.fzhhl.top

[D18] 扁平化嵌套数组
来源：http://sji.yueranfly.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dtd.sjlbkw.cn

PHP:  array_merge(...$nested);
来源：http://kuw.yuanzhike.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nxe.chenzaomai.com

TS:   nested.flat();
来源：http://zdj.316326.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zqy.zdqjudy.top

Go:   // 手写双层循环
来源：http://hfl.fehbvm.com

Ruby: nested.flatten
来源：http://djn.hnxiangtu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://wpt.aibaodan.cn

[D19] 按字段分组
来源：http://hjp.pycfn.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://oyt.sjlbkw.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://snj.zycfv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://itc.316326.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://jnc.dashuyun.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gcn.52xcode.cn

Go:   // 手写 map[string][]T
来源：http://dzq.epnwcf.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://ngd.hysaishi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wkp.cheryme.top

[D20] 统计每个元素出现次数
来源：http://lch.fengsongda.top

Py:   Counter(arr)
来源：http://qwe.zhaomingkeji.xyz

PHP:  array_count_values($arr);
来源：http://tlp.zycfv.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ypv.zhengqikj.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hoy.jianghu66.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vvf.c1oappe.top

Go:   // 手写 map[T]int
来源：http://ddd.svipenyu.cn

Ruby: arr.tally
来源：http://nrx.wangshuangyany.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bbb.zdbjq.cn

[D21] 判断是否包含某元素
来源：http://ugu.shanyushiyangtech.top

Py:   x in arr
来源：http://bfw.sufxvd.cn

PHP:  in_array($x, $arr, true);
来源：http://wjl.fanxiaobao.xyz

JS:   arr.includes(x)
来源：http://uum.gzhubu.top

TS:   arr.includes(x)
来源：http://aju.jyoumei.cn

Java: list.contains(x)
来源：http://wqs.kuanghao11.cn

Go:   slices.Contains(arr, x)
来源：http://egz.cqqwz.cn

Ruby: arr.include?(x)
来源：http://qsx.52xcode.cn

C#:   list.Contains(x)
来源：http://xxq.gaohongyu789.top

[D22] 复制数组（避免共享引用）
来源：http://pyi.hammf.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nxi.hongshengwenyu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ofv.yonumen.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bub.nanxuanxn.top

TS:   [...arr];
来源：http://aim.hcnkem.com

Java: new ArrayList<>(list);
来源：http://wox.9152youxi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ezd.sjlbkw.cn

Ruby: arr.dup;  arr.clone
来源：http://vav.zdbjq.cn

C#:   new List<int>(list);
来源：http://ery.nanxinkj.top

[D23] reduce 累积计算
来源：http://rfr.pengpengdd.cyou

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://peu.fzhhl.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yvk.bbcook.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jfk.fktsv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ogk.chenjidiqi.icu

Java: list.stream().reduce(0, Integer::sum)
来源：http://lby.andypj.xyz

Go:   // 手写循环
来源：http://gss.guannengcc.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mrz.chenjidiqi.icu

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://orr.sysykeji.top

[D24] 字典 / Map 基本操作
来源：http://avj.c1oappe.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wyh.jinqigfzy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kyy.gaohongyu789.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zqt.fehbvm.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qoq.zhijiandao.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jfl.wangdashe.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://iux.tanke756.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vwu.sufxvd.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://feh.ywan-chungtsiang.top

[D25] Set 集合去重与交并差
来源：http://fod.tianlin.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wgw.9152youxi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://joc.shangyingyoupin.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://whi.shangyingyoupin.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kjq.hnqzz.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vrj.tianlin.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://icf.ydjk.org.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mjn.hysaishi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xtz.kuanghao11.cn

[D26] 数组转字符串
来源：http://esz.aizwys.cn

Py:   ", ".join(map(str, arr))
来源：http://fpx.guowangkeji.top

PHP:  implode(", ", $arr);
来源：http://zwf.snrcjt.cn

JS:   arr.join(", ")
来源：http://yzb.hfpthk.cn

TS:   arr.join(", ")
来源：http://yxe.tanke756.top

Java: String.join(", ", list)
来源：http://wuj.zhixingplan.top

Go:   strings.Join(strs, ", ")
来源：http://ueu.cqqwz.cn

Ruby: arr.join(", ")
来源：http://gxv.fehbvm.com

C#:   string.Join(", ", list)
来源：http://ffs.chenzaomai.com

================================================================================
来源：http://gdo.zycfv.cn

E. 字符串处理
来源：http://fha.shzxlz.cn

================================================================================
来源：http://rrc.jianghu66.top

[E01] 拼接字符串
来源：http://cck.zhongyouzk.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kyc.cashguo.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qco.hnxiangtu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://puc.fehbvm.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://iyb.sufxvd.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mmu.jinghuilouyu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zyy.hcnkem.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lhp.quarkkingdee.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yqv.hongshengwenyu.top


<!-- 参考信息 -->