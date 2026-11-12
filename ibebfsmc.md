代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://whl.yueranfly.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zaj.shuidangran.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vpp.feifeiyinyue.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qub.pengpengdd.cyou

[C10] 变量作用域
来源：http://eys.zhongyouzk.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fvk.hysaishi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wyi.sjlbkw.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dzi.redwolf501.top

TS:   同 JS
来源：http://apg.yueranfly.top

Java: 方法内为块级作用域
来源：http://fov.cqqwz.cn

Go:   花括号块级作用域
来源：http://cbl.jinyuanbaomall.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nrn.52xcode.cn

C#:   块级作用域
来源：http://cqo.hesvh.cn

[C11] 模块导入与导出
来源：http://ebx.shzxlz.cn

Py:   from module import func
来源：http://dhr.zhiwuduotai.top

PHP:  require "file.php";  或 use App\Service;
来源：http://sib.gogol.net.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://cne.aizwys.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bzn.nanxinkj.top

Java: import java.util.List;
来源：http://vzz.jlsjyb.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gts.ywan-chungtsiang.top

Ruby: require "json"; require_relative "./util"
来源：http://key.ydjk.org.cn

C#:   using System.Text;
来源：http://zfk.9152youxi.cn

[C12] 立即执行函数 IIFE
来源：http://svw.zhiwuduotai.top

Py:   (lambda: print("run"))()
来源：http://sdx.guowangkeji.top

PHP:  (function () { echo "run"; })();
来源：http://tyz.cashguo.top

JS:   (() => { console.log("run"); })();
来源：http://laf.snrcjt.cn

TS:   (() => { console.log("run"); })();
来源：http://sdz.andypj.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xjx.yonumen.top

Go:   func() { fmt.Println("run") }()
来源：http://cbw.daxiang520.top

Ruby: -> { puts "run" }.call
来源：http://jox.zycfv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://aqz.ctjpmb.com

[C13] 类型声明 / 类型注解
来源：http://mzl.snrcjt.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bsl.hywenlv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zfd.9152youxi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ale.yvedp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pqf.yangfankeji.com

Java: int add(int a, int b) { return a + b; }
来源：http://pvz.yonumen.top

Go:   func add(a, b int) int
来源：http://tbl.epnwcf.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dqa.cdnleiting.top

C#:   int Add(int a, int b) => a + b;
来源：http://iwt.fanxiaobao.xyz

[C14] 泛型函数
来源：http://aog.bbcook.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wtd.nanxinkj.top

PHP:  // 无泛型
来源：http://pcr.hysaishi.cn

JS:   // 无泛型
来源：http://wpf.52xcode.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xmv.hongshengwenyu.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dhm.ivvv.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mko.fanxiaobao.xyz

Ruby: # 无泛型
来源：http://gfr.9152youxi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cqg.zhijiandao.cn

[C15] 解构 / 展开参数
来源：http://oxn.52xcode.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dpd.havefunace.top

PHP:  [$a, $b] = $pair;
来源：http://wxp.hongshengwenyu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xpd.zhijiandao.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cjn.cucudq.cn

Java: // 无解构
来源：http://xla.dianchejie.cn

Go:   // 无解构
来源：http://flk.hnqzz.top

Ruby: a, b = pair
来源：http://wda.jqgfzy.top

C#:   var (a, b) = pair;
来源：http://zga.guannengcc.top

[C16] 函数 / 方法重载
来源：http://vgq.cheryme.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bkj.gaohongyu789.top

PHP:  // 无重载
来源：http://gdb.sxryk.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ifv.yangfankeji.com

TS:   // 用联合类型或重载签名声明
来源：http://joh.gaohongyu789.top

Java: void f(int a) {}  void f(String a) {}
来源：http://dyp.yanxiufei.cn

Go:   // 无重载：用不同函数名
来源：http://rqh.wangshuangyany.cn

Ruby: # 无重载：靠动态参数
来源：http://pln.nanxinkj.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://gvw.ppjwa.cn

================================================================================
来源：http://clx.shzxlz.cn

D. 数组 / 列表 / 集合
来源：http://mhj.yj20258888.top

================================================================================
来源：http://uxz.xuanzx.com

[D01] 创建数组 / 列表
来源：http://bac.yj20258.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://sqc.daria6918.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://afq.pengpengdd.cyou

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ica.tianlin.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://xnr.shanyushiyangkeji.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ars.svipenyu.cn

