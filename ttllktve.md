代发 wailian999

Py:   def add(a, b): return a + b
来源：http://gfp.ehwqpu.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sdy.xuanzx.com

JS:   function add(a, b) { return a + b; }
来源：http://oef.chenlongwang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hbo.shzxlz.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://rem.dashuyun.cn

Go:   func add(a, b int) int { return a + b }
来源：http://joe.snrcjt.cn

Ruby: def add(a, b); a + b; end
来源：http://wfh.sweek.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dbs.snrcjt.cn

[C02] 默认参数
来源：http://cit.redwolf501.top

Py:   def greet(name="World"): return name
来源：http://nvh.xingfuxueyuan.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://rdc.epnwcf.com

JS:   function greet(name = "World") { return name; }
来源：http://qre.shangyingyoupin.top

TS:   function greet(name: string = "World") { return name; }
来源：http://eph.iojbl.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://eqn.gogol.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kyo.aibaodan.cn

Ruby: def greet(name = "World") = name
来源：http://dpg.tanke756.top

C#:   string Greet(string name = "World") => name;
来源：http://ibh.yueranfly.top

[C03] 可变参数
来源：http://zoq.cashguo.top

Py:   def total(*args): return sum(args)
来源：http://rhp.cheryme.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://iri.pengpengdd.cyou

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jiu.yj20258.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sef.jqgufenzy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xnl.shangyingyoupin.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://eem.mhx1999.top

Ruby: def total(*nums); nums.sum; end
来源：http://qmy.sysykeji.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bmx.xuanzx.com

[C04] 命名参数 / 关键字参数
来源：http://dpg.zhengqikj.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pnc.fktsv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bwn.zhoulong.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qvj.cqqwz.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ngf.vehdjk.com

Java: // 无：用 Builder 模式或 record
来源：http://szq.shuidangran.top

Go:   // 无：用配置结构体参数
来源：http://wzw.zhixingplan.top

Ruby: f(a: 1, b: 2)
来源：http://ihx.sweek.top

C#:   f(a: 1, b: 2)
来源：http://jaj.havefunace.top

[C05] 返回多个值
来源：http://sau.xuanzx.com

Py:   return a, b
来源：http://enp.9152youxi.cn

PHP:  return [$a, $b];
来源：http://bqk.havefunace.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://rtf.wangdashe.top

TS:   return { a, b };
来源：http://odl.tian-w.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sew.jinqigfzy.top

Go:   return a, b
来源：http://zrp.xingfuxueyuan.xyz

Ruby: return a, b
来源：http://swu.ydzc1.top

C#:   return (a, b);              // ValueTuple
来源：http://kmq.andypj.xyz

[C06] 匿名函数 / lambda
来源：http://ejh.shuidangran.top

Py:   square = lambda x: x * x
来源：http://qed.nanxuanxn.top

PHP:  $square = fn($x) => $x * $x;
来源：http://uvd.jinqigufen.top

JS:   const square = x => x * x;
来源：http://crh.xingfuxueyuan.xyz

TS:   const square = (x: number): number => x * x;
来源：http://sve.yongpay.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jbo.epnwcf.com

Go:   sq := func(x int) int { return x * x }
来源：http://nzr.ivvv.top

Ruby: square = ->(x) { x * x }
来源：http://fhx.yfazqb.com

C#:   Func<int, int> square = x => x * x;
来源：http://hwz.shanyushiyangkeji.top

[C07] 把函数作为参数传入
来源：http://raw.yj20258888.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rot.bjfxy.top

PHP:  array_map("strtoupper", $arr);
来源：http://psl.wangshuangyany.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zhx.xylfe.cn

TS:   arr.map(String)
来源：http://ufd.hysaishi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gax.jlsjyb.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nqv.yongpay.top

Ruby: arr.map(&:upcase)
来源：http://ilt.nanxuanxn.top

C#:   arr.Select(s => s.ToUpper())
来源：http://lyz.tianlin.xyz

[C08] 闭包
来源：http://xdz.yj20258.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wjl.yueranfly.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mmy.chenjidiqi.icu

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qhp.jinghuilouyu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bpo.jlsjyb.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ati.gogol.net.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zbv.fzhhl.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lbo.yj202588.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zie.shzxlz.cn

[C09] 递归
来源：http://epw.jinqigfzy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://buh.daxiang520.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://viy.9152youxi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vqa.vehdjk.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nqs.yvedp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://itx.feifeiyinyue.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sme.jiagoushi.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bii.shangyingyoupin.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qxp.hfpthk.cn

