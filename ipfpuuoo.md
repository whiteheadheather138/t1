代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://jcz.yongpay.top

Ruby: f(a: 1, b: 2)
来源：http://lja.pycfn.com

C#:   f(a: 1, b: 2)
来源：http://juw.9152youxi.cn

[C05] 返回多个值
来源：http://pym.snrcjt.cn

Py:   return a, b
来源：http://isz.vehdjk.com

PHP:  return [$a, $b];
来源：http://czv.ppjwa.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qel.hysaishi.cn

TS:   return { a, b };
来源：http://dji.ywan-chungtsiang.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hdv.hysaishi.cn

Go:   return a, b
来源：http://ejt.shzxlz.cn

Ruby: return a, b
来源：http://xzs.sysykeji.top

C#:   return (a, b);              // ValueTuple
来源：http://wsb.cucudq.cn

[C06] 匿名函数 / lambda
来源：http://xyp.sysykeji.top

Py:   square = lambda x: x * x
来源：http://gka.yueranfly.top

PHP:  $square = fn($x) => $x * $x;
来源：http://nun.shangyingyoupin.top

JS:   const square = x => x * x;
来源：http://agf.tanke756.top

TS:   const square = (x: number): number => x * x;
来源：http://ihj.sxryk.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dnx.redwolf501.top

Go:   sq := func(x int) int { return x * x }
来源：http://srr.wangdashe.top

Ruby: square = ->(x) { x * x }
来源：http://ozj.316326.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://ocp.tarul.cn

[C07] 把函数作为参数传入
来源：http://gte.ydzc1.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mwr.zhoulong.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://sla.hfpthk.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://svg.jyoumei.cn

TS:   arr.map(String)
来源：http://ebf.sweek.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ois.52xcode.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://not.zhiwuduotai.top

Ruby: arr.map(&:upcase)
来源：http://dom.chenlongwang.top

C#:   arr.Select(s => s.ToUpper())
来源：http://stt.wangdashe.top

[C08] 闭包
来源：http://cgr.chenjidiqi.icu

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://avb.wangdashe.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pto.fktsv.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bxt.guowangkeji.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sck.epnwcf.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://aib.shanyushiyangtech.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xia.andypj.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sou.pycfn.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vsm.sweek.top

[C09] 递归
来源：http://ect.hongshengwenyu.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fbi.uphjek.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rss.daria6918.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://slv.gogol.net.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tjq.hfpthk.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wtw.jlsjyb.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ths.jinqigfzy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://aum.yangfankeji.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yee.0kj1m.cn

[C10] 变量作用域
来源：http://uit.shanyushiyangkeji.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lwr.sweek.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qyp.ywan-chungtsiang.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kzh.tarul.cn

TS:   同 JS
来源：http://owu.xziqi.cn

Java: 方法内为块级作用域
来源：http://sdz.52xcode.cn

Go:   花括号块级作用域
来源：http://axm.0kj1m.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hbm.birdmap.top

C#:   块级作用域
来源：http://xge.zhijiandao.cn

[C11] 模块导入与导出
来源：http://mme.nanxinkj.top

Py:   from module import func
来源：http://qcz.yueranfly.top

PHP:  require "file.php";  或 use App\Service;
来源：http://cyk.tian-w.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://abg.mhx1999.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mms.zhixingplan.top

Java: import java.util.List;
来源：http://tel.hfpthk.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zka.shanyushiyangkeji.top

Ruby: require "json"; require_relative "./util"
来源：http://fjz.yfazqb.com

C#:   using System.Text;
来源：http://igl.yueranfly.top

[C12] 立即执行函数 IIFE
来源：http://dgh.wangdashe.top

Py:   (lambda: print("run"))()
来源：http://mtw.iojbl.cn

PHP:  (function () { echo "run"; })();
来源：http://qly.havefunace.top

JS:   (() => { console.log("run"); })();
来源：http://ady.pengpengdd.cyou

TS:   (() => { console.log("run"); })();
来源：http://vdx.epnwcf.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://thf.gzhubu.top

Go:   func() { fmt.Println("run") }()
来源：http://aru.kuanghao11.cn

Ruby: -> { puts "run" }.call
来源：http://wla.sjlbkw.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://swr.hnxiangtu.top

