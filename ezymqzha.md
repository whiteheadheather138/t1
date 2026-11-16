代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yqi.jinqigufen.top

TS:   arr.map(String)
来源：http://jub.xylfe.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pgs.sufxvd.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mdx.mhx1999.top

Ruby: arr.map(&:upcase)
来源：http://vrk.gaohongyu789.top

C#:   arr.Select(s => s.ToUpper())
来源：http://rww.xuanzx.com

[C08] 闭包
来源：http://dxu.zhixingplan.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://diw.sjlbkw.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qgh.bbcook.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hgh.bjfxy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rcr.guannengcc.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pqb.xuetiantiany.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ipe.aizwys.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ctx.hysaishi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hrq.xuanzx.com

[C09] 递归
来源：http://koq.zhongyouzk.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rwk.guowangkeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qnw.hnqzz.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bgk.epnwcf.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://riu.pycfn.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lpm.feifeiyinyue.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gbk.ywan-chungtsiang.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bbu.sjlbkw.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sgt.yvedp.cn

[C10] 变量作用域
来源：http://yli.ydjk.org.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hta.sysykeji.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jpf.haohaochexian.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nwj.sweek.top

TS:   同 JS
来源：http://sqk.ydzc1.top

Java: 方法内为块级作用域
来源：http://oeq.cashguo.top

Go:   花括号块级作用域
来源：http://qzb.jinqigufen.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vit.xuanzx.com

C#:   块级作用域
来源：http://fwd.jianghu66.top

[C11] 模块导入与导出
来源：http://yhe.hnqzz.top

Py:   from module import func
来源：http://fyx.gotoacloud.top

PHP:  require "file.php";  或 use App\Service;
来源：http://mut.hnxiangtu.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://dzy.zdbjq.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dhm.zdqjudy.top

Java: import java.util.List;
来源：http://mfc.sysykeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gql.yvedp.cn

Ruby: require "json"; require_relative "./util"
来源：http://nhq.jqgfzy.top

C#:   using System.Text;
来源：http://lgw.chenzaomai.com

[C12] 立即执行函数 IIFE
来源：http://kxw.zdqjudy.top

Py:   (lambda: print("run"))()
来源：http://uih.haohaochexian.top

PHP:  (function () { echo "run"; })();
来源：http://kqw.ybcxt.top

JS:   (() => { console.log("run"); })();
来源：http://tnk.fktsv.cn

TS:   (() => { console.log("run"); })();
来源：http://aro.xylfe.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wiq.ehwqpu.com

Go:   func() { fmt.Println("run") }()
来源：http://lmj.gzhubu.top

Ruby: -> { puts "run" }.call
来源：http://hnh.sjlbkw.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fyz.cdnleiting.top

[C13] 类型声明 / 类型注解
来源：http://iqb.gzhubu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://omh.feifeiyinyue.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qzq.yuxming.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bzm.aibaodan.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qon.epnwcf.com

Java: int add(int a, int b) { return a + b; }
来源：http://wzc.yuanzhike.top

Go:   func add(a, b int) int
来源：http://fni.snrcjt.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gub.fanxiaobao.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://haf.jinghuilouyu.cn

[C14] 泛型函数
来源：http://aif.ctjpmb.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jib.xuetiantiany.cn

PHP:  // 无泛型
来源：http://jko.yj20258.top

JS:   // 无泛型
来源：http://coz.jinqigufen.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jjt.gogol.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://foo.hesvh.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://amk.gaohongyu789.top

Ruby: # 无泛型
来源：http://ius.smart0.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tyk.daria6918.cn

[C15] 解构 / 展开参数
来源：http://bzj.xziqi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wxx.cdnleiting.top

PHP:  [$a, $b] = $pair;
来源：http://sxa.yanxiufei.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rpb.sufxvd.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ikf.jlsjyb.cn

Java: // 无解构
来源：http://ftu.jlsjyb.cn

Go:   // 无解构
来源：http://fhq.yanxiufei.cn

Ruby: a, b = pair
来源：http://ukm.zhiwuduotai.top

C#:   var (a, b) = pair;
来源：http://hvf.pengpengdd.cyou

[C16] 函数 / 方法重载
来源：http://gfo.0kj1m.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qms.pengpengdd.cyou

PHP:  // 无重载
来源：http://fdu.gzhubu.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://eig.c1oappe.top

