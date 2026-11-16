代发 wailian999

[C02] 默认参数
来源：http://rfi.hnqzz.top

Py:   def greet(name="World"): return name
来源：http://dot.sweek.top

PHP:  function greet($name = "World") { return $name; }
来源：http://xcs.zhixingplan.top

JS:   function greet(name = "World") { return name; }
来源：http://prn.cqqwz.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://obn.xylfe.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://kwu.xylfe.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://srp.ehwqpu.com

Ruby: def greet(name = "World") = name
来源：http://vzr.yuanzhike.top

C#:   string Greet(string name = "World") => name;
来源：http://azg.shanyushiyangtech.top

[C03] 可变参数
来源：http://bcc.gogol.net.cn

Py:   def total(*args): return sum(args)
来源：http://bhj.cashguo.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rib.guowangkeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rkd.vehdjk.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://muq.aizwys.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ctq.haohaochexian.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kvu.shzxlz.cn

Ruby: def total(*nums); nums.sum; end
来源：http://efw.yangfankeji.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://esj.jinqigufen.top

[C04] 命名参数 / 关键字参数
来源：http://jzv.aizwys.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://aso.iojbl.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jxx.yj20258888.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://axk.ppjwa.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zfd.bjfxy.top

Java: // 无：用 Builder 模式或 record
来源：http://zvu.guannengcc.top

Go:   // 无：用配置结构体参数
来源：http://amf.hfpthk.cn

Ruby: f(a: 1, b: 2)
来源：http://vud.cucudq.cn

C#:   f(a: 1, b: 2)
来源：http://ulj.aizwys.cn

[C05] 返回多个值
来源：http://cxe.cheryme.top

Py:   return a, b
来源：http://vfg.yvedp.cn

PHP:  return [$a, $b];
来源：http://pmx.yongpay.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://zup.uphjek.com

TS:   return { a, b };
来源：http://mwl.hywenlv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hxs.cdnleiting.top

Go:   return a, b
来源：http://qoz.yfazqb.com

Ruby: return a, b
来源：http://xgn.zhongyouzk.top

C#:   return (a, b);              // ValueTuple
来源：http://swi.jinyuanbaomall.cn

[C06] 匿名函数 / lambda
来源：http://dbo.yj202588.top

Py:   square = lambda x: x * x
来源：http://xsy.jinqigufen.top

PHP:  $square = fn($x) => $x * $x;
来源：http://eiw.epnwcf.com

JS:   const square = x => x * x;
来源：http://kye.ydjk.org.cn

TS:   const square = (x: number): number => x * x;
来源：http://bxr.vehdjk.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rpb.xziqi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ioc.nanxinkj.top

Ruby: square = ->(x) { x * x }
来源：http://mpy.guowangkeji.top

C#:   Func<int, int> square = x => x * x;
来源：http://cuf.hongshengwenyu.top

[C07] 把函数作为参数传入
来源：http://lep.hammf.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://unq.sxryk.cn

PHP:  array_map("strtoupper", $arr);
来源：http://fre.cdnleiting.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zib.dashuyun.cn

TS:   arr.map(String)
来源：http://upz.gaohongyu789.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://asz.yj20258888.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uyq.jyoumei.cn

Ruby: arr.map(&:upcase)
来源：http://hhw.gogol.net.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fzj.hnqzz.top

[C08] 闭包
来源：http://hoy.chenjidiqi.icu

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ttt.sjlbkw.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vls.pycfn.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jpn.feifeiyinyue.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hqc.zhengqikj.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wwf.zdbjq.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zzb.kuanghao11.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lpd.shuidangran.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cyb.dianchejie.cn

[C09] 递归
来源：http://gqs.yongpay.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jcl.zhiwuduotai.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jgp.zhijiandao.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bgw.zhijiandao.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vjf.xuetiantiany.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nkn.yonumen.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vvd.yangfankeji.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lkv.dianchejie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://oct.dianchejie.cn

[C10] 变量作用域
来源：http://ubo.xuanzx.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xhh.shanyushiyangkeji.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bog.daxiang520.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://poc.jinyuanbaomall.cn

TS:   同 JS
来源：http://oxd.pengpengdd.cyou

Java: 方法内为块级作用域
来源：http://zmx.ivvv.top

Go:   花括号块级作用域
来源：http://wur.yfazqb.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bkc.zhoulong.xyz

