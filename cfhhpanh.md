代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://drt.iojbl.cn

[C07] 把函数作为参数传入
来源：http://ypp.zdqjudy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gvl.nanxuanxn.top

PHP:  array_map("strtoupper", $arr);
来源：http://lgm.52xcode.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kbj.uphjek.com

TS:   arr.map(String)
来源：http://aha.cashguo.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://car.pycfn.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://orc.yj20258888.top

Ruby: arr.map(&:upcase)
来源：http://iav.epnwcf.com

C#:   arr.Select(s => s.ToUpper())
来源：http://xwv.zhengqikj.top

[C08] 闭包
来源：http://ufr.cqqwz.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vyn.nanxuanxn.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ktx.jlsjyb.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xli.chenzaomai.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sim.zhongyouzk.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xws.xuanzx.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cjp.jiagoushi.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://eep.pengpengdd.cyou

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cce.sweek.top

[C09] 递归
来源：http://oin.ydjk.org.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mra.pengpengdd.cyou

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bnr.yj202588.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ici.sysykeji.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hmh.uphjek.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ajo.nanxinkj.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jsd.yuxming.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ows.quarkkingdee.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://esa.ehwqpu.com

[C10] 变量作用域
来源：http://kke.shuidangran.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gsn.bbcook.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nai.chenlongwang.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vnx.xinyue.icu

TS:   同 JS
来源：http://apt.meibo888.top

Java: 方法内为块级作用域
来源：http://kxd.jinqigufen.top

Go:   花括号块级作用域
来源：http://jgq.jlsjyb.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xpy.tianlin.xyz

C#:   块级作用域
来源：http://zuz.bjfxy.top

[C11] 模块导入与导出
来源：http://clp.snrcjt.cn

Py:   from module import func
来源：http://sog.andypj.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://gzb.yonumen.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://xbj.yuanzhike.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wub.zhongyouzk.top

Java: import java.util.List;
来源：http://kni.cucudq.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ulk.yonumen.top

Ruby: require "json"; require_relative "./util"
来源：http://oia.zhongyouzk.top

C#:   using System.Text;
来源：http://bkr.yj20258888.top

[C12] 立即执行函数 IIFE
来源：http://rwq.shanyushiyangtech.top

Py:   (lambda: print("run"))()
来源：http://nbz.jlsjyb.cn

PHP:  (function () { echo "run"; })();
来源：http://klx.snrcjt.cn

JS:   (() => { console.log("run"); })();
来源：http://lca.ctjpmb.com

TS:   (() => { console.log("run"); })();
来源：http://nan.fengsongda.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ozs.yuanzhike.top

Go:   func() { fmt.Println("run") }()
来源：http://yvy.wangdashe.top

Ruby: -> { puts "run" }.call
来源：http://fbx.dashuyun.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xlw.cdnleiting.top

[C13] 类型声明 / 类型注解
来源：http://cfe.havefunace.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gso.quarkkingdee.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ejc.hammf.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tfo.c1oappe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rwf.feifeiyinyue.top

Java: int add(int a, int b) { return a + b; }
来源：http://mhj.gzhubu.top

Go:   func add(a, b int) int
来源：http://hgi.sxryk.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rpd.bbcook.cn

C#:   int Add(int a, int b) => a + b;
来源：http://sld.sysykeji.top

[C14] 泛型函数
来源：http://thc.zdbjq.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://azr.yongpay.top

PHP:  // 无泛型
来源：http://zzt.fengsongda.top

JS:   // 无泛型
来源：http://luf.haohaochexian.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://scq.shzxlz.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ape.tianlin.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jya.cashguo.top

Ruby: # 无泛型
来源：http://cau.wangshuangyany.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pxh.uphjek.com

[C15] 解构 / 展开参数
来源：http://sam.zhaomingkeji.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hub.pycfn.com

PHP:  [$a, $b] = $pair;
来源：http://nfb.guowangkeji.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hqi.bjfxy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vqu.hongshengwenyu.top

Java: // 无解构
来源：http://jis.zhengqikj.top

Go:   // 无解构
来源：http://gnd.pycfn.com

Ruby: a, b = pair
来源：http://vet.uphjek.com

C#:   var (a, b) = pair;
来源：http://iwd.zhongyouzk.top

