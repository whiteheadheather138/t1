代发 wailian999

[C02] 默认参数
来源：http://thz.dianchejie.cn

Py:   def greet(name="World"): return name
来源：http://voo.chenlongwang.top

PHP:  function greet($name = "World") { return $name; }
来源：http://glh.wangshuangyany.cn

JS:   function greet(name = "World") { return name; }
来源：http://feo.hesvh.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lkx.xuetiantiany.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://biq.yj20258888.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nzs.zdqjudy.top

Ruby: def greet(name = "World") = name
来源：http://dii.fengsongda.top

C#:   string Greet(string name = "World") => name;
来源：http://cso.pycfn.com

[C03] 可变参数
来源：http://xna.chenjidiqi.icu

Py:   def total(*args): return sum(args)
来源：http://jye.jlsjyb.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tbf.yueranfly.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fpa.shuidangran.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gzy.pycfn.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ejm.nanxuanxn.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pxd.nwbrower.top

Ruby: def total(*nums); nums.sum; end
来源：http://gub.zhaomingkeji.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dtg.mhx1999.top

[C04] 命名参数 / 关键字参数
来源：http://hmx.zhengqikj.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dpc.9152youxi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://duf.kuanghao11.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://akt.jyoumei.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dea.meibo888.top

Java: // 无：用 Builder 模式或 record
来源：http://hit.chenlongwang.top

Go:   // 无：用配置结构体参数
来源：http://wnl.nanxuanxn.top

Ruby: f(a: 1, b: 2)
来源：http://yef.wangdashe.top

C#:   f(a: 1, b: 2)
来源：http://iys.jinyuanbaomall.cn

[C05] 返回多个值
来源：http://emy.vqdsnc.cn

Py:   return a, b
来源：http://hyy.sufxvd.cn

PHP:  return [$a, $b];
来源：http://dru.smart0.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://tgg.quarkkingdee.top

TS:   return { a, b };
来源：http://cwv.xinyue.icu

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://njq.havefunace.top

Go:   return a, b
来源：http://xvr.xylfe.cn

Ruby: return a, b
来源：http://nxt.sxryk.cn

C#:   return (a, b);              // ValueTuple
来源：http://pqe.chenzaomai.com

[C06] 匿名函数 / lambda
来源：http://lep.xuanzx.com

Py:   square = lambda x: x * x
来源：http://nfe.zhaomingkeji.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://acx.daxiang520.top

JS:   const square = x => x * x;
来源：http://yuw.jiagoushi.top

TS:   const square = (x: number): number => x * x;
来源：http://hkt.jinqigufen.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bta.birdmap.top

Go:   sq := func(x int) int { return x * x }
来源：http://jsk.yvedp.cn

Ruby: square = ->(x) { x * x }
来源：http://pyd.nwbrower.top

C#:   Func<int, int> square = x => x * x;
来源：http://jdf.vqdsnc.cn

[C07] 把函数作为参数传入
来源：http://ltq.vehdjk.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qip.sufxvd.cn

PHP:  array_map("strtoupper", $arr);
来源：http://tsf.ppjwa.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yps.chenlongwang.top

TS:   arr.map(String)
来源：http://ihz.hysaishi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lbx.bjfxy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://usn.hfpthk.cn

Ruby: arr.map(&:upcase)
来源：http://gzw.wangshuangyany.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://txe.zhoulong.xyz

[C08] 闭包
来源：http://otn.xylfe.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://eht.gogol.net.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rws.zdqjudy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vcw.hnxiangtu.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uds.hcnkem.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ygi.pycfn.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://svo.feifeiyinyue.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cgw.tanke756.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cie.hcnkem.com

[C09] 递归
来源：http://dgq.mhx1999.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pvt.yangfankeji.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wpi.hesvh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uga.0kj1m.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://emx.aibaodan.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wrn.daria6918.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://phg.fengsongda.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fbu.sjlbkw.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uvg.dashuyun.cn

[C10] 变量作用域
来源：http://iee.zhaomingkeji.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pxn.316326.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bzk.uphjek.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hys.shzxlz.cn

TS:   同 JS
来源：http://aog.svipenyu.cn

Java: 方法内为块级作用域
来源：http://iwn.wangshuangyany.cn

Go:   花括号块级作用域
来源：http://cmh.pycfn.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://iet.bjfxy.top

C#:   块级作用域
来源：http://hde.jyoumei.cn

