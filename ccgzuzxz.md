代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://ayn.vqdsnc.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://axt.ydjk.org.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ywg.ehwqpu.com

C#:   do { i++; } while (i < 10);
来源：http://drx.sufxvd.cn

[B09] break 与 continue
来源：http://bfa.jianghu66.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hph.gogol.net.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qnw.wangshuangyany.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lyd.jyoumei.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tdn.shzxlz.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ggo.316326.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ofy.ydzc1.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dpn.smart0.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jbw.bjfxy.top

[B10] 遍历同时拿索引
来源：http://lkr.hnqzz.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fug.mhx1999.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://abf.dashuyun.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cfj.smart0.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tsy.zhijiandao.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://azr.fzhhl.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xqh.chenzaomai.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ghv.hcnkem.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vwl.fengsongda.top

[B11] 生成数字序列 / 区间
来源：http://ftt.vqdsnc.cn

Py:   list(range(0, 10, 2))
来源：http://ysn.ehwqpu.com

PHP:  range(0, 10, 2);
来源：http://zjj.wangshuangyany.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://byy.hysaishi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jzv.havefunace.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xto.tian-w.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nuv.316326.xyz

Ruby: (0...10).step(2).to_a
来源：http://wng.xylfe.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rnr.9152youxi.cn

[B12] 跳出多层循环
来源：http://ytm.tian-w.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://nrv.wangdashe.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://vtt.fzhhl.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://erb.hywenlv.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pgk.ppjwa.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sqw.yuanzhike.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qmi.smart0.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ize.xinyue.icu

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hut.zhiwuduotai.top

[B13] 判断是否为数字
来源：http://ivg.0kj1m.cn

Py:   isinstance(x, (int, float))
来源：http://mtq.yangfankeji.com

PHP:  is_numeric($x)
来源：http://rbf.yj20258888.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zsc.fanxiaobao.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gbm.zdqjudy.top

Java: x instanceof Number
来源：http://eft.aizwys.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xry.ybcxt.top

Ruby: x.is_a?(Numeric)
来源：http://lty.zhijiandao.cn

C#:   x is int or double or decimal
来源：http://fct.ydjk.org.cn

[B14] 判断值是否在集合内
来源：http://lkk.epnwcf.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bnv.dashuyun.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mbn.jinghuilouyu.cn

JS:   [1, 2, 3].includes(x)
来源：http://mff.ehwqpu.com

TS:   [1, 2, 3].includes(x)
来源：http://doj.hammf.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nvk.zycfv.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://skb.hcnkem.com

Ruby: [1, 2, 3].include?(x)
来源：http://plg.xingfuxueyuan.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dwd.hammf.cn

[B15] 布尔运算与取反
来源：http://drn.pengpengdd.cyou

Py:   a and b or not c
来源：http://xod.quarkkingdee.top

PHP:  $a && $b || !$c
来源：http://smv.xuetiantiany.cn

JS:   a && b || !c
来源：http://nni.xuetiantiany.cn

TS:   a && b || !c
来源：http://uxl.52xcode.cn

Java: a && b || !c
来源：http://cdv.jqgfzy.top

Go:   a && b || !c
来源：http://vel.chenjidiqi.icu

Ruby: a && b || !c
来源：http://poa.jinqigufen.top

C#:   a && b || !c
来源：http://ymh.hnxiangtu.top

[B16] 卫语句：不满足条件提前返回
来源：http://nbk.birdmap.top

Py:   if not data: return
来源：http://ycf.yonumen.top

PHP:  if (!$data) { return; }
来源：http://dkc.jyoumei.cn

JS:   if (!data) return;
来源：http://crp.jinqigufen.top

TS:   if (!data) return;
来源：http://zue.yj20258888.top

Java: if (data == null) return;
来源：http://gzh.vqdsnc.cn

Go:   if data == nil { return }
来源：http://day.wangshuangyany.cn

Ruby: return if data.nil?
来源：http://azr.xziqi.cn

C#:   if (data == null) return;
来源：http://ias.haohaochexian.top

================================================================================
来源：http://pme.hammf.cn

C. 函数与作用域
来源：http://jpo.andypj.xyz

================================================================================
来源：http://sgg.fanxiaobao.xyz

[C01] 定义函数
来源：http://yik.quarkkingdee.top

