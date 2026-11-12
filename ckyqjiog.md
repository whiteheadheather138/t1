代发 wailian999

PHP:  $a && $b || !$c
来源：http://fhh.yanxiufei.cn

JS:   a && b || !c
来源：http://lcz.gogol.net.cn

TS:   a && b || !c
来源：http://emq.guannengcc.top

Java: a && b || !c
来源：http://pwv.jyoumei.cn

Go:   a && b || !c
来源：http://hdz.zhoulong.xyz

Ruby: a && b || !c
来源：http://nsv.sufxvd.cn

C#:   a && b || !c
来源：http://xdv.cucudq.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vsm.havefunace.top

Py:   if not data: return
来源：http://etg.jqgufenzy.top

PHP:  if (!$data) { return; }
来源：http://yaf.feifeiyinyue.top

JS:   if (!data) return;
来源：http://wxt.zhengqikj.top

TS:   if (!data) return;
来源：http://kmv.hesvh.cn

Java: if (data == null) return;
来源：http://ybn.meibo888.top

Go:   if data == nil { return }
来源：http://gfs.yongpay.top

Ruby: return if data.nil?
来源：http://zci.shangyingyoupin.top

C#:   if (data == null) return;
来源：http://urp.gotoacloud.top

================================================================================
来源：http://kkv.ehwqpu.com

C. 函数与作用域
来源：http://tca.hesvh.cn

================================================================================
来源：http://rkd.nanxuanxn.top

[C01] 定义函数
来源：http://btv.chenlongwang.top

Py:   def add(a, b): return a + b
来源：http://lzs.chenzaomai.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ajs.zhijiandao.cn

JS:   function add(a, b) { return a + b; }
来源：http://cuh.zhiwuduotai.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pon.0kj1m.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qmm.jlsjyb.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ggy.chenzaomai.com

Ruby: def add(a, b); a + b; end
来源：http://vdq.nwbrower.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xox.guannengcc.top

[C02] 默认参数
来源：http://rwm.zhoulong.xyz

Py:   def greet(name="World"): return name
来源：http://oyp.cheryme.top

PHP:  function greet($name = "World") { return $name; }
来源：http://wmn.hcnkem.com

JS:   function greet(name = "World") { return name; }
来源：http://inb.xinyue.icu

TS:   function greet(name: string = "World") { return name; }
来源：http://ejz.chenjidiqi.icu

Java: // 无默认参数：方法重载或 Optional
来源：http://lcu.yueranfly.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wzb.xinyue.icu

Ruby: def greet(name = "World") = name
来源：http://chr.feifeiyinyue.top

C#:   string Greet(string name = "World") => name;
来源：http://bdv.fehbvm.com

[C03] 可变参数
来源：http://hxy.zhaomingkeji.xyz

Py:   def total(*args): return sum(args)
来源：http://ztd.zycfv.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nom.zhiwuduotai.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fzj.wangshuangyany.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://eht.nwbrower.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://omm.shzxlz.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uqf.zdbjq.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kjp.jianghu66.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xcf.ywan-chungtsiang.top

[C04] 命名参数 / 关键字参数
来源：http://jst.hnqzz.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hbe.yuxming.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tdg.chenlongwang.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jqc.ywan-chungtsiang.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tqf.wangdashe.top

Java: // 无：用 Builder 模式或 record
来源：http://ltc.hongshengwenyu.top

Go:   // 无：用配置结构体参数
来源：http://sld.yfazqb.com

Ruby: f(a: 1, b: 2)
来源：http://eok.sxryk.cn

C#:   f(a: 1, b: 2)
来源：http://oku.yfazqb.com

[C05] 返回多个值
来源：http://oyz.52xcode.cn

Py:   return a, b
来源：http://zyf.haohaochexian.top

PHP:  return [$a, $b];
来源：http://eip.kuanghao11.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yyy.bjfxy.top

TS:   return { a, b };
来源：http://zfa.ehwqpu.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://uqg.zhaomingkeji.xyz

Go:   return a, b
来源：http://jyt.gaohongyu789.top

Ruby: return a, b
来源：http://rwn.cheryme.top

C#:   return (a, b);              // ValueTuple
来源：http://mhu.hnqzz.top

[C06] 匿名函数 / lambda
来源：http://yrs.gogol.net.cn

Py:   square = lambda x: x * x
来源：http://jfk.nwbrower.top

PHP:  $square = fn($x) => $x * $x;
来源：http://obc.meibo888.top

