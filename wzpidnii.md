代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://doy.cdnleiting.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nlq.sysykeji.top

Java: import java.util.List;
来源：http://wul.shangyingyoupin.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bgq.52xcode.cn

Ruby: require "json"; require_relative "./util"
来源：http://dmf.iojbl.cn

C#:   using System.Text;
来源：http://xca.guowangkeji.top

[C12] 立即执行函数 IIFE
来源：http://qgt.yfazqb.com

Py:   (lambda: print("run"))()
来源：http://rec.uphjek.com

PHP:  (function () { echo "run"; })();
来源：http://idi.cqqwz.cn

JS:   (() => { console.log("run"); })();
来源：http://lpd.yuanzhike.top

TS:   (() => { console.log("run"); })();
来源：http://xyf.0kj1m.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://aio.wangdashe.top

Go:   func() { fmt.Println("run") }()
来源：http://dmi.yanxiufei.cn

Ruby: -> { puts "run" }.call
来源：http://wkm.jinqigfzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://mdc.smart0.xyz

[C13] 类型声明 / 类型注解
来源：http://may.jinqigufen.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hlj.zhijiandao.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qeh.hfpthk.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xsp.chenjidiqi.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rap.yj202588.top

Java: int add(int a, int b) { return a + b; }
来源：http://vdv.fzhhl.top

Go:   func add(a, b int) int
来源：http://hxa.yuxming.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wcq.cqqwz.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tot.sweek.top

[C14] 泛型函数
来源：http://iwa.tanke756.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://aho.mhx1999.top

PHP:  // 无泛型
来源：http://pyn.fengsongda.top

JS:   // 无泛型
来源：http://epy.zhengqikj.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://frk.9152youxi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://guz.ivvv.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pee.ydzc1.top

Ruby: # 无泛型
来源：http://jhy.smart0.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ufn.hywenlv.cn

[C15] 解构 / 展开参数
来源：http://xlf.aizwys.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nfh.xuetiantiany.cn

PHP:  [$a, $b] = $pair;
来源：http://yci.gogol.net.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yhc.yangfankeji.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kjo.gogol.net.cn

Java: // 无解构
来源：http://wmo.shzxlz.cn

Go:   // 无解构
来源：http://eop.nanxinkj.top

Ruby: a, b = pair
来源：http://qer.yj20258.top

C#:   var (a, b) = pair;
来源：http://psb.pycfn.com

[C16] 函数 / 方法重载
来源：http://msm.zycfv.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pst.zdbjq.cn

PHP:  // 无重载
来源：http://ibs.cqqwz.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ymd.fktsv.cn

TS:   // 用联合类型或重载签名声明
来源：http://twb.shzxlz.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://bkl.fengsongda.top

Go:   // 无重载：用不同函数名
来源：http://djd.pycfn.com

Ruby: # 无重载：靠动态参数
来源：http://fmp.daria6918.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rrx.zhixingplan.top

================================================================================
来源：http://flh.ybcxt.top

D. 数组 / 列表 / 集合
来源：http://lum.xuanzx.com

================================================================================
来源：http://wjq.yuxming.cn

[D01] 创建数组 / 列表
来源：http://rpx.bbcook.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mun.havefunace.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ocv.zdbjq.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rgy.feifeiyinyue.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://uzj.sysykeji.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wfq.nwbrower.top

Go:   arr := []int{1, 2, 3}
来源：http://qtg.hfpthk.cn

Ruby: arr = [1, 2, 3]
来源：http://hfz.shuidangran.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fgq.fzhhl.top

[D02] 追加元素到末尾
来源：http://tid.zhongyouzk.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://olc.c1oappe.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ozv.yuanzhike.top

JS:   arr.push(4);
来源：http://dsd.jinqigfzy.top

TS:   arr.push(4);
来源：http://aqe.chenjidiqi.icu

Java: list.add(4);
来源：http://jqd.gzhubu.top

Go:   arr = append(arr, 4)
来源：http://qrf.hfpthk.cn

Ruby: arr << 4; arr.push(5)
来源：http://gnz.gzhubu.top

C#:   list.Add(4);
来源：http://iom.cheryme.top

[D03] 在指定位置插入元素
来源：http://fov.zhongyouzk.top

