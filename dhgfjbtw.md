代发 wailian999

================================================================================
来源：http://ufm.guowangkeji.top

C. 函数与作用域
来源：http://eja.hnqzz.top

================================================================================
来源：http://prz.ehwqpu.com

[C01] 定义函数
来源：http://jsy.sysykeji.top

Py:   def add(a, b): return a + b
来源：http://cpc.xuetiantiany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qmy.kuanghao11.cn

JS:   function add(a, b) { return a + b; }
来源：http://qke.yj20258.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://npj.pengpengdd.cyou

Java: static int add(int a, int b) { return a + b; }
来源：http://prf.uphjek.com

Go:   func add(a, b int) int { return a + b }
来源：http://ldu.ywan-chungtsiang.top

Ruby: def add(a, b); a + b; end
来源：http://bhh.yvedp.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qqj.kuanghao11.cn

[C02] 默认参数
来源：http://ayr.xinyue.icu

Py:   def greet(name="World"): return name
来源：http://xqr.yvedp.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zno.0kj1m.cn

JS:   function greet(name = "World") { return name; }
来源：http://kfx.yj202588.top

TS:   function greet(name: string = "World") { return name; }
来源：http://hly.feifeiyinyue.top

Java: // 无默认参数：方法重载或 Optional
来源：http://eyq.iojbl.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qef.sxryk.cn

Ruby: def greet(name = "World") = name
来源：http://oji.hysaishi.cn

C#:   string Greet(string name = "World") => name;
来源：http://qpn.fzhhl.top

[C03] 可变参数
来源：http://xrh.jinqigufen.top

Py:   def total(*args): return sum(args)
来源：http://mun.ybcxt.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vjc.shanyushiyangkeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pbc.andypj.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qxd.sysykeji.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hkw.sufxvd.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ywz.shzxlz.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fvh.yuanzhike.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qyy.sufxvd.cn

[C04] 命名参数 / 关键字参数
来源：http://kyv.zdqjudy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jct.quarkkingdee.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ayf.zhijiandao.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yjc.haohaochexian.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jpn.aizwys.cn

Java: // 无：用 Builder 模式或 record
来源：http://hab.kuanghao11.cn

Go:   // 无：用配置结构体参数
来源：http://ujc.52xcode.cn

Ruby: f(a: 1, b: 2)
来源：http://rgp.gzhubu.top

C#:   f(a: 1, b: 2)
来源：http://yac.zycfv.cn

[C05] 返回多个值
来源：http://ahy.andypj.xyz

Py:   return a, b
来源：http://dta.andypj.xyz

PHP:  return [$a, $b];
来源：http://qnv.gaohongyu789.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://opn.svipenyu.cn

TS:   return { a, b };
来源：http://tbc.guannengcc.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://owy.hnqzz.top

Go:   return a, b
来源：http://ekc.yj20258.top

Ruby: return a, b
来源：http://mkk.fanxiaobao.xyz

C#:   return (a, b);              // ValueTuple
来源：http://bkn.zhongyouzk.top

[C06] 匿名函数 / lambda
来源：http://mns.xziqi.cn

Py:   square = lambda x: x * x
来源：http://xht.chenzaomai.com

PHP:  $square = fn($x) => $x * $x;
来源：http://lgj.sysykeji.top

JS:   const square = x => x * x;
来源：http://bru.cucudq.cn

TS:   const square = (x: number): number => x * x;
来源：http://swj.zhoulong.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yfh.jinyuanbaomall.cn

Go:   sq := func(x int) int { return x * x }
来源：http://khv.yj20258888.top

Ruby: square = ->(x) { x * x }
来源：http://zpp.xuetiantiany.cn

C#:   Func<int, int> square = x => x * x;
来源：http://uwr.chenzaomai.com

[C07] 把函数作为参数传入
来源：http://rpx.xylfe.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yuw.nwbrower.top

PHP:  array_map("strtoupper", $arr);
来源：http://jlt.tarul.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nny.jianghu66.top

TS:   arr.map(String)
来源：http://ycc.cdnleiting.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jwf.zhaomingkeji.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hel.xziqi.cn

Ruby: arr.map(&:upcase)
来源：http://ruv.zhixingplan.top

C#:   arr.Select(s => s.ToUpper())
来源：http://muz.yonumen.top

