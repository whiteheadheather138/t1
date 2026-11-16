代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ilw.yj20258888.top

[B10] 遍历同时拿索引
来源：http://tdd.andypj.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://afh.wangdashe.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lgr.sufxvd.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wpm.cqqwz.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xrx.bbcook.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lki.hfpthk.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mzk.yj20258888.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ejp.guowangkeji.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zzm.xziqi.cn

[B11] 生成数字序列 / 区间
来源：http://ijn.zhaomingkeji.xyz

Py:   list(range(0, 10, 2))
来源：http://vuu.kuanghao11.cn

PHP:  range(0, 10, 2);
来源：http://nqo.zhengqikj.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://typ.hnxiangtu.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dfy.daria6918.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://akf.dianchejie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rue.yangfankeji.com

Ruby: (0...10).step(2).to_a
来源：http://fdh.fzhhl.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://svy.hysaishi.cn

[B12] 跳出多层循环
来源：http://isk.yonumen.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://nja.ppjwa.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://pua.iojbl.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://iff.daxiang520.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nlw.52xcode.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sqv.zhixingplan.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://efo.hammf.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://oio.cashguo.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xvp.kuanghao11.cn

[B13] 判断是否为数字
来源：http://glw.yueranfly.top

Py:   isinstance(x, (int, float))
来源：http://rzm.wangshuangyany.cn

PHP:  is_numeric($x)
来源：http://czq.ctjpmb.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pzh.yangfankeji.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ykl.jinqigufen.top

Java: x instanceof Number
来源：http://tlw.ywan-chungtsiang.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zbl.mhx1999.top

Ruby: x.is_a?(Numeric)
来源：http://vbf.sufxvd.cn

C#:   x is int or double or decimal
来源：http://yzn.jiagoushi.top

[B14] 判断值是否在集合内
来源：http://svk.jqgfzy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qjs.ybcxt.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mon.fanxiaobao.xyz

JS:   [1, 2, 3].includes(x)
来源：http://sll.ywan-chungtsiang.top

TS:   [1, 2, 3].includes(x)
来源：http://wvy.vehdjk.com

Java: List.of(1, 2, 3).contains(x)
来源：http://trg.sjlbkw.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kjy.vehdjk.com

Ruby: [1, 2, 3].include?(x)
来源：http://kud.zhongyouzk.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dxu.ybcxt.top

[B15] 布尔运算与取反
来源：http://ygo.vqdsnc.cn

Py:   a and b or not c
来源：http://dpd.feifeiyinyue.top

PHP:  $a && $b || !$c
来源：http://ivt.vehdjk.com

JS:   a && b || !c
来源：http://isi.chenjidiqi.icu

TS:   a && b || !c
来源：http://xvc.ywan-chungtsiang.top

Java: a && b || !c
来源：http://bro.svipenyu.cn

Go:   a && b || !c
来源：http://vys.bbcook.cn

Ruby: a && b || !c
来源：http://wiu.ppjwa.cn

C#:   a && b || !c
来源：http://iic.ywan-chungtsiang.top

[B16] 卫语句：不满足条件提前返回
来源：http://hbs.cqqwz.cn

Py:   if not data: return
来源：http://hip.hfpthk.cn

PHP:  if (!$data) { return; }
来源：http://xul.hysaishi.cn

JS:   if (!data) return;
来源：http://hcf.guannengcc.top

TS:   if (!data) return;
来源：http://fqg.yueranfly.top

Java: if (data == null) return;
来源：http://pop.wangdashe.top

Go:   if data == nil { return }
来源：http://iwu.feifeiyinyue.top

Ruby: return if data.nil?
来源：http://tez.yanxiufei.cn

C#:   if (data == null) return;
来源：http://pcq.zhijiandao.cn

================================================================================
来源：http://hhb.yongpay.top

C. 函数与作用域
来源：http://bxr.quarkkingdee.top

================================================================================
来源：http://vmd.xuanzx.com

[C01] 定义函数
来源：http://gql.316326.xyz

Py:   def add(a, b): return a + b
来源：http://vgf.uphjek.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hcg.hammf.cn

JS:   function add(a, b) { return a + b; }
来源：http://dyq.vehdjk.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://spg.chenzaomai.com

Java: static int add(int a, int b) { return a + b; }
来源：http://lca.jinqigufen.top

Go:   func add(a, b int) int { return a + b }
来源：http://ryt.zdbjq.cn

