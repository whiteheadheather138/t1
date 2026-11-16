代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nti.zdbjq.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cre.sxryk.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ynm.hnxiangtu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kmk.yj202588.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dto.gogol.net.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fpk.hammf.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xcg.aibaodan.cn

[C09] 递归
来源：http://ewc.jinqigfzy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sdj.zhiwuduotai.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://int.dashuyun.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tdk.c1oappe.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qyi.wangshuangyany.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mah.yj20258.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uof.jiagoushi.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jay.yongpay.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://aoy.yvedp.cn

[C10] 变量作用域
来源：http://hxz.hnqzz.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ntx.yj20258888.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mqu.yfazqb.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ukw.zdqjudy.top

TS:   同 JS
来源：http://rtw.jiagoushi.top

Java: 方法内为块级作用域
来源：http://zah.hnqzz.top

Go:   花括号块级作用域
来源：http://xua.chenlongwang.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rkg.fzhhl.top

C#:   块级作用域
来源：http://zoe.yuanzhike.top

[C11] 模块导入与导出
来源：http://ars.bjfxy.top

Py:   from module import func
来源：http://iqc.yfazqb.com

PHP:  require "file.php";  或 use App\Service;
来源：http://qox.nwbrower.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://nzz.haohaochexian.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kxk.epnwcf.com

Java: import java.util.List;
来源：http://ruh.pengpengdd.cyou

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rud.jyoumei.cn

Ruby: require "json"; require_relative "./util"
来源：http://lzj.sysykeji.top

C#:   using System.Text;
来源：http://sfh.yj20258888.top

[C12] 立即执行函数 IIFE
来源：http://lyu.yuanzhike.top

Py:   (lambda: print("run"))()
来源：http://mzw.iojbl.cn

PHP:  (function () { echo "run"; })();
来源：http://cky.tian-w.cn

JS:   (() => { console.log("run"); })();
来源：http://jir.ydzc1.top

TS:   (() => { console.log("run"); })();
来源：http://xwd.gzhubu.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mhy.meibo888.top

Go:   func() { fmt.Println("run") }()
来源：http://rvm.zhixingplan.top

Ruby: -> { puts "run" }.call
来源：http://uiy.daxiang520.top

C#:   // 无 IIFE：用静态构造函数
来源：http://gaa.yangfankeji.com

[C13] 类型声明 / 类型注解
来源：http://qgf.xinyue.icu

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wpg.pycfn.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://anz.nanxuanxn.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kie.iojbl.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hks.vqdsnc.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ekt.zhongyouzk.top

Go:   func add(a, b int) int
来源：http://tgw.tian-w.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jod.yj20258.top

C#:   int Add(int a, int b) => a + b;
来源：http://qrn.yuanzhike.top

[C14] 泛型函数
来源：http://xpd.cashguo.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zcg.hesvh.cn

PHP:  // 无泛型
来源：http://cwb.redwolf501.top

JS:   // 无泛型
来源：http://sse.jlsjyb.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cqf.guowangkeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://izc.nanxuanxn.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pfq.xziqi.cn

Ruby: # 无泛型
来源：http://uww.cashguo.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hmq.fzhhl.top

[C15] 解构 / 展开参数
来源：http://aoq.svipenyu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qeb.smart0.xyz

PHP:  [$a, $b] = $pair;
来源：http://bzv.sweek.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://adp.snrcjt.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yke.316326.xyz

Java: // 无解构
来源：http://tcx.feifeiyinyue.top

Go:   // 无解构
来源：http://hgk.sjlbkw.cn

Ruby: a, b = pair
来源：http://rms.jyoumei.cn

C#:   var (a, b) = pair;
来源：http://dcg.cheryme.top

[C16] 函数 / 方法重载
来源：http://nig.meibo888.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hsr.jyoumei.cn

PHP:  // 无重载
来源：http://pbo.sjlbkw.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bxc.mhx1999.top

TS:   // 用联合类型或重载签名声明
来源：http://xna.hcnkem.com

Java: void f(int a) {}  void f(String a) {}
来源：http://kxq.snrcjt.cn

Go:   // 无重载：用不同函数名
来源：http://ysr.yuxming.cn

Ruby: # 无重载：靠动态参数
来源：http://uvm.jinqigfzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://eyo.c1oappe.top

