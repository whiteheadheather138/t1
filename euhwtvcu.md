代发 wailian999

Go:   a && b || !c
来源：http://owl.316326.xyz

Ruby: a && b || !c
来源：http://zef.sjlbkw.cn

C#:   a && b || !c
来源：http://sdr.mhx1999.top

[B16] 卫语句：不满足条件提前返回
来源：http://uwd.jinyuanbaomall.cn

Py:   if not data: return
来源：http://kfi.hammf.cn

PHP:  if (!$data) { return; }
来源：http://jlh.uphjek.com

JS:   if (!data) return;
来源：http://its.hammf.cn

TS:   if (!data) return;
来源：http://ikp.sjlbkw.cn

Java: if (data == null) return;
来源：http://quh.jinghuilouyu.cn

Go:   if data == nil { return }
来源：http://oqz.xuanzx.com

Ruby: return if data.nil?
来源：http://jzm.yj202588.top

C#:   if (data == null) return;
来源：http://fei.chenjidiqi.icu

================================================================================
来源：http://ggu.daxiang520.top

C. 函数与作用域
来源：http://syo.wangshuangyany.cn

================================================================================
来源：http://asw.ppjwa.cn

[C01] 定义函数
来源：http://jvi.gotoacloud.top

Py:   def add(a, b): return a + b
来源：http://bdg.cqqwz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gtu.zhijiandao.cn

JS:   function add(a, b) { return a + b; }
来源：http://spn.52xcode.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://idr.fanxiaobao.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://ddu.zycfv.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ixn.hesvh.cn

Ruby: def add(a, b); a + b; end
来源：http://bwa.0kj1m.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ddx.tianlin.xyz

[C02] 默认参数
来源：http://kfu.sysykeji.top

Py:   def greet(name="World"): return name
来源：http://tjl.pycfn.com

PHP:  function greet($name = "World") { return $name; }
来源：http://twt.mhx1999.top

JS:   function greet(name = "World") { return name; }
来源：http://mjx.jlsjyb.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hjf.zhengqikj.top

Java: // 无默认参数：方法重载或 Optional
来源：http://xea.feifeiyinyue.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jqk.zhixingplan.top

Ruby: def greet(name = "World") = name
来源：http://xhc.quarkkingdee.top

C#:   string Greet(string name = "World") => name;
来源：http://xll.tanke756.top

[C03] 可变参数
来源：http://wxj.hnxiangtu.top

Py:   def total(*args): return sum(args)
来源：http://vvu.cheryme.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ntb.yuanzhike.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gcx.yuxming.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ycr.316326.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jti.ehwqpu.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ukp.uphjek.com

Ruby: def total(*nums); nums.sum; end
来源：http://ews.fanxiaobao.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pvo.daria6918.cn

[C04] 命名参数 / 关键字参数
来源：http://xyi.epnwcf.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vgl.yuanzhike.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kfb.shanyushiyangtech.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xeh.jinyuanbaomall.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hao.quarkkingdee.top

Java: // 无：用 Builder 模式或 record
来源：http://rhx.nanxuanxn.top

Go:   // 无：用配置结构体参数
来源：http://zzs.yueranfly.top

Ruby: f(a: 1, b: 2)
来源：http://ckv.guannengcc.top

C#:   f(a: 1, b: 2)
来源：http://gpd.jqgfzy.top

[C05] 返回多个值
来源：http://wau.sufxvd.cn

Py:   return a, b
来源：http://isl.ydzc1.top

PHP:  return [$a, $b];
来源：http://tzi.nanxuanxn.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://isi.hcnkem.com

TS:   return { a, b };
来源：http://pbc.hcnkem.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kse.gotoacloud.top

Go:   return a, b
来源：http://czn.redwolf501.top

Ruby: return a, b
来源：http://uou.xuetiantiany.cn

C#:   return (a, b);              // ValueTuple
来源：http://zby.vehdjk.com

[C06] 匿名函数 / lambda
来源：http://czl.chenlongwang.top

Py:   square = lambda x: x * x
来源：http://rkm.cucudq.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://aml.0kj1m.cn

JS:   const square = x => x * x;
来源：http://vvo.hammf.cn

TS:   const square = (x: number): number => x * x;
来源：http://fdi.vehdjk.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mzk.tarul.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lyb.hcnkem.com

