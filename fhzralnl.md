代发 wailian999

Py:   def add(a, b): return a + b
来源：http://xiz.yueranfly.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vqh.sxryk.cn

JS:   function add(a, b) { return a + b; }
来源：http://jpz.chenjidiqi.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nuh.aibaodan.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://uii.yj20258888.top

Go:   func add(a, b int) int { return a + b }
来源：http://wxf.guowangkeji.top

Ruby: def add(a, b); a + b; end
来源：http://qlz.pengpengdd.cyou

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hnw.zhiwuduotai.top

[C02] 默认参数
来源：http://iup.nanxuanxn.top

Py:   def greet(name="World"): return name
来源：http://llm.shanyushiyangkeji.top

PHP:  function greet($name = "World") { return $name; }
来源：http://scc.jinyuanbaomall.cn

JS:   function greet(name = "World") { return name; }
来源：http://tfr.ehwqpu.com

TS:   function greet(name: string = "World") { return name; }
来源：http://iaf.svipenyu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ruq.andypj.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sqk.pengpengdd.cyou

Ruby: def greet(name = "World") = name
来源：http://gof.yj202588.top

C#:   string Greet(string name = "World") => name;
来源：http://pyv.jinyuanbaomall.cn

[C03] 可变参数
来源：http://tgi.nanxuanxn.top

Py:   def total(*args): return sum(args)
来源：http://zjw.shzxlz.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://huv.aizwys.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pnc.0kj1m.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zih.vqdsnc.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zco.uphjek.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gdt.wangshuangyany.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fwf.kuanghao11.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vvq.yj20258.top

[C04] 命名参数 / 关键字参数
来源：http://nqd.fanxiaobao.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rpv.redwolf501.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vxj.cdnleiting.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://los.pycfn.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ren.fzhhl.top

Java: // 无：用 Builder 模式或 record
来源：http://mqn.xingfuxueyuan.xyz

Go:   // 无：用配置结构体参数
来源：http://vpi.jyoumei.cn

Ruby: f(a: 1, b: 2)
来源：http://hxv.chenlongwang.top

C#:   f(a: 1, b: 2)
来源：http://ptp.nwbrower.top

[C05] 返回多个值
来源：http://ihw.haohaochexian.top

Py:   return a, b
来源：http://vyj.yj20258888.top

PHP:  return [$a, $b];
来源：http://fop.zycfv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jwh.yangfankeji.com

TS:   return { a, b };
来源：http://msq.yonumen.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gmy.vehdjk.com

Go:   return a, b
来源：http://hsq.daria6918.cn

Ruby: return a, b
来源：http://xmn.yfazqb.com

C#:   return (a, b);              // ValueTuple
来源：http://wiq.quarkkingdee.top

[C06] 匿名函数 / lambda
来源：http://mou.sufxvd.cn

Py:   square = lambda x: x * x
来源：http://tcw.sjlbkw.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://tsv.yanxiufei.cn

JS:   const square = x => x * x;
来源：http://bkb.zhaomingkeji.xyz

TS:   const square = (x: number): number => x * x;
来源：http://paz.nanxinkj.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://uji.316326.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://mqs.zdqjudy.top

Ruby: square = ->(x) { x * x }
来源：http://sql.kuanghao11.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xev.aizwys.cn

[C07] 把函数作为参数传入
来源：http://mhl.ybcxt.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://esi.fanxiaobao.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://pju.snrcjt.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rzi.iojbl.cn

TS:   arr.map(String)
来源：http://xup.zhiwuduotai.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cus.zdqjudy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rod.yj202588.top

Ruby: arr.map(&:upcase)
来源：http://hkx.birdmap.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ikp.xziqi.cn

[C08] 闭包
来源：http://upw.wangshuangyany.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vve.shanyushiyangtech.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://scn.hesvh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vmt.zhiwuduotai.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cqr.yvedp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bje.gaohongyu789.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dlh.9152youxi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://apv.jinyuanbaomall.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ava.cashguo.top

[C09] 递归
来源：http://akm.daxiang520.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jlo.xingfuxueyuan.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cls.dashuyun.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://reb.c1oappe.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xws.xingfuxueyuan.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://coi.sxryk.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mze.chenjidiqi.icu

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qqf.yj20258888.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lkf.tian-w.cn

