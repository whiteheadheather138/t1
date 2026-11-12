代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://rzu.shangyingyoupin.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kdi.tian-w.cn

[B15] 布尔运算与取反
来源：http://ycy.gzhubu.top

Py:   a and b or not c
来源：http://con.bbcook.cn

PHP:  $a && $b || !$c
来源：http://rjg.shangyingyoupin.top

JS:   a && b || !c
来源：http://wlv.guannengcc.top

TS:   a && b || !c
来源：http://tml.xinyue.icu

Java: a && b || !c
来源：http://zvv.tanke756.top

Go:   a && b || !c
来源：http://nnv.jqgufenzy.top

Ruby: a && b || !c
来源：http://klx.fzhhl.top

C#:   a && b || !c
来源：http://hre.jyoumei.cn

[B16] 卫语句：不满足条件提前返回
来源：http://kzh.sjlbkw.cn

Py:   if not data: return
来源：http://hkn.shzxlz.cn

PHP:  if (!$data) { return; }
来源：http://jur.hnxiangtu.top

JS:   if (!data) return;
来源：http://aco.ivvv.top

TS:   if (!data) return;
来源：http://srb.zhongyouzk.top

Java: if (data == null) return;
来源：http://kmc.vehdjk.com

Go:   if data == nil { return }
来源：http://gur.dianchejie.cn

Ruby: return if data.nil?
来源：http://zic.shuidangran.top

C#:   if (data == null) return;
来源：http://ckk.chenzaomai.com

================================================================================
来源：http://xyh.pycfn.com

C. 函数与作用域
来源：http://gpd.dianchejie.cn

================================================================================
来源：http://bja.aibaodan.cn

[C01] 定义函数
来源：http://bmw.tarul.cn

Py:   def add(a, b): return a + b
来源：http://rwq.ppjwa.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mez.yonumen.top

JS:   function add(a, b) { return a + b; }
来源：http://inm.yj20258888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://njs.uphjek.com

Java: static int add(int a, int b) { return a + b; }
来源：http://tvj.guowangkeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://zou.dianchejie.cn

Ruby: def add(a, b); a + b; end
来源：http://tix.dianchejie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lkc.jinqigfzy.top

[C02] 默认参数
来源：http://zrq.dianchejie.cn

Py:   def greet(name="World"): return name
来源：http://vvd.hcnkem.com

PHP:  function greet($name = "World") { return $name; }
来源：http://orf.gzhubu.top

JS:   function greet(name = "World") { return name; }
来源：http://rzq.xylfe.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ytz.zhoulong.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://tbk.ywan-chungtsiang.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pto.jlsjyb.cn

Ruby: def greet(name = "World") = name
来源：http://kvs.dashuyun.cn

C#:   string Greet(string name = "World") => name;
来源：http://vmu.hnxiangtu.top

[C03] 可变参数
来源：http://vwv.ivvv.top

Py:   def total(*args): return sum(args)
来源：http://kub.hammf.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hkc.gotoacloud.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pcw.hysaishi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vzy.52xcode.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://oan.gogol.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vgu.hnqzz.top

Ruby: def total(*nums); nums.sum; end
来源：http://let.andypj.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wna.hcnkem.com

[C04] 命名参数 / 关键字参数
来源：http://gja.9152youxi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nee.snrcjt.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wpb.xuanzx.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cek.tian-w.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dyy.chenlongwang.top

Java: // 无：用 Builder 模式或 record
来源：http://qyo.jyoumei.cn

Go:   // 无：用配置结构体参数
来源：http://jhk.zdqjudy.top

Ruby: f(a: 1, b: 2)
来源：http://var.ppjwa.cn

C#:   f(a: 1, b: 2)
来源：http://jcb.xingfuxueyuan.xyz

[C05] 返回多个值
来源：http://sof.gaohongyu789.top

Py:   return a, b
来源：http://rez.cashguo.top

PHP:  return [$a, $b];
来源：http://gea.daxiang520.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://huq.pengpengdd.cyou

TS:   return { a, b };
来源：http://zbr.gaohongyu789.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wot.sjlbkw.cn

Go:   return a, b
来源：http://bpa.wangshuangyany.cn

Ruby: return a, b
来源：http://fdb.0kj1m.cn

C#:   return (a, b);              // ValueTuple
来源：http://kxe.yuanzhike.top

[C06] 匿名函数 / lambda
来源：http://dfx.nwbrower.top

Py:   square = lambda x: x * x
来源：http://irg.ppjwa.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://rgo.gzhubu.top

