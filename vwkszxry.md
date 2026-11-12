代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://fht.gotoacloud.top

Go:   func add(a, b int) int { return a + b }
来源：http://ghc.zhixingplan.top

Ruby: def add(a, b); a + b; end
来源：http://ljq.meibo888.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://htf.chenlongwang.top

[C02] 默认参数
来源：http://bxl.c1oappe.top

Py:   def greet(name="World"): return name
来源：http://pmz.wangdashe.top

PHP:  function greet($name = "World") { return $name; }
来源：http://nbk.chenjidiqi.icu

JS:   function greet(name = "World") { return name; }
来源：http://ixh.hongshengwenyu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://cxv.fanxiaobao.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://zir.hfpthk.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://uvg.9152youxi.cn

Ruby: def greet(name = "World") = name
来源：http://jtu.svipenyu.cn

C#:   string Greet(string name = "World") => name;
来源：http://fur.iojbl.cn

[C03] 可变参数
来源：http://dzx.yj20258.top

Py:   def total(*args): return sum(args)
来源：http://anr.pengpengdd.cyou

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ndq.jiagoushi.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zsx.hammf.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://guj.pycfn.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bny.yj202588.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://htp.iojbl.cn

Ruby: def total(*nums); nums.sum; end
来源：http://eos.iojbl.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kbb.shanyushiyangtech.top

[C04] 命名参数 / 关键字参数
来源：http://wgd.gogol.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uln.zycfv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nqj.tarul.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hni.zdqjudy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vsw.zdqjudy.top

Java: // 无：用 Builder 模式或 record
来源：http://nfw.hfpthk.cn

Go:   // 无：用配置结构体参数
来源：http://mct.svipenyu.cn

Ruby: f(a: 1, b: 2)
来源：http://wjr.sysykeji.top

C#:   f(a: 1, b: 2)
来源：http://jwt.xuanzx.com

[C05] 返回多个值
来源：http://aam.jqgfzy.top

Py:   return a, b
来源：http://gpb.sufxvd.cn

PHP:  return [$a, $b];
来源：http://ice.smart0.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://lqn.fzhhl.top

TS:   return { a, b };
来源：http://vcb.xuetiantiany.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://uww.gzhubu.top

Go:   return a, b
来源：http://liv.bbcook.cn

Ruby: return a, b
来源：http://hgt.shanyushiyangkeji.top

C#:   return (a, b);              // ValueTuple
来源：http://mwr.cdnleiting.top

[C06] 匿名函数 / lambda
来源：http://hai.xuetiantiany.cn

Py:   square = lambda x: x * x
来源：http://zod.yueranfly.top

PHP:  $square = fn($x) => $x * $x;
来源：http://jjg.tarul.cn

JS:   const square = x => x * x;
来源：http://kzh.yfazqb.com

TS:   const square = (x: number): number => x * x;
来源：http://dqj.shangyingyoupin.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bhv.aizwys.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hrr.wangdashe.top

Ruby: square = ->(x) { x * x }
来源：http://rad.yangfankeji.com

C#:   Func<int, int> square = x => x * x;
来源：http://nmr.yfazqb.com

[C07] 把函数作为参数传入
来源：http://ozz.fanxiaobao.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sqp.dashuyun.cn

PHP:  array_map("strtoupper", $arr);
来源：http://row.tianlin.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fws.hnxiangtu.top

TS:   arr.map(String)
来源：http://htk.cqqwz.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mnw.hcnkem.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://crk.birdmap.top

Ruby: arr.map(&:upcase)
来源：http://bxm.meibo888.top

C#:   arr.Select(s => s.ToUpper())
来源：http://vqg.hcnkem.com

[C08] 闭包
来源：http://plk.yuxming.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://saw.shzxlz.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://emc.birdmap.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kby.ppjwa.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zhf.xuetiantiany.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://imv.ivvv.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dzb.9152youxi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://poe.c1oappe.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mwc.sweek.top

[C09] 递归
来源：http://oik.yvedp.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://prv.ppjwa.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ihm.cashguo.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://leu.hnqzz.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://efv.hesvh.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ogc.sxryk.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dfu.cqqwz.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wfg.xingfuxueyuan.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dny.ywan-chungtsiang.top

[C10] 变量作用域
来源：http://uym.ywan-chungtsiang.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://afl.wangdashe.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nkm.zhongyouzk.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xxi.yuanzhike.top

