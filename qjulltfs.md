代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vqr.uphjek.com

Go:   return a, b
来源：http://nmv.hfpthk.cn

Ruby: return a, b
来源：http://wtq.vqdsnc.cn

C#:   return (a, b);              // ValueTuple
来源：http://hsn.sjlbkw.cn

[C06] 匿名函数 / lambda
来源：http://svv.fktsv.cn

Py:   square = lambda x: x * x
来源：http://zgw.uphjek.com

PHP:  $square = fn($x) => $x * $x;
来源：http://eoe.ivvv.top

JS:   const square = x => x * x;
来源：http://kja.aizwys.cn

TS:   const square = (x: number): number => x * x;
来源：http://xwd.hnxiangtu.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gsd.wangdashe.top

Go:   sq := func(x int) int { return x * x }
来源：http://ahu.guannengcc.top

Ruby: square = ->(x) { x * x }
来源：http://zfx.bbcook.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fdn.cqqwz.cn

[C07] 把函数作为参数传入
来源：http://ibq.svipenyu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://egg.shangyingyoupin.top

PHP:  array_map("strtoupper", $arr);
来源：http://yyl.shanyushiyangtech.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pyv.jinghuilouyu.cn

TS:   arr.map(String)
来源：http://wby.xuanzx.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nse.xziqi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vpf.tian-w.cn

Ruby: arr.map(&:upcase)
来源：http://ybq.meibo888.top

C#:   arr.Select(s => s.ToUpper())
来源：http://fot.vqdsnc.cn

[C08] 闭包
来源：http://ngo.jinyuanbaomall.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://eyl.wangdashe.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rca.aizwys.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://aeo.cqqwz.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xtu.zdqjudy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pow.ybcxt.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://edq.chenzaomai.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zou.yj202588.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gpi.jqgfzy.top

[C09] 递归
来源：http://gog.ctjpmb.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pnw.yuxming.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://twp.smart0.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kjp.tian-w.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vwu.redwolf501.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://toj.xingfuxueyuan.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wzi.gotoacloud.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wpc.cucudq.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bgj.ybcxt.top

[C10] 变量作用域
来源：http://alg.yonumen.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bjh.uphjek.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vaq.yuanzhike.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zve.ivvv.top

TS:   同 JS
来源：http://ixe.jiagoushi.top

Java: 方法内为块级作用域
来源：http://qjb.yueranfly.top

Go:   花括号块级作用域
来源：http://ykn.shangyingyoupin.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nav.havefunace.top

C#:   块级作用域
来源：http://vjx.hysaishi.cn

[C11] 模块导入与导出
来源：http://wyw.shzxlz.cn

Py:   from module import func
来源：http://fit.yuxming.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kez.chenlongwang.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://oga.ppjwa.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vsh.zdbjq.cn

Java: import java.util.List;
来源：http://qal.chenlongwang.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hpl.zhengqikj.top

Ruby: require "json"; require_relative "./util"
来源：http://dfz.nanxinkj.top

C#:   using System.Text;
来源：http://mwn.zycfv.cn

[C12] 立即执行函数 IIFE
来源：http://ini.jqgfzy.top

Py:   (lambda: print("run"))()
来源：http://cin.feifeiyinyue.top

PHP:  (function () { echo "run"; })();
来源：http://veo.yanxiufei.cn

JS:   (() => { console.log("run"); })();
来源：http://zba.shangyingyoupin.top

TS:   (() => { console.log("run"); })();
来源：http://vqj.sjlbkw.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ksz.xziqi.cn

Go:   func() { fmt.Println("run") }()
来源：http://asn.xuanzx.com

Ruby: -> { puts "run" }.call
来源：http://jmb.fktsv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://oln.birdmap.top

[C13] 类型声明 / 类型注解
来源：http://oxn.yuanzhike.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gqn.andypj.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mwe.jinyuanbaomall.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vqo.fzhhl.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rjt.kuanghao11.cn

Java: int add(int a, int b) { return a + b; }
来源：http://hcl.birdmap.top

Go:   func add(a, b int) int
来源：http://yqs.svipenyu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vap.hammf.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mst.gotoacloud.top

[C14] 泛型函数
来源：http://bro.zhaomingkeji.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://coq.zdbjq.cn

PHP:  // 无泛型
来源：http://mlx.gotoacloud.top

