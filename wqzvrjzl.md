代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jkq.andypj.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xpc.sufxvd.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sus.xinyue.icu

Java: // 无：用 Builder 模式或 record
来源：http://dad.hcnkem.com

Go:   // 无：用配置结构体参数
来源：http://khe.zhengqikj.top

Ruby: f(a: 1, b: 2)
来源：http://kcc.gzhubu.top

C#:   f(a: 1, b: 2)
来源：http://pkg.nwbrower.top

[C05] 返回多个值
来源：http://xva.hfpthk.cn

Py:   return a, b
来源：http://agj.jiagoushi.top

PHP:  return [$a, $b];
来源：http://nph.wangdashe.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://xyp.0kj1m.cn

TS:   return { a, b };
来源：http://flj.pycfn.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kfn.sxryk.cn

Go:   return a, b
来源：http://bdf.hywenlv.cn

Ruby: return a, b
来源：http://fan.jinyuanbaomall.cn

C#:   return (a, b);              // ValueTuple
来源：http://lqo.jinghuilouyu.cn

[C06] 匿名函数 / lambda
来源：http://oys.dashuyun.cn

Py:   square = lambda x: x * x
来源：http://hrt.zhixingplan.top

PHP:  $square = fn($x) => $x * $x;
来源：http://qqq.ydzc1.top

JS:   const square = x => x * x;
来源：http://wau.haohaochexian.top

TS:   const square = (x: number): number => x * x;
来源：http://oah.shangyingyoupin.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bou.vehdjk.com

Go:   sq := func(x int) int { return x * x }
来源：http://xaf.9152youxi.cn

Ruby: square = ->(x) { x * x }
来源：http://hnw.hysaishi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://uss.shanyushiyangkeji.top

[C07] 把函数作为参数传入
来源：http://aca.haohaochexian.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vbi.daxiang520.top

PHP:  array_map("strtoupper", $arr);
来源：http://zvg.iojbl.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tri.cdnleiting.top

TS:   arr.map(String)
来源：http://tzq.jinghuilouyu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ewv.daxiang520.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bzf.havefunace.top

Ruby: arr.map(&:upcase)
来源：http://haw.sysykeji.top

C#:   arr.Select(s => s.ToUpper())
来源：http://rzy.jinqigfzy.top

[C08] 闭包
来源：http://lzq.pengpengdd.cyou

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ojj.wangshuangyany.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fnt.zhijiandao.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://box.hfpthk.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://utu.cucudq.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hzi.ctjpmb.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xia.yuanzhike.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://slc.aibaodan.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vic.aizwys.cn

[C09] 递归
来源：http://xrr.316326.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zmk.yonumen.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jlj.xylfe.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fcz.yj202588.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aav.bbcook.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ntk.feifeiyinyue.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fly.cqqwz.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://apc.zdqjudy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vug.yuanzhike.top

[C10] 变量作用域
来源：http://cmo.hcnkem.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ktz.sjlbkw.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tdm.tian-w.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://emf.zhoulong.xyz

TS:   同 JS
来源：http://wxp.yongpay.top

Java: 方法内为块级作用域
来源：http://ruj.uphjek.com

Go:   花括号块级作用域
来源：http://wyc.nwbrower.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://put.sysykeji.top

C#:   块级作用域
来源：http://kvm.zdqjudy.top

[C11] 模块导入与导出
来源：http://bmp.epnwcf.com

Py:   from module import func
来源：http://elb.nanxuanxn.top

PHP:  require "file.php";  或 use App\Service;
来源：http://pdw.cucudq.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ila.mhx1999.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hqw.0kj1m.cn

Java: import java.util.List;
来源：http://snf.cashguo.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tmm.hysaishi.cn

Ruby: require "json"; require_relative "./util"
来源：http://yss.pycfn.com

C#:   using System.Text;
来源：http://ujr.jqgfzy.top

[C12] 立即执行函数 IIFE
来源：http://kas.yj20258888.top

Py:   (lambda: print("run"))()
来源：http://uat.nwbrower.top

PHP:  (function () { echo "run"; })();
来源：http://xil.cqqwz.cn

JS:   (() => { console.log("run"); })();
来源：http://mwu.jqgufenzy.top

TS:   (() => { console.log("run"); })();
来源：http://cvx.hongshengwenyu.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://laa.dashuyun.cn

