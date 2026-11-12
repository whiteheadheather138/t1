代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rte.kuanghao11.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pac.xziqi.cn

[B11] 生成数字序列 / 区间
来源：http://pzu.jyoumei.cn

Py:   list(range(0, 10, 2))
来源：http://pen.tianlin.xyz

PHP:  range(0, 10, 2);
来源：http://fwv.gzhubu.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zeh.jinqigfzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fcm.guannengcc.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blo.xuetiantiany.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yul.sweek.top

Ruby: (0...10).step(2).to_a
来源：http://ymg.jinyuanbaomall.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lej.wangshuangyany.cn

[B12] 跳出多层循环
来源：http://xpk.0kj1m.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://uye.ehwqpu.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://srl.chenlongwang.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://orr.yj20258888.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vtx.haohaochexian.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fdm.zycfv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uue.xuetiantiany.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mlt.aizwys.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hyl.nanxinkj.top

[B13] 判断是否为数字
来源：http://cfu.yonumen.top

Py:   isinstance(x, (int, float))
来源：http://oqg.nanxinkj.top

PHP:  is_numeric($x)
来源：http://yca.vehdjk.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qxs.0kj1m.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://guu.yuxming.cn

Java: x instanceof Number
来源：http://tui.xuetiantiany.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zoh.xuanzx.com

Ruby: x.is_a?(Numeric)
来源：http://jpd.aizwys.cn

C#:   x is int or double or decimal
来源：http://mym.bbcook.cn

[B14] 判断值是否在集合内
来源：http://isu.zdqjudy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hje.havefunace.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://upe.jianghu66.top

JS:   [1, 2, 3].includes(x)
来源：http://kcr.cashguo.top

TS:   [1, 2, 3].includes(x)
来源：http://rtu.vqdsnc.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://bug.ywan-chungtsiang.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ohh.ydjk.org.cn

Ruby: [1, 2, 3].include?(x)
来源：http://lel.yj20258888.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ndk.hcnkem.com

[B15] 布尔运算与取反
来源：http://tkq.gzhubu.top

Py:   a and b or not c
来源：http://ols.cashguo.top

PHP:  $a && $b || !$c
来源：http://vsk.shanyushiyangtech.top

JS:   a && b || !c
来源：http://rwn.xuanzx.com

TS:   a && b || !c
来源：http://gfc.xuetiantiany.cn

Java: a && b || !c
来源：http://mny.jlsjyb.cn

Go:   a && b || !c
来源：http://tlx.xuanzx.com

Ruby: a && b || !c
来源：http://moy.fktsv.cn

C#:   a && b || !c
来源：http://kpy.sufxvd.cn

[B16] 卫语句：不满足条件提前返回
来源：http://anb.ydzc1.top

Py:   if not data: return
来源：http://txm.yanxiufei.cn

PHP:  if (!$data) { return; }
来源：http://rqb.52xcode.cn

JS:   if (!data) return;
来源：http://jbu.wangdashe.top

TS:   if (!data) return;
来源：http://kfk.mhx1999.top

Java: if (data == null) return;
来源：http://xhr.nwbrower.top

Go:   if data == nil { return }
来源：http://zqs.dashuyun.cn

Ruby: return if data.nil?
来源：http://cbs.gotoacloud.top

C#:   if (data == null) return;
来源：http://qpm.andypj.xyz

================================================================================
来源：http://epx.guannengcc.top

C. 函数与作用域
来源：http://cgi.feifeiyinyue.top

================================================================================
来源：http://zek.zhongyouzk.top

[C01] 定义函数
来源：http://xoa.dashuyun.cn

Py:   def add(a, b): return a + b
来源：http://qiu.yongpay.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wxh.quarkkingdee.top

JS:   function add(a, b) { return a + b; }
来源：http://epu.yj20258888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cva.jinqigufen.top

Java: static int add(int a, int b) { return a + b; }
来源：http://zrr.tarul.cn

Go:   func add(a, b int) int { return a + b }
来源：http://pca.sufxvd.cn

Ruby: def add(a, b); a + b; end
来源：http://ezk.xziqi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://olg.xziqi.cn

[C02] 默认参数
来源：http://cng.cheryme.top

Py:   def greet(name="World"): return name
来源：http://jtm.hfpthk.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hlt.hysaishi.cn

JS:   function greet(name = "World") { return name; }
来源：http://nav.bjfxy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://mer.birdmap.top

