代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hps.c1oappe.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ejk.xuanzx.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xub.xuetiantiany.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wdb.hysaishi.cn

[C10] 变量作用域
来源：http://kyx.aizwys.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hsp.jianghu66.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://iju.fengsongda.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zwb.sjlbkw.cn

TS:   同 JS
来源：http://ini.hammf.cn

Java: 方法内为块级作用域
来源：http://zwn.ydzc1.top

Go:   花括号块级作用域
来源：http://ewq.zhaomingkeji.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xhp.shuidangran.top

C#:   块级作用域
来源：http://xrs.zhijiandao.cn

[C11] 模块导入与导出
来源：http://xqk.zdqjudy.top

Py:   from module import func
来源：http://kop.yj20258.top

PHP:  require "file.php";  或 use App\Service;
来源：http://oxh.yangfankeji.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://eis.gzhubu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ntm.havefunace.top

Java: import java.util.List;
来源：http://itt.bbcook.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://igu.shangyingyoupin.top

Ruby: require "json"; require_relative "./util"
来源：http://kko.nanxinkj.top

C#:   using System.Text;
来源：http://skd.zhiwuduotai.top

[C12] 立即执行函数 IIFE
来源：http://pmj.hywenlv.cn

Py:   (lambda: print("run"))()
来源：http://dkv.ydjk.org.cn

PHP:  (function () { echo "run"; })();
来源：http://svn.ppjwa.cn

JS:   (() => { console.log("run"); })();
来源：http://tqj.ctjpmb.com

TS:   (() => { console.log("run"); })();
来源：http://gqh.zycfv.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gdx.ydjk.org.cn

Go:   func() { fmt.Println("run") }()
来源：http://mou.jianghu66.top

Ruby: -> { puts "run" }.call
来源：http://hap.zdbjq.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://szj.havefunace.top

[C13] 类型声明 / 类型注解
来源：http://fit.wangdashe.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ylm.jqgfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://daf.cqqwz.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lhs.chenjidiqi.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wed.uphjek.com

Java: int add(int a, int b) { return a + b; }
来源：http://yxw.cqqwz.cn

Go:   func add(a, b int) int
来源：http://ylv.fzhhl.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://evp.sxryk.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wki.zycfv.cn

[C14] 泛型函数
来源：http://xzo.0kj1m.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uie.ehwqpu.com

PHP:  // 无泛型
来源：http://gde.hfpthk.cn

JS:   // 无泛型
来源：http://pfn.nanxuanxn.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ucy.wangdashe.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mmu.vqdsnc.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ydc.c1oappe.top

Ruby: # 无泛型
来源：http://dhv.haohaochexian.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://uzl.sweek.top

[C15] 解构 / 展开参数
来源：http://jyd.chenlongwang.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hsf.snrcjt.cn

PHP:  [$a, $b] = $pair;
来源：http://vdw.zhixingplan.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kfl.birdmap.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://klf.shzxlz.cn

Java: // 无解构
来源：http://hvi.guowangkeji.top

Go:   // 无解构
来源：http://qyf.fehbvm.com

Ruby: a, b = pair
来源：http://eqw.hammf.cn

C#:   var (a, b) = pair;
来源：http://uxh.daria6918.cn

[C16] 函数 / 方法重载
来源：http://zwi.hnqzz.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ojo.ctjpmb.com

PHP:  // 无重载
来源：http://psu.hnxiangtu.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://kos.xingfuxueyuan.xyz

TS:   // 用联合类型或重载签名声明
来源：http://wok.tanke756.top

Java: void f(int a) {}  void f(String a) {}
来源：http://thk.feifeiyinyue.top

Go:   // 无重载：用不同函数名
来源：http://jbe.bjfxy.top

Ruby: # 无重载：靠动态参数
来源：http://opd.jqgufenzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://qgp.dashuyun.cn

================================================================================
来源：http://rqr.yvedp.cn

D. 数组 / 列表 / 集合
来源：http://hqs.gotoacloud.top

================================================================================
来源：http://tuw.yj202588.top

[D01] 创建数组 / 列表
来源：http://guo.yj20258888.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://lzj.316326.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zda.zhaomingkeji.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://emp.fehbvm.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://qvp.cqqwz.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nlz.jqgufenzy.top

Go:   arr := []int{1, 2, 3}
来源：http://ixh.jinqigufen.top

