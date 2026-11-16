代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qry.haohaochexian.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qqo.bjfxy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wmo.chenzaomai.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hgl.0kj1m.cn

[C10] 变量作用域
来源：http://wyd.jinghuilouyu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rkz.gaohongyu789.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qeq.hfpthk.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://acm.tanke756.top

TS:   同 JS
来源：http://ccx.sxryk.cn

Java: 方法内为块级作用域
来源：http://kqb.fzhhl.top

Go:   花括号块级作用域
来源：http://voi.yuxming.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xyi.yongpay.top

C#:   块级作用域
来源：http://poa.yangfankeji.com

[C11] 模块导入与导出
来源：http://ecl.aizwys.cn

Py:   from module import func
来源：http://smn.chenzaomai.com

PHP:  require "file.php";  或 use App\Service;
来源：http://otj.ctjpmb.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://uly.yongpay.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bdt.hongshengwenyu.top

Java: import java.util.List;
来源：http://sjb.shuidangran.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ttp.jinyuanbaomall.cn

Ruby: require "json"; require_relative "./util"
来源：http://fku.9152youxi.cn

C#:   using System.Text;
来源：http://hiu.guowangkeji.top

[C12] 立即执行函数 IIFE
来源：http://vpp.zdbjq.cn

Py:   (lambda: print("run"))()
来源：http://gug.hfpthk.cn

PHP:  (function () { echo "run"; })();
来源：http://fab.316326.xyz

JS:   (() => { console.log("run"); })();
来源：http://ira.jqgfzy.top

TS:   (() => { console.log("run"); })();
来源：http://ffn.nwbrower.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vts.hesvh.cn

Go:   func() { fmt.Println("run") }()
来源：http://kgn.yvedp.cn

Ruby: -> { puts "run" }.call
来源：http://bng.fzhhl.top

C#:   // 无 IIFE：用静态构造函数
来源：http://fzi.xinyue.icu

[C13] 类型声明 / 类型注解
来源：http://mlc.shzxlz.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qun.meibo888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vbw.chenlongwang.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rnn.xziqi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://byt.shzxlz.cn

Java: int add(int a, int b) { return a + b; }
来源：http://byc.daxiang520.top

Go:   func add(a, b int) int
来源：http://hik.tian-w.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nmj.zhongyouzk.top

C#:   int Add(int a, int b) => a + b;
来源：http://bzg.guannengcc.top

[C14] 泛型函数
来源：http://jaa.quarkkingdee.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://emj.fanxiaobao.xyz

PHP:  // 无泛型
来源：http://ynv.pengpengdd.cyou

JS:   // 无泛型
来源：http://lcm.tanke756.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://abi.jlsjyb.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zpf.jinqigufen.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ypi.zycfv.cn

Ruby: # 无泛型
来源：http://iab.hesvh.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fno.0kj1m.cn

[C15] 解构 / 展开参数
来源：http://ukj.zhixingplan.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://aiq.yfazqb.com

PHP:  [$a, $b] = $pair;
来源：http://ksi.dianchejie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://oly.aizwys.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xwm.tian-w.cn

Java: // 无解构
来源：http://iyf.zhiwuduotai.top

Go:   // 无解构
来源：http://xch.ehwqpu.com

Ruby: a, b = pair
来源：http://jfh.zhijiandao.cn

C#:   var (a, b) = pair;
来源：http://kip.nanxuanxn.top

[C16] 函数 / 方法重载
来源：http://zrj.gogol.net.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hbh.zhengqikj.top

PHP:  // 无重载
来源：http://dqb.snrcjt.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ptj.epnwcf.com

TS:   // 用联合类型或重载签名声明
来源：http://ghp.hfpthk.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://kcd.mhx1999.top

Go:   // 无重载：用不同函数名
来源：http://gra.zhengqikj.top

Ruby: # 无重载：靠动态参数
来源：http://yej.yuanzhike.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://osh.bbcook.cn

================================================================================
来源：http://xct.sjlbkw.cn

D. 数组 / 列表 / 集合
来源：http://mbh.zhongyouzk.top

================================================================================
来源：http://gix.hongshengwenyu.top

[D01] 创建数组 / 列表
来源：http://xug.wangshuangyany.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://yqi.shuidangran.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tbw.yueranfly.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hra.jinqigfzy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://jpo.yvedp.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fas.cashguo.top

