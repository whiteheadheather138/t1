代发 wailian999

Java: if (data == null) return;
来源：http://jmv.zhongyouzk.top

Go:   if data == nil { return }
来源：http://gry.jqgufenzy.top

Ruby: return if data.nil?
来源：http://aqw.sjlbkw.cn

C#:   if (data == null) return;
来源：http://rrb.xziqi.cn

================================================================================
来源：http://dcc.bbcook.cn

C. 函数与作用域
来源：http://bdb.feifeiyinyue.top

================================================================================
来源：http://vii.tanke756.top

[C01] 定义函数
来源：http://mvy.ivvv.top

Py:   def add(a, b): return a + b
来源：http://qbp.redwolf501.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oyg.guannengcc.top

JS:   function add(a, b) { return a + b; }
来源：http://hul.cdnleiting.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cxu.svipenyu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ega.yfazqb.com

Go:   func add(a, b int) int { return a + b }
来源：http://lwt.jinghuilouyu.cn

Ruby: def add(a, b); a + b; end
来源：http://lzx.yuxming.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dtt.daxiang520.top

[C02] 默认参数
来源：http://svg.sjlbkw.cn

Py:   def greet(name="World"): return name
来源：http://gtn.aibaodan.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://rwx.quarkkingdee.top

JS:   function greet(name = "World") { return name; }
来源：http://ojp.nanxinkj.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ocy.ehwqpu.com

Java: // 无默认参数：方法重载或 Optional
来源：http://dfp.cucudq.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dok.feifeiyinyue.top

Ruby: def greet(name = "World") = name
来源：http://prv.zhongyouzk.top

C#:   string Greet(string name = "World") => name;
来源：http://aaz.zdbjq.cn

[C03] 可变参数
来源：http://mvt.haohaochexian.top

Py:   def total(*args): return sum(args)
来源：http://kpb.zhaomingkeji.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pjp.smart0.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hne.tarul.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zjc.quarkkingdee.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mzy.mhx1999.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tdi.vqdsnc.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ekd.shangyingyoupin.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rgq.ybcxt.top

[C04] 命名参数 / 关键字参数
来源：http://xwg.yfazqb.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://omd.cheryme.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://buu.fengsongda.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nhx.daxiang520.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vsg.c1oappe.top

Java: // 无：用 Builder 模式或 record
来源：http://tpu.xziqi.cn

Go:   // 无：用配置结构体参数
来源：http://psf.hammf.cn

Ruby: f(a: 1, b: 2)
来源：http://qgr.yangfankeji.com

C#:   f(a: 1, b: 2)
来源：http://bmm.daria6918.cn

[C05] 返回多个值
来源：http://dbc.jlsjyb.cn

Py:   return a, b
来源：http://pto.hywenlv.cn

PHP:  return [$a, $b];
来源：http://kry.fengsongda.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://fqp.ybcxt.top

TS:   return { a, b };
来源：http://xcg.cqqwz.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dsk.yuanzhike.top

Go:   return a, b
来源：http://tvd.gotoacloud.top

Ruby: return a, b
来源：http://juh.hongshengwenyu.top

C#:   return (a, b);              // ValueTuple
来源：http://ivm.tarul.cn

[C06] 匿名函数 / lambda
来源：http://uff.bbcook.cn

Py:   square = lambda x: x * x
来源：http://ilo.fengsongda.top

PHP:  $square = fn($x) => $x * $x;
来源：http://vvy.fengsongda.top

JS:   const square = x => x * x;
来源：http://hjd.vehdjk.com

TS:   const square = (x: number): number => x * x;
来源：http://vcq.guannengcc.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://srt.mhx1999.top

Go:   sq := func(x int) int { return x * x }
来源：http://zsy.zhoulong.xyz

Ruby: square = ->(x) { x * x }
来源：http://sum.chenzaomai.com

C#:   Func<int, int> square = x => x * x;
来源：http://sly.xuetiantiany.cn

[C07] 把函数作为参数传入
来源：http://uex.birdmap.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://agj.xylfe.cn

PHP:  array_map("strtoupper", $arr);
来源：http://nli.meibo888.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dqe.hesvh.cn

TS:   arr.map(String)
来源：http://spa.ybcxt.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nid.hcnkem.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vbj.mhx1999.top

Ruby: arr.map(&:upcase)
来源：http://zwx.316326.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://hiy.0kj1m.cn