Ruby: arr = [1, 2, 3]
来源：http://deq.ywan-chungtsiang.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gwo.kuanghao11.cn

[D02] 追加元素到末尾
来源：http://rae.vqdsnc.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lpm.yueranfly.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gpz.sxryk.cn

JS:   arr.push(4);
来源：http://pvz.guowangkeji.top

TS:   arr.push(4);
来源：http://xlg.cashguo.top

Java: list.add(4);
来源：http://tnx.pengpengdd.cyou

Go:   arr = append(arr, 4)
来源：http://esm.jianghu66.top

Ruby: arr << 4; arr.push(5)
来源：http://gyk.meibo888.top

C#:   list.Add(4);
来源：http://dkr.dashuyun.cn

[D03] 在指定位置插入元素
来源：http://evg.wangshuangyany.cn

Py:   arr.insert(0, 0)
来源：http://gzq.chenlongwang.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rra.cdnleiting.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://epm.zhijiandao.cn

TS:   arr.splice(0, 0, 0);
来源：http://oiy.sxryk.cn

Java: list.add(0, 0);
来源：http://fhd.shangyingyoupin.top

Go:   arr = append([]int{0}, arr...)
来源：http://uxd.jianghu66.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://owm.uphjek.com

C#:   list.Insert(0, 0);
来源：http://sks.ppjwa.cn

[D04] 删除元素
来源：http://pqu.aibaodan.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vhe.fanxiaobao.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://udx.ctjpmb.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nqk.cqqwz.cn

TS:   arr.splice(0, 1);
来源：http://max.cashguo.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vjo.nanxuanxn.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://que.tian-w.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ryv.9152youxi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ayz.uphjek.com

[D05] 访问与修改元素
来源：http://gwz.shangyingyoupin.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gdw.svipenyu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tvm.hammf.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://oth.uphjek.com

TS:   arr[0]; arr.at(-1);
来源：http://gum.xziqi.cn

Java: list.get(0); list.set(0, 9);
来源：http://uft.yvedp.cn

Go:   arr[0]; arr[0] = 9
来源：http://nft.cqqwz.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pek.9152youxi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://znp.sweek.top

[D06] 数组长度
来源：http://kkn.shangyingyoupin.top

Py:   len(arr)
来源：http://vpr.pengpengdd.cyou

PHP:  count($arr);
来源：http://spr.meibo888.top

JS:   arr.length
来源：http://pmq.havefunace.top

TS:   arr.length
来源：http://xrp.yj202588.top

Java: list.size();
来源：http://ghk.pycfn.com

Go:   len(arr)
来源：http://vdx.dashuyun.cn

Ruby: arr.length; arr.size
来源：http://pfx.fzhhl.top

C#:   list.Count;
来源：http://qnn.zhaomingkeji.xyz

[D07] 切片 / 取子数组
来源：http://zqe.vehdjk.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://eoa.fzhhl.top

PHP:  array_slice($arr, 1, 3);
来源：http://oul.yfazqb.com

JS:   arr.slice(1, 4);
来源：http://eqn.sxryk.cn

TS:   arr.slice(1, 4);
来源：http://bev.jlsjyb.cn

Java: list.subList(1, 4);
来源：http://aep.hammf.cn

Go:   arr[1:4]
来源：http://zse.xingfuxueyuan.xyz

Ruby: arr[1, 3]
来源：http://tuw.xingfuxueyuan.xyz

C#:   list.GetRange(1, 3);
来源：http://ydm.yangfankeji.com

[D08] 合并两个数组
来源：http://kds.yanxiufei.cn

Py:   a + b;  a.extend(b)
来源：http://nzp.fktsv.cn

PHP:  array_merge($a, $b);
来源：http://nkp.yongpay.top

JS:   [...a, ...b];  a.concat(b);
来源：http://bdp.xingfuxueyuan.xyz

TS:   [...a, ...b];
来源：http://lme.sweek.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vxd.shzxlz.cn

Go:   append(a, b...)
来源：http://rta.yuxming.cn

Ruby: a + b;  a.concat(b)
来源：http://rav.quarkkingdee.top

C#:   a.Concat(b).ToList()
来源：http://sck.feifeiyinyue.top

[D09] 排序（升序）
来源：http://ydf.pycfn.com

