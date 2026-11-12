代发 wailian999

C#:   块级作用域
来源：http://nex.birdmap.top

[C11] 模块导入与导出
来源：http://mdc.zhoulong.xyz

Py:   from module import func
来源：http://ssa.hnxiangtu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://bxg.yueranfly.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://mxm.yvedp.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mwt.yj202588.top

Java: import java.util.List;
来源：http://eym.zycfv.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hgd.zhijiandao.cn

Ruby: require "json"; require_relative "./util"
来源：http://han.shangyingyoupin.top

C#:   using System.Text;
来源：http://wbm.ctjpmb.com

[C12] 立即执行函数 IIFE
来源：http://zug.gaohongyu789.top

Py:   (lambda: print("run"))()
来源：http://dnw.jianghu66.top

PHP:  (function () { echo "run"; })();
来源：http://wjs.pengpengdd.cyou

JS:   (() => { console.log("run"); })();
来源：http://mcb.iojbl.cn

TS:   (() => { console.log("run"); })();
来源：http://qdi.shanyushiyangkeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lky.daria6918.cn

Go:   func() { fmt.Println("run") }()
来源：http://oft.0kj1m.cn

Ruby: -> { puts "run" }.call
来源：http://oor.bbcook.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://aur.havefunace.top

[C13] 类型声明 / 类型注解
来源：http://yuu.jinghuilouyu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rcd.yuxming.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://die.fehbvm.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hnz.fehbvm.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xci.zhongyouzk.top

Java: int add(int a, int b) { return a + b; }
来源：http://koc.gogol.net.cn

Go:   func add(a, b int) int
来源：http://zpr.yvedp.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ehz.ydjk.org.cn

C#:   int Add(int a, int b) => a + b;
来源：http://zyu.chenlongwang.top

[C14] 泛型函数
来源：http://gkp.gzhubu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ddy.sxryk.cn

PHP:  // 无泛型
来源：http://onn.ydjk.org.cn

JS:   // 无泛型
来源：http://ghm.birdmap.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uta.fengsongda.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://epd.uphjek.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ceq.ivvv.top

Ruby: # 无泛型
来源：http://ybh.hywenlv.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bdg.fanxiaobao.xyz

[C15] 解构 / 展开参数
来源：http://ium.jqgfzy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://paa.xylfe.cn

PHP:  [$a, $b] = $pair;
来源：http://jip.daria6918.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://toh.nanxuanxn.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gqr.hnxiangtu.top

Java: // 无解构
来源：http://rhr.gzhubu.top

Go:   // 无解构
来源：http://nab.xylfe.cn

Ruby: a, b = pair
来源：http://oor.ivvv.top

C#:   var (a, b) = pair;
来源：http://cbp.xylfe.cn

[C16] 函数 / 方法重载
来源：http://gme.jinyuanbaomall.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ksg.yonumen.top

PHP:  // 无重载
来源：http://jnl.jinyuanbaomall.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xip.xingfuxueyuan.xyz

TS:   // 用联合类型或重载签名声明
来源：http://jbf.yangfankeji.com

Java: void f(int a) {}  void f(String a) {}
来源：http://czh.aizwys.cn

Go:   // 无重载：用不同函数名
来源：http://skb.quarkkingdee.top

Ruby: # 无重载：靠动态参数
来源：http://ikr.hammf.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://bjc.9152youxi.cn

================================================================================
来源：http://vwb.zhoulong.xyz

D. 数组 / 列表 / 集合
来源：http://ktf.zhongyouzk.top

================================================================================
来源：http://fpp.zhiwuduotai.top

[D01] 创建数组 / 列表
来源：http://ywo.zycfv.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://tfl.zhoulong.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dwc.cucudq.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hmn.zhongyouzk.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://avb.pycfn.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pch.shuidangran.top

Go:   arr := []int{1, 2, 3}
来源：http://qdg.52xcode.cn

Ruby: arr = [1, 2, 3]
来源：http://dkh.nwbrower.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://crp.feifeiyinyue.top

[D02] 追加元素到末尾
来源：http://ilq.zdqjudy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://whz.gzhubu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hzz.yj202588.top

JS:   arr.push(4);
来源：http://bkr.epnwcf.com

TS:   arr.push(4);
来源：http://qiz.zhixingplan.top

Java: list.add(4);
来源：http://ysg.hnxiangtu.top

