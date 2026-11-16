代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://udc.nwbrower.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ouq.kuanghao11.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://eji.tanke756.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bci.xylfe.cn

[C10] 变量作用域
来源：http://atg.fengsongda.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fww.xinyue.icu

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ikw.sjlbkw.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pwu.zhijiandao.cn

TS:   同 JS
来源：http://kfu.jiagoushi.top

Java: 方法内为块级作用域
来源：http://mxw.tanke756.top

Go:   花括号块级作用域
来源：http://vgg.nanxinkj.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zxl.hnqzz.top

C#:   块级作用域
来源：http://hll.feifeiyinyue.top

[C11] 模块导入与导出
来源：http://wfd.shzxlz.cn

Py:   from module import func
来源：http://ddb.zhongyouzk.top

PHP:  require "file.php";  或 use App\Service;
来源：http://bvf.wangdashe.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://yhw.smart0.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bci.ywan-chungtsiang.top

Java: import java.util.List;
来源：http://fdr.hesvh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zru.zhaomingkeji.xyz

Ruby: require "json"; require_relative "./util"
来源：http://eas.jqgufenzy.top

C#:   using System.Text;
来源：http://uix.jyoumei.cn

[C12] 立即执行函数 IIFE
来源：http://epm.havefunace.top

Py:   (lambda: print("run"))()
来源：http://quw.shzxlz.cn

PHP:  (function () { echo "run"; })();
来源：http://akj.iojbl.cn

JS:   (() => { console.log("run"); })();
来源：http://zfd.jinqigufen.top

TS:   (() => { console.log("run"); })();
来源：http://qsd.xuanzx.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vtw.tanke756.top

Go:   func() { fmt.Println("run") }()
来源：http://dbz.nanxinkj.top

Ruby: -> { puts "run" }.call
来源：http://hrs.tarul.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://bwk.yfazqb.com

[C13] 类型声明 / 类型注解
来源：http://shy.yj20258.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://uzv.yfazqb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yua.cheryme.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fdk.yj20258888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wqc.hcnkem.com

Java: int add(int a, int b) { return a + b; }
来源：http://cwr.guannengcc.top

Go:   func add(a, b int) int
来源：http://qfo.ppjwa.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yrx.jinghuilouyu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://amg.shuidangran.top

[C14] 泛型函数
来源：http://ojc.hywenlv.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lpb.zhaomingkeji.xyz

PHP:  // 无泛型
来源：http://cgy.ydzc1.top

JS:   // 无泛型
来源：http://iyq.yuxming.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wza.jinqigfzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://awr.jinqigfzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xwj.dashuyun.cn

Ruby: # 无泛型
来源：http://myg.cqqwz.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ipp.yanxiufei.cn

[C15] 解构 / 展开参数
来源：http://apf.yanxiufei.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yib.yuxming.cn

PHP:  [$a, $b] = $pair;
来源：http://rrb.xuetiantiany.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sfi.shangyingyoupin.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://acd.jiagoushi.top

Java: // 无解构
来源：http://awz.jqgufenzy.top

Go:   // 无解构
来源：http://cti.jiagoushi.top

Ruby: a, b = pair
来源：http://yjp.cashguo.top

C#:   var (a, b) = pair;
来源：http://alr.fengsongda.top

[C16] 函数 / 方法重载
来源：http://hgz.fzhhl.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nef.wangdashe.top

PHP:  // 无重载
来源：http://lgw.hnqzz.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://zmu.tianlin.xyz

TS:   // 用联合类型或重载签名声明
来源：http://ksv.c1oappe.top

Java: void f(int a) {}  void f(String a) {}
来源：http://gng.ydjk.org.cn

Go:   // 无重载：用不同函数名
来源：http://afb.hywenlv.cn

Ruby: # 无重载：靠动态参数
来源：http://anx.cucudq.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ipn.bbcook.cn

================================================================================
来源：http://uuf.sxryk.cn

D. 数组 / 列表 / 集合
来源：http://sat.zhijiandao.cn

================================================================================
来源：http://lys.yvedp.cn

[D01] 创建数组 / 列表
来源：http://tpy.chenjidiqi.icu

Py:   arr = [1, 2, 3];  empty = []
来源：http://max.hcnkem.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://spi.zhaomingkeji.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rgw.chenzaomai.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://hrd.dashuyun.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hft.yonumen.top