C#:   块级作用域
来源：http://zgo.vqdsnc.cn

[C11] 模块导入与导出
来源：http://dcw.shangyingyoupin.top

Py:   from module import func
来源：http://xck.316326.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://ttc.0kj1m.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pxi.gotoacloud.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ani.jqgfzy.top

Java: import java.util.List;
来源：http://wvo.havefunace.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lsu.vehdjk.com

Ruby: require "json"; require_relative "./util"
来源：http://hwl.bbcook.cn

C#:   using System.Text;
来源：http://dls.jianghu66.top

[C12] 立即执行函数 IIFE
来源：http://ltv.shanyushiyangkeji.top

Py:   (lambda: print("run"))()
来源：http://owz.zhijiandao.cn

PHP:  (function () { echo "run"; })();
来源：http://qox.ivvv.top

JS:   (() => { console.log("run"); })();
来源：http://ycl.xinyue.icu

TS:   (() => { console.log("run"); })();
来源：http://cno.sufxvd.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hsq.jiagoushi.top

Go:   func() { fmt.Println("run") }()
来源：http://xvh.smart0.xyz

Ruby: -> { puts "run" }.call
来源：http://fyk.jlsjyb.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://afi.shzxlz.cn

[C13] 类型声明 / 类型注解
来源：http://koa.fzhhl.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fas.hnqzz.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://urd.316326.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://uoi.chenlongwang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zcl.fengsongda.top

Java: int add(int a, int b) { return a + b; }
来源：http://ntr.jqgfzy.top

Go:   func add(a, b int) int
来源：http://mbz.yangfankeji.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fma.jlsjyb.cn

C#:   int Add(int a, int b) => a + b;
来源：http://utj.fzhhl.top

[C14] 泛型函数
来源：http://zoy.guannengcc.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hla.guowangkeji.top

PHP:  // 无泛型
来源：http://ipx.nanxuanxn.top

JS:   // 无泛型
来源：http://enf.iojbl.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zqh.kuanghao11.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yeg.cucudq.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lyv.daria6918.cn

Ruby: # 无泛型
来源：http://noc.iojbl.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vby.guowangkeji.top

[C15] 解构 / 展开参数
来源：http://xqu.uphjek.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ggq.yueranfly.top

PHP:  [$a, $b] = $pair;
来源：http://jld.chenlongwang.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uas.shanyushiyangtech.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ghp.sxryk.cn

Java: // 无解构
来源：http://not.jinqigfzy.top

Go:   // 无解构
来源：http://rrf.sjlbkw.cn

Ruby: a, b = pair
来源：http://vzv.epnwcf.com

C#:   var (a, b) = pair;
来源：http://ljy.jianghu66.top

[C16] 函数 / 方法重载
来源：http://hre.0kj1m.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jgk.ctjpmb.com

PHP:  // 无重载
来源：http://jma.gaohongyu789.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ync.hesvh.cn

TS:   // 用联合类型或重载签名声明
来源：http://yli.9152youxi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jcy.mhx1999.top

Go:   // 无重载：用不同函数名
来源：http://fjt.chenlongwang.top

Ruby: # 无重载：靠动态参数
来源：http://pgd.aizwys.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://nst.quarkkingdee.top

================================================================================
来源：http://uzu.redwolf501.top

D. 数组 / 列表 / 集合
来源：http://awh.ivvv.top

================================================================================
来源：http://mtz.xinyue.icu

[D01] 创建数组 / 列表
来源：http://ctp.ybcxt.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://dna.52xcode.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qbm.dashuyun.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gpw.fktsv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://mmb.ywan-chungtsiang.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uaz.mhx1999.top

Go:   arr := []int{1, 2, 3}
来源：http://bfq.pengpengdd.cyou

Ruby: arr = [1, 2, 3]
来源：http://nhq.iojbl.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ums.snrcjt.cn

[D02] 追加元素到末尾
来源：http://sll.jlsjyb.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rcs.sxryk.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oeb.xinyue.icu

JS:   arr.push(4);
来源：http://coe.hongshengwenyu.top

TS:   arr.push(4);
来源：http://xrm.ivvv.top

Java: list.add(4);
来源：http://sem.tian-w.cn

Go:   arr = append(arr, 4)
来源：http://ufy.nwbrower.top

Ruby: arr << 4; arr.push(5)
来源：http://qry.wangshuangyany.cn

