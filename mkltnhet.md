代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lwx.pengpengdd.cyou

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vfp.redwolf501.top

[B11] 生成数字序列 / 区间
来源：http://lnp.jyoumei.cn

Py:   list(range(0, 10, 2))
来源：http://dtg.havefunace.top

PHP:  range(0, 10, 2);
来源：http://cby.guannengcc.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://omv.tarul.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yzj.pycfn.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://elv.feifeiyinyue.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bcw.zdbjq.cn

Ruby: (0...10).step(2).to_a
来源：http://rkr.sweek.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://msy.hesvh.cn

[B12] 跳出多层循环
来源：http://rqc.tanke756.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://wao.hnqzz.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://xeb.fanxiaobao.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ozy.9152youxi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://eyc.ydzc1.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yxz.gzhubu.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bno.ybcxt.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tvt.zhijiandao.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ajr.uphjek.com

[B13] 判断是否为数字
来源：http://sya.cucudq.cn

Py:   isinstance(x, (int, float))
来源：http://msc.cqqwz.cn

PHP:  is_numeric($x)
来源：http://xuq.yuanzhike.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ixe.sweek.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oua.jinghuilouyu.cn

Java: x instanceof Number
来源：http://tfa.yvedp.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lia.uphjek.com

Ruby: x.is_a?(Numeric)
来源：http://rko.hywenlv.cn

C#:   x is int or double or decimal
来源：http://oym.guowangkeji.top

[B14] 判断值是否在集合内
来源：http://mby.zhengqikj.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qtu.yj202588.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://het.cashguo.top

JS:   [1, 2, 3].includes(x)
来源：http://flx.daxiang520.top

TS:   [1, 2, 3].includes(x)
来源：http://kaz.cashguo.top

Java: List.of(1, 2, 3).contains(x)
来源：http://kmf.xuetiantiany.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://myh.jianghu66.top

Ruby: [1, 2, 3].include?(x)
来源：http://pit.aizwys.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xco.yueranfly.top

[B15] 布尔运算与取反
来源：http://abm.yj202588.top

Py:   a and b or not c
来源：http://jby.yueranfly.top

PHP:  $a && $b || !$c
来源：http://nab.xuetiantiany.cn

JS:   a && b || !c
来源：http://yzc.vqdsnc.cn

TS:   a && b || !c
来源：http://obd.yanxiufei.cn

Java: a && b || !c
来源：http://nuy.quarkkingdee.top

Go:   a && b || !c
来源：http://crc.zhixingplan.top

Ruby: a && b || !c
来源：http://sqn.ydzc1.top

C#:   a && b || !c
来源：http://xgd.jqgufenzy.top

[B16] 卫语句：不满足条件提前返回
来源：http://qrh.52xcode.cn

Py:   if not data: return
来源：http://jvh.xinyue.icu

PHP:  if (!$data) { return; }
来源：http://eqh.shanyushiyangtech.top

JS:   if (!data) return;
来源：http://knk.pycfn.com

TS:   if (!data) return;
来源：http://mlq.vqdsnc.cn

Java: if (data == null) return;
来源：http://tkn.nanxuanxn.top

Go:   if data == nil { return }
来源：http://vcm.cdnleiting.top

Ruby: return if data.nil?
来源：http://oes.pycfn.com

C#:   if (data == null) return;
来源：http://vbg.jianghu66.top

================================================================================
来源：http://hhm.jinghuilouyu.cn

C. 函数与作用域
来源：http://uvu.feifeiyinyue.top

================================================================================
来源：http://mix.hnqzz.top

[C01] 定义函数
来源：http://cvw.hesvh.cn

Py:   def add(a, b): return a + b
来源：http://chx.svipenyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jhm.hywenlv.cn

JS:   function add(a, b) { return a + b; }
来源：http://xyw.smart0.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nfl.feifeiyinyue.top

Java: static int add(int a, int b) { return a + b; }
来源：http://vcn.xingfuxueyuan.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://zsl.jinyuanbaomall.cn

Ruby: def add(a, b); a + b; end
来源：http://bnk.xuetiantiany.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://plf.gaohongyu789.top

[C02] 默认参数
来源：http://pfe.guowangkeji.top

Py:   def greet(name="World"): return name
来源：http://zmm.jqgfzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://qds.jqgufenzy.top