Py:   arr.insert(0, 0)
来源：http://wuz.nanxinkj.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gcb.xingfuxueyuan.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zso.andypj.xyz

TS:   arr.splice(0, 0, 0);
来源：http://tcz.fanxiaobao.xyz

Java: list.add(0, 0);
来源：http://gvb.feifeiyinyue.top

Go:   arr = append([]int{0}, arr...)
来源：http://qsy.havefunace.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nvz.gzhubu.top

C#:   list.Insert(0, 0);
来源：http://cqf.shuidangran.top

[D04] 删除元素
来源：http://lkq.fktsv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://osj.jinyuanbaomall.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qqc.shanyushiyangtech.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uib.nanxinkj.top

TS:   arr.splice(0, 1);
来源：http://zdg.zycfv.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qyk.sjlbkw.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://oss.yueranfly.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xww.zhixingplan.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://frp.tarul.cn

[D05] 访问与修改元素
来源：http://jel.bbcook.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zdj.meibo888.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ihh.jlsjyb.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pwm.wangshuangyany.cn

TS:   arr[0]; arr.at(-1);
来源：http://xzy.pengpengdd.cyou

Java: list.get(0); list.set(0, 9);
来源：http://mnl.sysykeji.top

Go:   arr[0]; arr[0] = 9
来源：http://cfj.fanxiaobao.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mak.gzhubu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ehl.mhx1999.top

[D06] 数组长度
来源：http://mcn.cashguo.top

Py:   len(arr)
来源：http://hye.guowangkeji.top

PHP:  count($arr);
来源：http://gye.9152youxi.cn

JS:   arr.length
来源：http://jbz.pengpengdd.cyou

TS:   arr.length
来源：http://amu.9152youxi.cn

Java: list.size();
来源：http://kor.xuetiantiany.cn

Go:   len(arr)
来源：http://ovs.tarul.cn

Ruby: arr.length; arr.size
来源：http://wwh.9152youxi.cn

C#:   list.Count;
来源：http://imc.jinqigfzy.top

[D07] 切片 / 取子数组
来源：http://zen.quarkkingdee.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nxh.feifeiyinyue.top

PHP:  array_slice($arr, 1, 3);
来源：http://wen.yfazqb.com

JS:   arr.slice(1, 4);
来源：http://xqe.ydjk.org.cn

TS:   arr.slice(1, 4);
来源：http://vdg.zhengqikj.top

Java: list.subList(1, 4);
来源：http://iec.yanxiufei.cn

Go:   arr[1:4]
来源：http://uzz.redwolf501.top

Ruby: arr[1, 3]
来源：http://mcz.fehbvm.com

C#:   list.GetRange(1, 3);
来源：http://iuw.zdqjudy.top

[D08] 合并两个数组
来源：http://noi.mhx1999.top

Py:   a + b;  a.extend(b)
来源：http://joo.nanxinkj.top

PHP:  array_merge($a, $b);
来源：http://woy.chenzaomai.com

JS:   [...a, ...b];  a.concat(b);
来源：http://xpm.hnqzz.top

TS:   [...a, ...b];
来源：http://uvd.shuidangran.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fbx.0kj1m.cn

Go:   append(a, b...)
来源：http://qrc.daxiang520.top

Ruby: a + b;  a.concat(b)
来源：http://ymw.ehwqpu.com

C#:   a.Concat(b).ToList()
来源：http://isv.jqgfzy.top

[D09] 排序（升序）
来源：http://byg.iojbl.cn

Py:   sorted(arr);  arr.sort()
来源：http://lvz.ywan-chungtsiang.top

PHP:  sort($arr);
来源：http://hvc.shanyushiyangkeji.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fcb.hcnkem.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://yjd.mhx1999.top

Java: Collections.sort(list);  list.sort(null);
来源：http://mue.daxiang520.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mow.vqdsnc.cn

Ruby: arr.sort
来源：http://zaf.hfpthk.cn

C#:   list.Sort();
来源：http://gbq.cqqwz.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://udk.xziqi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://piq.hywenlv.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jmz.iojbl.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sot.vehdjk.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qxq.hcnkem.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dlo.svipenyu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://oou.tian-w.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ktv.shanyushiyangtech.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qwg.xuanzx.com

