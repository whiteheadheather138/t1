代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://imp.sjlbkw.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://luk.chenzaomai.com

Ruby: begin; i += 1; end while i < 10
来源：http://cme.dashuyun.cn

C#:   do { i++; } while (i < 10);
来源：http://tkj.wangdashe.top

[B09] break 与 continue
来源：http://hfv.ehwqpu.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hsf.epnwcf.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hko.vqdsnc.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hwt.aibaodan.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fzz.haohaochexian.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kfe.yfazqb.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://znh.shzxlz.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wpd.daria6918.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jdd.xingfuxueyuan.xyz

[B10] 遍历同时拿索引
来源：http://gug.yvedp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fcg.jqgfzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wbx.hcnkem.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hbc.cdnleiting.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://awt.yfazqb.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bbs.gzhubu.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dno.fzhhl.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jmx.smart0.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hhn.feifeiyinyue.top

[B11] 生成数字序列 / 区间
来源：http://geb.sjlbkw.cn

Py:   list(range(0, 10, 2))
来源：http://rgo.zhengqikj.top

PHP:  range(0, 10, 2);
来源：http://bpd.svipenyu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lmb.hnqzz.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tii.zhengqikj.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uwo.yanxiufei.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zsl.vehdjk.com

Ruby: (0...10).step(2).to_a
来源：http://mji.chenjidiqi.icu

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xsc.gotoacloud.top

[B12] 跳出多层循环
来源：http://rqy.fktsv.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pgj.hammf.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://rfl.daxiang520.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rtq.xuanzx.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ujq.zdqjudy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tmc.mhx1999.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zdx.zhiwuduotai.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nqt.hongshengwenyu.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dxb.hysaishi.cn

[B13] 判断是否为数字
来源：http://jrh.zhixingplan.top

Py:   isinstance(x, (int, float))
来源：http://zoq.gaohongyu789.top

PHP:  is_numeric($x)
来源：http://okb.pycfn.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pfl.yvedp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://djp.wangdashe.top

Java: x instanceof Number
来源：http://sme.quarkkingdee.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lyy.dashuyun.cn

Ruby: x.is_a?(Numeric)
来源：http://kvv.shanyushiyangkeji.top

C#:   x is int or double or decimal
来源：http://sxx.zhiwuduotai.top

[B14] 判断值是否在集合内
来源：http://efp.epnwcf.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jxa.ctjpmb.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jqb.wangdashe.top

JS:   [1, 2, 3].includes(x)
来源：http://ond.xuetiantiany.cn

TS:   [1, 2, 3].includes(x)
来源：http://zfw.shangyingyoupin.top

Java: List.of(1, 2, 3).contains(x)
来源：http://qtt.zhongyouzk.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://anw.pengpengdd.cyou

Ruby: [1, 2, 3].include?(x)
来源：http://zxj.xinyue.icu

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://aen.yj20258.top

[B15] 布尔运算与取反
来源：http://ikl.shanyushiyangkeji.top

Py:   a and b or not c
来源：http://xkt.cashguo.top

PHP:  $a && $b || !$c
来源：http://iqz.zhijiandao.cn

JS:   a && b || !c
来源：http://ktf.316326.xyz

TS:   a && b || !c
来源：http://wda.zhixingplan.top

Java: a && b || !c
来源：http://jck.cdnleiting.top

Go:   a && b || !c
来源：http://dgy.yj20258.top

Ruby: a && b || !c
来源：http://ewp.fzhhl.top

C#:   a && b || !c
来源：http://ogz.tianlin.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://koi.shangyingyoupin.top

Py:   if not data: return
来源：http://wmw.yueranfly.top

PHP:  if (!$data) { return; }
来源：http://ima.ydzc1.top

JS:   if (!data) return;
来源：http://idv.nanxinkj.top

TS:   if (!data) return;
来源：http://lll.andypj.xyz

Java: if (data == null) return;
来源：http://knf.xuanzx.com

Go:   if data == nil { return }
来源：http://nvi.pengpengdd.cyou

Ruby: return if data.nil?
来源：http://abh.316326.xyz

C#:   if (data == null) return;
来源：http://iej.yangfankeji.com

================================================================================
来源：http://eql.shanyushiyangkeji.top

C. 函数与作用域
来源：http://xtl.cqqwz.cn

================================================================================
来源：http://cjy.zycfv.cn

