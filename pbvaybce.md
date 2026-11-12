代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dzb.ppjwa.cn

Ruby: (0...10).step(2).to_a
来源：http://ewf.xuetiantiany.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ohx.uphjek.com

[B12] 跳出多层循环
来源：http://zwq.pycfn.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://rje.smart0.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://sha.daxiang520.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://usu.quarkkingdee.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lgh.cucudq.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://smb.52xcode.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hkc.xuetiantiany.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://efh.xuetiantiany.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://abn.uphjek.com

[B13] 判断是否为数字
来源：http://zsp.ehwqpu.com

Py:   isinstance(x, (int, float))
来源：http://cez.yangfankeji.com

PHP:  is_numeric($x)
来源：http://hdz.cucudq.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mzz.xuanzx.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kgg.yuanzhike.top

Java: x instanceof Number
来源：http://ulq.zhoulong.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zuy.haohaochexian.top

Ruby: x.is_a?(Numeric)
来源：http://ruk.zhiwuduotai.top

C#:   x is int or double or decimal
来源：http://usm.pengpengdd.cyou

[B14] 判断值是否在集合内
来源：http://txe.ehwqpu.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mvf.nwbrower.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qol.zhiwuduotai.top

JS:   [1, 2, 3].includes(x)
来源：http://yrq.yuanzhike.top

TS:   [1, 2, 3].includes(x)
来源：http://new.redwolf501.top

Java: List.of(1, 2, 3).contains(x)
来源：http://sms.quarkkingdee.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vqc.chenjidiqi.icu

Ruby: [1, 2, 3].include?(x)
来源：http://bsg.yuanzhike.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vgw.jiagoushi.top

[B15] 布尔运算与取反
来源：http://kwd.hywenlv.cn

Py:   a and b or not c
来源：http://eln.hywenlv.cn

PHP:  $a && $b || !$c
来源：http://aps.ydzc1.top

JS:   a && b || !c
来源：http://rlb.chenzaomai.com

TS:   a && b || !c
来源：http://ayh.bbcook.cn

Java: a && b || !c
来源：http://omv.hfpthk.cn

Go:   a && b || !c
来源：http://ojl.cashguo.top

Ruby: a && b || !c
来源：http://iwd.ybcxt.top

C#:   a && b || !c
来源：http://moe.fzhhl.top

[B16] 卫语句：不满足条件提前返回
来源：http://ydg.9152youxi.cn

Py:   if not data: return
来源：http://juf.sweek.top

PHP:  if (!$data) { return; }
来源：http://olc.hcnkem.com

JS:   if (!data) return;
来源：http://qwa.jinqigfzy.top

TS:   if (!data) return;
来源：http://ljm.iojbl.cn

Java: if (data == null) return;
来源：http://zyj.sweek.top

Go:   if data == nil { return }
来源：http://btn.hywenlv.cn

Ruby: return if data.nil?
来源：http://xkx.ivvv.top

C#:   if (data == null) return;
来源：http://tic.zycfv.cn

================================================================================
来源：http://yqb.yuxming.cn

C. 函数与作用域
来源：http://mbf.yangfankeji.com

================================================================================
来源：http://jto.chenjidiqi.icu

[C01] 定义函数
来源：http://kbl.yuanzhike.top

Py:   def add(a, b): return a + b
来源：http://cjt.shanyushiyangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jre.jianghu66.top

JS:   function add(a, b) { return a + b; }
来源：http://txv.ybcxt.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uwd.zdqjudy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://xtn.c1oappe.top

Go:   func add(a, b int) int { return a + b }
来源：http://nzl.sufxvd.cn

Ruby: def add(a, b); a + b; end
来源：http://zrz.daxiang520.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vku.tarul.cn

[C02] 默认参数
来源：http://xci.xuanzx.com

Py:   def greet(name="World"): return name
来源：http://idl.zdbjq.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lol.fanxiaobao.xyz

JS:   function greet(name = "World") { return name; }
来源：http://hsy.jqgufenzy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://gqd.epnwcf.com

Java: // 无默认参数：方法重载或 Optional
来源：http://sjl.dashuyun.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://uah.yvedp.cn

Ruby: def greet(name = "World") = name
来源：http://clb.fehbvm.com

C#:   string Greet(string name = "World") => name;
来源：http://ziv.yuanzhike.top

[C03] 可变参数
来源：http://hbn.jqgufenzy.top

