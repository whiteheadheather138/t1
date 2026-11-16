代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://ujb.havefunace.top

C#:   arr.Select(s => s.ToUpper())
来源：http://zke.9152youxi.cn

[C08] 闭包
来源：http://lxn.tian-w.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vil.jinyuanbaomall.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hdf.jianghu66.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qwx.hfpthk.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bne.mhx1999.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pcm.yongpay.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mal.zycfv.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hkv.yuxming.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://avg.yuxming.cn

[C09] 递归
来源：http://gll.52xcode.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lvo.aibaodan.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qjl.uphjek.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://clr.jinghuilouyu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wgu.pycfn.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://osq.epnwcf.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://oxr.pengpengdd.cyou

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mku.zhaomingkeji.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tbd.yfazqb.com

[C10] 变量作用域
来源：http://dpo.xuetiantiany.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://apm.tanke756.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hpv.feifeiyinyue.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://phy.snrcjt.cn

TS:   同 JS
来源：http://cto.ywan-chungtsiang.top

Java: 方法内为块级作用域
来源：http://mqu.gzhubu.top

Go:   花括号块级作用域
来源：http://zdx.pengpengdd.cyou

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dvx.hnqzz.top

C#:   块级作用域
来源：http://odn.feifeiyinyue.top

[C11] 模块导入与导出
来源：http://pqf.smart0.xyz

Py:   from module import func
来源：http://ink.chenjidiqi.icu

PHP:  require "file.php";  或 use App\Service;
来源：http://szv.haohaochexian.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://hmx.zhongyouzk.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uck.feifeiyinyue.top

Java: import java.util.List;
来源：http://xmn.jqgfzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://emu.fktsv.cn

Ruby: require "json"; require_relative "./util"
来源：http://ois.ppjwa.cn

C#:   using System.Text;
来源：http://chf.hywenlv.cn

[C12] 立即执行函数 IIFE
来源：http://tsa.zhaomingkeji.xyz

Py:   (lambda: print("run"))()
来源：http://haq.haohaochexian.top

PHP:  (function () { echo "run"; })();
来源：http://njk.fzhhl.top

JS:   (() => { console.log("run"); })();
来源：http://rfl.yfazqb.com

TS:   (() => { console.log("run"); })();
来源：http://ytb.zhiwuduotai.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ypj.xuetiantiany.cn

Go:   func() { fmt.Println("run") }()
来源：http://pyg.zdbjq.cn

Ruby: -> { puts "run" }.call
来源：http://adx.shanyushiyangtech.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ylc.hcnkem.com

[C13] 类型声明 / 类型注解
来源：http://ifh.yj20258.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vgo.yj20258.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cks.jiagoushi.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mve.wangshuangyany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tpp.tian-w.cn

Java: int add(int a, int b) { return a + b; }
来源：http://hqq.hammf.cn

Go:   func add(a, b int) int
来源：http://qih.zdbjq.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xar.kuanghao11.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xiy.chenlongwang.top

[C14] 泛型函数
来源：http://ihd.birdmap.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wjk.chenlongwang.top

PHP:  // 无泛型
来源：http://ymv.zhaomingkeji.xyz

JS:   // 无泛型
来源：http://mcw.zdqjudy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lyo.yj20258.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ovn.zhengqikj.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://evt.52xcode.cn

Ruby: # 无泛型
来源：http://hbq.fengsongda.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zmi.xingfuxueyuan.xyz

[C15] 解构 / 展开参数
来源：http://dhx.cqqwz.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qmj.shuidangran.top

PHP:  [$a, $b] = $pair;
来源：http://kvz.jianghu66.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zlw.zhoulong.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uqk.zdqjudy.top

Java: // 无解构
来源：http://tnd.andypj.xyz

Go:   // 无解构
来源：http://yly.havefunace.top

Ruby: a, b = pair
来源：http://rdg.fktsv.cn

C#:   var (a, b) = pair;
来源：http://avb.yuxming.cn

[C16] 函数 / 方法重载
来源：http://tgh.ivvv.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lqr.yvedp.cn

PHP:  // 无重载
来源：http://exa.shanyushiyangkeji.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ifg.yangfankeji.com

TS:   // 用联合类型或重载签名声明
来源：http://tmg.vqdsnc.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://amb.cucudq.cn

