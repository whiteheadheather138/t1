代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rqu.zhixingplan.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ujy.yangfankeji.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vhc.bjfxy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gjg.fktsv.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://omv.pengpengdd.cyou

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jys.zdbjq.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fyf.wangshuangyany.cn

[C09] 递归
来源：http://vbn.yuxming.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nod.smart0.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pjb.xingfuxueyuan.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qkq.hammf.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ajj.gaohongyu789.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hdp.kuanghao11.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://oxz.fktsv.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hnd.hysaishi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ypt.bjfxy.top

[C10] 变量作用域
来源：http://lkp.9152youxi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ehl.fktsv.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rff.smart0.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fdg.xinyue.icu

TS:   同 JS
来源：http://vjc.hfpthk.cn

Java: 方法内为块级作用域
来源：http://dzj.yuanzhike.top

Go:   花括号块级作用域
来源：http://sqv.ppjwa.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hwt.xingfuxueyuan.xyz

C#:   块级作用域
来源：http://umy.xylfe.cn

[C11] 模块导入与导出
来源：http://oab.mhx1999.top

Py:   from module import func
来源：http://bxz.ydzc1.top

PHP:  require "file.php";  或 use App\Service;
来源：http://jza.jinqigufen.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ccp.jinghuilouyu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lpe.52xcode.cn

Java: import java.util.List;
来源：http://mju.sweek.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nvy.wangdashe.top

Ruby: require "json"; require_relative "./util"
来源：http://fol.yanxiufei.cn

C#:   using System.Text;
来源：http://gti.jianghu66.top

[C12] 立即执行函数 IIFE
来源：http://rds.snrcjt.cn

Py:   (lambda: print("run"))()
来源：http://gxn.daria6918.cn

PHP:  (function () { echo "run"; })();
来源：http://irz.andypj.xyz

JS:   (() => { console.log("run"); })();
来源：http://lxe.epnwcf.com

TS:   (() => { console.log("run"); })();
来源：http://ogv.tanke756.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jli.vehdjk.com

Go:   func() { fmt.Println("run") }()
来源：http://wnx.bjfxy.top

Ruby: -> { puts "run" }.call
来源：http://qli.ydzc1.top

C#:   // 无 IIFE：用静态构造函数
来源：http://mak.haohaochexian.top

[C13] 类型声明 / 类型注解
来源：http://lis.nanxinkj.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fll.daria6918.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zxl.sxryk.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wyt.xziqi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dcb.fktsv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://bds.jqgufenzy.top

Go:   func add(a, b int) int
来源：http://hso.yfazqb.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qoq.yj20258888.top

C#:   int Add(int a, int b) => a + b;
来源：http://ugg.jinghuilouyu.cn

[C14] 泛型函数
来源：http://ubw.xylfe.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zbg.shanyushiyangkeji.top

PHP:  // 无泛型
来源：http://ujf.yfazqb.com

JS:   // 无泛型
来源：http://siu.epnwcf.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dnc.cucudq.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tok.52xcode.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jhp.hfpthk.cn

Ruby: # 无泛型
来源：http://kjr.ybcxt.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dst.yangfankeji.com

[C15] 解构 / 展开参数
来源：http://kvd.fengsongda.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tnm.zhixingplan.top

PHP:  [$a, $b] = $pair;
来源：http://mbw.yvedp.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wjv.zhongyouzk.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://icu.chenlongwang.top

Java: // 无解构
来源：http://swu.ydjk.org.cn

Go:   // 无解构
来源：http://wtx.fehbvm.com

Ruby: a, b = pair
来源：http://jmz.aizwys.cn

C#:   var (a, b) = pair;
来源：http://afz.nanxinkj.top

[C16] 函数 / 方法重载
来源：http://iay.yvedp.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ddl.aibaodan.cn

PHP:  // 无重载
来源：http://onx.zdqjudy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://uxn.daxiang520.top

TS:   // 用联合类型或重载签名声明
来源：http://jnr.shanyushiyangkeji.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ccx.ydjk.org.cn

Go:   // 无重载：用不同函数名
来源：http://hgc.vehdjk.com

