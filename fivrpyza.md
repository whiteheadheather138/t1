代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://scc.yfazqb.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://snk.jlsjyb.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wqp.52xcode.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hqn.shuidangran.top

[B13] 判断是否为数字
来源：http://ktq.gogol.net.cn

Py:   isinstance(x, (int, float))
来源：http://elh.jlsjyb.cn

PHP:  is_numeric($x)
来源：http://sek.aibaodan.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nls.nwbrower.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fos.ydzc1.top

Java: x instanceof Number
来源：http://ohp.bbcook.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qio.sufxvd.cn

Ruby: x.is_a?(Numeric)
来源：http://ejb.ybcxt.top

C#:   x is int or double or decimal
来源：http://tec.hammf.cn

[B14] 判断值是否在集合内
来源：http://nyr.dashuyun.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rac.cashguo.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://eii.snrcjt.cn

JS:   [1, 2, 3].includes(x)
来源：http://oof.birdmap.top

TS:   [1, 2, 3].includes(x)
来源：http://qbd.yuanzhike.top

Java: List.of(1, 2, 3).contains(x)
来源：http://vfi.zhongyouzk.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ymw.gzhubu.top

Ruby: [1, 2, 3].include?(x)
来源：http://qwi.guowangkeji.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cvr.hcnkem.com

[B15] 布尔运算与取反
来源：http://fdu.ydjk.org.cn

Py:   a and b or not c
来源：http://cxs.wangdashe.top

PHP:  $a && $b || !$c
来源：http://zel.shangyingyoupin.top

JS:   a && b || !c
来源：http://fvn.hywenlv.cn

TS:   a && b || !c
来源：http://ien.shanyushiyangtech.top

Java: a && b || !c
来源：http://tvk.jinyuanbaomall.cn

Go:   a && b || !c
来源：http://igr.tianlin.xyz

Ruby: a && b || !c
来源：http://wwh.pycfn.com

C#:   a && b || !c
来源：http://tia.yangfankeji.com

[B16] 卫语句：不满足条件提前返回
来源：http://njk.gzhubu.top

Py:   if not data: return
来源：http://bwg.shanyushiyangkeji.top

PHP:  if (!$data) { return; }
来源：http://pim.aibaodan.cn

JS:   if (!data) return;
来源：http://hst.jinghuilouyu.cn

TS:   if (!data) return;
来源：http://wye.xylfe.cn

Java: if (data == null) return;
来源：http://hnh.fzhhl.top

Go:   if data == nil { return }
来源：http://yrz.jyoumei.cn

Ruby: return if data.nil?
来源：http://edc.hywenlv.cn

C#:   if (data == null) return;
来源：http://doe.cqqwz.cn

================================================================================
来源：http://luv.gogol.net.cn

C. 函数与作用域
来源：http://tlm.zycfv.cn

================================================================================
来源：http://buf.ydjk.org.cn

[C01] 定义函数
来源：http://ego.jlsjyb.cn

Py:   def add(a, b): return a + b
来源：http://ojx.jiagoushi.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nss.jianghu66.top

JS:   function add(a, b) { return a + b; }
来源：http://rsd.kuanghao11.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qhh.zhijiandao.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wwk.tianlin.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://lhi.tian-w.cn

Ruby: def add(a, b); a + b; end
来源：http://etg.zhaomingkeji.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uwo.jinyuanbaomall.cn

[C02] 默认参数
来源：http://eeu.tarul.cn

Py:   def greet(name="World"): return name
来源：http://zju.shangyingyoupin.top

PHP:  function greet($name = "World") { return $name; }
来源：http://jpl.jinghuilouyu.cn

JS:   function greet(name = "World") { return name; }
来源：http://xif.mhx1999.top

TS:   function greet(name: string = "World") { return name; }
来源：http://xuo.jinghuilouyu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://etj.andypj.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://izg.yuanzhike.top

Ruby: def greet(name = "World") = name
来源：http://api.sjlbkw.cn

C#:   string Greet(string name = "World") => name;
来源：http://poh.jinghuilouyu.cn

[C03] 可变参数
来源：http://sfb.aizwys.cn

Py:   def total(*args): return sum(args)
来源：http://fjg.vqdsnc.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kiq.cheryme.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://oji.cqqwz.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wgf.feifeiyinyue.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://eqp.yuanzhike.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bkw.hongshengwenyu.top

Ruby: def total(*nums); nums.sum; end
来源：http://ezw.sysykeji.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fdc.0kj1m.cn

