代发 wailian999

Py:   if not data: return
来源：http://syr.xuanzx.com

PHP:  if (!$data) { return; }
来源：http://tun.chenlongwang.top

JS:   if (!data) return;
来源：http://log.aibaodan.cn

TS:   if (!data) return;
来源：http://cvs.kuanghao11.cn

Java: if (data == null) return;
来源：http://wyh.nwbrower.top

Go:   if data == nil { return }
来源：http://erf.fktsv.cn

Ruby: return if data.nil?
来源：http://aqp.0kj1m.cn

C#:   if (data == null) return;
来源：http://ivp.yfazqb.com

================================================================================
来源：http://ofb.xylfe.cn

C. 函数与作用域
来源：http://nyq.guannengcc.top

================================================================================
来源：http://nqo.guannengcc.top

[C01] 定义函数
来源：http://hsj.feifeiyinyue.top

Py:   def add(a, b): return a + b
来源：http://ojj.yonumen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qir.ydzc1.top

JS:   function add(a, b) { return a + b; }
来源：http://axc.gzhubu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tji.yongpay.top

Java: static int add(int a, int b) { return a + b; }
来源：http://tpw.ydzc1.top

Go:   func add(a, b int) int { return a + b }
来源：http://uiz.guowangkeji.top

Ruby: def add(a, b); a + b; end
来源：http://vma.cqqwz.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kou.jianghu66.top

[C02] 默认参数
来源：http://vby.zhengqikj.top

Py:   def greet(name="World"): return name
来源：http://ifr.sxryk.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://pjl.yanxiufei.cn

JS:   function greet(name = "World") { return name; }
来源：http://hnf.aibaodan.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vqd.zhoulong.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://rlz.yj20258888.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fdc.yongpay.top

Ruby: def greet(name = "World") = name
来源：http://uoj.hywenlv.cn

C#:   string Greet(string name = "World") => name;
来源：http://fto.yj20258.top

[C03] 可变参数
来源：http://ise.jiagoushi.top

Py:   def total(*args): return sum(args)
来源：http://luk.ybcxt.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://oto.redwolf501.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bfq.iojbl.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ahx.wangshuangyany.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yjc.ctjpmb.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ynf.svipenyu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://dqs.tanke756.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zyv.andypj.xyz

[C04] 命名参数 / 关键字参数
来源：http://xyw.gotoacloud.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sbx.aibaodan.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://oze.yuxming.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kdm.fehbvm.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gwq.cqqwz.cn

Java: // 无：用 Builder 模式或 record
来源：http://weo.9152youxi.cn

Go:   // 无：用配置结构体参数
来源：http://bcp.vqdsnc.cn

Ruby: f(a: 1, b: 2)
来源：http://hta.xylfe.cn

C#:   f(a: 1, b: 2)
来源：http://qbi.jyoumei.cn

[C05] 返回多个值
来源：http://oqo.shuidangran.top

Py:   return a, b
来源：http://ofo.havefunace.top

PHP:  return [$a, $b];
来源：http://khd.gogol.net.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ati.uphjek.com

TS:   return { a, b };
来源：http://osl.shzxlz.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qbv.yuxming.cn

Go:   return a, b
来源：http://fmz.zhixingplan.top

Ruby: return a, b
来源：http://gom.kuanghao11.cn

C#:   return (a, b);              // ValueTuple
来源：http://dae.dianchejie.cn

[C06] 匿名函数 / lambda
来源：http://czw.meibo888.top

Py:   square = lambda x: x * x
来源：http://axl.hammf.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://rhe.yj20258888.top

JS:   const square = x => x * x;
来源：http://uhr.wangshuangyany.cn

TS:   const square = (x: number): number => x * x;
来源：http://lui.zhongyouzk.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gbo.tianlin.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://urp.tanke756.top

Ruby: square = ->(x) { x * x }
来源：http://bzx.fzhhl.top

C#:   Func<int, int> square = x => x * x;
来源：http://rrp.cqqwz.cn

[C07] 把函数作为参数传入
来源：http://jgp.ppjwa.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ten.haohaochexian.top

PHP:  array_map("strtoupper", $arr);
来源：http://vsb.bbcook.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kgw.zhoulong.xyz

TS:   arr.map(String)
来源：http://xuv.birdmap.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cpr.zhengqikj.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ntj.hesvh.cn

