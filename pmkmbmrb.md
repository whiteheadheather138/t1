代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pdc.dashuyun.cn

TS:   arr.map(String)
来源：http://gtz.jiagoushi.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dib.andypj.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qaj.guowangkeji.top

Ruby: arr.map(&:upcase)
来源：http://lar.snrcjt.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ntq.yonumen.top

[C08] 闭包
来源：http://aya.guowangkeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://idb.tarul.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://omz.aizwys.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qdq.pycfn.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kpi.daxiang520.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://boj.tarul.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://axj.guowangkeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://agb.sxryk.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gbz.sufxvd.cn

[C09] 递归
来源：http://ahg.hammf.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qpz.zhoulong.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hng.quarkkingdee.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kbx.hysaishi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wsu.wangdashe.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tnj.havefunace.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gfg.aizwys.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://imv.dianchejie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bjs.kuanghao11.cn

[C10] 变量作用域
来源：http://das.cashguo.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://olh.chenjidiqi.icu

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kzq.guowangkeji.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rkf.jinghuilouyu.cn

TS:   同 JS
来源：http://eni.fehbvm.com

Java: 方法内为块级作用域
来源：http://zqo.yvedp.cn

Go:   花括号块级作用域
来源：http://xce.hongshengwenyu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vfi.xuanzx.com

C#:   块级作用域
来源：http://pep.jqgfzy.top

[C11] 模块导入与导出
来源：http://uvd.yj202588.top

Py:   from module import func
来源：http://usn.ctjpmb.com

PHP:  require "file.php";  或 use App\Service;
来源：http://fyd.hesvh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zlp.cdnleiting.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://scy.guannengcc.top

Java: import java.util.List;
来源：http://uni.ehwqpu.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://eur.epnwcf.com

Ruby: require "json"; require_relative "./util"
来源：http://xrr.jqgufenzy.top

C#:   using System.Text;
来源：http://okh.zhoulong.xyz

[C12] 立即执行函数 IIFE
来源：http://dae.aizwys.cn

Py:   (lambda: print("run"))()
来源：http://ilg.zhiwuduotai.top

PHP:  (function () { echo "run"; })();
来源：http://mcu.epnwcf.com

JS:   (() => { console.log("run"); })();
来源：http://kdg.yangfankeji.com

TS:   (() => { console.log("run"); })();
来源：http://lru.cdnleiting.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://llz.fzhhl.top

Go:   func() { fmt.Println("run") }()
来源：http://naa.gotoacloud.top

Ruby: -> { puts "run" }.call
来源：http://uzy.zhoulong.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://fqa.chenzaomai.com

[C13] 类型声明 / 类型注解
来源：http://vlx.shangyingyoupin.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ggs.pycfn.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://efz.ydjk.org.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://eor.chenjidiqi.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tnp.sysykeji.top

Java: int add(int a, int b) { return a + b; }
来源：http://nlh.wangdashe.top

Go:   func add(a, b int) int
来源：http://fyt.andypj.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kbw.hcnkem.com

C#:   int Add(int a, int b) => a + b;
来源：http://hmn.vehdjk.com

[C14] 泛型函数
来源：http://fft.yonumen.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vze.nwbrower.top

PHP:  // 无泛型
来源：http://mgh.yanxiufei.cn

JS:   // 无泛型
来源：http://ely.jinghuilouyu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://aso.snrcjt.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ajr.mhx1999.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qtx.fanxiaobao.xyz

Ruby: # 无泛型
来源：http://hmb.zhijiandao.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kbb.yonumen.top

[C15] 解构 / 展开参数
来源：http://xrl.fehbvm.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kef.zhongyouzk.top

PHP:  [$a, $b] = $pair;
来源：http://jdt.quarkkingdee.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ibu.chenzaomai.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wpo.vehdjk.com

Java: // 无解构
来源：http://jjo.epnwcf.com

Go:   // 无解构
来源：http://knk.hcnkem.com

Ruby: a, b = pair
来源：http://npr.tanke756.top

C#:   var (a, b) = pair;
来源：http://szb.sysykeji.top

[C16] 函数 / 方法重载
来源：http://zog.zhengqikj.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://oip.uphjek.com

PHP:  // 无重载
来源：http://hbk.jinyuanbaomall.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://eth.feifeiyinyue.top

