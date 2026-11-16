代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nkd.nanxuanxn.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://chx.jyoumei.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://doc.ppjwa.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uyw.sjlbkw.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ebb.yanxiufei.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pii.hnqzz.top

[C04] 命名参数 / 关键字参数
来源：http://xuc.xuanzx.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mnn.uphjek.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yyn.shanyushiyangtech.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vma.sxryk.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ioz.cucudq.cn

Java: // 无：用 Builder 模式或 record
来源：http://wth.nwbrower.top

Go:   // 无：用配置结构体参数
来源：http://rgw.xingfuxueyuan.xyz

Ruby: f(a: 1, b: 2)
来源：http://fye.daria6918.cn

C#:   f(a: 1, b: 2)
来源：http://ssy.guannengcc.top

[C05] 返回多个值
来源：http://duv.svipenyu.cn

Py:   return a, b
来源：http://zjt.316326.xyz

PHP:  return [$a, $b];
来源：http://dvm.vehdjk.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://xmb.yj20258888.top

TS:   return { a, b };
来源：http://pdf.nanxuanxn.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sqd.shanyushiyangtech.top

Go:   return a, b
来源：http://eyk.shzxlz.cn

Ruby: return a, b
来源：http://usl.pycfn.com

C#:   return (a, b);              // ValueTuple
来源：http://yin.hnxiangtu.top

[C06] 匿名函数 / lambda
来源：http://fvz.52xcode.cn

Py:   square = lambda x: x * x
来源：http://ucg.yvedp.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://kcs.smart0.xyz

JS:   const square = x => x * x;
来源：http://vkd.cucudq.cn

TS:   const square = (x: number): number => x * x;
来源：http://phc.sxryk.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sjs.zdbjq.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zbb.iojbl.cn

Ruby: square = ->(x) { x * x }
来源：http://cud.wangshuangyany.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xrn.jyoumei.cn

[C07] 把函数作为参数传入
来源：http://swo.gaohongyu789.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wvi.nanxinkj.top

PHP:  array_map("strtoupper", $arr);
来源：http://mra.fengsongda.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ifo.fzhhl.top

TS:   arr.map(String)
来源：http://ipy.xinyue.icu

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wiv.sweek.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qmb.yongpay.top

Ruby: arr.map(&:upcase)
来源：http://dny.xziqi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cvp.iojbl.cn

[C08] 闭包
来源：http://jdj.jqgufenzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://crx.kuanghao11.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ysy.yuxming.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://twr.hcnkem.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jlj.svipenyu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bzm.daria6918.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gko.redwolf501.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uek.wangdashe.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xpg.gogol.net.cn

[C09] 递归
来源：http://jrm.feifeiyinyue.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://aid.hywenlv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://arf.aizwys.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tnd.chenjidiqi.icu

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vli.gogol.net.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gvn.aizwys.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sly.zdqjudy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qqd.pycfn.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cvj.sweek.top

[C10] 变量作用域
来源：http://kke.sweek.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://oyk.52xcode.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tyz.9152youxi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xux.hongshengwenyu.top

TS:   同 JS
来源：http://rkc.havefunace.top

Java: 方法内为块级作用域
来源：http://yzr.guannengcc.top

Go:   花括号块级作用域
来源：http://mow.shuidangran.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mhp.fanxiaobao.xyz

C#:   块级作用域
来源：http://lik.daxiang520.top

[C11] 模块导入与导出
来源：http://ukz.wangdashe.top

Py:   from module import func
来源：http://web.sufxvd.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ako.yvedp.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kea.nwbrower.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nrx.fengsongda.top

Java: import java.util.List;
来源：http://pvp.hfpthk.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nwr.cucudq.cn

Ruby: require "json"; require_relative "./util"
来源：http://lxi.dianchejie.cn

C#:   using System.Text;
来源：http://xou.jyoumei.cn

[C12] 立即执行函数 IIFE
来源：http://wiz.shuidangran.top

Py:   (lambda: print("run"))()
来源：http://hfl.pengpengdd.cyou

PHP:  (function () { echo "run"; })();
来源：http://gtw.9152youxi.cn

JS:   (() => { console.log("run"); })();
来源：http://czv.tian-w.cn

