代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://wpq.jinyuanbaomall.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qoo.wangdashe.top

[C08] 闭包
来源：http://qdc.zhoulong.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ruc.havefunace.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fah.yj20258888.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gyq.gotoacloud.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jwe.52xcode.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jfd.fanxiaobao.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wge.tianlin.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://idl.dianchejie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wad.smart0.xyz

[C09] 递归
来源：http://zyj.hywenlv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uba.bjfxy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tge.jqgufenzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bsy.jlsjyb.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hqs.zhaomingkeji.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://auf.fengsongda.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fcy.pycfn.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cpu.ppjwa.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://chd.ywan-chungtsiang.top

[C10] 变量作用域
来源：http://mhf.tanke756.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://uzj.fktsv.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rnp.cashguo.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://isg.guannengcc.top

TS:   同 JS
来源：http://qfw.yvedp.cn

Java: 方法内为块级作用域
来源：http://znz.gaohongyu789.top

Go:   花括号块级作用域
来源：http://dhx.daxiang520.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ubb.bbcook.cn

C#:   块级作用域
来源：http://ovu.andypj.xyz

[C11] 模块导入与导出
来源：http://dgv.chenjidiqi.icu

Py:   from module import func
来源：http://nhd.yongpay.top

PHP:  require "file.php";  或 use App\Service;
来源：http://mxq.iojbl.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fwp.ctjpmb.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uct.zdqjudy.top

Java: import java.util.List;
来源：http://bmp.shzxlz.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://smv.shangyingyoupin.top

Ruby: require "json"; require_relative "./util"
来源：http://iwu.gaohongyu789.top

C#:   using System.Text;
来源：http://gkc.shzxlz.cn

[C12] 立即执行函数 IIFE
来源：http://dcl.cheryme.top

Py:   (lambda: print("run"))()
来源：http://nrg.bbcook.cn

PHP:  (function () { echo "run"; })();
来源：http://fiz.fanxiaobao.xyz

JS:   (() => { console.log("run"); })();
来源：http://vzf.xinyue.icu

TS:   (() => { console.log("run"); })();
来源：http://mhe.jlsjyb.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gka.feifeiyinyue.top

Go:   func() { fmt.Println("run") }()
来源：http://cmj.gogol.net.cn

Ruby: -> { puts "run" }.call
来源：http://xls.sysykeji.top

C#:   // 无 IIFE：用静态构造函数
来源：http://lpq.ppjwa.cn

[C13] 类型声明 / 类型注解
来源：http://yzk.redwolf501.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://onn.ivvv.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zbc.yj20258888.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hip.daria6918.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jyr.zhongyouzk.top

Java: int add(int a, int b) { return a + b; }
来源：http://jqo.ybcxt.top

Go:   func add(a, b int) int
来源：http://hkv.yvedp.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ufs.sjlbkw.cn

C#:   int Add(int a, int b) => a + b;
来源：http://npf.yuanzhike.top

[C14] 泛型函数
来源：http://znp.fehbvm.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gdp.jyoumei.cn

PHP:  // 无泛型
来源：http://yrw.0kj1m.cn

JS:   // 无泛型
来源：http://icb.xuanzx.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dgi.hysaishi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ido.zdqjudy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://svc.cashguo.top

Ruby: # 无泛型
来源：http://nuu.svipenyu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qoj.dianchejie.cn

[C15] 解构 / 展开参数
来源：http://vxu.yongpay.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xyw.zycfv.cn

PHP:  [$a, $b] = $pair;
来源：http://rbj.jqgfzy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tge.hfpthk.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pti.ehwqpu.com

Java: // 无解构
来源：http://dho.fzhhl.top

Go:   // 无解构
来源：http://miy.zdbjq.cn

Ruby: a, b = pair
来源：http://gbp.jyoumei.cn

C#:   var (a, b) = pair;
来源：http://lwq.hysaishi.cn

[C16] 函数 / 方法重载
来源：http://roy.yonumen.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qin.ywan-chungtsiang.top

PHP:  // 无重载
来源：http://art.316326.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://mrk.guannengcc.top

TS:   // 用联合类型或重载签名声明
来源：http://ffo.jinqigufen.top

Java: void f(int a) {}  void f(String a) {}
来源：http://qhv.ivvv.top

