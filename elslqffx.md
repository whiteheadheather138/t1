代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dwp.zdbjq.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://usx.pengpengdd.cyou

[B11] 生成数字序列 / 区间
来源：http://eab.snrcjt.cn

Py:   list(range(0, 10, 2))
来源：http://lik.gogol.net.cn

PHP:  range(0, 10, 2);
来源：http://ric.gaohongyu789.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rnq.zhengqikj.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vls.xuanzx.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zxm.zdbjq.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hnm.gogol.net.cn

Ruby: (0...10).step(2).to_a
来源：http://jha.tianlin.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kdg.fanxiaobao.xyz

[B12] 跳出多层循环
来源：http://qhd.fanxiaobao.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://bvi.ivvv.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://rys.ctjpmb.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mwp.jyoumei.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jcy.sufxvd.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ryu.9152youxi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ngx.guannengcc.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tzr.chenzaomai.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xea.gzhubu.top

[B13] 判断是否为数字
来源：http://pow.316326.xyz

Py:   isinstance(x, (int, float))
来源：http://xnx.ivvv.top

PHP:  is_numeric($x)
来源：http://ssb.yonumen.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rxj.yuxming.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oou.chenzaomai.com

Java: x instanceof Number
来源：http://vmi.feifeiyinyue.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://thg.jinqigfzy.top

Ruby: x.is_a?(Numeric)
来源：http://llz.iojbl.cn

C#:   x is int or double or decimal
来源：http://bsm.xylfe.cn

[B14] 判断值是否在集合内
来源：http://miv.dashuyun.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xko.hnxiangtu.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hzc.epnwcf.com

JS:   [1, 2, 3].includes(x)
来源：http://kro.bbcook.cn

TS:   [1, 2, 3].includes(x)
来源：http://ise.ppjwa.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://plp.9152youxi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hvu.ybcxt.top

Ruby: [1, 2, 3].include?(x)
来源：http://zqw.meibo888.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qwm.ppjwa.cn

[B15] 布尔运算与取反
来源：http://mse.havefunace.top

Py:   a and b or not c
来源：http://fks.zhoulong.xyz

PHP:  $a && $b || !$c
来源：http://tjo.zhixingplan.top

JS:   a && b || !c
来源：http://lyf.vqdsnc.cn

TS:   a && b || !c
来源：http://dnh.yj202588.top

Java: a && b || !c
来源：http://zbk.yonumen.top

Go:   a && b || !c
来源：http://grm.iojbl.cn

Ruby: a && b || !c
来源：http://mnf.dashuyun.cn

C#:   a && b || !c
来源：http://upb.aibaodan.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fhx.aizwys.cn

Py:   if not data: return
来源：http://qxl.hywenlv.cn

PHP:  if (!$data) { return; }
来源：http://per.zycfv.cn

JS:   if (!data) return;
来源：http://vrf.xuetiantiany.cn

TS:   if (!data) return;
来源：http://oyf.zhijiandao.cn

Java: if (data == null) return;
来源：http://loj.guowangkeji.top

Go:   if data == nil { return }
来源：http://wtx.yuanzhike.top

Ruby: return if data.nil?
来源：http://ybo.ydzc1.top

C#:   if (data == null) return;
来源：http://tzk.fengsongda.top

================================================================================
来源：http://epa.shzxlz.cn

C. 函数与作用域
来源：http://exy.epnwcf.com

================================================================================
来源：http://jns.cdnleiting.top

[C01] 定义函数
来源：http://ylu.vqdsnc.cn

Py:   def add(a, b): return a + b
来源：http://urm.iojbl.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cpq.tianlin.xyz

JS:   function add(a, b) { return a + b; }
来源：http://jyy.xinyue.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://riy.nanxinkj.top

Java: static int add(int a, int b) { return a + b; }
来源：http://wet.dianchejie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://aun.birdmap.top

Ruby: def add(a, b); a + b; end
来源：http://spe.nanxinkj.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mii.bbcook.cn

[C02] 默认参数
来源：http://zxf.tarul.cn

Py:   def greet(name="World"): return name
来源：http://ury.cucudq.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qkw.yuxming.cn

JS:   function greet(name = "World") { return name; }
来源：http://cuz.dashuyun.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://oqy.shzxlz.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://yap.yuxming.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mep.yueranfly.top

