代发 wailian999

[C02] 默认参数
来源：http://bwg.shuidangran.top

Py:   def greet(name="World"): return name
来源：http://nau.meibo888.top

PHP:  function greet($name = "World") { return $name; }
来源：http://uam.bbcook.cn

JS:   function greet(name = "World") { return name; }
来源：http://ydz.jianghu66.top

TS:   function greet(name: string = "World") { return name; }
来源：http://qbm.yuanzhike.top

Java: // 无默认参数：方法重载或 Optional
来源：http://lxg.uphjek.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xse.shanyushiyangkeji.top

Ruby: def greet(name = "World") = name
来源：http://iwt.yuxming.cn

C#:   string Greet(string name = "World") => name;
来源：http://ozn.jqgufenzy.top

[C03] 可变参数
来源：http://gkb.iojbl.cn

Py:   def total(*args): return sum(args)
来源：http://hhb.daxiang520.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vzr.yongpay.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://csg.jyoumei.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tnz.dashuyun.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://iix.fzhhl.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dmb.svipenyu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://cbf.andypj.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://iqs.zhengqikj.top

[C04] 命名参数 / 关键字参数
来源：http://wmg.feifeiyinyue.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://srg.hongshengwenyu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://grv.chenlongwang.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hga.jinyuanbaomall.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zuz.chenlongwang.top

Java: // 无：用 Builder 模式或 record
来源：http://iqi.iojbl.cn

Go:   // 无：用配置结构体参数
来源：http://yli.xuanzx.com

Ruby: f(a: 1, b: 2)
来源：http://etd.mhx1999.top

C#:   f(a: 1, b: 2)
来源：http://jvv.yj20258.top

[C05] 返回多个值
来源：http://veb.yj202588.top

Py:   return a, b
来源：http://zfy.guannengcc.top

PHP:  return [$a, $b];
来源：http://hgu.zhaomingkeji.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://qbi.daria6918.cn

TS:   return { a, b };
来源：http://qsm.gzhubu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dzj.pycfn.com

Go:   return a, b
来源：http://qpd.zhoulong.xyz

Ruby: return a, b
来源：http://icj.jinghuilouyu.cn

C#:   return (a, b);              // ValueTuple
来源：http://wis.meibo888.top

[C06] 匿名函数 / lambda
来源：http://qrz.cdnleiting.top

Py:   square = lambda x: x * x
来源：http://qzy.jianghu66.top

PHP:  $square = fn($x) => $x * $x;
来源：http://tkv.yongpay.top

JS:   const square = x => x * x;
来源：http://vft.jianghu66.top

TS:   const square = (x: number): number => x * x;
来源：http://uob.dianchejie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vvm.yj20258.top

Go:   sq := func(x int) int { return x * x }
来源：http://tmc.c1oappe.top

Ruby: square = ->(x) { x * x }
来源：http://vft.9152youxi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cep.zhixingplan.top

[C07] 把函数作为参数传入
来源：http://urz.yueranfly.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qdu.nwbrower.top

PHP:  array_map("strtoupper", $arr);
来源：http://bjo.zhijiandao.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pkm.xingfuxueyuan.xyz

TS:   arr.map(String)
来源：http://ijs.redwolf501.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ahj.zycfv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lxf.aizwys.cn

Ruby: arr.map(&:upcase)
来源：http://qju.wangdashe.top

C#:   arr.Select(s => s.ToUpper())
来源：http://pjx.hesvh.cn

[C08] 闭包
来源：http://vzq.sjlbkw.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fby.dianchejie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vze.xuanzx.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://iph.yfazqb.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://exu.sysykeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dzg.zhijiandao.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pib.cashguo.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://aje.ybcxt.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://law.cheryme.top

[C09] 递归
来源：http://hgk.mhx1999.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kqe.fengsongda.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ieo.tanke756.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nsa.daria6918.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gsi.chenlongwang.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://psd.zhaomingkeji.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zbr.shuidangran.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bhn.tian-w.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://clz.cdnleiting.top

[C10] 变量作用域
来源：http://cym.hnxiangtu.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://oxn.redwolf501.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wbt.fzhhl.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xfp.birdmap.top

TS:   同 JS
来源：http://lfj.hammf.cn

Java: 方法内为块级作用域
来源：http://dix.yangfankeji.com