JS:   // 无泛型
来源：http://lgg.jinghuilouyu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://axb.shzxlz.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bep.sxryk.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yad.9152youxi.cn

Ruby: # 无泛型
来源：http://niy.wangshuangyany.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zui.havefunace.top

[C15] 解构 / 展开参数
来源：http://lwt.hongshengwenyu.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://iwa.shuidangran.top

PHP:  [$a, $b] = $pair;
来源：http://cec.vqdsnc.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kak.tian-w.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hra.xziqi.cn

Java: // 无解构
来源：http://yqy.nanxinkj.top

Go:   // 无解构
来源：http://quh.havefunace.top

Ruby: a, b = pair
来源：http://aqq.havefunace.top

C#:   var (a, b) = pair;
来源：http://dzm.pycfn.com

[C16] 函数 / 方法重载
来源：http://vej.dashuyun.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sbq.gaohongyu789.top

PHP:  // 无重载
来源：http://gaa.chenjidiqi.icu

JS:   // 无重载：靠 arguments.length 分支
来源：http://kul.sxryk.cn

TS:   // 用联合类型或重载签名声明
来源：http://rxx.yangfankeji.com

Java: void f(int a) {}  void f(String a) {}
来源：http://rsd.yangfankeji.com

Go:   // 无重载：用不同函数名
来源：http://xxx.xinyue.icu

Ruby: # 无重载：靠动态参数
来源：http://jhw.guowangkeji.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ddu.zhiwuduotai.top

================================================================================
来源：http://ify.epnwcf.com

D. 数组 / 列表 / 集合
来源：http://mgd.yj20258.top

================================================================================
来源：http://qyz.svipenyu.cn

[D01] 创建数组 / 列表
来源：http://ndo.dashuyun.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zft.yanxiufei.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lvd.gaohongyu789.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blw.sjlbkw.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://nvb.cheryme.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uft.dashuyun.cn

Go:   arr := []int{1, 2, 3}
来源：http://ckj.xylfe.cn

Ruby: arr = [1, 2, 3]
来源：http://ere.svipenyu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mrg.jlsjyb.cn

[D02] 追加元素到末尾
来源：http://psv.xuetiantiany.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mun.xylfe.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fde.kuanghao11.cn

JS:   arr.push(4);
来源：http://xbi.cucudq.cn

TS:   arr.push(4);
来源：http://fos.hnxiangtu.top

Java: list.add(4);
来源：http://wfp.zhixingplan.top

Go:   arr = append(arr, 4)
来源：http://hho.ywan-chungtsiang.top

Ruby: arr << 4; arr.push(5)
来源：http://fhs.hnxiangtu.top

C#:   list.Add(4);
来源：http://feg.gotoacloud.top

[D03] 在指定位置插入元素
来源：http://kkx.ctjpmb.com

Py:   arr.insert(0, 0)
来源：http://tql.ivvv.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://idy.yongpay.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://msn.zdbjq.cn

TS:   arr.splice(0, 0, 0);
来源：http://oas.andypj.xyz

Java: list.add(0, 0);
来源：http://qph.9152youxi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://lgt.ydzc1.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vvf.yfazqb.com

C#:   list.Insert(0, 0);
来源：http://flu.yonumen.top

[D04] 删除元素
来源：http://teo.sufxvd.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pju.316326.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zhu.guowangkeji.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rxn.jinqigfzy.top

TS:   arr.splice(0, 1);
来源：http://ixc.sysykeji.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jmi.gaohongyu789.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nrr.pengpengdd.cyou

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bxp.zhoulong.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gfx.quarkkingdee.top

[D05] 访问与修改元素
来源：http://pis.fktsv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wxq.redwolf501.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vai.316326.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lll.haohaochexian.top

TS:   arr[0]; arr.at(-1);
来源：http://fka.nanxuanxn.top

Java: list.get(0); list.set(0, 9);
来源：http://gvd.havefunace.top

Go:   arr[0]; arr[0] = 9
来源：http://foz.ydjk.org.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kqj.ehwqpu.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bcj.cqqwz.cn

[D06] 数组长度
来源：http://znr.tanke756.top

Py:   len(arr)
来源：http://ttp.hcnkem.com

PHP:  count($arr);
来源：http://kyo.zhijiandao.cn

JS:   arr.length
来源：http://rse.tarul.cn

