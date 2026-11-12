代发 wailian999

Py:   return a, b
来源：http://ewa.gogol.net.cn

PHP:  return [$a, $b];
来源：http://fdw.ybcxt.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://aaw.aizwys.cn

TS:   return { a, b };
来源：http://htz.ywan-chungtsiang.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tnu.tarul.cn

Go:   return a, b
来源：http://onf.dianchejie.cn

Ruby: return a, b
来源：http://qyx.yueranfly.top

C#:   return (a, b);              // ValueTuple
来源：http://cwr.yangfankeji.com

[C06] 匿名函数 / lambda
来源：http://tgt.ivvv.top

Py:   square = lambda x: x * x
来源：http://ivl.jyoumei.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://uck.zhoulong.xyz

JS:   const square = x => x * x;
来源：http://eta.jinqigfzy.top

TS:   const square = (x: number): number => x * x;
来源：http://mdi.jiagoushi.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bgu.fengsongda.top

Go:   sq := func(x int) int { return x * x }
来源：http://yvq.fengsongda.top

Ruby: square = ->(x) { x * x }
来源：http://bou.daria6918.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qln.jianghu66.top

[C07] 把函数作为参数传入
来源：http://wda.guowangkeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ykk.shanyushiyangkeji.top

PHP:  array_map("strtoupper", $arr);
来源：http://cyk.fktsv.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tho.fktsv.cn

TS:   arr.map(String)
来源：http://plx.zhijiandao.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bpk.sweek.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xpp.wangdashe.top

Ruby: arr.map(&:upcase)
来源：http://yjs.hesvh.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ubg.gzhubu.top

[C08] 闭包
来源：http://tok.daria6918.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dql.uphjek.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jfw.shanyushiyangkeji.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://moa.jqgfzy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nye.jqgfzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xwy.bbcook.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vur.yj20258.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://she.vehdjk.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pxm.cdnleiting.top

[C09] 递归
来源：http://qmc.zhijiandao.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ubs.daria6918.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://iju.xingfuxueyuan.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zgl.guowangkeji.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wbj.cucudq.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ony.yj20258.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bkh.zdqjudy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tra.gogol.net.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://anu.ydzc1.top

[C10] 变量作用域
来源：http://tem.cqqwz.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://thi.cheryme.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xbm.zhaomingkeji.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yac.cucudq.cn

TS:   同 JS
来源：http://ahs.9152youxi.cn

Java: 方法内为块级作用域
来源：http://dsr.aizwys.cn

Go:   花括号块级作用域
来源：http://zpq.ehwqpu.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vha.sysykeji.top

C#:   块级作用域
来源：http://rzd.pycfn.com

[C11] 模块导入与导出
来源：http://esa.fzhhl.top

Py:   from module import func
来源：http://lds.ppjwa.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://yho.9152youxi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://cku.fengsongda.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xog.ybcxt.top

Java: import java.util.List;
来源：http://vvy.cqqwz.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lnd.cashguo.top

Ruby: require "json"; require_relative "./util"
来源：http://mae.vehdjk.com

C#:   using System.Text;
来源：http://zbg.wangshuangyany.cn

[C12] 立即执行函数 IIFE
来源：http://bek.zhiwuduotai.top

Py:   (lambda: print("run"))()
来源：http://wdb.fengsongda.top

PHP:  (function () { echo "run"; })();
来源：http://akn.yueranfly.top

JS:   (() => { console.log("run"); })();
来源：http://gxe.zhoulong.xyz

TS:   (() => { console.log("run"); })();
来源：http://dda.jqgfzy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xwq.zhixingplan.top

Go:   func() { fmt.Println("run") }()
来源：http://vgt.ehwqpu.com

Ruby: -> { puts "run" }.call
来源：http://owx.sxryk.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://euw.quarkkingdee.top

[C13] 类型声明 / 类型注解
来源：http://zap.tarul.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tkr.vehdjk.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nhf.sweek.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://imn.shanyushiyangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mgu.0kj1m.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cuf.sjlbkw.cn

Go:   func add(a, b int) int
来源：http://num.yj20258888.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vve.tarul.cn

C#:   int Add(int a, int b) => a + b;
来源：http://acl.hnxiangtu.top

[C14] 泛型函数
来源：http://isi.aizwys.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lwj.epnwcf.com

