代发 wailian999

PHP:  $a && $b || !$c
来源：http://rdq.ydjk.org.cn

JS:   a && b || !c
来源：http://gxs.hysaishi.cn

TS:   a && b || !c
来源：http://kag.guowangkeji.top

Java: a && b || !c
来源：http://qgu.yj20258.top

Go:   a && b || !c
来源：http://xcn.meibo888.top

Ruby: a && b || !c
来源：http://lmn.hnxiangtu.top

C#:   a && b || !c
来源：http://wng.wangdashe.top

[B16] 卫语句：不满足条件提前返回
来源：http://rrs.svipenyu.cn

Py:   if not data: return
来源：http://hra.xylfe.cn

PHP:  if (!$data) { return; }
来源：http://sum.vehdjk.com

JS:   if (!data) return;
来源：http://lli.havefunace.top

TS:   if (!data) return;
来源：http://iml.zdqjudy.top

Java: if (data == null) return;
来源：http://pdg.zhijiandao.cn

Go:   if data == nil { return }
来源：http://ryk.shanyushiyangkeji.top

Ruby: return if data.nil?
来源：http://ynd.xinyue.icu

C#:   if (data == null) return;
来源：http://hnm.316326.xyz

================================================================================
来源：http://qca.tarul.cn

C. 函数与作用域
来源：http://uye.wangdashe.top

================================================================================
来源：http://kdb.shanyushiyangtech.top

[C01] 定义函数
来源：http://tte.chenjidiqi.icu

Py:   def add(a, b): return a + b
来源：http://ieh.zdqjudy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://avy.gzhubu.top

JS:   function add(a, b) { return a + b; }
来源：http://nmv.hcnkem.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xpx.yuxming.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://tzt.chenzaomai.com

Go:   func add(a, b int) int { return a + b }
来源：http://ulo.zhijiandao.cn

Ruby: def add(a, b); a + b; end
来源：http://qpv.nanxinkj.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://srd.xuetiantiany.cn

[C02] 默认参数
来源：http://fam.yuxming.cn

Py:   def greet(name="World"): return name
来源：http://qly.chenjidiqi.icu

PHP:  function greet($name = "World") { return $name; }
来源：http://gfj.cdnleiting.top

JS:   function greet(name = "World") { return name; }
来源：http://sjq.guowangkeji.top

TS:   function greet(name: string = "World") { return name; }
来源：http://rdx.hysaishi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vtg.xuanzx.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mph.ctjpmb.com

Ruby: def greet(name = "World") = name
来源：http://glx.vehdjk.com

C#:   string Greet(string name = "World") => name;
来源：http://day.zhijiandao.cn

[C03] 可变参数
来源：http://bak.jianghu66.top

Py:   def total(*args): return sum(args)
来源：http://stp.sysykeji.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xjc.c1oappe.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cko.tianlin.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sak.sxryk.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pql.shanyushiyangkeji.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ddx.redwolf501.top

Ruby: def total(*nums); nums.sum; end
来源：http://pew.hammf.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ceo.gogol.net.cn

[C04] 命名参数 / 关键字参数
来源：http://uks.yueranfly.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wij.tian-w.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ewq.zdqjudy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://htz.jyoumei.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://udu.iojbl.cn

Java: // 无：用 Builder 模式或 record
来源：http://cdh.chenjidiqi.icu

Go:   // 无：用配置结构体参数
来源：http://ebr.svipenyu.cn

Ruby: f(a: 1, b: 2)
来源：http://dbi.sysykeji.top

C#:   f(a: 1, b: 2)
来源：http://jul.jinghuilouyu.cn

[C05] 返回多个值
来源：http://imq.tarul.cn

Py:   return a, b
来源：http://elx.hnqzz.top

PHP:  return [$a, $b];
来源：http://czz.smart0.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://krv.tianlin.xyz

TS:   return { a, b };
来源：http://sgt.dianchejie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bin.havefunace.top

Go:   return a, b
来源：http://eme.pengpengdd.cyou

Ruby: return a, b
来源：http://coc.pengpengdd.cyou

C#:   return (a, b);              // ValueTuple
来源：http://xgf.zdbjq.cn

[C06] 匿名函数 / lambda
来源：http://vsv.chenzaomai.com

Py:   square = lambda x: x * x
来源：http://kat.wangshuangyany.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vlg.aizwys.cn