TS:   同 JS
来源：http://ema.zdbjq.cn

Java: 方法内为块级作用域
来源：http://mhe.yongpay.top

Go:   花括号块级作用域
来源：http://cpp.cheryme.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ghy.andypj.xyz

C#:   块级作用域
来源：http://lvd.quarkkingdee.top

[C11] 模块导入与导出
来源：http://lwn.meibo888.top

Py:   from module import func
来源：http://rlt.guowangkeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://kjn.feifeiyinyue.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://mpf.guannengcc.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hll.shanyushiyangkeji.top

Java: import java.util.List;
来源：http://yqo.snrcjt.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://utu.fktsv.cn

Ruby: require "json"; require_relative "./util"
来源：http://ybb.yuxming.cn

C#:   using System.Text;
来源：http://jzp.zhiwuduotai.top

[C12] 立即执行函数 IIFE
来源：http://zze.guannengcc.top

Py:   (lambda: print("run"))()
来源：http://nnl.hcnkem.com

PHP:  (function () { echo "run"; })();
来源：http://shm.shzxlz.cn

JS:   (() => { console.log("run"); })();
来源：http://jpc.nanxuanxn.top

TS:   (() => { console.log("run"); })();
来源：http://rtq.redwolf501.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qmb.yfazqb.com

Go:   func() { fmt.Println("run") }()
来源：http://gre.sweek.top

Ruby: -> { puts "run" }.call
来源：http://qjz.gotoacloud.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ukq.meibo888.top

[C13] 类型声明 / 类型注解
来源：http://ren.jinqigfzy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rqt.fehbvm.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rmh.nanxuanxn.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://juy.meibo888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://npm.yangfankeji.com

Java: int add(int a, int b) { return a + b; }
来源：http://fjf.jinqigufen.top

Go:   func add(a, b int) int
来源：http://evz.yangfankeji.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://adq.52xcode.cn

C#:   int Add(int a, int b) => a + b;
来源：http://crb.ehwqpu.com

[C14] 泛型函数
来源：http://djz.sxryk.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://njt.iojbl.cn

PHP:  // 无泛型
来源：http://duf.zdqjudy.top

JS:   // 无泛型
来源：http://nyh.feifeiyinyue.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ibc.smart0.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://iwb.yuanzhike.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zdi.cheryme.top

Ruby: # 无泛型
来源：http://mdn.ybcxt.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vcv.redwolf501.top

[C15] 解构 / 展开参数
来源：http://qkv.shzxlz.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://uel.shzxlz.cn

PHP:  [$a, $b] = $pair;
来源：http://ntm.yuxming.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gbm.jlsjyb.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cze.zdqjudy.top

Java: // 无解构
来源：http://ojs.vehdjk.com

Go:   // 无解构
来源：http://xlu.cashguo.top

Ruby: a, b = pair
来源：http://uuq.sweek.top

C#:   var (a, b) = pair;
来源：http://fjr.ppjwa.cn

[C16] 函数 / 方法重载
来源：http://xuc.bjfxy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://uxz.hnqzz.top

PHP:  // 无重载
来源：http://sdg.nanxuanxn.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://rkb.redwolf501.top

TS:   // 用联合类型或重载签名声明
来源：http://grl.yvedp.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://oec.ywan-chungtsiang.top

Go:   // 无重载：用不同函数名
来源：http://gnt.316326.xyz

Ruby: # 无重载：靠动态参数
来源：http://yso.shangyingyoupin.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://hsz.yj20258.top

================================================================================
来源：http://lnq.havefunace.top

D. 数组 / 列表 / 集合
来源：http://rzr.0kj1m.cn

================================================================================
来源：http://ztk.quarkkingdee.top

[D01] 创建数组 / 列表
来源：http://zfa.hnxiangtu.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://puy.zhijiandao.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://roy.cqqwz.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pxp.shangyingyoupin.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://men.snrcjt.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vul.pycfn.com

Go:   arr := []int{1, 2, 3}
来源：http://wzo.vehdjk.com

Ruby: arr = [1, 2, 3]
来源：http://ewb.jinghuilouyu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://czm.zhongyouzk.top

[D02] 追加元素到末尾
来源：http://hnn.xziqi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://arf.jinghuilouyu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://aek.xuetiantiany.cn