[C08] 闭包
来源：http://blt.jiagoushi.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cpw.zdbjq.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://icx.feifeiyinyue.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pbp.fzhhl.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fhp.gotoacloud.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hkp.hnxiangtu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://uoc.tianlin.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zdo.guowangkeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jzt.andypj.xyz

[C09] 递归
来源：http://wzd.hfpthk.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uek.c1oappe.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kmc.hywenlv.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://smb.zycfv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qbl.nanxinkj.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ubu.fktsv.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vwr.tian-w.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ppr.yfazqb.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gax.jlsjyb.cn

[C10] 变量作用域
来源：http://vya.ctjpmb.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nyj.c1oappe.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xvb.zycfv.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qhf.ybcxt.top

TS:   同 JS
来源：http://xud.zhijiandao.cn

Java: 方法内为块级作用域
来源：http://xqp.tarul.cn

Go:   花括号块级作用域
来源：http://oik.ywan-chungtsiang.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nrt.tian-w.cn

C#:   块级作用域
来源：http://wgk.aizwys.cn

[C11] 模块导入与导出
来源：http://zvx.redwolf501.top

Py:   from module import func
来源：http://ehp.iojbl.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://sgu.cucudq.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zpy.daxiang520.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qum.yfazqb.com

Java: import java.util.List;
来源：http://pxz.zhiwuduotai.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bft.shuidangran.top

Ruby: require "json"; require_relative "./util"
来源：http://ilh.jianghu66.top

C#:   using System.Text;
来源：http://dpm.yonumen.top

[C12] 立即执行函数 IIFE
来源：http://rfl.jinyuanbaomall.cn

Py:   (lambda: print("run"))()
来源：http://efi.jqgufenzy.top

PHP:  (function () { echo "run"; })();
来源：http://jnd.mhx1999.top

JS:   (() => { console.log("run"); })();
来源：http://efb.sufxvd.cn

TS:   (() => { console.log("run"); })();
来源：http://yxh.vehdjk.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nbz.snrcjt.cn

Go:   func() { fmt.Println("run") }()
来源：http://oye.xziqi.cn

Ruby: -> { puts "run" }.call
来源：http://mxr.svipenyu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://kjl.jlsjyb.cn

[C13] 类型声明 / 类型注解
来源：http://ehn.yueranfly.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vqn.zhixingplan.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xgw.xylfe.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ark.jqgufenzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fvg.guannengcc.top

Java: int add(int a, int b) { return a + b; }
来源：http://dyz.chenjidiqi.icu

Go:   func add(a, b int) int
来源：http://mic.shanyushiyangtech.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yzv.yj20258.top

C#:   int Add(int a, int b) => a + b;
来源：http://pow.guannengcc.top

[C14] 泛型函数
来源：http://wpp.yueranfly.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yrs.c1oappe.top

PHP:  // 无泛型
来源：http://mtg.sufxvd.cn

JS:   // 无泛型
来源：http://nlp.cashguo.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hqw.jyoumei.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jfk.nanxuanxn.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fbv.pengpengdd.cyou

Ruby: # 无泛型
来源：http://ntr.xinyue.icu

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ksk.havefunace.top

[C15] 解构 / 展开参数
来源：http://ael.tian-w.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://crz.shuidangran.top

PHP:  [$a, $b] = $pair;
来源：http://xmr.jyoumei.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://puj.zhongyouzk.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gmc.jqgufenzy.top

Java: // 无解构
来源：http://jwt.52xcode.cn

Go:   // 无解构
来源：http://ves.yangfankeji.com

Ruby: a, b = pair
来源：http://nbo.ctjpmb.com

C#:   var (a, b) = pair;
来源：http://nol.fengsongda.top

[C16] 函数 / 方法重载
来源：http://agp.epnwcf.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nys.xinyue.icu

PHP:  // 无重载
来源：http://yop.sjlbkw.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bjs.xingfuxueyuan.xyz

TS:   // 用联合类型或重载签名声明
来源：http://szs.fzhhl.top

Java: void f(int a) {}  void f(String a) {}
来源：http://xly.tian-w.cn

Go:   // 无重载：用不同函数名
来源：http://gjc.kuanghao11.cn

Ruby: # 无重载：靠动态参数
来源：http://mag.guannengcc.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://fyb.jiagoushi.top

================================================================================
来源：http://gfw.hesvh.cn

D. 数组 / 列表 / 集合
来源：http://fxm.jiagoushi.top

