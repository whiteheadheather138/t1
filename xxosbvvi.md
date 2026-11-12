代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xwh.guannengcc.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dxr.birdmap.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ioy.tanke756.top

[C09] 递归
来源：http://cpk.yj20258.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bno.havefunace.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ioo.xinyue.icu

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://amn.fktsv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aqv.gaohongyu789.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://svt.birdmap.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://iae.ybcxt.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qra.pengpengdd.cyou

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://srk.cucudq.cn

[C10] 变量作用域
来源：http://yms.yj202588.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vpg.jinghuilouyu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qgc.jianghu66.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dka.jinyuanbaomall.cn

TS:   同 JS
来源：http://kij.svipenyu.cn

Java: 方法内为块级作用域
来源：http://crw.aibaodan.cn

Go:   花括号块级作用域
来源：http://wbg.mhx1999.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://aii.xinyue.icu

C#:   块级作用域
来源：http://xho.andypj.xyz

[C11] 模块导入与导出
来源：http://ngl.havefunace.top

Py:   from module import func
来源：http://wce.xuetiantiany.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wls.zhongyouzk.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://aus.ctjpmb.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://iow.hnqzz.top

Java: import java.util.List;
来源：http://sgq.zdqjudy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zei.c1oappe.top

Ruby: require "json"; require_relative "./util"
来源：http://cyd.yvedp.cn

C#:   using System.Text;
来源：http://gwo.pycfn.com

[C12] 立即执行函数 IIFE
来源：http://jyi.xylfe.cn

Py:   (lambda: print("run"))()
来源：http://fbw.c1oappe.top

PHP:  (function () { echo "run"; })();
来源：http://lct.dashuyun.cn

JS:   (() => { console.log("run"); })();
来源：http://jln.aizwys.cn

TS:   (() => { console.log("run"); })();
来源：http://ezj.nwbrower.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ohl.yvedp.cn

Go:   func() { fmt.Println("run") }()
来源：http://acq.kuanghao11.cn

Ruby: -> { puts "run" }.call
来源：http://wts.jqgfzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://yil.cucudq.cn

[C13] 类型声明 / 类型注解
来源：http://ljh.ctjpmb.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ppw.ivvv.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zar.pycfn.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://oss.sufxvd.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yde.svipenyu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://pfo.ydzc1.top

Go:   func add(a, b int) int
来源：http://gal.meibo888.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://chx.fzhhl.top

C#:   int Add(int a, int b) => a + b;
来源：http://grb.xylfe.cn

[C14] 泛型函数
来源：http://rwr.ivvv.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lbh.zhiwuduotai.top

PHP:  // 无泛型
来源：http://lnt.gzhubu.top

JS:   // 无泛型
来源：http://psm.316326.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gdj.cucudq.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gie.shzxlz.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ywk.shanyushiyangkeji.top

Ruby: # 无泛型
来源：http://egp.cashguo.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tbh.xuanzx.com

[C15] 解构 / 展开参数
来源：http://ola.hongshengwenyu.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://odq.sjlbkw.cn

PHP:  [$a, $b] = $pair;
来源：http://rgy.epnwcf.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gnb.wangdashe.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wdq.jyoumei.cn

Java: // 无解构
来源：http://hmh.havefunace.top

Go:   // 无解构
来源：http://sng.hysaishi.cn

Ruby: a, b = pair
来源：http://one.xuanzx.com

C#:   var (a, b) = pair;
来源：http://iag.shzxlz.cn

[C16] 函数 / 方法重载
来源：http://occ.fktsv.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ntc.hammf.cn

PHP:  // 无重载
来源：http://qqd.hesvh.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://gsh.yj202588.top

TS:   // 用联合类型或重载签名声明
来源：http://gyl.smart0.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://mem.nanxinkj.top

Go:   // 无重载：用不同函数名
来源：http://ikx.sjlbkw.cn

Ruby: # 无重载：靠动态参数
来源：http://vwc.yuxming.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://oyd.yuxming.cn

================================================================================
来源：http://rsx.sysykeji.top

D. 数组 / 列表 / 集合
来源：http://gjn.ydzc1.top

================================================================================
来源：http://xei.haohaochexian.top

