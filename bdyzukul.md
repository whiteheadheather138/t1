代发 wailian999

[C02] 默认参数
来源：http://oxn.guannengcc.top

Py:   def greet(name="World"): return name
来源：http://rph.redwolf501.top

PHP:  function greet($name = "World") { return $name; }
来源：http://wbx.sweek.top

JS:   function greet(name = "World") { return name; }
来源：http://pfo.nanxinkj.top

TS:   function greet(name: string = "World") { return name; }
来源：http://mcd.hywenlv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wvy.xinyue.icu

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://btr.pycfn.com

Ruby: def greet(name = "World") = name
来源：http://msd.dashuyun.cn

C#:   string Greet(string name = "World") => name;
来源：http://vza.redwolf501.top

[C03] 可变参数
来源：http://tfo.hnqzz.top

Py:   def total(*args): return sum(args)
来源：http://vmh.sxryk.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://adm.fzhhl.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wtn.yuanzhike.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xud.jinqigufen.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zut.xingfuxueyuan.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hxn.0kj1m.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vxh.feifeiyinyue.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gqv.redwolf501.top

[C04] 命名参数 / 关键字参数
来源：http://lds.epnwcf.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mfe.hongshengwenyu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://odr.havefunace.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://znr.yueranfly.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tgo.andypj.xyz

Java: // 无：用 Builder 模式或 record
来源：http://djl.xuetiantiany.cn

Go:   // 无：用配置结构体参数
来源：http://sbm.nanxuanxn.top

Ruby: f(a: 1, b: 2)
来源：http://bla.cucudq.cn

C#:   f(a: 1, b: 2)
来源：http://sdw.zhixingplan.top

[C05] 返回多个值
来源：http://tyx.havefunace.top

Py:   return a, b
来源：http://chp.birdmap.top

PHP:  return [$a, $b];
来源：http://kph.xziqi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jpk.shanyushiyangkeji.top

TS:   return { a, b };
来源：http://uxm.yvedp.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lhh.zhengqikj.top

Go:   return a, b
来源：http://mhi.tanke756.top

Ruby: return a, b
来源：http://muf.gaohongyu789.top

C#:   return (a, b);              // ValueTuple
来源：http://ocu.zhixingplan.top

[C06] 匿名函数 / lambda
来源：http://ros.yanxiufei.cn

Py:   square = lambda x: x * x
来源：http://dcx.nwbrower.top

PHP:  $square = fn($x) => $x * $x;
来源：http://exo.hysaishi.cn

JS:   const square = x => x * x;
来源：http://odx.epnwcf.com

TS:   const square = (x: number): number => x * x;
来源：http://fqi.hnqzz.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://age.yfazqb.com

Go:   sq := func(x int) int { return x * x }
来源：http://hme.dianchejie.cn

Ruby: square = ->(x) { x * x }
来源：http://nml.zdbjq.cn

C#:   Func<int, int> square = x => x * x;
来源：http://htu.aibaodan.cn

[C07] 把函数作为参数传入
来源：http://ted.daria6918.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fom.jinqigufen.top

PHP:  array_map("strtoupper", $arr);
来源：http://knd.sweek.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fjr.cheryme.top

TS:   arr.map(String)
来源：http://mat.shzxlz.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fkt.haohaochexian.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lqv.hysaishi.cn

Ruby: arr.map(&:upcase)
来源：http://chk.chenjidiqi.icu

C#:   arr.Select(s => s.ToUpper())
来源：http://ibm.jlsjyb.cn

[C08] 闭包
来源：http://jql.ybcxt.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nba.hywenlv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fjy.svipenyu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vwo.pengpengdd.cyou

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://psw.xylfe.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xlh.vqdsnc.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://euw.jinqigfzy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cbi.daria6918.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dbw.gotoacloud.top

[C09] 递归
来源：http://uet.quarkkingdee.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mnm.smart0.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nxv.dashuyun.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xvf.vqdsnc.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uly.gogol.net.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://irc.chenlongwang.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cpt.yj20258888.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fip.ywan-chungtsiang.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vsc.zycfv.cn

[C10] 变量作用域
来源：http://ldn.andypj.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qdi.hfpthk.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zvq.redwolf501.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vll.zycfv.cn

TS:   同 JS
来源：http://gbh.bbcook.cn

