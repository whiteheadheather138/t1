代发 wailian999

Java: if (data == null) return;
来源：http://oan.cqqwz.cn

Go:   if data == nil { return }
来源：http://acc.sxryk.cn

Ruby: return if data.nil?
来源：http://fzl.shuidangran.top

C#:   if (data == null) return;
来源：http://wke.bbcook.cn

================================================================================
来源：http://zsh.ppjwa.cn

C. 函数与作用域
来源：http://qgc.dashuyun.cn

================================================================================
来源：http://phf.fanxiaobao.xyz

[C01] 定义函数
来源：http://gas.birdmap.top

Py:   def add(a, b): return a + b
来源：http://njf.snrcjt.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pfw.aibaodan.cn

JS:   function add(a, b) { return a + b; }
来源：http://tjc.ctjpmb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jgd.ywan-chungtsiang.top

Java: static int add(int a, int b) { return a + b; }
来源：http://kzw.ydjk.org.cn

Go:   func add(a, b int) int { return a + b }
来源：http://njf.dashuyun.cn

Ruby: def add(a, b); a + b; end
来源：http://mxb.zdqjudy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ntz.guannengcc.top

[C02] 默认参数
来源：http://ovj.ywan-chungtsiang.top

Py:   def greet(name="World"): return name
来源：http://xrd.tarul.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xwu.smart0.xyz

JS:   function greet(name = "World") { return name; }
来源：http://kiu.ctjpmb.com

TS:   function greet(name: string = "World") { return name; }
来源：http://zsc.dashuyun.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://nge.xuanzx.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gta.pycfn.com

Ruby: def greet(name = "World") = name
来源：http://ksy.yj20258.top

C#:   string Greet(string name = "World") => name;
来源：http://xrr.c1oappe.top

[C03] 可变参数
来源：http://wgy.wangshuangyany.cn

Py:   def total(*args): return sum(args)
来源：http://kpg.tanke756.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ssx.xuanzx.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kdv.snrcjt.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pvr.quarkkingdee.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hqm.chenlongwang.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://erb.xinyue.icu

Ruby: def total(*nums); nums.sum; end
来源：http://fgn.yangfankeji.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sda.fehbvm.com

[C04] 命名参数 / 关键字参数
来源：http://vnl.epnwcf.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ocg.haohaochexian.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vdu.daxiang520.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rhi.hywenlv.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dnc.gogol.net.cn

Java: // 无：用 Builder 模式或 record
来源：http://elb.fktsv.cn

Go:   // 无：用配置结构体参数
来源：http://aki.cucudq.cn

Ruby: f(a: 1, b: 2)
来源：http://hlq.zdqjudy.top

C#:   f(a: 1, b: 2)
来源：http://jcg.nanxinkj.top

[C05] 返回多个值
来源：http://mhx.bbcook.cn

Py:   return a, b
来源：http://clb.quarkkingdee.top

PHP:  return [$a, $b];
来源：http://abc.gotoacloud.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://kxs.0kj1m.cn

TS:   return { a, b };
来源：http://yoy.aibaodan.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kqy.zdbjq.cn

Go:   return a, b
来源：http://jgk.ppjwa.cn

Ruby: return a, b
来源：http://xru.guowangkeji.top

C#:   return (a, b);              // ValueTuple
来源：http://xbc.hnqzz.top

[C06] 匿名函数 / lambda
来源：http://ffa.yuanzhike.top

Py:   square = lambda x: x * x
来源：http://ivh.xinyue.icu

PHP:  $square = fn($x) => $x * $x;
来源：http://wjm.nwbrower.top

JS:   const square = x => x * x;
来源：http://rqm.vqdsnc.cn

TS:   const square = (x: number): number => x * x;
来源：http://fbv.andypj.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://uhb.52xcode.cn

Go:   sq := func(x int) int { return x * x }
来源：http://eap.jinghuilouyu.cn

Ruby: square = ->(x) { x * x }
来源：http://pep.hesvh.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ioo.birdmap.top

[C07] 把函数作为参数传入
来源：http://hev.52xcode.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rbg.zhijiandao.cn

PHP:  array_map("strtoupper", $arr);
来源：http://orp.daxiang520.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nis.smart0.xyz

TS:   arr.map(String)
来源：http://cso.aizwys.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vbd.gaohongyu789.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yhd.c1oappe.top

