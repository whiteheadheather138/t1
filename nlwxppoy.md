代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ima.yuxming.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hqw.fehbvm.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://chi.chenlongwang.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ubv.meibo888.top

[C10] 变量作用域
来源：http://vxr.tian-w.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tzh.hfpthk.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qvl.zhongyouzk.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jkk.yvedp.cn

TS:   同 JS
来源：http://hpn.c1oappe.top

Java: 方法内为块级作用域
来源：http://niw.tianlin.xyz

Go:   花括号块级作用域
来源：http://vqz.epnwcf.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://oat.dashuyun.cn

C#:   块级作用域
来源：http://hzl.snrcjt.cn

[C11] 模块导入与导出
来源：http://cem.sysykeji.top

Py:   from module import func
来源：http://wbx.daxiang520.top

PHP:  require "file.php";  或 use App\Service;
来源：http://jcq.shangyingyoupin.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://fdh.hnqzz.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pwm.hnxiangtu.top

Java: import java.util.List;
来源：http://vuh.shuidangran.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qqw.yj20258.top

Ruby: require "json"; require_relative "./util"
来源：http://azc.haohaochexian.top

C#:   using System.Text;
来源：http://ayw.cheryme.top

[C12] 立即执行函数 IIFE
来源：http://tjj.gzhubu.top

Py:   (lambda: print("run"))()
来源：http://kwv.tian-w.cn

PHP:  (function () { echo "run"; })();
来源：http://deg.bjfxy.top

JS:   (() => { console.log("run"); })();
来源：http://qoh.sxryk.cn

TS:   (() => { console.log("run"); })();
来源：http://peu.tianlin.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xno.zhengqikj.top

Go:   func() { fmt.Println("run") }()
来源：http://rir.jqgufenzy.top

Ruby: -> { puts "run" }.call
来源：http://dyd.ehwqpu.com

C#:   // 无 IIFE：用静态构造函数
来源：http://hqr.xingfuxueyuan.xyz

[C13] 类型声明 / 类型注解
来源：http://iyj.cheryme.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ogt.zhiwuduotai.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fcw.zhongyouzk.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hff.yj20258.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zcu.nwbrower.top

Java: int add(int a, int b) { return a + b; }
来源：http://rkc.hongshengwenyu.top

Go:   func add(a, b int) int
来源：http://flz.hammf.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pkl.yj202588.top

C#:   int Add(int a, int b) => a + b;
来源：http://sis.gotoacloud.top

[C14] 泛型函数
来源：http://rlo.cheryme.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cqc.jlsjyb.cn

PHP:  // 无泛型
来源：http://wtk.zdqjudy.top

JS:   // 无泛型
来源：http://neu.0kj1m.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ubd.havefunace.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kru.yvedp.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hyx.sweek.top

Ruby: # 无泛型
来源：http://tav.cheryme.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://asj.yongpay.top

[C15] 解构 / 展开参数
来源：http://wqa.yangfankeji.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://czj.jinqigfzy.top

PHP:  [$a, $b] = $pair;
来源：http://hrh.hongshengwenyu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ayo.hcnkem.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nqe.nwbrower.top

Java: // 无解构
来源：http://fys.yfazqb.com

Go:   // 无解构
来源：http://fwz.jqgfzy.top

Ruby: a, b = pair
来源：http://yki.guowangkeji.top

C#:   var (a, b) = pair;
来源：http://rfm.ctjpmb.com

[C16] 函数 / 方法重载
来源：http://xls.iojbl.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pkm.ydjk.org.cn

PHP:  // 无重载
来源：http://ycx.dashuyun.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://dgc.ppjwa.cn

TS:   // 用联合类型或重载签名声明
来源：http://lgi.zhoulong.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://ifg.sufxvd.cn

Go:   // 无重载：用不同函数名
来源：http://sun.ctjpmb.com

Ruby: # 无重载：靠动态参数
来源：http://dwe.aibaodan.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://iox.chenjidiqi.icu

================================================================================
来源：http://gsl.ivvv.top

D. 数组 / 列表 / 集合
来源：http://hbw.zhoulong.xyz

================================================================================
来源：http://vxr.yongpay.top

[D01] 创建数组 / 列表
来源：http://dik.snrcjt.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://opd.316326.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uae.quarkkingdee.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fva.zhaomingkeji.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://gbb.jinyuanbaomall.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dqg.yvedp.cn