TS:   (() => { console.log("run"); })();
来源：http://dbt.yuanzhike.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jqa.gzhubu.top

Go:   func() { fmt.Println("run") }()
来源：http://cnv.fzhhl.top

Ruby: -> { puts "run" }.call
来源：http://knc.yvedp.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fro.xziqi.cn

[C13] 类型声明 / 类型注解
来源：http://rjb.tanke756.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ehq.c1oappe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kls.cheryme.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fch.shuidangran.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hzw.kuanghao11.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mhg.hywenlv.cn

Go:   func add(a, b int) int
来源：http://lky.cqqwz.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uzn.fzhhl.top

C#:   int Add(int a, int b) => a + b;
来源：http://skx.zhixingplan.top

[C14] 泛型函数
来源：http://tut.ivvv.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://slh.gogol.net.cn

PHP:  // 无泛型
来源：http://wub.yj202588.top

JS:   // 无泛型
来源：http://tef.gzhubu.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yfn.cdnleiting.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hys.sxryk.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lua.tarul.cn

Ruby: # 无泛型
来源：http://cpg.zdbjq.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rnm.vehdjk.com

[C15] 解构 / 展开参数
来源：http://gab.jinqigufen.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rdn.daria6918.cn

PHP:  [$a, $b] = $pair;
来源：http://olz.zdqjudy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ffs.snrcjt.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jch.nanxinkj.top

Java: // 无解构
来源：http://dvr.jqgfzy.top

Go:   // 无解构
来源：http://vzm.hnqzz.top

Ruby: a, b = pair
来源：http://ptc.tarul.cn

C#:   var (a, b) = pair;
来源：http://yab.sjlbkw.cn

[C16] 函数 / 方法重载
来源：http://cbg.gogol.net.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://laa.fktsv.cn

PHP:  // 无重载
来源：http://vvf.yuxming.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://beg.zhixingplan.top

TS:   // 用联合类型或重载签名声明
来源：http://awp.jlsjyb.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://kpf.yj20258888.top

Go:   // 无重载：用不同函数名
来源：http://lgq.fktsv.cn

Ruby: # 无重载：靠动态参数
来源：http://drp.jinqigufen.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://rwo.jyoumei.cn

================================================================================
来源：http://nwf.yonumen.top

D. 数组 / 列表 / 集合
来源：http://fxe.mhx1999.top

================================================================================
来源：http://pqb.hnqzz.top

[D01] 创建数组 / 列表
来源：http://lot.meibo888.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://plb.jinghuilouyu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xzx.daria6918.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dwn.zhiwuduotai.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ahz.fengsongda.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fmw.yj20258.top

Go:   arr := []int{1, 2, 3}
来源：http://ska.tianlin.xyz

Ruby: arr = [1, 2, 3]
来源：http://dqc.0kj1m.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tyq.yuanzhike.top

[D02] 追加元素到末尾
来源：http://zxk.tanke756.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mam.nwbrower.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ofw.jlsjyb.cn

JS:   arr.push(4);
来源：http://wyr.shuidangran.top

TS:   arr.push(4);
来源：http://qua.xingfuxueyuan.xyz

Java: list.add(4);
来源：http://tuz.cucudq.cn

Go:   arr = append(arr, 4)
来源：http://ati.ehwqpu.com

Ruby: arr << 4; arr.push(5)
来源：http://qqi.svipenyu.cn

C#:   list.Add(4);
来源：http://qfp.sxryk.cn

[D03] 在指定位置插入元素
来源：http://gud.shzxlz.cn

Py:   arr.insert(0, 0)
来源：http://tjw.wangshuangyany.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vfl.cdnleiting.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cny.hywenlv.cn

TS:   arr.splice(0, 0, 0);
来源：http://tka.shuidangran.top

Java: list.add(0, 0);
来源：http://dtf.316326.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://ett.zhongyouzk.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gmz.hammf.cn

C#:   list.Insert(0, 0);
来源：http://cjf.9152youxi.cn

[D04] 删除元素
来源：http://gro.zhengqikj.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jvj.xuetiantiany.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lva.kuanghao11.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xot.hammf.cn

