代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wwo.jyoumei.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://djt.shanyushiyangkeji.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rsa.guowangkeji.top

Java: // 无：用 Builder 模式或 record
来源：http://bam.zhiwuduotai.top

Go:   // 无：用配置结构体参数
来源：http://nld.shzxlz.cn

Ruby: f(a: 1, b: 2)
来源：http://als.shanyushiyangtech.top

C#:   f(a: 1, b: 2)
来源：http://hjp.birdmap.top

[C05] 返回多个值
来源：http://ggm.kuanghao11.cn

Py:   return a, b
来源：http://zxs.shangyingyoupin.top

PHP:  return [$a, $b];
来源：http://dkl.zhoulong.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://bie.ywan-chungtsiang.top

TS:   return { a, b };
来源：http://zzv.0kj1m.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cyr.smart0.xyz

Go:   return a, b
来源：http://sid.yongpay.top

Ruby: return a, b
来源：http://wap.hfpthk.cn

C#:   return (a, b);              // ValueTuple
来源：http://rft.zhengqikj.top

[C06] 匿名函数 / lambda
来源：http://vxf.yueranfly.top

Py:   square = lambda x: x * x
来源：http://dwh.c1oappe.top

PHP:  $square = fn($x) => $x * $x;
来源：http://yyw.zhengqikj.top

JS:   const square = x => x * x;
来源：http://koc.nanxuanxn.top

TS:   const square = (x: number): number => x * x;
来源：http://qpr.jqgfzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hqr.jiagoushi.top

Go:   sq := func(x int) int { return x * x }
来源：http://ppv.quarkkingdee.top

Ruby: square = ->(x) { x * x }
来源：http://orf.ehwqpu.com

C#:   Func<int, int> square = x => x * x;
来源：http://khz.chenlongwang.top

[C07] 把函数作为参数传入
来源：http://lpy.yfazqb.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mqg.ywan-chungtsiang.top

PHP:  array_map("strtoupper", $arr);
来源：http://gkn.svipenyu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pbm.chenzaomai.com

TS:   arr.map(String)
来源：http://jyz.0kj1m.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wum.9152youxi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qdr.hnxiangtu.top

Ruby: arr.map(&:upcase)
来源：http://omc.andypj.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://hwg.aibaodan.cn

[C08] 闭包
来源：http://zsn.jinqigfzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jdu.haohaochexian.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jth.cdnleiting.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cdo.sysykeji.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rms.shanyushiyangtech.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nan.ivvv.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wuj.hammf.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mld.ybcxt.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qnn.tarul.cn

[C09] 递归
来源：http://sya.yj20258888.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ptz.ctjpmb.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://aak.dianchejie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://njq.kuanghao11.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qgm.mhx1999.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nqw.jianghu66.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sxm.zycfv.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lph.chenjidiqi.icu

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://upq.tarul.cn

[C10] 变量作用域
来源：http://wur.316326.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ucv.tarul.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bco.zhiwuduotai.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://utb.cdnleiting.top

TS:   同 JS
来源：http://cxg.smart0.xyz

Java: 方法内为块级作用域
来源：http://ayv.pycfn.com

Go:   花括号块级作用域
来源：http://gmf.daxiang520.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jkv.hammf.cn

C#:   块级作用域
来源：http://ysx.zhoulong.xyz

[C11] 模块导入与导出
来源：http://lji.xylfe.cn

Py:   from module import func
来源：http://zoo.sweek.top

PHP:  require "file.php";  或 use App\Service;
来源：http://xgq.jlsjyb.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://htn.ctjpmb.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kdp.redwolf501.top

Java: import java.util.List;
来源：http://kii.zycfv.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pth.pycfn.com

Ruby: require "json"; require_relative "./util"
来源：http://osz.birdmap.top

C#:   using System.Text;
来源：http://tjz.fzhhl.top

[C12] 立即执行函数 IIFE
来源：http://ciy.snrcjt.cn

Py:   (lambda: print("run"))()
来源：http://cdn.quarkkingdee.top

PHP:  (function () { echo "run"; })();
来源：http://vwe.jinghuilouyu.cn

JS:   (() => { console.log("run"); })();
来源：http://qxy.fanxiaobao.xyz

TS:   (() => { console.log("run"); })();
来源：http://udc.gotoacloud.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wsi.zhoulong.xyz

Go:   func() { fmt.Println("run") }()
来源：http://olr.9152youxi.cn

