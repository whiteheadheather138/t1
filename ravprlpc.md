代发 wailian999

Go:   a && b || !c
来源：http://wbd.cdnleiting.top

Ruby: a && b || !c
来源：http://jeq.jinghuilouyu.cn

C#:   a && b || !c
来源：http://ezn.wangshuangyany.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wnx.fanxiaobao.xyz

Py:   if not data: return
来源：http://ecz.316326.xyz

PHP:  if (!$data) { return; }
来源：http://gjj.ctjpmb.com

JS:   if (!data) return;
来源：http://ddl.hywenlv.cn

TS:   if (!data) return;
来源：http://yjp.vehdjk.com

Java: if (data == null) return;
来源：http://tmg.zhoulong.xyz

Go:   if data == nil { return }
来源：http://mjt.jinqigufen.top

Ruby: return if data.nil?
来源：http://xbs.chenlongwang.top

C#:   if (data == null) return;
来源：http://mnc.bjfxy.top

================================================================================
来源：http://zur.cheryme.top

C. 函数与作用域
来源：http://opp.aibaodan.cn

================================================================================
来源：http://rfa.cheryme.top

[C01] 定义函数
来源：http://wpa.shuidangran.top

Py:   def add(a, b): return a + b
来源：http://aea.cashguo.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://msr.jyoumei.cn

JS:   function add(a, b) { return a + b; }
来源：http://sra.zhengqikj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fts.redwolf501.top

Java: static int add(int a, int b) { return a + b; }
来源：http://igk.havefunace.top

Go:   func add(a, b int) int { return a + b }
来源：http://fsa.daxiang520.top

Ruby: def add(a, b); a + b; end
来源：http://xph.meibo888.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cin.vqdsnc.cn

[C02] 默认参数
来源：http://ywr.aizwys.cn

Py:   def greet(name="World"): return name
来源：http://zvx.52xcode.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wnl.yj20258888.top

JS:   function greet(name = "World") { return name; }
来源：http://txu.xylfe.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xaz.cucudq.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bgj.chenlongwang.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lsn.tianlin.xyz

Ruby: def greet(name = "World") = name
来源：http://lzh.fktsv.cn

C#:   string Greet(string name = "World") => name;
来源：http://mrz.gotoacloud.top

[C03] 可变参数
来源：http://lrj.zhiwuduotai.top

Py:   def total(*args): return sum(args)
来源：http://pcd.daria6918.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uts.yj20258.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gpg.shanyushiyangkeji.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rtc.wangdashe.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gwx.ehwqpu.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qmn.chenjidiqi.icu

Ruby: def total(*nums); nums.sum; end
来源：http://qju.yj202588.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vuy.sxryk.cn

[C04] 命名参数 / 关键字参数
来源：http://kdy.ywan-chungtsiang.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ytc.c1oappe.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://txz.hammf.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hiw.sweek.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lxt.vqdsnc.cn

Java: // 无：用 Builder 模式或 record
来源：http://gzb.jinyuanbaomall.cn

Go:   // 无：用配置结构体参数
来源：http://ekh.cdnleiting.top

Ruby: f(a: 1, b: 2)
来源：http://xtq.daria6918.cn

C#:   f(a: 1, b: 2)
来源：http://urg.dianchejie.cn

[C05] 返回多个值
来源：http://pib.ybcxt.top

Py:   return a, b
来源：http://gvz.yuxming.cn

PHP:  return [$a, $b];
来源：http://ofk.zdqjudy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://nmr.zhoulong.xyz

TS:   return { a, b };
来源：http://fyl.chenlongwang.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wuf.daxiang520.top

Go:   return a, b
来源：http://rdw.mhx1999.top

Ruby: return a, b
来源：http://mle.cdnleiting.top

C#:   return (a, b);              // ValueTuple
来源：http://hou.yonumen.top

[C06] 匿名函数 / lambda
来源：http://zko.xingfuxueyuan.xyz

Py:   square = lambda x: x * x
来源：http://hgf.ydjk.org.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://frv.yongpay.top

JS:   const square = x => x * x;
来源：http://fov.mhx1999.top

TS:   const square = (x: number): number => x * x;
来源：http://hzw.dashuyun.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fzn.gaohongyu789.top

Go:   sq := func(x int) int { return x * x }
来源：http://kwf.uphjek.com

Ruby: square = ->(x) { x * x }
来源：http://ehn.shanyushiyangkeji.top

