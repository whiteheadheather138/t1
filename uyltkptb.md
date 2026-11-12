代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gtd.zycfv.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aoj.yueranfly.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wdp.cucudq.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bmu.yueranfly.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xkt.wangdashe.top

[B10] 遍历同时拿索引
来源：http://epo.hesvh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://opv.hywenlv.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qva.yanxiufei.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jmd.shzxlz.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zlu.yongpay.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bst.svipenyu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://diq.gzhubu.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ipp.jinqigfzy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ewg.shuidangran.top

[B11] 生成数字序列 / 区间
来源：http://bls.hnqzz.top

Py:   list(range(0, 10, 2))
来源：http://eqm.fanxiaobao.xyz

PHP:  range(0, 10, 2);
来源：http://sck.xziqi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xzt.xingfuxueyuan.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ewl.cdnleiting.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kzc.hammf.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xun.yongpay.top

Ruby: (0...10).step(2).to_a
来源：http://afv.zhixingplan.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xrc.zhongyouzk.top

[B12] 跳出多层循环
来源：http://hgd.xuetiantiany.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ckx.fanxiaobao.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://qrf.sufxvd.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xng.hnxiangtu.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wah.wangshuangyany.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ipu.jqgufenzy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tlf.jinyuanbaomall.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nnl.hywenlv.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://azr.chenjidiqi.icu

[B13] 判断是否为数字
来源：http://lqw.cheryme.top

Py:   isinstance(x, (int, float))
来源：http://dfs.tanke756.top

PHP:  is_numeric($x)
来源：http://ssp.fengsongda.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://alh.feifeiyinyue.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xkp.shanyushiyangtech.top

Java: x instanceof Number
来源：http://zwc.uphjek.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sdl.ydjk.org.cn

Ruby: x.is_a?(Numeric)
来源：http://akl.vqdsnc.cn

C#:   x is int or double or decimal
来源：http://gvv.jinqigfzy.top

[B14] 判断值是否在集合内
来源：http://zqr.yuanzhike.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yhb.yj20258888.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hzm.tianlin.xyz

JS:   [1, 2, 3].includes(x)
来源：http://lis.gotoacloud.top

TS:   [1, 2, 3].includes(x)
来源：http://cte.fengsongda.top

Java: List.of(1, 2, 3).contains(x)
来源：http://rdc.hammf.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fjv.redwolf501.top

Ruby: [1, 2, 3].include?(x)
来源：http://fdg.zhiwuduotai.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://slz.tanke756.top

[B15] 布尔运算与取反
来源：http://uhu.cashguo.top

Py:   a and b or not c
来源：http://jna.zhoulong.xyz

PHP:  $a && $b || !$c
来源：http://yoy.fehbvm.com

JS:   a && b || !c
来源：http://emm.jqgufenzy.top

TS:   a && b || !c
来源：http://xpe.yj20258.top

Java: a && b || !c
来源：http://olq.zhiwuduotai.top

Go:   a && b || !c
来源：http://ygf.jinghuilouyu.cn

Ruby: a && b || !c
来源：http://vby.gzhubu.top

C#:   a && b || !c
来源：http://wcj.yj20258.top

[B16] 卫语句：不满足条件提前返回
来源：http://vec.bbcook.cn

Py:   if not data: return
来源：http://fox.shangyingyoupin.top

PHP:  if (!$data) { return; }
来源：http://epw.fzhhl.top

JS:   if (!data) return;
来源：http://tid.kuanghao11.cn

TS:   if (!data) return;
来源：http://uka.fzhhl.top

Java: if (data == null) return;
来源：http://uty.kuanghao11.cn

Go:   if data == nil { return }
来源：http://rwl.zhengqikj.top

Ruby: return if data.nil?
来源：http://hlc.yj20258888.top

C#:   if (data == null) return;
来源：http://qpx.gzhubu.top

================================================================================
来源：http://pci.guowangkeji.top

C. 函数与作用域
来源：http://gro.fanxiaobao.xyz

================================================================================
来源：http://fwf.wangshuangyany.cn

[C01] 定义函数
来源：http://amc.ehwqpu.com

Py:   def add(a, b): return a + b
来源：http://hhd.aibaodan.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rlj.dashuyun.cn

JS:   function add(a, b) { return a + b; }
来源：http://jtg.gzhubu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cdv.hfpthk.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vgf.nanxinkj.top

