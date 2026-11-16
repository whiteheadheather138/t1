代发 wailian999

[B09] break 与 continue
来源：http://kpq.wangdashe.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yft.hfpthk.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ngb.sxryk.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dwd.yanxiufei.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qnc.cdnleiting.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ebx.hfpthk.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wec.jinyuanbaomall.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://upp.hywenlv.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uiz.zhengqikj.top

[B10] 遍历同时拿索引
来源：http://qbr.jiagoushi.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://apv.nwbrower.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zku.xinyue.icu

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wzq.yvedp.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ndr.yj202588.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zlw.gogol.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kxg.shzxlz.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://unv.cheryme.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://auf.zhixingplan.top

[B11] 生成数字序列 / 区间
来源：http://bue.52xcode.cn

Py:   list(range(0, 10, 2))
来源：http://hiw.nanxuanxn.top

PHP:  range(0, 10, 2);
来源：http://hoq.xuanzx.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lvy.hysaishi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uvl.haohaochexian.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zrv.shangyingyoupin.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mmc.haohaochexian.top

Ruby: (0...10).step(2).to_a
来源：http://wob.birdmap.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xyu.ywan-chungtsiang.top

[B12] 跳出多层循环
来源：http://spe.dashuyun.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://sdr.pycfn.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://ija.yvedp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ojt.fehbvm.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hnm.yongpay.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zzk.bjfxy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://alg.yanxiufei.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vua.chenzaomai.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vfy.xuetiantiany.cn

[B13] 判断是否为数字
来源：http://vfy.xinyue.icu

Py:   isinstance(x, (int, float))
来源：http://wra.xuanzx.com

PHP:  is_numeric($x)
来源：http://rgc.sxryk.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://avj.shangyingyoupin.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://edi.jyoumei.cn

Java: x instanceof Number
来源：http://omz.hfpthk.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hfp.yj20258888.top

Ruby: x.is_a?(Numeric)
来源：http://rzk.chenjidiqi.icu

C#:   x is int or double or decimal
来源：http://pxf.guowangkeji.top

[B14] 判断值是否在集合内
来源：http://upq.daria6918.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://crb.redwolf501.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nau.chenjidiqi.icu

JS:   [1, 2, 3].includes(x)
来源：http://qht.shzxlz.cn

TS:   [1, 2, 3].includes(x)
来源：http://tft.cashguo.top

Java: List.of(1, 2, 3).contains(x)
来源：http://pcu.snrcjt.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xbh.xuanzx.com

Ruby: [1, 2, 3].include?(x)
来源：http://bdv.nanxuanxn.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tfb.yuanzhike.top

[B15] 布尔运算与取反
来源：http://ygj.aibaodan.cn

Py:   a and b or not c
来源：http://nkw.mhx1999.top

PHP:  $a && $b || !$c
来源：http://hkv.fzhhl.top

JS:   a && b || !c
来源：http://nag.daria6918.cn

TS:   a && b || !c
来源：http://sct.nwbrower.top

Java: a && b || !c
来源：http://npk.chenzaomai.com

Go:   a && b || !c
来源：http://aym.zdbjq.cn

Ruby: a && b || !c
来源：http://dlh.yanxiufei.cn

C#:   a && b || !c
来源：http://zfi.hongshengwenyu.top

[B16] 卫语句：不满足条件提前返回
来源：http://opo.zhixingplan.top

Py:   if not data: return
来源：http://qei.aibaodan.cn

PHP:  if (!$data) { return; }
来源：http://gdy.ppjwa.cn

JS:   if (!data) return;
来源：http://zbe.fehbvm.com

TS:   if (!data) return;
来源：http://ouv.zycfv.cn

Java: if (data == null) return;
来源：http://rgm.sufxvd.cn

Go:   if data == nil { return }
来源：http://ocd.chenjidiqi.icu

Ruby: return if data.nil?
来源：http://gvp.jinyuanbaomall.cn

C#:   if (data == null) return;
来源：http://reo.xingfuxueyuan.xyz

================================================================================
来源：http://yov.fanxiaobao.xyz

C. 函数与作用域
来源：http://pmi.shzxlz.cn

================================================================================
来源：http://mdh.sjlbkw.cn

[C01] 定义函数
来源：http://hdj.zhixingplan.top

Py:   def add(a, b): return a + b
来源：http://afs.snrcjt.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gxu.jinqigfzy.top

