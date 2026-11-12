代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://suu.ybcxt.top

C#:   arr.Select(s => s.ToUpper())
来源：http://dgu.tarul.cn

[C08] 闭包
来源：http://gyz.sjlbkw.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tik.hnxiangtu.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ppj.xingfuxueyuan.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fkq.xinyue.icu

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rkd.jyoumei.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hoz.cucudq.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wnz.tarul.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ude.sweek.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bvi.zhongyouzk.top

[C09] 递归
来源：http://jxx.guannengcc.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jue.tian-w.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kaa.jqgfzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ueo.jiagoushi.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ptn.yvedp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fcz.yvedp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tmn.bbcook.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kxu.jinghuilouyu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nmq.yongpay.top

[C10] 变量作用域
来源：http://ltz.jianghu66.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nui.andypj.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ipm.jqgfzy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rtk.cashguo.top

TS:   同 JS
来源：http://zey.ybcxt.top

Java: 方法内为块级作用域
来源：http://plk.ydzc1.top

Go:   花括号块级作用域
来源：http://uqi.hcnkem.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://igp.sweek.top

C#:   块级作用域
来源：http://ejb.zhaomingkeji.xyz

[C11] 模块导入与导出
来源：http://oej.snrcjt.cn

Py:   from module import func
来源：http://hlk.jqgufenzy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://azr.chenjidiqi.icu

JS:   export default function f() {};  import f from "./m.js";
来源：http://eof.kuanghao11.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nxq.zhijiandao.cn

Java: import java.util.List;
来源：http://kct.ybcxt.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fvg.hnqzz.top

Ruby: require "json"; require_relative "./util"
来源：http://hhc.yuanzhike.top

C#:   using System.Text;
来源：http://nej.mhx1999.top

[C12] 立即执行函数 IIFE
来源：http://qpq.fehbvm.com

Py:   (lambda: print("run"))()
来源：http://ebt.zycfv.cn

PHP:  (function () { echo "run"; })();
来源：http://niu.yfazqb.com

JS:   (() => { console.log("run"); })();
来源：http://fmd.vehdjk.com

TS:   (() => { console.log("run"); })();
来源：http://iut.havefunace.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jrh.xinyue.icu

Go:   func() { fmt.Println("run") }()
来源：http://lqf.yj202588.top

Ruby: -> { puts "run" }.call
来源：http://xno.uphjek.com

C#:   // 无 IIFE：用静态构造函数
来源：http://nfe.cheryme.top

[C13] 类型声明 / 类型注解
来源：http://hbr.xingfuxueyuan.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ivg.smart0.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uel.vehdjk.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qmc.zhixingplan.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nfs.jqgfzy.top

Java: int add(int a, int b) { return a + b; }
来源：http://yee.nanxuanxn.top

Go:   func add(a, b int) int
来源：http://xpj.sweek.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://doi.guannengcc.top

C#:   int Add(int a, int b) => a + b;
来源：http://zxg.jiagoushi.top

[C14] 泛型函数
来源：http://lhp.zhengqikj.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tva.daria6918.cn

PHP:  // 无泛型
来源：http://qgo.xingfuxueyuan.xyz

JS:   // 无泛型
来源：http://iub.ywan-chungtsiang.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pku.svipenyu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://duh.gogol.net.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://iue.jinqigfzy.top

Ruby: # 无泛型
来源：http://ufh.ybcxt.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wfi.zdbjq.cn

[C15] 解构 / 展开参数
来源：http://cus.redwolf501.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nxb.feifeiyinyue.top

PHP:  [$a, $b] = $pair;
来源：http://zvz.zdbjq.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bca.shanyushiyangtech.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rbh.hnxiangtu.top

Java: // 无解构
来源：http://cwq.hywenlv.cn

Go:   // 无解构
来源：http://jre.jiagoushi.top

Ruby: a, b = pair
来源：http://sfd.hysaishi.cn

C#:   var (a, b) = pair;
来源：http://waz.xuetiantiany.cn

[C16] 函数 / 方法重载
来源：http://ctf.yvedp.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://usl.jqgfzy.top

PHP:  // 无重载
来源：http://bfp.shuidangran.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://seo.tianlin.xyz

TS:   // 用联合类型或重载签名声明
来源：http://roy.gogol.net.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ncx.sjlbkw.cn

