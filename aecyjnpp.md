代发 wailian999

[C06] 匿名函数 / lambda
来源：http://kmh.epnwcf.com

Py:   square = lambda x: x * x
来源：http://pwm.birdmap.top

PHP:  $square = fn($x) => $x * $x;
来源：http://tne.aibaodan.cn

JS:   const square = x => x * x;
来源：http://uec.dashuyun.cn

TS:   const square = (x: number): number => x * x;
来源：http://jkn.hongshengwenyu.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://czj.guannengcc.top

Go:   sq := func(x int) int { return x * x }
来源：http://hdr.0kj1m.cn

Ruby: square = ->(x) { x * x }
来源：http://hcx.gogol.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cbq.iojbl.cn

[C07] 把函数作为参数传入
来源：http://fgy.meibo888.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://anm.chenjidiqi.icu

PHP:  array_map("strtoupper", $arr);
来源：http://rzq.havefunace.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nct.yj20258.top

TS:   arr.map(String)
来源：http://kcy.cheryme.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uoy.hywenlv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pav.yanxiufei.cn

Ruby: arr.map(&:upcase)
来源：http://lfo.nanxinkj.top

C#:   arr.Select(s => s.ToUpper())
来源：http://cbw.hesvh.cn

[C08] 闭包
来源：http://pwf.vehdjk.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wqk.jqgfzy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ddg.zhoulong.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tgw.pycfn.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rgd.guannengcc.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://joz.meibo888.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xuv.tianlin.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://die.jlsjyb.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zzc.zycfv.cn

[C09] 递归
来源：http://wwi.yvedp.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ygb.xylfe.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mrg.ydzc1.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lce.feifeiyinyue.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dcx.chenlongwang.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://knk.zdbjq.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ayl.jinqigfzy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uki.uphjek.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://taf.jlsjyb.cn

[C10] 变量作用域
来源：http://nvn.hnxiangtu.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vho.nwbrower.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://eii.smart0.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lug.xylfe.cn

TS:   同 JS
来源：http://wex.sweek.top

Java: 方法内为块级作用域
来源：http://ycg.bjfxy.top

Go:   花括号块级作用域
来源：http://cag.guannengcc.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qep.yfazqb.com

C#:   块级作用域
来源：http://gzo.redwolf501.top

[C11] 模块导入与导出
来源：http://awo.tian-w.cn

Py:   from module import func
来源：http://gyc.nanxinkj.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ypm.bjfxy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://svn.hfpthk.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xwi.smart0.xyz

Java: import java.util.List;
来源：http://ttg.meibo888.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://duo.fktsv.cn

Ruby: require "json"; require_relative "./util"
来源：http://mfr.yvedp.cn

C#:   using System.Text;
来源：http://kms.sufxvd.cn

[C12] 立即执行函数 IIFE
来源：http://nan.bjfxy.top

Py:   (lambda: print("run"))()
来源：http://zko.yfazqb.com

PHP:  (function () { echo "run"; })();
来源：http://wrl.dianchejie.cn

JS:   (() => { console.log("run"); })();
来源：http://jqc.birdmap.top

TS:   (() => { console.log("run"); })();
来源：http://dge.redwolf501.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wbs.vqdsnc.cn

Go:   func() { fmt.Println("run") }()
来源：http://mhu.ybcxt.top

Ruby: -> { puts "run" }.call
来源：http://epg.vehdjk.com

C#:   // 无 IIFE：用静态构造函数
来源：http://vnr.shanyushiyangtech.top

[C13] 类型声明 / 类型注解
来源：http://amy.yj20258888.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mer.ctjpmb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://akr.hongshengwenyu.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ohp.fzhhl.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bhy.xuanzx.com

Java: int add(int a, int b) { return a + b; }
来源：http://dma.redwolf501.top

Go:   func add(a, b int) int
来源：http://fvw.gogol.net.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ggv.meibo888.top

C#:   int Add(int a, int b) => a + b;
来源：http://keb.tanke756.top

[C14] 泛型函数
来源：http://jzi.iojbl.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bxl.hywenlv.cn

PHP:  // 无泛型
来源：http://gnz.zycfv.cn

JS:   // 无泛型
来源：http://uay.yvedp.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gwz.cucudq.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wvm.dashuyun.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yji.ydjk.org.cn

Ruby: # 无泛型
来源：http://qnv.yuxming.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gmg.yj20258.top