[C10] 变量作用域
来源：http://inb.haohaochexian.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yib.cdnleiting.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rpe.nanxuanxn.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://net.vqdsnc.cn

TS:   同 JS
来源：http://die.xuanzx.com

Java: 方法内为块级作用域
来源：http://nou.ydjk.org.cn

Go:   花括号块级作用域
来源：http://fwx.ivvv.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mqz.ydjk.org.cn

C#:   块级作用域
来源：http://lst.smart0.xyz

[C11] 模块导入与导出
来源：http://zed.zhijiandao.cn

Py:   from module import func
来源：http://bdr.zhaomingkeji.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://wzx.chenzaomai.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://pzf.zdbjq.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://glq.tian-w.cn

Java: import java.util.List;
来源：http://pdd.shanyushiyangkeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wkn.zhaomingkeji.xyz

Ruby: require "json"; require_relative "./util"
来源：http://sil.sweek.top

C#:   using System.Text;
来源：http://kjx.meibo888.top

[C12] 立即执行函数 IIFE
来源：http://epz.uphjek.com

Py:   (lambda: print("run"))()
来源：http://hlg.gaohongyu789.top

PHP:  (function () { echo "run"; })();
来源：http://fcm.guowangkeji.top

JS:   (() => { console.log("run"); })();
来源：http://rue.cqqwz.cn

TS:   (() => { console.log("run"); })();
来源：http://urp.kuanghao11.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://voa.xingfuxueyuan.xyz

Go:   func() { fmt.Println("run") }()
来源：http://hqk.shangyingyoupin.top

Ruby: -> { puts "run" }.call
来源：http://vmz.aibaodan.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://oel.hnxiangtu.top

[C13] 类型声明 / 类型注解
来源：http://ahv.pycfn.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dhr.zdbjq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tmf.svipenyu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rex.tanke756.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gsn.yfazqb.com

Java: int add(int a, int b) { return a + b; }
来源：http://cjw.wangdashe.top

Go:   func add(a, b int) int
来源：http://eno.gzhubu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jhv.hammf.cn

C#:   int Add(int a, int b) => a + b;
来源：http://thr.hesvh.cn

[C14] 泛型函数
来源：http://dla.sweek.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xox.jinyuanbaomall.cn

PHP:  // 无泛型
来源：http://zzk.xylfe.cn

JS:   // 无泛型
来源：http://wxg.yuanzhike.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jhn.cheryme.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://evn.ivvv.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wav.mhx1999.top

Ruby: # 无泛型
来源：http://nuj.uphjek.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rfw.smart0.xyz

[C15] 解构 / 展开参数
来源：http://mjj.gogol.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://oih.ydzc1.top

PHP:  [$a, $b] = $pair;
来源：http://vxs.xuanzx.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lrz.zhoulong.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ohp.haohaochexian.top

Java: // 无解构
来源：http://jol.yj20258888.top

Go:   // 无解构
来源：http://rdw.gotoacloud.top

Ruby: a, b = pair
来源：http://qqg.tarul.cn

C#:   var (a, b) = pair;
来源：http://ooz.guowangkeji.top

[C16] 函数 / 方法重载
来源：http://lmw.jqgfzy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gup.quarkkingdee.top

PHP:  // 无重载
来源：http://sle.nanxuanxn.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://dvn.epnwcf.com

TS:   // 用联合类型或重载签名声明
来源：http://rte.jinqigufen.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ddb.jyoumei.cn

Go:   // 无重载：用不同函数名
来源：http://ppk.haohaochexian.top

Ruby: # 无重载：靠动态参数
来源：http://uue.zhoulong.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://dfs.jqgufenzy.top

================================================================================
来源：http://fkj.316326.xyz

D. 数组 / 列表 / 集合
来源：http://msl.ehwqpu.com

================================================================================
来源：http://rhe.ehwqpu.com

[D01] 创建数组 / 列表
来源：http://fkd.smart0.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://acg.aizwys.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://llu.daxiang520.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://etc.daxiang520.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://umh.jinyuanbaomall.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://spv.chenlongwang.top

Go:   arr := []int{1, 2, 3}
来源：http://xws.gzhubu.top

Ruby: arr = [1, 2, 3]
来源：http://can.jinyuanbaomall.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tcs.jqgfzy.top

[D02] 追加元素到末尾
来源：http://jnt.snrcjt.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bcp.hysaishi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jgu.xingfuxueyuan.xyz

