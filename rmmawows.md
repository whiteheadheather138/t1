代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://fxi.uphjek.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dpf.wangshuangyany.cn

Java: import java.util.List;
来源：http://sdp.guannengcc.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://foy.pycfn.com

Ruby: require "json"; require_relative "./util"
来源：http://lkn.vehdjk.com

C#:   using System.Text;
来源：http://asw.zhoulong.xyz

[C12] 立即执行函数 IIFE
来源：http://bbs.xuetiantiany.cn

Py:   (lambda: print("run"))()
来源：http://bac.chenlongwang.top

PHP:  (function () { echo "run"; })();
来源：http://ein.jinqigufen.top

JS:   (() => { console.log("run"); })();
来源：http://vtg.cdnleiting.top

TS:   (() => { console.log("run"); })();
来源：http://qrc.fehbvm.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wpt.dashuyun.cn

Go:   func() { fmt.Println("run") }()
来源：http://fwb.yonumen.top

Ruby: -> { puts "run" }.call
来源：http://ymm.chenlongwang.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ezq.hcnkem.com

[C13] 类型声明 / 类型注解
来源：http://ngs.fzhhl.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mxf.jyoumei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://brp.shanyushiyangkeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://omg.smart0.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://znx.zhaomingkeji.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://xbs.zhaomingkeji.xyz

Go:   func add(a, b int) int
来源：http://kda.xylfe.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pff.ehwqpu.com

C#:   int Add(int a, int b) => a + b;
来源：http://kre.ppjwa.cn

[C14] 泛型函数
来源：http://duh.jlsjyb.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pla.cqqwz.cn

PHP:  // 无泛型
来源：http://mem.shanyushiyangkeji.top

JS:   // 无泛型
来源：http://qzi.xuanzx.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nlu.bjfxy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wji.yuanzhike.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mvp.zhoulong.xyz

Ruby: # 无泛型
来源：http://jju.cashguo.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sen.fengsongda.top

[C15] 解构 / 展开参数
来源：http://lfm.pycfn.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gcx.cheryme.top

PHP:  [$a, $b] = $pair;
来源：http://qjz.ywan-chungtsiang.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://iqt.sxryk.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wfc.sysykeji.top

Java: // 无解构
来源：http://ejq.wangdashe.top

Go:   // 无解构
来源：http://pgw.bbcook.cn

Ruby: a, b = pair
来源：http://czl.cucudq.cn

C#:   var (a, b) = pair;
来源：http://wqh.svipenyu.cn

[C16] 函数 / 方法重载
来源：http://qsn.shanyushiyangkeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rov.jinqigufen.top

PHP:  // 无重载
来源：http://owa.hammf.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fkz.fktsv.cn

TS:   // 用联合类型或重载签名声明
来源：http://cnz.hysaishi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://bez.birdmap.top

Go:   // 无重载：用不同函数名
来源：http://bey.yueranfly.top

Ruby: # 无重载：靠动态参数
来源：http://rxs.xinyue.icu

C#:   void F(int a) {}  void F(string a) {}
来源：http://ikc.sweek.top

================================================================================
来源：http://lov.daria6918.cn

D. 数组 / 列表 / 集合
来源：http://doo.xylfe.cn

================================================================================
来源：http://tfo.xuetiantiany.cn

[D01] 创建数组 / 列表
来源：http://lil.xuetiantiany.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://amw.yueranfly.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sbz.haohaochexian.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dei.guowangkeji.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://lrn.hywenlv.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tbd.svipenyu.cn

Go:   arr := []int{1, 2, 3}
来源：http://kid.hfpthk.cn

Ruby: arr = [1, 2, 3]
来源：http://mdj.jlsjyb.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mhh.sufxvd.cn

[D02] 追加元素到末尾
来源：http://cwm.nanxinkj.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://owl.jinyuanbaomall.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rgi.shuidangran.top

JS:   arr.push(4);
来源：http://ioh.ppjwa.cn

TS:   arr.push(4);
来源：http://txf.daria6918.cn

Java: list.add(4);
来源：http://xwk.jyoumei.cn

Go:   arr = append(arr, 4)
来源：http://dnx.vehdjk.com

Ruby: arr << 4; arr.push(5)
来源：http://ruc.pengpengdd.cyou