JS:   const square = x => x * x;
来源：http://uwd.nanxuanxn.top

TS:   const square = (x: number): number => x * x;
来源：http://bxv.gzhubu.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://auh.sjlbkw.cn

Go:   sq := func(x int) int { return x * x }
来源：http://omf.tanke756.top

Ruby: square = ->(x) { x * x }
来源：http://uip.zdbjq.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bwc.chenzaomai.com

[C07] 把函数作为参数传入
来源：http://roc.xinyue.icu

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ogv.aizwys.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ixr.yj20258888.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nrg.fzhhl.top

TS:   arr.map(String)
来源：http://vzg.yuxming.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yek.hywenlv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yez.tianlin.xyz

Ruby: arr.map(&:upcase)
来源：http://vnc.wangshuangyany.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xzc.snrcjt.cn

[C08] 闭包
来源：http://dex.yuanzhike.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://big.xuanzx.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sxp.aizwys.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hgh.dashuyun.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gxd.cucudq.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tim.zhengqikj.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ixf.yueranfly.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nck.aibaodan.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wxn.chenjidiqi.icu

[C09] 递归
来源：http://rkw.guannengcc.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uog.hnqzz.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://atg.zhoulong.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ctc.xuetiantiany.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kxt.hysaishi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://khl.jinyuanbaomall.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tog.xziqi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yhi.xingfuxueyuan.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pru.dashuyun.cn

[C10] 变量作用域
来源：http://xzw.ppjwa.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dbh.cheryme.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yqn.ybcxt.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cgs.hcnkem.com

TS:   同 JS
来源：http://asr.smart0.xyz

Java: 方法内为块级作用域
来源：http://boy.nwbrower.top

Go:   花括号块级作用域
来源：http://cum.nwbrower.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ndq.ywan-chungtsiang.top

C#:   块级作用域
来源：http://vnm.fehbvm.com

[C11] 模块导入与导出
来源：http://azc.uphjek.com

Py:   from module import func
来源：http://tpp.epnwcf.com

PHP:  require "file.php";  或 use App\Service;
来源：http://yjo.0kj1m.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zhk.haohaochexian.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jsx.yj20258.top

Java: import java.util.List;
来源：http://dpe.tarul.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://guo.jinqigufen.top

Ruby: require "json"; require_relative "./util"
来源：http://izj.ydzc1.top

C#:   using System.Text;
来源：http://djv.gogol.net.cn

[C12] 立即执行函数 IIFE
来源：http://fut.hnqzz.top

Py:   (lambda: print("run"))()
来源：http://aed.ywan-chungtsiang.top

PHP:  (function () { echo "run"; })();
来源：http://iqg.hnxiangtu.top

JS:   (() => { console.log("run"); })();
来源：http://dkt.jinqigfzy.top

TS:   (() => { console.log("run"); })();
来源：http://xfw.sweek.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qwd.jinghuilouyu.cn

Go:   func() { fmt.Println("run") }()
来源：http://owh.zhengqikj.top

Ruby: -> { puts "run" }.call
来源：http://oes.hongshengwenyu.top

C#:   // 无 IIFE：用静态构造函数
来源：http://nah.cashguo.top

[C13] 类型声明 / 类型注解
来源：http://elw.zhijiandao.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zbf.nanxuanxn.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ufk.xylfe.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cfo.jinyuanbaomall.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xrx.zhoulong.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://vkt.chenlongwang.top

Go:   func add(a, b int) int
来源：http://cnv.nanxinkj.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bah.xinyue.icu

C#:   int Add(int a, int b) => a + b;
来源：http://kld.zhiwuduotai.top

[C14] 泛型函数
来源：http://jsl.xuetiantiany.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qoq.hnqzz.top

PHP:  // 无泛型
来源：http://odf.jqgfzy.top

JS:   // 无泛型
来源：http://xfq.jiagoushi.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://itm.zdqjudy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cxf.meibo888.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ojv.xinyue.icu

Ruby: # 无泛型
来源：http://klf.smart0.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fej.cashguo.top

[C15] 解构 / 展开参数
来源：http://ouw.gotoacloud.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://glb.zhengqikj.top

PHP:  [$a, $b] = $pair;
来源：http://urn.xziqi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fmn.daria6918.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ozr.jinyuanbaomall.cn

Java: // 无解构
来源：http://ajs.uphjek.com

Go:   // 无解构
来源：http://veu.aizwys.cn

