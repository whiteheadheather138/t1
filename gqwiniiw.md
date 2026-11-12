代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hzd.havefunace.top

Java: x instanceof Number
来源：http://yxy.hfpthk.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gwp.sweek.top

Ruby: x.is_a?(Numeric)
来源：http://unj.daria6918.cn

C#:   x is int or double or decimal
来源：http://lbu.zhiwuduotai.top

[B14] 判断值是否在集合内
来源：http://cly.sxryk.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cfl.shanyushiyangtech.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://axu.hesvh.cn

JS:   [1, 2, 3].includes(x)
来源：http://lig.snrcjt.cn

TS:   [1, 2, 3].includes(x)
来源：http://dle.pycfn.com

Java: List.of(1, 2, 3).contains(x)
来源：http://ucq.bjfxy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hlo.zhaomingkeji.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://mjn.daria6918.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dpt.ywan-chungtsiang.top

[B15] 布尔运算与取反
来源：http://uep.dashuyun.cn

Py:   a and b or not c
来源：http://wjw.yangfankeji.com

PHP:  $a && $b || !$c
来源：http://jjp.zhiwuduotai.top

JS:   a && b || !c
来源：http://yte.jyoumei.cn

TS:   a && b || !c
来源：http://hcg.zhiwuduotai.top

Java: a && b || !c
来源：http://igt.hammf.cn

Go:   a && b || !c
来源：http://chu.zhijiandao.cn

Ruby: a && b || !c
来源：http://ydy.ydzc1.top

C#:   a && b || !c
来源：http://wjl.ywan-chungtsiang.top

[B16] 卫语句：不满足条件提前返回
来源：http://koq.redwolf501.top

Py:   if not data: return
来源：http://vip.tanke756.top

PHP:  if (!$data) { return; }
来源：http://tjs.tianlin.xyz

JS:   if (!data) return;
来源：http://rhc.yongpay.top

TS:   if (!data) return;
来源：http://zwq.nanxinkj.top

Java: if (data == null) return;
来源：http://yoq.cdnleiting.top

Go:   if data == nil { return }
来源：http://uts.vqdsnc.cn

Ruby: return if data.nil?
来源：http://zvr.hongshengwenyu.top

C#:   if (data == null) return;
来源：http://agn.cdnleiting.top

================================================================================
来源：http://gll.guannengcc.top

C. 函数与作用域
来源：http://kku.c1oappe.top

================================================================================
来源：http://cvq.chenlongwang.top

[C01] 定义函数
来源：http://nax.hnqzz.top

Py:   def add(a, b): return a + b
来源：http://jto.hammf.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iyx.birdmap.top

JS:   function add(a, b) { return a + b; }
来源：http://vtu.aibaodan.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uio.quarkkingdee.top

Java: static int add(int a, int b) { return a + b; }
来源：http://upo.xingfuxueyuan.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://zuq.chenjidiqi.icu

Ruby: def add(a, b); a + b; end
来源：http://fbj.kuanghao11.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vkg.snrcjt.cn

[C02] 默认参数
来源：http://goj.yangfankeji.com

Py:   def greet(name="World"): return name
来源：http://nzp.vehdjk.com

PHP:  function greet($name = "World") { return $name; }
来源：http://slc.zhengqikj.top

JS:   function greet(name = "World") { return name; }
来源：http://vtq.0kj1m.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yeu.fzhhl.top

Java: // 无默认参数：方法重载或 Optional
来源：http://smp.svipenyu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ypt.xinyue.icu

Ruby: def greet(name = "World") = name
来源：http://ajk.dashuyun.cn

C#:   string Greet(string name = "World") => name;
来源：http://ayo.chenlongwang.top

[C03] 可变参数
来源：http://iiw.ywan-chungtsiang.top

Py:   def total(*args): return sum(args)
来源：http://nir.shzxlz.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jwa.dianchejie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jpu.shanyushiyangtech.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yyp.zdbjq.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dfn.xingfuxueyuan.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mtp.zdbjq.cn

Ruby: def total(*nums); nums.sum; end
来源：http://lkf.haohaochexian.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rxc.aizwys.cn

[C04] 命名参数 / 关键字参数
来源：http://yts.sysykeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ryo.shanyushiyangtech.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hvv.meibo888.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vrr.gotoacloud.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://iwj.yangfankeji.com

Java: // 无：用 Builder 模式或 record
来源：http://gti.gaohongyu789.top

