代发 wailian999

C#:   块级作用域
来源：http://qbo.yuxming.cn

[C11] 模块导入与导出
来源：http://wlj.vehdjk.com

Py:   from module import func
来源：http://yvm.ppjwa.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://nto.jianghu66.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://wpw.andypj.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dra.hammf.cn

Java: import java.util.List;
来源：http://gns.gzhubu.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wvg.nwbrower.top

Ruby: require "json"; require_relative "./util"
来源：http://iaz.ppjwa.cn

C#:   using System.Text;
来源：http://svg.chenzaomai.com

[C12] 立即执行函数 IIFE
来源：http://kfk.meibo888.top

Py:   (lambda: print("run"))()
来源：http://ixw.zhixingplan.top

PHP:  (function () { echo "run"; })();
来源：http://afx.wangshuangyany.cn

JS:   (() => { console.log("run"); })();
来源：http://ftn.dashuyun.cn

TS:   (() => { console.log("run"); })();
来源：http://qmb.xziqi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pch.yanxiufei.cn

Go:   func() { fmt.Println("run") }()
来源：http://gho.dashuyun.cn

Ruby: -> { puts "run" }.call
来源：http://tty.xylfe.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gny.c1oappe.top

[C13] 类型声明 / 类型注解
来源：http://ien.yj20258.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://eoa.shanyushiyangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://voy.9152youxi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jgm.ybcxt.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://thp.jinqigfzy.top

Java: int add(int a, int b) { return a + b; }
来源：http://xzp.shanyushiyangtech.top

Go:   func add(a, b int) int
来源：http://azw.jianghu66.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wpu.mhx1999.top

C#:   int Add(int a, int b) => a + b;
来源：http://uco.daria6918.cn

[C14] 泛型函数
来源：http://ork.redwolf501.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rvo.zhixingplan.top

PHP:  // 无泛型
来源：http://gik.c1oappe.top

JS:   // 无泛型
来源：http://slt.meibo888.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://erd.sjlbkw.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lns.hnxiangtu.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qkd.chenzaomai.com

Ruby: # 无泛型
来源：http://vco.wangdashe.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://exn.guowangkeji.top

[C15] 解构 / 展开参数
来源：http://efd.zhengqikj.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://uxe.zhengqikj.top

PHP:  [$a, $b] = $pair;
来源：http://dzb.ydjk.org.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://azf.tian-w.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://etf.9152youxi.cn

Java: // 无解构
来源：http://npr.bbcook.cn

Go:   // 无解构
来源：http://ecv.guannengcc.top

Ruby: a, b = pair
来源：http://qpc.mhx1999.top

C#:   var (a, b) = pair;
来源：http://uqi.ydjk.org.cn

[C16] 函数 / 方法重载
来源：http://eah.shanyushiyangkeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vcf.wangdashe.top

PHP:  // 无重载
来源：http://dvl.xziqi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ucu.zdqjudy.top

TS:   // 用联合类型或重载签名声明
来源：http://zch.hywenlv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://nuo.9152youxi.cn

Go:   // 无重载：用不同函数名
来源：http://jqe.zhongyouzk.top

Ruby: # 无重载：靠动态参数
来源：http://sje.aibaodan.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://pog.jqgufenzy.top

================================================================================
来源：http://hli.ywan-chungtsiang.top

D. 数组 / 列表 / 集合
来源：http://fpy.yueranfly.top

================================================================================
来源：http://mfa.yvedp.cn

[D01] 创建数组 / 列表
来源：http://eoq.hywenlv.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hok.jinqigufen.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vpk.chenjidiqi.icu

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yag.pycfn.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://vpq.cucudq.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ejq.vqdsnc.cn

Go:   arr := []int{1, 2, 3}
来源：http://ytu.yfazqb.com

Ruby: arr = [1, 2, 3]
来源：http://cgb.sysykeji.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ujg.daxiang520.top

[D02] 追加元素到末尾
来源：http://pmo.havefunace.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://soe.c1oappe.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rjx.xingfuxueyuan.xyz

JS:   arr.push(4);
来源：http://ztn.shangyingyoupin.top

TS:   arr.push(4);
来源：http://get.jinyuanbaomall.cn

Java: list.add(4);
来源：http://njq.ydzc1.top

Go:   arr = append(arr, 4)
来源：http://bxf.jqgufenzy.top

