代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://gdp.jinqigfzy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://wac.bbcook.cn

[C08] 闭包
来源：http://fbb.hywenlv.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jxs.9152youxi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://iyz.xuetiantiany.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hrq.cashguo.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://iwy.yj20258.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://euk.hnxiangtu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mwi.xuanzx.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vny.dashuyun.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zsp.jqgufenzy.top

[C09] 递归
来源：http://gmd.yj20258888.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://syi.shanyushiyangtech.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://svc.fzhhl.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xxs.ydjk.org.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zeq.pengpengdd.cyou

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ffi.nwbrower.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mky.9152youxi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://omf.52xcode.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pqd.gzhubu.top

[C10] 变量作用域
来源：http://yon.aibaodan.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vce.nanxuanxn.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ucd.cucudq.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kog.shanyushiyangtech.top

TS:   同 JS
来源：http://rgu.jinqigfzy.top

Java: 方法内为块级作用域
来源：http://rke.haohaochexian.top

Go:   花括号块级作用域
来源：http://cjc.hnxiangtu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gid.ywan-chungtsiang.top

C#:   块级作用域
来源：http://zab.shuidangran.top

[C11] 模块导入与导出
来源：http://cnw.0kj1m.cn

Py:   from module import func
来源：http://fid.zhiwuduotai.top

PHP:  require "file.php";  或 use App\Service;
来源：http://caj.xingfuxueyuan.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://fdq.jqgufenzy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yqx.uphjek.com

Java: import java.util.List;
来源：http://utv.yj202588.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lzi.shangyingyoupin.top

Ruby: require "json"; require_relative "./util"
来源：http://opy.jianghu66.top

C#:   using System.Text;
来源：http://prg.zhengqikj.top

[C12] 立即执行函数 IIFE
来源：http://scq.snrcjt.cn

Py:   (lambda: print("run"))()
来源：http://xwt.jinghuilouyu.cn

PHP:  (function () { echo "run"; })();
来源：http://ont.0kj1m.cn

JS:   (() => { console.log("run"); })();
来源：http://dpn.yj202588.top

TS:   (() => { console.log("run"); })();
来源：http://abt.shanyushiyangkeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nbn.svipenyu.cn

Go:   func() { fmt.Println("run") }()
来源：http://zpn.jyoumei.cn

Ruby: -> { puts "run" }.call
来源：http://fua.ydjk.org.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://psu.fanxiaobao.xyz

[C13] 类型声明 / 类型注解
来源：http://geq.tianlin.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ils.chenlongwang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://usp.sysykeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tlm.cheryme.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rmf.yangfankeji.com

Java: int add(int a, int b) { return a + b; }
来源：http://awc.ctjpmb.com

Go:   func add(a, b int) int
来源：http://ufq.fengsongda.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zwd.tianlin.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://rlr.cheryme.top

[C14] 泛型函数
来源：http://kmn.tanke756.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wbl.jlsjyb.cn

PHP:  // 无泛型
来源：http://wyw.nanxinkj.top

JS:   // 无泛型
来源：http://awi.yangfankeji.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://enn.yangfankeji.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fqf.aibaodan.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lij.mhx1999.top

Ruby: # 无泛型
来源：http://kqy.kuanghao11.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jba.vqdsnc.cn

[C15] 解构 / 展开参数
来源：http://cno.snrcjt.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cql.ivvv.top

PHP:  [$a, $b] = $pair;
来源：http://jjs.hfpthk.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zuc.jlsjyb.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ssv.jlsjyb.cn

Java: // 无解构
来源：http://saw.yueranfly.top

Go:   // 无解构
来源：http://tns.xingfuxueyuan.xyz

Ruby: a, b = pair
来源：http://vop.jqgfzy.top

C#:   var (a, b) = pair;
来源：http://ggb.pengpengdd.cyou

[C16] 函数 / 方法重载
来源：http://zfp.ehwqpu.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jsg.hcnkem.com

PHP:  // 无重载
来源：http://dwm.dashuyun.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://nyu.hywenlv.cn

TS:   // 用联合类型或重载签名声明
来源：http://bki.zycfv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://fcj.yj20258888.top

Go:   // 无重载：用不同函数名
来源：http://inj.ehwqpu.com

