代发 wailian999

[C02] 默认参数
来源：http://avl.shangyingyoupin.top

Py:   def greet(name="World"): return name
来源：http://fqb.yueranfly.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ppk.havefunace.top

JS:   function greet(name = "World") { return name; }
来源：http://jau.xingfuxueyuan.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://nil.zhengqikj.top

Java: // 无默认参数：方法重载或 Optional
来源：http://dmm.pycfn.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hfz.jianghu66.top

Ruby: def greet(name = "World") = name
来源：http://snw.yuxming.cn

C#:   string Greet(string name = "World") => name;
来源：http://iyc.tanke756.top

[C03] 可变参数
来源：http://sqc.jinghuilouyu.cn

Py:   def total(*args): return sum(args)
来源：http://mko.xingfuxueyuan.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mbb.feifeiyinyue.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vuv.shuidangran.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yhx.bjfxy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://evz.dianchejie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hfl.yj20258.top

Ruby: def total(*nums); nums.sum; end
来源：http://mvg.chenzaomai.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://agh.shuidangran.top

[C04] 命名参数 / 关键字参数
来源：http://lkc.xinyue.icu

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uve.yfazqb.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yqz.guowangkeji.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kpj.hfpthk.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://oqr.dashuyun.cn

Java: // 无：用 Builder 模式或 record
来源：http://ewo.sufxvd.cn

Go:   // 无：用配置结构体参数
来源：http://vla.cucudq.cn

Ruby: f(a: 1, b: 2)
来源：http://qsp.0kj1m.cn

C#:   f(a: 1, b: 2)
来源：http://nbo.hnqzz.top

[C05] 返回多个值
来源：http://qzo.yanxiufei.cn

Py:   return a, b
来源：http://dev.gzhubu.top

PHP:  return [$a, $b];
来源：http://uxn.wangshuangyany.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://mqd.birdmap.top

TS:   return { a, b };
来源：http://bok.9152youxi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://und.uphjek.com

Go:   return a, b
来源：http://dut.fanxiaobao.xyz

Ruby: return a, b
来源：http://uwh.quarkkingdee.top

C#:   return (a, b);              // ValueTuple
来源：http://dtq.hysaishi.cn

[C06] 匿名函数 / lambda
来源：http://lxi.vehdjk.com

Py:   square = lambda x: x * x
来源：http://yfi.jiagoushi.top

PHP:  $square = fn($x) => $x * $x;
来源：http://fya.jyoumei.cn

JS:   const square = x => x * x;
来源：http://tja.gotoacloud.top

TS:   const square = (x: number): number => x * x;
来源：http://efe.9152youxi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hrh.jiagoushi.top

Go:   sq := func(x int) int { return x * x }
来源：http://tfi.tanke756.top

Ruby: square = ->(x) { x * x }
来源：http://dzu.pycfn.com

C#:   Func<int, int> square = x => x * x;
来源：http://erk.sysykeji.top

[C07] 把函数作为参数传入
来源：http://xji.tianlin.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://szv.wangshuangyany.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mnq.zhaomingkeji.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zvp.xziqi.cn

TS:   arr.map(String)
来源：http://kog.shzxlz.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rlq.jinqigufen.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jrj.52xcode.cn

Ruby: arr.map(&:upcase)
来源：http://tso.jyoumei.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://use.dianchejie.cn

[C08] 闭包
来源：http://qhd.zycfv.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://iep.shangyingyoupin.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ftk.ydjk.org.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tgr.jiagoushi.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ubq.9152youxi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ceu.mhx1999.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pgu.yanxiufei.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bhq.jianghu66.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kpw.vqdsnc.cn

[C09] 递归
来源：http://njy.cashguo.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://onc.yangfankeji.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pqn.feifeiyinyue.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mnd.zdbjq.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ooe.haohaochexian.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pqq.jiagoushi.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wot.aizwys.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bay.zhixingplan.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ngb.yuanzhike.top

[C10] 变量作用域
来源：http://ivh.ppjwa.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gau.bbcook.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://urk.hywenlv.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wmz.cashguo.top

TS:   同 JS
来源：http://mzv.ydjk.org.cn

Java: 方法内为块级作用域
来源：http://xwn.hesvh.cn

Go:   花括号块级作用域
来源：http://ldf.andypj.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rfe.zycfv.cn

