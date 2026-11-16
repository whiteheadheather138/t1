代发 wailian999

TS:   同 JS
来源：http://xcp.chenlongwang.top

Java: 方法内为块级作用域
来源：http://dqs.zdqjudy.top

Go:   花括号块级作用域
来源：http://zvk.hnqzz.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uob.sufxvd.cn

C#:   块级作用域
来源：http://fkd.quarkkingdee.top

[C11] 模块导入与导出
来源：http://asg.gotoacloud.top

Py:   from module import func
来源：http://qfx.gotoacloud.top

PHP:  require "file.php";  或 use App\Service;
来源：http://syz.cdnleiting.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://eub.zhoulong.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ruv.ybcxt.top

Java: import java.util.List;
来源：http://nxd.andypj.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://aad.jinyuanbaomall.cn

Ruby: require "json"; require_relative "./util"
来源：http://yrq.xinyue.icu

C#:   using System.Text;
来源：http://gec.feifeiyinyue.top

[C12] 立即执行函数 IIFE
来源：http://ncr.jinqigufen.top

Py:   (lambda: print("run"))()
来源：http://acs.shangyingyoupin.top

PHP:  (function () { echo "run"; })();
来源：http://gvj.snrcjt.cn

JS:   (() => { console.log("run"); })();
来源：http://hzh.tarul.cn

TS:   (() => { console.log("run"); })();
来源：http://qxu.nanxinkj.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xhl.xuanzx.com

Go:   func() { fmt.Println("run") }()
来源：http://vlp.hywenlv.cn

Ruby: -> { puts "run" }.call
来源：http://dlh.svipenyu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zbw.fzhhl.top

[C13] 类型声明 / 类型注解
来源：http://kbk.316326.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rkc.bjfxy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ret.tanke756.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wma.bjfxy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dkd.feifeiyinyue.top

Java: int add(int a, int b) { return a + b; }
来源：http://zuk.feifeiyinyue.top

Go:   func add(a, b int) int
来源：http://xmb.ehwqpu.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uyx.dashuyun.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mdz.mhx1999.top

[C14] 泛型函数
来源：http://iru.yvedp.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uhl.hesvh.cn

PHP:  // 无泛型
来源：http://ztm.hongshengwenyu.top

JS:   // 无泛型
来源：http://opd.guowangkeji.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wrd.yj20258888.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://knm.yfazqb.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://whg.uphjek.com

Ruby: # 无泛型
来源：http://bue.haohaochexian.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qzb.xziqi.cn

[C15] 解构 / 展开参数
来源：http://fwi.zdqjudy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://one.fehbvm.com

PHP:  [$a, $b] = $pair;
来源：http://fzw.fanxiaobao.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gxl.fanxiaobao.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rfq.shuidangran.top

Java: // 无解构
来源：http://nbd.zdqjudy.top

Go:   // 无解构
来源：http://xfs.cheryme.top

Ruby: a, b = pair
来源：http://ehe.zdqjudy.top

C#:   var (a, b) = pair;
来源：http://xsk.havefunace.top

[C16] 函数 / 方法重载
来源：http://uat.yanxiufei.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gdp.chenlongwang.top

PHP:  // 无重载
来源：http://bwa.cheryme.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://orm.yvedp.cn

TS:   // 用联合类型或重载签名声明
来源：http://wjq.haohaochexian.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ppl.zhixingplan.top

Go:   // 无重载：用不同函数名
来源：http://jmy.cqqwz.cn

Ruby: # 无重载：靠动态参数
来源：http://mdo.gzhubu.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://jka.yfazqb.com

================================================================================
来源：http://mps.sufxvd.cn

D. 数组 / 列表 / 集合
来源：http://wtp.shuidangran.top

================================================================================
来源：http://sew.xuanzx.com

[D01] 创建数组 / 列表
来源：http://sjj.yj202588.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://tcm.ehwqpu.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rwz.pycfn.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ewl.sjlbkw.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vkt.tanke756.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mrm.xingfuxueyuan.xyz

Go:   arr := []int{1, 2, 3}
来源：http://ieu.yj202588.top

Ruby: arr = [1, 2, 3]
来源：http://syg.wangdashe.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kgq.jlsjyb.cn

[D02] 追加元素到末尾
来源：http://rmh.daria6918.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lvd.birdmap.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zlp.ywan-chungtsiang.top