TS:   arr.splice(0, 1);
来源：http://nau.kuanghao11.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gst.wangshuangyany.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xfq.gaohongyu789.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ikz.snrcjt.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://enq.jinqigufen.top

[D05] 访问与修改元素
来源：http://gac.uphjek.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ziv.fktsv.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hco.haohaochexian.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rgk.tian-w.cn

TS:   arr[0]; arr.at(-1);
来源：http://swz.jinyuanbaomall.cn

Java: list.get(0); list.set(0, 9);
来源：http://hpc.pengpengdd.cyou

Go:   arr[0]; arr[0] = 9
来源：http://xpb.sysykeji.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dfs.wangshuangyany.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hdc.tanke756.top

[D06] 数组长度
来源：http://jqa.cdnleiting.top

Py:   len(arr)
来源：http://jal.yuxming.cn

PHP:  count($arr);
来源：http://xqv.cucudq.cn

JS:   arr.length
来源：http://eeg.guowangkeji.top

TS:   arr.length
来源：http://rer.redwolf501.top

Java: list.size();
来源：http://vhf.ywan-chungtsiang.top

Go:   len(arr)
来源：http://ani.xuetiantiany.cn

Ruby: arr.length; arr.size
来源：http://ofe.tian-w.cn

C#:   list.Count;
来源：http://beh.jianghu66.top

[D07] 切片 / 取子数组
来源：http://xjs.52xcode.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rfk.cheryme.top

PHP:  array_slice($arr, 1, 3);
来源：http://fga.yuanzhike.top

JS:   arr.slice(1, 4);
来源：http://qoi.yanxiufei.cn

TS:   arr.slice(1, 4);
来源：http://fea.nwbrower.top

Java: list.subList(1, 4);
来源：http://pbj.svipenyu.cn

Go:   arr[1:4]
来源：http://ghp.fengsongda.top

Ruby: arr[1, 3]
来源：http://jdw.c1oappe.top

C#:   list.GetRange(1, 3);
来源：http://hte.ydjk.org.cn

[D08] 合并两个数组
来源：http://msl.jinghuilouyu.cn

Py:   a + b;  a.extend(b)
来源：http://don.yj20258888.top

PHP:  array_merge($a, $b);
来源：http://ist.hysaishi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xxr.jlsjyb.cn

TS:   [...a, ...b];
来源：http://mrc.fktsv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tzf.mhx1999.top

Go:   append(a, b...)
来源：http://qzg.quarkkingdee.top

Ruby: a + b;  a.concat(b)
来源：http://onz.shanyushiyangtech.top

C#:   a.Concat(b).ToList()
来源：http://bki.xylfe.cn

[D09] 排序（升序）
来源：http://ysr.iojbl.cn

Py:   sorted(arr);  arr.sort()
来源：http://cbp.jlsjyb.cn

PHP:  sort($arr);
来源：http://bud.havefunace.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jov.zhaomingkeji.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://ahj.zhengqikj.top

Java: Collections.sort(list);  list.sort(null);
来源：http://kms.nwbrower.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://imu.dashuyun.cn

Ruby: arr.sort
来源：http://bgu.xylfe.cn

C#:   list.Sort();
来源：http://hpr.gzhubu.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ugl.zhiwuduotai.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bch.zdqjudy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rqt.c1oappe.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dud.fengsongda.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nww.hcnkem.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xij.xuetiantiany.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qil.ydjk.org.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://aqk.gotoacloud.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ura.cucudq.cn

[D11] 反转数组
来源：http://vya.smart0.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://gog.hcnkem.com

PHP:  array_reverse($arr);
来源：http://sun.uphjek.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hxh.jinqigufen.top

TS:   [...arr].reverse();
来源：http://xra.zhaomingkeji.xyz

Java: Collections.reverse(list);
来源：http://xhy.zhijiandao.cn

Go:   slices.Reverse(arr)
来源：http://iqb.hnxiangtu.top

Ruby: arr.reverse
来源：http://tbe.fehbvm.com

C#:   list.Reverse();
来源：http://teb.hcnkem.com

[D12] 查找元素下标
来源：http://obg.tianlin.xyz