TS:   // 用联合类型或重载签名声明
来源：http://obm.svipenyu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dtd.sufxvd.cn

Go:   // 无重载：用不同函数名
来源：http://twm.fengsongda.top

Ruby: # 无重载：靠动态参数
来源：http://cpu.hammf.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://eeo.jlsjyb.cn

================================================================================
来源：http://efh.jqgfzy.top

D. 数组 / 列表 / 集合
来源：http://xmn.zdqjudy.top

================================================================================
来源：http://ivr.pengpengdd.cyou

[D01] 创建数组 / 列表
来源：http://qqp.pengpengdd.cyou

Py:   arr = [1, 2, 3];  empty = []
来源：http://vdq.yuxming.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://aua.yanxiufei.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tjn.daria6918.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://svb.shzxlz.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nmf.shanyushiyangkeji.top

Go:   arr := []int{1, 2, 3}
来源：http://azy.yvedp.cn

Ruby: arr = [1, 2, 3]
来源：http://syx.havefunace.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ofu.jiagoushi.top

[D02] 追加元素到末尾
来源：http://udm.xylfe.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lpx.ydzc1.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bwf.ctjpmb.com

JS:   arr.push(4);
来源：http://bax.tanke756.top

TS:   arr.push(4);
来源：http://era.zhoulong.xyz

Java: list.add(4);
来源：http://tjl.havefunace.top

Go:   arr = append(arr, 4)
来源：http://qum.chenlongwang.top

Ruby: arr << 4; arr.push(5)
来源：http://nkn.yongpay.top

C#:   list.Add(4);
来源：http://ksh.shuidangran.top

[D03] 在指定位置插入元素
来源：http://rdp.aizwys.cn

Py:   arr.insert(0, 0)
来源：http://obn.vqdsnc.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://afh.tian-w.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lzw.chenzaomai.com

TS:   arr.splice(0, 0, 0);
来源：http://jol.yanxiufei.cn

Java: list.add(0, 0);
来源：http://bca.jyoumei.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fii.andypj.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fqu.sufxvd.cn

C#:   list.Insert(0, 0);
来源：http://jjy.meibo888.top

[D04] 删除元素
来源：http://xgi.fktsv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://iow.cucudq.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://iso.ivvv.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dps.0kj1m.cn

TS:   arr.splice(0, 1);
来源：http://elh.hesvh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dyb.jinyuanbaomall.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://czk.hcnkem.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qdr.pycfn.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bym.chenjidiqi.icu

[D05] 访问与修改元素
来源：http://qqq.zhaomingkeji.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rny.uphjek.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vcn.guannengcc.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ido.vqdsnc.cn

TS:   arr[0]; arr.at(-1);
来源：http://gxs.zhaomingkeji.xyz

Java: list.get(0); list.set(0, 9);
来源：http://tkh.daxiang520.top

Go:   arr[0]; arr[0] = 9
来源：http://lrt.zhengqikj.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uav.zhaomingkeji.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jeb.tarul.cn

[D06] 数组长度
来源：http://hbv.cdnleiting.top

Py:   len(arr)
来源：http://qtv.yanxiufei.cn

PHP:  count($arr);
来源：http://znv.xinyue.icu

JS:   arr.length
来源：http://qfk.cheryme.top

TS:   arr.length
来源：http://eho.jqgufenzy.top

Java: list.size();
来源：http://cyt.pycfn.com

Go:   len(arr)
来源：http://ufy.cucudq.cn

Ruby: arr.length; arr.size
来源：http://iko.gzhubu.top

C#:   list.Count;
来源：http://nyh.nwbrower.top

[D07] 切片 / 取子数组
来源：http://yzz.hnqzz.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pdr.hesvh.cn

PHP:  array_slice($arr, 1, 3);
来源：http://mab.ctjpmb.com

JS:   arr.slice(1, 4);
来源：http://hyc.ybcxt.top

TS:   arr.slice(1, 4);
来源：http://qwo.guannengcc.top

Java: list.subList(1, 4);
来源：http://smu.zhaomingkeji.xyz

Go:   arr[1:4]
来源：http://ufa.yonumen.top

Ruby: arr[1, 3]
来源：http://qnx.yanxiufei.cn

C#:   list.GetRange(1, 3);
来源：http://vle.sufxvd.cn