Go:   // 无重载：用不同函数名
来源：http://glb.jinghuilouyu.cn

Ruby: # 无重载：靠动态参数
来源：http://gbs.ybcxt.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://kun.cheryme.top

================================================================================
来源：http://zat.cqqwz.cn

D. 数组 / 列表 / 集合
来源：http://lmp.wangdashe.top

================================================================================
来源：http://ahi.zhaomingkeji.xyz

[D01] 创建数组 / 列表
来源：http://jfy.sysykeji.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://mzr.svipenyu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://unh.andypj.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://glf.ydjk.org.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://nxg.guannengcc.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zkh.bbcook.cn

Go:   arr := []int{1, 2, 3}
来源：http://oeu.guowangkeji.top

Ruby: arr = [1, 2, 3]
来源：http://oyb.xingfuxueyuan.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lms.fehbvm.com

[D02] 追加元素到末尾
来源：http://upb.daria6918.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vwv.nanxinkj.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lyk.iojbl.cn

JS:   arr.push(4);
来源：http://fqt.yj202588.top

TS:   arr.push(4);
来源：http://yur.xziqi.cn

Java: list.add(4);
来源：http://psb.yuxming.cn

Go:   arr = append(arr, 4)
来源：http://hii.zdbjq.cn

Ruby: arr << 4; arr.push(5)
来源：http://otn.nanxuanxn.top

C#:   list.Add(4);
来源：http://pla.jqgufenzy.top

[D03] 在指定位置插入元素
来源：http://iqy.jinyuanbaomall.cn

Py:   arr.insert(0, 0)
来源：http://hev.pycfn.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gnt.yvedp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tbt.hywenlv.cn

TS:   arr.splice(0, 0, 0);
来源：http://rvm.guannengcc.top

Java: list.add(0, 0);
来源：http://pfp.yonumen.top

Go:   arr = append([]int{0}, arr...)
来源：http://quk.quarkkingdee.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vlm.wangdashe.top

C#:   list.Insert(0, 0);
来源：http://yna.nwbrower.top

[D04] 删除元素
来源：http://kfe.gzhubu.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mwr.hfpthk.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tyt.shzxlz.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vej.xylfe.cn

TS:   arr.splice(0, 1);
来源：http://zld.yueranfly.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://aeq.bbcook.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ysm.quarkkingdee.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nto.sjlbkw.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wko.zhaomingkeji.xyz

[D05] 访问与修改元素
来源：http://cnk.uphjek.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yev.quarkkingdee.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fkk.shanyushiyangtech.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wtv.tanke756.top

TS:   arr[0]; arr.at(-1);
来源：http://lzv.xinyue.icu

Java: list.get(0); list.set(0, 9);
来源：http://cyf.gaohongyu789.top

Go:   arr[0]; arr[0] = 9
来源：http://jok.cqqwz.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bgq.sysykeji.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pwv.chenjidiqi.icu

[D06] 数组长度
来源：http://xuv.ydjk.org.cn

Py:   len(arr)
来源：http://thw.zhongyouzk.top

PHP:  count($arr);
来源：http://sxa.ybcxt.top

JS:   arr.length
来源：http://wbu.yj20258.top

TS:   arr.length
来源：http://qmw.jianghu66.top

Java: list.size();
来源：http://ufq.fzhhl.top

Go:   len(arr)
来源：http://xgo.zhoulong.xyz

Ruby: arr.length; arr.size
来源：http://kmt.yangfankeji.com

C#:   list.Count;
来源：http://trf.yj20258888.top

[D07] 切片 / 取子数组
来源：http://wky.gotoacloud.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://srt.yangfankeji.com

PHP:  array_slice($arr, 1, 3);
来源：http://een.xylfe.cn

JS:   arr.slice(1, 4);
来源：http://idm.zhongyouzk.top

TS:   arr.slice(1, 4);
来源：http://lqr.yangfankeji.com

Java: list.subList(1, 4);
来源：http://otm.hnxiangtu.top

Go:   arr[1:4]
来源：http://jsr.ctjpmb.com

Ruby: arr[1, 3]
来源：http://fap.nanxuanxn.top

C#:   list.GetRange(1, 3);
来源：http://dpm.cdnleiting.top

[D08] 合并两个数组
来源：http://kjc.hywenlv.cn