Py:   arr.index(x);  x in arr
来源：http://vov.quarkkingdee.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://psj.guannengcc.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kzx.yongpay.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wwe.chenzaomai.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vyk.hysaishi.cn

Go:   slices.Index(arr, x)
来源：http://oql.jqgufenzy.top

Ruby: arr.index(x)
来源：http://vce.ydzc1.top

C#:   list.IndexOf(x);
来源：http://vre.hongshengwenyu.top

[D13] 过滤（保留满足条件的）
来源：http://bqx.mhx1999.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ysp.aizwys.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ugu.birdmap.top

JS:   arr.filter(x => x > 3)
来源：http://vhw.hywenlv.cn

TS:   arr.filter(x => x > 3)
来源：http://czr.hammf.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jlc.pengpengdd.cyou

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ugs.xinyue.icu

Ruby: arr.select { |x| x > 3 }
来源：http://ipd.hesvh.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://dxo.cqqwz.cn

[D14] 映射转换（每个元素变形）
来源：http://ilo.gotoacloud.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mbv.ppjwa.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uqm.xuanzx.com

JS:   arr.map(x => x * 2)
来源：http://tjj.cucudq.cn

TS:   arr.map(x => x * 2)
来源：http://crm.hongshengwenyu.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://qzh.fktsv.cn

Go:   // 手写循环
来源：http://bkg.sjlbkw.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zbf.xinyue.icu

C#:   list.Select(x => x * 2).ToList()
来源：http://vsc.tanke756.top

[D15] 去重
来源：http://kjh.ctjpmb.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cuz.shangyingyoupin.top

PHP:  array_unique($arr);
来源：http://wyw.haohaochexian.top

JS:   [...new Set(arr)]
来源：http://ohr.kuanghao11.cn

TS:   [...new Set(arr)]
来源：http://ble.316326.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gkj.jqgfzy.top

Go:   // 用 map[T]struct{} 手写
来源：http://skt.yongpay.top

Ruby: arr.uniq
来源：http://avq.hesvh.cn

C#:   list.Distinct().ToList()
来源：http://vwv.nanxinkj.top

[D16] 求和与平均值
来源：http://bre.andypj.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://czu.hongshengwenyu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ppa.zhiwuduotai.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wsq.yangfankeji.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jpi.snrcjt.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mih.shzxlz.cn

Go:   // 手写循环累加
来源：http://iaw.yuanzhike.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sdp.aizwys.cn

C#:   list.Sum();  list.Average()
来源：http://lxm.chenzaomai.com

[D17] 最大值与最小值
来源：http://khw.wangdashe.top

Py:   max(arr);  min(arr)
来源：http://gtm.ydzc1.top

PHP:  max($arr);  min($arr);
来源：http://zov.zhiwuduotai.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tck.xuetiantiany.cn

TS:   Math.max(...arr);
来源：http://qtm.shzxlz.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://soa.andypj.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qls.fanxiaobao.xyz

Ruby: arr.max;  arr.min
来源：http://sic.feifeiyinyue.top

C#:   list.Max();  list.Min()
来源：http://xyi.9152youxi.cn

[D18] 扁平化嵌套数组
来源：http://ooo.cdnleiting.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fck.cdnleiting.top

PHP:  array_merge(...$nested);
来源：http://gsk.yj20258.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ucz.jinqigufen.top

TS:   nested.flat();
来源：http://cav.nwbrower.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lbh.tianlin.xyz

Go:   // 手写双层循环
来源：http://uoi.daxiang520.top

Ruby: nested.flatten
来源：http://ejz.zhongyouzk.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ogh.kuanghao11.cn

[D19] 按字段分组
来源：http://irv.hnqzz.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jgc.redwolf501.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qcx.quarkkingdee.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dsp.snrcjt.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jff.bjfxy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rlg.cheryme.top

Go:   // 手写 map[string][]T
来源：http://pqx.bjfxy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://nso.aibaodan.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bny.tian-w.cn

[D20] 统计每个元素出现次数
来源：http://mmg.jiagoushi.top

Py:   Counter(arr)
来源：http://gau.yueranfly.top

PHP:  array_count_values($arr);
来源：http://vmu.ywan-chungtsiang.top


<!-- 参考信息 -->