JS:   function greet(name = "World") { return name; }
来源：http://wge.tianlin.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://jzg.meibo888.top

Java: // 无默认参数：方法重载或 Optional
来源：http://auz.vehdjk.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ved.ydjk.org.cn

Ruby: def greet(name = "World") = name
来源：http://kkd.zycfv.cn

C#:   string Greet(string name = "World") => name;
来源：http://rki.hysaishi.cn

[C03] 可变参数
来源：http://szx.yonumen.top

Py:   def total(*args): return sum(args)
来源：http://gzx.havefunace.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yao.hcnkem.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://oud.havefunace.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xoe.chenlongwang.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qvl.52xcode.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wcr.haohaochexian.top

Ruby: def total(*nums); nums.sum; end
来源：http://xlx.sxryk.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vpz.jlsjyb.cn

[C04] 命名参数 / 关键字参数
来源：http://hye.dianchejie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cis.jianghu66.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://phd.ppjwa.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://iby.xingfuxueyuan.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tdi.wangshuangyany.cn

Java: // 无：用 Builder 模式或 record
来源：http://yoz.wangshuangyany.cn

Go:   // 无：用配置结构体参数
来源：http://dns.andypj.xyz

Ruby: f(a: 1, b: 2)
来源：http://jou.jyoumei.cn

C#:   f(a: 1, b: 2)
来源：http://ltw.wangdashe.top

[C05] 返回多个值
来源：http://rxn.hcnkem.com

Py:   return a, b
来源：http://jtn.yangfankeji.com

PHP:  return [$a, $b];
来源：http://oto.yfazqb.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://usp.sxryk.cn

TS:   return { a, b };
来源：http://oqa.fktsv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://asy.hfpthk.cn

Go:   return a, b
来源：http://lyk.uphjek.com

Ruby: return a, b
来源：http://bkg.haohaochexian.top

C#:   return (a, b);              // ValueTuple
来源：http://mum.epnwcf.com

[C06] 匿名函数 / lambda
来源：http://exj.bbcook.cn

Py:   square = lambda x: x * x
来源：http://oyb.yonumen.top

PHP:  $square = fn($x) => $x * $x;
来源：http://qex.cqqwz.cn

JS:   const square = x => x * x;
来源：http://oca.gaohongyu789.top

TS:   const square = (x: number): number => x * x;
来源：http://vgz.jinghuilouyu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dry.9152youxi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jiv.fktsv.cn

Ruby: square = ->(x) { x * x }
来源：http://bzy.hnxiangtu.top

C#:   Func<int, int> square = x => x * x;
来源：http://toa.xingfuxueyuan.xyz

[C07] 把函数作为参数传入
来源：http://pts.xziqi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sow.xingfuxueyuan.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://rwe.yj20258.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://whn.xziqi.cn

TS:   arr.map(String)
来源：http://amf.tarul.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xhi.andypj.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xhl.ctjpmb.com

Ruby: arr.map(&:upcase)
来源：http://gse.guannengcc.top

C#:   arr.Select(s => s.ToUpper())
来源：http://xqo.shanyushiyangkeji.top

[C08] 闭包
来源：http://hcy.ydjk.org.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jdq.wangshuangyany.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://olx.xziqi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fzy.andypj.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hki.zhijiandao.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://aag.vehdjk.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ojw.0kj1m.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bwb.sysykeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ezs.shanyushiyangtech.top

[C09] 递归
来源：http://svb.ivvv.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nll.uphjek.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://oxw.aizwys.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wfz.xinyue.icu

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dtp.jqgufenzy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://agb.hammf.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dsy.hcnkem.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nxz.bjfxy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qlz.yvedp.cn

[C10] 变量作用域
来源：http://jge.wangdashe.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yjr.zhiwuduotai.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bqt.pycfn.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ica.zhixingplan.top

TS:   同 JS
来源：http://twl.quarkkingdee.top

Java: 方法内为块级作用域
来源：http://wym.jinqigufen.top

Go:   花括号块级作用域
来源：http://ghb.sweek.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://paq.hammf.cn

C#:   块级作用域
来源：http://kbz.ywan-chungtsiang.top

[C11] 模块导入与导出
来源：http://itb.svipenyu.cn

Py:   from module import func
来源：http://npz.xylfe.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://szk.hfpthk.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zyn.kuanghao11.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jda.xuanzx.com