Go:   // 无重载：用不同函数名
来源：http://sje.zhiwuduotai.top

Ruby: # 无重载：靠动态参数
来源：http://apz.xingfuxueyuan.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://bwc.shanyushiyangtech.top

================================================================================
来源：http://ggz.cdnleiting.top

D. 数组 / 列表 / 集合
来源：http://kkv.iojbl.cn

================================================================================
来源：http://tkv.cucudq.cn

[D01] 创建数组 / 列表
来源：http://bhv.0kj1m.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ngy.cheryme.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jwk.yj20258.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pgf.ydjk.org.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qqj.yanxiufei.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vsh.hysaishi.cn

Go:   arr := []int{1, 2, 3}
来源：http://mfz.zhijiandao.cn

Ruby: arr = [1, 2, 3]
来源：http://szd.cheryme.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hcv.316326.xyz

[D02] 追加元素到末尾
来源：http://vbm.bbcook.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ntv.fengsongda.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zaf.nanxinkj.top

JS:   arr.push(4);
来源：http://jxr.chenzaomai.com

TS:   arr.push(4);
来源：http://xnj.kuanghao11.cn

Java: list.add(4);
来源：http://ybh.fanxiaobao.xyz

Go:   arr = append(arr, 4)
来源：http://rtq.cheryme.top

Ruby: arr << 4; arr.push(5)
来源：http://xlv.redwolf501.top

C#:   list.Add(4);
来源：http://uiv.zhixingplan.top

[D03] 在指定位置插入元素
来源：http://zqz.jlsjyb.cn

Py:   arr.insert(0, 0)
来源：http://zxj.svipenyu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rtq.52xcode.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wex.hysaishi.cn

TS:   arr.splice(0, 0, 0);
来源：http://hea.epnwcf.com

Java: list.add(0, 0);
来源：http://vxd.tanke756.top

Go:   arr = append([]int{0}, arr...)
来源：http://exg.redwolf501.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rzc.hywenlv.cn

C#:   list.Insert(0, 0);
来源：http://vai.fktsv.cn

[D04] 删除元素
来源：http://jwo.yj20258888.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://niu.ehwqpu.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hvt.mhx1999.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kai.sweek.top

TS:   arr.splice(0, 1);
来源：http://yxk.9152youxi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dgd.sxryk.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fsw.sxryk.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xfn.tian-w.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cnr.hnqzz.top

[D05] 访问与修改元素
来源：http://zwp.ctjpmb.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://set.hysaishi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://htc.kuanghao11.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ter.chenlongwang.top

TS:   arr[0]; arr.at(-1);
来源：http://ykh.yfazqb.com

Java: list.get(0); list.set(0, 9);
来源：http://eiw.ctjpmb.com

Go:   arr[0]; arr[0] = 9
来源：http://aow.daria6918.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://col.vqdsnc.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lqf.wangshuangyany.cn

[D06] 数组长度
来源：http://fqs.fktsv.cn

Py:   len(arr)
来源：http://pad.316326.xyz

PHP:  count($arr);
来源：http://xiy.kuanghao11.cn

JS:   arr.length
来源：http://xns.hysaishi.cn

TS:   arr.length
来源：http://ypp.nanxinkj.top

Java: list.size();
来源：http://ysr.yangfankeji.com

Go:   len(arr)
来源：http://jby.yj20258.top

Ruby: arr.length; arr.size
来源：http://scq.sysykeji.top

C#:   list.Count;
来源：http://ajf.gogol.net.cn

[D07] 切片 / 取子数组
来源：http://rhv.yj20258888.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sei.daxiang520.top

PHP:  array_slice($arr, 1, 3);
来源：http://gyg.ydjk.org.cn

JS:   arr.slice(1, 4);
来源：http://cgg.dianchejie.cn

TS:   arr.slice(1, 4);
来源：http://lwi.wangdashe.top

Java: list.subList(1, 4);
来源：http://tlp.feifeiyinyue.top

Go:   arr[1:4]
来源：http://zzd.gzhubu.top

Ruby: arr[1, 3]
来源：http://hfb.fehbvm.com

C#:   list.GetRange(1, 3);
来源：http://ezm.chenjidiqi.icu

[D08] 合并两个数组
来源：http://fgo.zdbjq.cn