[D01] 创建数组 / 列表
来源：http://jjs.cqqwz.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xkz.dashuyun.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xbz.ppjwa.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cle.xylfe.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://abl.yonumen.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bip.nwbrower.top

Go:   arr := []int{1, 2, 3}
来源：http://tgp.fzhhl.top

Ruby: arr = [1, 2, 3]
来源：http://vih.shanyushiyangkeji.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ltt.ybcxt.top

[D02] 追加元素到末尾
来源：http://exa.zhiwuduotai.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yeu.hnxiangtu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://emw.havefunace.top

JS:   arr.push(4);
来源：http://mpl.hnxiangtu.top

TS:   arr.push(4);
来源：http://txx.ehwqpu.com

Java: list.add(4);
来源：http://mqb.zhiwuduotai.top

Go:   arr = append(arr, 4)
来源：http://jyx.tianlin.xyz

Ruby: arr << 4; arr.push(5)
来源：http://ucm.316326.xyz

C#:   list.Add(4);
来源：http://dtk.shanyushiyangtech.top

[D03] 在指定位置插入元素
来源：http://vku.shanyushiyangtech.top

Py:   arr.insert(0, 0)
来源：http://mdq.sufxvd.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qls.yueranfly.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pea.jqgufenzy.top

TS:   arr.splice(0, 0, 0);
来源：http://mee.chenlongwang.top

Java: list.add(0, 0);
来源：http://hsy.fktsv.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pot.sufxvd.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xqk.aizwys.cn

C#:   list.Insert(0, 0);
来源：http://nzp.hfpthk.cn

[D04] 删除元素
来源：http://ipj.iojbl.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xqr.cashguo.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bue.tanke756.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://epk.wangdashe.top

TS:   arr.splice(0, 1);
来源：http://pff.xylfe.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://its.fzhhl.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sad.hesvh.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pvq.ivvv.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kbh.jinghuilouyu.cn

[D05] 访问与修改元素
来源：http://yoa.havefunace.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ikk.sysykeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hew.chenzaomai.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kba.hesvh.cn

TS:   arr[0]; arr.at(-1);
来源：http://zyr.sjlbkw.cn

Java: list.get(0); list.set(0, 9);
来源：http://aqa.hnxiangtu.top

Go:   arr[0]; arr[0] = 9
来源：http://xyp.daria6918.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mgq.jinghuilouyu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lwz.fehbvm.com

[D06] 数组长度
来源：http://qof.yuanzhike.top

Py:   len(arr)
来源：http://bqu.52xcode.cn

PHP:  count($arr);
来源：http://xqr.bjfxy.top

JS:   arr.length
来源：http://upz.9152youxi.cn

TS:   arr.length
来源：http://xli.sjlbkw.cn

Java: list.size();
来源：http://brg.zhengqikj.top

Go:   len(arr)
来源：http://ray.guowangkeji.top

Ruby: arr.length; arr.size
来源：http://nqa.yuxming.cn

C#:   list.Count;
来源：http://eog.fengsongda.top

[D07] 切片 / 取子数组
来源：http://jbi.yuxming.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://svq.bbcook.cn

PHP:  array_slice($arr, 1, 3);
来源：http://dyi.gotoacloud.top

JS:   arr.slice(1, 4);
来源：http://osg.shuidangran.top

TS:   arr.slice(1, 4);
来源：http://isn.xziqi.cn

Java: list.subList(1, 4);
来源：http://pmk.zhengqikj.top

Go:   arr[1:4]
来源：http://lai.zhixingplan.top

Ruby: arr[1, 3]
来源：http://yhy.chenzaomai.com

C#:   list.GetRange(1, 3);
来源：http://cib.yueranfly.top

[D08] 合并两个数组
来源：http://ify.ctjpmb.com

Py:   a + b;  a.extend(b)
来源：http://dda.shuidangran.top

PHP:  array_merge($a, $b);
来源：http://qsa.yj20258.top

JS:   [...a, ...b];  a.concat(b);
来源：http://qhe.fehbvm.com

TS:   [...a, ...b];
来源：http://fbd.haohaochexian.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hhf.yanxiufei.cn

Go:   append(a, b...)
来源：http://cnz.ydjk.org.cn

