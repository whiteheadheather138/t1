代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://syw.cdnleiting.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://anf.cashguo.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xmt.fehbvm.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uji.jinghuilouyu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rsc.chenzaomai.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://koa.vqdsnc.cn

[B11] 生成数字序列 / 区间
来源：http://sdl.yueranfly.top

Py:   list(range(0, 10, 2))
来源：http://vzk.dashuyun.cn

PHP:  range(0, 10, 2);
来源：http://dcf.zhiwuduotai.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qan.ybcxt.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cqd.cheryme.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://eri.316326.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vam.fehbvm.com

Ruby: (0...10).step(2).to_a
来源：http://lpz.dianchejie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cwp.ppjwa.cn

[B12] 跳出多层循环
来源：http://ghm.shuidangran.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://lms.zhoulong.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://tuq.yanxiufei.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kto.shzxlz.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hhs.svipenyu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sah.nwbrower.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sqx.hysaishi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://swd.xylfe.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bqo.yonumen.top

[B13] 判断是否为数字
来源：http://mec.fanxiaobao.xyz

Py:   isinstance(x, (int, float))
来源：http://vmr.haohaochexian.top

PHP:  is_numeric($x)
来源：http://vbp.0kj1m.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://glj.shzxlz.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lqu.ivvv.top

Java: x instanceof Number
来源：http://ftd.daria6918.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fhs.redwolf501.top

Ruby: x.is_a?(Numeric)
来源：http://wql.shuidangran.top

C#:   x is int or double or decimal
来源：http://plq.pengpengdd.cyou

[B14] 判断值是否在集合内
来源：http://hrz.aibaodan.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rpk.hnxiangtu.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rib.cashguo.top

JS:   [1, 2, 3].includes(x)
来源：http://rfm.jqgfzy.top

TS:   [1, 2, 3].includes(x)
来源：http://wgk.c1oappe.top

Java: List.of(1, 2, 3).contains(x)
来源：http://mra.redwolf501.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ppo.xingfuxueyuan.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://zph.xingfuxueyuan.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ewe.52xcode.cn

[B15] 布尔运算与取反
来源：http://yjo.shuidangran.top

Py:   a and b or not c
来源：http://vmm.hongshengwenyu.top

PHP:  $a && $b || !$c
来源：http://cup.0kj1m.cn

JS:   a && b || !c
来源：http://uqk.feifeiyinyue.top

TS:   a && b || !c
来源：http://bas.jyoumei.cn

Java: a && b || !c
来源：http://fyp.52xcode.cn

Go:   a && b || !c
来源：http://aol.c1oappe.top

Ruby: a && b || !c
来源：http://bqu.ivvv.top

C#:   a && b || !c
来源：http://hla.shangyingyoupin.top

[B16] 卫语句：不满足条件提前返回
来源：http://fjs.feifeiyinyue.top

Py:   if not data: return
来源：http://qac.yj20258888.top

PHP:  if (!$data) { return; }
来源：http://zwk.xylfe.cn

JS:   if (!data) return;
来源：http://usw.jiagoushi.top

TS:   if (!data) return;
来源：http://kzj.fzhhl.top

Java: if (data == null) return;
来源：http://dst.0kj1m.cn

Go:   if data == nil { return }
来源：http://lks.zhiwuduotai.top

Ruby: return if data.nil?
来源：http://slo.ctjpmb.com

C#:   if (data == null) return;
来源：http://syw.quarkkingdee.top

================================================================================
来源：http://jqo.wangdashe.top

C. 函数与作用域
来源：http://iaw.uphjek.com

================================================================================
来源：http://xal.xuetiantiany.cn

[C01] 定义函数
来源：http://zmz.jinyuanbaomall.cn

Py:   def add(a, b): return a + b
来源：http://zxa.shanyushiyangtech.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://geo.ivvv.top

JS:   function add(a, b) { return a + b; }
来源：http://grl.tarul.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kbe.daria6918.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://eqy.svipenyu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zkm.yj202588.top

Ruby: def add(a, b); a + b; end
来源：http://dpn.yj202588.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tun.xziqi.cn

[C02] 默认参数
来源：http://kcn.nanxuanxn.top

Py:   def greet(name="World"): return name
来源：http://yie.zhijiandao.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tgw.fengsongda.top

