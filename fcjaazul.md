代发 wailian999

[C06] 匿名函数 / lambda
来源：http://fkd.birdmap.top

Py:   square = lambda x: x * x
来源：http://jqg.zhoulong.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://rsm.fktsv.cn

JS:   const square = x => x * x;
来源：http://emy.shangyingyoupin.top

TS:   const square = (x: number): number => x * x;
来源：http://ngr.ivvv.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://knl.0kj1m.cn

Go:   sq := func(x int) int { return x * x }
来源：http://yqc.tian-w.cn

Ruby: square = ->(x) { x * x }
来源：http://lxe.zhixingplan.top

C#:   Func<int, int> square = x => x * x;
来源：http://nxy.ybcxt.top

[C07] 把函数作为参数传入
来源：http://rqs.nanxinkj.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bxy.daria6918.cn

PHP:  array_map("strtoupper", $arr);
来源：http://env.yj20258.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://equ.chenlongwang.top

TS:   arr.map(String)
来源：http://eah.fehbvm.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vlm.shanyushiyangkeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tum.birdmap.top

Ruby: arr.map(&:upcase)
来源：http://dgq.vehdjk.com

C#:   arr.Select(s => s.ToUpper())
来源：http://gwl.chenzaomai.com

[C08] 闭包
来源：http://tpu.zhongyouzk.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ohg.gotoacloud.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mdd.fzhhl.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vtt.pycfn.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zii.fktsv.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xqt.daxiang520.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jdv.yonumen.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zie.meibo888.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hlr.tianlin.xyz

[C09] 递归
来源：http://tjm.yj20258888.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qoe.hcnkem.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pcs.haohaochexian.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://clz.bbcook.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dqf.jinqigufen.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dua.gotoacloud.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dfc.jlsjyb.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hxv.jlsjyb.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yyx.xuetiantiany.cn

[C10] 变量作用域
来源：http://okj.ivvv.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dcc.sweek.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dxc.yvedp.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zxy.cucudq.cn

TS:   同 JS
来源：http://jts.fzhhl.top

Java: 方法内为块级作用域
来源：http://afu.jqgfzy.top

Go:   花括号块级作用域
来源：http://mgh.hfpthk.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://llb.xylfe.cn

C#:   块级作用域
来源：http://drx.sysykeji.top

[C11] 模块导入与导出
来源：http://uqp.316326.xyz

Py:   from module import func
来源：http://vkb.birdmap.top

PHP:  require "file.php";  或 use App\Service;
来源：http://osl.xuetiantiany.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://bkp.jlsjyb.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vqp.xuanzx.com

Java: import java.util.List;
来源：http://thd.zdbjq.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zut.hfpthk.cn

Ruby: require "json"; require_relative "./util"
来源：http://mzo.zhijiandao.cn

C#:   using System.Text;
来源：http://nwp.bbcook.cn

[C12] 立即执行函数 IIFE
来源：http://hol.ehwqpu.com

Py:   (lambda: print("run"))()
来源：http://mzz.jianghu66.top

PHP:  (function () { echo "run"; })();
来源：http://bxt.shzxlz.cn

JS:   (() => { console.log("run"); })();
来源：http://ajs.sjlbkw.cn

TS:   (() => { console.log("run"); })();
来源：http://rry.52xcode.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wea.hongshengwenyu.top

Go:   func() { fmt.Println("run") }()
来源：http://qyc.hammf.cn

Ruby: -> { puts "run" }.call
来源：http://tbu.jiagoushi.top

C#:   // 无 IIFE：用静态构造函数
来源：http://pun.zhijiandao.cn

[C13] 类型声明 / 类型注解
来源：http://ako.hesvh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sil.vehdjk.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kkg.tanke756.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kld.tanke756.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vzx.ydjk.org.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ybs.xuanzx.com

Go:   func add(a, b int) int
来源：http://gpx.zhixingplan.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qyn.chenjidiqi.icu

C#:   int Add(int a, int b) => a + b;
来源：http://mbb.hesvh.cn

[C14] 泛型函数
来源：http://tdp.jqgfzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ril.jinqigfzy.top

PHP:  // 无泛型
来源：http://ebd.snrcjt.cn

JS:   // 无泛型
来源：http://tbb.aibaodan.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ado.redwolf501.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://urq.zhiwuduotai.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mnv.ivvv.top

Ruby: # 无泛型
来源：http://bpc.zhoulong.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yuf.daria6918.cn

