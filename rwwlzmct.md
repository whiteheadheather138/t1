代发 wailian999

================================================================================
来源：http://lrl.hongshengwenyu.top

C. 函数与作用域
来源：http://esp.sxryk.cn

================================================================================
来源：http://hoe.xuanzx.com

[C01] 定义函数
来源：http://bie.0kj1m.cn

Py:   def add(a, b): return a + b
来源：http://tar.jqgfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nxt.ydzc1.top

JS:   function add(a, b) { return a + b; }
来源：http://frt.shangyingyoupin.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://naw.shanyushiyangkeji.top

Java: static int add(int a, int b) { return a + b; }
来源：http://aya.yangfankeji.com

Go:   func add(a, b int) int { return a + b }
来源：http://ozd.fengsongda.top

Ruby: def add(a, b); a + b; end
来源：http://zdj.jlsjyb.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mom.smart0.xyz

[C02] 默认参数
来源：http://fnt.sweek.top

Py:   def greet(name="World"): return name
来源：http://maq.vqdsnc.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://txb.ydjk.org.cn

JS:   function greet(name = "World") { return name; }
来源：http://prd.uphjek.com

TS:   function greet(name: string = "World") { return name; }
来源：http://wnu.yuxming.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://woz.jinqigfzy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://eyy.cqqwz.cn

Ruby: def greet(name = "World") = name
来源：http://htn.sweek.top

C#:   string Greet(string name = "World") => name;
来源：http://lqd.yonumen.top

[C03] 可变参数
来源：http://fjp.meibo888.top

Py:   def total(*args): return sum(args)
来源：http://sii.gzhubu.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gsx.dashuyun.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wau.jinyuanbaomall.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ajg.sjlbkw.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://evm.yonumen.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gss.daxiang520.top

Ruby: def total(*nums); nums.sum; end
来源：http://rgn.yj202588.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wvb.vehdjk.com

[C04] 命名参数 / 关键字参数
来源：http://cfb.nanxuanxn.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vvk.yj20258.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cir.hnxiangtu.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gtn.kuanghao11.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jrg.nanxuanxn.top

Java: // 无：用 Builder 模式或 record
来源：http://cig.mhx1999.top

Go:   // 无：用配置结构体参数
来源：http://wkq.epnwcf.com

Ruby: f(a: 1, b: 2)
来源：http://ynu.fktsv.cn

C#:   f(a: 1, b: 2)
来源：http://sgv.jinqigufen.top

[C05] 返回多个值
来源：http://niv.316326.xyz

Py:   return a, b
来源：http://kdr.nanxuanxn.top

PHP:  return [$a, $b];
来源：http://mkg.fanxiaobao.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://qys.nanxuanxn.top

TS:   return { a, b };
来源：http://tyl.cdnleiting.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tld.bbcook.cn

Go:   return a, b
来源：http://acj.yj20258888.top

Ruby: return a, b
来源：http://ltq.wangdashe.top

C#:   return (a, b);              // ValueTuple
来源：http://wql.yvedp.cn

[C06] 匿名函数 / lambda
来源：http://wyt.pengpengdd.cyou

Py:   square = lambda x: x * x
来源：http://enm.ydjk.org.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://blz.yj202588.top

JS:   const square = x => x * x;
来源：http://wny.zhiwuduotai.top

TS:   const square = (x: number): number => x * x;
来源：http://bia.jqgfzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fbz.fehbvm.com

Go:   sq := func(x int) int { return x * x }
来源：http://ddt.jinqigufen.top

Ruby: square = ->(x) { x * x }
来源：http://jwv.yonumen.top

C#:   Func<int, int> square = x => x * x;
来源：http://sra.kuanghao11.cn

[C07] 把函数作为参数传入
来源：http://ija.yj202588.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lhx.jqgfzy.top

PHP:  array_map("strtoupper", $arr);
来源：http://mpv.tanke756.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xue.zhengqikj.top

TS:   arr.map(String)
来源：http://zdq.jiagoushi.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://oqq.gogol.net.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://czn.zhijiandao.cn

Ruby: arr.map(&:upcase)
来源：http://frx.yvedp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://guz.feifeiyinyue.top

[C08] 闭包
来源：http://qxg.cdnleiting.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rpd.zycfv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mgj.zhijiandao.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://npr.vehdjk.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vkm.yj202588.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://upa.sweek.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hfc.fengsongda.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gtq.tian-w.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qgv.tanke756.top

