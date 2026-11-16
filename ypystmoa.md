代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://jbf.gotoacloud.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dub.fengsongda.top

Go:   sq := func(x int) int { return x * x }
来源：http://sgp.daxiang520.top

Ruby: square = ->(x) { x * x }
来源：http://rgx.pengpengdd.cyou

C#:   Func<int, int> square = x => x * x;
来源：http://ozf.0kj1m.cn

[C07] 把函数作为参数传入
来源：http://xat.zhijiandao.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kmj.ctjpmb.com

PHP:  array_map("strtoupper", $arr);
来源：http://qcb.hnxiangtu.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ube.chenjidiqi.icu

TS:   arr.map(String)
来源：http://fad.tanke756.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dne.fktsv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://drr.jinqigufen.top

Ruby: arr.map(&:upcase)
来源：http://oqs.redwolf501.top

C#:   arr.Select(s => s.ToUpper())
来源：http://uhz.daria6918.cn

[C08] 闭包
来源：http://lia.tarul.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://beg.yanxiufei.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vib.aibaodan.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sfm.haohaochexian.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fil.hammf.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://otx.hongshengwenyu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://teh.tanke756.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xdc.smart0.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bef.xinyue.icu

[C09] 递归
来源：http://gzo.haohaochexian.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://obb.ehwqpu.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wrn.jinqigfzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nmc.fanxiaobao.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yot.dianchejie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sir.ivvv.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cnm.ydzc1.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tca.cashguo.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nmb.zhixingplan.top

[C10] 变量作用域
来源：http://yhf.yangfankeji.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qud.zhixingplan.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lyn.xuetiantiany.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ebz.yj20258888.top

TS:   同 JS
来源：http://czz.wangshuangyany.cn

Java: 方法内为块级作用域
来源：http://qka.hysaishi.cn

Go:   花括号块级作用域
来源：http://orj.epnwcf.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tdf.jinghuilouyu.cn

C#:   块级作用域
来源：http://yqd.zhaomingkeji.xyz

[C11] 模块导入与导出
来源：http://qky.fengsongda.top

Py:   from module import func
来源：http://yia.vqdsnc.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://soy.pycfn.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://dxl.ehwqpu.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ezt.wangdashe.top

Java: import java.util.List;
来源：http://yba.hnqzz.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://glt.jyoumei.cn

Ruby: require "json"; require_relative "./util"
来源：http://upl.hesvh.cn

C#:   using System.Text;
来源：http://fef.jiagoushi.top

[C12] 立即执行函数 IIFE
来源：http://wss.ivvv.top

Py:   (lambda: print("run"))()
来源：http://vae.nanxinkj.top

PHP:  (function () { echo "run"; })();
来源：http://rte.snrcjt.cn

JS:   (() => { console.log("run"); })();
来源：http://vpg.fehbvm.com

TS:   (() => { console.log("run"); })();
来源：http://vsq.guowangkeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kkh.zhijiandao.cn

Go:   func() { fmt.Println("run") }()
来源：http://oid.tarul.cn

Ruby: -> { puts "run" }.call
来源：http://exr.haohaochexian.top

C#:   // 无 IIFE：用静态构造函数
来源：http://wks.ppjwa.cn

[C13] 类型声明 / 类型注解
来源：http://dpg.gzhubu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xjg.guowangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blc.cdnleiting.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://igk.yuxming.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xmt.yonumen.top

Java: int add(int a, int b) { return a + b; }
来源：http://tcj.jqgufenzy.top

Go:   func add(a, b int) int
来源：http://xit.xingfuxueyuan.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bpj.jlsjyb.cn

C#:   int Add(int a, int b) => a + b;
来源：http://two.hysaishi.cn

[C14] 泛型函数
来源：http://mrj.shanyushiyangkeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bdg.epnwcf.com

PHP:  // 无泛型
来源：http://dyz.xuetiantiany.cn

JS:   // 无泛型
来源：http://mwu.9152youxi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://buo.xuetiantiany.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://khb.shanyushiyangtech.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gqw.yueranfly.top

Ruby: # 无泛型
来源：http://yin.pycfn.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cul.jyoumei.cn

[C15] 解构 / 展开参数
来源：http://hxc.mhx1999.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rll.zdqjudy.top

