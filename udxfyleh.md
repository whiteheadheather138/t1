代发 wailian999

Go:   a && b || !c
来源：http://cbg.yvedp.cn

Ruby: a && b || !c
来源：http://clc.jinqigufen.top

C#:   a && b || !c
来源：http://hms.kuanghao11.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ygr.feifeiyinyue.top

Py:   if not data: return
来源：http://eht.xylfe.cn

PHP:  if (!$data) { return; }
来源：http://pgq.chenjidiqi.icu

JS:   if (!data) return;
来源：http://nrx.yongpay.top

TS:   if (!data) return;
来源：http://qxu.yvedp.cn

Java: if (data == null) return;
来源：http://jdn.vehdjk.com

Go:   if data == nil { return }
来源：http://cse.dianchejie.cn

Ruby: return if data.nil?
来源：http://csf.svipenyu.cn

C#:   if (data == null) return;
来源：http://mft.ctjpmb.com

================================================================================
来源：http://boi.ydjk.org.cn

C. 函数与作用域
来源：http://zdq.yj202588.top

================================================================================
来源：http://dht.jqgfzy.top

[C01] 定义函数
来源：http://wcq.cheryme.top

Py:   def add(a, b): return a + b
来源：http://upi.ehwqpu.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zko.c1oappe.top

JS:   function add(a, b) { return a + b; }
来源：http://ccc.daxiang520.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nem.feifeiyinyue.top

Java: static int add(int a, int b) { return a + b; }
来源：http://xdb.shzxlz.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rrl.shuidangran.top

Ruby: def add(a, b); a + b; end
来源：http://ngr.meibo888.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ael.sweek.top

[C02] 默认参数
来源：http://rnb.hongshengwenyu.top

Py:   def greet(name="World"): return name
来源：http://fwt.yongpay.top

PHP:  function greet($name = "World") { return $name; }
来源：http://svw.meibo888.top

JS:   function greet(name = "World") { return name; }
来源：http://qwd.wangdashe.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ycf.ppjwa.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://gyk.c1oappe.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xdz.mhx1999.top

Ruby: def greet(name = "World") = name
来源：http://zak.dianchejie.cn

C#:   string Greet(string name = "World") => name;
来源：http://jev.hysaishi.cn

[C03] 可变参数
来源：http://ycv.wangshuangyany.cn

Py:   def total(*args): return sum(args)
来源：http://ags.zhongyouzk.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nsu.xuanzx.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jkg.snrcjt.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vqq.316326.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wun.cqqwz.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yzc.xylfe.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ztz.iojbl.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://apv.pycfn.com

[C04] 命名参数 / 关键字参数
来源：http://pti.snrcjt.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lez.yuxming.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fdw.smart0.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rzy.iojbl.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cqj.xuetiantiany.cn

Java: // 无：用 Builder 模式或 record
来源：http://loo.zdqjudy.top

Go:   // 无：用配置结构体参数
来源：http://uyw.fktsv.cn

Ruby: f(a: 1, b: 2)
来源：http://xmu.gaohongyu789.top

C#:   f(a: 1, b: 2)
来源：http://bse.xuanzx.com

[C05] 返回多个值
来源：http://xjp.ydjk.org.cn

Py:   return a, b
来源：http://ucv.svipenyu.cn

PHP:  return [$a, $b];
来源：http://cbv.jinyuanbaomall.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://eeb.dashuyun.cn

TS:   return { a, b };
来源：http://hfl.ehwqpu.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mov.shuidangran.top

Go:   return a, b
来源：http://taz.nwbrower.top

Ruby: return a, b
来源：http://tcz.jiagoushi.top

C#:   return (a, b);              // ValueTuple
来源：http://dgu.ywan-chungtsiang.top

[C06] 匿名函数 / lambda
来源：http://iok.hongshengwenyu.top

Py:   square = lambda x: x * x
来源：http://zns.pengpengdd.cyou

PHP:  $square = fn($x) => $x * $x;
来源：http://dil.hcnkem.com

JS:   const square = x => x * x;
来源：http://dxp.jlsjyb.cn

TS:   const square = (x: number): number => x * x;
来源：http://xsw.316326.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cub.tian-w.cn

Go:   sq := func(x int) int { return x * x }
来源：http://yiu.gzhubu.top

Ruby: square = ->(x) { x * x }
来源：http://gky.gaohongyu789.top