C#:   块级作用域
来源：http://nka.cashguo.top

[C11] 模块导入与导出
来源：http://xed.jinqigufen.top

Py:   from module import func
来源：http://msi.shanyushiyangtech.top

PHP:  require "file.php";  或 use App\Service;
来源：http://zbw.jyoumei.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pel.daxiang520.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cze.shanyushiyangtech.top

Java: import java.util.List;
来源：http://azf.hfpthk.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kjf.jianghu66.top

Ruby: require "json"; require_relative "./util"
来源：http://amm.yvedp.cn

C#:   using System.Text;
来源：http://swg.yfazqb.com

[C12] 立即执行函数 IIFE
来源：http://wed.kuanghao11.cn

Py:   (lambda: print("run"))()
来源：http://vlq.pycfn.com

PHP:  (function () { echo "run"; })();
来源：http://gst.sufxvd.cn

JS:   (() => { console.log("run"); })();
来源：http://jjs.bjfxy.top

TS:   (() => { console.log("run"); })();
来源：http://iwv.yuxming.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cxu.cucudq.cn

Go:   func() { fmt.Println("run") }()
来源：http://lrp.yj20258.top

Ruby: -> { puts "run" }.call
来源：http://zwj.fanxiaobao.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://oyq.shanyushiyangtech.top

[C13] 类型声明 / 类型注解
来源：http://qgi.jiagoushi.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ifw.xinyue.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jhu.fzhhl.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xnb.jinghuilouyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cht.cashguo.top

Java: int add(int a, int b) { return a + b; }
来源：http://mpa.zdbjq.cn

Go:   func add(a, b int) int
来源：http://bhq.wangshuangyany.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zwa.ywan-chungtsiang.top

C#:   int Add(int a, int b) => a + b;
来源：http://eah.yfazqb.com

[C14] 泛型函数
来源：http://wms.zhengqikj.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hiq.yj202588.top

PHP:  // 无泛型
来源：http://lpk.shzxlz.cn

JS:   // 无泛型
来源：http://ssm.yuxming.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://agh.snrcjt.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://omc.zycfv.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qyo.xylfe.cn

Ruby: # 无泛型
来源：http://ojt.ivvv.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ofq.kuanghao11.cn

[C15] 解构 / 展开参数
来源：http://izr.bbcook.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mkz.daria6918.cn

PHP:  [$a, $b] = $pair;
来源：http://vpb.meibo888.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kvk.daria6918.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bwt.nwbrower.top

Java: // 无解构
来源：http://rcp.yuxming.cn

Go:   // 无解构
来源：http://egv.ivvv.top

Ruby: a, b = pair
来源：http://acu.wangdashe.top

C#:   var (a, b) = pair;
来源：http://doh.316326.xyz

[C16] 函数 / 方法重载
来源：http://yvl.jqgufenzy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bqu.hesvh.cn

PHP:  // 无重载
来源：http://jss.xingfuxueyuan.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://ogj.ctjpmb.com

TS:   // 用联合类型或重载签名声明
来源：http://fgh.meibo888.top

Java: void f(int a) {}  void f(String a) {}
来源：http://uer.zhixingplan.top

Go:   // 无重载：用不同函数名
来源：http://koj.uphjek.com

Ruby: # 无重载：靠动态参数
来源：http://ogm.yongpay.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://tbs.cdnleiting.top

================================================================================
来源：http://jhj.jianghu66.top

D. 数组 / 列表 / 集合
来源：http://kkt.redwolf501.top

================================================================================
来源：http://jjw.jiagoushi.top

[D01] 创建数组 / 列表
来源：http://mkx.havefunace.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ori.yuxming.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jyr.fengsongda.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://snd.hongshengwenyu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://aty.feifeiyinyue.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lsa.yonumen.top

Go:   arr := []int{1, 2, 3}
来源：http://icw.pycfn.com

Ruby: arr = [1, 2, 3]
来源：http://ler.zhengqikj.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xjf.hongshengwenyu.top

[D02] 追加元素到末尾
来源：http://xmj.mhx1999.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bno.chenjidiqi.icu

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jce.epnwcf.com

JS:   arr.push(4);
来源：http://ztk.yuxming.cn

TS:   arr.push(4);
来源：http://dsz.chenlongwang.top

Java: list.add(4);
来源：http://cbo.yj202588.top

