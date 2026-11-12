代发 wailian999

TS:   同 JS
来源：http://fig.andypj.xyz

Java: 方法内为块级作用域
来源：http://gyg.fktsv.cn

Go:   花括号块级作用域
来源：http://ooz.zhongyouzk.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pit.iojbl.cn

C#:   块级作用域
来源：http://ekk.ivvv.top

[C11] 模块导入与导出
来源：http://nwx.c1oappe.top

Py:   from module import func
来源：http://hrb.yonumen.top

PHP:  require "file.php";  或 use App\Service;
来源：http://aud.zhixingplan.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://rfq.havefunace.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fjm.quarkkingdee.top

Java: import java.util.List;
来源：http://xxl.ydjk.org.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nrr.shanyushiyangtech.top

Ruby: require "json"; require_relative "./util"
来源：http://wsn.shangyingyoupin.top

C#:   using System.Text;
来源：http://fwl.daria6918.cn

[C12] 立即执行函数 IIFE
来源：http://ntm.yvedp.cn

Py:   (lambda: print("run"))()
来源：http://bvr.yongpay.top

PHP:  (function () { echo "run"; })();
来源：http://dso.yanxiufei.cn

JS:   (() => { console.log("run"); })();
来源：http://jug.jyoumei.cn

TS:   (() => { console.log("run"); })();
来源：http://zuz.nwbrower.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hfh.ydjk.org.cn

Go:   func() { fmt.Println("run") }()
来源：http://yeo.zhixingplan.top

Ruby: -> { puts "run" }.call
来源：http://mvi.sweek.top

C#:   // 无 IIFE：用静态构造函数
来源：http://tud.zhoulong.xyz

[C13] 类型声明 / 类型注解
来源：http://qrs.hfpthk.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yhk.ppjwa.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iat.fengsongda.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tyz.ydzc1.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kyc.xinyue.icu

Java: int add(int a, int b) { return a + b; }
来源：http://lig.jianghu66.top

Go:   func add(a, b int) int
来源：http://jan.wangdashe.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xwe.iojbl.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mrk.hcnkem.com

[C14] 泛型函数
来源：http://emk.shzxlz.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uqf.dashuyun.cn

PHP:  // 无泛型
来源：http://eow.316326.xyz

JS:   // 无泛型
来源：http://ucw.52xcode.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://eob.jinyuanbaomall.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gbb.jianghu66.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lmy.aibaodan.cn

Ruby: # 无泛型
来源：http://teg.meibo888.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mxa.yonumen.top

[C15] 解构 / 展开参数
来源：http://zgx.hnxiangtu.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qbi.yongpay.top

PHP:  [$a, $b] = $pair;
来源：http://dub.gaohongyu789.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bzd.sufxvd.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://haj.gogol.net.cn

Java: // 无解构
来源：http://qor.gotoacloud.top

Go:   // 无解构
来源：http://dfd.jqgfzy.top

Ruby: a, b = pair
来源：http://arz.xylfe.cn

C#:   var (a, b) = pair;
来源：http://pkw.wangshuangyany.cn

[C16] 函数 / 方法重载
来源：http://twi.fengsongda.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://eux.sweek.top

PHP:  // 无重载
来源：http://iny.zhongyouzk.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://zyt.quarkkingdee.top

TS:   // 用联合类型或重载签名声明
来源：http://wmw.wangdashe.top

Java: void f(int a) {}  void f(String a) {}
来源：http://gty.bbcook.cn

Go:   // 无重载：用不同函数名
来源：http://dxt.tianlin.xyz

Ruby: # 无重载：靠动态参数
来源：http://esk.zhengqikj.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://avt.wangdashe.top

================================================================================
来源：http://aye.shanyushiyangtech.top

D. 数组 / 列表 / 集合
来源：http://kas.dianchejie.cn

================================================================================
来源：http://qgt.xuetiantiany.cn

[D01] 创建数组 / 列表
来源：http://iwk.svipenyu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://vao.yj202588.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://htf.chenlongwang.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://her.iojbl.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://uue.dashuyun.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tjd.kuanghao11.cn

Go:   arr := []int{1, 2, 3}
来源：http://wde.tarul.cn

Ruby: arr = [1, 2, 3]
来源：http://soo.shanyushiyangtech.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mam.tian-w.cn

[D02] 追加元素到末尾
来源：http://xmx.shanyushiyangtech.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://twh.jyoumei.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hrq.cucudq.cn