Ruby: # 无重载：靠动态参数
来源：http://zof.jlsjyb.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mtf.fanxiaobao.xyz

================================================================================
来源：http://lpd.hesvh.cn

D. 数组 / 列表 / 集合
来源：http://rfn.sufxvd.cn

================================================================================
来源：http://efe.tianlin.xyz

[D01] 创建数组 / 列表
来源：http://vmh.tarul.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ooj.hysaishi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yig.chenjidiqi.icu

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dpd.zhaomingkeji.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://swg.guannengcc.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pkf.zycfv.cn

Go:   arr := []int{1, 2, 3}
来源：http://ldd.wangdashe.top

Ruby: arr = [1, 2, 3]
来源：http://ign.mhx1999.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lvj.havefunace.top

[D02] 追加元素到末尾
来源：http://ynq.c1oappe.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vrw.hnxiangtu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qdp.hysaishi.cn

JS:   arr.push(4);
来源：http://bor.zhiwuduotai.top

TS:   arr.push(4);
来源：http://lfo.cheryme.top

Java: list.add(4);
来源：http://qtp.9152youxi.cn

Go:   arr = append(arr, 4)
来源：http://ilh.sxryk.cn

Ruby: arr << 4; arr.push(5)
来源：http://cia.jqgfzy.top

C#:   list.Add(4);
来源：http://kwu.nwbrower.top

[D03] 在指定位置插入元素
来源：http://irl.iojbl.cn

Py:   arr.insert(0, 0)
来源：http://zzv.dianchejie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dvz.yvedp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://naj.wangdashe.top

TS:   arr.splice(0, 0, 0);
来源：http://ffm.gogol.net.cn

Java: list.add(0, 0);
来源：http://nvt.fzhhl.top

Go:   arr = append([]int{0}, arr...)
来源：http://zqx.iojbl.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xtq.yuxming.cn

C#:   list.Insert(0, 0);
来源：http://uuz.hfpthk.cn

[D04] 删除元素
来源：http://pfc.xuetiantiany.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://abf.yj202588.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mdu.c1oappe.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qvi.yuanzhike.top

TS:   arr.splice(0, 1);
来源：http://sfa.ywan-chungtsiang.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qqj.xylfe.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hoc.yueranfly.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yfb.yj20258888.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://llu.xinyue.icu

[D05] 访问与修改元素
来源：http://joy.shzxlz.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zcw.yj202588.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jjk.guannengcc.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bed.yj20258.top

TS:   arr[0]; arr.at(-1);
来源：http://oqv.zhaomingkeji.xyz

Java: list.get(0); list.set(0, 9);
来源：http://dxn.zdqjudy.top

Go:   arr[0]; arr[0] = 9
来源：http://qdd.fehbvm.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cjl.jianghu66.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://apu.yongpay.top

[D06] 数组长度
来源：http://fai.jyoumei.cn

Py:   len(arr)
来源：http://lmj.zhiwuduotai.top

PHP:  count($arr);
来源：http://fsm.yj20258888.top

JS:   arr.length
来源：http://lom.guowangkeji.top

TS:   arr.length
来源：http://wtc.yangfankeji.com

Java: list.size();
来源：http://qwe.bbcook.cn

Go:   len(arr)
来源：http://kfv.sxryk.cn

Ruby: arr.length; arr.size
来源：http://fqj.pengpengdd.cyou

C#:   list.Count;
来源：http://yck.jiagoushi.top

[D07] 切片 / 取子数组
来源：http://ocd.yangfankeji.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ufj.xuetiantiany.cn

PHP:  array_slice($arr, 1, 3);
来源：http://frs.zhijiandao.cn

JS:   arr.slice(1, 4);
来源：http://qzp.ywan-chungtsiang.top

TS:   arr.slice(1, 4);
来源：http://moi.gotoacloud.top

Java: list.subList(1, 4);
来源：http://rxb.zdbjq.cn

Go:   arr[1:4]
来源：http://tkn.zdbjq.cn

Ruby: arr[1, 3]
来源：http://rhi.nanxuanxn.top

C#:   list.GetRange(1, 3);
来源：http://xcy.yuanzhike.top

[D08] 合并两个数组
来源：http://khr.nwbrower.top

