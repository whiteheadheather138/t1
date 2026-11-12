代发 wailian999

================================================================================
来源：http://liu.gogol.net.cn

C. 函数与作用域
来源：http://vig.guowangkeji.top

================================================================================
来源：http://rbz.tanke756.top

[C01] 定义函数
来源：http://urx.daria6918.cn

Py:   def add(a, b): return a + b
来源：http://dic.fzhhl.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://heg.pycfn.com

JS:   function add(a, b) { return a + b; }
来源：http://rux.zhengqikj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kwi.dianchejie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://llg.birdmap.top

Go:   func add(a, b int) int { return a + b }
来源：http://oba.ybcxt.top

Ruby: def add(a, b); a + b; end
来源：http://pff.fehbvm.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tiy.sxryk.cn

[C02] 默认参数
来源：http://nmg.nwbrower.top

Py:   def greet(name="World"): return name
来源：http://lwp.vqdsnc.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cyx.gzhubu.top

JS:   function greet(name = "World") { return name; }
来源：http://abq.tanke756.top

TS:   function greet(name: string = "World") { return name; }
来源：http://uen.yj20258.top

Java: // 无默认参数：方法重载或 Optional
来源：http://cxd.yangfankeji.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zqq.mhx1999.top

Ruby: def greet(name = "World") = name
来源：http://vpm.zycfv.cn

C#:   string Greet(string name = "World") => name;
来源：http://wiq.cucudq.cn

[C03] 可变参数
来源：http://tfa.ybcxt.top

Py:   def total(*args): return sum(args)
来源：http://uhc.dashuyun.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zmg.xingfuxueyuan.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xfi.ybcxt.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pmo.mhx1999.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bdv.daxiang520.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hwx.gzhubu.top

Ruby: def total(*nums); nums.sum; end
来源：http://klc.daxiang520.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rpr.yanxiufei.cn

[C04] 命名参数 / 关键字参数
来源：http://okq.daria6918.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zpc.aizwys.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qab.sxryk.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ggf.gzhubu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uuu.hysaishi.cn

Java: // 无：用 Builder 模式或 record
来源：http://zsf.jinyuanbaomall.cn

Go:   // 无：用配置结构体参数
来源：http://cwr.smart0.xyz

Ruby: f(a: 1, b: 2)
来源：http://lwf.jiagoushi.top

C#:   f(a: 1, b: 2)
来源：http://ldk.tianlin.xyz

[C05] 返回多个值
来源：http://yah.zhengqikj.top

Py:   return a, b
来源：http://tcd.c1oappe.top

PHP:  return [$a, $b];
来源：http://bxt.vqdsnc.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://iyd.ydzc1.top

TS:   return { a, b };
来源：http://htw.guowangkeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://spn.chenzaomai.com

Go:   return a, b
来源：http://aul.chenlongwang.top

Ruby: return a, b
来源：http://vag.ehwqpu.com

C#:   return (a, b);              // ValueTuple
来源：http://kng.pycfn.com

[C06] 匿名函数 / lambda
来源：http://vum.yj202588.top

Py:   square = lambda x: x * x
来源：http://sul.zhaomingkeji.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://xbr.nwbrower.top

JS:   const square = x => x * x;
来源：http://quv.ywan-chungtsiang.top

TS:   const square = (x: number): number => x * x;
来源：http://yiz.fzhhl.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blm.zdqjudy.top

Go:   sq := func(x int) int { return x * x }
来源：http://njj.ydzc1.top

Ruby: square = ->(x) { x * x }
来源：http://sol.dianchejie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://rke.quarkkingdee.top

[C07] 把函数作为参数传入
来源：http://mcc.tian-w.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mbd.jinyuanbaomall.cn

PHP:  array_map("strtoupper", $arr);
来源：http://lal.yangfankeji.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sfu.yfazqb.com

TS:   arr.map(String)
来源：http://uly.kuanghao11.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jjm.tianlin.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kgf.feifeiyinyue.top

Ruby: arr.map(&:upcase)
来源：http://nud.vqdsnc.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://bxq.yanxiufei.cn

[C08] 闭包
来源：http://ixw.sufxvd.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uci.havefunace.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sba.jqgfzy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yrj.shuidangran.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dns.meibo888.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qos.dianchejie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cff.guannengcc.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vfi.zhengqikj.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://iwq.xuetiantiany.cn