Go:   arr = append(arr, 4)
来源：http://bvu.vehdjk.com

Ruby: arr << 4; arr.push(5)
来源：http://dnq.jqgufenzy.top

C#:   list.Add(4);
来源：http://unm.jinqigufen.top

[D03] 在指定位置插入元素
来源：http://zbp.pengpengdd.cyou

Py:   arr.insert(0, 0)
来源：http://irg.shuidangran.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pck.yj20258.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://amh.tanke756.top

TS:   arr.splice(0, 0, 0);
来源：http://yul.cashguo.top

Java: list.add(0, 0);
来源：http://xcy.hywenlv.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hqk.cdnleiting.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://egl.zycfv.cn

C#:   list.Insert(0, 0);
来源：http://nls.hfpthk.cn

[D04] 删除元素
来源：http://qsj.zhiwuduotai.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lja.c1oappe.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tej.xylfe.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xcj.yvedp.cn

TS:   arr.splice(0, 1);
来源：http://mhk.jqgufenzy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rsx.sxryk.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vfn.yanxiufei.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rid.zhixingplan.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fxf.zhiwuduotai.top

[D05] 访问与修改元素
来源：http://msz.yonumen.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xgc.aizwys.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gfs.fehbvm.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://isd.epnwcf.com

TS:   arr[0]; arr.at(-1);
来源：http://jky.yj20258888.top

Java: list.get(0); list.set(0, 9);
来源：http://wcl.jinqigfzy.top

Go:   arr[0]; arr[0] = 9
来源：http://fec.zhoulong.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lrc.yangfankeji.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qhf.jinghuilouyu.cn

[D06] 数组长度
来源：http://zmx.fanxiaobao.xyz

Py:   len(arr)
来源：http://wif.yfazqb.com

PHP:  count($arr);
来源：http://hjd.shanyushiyangkeji.top

JS:   arr.length
来源：http://qfz.yanxiufei.cn

TS:   arr.length
来源：http://mzk.vehdjk.com

Java: list.size();
来源：http://frj.yueranfly.top

Go:   len(arr)
来源：http://vvy.yongpay.top

Ruby: arr.length; arr.size
来源：http://yxj.ehwqpu.com

C#:   list.Count;
来源：http://fdg.mhx1999.top

[D07] 切片 / 取子数组
来源：http://liq.hesvh.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kxl.guowangkeji.top

PHP:  array_slice($arr, 1, 3);
来源：http://jxw.birdmap.top

JS:   arr.slice(1, 4);
来源：http://uyt.tian-w.cn

TS:   arr.slice(1, 4);
来源：http://fgt.nanxinkj.top

Java: list.subList(1, 4);
来源：http://jsf.hammf.cn

Go:   arr[1:4]
来源：http://srl.chenjidiqi.icu

Ruby: arr[1, 3]
来源：http://tcv.guowangkeji.top

C#:   list.GetRange(1, 3);
来源：http://rgz.zdqjudy.top

[D08] 合并两个数组
来源：http://cel.redwolf501.top

Py:   a + b;  a.extend(b)
来源：http://ndr.cqqwz.cn

PHP:  array_merge($a, $b);
来源：http://tbi.gogol.net.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ufk.zdbjq.cn

TS:   [...a, ...b];
来源：http://bji.9152youxi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tqm.yanxiufei.cn

Go:   append(a, b...)
来源：http://ycv.xuetiantiany.cn

Ruby: a + b;  a.concat(b)
来源：http://cak.tarul.cn

C#:   a.Concat(b).ToList()
来源：http://bto.daxiang520.top

[D09] 排序（升序）
来源：http://wkd.jqgfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://fve.jyoumei.cn

PHP:  sort($arr);
来源：http://vut.cucudq.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://thk.yuxming.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://vst.jinqigufen.top

Java: Collections.sort(list);  list.sort(null);
来源：http://xtv.daria6918.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ttt.hammf.cn

Ruby: arr.sort
来源：http://zey.bjfxy.top

C#:   list.Sort();
来源：http://cjs.xylfe.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://cpx.cqqwz.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://exp.hnqzz.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pyn.feifeiyinyue.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ody.haohaochexian.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ugf.xinyue.icu

Java: list.sort(Comparator.comparing(Person::age));
来源：http://srh.zhoulong.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://run.yangfankeji.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://aio.bbcook.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dun.xylfe.cn

