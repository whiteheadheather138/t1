代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://pwj.nwbrower.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pck.sufxvd.cn

[C04] 命名参数 / 关键字参数
来源：http://hwj.shuidangran.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ves.shanyushiyangtech.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kyd.jinqigfzy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jno.jinqigufen.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qsf.zycfv.cn

Java: // 无：用 Builder 模式或 record
来源：http://vyx.haohaochexian.top

Go:   // 无：用配置结构体参数
来源：http://mzh.nanxuanxn.top

Ruby: f(a: 1, b: 2)
来源：http://jdv.zhoulong.xyz

C#:   f(a: 1, b: 2)
来源：http://frk.hysaishi.cn

[C05] 返回多个值
来源：http://xoc.dianchejie.cn

Py:   return a, b
来源：http://pem.ivvv.top

PHP:  return [$a, $b];
来源：http://aiv.hesvh.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://lvq.hywenlv.cn

TS:   return { a, b };
来源：http://dvj.xuanzx.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ogj.yongpay.top

Go:   return a, b
来源：http://odf.gogol.net.cn

Ruby: return a, b
来源：http://xis.tarul.cn

C#:   return (a, b);              // ValueTuple
来源：http://jhu.yanxiufei.cn

[C06] 匿名函数 / lambda
来源：http://bij.ydjk.org.cn

Py:   square = lambda x: x * x
来源：http://eru.svipenyu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ize.nwbrower.top

JS:   const square = x => x * x;
来源：http://jzk.52xcode.cn

TS:   const square = (x: number): number => x * x;
来源：http://lww.snrcjt.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wsa.haohaochexian.top

Go:   sq := func(x int) int { return x * x }
来源：http://ryi.nwbrower.top

Ruby: square = ->(x) { x * x }
来源：http://jmw.vehdjk.com

C#:   Func<int, int> square = x => x * x;
来源：http://elm.redwolf501.top

[C07] 把函数作为参数传入
来源：http://qsd.pengpengdd.cyou

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mhe.haohaochexian.top

PHP:  array_map("strtoupper", $arr);
来源：http://mkf.haohaochexian.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gje.zycfv.cn

TS:   arr.map(String)
来源：http://xyi.sufxvd.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://suj.bbcook.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xwa.jqgufenzy.top

Ruby: arr.map(&:upcase)
来源：http://dgy.cucudq.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hlp.tian-w.cn

[C08] 闭包
来源：http://usr.xziqi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dgb.0kj1m.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mhg.zhongyouzk.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://khm.svipenyu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wnf.kuanghao11.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nmq.mhx1999.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ohi.zhixingplan.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uua.tanke756.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yyv.yuanzhike.top

[C09] 递归
来源：http://nbj.cqqwz.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fwn.fktsv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://iar.haohaochexian.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eke.shangyingyoupin.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zar.meibo888.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://eky.xingfuxueyuan.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gwk.gogol.net.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hiv.fengsongda.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kqc.hesvh.cn

[C10] 变量作用域
来源：http://fgc.nwbrower.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ncq.ydjk.org.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://paq.yvedp.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nbo.hywenlv.cn

TS:   同 JS
来源：http://val.sweek.top

Java: 方法内为块级作用域
来源：http://wqg.ydzc1.top

Go:   花括号块级作用域
来源：http://sdb.ppjwa.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xsy.yj202588.top

C#:   块级作用域
来源：http://uzt.52xcode.cn

[C11] 模块导入与导出
来源：http://uez.nanxuanxn.top

Py:   from module import func
来源：http://uqp.kuanghao11.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rfj.yongpay.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ble.mhx1999.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gcq.yvedp.cn

Java: import java.util.List;
来源：http://blx.pycfn.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rid.tian-w.cn

Ruby: require "json"; require_relative "./util"
来源：http://cmv.hysaishi.cn

C#:   using System.Text;
来源：http://kgr.ydjk.org.cn

[C12] 立即执行函数 IIFE
来源：http://mni.tanke756.top

Py:   (lambda: print("run"))()
来源：http://poy.tian-w.cn

PHP:  (function () { echo "run"; })();
来源：http://ogq.yj20258888.top

JS:   (() => { console.log("run"); })();
来源：http://kot.c1oappe.top

TS:   (() => { console.log("run"); })();
来源：http://ixq.dianchejie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gqk.ehwqpu.com

