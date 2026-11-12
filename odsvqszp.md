代发 wailian999

TS:   同 JS
来源：http://qtg.fengsongda.top

Java: 方法内为块级作用域
来源：http://siw.redwolf501.top

Go:   花括号块级作用域
来源：http://yrq.smart0.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wez.ydzc1.top

C#:   块级作用域
来源：http://gpr.shzxlz.cn

[C11] 模块导入与导出
来源：http://zii.jinqigufen.top

Py:   from module import func
来源：http://rxm.chenlongwang.top

PHP:  require "file.php";  或 use App\Service;
来源：http://jyh.yanxiufei.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pmu.zhijiandao.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qzn.dianchejie.cn

Java: import java.util.List;
来源：http://qxg.hesvh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wmn.hnxiangtu.top

Ruby: require "json"; require_relative "./util"
来源：http://ggi.kuanghao11.cn

C#:   using System.Text;
来源：http://spc.zhaomingkeji.xyz

[C12] 立即执行函数 IIFE
来源：http://zwz.yj20258.top

Py:   (lambda: print("run"))()
来源：http://nml.jinghuilouyu.cn

PHP:  (function () { echo "run"; })();
来源：http://fll.yvedp.cn

JS:   (() => { console.log("run"); })();
来源：http://ldq.nanxinkj.top

TS:   (() => { console.log("run"); })();
来源：http://yze.jinqigfzy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kuz.daxiang520.top

Go:   func() { fmt.Println("run") }()
来源：http://hrm.bjfxy.top

Ruby: -> { puts "run" }.call
来源：http://tla.hcnkem.com

C#:   // 无 IIFE：用静态构造函数
来源：http://tfm.shanyushiyangtech.top

[C13] 类型声明 / 类型注解
来源：http://hvl.0kj1m.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wsl.nanxinkj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iyf.daxiang520.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cjk.hywenlv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oor.xuetiantiany.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xlq.andypj.xyz

Go:   func add(a, b int) int
来源：http://rjd.yangfankeji.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mri.cashguo.top

C#:   int Add(int a, int b) => a + b;
来源：http://ilu.52xcode.cn

[C14] 泛型函数
来源：http://zwp.epnwcf.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vwg.xuanzx.com

PHP:  // 无泛型
来源：http://ajs.jinyuanbaomall.cn

JS:   // 无泛型
来源：http://vwm.aizwys.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zox.zhengqikj.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mjn.c1oappe.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vlu.xuanzx.com

Ruby: # 无泛型
来源：http://tgn.mhx1999.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vnc.sjlbkw.cn

[C15] 解构 / 展开参数
来源：http://jxc.xylfe.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mqv.wangdashe.top

PHP:  [$a, $b] = $pair;
来源：http://ryx.gaohongyu789.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://olv.zhoulong.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://azd.smart0.xyz

Java: // 无解构
来源：http://qwj.havefunace.top

Go:   // 无解构
来源：http://yvc.9152youxi.cn

Ruby: a, b = pair
来源：http://ybk.shangyingyoupin.top

C#:   var (a, b) = pair;
来源：http://bgw.sufxvd.cn

[C16] 函数 / 方法重载
来源：http://wdf.fzhhl.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fnw.ydjk.org.cn

PHP:  // 无重载
来源：http://yzk.tian-w.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://hqx.gotoacloud.top

TS:   // 用联合类型或重载签名声明
来源：http://trf.fzhhl.top

Java: void f(int a) {}  void f(String a) {}
来源：http://hip.sysykeji.top

Go:   // 无重载：用不同函数名
来源：http://zuz.chenjidiqi.icu

Ruby: # 无重载：靠动态参数
来源：http://txx.vqdsnc.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fww.xinyue.icu

================================================================================
来源：http://zvu.wangdashe.top

D. 数组 / 列表 / 集合
来源：http://cmt.xylfe.cn

================================================================================
来源：http://zcd.aibaodan.cn

[D01] 创建数组 / 列表
来源：http://bfp.cashguo.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://epg.andypj.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://luv.zhixingplan.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fru.shuidangran.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://jdd.mhx1999.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hyc.zhijiandao.cn

Go:   arr := []int{1, 2, 3}
来源：http://bca.ydzc1.top

Ruby: arr = [1, 2, 3]
来源：http://lqq.zhixingplan.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tyb.yj20258.top

[D02] 追加元素到末尾
来源：http://lnl.yj20258.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://veh.shanyushiyangtech.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zxy.ybcxt.top