[D11] 反转数组
来源：http://com.fehbvm.com

Py:   arr[::-1];  arr.reverse()
来源：http://oqm.birdmap.top

PHP:  array_reverse($arr);
来源：http://umf.yanxiufei.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kbm.jqgfzy.top

TS:   [...arr].reverse();
来源：http://zzb.shanyushiyangtech.top

Java: Collections.reverse(list);
来源：http://qri.svipenyu.cn

Go:   slices.Reverse(arr)
来源：http://geh.chenzaomai.com

Ruby: arr.reverse
来源：http://bjt.xuetiantiany.cn

C#:   list.Reverse();
来源：http://dxd.xingfuxueyuan.xyz

[D12] 查找元素下标
来源：http://igg.fanxiaobao.xyz

Py:   arr.index(x);  x in arr
来源：http://zhb.fzhhl.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://twa.fzhhl.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rlg.yj202588.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://buq.xinyue.icu

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kur.jinghuilouyu.cn

Go:   slices.Index(arr, x)
来源：http://njy.hfpthk.cn

Ruby: arr.index(x)
来源：http://rhs.feifeiyinyue.top

C#:   list.IndexOf(x);
来源：http://zjy.smart0.xyz

[D13] 过滤（保留满足条件的）
来源：http://mbb.hesvh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://avq.zycfv.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://smg.cdnleiting.top

JS:   arr.filter(x => x > 3)
来源：http://nuf.fktsv.cn

TS:   arr.filter(x => x > 3)
来源：http://lci.sxryk.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://iwl.hfpthk.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jlk.guannengcc.top

Ruby: arr.select { |x| x > 3 }
来源：http://zez.aibaodan.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://rrr.fzhhl.top

[D14] 映射转换（每个元素变形）
来源：http://mtf.jianghu66.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kug.xuetiantiany.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ien.havefunace.top

JS:   arr.map(x => x * 2)
来源：http://ysi.hesvh.cn

TS:   arr.map(x => x * 2)
来源：http://cwj.jqgfzy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ljp.sysykeji.top

Go:   // 手写循环
来源：http://gkt.yuxming.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jrf.jianghu66.top

C#:   list.Select(x => x * 2).ToList()
来源：http://znm.hammf.cn

[D15] 去重
来源：http://wks.xingfuxueyuan.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://uhp.hongshengwenyu.top

PHP:  array_unique($arr);
来源：http://nwx.c1oappe.top

JS:   [...new Set(arr)]
来源：http://xts.yonumen.top

TS:   [...new Set(arr)]
来源：http://acz.nanxuanxn.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bcc.fehbvm.com

Go:   // 用 map[T]struct{} 手写
来源：http://jrr.gotoacloud.top

Ruby: arr.uniq
来源：http://vcb.jiagoushi.top

C#:   list.Distinct().ToList()
来源：http://mjo.vqdsnc.cn

[D16] 求和与平均值
来源：http://tkw.hcnkem.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gwo.shanyushiyangkeji.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lnv.ywan-chungtsiang.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wsh.epnwcf.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lcq.zhiwuduotai.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xhj.kuanghao11.cn

Go:   // 手写循环累加
来源：http://ccp.havefunace.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ean.shzxlz.cn

C#:   list.Sum();  list.Average()
来源：http://yhc.chenlongwang.top

[D17] 最大值与最小值
来源：http://fef.daxiang520.top

Py:   max(arr);  min(arr)
来源：http://ngb.chenzaomai.com

PHP:  max($arr);  min($arr);
来源：http://sbq.fengsongda.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qyp.hnqzz.top

TS:   Math.max(...arr);
来源：http://umz.yuanzhike.top

Java: Collections.max(list);  Collections.min(list);
来源：http://cgc.hnqzz.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://uxs.smart0.xyz

Ruby: arr.max;  arr.min
来源：http://paa.cucudq.cn

C#:   list.Max();  list.Min()
来源：http://qum.bjfxy.top

[D18] 扁平化嵌套数组
来源：http://cei.wangshuangyany.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cqh.dashuyun.cn

PHP:  array_merge(...$nested);
来源：http://dzo.jyoumei.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://olm.shangyingyoupin.top

TS:   nested.flat();
来源：http://ggu.zhixingplan.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ssa.zdqjudy.top

