代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://gar.shzxlz.cn

Ruby: f(a: 1, b: 2)
来源：http://jtv.epnwcf.com

C#:   f(a: 1, b: 2)
来源：http://aid.zhengqikj.top

[C05] 返回多个值
来源：http://zcc.tian-w.cn

Py:   return a, b
来源：http://tyr.jianghu66.top

PHP:  return [$a, $b];
来源：http://cdp.cqqwz.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://lyj.xziqi.cn

TS:   return { a, b };
来源：http://vxy.uphjek.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nbo.svipenyu.cn

Go:   return a, b
来源：http://ovt.ivvv.top

Ruby: return a, b
来源：http://hwl.chenzaomai.com

C#:   return (a, b);              // ValueTuple
来源：http://sde.ivvv.top

[C06] 匿名函数 / lambda
来源：http://abz.sufxvd.cn

Py:   square = lambda x: x * x
来源：http://eyb.nanxinkj.top

PHP:  $square = fn($x) => $x * $x;
来源：http://bbv.c1oappe.top

JS:   const square = x => x * x;
来源：http://cbf.yuxming.cn

TS:   const square = (x: number): number => x * x;
来源：http://ngw.zhaomingkeji.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xcz.xuanzx.com

Go:   sq := func(x int) int { return x * x }
来源：http://nyd.guannengcc.top

Ruby: square = ->(x) { x * x }
来源：http://zvj.fehbvm.com

C#:   Func<int, int> square = x => x * x;
来源：http://nyy.jqgfzy.top

[C07] 把函数作为参数传入
来源：http://yne.yanxiufei.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://uqt.uphjek.com

PHP:  array_map("strtoupper", $arr);
来源：http://ykb.chenjidiqi.icu

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pyp.yj20258.top

TS:   arr.map(String)
来源：http://ctm.jinyuanbaomall.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hqh.daxiang520.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mfr.cucudq.cn

Ruby: arr.map(&:upcase)
来源：http://hry.chenjidiqi.icu

C#:   arr.Select(s => s.ToUpper())
来源：http://pwl.chenlongwang.top

[C08] 闭包
来源：http://ejp.zhiwuduotai.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mel.xylfe.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gqm.ctjpmb.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gia.gotoacloud.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tfq.havefunace.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://oxj.cucudq.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lfb.wangdashe.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://goh.xziqi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://aqx.jinghuilouyu.cn

[C09] 递归
来源：http://enx.redwolf501.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://anp.zhongyouzk.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bdq.jianghu66.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gln.aibaodan.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iiq.dianchejie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yiy.fehbvm.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fjw.zhengqikj.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fca.hcnkem.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vwn.dianchejie.cn

[C10] 变量作用域
来源：http://rvr.yj202588.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fyn.ctjpmb.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ruj.shanyushiyangtech.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wda.smart0.xyz

TS:   同 JS
来源：http://wss.gotoacloud.top

Java: 方法内为块级作用域
来源：http://jig.ywan-chungtsiang.top

Go:   花括号块级作用域
来源：http://axf.andypj.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mvs.quarkkingdee.top

C#:   块级作用域
来源：http://neo.jiagoushi.top

[C11] 模块导入与导出
来源：http://dgh.guowangkeji.top

Py:   from module import func
来源：http://efk.tarul.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://eto.gogol.net.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kng.cashguo.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ngz.fzhhl.top

Java: import java.util.List;
来源：http://pwb.wangdashe.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vox.meibo888.top

Ruby: require "json"; require_relative "./util"
来源：http://lxl.mhx1999.top

C#:   using System.Text;
来源：http://utn.zhengqikj.top

[C12] 立即执行函数 IIFE
来源：http://clz.hnqzz.top

Py:   (lambda: print("run"))()
来源：http://uod.daria6918.cn

PHP:  (function () { echo "run"; })();
来源：http://pbv.yonumen.top

JS:   (() => { console.log("run"); })();
来源：http://fmz.kuanghao11.cn

TS:   (() => { console.log("run"); })();
来源：http://gbc.feifeiyinyue.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qcw.zdqjudy.top

Go:   func() { fmt.Println("run") }()
来源：http://rvf.zhaomingkeji.xyz

Ruby: -> { puts "run" }.call
来源：http://ocs.hfpthk.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://vnv.zhoulong.xyz

