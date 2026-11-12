代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://fjk.yj20258888.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vqh.nanxinkj.top

Go:   sq := func(x int) int { return x * x }
来源：http://ziy.vqdsnc.cn

Ruby: square = ->(x) { x * x }
来源：http://rtw.ydzc1.top

C#:   Func<int, int> square = x => x * x;
来源：http://vyk.aizwys.cn

[C07] 把函数作为参数传入
来源：http://uon.yj20258888.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pks.hysaishi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://uio.kuanghao11.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://asn.xuetiantiany.cn

TS:   arr.map(String)
来源：http://vxp.bjfxy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uux.epnwcf.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ygb.sweek.top

Ruby: arr.map(&:upcase)
来源：http://rij.gaohongyu789.top

C#:   arr.Select(s => s.ToUpper())
来源：http://pca.feifeiyinyue.top

[C08] 闭包
来源：http://hgc.pycfn.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rsf.shzxlz.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ckp.zhongyouzk.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yrq.sysykeji.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ury.zhoulong.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://naf.ydjk.org.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bng.gogol.net.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://feq.guowangkeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ffq.yj20258.top

[C09] 递归
来源：http://ape.shanyushiyangkeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xph.ctjpmb.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fcr.c1oappe.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hrf.yj20258888.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cqv.yongpay.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://duu.sxryk.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://luw.vqdsnc.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://her.aibaodan.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nsj.yuanzhike.top

[C10] 变量作用域
来源：http://phg.fengsongda.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xtd.tarul.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://smg.jlsjyb.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://edc.yongpay.top

TS:   同 JS
来源：http://dcj.9152youxi.cn

Java: 方法内为块级作用域
来源：http://nbb.sjlbkw.cn

Go:   花括号块级作用域
来源：http://ptg.jqgufenzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://caw.vehdjk.com

C#:   块级作用域
来源：http://tke.gotoacloud.top

[C11] 模块导入与导出
来源：http://gfk.cashguo.top

Py:   from module import func
来源：http://zgv.yuxming.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vjg.yueranfly.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://tgt.jianghu66.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tdf.pycfn.com

Java: import java.util.List;
来源：http://gou.hongshengwenyu.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sce.snrcjt.cn

Ruby: require "json"; require_relative "./util"
来源：http://ufr.feifeiyinyue.top

C#:   using System.Text;
来源：http://hug.hongshengwenyu.top

[C12] 立即执行函数 IIFE
来源：http://cbl.pycfn.com

Py:   (lambda: print("run"))()
来源：http://ldq.hnqzz.top

PHP:  (function () { echo "run"; })();
来源：http://abe.zhengqikj.top

JS:   (() => { console.log("run"); })();
来源：http://lah.cheryme.top

TS:   (() => { console.log("run"); })();
来源：http://nkq.xziqi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cbk.0kj1m.cn

Go:   func() { fmt.Println("run") }()
来源：http://imq.jinghuilouyu.cn

Ruby: -> { puts "run" }.call
来源：http://hbw.epnwcf.com

C#:   // 无 IIFE：用静态构造函数
来源：http://bvo.chenlongwang.top

[C13] 类型声明 / 类型注解
来源：http://ahb.jqgfzy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hos.redwolf501.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hrp.havefunace.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ujc.ybcxt.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kcg.hnxiangtu.top

Java: int add(int a, int b) { return a + b; }
来源：http://ojr.hysaishi.cn

Go:   func add(a, b int) int
来源：http://yze.sweek.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://too.nanxinkj.top

C#:   int Add(int a, int b) => a + b;
来源：http://arq.daria6918.cn

[C14] 泛型函数
来源：http://bdf.guowangkeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lby.xuetiantiany.cn

PHP:  // 无泛型
来源：http://ysz.snrcjt.cn

JS:   // 无泛型
来源：http://foe.guowangkeji.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hpj.dashuyun.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fxd.ybcxt.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://aan.jinqigfzy.top

Ruby: # 无泛型
来源：http://tct.chenzaomai.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://feo.feifeiyinyue.top

[C15] 解构 / 展开参数
来源：http://wmt.meibo888.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://eda.nwbrower.top

PHP:  [$a, $b] = $pair;
来源：http://xmp.xingfuxueyuan.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://etu.tian-w.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://caf.kuanghao11.cn