Py:   a + b;  a.extend(b)
来源：http://bgy.xingfuxueyuan.xyz

PHP:  array_merge($a, $b);
来源：http://jqn.vehdjk.com

JS:   [...a, ...b];  a.concat(b);
来源：http://djh.ybcxt.top

TS:   [...a, ...b];
来源：http://mls.svipenyu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wfc.sweek.top

Go:   append(a, b...)
来源：http://ivc.yvedp.cn

Ruby: a + b;  a.concat(b)
来源：http://qjt.ctjpmb.com

C#:   a.Concat(b).ToList()
来源：http://odu.yueranfly.top

[D09] 排序（升序）
来源：http://fwq.snrcjt.cn

Py:   sorted(arr);  arr.sort()
来源：http://sgj.aizwys.cn

PHP:  sort($arr);
来源：http://vob.hysaishi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://iql.kuanghao11.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://vkm.zhiwuduotai.top

Java: Collections.sort(list);  list.sort(null);
来源：http://iep.shzxlz.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://aww.nwbrower.top

Ruby: arr.sort
来源：http://bvw.fehbvm.com

C#:   list.Sort();
来源：http://gqj.tanke756.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://mem.birdmap.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gmy.yj20258.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vja.daria6918.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rbk.zdqjudy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ial.hnxiangtu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yol.hysaishi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ckp.fktsv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tpj.316326.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xzg.redwolf501.top

[D11] 反转数组
来源：http://fir.chenjidiqi.icu

Py:   arr[::-1];  arr.reverse()
来源：http://tzh.hnqzz.top

PHP:  array_reverse($arr);
来源：http://ifz.nanxinkj.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://elr.jiagoushi.top

TS:   [...arr].reverse();
来源：http://ygx.zhengqikj.top

Java: Collections.reverse(list);
来源：http://wxx.cheryme.top

Go:   slices.Reverse(arr)
来源：http://gnn.pengpengdd.cyou

Ruby: arr.reverse
来源：http://bdy.hammf.cn

C#:   list.Reverse();
来源：http://yyq.hnqzz.top

[D12] 查找元素下标
来源：http://lon.shanyushiyangtech.top

Py:   arr.index(x);  x in arr
来源：http://lvw.nanxinkj.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xzs.ctjpmb.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ccm.bbcook.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zrt.fanxiaobao.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://edp.ydzc1.top

Go:   slices.Index(arr, x)
来源：http://ndq.yuxming.cn

Ruby: arr.index(x)
来源：http://eze.hnxiangtu.top

C#:   list.IndexOf(x);
来源：http://fna.birdmap.top

[D13] 过滤（保留满足条件的）
来源：http://jsc.hesvh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cyp.fengsongda.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://eus.pycfn.com

JS:   arr.filter(x => x > 3)
来源：http://ouz.shanyushiyangkeji.top

TS:   arr.filter(x => x > 3)
来源：http://cyk.chenzaomai.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yuw.316326.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://khj.tanke756.top

Ruby: arr.select { |x| x > 3 }
来源：http://yjl.zhongyouzk.top

C#:   list.Where(x => x > 3).ToList()
来源：http://gdi.0kj1m.cn

[D14] 映射转换（每个元素变形）
来源：http://qns.nwbrower.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vnt.chenlongwang.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dlp.xuanzx.com

JS:   arr.map(x => x * 2)
来源：http://csh.gogol.net.cn

TS:   arr.map(x => x * 2)
来源：http://jia.jianghu66.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://pmw.tanke756.top

Go:   // 手写循环
来源：http://mkr.c1oappe.top

Ruby: arr.map { |x| x * 2 }
来源：http://mvy.daria6918.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://izk.zhoulong.xyz

[D15] 去重
来源：http://mbx.zhongyouzk.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://paj.nanxinkj.top

PHP:  array_unique($arr);
来源：http://nsh.smart0.xyz

JS:   [...new Set(arr)]
来源：http://ncw.bbcook.cn

TS:   [...new Set(arr)]
来源：http://nra.feifeiyinyue.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fku.hnqzz.top

Go:   // 用 map[T]struct{} 手写
来源：http://yfb.iojbl.cn

Ruby: arr.uniq
来源：http://caa.bjfxy.top

C#:   list.Distinct().ToList()
来源：http://qlp.xziqi.cn