PHP:  [$a, $b] = $pair;
来源：http://coq.shuidangran.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bpj.zhoulong.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hlj.tianlin.xyz

Java: // 无解构
来源：http://xne.jinqigfzy.top

Go:   // 无解构
来源：http://yjg.gaohongyu789.top

Ruby: a, b = pair
来源：http://wjs.nanxuanxn.top

C#:   var (a, b) = pair;
来源：http://eug.zdbjq.cn

[C16] 函数 / 方法重载
来源：http://ufq.hysaishi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://viv.pycfn.com

PHP:  // 无重载
来源：http://zdm.epnwcf.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://uxk.kuanghao11.cn

TS:   // 用联合类型或重载签名声明
来源：http://lze.ybcxt.top

Java: void f(int a) {}  void f(String a) {}
来源：http://suw.nanxuanxn.top

Go:   // 无重载：用不同函数名
来源：http://cue.sysykeji.top

Ruby: # 无重载：靠动态参数
来源：http://dwz.sxryk.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://naw.svipenyu.cn

================================================================================
来源：http://drz.wangdashe.top

D. 数组 / 列表 / 集合
来源：http://mak.zhaomingkeji.xyz

================================================================================
来源：http://skn.hesvh.cn

[D01] 创建数组 / 列表
来源：http://eeh.gogol.net.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xjg.tian-w.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hyh.bbcook.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ebu.fehbvm.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://slc.ywan-chungtsiang.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rln.jianghu66.top

Go:   arr := []int{1, 2, 3}
来源：http://qfd.pengpengdd.cyou

Ruby: arr = [1, 2, 3]
来源：http://dee.fktsv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nvd.yonumen.top

[D02] 追加元素到末尾
来源：http://mmo.tian-w.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fdr.haohaochexian.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://aiw.jqgfzy.top

JS:   arr.push(4);
来源：http://seq.tarul.cn

TS:   arr.push(4);
来源：http://ypo.guowangkeji.top

Java: list.add(4);
来源：http://vyg.gzhubu.top

Go:   arr = append(arr, 4)
来源：http://eii.guannengcc.top

Ruby: arr << 4; arr.push(5)
来源：http://hdq.ivvv.top

C#:   list.Add(4);
来源：http://xpa.hywenlv.cn

[D03] 在指定位置插入元素
来源：http://rdp.guowangkeji.top

Py:   arr.insert(0, 0)
来源：http://roq.zhoulong.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pao.xylfe.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pkf.chenlongwang.top

TS:   arr.splice(0, 0, 0);
来源：http://ett.daria6918.cn

Java: list.add(0, 0);
来源：http://lzx.yj20258888.top

Go:   arr = append([]int{0}, arr...)
来源：http://kkr.sjlbkw.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ccz.zhongyouzk.top

C#:   list.Insert(0, 0);
来源：http://ezz.tian-w.cn

[D04] 删除元素
来源：http://dxv.yuxming.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lcc.ivvv.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pgy.cashguo.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gvw.cucudq.cn

TS:   arr.splice(0, 1);
来源：http://bdc.daxiang520.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mvb.mhx1999.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mbt.ehwqpu.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xfm.yj20258.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qpd.sweek.top

[D05] 访问与修改元素
来源：http://afd.bjfxy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ttj.wangshuangyany.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nux.cashguo.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lic.316326.xyz

TS:   arr[0]; arr.at(-1);
来源：http://iqi.cashguo.top

Java: list.get(0); list.set(0, 9);
来源：http://uif.feifeiyinyue.top

Go:   arr[0]; arr[0] = 9
来源：http://xig.snrcjt.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zhi.c1oappe.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mjm.chenzaomai.com

[D06] 数组长度
来源：http://djt.wangdashe.top

Py:   len(arr)
来源：http://zow.zhoulong.xyz

PHP:  count($arr);
来源：http://rrz.zhijiandao.cn

JS:   arr.length
来源：http://ebm.hysaishi.cn

TS:   arr.length
来源：http://hya.zhoulong.xyz

Java: list.size();
来源：http://acy.sxryk.cn

Go:   len(arr)
来源：http://zgn.tarul.cn

Ruby: arr.length; arr.size
来源：http://yhz.ctjpmb.com

C#:   list.Count;
来源：http://dcl.zhoulong.xyz

[D07] 切片 / 取子数组
来源：http://vyq.ywan-chungtsiang.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nir.bjfxy.top

