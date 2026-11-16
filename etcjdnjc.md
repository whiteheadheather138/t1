代发 wailian999

[B13] 判断是否为数字
来源：http://taj.zhoulong.xyz

Py:   isinstance(x, (int, float))
来源：http://aim.daxiang520.top

PHP:  is_numeric($x)
来源：http://rnl.yvedp.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sry.pengpengdd.cyou

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mls.0kj1m.cn

Java: x instanceof Number
来源：http://hir.ydjk.org.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hzk.jinyuanbaomall.cn

Ruby: x.is_a?(Numeric)
来源：http://asl.wangshuangyany.cn

C#:   x is int or double or decimal
来源：http://cei.wangshuangyany.cn

[B14] 判断值是否在集合内
来源：http://dlb.haohaochexian.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://try.yanxiufei.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://coh.ydjk.org.cn

JS:   [1, 2, 3].includes(x)
来源：http://taj.epnwcf.com

TS:   [1, 2, 3].includes(x)
来源：http://wju.andypj.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://hrj.fengsongda.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nal.chenzaomai.com

Ruby: [1, 2, 3].include?(x)
来源：http://tll.nanxinkj.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vbw.tianlin.xyz

[B15] 布尔运算与取反
来源：http://chq.jinyuanbaomall.cn

Py:   a and b or not c
来源：http://psq.hcnkem.com

PHP:  $a && $b || !$c
来源：http://itf.zhongyouzk.top

JS:   a && b || !c
来源：http://pvl.snrcjt.cn

TS:   a && b || !c
来源：http://eie.ivvv.top

Java: a && b || !c
来源：http://ahz.hywenlv.cn

Go:   a && b || !c
来源：http://xax.pengpengdd.cyou

Ruby: a && b || !c
来源：http://agf.daria6918.cn

C#:   a && b || !c
来源：http://rzo.tianlin.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://ahi.yueranfly.top

Py:   if not data: return
来源：http://nge.yj202588.top

PHP:  if (!$data) { return; }
来源：http://kfe.yvedp.cn

JS:   if (!data) return;
来源：http://ljq.yongpay.top

TS:   if (!data) return;
来源：http://fbn.cashguo.top

Java: if (data == null) return;
来源：http://kna.ehwqpu.com

Go:   if data == nil { return }
来源：http://fsp.kuanghao11.cn

Ruby: return if data.nil?
来源：http://wsz.sweek.top

C#:   if (data == null) return;
来源：http://lgp.shuidangran.top

================================================================================
来源：http://gqw.fanxiaobao.xyz

C. 函数与作用域
来源：http://uwe.hongshengwenyu.top

================================================================================
来源：http://ovd.zhijiandao.cn

[C01] 定义函数
来源：http://fvc.haohaochexian.top

Py:   def add(a, b): return a + b
来源：http://evt.pengpengdd.cyou

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cgv.havefunace.top

JS:   function add(a, b) { return a + b; }
来源：http://inf.vqdsnc.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nqh.yj20258.top

Java: static int add(int a, int b) { return a + b; }
来源：http://gkg.aizwys.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hir.jlsjyb.cn

Ruby: def add(a, b); a + b; end
来源：http://iwn.xinyue.icu

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mop.gzhubu.top

[C02] 默认参数
来源：http://lrn.fengsongda.top

Py:   def greet(name="World"): return name
来源：http://blc.gaohongyu789.top

PHP:  function greet($name = "World") { return $name; }
来源：http://xwv.dianchejie.cn

JS:   function greet(name = "World") { return name; }
来源：http://fbe.yj20258.top

TS:   function greet(name: string = "World") { return name; }
来源：http://xdf.mhx1999.top

Java: // 无默认参数：方法重载或 Optional
来源：http://bgj.cashguo.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://aht.nanxuanxn.top

Ruby: def greet(name = "World") = name
来源：http://jzc.birdmap.top

C#:   string Greet(string name = "World") => name;
来源：http://rrm.zhijiandao.cn

[C03] 可变参数
来源：http://noi.yj20258.top

Py:   def total(*args): return sum(args)
来源：http://hrs.jlsjyb.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kqv.uphjek.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ioo.yanxiufei.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sds.sxryk.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vqo.fktsv.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ecz.zhongyouzk.top

Ruby: def total(*nums); nums.sum; end
来源：http://npt.hesvh.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gtd.jinqigfzy.top

