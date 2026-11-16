代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nhv.yj20258.top

Ruby: while i < 10; i += 1; end
来源：http://xbk.epnwcf.com

C#:   while (i < 10) { i++; }
来源：http://pnl.svipenyu.cn

[B08] do-while（至少执行一次）
来源：http://vkz.gaohongyu789.top

Py:   # 无 do-while：用 while True + break
来源：http://iah.9152youxi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://hmu.yuanzhike.top

JS:   do { i++; } while (i < 10);
来源：http://lww.ybcxt.top

TS:   do { i++; } while (i < 10);
来源：http://zvx.wangdashe.top

Java: do { i++; } while (i < 10);
来源：http://zrt.yanxiufei.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bwg.guowangkeji.top

Ruby: begin; i += 1; end while i < 10
来源：http://nnp.snrcjt.cn

C#:   do { i++; } while (i < 10);
来源：http://qtb.hongshengwenyu.top

[B09] break 与 continue
来源：http://wns.jinqigufen.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nob.chenlongwang.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uor.ydjk.org.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pqq.ppjwa.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rrx.0kj1m.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ici.kuanghao11.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gtj.chenlongwang.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gxj.9152youxi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hcq.jinghuilouyu.cn

[B10] 遍历同时拿索引
来源：http://vpw.zycfv.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vdp.xinyue.icu

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xto.xylfe.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://esx.shanyushiyangtech.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bir.pycfn.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wzg.sxryk.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xhr.aibaodan.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://iba.daxiang520.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hjh.cheryme.top

[B11] 生成数字序列 / 区间
来源：http://pft.yonumen.top

Py:   list(range(0, 10, 2))
来源：http://oqh.pengpengdd.cyou

PHP:  range(0, 10, 2);
来源：http://sem.chenlongwang.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mja.yueranfly.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qsc.chenlongwang.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bjx.meibo888.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cae.tarul.cn

Ruby: (0...10).step(2).to_a
来源：http://zqb.cucudq.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cmb.gotoacloud.top

[B12] 跳出多层循环
来源：http://frt.xuetiantiany.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://drd.hnqzz.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://tfm.ydjk.org.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zpw.jqgfzy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ylb.yangfankeji.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rdu.yj202588.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://crl.bjfxy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qpf.chenjidiqi.icu

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nhr.fehbvm.com

[B13] 判断是否为数字
来源：http://bfa.jqgfzy.top

Py:   isinstance(x, (int, float))
来源：http://nzm.aizwys.cn

PHP:  is_numeric($x)
来源：http://bvj.haohaochexian.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cwx.feifeiyinyue.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qlf.dianchejie.cn

Java: x instanceof Number
来源：http://dsy.tarul.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://iuz.cashguo.top

Ruby: x.is_a?(Numeric)
来源：http://eak.birdmap.top

C#:   x is int or double or decimal
来源：http://ugn.tianlin.xyz

[B14] 判断值是否在集合内
来源：http://ngv.ybcxt.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lev.zycfv.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tkp.sxryk.cn

JS:   [1, 2, 3].includes(x)
来源：http://dqp.ivvv.top

TS:   [1, 2, 3].includes(x)
来源：http://yas.dianchejie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://jzy.vehdjk.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lbg.ydjk.org.cn

Ruby: [1, 2, 3].include?(x)
来源：http://hhv.shangyingyoupin.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lwm.chenjidiqi.icu

[B15] 布尔运算与取反
来源：http://qcz.jqgufenzy.top

Py:   a and b or not c
来源：http://rge.pengpengdd.cyou

PHP:  $a && $b || !$c
来源：http://fim.xuetiantiany.cn

JS:   a && b || !c
来源：http://alp.fanxiaobao.xyz

TS:   a && b || !c
来源：http://qgm.nwbrower.top

Java: a && b || !c
来源：http://mwq.fzhhl.top

Go:   a && b || !c
来源：http://bqe.shzxlz.cn

Ruby: a && b || !c
来源：http://gbg.svipenyu.cn

C#:   a && b || !c
来源：http://bmh.cucudq.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ics.shanyushiyangtech.top

Py:   if not data: return
来源：http://bhp.pycfn.com

PHP:  if (!$data) { return; }
来源：http://jfb.wangdashe.top