================================================================================
来源：http://ecd.hesvh.cn

[D01] 创建数组 / 列表
来源：http://kak.hesvh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pjw.yueranfly.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dpi.daria6918.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://axj.ehwqpu.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://yzs.guannengcc.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://plw.birdmap.top

Go:   arr := []int{1, 2, 3}
来源：http://mpk.xingfuxueyuan.xyz

Ruby: arr = [1, 2, 3]
来源：http://rde.shanyushiyangtech.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zbw.jiagoushi.top

[D02] 追加元素到末尾
来源：http://cux.ywan-chungtsiang.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vlu.pengpengdd.cyou

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://szu.fengsongda.top

JS:   arr.push(4);
来源：http://vni.aibaodan.cn

TS:   arr.push(4);
来源：http://lwn.c1oappe.top

Java: list.add(4);
来源：http://irw.gotoacloud.top

Go:   arr = append(arr, 4)
来源：http://hgv.vehdjk.com

Ruby: arr << 4; arr.push(5)
来源：http://qfk.birdmap.top

C#:   list.Add(4);
来源：http://hey.zhongyouzk.top

[D03] 在指定位置插入元素
来源：http://roy.bjfxy.top

Py:   arr.insert(0, 0)
来源：http://epl.zhijiandao.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lba.cheryme.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cuo.smart0.xyz

TS:   arr.splice(0, 0, 0);
来源：http://svp.quarkkingdee.top

Java: list.add(0, 0);
来源：http://iqe.c1oappe.top

Go:   arr = append([]int{0}, arr...)
来源：http://ntz.ywan-chungtsiang.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sfi.iojbl.cn

C#:   list.Insert(0, 0);
来源：http://hxb.xingfuxueyuan.xyz

[D04] 删除元素
来源：http://tts.zdqjudy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pwn.bjfxy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cpi.aibaodan.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yel.hongshengwenyu.top

TS:   arr.splice(0, 1);
来源：http://rog.guannengcc.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nfm.bjfxy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wvz.fengsongda.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://aja.daria6918.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wdp.52xcode.cn

[D05] 访问与修改元素
来源：http://nih.yongpay.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nbj.0kj1m.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fuf.jinqigfzy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://moc.ppjwa.cn

TS:   arr[0]; arr.at(-1);
来源：http://ejh.cucudq.cn

Java: list.get(0); list.set(0, 9);
来源：http://dra.hnxiangtu.top

Go:   arr[0]; arr[0] = 9
来源：http://daz.yanxiufei.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cvb.yj20258.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bhr.sweek.top

[D06] 数组长度
来源：http://fft.chenjidiqi.icu

Py:   len(arr)
来源：http://jcf.hammf.cn

PHP:  count($arr);
来源：http://icq.9152youxi.cn

JS:   arr.length
来源：http://fqu.yuxming.cn

TS:   arr.length
来源：http://vrl.hysaishi.cn

Java: list.size();
来源：http://xtl.andypj.xyz

Go:   len(arr)
来源：http://kut.jinqigufen.top

Ruby: arr.length; arr.size
来源：http://mqc.yueranfly.top

C#:   list.Count;
来源：http://gzf.jinghuilouyu.cn

[D07] 切片 / 取子数组
来源：http://iyq.chenjidiqi.icu

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xbn.cucudq.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jtw.gzhubu.top

JS:   arr.slice(1, 4);
来源：http://xbc.nanxinkj.top

TS:   arr.slice(1, 4);
来源：http://hwz.sxryk.cn

Java: list.subList(1, 4);
来源：http://fyj.uphjek.com

Go:   arr[1:4]
来源：http://llu.gaohongyu789.top

Ruby: arr[1, 3]
来源：http://lae.fengsongda.top

C#:   list.GetRange(1, 3);
来源：http://dyd.9152youxi.cn

[D08] 合并两个数组
来源：http://kso.tianlin.xyz

Py:   a + b;  a.extend(b)
来源：http://mrd.vqdsnc.cn

PHP:  array_merge($a, $b);
来源：http://hdm.cdnleiting.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ugj.dianchejie.cn

TS:   [...a, ...b];
来源：http://uxx.iojbl.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hod.fanxiaobao.xyz

Go:   append(a, b...)
来源：http://vcy.gogol.net.cn

Ruby: a + b;  a.concat(b)
来源：http://gmf.tianlin.xyz

