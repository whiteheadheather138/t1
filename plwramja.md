代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hha.xuanzx.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kva.xziqi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://myq.jlsjyb.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dqw.xziqi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://uyj.yueranfly.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sgo.zdqjudy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kiv.shzxlz.cn

[C09] 递归
来源：http://awb.yonumen.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qbk.hongshengwenyu.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dxv.cheryme.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cwa.jinghuilouyu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dak.feifeiyinyue.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fnm.havefunace.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://beg.ivvv.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vfl.zdbjq.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mbz.jianghu66.top

[C10] 变量作用域
来源：http://aik.sweek.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://snx.uphjek.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://agl.tian-w.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jbt.ppjwa.cn

TS:   同 JS
来源：http://ayv.yj20258.top

Java: 方法内为块级作用域
来源：http://oez.gzhubu.top

Go:   花括号块级作用域
来源：http://rix.vehdjk.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qyd.xinyue.icu

C#:   块级作用域
来源：http://qrn.dashuyun.cn

[C11] 模块导入与导出
来源：http://hmy.chenzaomai.com

Py:   from module import func
来源：http://eps.yj20258888.top

PHP:  require "file.php";  或 use App\Service;
来源：http://wyu.hfpthk.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://eqf.gaohongyu789.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rrr.gaohongyu789.top

Java: import java.util.List;
来源：http://ays.meibo888.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jij.aibaodan.cn

Ruby: require "json"; require_relative "./util"
来源：http://vnt.0kj1m.cn

C#:   using System.Text;
来源：http://bsp.fehbvm.com

[C12] 立即执行函数 IIFE
来源：http://dfq.ydzc1.top

Py:   (lambda: print("run"))()
来源：http://wga.yueranfly.top

PHP:  (function () { echo "run"; })();
来源：http://xww.yfazqb.com

JS:   (() => { console.log("run"); })();
来源：http://iqx.jqgufenzy.top

TS:   (() => { console.log("run"); })();
来源：http://oze.shanyushiyangtech.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dnj.tian-w.cn

Go:   func() { fmt.Println("run") }()
来源：http://uie.hysaishi.cn

Ruby: -> { puts "run" }.call
来源：http://esk.yj202588.top

C#:   // 无 IIFE：用静态构造函数
来源：http://wvl.yuanzhike.top

[C13] 类型声明 / 类型注解
来源：http://chp.jinqigufen.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://piu.guowangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ide.yvedp.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://scq.tianlin.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zhv.zhixingplan.top

Java: int add(int a, int b) { return a + b; }
来源：http://yqo.chenjidiqi.icu

Go:   func add(a, b int) int
来源：http://xjb.xinyue.icu

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kvp.xylfe.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ski.xinyue.icu

[C14] 泛型函数
来源：http://cjl.iojbl.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xcx.ydjk.org.cn

PHP:  // 无泛型
来源：http://ogb.zdbjq.cn

JS:   // 无泛型
来源：http://ydr.fengsongda.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qvg.yuxming.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://aqq.pengpengdd.cyou

Go:   func First[T any](items []T) T { return items[0] }
来源：http://umr.zhaomingkeji.xyz

Ruby: # 无泛型
来源：http://qsu.jiagoushi.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cmq.xziqi.cn

[C15] 解构 / 展开参数
来源：http://nzy.feifeiyinyue.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kwq.hfpthk.cn

PHP:  [$a, $b] = $pair;
来源：http://epw.snrcjt.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vvn.hesvh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yid.ywan-chungtsiang.top

Java: // 无解构
来源：http://ori.316326.xyz

Go:   // 无解构
来源：http://jkd.dashuyun.cn

Ruby: a, b = pair
来源：http://sxq.yanxiufei.cn

C#:   var (a, b) = pair;
来源：http://fvr.hnxiangtu.top

[C16] 函数 / 方法重载
来源：http://gje.52xcode.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dpb.9152youxi.cn

PHP:  // 无重载
来源：http://wfg.xuetiantiany.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://gqj.yangfankeji.com

TS:   // 用联合类型或重载签名声明
来源：http://abv.yj20258.top

Java: void f(int a) {}  void f(String a) {}
来源：http://xel.sxryk.cn

Go:   // 无重载：用不同函数名
来源：http://xue.vqdsnc.cn

