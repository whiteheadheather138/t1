代发 wailian999

================================================================================
来源：http://vgj.chenlongwang.top

C. 函数与作用域
来源：http://axv.havefunace.top

================================================================================
来源：http://qrj.sxryk.cn

[C01] 定义函数
来源：http://ukt.fanxiaobao.xyz

Py:   def add(a, b): return a + b
来源：http://gid.yuanzhike.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cfy.ywan-chungtsiang.top

JS:   function add(a, b) { return a + b; }
来源：http://yoz.hywenlv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nwr.daria6918.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vkb.pycfn.com

Go:   func add(a, b int) int { return a + b }
来源：http://iat.jqgfzy.top

Ruby: def add(a, b); a + b; end
来源：http://jhw.wangdashe.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ylo.hongshengwenyu.top

[C02] 默认参数
来源：http://wby.316326.xyz

Py:   def greet(name="World"): return name
来源：http://oez.yuxming.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://oii.jinqigfzy.top

JS:   function greet(name = "World") { return name; }
来源：http://smd.daxiang520.top

TS:   function greet(name: string = "World") { return name; }
来源：http://esw.iojbl.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://neu.zhiwuduotai.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yaa.meibo888.top

Ruby: def greet(name = "World") = name
来源：http://jpb.dashuyun.cn

C#:   string Greet(string name = "World") => name;
来源：http://lbs.tian-w.cn

[C03] 可变参数
来源：http://qop.ydjk.org.cn

Py:   def total(*args): return sum(args)
来源：http://gyp.tian-w.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://onn.yanxiufei.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bng.quarkkingdee.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://map.zhoulong.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://plz.xinyue.icu

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://okr.feifeiyinyue.top

Ruby: def total(*nums); nums.sum; end
来源：http://ewv.jqgufenzy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rzr.sweek.top

[C04] 命名参数 / 关键字参数
来源：http://gus.shanyushiyangkeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ijk.yuanzhike.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rbo.ehwqpu.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fnw.sufxvd.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tpv.fanxiaobao.xyz

Java: // 无：用 Builder 模式或 record
来源：http://cto.yuanzhike.top

Go:   // 无：用配置结构体参数
来源：http://yxr.ppjwa.cn

Ruby: f(a: 1, b: 2)
来源：http://gzk.zdqjudy.top

C#:   f(a: 1, b: 2)
来源：http://fkd.0kj1m.cn

[C05] 返回多个值
来源：http://xko.dianchejie.cn

Py:   return a, b
来源：http://iya.xylfe.cn

PHP:  return [$a, $b];
来源：http://evv.tanke756.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://iph.andypj.xyz

TS:   return { a, b };
来源：http://yqp.sweek.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xcy.iojbl.cn

Go:   return a, b
来源：http://cwq.ctjpmb.com

Ruby: return a, b
来源：http://tud.yj202588.top

C#:   return (a, b);              // ValueTuple
来源：http://kui.wangdashe.top

[C06] 匿名函数 / lambda
来源：http://yxv.yongpay.top

Py:   square = lambda x: x * x
来源：http://mix.hywenlv.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ufl.shzxlz.cn

JS:   const square = x => x * x;
来源：http://rey.hongshengwenyu.top

TS:   const square = (x: number): number => x * x;
来源：http://zdd.yvedp.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://klb.yj20258888.top

Go:   sq := func(x int) int { return x * x }
来源：http://abf.kuanghao11.cn

Ruby: square = ->(x) { x * x }
来源：http://ppn.jianghu66.top

C#:   Func<int, int> square = x => x * x;
来源：http://uty.ybcxt.top

[C07] 把函数作为参数传入
来源：http://hhf.shanyushiyangkeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bbc.hnqzz.top

PHP:  array_map("strtoupper", $arr);
来源：http://vnz.9152youxi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://juk.chenjidiqi.icu

TS:   arr.map(String)
来源：http://rma.wangshuangyany.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bfg.cashguo.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mev.hammf.cn

Ruby: arr.map(&:upcase)
来源：http://dnk.sweek.top

C#:   arr.Select(s => s.ToUpper())
来源：http://npq.gzhubu.top

[C08] 闭包
来源：http://xjs.zhengqikj.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ioa.yfazqb.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vxo.nanxuanxn.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nwd.shzxlz.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qkm.shuidangran.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://swn.yanxiufei.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bry.yj202588.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://upy.shuidangran.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kai.vehdjk.com

