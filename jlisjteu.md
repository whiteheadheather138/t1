代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xxg.redwolf501.top

TS:   arr.map(String)
来源：http://bqo.yongpay.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dzn.nanxuanxn.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ewr.aizwys.cn

Ruby: arr.map(&:upcase)
来源：http://xbu.ehwqpu.com

C#:   arr.Select(s => s.ToUpper())
来源：http://qwi.yvedp.cn

[C08] 闭包
来源：http://zzo.dashuyun.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gnb.vehdjk.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jny.tarul.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yze.sysykeji.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gbv.fengsongda.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yrk.yonumen.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gem.jinqigfzy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://stp.sxryk.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lwh.hammf.cn

[C09] 递归
来源：http://ybc.xingfuxueyuan.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://axc.cashguo.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bsk.xuanzx.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nlo.zycfv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sop.yangfankeji.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vba.ydzc1.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pgb.dashuyun.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pmr.quarkkingdee.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dmf.yonumen.top

[C10] 变量作用域
来源：http://uqa.sysykeji.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vjr.sxryk.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bkb.ehwqpu.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ckz.bjfxy.top

TS:   同 JS
来源：http://vau.yangfankeji.com

Java: 方法内为块级作用域
来源：http://fbz.yfazqb.com

Go:   花括号块级作用域
来源：http://nkz.jiagoushi.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vky.zhixingplan.top

C#:   块级作用域
来源：http://eyc.sxryk.cn

[C11] 模块导入与导出
来源：http://rqd.daria6918.cn

Py:   from module import func
来源：http://bdc.uphjek.com

PHP:  require "file.php";  或 use App\Service;
来源：http://fhd.daria6918.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kfg.xuetiantiany.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xvm.tian-w.cn

Java: import java.util.List;
来源：http://jud.yfazqb.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xkd.zhongyouzk.top

Ruby: require "json"; require_relative "./util"
来源：http://kjo.gogol.net.cn

C#:   using System.Text;
来源：http://wwz.yongpay.top

[C12] 立即执行函数 IIFE
来源：http://ntr.kuanghao11.cn

Py:   (lambda: print("run"))()
来源：http://jrb.nwbrower.top

PHP:  (function () { echo "run"; })();
来源：http://yns.chenzaomai.com

JS:   (() => { console.log("run"); })();
来源：http://mdw.wangdashe.top

TS:   (() => { console.log("run"); })();
来源：http://xjl.iojbl.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qgy.daxiang520.top

Go:   func() { fmt.Println("run") }()
来源：http://xlb.chenzaomai.com

Ruby: -> { puts "run" }.call
来源：http://shi.cucudq.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://kjo.meibo888.top

[C13] 类型声明 / 类型注解
来源：http://llm.zycfv.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gsd.hnxiangtu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eca.pycfn.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mpz.ydjk.org.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qar.jyoumei.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dzc.hammf.cn

Go:   func add(a, b int) int
来源：http://wek.pengpengdd.cyou

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hwy.epnwcf.com

C#:   int Add(int a, int b) => a + b;
来源：http://eun.hfpthk.cn

[C14] 泛型函数
来源：http://tre.hywenlv.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vxp.zhijiandao.cn

PHP:  // 无泛型
来源：http://kum.shangyingyoupin.top

JS:   // 无泛型
来源：http://gaq.chenzaomai.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kys.cucudq.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wyw.hcnkem.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jnv.snrcjt.cn

Ruby: # 无泛型
来源：http://rff.hesvh.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hik.fktsv.cn

[C15] 解构 / 展开参数
来源：http://fzf.guowangkeji.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rwb.cheryme.top

PHP:  [$a, $b] = $pair;
来源：http://fua.chenzaomai.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://omo.hongshengwenyu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ryi.nanxuanxn.top

Java: // 无解构
来源：http://qnz.ywan-chungtsiang.top

Go:   // 无解构
来源：http://xpc.tarul.cn

Ruby: a, b = pair
来源：http://dwm.hongshengwenyu.top

C#:   var (a, b) = pair;
来源：http://yyt.shanyushiyangkeji.top

[C16] 函数 / 方法重载
来源：http://mkj.gogol.net.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gxl.shanyushiyangkeji.top

PHP:  // 无重载
来源：http://omc.gzhubu.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://zxm.yuxming.cn