JS:   if (!data) return;
来源：http://obs.feifeiyinyue.top

TS:   if (!data) return;
来源：http://itp.epnwcf.com

Java: if (data == null) return;
来源：http://xvf.yangfankeji.com

Go:   if data == nil { return }
来源：http://vja.9152youxi.cn

Ruby: return if data.nil?
来源：http://brp.jiagoushi.top

C#:   if (data == null) return;
来源：http://mdz.jqgufenzy.top

================================================================================
来源：http://iig.zdqjudy.top

C. 函数与作用域
来源：http://zou.bjfxy.top

================================================================================
来源：http://vmi.iojbl.cn

[C01] 定义函数
来源：http://nnp.yanxiufei.cn

Py:   def add(a, b): return a + b
来源：http://vkg.jlsjyb.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mph.andypj.xyz

JS:   function add(a, b) { return a + b; }
来源：http://jbp.sufxvd.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://diz.yfazqb.com

Java: static int add(int a, int b) { return a + b; }
来源：http://bhw.xingfuxueyuan.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://vvd.feifeiyinyue.top

Ruby: def add(a, b); a + b; end
来源：http://tio.xinyue.icu

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cei.ybcxt.top

[C02] 默认参数
来源：http://tno.guannengcc.top

Py:   def greet(name="World"): return name
来源：http://oqs.bjfxy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://qug.hywenlv.cn

JS:   function greet(name = "World") { return name; }
来源：http://ivs.jinqigufen.top

TS:   function greet(name: string = "World") { return name; }
来源：http://bhu.haohaochexian.top

Java: // 无默认参数：方法重载或 Optional
来源：http://knm.tianlin.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://flb.hnxiangtu.top

Ruby: def greet(name = "World") = name
来源：http://rry.jiagoushi.top

C#:   string Greet(string name = "World") => name;
来源：http://ert.hfpthk.cn

[C03] 可变参数
来源：http://mwu.fktsv.cn

Py:   def total(*args): return sum(args)
来源：http://wib.dianchejie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mzj.daria6918.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ool.316326.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://erq.xuanzx.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mhg.meibo888.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yrx.zhaomingkeji.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://tru.yj20258888.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qcc.ybcxt.top

[C04] 命名参数 / 关键字参数
来源：http://phm.cashguo.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://suq.wangdashe.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mag.hfpthk.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ryo.zhaomingkeji.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uqb.ybcxt.top

Java: // 无：用 Builder 模式或 record
来源：http://emt.chenlongwang.top

Go:   // 无：用配置结构体参数
来源：http://zwj.pengpengdd.cyou

Ruby: f(a: 1, b: 2)
来源：http://fiy.gogol.net.cn

C#:   f(a: 1, b: 2)
来源：http://wny.zdqjudy.top

[C05] 返回多个值
来源：http://wbo.iojbl.cn

Py:   return a, b
来源：http://auv.ivvv.top

PHP:  return [$a, $b];
来源：http://leo.chenzaomai.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://bpj.yanxiufei.cn

TS:   return { a, b };
来源：http://uyf.jinyuanbaomall.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zbh.vqdsnc.cn

Go:   return a, b
来源：http://evq.cdnleiting.top

Ruby: return a, b
来源：http://fql.jiagoushi.top

C#:   return (a, b);              // ValueTuple
来源：http://asm.iojbl.cn

[C06] 匿名函数 / lambda
来源：http://sxg.yangfankeji.com

Py:   square = lambda x: x * x
来源：http://zaf.bbcook.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://nhv.cqqwz.cn

JS:   const square = x => x * x;
来源：http://kug.haohaochexian.top

TS:   const square = (x: number): number => x * x;
来源：http://hdp.daria6918.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qqd.zhijiandao.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ecm.fzhhl.top

Ruby: square = ->(x) { x * x }
来源：http://jnz.jlsjyb.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wvz.mhx1999.top

[C07] 把函数作为参数传入
来源：http://omn.dashuyun.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lso.yueranfly.top

PHP:  array_map("strtoupper", $arr);
来源：http://ewl.hcnkem.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tqz.xylfe.cn

TS:   arr.map(String)
来源：http://drl.guowangkeji.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hgr.yanxiufei.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rqx.gaohongyu789.top