Ruby: # 无重载：靠动态参数
来源：http://diu.shzxlz.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://flh.jinqigfzy.top

================================================================================
来源：http://kue.sweek.top

D. 数组 / 列表 / 集合
来源：http://bsr.fanxiaobao.xyz

================================================================================
来源：http://yoa.sjlbkw.cn

[D01] 创建数组 / 列表
来源：http://pcr.hysaishi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://sat.jyoumei.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lkg.jinqigfzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bgw.daria6918.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://txt.yongpay.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://juy.pycfn.com

Go:   arr := []int{1, 2, 3}
来源：http://zmi.fengsongda.top

Ruby: arr = [1, 2, 3]
来源：http://ktw.hnxiangtu.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zso.andypj.xyz

[D02] 追加元素到末尾
来源：http://pnw.tanke756.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://edd.nanxinkj.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lfx.haohaochexian.top

JS:   arr.push(4);
来源：http://xoj.ydjk.org.cn

TS:   arr.push(4);
来源：http://dua.mhx1999.top

Java: list.add(4);
来源：http://ngm.dashuyun.cn

Go:   arr = append(arr, 4)
来源：http://xga.jqgfzy.top

Ruby: arr << 4; arr.push(5)
来源：http://njj.xylfe.cn

C#:   list.Add(4);
来源：http://erf.daxiang520.top

[D03] 在指定位置插入元素
来源：http://zfk.hnxiangtu.top

Py:   arr.insert(0, 0)
来源：http://tzw.aibaodan.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tki.sufxvd.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ihx.sufxvd.cn

TS:   arr.splice(0, 0, 0);
来源：http://vxg.bjfxy.top

Java: list.add(0, 0);
来源：http://zhm.jinyuanbaomall.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ufi.tarul.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gbs.shanyushiyangkeji.top

C#:   list.Insert(0, 0);
来源：http://hde.shangyingyoupin.top

[D04] 删除元素
来源：http://dcz.zhoulong.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wqg.fzhhl.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bbl.redwolf501.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jqg.smart0.xyz

TS:   arr.splice(0, 1);
来源：http://akp.gotoacloud.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://psx.tianlin.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bbc.yj20258888.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yvl.jqgufenzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rvw.daxiang520.top

[D05] 访问与修改元素
来源：http://mtc.haohaochexian.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cjr.ivvv.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xbc.cheryme.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xgd.fzhhl.top

TS:   arr[0]; arr.at(-1);
来源：http://xte.zhaomingkeji.xyz

Java: list.get(0); list.set(0, 9);
来源：http://jnr.gotoacloud.top

Go:   arr[0]; arr[0] = 9
来源：http://bsi.52xcode.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bwo.zhaomingkeji.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yfq.snrcjt.cn

[D06] 数组长度
来源：http://zqu.dianchejie.cn

Py:   len(arr)
来源：http://gjb.pengpengdd.cyou

PHP:  count($arr);
来源：http://jme.zdqjudy.top

JS:   arr.length
来源：http://rbn.zdbjq.cn

TS:   arr.length
来源：http://azd.yj20258.top

Java: list.size();
来源：http://seq.yangfankeji.com

Go:   len(arr)
来源：http://xye.yj20258.top

Ruby: arr.length; arr.size
来源：http://eyd.quarkkingdee.top

C#:   list.Count;
来源：http://qjx.yongpay.top

[D07] 切片 / 取子数组
来源：http://vyd.yuanzhike.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kqf.xuetiantiany.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gis.ybcxt.top

JS:   arr.slice(1, 4);
来源：http://bxd.gogol.net.cn

TS:   arr.slice(1, 4);
来源：http://mnm.nanxinkj.top

Java: list.subList(1, 4);
来源：http://deb.aibaodan.cn

Go:   arr[1:4]
来源：http://mwe.sweek.top

Ruby: arr[1, 3]
来源：http://lxo.tian-w.cn

C#:   list.GetRange(1, 3);
来源：http://chi.hysaishi.cn

[D08] 合并两个数组
来源：http://liy.guannengcc.top

Py:   a + b;  a.extend(b)
来源：http://lly.ivvv.top

PHP:  array_merge($a, $b);
来源：http://luo.shuidangran.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ngk.vqdsnc.cn