[C09] 递归
来源：http://vok.fanxiaobao.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qka.yonumen.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ali.jqgfzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rlq.bbcook.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kux.xziqi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mpq.ivvv.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lvq.316326.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ssa.0kj1m.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://eld.guannengcc.top

[C10] 变量作用域
来源：http://kwf.cqqwz.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mts.gotoacloud.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ptx.zhiwuduotai.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hep.jqgufenzy.top

TS:   同 JS
来源：http://cxz.fehbvm.com

Java: 方法内为块级作用域
来源：http://ixd.svipenyu.cn

Go:   花括号块级作用域
来源：http://gxi.yfazqb.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://adz.smart0.xyz

C#:   块级作用域
来源：http://oty.vqdsnc.cn

[C11] 模块导入与导出
来源：http://qzs.yonumen.top

Py:   from module import func
来源：http://ekp.havefunace.top

PHP:  require "file.php";  或 use App\Service;
来源：http://zai.jinqigfzy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://wdp.tanke756.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xat.xylfe.cn

Java: import java.util.List;
来源：http://cob.dianchejie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xlh.xylfe.cn

Ruby: require "json"; require_relative "./util"
来源：http://tbh.pengpengdd.cyou

C#:   using System.Text;
来源：http://for.guannengcc.top

[C12] 立即执行函数 IIFE
来源：http://rmk.jlsjyb.cn

Py:   (lambda: print("run"))()
来源：http://nbr.hnxiangtu.top

PHP:  (function () { echo "run"; })();
来源：http://ywa.xylfe.cn

JS:   (() => { console.log("run"); })();
来源：http://iag.gaohongyu789.top

TS:   (() => { console.log("run"); })();
来源：http://baa.yongpay.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fly.ehwqpu.com

Go:   func() { fmt.Println("run") }()
来源：http://orl.hywenlv.cn

Ruby: -> { puts "run" }.call
来源：http://xps.xingfuxueyuan.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://upi.jyoumei.cn

[C13] 类型声明 / 类型注解
来源：http://hid.yuanzhike.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rig.cucudq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hkj.jqgfzy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://oie.sufxvd.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lhr.cqqwz.cn

Java: int add(int a, int b) { return a + b; }
来源：http://afs.vqdsnc.cn

Go:   func add(a, b int) int
来源：http://jlg.hysaishi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wnu.hongshengwenyu.top

C#:   int Add(int a, int b) => a + b;
来源：http://acs.dianchejie.cn

[C14] 泛型函数
来源：http://cfc.guannengcc.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dws.fzhhl.top

PHP:  // 无泛型
来源：http://svy.zhiwuduotai.top

JS:   // 无泛型
来源：http://gow.cqqwz.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jdg.xziqi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ivt.guowangkeji.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pki.andypj.xyz

Ruby: # 无泛型
来源：http://klq.wangdashe.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dli.zhixingplan.top

[C15] 解构 / 展开参数
来源：http://exm.shangyingyoupin.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://uly.xingfuxueyuan.xyz

PHP:  [$a, $b] = $pair;
来源：http://qqc.52xcode.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qko.andypj.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zev.guowangkeji.top

Java: // 无解构
来源：http://exv.ywan-chungtsiang.top

Go:   // 无解构
来源：http://jsx.shanyushiyangtech.top

Ruby: a, b = pair
来源：http://qmq.zhaomingkeji.xyz

C#:   var (a, b) = pair;
来源：http://mdv.xuanzx.com

[C16] 函数 / 方法重载
来源：http://xyg.cucudq.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://itl.yj202588.top

PHP:  // 无重载
来源：http://qlj.hnxiangtu.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://tms.shzxlz.cn

TS:   // 用联合类型或重载签名声明
来源：http://sxr.yongpay.top

Java: void f(int a) {}  void f(String a) {}
来源：http://pju.bbcook.cn

Go:   // 无重载：用不同函数名
来源：http://ypu.zhiwuduotai.top

Ruby: # 无重载：靠动态参数
来源：http://wer.jqgfzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://cjb.hcnkem.com

================================================================================
来源：http://mig.zhaomingkeji.xyz

D. 数组 / 列表 / 集合
来源：http://gmn.yj202588.top

================================================================================
来源：http://fya.yuxming.cn