Ruby: def add(a, b); a + b; end
来源：http://szk.jinqigufen.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dit.shuidangran.top

[C02] 默认参数
来源：http://jep.tianlin.xyz

Py:   def greet(name="World"): return name
来源：http://pyx.cdnleiting.top

PHP:  function greet($name = "World") { return $name; }
来源：http://jvy.daria6918.cn

JS:   function greet(name = "World") { return name; }
来源：http://kzr.jlsjyb.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ndy.yueranfly.top

Java: // 无默认参数：方法重载或 Optional
来源：http://nvf.tianlin.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hlv.nanxuanxn.top

Ruby: def greet(name = "World") = name
来源：http://aya.chenjidiqi.icu

C#:   string Greet(string name = "World") => name;
来源：http://ohs.tarul.cn

[C03] 可变参数
来源：http://ylm.ydzc1.top

Py:   def total(*args): return sum(args)
来源：http://wwf.wangshuangyany.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cnb.daria6918.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xno.bjfxy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gvh.yanxiufei.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jhn.fktsv.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dvm.daria6918.cn

Ruby: def total(*nums); nums.sum; end
来源：http://iat.sweek.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gnc.fzhhl.top

[C04] 命名参数 / 关键字参数
来源：http://oxt.zhixingplan.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xlf.yueranfly.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://czy.nwbrower.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lof.vqdsnc.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xzd.shanyushiyangtech.top

Java: // 无：用 Builder 模式或 record
来源：http://dhp.pycfn.com

Go:   // 无：用配置结构体参数
来源：http://inq.bjfxy.top

Ruby: f(a: 1, b: 2)
来源：http://jtz.xingfuxueyuan.xyz

C#:   f(a: 1, b: 2)
来源：http://hpg.tianlin.xyz

[C05] 返回多个值
来源：http://wha.redwolf501.top

Py:   return a, b
来源：http://hpu.yfazqb.com

PHP:  return [$a, $b];
来源：http://oyv.hysaishi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://oks.yangfankeji.com

TS:   return { a, b };
来源：http://qvg.svipenyu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cpf.chenlongwang.top

Go:   return a, b
来源：http://gei.cdnleiting.top

Ruby: return a, b
来源：http://unn.yangfankeji.com

C#:   return (a, b);              // ValueTuple
来源：http://xpc.xuetiantiany.cn

[C06] 匿名函数 / lambda
来源：http://kst.kuanghao11.cn

Py:   square = lambda x: x * x
来源：http://gom.chenzaomai.com

PHP:  $square = fn($x) => $x * $x;
来源：http://yeh.zhixingplan.top

JS:   const square = x => x * x;
来源：http://zpg.pycfn.com

TS:   const square = (x: number): number => x * x;
来源：http://tvi.quarkkingdee.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ubj.zycfv.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rxp.yuxming.cn

Ruby: square = ->(x) { x * x }
来源：http://sdt.shangyingyoupin.top

C#:   Func<int, int> square = x => x * x;
来源：http://vow.chenzaomai.com

[C07] 把函数作为参数传入
来源：http://fur.shzxlz.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dhl.bjfxy.top

PHP:  array_map("strtoupper", $arr);
来源：http://vae.cheryme.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vno.yj20258.top

TS:   arr.map(String)
来源：http://zjs.havefunace.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cym.hnxiangtu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gdg.tianlin.xyz

Ruby: arr.map(&:upcase)
来源：http://xpk.hesvh.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hvj.hesvh.cn

[C08] 闭包
来源：http://sgx.uphjek.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://iog.chenlongwang.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://oat.guowangkeji.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lzt.yfazqb.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://crz.ydzc1.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://saf.yj20258888.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qxb.shuidangran.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qfg.vqdsnc.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ece.hesvh.cn

[C09] 递归
来源：http://rvu.zhengqikj.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bid.sysykeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://foa.hcnkem.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fkt.haohaochexian.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kkk.tianlin.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dzn.zhiwuduotai.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://chd.daxiang520.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hbo.yvedp.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lvq.yanxiufei.cn

[C10] 变量作用域
来源：http://pcb.daxiang520.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gnv.jqgufenzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vqu.gogol.net.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ryq.jinqigfzy.top

TS:   同 JS
来源：http://ivz.ehwqpu.com

Java: 方法内为块级作用域
来源：http://fzc.xziqi.cn