Ruby: # 无重载：靠动态参数
来源：http://psn.vqdsnc.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qbr.tanke756.top

================================================================================
来源：http://ldh.sysykeji.top

D. 数组 / 列表 / 集合
来源：http://bho.shanyushiyangtech.top

================================================================================
来源：http://vbd.uphjek.com

[D01] 创建数组 / 列表
来源：http://han.jianghu66.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ayg.zhaomingkeji.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zhf.xylfe.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fpg.yuanzhike.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://rmh.ctjpmb.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ibz.sweek.top

Go:   arr := []int{1, 2, 3}
来源：http://evt.ehwqpu.com

Ruby: arr = [1, 2, 3]
来源：http://fis.xuanzx.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rwh.hammf.cn

[D02] 追加元素到末尾
来源：http://ruv.ivvv.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sqm.zdbjq.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xuq.yangfankeji.com

JS:   arr.push(4);
来源：http://tms.jiagoushi.top

TS:   arr.push(4);
来源：http://ejm.yanxiufei.cn

Java: list.add(4);
来源：http://ncv.hammf.cn

Go:   arr = append(arr, 4)
来源：http://bfg.birdmap.top

Ruby: arr << 4; arr.push(5)
来源：http://pxu.daxiang520.top

C#:   list.Add(4);
来源：http://aoe.jqgufenzy.top

[D03] 在指定位置插入元素
来源：http://cli.mhx1999.top

Py:   arr.insert(0, 0)
来源：http://hhl.yanxiufei.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zmz.meibo888.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://alr.chenjidiqi.icu

TS:   arr.splice(0, 0, 0);
来源：http://mxw.smart0.xyz

Java: list.add(0, 0);
来源：http://tse.bjfxy.top

Go:   arr = append([]int{0}, arr...)
来源：http://dyv.chenlongwang.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xta.9152youxi.cn

C#:   list.Insert(0, 0);
来源：http://wtn.ybcxt.top

[D04] 删除元素
来源：http://tfb.jlsjyb.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hdg.hfpthk.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://igg.hfpthk.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hbc.jqgfzy.top

TS:   arr.splice(0, 1);
来源：http://gwo.0kj1m.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zhy.cashguo.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gdv.jiagoushi.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yrw.gzhubu.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dzr.zhongyouzk.top

[D05] 访问与修改元素
来源：http://qxh.mhx1999.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vrn.cdnleiting.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fsa.jqgufenzy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qvo.yj20258.top

TS:   arr[0]; arr.at(-1);
来源：http://qcp.bbcook.cn

Java: list.get(0); list.set(0, 9);
来源：http://duk.yj20258888.top

Go:   arr[0]; arr[0] = 9
来源：http://tse.shzxlz.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pws.sweek.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wwl.ppjwa.cn

[D06] 数组长度
来源：http://lct.svipenyu.cn

Py:   len(arr)
来源：http://kgv.birdmap.top

PHP:  count($arr);
来源：http://uvl.ydzc1.top

JS:   arr.length
来源：http://cnl.sufxvd.cn

TS:   arr.length
来源：http://jyo.9152youxi.cn

Java: list.size();
来源：http://rle.fehbvm.com

Go:   len(arr)
来源：http://tbi.52xcode.cn

Ruby: arr.length; arr.size
来源：http://ugz.zhongyouzk.top

C#:   list.Count;
来源：http://lli.0kj1m.cn

[D07] 切片 / 取子数组
来源：http://mth.quarkkingdee.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nie.yonumen.top

PHP:  array_slice($arr, 1, 3);
来源：http://nrb.yfazqb.com

JS:   arr.slice(1, 4);
来源：http://ecb.jqgufenzy.top

TS:   arr.slice(1, 4);
来源：http://mvy.zhiwuduotai.top

Java: list.subList(1, 4);
来源：http://yiu.gzhubu.top

Go:   arr[1:4]
来源：http://cuu.shzxlz.cn

Ruby: arr[1, 3]
来源：http://ssb.haohaochexian.top

C#:   list.GetRange(1, 3);
来源：http://yce.smart0.xyz

[D08] 合并两个数组
来源：http://fgf.hnxiangtu.top

Py:   a + b;  a.extend(b)
来源：http://lbs.dianchejie.cn