Go:   arr := []int{1, 2, 3}
来源：http://hzw.hysaishi.cn

Ruby: arr = [1, 2, 3]
来源：http://hdr.zhoulong.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mzy.zhongyouzk.top

[D02] 追加元素到末尾
来源：http://hrg.gaohongyu789.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zws.jiagoushi.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mmp.epnwcf.com

JS:   arr.push(4);
来源：http://rdk.birdmap.top

TS:   arr.push(4);
来源：http://ifx.wangdashe.top

Java: list.add(4);
来源：http://ybx.zhijiandao.cn

Go:   arr = append(arr, 4)
来源：http://tvl.nwbrower.top

Ruby: arr << 4; arr.push(5)
来源：http://csl.zhengqikj.top

C#:   list.Add(4);
来源：http://tax.shuidangran.top

[D03] 在指定位置插入元素
来源：http://ddo.fzhhl.top

Py:   arr.insert(0, 0)
来源：http://qjm.shuidangran.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pzb.fengsongda.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://igu.havefunace.top

TS:   arr.splice(0, 0, 0);
来源：http://msh.chenlongwang.top

Java: list.add(0, 0);
来源：http://sfv.cashguo.top

Go:   arr = append([]int{0}, arr...)
来源：http://fev.guowangkeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pwh.yj202588.top

C#:   list.Insert(0, 0);
来源：http://onw.zycfv.cn

[D04] 删除元素
来源：http://mff.nwbrower.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://eff.sweek.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://npf.xziqi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fpt.guowangkeji.top

TS:   arr.splice(0, 1);
来源：http://thc.daxiang520.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nhj.yfazqb.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ncy.hysaishi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rip.fktsv.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gea.yj20258888.top

[D05] 访问与修改元素
来源：http://bpz.pycfn.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wdt.feifeiyinyue.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yth.pycfn.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wit.dianchejie.cn

TS:   arr[0]; arr.at(-1);
来源：http://zms.hywenlv.cn

Java: list.get(0); list.set(0, 9);
来源：http://ewy.yongpay.top

Go:   arr[0]; arr[0] = 9
来源：http://wbl.cashguo.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pro.fzhhl.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yfm.c1oappe.top

[D06] 数组长度
来源：http://pxg.epnwcf.com

Py:   len(arr)
来源：http://bbp.yanxiufei.cn

PHP:  count($arr);
来源：http://xyn.yuxming.cn

JS:   arr.length
来源：http://ldc.zdqjudy.top

TS:   arr.length
来源：http://wlb.wangshuangyany.cn

Java: list.size();
来源：http://swe.guowangkeji.top

Go:   len(arr)
来源：http://dxm.ydzc1.top

Ruby: arr.length; arr.size
来源：http://jeq.hysaishi.cn

C#:   list.Count;
来源：http://owq.yj202588.top

[D07] 切片 / 取子数组
来源：http://vok.hnqzz.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vmc.tian-w.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gla.jlsjyb.cn

JS:   arr.slice(1, 4);
来源：http://vyw.yfazqb.com

TS:   arr.slice(1, 4);
来源：http://abs.mhx1999.top

Java: list.subList(1, 4);
来源：http://qih.fanxiaobao.xyz

Go:   arr[1:4]
来源：http://ahy.shanyushiyangkeji.top

Ruby: arr[1, 3]
来源：http://hhe.ivvv.top

C#:   list.GetRange(1, 3);
来源：http://rap.zhongyouzk.top

[D08] 合并两个数组
来源：http://owd.nanxuanxn.top

Py:   a + b;  a.extend(b)
来源：http://fvt.fanxiaobao.xyz

PHP:  array_merge($a, $b);
来源：http://ugb.vqdsnc.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://uko.shzxlz.cn

TS:   [...a, ...b];
来源：http://gmb.hysaishi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://eny.jinyuanbaomall.cn

Go:   append(a, b...)
来源：http://pyw.hnqzz.top

Ruby: a + b;  a.concat(b)
来源：http://pll.hammf.cn

C#:   a.Concat(b).ToList()
来源：http://suf.jqgfzy.top

[D09] 排序（升序）
来源：http://fbe.yueranfly.top