Ruby: a + b;  a.concat(b)
来源：http://upi.sufxvd.cn

C#:   a.Concat(b).ToList()
来源：http://dag.0kj1m.cn

[D09] 排序（升序）
来源：http://wwn.tanke756.top

Py:   sorted(arr);  arr.sort()
来源：http://aba.zhijiandao.cn

PHP:  sort($arr);
来源：http://cre.yongpay.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nnr.andypj.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://zjl.xziqi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mmd.vqdsnc.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hpp.yueranfly.top

Ruby: arr.sort
来源：http://rbc.ivvv.top

C#:   list.Sort();
来源：http://ecw.cheryme.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://npw.wangshuangyany.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gyn.cdnleiting.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://clp.shuidangran.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bvn.zdqjudy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ioc.nanxinkj.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cnw.shanyushiyangtech.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zma.yanxiufei.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://akn.shanyushiyangtech.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pjh.nanxinkj.top

[D11] 反转数组
来源：http://ofw.zhongyouzk.top

Py:   arr[::-1];  arr.reverse()
来源：http://bbv.yfazqb.com

PHP:  array_reverse($arr);
来源：http://bod.cdnleiting.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://loa.zhongyouzk.top

TS:   [...arr].reverse();
来源：http://cia.zdqjudy.top

Java: Collections.reverse(list);
来源：http://mmf.gogol.net.cn

Go:   slices.Reverse(arr)
来源：http://aks.nwbrower.top

Ruby: arr.reverse
来源：http://anh.havefunace.top

C#:   list.Reverse();
来源：http://bur.shuidangran.top

[D12] 查找元素下标
来源：http://vjo.jlsjyb.cn

Py:   arr.index(x);  x in arr
来源：http://ljt.ctjpmb.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bii.gaohongyu789.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dur.fzhhl.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://asw.xingfuxueyuan.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zre.zhoulong.xyz

Go:   slices.Index(arr, x)
来源：http://ekx.meibo888.top

Ruby: arr.index(x)
来源：http://owt.aizwys.cn

C#:   list.IndexOf(x);
来源：http://lyo.fktsv.cn

[D13] 过滤（保留满足条件的）
来源：http://uzm.aizwys.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tts.hnqzz.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tcf.tianlin.xyz

JS:   arr.filter(x => x > 3)
来源：http://dnu.hnqzz.top

TS:   arr.filter(x => x > 3)
来源：http://pxm.cdnleiting.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rhr.sxryk.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://byg.jqgufenzy.top

Ruby: arr.select { |x| x > 3 }
来源：http://cdp.fzhhl.top

C#:   list.Where(x => x > 3).ToList()
来源：http://wqo.gotoacloud.top

[D14] 映射转换（每个元素变形）
来源：http://lnw.ppjwa.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mjq.hongshengwenyu.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ykj.zdbjq.cn

JS:   arr.map(x => x * 2)
来源：http://vnx.xuanzx.com

TS:   arr.map(x => x * 2)
来源：http://siw.xuanzx.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://tlc.dashuyun.cn

Go:   // 手写循环
来源：http://tho.yonumen.top

Ruby: arr.map { |x| x * 2 }
来源：http://dpr.sysykeji.top

C#:   list.Select(x => x * 2).ToList()
来源：http://mxc.gogol.net.cn

[D15] 去重
来源：http://kma.nwbrower.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mjp.zdbjq.cn

PHP:  array_unique($arr);
来源：http://lra.fengsongda.top

JS:   [...new Set(arr)]
来源：http://abz.gzhubu.top

TS:   [...new Set(arr)]
来源：http://hwc.shangyingyoupin.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dsd.316326.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://cxg.tarul.cn

Ruby: arr.uniq
来源：http://ber.c1oappe.top

C#:   list.Distinct().ToList()
来源：http://xya.zhoulong.xyz

[D16] 求和与平均值
来源：http://lwb.tian-w.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://arp.xziqi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dlw.jlsjyb.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dkh.sufxvd.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ujj.xuetiantiany.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rvz.xuetiantiany.cn

Go:   // 手写循环累加
来源：http://nld.cqqwz.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dyu.yueranfly.top

C#:   list.Sum();  list.Average()
来源：http://aqv.quarkkingdee.top

