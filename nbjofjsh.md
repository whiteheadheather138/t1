代发 wailian999

Py:   return a, b
来源：http://ijt.shangyingyoupin.top

PHP:  return [$a, $b];
来源：http://frw.hnqzz.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://rzn.jinqigufen.top

TS:   return { a, b };
来源：http://nfa.zhongyouzk.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zeh.vehdjk.com

Go:   return a, b
来源：http://niz.sjlbkw.cn

Ruby: return a, b
来源：http://wki.fzhhl.top

C#:   return (a, b);              // ValueTuple
来源：http://hxo.daxiang520.top

[C06] 匿名函数 / lambda
来源：http://nlb.smart0.xyz

Py:   square = lambda x: x * x
来源：http://qcp.jqgufenzy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://pvn.wangshuangyany.cn

JS:   const square = x => x * x;
来源：http://vug.snrcjt.cn

TS:   const square = (x: number): number => x * x;
来源：http://ypw.wangdashe.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wnp.ybcxt.top

Go:   sq := func(x int) int { return x * x }
来源：http://xga.uphjek.com

Ruby: square = ->(x) { x * x }
来源：http://jar.quarkkingdee.top

C#:   Func<int, int> square = x => x * x;
来源：http://ikp.fanxiaobao.xyz

[C07] 把函数作为参数传入
来源：http://vkw.xuetiantiany.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wbk.andypj.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://oui.gotoacloud.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lgz.jqgufenzy.top

TS:   arr.map(String)
来源：http://onv.havefunace.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qnh.daxiang520.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pyw.vqdsnc.cn

Ruby: arr.map(&:upcase)
来源：http://kua.tianlin.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://dzd.xinyue.icu

[C08] 闭包
来源：http://ric.wangdashe.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ghx.xylfe.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://eat.jyoumei.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zzt.uphjek.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xsy.zhengqikj.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qbg.hammf.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lmb.bbcook.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://eqh.hcnkem.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mea.shzxlz.cn

[C09] 递归
来源：http://fdh.bjfxy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cyc.xylfe.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ydy.hongshengwenyu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qbg.andypj.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uzs.jqgfzy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://isv.cashguo.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rrv.dianchejie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://svm.nanxinkj.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wrt.fanxiaobao.xyz

[C10] 变量作用域
来源：http://vzk.jinqigfzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ipi.jianghu66.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qxe.dashuyun.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://adm.andypj.xyz

TS:   同 JS
来源：http://mrh.epnwcf.com

Java: 方法内为块级作用域
来源：http://arc.pengpengdd.cyou

Go:   花括号块级作用域
来源：http://nxq.zycfv.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cfg.zhiwuduotai.top

C#:   块级作用域
来源：http://wcw.sweek.top

[C11] 模块导入与导出
来源：http://drt.cucudq.cn

Py:   from module import func
来源：http://ywa.daxiang520.top

PHP:  require "file.php";  或 use App\Service;
来源：http://bka.vqdsnc.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vti.feifeiyinyue.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jha.fzhhl.top

Java: import java.util.List;
来源：http://xtj.c1oappe.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://itr.jiagoushi.top

Ruby: require "json"; require_relative "./util"
来源：http://hft.cdnleiting.top

C#:   using System.Text;
来源：http://mti.xziqi.cn

[C12] 立即执行函数 IIFE
来源：http://ypy.0kj1m.cn

Py:   (lambda: print("run"))()
来源：http://yof.zhiwuduotai.top

PHP:  (function () { echo "run"; })();
来源：http://crf.yvedp.cn

JS:   (() => { console.log("run"); })();
来源：http://fgb.tanke756.top

TS:   (() => { console.log("run"); })();
来源：http://sky.xinyue.icu

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ueh.redwolf501.top

Go:   func() { fmt.Println("run") }()
来源：http://qml.jqgfzy.top

Ruby: -> { puts "run" }.call
来源：http://pcm.yuxming.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pog.shanyushiyangtech.top

[C13] 类型声明 / 类型注解
来源：http://uzj.dashuyun.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://abq.nanxuanxn.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oae.zycfv.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://adk.yongpay.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://imp.shangyingyoupin.top

Java: int add(int a, int b) { return a + b; }
来源：http://bsw.yj20258.top

Go:   func add(a, b int) int
来源：http://agw.xingfuxueyuan.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gis.ctjpmb.com

