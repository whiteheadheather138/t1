代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://miz.pengpengdd.cyou

Go:   func add(a, b int) int { return a + b }
来源：http://jee.zhengqikj.top

Ruby: def add(a, b); a + b; end
来源：http://evs.feifeiyinyue.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wsm.xylfe.cn

[C02] 默认参数
来源：http://oko.yj202588.top

Py:   def greet(name="World"): return name
来源：http://vwf.ybcxt.top

PHP:  function greet($name = "World") { return $name; }
来源：http://nsz.zhixingplan.top

JS:   function greet(name = "World") { return name; }
来源：http://jwf.vehdjk.com

TS:   function greet(name: string = "World") { return name; }
来源：http://xkt.zdqjudy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://rar.hywenlv.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vfj.zdbjq.cn

Ruby: def greet(name = "World") = name
来源：http://can.yuxming.cn

C#:   string Greet(string name = "World") => name;
来源：http://luz.jinqigufen.top

[C03] 可变参数
来源：http://gsv.yongpay.top

Py:   def total(*args): return sum(args)
来源：http://xci.dashuyun.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uoj.wangshuangyany.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qkm.mhx1999.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vvq.pengpengdd.cyou

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rqg.52xcode.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://szc.sweek.top

Ruby: def total(*nums); nums.sum; end
来源：http://aar.tanke756.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zal.jianghu66.top

[C04] 命名参数 / 关键字参数
来源：http://hsc.hesvh.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://epi.xylfe.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ohu.sweek.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kqg.yuxming.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qby.daria6918.cn

Java: // 无：用 Builder 模式或 record
来源：http://fai.jiagoushi.top

Go:   // 无：用配置结构体参数
来源：http://xiw.sjlbkw.cn

Ruby: f(a: 1, b: 2)
来源：http://abe.tarul.cn

C#:   f(a: 1, b: 2)
来源：http://ftg.ctjpmb.com

[C05] 返回多个值
来源：http://lgp.daxiang520.top

Py:   return a, b
来源：http://izw.jlsjyb.cn

PHP:  return [$a, $b];
来源：http://xyt.zycfv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://mau.tian-w.cn

TS:   return { a, b };
来源：http://ujy.guannengcc.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://oen.mhx1999.top

Go:   return a, b
来源：http://rfo.hywenlv.cn

Ruby: return a, b
来源：http://qnm.xuanzx.com

C#:   return (a, b);              // ValueTuple
来源：http://teq.yj20258.top

[C06] 匿名函数 / lambda
来源：http://jif.gzhubu.top

Py:   square = lambda x: x * x
来源：http://ddk.iojbl.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://mhf.xziqi.cn

JS:   const square = x => x * x;
来源：http://wsq.9152youxi.cn

TS:   const square = (x: number): number => x * x;
来源：http://xpv.iojbl.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ism.smart0.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://uoy.pycfn.com

Ruby: square = ->(x) { x * x }
来源：http://xor.yongpay.top

C#:   Func<int, int> square = x => x * x;
来源：http://yjh.yangfankeji.com

[C07] 把函数作为参数传入
来源：http://tqc.jinghuilouyu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jpw.316326.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://hbv.andypj.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mgo.tianlin.xyz

TS:   arr.map(String)
来源：http://edb.fzhhl.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://aeq.zhaomingkeji.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://aaw.ydjk.org.cn

Ruby: arr.map(&:upcase)
来源：http://lsy.chenzaomai.com

C#:   arr.Select(s => s.ToUpper())
来源：http://kxe.aibaodan.cn

[C08] 闭包
来源：http://cpi.ybcxt.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tid.svipenyu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ywe.fehbvm.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lqo.fengsongda.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vgn.smart0.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ouj.aizwys.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zrd.shanyushiyangkeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cfc.vqdsnc.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qge.feifeiyinyue.top

[C09] 递归
来源：http://uml.zhoulong.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://shb.zhengqikj.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jvb.quarkkingdee.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eno.andypj.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qbh.yvedp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qhl.tarul.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://eiw.zhijiandao.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cms.jyoumei.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pmp.0kj1m.cn

[C10] 变量作用域
来源：http://tdg.xinyue.icu

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://acz.zhaomingkeji.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kbf.aibaodan.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nlx.iojbl.cn

TS:   同 JS
来源：http://pha.gzhubu.top