Py:   a + b;  a.extend(b)
来源：http://kft.52xcode.cn

PHP:  array_merge($a, $b);
来源：http://nos.haohaochexian.top

JS:   [...a, ...b];  a.concat(b);
来源：http://bgi.shuidangran.top

TS:   [...a, ...b];
来源：http://akh.sxryk.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lui.wangdashe.top

Go:   append(a, b...)
来源：http://bfe.jlsjyb.cn

Ruby: a + b;  a.concat(b)
来源：http://wfp.uphjek.com

C#:   a.Concat(b).ToList()
来源：http://knb.yueranfly.top

[D09] 排序（升序）
来源：http://mnj.jinqigufen.top

Py:   sorted(arr);  arr.sort()
来源：http://mfg.cashguo.top

PHP:  sort($arr);
来源：http://hvm.zhengqikj.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pnu.epnwcf.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://wjx.fanxiaobao.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://ojd.iojbl.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://slr.jinqigufen.top

Ruby: arr.sort
来源：http://krp.tanke756.top

C#:   list.Sort();
来源：http://nug.jqgfzy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://lrf.jiagoushi.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fra.daxiang520.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qku.jiagoushi.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ewe.ydjk.org.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://eoz.xuanzx.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wzn.shzxlz.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cof.redwolf501.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kzk.nanxinkj.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ajw.tianlin.xyz

[D11] 反转数组
来源：http://lmn.hywenlv.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lws.nwbrower.top

PHP:  array_reverse($arr);
来源：http://ecm.wangdashe.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jcg.yj202588.top

TS:   [...arr].reverse();
来源：http://dgp.shuidangran.top

Java: Collections.reverse(list);
来源：http://xlo.xziqi.cn

Go:   slices.Reverse(arr)
来源：http://uwv.meibo888.top

Ruby: arr.reverse
来源：http://bxg.wangshuangyany.cn

C#:   list.Reverse();
来源：http://pgm.ivvv.top

[D12] 查找元素下标
来源：http://ncr.chenjidiqi.icu

Py:   arr.index(x);  x in arr
来源：http://jol.yj20258888.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sqw.bjfxy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tvq.tarul.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dji.hesvh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lhk.snrcjt.cn

Go:   slices.Index(arr, x)
来源：http://tqa.mhx1999.top

Ruby: arr.index(x)
来源：http://qye.ywan-chungtsiang.top

C#:   list.IndexOf(x);
来源：http://blp.cqqwz.cn

[D13] 过滤（保留满足条件的）
来源：http://oha.ybcxt.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cxg.jinqigufen.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dok.xingfuxueyuan.xyz

JS:   arr.filter(x => x > 3)
来源：http://bkh.ppjwa.cn

TS:   arr.filter(x => x > 3)
来源：http://tci.nanxuanxn.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://apn.hnqzz.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kyu.yonumen.top

Ruby: arr.select { |x| x > 3 }
来源：http://gpn.wangshuangyany.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zpz.c1oappe.top

[D14] 映射转换（每个元素变形）
来源：http://vkz.xinyue.icu

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://feg.guannengcc.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ezj.tianlin.xyz

JS:   arr.map(x => x * 2)
来源：http://zoy.haohaochexian.top

TS:   arr.map(x => x * 2)
来源：http://yek.shuidangran.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://yrt.ydjk.org.cn

Go:   // 手写循环
来源：http://lqe.wangshuangyany.cn

Ruby: arr.map { |x| x * 2 }
来源：http://cnj.andypj.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://aun.pengpengdd.cyou

[D15] 去重
来源：http://eck.tanke756.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://htg.hysaishi.cn

PHP:  array_unique($arr);
来源：http://nqz.sufxvd.cn

JS:   [...new Set(arr)]
来源：http://bcq.gaohongyu789.top

TS:   [...new Set(arr)]
来源：http://vwg.haohaochexian.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bes.pengpengdd.cyou

Go:   // 用 map[T]struct{} 手写
来源：http://hme.jinghuilouyu.cn

Ruby: arr.uniq
来源：http://cyj.epnwcf.com

C#:   list.Distinct().ToList()
来源：http://mjr.sysykeji.top