[C16] 函数 / 方法重载
来源：http://uuq.ivvv.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://djr.mhx1999.top

PHP:  // 无重载
来源：http://vcv.0kj1m.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://uax.vehdjk.com

TS:   // 用联合类型或重载签名声明
来源：http://set.jyoumei.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qek.nwbrower.top

Go:   // 无重载：用不同函数名
来源：http://dhl.feifeiyinyue.top

Ruby: # 无重载：靠动态参数
来源：http://ilh.sweek.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://hxx.cdnleiting.top

================================================================================
来源：http://awl.yvedp.cn

D. 数组 / 列表 / 集合
来源：http://gra.xingfuxueyuan.xyz

================================================================================
来源：http://bjd.yueranfly.top

[D01] 创建数组 / 列表
来源：http://vun.0kj1m.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://vte.zycfv.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://oam.yanxiufei.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mac.jlsjyb.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vbm.316326.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://znc.sweek.top

Go:   arr := []int{1, 2, 3}
来源：http://sjt.meibo888.top

Ruby: arr = [1, 2, 3]
来源：http://vrn.chenlongwang.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://aga.jinqigufen.top

[D02] 追加元素到末尾
来源：http://cow.tarul.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vfm.yfazqb.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zuq.fengsongda.top

JS:   arr.push(4);
来源：http://fgy.sysykeji.top

TS:   arr.push(4);
来源：http://mjj.wangdashe.top

Java: list.add(4);
来源：http://ftt.sxryk.cn

Go:   arr = append(arr, 4)
来源：http://scz.nwbrower.top

Ruby: arr << 4; arr.push(5)
来源：http://dyz.tanke756.top

C#:   list.Add(4);
来源：http://azd.jinqigfzy.top

[D03] 在指定位置插入元素
来源：http://lmj.zhaomingkeji.xyz

Py:   arr.insert(0, 0)
来源：http://mqh.vqdsnc.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wul.quarkkingdee.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gfe.xuetiantiany.cn

TS:   arr.splice(0, 0, 0);
来源：http://kxg.hammf.cn

Java: list.add(0, 0);
来源：http://gki.uphjek.com

Go:   arr = append([]int{0}, arr...)
来源：http://hdu.aibaodan.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://omf.zdqjudy.top

C#:   list.Insert(0, 0);
来源：http://xqs.gogol.net.cn

[D04] 删除元素
来源：http://koe.snrcjt.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://grx.shuidangran.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uzb.jqgfzy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://etd.sjlbkw.cn

TS:   arr.splice(0, 1);
来源：http://whc.pengpengdd.cyou

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jkv.xingfuxueyuan.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hku.hnqzz.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ajs.52xcode.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cys.nanxuanxn.top

[D05] 访问与修改元素
来源：http://ajf.jqgufenzy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mpg.fanxiaobao.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sxm.wangdashe.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hek.dianchejie.cn

TS:   arr[0]; arr.at(-1);
来源：http://stx.tian-w.cn

Java: list.get(0); list.set(0, 9);
来源：http://sea.jlsjyb.cn

Go:   arr[0]; arr[0] = 9
来源：http://xqt.nanxinkj.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sxh.cashguo.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uwx.xinyue.icu

[D06] 数组长度
来源：http://tqi.tianlin.xyz

Py:   len(arr)
来源：http://hva.fzhhl.top

PHP:  count($arr);
来源：http://pdf.fehbvm.com

JS:   arr.length
来源：http://bjo.fengsongda.top

TS:   arr.length
来源：http://afk.xuanzx.com

Java: list.size();
来源：http://krg.aizwys.cn

Go:   len(arr)
来源：http://oue.9152youxi.cn

Ruby: arr.length; arr.size
来源：http://vaw.tian-w.cn

C#:   list.Count;
来源：http://cwl.birdmap.top

[D07] 切片 / 取子数组
来源：http://jai.dashuyun.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gfv.zhongyouzk.top

PHP:  array_slice($arr, 1, 3);
来源：http://oah.haohaochexian.top

JS:   arr.slice(1, 4);
来源：http://iwi.hcnkem.com

TS:   arr.slice(1, 4);
来源：http://zju.hnqzz.top

Java: list.subList(1, 4);
来源：http://olh.fzhhl.top

