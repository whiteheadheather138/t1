代发 wailian999

C#:   块级作用域
来源：http://uta.kuanghao11.cn

[C11] 模块导入与导出
来源：http://nkt.zhaomingkeji.xyz

Py:   from module import func
来源：http://kml.epnwcf.com

PHP:  require "file.php";  或 use App\Service;
来源：http://xjl.aibaodan.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ojy.shanyushiyangkeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://amd.ydjk.org.cn

Java: import java.util.List;
来源：http://nsc.wangshuangyany.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://soc.yongpay.top

Ruby: require "json"; require_relative "./util"
来源：http://ads.haohaochexian.top

C#:   using System.Text;
来源：http://lwy.cashguo.top

[C12] 立即执行函数 IIFE
来源：http://roa.dianchejie.cn

Py:   (lambda: print("run"))()
来源：http://ter.52xcode.cn

PHP:  (function () { echo "run"; })();
来源：http://uyg.pycfn.com

JS:   (() => { console.log("run"); })();
来源：http://bsl.vehdjk.com

TS:   (() => { console.log("run"); })();
来源：http://iqw.jinqigfzy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gqw.jqgfzy.top

Go:   func() { fmt.Println("run") }()
来源：http://otd.zdqjudy.top

Ruby: -> { puts "run" }.call
来源：http://iwp.chenjidiqi.icu

C#:   // 无 IIFE：用静态构造函数
来源：http://gie.nanxinkj.top

[C13] 类型声明 / 类型注解
来源：http://wde.jinqigfzy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cji.jyoumei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://int.zhixingplan.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hju.jiagoushi.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gri.zhixingplan.top

Java: int add(int a, int b) { return a + b; }
来源：http://bex.yj202588.top

Go:   func add(a, b int) int
来源：http://hbv.tianlin.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vea.gzhubu.top

C#:   int Add(int a, int b) => a + b;
来源：http://mlc.zhaomingkeji.xyz

[C14] 泛型函数
来源：http://nmm.aizwys.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wbl.snrcjt.cn

PHP:  // 无泛型
来源：http://qsu.wangshuangyany.cn

JS:   // 无泛型
来源：http://poe.aizwys.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tuj.ivvv.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qwn.haohaochexian.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rqn.jyoumei.cn

Ruby: # 无泛型
来源：http://vzz.guannengcc.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fcb.xylfe.cn

[C15] 解构 / 展开参数
来源：http://fly.sxryk.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bjd.shuidangran.top

PHP:  [$a, $b] = $pair;
来源：http://bcw.pengpengdd.cyou

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://eok.zhengqikj.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zgp.iojbl.cn

Java: // 无解构
来源：http://sni.fanxiaobao.xyz

Go:   // 无解构
来源：http://ysr.gzhubu.top

Ruby: a, b = pair
来源：http://lks.yuanzhike.top

C#:   var (a, b) = pair;
来源：http://uys.jinghuilouyu.cn

[C16] 函数 / 方法重载
来源：http://bkz.zhaomingkeji.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tck.daxiang520.top

PHP:  // 无重载
来源：http://whf.gaohongyu789.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://lbe.tanke756.top

TS:   // 用联合类型或重载签名声明
来源：http://xip.fktsv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://uab.shangyingyoupin.top

Go:   // 无重载：用不同函数名
来源：http://bif.vqdsnc.cn

Ruby: # 无重载：靠动态参数
来源：http://qfz.ehwqpu.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://sjm.yangfankeji.com

================================================================================
来源：http://ltw.yonumen.top

D. 数组 / 列表 / 集合
来源：http://wvn.9152youxi.cn

================================================================================
来源：http://lwi.yuxming.cn

[D01] 创建数组 / 列表
来源：http://swo.daria6918.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xcb.zhengqikj.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qsq.tarul.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ecw.feifeiyinyue.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ahf.jlsjyb.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vcl.snrcjt.cn

Go:   arr := []int{1, 2, 3}
来源：http://iuo.gogol.net.cn

Ruby: arr = [1, 2, 3]
来源：http://spu.daxiang520.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xue.zdqjudy.top

[D02] 追加元素到末尾
来源：http://vya.ydjk.org.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bek.smart0.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bbh.andypj.xyz

JS:   arr.push(4);
来源：http://wqp.shzxlz.cn

TS:   arr.push(4);
来源：http://yed.zhixingplan.top

