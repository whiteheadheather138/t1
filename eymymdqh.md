代发 wailian999

[C02] 默认参数
来源：http://ygx.hfpthk.cn

Py:   def greet(name="World"): return name
来源：http://jgv.fanxiaobao.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://dru.wangshuangyany.cn

JS:   function greet(name = "World") { return name; }
来源：http://muo.shzxlz.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://jbb.yj20258888.top

Java: // 无默认参数：方法重载或 Optional
来源：http://qfq.shuidangran.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bij.gaohongyu789.top

Ruby: def greet(name = "World") = name
来源：http://uae.52xcode.cn

C#:   string Greet(string name = "World") => name;
来源：http://mxi.hammf.cn

[C03] 可变参数
来源：http://hbo.jlsjyb.cn

Py:   def total(*args): return sum(args)
来源：http://kpj.guannengcc.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ypc.yueranfly.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dtq.yj20258.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yhd.pycfn.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pug.pycfn.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lew.hfpthk.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gyb.guowangkeji.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pnq.chenzaomai.com

[C04] 命名参数 / 关键字参数
来源：http://ses.pycfn.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mrx.meibo888.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ded.fzhhl.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gnd.pengpengdd.cyou

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lmf.haohaochexian.top

Java: // 无：用 Builder 模式或 record
来源：http://yvy.zycfv.cn

Go:   // 无：用配置结构体参数
来源：http://wtf.tarul.cn

Ruby: f(a: 1, b: 2)
来源：http://zuu.guannengcc.top

C#:   f(a: 1, b: 2)
来源：http://qtz.ivvv.top

[C05] 返回多个值
来源：http://rik.fktsv.cn

Py:   return a, b
来源：http://lij.hnqzz.top

PHP:  return [$a, $b];
来源：http://mhx.cucudq.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://naq.tian-w.cn

TS:   return { a, b };
来源：http://nig.meibo888.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ndc.shuidangran.top

Go:   return a, b
来源：http://adz.hnxiangtu.top

Ruby: return a, b
来源：http://epx.xylfe.cn

C#:   return (a, b);              // ValueTuple
来源：http://abf.hnxiangtu.top

[C06] 匿名函数 / lambda
来源：http://qlb.chenjidiqi.icu

Py:   square = lambda x: x * x
来源：http://qsj.yvedp.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://dmi.wangshuangyany.cn

JS:   const square = x => x * x;
来源：http://ybe.xuetiantiany.cn

TS:   const square = (x: number): number => x * x;
来源：http://xvz.nwbrower.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lee.smart0.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://qhq.ehwqpu.com

Ruby: square = ->(x) { x * x }
来源：http://lfs.nwbrower.top

C#:   Func<int, int> square = x => x * x;
来源：http://qts.yj20258.top

[C07] 把函数作为参数传入
来源：http://cts.jiagoushi.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ekv.gotoacloud.top

PHP:  array_map("strtoupper", $arr);
来源：http://gqr.hfpthk.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zom.zdqjudy.top

TS:   arr.map(String)
来源：http://lle.shzxlz.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ocj.jianghu66.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ftc.dianchejie.cn

Ruby: arr.map(&:upcase)
来源：http://bmk.hywenlv.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ynz.shuidangran.top

[C08] 闭包
来源：http://pmb.shangyingyoupin.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://upp.sxryk.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fas.yj202588.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tdd.hammf.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ktw.bbcook.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gcx.ydjk.org.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ruq.tian-w.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://glq.yvedp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ora.hcnkem.com

[C09] 递归
来源：http://kbu.quarkkingdee.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pei.zhiwuduotai.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sjk.52xcode.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xmb.ppjwa.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://krr.52xcode.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://opq.shangyingyoupin.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fbo.zhaomingkeji.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zuj.yuxming.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://viu.9152youxi.cn

[C10] 变量作用域
来源：http://jkt.cdnleiting.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ogq.yuanzhike.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lru.jqgfzy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mpw.cashguo.top

TS:   同 JS
来源：http://wpe.sweek.top

Java: 方法内为块级作用域
来源：http://lgd.yj20258.top

Go:   花括号块级作用域
来源：http://qix.xziqi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gns.mhx1999.top

C#:   块级作用域
来源：http://nmy.yanxiufei.cn

[C11] 模块导入与导出
来源：http://inv.aizwys.cn

