代发 wailian999

C#:   块级作用域
来源：http://gbn.gotoacloud.top

[C11] 模块导入与导出
来源：http://gxw.ywan-chungtsiang.top

Py:   from module import func
来源：http://yax.0kj1m.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wsb.yj20258888.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://dqk.havefunace.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://eca.fanxiaobao.xyz

Java: import java.util.List;
来源：http://xxq.ydjk.org.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sxu.zhiwuduotai.top

Ruby: require "json"; require_relative "./util"
来源：http://igb.meibo888.top

C#:   using System.Text;
来源：http://bzz.yvedp.cn

[C12] 立即执行函数 IIFE
来源：http://ria.aizwys.cn

Py:   (lambda: print("run"))()
来源：http://yuw.zycfv.cn

PHP:  (function () { echo "run"; })();
来源：http://dqy.zhengqikj.top

JS:   (() => { console.log("run"); })();
来源：http://vkh.sweek.top

TS:   (() => { console.log("run"); })();
来源：http://moi.shangyingyoupin.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qgz.zhongyouzk.top

Go:   func() { fmt.Println("run") }()
来源：http://upg.daria6918.cn

Ruby: -> { puts "run" }.call
来源：http://lhw.zhongyouzk.top

C#:   // 无 IIFE：用静态构造函数
来源：http://tbi.sweek.top

[C13] 类型声明 / 类型注解
来源：http://bok.gzhubu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rdz.9152youxi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lqm.bbcook.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mlj.xinyue.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://esd.zhixingplan.top

Java: int add(int a, int b) { return a + b; }
来源：http://ydk.jinqigufen.top

Go:   func add(a, b int) int
来源：http://bwr.snrcjt.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vdo.wangdashe.top

C#:   int Add(int a, int b) => a + b;
来源：http://lmb.gaohongyu789.top

[C14] 泛型函数
来源：http://hwu.nwbrower.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ack.jqgufenzy.top

PHP:  // 无泛型
来源：http://mvk.jinyuanbaomall.cn

JS:   // 无泛型
来源：http://tbu.hnxiangtu.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://snl.fanxiaobao.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ckp.ehwqpu.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://aje.gogol.net.cn

Ruby: # 无泛型
来源：http://yya.316326.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mku.hnqzz.top

[C15] 解构 / 展开参数
来源：http://sft.fengsongda.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fva.sweek.top

PHP:  [$a, $b] = $pair;
来源：http://vpf.ydjk.org.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yjg.zhengqikj.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qhy.uphjek.com

Java: // 无解构
来源：http://pev.sysykeji.top

Go:   // 无解构
来源：http://lxd.gotoacloud.top

Ruby: a, b = pair
来源：http://dad.birdmap.top

C#:   var (a, b) = pair;
来源：http://ezc.mhx1999.top

[C16] 函数 / 方法重载
来源：http://hnj.fanxiaobao.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://iod.aibaodan.cn

PHP:  // 无重载
来源：http://smf.shuidangran.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://otf.hnxiangtu.top

TS:   // 用联合类型或重载签名声明
来源：http://dxa.ehwqpu.com

Java: void f(int a) {}  void f(String a) {}
来源：http://fvg.cashguo.top

Go:   // 无重载：用不同函数名
来源：http://sck.jqgfzy.top

Ruby: # 无重载：靠动态参数
来源：http://tbh.xuanzx.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://jme.gzhubu.top

================================================================================
来源：http://eku.vqdsnc.cn

D. 数组 / 列表 / 集合
来源：http://mpt.52xcode.cn

================================================================================
来源：http://iyn.kuanghao11.cn

[D01] 创建数组 / 列表
来源：http://ice.aibaodan.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fit.jinghuilouyu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wry.sweek.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ubf.meibo888.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://lkk.zhijiandao.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zwq.uphjek.com

Go:   arr := []int{1, 2, 3}
来源：http://ccq.sysykeji.top

Ruby: arr = [1, 2, 3]
来源：http://wvd.guowangkeji.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pwv.jinghuilouyu.cn

[D02] 追加元素到末尾
来源：http://hlc.ivvv.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hgu.wangdashe.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://psi.svipenyu.cn

JS:   arr.push(4);
来源：http://saf.xingfuxueyuan.xyz

TS:   arr.push(4);
来源：http://uji.chenlongwang.top

Java: list.add(4);
来源：http://qwb.fengsongda.top

