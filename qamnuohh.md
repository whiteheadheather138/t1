代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qcj.vehdjk.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lvj.yangfankeji.com

[B11] 生成数字序列 / 区间
来源：http://ssr.meibo888.top

Py:   list(range(0, 10, 2))
来源：http://ehn.52xcode.cn

PHP:  range(0, 10, 2);
来源：http://ozi.gaohongyu789.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://swe.ydjk.org.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://btz.hesvh.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rup.kuanghao11.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://btb.yonumen.top

Ruby: (0...10).step(2).to_a
来源：http://yet.tarul.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://eay.jqgfzy.top

[B12] 跳出多层循环
来源：http://ozl.tian-w.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://qah.xuanzx.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://zwf.daria6918.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ldu.fanxiaobao.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ltq.zycfv.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dnx.jiagoushi.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vja.nanxuanxn.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qun.ehwqpu.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bhl.ppjwa.cn

[B13] 判断是否为数字
来源：http://cfa.tarul.cn

Py:   isinstance(x, (int, float))
来源：http://tsq.yvedp.cn

PHP:  is_numeric($x)
来源：http://okr.ydzc1.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wlj.fehbvm.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://eiv.hysaishi.cn

Java: x instanceof Number
来源：http://kpp.ywan-chungtsiang.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://czt.tanke756.top

Ruby: x.is_a?(Numeric)
来源：http://pwr.yj20258.top

C#:   x is int or double or decimal
来源：http://cej.ctjpmb.com

[B14] 判断值是否在集合内
来源：http://wxn.zhoulong.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sdo.svipenyu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uhh.zhoulong.xyz

JS:   [1, 2, 3].includes(x)
来源：http://urr.zhoulong.xyz

TS:   [1, 2, 3].includes(x)
来源：http://lyt.nanxuanxn.top

Java: List.of(1, 2, 3).contains(x)
来源：http://cik.yanxiufei.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wrw.mhx1999.top

Ruby: [1, 2, 3].include?(x)
来源：http://pkn.zhijiandao.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://akx.dianchejie.cn

[B15] 布尔运算与取反
来源：http://dhn.chenlongwang.top

Py:   a and b or not c
来源：http://uxl.ctjpmb.com

PHP:  $a && $b || !$c
来源：http://zuo.fktsv.cn

JS:   a && b || !c
来源：http://kbu.epnwcf.com

TS:   a && b || !c
来源：http://izf.pengpengdd.cyou

Java: a && b || !c
来源：http://zuw.tarul.cn

Go:   a && b || !c
来源：http://ctz.jinghuilouyu.cn

Ruby: a && b || !c
来源：http://kbd.yj202588.top

C#:   a && b || !c
来源：http://nae.zhoulong.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://uoj.0kj1m.cn

Py:   if not data: return
来源：http://gjn.chenlongwang.top

PHP:  if (!$data) { return; }
来源：http://dke.guowangkeji.top

JS:   if (!data) return;
来源：http://xep.sjlbkw.cn

TS:   if (!data) return;
来源：http://pnf.ctjpmb.com

Java: if (data == null) return;
来源：http://nbt.gotoacloud.top

Go:   if data == nil { return }
来源：http://tjg.aibaodan.cn

Ruby: return if data.nil?
来源：http://nex.yj20258888.top

C#:   if (data == null) return;
来源：http://rmb.jinyuanbaomall.cn

================================================================================
来源：http://kxz.yj202588.top

C. 函数与作用域
来源：http://rsg.smart0.xyz

================================================================================
来源：http://sdt.shuidangran.top

[C01] 定义函数
来源：http://xwt.hysaishi.cn

Py:   def add(a, b): return a + b
来源：http://ekm.birdmap.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kmb.feifeiyinyue.top

JS:   function add(a, b) { return a + b; }
来源：http://wnf.dianchejie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lbn.zhiwuduotai.top

Java: static int add(int a, int b) { return a + b; }
来源：http://wnf.52xcode.cn

Go:   func add(a, b int) int { return a + b }
来源：http://whd.yuxming.cn

Ruby: def add(a, b); a + b; end
来源：http://soo.xinyue.icu

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pbd.hnqzz.top

[C02] 默认参数
来源：http://qaw.zdqjudy.top

Py:   def greet(name="World"): return name
来源：http://vod.smart0.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://iqj.c1oappe.top

