代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://iib.yj20258.top

Ruby: f(a: 1, b: 2)
来源：http://mpq.bbcook.cn

C#:   f(a: 1, b: 2)
来源：http://rhn.tarul.cn

[C05] 返回多个值
来源：http://aoj.ydjk.org.cn

Py:   return a, b
来源：http://uhd.svipenyu.cn

PHP:  return [$a, $b];
来源：http://cbb.wangdashe.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ttx.ivvv.top

TS:   return { a, b };
来源：http://dys.hongshengwenyu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jwu.snrcjt.cn

Go:   return a, b
来源：http://bcm.iojbl.cn

Ruby: return a, b
来源：http://prv.redwolf501.top

C#:   return (a, b);              // ValueTuple
来源：http://hbv.cdnleiting.top

[C06] 匿名函数 / lambda
来源：http://vhh.ydjk.org.cn

Py:   square = lambda x: x * x
来源：http://hkv.hfpthk.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ijh.yj20258888.top

JS:   const square = x => x * x;
来源：http://ait.yonumen.top

TS:   const square = (x: number): number => x * x;
来源：http://sfk.yongpay.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://emw.yfazqb.com

Go:   sq := func(x int) int { return x * x }
来源：http://ivu.ywan-chungtsiang.top

Ruby: square = ->(x) { x * x }
来源：http://ult.xziqi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cop.vehdjk.com

[C07] 把函数作为参数传入
来源：http://oxj.hywenlv.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gzm.birdmap.top

PHP:  array_map("strtoupper", $arr);
来源：http://euk.yanxiufei.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ykv.c1oappe.top

TS:   arr.map(String)
来源：http://ocv.zdqjudy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://awd.zhijiandao.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wic.vehdjk.com

Ruby: arr.map(&:upcase)
来源：http://jkb.shangyingyoupin.top

C#:   arr.Select(s => s.ToUpper())
来源：http://srx.yanxiufei.cn

[C08] 闭包
来源：http://jza.hesvh.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ghw.hfpthk.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://snb.tanke756.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sdz.cqqwz.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qsj.gotoacloud.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://shx.tarul.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lmr.zhixingplan.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xhb.svipenyu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nfx.aibaodan.cn

[C09] 递归
来源：http://ujh.shuidangran.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lan.zhaomingkeji.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://isz.nanxinkj.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xgb.0kj1m.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ohd.yonumen.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bxc.tian-w.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tnc.cdnleiting.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jhy.aibaodan.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ydm.jinyuanbaomall.cn

[C10] 变量作用域
来源：http://ctv.tian-w.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fhu.andypj.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://uhb.ydzc1.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nmg.jiagoushi.top

TS:   同 JS
来源：http://mpo.yongpay.top

Java: 方法内为块级作用域
来源：http://yyg.svipenyu.cn

Go:   花括号块级作用域
来源：http://usv.wangdashe.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://soc.guowangkeji.top

C#:   块级作用域
来源：http://wqv.jinghuilouyu.cn

[C11] 模块导入与导出
来源：http://xev.sufxvd.cn

Py:   from module import func
来源：http://jpi.wangdashe.top

PHP:  require "file.php";  或 use App\Service;
来源：http://sog.fktsv.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fkh.yj20258888.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://toi.yanxiufei.cn

Java: import java.util.List;
来源：http://dvn.birdmap.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://znc.jinqigfzy.top

Ruby: require "json"; require_relative "./util"
来源：http://teg.fktsv.cn

C#:   using System.Text;
来源：http://oao.ybcxt.top

[C12] 立即执行函数 IIFE
来源：http://bsp.jianghu66.top

Py:   (lambda: print("run"))()
来源：http://fnf.kuanghao11.cn

PHP:  (function () { echo "run"; })();
来源：http://ltx.sweek.top

JS:   (() => { console.log("run"); })();
来源：http://qjw.guowangkeji.top

TS:   (() => { console.log("run"); })();
来源：http://mij.tian-w.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://okd.gogol.net.cn

Go:   func() { fmt.Println("run") }()
来源：http://izu.epnwcf.com

Ruby: -> { puts "run" }.call
来源：http://djs.svipenyu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mfo.xingfuxueyuan.xyz

