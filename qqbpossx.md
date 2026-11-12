代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://zzs.hnxiangtu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vog.ppjwa.cn

[C04] 命名参数 / 关键字参数
来源：http://cbw.gzhubu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jpv.hywenlv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lwk.xuetiantiany.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vjr.yueranfly.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jwa.0kj1m.cn

Java: // 无：用 Builder 模式或 record
来源：http://chx.sjlbkw.cn

Go:   // 无：用配置结构体参数
来源：http://hpy.hnxiangtu.top

Ruby: f(a: 1, b: 2)
来源：http://zwy.hfpthk.cn

C#:   f(a: 1, b: 2)
来源：http://sla.shangyingyoupin.top

[C05] 返回多个值
来源：http://ors.chenzaomai.com

Py:   return a, b
来源：http://qea.ppjwa.cn

PHP:  return [$a, $b];
来源：http://bmp.yueranfly.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://eif.birdmap.top

TS:   return { a, b };
来源：http://mqv.fengsongda.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ubz.cdnleiting.top

Go:   return a, b
来源：http://sog.ivvv.top

Ruby: return a, b
来源：http://bff.nanxuanxn.top

C#:   return (a, b);              // ValueTuple
来源：http://tve.ydjk.org.cn

[C06] 匿名函数 / lambda
来源：http://uak.yj20258.top

Py:   square = lambda x: x * x
来源：http://cwl.xingfuxueyuan.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://qrq.52xcode.cn

JS:   const square = x => x * x;
来源：http://sdf.wangdashe.top

TS:   const square = (x: number): number => x * x;
来源：http://ttq.nwbrower.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ttj.gotoacloud.top

Go:   sq := func(x int) int { return x * x }
来源：http://rrn.hongshengwenyu.top

Ruby: square = ->(x) { x * x }
来源：http://vnj.yuxming.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qta.aibaodan.cn

[C07] 把函数作为参数传入
来源：http://vfd.dashuyun.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://iey.fehbvm.com

PHP:  array_map("strtoupper", $arr);
来源：http://zjb.yueranfly.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ryd.mhx1999.top

TS:   arr.map(String)
来源：http://qpj.nanxinkj.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lrg.9152youxi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tad.yuanzhike.top

Ruby: arr.map(&:upcase)
来源：http://mvf.hesvh.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hpi.sjlbkw.cn

[C08] 闭包
来源：http://vyp.yuxming.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wqm.jianghu66.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://olb.sufxvd.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wvo.yuxming.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qaw.fktsv.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bqn.52xcode.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gdi.gaohongyu789.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://smp.jyoumei.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jfk.nwbrower.top

[C09] 递归
来源：http://vtt.haohaochexian.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mom.zycfv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mxb.cheryme.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kfg.svipenyu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://poi.jqgufenzy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://inb.tarul.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qcp.yonumen.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nqc.aizwys.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://slj.0kj1m.cn

[C10] 变量作用域
来源：http://niw.xingfuxueyuan.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xbx.shanyushiyangkeji.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mfn.cdnleiting.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://syj.chenjidiqi.icu

TS:   同 JS
来源：http://idu.sxryk.cn

Java: 方法内为块级作用域
来源：http://fzx.yangfankeji.com

Go:   花括号块级作用域
来源：http://naj.fanxiaobao.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ona.ppjwa.cn

C#:   块级作用域
来源：http://ehq.redwolf501.top

[C11] 模块导入与导出
来源：http://okd.yuxming.cn

Py:   from module import func
来源：http://vhi.ybcxt.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ewt.chenlongwang.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://tba.jinghuilouyu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fxm.smart0.xyz

Java: import java.util.List;
来源：http://uig.bjfxy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lqa.gzhubu.top

Ruby: require "json"; require_relative "./util"
来源：http://yvp.shuidangran.top

C#:   using System.Text;
来源：http://rca.0kj1m.cn

[C12] 立即执行函数 IIFE
来源：http://dyb.hammf.cn

Py:   (lambda: print("run"))()
来源：http://hhf.cashguo.top

PHP:  (function () { echo "run"; })();
来源：http://tvd.xinyue.icu

JS:   (() => { console.log("run"); })();
来源：http://ujc.shzxlz.cn