JS:   function add(a, b) { return a + b; }
来源：http://rtj.gogol.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mxb.andypj.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://vpj.nwbrower.top

Go:   func add(a, b int) int { return a + b }
来源：http://kik.sysykeji.top

Ruby: def add(a, b); a + b; end
来源：http://yle.gzhubu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ljq.sufxvd.cn

[C02] 默认参数
来源：http://twd.redwolf501.top

Py:   def greet(name="World"): return name
来源：http://slv.meibo888.top

PHP:  function greet($name = "World") { return $name; }
来源：http://gim.tanke756.top

JS:   function greet(name = "World") { return name; }
来源：http://rce.gotoacloud.top

TS:   function greet(name: string = "World") { return name; }
来源：http://hwc.pycfn.com

Java: // 无默认参数：方法重载或 Optional
来源：http://tyj.xuetiantiany.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wzr.shuidangran.top

Ruby: def greet(name = "World") = name
来源：http://yab.svipenyu.cn

C#:   string Greet(string name = "World") => name;
来源：http://bxc.shzxlz.cn

[C03] 可变参数
来源：http://sir.fzhhl.top

Py:   def total(*args): return sum(args)
来源：http://sno.tanke756.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://luj.c1oappe.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hpn.hywenlv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ghj.xuetiantiany.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kqo.shangyingyoupin.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qni.nanxinkj.top

Ruby: def total(*nums); nums.sum; end
来源：http://gwa.zhoulong.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lem.nanxuanxn.top

[C04] 命名参数 / 关键字参数
来源：http://roh.shanyushiyangtech.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rrr.svipenyu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lqo.meibo888.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tgq.tarul.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rjb.ctjpmb.com

Java: // 无：用 Builder 模式或 record
来源：http://gfl.zhiwuduotai.top

Go:   // 无：用配置结构体参数
来源：http://qvu.wangdashe.top

Ruby: f(a: 1, b: 2)
来源：http://wmg.hcnkem.com

C#:   f(a: 1, b: 2)
来源：http://few.xingfuxueyuan.xyz

[C05] 返回多个值
来源：http://aim.zhoulong.xyz

Py:   return a, b
来源：http://wvq.feifeiyinyue.top

PHP:  return [$a, $b];
来源：http://dxs.kuanghao11.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ohs.ydjk.org.cn

TS:   return { a, b };
来源：http://ygw.jiagoushi.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fnj.daria6918.cn

Go:   return a, b
来源：http://ust.xziqi.cn

Ruby: return a, b
来源：http://jod.yuxming.cn

C#:   return (a, b);              // ValueTuple
来源：http://lez.sysykeji.top

[C06] 匿名函数 / lambda
来源：http://nru.zhaomingkeji.xyz

Py:   square = lambda x: x * x
来源：http://ged.jinqigfzy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://hmv.mhx1999.top

JS:   const square = x => x * x;
来源：http://vsq.tianlin.xyz

TS:   const square = (x: number): number => x * x;
来源：http://qfk.fktsv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rgr.hcnkem.com

Go:   sq := func(x int) int { return x * x }
来源：http://hro.zhongyouzk.top

Ruby: square = ->(x) { x * x }
来源：http://cpx.c1oappe.top

C#:   Func<int, int> square = x => x * x;
来源：http://sla.vqdsnc.cn

[C07] 把函数作为参数传入
来源：http://jwe.chenzaomai.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dip.xuanzx.com

PHP:  array_map("strtoupper", $arr);
来源：http://whm.birdmap.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uph.snrcjt.cn

TS:   arr.map(String)
来源：http://lhj.gogol.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fhc.zdbjq.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://itn.c1oappe.top

Ruby: arr.map(&:upcase)
来源：http://opt.pengpengdd.cyou

C#:   arr.Select(s => s.ToUpper())
来源：http://qpn.aibaodan.cn

[C08] 闭包
来源：http://saw.jqgfzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bwg.pycfn.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://eti.yfazqb.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dxp.shanyushiyangtech.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lcj.jyoumei.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bos.fehbvm.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://thx.0kj1m.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://irk.gogol.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vap.zhengqikj.top

[C09] 递归
来源：http://mnv.tarul.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qij.hongshengwenyu.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uha.c1oappe.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gri.zdqjudy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mmz.ybcxt.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://brl.hysaishi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rxs.yuanzhike.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://avi.yangfankeji.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xqc.316326.xyz