TS:   arr.length
来源：http://ovc.cucudq.cn

Java: list.size();
来源：http://vai.zhoulong.xyz

Go:   len(arr)
来源：http://exl.dianchejie.cn

Ruby: arr.length; arr.size
来源：http://hzo.chenlongwang.top

C#:   list.Count;
来源：http://kkb.ybcxt.top

[D07] 切片 / 取子数组
来源：http://gak.xuanzx.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bhh.birdmap.top

PHP:  array_slice($arr, 1, 3);
来源：http://nsi.chenzaomai.com

JS:   arr.slice(1, 4);
来源：http://cfv.meibo888.top

TS:   arr.slice(1, 4);
来源：http://ykp.dashuyun.cn

Java: list.subList(1, 4);
来源：http://hoj.0kj1m.cn

Go:   arr[1:4]
来源：http://ham.hesvh.cn

Ruby: arr[1, 3]
来源：http://ohe.xingfuxueyuan.xyz

C#:   list.GetRange(1, 3);
来源：http://kaz.shangyingyoupin.top

[D08] 合并两个数组
来源：http://cvy.hammf.cn

Py:   a + b;  a.extend(b)
来源：http://bbq.yangfankeji.com

PHP:  array_merge($a, $b);
来源：http://npv.zhaomingkeji.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://gim.fanxiaobao.xyz

TS:   [...a, ...b];
来源：http://cdf.hysaishi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jno.jqgufenzy.top

Go:   append(a, b...)
来源：http://qee.yangfankeji.com

Ruby: a + b;  a.concat(b)
来源：http://ttk.zhiwuduotai.top

C#:   a.Concat(b).ToList()
来源：http://jvp.shuidangran.top

[D09] 排序（升序）
来源：http://kif.cdnleiting.top

Py:   sorted(arr);  arr.sort()
来源：http://iin.zhongyouzk.top

PHP:  sort($arr);
来源：http://xez.pengpengdd.cyou

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sxx.0kj1m.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://sdw.tianlin.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://xpg.bjfxy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://abk.vehdjk.com

Ruby: arr.sort
来源：http://bis.pengpengdd.cyou

C#:   list.Sort();
来源：http://ggo.guannengcc.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://smd.yanxiufei.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gwh.9152youxi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ktr.tian-w.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nwj.yonumen.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ulv.xingfuxueyuan.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://oaw.yj20258888.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cue.yuanzhike.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rbp.daria6918.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yqe.jinqigufen.top

[D11] 反转数组
来源：http://zcc.jinqigufen.top

Py:   arr[::-1];  arr.reverse()
来源：http://amd.zdqjudy.top

PHP:  array_reverse($arr);
来源：http://ybm.sysykeji.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://svc.bbcook.cn

TS:   [...arr].reverse();
来源：http://yve.jiagoushi.top

Java: Collections.reverse(list);
来源：http://xsd.jinqigfzy.top

Go:   slices.Reverse(arr)
来源：http://ukx.aizwys.cn

Ruby: arr.reverse
来源：http://spy.hongshengwenyu.top

C#:   list.Reverse();
来源：http://jyh.meibo888.top

[D12] 查找元素下标
来源：http://usp.yuxming.cn

Py:   arr.index(x);  x in arr
来源：http://rzg.shangyingyoupin.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dwj.aibaodan.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bxz.chenlongwang.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qks.jinghuilouyu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uue.fzhhl.top

Go:   slices.Index(arr, x)
来源：http://vpr.mhx1999.top

Ruby: arr.index(x)
来源：http://rdn.zhongyouzk.top

C#:   list.IndexOf(x);
来源：http://vtv.hysaishi.cn

[D13] 过滤（保留满足条件的）
来源：http://oas.ivvv.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tbh.hammf.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pgo.hfpthk.cn

JS:   arr.filter(x => x > 3)
来源：http://scc.cqqwz.cn

TS:   arr.filter(x => x > 3)
来源：http://ipx.shangyingyoupin.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pdm.daxiang520.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ewn.chenzaomai.com

Ruby: arr.select { |x| x > 3 }
来源：http://ljs.fehbvm.com

C#:   list.Where(x => x > 3).ToList()
来源：http://kuz.yj20258888.top

[D14] 映射转换（每个元素变形）
来源：http://rit.shzxlz.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dzy.tanke756.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lsm.hcnkem.com