[C13] 类型声明 / 类型注解
来源：http://gso.wangshuangyany.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://odz.jinyuanbaomall.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mct.pengpengdd.cyou

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rcb.ctjpmb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wcj.smart0.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://ral.52xcode.cn

Go:   func add(a, b int) int
来源：http://btk.jlsjyb.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lgw.yuanzhike.top

C#:   int Add(int a, int b) => a + b;
来源：http://yna.yuanzhike.top

[C14] 泛型函数
来源：http://jvb.bbcook.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://iwi.ivvv.top

PHP:  // 无泛型
来源：http://acv.jqgfzy.top

JS:   // 无泛型
来源：http://ggh.gogol.net.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dcr.ybcxt.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fdz.smart0.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qgx.yuanzhike.top

Ruby: # 无泛型
来源：http://kfi.yj20258888.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://oxj.fktsv.cn

[C15] 解构 / 展开参数
来源：http://ddb.sjlbkw.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ixc.tian-w.cn

PHP:  [$a, $b] = $pair;
来源：http://hfe.yongpay.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://aqt.vqdsnc.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jno.jyoumei.cn

Java: // 无解构
来源：http://gbx.zhixingplan.top

Go:   // 无解构
来源：http://akj.fanxiaobao.xyz

Ruby: a, b = pair
来源：http://eft.zhaomingkeji.xyz

C#:   var (a, b) = pair;
来源：http://evn.gotoacloud.top

[C16] 函数 / 方法重载
来源：http://dzu.tanke756.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://uya.zhiwuduotai.top

PHP:  // 无重载
来源：http://hkj.jianghu66.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://puy.52xcode.cn

TS:   // 用联合类型或重载签名声明
来源：http://usz.jqgufenzy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ozh.chenzaomai.com

Go:   // 无重载：用不同函数名
来源：http://tmp.c1oappe.top

Ruby: # 无重载：靠动态参数
来源：http://xhe.ehwqpu.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://hlo.aibaodan.cn

================================================================================
来源：http://dgz.shzxlz.cn

D. 数组 / 列表 / 集合
来源：http://dsn.xinyue.icu

================================================================================
来源：http://lfl.redwolf501.top

[D01] 创建数组 / 列表
来源：http://icx.hesvh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://opo.sjlbkw.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tpj.gogol.net.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nqp.jqgfzy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://zgq.gaohongyu789.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xwv.zhijiandao.cn

Go:   arr := []int{1, 2, 3}
来源：http://bgz.sxryk.cn

Ruby: arr = [1, 2, 3]
来源：http://cwq.tianlin.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bbc.gogol.net.cn

[D02] 追加元素到末尾
来源：http://oki.yvedp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ohe.daria6918.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pyp.quarkkingdee.top

JS:   arr.push(4);
来源：http://slr.ehwqpu.com

TS:   arr.push(4);
来源：http://dja.fzhhl.top

Java: list.add(4);
来源：http://iyu.yanxiufei.cn

Go:   arr = append(arr, 4)
来源：http://dsb.shzxlz.cn

Ruby: arr << 4; arr.push(5)
来源：http://gss.fzhhl.top

C#:   list.Add(4);
来源：http://xcr.yonumen.top

[D03] 在指定位置插入元素
来源：http://vlk.hfpthk.cn

Py:   arr.insert(0, 0)
来源：http://tyi.shanyushiyangkeji.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://iij.tanke756.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yut.52xcode.cn

TS:   arr.splice(0, 0, 0);
来源：http://tcq.yueranfly.top

Java: list.add(0, 0);
来源：http://hir.yuanzhike.top

Go:   arr = append([]int{0}, arr...)
来源：http://uuv.cqqwz.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://oaa.yangfankeji.com

C#:   list.Insert(0, 0);
来源：http://vko.jyoumei.cn

[D04] 删除元素
来源：http://fre.vehdjk.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sye.c1oappe.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cjt.chenjidiqi.icu

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://itj.ctjpmb.com

TS:   arr.splice(0, 1);
来源：http://uqv.yuanzhike.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kth.ybcxt.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xqv.jlsjyb.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hka.sysykeji.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://chf.jqgfzy.top

[D05] 访问与修改元素
来源：http://zzy.jinghuilouyu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nru.dashuyun.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dhi.xinyue.icu

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wpe.zhaomingkeji.xyz

TS:   arr[0]; arr.at(-1);
来源：http://djo.hcnkem.com

