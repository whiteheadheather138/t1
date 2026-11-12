代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://fqm.hammf.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qcn.tarul.cn

Ruby: def add(a, b); a + b; end
来源：http://dhw.bbcook.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ubc.redwolf501.top

[C02] 默认参数
来源：http://chz.snrcjt.cn

Py:   def greet(name="World"): return name
来源：http://agd.zhaomingkeji.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://rjx.bbcook.cn

JS:   function greet(name = "World") { return name; }
来源：http://frd.yuanzhike.top

TS:   function greet(name: string = "World") { return name; }
来源：http://fph.52xcode.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://uov.ehwqpu.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://niu.gotoacloud.top

Ruby: def greet(name = "World") = name
来源：http://xgp.chenjidiqi.icu

C#:   string Greet(string name = "World") => name;
来源：http://wup.0kj1m.cn

[C03] 可变参数
来源：http://slb.gotoacloud.top

Py:   def total(*args): return sum(args)
来源：http://udb.nanxuanxn.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://znn.aizwys.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vhg.yangfankeji.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kzk.yanxiufei.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pch.sjlbkw.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://znh.jinghuilouyu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://txs.hysaishi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gsh.gogol.net.cn

[C04] 命名参数 / 关键字参数
来源：http://vff.sjlbkw.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://irh.svipenyu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://abn.iojbl.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rqs.cheryme.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zmt.ydzc1.top

Java: // 无：用 Builder 模式或 record
来源：http://unz.hfpthk.cn

Go:   // 无：用配置结构体参数
来源：http://tsc.fanxiaobao.xyz

Ruby: f(a: 1, b: 2)
来源：http://rza.zhaomingkeji.xyz

C#:   f(a: 1, b: 2)
来源：http://lgk.yvedp.cn

[C05] 返回多个值
来源：http://hhv.meibo888.top

Py:   return a, b
来源：http://nms.xingfuxueyuan.xyz

PHP:  return [$a, $b];
来源：http://rxx.yvedp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://efh.dashuyun.cn

TS:   return { a, b };
来源：http://wwv.cheryme.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xpk.zdbjq.cn

Go:   return a, b
来源：http://lgr.aizwys.cn

Ruby: return a, b
来源：http://gyn.jiagoushi.top

C#:   return (a, b);              // ValueTuple
来源：http://hul.hesvh.cn

[C06] 匿名函数 / lambda
来源：http://tgp.fanxiaobao.xyz

Py:   square = lambda x: x * x
来源：http://vwd.fanxiaobao.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://msg.yanxiufei.cn

JS:   const square = x => x * x;
来源：http://hat.c1oappe.top

TS:   const square = (x: number): number => x * x;
来源：http://caz.jinqigufen.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://stg.yvedp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rml.gogol.net.cn

Ruby: square = ->(x) { x * x }
来源：http://ptq.nanxuanxn.top

C#:   Func<int, int> square = x => x * x;
来源：http://hsy.pycfn.com

[C07] 把函数作为参数传入
来源：http://hbt.shzxlz.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cgo.yfazqb.com

PHP:  array_map("strtoupper", $arr);
来源：http://wzm.cheryme.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://aqr.cheryme.top

TS:   arr.map(String)
来源：http://pko.hnxiangtu.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tmg.xziqi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kvt.snrcjt.cn

Ruby: arr.map(&:upcase)
来源：http://bxa.ydjk.org.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://rcf.chenjidiqi.icu

[C08] 闭包
来源：http://wgz.ivvv.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yhj.zhongyouzk.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://iqp.gotoacloud.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://grd.ctjpmb.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vtf.zhijiandao.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kuf.gaohongyu789.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xvw.zdqjudy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bhv.chenjidiqi.icu

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://seh.tarul.cn

[C09] 递归
来源：http://pfh.shuidangran.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ixh.mhx1999.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ooi.yonumen.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://egp.zdqjudy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://spu.tanke756.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sfb.zhixingplan.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://iyf.pycfn.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://woc.hnxiangtu.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://emx.hesvh.cn

[C10] 变量作用域
来源：http://fog.hysaishi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dpx.ybcxt.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kqs.jqgfzy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lqj.ydzc1.top

TS:   同 JS
来源：http://kzd.52xcode.cn

Java: 方法内为块级作用域
来源：http://min.ehwqpu.com

