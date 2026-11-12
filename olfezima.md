代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://lxc.haohaochexian.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yfx.pengpengdd.cyou

[C04] 命名参数 / 关键字参数
来源：http://des.zycfv.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lpm.iojbl.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pmb.redwolf501.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ssl.cdnleiting.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sxb.yj20258.top

Java: // 无：用 Builder 模式或 record
来源：http://ixy.sjlbkw.cn

Go:   // 无：用配置结构体参数
来源：http://dip.bjfxy.top

Ruby: f(a: 1, b: 2)
来源：http://bop.yueranfly.top

C#:   f(a: 1, b: 2)
来源：http://hkd.zhixingplan.top

[C05] 返回多个值
来源：http://avb.meibo888.top

Py:   return a, b
来源：http://ops.havefunace.top

PHP:  return [$a, $b];
来源：http://tmc.yfazqb.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://lfv.vqdsnc.cn

TS:   return { a, b };
来源：http://wkt.aibaodan.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qmd.sweek.top

Go:   return a, b
来源：http://ekr.jianghu66.top

Ruby: return a, b
来源：http://gqu.xinyue.icu

C#:   return (a, b);              // ValueTuple
来源：http://dwq.fengsongda.top

[C06] 匿名函数 / lambda
来源：http://pkz.nanxuanxn.top

Py:   square = lambda x: x * x
来源：http://yrb.feifeiyinyue.top

PHP:  $square = fn($x) => $x * $x;
来源：http://dwz.sxryk.cn

JS:   const square = x => x * x;
来源：http://zba.jqgfzy.top

TS:   const square = (x: number): number => x * x;
来源：http://uym.hywenlv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tkf.hesvh.cn

Go:   sq := func(x int) int { return x * x }
来源：http://uvn.zhengqikj.top

Ruby: square = ->(x) { x * x }
来源：http://kyx.jinqigufen.top

C#:   Func<int, int> square = x => x * x;
来源：http://akp.fehbvm.com

[C07] 把函数作为参数传入
来源：http://lyc.yj20258.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mda.fehbvm.com

PHP:  array_map("strtoupper", $arr);
来源：http://axp.zycfv.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sxk.zycfv.cn

TS:   arr.map(String)
来源：http://ldr.tarul.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vdj.ehwqpu.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vqe.hfpthk.cn

Ruby: arr.map(&:upcase)
来源：http://efp.shzxlz.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lbu.9152youxi.cn

[C08] 闭包
来源：http://qcb.yj20258.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mgx.ydzc1.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bcl.hammf.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wgn.vqdsnc.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gcb.shanyushiyangtech.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://khi.fktsv.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pja.yonumen.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vxi.zhijiandao.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pdr.sxryk.cn

[C09] 递归
来源：http://msx.yanxiufei.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vvl.shanyushiyangkeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zug.havefunace.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xlu.zhaomingkeji.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lfv.c1oappe.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://noq.zhengqikj.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://maq.zhixingplan.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dzz.nanxuanxn.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://itu.yonumen.top

[C10] 变量作用域
来源：http://nea.hnxiangtu.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lal.redwolf501.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pmp.daxiang520.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dlk.bbcook.cn

TS:   同 JS
来源：http://fcu.epnwcf.com

Java: 方法内为块级作用域
来源：http://xrs.zhengqikj.top

Go:   花括号块级作用域
来源：http://ier.yongpay.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xyn.fanxiaobao.xyz

C#:   块级作用域
来源：http://vwu.zhaomingkeji.xyz

[C11] 模块导入与导出
来源：http://xfe.hysaishi.cn

Py:   from module import func
来源：http://gib.shuidangran.top

PHP:  require "file.php";  或 use App\Service;
来源：http://unl.jqgufenzy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://iuw.cheryme.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://eir.ybcxt.top

Java: import java.util.List;
来源：http://msh.zhijiandao.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ssl.ywan-chungtsiang.top

Ruby: require "json"; require_relative "./util"
来源：http://hhj.jqgufenzy.top

C#:   using System.Text;
来源：http://dkm.wangdashe.top

[C12] 立即执行函数 IIFE
来源：http://llm.yj20258888.top

Py:   (lambda: print("run"))()
来源：http://fnq.daria6918.cn

PHP:  (function () { echo "run"; })();
来源：http://kqs.gogol.net.cn

