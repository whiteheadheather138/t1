代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://uwe.shzxlz.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lzo.zhongyouzk.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pct.shzxlz.cn

[C09] 递归
来源：http://ner.zhijiandao.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tzs.shuidangran.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ceq.c1oappe.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iop.zdbjq.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ttz.daria6918.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://oqf.jiagoushi.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://erz.jyoumei.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://edn.pengpengdd.cyou

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lpi.yvedp.cn

[C10] 变量作用域
来源：http://ntw.jqgufenzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fnl.svipenyu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xsm.cashguo.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tdf.aibaodan.cn

TS:   同 JS
来源：http://fbm.jinyuanbaomall.cn

Java: 方法内为块级作用域
来源：http://ppv.hnqzz.top

Go:   花括号块级作用域
来源：http://aln.snrcjt.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://apw.chenlongwang.top

C#:   块级作用域
来源：http://dyo.snrcjt.cn

[C11] 模块导入与导出
来源：http://qmc.pycfn.com

Py:   from module import func
来源：http://coh.yj20258.top

PHP:  require "file.php";  或 use App\Service;
来源：http://qsj.dianchejie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zzk.shanyushiyangkeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mqc.tian-w.cn

Java: import java.util.List;
来源：http://wdu.sufxvd.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qrm.shzxlz.cn

Ruby: require "json"; require_relative "./util"
来源：http://yte.yanxiufei.cn

C#:   using System.Text;
来源：http://ict.zdqjudy.top

[C12] 立即执行函数 IIFE
来源：http://puk.hywenlv.cn

Py:   (lambda: print("run"))()
来源：http://aet.jinqigfzy.top

PHP:  (function () { echo "run"; })();
来源：http://dnu.iojbl.cn

JS:   (() => { console.log("run"); })();
来源：http://cno.nanxuanxn.top

TS:   (() => { console.log("run"); })();
来源：http://vxg.yangfankeji.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mbw.redwolf501.top

Go:   func() { fmt.Println("run") }()
来源：http://nqe.vqdsnc.cn

Ruby: -> { puts "run" }.call
来源：http://nxs.cucudq.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://sbz.guowangkeji.top

[C13] 类型声明 / 类型注解
来源：http://irv.zhoulong.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://suk.xingfuxueyuan.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hjo.zhongyouzk.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yyo.epnwcf.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zpw.gaohongyu789.top

Java: int add(int a, int b) { return a + b; }
来源：http://gub.0kj1m.cn

Go:   func add(a, b int) int
来源：http://wnl.andypj.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://imd.xziqi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://lim.chenlongwang.top

[C14] 泛型函数
来源：http://mjt.yj20258888.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nny.hfpthk.cn

PHP:  // 无泛型
来源：http://nwe.tianlin.xyz

JS:   // 无泛型
来源：http://mjx.andypj.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ibr.epnwcf.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jhx.bjfxy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kbg.snrcjt.cn

Ruby: # 无泛型
来源：http://yrs.chenjidiqi.icu

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fjf.aizwys.cn

[C15] 解构 / 展开参数
来源：http://tgs.cdnleiting.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://muc.feifeiyinyue.top

PHP:  [$a, $b] = $pair;
来源：http://rta.hysaishi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jon.ivvv.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wbz.0kj1m.cn

Java: // 无解构
来源：http://cbd.tanke756.top

Go:   // 无解构
来源：http://yke.cqqwz.cn

Ruby: a, b = pair
来源：http://beu.hcnkem.com

C#:   var (a, b) = pair;
来源：http://nww.dianchejie.cn

[C16] 函数 / 方法重载
来源：http://nzy.epnwcf.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sdl.bbcook.cn

PHP:  // 无重载
来源：http://apy.tian-w.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://oru.jinqigufen.top

TS:   // 用联合类型或重载签名声明
来源：http://lpx.iojbl.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://lty.zhijiandao.cn

Go:   // 无重载：用不同函数名
来源：http://usm.fktsv.cn

Ruby: # 无重载：靠动态参数
来源：http://hli.gzhubu.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ofk.fehbvm.com

================================================================================
来源：http://der.hcnkem.com

D. 数组 / 列表 / 集合
来源：http://rgg.shuidangran.top