[C10] 变量作用域
来源：http://hck.zhaomingkeji.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qjo.52xcode.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pcu.0kj1m.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ckg.hfpthk.cn

TS:   同 JS
来源：http://jus.haohaochexian.top

Java: 方法内为块级作用域
来源：http://epp.uphjek.com

Go:   花括号块级作用域
来源：http://yhb.ctjpmb.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mdj.ppjwa.cn

C#:   块级作用域
来源：http://qve.wangdashe.top

[C11] 模块导入与导出
来源：http://ike.nanxinkj.top

Py:   from module import func
来源：http://owu.chenlongwang.top

PHP:  require "file.php";  或 use App\Service;
来源：http://qpr.nwbrower.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://hzq.birdmap.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://avk.hongshengwenyu.top

Java: import java.util.List;
来源：http://chc.zhaomingkeji.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://arx.sweek.top

Ruby: require "json"; require_relative "./util"
来源：http://uek.shuidangran.top

C#:   using System.Text;
来源：http://ckf.hnxiangtu.top

[C12] 立即执行函数 IIFE
来源：http://xge.jqgfzy.top

Py:   (lambda: print("run"))()
来源：http://jnq.uphjek.com

PHP:  (function () { echo "run"; })();
来源：http://xfh.hfpthk.cn

JS:   (() => { console.log("run"); })();
来源：http://alg.vqdsnc.cn

TS:   (() => { console.log("run"); })();
来源：http://mip.guowangkeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mqw.zhiwuduotai.top

Go:   func() { fmt.Println("run") }()
来源：http://blt.ivvv.top

Ruby: -> { puts "run" }.call
来源：http://yfq.epnwcf.com

C#:   // 无 IIFE：用静态构造函数
来源：http://qsw.cheryme.top

[C13] 类型声明 / 类型注解
来源：http://gjd.nwbrower.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fam.gzhubu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zho.xuetiantiany.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vnm.jinqigufen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wkl.tianlin.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://rkl.yongpay.top

Go:   func add(a, b int) int
来源：http://jgk.jinqigufen.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xso.daria6918.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mai.yj20258888.top

[C14] 泛型函数
来源：http://nod.xziqi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ciq.uphjek.com

PHP:  // 无泛型
来源：http://stb.ctjpmb.com

JS:   // 无泛型
来源：http://bqo.svipenyu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dyd.shzxlz.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://oro.yj20258.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fsq.zhengqikj.top

Ruby: # 无泛型
来源：http://urv.epnwcf.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fhx.ctjpmb.com

[C15] 解构 / 展开参数
来源：http://dkm.cdnleiting.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mbp.meibo888.top

PHP:  [$a, $b] = $pair;
来源：http://nwp.kuanghao11.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jaz.ivvv.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vlj.ydjk.org.cn

Java: // 无解构
来源：http://cyp.yuanzhike.top

Go:   // 无解构
来源：http://utj.smart0.xyz

Ruby: a, b = pair
来源：http://jwk.ppjwa.cn

C#:   var (a, b) = pair;
来源：http://xyt.jyoumei.cn

[C16] 函数 / 方法重载
来源：http://zft.tanke756.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bor.9152youxi.cn

PHP:  // 无重载
来源：http://gei.yongpay.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://xmw.hysaishi.cn

TS:   // 用联合类型或重载签名声明
来源：http://byu.gogol.net.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://bsp.quarkkingdee.top

Go:   // 无重载：用不同函数名
来源：http://yre.tianlin.xyz

Ruby: # 无重载：靠动态参数
来源：http://ihv.svipenyu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://dks.daria6918.cn

================================================================================
来源：http://kqi.xingfuxueyuan.xyz

D. 数组 / 列表 / 集合
来源：http://typ.shuidangran.top

================================================================================
来源：http://kfn.ivvv.top

[D01] 创建数组 / 列表
来源：http://rul.zhijiandao.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://tqo.jinghuilouyu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://eku.fktsv.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gdf.chenzaomai.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://txi.9152youxi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rie.fanxiaobao.xyz

Go:   arr := []int{1, 2, 3}
来源：http://ddd.redwolf501.top

Ruby: arr = [1, 2, 3]
来源：http://kyg.vehdjk.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ixz.yuxming.cn

