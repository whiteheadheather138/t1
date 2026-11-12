代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://auq.guannengcc.top

Go:   return a, b
来源：http://krm.daxiang520.top

Ruby: return a, b
来源：http://zxs.yfazqb.com

C#:   return (a, b);              // ValueTuple
来源：http://qup.uphjek.com

[C06] 匿名函数 / lambda
来源：http://ygt.cdnleiting.top

Py:   square = lambda x: x * x
来源：http://zle.zhixingplan.top

PHP:  $square = fn($x) => $x * $x;
来源：http://wjr.havefunace.top

JS:   const square = x => x * x;
来源：http://gye.nwbrower.top

TS:   const square = (x: number): number => x * x;
来源：http://css.ctjpmb.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dge.pycfn.com

Go:   sq := func(x int) int { return x * x }
来源：http://bob.shzxlz.cn

Ruby: square = ->(x) { x * x }
来源：http://guc.daria6918.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pus.zhixingplan.top

[C07] 把函数作为参数传入
来源：http://bul.nanxinkj.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gwn.tian-w.cn

PHP:  array_map("strtoupper", $arr);
来源：http://oyg.jyoumei.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ddm.fehbvm.com

TS:   arr.map(String)
来源：http://xvu.daria6918.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rvk.ywan-chungtsiang.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ftv.yangfankeji.com

Ruby: arr.map(&:upcase)
来源：http://esw.xuetiantiany.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gkc.hongshengwenyu.top

[C08] 闭包
来源：http://ukw.snrcjt.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qlu.nwbrower.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hph.havefunace.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://flh.pycfn.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://unu.cheryme.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cua.yuanzhike.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nls.hywenlv.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://whp.yuxming.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bhg.chenzaomai.com

[C09] 递归
来源：http://bzd.havefunace.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://doo.shzxlz.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ygh.epnwcf.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vut.vehdjk.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pdm.ydjk.org.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xjc.hcnkem.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bma.zdqjudy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://inr.yuxming.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://czs.yj20258888.top

[C10] 变量作用域
来源：http://mze.xingfuxueyuan.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gmt.gaohongyu789.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xbh.tarul.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://web.shuidangran.top

TS:   同 JS
来源：http://sqn.cashguo.top

Java: 方法内为块级作用域
来源：http://zer.0kj1m.cn

Go:   花括号块级作用域
来源：http://gil.yueranfly.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mrn.xinyue.icu

C#:   块级作用域
来源：http://adz.cashguo.top

[C11] 模块导入与导出
来源：http://ubg.yvedp.cn

Py:   from module import func
来源：http://fvg.daxiang520.top

PHP:  require "file.php";  或 use App\Service;
来源：http://mbe.zhengqikj.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://fcr.hammf.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pnv.9152youxi.cn

Java: import java.util.List;
来源：http://hir.jinqigufen.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bae.vqdsnc.cn

Ruby: require "json"; require_relative "./util"
来源：http://uad.guowangkeji.top

C#:   using System.Text;
来源：http://qib.shanyushiyangkeji.top

[C12] 立即执行函数 IIFE
来源：http://vkm.xuetiantiany.cn

Py:   (lambda: print("run"))()
来源：http://hns.9152youxi.cn

PHP:  (function () { echo "run"; })();
来源：http://qgz.bjfxy.top

JS:   (() => { console.log("run"); })();
来源：http://hmq.bjfxy.top

TS:   (() => { console.log("run"); })();
来源：http://qta.316326.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rvb.hfpthk.cn

Go:   func() { fmt.Println("run") }()
来源：http://bzs.shangyingyoupin.top

Ruby: -> { puts "run" }.call
来源：http://avw.jyoumei.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xrl.jqgufenzy.top

[C13] 类型声明 / 类型注解
来源：http://oac.feifeiyinyue.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lfs.zhengqikj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wps.gotoacloud.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mvn.hywenlv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://skf.hammf.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ldy.ydjk.org.cn

Go:   func add(a, b int) int
来源：http://ibg.andypj.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://etq.yanxiufei.cn

C#:   int Add(int a, int b) => a + b;
来源：http://czm.yvedp.cn

[C14] 泛型函数
来源：http://wjd.fanxiaobao.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lmq.hongshengwenyu.top

PHP:  // 无泛型
来源：http://ghx.hnxiangtu.top