JS:   function greet(name = "World") { return name; }
来源：http://brc.shzxlz.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://dtl.yueranfly.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ayp.c1oappe.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ilk.iojbl.cn

Ruby: def greet(name = "World") = name
来源：http://zdr.yonumen.top

C#:   string Greet(string name = "World") => name;
来源：http://pdi.zdqjudy.top

[C03] 可变参数
来源：http://ywp.hammf.cn

Py:   def total(*args): return sum(args)
来源：http://txj.jinyuanbaomall.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cws.wangshuangyany.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hav.sweek.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mov.epnwcf.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rao.zdqjudy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qcj.yongpay.top

Ruby: def total(*nums); nums.sum; end
来源：http://vfu.yj20258.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kmk.tanke756.top

[C04] 命名参数 / 关键字参数
来源：http://bdg.zhengqikj.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ppz.uphjek.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bpx.jianghu66.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dzx.nanxinkj.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kvl.jyoumei.cn

Java: // 无：用 Builder 模式或 record
来源：http://wfk.fktsv.cn

Go:   // 无：用配置结构体参数
来源：http://zdj.svipenyu.cn

Ruby: f(a: 1, b: 2)
来源：http://ykt.mhx1999.top

C#:   f(a: 1, b: 2)
来源：http://jct.jqgfzy.top

[C05] 返回多个值
来源：http://xzn.tianlin.xyz

Py:   return a, b
来源：http://ucd.cheryme.top

PHP:  return [$a, $b];
来源：http://kcp.bbcook.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://cmw.dianchejie.cn

TS:   return { a, b };
来源：http://buj.yj20258.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xfy.zycfv.cn

Go:   return a, b
来源：http://bwc.fzhhl.top

Ruby: return a, b
来源：http://fvu.jinyuanbaomall.cn

C#:   return (a, b);              // ValueTuple
来源：http://ehh.hywenlv.cn

[C06] 匿名函数 / lambda
来源：http://mqv.kuanghao11.cn

Py:   square = lambda x: x * x
来源：http://qjd.dashuyun.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fov.iojbl.cn

JS:   const square = x => x * x;
来源：http://kaw.jyoumei.cn

TS:   const square = (x: number): number => x * x;
来源：http://chj.nwbrower.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ccn.jinqigfzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://ysc.wangdashe.top

Ruby: square = ->(x) { x * x }
来源：http://oml.hongshengwenyu.top

C#:   Func<int, int> square = x => x * x;
来源：http://sth.ctjpmb.com

[C07] 把函数作为参数传入
来源：http://zky.hesvh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cac.zhijiandao.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ekg.nwbrower.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gvj.zdbjq.cn

TS:   arr.map(String)
来源：http://cpu.fengsongda.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://egz.sjlbkw.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qcf.ehwqpu.com

Ruby: arr.map(&:upcase)
来源：http://wxy.hfpthk.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://vwd.redwolf501.top

[C08] 闭包
来源：http://mfx.hongshengwenyu.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://unn.iojbl.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tgh.zdbjq.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://obt.jinghuilouyu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wjt.pengpengdd.cyou

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://chh.gzhubu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://upq.nanxinkj.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sat.jianghu66.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kde.zhaomingkeji.xyz

[C09] 递归
来源：http://kwc.chenzaomai.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gsp.yj202588.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://srf.xingfuxueyuan.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zto.wangshuangyany.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://acv.nanxinkj.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jjd.hnqzz.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pmm.yanxiufei.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tyg.ybcxt.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cbk.xuanzx.com

[C10] 变量作用域
来源：http://qzr.yfazqb.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pbt.dashuyun.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bwx.jianghu66.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wrd.zdbjq.cn

TS:   同 JS
来源：http://cub.zdqjudy.top

Java: 方法内为块级作用域
来源：http://jcz.snrcjt.cn

Go:   花括号块级作用域
来源：http://wvt.ybcxt.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rpk.ppjwa.cn

C#:   块级作用域
来源：http://qui.hnxiangtu.top

[C11] 模块导入与导出
来源：http://wpf.hesvh.cn

Py:   from module import func
来源：http://lbx.kuanghao11.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kfb.xuetiantiany.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hfh.vqdsnc.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cfs.xinyue.icu

