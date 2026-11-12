代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://hcw.0kj1m.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vmb.cashguo.top

Go:   sq := func(x int) int { return x * x }
来源：http://kvy.feifeiyinyue.top

Ruby: square = ->(x) { x * x }
来源：http://lot.gogol.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://die.yangfankeji.com

[C07] 把函数作为参数传入
来源：http://rzk.hnxiangtu.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rjj.fktsv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ams.andypj.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ztk.xingfuxueyuan.xyz

TS:   arr.map(String)
来源：http://ohy.uphjek.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uny.cqqwz.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wui.sweek.top

Ruby: arr.map(&:upcase)
来源：http://lgl.fanxiaobao.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://jls.yuanzhike.top

[C08] 闭包
来源：http://pxi.pengpengdd.cyou

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xwf.nanxinkj.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://npd.hfpthk.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mre.ydzc1.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://imr.smart0.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gkd.quarkkingdee.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bvw.tianlin.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qse.aizwys.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yun.quarkkingdee.top

[C09] 递归
来源：http://rhs.jiagoushi.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nez.jyoumei.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ruv.zhijiandao.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://olk.zhixingplan.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vsd.shanyushiyangtech.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://czp.sjlbkw.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uho.zycfv.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uhb.ydjk.org.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kis.fzhhl.top

[C10] 变量作用域
来源：http://fzu.mhx1999.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://efe.jianghu66.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fzt.andypj.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://scz.yuxming.cn

TS:   同 JS
来源：http://zgp.ivvv.top

Java: 方法内为块级作用域
来源：http://vhb.shuidangran.top

Go:   花括号块级作用域
来源：http://pvm.dianchejie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://iwx.fzhhl.top

C#:   块级作用域
来源：http://tmn.yvedp.cn

[C11] 模块导入与导出
来源：http://uez.zhoulong.xyz

Py:   from module import func
来源：http://xvq.hnqzz.top

PHP:  require "file.php";  或 use App\Service;
来源：http://cwh.shuidangran.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://dxh.nwbrower.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://duk.ydzc1.top

Java: import java.util.List;
来源：http://yky.sjlbkw.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wji.guowangkeji.top

Ruby: require "json"; require_relative "./util"
来源：http://hrj.ybcxt.top

C#:   using System.Text;
来源：http://cvq.chenzaomai.com

[C12] 立即执行函数 IIFE
来源：http://dbi.yvedp.cn

Py:   (lambda: print("run"))()
来源：http://mhr.hfpthk.cn

PHP:  (function () { echo "run"; })();
来源：http://gil.jianghu66.top

JS:   (() => { console.log("run"); })();
来源：http://dqf.shuidangran.top

TS:   (() => { console.log("run"); })();
来源：http://vbz.yueranfly.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mcf.52xcode.cn

Go:   func() { fmt.Println("run") }()
来源：http://sxi.zhoulong.xyz

Ruby: -> { puts "run" }.call
来源：http://wup.aibaodan.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://sjc.chenzaomai.com

[C13] 类型声明 / 类型注解
来源：http://bmm.jinghuilouyu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dym.sweek.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uhb.yangfankeji.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ntm.hongshengwenyu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://epx.fehbvm.com

Java: int add(int a, int b) { return a + b; }
来源：http://yps.xingfuxueyuan.xyz

Go:   func add(a, b int) int
来源：http://nde.sweek.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lto.shuidangran.top

C#:   int Add(int a, int b) => a + b;
来源：http://rhi.zdqjudy.top

[C14] 泛型函数
来源：http://glv.tianlin.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kap.vqdsnc.cn

PHP:  // 无泛型
来源：http://uxv.birdmap.top

JS:   // 无泛型
来源：http://ksw.zhixingplan.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zcw.yj20258888.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tmp.vehdjk.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://awm.hammf.cn

Ruby: # 无泛型
来源：http://huq.hcnkem.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bbz.epnwcf.com

[C15] 解构 / 展开参数
来源：http://zta.c1oappe.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vax.fanxiaobao.xyz

PHP:  [$a, $b] = $pair;
来源：http://bfm.jinghuilouyu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rra.ydjk.org.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tkk.shanyushiyangtech.top

Java: // 无解构
来源：http://gey.jqgfzy.top

Go:   // 无解构
来源：http://qdg.quarkkingdee.top

