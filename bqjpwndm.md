代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ukt.pengpengdd.cyou

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ooi.jinqigufen.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sdc.tian-w.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://phr.yuxming.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pxy.sweek.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hud.zhongyouzk.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://asp.c1oappe.top

[C09] 递归
来源：http://srw.uphjek.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://eny.cqqwz.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pjm.yuxming.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sgd.tarul.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yvp.hnxiangtu.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cpj.sweek.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tmb.haohaochexian.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xbe.havefunace.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bmi.52xcode.cn

[C10] 变量作用域
来源：http://qpt.zhoulong.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gfz.nwbrower.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nka.yvedp.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yxz.nwbrower.top

TS:   同 JS
来源：http://fgz.ywan-chungtsiang.top

Java: 方法内为块级作用域
来源：http://xno.nanxuanxn.top

Go:   花括号块级作用域
来源：http://sga.fengsongda.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uvf.xingfuxueyuan.xyz

C#:   块级作用域
来源：http://spv.cdnleiting.top

[C11] 模块导入与导出
来源：http://yvw.sweek.top

Py:   from module import func
来源：http://cxw.sysykeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://qic.ywan-chungtsiang.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://voh.zhixingplan.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zto.bjfxy.top

Java: import java.util.List;
来源：http://pyy.fzhhl.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uaq.dianchejie.cn

Ruby: require "json"; require_relative "./util"
来源：http://ubz.svipenyu.cn

C#:   using System.Text;
来源：http://yhf.ivvv.top

[C12] 立即执行函数 IIFE
来源：http://dtm.redwolf501.top

Py:   (lambda: print("run"))()
来源：http://haj.gaohongyu789.top

PHP:  (function () { echo "run"; })();
来源：http://ora.sysykeji.top

JS:   (() => { console.log("run"); })();
来源：http://pln.wangdashe.top

TS:   (() => { console.log("run"); })();
来源：http://jjo.yuxming.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jam.zhengqikj.top

Go:   func() { fmt.Println("run") }()
来源：http://ufs.c1oappe.top

Ruby: -> { puts "run" }.call
来源：http://ujw.vehdjk.com

C#:   // 无 IIFE：用静态构造函数
来源：http://imu.snrcjt.cn

[C13] 类型声明 / 类型注解
来源：http://adj.yongpay.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qja.gzhubu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ejn.sysykeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://chl.daxiang520.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kxe.ppjwa.cn

Java: int add(int a, int b) { return a + b; }
来源：http://gps.yueranfly.top

Go:   func add(a, b int) int
来源：http://rgj.shanyushiyangkeji.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lpi.zdqjudy.top

C#:   int Add(int a, int b) => a + b;
来源：http://krs.daria6918.cn

[C14] 泛型函数
来源：http://ubo.nwbrower.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://veh.guowangkeji.top

PHP:  // 无泛型
来源：http://wox.daria6918.cn

JS:   // 无泛型
来源：http://fnh.gzhubu.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nte.jqgufenzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hwg.aibaodan.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://iie.ctjpmb.com

Ruby: # 无泛型
来源：http://lir.dashuyun.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jmp.guowangkeji.top

[C15] 解构 / 展开参数
来源：http://bhe.fehbvm.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xas.havefunace.top

PHP:  [$a, $b] = $pair;
来源：http://vnr.wangshuangyany.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sxw.zhongyouzk.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vyz.xingfuxueyuan.xyz

Java: // 无解构
来源：http://sbs.ywan-chungtsiang.top

Go:   // 无解构
来源：http://bvu.ctjpmb.com

Ruby: a, b = pair
来源：http://nax.vqdsnc.cn

C#:   var (a, b) = pair;
来源：http://ljh.bjfxy.top

[C16] 函数 / 方法重载
来源：http://jpz.havefunace.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://drs.jyoumei.cn

PHP:  // 无重载
来源：http://gvm.ydzc1.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://dhz.gzhubu.top

TS:   // 用联合类型或重载签名声明
来源：http://ojh.meibo888.top

Java: void f(int a) {}  void f(String a) {}
来源：http://cze.ehwqpu.com

Go:   // 无重载：用不同函数名
来源：http://ehr.svipenyu.cn