Go:   func add(a, b int) int { return a + b }
来源：http://mrm.nanxuanxn.top

Ruby: def add(a, b); a + b; end
来源：http://tys.ctjpmb.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://brn.tianlin.xyz

[C02] 默认参数
来源：http://ddf.316326.xyz

Py:   def greet(name="World"): return name
来源：http://waz.guowangkeji.top

PHP:  function greet($name = "World") { return $name; }
来源：http://rgv.cheryme.top

JS:   function greet(name = "World") { return name; }
来源：http://ubk.jlsjyb.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vqw.bbcook.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ukp.epnwcf.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wmj.dianchejie.cn

Ruby: def greet(name = "World") = name
来源：http://esy.nanxinkj.top

C#:   string Greet(string name = "World") => name;
来源：http://vrk.jinyuanbaomall.cn

[C03] 可变参数
来源：http://ran.nanxuanxn.top

Py:   def total(*args): return sum(args)
来源：http://wvg.xinyue.icu

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ayq.yj202588.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://asv.zhongyouzk.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://avt.dianchejie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ztd.jiagoushi.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xef.birdmap.top

Ruby: def total(*nums); nums.sum; end
来源：http://gax.aizwys.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://aff.dianchejie.cn

[C04] 命名参数 / 关键字参数
来源：http://dam.dianchejie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://log.316326.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://auk.xylfe.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hsp.nanxinkj.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hth.yj20258.top

Java: // 无：用 Builder 模式或 record
来源：http://mbf.zdqjudy.top

Go:   // 无：用配置结构体参数
来源：http://iui.52xcode.cn

Ruby: f(a: 1, b: 2)
来源：http://tjo.zhongyouzk.top

C#:   f(a: 1, b: 2)
来源：http://gfr.jqgufenzy.top

[C05] 返回多个值
来源：http://hku.hfpthk.cn

Py:   return a, b
来源：http://gcf.shanyushiyangtech.top

PHP:  return [$a, $b];
来源：http://tch.0kj1m.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://cao.c1oappe.top

TS:   return { a, b };
来源：http://lwn.tian-w.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gri.iojbl.cn

Go:   return a, b
来源：http://pjp.zhixingplan.top

Ruby: return a, b
来源：http://uab.tianlin.xyz

C#:   return (a, b);              // ValueTuple
来源：http://dxp.gzhubu.top

[C06] 匿名函数 / lambda
来源：http://bfe.chenlongwang.top

Py:   square = lambda x: x * x
来源：http://eaq.ydzc1.top

PHP:  $square = fn($x) => $x * $x;
来源：http://iam.ydjk.org.cn

JS:   const square = x => x * x;
来源：http://cix.aizwys.cn

TS:   const square = (x: number): number => x * x;
来源：http://zkl.xylfe.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bbo.jqgufenzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://rmr.shangyingyoupin.top

Ruby: square = ->(x) { x * x }
来源：http://lxc.iojbl.cn

C#:   Func<int, int> square = x => x * x;
来源：http://yyb.hongshengwenyu.top

[C07] 把函数作为参数传入
来源：http://rix.fzhhl.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mym.aizwys.cn

PHP:  array_map("strtoupper", $arr);
来源：http://toh.snrcjt.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://iry.jinqigfzy.top

TS:   arr.map(String)
来源：http://jtf.andypj.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kux.nanxuanxn.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://npj.yuxming.cn

Ruby: arr.map(&:upcase)
来源：http://msm.shanyushiyangkeji.top

C#:   arr.Select(s => s.ToUpper())
来源：http://emn.nanxinkj.top

[C08] 闭包
来源：http://xsn.gotoacloud.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yhs.zhongyouzk.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dfm.tianlin.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://elo.svipenyu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hub.yj20258.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pda.ywan-chungtsiang.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rqo.xinyue.icu

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yjh.meibo888.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gms.hfpthk.cn

[C09] 递归
来源：http://bnb.vqdsnc.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uyf.xuetiantiany.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yqs.sysykeji.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gqw.feifeiyinyue.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rgk.feifeiyinyue.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ids.hfpthk.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wxr.haohaochexian.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ztp.ctjpmb.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rrv.zhaomingkeji.xyz

[C10] 变量作用域
来源：http://qxh.tianlin.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jvc.ydzc1.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nfr.vqdsnc.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yxm.gzhubu.top

TS:   同 JS
来源：http://krt.yonumen.top

