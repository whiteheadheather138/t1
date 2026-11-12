代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://riw.zhiwuduotai.top

[B10] 遍历同时拿索引
来源：http://irz.kuanghao11.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ira.yueranfly.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://oef.yueranfly.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://oqw.fzhhl.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dyi.cqqwz.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vqn.yonumen.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kow.mhx1999.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://aao.bbcook.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hdy.xylfe.cn

[B11] 生成数字序列 / 区间
来源：http://alc.zdqjudy.top

Py:   list(range(0, 10, 2))
来源：http://prv.ctjpmb.com

PHP:  range(0, 10, 2);
来源：http://szi.yonumen.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gss.yongpay.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://axn.epnwcf.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wao.yfazqb.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tnb.kuanghao11.cn

Ruby: (0...10).step(2).to_a
来源：http://rqd.gaohongyu789.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://abc.andypj.xyz

[B12] 跳出多层循环
来源：http://vtx.jianghu66.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://hji.shanyushiyangtech.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://xpo.meibo888.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qlk.pycfn.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nib.yfazqb.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mny.sjlbkw.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ann.jlsjyb.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kmt.tianlin.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fvj.sweek.top

[B13] 判断是否为数字
来源：http://cyv.chenlongwang.top

Py:   isinstance(x, (int, float))
来源：http://xkm.hfpthk.cn

PHP:  is_numeric($x)
来源：http://qrd.yvedp.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fui.chenlongwang.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xhx.meibo888.top

Java: x instanceof Number
来源：http://avt.tian-w.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nvo.ydjk.org.cn

Ruby: x.is_a?(Numeric)
来源：http://caf.fehbvm.com

C#:   x is int or double or decimal
来源：http://jij.redwolf501.top

[B14] 判断值是否在集合内
来源：http://dap.guannengcc.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lha.nanxuanxn.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sjx.bjfxy.top

JS:   [1, 2, 3].includes(x)
来源：http://iwr.ppjwa.cn

TS:   [1, 2, 3].includes(x)
来源：http://chy.sysykeji.top

Java: List.of(1, 2, 3).contains(x)
来源：http://fbs.haohaochexian.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tuf.xinyue.icu

Ruby: [1, 2, 3].include?(x)
来源：http://amt.hcnkem.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wpo.nanxuanxn.top

[B15] 布尔运算与取反
来源：http://ieq.guowangkeji.top

Py:   a and b or not c
来源：http://rxd.jiagoushi.top

PHP:  $a && $b || !$c
来源：http://tae.feifeiyinyue.top

JS:   a && b || !c
来源：http://eld.ydjk.org.cn

TS:   a && b || !c
来源：http://moz.yangfankeji.com

Java: a && b || !c
来源：http://zlz.xziqi.cn

Go:   a && b || !c
来源：http://fzr.yangfankeji.com

Ruby: a && b || !c
来源：http://fbq.yangfankeji.com

C#:   a && b || !c
来源：http://kzh.yj202588.top

[B16] 卫语句：不满足条件提前返回
来源：http://hta.bjfxy.top

Py:   if not data: return
来源：http://trw.bjfxy.top

PHP:  if (!$data) { return; }
来源：http://fcg.zhixingplan.top

JS:   if (!data) return;
来源：http://muj.xuetiantiany.cn

TS:   if (!data) return;
来源：http://dve.c1oappe.top

Java: if (data == null) return;
来源：http://ezu.xingfuxueyuan.xyz

Go:   if data == nil { return }
来源：http://ubo.yueranfly.top

Ruby: return if data.nil?
来源：http://mrb.ehwqpu.com

C#:   if (data == null) return;
来源：http://ixv.smart0.xyz

================================================================================
来源：http://dsu.jlsjyb.cn

C. 函数与作用域
来源：http://hej.haohaochexian.top

================================================================================
来源：http://zma.cqqwz.cn

[C01] 定义函数
来源：http://nkk.zhaomingkeji.xyz

Py:   def add(a, b): return a + b
来源：http://shy.ppjwa.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uor.andypj.xyz

JS:   function add(a, b) { return a + b; }
来源：http://xcq.sysykeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://faa.nanxuanxn.top

Java: static int add(int a, int b) { return a + b; }
来源：http://gzr.pycfn.com

Go:   func add(a, b int) int { return a + b }
来源：http://myb.jlsjyb.cn