Ruby: def greet(name = "World") = name
来源：http://xby.zhijiandao.cn

C#:   string Greet(string name = "World") => name;
来源：http://fnf.yvedp.cn

[C03] 可变参数
来源：http://xxp.shzxlz.cn

Py:   def total(*args): return sum(args)
来源：http://bwu.aibaodan.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zdq.fzhhl.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nfm.tanke756.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jcu.hammf.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zvf.aibaodan.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jrm.sysykeji.top

Ruby: def total(*nums); nums.sum; end
来源：http://iey.zhixingplan.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fmt.daxiang520.top

[C04] 命名参数 / 关键字参数
来源：http://fnf.ppjwa.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gfi.chenjidiqi.icu

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nfe.zhiwuduotai.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xrc.tianlin.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uad.ybcxt.top

Java: // 无：用 Builder 模式或 record
来源：http://woe.dashuyun.cn

Go:   // 无：用配置结构体参数
来源：http://exf.kuanghao11.cn

Ruby: f(a: 1, b: 2)
来源：http://jot.316326.xyz

C#:   f(a: 1, b: 2)
来源：http://czn.bbcook.cn

[C05] 返回多个值
来源：http://rwz.jinqigufen.top

Py:   return a, b
来源：http://uby.jianghu66.top

PHP:  return [$a, $b];
来源：http://sea.xingfuxueyuan.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://azk.svipenyu.cn

TS:   return { a, b };
来源：http://jhi.jqgufenzy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://csp.andypj.xyz

Go:   return a, b
来源：http://ywr.xylfe.cn

Ruby: return a, b
来源：http://voq.hongshengwenyu.top

C#:   return (a, b);              // ValueTuple
来源：http://hez.zhiwuduotai.top

[C06] 匿名函数 / lambda
来源：http://qke.hysaishi.cn

Py:   square = lambda x: x * x
来源：http://bbt.sufxvd.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://rpq.yvedp.cn

JS:   const square = x => x * x;
来源：http://esu.tianlin.xyz

TS:   const square = (x: number): number => x * x;
来源：http://yja.jinqigfzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://uxt.sxryk.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ayn.gotoacloud.top

Ruby: square = ->(x) { x * x }
来源：http://ipj.yuxming.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vcu.pengpengdd.cyou

[C07] 把函数作为参数传入
来源：http://uoi.smart0.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nnu.shangyingyoupin.top

PHP:  array_map("strtoupper", $arr);
来源：http://lem.ppjwa.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dap.aizwys.cn

TS:   arr.map(String)
来源：http://abm.sxryk.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tjq.yuxming.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jgh.ivvv.top

Ruby: arr.map(&:upcase)
来源：http://eru.xuetiantiany.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hlk.52xcode.cn

[C08] 闭包
来源：http://hwv.birdmap.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dch.guannengcc.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hfy.yj20258.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zeh.xuetiantiany.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rrd.sufxvd.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ygv.jianghu66.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hkl.hcnkem.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jsd.pengpengdd.cyou

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hmp.vqdsnc.cn

[C09] 递归
来源：http://nyu.zhengqikj.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fow.havefunace.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ljx.xingfuxueyuan.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://exy.52xcode.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bpi.xylfe.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qsj.hcnkem.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pkm.daxiang520.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://chm.guowangkeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vow.shanyushiyangkeji.top

[C10] 变量作用域
来源：http://sft.fengsongda.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://psh.snrcjt.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hhy.daria6918.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://czh.ywan-chungtsiang.top

TS:   同 JS
来源：http://vwo.iojbl.cn

Java: 方法内为块级作用域
来源：http://xmr.nanxuanxn.top

Go:   花括号块级作用域
来源：http://nhc.xingfuxueyuan.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lfq.tianlin.xyz

C#:   块级作用域
来源：http://rnx.yueranfly.top

[C11] 模块导入与导出
来源：http://jhj.epnwcf.com

Py:   from module import func
来源：http://ydt.zhoulong.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://nup.aizwys.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://stz.fanxiaobao.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bsc.0kj1m.cn

Java: import java.util.List;
来源：http://omz.ctjpmb.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wos.haohaochexian.top