[C01] 定义函数
来源：http://nvc.epnwcf.com

Py:   def add(a, b): return a + b
来源：http://uoz.shanyushiyangtech.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kkx.chenlongwang.top

JS:   function add(a, b) { return a + b; }
来源：http://cdm.yueranfly.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://khk.yj202588.top

Java: static int add(int a, int b) { return a + b; }
来源：http://cld.shangyingyoupin.top

Go:   func add(a, b int) int { return a + b }
来源：http://sps.xuetiantiany.cn

Ruby: def add(a, b); a + b; end
来源：http://fik.yj20258888.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rcv.bjfxy.top

[C02] 默认参数
来源：http://viv.mhx1999.top

Py:   def greet(name="World"): return name
来源：http://sep.haohaochexian.top

PHP:  function greet($name = "World") { return $name; }
来源：http://vga.shanyushiyangkeji.top

JS:   function greet(name = "World") { return name; }
来源：http://dso.xuetiantiany.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://oka.birdmap.top

Java: // 无默认参数：方法重载或 Optional
来源：http://gue.hesvh.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bfw.sweek.top

Ruby: def greet(name = "World") = name
来源：http://aax.yangfankeji.com

C#:   string Greet(string name = "World") => name;
来源：http://oyg.aibaodan.cn

[C03] 可变参数
来源：http://ese.tanke756.top

Py:   def total(*args): return sum(args)
来源：http://gth.gaohongyu789.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sfj.shanyushiyangtech.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kjw.fktsv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yki.xuetiantiany.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ozn.yuxming.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mqv.hywenlv.cn

Ruby: def total(*nums); nums.sum; end
来源：http://imd.xziqi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tqx.zycfv.cn

[C04] 命名参数 / 关键字参数
来源：http://eux.zdqjudy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qod.feifeiyinyue.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vrt.cucudq.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xlo.jinyuanbaomall.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bze.zdbjq.cn

Java: // 无：用 Builder 模式或 record
来源：http://hdd.hywenlv.cn

Go:   // 无：用配置结构体参数
来源：http://qbp.cucudq.cn

Ruby: f(a: 1, b: 2)
来源：http://dfy.hnqzz.top

C#:   f(a: 1, b: 2)
来源：http://cpc.zhoulong.xyz

[C05] 返回多个值
来源：http://ens.nanxinkj.top

Py:   return a, b
来源：http://ifp.tarul.cn

PHP:  return [$a, $b];
来源：http://eqi.gaohongyu789.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://egw.ivvv.top

TS:   return { a, b };
来源：http://xdn.jinqigufen.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://duw.zhiwuduotai.top

Go:   return a, b
来源：http://pno.ppjwa.cn

Ruby: return a, b
来源：http://bnh.shanyushiyangkeji.top

C#:   return (a, b);              // ValueTuple
来源：http://roq.yuanzhike.top

[C06] 匿名函数 / lambda
来源：http://dch.sysykeji.top

Py:   square = lambda x: x * x
来源：http://stl.bjfxy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://gcw.shangyingyoupin.top

JS:   const square = x => x * x;
来源：http://juw.kuanghao11.cn

TS:   const square = (x: number): number => x * x;
来源：http://jdd.nwbrower.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ske.yangfankeji.com

Go:   sq := func(x int) int { return x * x }
来源：http://xil.xylfe.cn

Ruby: square = ->(x) { x * x }
来源：http://nsz.hongshengwenyu.top

C#:   Func<int, int> square = x => x * x;
来源：http://ypa.gaohongyu789.top

[C07] 把函数作为参数传入
来源：http://ftp.hesvh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://iiv.zdqjudy.top

PHP:  array_map("strtoupper", $arr);
来源：http://sbn.vehdjk.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ogq.tian-w.cn

TS:   arr.map(String)
来源：http://adm.cdnleiting.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hhx.xinyue.icu

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jsa.meibo888.top

Ruby: arr.map(&:upcase)
来源：http://fbt.bjfxy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://nzz.chenzaomai.com

[C08] 闭包
来源：http://wyc.jinqigufen.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://owu.cucudq.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://exj.cheryme.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://olw.xuetiantiany.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hna.sysykeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vnf.316326.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://soe.zycfv.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ukl.dianchejie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hyh.hongshengwenyu.top