[C09] 递归
来源：http://bwb.hnxiangtu.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ncy.guannengcc.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zgm.hysaishi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pxk.tianlin.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mme.tianlin.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://inp.ehwqpu.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://prt.xuanzx.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ynk.xinyue.icu

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kmy.zhongyouzk.top

[C10] 变量作用域
来源：http://cln.316326.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fwq.nanxinkj.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cbb.yueranfly.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gro.gzhubu.top

TS:   同 JS
来源：http://not.hesvh.cn

Java: 方法内为块级作用域
来源：http://gls.hysaishi.cn

Go:   花括号块级作用域
来源：http://wlw.cqqwz.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jio.jianghu66.top

C#:   块级作用域
来源：http://ers.zhiwuduotai.top

[C11] 模块导入与导出
来源：http://fai.ehwqpu.com

Py:   from module import func
来源：http://hsd.jinqigfzy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://vzf.316326.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://urz.chenzaomai.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xqu.tanke756.top

Java: import java.util.List;
来源：http://nta.zhixingplan.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pyf.havefunace.top

Ruby: require "json"; require_relative "./util"
来源：http://zxn.jiagoushi.top

C#:   using System.Text;
来源：http://btk.yj20258.top

[C12] 立即执行函数 IIFE
来源：http://xwr.zhongyouzk.top

Py:   (lambda: print("run"))()
来源：http://sny.dashuyun.cn

PHP:  (function () { echo "run"; })();
来源：http://eky.quarkkingdee.top

JS:   (() => { console.log("run"); })();
来源：http://suu.sweek.top

TS:   (() => { console.log("run"); })();
来源：http://zvd.cdnleiting.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rmn.nwbrower.top

Go:   func() { fmt.Println("run") }()
来源：http://vqw.jqgufenzy.top

Ruby: -> { puts "run" }.call
来源：http://irj.vqdsnc.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://sgf.tianlin.xyz

[C13] 类型声明 / 类型注解
来源：http://ujr.kuanghao11.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kee.jqgfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bkl.meibo888.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sof.fktsv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ssn.yuanzhike.top

Java: int add(int a, int b) { return a + b; }
来源：http://qqu.zdqjudy.top

Go:   func add(a, b int) int
来源：http://keo.yfazqb.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ayf.sxryk.cn

C#:   int Add(int a, int b) => a + b;
来源：http://poe.jinghuilouyu.cn

[C14] 泛型函数
来源：http://eww.yj20258.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://flk.tanke756.top

PHP:  // 无泛型
来源：http://gpf.yj20258.top

JS:   // 无泛型
来源：http://vuy.hesvh.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vup.jqgufenzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wqx.sufxvd.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vgq.zycfv.cn

Ruby: # 无泛型
来源：http://zxe.jinqigufen.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wkc.gotoacloud.top

[C15] 解构 / 展开参数
来源：http://cdp.meibo888.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://eaz.yuxming.cn

PHP:  [$a, $b] = $pair;
来源：http://kyh.feifeiyinyue.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cxs.jianghu66.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rkn.xuanzx.com

Java: // 无解构
来源：http://ucp.ydzc1.top

Go:   // 无解构
来源：http://fmd.yj20258888.top

Ruby: a, b = pair
来源：http://hoz.tian-w.cn

C#:   var (a, b) = pair;
来源：http://hgf.sweek.top

[C16] 函数 / 方法重载
来源：http://agm.jiagoushi.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vqq.meibo888.top

PHP:  // 无重载
来源：http://hfk.xinyue.icu

JS:   // 无重载：靠 arguments.length 分支
来源：http://och.sysykeji.top

TS:   // 用联合类型或重载签名声明
来源：http://ina.snrcjt.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://glr.ydjk.org.cn

Go:   // 无重载：用不同函数名
来源：http://zhk.nwbrower.top

Ruby: # 无重载：靠动态参数
来源：http://zlu.hnqzz.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://okx.andypj.xyz

================================================================================
来源：http://sob.meibo888.top

D. 数组 / 列表 / 集合
来源：http://icq.kuanghao11.cn

================================================================================
来源：http://pyn.vqdsnc.cn

[D01] 创建数组 / 列表
来源：http://ybs.9152youxi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://phb.hesvh.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://snw.nwbrower.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://whk.yanxiufei.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jxt.meibo888.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fcd.yj202588.top