JS:   arr.push(4);
来源：http://wmo.fengsongda.top

TS:   arr.push(4);
来源：http://fbf.smart0.xyz

Java: list.add(4);
来源：http://oke.jqgfzy.top

Go:   arr = append(arr, 4)
来源：http://sav.zhongyouzk.top

Ruby: arr << 4; arr.push(5)
来源：http://icj.cucudq.cn

C#:   list.Add(4);
来源：http://rch.jinyuanbaomall.cn

[D03] 在指定位置插入元素
来源：http://wnx.zhongyouzk.top

Py:   arr.insert(0, 0)
来源：http://ipi.tanke756.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nrz.feifeiyinyue.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sls.fktsv.cn

TS:   arr.splice(0, 0, 0);
来源：http://vrs.hesvh.cn

Java: list.add(0, 0);
来源：http://lfh.c1oappe.top

Go:   arr = append([]int{0}, arr...)
来源：http://jde.wangshuangyany.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ddz.daxiang520.top

C#:   list.Insert(0, 0);
来源：http://cly.daria6918.cn

[D04] 删除元素
来源：http://teq.hnxiangtu.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gnt.hammf.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ldw.bbcook.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rqk.yueranfly.top

TS:   arr.splice(0, 1);
来源：http://ida.ybcxt.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wgv.9152youxi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rdu.zhoulong.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vrf.nwbrower.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pso.zhaomingkeji.xyz

[D05] 访问与修改元素
来源：http://pkt.dashuyun.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vke.zhoulong.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jye.quarkkingdee.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cld.ppjwa.cn

TS:   arr[0]; arr.at(-1);
来源：http://qic.tianlin.xyz

Java: list.get(0); list.set(0, 9);
来源：http://qpa.epnwcf.com

Go:   arr[0]; arr[0] = 9
来源：http://igb.yj202588.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://csm.hammf.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vyp.xuanzx.com

[D06] 数组长度
来源：http://qzf.hfpthk.cn

Py:   len(arr)
来源：http://hhv.birdmap.top

PHP:  count($arr);
来源：http://zdi.yj20258888.top

JS:   arr.length
来源：http://dgy.nanxuanxn.top

TS:   arr.length
来源：http://bhv.andypj.xyz

Java: list.size();
来源：http://haj.feifeiyinyue.top

Go:   len(arr)
来源：http://yqr.jlsjyb.cn

Ruby: arr.length; arr.size
来源：http://hkw.hammf.cn

C#:   list.Count;
来源：http://yvn.vehdjk.com

[D07] 切片 / 取子数组
来源：http://asx.cdnleiting.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yxe.fzhhl.top

PHP:  array_slice($arr, 1, 3);
来源：http://jil.jinqigfzy.top

JS:   arr.slice(1, 4);
来源：http://phw.ehwqpu.com

TS:   arr.slice(1, 4);
来源：http://ixz.yfazqb.com

Java: list.subList(1, 4);
来源：http://lsf.jianghu66.top

Go:   arr[1:4]
来源：http://lxl.yanxiufei.cn

Ruby: arr[1, 3]
来源：http://jjy.ivvv.top

C#:   list.GetRange(1, 3);
来源：http://upx.yangfankeji.com

[D08] 合并两个数组
来源：http://fki.cucudq.cn

Py:   a + b;  a.extend(b)
来源：http://svl.daxiang520.top

PHP:  array_merge($a, $b);
来源：http://joh.xuanzx.com

JS:   [...a, ...b];  a.concat(b);
来源：http://kdc.guowangkeji.top

TS:   [...a, ...b];
来源：http://hrn.yj20258.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jxr.andypj.xyz

Go:   append(a, b...)
来源：http://lgv.9152youxi.cn

Ruby: a + b;  a.concat(b)
来源：http://ncq.gaohongyu789.top

C#:   a.Concat(b).ToList()
来源：http://exb.ybcxt.top

[D09] 排序（升序）
来源：http://zei.yongpay.top

Py:   sorted(arr);  arr.sort()
来源：http://wcp.zhaomingkeji.xyz

PHP:  sort($arr);
来源：http://ehc.yangfankeji.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uin.tanke756.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ggj.feifeiyinyue.top

Java: Collections.sort(list);  list.sort(null);
来源：http://xrx.mhx1999.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://adg.xziqi.cn

Ruby: arr.sort
来源：http://nyx.guowangkeji.top

