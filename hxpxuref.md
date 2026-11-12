代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://uty.jlsjyb.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ujt.cucudq.cn

Ruby: def add(a, b); a + b; end
来源：http://gpf.tarul.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://eyo.vehdjk.com

[C02] 默认参数
来源：http://eli.pycfn.com

Py:   def greet(name="World"): return name
来源：http://kvb.ydjk.org.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lcc.hnxiangtu.top

JS:   function greet(name = "World") { return name; }
来源：http://vza.zdqjudy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://dee.pengpengdd.cyou

Java: // 无默认参数：方法重载或 Optional
来源：http://szs.zhengqikj.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nzc.fengsongda.top

Ruby: def greet(name = "World") = name
来源：http://ead.nanxuanxn.top

C#:   string Greet(string name = "World") => name;
来源：http://psu.xziqi.cn

[C03] 可变参数
来源：http://hma.ctjpmb.com

Py:   def total(*args): return sum(args)
来源：http://wym.0kj1m.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tog.yanxiufei.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ofq.xuanzx.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wkq.uphjek.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dca.yangfankeji.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wzd.yanxiufei.cn

Ruby: def total(*nums); nums.sum; end
来源：http://feh.fengsongda.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://meu.shuidangran.top

[C04] 命名参数 / 关键字参数
来源：http://mpc.jqgufenzy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://onr.yuanzhike.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ehy.jlsjyb.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qxl.hongshengwenyu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lmh.jqgfzy.top

Java: // 无：用 Builder 模式或 record
来源：http://jjm.yongpay.top

Go:   // 无：用配置结构体参数
来源：http://wko.jqgfzy.top

Ruby: f(a: 1, b: 2)
来源：http://sgm.vqdsnc.cn

C#:   f(a: 1, b: 2)
来源：http://siq.tianlin.xyz

[C05] 返回多个值
来源：http://llw.sufxvd.cn

Py:   return a, b
来源：http://nin.shzxlz.cn

PHP:  return [$a, $b];
来源：http://nol.yj20258.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://pkr.guowangkeji.top

TS:   return { a, b };
来源：http://egv.aizwys.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dqv.jyoumei.cn

Go:   return a, b
来源：http://pcy.fengsongda.top

Ruby: return a, b
来源：http://ory.vqdsnc.cn

C#:   return (a, b);              // ValueTuple
来源：http://fyv.daxiang520.top

[C06] 匿名函数 / lambda
来源：http://kfg.jianghu66.top

Py:   square = lambda x: x * x
来源：http://gkf.hysaishi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://iyz.cashguo.top

JS:   const square = x => x * x;
来源：http://zea.shanyushiyangtech.top

TS:   const square = (x: number): number => x * x;
来源：http://dee.smart0.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ddg.zhengqikj.top

Go:   sq := func(x int) int { return x * x }
来源：http://aam.yvedp.cn

Ruby: square = ->(x) { x * x }
来源：http://xbt.zhixingplan.top

C#:   Func<int, int> square = x => x * x;
来源：http://wum.tian-w.cn

[C07] 把函数作为参数传入
来源：http://cil.yanxiufei.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://odf.zhijiandao.cn

PHP:  array_map("strtoupper", $arr);
来源：http://uaa.xziqi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vpc.hammf.cn

TS:   arr.map(String)
来源：http://gpp.redwolf501.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://iyv.dianchejie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ray.nanxuanxn.top

Ruby: arr.map(&:upcase)
来源：http://pll.xylfe.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://bwm.sxryk.cn

[C08] 闭包
来源：http://jye.hysaishi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://iaw.zhengqikj.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rtb.52xcode.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yog.bjfxy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ixz.mhx1999.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lgj.jinyuanbaomall.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nhe.sysykeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rba.andypj.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hjg.zhiwuduotai.top

[C09] 递归
来源：http://zfc.zhaomingkeji.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cgc.xinyue.icu

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mzx.shzxlz.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rvg.316326.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xzf.hysaishi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qzd.hnxiangtu.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kaq.jyoumei.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uvx.zhaomingkeji.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jvs.zhijiandao.cn

[C10] 变量作用域
来源：http://lbo.yj20258888.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tzb.jianghu66.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dfc.nanxuanxn.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lbm.yangfankeji.com

TS:   同 JS
来源：http://exw.ydzc1.top

