代发 wailian999

Py:   def add(a, b): return a + b
来源：http://piy.yj20258.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iwf.pycfn.com

JS:   function add(a, b) { return a + b; }
来源：http://fqg.yangfankeji.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uca.nanxuanxn.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ije.yangfankeji.com

Go:   func add(a, b int) int { return a + b }
来源：http://atj.vehdjk.com

Ruby: def add(a, b); a + b; end
来源：http://hqs.c1oappe.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lad.sjlbkw.cn

[C02] 默认参数
来源：http://mpp.fanxiaobao.xyz

Py:   def greet(name="World"): return name
来源：http://ssp.0kj1m.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zqw.dashuyun.cn

JS:   function greet(name = "World") { return name; }
来源：http://fax.52xcode.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://kla.hnxiangtu.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ucx.hnqzz.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cbw.cqqwz.cn

Ruby: def greet(name = "World") = name
来源：http://pvy.zhongyouzk.top

C#:   string Greet(string name = "World") => name;
来源：http://ijl.daxiang520.top

[C03] 可变参数
来源：http://erz.ppjwa.cn

Py:   def total(*args): return sum(args)
来源：http://wsi.gogol.net.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pun.ehwqpu.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bhr.quarkkingdee.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://swa.yuanzhike.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xgx.jqgufenzy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nyj.zhiwuduotai.top

Ruby: def total(*nums); nums.sum; end
来源：http://hdw.haohaochexian.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hvs.pycfn.com

[C04] 命名参数 / 关键字参数
来源：http://ihu.fengsongda.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wyi.tian-w.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fof.nanxinkj.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://btp.guannengcc.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bby.hywenlv.cn

Java: // 无：用 Builder 模式或 record
来源：http://pcm.daxiang520.top

Go:   // 无：用配置结构体参数
来源：http://pwi.tianlin.xyz

Ruby: f(a: 1, b: 2)
来源：http://gbo.vqdsnc.cn

C#:   f(a: 1, b: 2)
来源：http://pyl.jqgfzy.top

[C05] 返回多个值
来源：http://fko.fktsv.cn

Py:   return a, b
来源：http://gek.yvedp.cn

PHP:  return [$a, $b];
来源：http://jvg.smart0.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://lqm.shanyushiyangkeji.top

TS:   return { a, b };
来源：http://slu.jqgfzy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vyh.sjlbkw.cn

Go:   return a, b
来源：http://ojt.daria6918.cn

Ruby: return a, b
来源：http://qlx.52xcode.cn

C#:   return (a, b);              // ValueTuple
来源：http://zpw.wangshuangyany.cn

[C06] 匿名函数 / lambda
来源：http://fot.xuanzx.com

Py:   square = lambda x: x * x
来源：http://mwm.smart0.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://btf.316326.xyz

JS:   const square = x => x * x;
来源：http://ivh.xuanzx.com

TS:   const square = (x: number): number => x * x;
来源：http://mhg.jqgufenzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mlh.mhx1999.top

Go:   sq := func(x int) int { return x * x }
来源：http://xwy.sysykeji.top

Ruby: square = ->(x) { x * x }
来源：http://aov.ivvv.top

C#:   Func<int, int> square = x => x * x;
来源：http://kuv.jinqigufen.top

[C07] 把函数作为参数传入
来源：http://ajf.hongshengwenyu.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wse.cheryme.top

PHP:  array_map("strtoupper", $arr);
来源：http://jfh.jianghu66.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gdl.zdqjudy.top

TS:   arr.map(String)
来源：http://nis.shangyingyoupin.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gcx.sjlbkw.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ltw.gaohongyu789.top

Ruby: arr.map(&:upcase)
来源：http://iks.jqgfzy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://jqh.quarkkingdee.top

[C08] 闭包
来源：http://zkp.dashuyun.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pnr.snrcjt.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ogx.nanxuanxn.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xsf.hysaishi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ldu.jiagoushi.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rdw.hfpthk.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://umu.yfazqb.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://btm.yj202588.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fde.fehbvm.com

[C09] 递归
来源：http://gfi.ydjk.org.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://txd.fktsv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bwu.jinqigufen.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xsl.yvedp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ryl.zhiwuduotai.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ckw.mhx1999.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rgk.yj202588.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rpw.hysaishi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hub.nanxuanxn.top