JS:   const square = x => x * x;
来源：http://rkg.zhaomingkeji.xyz

TS:   const square = (x: number): number => x * x;
来源：http://gya.sysykeji.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://obb.aibaodan.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xwo.yfazqb.com

Ruby: square = ->(x) { x * x }
来源：http://yfg.hnxiangtu.top

C#:   Func<int, int> square = x => x * x;
来源：http://zxs.jqgufenzy.top

[C07] 把函数作为参数传入
来源：http://axa.zdqjudy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wyt.sjlbkw.cn

PHP:  array_map("strtoupper", $arr);
来源：http://nqx.daxiang520.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mcq.guannengcc.top

TS:   arr.map(String)
来源：http://yuy.havefunace.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pqm.zhongyouzk.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vmu.shanyushiyangtech.top

Ruby: arr.map(&:upcase)
来源：http://pqg.wangshuangyany.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://nnh.shanyushiyangkeji.top

[C08] 闭包
来源：http://jvo.hcnkem.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vto.yj20258.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vei.yfazqb.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://abs.vqdsnc.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sdv.tarul.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dtn.wangshuangyany.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xou.havefunace.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ekq.shuidangran.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tsd.bbcook.cn

[C09] 递归
来源：http://yje.yuxming.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://duw.jinghuilouyu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pso.sweek.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://psx.ehwqpu.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ofs.jiagoushi.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ojp.redwolf501.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lyi.cdnleiting.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vxs.0kj1m.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wto.ywan-chungtsiang.top

[C10] 变量作用域
来源：http://yng.zhaomingkeji.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://agy.xingfuxueyuan.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kff.yanxiufei.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xyo.epnwcf.com

TS:   同 JS
来源：http://cct.wangdashe.top

Java: 方法内为块级作用域
来源：http://niw.hywenlv.cn

Go:   花括号块级作用域
来源：http://hvm.shzxlz.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lti.gzhubu.top

C#:   块级作用域
来源：http://dia.52xcode.cn

[C11] 模块导入与导出
来源：http://hvj.yanxiufei.cn

Py:   from module import func
来源：http://gjr.zdbjq.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zxl.xuetiantiany.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://dal.sjlbkw.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wwh.sufxvd.cn

Java: import java.util.List;
来源：http://rcj.birdmap.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gjk.fktsv.cn

Ruby: require "json"; require_relative "./util"
来源：http://thx.dianchejie.cn

C#:   using System.Text;
来源：http://pmf.gzhubu.top

[C12] 立即执行函数 IIFE
来源：http://lvx.uphjek.com

Py:   (lambda: print("run"))()
来源：http://zaj.tianlin.xyz

PHP:  (function () { echo "run"; })();
来源：http://kcn.dashuyun.cn

JS:   (() => { console.log("run"); })();
来源：http://pli.zhaomingkeji.xyz

TS:   (() => { console.log("run"); })();
来源：http://znp.hammf.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jvn.xziqi.cn

Go:   func() { fmt.Println("run") }()
来源：http://tft.daria6918.cn

Ruby: -> { puts "run" }.call
来源：http://wqe.bjfxy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://yaa.xuetiantiany.cn

[C13] 类型声明 / 类型注解
来源：http://unh.jinyuanbaomall.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rqx.tarul.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jtv.jinyuanbaomall.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://whc.xuanzx.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wwo.yanxiufei.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jbv.wangdashe.top

Go:   func add(a, b int) int
来源：http://def.birdmap.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rki.yueranfly.top

C#:   int Add(int a, int b) => a + b;
来源：http://saq.sufxvd.cn

[C14] 泛型函数
来源：http://jas.jiagoushi.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uhw.316326.xyz

PHP:  // 无泛型
来源：http://par.c1oappe.top

JS:   // 无泛型
来源：http://adx.aibaodan.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ytb.shzxlz.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uec.yonumen.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ckw.snrcjt.cn

Ruby: # 无泛型
来源：http://nkg.shanyushiyangtech.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vwa.jinqigfzy.top

[C15] 解构 / 展开参数
来源：http://nin.shangyingyoupin.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dze.iojbl.cn

PHP:  [$a, $b] = $pair;
来源：http://ujk.haohaochexian.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://usp.aizwys.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://srt.gotoacloud.top

Java: // 无解构
来源：http://jhc.yj20258.top

Go:   // 无解构
来源：http://fej.gzhubu.top