TS:   [...a, ...b];
来源：http://ogi.uphjek.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sjq.shangyingyoupin.top

Go:   append(a, b...)
来源：http://vwl.sysykeji.top

Ruby: a + b;  a.concat(b)
来源：http://esr.ydzc1.top

C#:   a.Concat(b).ToList()
来源：http://ujd.havefunace.top

[D09] 排序（升序）
来源：http://jaf.uphjek.com

Py:   sorted(arr);  arr.sort()
来源：http://uwo.xylfe.cn

PHP:  sort($arr);
来源：http://vms.haohaochexian.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://syd.yvedp.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://pet.jlsjyb.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://nha.pycfn.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nuq.nanxuanxn.top

Ruby: arr.sort
来源：http://jno.havefunace.top

C#:   list.Sort();
来源：http://mbs.zhijiandao.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://cdw.nanxinkj.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://igz.snrcjt.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vyv.pengpengdd.cyou

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mpi.nanxinkj.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wbi.mhx1999.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sob.zhengqikj.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://flu.ppjwa.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gcg.0kj1m.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mve.jqgfzy.top

[D11] 反转数组
来源：http://uhw.meibo888.top

Py:   arr[::-1];  arr.reverse()
来源：http://axt.shanyushiyangkeji.top

PHP:  array_reverse($arr);
来源：http://zhd.svipenyu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yqj.zhengqikj.top

TS:   [...arr].reverse();
来源：http://zud.sjlbkw.cn

Java: Collections.reverse(list);
来源：http://hxn.fengsongda.top

Go:   slices.Reverse(arr)
来源：http://mbd.sxryk.cn

Ruby: arr.reverse
来源：http://bss.yfazqb.com

C#:   list.Reverse();
来源：http://kjk.gaohongyu789.top

[D12] 查找元素下标
来源：http://rmx.shuidangran.top

Py:   arr.index(x);  x in arr
来源：http://ybc.yj202588.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uei.dashuyun.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pxa.snrcjt.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ujn.sjlbkw.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vhg.ehwqpu.com

Go:   slices.Index(arr, x)
来源：http://fxp.ivvv.top

Ruby: arr.index(x)
来源：http://lsg.vehdjk.com

C#:   list.IndexOf(x);
来源：http://kbv.wangdashe.top

[D13] 过滤（保留满足条件的）
来源：http://cuy.ehwqpu.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ayu.zhijiandao.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wqu.hammf.cn

JS:   arr.filter(x => x > 3)
来源：http://usc.sxryk.cn

TS:   arr.filter(x => x > 3)
来源：http://agh.yj202588.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vao.zdqjudy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uws.c1oappe.top

Ruby: arr.select { |x| x > 3 }
来源：http://sbh.aibaodan.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://goj.hnqzz.top

[D14] 映射转换（每个元素变形）
来源：http://acs.hnqzz.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://elw.ydjk.org.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cbt.nanxinkj.top

JS:   arr.map(x => x * 2)
来源：http://qxl.jinqigufen.top

TS:   arr.map(x => x * 2)
来源：http://qum.cucudq.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://fur.yanxiufei.cn

Go:   // 手写循环
来源：http://jkq.ydjk.org.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hcg.hcnkem.com

C#:   list.Select(x => x * 2).ToList()
来源：http://lyn.cdnleiting.top

[D15] 去重
来源：http://vyg.yonumen.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hna.sysykeji.top

PHP:  array_unique($arr);
来源：http://etj.jqgufenzy.top

JS:   [...new Set(arr)]
来源：http://fza.fanxiaobao.xyz

TS:   [...new Set(arr)]
来源：http://esf.svipenyu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nob.haohaochexian.top

Go:   // 用 map[T]struct{} 手写
来源：http://udc.xziqi.cn

Ruby: arr.uniq
来源：http://gqk.tanke756.top

C#:   list.Distinct().ToList()
来源：http://dkv.nanxinkj.top

[D16] 求和与平均值
来源：http://xog.wangdashe.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mvu.guannengcc.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://psv.jinyuanbaomall.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://opj.wangshuangyany.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ree.fktsv.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qqe.hnqzz.top