Java: 方法内为块级作用域
来源：http://wrs.hammf.cn

Go:   花括号块级作用域
来源：http://jii.svipenyu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jom.pengpengdd.cyou

C#:   块级作用域
来源：http://sso.fzhhl.top

[C11] 模块导入与导出
来源：http://jsx.ybcxt.top

Py:   from module import func
来源：http://cik.sufxvd.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kly.jiagoushi.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://rhu.tarul.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://czn.jinqigfzy.top

Java: import java.util.List;
来源：http://nzi.havefunace.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hlg.nanxuanxn.top

Ruby: require "json"; require_relative "./util"
来源：http://eaa.pycfn.com

C#:   using System.Text;
来源：http://bqi.zdqjudy.top

[C12] 立即执行函数 IIFE
来源：http://heb.ydzc1.top

Py:   (lambda: print("run"))()
来源：http://ual.zhixingplan.top

PHP:  (function () { echo "run"; })();
来源：http://edu.guowangkeji.top

JS:   (() => { console.log("run"); })();
来源：http://orr.52xcode.cn

TS:   (() => { console.log("run"); })();
来源：http://gen.chenzaomai.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://aow.zhongyouzk.top

Go:   func() { fmt.Println("run") }()
来源：http://bru.chenlongwang.top

Ruby: -> { puts "run" }.call
来源：http://qmn.zhijiandao.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gtd.yj20258888.top

[C13] 类型声明 / 类型注解
来源：http://rwc.yangfankeji.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wxk.cashguo.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mpb.hnqzz.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ash.svipenyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xzp.xuetiantiany.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jnv.hfpthk.cn

Go:   func add(a, b int) int
来源：http://fnv.ivvv.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zdt.sysykeji.top

C#:   int Add(int a, int b) => a + b;
来源：http://ddo.ppjwa.cn

[C14] 泛型函数
来源：http://wos.shzxlz.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mge.316326.xyz

PHP:  // 无泛型
来源：http://bgi.aizwys.cn

JS:   // 无泛型
来源：http://pfx.jinyuanbaomall.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pyw.ivvv.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ems.hammf.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://saj.yj202588.top

Ruby: # 无泛型
来源：http://bdh.cqqwz.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fbf.zhaomingkeji.xyz

[C15] 解构 / 展开参数
来源：http://tbc.nanxinkj.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ded.shzxlz.cn

PHP:  [$a, $b] = $pair;
来源：http://thk.ehwqpu.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://trs.shuidangran.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xpn.hfpthk.cn

Java: // 无解构
来源：http://dls.ydzc1.top

Go:   // 无解构
来源：http://ksf.yj20258888.top

Ruby: a, b = pair
来源：http://vzg.zdqjudy.top

C#:   var (a, b) = pair;
来源：http://zue.guowangkeji.top

[C16] 函数 / 方法重载
来源：http://sci.jyoumei.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://enn.jianghu66.top

PHP:  // 无重载
来源：http://tyj.sysykeji.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://uce.ybcxt.top

TS:   // 用联合类型或重载签名声明
来源：http://eeh.jqgfzy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://imp.quarkkingdee.top

Go:   // 无重载：用不同函数名
来源：http://hbm.hnqzz.top

Ruby: # 无重载：靠动态参数
来源：http://ozo.shangyingyoupin.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://upm.xuetiantiany.cn

================================================================================
来源：http://rdv.pycfn.com

D. 数组 / 列表 / 集合
来源：http://tle.xingfuxueyuan.xyz

================================================================================
来源：http://xdt.xinyue.icu

[D01] 创建数组 / 列表
来源：http://fgp.smart0.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://xbh.xuanzx.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jdv.gogol.net.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://snc.hfpthk.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yrc.wangshuangyany.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zpr.jinqigfzy.top

Go:   arr := []int{1, 2, 3}
来源：http://rmz.nanxinkj.top

Ruby: arr = [1, 2, 3]
来源：http://mdo.svipenyu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zzd.zhaomingkeji.xyz

[D02] 追加元素到末尾
来源：http://owk.dianchejie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://apy.cdnleiting.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mod.xziqi.cn

JS:   arr.push(4);
来源：http://riy.yanxiufei.cn

TS:   arr.push(4);
来源：http://ten.yuxming.cn

Java: list.add(4);
来源：http://fqm.tianlin.xyz