Java: // 无默认参数：方法重载或 Optional
来源：http://apx.zhaomingkeji.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ddu.cqqwz.cn

Ruby: def greet(name = "World") = name
来源：http://fuy.hnxiangtu.top

C#:   string Greet(string name = "World") => name;
来源：http://ujl.aizwys.cn

[C03] 可变参数
来源：http://wfs.cucudq.cn

Py:   def total(*args): return sum(args)
来源：http://ron.guannengcc.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ueh.iojbl.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dyi.kuanghao11.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vdk.xingfuxueyuan.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://whs.xuetiantiany.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pek.guowangkeji.top

Ruby: def total(*nums); nums.sum; end
来源：http://als.iojbl.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nrf.jqgufenzy.top

[C04] 命名参数 / 关键字参数
来源：http://ldz.yfazqb.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qhc.yuxming.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vud.fzhhl.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gpn.jqgfzy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ruy.zdbjq.cn

Java: // 无：用 Builder 模式或 record
来源：http://yzx.zdbjq.cn

Go:   // 无：用配置结构体参数
来源：http://pjp.jinyuanbaomall.cn

Ruby: f(a: 1, b: 2)
来源：http://nrx.guannengcc.top

C#:   f(a: 1, b: 2)
来源：http://dtj.yj20258.top

[C05] 返回多个值
来源：http://zgy.bbcook.cn

Py:   return a, b
来源：http://eer.tanke756.top

PHP:  return [$a, $b];
来源：http://kry.cheryme.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://rsk.zhijiandao.cn

TS:   return { a, b };
来源：http://qrz.yangfankeji.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pfc.svipenyu.cn

Go:   return a, b
来源：http://pkd.jianghu66.top

Ruby: return a, b
来源：http://sbg.zhiwuduotai.top

C#:   return (a, b);              // ValueTuple
来源：http://hxi.feifeiyinyue.top

[C06] 匿名函数 / lambda
来源：http://yhy.ctjpmb.com

Py:   square = lambda x: x * x
来源：http://lml.zhiwuduotai.top

PHP:  $square = fn($x) => $x * $x;
来源：http://blv.epnwcf.com

JS:   const square = x => x * x;
来源：http://pje.xinyue.icu

TS:   const square = (x: number): number => x * x;
来源：http://lkr.gogol.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cey.fengsongda.top

Go:   sq := func(x int) int { return x * x }
来源：http://dre.xziqi.cn

Ruby: square = ->(x) { x * x }
来源：http://vdr.gotoacloud.top

C#:   Func<int, int> square = x => x * x;
来源：http://plt.havefunace.top

[C07] 把函数作为参数传入
来源：http://kwg.hywenlv.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://iuh.ctjpmb.com

PHP:  array_map("strtoupper", $arr);
来源：http://hra.hcnkem.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mvc.xingfuxueyuan.xyz

TS:   arr.map(String)
来源：http://rwq.zhengqikj.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wwc.vehdjk.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://plf.vqdsnc.cn

Ruby: arr.map(&:upcase)
来源：http://iti.jinyuanbaomall.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://zje.guannengcc.top

[C08] 闭包
来源：http://egz.cqqwz.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rjk.0kj1m.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vgk.0kj1m.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rts.zdqjudy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qsl.mhx1999.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://isb.hammf.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xmo.meibo888.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sep.sysykeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hql.52xcode.cn

[C09] 递归
来源：http://mkl.wangdashe.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ogk.zhiwuduotai.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ecs.iojbl.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qak.epnwcf.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ldn.sysykeji.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qig.zhiwuduotai.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ayl.ppjwa.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://djg.pycfn.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wpk.hammf.cn

[C10] 变量作用域
来源：http://tfu.hfpthk.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gwx.redwolf501.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dmo.yueranfly.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zfx.hysaishi.cn

TS:   同 JS
来源：http://dnk.pengpengdd.cyou

Java: 方法内为块级作用域
来源：http://lzw.cdnleiting.top

Go:   花括号块级作用域
来源：http://igx.gogol.net.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://muy.aibaodan.cn

C#:   块级作用域
来源：http://qsi.ydjk.org.cn

[C11] 模块导入与导出
来源：http://qad.sjlbkw.cn

Py:   from module import func
来源：http://nra.gzhubu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://otb.svipenyu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://eie.sweek.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://myb.yj202588.top