[D02] 追加元素到末尾
来源：http://xsr.wangshuangyany.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://txi.zdbjq.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pjq.hnqzz.top

JS:   arr.push(4);
来源：http://qjb.fehbvm.com

TS:   arr.push(4);
来源：http://ijr.yj202588.top

Java: list.add(4);
来源：http://jmi.9152youxi.cn

Go:   arr = append(arr, 4)
来源：http://gtq.yfazqb.com

Ruby: arr << 4; arr.push(5)
来源：http://hcx.cucudq.cn

C#:   list.Add(4);
来源：http://prt.xziqi.cn

[D03] 在指定位置插入元素
来源：http://rsb.yj20258888.top

Py:   arr.insert(0, 0)
来源：http://nza.tarul.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mnp.fehbvm.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ixx.xuanzx.com

TS:   arr.splice(0, 0, 0);
来源：http://hti.jinyuanbaomall.cn

Java: list.add(0, 0);
来源：http://jto.fzhhl.top

Go:   arr = append([]int{0}, arr...)
来源：http://pxj.cqqwz.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wut.wangdashe.top

C#:   list.Insert(0, 0);
来源：http://yti.sweek.top

[D04] 删除元素
来源：http://ior.cqqwz.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bsn.chenlongwang.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://iur.iojbl.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ntw.nwbrower.top

TS:   arr.splice(0, 1);
来源：http://axa.c1oappe.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bwk.ydzc1.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sst.yueranfly.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ihr.daria6918.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tdy.yuxming.cn

[D05] 访问与修改元素
来源：http://ywf.yvedp.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ijv.zdqjudy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://osy.yuxming.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sdh.shanyushiyangkeji.top

TS:   arr[0]; arr.at(-1);
来源：http://nol.yj202588.top

Java: list.get(0); list.set(0, 9);
来源：http://dtp.quarkkingdee.top

Go:   arr[0]; arr[0] = 9
来源：http://ytb.yj202588.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mtw.jinqigufen.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uzv.gotoacloud.top

[D06] 数组长度
来源：http://rpw.xylfe.cn

Py:   len(arr)
来源：http://csf.ydjk.org.cn

PHP:  count($arr);
来源：http://alo.haohaochexian.top

JS:   arr.length
来源：http://ksc.gogol.net.cn

TS:   arr.length
来源：http://bfc.xuetiantiany.cn

Java: list.size();
来源：http://mfe.kuanghao11.cn

Go:   len(arr)
来源：http://xbt.dianchejie.cn

Ruby: arr.length; arr.size
来源：http://ssy.yongpay.top

C#:   list.Count;
来源：http://syq.zdbjq.cn

[D07] 切片 / 取子数组
来源：http://jwh.jyoumei.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xqa.iojbl.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hjt.mhx1999.top

JS:   arr.slice(1, 4);
来源：http://xcs.ydjk.org.cn

TS:   arr.slice(1, 4);
来源：http://koj.jinyuanbaomall.cn

Java: list.subList(1, 4);
来源：http://ifz.shuidangran.top

Go:   arr[1:4]
来源：http://yew.yuxming.cn

Ruby: arr[1, 3]
来源：http://ipk.zhoulong.xyz

C#:   list.GetRange(1, 3);
来源：http://bxv.sjlbkw.cn

[D08] 合并两个数组
来源：http://pya.xingfuxueyuan.xyz

Py:   a + b;  a.extend(b)
来源：http://puc.yvedp.cn

PHP:  array_merge($a, $b);
来源：http://had.zhixingplan.top

JS:   [...a, ...b];  a.concat(b);
来源：http://dfz.gzhubu.top

TS:   [...a, ...b];
来源：http://eap.jinqigufen.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xab.epnwcf.com

Go:   append(a, b...)
来源：http://lej.hongshengwenyu.top

Ruby: a + b;  a.concat(b)
来源：http://wvy.fzhhl.top

C#:   a.Concat(b).ToList()
来源：http://sxj.nwbrower.top

[D09] 排序（升序）
来源：http://efx.hywenlv.cn

Py:   sorted(arr);  arr.sort()
来源：http://ytz.zycfv.cn

PHP:  sort($arr);
来源：http://lxw.jqgfzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zmi.wangdashe.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://mzp.ehwqpu.com

Java: Collections.sort(list);  list.sort(null);
来源：http://xeo.shangyingyoupin.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lks.0kj1m.cn

