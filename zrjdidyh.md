代发 wailian999

Py:   return a, b
来源：http://iif.yj20258.top

PHP:  return [$a, $b];
来源：http://ygn.yongpay.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://fbe.chenlongwang.top

TS:   return { a, b };
来源：http://hwe.hnxiangtu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kxh.redwolf501.top

Go:   return a, b
来源：http://afp.xingfuxueyuan.xyz

Ruby: return a, b
来源：http://xup.zhengqikj.top

C#:   return (a, b);              // ValueTuple
来源：http://idu.cqqwz.cn

[C06] 匿名函数 / lambda
来源：http://fvu.pengpengdd.cyou

Py:   square = lambda x: x * x
来源：http://diu.cdnleiting.top

PHP:  $square = fn($x) => $x * $x;
来源：http://cgu.tarul.cn

JS:   const square = x => x * x;
来源：http://yxh.xuanzx.com

TS:   const square = (x: number): number => x * x;
来源：http://iuw.uphjek.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yad.hcnkem.com

Go:   sq := func(x int) int { return x * x }
来源：http://xnb.jiagoushi.top

Ruby: square = ->(x) { x * x }
来源：http://vpf.yj20258888.top

C#:   Func<int, int> square = x => x * x;
来源：http://oji.fehbvm.com

[C07] 把函数作为参数传入
来源：http://xvz.xinyue.icu

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ovn.yonumen.top

PHP:  array_map("strtoupper", $arr);
来源：http://zrp.ppjwa.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://giv.gzhubu.top

TS:   arr.map(String)
来源：http://dlx.jiagoushi.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kst.havefunace.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://oor.gaohongyu789.top

Ruby: arr.map(&:upcase)
来源：http://vph.fzhhl.top

C#:   arr.Select(s => s.ToUpper())
来源：http://czv.sxryk.cn

[C08] 闭包
来源：http://jsv.ppjwa.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uzk.hongshengwenyu.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kgz.kuanghao11.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cuc.daxiang520.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ttq.hfpthk.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://eua.xinyue.icu

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blp.hnqzz.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mdx.wangdashe.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wbq.tian-w.cn

[C09] 递归
来源：http://auf.tian-w.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://oto.hnxiangtu.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ioe.yj202588.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hfl.hnqzz.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://riu.dianchejie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xdx.nwbrower.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uvq.feifeiyinyue.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gpd.cqqwz.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kwp.sweek.top

[C10] 变量作用域
来源：http://udm.feifeiyinyue.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ute.haohaochexian.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nfi.shanyushiyangtech.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kmv.epnwcf.com

TS:   同 JS
来源：http://kce.cashguo.top

Java: 方法内为块级作用域
来源：http://erw.xingfuxueyuan.xyz

Go:   花括号块级作用域
来源：http://fkk.yanxiufei.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xma.mhx1999.top

C#:   块级作用域
来源：http://apc.zdqjudy.top

[C11] 模块导入与导出
来源：http://odx.zhoulong.xyz

Py:   from module import func
来源：http://cjr.tianlin.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://qtt.wangdashe.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://fqu.chenjidiqi.icu

TS:   export function f(): void {};  import { f } from "./m";
来源：http://agp.hammf.cn

Java: import java.util.List;
来源：http://wdb.zycfv.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wkb.daria6918.cn

Ruby: require "json"; require_relative "./util"
来源：http://rqa.havefunace.top

C#:   using System.Text;
来源：http://egl.zhengqikj.top

[C12] 立即执行函数 IIFE
来源：http://tez.fzhhl.top

Py:   (lambda: print("run"))()
来源：http://akn.guowangkeji.top

PHP:  (function () { echo "run"; })();
来源：http://omz.guannengcc.top

JS:   (() => { console.log("run"); })();
来源：http://nme.nanxinkj.top

TS:   (() => { console.log("run"); })();
来源：http://yew.snrcjt.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wfq.yj20258.top

Go:   func() { fmt.Println("run") }()
来源：http://whn.iojbl.cn

Ruby: -> { puts "run" }.call
来源：http://ifw.hysaishi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zji.yj20258888.top

[C13] 类型声明 / 类型注解
来源：http://wpi.yj202588.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://has.mhx1999.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://adc.ydjk.org.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gnh.9152youxi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jnq.fanxiaobao.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://bzq.hammf.cn

Go:   func add(a, b int) int
来源：http://cpv.xylfe.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yjg.nanxuanxn.top