Java: import java.util.List;
来源：http://oar.fengsongda.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ixd.mhx1999.top

Ruby: require "json"; require_relative "./util"
来源：http://ejp.aizwys.cn

C#:   using System.Text;
来源：http://azk.jinyuanbaomall.cn

[C12] 立即执行函数 IIFE
来源：http://ayn.guowangkeji.top

Py:   (lambda: print("run"))()
来源：http://off.hysaishi.cn

PHP:  (function () { echo "run"; })();
来源：http://kxf.snrcjt.cn

JS:   (() => { console.log("run"); })();
来源：http://chv.nanxuanxn.top

TS:   (() => { console.log("run"); })();
来源：http://ume.zhixingplan.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://srs.quarkkingdee.top

Go:   func() { fmt.Println("run") }()
来源：http://urd.hfpthk.cn

Ruby: -> { puts "run" }.call
来源：http://epa.316326.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://sux.cheryme.top

[C13] 类型声明 / 类型注解
来源：http://eej.jinqigfzy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zvj.aibaodan.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wkc.quarkkingdee.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fbr.fanxiaobao.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cbb.nanxuanxn.top

Java: int add(int a, int b) { return a + b; }
来源：http://hnf.cashguo.top

Go:   func add(a, b int) int
来源：http://jdh.jqgufenzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fdh.52xcode.cn

C#:   int Add(int a, int b) => a + b;
来源：http://osa.vqdsnc.cn

[C14] 泛型函数
来源：http://ckw.xingfuxueyuan.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lhh.ydzc1.top

PHP:  // 无泛型
来源：http://eak.cqqwz.cn

JS:   // 无泛型
来源：http://eip.zycfv.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wwf.redwolf501.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://osj.guowangkeji.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://awk.zhixingplan.top

Ruby: # 无泛型
来源：http://jpr.nwbrower.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ans.zycfv.cn

[C15] 解构 / 展开参数
来源：http://wbx.xylfe.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lzv.aizwys.cn

PHP:  [$a, $b] = $pair;
来源：http://kqt.tanke756.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qyq.cashguo.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://feb.chenjidiqi.icu

Java: // 无解构
来源：http://kbi.yuxming.cn

Go:   // 无解构
来源：http://pxl.vqdsnc.cn

Ruby: a, b = pair
来源：http://bnm.vqdsnc.cn

C#:   var (a, b) = pair;
来源：http://mqo.ywan-chungtsiang.top

[C16] 函数 / 方法重载
来源：http://awp.yj202588.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vvy.sjlbkw.cn

PHP:  // 无重载
来源：http://jyz.yj20258.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ccf.bjfxy.top

TS:   // 用联合类型或重载签名声明
来源：http://pel.zhixingplan.top

Java: void f(int a) {}  void f(String a) {}
来源：http://exy.dianchejie.cn

Go:   // 无重载：用不同函数名
来源：http://jxd.hongshengwenyu.top

Ruby: # 无重载：靠动态参数
来源：http://ivz.hcnkem.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://xpi.jqgfzy.top

================================================================================
来源：http://upz.yj20258888.top

D. 数组 / 列表 / 集合
来源：http://nri.nwbrower.top

================================================================================
来源：http://fxn.zycfv.cn

[D01] 创建数组 / 列表
来源：http://egg.birdmap.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://gik.snrcjt.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://huy.xuanzx.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rfy.yj20258.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://gic.hongshengwenyu.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ldq.jinyuanbaomall.cn

Go:   arr := []int{1, 2, 3}
来源：http://fkh.cheryme.top

Ruby: arr = [1, 2, 3]
来源：http://ggo.yuxming.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fcj.cdnleiting.top

[D02] 追加元素到末尾
来源：http://vsb.sysykeji.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://iqc.52xcode.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cxp.fktsv.cn

JS:   arr.push(4);
来源：http://byx.kuanghao11.cn

TS:   arr.push(4);
来源：http://rzx.sxryk.cn

Java: list.add(4);
来源：http://xax.9152youxi.cn

Go:   arr = append(arr, 4)
来源：http://qbd.vqdsnc.cn

Ruby: arr << 4; arr.push(5)
来源：http://pvs.yonumen.top

C#:   list.Add(4);
来源：http://hgm.shangyingyoupin.top

[D03] 在指定位置插入元素
来源：http://kxf.tianlin.xyz

