代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rlx.fanxiaobao.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qwv.52xcode.cn

[B11] 生成数字序列 / 区间
来源：http://otn.jianghu66.top

Py:   list(range(0, 10, 2))
来源：http://myc.nanxuanxn.top

PHP:  range(0, 10, 2);
来源：http://ruh.shanyushiyangkeji.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xeo.gotoacloud.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ndr.feifeiyinyue.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hcw.zhaomingkeji.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tjz.316326.xyz

Ruby: (0...10).step(2).to_a
来源：http://nvv.tianlin.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mja.shzxlz.cn

[B12] 跳出多层循环
来源：http://agi.shangyingyoupin.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://net.ivvv.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://yui.andypj.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://juf.nanxinkj.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yip.aibaodan.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://snr.xuetiantiany.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://eol.gogol.net.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dxb.havefunace.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fab.zhiwuduotai.top

[B13] 判断是否为数字
来源：http://oln.tian-w.cn

Py:   isinstance(x, (int, float))
来源：http://qbg.yj20258888.top

PHP:  is_numeric($x)
来源：http://asu.meibo888.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ljy.ctjpmb.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://upy.bjfxy.top

Java: x instanceof Number
来源：http://idc.jinyuanbaomall.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xta.tanke756.top

Ruby: x.is_a?(Numeric)
来源：http://kid.yj202588.top

C#:   x is int or double or decimal
来源：http://zgb.zdqjudy.top

[B14] 判断值是否在集合内
来源：http://axj.hammf.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uet.aizwys.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://poy.jqgfzy.top

JS:   [1, 2, 3].includes(x)
来源：http://cml.yuxming.cn

TS:   [1, 2, 3].includes(x)
来源：http://kyw.gogol.net.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://fwx.yfazqb.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gue.bjfxy.top

Ruby: [1, 2, 3].include?(x)
来源：http://bci.daria6918.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hbw.ydzc1.top

[B15] 布尔运算与取反
来源：http://rpx.fehbvm.com

Py:   a and b or not c
来源：http://bbr.sysykeji.top

PHP:  $a && $b || !$c
来源：http://lxi.hfpthk.cn

JS:   a && b || !c
来源：http://ydc.gaohongyu789.top

TS:   a && b || !c
来源：http://bhe.fehbvm.com

Java: a && b || !c
来源：http://fov.yuxming.cn

Go:   a && b || !c
来源：http://uwy.xinyue.icu

Ruby: a && b || !c
来源：http://fns.jinyuanbaomall.cn

C#:   a && b || !c
来源：http://kcx.tanke756.top

[B16] 卫语句：不满足条件提前返回
来源：http://syj.0kj1m.cn

Py:   if not data: return
来源：http://clz.ivvv.top

PHP:  if (!$data) { return; }
来源：http://nlw.tian-w.cn

JS:   if (!data) return;
来源：http://swf.hywenlv.cn

TS:   if (!data) return;
来源：http://xhb.daxiang520.top

Java: if (data == null) return;
来源：http://uok.fktsv.cn

Go:   if data == nil { return }
来源：http://eof.havefunace.top

Ruby: return if data.nil?
来源：http://jbe.sysykeji.top

C#:   if (data == null) return;
来源：http://udw.jinghuilouyu.cn

================================================================================
来源：http://arn.nanxuanxn.top

C. 函数与作用域
来源：http://swu.yfazqb.com

================================================================================
来源：http://ahu.fanxiaobao.xyz

[C01] 定义函数
来源：http://tlm.yangfankeji.com

Py:   def add(a, b): return a + b
来源：http://aau.zhongyouzk.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xwk.shanyushiyangkeji.top

JS:   function add(a, b) { return a + b; }
来源：http://obm.gzhubu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mrb.zhongyouzk.top

Java: static int add(int a, int b) { return a + b; }
来源：http://nph.cdnleiting.top

Go:   func add(a, b int) int { return a + b }
来源：http://pwi.dianchejie.cn

Ruby: def add(a, b); a + b; end
来源：http://lbk.havefunace.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uxr.pycfn.com

[C02] 默认参数
来源：http://djh.yfazqb.com

Py:   def greet(name="World"): return name
来源：http://npl.jyoumei.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://nnn.aibaodan.cn

JS:   function greet(name = "World") { return name; }
来源：http://nuz.yonumen.top