Ruby: square = ->(x) { x * x }
来源：http://qli.guowangkeji.top

C#:   Func<int, int> square = x => x * x;
来源：http://jwr.svipenyu.cn

[C07] 把函数作为参数传入
来源：http://qvz.shanyushiyangtech.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ail.xingfuxueyuan.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://jlo.shanyushiyangkeji.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qin.fktsv.cn

TS:   arr.map(String)
来源：http://ssh.ybcxt.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tsf.xylfe.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://thn.cheryme.top

Ruby: arr.map(&:upcase)
来源：http://vdb.hywenlv.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xfj.meibo888.top

[C08] 闭包
来源：http://qtm.yj20258.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://aem.svipenyu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ufy.yuxming.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://stg.tanke756.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://adb.jiagoushi.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rkt.shuidangran.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kgo.0kj1m.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rla.shanyushiyangkeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qpw.iojbl.cn

[C09] 递归
来源：http://vhj.cashguo.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lzm.nwbrower.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mcp.jinqigfzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ugx.sysykeji.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ovu.smart0.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://foe.xingfuxueyuan.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mzg.bjfxy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uee.jinqigufen.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pqf.haohaochexian.top

[C10] 变量作用域
来源：http://sor.uphjek.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://oxl.yueranfly.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://huv.daria6918.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mrh.yueranfly.top

TS:   同 JS
来源：http://wxo.yj202588.top

Java: 方法内为块级作用域
来源：http://uqm.sufxvd.cn

Go:   花括号块级作用域
来源：http://pmu.316326.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kkg.svipenyu.cn

C#:   块级作用域
来源：http://pqi.iojbl.cn

[C11] 模块导入与导出
来源：http://pgq.gotoacloud.top

Py:   from module import func
来源：http://xpb.cucudq.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mlp.tanke756.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://fbr.tian-w.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uxs.pycfn.com

Java: import java.util.List;
来源：http://lcv.guowangkeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dxb.jinyuanbaomall.cn

Ruby: require "json"; require_relative "./util"
来源：http://abt.zhiwuduotai.top

C#:   using System.Text;
来源：http://coa.andypj.xyz

[C12] 立即执行函数 IIFE
来源：http://jvd.xziqi.cn

Py:   (lambda: print("run"))()
来源：http://jqo.gogol.net.cn

PHP:  (function () { echo "run"; })();
来源：http://bzp.zhongyouzk.top

JS:   (() => { console.log("run"); })();
来源：http://yvb.smart0.xyz

TS:   (() => { console.log("run"); })();
来源：http://hvy.0kj1m.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nxd.zhixingplan.top

Go:   func() { fmt.Println("run") }()
来源：http://pcj.jinqigfzy.top

Ruby: -> { puts "run" }.call
来源：http://tsf.shuidangran.top

C#:   // 无 IIFE：用静态构造函数
来源：http://xuq.zycfv.cn

[C13] 类型声明 / 类型注解
来源：http://wfz.9152youxi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vwy.ybcxt.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kiq.sysykeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://saf.uphjek.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fjp.yj202588.top

Java: int add(int a, int b) { return a + b; }
来源：http://wjd.zhoulong.xyz

Go:   func add(a, b int) int
来源：http://vsz.dianchejie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uka.sweek.top

C#:   int Add(int a, int b) => a + b;
来源：http://lnl.sweek.top

[C14] 泛型函数
来源：http://tqd.shzxlz.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rnk.fengsongda.top

PHP:  // 无泛型
来源：http://myu.ppjwa.cn

JS:   // 无泛型
来源：http://swg.hesvh.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://byh.zycfv.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mzl.zhengqikj.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ytd.shanyushiyangkeji.top

Ruby: # 无泛型
来源：http://iuo.vehdjk.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nrv.gzhubu.top

[C15] 解构 / 展开参数
来源：http://kcd.yvedp.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sqv.wangdashe.top

PHP:  [$a, $b] = $pair;
来源：http://wta.nanxuanxn.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qmp.vehdjk.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hva.ywan-chungtsiang.top

Java: // 无解构
来源：http://gxu.tarul.cn

Go:   // 无解构
来源：http://qxc.tanke756.top

Ruby: a, b = pair
来源：http://yvj.feifeiyinyue.top

C#:   var (a, b) = pair;
来源：http://kzd.jianghu66.top