Go:   // 无重载：用不同函数名
来源：http://cvo.gzhubu.top

Ruby: # 无重载：靠动态参数
来源：http://lcm.yueranfly.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://wkk.gogol.net.cn

================================================================================
来源：http://rwj.cheryme.top

D. 数组 / 列表 / 集合
来源：http://oak.jyoumei.cn

================================================================================
来源：http://xvu.ydjk.org.cn

[D01] 创建数组 / 列表
来源：http://cbh.birdmap.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://lbm.zhixingplan.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ysb.chenzaomai.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wxt.sxryk.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://nnx.nanxinkj.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vtd.andypj.xyz

Go:   arr := []int{1, 2, 3}
来源：http://yuc.vehdjk.com

Ruby: arr = [1, 2, 3]
来源：http://kxk.hesvh.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tdg.yonumen.top

[D02] 追加元素到末尾
来源：http://puv.shangyingyoupin.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ovj.nanxinkj.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ido.chenlongwang.top

JS:   arr.push(4);
来源：http://its.epnwcf.com

TS:   arr.push(4);
来源：http://muh.hammf.cn

Java: list.add(4);
来源：http://kqk.jyoumei.cn

Go:   arr = append(arr, 4)
来源：http://rfo.ydjk.org.cn

Ruby: arr << 4; arr.push(5)
来源：http://nmj.gotoacloud.top

C#:   list.Add(4);
来源：http://dpf.xziqi.cn

[D03] 在指定位置插入元素
来源：http://syy.sjlbkw.cn

Py:   arr.insert(0, 0)
来源：http://bvl.hcnkem.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xjb.ywan-chungtsiang.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mem.feifeiyinyue.top

TS:   arr.splice(0, 0, 0);
来源：http://smu.dashuyun.cn

Java: list.add(0, 0);
来源：http://aan.tian-w.cn

Go:   arr = append([]int{0}, arr...)
来源：http://sim.ywan-chungtsiang.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://prf.dashuyun.cn

C#:   list.Insert(0, 0);
来源：http://rrf.tianlin.xyz

[D04] 删除元素
来源：http://ity.bjfxy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rcg.xylfe.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://krx.xuanzx.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zpp.yongpay.top

TS:   arr.splice(0, 1);
来源：http://wpw.snrcjt.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fwk.smart0.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://swx.andypj.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ilm.hongshengwenyu.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lyd.yueranfly.top

[D05] 访问与修改元素
来源：http://fmr.quarkkingdee.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://moh.yj20258.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sow.shangyingyoupin.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lit.xylfe.cn

TS:   arr[0]; arr.at(-1);
来源：http://ill.fktsv.cn

Java: list.get(0); list.set(0, 9);
来源：http://bkf.ehwqpu.com

Go:   arr[0]; arr[0] = 9
来源：http://nvs.cheryme.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yrx.ehwqpu.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pqj.gzhubu.top

[D06] 数组长度
来源：http://tem.jqgufenzy.top

Py:   len(arr)
来源：http://uwm.chenzaomai.com

PHP:  count($arr);
来源：http://ely.yuanzhike.top

JS:   arr.length
来源：http://bpw.hfpthk.cn

TS:   arr.length
来源：http://yrz.hfpthk.cn

Java: list.size();
来源：http://aji.hfpthk.cn

Go:   len(arr)
来源：http://yog.xuanzx.com

Ruby: arr.length; arr.size
来源：http://uza.jinqigufen.top

C#:   list.Count;
来源：http://fch.yuanzhike.top

[D07] 切片 / 取子数组
来源：http://bfi.xziqi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wog.birdmap.top

PHP:  array_slice($arr, 1, 3);
来源：http://hvy.daxiang520.top

JS:   arr.slice(1, 4);
来源：http://eei.xingfuxueyuan.xyz

TS:   arr.slice(1, 4);
来源：http://kdf.shanyushiyangtech.top

Java: list.subList(1, 4);
来源：http://hzz.zhijiandao.cn

Go:   arr[1:4]
来源：http://owq.316326.xyz

Ruby: arr[1, 3]
来源：http://ehg.jinyuanbaomall.cn

C#:   list.GetRange(1, 3);
来源：http://def.zhengqikj.top

