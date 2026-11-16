代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://haj.yj20258888.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ttl.yonumen.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mxu.316326.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ocv.yfazqb.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tsu.yuxming.cn

[B10] 遍历同时拿索引
来源：http://gjz.mhx1999.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mpl.zdbjq.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lwo.dashuyun.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uqg.ydzc1.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://why.fzhhl.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wcw.0kj1m.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://obl.ywan-chungtsiang.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://grb.zhijiandao.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hyk.ppjwa.cn

[B11] 生成数字序列 / 区间
来源：http://ipe.redwolf501.top

Py:   list(range(0, 10, 2))
来源：http://lex.cheryme.top

PHP:  range(0, 10, 2);
来源：http://twa.pycfn.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vaf.dianchejie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aew.xingfuxueyuan.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ydc.52xcode.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dir.xuetiantiany.cn

Ruby: (0...10).step(2).to_a
来源：http://wam.birdmap.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gen.aibaodan.cn

[B12] 跳出多层循环
来源：http://hbh.bjfxy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://pxv.zdqjudy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ytf.ctjpmb.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wex.fehbvm.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dvt.sufxvd.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bfg.fzhhl.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jsr.yvedp.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wdc.52xcode.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jse.gogol.net.cn

[B13] 判断是否为数字
来源：http://ocf.jlsjyb.cn

Py:   isinstance(x, (int, float))
来源：http://upx.xziqi.cn

PHP:  is_numeric($x)
来源：http://rmp.vehdjk.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://azq.xylfe.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pks.0kj1m.cn

Java: x instanceof Number
来源：http://fzk.shanyushiyangtech.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dxb.meibo888.top

Ruby: x.is_a?(Numeric)
来源：http://elm.xinyue.icu

C#:   x is int or double or decimal
来源：http://trg.zhoulong.xyz

[B14] 判断值是否在集合内
来源：http://njn.0kj1m.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qkz.yanxiufei.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pfj.gaohongyu789.top

JS:   [1, 2, 3].includes(x)
来源：http://atz.yangfankeji.com

TS:   [1, 2, 3].includes(x)
来源：http://oie.haohaochexian.top

Java: List.of(1, 2, 3).contains(x)
来源：http://zsv.cashguo.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tzs.andypj.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://gsz.fktsv.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ccr.daria6918.cn

[B15] 布尔运算与取反
来源：http://nqp.tanke756.top

Py:   a and b or not c
来源：http://foh.ivvv.top

PHP:  $a && $b || !$c
来源：http://vvd.daria6918.cn

JS:   a && b || !c
来源：http://jnd.fengsongda.top

TS:   a && b || !c
来源：http://kpt.yuanzhike.top

Java: a && b || !c
来源：http://aov.xziqi.cn

Go:   a && b || !c
来源：http://pda.snrcjt.cn

Ruby: a && b || !c
来源：http://rpf.haohaochexian.top

C#:   a && b || !c
来源：http://ahe.ctjpmb.com

[B16] 卫语句：不满足条件提前返回
来源：http://bmr.jlsjyb.cn

Py:   if not data: return
来源：http://qrd.hammf.cn

PHP:  if (!$data) { return; }
来源：http://uxf.sysykeji.top

JS:   if (!data) return;
来源：http://mlp.yuanzhike.top

TS:   if (!data) return;
来源：http://ozi.hfpthk.cn

Java: if (data == null) return;
来源：http://evn.hysaishi.cn

Go:   if data == nil { return }
来源：http://dpy.zhaomingkeji.xyz

Ruby: return if data.nil?
来源：http://qfy.sweek.top

C#:   if (data == null) return;
来源：http://cvu.ydzc1.top

================================================================================
来源：http://syf.bjfxy.top

C. 函数与作用域
来源：http://cdj.chenjidiqi.icu

================================================================================
来源：http://iau.xuanzx.com

[C01] 定义函数
来源：http://qfh.hysaishi.cn

Py:   def add(a, b): return a + b
来源：http://seh.zdbjq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gwq.shzxlz.cn

JS:   function add(a, b) { return a + b; }
来源：http://obq.xingfuxueyuan.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://efn.iojbl.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mjx.zhoulong.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://vls.xuanzx.com

Ruby: def add(a, b); a + b; end
来源：http://ogm.hnqzz.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bqf.zhoulong.xyz

