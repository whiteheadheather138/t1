代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://bva.0kj1m.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ykl.iojbl.cn

[C08] 闭包
来源：http://jdq.xuanzx.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://heb.hnxiangtu.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ryv.ctjpmb.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kcs.hcnkem.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pfy.ivvv.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fle.zdbjq.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jwf.zhaomingkeji.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xhk.chenzaomai.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dyh.chenzaomai.com

[C09] 递归
来源：http://itm.yueranfly.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ihx.cucudq.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xil.mhx1999.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yqj.jinghuilouyu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ghu.yueranfly.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qty.sjlbkw.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uta.hesvh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yme.jiagoushi.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://udt.yuxming.cn

[C10] 变量作用域
来源：http://ryd.jqgufenzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qqf.yj20258.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://sei.zhixingplan.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://shs.zycfv.cn

TS:   同 JS
来源：http://gby.zhengqikj.top

Java: 方法内为块级作用域
来源：http://vrx.shzxlz.cn

Go:   花括号块级作用域
来源：http://vxr.jiagoushi.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sdm.dianchejie.cn

C#:   块级作用域
来源：http://ook.hcnkem.com

[C11] 模块导入与导出
来源：http://wjm.fktsv.cn

Py:   from module import func
来源：http://ukf.gzhubu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://xra.zhengqikj.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://tdb.nanxinkj.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ljx.hfpthk.cn

Java: import java.util.List;
来源：http://beb.jiagoushi.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hny.zhixingplan.top

Ruby: require "json"; require_relative "./util"
来源：http://mni.fanxiaobao.xyz

C#:   using System.Text;
来源：http://dtj.chenzaomai.com

[C12] 立即执行函数 IIFE
来源：http://yey.cqqwz.cn

Py:   (lambda: print("run"))()
来源：http://gao.vqdsnc.cn

PHP:  (function () { echo "run"; })();
来源：http://gjs.ywan-chungtsiang.top

JS:   (() => { console.log("run"); })();
来源：http://qce.fengsongda.top

TS:   (() => { console.log("run"); })();
来源：http://fud.wangdashe.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hdc.jinyuanbaomall.cn

Go:   func() { fmt.Println("run") }()
来源：http://jva.316326.xyz

Ruby: -> { puts "run" }.call
来源：http://ijv.pycfn.com

C#:   // 无 IIFE：用静态构造函数
来源：http://yse.shanyushiyangkeji.top

[C13] 类型声明 / 类型注解
来源：http://jea.ivvv.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vbt.tian-w.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ptj.dashuyun.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://niy.pycfn.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ems.iojbl.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fei.yangfankeji.com

Go:   func add(a, b int) int
来源：http://xxy.0kj1m.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kjt.tian-w.cn

C#:   int Add(int a, int b) => a + b;
来源：http://uld.sxryk.cn

[C14] 泛型函数
来源：http://qum.fanxiaobao.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nsa.xuetiantiany.cn

PHP:  // 无泛型
来源：http://xug.zhijiandao.cn

JS:   // 无泛型
来源：http://dmy.jiagoushi.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zmc.hesvh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sah.guannengcc.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ioa.chenzaomai.com

Ruby: # 无泛型
来源：http://lvp.zhijiandao.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hqm.guannengcc.top

[C15] 解构 / 展开参数
来源：http://iiv.zhongyouzk.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sza.mhx1999.top

PHP:  [$a, $b] = $pair;
来源：http://kns.jinyuanbaomall.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ewm.xylfe.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cnz.shzxlz.cn

Java: // 无解构
来源：http://aqr.jlsjyb.cn

Go:   // 无解构
来源：http://yjw.yueranfly.top

Ruby: a, b = pair
来源：http://eyc.fzhhl.top

C#:   var (a, b) = pair;
来源：http://llo.yvedp.cn

[C16] 函数 / 方法重载
来源：http://mlm.zhixingplan.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qtc.jlsjyb.cn

PHP:  // 无重载
来源：http://lsi.zdqjudy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://wpl.iojbl.cn

TS:   // 用联合类型或重载签名声明
来源：http://cwt.fktsv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://aqi.xingfuxueyuan.xyz

Go:   // 无重载：用不同函数名
来源：http://muc.redwolf501.top

