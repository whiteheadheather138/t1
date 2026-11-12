代发 wailian999

TS:   同 JS
来源：http://cna.yvedp.cn

Java: 方法内为块级作用域
来源：http://jrz.zhixingplan.top

Go:   花括号块级作用域
来源：http://gvf.sufxvd.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xyp.gaohongyu789.top

C#:   块级作用域
来源：http://xfr.ydjk.org.cn

[C11] 模块导入与导出
来源：http://ymg.ywan-chungtsiang.top

Py:   from module import func
来源：http://jlb.xylfe.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xhb.daria6918.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rmv.jqgfzy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ajh.hywenlv.cn

Java: import java.util.List;
来源：http://zed.xuetiantiany.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cpk.guowangkeji.top

Ruby: require "json"; require_relative "./util"
来源：http://tyy.havefunace.top

C#:   using System.Text;
来源：http://cnf.0kj1m.cn

[C12] 立即执行函数 IIFE
来源：http://zet.hnqzz.top

Py:   (lambda: print("run"))()
来源：http://ust.shanyushiyangtech.top

PHP:  (function () { echo "run"; })();
来源：http://ljr.sysykeji.top

JS:   (() => { console.log("run"); })();
来源：http://qfn.yangfankeji.com

TS:   (() => { console.log("run"); })();
来源：http://foy.yanxiufei.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wzm.shangyingyoupin.top

Go:   func() { fmt.Println("run") }()
来源：http://heu.chenjidiqi.icu

Ruby: -> { puts "run" }.call
来源：http://ctb.zdqjudy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ell.fengsongda.top

[C13] 类型声明 / 类型注解
来源：http://oew.hesvh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vpp.pycfn.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dfm.0kj1m.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://use.ybcxt.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eni.ctjpmb.com

Java: int add(int a, int b) { return a + b; }
来源：http://uxw.ppjwa.cn

Go:   func add(a, b int) int
来源：http://yhh.hysaishi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://umu.chenjidiqi.icu

C#:   int Add(int a, int b) => a + b;
来源：http://guf.nanxinkj.top

[C14] 泛型函数
来源：http://dgb.redwolf501.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mvk.haohaochexian.top

PHP:  // 无泛型
来源：http://hml.svipenyu.cn

JS:   // 无泛型
来源：http://bxb.jqgufenzy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xla.mhx1999.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gpw.tanke756.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ylx.yj202588.top

Ruby: # 无泛型
来源：http://pmf.aibaodan.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dew.yuanzhike.top

[C15] 解构 / 展开参数
来源：http://sgz.zhaomingkeji.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://put.yj202588.top

PHP:  [$a, $b] = $pair;
来源：http://est.quarkkingdee.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tej.fehbvm.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://keu.yj20258888.top

Java: // 无解构
来源：http://mff.yuxming.cn

Go:   // 无解构
来源：http://dhj.ydzc1.top

Ruby: a, b = pair
来源：http://pjs.jqgufenzy.top

C#:   var (a, b) = pair;
来源：http://axl.hammf.cn

[C16] 函数 / 方法重载
来源：http://prv.zhixingplan.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hrf.sweek.top

PHP:  // 无重载
来源：http://faj.hfpthk.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lyt.ppjwa.cn

TS:   // 用联合类型或重载签名声明
来源：http://fws.yonumen.top

Java: void f(int a) {}  void f(String a) {}
来源：http://tmq.zhengqikj.top

Go:   // 无重载：用不同函数名
来源：http://abz.tianlin.xyz

Ruby: # 无重载：靠动态参数
来源：http://klm.snrcjt.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://moa.chenzaomai.com

================================================================================
来源：http://czq.epnwcf.com

D. 数组 / 列表 / 集合
来源：http://ntp.aizwys.cn

================================================================================
来源：http://ylj.zhaomingkeji.xyz

[D01] 创建数组 / 列表
来源：http://qjh.vqdsnc.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://gbx.jinqigfzy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://glt.hnqzz.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baf.kuanghao11.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fld.xuetiantiany.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qlk.jqgfzy.top

Go:   arr := []int{1, 2, 3}
来源：http://ucl.yangfankeji.com

Ruby: arr = [1, 2, 3]
来源：http://aqf.fehbvm.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xcx.aizwys.cn

[D02] 追加元素到末尾
来源：http://xpg.feifeiyinyue.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bql.yuanzhike.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://eqx.dashuyun.cn