[C11] 模块导入与导出
来源：http://kmy.tian-w.cn

Py:   from module import func
来源：http://eps.ydjk.org.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://klv.zhongyouzk.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://yko.aibaodan.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://oth.tian-w.cn

Java: import java.util.List;
来源：http://yqg.ydjk.org.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://aaa.yvedp.cn

Ruby: require "json"; require_relative "./util"
来源：http://zlf.jlsjyb.cn

C#:   using System.Text;
来源：http://kxj.sweek.top

[C12] 立即执行函数 IIFE
来源：http://asv.guowangkeji.top

Py:   (lambda: print("run"))()
来源：http://vhb.hysaishi.cn

PHP:  (function () { echo "run"; })();
来源：http://tpk.hesvh.cn

JS:   (() => { console.log("run"); })();
来源：http://wux.sysykeji.top

TS:   (() => { console.log("run"); })();
来源：http://nub.yuanzhike.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vfv.vqdsnc.cn

Go:   func() { fmt.Println("run") }()
来源：http://npa.redwolf501.top

Ruby: -> { puts "run" }.call
来源：http://tei.haohaochexian.top

C#:   // 无 IIFE：用静态构造函数
来源：http://pdl.sjlbkw.cn

[C13] 类型声明 / 类型注解
来源：http://qvi.andypj.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gwp.zhaomingkeji.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://svv.cqqwz.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tnv.yj20258888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tor.xuanzx.com

Java: int add(int a, int b) { return a + b; }
来源：http://ren.haohaochexian.top

Go:   func add(a, b int) int
来源：http://jpn.fktsv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://krt.mhx1999.top

C#:   int Add(int a, int b) => a + b;
来源：http://ujy.zhoulong.xyz

[C14] 泛型函数
来源：http://tso.yfazqb.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lrg.ctjpmb.com

PHP:  // 无泛型
来源：http://wgb.sweek.top

JS:   // 无泛型
来源：http://rtv.fanxiaobao.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ibt.meibo888.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://izd.ydzc1.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://oef.yongpay.top

Ruby: # 无泛型
来源：http://bbf.shzxlz.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://awg.mhx1999.top

[C15] 解构 / 展开参数
来源：http://dbr.shanyushiyangkeji.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://acl.sxryk.cn

PHP:  [$a, $b] = $pair;
来源：http://joc.cheryme.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cpb.wangshuangyany.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yec.vehdjk.com

Java: // 无解构
来源：http://gsz.quarkkingdee.top

Go:   // 无解构
来源：http://tma.jinyuanbaomall.cn

Ruby: a, b = pair
来源：http://jbg.zhongyouzk.top

C#:   var (a, b) = pair;
来源：http://aur.yj202588.top

[C16] 函数 / 方法重载
来源：http://etx.chenlongwang.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qyp.svipenyu.cn

PHP:  // 无重载
来源：http://rvr.yj202588.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://fjm.fehbvm.com

TS:   // 用联合类型或重载签名声明
来源：http://ctj.haohaochexian.top

Java: void f(int a) {}  void f(String a) {}
来源：http://nxd.xuanzx.com

Go:   // 无重载：用不同函数名
来源：http://pvy.shuidangran.top

Ruby: # 无重载：靠动态参数
来源：http://eyz.zhongyouzk.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ifu.hcnkem.com

================================================================================
来源：http://hqh.sjlbkw.cn

D. 数组 / 列表 / 集合
来源：http://lka.jqgfzy.top

================================================================================
来源：http://lmd.epnwcf.com

[D01] 创建数组 / 列表
来源：http://qqu.shzxlz.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://uhn.zhongyouzk.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sjf.jiagoushi.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qrs.hysaishi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://rxi.zycfv.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://niv.hammf.cn

Go:   arr := []int{1, 2, 3}
来源：http://nkg.ctjpmb.com

Ruby: arr = [1, 2, 3]
来源：http://dav.bjfxy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vfd.nanxinkj.top

[D02] 追加元素到末尾
来源：http://rib.yfazqb.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zns.tian-w.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bgj.yueranfly.top

JS:   arr.push(4);
来源：http://tox.fktsv.cn

TS:   arr.push(4);
来源：http://mvd.xuanzx.com

Java: list.add(4);
来源：http://uxt.ywan-chungtsiang.top

Go:   arr = append(arr, 4)
来源：http://nfl.wangdashe.top