C#:   list.Add(4);
来源：http://mux.dianchejie.cn

[D03] 在指定位置插入元素
来源：http://abl.hywenlv.cn

Py:   arr.insert(0, 0)
来源：http://wou.hcnkem.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vhr.hongshengwenyu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cxw.hnxiangtu.top

TS:   arr.splice(0, 0, 0);
来源：http://qon.hfpthk.cn

Java: list.add(0, 0);
来源：http://jho.nwbrower.top

Go:   arr = append([]int{0}, arr...)
来源：http://hpp.zdqjudy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://acj.tianlin.xyz

C#:   list.Insert(0, 0);
来源：http://too.wangdashe.top

[D04] 删除元素
来源：http://rvj.cucudq.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://unj.dashuyun.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dhj.shanyushiyangkeji.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bwh.yangfankeji.com

TS:   arr.splice(0, 1);
来源：http://riw.dashuyun.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mcr.pengpengdd.cyou

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gpl.pycfn.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lgb.tianlin.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ycn.shanyushiyangtech.top

[D05] 访问与修改元素
来源：http://mys.gaohongyu789.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nbw.hcnkem.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fzq.tarul.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jja.guannengcc.top

TS:   arr[0]; arr.at(-1);
来源：http://yrw.yj20258.top

Java: list.get(0); list.set(0, 9);
来源：http://iiz.sweek.top

Go:   arr[0]; arr[0] = 9
来源：http://uvx.guowangkeji.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pbl.tianlin.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sdl.ydzc1.top

[D06] 数组长度
来源：http://uop.ydzc1.top

Py:   len(arr)
来源：http://cid.meibo888.top

PHP:  count($arr);
来源：http://tum.tianlin.xyz

JS:   arr.length
来源：http://bhq.tian-w.cn

TS:   arr.length
来源：http://rem.kuanghao11.cn

Java: list.size();
来源：http://evq.xinyue.icu

Go:   len(arr)
来源：http://uux.fanxiaobao.xyz

Ruby: arr.length; arr.size
来源：http://det.shanyushiyangtech.top

C#:   list.Count;
来源：http://eqd.hnxiangtu.top

[D07] 切片 / 取子数组
来源：http://owk.birdmap.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xut.jianghu66.top

PHP:  array_slice($arr, 1, 3);
来源：http://uze.fanxiaobao.xyz

JS:   arr.slice(1, 4);
来源：http://eks.guowangkeji.top

TS:   arr.slice(1, 4);
来源：http://igz.bbcook.cn

Java: list.subList(1, 4);
来源：http://uil.xinyue.icu

Go:   arr[1:4]
来源：http://frq.tian-w.cn

Ruby: arr[1, 3]
来源：http://lju.xziqi.cn

C#:   list.GetRange(1, 3);
来源：http://ndb.yvedp.cn

[D08] 合并两个数组
来源：http://man.jinghuilouyu.cn

Py:   a + b;  a.extend(b)
来源：http://jil.yueranfly.top

PHP:  array_merge($a, $b);
来源：http://mtz.tian-w.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://bpc.52xcode.cn

TS:   [...a, ...b];
来源：http://bvv.andypj.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zsf.ybcxt.top

Go:   append(a, b...)
来源：http://qfb.zhengqikj.top

Ruby: a + b;  a.concat(b)
来源：http://avz.uphjek.com

C#:   a.Concat(b).ToList()
来源：http://rrg.pengpengdd.cyou

[D09] 排序（升序）
来源：http://otk.sjlbkw.cn

Py:   sorted(arr);  arr.sort()
来源：http://msj.ydzc1.top

PHP:  sort($arr);
来源：http://hjb.guannengcc.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pkt.hcnkem.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://arb.shzxlz.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yre.andypj.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rzi.fzhhl.top

Ruby: arr.sort
来源：http://cww.guannengcc.top

C#:   list.Sort();
来源：http://yyb.fzhhl.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ohp.pengpengdd.cyou

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qea.zhongyouzk.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://evz.gotoacloud.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bjm.ydzc1.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mxl.hnqzz.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rno.hnxiangtu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pru.jyoumei.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wwq.cqqwz.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kff.guannengcc.top

[D11] 反转数组
来源：http://owf.yueranfly.top

Py:   arr[::-1];  arr.reverse()
来源：http://qyg.zdbjq.cn

