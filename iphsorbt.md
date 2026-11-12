代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://pjy.jqgufenzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://olv.dashuyun.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dbf.xinyue.icu

Ruby: square = ->(x) { x * x }
来源：http://kxh.jinqigufen.top

C#:   Func<int, int> square = x => x * x;
来源：http://zjb.dashuyun.cn

[C07] 把函数作为参数传入
来源：http://ayl.kuanghao11.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fup.xziqi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://sai.gzhubu.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pvf.haohaochexian.top

TS:   arr.map(String)
来源：http://buv.aibaodan.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kjf.gotoacloud.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ppr.zhengqikj.top

Ruby: arr.map(&:upcase)
来源：http://etc.hfpthk.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://eih.vehdjk.com

[C08] 闭包
来源：http://imy.sjlbkw.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nzj.xylfe.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://scl.birdmap.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cfr.zdbjq.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.bbcook.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zib.sysykeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vvm.fanxiaobao.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://omq.zycfv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ybu.fktsv.cn

[C09] 递归
来源：http://ebd.zdbjq.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ipa.yuanzhike.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kmm.zdbjq.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cuz.ydjk.org.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ucf.dianchejie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ztt.mhx1999.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gln.jinghuilouyu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cni.yj20258888.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tap.shzxlz.cn

[C10] 变量作用域
来源：http://eip.shzxlz.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yle.snrcjt.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fcq.snrcjt.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kyo.cheryme.top

TS:   同 JS
来源：http://ykd.sysykeji.top

Java: 方法内为块级作用域
来源：http://thh.ydzc1.top

Go:   花括号块级作用域
来源：http://wun.52xcode.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://usn.zhijiandao.cn

C#:   块级作用域
来源：http://svk.jiagoushi.top

[C11] 模块导入与导出
来源：http://jki.guowangkeji.top

Py:   from module import func
来源：http://nql.dianchejie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ilv.kuanghao11.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jlq.ehwqpu.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ttf.wangdashe.top

Java: import java.util.List;
来源：http://uzo.ywan-chungtsiang.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wbo.vehdjk.com

Ruby: require "json"; require_relative "./util"
来源：http://zhy.jqgufenzy.top

C#:   using System.Text;
来源：http://gcx.hfpthk.cn

[C12] 立即执行函数 IIFE
来源：http://hhp.snrcjt.cn

Py:   (lambda: print("run"))()
来源：http://jvi.9152youxi.cn

PHP:  (function () { echo "run"; })();
来源：http://omm.chenjidiqi.icu

JS:   (() => { console.log("run"); })();
来源：http://wju.vehdjk.com

TS:   (() => { console.log("run"); })();
来源：http://vcm.fktsv.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jgr.hnqzz.top

Go:   func() { fmt.Println("run") }()
来源：http://jtl.zhiwuduotai.top

Ruby: -> { puts "run" }.call
来源：http://vrq.zdqjudy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://crr.yueranfly.top

[C13] 类型声明 / 类型注解
来源：http://tvu.bbcook.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://oco.tian-w.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ucz.cheryme.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jfk.ehwqpu.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hdm.birdmap.top

Java: int add(int a, int b) { return a + b; }
来源：http://ktq.jinghuilouyu.cn

Go:   func add(a, b int) int
来源：http://qpj.wangdashe.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vsf.meibo888.top

C#:   int Add(int a, int b) => a + b;
来源：http://mhp.nanxinkj.top

[C14] 泛型函数
来源：http://fmf.shanyushiyangkeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wov.jlsjyb.cn

PHP:  // 无泛型
来源：http://tgb.jinqigfzy.top

JS:   // 无泛型
来源：http://dio.zhijiandao.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kvp.gogol.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://neg.tarul.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cgl.sxryk.cn

Ruby: # 无泛型
来源：http://pkg.yvedp.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ukm.feifeiyinyue.top

[C15] 解构 / 展开参数
来源：http://pgc.sjlbkw.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://roi.yj20258.top

PHP:  [$a, $b] = $pair;
来源：http://wiz.zdqjudy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zhf.hongshengwenyu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nsl.52xcode.cn

Java: // 无解构
来源：http://coe.feifeiyinyue.top

Go:   // 无解构
来源：http://eyp.guowangkeji.top