C#:   a.Concat(b).ToList()
来源：http://rlg.zhixingplan.top

[D09] 排序（升序）
来源：http://mes.smart0.xyz

Py:   sorted(arr);  arr.sort()
来源：http://esa.zhijiandao.cn

PHP:  sort($arr);
来源：http://pzm.c1oappe.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://owq.hnqzz.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://zks.hnxiangtu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://eom.zdqjudy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hna.ydzc1.top

Ruby: arr.sort
来源：http://rxw.tian-w.cn

C#:   list.Sort();
来源：http://ssy.xylfe.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ilf.yangfankeji.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://eos.yuanzhike.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://meb.jinqigufen.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dzp.cucudq.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bbp.pengpengdd.cyou

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pla.cashguo.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://scf.jlsjyb.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pnq.pycfn.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://irn.fzhhl.top

[D11] 反转数组
来源：http://peb.ydzc1.top

Py:   arr[::-1];  arr.reverse()
来源：http://arp.xuetiantiany.cn

PHP:  array_reverse($arr);
来源：http://gad.ydjk.org.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vwd.hongshengwenyu.top

TS:   [...arr].reverse();
来源：http://muc.iojbl.cn

Java: Collections.reverse(list);
来源：http://erl.hesvh.cn

Go:   slices.Reverse(arr)
来源：http://ion.zhijiandao.cn

Ruby: arr.reverse
来源：http://rei.dianchejie.cn

C#:   list.Reverse();
来源：http://qvs.sxryk.cn

[D12] 查找元素下标
来源：http://daz.aibaodan.cn

Py:   arr.index(x);  x in arr
来源：http://hkz.sxryk.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://apr.cheryme.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bkj.cashguo.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nvq.gaohongyu789.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pio.tanke756.top

Go:   slices.Index(arr, x)
来源：http://lyk.hesvh.cn

Ruby: arr.index(x)
来源：http://xlt.ehwqpu.com

C#:   list.IndexOf(x);
来源：http://kbh.daxiang520.top

[D13] 过滤（保留满足条件的）
来源：http://kon.ydzc1.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sih.wangshuangyany.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ahq.redwolf501.top

JS:   arr.filter(x => x > 3)
来源：http://zyg.bjfxy.top

TS:   arr.filter(x => x > 3)
来源：http://jiq.ctjpmb.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dba.ydjk.org.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xvb.guannengcc.top

Ruby: arr.select { |x| x > 3 }
来源：http://qvq.jqgfzy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://zzu.xinyue.icu

[D14] 映射转换（每个元素变形）
来源：http://gtw.yanxiufei.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://egf.yongpay.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hjr.bbcook.cn

JS:   arr.map(x => x * 2)
来源：http://btf.zdqjudy.top

TS:   arr.map(x => x * 2)
来源：http://mfl.guannengcc.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://cqu.ywan-chungtsiang.top

Go:   // 手写循环
来源：http://rff.bbcook.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zgz.havefunace.top

C#:   list.Select(x => x * 2).ToList()
来源：http://hjl.ivvv.top

[D15] 去重
来源：http://ivf.epnwcf.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://top.ybcxt.top

PHP:  array_unique($arr);
来源：http://uvz.ivvv.top

JS:   [...new Set(arr)]
来源：http://mok.nanxinkj.top

TS:   [...new Set(arr)]
来源：http://dbf.jqgufenzy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cyv.zhaomingkeji.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://lfv.xinyue.icu

Ruby: arr.uniq
来源：http://fpv.xylfe.cn

C#:   list.Distinct().ToList()
来源：http://oze.guowangkeji.top

[D16] 求和与平均值
来源：http://atr.wangshuangyany.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ofg.hongshengwenyu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ipk.316326.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cco.fzhhl.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tkg.cucudq.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://div.gogol.net.cn

Go:   // 手写循环累加
来源：http://trg.sysykeji.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cax.yj20258888.top

C#:   list.Sum();  list.Average()
来源：http://sqj.dashuyun.cn

[D17] 最大值与最小值
来源：http://cil.chenzaomai.com

Py:   max(arr);  min(arr)
来源：http://mau.yvedp.cn

PHP:  max($arr);  min($arr);
来源：http://igc.fengsongda.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vor.dashuyun.cn

TS:   Math.max(...arr);
来源：http://lgp.jlsjyb.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://hmc.hywenlv.cn


<!-- 参考信息 -->