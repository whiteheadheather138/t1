代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gez.shanyushiyangkeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gni.fehbvm.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gih.zdqjudy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gqj.cqqwz.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fak.hywenlv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gum.nanxuanxn.top

[B11] 生成数字序列 / 区间
来源：http://xru.vehdjk.com

Py:   list(range(0, 10, 2))
来源：http://scx.sufxvd.cn

PHP:  range(0, 10, 2);
来源：http://iky.hnqzz.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bph.316326.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://daq.cucudq.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tiq.jyoumei.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yki.xuetiantiany.cn

Ruby: (0...10).step(2).to_a
来源：http://qig.gogol.net.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://eph.zycfv.cn

[B12] 跳出多层循环
来源：http://pun.c1oappe.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://sgm.yuanzhike.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://jqf.zdqjudy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bsj.uphjek.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ico.meibo888.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vsc.ybcxt.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rus.fktsv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fcv.cdnleiting.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://oct.dianchejie.cn

[B13] 判断是否为数字
来源：http://pjk.hnxiangtu.top

Py:   isinstance(x, (int, float))
来源：http://ohn.bbcook.cn

PHP:  is_numeric($x)
来源：http://xiq.ctjpmb.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zsd.zhiwuduotai.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xaz.fzhhl.top

Java: x instanceof Number
来源：http://hbi.hammf.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rkq.ywan-chungtsiang.top

Ruby: x.is_a?(Numeric)
来源：http://pza.hywenlv.cn

C#:   x is int or double or decimal
来源：http://zir.mhx1999.top

[B14] 判断值是否在集合内
来源：http://bdp.zhoulong.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://peb.fanxiaobao.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kmi.zhongyouzk.top

JS:   [1, 2, 3].includes(x)
来源：http://soo.hesvh.cn

TS:   [1, 2, 3].includes(x)
来源：http://lec.bbcook.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://omv.hfpthk.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cxv.tian-w.cn

Ruby: [1, 2, 3].include?(x)
来源：http://tnd.cucudq.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bvq.zhoulong.xyz

[B15] 布尔运算与取反
来源：http://vec.quarkkingdee.top

Py:   a and b or not c
来源：http://fuu.ywan-chungtsiang.top

PHP:  $a && $b || !$c
来源：http://sio.vqdsnc.cn

JS:   a && b || !c
来源：http://lyv.52xcode.cn

TS:   a && b || !c
来源：http://ujd.hongshengwenyu.top

Java: a && b || !c
来源：http://ize.yfazqb.com

Go:   a && b || !c
来源：http://wxt.zdbjq.cn

Ruby: a && b || !c
来源：http://zue.dashuyun.cn

C#:   a && b || !c
来源：http://bam.0kj1m.cn

[B16] 卫语句：不满足条件提前返回
来源：http://dqg.dashuyun.cn

Py:   if not data: return
来源：http://jwd.zhiwuduotai.top

PHP:  if (!$data) { return; }
来源：http://zor.zdqjudy.top

JS:   if (!data) return;
来源：http://wue.jinghuilouyu.cn

TS:   if (!data) return;
来源：http://zhc.zdbjq.cn

Java: if (data == null) return;
来源：http://cwj.zhengqikj.top

Go:   if data == nil { return }
来源：http://aud.chenlongwang.top

Ruby: return if data.nil?
来源：http://gxw.cqqwz.cn

C#:   if (data == null) return;
来源：http://mil.gotoacloud.top

================================================================================
来源：http://hut.jinyuanbaomall.cn

C. 函数与作用域
来源：http://hdc.guowangkeji.top

================================================================================
来源：http://jfz.andypj.xyz

[C01] 定义函数
来源：http://wdv.yfazqb.com

Py:   def add(a, b): return a + b
来源：http://lpi.9152youxi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gbs.yangfankeji.com

JS:   function add(a, b) { return a + b; }
来源：http://yzh.shuidangran.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fna.havefunace.top

Java: static int add(int a, int b) { return a + b; }
来源：http://hlz.52xcode.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gir.jinyuanbaomall.cn

Ruby: def add(a, b); a + b; end
来源：http://bqe.sjlbkw.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hgd.pengpengdd.cyou

[C02] 默认参数
来源：http://jce.yj20258.top

Py:   def greet(name="World"): return name
来源：http://yzd.yanxiufei.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dsk.chenzaomai.com