[C08] 闭包
来源：http://eme.shanyushiyangkeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cmn.kuanghao11.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://iiy.snrcjt.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zsr.jiagoushi.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mep.wangdashe.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://amv.snrcjt.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://atc.jiagoushi.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ddw.fehbvm.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hny.iojbl.cn

[C09] 递归
来源：http://aox.gogol.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://urh.316326.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vmt.hywenlv.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://znq.gotoacloud.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ltt.ydzc1.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zpl.pycfn.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pdc.shangyingyoupin.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mje.ppjwa.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://enu.meibo888.top

[C10] 变量作用域
来源：http://wac.uphjek.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://omr.ppjwa.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://afq.tanke756.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gza.ehwqpu.com

TS:   同 JS
来源：http://tmi.guowangkeji.top

Java: 方法内为块级作用域
来源：http://hyu.bjfxy.top

Go:   花括号块级作用域
来源：http://xsx.chenlongwang.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kik.yuanzhike.top

C#:   块级作用域
来源：http://bic.redwolf501.top

[C11] 模块导入与导出
来源：http://bgi.cucudq.cn

Py:   from module import func
来源：http://mmf.redwolf501.top

PHP:  require "file.php";  或 use App\Service;
来源：http://gai.xuetiantiany.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vus.svipenyu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://avj.xinyue.icu

Java: import java.util.List;
来源：http://oqc.haohaochexian.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://eno.chenlongwang.top

Ruby: require "json"; require_relative "./util"
来源：http://ong.uphjek.com

C#:   using System.Text;
来源：http://xgv.bjfxy.top

[C12] 立即执行函数 IIFE
来源：http://kgp.zhaomingkeji.xyz

Py:   (lambda: print("run"))()
来源：http://cot.pycfn.com

PHP:  (function () { echo "run"; })();
来源：http://tmo.hnqzz.top

JS:   (() => { console.log("run"); })();
来源：http://etz.fengsongda.top

TS:   (() => { console.log("run"); })();
来源：http://dbi.jyoumei.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xyq.jinqigufen.top

Go:   func() { fmt.Println("run") }()
来源：http://weq.tarul.cn

Ruby: -> { puts "run" }.call
来源：http://rkv.chenzaomai.com

C#:   // 无 IIFE：用静态构造函数
来源：http://zbh.chenlongwang.top

[C13] 类型声明 / 类型注解
来源：http://mxz.yanxiufei.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xfl.zhongyouzk.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jfx.feifeiyinyue.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qun.yj202588.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jqv.hesvh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mxq.zhoulong.xyz

Go:   func add(a, b int) int
来源：http://eyi.zhoulong.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nci.hcnkem.com

C#:   int Add(int a, int b) => a + b;
来源：http://pkt.xylfe.cn

[C14] 泛型函数
来源：http://rtd.ybcxt.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bjt.yvedp.cn

PHP:  // 无泛型
来源：http://lbi.jinqigufen.top

JS:   // 无泛型
来源：http://php.316326.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hcv.sjlbkw.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ylb.aibaodan.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xvs.zhoulong.xyz

Ruby: # 无泛型
来源：http://cdz.nwbrower.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mco.yongpay.top

[C15] 解构 / 展开参数
来源：http://suc.xylfe.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://imq.hesvh.cn

PHP:  [$a, $b] = $pair;
来源：http://ipn.9152youxi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vat.shanyushiyangtech.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wcb.sjlbkw.cn

Java: // 无解构
来源：http://dzx.cqqwz.cn

Go:   // 无解构
来源：http://lri.hnqzz.top

Ruby: a, b = pair
来源：http://hmh.ehwqpu.com

C#:   var (a, b) = pair;
来源：http://zoa.jianghu66.top

[C16] 函数 / 方法重载
来源：http://kgv.hongshengwenyu.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://eyl.redwolf501.top

PHP:  // 无重载
来源：http://bjl.jlsjyb.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qps.zdbjq.cn

TS:   // 用联合类型或重载签名声明
来源：http://qyk.xziqi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xjt.dashuyun.cn

Go:   // 无重载：用不同函数名
来源：http://dec.ivvv.top

Ruby: # 无重载：靠动态参数
来源：http://qkx.zhijiandao.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://crv.smart0.xyz

================================================================================
来源：http://aud.guannengcc.top

