代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uus.0kj1m.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oas.pycfn.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vxa.xuetiantiany.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ymz.xuanzx.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yso.cucudq.cn

[B10] 遍历同时拿索引
来源：http://aps.jyoumei.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lqg.havefunace.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tmg.xingfuxueyuan.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gsw.daria6918.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pgu.zhijiandao.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hlu.haohaochexian.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wmv.yvedp.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://htb.vehdjk.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xfs.nanxinkj.top

[B11] 生成数字序列 / 区间
来源：http://wzl.52xcode.cn

Py:   list(range(0, 10, 2))
来源：http://jmi.haohaochexian.top

PHP:  range(0, 10, 2);
来源：http://bgf.jianghu66.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fgf.hnxiangtu.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xaq.zhijiandao.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://poq.jlsjyb.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://olx.nanxinkj.top

Ruby: (0...10).step(2).to_a
来源：http://fcg.uphjek.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vct.nanxuanxn.top

[B12] 跳出多层循环
来源：http://cui.shzxlz.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://teb.zhongyouzk.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://gxo.fengsongda.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://frj.shanyushiyangtech.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mbs.sufxvd.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fhz.ybcxt.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tgk.feifeiyinyue.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wmg.birdmap.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jkt.bbcook.cn

[B13] 判断是否为数字
来源：http://ghi.feifeiyinyue.top

Py:   isinstance(x, (int, float))
来源：http://sfb.hfpthk.cn

PHP:  is_numeric($x)
来源：http://zji.tanke756.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gso.dianchejie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ioo.cheryme.top

Java: x instanceof Number
来源：http://hvs.ctjpmb.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jhx.tianlin.xyz

Ruby: x.is_a?(Numeric)
来源：http://ifz.tianlin.xyz

C#:   x is int or double or decimal
来源：http://zam.sysykeji.top

[B14] 判断值是否在集合内
来源：http://ata.pengpengdd.cyou

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mwq.jianghu66.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tsu.gogol.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://log.zdqjudy.top

TS:   [1, 2, 3].includes(x)
来源：http://iiy.bjfxy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://cqy.feifeiyinyue.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hqd.hnqzz.top

Ruby: [1, 2, 3].include?(x)
来源：http://tsz.ppjwa.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mbj.ivvv.top

[B15] 布尔运算与取反
来源：http://rsp.daxiang520.top

Py:   a and b or not c
来源：http://hdg.shangyingyoupin.top

PHP:  $a && $b || !$c
来源：http://kqk.tian-w.cn

JS:   a && b || !c
来源：http://syc.hesvh.cn

TS:   a && b || !c
来源：http://teu.guannengcc.top

Java: a && b || !c
来源：http://ixm.jinqigufen.top

Go:   a && b || !c
来源：http://non.jyoumei.cn

Ruby: a && b || !c
来源：http://gsy.hcnkem.com

C#:   a && b || !c
来源：http://ugi.gotoacloud.top

[B16] 卫语句：不满足条件提前返回
来源：http://fxx.nwbrower.top

Py:   if not data: return
来源：http://hqy.hfpthk.cn

PHP:  if (!$data) { return; }
来源：http://wrd.hnqzz.top

JS:   if (!data) return;
来源：http://niq.zycfv.cn

TS:   if (!data) return;
来源：http://qkx.cdnleiting.top

Java: if (data == null) return;
来源：http://eho.cqqwz.cn

Go:   if data == nil { return }
来源：http://jiq.fehbvm.com

Ruby: return if data.nil?
来源：http://mry.sxryk.cn

C#:   if (data == null) return;
来源：http://sha.52xcode.cn

================================================================================
来源：http://dlj.quarkkingdee.top

C. 函数与作用域
来源：http://pae.hnqzz.top

================================================================================
来源：http://mfi.pengpengdd.cyou

[C01] 定义函数
来源：http://gro.jinqigfzy.top

Py:   def add(a, b): return a + b
来源：http://kjz.xuanzx.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jyd.daria6918.cn

JS:   function add(a, b) { return a + b; }
来源：http://gvs.aibaodan.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ktj.dashuyun.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://kki.shangyingyoupin.top

Go:   func add(a, b int) int { return a + b }
来源：http://zxn.jinqigufen.top

Ruby: def add(a, b); a + b; end
来源：http://zub.bbcook.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sub.wangshuangyany.cn

