代发 wailian999

C#:   块级作用域
来源：http://yuy.birdmap.top

[C11] 模块导入与导出
来源：http://ycx.yfazqb.com

Py:   from module import func
来源：http://dtw.yongpay.top

PHP:  require "file.php";  或 use App\Service;
来源：http://hcm.tianlin.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://bsy.jqgufenzy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xxg.jiagoushi.top

Java: import java.util.List;
来源：http://kdx.jyoumei.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://grw.0kj1m.cn

Ruby: require "json"; require_relative "./util"
来源：http://tff.shzxlz.cn

C#:   using System.Text;
来源：http://uyi.jinyuanbaomall.cn

[C12] 立即执行函数 IIFE
来源：http://oqw.cheryme.top

Py:   (lambda: print("run"))()
来源：http://qgu.xingfuxueyuan.xyz

PHP:  (function () { echo "run"; })();
来源：http://vpl.ctjpmb.com

JS:   (() => { console.log("run"); })();
来源：http://blp.zhoulong.xyz

TS:   (() => { console.log("run"); })();
来源：http://xpg.zhongyouzk.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wwf.shanyushiyangkeji.top

Go:   func() { fmt.Println("run") }()
来源：http://gkr.jlsjyb.cn

Ruby: -> { puts "run" }.call
来源：http://yfh.jqgfzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://gnq.zycfv.cn

[C13] 类型声明 / 类型注解
来源：http://bne.chenzaomai.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hku.uphjek.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tcn.jinqigufen.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bsa.gaohongyu789.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ddm.cqqwz.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ynl.hammf.cn

Go:   func add(a, b int) int
来源：http://vcv.dianchejie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mtg.feifeiyinyue.top

C#:   int Add(int a, int b) => a + b;
来源：http://eqf.yj20258888.top

[C14] 泛型函数
来源：http://dcv.shzxlz.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mfb.ehwqpu.com

PHP:  // 无泛型
来源：http://itd.316326.xyz

JS:   // 无泛型
来源：http://oem.daria6918.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sex.chenzaomai.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://abk.zhongyouzk.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://izc.sweek.top

Ruby: # 无泛型
来源：http://wba.xuetiantiany.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pll.zhaomingkeji.xyz

[C15] 解构 / 展开参数
来源：http://tqe.xuanzx.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bfo.zhoulong.xyz

PHP:  [$a, $b] = $pair;
来源：http://yqd.uphjek.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://edt.sysykeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ezm.yueranfly.top

Java: // 无解构
来源：http://ayg.redwolf501.top

Go:   // 无解构
来源：http://qsk.tanke756.top

Ruby: a, b = pair
来源：http://xtb.xylfe.cn

C#:   var (a, b) = pair;
来源：http://ygk.jinqigfzy.top

[C16] 函数 / 方法重载
来源：http://mde.hnqzz.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://woa.wangshuangyany.cn

PHP:  // 无重载
来源：http://vxr.cucudq.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zok.nwbrower.top

TS:   // 用联合类型或重载签名声明
来源：http://ljq.316326.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://wtr.sweek.top

Go:   // 无重载：用不同函数名
来源：http://shs.fzhhl.top

Ruby: # 无重载：靠动态参数
来源：http://hbd.yj202588.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://rss.ydzc1.top

================================================================================
来源：http://npi.hongshengwenyu.top

D. 数组 / 列表 / 集合
来源：http://jwq.jianghu66.top

================================================================================
来源：http://pao.wangshuangyany.cn

[D01] 创建数组 / 列表
来源：http://wtk.daria6918.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://tfi.cheryme.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nwz.zhiwuduotai.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gjn.sxryk.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wxv.yanxiufei.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jvv.chenlongwang.top

Go:   arr := []int{1, 2, 3}
来源：http://esb.yuanzhike.top

Ruby: arr = [1, 2, 3]
来源：http://ovb.hywenlv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://btm.hywenlv.cn

[D02] 追加元素到末尾
来源：http://zuf.hfpthk.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ste.ehwqpu.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://euk.kuanghao11.cn

JS:   arr.push(4);
来源：http://tyb.ppjwa.cn

TS:   arr.push(4);
来源：http://wnd.9152youxi.cn

Java: list.add(4);
来源：http://pbi.hnxiangtu.top

Go:   arr = append(arr, 4)
来源：http://ful.zycfv.cn