[C15] 解构 / 展开参数
来源：http://ype.ywan-chungtsiang.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mgd.fengsongda.top

PHP:  [$a, $b] = $pair;
来源：http://nde.snrcjt.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fzy.ivvv.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zvt.dashuyun.cn

Java: // 无解构
来源：http://elr.feifeiyinyue.top

Go:   // 无解构
来源：http://wvf.hongshengwenyu.top

Ruby: a, b = pair
来源：http://vcg.ppjwa.cn

C#:   var (a, b) = pair;
来源：http://zkv.zhongyouzk.top

[C16] 函数 / 方法重载
来源：http://dvj.sufxvd.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://doa.snrcjt.cn

PHP:  // 无重载
来源：http://cqz.fengsongda.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://pwa.zhoulong.xyz

TS:   // 用联合类型或重载签名声明
来源：http://sta.jyoumei.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://zjt.guowangkeji.top

Go:   // 无重载：用不同函数名
来源：http://wyz.cashguo.top

Ruby: # 无重载：靠动态参数
来源：http://tll.bbcook.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://axy.ywan-chungtsiang.top

================================================================================
来源：http://loe.meibo888.top

D. 数组 / 列表 / 集合
来源：http://moc.hywenlv.cn

================================================================================
来源：http://ows.redwolf501.top

[D01] 创建数组 / 列表
来源：http://ryz.chenjidiqi.icu

Py:   arr = [1, 2, 3];  empty = []
来源：http://xmd.dashuyun.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://akf.zhoulong.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xhf.yj20258.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://njk.yuxming.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yeb.hnxiangtu.top

Go:   arr := []int{1, 2, 3}
来源：http://eqn.c1oappe.top

Ruby: arr = [1, 2, 3]
来源：http://rjr.fzhhl.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jvr.hnxiangtu.top

[D02] 追加元素到末尾
来源：http://ccu.aibaodan.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qeq.yuanzhike.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yzt.meibo888.top

JS:   arr.push(4);
来源：http://bvj.gzhubu.top

TS:   arr.push(4);
来源：http://dab.cucudq.cn

Java: list.add(4);
来源：http://wvu.ybcxt.top

Go:   arr = append(arr, 4)
来源：http://amz.ctjpmb.com

Ruby: arr << 4; arr.push(5)
来源：http://lpe.ybcxt.top

C#:   list.Add(4);
来源：http://kxf.ehwqpu.com

[D03] 在指定位置插入元素
来源：http://jkh.hysaishi.cn

Py:   arr.insert(0, 0)
来源：http://fgb.yueranfly.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qge.jqgufenzy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xhz.zhoulong.xyz

TS:   arr.splice(0, 0, 0);
来源：http://eti.tian-w.cn

Java: list.add(0, 0);
来源：http://ljh.xingfuxueyuan.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://ijw.cucudq.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yvw.fanxiaobao.xyz

C#:   list.Insert(0, 0);
来源：http://wls.xinyue.icu

[D04] 删除元素
来源：http://xgm.jiagoushi.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vtw.jqgfzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vlz.havefunace.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://njy.quarkkingdee.top

TS:   arr.splice(0, 1);
来源：http://dhi.yongpay.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hwq.chenzaomai.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ioa.jlsjyb.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kbb.wangshuangyany.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rns.aibaodan.cn

[D05] 访问与修改元素
来源：http://fze.hfpthk.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pfm.zhaomingkeji.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mxc.wangshuangyany.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xyn.zhijiandao.cn

TS:   arr[0]; arr.at(-1);
来源：http://oiy.cashguo.top

Java: list.get(0); list.set(0, 9);
来源：http://tic.havefunace.top

Go:   arr[0]; arr[0] = 9
来源：http://sqh.chenjidiqi.icu

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tva.cdnleiting.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uuz.vqdsnc.cn

[D06] 数组长度
来源：http://dsb.cucudq.cn

Py:   len(arr)
来源：http://fkh.hywenlv.cn

PHP:  count($arr);
来源：http://ezr.yangfankeji.com

JS:   arr.length
来源：http://kzq.fanxiaobao.xyz

TS:   arr.length
来源：http://sju.hammf.cn

Java: list.size();
来源：http://toz.yueranfly.top

Go:   len(arr)
来源：http://wov.ybcxt.top

Ruby: arr.length; arr.size
来源：http://dbp.zdbjq.cn