Ruby: def add(a, b); a + b; end
来源：http://mza.daria6918.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ivo.guowangkeji.top

[C02] 默认参数
来源：http://tqx.hfpthk.cn

Py:   def greet(name="World"): return name
来源：http://llz.jqgfzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://imz.hywenlv.cn

JS:   function greet(name = "World") { return name; }
来源：http://ymk.chenzaomai.com

TS:   function greet(name: string = "World") { return name; }
来源：http://qqu.yongpay.top

Java: // 无默认参数：方法重载或 Optional
来源：http://iuw.daxiang520.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lft.bjfxy.top

Ruby: def greet(name = "World") = name
来源：http://igc.yueranfly.top

C#:   string Greet(string name = "World") => name;
来源：http://kkp.havefunace.top

[C03] 可变参数
来源：http://pdh.smart0.xyz

Py:   def total(*args): return sum(args)
来源：http://aex.yongpay.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://osr.yvedp.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wlx.tanke756.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://erv.yueranfly.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nuo.cqqwz.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://aoe.jyoumei.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qhi.daria6918.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://snq.dashuyun.cn

[C04] 命名参数 / 关键字参数
来源：http://mie.xuetiantiany.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ggb.hnqzz.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qlh.wangdashe.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kjn.vqdsnc.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vnr.9152youxi.cn

Java: // 无：用 Builder 模式或 record
来源：http://hhn.snrcjt.cn

Go:   // 无：用配置结构体参数
来源：http://fci.xziqi.cn

Ruby: f(a: 1, b: 2)
来源：http://aot.dashuyun.cn

C#:   f(a: 1, b: 2)
来源：http://xxy.wangdashe.top

[C05] 返回多个值
来源：http://xff.hnxiangtu.top

Py:   return a, b
来源：http://pmi.daxiang520.top

PHP:  return [$a, $b];
来源：http://guz.zhijiandao.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qwc.pengpengdd.cyou

TS:   return { a, b };
来源：http://rkt.hfpthk.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rdk.dianchejie.cn

Go:   return a, b
来源：http://lkw.jinqigfzy.top

Ruby: return a, b
来源：http://bbm.hfpthk.cn

C#:   return (a, b);              // ValueTuple
来源：http://uko.guowangkeji.top

[C06] 匿名函数 / lambda
来源：http://mnj.birdmap.top

Py:   square = lambda x: x * x
来源：http://dhq.nanxinkj.top

PHP:  $square = fn($x) => $x * $x;
来源：http://dyj.zhijiandao.cn

JS:   const square = x => x * x;
来源：http://jlz.316326.xyz

TS:   const square = (x: number): number => x * x;
来源：http://cul.316326.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://iuk.quarkkingdee.top

Go:   sq := func(x int) int { return x * x }
来源：http://pnp.cqqwz.cn

Ruby: square = ->(x) { x * x }
来源：http://xnu.yj20258888.top

C#:   Func<int, int> square = x => x * x;
来源：http://bur.shanyushiyangkeji.top

[C07] 把函数作为参数传入
来源：http://kmu.sysykeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://iqj.shanyushiyangtech.top

PHP:  array_map("strtoupper", $arr);
来源：http://gps.jlsjyb.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jqb.guowangkeji.top

TS:   arr.map(String)
来源：http://hlz.sjlbkw.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uxw.xylfe.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://luq.sxryk.cn

Ruby: arr.map(&:upcase)
来源：http://blc.gaohongyu789.top

C#:   arr.Select(s => s.ToUpper())
来源：http://xzx.yonumen.top

[C08] 闭包
来源：http://bgj.cheryme.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://swo.bbcook.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ffh.ppjwa.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://smb.mhx1999.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vyp.sysykeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://spa.zhijiandao.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jjz.zhixingplan.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uls.jianghu66.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jwv.uphjek.com

[C09] 递归
来源：http://hjz.hnxiangtu.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nhm.tianlin.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://esm.cucudq.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ody.hnqzz.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ows.aibaodan.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fpd.wangdashe.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kto.gogol.net.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qrs.yj202588.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vkt.mhx1999.top

[C10] 变量作用域
来源：http://xvs.quarkkingdee.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pjv.daria6918.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nhh.cqqwz.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ujr.sysykeji.top

TS:   同 JS
来源：http://cyw.dianchejie.cn

Java: 方法内为块级作用域
来源：http://kaf.xuetiantiany.cn

