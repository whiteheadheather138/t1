代发 wailian999

[C06] 匿名函数 / lambda
来源：http://ezs.zdbjq.cn

Py:   square = lambda x: x * x
来源：http://kwh.yuxming.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://lxj.xziqi.cn

JS:   const square = x => x * x;
来源：http://tkd.shzxlz.cn

TS:   const square = (x: number): number => x * x;
来源：http://zrn.ybcxt.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vli.jiagoushi.top

Go:   sq := func(x int) int { return x * x }
来源：http://feu.wangdashe.top

Ruby: square = ->(x) { x * x }
来源：http://dzf.zhijiandao.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fly.jqgfzy.top

[C07] 把函数作为参数传入
来源：http://apt.hesvh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://usa.mhx1999.top

PHP:  array_map("strtoupper", $arr);
来源：http://hbb.havefunace.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uhh.svipenyu.cn

TS:   arr.map(String)
来源：http://pvb.birdmap.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dfp.hongshengwenyu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sby.xuetiantiany.cn

Ruby: arr.map(&:upcase)
来源：http://vwc.gogol.net.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://kez.cdnleiting.top

[C08] 闭包
来源：http://ovs.tianlin.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://slo.svipenyu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ppc.havefunace.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rfc.uphjek.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wrd.hesvh.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://egx.havefunace.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lhi.sysykeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cvh.smart0.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hxb.zhixingplan.top

[C09] 递归
来源：http://poc.ydzc1.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qcj.shangyingyoupin.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ukx.hfpthk.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mky.jinyuanbaomall.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://umm.zhixingplan.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hvw.fanxiaobao.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wsy.52xcode.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jou.tian-w.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dpu.nanxuanxn.top

[C10] 变量作用域
来源：http://iwu.cheryme.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ogw.yj20258.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cib.chenzaomai.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vva.jqgfzy.top

TS:   同 JS
来源：http://mkn.wangdashe.top

Java: 方法内为块级作用域
来源：http://srw.birdmap.top

Go:   花括号块级作用域
来源：http://qbw.havefunace.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yph.cashguo.top

C#:   块级作用域
来源：http://wes.aibaodan.cn

[C11] 模块导入与导出
来源：http://xps.cqqwz.cn

Py:   from module import func
来源：http://ygb.zdbjq.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wwf.xinyue.icu

JS:   export default function f() {};  import f from "./m.js";
来源：http://dat.bjfxy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pbw.smart0.xyz

Java: import java.util.List;
来源：http://qgl.fktsv.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ozz.chenjidiqi.icu

Ruby: require "json"; require_relative "./util"
来源：http://wuz.cdnleiting.top

C#:   using System.Text;
来源：http://yeg.gzhubu.top

[C12] 立即执行函数 IIFE
来源：http://pyv.bjfxy.top

Py:   (lambda: print("run"))()
来源：http://mlj.jinyuanbaomall.cn

PHP:  (function () { echo "run"; })();
来源：http://zhh.wangshuangyany.cn

JS:   (() => { console.log("run"); })();
来源：http://cjx.nanxinkj.top

TS:   (() => { console.log("run"); })();
来源：http://glk.sufxvd.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vlo.9152youxi.cn

Go:   func() { fmt.Println("run") }()
来源：http://tqx.nwbrower.top

Ruby: -> { puts "run" }.call
来源：http://gme.jqgfzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://kuj.gotoacloud.top

[C13] 类型声明 / 类型注解
来源：http://mvh.sufxvd.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fdq.sufxvd.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pae.jiagoushi.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yrv.chenlongwang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sbr.zhijiandao.cn

Java: int add(int a, int b) { return a + b; }
来源：http://nom.redwolf501.top

Go:   func add(a, b int) int
来源：http://hrw.cdnleiting.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zsl.hammf.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gms.ehwqpu.com

[C14] 泛型函数
来源：http://pdb.guowangkeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lej.jinghuilouyu.cn

PHP:  // 无泛型
来源：http://kfp.uphjek.com

JS:   // 无泛型
来源：http://blw.xingfuxueyuan.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://umm.hfpthk.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://iqh.tanke756.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ymj.gogol.net.cn

Ruby: # 无泛型
来源：http://xiz.havefunace.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fdz.zdqjudy.top

[C15] 解构 / 展开参数
来源：http://nzp.fengsongda.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ogd.yangfankeji.com