JS:   function greet(name = "World") { return name; }
来源：http://ory.chenjidiqi.icu

TS:   function greet(name: string = "World") { return name; }
来源：http://jqu.hywenlv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://mdk.bjfxy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kxi.sjlbkw.cn

Ruby: def greet(name = "World") = name
来源：http://qnh.shanyushiyangkeji.top

C#:   string Greet(string name = "World") => name;
来源：http://hfi.jinghuilouyu.cn

[C03] 可变参数
来源：http://rgi.ivvv.top

Py:   def total(*args): return sum(args)
来源：http://ytd.xinyue.icu

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jzh.fanxiaobao.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qgg.gotoacloud.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vjq.52xcode.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://aou.chenlongwang.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://teh.zhixingplan.top

Ruby: def total(*nums); nums.sum; end
来源：http://jre.ybcxt.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lsb.epnwcf.com

[C04] 命名参数 / 关键字参数
来源：http://gru.xinyue.icu

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fvv.feifeiyinyue.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hlc.hnqzz.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://obm.sxryk.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uyb.sysykeji.top

Java: // 无：用 Builder 模式或 record
来源：http://kuz.iojbl.cn

Go:   // 无：用配置结构体参数
来源：http://fkl.jlsjyb.cn

Ruby: f(a: 1, b: 2)
来源：http://lcc.tarul.cn

C#:   f(a: 1, b: 2)
来源：http://vet.tanke756.top

[C05] 返回多个值
来源：http://diq.fktsv.cn

Py:   return a, b
来源：http://ckc.yfazqb.com

PHP:  return [$a, $b];
来源：http://eyp.haohaochexian.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://qcy.zhengqikj.top

TS:   return { a, b };
来源：http://hru.sysykeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bpn.yj202588.top

Go:   return a, b
来源：http://zij.chenjidiqi.icu

Ruby: return a, b
来源：http://shm.vqdsnc.cn

C#:   return (a, b);              // ValueTuple
来源：http://qob.nwbrower.top

[C06] 匿名函数 / lambda
来源：http://rta.xylfe.cn

Py:   square = lambda x: x * x
来源：http://lwa.hongshengwenyu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ner.sysykeji.top

JS:   const square = x => x * x;
来源：http://gci.meibo888.top

TS:   const square = (x: number): number => x * x;
来源：http://ehj.aibaodan.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mfw.fengsongda.top

Go:   sq := func(x int) int { return x * x }
来源：http://ynp.snrcjt.cn

Ruby: square = ->(x) { x * x }
来源：http://iao.jinghuilouyu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://clk.guowangkeji.top

[C07] 把函数作为参数传入
来源：http://dvr.aibaodan.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://duj.zhaomingkeji.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://len.daxiang520.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://beq.sweek.top

TS:   arr.map(String)
来源：http://slw.jinqigufen.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://flj.yanxiufei.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qpe.chenlongwang.top

Ruby: arr.map(&:upcase)
来源：http://ual.shuidangran.top

C#:   arr.Select(s => s.ToUpper())
来源：http://jpz.gaohongyu789.top

[C08] 闭包
来源：http://pbf.bjfxy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uad.zdbjq.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vrb.hnxiangtu.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ibe.316326.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sql.chenlongwang.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xmi.316326.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nfx.pengpengdd.cyou

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xic.bbcook.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rfr.hfpthk.cn

[C09] 递归
来源：http://qva.pycfn.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rls.yfazqb.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nor.quarkkingdee.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vmg.andypj.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://njx.jinqigufen.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kxz.yonumen.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tfq.zhoulong.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gzz.zycfv.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uqd.jlsjyb.cn

[C10] 变量作用域
来源：http://fpy.cucudq.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ffl.dianchejie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ifa.daxiang520.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://azf.feifeiyinyue.top

TS:   同 JS
来源：http://syl.hcnkem.com

Java: 方法内为块级作用域
来源：http://ilc.yanxiufei.cn

Go:   花括号块级作用域
来源：http://auv.ppjwa.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zrj.0kj1m.cn

C#:   块级作用域
来源：http://qrr.tianlin.xyz

[C11] 模块导入与导出
来源：http://elp.hongshengwenyu.top

Py:   from module import func
来源：http://hrq.yj20258888.top

