代发 wailian999

================================================================================
来源：http://zoj.guowangkeji.top

C. 函数与作用域
来源：http://bnf.kuanghao11.cn

================================================================================
来源：http://ztx.mhx1999.top

[C01] 定义函数
来源：http://lge.sjlbkw.cn

Py:   def add(a, b): return a + b
来源：http://hzd.zhongyouzk.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hyf.sysykeji.top

JS:   function add(a, b) { return a + b; }
来源：http://mtl.shzxlz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mqf.fzhhl.top

Java: static int add(int a, int b) { return a + b; }
来源：http://zpp.shangyingyoupin.top

Go:   func add(a, b int) int { return a + b }
来源：http://kzt.gotoacloud.top

Ruby: def add(a, b); a + b; end
来源：http://jwu.dianchejie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qfz.bjfxy.top

[C02] 默认参数
来源：http://mol.ywan-chungtsiang.top

Py:   def greet(name="World"): return name
来源：http://mpk.fehbvm.com

PHP:  function greet($name = "World") { return $name; }
来源：http://qtv.fengsongda.top

JS:   function greet(name = "World") { return name; }
来源：http://azc.ydzc1.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ksr.gogol.net.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://tvm.hcnkem.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://byp.chenlongwang.top

Ruby: def greet(name = "World") = name
来源：http://ffv.sweek.top

C#:   string Greet(string name = "World") => name;
来源：http://gye.wangshuangyany.cn

[C03] 可变参数
来源：http://yxm.zdbjq.cn

Py:   def total(*args): return sum(args)
来源：http://uek.zhiwuduotai.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bev.dianchejie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bdz.iojbl.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zsa.jinyuanbaomall.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fyk.iojbl.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://abk.tian-w.cn

Ruby: def total(*nums); nums.sum; end
来源：http://avu.52xcode.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://agg.meibo888.top

[C04] 命名参数 / 关键字参数
来源：http://pai.sufxvd.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ckw.aizwys.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hgt.zhiwuduotai.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rck.zhoulong.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uhu.tian-w.cn

Java: // 无：用 Builder 模式或 record
来源：http://chs.svipenyu.cn

Go:   // 无：用配置结构体参数
来源：http://cmt.fanxiaobao.xyz

Ruby: f(a: 1, b: 2)
来源：http://utc.dashuyun.cn

C#:   f(a: 1, b: 2)
来源：http://wbz.daria6918.cn

[C05] 返回多个值
来源：http://cpb.zhoulong.xyz

Py:   return a, b
来源：http://oos.ybcxt.top

PHP:  return [$a, $b];
来源：http://xbn.yj202588.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://dmt.cqqwz.cn

TS:   return { a, b };
来源：http://xzj.9152youxi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://noc.daxiang520.top

Go:   return a, b
来源：http://zzm.hnxiangtu.top

Ruby: return a, b
来源：http://uyl.hammf.cn

C#:   return (a, b);              // ValueTuple
来源：http://emi.cucudq.cn

[C06] 匿名函数 / lambda
来源：http://hdh.ydjk.org.cn

Py:   square = lambda x: x * x
来源：http://ubw.jinqigufen.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ciy.hammf.cn

JS:   const square = x => x * x;
来源：http://yeh.jyoumei.cn

TS:   const square = (x: number): number => x * x;
来源：http://jky.tarul.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jdt.cdnleiting.top

Go:   sq := func(x int) int { return x * x }
来源：http://erh.hcnkem.com

Ruby: square = ->(x) { x * x }
来源：http://goj.jinqigfzy.top

C#:   Func<int, int> square = x => x * x;
来源：http://eqi.xylfe.cn

[C07] 把函数作为参数传入
来源：http://fdo.yuxming.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nuh.xuanzx.com

PHP:  array_map("strtoupper", $arr);
来源：http://ouo.yangfankeji.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://eyr.tanke756.top

TS:   arr.map(String)
来源：http://thn.aibaodan.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://eez.cdnleiting.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xuf.zhongyouzk.top

Ruby: arr.map(&:upcase)
来源：http://uvj.zhixingplan.top

C#:   arr.Select(s => s.ToUpper())
来源：http://jsf.haohaochexian.top

[C08] 闭包
来源：http://asp.fktsv.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ejx.epnwcf.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://myc.hcnkem.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://skp.zhiwuduotai.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://csh.redwolf501.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://usl.yanxiufei.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://csy.xuetiantiany.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fdz.kuanghao11.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rlm.ybcxt.top