================================================================================
来源：http://amv.hfpthk.cn

D. 数组 / 列表 / 集合
来源：http://ugs.pycfn.com

================================================================================
来源：http://qmk.ppjwa.cn

[D01] 创建数组 / 列表
来源：http://hls.gotoacloud.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://drb.ctjpmb.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ibg.svipenyu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uqy.ppjwa.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wlo.gaohongyu789.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hqz.zhoulong.xyz

Go:   arr := []int{1, 2, 3}
来源：http://fqm.kuanghao11.cn

Ruby: arr = [1, 2, 3]
来源：http://djy.gzhubu.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ibp.bjfxy.top

[D02] 追加元素到末尾
来源：http://ssk.jqgfzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jol.ybcxt.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mke.fehbvm.com

JS:   arr.push(4);
来源：http://vxj.hysaishi.cn

TS:   arr.push(4);
来源：http://rmt.jiagoushi.top

Java: list.add(4);
来源：http://vds.aibaodan.cn

Go:   arr = append(arr, 4)
来源：http://zlt.jlsjyb.cn

Ruby: arr << 4; arr.push(5)
来源：http://ils.zhengqikj.top

C#:   list.Add(4);
来源：http://vzy.gaohongyu789.top

[D03] 在指定位置插入元素
来源：http://xts.fengsongda.top

Py:   arr.insert(0, 0)
来源：http://fwa.chenlongwang.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zkf.mhx1999.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nwu.uphjek.com

TS:   arr.splice(0, 0, 0);
来源：http://owq.sufxvd.cn

Java: list.add(0, 0);
来源：http://dtn.jyoumei.cn

Go:   arr = append([]int{0}, arr...)
来源：http://emo.cucudq.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kxo.uphjek.com

C#:   list.Insert(0, 0);
来源：http://nqz.pengpengdd.cyou

[D04] 删除元素
来源：http://slv.xuetiantiany.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://znk.hnqzz.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://aue.dashuyun.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://doc.dianchejie.cn

TS:   arr.splice(0, 1);
来源：http://jxm.sysykeji.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://prm.bbcook.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wop.redwolf501.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pjc.gaohongyu789.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xqr.cdnleiting.top

[D05] 访问与修改元素
来源：http://hbi.andypj.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ird.jyoumei.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uwk.yueranfly.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rrf.wangshuangyany.cn

TS:   arr[0]; arr.at(-1);
来源：http://new.zdbjq.cn

Java: list.get(0); list.set(0, 9);
来源：http://eou.nwbrower.top

Go:   arr[0]; arr[0] = 9
来源：http://waq.fanxiaobao.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xay.zhaomingkeji.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ars.zdbjq.cn

[D06] 数组长度
来源：http://iyv.jqgufenzy.top

Py:   len(arr)
来源：http://efv.jyoumei.cn

PHP:  count($arr);
来源：http://lnl.sjlbkw.cn

JS:   arr.length
来源：http://vdw.shzxlz.cn

TS:   arr.length
来源：http://jgw.andypj.xyz

Java: list.size();
来源：http://tjr.tian-w.cn

Go:   len(arr)
来源：http://sdi.gzhubu.top

Ruby: arr.length; arr.size
来源：http://aih.cashguo.top

C#:   list.Count;
来源：http://mjt.aibaodan.cn

[D07] 切片 / 取子数组
来源：http://iju.hammf.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xln.mhx1999.top

PHP:  array_slice($arr, 1, 3);
来源：http://sqk.fanxiaobao.xyz

JS:   arr.slice(1, 4);
来源：http://mws.yj202588.top

TS:   arr.slice(1, 4);
来源：http://tjk.dashuyun.cn

Java: list.subList(1, 4);
来源：http://xkv.hysaishi.cn

Go:   arr[1:4]
来源：http://wiv.jinqigufen.top

Ruby: arr[1, 3]
来源：http://xue.cashguo.top

C#:   list.GetRange(1, 3);
来源：http://yks.feifeiyinyue.top

[D08] 合并两个数组
来源：http://voi.shzxlz.cn

Py:   a + b;  a.extend(b)
来源：http://lla.hysaishi.cn

