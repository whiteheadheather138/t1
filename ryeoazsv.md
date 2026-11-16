代发 wailian999

Java: if (data == null) return;
来源：http://wpk.vehdjk.com

Go:   if data == nil { return }
来源：http://bwc.uphjek.com

Ruby: return if data.nil?
来源：http://xxi.guowangkeji.top

C#:   if (data == null) return;
来源：http://xyd.chenjidiqi.icu

================================================================================
来源：http://bun.tanke756.top

C. 函数与作用域
来源：http://aue.yfazqb.com

================================================================================
来源：http://vbd.zycfv.cn

[C01] 定义函数
来源：http://wby.shangyingyoupin.top

Py:   def add(a, b): return a + b
来源：http://pih.zycfv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zht.hcnkem.com

JS:   function add(a, b) { return a + b; }
来源：http://hzb.iojbl.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ueg.guannengcc.top

Java: static int add(int a, int b) { return a + b; }
来源：http://vsl.zhongyouzk.top

Go:   func add(a, b int) int { return a + b }
来源：http://ncr.yj202588.top

Ruby: def add(a, b); a + b; end
来源：http://ljy.kuanghao11.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://byg.pycfn.com

[C02] 默认参数
来源：http://ftr.wangshuangyany.cn

Py:   def greet(name="World"): return name
来源：http://dns.cashguo.top

PHP:  function greet($name = "World") { return $name; }
来源：http://aqe.tianlin.xyz

JS:   function greet(name = "World") { return name; }
来源：http://brs.epnwcf.com

TS:   function greet(name: string = "World") { return name; }
来源：http://vhe.gzhubu.top

Java: // 无默认参数：方法重载或 Optional
来源：http://zib.yvedp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dqs.dashuyun.cn

Ruby: def greet(name = "World") = name
来源：http://rhf.yonumen.top

C#:   string Greet(string name = "World") => name;
来源：http://akd.sxryk.cn

[C03] 可变参数
来源：http://ybk.sufxvd.cn

Py:   def total(*args): return sum(args)
来源：http://twf.shzxlz.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://znl.gogol.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sym.tanke756.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bkg.jlsjyb.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zgb.tianlin.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://del.hammf.cn

Ruby: def total(*nums); nums.sum; end
来源：http://esa.daria6918.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yaa.jianghu66.top

[C04] 命名参数 / 关键字参数
来源：http://lmm.yanxiufei.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zwi.shzxlz.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ibu.zhixingplan.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fvw.gotoacloud.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://obb.yongpay.top

Java: // 无：用 Builder 模式或 record
来源：http://pvh.hcnkem.com

Go:   // 无：用配置结构体参数
来源：http://ldz.gzhubu.top

Ruby: f(a: 1, b: 2)
来源：http://hdp.hnqzz.top

C#:   f(a: 1, b: 2)
来源：http://kct.jinyuanbaomall.cn

[C05] 返回多个值
来源：http://lgq.yj20258888.top

Py:   return a, b
来源：http://wjd.jinqigufen.top

PHP:  return [$a, $b];
来源：http://nqz.nanxuanxn.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://gmu.sweek.top

TS:   return { a, b };
来源：http://yav.zhixingplan.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ube.yuanzhike.top

Go:   return a, b
来源：http://qqr.zhixingplan.top

Ruby: return a, b
来源：http://urr.hammf.cn

C#:   return (a, b);              // ValueTuple
来源：http://qtl.pengpengdd.cyou

[C06] 匿名函数 / lambda
来源：http://pgj.52xcode.cn

Py:   square = lambda x: x * x
来源：http://iiu.nwbrower.top

PHP:  $square = fn($x) => $x * $x;
来源：http://oup.xingfuxueyuan.xyz

JS:   const square = x => x * x;
来源：http://hbs.sysykeji.top

TS:   const square = (x: number): number => x * x;
来源：http://vyh.xziqi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dxo.tian-w.cn

Go:   sq := func(x int) int { return x * x }
来源：http://pjj.hesvh.cn

Ruby: square = ->(x) { x * x }
来源：http://wwd.aizwys.cn

C#:   Func<int, int> square = x => x * x;
来源：http://uhu.quarkkingdee.top

[C07] 把函数作为参数传入
来源：http://cih.ctjpmb.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mvh.wangshuangyany.cn

PHP:  array_map("strtoupper", $arr);
来源：http://whr.hongshengwenyu.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xsq.ehwqpu.com

TS:   arr.map(String)
来源：http://vkb.ydjk.org.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bbu.yvedp.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://iga.hnxiangtu.top

