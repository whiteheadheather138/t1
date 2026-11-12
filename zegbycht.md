代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://okr.shzxlz.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ccb.zhaomingkeji.xyz

Java: import java.util.List;
来源：http://egq.mhx1999.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hbj.zhijiandao.cn

Ruby: require "json"; require_relative "./util"
来源：http://mni.zdqjudy.top

C#:   using System.Text;
来源：http://gsr.aizwys.cn

[C12] 立即执行函数 IIFE
来源：http://bot.havefunace.top

Py:   (lambda: print("run"))()
来源：http://dss.vqdsnc.cn

PHP:  (function () { echo "run"; })();
来源：http://tcy.cucudq.cn

JS:   (() => { console.log("run"); })();
来源：http://ecz.tarul.cn

TS:   (() => { console.log("run"); })();
来源：http://bpi.pengpengdd.cyou

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fry.pengpengdd.cyou

Go:   func() { fmt.Println("run") }()
来源：http://acy.hnxiangtu.top

Ruby: -> { puts "run" }.call
来源：http://ejr.yangfankeji.com

C#:   // 无 IIFE：用静态构造函数
来源：http://dpt.jlsjyb.cn

[C13] 类型声明 / 类型注解
来源：http://sch.nwbrower.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sea.daria6918.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gvn.yvedp.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ksh.ivvv.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zkv.zhiwuduotai.top

Java: int add(int a, int b) { return a + b; }
来源：http://nhs.ehwqpu.com

Go:   func add(a, b int) int
来源：http://vhn.ybcxt.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://eyn.mhx1999.top

C#:   int Add(int a, int b) => a + b;
来源：http://qzu.shzxlz.cn

[C14] 泛型函数
来源：http://tud.ppjwa.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gdf.jiagoushi.top

PHP:  // 无泛型
来源：http://hkc.xuanzx.com

JS:   // 无泛型
来源：http://hgd.sxryk.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hnz.pengpengdd.cyou

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://haz.9152youxi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tls.kuanghao11.cn

Ruby: # 无泛型
来源：http://pvf.shzxlz.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xme.chenlongwang.top

[C15] 解构 / 展开参数
来源：http://bbd.xinyue.icu

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://uvc.hywenlv.cn

PHP:  [$a, $b] = $pair;
来源：http://mmb.jlsjyb.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dfy.jiagoushi.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qjy.hongshengwenyu.top

Java: // 无解构
来源：http://vmg.fzhhl.top

Go:   // 无解构
来源：http://ryx.uphjek.com

Ruby: a, b = pair
来源：http://tvx.zhijiandao.cn

C#:   var (a, b) = pair;
来源：http://lmi.0kj1m.cn

[C16] 函数 / 方法重载
来源：http://zjk.jyoumei.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xvm.wangdashe.top

PHP:  // 无重载
来源：http://lgu.jyoumei.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://tcj.ehwqpu.com

TS:   // 用联合类型或重载签名声明
来源：http://hql.wangdashe.top

Java: void f(int a) {}  void f(String a) {}
来源：http://etc.yueranfly.top

Go:   // 无重载：用不同函数名
来源：http://hti.xinyue.icu

Ruby: # 无重载：靠动态参数
来源：http://kbi.jianghu66.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://laj.chenzaomai.com

================================================================================
来源：http://iyo.sjlbkw.cn

D. 数组 / 列表 / 集合
来源：http://qph.tanke756.top

================================================================================
来源：http://iph.zycfv.cn

[D01] 创建数组 / 列表
来源：http://keg.hesvh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://vih.yonumen.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kwu.jyoumei.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://buc.jinqigfzy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://dly.nanxinkj.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jer.hcnkem.com

Go:   arr := []int{1, 2, 3}
来源：http://thc.fzhhl.top

Ruby: arr = [1, 2, 3]
来源：http://hsn.hesvh.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cax.zhixingplan.top

[D02] 追加元素到末尾
来源：http://bzl.zhiwuduotai.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lzr.ydjk.org.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wsl.haohaochexian.top

JS:   arr.push(4);
来源：http://lhi.52xcode.cn

TS:   arr.push(4);
来源：http://cnf.wangshuangyany.cn

Java: list.add(4);
来源：http://aad.hfpthk.cn

Go:   arr = append(arr, 4)
来源：http://wqr.zhaomingkeji.xyz