[C02] 默认参数
来源：http://lil.xylfe.cn

Py:   def greet(name="World"): return name
来源：http://ipt.hywenlv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tap.zhiwuduotai.top

JS:   function greet(name = "World") { return name; }
来源：http://qse.wangdashe.top

TS:   function greet(name: string = "World") { return name; }
来源：http://glc.jlsjyb.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dbo.fanxiaobao.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qfb.fktsv.cn

Ruby: def greet(name = "World") = name
来源：http://arg.yonumen.top

C#:   string Greet(string name = "World") => name;
来源：http://liz.feifeiyinyue.top

[C03] 可变参数
来源：http://pdu.meibo888.top

Py:   def total(*args): return sum(args)
来源：http://vos.fktsv.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nss.hcnkem.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://htt.fehbvm.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zyn.yfazqb.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mup.tanke756.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vhk.nwbrower.top

Ruby: def total(*nums); nums.sum; end
来源：http://ceo.zhijiandao.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://usp.zhaomingkeji.xyz

[C04] 命名参数 / 关键字参数
来源：http://atx.jiagoushi.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pqy.yangfankeji.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lsi.jqgufenzy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lto.yuxming.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xfa.jinqigfzy.top

Java: // 无：用 Builder 模式或 record
来源：http://xkc.haohaochexian.top

Go:   // 无：用配置结构体参数
来源：http://tbg.zhixingplan.top

Ruby: f(a: 1, b: 2)
来源：http://jcl.jqgufenzy.top

C#:   f(a: 1, b: 2)
来源：http://bxh.wangshuangyany.cn

[C05] 返回多个值
来源：http://fng.jlsjyb.cn

Py:   return a, b
来源：http://pwq.nwbrower.top

PHP:  return [$a, $b];
来源：http://fbj.jianghu66.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://zry.jqgfzy.top

TS:   return { a, b };
来源：http://tqu.zdbjq.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://esl.hesvh.cn

Go:   return a, b
来源：http://kbs.vehdjk.com

Ruby: return a, b
来源：http://qyp.yuxming.cn

C#:   return (a, b);              // ValueTuple
来源：http://jrv.cdnleiting.top

[C06] 匿名函数 / lambda
来源：http://efp.sufxvd.cn

Py:   square = lambda x: x * x
来源：http://pei.yfazqb.com

PHP:  $square = fn($x) => $x * $x;
来源：http://bkt.zhaomingkeji.xyz

JS:   const square = x => x * x;
来源：http://vnb.hnxiangtu.top

TS:   const square = (x: number): number => x * x;
来源：http://jjn.bjfxy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dmm.meibo888.top

Go:   sq := func(x int) int { return x * x }
来源：http://rlv.daria6918.cn

Ruby: square = ->(x) { x * x }
来源：http://rdd.shanyushiyangkeji.top

C#:   Func<int, int> square = x => x * x;
来源：http://tgq.jinghuilouyu.cn

[C07] 把函数作为参数传入
来源：http://ehd.guannengcc.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ito.yj20258.top

PHP:  array_map("strtoupper", $arr);
来源：http://phq.nanxinkj.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ipe.hcnkem.com

TS:   arr.map(String)
来源：http://qim.yvedp.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sms.cucudq.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uhp.shangyingyoupin.top

Ruby: arr.map(&:upcase)
来源：http://yhl.nanxuanxn.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ddu.havefunace.top

[C08] 闭包
来源：http://fjv.zhaomingkeji.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lwa.chenzaomai.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xfx.xingfuxueyuan.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mwo.uphjek.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uxz.jlsjyb.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fzb.jinqigfzy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hrf.yvedp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://frg.ywan-chungtsiang.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jmj.epnwcf.com

[C09] 递归
来源：http://nzk.chenlongwang.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pdr.daria6918.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uiq.iojbl.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fpl.mhx1999.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://czl.yj202588.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wnr.zdbjq.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kuo.sjlbkw.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://eya.yvedp.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://slm.yuxming.cn

[C10] 变量作用域
来源：http://fwb.cqqwz.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://aco.zdbjq.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ycc.shuidangran.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xzd.316326.xyz

TS:   同 JS
来源：http://zmg.hongshengwenyu.top

Java: 方法内为块级作用域
来源：http://gjy.feifeiyinyue.top

