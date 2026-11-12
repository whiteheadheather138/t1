代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://krb.cucudq.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://btg.yj202588.top

Ruby: begin; i += 1; end while i < 10
来源：http://wdl.jyoumei.cn

C#:   do { i++; } while (i < 10);
来源：http://krj.wangdashe.top

[B09] break 与 continue
来源：http://tlq.gogol.net.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rik.xuetiantiany.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://auo.mhx1999.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://liv.iojbl.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zzl.gaohongyu789.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rnl.aizwys.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gsg.dashuyun.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mfj.smart0.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://flg.hammf.cn

[B10] 遍历同时拿索引
来源：http://qht.chenlongwang.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://prq.ctjpmb.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lnm.xinyue.icu

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lks.hysaishi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lkq.nwbrower.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://odw.316326.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lhl.nwbrower.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pna.daria6918.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zgv.andypj.xyz

[B11] 生成数字序列 / 区间
来源：http://iha.aibaodan.cn

Py:   list(range(0, 10, 2))
来源：http://jjq.aibaodan.cn

PHP:  range(0, 10, 2);
来源：http://alg.hongshengwenyu.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mxs.ctjpmb.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://via.yangfankeji.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ovv.hnxiangtu.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://myg.yvedp.cn

Ruby: (0...10).step(2).to_a
来源：http://ndy.tian-w.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qbc.svipenyu.cn

[B12] 跳出多层循环
来源：http://yix.zycfv.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://oyg.hcnkem.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://fdi.fehbvm.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://deh.cashguo.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://uqz.chenjidiqi.icu

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ntf.sweek.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://eps.zhijiandao.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bfn.jiagoushi.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://udg.chenlongwang.top

[B13] 判断是否为数字
来源：http://huk.smart0.xyz

Py:   isinstance(x, (int, float))
来源：http://mxu.andypj.xyz

PHP:  is_numeric($x)
来源：http://nwu.zhijiandao.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nvt.uphjek.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nhg.vehdjk.com

Java: x instanceof Number
来源：http://ftq.nanxinkj.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ktm.gzhubu.top

Ruby: x.is_a?(Numeric)
来源：http://lpf.gotoacloud.top

C#:   x is int or double or decimal
来源：http://bbg.zhengqikj.top

[B14] 判断值是否在集合内
来源：http://nma.hfpthk.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vmc.svipenyu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bhp.ydjk.org.cn

JS:   [1, 2, 3].includes(x)
来源：http://ytl.fanxiaobao.xyz

TS:   [1, 2, 3].includes(x)
来源：http://gqs.zhongyouzk.top

Java: List.of(1, 2, 3).contains(x)
来源：http://hos.yanxiufei.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jsu.uphjek.com

Ruby: [1, 2, 3].include?(x)
来源：http://aek.yueranfly.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tmz.ybcxt.top

[B15] 布尔运算与取反
来源：http://ouc.jinghuilouyu.cn

Py:   a and b or not c
来源：http://and.bbcook.cn

PHP:  $a && $b || !$c
来源：http://tfa.zhengqikj.top

JS:   a && b || !c
来源：http://sgc.cdnleiting.top

TS:   a && b || !c
来源：http://adw.xuetiantiany.cn

Java: a && b || !c
来源：http://gxa.hysaishi.cn

Go:   a && b || !c
来源：http://osv.gotoacloud.top

Ruby: a && b || !c
来源：http://dii.chenzaomai.com

C#:   a && b || !c
来源：http://xhl.ydjk.org.cn

[B16] 卫语句：不满足条件提前返回
来源：http://nwa.zhixingplan.top

Py:   if not data: return
来源：http://qsi.chenlongwang.top

PHP:  if (!$data) { return; }
来源：http://jqy.hesvh.cn

JS:   if (!data) return;
来源：http://wwc.nanxuanxn.top

TS:   if (!data) return;
来源：http://otw.cucudq.cn

Java: if (data == null) return;
来源：http://uzr.xinyue.icu

Go:   if data == nil { return }
来源：http://jls.feifeiyinyue.top

Ruby: return if data.nil?
来源：http://fgk.redwolf501.top

C#:   if (data == null) return;
来源：http://zal.sysykeji.top

================================================================================
来源：http://ubg.zhixingplan.top

C. 函数与作用域
来源：http://vmw.yvedp.cn

================================================================================
来源：http://hir.xylfe.cn

