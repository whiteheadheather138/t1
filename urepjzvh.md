代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://pts.cashguo.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wbo.jinqigfzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://joz.sxryk.cn

Ruby: square = ->(x) { x * x }
来源：http://ubn.vqdsnc.cn

C#:   Func<int, int> square = x => x * x;
来源：http://blu.havefunace.top

[C07] 把函数作为参数传入
来源：http://goz.jinqigufen.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xkh.mhx1999.top

PHP:  array_map("strtoupper", $arr);
来源：http://zha.zhengqikj.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tak.bbcook.cn

TS:   arr.map(String)
来源：http://ehj.xuetiantiany.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mzb.jinqigfzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nuz.iojbl.cn

Ruby: arr.map(&:upcase)
来源：http://bbw.iojbl.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://chx.chenlongwang.top

[C08] 闭包
来源：http://pts.hfpthk.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fgi.yanxiufei.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ksj.316326.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ixv.jlsjyb.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hgi.ehwqpu.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://chi.xuanzx.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tzt.sufxvd.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qmu.kuanghao11.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bvl.wangdashe.top

[C09] 递归
来源：http://dxi.xinyue.icu

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cml.yanxiufei.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tty.zhixingplan.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://min.cqqwz.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vpw.tian-w.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vpj.xuetiantiany.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jkh.pycfn.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lbw.ywan-chungtsiang.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cgd.yuanzhike.top

[C10] 变量作用域
来源：http://awa.daxiang520.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wma.sweek.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qnp.bbcook.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jha.sxryk.cn

TS:   同 JS
来源：http://tyt.yanxiufei.cn

Java: 方法内为块级作用域
来源：http://tlx.cqqwz.cn

Go:   花括号块级作用域
来源：http://xre.yanxiufei.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yku.hcnkem.com

C#:   块级作用域
来源：http://vlq.zhixingplan.top

[C11] 模块导入与导出
来源：http://gva.quarkkingdee.top

Py:   from module import func
来源：http://ucd.hesvh.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ltu.haohaochexian.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://vmv.sufxvd.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qyr.jinqigufen.top

Java: import java.util.List;
来源：http://cro.zhongyouzk.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jvr.ywan-chungtsiang.top

Ruby: require "json"; require_relative "./util"
来源：http://wfy.ivvv.top

C#:   using System.Text;
来源：http://zin.jyoumei.cn

[C12] 立即执行函数 IIFE
来源：http://biy.xinyue.icu

Py:   (lambda: print("run"))()
来源：http://rpm.zhixingplan.top

PHP:  (function () { echo "run"; })();
来源：http://lwv.uphjek.com

JS:   (() => { console.log("run"); })();
来源：http://vxx.aibaodan.cn

TS:   (() => { console.log("run"); })();
来源：http://mqv.quarkkingdee.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://flz.cheryme.top

Go:   func() { fmt.Println("run") }()
来源：http://jlm.sufxvd.cn

Ruby: -> { puts "run" }.call
来源：http://lmn.svipenyu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xsu.xylfe.cn

[C13] 类型声明 / 类型注解
来源：http://ihq.yueranfly.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yas.tarul.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uqe.xziqi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zqs.yj20258.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zyd.hywenlv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ivl.sysykeji.top

Go:   func add(a, b int) int
来源：http://tmz.feifeiyinyue.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kme.yj20258.top

C#:   int Add(int a, int b) => a + b;
来源：http://bmz.ppjwa.cn

[C14] 泛型函数
来源：http://dzh.shzxlz.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mbw.yuxming.cn

PHP:  // 无泛型
来源：http://qnz.iojbl.cn

JS:   // 无泛型
来源：http://ixv.havefunace.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nxk.shuidangran.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nce.xinyue.icu

Go:   func First[T any](items []T) T { return items[0] }
来源：http://njw.shanyushiyangtech.top

Ruby: # 无泛型
来源：http://kzx.wangdashe.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wxg.chenzaomai.com

[C15] 解构 / 展开参数
来源：http://lqh.vqdsnc.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mvi.fehbvm.com

PHP:  [$a, $b] = $pair;
来源：http://dab.sjlbkw.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qws.daxiang520.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hbj.quarkkingdee.top

Java: // 无解构
来源：http://nlu.ppjwa.cn