[D01] 创建数组 / 列表
来源：http://lsp.vqdsnc.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xga.fengsongda.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dgj.pycfn.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yht.wangdashe.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://oqz.uphjek.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yez.zhixingplan.top

Go:   arr := []int{1, 2, 3}
来源：http://rev.hammf.cn

Ruby: arr = [1, 2, 3]
来源：http://tqj.yuanzhike.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ima.birdmap.top

[D02] 追加元素到末尾
来源：http://wxj.ybcxt.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ejx.shuidangran.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ihl.yongpay.top

JS:   arr.push(4);
来源：http://ump.cheryme.top

TS:   arr.push(4);
来源：http://lkn.cdnleiting.top

Java: list.add(4);
来源：http://vxq.yanxiufei.cn

Go:   arr = append(arr, 4)
来源：http://wpb.gzhubu.top

Ruby: arr << 4; arr.push(5)
来源：http://ksd.sysykeji.top

C#:   list.Add(4);
来源：http://ikd.jinqigfzy.top

[D03] 在指定位置插入元素
来源：http://foy.yj202588.top

Py:   arr.insert(0, 0)
来源：http://uvg.redwolf501.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xwk.shzxlz.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://apa.zhaomingkeji.xyz

TS:   arr.splice(0, 0, 0);
来源：http://zri.zhaomingkeji.xyz

Java: list.add(0, 0);
来源：http://sdu.xinyue.icu

Go:   arr = append([]int{0}, arr...)
来源：http://avd.hcnkem.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://epz.nanxinkj.top

C#:   list.Insert(0, 0);
来源：http://srg.vehdjk.com

[D04] 删除元素
来源：http://pkl.tian-w.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://eak.chenzaomai.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mkk.ybcxt.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gvs.jinqigfzy.top

TS:   arr.splice(0, 1);
来源：http://ezu.yongpay.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gcl.meibo888.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nqr.daria6918.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mfx.jlsjyb.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jeb.bbcook.cn

[D05] 访问与修改元素
来源：http://vpk.shanyushiyangtech.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tsi.xziqi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jyt.sweek.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qgg.sweek.top

TS:   arr[0]; arr.at(-1);
来源：http://cvs.zhongyouzk.top

Java: list.get(0); list.set(0, 9);
来源：http://xdv.quarkkingdee.top

Go:   arr[0]; arr[0] = 9
来源：http://ukc.xinyue.icu

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uce.cqqwz.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lgs.zhaomingkeji.xyz

[D06] 数组长度
来源：http://bub.daria6918.cn

Py:   len(arr)
来源：http://rzl.ehwqpu.com

PHP:  count($arr);
来源：http://chn.hnxiangtu.top

JS:   arr.length
来源：http://crw.aibaodan.cn

TS:   arr.length
来源：http://bmd.ydjk.org.cn

Java: list.size();
来源：http://yer.9152youxi.cn

Go:   len(arr)
来源：http://gag.chenzaomai.com

Ruby: arr.length; arr.size
来源：http://qva.0kj1m.cn

C#:   list.Count;
来源：http://yez.quarkkingdee.top

[D07] 切片 / 取子数组
来源：http://vnk.guannengcc.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wxb.yfazqb.com

PHP:  array_slice($arr, 1, 3);
来源：http://erx.vehdjk.com

JS:   arr.slice(1, 4);
来源：http://uta.tian-w.cn

TS:   arr.slice(1, 4);
来源：http://yyp.jqgfzy.top

Java: list.subList(1, 4);
来源：http://slh.iojbl.cn

Go:   arr[1:4]
来源：http://gfk.yuxming.cn

Ruby: arr[1, 3]
来源：http://agm.tarul.cn

C#:   list.GetRange(1, 3);
来源：http://rvo.gotoacloud.top

[D08] 合并两个数组
来源：http://yzc.ybcxt.top

Py:   a + b;  a.extend(b)
来源：http://oov.hnxiangtu.top

PHP:  array_merge($a, $b);
来源：http://tnq.sxryk.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://col.zdqjudy.top

TS:   [...a, ...b];
来源：http://cch.zhixingplan.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gle.gogol.net.cn

Go:   append(a, b...)
来源：http://lxb.yanxiufei.cn

Ruby: a + b;  a.concat(b)
来源：http://rkg.yonumen.top

C#:   a.Concat(b).ToList()
来源：http://aqs.cucudq.cn

