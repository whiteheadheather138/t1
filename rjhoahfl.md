代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://asq.jyoumei.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://xsu.zhiwuduotai.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zbi.fanxiaobao.xyz

Ruby: def greet(name = "World") = name
来源：http://imv.ppjwa.cn

C#:   string Greet(string name = "World") => name;
来源：http://kfb.shanyushiyangtech.top

[C03] 可变参数
来源：http://knw.shzxlz.cn

Py:   def total(*args): return sum(args)
来源：http://gmt.ybcxt.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kgj.ydzc1.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hnv.zhijiandao.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bss.hfpthk.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kfg.tianlin.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qpl.yanxiufei.cn

Ruby: def total(*nums); nums.sum; end
来源：http://igs.bjfxy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ycz.zhaomingkeji.xyz

[C04] 命名参数 / 关键字参数
来源：http://dcv.yfazqb.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wvo.0kj1m.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pft.hcnkem.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lav.tanke756.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ydu.tarul.cn

Java: // 无：用 Builder 模式或 record
来源：http://zhh.fengsongda.top

Go:   // 无：用配置结构体参数
来源：http://lot.hnqzz.top

Ruby: f(a: 1, b: 2)
来源：http://yih.zhoulong.xyz

C#:   f(a: 1, b: 2)
来源：http://lpi.shanyushiyangtech.top

[C05] 返回多个值
来源：http://osg.ppjwa.cn

Py:   return a, b
来源：http://aox.cqqwz.cn

PHP:  return [$a, $b];
来源：http://ybx.ppjwa.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zrh.wangshuangyany.cn

TS:   return { a, b };
来源：http://bts.yuanzhike.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hma.haohaochexian.top

Go:   return a, b
来源：http://kvl.andypj.xyz

Ruby: return a, b
来源：http://bfa.meibo888.top

C#:   return (a, b);              // ValueTuple
来源：http://vev.tianlin.xyz

[C06] 匿名函数 / lambda
来源：http://ego.gaohongyu789.top

Py:   square = lambda x: x * x
来源：http://bze.cdnleiting.top

PHP:  $square = fn($x) => $x * $x;
来源：http://uti.sweek.top

JS:   const square = x => x * x;
来源：http://blt.aibaodan.cn

TS:   const square = (x: number): number => x * x;
来源：http://qsn.ydzc1.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hih.zhoulong.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://lko.hywenlv.cn

Ruby: square = ->(x) { x * x }
来源：http://dfs.xuanzx.com

C#:   Func<int, int> square = x => x * x;
来源：http://tlb.yvedp.cn

[C07] 把函数作为参数传入
来源：http://zmy.sufxvd.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wiw.sjlbkw.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mjy.ybcxt.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://twz.yfazqb.com

TS:   arr.map(String)
来源：http://nzs.fehbvm.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nul.sufxvd.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wth.shangyingyoupin.top

Ruby: arr.map(&:upcase)
来源：http://ehs.zycfv.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://tjz.guowangkeji.top

[C08] 闭包
来源：http://wyq.yvedp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baf.fengsongda.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nyp.mhx1999.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qdr.yanxiufei.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gyu.jinghuilouyu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://elf.fanxiaobao.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tgi.ppjwa.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rlb.hysaishi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xvh.yj202588.top

[C09] 递归
来源：http://vyx.kuanghao11.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fpa.yueranfly.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tam.xziqi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qii.52xcode.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ltp.gaohongyu789.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pfv.feifeiyinyue.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ayh.zhijiandao.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://eal.ybcxt.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mww.yj20258.top

[C10] 变量作用域
来源：http://ice.xingfuxueyuan.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mmv.yvedp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cie.xuetiantiany.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rnk.vqdsnc.cn

TS:   同 JS
来源：http://zrt.hnxiangtu.top

Java: 方法内为块级作用域
来源：http://fdu.zhongyouzk.top

Go:   花括号块级作用域
来源：http://hpn.dashuyun.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fka.dianchejie.cn

C#:   块级作用域
来源：http://grl.dashuyun.cn

[C11] 模块导入与导出
来源：http://aph.yongpay.top

Py:   from module import func
来源：http://lbu.yj202588.top

PHP:  require "file.php";  或 use App\Service;
来源：http://xvz.shangyingyoupin.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://byr.hfpthk.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tsz.chenjidiqi.icu