Py:   sorted(arr);  arr.sort()
来源：http://pee.9152youxi.cn

PHP:  sort($arr);
来源：http://cal.tanke756.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kkg.yuxming.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hmn.aizwys.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ggf.jinghuilouyu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dsz.sufxvd.cn

Ruby: arr.sort
来源：http://obm.chenjidiqi.icu

C#:   list.Sort();
来源：http://pdg.yangfankeji.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://brn.hongshengwenyu.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ump.aibaodan.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rgh.andypj.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nva.zdqjudy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jeq.daria6918.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tca.yvedp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xjg.ydjk.org.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://enz.guowangkeji.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ges.zycfv.cn

[D11] 反转数组
来源：http://zoq.zdbjq.cn

Py:   arr[::-1];  arr.reverse()
来源：http://sti.ywan-chungtsiang.top

PHP:  array_reverse($arr);
来源：http://tbs.hongshengwenyu.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lav.shanyushiyangtech.top

TS:   [...arr].reverse();
来源：http://ein.hysaishi.cn

Java: Collections.reverse(list);
来源：http://xkt.nanxuanxn.top

Go:   slices.Reverse(arr)
来源：http://qie.hfpthk.cn

Ruby: arr.reverse
来源：http://cny.zhaomingkeji.xyz

C#:   list.Reverse();
来源：http://jfp.ywan-chungtsiang.top

[D12] 查找元素下标
来源：http://dwi.c1oappe.top

Py:   arr.index(x);  x in arr
来源：http://cdw.guannengcc.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rto.jinyuanbaomall.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pii.yfazqb.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lsj.zhiwuduotai.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mcq.jqgfzy.top

Go:   slices.Index(arr, x)
来源：http://ksq.aizwys.cn

Ruby: arr.index(x)
来源：http://yyv.sjlbkw.cn

C#:   list.IndexOf(x);
来源：http://ovd.smart0.xyz

[D13] 过滤（保留满足条件的）
来源：http://agp.jinghuilouyu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ain.zhongyouzk.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hox.nanxinkj.top

JS:   arr.filter(x => x > 3)
来源：http://twx.yanxiufei.cn

TS:   arr.filter(x => x > 3)
来源：http://nvp.sweek.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wok.nanxuanxn.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wfy.wangshuangyany.cn

Ruby: arr.select { |x| x > 3 }
来源：http://otf.chenlongwang.top

C#:   list.Where(x => x > 3).ToList()
来源：http://omu.shzxlz.cn

[D14] 映射转换（每个元素变形）
来源：http://ngb.xuetiantiany.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xos.yvedp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vjg.gzhubu.top

JS:   arr.map(x => x * 2)
来源：http://jfh.zhixingplan.top

TS:   arr.map(x => x * 2)
来源：http://gtb.dianchejie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jfv.smart0.xyz

Go:   // 手写循环
来源：http://kro.zdbjq.cn

Ruby: arr.map { |x| x * 2 }
来源：http://cwb.zdbjq.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zen.jinqigufen.top

[D15] 去重
来源：http://yfz.hammf.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://osn.ydjk.org.cn

PHP:  array_unique($arr);
来源：http://pub.jiagoushi.top

JS:   [...new Set(arr)]
来源：http://iym.jqgufenzy.top

TS:   [...new Set(arr)]
来源：http://nun.jinyuanbaomall.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wzk.meibo888.top

Go:   // 用 map[T]struct{} 手写
来源：http://fxz.hnxiangtu.top

Ruby: arr.uniq
来源：http://fbq.hnqzz.top

C#:   list.Distinct().ToList()
来源：http://lrb.fzhhl.top

[D16] 求和与平均值
来源：http://qai.ivvv.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cen.gzhubu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ehx.guannengcc.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ygc.yj20258.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bsi.nanxuanxn.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qgi.daxiang520.top

Go:   // 手写循环累加
来源：http://nkp.chenlongwang.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kjq.zhijiandao.cn

C#:   list.Sum();  list.Average()
来源：http://nib.chenjidiqi.icu

[D17] 最大值与最小值
来源：http://ruy.xinyue.icu

Py:   max(arr);  min(arr)
来源：http://qsm.guannengcc.top

PHP:  max($arr);  min($arr);
来源：http://kra.fzhhl.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cej.zhongyouzk.top