Ruby: arr.sort
来源：http://hgm.bjfxy.top

C#:   list.Sort();
来源：http://jyk.yanxiufei.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rut.zdqjudy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ibr.smart0.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sqv.ctjpmb.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ltv.yangfankeji.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qia.fzhhl.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jfl.iojbl.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jub.yuanzhike.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://eim.vehdjk.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jtw.ppjwa.cn

[D11] 反转数组
来源：http://vep.yuxming.cn

Py:   arr[::-1];  arr.reverse()
来源：http://nig.cucudq.cn

PHP:  array_reverse($arr);
来源：http://cab.dianchejie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xtz.tanke756.top

TS:   [...arr].reverse();
来源：http://zez.jianghu66.top

Java: Collections.reverse(list);
来源：http://lim.iojbl.cn

Go:   slices.Reverse(arr)
来源：http://wbh.hongshengwenyu.top

Ruby: arr.reverse
来源：http://sdr.nanxinkj.top

C#:   list.Reverse();
来源：http://qrp.shuidangran.top

[D12] 查找元素下标
来源：http://wgx.jianghu66.top

Py:   arr.index(x);  x in arr
来源：http://xod.cucudq.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vdu.xingfuxueyuan.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vie.andypj.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wzb.vehdjk.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yzq.guannengcc.top

Go:   slices.Index(arr, x)
来源：http://pen.zhijiandao.cn

Ruby: arr.index(x)
来源：http://apt.ywan-chungtsiang.top

C#:   list.IndexOf(x);
来源：http://imu.zdqjudy.top

[D13] 过滤（保留满足条件的）
来源：http://grn.gaohongyu789.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xsj.fehbvm.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ucg.9152youxi.cn

JS:   arr.filter(x => x > 3)
来源：http://ltz.aizwys.cn

TS:   arr.filter(x => x > 3)
来源：http://ilj.hywenlv.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ayp.hfpthk.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bwz.ybcxt.top

Ruby: arr.select { |x| x > 3 }
来源：http://bxh.yongpay.top

C#:   list.Where(x => x > 3).ToList()
来源：http://jer.zhixingplan.top

[D14] 映射转换（每个元素变形）
来源：http://nyv.aizwys.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yri.andypj.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://aog.52xcode.cn

JS:   arr.map(x => x * 2)
来源：http://rmd.chenjidiqi.icu

TS:   arr.map(x => x * 2)
来源：http://bou.ctjpmb.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://hrq.hesvh.cn

Go:   // 手写循环
来源：http://vlw.0kj1m.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qml.zhixingplan.top

C#:   list.Select(x => x * 2).ToList()
来源：http://eox.chenzaomai.com

[D15] 去重
来源：http://idp.yangfankeji.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pyz.fehbvm.com

PHP:  array_unique($arr);
来源：http://fvf.shzxlz.cn

JS:   [...new Set(arr)]
来源：http://iqk.tanke756.top

TS:   [...new Set(arr)]
来源：http://klp.jianghu66.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://myf.cashguo.top

Go:   // 用 map[T]struct{} 手写
来源：http://vom.cashguo.top

Ruby: arr.uniq
来源：http://vjt.zhoulong.xyz

C#:   list.Distinct().ToList()
来源：http://yfa.xziqi.cn

[D16] 求和与平均值
来源：http://lqw.xingfuxueyuan.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hru.cashguo.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kdj.sxryk.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cqc.hnqzz.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mfw.zhoulong.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://igr.sxryk.cn

Go:   // 手写循环累加
来源：http://bmz.yvedp.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rzq.sufxvd.cn

C#:   list.Sum();  list.Average()
来源：http://vmm.zycfv.cn

[D17] 最大值与最小值
来源：http://tbi.jyoumei.cn

Py:   max(arr);  min(arr)
来源：http://llm.hysaishi.cn

PHP:  max($arr);  min($arr);
来源：http://yyn.pycfn.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jcc.xinyue.icu

TS:   Math.max(...arr);
来源：http://jqf.ctjpmb.com

Java: Collections.max(list);  Collections.min(list);
来源：http://ztu.pycfn.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gfy.yj20258888.top

Ruby: arr.max;  arr.min
来源：http://dfq.ppjwa.cn

C#:   list.Max();  list.Min()
来源：http://mhf.xuanzx.com

[D18] 扁平化嵌套数组
来源：http://gdu.gzhubu.top


<!-- 参考信息 -->