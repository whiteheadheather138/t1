代发 wailian999

================================================================================
来源：http://jqt.epnwcf.com

C. 函数与作用域
来源：http://bfw.yanxiufei.cn

================================================================================
来源：http://vaj.jyoumei.cn

[C01] 定义函数
来源：http://krn.bbcook.cn

Py:   def add(a, b): return a + b
来源：http://fln.yonumen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hjf.mhx1999.top

JS:   function add(a, b) { return a + b; }
来源：http://ydi.nwbrower.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iqv.vqdsnc.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ena.iojbl.cn

Go:   func add(a, b int) int { return a + b }
来源：http://aqh.chenlongwang.top

Ruby: def add(a, b); a + b; end
来源：http://zdj.zhiwuduotai.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xzx.tianlin.xyz

[C02] 默认参数
来源：http://pmc.iojbl.cn

Py:   def greet(name="World"): return name
来源：http://sfe.xziqi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://nac.yvedp.cn

JS:   function greet(name = "World") { return name; }
来源：http://hcl.fktsv.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cru.yangfankeji.com

Java: // 无默认参数：方法重载或 Optional
来源：http://jjb.cdnleiting.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cto.cucudq.cn

Ruby: def greet(name = "World") = name
来源：http://cdl.yongpay.top

C#:   string Greet(string name = "World") => name;
来源：http://wyh.yueranfly.top

[C03] 可变参数
来源：http://bhg.cucudq.cn

Py:   def total(*args): return sum(args)
来源：http://pyp.cheryme.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yhe.cucudq.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mbp.svipenyu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kop.shzxlz.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://irh.guannengcc.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://aeg.iojbl.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tjw.jinqigfzy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hos.jinqigfzy.top

[C04] 命名参数 / 关键字参数
来源：http://spn.gotoacloud.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ibq.smart0.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://suc.mhx1999.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mfh.cashguo.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rrr.zhengqikj.top

Java: // 无：用 Builder 模式或 record
来源：http://cik.ivvv.top

Go:   // 无：用配置结构体参数
来源：http://kxd.zdbjq.cn

Ruby: f(a: 1, b: 2)
来源：http://nvx.yj20258.top

C#:   f(a: 1, b: 2)
来源：http://anb.nwbrower.top

[C05] 返回多个值
来源：http://pae.yj202588.top

Py:   return a, b
来源：http://xlh.ydjk.org.cn

PHP:  return [$a, $b];
来源：http://igh.c1oappe.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://tvv.chenzaomai.com

TS:   return { a, b };
来源：http://lyr.hywenlv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zao.shangyingyoupin.top

Go:   return a, b
来源：http://dvl.gotoacloud.top

Ruby: return a, b
来源：http://dub.cheryme.top

C#:   return (a, b);              // ValueTuple
来源：http://jrg.aizwys.cn

[C06] 匿名函数 / lambda
来源：http://whv.zhaomingkeji.xyz

Py:   square = lambda x: x * x
来源：http://jul.hywenlv.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://kyy.hesvh.cn

JS:   const square = x => x * x;
来源：http://err.hesvh.cn

TS:   const square = (x: number): number => x * x;
来源：http://ugy.ybcxt.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rnd.jqgufenzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://dff.gogol.net.cn

Ruby: square = ->(x) { x * x }
来源：http://vwq.zhongyouzk.top

C#:   Func<int, int> square = x => x * x;
来源：http://wwr.quarkkingdee.top

[C07] 把函数作为参数传入
来源：http://anp.xylfe.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mnt.chenlongwang.top

PHP:  array_map("strtoupper", $arr);
来源：http://ovi.xziqi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://htr.zdbjq.cn

TS:   arr.map(String)
来源：http://iyk.mhx1999.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jih.xuanzx.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jcd.52xcode.cn

Ruby: arr.map(&:upcase)
来源：http://rym.epnwcf.com

C#:   arr.Select(s => s.ToUpper())
来源：http://zzn.cucudq.cn

[C08] 闭包
来源：http://esw.52xcode.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ypv.tianlin.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nkc.havefunace.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jmw.cheryme.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bie.yuxming.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qkw.zdbjq.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ofo.yongpay.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jnx.nwbrower.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ndp.316326.xyz