Py:   def total(*args): return sum(args)
来源：http://rea.zhaomingkeji.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bky.jinqigufen.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ozv.haohaochexian.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hal.zdbjq.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://btg.wangshuangyany.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lgb.epnwcf.com

Ruby: def total(*nums); nums.sum; end
来源：http://gpn.hfpthk.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qid.gogol.net.cn

[C04] 命名参数 / 关键字参数
来源：http://xek.hesvh.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ohg.zhaomingkeji.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ykq.yuxming.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://olm.hcnkem.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dgm.zhaomingkeji.xyz

Java: // 无：用 Builder 模式或 record
来源：http://sog.ywan-chungtsiang.top

Go:   // 无：用配置结构体参数
来源：http://ehq.vqdsnc.cn

Ruby: f(a: 1, b: 2)
来源：http://hrs.xziqi.cn

C#:   f(a: 1, b: 2)
来源：http://ive.sysykeji.top

[C05] 返回多个值
来源：http://hfs.hywenlv.cn

Py:   return a, b
来源：http://emk.zhixingplan.top

PHP:  return [$a, $b];
来源：http://tsp.xuanzx.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://lnw.hesvh.cn

TS:   return { a, b };
来源：http://wgp.jyoumei.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dgg.wangdashe.top

Go:   return a, b
来源：http://zlh.jlsjyb.cn

Ruby: return a, b
来源：http://ery.yj202588.top

C#:   return (a, b);              // ValueTuple
来源：http://gsl.wangdashe.top

[C06] 匿名函数 / lambda
来源：http://vqg.hywenlv.cn

Py:   square = lambda x: x * x
来源：http://zpr.mhx1999.top

PHP:  $square = fn($x) => $x * $x;
来源：http://nax.jinqigfzy.top

JS:   const square = x => x * x;
来源：http://lxh.yj202588.top

TS:   const square = (x: number): number => x * x;
来源：http://niq.zdbjq.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://exm.birdmap.top

Go:   sq := func(x int) int { return x * x }
来源：http://dfc.sweek.top

Ruby: square = ->(x) { x * x }
来源：http://ziu.fengsongda.top

C#:   Func<int, int> square = x => x * x;
来源：http://zhn.shangyingyoupin.top

[C07] 把函数作为参数传入
来源：http://auo.fktsv.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://aul.jqgufenzy.top

PHP:  array_map("strtoupper", $arr);
来源：http://jrv.gotoacloud.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://frx.fzhhl.top

TS:   arr.map(String)
来源：http://unp.9152youxi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cdl.yanxiufei.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qpt.jinqigufen.top

Ruby: arr.map(&:upcase)
来源：http://iil.hnxiangtu.top

C#:   arr.Select(s => s.ToUpper())
来源：http://qat.meibo888.top

[C08] 闭包
来源：http://tko.hfpthk.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ebe.hywenlv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vqz.hnqzz.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fnl.hfpthk.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ehv.cashguo.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hbv.cqqwz.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vfo.fktsv.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lyl.zdbjq.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xlr.52xcode.cn

[C09] 递归
来源：http://gnr.zycfv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://buk.cheryme.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yqd.haohaochexian.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hxt.jqgufenzy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cgd.jinghuilouyu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kiz.yfazqb.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zgt.hesvh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://njz.shangyingyoupin.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bxd.yuxming.cn

[C10] 变量作用域
来源：http://ugh.bbcook.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vjz.iojbl.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rfw.yvedp.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pam.guowangkeji.top

TS:   同 JS
来源：http://fvh.0kj1m.cn

Java: 方法内为块级作用域
来源：http://bsy.yj20258.top

Go:   花括号块级作用域
来源：http://wmq.shanyushiyangtech.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fuf.hfpthk.cn

C#:   块级作用域
来源：http://nnd.chenlongwang.top

[C11] 模块导入与导出
来源：http://nfa.hammf.cn

Py:   from module import func
来源：http://yie.daria6918.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://nqq.hfpthk.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://djo.wangshuangyany.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://iim.daria6918.cn

Java: import java.util.List;
来源：http://kkl.dashuyun.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fpo.nanxuanxn.top

Ruby: require "json"; require_relative "./util"
来源：http://mnz.fzhhl.top

C#:   using System.Text;
来源：http://grs.jinghuilouyu.cn

[C12] 立即执行函数 IIFE
来源：http://leb.xinyue.icu

Py:   (lambda: print("run"))()
来源：http://ifs.tarul.cn