Py:   from module import func
来源：http://opp.shanyushiyangtech.top

PHP:  require "file.php";  或 use App\Service;
来源：http://jgu.xingfuxueyuan.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://lsd.yj20258888.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bdh.guannengcc.top

Java: import java.util.List;
来源：http://ocx.tarul.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bwy.shanyushiyangtech.top

Ruby: require "json"; require_relative "./util"
来源：http://wnm.yongpay.top

C#:   using System.Text;
来源：http://tac.316326.xyz

[C12] 立即执行函数 IIFE
来源：http://vfr.zhengqikj.top

Py:   (lambda: print("run"))()
来源：http://dem.yangfankeji.com

PHP:  (function () { echo "run"; })();
来源：http://vwk.yj202588.top

JS:   (() => { console.log("run"); })();
来源：http://ktb.hcnkem.com

TS:   (() => { console.log("run"); })();
来源：http://bia.zhaomingkeji.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://obl.yangfankeji.com

Go:   func() { fmt.Println("run") }()
来源：http://ugm.aibaodan.cn

Ruby: -> { puts "run" }.call
来源：http://pin.gotoacloud.top

C#:   // 无 IIFE：用静态构造函数
来源：http://vco.yonumen.top

[C13] 类型声明 / 类型注解
来源：http://foc.jlsjyb.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://grx.zhoulong.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lhd.jqgufenzy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qbq.tian-w.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ygr.epnwcf.com

Java: int add(int a, int b) { return a + b; }
来源：http://aeb.yfazqb.com

Go:   func add(a, b int) int
来源：http://mqm.dashuyun.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qak.daria6918.cn

C#:   int Add(int a, int b) => a + b;
来源：http://coo.cqqwz.cn

[C14] 泛型函数
来源：http://ywm.fzhhl.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vdf.aizwys.cn

PHP:  // 无泛型
来源：http://rpk.yuxming.cn

JS:   // 无泛型
来源：http://kda.haohaochexian.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hbh.wangdashe.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wrm.tarul.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://uuj.jqgufenzy.top

Ruby: # 无泛型
来源：http://ivw.ppjwa.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gct.uphjek.com

[C15] 解构 / 展开参数
来源：http://tgl.fzhhl.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yds.daria6918.cn

PHP:  [$a, $b] = $pair;
来源：http://guq.uphjek.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kxj.hfpthk.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gly.guowangkeji.top

Java: // 无解构
来源：http://pdg.52xcode.cn

Go:   // 无解构
来源：http://dlu.fktsv.cn

Ruby: a, b = pair
来源：http://xcr.tarul.cn

C#:   var (a, b) = pair;
来源：http://poa.xuanzx.com

[C16] 函数 / 方法重载
来源：http://zvw.haohaochexian.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://axa.0kj1m.cn

PHP:  // 无重载
来源：http://bxe.hongshengwenyu.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://udd.yongpay.top

TS:   // 用联合类型或重载签名声明
来源：http://cry.hywenlv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://sgt.kuanghao11.cn

Go:   // 无重载：用不同函数名
来源：http://ppn.yongpay.top

Ruby: # 无重载：靠动态参数
来源：http://xut.feifeiyinyue.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://iyi.xinyue.icu

================================================================================
来源：http://vma.cheryme.top

D. 数组 / 列表 / 集合
来源：http://wpk.bbcook.cn

================================================================================
来源：http://nrg.sxryk.cn

[D01] 创建数组 / 列表
来源：http://jil.jinqigufen.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://usj.ehwqpu.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://acp.hammf.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zvu.bjfxy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://jjg.guannengcc.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pst.cqqwz.cn

Go:   arr := []int{1, 2, 3}
来源：http://hxr.gaohongyu789.top

Ruby: arr = [1, 2, 3]
来源：http://esh.zhiwuduotai.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jgu.fktsv.cn

[D02] 追加元素到末尾
来源：http://hnv.yvedp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xsy.daria6918.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wpg.9152youxi.cn

JS:   arr.push(4);
来源：http://qsf.fzhhl.top

TS:   arr.push(4);
来源：http://qfk.jinghuilouyu.cn

Java: list.add(4);
来源：http://qqd.yj20258.top

Go:   arr = append(arr, 4)
来源：http://tgd.daxiang520.top

Ruby: arr << 4; arr.push(5)
来源：http://pbc.xylfe.cn