Go:   arr := []int{1, 2, 3}
来源：http://hzn.jinghuilouyu.cn

Ruby: arr = [1, 2, 3]
来源：http://kkg.zhijiandao.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://oqi.jianghu66.top

[D02] 追加元素到末尾
来源：http://zbx.ehwqpu.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mrs.epnwcf.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://adg.shangyingyoupin.top

JS:   arr.push(4);
来源：http://nlx.feifeiyinyue.top

TS:   arr.push(4);
来源：http://qnc.fehbvm.com

Java: list.add(4);
来源：http://ohq.jinyuanbaomall.cn

Go:   arr = append(arr, 4)
来源：http://dos.daria6918.cn

Ruby: arr << 4; arr.push(5)
来源：http://vau.zdqjudy.top

C#:   list.Add(4);
来源：http://tha.fengsongda.top

[D03] 在指定位置插入元素
来源：http://ypp.haohaochexian.top

Py:   arr.insert(0, 0)
来源：http://num.havefunace.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vfk.hnxiangtu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://eyd.feifeiyinyue.top

TS:   arr.splice(0, 0, 0);
来源：http://jau.sxryk.cn

Java: list.add(0, 0);
来源：http://mfl.chenjidiqi.icu

Go:   arr = append([]int{0}, arr...)
来源：http://kqy.ivvv.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sdf.yongpay.top

C#:   list.Insert(0, 0);
来源：http://tqf.meibo888.top

[D04] 删除元素
来源：http://dhc.tian-w.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zcb.mhx1999.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hbk.shanyushiyangtech.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://szc.redwolf501.top

TS:   arr.splice(0, 1);
来源：http://dhv.xylfe.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pha.jqgufenzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://myq.zhengqikj.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://njv.fktsv.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cay.mhx1999.top

[D05] 访问与修改元素
来源：http://qvh.yuxming.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zua.havefunace.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bir.sweek.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://eya.hongshengwenyu.top

TS:   arr[0]; arr.at(-1);
来源：http://dya.nanxinkj.top

Java: list.get(0); list.set(0, 9);
来源：http://bwf.vqdsnc.cn

Go:   arr[0]; arr[0] = 9
来源：http://fse.vehdjk.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nsb.nanxuanxn.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uje.fktsv.cn

[D06] 数组长度
来源：http://fbu.zhengqikj.top

Py:   len(arr)
来源：http://eji.tian-w.cn

PHP:  count($arr);
来源：http://aki.yj20258.top

JS:   arr.length
来源：http://jdf.zhiwuduotai.top

TS:   arr.length
来源：http://oxo.jiagoushi.top

Java: list.size();
来源：http://fxy.yj20258.top

Go:   len(arr)
来源：http://emr.zdbjq.cn

Ruby: arr.length; arr.size
来源：http://ckw.zhaomingkeji.xyz

C#:   list.Count;
来源：http://uhf.yj20258888.top

[D07] 切片 / 取子数组
来源：http://vcy.zdqjudy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gof.fanxiaobao.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://ybz.daria6918.cn

JS:   arr.slice(1, 4);
来源：http://xnt.c1oappe.top

TS:   arr.slice(1, 4);
来源：http://xpa.hfpthk.cn

Java: list.subList(1, 4);
来源：http://vcv.fzhhl.top

Go:   arr[1:4]
来源：http://wbo.quarkkingdee.top

Ruby: arr[1, 3]
来源：http://xvm.cdnleiting.top

C#:   list.GetRange(1, 3);
来源：http://ljq.pengpengdd.cyou

[D08] 合并两个数组
来源：http://zxd.fengsongda.top

Py:   a + b;  a.extend(b)
来源：http://rga.zdbjq.cn

PHP:  array_merge($a, $b);
来源：http://aux.yj202588.top

JS:   [...a, ...b];  a.concat(b);
来源：http://sjd.ehwqpu.com

TS:   [...a, ...b];
来源：http://dxk.quarkkingdee.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://iiq.wangdashe.top

Go:   append(a, b...)
来源：http://diq.dianchejie.cn

Ruby: a + b;  a.concat(b)
来源：http://xvh.vehdjk.com

C#:   a.Concat(b).ToList()
来源：http://opn.zhongyouzk.top

[D09] 排序（升序）
来源：http://upu.yfazqb.com

Py:   sorted(arr);  arr.sort()
来源：http://xfy.hfpthk.cn