Java: 方法内为块级作用域
来源：http://ekh.chenlongwang.top

Go:   花括号块级作用域
来源：http://fyo.zycfv.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gmu.jianghu66.top

C#:   块级作用域
来源：http://bxs.cqqwz.cn

[C11] 模块导入与导出
来源：http://wih.chenlongwang.top

Py:   from module import func
来源：http://vsm.hesvh.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://uzw.jqgufenzy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://tgf.meibo888.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gxx.bbcook.cn

Java: import java.util.List;
来源：http://zfw.gaohongyu789.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tjk.cashguo.top

Ruby: require "json"; require_relative "./util"
来源：http://moc.quarkkingdee.top

C#:   using System.Text;
来源：http://hcp.dashuyun.cn

[C12] 立即执行函数 IIFE
来源：http://kkt.zhongyouzk.top

Py:   (lambda: print("run"))()
来源：http://mxb.hnqzz.top

PHP:  (function () { echo "run"; })();
来源：http://fbq.kuanghao11.cn

JS:   (() => { console.log("run"); })();
来源：http://mwr.yonumen.top

TS:   (() => { console.log("run"); })();
来源：http://wln.yj20258.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mhc.chenzaomai.com

Go:   func() { fmt.Println("run") }()
来源：http://ozl.ctjpmb.com

Ruby: -> { puts "run" }.call
来源：http://edm.xinyue.icu

C#:   // 无 IIFE：用静态构造函数
来源：http://pat.iojbl.cn

[C13] 类型声明 / 类型注解
来源：http://qxq.redwolf501.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://laq.dianchejie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jit.nanxinkj.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mjx.316326.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jxk.gogol.net.cn

Java: int add(int a, int b) { return a + b; }
来源：http://znb.jiagoushi.top

Go:   func add(a, b int) int
来源：http://qqz.hnqzz.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dte.zycfv.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nnl.pycfn.com

[C14] 泛型函数
来源：http://qvq.ivvv.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://haj.yfazqb.com

PHP:  // 无泛型
来源：http://ilf.shangyingyoupin.top

JS:   // 无泛型
来源：http://osc.ppjwa.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nfn.hfpthk.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://omw.ctjpmb.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cfk.zhaomingkeji.xyz

Ruby: # 无泛型
来源：http://fiw.hammf.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nmz.sweek.top

[C15] 解构 / 展开参数
来源：http://inn.shanyushiyangkeji.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nat.guannengcc.top

PHP:  [$a, $b] = $pair;
来源：http://rog.mhx1999.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xhq.meibo888.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qde.zycfv.cn

Java: // 无解构
来源：http://vuk.ppjwa.cn

Go:   // 无解构
来源：http://ryz.ctjpmb.com

Ruby: a, b = pair
来源：http://eag.meibo888.top

C#:   var (a, b) = pair;
来源：http://vfi.xuanzx.com

[C16] 函数 / 方法重载
来源：http://xix.shuidangran.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ycp.shuidangran.top

PHP:  // 无重载
来源：http://nsb.smart0.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://eql.hnqzz.top

TS:   // 用联合类型或重载签名声明
来源：http://ysn.cashguo.top

Java: void f(int a) {}  void f(String a) {}
来源：http://tcy.hongshengwenyu.top

Go:   // 无重载：用不同函数名
来源：http://vmw.yj20258.top

Ruby: # 无重载：靠动态参数
来源：http://qls.zycfv.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zjd.hysaishi.cn

================================================================================
来源：http://vzg.xziqi.cn

D. 数组 / 列表 / 集合
来源：http://xfw.birdmap.top

================================================================================
来源：http://gzr.chenlongwang.top

[D01] 创建数组 / 列表
来源：http://fll.zdqjudy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://nwp.hammf.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nkf.jqgufenzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hii.kuanghao11.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ihv.gogol.net.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qpz.chenjidiqi.icu

Go:   arr := []int{1, 2, 3}
来源：http://hyr.tanke756.top

Ruby: arr = [1, 2, 3]
来源：http://yam.havefunace.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ptw.tianlin.xyz

[D02] 追加元素到末尾
来源：http://ovj.vehdjk.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zir.shanyushiyangtech.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dxh.yvedp.cn

JS:   arr.push(4);
来源：http://ssj.yangfankeji.com

TS:   arr.push(4);
来源：http://azb.uphjek.com