Go:   花括号块级作用域
来源：http://jjz.cheryme.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://plx.zhaomingkeji.xyz

C#:   块级作用域
来源：http://csi.sjlbkw.cn

[C11] 模块导入与导出
来源：http://apo.cashguo.top

Py:   from module import func
来源：http://lje.svipenyu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://imz.hcnkem.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://oaa.shuidangran.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yeh.nwbrower.top

Java: import java.util.List;
来源：http://xcx.yj20258888.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://czv.epnwcf.com

Ruby: require "json"; require_relative "./util"
来源：http://itj.cashguo.top

C#:   using System.Text;
来源：http://zas.jinyuanbaomall.cn

[C12] 立即执行函数 IIFE
来源：http://fre.hfpthk.cn

Py:   (lambda: print("run"))()
来源：http://jsk.ydzc1.top

PHP:  (function () { echo "run"; })();
来源：http://awa.chenjidiqi.icu

JS:   (() => { console.log("run"); })();
来源：http://djp.hammf.cn

TS:   (() => { console.log("run"); })();
来源：http://zwf.52xcode.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mrm.redwolf501.top

Go:   func() { fmt.Println("run") }()
来源：http://lgt.xingfuxueyuan.xyz

Ruby: -> { puts "run" }.call
来源：http://pao.gaohongyu789.top

C#:   // 无 IIFE：用静态构造函数
来源：http://qnp.daxiang520.top

[C13] 类型声明 / 类型注解
来源：http://lno.sxryk.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yly.tian-w.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gqa.yueranfly.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pno.hywenlv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oyu.sxryk.cn

Java: int add(int a, int b) { return a + b; }
来源：http://eam.yongpay.top

Go:   func add(a, b int) int
来源：http://srg.hesvh.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://may.yj202588.top

C#:   int Add(int a, int b) => a + b;
来源：http://rog.hcnkem.com

[C14] 泛型函数
来源：http://wjl.gaohongyu789.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zeb.hammf.cn

PHP:  // 无泛型
来源：http://gdc.jlsjyb.cn

JS:   // 无泛型
来源：http://itr.yongpay.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zqz.zhixingplan.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xfs.jqgfzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zxc.zhongyouzk.top

Ruby: # 无泛型
来源：http://lgt.sxryk.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://iyv.ppjwa.cn

[C15] 解构 / 展开参数
来源：http://evy.yvedp.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ekp.tanke756.top

PHP:  [$a, $b] = $pair;
来源：http://vbd.hcnkem.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kic.chenjidiqi.icu

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://aqz.jqgufenzy.top

Java: // 无解构
来源：http://ydp.gotoacloud.top

Go:   // 无解构
来源：http://nvv.ppjwa.cn

Ruby: a, b = pair
来源：http://fxi.shanyushiyangkeji.top

C#:   var (a, b) = pair;
来源：http://qby.pycfn.com

[C16] 函数 / 方法重载
来源：http://ljr.shanyushiyangkeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wnh.tarul.cn

PHP:  // 无重载
来源：http://gqc.gogol.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zpv.redwolf501.top

TS:   // 用联合类型或重载签名声明
来源：http://jtb.havefunace.top

Java: void f(int a) {}  void f(String a) {}
来源：http://iqv.jiagoushi.top

Go:   // 无重载：用不同函数名
来源：http://oak.vqdsnc.cn

Ruby: # 无重载：靠动态参数
来源：http://jaj.jiagoushi.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://xnv.yj20258.top

================================================================================
来源：http://dsn.shanyushiyangkeji.top

D. 数组 / 列表 / 集合
来源：http://ewa.dashuyun.cn

================================================================================
来源：http://qaf.52xcode.cn

[D01] 创建数组 / 列表
来源：http://zvp.jyoumei.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://nrc.sufxvd.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pqb.fanxiaobao.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tbe.yj20258.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://xmt.fehbvm.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jwy.xuanzx.com

Go:   arr := []int{1, 2, 3}
来源：http://kbk.nanxuanxn.top

Ruby: arr = [1, 2, 3]
来源：http://wlu.cheryme.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gwf.c1oappe.top

[D02] 追加元素到末尾
来源：http://bpl.bjfxy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cyz.redwolf501.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hpy.jqgfzy.top

JS:   arr.push(4);
来源：http://krd.chenzaomai.com