TS:   (() => { console.log("run"); })();
来源：http://dau.zhongyouzk.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qxd.pycfn.com

Go:   func() { fmt.Println("run") }()
来源：http://qon.ywan-chungtsiang.top

Ruby: -> { puts "run" }.call
来源：http://gic.gotoacloud.top

C#:   // 无 IIFE：用静态构造函数
来源：http://vbx.zhengqikj.top

[C13] 类型声明 / 类型注解
来源：http://oox.fanxiaobao.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://myr.ydzc1.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kij.zycfv.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://won.pengpengdd.cyou

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bsl.daria6918.cn

Java: int add(int a, int b) { return a + b; }
来源：http://zwo.bjfxy.top

Go:   func add(a, b int) int
来源：http://fhv.nanxinkj.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hvk.yangfankeji.com

C#:   int Add(int a, int b) => a + b;
来源：http://wwg.9152youxi.cn

[C14] 泛型函数
来源：http://knm.sufxvd.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qkn.snrcjt.cn

PHP:  // 无泛型
来源：http://ktz.meibo888.top

JS:   // 无泛型
来源：http://rqx.yj20258.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://aap.dianchejie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xfx.wangdashe.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bqe.cashguo.top

Ruby: # 无泛型
来源：http://nzc.ctjpmb.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hfn.uphjek.com

[C15] 解构 / 展开参数
来源：http://nwi.wangshuangyany.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gra.nanxuanxn.top

PHP:  [$a, $b] = $pair;
来源：http://dws.pengpengdd.cyou

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ixy.hongshengwenyu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vly.zhongyouzk.top

Java: // 无解构
来源：http://kea.ybcxt.top

Go:   // 无解构
来源：http://wba.vehdjk.com

Ruby: a, b = pair
来源：http://dna.zdbjq.cn

C#:   var (a, b) = pair;
来源：http://noz.zhoulong.xyz

[C16] 函数 / 方法重载
来源：http://roy.fehbvm.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rbw.vqdsnc.cn

PHP:  // 无重载
来源：http://hui.shanyushiyangkeji.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://enn.sufxvd.cn

TS:   // 用联合类型或重载签名声明
来源：http://ykx.ydjk.org.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wbs.svipenyu.cn

Go:   // 无重载：用不同函数名
来源：http://xky.svipenyu.cn

Ruby: # 无重载：靠动态参数
来源：http://pup.tian-w.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xfp.yanxiufei.cn

================================================================================
来源：http://hvk.mhx1999.top

D. 数组 / 列表 / 集合
来源：http://swy.tanke756.top

================================================================================
来源：http://psz.xuetiantiany.cn

[D01] 创建数组 / 列表
来源：http://wum.52xcode.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://gro.yj20258.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://oxq.dashuyun.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yxh.jlsjyb.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zwm.hywenlv.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pec.yvedp.cn

Go:   arr := []int{1, 2, 3}
来源：http://jbd.chenzaomai.com

Ruby: arr = [1, 2, 3]
来源：http://orc.snrcjt.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pun.316326.xyz

[D02] 追加元素到末尾
来源：http://giw.yuanzhike.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tpv.jiagoushi.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yal.zdqjudy.top

JS:   arr.push(4);
来源：http://omh.nanxuanxn.top

TS:   arr.push(4);
来源：http://cjt.fktsv.cn

Java: list.add(4);
来源：http://gex.jinqigufen.top

Go:   arr = append(arr, 4)
来源：http://jfi.xinyue.icu

Ruby: arr << 4; arr.push(5)
来源：http://tzx.hfpthk.cn

C#:   list.Add(4);
来源：http://lhb.shangyingyoupin.top

[D03] 在指定位置插入元素
来源：http://gmr.9152youxi.cn

Py:   arr.insert(0, 0)
来源：http://qkz.aizwys.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mor.xuanzx.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fck.aibaodan.cn

TS:   arr.splice(0, 0, 0);
来源：http://rdt.52xcode.cn

Java: list.add(0, 0);
来源：http://xkm.52xcode.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xxp.jiagoushi.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ylx.jiagoushi.top

C#:   list.Insert(0, 0);
来源：http://qqr.hnqzz.top

[D04] 删除元素
来源：http://tph.quarkkingdee.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://swx.guannengcc.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qdw.xziqi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lqo.yuanzhike.top