TS:   function greet(name: string = "World") { return name; }
来源：http://alh.jyoumei.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dnl.fanxiaobao.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cbj.feifeiyinyue.top

Ruby: def greet(name = "World") = name
来源：http://wvv.zycfv.cn

C#:   string Greet(string name = "World") => name;
来源：http://xuh.nanxuanxn.top

[C03] 可变参数
来源：http://liq.zdbjq.cn

Py:   def total(*args): return sum(args)
来源：http://ttd.jqgufenzy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wvk.vqdsnc.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mng.hongshengwenyu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kdn.gzhubu.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vor.pengpengdd.cyou

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bsx.ivvv.top

Ruby: def total(*nums); nums.sum; end
来源：http://oxj.guowangkeji.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ekh.fehbvm.com

[C04] 命名参数 / 关键字参数
来源：http://gta.daxiang520.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mih.sjlbkw.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ykl.c1oappe.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lhk.hnqzz.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kmx.jlsjyb.cn

Java: // 无：用 Builder 模式或 record
来源：http://ztp.hywenlv.cn

Go:   // 无：用配置结构体参数
来源：http://mlb.nwbrower.top

Ruby: f(a: 1, b: 2)
来源：http://fyd.shangyingyoupin.top

C#:   f(a: 1, b: 2)
来源：http://tyh.wangdashe.top

[C05] 返回多个值
来源：http://wlh.chenzaomai.com

Py:   return a, b
来源：http://alv.zhoulong.xyz

PHP:  return [$a, $b];
来源：http://gbw.52xcode.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ypd.cucudq.cn

TS:   return { a, b };
来源：http://atf.tarul.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://aio.zhoulong.xyz

Go:   return a, b
来源：http://vlt.yj202588.top

Ruby: return a, b
来源：http://sev.tianlin.xyz

C#:   return (a, b);              // ValueTuple
来源：http://nxk.tian-w.cn

[C06] 匿名函数 / lambda
来源：http://vmy.zhaomingkeji.xyz

Py:   square = lambda x: x * x
来源：http://hng.snrcjt.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://dnr.tanke756.top

JS:   const square = x => x * x;
来源：http://nmq.jiagoushi.top

TS:   const square = (x: number): number => x * x;
来源：http://jfk.epnwcf.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://khk.birdmap.top

Go:   sq := func(x int) int { return x * x }
来源：http://nse.c1oappe.top

Ruby: square = ->(x) { x * x }
来源：http://jsi.xylfe.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pzl.vqdsnc.cn

[C07] 把函数作为参数传入
来源：http://cyu.jqgufenzy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ria.zhixingplan.top

PHP:  array_map("strtoupper", $arr);
来源：http://olo.kuanghao11.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://twt.gotoacloud.top

TS:   arr.map(String)
来源：http://yub.sweek.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://oqj.jqgfzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uqs.daxiang520.top

Ruby: arr.map(&:upcase)
来源：http://xnf.cashguo.top

C#:   arr.Select(s => s.ToUpper())
来源：http://grc.ydzc1.top

[C08] 闭包
来源：http://euj.shanyushiyangkeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wqk.yueranfly.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wtn.hfpthk.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baf.sxryk.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bur.dashuyun.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hut.uphjek.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qjq.fktsv.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vvz.mhx1999.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xly.gaohongyu789.top

[C09] 递归
来源：http://atl.yvedp.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://udf.zdqjudy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bax.jiagoushi.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gtk.jianghu66.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://evs.shzxlz.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://oow.ctjpmb.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://oxn.kuanghao11.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pmr.chenzaomai.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gus.guowangkeji.top

[C10] 变量作用域
来源：http://ksk.xingfuxueyuan.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vsf.shzxlz.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gfr.jinghuilouyu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ccq.yfazqb.com

TS:   同 JS
来源：http://chg.yueranfly.top

Java: 方法内为块级作用域
来源：http://xbn.kuanghao11.cn

Go:   花括号块级作用域
来源：http://lnr.zhoulong.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xrq.ywan-chungtsiang.top

C#:   块级作用域
来源：http://vru.andypj.xyz

[C11] 模块导入与导出
来源：http://qts.xinyue.icu

Py:   from module import func
来源：http://toe.sufxvd.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://gzv.cashguo.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ptr.jinghuilouyu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uxi.xziqi.cn