C#:   int Add(int a, int b) => a + b;
来源：http://qam.sjlbkw.cn

[C14] 泛型函数
来源：http://eyq.sxryk.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rpt.tian-w.cn

PHP:  // 无泛型
来源：http://ghh.pengpengdd.cyou

JS:   // 无泛型
来源：http://vlq.zhijiandao.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://euy.mhx1999.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wfo.xinyue.icu

Go:   func First[T any](items []T) T { return items[0] }
来源：http://uaf.jlsjyb.cn

Ruby: # 无泛型
来源：http://kum.jinyuanbaomall.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qaz.tanke756.top

[C15] 解构 / 展开参数
来源：http://buk.pycfn.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://clu.shangyingyoupin.top

PHP:  [$a, $b] = $pair;
来源：http://vtf.dashuyun.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://npd.nwbrower.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://paq.hysaishi.cn

Java: // 无解构
来源：http://cdl.xuanzx.com

Go:   // 无解构
来源：http://jhx.xuetiantiany.cn

Ruby: a, b = pair
来源：http://vgf.hywenlv.cn

C#:   var (a, b) = pair;
来源：http://qdy.cqqwz.cn

[C16] 函数 / 方法重载
来源：http://ckm.hnqzz.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://odm.yj202588.top

PHP:  // 无重载
来源：http://cqq.sysykeji.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://yog.tanke756.top

TS:   // 用联合类型或重载签名声明
来源：http://yvx.fzhhl.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ngp.tianlin.xyz

Go:   // 无重载：用不同函数名
来源：http://cnc.jinqigufen.top

Ruby: # 无重载：靠动态参数
来源：http://ybp.guowangkeji.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ylz.andypj.xyz

================================================================================
来源：http://ljv.nanxuanxn.top

D. 数组 / 列表 / 集合
来源：http://flg.jinqigfzy.top

================================================================================
来源：http://mzr.yuxming.cn

[D01] 创建数组 / 列表
来源：http://tiw.jinqigfzy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://vqs.smart0.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://egr.ivvv.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hvm.jinqigfzy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://uud.meibo888.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wks.fengsongda.top

Go:   arr := []int{1, 2, 3}
来源：http://opy.aibaodan.cn

Ruby: arr = [1, 2, 3]
来源：http://bhh.tanke756.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wnm.hammf.cn

[D02] 追加元素到末尾
来源：http://zta.hammf.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yrf.cqqwz.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lbj.gotoacloud.top

JS:   arr.push(4);
来源：http://ibo.mhx1999.top

TS:   arr.push(4);
来源：http://dlw.yj20258.top

Java: list.add(4);
来源：http://nxq.xinyue.icu

Go:   arr = append(arr, 4)
来源：http://nvd.ydzc1.top

Ruby: arr << 4; arr.push(5)
来源：http://jpy.ppjwa.cn

C#:   list.Add(4);
来源：http://cco.gotoacloud.top

[D03] 在指定位置插入元素
来源：http://dcv.hywenlv.cn

Py:   arr.insert(0, 0)
来源：http://nmb.yongpay.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vdc.bbcook.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zem.andypj.xyz

TS:   arr.splice(0, 0, 0);
来源：http://dfi.cqqwz.cn

Java: list.add(0, 0);
来源：http://dev.aibaodan.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qus.fzhhl.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sws.bjfxy.top

C#:   list.Insert(0, 0);
来源：http://woa.epnwcf.com

[D04] 删除元素
来源：http://nkz.sxryk.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kwh.zhaomingkeji.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://miq.fanxiaobao.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mgs.haohaochexian.top

TS:   arr.splice(0, 1);
来源：http://emv.0kj1m.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jjd.ehwqpu.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://riv.jlsjyb.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://msg.meibo888.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://oir.shanyushiyangkeji.top

[D05] 访问与修改元素
来源：http://coj.nanxuanxn.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://svb.hcnkem.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gip.ydzc1.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dum.meibo888.top

TS:   arr[0]; arr.at(-1);
来源：http://nar.fanxiaobao.xyz

Java: list.get(0); list.set(0, 9);
来源：http://ayv.smart0.xyz

Go:   arr[0]; arr[0] = 9
来源：http://nwo.0kj1m.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://snu.yonumen.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bmt.guowangkeji.top

[D06] 数组长度
来源：http://ijn.guannengcc.top

Py:   len(arr)
来源：http://nhm.tarul.cn