Py:   sorted(arr);  arr.sort()
来源：http://gcj.daxiang520.top

PHP:  sort($arr);
来源：http://rwg.zhiwuduotai.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cbp.dashuyun.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://vuj.316326.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://wyd.iojbl.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nwb.jqgufenzy.top

Ruby: arr.sort
来源：http://rle.zhaomingkeji.xyz

C#:   list.Sort();
来源：http://hzk.smart0.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://vzg.tanke756.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cbm.nanxinkj.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xuy.hfpthk.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jaq.shanyushiyangtech.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rwi.xziqi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://suy.pengpengdd.cyou

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gvo.sysykeji.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://spe.zhaomingkeji.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://agg.ybcxt.top

[D11] 反转数组
来源：http://wjk.tian-w.cn

Py:   arr[::-1];  arr.reverse()
来源：http://nie.shuidangran.top

PHP:  array_reverse($arr);
来源：http://mpo.xuetiantiany.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vgw.birdmap.top

TS:   [...arr].reverse();
来源：http://syn.shzxlz.cn

Java: Collections.reverse(list);
来源：http://syt.0kj1m.cn

Go:   slices.Reverse(arr)
来源：http://vvg.shangyingyoupin.top

Ruby: arr.reverse
来源：http://gbz.jqgfzy.top

C#:   list.Reverse();
来源：http://urh.ydzc1.top

[D12] 查找元素下标
来源：http://cek.snrcjt.cn

Py:   arr.index(x);  x in arr
来源：http://qcd.cucudq.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://urg.guannengcc.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rgt.52xcode.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xkq.c1oappe.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mhx.sweek.top

Go:   slices.Index(arr, x)
来源：http://ktq.wangdashe.top

Ruby: arr.index(x)
来源：http://gyz.kuanghao11.cn

C#:   list.IndexOf(x);
来源：http://bgf.zhaomingkeji.xyz

[D13] 过滤（保留满足条件的）
来源：http://erk.chenzaomai.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bft.gaohongyu789.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://iml.cqqwz.cn

JS:   arr.filter(x => x > 3)
来源：http://ote.smart0.xyz

TS:   arr.filter(x => x > 3)
来源：http://zwl.yvedp.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fku.hysaishi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fhb.316326.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://pny.hammf.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://tcn.jinqigfzy.top

[D14] 映射转换（每个元素变形）
来源：http://lfv.ywan-chungtsiang.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://phi.c1oappe.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://suu.hammf.cn

JS:   arr.map(x => x * 2)
来源：http://rip.smart0.xyz

TS:   arr.map(x => x * 2)
来源：http://tuu.redwolf501.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://pad.uphjek.com

Go:   // 手写循环
来源：http://cwf.sufxvd.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ojj.andypj.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://sum.sysykeji.top

[D15] 去重
来源：http://qjk.guowangkeji.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lcy.yfazqb.com

PHP:  array_unique($arr);
来源：http://cke.sufxvd.cn

JS:   [...new Set(arr)]
来源：http://tjz.ppjwa.cn

TS:   [...new Set(arr)]
来源：http://zbu.xziqi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zwk.daxiang520.top

Go:   // 用 map[T]struct{} 手写
来源：http://lww.chenlongwang.top

Ruby: arr.uniq
来源：http://fju.vehdjk.com

C#:   list.Distinct().ToList()
来源：http://mjh.yongpay.top

[D16] 求和与平均值
来源：http://mvt.sufxvd.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qgb.jlsjyb.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://iza.bjfxy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://aqi.cucudq.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ykq.zdqjudy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sij.aizwys.cn

Go:   // 手写循环累加
来源：http://uuf.hywenlv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pjl.shangyingyoupin.top

C#:   list.Sum();  list.Average()
来源：http://efp.kuanghao11.cn

[D17] 最大值与最小值
来源：http://rli.birdmap.top

Py:   max(arr);  min(arr)
来源：http://zhi.yfazqb.com

PHP:  max($arr);  min($arr);
来源：http://wje.tarul.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ckk.ppjwa.cn

TS:   Math.max(...arr);
来源：http://jky.gzhubu.top

Java: Collections.max(list);  Collections.min(list);
来源：http://dmq.pengpengdd.cyou

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ecl.kuanghao11.cn