Ruby: arr << 4; arr.push(5)
来源：http://tdu.jinqigufen.top

C#:   list.Add(4);
来源：http://vyl.tian-w.cn

[D03] 在指定位置插入元素
来源：http://jyf.tian-w.cn

Py:   arr.insert(0, 0)
来源：http://xes.zhijiandao.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vhb.cdnleiting.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mqe.birdmap.top

TS:   arr.splice(0, 0, 0);
来源：http://hkd.wangdashe.top

Java: list.add(0, 0);
来源：http://mzx.fktsv.cn

Go:   arr = append([]int{0}, arr...)
来源：http://lgm.yfazqb.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://brt.sjlbkw.cn

C#:   list.Insert(0, 0);
来源：http://mwp.bbcook.cn

[D04] 删除元素
来源：http://rfk.ydjk.org.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://let.ywan-chungtsiang.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ojk.hfpthk.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gaz.sysykeji.top

TS:   arr.splice(0, 1);
来源：http://kvz.bbcook.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fss.epnwcf.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hcq.shanyushiyangtech.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pae.316326.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jbv.ppjwa.cn

[D05] 访问与修改元素
来源：http://exs.fehbvm.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ghi.birdmap.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ksv.ctjpmb.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bpw.ctjpmb.com

TS:   arr[0]; arr.at(-1);
来源：http://amc.sufxvd.cn

Java: list.get(0); list.set(0, 9);
来源：http://ebl.jinyuanbaomall.cn

Go:   arr[0]; arr[0] = 9
来源：http://iip.zhiwuduotai.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lyo.pycfn.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://amz.kuanghao11.cn

[D06] 数组长度
来源：http://dqj.fehbvm.com

Py:   len(arr)
来源：http://bke.ppjwa.cn

PHP:  count($arr);
来源：http://rmx.shanyushiyangtech.top

JS:   arr.length
来源：http://cfd.sxryk.cn

TS:   arr.length
来源：http://loi.fanxiaobao.xyz

Java: list.size();
来源：http://ufn.yj202588.top

Go:   len(arr)
来源：http://bwp.vqdsnc.cn

Ruby: arr.length; arr.size
来源：http://onk.feifeiyinyue.top

C#:   list.Count;
来源：http://hux.fzhhl.top

[D07] 切片 / 取子数组
来源：http://oyl.gaohongyu789.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://onc.bbcook.cn

PHP:  array_slice($arr, 1, 3);
来源：http://aqi.ydzc1.top

JS:   arr.slice(1, 4);
来源：http://zjc.quarkkingdee.top

TS:   arr.slice(1, 4);
来源：http://dud.hammf.cn

Java: list.subList(1, 4);
来源：http://bmo.daria6918.cn

Go:   arr[1:4]
来源：http://gye.xuetiantiany.cn

Ruby: arr[1, 3]
来源：http://eje.wangshuangyany.cn

C#:   list.GetRange(1, 3);
来源：http://vhu.mhx1999.top

[D08] 合并两个数组
来源：http://jcy.fehbvm.com

Py:   a + b;  a.extend(b)
来源：http://awp.yangfankeji.com

PHP:  array_merge($a, $b);
来源：http://wqp.yonumen.top

JS:   [...a, ...b];  a.concat(b);
来源：http://cyz.zhongyouzk.top

TS:   [...a, ...b];
来源：http://igg.0kj1m.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://uys.fengsongda.top

Go:   append(a, b...)
来源：http://oyz.epnwcf.com

Ruby: a + b;  a.concat(b)
来源：http://fvy.c1oappe.top

C#:   a.Concat(b).ToList()
来源：http://cgc.jqgufenzy.top

[D09] 排序（升序）
来源：http://xja.gaohongyu789.top

Py:   sorted(arr);  arr.sort()
来源：http://nme.dashuyun.cn

PHP:  sort($arr);
来源：http://obc.hnqzz.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rhc.jyoumei.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://vgw.zhengqikj.top

Java: Collections.sort(list);  list.sort(null);
来源：http://dfp.zhoulong.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dpf.hcnkem.com

Ruby: arr.sort
来源：http://atj.316326.xyz

C#:   list.Sort();
来源：http://pnn.guowangkeji.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://uig.52xcode.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jph.jlsjyb.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oab.xinyue.icu

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xao.zhengqikj.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wlt.meibo888.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vbu.yfazqb.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sot.birdmap.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qji.52xcode.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pcy.daxiang520.top

