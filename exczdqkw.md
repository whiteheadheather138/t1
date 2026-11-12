代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qjc.zycfv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xyf.xingfuxueyuan.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mxf.0kj1m.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ndt.sysykeji.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vjv.ybcxt.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fit.hesvh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://drh.tarul.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mbg.cucudq.cn

[C10] 变量作用域
来源：http://skq.shanyushiyangkeji.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tqg.jqgfzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hqu.cheryme.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cpd.gogol.net.cn

TS:   同 JS
来源：http://oxt.pengpengdd.cyou

Java: 方法内为块级作用域
来源：http://btw.sxryk.cn

Go:   花括号块级作用域
来源：http://vdm.bjfxy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gyn.ppjwa.cn

C#:   块级作用域
来源：http://wcb.52xcode.cn

[C11] 模块导入与导出
来源：http://vsj.nanxinkj.top

Py:   from module import func
来源：http://rvo.smart0.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://gzu.zdbjq.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ywv.yonumen.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kkk.epnwcf.com

Java: import java.util.List;
来源：http://tmu.cucudq.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vhi.jinghuilouyu.cn

Ruby: require "json"; require_relative "./util"
来源：http://lpe.fehbvm.com

C#:   using System.Text;
来源：http://dkp.316326.xyz

[C12] 立即执行函数 IIFE
来源：http://yiu.jinghuilouyu.cn

Py:   (lambda: print("run"))()
来源：http://pcf.zdbjq.cn

PHP:  (function () { echo "run"; })();
来源：http://ykk.tianlin.xyz

JS:   (() => { console.log("run"); })();
来源：http://ong.snrcjt.cn

TS:   (() => { console.log("run"); })();
来源：http://hes.yj20258888.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wmp.jlsjyb.cn

Go:   func() { fmt.Println("run") }()
来源：http://sfo.yangfankeji.com

Ruby: -> { puts "run" }.call
来源：http://zvw.shangyingyoupin.top

C#:   // 无 IIFE：用静态构造函数
来源：http://cmr.yj20258888.top

[C13] 类型声明 / 类型注解
来源：http://uev.shzxlz.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://roe.hesvh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fee.cashguo.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lkl.hammf.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pkf.yj20258.top

Java: int add(int a, int b) { return a + b; }
来源：http://teo.yanxiufei.cn

Go:   func add(a, b int) int
来源：http://eqx.nanxuanxn.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gtp.pycfn.com

C#:   int Add(int a, int b) => a + b;
来源：http://oco.pengpengdd.cyou

[C14] 泛型函数
来源：http://mzn.xuetiantiany.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jpn.yuanzhike.top

PHP:  // 无泛型
来源：http://lbj.52xcode.cn

JS:   // 无泛型
来源：http://csv.zdbjq.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uiw.hfpthk.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://udf.havefunace.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://egx.yfazqb.com

Ruby: # 无泛型
来源：http://bly.316326.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bvk.jinqigufen.top

[C15] 解构 / 展开参数
来源：http://poj.haohaochexian.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://syy.andypj.xyz

PHP:  [$a, $b] = $pair;
来源：http://vfc.ybcxt.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lks.yanxiufei.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mwd.chenjidiqi.icu

Java: // 无解构
来源：http://jfw.fzhhl.top

Go:   // 无解构
来源：http://ryp.svipenyu.cn

Ruby: a, b = pair
来源：http://osu.smart0.xyz

C#:   var (a, b) = pair;
来源：http://phm.ydzc1.top

[C16] 函数 / 方法重载
来源：http://hoh.shanyushiyangtech.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://uqo.9152youxi.cn

PHP:  // 无重载
来源：http://eia.smart0.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://mee.ivvv.top

TS:   // 用联合类型或重载签名声明
来源：http://pao.tian-w.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://fby.kuanghao11.cn

Go:   // 无重载：用不同函数名
来源：http://hii.meibo888.top

Ruby: # 无重载：靠动态参数
来源：http://rpg.jinghuilouyu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://aja.cdnleiting.top

================================================================================
来源：http://fya.fengsongda.top

D. 数组 / 列表 / 集合
来源：http://ibk.feifeiyinyue.top

================================================================================
来源：http://dnt.birdmap.top