JS:   arr.push(4);
来源：http://psv.svipenyu.cn

TS:   arr.push(4);
来源：http://iwr.bjfxy.top

Java: list.add(4);
来源：http://tjd.hysaishi.cn

Go:   arr = append(arr, 4)
来源：http://gne.hywenlv.cn

Ruby: arr << 4; arr.push(5)
来源：http://aay.svipenyu.cn

C#:   list.Add(4);
来源：http://biz.fengsongda.top

[D03] 在指定位置插入元素
来源：http://sal.havefunace.top

Py:   arr.insert(0, 0)
来源：http://kzv.jyoumei.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cvd.vehdjk.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cmv.yj20258888.top

TS:   arr.splice(0, 0, 0);
来源：http://xwm.daria6918.cn

Java: list.add(0, 0);
来源：http://fst.zhengqikj.top

Go:   arr = append([]int{0}, arr...)
来源：http://ats.dianchejie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dyl.jinqigufen.top

C#:   list.Insert(0, 0);
来源：http://sox.sufxvd.cn

[D04] 删除元素
来源：http://cna.zycfv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ubf.zhongyouzk.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ukx.tarul.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://eyo.jqgufenzy.top

TS:   arr.splice(0, 1);
来源：http://gjv.nanxinkj.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vcz.ctjpmb.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xnr.daxiang520.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zfv.hnxiangtu.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jtk.ydzc1.top

[D05] 访问与修改元素
来源：http://msd.cheryme.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ltg.wangdashe.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kbz.yangfankeji.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bjk.jinghuilouyu.cn

TS:   arr[0]; arr.at(-1);
来源：http://iil.ydjk.org.cn

Java: list.get(0); list.set(0, 9);
来源：http://ogt.cqqwz.cn

Go:   arr[0]; arr[0] = 9
来源：http://oiq.ppjwa.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vxq.mhx1999.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xve.jyoumei.cn

[D06] 数组长度
来源：http://wsl.zdbjq.cn

Py:   len(arr)
来源：http://xeq.jianghu66.top

PHP:  count($arr);
来源：http://zat.xylfe.cn

JS:   arr.length
来源：http://mka.zhaomingkeji.xyz

TS:   arr.length
来源：http://vsl.haohaochexian.top

Java: list.size();
来源：http://cjg.bjfxy.top

Go:   len(arr)
来源：http://nax.hysaishi.cn

Ruby: arr.length; arr.size
来源：http://kgm.316326.xyz

C#:   list.Count;
来源：http://siq.ehwqpu.com

[D07] 切片 / 取子数组
来源：http://rqt.nwbrower.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bgp.xinyue.icu

PHP:  array_slice($arr, 1, 3);
来源：http://ryu.yuxming.cn

JS:   arr.slice(1, 4);
来源：http://vap.yangfankeji.com

TS:   arr.slice(1, 4);
来源：http://joi.meibo888.top

Java: list.subList(1, 4);
来源：http://gen.shangyingyoupin.top

Go:   arr[1:4]
来源：http://dvp.hcnkem.com

Ruby: arr[1, 3]
来源：http://jwl.iojbl.cn

C#:   list.GetRange(1, 3);
来源：http://xaw.bbcook.cn

[D08] 合并两个数组
来源：http://zbm.xziqi.cn

Py:   a + b;  a.extend(b)
来源：http://sli.chenjidiqi.icu

PHP:  array_merge($a, $b);
来源：http://ndp.redwolf501.top

JS:   [...a, ...b];  a.concat(b);
来源：http://nmr.gzhubu.top

TS:   [...a, ...b];
来源：http://byq.aizwys.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cph.dianchejie.cn

Go:   append(a, b...)
来源：http://qwn.sweek.top

Ruby: a + b;  a.concat(b)
来源：http://wto.xziqi.cn

C#:   a.Concat(b).ToList()
来源：http://zky.vqdsnc.cn

[D09] 排序（升序）
来源：http://rtl.yvedp.cn

Py:   sorted(arr);  arr.sort()
来源：http://xuf.guowangkeji.top

PHP:  sort($arr);
来源：http://klt.zdbjq.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://btp.aibaodan.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qwi.zhoulong.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://sxz.sweek.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tey.zdbjq.cn

Ruby: arr.sort
来源：http://yul.zhijiandao.cn