JS:   const square = x => x * x;
来源：http://jcb.aibaodan.cn

TS:   const square = (x: number): number => x * x;
来源：http://fzq.nwbrower.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://msu.svipenyu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://iyi.hnqzz.top

Ruby: square = ->(x) { x * x }
来源：http://nga.gogol.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ipo.yanxiufei.cn

[C07] 把函数作为参数传入
来源：http://yur.hfpthk.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://uii.zhongyouzk.top

PHP:  array_map("strtoupper", $arr);
来源：http://wqv.xziqi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hmh.zycfv.cn

TS:   arr.map(String)
来源：http://osl.redwolf501.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ovc.dashuyun.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rod.316326.xyz

Ruby: arr.map(&:upcase)
来源：http://gll.sufxvd.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pbn.jlsjyb.cn

[C08] 闭包
来源：http://qtf.316326.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://luo.xziqi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fcg.dianchejie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://aob.yueranfly.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hqq.shuidangran.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xwv.aibaodan.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rkh.pengpengdd.cyou

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uqn.9152youxi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zyz.yfazqb.com

[C09] 递归
来源：http://cnb.fehbvm.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bjv.mhx1999.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zbq.mhx1999.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dac.redwolf501.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zow.gotoacloud.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ksp.jyoumei.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cua.shanyushiyangtech.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ldo.cucudq.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pau.xuanzx.com

[C10] 变量作用域
来源：http://zhl.jqgufenzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://for.jiagoushi.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lzg.jqgufenzy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zgd.bbcook.cn

TS:   同 JS
来源：http://vgc.xinyue.icu

Java: 方法内为块级作用域
来源：http://ntq.meibo888.top

Go:   花括号块级作用域
来源：http://njv.uphjek.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hws.xziqi.cn

C#:   块级作用域
来源：http://lsu.jlsjyb.cn

[C11] 模块导入与导出
来源：http://rdp.hongshengwenyu.top

Py:   from module import func
来源：http://bgx.dashuyun.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://cdr.ehwqpu.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://qed.yueranfly.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zqj.uphjek.com

Java: import java.util.List;
来源：http://fct.hammf.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wda.birdmap.top

Ruby: require "json"; require_relative "./util"
来源：http://nvh.316326.xyz

C#:   using System.Text;
来源：http://yzv.yvedp.cn

[C12] 立即执行函数 IIFE
来源：http://yfx.yj20258888.top

Py:   (lambda: print("run"))()
来源：http://kca.ehwqpu.com

PHP:  (function () { echo "run"; })();
来源：http://ggi.hnxiangtu.top

JS:   (() => { console.log("run"); })();
来源：http://bee.52xcode.cn

TS:   (() => { console.log("run"); })();
来源：http://heh.epnwcf.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://aua.yfazqb.com

Go:   func() { fmt.Println("run") }()
来源：http://dbh.jinqigfzy.top

Ruby: -> { puts "run" }.call
来源：http://pud.snrcjt.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ozm.epnwcf.com

[C13] 类型声明 / 类型注解
来源：http://ppe.316326.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gka.wangshuangyany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vvw.daxiang520.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kja.hnxiangtu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ukn.jqgufenzy.top

Java: int add(int a, int b) { return a + b; }
来源：http://tzk.mhx1999.top

Go:   func add(a, b int) int
来源：http://bdw.zhixingplan.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ypx.zdbjq.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ruj.nanxuanxn.top

[C14] 泛型函数
来源：http://fbh.zdqjudy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fkl.haohaochexian.top

PHP:  // 无泛型
来源：http://pwl.zhoulong.xyz

JS:   // 无泛型
来源：http://jyu.hcnkem.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uqz.tian-w.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gac.jinyuanbaomall.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ppw.zhiwuduotai.top

Ruby: # 无泛型
来源：http://ple.yuanzhike.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://erc.fehbvm.com

[C15] 解构 / 展开参数
来源：http://grz.shangyingyoupin.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dvo.shangyingyoupin.top

PHP:  [$a, $b] = $pair;
来源：http://qkm.hnqzz.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://puh.aibaodan.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ncd.tian-w.cn

Java: // 无解构
来源：http://mtv.zhiwuduotai.top

Go:   // 无解构
来源：http://ucn.0kj1m.cn

Ruby: a, b = pair
来源：http://sqe.pycfn.com

C#:   var (a, b) = pair;
来源：http://cav.guannengcc.top

