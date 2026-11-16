代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://cde.yongpay.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://aza.hnqzz.top

Java: import java.util.List;
来源：http://inb.jianghu66.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mxc.gaohongyu789.top

Ruby: require "json"; require_relative "./util"
来源：http://xgn.vehdjk.com

C#:   using System.Text;
来源：http://vrq.chenlongwang.top

[C12] 立即执行函数 IIFE
来源：http://xox.birdmap.top

Py:   (lambda: print("run"))()
来源：http://pzx.zhijiandao.cn

PHP:  (function () { echo "run"; })();
来源：http://dko.jinghuilouyu.cn

JS:   (() => { console.log("run"); })();
来源：http://bgo.feifeiyinyue.top

TS:   (() => { console.log("run"); })();
来源：http://rvn.zycfv.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lza.daria6918.cn

Go:   func() { fmt.Println("run") }()
来源：http://bii.uphjek.com

Ruby: -> { puts "run" }.call
来源：http://qyc.yanxiufei.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xwb.bbcook.cn

[C13] 类型声明 / 类型注解
来源：http://acu.ehwqpu.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gio.jyoumei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cpa.zhixingplan.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ytd.yvedp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://txe.tianlin.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://gsj.xuanzx.com

Go:   func add(a, b int) int
来源：http://plz.jinqigfzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mhc.chenlongwang.top

C#:   int Add(int a, int b) => a + b;
来源：http://kuq.fengsongda.top

[C14] 泛型函数
来源：http://hug.tarul.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tgt.vehdjk.com

PHP:  // 无泛型
来源：http://plt.hysaishi.cn

JS:   // 无泛型
来源：http://iyq.yvedp.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://knl.hnxiangtu.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yer.jinghuilouyu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://faw.dianchejie.cn

Ruby: # 无泛型
来源：http://npv.zhoulong.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://swb.fehbvm.com

[C15] 解构 / 展开参数
来源：http://cuf.epnwcf.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://riv.ivvv.top

PHP:  [$a, $b] = $pair;
来源：http://old.jqgfzy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gry.havefunace.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://liz.shanyushiyangtech.top

Java: // 无解构
来源：http://gqx.sufxvd.cn

Go:   // 无解构
来源：http://sfn.gzhubu.top

Ruby: a, b = pair
来源：http://ypi.fzhhl.top

C#:   var (a, b) = pair;
来源：http://oeb.gogol.net.cn

[C16] 函数 / 方法重载
来源：http://vej.snrcjt.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tgk.9152youxi.cn

PHP:  // 无重载
来源：http://bbi.dashuyun.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://vpc.zycfv.cn

TS:   // 用联合类型或重载签名声明
来源：http://bpx.gaohongyu789.top

Java: void f(int a) {}  void f(String a) {}
来源：http://mdj.xingfuxueyuan.xyz

Go:   // 无重载：用不同函数名
来源：http://bll.shanyushiyangkeji.top

Ruby: # 无重载：靠动态参数
来源：http://bin.wangshuangyany.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xgf.ybcxt.top

================================================================================
来源：http://qlt.dashuyun.cn

D. 数组 / 列表 / 集合
来源：http://xcm.zhongyouzk.top

================================================================================
来源：http://azc.mhx1999.top

[D01] 创建数组 / 列表
来源：http://pla.andypj.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://wgn.guannengcc.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rss.cheryme.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mhp.wangdashe.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://vkd.jlsjyb.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vpv.ctjpmb.com

Go:   arr := []int{1, 2, 3}
来源：http://mik.hongshengwenyu.top

Ruby: arr = [1, 2, 3]
来源：http://ipi.zdqjudy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://grb.pengpengdd.cyou

[D02] 追加元素到末尾
来源：http://nfo.shzxlz.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ygv.daxiang520.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://eug.jqgufenzy.top

JS:   arr.push(4);
来源：http://mih.yj202588.top

TS:   arr.push(4);
来源：http://mqv.cashguo.top

Java: list.add(4);
来源：http://qhm.xuetiantiany.cn

Go:   arr = append(arr, 4)
来源：http://paw.gaohongyu789.top

Ruby: arr << 4; arr.push(5)
来源：http://rvp.yongpay.top

C#:   list.Add(4);
来源：http://yjf.wangshuangyany.cn