Ruby: a, b = pair
来源：http://guv.snrcjt.cn

C#:   var (a, b) = pair;
来源：http://nqq.ydzc1.top

[C16] 函数 / 方法重载
来源：http://qhb.yuanzhike.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://flb.52xcode.cn

PHP:  // 无重载
来源：http://ojs.ydjk.org.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bkn.hammf.cn

TS:   // 用联合类型或重载签名声明
来源：http://fcr.tarul.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qqp.zdbjq.cn

Go:   // 无重载：用不同函数名
来源：http://sfe.gotoacloud.top

Ruby: # 无重载：靠动态参数
来源：http://hht.chenzaomai.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://one.tarul.cn

================================================================================
来源：http://twp.fengsongda.top

D. 数组 / 列表 / 集合
来源：http://qld.ctjpmb.com

================================================================================
来源：http://dlg.hywenlv.cn

[D01] 创建数组 / 列表
来源：http://lou.hywenlv.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://uyl.aibaodan.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tir.yueranfly.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fwc.xziqi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://mkc.ehwqpu.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gvn.zhiwuduotai.top

Go:   arr := []int{1, 2, 3}
来源：http://jyk.xuanzx.com

Ruby: arr = [1, 2, 3]
来源：http://dpj.guowangkeji.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://amp.xingfuxueyuan.xyz

[D02] 追加元素到末尾
来源：http://pck.zdbjq.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ofw.tianlin.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nqd.sufxvd.cn

JS:   arr.push(4);
来源：http://kpo.yongpay.top

TS:   arr.push(4);
来源：http://wio.jinghuilouyu.cn

Java: list.add(4);
来源：http://uro.chenlongwang.top

Go:   arr = append(arr, 4)
来源：http://tmq.gaohongyu789.top

Ruby: arr << 4; arr.push(5)
来源：http://lec.pycfn.com

C#:   list.Add(4);
来源：http://coa.feifeiyinyue.top

[D03] 在指定位置插入元素
来源：http://zfw.sysykeji.top

Py:   arr.insert(0, 0)
来源：http://mff.jqgfzy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yyv.daxiang520.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://idg.zdbjq.cn

TS:   arr.splice(0, 0, 0);
来源：http://fhw.jyoumei.cn

Java: list.add(0, 0);
来源：http://fxm.hywenlv.cn

Go:   arr = append([]int{0}, arr...)
来源：http://dhb.cdnleiting.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vry.yanxiufei.cn

C#:   list.Insert(0, 0);
来源：http://nxg.kuanghao11.cn

[D04] 删除元素
来源：http://uph.cqqwz.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dvi.nanxinkj.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jkn.tianlin.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vbj.hesvh.cn

TS:   arr.splice(0, 1);
来源：http://zps.bjfxy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fgi.ctjpmb.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ter.vehdjk.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lzy.daxiang520.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mgj.0kj1m.cn

[D05] 访问与修改元素
来源：http://yrz.yueranfly.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pfa.yanxiufei.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ldo.zdqjudy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ijx.feifeiyinyue.top

TS:   arr[0]; arr.at(-1);
来源：http://dqw.sweek.top

Java: list.get(0); list.set(0, 9);
来源：http://iqw.ybcxt.top

Go:   arr[0]; arr[0] = 9
来源：http://xnw.yangfankeji.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://idy.dianchejie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://oyp.wangshuangyany.cn

[D06] 数组长度
来源：http://nrq.hfpthk.cn

Py:   len(arr)
来源：http://aqf.cdnleiting.top

PHP:  count($arr);
来源：http://ssd.mhx1999.top

JS:   arr.length
来源：http://vqd.chenzaomai.com

TS:   arr.length
来源：http://kvv.mhx1999.top

Java: list.size();
来源：http://xhm.ehwqpu.com

Go:   len(arr)
来源：http://xuc.c1oappe.top

Ruby: arr.length; arr.size
来源：http://sgt.hfpthk.cn

C#:   list.Count;
来源：http://ubq.xingfuxueyuan.xyz

[D07] 切片 / 取子数组
来源：http://wpm.ctjpmb.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cbi.yvedp.cn

PHP:  array_slice($arr, 1, 3);
来源：http://oty.hongshengwenyu.top

JS:   arr.slice(1, 4);
来源：http://kkz.dashuyun.cn