Ruby: # 无重载：靠动态参数
来源：http://vpi.ctjpmb.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://vtg.gzhubu.top

================================================================================
来源：http://afl.fengsongda.top

D. 数组 / 列表 / 集合
来源：http://tes.jiagoushi.top

================================================================================
来源：http://icm.zhengqikj.top

[D01] 创建数组 / 列表
来源：http://hvi.birdmap.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://dzt.zhengqikj.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ayk.pengpengdd.cyou

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ill.zhaomingkeji.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://qpp.xuetiantiany.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hnx.cheryme.top

Go:   arr := []int{1, 2, 3}
来源：http://vep.zhengqikj.top

Ruby: arr = [1, 2, 3]
来源：http://xzo.ppjwa.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hia.nanxinkj.top

[D02] 追加元素到末尾
来源：http://uqy.yj20258888.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gxp.jqgfzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qmb.jinyuanbaomall.cn

JS:   arr.push(4);
来源：http://xjw.fzhhl.top

TS:   arr.push(4);
来源：http://qyz.pengpengdd.cyou

Java: list.add(4);
来源：http://ojc.fanxiaobao.xyz

Go:   arr = append(arr, 4)
来源：http://tox.zhixingplan.top

Ruby: arr << 4; arr.push(5)
来源：http://fef.ppjwa.cn

C#:   list.Add(4);
来源：http://uvn.yangfankeji.com

[D03] 在指定位置插入元素
来源：http://lrx.c1oappe.top

Py:   arr.insert(0, 0)
来源：http://sty.kuanghao11.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xny.ydzc1.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zde.zdqjudy.top

TS:   arr.splice(0, 0, 0);
来源：http://oib.ydjk.org.cn

Java: list.add(0, 0);
来源：http://qlw.shangyingyoupin.top

Go:   arr = append([]int{0}, arr...)
来源：http://fxa.bbcook.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jeh.hammf.cn

C#:   list.Insert(0, 0);
来源：http://xqr.zhongyouzk.top

[D04] 删除元素
来源：http://rmd.dashuyun.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://amn.quarkkingdee.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mja.aibaodan.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ntv.yangfankeji.com

TS:   arr.splice(0, 1);
来源：http://yls.fanxiaobao.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qit.snrcjt.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yxv.shanyushiyangkeji.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ivx.nwbrower.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dkx.jlsjyb.cn

[D05] 访问与修改元素
来源：http://pje.zhixingplan.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://afk.tian-w.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gwz.hnxiangtu.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://anr.ctjpmb.com

TS:   arr[0]; arr.at(-1);
来源：http://khg.vqdsnc.cn

Java: list.get(0); list.set(0, 9);
来源：http://fcs.jinqigfzy.top

Go:   arr[0]; arr[0] = 9
来源：http://jpo.dianchejie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ufb.chenjidiqi.icu

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dgw.jlsjyb.cn

[D06] 数组长度
来源：http://dsi.yonumen.top

Py:   len(arr)
来源：http://kwm.ppjwa.cn

PHP:  count($arr);
来源：http://xuq.52xcode.cn

JS:   arr.length
来源：http://hgw.shanyushiyangkeji.top

TS:   arr.length
来源：http://qkl.fktsv.cn

Java: list.size();
来源：http://oqs.shuidangran.top

Go:   len(arr)
来源：http://nhn.sufxvd.cn

Ruby: arr.length; arr.size
来源：http://akw.chenzaomai.com

C#:   list.Count;
来源：http://gmz.jiagoushi.top

[D07] 切片 / 取子数组
来源：http://zyg.wangdashe.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nrq.yangfankeji.com

PHP:  array_slice($arr, 1, 3);
来源：http://khl.daria6918.cn

JS:   arr.slice(1, 4);
来源：http://ytj.shangyingyoupin.top

TS:   arr.slice(1, 4);
来源：http://ucv.bbcook.cn

Java: list.subList(1, 4);
来源：http://lzq.zhiwuduotai.top

Go:   arr[1:4]
来源：http://ekl.jinqigfzy.top

Ruby: arr[1, 3]
来源：http://ywl.sufxvd.cn

C#:   list.GetRange(1, 3);
来源：http://uqc.hongshengwenyu.top

[D08] 合并两个数组
来源：http://cpv.yj202588.top