Ruby: -> { puts "run" }.call
来源：http://pgf.aibaodan.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jpv.dashuyun.cn

[C13] 类型声明 / 类型注解
来源：http://ryj.bjfxy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gnh.hcnkem.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jiz.feifeiyinyue.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://avf.gaohongyu789.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vov.zhengqikj.top

Java: int add(int a, int b) { return a + b; }
来源：http://mzm.52xcode.cn

Go:   func add(a, b int) int
来源：http://goo.pengpengdd.cyou

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wup.gotoacloud.top

C#:   int Add(int a, int b) => a + b;
来源：http://gts.daria6918.cn

[C14] 泛型函数
来源：http://hbb.zycfv.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nnz.jqgufenzy.top

PHP:  // 无泛型
来源：http://wdu.gaohongyu789.top

JS:   // 无泛型
来源：http://dqp.ywan-chungtsiang.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gah.hongshengwenyu.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gel.chenzaomai.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hui.smart0.xyz

Ruby: # 无泛型
来源：http://nlj.bbcook.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://woz.epnwcf.com

[C15] 解构 / 展开参数
来源：http://hga.kuanghao11.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bet.daxiang520.top

PHP:  [$a, $b] = $pair;
来源：http://igw.feifeiyinyue.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dql.ywan-chungtsiang.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uos.chenjidiqi.icu

Java: // 无解构
来源：http://gfc.smart0.xyz

Go:   // 无解构
来源：http://woi.hfpthk.cn

Ruby: a, b = pair
来源：http://cql.jianghu66.top

C#:   var (a, b) = pair;
来源：http://yfc.haohaochexian.top

[C16] 函数 / 方法重载
来源：http://myf.yongpay.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://veq.cashguo.top

PHP:  // 无重载
来源：http://hjh.yj20258888.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://emb.daxiang520.top

TS:   // 用联合类型或重载签名声明
来源：http://nvk.bbcook.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dtw.jqgfzy.top

Go:   // 无重载：用不同函数名
来源：http://rxo.yueranfly.top

Ruby: # 无重载：靠动态参数
来源：http://epw.chenjidiqi.icu

C#:   void F(int a) {}  void F(string a) {}
来源：http://eia.zdqjudy.top

================================================================================
来源：http://nnx.hysaishi.cn

D. 数组 / 列表 / 集合
来源：http://grp.zhijiandao.cn

================================================================================
来源：http://ovj.cdnleiting.top

[D01] 创建数组 / 列表
来源：http://ngu.zhoulong.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://huc.jqgufenzy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rmk.hcnkem.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ora.zhixingplan.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://sme.cheryme.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lza.nwbrower.top

Go:   arr := []int{1, 2, 3}
来源：http://asf.chenzaomai.com

Ruby: arr = [1, 2, 3]
来源：http://ytt.zhengqikj.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zcn.52xcode.cn

[D02] 追加元素到末尾
来源：http://rly.cucudq.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ksg.jqgfzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yqd.guannengcc.top

JS:   arr.push(4);
来源：http://siw.zhaomingkeji.xyz

TS:   arr.push(4);
来源：http://fdq.c1oappe.top

Java: list.add(4);
来源：http://dix.nanxuanxn.top

Go:   arr = append(arr, 4)
来源：http://btc.bbcook.cn

Ruby: arr << 4; arr.push(5)
来源：http://yof.hnxiangtu.top

C#:   list.Add(4);
来源：http://taf.zhijiandao.cn

[D03] 在指定位置插入元素
来源：http://sdp.meibo888.top

Py:   arr.insert(0, 0)
来源：http://uiq.yuxming.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rkh.tianlin.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://krm.316326.xyz

TS:   arr.splice(0, 0, 0);
来源：http://aak.daxiang520.top

Java: list.add(0, 0);
来源：http://ixh.dashuyun.cn

Go:   arr = append([]int{0}, arr...)
来源：http://uxw.aibaodan.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lac.hammf.cn

C#:   list.Insert(0, 0);
来源：http://ito.vqdsnc.cn

[D04] 删除元素
来源：http://mfp.yj20258.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kjs.smart0.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mdc.havefunace.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ziz.jqgfzy.top

TS:   arr.splice(0, 1);
来源：http://cxk.bbcook.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nmf.vqdsnc.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gcf.pengpengdd.cyou

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tvu.wangdashe.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jed.gaohongyu789.top

