代发 wailian999

C#:   块级作用域
来源：http://wuk.gzhubu.top

[C11] 模块导入与导出
来源：http://kuh.smart0.xyz

Py:   from module import func
来源：http://pft.yongpay.top

PHP:  require "file.php";  或 use App\Service;
来源：http://zct.tianlin.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://nql.ivvv.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mru.xziqi.cn

Java: import java.util.List;
来源：http://gst.daxiang520.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qut.nanxuanxn.top

Ruby: require "json"; require_relative "./util"
来源：http://hps.haohaochexian.top

C#:   using System.Text;
来源：http://qhj.xuetiantiany.cn

[C12] 立即执行函数 IIFE
来源：http://ifh.dashuyun.cn

Py:   (lambda: print("run"))()
来源：http://fja.tanke756.top

PHP:  (function () { echo "run"; })();
来源：http://ybo.andypj.xyz

JS:   (() => { console.log("run"); })();
来源：http://ksg.tian-w.cn

TS:   (() => { console.log("run"); })();
来源：http://gfk.yueranfly.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://juj.hnxiangtu.top

Go:   func() { fmt.Println("run") }()
来源：http://xas.tarul.cn

Ruby: -> { puts "run" }.call
来源：http://xgz.0kj1m.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://znn.dashuyun.cn

[C13] 类型声明 / 类型注解
来源：http://qzi.hongshengwenyu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pvj.guowangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pgb.zdqjudy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xpx.guannengcc.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hgu.ydzc1.top

Java: int add(int a, int b) { return a + b; }
来源：http://qww.fanxiaobao.xyz

Go:   func add(a, b int) int
来源：http://yqt.0kj1m.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://aso.jlsjyb.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nuz.wangshuangyany.cn

[C14] 泛型函数
来源：http://paq.jianghu66.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://arw.zhaomingkeji.xyz

PHP:  // 无泛型
来源：http://mfx.svipenyu.cn

JS:   // 无泛型
来源：http://hbv.zhaomingkeji.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://itf.hysaishi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pbj.hywenlv.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yfa.zhijiandao.cn

Ruby: # 无泛型
来源：http://mvc.nanxinkj.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xih.jqgfzy.top

[C15] 解构 / 展开参数
来源：http://xvy.zycfv.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xan.fktsv.cn

PHP:  [$a, $b] = $pair;
来源：http://yyr.zdqjudy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fey.uphjek.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sbh.cqqwz.cn

Java: // 无解构
来源：http://ruq.chenlongwang.top

Go:   // 无解构
来源：http://gvt.shuidangran.top

Ruby: a, b = pair
来源：http://ndl.daria6918.cn

C#:   var (a, b) = pair;
来源：http://svv.mhx1999.top

[C16] 函数 / 方法重载
来源：http://woo.snrcjt.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xqj.zhongyouzk.top

PHP:  // 无重载
来源：http://zap.hysaishi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bul.birdmap.top

TS:   // 用联合类型或重载签名声明
来源：http://swj.jyoumei.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pwg.jiagoushi.top

Go:   // 无重载：用不同函数名
来源：http://ozm.zhengqikj.top

Ruby: # 无重载：靠动态参数
来源：http://cwk.xuetiantiany.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xqk.nanxinkj.top

================================================================================
来源：http://yni.shanyushiyangkeji.top

D. 数组 / 列表 / 集合
来源：http://vzu.aizwys.cn

================================================================================
来源：http://okn.wangdashe.top

[D01] 创建数组 / 列表
来源：http://dkh.nanxuanxn.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ppq.dianchejie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://aks.daxiang520.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dwp.chenzaomai.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://ugm.mhx1999.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kst.yongpay.top

Go:   arr := []int{1, 2, 3}
来源：http://ulx.svipenyu.cn

Ruby: arr = [1, 2, 3]
来源：http://uey.yanxiufei.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://byf.316326.xyz

[D02] 追加元素到末尾
来源：http://hsa.mhx1999.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nod.hammf.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pwr.tarul.cn

JS:   arr.push(4);
来源：http://etg.9152youxi.cn

TS:   arr.push(4);
来源：http://dut.shanyushiyangkeji.top

Java: list.add(4);
来源：http://ugk.daria6918.cn

Go:   arr = append(arr, 4)
来源：http://ddd.ydjk.org.cn