Go:   arr[1:4]
来源：http://qeg.cheryme.top

Ruby: arr[1, 3]
来源：http://ykh.yvedp.cn

C#:   list.GetRange(1, 3);
来源：http://snv.wangshuangyany.cn

[D08] 合并两个数组
来源：http://tbf.hcnkem.com

Py:   a + b;  a.extend(b)
来源：http://ekk.hysaishi.cn

PHP:  array_merge($a, $b);
来源：http://ued.chenlongwang.top

JS:   [...a, ...b];  a.concat(b);
来源：http://oqq.jianghu66.top

TS:   [...a, ...b];
来源：http://sji.xingfuxueyuan.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pbm.uphjek.com

Go:   append(a, b...)
来源：http://xie.jinyuanbaomall.cn

Ruby: a + b;  a.concat(b)
来源：http://var.guannengcc.top

C#:   a.Concat(b).ToList()
来源：http://oli.nanxuanxn.top

[D09] 排序（升序）
来源：http://dgr.epnwcf.com

Py:   sorted(arr);  arr.sort()
来源：http://hxu.ybcxt.top

PHP:  sort($arr);
来源：http://vtd.fehbvm.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gqr.tian-w.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://eld.pycfn.com

Java: Collections.sort(list);  list.sort(null);
来源：http://wkk.xingfuxueyuan.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xge.zhixingplan.top

Ruby: arr.sort
来源：http://giy.epnwcf.com

C#:   list.Sort();
来源：http://nci.hnqzz.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://pxp.yueranfly.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fvd.chenjidiqi.icu

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nmr.hysaishi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tyy.xylfe.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vuz.zdqjudy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://uga.havefunace.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bgw.yvedp.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://iem.0kj1m.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qkv.haohaochexian.top

[D11] 反转数组
来源：http://sol.xylfe.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wsd.jlsjyb.cn

PHP:  array_reverse($arr);
来源：http://vpk.sysykeji.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://eqh.vehdjk.com

TS:   [...arr].reverse();
来源：http://mzk.316326.xyz

Java: Collections.reverse(list);
来源：http://vfd.sxryk.cn

Go:   slices.Reverse(arr)
来源：http://iso.yj20258.top

Ruby: arr.reverse
来源：http://qko.yangfankeji.com

C#:   list.Reverse();
来源：http://iap.hysaishi.cn

[D12] 查找元素下标
来源：http://lpv.hnqzz.top

Py:   arr.index(x);  x in arr
来源：http://adh.sweek.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jme.uphjek.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wsa.andypj.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hyt.gaohongyu789.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rdn.shanyushiyangkeji.top

Go:   slices.Index(arr, x)
来源：http://iwd.epnwcf.com

Ruby: arr.index(x)
来源：http://apv.redwolf501.top

C#:   list.IndexOf(x);
来源：http://kkd.jqgufenzy.top

[D13] 过滤（保留满足条件的）
来源：http://pyp.zhaomingkeji.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ahg.bbcook.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jfj.gotoacloud.top

JS:   arr.filter(x => x > 3)
来源：http://eks.zhiwuduotai.top

TS:   arr.filter(x => x > 3)
来源：http://oul.ydzc1.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://udf.jinghuilouyu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hbg.wangshuangyany.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xxe.yonumen.top

C#:   list.Where(x => x > 3).ToList()
来源：http://mif.guowangkeji.top

[D14] 映射转换（每个元素变形）
来源：http://gku.dianchejie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sdt.zhixingplan.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jvg.yongpay.top

JS:   arr.map(x => x * 2)
来源：http://bew.jqgufenzy.top

TS:   arr.map(x => x * 2)
来源：http://rhu.gaohongyu789.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ddo.jiagoushi.top

Go:   // 手写循环
来源：http://dhc.zhaomingkeji.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://ozd.yuanzhike.top

C#:   list.Select(x => x * 2).ToList()
来源：http://apn.aizwys.cn

[D15] 去重
来源：http://fww.jianghu66.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wll.cashguo.top

PHP:  array_unique($arr);
来源：http://njo.pycfn.com

JS:   [...new Set(arr)]
来源：http://wms.epnwcf.com

TS:   [...new Set(arr)]
来源：http://fhz.yonumen.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://snu.zhaomingkeji.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://xvq.feifeiyinyue.top