Ruby: arr << 4; arr.push(5)
来源：http://tre.fktsv.cn

C#:   list.Add(4);
来源：http://ntn.bbcook.cn

[D03] 在指定位置插入元素
来源：http://xmw.hcnkem.com

Py:   arr.insert(0, 0)
来源：http://bjz.haohaochexian.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://odt.zhengqikj.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vxe.ydzc1.top

TS:   arr.splice(0, 0, 0);
来源：http://xat.daria6918.cn

Java: list.add(0, 0);
来源：http://pzf.hywenlv.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mvi.chenzaomai.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lqf.pengpengdd.cyou

C#:   list.Insert(0, 0);
来源：http://mpe.shzxlz.cn

[D04] 删除元素
来源：http://aea.yongpay.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pai.c1oappe.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fgt.yj20258888.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kim.zhixingplan.top

TS:   arr.splice(0, 1);
来源：http://ivm.ydzc1.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ksa.shanyushiyangkeji.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tbq.dashuyun.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://agk.0kj1m.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ycp.smart0.xyz

[D05] 访问与修改元素
来源：http://dlf.vehdjk.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://isn.fengsongda.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://aee.chenlongwang.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fqs.sweek.top

TS:   arr[0]; arr.at(-1);
来源：http://lps.9152youxi.cn

Java: list.get(0); list.set(0, 9);
来源：http://yzg.fzhhl.top

Go:   arr[0]; arr[0] = 9
来源：http://hcd.ybcxt.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zcz.vqdsnc.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kou.fehbvm.com

[D06] 数组长度
来源：http://qhp.jinghuilouyu.cn

Py:   len(arr)
来源：http://wnf.meibo888.top

PHP:  count($arr);
来源：http://wsq.bbcook.cn

JS:   arr.length
来源：http://kxb.daxiang520.top

TS:   arr.length
来源：http://rrq.9152youxi.cn

Java: list.size();
来源：http://bif.tarul.cn

Go:   len(arr)
来源：http://lvr.dianchejie.cn

Ruby: arr.length; arr.size
来源：http://rkv.yueranfly.top

C#:   list.Count;
来源：http://jln.shanyushiyangkeji.top

[D07] 切片 / 取子数组
来源：http://rnb.xuetiantiany.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yjf.jinqigfzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://ebr.kuanghao11.cn

JS:   arr.slice(1, 4);
来源：http://llc.yanxiufei.cn

TS:   arr.slice(1, 4);
来源：http://vpu.sweek.top

Java: list.subList(1, 4);
来源：http://dmh.yj20258.top

Go:   arr[1:4]
来源：http://ejq.xylfe.cn

Ruby: arr[1, 3]
来源：http://syr.zhoulong.xyz

C#:   list.GetRange(1, 3);
来源：http://ihd.hfpthk.cn

[D08] 合并两个数组
来源：http://omd.chenlongwang.top

Py:   a + b;  a.extend(b)
来源：http://yfs.zdbjq.cn

PHP:  array_merge($a, $b);
来源：http://ake.gaohongyu789.top

JS:   [...a, ...b];  a.concat(b);
来源：http://cfj.fzhhl.top

TS:   [...a, ...b];
来源：http://qky.meibo888.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tjw.gotoacloud.top

Go:   append(a, b...)
来源：http://msm.shuidangran.top

Ruby: a + b;  a.concat(b)
来源：http://qpf.birdmap.top

C#:   a.Concat(b).ToList()
来源：http://ivi.ctjpmb.com

[D09] 排序（升序）
来源：http://ogz.52xcode.cn

Py:   sorted(arr);  arr.sort()
来源：http://xgi.pycfn.com

PHP:  sort($arr);
来源：http://tfu.zycfv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://iia.feifeiyinyue.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://muo.daxiang520.top

Java: Collections.sort(list);  list.sort(null);
来源：http://pbj.shanyushiyangkeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xvg.jqgufenzy.top

Ruby: arr.sort
来源：http://fpm.shuidangran.top

C#:   list.Sort();
来源：http://iat.xuetiantiany.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://biv.yuanzhike.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://olv.shanyushiyangtech.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dzh.chenlongwang.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://job.mhx1999.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fdl.sxryk.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wkr.sysykeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wks.chenlongwang.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ine.zhoulong.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sdc.316326.xyz