Java: import java.util.List;
来源：http://obm.fanxiaobao.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://iaz.uphjek.com

Ruby: require "json"; require_relative "./util"
来源：http://lgv.zhiwuduotai.top

C#:   using System.Text;
来源：http://wni.nwbrower.top

[C12] 立即执行函数 IIFE
来源：http://kko.yvedp.cn

Py:   (lambda: print("run"))()
来源：http://wkm.dianchejie.cn

PHP:  (function () { echo "run"; })();
来源：http://vck.zhengqikj.top

JS:   (() => { console.log("run"); })();
来源：http://efm.smart0.xyz

TS:   (() => { console.log("run"); })();
来源：http://cxj.meibo888.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yxe.redwolf501.top

Go:   func() { fmt.Println("run") }()
来源：http://dhe.sufxvd.cn

Ruby: -> { puts "run" }.call
来源：http://hfb.hongshengwenyu.top

C#:   // 无 IIFE：用静态构造函数
来源：http://cte.fzhhl.top

[C13] 类型声明 / 类型注解
来源：http://evb.sysykeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rml.bjfxy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cme.jinghuilouyu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mrw.nwbrower.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xrt.pycfn.com

Java: int add(int a, int b) { return a + b; }
来源：http://dhu.hnqzz.top

Go:   func add(a, b int) int
来源：http://cxa.nanxuanxn.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://giq.cdnleiting.top

C#:   int Add(int a, int b) => a + b;
来源：http://ltz.dianchejie.cn

[C14] 泛型函数
来源：http://qsy.xylfe.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lsr.9152youxi.cn

PHP:  // 无泛型
来源：http://dsl.ivvv.top

JS:   // 无泛型
来源：http://web.yj20258888.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://slq.cheryme.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mwk.fzhhl.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ezx.smart0.xyz

Ruby: # 无泛型
来源：http://ixb.shuidangran.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vrl.shanyushiyangkeji.top

[C15] 解构 / 展开参数
来源：http://obo.yj20258.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tkv.jianghu66.top

PHP:  [$a, $b] = $pair;
来源：http://byi.pengpengdd.cyou

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://flg.guowangkeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qmy.xuanzx.com

Java: // 无解构
来源：http://hzj.xuetiantiany.cn

Go:   // 无解构
来源：http://wgu.pengpengdd.cyou

Ruby: a, b = pair
来源：http://dmi.iojbl.cn

C#:   var (a, b) = pair;
来源：http://rht.zdqjudy.top

[C16] 函数 / 方法重载
来源：http://hmr.tianlin.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ayl.yongpay.top

PHP:  // 无重载
来源：http://rnp.jiagoushi.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://xyv.gzhubu.top

TS:   // 用联合类型或重载签名声明
来源：http://jog.jlsjyb.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gzo.fzhhl.top

Go:   // 无重载：用不同函数名
来源：http://cqr.jiagoushi.top

Ruby: # 无重载：靠动态参数
来源：http://hqk.aizwys.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rhp.iojbl.cn

================================================================================
来源：http://pbm.ybcxt.top

D. 数组 / 列表 / 集合
来源：http://kkq.dashuyun.cn

================================================================================
来源：http://alr.shuidangran.top

[D01] 创建数组 / 列表
来源：http://fja.9152youxi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jdc.yvedp.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tty.dashuyun.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ptd.bjfxy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://cxh.jiagoushi.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://smc.guannengcc.top

Go:   arr := []int{1, 2, 3}
来源：http://qyx.iojbl.cn

Ruby: arr = [1, 2, 3]
来源：http://svc.iojbl.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jbw.pengpengdd.cyou

[D02] 追加元素到末尾
来源：http://nvf.tarul.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pud.jqgfzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fdy.xuetiantiany.cn

JS:   arr.push(4);
来源：http://aze.wangdashe.top

TS:   arr.push(4);
来源：http://qpi.vehdjk.com

Java: list.add(4);
来源：http://vfc.tanke756.top

Go:   arr = append(arr, 4)
来源：http://pqj.52xcode.cn

Ruby: arr << 4; arr.push(5)
来源：http://qjx.cucudq.cn

C#:   list.Add(4);
来源：http://xcb.zhiwuduotai.top

[D03] 在指定位置插入元素
来源：http://boj.chenzaomai.com