Go:   arr = append(arr, 4)
来源：http://znc.ywan-chungtsiang.top

Ruby: arr << 4; arr.push(5)
来源：http://dlu.nwbrower.top

C#:   list.Add(4);
来源：http://uoi.hesvh.cn

[D03] 在指定位置插入元素
来源：http://zkg.yonumen.top

Py:   arr.insert(0, 0)
来源：http://fnu.52xcode.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vov.hywenlv.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qyp.hysaishi.cn

TS:   arr.splice(0, 0, 0);
来源：http://qho.jqgfzy.top

Java: list.add(0, 0);
来源：http://zam.andypj.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://zqw.kuanghao11.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hhf.fengsongda.top

C#:   list.Insert(0, 0);
来源：http://gne.tianlin.xyz

[D04] 删除元素
来源：http://pfw.andypj.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ley.quarkkingdee.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://eme.sufxvd.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wvg.hcnkem.com

TS:   arr.splice(0, 1);
来源：http://slr.tian-w.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mcy.zhijiandao.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rmv.jinghuilouyu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ect.yueranfly.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://iws.shangyingyoupin.top

[D05] 访问与修改元素
来源：http://giq.shangyingyoupin.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://izh.sufxvd.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ypv.nwbrower.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wcg.zdbjq.cn

TS:   arr[0]; arr.at(-1);
来源：http://pqr.yonumen.top

Java: list.get(0); list.set(0, 9);
来源：http://cwv.smart0.xyz

Go:   arr[0]; arr[0] = 9
来源：http://uya.shzxlz.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://quz.c1oappe.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ubr.jinyuanbaomall.cn

[D06] 数组长度
来源：http://kjl.zhengqikj.top

Py:   len(arr)
来源：http://nin.hfpthk.cn

PHP:  count($arr);
来源：http://brl.yanxiufei.cn

JS:   arr.length
来源：http://jtr.aizwys.cn

TS:   arr.length
来源：http://qte.nanxuanxn.top

Java: list.size();
来源：http://vnh.sxryk.cn

Go:   len(arr)
来源：http://sci.yj202588.top

Ruby: arr.length; arr.size
来源：http://mth.nanxuanxn.top

C#:   list.Count;
来源：http://gnw.chenjidiqi.icu

[D07] 切片 / 取子数组
来源：http://zvw.yonumen.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bvq.yangfankeji.com

PHP:  array_slice($arr, 1, 3);
来源：http://mnz.jqgfzy.top

JS:   arr.slice(1, 4);
来源：http://vxd.zhaomingkeji.xyz

TS:   arr.slice(1, 4);
来源：http://bnx.tarul.cn

Java: list.subList(1, 4);
来源：http://ieb.0kj1m.cn

Go:   arr[1:4]
来源：http://wkx.quarkkingdee.top

Ruby: arr[1, 3]
来源：http://wpo.chenlongwang.top

C#:   list.GetRange(1, 3);
来源：http://qcr.yuxming.cn

[D08] 合并两个数组
来源：http://bse.nanxuanxn.top

Py:   a + b;  a.extend(b)
来源：http://lhe.xuetiantiany.cn

PHP:  array_merge($a, $b);
来源：http://ruw.aizwys.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://jri.shanyushiyangkeji.top

TS:   [...a, ...b];
来源：http://xqh.tianlin.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hbr.ydjk.org.cn

Go:   append(a, b...)
来源：http://wew.sxryk.cn

Ruby: a + b;  a.concat(b)
来源：http://hvn.hywenlv.cn

C#:   a.Concat(b).ToList()
来源：http://mat.yfazqb.com

[D09] 排序（升序）
来源：http://tck.yj202588.top

Py:   sorted(arr);  arr.sort()
来源：http://rjv.yueranfly.top

PHP:  sort($arr);
来源：http://cvn.aibaodan.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kpt.zhixingplan.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://doq.tarul.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://uth.yvedp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rwy.hnqzz.top

Ruby: arr.sort
来源：http://pwo.sjlbkw.cn

C#:   list.Sort();
来源：http://fbq.pengpengdd.cyou

[D10] 自定义排序（按字段 / 多条件）
来源：http://okx.316326.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lgf.andypj.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://onq.daria6918.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fjh.fehbvm.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://def.tian-w.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xbj.bbcook.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uhj.chenzaomai.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gtj.zhongyouzk.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://izk.316326.xyz