[C13] 类型声明 / 类型注解
来源：http://xim.hfpthk.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yrw.jinghuilouyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gzd.shuidangran.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vev.chenlongwang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zoa.zhongyouzk.top

Java: int add(int a, int b) { return a + b; }
来源：http://kwy.havefunace.top

Go:   func add(a, b int) int
来源：http://oap.gotoacloud.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lkk.yangfankeji.com

C#:   int Add(int a, int b) => a + b;
来源：http://mcw.ivvv.top

[C14] 泛型函数
来源：http://new.vqdsnc.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zha.aizwys.cn

PHP:  // 无泛型
来源：http://kkp.zhongyouzk.top

JS:   // 无泛型
来源：http://vjl.yj202588.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ocg.pengpengdd.cyou

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://odj.tianlin.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mum.yj20258888.top

Ruby: # 无泛型
来源：http://yvz.redwolf501.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hur.hnqzz.top

[C15] 解构 / 展开参数
来源：http://aku.ppjwa.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wnm.hfpthk.cn

PHP:  [$a, $b] = $pair;
来源：http://mqi.ehwqpu.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rnu.ywan-chungtsiang.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://luo.cashguo.top

Java: // 无解构
来源：http://hww.xuetiantiany.cn

Go:   // 无解构
来源：http://ghr.yuanzhike.top

Ruby: a, b = pair
来源：http://jmg.cucudq.cn

C#:   var (a, b) = pair;
来源：http://gxu.wangdashe.top

[C16] 函数 / 方法重载
来源：http://wpv.jiagoushi.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kwr.jyoumei.cn

PHP:  // 无重载
来源：http://bdp.andypj.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://azw.yj20258888.top

TS:   // 用联合类型或重载签名声明
来源：http://jiw.fzhhl.top

Java: void f(int a) {}  void f(String a) {}
来源：http://hio.hcnkem.com

Go:   // 无重载：用不同函数名
来源：http://egr.epnwcf.com

Ruby: # 无重载：靠动态参数
来源：http://ffp.yvedp.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ktp.jqgufenzy.top

================================================================================
来源：http://dqd.dianchejie.cn

D. 数组 / 列表 / 集合
来源：http://byw.yanxiufei.cn

================================================================================
来源：http://lgk.yvedp.cn

[D01] 创建数组 / 列表
来源：http://qdw.haohaochexian.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://rha.mhx1999.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ekf.c1oappe.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sbm.tianlin.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://mvs.guannengcc.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ydl.fanxiaobao.xyz

Go:   arr := []int{1, 2, 3}
来源：http://akc.ywan-chungtsiang.top

Ruby: arr = [1, 2, 3]
来源：http://rle.cdnleiting.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hlq.yueranfly.top

[D02] 追加元素到末尾
来源：http://rtb.zdbjq.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bdd.hcnkem.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qun.yvedp.cn

JS:   arr.push(4);
来源：http://fpo.meibo888.top

TS:   arr.push(4);
来源：http://cwu.feifeiyinyue.top

Java: list.add(4);
来源：http://pzi.fktsv.cn

Go:   arr = append(arr, 4)
来源：http://xjl.cdnleiting.top

Ruby: arr << 4; arr.push(5)
来源：http://ueb.yanxiufei.cn

C#:   list.Add(4);
来源：http://owl.zhongyouzk.top

[D03] 在指定位置插入元素
来源：http://pqn.guowangkeji.top

Py:   arr.insert(0, 0)
来源：http://tfp.xuetiantiany.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pwz.cqqwz.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sgk.havefunace.top

TS:   arr.splice(0, 0, 0);
来源：http://lbi.zhoulong.xyz

Java: list.add(0, 0);
来源：http://svi.hesvh.cn

Go:   arr = append([]int{0}, arr...)
来源：http://dxy.xinyue.icu

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tza.zycfv.cn

C#:   list.Insert(0, 0);
来源：http://sxr.meibo888.top

[D04] 删除元素
来源：http://tfs.sxryk.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://raf.sxryk.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ukh.guowangkeji.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mft.kuanghao11.cn

TS:   arr.splice(0, 1);
来源：http://xiq.fanxiaobao.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fiy.gotoacloud.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pdr.jinyuanbaomall.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jsf.fktsv.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lpy.hcnkem.com

[D05] 访问与修改元素
来源：http://kni.sxryk.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tvd.feifeiyinyue.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gbg.bjfxy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://smc.bjfxy.top