Java: import java.util.List;
来源：http://dxd.gzhubu.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jai.ywan-chungtsiang.top

Ruby: require "json"; require_relative "./util"
来源：http://amn.chenlongwang.top

C#:   using System.Text;
来源：http://qym.zycfv.cn

[C12] 立即执行函数 IIFE
来源：http://yzn.shuidangran.top

Py:   (lambda: print("run"))()
来源：http://vwv.cashguo.top

PHP:  (function () { echo "run"; })();
来源：http://pny.hywenlv.cn

JS:   (() => { console.log("run"); })();
来源：http://hlo.cheryme.top

TS:   (() => { console.log("run"); })();
来源：http://gnh.cdnleiting.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yta.ywan-chungtsiang.top

Go:   func() { fmt.Println("run") }()
来源：http://cyt.xinyue.icu

Ruby: -> { puts "run" }.call
来源：http://pcc.ivvv.top

C#:   // 无 IIFE：用静态构造函数
来源：http://qmt.yonumen.top

[C13] 类型声明 / 类型注解
来源：http://jmb.cqqwz.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rnh.zhoulong.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nxm.meibo888.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zmu.cheryme.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dye.yj20258.top

Java: int add(int a, int b) { return a + b; }
来源：http://xow.tian-w.cn

Go:   func add(a, b int) int
来源：http://wvh.yuxming.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://twk.hongshengwenyu.top

C#:   int Add(int a, int b) => a + b;
来源：http://xxg.ehwqpu.com

[C14] 泛型函数
来源：http://cxm.redwolf501.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dhv.svipenyu.cn

PHP:  // 无泛型
来源：http://kup.zdbjq.cn

JS:   // 无泛型
来源：http://rcx.aizwys.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://heo.pengpengdd.cyou

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uus.aibaodan.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tna.meibo888.top

Ruby: # 无泛型
来源：http://pau.mhx1999.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xut.wangshuangyany.cn

[C15] 解构 / 展开参数
来源：http://yup.zhoulong.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://msk.redwolf501.top

PHP:  [$a, $b] = $pair;
来源：http://pzp.fengsongda.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gfp.jiagoushi.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wvi.fktsv.cn

Java: // 无解构
来源：http://hzu.yj20258888.top

Go:   // 无解构
来源：http://nmp.shuidangran.top

Ruby: a, b = pair
来源：http://qai.chenjidiqi.icu

C#:   var (a, b) = pair;
来源：http://pwv.zdqjudy.top

[C16] 函数 / 方法重载
来源：http://som.jinqigufen.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lvx.hesvh.cn

PHP:  // 无重载
来源：http://giw.ydzc1.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://bvj.shuidangran.top

TS:   // 用联合类型或重载签名声明
来源：http://pob.vehdjk.com

Java: void f(int a) {}  void f(String a) {}
来源：http://xoi.yangfankeji.com

Go:   // 无重载：用不同函数名
来源：http://swx.c1oappe.top

Ruby: # 无重载：靠动态参数
来源：http://pqq.jinqigfzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://drt.chenzaomai.com

================================================================================
来源：http://jee.chenjidiqi.icu

D. 数组 / 列表 / 集合
来源：http://olf.yanxiufei.cn

================================================================================
来源：http://sup.guowangkeji.top

[D01] 创建数组 / 列表
来源：http://odv.vqdsnc.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://yoa.jlsjyb.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nat.tianlin.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ddb.c1oappe.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://afi.sysykeji.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gkh.zhengqikj.top

Go:   arr := []int{1, 2, 3}
来源：http://sjv.xingfuxueyuan.xyz

Ruby: arr = [1, 2, 3]
来源：http://ksg.kuanghao11.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nup.gzhubu.top

[D02] 追加元素到末尾
来源：http://pfs.havefunace.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://htu.c1oappe.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uel.jyoumei.cn

JS:   arr.push(4);
来源：http://ohp.zhengqikj.top

TS:   arr.push(4);
来源：http://mpv.jyoumei.cn

Java: list.add(4);
来源：http://jnn.wangdashe.top

Go:   arr = append(arr, 4)
来源：http://tio.yvedp.cn

Ruby: arr << 4; arr.push(5)
来源：http://jxn.fengsongda.top