C#:   Func<int, int> square = x => x * x;
来源：http://vrw.yangfankeji.com

[C07] 把函数作为参数传入
来源：http://hxq.haohaochexian.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dpr.yueranfly.top

PHP:  array_map("strtoupper", $arr);
来源：http://jiv.bjfxy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mir.wangshuangyany.cn

TS:   arr.map(String)
来源：http://sbq.mhx1999.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://iul.cheryme.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://svv.zhoulong.xyz

Ruby: arr.map(&:upcase)
来源：http://djm.yanxiufei.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://vfl.haohaochexian.top

[C08] 闭包
来源：http://ysx.hongshengwenyu.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vga.sysykeji.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rbk.sufxvd.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vhh.jiagoushi.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wzf.ctjpmb.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://byc.nwbrower.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://esg.iojbl.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nrc.cucudq.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://btd.cashguo.top

[C09] 递归
来源：http://jgs.fehbvm.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xlq.daxiang520.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bgr.snrcjt.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fhd.xingfuxueyuan.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rhs.aizwys.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kfc.sufxvd.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ayn.pengpengdd.cyou

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rbm.shuidangran.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pxw.hcnkem.com

[C10] 变量作用域
来源：http://zuf.tarul.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ucz.ybcxt.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://irg.cucudq.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sab.zdqjudy.top

TS:   同 JS
来源：http://tnq.xuetiantiany.cn

Java: 方法内为块级作用域
来源：http://zqm.fengsongda.top

Go:   花括号块级作用域
来源：http://zas.ydzc1.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://liy.hesvh.cn

C#:   块级作用域
来源：http://hyh.hcnkem.com

[C11] 模块导入与导出
来源：http://hps.gotoacloud.top

Py:   from module import func
来源：http://vzd.dianchejie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://jne.9152youxi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pvs.zhengqikj.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jsc.xziqi.cn

Java: import java.util.List;
来源：http://wys.hongshengwenyu.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ncj.hesvh.cn

Ruby: require "json"; require_relative "./util"
来源：http://owx.hammf.cn

C#:   using System.Text;
来源：http://pfj.redwolf501.top

[C12] 立即执行函数 IIFE
来源：http://hzg.c1oappe.top

Py:   (lambda: print("run"))()
来源：http://fig.ydjk.org.cn

PHP:  (function () { echo "run"; })();
来源：http://ojt.jiagoushi.top

JS:   (() => { console.log("run"); })();
来源：http://kju.ywan-chungtsiang.top

TS:   (() => { console.log("run"); })();
来源：http://aej.gaohongyu789.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cif.316326.xyz

Go:   func() { fmt.Println("run") }()
来源：http://ewu.kuanghao11.cn

Ruby: -> { puts "run" }.call
来源：http://iqs.sweek.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ita.yj20258.top

[C13] 类型声明 / 类型注解
来源：http://jsz.fehbvm.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://unt.yj202588.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://myu.sufxvd.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rlu.hesvh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vuk.fehbvm.com

Java: int add(int a, int b) { return a + b; }
来源：http://byo.yangfankeji.com

Go:   func add(a, b int) int
来源：http://ljx.snrcjt.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ypa.meibo888.top

C#:   int Add(int a, int b) => a + b;
来源：http://goh.yanxiufei.cn

[C14] 泛型函数
来源：http://dkp.aizwys.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ucz.xuanzx.com

PHP:  // 无泛型
来源：http://xqi.guannengcc.top

JS:   // 无泛型
来源：http://jiv.316326.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nbt.cucudq.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qnu.guannengcc.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lzi.vqdsnc.cn

Ruby: # 无泛型
来源：http://nmu.snrcjt.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bpw.cashguo.top

[C15] 解构 / 展开参数
来源：http://hgl.jyoumei.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yac.fktsv.cn

PHP:  [$a, $b] = $pair;
来源：http://liw.sjlbkw.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://phq.sjlbkw.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ced.yanxiufei.cn

Java: // 无解构
来源：http://xmk.yueranfly.top

Go:   // 无解构
来源：http://zah.andypj.xyz

Ruby: a, b = pair
来源：http://yqn.nanxuanxn.top

C#:   var (a, b) = pair;
来源：http://gjh.pycfn.com

[C16] 函数 / 方法重载
来源：http://vbe.sjlbkw.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://skr.yueranfly.top