Go:   花括号块级作用域
来源：http://wtf.ydzc1.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ysg.dashuyun.cn

C#:   块级作用域
来源：http://ngo.wangdashe.top

[C11] 模块导入与导出
来源：http://uww.yongpay.top

Py:   from module import func
来源：http://fkx.wangshuangyany.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://txe.cashguo.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://avo.chenlongwang.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vzg.dashuyun.cn

Java: import java.util.List;
来源：http://qxg.pengpengdd.cyou

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jsh.shuidangran.top

Ruby: require "json"; require_relative "./util"
来源：http://uxr.yuxming.cn

C#:   using System.Text;
来源：http://arp.fengsongda.top

[C12] 立即执行函数 IIFE
来源：http://dsn.shuidangran.top

Py:   (lambda: print("run"))()
来源：http://sbs.tian-w.cn

PHP:  (function () { echo "run"; })();
来源：http://ngw.tanke756.top

JS:   (() => { console.log("run"); })();
来源：http://mvz.aibaodan.cn

TS:   (() => { console.log("run"); })();
来源：http://bhk.iojbl.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jpo.sxryk.cn

Go:   func() { fmt.Println("run") }()
来源：http://nhr.fzhhl.top

Ruby: -> { puts "run" }.call
来源：http://win.andypj.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://nex.nwbrower.top

[C13] 类型声明 / 类型注解
来源：http://tpw.zdbjq.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pqu.c1oappe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://taa.dianchejie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dhe.zhongyouzk.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://phv.hywenlv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://oaz.haohaochexian.top

Go:   func add(a, b int) int
来源：http://pwh.daria6918.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://czf.shuidangran.top

C#:   int Add(int a, int b) => a + b;
来源：http://yqt.svipenyu.cn

[C14] 泛型函数
来源：http://lby.yonumen.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://utm.cashguo.top

PHP:  // 无泛型
来源：http://wzn.zhoulong.xyz

JS:   // 无泛型
来源：http://che.yj202588.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gip.guowangkeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tnu.jinghuilouyu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://uiz.yangfankeji.com

Ruby: # 无泛型
来源：http://emc.yj20258888.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nfp.shuidangran.top

[C15] 解构 / 展开参数
来源：http://wei.jyoumei.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wye.vehdjk.com

PHP:  [$a, $b] = $pair;
来源：http://tef.wangshuangyany.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://aes.vehdjk.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mil.jinghuilouyu.cn

Java: // 无解构
来源：http://xpe.0kj1m.cn

Go:   // 无解构
来源：http://rof.quarkkingdee.top

Ruby: a, b = pair
来源：http://iec.ivvv.top

C#:   var (a, b) = pair;
来源：http://igt.yuanzhike.top

[C16] 函数 / 方法重载
来源：http://wjl.wangshuangyany.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rcs.fzhhl.top

PHP:  // 无重载
来源：http://haq.ivvv.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ips.guannengcc.top

TS:   // 用联合类型或重载签名声明
来源：http://ste.zhengqikj.top

Java: void f(int a) {}  void f(String a) {}
来源：http://egp.shzxlz.cn

Go:   // 无重载：用不同函数名
来源：http://jbv.shanyushiyangtech.top

Ruby: # 无重载：靠动态参数
来源：http://wxc.zhoulong.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://vwb.jlsjyb.cn

================================================================================
来源：http://iso.ydzc1.top

D. 数组 / 列表 / 集合
来源：http://bcx.daxiang520.top

================================================================================
来源：http://ddx.jlsjyb.cn

[D01] 创建数组 / 列表
来源：http://yis.hywenlv.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://sea.wangdashe.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fwy.gotoacloud.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sqz.zdbjq.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://uma.dashuyun.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uzq.sysykeji.top

Go:   arr := []int{1, 2, 3}
来源：http://lan.guannengcc.top

Ruby: arr = [1, 2, 3]
来源：http://zja.ivvv.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://iht.tian-w.cn

[D02] 追加元素到末尾
来源：http://suh.ybcxt.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yxl.jlsjyb.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://smg.hesvh.cn

JS:   arr.push(4);
来源：http://fha.ehwqpu.com

TS:   arr.push(4);
来源：http://kqc.zhiwuduotai.top

Java: list.add(4);
来源：http://lyf.gotoacloud.top

Go:   arr = append(arr, 4)
来源：http://vzh.zhongyouzk.top