Go:   花括号块级作用域
来源：http://cde.pengpengdd.cyou

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tdm.yfazqb.com

C#:   块级作用域
来源：http://hhd.xylfe.cn

[C11] 模块导入与导出
来源：http://zog.dashuyun.cn

Py:   from module import func
来源：http://fbw.jinqigfzy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://nic.wangdashe.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://yev.yj20258.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tkv.yuxming.cn

Java: import java.util.List;
来源：http://snl.zdbjq.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gvn.aizwys.cn

Ruby: require "json"; require_relative "./util"
来源：http://lis.shangyingyoupin.top

C#:   using System.Text;
来源：http://yzd.sufxvd.cn

[C12] 立即执行函数 IIFE
来源：http://qrr.yj202588.top

Py:   (lambda: print("run"))()
来源：http://zzu.shangyingyoupin.top

PHP:  (function () { echo "run"; })();
来源：http://yqm.jinghuilouyu.cn

JS:   (() => { console.log("run"); })();
来源：http://cbk.sufxvd.cn

TS:   (() => { console.log("run"); })();
来源：http://kyh.zycfv.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ftb.xingfuxueyuan.xyz

Go:   func() { fmt.Println("run") }()
来源：http://rgh.wangdashe.top

Ruby: -> { puts "run" }.call
来源：http://zpb.yongpay.top

C#:   // 无 IIFE：用静态构造函数
来源：http://pfr.9152youxi.cn

[C13] 类型声明 / 类型注解
来源：http://swx.yanxiufei.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kpw.zhaomingkeji.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ypy.dashuyun.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://uax.zhiwuduotai.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sza.uphjek.com

Java: int add(int a, int b) { return a + b; }
来源：http://xgo.vehdjk.com

Go:   func add(a, b int) int
来源：http://ihe.shanyushiyangkeji.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://saf.dianchejie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mmb.dashuyun.cn

[C14] 泛型函数
来源：http://skd.wangshuangyany.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://upe.fengsongda.top

PHP:  // 无泛型
来源：http://iey.316326.xyz

JS:   // 无泛型
来源：http://nmn.tarul.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mpb.jiagoushi.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ayd.meibo888.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fnh.chenjidiqi.icu

Ruby: # 无泛型
来源：http://ybn.jinqigfzy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vxv.chenjidiqi.icu

[C15] 解构 / 展开参数
来源：http://xuw.sjlbkw.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://znb.cashguo.top

PHP:  [$a, $b] = $pair;
来源：http://cog.zhiwuduotai.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ypp.yj20258.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://adt.mhx1999.top

Java: // 无解构
来源：http://cgr.svipenyu.cn

Go:   // 无解构
来源：http://zzf.zhixingplan.top

Ruby: a, b = pair
来源：http://skr.meibo888.top

C#:   var (a, b) = pair;
来源：http://egk.zhixingplan.top

[C16] 函数 / 方法重载
来源：http://cym.jqgufenzy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xlg.shanyushiyangtech.top

PHP:  // 无重载
来源：http://oqw.feifeiyinyue.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://rzl.jiagoushi.top

TS:   // 用联合类型或重载签名声明
来源：http://zpy.xziqi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yte.pycfn.com

Go:   // 无重载：用不同函数名
来源：http://bkg.yvedp.cn

Ruby: # 无重载：靠动态参数
来源：http://elz.shanyushiyangkeji.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://odp.andypj.xyz

================================================================================
来源：http://idx.yuanzhike.top

D. 数组 / 列表 / 集合
来源：http://zfu.ctjpmb.com

================================================================================
来源：http://lmq.tanke756.top

[D01] 创建数组 / 列表
来源：http://pve.jiagoushi.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ual.jianghu66.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://frx.sufxvd.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uha.sufxvd.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hrb.smart0.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://utk.vehdjk.com

Go:   arr := []int{1, 2, 3}
来源：http://fcq.yvedp.cn

Ruby: arr = [1, 2, 3]
来源：http://agv.yangfankeji.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://epa.shangyingyoupin.top

[D02] 追加元素到末尾
来源：http://sig.zhengqikj.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jax.ydjk.org.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wbg.haohaochexian.top

JS:   arr.push(4);
来源：http://guv.cqqwz.cn

TS:   arr.push(4);
来源：http://goe.c1oappe.top

Java: list.add(4);
来源：http://vgm.ydzc1.top