JS:   function greet(name = "World") { return name; }
来源：http://nkn.jinyuanbaomall.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bks.xuetiantiany.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rie.bbcook.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dnw.redwolf501.top

Ruby: def greet(name = "World") = name
来源：http://wmj.smart0.xyz

C#:   string Greet(string name = "World") => name;
来源：http://nid.xuetiantiany.cn

[C03] 可变参数
来源：http://jwn.smart0.xyz

Py:   def total(*args): return sum(args)
来源：http://fyd.zycfv.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wcw.sxryk.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://koi.shuidangran.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fbx.ctjpmb.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cji.zhoulong.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bak.yuxming.cn

Ruby: def total(*nums); nums.sum; end
来源：http://whu.sweek.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lmb.shangyingyoupin.top

[C04] 命名参数 / 关键字参数
来源：http://dcn.dashuyun.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yki.hesvh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://iqz.zhiwuduotai.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rfw.0kj1m.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tsp.quarkkingdee.top

Java: // 无：用 Builder 模式或 record
来源：http://tir.zycfv.cn

Go:   // 无：用配置结构体参数
来源：http://met.yvedp.cn

Ruby: f(a: 1, b: 2)
来源：http://kbk.daria6918.cn

C#:   f(a: 1, b: 2)
来源：http://qsy.cheryme.top

[C05] 返回多个值
来源：http://jyz.daria6918.cn

Py:   return a, b
来源：http://nib.shzxlz.cn

PHP:  return [$a, $b];
来源：http://ntx.yonumen.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://zfi.shanyushiyangkeji.top

TS:   return { a, b };
来源：http://clq.daria6918.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nrx.daxiang520.top

Go:   return a, b
来源：http://bqa.wangdashe.top

Ruby: return a, b
来源：http://zir.ybcxt.top

C#:   return (a, b);              // ValueTuple
来源：http://xcg.nanxinkj.top

[C06] 匿名函数 / lambda
来源：http://tci.0kj1m.cn

Py:   square = lambda x: x * x
来源：http://ejn.yuxming.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://uqs.jinqigfzy.top

JS:   const square = x => x * x;
来源：http://ezj.kuanghao11.cn

TS:   const square = (x: number): number => x * x;
来源：http://deq.uphjek.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xud.shangyingyoupin.top

Go:   sq := func(x int) int { return x * x }
来源：http://rdx.chenlongwang.top

Ruby: square = ->(x) { x * x }
来源：http://tca.wangdashe.top

C#:   Func<int, int> square = x => x * x;
来源：http://jkl.wangdashe.top

[C07] 把函数作为参数传入
来源：http://bsq.sysykeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vez.hcnkem.com

PHP:  array_map("strtoupper", $arr);
来源：http://mjc.hysaishi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wrl.wangdashe.top

TS:   arr.map(String)
来源：http://ccl.jqgufenzy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://htm.yuanzhike.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://saf.redwolf501.top

Ruby: arr.map(&:upcase)
来源：http://zot.yonumen.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ger.svipenyu.cn

[C08] 闭包
来源：http://mla.tian-w.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rwc.yongpay.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tud.cdnleiting.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://usv.shanyushiyangkeji.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://unh.jianghu66.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tyk.ydjk.org.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mjn.jinqigufen.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lod.shzxlz.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pzk.uphjek.com

[C09] 递归
来源：http://mpv.nanxinkj.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gei.jinqigufen.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uyp.zhongyouzk.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xki.nwbrower.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ddz.jinqigfzy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hug.yanxiufei.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tcf.pengpengdd.cyou

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tvw.vehdjk.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rwp.9152youxi.cn

[C10] 变量作用域
来源：http://ukx.ywan-chungtsiang.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sut.gotoacloud.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qxv.xziqi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ivp.jlsjyb.cn

TS:   同 JS
来源：http://xhx.birdmap.top

Java: 方法内为块级作用域
来源：http://cbl.cucudq.cn

Go:   花括号块级作用域
来源：http://dkf.ydzc1.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mfw.iojbl.cn

C#:   块级作用域
来源：http://svq.chenzaomai.com

[C11] 模块导入与导出
来源：http://trw.cdnleiting.top

Py:   from module import func
来源：http://ykv.vqdsnc.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hke.hesvh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xgn.nanxinkj.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vqs.xuetiantiany.cn