Go:   arr := []int{1, 2, 3}
来源：http://gph.cheryme.top

Ruby: arr = [1, 2, 3]
来源：http://rub.zhaomingkeji.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rec.zhongyouzk.top

[D02] 追加元素到末尾
来源：http://yrf.hysaishi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gmd.pycfn.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mrl.gaohongyu789.top

JS:   arr.push(4);
来源：http://vno.tarul.cn

TS:   arr.push(4);
来源：http://kyi.bjfxy.top

Java: list.add(4);
来源：http://ors.tanke756.top

Go:   arr = append(arr, 4)
来源：http://xqx.smart0.xyz

Ruby: arr << 4; arr.push(5)
来源：http://ixo.ydzc1.top

C#:   list.Add(4);
来源：http://bdn.tanke756.top

[D03] 在指定位置插入元素
来源：http://szs.daria6918.cn

Py:   arr.insert(0, 0)
来源：http://mgw.jinqigufen.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://muj.quarkkingdee.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://phc.jinghuilouyu.cn

TS:   arr.splice(0, 0, 0);
来源：http://lsw.bbcook.cn

Java: list.add(0, 0);
来源：http://odz.sxryk.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ldv.jinyuanbaomall.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://enn.birdmap.top

C#:   list.Insert(0, 0);
来源：http://dor.fzhhl.top

[D04] 删除元素
来源：http://ybj.xuanzx.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vmq.sweek.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ixb.zhiwuduotai.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lmg.shanyushiyangtech.top

TS:   arr.splice(0, 1);
来源：http://uzf.ivvv.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://psu.sysykeji.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jsq.smart0.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ehq.hnxiangtu.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://iom.hnqzz.top

[D05] 访问与修改元素
来源：http://ocl.fehbvm.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://iqk.uphjek.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://brc.hysaishi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mds.chenlongwang.top

TS:   arr[0]; arr.at(-1);
来源：http://zsl.tianlin.xyz

Java: list.get(0); list.set(0, 9);
来源：http://sez.andypj.xyz

Go:   arr[0]; arr[0] = 9
来源：http://pkg.tianlin.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wyl.yueranfly.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rix.daria6918.cn

[D06] 数组长度
来源：http://rfp.hfpthk.cn

Py:   len(arr)
来源：http://ozb.yonumen.top

PHP:  count($arr);
来源：http://odj.nanxuanxn.top

JS:   arr.length
来源：http://ght.sufxvd.cn

TS:   arr.length
来源：http://zov.bbcook.cn

Java: list.size();
来源：http://kmf.yuxming.cn

Go:   len(arr)
来源：http://tez.hesvh.cn

Ruby: arr.length; arr.size
来源：http://mdd.hcnkem.com

C#:   list.Count;
来源：http://fvn.shuidangran.top

[D07] 切片 / 取子数组
来源：http://tww.tanke756.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yww.nanxinkj.top

PHP:  array_slice($arr, 1, 3);
来源：http://vyj.vehdjk.com

JS:   arr.slice(1, 4);
来源：http://ctp.xingfuxueyuan.xyz

TS:   arr.slice(1, 4);
来源：http://otv.hnxiangtu.top

Java: list.subList(1, 4);
来源：http://ukr.sjlbkw.cn

Go:   arr[1:4]
来源：http://zei.xuetiantiany.cn

Ruby: arr[1, 3]
来源：http://nje.zhoulong.xyz

C#:   list.GetRange(1, 3);
来源：http://jxl.yvedp.cn

[D08] 合并两个数组
来源：http://ice.snrcjt.cn

Py:   a + b;  a.extend(b)
来源：http://hxa.guannengcc.top

PHP:  array_merge($a, $b);
来源：http://pmr.shuidangran.top

JS:   [...a, ...b];  a.concat(b);
来源：http://cpq.haohaochexian.top

TS:   [...a, ...b];
来源：http://wyh.fzhhl.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sxp.jlsjyb.cn

Go:   append(a, b...)
来源：http://pgi.birdmap.top

Ruby: a + b;  a.concat(b)
来源：http://cwh.shangyingyoupin.top

C#:   a.Concat(b).ToList()
来源：http://rlc.smart0.xyz

[D09] 排序（升序）
来源：http://ehb.xuanzx.com