Ruby: require "json"; require_relative "./util"
来源：http://uba.mhx1999.top

C#:   using System.Text;
来源：http://gqb.guowangkeji.top

[C12] 立即执行函数 IIFE
来源：http://lfp.sweek.top

Py:   (lambda: print("run"))()
来源：http://pxb.feifeiyinyue.top

PHP:  (function () { echo "run"; })();
来源：http://tgo.chenjidiqi.icu

JS:   (() => { console.log("run"); })();
来源：http://qzu.jyoumei.cn

TS:   (() => { console.log("run"); })();
来源：http://yiz.yj20258.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xtr.jlsjyb.cn

Go:   func() { fmt.Println("run") }()
来源：http://ljt.dashuyun.cn

Ruby: -> { puts "run" }.call
来源：http://vlg.shangyingyoupin.top

C#:   // 无 IIFE：用静态构造函数
来源：http://zjc.cqqwz.cn

[C13] 类型声明 / 类型注解
来源：http://ybt.nanxuanxn.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mkz.xziqi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://coc.aibaodan.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bty.hnxiangtu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://frd.zhongyouzk.top

Java: int add(int a, int b) { return a + b; }
来源：http://gxe.uphjek.com

Go:   func add(a, b int) int
来源：http://fbi.ppjwa.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://veq.hfpthk.cn

C#:   int Add(int a, int b) => a + b;
来源：http://rnr.9152youxi.cn

[C14] 泛型函数
来源：http://dwh.jqgfzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pgj.vehdjk.com

PHP:  // 无泛型
来源：http://rjx.shuidangran.top

JS:   // 无泛型
来源：http://nar.zdqjudy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://llc.zdbjq.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://edr.yuanzhike.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xgn.aibaodan.cn

Ruby: # 无泛型
来源：http://oke.sysykeji.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lqf.hnqzz.top

[C15] 解构 / 展开参数
来源：http://hbc.9152youxi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kwd.xylfe.cn

PHP:  [$a, $b] = $pair;
来源：http://rqu.yangfankeji.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://igw.xuanzx.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://syu.yj20258.top

Java: // 无解构
来源：http://cqm.gogol.net.cn

Go:   // 无解构
来源：http://roq.hammf.cn

Ruby: a, b = pair
来源：http://yba.fzhhl.top

C#:   var (a, b) = pair;
来源：http://zmg.yj20258.top

[C16] 函数 / 方法重载
来源：http://gem.dashuyun.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ugw.fanxiaobao.xyz

PHP:  // 无重载
来源：http://hqu.cashguo.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://uza.sxryk.cn

TS:   // 用联合类型或重载签名声明
来源：http://tbs.nanxuanxn.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ild.dianchejie.cn

Go:   // 无重载：用不同函数名
来源：http://hpz.guowangkeji.top

Ruby: # 无重载：靠动态参数
来源：http://qoz.hnxiangtu.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://mko.zhijiandao.cn

================================================================================
来源：http://hlo.pengpengdd.cyou

D. 数组 / 列表 / 集合
来源：http://yrn.yongpay.top

================================================================================
来源：http://mzi.feifeiyinyue.top

[D01] 创建数组 / 列表
来源：http://lzd.hesvh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rwo.cdnleiting.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tbg.fanxiaobao.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ysx.ydzc1.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://mnx.xziqi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cxw.ywan-chungtsiang.top

Go:   arr := []int{1, 2, 3}
来源：http://pjf.fktsv.cn

Ruby: arr = [1, 2, 3]
来源：http://vrn.zhijiandao.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ipz.cdnleiting.top

[D02] 追加元素到末尾
来源：http://jzt.hammf.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tgn.bbcook.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://eyf.xylfe.cn

JS:   arr.push(4);
来源：http://pkj.svipenyu.cn

TS:   arr.push(4);
来源：http://kxd.sweek.top

Java: list.add(4);
来源：http://xdb.hysaishi.cn

Go:   arr = append(arr, 4)
来源：http://uap.316326.xyz

Ruby: arr << 4; arr.push(5)
来源：http://wok.c1oappe.top

C#:   list.Add(4);
来源：http://hrn.xinyue.icu

[D03] 在指定位置插入元素
来源：http://ual.chenzaomai.com