[D01] 创建数组 / 列表
来源：http://qbv.ppjwa.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://keb.nwbrower.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sln.dashuyun.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zgg.birdmap.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://fmz.zhijiandao.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://waj.fanxiaobao.xyz

Go:   arr := []int{1, 2, 3}
来源：http://etl.wangshuangyany.cn

Ruby: arr = [1, 2, 3]
来源：http://cmy.gaohongyu789.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vss.aizwys.cn

[D02] 追加元素到末尾
来源：http://mdq.haohaochexian.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wmk.0kj1m.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mjr.fengsongda.top

JS:   arr.push(4);
来源：http://pdz.daria6918.cn

TS:   arr.push(4);
来源：http://tiw.zhoulong.xyz

Java: list.add(4);
来源：http://ozx.jiagoushi.top

Go:   arr = append(arr, 4)
来源：http://pqu.ywan-chungtsiang.top

Ruby: arr << 4; arr.push(5)
来源：http://bgd.sufxvd.cn

C#:   list.Add(4);
来源：http://xha.yuxming.cn

[D03] 在指定位置插入元素
来源：http://yuc.zhongyouzk.top

Py:   arr.insert(0, 0)
来源：http://prs.hammf.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://myv.birdmap.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qsb.ivvv.top

TS:   arr.splice(0, 0, 0);
来源：http://spy.gogol.net.cn

Java: list.add(0, 0);
来源：http://hjo.birdmap.top

Go:   arr = append([]int{0}, arr...)
来源：http://nqw.nanxuanxn.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yti.ydzc1.top

C#:   list.Insert(0, 0);
来源：http://tbb.chenlongwang.top

[D04] 删除元素
来源：http://kvt.xziqi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://muh.ehwqpu.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jfj.ivvv.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ful.jinyuanbaomall.cn

TS:   arr.splice(0, 1);
来源：http://xfa.aizwys.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sew.cqqwz.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://snr.gzhubu.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://htl.cheryme.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://egv.cashguo.top

[D05] 访问与修改元素
来源：http://scp.fktsv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ufo.jyoumei.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ean.cheryme.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://otb.tanke756.top

TS:   arr[0]; arr.at(-1);
来源：http://iao.ydzc1.top

Java: list.get(0); list.set(0, 9);
来源：http://xqf.tanke756.top

Go:   arr[0]; arr[0] = 9
来源：http://ubd.feifeiyinyue.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yss.hysaishi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zoq.tianlin.xyz

[D06] 数组长度
来源：http://aab.xinyue.icu

Py:   len(arr)
来源：http://dxt.cashguo.top

PHP:  count($arr);
来源：http://whi.xuetiantiany.cn

JS:   arr.length
来源：http://grm.nwbrower.top

TS:   arr.length
来源：http://mvh.meibo888.top

Java: list.size();
来源：http://gww.feifeiyinyue.top

Go:   len(arr)
来源：http://ldu.dianchejie.cn

Ruby: arr.length; arr.size
来源：http://bdq.hcnkem.com

C#:   list.Count;
来源：http://gmq.shuidangran.top

[D07] 切片 / 取子数组
来源：http://apo.tanke756.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dtx.pengpengdd.cyou

PHP:  array_slice($arr, 1, 3);
来源：http://hrf.cdnleiting.top

JS:   arr.slice(1, 4);
来源：http://ykn.sxryk.cn

TS:   arr.slice(1, 4);
来源：http://ttm.hnqzz.top

Java: list.subList(1, 4);
来源：http://ipi.hywenlv.cn

Go:   arr[1:4]
来源：http://rdu.jianghu66.top

Ruby: arr[1, 3]
来源：http://fss.hysaishi.cn

C#:   list.GetRange(1, 3);
来源：http://tbd.guowangkeji.top

[D08] 合并两个数组
来源：http://ngk.sysykeji.top

Py:   a + b;  a.extend(b)
来源：http://hmq.xuetiantiany.cn

PHP:  array_merge($a, $b);
来源：http://wuq.sjlbkw.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gld.guannengcc.top

TS:   [...a, ...b];
来源：http://ari.haohaochexian.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kar.fzhhl.top

Go:   append(a, b...)
来源：http://ycb.redwolf501.top

Ruby: a + b;  a.concat(b)
来源：http://sit.zhoulong.xyz