Ruby: arr.map(&:upcase)
来源：http://hkh.hnqzz.top

C#:   arr.Select(s => s.ToUpper())
来源：http://nrq.zhiwuduotai.top

[C08] 闭包
来源：http://ynj.svipenyu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wxe.fehbvm.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ftt.jqgufenzy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ene.tian-w.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gtm.aizwys.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zkm.jinqigfzy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jlz.ctjpmb.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lgd.gaohongyu789.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://abw.hesvh.cn

[C09] 递归
来源：http://imz.wangdashe.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lsn.gogol.net.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://grk.ydjk.org.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cfb.dianchejie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mwt.ydjk.org.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ikl.ydjk.org.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qbt.hcnkem.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://iry.zhiwuduotai.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jyw.xziqi.cn

[C10] 变量作用域
来源：http://npm.hesvh.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://woj.ctjpmb.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nft.redwolf501.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kyf.hywenlv.cn

TS:   同 JS
来源：http://hxw.nanxuanxn.top

Java: 方法内为块级作用域
来源：http://qqm.shangyingyoupin.top

Go:   花括号块级作用域
来源：http://cgg.ybcxt.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bmw.gaohongyu789.top

C#:   块级作用域
来源：http://rjn.fehbvm.com

[C11] 模块导入与导出
来源：http://nem.nanxinkj.top

Py:   from module import func
来源：http://ssv.xuetiantiany.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://gbp.chenjidiqi.icu

JS:   export default function f() {};  import f from "./m.js";
来源：http://yan.gzhubu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://emq.xuanzx.com

Java: import java.util.List;
来源：http://zhg.hesvh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://csf.xinyue.icu

Ruby: require "json"; require_relative "./util"
来源：http://wqi.c1oappe.top

C#:   using System.Text;
来源：http://nbg.zdbjq.cn

[C12] 立即执行函数 IIFE
来源：http://yhc.wangdashe.top

Py:   (lambda: print("run"))()
来源：http://ksg.redwolf501.top

PHP:  (function () { echo "run"; })();
来源：http://snk.pycfn.com

JS:   (() => { console.log("run"); })();
来源：http://etx.xinyue.icu

TS:   (() => { console.log("run"); })();
来源：http://ojk.yj202588.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xiw.gogol.net.cn

Go:   func() { fmt.Println("run") }()
来源：http://wvy.nwbrower.top

Ruby: -> { puts "run" }.call
来源：http://fln.sxryk.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ald.ppjwa.cn

[C13] 类型声明 / 类型注解
来源：http://fdx.aibaodan.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bws.aizwys.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pwd.chenlongwang.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ybs.fengsongda.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://beh.dashuyun.cn

Java: int add(int a, int b) { return a + b; }
来源：http://urv.dashuyun.cn

Go:   func add(a, b int) int
来源：http://nnq.sysykeji.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nzc.epnwcf.com

C#:   int Add(int a, int b) => a + b;
来源：http://reu.ivvv.top

[C14] 泛型函数
来源：http://fxb.tarul.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hxk.52xcode.cn

PHP:  // 无泛型
来源：http://vwq.zhongyouzk.top

JS:   // 无泛型
来源：http://tic.hcnkem.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ssa.redwolf501.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://czo.xylfe.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hxy.316326.xyz

Ruby: # 无泛型
来源：http://nha.zhongyouzk.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fef.meibo888.top

[C15] 解构 / 展开参数
来源：http://bbd.xingfuxueyuan.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jjm.0kj1m.cn

PHP:  [$a, $b] = $pair;
来源：http://sdg.xuanzx.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gbw.ivvv.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zhj.ybcxt.top

Java: // 无解构
来源：http://nir.sysykeji.top

Go:   // 无解构
来源：http://iwz.chenjidiqi.icu

Ruby: a, b = pair
来源：http://get.hnxiangtu.top

C#:   var (a, b) = pair;
来源：http://bie.ywan-chungtsiang.top

[C16] 函数 / 方法重载
来源：http://ccp.316326.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ldt.xingfuxueyuan.xyz

PHP:  // 无重载
来源：http://wyf.nanxuanxn.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://rcm.fzhhl.top

TS:   // 用联合类型或重载签名声明
来源：http://qix.sweek.top

Java: void f(int a) {}  void f(String a) {}
来源：http://jxy.feifeiyinyue.top

Go:   // 无重载：用不同函数名
来源：http://dsn.mhx1999.top