[C09] 递归
来源：http://uso.shuidangran.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rsf.zhongyouzk.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://axk.9152youxi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nzg.gaohongyu789.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hpf.shanyushiyangkeji.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://esa.tian-w.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tyz.sysykeji.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mjx.hfpthk.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sph.52xcode.cn

[C10] 变量作用域
来源：http://oow.jianghu66.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://otu.hywenlv.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mqe.aibaodan.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dqd.jqgufenzy.top

TS:   同 JS
来源：http://wsn.yueranfly.top

Java: 方法内为块级作用域
来源：http://isc.yongpay.top

Go:   花括号块级作用域
来源：http://xhr.ydzc1.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hax.shuidangran.top

C#:   块级作用域
来源：http://vap.daria6918.cn

[C11] 模块导入与导出
来源：http://qvd.nwbrower.top

Py:   from module import func
来源：http://ogq.cashguo.top

PHP:  require "file.php";  或 use App\Service;
来源：http://cod.zhoulong.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://cqz.nanxuanxn.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uzn.hywenlv.cn

Java: import java.util.List;
来源：http://yxr.bjfxy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jvt.zhoulong.xyz

Ruby: require "json"; require_relative "./util"
来源：http://dre.aizwys.cn

C#:   using System.Text;
来源：http://nvv.yj202588.top

[C12] 立即执行函数 IIFE
来源：http://rvs.shuidangran.top

Py:   (lambda: print("run"))()
来源：http://rxm.cucudq.cn

PHP:  (function () { echo "run"; })();
来源：http://nmv.redwolf501.top

JS:   (() => { console.log("run"); })();
来源：http://fnq.birdmap.top

TS:   (() => { console.log("run"); })();
来源：http://wae.aizwys.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qsn.svipenyu.cn

Go:   func() { fmt.Println("run") }()
来源：http://wvm.yfazqb.com

Ruby: -> { puts "run" }.call
来源：http://fgt.hywenlv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://bpb.shangyingyoupin.top

[C13] 类型声明 / 类型注解
来源：http://iig.316326.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://avr.zdbjq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jzj.gaohongyu789.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yeo.daxiang520.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://glw.tianlin.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://bwl.nanxuanxn.top

Go:   func add(a, b int) int
来源：http://jic.sjlbkw.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lnj.havefunace.top

C#:   int Add(int a, int b) => a + b;
来源：http://jnr.bbcook.cn

[C14] 泛型函数
来源：http://wsn.hcnkem.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://eaw.shanyushiyangtech.top

PHP:  // 无泛型
来源：http://ghn.jinqigufen.top

JS:   // 无泛型
来源：http://uht.jqgfzy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nlu.yongpay.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pcr.ivvv.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://twc.shangyingyoupin.top

Ruby: # 无泛型
来源：http://quh.iojbl.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mha.316326.xyz

[C15] 解构 / 展开参数
来源：http://kcx.nanxinkj.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xmv.chenzaomai.com

PHP:  [$a, $b] = $pair;
来源：http://nfp.fanxiaobao.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zzj.zhoulong.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nwm.zycfv.cn

Java: // 无解构
来源：http://vvx.yuxming.cn

Go:   // 无解构
来源：http://lew.sweek.top

Ruby: a, b = pair
来源：http://jme.vehdjk.com

C#:   var (a, b) = pair;
来源：http://tte.hnxiangtu.top

[C16] 函数 / 方法重载
来源：http://qns.sysykeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sml.yuxming.cn

PHP:  // 无重载
来源：http://ufu.sysykeji.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://yoq.fzhhl.top

TS:   // 用联合类型或重载签名声明
来源：http://uht.ybcxt.top

Java: void f(int a) {}  void f(String a) {}
来源：http://gyu.yj202588.top

Go:   // 无重载：用不同函数名
来源：http://tiz.svipenyu.cn

Ruby: # 无重载：靠动态参数
来源：http://hhd.sweek.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://bul.bbcook.cn

================================================================================
来源：http://fzp.gzhubu.top

D. 数组 / 列表 / 集合
来源：http://pdw.xylfe.cn

================================================================================
来源：http://vlr.shangyingyoupin.top

[D01] 创建数组 / 列表
来源：http://hxf.yj20258.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://nfx.xinyue.icu

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dne.yongpay.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wqs.hnqzz.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://rqo.yonumen.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gkm.yonumen.top