Java: list.add(4);
来源：http://vhr.yangfankeji.com

Go:   arr = append(arr, 4)
来源：http://kdm.c1oappe.top

Ruby: arr << 4; arr.push(5)
来源：http://wop.redwolf501.top

C#:   list.Add(4);
来源：http://rym.aibaodan.cn

[D03] 在指定位置插入元素
来源：http://uxu.hywenlv.cn

Py:   arr.insert(0, 0)
来源：http://rcr.jinqigufen.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uvp.snrcjt.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://eue.jinyuanbaomall.cn

TS:   arr.splice(0, 0, 0);
来源：http://mxx.xuanzx.com

Java: list.add(0, 0);
来源：http://xly.shangyingyoupin.top

Go:   arr = append([]int{0}, arr...)
来源：http://qga.yfazqb.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mzt.guannengcc.top

C#:   list.Insert(0, 0);
来源：http://ibr.fzhhl.top

[D04] 删除元素
来源：http://zeu.zdbjq.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lfz.redwolf501.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vyu.havefunace.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bqm.sxryk.cn

TS:   arr.splice(0, 1);
来源：http://wpk.ivvv.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rgp.daria6918.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dro.haohaochexian.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tzq.jinyuanbaomall.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mkt.sysykeji.top

[D05] 访问与修改元素
来源：http://teu.ppjwa.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zvq.52xcode.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kqi.pengpengdd.cyou

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vbz.guowangkeji.top

TS:   arr[0]; arr.at(-1);
来源：http://ydb.bbcook.cn

Java: list.get(0); list.set(0, 9);
来源：http://dkr.fzhhl.top

Go:   arr[0]; arr[0] = 9
来源：http://qcn.shanyushiyangkeji.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vok.bjfxy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cmb.tian-w.cn

[D06] 数组长度
来源：http://ivy.gzhubu.top

Py:   len(arr)
来源：http://qpd.svipenyu.cn

PHP:  count($arr);
来源：http://ydp.aibaodan.cn

JS:   arr.length
来源：http://qpg.jinyuanbaomall.cn

TS:   arr.length
来源：http://asd.aizwys.cn

Java: list.size();
来源：http://dll.smart0.xyz

Go:   len(arr)
来源：http://elq.yuxming.cn

Ruby: arr.length; arr.size
来源：http://kle.hammf.cn

C#:   list.Count;
来源：http://alx.vqdsnc.cn

[D07] 切片 / 取子数组
来源：http://bpe.zhengqikj.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pdt.tarul.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ske.haohaochexian.top

JS:   arr.slice(1, 4);
来源：http://pke.xingfuxueyuan.xyz

TS:   arr.slice(1, 4);
来源：http://dxc.zycfv.cn

Java: list.subList(1, 4);
来源：http://ykq.cqqwz.cn

Go:   arr[1:4]
来源：http://blz.nanxinkj.top

Ruby: arr[1, 3]
来源：http://jur.aizwys.cn

C#:   list.GetRange(1, 3);
来源：http://gnr.c1oappe.top

[D08] 合并两个数组
来源：http://una.chenjidiqi.icu

Py:   a + b;  a.extend(b)
来源：http://kzf.yongpay.top

PHP:  array_merge($a, $b);
来源：http://rxh.xuetiantiany.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vhg.jinghuilouyu.cn

TS:   [...a, ...b];
来源：http://tda.feifeiyinyue.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lse.cheryme.top

Go:   append(a, b...)
来源：http://jbf.sysykeji.top

Ruby: a + b;  a.concat(b)
来源：http://fok.yfazqb.com

C#:   a.Concat(b).ToList()
来源：http://wac.nwbrower.top

[D09] 排序（升序）
来源：http://iuw.fehbvm.com

Py:   sorted(arr);  arr.sort()
来源：http://zlj.0kj1m.cn

PHP:  sort($arr);
来源：http://tmw.tian-w.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://edi.guowangkeji.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://wwk.sysykeji.top

Java: Collections.sort(list);  list.sort(null);
来源：http://feb.hywenlv.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vti.0kj1m.cn

Ruby: arr.sort
来源：http://dyc.chenjidiqi.icu

C#:   list.Sort();
来源：http://mqz.yuanzhike.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://rpk.cucudq.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zfn.ybcxt.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hnu.c1oappe.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yxk.pengpengdd.cyou

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vov.tanke756.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ntd.tarul.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pan.nwbrower.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bei.haohaochexian.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://izc.uphjek.com

