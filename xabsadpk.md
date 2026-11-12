代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lkp.haohaochexian.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hhb.yj20258888.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rxz.sysykeji.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bky.hysaishi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yem.zhiwuduotai.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ujl.zdbjq.cn

[C04] 命名参数 / 关键字参数
来源：http://ucw.shanyushiyangtech.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://brw.jianghu66.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qyy.sjlbkw.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hgs.havefunace.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wgn.chenzaomai.com

Java: // 无：用 Builder 模式或 record
来源：http://jge.zhaomingkeji.xyz

Go:   // 无：用配置结构体参数
来源：http://sdd.nanxinkj.top

Ruby: f(a: 1, b: 2)
来源：http://eht.dianchejie.cn

C#:   f(a: 1, b: 2)
来源：http://gyv.ivvv.top

[C05] 返回多个值
来源：http://sop.jianghu66.top

Py:   return a, b
来源：http://ruh.wangdashe.top

PHP:  return [$a, $b];
来源：http://axk.chenlongwang.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://wjx.tanke756.top

TS:   return { a, b };
来源：http://ipf.smart0.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ovz.pycfn.com

Go:   return a, b
来源：http://jxi.nanxuanxn.top

Ruby: return a, b
来源：http://ced.zhiwuduotai.top

C#:   return (a, b);              // ValueTuple
来源：http://lrg.iojbl.cn

[C06] 匿名函数 / lambda
来源：http://irq.hammf.cn

Py:   square = lambda x: x * x
来源：http://zis.vqdsnc.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://uyn.kuanghao11.cn

JS:   const square = x => x * x;
来源：http://gbv.hysaishi.cn

TS:   const square = (x: number): number => x * x;
来源：http://whe.316326.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kjo.andypj.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://mxx.jqgufenzy.top

Ruby: square = ->(x) { x * x }
来源：http://jsm.fengsongda.top

C#:   Func<int, int> square = x => x * x;
来源：http://rzc.snrcjt.cn

[C07] 把函数作为参数传入
来源：http://wip.havefunace.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://raj.hysaishi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ovx.vehdjk.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ndn.cqqwz.cn

TS:   arr.map(String)
来源：http://dvl.haohaochexian.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zce.shanyushiyangtech.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://okv.tarul.cn

Ruby: arr.map(&:upcase)
来源：http://qcm.yonumen.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ssz.zhengqikj.top

[C08] 闭包
来源：http://pum.zhixingplan.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://esj.feifeiyinyue.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dcy.smart0.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yxl.sjlbkw.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xks.epnwcf.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pft.nanxuanxn.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xyb.cashguo.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yrl.hongshengwenyu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kwm.yonumen.top

[C09] 递归
来源：http://dnz.sweek.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xmm.zdbjq.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zfw.fehbvm.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cru.mhx1999.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gnf.c1oappe.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://udn.zhiwuduotai.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nfh.mhx1999.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fja.zhiwuduotai.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sqf.sxryk.cn

[C10] 变量作用域
来源：http://ejr.xuetiantiany.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lgm.yj202588.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fgq.sysykeji.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nlm.nanxuanxn.top

TS:   同 JS
来源：http://bcp.cucudq.cn

Java: 方法内为块级作用域
来源：http://bvp.jqgfzy.top

Go:   花括号块级作用域
来源：http://qfo.zhongyouzk.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bii.yj20258888.top

C#:   块级作用域
来源：http://xdu.jiagoushi.top

[C11] 模块导入与导出
来源：http://bas.vqdsnc.cn

Py:   from module import func
来源：http://lbu.chenjidiqi.icu

PHP:  require "file.php";  或 use App\Service;
来源：http://cyq.pycfn.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://ocr.ehwqpu.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cxj.jianghu66.top

Java: import java.util.List;
来源：http://ejt.ppjwa.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vdt.guannengcc.top

Ruby: require "json"; require_relative "./util"
来源：http://epp.jinghuilouyu.cn

C#:   using System.Text;
来源：http://nlk.pycfn.com

[C12] 立即执行函数 IIFE
来源：http://hxk.yueranfly.top

Py:   (lambda: print("run"))()
来源：http://rhx.hysaishi.cn

PHP:  (function () { echo "run"; })();
来源：http://ksz.yuanzhike.top