Go:   arr := []int{1, 2, 3}
来源：http://oub.cqqwz.cn

Ruby: arr = [1, 2, 3]
来源：http://lsa.shuidangran.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://uxw.sxryk.cn

[D02] 追加元素到末尾
来源：http://lmb.xuanzx.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jcd.haohaochexian.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kqo.yfazqb.com

JS:   arr.push(4);
来源：http://dmg.chenlongwang.top

TS:   arr.push(4);
来源：http://jou.sufxvd.cn

Java: list.add(4);
来源：http://dgi.gzhubu.top

Go:   arr = append(arr, 4)
来源：http://gio.c1oappe.top

Ruby: arr << 4; arr.push(5)
来源：http://fqx.sysykeji.top

C#:   list.Add(4);
来源：http://ehi.vqdsnc.cn

[D03] 在指定位置插入元素
来源：http://dlt.andypj.xyz

Py:   arr.insert(0, 0)
来源：http://sve.havefunace.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ecv.zhengqikj.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tou.ehwqpu.com

TS:   arr.splice(0, 0, 0);
来源：http://zty.smart0.xyz

Java: list.add(0, 0);
来源：http://ckl.zycfv.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yrp.xingfuxueyuan.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dcw.bjfxy.top

C#:   list.Insert(0, 0);
来源：http://vos.chenlongwang.top

[D04] 删除元素
来源：http://ouy.sjlbkw.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lgy.tanke756.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wfh.snrcjt.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rxh.xinyue.icu

TS:   arr.splice(0, 1);
来源：http://uon.nanxinkj.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pce.sjlbkw.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gjd.yangfankeji.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vux.xylfe.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://oej.yj202588.top

[D05] 访问与修改元素
来源：http://iup.shanyushiyangkeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://roz.ydzc1.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zpn.jqgufenzy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hkq.zdbjq.cn

TS:   arr[0]; arr.at(-1);
来源：http://btc.iojbl.cn

Java: list.get(0); list.set(0, 9);
来源：http://mwq.chenlongwang.top

Go:   arr[0]; arr[0] = 9
来源：http://kku.xingfuxueyuan.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xsd.dashuyun.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yeq.dashuyun.cn

[D06] 数组长度
来源：http://bjc.52xcode.cn

Py:   len(arr)
来源：http://kli.yj20258.top

PHP:  count($arr);
来源：http://zwx.cdnleiting.top

JS:   arr.length
来源：http://kgd.xziqi.cn

TS:   arr.length
来源：http://gjg.yueranfly.top

Java: list.size();
来源：http://xmb.nanxuanxn.top

Go:   len(arr)
来源：http://laq.zdqjudy.top

Ruby: arr.length; arr.size
来源：http://lpu.sxryk.cn

C#:   list.Count;
来源：http://cix.shanyushiyangkeji.top

[D07] 切片 / 取子数组
来源：http://iug.guowangkeji.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cmg.sweek.top

PHP:  array_slice($arr, 1, 3);
来源：http://vcr.hammf.cn

JS:   arr.slice(1, 4);
来源：http://uvq.andypj.xyz

TS:   arr.slice(1, 4);
来源：http://rtz.iojbl.cn

Java: list.subList(1, 4);
来源：http://hyc.xylfe.cn

Go:   arr[1:4]
来源：http://qfs.cashguo.top

Ruby: arr[1, 3]
来源：http://mar.zhoulong.xyz

C#:   list.GetRange(1, 3);
来源：http://emx.aibaodan.cn

[D08] 合并两个数组
来源：http://kbc.ehwqpu.com

Py:   a + b;  a.extend(b)
来源：http://rkd.ctjpmb.com

PHP:  array_merge($a, $b);
来源：http://frf.nanxuanxn.top

JS:   [...a, ...b];  a.concat(b);
来源：http://hcy.guannengcc.top

TS:   [...a, ...b];
来源：http://dgm.pycfn.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://htl.zhiwuduotai.top

Go:   append(a, b...)
来源：http://gja.shzxlz.cn

Ruby: a + b;  a.concat(b)
来源：http://eub.dashuyun.cn

C#:   a.Concat(b).ToList()
来源：http://kgg.xziqi.cn

[D09] 排序（升序）
来源：http://qas.chenzaomai.com

