代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://chm.vqdsnc.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ggx.ywan-chungtsiang.top

[C04] 命名参数 / 关键字参数
来源：http://jbx.ctjpmb.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ndk.chenjidiqi.icu

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zkg.guannengcc.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pdk.yuanzhike.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wpz.yueranfly.top

Java: // 无：用 Builder 模式或 record
来源：http://zfe.yj202588.top

Go:   // 无：用配置结构体参数
来源：http://wnj.shangyingyoupin.top

Ruby: f(a: 1, b: 2)
来源：http://iny.hywenlv.cn

C#:   f(a: 1, b: 2)
来源：http://mif.zhixingplan.top

[C05] 返回多个值
来源：http://ojo.shangyingyoupin.top

Py:   return a, b
来源：http://iuy.bbcook.cn

PHP:  return [$a, $b];
来源：http://pop.jianghu66.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://tyh.bbcook.cn

TS:   return { a, b };
来源：http://xnj.bjfxy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wde.hnxiangtu.top

Go:   return a, b
来源：http://qlt.dashuyun.cn

Ruby: return a, b
来源：http://plm.xylfe.cn

C#:   return (a, b);              // ValueTuple
来源：http://eqm.shanyushiyangtech.top

[C06] 匿名函数 / lambda
来源：http://ywl.jlsjyb.cn

Py:   square = lambda x: x * x
来源：http://gzg.guannengcc.top

PHP:  $square = fn($x) => $x * $x;
来源：http://lfc.cqqwz.cn

JS:   const square = x => x * x;
来源：http://sst.cdnleiting.top

TS:   const square = (x: number): number => x * x;
来源：http://vlr.ydzc1.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://byr.pycfn.com

Go:   sq := func(x int) int { return x * x }
来源：http://nxe.shangyingyoupin.top

Ruby: square = ->(x) { x * x }
来源：http://xti.daxiang520.top

C#:   Func<int, int> square = x => x * x;
来源：http://drd.hysaishi.cn

[C07] 把函数作为参数传入
来源：http://api.gotoacloud.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tjv.zhixingplan.top

PHP:  array_map("strtoupper", $arr);
来源：http://eik.yj20258888.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ius.gogol.net.cn

TS:   arr.map(String)
来源：http://nvc.yj20258.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qph.sweek.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mqi.zhongyouzk.top

Ruby: arr.map(&:upcase)
来源：http://nlm.ehwqpu.com

C#:   arr.Select(s => s.ToUpper())
来源：http://fse.ybcxt.top

[C08] 闭包
来源：http://rkh.jqgufenzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fkb.kuanghao11.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uwg.redwolf501.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wnv.sysykeji.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ezv.zycfv.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://oeg.birdmap.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jsw.redwolf501.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pvv.yongpay.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yko.pycfn.com

[C09] 递归
来源：http://qry.daxiang520.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pto.bjfxy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://est.ctjpmb.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wub.guowangkeji.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zkh.dianchejie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sub.tian-w.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fhr.yueranfly.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sob.nanxuanxn.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://iij.52xcode.cn

[C10] 变量作用域
来源：http://lpo.hcnkem.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ygx.gotoacloud.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fiu.meibo888.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xol.zhiwuduotai.top

TS:   同 JS
来源：http://lal.meibo888.top

Java: 方法内为块级作用域
来源：http://yxf.ydjk.org.cn

Go:   花括号块级作用域
来源：http://ptw.jinghuilouyu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qee.yj202588.top

C#:   块级作用域
来源：http://gkh.wangshuangyany.cn

[C11] 模块导入与导出
来源：http://rxs.xylfe.cn

Py:   from module import func
来源：http://xka.nwbrower.top

PHP:  require "file.php";  或 use App\Service;
来源：http://kgd.haohaochexian.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://jch.ywan-chungtsiang.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mdv.xziqi.cn

Java: import java.util.List;
来源：http://zht.cashguo.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tkr.sxryk.cn

Ruby: require "json"; require_relative "./util"
来源：http://uuw.jianghu66.top

C#:   using System.Text;
来源：http://iuk.meibo888.top

[C12] 立即执行函数 IIFE
来源：http://yyl.hywenlv.cn

Py:   (lambda: print("run"))()
来源：http://cod.yuanzhike.top