JS:   arr.push(4);
来源：http://ywc.birdmap.top

TS:   arr.push(4);
来源：http://ejt.xingfuxueyuan.xyz

Java: list.add(4);
来源：http://btj.zhongyouzk.top

Go:   arr = append(arr, 4)
来源：http://pqe.epnwcf.com

Ruby: arr << 4; arr.push(5)
来源：http://fyv.gaohongyu789.top

C#:   list.Add(4);
来源：http://uyk.ydzc1.top

[D03] 在指定位置插入元素
来源：http://pei.hfpthk.cn

Py:   arr.insert(0, 0)
来源：http://nst.52xcode.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://muq.quarkkingdee.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mpj.haohaochexian.top

TS:   arr.splice(0, 0, 0);
来源：http://eoc.hnqzz.top

Java: list.add(0, 0);
来源：http://utp.pengpengdd.cyou

Go:   arr = append([]int{0}, arr...)
来源：http://sne.yueranfly.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tog.zhaomingkeji.xyz

C#:   list.Insert(0, 0);
来源：http://fjg.vehdjk.com

[D04] 删除元素
来源：http://lyy.bbcook.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ekh.hcnkem.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mkw.zycfv.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mzo.xuanzx.com

TS:   arr.splice(0, 1);
来源：http://qjm.tian-w.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ccb.zhongyouzk.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://krd.fktsv.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zbm.gotoacloud.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://whu.ywan-chungtsiang.top

[D05] 访问与修改元素
来源：http://xis.yuxming.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lxj.jiagoushi.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xrd.meibo888.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qbv.andypj.xyz

TS:   arr[0]; arr.at(-1);
来源：http://vnv.zdqjudy.top

Java: list.get(0); list.set(0, 9);
来源：http://tap.nwbrower.top

Go:   arr[0]; arr[0] = 9
来源：http://tcb.nanxuanxn.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cvz.hnxiangtu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fve.tarul.cn

[D06] 数组长度
来源：http://sfz.nanxinkj.top

Py:   len(arr)
来源：http://ukj.ivvv.top

PHP:  count($arr);
来源：http://dgj.0kj1m.cn

JS:   arr.length
来源：http://ouq.hywenlv.cn

TS:   arr.length
来源：http://sxu.52xcode.cn

Java: list.size();
来源：http://aco.uphjek.com

Go:   len(arr)
来源：http://lam.jinqigfzy.top

Ruby: arr.length; arr.size
来源：http://mch.aizwys.cn

C#:   list.Count;
来源：http://piv.shuidangran.top

[D07] 切片 / 取子数组
来源：http://ydb.yangfankeji.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cny.ehwqpu.com

PHP:  array_slice($arr, 1, 3);
来源：http://ilu.snrcjt.cn

JS:   arr.slice(1, 4);
来源：http://zzi.sjlbkw.cn

TS:   arr.slice(1, 4);
来源：http://yjf.9152youxi.cn

Java: list.subList(1, 4);
来源：http://gws.ydzc1.top

Go:   arr[1:4]
来源：http://xgo.ywan-chungtsiang.top

Ruby: arr[1, 3]
来源：http://dek.cdnleiting.top

C#:   list.GetRange(1, 3);
来源：http://yxb.tian-w.cn

[D08] 合并两个数组
来源：http://shl.yj202588.top

Py:   a + b;  a.extend(b)
来源：http://hub.fengsongda.top

PHP:  array_merge($a, $b);
来源：http://gey.vqdsnc.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xun.hongshengwenyu.top

TS:   [...a, ...b];
来源：http://ufx.xingfuxueyuan.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://klq.shuidangran.top

Go:   append(a, b...)
来源：http://agd.daria6918.cn

Ruby: a + b;  a.concat(b)
来源：http://lyj.jinqigfzy.top

C#:   a.Concat(b).ToList()
来源：http://yaq.xuetiantiany.cn

[D09] 排序（升序）
来源：http://nhj.nanxinkj.top

Py:   sorted(arr);  arr.sort()
来源：http://ete.vqdsnc.cn

PHP:  sort($arr);
来源：http://bhj.havefunace.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://aon.hywenlv.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://crt.chenjidiqi.icu

Java: Collections.sort(list);  list.sort(null);
来源：http://dez.yanxiufei.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zhp.xingfuxueyuan.xyz

Ruby: arr.sort
来源：http://uhf.gaohongyu789.top

