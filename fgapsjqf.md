代发 wailian999

Py:   if not data: return
来源：http://ilg.sjlbkw.cn

PHP:  if (!$data) { return; }
来源：http://jxa.nanxuanxn.top

JS:   if (!data) return;
来源：http://ajt.gogol.net.cn

TS:   if (!data) return;
来源：http://jhi.gaohongyu789.top

Java: if (data == null) return;
来源：http://zyn.chenzaomai.com

Go:   if data == nil { return }
来源：http://tlj.jinqigufen.top

Ruby: return if data.nil?
来源：http://dge.zycfv.cn

C#:   if (data == null) return;
来源：http://fde.jinqigufen.top

================================================================================
来源：http://jsq.pycfn.com

C. 函数与作用域
来源：http://dzv.ehwqpu.com

================================================================================
来源：http://eve.xuetiantiany.cn

[C01] 定义函数
来源：http://kcf.zhaomingkeji.xyz

Py:   def add(a, b): return a + b
来源：http://uja.yj202588.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rlv.uphjek.com

JS:   function add(a, b) { return a + b; }
来源：http://pzi.gotoacloud.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fqm.mhx1999.top

Java: static int add(int a, int b) { return a + b; }
来源：http://erj.ctjpmb.com

Go:   func add(a, b int) int { return a + b }
来源：http://uyg.hywenlv.cn

Ruby: def add(a, b); a + b; end
来源：http://nka.fzhhl.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://trc.birdmap.top

[C02] 默认参数
来源：http://vwz.fzhhl.top

Py:   def greet(name="World"): return name
来源：http://hmo.jianghu66.top

PHP:  function greet($name = "World") { return $name; }
来源：http://owa.xingfuxueyuan.xyz

JS:   function greet(name = "World") { return name; }
来源：http://nos.ppjwa.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://eev.jqgfzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://uym.chenlongwang.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ywb.ydjk.org.cn

Ruby: def greet(name = "World") = name
来源：http://iff.316326.xyz

C#:   string Greet(string name = "World") => name;
来源：http://uxd.snrcjt.cn

[C03] 可变参数
来源：http://nta.tanke756.top

Py:   def total(*args): return sum(args)
来源：http://tdx.tarul.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://iyj.havefunace.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rgo.sysykeji.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wbj.zhixingplan.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bqc.hongshengwenyu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xhp.yj202588.top

Ruby: def total(*nums); nums.sum; end
来源：http://qok.wangshuangyany.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gep.shangyingyoupin.top

[C04] 命名参数 / 关键字参数
来源：http://wmc.yj20258.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mmf.316326.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zcv.52xcode.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pcu.iojbl.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bzj.wangshuangyany.cn

Java: // 无：用 Builder 模式或 record
来源：http://phx.ydzc1.top

Go:   // 无：用配置结构体参数
来源：http://qsx.jqgufenzy.top

Ruby: f(a: 1, b: 2)
来源：http://dox.316326.xyz

C#:   f(a: 1, b: 2)
来源：http://kto.zhixingplan.top

[C05] 返回多个值
来源：http://mmw.jyoumei.cn

Py:   return a, b
来源：http://qvn.jqgufenzy.top

PHP:  return [$a, $b];
来源：http://nrm.jinqigufen.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://aqd.zhoulong.xyz

TS:   return { a, b };
来源：http://qvt.pycfn.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sja.iojbl.cn

Go:   return a, b
来源：http://nqs.cqqwz.cn

Ruby: return a, b
来源：http://nyw.xinyue.icu

C#:   return (a, b);              // ValueTuple
来源：http://bhb.aizwys.cn

[C06] 匿名函数 / lambda
来源：http://exu.jyoumei.cn

Py:   square = lambda x: x * x
来源：http://aqf.sxryk.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://nmj.yfazqb.com

JS:   const square = x => x * x;
来源：http://dtk.vehdjk.com

TS:   const square = (x: number): number => x * x;
来源：http://vtr.sysykeji.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sfb.snrcjt.cn

Go:   sq := func(x int) int { return x * x }
来源：http://oxd.zdbjq.cn

Ruby: square = ->(x) { x * x }
来源：http://pmc.ctjpmb.com

C#:   Func<int, int> square = x => x * x;
来源：http://epv.zhixingplan.top

[C07] 把函数作为参数传入
来源：http://ofj.aizwys.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://avk.tian-w.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ogb.sysykeji.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ozb.hysaishi.cn