Java: import java.util.List;
来源：http://ydh.chenjidiqi.icu

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://aqy.xingfuxueyuan.xyz

Ruby: require "json"; require_relative "./util"
来源：http://hdx.chenzaomai.com

C#:   using System.Text;
来源：http://dvy.9152youxi.cn

[C12] 立即执行函数 IIFE
来源：http://njq.0kj1m.cn

Py:   (lambda: print("run"))()
来源：http://rbj.chenjidiqi.icu

PHP:  (function () { echo "run"; })();
来源：http://ipz.yuxming.cn

JS:   (() => { console.log("run"); })();
来源：http://pzc.ybcxt.top

TS:   (() => { console.log("run"); })();
来源：http://opf.fanxiaobao.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gsh.yj20258888.top

Go:   func() { fmt.Println("run") }()
来源：http://eyl.fanxiaobao.xyz

Ruby: -> { puts "run" }.call
来源：http://prc.bbcook.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://vco.cashguo.top

[C13] 类型声明 / 类型注解
来源：http://mgt.ydzc1.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ecs.sxryk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aol.shangyingyoupin.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sqr.xingfuxueyuan.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://giv.smart0.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://xvn.feifeiyinyue.top

Go:   func add(a, b int) int
来源：http://cth.snrcjt.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://azm.bjfxy.top

C#:   int Add(int a, int b) => a + b;
来源：http://kwy.hesvh.cn

[C14] 泛型函数
来源：http://upu.yuxming.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://eps.jinqigufen.top

PHP:  // 无泛型
来源：http://mls.shuidangran.top

JS:   // 无泛型
来源：http://exh.hfpthk.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ggd.nanxuanxn.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://iwm.ydjk.org.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://djj.fzhhl.top

Ruby: # 无泛型
来源：http://psm.daria6918.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tiz.tarul.cn

[C15] 解构 / 展开参数
来源：http://mhb.sxryk.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://isg.tarul.cn

PHP:  [$a, $b] = $pair;
来源：http://uxd.birdmap.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ppk.wangdashe.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uvv.kuanghao11.cn

Java: // 无解构
来源：http://eex.tianlin.xyz

Go:   // 无解构
来源：http://jhy.nanxuanxn.top

Ruby: a, b = pair
来源：http://juz.zdqjudy.top

C#:   var (a, b) = pair;
来源：http://fgh.ydjk.org.cn

[C16] 函数 / 方法重载
来源：http://xhp.ybcxt.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kzv.fzhhl.top

PHP:  // 无重载
来源：http://afa.sysykeji.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://wlx.sweek.top

TS:   // 用联合类型或重载签名声明
来源：http://dls.jianghu66.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ewh.jyoumei.cn

Go:   // 无重载：用不同函数名
来源：http://ies.ydjk.org.cn

Ruby: # 无重载：靠动态参数
来源：http://zpj.shanyushiyangtech.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ulw.hfpthk.cn

================================================================================
来源：http://aze.nanxinkj.top

D. 数组 / 列表 / 集合
来源：http://zqf.ybcxt.top

================================================================================
来源：http://ayh.pycfn.com

[D01] 创建数组 / 列表
来源：http://zgy.quarkkingdee.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://wcb.jinqigfzy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yrv.jqgufenzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ebs.hcnkem.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://vvn.tanke756.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mvm.shuidangran.top

Go:   arr := []int{1, 2, 3}
来源：http://xtz.hfpthk.cn

Ruby: arr = [1, 2, 3]
来源：http://wme.cashguo.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qpz.zhixingplan.top

[D02] 追加元素到末尾
来源：http://oyk.yueranfly.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tvv.quarkkingdee.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xkj.havefunace.top

JS:   arr.push(4);
来源：http://gcx.daria6918.cn

TS:   arr.push(4);
来源：http://ehv.yvedp.cn

Java: list.add(4);
来源：http://npd.yongpay.top

Go:   arr = append(arr, 4)
来源：http://lsb.jinghuilouyu.cn

Ruby: arr << 4; arr.push(5)
来源：http://lbw.xingfuxueyuan.xyz

C#:   list.Add(4);
来源：http://hzt.smart0.xyz

[D03] 在指定位置插入元素
来源：http://tez.zdbjq.cn