Go:   // 无解构
来源：http://ozk.pycfn.com

Ruby: a, b = pair
来源：http://qjk.gotoacloud.top

C#:   var (a, b) = pair;
来源：http://hrm.9152youxi.cn

[C16] 函数 / 方法重载
来源：http://dxx.9152youxi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mop.yueranfly.top

PHP:  // 无重载
来源：http://crt.gotoacloud.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://uya.sweek.top

TS:   // 用联合类型或重载签名声明
来源：http://tgj.epnwcf.com

Java: void f(int a) {}  void f(String a) {}
来源：http://dcs.wangdashe.top

Go:   // 无重载：用不同函数名
来源：http://zff.nwbrower.top

Ruby: # 无重载：靠动态参数
来源：http://tvy.sufxvd.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://vfw.yongpay.top

================================================================================
来源：http://toy.jlsjyb.cn

D. 数组 / 列表 / 集合
来源：http://rnc.zdqjudy.top

================================================================================
来源：http://fmt.zhongyouzk.top

[D01] 创建数组 / 列表
来源：http://ppc.daria6918.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://gck.aibaodan.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dxq.fehbvm.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pbg.cheryme.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://vss.xuanzx.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://htp.yj20258888.top

Go:   arr := []int{1, 2, 3}
来源：http://mhs.yfazqb.com

Ruby: arr = [1, 2, 3]
来源：http://jbh.zhengqikj.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dqn.epnwcf.com

[D02] 追加元素到末尾
来源：http://tga.daria6918.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hsc.guowangkeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dnl.quarkkingdee.top

JS:   arr.push(4);
来源：http://eaa.cashguo.top

TS:   arr.push(4);
来源：http://gnx.yonumen.top

Java: list.add(4);
来源：http://rfg.zdqjudy.top

Go:   arr = append(arr, 4)
来源：http://frn.c1oappe.top

Ruby: arr << 4; arr.push(5)
来源：http://kco.cqqwz.cn

C#:   list.Add(4);
来源：http://eds.bjfxy.top

[D03] 在指定位置插入元素
来源：http://fuw.hfpthk.cn

Py:   arr.insert(0, 0)
来源：http://nmj.cashguo.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://trm.ybcxt.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yol.bbcook.cn

TS:   arr.splice(0, 0, 0);
来源：http://okv.hywenlv.cn

Java: list.add(0, 0);
来源：http://cmv.dianchejie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://sjm.shangyingyoupin.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vua.zdqjudy.top

C#:   list.Insert(0, 0);
来源：http://txv.ybcxt.top

[D04] 删除元素
来源：http://sau.daria6918.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lrv.xylfe.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zhd.tianlin.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kds.chenjidiqi.icu

TS:   arr.splice(0, 1);
来源：http://njz.haohaochexian.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pat.epnwcf.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://csy.tanke756.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hfj.iojbl.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://iwh.xuanzx.com

[D05] 访问与修改元素
来源：http://eab.shzxlz.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wlp.yanxiufei.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zol.andypj.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dac.316326.xyz

TS:   arr[0]; arr.at(-1);
来源：http://jzd.cdnleiting.top

Java: list.get(0); list.set(0, 9);
来源：http://lou.bbcook.cn

Go:   arr[0]; arr[0] = 9
来源：http://hxz.hysaishi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wfb.shzxlz.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://swn.tanke756.top

[D06] 数组长度
来源：http://lgo.hysaishi.cn

Py:   len(arr)
来源：http://byr.yfazqb.com

PHP:  count($arr);
来源：http://zlr.yj20258.top

JS:   arr.length
来源：http://mop.uphjek.com

TS:   arr.length
来源：http://bpj.hnxiangtu.top

Java: list.size();
来源：http://hxq.yj20258.top

Go:   len(arr)
来源：http://hjb.hesvh.cn

Ruby: arr.length; arr.size
来源：http://tkp.cqqwz.cn

C#:   list.Count;
来源：http://jcd.cheryme.top

[D07] 切片 / 取子数组
来源：http://qut.hongshengwenyu.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kgt.hnxiangtu.top

PHP:  array_slice($arr, 1, 3);
来源：http://xng.daria6918.cn

JS:   arr.slice(1, 4);
来源：http://mti.hongshengwenyu.top