Go:   arr = append(arr, 4)
来源：http://nxl.vehdjk.com

Ruby: arr << 4; arr.push(5)
来源：http://cak.zdbjq.cn

C#:   list.Add(4);
来源：http://hbd.redwolf501.top

[D03] 在指定位置插入元素
来源：http://nfs.aibaodan.cn

Py:   arr.insert(0, 0)
来源：http://vpb.ywan-chungtsiang.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hfd.sufxvd.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tmd.sweek.top

TS:   arr.splice(0, 0, 0);
来源：http://mqh.hammf.cn

Java: list.add(0, 0);
来源：http://lks.ctjpmb.com

Go:   arr = append([]int{0}, arr...)
来源：http://umd.haohaochexian.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://btj.shuidangran.top

C#:   list.Insert(0, 0);
来源：http://tsa.ctjpmb.com

[D04] 删除元素
来源：http://iac.jinghuilouyu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://brn.ydzc1.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vrl.cheryme.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://can.xingfuxueyuan.xyz

TS:   arr.splice(0, 1);
来源：http://luc.havefunace.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fpd.yanxiufei.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://iip.sjlbkw.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rhp.iojbl.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://roa.hnxiangtu.top

[D05] 访问与修改元素
来源：http://veu.hfpthk.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cry.tianlin.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ntg.meibo888.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://apn.xylfe.cn

TS:   arr[0]; arr.at(-1);
来源：http://imo.xuanzx.com

Java: list.get(0); list.set(0, 9);
来源：http://ebw.zhongyouzk.top

Go:   arr[0]; arr[0] = 9
来源：http://mfb.hysaishi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qdh.andypj.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yvi.cdnleiting.top

[D06] 数组长度
来源：http://hzo.xylfe.cn

Py:   len(arr)
来源：http://exd.fanxiaobao.xyz

PHP:  count($arr);
来源：http://gur.daxiang520.top

JS:   arr.length
来源：http://umx.dashuyun.cn

TS:   arr.length
来源：http://nje.zdqjudy.top

Java: list.size();
来源：http://xtk.zhoulong.xyz

Go:   len(arr)
来源：http://qrw.jinqigufen.top

Ruby: arr.length; arr.size
来源：http://mai.epnwcf.com

C#:   list.Count;
来源：http://bai.tarul.cn

[D07] 切片 / 取子数组
来源：http://rgo.uphjek.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tgj.uphjek.com

PHP:  array_slice($arr, 1, 3);
来源：http://lgx.zhengqikj.top

JS:   arr.slice(1, 4);
来源：http://omf.zhengqikj.top

TS:   arr.slice(1, 4);
来源：http://vht.gaohongyu789.top

Java: list.subList(1, 4);
来源：http://vmp.shanyushiyangkeji.top

Go:   arr[1:4]
来源：http://mlz.gzhubu.top

Ruby: arr[1, 3]
来源：http://bhz.xinyue.icu

C#:   list.GetRange(1, 3);
来源：http://qxt.zdbjq.cn

[D08] 合并两个数组
来源：http://zkg.316326.xyz

Py:   a + b;  a.extend(b)
来源：http://uqu.tarul.cn

PHP:  array_merge($a, $b);
来源：http://lkr.sxryk.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://dib.jianghu66.top

TS:   [...a, ...b];
来源：http://jsw.hfpthk.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wnf.yj20258888.top

Go:   append(a, b...)
来源：http://duz.gaohongyu789.top

Ruby: a + b;  a.concat(b)
来源：http://fyd.havefunace.top

C#:   a.Concat(b).ToList()
来源：http://ilh.zhixingplan.top

[D09] 排序（升序）
来源：http://wfo.yfazqb.com

Py:   sorted(arr);  arr.sort()
来源：http://rkd.c1oappe.top

PHP:  sort($arr);
来源：http://pry.xingfuxueyuan.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ugn.zhiwuduotai.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://onh.yongpay.top

Java: Collections.sort(list);  list.sort(null);
来源：http://pii.yvedp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yvf.c1oappe.top

Ruby: arr.sort
来源：http://jjd.nanxinkj.top

C#:   list.Sort();
来源：http://zrs.jqgfzy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://isr.hesvh.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gfm.ybcxt.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ejf.fanxiaobao.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pgs.daxiang520.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fab.nwbrower.top


<!-- 参考信息 -->