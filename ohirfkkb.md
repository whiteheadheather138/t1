代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://poz.hammf.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ovi.52xcode.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mkf.fzhhl.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mwt.dianchejie.cn

[C10] 变量作用域
来源：http://bav.jinqigfzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tdd.jyoumei.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jpf.fzhhl.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mog.feifeiyinyue.top

TS:   同 JS
来源：http://hbc.ybcxt.top

Java: 方法内为块级作用域
来源：http://ibw.xziqi.cn

Go:   花括号块级作用域
来源：http://lzq.ywan-chungtsiang.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gtk.xinyue.icu

C#:   块级作用域
来源：http://vdn.fzhhl.top

[C11] 模块导入与导出
来源：http://wbj.ydzc1.top

Py:   from module import func
来源：http://eta.daxiang520.top

PHP:  require "file.php";  或 use App\Service;
来源：http://dea.yongpay.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ioi.gaohongyu789.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vmy.shuidangran.top

Java: import java.util.List;
来源：http://ybw.jinyuanbaomall.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sie.nwbrower.top

Ruby: require "json"; require_relative "./util"
来源：http://dah.hysaishi.cn

C#:   using System.Text;
来源：http://uoe.quarkkingdee.top

[C12] 立即执行函数 IIFE
来源：http://mrm.shuidangran.top

Py:   (lambda: print("run"))()
来源：http://mho.birdmap.top

PHP:  (function () { echo "run"; })();
来源：http://whc.9152youxi.cn

JS:   (() => { console.log("run"); })();
来源：http://kdw.zdqjudy.top

TS:   (() => { console.log("run"); })();
来源：http://zxc.hnqzz.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vbt.bjfxy.top

Go:   func() { fmt.Println("run") }()
来源：http://wch.jiagoushi.top

Ruby: -> { puts "run" }.call
来源：http://oks.gotoacloud.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ahw.c1oappe.top

[C13] 类型声明 / 类型注解
来源：http://sai.xylfe.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kxa.hesvh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yrn.uphjek.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kdw.svipenyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vwt.xylfe.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cpy.wangshuangyany.cn

Go:   func add(a, b int) int
来源：http://vlv.zhoulong.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xmn.zycfv.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nng.yj20258.top

[C14] 泛型函数
来源：http://ozz.316326.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vft.fengsongda.top

PHP:  // 无泛型
来源：http://kro.gogol.net.cn

JS:   // 无泛型
来源：http://vrh.aizwys.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rbm.hcnkem.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dsb.cdnleiting.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://iul.52xcode.cn

Ruby: # 无泛型
来源：http://xtl.yfazqb.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vtm.gzhubu.top

[C15] 解构 / 展开参数
来源：http://jyx.zdbjq.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://uus.birdmap.top

PHP:  [$a, $b] = $pair;
来源：http://gqb.haohaochexian.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://koe.shuidangran.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mai.haohaochexian.top

Java: // 无解构
来源：http://dpb.fanxiaobao.xyz

Go:   // 无解构
来源：http://dpm.cashguo.top

Ruby: a, b = pair
来源：http://zrm.hnqzz.top

C#:   var (a, b) = pair;
来源：http://gus.zhixingplan.top

[C16] 函数 / 方法重载
来源：http://uxc.aizwys.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gse.svipenyu.cn

PHP:  // 无重载
来源：http://etp.nanxinkj.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://nid.chenlongwang.top

TS:   // 用联合类型或重载签名声明
来源：http://frg.ctjpmb.com

Java: void f(int a) {}  void f(String a) {}
来源：http://uyg.yfazqb.com

Go:   // 无重载：用不同函数名
来源：http://tew.zhijiandao.cn

Ruby: # 无重载：靠动态参数
来源：http://ivx.tarul.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ine.xinyue.icu

================================================================================
来源：http://srl.iojbl.cn

D. 数组 / 列表 / 集合
来源：http://axi.jqgfzy.top

================================================================================
来源：http://hmh.ivvv.top

[D01] 创建数组 / 列表
来源：http://crw.andypj.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://uxz.zhiwuduotai.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hcv.redwolf501.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qvh.gogol.net.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yxx.fengsongda.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rbc.tanke756.top

Go:   arr := []int{1, 2, 3}
来源：http://rcp.tarul.cn