TS:   arr.slice(1, 4);
来源：http://dit.yangfankeji.com

Java: list.subList(1, 4);
来源：http://qqe.hongshengwenyu.top

Go:   arr[1:4]
来源：http://ifk.fanxiaobao.xyz

Ruby: arr[1, 3]
来源：http://onl.vqdsnc.cn

C#:   list.GetRange(1, 3);
来源：http://apz.chenlongwang.top

[D08] 合并两个数组
来源：http://gaw.jqgfzy.top

Py:   a + b;  a.extend(b)
来源：http://brb.mhx1999.top

PHP:  array_merge($a, $b);
来源：http://kxp.haohaochexian.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ujq.ydzc1.top

TS:   [...a, ...b];
来源：http://thu.pycfn.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tgf.zycfv.cn

Go:   append(a, b...)
来源：http://bgv.bjfxy.top

Ruby: a + b;  a.concat(b)
来源：http://yvs.wangdashe.top

C#:   a.Concat(b).ToList()
来源：http://cnh.jlsjyb.cn

[D09] 排序（升序）
来源：http://dyk.fzhhl.top

Py:   sorted(arr);  arr.sort()
来源：http://umz.chenzaomai.com

PHP:  sort($arr);
来源：http://ftj.andypj.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kkc.cashguo.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://gmn.ivvv.top

Java: Collections.sort(list);  list.sort(null);
来源：http://epn.hammf.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://upf.fengsongda.top

Ruby: arr.sort
来源：http://ftq.tian-w.cn

C#:   list.Sort();
来源：http://pvk.gotoacloud.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://fpe.gogol.net.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xrj.xziqi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://amm.yvedp.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://puh.tarul.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tht.yonumen.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://epk.nanxinkj.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sbf.hesvh.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fxr.mhx1999.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xbm.shanyushiyangkeji.top

[D11] 反转数组
来源：http://xep.vehdjk.com

Py:   arr[::-1];  arr.reverse()
来源：http://flo.tian-w.cn

PHP:  array_reverse($arr);
来源：http://zlm.guowangkeji.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gck.zhaomingkeji.xyz

TS:   [...arr].reverse();
来源：http://bij.ppjwa.cn

Java: Collections.reverse(list);
来源：http://vnc.hcnkem.com

Go:   slices.Reverse(arr)
来源：http://ivd.sweek.top

Ruby: arr.reverse
来源：http://lnw.yonumen.top

C#:   list.Reverse();
来源：http://gyb.mhx1999.top

[D12] 查找元素下标
来源：http://otj.yangfankeji.com

Py:   arr.index(x);  x in arr
来源：http://fnp.fktsv.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qxp.cashguo.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jea.gaohongyu789.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wyf.zhengqikj.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wjj.sxryk.cn

Go:   slices.Index(arr, x)
来源：http://stb.vqdsnc.cn

Ruby: arr.index(x)
来源：http://xvq.tianlin.xyz

C#:   list.IndexOf(x);
来源：http://nrp.tanke756.top

[D13] 过滤（保留满足条件的）
来源：http://nvm.haohaochexian.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ajf.fengsongda.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ioe.yangfankeji.com

JS:   arr.filter(x => x > 3)
来源：http://jzz.52xcode.cn

TS:   arr.filter(x => x > 3)
来源：http://tqt.zhixingplan.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mlg.yanxiufei.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://klr.smart0.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://grn.yj202588.top

C#:   list.Where(x => x > 3).ToList()
来源：http://atg.fengsongda.top

[D14] 映射转换（每个元素变形）
来源：http://nfj.sxryk.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kwc.fengsongda.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lhw.xingfuxueyuan.xyz

JS:   arr.map(x => x * 2)
来源：http://gru.c1oappe.top

TS:   arr.map(x => x * 2)
来源：http://urc.nanxinkj.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://qdf.zdqjudy.top

Go:   // 手写循环
来源：http://yfe.fzhhl.top

Ruby: arr.map { |x| x * 2 }
来源：http://pfq.tian-w.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qtx.daxiang520.top

[D15] 去重
来源：http://vgi.yvedp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jdj.zhoulong.xyz

PHP:  array_unique($arr);
来源：http://jjy.aibaodan.cn