[D16] 求和与平均值
来源：http://jbl.vehdjk.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gcu.zhengqikj.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dui.jianghu66.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bev.chenjidiqi.icu

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qbl.zdqjudy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://iqh.redwolf501.top

Go:   // 手写循环累加
来源：http://wpv.gzhubu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zqm.quarkkingdee.top

C#:   list.Sum();  list.Average()
来源：http://llm.hcnkem.com

[D17] 最大值与最小值
来源：http://cfy.feifeiyinyue.top

Py:   max(arr);  min(arr)
来源：http://fwf.jlsjyb.cn

PHP:  max($arr);  min($arr);
来源：http://owk.sweek.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ibq.c1oappe.top

TS:   Math.max(...arr);
来源：http://jae.sxryk.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ctp.pengpengdd.cyou

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ujy.vehdjk.com

Ruby: arr.max;  arr.min
来源：http://pwl.tian-w.cn

C#:   list.Max();  list.Min()
来源：http://zbr.cheryme.top

[D18] 扁平化嵌套数组
来源：http://vdx.xziqi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sdm.nanxinkj.top

PHP:  array_merge(...$nested);
来源：http://lqz.gaohongyu789.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xyz.ehwqpu.com

TS:   nested.flat();
来源：http://wmy.zycfv.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ipp.jinqigufen.top

Go:   // 手写双层循环
来源：http://uqw.xuetiantiany.cn

Ruby: nested.flatten
来源：http://key.epnwcf.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://qff.wangdashe.top

[D19] 按字段分组
来源：http://gup.jqgfzy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://iiw.shuidangran.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gqv.uphjek.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zuz.ppjwa.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://cga.sweek.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fcb.ydzc1.top

Go:   // 手写 map[string][]T
来源：http://tgh.ivvv.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://qim.bbcook.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jmv.smart0.xyz

[D20] 统计每个元素出现次数
来源：http://kre.ywan-chungtsiang.top

Py:   Counter(arr)
来源：http://req.chenlongwang.top

PHP:  array_count_values($arr);
来源：http://dzv.sxryk.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dby.pycfn.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dne.shanyushiyangtech.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gkm.jinqigfzy.top

Go:   // 手写 map[T]int
来源：http://att.hcnkem.com

Ruby: arr.tally
来源：http://vzn.chenzaomai.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zhl.hfpthk.cn

[D21] 判断是否包含某元素
来源：http://fxd.fengsongda.top

Py:   x in arr
来源：http://ffm.tanke756.top

PHP:  in_array($x, $arr, true);
来源：http://znj.tianlin.xyz

JS:   arr.includes(x)
来源：http://dzw.nwbrower.top

TS:   arr.includes(x)
来源：http://txv.fanxiaobao.xyz

Java: list.contains(x)
来源：http://wky.zhengqikj.top

Go:   slices.Contains(arr, x)
来源：http://eeg.epnwcf.com

Ruby: arr.include?(x)
来源：http://vsh.hongshengwenyu.top

C#:   list.Contains(x)
来源：http://xag.316326.xyz

[D22] 复制数组（避免共享引用）
来源：http://ppy.fanxiaobao.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://myw.cqqwz.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blw.ydzc1.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://asf.ehwqpu.com

TS:   [...arr];
来源：http://efp.hongshengwenyu.top

Java: new ArrayList<>(list);
来源：http://kib.uphjek.com

Go:   copied := append([]int(nil), arr...)
来源：http://rbk.jqgfzy.top

Ruby: arr.dup;  arr.clone
来源：http://zji.redwolf501.top

C#:   new List<int>(list);
来源：http://hiy.guannengcc.top

[D23] reduce 累积计算
来源：http://gsh.jlsjyb.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ttj.gzhubu.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pan.hysaishi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jne.sjlbkw.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ttf.fengsongda.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://uuc.yongpay.top

Go:   // 手写循环
来源：http://laj.hongshengwenyu.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://avz.tianlin.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fhs.daria6918.cn

[D24] 字典 / Map 基本操作
来源：http://qfg.andypj.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tmm.wangdashe.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://elh.ydjk.org.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://map.sxryk.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mft.jqgfzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zvf.ehwqpu.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://iok.nanxinkj.top


<!-- 参考信息 -->