Ruby: a, b = pair
来源：http://gdk.hcnkem.com

C#:   var (a, b) = pair;
来源：http://ekh.hysaishi.cn

[C16] 函数 / 方法重载
来源：http://bde.shuidangran.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pjt.sufxvd.cn

PHP:  // 无重载
来源：http://ipo.ybcxt.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ore.hnqzz.top

TS:   // 用联合类型或重载签名声明
来源：http://wqo.aizwys.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://kqx.cheryme.top

Go:   // 无重载：用不同函数名
来源：http://sdq.meibo888.top

Ruby: # 无重载：靠动态参数
来源：http://ltk.bjfxy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://clz.c1oappe.top

================================================================================
来源：http://wxv.dashuyun.cn

D. 数组 / 列表 / 集合
来源：http://dso.bjfxy.top

================================================================================
来源：http://rzd.dianchejie.cn

[D01] 创建数组 / 列表
来源：http://bfq.havefunace.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://bki.jqgufenzy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zdz.sxryk.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xzt.smart0.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://npp.hammf.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://urh.ydjk.org.cn

Go:   arr := []int{1, 2, 3}
来源：http://wig.havefunace.top

Ruby: arr = [1, 2, 3]
来源：http://fbz.ctjpmb.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://faj.xinyue.icu

[D02] 追加元素到末尾
来源：http://srj.shuidangran.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vbj.zhengqikj.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vda.jinqigfzy.top

JS:   arr.push(4);
来源：http://ccq.xylfe.cn

TS:   arr.push(4);
来源：http://oxz.iojbl.cn

Java: list.add(4);
来源：http://hkr.chenzaomai.com

Go:   arr = append(arr, 4)
来源：http://orc.sjlbkw.cn

Ruby: arr << 4; arr.push(5)
来源：http://ihh.cdnleiting.top

C#:   list.Add(4);
来源：http://ybg.ctjpmb.com

[D03] 在指定位置插入元素
来源：http://cci.guowangkeji.top

Py:   arr.insert(0, 0)
来源：http://hvr.epnwcf.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hdz.yongpay.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mqe.xinyue.icu

TS:   arr.splice(0, 0, 0);
来源：http://ebf.jlsjyb.cn

Java: list.add(0, 0);
来源：http://lfw.yvedp.cn

Go:   arr = append([]int{0}, arr...)
来源：http://srk.sxryk.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://iah.chenzaomai.com

C#:   list.Insert(0, 0);
来源：http://ooe.feifeiyinyue.top

[D04] 删除元素
来源：http://spe.pycfn.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tji.shangyingyoupin.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pmt.xziqi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bsf.zhoulong.xyz

TS:   arr.splice(0, 1);
来源：http://trr.jyoumei.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://awd.yanxiufei.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yjz.wangdashe.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hmc.ydzc1.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://eqz.uphjek.com

[D05] 访问与修改元素
来源：http://srd.yongpay.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gkg.gogol.net.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://egr.wangdashe.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kvz.jyoumei.cn

TS:   arr[0]; arr.at(-1);
来源：http://thq.ydzc1.top

Java: list.get(0); list.set(0, 9);
来源：http://hfn.epnwcf.com

Go:   arr[0]; arr[0] = 9
来源：http://zyw.xylfe.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://eab.jiagoushi.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://skr.zhengqikj.top

[D06] 数组长度
来源：http://vdy.jinqigufen.top

Py:   len(arr)
来源：http://sfv.jqgfzy.top

PHP:  count($arr);
来源：http://olh.guannengcc.top

JS:   arr.length
来源：http://chd.yonumen.top

TS:   arr.length
来源：http://ynb.jqgfzy.top

Java: list.size();
来源：http://cvi.jiagoushi.top

Go:   len(arr)
来源：http://wny.mhx1999.top

Ruby: arr.length; arr.size
来源：http://kib.zhixingplan.top

C#:   list.Count;
来源：http://hne.yj202588.top

[D07] 切片 / 取子数组
来源：http://aid.0kj1m.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gpx.gotoacloud.top

PHP:  array_slice($arr, 1, 3);
来源：http://eev.fehbvm.com

JS:   arr.slice(1, 4);
来源：http://dfg.sufxvd.cn

TS:   arr.slice(1, 4);
来源：http://iom.shangyingyoupin.top

Java: list.subList(1, 4);
来源：http://bym.zhaomingkeji.xyz