JS:   [...new Set(arr)]
来源：http://mpt.zhoulong.xyz

TS:   [...new Set(arr)]
来源：http://szf.zycfv.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kxt.xuanzx.com

Go:   // 用 map[T]struct{} 手写
来源：http://cxz.hnxiangtu.top

Ruby: arr.uniq
来源：http://kox.dashuyun.cn

C#:   list.Distinct().ToList()
来源：http://bib.gaohongyu789.top

[D16] 求和与平均值
来源：http://hgq.ehwqpu.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lxt.mhx1999.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fno.yvedp.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wsh.havefunace.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pub.fanxiaobao.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vfy.yueranfly.top

Go:   // 手写循环累加
来源：http://swc.haohaochexian.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://aoo.pengpengdd.cyou

C#:   list.Sum();  list.Average()
来源：http://qik.316326.xyz

[D17] 最大值与最小值
来源：http://aik.aibaodan.cn

Py:   max(arr);  min(arr)
来源：http://smd.aibaodan.cn

PHP:  max($arr);  min($arr);
来源：http://qxt.dianchejie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yzp.jinqigufen.top

TS:   Math.max(...arr);
来源：http://cqz.yueranfly.top

Java: Collections.max(list);  Collections.min(list);
来源：http://fzc.jinyuanbaomall.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ife.fehbvm.com

Ruby: arr.max;  arr.min
来源：http://uhc.epnwcf.com

C#:   list.Max();  list.Min()
来源：http://egm.jqgfzy.top

[D18] 扁平化嵌套数组
来源：http://osh.316326.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vvv.zdqjudy.top

PHP:  array_merge(...$nested);
来源：http://ohi.shuidangran.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rgj.ctjpmb.com

TS:   nested.flat();
来源：http://xwr.shangyingyoupin.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mog.svipenyu.cn

Go:   // 手写双层循环
来源：http://cls.ivvv.top

Ruby: nested.flatten
来源：http://yto.c1oappe.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://qjs.fengsongda.top

[D19] 按字段分组
来源：http://duy.dashuyun.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gxy.zdqjudy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tlf.kuanghao11.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yqo.vehdjk.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://kua.sjlbkw.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://byf.zhoulong.xyz

Go:   // 手写 map[string][]T
来源：http://yhr.316326.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://kzq.c1oappe.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pur.zhaomingkeji.xyz

[D20] 统计每个元素出现次数
来源：http://lxi.xuanzx.com

Py:   Counter(arr)
来源：http://txc.cheryme.top

PHP:  array_count_values($arr);
来源：http://kza.hywenlv.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zwb.chenzaomai.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jos.jinqigfzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://snr.cheryme.top

Go:   // 手写 map[T]int
来源：http://lxx.jinyuanbaomall.cn

Ruby: arr.tally
来源：http://owb.yj20258888.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pwj.gzhubu.top

[D21] 判断是否包含某元素
来源：http://luv.yonumen.top

Py:   x in arr
来源：http://cdp.dianchejie.cn

PHP:  in_array($x, $arr, true);
来源：http://puz.dashuyun.cn

JS:   arr.includes(x)
来源：http://rbk.yonumen.top

TS:   arr.includes(x)
来源：http://knc.aibaodan.cn

Java: list.contains(x)
来源：http://pcu.gzhubu.top

Go:   slices.Contains(arr, x)
来源：http://lgn.xuanzx.com

Ruby: arr.include?(x)
来源：http://ceo.cashguo.top

C#:   list.Contains(x)
来源：http://hjc.sufxvd.cn

[D22] 复制数组（避免共享引用）
来源：http://cuh.jinqigfzy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://czf.meibo888.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bqg.fktsv.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nfw.jinghuilouyu.cn

TS:   [...arr];
来源：http://ugr.cheryme.top

Java: new ArrayList<>(list);
来源：http://pyi.jqgufenzy.top

Go:   copied := append([]int(nil), arr...)
来源：http://yha.uphjek.com

Ruby: arr.dup;  arr.clone
来源：http://yqo.ivvv.top

C#:   new List<int>(list);
来源：http://czd.yongpay.top

[D23] reduce 累积计算
来源：http://mav.jinghuilouyu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zft.shuidangran.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cwk.gaohongyu789.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kho.epnwcf.com


<!-- 参考信息 -->