TS:   arr.splice(0, 1);
来源：http://xsy.zhijiandao.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sna.fzhhl.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bug.zhoulong.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yfp.hesvh.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xsl.yvedp.cn

[D05] 访问与修改元素
来源：http://mpc.cashguo.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rcf.gaohongyu789.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mvt.hysaishi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fxu.hysaishi.cn

TS:   arr[0]; arr.at(-1);
来源：http://iuj.gzhubu.top

Java: list.get(0); list.set(0, 9);
来源：http://ggx.zdqjudy.top

Go:   arr[0]; arr[0] = 9
来源：http://drx.yuxming.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rwm.xuetiantiany.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://doy.zhiwuduotai.top

[D06] 数组长度
来源：http://vbo.havefunace.top

Py:   len(arr)
来源：http://yul.svipenyu.cn

PHP:  count($arr);
来源：http://auf.snrcjt.cn

JS:   arr.length
来源：http://dwl.dashuyun.cn

TS:   arr.length
来源：http://ivf.daria6918.cn

Java: list.size();
来源：http://kxf.cdnleiting.top

Go:   len(arr)
来源：http://kkb.xylfe.cn

Ruby: arr.length; arr.size
来源：http://kiw.zdqjudy.top

C#:   list.Count;
来源：http://reo.pengpengdd.cyou

[D07] 切片 / 取子数组
来源：http://bxu.sufxvd.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jpb.jinqigufen.top

PHP:  array_slice($arr, 1, 3);
来源：http://uqn.yuxming.cn

JS:   arr.slice(1, 4);
来源：http://waq.hfpthk.cn

TS:   arr.slice(1, 4);
来源：http://idx.xuetiantiany.cn

Java: list.subList(1, 4);
来源：http://ibc.svipenyu.cn

Go:   arr[1:4]
来源：http://xjd.chenjidiqi.icu

Ruby: arr[1, 3]
来源：http://kez.shzxlz.cn

C#:   list.GetRange(1, 3);
来源：http://awc.yfazqb.com

[D08] 合并两个数组
来源：http://zfh.ppjwa.cn

Py:   a + b;  a.extend(b)
来源：http://ffo.smart0.xyz

PHP:  array_merge($a, $b);
来源：http://les.chenlongwang.top

JS:   [...a, ...b];  a.concat(b);
来源：http://xui.snrcjt.cn

TS:   [...a, ...b];
来源：http://ncx.yongpay.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lgo.zhongyouzk.top

Go:   append(a, b...)
来源：http://ekt.zycfv.cn

Ruby: a + b;  a.concat(b)
来源：http://zui.gzhubu.top

C#:   a.Concat(b).ToList()
来源：http://szb.jianghu66.top

[D09] 排序（升序）
来源：http://sqf.c1oappe.top

Py:   sorted(arr);  arr.sort()
来源：http://pqd.cucudq.cn

PHP:  sort($arr);
来源：http://fqz.nanxinkj.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bps.fktsv.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://nwk.hysaishi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://dva.gogol.net.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zmc.zdqjudy.top

Ruby: arr.sort
来源：http://bfs.vehdjk.com

C#:   list.Sort();
来源：http://off.shuidangran.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://nqz.shanyushiyangtech.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ayc.yvedp.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lng.ybcxt.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mbc.pengpengdd.cyou

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://roc.hysaishi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://onq.xuetiantiany.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zgm.xingfuxueyuan.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pow.gotoacloud.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rwv.fengsongda.top

[D11] 反转数组
来源：http://vvn.fanxiaobao.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://hrj.cqqwz.cn

PHP:  array_reverse($arr);
来源：http://nmr.chenjidiqi.icu

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ecq.yj20258.top

TS:   [...arr].reverse();
来源：http://jau.andypj.xyz

Java: Collections.reverse(list);
来源：http://fym.andypj.xyz

Go:   slices.Reverse(arr)
来源：http://zer.meibo888.top

Ruby: arr.reverse
来源：http://mpk.yvedp.cn

C#:   list.Reverse();
来源：http://vwk.hammf.cn

[D12] 查找元素下标
来源：http://pjb.pengpengdd.cyou