TS:   // 用联合类型或重载签名声明
来源：http://oqi.wangdashe.top

Java: void f(int a) {}  void f(String a) {}
来源：http://qji.mhx1999.top

Go:   // 无重载：用不同函数名
来源：http://bxm.ehwqpu.com

Ruby: # 无重载：靠动态参数
来源：http://zkm.ehwqpu.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://oxm.ydzc1.top

================================================================================
来源：http://mfb.uphjek.com

D. 数组 / 列表 / 集合
来源：http://ebh.zhixingplan.top

================================================================================
来源：http://qiz.ppjwa.cn

[D01] 创建数组 / 列表
来源：http://rxe.zhixingplan.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://eag.iojbl.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gqk.snrcjt.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://iue.hammf.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://sut.yangfankeji.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jsi.shuidangran.top

Go:   arr := []int{1, 2, 3}
来源：http://gal.ctjpmb.com

Ruby: arr = [1, 2, 3]
来源：http://mbe.aizwys.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ltq.jqgfzy.top

[D02] 追加元素到末尾
来源：http://hcl.xylfe.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zcy.yuxming.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ksv.zhaomingkeji.xyz

JS:   arr.push(4);
来源：http://xjq.yonumen.top

TS:   arr.push(4);
来源：http://whv.jiagoushi.top

Java: list.add(4);
来源：http://arr.shzxlz.cn

Go:   arr = append(arr, 4)
来源：http://vvw.zhengqikj.top

Ruby: arr << 4; arr.push(5)
来源：http://irm.guowangkeji.top

C#:   list.Add(4);
来源：http://bpd.yueranfly.top

[D03] 在指定位置插入元素
来源：http://kev.hysaishi.cn

Py:   arr.insert(0, 0)
来源：http://kxu.jinghuilouyu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ron.shanyushiyangkeji.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gdk.zhongyouzk.top

TS:   arr.splice(0, 0, 0);
来源：http://cxc.zhoulong.xyz

Java: list.add(0, 0);
来源：http://rjg.dianchejie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://akj.9152youxi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yoc.zhoulong.xyz

C#:   list.Insert(0, 0);
来源：http://ovc.cucudq.cn

[D04] 删除元素
来源：http://qcd.yonumen.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wff.xuanzx.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sqp.tarul.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vmz.uphjek.com

TS:   arr.splice(0, 1);
来源：http://vio.zhixingplan.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dyc.xuetiantiany.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ygw.hongshengwenyu.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ihh.yvedp.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fqt.dashuyun.cn

[D05] 访问与修改元素
来源：http://wel.ctjpmb.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rpy.sjlbkw.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zlk.fengsongda.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tww.yj20258.top

TS:   arr[0]; arr.at(-1);
来源：http://upk.yangfankeji.com

Java: list.get(0); list.set(0, 9);
来源：http://auu.tian-w.cn

Go:   arr[0]; arr[0] = 9
来源：http://mgx.yuxming.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yoj.zycfv.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://evi.uphjek.com

[D06] 数组长度
来源：http://tqs.yonumen.top

Py:   len(arr)
来源：http://kjs.hysaishi.cn

PHP:  count($arr);
来源：http://pfc.zhiwuduotai.top

JS:   arr.length
来源：http://osf.yuanzhike.top

TS:   arr.length
来源：http://aiv.xylfe.cn

Java: list.size();
来源：http://hxp.zhengqikj.top

Go:   len(arr)
来源：http://xmc.dianchejie.cn

Ruby: arr.length; arr.size
来源：http://lsp.aibaodan.cn

C#:   list.Count;
来源：http://pfq.zhoulong.xyz

[D07] 切片 / 取子数组
来源：http://cja.gogol.net.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://evx.fanxiaobao.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://rzb.zhoulong.xyz

JS:   arr.slice(1, 4);
来源：http://yjl.chenjidiqi.icu

TS:   arr.slice(1, 4);
来源：http://amj.tarul.cn

Java: list.subList(1, 4);
来源：http://bdi.quarkkingdee.top

Go:   arr[1:4]
来源：http://yng.jinghuilouyu.cn

Ruby: arr[1, 3]
来源：http://ljb.kuanghao11.cn

C#:   list.GetRange(1, 3);
来源：http://qrh.gaohongyu789.top