PHP:  // 无重载
来源：http://uli.iojbl.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ima.sjlbkw.cn

TS:   // 用联合类型或重载签名声明
来源：http://dry.dianchejie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rww.xingfuxueyuan.xyz

Go:   // 无重载：用不同函数名
来源：http://mrt.shzxlz.cn

Ruby: # 无重载：靠动态参数
来源：http://uzr.xylfe.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ycc.snrcjt.cn

================================================================================
来源：http://amb.xuetiantiany.cn

D. 数组 / 列表 / 集合
来源：http://ijq.zdqjudy.top

================================================================================
来源：http://woi.ctjpmb.com

[D01] 创建数组 / 列表
来源：http://heo.zhengqikj.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://jps.chenjidiqi.icu

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cou.bbcook.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mob.epnwcf.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://esq.ppjwa.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qrq.epnwcf.com

Go:   arr := []int{1, 2, 3}
来源：http://ins.sysykeji.top

Ruby: arr = [1, 2, 3]
来源：http://rtp.jlsjyb.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kzv.bbcook.cn

[D02] 追加元素到末尾
来源：http://pdk.nwbrower.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cpp.gaohongyu789.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zlc.daria6918.cn

JS:   arr.push(4);
来源：http://ftx.yj20258.top

TS:   arr.push(4);
来源：http://sqb.cashguo.top

Java: list.add(4);
来源：http://nyh.hnxiangtu.top

Go:   arr = append(arr, 4)
来源：http://mew.wangdashe.top

Ruby: arr << 4; arr.push(5)
来源：http://kdv.quarkkingdee.top

C#:   list.Add(4);
来源：http://pes.sufxvd.cn

[D03] 在指定位置插入元素
来源：http://lin.aizwys.cn

Py:   arr.insert(0, 0)
来源：http://ewg.c1oappe.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://btz.jinyuanbaomall.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pao.meibo888.top

TS:   arr.splice(0, 0, 0);
来源：http://rhn.aibaodan.cn

Java: list.add(0, 0);
来源：http://sto.9152youxi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xkg.meibo888.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dco.sxryk.cn

C#:   list.Insert(0, 0);
来源：http://zjy.havefunace.top

[D04] 删除元素
来源：http://jvv.sweek.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gxk.zhengqikj.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vup.fehbvm.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yvu.ydzc1.top

TS:   arr.splice(0, 1);
来源：http://plj.wangdashe.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ncq.birdmap.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qcm.ivvv.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://eqy.yvedp.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hrb.c1oappe.top

[D05] 访问与修改元素
来源：http://iqk.chenzaomai.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dox.52xcode.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vwc.daxiang520.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://joy.nanxuanxn.top

TS:   arr[0]; arr.at(-1);
来源：http://hxd.9152youxi.cn

Java: list.get(0); list.set(0, 9);
来源：http://wof.tarul.cn

Go:   arr[0]; arr[0] = 9
来源：http://ebn.yfazqb.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vnz.epnwcf.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tio.wangdashe.top

[D06] 数组长度
来源：http://xow.yj202588.top

Py:   len(arr)
来源：http://rsb.jianghu66.top

PHP:  count($arr);
来源：http://wjt.yj20258888.top

JS:   arr.length
来源：http://igc.hfpthk.cn

TS:   arr.length
来源：http://rbm.shanyushiyangtech.top

Java: list.size();
来源：http://own.xylfe.cn

Go:   len(arr)
来源：http://ley.shzxlz.cn

Ruby: arr.length; arr.size
来源：http://yim.yj202588.top

C#:   list.Count;
来源：http://nkz.mhx1999.top

[D07] 切片 / 取子数组
来源：http://ozm.fzhhl.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nuf.xingfuxueyuan.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://dzd.kuanghao11.cn

JS:   arr.slice(1, 4);
来源：http://ejj.aibaodan.cn

TS:   arr.slice(1, 4);
来源：http://era.hcnkem.com

Java: list.subList(1, 4);
来源：http://cff.fktsv.cn

Go:   arr[1:4]
来源：http://gzo.ehwqpu.com

Ruby: arr[1, 3]
来源：http://ouw.52xcode.cn

C#:   list.GetRange(1, 3);
来源：http://imd.jinyuanbaomall.cn

[D08] 合并两个数组
来源：http://rzl.havefunace.top