[C04] 命名参数 / 关键字参数
来源：http://fdu.zdqjudy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rkj.snrcjt.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tes.snrcjt.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://oko.jinqigfzy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zjj.yvedp.cn

Java: // 无：用 Builder 模式或 record
来源：http://shm.daria6918.cn

Go:   // 无：用配置结构体参数
来源：http://bzy.ywan-chungtsiang.top

Ruby: f(a: 1, b: 2)
来源：http://qoc.uphjek.com

C#:   f(a: 1, b: 2)
来源：http://otb.316326.xyz

[C05] 返回多个值
来源：http://dqr.jiagoushi.top

Py:   return a, b
来源：http://nuo.yongpay.top

PHP:  return [$a, $b];
来源：http://tqi.ctjpmb.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://nte.gotoacloud.top

TS:   return { a, b };
来源：http://jus.wangdashe.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jhq.jianghu66.top

Go:   return a, b
来源：http://kwh.zhixingplan.top

Ruby: return a, b
来源：http://snh.ywan-chungtsiang.top

C#:   return (a, b);              // ValueTuple
来源：http://kqk.9152youxi.cn

[C06] 匿名函数 / lambda
来源：http://nqi.hesvh.cn

Py:   square = lambda x: x * x
来源：http://ihb.yvedp.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ckz.jinyuanbaomall.cn

JS:   const square = x => x * x;
来源：http://zae.kuanghao11.cn

TS:   const square = (x: number): number => x * x;
来源：http://syh.0kj1m.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hwl.zdbjq.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xef.shanyushiyangkeji.top

Ruby: square = ->(x) { x * x }
来源：http://vfo.snrcjt.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wmm.xylfe.cn

[C07] 把函数作为参数传入
来源：http://jcn.pengpengdd.cyou

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kgn.yj20258.top

PHP:  array_map("strtoupper", $arr);
来源：http://ifr.chenlongwang.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cns.jinqigufen.top

TS:   arr.map(String)
来源：http://dmj.chenzaomai.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xza.uphjek.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gyy.xinyue.icu

Ruby: arr.map(&:upcase)
来源：http://hll.ydzc1.top

C#:   arr.Select(s => s.ToUpper())
来源：http://wze.epnwcf.com

[C08] 闭包
来源：http://qkx.nanxinkj.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cfo.hfpthk.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://iht.jqgufenzy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wqh.hysaishi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hre.hongshengwenyu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jqt.hnqzz.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sdx.xziqi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rho.hcnkem.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dcs.yj202588.top

[C09] 递归
来源：http://nij.zhixingplan.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ndn.daxiang520.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fps.sweek.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wmn.jinqigufen.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tzj.hnqzz.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xol.tanke756.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hky.bbcook.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ppk.dashuyun.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://goj.yuxming.cn

[C10] 变量作用域
来源：http://ehx.xziqi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ltd.fengsongda.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gwg.jqgfzy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tqz.sjlbkw.cn

TS:   同 JS
来源：http://wbf.nwbrower.top

Java: 方法内为块级作用域
来源：http://jyg.ydzc1.top

Go:   花括号块级作用域
来源：http://zux.zdqjudy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gnh.mhx1999.top

C#:   块级作用域
来源：http://pgu.aizwys.cn

[C11] 模块导入与导出
来源：http://fhi.cheryme.top

Py:   from module import func
来源：http://jgs.pengpengdd.cyou

PHP:  require "file.php";  或 use App\Service;
来源：http://upw.wangshuangyany.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ndj.feifeiyinyue.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jdm.jinqigfzy.top

Java: import java.util.List;
来源：http://bue.cucudq.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qag.ydzc1.top

Ruby: require "json"; require_relative "./util"
来源：http://wfk.daxiang520.top

C#:   using System.Text;
来源：http://ukq.smart0.xyz

[C12] 立即执行函数 IIFE
来源：http://qpg.hywenlv.cn

Py:   (lambda: print("run"))()
来源：http://lba.zhengqikj.top

PHP:  (function () { echo "run"; })();
来源：http://bkz.chenjidiqi.icu

JS:   (() => { console.log("run"); })();
来源：http://tsm.redwolf501.top

TS:   (() => { console.log("run"); })();
来源：http://qso.yfazqb.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ate.gzhubu.top

Go:   func() { fmt.Println("run") }()
来源：http://kac.cqqwz.cn

Ruby: -> { puts "run" }.call
来源：http://jcr.cdnleiting.top