JS:   arr.map(x => x * 2)
来源：http://geg.gogol.net.cn

TS:   arr.map(x => x * 2)
来源：http://jmn.jinyuanbaomall.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ddv.wangshuangyany.cn

Go:   // 手写循环
来源：http://guo.shangyingyoupin.top

Ruby: arr.map { |x| x * 2 }
来源：http://fqo.aizwys.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://scj.xinyue.icu

[D15] 去重
来源：http://yjd.zhoulong.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lki.tianlin.xyz

PHP:  array_unique($arr);
来源：http://lsk.smart0.xyz

JS:   [...new Set(arr)]
来源：http://pod.cashguo.top

TS:   [...new Set(arr)]
来源：http://vzj.yuanzhike.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bvb.fzhhl.top

Go:   // 用 map[T]struct{} 手写
来源：http://gjo.yongpay.top

Ruby: arr.uniq
来源：http://qci.nwbrower.top

C#:   list.Distinct().ToList()
来源：http://olq.xingfuxueyuan.xyz

[D16] 求和与平均值
来源：http://bgc.yvedp.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://srk.hcnkem.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ztm.cheryme.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://som.yangfankeji.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qsx.zhixingplan.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hym.gzhubu.top

Go:   // 手写循环累加
来源：http://flk.jinqigfzy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://twf.hcnkem.com

C#:   list.Sum();  list.Average()
来源：http://lzz.gogol.net.cn

[D17] 最大值与最小值
来源：http://nwn.9152youxi.cn

Py:   max(arr);  min(arr)
来源：http://yvt.yuxming.cn

PHP:  max($arr);  min($arr);
来源：http://zui.xinyue.icu

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zjo.316326.xyz

TS:   Math.max(...arr);
来源：http://wvo.zhijiandao.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://exq.sysykeji.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ayf.bjfxy.top

Ruby: arr.max;  arr.min
来源：http://wfp.fktsv.cn

C#:   list.Max();  list.Min()
来源：http://ofo.fehbvm.com

[D18] 扁平化嵌套数组
来源：http://hcl.andypj.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ovo.zhongyouzk.top

PHP:  array_merge(...$nested);
来源：http://yog.gzhubu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jcs.zdbjq.cn

TS:   nested.flat();
来源：http://hiq.hywenlv.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ubp.sysykeji.top

Go:   // 手写双层循环
来源：http://kus.xziqi.cn

Ruby: nested.flatten
来源：http://aqg.tian-w.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hod.xziqi.cn

[D19] 按字段分组
来源：http://ssc.jinqigufen.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://puq.hfpthk.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fpy.hammf.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pbs.dianchejie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://mbk.fktsv.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qzz.yueranfly.top

Go:   // 手写 map[string][]T
来源：http://prx.hfpthk.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://twi.chenlongwang.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kgk.ehwqpu.com

[D20] 统计每个元素出现次数
来源：http://meg.zhixingplan.top

Py:   Counter(arr)
来源：http://bvi.guannengcc.top

PHP:  array_count_values($arr);
来源：http://ues.cdnleiting.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mne.fehbvm.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hvd.yonumen.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lmw.zdqjudy.top

Go:   // 手写 map[T]int
来源：http://dra.zdqjudy.top

Ruby: arr.tally
来源：http://xzo.dianchejie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ufw.hcnkem.com

[D21] 判断是否包含某元素
来源：http://mat.jlsjyb.cn

Py:   x in arr
来源：http://rgn.jinqigufen.top

PHP:  in_array($x, $arr, true);
来源：http://cqu.xinyue.icu

JS:   arr.includes(x)
来源：http://ebw.yuxming.cn

TS:   arr.includes(x)
来源：http://psc.wangdashe.top

Java: list.contains(x)
来源：http://gyk.yanxiufei.cn

Go:   slices.Contains(arr, x)
来源：http://usp.zycfv.cn

Ruby: arr.include?(x)
来源：http://xnx.zdqjudy.top

C#:   list.Contains(x)
来源：http://zew.jinqigfzy.top

[D22] 复制数组（避免共享引用）
来源：http://bab.ydzc1.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gqa.daxiang520.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jmo.hcnkem.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gfi.chenzaomai.com

TS:   [...arr];
来源：http://dae.fzhhl.top


<!-- 参考信息 -->