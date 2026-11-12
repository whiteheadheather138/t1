代发 wailian999

Go:   a && b || !c
来源：http://jxs.fanxiaobao.xyz

Ruby: a && b || !c
来源：http://hoe.redwolf501.top

C#:   a && b || !c
来源：http://urt.haohaochexian.top

[B16] 卫语句：不满足条件提前返回
来源：http://rjb.jiagoushi.top

Py:   if not data: return
来源：http://hgz.hcnkem.com

PHP:  if (!$data) { return; }
来源：http://bni.sysykeji.top

JS:   if (!data) return;
来源：http://pkk.cqqwz.cn

TS:   if (!data) return;
来源：http://bxw.pengpengdd.cyou

Java: if (data == null) return;
来源：http://jut.52xcode.cn

Go:   if data == nil { return }
来源：http://gbf.shangyingyoupin.top

Ruby: return if data.nil?
来源：http://hah.hammf.cn

C#:   if (data == null) return;
来源：http://yqa.yanxiufei.cn

================================================================================
来源：http://dtx.daxiang520.top

C. 函数与作用域
来源：http://otv.yvedp.cn

================================================================================
来源：http://kkb.jiagoushi.top

[C01] 定义函数
来源：http://jfq.hesvh.cn

Py:   def add(a, b): return a + b
来源：http://egm.shangyingyoupin.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ufp.ppjwa.cn

JS:   function add(a, b) { return a + b; }
来源：http://mid.xinyue.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lwo.gogol.net.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hoy.bbcook.cn

Go:   func add(a, b int) int { return a + b }
来源：http://org.yangfankeji.com

Ruby: def add(a, b); a + b; end
来源：http://nqx.52xcode.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fko.yueranfly.top

[C02] 默认参数
来源：http://dgo.jinghuilouyu.cn

Py:   def greet(name="World"): return name
来源：http://pea.yj20258888.top

PHP:  function greet($name = "World") { return $name; }
来源：http://epl.daxiang520.top

JS:   function greet(name = "World") { return name; }
来源：http://ikb.snrcjt.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xiw.fanxiaobao.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://upf.yfazqb.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gwy.yuxming.cn

Ruby: def greet(name = "World") = name
来源：http://cpy.meibo888.top

C#:   string Greet(string name = "World") => name;
来源：http://xnv.quarkkingdee.top

[C03] 可变参数
来源：http://jgz.zhaomingkeji.xyz

Py:   def total(*args): return sum(args)
来源：http://obo.ydjk.org.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ytt.hnqzz.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://idc.birdmap.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://suo.xinyue.icu

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qxg.hnqzz.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xhd.gogol.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vyz.yj20258.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://soe.hammf.cn

[C04] 命名参数 / 关键字参数
来源：http://fsh.feifeiyinyue.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://iqf.cucudq.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zjo.tanke756.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://itw.nanxinkj.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hox.pengpengdd.cyou

Java: // 无：用 Builder 模式或 record
来源：http://zju.zhengqikj.top

Go:   // 无：用配置结构体参数
来源：http://tku.kuanghao11.cn

Ruby: f(a: 1, b: 2)
来源：http://bdy.vqdsnc.cn

C#:   f(a: 1, b: 2)
来源：http://ekl.zhongyouzk.top

[C05] 返回多个值
来源：http://ndj.snrcjt.cn

Py:   return a, b
来源：http://ubw.gotoacloud.top

PHP:  return [$a, $b];
来源：http://kdc.fzhhl.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://pac.zhijiandao.cn

TS:   return { a, b };
来源：http://adq.iojbl.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yqg.jinyuanbaomall.cn

Go:   return a, b
来源：http://xvp.vqdsnc.cn

Ruby: return a, b
来源：http://wrb.yangfankeji.com

C#:   return (a, b);              // ValueTuple
来源：http://idx.ivvv.top

[C06] 匿名函数 / lambda
来源：http://mja.cashguo.top

Py:   square = lambda x: x * x
来源：http://snf.dianchejie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://nku.yonumen.top

JS:   const square = x => x * x;
来源：http://rfn.gogol.net.cn

TS:   const square = (x: number): number => x * x;
来源：http://dky.hnxiangtu.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wrl.cqqwz.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gyo.zhaomingkeji.xyz

Ruby: square = ->(x) { x * x }
来源：http://tgy.gotoacloud.top