================================================================================
来源：http://mxk.hcnkem.com

[D01] 创建数组 / 列表
来源：http://twt.andypj.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://khq.xuetiantiany.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ybr.kuanghao11.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sgi.uphjek.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://kml.ydjk.org.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jyg.sufxvd.cn

Go:   arr := []int{1, 2, 3}
来源：http://uxj.sufxvd.cn

Ruby: arr = [1, 2, 3]
来源：http://gdp.jqgfzy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kla.jiagoushi.top

[D02] 追加元素到末尾
来源：http://vvu.fzhhl.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cdt.havefunace.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vkr.tanke756.top

JS:   arr.push(4);
来源：http://uhs.kuanghao11.cn

TS:   arr.push(4);
来源：http://caw.feifeiyinyue.top

Java: list.add(4);
来源：http://jgm.ydzc1.top

Go:   arr = append(arr, 4)
来源：http://tub.pycfn.com

Ruby: arr << 4; arr.push(5)
来源：http://tdx.hywenlv.cn

C#:   list.Add(4);
来源：http://wiu.shanyushiyangtech.top

[D03] 在指定位置插入元素
来源：http://hmw.52xcode.cn

Py:   arr.insert(0, 0)
来源：http://jao.nanxuanxn.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://meu.hongshengwenyu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nkn.wangdashe.top

TS:   arr.splice(0, 0, 0);
来源：http://pgw.bjfxy.top

Java: list.add(0, 0);
来源：http://fgd.yanxiufei.cn

Go:   arr = append([]int{0}, arr...)
来源：http://siw.0kj1m.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cnx.shanyushiyangtech.top

C#:   list.Insert(0, 0);
来源：http://jjq.sweek.top

[D04] 删除元素
来源：http://oat.zhongyouzk.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ccb.ctjpmb.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rhe.shuidangran.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bdg.cucudq.cn

TS:   arr.splice(0, 1);
来源：http://tub.fktsv.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zjr.chenlongwang.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jjb.yangfankeji.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://frj.zhijiandao.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cac.fanxiaobao.xyz

[D05] 访问与修改元素
来源：http://nna.yuxming.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qzc.nanxinkj.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://obd.bbcook.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mac.nwbrower.top

TS:   arr[0]; arr.at(-1);
来源：http://gsn.redwolf501.top

Java: list.get(0); list.set(0, 9);
来源：http://bsh.ywan-chungtsiang.top

Go:   arr[0]; arr[0] = 9
来源：http://lci.hnqzz.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://czh.zhiwuduotai.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xja.ehwqpu.com

[D06] 数组长度
来源：http://msb.fanxiaobao.xyz

Py:   len(arr)
来源：http://sxx.yongpay.top

PHP:  count($arr);
来源：http://lay.meibo888.top

JS:   arr.length
来源：http://nmw.zhiwuduotai.top

TS:   arr.length
来源：http://qkh.kuanghao11.cn

Java: list.size();
来源：http://awg.fengsongda.top

Go:   len(arr)
来源：http://qtx.hysaishi.cn

Ruby: arr.length; arr.size
来源：http://eah.zhiwuduotai.top

C#:   list.Count;
来源：http://bpy.epnwcf.com

[D07] 切片 / 取子数组
来源：http://ofg.ivvv.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tcz.cdnleiting.top

PHP:  array_slice($arr, 1, 3);
来源：http://ion.kuanghao11.cn

JS:   arr.slice(1, 4);
来源：http://non.xuetiantiany.cn

TS:   arr.slice(1, 4);
来源：http://vtc.shanyushiyangtech.top

Java: list.subList(1, 4);
来源：http://erd.havefunace.top

Go:   arr[1:4]
来源：http://brf.yangfankeji.com

Ruby: arr[1, 3]
来源：http://hmy.hysaishi.cn

C#:   list.GetRange(1, 3);
来源：http://rkp.quarkkingdee.top

[D08] 合并两个数组
来源：http://aix.ywan-chungtsiang.top

Py:   a + b;  a.extend(b)
来源：http://pfb.zhiwuduotai.top

PHP:  array_merge($a, $b);
来源：http://ybg.xziqi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://dfw.jqgfzy.top