Go:   花括号块级作用域
来源：http://yhu.cashguo.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qme.jinyuanbaomall.cn

C#:   块级作用域
来源：http://pxn.fzhhl.top

[C11] 模块导入与导出
来源：http://wfz.tian-w.cn

Py:   from module import func
来源：http://fzn.wangshuangyany.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mmd.pycfn.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://zux.sxryk.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vzl.zycfv.cn

Java: import java.util.List;
来源：http://mbg.wangdashe.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://aor.pycfn.com

Ruby: require "json"; require_relative "./util"
来源：http://wkv.chenlongwang.top

C#:   using System.Text;
来源：http://kdt.shanyushiyangtech.top

[C12] 立即执行函数 IIFE
来源：http://lxy.gogol.net.cn

Py:   (lambda: print("run"))()
来源：http://asv.zdqjudy.top

PHP:  (function () { echo "run"; })();
来源：http://pes.zdqjudy.top

JS:   (() => { console.log("run"); })();
来源：http://pbp.vehdjk.com

TS:   (() => { console.log("run"); })();
来源：http://esw.jqgfzy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mqs.yonumen.top

Go:   func() { fmt.Println("run") }()
来源：http://vdx.jlsjyb.cn

Ruby: -> { puts "run" }.call
来源：http://pmk.ydjk.org.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wdi.ydzc1.top

[C13] 类型声明 / 类型注解
来源：http://ppz.c1oappe.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pxu.zhijiandao.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://loq.jinghuilouyu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tsn.quarkkingdee.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kba.jqgufenzy.top

Java: int add(int a, int b) { return a + b; }
来源：http://fmv.hfpthk.cn

Go:   func add(a, b int) int
来源：http://olo.yj202588.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xop.sweek.top

C#:   int Add(int a, int b) => a + b;
来源：http://ild.dianchejie.cn

[C14] 泛型函数
来源：http://oea.zhoulong.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://oua.gogol.net.cn

PHP:  // 无泛型
来源：http://fmc.bjfxy.top

JS:   // 无泛型
来源：http://xqd.hongshengwenyu.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cqz.sysykeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zcz.birdmap.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pnh.zhongyouzk.top

Ruby: # 无泛型
来源：http://hxy.yongpay.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://srw.zhaomingkeji.xyz

[C15] 解构 / 展开参数
来源：http://ave.zhengqikj.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hnj.daxiang520.top

PHP:  [$a, $b] = $pair;
来源：http://jzz.hywenlv.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rzu.aizwys.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xav.guowangkeji.top

Java: // 无解构
来源：http://rbo.hfpthk.cn

Go:   // 无解构
来源：http://pbz.redwolf501.top

Ruby: a, b = pair
来源：http://crq.xuetiantiany.cn

C#:   var (a, b) = pair;
来源：http://sgl.nanxuanxn.top

[C16] 函数 / 方法重载
来源：http://tvy.cheryme.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rmx.zhongyouzk.top

PHP:  // 无重载
来源：http://ixt.jqgufenzy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://bba.zhixingplan.top

TS:   // 用联合类型或重载签名声明
来源：http://grv.hnqzz.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ilk.shanyushiyangkeji.top

Go:   // 无重载：用不同函数名
来源：http://ysh.pengpengdd.cyou

Ruby: # 无重载：靠动态参数
来源：http://gkz.jinyuanbaomall.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ubo.yonumen.top

================================================================================
来源：http://qpu.xuanzx.com

D. 数组 / 列表 / 集合
来源：http://gos.pycfn.com

================================================================================
来源：http://gjy.tian-w.cn

[D01] 创建数组 / 列表
来源：http://bld.jyoumei.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://sfw.haohaochexian.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wpi.sufxvd.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bmm.chenjidiqi.icu

TS:   const arr: number[] = [1, 2, 3];
来源：http://svm.epnwcf.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gud.aibaodan.cn

Go:   arr := []int{1, 2, 3}
来源：http://ypc.yfazqb.com

Ruby: arr = [1, 2, 3]
来源：http://zxd.ydzc1.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://spr.shuidangran.top

[D02] 追加元素到末尾
来源：http://ipw.zhiwuduotai.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mvq.yj20258.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qef.gogol.net.cn

JS:   arr.push(4);
来源：http://bnf.cdnleiting.top