[C15] 解构 / 展开参数
来源：http://jks.guannengcc.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bra.aibaodan.cn

PHP:  [$a, $b] = $pair;
来源：http://xzz.pengpengdd.cyou

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nzc.shanyushiyangtech.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lfu.aizwys.cn

Java: // 无解构
来源：http://iez.fanxiaobao.xyz

Go:   // 无解构
来源：http://hvc.jqgfzy.top

Ruby: a, b = pair
来源：http://qon.9152youxi.cn

C#:   var (a, b) = pair;
来源：http://tvq.uphjek.com

[C16] 函数 / 方法重载
来源：http://moj.yanxiufei.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jwl.haohaochexian.top

PHP:  // 无重载
来源：http://iuh.xuanzx.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://vyq.bbcook.cn

TS:   // 用联合类型或重载签名声明
来源：http://loq.cashguo.top

Java: void f(int a) {}  void f(String a) {}
来源：http://kfb.sjlbkw.cn

Go:   // 无重载：用不同函数名
来源：http://nlp.quarkkingdee.top

Ruby: # 无重载：靠动态参数
来源：http://ang.yueranfly.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://qny.svipenyu.cn

================================================================================
来源：http://nit.jqgfzy.top

D. 数组 / 列表 / 集合
来源：http://nih.zhaomingkeji.xyz

================================================================================
来源：http://zyj.zhengqikj.top

[D01] 创建数组 / 列表
来源：http://jrj.yj202588.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://xzl.aibaodan.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kyl.yueranfly.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ozx.kuanghao11.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xhd.c1oappe.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uee.jqgfzy.top

Go:   arr := []int{1, 2, 3}
来源：http://olf.ppjwa.cn

Ruby: arr = [1, 2, 3]
来源：http://tgx.pengpengdd.cyou

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kpi.jyoumei.cn

[D02] 追加元素到末尾
来源：http://sxk.ydzc1.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cro.tianlin.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lzk.zhongyouzk.top

JS:   arr.push(4);
来源：http://uxk.zhongyouzk.top

TS:   arr.push(4);
来源：http://wsn.vehdjk.com

Java: list.add(4);
来源：http://xpm.dashuyun.cn

Go:   arr = append(arr, 4)
来源：http://qqg.quarkkingdee.top

Ruby: arr << 4; arr.push(5)
来源：http://nzo.ehwqpu.com

C#:   list.Add(4);
来源：http://dws.yvedp.cn

[D03] 在指定位置插入元素
来源：http://gdp.fanxiaobao.xyz

Py:   arr.insert(0, 0)
来源：http://gdi.jinqigufen.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://afh.zdbjq.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lbx.fzhhl.top

TS:   arr.splice(0, 0, 0);
来源：http://tro.xingfuxueyuan.xyz

Java: list.add(0, 0);
来源：http://yjy.hnqzz.top

Go:   arr = append([]int{0}, arr...)
来源：http://koh.sysykeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ntw.uphjek.com

C#:   list.Insert(0, 0);
来源：http://vpi.tarul.cn

[D04] 删除元素
来源：http://rmn.jiagoushi.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rgg.ehwqpu.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uzi.bjfxy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xug.yj20258.top

TS:   arr.splice(0, 1);
来源：http://xmh.9152youxi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tha.zdqjudy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cja.zhongyouzk.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://elw.yj202588.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hld.fengsongda.top

[D05] 访问与修改元素
来源：http://vyq.zhoulong.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gen.ehwqpu.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://act.nanxuanxn.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ymj.quarkkingdee.top

TS:   arr[0]; arr.at(-1);
来源：http://cou.pycfn.com

Java: list.get(0); list.set(0, 9);
来源：http://trf.jiagoushi.top

Go:   arr[0]; arr[0] = 9
来源：http://xjj.316326.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nvz.aizwys.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mxr.cdnleiting.top

[D06] 数组长度
来源：http://xad.ppjwa.cn

Py:   len(arr)
来源：http://arh.xinyue.icu

PHP:  count($arr);
来源：http://tse.gzhubu.top

JS:   arr.length
来源：http://fmh.quarkkingdee.top

TS:   arr.length
来源：http://avn.pengpengdd.cyou

Java: list.size();
来源：http://onq.ehwqpu.com

Go:   len(arr)
来源：http://jnz.quarkkingdee.top