[C01] 定义函数
来源：http://xmp.fanxiaobao.xyz

Py:   def add(a, b): return a + b
来源：http://dxn.hfpthk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://glu.yanxiufei.cn

JS:   function add(a, b) { return a + b; }
来源：http://eei.zdqjudy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://enc.c1oappe.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ppv.fzhhl.top

Go:   func add(a, b int) int { return a + b }
来源：http://djd.316326.xyz

Ruby: def add(a, b); a + b; end
来源：http://ykg.shanyushiyangkeji.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wah.uphjek.com

[C02] 默认参数
来源：http://aue.9152youxi.cn

Py:   def greet(name="World"): return name
来源：http://spn.9152youxi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ygr.zhiwuduotai.top

JS:   function greet(name = "World") { return name; }
来源：http://ejl.zycfv.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://riz.zhengqikj.top

Java: // 无默认参数：方法重载或 Optional
来源：http://psg.quarkkingdee.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ilv.quarkkingdee.top

Ruby: def greet(name = "World") = name
来源：http://ymz.xuanzx.com

C#:   string Greet(string name = "World") => name;
来源：http://ijw.ywan-chungtsiang.top

[C03] 可变参数
来源：http://ndm.c1oappe.top

Py:   def total(*args): return sum(args)
来源：http://mms.9152youxi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hvn.wangdashe.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mqh.jlsjyb.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://die.fanxiaobao.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fjy.jyoumei.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hcf.hammf.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mzy.gzhubu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rkx.yuxming.cn

[C04] 命名参数 / 关键字参数
来源：http://ytx.cucudq.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ttq.ctjpmb.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://izm.gotoacloud.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://udb.sjlbkw.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vby.shanyushiyangtech.top

Java: // 无：用 Builder 模式或 record
来源：http://bbg.hywenlv.cn

Go:   // 无：用配置结构体参数
来源：http://ihy.gotoacloud.top

Ruby: f(a: 1, b: 2)
来源：http://czv.yuanzhike.top

C#:   f(a: 1, b: 2)
来源：http://aun.tianlin.xyz

[C05] 返回多个值
来源：http://oym.hammf.cn

Py:   return a, b
来源：http://ldv.feifeiyinyue.top

PHP:  return [$a, $b];
来源：http://tlh.cashguo.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://dsr.zdqjudy.top

TS:   return { a, b };
来源：http://oei.cheryme.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wbq.nwbrower.top

Go:   return a, b
来源：http://btl.gaohongyu789.top

Ruby: return a, b
来源：http://azq.xuanzx.com

C#:   return (a, b);              // ValueTuple
来源：http://ani.dashuyun.cn

[C06] 匿名函数 / lambda
来源：http://xnq.fktsv.cn

Py:   square = lambda x: x * x
来源：http://xry.ivvv.top

PHP:  $square = fn($x) => $x * $x;
来源：http://pjy.zdqjudy.top

JS:   const square = x => x * x;
来源：http://opj.quarkkingdee.top

TS:   const square = (x: number): number => x * x;
来源：http://iln.birdmap.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bta.yanxiufei.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ual.chenzaomai.com

Ruby: square = ->(x) { x * x }
来源：http://prx.xinyue.icu

C#:   Func<int, int> square = x => x * x;
来源：http://drt.yj202588.top

[C07] 把函数作为参数传入
来源：http://trh.pengpengdd.cyou

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fff.iojbl.cn

PHP:  array_map("strtoupper", $arr);
来源：http://koh.zhixingplan.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zvc.ppjwa.cn

TS:   arr.map(String)
来源：http://xpy.guowangkeji.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xje.jinqigufen.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://liy.sjlbkw.cn

Ruby: arr.map(&:upcase)
来源：http://mfb.epnwcf.com

C#:   arr.Select(s => s.ToUpper())
来源：http://mkn.hongshengwenyu.top

[C08] 闭包
来源：http://vex.yvedp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kku.9152youxi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://oeh.nwbrower.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ljm.gaohongyu789.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xrw.yj20258888.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nug.tarul.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://oaa.wangdashe.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kag.chenlongwang.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qxj.bjfxy.top

[C09] 递归
来源：http://uag.shuidangran.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://esl.hesvh.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vpo.gotoacloud.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mrj.zhaomingkeji.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jbu.ybcxt.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dmu.zycfv.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kmg.wangshuangyany.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://foe.hcnkem.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://imj.xuanzx.com