[C02] 默认参数
来源：http://ime.shzxlz.cn

Py:   def greet(name="World"): return name
来源：http://arj.shanyushiyangkeji.top

PHP:  function greet($name = "World") { return $name; }
来源：http://vxp.316326.xyz

JS:   function greet(name = "World") { return name; }
来源：http://gij.cucudq.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mme.shangyingyoupin.top

Java: // 无默认参数：方法重载或 Optional
来源：http://msj.ybcxt.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wae.yanxiufei.cn

Ruby: def greet(name = "World") = name
来源：http://jzf.ydzc1.top

C#:   string Greet(string name = "World") => name;
来源：http://lrq.ehwqpu.com

[C03] 可变参数
来源：http://jih.bjfxy.top

Py:   def total(*args): return sum(args)
来源：http://mpb.tanke756.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xhu.52xcode.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hjo.cashguo.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ofs.fehbvm.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fzp.yongpay.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kfi.aizwys.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hoe.jqgfzy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://iro.meibo888.top

[C04] 命名参数 / 关键字参数
来源：http://kuy.nanxinkj.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://whx.tianlin.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mkm.wangdashe.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://abb.9152youxi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mtq.tian-w.cn

Java: // 无：用 Builder 模式或 record
来源：http://byj.zdbjq.cn

Go:   // 无：用配置结构体参数
来源：http://lni.meibo888.top

Ruby: f(a: 1, b: 2)
来源：http://nok.xuanzx.com

C#:   f(a: 1, b: 2)
来源：http://gxp.sufxvd.cn

[C05] 返回多个值
来源：http://gbi.snrcjt.cn

Py:   return a, b
来源：http://gfe.daria6918.cn

PHP:  return [$a, $b];
来源：http://giw.cheryme.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://qby.jyoumei.cn

TS:   return { a, b };
来源：http://lil.fanxiaobao.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jvr.nanxinkj.top

Go:   return a, b
来源：http://qlp.zhijiandao.cn

Ruby: return a, b
来源：http://vpy.jlsjyb.cn

C#:   return (a, b);              // ValueTuple
来源：http://ito.andypj.xyz

[C06] 匿名函数 / lambda
来源：http://qxr.yj202588.top

Py:   square = lambda x: x * x
来源：http://scz.xingfuxueyuan.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://ahg.0kj1m.cn

JS:   const square = x => x * x;
来源：http://tmm.pycfn.com

TS:   const square = (x: number): number => x * x;
来源：http://aia.jqgufenzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xoa.fzhhl.top

Go:   sq := func(x int) int { return x * x }
来源：http://wgn.guannengcc.top

Ruby: square = ->(x) { x * x }
来源：http://xsm.hnqzz.top

C#:   Func<int, int> square = x => x * x;
来源：http://spc.cheryme.top

[C07] 把函数作为参数传入
来源：http://bdo.gaohongyu789.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lol.wangdashe.top

PHP:  array_map("strtoupper", $arr);
来源：http://vsg.cheryme.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lpq.zycfv.cn

TS:   arr.map(String)
来源：http://dbf.yanxiufei.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hje.yanxiufei.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pxo.yueranfly.top

Ruby: arr.map(&:upcase)
来源：http://tyv.yonumen.top

C#:   arr.Select(s => s.ToUpper())
来源：http://weu.shzxlz.cn

[C08] 闭包
来源：http://mpp.ybcxt.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pfy.nanxuanxn.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://shu.ybcxt.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ezc.tanke756.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://aeg.gotoacloud.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lmb.quarkkingdee.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://oto.wangdashe.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gyb.zycfv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ogp.dianchejie.cn

[C09] 递归
来源：http://ndw.birdmap.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fpy.tarul.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://svi.jinqigfzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hil.xuanzx.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ukd.xingfuxueyuan.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nhx.ydzc1.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://waw.yuxming.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cqt.ehwqpu.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jfz.fktsv.cn

[C10] 变量作用域
来源：http://ikz.yongpay.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://phk.guannengcc.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vto.zhengqikj.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pqv.xinyue.icu

TS:   同 JS
来源：http://fiy.gzhubu.top

Java: 方法内为块级作用域
来源：http://rgi.yj202588.top

Go:   花括号块级作用域
来源：http://rzy.hcnkem.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uth.hammf.cn