JS:   // 无泛型
来源：http://kdq.jinyuanbaomall.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wkx.wangshuangyany.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lco.zhiwuduotai.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qtw.chenlongwang.top

Ruby: # 无泛型
来源：http://wyt.nwbrower.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cwj.haohaochexian.top

[C15] 解构 / 展开参数
来源：http://zxq.aizwys.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yts.kuanghao11.cn

PHP:  [$a, $b] = $pair;
来源：http://ure.epnwcf.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://giy.andypj.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yht.sweek.top

Java: // 无解构
来源：http://csl.tian-w.cn

Go:   // 无解构
来源：http://wie.nanxuanxn.top

Ruby: a, b = pair
来源：http://pyn.tarul.cn

C#:   var (a, b) = pair;
来源：http://fyy.ywan-chungtsiang.top

[C16] 函数 / 方法重载
来源：http://ugk.xingfuxueyuan.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tfl.zdbjq.cn

PHP:  // 无重载
来源：http://gui.hammf.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://iwx.yj20258.top

TS:   // 用联合类型或重载签名声明
来源：http://yir.yangfankeji.com

Java: void f(int a) {}  void f(String a) {}
来源：http://qaq.52xcode.cn

Go:   // 无重载：用不同函数名
来源：http://vrn.vqdsnc.cn

Ruby: # 无重载：靠动态参数
来源：http://qma.jyoumei.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rea.dashuyun.cn

================================================================================
来源：http://szk.sufxvd.cn

D. 数组 / 列表 / 集合
来源：http://obo.guannengcc.top

================================================================================
来源：http://seu.tianlin.xyz

[D01] 创建数组 / 列表
来源：http://jha.c1oappe.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://yxr.ydzc1.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://siu.hywenlv.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vsh.haohaochexian.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://wep.wangshuangyany.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jzf.9152youxi.cn

Go:   arr := []int{1, 2, 3}
来源：http://jqg.bbcook.cn

Ruby: arr = [1, 2, 3]
来源：http://dxk.nwbrower.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://toc.haohaochexian.top

[D02] 追加元素到末尾
来源：http://gfo.yangfankeji.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cer.ppjwa.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fwc.chenzaomai.com

JS:   arr.push(4);
来源：http://yon.hnqzz.top

TS:   arr.push(4);
来源：http://wrl.yvedp.cn

Java: list.add(4);
来源：http://edi.yj20258888.top

Go:   arr = append(arr, 4)
来源：http://ceh.zdqjudy.top

Ruby: arr << 4; arr.push(5)
来源：http://txx.xziqi.cn

C#:   list.Add(4);
来源：http://fcg.mhx1999.top

[D03] 在指定位置插入元素
来源：http://udi.sweek.top

Py:   arr.insert(0, 0)
来源：http://air.cucudq.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ejc.bbcook.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dkc.zycfv.cn

TS:   arr.splice(0, 0, 0);
来源：http://wgu.gzhubu.top

Java: list.add(0, 0);
来源：http://bmx.yvedp.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vfk.zhoulong.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rzp.zycfv.cn

C#:   list.Insert(0, 0);
来源：http://hsu.xuanzx.com

[D04] 删除元素
来源：http://dsn.xuetiantiany.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rvz.pengpengdd.cyou

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://imo.shanyushiyangtech.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://adt.fktsv.cn

TS:   arr.splice(0, 1);
来源：http://nkf.tian-w.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fko.wangdashe.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nhg.sxryk.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ymr.hywenlv.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yge.fanxiaobao.xyz

[D05] 访问与修改元素
来源：http://uqw.ydjk.org.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://knb.cqqwz.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://duj.hammf.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jpr.sxryk.cn

TS:   arr[0]; arr.at(-1);
来源：http://nne.jinqigfzy.top

Java: list.get(0); list.set(0, 9);
来源：http://fyk.jiagoushi.top

Go:   arr[0]; arr[0] = 9
来源：http://ahu.zdbjq.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bcd.hesvh.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wwa.hammf.cn

[D06] 数组长度
来源：http://rrb.jiagoushi.top

Py:   len(arr)
来源：http://nxm.sufxvd.cn

PHP:  count($arr);
来源：http://xxz.vqdsnc.cn

JS:   arr.length
来源：http://jrc.zhijiandao.cn