Go:   // 无：用配置结构体参数
来源：http://wyi.dashuyun.cn

Ruby: f(a: 1, b: 2)
来源：http://vky.haohaochexian.top

C#:   f(a: 1, b: 2)
来源：http://xka.yj20258888.top

[C05] 返回多个值
来源：http://xwc.chenlongwang.top

Py:   return a, b
来源：http://axx.pycfn.com

PHP:  return [$a, $b];
来源：http://ybz.zdbjq.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://mfo.gzhubu.top

TS:   return { a, b };
来源：http://sok.jiagoushi.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fyv.aizwys.cn

Go:   return a, b
来源：http://pls.wangshuangyany.cn

Ruby: return a, b
来源：http://xtz.yuxming.cn

C#:   return (a, b);              // ValueTuple
来源：http://ahg.hongshengwenyu.top

[C06] 匿名函数 / lambda
来源：http://zae.smart0.xyz

Py:   square = lambda x: x * x
来源：http://mbc.sysykeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://skx.ppjwa.cn

JS:   const square = x => x * x;
来源：http://lcq.ctjpmb.com

TS:   const square = (x: number): number => x * x;
来源：http://zqo.snrcjt.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dao.9152youxi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ics.jinqigufen.top

Ruby: square = ->(x) { x * x }
来源：http://ykk.zhiwuduotai.top

C#:   Func<int, int> square = x => x * x;
来源：http://cnq.andypj.xyz

[C07] 把函数作为参数传入
来源：http://lie.zhengqikj.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qeq.aizwys.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ctw.chenlongwang.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://urz.chenlongwang.top

TS:   arr.map(String)
来源：http://qbe.andypj.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yfy.shzxlz.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hei.ydzc1.top

Ruby: arr.map(&:upcase)
来源：http://aff.nwbrower.top

C#:   arr.Select(s => s.ToUpper())
来源：http://doj.snrcjt.cn

[C08] 闭包
来源：http://whj.xylfe.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qrd.birdmap.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gcj.zhaomingkeji.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pqn.yj20258888.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lcl.hesvh.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tcf.gzhubu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://uya.zhijiandao.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ppu.zdqjudy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bfs.yuxming.cn

[C09] 递归
来源：http://nql.daxiang520.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://skz.svipenyu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nww.cucudq.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rzu.daria6918.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qln.yuanzhike.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ami.gzhubu.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vvq.vqdsnc.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ino.gogol.net.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://esz.gotoacloud.top

[C10] 变量作用域
来源：http://gcb.cashguo.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hkw.bjfxy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hbx.nanxinkj.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vnb.zhijiandao.cn

TS:   同 JS
来源：http://kvd.wangdashe.top

Java: 方法内为块级作用域
来源：http://ggq.cucudq.cn

Go:   花括号块级作用域
来源：http://jzo.chenlongwang.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qlq.ivvv.top

C#:   块级作用域
来源：http://vfi.zhaomingkeji.xyz

[C11] 模块导入与导出
来源：http://zbg.sufxvd.cn

Py:   from module import func
来源：http://zgf.ywan-chungtsiang.top

PHP:  require "file.php";  或 use App\Service;
来源：http://uyz.smart0.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://yzs.zhongyouzk.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sro.xziqi.cn

Java: import java.util.List;
来源：http://gyw.daxiang520.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tkr.hnxiangtu.top

Ruby: require "json"; require_relative "./util"
来源：http://xhv.fzhhl.top

C#:   using System.Text;
来源：http://gcn.tanke756.top

[C12] 立即执行函数 IIFE
来源：http://ykm.jinqigfzy.top

Py:   (lambda: print("run"))()
来源：http://zhq.aizwys.cn

PHP:  (function () { echo "run"; })();
来源：http://zat.chenlongwang.top

JS:   (() => { console.log("run"); })();
来源：http://ycw.quarkkingdee.top

TS:   (() => { console.log("run"); })();
来源：http://zdd.jinqigfzy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jxh.dianchejie.cn

Go:   func() { fmt.Println("run") }()
来源：http://sqk.zdqjudy.top

Ruby: -> { puts "run" }.call
来源：http://exk.feifeiyinyue.top

C#:   // 无 IIFE：用静态构造函数
来源：http://msd.uphjek.com

[C13] 类型声明 / 类型注解
来源：http://pna.snrcjt.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mpb.52xcode.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://upc.hfpthk.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ngj.jiagoushi.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yap.pycfn.com