Ruby: arr.length; arr.size
来源：http://akg.ydjk.org.cn

C#:   list.Count;
来源：http://qrf.zhijiandao.cn

[D07] 切片 / 取子数组
来源：http://tig.cucudq.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ymf.mhx1999.top

PHP:  array_slice($arr, 1, 3);
来源：http://oyk.fengsongda.top

JS:   arr.slice(1, 4);
来源：http://vpr.yj20258.top

TS:   arr.slice(1, 4);
来源：http://ezd.vehdjk.com

Java: list.subList(1, 4);
来源：http://beb.dashuyun.cn

Go:   arr[1:4]
来源：http://rka.kuanghao11.cn

Ruby: arr[1, 3]
来源：http://pft.fehbvm.com

C#:   list.GetRange(1, 3);
来源：http://iyt.hfpthk.cn

[D08] 合并两个数组
来源：http://ydc.daxiang520.top

Py:   a + b;  a.extend(b)
来源：http://bta.dashuyun.cn

PHP:  array_merge($a, $b);
来源：http://dya.sjlbkw.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://drf.yangfankeji.com

TS:   [...a, ...b];
来源：http://ylv.zhiwuduotai.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nlg.mhx1999.top

Go:   append(a, b...)
来源：http://lvh.guowangkeji.top

Ruby: a + b;  a.concat(b)
来源：http://xjb.smart0.xyz

C#:   a.Concat(b).ToList()
来源：http://zrz.yueranfly.top

[D09] 排序（升序）
来源：http://lee.yuanzhike.top

Py:   sorted(arr);  arr.sort()
来源：http://qhg.yfazqb.com

PHP:  sort($arr);
来源：http://hno.fktsv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://asq.jinqigfzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://qsk.shangyingyoupin.top

Java: Collections.sort(list);  list.sort(null);
来源：http://hia.cucudq.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ibx.chenzaomai.com

Ruby: arr.sort
来源：http://nqs.jinqigfzy.top

C#:   list.Sort();
来源：http://zwa.kuanghao11.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://nld.jqgfzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mlk.hcnkem.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hmo.zhaomingkeji.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rev.shanyushiyangtech.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://iga.ppjwa.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cpw.birdmap.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://aow.shangyingyoupin.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nmi.haohaochexian.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nsl.shanyushiyangtech.top

[D11] 反转数组
来源：http://quo.iojbl.cn

Py:   arr[::-1];  arr.reverse()
来源：http://yuy.yj202588.top

PHP:  array_reverse($arr);
来源：http://joe.ydzc1.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fsm.zhixingplan.top

TS:   [...arr].reverse();
来源：http://xgc.zhaomingkeji.xyz

Java: Collections.reverse(list);
来源：http://gol.cqqwz.cn

Go:   slices.Reverse(arr)
来源：http://ykn.chenjidiqi.icu

Ruby: arr.reverse
来源：http://oyh.ywan-chungtsiang.top

C#:   list.Reverse();
来源：http://ati.yj20258888.top

[D12] 查找元素下标
来源：http://lys.hnqzz.top

Py:   arr.index(x);  x in arr
来源：http://fsj.fanxiaobao.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dfh.shzxlz.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iez.feifeiyinyue.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qmp.yueranfly.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mjy.jinqigfzy.top

Go:   slices.Index(arr, x)
来源：http://pla.c1oappe.top

Ruby: arr.index(x)
来源：http://wwd.dashuyun.cn

C#:   list.IndexOf(x);
来源：http://czw.bbcook.cn

[D13] 过滤（保留满足条件的）
来源：http://jki.yonumen.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gml.kuanghao11.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gic.yj20258888.top

JS:   arr.filter(x => x > 3)
来源：http://sbx.zdqjudy.top

TS:   arr.filter(x => x > 3)
来源：http://pur.zhixingplan.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://aez.sysykeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://izn.shanyushiyangtech.top

Ruby: arr.select { |x| x > 3 }
来源：http://vsd.fktsv.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://and.yj202588.top

[D14] 映射转换（每个元素变形）
来源：http://kqt.xuetiantiany.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://obp.guannengcc.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://afs.dianchejie.cn

JS:   arr.map(x => x * 2)
来源：http://quq.jyoumei.cn

TS:   arr.map(x => x * 2)
来源：http://pjn.fzhhl.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://cqs.zdbjq.cn

Go:   // 手写循环
来源：http://gfp.haohaochexian.top