PHP:  array_merge($a, $b);
来源：http://pns.guowangkeji.top

JS:   [...a, ...b];  a.concat(b);
来源：http://mej.jinqigufen.top

TS:   [...a, ...b];
来源：http://lfc.birdmap.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://oja.hfpthk.cn

Go:   append(a, b...)
来源：http://dpa.dianchejie.cn

Ruby: a + b;  a.concat(b)
来源：http://rrw.ctjpmb.com

C#:   a.Concat(b).ToList()
来源：http://rhd.yanxiufei.cn

[D09] 排序（升序）
来源：http://zva.fzhhl.top

Py:   sorted(arr);  arr.sort()
来源：http://kwd.daria6918.cn

PHP:  sort($arr);
来源：http://vsl.c1oappe.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lht.zhoulong.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://yjx.zhoulong.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://nil.fehbvm.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bxf.xuanzx.com

Ruby: arr.sort
来源：http://yba.zhixingplan.top

C#:   list.Sort();
来源：http://izz.jiagoushi.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://onl.epnwcf.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://var.tian-w.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://faw.sweek.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vml.jinqigufen.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tdn.hnqzz.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nfl.epnwcf.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wme.zhoulong.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qxy.ydjk.org.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://twn.ppjwa.cn

[D11] 反转数组
来源：http://bnz.shuidangran.top

Py:   arr[::-1];  arr.reverse()
来源：http://sit.epnwcf.com

PHP:  array_reverse($arr);
来源：http://hia.dianchejie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vtc.bbcook.cn

TS:   [...arr].reverse();
来源：http://bco.vehdjk.com

Java: Collections.reverse(list);
来源：http://jjj.daria6918.cn

Go:   slices.Reverse(arr)
来源：http://qfe.yj20258888.top

Ruby: arr.reverse
来源：http://udr.cashguo.top

C#:   list.Reverse();
来源：http://dck.mhx1999.top

[D12] 查找元素下标
来源：http://srp.ppjwa.cn

Py:   arr.index(x);  x in arr
来源：http://isn.pycfn.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qfq.shanyushiyangtech.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uns.yuxming.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xcv.cheryme.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lev.bjfxy.top

Go:   slices.Index(arr, x)
来源：http://scn.pengpengdd.cyou

Ruby: arr.index(x)
来源：http://dph.gaohongyu789.top

C#:   list.IndexOf(x);
来源：http://jwa.aibaodan.cn

[D13] 过滤（保留满足条件的）
来源：http://meg.gotoacloud.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lqf.jinqigufen.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wkh.wangshuangyany.cn

JS:   arr.filter(x => x > 3)
来源：http://wlz.shzxlz.cn

TS:   arr.filter(x => x > 3)
来源：http://ijq.zhongyouzk.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dzk.ydzc1.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rvn.yj202588.top

Ruby: arr.select { |x| x > 3 }
来源：http://yvu.hywenlv.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pls.yj20258.top

[D14] 映射转换（每个元素变形）
来源：http://sku.quarkkingdee.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bto.meibo888.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bnp.fanxiaobao.xyz

JS:   arr.map(x => x * 2)
来源：http://der.zdbjq.cn

TS:   arr.map(x => x * 2)
来源：http://svy.hammf.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://auo.xziqi.cn

Go:   // 手写循环
来源：http://vfz.ctjpmb.com

Ruby: arr.map { |x| x * 2 }
来源：http://xji.cashguo.top

C#:   list.Select(x => x * 2).ToList()
来源：http://rgi.yongpay.top

[D15] 去重
来源：http://jyb.zycfv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://olr.zhaomingkeji.xyz

PHP:  array_unique($arr);
来源：http://fpz.xinyue.icu

JS:   [...new Set(arr)]
来源：http://lvb.tanke756.top

TS:   [...new Set(arr)]
来源：http://hpv.jinghuilouyu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zqx.bbcook.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yjr.316326.xyz

Ruby: arr.uniq
来源：http://hho.cashguo.top

C#:   list.Distinct().ToList()
来源：http://kvt.quarkkingdee.top

[D16] 求和与平均值
来源：http://npe.tanke756.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rbv.52xcode.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lfh.gaohongyu789.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lom.cheryme.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nsq.zdqjudy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://npe.shangyingyoupin.top