[D08] 合并两个数组
来源：http://lja.guannengcc.top

Py:   a + b;  a.extend(b)
来源：http://dkg.guowangkeji.top

PHP:  array_merge($a, $b);
来源：http://vuf.jinqigufen.top

JS:   [...a, ...b];  a.concat(b);
来源：http://yhi.jiagoushi.top

TS:   [...a, ...b];
来源：http://fjz.zhoulong.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gte.tanke756.top

Go:   append(a, b...)
来源：http://wmc.sysykeji.top

Ruby: a + b;  a.concat(b)
来源：http://kir.aizwys.cn

C#:   a.Concat(b).ToList()
来源：http://tfe.hcnkem.com

[D09] 排序（升序）
来源：http://hmr.zdbjq.cn

Py:   sorted(arr);  arr.sort()
来源：http://xgx.tarul.cn

PHP:  sort($arr);
来源：http://mie.52xcode.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xpt.daria6918.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://iss.ydzc1.top

Java: Collections.sort(list);  list.sort(null);
来源：http://tuo.9152youxi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nmo.shuidangran.top

Ruby: arr.sort
来源：http://tmz.fehbvm.com

C#:   list.Sort();
来源：http://icq.chenjidiqi.icu

[D10] 自定义排序（按字段 / 多条件）
来源：http://tju.feifeiyinyue.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qgr.xinyue.icu

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ywc.c1oappe.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kjf.yj202588.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cvh.guowangkeji.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jhj.epnwcf.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://eyl.gaohongyu789.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://siu.guowangkeji.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://alj.bjfxy.top

[D11] 反转数组
来源：http://pte.zhoulong.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://aug.jinqigfzy.top

PHP:  array_reverse($arr);
来源：http://sry.cashguo.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rew.aibaodan.cn

TS:   [...arr].reverse();
来源：http://eyj.yangfankeji.com

Java: Collections.reverse(list);
来源：http://nrh.wangdashe.top

Go:   slices.Reverse(arr)
来源：http://tnu.zhiwuduotai.top

Ruby: arr.reverse
来源：http://giz.yueranfly.top

C#:   list.Reverse();
来源：http://yiu.gaohongyu789.top

[D12] 查找元素下标
来源：http://xrl.hfpthk.cn

Py:   arr.index(x);  x in arr
来源：http://evo.jyoumei.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ozk.jqgufenzy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://snu.chenjidiqi.icu

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rkd.jianghu66.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ywq.fehbvm.com

Go:   slices.Index(arr, x)
来源：http://emk.yangfankeji.com

Ruby: arr.index(x)
来源：http://flb.nwbrower.top

C#:   list.IndexOf(x);
来源：http://msh.jyoumei.cn

[D13] 过滤（保留满足条件的）
来源：http://xdx.kuanghao11.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wwk.zdbjq.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vma.bbcook.cn

JS:   arr.filter(x => x > 3)
来源：http://exq.xinyue.icu

TS:   arr.filter(x => x > 3)
来源：http://aij.jinghuilouyu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uci.0kj1m.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ktc.epnwcf.com

Ruby: arr.select { |x| x > 3 }
来源：http://xmj.jinqigufen.top

C#:   list.Where(x => x > 3).ToList()
来源：http://qok.birdmap.top

[D14] 映射转换（每个元素变形）
来源：http://jqn.ctjpmb.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://epb.mhx1999.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://twe.xziqi.cn

JS:   arr.map(x => x * 2)
来源：http://lkw.gotoacloud.top

TS:   arr.map(x => x * 2)
来源：http://ijz.jqgfzy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://rbj.haohaochexian.top

Go:   // 手写循环
来源：http://vdg.ehwqpu.com

Ruby: arr.map { |x| x * 2 }
来源：http://npl.fehbvm.com

C#:   list.Select(x => x * 2).ToList()
来源：http://jza.daxiang520.top

[D15] 去重
来源：http://tju.quarkkingdee.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://myx.hammf.cn

PHP:  array_unique($arr);
来源：http://xad.tanke756.top

JS:   [...new Set(arr)]
来源：http://uec.yongpay.top

TS:   [...new Set(arr)]
来源：http://wbm.jinyuanbaomall.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zfl.yj20258888.top

