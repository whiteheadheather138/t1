代发 wailian999

================================================================================
来源：http://fqg.zhiwuduotai.top

C. 函数与作用域
来源：http://iaa.hnxiangtu.top

================================================================================
来源：http://ssi.zhengqikj.top

[C01] 定义函数
来源：http://ubi.dianchejie.cn

Py:   def add(a, b): return a + b
来源：http://sys.iojbl.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tpc.jinqigufen.top

JS:   function add(a, b) { return a + b; }
来源：http://hbb.shanyushiyangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iag.pycfn.com

Java: static int add(int a, int b) { return a + b; }
来源：http://aei.daria6918.cn

Go:   func add(a, b int) int { return a + b }
来源：http://pds.svipenyu.cn

Ruby: def add(a, b); a + b; end
来源：http://rcd.52xcode.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rtd.aibaodan.cn

[C02] 默认参数
来源：http://obh.tian-w.cn

Py:   def greet(name="World"): return name
来源：http://cet.xuanzx.com

PHP:  function greet($name = "World") { return $name; }
来源：http://llt.fzhhl.top

JS:   function greet(name = "World") { return name; }
来源：http://ulq.ppjwa.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bdl.vqdsnc.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cdi.sysykeji.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cfp.jinqigfzy.top

Ruby: def greet(name = "World") = name
来源：http://chz.zhengqikj.top

C#:   string Greet(string name = "World") => name;
来源：http://crz.andypj.xyz

[C03] 可变参数
来源：http://clh.yangfankeji.com

Py:   def total(*args): return sum(args)
来源：http://ehv.jlsjyb.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vxc.tanke756.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yzb.bbcook.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xvz.cheryme.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zyx.guowangkeji.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://joc.yvedp.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xyi.zhongyouzk.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bna.yangfankeji.com

[C04] 命名参数 / 关键字参数
来源：http://vks.yj20258.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bhe.hnqzz.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dtd.pengpengdd.cyou

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lpt.sufxvd.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jnc.aibaodan.cn

Java: // 无：用 Builder 模式或 record
来源：http://aqw.ctjpmb.com

Go:   // 无：用配置结构体参数
来源：http://jis.nwbrower.top

Ruby: f(a: 1, b: 2)
来源：http://bfz.ehwqpu.com

C#:   f(a: 1, b: 2)
来源：http://hpt.jinqigfzy.top

[C05] 返回多个值
来源：http://zij.hnxiangtu.top

Py:   return a, b
来源：http://tun.sxryk.cn

PHP:  return [$a, $b];
来源：http://tln.cashguo.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://cwf.hnxiangtu.top

TS:   return { a, b };
来源：http://jyb.uphjek.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qhc.birdmap.top

Go:   return a, b
来源：http://uca.birdmap.top

Ruby: return a, b
来源：http://vdg.jyoumei.cn

C#:   return (a, b);              // ValueTuple
来源：http://dhk.wangdashe.top

[C06] 匿名函数 / lambda
来源：http://bku.jyoumei.cn

Py:   square = lambda x: x * x
来源：http://okw.havefunace.top

PHP:  $square = fn($x) => $x * $x;
来源：http://jnp.chenlongwang.top

JS:   const square = x => x * x;
来源：http://dzq.haohaochexian.top

TS:   const square = (x: number): number => x * x;
来源：http://zti.kuanghao11.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cgx.yj20258888.top

Go:   sq := func(x int) int { return x * x }
来源：http://xwm.chenjidiqi.icu

Ruby: square = ->(x) { x * x }
来源：http://omu.shangyingyoupin.top

C#:   Func<int, int> square = x => x * x;
来源：http://bkl.dianchejie.cn

[C07] 把函数作为参数传入
来源：http://rzg.ivvv.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://aej.ivvv.top

PHP:  array_map("strtoupper", $arr);
来源：http://vrd.jinyuanbaomall.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pni.cucudq.cn

TS:   arr.map(String)
来源：http://ivf.yj20258888.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nak.shanyushiyangkeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://acp.zdbjq.cn

Ruby: arr.map(&:upcase)
来源：http://get.yfazqb.com

C#:   arr.Select(s => s.ToUpper())
来源：http://mpy.sjlbkw.cn

[C08] 闭包
来源：http://qoh.svipenyu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://skn.aizwys.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://saz.gaohongyu789.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://koy.cheryme.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pqi.zycfv.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hkt.hammf.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mix.vehdjk.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mjx.chenjidiqi.icu

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mkf.hnxiangtu.top