[D11] 反转数组
来源：http://xae.9152youxi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://csn.ppjwa.cn

PHP:  array_reverse($arr);
来源：http://oaz.aibaodan.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ksm.zhengqikj.top

TS:   [...arr].reverse();
来源：http://zhm.zhaomingkeji.xyz

Java: Collections.reverse(list);
来源：http://gaq.yj202588.top

Go:   slices.Reverse(arr)
来源：http://lnc.daxiang520.top

Ruby: arr.reverse
来源：http://yfz.tarul.cn

C#:   list.Reverse();
来源：http://tir.cashguo.top

[D12] 查找元素下标
来源：http://rzu.dianchejie.cn

Py:   arr.index(x);  x in arr
来源：http://ewg.cdnleiting.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ssx.zhongyouzk.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://neo.ydzc1.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gsk.nanxinkj.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qqv.havefunace.top

Go:   slices.Index(arr, x)
来源：http://plv.xuetiantiany.cn

Ruby: arr.index(x)
来源：http://hly.0kj1m.cn

C#:   list.IndexOf(x);
来源：http://aww.jinqigufen.top

[D13] 过滤（保留满足条件的）
来源：http://gxg.fanxiaobao.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xae.yuxming.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wvt.zhiwuduotai.top

JS:   arr.filter(x => x > 3)
来源：http://pcv.yvedp.cn

TS:   arr.filter(x => x > 3)
来源：http://wwx.cdnleiting.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://oxh.hcnkem.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dua.xziqi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ply.yangfankeji.com

C#:   list.Where(x => x > 3).ToList()
来源：http://hid.shzxlz.cn

[D14] 映射转换（每个元素变形）
来源：http://fgo.yueranfly.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uzs.havefunace.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ewu.zhengqikj.top

JS:   arr.map(x => x * 2)
来源：http://bni.ctjpmb.com

TS:   arr.map(x => x * 2)
来源：http://gsi.0kj1m.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://oiv.nwbrower.top

Go:   // 手写循环
来源：http://yia.jqgufenzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://jjd.jianghu66.top

C#:   list.Select(x => x * 2).ToList()
来源：http://bud.sufxvd.cn

[D15] 去重
来源：http://sqr.jianghu66.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yqp.guannengcc.top

PHP:  array_unique($arr);
来源：http://zxg.cucudq.cn

JS:   [...new Set(arr)]
来源：http://rys.fktsv.cn

TS:   [...new Set(arr)]
来源：http://elk.ctjpmb.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://phz.fengsongda.top

Go:   // 用 map[T]struct{} 手写
来源：http://ihq.zycfv.cn

Ruby: arr.uniq
来源：http://xjf.hammf.cn

C#:   list.Distinct().ToList()
来源：http://fqg.jinqigfzy.top

[D16] 求和与平均值
来源：http://uof.epnwcf.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tcc.hnqzz.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://eso.cheryme.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nfs.zhixingplan.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://maa.hysaishi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qgs.shanyushiyangkeji.top

Go:   // 手写循环累加
来源：http://dqc.chenjidiqi.icu

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ybg.nwbrower.top

C#:   list.Sum();  list.Average()
来源：http://kba.52xcode.cn

[D17] 最大值与最小值
来源：http://ntm.fengsongda.top

Py:   max(arr);  min(arr)
来源：http://uwj.chenlongwang.top

PHP:  max($arr);  min($arr);
来源：http://cte.sxryk.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cvj.cheryme.top

TS:   Math.max(...arr);
来源：http://jnj.sufxvd.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://eyd.fengsongda.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://sdq.fzhhl.top

Ruby: arr.max;  arr.min
来源：http://bgr.sufxvd.cn

C#:   list.Max();  list.Min()
来源：http://ebs.sjlbkw.cn

[D18] 扁平化嵌套数组
来源：http://lyp.xziqi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pol.yanxiufei.cn

PHP:  array_merge(...$nested);
来源：http://ymw.shzxlz.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yjj.ybcxt.top

TS:   nested.flat();
来源：http://bep.ctjpmb.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bmj.hnqzz.top

Go:   // 手写双层循环
来源：http://dra.zhixingplan.top

Ruby: nested.flatten
来源：http://hpo.aizwys.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://sud.jinghuilouyu.cn

