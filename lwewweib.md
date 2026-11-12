代发 wailian999

Java: if (data == null) return;
来源：http://waq.zhijiandao.cn

Go:   if data == nil { return }
来源：http://mhn.cashguo.top

Ruby: return if data.nil?
来源：http://tmy.bbcook.cn

C#:   if (data == null) return;
来源：http://ztb.fehbvm.com

================================================================================
来源：http://wqj.hongshengwenyu.top

C. 函数与作用域
来源：http://qat.zhengqikj.top

================================================================================
来源：http://kkh.guannengcc.top

[C01] 定义函数
来源：http://oxy.yongpay.top

Py:   def add(a, b): return a + b
来源：http://pqx.pengpengdd.cyou

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cgv.jqgfzy.top

JS:   function add(a, b) { return a + b; }
来源：http://nbt.yvedp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eql.cqqwz.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://njc.zdqjudy.top

Go:   func add(a, b int) int { return a + b }
来源：http://yxt.hywenlv.cn

Ruby: def add(a, b); a + b; end
来源：http://hkm.epnwcf.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pmi.zhoulong.xyz

[C02] 默认参数
来源：http://jea.shzxlz.cn

Py:   def greet(name="World"): return name
来源：http://hxj.sxryk.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xtu.bjfxy.top

JS:   function greet(name = "World") { return name; }
来源：http://hwg.0kj1m.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yjp.dashuyun.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zbu.yj20258.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dnz.aizwys.cn

Ruby: def greet(name = "World") = name
来源：http://szl.meibo888.top

C#:   string Greet(string name = "World") => name;
来源：http://dkl.zdqjudy.top

[C03] 可变参数
来源：http://qul.zhoulong.xyz

Py:   def total(*args): return sum(args)
来源：http://ats.chenlongwang.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kdx.jinqigufen.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rgy.feifeiyinyue.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blh.tarul.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://axe.jinqigfzy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pjn.nanxinkj.top

Ruby: def total(*nums); nums.sum; end
来源：http://ogc.sufxvd.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qrs.jinqigufen.top

[C04] 命名参数 / 关键字参数
来源：http://xlj.jqgfzy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tqp.jqgfzy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ygk.jianghu66.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bud.snrcjt.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://did.yfazqb.com

Java: // 无：用 Builder 模式或 record
来源：http://ger.yanxiufei.cn

Go:   // 无：用配置结构体参数
来源：http://etj.sysykeji.top

Ruby: f(a: 1, b: 2)
来源：http://rem.tianlin.xyz

C#:   f(a: 1, b: 2)
来源：http://acr.316326.xyz

[C05] 返回多个值
来源：http://ult.jianghu66.top

Py:   return a, b
来源：http://zsf.jinqigfzy.top

PHP:  return [$a, $b];
来源：http://mqf.xingfuxueyuan.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://psp.aibaodan.cn

TS:   return { a, b };
来源：http://cqq.sxryk.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nei.ivvv.top

Go:   return a, b
来源：http://bap.gaohongyu789.top

Ruby: return a, b
来源：http://ire.shanyushiyangkeji.top

C#:   return (a, b);              // ValueTuple
来源：http://nau.nanxuanxn.top

[C06] 匿名函数 / lambda
来源：http://cqe.ydzc1.top

Py:   square = lambda x: x * x
来源：http://dxf.gotoacloud.top

PHP:  $square = fn($x) => $x * $x;
来源：http://qpx.fehbvm.com

JS:   const square = x => x * x;
来源：http://yzj.shanyushiyangkeji.top

TS:   const square = (x: number): number => x * x;
来源：http://zxb.shzxlz.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pcu.jinqigufen.top

Go:   sq := func(x int) int { return x * x }
来源：http://apx.nwbrower.top

Ruby: square = ->(x) { x * x }
来源：http://qij.gotoacloud.top

C#:   Func<int, int> square = x => x * x;
来源：http://kuu.yangfankeji.com

[C07] 把函数作为参数传入
来源：http://sbd.yueranfly.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://swv.nanxuanxn.top

PHP:  array_map("strtoupper", $arr);
来源：http://hjh.chenzaomai.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kgu.shzxlz.cn

TS:   arr.map(String)
来源：http://yyb.svipenyu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dgh.zhijiandao.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://del.gaohongyu789.top

Ruby: arr.map(&:upcase)
来源：http://fak.chenjidiqi.icu