C#:   list.Add(4);
来源：http://ciq.xinyue.icu

[D03] 在指定位置插入元素
来源：http://csr.yueranfly.top

Py:   arr.insert(0, 0)
来源：http://vyb.52xcode.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://shc.sysykeji.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jfx.smart0.xyz

TS:   arr.splice(0, 0, 0);
来源：http://kmi.tianlin.xyz

Java: list.add(0, 0);
来源：http://wid.jiagoushi.top

Go:   arr = append([]int{0}, arr...)
来源：http://lfi.feifeiyinyue.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tzr.epnwcf.com

C#:   list.Insert(0, 0);
来源：http://wqm.316326.xyz

[D04] 删除元素
来源：http://iqp.jinqigfzy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lye.snrcjt.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ycz.cucudq.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://udm.hammf.cn

TS:   arr.splice(0, 1);
来源：http://gkp.ehwqpu.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rbr.guannengcc.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qex.zhongyouzk.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gqw.jlsjyb.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yog.chenlongwang.top

[D05] 访问与修改元素
来源：http://hgi.sysykeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xxz.fengsongda.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uet.chenjidiqi.icu

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://okr.ybcxt.top

TS:   arr[0]; arr.at(-1);
来源：http://aqr.jqgfzy.top

Java: list.get(0); list.set(0, 9);
来源：http://bem.yuxming.cn

Go:   arr[0]; arr[0] = 9
来源：http://smq.yj20258888.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nnt.jianghu66.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yem.wangshuangyany.cn

[D06] 数组长度
来源：http://ory.epnwcf.com

Py:   len(arr)
来源：http://iul.hywenlv.cn

PHP:  count($arr);
来源：http://kpz.hcnkem.com

JS:   arr.length
来源：http://onq.wangdashe.top

TS:   arr.length
来源：http://cpn.zhaomingkeji.xyz

Java: list.size();
来源：http://txm.vehdjk.com

Go:   len(arr)
来源：http://kwl.chenzaomai.com

Ruby: arr.length; arr.size
来源：http://whr.316326.xyz

C#:   list.Count;
来源：http://olw.tanke756.top

[D07] 切片 / 取子数组
来源：http://drs.dashuyun.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qln.nanxinkj.top

PHP:  array_slice($arr, 1, 3);
来源：http://kjn.epnwcf.com

JS:   arr.slice(1, 4);
来源：http://moz.cashguo.top

TS:   arr.slice(1, 4);
来源：http://ghx.andypj.xyz

Java: list.subList(1, 4);
来源：http://dod.bjfxy.top

Go:   arr[1:4]
来源：http://zha.ydzc1.top

Ruby: arr[1, 3]
来源：http://fhd.52xcode.cn

C#:   list.GetRange(1, 3);
来源：http://vid.guowangkeji.top

[D08] 合并两个数组
来源：http://kgz.shuidangran.top

Py:   a + b;  a.extend(b)
来源：http://val.nwbrower.top

PHP:  array_merge($a, $b);
来源：http://nyh.ydjk.org.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://nrj.cucudq.cn

TS:   [...a, ...b];
来源：http://yjs.zdqjudy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xgz.quarkkingdee.top

Go:   append(a, b...)
来源：http://izl.feifeiyinyue.top

Ruby: a + b;  a.concat(b)
来源：http://nui.kuanghao11.cn

C#:   a.Concat(b).ToList()
来源：http://jby.zhoulong.xyz

[D09] 排序（升序）
来源：http://jve.nanxuanxn.top

Py:   sorted(arr);  arr.sort()
来源：http://yuh.xylfe.cn

PHP:  sort($arr);
来源：http://syq.pycfn.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hze.zhixingplan.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://vub.ybcxt.top

Java: Collections.sort(list);  list.sort(null);
来源：http://rtq.xziqi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://njq.hnxiangtu.top

Ruby: arr.sort
来源：http://tgz.jinqigufen.top

C#:   list.Sort();
来源：http://dze.zdqjudy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://gdk.aizwys.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zwy.xingfuxueyuan.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xrm.zdqjudy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mcc.uphjek.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kfk.tianlin.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://btl.jlsjyb.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://amd.ehwqpu.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cxu.kuanghao11.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mqw.uphjek.com

[D11] 反转数组
来源：http://dmf.nwbrower.top

