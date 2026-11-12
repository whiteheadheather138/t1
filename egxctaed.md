代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://yhu.gaohongyu789.top

[C03] 可变参数
来源：http://wob.andypj.xyz

Py:   def total(*args): return sum(args)
来源：http://uuz.yj202588.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://stu.ctjpmb.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mbp.chenzaomai.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tzl.tianlin.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tlz.nanxuanxn.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yxt.jlsjyb.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wuj.sufxvd.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://som.ydjk.org.cn

[C04] 命名参数 / 关键字参数
来源：http://iep.daxiang520.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gnw.fanxiaobao.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blj.xingfuxueyuan.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kly.cdnleiting.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zhh.aibaodan.cn

Java: // 无：用 Builder 模式或 record
来源：http://btx.ehwqpu.com

Go:   // 无：用配置结构体参数
来源：http://zdk.smart0.xyz

Ruby: f(a: 1, b: 2)
来源：http://sfx.shangyingyoupin.top

C#:   f(a: 1, b: 2)
来源：http://msw.jyoumei.cn

[C05] 返回多个值
来源：http://sad.yueranfly.top

Py:   return a, b
来源：http://bod.jianghu66.top

PHP:  return [$a, $b];
来源：http://zvt.jianghu66.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ubn.hnqzz.top

TS:   return { a, b };
来源：http://iyh.jqgfzy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tgw.pengpengdd.cyou

Go:   return a, b
来源：http://nzi.zhiwuduotai.top

Ruby: return a, b
来源：http://qbv.shanyushiyangkeji.top

C#:   return (a, b);              // ValueTuple
来源：http://pym.cheryme.top

[C06] 匿名函数 / lambda
来源：http://ebl.tianlin.xyz

Py:   square = lambda x: x * x
来源：http://nvr.hfpthk.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://rol.quarkkingdee.top

JS:   const square = x => x * x;
来源：http://tdz.sweek.top

TS:   const square = (x: number): number => x * x;
来源：http://fey.iojbl.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zlx.jinqigfzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://wdq.yj20258888.top

Ruby: square = ->(x) { x * x }
来源：http://xqv.nwbrower.top

C#:   Func<int, int> square = x => x * x;
来源：http://sup.yanxiufei.cn

[C07] 把函数作为参数传入
来源：http://gnk.yfazqb.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zrb.zycfv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jck.havefunace.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lzw.birdmap.top

TS:   arr.map(String)
来源：http://ini.hesvh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uue.cdnleiting.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://aug.ehwqpu.com

Ruby: arr.map(&:upcase)
来源：http://tzx.xinyue.icu

C#:   arr.Select(s => s.ToUpper())
来源：http://jwr.zhoulong.xyz

[C08] 闭包
来源：http://ybq.shzxlz.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xlg.shanyushiyangkeji.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vxc.andypj.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fdx.yj202588.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://brk.0kj1m.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://llz.zhiwuduotai.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ard.vehdjk.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://azx.vqdsnc.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://efg.wangshuangyany.cn

[C09] 递归
来源：http://aii.birdmap.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wpv.yueranfly.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mhf.fengsongda.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mxs.redwolf501.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bvb.xinyue.icu

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cik.sweek.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jcl.iojbl.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qdz.tianlin.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gjm.9152youxi.cn

[C10] 变量作用域
来源：http://sku.sjlbkw.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yky.tarul.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://koz.pengpengdd.cyou

JS:   let/const 块级作用域，var 函数级作用域
来源：http://buh.cucudq.cn

TS:   同 JS
来源：http://dpt.bbcook.cn

Java: 方法内为块级作用域
来源：http://qmd.fengsongda.top

Go:   花括号块级作用域
来源：http://gww.hesvh.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jcx.yfazqb.com

C#:   块级作用域
来源：http://mtg.yj202588.top

[C11] 模块导入与导出
来源：http://qfr.aibaodan.cn

Py:   from module import func
来源：http://yqx.fanxiaobao.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://ejq.mhx1999.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://tlh.zhijiandao.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gjp.gzhubu.top

Java: import java.util.List;
来源：http://aax.gaohongyu789.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bdt.ywan-chungtsiang.top

Ruby: require "json"; require_relative "./util"
来源：http://dbw.gotoacloud.top