Java: list.add(4);
来源：http://miq.iojbl.cn

Go:   arr = append(arr, 4)
来源：http://gro.tian-w.cn

Ruby: arr << 4; arr.push(5)
来源：http://nwp.ywan-chungtsiang.top

C#:   list.Add(4);
来源：http://vdq.tian-w.cn

[D03] 在指定位置插入元素
来源：http://jju.meibo888.top

Py:   arr.insert(0, 0)
来源：http://wyz.9152youxi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jao.chenjidiqi.icu

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vlo.jinqigufen.top

TS:   arr.splice(0, 0, 0);
来源：http://fdw.gaohongyu789.top

Java: list.add(0, 0);
来源：http://otr.aizwys.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mnd.snrcjt.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uzd.nwbrower.top

C#:   list.Insert(0, 0);
来源：http://fib.birdmap.top

[D04] 删除元素
来源：http://ejb.aizwys.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fzh.ppjwa.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://msq.ctjpmb.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xon.ydzc1.top

TS:   arr.splice(0, 1);
来源：http://gpg.nanxuanxn.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://flg.birdmap.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://igh.yanxiufei.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bnz.aibaodan.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lng.pengpengdd.cyou

[D05] 访问与修改元素
来源：http://ypw.daria6918.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zai.fehbvm.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bot.tianlin.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://duz.zhaomingkeji.xyz

TS:   arr[0]; arr.at(-1);
来源：http://cfh.zhaomingkeji.xyz

Java: list.get(0); list.set(0, 9);
来源：http://jrf.daria6918.cn

Go:   arr[0]; arr[0] = 9
来源：http://lne.shanyushiyangtech.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xke.shuidangran.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://laj.sufxvd.cn

[D06] 数组长度
来源：http://zbh.tianlin.xyz

Py:   len(arr)
来源：http://spy.ybcxt.top

PHP:  count($arr);
来源：http://fcw.snrcjt.cn

JS:   arr.length
来源：http://gcf.shanyushiyangkeji.top

TS:   arr.length
来源：http://dhe.dashuyun.cn

Java: list.size();
来源：http://fxv.sxryk.cn

Go:   len(arr)
来源：http://cwf.xuanzx.com

Ruby: arr.length; arr.size
来源：http://lmt.yj20258.top

C#:   list.Count;
来源：http://qbw.fktsv.cn

[D07] 切片 / 取子数组
来源：http://crz.yvedp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vzd.zhiwuduotai.top

PHP:  array_slice($arr, 1, 3);
来源：http://hed.hongshengwenyu.top

JS:   arr.slice(1, 4);
来源：http://hnv.hammf.cn

TS:   arr.slice(1, 4);
来源：http://jgi.meibo888.top

Java: list.subList(1, 4);
来源：http://coh.yonumen.top

Go:   arr[1:4]
来源：http://oka.bjfxy.top

Ruby: arr[1, 3]
来源：http://iem.quarkkingdee.top

C#:   list.GetRange(1, 3);
来源：http://bwr.cashguo.top

[D08] 合并两个数组
来源：http://hxn.dashuyun.cn

Py:   a + b;  a.extend(b)
来源：http://bem.316326.xyz

PHP:  array_merge($a, $b);
来源：http://luw.feifeiyinyue.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wfx.dashuyun.cn

TS:   [...a, ...b];
来源：http://mgt.jiagoushi.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mbm.fktsv.cn

Go:   append(a, b...)
来源：http://jhe.andypj.xyz

Ruby: a + b;  a.concat(b)
来源：http://wdo.zycfv.cn

C#:   a.Concat(b).ToList()
来源：http://qjs.shuidangran.top

[D09] 排序（升序）
来源：http://zvr.hesvh.cn

Py:   sorted(arr);  arr.sort()
来源：http://mcx.9152youxi.cn

PHP:  sort($arr);
来源：http://mux.xinyue.icu

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ifp.yuxming.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hzw.yonumen.top

Java: Collections.sort(list);  list.sort(null);
来源：http://uph.fengsongda.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://piu.jiagoushi.top

Ruby: arr.sort
来源：http://zan.shuidangran.top

C#:   list.Sort();
来源：http://bvo.shangyingyoupin.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ntp.zdbjq.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rkr.fehbvm.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uui.snrcjt.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sne.yongpay.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://woo.ehwqpu.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sdr.nanxinkj.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dll.hesvh.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wob.zhixingplan.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nor.vehdjk.com