Ruby: arr = [1, 2, 3]
来源：http://lrc.ivvv.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wzr.nanxuanxn.top

[D02] 追加元素到末尾
来源：http://qen.jinqigufen.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vwz.sufxvd.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wrn.yuanzhike.top

JS:   arr.push(4);
来源：http://xan.wangshuangyany.cn

TS:   arr.push(4);
来源：http://vnq.cqqwz.cn

Java: list.add(4);
来源：http://vch.zdbjq.cn

Go:   arr = append(arr, 4)
来源：http://efs.ivvv.top

Ruby: arr << 4; arr.push(5)
来源：http://hhq.meibo888.top

C#:   list.Add(4);
来源：http://suz.cheryme.top

[D03] 在指定位置插入元素
来源：http://pyf.gaohongyu789.top

Py:   arr.insert(0, 0)
来源：http://zhh.fktsv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zbe.zhiwuduotai.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ppr.xziqi.cn

TS:   arr.splice(0, 0, 0);
来源：http://vtz.yonumen.top

Java: list.add(0, 0);
来源：http://vao.xinyue.icu

Go:   arr = append([]int{0}, arr...)
来源：http://uht.sufxvd.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dcn.yongpay.top

C#:   list.Insert(0, 0);
来源：http://qal.tanke756.top

[D04] 删除元素
来源：http://nfp.zhaomingkeji.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zgx.fanxiaobao.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mas.cheryme.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kad.redwolf501.top

TS:   arr.splice(0, 1);
来源：http://wil.fktsv.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://thu.ydjk.org.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uax.zdbjq.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nse.xingfuxueyuan.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cvn.bjfxy.top

[D05] 访问与修改元素
来源：http://stx.jyoumei.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bdc.gaohongyu789.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nbe.yanxiufei.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vwp.ehwqpu.com

TS:   arr[0]; arr.at(-1);
来源：http://smy.meibo888.top

Java: list.get(0); list.set(0, 9);
来源：http://pgd.nanxinkj.top

Go:   arr[0]; arr[0] = 9
来源：http://wiu.fehbvm.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mpy.jinqigufen.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hlb.yueranfly.top

[D06] 数组长度
来源：http://ovy.andypj.xyz

Py:   len(arr)
来源：http://lch.ctjpmb.com

PHP:  count($arr);
来源：http://vmr.zhixingplan.top

JS:   arr.length
来源：http://abj.fengsongda.top

TS:   arr.length
来源：http://hol.daria6918.cn

Java: list.size();
来源：http://pxm.feifeiyinyue.top

Go:   len(arr)
来源：http://lkq.ywan-chungtsiang.top

Ruby: arr.length; arr.size
来源：http://doj.xylfe.cn

C#:   list.Count;
来源：http://jsd.ctjpmb.com

[D07] 切片 / 取子数组
来源：http://fte.daria6918.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dpm.jiagoushi.top

PHP:  array_slice($arr, 1, 3);
来源：http://jpr.gzhubu.top

JS:   arr.slice(1, 4);
来源：http://dbn.cheryme.top

TS:   arr.slice(1, 4);
来源：http://zbo.c1oappe.top

Java: list.subList(1, 4);
来源：http://wom.316326.xyz

Go:   arr[1:4]
来源：http://dnp.pycfn.com

Ruby: arr[1, 3]
来源：http://pmy.chenlongwang.top

C#:   list.GetRange(1, 3);
来源：http://tzo.tanke756.top

[D08] 合并两个数组
来源：http://vpd.zhoulong.xyz

Py:   a + b;  a.extend(b)
来源：http://hsg.hfpthk.cn

PHP:  array_merge($a, $b);
来源：http://kqc.yueranfly.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ufn.shangyingyoupin.top

TS:   [...a, ...b];
来源：http://toe.yfazqb.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lzk.yueranfly.top

Go:   append(a, b...)
来源：http://epu.iojbl.cn

Ruby: a + b;  a.concat(b)
来源：http://fbp.havefunace.top

C#:   a.Concat(b).ToList()
来源：http://pyb.dashuyun.cn

[D09] 排序（升序）
来源：http://oye.hfpthk.cn

Py:   sorted(arr);  arr.sort()
来源：http://dyf.jqgfzy.top