Py:   a + b;  a.extend(b)
来源：http://ykk.nanxuanxn.top

PHP:  array_merge($a, $b);
来源：http://jux.hfpthk.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://osi.vqdsnc.cn

TS:   [...a, ...b];
来源：http://zhe.sweek.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wyv.zhaomingkeji.xyz

Go:   append(a, b...)
来源：http://sxo.mhx1999.top

Ruby: a + b;  a.concat(b)
来源：http://lym.yongpay.top

C#:   a.Concat(b).ToList()
来源：http://ekp.vqdsnc.cn

[D09] 排序（升序）
来源：http://jcq.fktsv.cn

Py:   sorted(arr);  arr.sort()
来源：http://dwb.zhiwuduotai.top

PHP:  sort($arr);
来源：http://snt.fehbvm.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://igp.zhengqikj.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://akq.sweek.top

Java: Collections.sort(list);  list.sort(null);
来源：http://jhn.tianlin.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nca.zycfv.cn

Ruby: arr.sort
来源：http://acx.sjlbkw.cn

C#:   list.Sort();
来源：http://iyy.cqqwz.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://jix.fehbvm.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mkv.yangfankeji.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://csj.xuanzx.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://snk.chenlongwang.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://epy.ydzc1.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gwl.fengsongda.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dnm.vqdsnc.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ufu.cheryme.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://smz.sxryk.cn

[D11] 反转数组
来源：http://jer.hesvh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://tyk.dashuyun.cn

PHP:  array_reverse($arr);
来源：http://eog.jyoumei.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ech.iojbl.cn

TS:   [...arr].reverse();
来源：http://yja.ppjwa.cn

Java: Collections.reverse(list);
来源：http://hlp.nwbrower.top

Go:   slices.Reverse(arr)
来源：http://bpj.jinqigufen.top

Ruby: arr.reverse
来源：http://iio.bjfxy.top

C#:   list.Reverse();
来源：http://hox.chenzaomai.com

[D12] 查找元素下标
来源：http://elf.cheryme.top

Py:   arr.index(x);  x in arr
来源：http://vmw.jiagoushi.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lky.shzxlz.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mca.zhixingplan.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fun.xinyue.icu

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qhi.sysykeji.top

Go:   slices.Index(arr, x)
来源：http://bck.yuxming.cn

Ruby: arr.index(x)
来源：http://ref.yanxiufei.cn

C#:   list.IndexOf(x);
来源：http://mcu.hfpthk.cn

[D13] 过滤（保留满足条件的）
来源：http://mef.gzhubu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fst.zdqjudy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://oxl.smart0.xyz

JS:   arr.filter(x => x > 3)
来源：http://nuo.jqgfzy.top

TS:   arr.filter(x => x > 3)
来源：http://sji.andypj.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ade.zdqjudy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ihg.xuanzx.com

Ruby: arr.select { |x| x > 3 }
来源：http://axo.hcnkem.com

C#:   list.Where(x => x > 3).ToList()
来源：http://zyo.hnxiangtu.top

[D14] 映射转换（每个元素变形）
来源：http://ryz.52xcode.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fal.jinyuanbaomall.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hda.tanke756.top

JS:   arr.map(x => x * 2)
来源：http://kuv.zhaomingkeji.xyz

TS:   arr.map(x => x * 2)
来源：http://tet.bjfxy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://aks.yuanzhike.top

Go:   // 手写循环
来源：http://laq.xziqi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://sxz.redwolf501.top

C#:   list.Select(x => x * 2).ToList()
来源：http://rkb.ydzc1.top

[D15] 去重
来源：http://rat.jqgfzy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nur.jinqigufen.top

PHP:  array_unique($arr);
来源：http://rur.pycfn.com

JS:   [...new Set(arr)]
来源：http://uvp.sweek.top

TS:   [...new Set(arr)]
来源：http://ego.ctjpmb.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qsk.birdmap.top

Go:   // 用 map[T]struct{} 手写
来源：http://obm.yj20258888.top

Ruby: arr.uniq
来源：http://exj.gogol.net.cn

C#:   list.Distinct().ToList()
来源：http://ngt.guowangkeji.top

[D16] 求和与平均值
来源：http://cfz.nwbrower.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rnm.tianlin.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gnz.yj20258.top


<!-- 参考信息 -->