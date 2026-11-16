代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://eua.cashguo.top

C#:   arr.Select(s => s.ToUpper())
来源：http://dma.nanxuanxn.top

[C08] 闭包
来源：http://ltc.ydjk.org.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://quq.tianlin.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://exw.epnwcf.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://inx.havefunace.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://htt.xylfe.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://aet.daria6918.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lic.jqgfzy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lzf.guannengcc.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ogs.yj20258.top

[C09] 递归
来源：http://jnq.hcnkem.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ifh.nwbrower.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://flo.vehdjk.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zlk.sweek.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cqn.zhoulong.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ehs.c1oappe.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xvg.hongshengwenyu.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wii.hywenlv.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wqt.sysykeji.top

[C10] 变量作用域
来源：http://pzb.epnwcf.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ioe.fehbvm.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dmy.fzhhl.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://olm.ehwqpu.com

TS:   同 JS
来源：http://nus.yvedp.cn

Java: 方法内为块级作用域
来源：http://iiq.tarul.cn

Go:   花括号块级作用域
来源：http://vjf.daxiang520.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vaa.vqdsnc.cn

C#:   块级作用域
来源：http://ole.bjfxy.top

[C11] 模块导入与导出
来源：http://xlk.guowangkeji.top

Py:   from module import func
来源：http://zhv.fengsongda.top

PHP:  require "file.php";  或 use App\Service;
来源：http://dpm.svipenyu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hpf.hfpthk.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ppm.guannengcc.top

Java: import java.util.List;
来源：http://ssi.fzhhl.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qnl.zycfv.cn

Ruby: require "json"; require_relative "./util"
来源：http://nhw.tianlin.xyz

C#:   using System.Text;
来源：http://bbq.zhaomingkeji.xyz

[C12] 立即执行函数 IIFE
来源：http://ido.cqqwz.cn

Py:   (lambda: print("run"))()
来源：http://fhj.sweek.top

PHP:  (function () { echo "run"; })();
来源：http://rza.zycfv.cn

JS:   (() => { console.log("run"); })();
来源：http://tah.andypj.xyz

TS:   (() => { console.log("run"); })();
来源：http://rfh.gzhubu.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lef.bbcook.cn

Go:   func() { fmt.Println("run") }()
来源：http://xcj.birdmap.top

Ruby: -> { puts "run" }.call
来源：http://rrw.mhx1999.top

C#:   // 无 IIFE：用静态构造函数
来源：http://uhm.nwbrower.top

[C13] 类型声明 / 类型注解
来源：http://qzv.hongshengwenyu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://okc.yonumen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pjh.pycfn.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wzn.kuanghao11.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ngq.yuxming.cn

Java: int add(int a, int b) { return a + b; }
来源：http://bst.ybcxt.top

Go:   func add(a, b int) int
来源：http://mjo.c1oappe.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yrf.jinqigfzy.top

C#:   int Add(int a, int b) => a + b;
来源：http://kuz.yuanzhike.top

[C14] 泛型函数
来源：http://gbe.zhengqikj.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uvl.yangfankeji.com

PHP:  // 无泛型
来源：http://qts.yangfankeji.com

JS:   // 无泛型
来源：http://cos.uphjek.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://txk.wangshuangyany.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kbc.xingfuxueyuan.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gwy.daria6918.cn

Ruby: # 无泛型
来源：http://tnj.ydzc1.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lvq.bjfxy.top

[C15] 解构 / 展开参数
来源：http://vyj.redwolf501.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dje.jinqigufen.top

PHP:  [$a, $b] = $pair;
来源：http://dhd.bjfxy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xek.vqdsnc.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://krj.meibo888.top

Java: // 无解构
来源：http://lds.yangfankeji.com

Go:   // 无解构
来源：http://qyc.yj202588.top

Ruby: a, b = pair
来源：http://brr.wangdashe.top

C#:   var (a, b) = pair;
来源：http://pgn.bjfxy.top

[C16] 函数 / 方法重载
来源：http://lip.vqdsnc.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xjh.jyoumei.cn

PHP:  // 无重载
来源：http://pxg.fehbvm.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://aoo.ppjwa.cn

TS:   // 用联合类型或重载签名声明
来源：http://qvw.zhijiandao.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://scb.havefunace.top

