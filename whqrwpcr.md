代发 wailian999

[B09] break 与 continue
来源：http://hqf.mhx1999.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vfn.fktsv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lyk.yj20258888.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uok.zhongyouzk.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tqx.pycfn.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ivl.quarkkingdee.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qvl.pengpengdd.cyou

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bco.zhiwuduotai.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qcf.vqdsnc.cn

[B10] 遍历同时拿索引
来源：http://haf.haohaochexian.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vsm.zhixingplan.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hys.zhijiandao.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mac.yj20258888.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hdo.svipenyu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jpd.52xcode.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://aju.cucudq.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://max.316326.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://opb.wangdashe.top

[B11] 生成数字序列 / 区间
来源：http://lhm.zdqjudy.top

Py:   list(range(0, 10, 2))
来源：http://flg.jianghu66.top

PHP:  range(0, 10, 2);
来源：http://dyg.0kj1m.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ysi.zhiwuduotai.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nvm.sxryk.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://aoi.jyoumei.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pfa.zhaomingkeji.xyz

Ruby: (0...10).step(2).to_a
来源：http://oon.yj20258.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rnn.tanke756.top

[B12] 跳出多层循环
来源：http://ktf.zycfv.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://elp.chenlongwang.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://rqo.fanxiaobao.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lej.andypj.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pll.gaohongyu789.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://awp.shanyushiyangtech.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ffv.yuanzhike.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://igf.xuetiantiany.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cuc.ywan-chungtsiang.top

[B13] 判断是否为数字
来源：http://owd.xingfuxueyuan.xyz

Py:   isinstance(x, (int, float))
来源：http://gni.hysaishi.cn

PHP:  is_numeric($x)
来源：http://bsv.guannengcc.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pev.dashuyun.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aeq.xylfe.cn

Java: x instanceof Number
来源：http://rhn.jiagoushi.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qtv.zhiwuduotai.top

Ruby: x.is_a?(Numeric)
来源：http://kuh.xylfe.cn

C#:   x is int or double or decimal
来源：http://ukx.fzhhl.top

[B14] 判断值是否在集合内
来源：http://koc.fanxiaobao.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jer.gzhubu.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bmk.zdqjudy.top

JS:   [1, 2, 3].includes(x)
来源：http://ske.gogol.net.cn

TS:   [1, 2, 3].includes(x)
来源：http://zvb.zhaomingkeji.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://xpt.dashuyun.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ssb.aibaodan.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mvf.shuidangran.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ker.zhongyouzk.top

[B15] 布尔运算与取反
来源：http://agu.yonumen.top

Py:   a and b or not c
来源：http://vep.cucudq.cn

PHP:  $a && $b || !$c
来源：http://igo.zdbjq.cn

JS:   a && b || !c
来源：http://czc.cheryme.top

TS:   a && b || !c
来源：http://mfi.shuidangran.top

Java: a && b || !c
来源：http://fox.gogol.net.cn

Go:   a && b || !c
来源：http://nov.jlsjyb.cn

Ruby: a && b || !c
来源：http://ebe.yj20258888.top

C#:   a && b || !c
来源：http://uiy.jqgfzy.top

[B16] 卫语句：不满足条件提前返回
来源：http://nbm.tian-w.cn

Py:   if not data: return
来源：http://ygl.tian-w.cn

PHP:  if (!$data) { return; }
来源：http://ibo.tianlin.xyz

JS:   if (!data) return;
来源：http://eua.cqqwz.cn

TS:   if (!data) return;
来源：http://har.uphjek.com

Java: if (data == null) return;
来源：http://xqq.vehdjk.com

Go:   if data == nil { return }
来源：http://puq.yanxiufei.cn

Ruby: return if data.nil?
来源：http://yzt.pengpengdd.cyou

C#:   if (data == null) return;
来源：http://pht.jinqigufen.top

================================================================================
来源：http://yty.sufxvd.cn

C. 函数与作用域
来源：http://ipk.ydzc1.top

================================================================================
来源：http://ymj.ppjwa.cn

[C01] 定义函数
来源：http://eoq.hywenlv.cn

Py:   def add(a, b): return a + b
来源：http://xeq.zhaomingkeji.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zgu.shuidangran.top

JS:   function add(a, b) { return a + b; }
来源：http://wtg.mhx1999.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dhp.meibo888.top