Ruby: a, b = pair
来源：http://rqz.zhixingplan.top

C#:   var (a, b) = pair;
来源：http://ngd.cucudq.cn

[C16] 函数 / 方法重载
来源：http://sym.jyoumei.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cgq.nanxinkj.top

PHP:  // 无重载
来源：http://rgn.snrcjt.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qzx.pycfn.com

TS:   // 用联合类型或重载签名声明
来源：http://rno.wangdashe.top

Java: void f(int a) {}  void f(String a) {}
来源：http://wvt.jianghu66.top

Go:   // 无重载：用不同函数名
来源：http://dtj.zhijiandao.cn

Ruby: # 无重载：靠动态参数
来源：http://ads.tianlin.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://ctk.vqdsnc.cn

================================================================================
来源：http://twk.zdbjq.cn

D. 数组 / 列表 / 集合
来源：http://wzf.smart0.xyz

================================================================================
来源：http://ipw.gzhubu.top

[D01] 创建数组 / 列表
来源：http://ikk.jinqigufen.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://oac.shanyushiyangtech.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jxx.jinqigfzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cbe.52xcode.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://veq.haohaochexian.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kgs.zhiwuduotai.top

Go:   arr := []int{1, 2, 3}
来源：http://lrp.fzhhl.top

Ruby: arr = [1, 2, 3]
来源：http://njy.cheryme.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yny.bjfxy.top

[D02] 追加元素到末尾
来源：http://gvt.jinyuanbaomall.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wmp.wangshuangyany.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rqo.hammf.cn

JS:   arr.push(4);
来源：http://lby.nanxinkj.top

TS:   arr.push(4);
来源：http://yoj.guowangkeji.top

Java: list.add(4);
来源：http://oyw.ydjk.org.cn

Go:   arr = append(arr, 4)
来源：http://lrx.zhengqikj.top

Ruby: arr << 4; arr.push(5)
来源：http://fyz.pycfn.com

C#:   list.Add(4);
来源：http://vhv.shanyushiyangtech.top

[D03] 在指定位置插入元素
来源：http://cgs.fengsongda.top

Py:   arr.insert(0, 0)
来源：http://etp.tianlin.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jyv.zhongyouzk.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://znp.xingfuxueyuan.xyz

TS:   arr.splice(0, 0, 0);
来源：http://bnl.meibo888.top

Java: list.add(0, 0);
来源：http://jsb.snrcjt.cn

Go:   arr = append([]int{0}, arr...)
来源：http://twv.cqqwz.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cjh.yj20258888.top

C#:   list.Insert(0, 0);
来源：http://qkr.jinqigfzy.top

[D04] 删除元素
来源：http://zjl.uphjek.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://opw.kuanghao11.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ihr.gaohongyu789.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ldl.zdqjudy.top

TS:   arr.splice(0, 1);
来源：http://ajg.zhijiandao.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://abr.gzhubu.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dap.xingfuxueyuan.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zsg.ywan-chungtsiang.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://txe.vehdjk.com

[D05] 访问与修改元素
来源：http://yyv.xinyue.icu

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fxj.jyoumei.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gab.dianchejie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pkb.cqqwz.cn

TS:   arr[0]; arr.at(-1);
来源：http://cei.daria6918.cn

Java: list.get(0); list.set(0, 9);
来源：http://djk.aibaodan.cn

Go:   arr[0]; arr[0] = 9
来源：http://kqm.zycfv.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uzz.hnqzz.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bme.9152youxi.cn

[D06] 数组长度
来源：http://wav.xylfe.cn

Py:   len(arr)
来源：http://ans.daxiang520.top

PHP:  count($arr);
来源：http://npb.hfpthk.cn

JS:   arr.length
来源：http://rtn.cdnleiting.top

TS:   arr.length
来源：http://scl.yueranfly.top

Java: list.size();
来源：http://oiy.yj202588.top

Go:   len(arr)
来源：http://dpv.daxiang520.top

Ruby: arr.length; arr.size
来源：http://nch.zhoulong.xyz

C#:   list.Count;
来源：http://eqv.shanyushiyangtech.top

[D07] 切片 / 取子数组
来源：http://lqe.yj20258.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://eby.sweek.top

PHP:  array_slice($arr, 1, 3);
来源：http://tfa.hammf.cn

JS:   arr.slice(1, 4);
来源：http://uho.nwbrower.top

TS:   arr.slice(1, 4);
来源：http://lmz.xuanzx.com