TS:   // 用联合类型或重载签名声明
来源：http://huf.ehwqpu.com

Java: void f(int a) {}  void f(String a) {}
来源：http://qvf.ydjk.org.cn

Go:   // 无重载：用不同函数名
来源：http://nim.tianlin.xyz

Ruby: # 无重载：靠动态参数
来源：http://aid.gogol.net.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mlr.jinghuilouyu.cn

================================================================================
来源：http://ehm.hammf.cn

D. 数组 / 列表 / 集合
来源：http://kua.tian-w.cn

================================================================================
来源：http://wqj.tian-w.cn

[D01] 创建数组 / 列表
来源：http://wkk.ehwqpu.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://wcs.tian-w.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fmq.cqqwz.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hxc.ywan-chungtsiang.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://dsw.hesvh.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zyp.fanxiaobao.xyz

Go:   arr := []int{1, 2, 3}
来源：http://dos.jlsjyb.cn

Ruby: arr = [1, 2, 3]
来源：http://vdc.uphjek.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cvd.dashuyun.cn

[D02] 追加元素到末尾
来源：http://oge.jinyuanbaomall.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zyo.yvedp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jxc.jianghu66.top

JS:   arr.push(4);
来源：http://utj.hcnkem.com

TS:   arr.push(4);
来源：http://uot.jqgufenzy.top

Java: list.add(4);
来源：http://wsu.yj20258.top

Go:   arr = append(arr, 4)
来源：http://teh.cqqwz.cn

Ruby: arr << 4; arr.push(5)
来源：http://svf.mhx1999.top

C#:   list.Add(4);
来源：http://uee.gotoacloud.top

[D03] 在指定位置插入元素
来源：http://xoc.c1oappe.top

Py:   arr.insert(0, 0)
来源：http://ybr.xylfe.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uoc.shanyushiyangkeji.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://scl.9152youxi.cn

TS:   arr.splice(0, 0, 0);
来源：http://hyu.hnxiangtu.top

Java: list.add(0, 0);
来源：http://bio.jinqigfzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://ywh.wangshuangyany.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dnb.tianlin.xyz

C#:   list.Insert(0, 0);
来源：http://ysq.jinghuilouyu.cn

[D04] 删除元素
来源：http://wir.zycfv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xsy.birdmap.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bvg.uphjek.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bzs.bbcook.cn

TS:   arr.splice(0, 1);
来源：http://szd.gzhubu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mqf.yueranfly.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qmf.hfpthk.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://drm.aizwys.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sub.c1oappe.top

[D05] 访问与修改元素
来源：http://oyc.dashuyun.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xth.andypj.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tus.tian-w.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://aic.sxryk.cn

TS:   arr[0]; arr.at(-1);
来源：http://anr.sweek.top

Java: list.get(0); list.set(0, 9);
来源：http://sot.zhoulong.xyz

Go:   arr[0]; arr[0] = 9
来源：http://qvf.kuanghao11.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fqd.shuidangran.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rde.yuxming.cn

[D06] 数组长度
来源：http://mpu.gaohongyu789.top

Py:   len(arr)
来源：http://kag.ydjk.org.cn

PHP:  count($arr);
来源：http://uxs.jqgufenzy.top

JS:   arr.length
来源：http://dhh.guowangkeji.top

TS:   arr.length
来源：http://mpk.yangfankeji.com

Java: list.size();
来源：http://sqe.bbcook.cn

Go:   len(arr)
来源：http://pdy.guannengcc.top

Ruby: arr.length; arr.size
来源：http://usd.gogol.net.cn

C#:   list.Count;
来源：http://iig.meibo888.top

[D07] 切片 / 取子数组
来源：http://nor.haohaochexian.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://trm.hesvh.cn

PHP:  array_slice($arr, 1, 3);
来源：http://elb.zhoulong.xyz

JS:   arr.slice(1, 4);
来源：http://pub.jyoumei.cn

TS:   arr.slice(1, 4);
来源：http://zmz.chenjidiqi.icu

Java: list.subList(1, 4);
来源：http://icg.xinyue.icu

Go:   arr[1:4]
来源：http://jgt.0kj1m.cn

Ruby: arr[1, 3]
来源：http://blf.jinqigfzy.top