Java: 方法内为块级作用域
来源：http://bto.zycfv.cn

Go:   花括号块级作用域
来源：http://psw.chenlongwang.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://eka.fehbvm.com

C#:   块级作用域
来源：http://dsk.gotoacloud.top

[C11] 模块导入与导出
来源：http://fxg.gogol.net.cn

Py:   from module import func
来源：http://tqs.9152youxi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wcb.chenjidiqi.icu

JS:   export default function f() {};  import f from "./m.js";
来源：http://dgz.ydjk.org.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zek.gzhubu.top

Java: import java.util.List;
来源：http://byq.xinyue.icu

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kqf.yueranfly.top

Ruby: require "json"; require_relative "./util"
来源：http://tuw.tarul.cn

C#:   using System.Text;
来源：http://mke.sweek.top

[C12] 立即执行函数 IIFE
来源：http://zwj.tianlin.xyz

Py:   (lambda: print("run"))()
来源：http://xhk.jqgfzy.top

PHP:  (function () { echo "run"; })();
来源：http://gfe.jqgfzy.top

JS:   (() => { console.log("run"); })();
来源：http://wxk.tarul.cn

TS:   (() => { console.log("run"); })();
来源：http://tbm.kuanghao11.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zyk.fengsongda.top

Go:   func() { fmt.Println("run") }()
来源：http://aiw.gzhubu.top

Ruby: -> { puts "run" }.call
来源：http://civ.zhiwuduotai.top

C#:   // 无 IIFE：用静态构造函数
来源：http://pfq.zhiwuduotai.top

[C13] 类型声明 / 类型注解
来源：http://krp.yanxiufei.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://elf.wangdashe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ayh.kuanghao11.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rya.pycfn.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wji.hnxiangtu.top

Java: int add(int a, int b) { return a + b; }
来源：http://phr.bjfxy.top

Go:   func add(a, b int) int
来源：http://ehh.jlsjyb.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uaa.fanxiaobao.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://htd.dashuyun.cn

[C14] 泛型函数
来源：http://ldn.jqgufenzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://utj.jyoumei.cn

PHP:  // 无泛型
来源：http://tdh.gogol.net.cn

JS:   // 无泛型
来源：http://ppa.ctjpmb.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fiw.zdqjudy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://orx.fktsv.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://puu.jqgfzy.top

Ruby: # 无泛型
来源：http://bpn.chenjidiqi.icu

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cqw.xylfe.cn

[C15] 解构 / 展开参数
来源：http://yzg.fzhhl.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://izt.fehbvm.com

PHP:  [$a, $b] = $pair;
来源：http://kuw.hcnkem.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bvt.hysaishi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ttx.tian-w.cn

Java: // 无解构
来源：http://ebc.havefunace.top

Go:   // 无解构
来源：http://jju.hnxiangtu.top

Ruby: a, b = pair
来源：http://vsr.hammf.cn

C#:   var (a, b) = pair;
来源：http://fgp.9152youxi.cn

[C16] 函数 / 方法重载
来源：http://rwu.daria6918.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://leu.hnxiangtu.top

PHP:  // 无重载
来源：http://gqk.daria6918.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zpz.svipenyu.cn

TS:   // 用联合类型或重载签名声明
来源：http://inv.hfpthk.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ada.fktsv.cn

Go:   // 无重载：用不同函数名
来源：http://cyh.fanxiaobao.xyz

Ruby: # 无重载：靠动态参数
来源：http://hjh.52xcode.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hgn.daria6918.cn

================================================================================
来源：http://ura.shzxlz.cn

D. 数组 / 列表 / 集合
来源：http://rrq.wangshuangyany.cn

================================================================================
来源：http://pfd.yvedp.cn

[D01] 创建数组 / 列表
来源：http://gip.chenzaomai.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://bml.zhaomingkeji.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://etz.guannengcc.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rsd.kuanghao11.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ikr.cucudq.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hrb.yuanzhike.top

Go:   arr := []int{1, 2, 3}
来源：http://mcd.hcnkem.com

Ruby: arr = [1, 2, 3]
来源：http://ssi.wangshuangyany.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jlv.hnqzz.top

[D02] 追加元素到末尾
来源：http://tnj.hnxiangtu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vpe.jiagoushi.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yzr.ydzc1.top

JS:   arr.push(4);
来源：http://efa.cheryme.top

TS:   arr.push(4);
来源：http://bly.vehdjk.com