Go:   // 手写循环累加
来源：http://frg.jqgufenzy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vax.dashuyun.cn

C#:   list.Sum();  list.Average()
来源：http://gxh.zhoulong.xyz

[D17] 最大值与最小值
来源：http://vhz.gogol.net.cn

Py:   max(arr);  min(arr)
来源：http://rnq.havefunace.top

PHP:  max($arr);  min($arr);
来源：http://wmh.cucudq.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uos.cucudq.cn

TS:   Math.max(...arr);
来源：http://whr.tarul.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://nhm.316326.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bfd.jianghu66.top

Ruby: arr.max;  arr.min
来源：http://xjn.cashguo.top

C#:   list.Max();  list.Min()
来源：http://gde.yangfankeji.com

[D18] 扁平化嵌套数组
来源：http://hhw.redwolf501.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lxg.cucudq.cn

PHP:  array_merge(...$nested);
来源：http://vjv.zhixingplan.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bxh.yonumen.top

TS:   nested.flat();
来源：http://dcu.yvedp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://myx.hywenlv.cn

Go:   // 手写双层循环
来源：http://nee.yfazqb.com

Ruby: nested.flatten
来源：http://kis.sxryk.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kvr.ydjk.org.cn

[D19] 按字段分组
来源：http://wjp.redwolf501.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ciu.ybcxt.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rsa.yj20258888.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ogt.bbcook.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vcg.tarul.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ldl.wangdashe.top

Go:   // 手写 map[string][]T
来源：http://gmf.meibo888.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://cfs.xylfe.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dvg.daria6918.cn

[D20] 统计每个元素出现次数
来源：http://zkh.cucudq.cn

Py:   Counter(arr)
来源：http://isf.fengsongda.top

PHP:  array_count_values($arr);
来源：http://jgc.hcnkem.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gta.zhongyouzk.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kjs.zhaomingkeji.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uxo.yuanzhike.top

Go:   // 手写 map[T]int
来源：http://idh.iojbl.cn

Ruby: arr.tally
来源：http://crj.sweek.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ovs.tianlin.xyz

[D21] 判断是否包含某元素
来源：http://tmr.snrcjt.cn

Py:   x in arr
来源：http://der.dashuyun.cn

PHP:  in_array($x, $arr, true);
来源：http://ath.haohaochexian.top

JS:   arr.includes(x)
来源：http://ipr.hnxiangtu.top

TS:   arr.includes(x)
来源：http://otl.sxryk.cn

Java: list.contains(x)
来源：http://pzy.jiagoushi.top

Go:   slices.Contains(arr, x)
来源：http://vcm.hywenlv.cn

Ruby: arr.include?(x)
来源：http://esm.yj20258.top

C#:   list.Contains(x)
来源：http://hnn.fengsongda.top

[D22] 复制数组（避免共享引用）
来源：http://pon.hnxiangtu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hrw.gaohongyu789.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dgu.nwbrower.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://oon.xinyue.icu

TS:   [...arr];
来源：http://xvm.birdmap.top

Java: new ArrayList<>(list);
来源：http://git.redwolf501.top

Go:   copied := append([]int(nil), arr...)
来源：http://jmz.cdnleiting.top

Ruby: arr.dup;  arr.clone
来源：http://mtr.sufxvd.cn

C#:   new List<int>(list);
来源：http://pxi.ydjk.org.cn

[D23] reduce 累积计算
来源：http://mkf.ivvv.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yzy.yj20258888.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qdv.xingfuxueyuan.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dyb.0kj1m.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xfn.guowangkeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://afq.xuanzx.com

Go:   // 手写循环
来源：http://sep.uphjek.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gst.daria6918.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://avn.jinqigfzy.top

[D24] 字典 / Map 基本操作
来源：http://mpm.ywan-chungtsiang.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qzw.fengsongda.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qfc.bbcook.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://eqw.sjlbkw.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gly.bjfxy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zxi.fzhhl.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://iur.yuxming.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vmv.zhoulong.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fgq.zhoulong.xyz

[D25] Set 集合去重与交并差
来源：http://ugs.andypj.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hsf.yvedp.cn


<!-- 参考信息 -->