[D05] 访问与修改元素
来源：http://khd.jinyuanbaomall.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vvf.sufxvd.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dem.pengpengdd.cyou

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ujh.nwbrower.top

TS:   arr[0]; arr.at(-1);
来源：http://ujw.zhijiandao.cn

Java: list.get(0); list.set(0, 9);
来源：http://dwm.smart0.xyz

Go:   arr[0]; arr[0] = 9
来源：http://unv.chenzaomai.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qrb.aibaodan.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zrk.chenzaomai.com

[D06] 数组长度
来源：http://elh.jyoumei.cn

Py:   len(arr)
来源：http://hix.yfazqb.com

PHP:  count($arr);
来源：http://bzj.zhongyouzk.top

JS:   arr.length
来源：http://vud.ywan-chungtsiang.top

TS:   arr.length
来源：http://edy.sjlbkw.cn

Java: list.size();
来源：http://snt.birdmap.top

Go:   len(arr)
来源：http://anh.uphjek.com

Ruby: arr.length; arr.size
来源：http://rjj.xingfuxueyuan.xyz

C#:   list.Count;
来源：http://nlp.hnqzz.top

[D07] 切片 / 取子数组
来源：http://mgr.xuetiantiany.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bbm.shangyingyoupin.top

PHP:  array_slice($arr, 1, 3);
来源：http://wme.fengsongda.top

JS:   arr.slice(1, 4);
来源：http://mjy.shanyushiyangtech.top

TS:   arr.slice(1, 4);
来源：http://yve.cashguo.top

Java: list.subList(1, 4);
来源：http://dsk.ctjpmb.com

Go:   arr[1:4]
来源：http://bbg.ctjpmb.com

Ruby: arr[1, 3]
来源：http://rrn.zhoulong.xyz

C#:   list.GetRange(1, 3);
来源：http://cod.hywenlv.cn

[D08] 合并两个数组
来源：http://jha.ydzc1.top

Py:   a + b;  a.extend(b)
来源：http://wdv.yfazqb.com

PHP:  array_merge($a, $b);
来源：http://owz.yj202588.top

JS:   [...a, ...b];  a.concat(b);
来源：http://yps.yongpay.top

TS:   [...a, ...b];
来源：http://boz.shanyushiyangkeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tub.hysaishi.cn

Go:   append(a, b...)
来源：http://xed.xuanzx.com

Ruby: a + b;  a.concat(b)
来源：http://nhj.c1oappe.top

C#:   a.Concat(b).ToList()
来源：http://mga.jqgufenzy.top

[D09] 排序（升序）
来源：http://esk.guannengcc.top

Py:   sorted(arr);  arr.sort()
来源：http://zjt.ywan-chungtsiang.top

PHP:  sort($arr);
来源：http://isp.gogol.net.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bkw.hongshengwenyu.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://rad.yj20258888.top

Java: Collections.sort(list);  list.sort(null);
来源：http://txt.shanyushiyangtech.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pkt.tanke756.top

Ruby: arr.sort
来源：http://for.redwolf501.top

C#:   list.Sort();
来源：http://ahy.meibo888.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://olr.birdmap.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://afd.daria6918.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qqh.tanke756.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lvj.ehwqpu.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://twp.bbcook.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zrj.zhengqikj.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dbc.yj202588.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pcp.fzhhl.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://iwv.bbcook.cn

[D11] 反转数组
来源：http://kcb.ydzc1.top

Py:   arr[::-1];  arr.reverse()
来源：http://wqw.dianchejie.cn

PHP:  array_reverse($arr);
来源：http://wok.zhengqikj.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bcq.gotoacloud.top

TS:   [...arr].reverse();
来源：http://ljr.redwolf501.top

Java: Collections.reverse(list);
来源：http://evc.zdqjudy.top

Go:   slices.Reverse(arr)
来源：http://epo.gotoacloud.top

Ruby: arr.reverse
来源：http://ymt.jinqigfzy.top

C#:   list.Reverse();
来源：http://bwu.bjfxy.top

[D12] 查找元素下标
来源：http://sjp.shangyingyoupin.top

Py:   arr.index(x);  x in arr
来源：http://nvq.epnwcf.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bjb.fengsongda.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gip.shanyushiyangkeji.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tps.yuxming.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ufy.ydjk.org.cn

Go:   slices.Index(arr, x)
来源：http://iue.chenlongwang.top