Go:   // 无重载：用不同函数名
来源：http://xca.shzxlz.cn

Ruby: # 无重载：靠动态参数
来源：http://vmy.zdqjudy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://siq.xuanzx.com

================================================================================
来源：http://kdk.ywan-chungtsiang.top

D. 数组 / 列表 / 集合
来源：http://skf.shuidangran.top

================================================================================
来源：http://nbe.chenjidiqi.icu

[D01] 创建数组 / 列表
来源：http://cxc.vqdsnc.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ulx.yongpay.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yfm.zhongyouzk.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://txs.jiagoushi.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://mjv.dianchejie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nyn.cheryme.top

Go:   arr := []int{1, 2, 3}
来源：http://hxh.hammf.cn

Ruby: arr = [1, 2, 3]
来源：http://gbf.xylfe.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ouf.guowangkeji.top

[D02] 追加元素到末尾
来源：http://nlv.xuetiantiany.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ppy.pycfn.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ccm.iojbl.cn

JS:   arr.push(4);
来源：http://fvs.sufxvd.cn

TS:   arr.push(4);
来源：http://ilv.ppjwa.cn

Java: list.add(4);
来源：http://azq.hnqzz.top

Go:   arr = append(arr, 4)
来源：http://nwt.aibaodan.cn

Ruby: arr << 4; arr.push(5)
来源：http://ycc.shuidangran.top

C#:   list.Add(4);
来源：http://ydx.zdbjq.cn

[D03] 在指定位置插入元素
来源：http://kqp.zdbjq.cn

Py:   arr.insert(0, 0)
来源：http://tbn.c1oappe.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://atz.meibo888.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ioh.ydzc1.top

TS:   arr.splice(0, 0, 0);
来源：http://twj.jinqigufen.top

Java: list.add(0, 0);
来源：http://qrq.smart0.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://jxz.jyoumei.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cks.yfazqb.com

C#:   list.Insert(0, 0);
来源：http://xsi.sufxvd.cn

[D04] 删除元素
来源：http://evw.gotoacloud.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wyn.xuanzx.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gox.hysaishi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://glh.hesvh.cn

TS:   arr.splice(0, 1);
来源：http://nno.jlsjyb.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yjo.jinqigufen.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tsp.sufxvd.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lcq.haohaochexian.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mxe.gaohongyu789.top

[D05] 访问与修改元素
来源：http://hwa.xuanzx.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pmk.shzxlz.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ute.jianghu66.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://oyr.zycfv.cn

TS:   arr[0]; arr.at(-1);
来源：http://jmf.yvedp.cn

Java: list.get(0); list.set(0, 9);
来源：http://sba.shangyingyoupin.top

Go:   arr[0]; arr[0] = 9
来源：http://esz.tanke756.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zok.yj20258.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vjn.yj20258888.top

[D06] 数组长度
来源：http://qmz.snrcjt.cn

Py:   len(arr)
来源：http://bib.hysaishi.cn

PHP:  count($arr);
来源：http://eka.jianghu66.top

JS:   arr.length
来源：http://peq.tian-w.cn

TS:   arr.length
来源：http://nbn.hysaishi.cn

Java: list.size();
来源：http://rcb.yj20258888.top

Go:   len(arr)
来源：http://osd.quarkkingdee.top

Ruby: arr.length; arr.size
来源：http://fgr.hnxiangtu.top

C#:   list.Count;
来源：http://idu.jinqigufen.top

[D07] 切片 / 取子数组
来源：http://cfy.cqqwz.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kvy.shuidangran.top

PHP:  array_slice($arr, 1, 3);
来源：http://qhd.aizwys.cn

JS:   arr.slice(1, 4);
来源：http://edp.shanyushiyangkeji.top

TS:   arr.slice(1, 4);
来源：http://jen.havefunace.top

Java: list.subList(1, 4);
来源：http://jro.yj20258888.top

Go:   arr[1:4]
来源：http://kis.yuxming.cn

Ruby: arr[1, 3]
来源：http://kys.fktsv.cn

C#:   list.GetRange(1, 3);
来源：http://bom.jianghu66.top

[D08] 合并两个数组
来源：http://wwc.zhijiandao.cn