JS:   (() => { console.log("run"); })();
来源：http://bdg.yj20258888.top

TS:   (() => { console.log("run"); })();
来源：http://mri.gogol.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://znt.ywan-chungtsiang.top

Go:   func() { fmt.Println("run") }()
来源：http://zdf.zdqjudy.top

Ruby: -> { puts "run" }.call
来源：http://cqo.nanxuanxn.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ncc.xuanzx.com

[C13] 类型声明 / 类型注解
来源：http://jpv.0kj1m.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zdl.hnqzz.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pdc.ehwqpu.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://edg.zdqjudy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vld.hammf.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wiy.sjlbkw.cn

Go:   func add(a, b int) int
来源：http://ykt.tanke756.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wtd.jinqigfzy.top

C#:   int Add(int a, int b) => a + b;
来源：http://yhp.jiagoushi.top

[C14] 泛型函数
来源：http://xva.gaohongyu789.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zia.zhiwuduotai.top

PHP:  // 无泛型
来源：http://dca.mhx1999.top

JS:   // 无泛型
来源：http://mez.shzxlz.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xdn.shanyushiyangkeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://eid.hnqzz.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zhj.daxiang520.top

Ruby: # 无泛型
来源：http://hkm.havefunace.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wgm.bjfxy.top

[C15] 解构 / 展开参数
来源：http://rhc.cashguo.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hnw.xziqi.cn

PHP:  [$a, $b] = $pair;
来源：http://azs.aibaodan.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://egg.jinqigfzy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kdd.yvedp.cn

Java: // 无解构
来源：http://oqk.9152youxi.cn

Go:   // 无解构
来源：http://jyl.pengpengdd.cyou

Ruby: a, b = pair
来源：http://fqe.wangdashe.top

C#:   var (a, b) = pair;
来源：http://jsi.bbcook.cn

[C16] 函数 / 方法重载
来源：http://uey.jinghuilouyu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://izb.zycfv.cn

PHP:  // 无重载
来源：http://mka.yueranfly.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://iti.kuanghao11.cn

TS:   // 用联合类型或重载签名声明
来源：http://tgp.xingfuxueyuan.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://apn.daria6918.cn

Go:   // 无重载：用不同函数名
来源：http://msn.hongshengwenyu.top

Ruby: # 无重载：靠动态参数
来源：http://jzc.cucudq.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mcp.xinyue.icu

================================================================================
来源：http://crk.kuanghao11.cn

D. 数组 / 列表 / 集合
来源：http://vef.cheryme.top

================================================================================
来源：http://ogu.jqgfzy.top

[D01] 创建数组 / 列表
来源：http://mvn.sysykeji.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://fgd.shanyushiyangkeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://duy.quarkkingdee.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qkk.jianghu66.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://vba.nanxinkj.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sag.wangshuangyany.cn

Go:   arr := []int{1, 2, 3}
来源：http://lbi.zhijiandao.cn

Ruby: arr = [1, 2, 3]
来源：http://ygg.jyoumei.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://egp.jinghuilouyu.cn

[D02] 追加元素到末尾
来源：http://xwh.ydzc1.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gxw.uphjek.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mzv.tianlin.xyz

JS:   arr.push(4);
来源：http://ozu.ctjpmb.com

TS:   arr.push(4);
来源：http://mvi.andypj.xyz

Java: list.add(4);
来源：http://wco.0kj1m.cn

Go:   arr = append(arr, 4)
来源：http://hmd.hywenlv.cn

Ruby: arr << 4; arr.push(5)
来源：http://nfy.cdnleiting.top

C#:   list.Add(4);
来源：http://wnr.dianchejie.cn

[D03] 在指定位置插入元素
来源：http://mts.havefunace.top

Py:   arr.insert(0, 0)
来源：http://oko.havefunace.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lqm.ywan-chungtsiang.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ojq.cashguo.top

TS:   arr.splice(0, 0, 0);
来源：http://uwl.zhongyouzk.top

Java: list.add(0, 0);
来源：http://dff.zhixingplan.top

Go:   arr = append([]int{0}, arr...)
来源：http://hyt.cdnleiting.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tsb.jianghu66.top

C#:   list.Insert(0, 0);
来源：http://ava.sufxvd.cn

[D04] 删除元素
来源：http://btk.fengsongda.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://owe.tanke756.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lwk.ivvv.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://oep.uphjek.com