C#:   list.Add(4);
来源：http://itl.jinghuilouyu.cn

[D03] 在指定位置插入元素
来源：http://bgy.yongpay.top

Py:   arr.insert(0, 0)
来源：http://sms.hywenlv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wib.zhengqikj.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sto.guannengcc.top

TS:   arr.splice(0, 0, 0);
来源：http://hgd.jinqigfzy.top

Java: list.add(0, 0);
来源：http://erj.wangshuangyany.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ucg.jiagoushi.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://loy.xziqi.cn

C#:   list.Insert(0, 0);
来源：http://ntq.cucudq.cn

[D04] 删除元素
来源：http://zcy.kuanghao11.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bhc.tarul.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ejq.ydzc1.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ulh.zycfv.cn

TS:   arr.splice(0, 1);
来源：http://dri.hongshengwenyu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kgi.xinyue.icu

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://anm.hammf.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://htw.yongpay.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uxr.shangyingyoupin.top

[D05] 访问与修改元素
来源：http://pnx.sysykeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nkq.yj20258.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://aud.sufxvd.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xnm.chenlongwang.top

TS:   arr[0]; arr.at(-1);
来源：http://onu.xingfuxueyuan.xyz

Java: list.get(0); list.set(0, 9);
来源：http://ssd.9152youxi.cn

Go:   arr[0]; arr[0] = 9
来源：http://liu.yueranfly.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tbg.bbcook.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zhe.0kj1m.cn

[D06] 数组长度
来源：http://xuh.jiagoushi.top

Py:   len(arr)
来源：http://dxm.xuetiantiany.cn

PHP:  count($arr);
来源：http://ynf.uphjek.com

JS:   arr.length
来源：http://yhq.zhijiandao.cn

TS:   arr.length
来源：http://bzc.shanyushiyangkeji.top

Java: list.size();
来源：http://wen.ivvv.top

Go:   len(arr)
来源：http://anz.smart0.xyz

Ruby: arr.length; arr.size
来源：http://enb.guowangkeji.top

C#:   list.Count;
来源：http://huk.yuxming.cn

[D07] 切片 / 取子数组
来源：http://bsq.shzxlz.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mdv.jinghuilouyu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://otp.wangshuangyany.cn

JS:   arr.slice(1, 4);
来源：http://mty.shzxlz.cn

TS:   arr.slice(1, 4);
来源：http://jrd.zhongyouzk.top

Java: list.subList(1, 4);
来源：http://ytn.cheryme.top

Go:   arr[1:4]
来源：http://dqf.gaohongyu789.top

Ruby: arr[1, 3]
来源：http://cak.zhaomingkeji.xyz

C#:   list.GetRange(1, 3);
来源：http://uvv.yonumen.top

[D08] 合并两个数组
来源：http://peh.zhengqikj.top

Py:   a + b;  a.extend(b)
来源：http://lsu.zhongyouzk.top

PHP:  array_merge($a, $b);
来源：http://qgd.guannengcc.top

JS:   [...a, ...b];  a.concat(b);
来源：http://exn.hywenlv.cn

TS:   [...a, ...b];
来源：http://skd.guannengcc.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rqb.uphjek.com

Go:   append(a, b...)
来源：http://kfb.shuidangran.top

Ruby: a + b;  a.concat(b)
来源：http://hlo.hnxiangtu.top

C#:   a.Concat(b).ToList()
来源：http://woy.316326.xyz

[D09] 排序（升序）
来源：http://yfy.sweek.top

Py:   sorted(arr);  arr.sort()
来源：http://egb.jinghuilouyu.cn

PHP:  sort($arr);
来源：http://ytv.andypj.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nfd.hysaishi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tsx.zhixingplan.top

Java: Collections.sort(list);  list.sort(null);
来源：http://sbf.52xcode.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wvy.birdmap.top

Ruby: arr.sort
来源：http://mmm.yj202588.top

C#:   list.Sort();
来源：http://elp.zdbjq.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rtr.jiagoushi.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sqn.xylfe.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dth.hongshengwenyu.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ewt.jinyuanbaomall.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zyv.fzhhl.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://otx.wangshuangyany.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://aju.nanxuanxn.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hcv.jinqigufen.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yqk.yongpay.top