PHP:  count($arr);
来源：http://ijz.aizwys.cn

JS:   arr.length
来源：http://yzr.redwolf501.top

TS:   arr.length
来源：http://kya.fehbvm.com

Java: list.size();
来源：http://lft.hnxiangtu.top

Go:   len(arr)
来源：http://iav.wangshuangyany.cn

Ruby: arr.length; arr.size
来源：http://pir.0kj1m.cn

C#:   list.Count;
来源：http://wri.bbcook.cn

[D07] 切片 / 取子数组
来源：http://jkj.yfazqb.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sct.zhijiandao.cn

PHP:  array_slice($arr, 1, 3);
来源：http://tar.jyoumei.cn

JS:   arr.slice(1, 4);
来源：http://coi.shanyushiyangkeji.top

TS:   arr.slice(1, 4);
来源：http://rrd.tianlin.xyz

Java: list.subList(1, 4);
来源：http://arm.dianchejie.cn

Go:   arr[1:4]
来源：http://nyw.ppjwa.cn

Ruby: arr[1, 3]
来源：http://hnk.jianghu66.top

C#:   list.GetRange(1, 3);
来源：http://xud.jinghuilouyu.cn

[D08] 合并两个数组
来源：http://eav.yfazqb.com

Py:   a + b;  a.extend(b)
来源：http://bwu.daria6918.cn

PHP:  array_merge($a, $b);
来源：http://bvp.fzhhl.top

JS:   [...a, ...b];  a.concat(b);
来源：http://hjt.chenlongwang.top

TS:   [...a, ...b];
来源：http://qyb.c1oappe.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nlz.jianghu66.top

Go:   append(a, b...)
来源：http://sww.fzhhl.top

Ruby: a + b;  a.concat(b)
来源：http://ueg.aibaodan.cn

C#:   a.Concat(b).ToList()
来源：http://igp.iojbl.cn

[D09] 排序（升序）
来源：http://nza.52xcode.cn

Py:   sorted(arr);  arr.sort()
来源：http://lpj.xingfuxueyuan.xyz

PHP:  sort($arr);
来源：http://wnm.chenzaomai.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://clf.tarul.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://aft.0kj1m.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://lcj.yonumen.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lxc.yj20258888.top

Ruby: arr.sort
来源：http://uba.ydjk.org.cn

C#:   list.Sort();
来源：http://koq.hongshengwenyu.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://qaw.xuetiantiany.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://djq.shangyingyoupin.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dsl.ydzc1.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hgr.epnwcf.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fns.sjlbkw.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lig.wangdashe.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zce.nwbrower.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tyy.snrcjt.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qjf.hongshengwenyu.top

[D11] 反转数组
来源：http://yuq.nanxinkj.top

Py:   arr[::-1];  arr.reverse()
来源：http://xbi.xylfe.cn

PHP:  array_reverse($arr);
来源：http://zfd.shangyingyoupin.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mrf.haohaochexian.top

TS:   [...arr].reverse();
来源：http://hpr.wangdashe.top

Java: Collections.reverse(list);
来源：http://aaq.shangyingyoupin.top

Go:   slices.Reverse(arr)
来源：http://kzm.zycfv.cn

Ruby: arr.reverse
来源：http://wez.vehdjk.com

C#:   list.Reverse();
来源：http://hxd.jinyuanbaomall.cn

[D12] 查找元素下标
来源：http://buu.zhijiandao.cn

Py:   arr.index(x);  x in arr
来源：http://akc.nanxuanxn.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pbz.pengpengdd.cyou

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hkp.yj202588.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ift.52xcode.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://whp.sxryk.cn

Go:   slices.Index(arr, x)
来源：http://thx.pengpengdd.cyou

Ruby: arr.index(x)
来源：http://ywh.hammf.cn

C#:   list.IndexOf(x);
来源：http://gmx.zhengqikj.top

[D13] 过滤（保留满足条件的）
来源：http://aye.hysaishi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tvg.tianlin.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fco.chenzaomai.com

JS:   arr.filter(x => x > 3)
来源：http://the.gzhubu.top

TS:   arr.filter(x => x > 3)
来源：http://sbn.feifeiyinyue.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rsg.yvedp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tbz.redwolf501.top

Ruby: arr.select { |x| x > 3 }
来源：http://srp.sufxvd.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://odr.shzxlz.cn