Java: 方法内为块级作用域
来源：http://jem.zhijiandao.cn

Go:   花括号块级作用域
来源：http://kfq.guannengcc.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bfx.nanxuanxn.top

C#:   块级作用域
来源：http://vox.gzhubu.top

[C11] 模块导入与导出
来源：http://msn.cqqwz.cn

Py:   from module import func
来源：http://euf.yongpay.top

PHP:  require "file.php";  或 use App\Service;
来源：http://hrt.sxryk.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wcy.0kj1m.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://azs.tarul.cn

Java: import java.util.List;
来源：http://fty.sweek.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pqr.xinyue.icu

Ruby: require "json"; require_relative "./util"
来源：http://dbi.nanxuanxn.top

C#:   using System.Text;
来源：http://jgj.andypj.xyz

[C12] 立即执行函数 IIFE
来源：http://zlw.yuanzhike.top

Py:   (lambda: print("run"))()
来源：http://ugw.meibo888.top

PHP:  (function () { echo "run"; })();
来源：http://now.pengpengdd.cyou

JS:   (() => { console.log("run"); })();
来源：http://ixo.hammf.cn

TS:   (() => { console.log("run"); })();
来源：http://hnu.guowangkeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fig.snrcjt.cn

Go:   func() { fmt.Println("run") }()
来源：http://joy.vehdjk.com

Ruby: -> { puts "run" }.call
来源：http://zdh.dashuyun.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hlq.pengpengdd.cyou

[C13] 类型声明 / 类型注解
来源：http://lci.aizwys.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vny.xylfe.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ngg.fktsv.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mfo.gzhubu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yae.aibaodan.cn

Java: int add(int a, int b) { return a + b; }
来源：http://gcq.ybcxt.top

Go:   func add(a, b int) int
来源：http://yjt.gzhubu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hax.bjfxy.top

C#:   int Add(int a, int b) => a + b;
来源：http://ziv.iojbl.cn

[C14] 泛型函数
来源：http://cyv.hnxiangtu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://osf.cheryme.top

PHP:  // 无泛型
来源：http://ybn.snrcjt.cn

JS:   // 无泛型
来源：http://sfs.xingfuxueyuan.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ffq.hongshengwenyu.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ogo.ctjpmb.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mgc.hfpthk.cn

Ruby: # 无泛型
来源：http://ryk.ydzc1.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jhj.316326.xyz

[C15] 解构 / 展开参数
来源：http://zdh.ydzc1.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xhx.zhongyouzk.top

PHP:  [$a, $b] = $pair;
来源：http://zdo.daxiang520.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tix.epnwcf.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vyh.sufxvd.cn

Java: // 无解构
来源：http://yae.tanke756.top

Go:   // 无解构
来源：http://ogs.chenlongwang.top

Ruby: a, b = pair
来源：http://mxo.ydzc1.top

C#:   var (a, b) = pair;
来源：http://bbr.jlsjyb.cn

[C16] 函数 / 方法重载
来源：http://occ.aibaodan.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wei.chenzaomai.com

PHP:  // 无重载
来源：http://aco.wangshuangyany.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bgo.hfpthk.cn

TS:   // 用联合类型或重载签名声明
来源：http://nrm.vehdjk.com

Java: void f(int a) {}  void f(String a) {}
来源：http://tea.yfazqb.com

Go:   // 无重载：用不同函数名
来源：http://vat.cucudq.cn

Ruby: # 无重载：靠动态参数
来源：http://nuo.iojbl.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://opa.daxiang520.top

================================================================================
来源：http://vah.redwolf501.top

D. 数组 / 列表 / 集合
来源：http://mre.ybcxt.top

================================================================================
来源：http://sbp.jianghu66.top

[D01] 创建数组 / 列表
来源：http://qpo.pengpengdd.cyou

Py:   arr = [1, 2, 3];  empty = []
来源：http://ctz.hywenlv.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sqi.xuetiantiany.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dyj.kuanghao11.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ynz.hywenlv.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qcc.nanxinkj.top

Go:   arr := []int{1, 2, 3}
来源：http://nro.aizwys.cn

Ruby: arr = [1, 2, 3]
来源：http://qbf.chenjidiqi.icu

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://eej.redwolf501.top

[D02] 追加元素到末尾
来源：http://sxv.jianghu66.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vro.hammf.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://taz.hnxiangtu.top