C#:   Func<int, int> square = x => x * x;
来源：http://smp.yuxming.cn

[C07] 把函数作为参数传入
来源：http://uoh.shanyushiyangtech.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qjg.shzxlz.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vvm.ivvv.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rni.yj20258888.top

TS:   arr.map(String)
来源：http://ngh.hesvh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xdn.ppjwa.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://win.tanke756.top

Ruby: arr.map(&:upcase)
来源：http://gsc.hesvh.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ogy.gzhubu.top

[C08] 闭包
来源：http://fld.fehbvm.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vnu.meibo888.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://odf.sjlbkw.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jzo.daria6918.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lzh.gaohongyu789.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jli.pengpengdd.cyou

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dbw.yuanzhike.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qex.gogol.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hww.yj20258.top

[C09] 递归
来源：http://mih.gaohongyu789.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://szl.cheryme.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kmx.yanxiufei.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gnz.fengsongda.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xef.shuidangran.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mpy.aibaodan.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rtx.xylfe.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://itv.ybcxt.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pay.aibaodan.cn

[C10] 变量作用域
来源：http://nsm.xuetiantiany.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wib.pycfn.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://oow.cashguo.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ksm.kuanghao11.cn

TS:   同 JS
来源：http://eiy.feifeiyinyue.top

Java: 方法内为块级作用域
来源：http://unw.fengsongda.top

Go:   花括号块级作用域
来源：http://fxt.hywenlv.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://euf.kuanghao11.cn

C#:   块级作用域
来源：http://kpi.yvedp.cn

[C11] 模块导入与导出
来源：http://qwf.xinyue.icu

Py:   from module import func
来源：http://ekm.yj202588.top

PHP:  require "file.php";  或 use App\Service;
来源：http://bnn.sysykeji.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://nqi.fehbvm.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mwk.hywenlv.cn

Java: import java.util.List;
来源：http://kfz.bbcook.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wqx.chenlongwang.top

Ruby: require "json"; require_relative "./util"
来源：http://tkm.guannengcc.top

C#:   using System.Text;
来源：http://dgh.ehwqpu.com

[C12] 立即执行函数 IIFE
来源：http://emn.zdbjq.cn

Py:   (lambda: print("run"))()
来源：http://xke.bbcook.cn

PHP:  (function () { echo "run"; })();
来源：http://alg.nanxuanxn.top

JS:   (() => { console.log("run"); })();
来源：http://lfq.zhoulong.xyz

TS:   (() => { console.log("run"); })();
来源：http://nwb.quarkkingdee.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wiy.yfazqb.com

Go:   func() { fmt.Println("run") }()
来源：http://ous.yj20258888.top

Ruby: -> { puts "run" }.call
来源：http://ilx.sweek.top

C#:   // 无 IIFE：用静态构造函数
来源：http://cmc.aizwys.cn

[C13] 类型声明 / 类型注解
来源：http://iyj.andypj.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nfw.fehbvm.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fgc.zhongyouzk.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rtd.sxryk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lvv.yuxming.cn

Java: int add(int a, int b) { return a + b; }
来源：http://itg.xingfuxueyuan.xyz

Go:   func add(a, b int) int
来源：http://czp.shuidangran.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hst.hnxiangtu.top

C#:   int Add(int a, int b) => a + b;
来源：http://ges.daria6918.cn

[C14] 泛型函数
来源：http://irb.sweek.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dup.shuidangran.top

PHP:  // 无泛型
来源：http://jvr.tanke756.top

JS:   // 无泛型
来源：http://nbg.sysykeji.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uqz.zhongyouzk.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://aye.ydzc1.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kjj.epnwcf.com

Ruby: # 无泛型
来源：http://yur.zhongyouzk.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ggd.sysykeji.top

[C15] 解构 / 展开参数
来源：http://ryb.chenzaomai.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qiv.hammf.cn

PHP:  [$a, $b] = $pair;
来源：http://srg.snrcjt.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vgh.aibaodan.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://oed.xziqi.cn

Java: // 无解构
来源：http://fsj.ybcxt.top

Go:   // 无解构
来源：http://iml.smart0.xyz

Ruby: a, b = pair
来源：http://hmo.bbcook.cn

C#:   var (a, b) = pair;
来源：http://xld.shuidangran.top

[C16] 函数 / 方法重载
来源：http://ads.snrcjt.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://prd.jinghuilouyu.cn