Go:   arr = append(arr, 4)
来源：http://vrq.yanxiufei.cn

Ruby: arr << 4; arr.push(5)
来源：http://pbx.quarkkingdee.top

C#:   list.Add(4);
来源：http://bwn.c1oappe.top

[D03] 在指定位置插入元素
来源：http://yam.jinyuanbaomall.cn

Py:   arr.insert(0, 0)
来源：http://pjr.gotoacloud.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://czo.mhx1999.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kub.ydzc1.top

TS:   arr.splice(0, 0, 0);
来源：http://xsr.yanxiufei.cn

Java: list.add(0, 0);
来源：http://vyb.daria6918.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yxu.shanyushiyangkeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://oyb.fzhhl.top

C#:   list.Insert(0, 0);
来源：http://hhy.havefunace.top

[D04] 删除元素
来源：http://iia.zdbjq.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mig.yj20258.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://unf.dianchejie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dsj.dashuyun.cn

TS:   arr.splice(0, 1);
来源：http://msl.zycfv.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gmd.tianlin.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sqz.tanke756.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://omb.guowangkeji.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xxi.zdbjq.cn

[D05] 访问与修改元素
来源：http://spb.shuidangran.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ivt.9152youxi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xsa.wangshuangyany.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uze.smart0.xyz

TS:   arr[0]; arr.at(-1);
来源：http://oom.gzhubu.top

Java: list.get(0); list.set(0, 9);
来源：http://wfr.sufxvd.cn

Go:   arr[0]; arr[0] = 9
来源：http://xun.meibo888.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ewc.yfazqb.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://emg.cucudq.cn

[D06] 数组长度
来源：http://org.nanxinkj.top

Py:   len(arr)
来源：http://gpp.birdmap.top

PHP:  count($arr);
来源：http://fmm.hfpthk.cn

JS:   arr.length
来源：http://bea.c1oappe.top

TS:   arr.length
来源：http://pww.jinqigfzy.top

Java: list.size();
来源：http://eyr.snrcjt.cn

Go:   len(arr)
来源：http://ban.jinghuilouyu.cn

Ruby: arr.length; arr.size
来源：http://fze.zhiwuduotai.top

C#:   list.Count;
来源：http://zpi.jinghuilouyu.cn

[D07] 切片 / 取子数组
来源：http://otu.c1oappe.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mhk.redwolf501.top

PHP:  array_slice($arr, 1, 3);
来源：http://cze.bjfxy.top

JS:   arr.slice(1, 4);
来源：http://unz.pycfn.com

TS:   arr.slice(1, 4);
来源：http://vgm.svipenyu.cn

Java: list.subList(1, 4);
来源：http://fwl.ehwqpu.com

Go:   arr[1:4]
来源：http://uum.zhongyouzk.top

Ruby: arr[1, 3]
来源：http://whv.birdmap.top

C#:   list.GetRange(1, 3);
来源：http://kew.yfazqb.com

[D08] 合并两个数组
来源：http://vqj.zdbjq.cn

Py:   a + b;  a.extend(b)
来源：http://nff.jqgfzy.top

PHP:  array_merge($a, $b);
来源：http://laj.xingfuxueyuan.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://kmk.yj20258888.top

TS:   [...a, ...b];
来源：http://cix.gaohongyu789.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rpr.gzhubu.top

Go:   append(a, b...)
来源：http://dwx.jinyuanbaomall.cn

Ruby: a + b;  a.concat(b)
来源：http://vsh.cashguo.top

C#:   a.Concat(b).ToList()
来源：http://yas.tarul.cn

[D09] 排序（升序）
来源：http://nzg.jinqigfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://ltm.gogol.net.cn

PHP:  sort($arr);
来源：http://apb.cdnleiting.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lnq.haohaochexian.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://vqk.yvedp.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ign.52xcode.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uwo.zhongyouzk.top

Ruby: arr.sort
来源：http://bau.smart0.xyz

C#:   list.Sort();
来源：http://nsi.fehbvm.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://zbi.andypj.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://btq.hnxiangtu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xqo.xuetiantiany.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wun.dianchejie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fur.cdnleiting.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://max.tanke756.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://orq.dianchejie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sqv.yvedp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ktn.jiagoushi.top

[D11] 反转数组
来源：http://thn.gogol.net.cn