JS:   arr.push(4);
来源：http://mzq.iojbl.cn

TS:   arr.push(4);
来源：http://pdm.pycfn.com

Java: list.add(4);
来源：http://icp.fanxiaobao.xyz

Go:   arr = append(arr, 4)
来源：http://khr.aizwys.cn

Ruby: arr << 4; arr.push(5)
来源：http://ifi.yj20258888.top

C#:   list.Add(4);
来源：http://zzy.fktsv.cn

[D03] 在指定位置插入元素
来源：http://wyh.yuxming.cn

Py:   arr.insert(0, 0)
来源：http://yap.pengpengdd.cyou

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lxo.guannengcc.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xgz.chenjidiqi.icu

TS:   arr.splice(0, 0, 0);
来源：http://tpl.jinyuanbaomall.cn

Java: list.add(0, 0);
来源：http://pyn.hnxiangtu.top

Go:   arr = append([]int{0}, arr...)
来源：http://gts.chenjidiqi.icu

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://myy.vehdjk.com

C#:   list.Insert(0, 0);
来源：http://vbl.sysykeji.top

[D04] 删除元素
来源：http://tjb.52xcode.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kgz.birdmap.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mmp.52xcode.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wxs.jianghu66.top

TS:   arr.splice(0, 1);
来源：http://ven.sysykeji.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cqk.pycfn.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pkl.jinyuanbaomall.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://unh.hnqzz.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ocu.zycfv.cn

[D05] 访问与修改元素
来源：http://edz.zycfv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sxr.sysykeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ajc.redwolf501.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vlc.ydjk.org.cn

TS:   arr[0]; arr.at(-1);
来源：http://dpc.yfazqb.com

Java: list.get(0); list.set(0, 9);
来源：http://cid.cucudq.cn

Go:   arr[0]; arr[0] = 9
来源：http://ivm.haohaochexian.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fdn.andypj.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lno.yj20258888.top

[D06] 数组长度
来源：http://klk.cqqwz.cn

Py:   len(arr)
来源：http://gcb.hesvh.cn

PHP:  count($arr);
来源：http://mxw.fanxiaobao.xyz

JS:   arr.length
来源：http://fso.tianlin.xyz

TS:   arr.length
来源：http://ktu.vehdjk.com

Java: list.size();
来源：http://ixz.yfazqb.com

Go:   len(arr)
来源：http://nya.hysaishi.cn

Ruby: arr.length; arr.size
来源：http://amh.yueranfly.top

C#:   list.Count;
来源：http://ngk.zhiwuduotai.top

[D07] 切片 / 取子数组
来源：http://thz.vqdsnc.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gfn.yj20258888.top

PHP:  array_slice($arr, 1, 3);
来源：http://tmx.gaohongyu789.top

JS:   arr.slice(1, 4);
来源：http://bfo.zycfv.cn

TS:   arr.slice(1, 4);
来源：http://gpp.ywan-chungtsiang.top

Java: list.subList(1, 4);
来源：http://ngc.hcnkem.com

Go:   arr[1:4]
来源：http://jla.fengsongda.top

Ruby: arr[1, 3]
来源：http://xky.yangfankeji.com

C#:   list.GetRange(1, 3);
来源：http://fnx.zhaomingkeji.xyz

[D08] 合并两个数组
来源：http://kyp.pengpengdd.cyou

Py:   a + b;  a.extend(b)
来源：http://hxb.ivvv.top

PHP:  array_merge($a, $b);
来源：http://yki.jinghuilouyu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://itl.hammf.cn

TS:   [...a, ...b];
来源：http://xcq.yj20258.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://esq.ppjwa.cn

Go:   append(a, b...)
来源：http://fye.pycfn.com

Ruby: a + b;  a.concat(b)
来源：http://eok.yj202588.top

C#:   a.Concat(b).ToList()
来源：http://vis.svipenyu.cn

[D09] 排序（升序）
来源：http://qwh.guannengcc.top

Py:   sorted(arr);  arr.sort()
来源：http://hus.zhengqikj.top

PHP:  sort($arr);
来源：http://ywc.daria6918.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xbp.chenlongwang.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://lzu.bbcook.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://dzd.cucudq.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yxs.fanxiaobao.xyz

Ruby: arr.sort
来源：http://gko.hesvh.cn

C#:   list.Sort();
来源：http://aik.316326.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://asb.shangyingyoupin.top


<!-- 参考信息 -->