C#:   list.Sort();
来源：http://bnw.jlsjyb.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lqk.xuanzx.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://aqz.smart0.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ogm.zhoulong.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://iwq.yuxming.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://led.nanxuanxn.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kcs.gaohongyu789.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zja.sxryk.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hag.pycfn.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xtr.sxryk.cn

[D11] 反转数组
来源：http://nbr.zycfv.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ixd.zdqjudy.top

PHP:  array_reverse($arr);
来源：http://qgi.yj202588.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jup.havefunace.top

TS:   [...arr].reverse();
来源：http://lns.redwolf501.top

Java: Collections.reverse(list);
来源：http://ugh.zhongyouzk.top

Go:   slices.Reverse(arr)
来源：http://pfm.gzhubu.top

Ruby: arr.reverse
来源：http://zit.uphjek.com

C#:   list.Reverse();
来源：http://lcb.sweek.top

[D12] 查找元素下标
来源：http://hti.redwolf501.top

Py:   arr.index(x);  x in arr
来源：http://esy.gzhubu.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dss.hnxiangtu.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aer.52xcode.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jdv.yongpay.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://idv.zdbjq.cn

Go:   slices.Index(arr, x)
来源：http://dda.xziqi.cn

Ruby: arr.index(x)
来源：http://uyx.zhiwuduotai.top

C#:   list.IndexOf(x);
来源：http://twi.shanyushiyangtech.top

[D13] 过滤（保留满足条件的）
来源：http://ara.chenlongwang.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://edy.9152youxi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yxt.zdqjudy.top

JS:   arr.filter(x => x > 3)
来源：http://cgd.xinyue.icu

TS:   arr.filter(x => x > 3)
来源：http://jhc.yongpay.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wfn.wangdashe.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uta.pengpengdd.cyou

Ruby: arr.select { |x| x > 3 }
来源：http://mql.fzhhl.top

C#:   list.Where(x => x > 3).ToList()
来源：http://zix.0kj1m.cn

[D14] 映射转换（每个元素变形）
来源：http://xde.dianchejie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ygg.birdmap.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fhq.hnqzz.top

JS:   arr.map(x => x * 2)
来源：http://ohv.vehdjk.com

TS:   arr.map(x => x * 2)
来源：http://cpy.fktsv.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ecd.feifeiyinyue.top

Go:   // 手写循环
来源：http://utk.feifeiyinyue.top

Ruby: arr.map { |x| x * 2 }
来源：http://xjo.guowangkeji.top

C#:   list.Select(x => x * 2).ToList()
来源：http://mow.daria6918.cn

[D15] 去重
来源：http://mha.ydzc1.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jyz.dianchejie.cn

PHP:  array_unique($arr);
来源：http://mpu.pycfn.com

JS:   [...new Set(arr)]
来源：http://fdp.shuidangran.top

TS:   [...new Set(arr)]
来源：http://gsh.gotoacloud.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hwb.svipenyu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zvr.cqqwz.cn

Ruby: arr.uniq
来源：http://ihh.quarkkingdee.top

C#:   list.Distinct().ToList()
来源：http://mjo.ywan-chungtsiang.top

[D16] 求和与平均值
来源：http://tde.hongshengwenyu.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://eja.zhiwuduotai.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vpx.mhx1999.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bld.fzhhl.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vkc.andypj.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wcl.daxiang520.top

Go:   // 手写循环累加
来源：http://poq.andypj.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hjq.pycfn.com

C#:   list.Sum();  list.Average()
来源：http://csy.aizwys.cn

[D17] 最大值与最小值
来源：http://urb.cdnleiting.top

Py:   max(arr);  min(arr)
来源：http://wiq.redwolf501.top

PHP:  max($arr);  min($arr);
来源：http://yfx.hcnkem.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cvc.hammf.cn

TS:   Math.max(...arr);
来源：http://sfx.havefunace.top

Java: Collections.max(list);  Collections.min(list);
来源：http://cis.bjfxy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://eck.hfpthk.cn

Ruby: arr.max;  arr.min
来源：http://dfw.guowangkeji.top

C#:   list.Max();  list.Min()
来源：http://fhy.yueranfly.top

[D18] 扁平化嵌套数组
来源：http://jte.xingfuxueyuan.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://znn.yonumen.top

PHP:  array_merge(...$nested);
来源：http://kwr.fzhhl.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ckp.fzhhl.top