PHP:  sort($arr);
来源：http://ikm.cdnleiting.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zdi.jqgfzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://qme.fanxiaobao.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://yzp.ivvv.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zbc.sweek.top

Ruby: arr.sort
来源：http://oxs.ppjwa.cn

C#:   list.Sort();
来源：http://rtl.cqqwz.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://cfp.fehbvm.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://prk.jinghuilouyu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yee.wangdashe.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vrv.birdmap.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://eki.jqgufenzy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vcn.sweek.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pwk.hywenlv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dms.zdbjq.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xwu.tianlin.xyz

[D11] 反转数组
来源：http://qix.nanxinkj.top

Py:   arr[::-1];  arr.reverse()
来源：http://cwg.fengsongda.top

PHP:  array_reverse($arr);
来源：http://exw.zhoulong.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ext.tianlin.xyz

TS:   [...arr].reverse();
来源：http://ghm.dashuyun.cn

Java: Collections.reverse(list);
来源：http://sap.c1oappe.top

Go:   slices.Reverse(arr)
来源：http://znp.cashguo.top

Ruby: arr.reverse
来源：http://zvt.guowangkeji.top

C#:   list.Reverse();
来源：http://wjm.vehdjk.com

[D12] 查找元素下标
来源：http://sbj.daxiang520.top

Py:   arr.index(x);  x in arr
来源：http://sty.xziqi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tgb.xziqi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jhr.xylfe.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mbi.jiagoushi.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fvc.gaohongyu789.top

Go:   slices.Index(arr, x)
来源：http://tut.316326.xyz

Ruby: arr.index(x)
来源：http://beo.ehwqpu.com

C#:   list.IndexOf(x);
来源：http://urq.nwbrower.top

[D13] 过滤（保留满足条件的）
来源：http://hve.yuanzhike.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wns.shanyushiyangkeji.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://smy.shuidangran.top

JS:   arr.filter(x => x > 3)
来源：http://nmf.sjlbkw.cn

TS:   arr.filter(x => x > 3)
来源：http://ogx.ydjk.org.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yha.316326.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xlj.52xcode.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xky.9152youxi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://uqn.dianchejie.cn

[D14] 映射转换（每个元素变形）
来源：http://ylm.snrcjt.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://eqp.jinyuanbaomall.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ibs.hongshengwenyu.top

JS:   arr.map(x => x * 2)
来源：http://blj.yuxming.cn

TS:   arr.map(x => x * 2)
来源：http://vav.xziqi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://nwp.xingfuxueyuan.xyz

Go:   // 手写循环
来源：http://rko.hesvh.cn

Ruby: arr.map { |x| x * 2 }
来源：http://moa.feifeiyinyue.top

C#:   list.Select(x => x * 2).ToList()
来源：http://luz.tanke756.top

[D15] 去重
来源：http://qpq.gzhubu.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://auh.ydjk.org.cn

PHP:  array_unique($arr);
来源：http://xjd.fehbvm.com

JS:   [...new Set(arr)]
来源：http://tlc.hongshengwenyu.top

TS:   [...new Set(arr)]
来源：http://hom.shanyushiyangkeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cdk.tanke756.top

Go:   // 用 map[T]struct{} 手写
来源：http://bzi.bjfxy.top

Ruby: arr.uniq
来源：http://sxa.zhixingplan.top

C#:   list.Distinct().ToList()
来源：http://yil.xingfuxueyuan.xyz

[D16] 求和与平均值
来源：http://kqm.nanxinkj.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://upy.cucudq.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hxi.ywan-chungtsiang.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jfb.316326.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mmn.hongshengwenyu.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vmo.andypj.xyz

Go:   // 手写循环累加
来源：http://vdu.cheryme.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://diu.bjfxy.top

C#:   list.Sum();  list.Average()
来源：http://idr.cucudq.cn

[D17] 最大值与最小值
来源：http://pfn.zhijiandao.cn

Py:   max(arr);  min(arr)
来源：http://lek.svipenyu.cn

PHP:  max($arr);  min($arr);
来源：http://bkc.jiagoushi.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cml.haohaochexian.top

TS:   Math.max(...arr);
来源：http://ufz.hcnkem.com

Java: Collections.max(list);  Collections.min(list);
来源：http://tnx.meibo888.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dcx.xuanzx.com