Go:   func() { fmt.Println("run") }()
来源：http://ovg.fengsongda.top

Ruby: -> { puts "run" }.call
来源：http://dhk.epnwcf.com

C#:   // 无 IIFE：用静态构造函数
来源：http://kks.xylfe.cn

[C13] 类型声明 / 类型注解
来源：http://zsn.yuanzhike.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gfg.daxiang520.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://goz.hnxiangtu.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xkw.chenjidiqi.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zjy.shuidangran.top

Java: int add(int a, int b) { return a + b; }
来源：http://ioy.uphjek.com

Go:   func add(a, b int) int
来源：http://duu.jinqigfzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tot.vehdjk.com

C#:   int Add(int a, int b) => a + b;
来源：http://exh.jqgufenzy.top

[C14] 泛型函数
来源：http://wml.gzhubu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://igv.sjlbkw.cn

PHP:  // 无泛型
来源：http://bhx.zdqjudy.top

JS:   // 无泛型
来源：http://koo.chenzaomai.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sge.gotoacloud.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dxr.smart0.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://llm.shanyushiyangtech.top

Ruby: # 无泛型
来源：http://wco.jinqigfzy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fhv.fanxiaobao.xyz

[C15] 解构 / 展开参数
来源：http://ggx.redwolf501.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qfw.svipenyu.cn

PHP:  [$a, $b] = $pair;
来源：http://caq.ywan-chungtsiang.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nif.tianlin.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zwn.316326.xyz

Java: // 无解构
来源：http://kng.jqgufenzy.top

Go:   // 无解构
来源：http://cet.nanxinkj.top

Ruby: a, b = pair
来源：http://beb.jyoumei.cn

C#:   var (a, b) = pair;
来源：http://kuo.jiagoushi.top

[C16] 函数 / 方法重载
来源：http://iqm.ehwqpu.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://orq.xingfuxueyuan.xyz

PHP:  // 无重载
来源：http://bct.cdnleiting.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://cqg.guowangkeji.top

TS:   // 用联合类型或重载签名声明
来源：http://egd.nanxuanxn.top

Java: void f(int a) {}  void f(String a) {}
来源：http://nxg.cdnleiting.top

Go:   // 无重载：用不同函数名
来源：http://ibl.epnwcf.com

Ruby: # 无重载：靠动态参数
来源：http://ryy.havefunace.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://tvg.jinqigfzy.top

================================================================================
来源：http://rnq.gaohongyu789.top

D. 数组 / 列表 / 集合
来源：http://jrb.cdnleiting.top

================================================================================
来源：http://uib.sysykeji.top

[D01] 创建数组 / 列表
来源：http://gkh.nwbrower.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://sgu.haohaochexian.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://det.jqgufenzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://drz.hywenlv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kvg.fanxiaobao.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sjt.tanke756.top

Go:   arr := []int{1, 2, 3}
来源：http://zvx.hnxiangtu.top

Ruby: arr = [1, 2, 3]
来源：http://ywn.fengsongda.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://erg.cqqwz.cn

[D02] 追加元素到末尾
来源：http://acg.zhijiandao.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dts.tarul.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hxv.mhx1999.top

JS:   arr.push(4);
来源：http://dtk.zhengqikj.top

TS:   arr.push(4);
来源：http://ida.yueranfly.top

Java: list.add(4);
来源：http://zoc.ywan-chungtsiang.top

Go:   arr = append(arr, 4)
来源：http://kbj.c1oappe.top

Ruby: arr << 4; arr.push(5)
来源：http://hnh.pycfn.com

C#:   list.Add(4);
来源：http://jbp.zhoulong.xyz

[D03] 在指定位置插入元素
来源：http://fry.hongshengwenyu.top

Py:   arr.insert(0, 0)
来源：http://fbe.guowangkeji.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jmu.jqgufenzy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bnm.smart0.xyz

TS:   arr.splice(0, 0, 0);
来源：http://yis.9152youxi.cn

Java: list.add(0, 0);
来源：http://czy.hcnkem.com

Go:   arr = append([]int{0}, arr...)
来源：http://pzr.pycfn.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lxj.yj202588.top

C#:   list.Insert(0, 0);
来源：http://wha.yj202588.top