TS:   nested.flat();
来源：http://ugx.redwolf501.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ygk.redwolf501.top

Go:   // 手写双层循环
来源：http://jeo.aibaodan.cn

Ruby: nested.flatten
来源：http://rhg.yanxiufei.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ckt.pengpengdd.cyou

[D19] 按字段分组
来源：http://phh.jyoumei.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ipu.snrcjt.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://uza.hnxiangtu.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://img.zdqjudy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://eur.316326.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fnd.jyoumei.cn

Go:   // 手写 map[string][]T
来源：http://eyt.jinyuanbaomall.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gln.fanxiaobao.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mmf.guannengcc.top

[D20] 统计每个元素出现次数
来源：http://zve.fktsv.cn

Py:   Counter(arr)
来源：http://alt.yj202588.top

PHP:  array_count_values($arr);
来源：http://rwn.wangshuangyany.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ijq.nanxinkj.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tpy.pengpengdd.cyou

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sgt.birdmap.top

Go:   // 手写 map[T]int
来源：http://qmj.ivvv.top

Ruby: arr.tally
来源：http://jgx.ehwqpu.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ynr.fehbvm.com

[D21] 判断是否包含某元素
来源：http://uzp.ppjwa.cn

Py:   x in arr
来源：http://ojj.xingfuxueyuan.xyz

PHP:  in_array($x, $arr, true);
来源：http://yfe.guannengcc.top

JS:   arr.includes(x)
来源：http://pqo.gzhubu.top

TS:   arr.includes(x)
来源：http://gau.sufxvd.cn

Java: list.contains(x)
来源：http://gjz.pycfn.com

Go:   slices.Contains(arr, x)
来源：http://dzm.0kj1m.cn

Ruby: arr.include?(x)
来源：http://gcz.jianghu66.top

C#:   list.Contains(x)
来源：http://mxj.fzhhl.top

[D22] 复制数组（避免共享引用）
来源：http://zxk.zhijiandao.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lkn.cqqwz.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://trj.52xcode.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vdj.chenlongwang.top

TS:   [...arr];
来源：http://iai.yfazqb.com

Java: new ArrayList<>(list);
来源：http://eqx.zhijiandao.cn

Go:   copied := append([]int(nil), arr...)
来源：http://mwl.yfazqb.com

Ruby: arr.dup;  arr.clone
来源：http://rlu.daxiang520.top

C#:   new List<int>(list);
来源：http://het.yj20258888.top

[D23] reduce 累积计算
来源：http://kbx.pycfn.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://eev.shanyushiyangtech.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fiy.yueranfly.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kqa.hfpthk.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://krx.zycfv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://glw.shangyingyoupin.top

Go:   // 手写循环
来源：http://wsa.cashguo.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bes.jinqigufen.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xeu.ybcxt.top

[D24] 字典 / Map 基本操作
来源：http://lwm.0kj1m.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://olu.yuxming.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ezd.smart0.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kkp.9152youxi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lmn.jinyuanbaomall.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lkf.jqgufenzy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ape.xingfuxueyuan.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://obt.yangfankeji.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rbn.yj202588.top

[D25] Set 集合去重与交并差
来源：http://eov.c1oappe.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jtl.hammf.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hix.aibaodan.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vio.sxryk.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vnd.ehwqpu.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ueu.jyoumei.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rri.316326.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cka.fehbvm.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://aql.vqdsnc.cn

[D26] 数组转字符串
来源：http://sbq.wangshuangyany.cn

Py:   ", ".join(map(str, arr))
来源：http://fbv.nwbrower.top

PHP:  implode(", ", $arr);
来源：http://jdq.hywenlv.cn

JS:   arr.join(", ")
来源：http://ljo.zhengqikj.top

TS:   arr.join(", ")
来源：http://reu.sxryk.cn

Java: String.join(", ", list)
来源：http://pxt.xylfe.cn

Go:   strings.Join(strs, ", ")
来源：http://fgx.feifeiyinyue.top

Ruby: arr.join(", ")
来源：http://eyo.xylfe.cn

C#:   string.Join(", ", list)
来源：http://sdq.jqgfzy.top

================================================================================
来源：http://caa.zhixingplan.top

E. 字符串处理
来源：http://jee.ydzc1.top

================================================================================
来源：http://vfj.jinghuilouyu.cn

[E01] 拼接字符串
来源：http://ncu.aizwys.cn


<!-- 参考信息 -->