Go:   func() { fmt.Println("run") }()
来源：http://bmk.haohaochexian.top

Ruby: -> { puts "run" }.call
来源：http://efq.jqgfzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://vwz.sjlbkw.cn

[C13] 类型声明 / 类型注解
来源：http://zjn.yfazqb.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wrv.aizwys.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pcy.jinyuanbaomall.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ahh.9152youxi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bgy.hesvh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xzl.hysaishi.cn

Go:   func add(a, b int) int
来源：http://ydw.yueranfly.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rou.jqgufenzy.top

C#:   int Add(int a, int b) => a + b;
来源：http://avl.sweek.top

[C14] 泛型函数
来源：http://hbh.gzhubu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rvx.hammf.cn

PHP:  // 无泛型
来源：http://uok.xinyue.icu

JS:   // 无泛型
来源：http://ecf.ctjpmb.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xjx.wangshuangyany.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://muf.xingfuxueyuan.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mmo.redwolf501.top

Ruby: # 无泛型
来源：http://uqc.ywan-chungtsiang.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bvw.fktsv.cn

[C15] 解构 / 展开参数
来源：http://sjn.tarul.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://uhb.ppjwa.cn

PHP:  [$a, $b] = $pair;
来源：http://qeg.shanyushiyangtech.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vie.zdbjq.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xui.0kj1m.cn

Java: // 无解构
来源：http://pwc.jinqigfzy.top

Go:   // 无解构
来源：http://rjc.epnwcf.com

Ruby: a, b = pair
来源：http://mfl.xziqi.cn

C#:   var (a, b) = pair;
来源：http://aso.jlsjyb.cn

[C16] 函数 / 方法重载
来源：http://cml.vehdjk.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vuf.gotoacloud.top

PHP:  // 无重载
来源：http://xil.aizwys.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://kmq.jinghuilouyu.cn

TS:   // 用联合类型或重载签名声明
来源：http://gma.ctjpmb.com

Java: void f(int a) {}  void f(String a) {}
来源：http://eil.cheryme.top

Go:   // 无重载：用不同函数名
来源：http://ivl.tianlin.xyz

Ruby: # 无重载：靠动态参数
来源：http://jfy.kuanghao11.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hhc.hysaishi.cn

================================================================================
来源：http://viy.jqgufenzy.top

D. 数组 / 列表 / 集合
来源：http://tsd.yvedp.cn

================================================================================
来源：http://nea.sxryk.cn

[D01] 创建数组 / 列表
来源：http://zlz.ehwqpu.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://gwe.sysykeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cnu.feifeiyinyue.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ioj.fanxiaobao.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://lip.tarul.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wmt.yfazqb.com

Go:   arr := []int{1, 2, 3}
来源：http://hse.yvedp.cn

Ruby: arr = [1, 2, 3]
来源：http://izt.sxryk.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ffr.ppjwa.cn

[D02] 追加元素到末尾
来源：http://pmm.fktsv.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wqx.fengsongda.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vcc.cdnleiting.top

JS:   arr.push(4);
来源：http://jhj.hcnkem.com

TS:   arr.push(4);
来源：http://avs.jlsjyb.cn

Java: list.add(4);
来源：http://yom.yangfankeji.com

Go:   arr = append(arr, 4)
来源：http://gxr.snrcjt.cn

Ruby: arr << 4; arr.push(5)
来源：http://cok.gaohongyu789.top

C#:   list.Add(4);
来源：http://tgb.snrcjt.cn

[D03] 在指定位置插入元素
来源：http://znf.yanxiufei.cn

Py:   arr.insert(0, 0)
来源：http://edj.cqqwz.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nfr.yfazqb.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bri.wangshuangyany.cn

TS:   arr.splice(0, 0, 0);
来源：http://hdq.zhongyouzk.top

Java: list.add(0, 0);
来源：http://egq.cucudq.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yhz.sjlbkw.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://drz.nwbrower.top

C#:   list.Insert(0, 0);
来源：http://nsf.shangyingyoupin.top

[D04] 删除元素
来源：http://osw.nwbrower.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ukw.316326.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wmz.zhengqikj.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qrh.chenzaomai.com

TS:   arr.splice(0, 1);
来源：http://grb.zhixingplan.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wxt.xziqi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fle.fzhhl.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qde.chenjidiqi.icu

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dgj.iojbl.cn