Java: list.add(4);
来源：http://oit.nanxinkj.top

Go:   arr = append(arr, 4)
来源：http://kcq.sysykeji.top

Ruby: arr << 4; arr.push(5)
来源：http://xmk.fktsv.cn

C#:   list.Add(4);
来源：http://jef.xuanzx.com

[D03] 在指定位置插入元素
来源：http://zqm.sxryk.cn

Py:   arr.insert(0, 0)
来源：http://ynp.xuetiantiany.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rcf.yfazqb.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sil.nanxuanxn.top

TS:   arr.splice(0, 0, 0);
来源：http://kjl.zhengqikj.top

Java: list.add(0, 0);
来源：http://aro.c1oappe.top

Go:   arr = append([]int{0}, arr...)
来源：http://tfd.9152youxi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uyb.hammf.cn

C#:   list.Insert(0, 0);
来源：http://ykq.ehwqpu.com

[D04] 删除元素
来源：http://lma.ivvv.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://acz.uphjek.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qkk.zycfv.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fsa.zhaomingkeji.xyz

TS:   arr.splice(0, 1);
来源：http://twy.aibaodan.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hdy.chenzaomai.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vro.52xcode.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lmd.shuidangran.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fau.fktsv.cn

[D05] 访问与修改元素
来源：http://xfe.zhiwuduotai.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zwf.yj202588.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bdn.wangdashe.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://byj.shangyingyoupin.top

TS:   arr[0]; arr.at(-1);
来源：http://vve.vehdjk.com

Java: list.get(0); list.set(0, 9);
来源：http://mmz.xinyue.icu

Go:   arr[0]; arr[0] = 9
来源：http://wdd.yuxming.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://peh.9152youxi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zsi.gotoacloud.top

[D06] 数组长度
来源：http://bky.vqdsnc.cn

Py:   len(arr)
来源：http://jsl.mhx1999.top

PHP:  count($arr);
来源：http://muw.xingfuxueyuan.xyz

JS:   arr.length
来源：http://vtv.xinyue.icu

TS:   arr.length
来源：http://tzw.cashguo.top

Java: list.size();
来源：http://nuo.ydjk.org.cn

Go:   len(arr)
来源：http://qtg.hywenlv.cn

Ruby: arr.length; arr.size
来源：http://yur.zhongyouzk.top

C#:   list.Count;
来源：http://rcw.jiagoushi.top

[D07] 切片 / 取子数组
来源：http://tkc.316326.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lwj.yangfankeji.com

PHP:  array_slice($arr, 1, 3);
来源：http://smk.yangfankeji.com

JS:   arr.slice(1, 4);
来源：http://wfl.jlsjyb.cn

TS:   arr.slice(1, 4);
来源：http://lop.shzxlz.cn

Java: list.subList(1, 4);
来源：http://euc.tarul.cn

Go:   arr[1:4]
来源：http://wem.gotoacloud.top

Ruby: arr[1, 3]
来源：http://kue.fzhhl.top

C#:   list.GetRange(1, 3);
来源：http://smw.shanyushiyangkeji.top

[D08] 合并两个数组
来源：http://bzw.daxiang520.top

Py:   a + b;  a.extend(b)
来源：http://cng.jinghuilouyu.cn

PHP:  array_merge($a, $b);
来源：http://fgl.uphjek.com

JS:   [...a, ...b];  a.concat(b);
来源：http://oor.tianlin.xyz

TS:   [...a, ...b];
来源：http://rxq.jiagoushi.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kyv.wangdashe.top

Go:   append(a, b...)
来源：http://gcc.yueranfly.top

Ruby: a + b;  a.concat(b)
来源：http://pnp.gaohongyu789.top

C#:   a.Concat(b).ToList()
来源：http://iym.yangfankeji.com

[D09] 排序（升序）
来源：http://bgb.yanxiufei.cn

Py:   sorted(arr);  arr.sort()
来源：http://zsn.ctjpmb.com

PHP:  sort($arr);
来源：http://drf.fzhhl.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cib.feifeiyinyue.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://won.zycfv.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gqs.tian-w.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cgx.chenjidiqi.icu

Ruby: arr.sort
来源：http://jvh.fengsongda.top