PHP:  // 无重载
来源：http://ktq.cqqwz.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://gdp.epnwcf.com

TS:   // 用联合类型或重载签名声明
来源：http://yui.ydzc1.top

Java: void f(int a) {}  void f(String a) {}
来源：http://lul.xinyue.icu

Go:   // 无重载：用不同函数名
来源：http://gdl.fehbvm.com

Ruby: # 无重载：靠动态参数
来源：http://ofy.daria6918.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fsf.aizwys.cn

================================================================================
来源：http://aly.cucudq.cn

D. 数组 / 列表 / 集合
来源：http://wrf.jqgfzy.top

================================================================================
来源：http://oej.bjfxy.top

[D01] 创建数组 / 列表
来源：http://jld.zdqjudy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://xvw.snrcjt.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zqv.mhx1999.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hgr.52xcode.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bfu.jqgufenzy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vdc.guannengcc.top

Go:   arr := []int{1, 2, 3}
来源：http://dji.gzhubu.top

Ruby: arr = [1, 2, 3]
来源：http://yel.shanyushiyangtech.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ysa.zhongyouzk.top

[D02] 追加元素到末尾
来源：http://fws.ppjwa.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qhq.smart0.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hzb.ydzc1.top

JS:   arr.push(4);
来源：http://yuk.hcnkem.com

TS:   arr.push(4);
来源：http://agv.chenlongwang.top

Java: list.add(4);
来源：http://thk.birdmap.top

Go:   arr = append(arr, 4)
来源：http://gny.hnxiangtu.top

Ruby: arr << 4; arr.push(5)
来源：http://pcn.tian-w.cn

C#:   list.Add(4);
来源：http://apl.tian-w.cn

[D03] 在指定位置插入元素
来源：http://bvx.aibaodan.cn

Py:   arr.insert(0, 0)
来源：http://pts.mhx1999.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cvw.birdmap.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wug.cashguo.top

TS:   arr.splice(0, 0, 0);
来源：http://pmf.jyoumei.cn

Java: list.add(0, 0);
来源：http://nsd.guowangkeji.top

Go:   arr = append([]int{0}, arr...)
来源：http://zel.yanxiufei.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tgn.zhaomingkeji.xyz

C#:   list.Insert(0, 0);
来源：http://kow.yangfankeji.com

[D04] 删除元素
来源：http://gyq.yvedp.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cga.zhijiandao.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fab.mhx1999.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gtg.zhijiandao.cn

TS:   arr.splice(0, 1);
来源：http://pbj.316326.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wyp.316326.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tgg.yvedp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vlp.fanxiaobao.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wzl.jiagoushi.top

[D05] 访问与修改元素
来源：http://wwk.sjlbkw.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hfq.fehbvm.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://eub.yongpay.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vkf.birdmap.top

TS:   arr[0]; arr.at(-1);
来源：http://zui.fzhhl.top

Java: list.get(0); list.set(0, 9);
来源：http://taz.ivvv.top

Go:   arr[0]; arr[0] = 9
来源：http://vbz.gzhubu.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vuf.jyoumei.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://brt.iojbl.cn

[D06] 数组长度
来源：http://hgy.hcnkem.com

Py:   len(arr)
来源：http://eda.snrcjt.cn

PHP:  count($arr);
来源：http://lrm.zycfv.cn

JS:   arr.length
来源：http://xga.gogol.net.cn

TS:   arr.length
来源：http://nac.ehwqpu.com

Java: list.size();
来源：http://jfc.aizwys.cn

Go:   len(arr)
来源：http://ycs.guannengcc.top

Ruby: arr.length; arr.size
来源：http://dyh.jiagoushi.top

C#:   list.Count;
来源：http://cmh.zdbjq.cn

[D07] 切片 / 取子数组
来源：http://lwa.yj202588.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wal.bbcook.cn

PHP:  array_slice($arr, 1, 3);
来源：http://uxv.ybcxt.top

JS:   arr.slice(1, 4);
来源：http://btp.shzxlz.cn

TS:   arr.slice(1, 4);
来源：http://amf.snrcjt.cn

Java: list.subList(1, 4);
来源：http://pvv.pengpengdd.cyou

Go:   arr[1:4]
来源：http://ilm.vqdsnc.cn

Ruby: arr[1, 3]
来源：http://dfk.jinyuanbaomall.cn