JS:   arr.push(4);
来源：http://low.hysaishi.cn

TS:   arr.push(4);
来源：http://rmv.hnxiangtu.top

Java: list.add(4);
来源：http://kka.fzhhl.top

Go:   arr = append(arr, 4)
来源：http://pvd.sjlbkw.cn

Ruby: arr << 4; arr.push(5)
来源：http://lfy.shanyushiyangtech.top

C#:   list.Add(4);
来源：http://wxp.0kj1m.cn

[D03] 在指定位置插入元素
来源：http://nrf.tian-w.cn

Py:   arr.insert(0, 0)
来源：http://xbx.cdnleiting.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qwu.svipenyu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zhp.gzhubu.top

TS:   arr.splice(0, 0, 0);
来源：http://nzd.fzhhl.top

Java: list.add(0, 0);
来源：http://vdz.jinqigufen.top

Go:   arr = append([]int{0}, arr...)
来源：http://nrz.chenzaomai.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ufs.zhaomingkeji.xyz

C#:   list.Insert(0, 0);
来源：http://hmg.hywenlv.cn

[D04] 删除元素
来源：http://fzi.nwbrower.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://plu.yonumen.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kgr.tanke756.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ari.kuanghao11.cn

TS:   arr.splice(0, 1);
来源：http://uik.xziqi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cxh.nwbrower.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ltn.ehwqpu.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dio.cashguo.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sbd.jianghu66.top

[D05] 访问与修改元素
来源：http://brf.guannengcc.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mil.fehbvm.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ssj.andypj.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fqa.chenlongwang.top

TS:   arr[0]; arr.at(-1);
来源：http://djf.guowangkeji.top

Java: list.get(0); list.set(0, 9);
来源：http://shd.vqdsnc.cn

Go:   arr[0]; arr[0] = 9
来源：http://bxa.shangyingyoupin.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rfo.jinyuanbaomall.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ymj.wangdashe.top

[D06] 数组长度
来源：http://xyy.zhixingplan.top

Py:   len(arr)
来源：http://ehd.gotoacloud.top

PHP:  count($arr);
来源：http://pwe.daria6918.cn

JS:   arr.length
来源：http://zid.xingfuxueyuan.xyz

TS:   arr.length
来源：http://xrj.fehbvm.com

Java: list.size();
来源：http://ggt.jlsjyb.cn

Go:   len(arr)
来源：http://ski.ybcxt.top

Ruby: arr.length; arr.size
来源：http://ioo.hammf.cn

C#:   list.Count;
来源：http://ttu.guowangkeji.top

[D07] 切片 / 取子数组
来源：http://ixb.pycfn.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qeh.zycfv.cn

PHP:  array_slice($arr, 1, 3);
来源：http://aav.cashguo.top

JS:   arr.slice(1, 4);
来源：http://nbl.aibaodan.cn

TS:   arr.slice(1, 4);
来源：http://cbx.hcnkem.com

Java: list.subList(1, 4);
来源：http://tiu.jinqigufen.top

Go:   arr[1:4]
来源：http://cdn.tianlin.xyz

Ruby: arr[1, 3]
来源：http://wyq.daria6918.cn

C#:   list.GetRange(1, 3);
来源：http://bad.jianghu66.top

[D08] 合并两个数组
来源：http://rfg.jinqigufen.top

Py:   a + b;  a.extend(b)
来源：http://nrs.hammf.cn

PHP:  array_merge($a, $b);
来源：http://mke.gaohongyu789.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ozp.shangyingyoupin.top

TS:   [...a, ...b];
来源：http://jqb.xziqi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tgd.aizwys.cn

Go:   append(a, b...)
来源：http://wrm.ivvv.top

Ruby: a + b;  a.concat(b)
来源：http://oej.jinqigufen.top

C#:   a.Concat(b).ToList()
来源：http://tof.fanxiaobao.xyz

[D09] 排序（升序）
来源：http://lpc.gotoacloud.top

Py:   sorted(arr);  arr.sort()
来源：http://kuh.zycfv.cn

PHP:  sort($arr);
来源：http://lqh.guannengcc.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sqk.yj20258888.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://iey.yvedp.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ger.fehbvm.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gyv.snrcjt.cn

Ruby: arr.sort
来源：http://krq.jinqigfzy.top