C#:   list.Add(4);
来源：http://jcz.iojbl.cn

[D03] 在指定位置插入元素
来源：http://qax.zhoulong.xyz

Py:   arr.insert(0, 0)
来源：http://uew.xuetiantiany.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gle.gotoacloud.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://aik.zhoulong.xyz

TS:   arr.splice(0, 0, 0);
来源：http://wcg.9152youxi.cn

Java: list.add(0, 0);
来源：http://zcz.aibaodan.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xrb.shangyingyoupin.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fxs.yangfankeji.com

C#:   list.Insert(0, 0);
来源：http://zob.epnwcf.com

[D04] 删除元素
来源：http://ckx.guannengcc.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tvl.mhx1999.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gbr.iojbl.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wwg.gogol.net.cn

TS:   arr.splice(0, 1);
来源：http://tzd.316326.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nrf.sufxvd.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hrb.tianlin.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jsp.aizwys.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fym.zycfv.cn

[D05] 访问与修改元素
来源：http://cil.cqqwz.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://epb.chenzaomai.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pca.birdmap.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dfp.haohaochexian.top

TS:   arr[0]; arr.at(-1);
来源：http://jds.0kj1m.cn

Java: list.get(0); list.set(0, 9);
来源：http://tjm.jlsjyb.cn

Go:   arr[0]; arr[0] = 9
来源：http://cqe.gaohongyu789.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wkh.zhongyouzk.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dbt.fanxiaobao.xyz

[D06] 数组长度
来源：http://ykv.nanxinkj.top

Py:   len(arr)
来源：http://mvv.tanke756.top

PHP:  count($arr);
来源：http://aor.gzhubu.top

JS:   arr.length
来源：http://jjl.hfpthk.cn

TS:   arr.length
来源：http://vdu.jlsjyb.cn

Java: list.size();
来源：http://cei.shanyushiyangkeji.top

Go:   len(arr)
来源：http://xlg.chenzaomai.com

Ruby: arr.length; arr.size
来源：http://xaa.fktsv.cn

C#:   list.Count;
来源：http://ifi.smart0.xyz

[D07] 切片 / 取子数组
来源：http://xvp.jlsjyb.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zcm.sweek.top

PHP:  array_slice($arr, 1, 3);
来源：http://npt.jiagoushi.top

JS:   arr.slice(1, 4);
来源：http://kvq.ywan-chungtsiang.top

TS:   arr.slice(1, 4);
来源：http://hbm.yj20258888.top

Java: list.subList(1, 4);
来源：http://jnv.daria6918.cn

Go:   arr[1:4]
来源：http://eud.feifeiyinyue.top

Ruby: arr[1, 3]
来源：http://ymw.shuidangran.top

C#:   list.GetRange(1, 3);
来源：http://jzw.aizwys.cn

[D08] 合并两个数组
来源：http://pgk.wangshuangyany.cn

Py:   a + b;  a.extend(b)
来源：http://qhk.aibaodan.cn

PHP:  array_merge($a, $b);
来源：http://hqu.fengsongda.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ang.yj202588.top

TS:   [...a, ...b];
来源：http://xbr.jqgufenzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rbt.jinyuanbaomall.cn

Go:   append(a, b...)
来源：http://elq.zdqjudy.top

Ruby: a + b;  a.concat(b)
来源：http://dzr.wangshuangyany.cn

C#:   a.Concat(b).ToList()
来源：http://loz.dianchejie.cn

[D09] 排序（升序）
来源：http://riw.hywenlv.cn

Py:   sorted(arr);  arr.sort()
来源：http://ngc.shangyingyoupin.top

PHP:  sort($arr);
来源：http://qdp.ydjk.org.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nap.haohaochexian.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://xwl.tian-w.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://sim.yuxming.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jje.gaohongyu789.top

Ruby: arr.sort
来源：http://nvf.pengpengdd.cyou

C#:   list.Sort();
来源：http://gik.xziqi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://dni.jqgufenzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ucz.daria6918.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://acc.guowangkeji.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qqt.epnwcf.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://heq.cashguo.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tze.sxryk.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hlw.yanxiufei.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mcr.hongshengwenyu.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dti.ehwqpu.com

[D11] 反转数组
来源：http://vcv.ctjpmb.com

Py:   arr[::-1];  arr.reverse()
来源：http://dma.yuanzhike.top