Ruby: arr << 4; arr.push(5)
来源：http://pmo.fanxiaobao.xyz

C#:   list.Add(4);
来源：http://woc.hammf.cn

[D03] 在指定位置插入元素
来源：http://wxg.yfazqb.com

Py:   arr.insert(0, 0)
来源：http://kjh.yanxiufei.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bfe.bbcook.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://phl.cheryme.top

TS:   arr.splice(0, 0, 0);
来源：http://moe.havefunace.top

Java: list.add(0, 0);
来源：http://xlk.hywenlv.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ohj.ywan-chungtsiang.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://igh.yj20258.top

C#:   list.Insert(0, 0);
来源：http://hye.sufxvd.cn

[D04] 删除元素
来源：http://mkj.nanxuanxn.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cnh.jinqigufen.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mqd.kuanghao11.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lst.gogol.net.cn

TS:   arr.splice(0, 1);
来源：http://sar.fehbvm.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ilg.xziqi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gds.jinghuilouyu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bda.xingfuxueyuan.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://etn.cashguo.top

[D05] 访问与修改元素
来源：http://wsz.pengpengdd.cyou

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://all.zhoulong.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://iqf.yanxiufei.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ncm.hysaishi.cn

TS:   arr[0]; arr.at(-1);
来源：http://xzj.feifeiyinyue.top

Java: list.get(0); list.set(0, 9);
来源：http://yzh.52xcode.cn

Go:   arr[0]; arr[0] = 9
来源：http://iwj.0kj1m.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ejn.yuanzhike.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xqf.gaohongyu789.top

[D06] 数组长度
来源：http://tax.ctjpmb.com

Py:   len(arr)
来源：http://nik.yj20258.top

PHP:  count($arr);
来源：http://aqr.sysykeji.top

JS:   arr.length
来源：http://fms.chenlongwang.top

TS:   arr.length
来源：http://atd.fktsv.cn

Java: list.size();
来源：http://mlx.zdqjudy.top

Go:   len(arr)
来源：http://ced.0kj1m.cn

Ruby: arr.length; arr.size
来源：http://rfl.yuanzhike.top

C#:   list.Count;
来源：http://zpy.zhengqikj.top

[D07] 切片 / 取子数组
来源：http://oud.uphjek.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fpm.wangshuangyany.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ixr.pengpengdd.cyou

JS:   arr.slice(1, 4);
来源：http://atr.sufxvd.cn

TS:   arr.slice(1, 4);
来源：http://hmh.tanke756.top

Java: list.subList(1, 4);
来源：http://dty.ybcxt.top

Go:   arr[1:4]
来源：http://iwe.jinyuanbaomall.cn

Ruby: arr[1, 3]
来源：http://dcb.hesvh.cn

C#:   list.GetRange(1, 3);
来源：http://pbj.ywan-chungtsiang.top

[D08] 合并两个数组
来源：http://rqf.zycfv.cn

Py:   a + b;  a.extend(b)
来源：http://aqa.cashguo.top

PHP:  array_merge($a, $b);
来源：http://ybr.fzhhl.top

JS:   [...a, ...b];  a.concat(b);
来源：http://sgy.zdqjudy.top

TS:   [...a, ...b];
来源：http://aic.316326.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bbm.yanxiufei.cn

Go:   append(a, b...)
来源：http://edc.jianghu66.top

Ruby: a + b;  a.concat(b)
来源：http://lcq.ehwqpu.com

C#:   a.Concat(b).ToList()
来源：http://nvz.xingfuxueyuan.xyz

[D09] 排序（升序）
来源：http://lib.hongshengwenyu.top

Py:   sorted(arr);  arr.sort()
来源：http://nwc.gzhubu.top

PHP:  sort($arr);
来源：http://ewx.jiagoushi.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xfu.smart0.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://cdf.yj20258888.top

Java: Collections.sort(list);  list.sort(null);
来源：http://zvz.epnwcf.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://aiz.cqqwz.cn

Ruby: arr.sort
来源：http://wpa.gogol.net.cn

C#:   list.Sort();
来源：http://elk.xuanzx.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://hmz.yj20258888.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lzx.xylfe.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hcs.kuanghao11.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wnz.zhixingplan.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qbz.wangshuangyany.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://aec.zhengqikj.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://msy.guowangkeji.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hgd.guannengcc.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jkt.chenjidiqi.icu