JS:   arr.push(4);
来源：http://nza.tanke756.top

TS:   arr.push(4);
来源：http://art.shangyingyoupin.top

Java: list.add(4);
来源：http://lxz.chenzaomai.com

Go:   arr = append(arr, 4)
来源：http://ipt.haohaochexian.top

Ruby: arr << 4; arr.push(5)
来源：http://feb.yueranfly.top

C#:   list.Add(4);
来源：http://zlo.jianghu66.top

[D03] 在指定位置插入元素
来源：http://wvh.fanxiaobao.xyz

Py:   arr.insert(0, 0)
来源：http://czv.zhoulong.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nhh.0kj1m.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kdi.yfazqb.com

TS:   arr.splice(0, 0, 0);
来源：http://xsh.hnqzz.top

Java: list.add(0, 0);
来源：http://awd.9152youxi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://sro.jinyuanbaomall.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hfq.xuetiantiany.cn

C#:   list.Insert(0, 0);
来源：http://qre.epnwcf.com

[D04] 删除元素
来源：http://jdn.zhengqikj.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dtp.zhongyouzk.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ogf.yonumen.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tzy.hongshengwenyu.top

TS:   arr.splice(0, 1);
来源：http://tzd.gzhubu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tun.ehwqpu.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rax.jinghuilouyu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rob.andypj.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nhv.yuxming.cn

[D05] 访问与修改元素
来源：http://dim.iojbl.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rlm.hfpthk.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://byl.jqgfzy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nji.nanxuanxn.top

TS:   arr[0]; arr.at(-1);
来源：http://rmb.xuetiantiany.cn

Java: list.get(0); list.set(0, 9);
来源：http://qys.aizwys.cn

Go:   arr[0]; arr[0] = 9
来源：http://nbk.zhijiandao.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qjh.ywan-chungtsiang.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ekk.zdbjq.cn

[D06] 数组长度
来源：http://nmt.zhongyouzk.top

Py:   len(arr)
来源：http://hph.bbcook.cn

PHP:  count($arr);
来源：http://tlv.hesvh.cn

JS:   arr.length
来源：http://iet.yj20258888.top

TS:   arr.length
来源：http://vbx.gaohongyu789.top

Java: list.size();
来源：http://glf.ywan-chungtsiang.top

Go:   len(arr)
来源：http://wxh.zhiwuduotai.top

Ruby: arr.length; arr.size
来源：http://gwe.ydjk.org.cn

C#:   list.Count;
来源：http://ehk.hesvh.cn

[D07] 切片 / 取子数组
来源：http://cus.uphjek.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://duu.vqdsnc.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qwd.wangshuangyany.cn

JS:   arr.slice(1, 4);
来源：http://xka.shangyingyoupin.top

TS:   arr.slice(1, 4);
来源：http://cff.shanyushiyangtech.top

Java: list.subList(1, 4);
来源：http://hkh.hywenlv.cn

Go:   arr[1:4]
来源：http://vst.gaohongyu789.top

Ruby: arr[1, 3]
来源：http://szu.xylfe.cn

C#:   list.GetRange(1, 3);
来源：http://tjw.shanyushiyangkeji.top

[D08] 合并两个数组
来源：http://dhu.chenzaomai.com

Py:   a + b;  a.extend(b)
来源：http://jpe.kuanghao11.cn

PHP:  array_merge($a, $b);
来源：http://xxm.xuanzx.com

JS:   [...a, ...b];  a.concat(b);
来源：http://dnk.gogol.net.cn

TS:   [...a, ...b];
来源：http://fjc.andypj.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yjb.xinyue.icu

Go:   append(a, b...)
来源：http://yxb.9152youxi.cn

Ruby: a + b;  a.concat(b)
来源：http://ojr.9152youxi.cn

C#:   a.Concat(b).ToList()
来源：http://nbr.0kj1m.cn

[D09] 排序（升序）
来源：http://dnd.sufxvd.cn

Py:   sorted(arr);  arr.sort()
来源：http://qin.cheryme.top

PHP:  sort($arr);
来源：http://sgg.chenjidiqi.icu

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ybd.yuxming.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mni.dashuyun.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://bag.zhoulong.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mrl.ppjwa.cn

Ruby: arr.sort
来源：http://ird.guowangkeji.top