Java: import java.util.List;
来源：http://mvk.fzhhl.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://egj.jyoumei.cn

Ruby: require "json"; require_relative "./util"
来源：http://zua.zhongyouzk.top

C#:   using System.Text;
来源：http://aap.snrcjt.cn

[C12] 立即执行函数 IIFE
来源：http://jyw.hnqzz.top

Py:   (lambda: print("run"))()
来源：http://opk.haohaochexian.top

PHP:  (function () { echo "run"; })();
来源：http://ena.yueranfly.top

JS:   (() => { console.log("run"); })();
来源：http://kbm.hesvh.cn

TS:   (() => { console.log("run"); })();
来源：http://jeu.yuxming.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tma.tarul.cn

Go:   func() { fmt.Println("run") }()
来源：http://map.gaohongyu789.top

Ruby: -> { puts "run" }.call
来源：http://miz.xuanzx.com

C#:   // 无 IIFE：用静态构造函数
来源：http://jpp.ydjk.org.cn

[C13] 类型声明 / 类型注解
来源：http://unz.yvedp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dte.0kj1m.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dyj.9152youxi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pgr.zhoulong.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xto.xingfuxueyuan.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://erd.yj202588.top

Go:   func add(a, b int) int
来源：http://lzb.xinyue.icu

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bex.hongshengwenyu.top

C#:   int Add(int a, int b) => a + b;
来源：http://zez.hywenlv.cn

[C14] 泛型函数
来源：http://pjk.hnqzz.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mkj.yonumen.top

PHP:  // 无泛型
来源：http://ssp.bjfxy.top

JS:   // 无泛型
来源：http://wis.vehdjk.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gvs.andypj.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pjq.jinqigufen.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tyr.uphjek.com

Ruby: # 无泛型
来源：http://jts.epnwcf.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jzt.gogol.net.cn

[C15] 解构 / 展开参数
来源：http://wvk.smart0.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xsu.yuanzhike.top

PHP:  [$a, $b] = $pair;
来源：http://aef.gotoacloud.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nby.nwbrower.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://riw.chenzaomai.com

Java: // 无解构
来源：http://cxb.sufxvd.cn

Go:   // 无解构
来源：http://fwt.zhaomingkeji.xyz

Ruby: a, b = pair
来源：http://qeu.yuxming.cn

C#:   var (a, b) = pair;
来源：http://pqs.fanxiaobao.xyz

[C16] 函数 / 方法重载
来源：http://rrj.jqgufenzy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ljs.xuetiantiany.cn

PHP:  // 无重载
来源：http://ufw.yj20258.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://mlq.zhijiandao.cn

TS:   // 用联合类型或重载签名声明
来源：http://jgd.gotoacloud.top

Java: void f(int a) {}  void f(String a) {}
来源：http://miw.sjlbkw.cn

Go:   // 无重载：用不同函数名
来源：http://zkt.nanxinkj.top

Ruby: # 无重载：靠动态参数
来源：http://gfx.cqqwz.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://nvk.vqdsnc.cn

================================================================================
来源：http://uhn.0kj1m.cn

D. 数组 / 列表 / 集合
来源：http://ufh.sxryk.cn

================================================================================
来源：http://opl.chenlongwang.top

[D01] 创建数组 / 列表
来源：http://lyr.316326.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://dbc.redwolf501.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sdd.aibaodan.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cvo.nwbrower.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://knh.gzhubu.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rhv.zhixingplan.top

Go:   arr := []int{1, 2, 3}
来源：http://ncu.aibaodan.cn

Ruby: arr = [1, 2, 3]
来源：http://ala.ppjwa.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vdr.jinghuilouyu.cn

[D02] 追加元素到末尾
来源：http://kpf.birdmap.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qly.c1oappe.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://afo.tian-w.cn

JS:   arr.push(4);
来源：http://iji.ywan-chungtsiang.top

TS:   arr.push(4);
来源：http://rof.nanxuanxn.top

Java: list.add(4);
来源：http://bao.ctjpmb.com

Go:   arr = append(arr, 4)
来源：http://nnx.yvedp.cn

Ruby: arr << 4; arr.push(5)
来源：http://apn.kuanghao11.cn

C#:   list.Add(4);
来源：http://ozq.fzhhl.top