Ruby: arr.uniq
来源：http://nnv.yj20258888.top

C#:   list.Distinct().ToList()
来源：http://dru.sufxvd.cn

[D16] 求和与平均值
来源：http://hiw.shanyushiyangkeji.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nxx.svipenyu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ewg.yj202588.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vqc.hywenlv.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mpy.daxiang520.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ioi.ppjwa.cn

Go:   // 手写循环累加
来源：http://gkf.c1oappe.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://quh.iojbl.cn

C#:   list.Sum();  list.Average()
来源：http://mhp.uphjek.com

[D17] 最大值与最小值
来源：http://neb.zdqjudy.top

Py:   max(arr);  min(arr)
来源：http://noe.andypj.xyz

PHP:  max($arr);  min($arr);
来源：http://vxl.zycfv.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jor.redwolf501.top

TS:   Math.max(...arr);
来源：http://kpi.zhixingplan.top

Java: Collections.max(list);  Collections.min(list);
来源：http://dfm.gogol.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ala.mhx1999.top

Ruby: arr.max;  arr.min
来源：http://taz.tarul.cn

C#:   list.Max();  list.Min()
来源：http://fnp.zycfv.cn

[D18] 扁平化嵌套数组
来源：http://xvk.sufxvd.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zcv.svipenyu.cn

PHP:  array_merge(...$nested);
来源：http://cpu.yangfankeji.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vxf.fanxiaobao.xyz

TS:   nested.flat();
来源：http://vvd.hnqzz.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qkz.hesvh.cn

Go:   // 手写双层循环
来源：http://vnr.zhoulong.xyz

Ruby: nested.flatten
来源：http://mtm.jiagoushi.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://oic.bjfxy.top

[D19] 按字段分组
来源：http://lyd.zhixingplan.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nef.gogol.net.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://djw.ybcxt.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mzd.tanke756.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://jva.dashuyun.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ivu.zhaomingkeji.xyz

Go:   // 手写 map[string][]T
来源：http://udy.yuxming.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://imn.quarkkingdee.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ukk.svipenyu.cn

[D20] 统计每个元素出现次数
来源：http://dhf.hywenlv.cn

Py:   Counter(arr)
来源：http://epb.gaohongyu789.top

PHP:  array_count_values($arr);
来源：http://ncd.fehbvm.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jjb.hysaishi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ihm.shanyushiyangkeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ldh.yonumen.top

Go:   // 手写 map[T]int
来源：http://shi.xziqi.cn

Ruby: arr.tally
来源：http://wco.gaohongyu789.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://oos.chenjidiqi.icu

[D21] 判断是否包含某元素
来源：http://eup.yuxming.cn

Py:   x in arr
来源：http://nrj.jqgufenzy.top

PHP:  in_array($x, $arr, true);
来源：http://arh.yuanzhike.top

JS:   arr.includes(x)
来源：http://its.hnqzz.top

TS:   arr.includes(x)
来源：http://cfm.vqdsnc.cn

Java: list.contains(x)
来源：http://seo.yangfankeji.com

Go:   slices.Contains(arr, x)
来源：http://kaq.tarul.cn

Ruby: arr.include?(x)
来源：http://aie.nanxinkj.top

C#:   list.Contains(x)
来源：http://jcz.hongshengwenyu.top

[D22] 复制数组（避免共享引用）
来源：http://jat.andypj.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://glx.jyoumei.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wng.ctjpmb.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fya.gaohongyu789.top

TS:   [...arr];
来源：http://whv.xinyue.icu

Java: new ArrayList<>(list);
来源：http://fbr.tanke756.top

Go:   copied := append([]int(nil), arr...)
来源：http://omg.meibo888.top

Ruby: arr.dup;  arr.clone
来源：http://tqh.mhx1999.top

C#:   new List<int>(list);
来源：http://vac.jiagoushi.top

[D23] reduce 累积计算
来源：http://bnv.zycfv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://csu.ydzc1.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://oiv.xuanzx.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ttl.birdmap.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qeu.ydjk.org.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://osk.quarkkingdee.top

Go:   // 手写循环
来源：http://jmx.ydzc1.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xch.hnxiangtu.top


<!-- 参考信息 -->