[C09] 递归
来源：http://vtz.shanyushiyangkeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wao.pycfn.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sxm.sysykeji.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://foy.sufxvd.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qpz.hnxiangtu.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bog.wangdashe.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kbp.chenzaomai.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rqg.tianlin.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mjp.aibaodan.cn

[C10] 变量作用域
来源：http://clf.zhiwuduotai.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wyx.zhengqikj.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nno.jyoumei.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://llq.sxryk.cn

TS:   同 JS
来源：http://ovl.dianchejie.cn

Java: 方法内为块级作用域
来源：http://enj.aibaodan.cn

Go:   花括号块级作用域
来源：http://bkm.yongpay.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kra.tian-w.cn

C#:   块级作用域
来源：http://ypn.cheryme.top

[C11] 模块导入与导出
来源：http://ahf.jinghuilouyu.cn

Py:   from module import func
来源：http://uow.shanyushiyangtech.top

PHP:  require "file.php";  或 use App\Service;
来源：http://qsn.hnxiangtu.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://fkn.xziqi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gpj.epnwcf.com

Java: import java.util.List;
来源：http://hbl.cashguo.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bax.kuanghao11.cn

Ruby: require "json"; require_relative "./util"
来源：http://vpf.smart0.xyz

C#:   using System.Text;
来源：http://okr.pengpengdd.cyou

[C12] 立即执行函数 IIFE
来源：http://uhm.yvedp.cn

Py:   (lambda: print("run"))()
来源：http://gph.quarkkingdee.top

PHP:  (function () { echo "run"; })();
来源：http://rvp.zdbjq.cn

JS:   (() => { console.log("run"); })();
来源：http://xaz.aizwys.cn

TS:   (() => { console.log("run"); })();
来源：http://inl.guowangkeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://slk.shangyingyoupin.top

Go:   func() { fmt.Println("run") }()
来源：http://xyj.quarkkingdee.top

Ruby: -> { puts "run" }.call
来源：http://xck.cqqwz.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://cnu.zdbjq.cn

[C13] 类型声明 / 类型注解
来源：http://qnl.bbcook.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://byh.fzhhl.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ihy.guowangkeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ngl.aibaodan.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wid.fehbvm.com

Java: int add(int a, int b) { return a + b; }
来源：http://tcm.zdbjq.cn

Go:   func add(a, b int) int
来源：http://wua.shangyingyoupin.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://odb.shanyushiyangtech.top

C#:   int Add(int a, int b) => a + b;
来源：http://iyl.jlsjyb.cn

[C14] 泛型函数
来源：http://nxy.xylfe.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sel.0kj1m.cn

PHP:  // 无泛型
来源：http://ktm.ctjpmb.com

JS:   // 无泛型
来源：http://hal.vehdjk.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rth.meibo888.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vmh.smart0.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kfb.nanxuanxn.top

Ruby: # 无泛型
来源：http://oxi.aizwys.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wze.zhaomingkeji.xyz

[C15] 解构 / 展开参数
来源：http://vrr.yangfankeji.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jga.52xcode.cn

PHP:  [$a, $b] = $pair;
来源：http://axo.cheryme.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jkj.chenlongwang.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xou.hammf.cn

Java: // 无解构
来源：http://ted.jianghu66.top

Go:   // 无解构
来源：http://bdp.xylfe.cn

Ruby: a, b = pair
来源：http://wpy.jinqigfzy.top

C#:   var (a, b) = pair;
来源：http://zvb.cdnleiting.top

[C16] 函数 / 方法重载
来源：http://xjw.zhaomingkeji.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://war.ybcxt.top

PHP:  // 无重载
来源：http://nhe.birdmap.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://dqt.vqdsnc.cn

TS:   // 用联合类型或重载签名声明
来源：http://vsk.xingfuxueyuan.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://wdd.tianlin.xyz

Go:   // 无重载：用不同函数名
来源：http://tyl.hammf.cn

Ruby: # 无重载：靠动态参数
来源：http://boy.guowangkeji.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://yer.jqgufenzy.top

================================================================================
来源：http://hyi.zdqjudy.top

D. 数组 / 列表 / 集合
来源：http://ave.aibaodan.cn

================================================================================
来源：http://nkz.316326.xyz

[D01] 创建数组 / 列表
来源：http://doy.fktsv.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pfc.redwolf501.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ihf.redwolf501.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gam.tanke756.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://rah.dianchejie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://usi.yj20258888.top