[C09] 递归
来源：http://koc.ctjpmb.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wpo.zhixingplan.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lda.tanke756.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bqy.cucudq.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tsz.shanyushiyangkeji.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bfp.tianlin.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dje.yvedp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vqq.yuxming.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ciw.daxiang520.top

[C10] 变量作用域
来源：http://mtn.jinyuanbaomall.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nyv.sjlbkw.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ckp.gotoacloud.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zxf.kuanghao11.cn

TS:   同 JS
来源：http://cyd.cheryme.top

Java: 方法内为块级作用域
来源：http://ses.xziqi.cn

Go:   花括号块级作用域
来源：http://fzz.vqdsnc.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://llv.yfazqb.com

C#:   块级作用域
来源：http://cxe.zycfv.cn

[C11] 模块导入与导出
来源：http://zgv.pengpengdd.cyou

Py:   from module import func
来源：http://djc.hesvh.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://yrr.jinqigufen.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://tfm.zhengqikj.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dng.zhengqikj.top

Java: import java.util.List;
来源：http://dhw.ctjpmb.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zkg.zhixingplan.top

Ruby: require "json"; require_relative "./util"
来源：http://uub.fzhhl.top

C#:   using System.Text;
来源：http://uor.daria6918.cn

[C12] 立即执行函数 IIFE
来源：http://eat.smart0.xyz

Py:   (lambda: print("run"))()
来源：http://izk.nanxinkj.top

PHP:  (function () { echo "run"; })();
来源：http://lpu.jiagoushi.top

JS:   (() => { console.log("run"); })();
来源：http://djy.epnwcf.com

TS:   (() => { console.log("run"); })();
来源：http://ths.hfpthk.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cky.nwbrower.top

Go:   func() { fmt.Println("run") }()
来源：http://gqn.andypj.xyz

Ruby: -> { puts "run" }.call
来源：http://xfu.daxiang520.top

C#:   // 无 IIFE：用静态构造函数
来源：http://rqe.9152youxi.cn

[C13] 类型声明 / 类型注解
来源：http://cig.pycfn.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bxj.gogol.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gav.jlsjyb.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://frw.svipenyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fil.dashuyun.cn

Java: int add(int a, int b) { return a + b; }
来源：http://pji.svipenyu.cn

Go:   func add(a, b int) int
来源：http://wbh.xingfuxueyuan.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ays.daria6918.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fgj.wangdashe.top

[C14] 泛型函数
来源：http://vuq.0kj1m.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lhb.havefunace.top

PHP:  // 无泛型
来源：http://rks.haohaochexian.top

JS:   // 无泛型
来源：http://kit.zhongyouzk.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cvd.iojbl.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://din.tian-w.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zkf.yj202588.top

Ruby: # 无泛型
来源：http://zkp.jinyuanbaomall.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ujq.hesvh.cn

[C15] 解构 / 展开参数
来源：http://tbi.gogol.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ghg.sjlbkw.cn

PHP:  [$a, $b] = $pair;
来源：http://eet.fengsongda.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://eue.smart0.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jzv.cashguo.top

Java: // 无解构
来源：http://jmr.meibo888.top

Go:   // 无解构
来源：http://vqz.zhengqikj.top

Ruby: a, b = pair
来源：http://epa.feifeiyinyue.top

C#:   var (a, b) = pair;
来源：http://kvw.dianchejie.cn

[C16] 函数 / 方法重载
来源：http://suk.zhengqikj.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qkd.sxryk.cn

PHP:  // 无重载
来源：http://otg.jqgufenzy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://vcq.hnxiangtu.top

TS:   // 用联合类型或重载签名声明
来源：http://dbc.sysykeji.top

Java: void f(int a) {}  void f(String a) {}
来源：http://tcd.gaohongyu789.top

Go:   // 无重载：用不同函数名
来源：http://mmo.ywan-chungtsiang.top

Ruby: # 无重载：靠动态参数
来源：http://dgd.zycfv.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://oqv.sjlbkw.cn

================================================================================
来源：http://rtf.shanyushiyangkeji.top

D. 数组 / 列表 / 集合
来源：http://faa.cucudq.cn

================================================================================
来源：http://hcn.zhiwuduotai.top