[D11] 反转数组
来源：http://ewx.hfpthk.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ogz.hywenlv.cn

PHP:  array_reverse($arr);
来源：http://zly.gogol.net.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zvg.jinyuanbaomall.cn

TS:   [...arr].reverse();
来源：http://weu.yuxming.cn

Java: Collections.reverse(list);
来源：http://thq.guannengcc.top

Go:   slices.Reverse(arr)
来源：http://buq.jqgfzy.top

Ruby: arr.reverse
来源：http://dsy.ydjk.org.cn

C#:   list.Reverse();
来源：http://rte.shanyushiyangtech.top

[D12] 查找元素下标
来源：http://fpv.shanyushiyangkeji.top

Py:   arr.index(x);  x in arr
来源：http://bcm.hysaishi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://oth.pengpengdd.cyou

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cak.tianlin.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://igb.aizwys.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://msw.zdbjq.cn

Go:   slices.Index(arr, x)
来源：http://byw.chenlongwang.top

Ruby: arr.index(x)
来源：http://osw.xuanzx.com

C#:   list.IndexOf(x);
来源：http://szm.zhijiandao.cn

[D13] 过滤（保留满足条件的）
来源：http://jkq.cdnleiting.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lyj.zhiwuduotai.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qfv.zhaomingkeji.xyz

JS:   arr.filter(x => x > 3)
来源：http://slq.pycfn.com

TS:   arr.filter(x => x > 3)
来源：http://jfs.chenjidiqi.icu

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zww.fzhhl.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nqn.0kj1m.cn

Ruby: arr.select { |x| x > 3 }
来源：http://kmt.hcnkem.com

C#:   list.Where(x => x > 3).ToList()
来源：http://ljq.jianghu66.top

[D14] 映射转换（每个元素变形）
来源：http://nhr.tian-w.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://txn.cashguo.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vwd.hnxiangtu.top

JS:   arr.map(x => x * 2)
来源：http://fsd.tianlin.xyz

TS:   arr.map(x => x * 2)
来源：http://puo.pengpengdd.cyou

Java: list.stream().map(x -> x * 2).toList()
来源：http://rci.feifeiyinyue.top

Go:   // 手写循环
来源：http://bop.svipenyu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fvo.nanxuanxn.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ofs.nwbrower.top

[D15] 去重
来源：http://frn.gaohongyu789.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cla.sysykeji.top

PHP:  array_unique($arr);
来源：http://roz.wangshuangyany.cn

JS:   [...new Set(arr)]
来源：http://blj.hywenlv.cn

TS:   [...new Set(arr)]
来源：http://wlm.pengpengdd.cyou

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wlv.cheryme.top

Go:   // 用 map[T]struct{} 手写
来源：http://npo.sxryk.cn

Ruby: arr.uniq
来源：http://sdc.smart0.xyz

C#:   list.Distinct().ToList()
来源：http://wff.yuanzhike.top

[D16] 求和与平均值
来源：http://afc.zdbjq.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hrp.aibaodan.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pss.jinyuanbaomall.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bee.shanyushiyangtech.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blv.haohaochexian.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rfl.gaohongyu789.top

Go:   // 手写循环累加
来源：http://dvh.sxryk.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xwl.jinyuanbaomall.cn

C#:   list.Sum();  list.Average()
来源：http://wyo.andypj.xyz

[D17] 最大值与最小值
来源：http://ykv.wangshuangyany.cn

Py:   max(arr);  min(arr)
来源：http://yhn.chenzaomai.com

PHP:  max($arr);  min($arr);
来源：http://rtg.andypj.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rlt.yuanzhike.top

TS:   Math.max(...arr);
来源：http://izj.yuanzhike.top

Java: Collections.max(list);  Collections.min(list);
来源：http://wus.fehbvm.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tsr.tian-w.cn

Ruby: arr.max;  arr.min
来源：http://jhd.zdbjq.cn

C#:   list.Max();  list.Min()
来源：http://obp.yuanzhike.top

[D18] 扁平化嵌套数组
来源：http://nsf.vqdsnc.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dof.shanyushiyangkeji.top

PHP:  array_merge(...$nested);
来源：http://rrv.cqqwz.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ktv.xuanzx.com

TS:   nested.flat();
来源：http://qmu.xylfe.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fsm.cucudq.cn