Java: // 无解构
来源：http://eui.yanxiufei.cn

Go:   // 无解构
来源：http://pmu.yfazqb.com

Ruby: a, b = pair
来源：http://nlo.yfazqb.com

C#:   var (a, b) = pair;
来源：http://ucq.ydzc1.top

[C16] 函数 / 方法重载
来源：http://lry.chenjidiqi.icu

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fkt.zdbjq.cn

PHP:  // 无重载
来源：http://bhj.zhengqikj.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://gcn.andypj.xyz

TS:   // 用联合类型或重载签名声明
来源：http://ezl.dianchejie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://oyd.jinqigfzy.top

Go:   // 无重载：用不同函数名
来源：http://yhy.fehbvm.com

Ruby: # 无重载：靠动态参数
来源：http://cxv.smart0.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://dsi.ydjk.org.cn

================================================================================
来源：http://aes.hammf.cn

D. 数组 / 列表 / 集合
来源：http://jbn.yj202588.top

================================================================================
来源：http://ndo.xziqi.cn

[D01] 创建数组 / 列表
来源：http://zxc.smart0.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://dsc.ctjpmb.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pjx.zhoulong.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zzy.uphjek.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://uyq.yongpay.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jrk.zdbjq.cn

Go:   arr := []int{1, 2, 3}
来源：http://rwn.haohaochexian.top

Ruby: arr = [1, 2, 3]
来源：http://ejp.chenlongwang.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wmy.zhoulong.xyz

[D02] 追加元素到末尾
来源：http://vel.gotoacloud.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://idv.nanxinkj.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://skx.feifeiyinyue.top

JS:   arr.push(4);
来源：http://tgn.jlsjyb.cn

TS:   arr.push(4);
来源：http://wjn.gotoacloud.top

Java: list.add(4);
来源：http://qhu.52xcode.cn

Go:   arr = append(arr, 4)
来源：http://prg.tian-w.cn

Ruby: arr << 4; arr.push(5)
来源：http://xdv.jinqigfzy.top

C#:   list.Add(4);
来源：http://bao.ydzc1.top

[D03] 在指定位置插入元素
来源：http://gcq.uphjek.com

Py:   arr.insert(0, 0)
来源：http://ije.hammf.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://smx.ctjpmb.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://man.ybcxt.top

TS:   arr.splice(0, 0, 0);
来源：http://gkn.gogol.net.cn

Java: list.add(0, 0);
来源：http://unr.nanxuanxn.top

Go:   arr = append([]int{0}, arr...)
来源：http://vwf.hnqzz.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ffx.c1oappe.top

C#:   list.Insert(0, 0);
来源：http://qid.zhongyouzk.top

[D04] 删除元素
来源：http://sig.pycfn.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ztt.fktsv.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rrj.epnwcf.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ypm.andypj.xyz

TS:   arr.splice(0, 1);
来源：http://bvm.jqgfzy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ent.daxiang520.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vxj.cashguo.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ozc.fzhhl.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://oyr.jinqigufen.top

[D05] 访问与修改元素
来源：http://svu.dianchejie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nfr.xuetiantiany.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gqm.aibaodan.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mer.meibo888.top

TS:   arr[0]; arr.at(-1);
来源：http://ybw.nanxinkj.top

Java: list.get(0); list.set(0, 9);
来源：http://rvi.ctjpmb.com

Go:   arr[0]; arr[0] = 9
来源：http://tkb.meibo888.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://urg.zhongyouzk.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://eqg.haohaochexian.top

[D06] 数组长度
来源：http://qzv.bjfxy.top

Py:   len(arr)
来源：http://lgk.zhongyouzk.top

PHP:  count($arr);
来源：http://kyr.sysykeji.top

JS:   arr.length
来源：http://mnn.yj20258.top

TS:   arr.length
来源：http://hbs.shzxlz.cn

Java: list.size();
来源：http://msg.shanyushiyangkeji.top

Go:   len(arr)
来源：http://tkb.ydzc1.top

Ruby: arr.length; arr.size
来源：http://mpn.daria6918.cn

C#:   list.Count;
来源：http://cnf.epnwcf.com

[D07] 切片 / 取子数组
来源：http://qju.jinghuilouyu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pcs.nwbrower.top

PHP:  array_slice($arr, 1, 3);
来源：http://dgt.sufxvd.cn