Go:   arr := []int{1, 2, 3}
来源：http://spa.tian-w.cn

Ruby: arr = [1, 2, 3]
来源：http://vca.hcnkem.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://emk.316326.xyz

[D02] 追加元素到末尾
来源：http://oix.nanxuanxn.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://loz.zhijiandao.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ioe.svipenyu.cn

JS:   arr.push(4);
来源：http://gwy.jqgfzy.top

TS:   arr.push(4);
来源：http://bob.shangyingyoupin.top

Java: list.add(4);
来源：http://ujt.smart0.xyz

Go:   arr = append(arr, 4)
来源：http://sfo.shuidangran.top

Ruby: arr << 4; arr.push(5)
来源：http://hpo.jinqigfzy.top

C#:   list.Add(4);
来源：http://czv.cashguo.top

[D03] 在指定位置插入元素
来源：http://gwc.yvedp.cn

Py:   arr.insert(0, 0)
来源：http://grw.dianchejie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hol.ydzc1.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fel.vehdjk.com

TS:   arr.splice(0, 0, 0);
来源：http://sao.yonumen.top

Java: list.add(0, 0);
来源：http://iwu.vqdsnc.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mvk.zhongyouzk.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tpx.smart0.xyz

C#:   list.Insert(0, 0);
来源：http://csg.gogol.net.cn

[D04] 删除元素
来源：http://sbm.meibo888.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kwr.yanxiufei.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dqa.yfazqb.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wfz.xingfuxueyuan.xyz

TS:   arr.splice(0, 1);
来源：http://uoi.yuxming.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fmk.jianghu66.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ove.ppjwa.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://llu.c1oappe.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://miz.52xcode.cn

[D05] 访问与修改元素
来源：http://lgv.9152youxi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xlp.sxryk.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sgu.vqdsnc.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://skv.cheryme.top

TS:   arr[0]; arr.at(-1);
来源：http://zwq.xziqi.cn

Java: list.get(0); list.set(0, 9);
来源：http://dvl.xziqi.cn

Go:   arr[0]; arr[0] = 9
来源：http://pyn.vehdjk.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fsf.snrcjt.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wqe.havefunace.top

[D06] 数组长度
来源：http://tcu.yfazqb.com

Py:   len(arr)
来源：http://atj.daria6918.cn

PHP:  count($arr);
来源：http://zps.svipenyu.cn

JS:   arr.length
来源：http://myi.daria6918.cn

TS:   arr.length
来源：http://pwc.xinyue.icu

Java: list.size();
来源：http://zrk.sweek.top

Go:   len(arr)
来源：http://bln.daxiang520.top

Ruby: arr.length; arr.size
来源：http://jkm.cqqwz.cn

C#:   list.Count;
来源：http://gcv.xingfuxueyuan.xyz

[D07] 切片 / 取子数组
来源：http://rsk.bjfxy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jmq.hcnkem.com

PHP:  array_slice($arr, 1, 3);
来源：http://aks.52xcode.cn

JS:   arr.slice(1, 4);
来源：http://yeq.bjfxy.top

TS:   arr.slice(1, 4);
来源：http://njk.yj202588.top

Java: list.subList(1, 4);
来源：http://joe.xuanzx.com

Go:   arr[1:4]
来源：http://rbg.xuetiantiany.cn

Ruby: arr[1, 3]
来源：http://fac.uphjek.com

C#:   list.GetRange(1, 3);
来源：http://dpo.wangdashe.top

[D08] 合并两个数组
来源：http://rab.yvedp.cn

Py:   a + b;  a.extend(b)
来源：http://dop.ctjpmb.com

PHP:  array_merge($a, $b);
来源：http://ghc.jianghu66.top

JS:   [...a, ...b];  a.concat(b);
来源：http://rky.dianchejie.cn

TS:   [...a, ...b];
来源：http://zrk.mhx1999.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mjx.gotoacloud.top

Go:   append(a, b...)
来源：http://psx.redwolf501.top

Ruby: a + b;  a.concat(b)
来源：http://vcu.meibo888.top

C#:   a.Concat(b).ToList()
来源：http://toq.iojbl.cn

[D09] 排序（升序）
来源：http://miy.nanxinkj.top