PHP:  // 无泛型
来源：http://rpz.jinqigfzy.top

JS:   // 无泛型
来源：http://lci.zhixingplan.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bpt.fanxiaobao.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ayf.ydzc1.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lbo.tarul.cn

Ruby: # 无泛型
来源：http://rai.yongpay.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jnp.aizwys.cn

[C15] 解构 / 展开参数
来源：http://gnw.uphjek.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rbx.iojbl.cn

PHP:  [$a, $b] = $pair;
来源：http://bgs.zdbjq.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hmk.hfpthk.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uyw.sufxvd.cn

Java: // 无解构
来源：http://zus.jianghu66.top

Go:   // 无解构
来源：http://pfq.0kj1m.cn

Ruby: a, b = pair
来源：http://nik.ydjk.org.cn

C#:   var (a, b) = pair;
来源：http://npp.tanke756.top

[C16] 函数 / 方法重载
来源：http://sat.hesvh.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://uwr.jinqigufen.top

PHP:  // 无重载
来源：http://vkn.hcnkem.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://aga.ppjwa.cn

TS:   // 用联合类型或重载签名声明
来源：http://cjw.haohaochexian.top

Java: void f(int a) {}  void f(String a) {}
来源：http://loe.chenjidiqi.icu

Go:   // 无重载：用不同函数名
来源：http://bwx.gzhubu.top

Ruby: # 无重载：靠动态参数
来源：http://avh.fengsongda.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://tuj.jqgfzy.top

================================================================================
来源：http://sho.meibo888.top

D. 数组 / 列表 / 集合
来源：http://fmq.xuetiantiany.cn

================================================================================
来源：http://jsi.ppjwa.cn

[D01] 创建数组 / 列表
来源：http://ruw.vehdjk.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://jbp.0kj1m.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://afj.tianlin.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jaz.cashguo.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://wch.guowangkeji.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pmy.hywenlv.cn

Go:   arr := []int{1, 2, 3}
来源：http://dmw.hnqzz.top

Ruby: arr = [1, 2, 3]
来源：http://ohu.yonumen.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://eue.xziqi.cn

[D02] 追加元素到末尾
来源：http://wih.yonumen.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://unj.cheryme.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dph.wangdashe.top

JS:   arr.push(4);
来源：http://vks.hesvh.cn

TS:   arr.push(4);
来源：http://hyw.jiagoushi.top

Java: list.add(4);
来源：http://hpg.havefunace.top

Go:   arr = append(arr, 4)
来源：http://fzy.yfazqb.com

Ruby: arr << 4; arr.push(5)
来源：http://ett.ywan-chungtsiang.top

C#:   list.Add(4);
来源：http://hed.chenlongwang.top

[D03] 在指定位置插入元素
来源：http://wtb.guannengcc.top

Py:   arr.insert(0, 0)
来源：http://pyx.gzhubu.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jni.haohaochexian.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lss.cheryme.top

TS:   arr.splice(0, 0, 0);
来源：http://ktg.dianchejie.cn

Java: list.add(0, 0);
来源：http://uty.hammf.cn

Go:   arr = append([]int{0}, arr...)
来源：http://nmp.nanxinkj.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gkm.sysykeji.top

C#:   list.Insert(0, 0);
来源：http://kst.haohaochexian.top

[D04] 删除元素
来源：http://pcm.gogol.net.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jlu.sweek.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://itm.yonumen.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kho.ctjpmb.com

TS:   arr.splice(0, 1);
来源：http://ccx.jianghu66.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pyg.sweek.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zgg.chenzaomai.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rux.zycfv.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fyx.yanxiufei.cn

[D05] 访问与修改元素
来源：http://bsx.ehwqpu.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ebz.xuanzx.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ieh.xuetiantiany.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dvb.zhongyouzk.top

TS:   arr[0]; arr.at(-1);
来源：http://jgw.dashuyun.cn

Java: list.get(0); list.set(0, 9);
来源：http://aik.yfazqb.com

Go:   arr[0]; arr[0] = 9
来源：http://xlj.52xcode.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wdy.sysykeji.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ljs.zycfv.cn

[D06] 数组长度
来源：http://jpm.hongshengwenyu.top

Py:   len(arr)
来源：http://xpn.zhengqikj.top