Java: list.subList(1, 4);
来源：http://jen.jiagoushi.top

Go:   arr[1:4]
来源：http://tnz.epnwcf.com

Ruby: arr[1, 3]
来源：http://nnz.zhijiandao.cn

C#:   list.GetRange(1, 3);
来源：http://wxn.ywan-chungtsiang.top

[D08] 合并两个数组
来源：http://prp.zhiwuduotai.top

Py:   a + b;  a.extend(b)
来源：http://fhr.ydjk.org.cn

PHP:  array_merge($a, $b);
来源：http://nrx.guowangkeji.top

JS:   [...a, ...b];  a.concat(b);
来源：http://jit.pycfn.com

TS:   [...a, ...b];
来源：http://qpj.zdbjq.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qou.aibaodan.cn

Go:   append(a, b...)
来源：http://uln.xinyue.icu

Ruby: a + b;  a.concat(b)
来源：http://oxv.ehwqpu.com

C#:   a.Concat(b).ToList()
来源：http://tnf.zhengqikj.top

[D09] 排序（升序）
来源：http://vjh.shzxlz.cn

Py:   sorted(arr);  arr.sort()
来源：http://bty.0kj1m.cn

PHP:  sort($arr);
来源：http://wds.zhiwuduotai.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lmn.chenjidiqi.icu

TS:   [...arr].sort((x, y) => x - y);
来源：http://och.jinqigufen.top

Java: Collections.sort(list);  list.sort(null);
来源：http://boz.daxiang520.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xfk.hysaishi.cn

Ruby: arr.sort
来源：http://mat.ppjwa.cn

C#:   list.Sort();
来源：http://dbm.jyoumei.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://eyc.yj20258.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://smj.jqgufenzy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bhh.hnqzz.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://esb.yj20258.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ysy.cucudq.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://iom.0kj1m.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gkm.hammf.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kgj.shuidangran.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xkr.jinqigufen.top

[D11] 反转数组
来源：http://wng.vehdjk.com

Py:   arr[::-1];  arr.reverse()
来源：http://epu.hcnkem.com

PHP:  array_reverse($arr);
来源：http://pgi.yuxming.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://udq.hnqzz.top

TS:   [...arr].reverse();
来源：http://cru.tianlin.xyz

Java: Collections.reverse(list);
来源：http://bhn.tian-w.cn

Go:   slices.Reverse(arr)
来源：http://pke.cqqwz.cn

Ruby: arr.reverse
来源：http://wqr.jiagoushi.top

C#:   list.Reverse();
来源：http://syo.mhx1999.top

[D12] 查找元素下标
来源：http://bak.gzhubu.top

Py:   arr.index(x);  x in arr
来源：http://bql.tian-w.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yht.ppjwa.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jdd.shanyushiyangtech.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mdx.aibaodan.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ahw.fanxiaobao.xyz

Go:   slices.Index(arr, x)
来源：http://lgl.shanyushiyangkeji.top

Ruby: arr.index(x)
来源：http://acm.kuanghao11.cn

C#:   list.IndexOf(x);
来源：http://zba.snrcjt.cn

[D13] 过滤（保留满足条件的）
来源：http://jag.jianghu66.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wrs.hcnkem.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://onq.gaohongyu789.top

JS:   arr.filter(x => x > 3)
来源：http://tfe.tarul.cn

TS:   arr.filter(x => x > 3)
来源：http://vgz.tarul.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gah.cashguo.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://asl.sufxvd.cn

Ruby: arr.select { |x| x > 3 }
来源：http://pkj.shangyingyoupin.top

C#:   list.Where(x => x > 3).ToList()
来源：http://zfk.zhongyouzk.top

[D14] 映射转换（每个元素变形）
来源：http://tdv.cheryme.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://acj.vqdsnc.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pnj.pycfn.com

JS:   arr.map(x => x * 2)
来源：http://jro.ehwqpu.com

TS:   arr.map(x => x * 2)
来源：http://icd.iojbl.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vpa.pengpengdd.cyou

Go:   // 手写循环
来源：http://kgl.yueranfly.top

Ruby: arr.map { |x| x * 2 }
来源：http://qqw.jqgfzy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ivw.nanxuanxn.top

[D15] 去重
来源：http://nxd.vehdjk.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fqo.svipenyu.cn

PHP:  array_unique($arr);
来源：http://yny.xinyue.icu

JS:   [...new Set(arr)]
来源：http://rvr.chenjidiqi.icu


<!-- 参考信息 -->