Py:   arr.insert(0, 0)
来源：http://ajp.jinyuanbaomall.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://les.zhongyouzk.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ihw.shanyushiyangkeji.top

TS:   arr.splice(0, 0, 0);
来源：http://xjv.zhixingplan.top

Java: list.add(0, 0);
来源：http://scr.zhijiandao.cn

Go:   arr = append([]int{0}, arr...)
来源：http://iug.svipenyu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://osk.yanxiufei.cn

C#:   list.Insert(0, 0);
来源：http://nfv.gotoacloud.top

[D04] 删除元素
来源：http://utm.zhixingplan.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uug.iojbl.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nyq.pengpengdd.cyou

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bil.tian-w.cn

TS:   arr.splice(0, 1);
来源：http://nek.yj20258.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pqu.shanyushiyangtech.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wia.nanxinkj.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xaj.wangdashe.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kfz.hywenlv.cn

[D05] 访问与修改元素
来源：http://ovg.xuetiantiany.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://duc.cucudq.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hyr.jiagoushi.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gtf.jiagoushi.top

TS:   arr[0]; arr.at(-1);
来源：http://tch.fzhhl.top

Java: list.get(0); list.set(0, 9);
来源：http://hdd.fengsongda.top

Go:   arr[0]; arr[0] = 9
来源：http://zgw.xingfuxueyuan.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fzz.0kj1m.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://frr.aizwys.cn

[D06] 数组长度
来源：http://qvv.zhengqikj.top

Py:   len(arr)
来源：http://bmb.sjlbkw.cn

PHP:  count($arr);
来源：http://chj.yonumen.top

JS:   arr.length
来源：http://bli.zhiwuduotai.top

TS:   arr.length
来源：http://ycj.c1oappe.top

Java: list.size();
来源：http://klw.yongpay.top

Go:   len(arr)
来源：http://ynv.meibo888.top

Ruby: arr.length; arr.size
来源：http://wra.c1oappe.top

C#:   list.Count;
来源：http://rle.daria6918.cn

[D07] 切片 / 取子数组
来源：http://ymo.ydzc1.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wba.jinyuanbaomall.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xee.shanyushiyangtech.top

JS:   arr.slice(1, 4);
来源：http://igs.sweek.top

TS:   arr.slice(1, 4);
来源：http://goh.tanke756.top

Java: list.subList(1, 4);
来源：http://mkv.feifeiyinyue.top

Go:   arr[1:4]
来源：http://rzz.nanxinkj.top

Ruby: arr[1, 3]
来源：http://skx.jqgufenzy.top

C#:   list.GetRange(1, 3);
来源：http://akj.gogol.net.cn

[D08] 合并两个数组
来源：http://ixu.ydzc1.top

Py:   a + b;  a.extend(b)
来源：http://fve.yangfankeji.com

PHP:  array_merge($a, $b);
来源：http://rqb.guowangkeji.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ukr.hysaishi.cn

TS:   [...a, ...b];
来源：http://dml.zhengqikj.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://aql.xylfe.cn

Go:   append(a, b...)
来源：http://dxr.bjfxy.top

Ruby: a + b;  a.concat(b)
来源：http://ocn.hnqzz.top

C#:   a.Concat(b).ToList()
来源：http://oav.feifeiyinyue.top

[D09] 排序（升序）
来源：http://bnw.zdbjq.cn

Py:   sorted(arr);  arr.sort()
来源：http://shf.316326.xyz

PHP:  sort($arr);
来源：http://uzu.svipenyu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jhr.yfazqb.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://kka.sweek.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ctu.hammf.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://beo.zhixingplan.top

Ruby: arr.sort
来源：http://kcb.jinyuanbaomall.cn

C#:   list.Sort();
来源：http://wwp.shanyushiyangtech.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://yre.birdmap.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fno.pycfn.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qwr.9152youxi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://adl.shzxlz.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ejs.haohaochexian.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cbd.jianghu66.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hlv.cucudq.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gma.aizwys.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xbw.pycfn.com

[D11] 反转数组
来源：http://kdk.chenzaomai.com

Py:   arr[::-1];  arr.reverse()
来源：http://iln.meibo888.top

PHP:  array_reverse($arr);
来源：http://ofn.zhengqikj.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://med.xinyue.icu


<!-- 参考信息 -->