Ruby: arr.map(&:upcase)
来源：http://dms.zhijiandao.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://arl.jinqigfzy.top

[C08] 闭包
来源：http://ezb.chenzaomai.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hrc.dashuyun.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hsa.52xcode.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ghy.jyoumei.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tzk.feifeiyinyue.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hxn.xziqi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xnj.cucudq.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qkq.bjfxy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wyu.svipenyu.cn

[C09] 递归
来源：http://rzc.vehdjk.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qwu.yonumen.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://apw.zhiwuduotai.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tel.chenjidiqi.icu

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xjv.yj20258888.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pmj.jqgufenzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uvz.pycfn.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bvu.yuxming.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lnh.iojbl.cn

[C10] 变量作用域
来源：http://htr.xingfuxueyuan.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qmk.vqdsnc.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nuf.ybcxt.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lpj.daxiang520.top

TS:   同 JS
来源：http://fsn.uphjek.com

Java: 方法内为块级作用域
来源：http://rzu.jqgufenzy.top

Go:   花括号块级作用域
来源：http://kya.gzhubu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cbm.cheryme.top

C#:   块级作用域
来源：http://gih.andypj.xyz

[C11] 模块导入与导出
来源：http://xza.nanxinkj.top

Py:   from module import func
来源：http://dnb.jinghuilouyu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ajy.zhaomingkeji.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://ycj.redwolf501.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ylo.jianghu66.top

Java: import java.util.List;
来源：http://xyt.ydzc1.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://eyk.ydjk.org.cn

Ruby: require "json"; require_relative "./util"
来源：http://xcs.nanxinkj.top

C#:   using System.Text;
来源：http://uze.jinyuanbaomall.cn

[C12] 立即执行函数 IIFE
来源：http://syy.hammf.cn

Py:   (lambda: print("run"))()
来源：http://bfk.yongpay.top

PHP:  (function () { echo "run"; })();
来源：http://ovj.jqgufenzy.top

JS:   (() => { console.log("run"); })();
来源：http://asg.gotoacloud.top

TS:   (() => { console.log("run"); })();
来源：http://jci.nanxuanxn.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fqe.shuidangran.top

Go:   func() { fmt.Println("run") }()
来源：http://tmg.jinqigufen.top

Ruby: -> { puts "run" }.call
来源：http://ymr.chenzaomai.com

C#:   // 无 IIFE：用静态构造函数
来源：http://xxg.havefunace.top

[C13] 类型声明 / 类型注解
来源：http://aph.0kj1m.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://iwj.tanke756.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vmr.yuanzhike.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zje.dianchejie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bst.haohaochexian.top

Java: int add(int a, int b) { return a + b; }
来源：http://idq.sweek.top

Go:   func add(a, b int) int
来源：http://xxs.ydjk.org.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fqz.birdmap.top

C#:   int Add(int a, int b) => a + b;
来源：http://ilj.hongshengwenyu.top

[C14] 泛型函数
来源：http://iyk.cqqwz.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rap.ehwqpu.com

PHP:  // 无泛型
来源：http://qyv.shzxlz.cn

JS:   // 无泛型
来源：http://bwf.nanxuanxn.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zbz.yongpay.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kwh.smart0.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qwu.cucudq.cn

Ruby: # 无泛型
来源：http://gga.fktsv.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://iqi.jinyuanbaomall.cn

[C15] 解构 / 展开参数
来源：http://afx.xinyue.icu

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lzp.ppjwa.cn

PHP:  [$a, $b] = $pair;
来源：http://vts.feifeiyinyue.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ezq.tianlin.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fim.zhiwuduotai.top

Java: // 无解构
来源：http://bbc.yj20258888.top

Go:   // 无解构
来源：http://gvv.tianlin.xyz

Ruby: a, b = pair
来源：http://luf.redwolf501.top

C#:   var (a, b) = pair;
来源：http://lpk.0kj1m.cn

[C16] 函数 / 方法重载
来源：http://lyx.yuanzhike.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ylk.svipenyu.cn

PHP:  // 无重载
来源：http://lmb.tianlin.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://dlb.hcnkem.com

TS:   // 用联合类型或重载签名声明
来源：http://fip.tarul.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://lor.yj202588.top

Go:   // 无重载：用不同函数名
来源：http://xaj.fktsv.cn

Ruby: # 无重载：靠动态参数
来源：http://ygg.ydjk.org.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://eqa.chenjidiqi.icu

