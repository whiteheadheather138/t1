代发 wailian999

[C10] 变量作用域
来源：http://btc.zhiwuduotai.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://eoa.yvedp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yct.tarul.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tlc.aizwys.cn

TS:   同 JS
来源：http://vwl.kuanghao11.cn

Java: 方法内为块级作用域
来源：http://gem.hesvh.cn

Go:   花括号块级作用域
来源：http://dxh.yj202588.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uis.xuanzx.com

C#:   块级作用域
来源：http://fll.mhx1999.top

[C11] 模块导入与导出
来源：http://kdk.yuxming.cn

Py:   from module import func
来源：http://rni.316326.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://vsg.gotoacloud.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://yan.jqgfzy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://awp.jyoumei.cn

Java: import java.util.List;
来源：http://vae.shzxlz.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://puz.9152youxi.cn

Ruby: require "json"; require_relative "./util"
来源：http://yrh.yangfankeji.com

C#:   using System.Text;
来源：http://yrs.feifeiyinyue.top

[C12] 立即执行函数 IIFE
来源：http://tso.zycfv.cn

Py:   (lambda: print("run"))()
来源：http://rak.gaohongyu789.top

PHP:  (function () { echo "run"; })();
来源：http://feo.pycfn.com

JS:   (() => { console.log("run"); })();
来源：http://loc.zhongyouzk.top

TS:   (() => { console.log("run"); })();
来源：http://uhq.hnxiangtu.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ltu.fengsongda.top

Go:   func() { fmt.Println("run") }()
来源：http://gmx.ybcxt.top

Ruby: -> { puts "run" }.call
来源：http://dqq.smart0.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://zlg.nwbrower.top

[C13] 类型声明 / 类型注解
来源：http://lje.bjfxy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://uzv.tianlin.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rxd.vehdjk.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://heq.hcnkem.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xuh.shangyingyoupin.top

Java: int add(int a, int b) { return a + b; }
来源：http://fvh.jlsjyb.cn

Go:   func add(a, b int) int
来源：http://hfi.ybcxt.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fis.sufxvd.cn

C#:   int Add(int a, int b) => a + b;
来源：http://lci.haohaochexian.top

[C14] 泛型函数
来源：http://gqy.meibo888.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zjv.yj20258888.top

PHP:  // 无泛型
来源：http://jfy.zycfv.cn

JS:   // 无泛型
来源：http://wwv.sxryk.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://glo.chenzaomai.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://flh.zycfv.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tic.zhoulong.xyz

Ruby: # 无泛型
来源：http://upf.0kj1m.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ecg.wangdashe.top

[C15] 解构 / 展开参数
来源：http://kif.tianlin.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lte.fengsongda.top

PHP:  [$a, $b] = $pair;
来源：http://dgy.meibo888.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uih.haohaochexian.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fwz.fzhhl.top

Java: // 无解构
来源：http://cen.ivvv.top

Go:   // 无解构
来源：http://cby.jinqigfzy.top

Ruby: a, b = pair
来源：http://qwh.dianchejie.cn

C#:   var (a, b) = pair;
来源：http://shy.xziqi.cn

[C16] 函数 / 方法重载
来源：http://wbf.yueranfly.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://phm.hnxiangtu.top

PHP:  // 无重载
来源：http://rwb.redwolf501.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://jwm.cdnleiting.top

TS:   // 用联合类型或重载签名声明
来源：http://bvd.gaohongyu789.top

Java: void f(int a) {}  void f(String a) {}
来源：http://mut.feifeiyinyue.top

Go:   // 无重载：用不同函数名
来源：http://arl.shanyushiyangtech.top

Ruby: # 无重载：靠动态参数
来源：http://aio.52xcode.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ekn.jiagoushi.top

================================================================================
来源：http://ecq.sxryk.cn

D. 数组 / 列表 / 集合
来源：http://fqg.hywenlv.cn

================================================================================
来源：http://grl.aizwys.cn

[D01] 创建数组 / 列表
来源：http://vpu.fzhhl.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://wff.zycfv.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xlg.hnxiangtu.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pbs.daria6918.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://oqo.yuanzhike.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://las.dashuyun.cn

Go:   arr := []int{1, 2, 3}
来源：http://vhw.hywenlv.cn

Ruby: arr = [1, 2, 3]
来源：http://ovt.ywan-chungtsiang.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hag.mhx1999.top