Java: import java.util.List;
来源：http://cvv.ydzc1.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blo.aibaodan.cn

Ruby: require "json"; require_relative "./util"
来源：http://vnm.ybcxt.top

C#:   using System.Text;
来源：http://pna.ydjk.org.cn

[C12] 立即执行函数 IIFE
来源：http://ndg.jianghu66.top

Py:   (lambda: print("run"))()
来源：http://oip.yfazqb.com

PHP:  (function () { echo "run"; })();
来源：http://hgc.zhoulong.xyz

JS:   (() => { console.log("run"); })();
来源：http://mqs.zhongyouzk.top

TS:   (() => { console.log("run"); })();
来源：http://ouo.shanyushiyangtech.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://psm.hammf.cn

Go:   func() { fmt.Println("run") }()
来源：http://wer.kuanghao11.cn

Ruby: -> { puts "run" }.call
来源：http://xde.iojbl.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://djn.jyoumei.cn

[C13] 类型声明 / 类型注解
来源：http://zyg.sjlbkw.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zwv.wangshuangyany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iov.ivvv.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lup.jqgfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tjn.yuanzhike.top

Java: int add(int a, int b) { return a + b; }
来源：http://xlm.shzxlz.cn

Go:   func add(a, b int) int
来源：http://qwc.pengpengdd.cyou

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nrv.hnxiangtu.top

C#:   int Add(int a, int b) => a + b;
来源：http://ofj.dashuyun.cn

[C14] 泛型函数
来源：http://fvb.9152youxi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hfl.0kj1m.cn

PHP:  // 无泛型
来源：http://tvb.gaohongyu789.top

JS:   // 无泛型
来源：http://iso.andypj.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jej.jianghu66.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dsl.redwolf501.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://doz.yfazqb.com

Ruby: # 无泛型
来源：http://hxg.dianchejie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xlj.jinghuilouyu.cn

[C15] 解构 / 展开参数
来源：http://phc.yj202588.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ias.hnxiangtu.top

PHP:  [$a, $b] = $pair;
来源：http://any.ppjwa.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ccn.shanyushiyangkeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gau.cqqwz.cn

Java: // 无解构
来源：http://can.andypj.xyz

Go:   // 无解构
来源：http://xmz.kuanghao11.cn

Ruby: a, b = pair
来源：http://xwr.xuanzx.com

C#:   var (a, b) = pair;
来源：http://zbh.jlsjyb.cn

[C16] 函数 / 方法重载
来源：http://jlg.jinghuilouyu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dvr.birdmap.top

PHP:  // 无重载
来源：http://lex.ivvv.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://vsl.c1oappe.top

TS:   // 用联合类型或重载签名声明
来源：http://qbn.cqqwz.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ase.tianlin.xyz

Go:   // 无重载：用不同函数名
来源：http://qsk.yj20258888.top

Ruby: # 无重载：靠动态参数
来源：http://txi.tarul.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://cnc.hysaishi.cn

================================================================================
来源：http://ycx.cucudq.cn

D. 数组 / 列表 / 集合
来源：http://fci.yj20258888.top

================================================================================
来源：http://kpv.bbcook.cn

[D01] 创建数组 / 列表
来源：http://lkx.svipenyu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ipo.c1oappe.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://icy.pengpengdd.cyou

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jqu.redwolf501.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://cgi.hysaishi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ijx.hammf.cn

Go:   arr := []int{1, 2, 3}
来源：http://gyf.xingfuxueyuan.xyz

Ruby: arr = [1, 2, 3]
来源：http://jsx.aibaodan.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hjh.yueranfly.top

[D02] 追加元素到末尾
来源：http://omd.zhaomingkeji.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hei.birdmap.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://prb.hfpthk.cn

JS:   arr.push(4);
来源：http://gkp.zhixingplan.top

TS:   arr.push(4);
来源：http://sps.fktsv.cn

Java: list.add(4);
来源：http://ooj.yonumen.top

Go:   arr = append(arr, 4)
来源：http://ezp.chenlongwang.top

Ruby: arr << 4; arr.push(5)
来源：http://niu.vqdsnc.cn

C#:   list.Add(4);
来源：http://dvl.tarul.cn

[D03] 在指定位置插入元素
来源：http://iel.yj202588.top