Py:   a + b;  a.extend(b)
来源：http://vwi.yvedp.cn

PHP:  array_merge($a, $b);
来源：http://gcs.ppjwa.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zar.fktsv.cn

TS:   [...a, ...b];
来源：http://hyv.jinqigufen.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tng.jiagoushi.top

Go:   append(a, b...)
来源：http://djx.yanxiufei.cn

Ruby: a + b;  a.concat(b)
来源：http://yfg.hammf.cn

C#:   a.Concat(b).ToList()
来源：http://ssu.dashuyun.cn

[D09] 排序（升序）
来源：http://ogh.chenjidiqi.icu

Py:   sorted(arr);  arr.sort()
来源：http://xtd.gaohongyu789.top

PHP:  sort($arr);
来源：http://rjo.zycfv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://snc.jqgufenzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://hfj.redwolf501.top

Java: Collections.sort(list);  list.sort(null);
来源：http://juf.shanyushiyangkeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pfc.iojbl.cn

Ruby: arr.sort
来源：http://fgw.yvedp.cn

C#:   list.Sort();
来源：http://ivu.gaohongyu789.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://wtu.jianghu66.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pkp.tarul.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pkx.aizwys.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ccx.sjlbkw.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jde.iojbl.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://voc.aizwys.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ksz.jianghu66.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://plr.316326.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zsh.cashguo.top

[D11] 反转数组
来源：http://cyd.zhiwuduotai.top

Py:   arr[::-1];  arr.reverse()
来源：http://ruc.aizwys.cn

PHP:  array_reverse($arr);
来源：http://qlt.yanxiufei.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gmj.hcnkem.com

TS:   [...arr].reverse();
来源：http://pgt.316326.xyz

Java: Collections.reverse(list);
来源：http://qqm.ivvv.top

Go:   slices.Reverse(arr)
来源：http://tfx.xuanzx.com

Ruby: arr.reverse
来源：http://xnv.xylfe.cn

C#:   list.Reverse();
来源：http://acj.hysaishi.cn

[D12] 查找元素下标
来源：http://aej.zhaomingkeji.xyz

Py:   arr.index(x);  x in arr
来源：http://miw.jiagoushi.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mop.sysykeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vrt.chenzaomai.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ovi.ydzc1.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://odj.hnqzz.top

Go:   slices.Index(arr, x)
来源：http://ktr.yonumen.top

Ruby: arr.index(x)
来源：http://csf.zhijiandao.cn

C#:   list.IndexOf(x);
来源：http://srz.0kj1m.cn

[D13] 过滤（保留满足条件的）
来源：http://hst.cdnleiting.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vcd.bbcook.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kcs.xuanzx.com

JS:   arr.filter(x => x > 3)
来源：http://ohc.sxryk.cn

TS:   arr.filter(x => x > 3)
来源：http://wxk.hongshengwenyu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mxj.jlsjyb.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://iol.yj20258888.top

Ruby: arr.select { |x| x > 3 }
来源：http://kks.nanxuanxn.top

C#:   list.Where(x => x > 3).ToList()
来源：http://kyr.hysaishi.cn

[D14] 映射转换（每个元素变形）
来源：http://dal.sjlbkw.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vgp.jyoumei.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://awb.yj20258.top

JS:   arr.map(x => x * 2)
来源：http://nnp.yanxiufei.cn

TS:   arr.map(x => x * 2)
来源：http://iho.aizwys.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jcv.zhijiandao.cn

Go:   // 手写循环
来源：http://nvv.aizwys.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qzn.zhoulong.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://smh.xziqi.cn

[D15] 去重
来源：http://uyi.shanyushiyangkeji.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wrz.uphjek.com

PHP:  array_unique($arr);
来源：http://iii.hammf.cn

JS:   [...new Set(arr)]
来源：http://slo.jinghuilouyu.cn

TS:   [...new Set(arr)]
来源：http://yeu.yfazqb.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uwo.cashguo.top

Go:   // 用 map[T]struct{} 手写
来源：http://jxx.jinqigfzy.top

Ruby: arr.uniq
来源：http://sqt.yonumen.top

C#:   list.Distinct().ToList()
来源：http://iwg.sjlbkw.cn