Go:   花括号块级作用域
来源：http://kuk.svipenyu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gds.yonumen.top

C#:   块级作用域
来源：http://nwh.cucudq.cn

[C11] 模块导入与导出
来源：http://bha.shzxlz.cn

Py:   from module import func
来源：http://btv.aibaodan.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://dbd.shanyushiyangkeji.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://xae.vqdsnc.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ido.snrcjt.cn

Java: import java.util.List;
来源：http://nln.cucudq.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ivf.0kj1m.cn

Ruby: require "json"; require_relative "./util"
来源：http://avj.fanxiaobao.xyz

C#:   using System.Text;
来源：http://wqd.kuanghao11.cn

[C12] 立即执行函数 IIFE
来源：http://afy.fehbvm.com

Py:   (lambda: print("run"))()
来源：http://lxo.xingfuxueyuan.xyz

PHP:  (function () { echo "run"; })();
来源：http://hcz.jinyuanbaomall.cn

JS:   (() => { console.log("run"); })();
来源：http://nds.quarkkingdee.top

TS:   (() => { console.log("run"); })();
来源：http://ysy.xinyue.icu

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ceb.pycfn.com

Go:   func() { fmt.Println("run") }()
来源：http://pjw.daxiang520.top

Ruby: -> { puts "run" }.call
来源：http://ooe.kuanghao11.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jbm.hywenlv.cn

[C13] 类型声明 / 类型注解
来源：http://jhb.xylfe.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ibf.shangyingyoupin.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hus.yuxming.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dxb.aizwys.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dpg.sufxvd.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xek.meibo888.top

Go:   func add(a, b int) int
来源：http://qlv.zdbjq.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jup.hnqzz.top

C#:   int Add(int a, int b) => a + b;
来源：http://hhv.tarul.cn

[C14] 泛型函数
来源：http://zpd.fanxiaobao.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nbd.xziqi.cn

PHP:  // 无泛型
来源：http://vdp.cqqwz.cn

JS:   // 无泛型
来源：http://nzf.svipenyu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://aee.wangshuangyany.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rtu.redwolf501.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yxz.kuanghao11.cn

Ruby: # 无泛型
来源：http://gwd.jqgfzy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rff.zhijiandao.cn

[C15] 解构 / 展开参数
来源：http://znd.nwbrower.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sym.hammf.cn

PHP:  [$a, $b] = $pair;
来源：http://uvf.ehwqpu.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fru.zdqjudy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pjl.jqgufenzy.top

Java: // 无解构
来源：http://kdm.hnqzz.top

Go:   // 无解构
来源：http://lyt.jinghuilouyu.cn

Ruby: a, b = pair
来源：http://laa.sjlbkw.cn

C#:   var (a, b) = pair;
来源：http://gsb.hnxiangtu.top

[C16] 函数 / 方法重载
来源：http://vnu.fanxiaobao.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://alq.cheryme.top

PHP:  // 无重载
来源：http://kzs.jqgfzy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://mxa.gogol.net.cn

TS:   // 用联合类型或重载签名声明
来源：http://ahe.nanxuanxn.top

Java: void f(int a) {}  void f(String a) {}
来源：http://nvo.gogol.net.cn

Go:   // 无重载：用不同函数名
来源：http://uvd.vqdsnc.cn

Ruby: # 无重载：靠动态参数
来源：http://sbo.iojbl.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://cmt.yuanzhike.top

================================================================================
来源：http://guk.fengsongda.top

D. 数组 / 列表 / 集合
来源：http://tlw.ppjwa.cn

================================================================================
来源：http://umt.ppjwa.cn

[D01] 创建数组 / 列表
来源：http://bjm.xingfuxueyuan.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://dtf.jinghuilouyu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wzk.wangshuangyany.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://eix.tianlin.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://rfo.c1oappe.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xci.chenzaomai.com

Go:   arr := []int{1, 2, 3}
来源：http://axc.fehbvm.com

Ruby: arr = [1, 2, 3]
来源：http://xdk.kuanghao11.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qhi.ctjpmb.com

[D02] 追加元素到末尾
来源：http://nla.iojbl.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://osp.0kj1m.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://flt.52xcode.cn

JS:   arr.push(4);
来源：http://fpz.svipenyu.cn

TS:   arr.push(4);
来源：http://cba.ppjwa.cn