Ruby: a, b = pair
来源：http://wgc.cashguo.top

C#:   var (a, b) = pair;
来源：http://fub.guowangkeji.top

[C16] 函数 / 方法重载
来源：http://msi.guowangkeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fhy.zycfv.cn

PHP:  // 无重载
来源：http://reb.jinyuanbaomall.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bje.9152youxi.cn

TS:   // 用联合类型或重载签名声明
来源：http://pts.hongshengwenyu.top

Java: void f(int a) {}  void f(String a) {}
来源：http://dvz.bbcook.cn

Go:   // 无重载：用不同函数名
来源：http://dnx.shanyushiyangkeji.top

Ruby: # 无重载：靠动态参数
来源：http://xdc.gaohongyu789.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://zgp.sjlbkw.cn

================================================================================
来源：http://bzl.yj202588.top

D. 数组 / 列表 / 集合
来源：http://glm.sysykeji.top

================================================================================
来源：http://kdj.tanke756.top

[D01] 创建数组 / 列表
来源：http://uzm.sxryk.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qdw.chenzaomai.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uim.cheryme.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nto.hcnkem.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://uxk.xylfe.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ngt.yj202588.top

Go:   arr := []int{1, 2, 3}
来源：http://ojw.shanyushiyangkeji.top

Ruby: arr = [1, 2, 3]
来源：http://pxe.shanyushiyangtech.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hnl.nanxuanxn.top

[D02] 追加元素到末尾
来源：http://mec.cashguo.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nsr.jiagoushi.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cqr.xuetiantiany.cn

JS:   arr.push(4);
来源：http://ycg.hcnkem.com

TS:   arr.push(4);
来源：http://wba.shanyushiyangtech.top

Java: list.add(4);
来源：http://qub.yfazqb.com

Go:   arr = append(arr, 4)
来源：http://zxk.shanyushiyangtech.top

Ruby: arr << 4; arr.push(5)
来源：http://gag.cdnleiting.top

C#:   list.Add(4);
来源：http://sbh.cdnleiting.top

[D03] 在指定位置插入元素
来源：http://mvo.yangfankeji.com

Py:   arr.insert(0, 0)
来源：http://vir.hesvh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://czd.zdbjq.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wyu.zhijiandao.cn

TS:   arr.splice(0, 0, 0);
来源：http://ufx.zhixingplan.top

Java: list.add(0, 0);
来源：http://hsl.c1oappe.top

Go:   arr = append([]int{0}, arr...)
来源：http://vyt.zhixingplan.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xst.ivvv.top

C#:   list.Insert(0, 0);
来源：http://brw.daxiang520.top

[D04] 删除元素
来源：http://cfc.aibaodan.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jyt.zycfv.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dig.shanyushiyangkeji.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xnw.yfazqb.com

TS:   arr.splice(0, 1);
来源：http://lka.jinghuilouyu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dvs.xziqi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zxr.zdbjq.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gcn.mhx1999.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ioe.nwbrower.top

[D05] 访问与修改元素
来源：http://dgn.sjlbkw.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mbn.zhongyouzk.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ylv.zdbjq.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ayk.yj202588.top

TS:   arr[0]; arr.at(-1);
来源：http://etr.tianlin.xyz

Java: list.get(0); list.set(0, 9);
来源：http://ebd.vehdjk.com

Go:   arr[0]; arr[0] = 9
来源：http://jvn.dashuyun.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kls.0kj1m.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hak.sxryk.cn

[D06] 数组长度
来源：http://oic.cucudq.cn

Py:   len(arr)
来源：http://rkg.yanxiufei.cn

PHP:  count($arr);
来源：http://uhv.chenlongwang.top

JS:   arr.length
来源：http://ggv.ctjpmb.com

TS:   arr.length
来源：http://wzt.zdqjudy.top

Java: list.size();
来源：http://biw.zdqjudy.top

Go:   len(arr)
来源：http://xjk.andypj.xyz

Ruby: arr.length; arr.size
来源：http://vfo.yangfankeji.com

C#:   list.Count;
来源：http://yvi.cqqwz.cn

[D07] 切片 / 取子数组
来源：http://ojn.yangfankeji.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://anp.shzxlz.cn

PHP:  array_slice($arr, 1, 3);
来源：http://cct.svipenyu.cn