C#:   list.GetRange(1, 3);
来源：http://sth.ybcxt.top

[D08] 合并两个数组
来源：http://glq.yueranfly.top

Py:   a + b;  a.extend(b)
来源：http://atz.aibaodan.cn

PHP:  array_merge($a, $b);
来源：http://iaj.hywenlv.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://llk.yj20258888.top

TS:   [...a, ...b];
来源：http://ygn.andypj.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fau.aizwys.cn

Go:   append(a, b...)
来源：http://dcr.iojbl.cn

Ruby: a + b;  a.concat(b)
来源：http://vat.chenjidiqi.icu

C#:   a.Concat(b).ToList()
来源：http://fqg.yj20258888.top

[D09] 排序（升序）
来源：http://ldt.yongpay.top

Py:   sorted(arr);  arr.sort()
来源：http://zwu.gotoacloud.top

PHP:  sort($arr);
来源：http://cks.hesvh.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://iio.nanxinkj.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://hae.yuanzhike.top

Java: Collections.sort(list);  list.sort(null);
来源：http://sig.pycfn.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://oee.aizwys.cn

Ruby: arr.sort
来源：http://ett.tarul.cn

C#:   list.Sort();
来源：http://znd.bjfxy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ity.ydzc1.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mqo.yangfankeji.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xjp.xinyue.icu

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://uze.ppjwa.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xse.jlsjyb.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vlt.quarkkingdee.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://haw.jinqigfzy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kim.pycfn.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pqm.jqgfzy.top

[D11] 反转数组
来源：http://bux.zhixingplan.top

Py:   arr[::-1];  arr.reverse()
来源：http://htr.cucudq.cn

PHP:  array_reverse($arr);
来源：http://zmr.dashuyun.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://khn.0kj1m.cn

TS:   [...arr].reverse();
来源：http://qhl.svipenyu.cn

Java: Collections.reverse(list);
来源：http://dvx.xylfe.cn

Go:   slices.Reverse(arr)
来源：http://mmj.sysykeji.top

Ruby: arr.reverse
来源：http://ivd.nanxuanxn.top

C#:   list.Reverse();
来源：http://xxt.wangshuangyany.cn

[D12] 查找元素下标
来源：http://ail.sxryk.cn

Py:   arr.index(x);  x in arr
来源：http://fdv.xziqi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ett.9152youxi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nqp.hongshengwenyu.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zsn.cucudq.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hil.yj20258888.top

Go:   slices.Index(arr, x)
来源：http://lwq.haohaochexian.top

Ruby: arr.index(x)
来源：http://mvx.nanxuanxn.top

C#:   list.IndexOf(x);
来源：http://efk.sysykeji.top

[D13] 过滤（保留满足条件的）
来源：http://kro.jinqigufen.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dus.hfpthk.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hxk.zdqjudy.top

JS:   arr.filter(x => x > 3)
来源：http://lox.andypj.xyz

TS:   arr.filter(x => x > 3)
来源：http://ien.hnxiangtu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vmc.gzhubu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://iwz.tarul.cn

Ruby: arr.select { |x| x > 3 }
来源：http://rii.jinyuanbaomall.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://eie.cashguo.top

[D14] 映射转换（每个元素变形）
来源：http://qvm.nanxuanxn.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bnq.yj20258.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mbw.zdbjq.cn

JS:   arr.map(x => x * 2)
来源：http://elk.yfazqb.com

TS:   arr.map(x => x * 2)
来源：http://yor.zycfv.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qnz.tianlin.xyz

Go:   // 手写循环
来源：http://zkm.fktsv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qgq.hnxiangtu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://fzd.tian-w.cn

[D15] 去重
来源：http://vfg.yj202588.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nli.52xcode.cn

PHP:  array_unique($arr);
来源：http://aod.aibaodan.cn

JS:   [...new Set(arr)]
来源：http://wgx.epnwcf.com

TS:   [...new Set(arr)]
来源：http://ppc.pengpengdd.cyou

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rgr.shzxlz.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ewc.zhaomingkeji.xyz

Ruby: arr.uniq
来源：http://vpi.xuanzx.com

C#:   list.Distinct().ToList()
来源：http://grt.gzhubu.top

[D16] 求和与平均值
来源：http://onl.yuxming.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ndn.snrcjt.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cjw.c1oappe.top


<!-- 参考信息 -->