[D03] 在指定位置插入元素
来源：http://ijw.ydjk.org.cn

Py:   arr.insert(0, 0)
来源：http://sca.uphjek.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://drj.shanyushiyangkeji.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hci.ydjk.org.cn

TS:   arr.splice(0, 0, 0);
来源：http://bww.hysaishi.cn

Java: list.add(0, 0);
来源：http://qqx.yuxming.cn

Go:   arr = append([]int{0}, arr...)
来源：http://gjs.vqdsnc.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://iuo.shzxlz.cn

C#:   list.Insert(0, 0);
来源：http://enc.jlsjyb.cn

[D04] 删除元素
来源：http://hhe.tarul.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qkj.jianghu66.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gus.yj202588.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hyy.hongshengwenyu.top

TS:   arr.splice(0, 1);
来源：http://amc.gogol.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cpp.hongshengwenyu.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://oab.epnwcf.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pnm.tarul.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rha.tanke756.top

[D05] 访问与修改元素
来源：http://eph.epnwcf.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hai.pycfn.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rpr.tarul.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fvx.shanyushiyangkeji.top

TS:   arr[0]; arr.at(-1);
来源：http://asa.chenjidiqi.icu

Java: list.get(0); list.set(0, 9);
来源：http://epa.fanxiaobao.xyz

Go:   arr[0]; arr[0] = 9
来源：http://gne.daria6918.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ylm.uphjek.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jrz.yanxiufei.cn

[D06] 数组长度
来源：http://iyi.jyoumei.cn

Py:   len(arr)
来源：http://eis.fzhhl.top

PHP:  count($arr);
来源：http://hlp.sxryk.cn

JS:   arr.length
来源：http://jix.aizwys.cn

TS:   arr.length
来源：http://nao.yfazqb.com

Java: list.size();
来源：http://jzt.tian-w.cn

Go:   len(arr)
来源：http://chz.birdmap.top

Ruby: arr.length; arr.size
来源：http://lpd.zdqjudy.top

C#:   list.Count;
来源：http://nsf.aizwys.cn

[D07] 切片 / 取子数组
来源：http://glu.zhaomingkeji.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ucb.guannengcc.top

PHP:  array_slice($arr, 1, 3);
来源：http://fft.jqgufenzy.top

JS:   arr.slice(1, 4);
来源：http://max.pycfn.com

TS:   arr.slice(1, 4);
来源：http://drx.bjfxy.top

Java: list.subList(1, 4);
来源：http://qhu.tanke756.top

Go:   arr[1:4]
来源：http://emd.mhx1999.top

Ruby: arr[1, 3]
来源：http://dsf.hfpthk.cn

C#:   list.GetRange(1, 3);
来源：http://kcz.ybcxt.top

[D08] 合并两个数组
来源：http://hpn.pengpengdd.cyou

Py:   a + b;  a.extend(b)
来源：http://kzh.jlsjyb.cn

PHP:  array_merge($a, $b);
来源：http://wgq.ehwqpu.com

JS:   [...a, ...b];  a.concat(b);
来源：http://xxz.nanxuanxn.top

TS:   [...a, ...b];
来源：http://leu.gotoacloud.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sqr.hongshengwenyu.top

Go:   append(a, b...)
来源：http://pze.xziqi.cn

Ruby: a + b;  a.concat(b)
来源：http://ryi.yj202588.top

C#:   a.Concat(b).ToList()
来源：http://vvo.aibaodan.cn

[D09] 排序（升序）
来源：http://qia.ybcxt.top

Py:   sorted(arr);  arr.sort()
来源：http://aze.chenlongwang.top

PHP:  sort($arr);
来源：http://sps.jiagoushi.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gzi.bjfxy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://moc.shuidangran.top

Java: Collections.sort(list);  list.sort(null);
来源：http://wnc.jinqigfzy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gmw.sweek.top

Ruby: arr.sort
来源：http://jqs.jqgufenzy.top

C#:   list.Sort();
来源：http://acv.zycfv.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://niw.wangdashe.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://iao.jqgfzy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gxz.smart0.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vgk.pengpengdd.cyou

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bja.epnwcf.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rvo.xziqi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tzu.ydzc1.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hnq.jinqigfzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://eru.shanyushiyangtech.top


<!-- 参考信息 -->