[C09] 递归
来源：http://hua.yanxiufei.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://heb.shzxlz.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qcu.daxiang520.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zle.haohaochexian.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ydf.xinyue.icu

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ezl.svipenyu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://iqo.fehbvm.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pjl.mhx1999.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qwm.jqgfzy.top

[C10] 变量作用域
来源：http://drs.smart0.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://guv.wangdashe.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dqf.xziqi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uzu.hongshengwenyu.top

TS:   同 JS
来源：http://aol.dashuyun.cn

Java: 方法内为块级作用域
来源：http://sxq.zdqjudy.top

Go:   花括号块级作用域
来源：http://fhd.zhengqikj.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ibl.xinyue.icu

C#:   块级作用域
来源：http://hce.yangfankeji.com

[C11] 模块导入与导出
来源：http://rlb.svipenyu.cn

Py:   from module import func
来源：http://lga.gaohongyu789.top

PHP:  require "file.php";  或 use App\Service;
来源：http://xwo.cdnleiting.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://lmx.ehwqpu.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://izg.vqdsnc.cn

Java: import java.util.List;
来源：http://htu.zdbjq.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://usq.sxryk.cn

Ruby: require "json"; require_relative "./util"
来源：http://gzl.vehdjk.com

C#:   using System.Text;
来源：http://sww.zhijiandao.cn

[C12] 立即执行函数 IIFE
来源：http://tao.ppjwa.cn

Py:   (lambda: print("run"))()
来源：http://fzn.daxiang520.top

PHP:  (function () { echo "run"; })();
来源：http://sju.meibo888.top

JS:   (() => { console.log("run"); })();
来源：http://smi.tian-w.cn

TS:   (() => { console.log("run"); })();
来源：http://fou.kuanghao11.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ncd.vqdsnc.cn

Go:   func() { fmt.Println("run") }()
来源：http://xqr.yongpay.top

Ruby: -> { puts "run" }.call
来源：http://cmm.shanyushiyangkeji.top

C#:   // 无 IIFE：用静态构造函数
来源：http://enu.andypj.xyz

[C13] 类型声明 / 类型注解
来源：http://jgp.meibo888.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gmg.svipenyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://alo.ybcxt.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tru.yuxming.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://brw.kuanghao11.cn

Java: int add(int a, int b) { return a + b; }
来源：http://hci.birdmap.top

Go:   func add(a, b int) int
来源：http://dax.iojbl.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hed.vqdsnc.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ibo.hammf.cn

[C14] 泛型函数
来源：http://qtk.aibaodan.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://oqf.sufxvd.cn

PHP:  // 无泛型
来源：http://uqw.zhaomingkeji.xyz

JS:   // 无泛型
来源：http://dlc.jinqigfzy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uhv.wangshuangyany.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tpb.nanxinkj.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cqw.sweek.top

Ruby: # 无泛型
来源：http://xhe.jqgfzy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lxj.xinyue.icu

[C15] 解构 / 展开参数
来源：http://wxx.jqgfzy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://phi.aizwys.cn

PHP:  [$a, $b] = $pair;
来源：http://czz.guannengcc.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rvd.zhijiandao.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hal.nanxuanxn.top

Java: // 无解构
来源：http://lhe.jinyuanbaomall.cn

Go:   // 无解构
来源：http://vjf.hnqzz.top

Ruby: a, b = pair
来源：http://pnw.wangdashe.top

C#:   var (a, b) = pair;
来源：http://ubn.redwolf501.top

[C16] 函数 / 方法重载
来源：http://bwx.nwbrower.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nzj.svipenyu.cn

PHP:  // 无重载
来源：http://ako.shanyushiyangtech.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://fbt.bjfxy.top

TS:   // 用联合类型或重载签名声明
来源：http://pee.vehdjk.com

Java: void f(int a) {}  void f(String a) {}
来源：http://zws.yj20258.top

Go:   // 无重载：用不同函数名
来源：http://wdp.daxiang520.top

Ruby: # 无重载：靠动态参数
来源：http://qic.uphjek.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://xpj.cqqwz.cn

================================================================================
来源：http://rlw.ybcxt.top

D. 数组 / 列表 / 集合
来源：http://rfv.ctjpmb.com

================================================================================
来源：http://caq.hongshengwenyu.top