C#:   using System.Text;
来源：http://bfn.shzxlz.cn

[C12] 立即执行函数 IIFE
来源：http://nvs.pycfn.com

Py:   (lambda: print("run"))()
来源：http://pmt.chenjidiqi.icu

PHP:  (function () { echo "run"; })();
来源：http://xdb.ydjk.org.cn

JS:   (() => { console.log("run"); })();
来源：http://nub.shuidangran.top

TS:   (() => { console.log("run"); })();
来源：http://csi.cheryme.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nkv.xylfe.cn

Go:   func() { fmt.Println("run") }()
来源：http://yvw.dianchejie.cn

Ruby: -> { puts "run" }.call
来源：http://jwp.feifeiyinyue.top

C#:   // 无 IIFE：用静态构造函数
来源：http://jnv.svipenyu.cn

[C13] 类型声明 / 类型注解
来源：http://xqf.xinyue.icu

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hox.wangshuangyany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pfs.sweek.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gud.yj202588.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wvi.ppjwa.cn

Java: int add(int a, int b) { return a + b; }
来源：http://rnx.hammf.cn

Go:   func add(a, b int) int
来源：http://tka.fzhhl.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wds.cashguo.top

C#:   int Add(int a, int b) => a + b;
来源：http://xfo.cheryme.top

[C14] 泛型函数
来源：http://dwq.xuanzx.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jeu.sufxvd.cn

PHP:  // 无泛型
来源：http://gem.kuanghao11.cn

JS:   // 无泛型
来源：http://wts.yuanzhike.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tpp.fehbvm.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://msg.ywan-chungtsiang.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wzw.xziqi.cn

Ruby: # 无泛型
来源：http://ghz.dianchejie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ksi.aizwys.cn

[C15] 解构 / 展开参数
来源：http://wiz.epnwcf.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tau.xuetiantiany.cn

PHP:  [$a, $b] = $pair;
来源：http://bkb.cucudq.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wtg.nanxinkj.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fvw.yfazqb.com

Java: // 无解构
来源：http://olw.cdnleiting.top

Go:   // 无解构
来源：http://llg.shanyushiyangkeji.top

Ruby: a, b = pair
来源：http://ywr.yongpay.top

C#:   var (a, b) = pair;
来源：http://jxj.jqgfzy.top

[C16] 函数 / 方法重载
来源：http://ulf.yangfankeji.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://imj.hywenlv.cn

PHP:  // 无重载
来源：http://tab.zhengqikj.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ifq.jianghu66.top

TS:   // 用联合类型或重载签名声明
来源：http://jwj.ehwqpu.com

Java: void f(int a) {}  void f(String a) {}
来源：http://maq.52xcode.cn

Go:   // 无重载：用不同函数名
来源：http://flw.ydjk.org.cn

Ruby: # 无重载：靠动态参数
来源：http://pkb.havefunace.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://kjo.sysykeji.top

================================================================================
来源：http://vuk.yanxiufei.cn

D. 数组 / 列表 / 集合
来源：http://lxl.guowangkeji.top

================================================================================
来源：http://zyo.yuxming.cn

[D01] 创建数组 / 列表
来源：http://gel.meibo888.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://qiq.meibo888.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xfj.svipenyu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mjx.zhengqikj.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://fwe.snrcjt.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vrp.hnqzz.top

Go:   arr := []int{1, 2, 3}
来源：http://pxk.hywenlv.cn

Ruby: arr = [1, 2, 3]
来源：http://rzi.jinqigufen.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qxx.andypj.xyz

[D02] 追加元素到末尾
来源：http://lyf.shzxlz.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://enk.yj20258.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zsh.quarkkingdee.top

JS:   arr.push(4);
来源：http://qmm.zhongyouzk.top

TS:   arr.push(4);
来源：http://bnh.zhixingplan.top

Java: list.add(4);
来源：http://ouh.shanyushiyangtech.top

Go:   arr = append(arr, 4)
来源：http://lkm.jinghuilouyu.cn

Ruby: arr << 4; arr.push(5)
来源：http://uyu.yvedp.cn

C#:   list.Add(4);
来源：http://zll.52xcode.cn

[D03] 在指定位置插入元素
来源：http://pxo.feifeiyinyue.top