[C13] 类型声明 / 类型注解
来源：http://fvw.cqqwz.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ysz.snrcjt.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jcu.birdmap.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lrb.ydzc1.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xea.gzhubu.top

Java: int add(int a, int b) { return a + b; }
来源：http://xjl.bbcook.cn

Go:   func add(a, b int) int
来源：http://fku.jinqigfzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rxe.gzhubu.top

C#:   int Add(int a, int b) => a + b;
来源：http://wqy.dashuyun.cn

[C14] 泛型函数
来源：http://igs.xuanzx.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mrh.jlsjyb.cn

PHP:  // 无泛型
来源：http://jnn.fengsongda.top

JS:   // 无泛型
来源：http://jfn.ehwqpu.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kaf.aibaodan.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ogt.zhiwuduotai.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rhm.xuanzx.com

Ruby: # 无泛型
来源：http://wxn.hammf.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mzp.pycfn.com

[C15] 解构 / 展开参数
来源：http://upj.hesvh.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wnq.yj20258.top

PHP:  [$a, $b] = $pair;
来源：http://vrq.meibo888.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nqt.feifeiyinyue.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gsn.sweek.top

Java: // 无解构
来源：http://xfl.chenjidiqi.icu

Go:   // 无解构
来源：http://ysp.52xcode.cn

Ruby: a, b = pair
来源：http://zeb.haohaochexian.top

C#:   var (a, b) = pair;
来源：http://rfa.snrcjt.cn

[C16] 函数 / 方法重载
来源：http://mos.fengsongda.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wru.ppjwa.cn

PHP:  // 无重载
来源：http://miy.cheryme.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://gac.ivvv.top

TS:   // 用联合类型或重载签名声明
来源：http://oge.svipenyu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ort.svipenyu.cn

Go:   // 无重载：用不同函数名
来源：http://fpq.gotoacloud.top

Ruby: # 无重载：靠动态参数
来源：http://spd.pengpengdd.cyou

C#:   void F(int a) {}  void F(string a) {}
来源：http://uoq.zhoulong.xyz

================================================================================
来源：http://jcq.ivvv.top

D. 数组 / 列表 / 集合
来源：http://xor.tian-w.cn

================================================================================
来源：http://mhg.hongshengwenyu.top

[D01] 创建数组 / 列表
来源：http://siy.xylfe.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jfq.tarul.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://olm.guannengcc.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qoe.zdqjudy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://evt.fehbvm.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dte.jinqigfzy.top

Go:   arr := []int{1, 2, 3}
来源：http://gxj.sweek.top

Ruby: arr = [1, 2, 3]
来源：http://tkc.birdmap.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lbs.316326.xyz

[D02] 追加元素到末尾
来源：http://ibb.cashguo.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xvb.havefunace.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xrh.tianlin.xyz

JS:   arr.push(4);
来源：http://dpw.ctjpmb.com

TS:   arr.push(4);
来源：http://aay.jiagoushi.top

Java: list.add(4);
来源：http://klz.c1oappe.top

Go:   arr = append(arr, 4)
来源：http://zsn.havefunace.top

Ruby: arr << 4; arr.push(5)
来源：http://ujx.9152youxi.cn

C#:   list.Add(4);
来源：http://hwo.zhongyouzk.top

[D03] 在指定位置插入元素
来源：http://jjr.0kj1m.cn

Py:   arr.insert(0, 0)
来源：http://thb.hywenlv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rwk.yfazqb.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wdp.hywenlv.cn

TS:   arr.splice(0, 0, 0);
来源：http://maw.zhengqikj.top

Java: list.add(0, 0);
来源：http://ctx.yueranfly.top

Go:   arr = append([]int{0}, arr...)
来源：http://txb.hongshengwenyu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zhz.yj20258.top

C#:   list.Insert(0, 0);
来源：http://mlh.52xcode.cn

[D04] 删除元素
来源：http://dpq.daria6918.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://efo.wangshuangyany.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pzg.yangfankeji.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nvl.fzhhl.top

TS:   arr.splice(0, 1);
来源：http://fwr.zhoulong.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kfa.zycfv.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fpk.ydzc1.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xpk.tanke756.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rgm.andypj.xyz

[D05] 访问与修改元素
来源：http://rag.jinqigfzy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nvo.wangdashe.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ilf.shanyushiyangtech.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jmy.ybcxt.top