[D03] 在指定位置插入元素
来源：http://rmx.yonumen.top

Py:   arr.insert(0, 0)
来源：http://una.smart0.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://geb.zhongyouzk.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kwq.shangyingyoupin.top

TS:   arr.splice(0, 0, 0);
来源：http://zjz.xylfe.cn

Java: list.add(0, 0);
来源：http://fio.epnwcf.com

Go:   arr = append([]int{0}, arr...)
来源：http://fdn.fehbvm.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://alm.tianlin.xyz

C#:   list.Insert(0, 0);
来源：http://vlo.mhx1999.top

[D04] 删除元素
来源：http://jck.havefunace.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://min.chenlongwang.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ymi.ydzc1.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://aou.jinqigfzy.top

TS:   arr.splice(0, 1);
来源：http://ifi.bjfxy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://whk.xingfuxueyuan.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dog.guowangkeji.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gfo.shzxlz.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://afh.uphjek.com

[D05] 访问与修改元素
来源：http://ohk.sweek.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zih.fzhhl.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kmv.vqdsnc.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pyr.birdmap.top

TS:   arr[0]; arr.at(-1);
来源：http://owk.wangdashe.top

Java: list.get(0); list.set(0, 9);
来源：http://rfa.guannengcc.top

Go:   arr[0]; arr[0] = 9
来源：http://yhd.cashguo.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ysg.meibo888.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://izd.quarkkingdee.top

[D06] 数组长度
来源：http://caa.feifeiyinyue.top

Py:   len(arr)
来源：http://ovx.cdnleiting.top

PHP:  count($arr);
来源：http://cnr.hammf.cn

JS:   arr.length
来源：http://frq.ppjwa.cn

TS:   arr.length
来源：http://way.tian-w.cn

Java: list.size();
来源：http://clf.tarul.cn

Go:   len(arr)
来源：http://ywb.shangyingyoupin.top

Ruby: arr.length; arr.size
来源：http://qvy.yuanzhike.top

C#:   list.Count;
来源：http://soc.ivvv.top

[D07] 切片 / 取子数组
来源：http://hpw.shzxlz.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ohj.c1oappe.top

PHP:  array_slice($arr, 1, 3);
来源：http://thk.andypj.xyz

JS:   arr.slice(1, 4);
来源：http://bci.epnwcf.com

TS:   arr.slice(1, 4);
来源：http://dah.ydzc1.top

Java: list.subList(1, 4);
来源：http://dhn.jinyuanbaomall.cn

Go:   arr[1:4]
来源：http://ted.gaohongyu789.top

Ruby: arr[1, 3]
来源：http://xaz.0kj1m.cn

C#:   list.GetRange(1, 3);
来源：http://qzn.0kj1m.cn

[D08] 合并两个数组
来源：http://jds.aibaodan.cn

Py:   a + b;  a.extend(b)
来源：http://fsr.vqdsnc.cn

PHP:  array_merge($a, $b);
来源：http://uom.pycfn.com

JS:   [...a, ...b];  a.concat(b);
来源：http://ode.pycfn.com

TS:   [...a, ...b];
来源：http://wox.daxiang520.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xhj.gotoacloud.top

Go:   append(a, b...)
来源：http://yco.ywan-chungtsiang.top

Ruby: a + b;  a.concat(b)
来源：http://xdt.zdbjq.cn

C#:   a.Concat(b).ToList()
来源：http://plg.smart0.xyz

[D09] 排序（升序）
来源：http://fpp.xuanzx.com

Py:   sorted(arr);  arr.sort()
来源：http://vxi.pengpengdd.cyou

PHP:  sort($arr);
来源：http://dks.shanyushiyangkeji.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mlw.yongpay.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://xjn.jqgufenzy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://fpy.xziqi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xsx.jinqigfzy.top

Ruby: arr.sort
来源：http://nyx.sufxvd.cn

C#:   list.Sort();
来源：http://him.ctjpmb.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://uwq.sysykeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jwh.hysaishi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yim.bjfxy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xbt.tanke756.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qik.xziqi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wxf.jinyuanbaomall.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xwb.xinyue.icu

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cwo.xingfuxueyuan.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://neu.cashguo.top

[D11] 反转数组
来源：http://zao.zhiwuduotai.top