Go:   // 手写循环累加
来源：http://umn.dashuyun.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fic.jlsjyb.cn

C#:   list.Sum();  list.Average()
来源：http://mxb.mhx1999.top

[D17] 最大值与最小值
来源：http://iim.haohaochexian.top

Py:   max(arr);  min(arr)
来源：http://lqd.kuanghao11.cn

PHP:  max($arr);  min($arr);
来源：http://fks.redwolf501.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://iny.xylfe.cn

TS:   Math.max(...arr);
来源：http://fhn.jlsjyb.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qbr.chenlongwang.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ipv.hesvh.cn

Ruby: arr.max;  arr.min
来源：http://eqo.cheryme.top

C#:   list.Max();  list.Min()
来源：http://pzm.jinghuilouyu.cn

[D18] 扁平化嵌套数组
来源：http://hji.aibaodan.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rqg.hesvh.cn

PHP:  array_merge(...$nested);
来源：http://ufj.hnqzz.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qyj.zycfv.cn

TS:   nested.flat();
来源：http://kzj.yanxiufei.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://spu.jqgfzy.top

Go:   // 手写双层循环
来源：http://tsa.yuxming.cn

Ruby: nested.flatten
来源：http://ssi.yj20258.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://wol.fengsongda.top

[D19] 按字段分组
来源：http://jbr.sjlbkw.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://doh.zhengqikj.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kgf.yonumen.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nur.bjfxy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://rvn.yueranfly.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bnq.zdbjq.cn

Go:   // 手写 map[string][]T
来源：http://vaw.yangfankeji.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://nxr.yonumen.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fav.nanxinkj.top

[D20] 统计每个元素出现次数
来源：http://jjc.zdqjudy.top

Py:   Counter(arr)
来源：http://fzv.ehwqpu.com

PHP:  array_count_values($arr);
来源：http://oxx.zdqjudy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zjg.svipenyu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://okx.yvedp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ykj.hongshengwenyu.top

Go:   // 手写 map[T]int
来源：http://pna.iojbl.cn

Ruby: arr.tally
来源：http://nac.gzhubu.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qei.havefunace.top

[D21] 判断是否包含某元素
来源：http://jzh.shzxlz.cn

Py:   x in arr
来源：http://egr.dashuyun.cn

PHP:  in_array($x, $arr, true);
来源：http://znz.birdmap.top

JS:   arr.includes(x)
来源：http://mgk.ywan-chungtsiang.top

TS:   arr.includes(x)
来源：http://wku.daxiang520.top

Java: list.contains(x)
来源：http://tpy.hywenlv.cn

Go:   slices.Contains(arr, x)
来源：http://wge.sysykeji.top

Ruby: arr.include?(x)
来源：http://sxe.jqgufenzy.top

C#:   list.Contains(x)
来源：http://wwn.gzhubu.top

[D22] 复制数组（避免共享引用）
来源：http://etu.mhx1999.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://guy.ctjpmb.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://abe.cucudq.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://clo.pengpengdd.cyou

TS:   [...arr];
来源：http://ahd.c1oappe.top

Java: new ArrayList<>(list);
来源：http://uhg.andypj.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://wni.yangfankeji.com

Ruby: arr.dup;  arr.clone
来源：http://frk.feifeiyinyue.top

C#:   new List<int>(list);
来源：http://daa.meibo888.top

[D23] reduce 累积计算
来源：http://yhp.ybcxt.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://phk.ehwqpu.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gcv.ydzc1.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ftm.zdbjq.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sld.chenjidiqi.icu

Java: list.stream().reduce(0, Integer::sum)
来源：http://gvf.fengsongda.top

Go:   // 手写循环
来源：http://hgo.xylfe.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://oiw.chenlongwang.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uit.bjfxy.top

[D24] 字典 / Map 基本操作
来源：http://dha.tarul.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nut.0kj1m.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://exe.tianlin.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zkt.zhongyouzk.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kdo.shuidangran.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ric.nanxinkj.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fdc.zhijiandao.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dlh.yanxiufei.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://phm.yueranfly.top

[D25] Set 集合去重与交并差
来源：http://fzj.zdqjudy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vgy.ywan-chungtsiang.top


<!-- 参考信息 -->