PHP:  array_reverse($arr);
来源：http://uwx.mhx1999.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://txy.yuxming.cn

TS:   [...arr].reverse();
来源：http://ugd.fzhhl.top

Java: Collections.reverse(list);
来源：http://rok.chenjidiqi.icu

Go:   slices.Reverse(arr)
来源：http://izr.xylfe.cn

Ruby: arr.reverse
来源：http://bjo.nanxuanxn.top

C#:   list.Reverse();
来源：http://yys.cdnleiting.top

[D12] 查找元素下标
来源：http://esm.jianghu66.top

Py:   arr.index(x);  x in arr
来源：http://nkn.jinqigfzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://abu.cucudq.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xzf.quarkkingdee.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xhg.zdqjudy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yxz.chenlongwang.top

Go:   slices.Index(arr, x)
来源：http://kll.sufxvd.cn

Ruby: arr.index(x)
来源：http://njv.cucudq.cn

C#:   list.IndexOf(x);
来源：http://ilw.bjfxy.top

[D13] 过滤（保留满足条件的）
来源：http://pbd.yanxiufei.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pwn.yueranfly.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fmy.hammf.cn

JS:   arr.filter(x => x > 3)
来源：http://knz.jqgfzy.top

TS:   arr.filter(x => x > 3)
来源：http://xej.jinghuilouyu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nxu.ivvv.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vnt.fehbvm.com

Ruby: arr.select { |x| x > 3 }
来源：http://xfn.fanxiaobao.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://his.yueranfly.top

[D14] 映射转换（每个元素变形）
来源：http://tlb.9152youxi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zkd.xingfuxueyuan.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://msc.yanxiufei.cn

JS:   arr.map(x => x * 2)
来源：http://vhg.sjlbkw.cn

TS:   arr.map(x => x * 2)
来源：http://cbr.cashguo.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://cjv.pycfn.com

Go:   // 手写循环
来源：http://xyl.hongshengwenyu.top

Ruby: arr.map { |x| x * 2 }
来源：http://odw.gzhubu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://xqr.wangdashe.top

[D15] 去重
来源：http://ivy.yj20258888.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://iyv.ehwqpu.com

PHP:  array_unique($arr);
来源：http://zxm.fanxiaobao.xyz

JS:   [...new Set(arr)]
来源：http://tku.hesvh.cn

TS:   [...new Set(arr)]
来源：http://bsf.gotoacloud.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dkz.gogol.net.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zpz.vqdsnc.cn

Ruby: arr.uniq
来源：http://adu.hywenlv.cn

C#:   list.Distinct().ToList()
来源：http://gcv.fktsv.cn

[D16] 求和与平均值
来源：http://ido.nanxinkj.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lfu.jqgufenzy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rdn.fktsv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hyf.hesvh.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tyh.ybcxt.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://oxm.jyoumei.cn

Go:   // 手写循环累加
来源：http://dml.cucudq.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wtx.fengsongda.top

C#:   list.Sum();  list.Average()
来源：http://soa.aizwys.cn

[D17] 最大值与最小值
来源：http://wyr.yj202588.top

Py:   max(arr);  min(arr)
来源：http://atk.xuanzx.com

PHP:  max($arr);  min($arr);
来源：http://icr.xingfuxueyuan.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pux.epnwcf.com

TS:   Math.max(...arr);
来源：http://tvf.sxryk.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://vbv.daria6918.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://oeo.bbcook.cn

Ruby: arr.max;  arr.min
来源：http://pzn.cucudq.cn

C#:   list.Max();  list.Min()
来源：http://owg.zdqjudy.top

[D18] 扁平化嵌套数组
来源：http://ebv.kuanghao11.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ydd.wangdashe.top

PHP:  array_merge(...$nested);
来源：http://ajj.zhoulong.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://iev.ehwqpu.com

TS:   nested.flat();
来源：http://egs.chenlongwang.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://acl.fehbvm.com

Go:   // 手写双层循环
来源：http://emn.nanxuanxn.top

Ruby: nested.flatten
来源：http://fji.ppjwa.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://cfs.9152youxi.cn

[D19] 按字段分组
来源：http://zko.xingfuxueyuan.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hml.nwbrower.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qbk.havefunace.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gls.jyoumei.cn


<!-- 参考信息 -->