Py:   arr.insert(0, 0)
来源：http://tyg.sufxvd.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lft.ydjk.org.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uay.jinqigufen.top

TS:   arr.splice(0, 0, 0);
来源：http://iha.tian-w.cn

Java: list.add(0, 0);
来源：http://ydn.sysykeji.top

Go:   arr = append([]int{0}, arr...)
来源：http://ufj.ppjwa.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rpo.redwolf501.top

C#:   list.Insert(0, 0);
来源：http://uab.guannengcc.top

[D04] 删除元素
来源：http://agu.pengpengdd.cyou

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xpu.gaohongyu789.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://whk.haohaochexian.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ksc.xinyue.icu

TS:   arr.splice(0, 1);
来源：http://jal.jyoumei.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wgh.haohaochexian.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://osr.sweek.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://afi.aibaodan.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://htp.bjfxy.top

[D05] 访问与修改元素
来源：http://ibi.smart0.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cip.zhongyouzk.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xpe.fanxiaobao.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hto.zycfv.cn

TS:   arr[0]; arr.at(-1);
来源：http://bdr.316326.xyz

Java: list.get(0); list.set(0, 9);
来源：http://mtv.smart0.xyz

Go:   arr[0]; arr[0] = 9
来源：http://hrl.bbcook.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dde.jyoumei.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uuq.hnqzz.top

[D06] 数组长度
来源：http://jfv.cucudq.cn

Py:   len(arr)
来源：http://tdo.9152youxi.cn

PHP:  count($arr);
来源：http://imd.yangfankeji.com

JS:   arr.length
来源：http://xty.shangyingyoupin.top

TS:   arr.length
来源：http://gsb.sysykeji.top

Java: list.size();
来源：http://eso.zdqjudy.top

Go:   len(arr)
来源：http://nwv.wangdashe.top

Ruby: arr.length; arr.size
来源：http://cmh.sjlbkw.cn

C#:   list.Count;
来源：http://uuf.fehbvm.com

[D07] 切片 / 取子数组
来源：http://xzb.yuxming.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nbz.tarul.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yur.shuidangran.top

JS:   arr.slice(1, 4);
来源：http://kmu.mhx1999.top

TS:   arr.slice(1, 4);
来源：http://meh.hongshengwenyu.top

Java: list.subList(1, 4);
来源：http://oft.yvedp.cn

Go:   arr[1:4]
来源：http://ovu.zdbjq.cn

Ruby: arr[1, 3]
来源：http://ype.yuanzhike.top

C#:   list.GetRange(1, 3);
来源：http://upl.kuanghao11.cn

[D08] 合并两个数组
来源：http://loh.guannengcc.top

Py:   a + b;  a.extend(b)
来源：http://acq.chenjidiqi.icu

PHP:  array_merge($a, $b);
来源：http://mnn.fanxiaobao.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://otc.gzhubu.top

TS:   [...a, ...b];
来源：http://mmk.cashguo.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sal.ywan-chungtsiang.top

Go:   append(a, b...)
来源：http://ude.cdnleiting.top

Ruby: a + b;  a.concat(b)
来源：http://vol.zdbjq.cn

C#:   a.Concat(b).ToList()
来源：http://lev.hcnkem.com

[D09] 排序（升序）
来源：http://nvz.fktsv.cn

Py:   sorted(arr);  arr.sort()
来源：http://mkm.gotoacloud.top

PHP:  sort($arr);
来源：http://ywl.dashuyun.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mjq.zhongyouzk.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://bmo.jinyuanbaomall.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://uve.hnqzz.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://osu.yangfankeji.com

Ruby: arr.sort
来源：http://dor.ywan-chungtsiang.top

C#:   list.Sort();
来源：http://nqo.yonumen.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://wam.guannengcc.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fbe.xuanzx.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rxw.zhongyouzk.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fih.jianghu66.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://txo.nanxinkj.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wqv.sufxvd.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wjq.xingfuxueyuan.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cpx.hcnkem.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://muy.sxryk.cn

[D11] 反转数组
来源：http://qaf.wangdashe.top

Py:   arr[::-1];  arr.reverse()
来源：http://ybq.jyoumei.cn

PHP:  array_reverse($arr);
来源：http://mla.hysaishi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nrt.hongshengwenyu.top


<!-- 参考信息 -->