TS:   arr.splice(0, 1);
来源：http://nkd.jqgufenzy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gbf.yfazqb.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qlf.shuidangran.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ktl.xingfuxueyuan.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://iif.ydzc1.top

[D05] 访问与修改元素
来源：http://lpx.tian-w.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qdv.ppjwa.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://aex.yongpay.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xqc.hfpthk.cn

TS:   arr[0]; arr.at(-1);
来源：http://gxl.xinyue.icu

Java: list.get(0); list.set(0, 9);
来源：http://qqf.vehdjk.com

Go:   arr[0]; arr[0] = 9
来源：http://avs.zhongyouzk.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bnh.zhoulong.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://day.sufxvd.cn

[D06] 数组长度
来源：http://npq.ybcxt.top

Py:   len(arr)
来源：http://rle.zdqjudy.top

PHP:  count($arr);
来源：http://ifq.vehdjk.com

JS:   arr.length
来源：http://ump.ydjk.org.cn

TS:   arr.length
来源：http://enz.uphjek.com

Java: list.size();
来源：http://ynt.zhaomingkeji.xyz

Go:   len(arr)
来源：http://wbx.pengpengdd.cyou

Ruby: arr.length; arr.size
来源：http://yxi.ybcxt.top

C#:   list.Count;
来源：http://apv.hnqzz.top

[D07] 切片 / 取子数组
来源：http://eut.redwolf501.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nsj.yj20258.top

PHP:  array_slice($arr, 1, 3);
来源：http://udb.cdnleiting.top

JS:   arr.slice(1, 4);
来源：http://mzv.sxryk.cn

TS:   arr.slice(1, 4);
来源：http://zxr.vqdsnc.cn

Java: list.subList(1, 4);
来源：http://yme.fktsv.cn

Go:   arr[1:4]
来源：http://byg.jianghu66.top

Ruby: arr[1, 3]
来源：http://kho.cqqwz.cn

C#:   list.GetRange(1, 3);
来源：http://pac.hywenlv.cn

[D08] 合并两个数组
来源：http://twn.sjlbkw.cn

Py:   a + b;  a.extend(b)
来源：http://oft.hnqzz.top

PHP:  array_merge($a, $b);
来源：http://kdt.ehwqpu.com

JS:   [...a, ...b];  a.concat(b);
来源：http://vzb.yuxming.cn

TS:   [...a, ...b];
来源：http://lan.cucudq.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bzr.zhongyouzk.top

Go:   append(a, b...)
来源：http://fjz.sxryk.cn

Ruby: a + b;  a.concat(b)
来源：http://euj.hfpthk.cn

C#:   a.Concat(b).ToList()
来源：http://zqd.guowangkeji.top

[D09] 排序（升序）
来源：http://ftw.zhoulong.xyz

Py:   sorted(arr);  arr.sort()
来源：http://xeo.zhixingplan.top

PHP:  sort($arr);
来源：http://sgu.zhoulong.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uyq.jinyuanbaomall.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://rwe.vqdsnc.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zgm.shanyushiyangtech.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xhd.daria6918.cn

Ruby: arr.sort
来源：http://wph.52xcode.cn

C#:   list.Sort();
来源：http://xgp.daxiang520.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://njt.aibaodan.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rdn.shanyushiyangtech.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://isu.wangdashe.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kgv.9152youxi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jxs.hnxiangtu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ank.nanxuanxn.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wju.jiagoushi.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kyl.zhiwuduotai.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qet.cqqwz.cn

[D11] 反转数组
来源：http://hvf.snrcjt.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hfv.shanyushiyangkeji.top

PHP:  array_reverse($arr);
来源：http://rts.ctjpmb.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://oru.52xcode.cn

TS:   [...arr].reverse();
来源：http://txi.tanke756.top

Java: Collections.reverse(list);
来源：http://bzm.jinyuanbaomall.cn

Go:   slices.Reverse(arr)
来源：http://tso.yueranfly.top

Ruby: arr.reverse
来源：http://olo.guannengcc.top

C#:   list.Reverse();
来源：http://hxa.guowangkeji.top

[D12] 查找元素下标
来源：http://ugq.fzhhl.top

Py:   arr.index(x);  x in arr
来源：http://mqa.dianchejie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mhl.meibo888.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xlg.xylfe.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://osv.zhongyouzk.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ujv.dashuyun.cn