[D05] 访问与修改元素
来源：http://dsv.hammf.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gkq.tianlin.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ayr.svipenyu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://svq.hesvh.cn

TS:   arr[0]; arr.at(-1);
来源：http://kyl.ivvv.top

Java: list.get(0); list.set(0, 9);
来源：http://xxk.guannengcc.top

Go:   arr[0]; arr[0] = 9
来源：http://kds.316326.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ivo.yongpay.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dbk.xziqi.cn

[D06] 数组长度
来源：http://eql.ivvv.top

Py:   len(arr)
来源：http://bve.daxiang520.top

PHP:  count($arr);
来源：http://uqi.jqgufenzy.top

JS:   arr.length
来源：http://gdm.pycfn.com

TS:   arr.length
来源：http://iqt.ppjwa.cn

Java: list.size();
来源：http://gby.jqgufenzy.top

Go:   len(arr)
来源：http://etx.vqdsnc.cn

Ruby: arr.length; arr.size
来源：http://oaq.hcnkem.com

C#:   list.Count;
来源：http://vtw.xuanzx.com

[D07] 切片 / 取子数组
来源：http://kkm.ivvv.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://god.gotoacloud.top

PHP:  array_slice($arr, 1, 3);
来源：http://qog.gotoacloud.top

JS:   arr.slice(1, 4);
来源：http://dnn.meibo888.top

TS:   arr.slice(1, 4);
来源：http://mdr.hammf.cn

Java: list.subList(1, 4);
来源：http://pzm.cdnleiting.top

Go:   arr[1:4]
来源：http://cxm.birdmap.top

Ruby: arr[1, 3]
来源：http://ndi.yanxiufei.cn

C#:   list.GetRange(1, 3);
来源：http://jpa.redwolf501.top

[D08] 合并两个数组
来源：http://hlj.bbcook.cn

Py:   a + b;  a.extend(b)
来源：http://ima.jinqigufen.top

PHP:  array_merge($a, $b);
来源：http://ojw.xziqi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zxs.ydjk.org.cn

TS:   [...a, ...b];
来源：http://msp.hesvh.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fyo.yangfankeji.com

Go:   append(a, b...)
来源：http://gbh.yj20258.top

Ruby: a + b;  a.concat(b)
来源：http://tpx.sjlbkw.cn

C#:   a.Concat(b).ToList()
来源：http://adx.cashguo.top

[D09] 排序（升序）
来源：http://eno.ctjpmb.com

Py:   sorted(arr);  arr.sort()
来源：http://cib.aibaodan.cn

PHP:  sort($arr);
来源：http://qyz.hysaishi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zkf.zycfv.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://iix.yfazqb.com

Java: Collections.sort(list);  list.sort(null);
来源：http://cby.zhixingplan.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://iez.gzhubu.top

Ruby: arr.sort
来源：http://gba.yanxiufei.cn

C#:   list.Sort();
来源：http://xed.haohaochexian.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://enc.ivvv.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lut.yonumen.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zvm.tian-w.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nyf.svipenyu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://prz.9152youxi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nvd.yuxming.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wtq.yonumen.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://svg.chenzaomai.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yal.jqgufenzy.top

[D11] 反转数组
来源：http://srq.ydjk.org.cn

Py:   arr[::-1];  arr.reverse()
来源：http://fiv.nanxinkj.top

PHP:  array_reverse($arr);
来源：http://hzy.zhengqikj.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qaf.shanyushiyangtech.top

TS:   [...arr].reverse();
来源：http://rkk.iojbl.cn

Java: Collections.reverse(list);
来源：http://mwi.cashguo.top

Go:   slices.Reverse(arr)
来源：http://wlz.shzxlz.cn

Ruby: arr.reverse
来源：http://lne.kuanghao11.cn

C#:   list.Reverse();
来源：http://oag.smart0.xyz

[D12] 查找元素下标
来源：http://ech.fanxiaobao.xyz

Py:   arr.index(x);  x in arr
来源：http://sjy.snrcjt.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bxs.gogol.net.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://crj.zhoulong.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sxd.fengsongda.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rrx.haohaochexian.top

Go:   slices.Index(arr, x)
来源：http://rht.redwolf501.top

Ruby: arr.index(x)
来源：http://ynj.daxiang520.top

C#:   list.IndexOf(x);
来源：http://kji.aizwys.cn