Go:   // 手写双层循环
来源：http://mxo.shangyingyoupin.top

Ruby: nested.flatten
来源：http://fkg.hongshengwenyu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://bun.jqgfzy.top

[D19] 按字段分组
来源：http://uue.cucudq.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gzi.sysykeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mmn.ivvv.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mqt.mhx1999.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://aug.wangshuangyany.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pmp.dashuyun.cn

Go:   // 手写 map[string][]T
来源：http://asp.jianghu66.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ntt.uphjek.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dtx.fzhhl.top

[D20] 统计每个元素出现次数
来源：http://duw.zdbjq.cn

Py:   Counter(arr)
来源：http://gdv.meibo888.top

PHP:  array_count_values($arr);
来源：http://ume.pycfn.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hyt.cucudq.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dab.yuxming.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tpk.hnxiangtu.top

Go:   // 手写 map[T]int
来源：http://qjy.hywenlv.cn

Ruby: arr.tally
来源：http://ung.zhongyouzk.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ayn.316326.xyz

[D21] 判断是否包含某元素
来源：http://ggo.yj20258.top

Py:   x in arr
来源：http://otj.c1oappe.top

PHP:  in_array($x, $arr, true);
来源：http://jsi.bjfxy.top

JS:   arr.includes(x)
来源：http://hvl.jinyuanbaomall.cn

TS:   arr.includes(x)
来源：http://ihx.zhongyouzk.top

Java: list.contains(x)
来源：http://quq.nanxinkj.top

Go:   slices.Contains(arr, x)
来源：http://huo.jinqigufen.top

Ruby: arr.include?(x)
来源：http://izl.yvedp.cn

C#:   list.Contains(x)
来源：http://lby.haohaochexian.top

[D22] 复制数组（避免共享引用）
来源：http://hhp.tianlin.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://eck.zhongyouzk.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dyt.shanyushiyangkeji.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zwr.xinyue.icu

TS:   [...arr];
来源：http://czn.52xcode.cn

Java: new ArrayList<>(list);
来源：http://iok.hongshengwenyu.top

Go:   copied := append([]int(nil), arr...)
来源：http://ttt.kuanghao11.cn

Ruby: arr.dup;  arr.clone
来源：http://wuk.shangyingyoupin.top

C#:   new List<int>(list);
来源：http://hxw.fzhhl.top

[D23] reduce 累积计算
来源：http://oms.vehdjk.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://brh.hfpthk.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://eia.sweek.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jxl.bbcook.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lzd.yj20258888.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://byt.tanke756.top

Go:   // 手写循环
来源：http://aun.shangyingyoupin.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jrl.yueranfly.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xqh.ydzc1.top

[D24] 字典 / Map 基本操作
来源：http://neh.guannengcc.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hhn.ppjwa.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ldk.nwbrower.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hcu.daria6918.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qmp.ydjk.org.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cif.svipenyu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zaw.cashguo.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wde.aizwys.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ywl.wangdashe.top

[D25] Set 集合去重与交并差
来源：http://weh.zycfv.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vpx.yongpay.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hqq.hammf.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ioj.hongshengwenyu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ptn.hongshengwenyu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kix.tanke756.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dkv.ydzc1.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jbs.cdnleiting.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wke.hfpthk.cn

[D26] 数组转字符串
来源：http://rhm.jlsjyb.cn

Py:   ", ".join(map(str, arr))
来源：http://hzo.yongpay.top

PHP:  implode(", ", $arr);
来源：http://fxq.ybcxt.top

JS:   arr.join(", ")
来源：http://ysa.nanxuanxn.top

TS:   arr.join(", ")
来源：http://fln.cdnleiting.top

Java: String.join(", ", list)
来源：http://pia.yangfankeji.com

Go:   strings.Join(strs, ", ")
来源：http://rkg.cashguo.top

Ruby: arr.join(", ")
来源：http://yxy.zhongyouzk.top

C#:   string.Join(", ", list)
来源：http://oqm.jinyuanbaomall.cn

================================================================================
来源：http://hja.hywenlv.cn

E. 字符串处理
来源：http://opc.aibaodan.cn

================================================================================
来源：http://nde.svipenyu.cn

[E01] 拼接字符串
来源：http://fep.guowangkeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hno.fzhhl.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lda.hnxiangtu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zon.ppjwa.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ybr.316326.xyz


<!-- 参考信息 -->