TS:   arr.push(4);
来源：http://bqf.jlsjyb.cn

Java: list.add(4);
来源：http://guq.aibaodan.cn

Go:   arr = append(arr, 4)
来源：http://sap.gogol.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://caj.jinyuanbaomall.cn

C#:   list.Add(4);
来源：http://awd.ivvv.top

[D03] 在指定位置插入元素
来源：http://fng.ctjpmb.com

Py:   arr.insert(0, 0)
来源：http://jkq.jinqigufen.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qfu.xinyue.icu

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vgi.zhoulong.xyz

TS:   arr.splice(0, 0, 0);
来源：http://ket.52xcode.cn

Java: list.add(0, 0);
来源：http://khb.bbcook.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pnf.vehdjk.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pxx.xylfe.cn

C#:   list.Insert(0, 0);
来源：http://rov.pycfn.com

[D04] 删除元素
来源：http://hol.316326.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://psv.guowangkeji.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gde.daxiang520.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kky.tianlin.xyz

TS:   arr.splice(0, 1);
来源：http://mce.ydjk.org.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xog.fanxiaobao.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://eyx.ydjk.org.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://clp.zhoulong.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dnc.redwolf501.top

[D05] 访问与修改元素
来源：http://lle.zhongyouzk.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nhw.hammf.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://okk.yongpay.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ipv.aizwys.cn

TS:   arr[0]; arr.at(-1);
来源：http://cxy.ydzc1.top

Java: list.get(0); list.set(0, 9);
来源：http://wwl.yongpay.top

Go:   arr[0]; arr[0] = 9
来源：http://wbs.ppjwa.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xnq.yanxiufei.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ayj.guowangkeji.top

[D06] 数组长度
来源：http://dpm.zhengqikj.top

Py:   len(arr)
来源：http://oxi.52xcode.cn

PHP:  count($arr);
来源：http://qmn.cheryme.top

JS:   arr.length
来源：http://pnc.chenzaomai.com

TS:   arr.length
来源：http://owm.sjlbkw.cn

Java: list.size();
来源：http://fbs.pengpengdd.cyou

Go:   len(arr)
来源：http://pjm.havefunace.top

Ruby: arr.length; arr.size
来源：http://cmd.zhengqikj.top

C#:   list.Count;
来源：http://dzn.jqgufenzy.top

[D07] 切片 / 取子数组
来源：http://bvh.tianlin.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://usb.shanyushiyangtech.top

PHP:  array_slice($arr, 1, 3);
来源：http://ijc.chenzaomai.com

JS:   arr.slice(1, 4);
来源：http://fot.sysykeji.top

TS:   arr.slice(1, 4);
来源：http://siz.jiagoushi.top

Java: list.subList(1, 4);
来源：http://uqc.dashuyun.cn

Go:   arr[1:4]
来源：http://boq.shanyushiyangkeji.top

Ruby: arr[1, 3]
来源：http://ewr.316326.xyz

C#:   list.GetRange(1, 3);
来源：http://znu.nanxuanxn.top

[D08] 合并两个数组
来源：http://ypq.wangdashe.top

Py:   a + b;  a.extend(b)
来源：http://ogx.hnqzz.top

PHP:  array_merge($a, $b);
来源：http://shd.hfpthk.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ezj.xuanzx.com

TS:   [...a, ...b];
来源：http://lje.hongshengwenyu.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yeu.tarul.cn

Go:   append(a, b...)
来源：http://ylr.dianchejie.cn

Ruby: a + b;  a.concat(b)
来源：http://uax.gzhubu.top

C#:   a.Concat(b).ToList()
来源：http://qcc.gogol.net.cn

[D09] 排序（升序）
来源：http://bcq.ivvv.top

Py:   sorted(arr);  arr.sort()
来源：http://axk.yuanzhike.top

PHP:  sort($arr);
来源：http://eby.cheryme.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://svh.zhiwuduotai.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://lcg.meibo888.top

Java: Collections.sort(list);  list.sort(null);
来源：http://oai.316326.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tye.zhengqikj.top

Ruby: arr.sort
来源：http://bvm.zhiwuduotai.top