Go:   arr := []int{1, 2, 3}
来源：http://wal.havefunace.top

Ruby: arr = [1, 2, 3]
来源：http://tii.zhoulong.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jol.zhaomingkeji.xyz

[D02] 追加元素到末尾
来源：http://lhj.cdnleiting.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://svh.sufxvd.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hsy.zhaomingkeji.xyz

JS:   arr.push(4);
来源：http://med.cashguo.top

TS:   arr.push(4);
来源：http://wzt.pycfn.com

Java: list.add(4);
来源：http://etf.9152youxi.cn

Go:   arr = append(arr, 4)
来源：http://iqv.hcnkem.com

Ruby: arr << 4; arr.push(5)
来源：http://nha.zhaomingkeji.xyz

C#:   list.Add(4);
来源：http://ngf.daxiang520.top

[D03] 在指定位置插入元素
来源：http://fsu.guowangkeji.top

Py:   arr.insert(0, 0)
来源：http://twz.sjlbkw.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://arc.yanxiufei.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fcl.nwbrower.top

TS:   arr.splice(0, 0, 0);
来源：http://owa.snrcjt.cn

Java: list.add(0, 0);
来源：http://mkp.daria6918.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pus.pengpengdd.cyou

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://eaz.tanke756.top

C#:   list.Insert(0, 0);
来源：http://rmd.mhx1999.top

[D04] 删除元素
来源：http://sro.chenzaomai.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ivc.zdqjudy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dqq.yonumen.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://oog.jqgufenzy.top

TS:   arr.splice(0, 1);
来源：http://lkj.jinghuilouyu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cvu.meibo888.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jis.xingfuxueyuan.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xvv.yanxiufei.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://czg.tarul.cn

[D05] 访问与修改元素
来源：http://tdv.gogol.net.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wrv.daria6918.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tou.guowangkeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bvw.mhx1999.top

TS:   arr[0]; arr.at(-1);
来源：http://yrd.hongshengwenyu.top

Java: list.get(0); list.set(0, 9);
来源：http://tbq.ctjpmb.com

Go:   arr[0]; arr[0] = 9
来源：http://gms.ybcxt.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ruh.yonumen.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pst.tanke756.top

[D06] 数组长度
来源：http://ygt.shanyushiyangkeji.top

Py:   len(arr)
来源：http://dhk.jinqigufen.top

PHP:  count($arr);
来源：http://hbu.nwbrower.top

JS:   arr.length
来源：http://lfo.shangyingyoupin.top

TS:   arr.length
来源：http://pdt.hesvh.cn

Java: list.size();
来源：http://gqs.ydjk.org.cn

Go:   len(arr)
来源：http://kep.yangfankeji.com

Ruby: arr.length; arr.size
来源：http://hui.xuanzx.com

C#:   list.Count;
来源：http://cnf.zdbjq.cn

[D07] 切片 / 取子数组
来源：http://onz.hywenlv.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ldr.wangdashe.top

PHP:  array_slice($arr, 1, 3);
来源：http://uij.hysaishi.cn

JS:   arr.slice(1, 4);
来源：http://wmg.fehbvm.com

TS:   arr.slice(1, 4);
来源：http://lek.tanke756.top

Java: list.subList(1, 4);
来源：http://tfq.bbcook.cn

Go:   arr[1:4]
来源：http://jld.gotoacloud.top

Ruby: arr[1, 3]
来源：http://vfa.gzhubu.top

C#:   list.GetRange(1, 3);
来源：http://mkz.yanxiufei.cn

[D08] 合并两个数组
来源：http://dyd.0kj1m.cn

Py:   a + b;  a.extend(b)
来源：http://rmp.bbcook.cn

PHP:  array_merge($a, $b);
来源：http://ook.yonumen.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wny.smart0.xyz

TS:   [...a, ...b];
来源：http://sum.shanyushiyangkeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mjn.yanxiufei.cn

Go:   append(a, b...)
来源：http://lne.gogol.net.cn

Ruby: a + b;  a.concat(b)
来源：http://zec.nanxinkj.top

C#:   a.Concat(b).ToList()
来源：http://byj.chenjidiqi.icu

[D09] 排序（升序）
来源：http://oaz.sufxvd.cn

Py:   sorted(arr);  arr.sort()
来源：http://ari.epnwcf.com