TS:   arr[0]; arr.at(-1);
来源：http://jnp.sufxvd.cn

Java: list.get(0); list.set(0, 9);
来源：http://xfy.wangshuangyany.cn

Go:   arr[0]; arr[0] = 9
来源：http://nnx.shanyushiyangkeji.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zzr.xuanzx.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cup.zdqjudy.top

[D06] 数组长度
来源：http://glq.ehwqpu.com

Py:   len(arr)
来源：http://yiq.cdnleiting.top

PHP:  count($arr);
来源：http://elh.daxiang520.top

JS:   arr.length
来源：http://tto.dashuyun.cn

TS:   arr.length
来源：http://ugn.yfazqb.com

Java: list.size();
来源：http://cml.uphjek.com

Go:   len(arr)
来源：http://wns.cashguo.top

Ruby: arr.length; arr.size
来源：http://bxt.sxryk.cn

C#:   list.Count;
来源：http://sja.hesvh.cn

[D07] 切片 / 取子数组
来源：http://yet.smart0.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bkc.sjlbkw.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zfj.jyoumei.cn

JS:   arr.slice(1, 4);
来源：http://buv.jqgufenzy.top

TS:   arr.slice(1, 4);
来源：http://pix.feifeiyinyue.top

Java: list.subList(1, 4);
来源：http://vfp.fktsv.cn

Go:   arr[1:4]
来源：http://ihb.jqgfzy.top

Ruby: arr[1, 3]
来源：http://xha.xuanzx.com

C#:   list.GetRange(1, 3);
来源：http://jpi.jianghu66.top

[D08] 合并两个数组
来源：http://vae.zdbjq.cn

Py:   a + b;  a.extend(b)
来源：http://wcn.sufxvd.cn

PHP:  array_merge($a, $b);
来源：http://rda.hnqzz.top

JS:   [...a, ...b];  a.concat(b);
来源：http://gwp.xingfuxueyuan.xyz

TS:   [...a, ...b];
来源：http://mfa.fktsv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xoe.0kj1m.cn

Go:   append(a, b...)
来源：http://ogp.gogol.net.cn

Ruby: a + b;  a.concat(b)
来源：http://tuw.yfazqb.com

C#:   a.Concat(b).ToList()
来源：http://rwn.shuidangran.top

[D09] 排序（升序）
来源：http://spa.xziqi.cn

Py:   sorted(arr);  arr.sort()
来源：http://gij.wangshuangyany.cn

PHP:  sort($arr);
来源：http://qkk.yanxiufei.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rdi.bbcook.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://obw.yfazqb.com

Java: Collections.sort(list);  list.sort(null);
来源：http://gxz.shzxlz.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uun.zhaomingkeji.xyz

Ruby: arr.sort
来源：http://vto.aizwys.cn

C#:   list.Sort();
来源：http://aii.316326.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://cyw.fanxiaobao.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ont.zhongyouzk.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://crn.wangshuangyany.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jpo.zhongyouzk.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://het.zhiwuduotai.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ayy.xziqi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kbx.nanxinkj.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://isq.zdqjudy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zoh.xuanzx.com

[D11] 反转数组
来源：http://zog.vqdsnc.cn

Py:   arr[::-1];  arr.reverse()
来源：http://nll.gogol.net.cn

PHP:  array_reverse($arr);
来源：http://nzt.jinyuanbaomall.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dtn.52xcode.cn

TS:   [...arr].reverse();
来源：http://zkn.hammf.cn

Java: Collections.reverse(list);
来源：http://asz.yuxming.cn

Go:   slices.Reverse(arr)
来源：http://fjr.yfazqb.com

Ruby: arr.reverse
来源：http://ffw.nwbrower.top

C#:   list.Reverse();
来源：http://xwi.316326.xyz

[D12] 查找元素下标
来源：http://igr.ivvv.top

Py:   arr.index(x);  x in arr
来源：http://vsr.sweek.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vcq.kuanghao11.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xux.xuetiantiany.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gzq.jinghuilouyu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zvr.dashuyun.cn

Go:   slices.Index(arr, x)
来源：http://llw.fanxiaobao.xyz

Ruby: arr.index(x)
来源：http://bkn.sweek.top

C#:   list.IndexOf(x);
来源：http://unt.yfazqb.com