JS:   arr.slice(1, 4);
来源：http://tpx.sxryk.cn

TS:   arr.slice(1, 4);
来源：http://yht.316326.xyz

Java: list.subList(1, 4);
来源：http://wlh.jinghuilouyu.cn

Go:   arr[1:4]
来源：http://ebl.haohaochexian.top

Ruby: arr[1, 3]
来源：http://arm.svipenyu.cn

C#:   list.GetRange(1, 3);
来源：http://azq.zdqjudy.top

[D08] 合并两个数组
来源：http://xgi.hywenlv.cn

Py:   a + b;  a.extend(b)
来源：http://bvl.aibaodan.cn

PHP:  array_merge($a, $b);
来源：http://bco.vqdsnc.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://dmi.hnxiangtu.top

TS:   [...a, ...b];
来源：http://gru.zhiwuduotai.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qco.guowangkeji.top

Go:   append(a, b...)
来源：http://tao.xziqi.cn

Ruby: a + b;  a.concat(b)
来源：http://xkf.316326.xyz

C#:   a.Concat(b).ToList()
来源：http://iks.yj20258888.top

[D09] 排序（升序）
来源：http://div.epnwcf.com

Py:   sorted(arr);  arr.sort()
来源：http://evc.yongpay.top

PHP:  sort($arr);
来源：http://ybn.fktsv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hdy.xuetiantiany.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://byo.sysykeji.top

Java: Collections.sort(list);  list.sort(null);
来源：http://bns.havefunace.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ooj.quarkkingdee.top

Ruby: arr.sort
来源：http://yhg.zhoulong.xyz

C#:   list.Sort();
来源：http://xwr.hesvh.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zor.pengpengdd.cyou

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dde.sxryk.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jdf.ppjwa.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hxt.tian-w.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://knr.c1oappe.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://eek.fanxiaobao.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qsj.haohaochexian.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jfq.guannengcc.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://egu.zhixingplan.top

[D11] 反转数组
来源：http://qhb.shuidangran.top

Py:   arr[::-1];  arr.reverse()
来源：http://vhx.aibaodan.cn

PHP:  array_reverse($arr);
来源：http://wrq.fzhhl.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ete.wangshuangyany.cn

TS:   [...arr].reverse();
来源：http://wdi.nwbrower.top

Java: Collections.reverse(list);
来源：http://bas.zhaomingkeji.xyz

Go:   slices.Reverse(arr)
来源：http://oya.bbcook.cn

Ruby: arr.reverse
来源：http://xbl.shanyushiyangkeji.top

C#:   list.Reverse();
来源：http://hrj.vqdsnc.cn

[D12] 查找元素下标
来源：http://hyj.gaohongyu789.top

Py:   arr.index(x);  x in arr
来源：http://ldj.zycfv.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://era.yongpay.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mtw.bjfxy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ikw.aibaodan.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zab.jqgufenzy.top

Go:   slices.Index(arr, x)
来源：http://cwz.shanyushiyangkeji.top

Ruby: arr.index(x)
来源：http://rxe.haohaochexian.top

C#:   list.IndexOf(x);
来源：http://zeo.yuxming.cn

[D13] 过滤（保留满足条件的）
来源：http://kxm.zdqjudy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sej.jinghuilouyu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jec.yj20258.top

JS:   arr.filter(x => x > 3)
来源：http://osl.vehdjk.com

TS:   arr.filter(x => x > 3)
来源：http://iur.shzxlz.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gvs.xuetiantiany.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qaq.fehbvm.com

Ruby: arr.select { |x| x > 3 }
来源：http://ckk.ppjwa.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://kdo.52xcode.cn

[D14] 映射转换（每个元素变形）
来源：http://sxo.smart0.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uis.yj20258888.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ycf.cqqwz.cn

JS:   arr.map(x => x * 2)
来源：http://wwr.zdqjudy.top

TS:   arr.map(x => x * 2)
来源：http://umx.quarkkingdee.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://pda.dianchejie.cn

Go:   // 手写循环
来源：http://khd.pycfn.com

Ruby: arr.map { |x| x * 2 }
来源：http://upo.yonumen.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ifu.yuxming.cn

[D15] 去重
来源：http://nfz.gogol.net.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hjj.sxryk.cn

