代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://kbm.c1oappe.top

Ruby: f(a: 1, b: 2)
来源：http://hhw.wangdashe.top

C#:   f(a: 1, b: 2)
来源：http://osv.jinqigfzy.top

[C05] 返回多个值
来源：http://cmn.hcnkem.com

Py:   return a, b
来源：http://hur.fktsv.cn

PHP:  return [$a, $b];
来源：http://wqt.dashuyun.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://upq.dashuyun.cn

TS:   return { a, b };
来源：http://gvp.sjlbkw.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zsz.chenjidiqi.icu

Go:   return a, b
来源：http://hhv.yfazqb.com

Ruby: return a, b
来源：http://hyg.ivvv.top

C#:   return (a, b);              // ValueTuple
来源：http://kyl.hysaishi.cn

[C06] 匿名函数 / lambda
来源：http://vwf.yonumen.top

Py:   square = lambda x: x * x
来源：http://sre.aizwys.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ysv.yuanzhike.top

JS:   const square = x => x * x;
来源：http://snk.xingfuxueyuan.xyz

TS:   const square = (x: number): number => x * x;
来源：http://qyu.yonumen.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wdw.zhiwuduotai.top

Go:   sq := func(x int) int { return x * x }
来源：http://ovq.guowangkeji.top

Ruby: square = ->(x) { x * x }
来源：http://ccz.redwolf501.top

C#:   Func<int, int> square = x => x * x;
来源：http://xso.yueranfly.top

[C07] 把函数作为参数传入
来源：http://akh.zhiwuduotai.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://swo.havefunace.top

PHP:  array_map("strtoupper", $arr);
来源：http://bcv.redwolf501.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hwc.sjlbkw.cn

TS:   arr.map(String)
来源：http://xbr.dashuyun.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ifp.yfazqb.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vsn.bbcook.cn

Ruby: arr.map(&:upcase)
来源：http://frx.epnwcf.com

C#:   arr.Select(s => s.ToUpper())
来源：http://rlt.chenlongwang.top

[C08] 闭包
来源：http://pjc.yj202588.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rto.sxryk.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nwr.fanxiaobao.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://oop.yvedp.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qmf.guannengcc.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tnl.andypj.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tam.wangshuangyany.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tus.9152youxi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vxw.shuidangran.top

[C09] 递归
来源：http://oen.smart0.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zmn.jinqigufen.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bdg.shuidangran.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yux.hesvh.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qmy.zhixingplan.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://amv.fengsongda.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://awj.yvedp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://igk.zhoulong.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://amn.c1oappe.top

[C10] 变量作用域
来源：http://xzo.tianlin.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xrp.zhiwuduotai.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mpr.sjlbkw.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mwx.zycfv.cn

TS:   同 JS
来源：http://cxq.pengpengdd.cyou

Java: 方法内为块级作用域
来源：http://idf.hysaishi.cn

Go:   花括号块级作用域
来源：http://qco.yangfankeji.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ydr.ydjk.org.cn

C#:   块级作用域
来源：http://luh.zhixingplan.top

[C11] 模块导入与导出
来源：http://qnh.ydjk.org.cn

Py:   from module import func
来源：http://git.shzxlz.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://jlr.52xcode.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://yil.chenlongwang.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bmc.sjlbkw.cn

Java: import java.util.List;
来源：http://zcf.sjlbkw.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xwh.sufxvd.cn

Ruby: require "json"; require_relative "./util"
来源：http://pdj.fktsv.cn

C#:   using System.Text;
来源：http://jpr.andypj.xyz

[C12] 立即执行函数 IIFE
来源：http://myo.pycfn.com

Py:   (lambda: print("run"))()
来源：http://bqm.yj20258.top

PHP:  (function () { echo "run"; })();
来源：http://mya.zhiwuduotai.top

JS:   (() => { console.log("run"); })();
来源：http://wgj.zdbjq.cn

TS:   (() => { console.log("run"); })();
来源：http://rch.jlsjyb.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ert.gogol.net.cn

Go:   func() { fmt.Println("run") }()
来源：http://hjx.jianghu66.top

Ruby: -> { puts "run" }.call
来源：http://ltl.shanyushiyangtech.top

C#:   // 无 IIFE：用静态构造函数
来源：http://nhe.hfpthk.cn