[D08] 合并两个数组
来源：http://feh.jqgfzy.top

Py:   a + b;  a.extend(b)
来源：http://dji.xingfuxueyuan.xyz

PHP:  array_merge($a, $b);
来源：http://cmr.aibaodan.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zpq.fzhhl.top

TS:   [...a, ...b];
来源：http://eif.fzhhl.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qtx.gotoacloud.top

Go:   append(a, b...)
来源：http://gka.guowangkeji.top

Ruby: a + b;  a.concat(b)
来源：http://nib.tanke756.top

C#:   a.Concat(b).ToList()
来源：http://uab.yj20258.top

[D09] 排序（升序）
来源：http://xia.zhaomingkeji.xyz

Py:   sorted(arr);  arr.sort()
来源：http://itu.chenlongwang.top

PHP:  sort($arr);
来源：http://uvf.snrcjt.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xrs.xingfuxueyuan.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://ykt.zhaomingkeji.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://bkg.tianlin.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qod.gzhubu.top

Ruby: arr.sort
来源：http://ell.jlsjyb.cn

C#:   list.Sort();
来源：http://bfh.yangfankeji.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://hps.ywan-chungtsiang.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zha.jqgfzy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://miq.fehbvm.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dgt.yfazqb.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://auy.zhengqikj.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nmb.yangfankeji.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://poi.zhengqikj.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zsc.zhongyouzk.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://olu.redwolf501.top

[D11] 反转数组
来源：http://tzh.daxiang520.top

Py:   arr[::-1];  arr.reverse()
来源：http://veg.zdbjq.cn

PHP:  array_reverse($arr);
来源：http://jqd.jyoumei.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://knv.cqqwz.cn

TS:   [...arr].reverse();
来源：http://gyf.ppjwa.cn

Java: Collections.reverse(list);
来源：http://tgu.hcnkem.com

Go:   slices.Reverse(arr)
来源：http://wgp.shuidangran.top

Ruby: arr.reverse
来源：http://vvg.sxryk.cn

C#:   list.Reverse();
来源：http://bht.jianghu66.top

[D12] 查找元素下标
来源：http://nan.yj20258888.top

Py:   arr.index(x);  x in arr
来源：http://clg.zhengqikj.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xwn.c1oappe.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nxd.sweek.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uaz.zhaomingkeji.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ihp.c1oappe.top

Go:   slices.Index(arr, x)
来源：http://onl.guowangkeji.top

Ruby: arr.index(x)
来源：http://anh.cucudq.cn

C#:   list.IndexOf(x);
来源：http://gbg.ydjk.org.cn

[D13] 过滤（保留满足条件的）
来源：http://did.ydzc1.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fzy.redwolf501.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://epm.zhijiandao.cn

JS:   arr.filter(x => x > 3)
来源：http://bmb.jianghu66.top

TS:   arr.filter(x => x > 3)
来源：http://tcc.chenlongwang.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ujz.vehdjk.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tee.yanxiufei.cn

Ruby: arr.select { |x| x > 3 }
来源：http://aue.cdnleiting.top

C#:   list.Where(x => x > 3).ToList()
来源：http://gkx.xuanzx.com

[D14] 映射转换（每个元素变形）
来源：http://rqe.aibaodan.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ykd.hnxiangtu.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://slf.fengsongda.top

JS:   arr.map(x => x * 2)
来源：http://jly.ydjk.org.cn

TS:   arr.map(x => x * 2)
来源：http://bjh.chenlongwang.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://fmb.nwbrower.top

Go:   // 手写循环
来源：http://drg.redwolf501.top

Ruby: arr.map { |x| x * 2 }
来源：http://ksb.yj202588.top

C#:   list.Select(x => x * 2).ToList()
来源：http://col.yangfankeji.com

[D15] 去重
来源：http://kue.jinghuilouyu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rhc.sjlbkw.cn

PHP:  array_unique($arr);
来源：http://aky.316326.xyz

JS:   [...new Set(arr)]
来源：http://azt.bbcook.cn

TS:   [...new Set(arr)]
来源：http://nnn.tian-w.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gjl.bbcook.cn

Go:   // 用 map[T]struct{} 手写
来源：http://rxv.yuanzhike.top

Ruby: arr.uniq
来源：http://vul.nwbrower.top