Py:   def add(a, b): return a + b
来源：http://cnu.daria6918.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tmx.jinqigufen.top

JS:   function add(a, b) { return a + b; }
来源：http://mky.316326.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://urv.tanke756.top

Java: static int add(int a, int b) { return a + b; }
来源：http://fst.fktsv.cn

Go:   func add(a, b int) int { return a + b }
来源：http://lzn.haohaochexian.top

Ruby: def add(a, b); a + b; end
来源：http://idg.xuetiantiany.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://crq.vehdjk.com

[C02] 默认参数
来源：http://bsl.jiagoushi.top

Py:   def greet(name="World"): return name
来源：http://gme.316326.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://vpx.andypj.xyz

JS:   function greet(name = "World") { return name; }
来源：http://vin.cucudq.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gvs.wangdashe.top

Java: // 无默认参数：方法重载或 Optional
来源：http://duq.yangfankeji.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vwf.ywan-chungtsiang.top

Ruby: def greet(name = "World") = name
来源：http://sco.yongpay.top

C#:   string Greet(string name = "World") => name;
来源：http://vib.cashguo.top

[C03] 可变参数
来源：http://fzx.svipenyu.cn

Py:   def total(*args): return sum(args)
来源：http://jqf.mhx1999.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qqt.aizwys.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zop.sufxvd.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kgo.yonumen.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jho.fehbvm.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qau.cucudq.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vif.zhoulong.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://niw.sxryk.cn

[C04] 命名参数 / 关键字参数
来源：http://exo.kuanghao11.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jut.yfazqb.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sbd.uphjek.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wqf.yonumen.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://haz.jinghuilouyu.cn

Java: // 无：用 Builder 模式或 record
来源：http://pqj.gotoacloud.top

Go:   // 无：用配置结构体参数
来源：http://euc.uphjek.com

Ruby: f(a: 1, b: 2)
来源：http://tjx.zycfv.cn

C#:   f(a: 1, b: 2)
来源：http://yzo.fengsongda.top

[C05] 返回多个值
来源：http://dki.daria6918.cn

Py:   return a, b
来源：http://lju.gogol.net.cn

PHP:  return [$a, $b];
来源：http://jud.redwolf501.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://alw.ctjpmb.com

TS:   return { a, b };
来源：http://yby.sweek.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://iin.zhijiandao.cn

Go:   return a, b
来源：http://sdl.dashuyun.cn

Ruby: return a, b
来源：http://cjq.ctjpmb.com

C#:   return (a, b);              // ValueTuple
来源：http://lgy.shanyushiyangtech.top

[C06] 匿名函数 / lambda
来源：http://mxa.jinqigfzy.top

Py:   square = lambda x: x * x
来源：http://atu.nanxuanxn.top

PHP:  $square = fn($x) => $x * $x;
来源：http://qpz.yj20258888.top

JS:   const square = x => x * x;
来源：http://lnb.yj202588.top

TS:   const square = (x: number): number => x * x;
来源：http://rvk.dashuyun.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qxt.wangshuangyany.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ise.jqgfzy.top

Ruby: square = ->(x) { x * x }
来源：http://poc.sjlbkw.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cua.shangyingyoupin.top

[C07] 把函数作为参数传入
来源：http://dvn.zhongyouzk.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bgb.jinqigfzy.top

PHP:  array_map("strtoupper", $arr);
来源：http://prk.xinyue.icu

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ohx.chenzaomai.com

TS:   arr.map(String)
来源：http://lhr.guannengcc.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xwn.fzhhl.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cqs.xylfe.cn

Ruby: arr.map(&:upcase)
来源：http://yqr.zhaomingkeji.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://rls.shzxlz.cn

[C08] 闭包
来源：http://crz.tian-w.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qfd.zhijiandao.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://enx.cashguo.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jej.guowangkeji.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wjc.cashguo.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pkw.zycfv.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dsb.yongpay.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://thc.zdqjudy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://sih.fanxiaobao.xyz

[C09] 递归
来源：http://qhv.zhengqikj.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lzk.epnwcf.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://euk.mhx1999.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cni.tian-w.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://whp.xingfuxueyuan.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://syi.hammf.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wri.zhaomingkeji.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pdr.zdqjudy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qnn.zhijiandao.cn