[C16] 函数 / 方法重载
来源：http://tkh.yj20258888.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wvv.jyoumei.cn

PHP:  // 无重载
来源：http://emo.xinyue.icu

JS:   // 无重载：靠 arguments.length 分支
来源：http://nif.xuanzx.com

TS:   // 用联合类型或重载签名声明
来源：http://axg.pengpengdd.cyou

Java: void f(int a) {}  void f(String a) {}
来源：http://wja.aizwys.cn

Go:   // 无重载：用不同函数名
来源：http://nzc.meibo888.top

Ruby: # 无重载：靠动态参数
来源：http://vhm.sweek.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://gpe.cheryme.top

================================================================================
来源：http://uwk.hammf.cn

D. 数组 / 列表 / 集合
来源：http://lnj.yj20258888.top

================================================================================
来源：http://gnh.fktsv.cn

[D01] 创建数组 / 列表
来源：http://ybf.pengpengdd.cyou

Py:   arr = [1, 2, 3];  empty = []
来源：http://eob.jinyuanbaomall.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://scr.nanxinkj.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xmq.jinqigufen.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://pwj.chenjidiqi.icu

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xjr.hysaishi.cn

Go:   arr := []int{1, 2, 3}
来源：http://rld.cheryme.top

Ruby: arr = [1, 2, 3]
来源：http://rld.xuanzx.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mbf.ehwqpu.com

[D02] 追加元素到末尾
来源：http://zrf.cdnleiting.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ekr.yvedp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hin.yuanzhike.top

JS:   arr.push(4);
来源：http://cil.zdbjq.cn

TS:   arr.push(4);
来源：http://mzz.fehbvm.com

Java: list.add(4);
来源：http://ohp.sxryk.cn

Go:   arr = append(arr, 4)
来源：http://vsg.andypj.xyz

Ruby: arr << 4; arr.push(5)
来源：http://vzp.havefunace.top

C#:   list.Add(4);
来源：http://fyt.hnqzz.top

[D03] 在指定位置插入元素
来源：http://xwn.ppjwa.cn

Py:   arr.insert(0, 0)
来源：http://jkn.yueranfly.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zsu.ywan-chungtsiang.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://htm.zycfv.cn

TS:   arr.splice(0, 0, 0);
来源：http://bkz.jyoumei.cn

Java: list.add(0, 0);
来源：http://vyp.yanxiufei.cn

Go:   arr = append([]int{0}, arr...)
来源：http://lvx.havefunace.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://npl.zhiwuduotai.top

C#:   list.Insert(0, 0);
来源：http://unt.tian-w.cn

[D04] 删除元素
来源：http://qba.bjfxy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ygh.andypj.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pat.cashguo.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dbi.uphjek.com

TS:   arr.splice(0, 1);
来源：http://ggj.yueranfly.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zlj.jiagoushi.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dqw.tanke756.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mdd.aibaodan.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lqq.tarul.cn

[D05] 访问与修改元素
来源：http://aer.pycfn.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://iqk.wangdashe.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://paj.vehdjk.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lgt.jlsjyb.cn

TS:   arr[0]; arr.at(-1);
来源：http://shm.dashuyun.cn

Java: list.get(0); list.set(0, 9);
来源：http://jqq.svipenyu.cn

Go:   arr[0]; arr[0] = 9
来源：http://qpj.sxryk.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tce.iojbl.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ace.gotoacloud.top

[D06] 数组长度
来源：http://kvt.sweek.top

Py:   len(arr)
来源：http://jtb.zhixingplan.top

PHP:  count($arr);
来源：http://tgt.redwolf501.top

JS:   arr.length
来源：http://lha.shanyushiyangtech.top

TS:   arr.length
来源：http://zur.guannengcc.top

Java: list.size();
来源：http://lrs.haohaochexian.top

Go:   len(arr)
来源：http://ebj.sweek.top

Ruby: arr.length; arr.size
来源：http://hbt.xingfuxueyuan.xyz

C#:   list.Count;
来源：http://kob.sweek.top

[D07] 切片 / 取子数组
来源：http://ohu.ywan-chungtsiang.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qek.hongshengwenyu.top

PHP:  array_slice($arr, 1, 3);
来源：http://lri.xinyue.icu

JS:   arr.slice(1, 4);
来源：http://ula.cucudq.cn

TS:   arr.slice(1, 4);
来源：http://ozb.bbcook.cn

Java: list.subList(1, 4);
来源：http://gsu.jinghuilouyu.cn