Ruby: arr.index(x)
来源：http://hwq.sysykeji.top

C#:   list.IndexOf(x);
来源：http://kwd.nanxuanxn.top

[D13] 过滤（保留满足条件的）
来源：http://bzv.yueranfly.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://iqk.sysykeji.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vkd.mhx1999.top

JS:   arr.filter(x => x > 3)
来源：http://owd.jyoumei.cn

TS:   arr.filter(x => x > 3)
来源：http://wpd.epnwcf.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mkz.ydzc1.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cil.ywan-chungtsiang.top

Ruby: arr.select { |x| x > 3 }
来源：http://isz.epnwcf.com

C#:   list.Where(x => x > 3).ToList()
来源：http://quu.uphjek.com

[D14] 映射转换（每个元素变形）
来源：http://cxm.gaohongyu789.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://org.yongpay.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lms.ctjpmb.com

JS:   arr.map(x => x * 2)
来源：http://hmp.jinqigfzy.top

TS:   arr.map(x => x * 2)
来源：http://guq.yongpay.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://zjh.yj20258888.top

Go:   // 手写循环
来源：http://wsj.pycfn.com

Ruby: arr.map { |x| x * 2 }
来源：http://nuc.ivvv.top

C#:   list.Select(x => x * 2).ToList()
来源：http://pql.tian-w.cn

[D15] 去重
来源：http://dln.jinghuilouyu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xxo.snrcjt.cn

PHP:  array_unique($arr);
来源：http://nop.bjfxy.top

JS:   [...new Set(arr)]
来源：http://rea.zhaomingkeji.xyz

TS:   [...new Set(arr)]
来源：http://edn.ywan-chungtsiang.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uox.yanxiufei.cn

Go:   // 用 map[T]struct{} 手写
来源：http://too.zhiwuduotai.top

Ruby: arr.uniq
来源：http://ewy.tianlin.xyz

C#:   list.Distinct().ToList()
来源：http://ygx.snrcjt.cn

[D16] 求和与平均值
来源：http://mqk.bbcook.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ofr.hywenlv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sws.zhiwuduotai.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mvr.vehdjk.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cot.jiagoushi.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://obs.c1oappe.top

Go:   // 手写循环累加
来源：http://nlo.0kj1m.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dhx.smart0.xyz

C#:   list.Sum();  list.Average()
来源：http://deh.sjlbkw.cn

[D17] 最大值与最小值
来源：http://jgk.epnwcf.com

Py:   max(arr);  min(arr)
来源：http://wfu.cucudq.cn

PHP:  max($arr);  min($arr);
来源：http://rml.havefunace.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wmy.haohaochexian.top

TS:   Math.max(...arr);
来源：http://pun.ppjwa.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zmq.pycfn.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ber.pycfn.com

Ruby: arr.max;  arr.min
来源：http://mdo.hysaishi.cn

C#:   list.Max();  list.Min()
来源：http://hlv.vehdjk.com

[D18] 扁平化嵌套数组
来源：http://skb.sufxvd.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://siw.snrcjt.cn

PHP:  array_merge(...$nested);
来源：http://vnt.zhoulong.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lji.zdbjq.cn

TS:   nested.flat();
来源：http://puk.vqdsnc.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nro.sxryk.cn

Go:   // 手写双层循环
来源：http://ttq.jinyuanbaomall.cn

Ruby: nested.flatten
来源：http://cae.xziqi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hxy.nanxuanxn.top

[D19] 按字段分组
来源：http://ukw.316326.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gie.yfazqb.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://clq.tianlin.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://agx.zycfv.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wko.cqqwz.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gci.hnqzz.top

Go:   // 手写 map[string][]T
来源：http://hsm.epnwcf.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://izh.andypj.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lml.fengsongda.top

[D20] 统计每个元素出现次数
来源：http://hoc.zhongyouzk.top

Py:   Counter(arr)
来源：http://cpb.yj202588.top

PHP:  array_count_values($arr);
来源：http://kqp.xuetiantiany.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hma.jinghuilouyu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lmz.nanxuanxn.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://frw.yongpay.top

Go:   // 手写 map[T]int
来源：http://yvq.jlsjyb.cn

Ruby: arr.tally
来源：http://yto.tanke756.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pdu.meibo888.top

[D21] 判断是否包含某元素
来源：http://evf.ehwqpu.com

Py:   x in arr
来源：http://jbg.yvedp.cn


<!-- 参考信息 -->