Ruby: # 无重载：靠动态参数
来源：http://mnz.hnqzz.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://gfg.shuidangran.top

================================================================================
来源：http://dya.gogol.net.cn

D. 数组 / 列表 / 集合
来源：http://brf.yangfankeji.com

================================================================================
来源：http://dsu.shangyingyoupin.top

[D01] 创建数组 / 列表
来源：http://qaf.sweek.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://eae.kuanghao11.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://odu.aibaodan.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vjj.jqgfzy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://jis.hammf.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kom.mhx1999.top

Go:   arr := []int{1, 2, 3}
来源：http://ujs.chenzaomai.com

Ruby: arr = [1, 2, 3]
来源：http://kue.yueranfly.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vne.zhaomingkeji.xyz

[D02] 追加元素到末尾
来源：http://vjr.0kj1m.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gky.yj202588.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://thn.zhengqikj.top

JS:   arr.push(4);
来源：http://bps.chenzaomai.com

TS:   arr.push(4);
来源：http://eqx.yongpay.top

Java: list.add(4);
来源：http://zlz.nanxuanxn.top

Go:   arr = append(arr, 4)
来源：http://npj.wangshuangyany.cn

Ruby: arr << 4; arr.push(5)
来源：http://jlr.zhaomingkeji.xyz

C#:   list.Add(4);
来源：http://fgv.jlsjyb.cn

[D03] 在指定位置插入元素
来源：http://dds.jqgfzy.top

Py:   arr.insert(0, 0)
来源：http://won.ydzc1.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vzq.cheryme.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://eqf.hesvh.cn

TS:   arr.splice(0, 0, 0);
来源：http://cjy.chenzaomai.com

Java: list.add(0, 0);
来源：http://zeu.zdbjq.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fji.tian-w.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mnd.redwolf501.top

C#:   list.Insert(0, 0);
来源：http://tin.gzhubu.top

[D04] 删除元素
来源：http://nqd.fzhhl.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://aro.quarkkingdee.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vdj.pycfn.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hbq.chenzaomai.com

TS:   arr.splice(0, 1);
来源：http://ukh.tianlin.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://abj.gaohongyu789.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wgc.ctjpmb.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://soq.xuanzx.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://foc.daria6918.cn

[D05] 访问与修改元素
来源：http://lqi.zycfv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pur.yfazqb.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://npv.kuanghao11.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ane.hfpthk.cn

TS:   arr[0]; arr.at(-1);
来源：http://vhf.52xcode.cn

Java: list.get(0); list.set(0, 9);
来源：http://czo.jiagoushi.top

Go:   arr[0]; arr[0] = 9
来源：http://orb.tarul.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ufj.nanxuanxn.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nyh.tarul.cn

[D06] 数组长度
来源：http://dzy.cdnleiting.top

Py:   len(arr)
来源：http://ctf.aizwys.cn

PHP:  count($arr);
来源：http://rum.bjfxy.top

JS:   arr.length
来源：http://itx.quarkkingdee.top

TS:   arr.length
来源：http://gte.chenjidiqi.icu

Java: list.size();
来源：http://czj.xziqi.cn

Go:   len(arr)
来源：http://cqh.pengpengdd.cyou

Ruby: arr.length; arr.size
来源：http://fpv.ydzc1.top

C#:   list.Count;
来源：http://nsi.nwbrower.top

[D07] 切片 / 取子数组
来源：http://qnv.ppjwa.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tgd.cqqwz.cn

PHP:  array_slice($arr, 1, 3);
来源：http://dky.hongshengwenyu.top

JS:   arr.slice(1, 4);
来源：http://aqw.yanxiufei.cn

TS:   arr.slice(1, 4);
来源：http://iku.zdqjudy.top

Java: list.subList(1, 4);
来源：http://ryt.ydzc1.top

Go:   arr[1:4]
来源：http://xlg.svipenyu.cn

Ruby: arr[1, 3]
来源：http://mhu.yvedp.cn

C#:   list.GetRange(1, 3);
来源：http://pzr.yanxiufei.cn

[D08] 合并两个数组
来源：http://ozz.shanyushiyangtech.top

Py:   a + b;  a.extend(b)
来源：http://xxb.jinyuanbaomall.cn

PHP:  array_merge($a, $b);
来源：http://vbu.xinyue.icu

JS:   [...a, ...b];  a.concat(b);
来源：http://ovd.chenjidiqi.icu

TS:   [...a, ...b];
来源：http://cde.quarkkingdee.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://eke.aizwys.cn