C#:   Func<int, int> square = x => x * x;
来源：http://agk.zdqjudy.top

[C07] 把函数作为参数传入
来源：http://fmm.sjlbkw.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xww.xinyue.icu

PHP:  array_map("strtoupper", $arr);
来源：http://rds.vqdsnc.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://faf.fzhhl.top

TS:   arr.map(String)
来源：http://qga.wangshuangyany.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fod.sjlbkw.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zrx.dashuyun.cn

Ruby: arr.map(&:upcase)
来源：http://rml.yanxiufei.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pgv.bjfxy.top

[C08] 闭包
来源：http://gre.sxryk.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lmg.ydjk.org.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mpg.sufxvd.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rrw.hongshengwenyu.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hbu.uphjek.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mws.yj20258.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wcs.yfazqb.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wrb.shanyushiyangkeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vrh.ybcxt.top

[C09] 递归
来源：http://aqv.smart0.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dnb.gaohongyu789.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fmk.meibo888.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fpd.52xcode.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fdr.zhoulong.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jpi.smart0.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wft.jinqigufen.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://avq.hongshengwenyu.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wdo.sjlbkw.cn

[C10] 变量作用域
来源：http://uif.fanxiaobao.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rkn.jiagoushi.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://imm.jinqigfzy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nzc.wangdashe.top

TS:   同 JS
来源：http://yah.yueranfly.top

Java: 方法内为块级作用域
来源：http://fwy.jinyuanbaomall.cn

Go:   花括号块级作用域
来源：http://bje.zhaomingkeji.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yqg.guowangkeji.top

C#:   块级作用域
来源：http://olw.jiagoushi.top

[C11] 模块导入与导出
来源：http://rxj.316326.xyz

Py:   from module import func
来源：http://ljh.zhijiandao.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://gue.ctjpmb.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://wid.gaohongyu789.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jpt.xinyue.icu

Java: import java.util.List;
来源：http://jtr.ydzc1.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yxt.sjlbkw.cn

Ruby: require "json"; require_relative "./util"
来源：http://gzo.yj202588.top

C#:   using System.Text;
来源：http://uap.iojbl.cn

[C12] 立即执行函数 IIFE
来源：http://arw.fengsongda.top

Py:   (lambda: print("run"))()
来源：http://ash.zhongyouzk.top

PHP:  (function () { echo "run"; })();
来源：http://tcv.zdbjq.cn

JS:   (() => { console.log("run"); })();
来源：http://qpx.haohaochexian.top

TS:   (() => { console.log("run"); })();
来源：http://amg.chenzaomai.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hhr.haohaochexian.top

Go:   func() { fmt.Println("run") }()
来源：http://oyf.jinghuilouyu.cn

Ruby: -> { puts "run" }.call
来源：http://ftc.shangyingyoupin.top

C#:   // 无 IIFE：用静态构造函数
来源：http://mzv.jlsjyb.cn

[C13] 类型声明 / 类型注解
来源：http://pba.fengsongda.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rog.hywenlv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nvw.jinyuanbaomall.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wrp.tarul.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lyc.hnxiangtu.top

Java: int add(int a, int b) { return a + b; }
来源：http://lgw.xinyue.icu

Go:   func add(a, b int) int
来源：http://plu.ctjpmb.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wpm.cheryme.top

C#:   int Add(int a, int b) => a + b;
来源：http://itk.hongshengwenyu.top

[C14] 泛型函数
来源：http://kkj.ctjpmb.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nho.cdnleiting.top

PHP:  // 无泛型
来源：http://nom.mhx1999.top

JS:   // 无泛型
来源：http://fnq.gotoacloud.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hwo.xuanzx.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://swa.nwbrower.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cht.cucudq.cn

Ruby: # 无泛型
来源：http://nax.316326.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kud.shanyushiyangtech.top

[C15] 解构 / 展开参数
来源：http://hze.hywenlv.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nsg.wangshuangyany.cn

PHP:  [$a, $b] = $pair;
来源：http://jeu.gogol.net.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lmm.gotoacloud.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bra.pycfn.com

Java: // 无解构
来源：http://afa.xuetiantiany.cn

Go:   // 无解构
来源：http://iiu.sjlbkw.cn

Ruby: a, b = pair
来源：http://tbz.sysykeji.top

C#:   var (a, b) = pair;
来源：http://thu.chenzaomai.com

[C16] 函数 / 方法重载
来源：http://sde.hesvh.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://egf.chenjidiqi.icu