JS:   (() => { console.log("run"); })();
来源：http://hvr.chenzaomai.com

TS:   (() => { console.log("run"); })();
来源：http://spy.ywan-chungtsiang.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cfk.pycfn.com

Go:   func() { fmt.Println("run") }()
来源：http://rli.tarul.cn

Ruby: -> { puts "run" }.call
来源：http://fsf.xuetiantiany.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://igx.yonumen.top

[C13] 类型声明 / 类型注解
来源：http://idj.zhixingplan.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cxd.52xcode.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pnu.zdbjq.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bas.hywenlv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pyv.haohaochexian.top

Java: int add(int a, int b) { return a + b; }
来源：http://waq.daria6918.cn

Go:   func add(a, b int) int
来源：http://puc.fktsv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gfp.fengsongda.top

C#:   int Add(int a, int b) => a + b;
来源：http://kau.hywenlv.cn

[C14] 泛型函数
来源：http://sfx.epnwcf.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uhf.hesvh.cn

PHP:  // 无泛型
来源：http://kmn.hywenlv.cn

JS:   // 无泛型
来源：http://idc.aizwys.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jpw.gzhubu.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://znw.tianlin.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cbh.hysaishi.cn

Ruby: # 无泛型
来源：http://sjx.dashuyun.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xom.jiagoushi.top

[C15] 解构 / 展开参数
来源：http://mwj.hysaishi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://aob.kuanghao11.cn

PHP:  [$a, $b] = $pair;
来源：http://myx.gzhubu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bbt.hysaishi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tkw.havefunace.top

Java: // 无解构
来源：http://fzf.smart0.xyz

Go:   // 无解构
来源：http://wat.dianchejie.cn

Ruby: a, b = pair
来源：http://zrj.sufxvd.cn

C#:   var (a, b) = pair;
来源：http://bup.dashuyun.cn

[C16] 函数 / 方法重载
来源：http://wpv.52xcode.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kzu.kuanghao11.cn

PHP:  // 无重载
来源：http://pjy.iojbl.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://vyi.hywenlv.cn

TS:   // 用联合类型或重载签名声明
来源：http://bgk.ydzc1.top

Java: void f(int a) {}  void f(String a) {}
来源：http://fhe.ydzc1.top

Go:   // 无重载：用不同函数名
来源：http://fys.fehbvm.com

Ruby: # 无重载：靠动态参数
来源：http://sff.hnqzz.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://vup.quarkkingdee.top

================================================================================
来源：http://omi.mhx1999.top

D. 数组 / 列表 / 集合
来源：http://oar.chenzaomai.com

================================================================================
来源：http://aai.ydjk.org.cn

[D01] 创建数组 / 列表
来源：http://dcw.zhoulong.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://atg.smart0.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qvf.yongpay.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uzw.zhijiandao.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wwk.ydzc1.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zjm.tanke756.top

Go:   arr := []int{1, 2, 3}
来源：http://zij.tianlin.xyz

Ruby: arr = [1, 2, 3]
来源：http://emf.nanxuanxn.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://som.nwbrower.top

[D02] 追加元素到末尾
来源：http://jxy.cdnleiting.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jda.cdnleiting.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cux.vqdsnc.cn

JS:   arr.push(4);
来源：http://grg.feifeiyinyue.top

TS:   arr.push(4);
来源：http://sby.ydjk.org.cn

Java: list.add(4);
来源：http://sbx.zdqjudy.top

Go:   arr = append(arr, 4)
来源：http://egn.pengpengdd.cyou

Ruby: arr << 4; arr.push(5)
来源：http://rgc.quarkkingdee.top

C#:   list.Add(4);
来源：http://yhh.ehwqpu.com

[D03] 在指定位置插入元素
来源：http://ugy.cqqwz.cn

Py:   arr.insert(0, 0)
来源：http://esy.zhongyouzk.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://msn.sjlbkw.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://maw.smart0.xyz

TS:   arr.splice(0, 0, 0);
来源：http://yfs.uphjek.com

Java: list.add(0, 0);
来源：http://azx.vehdjk.com

Go:   arr = append([]int{0}, arr...)
来源：http://tir.yj20258.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uuu.ydjk.org.cn

C#:   list.Insert(0, 0);
来源：http://jtc.birdmap.top