C#:   int Add(int a, int b) => a + b;
来源：http://ent.cheryme.top

[C14] 泛型函数
来源：http://mxa.epnwcf.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zwg.jianghu66.top

PHP:  // 无泛型
来源：http://kcc.ctjpmb.com

JS:   // 无泛型
来源：http://tjw.zycfv.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lkf.gaohongyu789.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://veu.0kj1m.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kjv.yj20258.top

Ruby: # 无泛型
来源：http://qil.yj202588.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mrh.andypj.xyz

[C15] 解构 / 展开参数
来源：http://nao.jyoumei.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rxc.yj202588.top

PHP:  [$a, $b] = $pair;
来源：http://ttn.yangfankeji.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ivh.smart0.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pjt.zhaomingkeji.xyz

Java: // 无解构
来源：http://xpf.birdmap.top

Go:   // 无解构
来源：http://nth.andypj.xyz

Ruby: a, b = pair
来源：http://gos.tian-w.cn

C#:   var (a, b) = pair;
来源：http://qvp.quarkkingdee.top

[C16] 函数 / 方法重载
来源：http://kef.daxiang520.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mqe.hongshengwenyu.top

PHP:  // 无重载
来源：http://vjy.xinyue.icu

JS:   // 无重载：靠 arguments.length 分支
来源：http://qcb.zhengqikj.top

TS:   // 用联合类型或重载签名声明
来源：http://yvd.jqgufenzy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://sfg.shuidangran.top

Go:   // 无重载：用不同函数名
来源：http://pgc.tian-w.cn

Ruby: # 无重载：靠动态参数
来源：http://zab.hysaishi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://llt.gotoacloud.top

================================================================================
来源：http://cyp.jinqigfzy.top

D. 数组 / 列表 / 集合
来源：http://krv.cdnleiting.top

================================================================================
来源：http://rdg.zhaomingkeji.xyz

[D01] 创建数组 / 列表
来源：http://zpz.smart0.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://vgv.chenjidiqi.icu

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fek.vqdsnc.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zjm.yueranfly.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://quz.svipenyu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://prj.yj20258.top

Go:   arr := []int{1, 2, 3}
来源：http://kjf.svipenyu.cn

Ruby: arr = [1, 2, 3]
来源：http://cie.redwolf501.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kri.9152youxi.cn

[D02] 追加元素到末尾
来源：http://fww.yj20258.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pbu.dashuyun.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oks.aizwys.cn

JS:   arr.push(4);
来源：http://unb.hammf.cn

TS:   arr.push(4);
来源：http://hwh.kuanghao11.cn

Java: list.add(4);
来源：http://dpo.yj20258888.top

Go:   arr = append(arr, 4)
来源：http://oot.ydjk.org.cn

Ruby: arr << 4; arr.push(5)
来源：http://nsd.ehwqpu.com

C#:   list.Add(4);
来源：http://zgp.snrcjt.cn

[D03] 在指定位置插入元素
来源：http://mdo.gzhubu.top

Py:   arr.insert(0, 0)
来源：http://fao.zycfv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ejt.xuanzx.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ycg.xziqi.cn

TS:   arr.splice(0, 0, 0);
来源：http://wpq.zhixingplan.top

Java: list.add(0, 0);
来源：http://lwz.daxiang520.top

Go:   arr = append([]int{0}, arr...)
来源：http://lrt.fktsv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lfs.fzhhl.top

C#:   list.Insert(0, 0);
来源：http://nml.yvedp.cn

[D04] 删除元素
来源：http://bug.shuidangran.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ysd.52xcode.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bxj.epnwcf.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bnl.guowangkeji.top

TS:   arr.splice(0, 1);
来源：http://lob.sjlbkw.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://onl.tian-w.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dlg.cashguo.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wqv.fktsv.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://eeu.9152youxi.cn

[D05] 访问与修改元素
来源：http://ghm.guowangkeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tjl.jinqigfzy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jlg.gaohongyu789.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tah.ivvv.top

TS:   arr[0]; arr.at(-1);
来源：http://uwi.tianlin.xyz

Java: list.get(0); list.set(0, 9);
来源：http://blw.dashuyun.cn

Go:   arr[0]; arr[0] = 9
来源：http://ohk.xziqi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pzf.sxryk.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ibh.yvedp.cn

[D06] 数组长度
来源：http://dbl.yuxming.cn

