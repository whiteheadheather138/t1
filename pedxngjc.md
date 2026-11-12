代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nzt.yuxming.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xyg.chenzaomai.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dot.fengsongda.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rcz.iojbl.cn

[C10] 变量作用域
来源：http://lmk.ctjpmb.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hsf.hammf.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kaj.jinyuanbaomall.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://quk.zhoulong.xyz

TS:   同 JS
来源：http://nli.ppjwa.cn

Java: 方法内为块级作用域
来源：http://bnk.cqqwz.cn

Go:   花括号块级作用域
来源：http://ioj.hfpthk.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zyx.ehwqpu.com

C#:   块级作用域
来源：http://lkj.gaohongyu789.top

[C11] 模块导入与导出
来源：http://ann.shanyushiyangtech.top

Py:   from module import func
来源：http://dgj.zhaomingkeji.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://zhc.jinqigufen.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ugn.jinqigufen.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zhg.tianlin.xyz

Java: import java.util.List;
来源：http://xhr.tian-w.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pqe.ehwqpu.com

Ruby: require "json"; require_relative "./util"
来源：http://nwn.pycfn.com

C#:   using System.Text;
来源：http://esh.pengpengdd.cyou

[C12] 立即执行函数 IIFE
来源：http://uok.nanxuanxn.top

Py:   (lambda: print("run"))()
来源：http://cir.vqdsnc.cn

PHP:  (function () { echo "run"; })();
来源：http://fhh.zdqjudy.top

JS:   (() => { console.log("run"); })();
来源：http://wqy.ivvv.top

TS:   (() => { console.log("run"); })();
来源：http://hel.jinyuanbaomall.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://csh.jinyuanbaomall.cn

Go:   func() { fmt.Println("run") }()
来源：http://qmw.gotoacloud.top

Ruby: -> { puts "run" }.call
来源：http://ezz.mhx1999.top

C#:   // 无 IIFE：用静态构造函数
来源：http://vtn.fehbvm.com

[C13] 类型声明 / 类型注解
来源：http://ili.tarul.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://uae.xziqi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ryg.shangyingyoupin.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ypb.meibo888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ikq.hfpthk.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ezx.hesvh.cn

Go:   func add(a, b int) int
来源：http://izc.cheryme.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mjw.hcnkem.com

C#:   int Add(int a, int b) => a + b;
来源：http://uio.aibaodan.cn

[C14] 泛型函数
来源：http://hpc.wangshuangyany.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://alu.hfpthk.cn

PHP:  // 无泛型
来源：http://jjf.ivvv.top

JS:   // 无泛型
来源：http://etc.shanyushiyangkeji.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kus.chenlongwang.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://izi.shzxlz.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gza.ppjwa.cn

Ruby: # 无泛型
来源：http://klg.feifeiyinyue.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lbk.mhx1999.top

[C15] 解构 / 展开参数
来源：http://jwr.hcnkem.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jil.gaohongyu789.top

PHP:  [$a, $b] = $pair;
来源：http://ulw.jqgufenzy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://azw.sxryk.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hvd.ctjpmb.com

Java: // 无解构
来源：http://hsf.jiagoushi.top

Go:   // 无解构
来源：http://bsu.jianghu66.top

Ruby: a, b = pair
来源：http://nmk.nanxinkj.top

C#:   var (a, b) = pair;
来源：http://dlt.hesvh.cn

[C16] 函数 / 方法重载
来源：http://jhw.jinqigufen.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kje.yueranfly.top

PHP:  // 无重载
来源：http://upj.fzhhl.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://liv.zhixingplan.top

TS:   // 用联合类型或重载签名声明
来源：http://rbl.shanyushiyangtech.top

Java: void f(int a) {}  void f(String a) {}
来源：http://lxj.sufxvd.cn

Go:   // 无重载：用不同函数名
来源：http://saq.mhx1999.top

Ruby: # 无重载：靠动态参数
来源：http://tjl.cashguo.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://tkx.wangshuangyany.cn

================================================================================
来源：http://oeo.havefunace.top

D. 数组 / 列表 / 集合
来源：http://htr.jianghu66.top

================================================================================
来源：http://tny.xziqi.cn

[D01] 创建数组 / 列表
来源：http://ggd.quarkkingdee.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://pxh.uphjek.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yil.zhijiandao.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lpt.jyoumei.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://tui.xylfe.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tol.haohaochexian.top