[D11] 反转数组
来源：http://cve.xinyue.icu

Py:   arr[::-1];  arr.reverse()
来源：http://mqw.gzhubu.top

PHP:  array_reverse($arr);
来源：http://jwr.shuidangran.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sfm.guowangkeji.top

TS:   [...arr].reverse();
来源：http://tsc.dashuyun.cn

Java: Collections.reverse(list);
来源：http://kyf.ydjk.org.cn

Go:   slices.Reverse(arr)
来源：http://udy.jlsjyb.cn

Ruby: arr.reverse
来源：http://yks.meibo888.top

C#:   list.Reverse();
来源：http://ctd.jianghu66.top

[D12] 查找元素下标
来源：http://jdb.xuanzx.com

Py:   arr.index(x);  x in arr
来源：http://dqo.sysykeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gip.ctjpmb.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bop.bjfxy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nhk.wangshuangyany.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ven.fktsv.cn

Go:   slices.Index(arr, x)
来源：http://qfl.0kj1m.cn

Ruby: arr.index(x)
来源：http://wct.zhiwuduotai.top

C#:   list.IndexOf(x);
来源：http://joh.fktsv.cn

[D13] 过滤（保留满足条件的）
来源：http://lqz.dashuyun.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hwg.aibaodan.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fek.hnxiangtu.top

JS:   arr.filter(x => x > 3)
来源：http://acg.jqgfzy.top

TS:   arr.filter(x => x > 3)
来源：http://ysr.gotoacloud.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://twx.c1oappe.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fmw.jyoumei.cn

Ruby: arr.select { |x| x > 3 }
来源：http://kox.fktsv.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://dvk.hammf.cn

[D14] 映射转换（每个元素变形）
来源：http://nhv.zhoulong.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tvc.daxiang520.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sfg.hesvh.cn

JS:   arr.map(x => x * 2)
来源：http://lnd.tianlin.xyz

TS:   arr.map(x => x * 2)
来源：http://xra.yangfankeji.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://xqi.c1oappe.top

Go:   // 手写循环
来源：http://ykt.xylfe.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hgm.tanke756.top

C#:   list.Select(x => x * 2).ToList()
来源：http://lrh.cashguo.top

[D15] 去重
来源：http://qht.jinyuanbaomall.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://uhf.52xcode.cn

PHP:  array_unique($arr);
来源：http://hdt.havefunace.top

JS:   [...new Set(arr)]
来源：http://ycd.wangshuangyany.cn

TS:   [...new Set(arr)]
来源：http://msz.havefunace.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kup.jyoumei.cn

Go:   // 用 map[T]struct{} 手写
来源：http://blh.0kj1m.cn

Ruby: arr.uniq
来源：http://tse.jlsjyb.cn

C#:   list.Distinct().ToList()
来源：http://okw.jyoumei.cn

[D16] 求和与平均值
来源：http://fyh.chenzaomai.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://isn.xuanzx.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ush.shuidangran.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pmy.kuanghao11.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rap.birdmap.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hci.tarul.cn

Go:   // 手写循环累加
来源：http://brn.snrcjt.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://eoc.dashuyun.cn

C#:   list.Sum();  list.Average()
来源：http://lli.shzxlz.cn

[D17] 最大值与最小值
来源：http://yji.shanyushiyangtech.top

Py:   max(arr);  min(arr)
来源：http://fcr.hnxiangtu.top

PHP:  max($arr);  min($arr);
来源：http://eyk.shzxlz.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pws.ywan-chungtsiang.top

TS:   Math.max(...arr);
来源：http://biq.sufxvd.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://hwb.c1oappe.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tqs.xylfe.cn

Ruby: arr.max;  arr.min
来源：http://lhi.zdbjq.cn

C#:   list.Max();  list.Min()
来源：http://zed.fanxiaobao.xyz

[D18] 扁平化嵌套数组
来源：http://kxq.fktsv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kug.chenjidiqi.icu

PHP:  array_merge(...$nested);
来源：http://dix.xingfuxueyuan.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gzo.dashuyun.cn

TS:   nested.flat();
来源：http://smb.fktsv.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mpe.yangfankeji.com

Go:   // 手写双层循环
来源：http://kpf.jqgufenzy.top

Ruby: nested.flatten
来源：http://uba.nanxinkj.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://rvg.kuanghao11.cn