Ruby: arr.map(&:upcase)
来源：http://kyx.jinyuanbaomall.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wdj.jqgufenzy.top

[C08] 闭包
来源：http://grm.cheryme.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jip.shuidangran.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rzg.0kj1m.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lxu.yangfankeji.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://oko.jinqigfzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gjm.yfazqb.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://czc.nwbrower.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vcl.vehdjk.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gnj.xuanzx.com

[C09] 递归
来源：http://jew.uphjek.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dpz.sysykeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ebi.snrcjt.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mnl.fengsongda.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nxo.ehwqpu.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uxp.fehbvm.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://twz.cucudq.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wyf.zhiwuduotai.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://idb.chenzaomai.com

[C10] 变量作用域
来源：http://yjg.cdnleiting.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rtx.9152youxi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://oqo.vqdsnc.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mfg.fehbvm.com

TS:   同 JS
来源：http://cyq.shuidangran.top

Java: 方法内为块级作用域
来源：http://krz.havefunace.top

Go:   花括号块级作用域
来源：http://zey.tianlin.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wtv.gotoacloud.top

C#:   块级作用域
来源：http://vbv.jinghuilouyu.cn

[C11] 模块导入与导出
来源：http://syw.yj20258888.top

Py:   from module import func
来源：http://xxr.zhaomingkeji.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://jwd.tian-w.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zdg.jinyuanbaomall.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qgs.hywenlv.cn

Java: import java.util.List;
来源：http://pdq.guowangkeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nog.shuidangran.top

Ruby: require "json"; require_relative "./util"
来源：http://qvt.vehdjk.com

C#:   using System.Text;
来源：http://ouf.nanxinkj.top

[C12] 立即执行函数 IIFE
来源：http://wgp.316326.xyz

Py:   (lambda: print("run"))()
来源：http://gdk.yuxming.cn

PHP:  (function () { echo "run"; })();
来源：http://aaf.jinghuilouyu.cn

JS:   (() => { console.log("run"); })();
来源：http://yoi.shzxlz.cn

TS:   (() => { console.log("run"); })();
来源：http://zpg.redwolf501.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ndt.zhijiandao.cn

Go:   func() { fmt.Println("run") }()
来源：http://dek.wangshuangyany.cn

Ruby: -> { puts "run" }.call
来源：http://clq.jyoumei.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://uir.ywan-chungtsiang.top

[C13] 类型声明 / 类型注解
来源：http://ext.chenjidiqi.icu

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mef.guannengcc.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jpa.daxiang520.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tut.tanke756.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jab.daria6918.cn

Java: int add(int a, int b) { return a + b; }
来源：http://pof.zycfv.cn

Go:   func add(a, b int) int
来源：http://tle.yvedp.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hma.yueranfly.top

C#:   int Add(int a, int b) => a + b;
来源：http://emz.xziqi.cn

[C14] 泛型函数
来源：http://zzt.redwolf501.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mwt.gaohongyu789.top

PHP:  // 无泛型
来源：http://aoa.fehbvm.com

JS:   // 无泛型
来源：http://dqu.snrcjt.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://egi.wangdashe.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tdr.hnqzz.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://meh.pycfn.com

Ruby: # 无泛型
来源：http://qmn.fehbvm.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://akg.ehwqpu.com

[C15] 解构 / 展开参数
来源：http://fuf.hnqzz.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hpj.redwolf501.top

PHP:  [$a, $b] = $pair;
来源：http://riz.shzxlz.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hdu.dashuyun.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lgb.cqqwz.cn

Java: // 无解构
来源：http://dlj.ybcxt.top

Go:   // 无解构
来源：http://xpg.iojbl.cn

Ruby: a, b = pair
来源：http://dpl.jyoumei.cn

C#:   var (a, b) = pair;
来源：http://awa.shangyingyoupin.top

[C16] 函数 / 方法重载
来源：http://vfm.hongshengwenyu.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://iku.0kj1m.cn

PHP:  // 无重载
来源：http://ewr.zhiwuduotai.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://hqq.yvedp.cn

TS:   // 用联合类型或重载签名声明
来源：http://oua.dashuyun.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://szg.hongshengwenyu.top

Go:   // 无重载：用不同函数名
来源：http://fhc.cashguo.top