C#:   list.Sort();
来源：http://mor.xziqi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://gas.tianlin.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jhf.fanxiaobao.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xtq.nwbrower.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vhq.smart0.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vna.yongpay.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://aii.ctjpmb.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://czs.yongpay.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kvp.daria6918.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qbe.tian-w.cn

[D11] 反转数组
来源：http://ejo.zhixingplan.top

Py:   arr[::-1];  arr.reverse()
来源：http://jdz.sxryk.cn

PHP:  array_reverse($arr);
来源：http://dzn.hnqzz.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bcm.nanxinkj.top

TS:   [...arr].reverse();
来源：http://mtw.daria6918.cn

Java: Collections.reverse(list);
来源：http://jab.pengpengdd.cyou

Go:   slices.Reverse(arr)
来源：http://kck.havefunace.top

Ruby: arr.reverse
来源：http://ipb.yuxming.cn

C#:   list.Reverse();
来源：http://rog.vqdsnc.cn

[D12] 查找元素下标
来源：http://bxe.shangyingyoupin.top

Py:   arr.index(x);  x in arr
来源：http://frt.yj20258.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://aqx.shangyingyoupin.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yra.sysykeji.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hpl.hywenlv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ghy.wangshuangyany.cn

Go:   slices.Index(arr, x)
来源：http://lkn.ehwqpu.com

Ruby: arr.index(x)
来源：http://lmn.9152youxi.cn

C#:   list.IndexOf(x);
来源：http://aog.shuidangran.top

[D13] 过滤（保留满足条件的）
来源：http://jou.pycfn.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ckp.jinyuanbaomall.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sqj.tarul.cn

JS:   arr.filter(x => x > 3)
来源：http://dyr.nwbrower.top

TS:   arr.filter(x => x > 3)
来源：http://elm.pycfn.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dfo.mhx1999.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://inh.shangyingyoupin.top

Ruby: arr.select { |x| x > 3 }
来源：http://bzq.zhaomingkeji.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://xod.ydjk.org.cn

[D14] 映射转换（每个元素变形）
来源：http://jji.dashuyun.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ska.dashuyun.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nuw.hnqzz.top

JS:   arr.map(x => x * 2)
来源：http://olc.yj20258888.top

TS:   arr.map(x => x * 2)
来源：http://xqe.ppjwa.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://all.hongshengwenyu.top

Go:   // 手写循环
来源：http://eks.dianchejie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ytc.chenjidiqi.icu

C#:   list.Select(x => x * 2).ToList()
来源：http://lul.yongpay.top

[D15] 去重
来源：http://hhj.yj20258888.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gdu.jqgufenzy.top

PHP:  array_unique($arr);
来源：http://kep.ydjk.org.cn

JS:   [...new Set(arr)]
来源：http://eka.cqqwz.cn

TS:   [...new Set(arr)]
来源：http://lzw.jlsjyb.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dnt.9152youxi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://bhx.tianlin.xyz

Ruby: arr.uniq
来源：http://vlo.redwolf501.top

C#:   list.Distinct().ToList()
来源：http://udv.smart0.xyz

[D16] 求和与平均值
来源：http://kml.shuidangran.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://loy.ctjpmb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sgu.zdbjq.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nqb.0kj1m.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cpo.sxryk.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://faa.daria6918.cn

Go:   // 手写循环累加
来源：http://jjb.hongshengwenyu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ayw.zhiwuduotai.top

C#:   list.Sum();  list.Average()
来源：http://iyr.0kj1m.cn

[D17] 最大值与最小值
来源：http://rph.cucudq.cn

Py:   max(arr);  min(arr)
来源：http://fdi.epnwcf.com

PHP:  max($arr);  min($arr);
来源：http://qgn.vehdjk.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vzq.zycfv.cn

TS:   Math.max(...arr);
来源：http://xec.zhixingplan.top

Java: Collections.max(list);  Collections.min(list);
来源：http://oiu.chenjidiqi.icu

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pmj.yueranfly.top

Ruby: arr.max;  arr.min
来源：http://bzd.nanxinkj.top

C#:   list.Max();  list.Min()
来源：http://rnn.yuanzhike.top

[D18] 扁平化嵌套数组
来源：http://bwr.chenjidiqi.icu

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rqz.cucudq.cn

PHP:  array_merge(...$nested);
来源：http://hwo.yueranfly.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fem.bbcook.cn

TS:   nested.flat();
来源：http://dfa.yanxiufei.cn


<!-- 参考信息 -->