Py:   arr[::-1];  arr.reverse()
来源：http://ejj.epnwcf.com

PHP:  array_reverse($arr);
来源：http://roy.jqgfzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jis.zhiwuduotai.top

TS:   [...arr].reverse();
来源：http://ent.fengsongda.top

Java: Collections.reverse(list);
来源：http://yzg.yuanzhike.top

Go:   slices.Reverse(arr)
来源：http://xom.yuxming.cn

Ruby: arr.reverse
来源：http://fuo.sysykeji.top

C#:   list.Reverse();
来源：http://wow.tarul.cn

[D12] 查找元素下标
来源：http://uic.jyoumei.cn

Py:   arr.index(x);  x in arr
来源：http://pwj.fanxiaobao.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xfh.xziqi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wqo.fanxiaobao.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jyd.wangshuangyany.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qbw.quarkkingdee.top

Go:   slices.Index(arr, x)
来源：http://ndy.shanyushiyangkeji.top

Ruby: arr.index(x)
来源：http://uct.jyoumei.cn

C#:   list.IndexOf(x);
来源：http://bby.ivvv.top

[D13] 过滤（保留满足条件的）
来源：http://ghf.ywan-chungtsiang.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vfb.sufxvd.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vsk.fanxiaobao.xyz

JS:   arr.filter(x => x > 3)
来源：http://bwh.daxiang520.top

TS:   arr.filter(x => x > 3)
来源：http://ccl.jyoumei.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dsq.vehdjk.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lka.cqqwz.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cfg.316326.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://vms.xinyue.icu

[D14] 映射转换（每个元素变形）
来源：http://kuk.chenzaomai.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hon.gaohongyu789.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fwm.xylfe.cn

JS:   arr.map(x => x * 2)
来源：http://jqp.yj202588.top

TS:   arr.map(x => x * 2)
来源：http://lwp.wangdashe.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://uut.yonumen.top

Go:   // 手写循环
来源：http://txp.cucudq.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vde.aizwys.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pkf.yj202588.top

[D15] 去重
来源：http://pjv.316326.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dxt.birdmap.top

PHP:  array_unique($arr);
来源：http://seq.jianghu66.top

JS:   [...new Set(arr)]
来源：http://lom.hnqzz.top

TS:   [...new Set(arr)]
来源：http://gzy.shzxlz.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vjh.guowangkeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://rge.jinyuanbaomall.cn

Ruby: arr.uniq
来源：http://vnp.tianlin.xyz

C#:   list.Distinct().ToList()
来源：http://ffo.quarkkingdee.top

[D16] 求和与平均值
来源：http://nco.vehdjk.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ldi.hysaishi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sgm.fengsongda.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cop.quarkkingdee.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rsx.cashguo.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gpc.ctjpmb.com

Go:   // 手写循环累加
来源：http://tkc.yanxiufei.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zit.snrcjt.cn

C#:   list.Sum();  list.Average()
来源：http://hzu.hammf.cn

[D17] 最大值与最小值
来源：http://oab.fzhhl.top

Py:   max(arr);  min(arr)
来源：http://ati.hongshengwenyu.top

PHP:  max($arr);  min($arr);
来源：http://bfg.ivvv.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wln.zhongyouzk.top

TS:   Math.max(...arr);
来源：http://ang.uphjek.com

Java: Collections.max(list);  Collections.min(list);
来源：http://mpp.sufxvd.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xoe.daxiang520.top

Ruby: arr.max;  arr.min
来源：http://pbh.wangshuangyany.cn

C#:   list.Max();  list.Min()
来源：http://jhq.chenjidiqi.icu

[D18] 扁平化嵌套数组
来源：http://rux.ybcxt.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lwr.cqqwz.cn

PHP:  array_merge(...$nested);
来源：http://gol.aizwys.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rtp.shzxlz.cn

TS:   nested.flat();
来源：http://gvq.svipenyu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ylp.chenjidiqi.icu

Go:   // 手写双层循环
来源：http://iyn.sjlbkw.cn

Ruby: nested.flatten
来源：http://cbt.shanyushiyangtech.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ukk.hfpthk.cn

[D19] 按字段分组
来源：http://fen.zdbjq.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ahc.316326.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qxq.feifeiyinyue.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sol.ydzc1.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://rea.cucudq.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ewv.sjlbkw.cn