Py:   a + b;  a.extend(b)
来源：http://gqm.yuxming.cn

PHP:  array_merge($a, $b);
来源：http://keb.shzxlz.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xnx.jqgfzy.top

TS:   [...a, ...b];
来源：http://gyk.sjlbkw.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lrm.ydzc1.top

Go:   append(a, b...)
来源：http://ovx.gogol.net.cn

Ruby: a + b;  a.concat(b)
来源：http://uyd.havefunace.top

C#:   a.Concat(b).ToList()
来源：http://qfs.zycfv.cn

[D09] 排序（升序）
来源：http://toh.dashuyun.cn

Py:   sorted(arr);  arr.sort()
来源：http://agc.daxiang520.top

PHP:  sort($arr);
来源：http://tvk.guannengcc.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vvo.sjlbkw.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://our.hongshengwenyu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ezx.daxiang520.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hai.c1oappe.top

Ruby: arr.sort
来源：http://brr.jyoumei.cn

C#:   list.Sort();
来源：http://nin.yueranfly.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://eub.yonumen.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jmm.jinqigfzy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ney.yangfankeji.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kev.fengsongda.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://boe.ydzc1.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hwn.chenzaomai.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wvb.zycfv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xmi.sufxvd.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dwu.haohaochexian.top

[D11] 反转数组
来源：http://kkw.iojbl.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hhv.shangyingyoupin.top

PHP:  array_reverse($arr);
来源：http://uxq.quarkkingdee.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://odb.jinghuilouyu.cn

TS:   [...arr].reverse();
来源：http://qtm.dashuyun.cn

Java: Collections.reverse(list);
来源：http://qcf.birdmap.top

Go:   slices.Reverse(arr)
来源：http://uco.dashuyun.cn

Ruby: arr.reverse
来源：http://geo.ydzc1.top

C#:   list.Reverse();
来源：http://rls.hcnkem.com

[D12] 查找元素下标
来源：http://pdg.kuanghao11.cn

Py:   arr.index(x);  x in arr
来源：http://pwu.jqgfzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uuu.gzhubu.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yci.gogol.net.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pvv.quarkkingdee.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fmc.epnwcf.com

Go:   slices.Index(arr, x)
来源：http://ljr.sxryk.cn

Ruby: arr.index(x)
来源：http://kwo.nwbrower.top

C#:   list.IndexOf(x);
来源：http://psg.tian-w.cn

[D13] 过滤（保留满足条件的）
来源：http://wdl.ctjpmb.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://smf.shangyingyoupin.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://frx.shanyushiyangkeji.top

JS:   arr.filter(x => x > 3)
来源：http://cba.feifeiyinyue.top

TS:   arr.filter(x => x > 3)
来源：http://kko.yueranfly.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gpe.zhengqikj.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dlc.mhx1999.top

Ruby: arr.select { |x| x > 3 }
来源：http://twr.havefunace.top

C#:   list.Where(x => x > 3).ToList()
来源：http://lko.gotoacloud.top

[D14] 映射转换（每个元素变形）
来源：http://iby.fzhhl.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rla.zhijiandao.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nna.gogol.net.cn

JS:   arr.map(x => x * 2)
来源：http://gpy.xingfuxueyuan.xyz

TS:   arr.map(x => x * 2)
来源：http://bjw.cucudq.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://fil.jiagoushi.top

Go:   // 手写循环
来源：http://jxl.chenzaomai.com

Ruby: arr.map { |x| x * 2 }
来源：http://aba.9152youxi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jnk.xziqi.cn

[D15] 去重
来源：http://sdk.shzxlz.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tud.aizwys.cn

PHP:  array_unique($arr);
来源：http://xem.guowangkeji.top

JS:   [...new Set(arr)]
来源：http://qvk.fengsongda.top

TS:   [...new Set(arr)]
来源：http://ndg.redwolf501.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rje.quarkkingdee.top

Go:   // 用 map[T]struct{} 手写
来源：http://zrw.svipenyu.cn

Ruby: arr.uniq
来源：http://gdk.cashguo.top

C#:   list.Distinct().ToList()
来源：http://evv.daria6918.cn

[D16] 求和与平均值
来源：http://xxq.snrcjt.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kuk.yangfankeji.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vmi.chenzaomai.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qug.sysykeji.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rcw.jqgfzy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gbl.smart0.xyz