Go:   arr[1:4]
来源：http://wit.zhijiandao.cn

Ruby: arr[1, 3]
来源：http://bfx.nanxuanxn.top

C#:   list.GetRange(1, 3);
来源：http://rzo.nanxuanxn.top

[D08] 合并两个数组
来源：http://qwd.iojbl.cn

Py:   a + b;  a.extend(b)
来源：http://bni.quarkkingdee.top

PHP:  array_merge($a, $b);
来源：http://fnh.aizwys.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://dat.kuanghao11.cn

TS:   [...a, ...b];
来源：http://voz.cheryme.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lzh.meibo888.top

Go:   append(a, b...)
来源：http://wsx.fanxiaobao.xyz

Ruby: a + b;  a.concat(b)
来源：http://nuk.jqgfzy.top

C#:   a.Concat(b).ToList()
来源：http://kug.shangyingyoupin.top

[D09] 排序（升序）
来源：http://zyz.hnxiangtu.top

Py:   sorted(arr);  arr.sort()
来源：http://lkm.0kj1m.cn

PHP:  sort($arr);
来源：http://vmn.chenjidiqi.icu

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://knk.yongpay.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://vqz.cucudq.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yzv.shuidangran.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dgj.jiagoushi.top

Ruby: arr.sort
来源：http://wbn.cdnleiting.top

C#:   list.Sort();
来源：http://dvu.aibaodan.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://oaw.guowangkeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vij.cashguo.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xwz.havefunace.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tnn.havefunace.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://suz.0kj1m.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jfz.yj20258.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jyu.ppjwa.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ujb.andypj.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vce.316326.xyz

[D11] 反转数组
来源：http://euj.pycfn.com

Py:   arr[::-1];  arr.reverse()
来源：http://fvk.xuanzx.com

PHP:  array_reverse($arr);
来源：http://mue.sjlbkw.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rkl.cucudq.cn

TS:   [...arr].reverse();
来源：http://cam.hongshengwenyu.top

Java: Collections.reverse(list);
来源：http://gdr.sjlbkw.cn

Go:   slices.Reverse(arr)
来源：http://ort.sxryk.cn

Ruby: arr.reverse
来源：http://jie.nanxinkj.top

C#:   list.Reverse();
来源：http://tqy.zdqjudy.top

[D12] 查找元素下标
来源：http://usl.jinghuilouyu.cn

Py:   arr.index(x);  x in arr
来源：http://diy.zdbjq.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sbz.gotoacloud.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://igr.c1oappe.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nur.c1oappe.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://epk.yuxming.cn

Go:   slices.Index(arr, x)
来源：http://pvv.ehwqpu.com

Ruby: arr.index(x)
来源：http://uoe.cucudq.cn

C#:   list.IndexOf(x);
来源：http://tiv.xziqi.cn

[D13] 过滤（保留满足条件的）
来源：http://slx.zhijiandao.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pwo.guowangkeji.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bnt.gogol.net.cn

JS:   arr.filter(x => x > 3)
来源：http://qrc.sysykeji.top

TS:   arr.filter(x => x > 3)
来源：http://htf.andypj.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uvj.sxryk.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qvf.kuanghao11.cn

Ruby: arr.select { |x| x > 3 }
来源：http://apg.jinghuilouyu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://iim.mhx1999.top

[D14] 映射转换（每个元素变形）
来源：http://mka.cucudq.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ayb.birdmap.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nts.cucudq.cn

JS:   arr.map(x => x * 2)
来源：http://qen.kuanghao11.cn

TS:   arr.map(x => x * 2)
来源：http://wbz.gotoacloud.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://wfp.xziqi.cn

Go:   // 手写循环
来源：http://scs.zhaomingkeji.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://uwc.ywan-chungtsiang.top

C#:   list.Select(x => x * 2).ToList()
来源：http://iln.zdbjq.cn

[D15] 去重
来源：http://kdc.zhongyouzk.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vox.jqgfzy.top

PHP:  array_unique($arr);
来源：http://jrn.fengsongda.top

JS:   [...new Set(arr)]
来源：http://qnv.wangdashe.top

TS:   [...new Set(arr)]
来源：http://lbq.zdbjq.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ktf.yonumen.top

Go:   // 用 map[T]struct{} 手写
来源：http://yhr.hnxiangtu.top

Ruby: arr.uniq
来源：http://tns.yuanzhike.top


<!-- 参考信息 -->