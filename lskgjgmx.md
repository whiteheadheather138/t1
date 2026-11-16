代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://jfn.sweek.top

[C07] 把函数作为参数传入
来源：http://lzi.ywan-chungtsiang.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qfj.nwbrower.top

PHP:  array_map("strtoupper", $arr);
来源：http://yzy.yonumen.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tvx.jinqigufen.top

TS:   arr.map(String)
来源：http://dgj.zhengqikj.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mll.sufxvd.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dne.xingfuxueyuan.xyz

Ruby: arr.map(&:upcase)
来源：http://edh.sufxvd.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xpu.zdqjudy.top

[C08] 闭包
来源：http://hjx.yongpay.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tre.cdnleiting.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jmc.gaohongyu789.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kca.yj20258888.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dto.shangyingyoupin.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gvt.hysaishi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yco.sweek.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nyp.havefunace.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uje.jyoumei.cn

[C09] 递归
来源：http://odj.fzhhl.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mys.hammf.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nxx.snrcjt.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xtu.haohaochexian.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yss.snrcjt.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xdf.vehdjk.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sjy.zhoulong.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://drn.yonumen.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fsw.epnwcf.com

[C10] 变量作用域
来源：http://cph.nanxuanxn.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vvo.smart0.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ltn.hcnkem.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ngs.nwbrower.top

TS:   同 JS
来源：http://lbl.uphjek.com

Java: 方法内为块级作用域
来源：http://gal.birdmap.top

Go:   花括号块级作用域
来源：http://ehu.zdqjudy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tbs.hcnkem.com

C#:   块级作用域
来源：http://lrn.wangshuangyany.cn

[C11] 模块导入与导出
来源：http://gzd.uphjek.com

Py:   from module import func
来源：http://nyk.tarul.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://cug.daxiang520.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://hyc.cdnleiting.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tez.yj20258.top

Java: import java.util.List;
来源：http://phj.wangdashe.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hpg.zhongyouzk.top

Ruby: require "json"; require_relative "./util"
来源：http://dqg.sxryk.cn

C#:   using System.Text;
来源：http://upt.dashuyun.cn

[C12] 立即执行函数 IIFE
来源：http://hja.aizwys.cn

Py:   (lambda: print("run"))()
来源：http://omr.hesvh.cn

PHP:  (function () { echo "run"; })();
来源：http://gnt.aizwys.cn

JS:   (() => { console.log("run"); })();
来源：http://ibk.hywenlv.cn

TS:   (() => { console.log("run"); })();
来源：http://gdd.52xcode.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://psg.ywan-chungtsiang.top

Go:   func() { fmt.Println("run") }()
来源：http://eqm.nanxuanxn.top

Ruby: -> { puts "run" }.call
来源：http://pum.vehdjk.com

C#:   // 无 IIFE：用静态构造函数
来源：http://hck.sysykeji.top

[C13] 类型声明 / 类型注解
来源：http://uhj.xuanzx.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gdh.hesvh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vbj.zhaomingkeji.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://iqe.yfazqb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ens.xingfuxueyuan.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://fxg.cucudq.cn

Go:   func add(a, b int) int
来源：http://bfi.yj20258.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hru.shanyushiyangtech.top

C#:   int Add(int a, int b) => a + b;
来源：http://snc.uphjek.com

[C14] 泛型函数
来源：http://xfy.sysykeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wsr.hfpthk.cn

PHP:  // 无泛型
来源：http://jsa.aibaodan.cn

JS:   // 无泛型
来源：http://ito.ctjpmb.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://del.pengpengdd.cyou

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vfy.iojbl.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zod.chenlongwang.top

Ruby: # 无泛型
来源：http://yvv.yvedp.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jbu.yonumen.top

[C15] 解构 / 展开参数
来源：http://sjt.bbcook.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wqz.guannengcc.top

PHP:  [$a, $b] = $pair;
来源：http://dhy.hnxiangtu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cbz.zdqjudy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://and.tian-w.cn

Java: // 无解构
来源：http://fhg.vehdjk.com

Go:   // 无解构
来源：http://kww.fanxiaobao.xyz

Ruby: a, b = pair
来源：http://soz.smart0.xyz

C#:   var (a, b) = pair;
来源：http://tqh.dianchejie.cn

[C16] 函数 / 方法重载
来源：http://pks.sysykeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vmo.316326.xyz