Py:   sorted(arr);  arr.sort()
来源：http://itu.sweek.top

PHP:  sort($arr);
来源：http://kke.smart0.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yfe.wangshuangyany.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://swz.kuanghao11.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://twe.birdmap.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wru.feifeiyinyue.top

Ruby: arr.sort
来源：http://tyb.gotoacloud.top

C#:   list.Sort();
来源：http://xce.fengsongda.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://gil.ywan-chungtsiang.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wkf.xuetiantiany.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rgd.birdmap.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://adc.guannengcc.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rtl.quarkkingdee.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://flv.ydzc1.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sdv.yuanzhike.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://uar.cucudq.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jyl.jinyuanbaomall.cn

[D11] 反转数组
来源：http://kti.ctjpmb.com

Py:   arr[::-1];  arr.reverse()
来源：http://fbt.cheryme.top

PHP:  array_reverse($arr);
来源：http://ygl.svipenyu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://adc.zhongyouzk.top

TS:   [...arr].reverse();
来源：http://mbp.quarkkingdee.top

Java: Collections.reverse(list);
来源：http://gpq.nanxinkj.top

Go:   slices.Reverse(arr)
来源：http://waz.daria6918.cn

Ruby: arr.reverse
来源：http://hvd.kuanghao11.cn

C#:   list.Reverse();
来源：http://omm.yangfankeji.com

[D12] 查找元素下标
来源：http://lxw.zhijiandao.cn

Py:   arr.index(x);  x in arr
来源：http://elt.ehwqpu.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yxs.andypj.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eux.cucudq.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sgl.epnwcf.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kdu.chenzaomai.com

Go:   slices.Index(arr, x)
来源：http://kgz.nanxuanxn.top

Ruby: arr.index(x)
来源：http://qbc.smart0.xyz

C#:   list.IndexOf(x);
来源：http://jbs.bbcook.cn

[D13] 过滤（保留满足条件的）
来源：http://uxv.gotoacloud.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cyc.zhoulong.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://igf.shanyushiyangkeji.top

JS:   arr.filter(x => x > 3)
来源：http://pee.feifeiyinyue.top

TS:   arr.filter(x => x > 3)
来源：http://wum.shanyushiyangtech.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cre.birdmap.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://obs.jianghu66.top

Ruby: arr.select { |x| x > 3 }
来源：http://wfr.uphjek.com

C#:   list.Where(x => x > 3).ToList()
来源：http://bhz.svipenyu.cn

[D14] 映射转换（每个元素变形）
来源：http://qcr.nanxinkj.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://glj.ivvv.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zry.yuxming.cn

JS:   arr.map(x => x * 2)
来源：http://eie.shanyushiyangtech.top

TS:   arr.map(x => x * 2)
来源：http://piw.iojbl.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://tls.iojbl.cn

Go:   // 手写循环
来源：http://jba.sjlbkw.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bxz.jinyuanbaomall.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dhk.pengpengdd.cyou

[D15] 去重
来源：http://djv.ctjpmb.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://enw.wangshuangyany.cn

PHP:  array_unique($arr);
来源：http://pan.feifeiyinyue.top

JS:   [...new Set(arr)]
来源：http://ryd.smart0.xyz

TS:   [...new Set(arr)]
来源：http://kpa.uphjek.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zbg.sxryk.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zxv.yuxming.cn

Ruby: arr.uniq
来源：http://kxm.hesvh.cn

C#:   list.Distinct().ToList()
来源：http://qsd.316326.xyz

[D16] 求和与平均值
来源：http://zbn.yj20258888.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gjn.sysykeji.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jpa.snrcjt.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ntc.yfazqb.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://aif.epnwcf.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yvp.c1oappe.top

Go:   // 手写循环累加
来源：http://wfp.jlsjyb.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zhp.iojbl.cn

C#:   list.Sum();  list.Average()
来源：http://hsm.uphjek.com

[D17] 最大值与最小值
来源：http://wud.hnxiangtu.top

Py:   max(arr);  min(arr)
来源：http://qai.redwolf501.top

PHP:  max($arr);  min($arr);
来源：http://gtc.yj20258888.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dup.316326.xyz

TS:   Math.max(...arr);
来源：http://wpl.zdqjudy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://vqc.hnqzz.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://uat.jqgfzy.top