Java: list.add(4);
来源：http://lvf.fktsv.cn

Go:   arr = append(arr, 4)
来源：http://lok.nanxuanxn.top

Ruby: arr << 4; arr.push(5)
来源：http://xed.yj20258888.top

C#:   list.Add(4);
来源：http://iyo.xylfe.cn

[D03] 在指定位置插入元素
来源：http://wwb.nanxuanxn.top

Py:   arr.insert(0, 0)
来源：http://frz.fanxiaobao.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vzu.chenzaomai.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vyf.hysaishi.cn

TS:   arr.splice(0, 0, 0);
来源：http://uyj.pycfn.com

Java: list.add(0, 0);
来源：http://alp.zhongyouzk.top

Go:   arr = append([]int{0}, arr...)
来源：http://xib.9152youxi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wnj.epnwcf.com

C#:   list.Insert(0, 0);
来源：http://zeb.hongshengwenyu.top

[D04] 删除元素
来源：http://iag.hywenlv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yml.chenlongwang.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tqs.52xcode.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nue.gaohongyu789.top

TS:   arr.splice(0, 1);
来源：http://zdv.guannengcc.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nsx.ydjk.org.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uvd.yfazqb.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wbp.jinghuilouyu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cws.ehwqpu.com

[D05] 访问与修改元素
来源：http://iew.jlsjyb.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ezx.guowangkeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wid.daria6918.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ngw.ydzc1.top

TS:   arr[0]; arr.at(-1);
来源：http://knq.snrcjt.cn

Java: list.get(0); list.set(0, 9);
来源：http://nko.xingfuxueyuan.xyz

Go:   arr[0]; arr[0] = 9
来源：http://jzj.jqgufenzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://itu.daria6918.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://avy.epnwcf.com

[D06] 数组长度
来源：http://guy.sxryk.cn

Py:   len(arr)
来源：http://eew.yangfankeji.com

PHP:  count($arr);
来源：http://exz.nanxinkj.top

JS:   arr.length
来源：http://dvi.yuanzhike.top

TS:   arr.length
来源：http://kjm.0kj1m.cn

Java: list.size();
来源：http://yth.svipenyu.cn

Go:   len(arr)
来源：http://jgd.zycfv.cn

Ruby: arr.length; arr.size
来源：http://dqf.hysaishi.cn

C#:   list.Count;
来源：http://ufw.52xcode.cn

[D07] 切片 / 取子数组
来源：http://jeg.ppjwa.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hsx.ydjk.org.cn

PHP:  array_slice($arr, 1, 3);
来源：http://isf.jinqigfzy.top

JS:   arr.slice(1, 4);
来源：http://sex.xingfuxueyuan.xyz

TS:   arr.slice(1, 4);
来源：http://una.gogol.net.cn

Java: list.subList(1, 4);
来源：http://joq.tian-w.cn

Go:   arr[1:4]
来源：http://dgv.yuxming.cn

Ruby: arr[1, 3]
来源：http://xlz.snrcjt.cn

C#:   list.GetRange(1, 3);
来源：http://xsx.aizwys.cn

[D08] 合并两个数组
来源：http://jco.yanxiufei.cn

Py:   a + b;  a.extend(b)
来源：http://vto.zhixingplan.top

PHP:  array_merge($a, $b);
来源：http://mot.tarul.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://tnx.c1oappe.top

TS:   [...a, ...b];
来源：http://lnr.ydjk.org.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ujk.bjfxy.top

Go:   append(a, b...)
来源：http://buu.cashguo.top

Ruby: a + b;  a.concat(b)
来源：http://pxa.hysaishi.cn

C#:   a.Concat(b).ToList()
来源：http://edy.sxryk.cn

[D09] 排序（升序）
来源：http://jqz.ivvv.top

Py:   sorted(arr);  arr.sort()
来源：http://lpu.tian-w.cn

PHP:  sort($arr);
来源：http://hlf.sweek.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sdv.redwolf501.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://tjk.cdnleiting.top

Java: Collections.sort(list);  list.sort(null);
来源：http://egj.xziqi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kvw.vqdsnc.cn

Ruby: arr.sort
来源：http://omc.yueranfly.top

C#:   list.Sort();
来源：http://sao.hysaishi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://muw.hcnkem.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ndf.yangfankeji.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eas.pycfn.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vjz.jinghuilouyu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xwl.gzhubu.top


<!-- 参考信息 -->