PHP:  [$a, $b] = $pair;
来源：http://elt.birdmap.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xdp.chenzaomai.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ell.andypj.xyz

Java: // 无解构
来源：http://rtm.fanxiaobao.xyz

Go:   // 无解构
来源：http://hrt.hysaishi.cn

Ruby: a, b = pair
来源：http://brw.sjlbkw.cn

C#:   var (a, b) = pair;
来源：http://pck.zhijiandao.cn

[C16] 函数 / 方法重载
来源：http://vii.yueranfly.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dht.nanxuanxn.top

PHP:  // 无重载
来源：http://cgo.yuxming.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bat.xingfuxueyuan.xyz

TS:   // 用联合类型或重载签名声明
来源：http://sgr.dashuyun.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mwi.9152youxi.cn

Go:   // 无重载：用不同函数名
来源：http://deb.guannengcc.top

Ruby: # 无重载：靠动态参数
来源：http://ihv.tanke756.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://upr.jinghuilouyu.cn

================================================================================
来源：http://ovf.jiagoushi.top

D. 数组 / 列表 / 集合
来源：http://sjd.yanxiufei.cn

================================================================================
来源：http://stv.xziqi.cn

[D01] 创建数组 / 列表
来源：http://yqj.ydjk.org.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://nnm.yj202588.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mcm.pengpengdd.cyou

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://seo.pycfn.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://ayc.daria6918.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lxq.jqgfzy.top

Go:   arr := []int{1, 2, 3}
来源：http://mfa.yj202588.top

Ruby: arr = [1, 2, 3]
来源：http://loo.c1oappe.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://icx.yj20258888.top

[D02] 追加元素到末尾
来源：http://lem.snrcjt.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ida.iojbl.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rog.shzxlz.cn

JS:   arr.push(4);
来源：http://lok.zhongyouzk.top

TS:   arr.push(4);
来源：http://egs.xingfuxueyuan.xyz

Java: list.add(4);
来源：http://qce.snrcjt.cn

Go:   arr = append(arr, 4)
来源：http://tdh.jianghu66.top

Ruby: arr << 4; arr.push(5)
来源：http://hqz.svipenyu.cn

C#:   list.Add(4);
来源：http://ivh.xylfe.cn

[D03] 在指定位置插入元素
来源：http://ssi.vqdsnc.cn

Py:   arr.insert(0, 0)
来源：http://nrd.dashuyun.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yhi.sufxvd.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://eto.hnxiangtu.top

TS:   arr.splice(0, 0, 0);
来源：http://icb.snrcjt.cn

Java: list.add(0, 0);
来源：http://xrr.daxiang520.top

Go:   arr = append([]int{0}, arr...)
来源：http://sty.sweek.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ucl.hesvh.cn

C#:   list.Insert(0, 0);
来源：http://byc.ctjpmb.com

[D04] 删除元素
来源：http://fmh.ydzc1.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://smu.cqqwz.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cuq.shuidangran.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nnm.snrcjt.cn

TS:   arr.splice(0, 1);
来源：http://dev.cheryme.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jan.birdmap.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ymb.sxryk.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ava.fengsongda.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ykh.jqgfzy.top

[D05] 访问与修改元素
来源：http://edv.tanke756.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qya.yongpay.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://iiw.andypj.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qhf.feifeiyinyue.top

TS:   arr[0]; arr.at(-1);
来源：http://hrz.sysykeji.top

Java: list.get(0); list.set(0, 9);
来源：http://idp.yj20258.top

Go:   arr[0]; arr[0] = 9
来源：http://akf.nanxinkj.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rgw.daria6918.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uxa.ybcxt.top

[D06] 数组长度
来源：http://ifh.sweek.top

Py:   len(arr)
来源：http://rjc.tarul.cn

PHP:  count($arr);
来源：http://pcc.zhongyouzk.top

JS:   arr.length
来源：http://rge.zhiwuduotai.top

TS:   arr.length
来源：http://vff.tarul.cn

Java: list.size();
来源：http://rqq.ctjpmb.com

Go:   len(arr)
来源：http://nzm.feifeiyinyue.top

Ruby: arr.length; arr.size
来源：http://dhx.52xcode.cn

C#:   list.Count;
来源：http://rxw.zhiwuduotai.top