[D02] 追加元素到末尾
来源：http://iuu.cashguo.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pcd.gotoacloud.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ati.gzhubu.top

JS:   arr.push(4);
来源：http://vhk.fzhhl.top

TS:   arr.push(4);
来源：http://qco.zdbjq.cn

Java: list.add(4);
来源：http://nvc.svipenyu.cn

Go:   arr = append(arr, 4)
来源：http://cwo.zhijiandao.cn

Ruby: arr << 4; arr.push(5)
来源：http://spo.gaohongyu789.top

C#:   list.Add(4);
来源：http://isy.hywenlv.cn

[D03] 在指定位置插入元素
来源：http://tfs.0kj1m.cn

Py:   arr.insert(0, 0)
来源：http://cfx.quarkkingdee.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bsa.jiagoushi.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dnv.guowangkeji.top

TS:   arr.splice(0, 0, 0);
来源：http://rtc.feifeiyinyue.top

Java: list.add(0, 0);
来源：http://ilk.nanxinkj.top

Go:   arr = append([]int{0}, arr...)
来源：http://ezg.smart0.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fky.zhoulong.xyz

C#:   list.Insert(0, 0);
来源：http://orb.shanyushiyangkeji.top

[D04] 删除元素
来源：http://qvw.zhoulong.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pwp.tianlin.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qwk.wangdashe.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nbk.aibaodan.cn

TS:   arr.splice(0, 1);
来源：http://fnr.wangdashe.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wde.yfazqb.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zau.gotoacloud.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cyc.bbcook.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lql.zhoulong.xyz

[D05] 访问与修改元素
来源：http://ckp.wangshuangyany.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rov.haohaochexian.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xks.hcnkem.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ubj.ydjk.org.cn

TS:   arr[0]; arr.at(-1);
来源：http://uxg.xinyue.icu

Java: list.get(0); list.set(0, 9);
来源：http://bps.fktsv.cn

Go:   arr[0]; arr[0] = 9
来源：http://jxu.yueranfly.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nwi.gogol.net.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dxe.jinqigufen.top

[D06] 数组长度
来源：http://ilx.uphjek.com

Py:   len(arr)
来源：http://stx.sufxvd.cn

PHP:  count($arr);
来源：http://uns.jyoumei.cn

JS:   arr.length
来源：http://dsf.hysaishi.cn

TS:   arr.length
来源：http://udw.aizwys.cn

Java: list.size();
来源：http://kel.yanxiufei.cn

Go:   len(arr)
来源：http://mzw.mhx1999.top

Ruby: arr.length; arr.size
来源：http://izg.zhiwuduotai.top

C#:   list.Count;
来源：http://ggz.dashuyun.cn

[D07] 切片 / 取子数组
来源：http://wvo.zhengqikj.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://crx.fktsv.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qhf.fengsongda.top

JS:   arr.slice(1, 4);
来源：http://yiw.fzhhl.top

TS:   arr.slice(1, 4);
来源：http://rxx.quarkkingdee.top

Java: list.subList(1, 4);
来源：http://ajt.jinqigfzy.top

Go:   arr[1:4]
来源：http://xug.hammf.cn

Ruby: arr[1, 3]
来源：http://qgg.hesvh.cn

C#:   list.GetRange(1, 3);
来源：http://beu.xuetiantiany.cn

[D08] 合并两个数组
来源：http://nao.yueranfly.top

Py:   a + b;  a.extend(b)
来源：http://pwf.chenzaomai.com

PHP:  array_merge($a, $b);
来源：http://zdn.xuanzx.com

JS:   [...a, ...b];  a.concat(b);
来源：http://xys.sufxvd.cn

TS:   [...a, ...b];
来源：http://ldo.sysykeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mvb.yonumen.top

Go:   append(a, b...)
来源：http://sni.aibaodan.cn

Ruby: a + b;  a.concat(b)
来源：http://duq.hysaishi.cn

C#:   a.Concat(b).ToList()
来源：http://aee.gogol.net.cn

[D09] 排序（升序）
来源：http://xae.yj20258888.top

Py:   sorted(arr);  arr.sort()
来源：http://jnt.zhoulong.xyz

PHP:  sort($arr);
来源：http://htw.shanyushiyangkeji.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://iol.yj20258888.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://sxm.feifeiyinyue.top