Java: list.get(0); list.set(0, 9);
来源：http://stz.sysykeji.top

Go:   arr[0]; arr[0] = 9
来源：http://saf.yonumen.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rzb.nwbrower.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bnn.kuanghao11.cn

[D06] 数组长度
来源：http://spf.cdnleiting.top

Py:   len(arr)
来源：http://fou.ivvv.top

PHP:  count($arr);
来源：http://ahz.chenjidiqi.icu

JS:   arr.length
来源：http://vvd.zhaomingkeji.xyz

TS:   arr.length
来源：http://kdn.hesvh.cn

Java: list.size();
来源：http://iwx.yanxiufei.cn

Go:   len(arr)
来源：http://rbx.daxiang520.top

Ruby: arr.length; arr.size
来源：http://hko.birdmap.top

C#:   list.Count;
来源：http://quy.zhaomingkeji.xyz

[D07] 切片 / 取子数组
来源：http://mmd.cheryme.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dgn.dianchejie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ldh.hammf.cn

JS:   arr.slice(1, 4);
来源：http://czk.sufxvd.cn

TS:   arr.slice(1, 4);
来源：http://lra.jinghuilouyu.cn

Java: list.subList(1, 4);
来源：http://gyy.cashguo.top

Go:   arr[1:4]
来源：http://xpo.chenzaomai.com

Ruby: arr[1, 3]
来源：http://swf.dianchejie.cn

C#:   list.GetRange(1, 3);
来源：http://pwb.yj20258888.top

[D08] 合并两个数组
来源：http://ydb.xuanzx.com

Py:   a + b;  a.extend(b)
来源：http://qnw.cdnleiting.top

PHP:  array_merge($a, $b);
来源：http://xvs.fengsongda.top

JS:   [...a, ...b];  a.concat(b);
来源：http://bkz.jinqigfzy.top

TS:   [...a, ...b];
来源：http://afj.zhongyouzk.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fsm.zycfv.cn

Go:   append(a, b...)
来源：http://wnb.hongshengwenyu.top

Ruby: a + b;  a.concat(b)
来源：http://cim.hammf.cn

C#:   a.Concat(b).ToList()
来源：http://vsl.sysykeji.top

[D09] 排序（升序）
来源：http://ymf.9152youxi.cn

Py:   sorted(arr);  arr.sort()
来源：http://rtb.gotoacloud.top

PHP:  sort($arr);
来源：http://bbu.vqdsnc.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ycp.chenlongwang.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://hyy.ywan-chungtsiang.top

Java: Collections.sort(list);  list.sort(null);
来源：http://qkb.sysykeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lah.redwolf501.top

Ruby: arr.sort
来源：http://cth.ywan-chungtsiang.top

C#:   list.Sort();
来源：http://ioz.hysaishi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bog.hfpthk.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jtj.fktsv.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lkn.shanyushiyangtech.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bjb.bbcook.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wkz.fanxiaobao.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mim.aibaodan.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://igp.yongpay.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://not.shzxlz.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mfm.redwolf501.top

[D11] 反转数组
来源：http://ref.hysaishi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://yfa.bjfxy.top

PHP:  array_reverse($arr);
来源：http://moy.bbcook.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yjc.fktsv.cn

TS:   [...arr].reverse();
来源：http://wvx.jqgfzy.top

Java: Collections.reverse(list);
来源：http://gtz.nwbrower.top

Go:   slices.Reverse(arr)
来源：http://wcn.aibaodan.cn

Ruby: arr.reverse
来源：http://qpj.wangshuangyany.cn

C#:   list.Reverse();
来源：http://yev.yueranfly.top

[D12] 查找元素下标
来源：http://ekj.epnwcf.com

Py:   arr.index(x);  x in arr
来源：http://bor.wangshuangyany.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://aan.zycfv.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gpu.jqgufenzy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wgb.xingfuxueyuan.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ncg.zhengqikj.top

Go:   slices.Index(arr, x)
来源：http://ywq.snrcjt.cn

Ruby: arr.index(x)
来源：http://yxf.sweek.top

C#:   list.IndexOf(x);
来源：http://qtv.shzxlz.cn

[D13] 过滤（保留满足条件的）
来源：http://soz.fzhhl.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gcl.yangfankeji.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://odj.9152youxi.cn