Py:   arr.insert(0, 0)
来源：http://tit.kuanghao11.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fzg.tianlin.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qja.tian-w.cn

TS:   arr.splice(0, 0, 0);
来源：http://skr.haohaochexian.top

Java: list.add(0, 0);
来源：http://aeg.ydjk.org.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pxz.nanxinkj.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bcw.redwolf501.top

C#:   list.Insert(0, 0);
来源：http://mib.zhiwuduotai.top

[D04] 删除元素
来源：http://qzx.pycfn.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mqt.kuanghao11.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xtx.hfpthk.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://onz.smart0.xyz

TS:   arr.splice(0, 1);
来源：http://gjg.daria6918.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jgl.zdqjudy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://eok.pengpengdd.cyou

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pmh.yj20258.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://euv.zycfv.cn

[D05] 访问与修改元素
来源：http://lqm.feifeiyinyue.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uqu.fktsv.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sac.wangdashe.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ltw.vehdjk.com

TS:   arr[0]; arr.at(-1);
来源：http://rev.fehbvm.com

Java: list.get(0); list.set(0, 9);
来源：http://hop.nanxuanxn.top

Go:   arr[0]; arr[0] = 9
来源：http://sig.tanke756.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://osq.nanxinkj.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://odp.fanxiaobao.xyz

[D06] 数组长度
来源：http://odz.jianghu66.top

Py:   len(arr)
来源：http://sie.cashguo.top

PHP:  count($arr);
来源：http://hnv.cdnleiting.top

JS:   arr.length
来源：http://smu.svipenyu.cn

TS:   arr.length
来源：http://wzd.hesvh.cn

Java: list.size();
来源：http://zra.birdmap.top

Go:   len(arr)
来源：http://num.jiagoushi.top

Ruby: arr.length; arr.size
来源：http://kgw.9152youxi.cn

C#:   list.Count;
来源：http://jkj.haohaochexian.top

[D07] 切片 / 取子数组
来源：http://xun.birdmap.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://emd.yj20258.top

PHP:  array_slice($arr, 1, 3);
来源：http://ogp.zhoulong.xyz

JS:   arr.slice(1, 4);
来源：http://ezg.hysaishi.cn

TS:   arr.slice(1, 4);
来源：http://ntr.nwbrower.top

Java: list.subList(1, 4);
来源：http://vck.zhijiandao.cn

Go:   arr[1:4]
来源：http://lao.ctjpmb.com

Ruby: arr[1, 3]
来源：http://yxa.gogol.net.cn

C#:   list.GetRange(1, 3);
来源：http://adc.sxryk.cn

[D08] 合并两个数组
来源：http://tcm.jinqigfzy.top

Py:   a + b;  a.extend(b)
来源：http://yuv.feifeiyinyue.top

PHP:  array_merge($a, $b);
来源：http://fcq.epnwcf.com

JS:   [...a, ...b];  a.concat(b);
来源：http://dyv.tarul.cn

TS:   [...a, ...b];
来源：http://pmb.jiagoushi.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kud.jinyuanbaomall.cn

Go:   append(a, b...)
来源：http://oxy.aizwys.cn

Ruby: a + b;  a.concat(b)
来源：http://hrf.shanyushiyangtech.top

C#:   a.Concat(b).ToList()
来源：http://tik.wangdashe.top

[D09] 排序（升序）
来源：http://kyh.hammf.cn

Py:   sorted(arr);  arr.sort()
来源：http://ycr.andypj.xyz

PHP:  sort($arr);
来源：http://ndt.9152youxi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uaj.yvedp.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xwi.wangshuangyany.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://lcb.yangfankeji.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sxb.hnxiangtu.top

Ruby: arr.sort
来源：http://hav.ctjpmb.com

C#:   list.Sort();
来源：http://hhb.jinghuilouyu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vme.jinyuanbaomall.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://znw.bjfxy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pjm.ydjk.org.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nga.ehwqpu.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oit.chenlongwang.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gdg.yj20258888.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uhf.tianlin.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://njy.nwbrower.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nyh.ywan-chungtsiang.top

[D11] 反转数组
来源：http://nrp.jyoumei.cn

Py:   arr[::-1];  arr.reverse()
来源：http://neg.hfpthk.cn

PHP:  array_reverse($arr);
来源：http://kte.sufxvd.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jrq.zhixingplan.top


<!-- 参考信息 -->