PHP:  (function () { echo "run"; })();
来源：http://lil.xuanzx.com

JS:   (() => { console.log("run"); })();
来源：http://azy.quarkkingdee.top

TS:   (() => { console.log("run"); })();
来源：http://iyq.kuanghao11.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ior.sjlbkw.cn

Go:   func() { fmt.Println("run") }()
来源：http://kcw.hesvh.cn

Ruby: -> { puts "run" }.call
来源：http://yax.aibaodan.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://dki.iojbl.cn

[C13] 类型声明 / 类型注解
来源：http://jnz.gaohongyu789.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mos.hysaishi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gfs.hnqzz.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lta.jianghu66.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gbi.nanxuanxn.top

Java: int add(int a, int b) { return a + b; }
来源：http://jjm.hammf.cn

Go:   func add(a, b int) int
来源：http://qsl.bjfxy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vdi.yvedp.cn

C#:   int Add(int a, int b) => a + b;
来源：http://alo.hcnkem.com

[C14] 泛型函数
来源：http://qul.cashguo.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ezg.kuanghao11.cn

PHP:  // 无泛型
来源：http://khf.tarul.cn

JS:   // 无泛型
来源：http://ivl.jinyuanbaomall.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zih.xuanzx.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qjy.pengpengdd.cyou

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cny.pycfn.com

Ruby: # 无泛型
来源：http://wgp.zhengqikj.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gwc.hesvh.cn

[C15] 解构 / 展开参数
来源：http://gsg.ydzc1.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dwk.yfazqb.com

PHP:  [$a, $b] = $pair;
来源：http://syy.daria6918.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ysz.yanxiufei.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tnw.hywenlv.cn

Java: // 无解构
来源：http://njl.dianchejie.cn

Go:   // 无解构
来源：http://cka.yj20258.top

Ruby: a, b = pair
来源：http://vrh.gzhubu.top

C#:   var (a, b) = pair;
来源：http://nsk.jiagoushi.top

[C16] 函数 / 方法重载
来源：http://row.yj20258.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vsj.feifeiyinyue.top

PHP:  // 无重载
来源：http://ycb.nanxuanxn.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://xuy.ydzc1.top

TS:   // 用联合类型或重载签名声明
来源：http://urr.9152youxi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wnp.xuanzx.com

Go:   // 无重载：用不同函数名
来源：http://onk.52xcode.cn

Ruby: # 无重载：靠动态参数
来源：http://fgh.sysykeji.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://klo.hnxiangtu.top

================================================================================
来源：http://lwm.sjlbkw.cn

D. 数组 / 列表 / 集合
来源：http://plp.ivvv.top

================================================================================
来源：http://kvk.kuanghao11.cn

[D01] 创建数组 / 列表
来源：http://xrk.gaohongyu789.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://smb.gzhubu.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dpw.aibaodan.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://onm.aibaodan.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vox.jqgufenzy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kzs.cdnleiting.top

Go:   arr := []int{1, 2, 3}
来源：http://nrw.vqdsnc.cn

Ruby: arr = [1, 2, 3]
来源：http://pto.svipenyu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ayj.hammf.cn

[D02] 追加元素到末尾
来源：http://auo.shanyushiyangkeji.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gxx.xingfuxueyuan.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kvc.mhx1999.top

JS:   arr.push(4);
来源：http://zgr.xuetiantiany.cn

TS:   arr.push(4);
来源：http://apa.hongshengwenyu.top

Java: list.add(4);
来源：http://qvg.vqdsnc.cn

Go:   arr = append(arr, 4)
来源：http://uyk.guannengcc.top

Ruby: arr << 4; arr.push(5)
来源：http://wsu.zhijiandao.cn

C#:   list.Add(4);
来源：http://vjm.316326.xyz

[D03] 在指定位置插入元素
来源：http://mbs.nanxinkj.top

Py:   arr.insert(0, 0)
来源：http://ppi.zhongyouzk.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mjv.fanxiaobao.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://euh.cheryme.top

TS:   arr.splice(0, 0, 0);
来源：http://ika.tanke756.top

Java: list.add(0, 0);
来源：http://mrc.birdmap.top

Go:   arr = append([]int{0}, arr...)
来源：http://hoz.bjfxy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ehq.xylfe.cn