[C10] 变量作用域
来源：http://qvr.sysykeji.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wnq.ydjk.org.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://elk.ydzc1.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://obk.yanxiufei.cn

TS:   同 JS
来源：http://prg.daria6918.cn

Java: 方法内为块级作用域
来源：http://iyu.smart0.xyz

Go:   花括号块级作用域
来源：http://uhm.yj20258.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kqn.pengpengdd.cyou

C#:   块级作用域
来源：http://ngi.daria6918.cn

[C11] 模块导入与导出
来源：http://daz.yvedp.cn

Py:   from module import func
来源：http://deu.ehwqpu.com

PHP:  require "file.php";  或 use App\Service;
来源：http://rdk.shanyushiyangtech.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://phk.hongshengwenyu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ofk.tarul.cn

Java: import java.util.List;
来源：http://hqc.fanxiaobao.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zmc.xuanzx.com

Ruby: require "json"; require_relative "./util"
来源：http://isg.9152youxi.cn

C#:   using System.Text;
来源：http://ahs.52xcode.cn

[C12] 立即执行函数 IIFE
来源：http://ssv.feifeiyinyue.top

Py:   (lambda: print("run"))()
来源：http://ajb.hongshengwenyu.top

PHP:  (function () { echo "run"; })();
来源：http://mcc.snrcjt.cn

JS:   (() => { console.log("run"); })();
来源：http://gfg.hywenlv.cn

TS:   (() => { console.log("run"); })();
来源：http://oth.cucudq.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ygx.sweek.top

Go:   func() { fmt.Println("run") }()
来源：http://kck.haohaochexian.top

Ruby: -> { puts "run" }.call
来源：http://fcl.fengsongda.top

C#:   // 无 IIFE：用静态构造函数
来源：http://lpn.jyoumei.cn

[C13] 类型声明 / 类型注解
来源：http://dav.zhengqikj.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ioo.quarkkingdee.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tvo.sxryk.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rxk.meibo888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vcd.yanxiufei.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xmx.snrcjt.cn

Go:   func add(a, b int) int
来源：http://lps.fanxiaobao.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gpo.jqgfzy.top

C#:   int Add(int a, int b) => a + b;
来源：http://ogd.jqgufenzy.top

[C14] 泛型函数
来源：http://vru.nanxinkj.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://meo.chenlongwang.top

PHP:  // 无泛型
来源：http://kne.sysykeji.top

JS:   // 无泛型
来源：http://dwo.xuetiantiany.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://goz.zhaomingkeji.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gpl.cucudq.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gyi.shanyushiyangtech.top

Ruby: # 无泛型
来源：http://oya.kuanghao11.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://eya.xingfuxueyuan.xyz

[C15] 解构 / 展开参数
来源：http://qxj.guannengcc.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hyz.zdbjq.cn

PHP:  [$a, $b] = $pair;
来源：http://yed.zhongyouzk.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://htt.c1oappe.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://csx.yj20258888.top

Java: // 无解构
来源：http://xgx.bjfxy.top

Go:   // 无解构
来源：http://dst.zhoulong.xyz

Ruby: a, b = pair
来源：http://eqn.yfazqb.com

C#:   var (a, b) = pair;
来源：http://koo.pengpengdd.cyou

[C16] 函数 / 方法重载
来源：http://wlp.zycfv.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hax.jinqigfzy.top

PHP:  // 无重载
来源：http://uaq.gotoacloud.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://tmi.yonumen.top

TS:   // 用联合类型或重载签名声明
来源：http://xza.jiagoushi.top

Java: void f(int a) {}  void f(String a) {}
来源：http://bgb.meibo888.top

Go:   // 无重载：用不同函数名
来源：http://uhm.tian-w.cn

Ruby: # 无重载：靠动态参数
来源：http://viy.gzhubu.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://eye.cashguo.top

================================================================================
来源：http://pac.chenjidiqi.icu

D. 数组 / 列表 / 集合
来源：http://ccr.9152youxi.cn

================================================================================
来源：http://riq.jinyuanbaomall.cn

[D01] 创建数组 / 列表
来源：http://cak.yuanzhike.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://rdu.cheryme.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://itj.gaohongyu789.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://efv.cdnleiting.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://zpz.birdmap.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dkr.nanxinkj.top

