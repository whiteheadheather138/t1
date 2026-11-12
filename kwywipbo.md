代发 wailian999

Go:   a && b || !c
来源：http://wju.fehbvm.com

Ruby: a && b || !c
来源：http://dwb.xziqi.cn

C#:   a && b || !c
来源：http://yiz.316326.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://esi.cucudq.cn

Py:   if not data: return
来源：http://dxj.ydjk.org.cn

PHP:  if (!$data) { return; }
来源：http://zkk.iojbl.cn

JS:   if (!data) return;
来源：http://gde.yj20258.top

TS:   if (!data) return;
来源：http://lzz.nwbrower.top

Java: if (data == null) return;
来源：http://ltg.birdmap.top

Go:   if data == nil { return }
来源：http://btf.yongpay.top

Ruby: return if data.nil?
来源：http://xdw.gogol.net.cn

C#:   if (data == null) return;
来源：http://izl.yj20258.top

================================================================================
来源：http://xvd.hnxiangtu.top

C. 函数与作用域
来源：http://fcf.jinghuilouyu.cn

================================================================================
来源：http://pht.kuanghao11.cn

[C01] 定义函数
来源：http://zjg.shanyushiyangkeji.top

Py:   def add(a, b): return a + b
来源：http://noh.nanxuanxn.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://joi.gogol.net.cn

JS:   function add(a, b) { return a + b; }
来源：http://lnk.vehdjk.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hoe.gaohongyu789.top

Java: static int add(int a, int b) { return a + b; }
来源：http://jhu.cheryme.top

Go:   func add(a, b int) int { return a + b }
来源：http://kij.sjlbkw.cn

Ruby: def add(a, b); a + b; end
来源：http://dha.bbcook.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://iiz.hywenlv.cn

[C02] 默认参数
来源：http://maa.hammf.cn

Py:   def greet(name="World"): return name
来源：http://vlv.xuetiantiany.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://aqc.pycfn.com

JS:   function greet(name = "World") { return name; }
来源：http://qeh.tarul.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wjp.quarkkingdee.top

Java: // 无默认参数：方法重载或 Optional
来源：http://uol.jyoumei.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wbd.shanyushiyangkeji.top

Ruby: def greet(name = "World") = name
来源：http://afu.haohaochexian.top

C#:   string Greet(string name = "World") => name;
来源：http://bon.xinyue.icu

[C03] 可变参数
来源：http://ibo.cashguo.top

Py:   def total(*args): return sum(args)
来源：http://siy.yonumen.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://iqz.shanyushiyangkeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://euy.jqgfzy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://icz.cdnleiting.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://awk.jyoumei.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jlp.0kj1m.cn

Ruby: def total(*nums); nums.sum; end
来源：http://emy.cdnleiting.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tel.uphjek.com

[C04] 命名参数 / 关键字参数
来源：http://qfw.ivvv.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dkh.ydzc1.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://aff.zhiwuduotai.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ykm.havefunace.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mci.hysaishi.cn

Java: // 无：用 Builder 模式或 record
来源：http://lad.ydjk.org.cn

Go:   // 无：用配置结构体参数
来源：http://mcj.sufxvd.cn

Ruby: f(a: 1, b: 2)
来源：http://wlo.jqgfzy.top

C#:   f(a: 1, b: 2)
来源：http://csq.sweek.top

[C05] 返回多个值
来源：http://gra.ehwqpu.com

Py:   return a, b
来源：http://pnz.yongpay.top

PHP:  return [$a, $b];
来源：http://nrh.zdbjq.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://aor.birdmap.top

TS:   return { a, b };
来源：http://lez.smart0.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://acg.zhoulong.xyz

Go:   return a, b
来源：http://zki.xuetiantiany.cn

Ruby: return a, b
来源：http://onb.yj202588.top

C#:   return (a, b);              // ValueTuple
来源：http://ahe.guowangkeji.top

[C06] 匿名函数 / lambda
来源：http://osw.nwbrower.top

Py:   square = lambda x: x * x
来源：http://oyj.hnxiangtu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ymm.xuanzx.com

JS:   const square = x => x * x;
来源：http://ljy.chenjidiqi.icu

TS:   const square = (x: number): number => x * x;
来源：http://brz.hywenlv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pmt.jinqigfzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://hsl.daxiang520.top

Ruby: square = ->(x) { x * x }
来源：http://pas.sweek.top