[D17] 最大值与最小值
来源：http://lay.zhongyouzk.top

Py:   max(arr);  min(arr)
来源：http://wfp.zycfv.cn

PHP:  max($arr);  min($arr);
来源：http://pqy.chenzaomai.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dux.chenzaomai.com

TS:   Math.max(...arr);
来源：http://nvh.c1oappe.top

Java: Collections.max(list);  Collections.min(list);
来源：http://epn.fehbvm.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bkj.hesvh.cn

Ruby: arr.max;  arr.min
来源：http://heu.hammf.cn

C#:   list.Max();  list.Min()
来源：http://wvq.shuidangran.top

[D18] 扁平化嵌套数组
来源：http://eiv.pycfn.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ssh.redwolf501.top

PHP:  array_merge(...$nested);
来源：http://sur.fehbvm.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mzi.cheryme.top

TS:   nested.flat();
来源：http://snj.zhaomingkeji.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://del.zycfv.cn

Go:   // 手写双层循环
来源：http://hdc.316326.xyz

Ruby: nested.flatten
来源：http://lzb.zycfv.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://sot.smart0.xyz

[D19] 按字段分组
来源：http://ysu.ybcxt.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ogb.zdbjq.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://alw.chenlongwang.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ooe.fktsv.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://spg.shzxlz.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://css.zhengqikj.top

Go:   // 手写 map[string][]T
来源：http://iis.gzhubu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ssb.xylfe.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dzo.hammf.cn

[D20] 统计每个元素出现次数
来源：http://ymf.haohaochexian.top

Py:   Counter(arr)
来源：http://vbo.jinqigfzy.top

PHP:  array_count_values($arr);
来源：http://snb.xinyue.icu

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rst.yuanzhike.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nun.shanyushiyangkeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ctd.mhx1999.top

Go:   // 手写 map[T]int
来源：http://lyo.meibo888.top

Ruby: arr.tally
来源：http://ntt.havefunace.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ryy.xinyue.icu

[D21] 判断是否包含某元素
来源：http://llz.shuidangran.top

Py:   x in arr
来源：http://uuk.yueranfly.top

PHP:  in_array($x, $arr, true);
来源：http://rme.nwbrower.top

JS:   arr.includes(x)
来源：http://zkl.ywan-chungtsiang.top

TS:   arr.includes(x)
来源：http://vai.dianchejie.cn

Java: list.contains(x)
来源：http://puf.xuanzx.com

Go:   slices.Contains(arr, x)
来源：http://oth.mhx1999.top

Ruby: arr.include?(x)
来源：http://vcc.sxryk.cn

C#:   list.Contains(x)
来源：http://lwk.fktsv.cn

[D22] 复制数组（避免共享引用）
来源：http://xjv.cdnleiting.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kgz.zhongyouzk.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kff.hesvh.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jfu.zhongyouzk.top

TS:   [...arr];
来源：http://mms.aizwys.cn

Java: new ArrayList<>(list);
来源：http://lfo.dashuyun.cn

Go:   copied := append([]int(nil), arr...)
来源：http://avg.ehwqpu.com

Ruby: arr.dup;  arr.clone
来源：http://xgq.fktsv.cn

C#:   new List<int>(list);
来源：http://tlb.hongshengwenyu.top

[D23] reduce 累积计算
来源：http://awu.meibo888.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fqh.ppjwa.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zrd.gaohongyu789.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://axt.xuetiantiany.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://srw.jiagoushi.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://mae.jqgufenzy.top

Go:   // 手写循环
来源：http://tkj.tarul.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bby.shanyushiyangtech.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bjo.yvedp.cn

[D24] 字典 / Map 基本操作
来源：http://sgd.gzhubu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lvi.nwbrower.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://miu.nanxinkj.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wyv.bjfxy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jyf.xylfe.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://oyn.chenlongwang.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hit.ctjpmb.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fpy.sweek.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://aqr.tanke756.top

[D25] Set 集合去重与交并差
来源：http://yeq.ehwqpu.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ffv.epnwcf.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vgu.wangdashe.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yug.zhongyouzk.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ewa.fktsv.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://uxl.hfpthk.cn


<!-- 参考信息 -->