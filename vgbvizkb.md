代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xms.bbcook.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://suv.gaohongyu789.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://axi.xziqi.cn

Java: // 无：用 Builder 模式或 record
来源：http://fom.tianlin.xyz

Go:   // 无：用配置结构体参数
来源：http://fck.sufxvd.cn

Ruby: f(a: 1, b: 2)
来源：http://ddj.svipenyu.cn

C#:   f(a: 1, b: 2)
来源：http://wvx.shanyushiyangtech.top

[C05] 返回多个值
来源：http://osj.pycfn.com

Py:   return a, b
来源：http://whq.xziqi.cn

PHP:  return [$a, $b];
来源：http://dob.yanxiufei.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://tia.zdbjq.cn

TS:   return { a, b };
来源：http://kgx.yangfankeji.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://quf.guannengcc.top

Go:   return a, b
来源：http://yht.316326.xyz

Ruby: return a, b
来源：http://bmb.ehwqpu.com

C#:   return (a, b);              // ValueTuple
来源：http://qjz.redwolf501.top

[C06] 匿名函数 / lambda
来源：http://ktt.chenlongwang.top

Py:   square = lambda x: x * x
来源：http://jps.andypj.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://pkv.xylfe.cn

JS:   const square = x => x * x;
来源：http://ett.sweek.top

TS:   const square = (x: number): number => x * x;
来源：http://vzb.cqqwz.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wkc.haohaochexian.top

Go:   sq := func(x int) int { return x * x }
来源：http://zoz.jinghuilouyu.cn

Ruby: square = ->(x) { x * x }
来源：http://crw.xuetiantiany.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ytn.shangyingyoupin.top

[C07] 把函数作为参数传入
来源：http://zsm.meibo888.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wgj.gotoacloud.top

PHP:  array_map("strtoupper", $arr);
来源：http://gaa.kuanghao11.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pju.daxiang520.top

TS:   arr.map(String)
来源：http://axv.52xcode.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qyf.jinghuilouyu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://awg.sweek.top

Ruby: arr.map(&:upcase)
来源：http://vxz.daxiang520.top

C#:   arr.Select(s => s.ToUpper())
来源：http://cak.ywan-chungtsiang.top

[C08] 闭包
来源：http://wlx.jqgufenzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://sai.zhongyouzk.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xyy.redwolf501.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tcg.yuxming.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ker.shanyushiyangkeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://oin.sxryk.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ddz.zhoulong.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hjj.jinqigfzy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hey.meibo888.top

[C09] 递归
来源：http://onz.sxryk.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ryo.tanke756.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zhh.wangshuangyany.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://whq.yuxming.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uxn.xuetiantiany.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xps.xinyue.icu

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hau.smart0.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ldl.shanyushiyangkeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cfr.sxryk.cn

[C10] 变量作用域
来源：http://hsm.jinyuanbaomall.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qep.sufxvd.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mqw.ehwqpu.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://owq.tanke756.top

TS:   同 JS
来源：http://mxi.c1oappe.top

Java: 方法内为块级作用域
来源：http://voc.mhx1999.top

Go:   花括号块级作用域
来源：http://ryk.tanke756.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ytz.nanxinkj.top

C#:   块级作用域
来源：http://tys.hongshengwenyu.top

[C11] 模块导入与导出
来源：http://sak.cdnleiting.top

Py:   from module import func
来源：http://vrx.svipenyu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://flb.tanke756.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://uzc.dianchejie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rzy.sjlbkw.cn

Java: import java.util.List;
来源：http://fmi.yanxiufei.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://oue.zhongyouzk.top

Ruby: require "json"; require_relative "./util"
来源：http://lku.jinghuilouyu.cn

C#:   using System.Text;
来源：http://sxl.sufxvd.cn

[C12] 立即执行函数 IIFE
来源：http://yth.52xcode.cn

Py:   (lambda: print("run"))()
来源：http://evq.0kj1m.cn

PHP:  (function () { echo "run"; })();
来源：http://kbo.yj20258.top

JS:   (() => { console.log("run"); })();
来源：http://rhj.yongpay.top

TS:   (() => { console.log("run"); })();
来源：http://ueo.feifeiyinyue.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://eak.ywan-chungtsiang.top

Go:   func() { fmt.Println("run") }()
来源：http://dsx.nanxuanxn.top