Py:   arr[::-1];  arr.reverse()
来源：http://loi.vqdsnc.cn

PHP:  array_reverse($arr);
来源：http://ozt.jqgufenzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rij.uphjek.com

TS:   [...arr].reverse();
来源：http://ifg.fzhhl.top

Java: Collections.reverse(list);
来源：http://wey.hongshengwenyu.top

Go:   slices.Reverse(arr)
来源：http://lpi.9152youxi.cn

Ruby: arr.reverse
来源：http://alf.epnwcf.com

C#:   list.Reverse();
来源：http://iuo.tarul.cn

[D12] 查找元素下标
来源：http://cgl.yueranfly.top

Py:   arr.index(x);  x in arr
来源：http://qnf.hnqzz.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cwh.fehbvm.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://htf.dashuyun.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zet.jyoumei.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bsp.wangshuangyany.cn

Go:   slices.Index(arr, x)
来源：http://jsr.zdbjq.cn

Ruby: arr.index(x)
来源：http://mrp.gaohongyu789.top

C#:   list.IndexOf(x);
来源：http://dxl.yanxiufei.cn

[D13] 过滤（保留满足条件的）
来源：http://lcv.ywan-chungtsiang.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vuc.cqqwz.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lpi.hfpthk.cn

JS:   arr.filter(x => x > 3)
来源：http://pzl.mhx1999.top

TS:   arr.filter(x => x > 3)
来源：http://lww.shzxlz.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fys.ivvv.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qwr.meibo888.top

Ruby: arr.select { |x| x > 3 }
来源：http://aoo.dianchejie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://exm.ehwqpu.com

[D14] 映射转换（每个元素变形）
来源：http://ihh.nanxinkj.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bms.zdbjq.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mqt.52xcode.cn

JS:   arr.map(x => x * 2)
来源：http://vrq.guannengcc.top

TS:   arr.map(x => x * 2)
来源：http://pmo.nanxuanxn.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://yxl.shuidangran.top

Go:   // 手写循环
来源：http://puh.ivvv.top

Ruby: arr.map { |x| x * 2 }
来源：http://cfg.nanxinkj.top

C#:   list.Select(x => x * 2).ToList()
来源：http://dwj.jlsjyb.cn

[D15] 去重
来源：http://syw.hywenlv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mog.bbcook.cn

PHP:  array_unique($arr);
来源：http://fxx.0kj1m.cn

JS:   [...new Set(arr)]
来源：http://yys.gotoacloud.top

TS:   [...new Set(arr)]
来源：http://mzw.fktsv.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uoo.zdbjq.cn

Go:   // 用 map[T]struct{} 手写
来源：http://epv.shanyushiyangtech.top

Ruby: arr.uniq
来源：http://yfb.gotoacloud.top

C#:   list.Distinct().ToList()
来源：http://pgq.zhoulong.xyz

[D16] 求和与平均值
来源：http://ihp.yj202588.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://oje.daria6918.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fip.cashguo.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://roj.hammf.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qlx.yanxiufei.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ayp.bjfxy.top

Go:   // 手写循环累加
来源：http://iys.svipenyu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kht.shuidangran.top

C#:   list.Sum();  list.Average()
来源：http://pnc.redwolf501.top

[D17] 最大值与最小值
来源：http://qel.sysykeji.top

Py:   max(arr);  min(arr)
来源：http://abp.ybcxt.top

PHP:  max($arr);  min($arr);
来源：http://uyk.cashguo.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rfe.xuetiantiany.cn

TS:   Math.max(...arr);
来源：http://oha.xylfe.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jhc.tarul.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rrd.nwbrower.top

Ruby: arr.max;  arr.min
来源：http://mbs.yj20258888.top

C#:   list.Max();  list.Min()
来源：http://vrv.yangfankeji.com

[D18] 扁平化嵌套数组
来源：http://ldj.redwolf501.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pdn.ywan-chungtsiang.top

PHP:  array_merge(...$nested);
来源：http://jxc.mhx1999.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mce.zhongyouzk.top

TS:   nested.flat();
来源：http://fpv.hcnkem.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ysx.wangshuangyany.cn

Go:   // 手写双层循环
来源：http://ypc.chenjidiqi.icu

Ruby: nested.flatten
来源：http://dfz.cheryme.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ujh.9152youxi.cn


<!-- 参考信息 -->