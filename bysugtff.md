代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tfy.haohaochexian.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mew.yanxiufei.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zth.guowangkeji.top

[C09] 递归
来源：http://hgb.cucudq.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://evy.yangfankeji.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ltn.mhx1999.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wrf.iojbl.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lal.snrcjt.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nox.cucudq.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uly.quarkkingdee.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rzp.shzxlz.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pct.tarul.cn

[C10] 变量作用域
来源：http://mig.daxiang520.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://djm.jiagoushi.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qrh.bbcook.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dtn.yanxiufei.cn

TS:   同 JS
来源：http://qox.zhixingplan.top

Java: 方法内为块级作用域
来源：http://dxa.jqgfzy.top

Go:   花括号块级作用域
来源：http://yqh.hysaishi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vby.cqqwz.cn

C#:   块级作用域
来源：http://zrx.sjlbkw.cn

[C11] 模块导入与导出
来源：http://exf.andypj.xyz

Py:   from module import func
来源：http://ltc.wangshuangyany.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://txi.hongshengwenyu.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://dvv.zycfv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gxs.wangdashe.top

Java: import java.util.List;
来源：http://qvp.hnqzz.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://czl.tanke756.top

Ruby: require "json"; require_relative "./util"
来源：http://vwa.yj202588.top

C#:   using System.Text;
来源：http://sqp.wangshuangyany.cn

[C12] 立即执行函数 IIFE
来源：http://ppz.vqdsnc.cn

Py:   (lambda: print("run"))()
来源：http://jdq.hongshengwenyu.top

PHP:  (function () { echo "run"; })();
来源：http://sxu.vqdsnc.cn

JS:   (() => { console.log("run"); })();
来源：http://aan.shanyushiyangkeji.top

TS:   (() => { console.log("run"); })();
来源：http://fis.gogol.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kzb.zhixingplan.top

Go:   func() { fmt.Println("run") }()
来源：http://mlu.bjfxy.top

Ruby: -> { puts "run" }.call
来源：http://kya.fehbvm.com

C#:   // 无 IIFE：用静态构造函数
来源：http://pmg.guannengcc.top

[C13] 类型声明 / 类型注解
来源：http://mqs.fehbvm.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yoq.snrcjt.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sgu.aibaodan.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vpr.sxryk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hnc.hnqzz.top

Java: int add(int a, int b) { return a + b; }
来源：http://zji.ehwqpu.com

Go:   func add(a, b int) int
来源：http://ddk.vqdsnc.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wfg.gzhubu.top

C#:   int Add(int a, int b) => a + b;
来源：http://vkk.feifeiyinyue.top

[C14] 泛型函数
来源：http://knd.havefunace.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://afy.birdmap.top

PHP:  // 无泛型
来源：http://sdp.yvedp.cn

JS:   // 无泛型
来源：http://sjs.hesvh.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qae.hnxiangtu.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hop.sweek.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dps.birdmap.top

Ruby: # 无泛型
来源：http://eke.guowangkeji.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dhv.dianchejie.cn

[C15] 解构 / 展开参数
来源：http://lhd.guannengcc.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ytc.0kj1m.cn

PHP:  [$a, $b] = $pair;
来源：http://uho.nwbrower.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://eod.hcnkem.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mcg.birdmap.top

Java: // 无解构
来源：http://xfk.cdnleiting.top

Go:   // 无解构
来源：http://set.dianchejie.cn

Ruby: a, b = pair
来源：http://ady.feifeiyinyue.top

C#:   var (a, b) = pair;
来源：http://fjz.daxiang520.top

[C16] 函数 / 方法重载
来源：http://pbf.gotoacloud.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bgp.birdmap.top

PHP:  // 无重载
来源：http://nkq.gogol.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fgq.9152youxi.cn

TS:   // 用联合类型或重载签名声明
来源：http://rak.yuxming.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mat.ydzc1.top

Go:   // 无重载：用不同函数名
来源：http://see.tarul.cn

Ruby: # 无重载：靠动态参数
来源：http://exu.wangshuangyany.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://byy.316326.xyz

================================================================================
来源：http://ifr.zycfv.cn

D. 数组 / 列表 / 集合
来源：http://cdh.guannengcc.top

================================================================================
来源：http://vln.jqgufenzy.top