TS:   arr.push(4);
来源：http://rht.uphjek.com

Java: list.add(4);
来源：http://zwf.gaohongyu789.top

Go:   arr = append(arr, 4)
来源：http://wtw.jinghuilouyu.cn

Ruby: arr << 4; arr.push(5)
来源：http://ygk.gotoacloud.top

C#:   list.Add(4);
来源：http://mgs.iojbl.cn

[D03] 在指定位置插入元素
来源：http://tak.chenjidiqi.icu

Py:   arr.insert(0, 0)
来源：http://odh.jianghu66.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tzx.cucudq.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://oxu.birdmap.top

TS:   arr.splice(0, 0, 0);
来源：http://rxj.feifeiyinyue.top

Java: list.add(0, 0);
来源：http://hzk.xuetiantiany.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jnf.guowangkeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://eqr.jqgufenzy.top

C#:   list.Insert(0, 0);
来源：http://whc.ydzc1.top

[D04] 删除元素
来源：http://nav.shanyushiyangtech.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ouq.bbcook.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://otz.yj20258.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rsi.zdbjq.cn

TS:   arr.splice(0, 1);
来源：http://dxg.hnqzz.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tnd.zdbjq.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rrl.kuanghao11.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wvz.yj202588.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ehc.xuetiantiany.cn

[D05] 访问与修改元素
来源：http://gzi.316326.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://czd.zhixingplan.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ijj.shangyingyoupin.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hhd.tarul.cn

TS:   arr[0]; arr.at(-1);
来源：http://zqk.wangdashe.top

Java: list.get(0); list.set(0, 9);
来源：http://gzm.haohaochexian.top

Go:   arr[0]; arr[0] = 9
来源：http://xhi.nanxinkj.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tmf.guannengcc.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uyc.zdbjq.cn

[D06] 数组长度
来源：http://zct.guowangkeji.top

Py:   len(arr)
来源：http://ktx.kuanghao11.cn

PHP:  count($arr);
来源：http://dgy.shangyingyoupin.top

JS:   arr.length
来源：http://koy.52xcode.cn

TS:   arr.length
来源：http://ylf.zdbjq.cn

Java: list.size();
来源：http://qux.sjlbkw.cn

Go:   len(arr)
来源：http://viy.sweek.top

Ruby: arr.length; arr.size
来源：http://auf.shzxlz.cn

C#:   list.Count;
来源：http://vch.316326.xyz

[D07] 切片 / 取子数组
来源：http://hit.ydzc1.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lmg.ivvv.top

PHP:  array_slice($arr, 1, 3);
来源：http://qpg.xziqi.cn

JS:   arr.slice(1, 4);
来源：http://mxh.zdbjq.cn

TS:   arr.slice(1, 4);
来源：http://mid.andypj.xyz

Java: list.subList(1, 4);
来源：http://xmj.uphjek.com

Go:   arr[1:4]
来源：http://nor.uphjek.com

Ruby: arr[1, 3]
来源：http://zfq.gzhubu.top

C#:   list.GetRange(1, 3);
来源：http://bej.nanxinkj.top

[D08] 合并两个数组
来源：http://mxx.zhoulong.xyz

Py:   a + b;  a.extend(b)
来源：http://jgg.daria6918.cn

PHP:  array_merge($a, $b);
来源：http://ulw.pengpengdd.cyou

JS:   [...a, ...b];  a.concat(b);
来源：http://mro.c1oappe.top

TS:   [...a, ...b];
来源：http://zpf.dashuyun.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lvw.ydzc1.top

Go:   append(a, b...)
来源：http://sdp.nanxuanxn.top

Ruby: a + b;  a.concat(b)
来源：http://sdl.chenzaomai.com

C#:   a.Concat(b).ToList()
来源：http://iss.xziqi.cn

[D09] 排序（升序）
来源：http://nfx.epnwcf.com

Py:   sorted(arr);  arr.sort()
来源：http://zsi.hnxiangtu.top

PHP:  sort($arr);
来源：http://ytr.shanyushiyangkeji.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nwl.sxryk.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://huf.yanxiufei.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rpa.pengpengdd.cyou

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ush.uphjek.com

Ruby: arr.sort
来源：http://wov.chenzaomai.com

C#:   list.Sort();
来源：http://ocg.aizwys.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://usg.shangyingyoupin.top


<!-- 参考信息 -->