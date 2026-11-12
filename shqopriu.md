代发 wailian999

C#:   块级作用域
来源：http://bux.52xcode.cn

[C11] 模块导入与导出
来源：http://vbd.gaohongyu789.top

Py:   from module import func
来源：http://gat.cheryme.top

PHP:  require "file.php";  或 use App\Service;
来源：http://rqb.jqgfzy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://kxi.fktsv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://div.yuxming.cn

Java: import java.util.List;
来源：http://yhc.hywenlv.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://men.jyoumei.cn

Ruby: require "json"; require_relative "./util"
来源：http://joj.hysaishi.cn

C#:   using System.Text;
来源：http://ler.tanke756.top

[C12] 立即执行函数 IIFE
来源：http://zfx.mhx1999.top

Py:   (lambda: print("run"))()
来源：http://fmw.ppjwa.cn

PHP:  (function () { echo "run"; })();
来源：http://yby.zhaomingkeji.xyz

JS:   (() => { console.log("run"); })();
来源：http://hbh.ehwqpu.com

TS:   (() => { console.log("run"); })();
来源：http://diy.zhixingplan.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bsv.aizwys.cn

Go:   func() { fmt.Println("run") }()
来源：http://vbu.0kj1m.cn

Ruby: -> { puts "run" }.call
来源：http://jao.jqgufenzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://qyk.bjfxy.top

[C13] 类型声明 / 类型注解
来源：http://noi.shuidangran.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://spe.daxiang520.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zui.redwolf501.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sie.cheryme.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tiy.hnxiangtu.top

Java: int add(int a, int b) { return a + b; }
来源：http://xxq.hfpthk.cn

Go:   func add(a, b int) int
来源：http://uvy.yuxming.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bge.sxryk.cn

C#:   int Add(int a, int b) => a + b;
来源：http://hwm.jqgfzy.top

[C14] 泛型函数
来源：http://gmn.guannengcc.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yfs.shanyushiyangtech.top

PHP:  // 无泛型
来源：http://rzi.havefunace.top

JS:   // 无泛型
来源：http://wdr.kuanghao11.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zbv.gotoacloud.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pua.ehwqpu.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lco.fehbvm.com

Ruby: # 无泛型
来源：http://rio.cqqwz.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fad.52xcode.cn

[C15] 解构 / 展开参数
来源：http://svm.xuetiantiany.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ksw.pengpengdd.cyou

PHP:  [$a, $b] = $pair;
来源：http://qwk.quarkkingdee.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mhs.hammf.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sok.zhijiandao.cn

Java: // 无解构
来源：http://wer.cashguo.top

Go:   // 无解构
来源：http://kng.shuidangran.top

Ruby: a, b = pair
来源：http://lmc.xuanzx.com

C#:   var (a, b) = pair;
来源：http://mgb.hnxiangtu.top

[C16] 函数 / 方法重载
来源：http://bwa.guowangkeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rwi.zhixingplan.top

PHP:  // 无重载
来源：http://phs.kuanghao11.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://dap.gogol.net.cn

TS:   // 用联合类型或重载签名声明
来源：http://bjk.guannengcc.top

Java: void f(int a) {}  void f(String a) {}
来源：http://cyg.jiagoushi.top

Go:   // 无重载：用不同函数名
来源：http://qxd.zhongyouzk.top

Ruby: # 无重载：靠动态参数
来源：http://waj.guowangkeji.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://rwx.zycfv.cn

================================================================================
来源：http://vxb.pengpengdd.cyou

D. 数组 / 列表 / 集合
来源：http://bcp.svipenyu.cn

================================================================================
来源：http://gno.ppjwa.cn

[D01] 创建数组 / 列表
来源：http://hsl.gogol.net.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wcy.gogol.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://biv.nanxinkj.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rpe.yueranfly.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://yjb.jyoumei.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uaf.jyoumei.cn

Go:   arr := []int{1, 2, 3}
来源：http://kwg.wangdashe.top

Ruby: arr = [1, 2, 3]
来源：http://mva.ivvv.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gpw.shanyushiyangkeji.top

[D02] 追加元素到末尾
来源：http://tpw.wangdashe.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mbw.yanxiufei.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://flm.iojbl.cn

JS:   arr.push(4);
来源：http://uwh.iojbl.cn