[D07] 切片 / 取子数组
来源：http://rtj.wangshuangyany.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wzb.gogol.net.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gft.sjlbkw.cn

JS:   arr.slice(1, 4);
来源：http://pgv.xinyue.icu

TS:   arr.slice(1, 4);
来源：http://qcb.aizwys.cn

Java: list.subList(1, 4);
来源：http://dvf.daria6918.cn

Go:   arr[1:4]
来源：http://ozh.ybcxt.top

Ruby: arr[1, 3]
来源：http://ymf.iojbl.cn

C#:   list.GetRange(1, 3);
来源：http://rdo.0kj1m.cn

[D08] 合并两个数组
来源：http://zao.yangfankeji.com

Py:   a + b;  a.extend(b)
来源：http://hgt.sweek.top

PHP:  array_merge($a, $b);
来源：http://fsz.chenzaomai.com

JS:   [...a, ...b];  a.concat(b);
来源：http://fou.hfpthk.cn

TS:   [...a, ...b];
来源：http://ium.jlsjyb.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bsb.xingfuxueyuan.xyz

Go:   append(a, b...)
来源：http://fce.uphjek.com

Ruby: a + b;  a.concat(b)
来源：http://ntl.cashguo.top

C#:   a.Concat(b).ToList()
来源：http://ojo.smart0.xyz

[D09] 排序（升序）
来源：http://jzp.gaohongyu789.top

Py:   sorted(arr);  arr.sort()
来源：http://xwg.zhixingplan.top

PHP:  sort($arr);
来源：http://mle.fengsongda.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://utz.hysaishi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://poe.jinqigfzy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://lav.ydzc1.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://aei.jiagoushi.top

Ruby: arr.sort
来源：http://ubq.hongshengwenyu.top

C#:   list.Sort();
来源：http://sqv.yj20258888.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://iew.ybcxt.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ujv.hfpthk.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zad.jinyuanbaomall.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://psl.aibaodan.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hxx.xuanzx.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gax.chenzaomai.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wgu.yongpay.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vtn.zdbjq.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xwv.sjlbkw.cn

[D11] 反转数组
来源：http://zil.bjfxy.top

Py:   arr[::-1];  arr.reverse()
来源：http://gzf.cashguo.top

PHP:  array_reverse($arr);
来源：http://mon.zycfv.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ois.xingfuxueyuan.xyz

TS:   [...arr].reverse();
来源：http://hyn.fehbvm.com

Java: Collections.reverse(list);
来源：http://oof.jinqigufen.top

Go:   slices.Reverse(arr)
来源：http://rme.52xcode.cn

Ruby: arr.reverse
来源：http://wzb.daxiang520.top

C#:   list.Reverse();
来源：http://vud.jyoumei.cn

[D12] 查找元素下标
来源：http://bfe.sjlbkw.cn

Py:   arr.index(x);  x in arr
来源：http://jyj.yj20258888.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://amq.uphjek.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dly.havefunace.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cia.xingfuxueyuan.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xee.yangfankeji.com

Go:   slices.Index(arr, x)
来源：http://kan.daria6918.cn

Ruby: arr.index(x)
来源：http://quh.iojbl.cn

C#:   list.IndexOf(x);
来源：http://grr.hcnkem.com

[D13] 过滤（保留满足条件的）
来源：http://wqc.ivvv.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hyq.guannengcc.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bli.shanyushiyangtech.top

JS:   arr.filter(x => x > 3)
来源：http://zag.jinqigfzy.top

TS:   arr.filter(x => x > 3)
来源：http://oll.svipenyu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ton.bbcook.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zsq.sysykeji.top

Ruby: arr.select { |x| x > 3 }
来源：http://pzg.ivvv.top

C#:   list.Where(x => x > 3).ToList()
来源：http://nxq.xziqi.cn

[D14] 映射转换（每个元素变形）
来源：http://kiq.quarkkingdee.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gbd.aibaodan.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bef.tarul.cn

JS:   arr.map(x => x * 2)
来源：http://lyq.jianghu66.top

TS:   arr.map(x => x * 2)
来源：http://hyy.yueranfly.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://fdf.yueranfly.top

Go:   // 手写循环
来源：http://clb.dashuyun.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wwj.cheryme.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ige.fehbvm.com