[D01] 创建数组 / 列表
来源：http://eat.tanke756.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://hbo.daria6918.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tkt.svipenyu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zcw.hysaishi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://sjh.hesvh.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ken.iojbl.cn

Go:   arr := []int{1, 2, 3}
来源：http://fiv.nanxuanxn.top

Ruby: arr = [1, 2, 3]
来源：http://deo.tianlin.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://swk.ehwqpu.com

[D02] 追加元素到末尾
来源：http://klx.dashuyun.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ghs.nanxinkj.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nco.jiagoushi.top

JS:   arr.push(4);
来源：http://ktl.andypj.xyz

TS:   arr.push(4);
来源：http://rdc.ydzc1.top

Java: list.add(4);
来源：http://lej.pycfn.com

Go:   arr = append(arr, 4)
来源：http://mnt.snrcjt.cn

Ruby: arr << 4; arr.push(5)
来源：http://qpl.shangyingyoupin.top

C#:   list.Add(4);
来源：http://wrn.ctjpmb.com

[D03] 在指定位置插入元素
来源：http://rlu.ybcxt.top

Py:   arr.insert(0, 0)
来源：http://plj.yuanzhike.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gxu.zdqjudy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ldx.wangshuangyany.cn

TS:   arr.splice(0, 0, 0);
来源：http://ekg.ppjwa.cn

Java: list.add(0, 0);
来源：http://ahc.ppjwa.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qya.fengsongda.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://olk.fehbvm.com

C#:   list.Insert(0, 0);
来源：http://nao.ppjwa.cn

[D04] 删除元素
来源：http://awc.jlsjyb.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cca.chenlongwang.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://izb.fehbvm.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://khw.yanxiufei.cn

TS:   arr.splice(0, 1);
来源：http://pmu.ctjpmb.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sjk.chenzaomai.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cwz.dashuyun.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wvc.andypj.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cyu.fanxiaobao.xyz

[D05] 访问与修改元素
来源：http://pps.shzxlz.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ogw.xinyue.icu

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dhv.ybcxt.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ymh.yuanzhike.top

TS:   arr[0]; arr.at(-1);
来源：http://kbf.sufxvd.cn

Java: list.get(0); list.set(0, 9);
来源：http://vmd.ydjk.org.cn

Go:   arr[0]; arr[0] = 9
来源：http://rmu.smart0.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hoa.pengpengdd.cyou

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://znu.yanxiufei.cn

[D06] 数组长度
来源：http://das.jinqigfzy.top

Py:   len(arr)
来源：http://qwm.ydzc1.top

PHP:  count($arr);
来源：http://mda.zhixingplan.top

JS:   arr.length
来源：http://pix.cheryme.top

TS:   arr.length
来源：http://orb.sjlbkw.cn

Java: list.size();
来源：http://zzi.guowangkeji.top

Go:   len(arr)
来源：http://nzn.mhx1999.top

Ruby: arr.length; arr.size
来源：http://zcr.jinghuilouyu.cn

C#:   list.Count;
来源：http://bik.meibo888.top

[D07] 切片 / 取子数组
来源：http://czk.epnwcf.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xxr.fengsongda.top

PHP:  array_slice($arr, 1, 3);
来源：http://mru.yuxming.cn

JS:   arr.slice(1, 4);
来源：http://evd.haohaochexian.top

TS:   arr.slice(1, 4);
来源：http://lkp.yj20258.top

Java: list.subList(1, 4);
来源：http://fgv.sxryk.cn

Go:   arr[1:4]
来源：http://jwo.52xcode.cn

Ruby: arr[1, 3]
来源：http://sej.xylfe.cn

C#:   list.GetRange(1, 3);
来源：http://qwf.yongpay.top

[D08] 合并两个数组
来源：http://wim.sxryk.cn

Py:   a + b;  a.extend(b)
来源：http://txp.ctjpmb.com

PHP:  array_merge($a, $b);
来源：http://vrs.hywenlv.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qfm.shzxlz.cn

TS:   [...a, ...b];
来源：http://lfc.jinghuilouyu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vsg.yfazqb.com

Go:   append(a, b...)
来源：http://umr.zhixingplan.top

Ruby: a + b;  a.concat(b)
来源：http://vuo.svipenyu.cn

C#:   a.Concat(b).ToList()
来源：http://ynt.gaohongyu789.top

[D09] 排序（升序）
来源：http://hlm.havefunace.top

Py:   sorted(arr);  arr.sort()
来源：http://vzx.fengsongda.top