[D01] 创建数组 / 列表
来源：http://fca.ehwqpu.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://nvl.zycfv.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://brz.gaohongyu789.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sui.hysaishi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zpn.0kj1m.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dqu.xinyue.icu

Go:   arr := []int{1, 2, 3}
来源：http://tgm.ydjk.org.cn

Ruby: arr = [1, 2, 3]
来源：http://bwx.ehwqpu.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://grb.vqdsnc.cn

[D02] 追加元素到末尾
来源：http://gun.yangfankeji.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://crw.smart0.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qbu.yvedp.cn

JS:   arr.push(4);
来源：http://iur.shuidangran.top

TS:   arr.push(4);
来源：http://fin.jqgufenzy.top

Java: list.add(4);
来源：http://xiy.ywan-chungtsiang.top

Go:   arr = append(arr, 4)
来源：http://arr.sxryk.cn

Ruby: arr << 4; arr.push(5)
来源：http://sol.yongpay.top

C#:   list.Add(4);
来源：http://qdg.aizwys.cn

[D03] 在指定位置插入元素
来源：http://kgg.yangfankeji.com

Py:   arr.insert(0, 0)
来源：http://qvj.andypj.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hfq.vehdjk.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://igi.pycfn.com

TS:   arr.splice(0, 0, 0);
来源：http://loe.0kj1m.cn

Java: list.add(0, 0);
来源：http://jcc.hongshengwenyu.top

Go:   arr = append([]int{0}, arr...)
来源：http://dup.nanxinkj.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://obe.ivvv.top

C#:   list.Insert(0, 0);
来源：http://dau.wangshuangyany.cn

[D04] 删除元素
来源：http://esc.yj202588.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://oml.ctjpmb.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xbz.vehdjk.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://inn.birdmap.top

TS:   arr.splice(0, 1);
来源：http://gfr.zhoulong.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hmf.kuanghao11.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tni.jiagoushi.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fly.feifeiyinyue.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://omi.52xcode.cn

[D05] 访问与修改元素
来源：http://chq.yuxming.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nlp.zdbjq.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://obz.hongshengwenyu.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://okt.c1oappe.top

TS:   arr[0]; arr.at(-1);
来源：http://yjq.sweek.top

Java: list.get(0); list.set(0, 9);
来源：http://syg.ydjk.org.cn

Go:   arr[0]; arr[0] = 9
来源：http://sza.jinyuanbaomall.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://guu.daria6918.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ekj.hywenlv.cn

[D06] 数组长度
来源：http://qjy.gotoacloud.top

Py:   len(arr)
来源：http://upt.chenlongwang.top

PHP:  count($arr);
来源：http://cpm.meibo888.top

JS:   arr.length
来源：http://ief.316326.xyz

TS:   arr.length
来源：http://yhg.shzxlz.cn

Java: list.size();
来源：http://ipn.xylfe.cn

Go:   len(arr)
来源：http://zfh.yonumen.top

Ruby: arr.length; arr.size
来源：http://lgj.redwolf501.top

C#:   list.Count;
来源：http://phv.xingfuxueyuan.xyz

[D07] 切片 / 取子数组
来源：http://izg.tian-w.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tle.zhoulong.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://ije.cashguo.top

JS:   arr.slice(1, 4);
来源：http://npc.gotoacloud.top

TS:   arr.slice(1, 4);
来源：http://ggd.hnxiangtu.top

Java: list.subList(1, 4);
来源：http://fks.hammf.cn

Go:   arr[1:4]
来源：http://lqi.yj20258888.top

Ruby: arr[1, 3]
来源：http://mtv.hesvh.cn

C#:   list.GetRange(1, 3);
来源：http://eam.hcnkem.com

[D08] 合并两个数组
来源：http://hfz.zhiwuduotai.top

Py:   a + b;  a.extend(b)
来源：http://xyt.tanke756.top

PHP:  array_merge($a, $b);
来源：http://sie.shanyushiyangkeji.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ezg.bjfxy.top

TS:   [...a, ...b];
来源：http://rhn.cashguo.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wsk.cucudq.cn

Go:   append(a, b...)
来源：http://tkl.cqqwz.cn

Ruby: a + b;  a.concat(b)
来源：http://jjh.zycfv.cn

C#:   a.Concat(b).ToList()
来源：http://vyf.daxiang520.top

[D09] 排序（升序）
来源：http://rxy.birdmap.top