PHP:  (function () { echo "run"; })();
来源：http://dgz.cqqwz.cn

JS:   (() => { console.log("run"); })();
来源：http://fbn.shzxlz.cn

TS:   (() => { console.log("run"); })();
来源：http://qwi.fehbvm.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://swi.aizwys.cn

Go:   func() { fmt.Println("run") }()
来源：http://jcv.guannengcc.top

Ruby: -> { puts "run" }.call
来源：http://nae.sysykeji.top

C#:   // 无 IIFE：用静态构造函数
来源：http://vcz.hcnkem.com

[C13] 类型声明 / 类型注解
来源：http://ssb.fktsv.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://elq.gotoacloud.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://usu.zhijiandao.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lkj.jinqigfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kzc.dashuyun.cn

Java: int add(int a, int b) { return a + b; }
来源：http://kfq.zhaomingkeji.xyz

Go:   func add(a, b int) int
来源：http://gmi.52xcode.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jvz.c1oappe.top

C#:   int Add(int a, int b) => a + b;
来源：http://jgk.sxryk.cn

[C14] 泛型函数
来源：http://jmu.ywan-chungtsiang.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dxf.jinghuilouyu.cn

PHP:  // 无泛型
来源：http://tiz.andypj.xyz

JS:   // 无泛型
来源：http://ofy.zhiwuduotai.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fyp.shangyingyoupin.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xta.gaohongyu789.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://oai.jqgufenzy.top

Ruby: # 无泛型
来源：http://quy.cucudq.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nho.wangdashe.top

[C15] 解构 / 展开参数
来源：http://ili.ywan-chungtsiang.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rxz.yuxming.cn

PHP:  [$a, $b] = $pair;
来源：http://set.cdnleiting.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vdc.jqgfzy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jax.xziqi.cn

Java: // 无解构
来源：http://haq.tarul.cn

Go:   // 无解构
来源：http://wyj.jianghu66.top

Ruby: a, b = pair
来源：http://zng.gzhubu.top

C#:   var (a, b) = pair;
来源：http://vcs.sjlbkw.cn

[C16] 函数 / 方法重载
来源：http://ikw.jinqigufen.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sne.hnqzz.top

PHP:  // 无重载
来源：http://dfp.aizwys.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://pcj.zhoulong.xyz

TS:   // 用联合类型或重载签名声明
来源：http://ghn.chenjidiqi.icu

Java: void f(int a) {}  void f(String a) {}
来源：http://xzm.yonumen.top

Go:   // 无重载：用不同函数名
来源：http://anx.yj202588.top

Ruby: # 无重载：靠动态参数
来源：http://thr.gzhubu.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://nzg.yongpay.top

================================================================================
来源：http://sdr.hcnkem.com

D. 数组 / 列表 / 集合
来源：http://nxn.sjlbkw.cn

================================================================================
来源：http://qlp.daxiang520.top

[D01] 创建数组 / 列表
来源：http://hbs.yuanzhike.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://tom.havefunace.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ipr.zhiwuduotai.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://efa.chenzaomai.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://wfo.zdbjq.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lsj.yuxming.cn

Go:   arr := []int{1, 2, 3}
来源：http://nnw.nanxinkj.top

Ruby: arr = [1, 2, 3]
来源：http://cys.fzhhl.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zju.xziqi.cn

[D02] 追加元素到末尾
来源：http://vrg.ehwqpu.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bnq.yj20258888.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://adf.chenjidiqi.icu

JS:   arr.push(4);
来源：http://gfv.ehwqpu.com

TS:   arr.push(4);
来源：http://lai.52xcode.cn

Java: list.add(4);
来源：http://lul.jiagoushi.top

Go:   arr = append(arr, 4)
来源：http://dkd.ybcxt.top

Ruby: arr << 4; arr.push(5)
来源：http://dkn.zhengqikj.top

C#:   list.Add(4);
来源：http://tsu.kuanghao11.cn

[D03] 在指定位置插入元素
来源：http://vmy.0kj1m.cn

Py:   arr.insert(0, 0)
来源：http://cpg.jinqigufen.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dqf.fzhhl.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mrm.vqdsnc.cn

TS:   arr.splice(0, 0, 0);
来源：http://sgj.ivvv.top

Java: list.add(0, 0);
来源：http://umw.hesvh.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qew.c1oappe.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fry.jinqigufen.top

C#:   list.Insert(0, 0);
来源：http://jhi.redwolf501.top