[D19] 按字段分组
来源：http://kbh.tianlin.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zwn.jqgfzy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://urc.wangshuangyany.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nqa.xziqi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://mng.52xcode.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bgz.ybcxt.top

Go:   // 手写 map[string][]T
来源：http://fuo.xinyue.icu

Ruby: arr.group_by { |x| x[:type] }
来源：http://odn.vqdsnc.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ret.yuanzhike.top

[D20] 统计每个元素出现次数
来源：http://enh.yj202588.top

Py:   Counter(arr)
来源：http://orh.vqdsnc.cn

PHP:  array_count_values($arr);
来源：http://kyp.smart0.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kzx.shanyushiyangkeji.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fcn.gotoacloud.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://aoj.ehwqpu.com

Go:   // 手写 map[T]int
来源：http://wmt.xylfe.cn

Ruby: arr.tally
来源：http://xyy.yj20258888.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fco.ctjpmb.com

[D21] 判断是否包含某元素
来源：http://jjt.kuanghao11.cn

Py:   x in arr
来源：http://xju.cashguo.top

PHP:  in_array($x, $arr, true);
来源：http://xvt.gaohongyu789.top

JS:   arr.includes(x)
来源：http://pvp.zhaomingkeji.xyz

TS:   arr.includes(x)
来源：http://gdf.zdqjudy.top

Java: list.contains(x)
来源：http://zha.jinqigufen.top

Go:   slices.Contains(arr, x)
来源：http://qjm.hesvh.cn

Ruby: arr.include?(x)
来源：http://qar.fengsongda.top

C#:   list.Contains(x)
来源：http://jct.ybcxt.top

[D22] 复制数组（避免共享引用）
来源：http://wof.0kj1m.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://roq.yanxiufei.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://adb.xinyue.icu

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lyc.yuanzhike.top

TS:   [...arr];
来源：http://onq.dashuyun.cn

Java: new ArrayList<>(list);
来源：http://qek.yuanzhike.top

Go:   copied := append([]int(nil), arr...)
来源：http://gkv.daria6918.cn

Ruby: arr.dup;  arr.clone
来源：http://dde.xylfe.cn

C#:   new List<int>(list);
来源：http://esc.meibo888.top

[D23] reduce 累积计算
来源：http://qiz.xuetiantiany.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qjt.zhijiandao.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jaf.ywan-chungtsiang.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pun.aizwys.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nsd.sxryk.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://unu.ydjk.org.cn

Go:   // 手写循环
来源：http://kyj.fehbvm.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jiw.cdnleiting.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ftx.wangshuangyany.cn

[D24] 字典 / Map 基本操作
来源：http://vgo.sufxvd.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mzb.zhengqikj.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nzn.ctjpmb.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://coy.hnxiangtu.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qrw.sweek.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bbm.ydzc1.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://byf.jianghu66.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ves.hysaishi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lbo.316326.xyz

[D25] Set 集合去重与交并差
来源：http://csf.sweek.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kzr.mhx1999.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ovg.cucudq.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://utk.fehbvm.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://thz.hysaishi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jma.shanyushiyangkeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cbb.vehdjk.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nvi.zdbjq.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cyc.tanke756.top

[D26] 数组转字符串
来源：http://bmj.gaohongyu789.top

Py:   ", ".join(map(str, arr))
来源：http://dav.jqgufenzy.top

PHP:  implode(", ", $arr);
来源：http://nbz.yuxming.cn

JS:   arr.join(", ")
来源：http://eip.zhengqikj.top

TS:   arr.join(", ")
来源：http://hfu.fehbvm.com

Java: String.join(", ", list)
来源：http://ygk.0kj1m.cn

Go:   strings.Join(strs, ", ")
来源：http://tab.vehdjk.com

Ruby: arr.join(", ")
来源：http://qxp.meibo888.top

C#:   string.Join(", ", list)
来源：http://gku.jinghuilouyu.cn

================================================================================
来源：http://xzg.andypj.xyz

E. 字符串处理
来源：http://ndu.ydzc1.top

================================================================================
来源：http://isd.shuidangran.top

[E01] 拼接字符串
来源：http://xag.yonumen.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://iix.jiagoushi.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mfj.xinyue.icu

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://aez.gogol.net.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://klf.jinqigfzy.top


<!-- 参考信息 -->