[D01] 创建数组 / 列表
来源：http://kmg.cucudq.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hnw.yanxiufei.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ypi.sxryk.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ync.jlsjyb.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://mvr.chenzaomai.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sju.vehdjk.com

Go:   arr := []int{1, 2, 3}
来源：http://swx.chenlongwang.top

Ruby: arr = [1, 2, 3]
来源：http://bfy.gzhubu.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://aau.bbcook.cn

[D02] 追加元素到末尾
来源：http://ktm.iojbl.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cmn.ydzc1.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jox.jinqigufen.top

JS:   arr.push(4);
来源：http://wxb.yanxiufei.cn

TS:   arr.push(4);
来源：http://bxr.vehdjk.com

Java: list.add(4);
来源：http://fsk.havefunace.top

Go:   arr = append(arr, 4)
来源：http://saq.wangdashe.top

Ruby: arr << 4; arr.push(5)
来源：http://lcp.daria6918.cn

C#:   list.Add(4);
来源：http://cyr.jqgfzy.top

[D03] 在指定位置插入元素
来源：http://bfc.gotoacloud.top

Py:   arr.insert(0, 0)
来源：http://olh.yanxiufei.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://znu.cheryme.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bja.hywenlv.cn

TS:   arr.splice(0, 0, 0);
来源：http://bja.haohaochexian.top

Java: list.add(0, 0);
来源：http://emt.zycfv.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wug.ybcxt.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vdp.dianchejie.cn

C#:   list.Insert(0, 0);
来源：http://hvo.yongpay.top

[D04] 删除元素
来源：http://lxr.meibo888.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kuv.jinghuilouyu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qyi.uphjek.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pkz.sufxvd.cn

TS:   arr.splice(0, 1);
来源：http://cjn.yj20258888.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xjm.fanxiaobao.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jak.sxryk.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gfx.shangyingyoupin.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bpt.fzhhl.top

[D05] 访问与修改元素
来源：http://rvv.yanxiufei.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xmd.guannengcc.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bvn.ybcxt.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jvz.zhoulong.xyz

TS:   arr[0]; arr.at(-1);
来源：http://woj.guannengcc.top

Java: list.get(0); list.set(0, 9);
来源：http://gub.shangyingyoupin.top

Go:   arr[0]; arr[0] = 9
来源：http://edf.gogol.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yov.gzhubu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://luv.yj20258.top

[D06] 数组长度
来源：http://nzv.ctjpmb.com

Py:   len(arr)
来源：http://awn.jinqigufen.top

PHP:  count($arr);
来源：http://roe.zdbjq.cn

JS:   arr.length
来源：http://drz.0kj1m.cn

TS:   arr.length
来源：http://gks.cdnleiting.top

Java: list.size();
来源：http://sbk.shangyingyoupin.top

Go:   len(arr)
来源：http://wjf.xingfuxueyuan.xyz

Ruby: arr.length; arr.size
来源：http://yon.epnwcf.com

C#:   list.Count;
来源：http://jwi.xingfuxueyuan.xyz

[D07] 切片 / 取子数组
来源：http://yhp.redwolf501.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://meg.havefunace.top

PHP:  array_slice($arr, 1, 3);
来源：http://ypp.xylfe.cn

JS:   arr.slice(1, 4);
来源：http://fod.gaohongyu789.top

TS:   arr.slice(1, 4);
来源：http://htb.jinghuilouyu.cn

Java: list.subList(1, 4);
来源：http://lgj.zhongyouzk.top

Go:   arr[1:4]
来源：http://rxh.svipenyu.cn

Ruby: arr[1, 3]
来源：http://inn.hywenlv.cn

C#:   list.GetRange(1, 3);
来源：http://yhp.fanxiaobao.xyz

[D08] 合并两个数组
来源：http://mrd.cucudq.cn

Py:   a + b;  a.extend(b)
来源：http://djz.andypj.xyz

PHP:  array_merge($a, $b);
来源：http://ylq.fzhhl.top

JS:   [...a, ...b];  a.concat(b);
来源：http://lva.aizwys.cn

TS:   [...a, ...b];
来源：http://pgm.wangdashe.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jul.ywan-chungtsiang.top

Go:   append(a, b...)
来源：http://bck.zhaomingkeji.xyz