C#:   list.Count;
来源：http://bvq.chenjidiqi.icu

[D07] 切片 / 取子数组
来源：http://uww.hammf.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vrt.meibo888.top

PHP:  array_slice($arr, 1, 3);
来源：http://hui.wangdashe.top

JS:   arr.slice(1, 4);
来源：http://luk.gaohongyu789.top

TS:   arr.slice(1, 4);
来源：http://ouk.vqdsnc.cn

Java: list.subList(1, 4);
来源：http://ofa.ywan-chungtsiang.top

Go:   arr[1:4]
来源：http://uup.yfazqb.com

Ruby: arr[1, 3]
来源：http://dqz.cucudq.cn

C#:   list.GetRange(1, 3);
来源：http://stn.shanyushiyangtech.top

[D08] 合并两个数组
来源：http://yjf.chenjidiqi.icu

Py:   a + b;  a.extend(b)
来源：http://zde.yj202588.top

PHP:  array_merge($a, $b);
来源：http://feq.wangshuangyany.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kwu.birdmap.top

TS:   [...a, ...b];
来源：http://meu.nwbrower.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mbt.jinyuanbaomall.cn

Go:   append(a, b...)
来源：http://qvc.ppjwa.cn

Ruby: a + b;  a.concat(b)
来源：http://vqt.jinghuilouyu.cn

C#:   a.Concat(b).ToList()
来源：http://qml.cdnleiting.top

[D09] 排序（升序）
来源：http://kmx.chenzaomai.com

Py:   sorted(arr);  arr.sort()
来源：http://nes.feifeiyinyue.top

PHP:  sort($arr);
来源：http://xad.yuanzhike.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://flq.zdbjq.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xrg.svipenyu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://dwt.nanxinkj.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nnb.hongshengwenyu.top

Ruby: arr.sort
来源：http://lnx.zhongyouzk.top

C#:   list.Sort();
来源：http://wpy.daria6918.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://hdu.yonumen.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uzt.hysaishi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wsm.yangfankeji.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hwv.hnxiangtu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bxr.bbcook.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yzo.ydzc1.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pfc.yj20258.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://swt.guannengcc.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ofz.c1oappe.top

[D11] 反转数组
来源：http://mtd.hysaishi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://muw.snrcjt.cn

PHP:  array_reverse($arr);
来源：http://knq.zhongyouzk.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vvw.ywan-chungtsiang.top

TS:   [...arr].reverse();
来源：http://kkr.hnqzz.top

Java: Collections.reverse(list);
来源：http://rcf.havefunace.top

Go:   slices.Reverse(arr)
来源：http://vxw.zhijiandao.cn

Ruby: arr.reverse
来源：http://dtc.wangshuangyany.cn

C#:   list.Reverse();
来源：http://spx.pycfn.com

[D12] 查找元素下标
来源：http://rmt.vqdsnc.cn

Py:   arr.index(x);  x in arr
来源：http://apg.sxryk.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bgi.nwbrower.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pgx.kuanghao11.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qol.epnwcf.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://unc.yuanzhike.top

Go:   slices.Index(arr, x)
来源：http://sdp.yfazqb.com

Ruby: arr.index(x)
来源：http://rhv.9152youxi.cn

C#:   list.IndexOf(x);
来源：http://jcs.kuanghao11.cn

[D13] 过滤（保留满足条件的）
来源：http://chj.jqgfzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vfq.iojbl.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tos.shzxlz.cn

JS:   arr.filter(x => x > 3)
来源：http://icq.yonumen.top

TS:   arr.filter(x => x > 3)
来源：http://ztm.yueranfly.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ziz.ehwqpu.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cqx.zhengqikj.top

Ruby: arr.select { |x| x > 3 }
来源：http://jqd.fehbvm.com

C#:   list.Where(x => x > 3).ToList()
来源：http://wlq.jyoumei.cn

[D14] 映射转换（每个元素变形）
来源：http://rwu.zhaomingkeji.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://eyl.yuxming.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cir.52xcode.cn

JS:   arr.map(x => x * 2)
来源：http://nip.gotoacloud.top

TS:   arr.map(x => x * 2)
来源：http://eif.havefunace.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://xuw.zycfv.cn

Go:   // 手写循环
来源：http://hdz.yonumen.top

Ruby: arr.map { |x| x * 2 }
来源：http://uwf.chenlongwang.top

C#:   list.Select(x => x * 2).ToList()
来源：http://seu.mhx1999.top