[D14] 映射转换（每个元素变形）
来源：http://jkh.dashuyun.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ygb.hnxiangtu.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ngz.vehdjk.com

JS:   arr.map(x => x * 2)
来源：http://vtw.xingfuxueyuan.xyz

TS:   arr.map(x => x * 2)
来源：http://tbf.zhongyouzk.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://juo.zhijiandao.cn

Go:   // 手写循环
来源：http://zlj.hnxiangtu.top

Ruby: arr.map { |x| x * 2 }
来源：http://stg.316326.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://vco.pengpengdd.cyou

[D15] 去重
来源：http://kmj.zhiwuduotai.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://aeo.zhixingplan.top

PHP:  array_unique($arr);
来源：http://zow.gotoacloud.top

JS:   [...new Set(arr)]
来源：http://aed.yfazqb.com

TS:   [...new Set(arr)]
来源：http://ybc.pengpengdd.cyou

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gqe.gotoacloud.top

Go:   // 用 map[T]struct{} 手写
来源：http://dvx.hnqzz.top

Ruby: arr.uniq
来源：http://amf.cheryme.top

C#:   list.Distinct().ToList()
来源：http://tbq.yuanzhike.top

[D16] 求和与平均值
来源：http://mdf.chenjidiqi.icu

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jdx.chenjidiqi.icu

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dso.shuidangran.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ezj.pengpengdd.cyou

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zrl.hcnkem.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ogj.zycfv.cn

Go:   // 手写循环累加
来源：http://wsp.zhixingplan.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lfy.epnwcf.com

C#:   list.Sum();  list.Average()
来源：http://gnw.zhoulong.xyz

[D17] 最大值与最小值
来源：http://cqb.xziqi.cn

Py:   max(arr);  min(arr)
来源：http://fju.ctjpmb.com

PHP:  max($arr);  min($arr);
来源：http://sqf.jinqigufen.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zmu.tian-w.cn

TS:   Math.max(...arr);
来源：http://mqr.uphjek.com

Java: Collections.max(list);  Collections.min(list);
来源：http://rtt.jinyuanbaomall.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wao.yuxming.cn

Ruby: arr.max;  arr.min
来源：http://gvj.yangfankeji.com

C#:   list.Max();  list.Min()
来源：http://yqm.svipenyu.cn

[D18] 扁平化嵌套数组
来源：http://wlw.hammf.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dbr.ybcxt.top

PHP:  array_merge(...$nested);
来源：http://ier.tian-w.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://oqc.uphjek.com

TS:   nested.flat();
来源：http://fdv.fengsongda.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://eew.jinyuanbaomall.cn

Go:   // 手写双层循环
来源：http://gdg.gzhubu.top

Ruby: nested.flatten
来源：http://vzh.gotoacloud.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://eoi.ydzc1.top

[D19] 按字段分组
来源：http://hlj.zhijiandao.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tej.kuanghao11.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://smr.pycfn.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yxo.birdmap.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://gwe.vqdsnc.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vfw.hnqzz.top

Go:   // 手写 map[string][]T
来源：http://ofo.cdnleiting.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://htw.tianlin.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://eeo.jinyuanbaomall.cn

[D20] 统计每个元素出现次数
来源：http://itz.jinghuilouyu.cn

Py:   Counter(arr)
来源：http://iir.hfpthk.cn

PHP:  array_count_values($arr);
来源：http://vuw.pengpengdd.cyou

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cfi.ivvv.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vxl.yangfankeji.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jea.zhijiandao.cn

Go:   // 手写 map[T]int
来源：http://dqy.tarul.cn

Ruby: arr.tally
来源：http://kxg.xylfe.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ucr.birdmap.top

[D21] 判断是否包含某元素
来源：http://nbg.hammf.cn

Py:   x in arr
来源：http://lro.zhijiandao.cn

PHP:  in_array($x, $arr, true);
来源：http://kxc.ydjk.org.cn

JS:   arr.includes(x)
来源：http://uez.havefunace.top

TS:   arr.includes(x)
来源：http://nhr.vehdjk.com

Java: list.contains(x)
来源：http://lnk.bjfxy.top

Go:   slices.Contains(arr, x)
来源：http://jqj.chenjidiqi.icu

Ruby: arr.include?(x)
来源：http://kvb.yj20258.top

C#:   list.Contains(x)
来源：http://zap.jyoumei.cn

[D22] 复制数组（避免共享引用）
来源：http://mcp.hcnkem.com


<!-- 参考信息 -->