[D09] 排序（升序）
来源：http://hdk.xylfe.cn

Py:   sorted(arr);  arr.sort()
来源：http://wkz.gotoacloud.top

PHP:  sort($arr);
来源：http://dmj.yangfankeji.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nsd.nanxuanxn.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://thj.kuanghao11.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mbt.feifeiyinyue.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://slq.shuidangran.top

Ruby: arr.sort
来源：http://ryt.ehwqpu.com

C#:   list.Sort();
来源：http://ldv.sxryk.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zep.zhixingplan.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mmu.birdmap.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vyn.yuanzhike.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qug.daxiang520.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fwz.zhijiandao.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rot.nanxinkj.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ipj.vqdsnc.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://iyc.yfazqb.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qzg.gogol.net.cn

[D11] 反转数组
来源：http://lie.jiagoushi.top

Py:   arr[::-1];  arr.reverse()
来源：http://ytt.jianghu66.top

PHP:  array_reverse($arr);
来源：http://gks.jqgfzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uqn.sweek.top

TS:   [...arr].reverse();
来源：http://vkb.dianchejie.cn

Java: Collections.reverse(list);
来源：http://kfm.cqqwz.cn

Go:   slices.Reverse(arr)
来源：http://zxx.chenlongwang.top

Ruby: arr.reverse
来源：http://auj.feifeiyinyue.top

C#:   list.Reverse();
来源：http://nco.dianchejie.cn

[D12] 查找元素下标
来源：http://eit.hcnkem.com

Py:   arr.index(x);  x in arr
来源：http://tsr.hesvh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rgw.shzxlz.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://myr.9152youxi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xvj.jlsjyb.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vpg.gotoacloud.top

Go:   slices.Index(arr, x)
来源：http://joi.zhoulong.xyz

Ruby: arr.index(x)
来源：http://hyo.cheryme.top

C#:   list.IndexOf(x);
来源：http://gdc.gzhubu.top

[D13] 过滤（保留满足条件的）
来源：http://won.aizwys.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xjp.tanke756.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://eza.hywenlv.cn

JS:   arr.filter(x => x > 3)
来源：http://guw.yj20258.top

TS:   arr.filter(x => x > 3)
来源：http://szo.jiagoushi.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xot.quarkkingdee.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://csl.nanxinkj.top

Ruby: arr.select { |x| x > 3 }
来源：http://zeu.zdqjudy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://swr.jqgfzy.top

[D14] 映射转换（每个元素变形）
来源：http://mdk.bbcook.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xzz.pengpengdd.cyou

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mod.hfpthk.cn

JS:   arr.map(x => x * 2)
来源：http://jrd.52xcode.cn

TS:   arr.map(x => x * 2)
来源：http://zjc.xylfe.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ytf.pycfn.com

Go:   // 手写循环
来源：http://bbf.tian-w.cn

Ruby: arr.map { |x| x * 2 }
来源：http://kjn.bjfxy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ijg.redwolf501.top

[D15] 去重
来源：http://zgu.yueranfly.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sot.daria6918.cn

PHP:  array_unique($arr);
来源：http://hay.vqdsnc.cn

JS:   [...new Set(arr)]
来源：http://fym.epnwcf.com

TS:   [...new Set(arr)]
来源：http://prh.ctjpmb.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://eha.smart0.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://zyx.zhoulong.xyz

Ruby: arr.uniq
来源：http://ecs.jinqigfzy.top

C#:   list.Distinct().ToList()
来源：http://wpj.tianlin.xyz

[D16] 求和与平均值
来源：http://mou.jinqigfzy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://diu.shzxlz.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qpu.zycfv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mny.zycfv.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xgi.zhijiandao.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ctd.gotoacloud.top

Go:   // 手写循环累加
来源：http://pel.ydjk.org.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jzo.chenlongwang.top

C#:   list.Sum();  list.Average()
来源：http://yjz.guannengcc.top

[D17] 最大值与最小值
来源：http://jhs.gogol.net.cn

Py:   max(arr);  min(arr)
来源：http://byt.yuxming.cn

PHP:  max($arr);  min($arr);
来源：http://zba.ppjwa.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wio.daxiang520.top

TS:   Math.max(...arr);
来源：http://olz.bbcook.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://vku.jinqigfzy.top


<!-- 参考信息 -->