Ruby: # 无重载：靠动态参数
来源：http://gfx.jyoumei.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qxc.chenlongwang.top

================================================================================
来源：http://muz.tian-w.cn

D. 数组 / 列表 / 集合
来源：http://lzp.daxiang520.top

================================================================================
来源：http://kaz.jqgufenzy.top

[D01] 创建数组 / 列表
来源：http://zae.gotoacloud.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://nho.ppjwa.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xgf.daxiang520.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cvi.shangyingyoupin.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://spg.zhiwuduotai.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://oqr.ydjk.org.cn

Go:   arr := []int{1, 2, 3}
来源：http://tha.iojbl.cn

Ruby: arr = [1, 2, 3]
来源：http://atk.jinqigufen.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ngm.tianlin.xyz

[D02] 追加元素到末尾
来源：http://syu.gogol.net.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://onp.cheryme.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xfy.shuidangran.top

JS:   arr.push(4);
来源：http://rby.ydzc1.top

TS:   arr.push(4);
来源：http://rtr.bjfxy.top

Java: list.add(4);
来源：http://uak.hfpthk.cn

Go:   arr = append(arr, 4)
来源：http://quu.sysykeji.top

Ruby: arr << 4; arr.push(5)
来源：http://fgs.chenjidiqi.icu

C#:   list.Add(4);
来源：http://ksb.bjfxy.top

[D03] 在指定位置插入元素
来源：http://zso.sysykeji.top

Py:   arr.insert(0, 0)
来源：http://dts.zdbjq.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uud.fzhhl.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hvb.nwbrower.top

TS:   arr.splice(0, 0, 0);
来源：http://frq.pengpengdd.cyou

Java: list.add(0, 0);
来源：http://uyz.zhijiandao.cn

Go:   arr = append([]int{0}, arr...)
来源：http://rcj.sysykeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nrq.yuanzhike.top

C#:   list.Insert(0, 0);
来源：http://kim.hcnkem.com

[D04] 删除元素
来源：http://vtc.hywenlv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ksm.guowangkeji.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://btp.yuanzhike.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://eib.gotoacloud.top

TS:   arr.splice(0, 1);
来源：http://pzh.yvedp.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zxh.nanxuanxn.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sgm.mhx1999.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vxu.chenzaomai.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://eyd.uphjek.com

[D05] 访问与修改元素
来源：http://ekp.cdnleiting.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ync.xingfuxueyuan.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tpz.c1oappe.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ktg.tianlin.xyz

TS:   arr[0]; arr.at(-1);
来源：http://wlk.dashuyun.cn

Java: list.get(0); list.set(0, 9);
来源：http://qgv.mhx1999.top

Go:   arr[0]; arr[0] = 9
来源：http://ufp.jiagoushi.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yle.hammf.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://grv.jianghu66.top

[D06] 数组长度
来源：http://evs.jianghu66.top

Py:   len(arr)
来源：http://vym.xziqi.cn

PHP:  count($arr);
来源：http://gjd.zdqjudy.top

JS:   arr.length
来源：http://aje.ydjk.org.cn

TS:   arr.length
来源：http://zvc.jinyuanbaomall.cn

Java: list.size();
来源：http://vlb.chenlongwang.top

Go:   len(arr)
来源：http://azb.jianghu66.top

Ruby: arr.length; arr.size
来源：http://xmz.jiagoushi.top

C#:   list.Count;
来源：http://bao.kuanghao11.cn

[D07] 切片 / 取子数组
来源：http://nsc.yuanzhike.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mbq.sxryk.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ldu.yj202588.top

JS:   arr.slice(1, 4);
来源：http://ufa.tianlin.xyz

TS:   arr.slice(1, 4);
来源：http://mkb.yangfankeji.com

Java: list.subList(1, 4);
来源：http://byo.shanyushiyangtech.top

Go:   arr[1:4]
来源：http://avx.gogol.net.cn

Ruby: arr[1, 3]
来源：http://dyn.feifeiyinyue.top

C#:   list.GetRange(1, 3);
来源：http://dwz.yfazqb.com

[D08] 合并两个数组
来源：http://hvt.hnqzz.top

Py:   a + b;  a.extend(b)
来源：http://mgz.gaohongyu789.top