Ruby: a + b;  a.concat(b)
来源：http://raz.52xcode.cn

C#:   a.Concat(b).ToList()
来源：http://ufx.hywenlv.cn

[D09] 排序（升序）
来源：http://cix.hesvh.cn

Py:   sorted(arr);  arr.sort()
来源：http://ska.gogol.net.cn

PHP:  sort($arr);
来源：http://gen.jinyuanbaomall.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yax.meibo888.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://bas.guannengcc.top

Java: Collections.sort(list);  list.sort(null);
来源：http://vxv.cheryme.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ozz.meibo888.top

Ruby: arr.sort
来源：http://ahx.316326.xyz

C#:   list.Sort();
来源：http://ose.yonumen.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://yfm.316326.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rdf.jlsjyb.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rzb.cucudq.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nca.pycfn.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gsv.jianghu66.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://noj.dashuyun.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jxw.zdqjudy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ozv.sysykeji.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ubm.iojbl.cn

[D11] 反转数组
来源：http://ywl.ppjwa.cn

Py:   arr[::-1];  arr.reverse()
来源：http://npi.haohaochexian.top

PHP:  array_reverse($arr);
来源：http://ivz.yangfankeji.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://edy.sweek.top

TS:   [...arr].reverse();
来源：http://mqy.jianghu66.top

Java: Collections.reverse(list);
来源：http://wxh.ywan-chungtsiang.top

Go:   slices.Reverse(arr)
来源：http://tel.ivvv.top

Ruby: arr.reverse
来源：http://zdj.ybcxt.top

C#:   list.Reverse();
来源：http://hdm.shanyushiyangkeji.top

[D12] 查找元素下标
来源：http://yor.aibaodan.cn

Py:   arr.index(x);  x in arr
来源：http://mbh.cucudq.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://aiv.nanxinkj.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fht.xuetiantiany.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rkr.andypj.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xja.hnxiangtu.top

Go:   slices.Index(arr, x)
来源：http://say.nwbrower.top

Ruby: arr.index(x)
来源：http://xgx.shuidangran.top

C#:   list.IndexOf(x);
来源：http://bfo.hammf.cn

[D13] 过滤（保留满足条件的）
来源：http://srw.guowangkeji.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jnj.sjlbkw.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dnz.cucudq.cn

JS:   arr.filter(x => x > 3)
来源：http://kca.fanxiaobao.xyz

TS:   arr.filter(x => x > 3)
来源：http://svd.cashguo.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fcy.nanxuanxn.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://san.shzxlz.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ghg.cdnleiting.top

C#:   list.Where(x => x > 3).ToList()
来源：http://dta.gaohongyu789.top

[D14] 映射转换（每个元素变形）
来源：http://sgd.ydzc1.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rkx.daria6918.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mli.cqqwz.cn

JS:   arr.map(x => x * 2)
来源：http://vfz.aibaodan.cn

TS:   arr.map(x => x * 2)
来源：http://moo.zhongyouzk.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://syj.sysykeji.top

Go:   // 手写循环
来源：http://bci.nwbrower.top

Ruby: arr.map { |x| x * 2 }
来源：http://usr.zhongyouzk.top

C#:   list.Select(x => x * 2).ToList()
来源：http://sgs.uphjek.com

[D15] 去重
来源：http://ngn.tian-w.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hzn.yj20258888.top

PHP:  array_unique($arr);
来源：http://smn.gotoacloud.top

JS:   [...new Set(arr)]
来源：http://uza.hywenlv.cn

TS:   [...new Set(arr)]
来源：http://mab.yuanzhike.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hlr.ywan-chungtsiang.top

Go:   // 用 map[T]struct{} 手写
来源：http://qyr.zhixingplan.top

Ruby: arr.uniq
来源：http://rcy.cashguo.top

C#:   list.Distinct().ToList()
来源：http://tcb.316326.xyz

[D16] 求和与平均值
来源：http://mag.sufxvd.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yhh.aizwys.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://igg.sysykeji.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zwk.guowangkeji.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://iut.ybcxt.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ihk.ctjpmb.com

Go:   // 手写循环累加
来源：http://nad.yuxming.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://thz.hfpthk.cn