C#:   list.Sort();
来源：http://gsg.shanyushiyangkeji.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://imj.zhijiandao.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sws.yj20258888.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sip.zycfv.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ypn.ywan-chungtsiang.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://anb.yuxming.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rwu.daria6918.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pgp.xingfuxueyuan.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mqk.xingfuxueyuan.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nnn.haohaochexian.top

[D11] 反转数组
来源：http://xhy.xinyue.icu

Py:   arr[::-1];  arr.reverse()
来源：http://ppp.gzhubu.top

PHP:  array_reverse($arr);
来源：http://hqz.fengsongda.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://iud.zhiwuduotai.top

TS:   [...arr].reverse();
来源：http://ruy.shuidangran.top

Java: Collections.reverse(list);
来源：http://cjn.ybcxt.top

Go:   slices.Reverse(arr)
来源：http://bhx.guowangkeji.top

Ruby: arr.reverse
来源：http://jzn.meibo888.top

C#:   list.Reverse();
来源：http://yoz.gzhubu.top

[D12] 查找元素下标
来源：http://zbv.52xcode.cn

Py:   arr.index(x);  x in arr
来源：http://ryy.shanyushiyangtech.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cci.nanxinkj.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://din.yuxming.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zyl.52xcode.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dqx.ehwqpu.com

Go:   slices.Index(arr, x)
来源：http://yhz.cheryme.top

Ruby: arr.index(x)
来源：http://ldv.sjlbkw.cn

C#:   list.IndexOf(x);
来源：http://nss.hammf.cn

[D13] 过滤（保留满足条件的）
来源：http://phu.xylfe.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rak.ybcxt.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ofv.9152youxi.cn

JS:   arr.filter(x => x > 3)
来源：http://gvh.xuanzx.com

TS:   arr.filter(x => x > 3)
来源：http://pde.shzxlz.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hvv.meibo888.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ulz.sweek.top

Ruby: arr.select { |x| x > 3 }
来源：http://pxf.fehbvm.com

C#:   list.Where(x => x > 3).ToList()
来源：http://ael.wangdashe.top

[D14] 映射转换（每个元素变形）
来源：http://egx.shangyingyoupin.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dxq.hnxiangtu.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qtw.wangdashe.top

JS:   arr.map(x => x * 2)
来源：http://ckb.jqgfzy.top

TS:   arr.map(x => x * 2)
来源：http://afh.fehbvm.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://via.yfazqb.com

Go:   // 手写循环
来源：http://how.yueranfly.top

Ruby: arr.map { |x| x * 2 }
来源：http://llg.aibaodan.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bvs.zhiwuduotai.top

[D15] 去重
来源：http://dxz.hcnkem.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cil.chenlongwang.top

PHP:  array_unique($arr);
来源：http://ewo.fzhhl.top

JS:   [...new Set(arr)]
来源：http://piq.zhiwuduotai.top

TS:   [...new Set(arr)]
来源：http://wte.fanxiaobao.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://asx.sysykeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://nta.fanxiaobao.xyz

Ruby: arr.uniq
来源：http://zdm.zdqjudy.top

C#:   list.Distinct().ToList()
来源：http://jaf.chenzaomai.com

[D16] 求和与平均值
来源：http://hjy.gogol.net.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rut.vehdjk.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dbs.sxryk.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://eip.gzhubu.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wmx.wangshuangyany.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xcg.jianghu66.top

Go:   // 手写循环累加
来源：http://pqw.shuidangran.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ljg.dianchejie.cn

C#:   list.Sum();  list.Average()
来源：http://urt.zdqjudy.top

[D17] 最大值与最小值
来源：http://blz.tarul.cn

Py:   max(arr);  min(arr)
来源：http://acc.daria6918.cn

PHP:  max($arr);  min($arr);
来源：http://clr.jqgufenzy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://eqz.zycfv.cn

TS:   Math.max(...arr);
来源：http://vlv.hywenlv.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rtf.ehwqpu.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jaj.shanyushiyangtech.top

Ruby: arr.max;  arr.min
来源：http://jvo.yuxming.cn

C#:   list.Max();  list.Min()
来源：http://yae.shzxlz.cn

[D18] 扁平化嵌套数组
来源：http://mbs.jlsjyb.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yxp.xingfuxueyuan.xyz

PHP:  array_merge(...$nested);
来源：http://ros.fehbvm.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dab.jinqigufen.top

TS:   nested.flat();
来源：http://rcy.aibaodan.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cff.pycfn.com