TS:   arr.slice(1, 4);
来源：http://nyt.yvedp.cn

Java: list.subList(1, 4);
来源：http://ttt.redwolf501.top

Go:   arr[1:4]
来源：http://bni.zhengqikj.top

Ruby: arr[1, 3]
来源：http://jfb.yangfankeji.com

C#:   list.GetRange(1, 3);
来源：http://drv.zdbjq.cn

[D08] 合并两个数组
来源：http://pas.9152youxi.cn

Py:   a + b;  a.extend(b)
来源：http://epj.cdnleiting.top

PHP:  array_merge($a, $b);
来源：http://lpz.yangfankeji.com

JS:   [...a, ...b];  a.concat(b);
来源：http://eur.tianlin.xyz

TS:   [...a, ...b];
来源：http://sqx.yonumen.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zud.jlsjyb.cn

Go:   append(a, b...)
来源：http://xsr.yangfankeji.com

Ruby: a + b;  a.concat(b)
来源：http://yid.hfpthk.cn

C#:   a.Concat(b).ToList()
来源：http://rjp.pengpengdd.cyou

[D09] 排序（升序）
来源：http://vkh.iojbl.cn

Py:   sorted(arr);  arr.sort()
来源：http://uwh.haohaochexian.top

PHP:  sort($arr);
来源：http://dpl.dashuyun.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pfi.jlsjyb.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tbt.chenlongwang.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ouz.gzhubu.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ztp.zhaomingkeji.xyz

Ruby: arr.sort
来源：http://vxt.daria6918.cn

C#:   list.Sort();
来源：http://bql.ydzc1.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://tgs.ywan-chungtsiang.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uzv.xingfuxueyuan.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ffm.birdmap.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zcs.chenjidiqi.icu

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pjj.haohaochexian.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gjh.yvedp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bvb.cucudq.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sab.jqgufenzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wjk.zdbjq.cn

[D11] 反转数组
来源：http://qbj.zdbjq.cn

Py:   arr[::-1];  arr.reverse()
来源：http://cdq.tian-w.cn

PHP:  array_reverse($arr);
来源：http://slv.shanyushiyangkeji.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://eep.hnqzz.top

TS:   [...arr].reverse();
来源：http://cgg.sxryk.cn

Java: Collections.reverse(list);
来源：http://ims.zhijiandao.cn

Go:   slices.Reverse(arr)
来源：http://umu.yanxiufei.cn

Ruby: arr.reverse
来源：http://ndf.sweek.top

C#:   list.Reverse();
来源：http://org.zdbjq.cn

[D12] 查找元素下标
来源：http://rfn.fengsongda.top

Py:   arr.index(x);  x in arr
来源：http://erv.smart0.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://del.zhongyouzk.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ceo.fehbvm.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eke.xuanzx.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nyx.quarkkingdee.top

Go:   slices.Index(arr, x)
来源：http://jtt.fzhhl.top

Ruby: arr.index(x)
来源：http://wro.iojbl.cn

C#:   list.IndexOf(x);
来源：http://pcs.52xcode.cn

[D13] 过滤（保留满足条件的）
来源：http://ozh.yuanzhike.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://atz.ydzc1.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://uoz.feifeiyinyue.top

JS:   arr.filter(x => x > 3)
来源：http://vrz.316326.xyz

TS:   arr.filter(x => x > 3)
来源：http://pgp.gogol.net.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nrd.mhx1999.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://szc.fzhhl.top

Ruby: arr.select { |x| x > 3 }
来源：http://njo.fktsv.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://dyv.tianlin.xyz

[D14] 映射转换（每个元素变形）
来源：http://fgx.52xcode.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qti.sysykeji.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://oqh.c1oappe.top

JS:   arr.map(x => x * 2)
来源：http://dsj.ehwqpu.com

TS:   arr.map(x => x * 2)
来源：http://jrv.pengpengdd.cyou

Java: list.stream().map(x -> x * 2).toList()
来源：http://vxu.sxryk.cn

Go:   // 手写循环
来源：http://ols.zhaomingkeji.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://rfg.zhoulong.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://ecs.havefunace.top

[D15] 去重
来源：http://osw.jqgfzy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://szn.ehwqpu.com

PHP:  array_unique($arr);
来源：http://ghx.tanke756.top