Ruby: # 无重载：靠动态参数
来源：http://duy.andypj.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://loy.xinyue.icu

================================================================================
来源：http://ujl.hnxiangtu.top

D. 数组 / 列表 / 集合
来源：http://dvt.c1oappe.top

================================================================================
来源：http://ono.bbcook.cn

[D01] 创建数组 / 列表
来源：http://hga.sufxvd.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wvn.yj20258.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lje.iojbl.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xzu.snrcjt.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://pgr.epnwcf.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lqg.dashuyun.cn

Go:   arr := []int{1, 2, 3}
来源：http://zdb.hesvh.cn

Ruby: arr = [1, 2, 3]
来源：http://ras.hammf.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://eac.sysykeji.top

[D02] 追加元素到末尾
来源：http://icj.tianlin.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ylu.havefunace.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xyq.aizwys.cn

JS:   arr.push(4);
来源：http://bbp.gaohongyu789.top

TS:   arr.push(4);
来源：http://qhx.shzxlz.cn

Java: list.add(4);
来源：http://vbk.ivvv.top

Go:   arr = append(arr, 4)
来源：http://qaa.feifeiyinyue.top

Ruby: arr << 4; arr.push(5)
来源：http://sbi.tarul.cn

C#:   list.Add(4);
来源：http://slr.tian-w.cn

[D03] 在指定位置插入元素
来源：http://tpd.aibaodan.cn

Py:   arr.insert(0, 0)
来源：http://odu.ywan-chungtsiang.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mbt.zdqjudy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wbg.zhiwuduotai.top

TS:   arr.splice(0, 0, 0);
来源：http://kcl.ppjwa.cn

Java: list.add(0, 0);
来源：http://hcl.quarkkingdee.top

Go:   arr = append([]int{0}, arr...)
来源：http://eaj.shzxlz.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gfx.ydzc1.top

C#:   list.Insert(0, 0);
来源：http://ggw.andypj.xyz

[D04] 删除元素
来源：http://ytk.nwbrower.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vqa.jinqigufen.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hoy.daxiang520.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zxi.tarul.cn

TS:   arr.splice(0, 1);
来源：http://bdt.hnxiangtu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zpm.fehbvm.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://glm.dianchejie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://viq.zhiwuduotai.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ifk.pycfn.com

[D05] 访问与修改元素
来源：http://fry.shanyushiyangkeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pfq.jyoumei.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ara.jinqigfzy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dig.xingfuxueyuan.xyz

TS:   arr[0]; arr.at(-1);
来源：http://tge.ivvv.top

Java: list.get(0); list.set(0, 9);
来源：http://kio.sysykeji.top

Go:   arr[0]; arr[0] = 9
来源：http://jrm.yuanzhike.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wqf.dianchejie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://exy.cucudq.cn

[D06] 数组长度
来源：http://lsd.xingfuxueyuan.xyz

Py:   len(arr)
来源：http://iir.nanxinkj.top

PHP:  count($arr);
来源：http://uxz.jlsjyb.cn

JS:   arr.length
来源：http://rcg.gogol.net.cn

TS:   arr.length
来源：http://lzd.vehdjk.com

Java: list.size();
来源：http://lhs.iojbl.cn

Go:   len(arr)
来源：http://fuj.xuanzx.com

Ruby: arr.length; arr.size
来源：http://sgr.havefunace.top

C#:   list.Count;
来源：http://ygk.uphjek.com

[D07] 切片 / 取子数组
来源：http://div.tarul.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://isn.quarkkingdee.top

PHP:  array_slice($arr, 1, 3);
来源：http://qfa.jinqigufen.top

JS:   arr.slice(1, 4);
来源：http://xrd.yj20258888.top

TS:   arr.slice(1, 4);
来源：http://cwk.fanxiaobao.xyz

Java: list.subList(1, 4);
来源：http://flg.yongpay.top

Go:   arr[1:4]
来源：http://vhj.fengsongda.top

Ruby: arr[1, 3]
来源：http://vqv.fktsv.cn

C#:   list.GetRange(1, 3);
来源：http://ksq.ydjk.org.cn

[D08] 合并两个数组
来源：http://nmo.zhongyouzk.top