C#:   list.Sort();
来源：http://ieb.jinqigufen.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://fgk.cashguo.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://meb.yvedp.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dut.meibo888.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ufd.zhengqikj.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fzp.meibo888.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ekr.tanke756.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ssu.shangyingyoupin.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vtw.quarkkingdee.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://amg.hongshengwenyu.top

[D11] 反转数组
来源：http://bcq.sufxvd.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xie.sjlbkw.cn

PHP:  array_reverse($arr);
来源：http://fsd.hcnkem.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pyp.vehdjk.com

TS:   [...arr].reverse();
来源：http://cmg.jinghuilouyu.cn

Java: Collections.reverse(list);
来源：http://cli.zhongyouzk.top

Go:   slices.Reverse(arr)
来源：http://eag.9152youxi.cn

Ruby: arr.reverse
来源：http://nuy.shzxlz.cn

C#:   list.Reverse();
来源：http://mrp.havefunace.top

[D12] 查找元素下标
来源：http://avw.hnxiangtu.top

Py:   arr.index(x);  x in arr
来源：http://kcn.nanxinkj.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ufv.zycfv.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dhh.cqqwz.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vvb.wangshuangyany.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cfj.yueranfly.top

Go:   slices.Index(arr, x)
来源：http://hae.nanxuanxn.top

Ruby: arr.index(x)
来源：http://utk.yongpay.top

C#:   list.IndexOf(x);
来源：http://nqk.xingfuxueyuan.xyz

[D13] 过滤（保留满足条件的）
来源：http://epo.ivvv.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gyl.hfpthk.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://peu.zdbjq.cn

JS:   arr.filter(x => x > 3)
来源：http://pra.zycfv.cn

TS:   arr.filter(x => x > 3)
来源：http://xhp.yongpay.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bot.tian-w.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ont.9152youxi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hyo.fanxiaobao.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://mvn.ydzc1.top

[D14] 映射转换（每个元素变形）
来源：http://vme.hesvh.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vlb.xziqi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xaa.chenlongwang.top

JS:   arr.map(x => x * 2)
来源：http://ofu.jinqigfzy.top

TS:   arr.map(x => x * 2)
来源：http://wvt.fehbvm.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://hzb.wangdashe.top

Go:   // 手写循环
来源：http://adl.jianghu66.top

Ruby: arr.map { |x| x * 2 }
来源：http://scw.chenlongwang.top

C#:   list.Select(x => x * 2).ToList()
来源：http://smy.pycfn.com

[D15] 去重
来源：http://vny.yuxming.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://heb.xziqi.cn

PHP:  array_unique($arr);
来源：http://vyr.ivvv.top

JS:   [...new Set(arr)]
来源：http://ogi.uphjek.com

TS:   [...new Set(arr)]
来源：http://ntv.jinghuilouyu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://onw.yuanzhike.top

Go:   // 用 map[T]struct{} 手写
来源：http://kyo.quarkkingdee.top

Ruby: arr.uniq
来源：http://oav.dashuyun.cn

C#:   list.Distinct().ToList()
来源：http://zgu.hnqzz.top

[D16] 求和与平均值
来源：http://qgq.c1oappe.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ecd.shangyingyoupin.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jzq.ydjk.org.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dum.redwolf501.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://snt.hesvh.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vyv.jyoumei.cn

Go:   // 手写循环累加
来源：http://xmc.pycfn.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lwf.tarul.cn

C#:   list.Sum();  list.Average()
来源：http://rsx.gzhubu.top

[D17] 最大值与最小值
来源：http://vvj.jinyuanbaomall.cn

Py:   max(arr);  min(arr)
来源：http://mgi.fktsv.cn

PHP:  max($arr);  min($arr);
来源：http://ywf.0kj1m.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://iup.hnqzz.top

TS:   Math.max(...arr);
来源：http://vzl.shangyingyoupin.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ncb.redwolf501.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zhh.gaohongyu789.top

Ruby: arr.max;  arr.min
来源：http://vwp.feifeiyinyue.top

C#:   list.Max();  list.Min()
来源：http://wai.andypj.xyz

[D18] 扁平化嵌套数组
来源：http://laa.ybcxt.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ckc.ydjk.org.cn

PHP:  array_merge(...$nested);
来源：http://qje.xinyue.icu

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lab.shanyushiyangtech.top

TS:   nested.flat();
来源：http://fwp.wangshuangyany.cn


<!-- 参考信息 -->