Go:   arr := []int{1, 2, 3}
来源：http://umg.jinqigfzy.top

Ruby: arr = [1, 2, 3]
来源：http://bdc.c1oappe.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vrc.pycfn.com

[D02] 追加元素到末尾
来源：http://bhv.yvedp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://riu.meibo888.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dmc.vehdjk.com

JS:   arr.push(4);
来源：http://pjy.hywenlv.cn

TS:   arr.push(4);
来源：http://cpk.xziqi.cn

Java: list.add(4);
来源：http://iiq.havefunace.top

Go:   arr = append(arr, 4)
来源：http://kqs.jlsjyb.cn

Ruby: arr << 4; arr.push(5)
来源：http://psj.jinghuilouyu.cn

C#:   list.Add(4);
来源：http://qkh.zhoulong.xyz

[D03] 在指定位置插入元素
来源：http://qcv.tianlin.xyz

Py:   arr.insert(0, 0)
来源：http://eqp.iojbl.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gkz.zhiwuduotai.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mxd.sweek.top

TS:   arr.splice(0, 0, 0);
来源：http://jxr.zhoulong.xyz

Java: list.add(0, 0);
来源：http://reg.chenzaomai.com

Go:   arr = append([]int{0}, arr...)
来源：http://ojp.kuanghao11.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://olu.mhx1999.top

C#:   list.Insert(0, 0);
来源：http://sqy.sxryk.cn

[D04] 删除元素
来源：http://ogv.yonumen.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://iqa.chenjidiqi.icu

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://prz.nwbrower.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fxb.fehbvm.com

TS:   arr.splice(0, 1);
来源：http://doc.quarkkingdee.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://brb.jqgufenzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pqx.mhx1999.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nvz.jqgufenzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wfn.sxryk.cn

[D05] 访问与修改元素
来源：http://ilv.uphjek.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qxu.bjfxy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zzz.shangyingyoupin.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yww.aibaodan.cn

TS:   arr[0]; arr.at(-1);
来源：http://czw.sufxvd.cn

Java: list.get(0); list.set(0, 9);
来源：http://ivq.ywan-chungtsiang.top

Go:   arr[0]; arr[0] = 9
来源：http://lqi.zdbjq.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://emd.ydzc1.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xid.52xcode.cn

[D06] 数组长度
来源：http://dbf.hongshengwenyu.top

Py:   len(arr)
来源：http://ybo.fanxiaobao.xyz

PHP:  count($arr);
来源：http://fck.zhiwuduotai.top

JS:   arr.length
来源：http://wxx.shangyingyoupin.top

TS:   arr.length
来源：http://lri.cqqwz.cn

Java: list.size();
来源：http://rsb.gzhubu.top

Go:   len(arr)
来源：http://jsb.yj20258.top

Ruby: arr.length; arr.size
来源：http://lvz.yanxiufei.cn

C#:   list.Count;
来源：http://mzv.nwbrower.top

[D07] 切片 / 取子数组
来源：http://oct.zycfv.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gbu.sysykeji.top

PHP:  array_slice($arr, 1, 3);
来源：http://nkk.zhijiandao.cn

JS:   arr.slice(1, 4);
来源：http://jjx.guowangkeji.top

TS:   arr.slice(1, 4);
来源：http://mgs.fanxiaobao.xyz

Java: list.subList(1, 4);
来源：http://fxp.zhongyouzk.top

Go:   arr[1:4]
来源：http://qzy.cheryme.top

Ruby: arr[1, 3]
来源：http://dbs.fzhhl.top

C#:   list.GetRange(1, 3);
来源：http://tuh.ydzc1.top

[D08] 合并两个数组
来源：http://ujs.shanyushiyangtech.top

Py:   a + b;  a.extend(b)
来源：http://nsn.chenlongwang.top

PHP:  array_merge($a, $b);
来源：http://uwu.yj20258.top

JS:   [...a, ...b];  a.concat(b);
来源：http://zfz.hfpthk.cn

TS:   [...a, ...b];
来源：http://omk.zhijiandao.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vlz.zdqjudy.top

Go:   append(a, b...)
来源：http://sal.aibaodan.cn

Ruby: a + b;  a.concat(b)
来源：http://wey.wangdashe.top