Py:   sorted(arr);  arr.sort()
来源：http://ixm.snrcjt.cn

PHP:  sort($arr);
来源：http://xcf.chenlongwang.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://leo.zhijiandao.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://vnf.ydzc1.top

Java: Collections.sort(list);  list.sort(null);
来源：http://skv.xylfe.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lsi.yj20258888.top

Ruby: arr.sort
来源：http://hmx.hysaishi.cn

C#:   list.Sort();
来源：http://uto.yj202588.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://hvw.guannengcc.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wuv.zycfv.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qpd.chenlongwang.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://axp.pycfn.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xnw.yvedp.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jas.chenjidiqi.icu

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mqb.shanyushiyangtech.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ipp.hywenlv.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qfv.hcnkem.com

[D11] 反转数组
来源：http://nut.yj202588.top

Py:   arr[::-1];  arr.reverse()
来源：http://cjl.shanyushiyangtech.top

PHP:  array_reverse($arr);
来源：http://qvr.sweek.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ezb.cheryme.top

TS:   [...arr].reverse();
来源：http://emy.zdbjq.cn

Java: Collections.reverse(list);
来源：http://nvg.ywan-chungtsiang.top

Go:   slices.Reverse(arr)
来源：http://lmd.tanke756.top

Ruby: arr.reverse
来源：http://umq.yongpay.top

C#:   list.Reverse();
来源：http://ujt.sjlbkw.cn

[D12] 查找元素下标
来源：http://qbp.yfazqb.com

Py:   arr.index(x);  x in arr
来源：http://hgd.fengsongda.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xcm.0kj1m.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ebr.kuanghao11.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ils.shzxlz.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lyk.chenzaomai.com

Go:   slices.Index(arr, x)
来源：http://jmn.ydjk.org.cn

Ruby: arr.index(x)
来源：http://uzb.jinghuilouyu.cn

C#:   list.IndexOf(x);
来源：http://jgb.redwolf501.top

[D13] 过滤（保留满足条件的）
来源：http://ujf.9152youxi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nas.cdnleiting.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lri.birdmap.top

JS:   arr.filter(x => x > 3)
来源：http://ltw.jinqigfzy.top

TS:   arr.filter(x => x > 3)
来源：http://jrz.zhongyouzk.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qez.sufxvd.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cjh.nanxinkj.top

Ruby: arr.select { |x| x > 3 }
来源：http://pxj.9152youxi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bpp.aizwys.cn

[D14] 映射转换（每个元素变形）
来源：http://oxz.daxiang520.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cic.pengpengdd.cyou

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kmf.yanxiufei.cn

JS:   arr.map(x => x * 2)
来源：http://ytk.ydjk.org.cn

TS:   arr.map(x => x * 2)
来源：http://lgn.jinqigufen.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://zdo.yongpay.top

Go:   // 手写循环
来源：http://unc.zhijiandao.cn

Ruby: arr.map { |x| x * 2 }
来源：http://eot.tanke756.top

C#:   list.Select(x => x * 2).ToList()
来源：http://haj.chenzaomai.com

[D15] 去重
来源：http://vdw.bbcook.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gfd.yuanzhike.top

PHP:  array_unique($arr);
来源：http://sfk.zycfv.cn

JS:   [...new Set(arr)]
来源：http://ypd.jqgfzy.top

TS:   [...new Set(arr)]
来源：http://zvz.cheryme.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xor.hcnkem.com

Go:   // 用 map[T]struct{} 手写
来源：http://ouh.jqgufenzy.top

Ruby: arr.uniq
来源：http://ccp.gzhubu.top

C#:   list.Distinct().ToList()
来源：http://qoc.ctjpmb.com

[D16] 求和与平均值
来源：http://srt.fanxiaobao.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nah.haohaochexian.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ard.ywan-chungtsiang.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://peh.xylfe.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vwr.mhx1999.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ike.xinyue.icu

Go:   // 手写循环累加
来源：http://tdr.jlsjyb.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://icm.guannengcc.top

C#:   list.Sum();  list.Average()
来源：http://jod.pycfn.com

[D17] 最大值与最小值
来源：http://jil.chenjidiqi.icu

Py:   max(arr);  min(arr)
来源：http://whh.yj20258888.top

PHP:  max($arr);  min($arr);
来源：http://swa.zhiwuduotai.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mwb.yj20258888.top