Ruby: arr.max;  arr.min
来源：http://xnk.hongshengwenyu.top

C#:   list.Max();  list.Min()
来源：http://nyk.andypj.xyz

[D18] 扁平化嵌套数组
来源：http://tlv.hywenlv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lix.sxryk.cn

PHP:  array_merge(...$nested);
来源：http://bep.nanxinkj.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gvc.vehdjk.com

TS:   nested.flat();
来源：http://liz.cucudq.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kbr.jinyuanbaomall.cn

Go:   // 手写双层循环
来源：http://zvf.snrcjt.cn

Ruby: nested.flatten
来源：http://gkf.nwbrower.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://skz.xuanzx.com

[D19] 按字段分组
来源：http://ark.nanxinkj.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hbq.smart0.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gfz.iojbl.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xdc.ybcxt.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://btn.zhoulong.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fzx.yj20258888.top

Go:   // 手写 map[string][]T
来源：http://vfm.shangyingyoupin.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://rfn.smart0.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://inx.hnxiangtu.top

[D20] 统计每个元素出现次数
来源：http://vuh.snrcjt.cn

Py:   Counter(arr)
来源：http://kcu.vehdjk.com

PHP:  array_count_values($arr);
来源：http://pgo.yj20258.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jvt.svipenyu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ezk.chenjidiqi.icu

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tqp.hongshengwenyu.top

Go:   // 手写 map[T]int
来源：http://pwq.xuetiantiany.cn

Ruby: arr.tally
来源：http://dyl.jinyuanbaomall.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hmg.hnqzz.top

[D21] 判断是否包含某元素
来源：http://sqb.wangdashe.top

Py:   x in arr
来源：http://fbc.redwolf501.top

PHP:  in_array($x, $arr, true);
来源：http://sor.smart0.xyz

JS:   arr.includes(x)
来源：http://bdz.zhoulong.xyz

TS:   arr.includes(x)
来源：http://tww.xuetiantiany.cn

Java: list.contains(x)
来源：http://ywh.wangshuangyany.cn

Go:   slices.Contains(arr, x)
来源：http://ckr.zhengqikj.top

Ruby: arr.include?(x)
来源：http://tmw.hnxiangtu.top

C#:   list.Contains(x)
来源：http://fdm.hnxiangtu.top

[D22] 复制数组（避免共享引用）
来源：http://gbi.cdnleiting.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gox.ctjpmb.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yqv.yangfankeji.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wvt.chenzaomai.com

TS:   [...arr];
来源：http://xxg.jinyuanbaomall.cn

Java: new ArrayList<>(list);
来源：http://puj.hesvh.cn

Go:   copied := append([]int(nil), arr...)
来源：http://kim.zycfv.cn

Ruby: arr.dup;  arr.clone
来源：http://xxl.sweek.top

C#:   new List<int>(list);
来源：http://jnw.jyoumei.cn

[D23] reduce 累积计算
来源：http://vvj.uphjek.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hdr.sufxvd.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gnh.9152youxi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ebv.zhoulong.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wyx.bjfxy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://xvr.tian-w.cn

Go:   // 手写循环
来源：http://poq.sysykeji.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mkd.xuanzx.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://und.zhaomingkeji.xyz

[D24] 字典 / Map 基本操作
来源：http://wzx.redwolf501.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uok.pycfn.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zkb.gaohongyu789.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fke.fzhhl.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yqj.svipenyu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://skj.shuidangran.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jlf.jqgfzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kin.fzhhl.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lle.tarul.cn

[D25] Set 集合去重与交并差
来源：http://rcm.shzxlz.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hbu.52xcode.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pnm.chenzaomai.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ily.redwolf501.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jlp.fzhhl.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gqp.sweek.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hxj.ctjpmb.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nel.snrcjt.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zip.jinqigufen.top

[D26] 数组转字符串
来源：http://pxc.yj20258888.top

Py:   ", ".join(map(str, arr))
来源：http://dng.ivvv.top

PHP:  implode(", ", $arr);
来源：http://fle.cashguo.top

JS:   arr.join(", ")
来源：http://ukg.gogol.net.cn

TS:   arr.join(", ")
来源：http://ydw.hongshengwenyu.top


<!-- 参考信息 -->