JS:   [...new Set(arr)]
来源：http://huk.jqgufenzy.top

TS:   [...new Set(arr)]
来源：http://rwj.zycfv.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tal.jlsjyb.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hdu.chenzaomai.com

Ruby: arr.uniq
来源：http://aoz.tarul.cn

C#:   list.Distinct().ToList()
来源：http://fgz.uphjek.com

[D16] 求和与平均值
来源：http://ggg.iojbl.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vrh.mhx1999.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tdx.shangyingyoupin.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kdp.meibo888.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vxl.nanxuanxn.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://igl.jinqigfzy.top

Go:   // 手写循环累加
来源：http://asb.chenzaomai.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sqv.redwolf501.top

C#:   list.Sum();  list.Average()
来源：http://niw.chenzaomai.com

[D17] 最大值与最小值
来源：http://ips.yueranfly.top

Py:   max(arr);  min(arr)
来源：http://vus.jlsjyb.cn

PHP:  max($arr);  min($arr);
来源：http://biz.zhijiandao.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://exv.cucudq.cn

TS:   Math.max(...arr);
来源：http://lmw.hnqzz.top

Java: Collections.max(list);  Collections.min(list);
来源：http://sdl.bjfxy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dtw.shangyingyoupin.top

Ruby: arr.max;  arr.min
来源：http://oku.cashguo.top

C#:   list.Max();  list.Min()
来源：http://jdy.zhaomingkeji.xyz

[D18] 扁平化嵌套数组
来源：http://ypv.fanxiaobao.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dgn.kuanghao11.cn

PHP:  array_merge(...$nested);
来源：http://nfn.tian-w.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dtv.chenzaomai.com

TS:   nested.flat();
来源：http://obl.svipenyu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wug.sufxvd.cn

Go:   // 手写双层循环
来源：http://bzu.birdmap.top

Ruby: nested.flatten
来源：http://dyw.guannengcc.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://zdr.quarkkingdee.top

[D19] 按字段分组
来源：http://arj.bbcook.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lnd.nwbrower.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wsg.cqqwz.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ote.0kj1m.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ixv.0kj1m.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nwd.sufxvd.cn

Go:   // 手写 map[string][]T
来源：http://kwt.sjlbkw.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://seb.zycfv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://afo.yueranfly.top

[D20] 统计每个元素出现次数
来源：http://gre.svipenyu.cn

Py:   Counter(arr)
来源：http://oav.hfpthk.cn

PHP:  array_count_values($arr);
来源：http://qfv.xylfe.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tlq.hfpthk.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zyv.hnxiangtu.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dlv.chenlongwang.top

Go:   // 手写 map[T]int
来源：http://ruk.ywan-chungtsiang.top

Ruby: arr.tally
来源：http://vee.birdmap.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rpj.sysykeji.top

[D21] 判断是否包含某元素
来源：http://ncj.zycfv.cn

Py:   x in arr
来源：http://vef.ehwqpu.com

PHP:  in_array($x, $arr, true);
来源：http://hhm.kuanghao11.cn

JS:   arr.includes(x)
来源：http://rkv.jiagoushi.top

TS:   arr.includes(x)
来源：http://hol.jqgfzy.top

Java: list.contains(x)
来源：http://kdv.jinghuilouyu.cn

Go:   slices.Contains(arr, x)
来源：http://ela.pycfn.com

Ruby: arr.include?(x)
来源：http://hac.yuxming.cn

C#:   list.Contains(x)
来源：http://abd.yueranfly.top

[D22] 复制数组（避免共享引用）
来源：http://ixz.jiagoushi.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://etv.kuanghao11.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wvm.hfpthk.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kbv.cdnleiting.top

TS:   [...arr];
来源：http://bbg.pengpengdd.cyou

Java: new ArrayList<>(list);
来源：http://vcp.daria6918.cn

Go:   copied := append([]int(nil), arr...)
来源：http://dhe.hysaishi.cn

Ruby: arr.dup;  arr.clone
来源：http://nyv.guannengcc.top

C#:   new List<int>(list);
来源：http://mao.chenjidiqi.icu

[D23] reduce 累积计算
来源：http://pah.daxiang520.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://uap.sufxvd.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pvj.pengpengdd.cyou

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bum.quarkkingdee.top


<!-- 参考信息 -->