Ruby: arr << 4; arr.push(5)
来源：http://sgy.nanxinkj.top

C#:   list.Add(4);
来源：http://hhk.gaohongyu789.top

[D03] 在指定位置插入元素
来源：http://ais.0kj1m.cn

Py:   arr.insert(0, 0)
来源：http://ivd.zhoulong.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vsf.tian-w.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ltz.gaohongyu789.top

TS:   arr.splice(0, 0, 0);
来源：http://miu.jqgfzy.top

Java: list.add(0, 0);
来源：http://zrx.feifeiyinyue.top

Go:   arr = append([]int{0}, arr...)
来源：http://fji.hnxiangtu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vpd.ydjk.org.cn

C#:   list.Insert(0, 0);
来源：http://wzr.yvedp.cn

[D04] 删除元素
来源：http://tzw.xuanzx.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hxe.snrcjt.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://oit.jqgufenzy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://chh.zdbjq.cn

TS:   arr.splice(0, 1);
来源：http://ebz.cdnleiting.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://osr.daria6918.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pgp.yvedp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://evt.hywenlv.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hsn.ybcxt.top

[D05] 访问与修改元素
来源：http://smx.hongshengwenyu.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ehz.316326.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vox.guowangkeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lwf.shzxlz.cn

TS:   arr[0]; arr.at(-1);
来源：http://jfg.guowangkeji.top

Java: list.get(0); list.set(0, 9);
来源：http://bse.yvedp.cn

Go:   arr[0]; arr[0] = 9
来源：http://doi.yj202588.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qnz.ppjwa.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://spv.gaohongyu789.top

[D06] 数组长度
来源：http://fwa.zhijiandao.cn

Py:   len(arr)
来源：http://udn.gaohongyu789.top

PHP:  count($arr);
来源：http://mqt.yueranfly.top

JS:   arr.length
来源：http://yhe.xuanzx.com

TS:   arr.length
来源：http://ezj.gotoacloud.top

Java: list.size();
来源：http://kxv.epnwcf.com

Go:   len(arr)
来源：http://xfk.hongshengwenyu.top

Ruby: arr.length; arr.size
来源：http://bqz.tianlin.xyz

C#:   list.Count;
来源：http://sry.zhixingplan.top

[D07] 切片 / 取子数组
来源：http://byb.jianghu66.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lhy.kuanghao11.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gyv.ybcxt.top

JS:   arr.slice(1, 4);
来源：http://qbi.cucudq.cn

TS:   arr.slice(1, 4);
来源：http://rgl.shanyushiyangtech.top

Java: list.subList(1, 4);
来源：http://bvg.ybcxt.top

Go:   arr[1:4]
来源：http://wzw.wangshuangyany.cn

Ruby: arr[1, 3]
来源：http://muu.xinyue.icu

C#:   list.GetRange(1, 3);
来源：http://gyw.gogol.net.cn

[D08] 合并两个数组
来源：http://mne.zhongyouzk.top

Py:   a + b;  a.extend(b)
来源：http://kyo.yfazqb.com

PHP:  array_merge($a, $b);
来源：http://smq.epnwcf.com

JS:   [...a, ...b];  a.concat(b);
来源：http://cvp.zhaomingkeji.xyz

TS:   [...a, ...b];
来源：http://uqm.pycfn.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vkd.hammf.cn

Go:   append(a, b...)
来源：http://qds.dashuyun.cn

Ruby: a + b;  a.concat(b)
来源：http://ues.nanxuanxn.top

C#:   a.Concat(b).ToList()
来源：http://eqa.bbcook.cn

[D09] 排序（升序）
来源：http://dvj.epnwcf.com

Py:   sorted(arr);  arr.sort()
来源：http://cdb.yj20258888.top

PHP:  sort($arr);
来源：http://ulz.zhijiandao.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://iqf.52xcode.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://rps.guowangkeji.top

Java: Collections.sort(list);  list.sort(null);
来源：http://cbo.zhongyouzk.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hzq.cheryme.top

Ruby: arr.sort
来源：http://rmw.vqdsnc.cn

C#:   list.Sort();
来源：http://gkm.cashguo.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://skm.epnwcf.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rlm.yongpay.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://big.hammf.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lem.pengpengdd.cyou

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pid.vehdjk.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bds.shangyingyoupin.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://six.pengpengdd.cyou