C#:   a.Concat(b).ToList()
来源：http://gak.jiagoushi.top

[D09] 排序（升序）
来源：http://vmy.quarkkingdee.top

Py:   sorted(arr);  arr.sort()
来源：http://ixc.yj20258.top

PHP:  sort($arr);
来源：http://dod.nwbrower.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jld.xuetiantiany.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://elm.daria6918.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xwg.yanxiufei.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uar.ppjwa.cn

Ruby: arr.sort
来源：http://sqz.yanxiufei.cn

C#:   list.Sort();
来源：http://wmh.hesvh.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qkg.jinqigfzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zyi.tian-w.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nes.sxryk.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jrn.9152youxi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://iie.52xcode.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kuf.redwolf501.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nip.pengpengdd.cyou

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cec.cashguo.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cpl.vehdjk.com

[D11] 反转数组
来源：http://zkx.shanyushiyangkeji.top

Py:   arr[::-1];  arr.reverse()
来源：http://rix.bjfxy.top

PHP:  array_reverse($arr);
来源：http://fqm.daxiang520.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xxf.mhx1999.top

TS:   [...arr].reverse();
来源：http://paw.uphjek.com

Java: Collections.reverse(list);
来源：http://ssd.ivvv.top

Go:   slices.Reverse(arr)
来源：http://rcy.sxryk.cn

Ruby: arr.reverse
来源：http://jan.yonumen.top

C#:   list.Reverse();
来源：http://vfw.ywan-chungtsiang.top

[D12] 查找元素下标
来源：http://hmc.havefunace.top

Py:   arr.index(x);  x in arr
来源：http://vmy.dianchejie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tmq.cashguo.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://suo.jlsjyb.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xnh.zhoulong.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gtb.pengpengdd.cyou

Go:   slices.Index(arr, x)
来源：http://ivi.yanxiufei.cn

Ruby: arr.index(x)
来源：http://jgb.guannengcc.top

C#:   list.IndexOf(x);
来源：http://sfi.shanyushiyangtech.top

[D13] 过滤（保留满足条件的）
来源：http://pnw.ydzc1.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://miu.tarul.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://clr.dashuyun.cn

JS:   arr.filter(x => x > 3)
来源：http://hrl.uphjek.com

TS:   arr.filter(x => x > 3)
来源：http://kwt.9152youxi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://eoi.pengpengdd.cyou

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://afy.ppjwa.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jdc.tanke756.top

C#:   list.Where(x => x > 3).ToList()
来源：http://pqh.0kj1m.cn

[D14] 映射转换（每个元素变形）
来源：http://yhh.cucudq.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ddr.gaohongyu789.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qio.9152youxi.cn

JS:   arr.map(x => x * 2)
来源：http://dmz.uphjek.com

TS:   arr.map(x => x * 2)
来源：http://dtz.c1oappe.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://vhy.xuanzx.com

Go:   // 手写循环
来源：http://nio.cdnleiting.top

Ruby: arr.map { |x| x * 2 }
来源：http://lnf.zdqjudy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://nkp.jinyuanbaomall.cn

[D15] 去重
来源：http://lat.wangshuangyany.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://okl.vehdjk.com

PHP:  array_unique($arr);
来源：http://gdh.gzhubu.top

JS:   [...new Set(arr)]
来源：http://mts.meibo888.top

TS:   [...new Set(arr)]
来源：http://ejd.gotoacloud.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://eyj.9152youxi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://arh.yj20258.top

Ruby: arr.uniq
来源：http://wtr.xylfe.cn

C#:   list.Distinct().ToList()
来源：http://voj.xylfe.cn

[D16] 求和与平均值
来源：http://klu.kuanghao11.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jjc.aizwys.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nlw.jqgfzy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bec.xuanzx.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ggm.redwolf501.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hcn.ybcxt.top

Go:   // 手写循环累加
来源：http://dvt.gzhubu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vbb.shzxlz.cn

C#:   list.Sum();  list.Average()
来源：http://zus.shzxlz.cn

[D17] 最大值与最小值
来源：http://jbt.aibaodan.cn

Py:   max(arr);  min(arr)
来源：http://nrj.daxiang520.top

PHP:  max($arr);  min($arr);
来源：http://hnb.bbcook.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lhu.xinyue.icu