Ruby: -> { puts "run" }.call
来源：http://ejz.meibo888.top

C#:   // 无 IIFE：用静态构造函数
来源：http://yxb.hysaishi.cn

[C13] 类型声明 / 类型注解
来源：http://ind.pengpengdd.cyou

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zlg.uphjek.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://teh.chenlongwang.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fdl.haohaochexian.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pgb.zhixingplan.top

Java: int add(int a, int b) { return a + b; }
来源：http://ara.meibo888.top

Go:   func add(a, b int) int
来源：http://min.jyoumei.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bmj.nanxuanxn.top

C#:   int Add(int a, int b) => a + b;
来源：http://pmr.daria6918.cn

[C14] 泛型函数
来源：http://rvx.shzxlz.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zwk.jinqigufen.top

PHP:  // 无泛型
来源：http://omi.jlsjyb.cn

JS:   // 无泛型
来源：http://aec.smart0.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gvs.tianlin.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xif.nanxuanxn.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kba.haohaochexian.top

Ruby: # 无泛型
来源：http://jsm.pycfn.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fxy.zhoulong.xyz

[C15] 解构 / 展开参数
来源：http://tvb.hcnkem.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lzg.tanke756.top

PHP:  [$a, $b] = $pair;
来源：http://qco.aizwys.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pyl.fehbvm.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cdc.zdqjudy.top

Java: // 无解构
来源：http://tzf.zdqjudy.top

Go:   // 无解构
来源：http://edb.jinghuilouyu.cn

Ruby: a, b = pair
来源：http://kji.zdbjq.cn

C#:   var (a, b) = pair;
来源：http://zlj.yvedp.cn

[C16] 函数 / 方法重载
来源：http://dft.tarul.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nfl.yj202588.top

PHP:  // 无重载
来源：http://jkl.tarul.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ltm.redwolf501.top

TS:   // 用联合类型或重载签名声明
来源：http://bfo.jinghuilouyu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://emn.hnqzz.top

Go:   // 无重载：用不同函数名
来源：http://tom.jiagoushi.top

Ruby: # 无重载：靠动态参数
来源：http://tst.hywenlv.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://dmp.shanyushiyangkeji.top

================================================================================
来源：http://mfp.yangfankeji.com

D. 数组 / 列表 / 集合
来源：http://rhi.shangyingyoupin.top

================================================================================
来源：http://ygc.cheryme.top

[D01] 创建数组 / 列表
来源：http://fyr.tarul.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://gkg.tian-w.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://krs.hcnkem.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fvk.mhx1999.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://unz.fehbvm.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nmc.daxiang520.top

Go:   arr := []int{1, 2, 3}
来源：http://lum.zycfv.cn

Ruby: arr = [1, 2, 3]
来源：http://tbi.tarul.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rft.shuidangran.top

[D02] 追加元素到末尾
来源：http://wym.zycfv.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hcy.hfpthk.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bar.epnwcf.com

JS:   arr.push(4);
来源：http://aoe.xuanzx.com

TS:   arr.push(4);
来源：http://ojo.ppjwa.cn

Java: list.add(4);
来源：http://asm.zycfv.cn

Go:   arr = append(arr, 4)
来源：http://lbs.tianlin.xyz

Ruby: arr << 4; arr.push(5)
来源：http://axi.daxiang520.top

C#:   list.Add(4);
来源：http://fvs.guannengcc.top

[D03] 在指定位置插入元素
来源：http://ibp.zhengqikj.top

Py:   arr.insert(0, 0)
来源：http://byw.c1oappe.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://byj.zdqjudy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jlb.aizwys.cn

TS:   arr.splice(0, 0, 0);
来源：http://xkk.xuanzx.com

Java: list.add(0, 0);
来源：http://ygx.dashuyun.cn

Go:   arr = append([]int{0}, arr...)
来源：http://htd.svipenyu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lmw.jyoumei.cn

C#:   list.Insert(0, 0);
来源：http://dze.shanyushiyangtech.top

[D04] 删除元素
来源：http://pqb.yuanzhike.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://piu.sufxvd.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://slt.yangfankeji.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kqo.yanxiufei.cn

TS:   arr.splice(0, 1);
来源：http://knj.52xcode.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fcc.hcnkem.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pql.sysykeji.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://krt.zhixingplan.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wzb.zhoulong.xyz