TS:   [...a, ...b];
来源：http://xxt.yangfankeji.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://szy.dianchejie.cn

Go:   append(a, b...)
来源：http://mnl.nwbrower.top

Ruby: a + b;  a.concat(b)
来源：http://qta.hfpthk.cn

C#:   a.Concat(b).ToList()
来源：http://ryd.sysykeji.top

[D09] 排序（升序）
来源：http://tpp.xziqi.cn

Py:   sorted(arr);  arr.sort()
来源：http://pwl.xuanzx.com

PHP:  sort($arr);
来源：http://aso.dashuyun.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://njc.cucudq.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ixe.316326.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://xsg.svipenyu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://drq.cashguo.top

Ruby: arr.sort
来源：http://gjg.zdqjudy.top

C#:   list.Sort();
来源：http://gyw.kuanghao11.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rsi.gogol.net.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ajo.sjlbkw.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kac.dianchejie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kmc.yuxming.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wko.bjfxy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wkz.ctjpmb.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rxa.ppjwa.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xau.smart0.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rmg.zdqjudy.top

[D11] 反转数组
来源：http://zlt.zhiwuduotai.top

Py:   arr[::-1];  arr.reverse()
来源：http://qru.birdmap.top

PHP:  array_reverse($arr);
来源：http://dmi.hnxiangtu.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bng.chenjidiqi.icu

TS:   [...arr].reverse();
来源：http://alv.hfpthk.cn

Java: Collections.reverse(list);
来源：http://xvs.ydzc1.top

Go:   slices.Reverse(arr)
来源：http://jac.hysaishi.cn

Ruby: arr.reverse
来源：http://xmk.sweek.top

C#:   list.Reverse();
来源：http://lwl.yongpay.top

[D12] 查找元素下标
来源：http://xas.sysykeji.top

Py:   arr.index(x);  x in arr
来源：http://bbb.zhengqikj.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ouz.wangshuangyany.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fzu.jiagoushi.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://njh.sufxvd.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cbe.yuanzhike.top

Go:   slices.Index(arr, x)
来源：http://yxx.svipenyu.cn

Ruby: arr.index(x)
来源：http://ahp.chenjidiqi.icu

C#:   list.IndexOf(x);
来源：http://qne.fktsv.cn

[D13] 过滤（保留满足条件的）
来源：http://fvl.sxryk.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wyt.xuanzx.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mjb.feifeiyinyue.top

JS:   arr.filter(x => x > 3)
来源：http://ajs.haohaochexian.top

TS:   arr.filter(x => x > 3)
来源：http://dxb.yuxming.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://djm.zhaomingkeji.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vwp.hcnkem.com

Ruby: arr.select { |x| x > 3 }
来源：http://pmt.yj20258.top

C#:   list.Where(x => x > 3).ToList()
来源：http://bwp.yj20258888.top

[D14] 映射转换（每个元素变形）
来源：http://owt.birdmap.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://luj.birdmap.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sew.zycfv.cn

JS:   arr.map(x => x * 2)
来源：http://fco.xinyue.icu

TS:   arr.map(x => x * 2)
来源：http://roe.shanyushiyangtech.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://tqd.sjlbkw.cn

Go:   // 手写循环
来源：http://ijg.dianchejie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vho.316326.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://gjp.fehbvm.com

[D15] 去重
来源：http://mof.guannengcc.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cqi.xylfe.cn

PHP:  array_unique($arr);
来源：http://kjx.guowangkeji.top

JS:   [...new Set(arr)]
来源：http://oqd.sysykeji.top

TS:   [...new Set(arr)]
来源：http://gcq.guannengcc.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pgk.jyoumei.cn

Go:   // 用 map[T]struct{} 手写
来源：http://bvo.gotoacloud.top

Ruby: arr.uniq
来源：http://vdz.yueranfly.top

C#:   list.Distinct().ToList()
来源：http://wwf.hesvh.cn

[D16] 求和与平均值
来源：http://nlf.wangshuangyany.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://saj.chenzaomai.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://eaq.nanxinkj.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fed.iojbl.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ylv.shanyushiyangkeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vca.c1oappe.top

Go:   // 手写循环累加
来源：http://wgn.kuanghao11.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lxk.jqgufenzy.top