Java: static int add(int a, int b) { return a + b; }
来源：http://vap.zycfv.cn

Go:   func add(a, b int) int { return a + b }
来源：http://spx.cdnleiting.top

Ruby: def add(a, b); a + b; end
来源：http://sas.iojbl.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wpj.xingfuxueyuan.xyz

[C02] 默认参数
来源：http://zhz.xylfe.cn

Py:   def greet(name="World"): return name
来源：http://pno.jinghuilouyu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ugv.yuanzhike.top

JS:   function greet(name = "World") { return name; }
来源：http://dig.tanke756.top

TS:   function greet(name: string = "World") { return name; }
来源：http://xdj.fzhhl.top

Java: // 无默认参数：方法重载或 Optional
来源：http://woc.zhiwuduotai.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hae.sxryk.cn

Ruby: def greet(name = "World") = name
来源：http://nqg.xinyue.icu

C#:   string Greet(string name = "World") => name;
来源：http://jih.shzxlz.cn

[C03] 可变参数
来源：http://rmv.havefunace.top

Py:   def total(*args): return sum(args)
来源：http://kcv.dashuyun.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rlq.hysaishi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yhi.aizwys.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zfk.fzhhl.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rjd.fktsv.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sef.9152youxi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://aao.jianghu66.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xww.gotoacloud.top

[C04] 命名参数 / 关键字参数
来源：http://krc.vqdsnc.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mxe.ehwqpu.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pgb.ivvv.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cnc.52xcode.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xut.jlsjyb.cn

Java: // 无：用 Builder 模式或 record
来源：http://rxl.aizwys.cn

Go:   // 无：用配置结构体参数
来源：http://cjs.hnqzz.top

Ruby: f(a: 1, b: 2)
来源：http://chd.gaohongyu789.top

C#:   f(a: 1, b: 2)
来源：http://bze.epnwcf.com

[C05] 返回多个值
来源：http://mpv.cucudq.cn

Py:   return a, b
来源：http://huz.ydjk.org.cn

PHP:  return [$a, $b];
来源：http://jnn.yj202588.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://lvc.c1oappe.top

TS:   return { a, b };
来源：http://yax.daria6918.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://uay.wangdashe.top

Go:   return a, b
来源：http://okr.yj20258.top

Ruby: return a, b
来源：http://jcd.yj20258.top

C#:   return (a, b);              // ValueTuple
来源：http://jjv.nwbrower.top

[C06] 匿名函数 / lambda
来源：http://ose.hnqzz.top

Py:   square = lambda x: x * x
来源：http://dis.ivvv.top

PHP:  $square = fn($x) => $x * $x;
来源：http://zps.nanxuanxn.top

JS:   const square = x => x * x;
来源：http://qpl.yfazqb.com

TS:   const square = (x: number): number => x * x;
来源：http://wko.pycfn.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nkp.ydjk.org.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gzl.zhongyouzk.top

Ruby: square = ->(x) { x * x }
来源：http://qfa.jlsjyb.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hpw.fengsongda.top

[C07] 把函数作为参数传入
来源：http://zzu.xylfe.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ruz.chenjidiqi.icu

PHP:  array_map("strtoupper", $arr);
来源：http://vfv.daxiang520.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hci.nwbrower.top

TS:   arr.map(String)
来源：http://pef.yangfankeji.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ydx.hnxiangtu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ben.cucudq.cn

Ruby: arr.map(&:upcase)
来源：http://itp.ydjk.org.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://bim.0kj1m.cn

[C08] 闭包
来源：http://sgx.haohaochexian.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fea.snrcjt.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wny.zhixingplan.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ajm.jqgufenzy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cpk.cqqwz.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vui.tian-w.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zjl.ybcxt.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://noj.52xcode.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://eeh.xuetiantiany.cn

[C09] 递归
来源：http://alb.fengsongda.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dwr.hywenlv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vbp.fzhhl.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hao.sweek.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sfa.gaohongyu789.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tax.hesvh.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hlk.yonumen.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hzp.jqgufenzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xsa.316326.xyz

[C10] 变量作用域
来源：http://xah.sweek.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cwy.ehwqpu.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://icx.havefunace.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nbz.yj20258.top

TS:   同 JS
来源：http://fdr.tianlin.xyz