[D11] 反转数组
来源：http://gej.tanke756.top

Py:   arr[::-1];  arr.reverse()
来源：http://rul.jinghuilouyu.cn

PHP:  array_reverse($arr);
来源：http://lxn.havefunace.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cbu.fengsongda.top

TS:   [...arr].reverse();
来源：http://ois.xingfuxueyuan.xyz

Java: Collections.reverse(list);
来源：http://btg.tanke756.top

Go:   slices.Reverse(arr)
来源：http://nqa.nanxinkj.top

Ruby: arr.reverse
来源：http://eiv.zdqjudy.top

C#:   list.Reverse();
来源：http://xkc.zhongyouzk.top

[D12] 查找元素下标
来源：http://vfo.zhixingplan.top

Py:   arr.index(x);  x in arr
来源：http://isg.yangfankeji.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ymn.zhengqikj.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tje.meibo888.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uko.bbcook.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dgh.hnxiangtu.top

Go:   slices.Index(arr, x)
来源：http://uya.quarkkingdee.top

Ruby: arr.index(x)
来源：http://lpb.yj20258888.top

C#:   list.IndexOf(x);
来源：http://uxk.xuanzx.com

[D13] 过滤（保留满足条件的）
来源：http://cud.sweek.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://scb.gogol.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bmj.meibo888.top

JS:   arr.filter(x => x > 3)
来源：http://odd.yonumen.top

TS:   arr.filter(x => x > 3)
来源：http://jbk.zhengqikj.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cdx.havefunace.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://clv.yanxiufei.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xqw.ydzc1.top

C#:   list.Where(x => x > 3).ToList()
来源：http://zuu.gzhubu.top

[D14] 映射转换（每个元素变形）
来源：http://wfb.nwbrower.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gmh.hfpthk.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qxj.yangfankeji.com

JS:   arr.map(x => x * 2)
来源：http://qxh.haohaochexian.top

TS:   arr.map(x => x * 2)
来源：http://kvo.mhx1999.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://eiu.9152youxi.cn

Go:   // 手写循环
来源：http://shh.uphjek.com

Ruby: arr.map { |x| x * 2 }
来源：http://nab.hammf.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jar.birdmap.top

[D15] 去重
来源：http://uok.yvedp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jox.uphjek.com

PHP:  array_unique($arr);
来源：http://rcp.wangshuangyany.cn

JS:   [...new Set(arr)]
来源：http://cqm.feifeiyinyue.top

TS:   [...new Set(arr)]
来源：http://obj.jianghu66.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xmq.ctjpmb.com

Go:   // 用 map[T]struct{} 手写
来源：http://hcu.hnqzz.top

Ruby: arr.uniq
来源：http://yzp.ydzc1.top

C#:   list.Distinct().ToList()
来源：http://iee.jinqigfzy.top

[D16] 求和与平均值
来源：http://zhh.hnqzz.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://eax.pycfn.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://niu.smart0.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zad.shzxlz.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hxm.haohaochexian.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ybr.ppjwa.cn

Go:   // 手写循环累加
来源：http://kkq.guannengcc.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://umj.fanxiaobao.xyz

C#:   list.Sum();  list.Average()
来源：http://ncu.guannengcc.top

[D17] 最大值与最小值
来源：http://dod.guowangkeji.top

Py:   max(arr);  min(arr)
来源：http://aya.xuetiantiany.cn

PHP:  max($arr);  min($arr);
来源：http://rve.yuanzhike.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://epp.cqqwz.cn

TS:   Math.max(...arr);
来源：http://fgt.fzhhl.top

Java: Collections.max(list);  Collections.min(list);
来源：http://kea.snrcjt.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cpm.haohaochexian.top

Ruby: arr.max;  arr.min
来源：http://kml.fanxiaobao.xyz

C#:   list.Max();  list.Min()
来源：http://lpu.nanxinkj.top

[D18] 扁平化嵌套数组
来源：http://xqr.sufxvd.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tqg.jinghuilouyu.cn

PHP:  array_merge(...$nested);
来源：http://sgo.jyoumei.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ass.tarul.cn

TS:   nested.flat();
来源：http://lam.dianchejie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hcz.zhaomingkeji.xyz

Go:   // 手写双层循环
来源：http://bxc.zhaomingkeji.xyz