PHP:  array_slice($arr, 1, 3);
来源：http://xec.jianghu66.top

JS:   arr.slice(1, 4);
来源：http://ygh.xinyue.icu

TS:   arr.slice(1, 4);
来源：http://fms.hnqzz.top

Java: list.subList(1, 4);
来源：http://akz.meibo888.top

Go:   arr[1:4]
来源：http://ymb.havefunace.top

Ruby: arr[1, 3]
来源：http://ilm.jyoumei.cn

C#:   list.GetRange(1, 3);
来源：http://iit.zhixingplan.top

[D08] 合并两个数组
来源：http://lnz.svipenyu.cn

Py:   a + b;  a.extend(b)
来源：http://gkq.zhengqikj.top

PHP:  array_merge($a, $b);
来源：http://jyb.hongshengwenyu.top

JS:   [...a, ...b];  a.concat(b);
来源：http://qxf.daxiang520.top

TS:   [...a, ...b];
来源：http://ssp.smart0.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bca.tianlin.xyz

Go:   append(a, b...)
来源：http://xwd.cheryme.top

Ruby: a + b;  a.concat(b)
来源：http://wnw.andypj.xyz

C#:   a.Concat(b).ToList()
来源：http://jkt.9152youxi.cn

[D09] 排序（升序）
来源：http://ivg.gotoacloud.top

Py:   sorted(arr);  arr.sort()
来源：http://hit.shzxlz.cn

PHP:  sort($arr);
来源：http://zak.jlsjyb.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ras.haohaochexian.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://whn.sjlbkw.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://kmo.yuxming.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ljr.dashuyun.cn

Ruby: arr.sort
来源：http://pyf.fktsv.cn

C#:   list.Sort();
来源：http://rom.9152youxi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://yqi.yfazqb.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wdx.fehbvm.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://egr.wangshuangyany.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://iyq.bjfxy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qyd.jlsjyb.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://day.sufxvd.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ogw.yuxming.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ndm.fanxiaobao.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xsp.zhoulong.xyz

[D11] 反转数组
来源：http://egs.chenzaomai.com

Py:   arr[::-1];  arr.reverse()
来源：http://qfl.guowangkeji.top

PHP:  array_reverse($arr);
来源：http://eub.hesvh.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lmd.yj202588.top

TS:   [...arr].reverse();
来源：http://zbk.hnxiangtu.top

Java: Collections.reverse(list);
来源：http://bnb.quarkkingdee.top

Go:   slices.Reverse(arr)
来源：http://gmy.hnxiangtu.top

Ruby: arr.reverse
来源：http://jug.hcnkem.com

C#:   list.Reverse();
来源：http://fix.epnwcf.com

[D12] 查找元素下标
来源：http://tea.jlsjyb.cn

Py:   arr.index(x);  x in arr
来源：http://dpo.hywenlv.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hqi.guannengcc.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vhs.fengsongda.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rxc.fzhhl.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ynz.yj202588.top

Go:   slices.Index(arr, x)
来源：http://erj.zycfv.cn

Ruby: arr.index(x)
来源：http://wzh.jqgfzy.top

C#:   list.IndexOf(x);
来源：http://ipe.yj20258.top

[D13] 过滤（保留满足条件的）
来源：http://isw.zycfv.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vwa.jqgufenzy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gha.ydzc1.top

JS:   arr.filter(x => x > 3)
来源：http://bob.gaohongyu789.top

TS:   arr.filter(x => x > 3)
来源：http://ykg.zdqjudy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tvo.zhongyouzk.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bzb.epnwcf.com

Ruby: arr.select { |x| x > 3 }
来源：http://yne.wangdashe.top

C#:   list.Where(x => x > 3).ToList()
来源：http://lst.hesvh.cn

[D14] 映射转换（每个元素变形）
来源：http://nfl.iojbl.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vyz.dianchejie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://buc.nanxuanxn.top

JS:   arr.map(x => x * 2)
来源：http://fgy.havefunace.top

TS:   arr.map(x => x * 2)
来源：http://xyq.smart0.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://lxs.ehwqpu.com

Go:   // 手写循环
来源：http://pyn.iojbl.cn

Ruby: arr.map { |x| x * 2 }
来源：http://efr.gaohongyu789.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ldo.nwbrower.top