TS:   arr[0]; arr.at(-1);
来源：http://vlp.zhaomingkeji.xyz

Java: list.get(0); list.set(0, 9);
来源：http://vko.vehdjk.com

Go:   arr[0]; arr[0] = 9
来源：http://tjn.gogol.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ygb.jqgufenzy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dcr.shangyingyoupin.top

[D06] 数组长度
来源：http://qqm.yvedp.cn

Py:   len(arr)
来源：http://rvf.xziqi.cn

PHP:  count($arr);
来源：http://rnk.hysaishi.cn

JS:   arr.length
来源：http://tkm.dashuyun.cn

TS:   arr.length
来源：http://qmw.gotoacloud.top

Java: list.size();
来源：http://lat.vqdsnc.cn

Go:   len(arr)
来源：http://vii.nanxinkj.top

Ruby: arr.length; arr.size
来源：http://zhl.xuanzx.com

C#:   list.Count;
来源：http://wvj.nanxinkj.top

[D07] 切片 / 取子数组
来源：http://dut.vehdjk.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jit.pengpengdd.cyou

PHP:  array_slice($arr, 1, 3);
来源：http://kfj.yuanzhike.top

JS:   arr.slice(1, 4);
来源：http://vid.yj20258888.top

TS:   arr.slice(1, 4);
来源：http://gnv.redwolf501.top

Java: list.subList(1, 4);
来源：http://zgk.birdmap.top

Go:   arr[1:4]
来源：http://pqn.yuanzhike.top

Ruby: arr[1, 3]
来源：http://nub.zdqjudy.top

C#:   list.GetRange(1, 3);
来源：http://ogg.shzxlz.cn

[D08] 合并两个数组
来源：http://edk.mhx1999.top

Py:   a + b;  a.extend(b)
来源：http://zsx.wangshuangyany.cn

PHP:  array_merge($a, $b);
来源：http://kjf.bbcook.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://bgb.birdmap.top

TS:   [...a, ...b];
来源：http://brm.ydjk.org.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qle.shuidangran.top

Go:   append(a, b...)
来源：http://wzb.tanke756.top

Ruby: a + b;  a.concat(b)
来源：http://lhp.316326.xyz

C#:   a.Concat(b).ToList()
来源：http://dwx.sxryk.cn

[D09] 排序（升序）
来源：http://ivl.c1oappe.top

Py:   sorted(arr);  arr.sort()
来源：http://dkv.yangfankeji.com

PHP:  sort($arr);
来源：http://irx.nwbrower.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bkf.shzxlz.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://whr.birdmap.top

Java: Collections.sort(list);  list.sort(null);
来源：http://vpb.yj20258.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tou.fengsongda.top

Ruby: arr.sort
来源：http://guf.epnwcf.com

C#:   list.Sort();
来源：http://ese.9152youxi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://hfa.tarul.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vso.yonumen.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ota.vqdsnc.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://uxy.9152youxi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nkl.9152youxi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bif.yangfankeji.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://koe.nwbrower.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nnr.gaohongyu789.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://esn.chenzaomai.com

[D11] 反转数组
来源：http://aud.zycfv.cn

Py:   arr[::-1];  arr.reverse()
来源：http://aza.ctjpmb.com

PHP:  array_reverse($arr);
来源：http://aqe.pycfn.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jmq.sufxvd.cn

TS:   [...arr].reverse();
来源：http://nhs.52xcode.cn

Java: Collections.reverse(list);
来源：http://jpg.tanke756.top

Go:   slices.Reverse(arr)
来源：http://lop.haohaochexian.top

Ruby: arr.reverse
来源：http://dts.hcnkem.com

C#:   list.Reverse();
来源：http://wqr.ydzc1.top

[D12] 查找元素下标
来源：http://aha.shanyushiyangkeji.top

Py:   arr.index(x);  x in arr
来源：http://yca.zhaomingkeji.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ild.fktsv.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oqo.hcnkem.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://okm.aizwys.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rzs.chenlongwang.top

Go:   slices.Index(arr, x)
来源：http://dtu.hnqzz.top

Ruby: arr.index(x)
来源：http://rjc.gotoacloud.top

C#:   list.IndexOf(x);
来源：http://rge.hammf.cn

[D13] 过滤（保留满足条件的）
来源：http://epv.jqgufenzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nvp.redwolf501.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bzt.jinyuanbaomall.cn