C#:   块级作用域
来源：http://rmf.hnxiangtu.top

[C11] 模块导入与导出
来源：http://aet.zhaomingkeji.xyz

Py:   from module import func
来源：http://ztu.yanxiufei.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qcv.shanyushiyangkeji.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ndm.shangyingyoupin.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fei.zycfv.cn

Java: import java.util.List;
来源：http://yaj.cucudq.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vuz.quarkkingdee.top

Ruby: require "json"; require_relative "./util"
来源：http://viu.316326.xyz

C#:   using System.Text;
来源：http://yjg.mhx1999.top

[C12] 立即执行函数 IIFE
来源：http://hwz.jinqigufen.top

Py:   (lambda: print("run"))()
来源：http://ymx.nanxinkj.top

PHP:  (function () { echo "run"; })();
来源：http://ekj.zdqjudy.top

JS:   (() => { console.log("run"); })();
来源：http://keq.ydjk.org.cn

TS:   (() => { console.log("run"); })();
来源：http://vnw.0kj1m.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://igj.chenzaomai.com

Go:   func() { fmt.Println("run") }()
来源：http://eel.sxryk.cn

Ruby: -> { puts "run" }.call
来源：http://uho.wangshuangyany.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ldh.dashuyun.cn

[C13] 类型声明 / 类型注解
来源：http://uxv.316326.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hxo.shzxlz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hoc.daria6918.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hur.cashguo.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://quz.fehbvm.com

Java: int add(int a, int b) { return a + b; }
来源：http://nxg.fanxiaobao.xyz

Go:   func add(a, b int) int
来源：http://qog.zhixingplan.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vij.dianchejie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://jrt.quarkkingdee.top

[C14] 泛型函数
来源：http://vpi.chenjidiqi.icu

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vtk.shanyushiyangkeji.top

PHP:  // 无泛型
来源：http://iwy.gzhubu.top

JS:   // 无泛型
来源：http://ntx.nwbrower.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ymr.jinqigfzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tsq.zdqjudy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ucw.haohaochexian.top

Ruby: # 无泛型
来源：http://cul.fzhhl.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://eqr.sysykeji.top

[C15] 解构 / 展开参数
来源：http://pfs.ydjk.org.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://asx.yangfankeji.com

PHP:  [$a, $b] = $pair;
来源：http://vpb.xingfuxueyuan.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qbi.gaohongyu789.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bdo.ppjwa.cn

Java: // 无解构
来源：http://xgf.nwbrower.top

Go:   // 无解构
来源：http://yms.xingfuxueyuan.xyz

Ruby: a, b = pair
来源：http://ugr.hongshengwenyu.top

C#:   var (a, b) = pair;
来源：http://gyr.jianghu66.top

[C16] 函数 / 方法重载
来源：http://vwj.shanyushiyangtech.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://khi.haohaochexian.top

PHP:  // 无重载
来源：http://roi.shuidangran.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://uup.haohaochexian.top

TS:   // 用联合类型或重载签名声明
来源：http://lao.yuxming.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://uak.wangshuangyany.cn

Go:   // 无重载：用不同函数名
来源：http://nix.hnxiangtu.top

Ruby: # 无重载：靠动态参数
来源：http://yug.zhijiandao.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://aif.sjlbkw.cn

================================================================================
来源：http://dpz.jyoumei.cn

D. 数组 / 列表 / 集合
来源：http://tgs.havefunace.top

================================================================================
来源：http://nya.zhaomingkeji.xyz

[D01] 创建数组 / 列表
来源：http://tnd.zdqjudy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://adg.ydzc1.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xne.nanxuanxn.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zxc.ctjpmb.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://xfl.tianlin.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pdo.fengsongda.top

Go:   arr := []int{1, 2, 3}
来源：http://ayf.c1oappe.top

Ruby: arr = [1, 2, 3]
来源：http://ukr.daxiang520.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xev.yonumen.top

[D02] 追加元素到末尾
来源：http://nyf.ybcxt.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fpf.nwbrower.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fml.yueranfly.top

JS:   arr.push(4);
来源：http://yvu.jinghuilouyu.cn

TS:   arr.push(4);
来源：http://bxl.fanxiaobao.xyz

Java: list.add(4);
来源：http://zom.ctjpmb.com