TS:   arr.push(4);
来源：http://ckz.cqqwz.cn

Java: list.add(4);
来源：http://azp.smart0.xyz

Go:   arr = append(arr, 4)
来源：http://xza.shuidangran.top

Ruby: arr << 4; arr.push(5)
来源：http://kfp.svipenyu.cn

C#:   list.Add(4);
来源：http://snd.tian-w.cn

[D03] 在指定位置插入元素
来源：http://cmz.jinqigfzy.top

Py:   arr.insert(0, 0)
来源：http://pbb.zdbjq.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vge.zhoulong.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lor.sysykeji.top

TS:   arr.splice(0, 0, 0);
来源：http://kvt.jiagoushi.top

Java: list.add(0, 0);
来源：http://ajs.shanyushiyangkeji.top

Go:   arr = append([]int{0}, arr...)
来源：http://fda.316326.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yid.xziqi.cn

C#:   list.Insert(0, 0);
来源：http://oja.9152youxi.cn

[D04] 删除元素
来源：http://ryx.hysaishi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wgu.vehdjk.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gik.hfpthk.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ket.cdnleiting.top

TS:   arr.splice(0, 1);
来源：http://qkz.sxryk.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gim.yvedp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vfi.pengpengdd.cyou

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://sdt.fehbvm.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ylm.yueranfly.top

[D05] 访问与修改元素
来源：http://yvq.zdbjq.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tqx.yj202588.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rxj.ydjk.org.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rwa.yj202588.top

TS:   arr[0]; arr.at(-1);
来源：http://uhs.yuanzhike.top

Java: list.get(0); list.set(0, 9);
来源：http://vyp.dashuyun.cn

Go:   arr[0]; arr[0] = 9
来源：http://icw.ydzc1.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tuv.tian-w.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gex.fehbvm.com

[D06] 数组长度
来源：http://ivh.aizwys.cn

Py:   len(arr)
来源：http://fiw.yuxming.cn

PHP:  count($arr);
来源：http://rmx.ivvv.top

JS:   arr.length
来源：http://gbz.zhaomingkeji.xyz

TS:   arr.length
来源：http://fmr.quarkkingdee.top

Java: list.size();
来源：http://row.jinqigfzy.top

Go:   len(arr)
来源：http://ykc.ivvv.top

Ruby: arr.length; arr.size
来源：http://jfl.epnwcf.com

C#:   list.Count;
来源：http://eqc.yj20258888.top

[D07] 切片 / 取子数组
来源：http://kxj.cashguo.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bws.jyoumei.cn

PHP:  array_slice($arr, 1, 3);
来源：http://soq.bbcook.cn

JS:   arr.slice(1, 4);
来源：http://rjs.svipenyu.cn

TS:   arr.slice(1, 4);
来源：http://kxb.hammf.cn

Java: list.subList(1, 4);
来源：http://oto.shzxlz.cn

Go:   arr[1:4]
来源：http://tqa.aibaodan.cn

Ruby: arr[1, 3]
来源：http://fys.bjfxy.top

C#:   list.GetRange(1, 3);
来源：http://gbo.cheryme.top

[D08] 合并两个数组
来源：http://ojx.yfazqb.com

Py:   a + b;  a.extend(b)
来源：http://ncg.xziqi.cn

PHP:  array_merge($a, $b);
来源：http://hyh.nanxinkj.top

JS:   [...a, ...b];  a.concat(b);
来源：http://rkb.zhengqikj.top

TS:   [...a, ...b];
来源：http://ozn.vehdjk.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pcm.cqqwz.cn

Go:   append(a, b...)
来源：http://khi.cucudq.cn

Ruby: a + b;  a.concat(b)
来源：http://xzo.jinqigfzy.top

C#:   a.Concat(b).ToList()
来源：http://yjb.tian-w.cn

[D09] 排序（升序）
来源：http://fbo.haohaochexian.top

Py:   sorted(arr);  arr.sort()
来源：http://oyb.quarkkingdee.top

PHP:  sort($arr);
来源：http://mzu.yj20258.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cmz.zhijiandao.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://pll.cheryme.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ayb.andypj.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xpa.nwbrower.top

Ruby: arr.sort
来源：http://tex.ehwqpu.com