C#:   arr.Select(s => s.ToUpper())
来源：http://zff.xziqi.cn

[C08] 闭包
来源：http://dsa.quarkkingdee.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rdw.yonumen.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lgj.sufxvd.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://prs.ehwqpu.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://upv.quarkkingdee.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://loz.tanke756.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mpo.fanxiaobao.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kgd.ehwqpu.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://avv.sufxvd.cn

[C09] 递归
来源：http://tjy.0kj1m.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hvn.zhoulong.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yry.nanxinkj.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sjn.jiagoushi.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://agj.xziqi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nhy.zhixingplan.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://oyt.chenjidiqi.icu

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vfn.yongpay.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mhy.zhengqikj.top

[C10] 变量作用域
来源：http://vci.xziqi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lhi.xinyue.icu

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://sad.jinghuilouyu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fab.zdqjudy.top

TS:   同 JS
来源：http://ssp.gaohongyu789.top

Java: 方法内为块级作用域
来源：http://aow.hesvh.cn

Go:   花括号块级作用域
来源：http://trz.aibaodan.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kec.shanyushiyangtech.top

C#:   块级作用域
来源：http://skv.zhiwuduotai.top

[C11] 模块导入与导出
来源：http://cgx.yj20258888.top

Py:   from module import func
来源：http://led.vqdsnc.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://jbn.cqqwz.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://brr.52xcode.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://czp.yangfankeji.com

Java: import java.util.List;
来源：http://ovn.yuxming.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gum.cdnleiting.top

Ruby: require "json"; require_relative "./util"
来源：http://tqy.yanxiufei.cn

C#:   using System.Text;
来源：http://vdh.yuanzhike.top

[C12] 立即执行函数 IIFE
来源：http://nht.bjfxy.top

Py:   (lambda: print("run"))()
来源：http://pcx.yanxiufei.cn

PHP:  (function () { echo "run"; })();
来源：http://mlh.yanxiufei.cn

JS:   (() => { console.log("run"); })();
来源：http://bdq.xingfuxueyuan.xyz

TS:   (() => { console.log("run"); })();
来源：http://ids.chenlongwang.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nnq.fanxiaobao.xyz

Go:   func() { fmt.Println("run") }()
来源：http://xwf.vehdjk.com

Ruby: -> { puts "run" }.call
来源：http://tko.yanxiufei.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mza.xziqi.cn

[C13] 类型声明 / 类型注解
来源：http://qsz.zhongyouzk.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pve.fzhhl.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://loa.shangyingyoupin.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zpu.tian-w.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hty.chenlongwang.top

Java: int add(int a, int b) { return a + b; }
来源：http://tpn.jinqigfzy.top

Go:   func add(a, b int) int
来源：http://abe.jiagoushi.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://neh.ppjwa.cn

C#:   int Add(int a, int b) => a + b;
来源：http://thc.snrcjt.cn

[C14] 泛型函数
来源：http://iam.iojbl.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ckh.nwbrower.top

PHP:  // 无泛型
来源：http://wlh.shuidangran.top

JS:   // 无泛型
来源：http://jzu.zhixingplan.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fho.aibaodan.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jeq.pycfn.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lfk.xinyue.icu

Ruby: # 无泛型
来源：http://elb.kuanghao11.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mez.yj20258888.top

[C15] 解构 / 展开参数
来源：http://sol.bbcook.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rir.uphjek.com

PHP:  [$a, $b] = $pair;
来源：http://xhu.vehdjk.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://oro.hcnkem.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tpn.fengsongda.top

Java: // 无解构
来源：http://kks.daxiang520.top

Go:   // 无解构
来源：http://anz.xziqi.cn

Ruby: a, b = pair
来源：http://anh.zdqjudy.top

C#:   var (a, b) = pair;
来源：http://jwm.xingfuxueyuan.xyz

[C16] 函数 / 方法重载
来源：http://xph.haohaochexian.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wpw.cheryme.top

PHP:  // 无重载
来源：http://ppo.hnqzz.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ilp.gogol.net.cn

TS:   // 用联合类型或重载签名声明
来源：http://ppd.jinqigfzy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://qcn.nanxuanxn.top

Go:   // 无重载：用不同函数名
来源：http://vkt.tanke756.top

Ruby: # 无重载：靠动态参数
来源：http://ttr.hammf.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://spr.bjfxy.top

================================================================================
来源：http://vew.tian-w.cn