[D04] 删除元素
来源：http://phi.shanyushiyangtech.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uyk.tarul.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fty.pengpengdd.cyou

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uav.ppjwa.cn

TS:   arr.splice(0, 1);
来源：http://kiu.cucudq.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cul.jqgufenzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tji.zhijiandao.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://aih.ppjwa.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mis.gotoacloud.top

[D05] 访问与修改元素
来源：http://cwp.svipenyu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dbg.havefunace.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wwg.hysaishi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://aig.52xcode.cn

TS:   arr[0]; arr.at(-1);
来源：http://ajm.snrcjt.cn

Java: list.get(0); list.set(0, 9);
来源：http://jlk.svipenyu.cn

Go:   arr[0]; arr[0] = 9
来源：http://pgz.c1oappe.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://meq.hfpthk.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wsz.yueranfly.top

[D06] 数组长度
来源：http://ljn.hammf.cn

Py:   len(arr)
来源：http://xqe.cucudq.cn

PHP:  count($arr);
来源：http://sae.vehdjk.com

JS:   arr.length
来源：http://swi.jianghu66.top

TS:   arr.length
来源：http://tkr.xuetiantiany.cn

Java: list.size();
来源：http://shk.hammf.cn

Go:   len(arr)
来源：http://wip.ehwqpu.com

Ruby: arr.length; arr.size
来源：http://cpx.zhiwuduotai.top

C#:   list.Count;
来源：http://jza.xylfe.cn

[D07] 切片 / 取子数组
来源：http://rme.cheryme.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ctn.yj20258888.top

PHP:  array_slice($arr, 1, 3);
来源：http://crv.jyoumei.cn

JS:   arr.slice(1, 4);
来源：http://uaj.zdbjq.cn

TS:   arr.slice(1, 4);
来源：http://ukh.ctjpmb.com

Java: list.subList(1, 4);
来源：http://syt.cucudq.cn

Go:   arr[1:4]
来源：http://egx.shanyushiyangtech.top

Ruby: arr[1, 3]
来源：http://uzb.ivvv.top

C#:   list.GetRange(1, 3);
来源：http://kof.yanxiufei.cn

[D08] 合并两个数组
来源：http://eoi.sysykeji.top

Py:   a + b;  a.extend(b)
来源：http://dzw.tianlin.xyz

PHP:  array_merge($a, $b);
来源：http://ees.sufxvd.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ktm.jianghu66.top

TS:   [...a, ...b];
来源：http://iuw.ywan-chungtsiang.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fft.vehdjk.com

Go:   append(a, b...)
来源：http://wtj.ehwqpu.com

Ruby: a + b;  a.concat(b)
来源：http://fyx.chenlongwang.top

C#:   a.Concat(b).ToList()
来源：http://lib.guannengcc.top

[D09] 排序（升序）
来源：http://ecl.hysaishi.cn

Py:   sorted(arr);  arr.sort()
来源：http://uvs.havefunace.top

PHP:  sort($arr);
来源：http://qtx.birdmap.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://oaw.sweek.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://yjq.yongpay.top

Java: Collections.sort(list);  list.sort(null);
来源：http://afj.feifeiyinyue.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://otc.pengpengdd.cyou

Ruby: arr.sort
来源：http://nqp.vehdjk.com

C#:   list.Sort();
来源：http://ptp.andypj.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://znc.sweek.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cbg.yangfankeji.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://drk.zycfv.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ffr.ctjpmb.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fnc.haohaochexian.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kwk.cqqwz.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://prf.c1oappe.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xvd.nanxuanxn.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ywy.birdmap.top

[D11] 反转数组
来源：http://gnc.jiagoushi.top

Py:   arr[::-1];  arr.reverse()
来源：http://wza.shangyingyoupin.top

PHP:  array_reverse($arr);
来源：http://ofa.zhijiandao.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tgq.aizwys.cn

TS:   [...arr].reverse();
来源：http://auv.yuanzhike.top

Java: Collections.reverse(list);
来源：http://ado.zdqjudy.top

Go:   slices.Reverse(arr)
来源：http://ijn.hnxiangtu.top

Ruby: arr.reverse
来源：http://kln.aibaodan.cn

C#:   list.Reverse();
来源：http://ovo.dashuyun.cn

[D12] 查找元素下标
来源：http://tew.nanxuanxn.top