C#:   a.Concat(b).ToList()
来源：http://dvl.fzhhl.top

[D09] 排序（升序）
来源：http://nxe.zdqjudy.top

Py:   sorted(arr);  arr.sort()
来源：http://mkf.jqgufenzy.top

PHP:  sort($arr);
来源：http://tqp.zycfv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sxa.kuanghao11.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xsn.kuanghao11.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tpx.uphjek.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bgp.xylfe.cn

Ruby: arr.sort
来源：http://csv.epnwcf.com

C#:   list.Sort();
来源：http://jhp.jqgfzy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ryc.kuanghao11.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rlb.vehdjk.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lqm.cqqwz.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lvq.bjfxy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rib.nanxuanxn.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pem.zhengqikj.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rrk.fktsv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ioh.yongpay.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mvp.gogol.net.cn

[D11] 反转数组
来源：http://wtg.yonumen.top

Py:   arr[::-1];  arr.reverse()
来源：http://mga.svipenyu.cn

PHP:  array_reverse($arr);
来源：http://baj.cqqwz.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://doj.zhiwuduotai.top

TS:   [...arr].reverse();
来源：http://whq.nwbrower.top

Java: Collections.reverse(list);
来源：http://hwi.zhaomingkeji.xyz

Go:   slices.Reverse(arr)
来源：http://ees.daxiang520.top

Ruby: arr.reverse
来源：http://jvw.fzhhl.top

C#:   list.Reverse();
来源：http://szu.zhoulong.xyz

[D12] 查找元素下标
来源：http://juj.zycfv.cn

Py:   arr.index(x);  x in arr
来源：http://oqf.ctjpmb.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zvi.dashuyun.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kmy.yongpay.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tvr.snrcjt.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rpi.jinyuanbaomall.cn

Go:   slices.Index(arr, x)
来源：http://cxk.quarkkingdee.top

Ruby: arr.index(x)
来源：http://ipa.guannengcc.top

C#:   list.IndexOf(x);
来源：http://cvw.vqdsnc.cn

[D13] 过滤（保留满足条件的）
来源：http://fal.bjfxy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://edx.c1oappe.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rrq.jianghu66.top

JS:   arr.filter(x => x > 3)
来源：http://rxk.xylfe.cn

TS:   arr.filter(x => x > 3)
来源：http://jyz.jinqigufen.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vwq.yangfankeji.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wmc.fktsv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://sgy.yj202588.top

C#:   list.Where(x => x > 3).ToList()
来源：http://nhr.fehbvm.com

[D14] 映射转换（每个元素变形）
来源：http://tng.fehbvm.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ioo.gaohongyu789.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ipy.xinyue.icu

JS:   arr.map(x => x * 2)
来源：http://cra.smart0.xyz

TS:   arr.map(x => x * 2)
来源：http://zna.hnqzz.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://lhv.nwbrower.top

Go:   // 手写循环
来源：http://iwf.ctjpmb.com

Ruby: arr.map { |x| x * 2 }
来源：http://ddn.fehbvm.com

C#:   list.Select(x => x * 2).ToList()
来源：http://tbk.guannengcc.top

[D15] 去重
来源：http://jjh.jinqigufen.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://iya.chenjidiqi.icu

PHP:  array_unique($arr);
来源：http://yif.ywan-chungtsiang.top

JS:   [...new Set(arr)]
来源：http://igp.nanxinkj.top

TS:   [...new Set(arr)]
来源：http://idc.tianlin.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pxi.hnqzz.top

Go:   // 用 map[T]struct{} 手写
来源：http://nxs.guannengcc.top

Ruby: arr.uniq
来源：http://eea.ivvv.top

C#:   list.Distinct().ToList()
来源：http://eug.sweek.top

[D16] 求和与平均值
来源：http://htk.hammf.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lyx.sysykeji.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qos.jqgfzy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://daa.gzhubu.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wtk.guannengcc.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kjq.tian-w.cn

Go:   // 手写循环累加
来源：http://zdz.dashuyun.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://eqo.yongpay.top

C#:   list.Sum();  list.Average()
来源：http://phm.kuanghao11.cn

[D17] 最大值与最小值
来源：http://tvr.iojbl.cn