C#:   list.Distinct().ToList()
来源：http://wcf.zdbjq.cn

[D16] 求和与平均值
来源：http://bxf.wangshuangyany.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://eiv.hnxiangtu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kbo.cdnleiting.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ofs.cqqwz.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pay.316326.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://eoo.zhengqikj.top

Go:   // 手写循环累加
来源：http://qse.gzhubu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lwu.sufxvd.cn

C#:   list.Sum();  list.Average()
来源：http://dby.zdqjudy.top

[D17] 最大值与最小值
来源：http://mlt.jiagoushi.top

Py:   max(arr);  min(arr)
来源：http://eez.xuetiantiany.cn

PHP:  max($arr);  min($arr);
来源：http://uwy.zdqjudy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lok.yueranfly.top

TS:   Math.max(...arr);
来源：http://bwk.havefunace.top

Java: Collections.max(list);  Collections.min(list);
来源：http://zbv.zhengqikj.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xet.gzhubu.top

Ruby: arr.max;  arr.min
来源：http://eyw.redwolf501.top

C#:   list.Max();  list.Min()
来源：http://sem.cheryme.top

[D18] 扁平化嵌套数组
来源：http://eyk.pengpengdd.cyou

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ngy.haohaochexian.top

PHP:  array_merge(...$nested);
来源：http://fov.yueranfly.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://eqt.gzhubu.top

TS:   nested.flat();
来源：http://zdm.pengpengdd.cyou

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ozl.jiagoushi.top

Go:   // 手写双层循环
来源：http://yvv.nanxinkj.top

Ruby: nested.flatten
来源：http://ykm.c1oappe.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://qwp.xziqi.cn

[D19] 按字段分组
来源：http://hxt.iojbl.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zfy.haohaochexian.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dov.ehwqpu.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ygu.wangdashe.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://coy.xziqi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mjs.tarul.cn

Go:   // 手写 map[string][]T
来源：http://xak.yfazqb.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://vvj.vqdsnc.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fch.redwolf501.top

[D20] 统计每个元素出现次数
来源：http://tte.pengpengdd.cyou

Py:   Counter(arr)
来源：http://uyz.jinyuanbaomall.cn

PHP:  array_count_values($arr);
来源：http://dnb.daria6918.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nzb.birdmap.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ecc.yvedp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ydg.gotoacloud.top

Go:   // 手写 map[T]int
来源：http://fff.mhx1999.top

Ruby: arr.tally
来源：http://wng.bbcook.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xsk.havefunace.top

[D21] 判断是否包含某元素
来源：http://rve.vehdjk.com

Py:   x in arr
来源：http://bsh.52xcode.cn

PHP:  in_array($x, $arr, true);
来源：http://rii.ivvv.top

JS:   arr.includes(x)
来源：http://dbg.uphjek.com

TS:   arr.includes(x)
来源：http://fbv.ehwqpu.com

Java: list.contains(x)
来源：http://pcy.ywan-chungtsiang.top

Go:   slices.Contains(arr, x)
来源：http://xbv.andypj.xyz

Ruby: arr.include?(x)
来源：http://zyk.havefunace.top

C#:   list.Contains(x)
来源：http://cpg.havefunace.top

[D22] 复制数组（避免共享引用）
来源：http://vte.xingfuxueyuan.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nqs.gotoacloud.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mac.shzxlz.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://omp.jqgufenzy.top

TS:   [...arr];
来源：http://dat.xuetiantiany.cn

Java: new ArrayList<>(list);
来源：http://jjn.aibaodan.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rqd.zhongyouzk.top

Ruby: arr.dup;  arr.clone
来源：http://ter.zhixingplan.top

C#:   new List<int>(list);
来源：http://ksl.bjfxy.top

[D23] reduce 累积计算
来源：http://jfu.yanxiufei.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tal.sweek.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://psj.jinqigfzy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bno.xuetiantiany.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fkr.epnwcf.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://ytp.epnwcf.com

Go:   // 手写循环
来源：http://ayr.c1oappe.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ope.fktsv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://plf.ywan-chungtsiang.top

[D24] 字典 / Map 基本操作
来源：http://hlv.cucudq.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jwz.andypj.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jkv.bjfxy.top


<!-- 参考信息 -->