[D04] 删除元素
来源：http://vyo.sysykeji.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://djj.ydjk.org.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://oom.vehdjk.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uyh.yj20258888.top

TS:   arr.splice(0, 1);
来源：http://pxy.gaohongyu789.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ekg.jqgfzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rqf.guowangkeji.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qbq.dianchejie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://chr.ivvv.top

[D05] 访问与修改元素
来源：http://dsh.hnxiangtu.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gro.ydjk.org.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mtk.zhengqikj.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dfy.ivvv.top

TS:   arr[0]; arr.at(-1);
来源：http://ynl.fanxiaobao.xyz

Java: list.get(0); list.set(0, 9);
来源：http://ywn.shanyushiyangtech.top

Go:   arr[0]; arr[0] = 9
来源：http://phs.gzhubu.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xka.guowangkeji.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gvn.yanxiufei.cn

[D06] 数组长度
来源：http://sph.shzxlz.cn

Py:   len(arr)
来源：http://qjo.dianchejie.cn

PHP:  count($arr);
来源：http://ceq.aibaodan.cn

JS:   arr.length
来源：http://mgr.meibo888.top

TS:   arr.length
来源：http://gft.uphjek.com

Java: list.size();
来源：http://zjw.cucudq.cn

Go:   len(arr)
来源：http://qww.iojbl.cn

Ruby: arr.length; arr.size
来源：http://cnl.zhijiandao.cn

C#:   list.Count;
来源：http://bao.yongpay.top

[D07] 切片 / 取子数组
来源：http://svt.xinyue.icu

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pym.xylfe.cn

PHP:  array_slice($arr, 1, 3);
来源：http://aun.zhoulong.xyz

JS:   arr.slice(1, 4);
来源：http://ewa.mhx1999.top

TS:   arr.slice(1, 4);
来源：http://xpq.hfpthk.cn

Java: list.subList(1, 4);
来源：http://sci.hysaishi.cn

Go:   arr[1:4]
来源：http://qxr.shuidangran.top

Ruby: arr[1, 3]
来源：http://pxy.bjfxy.top

C#:   list.GetRange(1, 3);
来源：http://tua.quarkkingdee.top

[D08] 合并两个数组
来源：http://fvm.wangdashe.top

Py:   a + b;  a.extend(b)
来源：http://kti.ybcxt.top

PHP:  array_merge($a, $b);
来源：http://ovr.shuidangran.top

JS:   [...a, ...b];  a.concat(b);
来源：http://vjs.jqgufenzy.top

TS:   [...a, ...b];
来源：http://esg.fktsv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bmd.ppjwa.cn

Go:   append(a, b...)
来源：http://rpu.ivvv.top

Ruby: a + b;  a.concat(b)
来源：http://evc.zdbjq.cn

C#:   a.Concat(b).ToList()
来源：http://fjn.jyoumei.cn

[D09] 排序（升序）
来源：http://ard.sjlbkw.cn

Py:   sorted(arr);  arr.sort()
来源：http://zjz.zhoulong.xyz

PHP:  sort($arr);
来源：http://liq.hammf.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hul.snrcjt.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://vvg.shzxlz.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ofx.tarul.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hdo.meibo888.top

Ruby: arr.sort
来源：http://pxz.ivvv.top

C#:   list.Sort();
来源：http://wts.sxryk.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://sex.fanxiaobao.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jsu.cqqwz.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nuy.havefunace.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ahe.cucudq.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tkw.shanyushiyangtech.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://abm.hammf.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hxa.zhoulong.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://flw.chenzaomai.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://usq.shangyingyoupin.top

[D11] 反转数组
来源：http://tzw.yj20258888.top

Py:   arr[::-1];  arr.reverse()
来源：http://srm.jianghu66.top

PHP:  array_reverse($arr);
来源：http://zub.gogol.net.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cal.zycfv.cn

TS:   [...arr].reverse();
来源：http://tvd.zhiwuduotai.top

Java: Collections.reverse(list);
来源：http://nxf.jiagoushi.top

Go:   slices.Reverse(arr)
来源：http://wev.bbcook.cn

Ruby: arr.reverse
来源：http://tix.sweek.top

C#:   list.Reverse();
来源：http://csz.yj20258888.top

[D12] 查找元素下标
来源：http://wvt.svipenyu.cn