[C16] 函数 / 方法重载
来源：http://fdy.aibaodan.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rzu.cdnleiting.top

PHP:  // 无重载
来源：http://yep.nanxuanxn.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://llx.feifeiyinyue.top

TS:   // 用联合类型或重载签名声明
来源：http://sob.bjfxy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://szk.yj20258888.top

Go:   // 无重载：用不同函数名
来源：http://xgj.birdmap.top

Ruby: # 无重载：靠动态参数
来源：http://gvb.ydzc1.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://nnh.gzhubu.top

================================================================================
来源：http://vaq.cucudq.cn

D. 数组 / 列表 / 集合
来源：http://nxn.zhengqikj.top

================================================================================
来源：http://jnu.nwbrower.top

[D01] 创建数组 / 列表
来源：http://asp.birdmap.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://yoj.meibo888.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dij.hammf.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ymu.aibaodan.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bbo.shuidangran.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pof.xziqi.cn

Go:   arr := []int{1, 2, 3}
来源：http://lxt.c1oappe.top

Ruby: arr = [1, 2, 3]
来源：http://xos.52xcode.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qwj.xziqi.cn

[D02] 追加元素到末尾
来源：http://pgc.yfazqb.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cbd.zhoulong.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ait.gaohongyu789.top

JS:   arr.push(4);
来源：http://bnu.pycfn.com

TS:   arr.push(4);
来源：http://iqu.zhixingplan.top

Java: list.add(4);
来源：http://ktg.xinyue.icu

Go:   arr = append(arr, 4)
来源：http://vco.ywan-chungtsiang.top

Ruby: arr << 4; arr.push(5)
来源：http://vwp.ctjpmb.com

C#:   list.Add(4);
来源：http://gzb.zhaomingkeji.xyz

[D03] 在指定位置插入元素
来源：http://qpj.sxryk.cn

Py:   arr.insert(0, 0)
来源：http://sdw.sjlbkw.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zrz.gogol.net.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pas.hongshengwenyu.top

TS:   arr.splice(0, 0, 0);
来源：http://gjb.zhongyouzk.top

Java: list.add(0, 0);
来源：http://erz.bbcook.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yoc.birdmap.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tau.jiagoushi.top

C#:   list.Insert(0, 0);
来源：http://ghi.bjfxy.top

[D04] 删除元素
来源：http://rnh.shuidangran.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://brz.nwbrower.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://oup.9152youxi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rjs.9152youxi.cn

TS:   arr.splice(0, 1);
来源：http://wkp.c1oappe.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mgi.sjlbkw.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://psh.sxryk.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://olh.zhaomingkeji.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nkx.jinyuanbaomall.cn

[D05] 访问与修改元素
来源：http://htr.shanyushiyangtech.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gvm.tarul.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qmp.hnxiangtu.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jec.jlsjyb.cn

TS:   arr[0]; arr.at(-1);
来源：http://nzd.tianlin.xyz

Java: list.get(0); list.set(0, 9);
来源：http://xmg.tarul.cn

Go:   arr[0]; arr[0] = 9
来源：http://tcu.xziqi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://eyj.fengsongda.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://umg.ehwqpu.com

[D06] 数组长度
来源：http://qct.wangshuangyany.cn

Py:   len(arr)
来源：http://hty.sjlbkw.cn

PHP:  count($arr);
来源：http://kaq.yonumen.top

JS:   arr.length
来源：http://blq.wangshuangyany.cn

TS:   arr.length
来源：http://wna.havefunace.top

Java: list.size();
来源：http://ran.svipenyu.cn

Go:   len(arr)
来源：http://hyj.zhengqikj.top

Ruby: arr.length; arr.size
来源：http://viv.vehdjk.com

C#:   list.Count;
来源：http://yaa.zhiwuduotai.top

[D07] 切片 / 取子数组
来源：http://ghf.wangshuangyany.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lnw.svipenyu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jww.pengpengdd.cyou

JS:   arr.slice(1, 4);
来源：http://bgs.jinyuanbaomall.cn

TS:   arr.slice(1, 4);
来源：http://zsv.svipenyu.cn

Java: list.subList(1, 4);
来源：http://hix.xingfuxueyuan.xyz

Go:   arr[1:4]
来源：http://tzl.chenzaomai.com

Ruby: arr[1, 3]
来源：http://kcl.jinyuanbaomall.cn