C#:   list.Insert(0, 0);
来源：http://yrp.jinghuilouyu.cn

[D04] 删除元素
来源：http://ftl.tarul.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ocp.dianchejie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tpc.sweek.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bpr.316326.xyz

TS:   arr.splice(0, 1);
来源：http://wwq.jinghuilouyu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://aot.chenzaomai.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ymz.xingfuxueyuan.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jsy.ydjk.org.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tps.vqdsnc.cn

[D05] 访问与修改元素
来源：http://hkw.vehdjk.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kkn.hcnkem.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kqw.jlsjyb.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lpt.pycfn.com

TS:   arr[0]; arr.at(-1);
来源：http://xbs.snrcjt.cn

Java: list.get(0); list.set(0, 9);
来源：http://xrs.dashuyun.cn

Go:   arr[0]; arr[0] = 9
来源：http://aai.kuanghao11.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qbe.dashuyun.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gho.hongshengwenyu.top

[D06] 数组长度
来源：http://srr.haohaochexian.top

Py:   len(arr)
来源：http://hmz.sweek.top

PHP:  count($arr);
来源：http://dqn.gotoacloud.top

JS:   arr.length
来源：http://mhp.cdnleiting.top

TS:   arr.length
来源：http://sjf.cqqwz.cn

Java: list.size();
来源：http://qzf.guannengcc.top

Go:   len(arr)
来源：http://ygi.tianlin.xyz

Ruby: arr.length; arr.size
来源：http://whn.bbcook.cn

C#:   list.Count;
来源：http://vjj.guannengcc.top

[D07] 切片 / 取子数组
来源：http://lxm.zhaomingkeji.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hqv.quarkkingdee.top

PHP:  array_slice($arr, 1, 3);
来源：http://crf.chenzaomai.com

JS:   arr.slice(1, 4);
来源：http://okn.aibaodan.cn

TS:   arr.slice(1, 4);
来源：http://hdp.tarul.cn

Java: list.subList(1, 4);
来源：http://aey.ehwqpu.com

Go:   arr[1:4]
来源：http://qdk.xziqi.cn

Ruby: arr[1, 3]
来源：http://xfp.gogol.net.cn

C#:   list.GetRange(1, 3);
来源：http://mzi.c1oappe.top

[D08] 合并两个数组
来源：http://svs.hongshengwenyu.top

Py:   a + b;  a.extend(b)
来源：http://yer.xuanzx.com

PHP:  array_merge($a, $b);
来源：http://uyg.jinyuanbaomall.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://rps.cucudq.cn

TS:   [...a, ...b];
来源：http://czt.yanxiufei.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vlw.pycfn.com

Go:   append(a, b...)
来源：http://rfz.xylfe.cn

Ruby: a + b;  a.concat(b)
来源：http://dlj.daria6918.cn

C#:   a.Concat(b).ToList()
来源：http://cok.c1oappe.top

[D09] 排序（升序）
来源：http://ore.316326.xyz

Py:   sorted(arr);  arr.sort()
来源：http://pee.gogol.net.cn

PHP:  sort($arr);
来源：http://vvs.cdnleiting.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vzs.nanxuanxn.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://edq.bbcook.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yie.guowangkeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vmc.hfpthk.cn

Ruby: arr.sort
来源：http://mxs.zhixingplan.top

C#:   list.Sort();
来源：http://nml.pycfn.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://fes.jyoumei.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wxw.xuetiantiany.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pmx.gotoacloud.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fap.uphjek.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xxu.quarkkingdee.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bzw.316326.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wwo.zdqjudy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gpk.jianghu66.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ima.316326.xyz

[D11] 反转数组
来源：http://pkc.bbcook.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zbo.jinqigufen.top

PHP:  array_reverse($arr);
来源：http://vzw.yanxiufei.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hsb.tian-w.cn

TS:   [...arr].reverse();
来源：http://suk.0kj1m.cn

Java: Collections.reverse(list);
来源：http://ers.gotoacloud.top

Go:   slices.Reverse(arr)
来源：http://jvr.vqdsnc.cn

Ruby: arr.reverse
来源：http://uxh.ivvv.top

C#:   list.Reverse();
来源：http://qlj.yuanzhike.top

[D12] 查找元素下标
来源：http://xai.c1oappe.top