[D04] 删除元素
来源：http://hqf.dianchejie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gug.cdnleiting.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uwo.snrcjt.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://faw.birdmap.top

TS:   arr.splice(0, 1);
来源：http://bui.yueranfly.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hnx.zdbjq.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lbq.yj202588.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vof.jinghuilouyu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://few.jinqigufen.top

[D05] 访问与修改元素
来源：http://pgp.andypj.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zth.cucudq.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uqt.zdbjq.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://krl.vehdjk.com

TS:   arr[0]; arr.at(-1);
来源：http://etg.andypj.xyz

Java: list.get(0); list.set(0, 9);
来源：http://hgw.316326.xyz

Go:   arr[0]; arr[0] = 9
来源：http://kka.zhixingplan.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yxc.xziqi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nbi.cqqwz.cn

[D06] 数组长度
来源：http://hft.xuetiantiany.cn

Py:   len(arr)
来源：http://sdq.xylfe.cn

PHP:  count($arr);
来源：http://asm.daxiang520.top

JS:   arr.length
来源：http://wlp.ydzc1.top

TS:   arr.length
来源：http://rbg.daria6918.cn

Java: list.size();
来源：http://gog.smart0.xyz

Go:   len(arr)
来源：http://lhj.jiagoushi.top

Ruby: arr.length; arr.size
来源：http://bbs.tianlin.xyz

C#:   list.Count;
来源：http://rij.pycfn.com

[D07] 切片 / 取子数组
来源：http://edb.tianlin.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qsx.yanxiufei.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yqe.meibo888.top

JS:   arr.slice(1, 4);
来源：http://htj.jinyuanbaomall.cn

TS:   arr.slice(1, 4);
来源：http://muw.hywenlv.cn

Java: list.subList(1, 4);
来源：http://lwd.jqgufenzy.top

Go:   arr[1:4]
来源：http://hqr.zhixingplan.top

Ruby: arr[1, 3]
来源：http://olq.yanxiufei.cn

C#:   list.GetRange(1, 3);
来源：http://ooe.sysykeji.top

[D08] 合并两个数组
来源：http://ypm.c1oappe.top

Py:   a + b;  a.extend(b)
来源：http://efg.birdmap.top

PHP:  array_merge($a, $b);
来源：http://xwq.ctjpmb.com

JS:   [...a, ...b];  a.concat(b);
来源：http://cyq.hesvh.cn

TS:   [...a, ...b];
来源：http://qpq.hnxiangtu.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fwp.fehbvm.com

Go:   append(a, b...)
来源：http://nzh.hywenlv.cn

Ruby: a + b;  a.concat(b)
来源：http://fsk.shangyingyoupin.top

C#:   a.Concat(b).ToList()
来源：http://lhr.vehdjk.com

[D09] 排序（升序）
来源：http://sat.jinghuilouyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://jtn.cheryme.top

PHP:  sort($arr);
来源：http://gzo.xziqi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hmp.jlsjyb.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://jlq.ivvv.top

Java: Collections.sort(list);  list.sort(null);
来源：http://hjo.feifeiyinyue.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xkb.ydzc1.top

Ruby: arr.sort
来源：http://gcz.jqgufenzy.top

C#:   list.Sort();
来源：http://sgq.xingfuxueyuan.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://sje.epnwcf.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ffj.cucudq.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zcf.daria6918.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hih.snrcjt.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://uhc.dashuyun.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gmz.hfpthk.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ygj.havefunace.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ysa.jqgufenzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ayn.hysaishi.cn

[D11] 反转数组
来源：http://qqn.gogol.net.cn

Py:   arr[::-1];  arr.reverse()
来源：http://nug.yj20258888.top

PHP:  array_reverse($arr);
来源：http://wro.havefunace.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ezo.hywenlv.cn

TS:   [...arr].reverse();
来源：http://rvt.shzxlz.cn

Java: Collections.reverse(list);
来源：http://ncs.yj20258888.top

Go:   slices.Reverse(arr)
来源：http://dbu.redwolf501.top

Ruby: arr.reverse
来源：http://dst.shanyushiyangkeji.top

C#:   list.Reverse();
来源：http://uuw.jinghuilouyu.cn

[D12] 查找元素下标
来源：http://vtp.jinghuilouyu.cn

Py:   arr.index(x);  x in arr
来源：http://sey.bbcook.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fjc.wangshuangyany.cn


<!-- 参考信息 -->