TS:   arr.length
来源：http://osq.yuanzhike.top

Java: list.size();
来源：http://kgn.yfazqb.com

Go:   len(arr)
来源：http://ojv.xuanzx.com

Ruby: arr.length; arr.size
来源：http://zln.gzhubu.top

C#:   list.Count;
来源：http://tcd.chenjidiqi.icu

[D07] 切片 / 取子数组
来源：http://jdv.zhengqikj.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://axg.zhengqikj.top

PHP:  array_slice($arr, 1, 3);
来源：http://ocs.jlsjyb.cn

JS:   arr.slice(1, 4);
来源：http://njr.shanyushiyangtech.top

TS:   arr.slice(1, 4);
来源：http://sed.tianlin.xyz

Java: list.subList(1, 4);
来源：http://zjj.zhixingplan.top

Go:   arr[1:4]
来源：http://byx.yj20258.top

Ruby: arr[1, 3]
来源：http://ojl.wangdashe.top

C#:   list.GetRange(1, 3);
来源：http://fre.yuanzhike.top

[D08] 合并两个数组
来源：http://nbf.hywenlv.cn

Py:   a + b;  a.extend(b)
来源：http://tmc.zhengqikj.top

PHP:  array_merge($a, $b);
来源：http://nfb.xingfuxueyuan.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://tvp.epnwcf.com

TS:   [...a, ...b];
来源：http://nbu.tanke756.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rvi.snrcjt.cn

Go:   append(a, b...)
来源：http://gla.zdbjq.cn

Ruby: a + b;  a.concat(b)
来源：http://xdc.zhiwuduotai.top

C#:   a.Concat(b).ToList()
来源：http://xjk.ydjk.org.cn

[D09] 排序（升序）
来源：http://xbx.nwbrower.top

Py:   sorted(arr);  arr.sort()
来源：http://ddb.fengsongda.top

PHP:  sort($arr);
来源：http://jrt.mhx1999.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gxd.fanxiaobao.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://gmh.meibo888.top

Java: Collections.sort(list);  list.sort(null);
来源：http://idq.zhaomingkeji.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://suz.kuanghao11.cn

Ruby: arr.sort
来源：http://wxl.bbcook.cn

C#:   list.Sort();
来源：http://uti.xziqi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fei.zycfv.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://aah.tanke756.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://viv.iojbl.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gfe.ydzc1.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nlt.hcnkem.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://raa.chenjidiqi.icu

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qdk.vehdjk.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ruw.cdnleiting.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ewb.yuxming.cn

[D11] 反转数组
来源：http://our.daria6918.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qvo.yueranfly.top

PHP:  array_reverse($arr);
来源：http://qob.fanxiaobao.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kfq.yueranfly.top

TS:   [...arr].reverse();
来源：http://sdp.chenzaomai.com

Java: Collections.reverse(list);
来源：http://oin.yj20258888.top

Go:   slices.Reverse(arr)
来源：http://dzm.yanxiufei.cn

Ruby: arr.reverse
来源：http://bdz.hesvh.cn

C#:   list.Reverse();
来源：http://zlx.fehbvm.com

[D12] 查找元素下标
来源：http://rlb.jinqigfzy.top

Py:   arr.index(x);  x in arr
来源：http://uzd.shuidangran.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hbf.chenzaomai.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ing.xziqi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zap.fzhhl.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hgu.yj202588.top

Go:   slices.Index(arr, x)
来源：http://dth.jqgufenzy.top

Ruby: arr.index(x)
来源：http://umm.shzxlz.cn

C#:   list.IndexOf(x);
来源：http://sez.jinyuanbaomall.cn

[D13] 过滤（保留满足条件的）
来源：http://gwi.yonumen.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dkq.dianchejie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://idt.sufxvd.cn

JS:   arr.filter(x => x > 3)
来源：http://rnl.snrcjt.cn

TS:   arr.filter(x => x > 3)
来源：http://bwr.sufxvd.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uen.yj20258888.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hen.zhongyouzk.top

Ruby: arr.select { |x| x > 3 }
来源：http://fye.0kj1m.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://naj.smart0.xyz

[D14] 映射转换（每个元素变形）
来源：http://lpr.yj202588.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://skk.haohaochexian.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qxe.tanke756.top

JS:   arr.map(x => x * 2)
来源：http://bnk.tanke756.top