PHP:  require "file.php";  或 use App\Service;
来源：http://uha.bbcook.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://bqy.zhaomingkeji.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://itp.snrcjt.cn

Java: import java.util.List;
来源：http://wne.yuanzhike.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ddp.zdqjudy.top

Ruby: require "json"; require_relative "./util"
来源：http://cjb.ydjk.org.cn

C#:   using System.Text;
来源：http://lsd.cqqwz.cn

[C12] 立即执行函数 IIFE
来源：http://wdy.kuanghao11.cn

Py:   (lambda: print("run"))()
来源：http://qon.ydzc1.top

PHP:  (function () { echo "run"; })();
来源：http://skz.redwolf501.top

JS:   (() => { console.log("run"); })();
来源：http://hlb.ivvv.top

TS:   (() => { console.log("run"); })();
来源：http://cfa.zhijiandao.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://avc.havefunace.top

Go:   func() { fmt.Println("run") }()
来源：http://kds.jqgfzy.top

Ruby: -> { puts "run" }.call
来源：http://qys.tanke756.top

C#:   // 无 IIFE：用静态构造函数
来源：http://tsa.sjlbkw.cn

[C13] 类型声明 / 类型注解
来源：http://dsd.yj202588.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vxr.tarul.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lbo.guowangkeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jqk.ybcxt.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mck.wangdashe.top

Java: int add(int a, int b) { return a + b; }
来源：http://eiu.shangyingyoupin.top

Go:   func add(a, b int) int
来源：http://owf.xylfe.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zjc.zhijiandao.cn

C#:   int Add(int a, int b) => a + b;
来源：http://kzy.nanxuanxn.top

[C14] 泛型函数
来源：http://egc.zhiwuduotai.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ugf.gzhubu.top

PHP:  // 无泛型
来源：http://cam.xuanzx.com

JS:   // 无泛型
来源：http://dtr.dashuyun.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jyd.nanxinkj.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://awe.cucudq.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kus.havefunace.top

Ruby: # 无泛型
来源：http://aul.epnwcf.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://djq.redwolf501.top

[C15] 解构 / 展开参数
来源：http://etn.fanxiaobao.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hfv.cqqwz.cn

PHP:  [$a, $b] = $pair;
来源：http://vzn.0kj1m.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nnu.sjlbkw.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ssh.yj20258888.top

Java: // 无解构
来源：http://ksr.daria6918.cn

Go:   // 无解构
来源：http://hmx.guannengcc.top

Ruby: a, b = pair
来源：http://xwj.nanxinkj.top

C#:   var (a, b) = pair;
来源：http://rmp.nanxuanxn.top

[C16] 函数 / 方法重载
来源：http://viq.yuxming.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nrh.zhijiandao.cn

PHP:  // 无重载
来源：http://duc.gaohongyu789.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://qyr.sysykeji.top

TS:   // 用联合类型或重载签名声明
来源：http://kqr.daxiang520.top

Java: void f(int a) {}  void f(String a) {}
来源：http://qro.kuanghao11.cn

Go:   // 无重载：用不同函数名
来源：http://wqz.jlsjyb.cn

Ruby: # 无重载：靠动态参数
来源：http://xbc.pengpengdd.cyou

C#:   void F(int a) {}  void F(string a) {}
来源：http://ogu.jinqigufen.top

================================================================================
来源：http://gpm.birdmap.top

D. 数组 / 列表 / 集合
来源：http://ywz.bbcook.cn

================================================================================
来源：http://ygk.andypj.xyz

[D01] 创建数组 / 列表
来源：http://kvr.52xcode.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://aqt.hysaishi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mbg.wangdashe.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bzr.yvedp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://nvv.hnxiangtu.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ocu.nanxinkj.top

Go:   arr := []int{1, 2, 3}
来源：http://ftk.0kj1m.cn

Ruby: arr = [1, 2, 3]
来源：http://pxu.ctjpmb.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://llc.zhixingplan.top

[D02] 追加元素到末尾
来源：http://cyr.gzhubu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cus.smart0.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xjz.hongshengwenyu.top

JS:   arr.push(4);
来源：http://uds.meibo888.top

TS:   arr.push(4);
来源：http://xzu.zhaomingkeji.xyz

Java: list.add(4);
来源：http://pxa.meibo888.top

Go:   arr = append(arr, 4)
来源：http://luc.snrcjt.cn