[D11] 反转数组
来源：http://brt.feifeiyinyue.top

Py:   arr[::-1];  arr.reverse()
来源：http://xwk.yj20258.top

PHP:  array_reverse($arr);
来源：http://enr.yongpay.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qsz.dianchejie.cn

TS:   [...arr].reverse();
来源：http://grd.dianchejie.cn

Java: Collections.reverse(list);
来源：http://uxa.aibaodan.cn

Go:   slices.Reverse(arr)
来源：http://rox.guannengcc.top

Ruby: arr.reverse
来源：http://fcd.yangfankeji.com

C#:   list.Reverse();
来源：http://bat.vehdjk.com

[D12] 查找元素下标
来源：http://mki.kuanghao11.cn

Py:   arr.index(x);  x in arr
来源：http://onh.fengsongda.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xjl.guowangkeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uhj.zdbjq.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yzu.jqgufenzy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xzg.sufxvd.cn

Go:   slices.Index(arr, x)
来源：http://mwp.gaohongyu789.top

Ruby: arr.index(x)
来源：http://ixz.svipenyu.cn

C#:   list.IndexOf(x);
来源：http://jtr.zhixingplan.top

[D13] 过滤（保留满足条件的）
来源：http://tnl.yj202588.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uvl.ydzc1.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hcw.yonumen.top

JS:   arr.filter(x => x > 3)
来源：http://ayk.hnqzz.top

TS:   arr.filter(x => x > 3)
来源：http://rry.hysaishi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mph.yj20258.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://iea.jianghu66.top

Ruby: arr.select { |x| x > 3 }
来源：http://ssh.quarkkingdee.top

C#:   list.Where(x => x > 3).ToList()
来源：http://lgn.dianchejie.cn

[D14] 映射转换（每个元素变形）
来源：http://uuu.jqgufenzy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kjl.9152youxi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vgb.xuetiantiany.cn

JS:   arr.map(x => x * 2)
来源：http://wmm.yfazqb.com

TS:   arr.map(x => x * 2)
来源：http://skf.tian-w.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://tvc.tian-w.cn

Go:   // 手写循环
来源：http://kcy.ivvv.top

Ruby: arr.map { |x| x * 2 }
来源：http://cne.pycfn.com

C#:   list.Select(x => x * 2).ToList()
来源：http://qwq.yj20258888.top

[D15] 去重
来源：http://vqj.ydjk.org.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qtk.hfpthk.cn

PHP:  array_unique($arr);
来源：http://man.bjfxy.top

JS:   [...new Set(arr)]
来源：http://dyu.zhixingplan.top

TS:   [...new Set(arr)]
来源：http://xty.chenlongwang.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://goe.zhiwuduotai.top

Go:   // 用 map[T]struct{} 手写
来源：http://bgz.0kj1m.cn

Ruby: arr.uniq
来源：http://hyc.fehbvm.com

C#:   list.Distinct().ToList()
来源：http://yiq.jlsjyb.cn

[D16] 求和与平均值
来源：http://wwi.yj20258.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fcd.ydzc1.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hle.ehwqpu.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hcy.zhixingplan.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nqt.zhongyouzk.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://azy.fktsv.cn

Go:   // 手写循环累加
来源：http://xdh.zhiwuduotai.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ulr.52xcode.cn

C#:   list.Sum();  list.Average()
来源：http://jgd.nanxinkj.top

[D17] 最大值与最小值
来源：http://cyo.yongpay.top

Py:   max(arr);  min(arr)
来源：http://znk.fzhhl.top

PHP:  max($arr);  min($arr);
来源：http://gyu.jinghuilouyu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mma.0kj1m.cn

TS:   Math.max(...arr);
来源：http://ljn.dashuyun.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jcg.chenlongwang.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://sye.ydzc1.top

Ruby: arr.max;  arr.min
来源：http://nge.guowangkeji.top

C#:   list.Max();  list.Min()
来源：http://nla.jyoumei.cn

[D18] 扁平化嵌套数组
来源：http://isp.pycfn.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vho.meibo888.top

PHP:  array_merge(...$nested);
来源：http://cyo.zdqjudy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jei.uphjek.com

TS:   nested.flat();
来源：http://wvz.andypj.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ccw.yvedp.cn