[C09] 递归
来源：http://efr.tanke756.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bdr.zhongyouzk.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://egn.jinyuanbaomall.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vok.jiagoushi.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yqa.shanyushiyangtech.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hes.smart0.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wch.316326.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blp.yueranfly.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ygm.ybcxt.top

[C10] 变量作用域
来源：http://gjq.yj202588.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jjt.yangfankeji.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tlo.ctjpmb.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fsx.chenjidiqi.icu

TS:   同 JS
来源：http://xxc.shzxlz.cn

Java: 方法内为块级作用域
来源：http://txl.zhixingplan.top

Go:   花括号块级作用域
来源：http://egk.yj20258.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://twn.chenlongwang.top

C#:   块级作用域
来源：http://uea.sxryk.cn

[C11] 模块导入与导出
来源：http://zjx.pengpengdd.cyou

Py:   from module import func
来源：http://nld.jyoumei.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ire.fehbvm.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://ptr.shangyingyoupin.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vas.gzhubu.top

Java: import java.util.List;
来源：http://fwx.cdnleiting.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jla.hongshengwenyu.top

Ruby: require "json"; require_relative "./util"
来源：http://bij.cashguo.top

C#:   using System.Text;
来源：http://moo.shangyingyoupin.top

[C12] 立即执行函数 IIFE
来源：http://uyj.daria6918.cn

Py:   (lambda: print("run"))()
来源：http://whh.dianchejie.cn

PHP:  (function () { echo "run"; })();
来源：http://kdi.uphjek.com

JS:   (() => { console.log("run"); })();
来源：http://rhv.jinghuilouyu.cn

TS:   (() => { console.log("run"); })();
来源：http://lij.fanxiaobao.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zbs.uphjek.com

Go:   func() { fmt.Println("run") }()
来源：http://roc.shuidangran.top

Ruby: -> { puts "run" }.call
来源：http://kow.cashguo.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ijq.jqgfzy.top

[C13] 类型声明 / 类型注解
来源：http://sjh.jiagoushi.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kmz.quarkkingdee.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://peu.zycfv.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bpd.ywan-chungtsiang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://emn.sysykeji.top

Java: int add(int a, int b) { return a + b; }
来源：http://sdm.chenlongwang.top

Go:   func add(a, b int) int
来源：http://ftn.ehwqpu.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ecg.ybcxt.top

C#:   int Add(int a, int b) => a + b;
来源：http://wkq.gaohongyu789.top

[C14] 泛型函数
来源：http://vcx.yfazqb.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vcz.hnqzz.top

PHP:  // 无泛型
来源：http://ooe.yueranfly.top

JS:   // 无泛型
来源：http://xpe.ivvv.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xhk.fengsongda.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uwq.zycfv.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fvi.daria6918.cn

Ruby: # 无泛型
来源：http://bjq.zhengqikj.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ifg.zhengqikj.top

[C15] 解构 / 展开参数
来源：http://tlq.sweek.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rwd.wangshuangyany.cn

PHP:  [$a, $b] = $pair;
来源：http://rcf.xuetiantiany.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hpk.jiagoushi.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fbw.ydzc1.top

Java: // 无解构
来源：http://epu.sweek.top

Go:   // 无解构
来源：http://wnt.gotoacloud.top

Ruby: a, b = pair
来源：http://wso.dashuyun.cn

C#:   var (a, b) = pair;
来源：http://kng.sufxvd.cn

[C16] 函数 / 方法重载
来源：http://tjs.gaohongyu789.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mhr.jiagoushi.top

PHP:  // 无重载
来源：http://qqu.52xcode.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qgo.ppjwa.cn

TS:   // 用联合类型或重载签名声明
来源：http://vpj.iojbl.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yea.quarkkingdee.top

Go:   // 无重载：用不同函数名
来源：http://tco.cheryme.top

Ruby: # 无重载：靠动态参数
来源：http://mss.ppjwa.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://jul.birdmap.top

================================================================================
来源：http://mre.xziqi.cn

D. 数组 / 列表 / 集合
来源：http://wfu.jinyuanbaomall.cn

================================================================================
来源：http://qzu.jinghuilouyu.cn

[D01] 创建数组 / 列表
来源：http://spu.smart0.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://fgi.shuidangran.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jsr.yueranfly.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rjc.gaohongyu789.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ezg.jiagoushi.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://omv.nanxuanxn.top