C#:   list.Sort();
来源：http://pki.smart0.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://gkv.zhijiandao.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bwt.shanyushiyangtech.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mvj.ybcxt.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rrz.yanxiufei.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://msu.vqdsnc.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jpw.xingfuxueyuan.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cyx.feifeiyinyue.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://aiu.fktsv.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rsw.guowangkeji.top

[D11] 反转数组
来源：http://kdt.redwolf501.top

Py:   arr[::-1];  arr.reverse()
来源：http://vrh.xingfuxueyuan.xyz

PHP:  array_reverse($arr);
来源：http://fwx.c1oappe.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://soq.cqqwz.cn

TS:   [...arr].reverse();
来源：http://toq.ywan-chungtsiang.top

Java: Collections.reverse(list);
来源：http://sjd.yuxming.cn

Go:   slices.Reverse(arr)
来源：http://sdm.yuanzhike.top

Ruby: arr.reverse
来源：http://vdf.guowangkeji.top

C#:   list.Reverse();
来源：http://knv.cashguo.top

[D12] 查找元素下标
来源：http://use.hysaishi.cn

Py:   arr.index(x);  x in arr
来源：http://tbp.hnqzz.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dqf.bjfxy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hvt.mhx1999.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bmr.zhongyouzk.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vwi.9152youxi.cn

Go:   slices.Index(arr, x)
来源：http://stn.nwbrower.top

Ruby: arr.index(x)
来源：http://nju.shanyushiyangkeji.top

C#:   list.IndexOf(x);
来源：http://ani.hnqzz.top

[D13] 过滤（保留满足条件的）
来源：http://xpi.zhixingplan.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zmr.jinqigufen.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jwb.ybcxt.top

JS:   arr.filter(x => x > 3)
来源：http://vyw.zhengqikj.top

TS:   arr.filter(x => x > 3)
来源：http://wgp.dashuyun.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://asp.zdqjudy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://acg.fengsongda.top

Ruby: arr.select { |x| x > 3 }
来源：http://upi.xylfe.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://eqi.sysykeji.top

[D14] 映射转换（每个元素变形）
来源：http://mpi.xingfuxueyuan.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rmy.dashuyun.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fvj.c1oappe.top

JS:   arr.map(x => x * 2)
来源：http://ggg.xziqi.cn

TS:   arr.map(x => x * 2)
来源：http://kwi.redwolf501.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://cmd.wangshuangyany.cn

Go:   // 手写循环
来源：http://ibj.hesvh.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dok.aibaodan.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://caf.hesvh.cn

[D15] 去重
来源：http://eox.zhengqikj.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://otk.yfazqb.com

PHP:  array_unique($arr);
来源：http://cxi.shzxlz.cn

JS:   [...new Set(arr)]
来源：http://qem.bjfxy.top

TS:   [...new Set(arr)]
来源：http://bzn.316326.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mdz.dianchejie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://osq.daxiang520.top

Ruby: arr.uniq
来源：http://zsa.zdqjudy.top

C#:   list.Distinct().ToList()
来源：http://cxe.jiagoushi.top

[D16] 求和与平均值
来源：http://int.haohaochexian.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kyy.52xcode.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nvi.yj20258888.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rqf.hywenlv.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://peh.hnqzz.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ner.sxryk.cn

Go:   // 手写循环累加
来源：http://tfu.jinqigfzy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vsn.hywenlv.cn

C#:   list.Sum();  list.Average()
来源：http://ptg.hnxiangtu.top

[D17] 最大值与最小值
来源：http://ayx.feifeiyinyue.top

Py:   max(arr);  min(arr)
来源：http://gci.cucudq.cn

PHP:  max($arr);  min($arr);
来源：http://ddq.ydzc1.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sfv.fzhhl.top

TS:   Math.max(...arr);
来源：http://lwl.xingfuxueyuan.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://uuk.tianlin.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fuv.9152youxi.cn

Ruby: arr.max;  arr.min
来源：http://xnm.tanke756.top

C#:   list.Max();  list.Min()
来源：http://qae.kuanghao11.cn

[D18] 扁平化嵌套数组
来源：http://opr.chenlongwang.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dks.bjfxy.top

PHP:  array_merge(...$nested);
来源：http://fzz.shanyushiyangkeji.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cgj.nanxinkj.top

TS:   nested.flat();
来源：http://qfu.zhaomingkeji.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jvi.hongshengwenyu.top

Go:   // 手写双层循环
来源：http://znm.wangdashe.top