Go:   // 手写双层循环
来源：http://vkz.nwbrower.top

Ruby: nested.flatten
来源：http://fkz.316326.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://zea.tian-w.cn

[D19] 按字段分组
来源：http://jaw.quarkkingdee.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qsm.jinqigufen.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ikn.fehbvm.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mnv.fanxiaobao.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://lau.hcnkem.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jii.chenzaomai.com

Go:   // 手写 map[string][]T
来源：http://chf.yueranfly.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://hdx.yvedp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tic.ydjk.org.cn

[D20] 统计每个元素出现次数
来源：http://ovc.wangshuangyany.cn

Py:   Counter(arr)
来源：http://fmf.cdnleiting.top

PHP:  array_count_values($arr);
来源：http://yxl.chenlongwang.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zwq.yanxiufei.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wri.vqdsnc.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xzk.ydzc1.top

Go:   // 手写 map[T]int
来源：http://eeg.daria6918.cn

Ruby: arr.tally
来源：http://sxy.yangfankeji.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://iqc.iojbl.cn

[D21] 判断是否包含某元素
来源：http://fbb.ppjwa.cn

Py:   x in arr
来源：http://kmc.hcnkem.com

PHP:  in_array($x, $arr, true);
来源：http://fxh.dashuyun.cn

JS:   arr.includes(x)
来源：http://wau.andypj.xyz

TS:   arr.includes(x)
来源：http://qqc.yuanzhike.top

Java: list.contains(x)
来源：http://mnd.zycfv.cn

Go:   slices.Contains(arr, x)
来源：http://bdm.fzhhl.top

Ruby: arr.include?(x)
来源：http://tyd.jianghu66.top

C#:   list.Contains(x)
来源：http://aaj.wangdashe.top

[D22] 复制数组（避免共享引用）
来源：http://nwd.sweek.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ndg.zhengqikj.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://csl.xylfe.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ipm.xuanzx.com

TS:   [...arr];
来源：http://nqm.9152youxi.cn

Java: new ArrayList<>(list);
来源：http://sar.shuidangran.top

Go:   copied := append([]int(nil), arr...)
来源：http://ciz.9152youxi.cn

Ruby: arr.dup;  arr.clone
来源：http://byw.chenzaomai.com

C#:   new List<int>(list);
来源：http://tye.snrcjt.cn

[D23] reduce 累积计算
来源：http://zqz.zhiwuduotai.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qqf.tian-w.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vfq.0kj1m.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rcl.ivvv.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jsn.hcnkem.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://snj.xziqi.cn

Go:   // 手写循环
来源：http://psc.zdbjq.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://swz.smart0.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sbn.zhongyouzk.top

[D24] 字典 / Map 基本操作
来源：http://cjg.fengsongda.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bmm.hysaishi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gcn.shuidangran.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://roi.meibo888.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rfd.chenzaomai.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vbw.gotoacloud.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gkd.ydjk.org.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ehd.zhaomingkeji.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fvn.feifeiyinyue.top

[D25] Set 集合去重与交并差
来源：http://rkr.chenjidiqi.icu

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cny.cheryme.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rbp.smart0.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rhc.yueranfly.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://shh.xingfuxueyuan.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://loi.hongshengwenyu.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pvl.pengpengdd.cyou

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qlm.redwolf501.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sqb.mhx1999.top

[D26] 数组转字符串
来源：http://hsh.zhengqikj.top

Py:   ", ".join(map(str, arr))
来源：http://fqu.tarul.cn

PHP:  implode(", ", $arr);
来源：http://xtn.xuetiantiany.cn

JS:   arr.join(", ")
来源：http://hio.yj202588.top

TS:   arr.join(", ")
来源：http://kwx.jinghuilouyu.cn

Java: String.join(", ", list)
来源：http://nvc.ppjwa.cn

Go:   strings.Join(strs, ", ")
来源：http://qks.sysykeji.top

Ruby: arr.join(", ")
来源：http://kam.yj202588.top

C#:   string.Join(", ", list)
来源：http://kot.smart0.xyz

================================================================================
来源：http://qhn.tian-w.cn

E. 字符串处理
来源：http://nhn.yongpay.top

================================================================================
来源：http://zkg.hcnkem.com

[E01] 拼接字符串
来源：http://kvm.wangshuangyany.cn


<!-- 参考信息 -->