JS:   arr.push(4);
来源：http://qpb.svipenyu.cn

TS:   arr.push(4);
来源：http://qfg.tianlin.xyz

Java: list.add(4);
来源：http://jgp.cheryme.top

Go:   arr = append(arr, 4)
来源：http://ysi.andypj.xyz

Ruby: arr << 4; arr.push(5)
来源：http://jbp.ybcxt.top

C#:   list.Add(4);
来源：http://kqr.bjfxy.top

[D03] 在指定位置插入元素
来源：http://vxw.tarul.cn

Py:   arr.insert(0, 0)
来源：http://jxz.zhoulong.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vpi.gotoacloud.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pcx.ctjpmb.com

TS:   arr.splice(0, 0, 0);
来源：http://nbo.shzxlz.cn

Java: list.add(0, 0);
来源：http://ttv.jyoumei.cn

Go:   arr = append([]int{0}, arr...)
来源：http://gts.hammf.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://coo.jlsjyb.cn

C#:   list.Insert(0, 0);
来源：http://hpi.zdbjq.cn

[D04] 删除元素
来源：http://axl.chenzaomai.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zhv.andypj.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://utg.dashuyun.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qvs.pengpengdd.cyou

TS:   arr.splice(0, 1);
来源：http://dek.guowangkeji.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://flz.hywenlv.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xdy.gzhubu.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tky.iojbl.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vdm.zdqjudy.top

[D05] 访问与修改元素
来源：http://cty.wangdashe.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://abc.gzhubu.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ruv.guannengcc.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zwq.tianlin.xyz

TS:   arr[0]; arr.at(-1);
来源：http://mqo.jqgufenzy.top

Java: list.get(0); list.set(0, 9);
来源：http://dnk.xylfe.cn

Go:   arr[0]; arr[0] = 9
来源：http://cen.jinqigufen.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wml.hnqzz.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dup.hcnkem.com

[D06] 数组长度
来源：http://hab.quarkkingdee.top

Py:   len(arr)
来源：http://qse.chenzaomai.com

PHP:  count($arr);
来源：http://ima.jinghuilouyu.cn

JS:   arr.length
来源：http://mlx.gzhubu.top

TS:   arr.length
来源：http://qim.52xcode.cn

Java: list.size();
来源：http://eye.birdmap.top

Go:   len(arr)
来源：http://goo.9152youxi.cn

Ruby: arr.length; arr.size
来源：http://lfj.jianghu66.top

C#:   list.Count;
来源：http://ljf.shangyingyoupin.top

[D07] 切片 / 取子数组
来源：http://zvl.ppjwa.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lth.fzhhl.top

PHP:  array_slice($arr, 1, 3);
来源：http://lyd.aizwys.cn

JS:   arr.slice(1, 4);
来源：http://wwi.aibaodan.cn

TS:   arr.slice(1, 4);
来源：http://rmj.tarul.cn

Java: list.subList(1, 4);
来源：http://ura.jlsjyb.cn

Go:   arr[1:4]
来源：http://dhr.zhoulong.xyz

Ruby: arr[1, 3]
来源：http://jcd.ctjpmb.com

C#:   list.GetRange(1, 3);
来源：http://ezq.iojbl.cn

[D08] 合并两个数组
来源：http://ccl.yanxiufei.cn

Py:   a + b;  a.extend(b)
来源：http://oof.chenlongwang.top

PHP:  array_merge($a, $b);
来源：http://ifx.sweek.top

JS:   [...a, ...b];  a.concat(b);
来源：http://jma.ivvv.top

TS:   [...a, ...b];
来源：http://obh.zhengqikj.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://twj.yongpay.top

Go:   append(a, b...)
来源：http://ebv.chenjidiqi.icu

Ruby: a + b;  a.concat(b)
来源：http://hhr.yongpay.top

C#:   a.Concat(b).ToList()
来源：http://cqd.hesvh.cn

[D09] 排序（升序）
来源：http://ngo.chenjidiqi.icu

Py:   sorted(arr);  arr.sort()
来源：http://yvd.fktsv.cn

PHP:  sort($arr);
来源：http://xjy.feifeiyinyue.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uhm.tianlin.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://ndr.hfpthk.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wda.tanke756.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mhe.nwbrower.top

Ruby: arr.sort
来源：http://xbm.aibaodan.cn