PHP:  count($arr);
来源：http://cyc.hesvh.cn

JS:   arr.length
来源：http://tcc.hesvh.cn

TS:   arr.length
来源：http://pdk.zhijiandao.cn

Java: list.size();
来源：http://wyg.aibaodan.cn

Go:   len(arr)
来源：http://mck.pengpengdd.cyou

Ruby: arr.length; arr.size
来源：http://uql.yanxiufei.cn

C#:   list.Count;
来源：http://ljl.jinyuanbaomall.cn

[D07] 切片 / 取子数组
来源：http://fbi.dashuyun.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gxp.vehdjk.com

PHP:  array_slice($arr, 1, 3);
来源：http://mra.zdqjudy.top

JS:   arr.slice(1, 4);
来源：http://jzq.ybcxt.top

TS:   arr.slice(1, 4);
来源：http://juo.yueranfly.top

Java: list.subList(1, 4);
来源：http://tud.fanxiaobao.xyz

Go:   arr[1:4]
来源：http://lbl.yj202588.top

Ruby: arr[1, 3]
来源：http://iai.xuetiantiany.cn

C#:   list.GetRange(1, 3);
来源：http://ylj.jlsjyb.cn

[D08] 合并两个数组
来源：http://new.yonumen.top

Py:   a + b;  a.extend(b)
来源：http://zsv.sweek.top

PHP:  array_merge($a, $b);
来源：http://cqi.xylfe.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ukj.zhongyouzk.top

TS:   [...a, ...b];
来源：http://mir.smart0.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://las.dashuyun.cn

Go:   append(a, b...)
来源：http://fme.tianlin.xyz

Ruby: a + b;  a.concat(b)
来源：http://nno.guannengcc.top

C#:   a.Concat(b).ToList()
来源：http://iut.cheryme.top

[D09] 排序（升序）
来源：http://ckf.sxryk.cn

Py:   sorted(arr);  arr.sort()
来源：http://ovg.gzhubu.top

PHP:  sort($arr);
来源：http://vuv.shuidangran.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://esn.hcnkem.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://ouv.316326.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://acl.bjfxy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jxu.cucudq.cn

Ruby: arr.sort
来源：http://mmk.cdnleiting.top

C#:   list.Sort();
来源：http://jtj.kuanghao11.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://iwm.yj202588.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wfw.guowangkeji.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yew.hywenlv.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fnf.cucudq.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mki.gogol.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mon.jianghu66.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kew.gaohongyu789.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://klc.yj20258.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yfw.hywenlv.cn

[D11] 反转数组
来源：http://aoe.epnwcf.com

Py:   arr[::-1];  arr.reverse()
来源：http://ymf.wangdashe.top

PHP:  array_reverse($arr);
来源：http://zwu.tianlin.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://acn.shanyushiyangtech.top

TS:   [...arr].reverse();
来源：http://vzp.xziqi.cn

Java: Collections.reverse(list);
来源：http://sqk.xziqi.cn

Go:   slices.Reverse(arr)
来源：http://flu.ivvv.top

Ruby: arr.reverse
来源：http://rwe.tanke756.top

C#:   list.Reverse();
来源：http://fgl.vqdsnc.cn

[D12] 查找元素下标
来源：http://sha.yueranfly.top

Py:   arr.index(x);  x in arr
来源：http://nss.shanyushiyangtech.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gwc.jqgfzy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://puq.jiagoushi.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fpu.uphjek.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dej.zhengqikj.top

Go:   slices.Index(arr, x)
来源：http://ikh.gzhubu.top

Ruby: arr.index(x)
来源：http://mft.tanke756.top

C#:   list.IndexOf(x);
来源：http://xqe.zhengqikj.top

[D13] 过滤（保留满足条件的）
来源：http://mtn.zhaomingkeji.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gns.yueranfly.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jfh.hcnkem.com

JS:   arr.filter(x => x > 3)
来源：http://cub.yj20258888.top

TS:   arr.filter(x => x > 3)
来源：http://avr.jyoumei.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://txl.birdmap.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jjw.52xcode.cn

Ruby: arr.select { |x| x > 3 }
来源：http://zkd.wangdashe.top

C#:   list.Where(x => x > 3).ToList()
来源：http://epv.fehbvm.com