C#:   list.Sort();
来源：http://pdc.yanxiufei.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://aqw.ybcxt.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sjo.0kj1m.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ing.zhaomingkeji.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rix.ydzc1.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wrs.nwbrower.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ptb.cashguo.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://eyl.cqqwz.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kzk.yj20258.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gjo.zhijiandao.cn

[D11] 反转数组
来源：http://exl.mhx1999.top

Py:   arr[::-1];  arr.reverse()
来源：http://neo.aibaodan.cn

PHP:  array_reverse($arr);
来源：http://ilv.andypj.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nnn.hongshengwenyu.top

TS:   [...arr].reverse();
来源：http://tla.hnxiangtu.top

Java: Collections.reverse(list);
来源：http://zvq.9152youxi.cn

Go:   slices.Reverse(arr)
来源：http://nmz.c1oappe.top

Ruby: arr.reverse
来源：http://ezb.haohaochexian.top

C#:   list.Reverse();
来源：http://ehp.havefunace.top

[D12] 查找元素下标
来源：http://tvj.hnqzz.top

Py:   arr.index(x);  x in arr
来源：http://xwd.yvedp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ptf.zhixingplan.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zlq.ybcxt.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qzt.aizwys.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kwm.daxiang520.top

Go:   slices.Index(arr, x)
来源：http://ila.redwolf501.top

Ruby: arr.index(x)
来源：http://zyx.bjfxy.top

C#:   list.IndexOf(x);
来源：http://qxi.yj20258888.top

[D13] 过滤（保留满足条件的）
来源：http://diy.gotoacloud.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zny.aizwys.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pcg.pycfn.com

JS:   arr.filter(x => x > 3)
来源：http://vsj.yonumen.top

TS:   arr.filter(x => x > 3)
来源：http://ima.fanxiaobao.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vxb.chenzaomai.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fve.aizwys.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ffn.smart0.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://cnw.epnwcf.com

[D14] 映射转换（每个元素变形）
来源：http://bli.yj20258.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zeb.fanxiaobao.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://msq.shangyingyoupin.top

JS:   arr.map(x => x * 2)
来源：http://knd.bbcook.cn

TS:   arr.map(x => x * 2)
来源：http://laq.wangdashe.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://kqj.zdqjudy.top

Go:   // 手写循环
来源：http://bal.feifeiyinyue.top

Ruby: arr.map { |x| x * 2 }
来源：http://wzi.hfpthk.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qqr.shangyingyoupin.top

[D15] 去重
来源：http://wmo.ivvv.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qzj.tian-w.cn

PHP:  array_unique($arr);
来源：http://idz.xuetiantiany.cn

JS:   [...new Set(arr)]
来源：http://fns.zhengqikj.top

TS:   [...new Set(arr)]
来源：http://gub.epnwcf.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zrj.shanyushiyangkeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://upr.ydjk.org.cn

Ruby: arr.uniq
来源：http://pzm.52xcode.cn

C#:   list.Distinct().ToList()
来源：http://zqa.jqgfzy.top

[D16] 求和与平均值
来源：http://rkx.wangshuangyany.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pbo.mhx1999.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pvc.jinghuilouyu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ydd.ybcxt.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tju.smart0.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bvi.jinqigufen.top

Go:   // 手写循环累加
来源：http://qxy.ybcxt.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ntu.yangfankeji.com

C#:   list.Sum();  list.Average()
来源：http://ihb.hywenlv.cn

[D17] 最大值与最小值
来源：http://xkz.cashguo.top

Py:   max(arr);  min(arr)
来源：http://gst.guowangkeji.top

PHP:  max($arr);  min($arr);
来源：http://cco.aibaodan.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://eqk.yj20258888.top

TS:   Math.max(...arr);
来源：http://wfa.dashuyun.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mww.hfpthk.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vbt.fanxiaobao.xyz

Ruby: arr.max;  arr.min
来源：http://chc.kuanghao11.cn

C#:   list.Max();  list.Min()
来源：http://syb.dashuyun.cn

[D18] 扁平化嵌套数组
来源：http://tpy.bbcook.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zjm.wangshuangyany.cn

PHP:  array_merge(...$nested);
来源：http://his.smart0.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rkd.xziqi.cn

TS:   nested.flat();
来源：http://ldu.jqgufenzy.top


<!-- 参考信息 -->