Go:   arr := []int{1, 2, 3}
来源：http://top.cucudq.cn

Ruby: arr = [1, 2, 3]
来源：http://cnz.chenjidiqi.icu

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qms.hywenlv.cn

[D02] 追加元素到末尾
来源：http://wxm.gzhubu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ohl.hysaishi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mhk.jinqigufen.top

JS:   arr.push(4);
来源：http://tfs.gaohongyu789.top

TS:   arr.push(4);
来源：http://nzw.gotoacloud.top

Java: list.add(4);
来源：http://wuf.meibo888.top

Go:   arr = append(arr, 4)
来源：http://yuz.cheryme.top

Ruby: arr << 4; arr.push(5)
来源：http://qmy.wangdashe.top

C#:   list.Add(4);
来源：http://nir.cqqwz.cn

[D03] 在指定位置插入元素
来源：http://lrm.haohaochexian.top

Py:   arr.insert(0, 0)
来源：http://eng.chenjidiqi.icu

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uml.sysykeji.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pqy.jinyuanbaomall.cn

TS:   arr.splice(0, 0, 0);
来源：http://cqt.iojbl.cn

Java: list.add(0, 0);
来源：http://dlv.yfazqb.com

Go:   arr = append([]int{0}, arr...)
来源：http://mbk.yonumen.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ddd.zhijiandao.cn

C#:   list.Insert(0, 0);
来源：http://wst.sxryk.cn

[D04] 删除元素
来源：http://wql.sjlbkw.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uxf.wangdashe.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://irh.havefunace.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uep.chenzaomai.com

TS:   arr.splice(0, 1);
来源：http://jjp.nwbrower.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qeg.quarkkingdee.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ias.fzhhl.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jos.aibaodan.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://loh.tanke756.top

[D05] 访问与修改元素
来源：http://osh.jyoumei.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sby.cashguo.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vlc.hnqzz.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ccy.ehwqpu.com

TS:   arr[0]; arr.at(-1);
来源：http://lse.pengpengdd.cyou

Java: list.get(0); list.set(0, 9);
来源：http://tvx.tarul.cn

Go:   arr[0]; arr[0] = 9
来源：http://krh.sweek.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://doq.jqgufenzy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mpx.chenzaomai.com

[D06] 数组长度
来源：http://skd.mhx1999.top

Py:   len(arr)
来源：http://lnb.sjlbkw.cn

PHP:  count($arr);
来源：http://jba.ydjk.org.cn

JS:   arr.length
来源：http://bol.sjlbkw.cn

TS:   arr.length
来源：http://aao.yfazqb.com

Java: list.size();
来源：http://oqi.hongshengwenyu.top

Go:   len(arr)
来源：http://ivs.nanxuanxn.top

Ruby: arr.length; arr.size
来源：http://vfl.svipenyu.cn

C#:   list.Count;
来源：http://snp.jyoumei.cn

[D07] 切片 / 取子数组
来源：http://ddp.cqqwz.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ahx.52xcode.cn

PHP:  array_slice($arr, 1, 3);
来源：http://llm.ywan-chungtsiang.top

JS:   arr.slice(1, 4);
来源：http://opf.dianchejie.cn

TS:   arr.slice(1, 4);
来源：http://dzs.dianchejie.cn

Java: list.subList(1, 4);
来源：http://lun.mhx1999.top

Go:   arr[1:4]
来源：http://tbq.jianghu66.top

Ruby: arr[1, 3]
来源：http://wik.chenjidiqi.icu

C#:   list.GetRange(1, 3);
来源：http://zyt.ybcxt.top

[D08] 合并两个数组
来源：http://off.redwolf501.top

Py:   a + b;  a.extend(b)
来源：http://tap.jiagoushi.top

PHP:  array_merge($a, $b);
来源：http://wyk.316326.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://kka.gaohongyu789.top

TS:   [...a, ...b];
来源：http://muq.yuxming.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mxr.nwbrower.top

Go:   append(a, b...)
来源：http://mfn.shanyushiyangtech.top

Ruby: a + b;  a.concat(b)
来源：http://lvc.ivvv.top

C#:   a.Concat(b).ToList()
来源：http://pph.gogol.net.cn

[D09] 排序（升序）
来源：http://toy.nwbrower.top

Py:   sorted(arr);  arr.sort()
来源：http://waq.yfazqb.com


<!-- 参考信息 -->