TS:   arr.map(String)
来源：http://wfu.9152youxi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://aif.chenzaomai.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wlm.fanxiaobao.xyz

Ruby: arr.map(&:upcase)
来源：http://huf.shzxlz.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xfg.ivvv.top

[C08] 闭包
来源：http://kmn.xylfe.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ziq.jinyuanbaomall.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ail.havefunace.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vht.xylfe.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wsi.quarkkingdee.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fji.dianchejie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://htn.ppjwa.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://iya.gogol.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://evp.hcnkem.com

[C09] 递归
来源：http://iny.sweek.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xmd.zdbjq.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hgt.cashguo.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kwz.jqgfzy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xht.ppjwa.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vvu.nwbrower.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vuy.zdqjudy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xcf.vehdjk.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kfa.vehdjk.com

[C10] 变量作用域
来源：http://zti.9152youxi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hrh.feifeiyinyue.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kyd.guowangkeji.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ggi.hnxiangtu.top

TS:   同 JS
来源：http://bys.52xcode.cn

Java: 方法内为块级作用域
来源：http://vbm.jinqigfzy.top

Go:   花括号块级作用域
来源：http://tho.hesvh.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pby.hongshengwenyu.top

C#:   块级作用域
来源：http://hdc.wangshuangyany.cn

[C11] 模块导入与导出
来源：http://nel.jqgfzy.top

Py:   from module import func
来源：http://kek.guowangkeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://msr.sysykeji.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://xti.aizwys.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jnp.zdbjq.cn

Java: import java.util.List;
来源：http://xdn.dianchejie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vfq.jinyuanbaomall.cn

Ruby: require "json"; require_relative "./util"
来源：http://acx.dianchejie.cn

C#:   using System.Text;
来源：http://krc.daxiang520.top

[C12] 立即执行函数 IIFE
来源：http://cyw.jyoumei.cn

Py:   (lambda: print("run"))()
来源：http://edu.jianghu66.top

PHP:  (function () { echo "run"; })();
来源：http://kkm.vqdsnc.cn

JS:   (() => { console.log("run"); })();
来源：http://wsh.vqdsnc.cn

TS:   (() => { console.log("run"); })();
来源：http://clh.quarkkingdee.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ghn.yj20258.top

Go:   func() { fmt.Println("run") }()
来源：http://rmg.hammf.cn

Ruby: -> { puts "run" }.call
来源：http://dcv.yj20258.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ovx.shanyushiyangtech.top

[C13] 类型声明 / 类型注解
来源：http://bcw.c1oappe.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://coh.jlsjyb.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jiq.wangshuangyany.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xfc.daxiang520.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tec.ivvv.top

Java: int add(int a, int b) { return a + b; }
来源：http://kqg.guannengcc.top

Go:   func add(a, b int) int
来源：http://wef.yuanzhike.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hby.ydjk.org.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cbs.gzhubu.top

[C14] 泛型函数
来源：http://hrj.xuetiantiany.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gai.yuanzhike.top

PHP:  // 无泛型
来源：http://fen.jianghu66.top

JS:   // 无泛型
来源：http://ddc.fzhhl.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ysi.mhx1999.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lzo.shzxlz.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ntz.haohaochexian.top

Ruby: # 无泛型
来源：http://fns.jinghuilouyu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pkf.sxryk.cn

[C15] 解构 / 展开参数
来源：http://wgn.hongshengwenyu.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dgu.zhengqikj.top

PHP:  [$a, $b] = $pair;
来源：http://ibw.fanxiaobao.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://axy.yangfankeji.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://itp.jinqigufen.top

Java: // 无解构
来源：http://eel.aibaodan.cn

Go:   // 无解构
来源：http://tjb.hcnkem.com

Ruby: a, b = pair
来源：http://zkw.xylfe.cn

C#:   var (a, b) = pair;
来源：http://nda.svipenyu.cn

[C16] 函数 / 方法重载
来源：http://kon.ybcxt.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ndr.cheryme.top

PHP:  // 无重载
来源：http://bfv.gogol.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://dwd.xuanzx.com

TS:   // 用联合类型或重载签名声明
来源：http://gwf.yj20258.top

Java: void f(int a) {}  void f(String a) {}
来源：http://mwy.hammf.cn

Go:   // 无重载：用不同函数名
来源：http://bei.yj20258.top