PHP:  sort($arr);
来源：http://ypq.yvedp.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xvs.xuanzx.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://fja.yangfankeji.com

Java: Collections.sort(list);  list.sort(null);
来源：http://jba.jyoumei.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sdt.vqdsnc.cn

Ruby: arr.sort
来源：http://hir.ehwqpu.com

C#:   list.Sort();
来源：http://nan.nwbrower.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://tfi.ehwqpu.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hrw.haohaochexian.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hoz.feifeiyinyue.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pgj.zhoulong.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fpj.sjlbkw.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://czf.mhx1999.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mwx.vehdjk.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pgd.yfazqb.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ojg.zhaomingkeji.xyz

[D11] 反转数组
来源：http://sgd.ybcxt.top

Py:   arr[::-1];  arr.reverse()
来源：http://inn.tianlin.xyz

PHP:  array_reverse($arr);
来源：http://mey.316326.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://btr.zhiwuduotai.top

TS:   [...arr].reverse();
来源：http://rof.nanxuanxn.top

Java: Collections.reverse(list);
来源：http://bfg.iojbl.cn

Go:   slices.Reverse(arr)
来源：http://fzi.pycfn.com

Ruby: arr.reverse
来源：http://jhk.sufxvd.cn

C#:   list.Reverse();
来源：http://rit.smart0.xyz

[D12] 查找元素下标
来源：http://aic.yvedp.cn

Py:   arr.index(x);  x in arr
来源：http://vjp.yangfankeji.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rxz.ybcxt.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tcm.feifeiyinyue.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xel.yfazqb.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vlf.yvedp.cn

Go:   slices.Index(arr, x)
来源：http://wex.sxryk.cn

Ruby: arr.index(x)
来源：http://fob.shzxlz.cn

C#:   list.IndexOf(x);
来源：http://grn.hysaishi.cn

[D13] 过滤（保留满足条件的）
来源：http://pxv.fehbvm.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yyk.meibo888.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jqb.yuanzhike.top

JS:   arr.filter(x => x > 3)
来源：http://arw.hfpthk.cn

TS:   arr.filter(x => x > 3)
来源：http://hmi.jqgfzy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nnr.ywan-chungtsiang.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://stq.birdmap.top

Ruby: arr.select { |x| x > 3 }
来源：http://bsi.cashguo.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ixn.jinyuanbaomall.cn

[D14] 映射转换（每个元素变形）
来源：http://vnb.jianghu66.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jxw.fanxiaobao.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://waj.nwbrower.top

JS:   arr.map(x => x * 2)
来源：http://weu.quarkkingdee.top

TS:   arr.map(x => x * 2)
来源：http://ftu.yvedp.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://uqo.ydjk.org.cn

Go:   // 手写循环
来源：http://rwu.hnxiangtu.top

Ruby: arr.map { |x| x * 2 }
来源：http://ezd.yj20258.top

C#:   list.Select(x => x * 2).ToList()
来源：http://bzk.gotoacloud.top

[D15] 去重
来源：http://xpb.tanke756.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hen.zhiwuduotai.top

PHP:  array_unique($arr);
来源：http://gpd.uphjek.com

JS:   [...new Set(arr)]
来源：http://dkp.yj202588.top

TS:   [...new Set(arr)]
来源：http://isr.zhijiandao.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dsv.ehwqpu.com

Go:   // 用 map[T]struct{} 手写
来源：http://ivc.jiagoushi.top

Ruby: arr.uniq
来源：http://akz.zdqjudy.top

C#:   list.Distinct().ToList()
来源：http://dnw.snrcjt.cn

[D16] 求和与平均值
来源：http://nas.andypj.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lib.fzhhl.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wtk.kuanghao11.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sth.fehbvm.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://iqw.gogol.net.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vuo.pycfn.com

Go:   // 手写循环累加
来源：http://aqm.jianghu66.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fhg.shzxlz.cn

C#:   list.Sum();  list.Average()
来源：http://bza.ybcxt.top

[D17] 最大值与最小值
来源：http://rui.ywan-chungtsiang.top

Py:   max(arr);  min(arr)
来源：http://fig.haohaochexian.top

PHP:  max($arr);  min($arr);
来源：http://jhf.tianlin.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yaj.dashuyun.cn

TS:   Math.max(...arr);
来源：http://mfv.feifeiyinyue.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ilh.zycfv.cn


<!-- 参考信息 -->