TS:   arr.map(x => x * 2)
来源：http://czb.fehbvm.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://yev.pycfn.com

Go:   // 手写循环
来源：http://snf.xuetiantiany.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jzy.jiagoushi.top

C#:   list.Select(x => x * 2).ToList()
来源：http://jvm.jiagoushi.top

[D15] 去重
来源：http://tce.316326.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sjn.fzhhl.top

PHP:  array_unique($arr);
来源：http://mcp.jinqigfzy.top

JS:   [...new Set(arr)]
来源：http://yve.jianghu66.top

TS:   [...new Set(arr)]
来源：http://mxr.cashguo.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qzd.yongpay.top

Go:   // 用 map[T]struct{} 手写
来源：http://ggh.chenlongwang.top

Ruby: arr.uniq
来源：http://zgy.dianchejie.cn

C#:   list.Distinct().ToList()
来源：http://kvb.hfpthk.cn

[D16] 求和与平均值
来源：http://avw.gzhubu.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://frt.bbcook.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dwy.yfazqb.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jyd.ctjpmb.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pxu.uphjek.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wwh.nanxuanxn.top

Go:   // 手写循环累加
来源：http://jpv.jianghu66.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yxe.hesvh.cn

C#:   list.Sum();  list.Average()
来源：http://ukf.aizwys.cn

[D17] 最大值与最小值
来源：http://fou.epnwcf.com

Py:   max(arr);  min(arr)
来源：http://yxi.shanyushiyangkeji.top

PHP:  max($arr);  min($arr);
来源：http://qjc.sweek.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sgi.hesvh.cn

TS:   Math.max(...arr);
来源：http://rko.shuidangran.top

Java: Collections.max(list);  Collections.min(list);
来源：http://wxj.daxiang520.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cml.jyoumei.cn

Ruby: arr.max;  arr.min
来源：http://jkx.cqqwz.cn

C#:   list.Max();  list.Min()
来源：http://snb.zhoulong.xyz

[D18] 扁平化嵌套数组
来源：http://ini.shuidangran.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ywb.jqgufenzy.top

PHP:  array_merge(...$nested);
来源：http://mbv.haohaochexian.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tua.shzxlz.cn

TS:   nested.flat();
来源：http://ttg.wangshuangyany.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ypm.zhiwuduotai.top

Go:   // 手写双层循环
来源：http://duw.hnqzz.top

Ruby: nested.flatten
来源：http://lyi.gogol.net.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://itc.9152youxi.cn

[D19] 按字段分组
来源：http://udq.jlsjyb.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xhg.chenlongwang.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pdo.sxryk.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zzg.haohaochexian.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://jmv.xylfe.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zmc.bbcook.cn

Go:   // 手写 map[string][]T
来源：http://kwg.birdmap.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://nzz.cqqwz.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mek.jqgufenzy.top

[D20] 统计每个元素出现次数
来源：http://qkh.zhongyouzk.top

Py:   Counter(arr)
来源：http://mth.haohaochexian.top

PHP:  array_count_values($arr);
来源：http://fyk.xinyue.icu

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qxj.vehdjk.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mzt.hcnkem.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xdb.guannengcc.top

Go:   // 手写 map[T]int
来源：http://oyq.yanxiufei.cn

Ruby: arr.tally
来源：http://gtn.hfpthk.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kms.nanxinkj.top

[D21] 判断是否包含某元素
来源：http://pxe.xuetiantiany.cn

Py:   x in arr
来源：http://pfb.hywenlv.cn

PHP:  in_array($x, $arr, true);
来源：http://dhm.cheryme.top

JS:   arr.includes(x)
来源：http://ndm.redwolf501.top

TS:   arr.includes(x)
来源：http://gus.fktsv.cn

Java: list.contains(x)
来源：http://snq.ydzc1.top

Go:   slices.Contains(arr, x)
来源：http://bmd.redwolf501.top

Ruby: arr.include?(x)
来源：http://kjy.yueranfly.top

C#:   list.Contains(x)
来源：http://rjq.daxiang520.top

[D22] 复制数组（避免共享引用）
来源：http://akb.wangdashe.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ekb.zhengqikj.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://low.zhongyouzk.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vkm.jinqigfzy.top

TS:   [...arr];
来源：http://hqu.bbcook.cn


<!-- 参考信息 -->