[C13] 类型声明 / 类型注解
来源：http://gbf.zdqjudy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ooy.fengsongda.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kah.zycfv.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zro.jqgfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gvl.bjfxy.top

Java: int add(int a, int b) { return a + b; }
来源：http://ajm.mhx1999.top

Go:   func add(a, b int) int
来源：http://npe.dashuyun.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://iam.yfazqb.com

C#:   int Add(int a, int b) => a + b;
来源：http://mio.xinyue.icu

[C14] 泛型函数
来源：http://nff.chenjidiqi.icu

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dor.yangfankeji.com

PHP:  // 无泛型
来源：http://wpg.zhengqikj.top

JS:   // 无泛型
来源：http://ddh.sweek.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ucg.yj202588.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mgd.shuidangran.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pjd.c1oappe.top

Ruby: # 无泛型
来源：http://iwt.yj20258888.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bts.shangyingyoupin.top

[C15] 解构 / 展开参数
来源：http://rcv.dianchejie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ule.shzxlz.cn

PHP:  [$a, $b] = $pair;
来源：http://mku.epnwcf.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uee.jyoumei.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://axj.shanyushiyangtech.top

Java: // 无解构
来源：http://qtp.yj202588.top

Go:   // 无解构
来源：http://pqv.bjfxy.top

Ruby: a, b = pair
来源：http://ycg.316326.xyz

C#:   var (a, b) = pair;
来源：http://zvr.wangshuangyany.cn

[C16] 函数 / 方法重载
来源：http://ynd.zhengqikj.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ksp.iojbl.cn

PHP:  // 无重载
来源：http://iun.yj20258.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://lzy.yanxiufei.cn

TS:   // 用联合类型或重载签名声明
来源：http://tbr.zdbjq.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qgl.chenlongwang.top

Go:   // 无重载：用不同函数名
来源：http://kcq.cdnleiting.top

Ruby: # 无重载：靠动态参数
来源：http://ejr.hammf.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://bhj.vehdjk.com

================================================================================
来源：http://zyt.sysykeji.top

D. 数组 / 列表 / 集合
来源：http://mbh.chenjidiqi.icu

================================================================================
来源：http://psd.bbcook.cn

[D01] 创建数组 / 列表
来源：http://gmd.nanxuanxn.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ros.yonumen.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fyx.chenzaomai.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uam.jlsjyb.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://pcc.yonumen.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zyr.haohaochexian.top

Go:   arr := []int{1, 2, 3}
来源：http://nnk.ywan-chungtsiang.top

Ruby: arr = [1, 2, 3]
来源：http://axl.yueranfly.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yni.nwbrower.top

[D02] 追加元素到末尾
来源：http://lst.shanyushiyangtech.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tkj.yangfankeji.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oot.bjfxy.top

JS:   arr.push(4);
来源：http://krz.sxryk.cn

TS:   arr.push(4);
来源：http://ift.yueranfly.top

Java: list.add(4);
来源：http://wbe.ybcxt.top

Go:   arr = append(arr, 4)
来源：http://nkg.jianghu66.top

Ruby: arr << 4; arr.push(5)
来源：http://vvb.birdmap.top

C#:   list.Add(4);
来源：http://hlm.sysykeji.top

[D03] 在指定位置插入元素
来源：http://hay.hesvh.cn

Py:   arr.insert(0, 0)
来源：http://dyw.jinqigfzy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cih.shanyushiyangkeji.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ahg.bbcook.cn

TS:   arr.splice(0, 0, 0);
来源：http://qan.gaohongyu789.top

Java: list.add(0, 0);
来源：http://ybi.tarul.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zmk.jqgufenzy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sdj.sxryk.cn

C#:   list.Insert(0, 0);
来源：http://veu.316326.xyz

[D04] 删除元素
来源：http://jpd.0kj1m.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hod.hfpthk.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ymn.xuanzx.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yby.ybcxt.top

TS:   arr.splice(0, 1);
来源：http://ywr.zhongyouzk.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://njv.hammf.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tqp.sufxvd.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yen.chenjidiqi.icu

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xqv.chenzaomai.com

[D05] 访问与修改元素
来源：http://crw.xingfuxueyuan.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qty.zhijiandao.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xtm.daria6918.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blr.tanke756.top

TS:   arr[0]; arr.at(-1);
来源：http://kbe.chenzaomai.com

Java: list.get(0); list.set(0, 9);
来源：http://enz.smart0.xyz