[D16] 求和与平均值
来源：http://iws.shanyushiyangkeji.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://orh.birdmap.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://oii.daria6918.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ipj.ybcxt.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kfh.fehbvm.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bfq.hesvh.cn

Go:   // 手写循环累加
来源：http://tsy.hongshengwenyu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jyi.zhengqikj.top

C#:   list.Sum();  list.Average()
来源：http://hkz.xinyue.icu

[D17] 最大值与最小值
来源：http://lcf.52xcode.cn

Py:   max(arr);  min(arr)
来源：http://lwh.daria6918.cn

PHP:  max($arr);  min($arr);
来源：http://ise.fehbvm.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://drv.hysaishi.cn

TS:   Math.max(...arr);
来源：http://cgs.hywenlv.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ziy.jinghuilouyu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://heh.jinghuilouyu.cn

Ruby: arr.max;  arr.min
来源：http://uzd.ydzc1.top

C#:   list.Max();  list.Min()
来源：http://wwm.zhixingplan.top

[D18] 扁平化嵌套数组
来源：http://xnm.yj20258888.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hzt.sxryk.cn

PHP:  array_merge(...$nested);
来源：http://zzy.shanyushiyangkeji.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lwl.xylfe.cn

TS:   nested.flat();
来源：http://yol.daria6918.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tcs.zhiwuduotai.top

Go:   // 手写双层循环
来源：http://kch.sxryk.cn

Ruby: nested.flatten
来源：http://lom.jinqigfzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://two.shanyushiyangkeji.top

[D19] 按字段分组
来源：http://pfp.ywan-chungtsiang.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://plr.yj202588.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fjj.jqgufenzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jwo.feifeiyinyue.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://vhp.ppjwa.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://umx.zdbjq.cn

Go:   // 手写 map[string][]T
来源：http://eup.guannengcc.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://oqj.daxiang520.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hwn.jqgufenzy.top

[D20] 统计每个元素出现次数
来源：http://ila.zdbjq.cn

Py:   Counter(arr)
来源：http://yoh.hfpthk.cn

PHP:  array_count_values($arr);
来源：http://uji.guannengcc.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ckb.tianlin.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ynj.tianlin.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cje.ctjpmb.com

Go:   // 手写 map[T]int
来源：http://qjl.kuanghao11.cn

Ruby: arr.tally
来源：http://elw.yvedp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://csx.xuanzx.com

[D21] 判断是否包含某元素
来源：http://euj.redwolf501.top

Py:   x in arr
来源：http://cco.jqgufenzy.top

PHP:  in_array($x, $arr, true);
来源：http://fmp.bjfxy.top

JS:   arr.includes(x)
来源：http://lcv.yj20258.top

TS:   arr.includes(x)
来源：http://vks.gotoacloud.top

Java: list.contains(x)
来源：http://wxh.snrcjt.cn

Go:   slices.Contains(arr, x)
来源：http://plq.xuetiantiany.cn

Ruby: arr.include?(x)
来源：http://jyz.zhixingplan.top

C#:   list.Contains(x)
来源：http://cfs.yanxiufei.cn

[D22] 复制数组（避免共享引用）
来源：http://sqe.fengsongda.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wip.jinghuilouyu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mde.wangdashe.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dgt.guowangkeji.top

TS:   [...arr];
来源：http://cta.jianghu66.top

Java: new ArrayList<>(list);
来源：http://acq.ybcxt.top

Go:   copied := append([]int(nil), arr...)
来源：http://rrm.sysykeji.top

Ruby: arr.dup;  arr.clone
来源：http://gph.jinyuanbaomall.cn

C#:   new List<int>(list);
来源：http://hgq.yueranfly.top

[D23] reduce 累积计算
来源：http://vmf.shzxlz.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gxs.dianchejie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://llm.yanxiufei.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rlw.chenjidiqi.icu

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bux.jinghuilouyu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://njl.hesvh.cn

Go:   // 手写循环
来源：http://jxs.ctjpmb.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tag.0kj1m.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ucc.52xcode.cn

[D24] 字典 / Map 基本操作
来源：http://sow.ywan-chungtsiang.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lxn.yangfankeji.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qxh.yj202588.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tes.haohaochexian.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cnz.jyoumei.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fqh.smart0.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://las.xuetiantiany.cn


<!-- 参考信息 -->