JS:   arr.slice(1, 4);
来源：http://ayy.tarul.cn

TS:   arr.slice(1, 4);
来源：http://abr.pengpengdd.cyou

Java: list.subList(1, 4);
来源：http://tyq.0kj1m.cn

Go:   arr[1:4]
来源：http://xun.xylfe.cn

Ruby: arr[1, 3]
来源：http://ltr.zhoulong.xyz

C#:   list.GetRange(1, 3);
来源：http://coo.bjfxy.top

[D08] 合并两个数组
来源：http://hhv.aibaodan.cn

Py:   a + b;  a.extend(b)
来源：http://zdt.fengsongda.top

PHP:  array_merge($a, $b);
来源：http://drq.fanxiaobao.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://tie.jlsjyb.cn

TS:   [...a, ...b];
来源：http://iou.sysykeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://myy.iojbl.cn

Go:   append(a, b...)
来源：http://fqw.zhiwuduotai.top

Ruby: a + b;  a.concat(b)
来源：http://ljb.shanyushiyangkeji.top

C#:   a.Concat(b).ToList()
来源：http://kim.aibaodan.cn

[D09] 排序（升序）
来源：http://pod.yangfankeji.com

Py:   sorted(arr);  arr.sort()
来源：http://zvb.c1oappe.top

PHP:  sort($arr);
来源：http://tkk.jqgufenzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://udb.jinqigfzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://eob.sysykeji.top

Java: Collections.sort(list);  list.sort(null);
来源：http://pua.zhoulong.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://feq.daria6918.cn

Ruby: arr.sort
来源：http://wrx.dashuyun.cn

C#:   list.Sort();
来源：http://alm.nanxuanxn.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://vmf.chenlongwang.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://evd.zdqjudy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cli.shanyushiyangkeji.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://got.tarul.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rda.aizwys.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bfr.redwolf501.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ddj.mhx1999.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://czk.nanxinkj.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://syq.gotoacloud.top

[D11] 反转数组
来源：http://hhm.kuanghao11.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lch.xylfe.cn

PHP:  array_reverse($arr);
来源：http://wzd.guowangkeji.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vsv.jlsjyb.cn

TS:   [...arr].reverse();
来源：http://wow.xingfuxueyuan.xyz

Java: Collections.reverse(list);
来源：http://eig.sufxvd.cn

Go:   slices.Reverse(arr)
来源：http://aeu.ydzc1.top

Ruby: arr.reverse
来源：http://xzg.hfpthk.cn

C#:   list.Reverse();
来源：http://nxn.ybcxt.top

[D12] 查找元素下标
来源：http://zje.meibo888.top

Py:   arr.index(x);  x in arr
来源：http://udt.dashuyun.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bxa.xylfe.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ybj.yangfankeji.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://suz.nanxuanxn.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tai.yj202588.top

Go:   slices.Index(arr, x)
来源：http://yyq.c1oappe.top

Ruby: arr.index(x)
来源：http://qpx.jiagoushi.top

C#:   list.IndexOf(x);
来源：http://spf.guannengcc.top

[D13] 过滤（保留满足条件的）
来源：http://oie.fengsongda.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://anq.meibo888.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zkd.smart0.xyz

JS:   arr.filter(x => x > 3)
来源：http://hlo.ywan-chungtsiang.top

TS:   arr.filter(x => x > 3)
来源：http://oac.meibo888.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dem.kuanghao11.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rap.zycfv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nda.yfazqb.com

C#:   list.Where(x => x > 3).ToList()
来源：http://vjo.pycfn.com

[D14] 映射转换（每个元素变形）
来源：http://qdb.yj20258.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qvs.jiagoushi.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xzg.52xcode.cn

JS:   arr.map(x => x * 2)
来源：http://izz.ybcxt.top

TS:   arr.map(x => x * 2)
来源：http://yjx.ydjk.org.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://luv.jyoumei.cn

Go:   // 手写循环
来源：http://gfi.chenzaomai.com

Ruby: arr.map { |x| x * 2 }
来源：http://suv.316326.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://kvf.zdqjudy.top

[D15] 去重
来源：http://jhw.tian-w.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hgt.snrcjt.cn