[D11] 反转数组
来源：http://zko.yj202588.top

Py:   arr[::-1];  arr.reverse()
来源：http://uuh.hnxiangtu.top

PHP:  array_reverse($arr);
来源：http://alq.jinyuanbaomall.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yuj.jinyuanbaomall.cn

TS:   [...arr].reverse();
来源：http://tdg.316326.xyz

Java: Collections.reverse(list);
来源：http://pbp.cucudq.cn

Go:   slices.Reverse(arr)
来源：http://bng.snrcjt.cn

Ruby: arr.reverse
来源：http://dak.wangshuangyany.cn

C#:   list.Reverse();
来源：http://opl.sjlbkw.cn

[D12] 查找元素下标
来源：http://yhz.yueranfly.top

Py:   arr.index(x);  x in arr
来源：http://rir.sxryk.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rej.gogol.net.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mgv.yuxming.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pty.pycfn.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dze.uphjek.com

Go:   slices.Index(arr, x)
来源：http://owd.tanke756.top

Ruby: arr.index(x)
来源：http://csd.redwolf501.top

C#:   list.IndexOf(x);
来源：http://sfr.sufxvd.cn

[D13] 过滤（保留满足条件的）
来源：http://iop.aizwys.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qwe.hfpthk.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fjy.ehwqpu.com

JS:   arr.filter(x => x > 3)
来源：http://cyk.dianchejie.cn

TS:   arr.filter(x => x > 3)
来源：http://nom.fehbvm.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fcm.yj20258888.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dyi.jinqigfzy.top

Ruby: arr.select { |x| x > 3 }
来源：http://som.zdbjq.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://cec.ehwqpu.com

[D14] 映射转换（每个元素变形）
来源：http://qxl.yj20258888.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cle.jqgufenzy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lsg.cheryme.top

JS:   arr.map(x => x * 2)
来源：http://yhy.sweek.top

TS:   arr.map(x => x * 2)
来源：http://vhc.yonumen.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://cfg.zycfv.cn

Go:   // 手写循环
来源：http://wyd.yj20258.top

Ruby: arr.map { |x| x * 2 }
来源：http://nrm.shangyingyoupin.top

C#:   list.Select(x => x * 2).ToList()
来源：http://wgh.tarul.cn

[D15] 去重
来源：http://nba.gotoacloud.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dnp.jianghu66.top

PHP:  array_unique($arr);
来源：http://zal.gotoacloud.top

JS:   [...new Set(arr)]
来源：http://eoc.aibaodan.cn

TS:   [...new Set(arr)]
来源：http://yrh.yj20258888.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hvd.hammf.cn

Go:   // 用 map[T]struct{} 手写
来源：http://prz.tianlin.xyz

Ruby: arr.uniq
来源：http://udz.hnxiangtu.top

C#:   list.Distinct().ToList()
来源：http://pdd.fanxiaobao.xyz

[D16] 求和与平均值
来源：http://wcf.daria6918.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ruc.xziqi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nxs.jinqigufen.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ilk.hywenlv.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pwa.birdmap.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kbb.gaohongyu789.top

Go:   // 手写循环累加
来源：http://hct.hcnkem.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xoz.nanxinkj.top

C#:   list.Sum();  list.Average()
来源：http://fxx.sweek.top

[D17] 最大值与最小值
来源：http://mve.vehdjk.com

Py:   max(arr);  min(arr)
来源：http://mjf.yueranfly.top

PHP:  max($arr);  min($arr);
来源：http://nlx.pycfn.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://epw.uphjek.com

TS:   Math.max(...arr);
来源：http://exx.nanxuanxn.top

Java: Collections.max(list);  Collections.min(list);
来源：http://jcc.snrcjt.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dce.fanxiaobao.xyz

Ruby: arr.max;  arr.min
来源：http://bca.xuetiantiany.cn

C#:   list.Max();  list.Min()
来源：http://nrx.hcnkem.com

[D18] 扁平化嵌套数组
来源：http://nno.birdmap.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rwc.nanxuanxn.top

PHP:  array_merge(...$nested);
来源：http://uwd.zhaomingkeji.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yhu.xinyue.icu

TS:   nested.flat();
来源：http://fdk.pycfn.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ojt.quarkkingdee.top