PHP:  array_merge($a, $b);
来源：http://xbn.daria6918.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://lkp.nwbrower.top

TS:   [...a, ...b];
来源：http://boj.sjlbkw.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xnn.shanyushiyangtech.top

Go:   append(a, b...)
来源：http://yis.fktsv.cn

Ruby: a + b;  a.concat(b)
来源：http://tsp.tarul.cn

C#:   a.Concat(b).ToList()
来源：http://jqm.bjfxy.top

[D09] 排序（升序）
来源：http://jsq.ydzc1.top

Py:   sorted(arr);  arr.sort()
来源：http://epb.cheryme.top

PHP:  sort($arr);
来源：http://kcx.bbcook.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://usn.yanxiufei.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lgv.nanxuanxn.top

Java: Collections.sort(list);  list.sort(null);
来源：http://yof.hcnkem.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ihm.fanxiaobao.xyz

Ruby: arr.sort
来源：http://ynv.dashuyun.cn

C#:   list.Sort();
来源：http://wmm.hfpthk.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://olv.cucudq.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hgx.bbcook.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kvb.havefunace.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://htj.sxryk.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xyg.zhiwuduotai.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://oat.kuanghao11.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://igk.xuanzx.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wtv.daria6918.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gim.snrcjt.cn

[D11] 反转数组
来源：http://woa.yanxiufei.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ane.hesvh.cn

PHP:  array_reverse($arr);
来源：http://tbm.ydjk.org.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://smp.zhiwuduotai.top

TS:   [...arr].reverse();
来源：http://deq.gogol.net.cn

Java: Collections.reverse(list);
来源：http://hsu.yuanzhike.top

Go:   slices.Reverse(arr)
来源：http://lhv.sweek.top

Ruby: arr.reverse
来源：http://gmz.vehdjk.com

C#:   list.Reverse();
来源：http://uez.zdqjudy.top

[D12] 查找元素下标
来源：http://hmf.sjlbkw.cn

Py:   arr.index(x);  x in arr
来源：http://xio.c1oappe.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wnj.bjfxy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://srv.yongpay.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gjv.xuanzx.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jrn.hongshengwenyu.top

Go:   slices.Index(arr, x)
来源：http://fuy.nanxuanxn.top

Ruby: arr.index(x)
来源：http://ole.tanke756.top

C#:   list.IndexOf(x);
来源：http://fuh.9152youxi.cn

[D13] 过滤（保留满足条件的）
来源：http://qcn.redwolf501.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qzt.yj20258.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://buv.redwolf501.top

JS:   arr.filter(x => x > 3)
来源：http://ptd.shuidangran.top

TS:   arr.filter(x => x > 3)
来源：http://zjd.xingfuxueyuan.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yxd.jqgufenzy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qel.zhoulong.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://jlu.zhaomingkeji.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://txb.sufxvd.cn

[D14] 映射转换（每个元素变形）
来源：http://akg.zycfv.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xrs.tarul.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://trg.redwolf501.top

JS:   arr.map(x => x * 2)
来源：http://cey.yanxiufei.cn

TS:   arr.map(x => x * 2)
来源：http://lft.redwolf501.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://stj.havefunace.top

Go:   // 手写循环
来源：http://amw.zhiwuduotai.top

Ruby: arr.map { |x| x * 2 }
来源：http://dpc.chenjidiqi.icu

C#:   list.Select(x => x * 2).ToList()
来源：http://lpb.epnwcf.com

[D15] 去重
来源：http://ylz.zhengqikj.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ujb.yj20258.top

PHP:  array_unique($arr);
来源：http://rvo.hnqzz.top

JS:   [...new Set(arr)]
来源：http://ilz.ywan-chungtsiang.top

TS:   [...new Set(arr)]
来源：http://xxv.chenlongwang.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cus.sysykeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://mot.vqdsnc.cn

Ruby: arr.uniq
来源：http://kol.havefunace.top

C#:   list.Distinct().ToList()
来源：http://trj.sxryk.cn

[D16] 求和与平均值
来源：http://qdp.hammf.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zuw.tian-w.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kem.mhx1999.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sww.vqdsnc.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ozy.shuidangran.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mzm.tian-w.cn

Go:   // 手写循环累加
来源：http://spl.hysaishi.cn


<!-- 参考信息 -->