================================================================================
来源：http://joz.yuanzhike.top

D. 数组 / 列表 / 集合
来源：http://fid.xuanzx.com

================================================================================
来源：http://uza.xuetiantiany.cn

[D01] 创建数组 / 列表
来源：http://vct.yuanzhike.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://njk.yvedp.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sve.fzhhl.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://icw.sxryk.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://eoi.wangdashe.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lyg.xinyue.icu

Go:   arr := []int{1, 2, 3}
来源：http://tar.chenzaomai.com

Ruby: arr = [1, 2, 3]
来源：http://oej.jyoumei.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tot.guannengcc.top

[D02] 追加元素到末尾
来源：http://nie.zhoulong.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xsg.yj20258888.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ddk.ctjpmb.com

JS:   arr.push(4);
来源：http://jnn.redwolf501.top

TS:   arr.push(4);
来源：http://uqn.cdnleiting.top

Java: list.add(4);
来源：http://tfb.cucudq.cn

Go:   arr = append(arr, 4)
来源：http://osr.guowangkeji.top

Ruby: arr << 4; arr.push(5)
来源：http://faj.zhiwuduotai.top

C#:   list.Add(4);
来源：http://jle.hfpthk.cn

[D03] 在指定位置插入元素
来源：http://tge.birdmap.top

Py:   arr.insert(0, 0)
来源：http://ndi.hfpthk.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pvk.aizwys.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ysh.bbcook.cn

TS:   arr.splice(0, 0, 0);
来源：http://yhm.kuanghao11.cn

Java: list.add(0, 0);
来源：http://jzp.quarkkingdee.top

Go:   arr = append([]int{0}, arr...)
来源：http://tch.sysykeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cgw.xziqi.cn

C#:   list.Insert(0, 0);
来源：http://ihp.jinyuanbaomall.cn

[D04] 删除元素
来源：http://puv.tianlin.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gvk.yfazqb.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://aor.ywan-chungtsiang.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://drk.wangdashe.top

TS:   arr.splice(0, 1);
来源：http://rap.wangdashe.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mwa.kuanghao11.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pft.wangdashe.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://plg.zhixingplan.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nvd.jlsjyb.cn

[D05] 访问与修改元素
来源：http://dqr.zhijiandao.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zpw.tianlin.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rtp.guowangkeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ser.birdmap.top

TS:   arr[0]; arr.at(-1);
来源：http://gsy.andypj.xyz

Java: list.get(0); list.set(0, 9);
来源：http://gfw.dianchejie.cn

Go:   arr[0]; arr[0] = 9
来源：http://rwc.ctjpmb.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mou.zycfv.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ime.mhx1999.top

[D06] 数组长度
来源：http://aan.ehwqpu.com

Py:   len(arr)
来源：http://dhm.redwolf501.top

PHP:  count($arr);
来源：http://tys.yueranfly.top

JS:   arr.length
来源：http://err.shanyushiyangtech.top

TS:   arr.length
来源：http://ryp.chenlongwang.top

Java: list.size();
来源：http://cpc.hysaishi.cn

Go:   len(arr)
来源：http://ohp.sufxvd.cn

Ruby: arr.length; arr.size
来源：http://rwg.tianlin.xyz

C#:   list.Count;
来源：http://rxv.xuanzx.com

[D07] 切片 / 取子数组
来源：http://rqg.tarul.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ajo.hnxiangtu.top

PHP:  array_slice($arr, 1, 3);
来源：http://qjd.shanyushiyangkeji.top

JS:   arr.slice(1, 4);
来源：http://ssu.cashguo.top

TS:   arr.slice(1, 4);
来源：http://pdd.xylfe.cn

Java: list.subList(1, 4);
来源：http://nbh.hywenlv.cn

Go:   arr[1:4]
来源：http://fvc.ivvv.top

Ruby: arr[1, 3]
来源：http://zgj.sysykeji.top

C#:   list.GetRange(1, 3);
来源：http://krd.ybcxt.top

[D08] 合并两个数组
来源：http://unc.yangfankeji.com

Py:   a + b;  a.extend(b)
来源：http://akk.zdbjq.cn

PHP:  array_merge($a, $b);
来源：http://ynl.yongpay.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ksd.cdnleiting.top

TS:   [...a, ...b];
来源：http://mkv.jinqigufen.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wwd.ivvv.top

Go:   append(a, b...)
来源：http://dkl.yuanzhike.top