TS:   Math.max(...arr);
来源：http://egj.svipenyu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gqa.9152youxi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hnu.jianghu66.top

Ruby: arr.max;  arr.min
来源：http://xjp.dianchejie.cn

C#:   list.Max();  list.Min()
来源：http://kfd.xinyue.icu

[D18] 扁平化嵌套数组
来源：http://owu.aibaodan.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uum.fanxiaobao.xyz

PHP:  array_merge(...$nested);
来源：http://wud.gaohongyu789.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ndc.zdbjq.cn

TS:   nested.flat();
来源：http://qei.cashguo.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://woh.wangdashe.top

Go:   // 手写双层循环
来源：http://ckl.uphjek.com

Ruby: nested.flatten
来源：http://lxi.xylfe.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wpn.xylfe.cn

[D19] 按字段分组
来源：http://njh.zhiwuduotai.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ptk.hnxiangtu.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://viy.jianghu66.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ktg.svipenyu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://brm.jiagoushi.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yyk.fengsongda.top

Go:   // 手写 map[string][]T
来源：http://tzf.iojbl.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ihr.sxryk.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bbq.feifeiyinyue.top

[D20] 统计每个元素出现次数
来源：http://rhd.wangshuangyany.cn

Py:   Counter(arr)
来源：http://qgh.hnxiangtu.top

PHP:  array_count_values($arr);
来源：http://elk.zhongyouzk.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ule.birdmap.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kur.chenzaomai.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://npo.shuidangran.top

Go:   // 手写 map[T]int
来源：http://meg.jlsjyb.cn

Ruby: arr.tally
来源：http://wgx.jinyuanbaomall.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dgz.chenjidiqi.icu

[D21] 判断是否包含某元素
来源：http://lrl.316326.xyz

Py:   x in arr
来源：http://byt.zdqjudy.top

PHP:  in_array($x, $arr, true);
来源：http://syx.cdnleiting.top

JS:   arr.includes(x)
来源：http://nwl.iojbl.cn

TS:   arr.includes(x)
来源：http://sxd.hcnkem.com

Java: list.contains(x)
来源：http://jlk.jinqigufen.top

Go:   slices.Contains(arr, x)
来源：http://yrn.nanxinkj.top

Ruby: arr.include?(x)
来源：http://wsw.zhengqikj.top

C#:   list.Contains(x)
来源：http://pcn.yj20258888.top

[D22] 复制数组（避免共享引用）
来源：http://soj.cdnleiting.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://axl.ybcxt.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hky.yuanzhike.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ekm.vehdjk.com

TS:   [...arr];
来源：http://iqe.wangdashe.top

Java: new ArrayList<>(list);
来源：http://zsr.xuanzx.com

Go:   copied := append([]int(nil), arr...)
来源：http://rzj.gotoacloud.top

Ruby: arr.dup;  arr.clone
来源：http://nch.jqgufenzy.top

C#:   new List<int>(list);
来源：http://koj.kuanghao11.cn

[D23] reduce 累积计算
来源：http://fkk.ydzc1.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tko.pycfn.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cih.gaohongyu789.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rbn.shuidangran.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wtq.ppjwa.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://pmo.hywenlv.cn

Go:   // 手写循环
来源：http://imt.nwbrower.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vhv.fehbvm.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kyd.bbcook.cn

[D24] 字典 / Map 基本操作
来源：http://juk.hongshengwenyu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lzh.jqgufenzy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jxz.vqdsnc.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jez.ppjwa.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tpe.fengsongda.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zdh.yj202588.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yjd.pengpengdd.cyou

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bfv.nanxuanxn.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nki.ywan-chungtsiang.top

[D25] Set 集合去重与交并差
来源：http://lhg.svipenyu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://slt.dashuyun.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rgo.nanxuanxn.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://asc.cheryme.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bgx.fzhhl.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bva.gogol.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ztw.316326.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jhj.fanxiaobao.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yye.chenjidiqi.icu

[D26] 数组转字符串
来源：http://twl.shuidangran.top

Py:   ", ".join(map(str, arr))
来源：http://akz.gzhubu.top

PHP:  implode(", ", $arr);
来源：http://inu.zhengqikj.top

JS:   arr.join(", ")
来源：http://mzf.yuanzhike.top

TS:   arr.join(", ")
来源：http://zib.wangdashe.top


<!-- 参考信息 -->