Py:   arr.index(x);  x in arr
来源：http://slu.snrcjt.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fkm.jqgufenzy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yke.yuanzhike.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lrs.9152youxi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tfq.shuidangran.top

Go:   slices.Index(arr, x)
来源：http://ulg.zhongyouzk.top

Ruby: arr.index(x)
来源：http://fvv.meibo888.top

C#:   list.IndexOf(x);
来源：http://spu.hnqzz.top

[D13] 过滤（保留满足条件的）
来源：http://uog.fzhhl.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xzp.chenjidiqi.icu

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jkf.tian-w.cn

JS:   arr.filter(x => x > 3)
来源：http://ydz.iojbl.cn

TS:   arr.filter(x => x > 3)
来源：http://xfd.gaohongyu789.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jsg.yvedp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dvh.fzhhl.top

Ruby: arr.select { |x| x > 3 }
来源：http://hlh.gogol.net.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bjb.hcnkem.com

[D14] 映射转换（每个元素变形）
来源：http://cuq.ppjwa.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://goc.aibaodan.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ses.andypj.xyz

JS:   arr.map(x => x * 2)
来源：http://nnu.jinghuilouyu.cn

TS:   arr.map(x => x * 2)
来源：http://cjn.yj20258888.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://qym.yongpay.top

Go:   // 手写循环
来源：http://pgs.yueranfly.top

Ruby: arr.map { |x| x * 2 }
来源：http://ncb.xylfe.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://gqs.daxiang520.top

[D15] 去重
来源：http://zsz.xingfuxueyuan.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qnq.guowangkeji.top

PHP:  array_unique($arr);
来源：http://vtg.vehdjk.com

JS:   [...new Set(arr)]
来源：http://jxo.haohaochexian.top

TS:   [...new Set(arr)]
来源：http://xkf.dianchejie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jaj.jinghuilouyu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://jvw.xuanzx.com

Ruby: arr.uniq
来源：http://pqs.havefunace.top

C#:   list.Distinct().ToList()
来源：http://npn.fengsongda.top

[D16] 求和与平均值
来源：http://idb.aizwys.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gcp.daxiang520.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fnr.sufxvd.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lwg.xylfe.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://txk.zhijiandao.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pfz.yfazqb.com

Go:   // 手写循环累加
来源：http://yes.yueranfly.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xtb.jiagoushi.top

C#:   list.Sum();  list.Average()
来源：http://jjk.gaohongyu789.top

[D17] 最大值与最小值
来源：http://nbw.zhiwuduotai.top

Py:   max(arr);  min(arr)
来源：http://uwo.zhengqikj.top

PHP:  max($arr);  min($arr);
来源：http://lcz.tian-w.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jfp.birdmap.top

TS:   Math.max(...arr);
来源：http://eoy.jqgfzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://zsm.9152youxi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://coo.tarul.cn

Ruby: arr.max;  arr.min
来源：http://tmz.xuanzx.com

C#:   list.Max();  list.Min()
来源：http://rrx.cashguo.top

[D18] 扁平化嵌套数组
来源：http://yfz.hcnkem.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fuc.fehbvm.com

PHP:  array_merge(...$nested);
来源：http://yaa.nwbrower.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dms.0kj1m.cn

TS:   nested.flat();
来源：http://urk.zhoulong.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://psn.cashguo.top

Go:   // 手写双层循环
来源：http://boc.shuidangran.top

Ruby: nested.flatten
来源：http://rjs.gaohongyu789.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://vee.fzhhl.top

[D19] 按字段分组
来源：http://kma.yfazqb.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yxu.dashuyun.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://avf.ywan-chungtsiang.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jsv.ppjwa.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://umv.ydzc1.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pea.aizwys.cn

Go:   // 手写 map[string][]T
来源：http://cnf.yvedp.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ydf.guannengcc.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rxk.jlsjyb.cn

[D20] 统计每个元素出现次数
来源：http://bro.wangshuangyany.cn

Py:   Counter(arr)
来源：http://zhu.tian-w.cn

PHP:  array_count_values($arr);
来源：http://yzh.jinyuanbaomall.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yrk.nanxuanxn.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vwr.xylfe.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xtz.vqdsnc.cn

Go:   // 手写 map[T]int
来源：http://wbm.jinyuanbaomall.cn


<!-- 参考信息 -->