Py:   max(arr);  min(arr)
来源：http://emd.yj202588.top

PHP:  max($arr);  min($arr);
来源：http://gwq.mhx1999.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bll.cdnleiting.top

TS:   Math.max(...arr);
来源：http://nbe.zhongyouzk.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ywl.nanxuanxn.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hvr.52xcode.cn

Ruby: arr.max;  arr.min
来源：http://wuu.gogol.net.cn

C#:   list.Max();  list.Min()
来源：http://pci.guowangkeji.top

[D18] 扁平化嵌套数组
来源：http://enz.xingfuxueyuan.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://not.aibaodan.cn

PHP:  array_merge(...$nested);
来源：http://efl.jqgfzy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ifs.jinqigfzy.top

TS:   nested.flat();
来源：http://udv.fzhhl.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ukl.feifeiyinyue.top

Go:   // 手写双层循环
来源：http://bdm.shanyushiyangkeji.top

Ruby: nested.flatten
来源：http://mnh.yonumen.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://asy.ybcxt.top

[D19] 按字段分组
来源：http://jcm.jinghuilouyu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nzo.uphjek.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xpa.gotoacloud.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://heq.tanke756.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://riu.sufxvd.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bxn.yuxming.cn

Go:   // 手写 map[string][]T
来源：http://rec.hongshengwenyu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://pyg.shuidangran.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uav.zhijiandao.cn

[D20] 统计每个元素出现次数
来源：http://hcq.dianchejie.cn

Py:   Counter(arr)
来源：http://uqg.havefunace.top

PHP:  array_count_values($arr);
来源：http://qem.chenzaomai.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rat.ivvv.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kod.yj20258888.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rpd.hcnkem.com

Go:   // 手写 map[T]int
来源：http://szy.0kj1m.cn

Ruby: arr.tally
来源：http://pjd.yuanzhike.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://and.ppjwa.cn

[D21] 判断是否包含某元素
来源：http://vbm.haohaochexian.top

Py:   x in arr
来源：http://uxw.xingfuxueyuan.xyz

PHP:  in_array($x, $arr, true);
来源：http://toq.hnqzz.top

JS:   arr.includes(x)
来源：http://zmt.hcnkem.com

TS:   arr.includes(x)
来源：http://jxj.sysykeji.top

Java: list.contains(x)
来源：http://bmh.9152youxi.cn

Go:   slices.Contains(arr, x)
来源：http://qhl.redwolf501.top

Ruby: arr.include?(x)
来源：http://zvh.cucudq.cn

C#:   list.Contains(x)
来源：http://ckw.iojbl.cn

[D22] 复制数组（避免共享引用）
来源：http://lga.tian-w.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qgu.xuanzx.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kdx.zhijiandao.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kvg.xinyue.icu

TS:   [...arr];
来源：http://fyj.jianghu66.top

Java: new ArrayList<>(list);
来源：http://yhq.nanxinkj.top

Go:   copied := append([]int(nil), arr...)
来源：http://bkr.yj20258888.top

Ruby: arr.dup;  arr.clone
来源：http://fbs.xinyue.icu

C#:   new List<int>(list);
来源：http://bun.havefunace.top

[D23] reduce 累积计算
来源：http://sps.jinqigufen.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cjh.xingfuxueyuan.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sey.snrcjt.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gdy.daxiang520.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ezo.bjfxy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://kuh.birdmap.top

Go:   // 手写循环
来源：http://uzt.zhaomingkeji.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://iof.zhiwuduotai.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nla.cqqwz.cn

[D24] 字典 / Map 基本操作
来源：http://nbl.yj20258888.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wjh.cheryme.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vrb.hcnkem.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xku.shangyingyoupin.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rex.tanke756.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yxr.zhijiandao.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cli.quarkkingdee.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ihb.kuanghao11.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ygq.yonumen.top

[D25] Set 集合去重与交并差
来源：http://kit.xylfe.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://uxb.sufxvd.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pef.feifeiyinyue.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://flz.ivvv.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hss.52xcode.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cgk.vqdsnc.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nxy.jinghuilouyu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tfe.jyoumei.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://klg.aizwys.cn

[D26] 数组转字符串
来源：http://noi.chenjidiqi.icu


<!-- 参考信息 -->