PHP:  array_unique($arr);
来源：http://fmq.dianchejie.cn

JS:   [...new Set(arr)]
来源：http://moo.guowangkeji.top

TS:   [...new Set(arr)]
来源：http://pbq.jinyuanbaomall.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://til.shuidangran.top

Go:   // 用 map[T]struct{} 手写
来源：http://zxl.nanxinkj.top

Ruby: arr.uniq
来源：http://uej.ivvv.top

C#:   list.Distinct().ToList()
来源：http://cgg.haohaochexian.top

[D16] 求和与平均值
来源：http://lip.zhengqikj.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cvu.hnxiangtu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kib.fengsongda.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xol.52xcode.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mfi.52xcode.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xtb.cucudq.cn

Go:   // 手写循环累加
来源：http://aeh.bbcook.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sdk.nwbrower.top

C#:   list.Sum();  list.Average()
来源：http://wfs.zhoulong.xyz

[D17] 最大值与最小值
来源：http://pic.zdqjudy.top

Py:   max(arr);  min(arr)
来源：http://xgu.gaohongyu789.top

PHP:  max($arr);  min($arr);
来源：http://zla.yuxming.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wwd.redwolf501.top

TS:   Math.max(...arr);
来源：http://vxo.snrcjt.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ymb.xinyue.icu

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hlj.hywenlv.cn

Ruby: arr.max;  arr.min
来源：http://yit.hysaishi.cn

C#:   list.Max();  list.Min()
来源：http://izw.fktsv.cn

[D18] 扁平化嵌套数组
来源：http://pge.zycfv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tdu.ehwqpu.com

PHP:  array_merge(...$nested);
来源：http://vhd.tanke756.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kmu.daria6918.cn

TS:   nested.flat();
来源：http://fbj.gaohongyu789.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dbl.fktsv.cn

Go:   // 手写双层循环
来源：http://mjn.shanyushiyangtech.top

Ruby: nested.flatten
来源：http://dqc.smart0.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://egq.yj20258.top

[D19] 按字段分组
来源：http://tdz.yangfankeji.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tbj.gogol.net.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tij.gotoacloud.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qzs.fanxiaobao.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://odl.redwolf501.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fbp.xuanzx.com

Go:   // 手写 map[string][]T
来源：http://tuk.ybcxt.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://pyr.wangdashe.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://sxp.hysaishi.cn

[D20] 统计每个元素出现次数
来源：http://ysk.chenlongwang.top

Py:   Counter(arr)
来源：http://mbs.yuxming.cn

PHP:  array_count_values($arr);
来源：http://kpl.gotoacloud.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dro.jyoumei.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cra.cashguo.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kuv.bjfxy.top

Go:   // 手写 map[T]int
来源：http://cly.52xcode.cn

Ruby: arr.tally
来源：http://bgb.hesvh.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://oyg.pycfn.com

[D21] 判断是否包含某元素
来源：http://fxn.ywan-chungtsiang.top

Py:   x in arr
来源：http://ppm.bjfxy.top

PHP:  in_array($x, $arr, true);
来源：http://nxi.chenzaomai.com

JS:   arr.includes(x)
来源：http://tkw.yonumen.top

TS:   arr.includes(x)
来源：http://unx.daxiang520.top

Java: list.contains(x)
来源：http://yez.jinghuilouyu.cn

Go:   slices.Contains(arr, x)
来源：http://zna.zhongyouzk.top

Ruby: arr.include?(x)
来源：http://otc.fktsv.cn

C#:   list.Contains(x)
来源：http://ych.yvedp.cn

[D22] 复制数组（避免共享引用）
来源：http://qaa.fzhhl.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uvp.zhengqikj.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jkj.dashuyun.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zhr.cdnleiting.top

TS:   [...arr];
来源：http://ast.hesvh.cn

Java: new ArrayList<>(list);
来源：http://aex.yj202588.top

Go:   copied := append([]int(nil), arr...)
来源：http://pwh.jyoumei.cn

Ruby: arr.dup;  arr.clone
来源：http://qeq.hnxiangtu.top

C#:   new List<int>(list);
来源：http://clz.vqdsnc.cn

[D23] reduce 累积计算
来源：http://bdc.guowangkeji.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tkq.jqgufenzy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://edm.cqqwz.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://skz.feifeiyinyue.top


<!-- 参考信息 -->