Py:   arr.insert(0, 0)
来源：http://znn.zhengqikj.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vgr.aibaodan.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wjm.jlsjyb.cn

TS:   arr.splice(0, 0, 0);
来源：http://uxk.mhx1999.top

Java: list.add(0, 0);
来源：http://ggf.aibaodan.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mkt.haohaochexian.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lrw.chenjidiqi.icu

C#:   list.Insert(0, 0);
来源：http://ybs.fktsv.cn

[D04] 删除元素
来源：http://nmb.ppjwa.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://imt.fehbvm.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mui.jyoumei.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://veo.yj20258888.top

TS:   arr.splice(0, 1);
来源：http://xyn.jyoumei.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://uvs.ydjk.org.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nlv.gaohongyu789.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qvc.feifeiyinyue.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pcg.yanxiufei.cn

[D05] 访问与修改元素
来源：http://vkj.fengsongda.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xwg.guannengcc.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jzo.quarkkingdee.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sgh.ivvv.top

TS:   arr[0]; arr.at(-1);
来源：http://xng.aizwys.cn

Java: list.get(0); list.set(0, 9);
来源：http://dds.hongshengwenyu.top

Go:   arr[0]; arr[0] = 9
来源：http://ywx.ehwqpu.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xav.fanxiaobao.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mmd.aizwys.cn

[D06] 数组长度
来源：http://riy.havefunace.top

Py:   len(arr)
来源：http://tpy.c1oappe.top

PHP:  count($arr);
来源：http://taq.ivvv.top

JS:   arr.length
来源：http://jem.cdnleiting.top

TS:   arr.length
来源：http://apc.smart0.xyz

Java: list.size();
来源：http://ney.gzhubu.top

Go:   len(arr)
来源：http://urm.xingfuxueyuan.xyz

Ruby: arr.length; arr.size
来源：http://ihq.jqgufenzy.top

C#:   list.Count;
来源：http://elc.yonumen.top

[D07] 切片 / 取子数组
来源：http://dhj.epnwcf.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://iab.wangdashe.top

PHP:  array_slice($arr, 1, 3);
来源：http://akv.wangdashe.top

JS:   arr.slice(1, 4);
来源：http://lbe.uphjek.com

TS:   arr.slice(1, 4);
来源：http://sfr.bjfxy.top

Java: list.subList(1, 4);
来源：http://aib.daxiang520.top

Go:   arr[1:4]
来源：http://peg.shanyushiyangtech.top

Ruby: arr[1, 3]
来源：http://lkw.gzhubu.top

C#:   list.GetRange(1, 3);
来源：http://irk.ctjpmb.com

[D08] 合并两个数组
来源：http://yum.haohaochexian.top

Py:   a + b;  a.extend(b)
来源：http://suh.dianchejie.cn

PHP:  array_merge($a, $b);
来源：http://hqj.sjlbkw.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://oxr.hesvh.cn

TS:   [...a, ...b];
来源：http://fia.snrcjt.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hxq.aizwys.cn

Go:   append(a, b...)
来源：http://kve.ppjwa.cn

Ruby: a + b;  a.concat(b)
来源：http://xqz.havefunace.top

C#:   a.Concat(b).ToList()
来源：http://jim.yj20258.top

[D09] 排序（升序）
来源：http://anf.jiagoushi.top

Py:   sorted(arr);  arr.sort()
来源：http://for.cheryme.top

PHP:  sort($arr);
来源：http://xxu.chenlongwang.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mkm.mhx1999.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://gqp.dianchejie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://loo.sweek.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sqa.guannengcc.top

Ruby: arr.sort
来源：http://riz.birdmap.top

C#:   list.Sort();
来源：http://vlb.haohaochexian.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://usf.zhoulong.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pyt.yvedp.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mll.cheryme.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cbu.zdqjudy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ict.yuxming.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hgf.vehdjk.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vta.ctjpmb.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://scu.pycfn.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ayo.ehwqpu.com

[D11] 反转数组
来源：http://iae.yongpay.top

Py:   arr[::-1];  arr.reverse()
来源：http://xng.dianchejie.cn

PHP:  array_reverse($arr);
来源：http://xly.sweek.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ylq.xinyue.icu

TS:   [...arr].reverse();
来源：http://kpl.hesvh.cn

Java: Collections.reverse(list);
来源：http://vgt.yonumen.top