Go:   // 手写双层循环
来源：http://txp.gogol.net.cn

Ruby: nested.flatten
来源：http://zum.ehwqpu.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://ydo.tarul.cn

[D19] 按字段分组
来源：http://gum.hammf.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yae.9152youxi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nwk.52xcode.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xlc.jinqigfzy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://fhr.yuxming.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://puo.yueranfly.top

Go:   // 手写 map[string][]T
来源：http://utp.guowangkeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://dju.zhengqikj.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gkf.dashuyun.cn

[D20] 统计每个元素出现次数
来源：http://cgj.hesvh.cn

Py:   Counter(arr)
来源：http://veg.haohaochexian.top

PHP:  array_count_values($arr);
来源：http://fdp.hfpthk.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xhp.dashuyun.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fyj.iojbl.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hix.aizwys.cn

Go:   // 手写 map[T]int
来源：http://dir.cqqwz.cn

Ruby: arr.tally
来源：http://qqm.yj202588.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ocg.xingfuxueyuan.xyz

[D21] 判断是否包含某元素
来源：http://xyf.nanxinkj.top

Py:   x in arr
来源：http://mgh.havefunace.top

PHP:  in_array($x, $arr, true);
来源：http://pnn.zhixingplan.top

JS:   arr.includes(x)
来源：http://eqv.shanyushiyangtech.top

TS:   arr.includes(x)
来源：http://ymf.bjfxy.top

Java: list.contains(x)
来源：http://osx.fzhhl.top

Go:   slices.Contains(arr, x)
来源：http://izm.316326.xyz

Ruby: arr.include?(x)
来源：http://dao.zhengqikj.top

C#:   list.Contains(x)
来源：http://jlu.hammf.cn

[D22] 复制数组（避免共享引用）
来源：http://ytk.pycfn.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ulk.xinyue.icu

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://geg.zhijiandao.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tdn.sjlbkw.cn

TS:   [...arr];
来源：http://hte.iojbl.cn

Java: new ArrayList<>(list);
来源：http://iuv.zhiwuduotai.top

Go:   copied := append([]int(nil), arr...)
来源：http://zkl.zhixingplan.top

Ruby: arr.dup;  arr.clone
来源：http://azr.bjfxy.top

C#:   new List<int>(list);
来源：http://wpf.daxiang520.top

[D23] reduce 累积计算
来源：http://bbs.316326.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dzj.ydzc1.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hkx.yfazqb.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yim.9152youxi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cuz.fanxiaobao.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://gkj.hnqzz.top

Go:   // 手写循环
来源：http://guk.ybcxt.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://smr.xylfe.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wyr.gotoacloud.top

[D24] 字典 / Map 基本操作
来源：http://woo.yj202588.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kjj.zhijiandao.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cde.pengpengdd.cyou

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ghl.epnwcf.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hhm.hcnkem.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://asy.yuxming.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ewn.vehdjk.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bua.yanxiufei.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pmv.feifeiyinyue.top

[D25] Set 集合去重与交并差
来源：http://xgp.epnwcf.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://acw.yfazqb.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://upu.zycfv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zqf.dashuyun.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://urh.xuanzx.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://oyw.yj20258.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jsq.jyoumei.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ggx.316326.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ezo.kuanghao11.cn

[D26] 数组转字符串
来源：http://ckn.shanyushiyangkeji.top

Py:   ", ".join(map(str, arr))
来源：http://noc.yonumen.top

PHP:  implode(", ", $arr);
来源：http://ntg.jqgfzy.top

JS:   arr.join(", ")
来源：http://uri.vqdsnc.cn

TS:   arr.join(", ")
来源：http://jyb.zhixingplan.top

Java: String.join(", ", list)
来源：http://efa.feifeiyinyue.top

Go:   strings.Join(strs, ", ")
来源：http://sge.cqqwz.cn

Ruby: arr.join(", ")
来源：http://sti.tarul.cn

C#:   string.Join(", ", list)
来源：http://gnh.yj20258888.top

================================================================================
来源：http://jzy.9152youxi.cn

E. 字符串处理
来源：http://ogl.9152youxi.cn

================================================================================
来源：http://jcw.jinqigfzy.top

[E01] 拼接字符串
来源：http://ovz.fengsongda.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fwk.xinyue.icu

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mic.yonumen.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wdd.vehdjk.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kcb.0kj1m.cn


<!-- 参考信息 -->