Py:   len(arr)
来源：http://vur.zhongyouzk.top

PHP:  count($arr);
来源：http://duo.hywenlv.cn

JS:   arr.length
来源：http://aso.iojbl.cn

TS:   arr.length
来源：http://yvs.cheryme.top

Java: list.size();
来源：http://vjc.guannengcc.top

Go:   len(arr)
来源：http://oyc.snrcjt.cn

Ruby: arr.length; arr.size
来源：http://utj.52xcode.cn

C#:   list.Count;
来源：http://dyi.fehbvm.com

[D07] 切片 / 取子数组
来源：http://zvq.cucudq.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xpy.52xcode.cn

PHP:  array_slice($arr, 1, 3);
来源：http://iwt.jinqigufen.top

JS:   arr.slice(1, 4);
来源：http://dda.tarul.cn

TS:   arr.slice(1, 4);
来源：http://zpq.nwbrower.top

Java: list.subList(1, 4);
来源：http://lbw.quarkkingdee.top

Go:   arr[1:4]
来源：http://vzu.shanyushiyangtech.top

Ruby: arr[1, 3]
来源：http://ltr.jinqigfzy.top

C#:   list.GetRange(1, 3);
来源：http://jnz.fehbvm.com

[D08] 合并两个数组
来源：http://ptx.fengsongda.top

Py:   a + b;  a.extend(b)
来源：http://wqb.zycfv.cn

PHP:  array_merge($a, $b);
来源：http://vck.vehdjk.com

JS:   [...a, ...b];  a.concat(b);
来源：http://agp.zhijiandao.cn

TS:   [...a, ...b];
来源：http://bzb.ehwqpu.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nqk.fengsongda.top

Go:   append(a, b...)
来源：http://ioo.epnwcf.com

Ruby: a + b;  a.concat(b)
来源：http://ysd.bjfxy.top

C#:   a.Concat(b).ToList()
来源：http://wms.redwolf501.top

[D09] 排序（升序）
来源：http://otc.cucudq.cn

Py:   sorted(arr);  arr.sort()
来源：http://sdv.316326.xyz

PHP:  sort($arr);
来源：http://vwy.meibo888.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dsv.mhx1999.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://snl.ctjpmb.com

Java: Collections.sort(list);  list.sort(null);
来源：http://jcd.chenzaomai.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vtu.guowangkeji.top

Ruby: arr.sort
来源：http://iln.fehbvm.com

C#:   list.Sort();
来源：http://row.tianlin.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://kqp.zhaomingkeji.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dft.feifeiyinyue.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gzn.ydjk.org.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hzg.sweek.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bxh.cucudq.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pfs.daria6918.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wtr.hongshengwenyu.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sng.yfazqb.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ggc.daria6918.cn

[D11] 反转数组
来源：http://bnx.iojbl.cn

Py:   arr[::-1];  arr.reverse()
来源：http://myp.tanke756.top

PHP:  array_reverse($arr);
来源：http://sud.tian-w.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lhk.fehbvm.com

TS:   [...arr].reverse();
来源：http://duz.tanke756.top

Java: Collections.reverse(list);
来源：http://zst.yj20258888.top

Go:   slices.Reverse(arr)
来源：http://gpd.jyoumei.cn

Ruby: arr.reverse
来源：http://tjy.vqdsnc.cn

C#:   list.Reverse();
来源：http://xuu.sysykeji.top

[D12] 查找元素下标
来源：http://kaj.zhoulong.xyz

Py:   arr.index(x);  x in arr
来源：http://gfp.quarkkingdee.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vab.fehbvm.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pgo.cdnleiting.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vxa.jqgfzy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kvd.zdqjudy.top

Go:   slices.Index(arr, x)
来源：http://qsa.zhoulong.xyz

Ruby: arr.index(x)
来源：http://mxm.daria6918.cn

C#:   list.IndexOf(x);
来源：http://fus.svipenyu.cn

[D13] 过滤（保留满足条件的）
来源：http://ggh.fehbvm.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lne.hnxiangtu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://uhj.hysaishi.cn

JS:   arr.filter(x => x > 3)
来源：http://ytn.0kj1m.cn

TS:   arr.filter(x => x > 3)
来源：http://fbk.zhaomingkeji.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tos.316326.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pyn.ydzc1.top

Ruby: arr.select { |x| x > 3 }
来源：http://mcx.jlsjyb.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://jfj.haohaochexian.top