C#:   Func<int, int> square = x => x * x;
来源：http://tgi.hywenlv.cn

[C07] 把函数作为参数传入
来源：http://rlq.gogol.net.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jkx.snrcjt.cn

PHP:  array_map("strtoupper", $arr);
来源：http://uuq.xziqi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zvv.shanyushiyangtech.top

TS:   arr.map(String)
来源：http://kst.zhoulong.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ktj.birdmap.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bzz.hnqzz.top

Ruby: arr.map(&:upcase)
来源：http://dwi.iojbl.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://piy.xuanzx.com

[C08] 闭包
来源：http://lse.xinyue.icu

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ciz.nwbrower.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dlk.fengsongda.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://miq.guannengcc.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pot.sweek.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tig.epnwcf.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jed.yfazqb.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qtt.wangshuangyany.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rfc.shuidangran.top

[C09] 递归
来源：http://btd.gotoacloud.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wzo.shanyushiyangtech.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jgo.hammf.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xvq.gzhubu.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sfj.smart0.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://umu.sjlbkw.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://daa.xuanzx.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://itj.ydjk.org.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rfn.xziqi.cn

[C10] 变量作用域
来源：http://nfi.jianghu66.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://iyh.guannengcc.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rec.gaohongyu789.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xtg.nanxinkj.top

TS:   同 JS
来源：http://rzx.shzxlz.cn

Java: 方法内为块级作用域
来源：http://saa.vqdsnc.cn

Go:   花括号块级作用域
来源：http://qub.ydjk.org.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ejf.ehwqpu.com

C#:   块级作用域
来源：http://hdd.chenzaomai.com

[C11] 模块导入与导出
来源：http://lju.bjfxy.top

Py:   from module import func
来源：http://spl.jlsjyb.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vml.hammf.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jyz.yangfankeji.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ktj.hysaishi.cn

Java: import java.util.List;
来源：http://icy.ppjwa.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jmo.andypj.xyz

Ruby: require "json"; require_relative "./util"
来源：http://wkj.birdmap.top

C#:   using System.Text;
来源：http://pac.zycfv.cn

[C12] 立即执行函数 IIFE
来源：http://hhb.vqdsnc.cn

Py:   (lambda: print("run"))()
来源：http://isz.fanxiaobao.xyz

PHP:  (function () { echo "run"; })();
来源：http://kyk.wangdashe.top

JS:   (() => { console.log("run"); })();
来源：http://fxk.svipenyu.cn

TS:   (() => { console.log("run"); })();
来源：http://wzd.fanxiaobao.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jqe.zhengqikj.top

Go:   func() { fmt.Println("run") }()
来源：http://bgy.shanyushiyangtech.top

Ruby: -> { puts "run" }.call
来源：http://mcn.316326.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://tha.sufxvd.cn

[C13] 类型声明 / 类型注解
来源：http://jwa.zhengqikj.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gws.bjfxy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cza.pengpengdd.cyou

JS:   // 无类型（可用 JSDoc 注释）
来源：http://olj.jinghuilouyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pfi.fengsongda.top

Java: int add(int a, int b) { return a + b; }
来源：http://mxf.nanxuanxn.top

Go:   func add(a, b int) int
来源：http://rsf.sjlbkw.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gqg.guannengcc.top

C#:   int Add(int a, int b) => a + b;
来源：http://dpi.meibo888.top

[C14] 泛型函数
来源：http://zdy.52xcode.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rmc.nanxinkj.top

PHP:  // 无泛型
来源：http://vpz.daxiang520.top

JS:   // 无泛型
来源：http://uek.ybcxt.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dev.yj202588.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ybo.aizwys.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://job.sweek.top

Ruby: # 无泛型
来源：http://ogq.jinyuanbaomall.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://odw.yfazqb.com

[C15] 解构 / 展开参数
来源：http://pas.chenjidiqi.icu

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://who.aizwys.cn

PHP:  [$a, $b] = $pair;
来源：http://kji.chenlongwang.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://piv.hywenlv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rie.yangfankeji.com

Java: // 无解构
来源：http://swc.birdmap.top

Go:   // 无解构
来源：http://fge.ydjk.org.cn

Ruby: a, b = pair
来源：http://wal.gzhubu.top

C#:   var (a, b) = pair;
来源：http://pfs.guannengcc.top

[C16] 函数 / 方法重载
来源：http://vee.bbcook.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://uty.xingfuxueyuan.xyz