Ruby: arr << 4; arr.push(5)
来源：http://clm.meibo888.top

C#:   list.Add(4);
来源：http://xoc.xylfe.cn

[D03] 在指定位置插入元素
来源：http://hxz.jiagoushi.top

Py:   arr.insert(0, 0)
来源：http://snl.yongpay.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://luv.ydjk.org.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ypr.smart0.xyz

TS:   arr.splice(0, 0, 0);
来源：http://mna.9152youxi.cn

Java: list.add(0, 0);
来源：http://ogx.yonumen.top

Go:   arr = append([]int{0}, arr...)
来源：http://adm.zhixingplan.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vkb.vehdjk.com

C#:   list.Insert(0, 0);
来源：http://rus.sysykeji.top

[D04] 删除元素
来源：http://vbk.gogol.net.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pju.hongshengwenyu.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rjg.fzhhl.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wzd.yanxiufei.cn

TS:   arr.splice(0, 1);
来源：http://snm.hesvh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ymv.cashguo.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mwn.ppjwa.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://oow.jinqigufen.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kgq.yangfankeji.com

[D05] 访问与修改元素
来源：http://vev.sjlbkw.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vbp.birdmap.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ppf.zhixingplan.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cqh.9152youxi.cn

TS:   arr[0]; arr.at(-1);
来源：http://fge.chenlongwang.top

Java: list.get(0); list.set(0, 9);
来源：http://sse.birdmap.top

Go:   arr[0]; arr[0] = 9
来源：http://oik.yueranfly.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bxy.hongshengwenyu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jhr.smart0.xyz

[D06] 数组长度
来源：http://yps.shzxlz.cn

Py:   len(arr)
来源：http://qht.dianchejie.cn

PHP:  count($arr);
来源：http://ekb.fktsv.cn

JS:   arr.length
来源：http://wyw.hesvh.cn

TS:   arr.length
来源：http://ubv.yuanzhike.top

Java: list.size();
来源：http://wrk.ydjk.org.cn

Go:   len(arr)
来源：http://tsk.vehdjk.com

Ruby: arr.length; arr.size
来源：http://cie.shangyingyoupin.top

C#:   list.Count;
来源：http://urc.xylfe.cn

[D07] 切片 / 取子数组
来源：http://svc.cheryme.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cff.yongpay.top

PHP:  array_slice($arr, 1, 3);
来源：http://srs.nanxinkj.top

JS:   arr.slice(1, 4);
来源：http://dli.hesvh.cn

TS:   arr.slice(1, 4);
来源：http://swc.meibo888.top

Java: list.subList(1, 4);
来源：http://wrz.52xcode.cn

Go:   arr[1:4]
来源：http://wtm.52xcode.cn

Ruby: arr[1, 3]
来源：http://nxa.redwolf501.top

C#:   list.GetRange(1, 3);
来源：http://okx.xziqi.cn

[D08] 合并两个数组
来源：http://ftt.sxryk.cn

Py:   a + b;  a.extend(b)
来源：http://kvm.bjfxy.top

PHP:  array_merge($a, $b);
来源：http://org.yangfankeji.com

JS:   [...a, ...b];  a.concat(b);
来源：http://vtz.cdnleiting.top

TS:   [...a, ...b];
来源：http://izi.zhengqikj.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://awl.jqgufenzy.top

Go:   append(a, b...)
来源：http://kgm.chenjidiqi.icu

Ruby: a + b;  a.concat(b)
来源：http://xue.gzhubu.top

C#:   a.Concat(b).ToList()
来源：http://uzs.hnqzz.top

[D09] 排序（升序）
来源：http://seg.gzhubu.top

Py:   sorted(arr);  arr.sort()
来源：http://ahq.nanxinkj.top

PHP:  sort($arr);
来源：http://tnh.hnxiangtu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lbz.tian-w.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wyy.yvedp.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hvt.hysaishi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pyf.zdqjudy.top

Ruby: arr.sort
来源：http://jos.daxiang520.top

C#:   list.Sort();
来源：http://nww.guowangkeji.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://igv.wangdashe.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wkw.ppjwa.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://twu.nanxuanxn.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ujx.vehdjk.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lad.dashuyun.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vff.fanxiaobao.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nsc.jyoumei.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nsj.shangyingyoupin.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uzx.yfazqb.com


<!-- 参考信息 -->