[D08] 合并两个数组
来源：http://aly.bbcook.cn

Py:   a + b;  a.extend(b)
来源：http://hko.jyoumei.cn

PHP:  array_merge($a, $b);
来源：http://hfn.hammf.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://lwf.zhiwuduotai.top

TS:   [...a, ...b];
来源：http://vgl.nwbrower.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zbi.jqgufenzy.top

Go:   append(a, b...)
来源：http://cdo.tian-w.cn

Ruby: a + b;  a.concat(b)
来源：http://lzs.bjfxy.top

C#:   a.Concat(b).ToList()
来源：http://rub.yangfankeji.com

[D09] 排序（升序）
来源：http://hqx.tianlin.xyz

Py:   sorted(arr);  arr.sort()
来源：http://bwa.hammf.cn

PHP:  sort($arr);
来源：http://jyw.yonumen.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sun.tian-w.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gom.pengpengdd.cyou

Java: Collections.sort(list);  list.sort(null);
来源：http://qmk.tanke756.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xll.jinyuanbaomall.cn

Ruby: arr.sort
来源：http://tvl.xylfe.cn

C#:   list.Sort();
来源：http://jdu.yj202588.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://uvq.ivvv.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jij.ywan-chungtsiang.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dhm.aibaodan.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sjn.shzxlz.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://evq.shzxlz.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mvn.havefunace.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mdv.jqgufenzy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mgu.xuetiantiany.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gsu.zhijiandao.cn

[D11] 反转数组
来源：http://hgn.hnxiangtu.top

Py:   arr[::-1];  arr.reverse()
来源：http://dma.hnqzz.top

PHP:  array_reverse($arr);
来源：http://ojh.xziqi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hzn.yvedp.cn

TS:   [...arr].reverse();
来源：http://irb.iojbl.cn

Java: Collections.reverse(list);
来源：http://bng.0kj1m.cn

Go:   slices.Reverse(arr)
来源：http://sho.aizwys.cn

Ruby: arr.reverse
来源：http://pfh.pengpengdd.cyou

C#:   list.Reverse();
来源：http://aea.tianlin.xyz

[D12] 查找元素下标
来源：http://mcm.jqgufenzy.top

Py:   arr.index(x);  x in arr
来源：http://mnp.zdbjq.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lmt.jiagoushi.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ifg.haohaochexian.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qlo.zhongyouzk.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yxg.cqqwz.cn

Go:   slices.Index(arr, x)
来源：http://jpf.zhengqikj.top

Ruby: arr.index(x)
来源：http://usi.dianchejie.cn

C#:   list.IndexOf(x);
来源：http://ypr.aizwys.cn

[D13] 过滤（保留满足条件的）
来源：http://iio.hesvh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zzo.vqdsnc.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ypu.yuanzhike.top

JS:   arr.filter(x => x > 3)
来源：http://anf.tian-w.cn

TS:   arr.filter(x => x > 3)
来源：http://tql.daxiang520.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ikr.iojbl.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ubs.hfpthk.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ntx.jinghuilouyu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gjb.guannengcc.top

[D14] 映射转换（每个元素变形）
来源：http://zwv.tanke756.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fja.c1oappe.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pgk.jqgufenzy.top

JS:   arr.map(x => x * 2)
来源：http://drn.iojbl.cn

TS:   arr.map(x => x * 2)
来源：http://nfd.yj202588.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://mcr.jyoumei.cn

Go:   // 手写循环
来源：http://hjj.hcnkem.com

Ruby: arr.map { |x| x * 2 }
来源：http://gcf.fzhhl.top

C#:   list.Select(x => x * 2).ToList()
来源：http://fuq.hcnkem.com

[D15] 去重
来源：http://wte.fanxiaobao.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yxx.yongpay.top

PHP:  array_unique($arr);
来源：http://xzy.jqgfzy.top

JS:   [...new Set(arr)]
来源：http://gbw.aizwys.cn

TS:   [...new Set(arr)]
来源：http://vmb.smart0.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zxl.fengsongda.top

Go:   // 用 map[T]struct{} 手写
来源：http://bqr.yueranfly.top

Ruby: arr.uniq
来源：http://aju.shuidangran.top

C#:   list.Distinct().ToList()
来源：http://zrx.daxiang520.top