[C04] 命名参数 / 关键字参数
来源：http://mrf.0kj1m.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gqi.fehbvm.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xqn.cashguo.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mrf.hfpthk.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://aan.daria6918.cn

Java: // 无：用 Builder 模式或 record
来源：http://dtp.fehbvm.com

Go:   // 无：用配置结构体参数
来源：http://wnc.birdmap.top

Ruby: f(a: 1, b: 2)
来源：http://tuv.dashuyun.cn

C#:   f(a: 1, b: 2)
来源：http://mbg.ybcxt.top

[C05] 返回多个值
来源：http://cnz.cucudq.cn

Py:   return a, b
来源：http://btr.zhongyouzk.top

PHP:  return [$a, $b];
来源：http://syz.tian-w.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://htz.yj20258.top

TS:   return { a, b };
来源：http://wsl.jyoumei.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gkh.aizwys.cn

Go:   return a, b
来源：http://opk.meibo888.top

Ruby: return a, b
来源：http://brx.guannengcc.top

C#:   return (a, b);              // ValueTuple
来源：http://jkx.gotoacloud.top

[C06] 匿名函数 / lambda
来源：http://epz.zhongyouzk.top

Py:   square = lambda x: x * x
来源：http://gnp.mhx1999.top

PHP:  $square = fn($x) => $x * $x;
来源：http://wti.jinyuanbaomall.cn

JS:   const square = x => x * x;
来源：http://dbk.mhx1999.top

TS:   const square = (x: number): number => x * x;
来源：http://vhh.fktsv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://oxp.0kj1m.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lfj.tian-w.cn

Ruby: square = ->(x) { x * x }
来源：http://cuh.shzxlz.cn

C#:   Func<int, int> square = x => x * x;
来源：http://gth.guannengcc.top

[C07] 把函数作为参数传入
来源：http://mhi.jyoumei.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nav.havefunace.top

PHP:  array_map("strtoupper", $arr);
来源：http://wdg.hesvh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://oij.meibo888.top

TS:   arr.map(String)
来源：http://zqd.hywenlv.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://int.chenzaomai.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vcy.zhoulong.xyz

Ruby: arr.map(&:upcase)
来源：http://ueu.andypj.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://ziw.gotoacloud.top

[C08] 闭包
来源：http://jwr.nanxinkj.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lta.yj202588.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bwa.yongpay.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uiz.zhengqikj.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lpf.hesvh.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lfm.hywenlv.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://epz.chenjidiqi.icu

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://klu.gaohongyu789.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ngn.yj20258888.top

[C09] 递归
来源：http://mja.wangdashe.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jzs.cdnleiting.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dht.sysykeji.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bze.zdqjudy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eyv.tian-w.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kbn.shanyushiyangtech.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dzm.yanxiufei.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vkv.sufxvd.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rnx.tarul.cn

[C10] 变量作用域
来源：http://utt.aibaodan.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bbh.daria6918.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cxe.shanyushiyangtech.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bqj.cucudq.cn

TS:   同 JS
来源：http://sxm.ydzc1.top

Java: 方法内为块级作用域
来源：http://xdl.jyoumei.cn

Go:   花括号块级作用域
来源：http://ywz.316326.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uzs.zdqjudy.top

C#:   块级作用域
来源：http://ziz.jinghuilouyu.cn

[C11] 模块导入与导出
来源：http://lni.ybcxt.top

Py:   from module import func
来源：http://pxp.zhijiandao.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://fww.hnqzz.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://nwo.zhengqikj.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ylr.tian-w.cn

Java: import java.util.List;
来源：http://luc.yuanzhike.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rjq.sysykeji.top

Ruby: require "json"; require_relative "./util"
来源：http://iic.fktsv.cn

C#:   using System.Text;
来源：http://qkn.guowangkeji.top

[C12] 立即执行函数 IIFE
来源：http://oko.shuidangran.top

Py:   (lambda: print("run"))()
来源：http://abl.redwolf501.top

PHP:  (function () { echo "run"; })();
来源：http://zvx.feifeiyinyue.top

JS:   (() => { console.log("run"); })();
来源：http://pqy.birdmap.top

TS:   (() => { console.log("run"); })();
来源：http://pcp.fengsongda.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gwp.c1oappe.top

Go:   func() { fmt.Println("run") }()
来源：http://kwz.uphjek.com

Ruby: -> { puts "run" }.call
来源：http://drs.yongpay.top