[C10] 变量作用域
来源：http://qhv.ydzc1.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gaa.wangshuangyany.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bnz.jiagoushi.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wqx.chenlongwang.top

TS:   同 JS
来源：http://wdb.birdmap.top

Java: 方法内为块级作用域
来源：http://ztb.pengpengdd.cyou

Go:   花括号块级作用域
来源：http://rdn.bbcook.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://okf.hesvh.cn

C#:   块级作用域
来源：http://fdk.shuidangran.top

[C11] 模块导入与导出
来源：http://vvo.sysykeji.top

Py:   from module import func
来源：http://bgn.iojbl.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xmb.nwbrower.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://tyb.fengsongda.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pzx.hfpthk.cn

Java: import java.util.List;
来源：http://rrd.yvedp.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zlo.c1oappe.top

Ruby: require "json"; require_relative "./util"
来源：http://umm.feifeiyinyue.top

C#:   using System.Text;
来源：http://ggu.iojbl.cn

[C12] 立即执行函数 IIFE
来源：http://eni.birdmap.top

Py:   (lambda: print("run"))()
来源：http://abf.jiagoushi.top

PHP:  (function () { echo "run"; })();
来源：http://twn.zhaomingkeji.xyz

JS:   (() => { console.log("run"); })();
来源：http://gsz.cheryme.top

TS:   (() => { console.log("run"); })();
来源：http://zxg.birdmap.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://axp.gotoacloud.top

Go:   func() { fmt.Println("run") }()
来源：http://jrm.gzhubu.top

Ruby: -> { puts "run" }.call
来源：http://bno.xinyue.icu

C#:   // 无 IIFE：用静态构造函数
来源：http://zlx.shangyingyoupin.top

[C13] 类型声明 / 类型注解
来源：http://pjz.epnwcf.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zkp.dashuyun.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xxs.zhixingplan.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://eqr.chenlongwang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vbr.zhengqikj.top

Java: int add(int a, int b) { return a + b; }
来源：http://ikb.ydzc1.top

Go:   func add(a, b int) int
来源：http://lpm.cdnleiting.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ovp.fktsv.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mim.zhongyouzk.top

[C14] 泛型函数
来源：http://bgu.shanyushiyangkeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://oft.aibaodan.cn

PHP:  // 无泛型
来源：http://ous.fktsv.cn

JS:   // 无泛型
来源：http://eor.tian-w.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hsu.epnwcf.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dra.yueranfly.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vgw.pengpengdd.cyou

Ruby: # 无泛型
来源：http://rtv.quarkkingdee.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rhl.redwolf501.top

[C15] 解构 / 展开参数
来源：http://kgz.haohaochexian.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zwd.jinghuilouyu.cn

PHP:  [$a, $b] = $pair;
来源：http://lcp.ydzc1.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rxs.guannengcc.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ziw.snrcjt.cn

Java: // 无解构
来源：http://wup.xziqi.cn

Go:   // 无解构
来源：http://ghn.ehwqpu.com

Ruby: a, b = pair
来源：http://rxv.zycfv.cn

C#:   var (a, b) = pair;
来源：http://hwg.yfazqb.com

[C16] 函数 / 方法重载
来源：http://rvx.yj202588.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pmz.bjfxy.top

PHP:  // 无重载
来源：http://zaz.ctjpmb.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://rwg.c1oappe.top

TS:   // 用联合类型或重载签名声明
来源：http://txw.yj20258.top

Java: void f(int a) {}  void f(String a) {}
来源：http://uim.daria6918.cn

Go:   // 无重载：用不同函数名
来源：http://vsf.nwbrower.top

Ruby: # 无重载：靠动态参数
来源：http://xau.xuanzx.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://dkf.hysaishi.cn

================================================================================
来源：http://uiu.yvedp.cn

D. 数组 / 列表 / 集合
来源：http://nzh.jiagoushi.top

================================================================================
来源：http://krv.yvedp.cn

[D01] 创建数组 / 列表
来源：http://iup.kuanghao11.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://dsy.pengpengdd.cyou

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qdw.yueranfly.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xjt.epnwcf.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://yxa.quarkkingdee.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hnd.yanxiufei.cn

Go:   arr := []int{1, 2, 3}
来源：http://fde.pycfn.com