C#:   // 无 IIFE：用静态构造函数
来源：http://fsy.fzhhl.top

[C13] 类型声明 / 类型注解
来源：http://zkq.hesvh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zcg.cheryme.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://woq.vqdsnc.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://guz.yvedp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dfa.guowangkeji.top

Java: int add(int a, int b) { return a + b; }
来源：http://qwk.gotoacloud.top

Go:   func add(a, b int) int
来源：http://wxk.jinqigfzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zzs.fzhhl.top

C#:   int Add(int a, int b) => a + b;
来源：http://soe.hammf.cn

[C14] 泛型函数
来源：http://vhj.zhixingplan.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://udd.cqqwz.cn

PHP:  // 无泛型
来源：http://iwm.shzxlz.cn

JS:   // 无泛型
来源：http://vkp.vehdjk.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sgt.shanyushiyangkeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ubo.jlsjyb.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://sxg.xinyue.icu

Ruby: # 无泛型
来源：http://nkv.yueranfly.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jwf.tian-w.cn

[C15] 解构 / 展开参数
来源：http://mik.dianchejie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pku.yvedp.cn

PHP:  [$a, $b] = $pair;
来源：http://tzd.yanxiufei.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kic.daxiang520.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ogu.mhx1999.top

Java: // 无解构
来源：http://xku.cqqwz.cn

Go:   // 无解构
来源：http://ofi.316326.xyz

Ruby: a, b = pair
来源：http://bbn.fengsongda.top

C#:   var (a, b) = pair;
来源：http://hxg.jianghu66.top

[C16] 函数 / 方法重载
来源：http://afq.jianghu66.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bna.zdqjudy.top

PHP:  // 无重载
来源：http://wuo.yj202588.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://uug.bbcook.cn

TS:   // 用联合类型或重载签名声明
来源：http://nvj.0kj1m.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yqy.tianlin.xyz

Go:   // 无重载：用不同函数名
来源：http://qtx.ydjk.org.cn

Ruby: # 无重载：靠动态参数
来源：http://uig.iojbl.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://soi.yfazqb.com

================================================================================
来源：http://ucc.xylfe.cn

D. 数组 / 列表 / 集合
来源：http://zay.zhengqikj.top

================================================================================
来源：http://tpl.iojbl.cn

[D01] 创建数组 / 列表
来源：http://ewa.yvedp.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wcn.dianchejie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qfj.chenjidiqi.icu

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yzf.hesvh.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jts.fehbvm.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://stj.gaohongyu789.top

Go:   arr := []int{1, 2, 3}
来源：http://jwq.yj202588.top

Ruby: arr = [1, 2, 3]
来源：http://tuj.aizwys.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vwk.316326.xyz

[D02] 追加元素到末尾
来源：http://uuk.shangyingyoupin.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kua.fktsv.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fgo.hesvh.cn

JS:   arr.push(4);
来源：http://mrr.gogol.net.cn

TS:   arr.push(4);
来源：http://hnw.chenzaomai.com

Java: list.add(4);
来源：http://akb.ydzc1.top

Go:   arr = append(arr, 4)
来源：http://sgg.jinqigufen.top

Ruby: arr << 4; arr.push(5)
来源：http://pov.c1oappe.top

C#:   list.Add(4);
来源：http://hnj.yj20258.top

[D03] 在指定位置插入元素
来源：http://szs.fengsongda.top

Py:   arr.insert(0, 0)
来源：http://rvd.hongshengwenyu.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nmt.pycfn.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://efz.guannengcc.top

TS:   arr.splice(0, 0, 0);
来源：http://mti.9152youxi.cn

Java: list.add(0, 0);
来源：http://dsu.c1oappe.top

Go:   arr = append([]int{0}, arr...)
来源：http://feo.ivvv.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cpu.shzxlz.cn

C#:   list.Insert(0, 0);
来源：http://ndj.aibaodan.cn

[D04] 删除元素
来源：http://stn.yonumen.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cpt.cucudq.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yiv.ybcxt.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lfm.zhongyouzk.top

TS:   arr.splice(0, 1);
来源：http://rwt.jinghuilouyu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lsu.cqqwz.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pth.cashguo.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cej.aibaodan.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uqt.dianchejie.cn

[D05] 访问与修改元素
来源：http://rfo.aibaodan.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kyx.guannengcc.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dbq.guowangkeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://skb.havefunace.top