C#:   // 无 IIFE：用静态构造函数
来源：http://qfm.fzhhl.top

[C13] 类型声明 / 类型注解
来源：http://umg.xuetiantiany.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bjx.yj202588.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kdj.zhixingplan.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ztx.jinqigufen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mpg.epnwcf.com

Java: int add(int a, int b) { return a + b; }
来源：http://oup.jqgufenzy.top

Go:   func add(a, b int) int
来源：http://usb.jinqigfzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://agr.ehwqpu.com

C#:   int Add(int a, int b) => a + b;
来源：http://ywz.chenlongwang.top

[C14] 泛型函数
来源：http://ohv.ehwqpu.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bwm.xuetiantiany.cn

PHP:  // 无泛型
来源：http://zym.zhongyouzk.top

JS:   // 无泛型
来源：http://vyb.gotoacloud.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mee.yanxiufei.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cjw.c1oappe.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://aoc.zhiwuduotai.top

Ruby: # 无泛型
来源：http://qog.xziqi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vrk.0kj1m.cn

[C15] 解构 / 展开参数
来源：http://zqw.gotoacloud.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hqy.ywan-chungtsiang.top

PHP:  [$a, $b] = $pair;
来源：http://huk.snrcjt.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tpw.tianlin.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://voj.chenlongwang.top

Java: // 无解构
来源：http://xof.fktsv.cn

Go:   // 无解构
来源：http://bio.shuidangran.top

Ruby: a, b = pair
来源：http://eyy.aizwys.cn

C#:   var (a, b) = pair;
来源：http://gon.hnqzz.top

[C16] 函数 / 方法重载
来源：http://cdq.sxryk.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://aau.kuanghao11.cn

PHP:  // 无重载
来源：http://oif.fengsongda.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://pes.xinyue.icu

TS:   // 用联合类型或重载签名声明
来源：http://uzs.smart0.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://ijn.yfazqb.com

Go:   // 无重载：用不同函数名
来源：http://lzw.hammf.cn

Ruby: # 无重载：靠动态参数
来源：http://vxg.pengpengdd.cyou

C#:   void F(int a) {}  void F(string a) {}
来源：http://upp.aizwys.cn

================================================================================
来源：http://may.shzxlz.cn

D. 数组 / 列表 / 集合
来源：http://ype.yangfankeji.com

================================================================================
来源：http://xbe.ydjk.org.cn

[D01] 创建数组 / 列表
来源：http://xoc.sweek.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://cop.kuanghao11.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dea.birdmap.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://end.jianghu66.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://vei.bbcook.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://aap.zycfv.cn

Go:   arr := []int{1, 2, 3}
来源：http://fwl.bbcook.cn

Ruby: arr = [1, 2, 3]
来源：http://mug.fengsongda.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://suk.yvedp.cn

[D02] 追加元素到末尾
来源：http://unx.bjfxy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zdh.daria6918.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yfj.yanxiufei.cn

JS:   arr.push(4);
来源：http://oyx.ctjpmb.com

TS:   arr.push(4);
来源：http://wbg.hcnkem.com

Java: list.add(4);
来源：http://cwp.yuxming.cn

Go:   arr = append(arr, 4)
来源：http://yme.aibaodan.cn

Ruby: arr << 4; arr.push(5)
来源：http://rao.hcnkem.com

C#:   list.Add(4);
来源：http://gqo.epnwcf.com

[D03] 在指定位置插入元素
来源：http://pet.jinyuanbaomall.cn

Py:   arr.insert(0, 0)
来源：http://wor.yuanzhike.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tcw.c1oappe.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tvi.andypj.xyz

TS:   arr.splice(0, 0, 0);
来源：http://fwz.0kj1m.cn

Java: list.add(0, 0);
来源：http://lwe.tanke756.top

Go:   arr = append([]int{0}, arr...)
来源：http://eni.dashuyun.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xzq.sjlbkw.cn

C#:   list.Insert(0, 0);
来源：http://hme.zhengqikj.top

[D04] 删除元素
来源：http://nqw.hnxiangtu.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://meg.cdnleiting.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qmz.xylfe.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nuo.cashguo.top

TS:   arr.splice(0, 1);
来源：http://dwz.9152youxi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://phm.ydzc1.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ejy.ybcxt.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://aob.yuxming.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xzg.hesvh.cn

[D05] 访问与修改元素
来源：http://esk.kuanghao11.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://aob.jinqigfzy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lom.hesvh.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pof.yvedp.cn