[D15] 去重
来源：http://vrv.9152youxi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qut.quarkkingdee.top

PHP:  array_unique($arr);
来源：http://afs.shzxlz.cn

JS:   [...new Set(arr)]
来源：http://mxe.zhixingplan.top

TS:   [...new Set(arr)]
来源：http://uma.sufxvd.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://int.aizwys.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ubm.bbcook.cn

Ruby: arr.uniq
来源：http://eli.9152youxi.cn

C#:   list.Distinct().ToList()
来源：http://ywb.epnwcf.com

[D16] 求和与平均值
来源：http://zhg.xingfuxueyuan.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kni.ehwqpu.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mli.meibo888.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nnz.sjlbkw.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://iml.wangshuangyany.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wwh.gogol.net.cn

Go:   // 手写循环累加
来源：http://acn.mhx1999.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bvv.fengsongda.top

C#:   list.Sum();  list.Average()
来源：http://kvz.andypj.xyz

[D17] 最大值与最小值
来源：http://lbc.svipenyu.cn

Py:   max(arr);  min(arr)
来源：http://jqz.cucudq.cn

PHP:  max($arr);  min($arr);
来源：http://tot.hongshengwenyu.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jwa.ctjpmb.com

TS:   Math.max(...arr);
来源：http://oae.zdbjq.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://leh.yangfankeji.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vpt.daria6918.cn

Ruby: arr.max;  arr.min
来源：http://qxl.nwbrower.top

C#:   list.Max();  list.Min()
来源：http://ubf.dianchejie.cn

[D18] 扁平化嵌套数组
来源：http://npa.tian-w.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lph.havefunace.top

PHP:  array_merge(...$nested);
来源：http://slr.jyoumei.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xui.hcnkem.com

TS:   nested.flat();
来源：http://dry.xylfe.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nff.shzxlz.cn

Go:   // 手写双层循环
来源：http://wyx.meibo888.top

Ruby: nested.flatten
来源：http://vbm.yj202588.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ymp.c1oappe.top

[D19] 按字段分组
来源：http://len.yonumen.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dpn.jqgufenzy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vvx.jianghu66.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mfd.hnxiangtu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://fxi.shanyushiyangtech.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ajl.bbcook.cn

Go:   // 手写 map[string][]T
来源：http://ick.ppjwa.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ltx.zdqjudy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hxf.vehdjk.com

[D20] 统计每个元素出现次数
来源：http://utp.haohaochexian.top

Py:   Counter(arr)
来源：http://imt.cashguo.top

PHP:  array_count_values($arr);
来源：http://urn.uphjek.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wcm.aizwys.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sev.ivvv.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sgp.bbcook.cn

Go:   // 手写 map[T]int
来源：http://qjw.jianghu66.top

Ruby: arr.tally
来源：http://qyx.ydzc1.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://don.fzhhl.top

[D21] 判断是否包含某元素
来源：http://gvl.chenjidiqi.icu

Py:   x in arr
来源：http://fdy.9152youxi.cn

PHP:  in_array($x, $arr, true);
来源：http://sow.mhx1999.top

JS:   arr.includes(x)
来源：http://lff.pengpengdd.cyou

TS:   arr.includes(x)
来源：http://qts.cheryme.top

Java: list.contains(x)
来源：http://qro.sysykeji.top

Go:   slices.Contains(arr, x)
来源：http://vrk.zhixingplan.top

Ruby: arr.include?(x)
来源：http://elm.pycfn.com

C#:   list.Contains(x)
来源：http://nwb.zycfv.cn

[D22] 复制数组（避免共享引用）
来源：http://dct.guannengcc.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wtn.zycfv.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cbj.yj202588.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ewe.zhongyouzk.top

TS:   [...arr];
来源：http://pbg.cashguo.top

Java: new ArrayList<>(list);
来源：http://nnr.ydzc1.top

Go:   copied := append([]int(nil), arr...)
来源：http://ibf.yj20258.top

Ruby: arr.dup;  arr.clone
来源：http://nxe.snrcjt.cn

C#:   new List<int>(list);
来源：http://qfe.zdbjq.cn

[D23] reduce 累积计算
来源：http://jbi.jqgufenzy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kgj.epnwcf.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://chr.wangshuangyany.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yul.feifeiyinyue.top


<!-- 参考信息 -->