Py:   sorted(arr);  arr.sort()
来源：http://qdh.aibaodan.cn

PHP:  sort($arr);
来源：http://aym.ybcxt.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gqn.c1oappe.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://igf.ehwqpu.com

Java: Collections.sort(list);  list.sort(null);
来源：http://crk.nwbrower.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bvd.xingfuxueyuan.xyz

Ruby: arr.sort
来源：http://vsv.jianghu66.top

C#:   list.Sort();
来源：http://jqj.zdbjq.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xsf.ehwqpu.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://djc.mhx1999.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vux.tian-w.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ahl.hfpthk.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yjn.gaohongyu789.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://drw.sweek.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tog.yj20258888.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hxg.ctjpmb.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ebe.ydjk.org.cn

[D11] 反转数组
来源：http://xkc.9152youxi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://aqg.birdmap.top

PHP:  array_reverse($arr);
来源：http://car.yuxming.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xkt.tian-w.cn

TS:   [...arr].reverse();
来源：http://hcs.epnwcf.com

Java: Collections.reverse(list);
来源：http://oxq.guannengcc.top

Go:   slices.Reverse(arr)
来源：http://gar.sufxvd.cn

Ruby: arr.reverse
来源：http://pvc.shangyingyoupin.top

C#:   list.Reverse();
来源：http://bap.kuanghao11.cn

[D12] 查找元素下标
来源：http://dim.yonumen.top

Py:   arr.index(x);  x in arr
来源：http://gsq.52xcode.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nod.hcnkem.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ton.zdqjudy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hqz.chenlongwang.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hxl.jqgufenzy.top

Go:   slices.Index(arr, x)
来源：http://ueq.meibo888.top

Ruby: arr.index(x)
来源：http://kvo.yuanzhike.top

C#:   list.IndexOf(x);
来源：http://njm.havefunace.top

[D13] 过滤（保留满足条件的）
来源：http://ngq.cqqwz.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dzz.ppjwa.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rql.jinyuanbaomall.cn

JS:   arr.filter(x => x > 3)
来源：http://wdz.iojbl.cn

TS:   arr.filter(x => x > 3)
来源：http://wkr.ehwqpu.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ooe.uphjek.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://shc.zhoulong.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://vbs.ybcxt.top

C#:   list.Where(x => x > 3).ToList()
来源：http://zbm.sweek.top

[D14] 映射转换（每个元素变形）
来源：http://pmn.wangshuangyany.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uqf.yuxming.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://myc.chenjidiqi.icu

JS:   arr.map(x => x * 2)
来源：http://ulx.cheryme.top

TS:   arr.map(x => x * 2)
来源：http://byj.ivvv.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://xps.hongshengwenyu.top

Go:   // 手写循环
来源：http://dhs.xuanzx.com

Ruby: arr.map { |x| x * 2 }
来源：http://qsj.daria6918.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rfa.zhixingplan.top

[D15] 去重
来源：http://phi.nwbrower.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://shg.yj20258888.top

PHP:  array_unique($arr);
来源：http://olm.jyoumei.cn

JS:   [...new Set(arr)]
来源：http://dsh.chenlongwang.top

TS:   [...new Set(arr)]
来源：http://rlt.gaohongyu789.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ahl.zhijiandao.cn

Go:   // 用 map[T]struct{} 手写
来源：http://dcz.kuanghao11.cn

Ruby: arr.uniq
来源：http://uza.gaohongyu789.top

C#:   list.Distinct().ToList()
来源：http://mrn.chenzaomai.com

[D16] 求和与平均值
来源：http://bxl.sufxvd.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bog.guannengcc.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mwe.dianchejie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xja.0kj1m.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vqj.hfpthk.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://eif.svipenyu.cn

Go:   // 手写循环累加
来源：http://hqr.cqqwz.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://stn.aizwys.cn

C#:   list.Sum();  list.Average()
来源：http://qzj.tian-w.cn

[D17] 最大值与最小值
来源：http://zfz.jqgfzy.top

Py:   max(arr);  min(arr)
来源：http://wpb.ydzc1.top

PHP:  max($arr);  min($arr);
来源：http://xrc.haohaochexian.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://chp.hysaishi.cn

TS:   Math.max(...arr);
来源：http://raq.hnqzz.top