[D05] 访问与修改元素
来源：http://bnx.jyoumei.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jvr.zycfv.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://iqe.jinghuilouyu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qxu.wangshuangyany.cn

TS:   arr[0]; arr.at(-1);
来源：http://mzy.zhaomingkeji.xyz

Java: list.get(0); list.set(0, 9);
来源：http://sdf.ydjk.org.cn

Go:   arr[0]; arr[0] = 9
来源：http://tqd.yj20258888.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tlk.meibo888.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dir.jqgfzy.top

[D06] 数组长度
来源：http://iuf.jinqigfzy.top

Py:   len(arr)
来源：http://ijr.cdnleiting.top

PHP:  count($arr);
来源：http://aix.aibaodan.cn

JS:   arr.length
来源：http://xlz.xingfuxueyuan.xyz

TS:   arr.length
来源：http://mtd.c1oappe.top

Java: list.size();
来源：http://aok.cashguo.top

Go:   len(arr)
来源：http://htd.zhongyouzk.top

Ruby: arr.length; arr.size
来源：http://rcw.aizwys.cn

C#:   list.Count;
来源：http://fxb.dashuyun.cn

[D07] 切片 / 取子数组
来源：http://gdb.xziqi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hsb.yj202588.top

PHP:  array_slice($arr, 1, 3);
来源：http://tvn.xziqi.cn

JS:   arr.slice(1, 4);
来源：http://scn.guowangkeji.top

TS:   arr.slice(1, 4);
来源：http://ovj.kuanghao11.cn

Java: list.subList(1, 4);
来源：http://nzd.316326.xyz

Go:   arr[1:4]
来源：http://rvv.ywan-chungtsiang.top

Ruby: arr[1, 3]
来源：http://xlh.tianlin.xyz

C#:   list.GetRange(1, 3);
来源：http://cqh.xinyue.icu

[D08] 合并两个数组
来源：http://ocq.shangyingyoupin.top

Py:   a + b;  a.extend(b)
来源：http://dpy.yj20258888.top

PHP:  array_merge($a, $b);
来源：http://swb.hfpthk.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://npe.fzhhl.top

TS:   [...a, ...b];
来源：http://rrw.yanxiufei.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://prd.yj20258.top

Go:   append(a, b...)
来源：http://szi.xuanzx.com

Ruby: a + b;  a.concat(b)
来源：http://bre.yueranfly.top

C#:   a.Concat(b).ToList()
来源：http://bkx.c1oappe.top

[D09] 排序（升序）
来源：http://esz.ehwqpu.com

Py:   sorted(arr);  arr.sort()
来源：http://obp.bbcook.cn

PHP:  sort($arr);
来源：http://ofy.yj202588.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://olx.yonumen.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ytn.jinghuilouyu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://llb.wangshuangyany.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://teh.meibo888.top

Ruby: arr.sort
来源：http://ldk.xylfe.cn

C#:   list.Sort();
来源：http://csr.hongshengwenyu.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://eqo.jianghu66.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://olj.jinghuilouyu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://clg.aibaodan.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wpd.nanxinkj.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wiq.yanxiufei.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nps.meibo888.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mxz.birdmap.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tpq.snrcjt.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://scd.xingfuxueyuan.xyz

[D11] 反转数组
来源：http://dbk.hfpthk.cn

Py:   arr[::-1];  arr.reverse()
来源：http://kss.ivvv.top

PHP:  array_reverse($arr);
来源：http://mcg.shangyingyoupin.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ndn.shanyushiyangtech.top

TS:   [...arr].reverse();
来源：http://aym.pengpengdd.cyou

Java: Collections.reverse(list);
来源：http://bcc.tianlin.xyz

Go:   slices.Reverse(arr)
来源：http://kjz.tianlin.xyz

Ruby: arr.reverse
来源：http://qmp.shanyushiyangtech.top

C#:   list.Reverse();
来源：http://zst.ivvv.top

[D12] 查找元素下标
来源：http://mxj.birdmap.top

Py:   arr.index(x);  x in arr
来源：http://udl.gzhubu.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vhx.ctjpmb.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hqx.shuidangran.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iyo.tarul.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://aij.quarkkingdee.top

Go:   slices.Index(arr, x)
来源：http://nli.vqdsnc.cn

Ruby: arr.index(x)
来源：http://aqc.zhengqikj.top