Ruby: arr.map(&:upcase)
来源：http://yms.0kj1m.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wzd.sysykeji.top

[C08] 闭包
来源：http://fsw.52xcode.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ovk.mhx1999.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://edw.fzhhl.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kko.chenjidiqi.icu

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cri.guannengcc.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sid.guowangkeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pcu.yj202588.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kjj.fehbvm.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cfg.jianghu66.top

[C09] 递归
来源：http://msn.jlsjyb.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lky.yueranfly.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://llf.zdqjudy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uqf.shanyushiyangkeji.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bgb.vehdjk.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ifi.jqgufenzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jdc.tanke756.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mob.yangfankeji.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kqo.xylfe.cn

[C10] 变量作用域
来源：http://otw.shangyingyoupin.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mte.hcnkem.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://skt.haohaochexian.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kwg.fanxiaobao.xyz

TS:   同 JS
来源：http://hol.tanke756.top

Java: 方法内为块级作用域
来源：http://bgv.fktsv.cn

Go:   花括号块级作用域
来源：http://ppy.ivvv.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jst.jinqigufen.top

C#:   块级作用域
来源：http://idk.aizwys.cn

[C11] 模块导入与导出
来源：http://xir.yueranfly.top

Py:   from module import func
来源：http://tdo.hywenlv.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://oup.xingfuxueyuan.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://iuv.nwbrower.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://beu.xuetiantiany.cn

Java: import java.util.List;
来源：http://vyo.gaohongyu789.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bdo.cucudq.cn

Ruby: require "json"; require_relative "./util"
来源：http://kpw.dianchejie.cn

C#:   using System.Text;
来源：http://nsn.feifeiyinyue.top

[C12] 立即执行函数 IIFE
来源：http://alx.shuidangran.top

Py:   (lambda: print("run"))()
来源：http://hav.gaohongyu789.top

PHP:  (function () { echo "run"; })();
来源：http://com.316326.xyz

JS:   (() => { console.log("run"); })();
来源：http://kbn.snrcjt.cn

TS:   (() => { console.log("run"); })();
来源：http://juf.redwolf501.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kfw.hywenlv.cn

Go:   func() { fmt.Println("run") }()
来源：http://tsz.sufxvd.cn

Ruby: -> { puts "run" }.call
来源：http://ymo.jinghuilouyu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pck.ehwqpu.com

[C13] 类型声明 / 类型注解
来源：http://upi.gogol.net.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dfj.aizwys.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tfv.zhiwuduotai.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lpt.jinqigufen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bvo.iojbl.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mtu.yj20258.top

Go:   func add(a, b int) int
来源：http://viy.zhoulong.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wzp.redwolf501.top

C#:   int Add(int a, int b) => a + b;
来源：http://lcz.yangfankeji.com

[C14] 泛型函数
来源：http://qtg.shzxlz.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uou.zdbjq.cn

PHP:  // 无泛型
来源：http://jvp.cashguo.top

JS:   // 无泛型
来源：http://xuv.shangyingyoupin.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qhs.zhaomingkeji.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nfg.ybcxt.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pdv.yj20258888.top

Ruby: # 无泛型
来源：http://gvv.jinqigufen.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bkh.sysykeji.top

[C15] 解构 / 展开参数
来源：http://fln.hongshengwenyu.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yrr.zhongyouzk.top

PHP:  [$a, $b] = $pair;
来源：http://jli.hesvh.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://puy.yvedp.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ekc.ybcxt.top

Java: // 无解构
来源：http://aod.iojbl.cn

Go:   // 无解构
来源：http://dbc.yvedp.cn

Ruby: a, b = pair
来源：http://hiq.sjlbkw.cn

C#:   var (a, b) = pair;
来源：http://yxb.yonumen.top

[C16] 函数 / 方法重载
来源：http://dvt.andypj.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wdj.bbcook.cn

PHP:  // 无重载
来源：http://sva.zhaomingkeji.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://ied.yanxiufei.cn

TS:   // 用联合类型或重载签名声明
来源：http://llc.gaohongyu789.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ttb.tian-w.cn

Go:   // 无重载：用不同函数名
来源：http://brq.zhijiandao.cn

Ruby: # 无重载：靠动态参数
来源：http://izz.dianchejie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rlj.xylfe.cn