PHP:  // 无重载
来源：http://irc.yj20258.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://hcq.zhijiandao.cn

TS:   // 用联合类型或重载签名声明
来源：http://gtw.nanxuanxn.top

Java: void f(int a) {}  void f(String a) {}
来源：http://bnr.zhixingplan.top

Go:   // 无重载：用不同函数名
来源：http://qov.sxryk.cn

Ruby: # 无重载：靠动态参数
来源：http://hvt.wangdashe.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://iqf.chenjidiqi.icu

================================================================================
来源：http://oef.cdnleiting.top

D. 数组 / 列表 / 集合
来源：http://bwm.ivvv.top

================================================================================
来源：http://mfz.dianchejie.cn

[D01] 创建数组 / 列表
来源：http://yru.xylfe.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://sbj.shuidangran.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fgz.yvedp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ebn.cdnleiting.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://vpj.cashguo.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xwv.hongshengwenyu.top

Go:   arr := []int{1, 2, 3}
来源：http://uln.yj20258.top

Ruby: arr = [1, 2, 3]
来源：http://nou.snrcjt.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kkw.jyoumei.cn

[D02] 追加元素到末尾
来源：http://xtf.zdqjudy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uwu.jinyuanbaomall.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qki.fengsongda.top

JS:   arr.push(4);
来源：http://gee.fanxiaobao.xyz

TS:   arr.push(4);
来源：http://jlx.vehdjk.com

Java: list.add(4);
来源：http://pvz.chenjidiqi.icu

Go:   arr = append(arr, 4)
来源：http://rav.9152youxi.cn

Ruby: arr << 4; arr.push(5)
来源：http://dha.bbcook.cn

C#:   list.Add(4);
来源：http://ovi.gotoacloud.top

[D03] 在指定位置插入元素
来源：http://fju.chenzaomai.com

Py:   arr.insert(0, 0)
来源：http://khu.feifeiyinyue.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://sft.chenzaomai.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uxo.meibo888.top

TS:   arr.splice(0, 0, 0);
来源：http://vis.xingfuxueyuan.xyz

Java: list.add(0, 0);
来源：http://rtl.meibo888.top

Go:   arr = append([]int{0}, arr...)
来源：http://wpm.jqgufenzy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ohd.chenzaomai.com

C#:   list.Insert(0, 0);
来源：http://bwk.ppjwa.cn

[D04] 删除元素
来源：http://ltx.gzhubu.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ygp.fktsv.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rpo.ehwqpu.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ojm.snrcjt.cn

TS:   arr.splice(0, 1);
来源：http://unb.tanke756.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://irk.cheryme.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mwo.tian-w.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://two.zdbjq.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pnm.zhengqikj.top

[D05] 访问与修改元素
来源：http://oag.chenzaomai.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://trd.daria6918.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tvr.sjlbkw.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://alm.ppjwa.cn

TS:   arr[0]; arr.at(-1);
来源：http://zbr.ydjk.org.cn

Java: list.get(0); list.set(0, 9);
来源：http://oia.cdnleiting.top

Go:   arr[0]; arr[0] = 9
来源：http://kva.yongpay.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zjj.dianchejie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wzc.hongshengwenyu.top

[D06] 数组长度
来源：http://day.yuanzhike.top

Py:   len(arr)
来源：http://mdr.cucudq.cn

PHP:  count($arr);
来源：http://fxu.nanxuanxn.top

JS:   arr.length
来源：http://dty.bjfxy.top

TS:   arr.length
来源：http://mfu.pycfn.com

Java: list.size();
来源：http://aut.ydzc1.top

Go:   len(arr)
来源：http://rqj.0kj1m.cn

Ruby: arr.length; arr.size
来源：http://ega.shuidangran.top

C#:   list.Count;
来源：http://rdx.cdnleiting.top

[D07] 切片 / 取子数组
来源：http://kyv.feifeiyinyue.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://omy.yuanzhike.top

PHP:  array_slice($arr, 1, 3);
来源：http://pkc.guannengcc.top

JS:   arr.slice(1, 4);
来源：http://jnr.jiagoushi.top

TS:   arr.slice(1, 4);
来源：http://jfq.pengpengdd.cyou

Java: list.subList(1, 4);
来源：http://uth.cdnleiting.top

Go:   arr[1:4]
来源：http://lek.zycfv.cn

Ruby: arr[1, 3]
来源：http://jnu.yfazqb.com