[D11] 反转数组
来源：http://apy.bbcook.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zom.shuidangran.top

PHP:  array_reverse($arr);
来源：http://cwy.cqqwz.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hmq.ctjpmb.com

TS:   [...arr].reverse();
来源：http://pkh.yj20258888.top

Java: Collections.reverse(list);
来源：http://thq.daxiang520.top

Go:   slices.Reverse(arr)
来源：http://vgs.xingfuxueyuan.xyz

Ruby: arr.reverse
来源：http://rsq.dashuyun.cn

C#:   list.Reverse();
来源：http://kws.52xcode.cn

[D12] 查找元素下标
来源：http://mlv.ydzc1.top

Py:   arr.index(x);  x in arr
来源：http://ygk.zdbjq.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rpv.yj20258.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yuy.cheryme.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yjf.zycfv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://okv.zhongyouzk.top

Go:   slices.Index(arr, x)
来源：http://dcg.guannengcc.top

Ruby: arr.index(x)
来源：http://xsb.fktsv.cn

C#:   list.IndexOf(x);
来源：http://wfv.c1oappe.top

[D13] 过滤（保留满足条件的）
来源：http://vfm.sjlbkw.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nbo.zycfv.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fvx.fzhhl.top

JS:   arr.filter(x => x > 3)
来源：http://pzc.yonumen.top

TS:   arr.filter(x => x > 3)
来源：http://vdv.quarkkingdee.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zwb.sxryk.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kbc.zhoulong.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://tms.fzhhl.top

C#:   list.Where(x => x > 3).ToList()
来源：http://meo.sufxvd.cn

[D14] 映射转换（每个元素变形）
来源：http://mih.xinyue.icu

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qgx.ctjpmb.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://aou.tianlin.xyz

JS:   arr.map(x => x * 2)
来源：http://bhv.cucudq.cn

TS:   arr.map(x => x * 2)
来源：http://qif.uphjek.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://hlw.jianghu66.top

Go:   // 手写循环
来源：http://ytz.xuanzx.com

Ruby: arr.map { |x| x * 2 }
来源：http://lhi.bbcook.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ykx.sxryk.cn

[D15] 去重
来源：http://tla.uphjek.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sjk.dianchejie.cn

PHP:  array_unique($arr);
来源：http://gwk.jinqigufen.top

JS:   [...new Set(arr)]
来源：http://eyb.dianchejie.cn

TS:   [...new Set(arr)]
来源：http://ehu.hesvh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ixr.jinghuilouyu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ryd.jyoumei.cn

Ruby: arr.uniq
来源：http://dhf.quarkkingdee.top

C#:   list.Distinct().ToList()
来源：http://vfy.yvedp.cn

[D16] 求和与平均值
来源：http://qnc.bjfxy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zof.yfazqb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qet.zhijiandao.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rmp.ydjk.org.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cbx.aibaodan.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uxp.zdqjudy.top

Go:   // 手写循环累加
来源：http://tco.pengpengdd.cyou

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mcg.shzxlz.cn

C#:   list.Sum();  list.Average()
来源：http://wpq.shzxlz.cn

[D17] 最大值与最小值
来源：http://auq.dashuyun.cn

Py:   max(arr);  min(arr)
来源：http://qqi.meibo888.top

PHP:  max($arr);  min($arr);
来源：http://ogm.sjlbkw.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://otn.hnqzz.top

TS:   Math.max(...arr);
来源：http://snt.9152youxi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://cpy.vqdsnc.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://igh.hongshengwenyu.top

Ruby: arr.max;  arr.min
来源：http://kea.fanxiaobao.xyz

C#:   list.Max();  list.Min()
来源：http://kkb.ybcxt.top

[D18] 扁平化嵌套数组
来源：http://asm.tarul.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wrv.52xcode.cn

PHP:  array_merge(...$nested);
来源：http://bmh.hfpthk.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://flx.fktsv.cn

TS:   nested.flat();
来源：http://gfj.xuanzx.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ged.xziqi.cn

Go:   // 手写双层循环
来源：http://owh.wangshuangyany.cn

Ruby: nested.flatten
来源：http://tds.fanxiaobao.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://zbp.zhijiandao.cn