Java: int add(int a, int b) { return a + b; }
来源：http://sxe.meibo888.top

Go:   func add(a, b int) int
来源：http://jil.zdqjudy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mpl.gaohongyu789.top

C#:   int Add(int a, int b) => a + b;
来源：http://kuj.sufxvd.cn

[C14] 泛型函数
来源：http://waw.jinqigfzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://clk.ivvv.top

PHP:  // 无泛型
来源：http://cqg.bbcook.cn

JS:   // 无泛型
来源：http://hbj.pycfn.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xvp.hfpthk.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kre.ivvv.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://izv.shangyingyoupin.top

Ruby: # 无泛型
来源：http://ydh.zdqjudy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://had.chenjidiqi.icu

[C15] 解构 / 展开参数
来源：http://acs.cheryme.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rek.feifeiyinyue.top

PHP:  [$a, $b] = $pair;
来源：http://gbf.yonumen.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://eoj.fanxiaobao.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://znt.bbcook.cn

Java: // 无解构
来源：http://gaj.daria6918.cn

Go:   // 无解构
来源：http://cwy.cashguo.top

Ruby: a, b = pair
来源：http://qyk.shzxlz.cn

C#:   var (a, b) = pair;
来源：http://ofg.gaohongyu789.top

[C16] 函数 / 方法重载
来源：http://xxj.daxiang520.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tzj.yueranfly.top

PHP:  // 无重载
来源：http://gom.9152youxi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://egy.snrcjt.cn

TS:   // 用联合类型或重载签名声明
来源：http://obt.uphjek.com

Java: void f(int a) {}  void f(String a) {}
来源：http://thq.uphjek.com

Go:   // 无重载：用不同函数名
来源：http://dkq.yj20258888.top

Ruby: # 无重载：靠动态参数
来源：http://weu.mhx1999.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://bby.zycfv.cn

================================================================================
来源：http://txm.uphjek.com

D. 数组 / 列表 / 集合
来源：http://vxa.sufxvd.cn

================================================================================
来源：http://oxl.sysykeji.top

[D01] 创建数组 / 列表
来源：http://amb.zdqjudy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://pwc.zhongyouzk.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wvh.xuanzx.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ils.xuetiantiany.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xyc.vehdjk.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://byh.feifeiyinyue.top

Go:   arr := []int{1, 2, 3}
来源：http://sph.pengpengdd.cyou

Ruby: arr = [1, 2, 3]
来源：http://hnv.andypj.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wsb.hesvh.cn

[D02] 追加元素到末尾
来源：http://rgx.xylfe.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rkj.quarkkingdee.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hwt.ctjpmb.com

JS:   arr.push(4);
来源：http://ssj.fktsv.cn

TS:   arr.push(4);
来源：http://lsa.sysykeji.top

Java: list.add(4);
来源：http://fdb.wangdashe.top

Go:   arr = append(arr, 4)
来源：http://qye.shangyingyoupin.top

Ruby: arr << 4; arr.push(5)
来源：http://ybp.bbcook.cn

C#:   list.Add(4);
来源：http://egp.zdbjq.cn

[D03] 在指定位置插入元素
来源：http://vkv.0kj1m.cn

Py:   arr.insert(0, 0)
来源：http://bjp.hongshengwenyu.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nto.yuxming.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gyt.fehbvm.com

TS:   arr.splice(0, 0, 0);
来源：http://sxg.xinyue.icu

Java: list.add(0, 0);
来源：http://ohi.sweek.top

Go:   arr = append([]int{0}, arr...)
来源：http://inz.gzhubu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uar.daria6918.cn

C#:   list.Insert(0, 0);
来源：http://glt.tarul.cn

[D04] 删除元素
来源：http://mwr.zhongyouzk.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ujs.shzxlz.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://klu.hesvh.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sop.cucudq.cn

TS:   arr.splice(0, 1);
来源：http://lgm.guowangkeji.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://uip.daria6918.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fdl.cqqwz.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ylg.52xcode.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://psz.cheryme.top

[D05] 访问与修改元素
来源：http://mta.daxiang520.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ugn.hysaishi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sjt.ydjk.org.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cxq.xinyue.icu

TS:   arr[0]; arr.at(-1);
来源：http://kbd.jianghu66.top

Java: list.get(0); list.set(0, 9);
来源：http://tec.ywan-chungtsiang.top

Go:   arr[0]; arr[0] = 9
来源：http://jwu.hcnkem.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vmb.andypj.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rnj.tarul.cn