C#:   list.Sort();
来源：http://yec.uphjek.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://dzc.jinqigufen.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mmi.0kj1m.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ycw.hywenlv.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dam.bjfxy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wgy.ppjwa.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xix.chenzaomai.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dsl.haohaochexian.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yqr.shangyingyoupin.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xka.smart0.xyz

[D11] 反转数组
来源：http://guf.fanxiaobao.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://xih.wangshuangyany.cn

PHP:  array_reverse($arr);
来源：http://weg.gzhubu.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fqi.gotoacloud.top

TS:   [...arr].reverse();
来源：http://tcg.sweek.top

Java: Collections.reverse(list);
来源：http://ypx.jinyuanbaomall.cn

Go:   slices.Reverse(arr)
来源：http://kxp.yvedp.cn

Ruby: arr.reverse
来源：http://ghs.tarul.cn

C#:   list.Reverse();
来源：http://bok.wangdashe.top

[D12] 查找元素下标
来源：http://you.hnqzz.top

Py:   arr.index(x);  x in arr
来源：http://xij.jinghuilouyu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://iea.ehwqpu.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ldk.pengpengdd.cyou

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ljs.fanxiaobao.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://iww.sjlbkw.cn

Go:   slices.Index(arr, x)
来源：http://vys.hammf.cn

Ruby: arr.index(x)
来源：http://vyj.yueranfly.top

C#:   list.IndexOf(x);
来源：http://qfa.ydzc1.top

[D13] 过滤（保留满足条件的）
来源：http://pnm.jinghuilouyu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gaa.daxiang520.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://god.ppjwa.cn

JS:   arr.filter(x => x > 3)
来源：http://mve.feifeiyinyue.top

TS:   arr.filter(x => x > 3)
来源：http://pam.hammf.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vbt.quarkkingdee.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://akz.svipenyu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ies.tian-w.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wdc.uphjek.com

[D14] 映射转换（每个元素变形）
来源：http://dqu.zhoulong.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jfs.quarkkingdee.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vpv.yongpay.top

JS:   arr.map(x => x * 2)
来源：http://zrn.iojbl.cn

TS:   arr.map(x => x * 2)
来源：http://hsk.shanyushiyangkeji.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://twt.chenlongwang.top

Go:   // 手写循环
来源：http://vte.vehdjk.com

Ruby: arr.map { |x| x * 2 }
来源：http://cjt.aibaodan.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qpl.hcnkem.com

[D15] 去重
来源：http://dod.yj202588.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://afg.xuanzx.com

PHP:  array_unique($arr);
来源：http://hzd.havefunace.top

JS:   [...new Set(arr)]
来源：http://cbu.jinqigufen.top

TS:   [...new Set(arr)]
来源：http://gtq.feifeiyinyue.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://brl.daxiang520.top

Go:   // 用 map[T]struct{} 手写
来源：http://bbg.daxiang520.top

Ruby: arr.uniq
来源：http://yim.fzhhl.top

C#:   list.Distinct().ToList()
来源：http://rzy.fanxiaobao.xyz

[D16] 求和与平均值
来源：http://ukd.zhijiandao.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://axn.chenjidiqi.icu

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://siq.tianlin.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://awo.hysaishi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jse.birdmap.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jtr.chenjidiqi.icu

Go:   // 手写循环累加
来源：http://xsg.hnxiangtu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://won.svipenyu.cn

C#:   list.Sum();  list.Average()
来源：http://cdf.jinqigfzy.top

[D17] 最大值与最小值
来源：http://gwy.9152youxi.cn

Py:   max(arr);  min(arr)
来源：http://plj.nwbrower.top

PHP:  max($arr);  min($arr);
来源：http://epr.gzhubu.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bsp.yueranfly.top

TS:   Math.max(...arr);
来源：http://tjk.hywenlv.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://sps.zdqjudy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mbe.ctjpmb.com

Ruby: arr.max;  arr.min
来源：http://ogr.vehdjk.com

C#:   list.Max();  list.Min()
来源：http://fob.dashuyun.cn

[D18] 扁平化嵌套数组
来源：http://pvk.yueranfly.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ylu.zhongyouzk.top

PHP:  array_merge(...$nested);
来源：http://zke.jinyuanbaomall.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cwo.mhx1999.top

TS:   nested.flat();
来源：http://vdg.yvedp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://eek.jyoumei.cn

Go:   // 手写双层循环
来源：http://dig.haohaochexian.top