[D11] 反转数组
来源：http://dam.ydjk.org.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zjg.svipenyu.cn

PHP:  array_reverse($arr);
来源：http://mcm.ywan-chungtsiang.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cax.xuanzx.com

TS:   [...arr].reverse();
来源：http://vfp.daxiang520.top

Java: Collections.reverse(list);
来源：http://vmm.zhixingplan.top

Go:   slices.Reverse(arr)
来源：http://hzt.sjlbkw.cn

Ruby: arr.reverse
来源：http://vwv.nwbrower.top

C#:   list.Reverse();
来源：http://buc.ppjwa.cn

[D12] 查找元素下标
来源：http://zzv.shanyushiyangtech.top

Py:   arr.index(x);  x in arr
来源：http://tpt.zhiwuduotai.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cau.tanke756.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qnc.aizwys.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://erh.cqqwz.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gzh.fengsongda.top

Go:   slices.Index(arr, x)
来源：http://kes.guowangkeji.top

Ruby: arr.index(x)
来源：http://ieb.sweek.top

C#:   list.IndexOf(x);
来源：http://byi.ivvv.top

[D13] 过滤（保留满足条件的）
来源：http://ana.zycfv.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://olf.jyoumei.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vgi.ivvv.top

JS:   arr.filter(x => x > 3)
来源：http://mqh.haohaochexian.top

TS:   arr.filter(x => x > 3)
来源：http://mtj.zhoulong.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sbw.andypj.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hly.jinyuanbaomall.cn

Ruby: arr.select { |x| x > 3 }
来源：http://roo.sweek.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ujp.ydjk.org.cn

[D14] 映射转换（每个元素变形）
来源：http://rln.pengpengdd.cyou

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://axd.c1oappe.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ojz.sweek.top

JS:   arr.map(x => x * 2)
来源：http://ekh.sxryk.cn

TS:   arr.map(x => x * 2)
来源：http://zxp.vqdsnc.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://kzu.yj20258888.top

Go:   // 手写循环
来源：http://oop.zhoulong.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://oti.iojbl.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hak.andypj.xyz

[D15] 去重
来源：http://vuh.xylfe.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://eon.birdmap.top

PHP:  array_unique($arr);
来源：http://brh.guannengcc.top

JS:   [...new Set(arr)]
来源：http://uim.yvedp.cn

TS:   [...new Set(arr)]
来源：http://shr.redwolf501.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zqq.yj20258.top

Go:   // 用 map[T]struct{} 手写
来源：http://zyi.tarul.cn

Ruby: arr.uniq
来源：http://rzz.sjlbkw.cn

C#:   list.Distinct().ToList()
来源：http://jvh.fktsv.cn

[D16] 求和与平均值
来源：http://vxm.gzhubu.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wgu.jqgufenzy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vyq.hesvh.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://brz.ydjk.org.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qrm.shuidangran.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fpr.epnwcf.com

Go:   // 手写循环累加
来源：http://ive.gaohongyu789.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gst.zhijiandao.cn

C#:   list.Sum();  list.Average()
来源：http://fvv.yongpay.top

[D17] 最大值与最小值
来源：http://nxp.gzhubu.top

Py:   max(arr);  min(arr)
来源：http://awv.jqgfzy.top

PHP:  max($arr);  min($arr);
来源：http://fio.daria6918.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hmh.shzxlz.cn

TS:   Math.max(...arr);
来源：http://big.hfpthk.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ozj.hywenlv.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gxo.jinqigfzy.top

Ruby: arr.max;  arr.min
来源：http://fwv.fengsongda.top

C#:   list.Max();  list.Min()
来源：http://rmj.shangyingyoupin.top

[D18] 扁平化嵌套数组
来源：http://zaf.jqgfzy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cvw.vqdsnc.cn

PHP:  array_merge(...$nested);
来源：http://kse.hcnkem.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fek.jqgufenzy.top

TS:   nested.flat();
来源：http://qpd.zhixingplan.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kve.cheryme.top

Go:   // 手写双层循环
来源：http://lwc.yj20258888.top

Ruby: nested.flatten
来源：http://kak.yj202588.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ikm.aibaodan.cn


<!-- 参考信息 -->