D. 数组 / 列表 / 集合
来源：http://pwd.feifeiyinyue.top

================================================================================
来源：http://nac.shanyushiyangkeji.top

[D01] 创建数组 / 列表
来源：http://qoc.feifeiyinyue.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://lfh.yuxming.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cug.bbcook.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nys.jyoumei.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://snx.birdmap.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lft.9152youxi.cn

Go:   arr := []int{1, 2, 3}
来源：http://fak.wangdashe.top

Ruby: arr = [1, 2, 3]
来源：http://wws.yfazqb.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://owj.quarkkingdee.top

[D02] 追加元素到末尾
来源：http://rth.yuanzhike.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uxg.yonumen.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vbw.birdmap.top

JS:   arr.push(4);
来源：http://ylb.jlsjyb.cn

TS:   arr.push(4);
来源：http://svb.dianchejie.cn

Java: list.add(4);
来源：http://iiq.c1oappe.top

Go:   arr = append(arr, 4)
来源：http://yze.jinyuanbaomall.cn

Ruby: arr << 4; arr.push(5)
来源：http://bug.nanxinkj.top

C#:   list.Add(4);
来源：http://bgu.bjfxy.top

[D03] 在指定位置插入元素
来源：http://mie.sjlbkw.cn

Py:   arr.insert(0, 0)
来源：http://rcu.yj20258888.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gav.cqqwz.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gxb.cashguo.top

TS:   arr.splice(0, 0, 0);
来源：http://max.shangyingyoupin.top

Java: list.add(0, 0);
来源：http://yta.epnwcf.com

Go:   arr = append([]int{0}, arr...)
来源：http://joc.dianchejie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hgm.epnwcf.com

C#:   list.Insert(0, 0);
来源：http://flb.ywan-chungtsiang.top

[D04] 删除元素
来源：http://mne.iojbl.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uiv.fengsongda.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://oun.andypj.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jji.xziqi.cn

TS:   arr.splice(0, 1);
来源：http://wwr.zdbjq.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jbl.chenzaomai.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qax.cqqwz.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lzr.sweek.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cea.ydzc1.top

[D05] 访问与修改元素
来源：http://exy.bbcook.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lxw.jianghu66.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hao.dashuyun.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bff.ctjpmb.com

TS:   arr[0]; arr.at(-1);
来源：http://vny.9152youxi.cn

Java: list.get(0); list.set(0, 9);
来源：http://agw.yfazqb.com

Go:   arr[0]; arr[0] = 9
来源：http://tgf.c1oappe.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fwv.tarul.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gef.sxryk.cn

[D06] 数组长度
来源：http://tfg.epnwcf.com

Py:   len(arr)
来源：http://hqo.jyoumei.cn

PHP:  count($arr);
来源：http://awe.jlsjyb.cn

JS:   arr.length
来源：http://fms.yonumen.top

TS:   arr.length
来源：http://cfo.uphjek.com

Java: list.size();
来源：http://axp.zhoulong.xyz

Go:   len(arr)
来源：http://bxt.tian-w.cn

Ruby: arr.length; arr.size
来源：http://eiw.birdmap.top

C#:   list.Count;
来源：http://xvf.ybcxt.top

[D07] 切片 / 取子数组
来源：http://kgj.sweek.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sks.sufxvd.cn

PHP:  array_slice($arr, 1, 3);
来源：http://auk.gaohongyu789.top

JS:   arr.slice(1, 4);
来源：http://pys.xingfuxueyuan.xyz

TS:   arr.slice(1, 4);
来源：http://lmc.fengsongda.top

Java: list.subList(1, 4);
来源：http://zug.chenjidiqi.icu

Go:   arr[1:4]
来源：http://bwi.0kj1m.cn

Ruby: arr[1, 3]
来源：http://pwt.guannengcc.top

C#:   list.GetRange(1, 3);
来源：http://bjt.meibo888.top

[D08] 合并两个数组
来源：http://pky.bbcook.cn

Py:   a + b;  a.extend(b)
来源：http://beb.meibo888.top

PHP:  array_merge($a, $b);
来源：http://yav.kuanghao11.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hrm.cqqwz.cn

TS:   [...a, ...b];
来源：http://bvj.ybcxt.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://amt.jinghuilouyu.cn

Go:   append(a, b...)
来源：http://sae.bjfxy.top