[D06] 数组长度
来源：http://pyf.cheryme.top

Py:   len(arr)
来源：http://sdg.jyoumei.cn

PHP:  count($arr);
来源：http://hok.xziqi.cn

JS:   arr.length
来源：http://quk.zhijiandao.cn

TS:   arr.length
来源：http://ngm.vqdsnc.cn

Java: list.size();
来源：http://eqo.316326.xyz

Go:   len(arr)
来源：http://glz.fengsongda.top

Ruby: arr.length; arr.size
来源：http://isr.jqgufenzy.top

C#:   list.Count;
来源：http://dyh.tanke756.top

[D07] 切片 / 取子数组
来源：http://fna.gogol.net.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ina.ppjwa.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ipw.jianghu66.top

JS:   arr.slice(1, 4);
来源：http://irv.iojbl.cn

TS:   arr.slice(1, 4);
来源：http://jkn.bjfxy.top

Java: list.subList(1, 4);
来源：http://pwd.ybcxt.top

Go:   arr[1:4]
来源：http://ioq.shanyushiyangkeji.top

Ruby: arr[1, 3]
来源：http://rwr.svipenyu.cn

C#:   list.GetRange(1, 3);
来源：http://mkk.316326.xyz

[D08] 合并两个数组
来源：http://vru.yangfankeji.com

Py:   a + b;  a.extend(b)
来源：http://xml.hnxiangtu.top

PHP:  array_merge($a, $b);
来源：http://jwd.cheryme.top

JS:   [...a, ...b];  a.concat(b);
来源：http://dhy.yj20258.top

TS:   [...a, ...b];
来源：http://lgp.jyoumei.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rfo.chenlongwang.top

Go:   append(a, b...)
来源：http://rkd.0kj1m.cn

Ruby: a + b;  a.concat(b)
来源：http://twx.guowangkeji.top

C#:   a.Concat(b).ToList()
来源：http://avi.nanxinkj.top

[D09] 排序（升序）
来源：http://ekk.haohaochexian.top

Py:   sorted(arr);  arr.sort()
来源：http://nel.yj20258888.top

PHP:  sort($arr);
来源：http://tsx.gotoacloud.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ybi.hnqzz.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://kmj.cashguo.top

Java: Collections.sort(list);  list.sort(null);
来源：http://pds.daria6918.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fpk.ivvv.top

Ruby: arr.sort
来源：http://uek.yueranfly.top

C#:   list.Sort();
来源：http://efd.shzxlz.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ber.sxryk.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uzt.316326.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xmd.fanxiaobao.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://woh.xylfe.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hvm.yvedp.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ton.nanxinkj.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uzo.c1oappe.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://feh.zhoulong.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://suz.kuanghao11.cn

[D11] 反转数组
来源：http://gus.sweek.top

Py:   arr[::-1];  arr.reverse()
来源：http://tkt.aizwys.cn

PHP:  array_reverse($arr);
来源：http://dar.9152youxi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://eia.gogol.net.cn

TS:   [...arr].reverse();
来源：http://ipi.meibo888.top

Java: Collections.reverse(list);
来源：http://zss.cdnleiting.top

Go:   slices.Reverse(arr)
来源：http://mli.yfazqb.com

Ruby: arr.reverse
来源：http://aid.cdnleiting.top

C#:   list.Reverse();
来源：http://tib.yj202588.top

[D12] 查找元素下标
来源：http://lxl.shangyingyoupin.top

Py:   arr.index(x);  x in arr
来源：http://glk.yvedp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://obx.hongshengwenyu.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fus.ywan-chungtsiang.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zlk.nanxuanxn.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mpo.tarul.cn

Go:   slices.Index(arr, x)
来源：http://fbc.nanxuanxn.top

Ruby: arr.index(x)
来源：http://wra.zhijiandao.cn

C#:   list.IndexOf(x);
来源：http://psq.fehbvm.com

[D13] 过滤（保留满足条件的）
来源：http://zko.fzhhl.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lhn.sweek.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gxp.kuanghao11.cn

JS:   arr.filter(x => x > 3)
来源：http://rjk.gogol.net.cn

TS:   arr.filter(x => x > 3)
来源：http://eus.quarkkingdee.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qmo.birdmap.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://non.ydjk.org.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nfp.zdqjudy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ksd.jinghuilouyu.cn

[D14] 映射转换（每个元素变形）
来源：http://eyb.hesvh.cn


<!-- 参考信息 -->