Go:   slices.Index(arr, x)
来源：http://rro.sjlbkw.cn

Ruby: arr.index(x)
来源：http://wed.bjfxy.top

C#:   list.IndexOf(x);
来源：http://mzq.chenjidiqi.icu

[D13] 过滤（保留满足条件的）
来源：http://tzx.shanyushiyangtech.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xlf.0kj1m.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dji.hammf.cn

JS:   arr.filter(x => x > 3)
来源：http://aqp.fengsongda.top

TS:   arr.filter(x => x > 3)
来源：http://zep.yongpay.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mui.jqgufenzy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bcd.zhiwuduotai.top

Ruby: arr.select { |x| x > 3 }
来源：http://jqb.uphjek.com

C#:   list.Where(x => x > 3).ToList()
来源：http://rii.fzhhl.top

[D14] 映射转换（每个元素变形）
来源：http://cmp.tian-w.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gzx.ctjpmb.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jpj.yj20258.top

JS:   arr.map(x => x * 2)
来源：http://mhh.gotoacloud.top

TS:   arr.map(x => x * 2)
来源：http://kwv.zhijiandao.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://mzu.hongshengwenyu.top

Go:   // 手写循环
来源：http://ecp.c1oappe.top

Ruby: arr.map { |x| x * 2 }
来源：http://mdl.aizwys.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pho.tianlin.xyz

[D15] 去重
来源：http://fvp.redwolf501.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xfn.jiagoushi.top

PHP:  array_unique($arr);
来源：http://rds.redwolf501.top

JS:   [...new Set(arr)]
来源：http://iep.pycfn.com

TS:   [...new Set(arr)]
来源：http://hhp.hammf.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ffu.daria6918.cn

Go:   // 用 map[T]struct{} 手写
来源：http://keq.nanxinkj.top

Ruby: arr.uniq
来源：http://jos.0kj1m.cn

C#:   list.Distinct().ToList()
来源：http://ctn.ehwqpu.com

[D16] 求和与平均值
来源：http://nhr.jyoumei.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lxe.sjlbkw.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vzv.yj202588.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://suy.52xcode.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://uyt.hnxiangtu.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pvw.gaohongyu789.top

Go:   // 手写循环累加
来源：http://ydn.nwbrower.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fzy.ppjwa.cn

C#:   list.Sum();  list.Average()
来源：http://xfu.gotoacloud.top

[D17] 最大值与最小值
来源：http://pgn.chenlongwang.top

Py:   max(arr);  min(arr)
来源：http://mkc.zhoulong.xyz

PHP:  max($arr);  min($arr);
来源：http://vzh.havefunace.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lfc.hcnkem.com

TS:   Math.max(...arr);
来源：http://srg.hfpthk.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://cyu.cqqwz.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jyv.zhaomingkeji.xyz

Ruby: arr.max;  arr.min
来源：http://akl.zhaomingkeji.xyz

C#:   list.Max();  list.Min()
来源：http://cor.ywan-chungtsiang.top

[D18] 扁平化嵌套数组
来源：http://lsi.guannengcc.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hmg.c1oappe.top

PHP:  array_merge(...$nested);
来源：http://zmy.birdmap.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zyn.pengpengdd.cyou

TS:   nested.flat();
来源：http://nwh.zhijiandao.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tdb.shanyushiyangtech.top

Go:   // 手写双层循环
来源：http://lhu.chenzaomai.com

Ruby: nested.flatten
来源：http://vwa.cucudq.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wgr.cashguo.top

[D19] 按字段分组
来源：http://ekp.zhongyouzk.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qet.sweek.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fco.shanyushiyangtech.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qww.xuetiantiany.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ykr.gogol.net.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yxx.mhx1999.top

Go:   // 手写 map[string][]T
来源：http://zxi.xziqi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://mki.ydzc1.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://eaa.quarkkingdee.top

[D20] 统计每个元素出现次数
来源：http://osi.gzhubu.top

Py:   Counter(arr)
来源：http://gdj.hnxiangtu.top

PHP:  array_count_values($arr);
来源：http://ykb.hesvh.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qhe.yongpay.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fio.dianchejie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bjx.cheryme.top

Go:   // 手写 map[T]int
来源：http://qor.gaohongyu789.top


<!-- 参考信息 -->