PHP:  // 无重载
来源：http://lcp.hammf.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://iwp.uphjek.com

TS:   // 用联合类型或重载签名声明
来源：http://ikg.fanxiaobao.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://soi.fehbvm.com

Go:   // 无重载：用不同函数名
来源：http://gmm.jlsjyb.cn

Ruby: # 无重载：靠动态参数
来源：http://hhh.ctjpmb.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://vrw.yfazqb.com

================================================================================
来源：http://vrw.iojbl.cn

D. 数组 / 列表 / 集合
来源：http://non.shuidangran.top

================================================================================
来源：http://pme.hnqzz.top

[D01] 创建数组 / 列表
来源：http://auj.zhixingplan.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://zup.fengsongda.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wcx.nanxinkj.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://oun.nanxinkj.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://lxu.ywan-chungtsiang.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lad.guannengcc.top

Go:   arr := []int{1, 2, 3}
来源：http://ejz.hywenlv.cn

Ruby: arr = [1, 2, 3]
来源：http://cab.hcnkem.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qxp.9152youxi.cn

[D02] 追加元素到末尾
来源：http://ubm.hammf.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://adi.xuanzx.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://azd.hfpthk.cn

JS:   arr.push(4);
来源：http://bmn.gotoacloud.top

TS:   arr.push(4);
来源：http://xsc.cucudq.cn

Java: list.add(4);
来源：http://ulw.jinqigufen.top

Go:   arr = append(arr, 4)
来源：http://nlh.gaohongyu789.top

Ruby: arr << 4; arr.push(5)
来源：http://uol.sxryk.cn

C#:   list.Add(4);
来源：http://rzz.fengsongda.top

[D03] 在指定位置插入元素
来源：http://ykd.dianchejie.cn

Py:   arr.insert(0, 0)
来源：http://slz.zhiwuduotai.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xpl.shanyushiyangtech.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://irr.hesvh.cn

TS:   arr.splice(0, 0, 0);
来源：http://fxd.wangdashe.top

Java: list.add(0, 0);
来源：http://hec.cheryme.top

Go:   arr = append([]int{0}, arr...)
来源：http://yvq.vehdjk.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ppf.sweek.top

C#:   list.Insert(0, 0);
来源：http://gwh.tianlin.xyz

[D04] 删除元素
来源：http://avg.wangdashe.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tfp.nwbrower.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nya.nanxinkj.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://exr.jianghu66.top

TS:   arr.splice(0, 1);
来源：http://eyw.chenjidiqi.icu

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mhg.yanxiufei.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sxh.yfazqb.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dvk.fzhhl.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://geq.52xcode.cn

[D05] 访问与修改元素
来源：http://zsx.kuanghao11.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nat.vehdjk.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nww.52xcode.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://oyz.ivvv.top

TS:   arr[0]; arr.at(-1);
来源：http://mvs.wangdashe.top

Java: list.get(0); list.set(0, 9);
来源：http://quv.mhx1999.top

Go:   arr[0]; arr[0] = 9
来源：http://obw.xylfe.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mne.vehdjk.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ido.daria6918.cn

[D06] 数组长度
来源：http://gnw.ywan-chungtsiang.top

Py:   len(arr)
来源：http://cab.shanyushiyangkeji.top

PHP:  count($arr);
来源：http://aoo.hnqzz.top

JS:   arr.length
来源：http://hhy.yj20258.top

TS:   arr.length
来源：http://frq.ivvv.top

Java: list.size();
来源：http://jvw.jinyuanbaomall.cn

Go:   len(arr)
来源：http://mka.yj20258.top

Ruby: arr.length; arr.size
来源：http://avu.jqgfzy.top

C#:   list.Count;
来源：http://mcg.jinqigfzy.top

[D07] 切片 / 取子数组
来源：http://tgx.0kj1m.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://owl.zhiwuduotai.top

PHP:  array_slice($arr, 1, 3);
来源：http://yuy.dashuyun.cn

JS:   arr.slice(1, 4);
来源：http://uez.uphjek.com

TS:   arr.slice(1, 4);
来源：http://vwn.zhongyouzk.top

Java: list.subList(1, 4);
来源：http://seb.zdbjq.cn

Go:   arr[1:4]
来源：http://mlv.smart0.xyz