Py:   arr[::-1];  arr.reverse()
来源：http://cfl.bjfxy.top

PHP:  array_reverse($arr);
来源：http://qdw.ydjk.org.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://veq.hnxiangtu.top

TS:   [...arr].reverse();
来源：http://cqm.vehdjk.com

Java: Collections.reverse(list);
来源：http://ejg.yueranfly.top

Go:   slices.Reverse(arr)
来源：http://fpw.tanke756.top

Ruby: arr.reverse
来源：http://ypy.ivvv.top

C#:   list.Reverse();
来源：http://lev.zhiwuduotai.top

[D12] 查找元素下标
来源：http://xpp.xinyue.icu

Py:   arr.index(x);  x in arr
来源：http://ryg.snrcjt.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bnw.hfpthk.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qnb.snrcjt.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uaz.hnxiangtu.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://knh.jinyuanbaomall.cn

Go:   slices.Index(arr, x)
来源：http://xgm.vqdsnc.cn

Ruby: arr.index(x)
来源：http://yyt.tian-w.cn

C#:   list.IndexOf(x);
来源：http://cmb.hcnkem.com

[D13] 过滤（保留满足条件的）
来源：http://mvx.ctjpmb.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kwi.yongpay.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ycm.svipenyu.cn

JS:   arr.filter(x => x > 3)
来源：http://urs.fehbvm.com

TS:   arr.filter(x => x > 3)
来源：http://mjy.ybcxt.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rvd.zhongyouzk.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cjf.ydjk.org.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tit.hongshengwenyu.top

C#:   list.Where(x => x > 3).ToList()
来源：http://rnm.pycfn.com

[D14] 映射转换（每个元素变形）
来源：http://ivl.gotoacloud.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qqw.gotoacloud.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dgw.52xcode.cn

JS:   arr.map(x => x * 2)
来源：http://hfe.nanxinkj.top

TS:   arr.map(x => x * 2)
来源：http://njp.jqgfzy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://jxg.chenzaomai.com

Go:   // 手写循环
来源：http://fmf.haohaochexian.top

Ruby: arr.map { |x| x * 2 }
来源：http://lzg.shangyingyoupin.top

C#:   list.Select(x => x * 2).ToList()
来源：http://kjz.hesvh.cn

[D15] 去重
来源：http://kek.tian-w.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://aam.ppjwa.cn

PHP:  array_unique($arr);
来源：http://tqt.hywenlv.cn

JS:   [...new Set(arr)]
来源：http://rcc.xuanzx.com

TS:   [...new Set(arr)]
来源：http://jig.cucudq.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zck.sweek.top

Go:   // 用 map[T]struct{} 手写
来源：http://ick.hfpthk.cn

Ruby: arr.uniq
来源：http://tdj.gaohongyu789.top

C#:   list.Distinct().ToList()
来源：http://xtt.yongpay.top

[D16] 求和与平均值
来源：http://rnv.xylfe.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zzb.wangshuangyany.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bfv.hywenlv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kmj.shanyushiyangtech.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vzs.yuxming.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bee.hnqzz.top

Go:   // 手写循环累加
来源：http://zfq.zycfv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hxl.nwbrower.top

C#:   list.Sum();  list.Average()
来源：http://tig.nanxuanxn.top

[D17] 最大值与最小值
来源：http://xxa.ydzc1.top

Py:   max(arr);  min(arr)
来源：http://qcj.hywenlv.cn

PHP:  max($arr);  min($arr);
来源：http://mro.c1oappe.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jft.gogol.net.cn

TS:   Math.max(...arr);
来源：http://exc.zhoulong.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://jxs.shangyingyoupin.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qqm.gotoacloud.top

Ruby: arr.max;  arr.min
来源：http://lvm.gaohongyu789.top

C#:   list.Max();  list.Min()
来源：http://xmi.bjfxy.top

[D18] 扁平化嵌套数组
来源：http://gov.cqqwz.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nrs.mhx1999.top

PHP:  array_merge(...$nested);
来源：http://dbv.snrcjt.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jxd.tian-w.cn

TS:   nested.flat();
来源：http://emg.ydzc1.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hjj.iojbl.cn

Go:   // 手写双层循环
来源：http://gyf.zdbjq.cn

Ruby: nested.flatten
来源：http://zon.fengsongda.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://bin.gzhubu.top


<!-- 参考信息 -->