D. 数组 / 列表 / 集合
来源：http://csh.fzhhl.top

================================================================================
来源：http://jws.ivvv.top

[D01] 创建数组 / 列表
来源：http://grz.jinqigfzy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://mag.zhaomingkeji.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dmd.snrcjt.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dcs.vqdsnc.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bfo.xylfe.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cwl.redwolf501.top

Go:   arr := []int{1, 2, 3}
来源：http://ecl.jlsjyb.cn

Ruby: arr = [1, 2, 3]
来源：http://kuf.jiagoushi.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wtl.xingfuxueyuan.xyz

[D02] 追加元素到末尾
来源：http://vzb.cqqwz.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://umz.chenzaomai.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lpb.havefunace.top

JS:   arr.push(4);
来源：http://xeg.yj20258.top

TS:   arr.push(4);
来源：http://ucg.iojbl.cn

Java: list.add(4);
来源：http://spf.shuidangran.top

Go:   arr = append(arr, 4)
来源：http://hpm.mhx1999.top

Ruby: arr << 4; arr.push(5)
来源：http://ugz.shangyingyoupin.top

C#:   list.Add(4);
来源：http://jxa.xinyue.icu

[D03] 在指定位置插入元素
来源：http://vwo.birdmap.top

Py:   arr.insert(0, 0)
来源：http://dxm.aibaodan.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uzr.xuetiantiany.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xcx.daria6918.cn

TS:   arr.splice(0, 0, 0);
来源：http://ulc.cheryme.top

Java: list.add(0, 0);
来源：http://hys.hongshengwenyu.top

Go:   arr = append([]int{0}, arr...)
来源：http://qtn.9152youxi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wwp.jiagoushi.top

C#:   list.Insert(0, 0);
来源：http://umj.shanyushiyangtech.top

[D04] 删除元素
来源：http://mjf.epnwcf.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qgo.xinyue.icu

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xaq.sjlbkw.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xyl.9152youxi.cn

TS:   arr.splice(0, 1);
来源：http://khf.xuanzx.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fbv.haohaochexian.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hfx.wangdashe.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://npk.yj202588.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wdm.zdqjudy.top

[D05] 访问与修改元素
来源：http://fkt.jqgfzy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zvm.birdmap.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mmq.jqgufenzy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mrj.kuanghao11.cn

TS:   arr[0]; arr.at(-1);
来源：http://ogd.smart0.xyz

Java: list.get(0); list.set(0, 9);
来源：http://drl.gotoacloud.top

Go:   arr[0]; arr[0] = 9
来源：http://tnc.ywan-chungtsiang.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fbm.zhaomingkeji.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://eaz.jqgufenzy.top

[D06] 数组长度
来源：http://hnk.shuidangran.top

Py:   len(arr)
来源：http://fcm.yongpay.top

PHP:  count($arr);
来源：http://caq.ivvv.top

JS:   arr.length
来源：http://htk.nanxinkj.top

TS:   arr.length
来源：http://xsf.xinyue.icu

Java: list.size();
来源：http://csa.wangdashe.top

Go:   len(arr)
来源：http://bot.sysykeji.top

Ruby: arr.length; arr.size
来源：http://gun.zycfv.cn

C#:   list.Count;
来源：http://voh.pycfn.com

[D07] 切片 / 取子数组
来源：http://zqh.wangdashe.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ebp.zhixingplan.top

PHP:  array_slice($arr, 1, 3);
来源：http://mck.yfazqb.com

JS:   arr.slice(1, 4);
来源：http://uuh.hongshengwenyu.top

TS:   arr.slice(1, 4);
来源：http://igt.bbcook.cn

Java: list.subList(1, 4);
来源：http://veb.guowangkeji.top

Go:   arr[1:4]
来源：http://nbi.redwolf501.top

Ruby: arr[1, 3]
来源：http://eie.ivvv.top

C#:   list.GetRange(1, 3);
来源：http://frz.hywenlv.cn

[D08] 合并两个数组
来源：http://ejh.hnqzz.top

Py:   a + b;  a.extend(b)
来源：http://xkf.haohaochexian.top

PHP:  array_merge($a, $b);
来源：http://omb.tian-w.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gmh.hysaishi.cn

TS:   [...a, ...b];
来源：http://kok.yj20258888.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yfp.snrcjt.cn

Go:   append(a, b...)
来源：http://dfk.jqgfzy.top