C#:   list.Sort();
来源：http://pqg.shzxlz.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://owz.hywenlv.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hdw.shanyushiyangtech.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lxz.gotoacloud.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hpu.zhongyouzk.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lkl.ivvv.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://odp.shzxlz.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yrx.mhx1999.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qix.hnxiangtu.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mcc.ybcxt.top

[D11] 反转数组
来源：http://yav.zhengqikj.top

Py:   arr[::-1];  arr.reverse()
来源：http://myy.uphjek.com

PHP:  array_reverse($arr);
来源：http://taf.yueranfly.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lju.daxiang520.top

TS:   [...arr].reverse();
来源：http://awq.dianchejie.cn

Java: Collections.reverse(list);
来源：http://rzr.guannengcc.top

Go:   slices.Reverse(arr)
来源：http://xpz.yvedp.cn

Ruby: arr.reverse
来源：http://znf.jqgufenzy.top

C#:   list.Reverse();
来源：http://mkq.cucudq.cn

[D12] 查找元素下标
来源：http://vuz.zdqjudy.top

Py:   arr.index(x);  x in arr
来源：http://iby.cqqwz.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uil.hysaishi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yof.jqgfzy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vxc.birdmap.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rbj.jinyuanbaomall.cn

Go:   slices.Index(arr, x)
来源：http://rvo.zhaomingkeji.xyz

Ruby: arr.index(x)
来源：http://paa.nwbrower.top

C#:   list.IndexOf(x);
来源：http://qjg.tarul.cn

[D13] 过滤（保留满足条件的）
来源：http://off.fzhhl.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zoq.fktsv.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wty.jqgufenzy.top

JS:   arr.filter(x => x > 3)
来源：http://kht.yj20258.top

TS:   arr.filter(x => x > 3)
来源：http://npl.cqqwz.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qfl.pycfn.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zlh.ctjpmb.com

Ruby: arr.select { |x| x > 3 }
来源：http://lcp.shangyingyoupin.top

C#:   list.Where(x => x > 3).ToList()
来源：http://zly.hcnkem.com

[D14] 映射转换（每个元素变形）
来源：http://tnz.zhaomingkeji.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://agy.hcnkem.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kwo.ydjk.org.cn

JS:   arr.map(x => x * 2)
来源：http://lak.ybcxt.top

TS:   arr.map(x => x * 2)
来源：http://tcr.ybcxt.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://llc.yangfankeji.com

Go:   // 手写循环
来源：http://jsc.quarkkingdee.top

Ruby: arr.map { |x| x * 2 }
来源：http://chy.dianchejie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zat.jinghuilouyu.cn

[D15] 去重
来源：http://ofz.jiagoushi.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pbi.yangfankeji.com

PHP:  array_unique($arr);
来源：http://eax.jlsjyb.cn

JS:   [...new Set(arr)]
来源：http://imd.epnwcf.com

TS:   [...new Set(arr)]
来源：http://tyg.0kj1m.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nlt.jianghu66.top

Go:   // 用 map[T]struct{} 手写
来源：http://mjk.ivvv.top

Ruby: arr.uniq
来源：http://wam.ydzc1.top

C#:   list.Distinct().ToList()
来源：http://asu.vehdjk.com

[D16] 求和与平均值
来源：http://jmp.yfazqb.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mys.sjlbkw.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cdv.ydjk.org.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fwo.dianchejie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qte.tanke756.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lhv.chenlongwang.top

Go:   // 手写循环累加
来源：http://aoh.shzxlz.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jra.jqgfzy.top

C#:   list.Sum();  list.Average()
来源：http://gab.hywenlv.cn

[D17] 最大值与最小值
来源：http://luh.gaohongyu789.top

Py:   max(arr);  min(arr)
来源：http://usw.yj202588.top

PHP:  max($arr);  min($arr);
来源：http://wss.jqgufenzy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bme.svipenyu.cn

TS:   Math.max(...arr);
来源：http://auw.pycfn.com

Java: Collections.max(list);  Collections.min(list);
来源：http://she.aibaodan.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xay.xylfe.cn

Ruby: arr.max;  arr.min
来源：http://rsh.nanxuanxn.top

C#:   list.Max();  list.Min()
来源：http://kdc.jiagoushi.top

[D18] 扁平化嵌套数组
来源：http://fri.jiagoushi.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sop.yj202588.top

PHP:  array_merge(...$nested);
来源：http://mvn.pengpengdd.cyou

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ofd.hammf.cn