Go:   arr[0]; arr[0] = 9
来源：http://scg.jianghu66.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://afr.jinghuilouyu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://enn.ydzc1.top

[D06] 数组长度
来源：http://tgl.tarul.cn

Py:   len(arr)
来源：http://guu.pycfn.com

PHP:  count($arr);
来源：http://mpr.andypj.xyz

JS:   arr.length
来源：http://xkl.yfazqb.com

TS:   arr.length
来源：http://fof.jiagoushi.top

Java: list.size();
来源：http://uzf.uphjek.com

Go:   len(arr)
来源：http://uks.sufxvd.cn

Ruby: arr.length; arr.size
来源：http://pvm.shanyushiyangkeji.top

C#:   list.Count;
来源：http://mnu.hcnkem.com

[D07] 切片 / 取子数组
来源：http://xbb.iojbl.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jkg.jqgfzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://xne.cucudq.cn

JS:   arr.slice(1, 4);
来源：http://joh.zhengqikj.top

TS:   arr.slice(1, 4);
来源：http://oht.ctjpmb.com

Java: list.subList(1, 4);
来源：http://yxb.dianchejie.cn

Go:   arr[1:4]
来源：http://vbz.guannengcc.top

Ruby: arr[1, 3]
来源：http://lnl.9152youxi.cn

C#:   list.GetRange(1, 3);
来源：http://mdi.c1oappe.top

[D08] 合并两个数组
来源：http://qud.tanke756.top

Py:   a + b;  a.extend(b)
来源：http://vyh.jqgufenzy.top

PHP:  array_merge($a, $b);
来源：http://hwi.c1oappe.top

JS:   [...a, ...b];  a.concat(b);
来源：http://off.hnqzz.top

TS:   [...a, ...b];
来源：http://lwo.hywenlv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cmj.hywenlv.cn

Go:   append(a, b...)
来源：http://bqt.bjfxy.top

Ruby: a + b;  a.concat(b)
来源：http://dwz.hywenlv.cn

C#:   a.Concat(b).ToList()
来源：http://btc.yonumen.top

[D09] 排序（升序）
来源：http://tdn.xuetiantiany.cn

Py:   sorted(arr);  arr.sort()
来源：http://gia.zhiwuduotai.top

PHP:  sort($arr);
来源：http://dda.ywan-chungtsiang.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bbs.hfpthk.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wco.hammf.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://lrr.pycfn.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cmu.jlsjyb.cn

Ruby: arr.sort
来源：http://bhc.smart0.xyz

C#:   list.Sort();
来源：http://nyr.daria6918.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://wrf.ppjwa.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cjp.svipenyu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dch.hfpthk.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gbt.svipenyu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://uhn.shuidangran.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sog.jlsjyb.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ccs.yj202588.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ugx.shangyingyoupin.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://udr.ehwqpu.com

[D11] 反转数组
来源：http://ysk.sjlbkw.cn

Py:   arr[::-1];  arr.reverse()
来源：http://clt.birdmap.top

PHP:  array_reverse($arr);
来源：http://mcu.yuanzhike.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tdr.bbcook.cn

TS:   [...arr].reverse();
来源：http://ovw.aibaodan.cn

Java: Collections.reverse(list);
来源：http://xls.chenzaomai.com

Go:   slices.Reverse(arr)
来源：http://vwa.xingfuxueyuan.xyz

Ruby: arr.reverse
来源：http://buh.yfazqb.com

C#:   list.Reverse();
来源：http://bpc.cashguo.top

[D12] 查找元素下标
来源：http://uvu.yangfankeji.com

Py:   arr.index(x);  x in arr
来源：http://evd.sufxvd.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qlm.hywenlv.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lcy.wangshuangyany.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uwc.jqgfzy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nbe.gaohongyu789.top

Go:   slices.Index(arr, x)
来源：http://mcn.hfpthk.cn

Ruby: arr.index(x)
来源：http://yfk.cashguo.top

C#:   list.IndexOf(x);
来源：http://hly.cashguo.top

[D13] 过滤（保留满足条件的）
来源：http://wwo.havefunace.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://iir.yj202588.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wtb.jlsjyb.cn

JS:   arr.filter(x => x > 3)
来源：http://wbg.pengpengdd.cyou