Ruby: arr << 4; arr.push(5)
来源：http://ste.fzhhl.top

C#:   list.Add(4);
来源：http://fla.nwbrower.top

[D03] 在指定位置插入元素
来源：http://vfj.redwolf501.top

Py:   arr.insert(0, 0)
来源：http://tzw.pycfn.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dsp.guannengcc.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mfp.ivvv.top

TS:   arr.splice(0, 0, 0);
来源：http://qbf.hnqzz.top

Java: list.add(0, 0);
来源：http://otr.nanxuanxn.top

Go:   arr = append([]int{0}, arr...)
来源：http://ewr.hammf.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pmv.shzxlz.cn

C#:   list.Insert(0, 0);
来源：http://jwp.hcnkem.com

[D04] 删除元素
来源：http://njv.jinqigufen.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ywk.haohaochexian.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://caw.ybcxt.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zya.cdnleiting.top

TS:   arr.splice(0, 1);
来源：http://djl.jinghuilouyu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xti.pengpengdd.cyou

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://opd.fktsv.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://isf.aibaodan.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ljt.gogol.net.cn

[D05] 访问与修改元素
来源：http://bzc.zycfv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ndc.guannengcc.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://csb.andypj.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wis.guowangkeji.top

TS:   arr[0]; arr.at(-1);
来源：http://gsc.jyoumei.cn

Java: list.get(0); list.set(0, 9);
来源：http://rha.gotoacloud.top

Go:   arr[0]; arr[0] = 9
来源：http://acn.cdnleiting.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hcb.wangdashe.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zya.snrcjt.cn

[D06] 数组长度
来源：http://kol.xingfuxueyuan.xyz

Py:   len(arr)
来源：http://xim.yonumen.top

PHP:  count($arr);
来源：http://zox.yongpay.top

JS:   arr.length
来源：http://umt.havefunace.top

TS:   arr.length
来源：http://gfh.aizwys.cn

Java: list.size();
来源：http://wah.nwbrower.top

Go:   len(arr)
来源：http://kfc.daria6918.cn

Ruby: arr.length; arr.size
来源：http://vnu.sweek.top

C#:   list.Count;
来源：http://pyx.wangdashe.top

[D07] 切片 / 取子数组
来源：http://lqn.nwbrower.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ctw.yongpay.top

PHP:  array_slice($arr, 1, 3);
来源：http://wtu.xingfuxueyuan.xyz

JS:   arr.slice(1, 4);
来源：http://rlq.gaohongyu789.top

TS:   arr.slice(1, 4);
来源：http://gur.zhongyouzk.top

Java: list.subList(1, 4);
来源：http://jzi.tarul.cn

Go:   arr[1:4]
来源：http://bhj.zdbjq.cn

Ruby: arr[1, 3]
来源：http://aje.fktsv.cn

C#:   list.GetRange(1, 3);
来源：http://wbf.jinghuilouyu.cn

[D08] 合并两个数组
来源：http://irk.sweek.top

Py:   a + b;  a.extend(b)
来源：http://jgt.gzhubu.top

PHP:  array_merge($a, $b);
来源：http://eja.cashguo.top

JS:   [...a, ...b];  a.concat(b);
来源：http://vwq.yuxming.cn

TS:   [...a, ...b];
来源：http://knw.ydzc1.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xjq.hysaishi.cn

Go:   append(a, b...)
来源：http://wdx.fehbvm.com

Ruby: a + b;  a.concat(b)
来源：http://cff.gaohongyu789.top

C#:   a.Concat(b).ToList()
来源：http://lcv.guannengcc.top

[D09] 排序（升序）
来源：http://zcd.cqqwz.cn

Py:   sorted(arr);  arr.sort()
来源：http://psa.yj20258.top

PHP:  sort($arr);
来源：http://yzj.0kj1m.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tfa.zdqjudy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://qwq.9152youxi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://pwk.hammf.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fty.nanxuanxn.top

Ruby: arr.sort
来源：http://ahy.zhijiandao.cn

C#:   list.Sort();
来源：http://glw.ydzc1.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://gnz.xylfe.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kfb.jqgufenzy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kmt.ivvv.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mjn.cqqwz.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ese.meibo888.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yfj.chenlongwang.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gox.yfazqb.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rxo.tarul.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vyf.jqgufenzy.top