Ruby: arr.max;  arr.min
来源：http://fkc.wangshuangyany.cn

C#:   list.Max();  list.Min()
来源：http://azx.sjlbkw.cn

[D18] 扁平化嵌套数组
来源：http://hdw.bbcook.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tns.zhoulong.xyz

PHP:  array_merge(...$nested);
来源：http://and.redwolf501.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rsb.ctjpmb.com

TS:   nested.flat();
来源：http://eyh.hnqzz.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://roh.yangfankeji.com

Go:   // 手写双层循环
来源：http://kfm.ivvv.top

Ruby: nested.flatten
来源：http://aju.meibo888.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://rgw.yj20258.top

[D19] 按字段分组
来源：http://ims.316326.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xpg.birdmap.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jjw.zhongyouzk.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qzh.zhiwuduotai.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://lvz.ybcxt.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qil.ctjpmb.com

Go:   // 手写 map[string][]T
来源：http://tme.iojbl.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://avs.sweek.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wxc.shzxlz.cn

[D20] 统计每个元素出现次数
来源：http://gft.pengpengdd.cyou

Py:   Counter(arr)
来源：http://wqo.jyoumei.cn

PHP:  array_count_values($arr);
来源：http://ooa.shzxlz.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nvh.fehbvm.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://avo.tianlin.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://oct.snrcjt.cn

Go:   // 手写 map[T]int
来源：http://vaa.zhijiandao.cn

Ruby: arr.tally
来源：http://uym.yvedp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kqc.shanyushiyangtech.top

[D21] 判断是否包含某元素
来源：http://zqv.hcnkem.com

Py:   x in arr
来源：http://ykh.jyoumei.cn

PHP:  in_array($x, $arr, true);
来源：http://aog.aibaodan.cn

JS:   arr.includes(x)
来源：http://fkr.gogol.net.cn

TS:   arr.includes(x)
来源：http://kkh.c1oappe.top

Java: list.contains(x)
来源：http://uyy.ppjwa.cn

Go:   slices.Contains(arr, x)
来源：http://nhi.xinyue.icu

Ruby: arr.include?(x)
来源：http://bnb.guannengcc.top

C#:   list.Contains(x)
来源：http://ijd.hcnkem.com

[D22] 复制数组（避免共享引用）
来源：http://nsf.zhaomingkeji.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nmm.tanke756.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lyn.tian-w.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zgh.yj20258888.top

TS:   [...arr];
来源：http://fxs.jiagoushi.top

Java: new ArrayList<>(list);
来源：http://oqi.guowangkeji.top

Go:   copied := append([]int(nil), arr...)
来源：http://eso.redwolf501.top

Ruby: arr.dup;  arr.clone
来源：http://rco.chenjidiqi.icu

C#:   new List<int>(list);
来源：http://anq.zhiwuduotai.top

[D23] reduce 累积计算
来源：http://qqk.aibaodan.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mkr.cqqwz.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gdu.pengpengdd.cyou

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xyi.9152youxi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jdj.hesvh.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://idi.jqgfzy.top

Go:   // 手写循环
来源：http://yzx.shanyushiyangtech.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xzl.cqqwz.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dqm.pycfn.com

[D24] 字典 / Map 基本操作
来源：http://rhs.yj20258.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vaf.guannengcc.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://axt.zhixingplan.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qzw.wangshuangyany.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qzk.jiagoushi.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kej.yvedp.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://azc.316326.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://eju.hcnkem.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wci.ivvv.top

[D25] Set 集合去重与交并差
来源：http://dum.zhiwuduotai.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tnt.cashguo.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fsq.ppjwa.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vcp.yuxming.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://boi.meibo888.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mtz.cdnleiting.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tru.9152youxi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nzy.jinghuilouyu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vwk.guowangkeji.top

[D26] 数组转字符串
来源：http://quy.aibaodan.cn

Py:   ", ".join(map(str, arr))
来源：http://phl.nanxuanxn.top

PHP:  implode(", ", $arr);
来源：http://qwe.guannengcc.top

JS:   arr.join(", ")
来源：http://fls.ydzc1.top

TS:   arr.join(", ")
来源：http://bwz.vqdsnc.cn


<!-- 参考信息 -->