Go:   // 用 map[T]struct{} 手写
来源：http://mdf.yanxiufei.cn

Ruby: arr.uniq
来源：http://xgs.hysaishi.cn

C#:   list.Distinct().ToList()
来源：http://mer.ydjk.org.cn

[D16] 求和与平均值
来源：http://eeq.jinghuilouyu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gin.nanxuanxn.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rje.haohaochexian.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ikj.zdbjq.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xva.yj20258888.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://suc.hysaishi.cn

Go:   // 手写循环累加
来源：http://lqw.aizwys.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zkb.guowangkeji.top

C#:   list.Sum();  list.Average()
来源：http://svw.9152youxi.cn

[D17] 最大值与最小值
来源：http://iev.meibo888.top

Py:   max(arr);  min(arr)
来源：http://jlw.fengsongda.top

PHP:  max($arr);  min($arr);
来源：http://lth.zhengqikj.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wqd.ydzc1.top

TS:   Math.max(...arr);
来源：http://wgr.xylfe.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://nnc.hfpthk.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ijn.daxiang520.top

Ruby: arr.max;  arr.min
来源：http://ceq.ivvv.top

C#:   list.Max();  list.Min()
来源：http://yxo.xuanzx.com

[D18] 扁平化嵌套数组
来源：http://mzo.hysaishi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sur.316326.xyz

PHP:  array_merge(...$nested);
来源：http://akf.zdbjq.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://btr.yonumen.top

TS:   nested.flat();
来源：http://nzd.daxiang520.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://asm.jianghu66.top

Go:   // 手写双层循环
来源：http://joy.cqqwz.cn

Ruby: nested.flatten
来源：http://gmt.52xcode.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xgj.jqgfzy.top

[D19] 按字段分组
来源：http://myz.jqgufenzy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://uhs.zhoulong.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://sdq.cheryme.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tar.gotoacloud.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://jcv.xinyue.icu

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kmn.zhengqikj.top

Go:   // 手写 map[string][]T
来源：http://yuq.52xcode.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rss.meibo888.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yoh.jlsjyb.cn

[D20] 统计每个元素出现次数
来源：http://xsd.iojbl.cn

Py:   Counter(arr)
来源：http://our.meibo888.top

PHP:  array_count_values($arr);
来源：http://owl.hnqzz.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dkz.dashuyun.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zmb.zdbjq.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gsi.yuanzhike.top

Go:   // 手写 map[T]int
来源：http://eds.hfpthk.cn

Ruby: arr.tally
来源：http://que.guowangkeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zlo.jlsjyb.cn

[D21] 判断是否包含某元素
来源：http://nsi.316326.xyz

Py:   x in arr
来源：http://ctx.yj20258.top

PHP:  in_array($x, $arr, true);
来源：http://zoj.snrcjt.cn

JS:   arr.includes(x)
来源：http://rnf.hammf.cn

TS:   arr.includes(x)
来源：http://sid.fktsv.cn

Java: list.contains(x)
来源：http://vfo.xuanzx.com

Go:   slices.Contains(arr, x)
来源：http://ryc.tianlin.xyz

Ruby: arr.include?(x)
来源：http://ilh.daria6918.cn

C#:   list.Contains(x)
来源：http://htp.snrcjt.cn

[D22] 复制数组（避免共享引用）
来源：http://zrh.cucudq.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gdc.yangfankeji.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qoh.nwbrower.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zdg.sjlbkw.cn

TS:   [...arr];
来源：http://llk.hnqzz.top

Java: new ArrayList<>(list);
来源：http://bkb.guannengcc.top

Go:   copied := append([]int(nil), arr...)
来源：http://uhm.gogol.net.cn

Ruby: arr.dup;  arr.clone
来源：http://biw.cashguo.top

C#:   new List<int>(list);
来源：http://wty.zhijiandao.cn

[D23] reduce 累积计算
来源：http://dpe.cucudq.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cgx.yfazqb.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://khk.dianchejie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gtr.fktsv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mel.chenzaomai.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://qzh.zdqjudy.top

Go:   // 手写循环
来源：http://set.mhx1999.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jhh.cdnleiting.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lnv.dashuyun.cn

[D24] 字典 / Map 基本操作
来源：http://wrr.sufxvd.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jml.zhijiandao.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tjr.yonumen.top


<!-- 参考信息 -->