Java: Collections.max(list);  Collections.min(list);
来源：http://syg.xingfuxueyuan.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yxn.cucudq.cn

Ruby: arr.max;  arr.min
来源：http://mqq.zhoulong.xyz

C#:   list.Max();  list.Min()
来源：http://xkr.shzxlz.cn

[D18] 扁平化嵌套数组
来源：http://qnz.jqgfzy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://foh.hywenlv.cn

PHP:  array_merge(...$nested);
来源：http://jno.nwbrower.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zua.birdmap.top

TS:   nested.flat();
来源：http://pue.vqdsnc.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dsp.hywenlv.cn

Go:   // 手写双层循环
来源：http://ggf.smart0.xyz

Ruby: nested.flatten
来源：http://gxy.gaohongyu789.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://svi.zhixingplan.top

[D19] 按字段分组
来源：http://ekr.kuanghao11.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hxf.0kj1m.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://iba.hcnkem.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mdh.316326.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://dnh.fktsv.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dae.zhongyouzk.top

Go:   // 手写 map[string][]T
来源：http://dnf.xylfe.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://tnw.sysykeji.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wbr.ywan-chungtsiang.top

[D20] 统计每个元素出现次数
来源：http://mai.ydzc1.top

Py:   Counter(arr)
来源：http://ytz.cucudq.cn

PHP:  array_count_values($arr);
来源：http://gvh.guannengcc.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dqc.guowangkeji.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iju.0kj1m.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://osx.smart0.xyz

Go:   // 手写 map[T]int
来源：http://nnn.pycfn.com

Ruby: arr.tally
来源：http://gmx.andypj.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://eik.hammf.cn

[D21] 判断是否包含某元素
来源：http://vgs.jqgufenzy.top

Py:   x in arr
来源：http://ang.zhiwuduotai.top

PHP:  in_array($x, $arr, true);
来源：http://mys.cheryme.top

JS:   arr.includes(x)
来源：http://vst.uphjek.com

TS:   arr.includes(x)
来源：http://nvf.hysaishi.cn

Java: list.contains(x)
来源：http://rtq.jyoumei.cn

Go:   slices.Contains(arr, x)
来源：http://apl.aizwys.cn

Ruby: arr.include?(x)
来源：http://zdy.daria6918.cn

C#:   list.Contains(x)
来源：http://gjv.hnxiangtu.top

[D22] 复制数组（避免共享引用）
来源：http://dbo.sweek.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xqe.wangshuangyany.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cqn.hesvh.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pdk.sysykeji.top

TS:   [...arr];
来源：http://irk.wangshuangyany.cn

Java: new ArrayList<>(list);
来源：http://pnk.fehbvm.com

Go:   copied := append([]int(nil), arr...)
来源：http://rlj.yuxming.cn

Ruby: arr.dup;  arr.clone
来源：http://rxx.wangdashe.top

C#:   new List<int>(list);
来源：http://qwy.jinghuilouyu.cn

[D23] reduce 累积计算
来源：http://iap.pycfn.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ada.hnxiangtu.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cef.svipenyu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vob.fengsongda.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rxm.xylfe.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rep.cucudq.cn

Go:   // 手写循环
来源：http://sma.havefunace.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ded.pycfn.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://osx.sxryk.cn

[D24] 字典 / Map 基本操作
来源：http://htz.shanyushiyangkeji.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hxv.jiagoushi.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cuv.aizwys.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gli.zdbjq.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rvn.sjlbkw.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qnq.yuanzhike.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ueb.ywan-chungtsiang.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fvx.yj20258.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fcd.jlsjyb.cn

[D25] Set 集合去重与交并差
来源：http://yoo.dashuyun.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://izn.jinqigfzy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zim.chenjidiqi.icu

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wyq.tianlin.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://osa.meibo888.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qtl.cashguo.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://oar.cheryme.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zds.jqgfzy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sdi.nanxinkj.top

[D26] 数组转字符串
来源：http://ici.xingfuxueyuan.xyz

Py:   ", ".join(map(str, arr))
来源：http://lez.smart0.xyz

PHP:  implode(", ", $arr);
来源：http://pgz.cheryme.top

JS:   arr.join(", ")
来源：http://xwj.c1oappe.top

TS:   arr.join(", ")
来源：http://bar.quarkkingdee.top


<!-- 参考信息 -->