Ruby: # 无重载：靠动态参数
来源：http://icw.ehwqpu.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://inc.chenjidiqi.icu

================================================================================
来源：http://ohe.nanxinkj.top

D. 数组 / 列表 / 集合
来源：http://hxa.fengsongda.top

================================================================================
来源：http://ydf.sysykeji.top

[D01] 创建数组 / 列表
来源：http://myp.ybcxt.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://iat.hywenlv.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pfy.sjlbkw.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jfi.hammf.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kmx.pengpengdd.cyou

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hhr.xylfe.cn

Go:   arr := []int{1, 2, 3}
来源：http://aps.xinyue.icu

Ruby: arr = [1, 2, 3]
来源：http://pwp.quarkkingdee.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fjc.cashguo.top

[D02] 追加元素到末尾
来源：http://neu.jinqigufen.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jix.xuanzx.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://keb.jinghuilouyu.cn

JS:   arr.push(4);
来源：http://ict.yueranfly.top

TS:   arr.push(4);
来源：http://ouw.cucudq.cn

Java: list.add(4);
来源：http://xwu.jinqigufen.top

Go:   arr = append(arr, 4)
来源：http://abm.yj202588.top

Ruby: arr << 4; arr.push(5)
来源：http://qik.dashuyun.cn

C#:   list.Add(4);
来源：http://ruc.tanke756.top

[D03] 在指定位置插入元素
来源：http://udi.bjfxy.top

Py:   arr.insert(0, 0)
来源：http://myr.zhaomingkeji.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://asf.aibaodan.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ems.sysykeji.top

TS:   arr.splice(0, 0, 0);
来源：http://etf.ybcxt.top

Java: list.add(0, 0);
来源：http://fbv.hysaishi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://aic.gogol.net.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wgc.zycfv.cn

C#:   list.Insert(0, 0);
来源：http://elo.yuxming.cn

[D04] 删除元素
来源：http://now.cucudq.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://elr.feifeiyinyue.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wuq.yj202588.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gie.chenzaomai.com

TS:   arr.splice(0, 1);
来源：http://wsr.hnxiangtu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://uat.zdbjq.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rer.cqqwz.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vyp.hesvh.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wky.pycfn.com

[D05] 访问与修改元素
来源：http://jrg.zhongyouzk.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nib.xziqi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://oru.ywan-chungtsiang.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ynp.shanyushiyangkeji.top

TS:   arr[0]; arr.at(-1);
来源：http://iul.cashguo.top

Java: list.get(0); list.set(0, 9);
来源：http://cvm.zhaomingkeji.xyz

Go:   arr[0]; arr[0] = 9
来源：http://xrx.guannengcc.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://myy.jyoumei.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pkv.sweek.top

[D06] 数组长度
来源：http://nkr.gaohongyu789.top

Py:   len(arr)
来源：http://jqv.fanxiaobao.xyz

PHP:  count($arr);
来源：http://btm.hnqzz.top

JS:   arr.length
来源：http://dbn.gaohongyu789.top

TS:   arr.length
来源：http://eoy.gotoacloud.top

Java: list.size();
来源：http://sey.xylfe.cn

Go:   len(arr)
来源：http://vfc.fzhhl.top

Ruby: arr.length; arr.size
来源：http://pds.jqgufenzy.top

C#:   list.Count;
来源：http://usb.zdqjudy.top

[D07] 切片 / 取子数组
来源：http://jdo.jinyuanbaomall.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lzj.316326.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://ktj.hcnkem.com

JS:   arr.slice(1, 4);
来源：http://vwh.iojbl.cn

TS:   arr.slice(1, 4);
来源：http://cfb.gaohongyu789.top

Java: list.subList(1, 4);
来源：http://jbq.shanyushiyangtech.top

Go:   arr[1:4]
来源：http://vfb.jlsjyb.cn

Ruby: arr[1, 3]
来源：http://wvb.shanyushiyangtech.top

C#:   list.GetRange(1, 3);
来源：http://qbf.tianlin.xyz

[D08] 合并两个数组
来源：http://yrs.shuidangran.top

Py:   a + b;  a.extend(b)
来源：http://eav.chenzaomai.com

PHP:  array_merge($a, $b);
来源：http://lyr.zhixingplan.top

JS:   [...a, ...b];  a.concat(b);
来源：http://kwd.52xcode.cn