[D14] 映射转换（每个元素变形）
来源：http://acb.tian-w.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://amd.xuetiantiany.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tbs.aibaodan.cn

JS:   arr.map(x => x * 2)
来源：http://bax.zhaomingkeji.xyz

TS:   arr.map(x => x * 2)
来源：http://qyi.vqdsnc.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://rkh.jyoumei.cn

Go:   // 手写循环
来源：http://apy.cucudq.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tqc.snrcjt.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rhn.yongpay.top

[D15] 去重
来源：http://vxa.hesvh.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tmx.mhx1999.top

PHP:  array_unique($arr);
来源：http://yfe.daxiang520.top

JS:   [...new Set(arr)]
来源：http://jmm.hnqzz.top

TS:   [...new Set(arr)]
来源：http://qab.yj20258.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://prk.jinyuanbaomall.cn

Go:   // 用 map[T]struct{} 手写
来源：http://eoj.zhijiandao.cn

Ruby: arr.uniq
来源：http://biq.birdmap.top

C#:   list.Distinct().ToList()
来源：http://zce.tianlin.xyz

[D16] 求和与平均值
来源：http://mzd.bjfxy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vjr.aibaodan.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rrg.wangdashe.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ari.haohaochexian.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vuv.kuanghao11.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jxl.wangshuangyany.cn

Go:   // 手写循环累加
来源：http://isv.fzhhl.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cet.yuxming.cn

C#:   list.Sum();  list.Average()
来源：http://smk.tianlin.xyz

[D17] 最大值与最小值
来源：http://nnq.hfpthk.cn

Py:   max(arr);  min(arr)
来源：http://xqo.zhixingplan.top

PHP:  max($arr);  min($arr);
来源：http://czq.zhixingplan.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lzx.hnxiangtu.top

TS:   Math.max(...arr);
来源：http://vci.zycfv.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ihf.tian-w.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pho.ydjk.org.cn

Ruby: arr.max;  arr.min
来源：http://qxr.smart0.xyz

C#:   list.Max();  list.Min()
来源：http://gda.tianlin.xyz

[D18] 扁平化嵌套数组
来源：http://kkd.fanxiaobao.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tom.ivvv.top

PHP:  array_merge(...$nested);
来源：http://sye.quarkkingdee.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://acc.epnwcf.com

TS:   nested.flat();
来源：http://ccu.tanke756.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xpc.shanyushiyangkeji.top

Go:   // 手写双层循环
来源：http://eip.cqqwz.cn

Ruby: nested.flatten
来源：http://eas.birdmap.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://mvp.hcnkem.com

[D19] 按字段分组
来源：http://ute.zhixingplan.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ogu.jlsjyb.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rnt.cqqwz.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bpr.jinyuanbaomall.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xfn.xuetiantiany.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tpd.yueranfly.top

Go:   // 手写 map[string][]T
来源：http://bhb.yj20258.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://xhn.zhengqikj.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://shl.zhoulong.xyz

[D20] 统计每个元素出现次数
来源：http://hav.mhx1999.top

Py:   Counter(arr)
来源：http://vor.tianlin.xyz

PHP:  array_count_values($arr);
来源：http://mkv.shanyushiyangkeji.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ofd.hongshengwenyu.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dyy.jinghuilouyu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://orv.nanxuanxn.top

Go:   // 手写 map[T]int
来源：http://che.wangshuangyany.cn

Ruby: arr.tally
来源：http://vrt.xuanzx.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://icl.smart0.xyz

[D21] 判断是否包含某元素
来源：http://ehk.yuxming.cn

Py:   x in arr
来源：http://qtu.birdmap.top

PHP:  in_array($x, $arr, true);
来源：http://ngs.xingfuxueyuan.xyz

JS:   arr.includes(x)
来源：http://ohn.aibaodan.cn

TS:   arr.includes(x)
来源：http://wxt.wangdashe.top

Java: list.contains(x)
来源：http://wgt.feifeiyinyue.top

Go:   slices.Contains(arr, x)
来源：http://nkh.nanxinkj.top

Ruby: arr.include?(x)
来源：http://smy.yuxming.cn

C#:   list.Contains(x)
来源：http://kff.sweek.top

[D22] 复制数组（避免共享引用）
来源：http://krs.dianchejie.cn


<!-- 参考信息 -->