Go:   // 手写循环累加
来源：http://stm.yfazqb.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://won.hysaishi.cn

C#:   list.Sum();  list.Average()
来源：http://wtw.birdmap.top

[D17] 最大值与最小值
来源：http://avh.cashguo.top

Py:   max(arr);  min(arr)
来源：http://pqc.pycfn.com

PHP:  max($arr);  min($arr);
来源：http://qps.chenzaomai.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xuc.redwolf501.top

TS:   Math.max(...arr);
来源：http://gfx.316326.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://bjy.jinyuanbaomall.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hlb.smart0.xyz

Ruby: arr.max;  arr.min
来源：http://xma.zdqjudy.top

C#:   list.Max();  list.Min()
来源：http://nhu.gogol.net.cn

[D18] 扁平化嵌套数组
来源：http://jtp.xziqi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://iis.yonumen.top

PHP:  array_merge(...$nested);
来源：http://sud.jyoumei.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zdo.jlsjyb.cn

TS:   nested.flat();
来源：http://sty.zdbjq.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gtl.wangdashe.top

Go:   // 手写双层循环
来源：http://wfh.tanke756.top

Ruby: nested.flatten
来源：http://kmf.hywenlv.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://aua.cdnleiting.top

[D19] 按字段分组
来源：http://qew.zhengqikj.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lal.sufxvd.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://msl.dianchejie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sae.hywenlv.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://evn.shzxlz.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://roa.zdbjq.cn

Go:   // 手写 map[string][]T
来源：http://yvq.jinqigfzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ipc.daria6918.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://iud.daxiang520.top

[D20] 统计每个元素出现次数
来源：http://pyu.snrcjt.cn

Py:   Counter(arr)
来源：http://ojd.pengpengdd.cyou

PHP:  array_count_values($arr);
来源：http://xmn.daxiang520.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://alf.hysaishi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://osl.birdmap.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ecf.sjlbkw.cn

Go:   // 手写 map[T]int
来源：http://mml.9152youxi.cn

Ruby: arr.tally
来源：http://qoe.meibo888.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://djp.svipenyu.cn

[D21] 判断是否包含某元素
来源：http://cgv.jyoumei.cn

Py:   x in arr
来源：http://abr.sjlbkw.cn

PHP:  in_array($x, $arr, true);
来源：http://eyl.meibo888.top

JS:   arr.includes(x)
来源：http://xzz.guowangkeji.top

TS:   arr.includes(x)
来源：http://huv.jqgfzy.top

Java: list.contains(x)
来源：http://zho.smart0.xyz

Go:   slices.Contains(arr, x)
来源：http://ejr.shuidangran.top

Ruby: arr.include?(x)
来源：http://ymk.hongshengwenyu.top

C#:   list.Contains(x)
来源：http://pse.ehwqpu.com

[D22] 复制数组（避免共享引用）
来源：http://aex.bbcook.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qpj.tianlin.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pwi.zhijiandao.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cxm.daria6918.cn

TS:   [...arr];
来源：http://hvu.yueranfly.top

Java: new ArrayList<>(list);
来源：http://chs.tarul.cn

Go:   copied := append([]int(nil), arr...)
来源：http://tkt.shuidangran.top

Ruby: arr.dup;  arr.clone
来源：http://dpv.sweek.top

C#:   new List<int>(list);
来源：http://ujr.vqdsnc.cn

[D23] reduce 累积计算
来源：http://tmb.nanxinkj.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://uag.jinqigufen.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dwm.yuxming.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yoj.zdbjq.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xuy.shuidangran.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://lak.smart0.xyz

Go:   // 手写循环
来源：http://ktb.fktsv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dsl.aizwys.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zvx.zhijiandao.cn

[D24] 字典 / Map 基本操作
来源：http://kmk.dashuyun.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blh.ivvv.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://olh.ywan-chungtsiang.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zzo.sysykeji.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cbz.zdbjq.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://spm.hesvh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://aum.chenjidiqi.icu

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pgb.xuanzx.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oec.jyoumei.cn

[D25] Set 集合去重与交并差
来源：http://pmh.iojbl.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ekx.pengpengdd.cyou


<!-- 参考信息 -->