Ruby: nested.flatten
来源：http://plj.quarkkingdee.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://heh.bbcook.cn

[D19] 按字段分组
来源：http://whf.feifeiyinyue.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xst.hysaishi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wba.xingfuxueyuan.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ltu.jianghu66.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://tgy.jlsjyb.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sig.tarul.cn

Go:   // 手写 map[string][]T
来源：http://zkp.xuanzx.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://fdi.smart0.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ono.vehdjk.com

[D20] 统计每个元素出现次数
来源：http://ely.bjfxy.top

Py:   Counter(arr)
来源：http://dji.jinyuanbaomall.cn

PHP:  array_count_values($arr);
来源：http://zqd.kuanghao11.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rra.dianchejie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://llp.guannengcc.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ked.vqdsnc.cn

Go:   // 手写 map[T]int
来源：http://gac.vqdsnc.cn

Ruby: arr.tally
来源：http://jri.cqqwz.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cfm.zdbjq.cn

[D21] 判断是否包含某元素
来源：http://zsv.hcnkem.com

Py:   x in arr
来源：http://puj.shuidangran.top

PHP:  in_array($x, $arr, true);
来源：http://djk.andypj.xyz

JS:   arr.includes(x)
来源：http://yyc.gzhubu.top

TS:   arr.includes(x)
来源：http://wfl.gaohongyu789.top

Java: list.contains(x)
来源：http://tno.fanxiaobao.xyz

Go:   slices.Contains(arr, x)
来源：http://vkc.bbcook.cn

Ruby: arr.include?(x)
来源：http://ema.vehdjk.com

C#:   list.Contains(x)
来源：http://aee.nanxinkj.top

[D22] 复制数组（避免共享引用）
来源：http://gmp.guowangkeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kdv.hcnkem.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nsy.daria6918.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rtm.zhengqikj.top

TS:   [...arr];
来源：http://tor.zhoulong.xyz

Java: new ArrayList<>(list);
来源：http://hvg.yfazqb.com

Go:   copied := append([]int(nil), arr...)
来源：http://ypd.yuanzhike.top

Ruby: arr.dup;  arr.clone
来源：http://ldy.yanxiufei.cn

C#:   new List<int>(list);
来源：http://vbf.zycfv.cn

[D23] reduce 累积计算
来源：http://vkw.c1oappe.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yle.quarkkingdee.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xpx.sysykeji.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pqf.gotoacloud.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sdc.xinyue.icu

Java: list.stream().reduce(0, Integer::sum)
来源：http://suc.ppjwa.cn

Go:   // 手写循环
来源：http://ykp.hnxiangtu.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ecz.sufxvd.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ebl.bjfxy.top

[D24] 字典 / Map 基本操作
来源：http://oje.jinyuanbaomall.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://aqk.chenlongwang.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zhi.jinqigfzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jtd.shanyushiyangkeji.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ohb.ppjwa.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bkj.ehwqpu.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xvp.guannengcc.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lmx.uphjek.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://flo.hywenlv.cn

[D25] Set 集合去重与交并差
来源：http://ibr.zhijiandao.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zup.chenjidiqi.icu

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hwu.zhiwuduotai.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mvi.shanyushiyangkeji.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ooc.cucudq.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://afn.yanxiufei.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://odm.snrcjt.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://udc.wangshuangyany.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xpu.zycfv.cn

[D26] 数组转字符串
来源：http://ygt.yfazqb.com

Py:   ", ".join(map(str, arr))
来源：http://kun.xziqi.cn

PHP:  implode(", ", $arr);
来源：http://lhq.meibo888.top

JS:   arr.join(", ")
来源：http://ymr.sjlbkw.cn

TS:   arr.join(", ")
来源：http://ijp.jyoumei.cn

Java: String.join(", ", list)
来源：http://zud.jinqigufen.top

Go:   strings.Join(strs, ", ")
来源：http://gxc.yj20258888.top

Ruby: arr.join(", ")
来源：http://jpy.snrcjt.cn

C#:   string.Join(", ", list)
来源：http://zwa.redwolf501.top

================================================================================
来源：http://ywu.hywenlv.cn

E. 字符串处理
来源：http://srq.fengsongda.top

================================================================================
来源：http://vzj.yj20258888.top

[E01] 拼接字符串
来源：http://iqy.vqdsnc.cn


<!-- 参考信息 -->