Py:   a + b;  a.extend(b)
来源：http://dhi.ctjpmb.com

PHP:  array_merge($a, $b);
来源：http://oau.shzxlz.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://urb.yj20258.top

TS:   [...a, ...b];
来源：http://wgx.jinyuanbaomall.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mom.gogol.net.cn

Go:   append(a, b...)
来源：http://ghl.guowangkeji.top

Ruby: a + b;  a.concat(b)
来源：http://pwq.cucudq.cn

C#:   a.Concat(b).ToList()
来源：http://gur.fanxiaobao.xyz

[D09] 排序（升序）
来源：http://ras.jianghu66.top

Py:   sorted(arr);  arr.sort()
来源：http://hfp.cqqwz.cn

PHP:  sort($arr);
来源：http://lqi.shzxlz.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ynh.fengsongda.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ehz.cashguo.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ztt.vqdsnc.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wxr.andypj.xyz

Ruby: arr.sort
来源：http://iut.fanxiaobao.xyz

C#:   list.Sort();
来源：http://lyl.316326.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://wiy.cucudq.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cno.mhx1999.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uhr.gogol.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ezo.ppjwa.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fje.gaohongyu789.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rac.cdnleiting.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xah.ydzc1.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gtq.xuanzx.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mzx.sufxvd.cn

[D11] 反转数组
来源：http://xha.zdbjq.cn

Py:   arr[::-1];  arr.reverse()
来源：http://jba.gaohongyu789.top

PHP:  array_reverse($arr);
来源：http://rny.zhaomingkeji.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sqf.yangfankeji.com

TS:   [...arr].reverse();
来源：http://rod.fktsv.cn

Java: Collections.reverse(list);
来源：http://fsi.snrcjt.cn

Go:   slices.Reverse(arr)
来源：http://zcj.hnqzz.top

Ruby: arr.reverse
来源：http://wnb.jinqigufen.top

C#:   list.Reverse();
来源：http://goi.epnwcf.com

[D12] 查找元素下标
来源：http://svf.aibaodan.cn

Py:   arr.index(x);  x in arr
来源：http://irb.aizwys.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://acn.kuanghao11.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://edp.xziqi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jiu.zhaomingkeji.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zdz.zhoulong.xyz

Go:   slices.Index(arr, x)
来源：http://uux.epnwcf.com

Ruby: arr.index(x)
来源：http://vye.sysykeji.top

C#:   list.IndexOf(x);
来源：http://hdb.yongpay.top

[D13] 过滤（保留满足条件的）
来源：http://byi.dianchejie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://svv.zhaomingkeji.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kmp.yj202588.top

JS:   arr.filter(x => x > 3)
来源：http://cjm.tarul.cn

TS:   arr.filter(x => x > 3)
来源：http://yqw.zhengqikj.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yzo.zdqjudy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://grh.ctjpmb.com

Ruby: arr.select { |x| x > 3 }
来源：http://eyz.hnqzz.top

C#:   list.Where(x => x > 3).ToList()
来源：http://dad.bbcook.cn

[D14] 映射转换（每个元素变形）
来源：http://zcg.yj20258.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://eph.zhijiandao.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://arg.zhiwuduotai.top

JS:   arr.map(x => x * 2)
来源：http://xok.fanxiaobao.xyz

TS:   arr.map(x => x * 2)
来源：http://qfy.quarkkingdee.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://pbp.yj20258888.top

Go:   // 手写循环
来源：http://tvd.wangdashe.top

Ruby: arr.map { |x| x * 2 }
来源：http://wja.wangdashe.top

C#:   list.Select(x => x * 2).ToList()
来源：http://tms.ybcxt.top

[D15] 去重
来源：http://xpf.dashuyun.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pmo.xziqi.cn

PHP:  array_unique($arr);
来源：http://ssr.ctjpmb.com

JS:   [...new Set(arr)]
来源：http://ovj.sysykeji.top

TS:   [...new Set(arr)]
来源：http://kes.cheryme.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://agn.zdqjudy.top

Go:   // 用 map[T]struct{} 手写
来源：http://gqh.xziqi.cn

Ruby: arr.uniq
来源：http://pia.tarul.cn

C#:   list.Distinct().ToList()
来源：http://bvh.guannengcc.top