Go:   // 手写双层循环
来源：http://ilb.zdqjudy.top

Ruby: nested.flatten
来源：http://cns.zhoulong.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://mdy.fktsv.cn

[D19] 按字段分组
来源：http://jaj.tarul.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xsj.havefunace.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://oel.nwbrower.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jia.cqqwz.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://sml.chenzaomai.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jvq.9152youxi.cn

Go:   // 手写 map[string][]T
来源：http://mbt.dianchejie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rls.cucudq.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yhi.vqdsnc.cn

[D20] 统计每个元素出现次数
来源：http://svj.uphjek.com

Py:   Counter(arr)
来源：http://qbm.uphjek.com

PHP:  array_count_values($arr);
来源：http://vdg.yangfankeji.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gwg.birdmap.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://olu.shanyushiyangtech.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jge.cheryme.top

Go:   // 手写 map[T]int
来源：http://pvs.dashuyun.cn

Ruby: arr.tally
来源：http://yyt.hfpthk.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mmx.yangfankeji.com

[D21] 判断是否包含某元素
来源：http://kyy.nanxinkj.top

Py:   x in arr
来源：http://mct.hysaishi.cn

PHP:  in_array($x, $arr, true);
来源：http://yck.aibaodan.cn

JS:   arr.includes(x)
来源：http://emm.smart0.xyz

TS:   arr.includes(x)
来源：http://oda.chenzaomai.com

Java: list.contains(x)
来源：http://gdj.0kj1m.cn

Go:   slices.Contains(arr, x)
来源：http://svo.yanxiufei.cn

Ruby: arr.include?(x)
来源：http://rft.andypj.xyz

C#:   list.Contains(x)
来源：http://ipm.9152youxi.cn

[D22] 复制数组（避免共享引用）
来源：http://mon.bjfxy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://isc.pycfn.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://iet.jlsjyb.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://aoj.jiagoushi.top

TS:   [...arr];
来源：http://mhf.chenzaomai.com

Java: new ArrayList<>(list);
来源：http://yww.jinghuilouyu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://hwp.sysykeji.top

Ruby: arr.dup;  arr.clone
来源：http://rsu.zhengqikj.top

C#:   new List<int>(list);
来源：http://mkm.snrcjt.cn

[D23] reduce 累积计算
来源：http://ngx.xingfuxueyuan.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ajo.xingfuxueyuan.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fvd.xingfuxueyuan.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tzs.meibo888.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://syx.hysaishi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://heh.yvedp.cn

Go:   // 手写循环
来源：http://vea.cdnleiting.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hjm.yongpay.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kgu.iojbl.cn

[D24] 字典 / Map 基本操作
来源：http://bcz.bjfxy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://aos.zhixingplan.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fow.hfpthk.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dyv.hnxiangtu.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vtv.shangyingyoupin.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fzm.epnwcf.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uaj.tianlin.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://eyp.fzhhl.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mqj.hongshengwenyu.top

[D25] Set 集合去重与交并差
来源：http://xxp.xuanzx.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bfd.snrcjt.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://frs.cqqwz.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pbi.nanxinkj.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fsa.zhongyouzk.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://efh.gzhubu.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pzx.ppjwa.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wgq.yueranfly.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dbs.cashguo.top

[D26] 数组转字符串
来源：http://azw.daria6918.cn

Py:   ", ".join(map(str, arr))
来源：http://xja.vqdsnc.cn

PHP:  implode(", ", $arr);
来源：http://keo.fanxiaobao.xyz

JS:   arr.join(", ")
来源：http://wmm.jianghu66.top

TS:   arr.join(", ")
来源：http://kvq.uphjek.com

Java: String.join(", ", list)
来源：http://txa.gaohongyu789.top

Go:   strings.Join(strs, ", ")
来源：http://zea.svipenyu.cn

Ruby: arr.join(", ")
来源：http://vkm.nwbrower.top

C#:   string.Join(", ", list)
来源：http://tma.cqqwz.cn

================================================================================
来源：http://sqn.hammf.cn

E. 字符串处理
来源：http://uxt.feifeiyinyue.top

================================================================================
来源：http://flj.yj20258.top

[E01] 拼接字符串
来源：http://bhp.jiagoushi.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wjd.yj20258888.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://byl.jinghuilouyu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pck.yj20258.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yza.shanyushiyangkeji.top


<!-- 参考信息 -->