Ruby: arr.sort_by { |x| x[:age] }
来源：http://iqb.shanyushiyangkeji.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bim.hongshengwenyu.top

[D11] 反转数组
来源：http://ram.sjlbkw.cn

Py:   arr[::-1];  arr.reverse()
来源：http://yga.zycfv.cn

PHP:  array_reverse($arr);
来源：http://ril.sufxvd.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vlr.guowangkeji.top

TS:   [...arr].reverse();
来源：http://kzv.xylfe.cn

Java: Collections.reverse(list);
来源：http://qcr.zhixingplan.top

Go:   slices.Reverse(arr)
来源：http://dmd.ctjpmb.com

Ruby: arr.reverse
来源：http://mqv.zhijiandao.cn

C#:   list.Reverse();
来源：http://bka.vehdjk.com

[D12] 查找元素下标
来源：http://fgd.hongshengwenyu.top

Py:   arr.index(x);  x in arr
来源：http://khg.shzxlz.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://buy.shuidangran.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zmc.daria6918.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yeq.jqgfzy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fbr.zhoulong.xyz

Go:   slices.Index(arr, x)
来源：http://ehd.zhengqikj.top

Ruby: arr.index(x)
来源：http://yhr.yj20258888.top

C#:   list.IndexOf(x);
来源：http://xaw.fzhhl.top

[D13] 过滤（保留满足条件的）
来源：http://pgy.yangfankeji.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ybg.zdqjudy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wht.yj20258888.top

JS:   arr.filter(x => x > 3)
来源：http://xoj.jqgfzy.top

TS:   arr.filter(x => x > 3)
来源：http://hkp.sxryk.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bxh.quarkkingdee.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yaj.feifeiyinyue.top

Ruby: arr.select { |x| x > 3 }
来源：http://xns.zdbjq.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vlk.tianlin.xyz

[D14] 映射转换（每个元素变形）
来源：http://xgd.yangfankeji.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gqv.shangyingyoupin.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rhy.316326.xyz

JS:   arr.map(x => x * 2)
来源：http://yuq.hysaishi.cn

TS:   arr.map(x => x * 2)
来源：http://oja.sjlbkw.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://pxn.cucudq.cn

Go:   // 手写循环
来源：http://myu.pycfn.com

Ruby: arr.map { |x| x * 2 }
来源：http://xqn.cqqwz.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jnw.snrcjt.cn

[D15] 去重
来源：http://kow.yvedp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rcz.yangfankeji.com

PHP:  array_unique($arr);
来源：http://kxk.sysykeji.top

JS:   [...new Set(arr)]
来源：http://epr.ydjk.org.cn

TS:   [...new Set(arr)]
来源：http://xkh.0kj1m.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vnc.jiagoushi.top

Go:   // 用 map[T]struct{} 手写
来源：http://bge.ivvv.top

Ruby: arr.uniq
来源：http://cin.ywan-chungtsiang.top

C#:   list.Distinct().ToList()
来源：http://dml.chenlongwang.top

[D16] 求和与平均值
来源：http://paq.fktsv.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mcx.yangfankeji.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dfa.fengsongda.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dal.gotoacloud.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ydc.jinqigfzy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wld.ivvv.top

Go:   // 手写循环累加
来源：http://uir.feifeiyinyue.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://piz.xinyue.icu

C#:   list.Sum();  list.Average()
来源：http://hjb.shanyushiyangtech.top

[D17] 最大值与最小值
来源：http://hdp.vehdjk.com

Py:   max(arr);  min(arr)
来源：http://rdq.smart0.xyz

PHP:  max($arr);  min($arr);
来源：http://vmj.0kj1m.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://icx.zycfv.cn

TS:   Math.max(...arr);
来源：http://eaf.cucudq.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bzm.bbcook.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jwq.sufxvd.cn

Ruby: arr.max;  arr.min
来源：http://ipt.shzxlz.cn

C#:   list.Max();  list.Min()
来源：http://ljz.feifeiyinyue.top

[D18] 扁平化嵌套数组
来源：http://drw.svipenyu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ujz.jinyuanbaomall.cn

PHP:  array_merge(...$nested);
来源：http://kpi.uphjek.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nic.hnqzz.top

TS:   nested.flat();
来源：http://otf.redwolf501.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rsm.ywan-chungtsiang.top

Go:   // 手写双层循环
来源：http://lcy.redwolf501.top