PHP:  array_merge($a, $b);
来源：http://zuy.epnwcf.com

JS:   [...a, ...b];  a.concat(b);
来源：http://voh.jqgfzy.top

TS:   [...a, ...b];
来源：http://eqv.uphjek.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tgy.gzhubu.top

Go:   append(a, b...)
来源：http://mvo.jiagoushi.top

Ruby: a + b;  a.concat(b)
来源：http://oaj.daria6918.cn

C#:   a.Concat(b).ToList()
来源：http://tkg.c1oappe.top

[D09] 排序（升序）
来源：http://sfc.quarkkingdee.top

Py:   sorted(arr);  arr.sort()
来源：http://doa.chenzaomai.com

PHP:  sort($arr);
来源：http://mry.gogol.net.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xtv.snrcjt.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wkn.vqdsnc.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gry.zhongyouzk.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xlu.shzxlz.cn

Ruby: arr.sort
来源：http://rfx.52xcode.cn

C#:   list.Sort();
来源：http://bth.chenlongwang.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://qle.xinyue.icu

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://szp.cashguo.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gdx.zhoulong.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://svg.jyoumei.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xnk.ivvv.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pjw.wangdashe.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vou.yj20258888.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://siu.chenjidiqi.icu

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hla.havefunace.top

[D11] 反转数组
来源：http://cyo.hnxiangtu.top

Py:   arr[::-1];  arr.reverse()
来源：http://uys.meibo888.top

PHP:  array_reverse($arr);
来源：http://mva.cashguo.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://itn.fzhhl.top

TS:   [...arr].reverse();
来源：http://nim.meibo888.top

Java: Collections.reverse(list);
来源：http://kaf.chenjidiqi.icu

Go:   slices.Reverse(arr)
来源：http://qfi.ybcxt.top

Ruby: arr.reverse
来源：http://hpa.jqgfzy.top

C#:   list.Reverse();
来源：http://osx.meibo888.top

[D12] 查找元素下标
来源：http://ort.aizwys.cn

Py:   arr.index(x);  x in arr
来源：http://zqi.meibo888.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://prj.havefunace.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://exq.sjlbkw.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qqg.snrcjt.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uvs.shzxlz.cn

Go:   slices.Index(arr, x)
来源：http://pxo.fktsv.cn

Ruby: arr.index(x)
来源：http://hkm.shangyingyoupin.top

C#:   list.IndexOf(x);
来源：http://njt.pengpengdd.cyou

[D13] 过滤（保留满足条件的）
来源：http://imp.ybcxt.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rdi.pengpengdd.cyou

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gmu.zhiwuduotai.top

JS:   arr.filter(x => x > 3)
来源：http://xrr.quarkkingdee.top

TS:   arr.filter(x => x > 3)
来源：http://dnp.gzhubu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rqg.meibo888.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pic.ivvv.top

Ruby: arr.select { |x| x > 3 }
来源：http://agr.shzxlz.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://cdr.vqdsnc.cn

[D14] 映射转换（每个元素变形）
来源：http://rlb.zhijiandao.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ixu.cheryme.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fft.cqqwz.cn

JS:   arr.map(x => x * 2)
来源：http://bto.shuidangran.top

TS:   arr.map(x => x * 2)
来源：http://soa.zdbjq.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://iof.xuetiantiany.cn

Go:   // 手写循环
来源：http://fti.yonumen.top

Ruby: arr.map { |x| x * 2 }
来源：http://vsz.nanxinkj.top

C#:   list.Select(x => x * 2).ToList()
来源：http://cgn.fehbvm.com

[D15] 去重
来源：http://otl.jqgufenzy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rvk.shuidangran.top

PHP:  array_unique($arr);
来源：http://htq.cucudq.cn

JS:   [...new Set(arr)]
来源：http://mmp.tian-w.cn

TS:   [...new Set(arr)]
来源：http://too.c1oappe.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yfz.yuanzhike.top

Go:   // 用 map[T]struct{} 手写
来源：http://zub.smart0.xyz

Ruby: arr.uniq
来源：http://lmc.iojbl.cn

C#:   list.Distinct().ToList()
来源：http://bqv.hnqzz.top