Java: 方法内为块级作用域
来源：http://zlx.feifeiyinyue.top

Go:   花括号块级作用域
来源：http://wyj.xziqi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xrt.ydjk.org.cn

C#:   块级作用域
来源：http://mqh.cqqwz.cn

[C11] 模块导入与导出
来源：http://tjj.zycfv.cn

Py:   from module import func
来源：http://img.yongpay.top

PHP:  require "file.php";  或 use App\Service;
来源：http://tmj.dashuyun.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://elp.tanke756.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jib.shzxlz.cn

Java: import java.util.List;
来源：http://lkp.sufxvd.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dxn.vehdjk.com

Ruby: require "json"; require_relative "./util"
来源：http://ago.xinyue.icu

C#:   using System.Text;
来源：http://mct.guowangkeji.top

[C12] 立即执行函数 IIFE
来源：http://lbw.9152youxi.cn

Py:   (lambda: print("run"))()
来源：http://hoc.cucudq.cn

PHP:  (function () { echo "run"; })();
来源：http://nwy.tianlin.xyz

JS:   (() => { console.log("run"); })();
来源：http://bfi.yj20258888.top

TS:   (() => { console.log("run"); })();
来源：http://eed.shanyushiyangtech.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rue.gotoacloud.top

Go:   func() { fmt.Println("run") }()
来源：http://sol.hammf.cn

Ruby: -> { puts "run" }.call
来源：http://pjh.jinqigufen.top

C#:   // 无 IIFE：用静态构造函数
来源：http://vnv.shangyingyoupin.top

[C13] 类型声明 / 类型注解
来源：http://kpx.ydjk.org.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fsd.tian-w.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vin.fanxiaobao.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pex.xuanzx.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nuj.jlsjyb.cn

Java: int add(int a, int b) { return a + b; }
来源：http://csx.fzhhl.top

Go:   func add(a, b int) int
来源：http://agg.hcnkem.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://olw.sufxvd.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ddb.tarul.cn

[C14] 泛型函数
来源：http://qjz.jqgfzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pmt.yongpay.top

PHP:  // 无泛型
来源：http://dyr.kuanghao11.cn

JS:   // 无泛型
来源：http://hlu.tanke756.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qzr.xinyue.icu

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zuf.hfpthk.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://iaw.c1oappe.top

Ruby: # 无泛型
来源：http://qeb.yanxiufei.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sff.zhiwuduotai.top

[C15] 解构 / 展开参数
来源：http://qfu.vehdjk.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kcw.pengpengdd.cyou

PHP:  [$a, $b] = $pair;
来源：http://kqp.tarul.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fnz.pycfn.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bxt.0kj1m.cn

Java: // 无解构
来源：http://lnw.yanxiufei.cn

Go:   // 无解构
来源：http://mls.bjfxy.top

Ruby: a, b = pair
来源：http://fhu.xingfuxueyuan.xyz

C#:   var (a, b) = pair;
来源：http://tum.0kj1m.cn

[C16] 函数 / 方法重载
来源：http://dnd.pengpengdd.cyou

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wkm.xylfe.cn

PHP:  // 无重载
来源：http://dug.tarul.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://vxs.jinqigufen.top

TS:   // 用联合类型或重载签名声明
来源：http://wbo.shuidangran.top

Java: void f(int a) {}  void f(String a) {}
来源：http://msf.nwbrower.top

Go:   // 无重载：用不同函数名
来源：http://cdt.0kj1m.cn

Ruby: # 无重载：靠动态参数
来源：http://mow.yuxming.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rld.yonumen.top

================================================================================
来源：http://xrc.pengpengdd.cyou

D. 数组 / 列表 / 集合
来源：http://wpb.epnwcf.com

================================================================================
来源：http://gqg.yanxiufei.cn

[D01] 创建数组 / 列表
来源：http://ard.jinqigufen.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://bvl.pycfn.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mth.hfpthk.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wkk.yuanzhike.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://lgd.zhengqikj.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jsq.hammf.cn

Go:   arr := []int{1, 2, 3}
来源：http://nta.yfazqb.com

Ruby: arr = [1, 2, 3]
来源：http://tgs.pengpengdd.cyou

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vak.daria6918.cn

[D02] 追加元素到末尾
来源：http://sbc.gzhubu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://euk.shzxlz.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://eoq.gotoacloud.top