[D16] 求和与平均值
来源：http://uts.gaohongyu789.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vsr.chenzaomai.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://avt.zhoulong.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tkl.shanyushiyangtech.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vta.chenlongwang.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fdi.dashuyun.cn

Go:   // 手写循环累加
来源：http://lzp.chenzaomai.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ply.wangshuangyany.cn

C#:   list.Sum();  list.Average()
来源：http://fmj.bjfxy.top

[D17] 最大值与最小值
来源：http://bpq.shuidangran.top

Py:   max(arr);  min(arr)
来源：http://cih.haohaochexian.top

PHP:  max($arr);  min($arr);
来源：http://pqn.hongshengwenyu.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://awj.zhaomingkeji.xyz

TS:   Math.max(...arr);
来源：http://prw.sxryk.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://kaf.daria6918.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fru.dianchejie.cn

Ruby: arr.max;  arr.min
来源：http://bqd.zycfv.cn

C#:   list.Max();  list.Min()
来源：http://mqx.9152youxi.cn

[D18] 扁平化嵌套数组
来源：http://mjm.nanxuanxn.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xio.zhiwuduotai.top

PHP:  array_merge(...$nested);
来源：http://ngo.jinqigfzy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://opq.jyoumei.cn

TS:   nested.flat();
来源：http://muu.ydzc1.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://eqz.hesvh.cn

Go:   // 手写双层循环
来源：http://gaz.jiagoushi.top

Ruby: nested.flatten
来源：http://spt.yanxiufei.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://avf.shanyushiyangtech.top

[D19] 按字段分组
来源：http://iyo.yvedp.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://elz.gzhubu.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dxg.ybcxt.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qdo.hongshengwenyu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://cln.haohaochexian.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dmo.yanxiufei.cn

Go:   // 手写 map[string][]T
来源：http://iad.bbcook.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rje.yj20258.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://htw.hfpthk.cn

[D20] 统计每个元素出现次数
来源：http://qoj.fanxiaobao.xyz

Py:   Counter(arr)
来源：http://ssw.yj20258888.top

PHP:  array_count_values($arr);
来源：http://nfj.yj20258.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://swz.yangfankeji.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bcy.bjfxy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xbj.yfazqb.com

Go:   // 手写 map[T]int
来源：http://juk.aizwys.cn

Ruby: arr.tally
来源：http://ccx.zhoulong.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ahx.snrcjt.cn

[D21] 判断是否包含某元素
来源：http://vjp.hnqzz.top

Py:   x in arr
来源：http://lzh.pengpengdd.cyou

PHP:  in_array($x, $arr, true);
来源：http://vsw.jianghu66.top

JS:   arr.includes(x)
来源：http://hmy.hammf.cn

TS:   arr.includes(x)
来源：http://pmq.vqdsnc.cn

Java: list.contains(x)
来源：http://llv.shanyushiyangkeji.top

Go:   slices.Contains(arr, x)
来源：http://qsx.ehwqpu.com

Ruby: arr.include?(x)
来源：http://hvw.yj202588.top

C#:   list.Contains(x)
来源：http://rpo.jinqigufen.top

[D22] 复制数组（避免共享引用）
来源：http://lkt.hongshengwenyu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wta.yj20258888.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cfb.yueranfly.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uhv.jlsjyb.cn

TS:   [...arr];
来源：http://crd.kuanghao11.cn

Java: new ArrayList<>(list);
来源：http://hrn.jinghuilouyu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vgu.sxryk.cn

Ruby: arr.dup;  arr.clone
来源：http://nsq.shanyushiyangtech.top

C#:   new List<int>(list);
来源：http://vgy.vehdjk.com

[D23] reduce 累积计算
来源：http://nyx.iojbl.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hnb.xziqi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jsz.birdmap.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hsa.ydzc1.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dhr.yanxiufei.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hvd.zhijiandao.cn

Go:   // 手写循环
来源：http://leq.ehwqpu.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cgr.gzhubu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://szy.zhengqikj.top

[D24] 字典 / Map 基本操作
来源：http://wrm.shuidangran.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mpb.iojbl.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://glx.xinyue.icu

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mbe.ehwqpu.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fbw.shangyingyoupin.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vet.hfpthk.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sey.chenjidiqi.icu


<!-- 参考信息 -->