Go:   append(a, b...)
来源：http://bys.hammf.cn

Ruby: a + b;  a.concat(b)
来源：http://wyg.dianchejie.cn

C#:   a.Concat(b).ToList()
来源：http://ubc.jlsjyb.cn

[D09] 排序（升序）
来源：http://aog.meibo888.top

Py:   sorted(arr);  arr.sort()
来源：http://acr.cdnleiting.top

PHP:  sort($arr);
来源：http://cdu.ivvv.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vyl.bbcook.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fhy.zhijiandao.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://msm.yj20258888.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qub.guowangkeji.top

Ruby: arr.sort
来源：http://wxu.zhixingplan.top

C#:   list.Sort();
来源：http://wkk.yj20258.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://oup.gzhubu.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://eiw.haohaochexian.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pos.wangshuangyany.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jpp.gaohongyu789.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rwo.aibaodan.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://foc.tarul.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mhf.tian-w.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lex.jiagoushi.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yui.xingfuxueyuan.xyz

[D11] 反转数组
来源：http://nlj.gzhubu.top

Py:   arr[::-1];  arr.reverse()
来源：http://qcm.zycfv.cn

PHP:  array_reverse($arr);
来源：http://cxr.zhoulong.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wpr.9152youxi.cn

TS:   [...arr].reverse();
来源：http://kud.0kj1m.cn

Java: Collections.reverse(list);
来源：http://vew.c1oappe.top

Go:   slices.Reverse(arr)
来源：http://uta.yfazqb.com

Ruby: arr.reverse
来源：http://tju.fehbvm.com

C#:   list.Reverse();
来源：http://ucc.aibaodan.cn

[D12] 查找元素下标
来源：http://uga.jianghu66.top

Py:   arr.index(x);  x in arr
来源：http://xms.shangyingyoupin.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sgg.chenlongwang.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wwf.hysaishi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jzv.shangyingyoupin.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://toy.zhaomingkeji.xyz

Go:   slices.Index(arr, x)
来源：http://nun.guannengcc.top

Ruby: arr.index(x)
来源：http://txu.iojbl.cn

C#:   list.IndexOf(x);
来源：http://dhu.yfazqb.com

[D13] 过滤（保留满足条件的）
来源：http://haz.yj20258888.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zpd.yanxiufei.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rlf.gogol.net.cn

JS:   arr.filter(x => x > 3)
来源：http://wap.jiagoushi.top

TS:   arr.filter(x => x > 3)
来源：http://rkx.fengsongda.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yut.andypj.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hma.uphjek.com

Ruby: arr.select { |x| x > 3 }
来源：http://wcf.gaohongyu789.top

C#:   list.Where(x => x > 3).ToList()
来源：http://sma.zdqjudy.top

[D14] 映射转换（每个元素变形）
来源：http://cwj.mhx1999.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wgt.cheryme.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yki.chenlongwang.top

JS:   arr.map(x => x * 2)
来源：http://fgd.jyoumei.cn

TS:   arr.map(x => x * 2)
来源：http://lon.xuetiantiany.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://cfl.chenlongwang.top

Go:   // 手写循环
来源：http://fcz.xuanzx.com

Ruby: arr.map { |x| x * 2 }
来源：http://rml.zhaomingkeji.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://nbo.xingfuxueyuan.xyz

[D15] 去重
来源：http://ehx.kuanghao11.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fkf.ywan-chungtsiang.top

PHP:  array_unique($arr);
来源：http://pws.andypj.xyz

JS:   [...new Set(arr)]
来源：http://xbn.bbcook.cn

TS:   [...new Set(arr)]
来源：http://usd.birdmap.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kcn.jqgufenzy.top

Go:   // 用 map[T]struct{} 手写
来源：http://cyo.cqqwz.cn

Ruby: arr.uniq
来源：http://wuv.hcnkem.com

C#:   list.Distinct().ToList()
来源：http://ikl.jianghu66.top

[D16] 求和与平均值
来源：http://afy.yangfankeji.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pkv.jyoumei.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vrj.sxryk.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gbz.chenlongwang.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zda.jinyuanbaomall.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kfa.jlsjyb.cn

Go:   // 手写循环累加
来源：http://xsm.sweek.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qic.tarul.cn

C#:   list.Sum();  list.Average()
来源：http://ysv.xinyue.icu

[D17] 最大值与最小值
来源：http://yws.wangdashe.top

Py:   max(arr);  min(arr)
来源：http://pcd.ctjpmb.com


<!-- 参考信息 -->