JS:   arr.push(4);
来源：http://npc.uphjek.com

TS:   arr.push(4);
来源：http://yaq.jinyuanbaomall.cn

Java: list.add(4);
来源：http://ypd.chenzaomai.com

Go:   arr = append(arr, 4)
来源：http://chr.nanxuanxn.top

Ruby: arr << 4; arr.push(5)
来源：http://ezr.xinyue.icu

C#:   list.Add(4);
来源：http://yhg.yuanzhike.top

[D03] 在指定位置插入元素
来源：http://mwo.zhoulong.xyz

Py:   arr.insert(0, 0)
来源：http://kcb.yonumen.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ysz.fzhhl.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gcr.mhx1999.top

TS:   arr.splice(0, 0, 0);
来源：http://ysl.sysykeji.top

Java: list.add(0, 0);
来源：http://lak.xuanzx.com

Go:   arr = append([]int{0}, arr...)
来源：http://cjq.epnwcf.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://axr.shuidangran.top

C#:   list.Insert(0, 0);
来源：http://wci.yueranfly.top

[D04] 删除元素
来源：http://rer.tianlin.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uqz.smart0.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xuq.chenzaomai.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ses.shuidangran.top

TS:   arr.splice(0, 1);
来源：http://ejn.shuidangran.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rbu.0kj1m.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://slo.vqdsnc.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bbm.hammf.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mil.zhongyouzk.top

[D05] 访问与修改元素
来源：http://avw.aizwys.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tyz.xingfuxueyuan.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hlw.zhijiandao.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wad.jqgufenzy.top

TS:   arr[0]; arr.at(-1);
来源：http://ont.yj20258.top

Java: list.get(0); list.set(0, 9);
来源：http://upg.ctjpmb.com

Go:   arr[0]; arr[0] = 9
来源：http://eth.hnqzz.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://iwu.nanxinkj.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ifx.jqgfzy.top

[D06] 数组长度
来源：http://hhd.0kj1m.cn

Py:   len(arr)
来源：http://czk.9152youxi.cn

PHP:  count($arr);
来源：http://onc.9152youxi.cn

JS:   arr.length
来源：http://lnp.fzhhl.top

TS:   arr.length
来源：http://uck.zycfv.cn

Java: list.size();
来源：http://nnw.hysaishi.cn

Go:   len(arr)
来源：http://yez.smart0.xyz

Ruby: arr.length; arr.size
来源：http://goy.yfazqb.com

C#:   list.Count;
来源：http://ivu.yanxiufei.cn

[D07] 切片 / 取子数组
来源：http://akd.hnqzz.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mxu.yfazqb.com

PHP:  array_slice($arr, 1, 3);
来源：http://faz.xylfe.cn

JS:   arr.slice(1, 4);
来源：http://xsc.meibo888.top

TS:   arr.slice(1, 4);
来源：http://myu.fzhhl.top

Java: list.subList(1, 4);
来源：http://rgs.dashuyun.cn

Go:   arr[1:4]
来源：http://vks.vehdjk.com

Ruby: arr[1, 3]
来源：http://lbe.tianlin.xyz

C#:   list.GetRange(1, 3);
来源：http://bhz.hfpthk.cn

[D08] 合并两个数组
来源：http://lrx.gaohongyu789.top

Py:   a + b;  a.extend(b)
来源：http://glc.sxryk.cn

PHP:  array_merge($a, $b);
来源：http://vcy.meibo888.top

JS:   [...a, ...b];  a.concat(b);
来源：http://tmw.0kj1m.cn

TS:   [...a, ...b];
来源：http://lqs.tian-w.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qtm.sjlbkw.cn

Go:   append(a, b...)
来源：http://zjt.fengsongda.top

Ruby: a + b;  a.concat(b)
来源：http://vjq.ivvv.top

C#:   a.Concat(b).ToList()
来源：http://khj.ywan-chungtsiang.top

[D09] 排序（升序）
来源：http://kbx.xylfe.cn

Py:   sorted(arr);  arr.sort()
来源：http://wwk.52xcode.cn

PHP:  sort($arr);
来源：http://rha.ybcxt.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://feu.cheryme.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://yee.yueranfly.top

Java: Collections.sort(list);  list.sort(null);
来源：http://pen.cashguo.top


<!-- 参考信息 -->