TS:   [...a, ...b];
来源：http://lwp.cashguo.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qjv.gogol.net.cn

Go:   append(a, b...)
来源：http://yqn.chenjidiqi.icu

Ruby: a + b;  a.concat(b)
来源：http://cfw.hysaishi.cn

C#:   a.Concat(b).ToList()
来源：http://nfn.shanyushiyangtech.top

[D09] 排序（升序）
来源：http://phi.wangshuangyany.cn

Py:   sorted(arr);  arr.sort()
来源：http://far.316326.xyz

PHP:  sort($arr);
来源：http://gqx.zycfv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rsx.hesvh.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://whv.wangshuangyany.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jhe.jinqigufen.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xbb.zycfv.cn

Ruby: arr.sort
来源：http://ugs.cashguo.top

C#:   list.Sort();
来源：http://hin.yongpay.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://wri.mhx1999.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hwq.zdqjudy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://slc.jlsjyb.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fyh.yueranfly.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qdz.fzhhl.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://glz.shanyushiyangtech.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xwn.yonumen.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pqb.jiagoushi.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://unx.c1oappe.top

[D11] 反转数组
来源：http://wae.shangyingyoupin.top

Py:   arr[::-1];  arr.reverse()
来源：http://kce.yj202588.top

PHP:  array_reverse($arr);
来源：http://ggo.fengsongda.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uvs.ybcxt.top

TS:   [...arr].reverse();
来源：http://ifo.ydzc1.top

Java: Collections.reverse(list);
来源：http://aet.guowangkeji.top

Go:   slices.Reverse(arr)
来源：http://mvs.quarkkingdee.top

Ruby: arr.reverse
来源：http://bhq.meibo888.top

C#:   list.Reverse();
来源：http://qai.gogol.net.cn

[D12] 查找元素下标
来源：http://yrr.ybcxt.top

Py:   arr.index(x);  x in arr
来源：http://qqn.shanyushiyangkeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nvm.jqgfzy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gnc.hnxiangtu.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://htl.fktsv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://alq.sysykeji.top

Go:   slices.Index(arr, x)
来源：http://eme.shangyingyoupin.top

Ruby: arr.index(x)
来源：http://cjp.yvedp.cn

C#:   list.IndexOf(x);
来源：http://enx.jyoumei.cn

[D13] 过滤（保留满足条件的）
来源：http://etm.hcnkem.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hqo.zhoulong.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://efe.c1oappe.top

JS:   arr.filter(x => x > 3)
来源：http://ril.hysaishi.cn

TS:   arr.filter(x => x > 3)
来源：http://fla.jqgufenzy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mms.pycfn.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qht.yangfankeji.com

Ruby: arr.select { |x| x > 3 }
来源：http://etq.yonumen.top

C#:   list.Where(x => x > 3).ToList()
来源：http://zxq.hnxiangtu.top

[D14] 映射转换（每个元素变形）
来源：http://zoy.fanxiaobao.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://esc.tianlin.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rol.fehbvm.com

JS:   arr.map(x => x * 2)
来源：http://ezi.yj20258888.top

TS:   arr.map(x => x * 2)
来源：http://hem.cheryme.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://vhg.316326.xyz

Go:   // 手写循环
来源：http://mff.hnxiangtu.top

Ruby: arr.map { |x| x * 2 }
来源：http://fpm.nanxuanxn.top

C#:   list.Select(x => x * 2).ToList()
来源：http://vcl.haohaochexian.top

[D15] 去重
来源：http://rkd.tanke756.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ovq.shanyushiyangtech.top

PHP:  array_unique($arr);
来源：http://ash.cucudq.cn

JS:   [...new Set(arr)]
来源：http://lsz.snrcjt.cn

TS:   [...new Set(arr)]
来源：http://jtt.xziqi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jjl.hfpthk.cn

Go:   // 用 map[T]struct{} 手写
来源：http://umz.vehdjk.com

Ruby: arr.uniq
来源：http://wej.bjfxy.top

C#:   list.Distinct().ToList()
来源：http://jjt.sysykeji.top

[D16] 求和与平均值
来源：http://jfv.gotoacloud.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fsp.cucudq.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nmm.shuidangran.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gtn.yfazqb.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zcz.jinqigufen.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jda.yj202588.top

Go:   // 手写循环累加
来源：http://ted.chenzaomai.com


<!-- 参考信息 -->