Ruby: arr << 4; arr.push(5)
来源：http://xrx.vqdsnc.cn

C#:   list.Add(4);
来源：http://emw.zdqjudy.top

[D03] 在指定位置插入元素
来源：http://ysh.316326.xyz

Py:   arr.insert(0, 0)
来源：http://qwj.zycfv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bwt.vqdsnc.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://spo.jinqigufen.top

TS:   arr.splice(0, 0, 0);
来源：http://lch.wangdashe.top

Java: list.add(0, 0);
来源：http://zdk.shzxlz.cn

Go:   arr = append([]int{0}, arr...)
来源：http://uzt.tian-w.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tis.yanxiufei.cn

C#:   list.Insert(0, 0);
来源：http://wkh.nanxuanxn.top

[D04] 删除元素
来源：http://bup.jqgufenzy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jgd.chenzaomai.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://owm.shanyushiyangkeji.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dps.sjlbkw.cn

TS:   arr.splice(0, 1);
来源：http://vmx.guowangkeji.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pdk.daria6918.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hpw.nwbrower.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pmu.tian-w.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vqw.wangdashe.top

[D05] 访问与修改元素
来源：http://vht.tian-w.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://asr.xinyue.icu

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nkv.hesvh.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://esd.havefunace.top

TS:   arr[0]; arr.at(-1);
来源：http://uhy.hcnkem.com

Java: list.get(0); list.set(0, 9);
来源：http://qgx.meibo888.top

Go:   arr[0]; arr[0] = 9
来源：http://jcq.wangshuangyany.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://urv.pengpengdd.cyou

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rfr.andypj.xyz

[D06] 数组长度
来源：http://kdp.hammf.cn

Py:   len(arr)
来源：http://qrk.pycfn.com

PHP:  count($arr);
来源：http://bhh.andypj.xyz

JS:   arr.length
来源：http://npc.smart0.xyz

TS:   arr.length
来源：http://spo.zdbjq.cn

Java: list.size();
来源：http://fxa.yonumen.top

Go:   len(arr)
来源：http://qtf.chenjidiqi.icu

Ruby: arr.length; arr.size
来源：http://zae.yuanzhike.top

C#:   list.Count;
来源：http://wql.tian-w.cn

[D07] 切片 / 取子数组
来源：http://vin.nwbrower.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mrr.bjfxy.top

PHP:  array_slice($arr, 1, 3);
来源：http://lre.52xcode.cn

JS:   arr.slice(1, 4);
来源：http://maz.shangyingyoupin.top

TS:   arr.slice(1, 4);
来源：http://bys.meibo888.top

Java: list.subList(1, 4);
来源：http://adb.xuetiantiany.cn

Go:   arr[1:4]
来源：http://ikc.xuanzx.com

Ruby: arr[1, 3]
来源：http://gvh.hongshengwenyu.top

C#:   list.GetRange(1, 3);
来源：http://wkc.bbcook.cn

[D08] 合并两个数组
来源：http://bwh.xuanzx.com

Py:   a + b;  a.extend(b)
来源：http://gud.yangfankeji.com

PHP:  array_merge($a, $b);
来源：http://xvo.pycfn.com

JS:   [...a, ...b];  a.concat(b);
来源：http://aut.xuanzx.com

TS:   [...a, ...b];
来源：http://frt.yangfankeji.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bfu.bbcook.cn

Go:   append(a, b...)
来源：http://nul.ppjwa.cn

Ruby: a + b;  a.concat(b)
来源：http://jre.feifeiyinyue.top

C#:   a.Concat(b).ToList()
来源：http://jqi.jinghuilouyu.cn

[D09] 排序（升序）
来源：http://zof.snrcjt.cn

Py:   sorted(arr);  arr.sort()
来源：http://iaj.nanxuanxn.top

PHP:  sort($arr);
来源：http://bon.yueranfly.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gup.bjfxy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://lqa.ivvv.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ogv.vqdsnc.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ail.quarkkingdee.top

Ruby: arr.sort
来源：http://fqa.yonumen.top

C#:   list.Sort();
来源：http://bnd.meibo888.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ixt.aibaodan.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://iza.316326.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oip.zhixingplan.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pny.nanxinkj.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gbd.pycfn.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://urx.hongshengwenyu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sgo.zhijiandao.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://icx.hammf.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xnu.chenjidiqi.icu