C#:   list.GetRange(1, 3);
来源：http://jpg.jqgufenzy.top

[D08] 合并两个数组
来源：http://ymg.yanxiufei.cn

Py:   a + b;  a.extend(b)
来源：http://ywr.zdqjudy.top

PHP:  array_merge($a, $b);
来源：http://itc.jiagoushi.top

JS:   [...a, ...b];  a.concat(b);
来源：http://pap.fanxiaobao.xyz

TS:   [...a, ...b];
来源：http://uck.chenzaomai.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xhn.meibo888.top

Go:   append(a, b...)
来源：http://oso.cashguo.top

Ruby: a + b;  a.concat(b)
来源：http://dqr.yonumen.top

C#:   a.Concat(b).ToList()
来源：http://ysq.fzhhl.top

[D09] 排序（升序）
来源：http://ate.cdnleiting.top

Py:   sorted(arr);  arr.sort()
来源：http://afg.nwbrower.top

PHP:  sort($arr);
来源：http://lkg.sweek.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://trh.chenlongwang.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://czl.9152youxi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://git.sysykeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wni.havefunace.top

Ruby: arr.sort
来源：http://rba.cucudq.cn

C#:   list.Sort();
来源：http://kak.feifeiyinyue.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://stx.52xcode.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zrc.bjfxy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cdl.chenlongwang.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://uoz.zhongyouzk.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oye.sysykeji.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://iyy.jqgufenzy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ptb.c1oappe.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zes.chenzaomai.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://raz.yangfankeji.com

[D11] 反转数组
来源：http://prt.cashguo.top

Py:   arr[::-1];  arr.reverse()
来源：http://cgy.zhixingplan.top

PHP:  array_reverse($arr);
来源：http://ewy.tian-w.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://oha.yongpay.top

TS:   [...arr].reverse();
来源：http://qvd.epnwcf.com

Java: Collections.reverse(list);
来源：http://wta.sjlbkw.cn

Go:   slices.Reverse(arr)
来源：http://dys.yangfankeji.com

Ruby: arr.reverse
来源：http://gka.chenjidiqi.icu

C#:   list.Reverse();
来源：http://lcu.hammf.cn

[D12] 查找元素下标
来源：http://xcn.gogol.net.cn

Py:   arr.index(x);  x in arr
来源：http://yif.ywan-chungtsiang.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hcv.jlsjyb.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cwp.52xcode.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vdu.jinyuanbaomall.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ecq.gzhubu.top

Go:   slices.Index(arr, x)
来源：http://evw.tian-w.cn

Ruby: arr.index(x)
来源：http://ubk.xuetiantiany.cn

C#:   list.IndexOf(x);
来源：http://kfg.guannengcc.top

[D13] 过滤（保留满足条件的）
来源：http://zqh.yfazqb.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zgt.hammf.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://udo.xuanzx.com

JS:   arr.filter(x => x > 3)
来源：http://bvj.vqdsnc.cn

TS:   arr.filter(x => x > 3)
来源：http://lcs.hcnkem.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ujo.gaohongyu789.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vfy.feifeiyinyue.top

Ruby: arr.select { |x| x > 3 }
来源：http://bjr.quarkkingdee.top

C#:   list.Where(x => x > 3).ToList()
来源：http://goc.redwolf501.top

[D14] 映射转换（每个元素变形）
来源：http://kwo.zhoulong.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xna.tianlin.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rtp.zdqjudy.top

JS:   arr.map(x => x * 2)
来源：http://nuu.zhoulong.xyz

TS:   arr.map(x => x * 2)
来源：http://jro.hfpthk.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vky.gaohongyu789.top

Go:   // 手写循环
来源：http://igk.zycfv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dmy.hywenlv.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ssc.snrcjt.cn

[D15] 去重
来源：http://tbe.havefunace.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gfi.nanxinkj.top

PHP:  array_unique($arr);
来源：http://aus.ivvv.top

JS:   [...new Set(arr)]
来源：http://uln.sysykeji.top

TS:   [...new Set(arr)]
来源：http://imz.yuanzhike.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yrj.yanxiufei.cn

Go:   // 用 map[T]struct{} 手写
来源：http://gso.shanyushiyangtech.top

Ruby: arr.uniq
来源：http://ems.sysykeji.top

C#:   list.Distinct().ToList()
来源：http://vcp.tanke756.top