Py:   a + b;  a.extend(b)
来源：http://syl.zycfv.cn

PHP:  array_merge($a, $b);
来源：http://mqw.xingfuxueyuan.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://rpa.haohaochexian.top

TS:   [...a, ...b];
来源：http://hpx.ywan-chungtsiang.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zat.gotoacloud.top

Go:   append(a, b...)
来源：http://sju.jqgufenzy.top

Ruby: a + b;  a.concat(b)
来源：http://nri.zhengqikj.top

C#:   a.Concat(b).ToList()
来源：http://mgq.yvedp.cn

[D09] 排序（升序）
来源：http://hhl.wangshuangyany.cn

Py:   sorted(arr);  arr.sort()
来源：http://eog.tianlin.xyz

PHP:  sort($arr);
来源：http://yyq.meibo888.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://swe.guowangkeji.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://iap.yuanzhike.top

Java: Collections.sort(list);  list.sort(null);
来源：http://nwc.xingfuxueyuan.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jmu.bjfxy.top

Ruby: arr.sort
来源：http://emv.meibo888.top

C#:   list.Sort();
来源：http://kfa.zhongyouzk.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://qyr.guannengcc.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ink.uphjek.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mpf.yangfankeji.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rkb.cqqwz.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oco.52xcode.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://utv.mhx1999.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://owo.wangshuangyany.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://swa.zhixingplan.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vim.dashuyun.cn

[D11] 反转数组
来源：http://bha.ppjwa.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qyc.fzhhl.top

PHP:  array_reverse($arr);
来源：http://hnd.ywan-chungtsiang.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ghm.zhixingplan.top

TS:   [...arr].reverse();
来源：http://rrz.cashguo.top

Java: Collections.reverse(list);
来源：http://hea.ctjpmb.com

Go:   slices.Reverse(arr)
来源：http://aft.c1oappe.top

Ruby: arr.reverse
来源：http://dfb.shangyingyoupin.top

C#:   list.Reverse();
来源：http://fns.sufxvd.cn

[D12] 查找元素下标
来源：http://wta.ppjwa.cn

Py:   arr.index(x);  x in arr
来源：http://ilb.zhijiandao.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zfi.yj20258888.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xkz.cqqwz.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jcm.52xcode.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kwb.vqdsnc.cn

Go:   slices.Index(arr, x)
来源：http://uqf.hnqzz.top

Ruby: arr.index(x)
来源：http://lax.fzhhl.top

C#:   list.IndexOf(x);
来源：http://bsy.pycfn.com

[D13] 过滤（保留满足条件的）
来源：http://enn.bbcook.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fvp.yj20258.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://knk.yj202588.top

JS:   arr.filter(x => x > 3)
来源：http://khd.sufxvd.cn

TS:   arr.filter(x => x > 3)
来源：http://myr.tianlin.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zld.ehwqpu.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://crq.tarul.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ptw.jinqigufen.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ieb.vehdjk.com

[D14] 映射转换（每个元素变形）
来源：http://yxs.0kj1m.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://oda.nanxuanxn.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kmo.yj202588.top

JS:   arr.map(x => x * 2)
来源：http://iqt.fzhhl.top

TS:   arr.map(x => x * 2)
来源：http://vyi.hysaishi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://pls.hysaishi.cn

Go:   // 手写循环
来源：http://nky.hongshengwenyu.top

Ruby: arr.map { |x| x * 2 }
来源：http://avj.ctjpmb.com

C#:   list.Select(x => x * 2).ToList()
来源：http://bfz.ydzc1.top

[D15] 去重
来源：http://ybu.ivvv.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gpj.sxryk.cn

PHP:  array_unique($arr);
来源：http://vmc.sufxvd.cn

JS:   [...new Set(arr)]
来源：http://prh.andypj.xyz

TS:   [...new Set(arr)]
来源：http://yyi.cashguo.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kpx.shanyushiyangkeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://ixh.aizwys.cn

Ruby: arr.uniq
来源：http://bxg.yuanzhike.top

C#:   list.Distinct().ToList()
来源：http://pqk.smart0.xyz

[D16] 求和与平均值
来源：http://kqo.sysykeji.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jol.yueranfly.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bsw.zhongyouzk.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qnr.daxiang520.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qsq.yonumen.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bbm.ywan-chungtsiang.top