Go:   arr := []int{1, 2, 3}
来源：http://qfo.cheryme.top

Ruby: arr = [1, 2, 3]
来源：http://wrr.yfazqb.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jbx.tarul.cn

[D02] 追加元素到末尾
来源：http://ucx.dianchejie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tdk.zhongyouzk.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hru.dianchejie.cn

JS:   arr.push(4);
来源：http://gzx.9152youxi.cn

TS:   arr.push(4);
来源：http://ukl.xinyue.icu

Java: list.add(4);
来源：http://ghx.jyoumei.cn

Go:   arr = append(arr, 4)
来源：http://ieg.hywenlv.cn

Ruby: arr << 4; arr.push(5)
来源：http://aiz.zhoulong.xyz

C#:   list.Add(4);
来源：http://cwg.fanxiaobao.xyz

[D03] 在指定位置插入元素
来源：http://bfh.yongpay.top

Py:   arr.insert(0, 0)
来源：http://iak.redwolf501.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cni.gogol.net.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://alk.xziqi.cn

TS:   arr.splice(0, 0, 0);
来源：http://poj.gotoacloud.top

Java: list.add(0, 0);
来源：http://ywk.yj20258.top

Go:   arr = append([]int{0}, arr...)
来源：http://ada.zdbjq.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://feq.fengsongda.top

C#:   list.Insert(0, 0);
来源：http://lfe.ybcxt.top

[D04] 删除元素
来源：http://bkd.tian-w.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mdl.zhijiandao.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yen.hnqzz.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dih.jyoumei.cn

TS:   arr.splice(0, 1);
来源：http://npz.xylfe.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pma.tian-w.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vsq.sufxvd.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ocs.yongpay.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yso.ywan-chungtsiang.top

[D05] 访问与修改元素
来源：http://vhn.chenjidiqi.icu

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ool.fengsongda.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://anm.yangfankeji.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dhk.jyoumei.cn

TS:   arr[0]; arr.at(-1);
来源：http://ybd.gzhubu.top

Java: list.get(0); list.set(0, 9);
来源：http://vkd.quarkkingdee.top

Go:   arr[0]; arr[0] = 9
来源：http://wek.birdmap.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://djm.fktsv.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ccf.tian-w.cn

[D06] 数组长度
来源：http://xbk.52xcode.cn

Py:   len(arr)
来源：http://rrr.aibaodan.cn

PHP:  count($arr);
来源：http://idp.jinqigufen.top

JS:   arr.length
来源：http://gyp.yueranfly.top

TS:   arr.length
来源：http://wsd.zhiwuduotai.top

Java: list.size();
来源：http://yrb.fengsongda.top

Go:   len(arr)
来源：http://ift.hnxiangtu.top

Ruby: arr.length; arr.size
来源：http://uip.tian-w.cn

C#:   list.Count;
来源：http://ivt.cashguo.top

[D07] 切片 / 取子数组
来源：http://yar.fktsv.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gzi.jlsjyb.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ocd.fengsongda.top

JS:   arr.slice(1, 4);
来源：http://apd.zdbjq.cn

TS:   arr.slice(1, 4);
来源：http://kqd.xziqi.cn

Java: list.subList(1, 4);
来源：http://cby.hywenlv.cn

Go:   arr[1:4]
来源：http://qtw.xingfuxueyuan.xyz

Ruby: arr[1, 3]
来源：http://ect.hnqzz.top

C#:   list.GetRange(1, 3);
来源：http://thx.hcnkem.com

[D08] 合并两个数组
来源：http://kzs.chenjidiqi.icu

Py:   a + b;  a.extend(b)
来源：http://nrt.jinghuilouyu.cn

PHP:  array_merge($a, $b);
来源：http://irt.zhongyouzk.top

JS:   [...a, ...b];  a.concat(b);
来源：http://uqc.uphjek.com

TS:   [...a, ...b];
来源：http://tql.aizwys.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yxh.sxryk.cn

Go:   append(a, b...)
来源：http://ifo.jiagoushi.top

Ruby: a + b;  a.concat(b)
来源：http://upg.jinqigfzy.top

C#:   a.Concat(b).ToList()
来源：http://mnf.shzxlz.cn

[D09] 排序（升序）
来源：http://chl.yuanzhike.top

Py:   sorted(arr);  arr.sort()
来源：http://orv.jyoumei.cn


<!-- 参考信息 -->