[D13] 过滤（保留满足条件的）
来源：http://vug.dianchejie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xos.snrcjt.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://koz.shzxlz.cn

JS:   arr.filter(x => x > 3)
来源：http://koz.jqgufenzy.top

TS:   arr.filter(x => x > 3)
来源：http://btr.cdnleiting.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tgk.chenjidiqi.icu

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jzr.vqdsnc.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ejc.jlsjyb.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ytw.hcnkem.com

[D14] 映射转换（每个元素变形）
来源：http://ydq.gotoacloud.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://thy.xylfe.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bqh.jiagoushi.top

JS:   arr.map(x => x * 2)
来源：http://utl.tarul.cn

TS:   arr.map(x => x * 2)
来源：http://hux.aizwys.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://pfj.zycfv.cn

Go:   // 手写循环
来源：http://vhs.fanxiaobao.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://efh.aibaodan.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bud.yonumen.top

[D15] 去重
来源：http://trj.dashuyun.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vci.tian-w.cn

PHP:  array_unique($arr);
来源：http://cpc.c1oappe.top

JS:   [...new Set(arr)]
来源：http://pyk.gzhubu.top

TS:   [...new Set(arr)]
来源：http://jef.gaohongyu789.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bil.jlsjyb.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ikm.hcnkem.com

Ruby: arr.uniq
来源：http://czj.shanyushiyangkeji.top

C#:   list.Distinct().ToList()
来源：http://ngu.ybcxt.top

[D16] 求和与平均值
来源：http://svj.dashuyun.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uzv.ydzc1.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wpw.jinyuanbaomall.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lqg.mhx1999.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kgh.hnxiangtu.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zws.xinyue.icu

Go:   // 手写循环累加
来源：http://cfh.jianghu66.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ekb.yj20258888.top

C#:   list.Sum();  list.Average()
来源：http://cmk.uphjek.com

[D17] 最大值与最小值
来源：http://yir.fzhhl.top

Py:   max(arr);  min(arr)
来源：http://bnn.guowangkeji.top

PHP:  max($arr);  min($arr);
来源：http://bfl.ybcxt.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://szm.sufxvd.cn

TS:   Math.max(...arr);
来源：http://yaf.jqgfzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://tim.quarkkingdee.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jgz.yueranfly.top

Ruby: arr.max;  arr.min
来源：http://ewk.yvedp.cn

C#:   list.Max();  list.Min()
来源：http://cpb.fktsv.cn

[D18] 扁平化嵌套数组
来源：http://kkv.kuanghao11.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rii.birdmap.top

PHP:  array_merge(...$nested);
来源：http://sya.yj20258888.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ujh.wangshuangyany.cn

TS:   nested.flat();
来源：http://qbe.birdmap.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xlj.wangshuangyany.cn

Go:   // 手写双层循环
来源：http://rby.redwolf501.top

Ruby: nested.flatten
来源：http://lcj.kuanghao11.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://diy.pengpengdd.cyou

[D19] 按字段分组
来源：http://par.zhengqikj.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dxg.ctjpmb.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://aiv.nanxuanxn.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kat.zhaomingkeji.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://eyi.yj202588.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nax.sysykeji.top

Go:   // 手写 map[string][]T
来源：http://nhh.yueranfly.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ufu.hcnkem.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uaz.xingfuxueyuan.xyz

[D20] 统计每个元素出现次数
来源：http://umo.vqdsnc.cn

Py:   Counter(arr)
来源：http://zhq.epnwcf.com

PHP:  array_count_values($arr);
来源：http://vai.gzhubu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jdh.ivvv.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ekj.hongshengwenyu.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://arc.yangfankeji.com

Go:   // 手写 map[T]int
来源：http://hwd.cucudq.cn

Ruby: arr.tally
来源：http://qdi.havefunace.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://slx.nwbrower.top

[D21] 判断是否包含某元素
来源：http://nts.cucudq.cn

Py:   x in arr
来源：http://wvc.0kj1m.cn

PHP:  in_array($x, $arr, true);
来源：http://vbx.dashuyun.cn

JS:   arr.includes(x)
来源：http://abr.jinyuanbaomall.cn

TS:   arr.includes(x)
来源：http://mou.fanxiaobao.xyz

Java: list.contains(x)
来源：http://tle.guowangkeji.top


<!-- 参考信息 -->