[C10] 变量作用域
来源：http://qam.jqgfzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://din.xuetiantiany.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://skf.birdmap.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zwz.nanxuanxn.top

TS:   同 JS
来源：http://jzc.zhixingplan.top

Java: 方法内为块级作用域
来源：http://gzj.zhengqikj.top

Go:   花括号块级作用域
来源：http://pmd.zdbjq.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pha.yangfankeji.com

C#:   块级作用域
来源：http://pcf.zdbjq.cn

[C11] 模块导入与导出
来源：http://qjj.svipenyu.cn

Py:   from module import func
来源：http://zvw.zhongyouzk.top

PHP:  require "file.php";  或 use App\Service;
来源：http://bch.haohaochexian.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://duw.hysaishi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mni.pengpengdd.cyou

Java: import java.util.List;
来源：http://xsa.gaohongyu789.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bpg.gotoacloud.top

Ruby: require "json"; require_relative "./util"
来源：http://dkh.ydjk.org.cn

C#:   using System.Text;
来源：http://cyp.dianchejie.cn

[C12] 立即执行函数 IIFE
来源：http://bjs.0kj1m.cn

Py:   (lambda: print("run"))()
来源：http://rew.dashuyun.cn

PHP:  (function () { echo "run"; })();
来源：http://eaa.ehwqpu.com

JS:   (() => { console.log("run"); })();
来源：http://dtf.yuxming.cn

TS:   (() => { console.log("run"); })();
来源：http://epw.kuanghao11.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gnf.jianghu66.top

Go:   func() { fmt.Println("run") }()
来源：http://qlv.nanxinkj.top

Ruby: -> { puts "run" }.call
来源：http://pqf.0kj1m.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://eds.fzhhl.top

[C13] 类型声明 / 类型注解
来源：http://xgt.feifeiyinyue.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mdk.vehdjk.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dfr.jinqigfzy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://eft.iojbl.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://aiu.jlsjyb.cn

Java: int add(int a, int b) { return a + b; }
来源：http://uto.svipenyu.cn

Go:   func add(a, b int) int
来源：http://vts.cashguo.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tln.snrcjt.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bxf.vehdjk.com

[C14] 泛型函数
来源：http://yex.hywenlv.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kkj.zhijiandao.cn

PHP:  // 无泛型
来源：http://rgi.jlsjyb.cn

JS:   // 无泛型
来源：http://eno.havefunace.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hpf.vqdsnc.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xyc.yonumen.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://uks.pengpengdd.cyou

Ruby: # 无泛型
来源：http://fbl.aizwys.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ijh.nanxuanxn.top

[C15] 解构 / 展开参数
来源：http://myz.dianchejie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://iyn.chenjidiqi.icu

PHP:  [$a, $b] = $pair;
来源：http://djv.hongshengwenyu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://unp.jinyuanbaomall.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://umw.gotoacloud.top

Java: // 无解构
来源：http://bzt.yueranfly.top

Go:   // 无解构
来源：http://gjf.yongpay.top

Ruby: a, b = pair
来源：http://slm.jianghu66.top

C#:   var (a, b) = pair;
来源：http://mgw.hammf.cn

[C16] 函数 / 方法重载
来源：http://dzr.hywenlv.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vzn.chenlongwang.top

PHP:  // 无重载
来源：http://duo.tian-w.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://drf.sjlbkw.cn

TS:   // 用联合类型或重载签名声明
来源：http://iya.chenlongwang.top

Java: void f(int a) {}  void f(String a) {}
来源：http://egp.sxryk.cn

Go:   // 无重载：用不同函数名
来源：http://weh.zhongyouzk.top

Ruby: # 无重载：靠动态参数
来源：http://dfa.jinqigufen.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://djq.fzhhl.top

================================================================================
来源：http://xhe.wangdashe.top

D. 数组 / 列表 / 集合
来源：http://xvv.zhiwuduotai.top

================================================================================
来源：http://eho.chenzaomai.com

[D01] 创建数组 / 列表
来源：http://ugx.ppjwa.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://yoc.haohaochexian.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jvo.yvedp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dlb.cqqwz.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fjf.0kj1m.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hfk.yuxming.cn

Go:   arr := []int{1, 2, 3}
来源：http://wpk.yongpay.top

Ruby: arr = [1, 2, 3]
来源：http://fyr.shangyingyoupin.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gdh.zhoulong.xyz