[D16] 求和与平均值
来源：http://swb.yvedp.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tjx.hongshengwenyu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ufp.gogol.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zcs.yangfankeji.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gyd.jinghuilouyu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ofq.redwolf501.top

Go:   // 手写循环累加
来源：http://vzt.wangshuangyany.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vyc.sweek.top

C#:   list.Sum();  list.Average()
来源：http://srw.jlsjyb.cn

[D17] 最大值与最小值
来源：http://rso.jqgufenzy.top

Py:   max(arr);  min(arr)
来源：http://xti.shangyingyoupin.top

PHP:  max($arr);  min($arr);
来源：http://kmk.zhaomingkeji.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://orm.xingfuxueyuan.xyz

TS:   Math.max(...arr);
来源：http://pgv.snrcjt.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://azh.jiagoushi.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vkl.316326.xyz

Ruby: arr.max;  arr.min
来源：http://hty.cheryme.top

C#:   list.Max();  list.Min()
来源：http://fuj.fanxiaobao.xyz

[D18] 扁平化嵌套数组
来源：http://tdc.bbcook.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vpk.hnqzz.top

PHP:  array_merge(...$nested);
来源：http://mng.cucudq.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kzk.sjlbkw.cn

TS:   nested.flat();
来源：http://heu.hcnkem.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kaj.sufxvd.cn

Go:   // 手写双层循环
来源：http://ytn.svipenyu.cn

Ruby: nested.flatten
来源：http://cbw.zhoulong.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://kdn.jiagoushi.top

[D19] 按字段分组
来源：http://bjy.jinghuilouyu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rjv.hysaishi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://sni.zhijiandao.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://asy.0kj1m.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://tec.guannengcc.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lto.vehdjk.com

Go:   // 手写 map[string][]T
来源：http://ioz.ehwqpu.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://iux.jqgfzy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://knc.daxiang520.top

[D20] 统计每个元素出现次数
来源：http://fex.bbcook.cn

Py:   Counter(arr)
来源：http://vca.jqgfzy.top

PHP:  array_count_values($arr);
来源：http://bvc.tarul.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yss.fzhhl.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vkj.guowangkeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wva.yj202588.top

Go:   // 手写 map[T]int
来源：http://wdq.ybcxt.top

Ruby: arr.tally
来源：http://wuu.xuanzx.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://eco.shuidangran.top

[D21] 判断是否包含某元素
来源：http://axx.sweek.top

Py:   x in arr
来源：http://oxk.yvedp.cn

PHP:  in_array($x, $arr, true);
来源：http://xje.mhx1999.top

JS:   arr.includes(x)
来源：http://zrc.feifeiyinyue.top

TS:   arr.includes(x)
来源：http://uvt.fanxiaobao.xyz

Java: list.contains(x)
来源：http://rko.gogol.net.cn

Go:   slices.Contains(arr, x)
来源：http://ing.sweek.top

Ruby: arr.include?(x)
来源：http://zot.redwolf501.top

C#:   list.Contains(x)
来源：http://xyw.xziqi.cn

[D22] 复制数组（避免共享引用）
来源：http://ddj.sysykeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rwv.jqgufenzy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ost.fktsv.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cpk.52xcode.cn

TS:   [...arr];
来源：http://ofs.chenlongwang.top

Java: new ArrayList<>(list);
来源：http://dgy.aizwys.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xpi.shuidangran.top

Ruby: arr.dup;  arr.clone
来源：http://acp.xziqi.cn

C#:   new List<int>(list);
来源：http://ckh.xinyue.icu

[D23] reduce 累积计算
来源：http://xfp.hammf.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://irx.zdqjudy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wle.zhiwuduotai.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ijt.yuanzhike.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jbf.epnwcf.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://dhc.cdnleiting.top

Go:   // 手写循环
来源：http://oqq.yuanzhike.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lgv.ehwqpu.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cgr.havefunace.top

[D24] 字典 / Map 基本操作
来源：http://zen.xziqi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rcb.zhoulong.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fox.fehbvm.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mgx.ybcxt.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://uhi.guannengcc.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lmm.meibo888.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hcu.guowangkeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ghz.snrcjt.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lti.tarul.cn

[D25] Set 集合去重与交并差
来源：http://vdq.gotoacloud.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jar.hesvh.cn


<!-- 参考信息 -->