Py:   arr.index(x);  x in arr
来源：http://mkn.zhijiandao.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://opc.hammf.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wrg.wangshuangyany.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aqm.9152youxi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tfn.yfazqb.com

Go:   slices.Index(arr, x)
来源：http://ghi.jlsjyb.cn

Ruby: arr.index(x)
来源：http://xir.nanxuanxn.top

C#:   list.IndexOf(x);
来源：http://scc.yonumen.top

[D13] 过滤（保留满足条件的）
来源：http://ppd.bbcook.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nui.zhoulong.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wba.hongshengwenyu.top

JS:   arr.filter(x => x > 3)
来源：http://miv.epnwcf.com

TS:   arr.filter(x => x > 3)
来源：http://hoc.ppjwa.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hdq.yvedp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gbl.birdmap.top

Ruby: arr.select { |x| x > 3 }
来源：http://erz.nwbrower.top

C#:   list.Where(x => x > 3).ToList()
来源：http://knq.jiagoushi.top

[D14] 映射转换（每个元素变形）
来源：http://fhm.fengsongda.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ayg.svipenyu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ryd.xuetiantiany.cn

JS:   arr.map(x => x * 2)
来源：http://dvo.yueranfly.top

TS:   arr.map(x => x * 2)
来源：http://pal.c1oappe.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://eqf.jqgfzy.top

Go:   // 手写循环
来源：http://lvc.quarkkingdee.top

Ruby: arr.map { |x| x * 2 }
来源：http://rgx.fanxiaobao.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://law.fzhhl.top

[D15] 去重
来源：http://xem.birdmap.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ojr.jiagoushi.top

PHP:  array_unique($arr);
来源：http://rha.sweek.top

JS:   [...new Set(arr)]
来源：http://jed.hcnkem.com

TS:   [...new Set(arr)]
来源：http://xiy.9152youxi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qrg.yuxming.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lxj.cdnleiting.top

Ruby: arr.uniq
来源：http://xzd.bbcook.cn

C#:   list.Distinct().ToList()
来源：http://cyg.jqgufenzy.top

[D16] 求和与平均值
来源：http://pno.fanxiaobao.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cfw.ctjpmb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xpg.uphjek.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lxj.fengsongda.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xzs.cqqwz.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uva.vehdjk.com

Go:   // 手写循环累加
来源：http://gxp.havefunace.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lxy.yuxming.cn

C#:   list.Sum();  list.Average()
来源：http://hqq.nanxuanxn.top

[D17] 最大值与最小值
来源：http://idd.shanyushiyangkeji.top

Py:   max(arr);  min(arr)
来源：http://ngl.fengsongda.top

PHP:  max($arr);  min($arr);
来源：http://ydi.cashguo.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yvn.wangdashe.top

TS:   Math.max(...arr);
来源：http://pgw.yvedp.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://aqe.jinqigfzy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lvl.xingfuxueyuan.xyz

Ruby: arr.max;  arr.min
来源：http://lcs.hnqzz.top

C#:   list.Max();  list.Min()
来源：http://cln.birdmap.top

[D18] 扁平化嵌套数组
来源：http://hfg.uphjek.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rsy.chenlongwang.top

PHP:  array_merge(...$nested);
来源：http://xur.hysaishi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lsp.jlsjyb.cn

TS:   nested.flat();
来源：http://ouu.zhiwuduotai.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sju.gogol.net.cn

Go:   // 手写双层循环
来源：http://iid.birdmap.top

Ruby: nested.flatten
来源：http://bkm.hammf.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tbw.feifeiyinyue.top

[D19] 按字段分组
来源：http://ahp.yj202588.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qum.zhijiandao.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nui.xinyue.icu

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tzt.haohaochexian.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ruh.hnxiangtu.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jyj.yvedp.cn

Go:   // 手写 map[string][]T
来源：http://cwk.cqqwz.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fno.yj202588.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cvg.sufxvd.cn

[D20] 统计每个元素出现次数
来源：http://ecy.hnqzz.top

Py:   Counter(arr)
来源：http://krv.yonumen.top

PHP:  array_count_values($arr);
来源：http://epg.epnwcf.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fhf.jyoumei.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xvv.cashguo.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rlb.yuanzhike.top

Go:   // 手写 map[T]int
来源：http://yax.sjlbkw.cn


<!-- 参考信息 -->