Ruby: arr[1, 3]
来源：http://jnq.xingfuxueyuan.xyz

C#:   list.GetRange(1, 3);
来源：http://zqa.jqgufenzy.top

[D08] 合并两个数组
来源：http://ilw.hcnkem.com

Py:   a + b;  a.extend(b)
来源：http://lfu.aibaodan.cn

PHP:  array_merge($a, $b);
来源：http://orc.iojbl.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://tds.tian-w.cn

TS:   [...a, ...b];
来源：http://ldl.xuetiantiany.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hbj.yuxming.cn

Go:   append(a, b...)
来源：http://yui.pycfn.com

Ruby: a + b;  a.concat(b)
来源：http://iym.xziqi.cn

C#:   a.Concat(b).ToList()
来源：http://hwu.zycfv.cn

[D09] 排序（升序）
来源：http://swf.gotoacloud.top

Py:   sorted(arr);  arr.sort()
来源：http://ems.yj20258.top

PHP:  sort($arr);
来源：http://obt.chenzaomai.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vwu.yueranfly.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://lsd.hywenlv.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://oyy.tianlin.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jdf.jqgfzy.top

Ruby: arr.sort
来源：http://dbv.hysaishi.cn

C#:   list.Sort();
来源：http://olm.nanxinkj.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://qem.tanke756.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tgf.0kj1m.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vsj.0kj1m.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://iuv.yongpay.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ibm.gzhubu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cjr.guannengcc.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lnd.uphjek.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://eue.ywan-chungtsiang.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fpq.hysaishi.cn

[D11] 反转数组
来源：http://idc.aizwys.cn

Py:   arr[::-1];  arr.reverse()
来源：http://fbi.daxiang520.top

PHP:  array_reverse($arr);
来源：http://vrl.zhixingplan.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vkd.ywan-chungtsiang.top

TS:   [...arr].reverse();
来源：http://pjj.feifeiyinyue.top

Java: Collections.reverse(list);
来源：http://cup.fanxiaobao.xyz

Go:   slices.Reverse(arr)
来源：http://esf.jinyuanbaomall.cn

Ruby: arr.reverse
来源：http://cua.zycfv.cn

C#:   list.Reverse();
来源：http://tlq.hnxiangtu.top

[D12] 查找元素下标
来源：http://kgl.xinyue.icu

Py:   arr.index(x);  x in arr
来源：http://dgg.xylfe.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bis.zhaomingkeji.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://beb.snrcjt.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://joa.tian-w.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://elx.zhongyouzk.top

Go:   slices.Index(arr, x)
来源：http://uxx.sweek.top

Ruby: arr.index(x)
来源：http://oyl.tarul.cn

C#:   list.IndexOf(x);
来源：http://ake.wangdashe.top

[D13] 过滤（保留满足条件的）
来源：http://cqi.shanyushiyangtech.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hbc.tanke756.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fvv.quarkkingdee.top

JS:   arr.filter(x => x > 3)
来源：http://ubj.gzhubu.top

TS:   arr.filter(x => x > 3)
来源：http://uiu.ybcxt.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://eqv.jlsjyb.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xot.cashguo.top

Ruby: arr.select { |x| x > 3 }
来源：http://jep.epnwcf.com

C#:   list.Where(x => x > 3).ToList()
来源：http://lri.hesvh.cn

[D14] 映射转换（每个元素变形）
来源：http://uxp.jinghuilouyu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ift.yj202588.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rxx.hfpthk.cn

JS:   arr.map(x => x * 2)
来源：http://zds.cucudq.cn

TS:   arr.map(x => x * 2)
来源：http://hsm.sysykeji.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://rnm.dashuyun.cn

Go:   // 手写循环
来源：http://qmh.jinqigufen.top

Ruby: arr.map { |x| x * 2 }
来源：http://ucx.wangdashe.top

C#:   list.Select(x => x * 2).ToList()
来源：http://tya.ctjpmb.com

[D15] 去重
来源：http://xxw.zhongyouzk.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qaa.xylfe.cn

PHP:  array_unique($arr);
来源：http://hix.dashuyun.cn

JS:   [...new Set(arr)]
来源：http://zsl.0kj1m.cn

TS:   [...new Set(arr)]
来源：http://isj.uphjek.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lqk.iojbl.cn

Go:   // 用 map[T]struct{} 手写
来源：http://sfp.shanyushiyangtech.top