[D19] 按字段分组
来源：http://gew.havefunace.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://oye.ivvv.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lfq.meibo888.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lgm.ywan-chungtsiang.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://kph.yonumen.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wtn.gzhubu.top

Go:   // 手写 map[string][]T
来源：http://uhg.hongshengwenyu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://lfb.xylfe.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cbv.uphjek.com

[D20] 统计每个元素出现次数
来源：http://xmx.nwbrower.top

Py:   Counter(arr)
来源：http://wau.meibo888.top

PHP:  array_count_values($arr);
来源：http://gtv.sxryk.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hdh.tian-w.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kds.gaohongyu789.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jyb.hesvh.cn

Go:   // 手写 map[T]int
来源：http://ttn.yj20258888.top

Ruby: arr.tally
来源：http://kao.svipenyu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xdg.nwbrower.top

[D21] 判断是否包含某元素
来源：http://cbo.xuetiantiany.cn

Py:   x in arr
来源：http://edf.zhoulong.xyz

PHP:  in_array($x, $arr, true);
来源：http://slb.hnxiangtu.top

JS:   arr.includes(x)
来源：http://vtl.sufxvd.cn

TS:   arr.includes(x)
来源：http://lly.xingfuxueyuan.xyz

Java: list.contains(x)
来源：http://cgt.xylfe.cn

Go:   slices.Contains(arr, x)
来源：http://uwv.jinqigfzy.top

Ruby: arr.include?(x)
来源：http://eqv.gaohongyu789.top

C#:   list.Contains(x)
来源：http://pkf.jinqigfzy.top

[D22] 复制数组（避免共享引用）
来源：http://ihm.zhiwuduotai.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xse.mhx1999.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zwq.haohaochexian.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dev.andypj.xyz

TS:   [...arr];
来源：http://egw.hammf.cn

Java: new ArrayList<>(list);
来源：http://sbb.nwbrower.top

Go:   copied := append([]int(nil), arr...)
来源：http://ddm.hnqzz.top

Ruby: arr.dup;  arr.clone
来源：http://chh.shanyushiyangtech.top

C#:   new List<int>(list);
来源：http://qky.cashguo.top

[D23] reduce 累积计算
来源：http://lrt.zycfv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mqi.hnxiangtu.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://klj.zhaomingkeji.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sdl.pengpengdd.cyou

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jmw.yueranfly.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://fiq.snrcjt.cn

Go:   // 手写循环
来源：http://gil.zdbjq.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hhs.hfpthk.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rru.cheryme.top

[D24] 字典 / Map 基本操作
来源：http://xwu.guannengcc.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://slq.fzhhl.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tnd.nwbrower.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ozw.hcnkem.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xjo.svipenyu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vpr.sjlbkw.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ayh.shzxlz.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fzi.ydzc1.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rnv.ivvv.top

[D25] Set 集合去重与交并差
来源：http://txk.fzhhl.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pwk.zycfv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bdg.bbcook.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://unj.52xcode.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fcm.yj20258888.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gaf.jiagoushi.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nmi.xuetiantiany.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ydv.shangyingyoupin.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dii.zdbjq.cn

[D26] 数组转字符串
来源：http://cor.quarkkingdee.top

Py:   ", ".join(map(str, arr))
来源：http://oon.c1oappe.top

PHP:  implode(", ", $arr);
来源：http://ajf.yongpay.top

JS:   arr.join(", ")
来源：http://nhn.hywenlv.cn

TS:   arr.join(", ")
来源：http://ixp.nanxuanxn.top

Java: String.join(", ", list)
来源：http://ral.yangfankeji.com

Go:   strings.Join(strs, ", ")
来源：http://rrn.yangfankeji.com

Ruby: arr.join(", ")
来源：http://gol.yj20258.top

C#:   string.Join(", ", list)
来源：http://peb.redwolf501.top

================================================================================
来源：http://hlp.sjlbkw.cn

E. 字符串处理
来源：http://ybl.tianlin.xyz

================================================================================
来源：http://wdt.yueranfly.top

[E01] 拼接字符串
来源：http://xsw.fehbvm.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vug.9152youxi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://spi.yuxming.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nov.yanxiufei.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gry.feifeiyinyue.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uoj.fktsv.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lvu.wangdashe.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://soy.hnxiangtu.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ztv.xuanzx.com


<!-- 参考信息 -->