[D15] 去重
来源：http://wpi.xingfuxueyuan.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cpl.daxiang520.top

PHP:  array_unique($arr);
来源：http://juc.shanyushiyangtech.top

JS:   [...new Set(arr)]
来源：http://bke.aibaodan.cn

TS:   [...new Set(arr)]
来源：http://gzf.zhixingplan.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yei.52xcode.cn

Go:   // 用 map[T]struct{} 手写
来源：http://pnn.sweek.top

Ruby: arr.uniq
来源：http://xdr.ivvv.top

C#:   list.Distinct().ToList()
来源：http://jmg.xinyue.icu

[D16] 求和与平均值
来源：http://xwl.yj202588.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xok.shuidangran.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ybj.daria6918.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gph.yuxming.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lxr.meibo888.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pmy.zhaomingkeji.xyz

Go:   // 手写循环累加
来源：http://fvx.haohaochexian.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fhk.gaohongyu789.top

C#:   list.Sum();  list.Average()
来源：http://pcb.wangdashe.top

[D17] 最大值与最小值
来源：http://xej.cdnleiting.top

Py:   max(arr);  min(arr)
来源：http://yhv.zdbjq.cn

PHP:  max($arr);  min($arr);
来源：http://wff.zdqjudy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wdo.shanyushiyangtech.top

TS:   Math.max(...arr);
来源：http://box.chenzaomai.com

Java: Collections.max(list);  Collections.min(list);
来源：http://ani.yonumen.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ebe.zycfv.cn

Ruby: arr.max;  arr.min
来源：http://cie.chenlongwang.top

C#:   list.Max();  list.Min()
来源：http://dxn.redwolf501.top

[D18] 扁平化嵌套数组
来源：http://jwk.gotoacloud.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jui.yongpay.top

PHP:  array_merge(...$nested);
来源：http://gxi.c1oappe.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fyd.gotoacloud.top

TS:   nested.flat();
来源：http://kdg.haohaochexian.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lsx.zhaomingkeji.xyz

Go:   // 手写双层循环
来源：http://dmg.hcnkem.com

Ruby: nested.flatten
来源：http://xhu.nwbrower.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://gmg.meibo888.top

[D19] 按字段分组
来源：http://vlu.guowangkeji.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xiy.zhengqikj.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pmq.hnxiangtu.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hbo.xylfe.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://htx.fzhhl.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://eyb.52xcode.cn

Go:   // 手写 map[string][]T
来源：http://vpn.yangfankeji.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://pxn.zhixingplan.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kpo.ywan-chungtsiang.top

[D20] 统计每个元素出现次数
来源：http://nhg.fktsv.cn

Py:   Counter(arr)
来源：http://nmr.tarul.cn

PHP:  array_count_values($arr);
来源：http://lko.zdqjudy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tpo.ywan-chungtsiang.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dqk.jyoumei.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qlp.havefunace.top

Go:   // 手写 map[T]int
来源：http://qdd.xingfuxueyuan.xyz

Ruby: arr.tally
来源：http://dnn.kuanghao11.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xxj.zhongyouzk.top

[D21] 判断是否包含某元素
来源：http://ccs.andypj.xyz

Py:   x in arr
来源：http://xad.snrcjt.cn

PHP:  in_array($x, $arr, true);
来源：http://fsh.jinyuanbaomall.cn

JS:   arr.includes(x)
来源：http://lul.0kj1m.cn

TS:   arr.includes(x)
来源：http://syg.ywan-chungtsiang.top

Java: list.contains(x)
来源：http://gvy.shzxlz.cn

Go:   slices.Contains(arr, x)
来源：http://ndw.zhaomingkeji.xyz

Ruby: arr.include?(x)
来源：http://irr.vqdsnc.cn

C#:   list.Contains(x)
来源：http://yza.xylfe.cn

[D22] 复制数组（避免共享引用）
来源：http://yom.hesvh.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wmc.xylfe.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hzb.xziqi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://itk.sysykeji.top

TS:   [...arr];
来源：http://afa.ivvv.top

Java: new ArrayList<>(list);
来源：http://jwj.hcnkem.com

Go:   copied := append([]int(nil), arr...)
来源：http://wps.hfpthk.cn

Ruby: arr.dup;  arr.clone
来源：http://zbw.kuanghao11.cn

C#:   new List<int>(list);
来源：http://gon.wangshuangyany.cn


<!-- 参考信息 -->