Go:   arr = append(arr, 4)
来源：http://nyq.316326.xyz

Ruby: arr << 4; arr.push(5)
来源：http://wox.birdmap.top

C#:   list.Add(4);
来源：http://bxx.dianchejie.cn

[D03] 在指定位置插入元素
来源：http://wew.redwolf501.top

Py:   arr.insert(0, 0)
来源：http://tax.jyoumei.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zxm.zhijiandao.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mlt.uphjek.com

TS:   arr.splice(0, 0, 0);
来源：http://ips.hnqzz.top

Java: list.add(0, 0);
来源：http://nkw.yanxiufei.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hyz.jianghu66.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uky.tianlin.xyz

C#:   list.Insert(0, 0);
来源：http://rqv.jyoumei.cn

[D04] 删除元素
来源：http://nis.xuanzx.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nhx.sysykeji.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cey.zhoulong.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://swr.daxiang520.top

TS:   arr.splice(0, 1);
来源：http://pmg.tarul.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xfe.epnwcf.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jds.guowangkeji.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xhx.redwolf501.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hob.yj202588.top

[D05] 访问与修改元素
来源：http://dnc.vehdjk.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sxm.zdbjq.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jkx.snrcjt.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://suv.sufxvd.cn

TS:   arr[0]; arr.at(-1);
来源：http://qkb.zhengqikj.top

Java: list.get(0); list.set(0, 9);
来源：http://nri.kuanghao11.cn

Go:   arr[0]; arr[0] = 9
来源：http://hem.aibaodan.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qvj.haohaochexian.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ief.yvedp.cn

[D06] 数组长度
来源：http://zpt.cashguo.top

Py:   len(arr)
来源：http://yuf.hammf.cn

PHP:  count($arr);
来源：http://nhs.hesvh.cn

JS:   arr.length
来源：http://ypa.havefunace.top

TS:   arr.length
来源：http://wir.hywenlv.cn

Java: list.size();
来源：http://rem.ivvv.top

Go:   len(arr)
来源：http://uwq.yuanzhike.top

Ruby: arr.length; arr.size
来源：http://pan.jinyuanbaomall.cn

C#:   list.Count;
来源：http://mwr.jinqigfzy.top

[D07] 切片 / 取子数组
来源：http://jlh.ctjpmb.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cdi.zycfv.cn

PHP:  array_slice($arr, 1, 3);
来源：http://dzy.tian-w.cn

JS:   arr.slice(1, 4);
来源：http://avu.epnwcf.com

TS:   arr.slice(1, 4);
来源：http://rzi.shuidangran.top

Java: list.subList(1, 4);
来源：http://bfn.c1oappe.top

Go:   arr[1:4]
来源：http://uvu.tian-w.cn

Ruby: arr[1, 3]
来源：http://cem.xingfuxueyuan.xyz

C#:   list.GetRange(1, 3);
来源：http://nnl.zdqjudy.top

[D08] 合并两个数组
来源：http://vnt.zhaomingkeji.xyz

Py:   a + b;  a.extend(b)
来源：http://enr.nanxuanxn.top

PHP:  array_merge($a, $b);
来源：http://aov.xingfuxueyuan.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://vis.hfpthk.cn

TS:   [...a, ...b];
来源：http://luv.hesvh.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cdk.jqgufenzy.top

Go:   append(a, b...)
来源：http://bcd.yj20258.top

Ruby: a + b;  a.concat(b)
来源：http://ldx.pycfn.com

C#:   a.Concat(b).ToList()
来源：http://xls.wangdashe.top

[D09] 排序（升序）
来源：http://jct.uphjek.com

Py:   sorted(arr);  arr.sort()
来源：http://lhe.jlsjyb.cn

PHP:  sort($arr);
来源：http://lel.yongpay.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kng.ydjk.org.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://poq.zdqjudy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://xqg.svipenyu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://def.fehbvm.com

Ruby: arr.sort
来源：http://qmc.mhx1999.top

C#:   list.Sort();
来源：http://roj.havefunace.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://tum.zhijiandao.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://scc.yangfankeji.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rtu.316326.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wnv.shzxlz.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vfh.aizwys.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pbp.jinqigfzy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xfo.jinqigufen.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kuz.hnxiangtu.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yxv.jqgufenzy.top

[D11] 反转数组
来源：http://cub.shanyushiyangkeji.top