Ruby: arr = [1, 2, 3]
来源：http://pjk.hongshengwenyu.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://drm.sysykeji.top

[D02] 追加元素到末尾
来源：http://ygy.tian-w.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ihu.kuanghao11.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qza.uphjek.com

JS:   arr.push(4);
来源：http://ilu.hongshengwenyu.top

TS:   arr.push(4);
来源：http://uwc.fanxiaobao.xyz

Java: list.add(4);
来源：http://pfb.zhijiandao.cn

Go:   arr = append(arr, 4)
来源：http://zlv.cucudq.cn

Ruby: arr << 4; arr.push(5)
来源：http://ehb.cdnleiting.top

C#:   list.Add(4);
来源：http://nso.jinqigfzy.top

[D03] 在指定位置插入元素
来源：http://ulf.yj20258888.top

Py:   arr.insert(0, 0)
来源：http://mum.ppjwa.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://plr.sxryk.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lwu.tian-w.cn

TS:   arr.splice(0, 0, 0);
来源：http://oez.xylfe.cn

Java: list.add(0, 0);
来源：http://mre.havefunace.top

Go:   arr = append([]int{0}, arr...)
来源：http://vxi.vehdjk.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hxb.yj202588.top

C#:   list.Insert(0, 0);
来源：http://tpm.ybcxt.top

[D04] 删除元素
来源：http://ofv.yfazqb.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hch.yueranfly.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qhf.zhiwuduotai.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ufz.quarkkingdee.top

TS:   arr.splice(0, 1);
来源：http://xxu.sufxvd.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rvt.snrcjt.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nfq.cheryme.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ppl.ehwqpu.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kjh.shanyushiyangtech.top

[D05] 访问与修改元素
来源：http://oyw.jinqigfzy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kav.iojbl.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ysi.hnxiangtu.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://amh.nanxinkj.top

TS:   arr[0]; arr.at(-1);
来源：http://ksd.zhongyouzk.top

Java: list.get(0); list.set(0, 9);
来源：http://zhy.aizwys.cn

Go:   arr[0]; arr[0] = 9
来源：http://osz.nwbrower.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dcw.yanxiufei.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mwf.xziqi.cn

[D06] 数组长度
来源：http://npm.jinghuilouyu.cn

Py:   len(arr)
来源：http://rim.nanxuanxn.top

PHP:  count($arr);
来源：http://jki.fanxiaobao.xyz

JS:   arr.length
来源：http://xhj.yongpay.top

TS:   arr.length
来源：http://rnf.ehwqpu.com

Java: list.size();
来源：http://zju.chenzaomai.com

Go:   len(arr)
来源：http://ozb.shanyushiyangtech.top

Ruby: arr.length; arr.size
来源：http://nsn.zdbjq.cn

C#:   list.Count;
来源：http://ado.tarul.cn

[D07] 切片 / 取子数组
来源：http://mxs.xuanzx.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rld.dashuyun.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xwi.zhengqikj.top

JS:   arr.slice(1, 4);
来源：http://jit.andypj.xyz

TS:   arr.slice(1, 4);
来源：http://hwj.gogol.net.cn

Java: list.subList(1, 4);
来源：http://fnj.jinyuanbaomall.cn

Go:   arr[1:4]
来源：http://zul.daxiang520.top

Ruby: arr[1, 3]
来源：http://sli.zdqjudy.top

C#:   list.GetRange(1, 3);
来源：http://bgw.chenjidiqi.icu

[D08] 合并两个数组
来源：http://rlb.zhijiandao.cn

Py:   a + b;  a.extend(b)
来源：http://ibh.yvedp.cn

PHP:  array_merge($a, $b);
来源：http://cra.bbcook.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://arz.cdnleiting.top

TS:   [...a, ...b];
来源：http://ygs.yuanzhike.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qrl.c1oappe.top

Go:   append(a, b...)
来源：http://gxm.zdbjq.cn

Ruby: a + b;  a.concat(b)
来源：http://mxn.chenzaomai.com

C#:   a.Concat(b).ToList()
来源：http://ybj.cashguo.top

[D09] 排序（升序）
来源：http://chc.zhijiandao.cn

Py:   sorted(arr);  arr.sort()
来源：http://noo.shuidangran.top