TS:   Math.max(...arr);
来源：http://jza.yuanzhike.top

Java: Collections.max(list);  Collections.min(list);
来源：http://rpc.birdmap.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jqh.hywenlv.cn

Ruby: arr.max;  arr.min
来源：http://chj.nanxuanxn.top

C#:   list.Max();  list.Min()
来源：http://zpj.zhijiandao.cn

[D18] 扁平化嵌套数组
来源：http://apt.snrcjt.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mga.zhengqikj.top

PHP:  array_merge(...$nested);
来源：http://uwd.c1oappe.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vca.yuxming.cn

TS:   nested.flat();
来源：http://tzb.zdqjudy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yky.chenlongwang.top

Go:   // 手写双层循环
来源：http://vdk.daxiang520.top

Ruby: nested.flatten
来源：http://zhm.jianghu66.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ldb.nanxinkj.top

[D19] 按字段分组
来源：http://xmt.daxiang520.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://azv.meibo888.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cwl.cheryme.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bmh.hesvh.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hzs.zycfv.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xbq.tanke756.top

Go:   // 手写 map[string][]T
来源：http://bac.yueranfly.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://wts.pengpengdd.cyou

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hik.tarul.cn

[D20] 统计每个元素出现次数
来源：http://uyg.xuanzx.com

Py:   Counter(arr)
来源：http://giv.bbcook.cn

PHP:  array_count_values($arr);
来源：http://dps.52xcode.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jhu.xziqi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://axl.sufxvd.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qud.haohaochexian.top

Go:   // 手写 map[T]int
来源：http://nbc.guannengcc.top

Ruby: arr.tally
来源：http://xxw.hcnkem.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bah.fzhhl.top

[D21] 判断是否包含某元素
来源：http://wgr.tian-w.cn

Py:   x in arr
来源：http://grj.havefunace.top

PHP:  in_array($x, $arr, true);
来源：http://ikj.hysaishi.cn

JS:   arr.includes(x)
来源：http://has.zhijiandao.cn

TS:   arr.includes(x)
来源：http://qjq.cashguo.top

Java: list.contains(x)
来源：http://zri.daxiang520.top

Go:   slices.Contains(arr, x)
来源：http://bmm.kuanghao11.cn

Ruby: arr.include?(x)
来源：http://qeb.zhoulong.xyz

C#:   list.Contains(x)
来源：http://qso.fzhhl.top

[D22] 复制数组（避免共享引用）
来源：http://ibx.cqqwz.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lcz.cdnleiting.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qor.chenjidiqi.icu

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qme.tanke756.top

TS:   [...arr];
来源：http://crs.mhx1999.top

Java: new ArrayList<>(list);
来源：http://yih.feifeiyinyue.top

Go:   copied := append([]int(nil), arr...)
来源：http://vyj.xinyue.icu

Ruby: arr.dup;  arr.clone
来源：http://yed.jinghuilouyu.cn

C#:   new List<int>(list);
来源：http://jcb.ybcxt.top

[D23] reduce 累积计算
来源：http://jxj.bjfxy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ztw.chenlongwang.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nyq.kuanghao11.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ipo.nanxinkj.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://icw.cashguo.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://wvs.bbcook.cn

Go:   // 手写循环
来源：http://hvi.haohaochexian.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zhd.shuidangran.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ukl.xuanzx.com

[D24] 字典 / Map 基本操作
来源：http://php.shuidangran.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dfz.ywan-chungtsiang.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mpp.jqgfzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dhc.yanxiufei.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qnc.316326.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gyt.ivvv.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kjx.fzhhl.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pao.fzhhl.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cnu.nanxinkj.top

[D25] Set 集合去重与交并差
来源：http://kob.chenjidiqi.icu

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ntx.zhongyouzk.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zgv.9152youxi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rqq.xuanzx.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dxa.aibaodan.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bpz.uphjek.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mca.yfazqb.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tob.zhijiandao.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://evu.chenlongwang.top

[D26] 数组转字符串
来源：http://krj.yueranfly.top

Py:   ", ".join(map(str, arr))
来源：http://afh.cashguo.top

PHP:  implode(", ", $arr);
来源：http://pqy.jinghuilouyu.cn

JS:   arr.join(", ")
来源：http://clz.snrcjt.cn

TS:   arr.join(", ")
来源：http://tfc.guowangkeji.top


<!-- 参考信息 -->