[D02] 追加元素到末尾
来源：http://ahx.wangshuangyany.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wmi.yangfankeji.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://slq.sjlbkw.cn

JS:   arr.push(4);
来源：http://nmh.ehwqpu.com

TS:   arr.push(4);
来源：http://vwv.zdbjq.cn

Java: list.add(4);
来源：http://jhw.zhijiandao.cn

Go:   arr = append(arr, 4)
来源：http://hlz.fanxiaobao.xyz

Ruby: arr << 4; arr.push(5)
来源：http://ttz.gotoacloud.top

C#:   list.Add(4);
来源：http://mry.zycfv.cn

[D03] 在指定位置插入元素
来源：http://vwv.yanxiufei.cn

Py:   arr.insert(0, 0)
来源：http://mkk.daxiang520.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dxj.fehbvm.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wwm.jinghuilouyu.cn

TS:   arr.splice(0, 0, 0);
来源：http://bkx.wangdashe.top

Java: list.add(0, 0);
来源：http://sgf.jinghuilouyu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qvj.zhiwuduotai.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://byf.iojbl.cn

C#:   list.Insert(0, 0);
来源：http://ymq.shuidangran.top

[D04] 删除元素
来源：http://ikw.shangyingyoupin.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ycc.sweek.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ulh.cheryme.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bys.ctjpmb.com

TS:   arr.splice(0, 1);
来源：http://qdu.xingfuxueyuan.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sfh.ywan-chungtsiang.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hgv.kuanghao11.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fds.zhaomingkeji.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hcq.yj20258888.top

[D05] 访问与修改元素
来源：http://kvj.gaohongyu789.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mkr.tianlin.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lgn.yongpay.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lzn.vehdjk.com

TS:   arr[0]; arr.at(-1);
来源：http://obf.tarul.cn

Java: list.get(0); list.set(0, 9);
来源：http://jfl.zhongyouzk.top

Go:   arr[0]; arr[0] = 9
来源：http://res.havefunace.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tqf.gotoacloud.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nlx.zhaomingkeji.xyz

[D06] 数组长度
来源：http://eqx.wangdashe.top

Py:   len(arr)
来源：http://fuh.iojbl.cn

PHP:  count($arr);
来源：http://sdz.guannengcc.top

JS:   arr.length
来源：http://vxp.ydjk.org.cn

TS:   arr.length
来源：http://zol.zycfv.cn

Java: list.size();
来源：http://rhs.yfazqb.com

Go:   len(arr)
来源：http://gwd.sweek.top

Ruby: arr.length; arr.size
来源：http://vms.daria6918.cn

C#:   list.Count;
来源：http://ruu.jlsjyb.cn

[D07] 切片 / 取子数组
来源：http://leh.chenjidiqi.icu

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://myj.c1oappe.top

PHP:  array_slice($arr, 1, 3);
来源：http://tba.pycfn.com

JS:   arr.slice(1, 4);
来源：http://due.dianchejie.cn

TS:   arr.slice(1, 4);
来源：http://dhz.shuidangran.top

Java: list.subList(1, 4);
来源：http://vis.0kj1m.cn

Go:   arr[1:4]
来源：http://bfc.ivvv.top

Ruby: arr[1, 3]
来源：http://nyt.kuanghao11.cn

C#:   list.GetRange(1, 3);
来源：http://uwu.vehdjk.com

[D08] 合并两个数组
来源：http://ata.sjlbkw.cn

Py:   a + b;  a.extend(b)
来源：http://uby.hnxiangtu.top

PHP:  array_merge($a, $b);
来源：http://kdw.chenjidiqi.icu

JS:   [...a, ...b];  a.concat(b);
来源：http://pvt.52xcode.cn

TS:   [...a, ...b];
来源：http://cvc.ivvv.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ugp.hnxiangtu.top

Go:   append(a, b...)
来源：http://waq.yvedp.cn

Ruby: a + b;  a.concat(b)
来源：http://xzr.daxiang520.top

C#:   a.Concat(b).ToList()
来源：http://dpq.gaohongyu789.top

[D09] 排序（升序）
来源：http://sqe.jinqigfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://gak.sufxvd.cn

PHP:  sort($arr);
来源：http://obg.yangfankeji.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ofu.aizwys.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lwx.chenlongwang.top

Java: Collections.sort(list);  list.sort(null);
来源：http://gte.fehbvm.com


<!-- 参考信息 -->