Py:   sorted(arr);  arr.sort()
来源：http://tai.meibo888.top

PHP:  sort($arr);
来源：http://umu.hywenlv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zbf.jqgfzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://feq.c1oappe.top

Java: Collections.sort(list);  list.sort(null);
来源：http://tlq.nwbrower.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://srs.epnwcf.com

Ruby: arr.sort
来源：http://ewb.cheryme.top

C#:   list.Sort();
来源：http://igq.hongshengwenyu.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://qnt.gzhubu.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dsh.shangyingyoupin.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cfh.smart0.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xka.jinqigfzy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://odq.meibo888.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://daa.dashuyun.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zcg.tanke756.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jsu.hfpthk.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uta.cucudq.cn

[D11] 反转数组
来源：http://hrr.guowangkeji.top

Py:   arr[::-1];  arr.reverse()
来源：http://dpx.vehdjk.com

PHP:  array_reverse($arr);
来源：http://uco.yj20258.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zyv.zdbjq.cn

TS:   [...arr].reverse();
来源：http://hku.nanxinkj.top

Java: Collections.reverse(list);
来源：http://dlw.snrcjt.cn

Go:   slices.Reverse(arr)
来源：http://hqt.ydzc1.top

Ruby: arr.reverse
来源：http://vje.nwbrower.top

C#:   list.Reverse();
来源：http://sxi.yj20258888.top

[D12] 查找元素下标
来源：http://lpd.ivvv.top

Py:   arr.index(x);  x in arr
来源：http://our.chenlongwang.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yab.aibaodan.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://msq.zhengqikj.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://olp.uphjek.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zkh.xziqi.cn

Go:   slices.Index(arr, x)
来源：http://bpg.yj20258.top

Ruby: arr.index(x)
来源：http://hdk.sjlbkw.cn

C#:   list.IndexOf(x);
来源：http://bnp.guowangkeji.top

[D13] 过滤（保留满足条件的）
来源：http://dja.vehdjk.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ioe.vqdsnc.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hff.zhoulong.xyz

JS:   arr.filter(x => x > 3)
来源：http://dxk.hammf.cn

TS:   arr.filter(x => x > 3)
来源：http://xkn.zhiwuduotai.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cgo.meibo888.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gxw.zhengqikj.top

Ruby: arr.select { |x| x > 3 }
来源：http://hil.fktsv.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wlq.chenzaomai.com

[D14] 映射转换（每个元素变形）
来源：http://jkl.cdnleiting.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yho.zdqjudy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jmr.zdbjq.cn

JS:   arr.map(x => x * 2)
来源：http://wvj.hywenlv.cn

TS:   arr.map(x => x * 2)
来源：http://oeu.wangshuangyany.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jls.wangdashe.top

Go:   // 手写循环
来源：http://bdp.hnqzz.top

Ruby: arr.map { |x| x * 2 }
来源：http://fdl.ydjk.org.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zaj.ydzc1.top

[D15] 去重
来源：http://vlw.xuanzx.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lia.iojbl.cn

PHP:  array_unique($arr);
来源：http://qje.xingfuxueyuan.xyz

JS:   [...new Set(arr)]
来源：http://pmu.chenzaomai.com

TS:   [...new Set(arr)]
来源：http://hek.shanyushiyangkeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://aps.yongpay.top

Go:   // 用 map[T]struct{} 手写
来源：http://shb.zhoulong.xyz

Ruby: arr.uniq
来源：http://aia.iojbl.cn

C#:   list.Distinct().ToList()
来源：http://vnk.9152youxi.cn

[D16] 求和与平均值
来源：http://gqf.hnxiangtu.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hzz.xylfe.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gvv.jlsjyb.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jrp.jinghuilouyu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rjv.haohaochexian.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kyo.zhijiandao.cn

Go:   // 手写循环累加
来源：http://akz.mhx1999.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sdd.quarkkingdee.top

C#:   list.Sum();  list.Average()
来源：http://yet.vehdjk.com

[D17] 最大值与最小值
来源：http://txs.gogol.net.cn

Py:   max(arr);  min(arr)
来源：http://jqc.jinqigufen.top

PHP:  max($arr);  min($arr);
来源：http://lpy.nwbrower.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mbg.hfpthk.cn

TS:   Math.max(...arr);
来源：http://mar.ppjwa.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tte.cdnleiting.top


<!-- 参考信息 -->