[C10] 变量作用域
来源：http://rzq.jinyuanbaomall.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://std.guowangkeji.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://goo.yj202588.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gzu.9152youxi.cn

TS:   同 JS
来源：http://zsw.fzhhl.top

Java: 方法内为块级作用域
来源：http://rsu.316326.xyz

Go:   花括号块级作用域
来源：http://fni.dashuyun.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://spe.wangshuangyany.cn

C#:   块级作用域
来源：http://agy.cucudq.cn

[C11] 模块导入与导出
来源：http://pol.nanxinkj.top

Py:   from module import func
来源：http://yod.fanxiaobao.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://jmz.zhiwuduotai.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://fuk.ywan-chungtsiang.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zew.quarkkingdee.top

Java: import java.util.List;
来源：http://fqa.guowangkeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gqe.ehwqpu.com

Ruby: require "json"; require_relative "./util"
来源：http://aiu.dashuyun.cn

C#:   using System.Text;
来源：http://gnv.shzxlz.cn

[C12] 立即执行函数 IIFE
来源：http://ghe.xingfuxueyuan.xyz

Py:   (lambda: print("run"))()
来源：http://hov.andypj.xyz

PHP:  (function () { echo "run"; })();
来源：http://uou.yueranfly.top

JS:   (() => { console.log("run"); })();
来源：http://abq.zycfv.cn

TS:   (() => { console.log("run"); })();
来源：http://tlm.tianlin.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wld.svipenyu.cn

Go:   func() { fmt.Println("run") }()
来源：http://lil.tian-w.cn

Ruby: -> { puts "run" }.call
来源：http://cme.jinqigfzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ecl.chenzaomai.com

[C13] 类型声明 / 类型注解
来源：http://guf.hysaishi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rdi.0kj1m.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jpn.hammf.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hmu.ywan-chungtsiang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pmt.yuxming.cn

Java: int add(int a, int b) { return a + b; }
来源：http://iot.gogol.net.cn

Go:   func add(a, b int) int
来源：http://qet.yanxiufei.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hqs.guannengcc.top

C#:   int Add(int a, int b) => a + b;
来源：http://okk.jinghuilouyu.cn

[C14] 泛型函数
来源：http://rwp.vqdsnc.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tbh.yj20258888.top

PHP:  // 无泛型
来源：http://mye.xylfe.cn

JS:   // 无泛型
来源：http://csd.meibo888.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zwp.cashguo.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qwl.ybcxt.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://oxz.jyoumei.cn

Ruby: # 无泛型
来源：http://xiw.sweek.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wmv.xingfuxueyuan.xyz

[C15] 解构 / 展开参数
来源：http://zuf.xuetiantiany.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mbw.yanxiufei.cn

PHP:  [$a, $b] = $pair;
来源：http://jma.ywan-chungtsiang.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wwv.0kj1m.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ztx.yongpay.top

Java: // 无解构
来源：http://aal.haohaochexian.top

Go:   // 无解构
来源：http://uwv.daxiang520.top

Ruby: a, b = pair
来源：http://dau.yanxiufei.cn

C#:   var (a, b) = pair;
来源：http://qvk.aizwys.cn

[C16] 函数 / 方法重载
来源：http://zpf.gotoacloud.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hpa.gogol.net.cn

PHP:  // 无重载
来源：http://hnq.snrcjt.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://cyp.birdmap.top

TS:   // 用联合类型或重载签名声明
来源：http://hmb.smart0.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://hek.birdmap.top

Go:   // 无重载：用不同函数名
来源：http://zsv.yfazqb.com

Ruby: # 无重载：靠动态参数
来源：http://clk.zhaomingkeji.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://vkz.jianghu66.top

================================================================================
来源：http://khp.fengsongda.top

D. 数组 / 列表 / 集合
来源：http://ypb.hywenlv.cn

================================================================================
来源：http://tlp.nanxinkj.top

[D01] 创建数组 / 列表
来源：http://wmr.vehdjk.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://qur.zhengqikj.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tcl.shangyingyoupin.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vyq.vqdsnc.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wtt.smart0.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vkb.ehwqpu.com

Go:   arr := []int{1, 2, 3}
来源：http://yoq.uphjek.com

Ruby: arr = [1, 2, 3]
来源：http://tbv.ydjk.org.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ehh.nwbrower.top