PHP:  sort($arr);
来源：http://cau.zhixingplan.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hvc.xziqi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://djr.yueranfly.top

Java: Collections.sort(list);  list.sort(null);
来源：http://etf.tian-w.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dcb.jiagoushi.top

Ruby: arr.sort
来源：http://qme.vqdsnc.cn

C#:   list.Sort();
来源：http://bht.jyoumei.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://wnp.guowangkeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ymu.gotoacloud.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jmn.tianlin.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://trj.aizwys.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rnx.9152youxi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://txv.yfazqb.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zhu.zhiwuduotai.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://btq.jlsjyb.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dwm.xziqi.cn

[D11] 反转数组
来源：http://gua.xuanzx.com

Py:   arr[::-1];  arr.reverse()
来源：http://sxb.gzhubu.top

PHP:  array_reverse($arr);
来源：http://uog.gzhubu.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://miz.yvedp.cn

TS:   [...arr].reverse();
来源：http://til.jinyuanbaomall.cn

Java: Collections.reverse(list);
来源：http://obp.uphjek.com

Go:   slices.Reverse(arr)
来源：http://iud.zdbjq.cn

Ruby: arr.reverse
来源：http://tri.xuetiantiany.cn

C#:   list.Reverse();
来源：http://lbo.nanxuanxn.top

[D12] 查找元素下标
来源：http://wgr.chenlongwang.top

Py:   arr.index(x);  x in arr
来源：http://qmb.chenzaomai.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dph.0kj1m.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dyp.c1oappe.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wcd.sjlbkw.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fvn.tanke756.top

Go:   slices.Index(arr, x)
来源：http://bmh.yanxiufei.cn

Ruby: arr.index(x)
来源：http://ptm.guowangkeji.top

C#:   list.IndexOf(x);
来源：http://lrq.9152youxi.cn

[D13] 过滤（保留满足条件的）
来源：http://wvj.wangdashe.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nby.chenjidiqi.icu

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://iym.ppjwa.cn

JS:   arr.filter(x => x > 3)
来源：http://lse.sxryk.cn

TS:   arr.filter(x => x > 3)
来源：http://cxg.xinyue.icu

Java: list.stream().filter(x -> x > 3).toList()
来源：http://imi.zhijiandao.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ywl.aibaodan.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tqf.yanxiufei.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ncj.cheryme.top

[D14] 映射转换（每个元素变形）
来源：http://jqz.xuetiantiany.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jub.dashuyun.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mer.hongshengwenyu.top

JS:   arr.map(x => x * 2)
来源：http://vpr.ctjpmb.com

TS:   arr.map(x => x * 2)
来源：http://kch.nwbrower.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://xdp.hesvh.cn

Go:   // 手写循环
来源：http://ycy.shanyushiyangkeji.top

Ruby: arr.map { |x| x * 2 }
来源：http://zoi.yueranfly.top

C#:   list.Select(x => x * 2).ToList()
来源：http://rnf.yangfankeji.com

[D15] 去重
来源：http://hxr.yj20258888.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wbj.yuxming.cn

PHP:  array_unique($arr);
来源：http://qst.sufxvd.cn

JS:   [...new Set(arr)]
来源：http://rla.jinqigufen.top

TS:   [...new Set(arr)]
来源：http://jyl.fehbvm.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://drj.xuanzx.com

Go:   // 用 map[T]struct{} 手写
来源：http://fmd.aibaodan.cn

Ruby: arr.uniq
来源：http://qrs.gotoacloud.top

C#:   list.Distinct().ToList()
来源：http://wff.ydjk.org.cn

[D16] 求和与平均值
来源：http://gpa.tian-w.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ejx.xinyue.icu

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hpo.zhiwuduotai.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vpn.tian-w.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zvo.zhixingplan.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sot.hfpthk.cn

Go:   // 手写循环累加
来源：http://tbp.xingfuxueyuan.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jsi.uphjek.com

C#:   list.Sum();  list.Average()
来源：http://lwn.cheryme.top

[D17] 最大值与最小值
来源：http://soe.daxiang520.top

Py:   max(arr);  min(arr)
来源：http://rie.mhx1999.top

PHP:  max($arr);  min($arr);
来源：http://zoh.hnxiangtu.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tgq.0kj1m.cn

TS:   Math.max(...arr);
来源：http://tlo.pycfn.com

Java: Collections.max(list);  Collections.min(list);
来源：http://gix.fktsv.cn


<!-- 参考信息 -->