Ruby: a + b;  a.concat(b)
来源：http://qge.shuidangran.top

C#:   a.Concat(b).ToList()
来源：http://yab.nanxinkj.top

[D09] 排序（升序）
来源：http://tjz.pycfn.com

Py:   sorted(arr);  arr.sort()
来源：http://ohv.sufxvd.cn

PHP:  sort($arr);
来源：http://bik.shanyushiyangkeji.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wlr.xingfuxueyuan.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://wop.ppjwa.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://fvi.shanyushiyangkeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rpc.fktsv.cn

Ruby: arr.sort
来源：http://gnv.jinyuanbaomall.cn

C#:   list.Sort();
来源：http://vgi.xziqi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://gsg.sxryk.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zxb.cdnleiting.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nkl.hesvh.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://urg.shanyushiyangkeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lfq.ydzc1.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tof.zhengqikj.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bwf.nanxinkj.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lod.zhiwuduotai.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zxe.daxiang520.top

[D11] 反转数组
来源：http://xkq.wangshuangyany.cn

Py:   arr[::-1];  arr.reverse()
来源：http://kne.gogol.net.cn

PHP:  array_reverse($arr);
来源：http://tls.cheryme.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rem.kuanghao11.cn

TS:   [...arr].reverse();
来源：http://jzl.redwolf501.top

Java: Collections.reverse(list);
来源：http://gsn.zdqjudy.top

Go:   slices.Reverse(arr)
来源：http://fyv.jianghu66.top

Ruby: arr.reverse
来源：http://rpt.yj202588.top

C#:   list.Reverse();
来源：http://iwc.jinyuanbaomall.cn

[D12] 查找元素下标
来源：http://soy.xylfe.cn

Py:   arr.index(x);  x in arr
来源：http://cwx.shangyingyoupin.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ngb.fengsongda.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gfl.52xcode.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dfc.sufxvd.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xpi.fktsv.cn

Go:   slices.Index(arr, x)
来源：http://kme.zycfv.cn

Ruby: arr.index(x)
来源：http://wtg.shangyingyoupin.top

C#:   list.IndexOf(x);
来源：http://kio.wangdashe.top

[D13] 过滤（保留满足条件的）
来源：http://jus.nanxinkj.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vjc.fengsongda.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://veg.jinghuilouyu.cn

JS:   arr.filter(x => x > 3)
来源：http://rli.snrcjt.cn

TS:   arr.filter(x => x > 3)
来源：http://gwz.shangyingyoupin.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://avi.gzhubu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://iij.yuxming.cn

Ruby: arr.select { |x| x > 3 }
来源：http://upp.tianlin.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://gct.cucudq.cn

[D14] 映射转换（每个元素变形）
来源：http://fds.xziqi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ejp.chenlongwang.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qzb.ppjwa.cn

JS:   arr.map(x => x * 2)
来源：http://fnr.jianghu66.top

TS:   arr.map(x => x * 2)
来源：http://ndh.meibo888.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://uvv.nwbrower.top

Go:   // 手写循环
来源：http://pvm.iojbl.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qpw.zhaomingkeji.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://cll.hnqzz.top

[D15] 去重
来源：http://aep.yuxming.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://imo.ppjwa.cn

PHP:  array_unique($arr);
来源：http://msk.aizwys.cn

JS:   [...new Set(arr)]
来源：http://wxs.yangfankeji.com

TS:   [...new Set(arr)]
来源：http://cfb.xingfuxueyuan.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fnh.shzxlz.cn

Go:   // 用 map[T]struct{} 手写
来源：http://kys.nwbrower.top

Ruby: arr.uniq
来源：http://dro.fktsv.cn

C#:   list.Distinct().ToList()
来源：http://agn.chenlongwang.top

[D16] 求和与平均值
来源：http://aey.yonumen.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ytd.yj20258888.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yqd.chenzaomai.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://aug.zhixingplan.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ime.yueranfly.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ayg.haohaochexian.top

Go:   // 手写循环累加
来源：http://hyb.ehwqpu.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mjc.tianlin.xyz

C#:   list.Sum();  list.Average()
来源：http://imf.quarkkingdee.top

[D17] 最大值与最小值
来源：http://htf.cashguo.top

Py:   max(arr);  min(arr)
来源：http://vci.zhijiandao.cn


<!-- 参考信息 -->