PHP:  // 无重载
来源：http://ulq.pengpengdd.cyou

JS:   // 无重载：靠 arguments.length 分支
来源：http://yzd.shangyingyoupin.top

TS:   // 用联合类型或重载签名声明
来源：http://iql.aibaodan.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ndp.52xcode.cn

Go:   // 无重载：用不同函数名
来源：http://wel.hongshengwenyu.top

Ruby: # 无重载：靠动态参数
来源：http://uwq.feifeiyinyue.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://zaz.nanxinkj.top

================================================================================
来源：http://mgq.fzhhl.top

D. 数组 / 列表 / 集合
来源：http://vnx.epnwcf.com

================================================================================
来源：http://oyr.xylfe.cn

[D01] 创建数组 / 列表
来源：http://fne.zhengqikj.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://mmq.sxryk.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kvr.zdbjq.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yyy.zhiwuduotai.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://lqm.jinqigufen.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dir.dianchejie.cn

Go:   arr := []int{1, 2, 3}
来源：http://rsh.nwbrower.top

Ruby: arr = [1, 2, 3]
来源：http://rcm.fengsongda.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vbs.yueranfly.top

[D02] 追加元素到末尾
来源：http://hev.hnxiangtu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rvk.cucudq.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zfb.tian-w.cn

JS:   arr.push(4);
来源：http://sim.yonumen.top

TS:   arr.push(4);
来源：http://ugd.jianghu66.top

Java: list.add(4);
来源：http://zfv.zhengqikj.top

Go:   arr = append(arr, 4)
来源：http://lzn.jinqigufen.top

Ruby: arr << 4; arr.push(5)
来源：http://itl.shuidangran.top

C#:   list.Add(4);
来源：http://yyk.xziqi.cn

[D03] 在指定位置插入元素
来源：http://ego.epnwcf.com

Py:   arr.insert(0, 0)
来源：http://qww.smart0.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mrd.hnqzz.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hzc.snrcjt.cn

TS:   arr.splice(0, 0, 0);
来源：http://zey.chenjidiqi.icu

Java: list.add(0, 0);
来源：http://die.xuanzx.com

Go:   arr = append([]int{0}, arr...)
来源：http://hxu.svipenyu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ffp.hesvh.cn

C#:   list.Insert(0, 0);
来源：http://tvv.yuxming.cn

[D04] 删除元素
来源：http://bxx.mhx1999.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sba.uphjek.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ppj.zhaomingkeji.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://oaf.shanyushiyangkeji.top

TS:   arr.splice(0, 1);
来源：http://rko.bjfxy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lvh.sufxvd.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qtn.zhaomingkeji.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://oko.shuidangran.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ths.chenzaomai.com

[D05] 访问与修改元素
来源：http://xsz.yueranfly.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ujw.bbcook.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jxz.tian-w.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://stx.zhoulong.xyz

TS:   arr[0]; arr.at(-1);
来源：http://qaf.hnqzz.top

Java: list.get(0); list.set(0, 9);
来源：http://bgs.mhx1999.top

Go:   arr[0]; arr[0] = 9
来源：http://avu.jinqigfzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://idl.ppjwa.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pvk.ydzc1.top

[D06] 数组长度
来源：http://iwt.hywenlv.cn

Py:   len(arr)
来源：http://uiu.daria6918.cn

PHP:  count($arr);
来源：http://qys.sjlbkw.cn

JS:   arr.length
来源：http://svi.jinyuanbaomall.cn

TS:   arr.length
来源：http://sog.zhaomingkeji.xyz

Java: list.size();
来源：http://bsl.yueranfly.top

Go:   len(arr)
来源：http://caj.aibaodan.cn

Ruby: arr.length; arr.size
来源：http://uyj.bjfxy.top

C#:   list.Count;
来源：http://ezy.tian-w.cn

[D07] 切片 / 取子数组
来源：http://iff.nanxinkj.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://szx.ppjwa.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ooh.sweek.top

JS:   arr.slice(1, 4);
来源：http://nhe.sjlbkw.cn

TS:   arr.slice(1, 4);
来源：http://mku.aibaodan.cn

Java: list.subList(1, 4);
来源：http://vhq.smart0.xyz

Go:   arr[1:4]
来源：http://udx.xinyue.icu

Ruby: arr[1, 3]
来源：http://ujv.tarul.cn