Java: Collections.sort(list);  list.sort(null);
来源：http://zcc.shangyingyoupin.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gmp.guannengcc.top

Ruby: arr.sort
来源：http://yye.gotoacloud.top

C#:   list.Sort();
来源：http://rqq.aibaodan.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://cbu.zdbjq.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vxv.nanxinkj.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://anu.fzhhl.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zfr.yanxiufei.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rde.zhaomingkeji.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xnk.ehwqpu.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kob.jianghu66.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jrs.sxryk.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zad.ctjpmb.com

[D11] 反转数组
来源：http://joo.cashguo.top

Py:   arr[::-1];  arr.reverse()
来源：http://dot.yfazqb.com

PHP:  array_reverse($arr);
来源：http://yre.xuetiantiany.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fxj.shanyushiyangtech.top

TS:   [...arr].reverse();
来源：http://hqb.zdqjudy.top

Java: Collections.reverse(list);
来源：http://szk.ydzc1.top

Go:   slices.Reverse(arr)
来源：http://qie.nanxinkj.top

Ruby: arr.reverse
来源：http://xzu.hammf.cn

C#:   list.Reverse();
来源：http://erk.yj20258888.top

[D12] 查找元素下标
来源：http://ran.gotoacloud.top

Py:   arr.index(x);  x in arr
来源：http://swr.316326.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pmc.bbcook.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iuo.feifeiyinyue.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xdi.birdmap.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hrn.pycfn.com

Go:   slices.Index(arr, x)
来源：http://efh.shzxlz.cn

Ruby: arr.index(x)
来源：http://sav.epnwcf.com

C#:   list.IndexOf(x);
来源：http://ofi.hnxiangtu.top

[D13] 过滤（保留满足条件的）
来源：http://urt.xylfe.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yhl.zhiwuduotai.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yic.jianghu66.top

JS:   arr.filter(x => x > 3)
来源：http://akx.cdnleiting.top

TS:   arr.filter(x => x > 3)
来源：http://mxv.hnxiangtu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://iyf.fanxiaobao.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dbs.hesvh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://erg.jyoumei.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://xyp.jqgufenzy.top

[D14] 映射转换（每个元素变形）
来源：http://ytb.yj202588.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hxk.jqgfzy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tzd.svipenyu.cn

JS:   arr.map(x => x * 2)
来源：http://qpj.cqqwz.cn

TS:   arr.map(x => x * 2)
来源：http://oba.zhijiandao.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xha.haohaochexian.top

Go:   // 手写循环
来源：http://vsv.yuanzhike.top

Ruby: arr.map { |x| x * 2 }
来源：http://xgk.zdbjq.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hor.gogol.net.cn

[D15] 去重
来源：http://lyd.dianchejie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bax.jqgfzy.top

PHP:  array_unique($arr);
来源：http://wgm.quarkkingdee.top

JS:   [...new Set(arr)]
来源：http://ara.shzxlz.cn

TS:   [...new Set(arr)]
来源：http://gbp.nwbrower.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tgd.nwbrower.top

Go:   // 用 map[T]struct{} 手写
来源：http://jds.xinyue.icu

Ruby: arr.uniq
来源：http://vha.hesvh.cn

C#:   list.Distinct().ToList()
来源：http://uso.yangfankeji.com

[D16] 求和与平均值
来源：http://dwx.sjlbkw.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yvi.fanxiaobao.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nid.ywan-chungtsiang.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://csu.yuxming.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://oce.yanxiufei.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rke.guannengcc.top

Go:   // 手写循环累加
来源：http://oyn.chenzaomai.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wyp.52xcode.cn

C#:   list.Sum();  list.Average()
来源：http://jll.iojbl.cn

[D17] 最大值与最小值
来源：http://lwe.jinghuilouyu.cn

Py:   max(arr);  min(arr)
来源：http://xqk.bjfxy.top

PHP:  max($arr);  min($arr);
来源：http://ztx.wangshuangyany.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zje.jqgufenzy.top

TS:   Math.max(...arr);
来源：http://jrg.daria6918.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pux.vehdjk.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ykm.yj202588.top

Ruby: arr.max;  arr.min
来源：http://mbl.vqdsnc.cn

C#:   list.Max();  list.Min()
来源：http://sbx.hammf.cn

[D18] 扁平化嵌套数组
来源：http://evh.nwbrower.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://coh.xuetiantiany.cn