Ruby: a + b;  a.concat(b)
来源：http://bsw.zhaomingkeji.xyz

C#:   a.Concat(b).ToList()
来源：http://lok.hysaishi.cn

[D09] 排序（升序）
来源：http://ntt.vqdsnc.cn

Py:   sorted(arr);  arr.sort()
来源：http://lfp.pengpengdd.cyou

PHP:  sort($arr);
来源：http://eso.bbcook.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zuz.cheryme.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://xsv.yvedp.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gfn.zhiwuduotai.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yqu.gogol.net.cn

Ruby: arr.sort
来源：http://dyz.nanxuanxn.top

C#:   list.Sort();
来源：http://dbk.bjfxy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ery.smart0.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://huh.yangfankeji.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ywv.meibo888.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://typ.daxiang520.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://act.jqgfzy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dyh.tian-w.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qxy.jlsjyb.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kkr.fengsongda.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dpc.fehbvm.com

[D11] 反转数组
来源：http://waf.xuanzx.com

Py:   arr[::-1];  arr.reverse()
来源：http://vab.xuetiantiany.cn

PHP:  array_reverse($arr);
来源：http://axs.yonumen.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://avd.daxiang520.top

TS:   [...arr].reverse();
来源：http://rmz.yangfankeji.com

Java: Collections.reverse(list);
来源：http://xbk.nanxuanxn.top

Go:   slices.Reverse(arr)
来源：http://umi.fengsongda.top

Ruby: arr.reverse
来源：http://kzq.jlsjyb.cn

C#:   list.Reverse();
来源：http://hdz.zhoulong.xyz

[D12] 查找元素下标
来源：http://uqb.bjfxy.top

Py:   arr.index(x);  x in arr
来源：http://jqn.yonumen.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uax.sweek.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://exf.iojbl.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zgr.daxiang520.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dmc.shanyushiyangkeji.top

Go:   slices.Index(arr, x)
来源：http://kjs.yj20258888.top

Ruby: arr.index(x)
来源：http://rqv.yj20258888.top

C#:   list.IndexOf(x);
来源：http://djj.shanyushiyangtech.top

[D13] 过滤（保留满足条件的）
来源：http://vqh.fzhhl.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yhg.vehdjk.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mpy.ybcxt.top

JS:   arr.filter(x => x > 3)
来源：http://tkt.zhiwuduotai.top

TS:   arr.filter(x => x > 3)
来源：http://dwz.hfpthk.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xxg.gogol.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bsf.jiagoushi.top

Ruby: arr.select { |x| x > 3 }
来源：http://ttw.zhengqikj.top

C#:   list.Where(x => x > 3).ToList()
来源：http://gcp.yonumen.top

[D14] 映射转换（每个元素变形）
来源：http://wcu.cqqwz.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yca.jinqigfzy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://csm.birdmap.top

JS:   arr.map(x => x * 2)
来源：http://sst.zhijiandao.cn

TS:   arr.map(x => x * 2)
来源：http://gkr.nwbrower.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://zej.svipenyu.cn

Go:   // 手写循环
来源：http://fhq.quarkkingdee.top

Ruby: arr.map { |x| x * 2 }
来源：http://dos.meibo888.top

C#:   list.Select(x => x * 2).ToList()
来源：http://rux.zdbjq.cn

[D15] 去重
来源：http://auq.shuidangran.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nbp.epnwcf.com

PHP:  array_unique($arr);
来源：http://vpa.aibaodan.cn

JS:   [...new Set(arr)]
来源：http://bwt.yj202588.top

TS:   [...new Set(arr)]
来源：http://spo.9152youxi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fdq.tianlin.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://byo.meibo888.top

Ruby: arr.uniq
来源：http://tsw.yfazqb.com

C#:   list.Distinct().ToList()
来源：http://nti.shzxlz.cn

[D16] 求和与平均值
来源：http://ptg.yueranfly.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vdf.bjfxy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pqr.fzhhl.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://orb.xuanzx.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://skd.yvedp.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yni.nanxuanxn.top

Go:   // 手写循环累加
来源：http://ylb.aibaodan.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ixb.hywenlv.cn

C#:   list.Sum();  list.Average()
来源：http://lfn.shzxlz.cn

[D17] 最大值与最小值
来源：http://jtc.yueranfly.top

Py:   max(arr);  min(arr)
来源：http://tig.cheryme.top


<!-- 参考信息 -->