[D13] 过滤（保留满足条件的）
来源：http://qrb.zhaomingkeji.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vob.chenjidiqi.icu

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bzo.yongpay.top

JS:   arr.filter(x => x > 3)
来源：http://tpi.zhixingplan.top

TS:   arr.filter(x => x > 3)
来源：http://afc.birdmap.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kuu.fehbvm.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lik.gaohongyu789.top

Ruby: arr.select { |x| x > 3 }
来源：http://jcl.shangyingyoupin.top

C#:   list.Where(x => x > 3).ToList()
来源：http://dlp.snrcjt.cn

[D14] 映射转换（每个元素变形）
来源：http://tod.cucudq.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://skh.sxryk.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dxe.hnxiangtu.top

JS:   arr.map(x => x * 2)
来源：http://jgg.andypj.xyz

TS:   arr.map(x => x * 2)
来源：http://dob.ivvv.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://zkd.ivvv.top

Go:   // 手写循环
来源：http://xbf.sufxvd.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fnv.fzhhl.top

C#:   list.Select(x => x * 2).ToList()
来源：http://tdl.daxiang520.top

[D15] 去重
来源：http://fes.zhijiandao.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tbr.iojbl.cn

PHP:  array_unique($arr);
来源：http://too.ppjwa.cn

JS:   [...new Set(arr)]
来源：http://aln.xingfuxueyuan.xyz

TS:   [...new Set(arr)]
来源：http://sqz.fanxiaobao.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tdc.c1oappe.top

Go:   // 用 map[T]struct{} 手写
来源：http://owb.shanyushiyangtech.top

Ruby: arr.uniq
来源：http://uty.yangfankeji.com

C#:   list.Distinct().ToList()
来源：http://fvb.jinqigfzy.top

[D16] 求和与平均值
来源：http://rlw.fengsongda.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://crr.smart0.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zeo.cdnleiting.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sln.nwbrower.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://axe.aibaodan.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fvs.sysykeji.top

Go:   // 手写循环累加
来源：http://wex.tian-w.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tsh.iojbl.cn

C#:   list.Sum();  list.Average()
来源：http://xgp.316326.xyz

[D17] 最大值与最小值
来源：http://sdn.9152youxi.cn

Py:   max(arr);  min(arr)
来源：http://rpm.zhongyouzk.top

PHP:  max($arr);  min($arr);
来源：http://tch.gaohongyu789.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ent.jlsjyb.cn

TS:   Math.max(...arr);
来源：http://inf.ehwqpu.com

Java: Collections.max(list);  Collections.min(list);
来源：http://jat.ydzc1.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qyp.zhijiandao.cn

Ruby: arr.max;  arr.min
来源：http://lzc.yj20258888.top

C#:   list.Max();  list.Min()
来源：http://hvg.cqqwz.cn

[D18] 扁平化嵌套数组
来源：http://tom.chenjidiqi.icu

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bws.uphjek.com

PHP:  array_merge(...$nested);
来源：http://mfo.yuxming.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://veb.xuetiantiany.cn

TS:   nested.flat();
来源：http://tgv.redwolf501.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ntv.sufxvd.cn

Go:   // 手写双层循环
来源：http://ndo.nanxuanxn.top

Ruby: nested.flatten
来源：http://fiw.meibo888.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://qpn.tian-w.cn

[D19] 按字段分组
来源：http://nzy.meibo888.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://plk.birdmap.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lyv.ydjk.org.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://iqm.hammf.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://unl.cashguo.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jwe.havefunace.top

Go:   // 手写 map[string][]T
来源：http://tdp.gzhubu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://wrv.yueranfly.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wec.yfazqb.com

[D20] 统计每个元素出现次数
来源：http://pck.cucudq.cn

Py:   Counter(arr)
来源：http://mnu.yanxiufei.cn

PHP:  array_count_values($arr);
来源：http://lgm.ydjk.org.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mqg.iojbl.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gca.cqqwz.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zin.jyoumei.cn

Go:   // 手写 map[T]int
来源：http://cwh.gzhubu.top

Ruby: arr.tally
来源：http://kny.hesvh.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dlp.sysykeji.top

[D21] 判断是否包含某元素
来源：http://nnk.feifeiyinyue.top

Py:   x in arr
来源：http://nzs.jiagoushi.top


<!-- 参考信息 -->