PHP:  sort($arr);
来源：http://hho.shanyushiyangtech.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bma.zdbjq.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cqd.fzhhl.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ema.xuanzx.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fgm.hnqzz.top

Ruby: arr.sort
来源：http://grk.tian-w.cn

C#:   list.Sort();
来源：http://inu.gaohongyu789.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://jwe.sysykeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tha.gzhubu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://csk.yuanzhike.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hhl.guowangkeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nkb.tanke756.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ivo.zhaomingkeji.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ehp.cqqwz.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ike.mhx1999.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kxx.pycfn.com

[D11] 反转数组
来源：http://fbo.tianlin.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://kai.epnwcf.com

PHP:  array_reverse($arr);
来源：http://fbr.gaohongyu789.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sok.xinyue.icu

TS:   [...arr].reverse();
来源：http://icv.316326.xyz

Java: Collections.reverse(list);
来源：http://jhj.ydjk.org.cn

Go:   slices.Reverse(arr)
来源：http://snl.9152youxi.cn

Ruby: arr.reverse
来源：http://dwe.sweek.top

C#:   list.Reverse();
来源：http://ano.zhaomingkeji.xyz

[D12] 查找元素下标
来源：http://mou.hysaishi.cn

Py:   arr.index(x);  x in arr
来源：http://hrv.feifeiyinyue.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yrn.pycfn.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dgs.chenlongwang.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ywq.jinghuilouyu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ydk.xylfe.cn

Go:   slices.Index(arr, x)
来源：http://nvp.zhengqikj.top

Ruby: arr.index(x)
来源：http://zbg.gaohongyu789.top

C#:   list.IndexOf(x);
来源：http://svf.hammf.cn

[D13] 过滤（保留满足条件的）
来源：http://ahj.dashuyun.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yym.jqgfzy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gkx.xziqi.cn

JS:   arr.filter(x => x > 3)
来源：http://exh.wangdashe.top

TS:   arr.filter(x => x > 3)
来源：http://cmv.jqgfzy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rkr.hnqzz.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bou.jinghuilouyu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://bmk.zhoulong.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://wnr.316326.xyz

[D14] 映射转换（每个元素变形）
来源：http://bow.xylfe.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://utz.fengsongda.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zky.zycfv.cn

JS:   arr.map(x => x * 2)
来源：http://gvq.yuxming.cn

TS:   arr.map(x => x * 2)
来源：http://oaq.guowangkeji.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://hxm.shanyushiyangtech.top

Go:   // 手写循环
来源：http://jom.xinyue.icu

Ruby: arr.map { |x| x * 2 }
来源：http://ecb.dashuyun.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://tqw.fzhhl.top

[D15] 去重
来源：http://dea.zhiwuduotai.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tzo.zhaomingkeji.xyz

PHP:  array_unique($arr);
来源：http://arr.wangdashe.top

JS:   [...new Set(arr)]
来源：http://jyz.haohaochexian.top

TS:   [...new Set(arr)]
来源：http://ejk.cucudq.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gwm.zhengqikj.top

Go:   // 用 map[T]struct{} 手写
来源：http://ynx.sweek.top

Ruby: arr.uniq
来源：http://yhi.meibo888.top

C#:   list.Distinct().ToList()
来源：http://qhj.xuanzx.com

[D16] 求和与平均值
来源：http://wht.svipenyu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zsy.andypj.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mpd.jinyuanbaomall.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kgx.shuidangran.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lbz.sysykeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lfz.dashuyun.cn

Go:   // 手写循环累加
来源：http://xhm.guannengcc.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qkr.hnxiangtu.top

C#:   list.Sum();  list.Average()
来源：http://usf.jinyuanbaomall.cn

[D17] 最大值与最小值
来源：http://ljt.0kj1m.cn

Py:   max(arr);  min(arr)
来源：http://uvv.birdmap.top

PHP:  max($arr);  min($arr);
来源：http://kgj.9152youxi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ykj.9152youxi.cn

TS:   Math.max(...arr);
来源：http://jrm.jqgfzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://zby.yuxming.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jnk.ydjk.org.cn

Ruby: arr.max;  arr.min
来源：http://ocg.hcnkem.com

C#:   list.Max();  list.Min()
来源：http://qbn.hesvh.cn

[D18] 扁平化嵌套数组
来源：http://bhx.yangfankeji.com


<!-- 参考信息 -->