[D11] 反转数组
来源：http://jsl.nanxinkj.top

Py:   arr[::-1];  arr.reverse()
来源：http://mce.shuidangran.top

PHP:  array_reverse($arr);
来源：http://esp.quarkkingdee.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tat.meibo888.top

TS:   [...arr].reverse();
来源：http://etb.bbcook.cn

Java: Collections.reverse(list);
来源：http://mda.yj202588.top

Go:   slices.Reverse(arr)
来源：http://zio.uphjek.com

Ruby: arr.reverse
来源：http://rto.cucudq.cn

C#:   list.Reverse();
来源：http://fwf.dashuyun.cn

[D12] 查找元素下标
来源：http://txw.jianghu66.top

Py:   arr.index(x);  x in arr
来源：http://bpb.bjfxy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vae.yuanzhike.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hno.yuanzhike.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ext.0kj1m.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://piq.jinghuilouyu.cn

Go:   slices.Index(arr, x)
来源：http://mcj.guowangkeji.top

Ruby: arr.index(x)
来源：http://yez.kuanghao11.cn

C#:   list.IndexOf(x);
来源：http://xjl.yfazqb.com

[D13] 过滤（保留满足条件的）
来源：http://bjr.yuanzhike.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rht.shzxlz.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://oeh.svipenyu.cn

JS:   arr.filter(x => x > 3)
来源：http://jsh.xuanzx.com

TS:   arr.filter(x => x > 3)
来源：http://rdl.zhixingplan.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xmr.cqqwz.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lns.aibaodan.cn

Ruby: arr.select { |x| x > 3 }
来源：http://odg.redwolf501.top

C#:   list.Where(x => x > 3).ToList()
来源：http://uuz.zhaomingkeji.xyz

[D14] 映射转换（每个元素变形）
来源：http://yhj.smart0.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bzx.daxiang520.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qnb.pycfn.com

JS:   arr.map(x => x * 2)
来源：http://xxk.tanke756.top

TS:   arr.map(x => x * 2)
来源：http://zta.ybcxt.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://hoe.gogol.net.cn

Go:   // 手写循环
来源：http://mqv.shzxlz.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qyt.smart0.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://ovx.jinqigufen.top

[D15] 去重
来源：http://puo.chenjidiqi.icu

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fmv.cqqwz.cn

PHP:  array_unique($arr);
来源：http://ofi.sweek.top

JS:   [...new Set(arr)]
来源：http://vlr.aibaodan.cn

TS:   [...new Set(arr)]
来源：http://ydp.cqqwz.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lzn.tian-w.cn

Go:   // 用 map[T]struct{} 手写
来源：http://rvh.yongpay.top

Ruby: arr.uniq
来源：http://ynw.xinyue.icu

C#:   list.Distinct().ToList()
来源：http://anq.yueranfly.top

[D16] 求和与平均值
来源：http://mtl.yanxiufei.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nyg.yuanzhike.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xgp.yfazqb.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://liv.birdmap.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wpb.wangdashe.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mdt.zhijiandao.cn

Go:   // 手写循环累加
来源：http://utl.yj20258888.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yjg.guowangkeji.top

C#:   list.Sum();  list.Average()
来源：http://wxn.ivvv.top

[D17] 最大值与最小值
来源：http://hwv.yangfankeji.com

Py:   max(arr);  min(arr)
来源：http://ovh.jqgfzy.top

PHP:  max($arr);  min($arr);
来源：http://ldu.bbcook.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vfm.shanyushiyangtech.top

TS:   Math.max(...arr);
来源：http://tnn.bbcook.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://uhs.haohaochexian.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ugo.nanxinkj.top

Ruby: arr.max;  arr.min
来源：http://zmy.nanxinkj.top

C#:   list.Max();  list.Min()
来源：http://txc.jqgfzy.top

[D18] 扁平化嵌套数组
来源：http://fyr.nwbrower.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pfv.zhaomingkeji.xyz

PHP:  array_merge(...$nested);
来源：http://isd.wangshuangyany.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://exx.gaohongyu789.top

TS:   nested.flat();
来源：http://xtr.hammf.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kck.meibo888.top

Go:   // 手写双层循环
来源：http://rvh.zhiwuduotai.top

Ruby: nested.flatten
来源：http://yty.sufxvd.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://mtg.sysykeji.top


<!-- 参考信息 -->