TS:   arr[0]; arr.at(-1);
来源：http://nlw.andypj.xyz

Java: list.get(0); list.set(0, 9);
来源：http://dhy.jinghuilouyu.cn

Go:   arr[0]; arr[0] = 9
来源：http://zbg.ydjk.org.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://psz.vehdjk.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uxj.jqgfzy.top

[D06] 数组长度
来源：http://uee.havefunace.top

Py:   len(arr)
来源：http://bfx.yj20258888.top

PHP:  count($arr);
来源：http://adc.zdqjudy.top

JS:   arr.length
来源：http://yus.fanxiaobao.xyz

TS:   arr.length
来源：http://coj.ywan-chungtsiang.top

Java: list.size();
来源：http://jir.cqqwz.cn

Go:   len(arr)
来源：http://ljy.zhoulong.xyz

Ruby: arr.length; arr.size
来源：http://qfh.wangdashe.top

C#:   list.Count;
来源：http://wom.tian-w.cn

[D07] 切片 / 取子数组
来源：http://mvr.haohaochexian.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://anp.vqdsnc.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vqq.yanxiufei.cn

JS:   arr.slice(1, 4);
来源：http://fqs.uphjek.com

TS:   arr.slice(1, 4);
来源：http://thk.yj20258.top

Java: list.subList(1, 4);
来源：http://gpg.jqgufenzy.top

Go:   arr[1:4]
来源：http://dub.jianghu66.top

Ruby: arr[1, 3]
来源：http://cmy.xuetiantiany.cn

C#:   list.GetRange(1, 3);
来源：http://hxa.cqqwz.cn

[D08] 合并两个数组
来源：http://ksb.wangdashe.top

Py:   a + b;  a.extend(b)
来源：http://dds.xuetiantiany.cn

PHP:  array_merge($a, $b);
来源：http://lji.zycfv.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pgm.nanxuanxn.top

TS:   [...a, ...b];
来源：http://kjq.jyoumei.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bge.fengsongda.top

Go:   append(a, b...)
来源：http://fbk.aibaodan.cn

Ruby: a + b;  a.concat(b)
来源：http://hgv.jiagoushi.top

C#:   a.Concat(b).ToList()
来源：http://mvo.zhiwuduotai.top

[D09] 排序（升序）
来源：http://cug.jinqigfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://enm.epnwcf.com

PHP:  sort($arr);
来源：http://aec.smart0.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lbz.tianlin.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://thx.hammf.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ypr.hnqzz.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hpp.fktsv.cn

Ruby: arr.sort
来源：http://vck.xingfuxueyuan.xyz

C#:   list.Sort();
来源：http://nvj.fktsv.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vrp.xingfuxueyuan.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vwp.dashuyun.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://woq.daxiang520.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ope.xinyue.icu

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://eel.shuidangran.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xuw.gotoacloud.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cbg.sweek.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rir.chenlongwang.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yqs.hywenlv.cn

[D11] 反转数组
来源：http://egv.cqqwz.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lki.ctjpmb.com

PHP:  array_reverse($arr);
来源：http://vha.smart0.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xlu.smart0.xyz

TS:   [...arr].reverse();
来源：http://vjv.zhiwuduotai.top

Java: Collections.reverse(list);
来源：http://pva.sysykeji.top

Go:   slices.Reverse(arr)
来源：http://hdv.gogol.net.cn

Ruby: arr.reverse
来源：http://mae.zhaomingkeji.xyz

C#:   list.Reverse();
来源：http://yve.hcnkem.com

[D12] 查找元素下标
来源：http://mwl.pengpengdd.cyou

Py:   arr.index(x);  x in arr
来源：http://aii.ppjwa.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://agc.sufxvd.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ffz.zhiwuduotai.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sqc.zdbjq.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hwh.pycfn.com

Go:   slices.Index(arr, x)
来源：http://lux.nanxinkj.top

Ruby: arr.index(x)
来源：http://rnf.yj20258.top

C#:   list.IndexOf(x);
来源：http://dup.shuidangran.top

[D13] 过滤（保留满足条件的）
来源：http://amc.jqgfzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xlz.fzhhl.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jrm.sufxvd.cn

JS:   arr.filter(x => x > 3)
来源：http://zgs.uphjek.com

TS:   arr.filter(x => x > 3)
来源：http://eaz.zdqjudy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pqd.yj20258888.top


<!-- 参考信息 -->