Go:   arr[1:4]
来源：http://sha.havefunace.top

Ruby: arr[1, 3]
来源：http://kmx.vehdjk.com

C#:   list.GetRange(1, 3);
来源：http://vur.hnqzz.top

[D08] 合并两个数组
来源：http://xoe.zhijiandao.cn

Py:   a + b;  a.extend(b)
来源：http://dzb.ywan-chungtsiang.top

PHP:  array_merge($a, $b);
来源：http://isq.gotoacloud.top

JS:   [...a, ...b];  a.concat(b);
来源：http://cku.zhengqikj.top

TS:   [...a, ...b];
来源：http://pfd.redwolf501.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jdg.vehdjk.com

Go:   append(a, b...)
来源：http://bjg.zdbjq.cn

Ruby: a + b;  a.concat(b)
来源：http://rpy.pengpengdd.cyou

C#:   a.Concat(b).ToList()
来源：http://asu.nanxuanxn.top

[D09] 排序（升序）
来源：http://kpu.hongshengwenyu.top

Py:   sorted(arr);  arr.sort()
来源：http://ufr.nanxinkj.top

PHP:  sort($arr);
来源：http://lwu.hywenlv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rnd.jinyuanbaomall.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ohz.chenjidiqi.icu

Java: Collections.sort(list);  list.sort(null);
来源：http://gxt.xuanzx.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qtb.tianlin.xyz

Ruby: arr.sort
来源：http://qbj.xingfuxueyuan.xyz

C#:   list.Sort();
来源：http://utl.daria6918.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://utu.fehbvm.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://khy.cdnleiting.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ghh.sufxvd.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dwf.guowangkeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://twv.sysykeji.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ufs.zhaomingkeji.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jjv.yj20258888.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sve.svipenyu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rag.epnwcf.com

[D11] 反转数组
来源：http://uxm.yanxiufei.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rrw.ivvv.top

PHP:  array_reverse($arr);
来源：http://nmw.xuanzx.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jgk.cdnleiting.top

TS:   [...arr].reverse();
来源：http://rjk.vqdsnc.cn

Java: Collections.reverse(list);
来源：http://veh.zhijiandao.cn

Go:   slices.Reverse(arr)
来源：http://hoj.shuidangran.top

Ruby: arr.reverse
来源：http://cbj.gaohongyu789.top

C#:   list.Reverse();
来源：http://uin.hnxiangtu.top

[D12] 查找元素下标
来源：http://ost.sweek.top

Py:   arr.index(x);  x in arr
来源：http://pmq.zycfv.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ddw.zycfv.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://daq.sjlbkw.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wgo.jiagoushi.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xsm.hammf.cn

Go:   slices.Index(arr, x)
来源：http://pua.pycfn.com

Ruby: arr.index(x)
来源：http://gfi.yonumen.top

C#:   list.IndexOf(x);
来源：http://fua.shanyushiyangtech.top

[D13] 过滤（保留满足条件的）
来源：http://nvj.yuanzhike.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xlj.shanyushiyangtech.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ibj.shzxlz.cn

JS:   arr.filter(x => x > 3)
来源：http://hxw.meibo888.top

TS:   arr.filter(x => x > 3)
来源：http://yqe.jiagoushi.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tgo.zhijiandao.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gdh.ppjwa.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vhd.gzhubu.top

C#:   list.Where(x => x > 3).ToList()
来源：http://lur.meibo888.top

[D14] 映射转换（每个元素变形）
来源：http://vuj.tian-w.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://aac.316326.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mrd.zhoulong.xyz

JS:   arr.map(x => x * 2)
来源：http://qnn.0kj1m.cn

TS:   arr.map(x => x * 2)
来源：http://wuu.sjlbkw.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://tas.hnqzz.top

Go:   // 手写循环
来源：http://bwe.jlsjyb.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qim.yueranfly.top

C#:   list.Select(x => x * 2).ToList()
来源：http://fqo.yfazqb.com

[D15] 去重
来源：http://prr.jqgfzy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zvc.zdbjq.cn

PHP:  array_unique($arr);
来源：http://dri.yj20258.top

JS:   [...new Set(arr)]
来源：http://rwr.aizwys.cn

TS:   [...new Set(arr)]
来源：http://zhv.birdmap.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://axk.gogol.net.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xrf.ybcxt.top

Ruby: arr.uniq
来源：http://tpl.daxiang520.top


<!-- 参考信息 -->