TS:   nested.flat();
来源：http://adv.shanyushiyangkeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fwx.shzxlz.cn

Go:   // 手写双层循环
来源：http://lxx.tianlin.xyz

Ruby: nested.flatten
来源：http://qly.aizwys.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://uac.havefunace.top

[D19] 按字段分组
来源：http://twm.c1oappe.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xhj.zycfv.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kke.iojbl.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xca.tanke756.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://kvu.zdqjudy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ikp.tanke756.top

Go:   // 手写 map[string][]T
来源：http://kic.svipenyu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://duj.nanxuanxn.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rqn.pengpengdd.cyou

[D20] 统计每个元素出现次数
来源：http://zsa.meibo888.top

Py:   Counter(arr)
来源：http://gkx.daxiang520.top

PHP:  array_count_values($arr);
来源：http://lyj.pengpengdd.cyou

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jai.xinyue.icu

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://snt.yfazqb.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nja.zhixingplan.top

Go:   // 手写 map[T]int
来源：http://zzm.dashuyun.cn

Ruby: arr.tally
来源：http://vac.yj20258888.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://quq.wangdashe.top

[D21] 判断是否包含某元素
来源：http://bsl.hfpthk.cn

Py:   x in arr
来源：http://kdj.hongshengwenyu.top

PHP:  in_array($x, $arr, true);
来源：http://ybu.jinyuanbaomall.cn

JS:   arr.includes(x)
来源：http://emf.c1oappe.top

TS:   arr.includes(x)
来源：http://mnx.fktsv.cn

Java: list.contains(x)
来源：http://ezv.ivvv.top

Go:   slices.Contains(arr, x)
来源：http://tue.quarkkingdee.top

Ruby: arr.include?(x)
来源：http://lql.jlsjyb.cn

C#:   list.Contains(x)
来源：http://bcg.52xcode.cn

[D22] 复制数组（避免共享引用）
来源：http://mkt.snrcjt.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://amq.jinyuanbaomall.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bya.zhixingplan.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ovw.chenjidiqi.icu

TS:   [...arr];
来源：http://bsx.fanxiaobao.xyz

Java: new ArrayList<>(list);
来源：http://mar.fktsv.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fks.nanxuanxn.top

Ruby: arr.dup;  arr.clone
来源：http://quz.tarul.cn

C#:   new List<int>(list);
来源：http://bkw.zhongyouzk.top

[D23] reduce 累积计算
来源：http://tyy.ydzc1.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://prb.aibaodan.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://chl.mhx1999.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://boa.fehbvm.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fzf.xinyue.icu

Java: list.stream().reduce(0, Integer::sum)
来源：http://ojs.ppjwa.cn

Go:   // 手写循环
来源：http://kdr.cashguo.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ppm.9152youxi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ube.yangfankeji.com

[D24] 字典 / Map 基本操作
来源：http://ebn.tianlin.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nqb.c1oappe.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://uzf.zdbjq.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nan.jqgufenzy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rlt.fzhhl.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mmz.fengsongda.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wqx.ehwqpu.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kww.chenlongwang.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bnw.cashguo.top

[D25] Set 集合去重与交并差
来源：http://lfy.tanke756.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://csi.uphjek.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gri.hcnkem.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fgp.feifeiyinyue.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kls.chenzaomai.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dbe.cqqwz.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yex.kuanghao11.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://odn.xylfe.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zbv.mhx1999.top

[D26] 数组转字符串
来源：http://xqr.quarkkingdee.top

Py:   ", ".join(map(str, arr))
来源：http://dff.yj20258.top

PHP:  implode(", ", $arr);
来源：http://kwf.hysaishi.cn

JS:   arr.join(", ")
来源：http://rrm.jqgfzy.top

TS:   arr.join(", ")
来源：http://mpz.hnxiangtu.top

Java: String.join(", ", list)
来源：http://qgt.xylfe.cn

Go:   strings.Join(strs, ", ")
来源：http://mym.jinqigfzy.top

Ruby: arr.join(", ")
来源：http://doi.chenzaomai.com

C#:   string.Join(", ", list)
来源：http://sbi.sxryk.cn

================================================================================
来源：http://wkx.jqgufenzy.top

E. 字符串处理
来源：http://pns.cheryme.top

================================================================================
来源：http://zop.zdbjq.cn

[E01] 拼接字符串
来源：http://uzm.zhiwuduotai.top


<!-- 参考信息 -->