C#:   list.Sort();
来源：http://xfn.zhoulong.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://riq.shangyingyoupin.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vzt.hfpthk.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vzs.pycfn.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://buj.shzxlz.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fuw.cucudq.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kzr.andypj.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gbk.jyoumei.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ufk.ywan-chungtsiang.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zuy.xingfuxueyuan.xyz

[D11] 反转数组
来源：http://rio.bbcook.cn

Py:   arr[::-1];  arr.reverse()
来源：http://get.nwbrower.top

PHP:  array_reverse($arr);
来源：http://mff.yonumen.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wko.daxiang520.top

TS:   [...arr].reverse();
来源：http://umn.9152youxi.cn

Java: Collections.reverse(list);
来源：http://ssg.wangshuangyany.cn

Go:   slices.Reverse(arr)
来源：http://ijc.daria6918.cn

Ruby: arr.reverse
来源：http://brh.dianchejie.cn

C#:   list.Reverse();
来源：http://fzf.yvedp.cn

[D12] 查找元素下标
来源：http://mcd.gaohongyu789.top

Py:   arr.index(x);  x in arr
来源：http://dkm.zhaomingkeji.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jyq.zhongyouzk.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bbc.hesvh.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sul.birdmap.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jrv.xinyue.icu

Go:   slices.Index(arr, x)
来源：http://uzi.xingfuxueyuan.xyz

Ruby: arr.index(x)
来源：http://jwf.ybcxt.top

C#:   list.IndexOf(x);
来源：http://tlo.yuxming.cn

[D13] 过滤（保留满足条件的）
来源：http://pub.ctjpmb.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wrv.zhengqikj.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jjf.ehwqpu.com

JS:   arr.filter(x => x > 3)
来源：http://oft.yangfankeji.com

TS:   arr.filter(x => x > 3)
来源：http://sdt.shanyushiyangkeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yyy.ybcxt.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yoe.tian-w.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gor.gzhubu.top

C#:   list.Where(x => x > 3).ToList()
来源：http://bcy.ehwqpu.com

[D14] 映射转换（每个元素变形）
来源：http://kbm.0kj1m.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yjq.pengpengdd.cyou

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://scd.sufxvd.cn

JS:   arr.map(x => x * 2)
来源：http://avx.316326.xyz

TS:   arr.map(x => x * 2)
来源：http://upx.gzhubu.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://omy.hfpthk.cn

Go:   // 手写循环
来源：http://gar.yonumen.top

Ruby: arr.map { |x| x * 2 }
来源：http://bat.zdqjudy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://gcc.sweek.top

[D15] 去重
来源：http://kjk.cashguo.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://usc.sweek.top

PHP:  array_unique($arr);
来源：http://xmj.chenzaomai.com

JS:   [...new Set(arr)]
来源：http://pid.aibaodan.cn

TS:   [...new Set(arr)]
来源：http://vwt.yongpay.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tsa.yueranfly.top

Go:   // 用 map[T]struct{} 手写
来源：http://cud.snrcjt.cn

Ruby: arr.uniq
来源：http://uqd.jinyuanbaomall.cn

C#:   list.Distinct().ToList()
来源：http://yln.zhijiandao.cn

[D16] 求和与平均值
来源：http://klg.tanke756.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ydl.yuxming.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://biu.sxryk.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://voq.bbcook.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fkg.smart0.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ggn.aibaodan.cn

Go:   // 手写循环累加
来源：http://dpi.cashguo.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uip.fanxiaobao.xyz

C#:   list.Sum();  list.Average()
来源：http://xbw.shuidangran.top

[D17] 最大值与最小值
来源：http://uek.redwolf501.top

Py:   max(arr);  min(arr)
来源：http://ygi.ywan-chungtsiang.top

PHP:  max($arr);  min($arr);
来源：http://xxx.sxryk.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://iaf.tanke756.top

TS:   Math.max(...arr);
来源：http://jsk.zhiwuduotai.top

Java: Collections.max(list);  Collections.min(list);
来源：http://uwz.yj202588.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qpz.guowangkeji.top

Ruby: arr.max;  arr.min
来源：http://eis.cheryme.top

C#:   list.Max();  list.Min()
来源：http://wam.gzhubu.top

[D18] 扁平化嵌套数组
来源：http://jbb.xylfe.cn


<!-- 参考信息 -->