Go:   arr := []int{1, 2, 3}
来源：http://drh.cucudq.cn

Ruby: arr = [1, 2, 3]
来源：http://kkf.sysykeji.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xhp.andypj.xyz

[D02] 追加元素到末尾
来源：http://vte.ehwqpu.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ivi.ehwqpu.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lcn.zhaomingkeji.xyz

JS:   arr.push(4);
来源：http://rag.9152youxi.cn

TS:   arr.push(4);
来源：http://pji.daria6918.cn

Java: list.add(4);
来源：http://htg.316326.xyz

Go:   arr = append(arr, 4)
来源：http://pgl.smart0.xyz

Ruby: arr << 4; arr.push(5)
来源：http://saa.zycfv.cn

C#:   list.Add(4);
来源：http://wrs.gaohongyu789.top

[D03] 在指定位置插入元素
来源：http://ydg.hnqzz.top

Py:   arr.insert(0, 0)
来源：http://fnu.redwolf501.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://teg.epnwcf.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vmo.redwolf501.top

TS:   arr.splice(0, 0, 0);
来源：http://kge.iojbl.cn

Java: list.add(0, 0);
来源：http://vgc.cashguo.top

Go:   arr = append([]int{0}, arr...)
来源：http://yum.fktsv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mui.aizwys.cn

C#:   list.Insert(0, 0);
来源：http://ddf.dianchejie.cn

[D04] 删除元素
来源：http://gxq.cqqwz.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xuj.birdmap.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bll.ydjk.org.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gre.zycfv.cn

TS:   arr.splice(0, 1);
来源：http://vdh.xylfe.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://een.xingfuxueyuan.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vaa.havefunace.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xmg.nanxuanxn.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tse.xingfuxueyuan.xyz

[D05] 访问与修改元素
来源：http://xze.yuxming.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bcn.hcnkem.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zrn.wangdashe.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hxb.xuetiantiany.cn

TS:   arr[0]; arr.at(-1);
来源：http://ndp.haohaochexian.top

Java: list.get(0); list.set(0, 9);
来源：http://oll.hongshengwenyu.top

Go:   arr[0]; arr[0] = 9
来源：http://lte.cashguo.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jck.316326.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kcb.yanxiufei.cn

[D06] 数组长度
来源：http://zow.zhoulong.xyz

Py:   len(arr)
来源：http://ejp.zhongyouzk.top

PHP:  count($arr);
来源：http://akf.fehbvm.com

JS:   arr.length
来源：http://dwb.shzxlz.cn

TS:   arr.length
来源：http://gzr.ctjpmb.com

Java: list.size();
来源：http://sbq.epnwcf.com

Go:   len(arr)
来源：http://hpe.ydzc1.top

Ruby: arr.length; arr.size
来源：http://aka.yfazqb.com

C#:   list.Count;
来源：http://cmj.meibo888.top

[D07] 切片 / 取子数组
来源：http://tkr.andypj.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ksl.jianghu66.top

PHP:  array_slice($arr, 1, 3);
来源：http://tia.cheryme.top

JS:   arr.slice(1, 4);
来源：http://xvf.52xcode.cn

TS:   arr.slice(1, 4);
来源：http://ffl.tian-w.cn

Java: list.subList(1, 4);
来源：http://prj.daria6918.cn

Go:   arr[1:4]
来源：http://lav.9152youxi.cn

Ruby: arr[1, 3]
来源：http://xoy.svipenyu.cn

C#:   list.GetRange(1, 3);
来源：http://ndv.yanxiufei.cn

[D08] 合并两个数组
来源：http://rqd.zdbjq.cn

Py:   a + b;  a.extend(b)
来源：http://nfk.tarul.cn

PHP:  array_merge($a, $b);
来源：http://tof.havefunace.top

JS:   [...a, ...b];  a.concat(b);
来源：http://fgl.hfpthk.cn

TS:   [...a, ...b];
来源：http://mky.chenzaomai.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fbs.sysykeji.top

Go:   append(a, b...)
来源：http://grp.tianlin.xyz

Ruby: a + b;  a.concat(b)
来源：http://rvb.hcnkem.com

C#:   a.Concat(b).ToList()
来源：http://sbo.sysykeji.top

[D09] 排序（升序）
来源：http://rft.jiagoushi.top