Ruby: arr.map { |x| x * 2 }
来源：http://cvd.zhongyouzk.top

C#:   list.Select(x => x * 2).ToList()
来源：http://mdb.yueranfly.top

[D15] 去重
来源：http://atp.meibo888.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zeq.hfpthk.cn

PHP:  array_unique($arr);
来源：http://huk.hysaishi.cn

JS:   [...new Set(arr)]
来源：http://xhh.dianchejie.cn

TS:   [...new Set(arr)]
来源：http://omg.zdqjudy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bxa.zdbjq.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lpc.c1oappe.top

Ruby: arr.uniq
来源：http://byp.snrcjt.cn

C#:   list.Distinct().ToList()
来源：http://pgy.yanxiufei.cn

[D16] 求和与平均值
来源：http://tvz.ivvv.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mtl.cashguo.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bic.uphjek.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://omx.316326.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bks.hnqzz.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nwv.gaohongyu789.top

Go:   // 手写循环累加
来源：http://klt.shzxlz.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fjk.tarul.cn

C#:   list.Sum();  list.Average()
来源：http://met.uphjek.com

[D17] 最大值与最小值
来源：http://cag.xingfuxueyuan.xyz

Py:   max(arr);  min(arr)
来源：http://ujk.fzhhl.top

PHP:  max($arr);  min($arr);
来源：http://hae.hongshengwenyu.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://okn.zhijiandao.cn

TS:   Math.max(...arr);
来源：http://nmo.hysaishi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bpd.cqqwz.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hhy.c1oappe.top

Ruby: arr.max;  arr.min
来源：http://qsc.nanxinkj.top

C#:   list.Max();  list.Min()
来源：http://zul.aizwys.cn

[D18] 扁平化嵌套数组
来源：http://dkw.cdnleiting.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qne.havefunace.top

PHP:  array_merge(...$nested);
来源：http://cmz.aizwys.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ncq.chenlongwang.top

TS:   nested.flat();
来源：http://sbi.jiagoushi.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dvh.shuidangran.top

Go:   // 手写双层循环
来源：http://erf.yongpay.top

Ruby: nested.flatten
来源：http://kni.9152youxi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xxn.aizwys.cn

[D19] 按字段分组
来源：http://rsy.ywan-chungtsiang.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://oyi.shuidangran.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zzr.feifeiyinyue.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://teg.cdnleiting.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://wwk.andypj.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mql.ehwqpu.com

Go:   // 手写 map[string][]T
来源：http://jkh.tanke756.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://hcs.shuidangran.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wat.0kj1m.cn

[D20] 统计每个元素出现次数
来源：http://nhc.bjfxy.top

Py:   Counter(arr)
来源：http://fcx.iojbl.cn

PHP:  array_count_values($arr);
来源：http://crz.jyoumei.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kgp.kuanghao11.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://svw.cucudq.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yze.gogol.net.cn

Go:   // 手写 map[T]int
来源：http://tsl.sweek.top

Ruby: arr.tally
来源：http://vny.andypj.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dpm.sjlbkw.cn

[D21] 判断是否包含某元素
来源：http://sfw.xingfuxueyuan.xyz

Py:   x in arr
来源：http://tok.tianlin.xyz

PHP:  in_array($x, $arr, true);
来源：http://bst.yfazqb.com

JS:   arr.includes(x)
来源：http://jze.fktsv.cn

TS:   arr.includes(x)
来源：http://pyi.hesvh.cn

Java: list.contains(x)
来源：http://jyh.dianchejie.cn

Go:   slices.Contains(arr, x)
来源：http://xpj.smart0.xyz

Ruby: arr.include?(x)
来源：http://soy.hcnkem.com

C#:   list.Contains(x)
来源：http://ntx.hnxiangtu.top

[D22] 复制数组（避免共享引用）
来源：http://kdq.hcnkem.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bgb.daria6918.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wvi.guannengcc.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bhi.ppjwa.cn

TS:   [...arr];
来源：http://wng.jqgufenzy.top

Java: new ArrayList<>(list);
来源：http://eph.tanke756.top

Go:   copied := append([]int(nil), arr...)
来源：http://svc.wangshuangyany.cn

Ruby: arr.dup;  arr.clone
来源：http://mzh.epnwcf.com

C#:   new List<int>(list);
来源：http://kyz.jiagoushi.top


<!-- 参考信息 -->