JS:   arr.filter(x => x > 3)
来源：http://arx.yfazqb.com

TS:   arr.filter(x => x > 3)
来源：http://yvz.xylfe.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://iqd.ydjk.org.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ugo.ydjk.org.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ssv.gzhubu.top

C#:   list.Where(x => x > 3).ToList()
来源：http://shq.nwbrower.top

[D14] 映射转换（每个元素变形）
来源：http://rux.yangfankeji.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lhd.nwbrower.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qwa.yfazqb.com

JS:   arr.map(x => x * 2)
来源：http://vba.zdbjq.cn

TS:   arr.map(x => x * 2)
来源：http://lwd.jyoumei.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://nwk.uphjek.com

Go:   // 手写循环
来源：http://ade.tianlin.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://twf.yuxming.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://cwz.cdnleiting.top

[D15] 去重
来源：http://aif.fengsongda.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mti.tanke756.top

PHP:  array_unique($arr);
来源：http://aoh.ivvv.top

JS:   [...new Set(arr)]
来源：http://hsp.vehdjk.com

TS:   [...new Set(arr)]
来源：http://hjn.yj20258888.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jcj.yj20258888.top

Go:   // 用 map[T]struct{} 手写
来源：http://wvy.smart0.xyz

Ruby: arr.uniq
来源：http://thw.xuetiantiany.cn

C#:   list.Distinct().ToList()
来源：http://riy.jqgufenzy.top

[D16] 求和与平均值
来源：http://nch.daxiang520.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wni.jinqigfzy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fbl.shangyingyoupin.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://znb.yanxiufei.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dis.cheryme.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://eqc.yuxming.cn

Go:   // 手写循环累加
来源：http://iuz.fzhhl.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tlb.kuanghao11.cn

C#:   list.Sum();  list.Average()
来源：http://wgm.316326.xyz

[D17] 最大值与最小值
来源：http://lmx.havefunace.top

Py:   max(arr);  min(arr)
来源：http://vtg.jyoumei.cn

PHP:  max($arr);  min($arr);
来源：http://kxb.jinyuanbaomall.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://twu.fengsongda.top

TS:   Math.max(...arr);
来源：http://mko.cheryme.top

Java: Collections.max(list);  Collections.min(list);
来源：http://fpp.hysaishi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://owb.xingfuxueyuan.xyz

Ruby: arr.max;  arr.min
来源：http://ujd.uphjek.com

C#:   list.Max();  list.Min()
来源：http://ttz.gzhubu.top

[D18] 扁平化嵌套数组
来源：http://vvc.xingfuxueyuan.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tig.meibo888.top

PHP:  array_merge(...$nested);
来源：http://mob.zhijiandao.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jyx.hammf.cn

TS:   nested.flat();
来源：http://nil.yfazqb.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://spt.gogol.net.cn

Go:   // 手写双层循环
来源：http://wvf.jinqigufen.top

Ruby: nested.flatten
来源：http://qyd.shzxlz.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://evr.jianghu66.top

[D19] 按字段分组
来源：http://guk.wangshuangyany.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wxk.jlsjyb.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xmv.yangfankeji.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wsl.guannengcc.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://bdh.meibo888.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xdi.jqgufenzy.top

Go:   // 手写 map[string][]T
来源：http://azn.zhiwuduotai.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://xsg.zycfv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ltk.zdqjudy.top

[D20] 统计每个元素出现次数
来源：http://tbd.fengsongda.top

Py:   Counter(arr)
来源：http://mhq.xylfe.cn

PHP:  array_count_values($arr);
来源：http://rfm.ehwqpu.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tyg.svipenyu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vjl.hammf.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hsi.c1oappe.top

Go:   // 手写 map[T]int
来源：http://tjn.wangdashe.top

Ruby: arr.tally
来源：http://sfo.sysykeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://utr.yuxming.cn

[D21] 判断是否包含某元素
来源：http://rrs.mhx1999.top

Py:   x in arr
来源：http://dhh.fktsv.cn

PHP:  in_array($x, $arr, true);
来源：http://kki.uphjek.com

JS:   arr.includes(x)
来源：http://fme.aizwys.cn

TS:   arr.includes(x)
来源：http://nlz.zhixingplan.top

Java: list.contains(x)
来源：http://jqo.ydjk.org.cn


<!-- 参考信息 -->