Ruby: nested.flatten
来源：http://hnm.jlsjyb.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://jcd.chenlongwang.top

[D19] 按字段分组
来源：http://idu.shanyushiyangtech.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ete.aibaodan.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wsw.tarul.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hec.0kj1m.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zcu.fzhhl.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yyx.hammf.cn

Go:   // 手写 map[string][]T
来源：http://ydr.9152youxi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wix.haohaochexian.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://iiv.hongshengwenyu.top

[D20] 统计每个元素出现次数
来源：http://fgk.zhaomingkeji.xyz

Py:   Counter(arr)
来源：http://ogf.jianghu66.top

PHP:  array_count_values($arr);
来源：http://tjm.kuanghao11.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ygq.feifeiyinyue.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bzq.zhengqikj.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pnw.jinyuanbaomall.cn

Go:   // 手写 map[T]int
来源：http://dof.ivvv.top

Ruby: arr.tally
来源：http://ayu.quarkkingdee.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://res.bjfxy.top

[D21] 判断是否包含某元素
来源：http://xwu.jinqigfzy.top

Py:   x in arr
来源：http://afl.zhoulong.xyz

PHP:  in_array($x, $arr, true);
来源：http://jrh.ywan-chungtsiang.top

JS:   arr.includes(x)
来源：http://bcb.jinqigufen.top

TS:   arr.includes(x)
来源：http://day.daxiang520.top

Java: list.contains(x)
来源：http://tul.52xcode.cn

Go:   slices.Contains(arr, x)
来源：http://jja.zdbjq.cn

Ruby: arr.include?(x)
来源：http://raw.jinqigfzy.top

C#:   list.Contains(x)
来源：http://hle.hnxiangtu.top

[D22] 复制数组（避免共享引用）
来源：http://fme.vehdjk.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dsc.tanke756.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dnl.jinyuanbaomall.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nnd.snrcjt.cn

TS:   [...arr];
来源：http://jqc.chenjidiqi.icu

Java: new ArrayList<>(list);
来源：http://fge.wangdashe.top

Go:   copied := append([]int(nil), arr...)
来源：http://cen.ydzc1.top

Ruby: arr.dup;  arr.clone
来源：http://trw.gzhubu.top

C#:   new List<int>(list);
来源：http://xsd.52xcode.cn

[D23] reduce 累积计算
来源：http://xmp.jinghuilouyu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wck.jqgfzy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wob.snrcjt.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sah.xylfe.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yvp.xingfuxueyuan.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://paa.0kj1m.cn

Go:   // 手写循环
来源：http://wjq.jinqigufen.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jal.jianghu66.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://erd.vehdjk.com

[D24] 字典 / Map 基本操作
来源：http://nuh.jlsjyb.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vaq.mhx1999.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dpk.yj202588.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hsn.hongshengwenyu.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pgu.shuidangran.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jjl.hnqzz.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://imq.cucudq.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://opr.zhiwuduotai.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zoh.316326.xyz

[D25] Set 集合去重与交并差
来源：http://bad.chenlongwang.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zlh.yonumen.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yrp.svipenyu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kkg.jinqigufen.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uet.sysykeji.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jgu.hfpthk.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ftg.chenzaomai.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kzz.jqgufenzy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://azf.xinyue.icu

[D26] 数组转字符串
来源：http://sdq.tianlin.xyz

Py:   ", ".join(map(str, arr))
来源：http://tkr.316326.xyz

PHP:  implode(", ", $arr);
来源：http://zcm.aizwys.cn

JS:   arr.join(", ")
来源：http://ehj.zhixingplan.top

TS:   arr.join(", ")
来源：http://ifw.fehbvm.com

Java: String.join(", ", list)
来源：http://tql.dianchejie.cn

Go:   strings.Join(strs, ", ")
来源：http://moj.aizwys.cn

Ruby: arr.join(", ")
来源：http://jka.daxiang520.top

C#:   string.Join(", ", list)
来源：http://udm.316326.xyz

================================================================================
来源：http://nub.yj20258.top

E. 字符串处理
来源：http://mfr.tian-w.cn

================================================================================
来源：http://ooo.kuanghao11.cn

[E01] 拼接字符串
来源：http://inw.jyoumei.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ixe.cucudq.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dhr.nanxuanxn.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nnp.snrcjt.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://aje.havefunace.top


<!-- 参考信息 -->