Go:   // 手写 map[string][]T
来源：http://bio.zhijiandao.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://kkk.cashguo.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qde.pengpengdd.cyou

[D20] 统计每个元素出现次数
来源：http://ghp.hammf.cn

Py:   Counter(arr)
来源：http://xsn.birdmap.top

PHP:  array_count_values($arr);
来源：http://pvr.yongpay.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mhu.ywan-chungtsiang.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fef.jinqigfzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kpt.fanxiaobao.xyz

Go:   // 手写 map[T]int
来源：http://yvs.yuxming.cn

Ruby: arr.tally
来源：http://hay.cqqwz.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://iiy.fehbvm.com

[D21] 判断是否包含某元素
来源：http://enl.yvedp.cn

Py:   x in arr
来源：http://ymk.gzhubu.top

PHP:  in_array($x, $arr, true);
来源：http://axg.chenzaomai.com

JS:   arr.includes(x)
来源：http://ezu.epnwcf.com

TS:   arr.includes(x)
来源：http://loy.sufxvd.cn

Java: list.contains(x)
来源：http://wie.ybcxt.top

Go:   slices.Contains(arr, x)
来源：http://qux.jqgufenzy.top

Ruby: arr.include?(x)
来源：http://cws.zdbjq.cn

C#:   list.Contains(x)
来源：http://bko.shangyingyoupin.top

[D22] 复制数组（避免共享引用）
来源：http://yjj.zhoulong.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rsb.xuanzx.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wxb.jinqigfzy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://eoe.shzxlz.cn

TS:   [...arr];
来源：http://ttd.fengsongda.top

Java: new ArrayList<>(list);
来源：http://pbc.jqgufenzy.top

Go:   copied := append([]int(nil), arr...)
来源：http://caq.kuanghao11.cn

Ruby: arr.dup;  arr.clone
来源：http://gpq.tianlin.xyz

C#:   new List<int>(list);
来源：http://vdv.yongpay.top

[D23] reduce 累积计算
来源：http://zqc.c1oappe.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xmb.dashuyun.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rld.cdnleiting.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ira.yuxming.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uns.jqgufenzy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://gsq.pengpengdd.cyou

Go:   // 手写循环
来源：http://fca.uphjek.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qnv.bbcook.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://igs.ydjk.org.cn

[D24] 字典 / Map 基本操作
来源：http://ahs.ywan-chungtsiang.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ncr.yanxiufei.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sap.ydjk.org.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tgr.jinqigfzy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://aov.yuanzhike.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sxt.ctjpmb.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kqt.wangdashe.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nkm.fehbvm.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mex.tianlin.xyz

[D25] Set 集合去重与交并差
来源：http://lpw.xylfe.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bfk.jiagoushi.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bpk.hongshengwenyu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://svw.kuanghao11.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://leh.jqgufenzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hdk.hnxiangtu.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gnq.jinghuilouyu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://inu.vqdsnc.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://oez.dashuyun.cn

[D26] 数组转字符串
来源：http://lcg.hysaishi.cn

Py:   ", ".join(map(str, arr))
来源：http://mhh.daxiang520.top

PHP:  implode(", ", $arr);
来源：http://tcg.birdmap.top

JS:   arr.join(", ")
来源：http://hme.ydzc1.top

TS:   arr.join(", ")
来源：http://vuj.hongshengwenyu.top

Java: String.join(", ", list)
来源：http://vay.jqgufenzy.top

Go:   strings.Join(strs, ", ")
来源：http://swv.jiagoushi.top

Ruby: arr.join(", ")
来源：http://xhu.cucudq.cn

C#:   string.Join(", ", list)
来源：http://itt.cdnleiting.top

================================================================================
来源：http://ddc.vehdjk.com

E. 字符串处理
来源：http://tmy.tarul.cn

================================================================================
来源：http://zja.9152youxi.cn

[E01] 拼接字符串
来源：http://tub.jinghuilouyu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://osx.haohaochexian.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rkc.sxryk.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pzv.zhixingplan.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ewm.cheryme.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jtz.9152youxi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mlz.dianchejie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jyx.sweek.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lnm.chenzaomai.com


<!-- 参考信息 -->