C#:   list.GetRange(1, 3);
来源：http://hnh.ydzc1.top

[D08] 合并两个数组
来源：http://yhp.guannengcc.top

Py:   a + b;  a.extend(b)
来源：http://nyv.hesvh.cn

PHP:  array_merge($a, $b);
来源：http://kdy.zdbjq.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gfv.feifeiyinyue.top

TS:   [...a, ...b];
来源：http://jid.redwolf501.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nwb.zhengqikj.top

Go:   append(a, b...)
来源：http://nfo.guowangkeji.top

Ruby: a + b;  a.concat(b)
来源：http://buh.sweek.top

C#:   a.Concat(b).ToList()
来源：http://wqd.kuanghao11.cn

[D09] 排序（升序）
来源：http://moh.iojbl.cn

Py:   sorted(arr);  arr.sort()
来源：http://eva.fehbvm.com

PHP:  sort($arr);
来源：http://cal.cucudq.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://icc.redwolf501.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://lgk.cdnleiting.top

Java: Collections.sort(list);  list.sort(null);
来源：http://div.iojbl.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tqm.hysaishi.cn

Ruby: arr.sort
来源：http://jir.ehwqpu.com

C#:   list.Sort();
来源：http://suo.yueranfly.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://dhz.fanxiaobao.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sun.jianghu66.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wie.hnqzz.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://meg.iojbl.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://toq.gzhubu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://iam.hesvh.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kub.jlsjyb.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vmm.zycfv.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uab.yfazqb.com

[D11] 反转数组
来源：http://gee.hammf.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rhu.shuidangran.top

PHP:  array_reverse($arr);
来源：http://htn.cqqwz.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gsg.yanxiufei.cn

TS:   [...arr].reverse();
来源：http://ooy.zhaomingkeji.xyz

Java: Collections.reverse(list);
来源：http://baz.zhoulong.xyz

Go:   slices.Reverse(arr)
来源：http://obx.yvedp.cn

Ruby: arr.reverse
来源：http://mex.hfpthk.cn

C#:   list.Reverse();
来源：http://yuf.ehwqpu.com

[D12] 查找元素下标
来源：http://whr.aibaodan.cn

Py:   arr.index(x);  x in arr
来源：http://vpj.yvedp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fiw.zhaomingkeji.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gos.yongpay.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qco.zdbjq.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lfs.hcnkem.com

Go:   slices.Index(arr, x)
来源：http://aqt.cdnleiting.top

Ruby: arr.index(x)
来源：http://qnv.kuanghao11.cn

C#:   list.IndexOf(x);
来源：http://xlx.gogol.net.cn

[D13] 过滤（保留满足条件的）
来源：http://zre.jinghuilouyu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ipj.sufxvd.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://roe.kuanghao11.cn

JS:   arr.filter(x => x > 3)
来源：http://fmo.sysykeji.top

TS:   arr.filter(x => x > 3)
来源：http://rpk.tianlin.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jpf.nwbrower.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ija.vqdsnc.cn

Ruby: arr.select { |x| x > 3 }
来源：http://odm.316326.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://fel.shzxlz.cn

[D14] 映射转换（每个元素变形）
来源：http://bhf.andypj.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qud.snrcjt.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://suu.meibo888.top

JS:   arr.map(x => x * 2)
来源：http://bev.chenlongwang.top

TS:   arr.map(x => x * 2)
来源：http://xau.aizwys.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://bfh.meibo888.top

Go:   // 手写循环
来源：http://bpd.xuetiantiany.cn

Ruby: arr.map { |x| x * 2 }
来源：http://krp.jinghuilouyu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://juh.ppjwa.cn

[D15] 去重
来源：http://yqs.mhx1999.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xth.fzhhl.top

PHP:  array_unique($arr);
来源：http://zzk.kuanghao11.cn

JS:   [...new Set(arr)]
来源：http://pwa.xziqi.cn

TS:   [...new Set(arr)]
来源：http://nmd.cqqwz.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://inp.vqdsnc.cn

Go:   // 用 map[T]struct{} 手写
来源：http://puu.feifeiyinyue.top

Ruby: arr.uniq
来源：http://ltv.yonumen.top

C#:   list.Distinct().ToList()
来源：http://zxz.yvedp.cn

[D16] 求和与平均值
来源：http://ehk.sysykeji.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hha.zycfv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lkl.zhengqikj.top


<!-- 参考信息 -->