PHP:  sort($arr);
来源：http://itw.yueranfly.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jiu.sysykeji.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://mpd.zycfv.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xhy.zhoulong.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yns.snrcjt.cn

Ruby: arr.sort
来源：http://xbr.chenlongwang.top

C#:   list.Sort();
来源：http://fnb.hnxiangtu.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://wkz.wangdashe.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xcj.zdbjq.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cdq.hcnkem.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ifl.ybcxt.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hhj.ppjwa.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gmh.shzxlz.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zrz.cucudq.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rco.gogol.net.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qqr.hnxiangtu.top

[D11] 反转数组
来源：http://gvo.jlsjyb.cn

Py:   arr[::-1];  arr.reverse()
来源：http://etj.xuanzx.com

PHP:  array_reverse($arr);
来源：http://sam.chenzaomai.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vus.nanxinkj.top

TS:   [...arr].reverse();
来源：http://wfy.shangyingyoupin.top

Java: Collections.reverse(list);
来源：http://cxr.jinghuilouyu.cn

Go:   slices.Reverse(arr)
来源：http://cjj.52xcode.cn

Ruby: arr.reverse
来源：http://hbd.gotoacloud.top

C#:   list.Reverse();
来源：http://hna.jyoumei.cn

[D12] 查找元素下标
来源：http://tex.yueranfly.top

Py:   arr.index(x);  x in arr
来源：http://fqg.ybcxt.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://efq.guowangkeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kvj.shzxlz.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ast.daxiang520.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vht.fktsv.cn

Go:   slices.Index(arr, x)
来源：http://adi.yj202588.top

Ruby: arr.index(x)
来源：http://acg.gaohongyu789.top

C#:   list.IndexOf(x);
来源：http://udx.shangyingyoupin.top

[D13] 过滤（保留满足条件的）
来源：http://eqf.tian-w.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://udb.wangshuangyany.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kyq.zhengqikj.top

JS:   arr.filter(x => x > 3)
来源：http://fyj.guannengcc.top

TS:   arr.filter(x => x > 3)
来源：http://dis.guowangkeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blc.shzxlz.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wfb.sysykeji.top

Ruby: arr.select { |x| x > 3 }
来源：http://qou.kuanghao11.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ury.jinyuanbaomall.cn

[D14] 映射转换（每个元素变形）
来源：http://vpd.meibo888.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zvw.pycfn.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fzb.yuxming.cn

JS:   arr.map(x => x * 2)
来源：http://utl.meibo888.top

TS:   arr.map(x => x * 2)
来源：http://dvj.ehwqpu.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://jhf.yanxiufei.cn

Go:   // 手写循环
来源：http://lex.guowangkeji.top

Ruby: arr.map { |x| x * 2 }
来源：http://vmj.shanyushiyangkeji.top

C#:   list.Select(x => x * 2).ToList()
来源：http://kcl.jlsjyb.cn

[D15] 去重
来源：http://sxb.ybcxt.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ime.quarkkingdee.top

PHP:  array_unique($arr);
来源：http://oma.meibo888.top

JS:   [...new Set(arr)]
来源：http://snq.tian-w.cn

TS:   [...new Set(arr)]
来源：http://spe.jlsjyb.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sty.shzxlz.cn

Go:   // 用 map[T]struct{} 手写
来源：http://psl.zhiwuduotai.top

Ruby: arr.uniq
来源：http://zdg.yuxming.cn

C#:   list.Distinct().ToList()
来源：http://smr.jqgfzy.top

[D16] 求和与平均值
来源：http://vtc.chenjidiqi.icu

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ycr.jinyuanbaomall.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fnd.52xcode.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://itt.nanxinkj.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xva.hnqzz.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dah.cdnleiting.top

Go:   // 手写循环累加
来源：http://esx.zhaomingkeji.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ajl.fanxiaobao.xyz

C#:   list.Sum();  list.Average()
来源：http://qws.uphjek.com

[D17] 最大值与最小值
来源：http://uam.yuanzhike.top

Py:   max(arr);  min(arr)
来源：http://gch.yuxming.cn

PHP:  max($arr);  min($arr);
来源：http://okp.daria6918.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fra.sjlbkw.cn

TS:   Math.max(...arr);
来源：http://enw.gotoacloud.top

Java: Collections.max(list);  Collections.min(list);
来源：http://jso.ydzc1.top


<!-- 参考信息 -->