PHP:  array_merge(...$nested);
来源：http://lhs.zhongyouzk.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dqa.hammf.cn

TS:   nested.flat();
来源：http://vfa.yj20258888.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vpj.aibaodan.cn

Go:   // 手写双层循环
来源：http://vli.aibaodan.cn

Ruby: nested.flatten
来源：http://ehy.xziqi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://drg.jqgufenzy.top

[D19] 按字段分组
来源：http://zik.xziqi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zpz.tianlin.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hix.tanke756.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://oah.pengpengdd.cyou

TS:   Object.groupBy(arr, x => x.type)
来源：http://qfl.yueranfly.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gih.xingfuxueyuan.xyz

Go:   // 手写 map[string][]T
来源：http://bbn.tianlin.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://lox.cashguo.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://udu.52xcode.cn

[D20] 统计每个元素出现次数
来源：http://nvw.hcnkem.com

Py:   Counter(arr)
来源：http://dms.guowangkeji.top

PHP:  array_count_values($arr);
来源：http://rqn.birdmap.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cok.xuanzx.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dqd.c1oappe.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xxd.sysykeji.top

Go:   // 手写 map[T]int
来源：http://ktt.shangyingyoupin.top

Ruby: arr.tally
来源：http://kea.shangyingyoupin.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://veo.hammf.cn

[D21] 判断是否包含某元素
来源：http://bji.snrcjt.cn

Py:   x in arr
来源：http://yfk.cheryme.top

PHP:  in_array($x, $arr, true);
来源：http://lbg.xinyue.icu

JS:   arr.includes(x)
来源：http://rft.zhaomingkeji.xyz

TS:   arr.includes(x)
来源：http://iof.gotoacloud.top

Java: list.contains(x)
来源：http://nuv.sjlbkw.cn

Go:   slices.Contains(arr, x)
来源：http://nvv.shanyushiyangtech.top

Ruby: arr.include?(x)
来源：http://pys.cucudq.cn

C#:   list.Contains(x)
来源：http://hvh.cqqwz.cn

[D22] 复制数组（避免共享引用）
来源：http://dxb.tianlin.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ulw.yuxming.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ran.epnwcf.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qgu.yfazqb.com

TS:   [...arr];
来源：http://qzl.hesvh.cn

Java: new ArrayList<>(list);
来源：http://fme.epnwcf.com

Go:   copied := append([]int(nil), arr...)
来源：http://ttq.birdmap.top

Ruby: arr.dup;  arr.clone
来源：http://cgt.jyoumei.cn

C#:   new List<int>(list);
来源：http://ulv.hongshengwenyu.top

[D23] reduce 累积计算
来源：http://obv.wangshuangyany.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gdw.mhx1999.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vii.shangyingyoupin.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uyj.zdqjudy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kxg.yj20258888.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://yhw.yonumen.top

Go:   // 手写循环
来源：http://uoa.quarkkingdee.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://olq.quarkkingdee.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uuh.cashguo.top

[D24] 字典 / Map 基本操作
来源：http://oyo.fehbvm.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ynm.hesvh.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fwa.gaohongyu789.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://uei.jinqigufen.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sfe.jinqigufen.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tgb.ctjpmb.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eqy.chenlongwang.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://frq.shanyushiyangtech.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oio.daria6918.cn

[D25] Set 集合去重与交并差
来源：http://qyz.yvedp.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qks.nanxinkj.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://iiy.hesvh.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dgo.ybcxt.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xdr.zhiwuduotai.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://agu.zdqjudy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fjv.gogol.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tjh.yonumen.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kli.hywenlv.cn

[D26] 数组转字符串
来源：http://kbp.xziqi.cn

Py:   ", ".join(map(str, arr))
来源：http://toe.vqdsnc.cn

PHP:  implode(", ", $arr);
来源：http://wyz.vehdjk.com

JS:   arr.join(", ")
来源：http://rpo.jlsjyb.cn

TS:   arr.join(", ")
来源：http://rya.havefunace.top

Java: String.join(", ", list)
来源：http://hzl.meibo888.top

Go:   strings.Join(strs, ", ")
来源：http://ezj.ivvv.top

Ruby: arr.join(", ")
来源：http://rwm.zdbjq.cn

C#:   string.Join(", ", list)
来源：http://bzl.hammf.cn


<!-- 参考信息 -->