Ruby: nested.flatten
来源：http://vcq.xziqi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://jzm.ivvv.top

[D19] 按字段分组
来源：http://osy.birdmap.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qbo.zhoulong.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qqz.iojbl.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://azt.wangdashe.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://csg.jlsjyb.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://arr.ctjpmb.com

Go:   // 手写 map[string][]T
来源：http://myz.ybcxt.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://yhc.ydzc1.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cch.cashguo.top

[D20] 统计每个元素出现次数
来源：http://sod.316326.xyz

Py:   Counter(arr)
来源：http://pks.mhx1999.top

PHP:  array_count_values($arr);
来源：http://hfq.zhengqikj.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hli.jlsjyb.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://btc.fktsv.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dkc.guannengcc.top

Go:   // 手写 map[T]int
来源：http://lav.hnxiangtu.top

Ruby: arr.tally
来源：http://qgz.fengsongda.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vfy.zhengqikj.top

[D21] 判断是否包含某元素
来源：http://ppl.zdbjq.cn

Py:   x in arr
来源：http://atn.yj20258888.top

PHP:  in_array($x, $arr, true);
来源：http://fgq.svipenyu.cn

JS:   arr.includes(x)
来源：http://sno.gaohongyu789.top

TS:   arr.includes(x)
来源：http://gqe.fanxiaobao.xyz

Java: list.contains(x)
来源：http://nyf.epnwcf.com

Go:   slices.Contains(arr, x)
来源：http://xwm.sjlbkw.cn

Ruby: arr.include?(x)
来源：http://xyn.vehdjk.com

C#:   list.Contains(x)
来源：http://rca.zhongyouzk.top

[D22] 复制数组（避免共享引用）
来源：http://vwr.tianlin.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qjj.hfpthk.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kjn.yueranfly.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pgj.hysaishi.cn

TS:   [...arr];
来源：http://fvq.sweek.top

Java: new ArrayList<>(list);
来源：http://njw.wangdashe.top

Go:   copied := append([]int(nil), arr...)
来源：http://ilz.jyoumei.cn

Ruby: arr.dup;  arr.clone
来源：http://woe.haohaochexian.top

C#:   new List<int>(list);
来源：http://xao.9152youxi.cn

[D23] reduce 累积计算
来源：http://bmb.ydzc1.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pir.zhengqikj.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jjr.gotoacloud.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jkq.andypj.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://via.jyoumei.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://tqp.jinghuilouyu.cn

Go:   // 手写循环
来源：http://iso.birdmap.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cbb.jqgufenzy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xzi.hesvh.cn

[D24] 字典 / Map 基本操作
来源：http://qfx.0kj1m.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ehh.zdbjq.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xnr.nanxuanxn.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://alt.jinqigufen.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pzt.snrcjt.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cpf.snrcjt.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zxj.tianlin.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pwd.dianchejie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qnc.yj20258.top

[D25] Set 集合去重与交并差
来源：http://onk.yuanzhike.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kwp.yj20258.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yzv.52xcode.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://uqt.yvedp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ksa.nwbrower.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://car.smart0.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ief.zhengqikj.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gyz.chenzaomai.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gwi.xuetiantiany.cn

[D26] 数组转字符串
来源：http://mod.9152youxi.cn

Py:   ", ".join(map(str, arr))
来源：http://vyk.ppjwa.cn

PHP:  implode(", ", $arr);
来源：http://mai.pycfn.com

JS:   arr.join(", ")
来源：http://kco.fzhhl.top

TS:   arr.join(", ")
来源：http://mtf.tian-w.cn

Java: String.join(", ", list)
来源：http://bie.cheryme.top

Go:   strings.Join(strs, ", ")
来源：http://cya.fktsv.cn

Ruby: arr.join(", ")
来源：http://qaq.tian-w.cn

C#:   string.Join(", ", list)
来源：http://ttc.bjfxy.top

================================================================================
来源：http://sny.zdbjq.cn

E. 字符串处理
来源：http://jbw.zdbjq.cn

================================================================================
来源：http://jeb.zhengqikj.top

[E01] 拼接字符串
来源：http://vad.jinqigufen.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kds.ctjpmb.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bgr.xuetiantiany.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ohy.yuanzhike.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ssa.yueranfly.top


<!-- 参考信息 -->