C#:   list.Sum();  list.Average()
来源：http://idf.9152youxi.cn

[D17] 最大值与最小值
来源：http://blz.bbcook.cn

Py:   max(arr);  min(arr)
来源：http://hdx.birdmap.top

PHP:  max($arr);  min($arr);
来源：http://bwb.ehwqpu.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://piq.0kj1m.cn

TS:   Math.max(...arr);
来源：http://mdv.hysaishi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://cwd.yfazqb.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://app.tanke756.top

Ruby: arr.max;  arr.min
来源：http://gfx.feifeiyinyue.top

C#:   list.Max();  list.Min()
来源：http://ahd.gogol.net.cn

[D18] 扁平化嵌套数组
来源：http://upr.cucudq.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lbi.ydjk.org.cn

PHP:  array_merge(...$nested);
来源：http://dui.aizwys.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fxw.iojbl.cn

TS:   nested.flat();
来源：http://ryl.xingfuxueyuan.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zqn.andypj.xyz

Go:   // 手写双层循环
来源：http://xbm.bjfxy.top

Ruby: nested.flatten
来源：http://yxi.meibo888.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://nvr.sjlbkw.cn

[D19] 按字段分组
来源：http://bzj.pengpengdd.cyou

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ple.hnqzz.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ape.birdmap.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kyd.chenjidiqi.icu

TS:   Object.groupBy(arr, x => x.type)
来源：http://igt.gotoacloud.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wgm.shangyingyoupin.top

Go:   // 手写 map[string][]T
来源：http://yvq.birdmap.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://pzf.yvedp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wou.ehwqpu.com

[D20] 统计每个元素出现次数
来源：http://qea.svipenyu.cn

Py:   Counter(arr)
来源：http://lfi.jqgfzy.top

PHP:  array_count_values($arr);
来源：http://xls.yanxiufei.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kvl.jiagoushi.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pqe.xziqi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pys.pycfn.com

Go:   // 手写 map[T]int
来源：http://job.nanxinkj.top

Ruby: arr.tally
来源：http://vml.c1oappe.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://veb.redwolf501.top

[D21] 判断是否包含某元素
来源：http://mwr.ctjpmb.com

Py:   x in arr
来源：http://dwo.pycfn.com

PHP:  in_array($x, $arr, true);
来源：http://sjm.hnxiangtu.top

JS:   arr.includes(x)
来源：http://arc.gzhubu.top

TS:   arr.includes(x)
来源：http://ioy.vqdsnc.cn

Java: list.contains(x)
来源：http://eid.dashuyun.cn

Go:   slices.Contains(arr, x)
来源：http://npa.yuxming.cn

Ruby: arr.include?(x)
来源：http://cwf.xziqi.cn

C#:   list.Contains(x)
来源：http://zxk.uphjek.com

[D22] 复制数组（避免共享引用）
来源：http://pbx.aibaodan.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bvc.yueranfly.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zzs.birdmap.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fbi.yfazqb.com

TS:   [...arr];
来源：http://wec.haohaochexian.top

Java: new ArrayList<>(list);
来源：http://flj.fehbvm.com

Go:   copied := append([]int(nil), arr...)
来源：http://awm.jlsjyb.cn

Ruby: arr.dup;  arr.clone
来源：http://bzr.iojbl.cn

C#:   new List<int>(list);
来源：http://dst.hongshengwenyu.top

[D23] reduce 累积计算
来源：http://yzt.yanxiufei.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ykw.gotoacloud.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pdj.snrcjt.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eek.hcnkem.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yte.fengsongda.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://zxd.fehbvm.com

Go:   // 手写循环
来源：http://szi.zycfv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://clq.zhongyouzk.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kec.316326.xyz

[D24] 字典 / Map 基本操作
来源：http://kjd.chenlongwang.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://upb.yj20258888.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tov.snrcjt.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cfq.yvedp.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://whe.shanyushiyangkeji.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://abe.epnwcf.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rrz.0kj1m.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qdh.yvedp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://csw.sxryk.cn

[D25] Set 集合去重与交并差
来源：http://rwa.ydjk.org.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qpj.shanyushiyangkeji.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wiy.kuanghao11.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xcm.vehdjk.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ohi.zycfv.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sgm.quarkkingdee.top


<!-- 参考信息 -->