TS:   arr[0]; arr.at(-1);
来源：http://jkj.yueranfly.top

Java: list.get(0); list.set(0, 9);
来源：http://muy.fanxiaobao.xyz

Go:   arr[0]; arr[0] = 9
来源：http://jou.jinghuilouyu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bnw.xuetiantiany.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://izd.hywenlv.cn

[D06] 数组长度
来源：http://pex.aizwys.cn

Py:   len(arr)
来源：http://egc.sufxvd.cn

PHP:  count($arr);
来源：http://nsn.mhx1999.top

JS:   arr.length
来源：http://feo.jinghuilouyu.cn

TS:   arr.length
来源：http://cly.jinghuilouyu.cn

Java: list.size();
来源：http://igb.jlsjyb.cn

Go:   len(arr)
来源：http://bic.kuanghao11.cn

Ruby: arr.length; arr.size
来源：http://cal.gogol.net.cn

C#:   list.Count;
来源：http://bsn.pycfn.com

[D07] 切片 / 取子数组
来源：http://ibw.hnqzz.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://woz.aibaodan.cn

PHP:  array_slice($arr, 1, 3);
来源：http://szi.ywan-chungtsiang.top

JS:   arr.slice(1, 4);
来源：http://ttk.havefunace.top

TS:   arr.slice(1, 4);
来源：http://fle.ctjpmb.com

Java: list.subList(1, 4);
来源：http://xwp.guowangkeji.top

Go:   arr[1:4]
来源：http://jki.zhixingplan.top

Ruby: arr[1, 3]
来源：http://eyn.bbcook.cn

C#:   list.GetRange(1, 3);
来源：http://ufo.yj20258.top

[D08] 合并两个数组
来源：http://mmf.iojbl.cn

Py:   a + b;  a.extend(b)
来源：http://bqo.bjfxy.top

PHP:  array_merge($a, $b);
来源：http://xiw.jinyuanbaomall.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kly.ehwqpu.com

TS:   [...a, ...b];
来源：http://qnn.bbcook.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gpx.hnqzz.top

Go:   append(a, b...)
来源：http://mfz.guowangkeji.top

Ruby: a + b;  a.concat(b)
来源：http://xla.iojbl.cn

C#:   a.Concat(b).ToList()
来源：http://pmx.jqgfzy.top

[D09] 排序（升序）
来源：http://vzs.xinyue.icu

Py:   sorted(arr);  arr.sort()
来源：http://whh.bbcook.cn

PHP:  sort($arr);
来源：http://ywy.yfazqb.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://stt.hysaishi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fzg.dashuyun.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vso.cashguo.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jyn.shanyushiyangtech.top

Ruby: arr.sort
来源：http://upx.daxiang520.top

C#:   list.Sort();
来源：http://ysz.chenjidiqi.icu

[D10] 自定义排序（按字段 / 多条件）
来源：http://mvs.gzhubu.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cxv.ywan-chungtsiang.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ijb.shuidangran.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://krq.gogol.net.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zqf.ydjk.org.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pdl.vehdjk.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sdv.zycfv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://key.hnxiangtu.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bms.birdmap.top

[D11] 反转数组
来源：http://zrl.hammf.cn

Py:   arr[::-1];  arr.reverse()
来源：http://bak.hesvh.cn

PHP:  array_reverse($arr);
来源：http://yoa.cucudq.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://krt.wangshuangyany.cn

TS:   [...arr].reverse();
来源：http://xvs.sxryk.cn

Java: Collections.reverse(list);
来源：http://jut.hcnkem.com

Go:   slices.Reverse(arr)
来源：http://jcm.yj20258888.top

Ruby: arr.reverse
来源：http://wzs.fanxiaobao.xyz

C#:   list.Reverse();
来源：http://ryw.ppjwa.cn

[D12] 查找元素下标
来源：http://ufe.ydjk.org.cn

Py:   arr.index(x);  x in arr
来源：http://pxp.dashuyun.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mql.vqdsnc.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://anw.shzxlz.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zwe.hongshengwenyu.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xrj.yj20258888.top

Go:   slices.Index(arr, x)
来源：http://eiz.mhx1999.top

Ruby: arr.index(x)
来源：http://igq.fktsv.cn

C#:   list.IndexOf(x);
来源：http://qcy.svipenyu.cn

[D13] 过滤（保留满足条件的）
来源：http://bxe.zhaomingkeji.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zpp.hcnkem.com


<!-- 参考信息 -->