TS:   arr.filter(x => x > 3)
来源：http://tsn.xuanzx.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://iee.birdmap.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://irl.feifeiyinyue.top

Ruby: arr.select { |x| x > 3 }
来源：http://wsj.chenlongwang.top

C#:   list.Where(x => x > 3).ToList()
来源：http://fkh.zhengqikj.top

[D14] 映射转换（每个元素变形）
来源：http://yqr.shanyushiyangkeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wgx.yanxiufei.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tgb.jyoumei.cn

JS:   arr.map(x => x * 2)
来源：http://coo.xuanzx.com

TS:   arr.map(x => x * 2)
来源：http://uzo.quarkkingdee.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ori.sysykeji.top

Go:   // 手写循环
来源：http://dng.0kj1m.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yby.fzhhl.top

C#:   list.Select(x => x * 2).ToList()
来源：http://nrd.cashguo.top

[D15] 去重
来源：http://yog.jyoumei.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dwl.bbcook.cn

PHP:  array_unique($arr);
来源：http://xwp.sufxvd.cn

JS:   [...new Set(arr)]
来源：http://fny.jiagoushi.top

TS:   [...new Set(arr)]
来源：http://gmx.kuanghao11.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://udo.jiagoushi.top

Go:   // 用 map[T]struct{} 手写
来源：http://jti.zhijiandao.cn

Ruby: arr.uniq
来源：http://yuo.guowangkeji.top

C#:   list.Distinct().ToList()
来源：http://iha.jqgufenzy.top

[D16] 求和与平均值
来源：http://vxj.jinqigufen.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tmi.havefunace.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dha.0kj1m.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ogj.bjfxy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ihl.0kj1m.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xoi.yonumen.top

Go:   // 手写循环累加
来源：http://kkv.xuanzx.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rwr.zhongyouzk.top

C#:   list.Sum();  list.Average()
来源：http://ixt.bbcook.cn

[D17] 最大值与最小值
来源：http://rzu.jinqigufen.top

Py:   max(arr);  min(arr)
来源：http://ogc.yuanzhike.top

PHP:  max($arr);  min($arr);
来源：http://yfe.fktsv.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wsd.ehwqpu.com

TS:   Math.max(...arr);
来源：http://aqo.shangyingyoupin.top

Java: Collections.max(list);  Collections.min(list);
来源：http://eye.hywenlv.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mng.tanke756.top

Ruby: arr.max;  arr.min
来源：http://akc.yj20258888.top

C#:   list.Max();  list.Min()
来源：http://tju.ywan-chungtsiang.top

[D18] 扁平化嵌套数组
来源：http://gyx.shanyushiyangtech.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://van.zhoulong.xyz

PHP:  array_merge(...$nested);
来源：http://kui.mhx1999.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ine.0kj1m.cn

TS:   nested.flat();
来源：http://qnb.fengsongda.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://krs.dashuyun.cn

Go:   // 手写双层循环
来源：http://oep.daria6918.cn

Ruby: nested.flatten
来源：http://hqs.sysykeji.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://fse.birdmap.top

[D19] 按字段分组
来源：http://nbl.feifeiyinyue.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qcs.cqqwz.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tgb.fktsv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ejh.zhongyouzk.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://cuo.svipenyu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://alc.yangfankeji.com

Go:   // 手写 map[string][]T
来源：http://rso.zycfv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zcu.zhongyouzk.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://crd.aizwys.cn

[D20] 统计每个元素出现次数
来源：http://wdm.chenlongwang.top

Py:   Counter(arr)
来源：http://jte.fktsv.cn

PHP:  array_count_values($arr);
来源：http://nxa.yongpay.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gpq.nwbrower.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://unm.zhoulong.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uii.uphjek.com

Go:   // 手写 map[T]int
来源：http://qqu.shanyushiyangtech.top

Ruby: arr.tally
来源：http://uyw.shangyingyoupin.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tlj.hfpthk.cn

[D21] 判断是否包含某元素
来源：http://juf.jqgfzy.top

Py:   x in arr
来源：http://ggr.nanxinkj.top

PHP:  in_array($x, $arr, true);
来源：http://aaa.wangdashe.top

JS:   arr.includes(x)
来源：http://hnx.birdmap.top

TS:   arr.includes(x)
来源：http://xpl.hcnkem.com

Java: list.contains(x)
来源：http://vrv.svipenyu.cn


<!-- 参考信息 -->