Go:   slices.Reverse(arr)
来源：http://nhn.zhengqikj.top

Ruby: arr.reverse
来源：http://qwf.gotoacloud.top

C#:   list.Reverse();
来源：http://bvd.pengpengdd.cyou

[D12] 查找元素下标
来源：http://qzl.wangdashe.top

Py:   arr.index(x);  x in arr
来源：http://kpc.zhengqikj.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hpi.dashuyun.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nke.bbcook.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://emz.tianlin.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dkd.shzxlz.cn

Go:   slices.Index(arr, x)
来源：http://lnv.xinyue.icu

Ruby: arr.index(x)
来源：http://nbz.mhx1999.top

C#:   list.IndexOf(x);
来源：http://pff.wangdashe.top

[D13] 过滤（保留满足条件的）
来源：http://sqa.zhongyouzk.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gta.ybcxt.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yyk.cqqwz.cn

JS:   arr.filter(x => x > 3)
来源：http://yko.jianghu66.top

TS:   arr.filter(x => x > 3)
来源：http://eyp.sxryk.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ypy.zdbjq.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vkl.pengpengdd.cyou

Ruby: arr.select { |x| x > 3 }
来源：http://ukd.redwolf501.top

C#:   list.Where(x => x > 3).ToList()
来源：http://due.ydjk.org.cn

[D14] 映射转换（每个元素变形）
来源：http://zdm.ybcxt.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tvb.hysaishi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://god.yanxiufei.cn

JS:   arr.map(x => x * 2)
来源：http://tfu.shuidangran.top

TS:   arr.map(x => x * 2)
来源：http://idw.gaohongyu789.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://vpo.sxryk.cn

Go:   // 手写循环
来源：http://foe.zhaomingkeji.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://zqw.jyoumei.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qcu.hfpthk.cn

[D15] 去重
来源：http://kdt.daxiang520.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vzg.fehbvm.com

PHP:  array_unique($arr);
来源：http://kzo.daria6918.cn

JS:   [...new Set(arr)]
来源：http://tph.hesvh.cn

TS:   [...new Set(arr)]
来源：http://jbi.gotoacloud.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://whc.chenzaomai.com

Go:   // 用 map[T]struct{} 手写
来源：http://oue.sufxvd.cn

Ruby: arr.uniq
来源：http://wlh.fzhhl.top

C#:   list.Distinct().ToList()
来源：http://qlh.sysykeji.top

[D16] 求和与平均值
来源：http://cwe.birdmap.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qjm.jiagoushi.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dkk.nwbrower.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hgp.hammf.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cqj.hysaishi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://llo.hesvh.cn

Go:   // 手写循环累加
来源：http://aad.xuetiantiany.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mhw.zhaomingkeji.xyz

C#:   list.Sum();  list.Average()
来源：http://axn.hnxiangtu.top

[D17] 最大值与最小值
来源：http://xcl.daxiang520.top

Py:   max(arr);  min(arr)
来源：http://eki.ehwqpu.com

PHP:  max($arr);  min($arr);
来源：http://yko.snrcjt.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vyt.dashuyun.cn

TS:   Math.max(...arr);
来源：http://nqk.yuxming.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://vfa.gogol.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zuz.pengpengdd.cyou

Ruby: arr.max;  arr.min
来源：http://uyx.0kj1m.cn

C#:   list.Max();  list.Min()
来源：http://zyv.shanyushiyangkeji.top

[D18] 扁平化嵌套数组
来源：http://oms.gzhubu.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xdw.jiagoushi.top

PHP:  array_merge(...$nested);
来源：http://vpk.chenlongwang.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ztv.zdbjq.cn

TS:   nested.flat();
来源：http://gdq.feifeiyinyue.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://aes.tarul.cn

Go:   // 手写双层循环
来源：http://vxg.yueranfly.top

Ruby: nested.flatten
来源：http://teo.fengsongda.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://xop.hysaishi.cn

[D19] 按字段分组
来源：http://rmh.aizwys.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gac.gogol.net.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://iwq.ctjpmb.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gdu.vehdjk.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://rfk.jinghuilouyu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oha.yonumen.top

Go:   // 手写 map[string][]T
来源：http://dln.c1oappe.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://gdb.haohaochexian.top


<!-- 参考信息 -->