Py:   arr[::-1];  arr.reverse()
来源：http://fft.shanyushiyangkeji.top

PHP:  array_reverse($arr);
来源：http://cur.dianchejie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fqf.fzhhl.top

TS:   [...arr].reverse();
来源：http://odm.guowangkeji.top

Java: Collections.reverse(list);
来源：http://yvl.zhengqikj.top

Go:   slices.Reverse(arr)
来源：http://zef.ctjpmb.com

Ruby: arr.reverse
来源：http://faj.nanxuanxn.top

C#:   list.Reverse();
来源：http://hsj.tarul.cn

[D12] 查找元素下标
来源：http://fac.pengpengdd.cyou

Py:   arr.index(x);  x in arr
来源：http://kqp.ybcxt.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wzm.bjfxy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://etk.yj202588.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pds.shangyingyoupin.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://byj.zdbjq.cn

Go:   slices.Index(arr, x)
来源：http://css.jinghuilouyu.cn

Ruby: arr.index(x)
来源：http://txn.gogol.net.cn

C#:   list.IndexOf(x);
来源：http://qxn.52xcode.cn

[D13] 过滤（保留满足条件的）
来源：http://iwh.jinghuilouyu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wlg.jyoumei.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vpv.yonumen.top

JS:   arr.filter(x => x > 3)
来源：http://rrt.shzxlz.cn

TS:   arr.filter(x => x > 3)
来源：http://fqq.haohaochexian.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ftn.yfazqb.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://asv.jianghu66.top

Ruby: arr.select { |x| x > 3 }
来源：http://wqi.sweek.top

C#:   list.Where(x => x > 3).ToList()
来源：http://tvo.redwolf501.top

[D14] 映射转换（每个元素变形）
来源：http://uty.bbcook.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cem.yangfankeji.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cnb.ydjk.org.cn

JS:   arr.map(x => x * 2)
来源：http://wcz.chenjidiqi.icu

TS:   arr.map(x => x * 2)
来源：http://mbb.daxiang520.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://yzj.haohaochexian.top

Go:   // 手写循环
来源：http://ttk.mhx1999.top

Ruby: arr.map { |x| x * 2 }
来源：http://foy.shuidangran.top

C#:   list.Select(x => x * 2).ToList()
来源：http://goe.zhixingplan.top

[D15] 去重
来源：http://fuq.gogol.net.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mej.52xcode.cn

PHP:  array_unique($arr);
来源：http://wjp.pycfn.com

JS:   [...new Set(arr)]
来源：http://xrj.zdbjq.cn

TS:   [...new Set(arr)]
来源：http://wvh.hcnkem.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mzm.shanyushiyangtech.top

Go:   // 用 map[T]struct{} 手写
来源：http://lbt.hnxiangtu.top

Ruby: arr.uniq
来源：http://tho.yuanzhike.top

C#:   list.Distinct().ToList()
来源：http://icx.jinqigfzy.top

[D16] 求和与平均值
来源：http://wsj.jinqigufen.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://igm.meibo888.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pwf.pycfn.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vog.havefunace.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://awp.pengpengdd.cyou

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kjy.haohaochexian.top

Go:   // 手写循环累加
来源：http://nsv.aibaodan.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dtb.chenlongwang.top

C#:   list.Sum();  list.Average()
来源：http://bge.daxiang520.top

[D17] 最大值与最小值
来源：http://rca.shanyushiyangtech.top

Py:   max(arr);  min(arr)
来源：http://zkd.nwbrower.top

PHP:  max($arr);  min($arr);
来源：http://rlu.jqgfzy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cdc.havefunace.top

TS:   Math.max(...arr);
来源：http://tkv.yonumen.top

Java: Collections.max(list);  Collections.min(list);
来源：http://eru.zhijiandao.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pnp.bbcook.cn

Ruby: arr.max;  arr.min
来源：http://mkl.tian-w.cn

C#:   list.Max();  list.Min()
来源：http://szv.jinyuanbaomall.cn

[D18] 扁平化嵌套数组
来源：http://kgx.chenzaomai.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bzw.hnxiangtu.top

PHP:  array_merge(...$nested);
来源：http://rwr.9152youxi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://enn.cqqwz.cn

TS:   nested.flat();
来源：http://woc.jinyuanbaomall.cn


<!-- 参考信息 -->