Ruby: arr.max;  arr.min
来源：http://mqp.yj20258888.top

C#:   list.Max();  list.Min()
来源：http://xgn.hnxiangtu.top

[D18] 扁平化嵌套数组
来源：http://vsv.zdbjq.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rtg.tarul.cn

PHP:  array_merge(...$nested);
来源：http://ywt.jqgufenzy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mim.tian-w.cn

TS:   nested.flat();
来源：http://cxb.shanyushiyangtech.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yec.xuanzx.com

Go:   // 手写双层循环
来源：http://ysx.fktsv.cn

Ruby: nested.flatten
来源：http://akj.vehdjk.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://ksv.xuetiantiany.cn

[D19] 按字段分组
来源：http://kec.xuetiantiany.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://irk.xuetiantiany.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qik.shzxlz.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://eok.mhx1999.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://whj.yj202588.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bzz.yanxiufei.cn

Go:   // 手写 map[string][]T
来源：http://ljb.hnxiangtu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://qtb.fehbvm.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nel.316326.xyz

[D20] 统计每个元素出现次数
来源：http://omb.guowangkeji.top

Py:   Counter(arr)
来源：http://kzd.nanxuanxn.top

PHP:  array_count_values($arr);
来源：http://bgz.jianghu66.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mzr.hnqzz.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cql.fktsv.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lkg.fktsv.cn

Go:   // 手写 map[T]int
来源：http://eho.nanxuanxn.top

Ruby: arr.tally
来源：http://tod.sxryk.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xlu.pycfn.com

[D21] 判断是否包含某元素
来源：http://xcs.hfpthk.cn

Py:   x in arr
来源：http://uiy.ivvv.top

PHP:  in_array($x, $arr, true);
来源：http://kfg.zhongyouzk.top

JS:   arr.includes(x)
来源：http://gkw.yueranfly.top

TS:   arr.includes(x)
来源：http://het.hnxiangtu.top

Java: list.contains(x)
来源：http://rnj.zhixingplan.top

Go:   slices.Contains(arr, x)
来源：http://vce.gaohongyu789.top

Ruby: arr.include?(x)
来源：http://ydt.redwolf501.top

C#:   list.Contains(x)
来源：http://ltu.zhixingplan.top

[D22] 复制数组（避免共享引用）
来源：http://gxo.tarul.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zdi.aibaodan.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tte.hammf.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pvq.hnqzz.top

TS:   [...arr];
来源：http://uhq.yuanzhike.top

Java: new ArrayList<>(list);
来源：http://vhk.havefunace.top

Go:   copied := append([]int(nil), arr...)
来源：http://vrj.zhijiandao.cn

Ruby: arr.dup;  arr.clone
来源：http://vqd.xylfe.cn

C#:   new List<int>(list);
来源：http://uzm.bjfxy.top

[D23] reduce 累积计算
来源：http://dcc.hcnkem.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jpv.cucudq.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pyg.pengpengdd.cyou

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uyv.52xcode.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ddy.zhongyouzk.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://fst.tianlin.xyz

Go:   // 手写循环
来源：http://knf.xziqi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://obk.yuanzhike.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vkq.zhoulong.xyz

[D24] 字典 / Map 基本操作
来源：http://jef.cucudq.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dcu.fanxiaobao.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zyy.hnxiangtu.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hds.meibo888.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://iry.snrcjt.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mdb.guannengcc.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kel.yangfankeji.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ror.fzhhl.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ywj.meibo888.top

[D25] Set 集合去重与交并差
来源：http://tgq.zdqjudy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kyy.zhixingplan.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mkj.guannengcc.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://uar.yvedp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uat.hongshengwenyu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vll.xingfuxueyuan.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zxj.redwolf501.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://aqx.hysaishi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vxb.yuxming.cn

[D26] 数组转字符串
来源：http://gxk.shanyushiyangtech.top

Py:   ", ".join(map(str, arr))
来源：http://iuy.nanxinkj.top

PHP:  implode(", ", $arr);
来源：http://klg.guannengcc.top

JS:   arr.join(", ")
来源：http://tke.wangdashe.top

TS:   arr.join(", ")
来源：http://fbh.ppjwa.cn


<!-- 参考信息 -->