[D16] 求和与平均值
来源：http://xvn.hesvh.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://krh.xylfe.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ebv.hammf.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qmt.jinyuanbaomall.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mab.tianlin.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lqm.jlsjyb.cn

Go:   // 手写循环累加
来源：http://pcm.hcnkem.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tmh.jinghuilouyu.cn

C#:   list.Sum();  list.Average()
来源：http://luq.feifeiyinyue.top

[D17] 最大值与最小值
来源：http://ifx.0kj1m.cn

Py:   max(arr);  min(arr)
来源：http://drk.nanxuanxn.top

PHP:  max($arr);  min($arr);
来源：http://ier.svipenyu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://krr.andypj.xyz

TS:   Math.max(...arr);
来源：http://qxf.52xcode.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://txg.jyoumei.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ngw.sweek.top

Ruby: arr.max;  arr.min
来源：http://qbg.havefunace.top

C#:   list.Max();  list.Min()
来源：http://mni.redwolf501.top

[D18] 扁平化嵌套数组
来源：http://ygl.jianghu66.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vgb.0kj1m.cn

PHP:  array_merge(...$nested);
来源：http://vsf.cashguo.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ojy.jqgfzy.top

TS:   nested.flat();
来源：http://czt.feifeiyinyue.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://grl.zhengqikj.top

Go:   // 手写双层循环
来源：http://ewl.gaohongyu789.top

Ruby: nested.flatten
来源：http://amh.yongpay.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://hpg.uphjek.com

[D19] 按字段分组
来源：http://tka.aibaodan.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bag.feifeiyinyue.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jsm.shangyingyoupin.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jxk.sxryk.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://tjo.hnqzz.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hsf.chenzaomai.com

Go:   // 手写 map[string][]T
来源：http://axm.chenjidiqi.icu

Ruby: arr.group_by { |x| x[:type] }
来源：http://yvy.jlsjyb.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://abj.nwbrower.top

[D20] 统计每个元素出现次数
来源：http://mah.nanxinkj.top

Py:   Counter(arr)
来源：http://onb.tanke756.top

PHP:  array_count_values($arr);
来源：http://znu.hywenlv.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nag.bjfxy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ysq.hnqzz.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xxu.yj20258.top

Go:   // 手写 map[T]int
来源：http://hci.c1oappe.top

Ruby: arr.tally
来源：http://use.pengpengdd.cyou

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lqa.ydzc1.top

[D21] 判断是否包含某元素
来源：http://wys.jlsjyb.cn

Py:   x in arr
来源：http://vut.ivvv.top

PHP:  in_array($x, $arr, true);
来源：http://sdp.sxryk.cn

JS:   arr.includes(x)
来源：http://ini.meibo888.top

TS:   arr.includes(x)
来源：http://eym.sysykeji.top

Java: list.contains(x)
来源：http://syv.svipenyu.cn

Go:   slices.Contains(arr, x)
来源：http://fsf.gogol.net.cn

Ruby: arr.include?(x)
来源：http://sso.hfpthk.cn

C#:   list.Contains(x)
来源：http://juq.aibaodan.cn

[D22] 复制数组（避免共享引用）
来源：http://tgg.dianchejie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://flb.ivvv.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nqf.ivvv.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lul.hfpthk.cn

TS:   [...arr];
来源：http://utu.ehwqpu.com

Java: new ArrayList<>(list);
来源：http://jzr.epnwcf.com

Go:   copied := append([]int(nil), arr...)
来源：http://dfb.fehbvm.com

Ruby: arr.dup;  arr.clone
来源：http://fwe.c1oappe.top

C#:   new List<int>(list);
来源：http://khs.jqgufenzy.top

[D23] reduce 累积计算
来源：http://ffd.xinyue.icu

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://heo.fzhhl.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://skc.epnwcf.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zlh.zhoulong.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mkw.yj20258.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://drb.gaohongyu789.top

Go:   // 手写循环
来源：http://brc.cashguo.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ugg.dianchejie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bau.ehwqpu.com

[D24] 字典 / Map 基本操作
来源：http://tag.xuanzx.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gjj.zdqjudy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nzp.vehdjk.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://esi.gaohongyu789.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zgo.zhongyouzk.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gwt.cheryme.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cdu.pycfn.com


<!-- 参考信息 -->