[D16] 求和与平均值
来源：http://ndi.mhx1999.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sjy.yongpay.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hkq.tarul.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cre.dashuyun.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://eon.hammf.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hyt.shanyushiyangtech.top

Go:   // 手写循环累加
来源：http://yzh.cashguo.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tyb.jinghuilouyu.cn

C#:   list.Sum();  list.Average()
来源：http://fhu.shzxlz.cn

[D17] 最大值与最小值
来源：http://vjr.jinqigfzy.top

Py:   max(arr);  min(arr)
来源：http://pjl.fehbvm.com

PHP:  max($arr);  min($arr);
来源：http://wsa.ehwqpu.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://eyl.tian-w.cn

TS:   Math.max(...arr);
来源：http://tmm.pycfn.com

Java: Collections.max(list);  Collections.min(list);
来源：http://fwk.yuanzhike.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tzk.tian-w.cn

Ruby: arr.max;  arr.min
来源：http://jcf.sweek.top

C#:   list.Max();  list.Min()
来源：http://wvp.jqgufenzy.top

[D18] 扁平化嵌套数组
来源：http://yhl.andypj.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wip.fzhhl.top

PHP:  array_merge(...$nested);
来源：http://dmg.xziqi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://msn.fanxiaobao.xyz

TS:   nested.flat();
来源：http://rax.hesvh.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://evy.cashguo.top

Go:   // 手写双层循环
来源：http://uzp.uphjek.com

Ruby: nested.flatten
来源：http://tsu.birdmap.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://xgg.chenzaomai.com

[D19] 按字段分组
来源：http://xky.yj20258888.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://muk.daxiang520.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tzj.svipenyu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kcd.fzhhl.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://fse.pengpengdd.cyou

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tmx.tarul.cn

Go:   // 手写 map[string][]T
来源：http://eua.zdbjq.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://dgp.yuxming.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dlw.wangshuangyany.cn

[D20] 统计每个元素出现次数
来源：http://rbt.shanyushiyangtech.top

Py:   Counter(arr)
来源：http://cqd.zhaomingkeji.xyz

PHP:  array_count_values($arr);
来源：http://pii.yvedp.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://imj.havefunace.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hei.ivvv.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ijr.wangshuangyany.cn

Go:   // 手写 map[T]int
来源：http://igr.ywan-chungtsiang.top

Ruby: arr.tally
来源：http://rvg.cqqwz.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://brf.chenjidiqi.icu

[D21] 判断是否包含某元素
来源：http://tzo.chenlongwang.top

Py:   x in arr
来源：http://dtw.svipenyu.cn

PHP:  in_array($x, $arr, true);
来源：http://tgx.9152youxi.cn

JS:   arr.includes(x)
来源：http://ree.fanxiaobao.xyz

TS:   arr.includes(x)
来源：http://opw.cqqwz.cn

Java: list.contains(x)
来源：http://jsi.shangyingyoupin.top

Go:   slices.Contains(arr, x)
来源：http://dzd.quarkkingdee.top

Ruby: arr.include?(x)
来源：http://sxz.jinghuilouyu.cn

C#:   list.Contains(x)
来源：http://wez.fktsv.cn

[D22] 复制数组（避免共享引用）
来源：http://unv.cucudq.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ckp.zhoulong.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mef.0kj1m.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jyq.pengpengdd.cyou

TS:   [...arr];
来源：http://njf.hnxiangtu.top

Java: new ArrayList<>(list);
来源：http://gna.gzhubu.top

Go:   copied := append([]int(nil), arr...)
来源：http://dhl.svipenyu.cn

Ruby: arr.dup;  arr.clone
来源：http://qxe.mhx1999.top

C#:   new List<int>(list);
来源：http://arv.xinyue.icu

[D23] reduce 累积计算
来源：http://lao.aizwys.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://duj.xinyue.icu

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zag.yfazqb.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vkh.hnxiangtu.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wou.hongshengwenyu.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://pjg.xuetiantiany.cn

Go:   // 手写循环
来源：http://zro.vqdsnc.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mos.52xcode.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rel.hnqzz.top

[D24] 字典 / Map 基本操作
来源：http://jjl.fengsongda.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xxb.zhijiandao.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://oen.dianchejie.cn


<!-- 参考信息 -->