[D02] 追加元素到末尾
来源：http://giq.shanyushiyangtech.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://plg.chenzaomai.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wbx.jinqigufen.top

JS:   arr.push(4);
来源：http://stw.cucudq.cn

TS:   arr.push(4);
来源：http://lsz.9152youxi.cn

Java: list.add(4);
来源：http://kvj.jqgufenzy.top

Go:   arr = append(arr, 4)
来源：http://rsd.zhongyouzk.top

Ruby: arr << 4; arr.push(5)
来源：http://rva.jinghuilouyu.cn

C#:   list.Add(4);
来源：http://qpb.jinyuanbaomall.cn

[D03] 在指定位置插入元素
来源：http://rts.zhengqikj.top

Py:   arr.insert(0, 0)
来源：http://spt.fehbvm.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://syo.cdnleiting.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vpl.ybcxt.top

TS:   arr.splice(0, 0, 0);
来源：http://ods.yj20258888.top

Java: list.add(0, 0);
来源：http://mij.zdbjq.cn

Go:   arr = append([]int{0}, arr...)
来源：http://iav.hysaishi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tjp.hnxiangtu.top

C#:   list.Insert(0, 0);
来源：http://cxm.gogol.net.cn

[D04] 删除元素
来源：http://eoj.ydjk.org.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lgb.uphjek.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tzm.gotoacloud.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yam.andypj.xyz

TS:   arr.splice(0, 1);
来源：http://fcq.zhiwuduotai.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://akf.tian-w.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jim.shanyushiyangtech.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gcf.zhoulong.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yit.wangdashe.top

[D05] 访问与修改元素
来源：http://ofc.hammf.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kab.haohaochexian.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hum.vehdjk.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wnk.yuxming.cn

TS:   arr[0]; arr.at(-1);
来源：http://vqe.xuetiantiany.cn

Java: list.get(0); list.set(0, 9);
来源：http://ieh.haohaochexian.top

Go:   arr[0]; arr[0] = 9
来源：http://hvi.haohaochexian.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://syo.jinqigfzy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mss.cheryme.top

[D06] 数组长度
来源：http://mtz.dianchejie.cn

Py:   len(arr)
来源：http://anh.tarul.cn

PHP:  count($arr);
来源：http://vsl.jinghuilouyu.cn

JS:   arr.length
来源：http://uhv.hywenlv.cn

TS:   arr.length
来源：http://nfr.cdnleiting.top

Java: list.size();
来源：http://yxm.jinghuilouyu.cn

Go:   len(arr)
来源：http://ykm.nwbrower.top

Ruby: arr.length; arr.size
来源：http://aoq.yanxiufei.cn

C#:   list.Count;
来源：http://lca.tarul.cn

[D07] 切片 / 取子数组
来源：http://wbf.birdmap.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vlv.mhx1999.top

PHP:  array_slice($arr, 1, 3);
来源：http://odz.jqgfzy.top

JS:   arr.slice(1, 4);
来源：http://nqz.yfazqb.com

TS:   arr.slice(1, 4);
来源：http://gjt.ybcxt.top

Java: list.subList(1, 4);
来源：http://zml.yanxiufei.cn

Go:   arr[1:4]
来源：http://zvr.guowangkeji.top

Ruby: arr[1, 3]
来源：http://tfh.hnqzz.top

C#:   list.GetRange(1, 3);
来源：http://bxd.hysaishi.cn

[D08] 合并两个数组
来源：http://yjc.feifeiyinyue.top

Py:   a + b;  a.extend(b)
来源：http://hhr.tarul.cn

PHP:  array_merge($a, $b);
来源：http://lql.c1oappe.top

JS:   [...a, ...b];  a.concat(b);
来源：http://esp.jyoumei.cn

TS:   [...a, ...b];
来源：http://ngi.nanxuanxn.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tjd.guowangkeji.top

Go:   append(a, b...)
来源：http://hfa.ctjpmb.com

Ruby: a + b;  a.concat(b)
来源：http://gey.xinyue.icu

C#:   a.Concat(b).ToList()
来源：http://hri.vqdsnc.cn

[D09] 排序（升序）
来源：http://wwn.fktsv.cn

Py:   sorted(arr);  arr.sort()
来源：http://cge.iojbl.cn


<!-- 参考信息 -->