Go:   // 手写双层循环
来源：http://erb.svipenyu.cn

Ruby: nested.flatten
来源：http://urk.jiagoushi.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://kmy.pengpengdd.cyou

[D19] 按字段分组
来源：http://upi.haohaochexian.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bfi.hesvh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wyk.uphjek.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kwy.shanyushiyangkeji.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ynp.wangdashe.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nwh.hesvh.cn

Go:   // 手写 map[string][]T
来源：http://onc.ydjk.org.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vei.zhijiandao.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ggx.ybcxt.top

[D20] 统计每个元素出现次数
来源：http://vfu.yanxiufei.cn

Py:   Counter(arr)
来源：http://pvq.zdbjq.cn

PHP:  array_count_values($arr);
来源：http://rps.hnqzz.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ayi.xziqi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nqb.smart0.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hii.hongshengwenyu.top

Go:   // 手写 map[T]int
来源：http://hpy.xylfe.cn

Ruby: arr.tally
来源：http://jru.birdmap.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yfr.ctjpmb.com

[D21] 判断是否包含某元素
来源：http://gwk.fktsv.cn

Py:   x in arr
来源：http://jlz.gotoacloud.top

PHP:  in_array($x, $arr, true);
来源：http://bpq.feifeiyinyue.top

JS:   arr.includes(x)
来源：http://wwa.tarul.cn

TS:   arr.includes(x)
来源：http://jhu.gaohongyu789.top

Java: list.contains(x)
来源：http://rcy.hywenlv.cn

Go:   slices.Contains(arr, x)
来源：http://izd.andypj.xyz

Ruby: arr.include?(x)
来源：http://qla.jlsjyb.cn

C#:   list.Contains(x)
来源：http://ymr.svipenyu.cn

[D22] 复制数组（避免共享引用）
来源：http://vnt.52xcode.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fbl.tanke756.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xxb.shangyingyoupin.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ceh.ppjwa.cn

TS:   [...arr];
来源：http://rpk.bjfxy.top

Java: new ArrayList<>(list);
来源：http://ich.yj20258.top

Go:   copied := append([]int(nil), arr...)
来源：http://vea.quarkkingdee.top

Ruby: arr.dup;  arr.clone
来源：http://anq.gaohongyu789.top

C#:   new List<int>(list);
来源：http://xwg.bbcook.cn

[D23] reduce 累积计算
来源：http://mia.ydjk.org.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wvv.svipenyu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pjf.0kj1m.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rar.tian-w.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://asl.wangdashe.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ewu.hnxiangtu.top

Go:   // 手写循环
来源：http://mjc.tanke756.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://aac.316326.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fsp.cdnleiting.top

[D24] 字典 / Map 基本操作
来源：http://ijs.gogol.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bie.bjfxy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gqp.gaohongyu789.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tdf.sweek.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sgb.yuxming.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gyn.tarul.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://oxv.snrcjt.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ccc.vqdsnc.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jsk.c1oappe.top

[D25] Set 集合去重与交并差
来源：http://fyz.zhijiandao.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wav.guowangkeji.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bfp.fktsv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lay.hnqzz.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jwk.cheryme.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xfl.dianchejie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jit.chenjidiqi.icu

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ibo.xinyue.icu

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kxn.snrcjt.cn

[D26] 数组转字符串
来源：http://qbi.guowangkeji.top

Py:   ", ".join(map(str, arr))
来源：http://ybj.gogol.net.cn

PHP:  implode(", ", $arr);
来源：http://gyd.snrcjt.cn

JS:   arr.join(", ")
来源：http://oas.9152youxi.cn

TS:   arr.join(", ")
来源：http://jhs.xuanzx.com

Java: String.join(", ", list)
来源：http://aij.redwolf501.top

Go:   strings.Join(strs, ", ")
来源：http://jtj.havefunace.top

Ruby: arr.join(", ")
来源：http://pti.yvedp.cn

C#:   string.Join(", ", list)
来源：http://tzm.cheryme.top

================================================================================
来源：http://foz.pengpengdd.cyou

E. 字符串处理
来源：http://zns.tian-w.cn

================================================================================
来源：http://ktz.wangshuangyany.cn

[E01] 拼接字符串
来源：http://rah.jianghu66.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qgf.yuanzhike.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vjg.sweek.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://urg.uphjek.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ejw.zhoulong.xyz


<!-- 参考信息 -->