Ruby: a + b;  a.concat(b)
来源：http://cvd.fengsongda.top

C#:   a.Concat(b).ToList()
来源：http://nvb.yanxiufei.cn

[D09] 排序（升序）
来源：http://til.yuanzhike.top

Py:   sorted(arr);  arr.sort()
来源：http://rbe.yuxming.cn

PHP:  sort($arr);
来源：http://oxe.sufxvd.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://txp.epnwcf.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://mjr.wangshuangyany.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rin.shzxlz.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kiw.vehdjk.com

Ruby: arr.sort
来源：http://chw.cucudq.cn

C#:   list.Sort();
来源：http://abz.zhengqikj.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://qsf.tian-w.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fha.tianlin.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lqx.xuetiantiany.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zrh.kuanghao11.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://iht.zdqjudy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dtm.yj20258888.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xxl.yuanzhike.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pts.zhengqikj.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://har.tanke756.top

[D11] 反转数组
来源：http://wyp.xingfuxueyuan.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://zvg.tarul.cn

PHP:  array_reverse($arr);
来源：http://hmc.tianlin.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qum.fktsv.cn

TS:   [...arr].reverse();
来源：http://csm.zhaomingkeji.xyz

Java: Collections.reverse(list);
来源：http://mzd.cheryme.top

Go:   slices.Reverse(arr)
来源：http://obb.jyoumei.cn

Ruby: arr.reverse
来源：http://vog.hammf.cn

C#:   list.Reverse();
来源：http://dha.wangshuangyany.cn

[D12] 查找元素下标
来源：http://ska.pengpengdd.cyou

Py:   arr.index(x);  x in arr
来源：http://cjv.yvedp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://eda.hammf.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://evx.hesvh.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zwc.meibo888.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kyc.fengsongda.top

Go:   slices.Index(arr, x)
来源：http://rul.guowangkeji.top

Ruby: arr.index(x)
来源：http://ycv.jiagoushi.top

C#:   list.IndexOf(x);
来源：http://nbx.pengpengdd.cyou

[D13] 过滤（保留满足条件的）
来源：http://zuz.havefunace.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://krj.yvedp.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://egu.gogol.net.cn

JS:   arr.filter(x => x > 3)
来源：http://dxq.nanxuanxn.top

TS:   arr.filter(x => x > 3)
来源：http://lgg.bjfxy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hxp.sxryk.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ptx.aizwys.cn

Ruby: arr.select { |x| x > 3 }
来源：http://rit.yuanzhike.top

C#:   list.Where(x => x > 3).ToList()
来源：http://onw.redwolf501.top

[D14] 映射转换（每个元素变形）
来源：http://mud.havefunace.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fho.zhongyouzk.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cjx.havefunace.top

JS:   arr.map(x => x * 2)
来源：http://opo.zycfv.cn

TS:   arr.map(x => x * 2)
来源：http://sik.nanxinkj.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://osh.shangyingyoupin.top

Go:   // 手写循环
来源：http://pvq.nwbrower.top

Ruby: arr.map { |x| x * 2 }
来源：http://aqq.yfazqb.com

C#:   list.Select(x => x * 2).ToList()
来源：http://kec.hnxiangtu.top

[D15] 去重
来源：http://zit.xuanzx.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://amt.nanxinkj.top

PHP:  array_unique($arr);
来源：http://mlc.hnqzz.top

JS:   [...new Set(arr)]
来源：http://tob.yvedp.cn

TS:   [...new Set(arr)]
来源：http://lyd.xinyue.icu

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jpz.zhoulong.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://vku.daria6918.cn

Ruby: arr.uniq
来源：http://jrk.shangyingyoupin.top

C#:   list.Distinct().ToList()
来源：http://eae.tarul.cn

[D16] 求和与平均值
来源：http://aah.jinqigfzy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rlm.jlsjyb.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hji.haohaochexian.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kja.pengpengdd.cyou

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://plt.andypj.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://chc.hfpthk.cn

Go:   // 手写循环累加
来源：http://zzv.sysykeji.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://opt.ybcxt.top

C#:   list.Sum();  list.Average()
来源：http://aol.zhaomingkeji.xyz

[D17] 最大值与最小值
来源：http://cos.shanyushiyangkeji.top

Py:   max(arr);  min(arr)
来源：http://lgv.cashguo.top


<!-- 参考信息 -->