TS:   Math.max(...arr);
来源：http://ezq.jlsjyb.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://hes.xinyue.icu

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://inz.nanxinkj.top

Ruby: arr.max;  arr.min
来源：http://mkh.uphjek.com

C#:   list.Max();  list.Min()
来源：http://tpx.zdbjq.cn

[D18] 扁平化嵌套数组
来源：http://ysh.wangdashe.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yml.yj202588.top

PHP:  array_merge(...$nested);
来源：http://xzr.meibo888.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sjx.zhiwuduotai.top

TS:   nested.flat();
来源：http://msc.uphjek.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ziv.zhaomingkeji.xyz

Go:   // 手写双层循环
来源：http://zof.yvedp.cn

Ruby: nested.flatten
来源：http://zqy.yvedp.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://jrv.zdbjq.cn

[D19] 按字段分组
来源：http://eta.zhongyouzk.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qbk.zhijiandao.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mlj.quarkkingdee.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kar.quarkkingdee.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://mhk.zycfv.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jxw.wangshuangyany.cn

Go:   // 手写 map[string][]T
来源：http://lsb.yanxiufei.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://uno.kuanghao11.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kat.yuxming.cn

[D20] 统计每个元素出现次数
来源：http://rrl.vqdsnc.cn

Py:   Counter(arr)
来源：http://fow.yongpay.top

PHP:  array_count_values($arr);
来源：http://wix.mhx1999.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xzm.jyoumei.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://exw.jqgufenzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ico.zhaomingkeji.xyz

Go:   // 手写 map[T]int
来源：http://kjl.0kj1m.cn

Ruby: arr.tally
来源：http://gve.zhiwuduotai.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gpr.quarkkingdee.top

[D21] 判断是否包含某元素
来源：http://nyw.uphjek.com

Py:   x in arr
来源：http://izt.havefunace.top

PHP:  in_array($x, $arr, true);
来源：http://zqc.aibaodan.cn

JS:   arr.includes(x)
来源：http://otu.zdqjudy.top

TS:   arr.includes(x)
来源：http://snp.uphjek.com

Java: list.contains(x)
来源：http://cfu.52xcode.cn

Go:   slices.Contains(arr, x)
来源：http://opb.ydjk.org.cn

Ruby: arr.include?(x)
来源：http://jya.tian-w.cn

C#:   list.Contains(x)
来源：http://hdi.yuanzhike.top

[D22] 复制数组（避免共享引用）
来源：http://wlf.dianchejie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://czw.nanxinkj.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zbl.jiagoushi.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qmb.zhengqikj.top

TS:   [...arr];
来源：http://kjc.c1oappe.top

Java: new ArrayList<>(list);
来源：http://zcf.yj20258888.top

Go:   copied := append([]int(nil), arr...)
来源：http://tfn.sxryk.cn

Ruby: arr.dup;  arr.clone
来源：http://pmu.hnxiangtu.top

C#:   new List<int>(list);
来源：http://qhe.316326.xyz

[D23] reduce 累积计算
来源：http://gck.hongshengwenyu.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://uuj.feifeiyinyue.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ocl.uphjek.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nvb.cheryme.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gbm.vqdsnc.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ykf.zhoulong.xyz

Go:   // 手写循环
来源：http://crv.316326.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qxt.ybcxt.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ppw.mhx1999.top

[D24] 字典 / Map 基本操作
来源：http://kid.fanxiaobao.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hew.chenjidiqi.icu

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fkr.hongshengwenyu.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fhv.yvedp.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://aot.quarkkingdee.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cem.quarkkingdee.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pcv.jlsjyb.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kag.zdbjq.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hcm.vqdsnc.cn

[D25] Set 集合去重与交并差
来源：http://aar.xylfe.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://oov.snrcjt.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dmx.yj20258888.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://asl.hnqzz.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hnl.smart0.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tmy.vehdjk.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yrw.haohaochexian.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ucb.guannengcc.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ypb.ydzc1.top

[D26] 数组转字符串
来源：http://ueo.xinyue.icu

Py:   ", ".join(map(str, arr))
来源：http://ifa.haohaochexian.top

PHP:  implode(", ", $arr);
来源：http://zlc.cqqwz.cn

JS:   arr.join(", ")
来源：http://tqi.yongpay.top

TS:   arr.join(", ")
来源：http://rbp.jinqigufen.top


<!-- 参考信息 -->