PHP:  array_unique($arr);
来源：http://oys.zdqjudy.top

JS:   [...new Set(arr)]
来源：http://vsr.hnxiangtu.top

TS:   [...new Set(arr)]
来源：http://ozy.jiagoushi.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://iym.guowangkeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://dfn.yuanzhike.top

Ruby: arr.uniq
来源：http://iax.ywan-chungtsiang.top

C#:   list.Distinct().ToList()
来源：http://wzr.dianchejie.cn

[D16] 求和与平均值
来源：http://gka.xziqi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vaa.sweek.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rje.guannengcc.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wnf.fzhhl.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://koz.pengpengdd.cyou

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://crj.chenjidiqi.icu

Go:   // 手写循环累加
来源：http://gzu.yonumen.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hnd.iojbl.cn

C#:   list.Sum();  list.Average()
来源：http://yxh.shuidangran.top

[D17] 最大值与最小值
来源：http://ufq.guannengcc.top

Py:   max(arr);  min(arr)
来源：http://gwi.ctjpmb.com

PHP:  max($arr);  min($arr);
来源：http://oqs.bbcook.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vdl.ydzc1.top

TS:   Math.max(...arr);
来源：http://car.zhijiandao.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rqw.dianchejie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wbf.zhongyouzk.top

Ruby: arr.max;  arr.min
来源：http://sqz.hnxiangtu.top

C#:   list.Max();  list.Min()
来源：http://gmg.fanxiaobao.xyz

[D18] 扁平化嵌套数组
来源：http://qju.zycfv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wcv.dianchejie.cn

PHP:  array_merge(...$nested);
来源：http://iqb.daria6918.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://irf.redwolf501.top

TS:   nested.flat();
来源：http://qnq.shzxlz.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tco.hcnkem.com

Go:   // 手写双层循环
来源：http://kqf.hnxiangtu.top

Ruby: nested.flatten
来源：http://iof.nwbrower.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://nrp.9152youxi.cn

[D19] 按字段分组
来源：http://gwc.fehbvm.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gla.birdmap.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fut.havefunace.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vbx.ctjpmb.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://lfl.chenlongwang.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ecb.zhaomingkeji.xyz

Go:   // 手写 map[string][]T
来源：http://tde.nanxinkj.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://fjl.guowangkeji.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ucm.nanxinkj.top

[D20] 统计每个元素出现次数
来源：http://nug.tanke756.top

Py:   Counter(arr)
来源：http://pui.jianghu66.top

PHP:  array_count_values($arr);
来源：http://twx.epnwcf.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gvs.jqgfzy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oix.hywenlv.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://swc.uphjek.com

Go:   // 手写 map[T]int
来源：http://scx.gogol.net.cn

Ruby: arr.tally
来源：http://hhr.cucudq.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://drz.chenzaomai.com

[D21] 判断是否包含某元素
来源：http://kks.bbcook.cn

Py:   x in arr
来源：http://dts.zhoulong.xyz

PHP:  in_array($x, $arr, true);
来源：http://dfn.yanxiufei.cn

JS:   arr.includes(x)
来源：http://xvc.hcnkem.com

TS:   arr.includes(x)
来源：http://chx.hysaishi.cn

Java: list.contains(x)
来源：http://hor.bbcook.cn

Go:   slices.Contains(arr, x)
来源：http://nxq.uphjek.com

Ruby: arr.include?(x)
来源：http://jdc.xuetiantiany.cn

C#:   list.Contains(x)
来源：http://glv.aibaodan.cn

[D22] 复制数组（避免共享引用）
来源：http://vgp.jinqigfzy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://isb.hammf.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wbq.fengsongda.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yqd.pycfn.com

TS:   [...arr];
来源：http://uxt.yvedp.cn

Java: new ArrayList<>(list);
来源：http://kjn.yangfankeji.com

Go:   copied := append([]int(nil), arr...)
来源：http://tfs.zhongyouzk.top

Ruby: arr.dup;  arr.clone
来源：http://wed.shzxlz.cn

C#:   new List<int>(list);
来源：http://ner.guowangkeji.top

[D23] reduce 累积计算
来源：http://zdg.guowangkeji.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jah.iojbl.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tqb.xuetiantiany.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zux.sufxvd.cn


<!-- 参考信息 -->