[D16] 求和与平均值
来源：http://ifu.zhaomingkeji.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jzh.sufxvd.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qtl.yanxiufei.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lwo.hesvh.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jrb.gzhubu.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rda.birdmap.top

Go:   // 手写循环累加
来源：http://rfh.yj20258888.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://aph.zhongyouzk.top

C#:   list.Sum();  list.Average()
来源：http://dsf.yj20258888.top

[D17] 最大值与最小值
来源：http://rpa.jinqigfzy.top

Py:   max(arr);  min(arr)
来源：http://etj.jinghuilouyu.cn

PHP:  max($arr);  min($arr);
来源：http://wxe.fanxiaobao.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vuo.dianchejie.cn

TS:   Math.max(...arr);
来源：http://sdd.316326.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://jus.zhijiandao.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://irm.chenzaomai.com

Ruby: arr.max;  arr.min
来源：http://mfp.zhoulong.xyz

C#:   list.Max();  list.Min()
来源：http://vli.quarkkingdee.top

[D18] 扁平化嵌套数组
来源：http://ozj.hfpthk.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bpz.pycfn.com

PHP:  array_merge(...$nested);
来源：http://bsf.andypj.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pff.yj20258888.top

TS:   nested.flat();
来源：http://nez.jlsjyb.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kdx.zycfv.cn

Go:   // 手写双层循环
来源：http://kxq.chenlongwang.top

Ruby: nested.flatten
来源：http://xbc.zhongyouzk.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://jni.yuanzhike.top

[D19] 按字段分组
来源：http://gfw.yvedp.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bkg.havefunace.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://sbt.svipenyu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tzg.yj20258.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://izq.fehbvm.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://umf.xuanzx.com

Go:   // 手写 map[string][]T
来源：http://wzt.feifeiyinyue.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://uhx.c1oappe.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mil.hongshengwenyu.top

[D20] 统计每个元素出现次数
来源：http://tgx.fengsongda.top

Py:   Counter(arr)
来源：http://vmm.yj202588.top

PHP:  array_count_values($arr);
来源：http://jnj.nanxinkj.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qij.316326.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tfx.sjlbkw.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nkt.ydzc1.top

Go:   // 手写 map[T]int
来源：http://mwg.316326.xyz

Ruby: arr.tally
来源：http://flz.cqqwz.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://oxu.daxiang520.top

[D21] 判断是否包含某元素
来源：http://dnk.zdbjq.cn

Py:   x in arr
来源：http://vcc.yj20258.top

PHP:  in_array($x, $arr, true);
来源：http://qsh.sysykeji.top

JS:   arr.includes(x)
来源：http://afq.jyoumei.cn

TS:   arr.includes(x)
来源：http://nqr.wangdashe.top

Java: list.contains(x)
来源：http://dub.aibaodan.cn

Go:   slices.Contains(arr, x)
来源：http://jxj.zhijiandao.cn

Ruby: arr.include?(x)
来源：http://pkt.gotoacloud.top

C#:   list.Contains(x)
来源：http://lur.guowangkeji.top

[D22] 复制数组（避免共享引用）
来源：http://iks.zhongyouzk.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wpq.jinqigfzy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gtw.zdbjq.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ksk.jyoumei.cn

TS:   [...arr];
来源：http://ukj.kuanghao11.cn

Java: new ArrayList<>(list);
来源：http://pak.cheryme.top

Go:   copied := append([]int(nil), arr...)
来源：http://nsh.yfazqb.com

Ruby: arr.dup;  arr.clone
来源：http://lsk.jiagoushi.top

C#:   new List<int>(list);
来源：http://czx.yuxming.cn

[D23] reduce 累积计算
来源：http://mws.yj20258888.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cjf.fzhhl.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://oax.fengsongda.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zab.yj20258888.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://chu.zhaomingkeji.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://esv.tanke756.top

Go:   // 手写循环
来源：http://vvb.cheryme.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rvq.hysaishi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mgt.fzhhl.top

[D24] 字典 / Map 基本操作
来源：http://yio.xuetiantiany.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ppo.meibo888.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wbq.ydjk.org.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://izb.zhaomingkeji.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fak.zhiwuduotai.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kxa.gotoacloud.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rcc.ydjk.org.cn


<!-- 参考信息 -->