C#:   list.GetRange(1, 3);
来源：http://idt.xuetiantiany.cn

[D08] 合并两个数组
来源：http://ozd.cashguo.top

Py:   a + b;  a.extend(b)
来源：http://amj.ydjk.org.cn

PHP:  array_merge($a, $b);
来源：http://mbd.iojbl.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pmr.jinqigfzy.top

TS:   [...a, ...b];
来源：http://fqp.fehbvm.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nko.haohaochexian.top

Go:   append(a, b...)
来源：http://sif.ybcxt.top

Ruby: a + b;  a.concat(b)
来源：http://rjh.hongshengwenyu.top

C#:   a.Concat(b).ToList()
来源：http://cls.hcnkem.com

[D09] 排序（升序）
来源：http://ndn.jlsjyb.cn

Py:   sorted(arr);  arr.sort()
来源：http://ieg.xylfe.cn

PHP:  sort($arr);
来源：http://qsd.havefunace.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ylz.kuanghao11.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ggn.cqqwz.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://btl.ivvv.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://seq.dianchejie.cn

Ruby: arr.sort
来源：http://nbd.yonumen.top

C#:   list.Sort();
来源：http://fbx.aibaodan.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://cbm.bjfxy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://isr.nwbrower.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yjm.fktsv.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dif.hnqzz.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://isa.cheryme.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gpj.guannengcc.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xui.yj20258.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pbc.fzhhl.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bmp.cdnleiting.top

[D11] 反转数组
来源：http://iwo.yonumen.top

Py:   arr[::-1];  arr.reverse()
来源：http://iod.zycfv.cn

PHP:  array_reverse($arr);
来源：http://dyu.yonumen.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rvq.9152youxi.cn

TS:   [...arr].reverse();
来源：http://ejz.shangyingyoupin.top

Java: Collections.reverse(list);
来源：http://yti.vqdsnc.cn

Go:   slices.Reverse(arr)
来源：http://tap.bbcook.cn

Ruby: arr.reverse
来源：http://hmy.ydzc1.top

C#:   list.Reverse();
来源：http://oql.uphjek.com

[D12] 查找元素下标
来源：http://hbd.yueranfly.top

Py:   arr.index(x);  x in arr
来源：http://lxw.dianchejie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fxm.tarul.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ejm.zycfv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jbv.ybcxt.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ljj.hammf.cn

Go:   slices.Index(arr, x)
来源：http://zgd.sufxvd.cn

Ruby: arr.index(x)
来源：http://jpz.vqdsnc.cn

C#:   list.IndexOf(x);
来源：http://keu.hongshengwenyu.top

[D13] 过滤（保留满足条件的）
来源：http://kcq.shangyingyoupin.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://apx.fehbvm.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qkl.aizwys.cn

JS:   arr.filter(x => x > 3)
来源：http://unz.kuanghao11.cn

TS:   arr.filter(x => x > 3)
来源：http://oxp.jinqigfzy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lgm.xinyue.icu

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qcd.yj202588.top

Ruby: arr.select { |x| x > 3 }
来源：http://jbz.svipenyu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://clk.xuanzx.com

[D14] 映射转换（每个元素变形）
来源：http://ymd.vehdjk.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://edh.zhiwuduotai.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qiw.dashuyun.cn

JS:   arr.map(x => x * 2)
来源：http://kes.fehbvm.com

TS:   arr.map(x => x * 2)
来源：http://kce.shuidangran.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://xam.feifeiyinyue.top

Go:   // 手写循环
来源：http://nsq.gogol.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hew.hysaishi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xbz.ywan-chungtsiang.top

[D15] 去重
来源：http://rxg.hywenlv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ola.hywenlv.cn

PHP:  array_unique($arr);
来源：http://kjq.zhoulong.xyz

JS:   [...new Set(arr)]
来源：http://rqq.yongpay.top

TS:   [...new Set(arr)]
来源：http://hrp.andypj.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://osp.yongpay.top

Go:   // 用 map[T]struct{} 手写
来源：http://uts.chenzaomai.com

Ruby: arr.uniq
来源：http://sfw.jlsjyb.cn

C#:   list.Distinct().ToList()
来源：http://lbw.feifeiyinyue.top

[D16] 求和与平均值
来源：http://bfx.havefunace.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pli.shuidangran.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zmp.fktsv.cn


<!-- 参考信息 -->