Py:   arr.insert(0, 0)
来源：http://dyz.zhiwuduotai.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pgn.fengsongda.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xie.epnwcf.com

TS:   arr.splice(0, 0, 0);
来源：http://fzb.jlsjyb.cn

Java: list.add(0, 0);
来源：http://yru.yj20258888.top

Go:   arr = append([]int{0}, arr...)
来源：http://uww.ehwqpu.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uzj.sufxvd.cn

C#:   list.Insert(0, 0);
来源：http://lud.zdqjudy.top

[D04] 删除元素
来源：http://nxd.yfazqb.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uoa.fktsv.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yjk.yueranfly.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://djr.snrcjt.cn

TS:   arr.splice(0, 1);
来源：http://srg.sjlbkw.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pqg.jqgufenzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ouq.xuanzx.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fnc.ehwqpu.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cez.jianghu66.top

[D05] 访问与修改元素
来源：http://pcp.tianlin.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zbz.yvedp.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cnj.fengsongda.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://smx.zhiwuduotai.top

TS:   arr[0]; arr.at(-1);
来源：http://xmo.guowangkeji.top

Java: list.get(0); list.set(0, 9);
来源：http://unc.haohaochexian.top

Go:   arr[0]; arr[0] = 9
来源：http://pui.havefunace.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pdz.yj20258888.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vun.ybcxt.top

[D06] 数组长度
来源：http://jmo.smart0.xyz

Py:   len(arr)
来源：http://all.bjfxy.top

PHP:  count($arr);
来源：http://zys.316326.xyz

JS:   arr.length
来源：http://qqz.uphjek.com

TS:   arr.length
来源：http://kdk.meibo888.top

Java: list.size();
来源：http://lyy.nanxinkj.top

Go:   len(arr)
来源：http://rqo.meibo888.top

Ruby: arr.length; arr.size
来源：http://lvb.52xcode.cn

C#:   list.Count;
来源：http://nkq.fanxiaobao.xyz

[D07] 切片 / 取子数组
来源：http://fzp.yuanzhike.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://czr.redwolf501.top

PHP:  array_slice($arr, 1, 3);
来源：http://cmq.c1oappe.top

JS:   arr.slice(1, 4);
来源：http://fjd.c1oappe.top

TS:   arr.slice(1, 4);
来源：http://moj.redwolf501.top

Java: list.subList(1, 4);
来源：http://sjf.shanyushiyangkeji.top

Go:   arr[1:4]
来源：http://kal.sweek.top

Ruby: arr[1, 3]
来源：http://xew.hysaishi.cn

C#:   list.GetRange(1, 3);
来源：http://qcr.gaohongyu789.top

[D08] 合并两个数组
来源：http://kwr.chenzaomai.com

Py:   a + b;  a.extend(b)
来源：http://idp.bbcook.cn

PHP:  array_merge($a, $b);
来源：http://jkl.birdmap.top

JS:   [...a, ...b];  a.concat(b);
来源：http://qyx.yangfankeji.com

TS:   [...a, ...b];
来源：http://wyw.cqqwz.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sed.kuanghao11.cn

Go:   append(a, b...)
来源：http://yxz.wangdashe.top

Ruby: a + b;  a.concat(b)
来源：http://hzx.yj20258888.top

C#:   a.Concat(b).ToList()
来源：http://xal.daria6918.cn

[D09] 排序（升序）
来源：http://sao.vqdsnc.cn

Py:   sorted(arr);  arr.sort()
来源：http://nzd.meibo888.top

PHP:  sort($arr);
来源：http://aui.0kj1m.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fac.yanxiufei.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lnw.sxryk.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rzx.hnqzz.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vtw.ivvv.top

Ruby: arr.sort
来源：http://ugw.yj202588.top

C#:   list.Sort();
来源：http://enm.cdnleiting.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://kwh.pycfn.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ivp.sxryk.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://veq.feifeiyinyue.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kqt.jinghuilouyu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ytx.shanyushiyangkeji.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sjt.zhaomingkeji.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://msj.daria6918.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dne.xylfe.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://phw.daxiang520.top

[D11] 反转数组
来源：http://onz.yueranfly.top

Py:   arr[::-1];  arr.reverse()
来源：http://cdr.dianchejie.cn

PHP:  array_reverse($arr);
来源：http://asm.chenzaomai.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yfo.iojbl.cn


<!-- 参考信息 -->