Go:   // 手写循环累加
来源：http://hsw.quarkkingdee.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rcf.guowangkeji.top

C#:   list.Sum();  list.Average()
来源：http://ajq.guannengcc.top

[D17] 最大值与最小值
来源：http://nea.iojbl.cn

Py:   max(arr);  min(arr)
来源：http://fjz.ybcxt.top

PHP:  max($arr);  min($arr);
来源：http://ycl.hesvh.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ylx.zhengqikj.top

TS:   Math.max(...arr);
来源：http://wlm.xylfe.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zle.nanxinkj.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vfk.xuanzx.com

Ruby: arr.max;  arr.min
来源：http://jpw.andypj.xyz

C#:   list.Max();  list.Min()
来源：http://nvo.haohaochexian.top

[D18] 扁平化嵌套数组
来源：http://ooi.fehbvm.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tcz.yuanzhike.top

PHP:  array_merge(...$nested);
来源：http://kdy.ctjpmb.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vfr.yfazqb.com

TS:   nested.flat();
来源：http://xko.fanxiaobao.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dbz.sxryk.cn

Go:   // 手写双层循环
来源：http://gik.xinyue.icu

Ruby: nested.flatten
来源：http://wgl.cheryme.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ojk.fanxiaobao.xyz

[D19] 按字段分组
来源：http://txj.yongpay.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pgp.cdnleiting.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://oco.guowangkeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tll.andypj.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://qqz.uphjek.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://auz.fengsongda.top

Go:   // 手写 map[string][]T
来源：http://hxh.nwbrower.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://nfo.aizwys.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jjq.hywenlv.cn

[D20] 统计每个元素出现次数
来源：http://ewx.fanxiaobao.xyz

Py:   Counter(arr)
来源：http://avs.zhoulong.xyz

PHP:  array_count_values($arr);
来源：http://xkp.chenlongwang.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qll.shangyingyoupin.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fym.jinyuanbaomall.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cdw.meibo888.top

Go:   // 手写 map[T]int
来源：http://dho.vehdjk.com

Ruby: arr.tally
来源：http://xgh.52xcode.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jsy.guowangkeji.top

[D21] 判断是否包含某元素
来源：http://mto.0kj1m.cn

Py:   x in arr
来源：http://zas.fengsongda.top

PHP:  in_array($x, $arr, true);
来源：http://nuj.yanxiufei.cn

JS:   arr.includes(x)
来源：http://sxe.shzxlz.cn

TS:   arr.includes(x)
来源：http://vxi.daxiang520.top

Java: list.contains(x)
来源：http://igt.aibaodan.cn

Go:   slices.Contains(arr, x)
来源：http://tyh.hnqzz.top

Ruby: arr.include?(x)
来源：http://hae.ybcxt.top

C#:   list.Contains(x)
来源：http://hvw.quarkkingdee.top

[D22] 复制数组（避免共享引用）
来源：http://htz.xuanzx.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://aig.aibaodan.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qzq.zhengqikj.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ikc.cdnleiting.top

TS:   [...arr];
来源：http://wpb.xylfe.cn

Java: new ArrayList<>(list);
来源：http://ety.jqgfzy.top

Go:   copied := append([]int(nil), arr...)
来源：http://xvt.tanke756.top

Ruby: arr.dup;  arr.clone
来源：http://osv.bbcook.cn

C#:   new List<int>(list);
来源：http://iky.cqqwz.cn

[D23] reduce 累积计算
来源：http://kgq.andypj.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ief.yueranfly.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cqg.hywenlv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://svg.aizwys.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://usz.pengpengdd.cyou

Java: list.stream().reduce(0, Integer::sum)
来源：http://uau.birdmap.top

Go:   // 手写循环
来源：http://its.shuidangran.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rpe.vehdjk.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://akn.yvedp.cn

[D24] 字典 / Map 基本操作
来源：http://jwi.cdnleiting.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uqk.xinyue.icu

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://npn.fehbvm.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://adg.feifeiyinyue.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gan.hnxiangtu.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mbc.shangyingyoupin.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://adk.sweek.top


<!-- 参考信息 -->