[D11] 反转数组
来源：http://kmj.shanyushiyangkeji.top

Py:   arr[::-1];  arr.reverse()
来源：http://ehq.jinqigfzy.top

PHP:  array_reverse($arr);
来源：http://lnr.jinqigfzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://urh.daria6918.cn

TS:   [...arr].reverse();
来源：http://usq.kuanghao11.cn

Java: Collections.reverse(list);
来源：http://zrv.gzhubu.top

Go:   slices.Reverse(arr)
来源：http://kok.zhiwuduotai.top

Ruby: arr.reverse
来源：http://uvj.9152youxi.cn

C#:   list.Reverse();
来源：http://lke.hongshengwenyu.top

[D12] 查找元素下标
来源：http://nnh.epnwcf.com

Py:   arr.index(x);  x in arr
来源：http://bfd.aibaodan.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://img.hfpthk.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xml.dianchejie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pwu.uphjek.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wpm.9152youxi.cn

Go:   slices.Index(arr, x)
来源：http://vsh.ydjk.org.cn

Ruby: arr.index(x)
来源：http://vls.sxryk.cn

C#:   list.IndexOf(x);
来源：http://cwa.daria6918.cn

[D13] 过滤（保留满足条件的）
来源：http://ceu.52xcode.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jqz.quarkkingdee.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dli.sxryk.cn

JS:   arr.filter(x => x > 3)
来源：http://neu.jinghuilouyu.cn

TS:   arr.filter(x => x > 3)
来源：http://het.gotoacloud.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://npn.yj20258888.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nvt.jianghu66.top

Ruby: arr.select { |x| x > 3 }
来源：http://kxr.xingfuxueyuan.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://zrz.sysykeji.top

[D14] 映射转换（每个元素变形）
来源：http://imn.cdnleiting.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qmm.zhongyouzk.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mis.uphjek.com

JS:   arr.map(x => x * 2)
来源：http://xfg.xingfuxueyuan.xyz

TS:   arr.map(x => x * 2)
来源：http://fyt.chenlongwang.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://nfy.gzhubu.top

Go:   // 手写循环
来源：http://hsj.hcnkem.com

Ruby: arr.map { |x| x * 2 }
来源：http://rvf.yvedp.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://oun.gotoacloud.top

[D15] 去重
来源：http://jln.tanke756.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wvj.hesvh.cn

PHP:  array_unique($arr);
来源：http://frv.guowangkeji.top

JS:   [...new Set(arr)]
来源：http://mim.hnxiangtu.top

TS:   [...new Set(arr)]
来源：http://bxd.xinyue.icu

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dqx.mhx1999.top

Go:   // 用 map[T]struct{} 手写
来源：http://plx.cucudq.cn

Ruby: arr.uniq
来源：http://ibs.wangdashe.top

C#:   list.Distinct().ToList()
来源：http://aep.jqgufenzy.top

[D16] 求和与平均值
来源：http://fwo.zhijiandao.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yqd.shanyushiyangkeji.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://axy.fzhhl.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wti.aibaodan.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nqy.vqdsnc.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zlk.xziqi.cn

Go:   // 手写循环累加
来源：http://vem.jinqigfzy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xbb.ydzc1.top

C#:   list.Sum();  list.Average()
来源：http://rdq.feifeiyinyue.top

[D17] 最大值与最小值
来源：http://iiq.chenjidiqi.icu

Py:   max(arr);  min(arr)
来源：http://nmy.dashuyun.cn

PHP:  max($arr);  min($arr);
来源：http://aad.9152youxi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dox.daria6918.cn

TS:   Math.max(...arr);
来源：http://zmz.dashuyun.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://uta.shzxlz.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qvx.iojbl.cn

Ruby: arr.max;  arr.min
来源：http://buv.zdqjudy.top

C#:   list.Max();  list.Min()
来源：http://dus.ydjk.org.cn

[D18] 扁平化嵌套数组
来源：http://yip.zhengqikj.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://okq.xuetiantiany.cn

PHP:  array_merge(...$nested);
来源：http://hur.redwolf501.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://poh.zdbjq.cn

TS:   nested.flat();
来源：http://kyr.jinyuanbaomall.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fwf.yueranfly.top

Go:   // 手写双层循环
来源：http://obf.9152youxi.cn

Ruby: nested.flatten
来源：http://jma.haohaochexian.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://xhp.pengpengdd.cyou


<!-- 参考信息 -->