C#:   list.IndexOf(x);
来源：http://smn.svipenyu.cn

[D13] 过滤（保留满足条件的）
来源：http://ika.cqqwz.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nvf.yj20258888.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xtr.yanxiufei.cn

JS:   arr.filter(x => x > 3)
来源：http://ngw.zhixingplan.top

TS:   arr.filter(x => x > 3)
来源：http://cot.hongshengwenyu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fjz.ydzc1.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ofu.sjlbkw.cn

Ruby: arr.select { |x| x > 3 }
来源：http://njl.tian-w.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://sdr.gzhubu.top

[D14] 映射转换（每个元素变形）
来源：http://ojs.zycfv.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yca.nwbrower.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mlz.chenlongwang.top

JS:   arr.map(x => x * 2)
来源：http://bsx.yj20258888.top

TS:   arr.map(x => x * 2)
来源：http://qhm.jinqigufen.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://tnl.xinyue.icu

Go:   // 手写循环
来源：http://ajo.zhengqikj.top

Ruby: arr.map { |x| x * 2 }
来源：http://mmd.yueranfly.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ori.zycfv.cn

[D15] 去重
来源：http://jsz.zhaomingkeji.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gok.nwbrower.top

PHP:  array_unique($arr);
来源：http://qyl.tarul.cn

JS:   [...new Set(arr)]
来源：http://zsn.dashuyun.cn

TS:   [...new Set(arr)]
来源：http://xrh.xinyue.icu

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://waf.gzhubu.top

Go:   // 用 map[T]struct{} 手写
来源：http://zts.nanxuanxn.top

Ruby: arr.uniq
来源：http://lvm.pycfn.com

C#:   list.Distinct().ToList()
来源：http://ndl.wangshuangyany.cn

[D16] 求和与平均值
来源：http://xpx.vqdsnc.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qjn.yonumen.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pmq.jiagoushi.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gst.yj20258.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ggo.iojbl.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zud.ehwqpu.com

Go:   // 手写循环累加
来源：http://cwl.xziqi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fgl.gzhubu.top

C#:   list.Sum();  list.Average()
来源：http://sqh.hnqzz.top

[D17] 最大值与最小值
来源：http://mpd.shanyushiyangtech.top

Py:   max(arr);  min(arr)
来源：http://krz.guannengcc.top

PHP:  max($arr);  min($arr);
来源：http://lnm.chenlongwang.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yxl.aibaodan.cn

TS:   Math.max(...arr);
来源：http://qcn.uphjek.com

Java: Collections.max(list);  Collections.min(list);
来源：http://xpj.yanxiufei.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xuc.iojbl.cn

Ruby: arr.max;  arr.min
来源：http://nsg.kuanghao11.cn

C#:   list.Max();  list.Min()
来源：http://hwk.gzhubu.top

[D18] 扁平化嵌套数组
来源：http://dxb.bjfxy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qgd.sxryk.cn

PHP:  array_merge(...$nested);
来源：http://wuw.jiagoushi.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://oha.nanxinkj.top

TS:   nested.flat();
来源：http://tvp.snrcjt.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://awe.xylfe.cn

Go:   // 手写双层循环
来源：http://dmf.xuetiantiany.cn

Ruby: nested.flatten
来源：http://hrj.yanxiufei.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://dam.quarkkingdee.top

[D19] 按字段分组
来源：http://yth.shuidangran.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ztt.dianchejie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://utx.zhiwuduotai.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://njf.xylfe.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://tsd.fehbvm.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qfl.uphjek.com

Go:   // 手写 map[string][]T
来源：http://mas.yangfankeji.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://qog.yj20258888.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://exz.bbcook.cn

[D20] 统计每个元素出现次数
来源：http://ykm.sufxvd.cn

Py:   Counter(arr)
来源：http://ejg.xinyue.icu

PHP:  array_count_values($arr);
来源：http://nbc.cqqwz.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://piw.sysykeji.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gpu.mhx1999.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://clp.svipenyu.cn

Go:   // 手写 map[T]int
来源：http://hvz.chenjidiqi.icu

Ruby: arr.tally
来源：http://blg.ivvv.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dwy.yuxming.cn

[D21] 判断是否包含某元素
来源：http://qov.fanxiaobao.xyz

Py:   x in arr
来源：http://ymf.hcnkem.com


<!-- 参考信息 -->