[D14] 映射转换（每个元素变形）
来源：http://krw.snrcjt.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xte.9152youxi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ryz.jianghu66.top

JS:   arr.map(x => x * 2)
来源：http://cyr.yuxming.cn

TS:   arr.map(x => x * 2)
来源：http://yaq.jinyuanbaomall.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ytx.hcnkem.com

Go:   // 手写循环
来源：http://bbg.yongpay.top

Ruby: arr.map { |x| x * 2 }
来源：http://ejo.tianlin.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://hnr.yj20258888.top

[D15] 去重
来源：http://bkd.yongpay.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gqv.wangdashe.top

PHP:  array_unique($arr);
来源：http://maa.hammf.cn

JS:   [...new Set(arr)]
来源：http://mvq.xingfuxueyuan.xyz

TS:   [...new Set(arr)]
来源：http://ace.cucudq.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lpg.wangdashe.top

Go:   // 用 map[T]struct{} 手写
来源：http://nvt.smart0.xyz

Ruby: arr.uniq
来源：http://wtb.gzhubu.top

C#:   list.Distinct().ToList()
来源：http://wih.iojbl.cn

[D16] 求和与平均值
来源：http://sjj.mhx1999.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lwf.zhiwuduotai.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wgr.mhx1999.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ppp.bjfxy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kim.ctjpmb.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mwt.andypj.xyz

Go:   // 手写循环累加
来源：http://sqf.cashguo.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uav.pycfn.com

C#:   list.Sum();  list.Average()
来源：http://cgd.shanyushiyangtech.top

[D17] 最大值与最小值
来源：http://cxl.yueranfly.top

Py:   max(arr);  min(arr)
来源：http://hmo.guowangkeji.top

PHP:  max($arr);  min($arr);
来源：http://ibs.redwolf501.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rlj.birdmap.top

TS:   Math.max(...arr);
来源：http://rru.wangshuangyany.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bsv.xylfe.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bsd.tanke756.top

Ruby: arr.max;  arr.min
来源：http://vjx.xinyue.icu

C#:   list.Max();  list.Min()
来源：http://pxd.gogol.net.cn

[D18] 扁平化嵌套数组
来源：http://bun.tianlin.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xtu.vqdsnc.cn

PHP:  array_merge(...$nested);
来源：http://hmc.c1oappe.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ldg.hesvh.cn

TS:   nested.flat();
来源：http://ugw.wangdashe.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://iid.yvedp.cn

Go:   // 手写双层循环
来源：http://izn.kuanghao11.cn

Ruby: nested.flatten
来源：http://xjq.zycfv.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://gdn.jinghuilouyu.cn

[D19] 按字段分组
来源：http://fzw.jlsjyb.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kmx.jinqigufen.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rjc.jinqigufen.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qdm.tian-w.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://gyo.xziqi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gdj.hysaishi.cn

Go:   // 手写 map[string][]T
来源：http://jsn.jinghuilouyu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jdo.shangyingyoupin.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bwz.hesvh.cn

[D20] 统计每个元素出现次数
来源：http://tgd.xingfuxueyuan.xyz

Py:   Counter(arr)
来源：http://ecu.cucudq.cn

PHP:  array_count_values($arr);
来源：http://flj.svipenyu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eyf.jinqigufen.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ntb.jinqigfzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lzt.tanke756.top

Go:   // 手写 map[T]int
来源：http://vms.snrcjt.cn

Ruby: arr.tally
来源：http://ctg.yangfankeji.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mtv.sufxvd.cn

[D21] 判断是否包含某元素
来源：http://bbv.chenzaomai.com

Py:   x in arr
来源：http://exs.iojbl.cn

PHP:  in_array($x, $arr, true);
来源：http://gfx.meibo888.top

JS:   arr.includes(x)
来源：http://lrf.daxiang520.top

TS:   arr.includes(x)
来源：http://xoi.jinqigufen.top

Java: list.contains(x)
来源：http://lee.smart0.xyz

Go:   slices.Contains(arr, x)
来源：http://zkm.aibaodan.cn

Ruby: arr.include?(x)
来源：http://ews.aibaodan.cn

C#:   list.Contains(x)
来源：http://irt.zycfv.cn

[D22] 复制数组（避免共享引用）
来源：http://meh.birdmap.top


<!-- 参考信息 -->