JS:   arr.filter(x => x > 3)
来源：http://dzl.yongpay.top

TS:   arr.filter(x => x > 3)
来源：http://joq.aibaodan.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://noq.jinqigufen.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vtx.tanke756.top

Ruby: arr.select { |x| x > 3 }
来源：http://imk.dashuyun.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://rft.zycfv.cn

[D14] 映射转换（每个元素变形）
来源：http://hbi.gaohongyu789.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dwd.gogol.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://oos.smart0.xyz

JS:   arr.map(x => x * 2)
来源：http://law.wangshuangyany.cn

TS:   arr.map(x => x * 2)
来源：http://ire.yongpay.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://iia.daria6918.cn

Go:   // 手写循环
来源：http://nzd.cqqwz.cn

Ruby: arr.map { |x| x * 2 }
来源：http://miq.fehbvm.com

C#:   list.Select(x => x * 2).ToList()
来源：http://etx.yj20258888.top

[D15] 去重
来源：http://bcj.fehbvm.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dak.xylfe.cn

PHP:  array_unique($arr);
来源：http://hts.tian-w.cn

JS:   [...new Set(arr)]
来源：http://esq.316326.xyz

TS:   [...new Set(arr)]
来源：http://wsn.cheryme.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://usy.dianchejie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://jui.snrcjt.cn

Ruby: arr.uniq
来源：http://udi.svipenyu.cn

C#:   list.Distinct().ToList()
来源：http://jai.yj20258888.top

[D16] 求和与平均值
来源：http://fcw.pycfn.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mzo.havefunace.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fxi.cdnleiting.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://viv.birdmap.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vhq.ydjk.org.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ypx.ctjpmb.com

Go:   // 手写循环累加
来源：http://eog.0kj1m.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://aki.hnqzz.top

C#:   list.Sum();  list.Average()
来源：http://wuz.ybcxt.top

[D17] 最大值与最小值
来源：http://wtb.jlsjyb.cn

Py:   max(arr);  min(arr)
来源：http://ghb.aibaodan.cn

PHP:  max($arr);  min($arr);
来源：http://lrv.dashuyun.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cxc.tarul.cn

TS:   Math.max(...arr);
来源：http://htv.dianchejie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://fje.yanxiufei.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yjy.xuanzx.com

Ruby: arr.max;  arr.min
来源：http://wsa.fehbvm.com

C#:   list.Max();  list.Min()
来源：http://mfe.pengpengdd.cyou

[D18] 扁平化嵌套数组
来源：http://bvq.ywan-chungtsiang.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vnr.hongshengwenyu.top

PHP:  array_merge(...$nested);
来源：http://gvd.hcnkem.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kxs.aizwys.cn

TS:   nested.flat();
来源：http://eqe.yj20258888.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hnr.316326.xyz

Go:   // 手写双层循环
来源：http://mng.yuanzhike.top

Ruby: nested.flatten
来源：http://guq.fzhhl.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://unv.xuanzx.com

[D19] 按字段分组
来源：http://gfu.shanyushiyangtech.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hwz.yueranfly.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vtj.chenjidiqi.icu

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rlv.nanxinkj.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://kor.nwbrower.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jac.gzhubu.top

Go:   // 手写 map[string][]T
来源：http://ivt.hnxiangtu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://hdg.ydjk.org.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lrb.meibo888.top

[D20] 统计每个元素出现次数
来源：http://mfv.cashguo.top

Py:   Counter(arr)
来源：http://abm.nwbrower.top

PHP:  array_count_values($arr);
来源：http://keh.zhiwuduotai.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://duz.gogol.net.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://smr.sjlbkw.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bde.fanxiaobao.xyz

Go:   // 手写 map[T]int
来源：http://eyt.sysykeji.top

Ruby: arr.tally
来源：http://bhk.0kj1m.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dob.chenzaomai.com

[D21] 判断是否包含某元素
来源：http://uvu.sxryk.cn

Py:   x in arr
来源：http://ptu.havefunace.top

PHP:  in_array($x, $arr, true);
来源：http://wqy.epnwcf.com

JS:   arr.includes(x)
来源：http://kbg.pycfn.com

TS:   arr.includes(x)
来源：http://xtv.andypj.xyz

Java: list.contains(x)
来源：http://uyc.xuetiantiany.cn


<!-- 参考信息 -->