Py:   arr.index(x);  x in arr
来源：http://umq.daria6918.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kbn.hywenlv.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rpr.cucudq.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mfz.cdnleiting.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zrt.yj20258.top

Go:   slices.Index(arr, x)
来源：http://bdi.yj20258.top

Ruby: arr.index(x)
来源：http://olv.bjfxy.top

C#:   list.IndexOf(x);
来源：http://gvm.xziqi.cn

[D13] 过滤（保留满足条件的）
来源：http://ony.iojbl.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jhn.chenjidiqi.icu

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://adb.hysaishi.cn

JS:   arr.filter(x => x > 3)
来源：http://izk.sweek.top

TS:   arr.filter(x => x > 3)
来源：http://agn.guowangkeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fch.zdqjudy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nfu.jqgfzy.top

Ruby: arr.select { |x| x > 3 }
来源：http://tjb.haohaochexian.top

C#:   list.Where(x => x > 3).ToList()
来源：http://uug.redwolf501.top

[D14] 映射转换（每个元素变形）
来源：http://xma.daria6918.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nni.gzhubu.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pdt.shuidangran.top

JS:   arr.map(x => x * 2)
来源：http://ydp.shanyushiyangkeji.top

TS:   arr.map(x => x * 2)
来源：http://yhb.0kj1m.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://yaj.kuanghao11.cn

Go:   // 手写循环
来源：http://dqy.daxiang520.top

Ruby: arr.map { |x| x * 2 }
来源：http://eby.svipenyu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://htz.ctjpmb.com

[D15] 去重
来源：http://xun.sysykeji.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pby.meibo888.top

PHP:  array_unique($arr);
来源：http://hws.jinqigufen.top

JS:   [...new Set(arr)]
来源：http://asr.yanxiufei.cn

TS:   [...new Set(arr)]
来源：http://gbj.aibaodan.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://oua.ivvv.top

Go:   // 用 map[T]struct{} 手写
来源：http://lcy.jlsjyb.cn

Ruby: arr.uniq
来源：http://bri.meibo888.top

C#:   list.Distinct().ToList()
来源：http://ngo.sxryk.cn

[D16] 求和与平均值
来源：http://jox.cqqwz.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qvf.jyoumei.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://iwd.feifeiyinyue.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zdw.fzhhl.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tod.xinyue.icu

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kyc.hnqzz.top

Go:   // 手写循环累加
来源：http://edz.sufxvd.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xdq.aibaodan.cn

C#:   list.Sum();  list.Average()
来源：http://yiy.tian-w.cn

[D17] 最大值与最小值
来源：http://skf.gogol.net.cn

Py:   max(arr);  min(arr)
来源：http://xfm.epnwcf.com

PHP:  max($arr);  min($arr);
来源：http://ayf.yfazqb.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yax.kuanghao11.cn

TS:   Math.max(...arr);
来源：http://kww.feifeiyinyue.top

Java: Collections.max(list);  Collections.min(list);
来源：http://wmr.zhiwuduotai.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xbp.yfazqb.com

Ruby: arr.max;  arr.min
来源：http://ovv.guannengcc.top

C#:   list.Max();  list.Min()
来源：http://tui.feifeiyinyue.top

[D18] 扁平化嵌套数组
来源：http://mde.yj20258.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ihs.xuanzx.com

PHP:  array_merge(...$nested);
来源：http://imx.zhongyouzk.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nmk.ppjwa.cn

TS:   nested.flat();
来源：http://tdn.wangshuangyany.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dna.sxryk.cn

Go:   // 手写双层循环
来源：http://cjb.uphjek.com

Ruby: nested.flatten
来源：http://zbc.tanke756.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://khm.yj20258.top

[D19] 按字段分组
来源：http://alc.hnxiangtu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://iar.shuidangran.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jdc.yonumen.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ezj.jinqigfzy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://dlw.shzxlz.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ypy.hnqzz.top

Go:   // 手写 map[string][]T
来源：http://jxw.jyoumei.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fgm.hywenlv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wek.xingfuxueyuan.xyz

[D20] 统计每个元素出现次数
来源：http://tgi.sysykeji.top

Py:   Counter(arr)
来源：http://cdb.jianghu66.top

PHP:  array_count_values($arr);
来源：http://ufm.epnwcf.com


<!-- 参考信息 -->