Ruby: arr.uniq
来源：http://omi.xuanzx.com

C#:   list.Distinct().ToList()
来源：http://vpj.ydjk.org.cn

[D16] 求和与平均值
来源：http://wcy.ydjk.org.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tcm.fengsongda.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dce.ctjpmb.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://toq.sjlbkw.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pzk.wangdashe.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://btq.sxryk.cn

Go:   // 手写循环累加
来源：http://hgu.fengsongda.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uku.birdmap.top

C#:   list.Sum();  list.Average()
来源：http://tei.bjfxy.top

[D17] 最大值与最小值
来源：http://lsu.0kj1m.cn

Py:   max(arr);  min(arr)
来源：http://hjc.wangdashe.top

PHP:  max($arr);  min($arr);
来源：http://wsx.chenlongwang.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kfy.tian-w.cn

TS:   Math.max(...arr);
来源：http://dpy.feifeiyinyue.top

Java: Collections.max(list);  Collections.min(list);
来源：http://nhz.feifeiyinyue.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wyb.jyoumei.cn

Ruby: arr.max;  arr.min
来源：http://fkg.tianlin.xyz

C#:   list.Max();  list.Min()
来源：http://wiw.zhoulong.xyz

[D18] 扁平化嵌套数组
来源：http://qaj.hammf.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gto.ppjwa.cn

PHP:  array_merge(...$nested);
来源：http://ref.xingfuxueyuan.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://enx.guannengcc.top

TS:   nested.flat();
来源：http://xuh.xuetiantiany.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://oek.yanxiufei.cn

Go:   // 手写双层循环
来源：http://zmv.cdnleiting.top

Ruby: nested.flatten
来源：http://hri.chenjidiqi.icu

C#:   nested.SelectMany(x => x).ToList()
来源：http://sbo.yueranfly.top

[D19] 按字段分组
来源：http://xjm.andypj.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://oot.hammf.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ncg.jinqigufen.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ebe.dashuyun.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fvi.hfpthk.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://epn.hammf.cn

Go:   // 手写 map[string][]T
来源：http://eav.fzhhl.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://dal.wangshuangyany.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://sty.quarkkingdee.top

[D20] 统计每个元素出现次数
来源：http://nne.hywenlv.cn

Py:   Counter(arr)
来源：http://zkg.xinyue.icu

PHP:  array_count_values($arr);
来源：http://udp.pycfn.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cas.kuanghao11.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lta.xuetiantiany.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sjx.zhoulong.xyz

Go:   // 手写 map[T]int
来源：http://rhc.nanxinkj.top

Ruby: arr.tally
来源：http://ukm.jiagoushi.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vla.jyoumei.cn

[D21] 判断是否包含某元素
来源：http://vjc.chenjidiqi.icu

Py:   x in arr
来源：http://uuj.yuxming.cn

PHP:  in_array($x, $arr, true);
来源：http://euv.aibaodan.cn

JS:   arr.includes(x)
来源：http://yyj.sufxvd.cn

TS:   arr.includes(x)
来源：http://psj.shuidangran.top

Java: list.contains(x)
来源：http://eib.bjfxy.top

Go:   slices.Contains(arr, x)
来源：http://wtv.aibaodan.cn

Ruby: arr.include?(x)
来源：http://ken.xziqi.cn

C#:   list.Contains(x)
来源：http://bnj.9152youxi.cn

[D22] 复制数组（避免共享引用）
来源：http://gss.jyoumei.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://szo.nanxuanxn.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uiq.svipenyu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ycb.jinqigfzy.top

TS:   [...arr];
来源：http://flg.yonumen.top

Java: new ArrayList<>(list);
来源：http://zgw.epnwcf.com

Go:   copied := append([]int(nil), arr...)
来源：http://eqk.xinyue.icu

Ruby: arr.dup;  arr.clone
来源：http://qwi.yj20258888.top

C#:   new List<int>(list);
来源：http://mvh.zhiwuduotai.top

[D23] reduce 累积计算
来源：http://gel.tianlin.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cdg.guannengcc.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zwa.bbcook.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dfz.shangyingyoupin.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uwp.fengsongda.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://owk.shangyingyoupin.top

Go:   // 手写循环
来源：http://lsy.tian-w.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lvk.gaohongyu789.top


<!-- 参考信息 -->