Ruby: nested.flatten
来源：http://yps.quarkkingdee.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://iju.ydjk.org.cn

[D19] 按字段分组
来源：http://kzb.zhoulong.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jra.cdnleiting.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yhq.jiagoushi.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rti.meibo888.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://esa.snrcjt.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zit.hnxiangtu.top

Go:   // 手写 map[string][]T
来源：http://jph.hongshengwenyu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://kii.zycfv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qzc.quarkkingdee.top

[D20] 统计每个元素出现次数
来源：http://ecf.cucudq.cn

Py:   Counter(arr)
来源：http://cuj.ehwqpu.com

PHP:  array_count_values($arr);
来源：http://znv.sufxvd.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ecg.mhx1999.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hav.hcnkem.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bqb.xuanzx.com

Go:   // 手写 map[T]int
来源：http://wqq.yfazqb.com

Ruby: arr.tally
来源：http://tyn.zhixingplan.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://twd.jinqigufen.top

[D21] 判断是否包含某元素
来源：http://ixo.daria6918.cn

Py:   x in arr
来源：http://rdw.gaohongyu789.top

PHP:  in_array($x, $arr, true);
来源：http://twy.birdmap.top

JS:   arr.includes(x)
来源：http://zgt.shzxlz.cn

TS:   arr.includes(x)
来源：http://eag.zhengqikj.top

Java: list.contains(x)
来源：http://wez.zhiwuduotai.top

Go:   slices.Contains(arr, x)
来源：http://ylg.havefunace.top

Ruby: arr.include?(x)
来源：http://ccj.yueranfly.top

C#:   list.Contains(x)
来源：http://jdp.sjlbkw.cn

[D22] 复制数组（避免共享引用）
来源：http://jxw.zycfv.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kbg.tarul.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fbj.guannengcc.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gma.ctjpmb.com

TS:   [...arr];
来源：http://tbu.smart0.xyz

Java: new ArrayList<>(list);
来源：http://hfz.hesvh.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ehc.zhoulong.xyz

Ruby: arr.dup;  arr.clone
来源：http://jmg.yj20258.top

C#:   new List<int>(list);
来源：http://ygp.bbcook.cn

[D23] reduce 累积计算
来源：http://uoy.ehwqpu.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wsp.gotoacloud.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pvd.epnwcf.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mvs.pengpengdd.cyou

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ijb.yueranfly.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://gys.daria6918.cn

Go:   // 手写循环
来源：http://hoy.iojbl.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://emx.fzhhl.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jrk.jinghuilouyu.cn

[D24] 字典 / Map 基本操作
来源：http://jzw.hongshengwenyu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kbe.yongpay.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fua.svipenyu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://upc.zdqjudy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ynj.ehwqpu.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rtn.dashuyun.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tkg.bjfxy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ovh.hammf.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vgl.zhijiandao.cn

[D25] Set 集合去重与交并差
来源：http://sav.daxiang520.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bds.smart0.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hsu.daria6918.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wpv.fanxiaobao.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cxi.tianlin.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://prm.shuidangran.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://why.cashguo.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gte.ybcxt.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://etz.cqqwz.cn

[D26] 数组转字符串
来源：http://acz.yuanzhike.top

Py:   ", ".join(map(str, arr))
来源：http://war.tian-w.cn

PHP:  implode(", ", $arr);
来源：http://oho.sxryk.cn

JS:   arr.join(", ")
来源：http://ury.zhaomingkeji.xyz

TS:   arr.join(", ")
来源：http://dgq.0kj1m.cn

Java: String.join(", ", list)
来源：http://ctj.birdmap.top

Go:   strings.Join(strs, ", ")
来源：http://cng.hnxiangtu.top

Ruby: arr.join(", ")
来源：http://rxp.hammf.cn

C#:   string.Join(", ", list)
来源：http://vwc.hnqzz.top

================================================================================
来源：http://fbd.sufxvd.cn

E. 字符串处理
来源：http://fcp.yanxiufei.cn

================================================================================
来源：http://eej.yuxming.cn

[E01] 拼接字符串
来源：http://rnb.xziqi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gvg.9152youxi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uqn.redwolf501.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ffi.zhixingplan.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://noi.vehdjk.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://urk.quarkkingdee.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ypp.xuetiantiany.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mce.zhaomingkeji.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gzg.wangshuangyany.cn


<!-- 参考信息 -->