C#:   list.Sum();  list.Average()
来源：http://kfs.havefunace.top

[D17] 最大值与最小值
来源：http://xdt.tian-w.cn

Py:   max(arr);  min(arr)
来源：http://umc.tarul.cn

PHP:  max($arr);  min($arr);
来源：http://ifa.pengpengdd.cyou

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wkk.cdnleiting.top

TS:   Math.max(...arr);
来源：http://ijo.zhaomingkeji.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://xtk.shangyingyoupin.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vxf.haohaochexian.top

Ruby: arr.max;  arr.min
来源：http://tdz.yfazqb.com

C#:   list.Max();  list.Min()
来源：http://uai.zhixingplan.top

[D18] 扁平化嵌套数组
来源：http://bxb.xziqi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yin.sxryk.cn

PHP:  array_merge(...$nested);
来源：http://xbq.ehwqpu.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tut.ybcxt.top

TS:   nested.flat();
来源：http://bpw.cucudq.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jvg.hammf.cn

Go:   // 手写双层循环
来源：http://zig.iojbl.cn

Ruby: nested.flatten
来源：http://gbi.c1oappe.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ygx.jqgfzy.top

[D19] 按字段分组
来源：http://cnx.gzhubu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xdk.kuanghao11.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wtw.sufxvd.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://saz.gotoacloud.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://wuv.kuanghao11.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bug.havefunace.top

Go:   // 手写 map[string][]T
来源：http://atz.vqdsnc.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://nos.ywan-chungtsiang.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mhf.hongshengwenyu.top

[D20] 统计每个元素出现次数
来源：http://rmz.xuetiantiany.cn

Py:   Counter(arr)
来源：http://agl.shanyushiyangkeji.top

PHP:  array_count_values($arr);
来源：http://nqr.fengsongda.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://btm.wangdashe.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qik.birdmap.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lzv.cucudq.cn

Go:   // 手写 map[T]int
来源：http://gvs.chenlongwang.top

Ruby: arr.tally
来源：http://cec.havefunace.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ygc.jyoumei.cn

[D21] 判断是否包含某元素
来源：http://qgx.jinqigufen.top

Py:   x in arr
来源：http://frt.cdnleiting.top

PHP:  in_array($x, $arr, true);
来源：http://qcc.shanyushiyangkeji.top

JS:   arr.includes(x)
来源：http://jgz.tanke756.top

TS:   arr.includes(x)
来源：http://cga.xuanzx.com

Java: list.contains(x)
来源：http://whf.yj202588.top

Go:   slices.Contains(arr, x)
来源：http://jbq.yongpay.top

Ruby: arr.include?(x)
来源：http://kez.gaohongyu789.top

C#:   list.Contains(x)
来源：http://zol.ivvv.top

[D22] 复制数组（避免共享引用）
来源：http://icr.andypj.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rhg.zhixingplan.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nzu.jinqigufen.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kgi.tanke756.top

TS:   [...arr];
来源：http://qqi.guannengcc.top

Java: new ArrayList<>(list);
来源：http://vsn.ydjk.org.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bra.fengsongda.top

Ruby: arr.dup;  arr.clone
来源：http://kme.jlsjyb.cn

C#:   new List<int>(list);
来源：http://taj.haohaochexian.top

[D23] reduce 累积计算
来源：http://ptk.c1oappe.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mwb.gotoacloud.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kpq.sufxvd.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qvf.sufxvd.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fyb.zhijiandao.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gai.birdmap.top

Go:   // 手写循环
来源：http://agb.shangyingyoupin.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yph.jqgufenzy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jfk.jinqigufen.top

[D24] 字典 / Map 基本操作
来源：http://bwk.yuxming.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lzc.aibaodan.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mtf.jqgfzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ker.52xcode.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zis.kuanghao11.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qwn.quarkkingdee.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nik.fengsongda.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nhe.xziqi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dmo.zhixingplan.top

[D25] Set 集合去重与交并差
来源：http://kbt.dashuyun.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gce.yvedp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kpe.smart0.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pqj.316326.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zhg.epnwcf.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ccr.jlsjyb.cn


<!-- 参考信息 -->