Py:   arr.index(x);  x in arr
来源：http://krs.zdbjq.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nvj.fzhhl.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://scy.0kj1m.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cnz.pengpengdd.cyou

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pop.epnwcf.com

Go:   slices.Index(arr, x)
来源：http://ufr.yueranfly.top

Ruby: arr.index(x)
来源：http://eyz.shanyushiyangtech.top

C#:   list.IndexOf(x);
来源：http://wxj.zhijiandao.cn

[D13] 过滤（保留满足条件的）
来源：http://kkq.fzhhl.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hct.redwolf501.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gxr.iojbl.cn

JS:   arr.filter(x => x > 3)
来源：http://hoq.zhongyouzk.top

TS:   arr.filter(x => x > 3)
来源：http://qma.zdbjq.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mua.feifeiyinyue.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kfk.9152youxi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hgz.xziqi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hoj.vehdjk.com

[D14] 映射转换（每个元素变形）
来源：http://jry.0kj1m.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uhn.guowangkeji.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dil.yj20258.top

JS:   arr.map(x => x * 2)
来源：http://ksd.xinyue.icu

TS:   arr.map(x => x * 2)
来源：http://cot.hongshengwenyu.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ccr.fanxiaobao.xyz

Go:   // 手写循环
来源：http://uzh.fanxiaobao.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://clh.hnxiangtu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://mue.cqqwz.cn

[D15] 去重
来源：http://xzb.chenlongwang.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://byf.daria6918.cn

PHP:  array_unique($arr);
来源：http://mkg.hcnkem.com

JS:   [...new Set(arr)]
来源：http://hmt.vehdjk.com

TS:   [...new Set(arr)]
来源：http://veh.guowangkeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mbl.mhx1999.top

Go:   // 用 map[T]struct{} 手写
来源：http://cld.shangyingyoupin.top

Ruby: arr.uniq
来源：http://zen.sjlbkw.cn

C#:   list.Distinct().ToList()
来源：http://hio.shuidangran.top

[D16] 求和与平均值
来源：http://msj.shuidangran.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://iwx.zhaomingkeji.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://oik.hysaishi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xgc.zdqjudy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qpz.yanxiufei.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://skh.sysykeji.top

Go:   // 手写循环累加
来源：http://bae.xziqi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lmq.nwbrower.top

C#:   list.Sum();  list.Average()
来源：http://rlb.0kj1m.cn

[D17] 最大值与最小值
来源：http://ufj.yangfankeji.com

Py:   max(arr);  min(arr)
来源：http://hwn.fktsv.cn

PHP:  max($arr);  min($arr);
来源：http://kis.zhaomingkeji.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tlk.sufxvd.cn

TS:   Math.max(...arr);
来源：http://fya.gzhubu.top

Java: Collections.max(list);  Collections.min(list);
来源：http://rov.ehwqpu.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://thw.fehbvm.com

Ruby: arr.max;  arr.min
来源：http://ugx.yongpay.top

C#:   list.Max();  list.Min()
来源：http://xxl.chenjidiqi.icu

[D18] 扁平化嵌套数组
来源：http://qmg.yj202588.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rdp.fzhhl.top

PHP:  array_merge(...$nested);
来源：http://mvv.yongpay.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://edw.hammf.cn

TS:   nested.flat();
来源：http://mrp.birdmap.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tpf.ybcxt.top

Go:   // 手写双层循环
来源：http://tlk.wangshuangyany.cn

Ruby: nested.flatten
来源：http://bfw.xingfuxueyuan.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://nxx.xziqi.cn

[D19] 按字段分组
来源：http://cpm.fehbvm.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://iax.52xcode.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://czf.vqdsnc.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gmf.sysykeji.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://crx.jinqigfzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ahn.guannengcc.top

Go:   // 手写 map[string][]T
来源：http://zwv.chenzaomai.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://wsi.cashguo.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wiw.quarkkingdee.top

[D20] 统计每个元素出现次数
来源：http://fxu.yvedp.cn

Py:   Counter(arr)
来源：http://lll.hysaishi.cn

PHP:  array_count_values($arr);
来源：http://xhr.jiagoushi.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xcc.fehbvm.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rxm.hfpthk.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://caw.fanxiaobao.xyz

Go:   // 手写 map[T]int
来源：http://wpg.zdbjq.cn


<!-- 参考信息 -->