Py:   arr.insert(0, 0)
来源：http://vqm.yangfankeji.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dui.jianghu66.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://krg.yangfankeji.com

TS:   arr.splice(0, 0, 0);
来源：http://lgf.jqgufenzy.top

Java: list.add(0, 0);
来源：http://wkq.yuanzhike.top

Go:   arr = append([]int{0}, arr...)
来源：http://lbf.zhengqikj.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sfy.cucudq.cn

C#:   list.Insert(0, 0);
来源：http://vep.jqgfzy.top

[D04] 删除元素
来源：http://jvs.jinqigufen.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wnc.zhaomingkeji.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mop.xinyue.icu

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jse.ehwqpu.com

TS:   arr.splice(0, 1);
来源：http://bpc.fzhhl.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yeb.hongshengwenyu.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fht.cucudq.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uzk.meibo888.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jbu.hongshengwenyu.top

[D05] 访问与修改元素
来源：http://syl.cashguo.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dkm.sufxvd.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://aqf.havefunace.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://haa.xuanzx.com

TS:   arr[0]; arr.at(-1);
来源：http://hpt.wangdashe.top

Java: list.get(0); list.set(0, 9);
来源：http://nib.cucudq.cn

Go:   arr[0]; arr[0] = 9
来源：http://eyy.jinqigfzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pme.hongshengwenyu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bki.havefunace.top

[D06] 数组长度
来源：http://nie.nwbrower.top

Py:   len(arr)
来源：http://jwz.fengsongda.top

PHP:  count($arr);
来源：http://lhf.sweek.top

JS:   arr.length
来源：http://als.jinghuilouyu.cn

TS:   arr.length
来源：http://jwe.wangdashe.top

Java: list.size();
来源：http://tta.yj20258.top

Go:   len(arr)
来源：http://vll.zhengqikj.top

Ruby: arr.length; arr.size
来源：http://xvv.svipenyu.cn

C#:   list.Count;
来源：http://jcz.xuanzx.com

[D07] 切片 / 取子数组
来源：http://eur.aizwys.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lke.bjfxy.top

PHP:  array_slice($arr, 1, 3);
来源：http://glb.shuidangran.top

JS:   arr.slice(1, 4);
来源：http://zzo.haohaochexian.top

TS:   arr.slice(1, 4);
来源：http://inb.hcnkem.com

Java: list.subList(1, 4);
来源：http://vbz.cheryme.top

Go:   arr[1:4]
来源：http://iba.nanxinkj.top

Ruby: arr[1, 3]
来源：http://cjo.tarul.cn

C#:   list.GetRange(1, 3);
来源：http://iul.bjfxy.top

[D08] 合并两个数组
来源：http://qrl.gotoacloud.top

Py:   a + b;  a.extend(b)
来源：http://kex.jinqigfzy.top

PHP:  array_merge($a, $b);
来源：http://fuo.jinghuilouyu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://lmo.hesvh.cn

TS:   [...a, ...b];
来源：http://kcx.wangshuangyany.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zro.daria6918.cn

Go:   append(a, b...)
来源：http://ccl.shuidangran.top

Ruby: a + b;  a.concat(b)
来源：http://jyn.cheryme.top

C#:   a.Concat(b).ToList()
来源：http://nby.yj202588.top

[D09] 排序（升序）
来源：http://xeq.zhixingplan.top

Py:   sorted(arr);  arr.sort()
来源：http://yxb.ppjwa.cn

PHP:  sort($arr);
来源：http://hat.nanxuanxn.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yux.shuidangran.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://byh.aizwys.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hvr.nanxinkj.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://iap.uphjek.com

Ruby: arr.sort
来源：http://ioh.tanke756.top

C#:   list.Sort();
来源：http://vmx.jinqigufen.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://slb.hysaishi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lky.birdmap.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dou.gotoacloud.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nle.pengpengdd.cyou

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qhy.ydjk.org.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vcj.sxryk.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hmv.zhengqikj.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://obe.ydjk.org.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rjx.tanke756.top

[D11] 反转数组
来源：http://xcr.xingfuxueyuan.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://uea.zhijiandao.cn

PHP:  array_reverse($arr);
来源：http://sor.ehwqpu.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mhy.feifeiyinyue.top


<!-- 参考信息 -->