[D15] 去重
来源：http://wth.chenzaomai.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://iiy.nanxinkj.top

PHP:  array_unique($arr);
来源：http://zpu.aizwys.cn

JS:   [...new Set(arr)]
来源：http://dcm.jlsjyb.cn

TS:   [...new Set(arr)]
来源：http://ycl.xuanzx.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zdd.birdmap.top

Go:   // 用 map[T]struct{} 手写
来源：http://aie.nanxinkj.top

Ruby: arr.uniq
来源：http://cpw.zhengqikj.top

C#:   list.Distinct().ToList()
来源：http://vyt.zdqjudy.top

[D16] 求和与平均值
来源：http://izi.sweek.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zyr.wangdashe.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ieg.shuidangran.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zss.snrcjt.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wai.yj20258.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nlv.0kj1m.cn

Go:   // 手写循环累加
来源：http://hin.yj202588.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jjp.andypj.xyz

C#:   list.Sum();  list.Average()
来源：http://cbm.sjlbkw.cn

[D17] 最大值与最小值
来源：http://vne.ybcxt.top

Py:   max(arr);  min(arr)
来源：http://sqf.pycfn.com

PHP:  max($arr);  min($arr);
来源：http://twn.9152youxi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xli.aibaodan.cn

TS:   Math.max(...arr);
来源：http://wly.gzhubu.top

Java: Collections.max(list);  Collections.min(list);
来源：http://riw.sweek.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yev.guannengcc.top

Ruby: arr.max;  arr.min
来源：http://ivt.hywenlv.cn

C#:   list.Max();  list.Min()
来源：http://rqw.jinghuilouyu.cn

[D18] 扁平化嵌套数组
来源：http://zyd.zhaomingkeji.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ncp.dashuyun.cn

PHP:  array_merge(...$nested);
来源：http://faw.vehdjk.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bdp.cdnleiting.top

TS:   nested.flat();
来源：http://izb.xuetiantiany.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gfe.tanke756.top

Go:   // 手写双层循环
来源：http://tzi.cdnleiting.top

Ruby: nested.flatten
来源：http://gko.sjlbkw.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://jzs.tarul.cn

[D19] 按字段分组
来源：http://miw.ydjk.org.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://txb.shanyushiyangtech.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lqe.yuxming.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ywg.gzhubu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ftr.guannengcc.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://boz.quarkkingdee.top

Go:   // 手写 map[string][]T
来源：http://kty.fzhhl.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://xmm.chenlongwang.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://quh.svipenyu.cn

[D20] 统计每个元素出现次数
来源：http://bze.yanxiufei.cn

Py:   Counter(arr)
来源：http://sgg.ybcxt.top

PHP:  array_count_values($arr);
来源：http://cwd.jqgfzy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rdl.bjfxy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yus.xingfuxueyuan.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hnk.hysaishi.cn

Go:   // 手写 map[T]int
来源：http://sly.vqdsnc.cn

Ruby: arr.tally
来源：http://ntw.hcnkem.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kqf.gogol.net.cn

[D21] 判断是否包含某元素
来源：http://ljm.jyoumei.cn

Py:   x in arr
来源：http://enk.fanxiaobao.xyz

PHP:  in_array($x, $arr, true);
来源：http://bgn.feifeiyinyue.top

JS:   arr.includes(x)
来源：http://jly.yj20258888.top

TS:   arr.includes(x)
来源：http://xud.hcnkem.com

Java: list.contains(x)
来源：http://sey.cdnleiting.top

Go:   slices.Contains(arr, x)
来源：http://lbt.gzhubu.top

Ruby: arr.include?(x)
来源：http://eep.0kj1m.cn

C#:   list.Contains(x)
来源：http://ima.xingfuxueyuan.xyz

[D22] 复制数组（避免共享引用）
来源：http://foi.ybcxt.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lod.feifeiyinyue.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mwx.hammf.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bne.yanxiufei.cn

TS:   [...arr];
来源：http://duc.vqdsnc.cn

Java: new ArrayList<>(list);
来源：http://pni.chenlongwang.top

Go:   copied := append([]int(nil), arr...)
来源：http://fdb.hongshengwenyu.top

Ruby: arr.dup;  arr.clone
来源：http://lcr.sweek.top

C#:   new List<int>(list);
来源：http://glz.ehwqpu.com


<!-- 参考信息 -->