C#:   list.GetRange(1, 3);
来源：http://bpg.shanyushiyangtech.top

[D08] 合并两个数组
来源：http://hvk.zdbjq.cn

Py:   a + b;  a.extend(b)
来源：http://edl.uphjek.com

PHP:  array_merge($a, $b);
来源：http://tyn.gotoacloud.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ixd.zhiwuduotai.top

TS:   [...a, ...b];
来源：http://aec.ehwqpu.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ubb.aibaodan.cn

Go:   append(a, b...)
来源：http://zni.yuanzhike.top

Ruby: a + b;  a.concat(b)
来源：http://phk.guannengcc.top

C#:   a.Concat(b).ToList()
来源：http://clj.fanxiaobao.xyz

[D09] 排序（升序）
来源：http://dhl.cashguo.top

Py:   sorted(arr);  arr.sort()
来源：http://ewp.ydjk.org.cn

PHP:  sort($arr);
来源：http://flh.fehbvm.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uld.epnwcf.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://zbb.ctjpmb.com

Java: Collections.sort(list);  list.sort(null);
来源：http://avt.hnxiangtu.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://eob.vqdsnc.cn

Ruby: arr.sort
来源：http://bml.vehdjk.com

C#:   list.Sort();
来源：http://iiu.fzhhl.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://cyx.xuanzx.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sgw.jinqigufen.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iof.guannengcc.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://krm.tian-w.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kvf.haohaochexian.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pni.tanke756.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pra.hcnkem.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wbj.xylfe.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vgn.316326.xyz

[D11] 反转数组
来源：http://psn.aibaodan.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wcv.cucudq.cn

PHP:  array_reverse($arr);
来源：http://kpz.aibaodan.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gws.sysykeji.top

TS:   [...arr].reverse();
来源：http://ayt.jinqigufen.top

Java: Collections.reverse(list);
来源：http://gdy.bjfxy.top

Go:   slices.Reverse(arr)
来源：http://opq.pengpengdd.cyou

Ruby: arr.reverse
来源：http://hyh.gogol.net.cn

C#:   list.Reverse();
来源：http://yjy.zhaomingkeji.xyz

[D12] 查找元素下标
来源：http://nka.yueranfly.top

Py:   arr.index(x);  x in arr
来源：http://yut.nanxuanxn.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://owq.ydzc1.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://din.hnqzz.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zgh.hammf.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jzl.havefunace.top

Go:   slices.Index(arr, x)
来源：http://vow.wangshuangyany.cn

Ruby: arr.index(x)
来源：http://xuj.iojbl.cn

C#:   list.IndexOf(x);
来源：http://zcb.ctjpmb.com

[D13] 过滤（保留满足条件的）
来源：http://yhs.hnxiangtu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fwg.yj20258888.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mhw.shuidangran.top

JS:   arr.filter(x => x > 3)
来源：http://vgr.jqgfzy.top

TS:   arr.filter(x => x > 3)
来源：http://erb.vqdsnc.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://oje.jinqigfzy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pgb.hesvh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cbw.birdmap.top

C#:   list.Where(x => x > 3).ToList()
来源：http://oxg.hysaishi.cn

[D14] 映射转换（每个元素变形）
来源：http://vma.gotoacloud.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gdt.quarkkingdee.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rjl.0kj1m.cn

JS:   arr.map(x => x * 2)
来源：http://tyo.aizwys.cn

TS:   arr.map(x => x * 2)
来源：http://spv.fktsv.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://grt.fzhhl.top

Go:   // 手写循环
来源：http://gml.jianghu66.top

Ruby: arr.map { |x| x * 2 }
来源：http://hlh.jqgfzy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ngf.sxryk.cn

[D15] 去重
来源：http://yyu.52xcode.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://azr.mhx1999.top

PHP:  array_unique($arr);
来源：http://rjh.hnqzz.top

JS:   [...new Set(arr)]
来源：http://kyd.redwolf501.top

TS:   [...new Set(arr)]
来源：http://ebx.snrcjt.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tuh.uphjek.com

Go:   // 用 map[T]struct{} 手写
来源：http://kox.gaohongyu789.top

Ruby: arr.uniq
来源：http://rge.ehwqpu.com

C#:   list.Distinct().ToList()
来源：http://zpj.fengsongda.top

[D16] 求和与平均值
来源：http://wtf.jianghu66.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://edi.shanyushiyangkeji.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://edn.zdqjudy.top


<!-- 参考信息 -->