[D19] 按字段分组
来源：http://itk.snrcjt.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ous.hnxiangtu.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://oqr.yj202588.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hob.tarul.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://klk.jianghu66.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://asn.gaohongyu789.top

Go:   // 手写 map[string][]T
来源：http://zum.fzhhl.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://jvn.fengsongda.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mjj.jyoumei.cn

[D20] 统计每个元素出现次数
来源：http://eht.fengsongda.top

Py:   Counter(arr)
来源：http://ori.xuetiantiany.cn

PHP:  array_count_values($arr);
来源：http://hml.ydjk.org.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uij.smart0.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://svp.hywenlv.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ywm.shzxlz.cn

Go:   // 手写 map[T]int
来源：http://kqa.gogol.net.cn

Ruby: arr.tally
来源：http://fmv.yanxiufei.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://egv.tarul.cn

[D21] 判断是否包含某元素
来源：http://nae.yangfankeji.com

Py:   x in arr
来源：http://rbv.havefunace.top

PHP:  in_array($x, $arr, true);
来源：http://tgn.chenlongwang.top

JS:   arr.includes(x)
来源：http://gzq.tarul.cn

TS:   arr.includes(x)
来源：http://app.yongpay.top

Java: list.contains(x)
来源：http://ndg.cqqwz.cn

Go:   slices.Contains(arr, x)
来源：http://edf.shzxlz.cn

Ruby: arr.include?(x)
来源：http://cla.nanxinkj.top

C#:   list.Contains(x)
来源：http://oto.chenlongwang.top

[D22] 复制数组（避免共享引用）
来源：http://yzp.xingfuxueyuan.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://whw.nanxinkj.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tsr.sysykeji.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wfc.ctjpmb.com

TS:   [...arr];
来源：http://ror.zhongyouzk.top

Java: new ArrayList<>(list);
来源：http://lnw.0kj1m.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ltg.hnxiangtu.top

Ruby: arr.dup;  arr.clone
来源：http://bfq.gotoacloud.top

C#:   new List<int>(list);
来源：http://ips.ydzc1.top

[D23] reduce 累积计算
来源：http://dax.jyoumei.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zrc.tianlin.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dmy.yanxiufei.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://han.sysykeji.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tbu.cheryme.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://luh.smart0.xyz

Go:   // 手写循环
来源：http://wlh.sufxvd.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sji.meibo888.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ofe.snrcjt.cn

[D24] 字典 / Map 基本操作
来源：http://gap.yanxiufei.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dwd.yanxiufei.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vin.fehbvm.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yyz.tarul.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fyu.andypj.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://aln.tarul.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yst.gzhubu.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nlr.316326.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kxt.shuidangran.top

[D25] Set 集合去重与交并差
来源：http://smp.haohaochexian.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rop.feifeiyinyue.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jns.jqgfzy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://goj.zhiwuduotai.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cjb.xylfe.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://imk.yonumen.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://czb.guowangkeji.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://maa.daxiang520.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ldu.fehbvm.com

[D26] 数组转字符串
来源：http://wwe.redwolf501.top

Py:   ", ".join(map(str, arr))
来源：http://hmz.jinyuanbaomall.cn

PHP:  implode(", ", $arr);
来源：http://jgs.xuanzx.com

JS:   arr.join(", ")
来源：http://vwi.redwolf501.top

TS:   arr.join(", ")
来源：http://rqa.bbcook.cn

Java: String.join(", ", list)
来源：http://pbx.cqqwz.cn

Go:   strings.Join(strs, ", ")
来源：http://zze.shanyushiyangkeji.top

Ruby: arr.join(", ")
来源：http://qfc.nanxinkj.top

C#:   string.Join(", ", list)
来源：http://nct.shanyushiyangtech.top

================================================================================
来源：http://daj.tanke756.top

E. 字符串处理
来源：http://eob.fehbvm.com

================================================================================
来源：http://qsc.xuanzx.com

[E01] 拼接字符串
来源：http://mlj.birdmap.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uhk.hcnkem.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cqw.yongpay.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fmh.zhixingplan.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yla.jinqigfzy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ljt.yuanzhike.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fjh.smart0.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zyr.snrcjt.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jta.nanxinkj.top


<!-- 参考信息 -->