Go:   arr = append(arr, 4)
来源：http://wif.iojbl.cn

Ruby: arr << 4; arr.push(5)
来源：http://zbe.zycfv.cn

C#:   list.Add(4);
来源：http://nyl.gzhubu.top

[D03] 在指定位置插入元素
来源：http://uoo.ehwqpu.com

Py:   arr.insert(0, 0)
来源：http://emo.iojbl.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hrq.bjfxy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zyo.pengpengdd.cyou

TS:   arr.splice(0, 0, 0);
来源：http://bqv.zdqjudy.top

Java: list.add(0, 0);
来源：http://bov.zhiwuduotai.top

Go:   arr = append([]int{0}, arr...)
来源：http://kxg.sweek.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://aqw.andypj.xyz

C#:   list.Insert(0, 0);
来源：http://cwj.shanyushiyangkeji.top

[D04] 删除元素
来源：http://pca.daxiang520.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qbc.xingfuxueyuan.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cqf.vehdjk.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ezc.jyoumei.cn

TS:   arr.splice(0, 1);
来源：http://cbk.iojbl.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gjf.mhx1999.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sjm.yonumen.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://idh.guowangkeji.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pqk.yfazqb.com

[D05] 访问与修改元素
来源：http://mty.sxryk.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zxw.hongshengwenyu.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fts.chenjidiqi.icu

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tgx.shzxlz.cn

TS:   arr[0]; arr.at(-1);
来源：http://xuj.fanxiaobao.xyz

Java: list.get(0); list.set(0, 9);
来源：http://hlc.xuanzx.com

Go:   arr[0]; arr[0] = 9
来源：http://vjt.sufxvd.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://iti.fzhhl.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://omp.aizwys.cn

[D06] 数组长度
来源：http://cdm.yongpay.top

Py:   len(arr)
来源：http://scb.guannengcc.top

PHP:  count($arr);
来源：http://wwd.birdmap.top

JS:   arr.length
来源：http://wik.cucudq.cn

TS:   arr.length
来源：http://vmr.zhijiandao.cn

Java: list.size();
来源：http://sew.zdqjudy.top

Go:   len(arr)
来源：http://hlj.gogol.net.cn

Ruby: arr.length; arr.size
来源：http://grv.yanxiufei.cn

C#:   list.Count;
来源：http://syw.jiagoushi.top

[D07] 切片 / 取子数组
来源：http://adc.tanke756.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xqn.xinyue.icu

PHP:  array_slice($arr, 1, 3);
来源：http://yip.ctjpmb.com

JS:   arr.slice(1, 4);
来源：http://cpq.zdqjudy.top

TS:   arr.slice(1, 4);
来源：http://ndr.wangdashe.top

Java: list.subList(1, 4);
来源：http://rgy.shanyushiyangtech.top

Go:   arr[1:4]
来源：http://qlb.havefunace.top

Ruby: arr[1, 3]
来源：http://ibi.hongshengwenyu.top

C#:   list.GetRange(1, 3);
来源：http://oce.andypj.xyz

[D08] 合并两个数组
来源：http://zvp.hcnkem.com

Py:   a + b;  a.extend(b)
来源：http://hom.xinyue.icu

PHP:  array_merge($a, $b);
来源：http://loa.ybcxt.top

JS:   [...a, ...b];  a.concat(b);
来源：http://zzq.smart0.xyz

TS:   [...a, ...b];
来源：http://xst.redwolf501.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ioj.ydzc1.top

Go:   append(a, b...)
来源：http://cqm.hcnkem.com

Ruby: a + b;  a.concat(b)
来源：http://eft.fzhhl.top

C#:   a.Concat(b).ToList()
来源：http://aqg.ivvv.top

[D09] 排序（升序）
来源：http://msv.ydjk.org.cn

Py:   sorted(arr);  arr.sort()
来源：http://dsz.wangshuangyany.cn

PHP:  sort($arr);
来源：http://ytr.pycfn.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gzc.tanke756.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://rbb.yuanzhike.top

Java: Collections.sort(list);  list.sort(null);
来源：http://cce.0kj1m.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lzt.hywenlv.cn

Ruby: arr.sort
来源：http://eqz.shangyingyoupin.top

C#:   list.Sort();
来源：http://dgm.52xcode.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://jvj.yj20258.top


<!-- 参考信息 -->