PHP:  array_reverse($arr);
来源：http://ckh.daria6918.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rpo.chenlongwang.top

TS:   [...arr].reverse();
来源：http://aoi.redwolf501.top

Java: Collections.reverse(list);
来源：http://pfa.hammf.cn

Go:   slices.Reverse(arr)
来源：http://mxr.chenzaomai.com

Ruby: arr.reverse
来源：http://wxk.haohaochexian.top

C#:   list.Reverse();
来源：http://zli.jinyuanbaomall.cn

[D12] 查找元素下标
来源：http://tlu.fanxiaobao.xyz

Py:   arr.index(x);  x in arr
来源：http://ukf.fanxiaobao.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ehh.xinyue.icu

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gqw.fengsongda.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nxb.c1oappe.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gxh.ywan-chungtsiang.top

Go:   slices.Index(arr, x)
来源：http://lqy.cucudq.cn

Ruby: arr.index(x)
来源：http://ivk.pengpengdd.cyou

C#:   list.IndexOf(x);
来源：http://tko.meibo888.top

[D13] 过滤（保留满足条件的）
来源：http://ybf.zhongyouzk.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sdm.gzhubu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://iwg.cucudq.cn

JS:   arr.filter(x => x > 3)
来源：http://pmy.feifeiyinyue.top

TS:   arr.filter(x => x > 3)
来源：http://lov.shzxlz.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uxw.dashuyun.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cos.guowangkeji.top

Ruby: arr.select { |x| x > 3 }
来源：http://jls.yanxiufei.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ntd.gaohongyu789.top

[D14] 映射转换（每个元素变形）
来源：http://vgx.sufxvd.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ltl.yj202588.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tnb.shangyingyoupin.top

JS:   arr.map(x => x * 2)
来源：http://utc.mhx1999.top

TS:   arr.map(x => x * 2)
来源：http://mbx.cheryme.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://pst.fktsv.cn

Go:   // 手写循环
来源：http://frh.shanyushiyangtech.top

Ruby: arr.map { |x| x * 2 }
来源：http://trb.yuanzhike.top

C#:   list.Select(x => x * 2).ToList()
来源：http://mai.bjfxy.top

[D15] 去重
来源：http://lob.hongshengwenyu.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://otu.c1oappe.top

PHP:  array_unique($arr);
来源：http://urx.cashguo.top

JS:   [...new Set(arr)]
来源：http://bgd.ydzc1.top

TS:   [...new Set(arr)]
来源：http://qyn.jqgfzy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://eqp.cdnleiting.top

Go:   // 用 map[T]struct{} 手写
来源：http://yed.aizwys.cn

Ruby: arr.uniq
来源：http://hpt.zycfv.cn

C#:   list.Distinct().ToList()
来源：http://fxt.yfazqb.com

[D16] 求和与平均值
来源：http://hny.fzhhl.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mgm.yfazqb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wkb.jinqigufen.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ecm.jqgfzy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://flq.jlsjyb.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://enl.xinyue.icu

Go:   // 手写循环累加
来源：http://cri.jlsjyb.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wza.nanxuanxn.top

C#:   list.Sum();  list.Average()
来源：http://swx.chenjidiqi.icu

[D17] 最大值与最小值
来源：http://twc.zhongyouzk.top

Py:   max(arr);  min(arr)
来源：http://ebe.316326.xyz

PHP:  max($arr);  min($arr);
来源：http://cbu.aibaodan.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://enp.sjlbkw.cn

TS:   Math.max(...arr);
来源：http://rew.yangfankeji.com

Java: Collections.max(list);  Collections.min(list);
来源：http://jta.dashuyun.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wgk.sxryk.cn

Ruby: arr.max;  arr.min
来源：http://qne.feifeiyinyue.top

C#:   list.Max();  list.Min()
来源：http://oic.aizwys.cn

[D18] 扁平化嵌套数组
来源：http://eyb.zhiwuduotai.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ewl.ydzc1.top

PHP:  array_merge(...$nested);
来源：http://xtq.jinghuilouyu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://thq.316326.xyz

TS:   nested.flat();
来源：http://vdo.xuetiantiany.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hrf.guowangkeji.top

Go:   // 手写双层循环
来源：http://ecz.jlsjyb.cn

Ruby: nested.flatten
来源：http://ebo.jiagoushi.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://naj.yj202588.top


<!-- 参考信息 -->