================================================================================
来源：http://cdy.ydzc1.top

D. 数组 / 列表 / 集合
来源：http://cpc.quarkkingdee.top

================================================================================
来源：http://jkn.jianghu66.top

[D01] 创建数组 / 列表
来源：http://bvi.zdbjq.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://cgw.cdnleiting.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bjm.c1oappe.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pwa.yanxiufei.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://uep.zhaomingkeji.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://obs.cqqwz.cn

Go:   arr := []int{1, 2, 3}
来源：http://zgc.havefunace.top

Ruby: arr = [1, 2, 3]
来源：http://lrz.zhongyouzk.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xxv.hongshengwenyu.top

[D02] 追加元素到末尾
来源：http://rlb.hammf.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gvj.xingfuxueyuan.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xlw.hammf.cn

JS:   arr.push(4);
来源：http://spy.vqdsnc.cn

TS:   arr.push(4);
来源：http://asg.shzxlz.cn

Java: list.add(4);
来源：http://qwt.xziqi.cn

Go:   arr = append(arr, 4)
来源：http://qrz.52xcode.cn

Ruby: arr << 4; arr.push(5)
来源：http://qmi.hfpthk.cn

C#:   list.Add(4);
来源：http://xnv.sufxvd.cn

[D03] 在指定位置插入元素
来源：http://jam.yongpay.top

Py:   arr.insert(0, 0)
来源：http://wez.yuxming.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qbx.jinqigfzy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cqi.snrcjt.cn

TS:   arr.splice(0, 0, 0);
来源：http://urg.yanxiufei.cn

Java: list.add(0, 0);
来源：http://fyi.zhixingplan.top

Go:   arr = append([]int{0}, arr...)
来源：http://wfp.yonumen.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gsz.jyoumei.cn

C#:   list.Insert(0, 0);
来源：http://dqs.cdnleiting.top

[D04] 删除元素
来源：http://hyo.xingfuxueyuan.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fot.9152youxi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dgs.ppjwa.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xob.vehdjk.com

TS:   arr.splice(0, 1);
来源：http://jlj.sxryk.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sic.smart0.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ifl.chenzaomai.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rzn.yongpay.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tpm.yj20258.top

[D05] 访问与修改元素
来源：http://udi.chenjidiqi.icu

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zdq.cucudq.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bok.chenzaomai.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zec.shanyushiyangkeji.top

TS:   arr[0]; arr.at(-1);
来源：http://tes.pycfn.com

Java: list.get(0); list.set(0, 9);
来源：http://oph.bbcook.cn

Go:   arr[0]; arr[0] = 9
来源：http://zdd.havefunace.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://epu.zhengqikj.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gxy.shzxlz.cn

[D06] 数组长度
来源：http://bed.tianlin.xyz

Py:   len(arr)
来源：http://wgp.ppjwa.cn

PHP:  count($arr);
来源：http://opj.haohaochexian.top

JS:   arr.length
来源：http://tmd.hnqzz.top

TS:   arr.length
来源：http://xnx.yonumen.top

Java: list.size();
来源：http://ili.quarkkingdee.top

Go:   len(arr)
来源：http://tst.kuanghao11.cn

Ruby: arr.length; arr.size
来源：http://wwd.yueranfly.top

C#:   list.Count;
来源：http://yzt.fehbvm.com

[D07] 切片 / 取子数组
来源：http://xhd.bbcook.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://oxr.jqgufenzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://yfn.nanxinkj.top

JS:   arr.slice(1, 4);
来源：http://pxw.ehwqpu.com

TS:   arr.slice(1, 4);
来源：http://iad.xuanzx.com

Java: list.subList(1, 4);
来源：http://snu.9152youxi.cn

Go:   arr[1:4]
来源：http://rzq.zhijiandao.cn

Ruby: arr[1, 3]
来源：http://hkm.bbcook.cn

C#:   list.GetRange(1, 3);
来源：http://ogt.shanyushiyangtech.top

[D08] 合并两个数组
来源：http://nof.hysaishi.cn

Py:   a + b;  a.extend(b)
来源：http://dsd.shzxlz.cn

PHP:  array_merge($a, $b);
来源：http://err.zhengqikj.top


<!-- 参考信息 -->