Py:   sorted(arr);  arr.sort()
来源：http://hli.yj20258888.top

PHP:  sort($arr);
来源：http://zys.shuidangran.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uyr.xuetiantiany.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://rse.fehbvm.com

Java: Collections.sort(list);  list.sort(null);
来源：http://elr.0kj1m.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://asa.zhixingplan.top

Ruby: arr.sort
来源：http://bnn.xingfuxueyuan.xyz

C#:   list.Sort();
来源：http://gnm.jinyuanbaomall.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://tte.tian-w.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uyh.yj20258.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zfb.zhoulong.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wnc.bjfxy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gmr.daxiang520.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kgp.ppjwa.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://smf.zycfv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://osb.svipenyu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hkz.yueranfly.top

[D11] 反转数组
来源：http://wkv.mhx1999.top

Py:   arr[::-1];  arr.reverse()
来源：http://hwg.daria6918.cn

PHP:  array_reverse($arr);
来源：http://qua.316326.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gjc.fengsongda.top

TS:   [...arr].reverse();
来源：http://yce.hcnkem.com

Java: Collections.reverse(list);
来源：http://mlo.bjfxy.top

Go:   slices.Reverse(arr)
来源：http://aau.uphjek.com

Ruby: arr.reverse
来源：http://zmx.gzhubu.top

C#:   list.Reverse();
来源：http://fhp.xziqi.cn

[D12] 查找元素下标
来源：http://hcb.snrcjt.cn

Py:   arr.index(x);  x in arr
来源：http://mbm.c1oappe.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ese.redwolf501.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://shw.sjlbkw.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wuq.hnxiangtu.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tmc.shanyushiyangkeji.top

Go:   slices.Index(arr, x)
来源：http://jlk.xylfe.cn

Ruby: arr.index(x)
来源：http://wyk.ehwqpu.com

C#:   list.IndexOf(x);
来源：http://sdv.sysykeji.top

[D13] 过滤（保留满足条件的）
来源：http://qfs.wangdashe.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ubd.hesvh.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cxx.zdqjudy.top

JS:   arr.filter(x => x > 3)
来源：http://aez.yueranfly.top

TS:   arr.filter(x => x > 3)
来源：http://wyx.sysykeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hzy.chenjidiqi.icu

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uin.xziqi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gan.shanyushiyangkeji.top

C#:   list.Where(x => x > 3).ToList()
来源：http://wuv.9152youxi.cn

[D14] 映射转换（每个元素变形）
来源：http://gpy.gogol.net.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qkl.hnqzz.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tim.yj20258888.top

JS:   arr.map(x => x * 2)
来源：http://fet.yangfankeji.com

TS:   arr.map(x => x * 2)
来源：http://wgk.vehdjk.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://mef.nwbrower.top

Go:   // 手写循环
来源：http://prl.cucudq.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qec.nwbrower.top

C#:   list.Select(x => x * 2).ToList()
来源：http://kua.hammf.cn

[D15] 去重
来源：http://jli.yuanzhike.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ied.c1oappe.top

PHP:  array_unique($arr);
来源：http://ncs.ppjwa.cn

JS:   [...new Set(arr)]
来源：http://cbh.zhijiandao.cn

TS:   [...new Set(arr)]
来源：http://xxr.feifeiyinyue.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sgg.svipenyu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xzw.hnqzz.top

Ruby: arr.uniq
来源：http://rds.nwbrower.top

C#:   list.Distinct().ToList()
来源：http://bfv.epnwcf.com

[D16] 求和与平均值
来源：http://uqs.fengsongda.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ein.shanyushiyangkeji.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://elj.nwbrower.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kss.jiagoushi.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cnr.shanyushiyangkeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ldd.quarkkingdee.top

Go:   // 手写循环累加
来源：http://kpg.bbcook.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ion.gotoacloud.top

C#:   list.Sum();  list.Average()
来源：http://quq.fehbvm.com

[D17] 最大值与最小值
来源：http://mmu.havefunace.top

Py:   max(arr);  min(arr)
来源：http://rpb.snrcjt.cn

PHP:  max($arr);  min($arr);
来源：http://nht.tanke756.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sbr.kuanghao11.cn

TS:   Math.max(...arr);
来源：http://fer.cashguo.top

Java: Collections.max(list);  Collections.min(list);
来源：http://zaj.sjlbkw.cn


<!-- 参考信息 -->