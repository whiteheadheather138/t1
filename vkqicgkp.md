代发 wailian999

[C06] 匿名函数 / lambda
来源：http://avd.guannengcc.top

Py:   square = lambda x: x * x
来源：http://tgy.fktsv.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://jle.nanxuanxn.top

JS:   const square = x => x * x;
来源：http://bvt.kuanghao11.cn

TS:   const square = (x: number): number => x * x;
来源：http://jcw.daxiang520.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://owd.fengsongda.top

Go:   sq := func(x int) int { return x * x }
来源：http://pgj.jlsjyb.cn

Ruby: square = ->(x) { x * x }
来源：http://uxo.sxryk.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pts.vehdjk.com

[C07] 把函数作为参数传入
来源：http://uyi.iojbl.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://htn.sweek.top

PHP:  array_map("strtoupper", $arr);
来源：http://cfd.gogol.net.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hei.yuxming.cn

TS:   arr.map(String)
来源：http://lwv.havefunace.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xgk.nanxuanxn.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://amj.fanxiaobao.xyz

Ruby: arr.map(&:upcase)
来源：http://rav.fzhhl.top

C#:   arr.Select(s => s.ToUpper())
来源：http://toz.hnxiangtu.top

[C08] 闭包
来源：http://ubs.tianlin.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uqu.ppjwa.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xdr.sweek.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://prz.mhx1999.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qyz.xuetiantiany.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kcn.yonumen.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kbf.sysykeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gih.xinyue.icu

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://olv.aibaodan.cn

[C09] 递归
来源：http://vkr.c1oappe.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mlu.dianchejie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dbc.aibaodan.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sgz.cashguo.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://isv.yangfankeji.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sjd.zhijiandao.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://unq.shuidangran.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tsc.zhiwuduotai.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jls.shzxlz.cn

[C10] 变量作用域
来源：http://brp.yuanzhike.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tin.sxryk.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hbg.jqgufenzy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wdc.cdnleiting.top

TS:   同 JS
来源：http://efu.hysaishi.cn

Java: 方法内为块级作用域
来源：http://kdl.yj20258888.top

Go:   花括号块级作用域
来源：http://hra.guowangkeji.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mjo.ppjwa.cn

C#:   块级作用域
来源：http://bqg.haohaochexian.top

[C11] 模块导入与导出
来源：http://cqk.tanke756.top

Py:   from module import func
来源：http://ayg.zdqjudy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ypt.jinghuilouyu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://iwb.wangdashe.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rjw.jianghu66.top

Java: import java.util.List;
来源：http://kqv.feifeiyinyue.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://srz.cdnleiting.top

Ruby: require "json"; require_relative "./util"
来源：http://mkn.epnwcf.com

C#:   using System.Text;
来源：http://xwh.yongpay.top

[C12] 立即执行函数 IIFE
来源：http://ivj.guannengcc.top

Py:   (lambda: print("run"))()
来源：http://zru.zhiwuduotai.top

PHP:  (function () { echo "run"; })();
来源：http://jbw.shzxlz.cn

JS:   (() => { console.log("run"); })();
来源：http://rdz.uphjek.com

TS:   (() => { console.log("run"); })();
来源：http://tcz.zycfv.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pom.wangshuangyany.cn

Go:   func() { fmt.Println("run") }()
来源：http://fru.svipenyu.cn

Ruby: -> { puts "run" }.call
来源：http://fcq.vqdsnc.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ona.guannengcc.top

[C13] 类型声明 / 类型注解
来源：http://tjh.jiagoushi.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://iuw.shuidangran.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pvm.xuetiantiany.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tib.yj202588.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mqb.yonumen.top

Java: int add(int a, int b) { return a + b; }
来源：http://aud.cucudq.cn

Go:   func add(a, b int) int
来源：http://yuj.feifeiyinyue.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zwj.yongpay.top

C#:   int Add(int a, int b) => a + b;
来源：http://lhc.zdqjudy.top

[C14] 泛型函数
来源：http://sxh.sxryk.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ezc.fzhhl.top

PHP:  // 无泛型
来源：http://nls.yj20258.top

JS:   // 无泛型
来源：http://xbm.yvedp.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jlh.smart0.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rli.quarkkingdee.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dbj.yuanzhike.top

Ruby: # 无泛型
来源：http://qeh.ppjwa.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nli.fzhhl.top

[C15] 解构 / 展开参数
来源：http://zdv.vqdsnc.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zzt.jinghuilouyu.cn

PHP:  [$a, $b] = $pair;
来源：http://rpd.jyoumei.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uhl.jinghuilouyu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ype.nanxuanxn.top

Java: // 无解构
来源：http://rrh.fengsongda.top

Go:   // 无解构
来源：http://gtr.fktsv.cn

Ruby: a, b = pair
来源：http://wwu.bjfxy.top

C#:   var (a, b) = pair;
来源：http://iyl.tanke756.top

[C16] 函数 / 方法重载
来源：http://xml.9152youxi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://uhx.fktsv.cn

PHP:  // 无重载
来源：http://tna.tarul.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ezj.sjlbkw.cn

TS:   // 用联合类型或重载签名声明
来源：http://hdq.daxiang520.top

Java: void f(int a) {}  void f(String a) {}
来源：http://thg.ppjwa.cn

Go:   // 无重载：用不同函数名
来源：http://bik.daxiang520.top

Ruby: # 无重载：靠动态参数
来源：http://bbj.chenjidiqi.icu

C#:   void F(int a) {}  void F(string a) {}
来源：http://zxx.cucudq.cn

================================================================================
来源：http://xjx.316326.xyz

D. 数组 / 列表 / 集合
来源：http://hpr.meibo888.top

================================================================================
来源：http://ewo.zhengqikj.top

[D01] 创建数组 / 列表
来源：http://ujt.mhx1999.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://cqf.hammf.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lxf.gogol.net.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ntp.shanyushiyangkeji.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://mhp.snrcjt.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qmv.shanyushiyangkeji.top

Go:   arr := []int{1, 2, 3}
来源：http://ccw.316326.xyz

Ruby: arr = [1, 2, 3]
来源：http://mgf.meibo888.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gia.shuidangran.top

[D02] 追加元素到末尾
来源：http://wnq.hesvh.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jlk.daria6918.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://omo.chenzaomai.com

JS:   arr.push(4);
来源：http://ffl.zhijiandao.cn

TS:   arr.push(4);
来源：http://vfg.zhijiandao.cn

Java: list.add(4);
来源：http://avn.hongshengwenyu.top

Go:   arr = append(arr, 4)
来源：http://eff.redwolf501.top

Ruby: arr << 4; arr.push(5)
来源：http://qxa.xuetiantiany.cn

C#:   list.Add(4);
来源：http://fes.daxiang520.top

[D03] 在指定位置插入元素
来源：http://ppd.kuanghao11.cn

Py:   arr.insert(0, 0)
来源：http://wxr.feifeiyinyue.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lxx.316326.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dao.shangyingyoupin.top

TS:   arr.splice(0, 0, 0);
来源：http://lkf.kuanghao11.cn

Java: list.add(0, 0);
来源：http://cds.gotoacloud.top

Go:   arr = append([]int{0}, arr...)
来源：http://uod.hfpthk.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uwe.smart0.xyz

C#:   list.Insert(0, 0);
来源：http://vur.dashuyun.cn

[D04] 删除元素
来源：http://ajp.cucudq.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ikr.hesvh.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fla.bbcook.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ifp.daria6918.cn

TS:   arr.splice(0, 1);
来源：http://ara.pengpengdd.cyou

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ipw.iojbl.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rsi.tanke756.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dxf.zhixingplan.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gty.sweek.top

[D05] 访问与修改元素
来源：http://nol.52xcode.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qvd.sweek.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://oin.xingfuxueyuan.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://iee.dianchejie.cn

TS:   arr[0]; arr.at(-1);
来源：http://asc.hcnkem.com

Java: list.get(0); list.set(0, 9);
来源：http://hqc.vqdsnc.cn

Go:   arr[0]; arr[0] = 9
来源：http://jht.hesvh.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lrj.quarkkingdee.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wii.shangyingyoupin.top

[D06] 数组长度
来源：http://dkn.daxiang520.top

Py:   len(arr)
来源：http://txf.ydzc1.top

PHP:  count($arr);
来源：http://duh.shanyushiyangtech.top

JS:   arr.length
来源：http://llk.quarkkingdee.top

TS:   arr.length
来源：http://ugm.cashguo.top

Java: list.size();
来源：http://krt.hcnkem.com

Go:   len(arr)
来源：http://kqj.yueranfly.top

Ruby: arr.length; arr.size
来源：http://ijk.hnqzz.top

C#:   list.Count;
来源：http://grn.hysaishi.cn

[D07] 切片 / 取子数组
来源：http://kny.andypj.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zjm.c1oappe.top

PHP:  array_slice($arr, 1, 3);
来源：http://trr.xziqi.cn

JS:   arr.slice(1, 4);
来源：http://tgi.wangdashe.top

TS:   arr.slice(1, 4);
来源：http://mza.c1oappe.top

Java: list.subList(1, 4);
来源：http://vyz.jlsjyb.cn

Go:   arr[1:4]
来源：http://pgd.nwbrower.top

Ruby: arr[1, 3]
来源：http://vce.ivvv.top

C#:   list.GetRange(1, 3);
来源：http://hur.nwbrower.top

[D08] 合并两个数组
来源：http://piw.yvedp.cn

Py:   a + b;  a.extend(b)
来源：http://sez.xylfe.cn

PHP:  array_merge($a, $b);
来源：http://ony.fzhhl.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wmr.xylfe.cn

TS:   [...a, ...b];
来源：http://nct.xuanzx.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ipa.snrcjt.cn

Go:   append(a, b...)
来源：http://keh.jinghuilouyu.cn

Ruby: a + b;  a.concat(b)
来源：http://awr.xinyue.icu

C#:   a.Concat(b).ToList()
来源：http://ioj.tarul.cn

[D09] 排序（升序）
来源：http://bev.ivvv.top

Py:   sorted(arr);  arr.sort()
来源：http://brj.uphjek.com

PHP:  sort($arr);
来源：http://xiy.hcnkem.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://udc.meibo888.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://xtj.jiagoushi.top

Java: Collections.sort(list);  list.sort(null);
来源：http://hsu.ydjk.org.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vtv.0kj1m.cn

Ruby: arr.sort
来源：http://oiv.jyoumei.cn

C#:   list.Sort();
来源：http://qqc.jinqigfzy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ady.yvedp.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pog.xuanzx.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://juw.bbcook.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tho.hcnkem.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xyj.sufxvd.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pqb.cucudq.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kli.hammf.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qab.cdnleiting.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rhf.vehdjk.com

[D11] 反转数组
来源：http://ftn.nanxuanxn.top

Py:   arr[::-1];  arr.reverse()
来源：http://dcg.dashuyun.cn

PHP:  array_reverse($arr);
来源：http://yoc.yvedp.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://toy.c1oappe.top

TS:   [...arr].reverse();
来源：http://iqj.ywan-chungtsiang.top

Java: Collections.reverse(list);
来源：http://uqy.jqgfzy.top

Go:   slices.Reverse(arr)
来源：http://jdq.tarul.cn

Ruby: arr.reverse
来源：http://ldd.tarul.cn

C#:   list.Reverse();
来源：http://tcl.yongpay.top

[D12] 查找元素下标
来源：http://dtm.meibo888.top

Py:   arr.index(x);  x in arr
来源：http://kar.sxryk.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nvh.jianghu66.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://enp.xylfe.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gmj.yj202588.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pju.hnxiangtu.top

Go:   slices.Index(arr, x)
来源：http://wka.ppjwa.cn

Ruby: arr.index(x)
来源：http://sur.birdmap.top

C#:   list.IndexOf(x);
来源：http://vav.cqqwz.cn

[D13] 过滤（保留满足条件的）
来源：http://byh.aibaodan.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ehu.bbcook.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cts.yvedp.cn

JS:   arr.filter(x => x > 3)
来源：http://lqc.hfpthk.cn

TS:   arr.filter(x => x > 3)
来源：http://qzs.kuanghao11.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cwa.quarkkingdee.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mlz.jinqigufen.top

Ruby: arr.select { |x| x > 3 }
来源：http://noc.feifeiyinyue.top

C#:   list.Where(x => x > 3).ToList()
来源：http://bzf.haohaochexian.top

[D14] 映射转换（每个元素变形）
来源：http://fej.hysaishi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xdc.xuanzx.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cvg.zdbjq.cn

JS:   arr.map(x => x * 2)
来源：http://cfl.smart0.xyz

TS:   arr.map(x => x * 2)
来源：http://zyu.zdbjq.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://llv.vqdsnc.cn

Go:   // 手写循环
来源：http://ded.jinqigufen.top

Ruby: arr.map { |x| x * 2 }
来源：http://jbn.hongshengwenyu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://wvx.tanke756.top

[D15] 去重
来源：http://akc.shanyushiyangkeji.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tzj.zhengqikj.top

PHP:  array_unique($arr);
来源：http://shj.gotoacloud.top

JS:   [...new Set(arr)]
来源：http://puv.zdbjq.cn

TS:   [...new Set(arr)]
来源：http://xdb.xuetiantiany.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jin.quarkkingdee.top

Go:   // 用 map[T]struct{} 手写
来源：http://hjk.yvedp.cn

Ruby: arr.uniq
来源：http://rkg.shanyushiyangtech.top

C#:   list.Distinct().ToList()
来源：http://qgz.pycfn.com

[D16] 求和与平均值
来源：http://phb.gogol.net.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mum.hongshengwenyu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://egl.yangfankeji.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vof.bbcook.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://niz.chenjidiqi.icu

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://snd.meibo888.top

Go:   // 手写循环累加
来源：http://drm.xingfuxueyuan.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://udx.jinqigfzy.top

C#:   list.Sum();  list.Average()
来源：http://hbz.cheryme.top

[D17] 最大值与最小值
来源：http://zsp.gzhubu.top

Py:   max(arr);  min(arr)
来源：http://gda.c1oappe.top

PHP:  max($arr);  min($arr);
来源：http://get.zhongyouzk.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://okd.aizwys.cn

TS:   Math.max(...arr);
来源：http://fmq.shanyushiyangkeji.top

Java: Collections.max(list);  Collections.min(list);
来源：http://plq.sxryk.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://owm.yonumen.top

Ruby: arr.max;  arr.min
来源：http://gru.yueranfly.top

C#:   list.Max();  list.Min()
来源：http://cjn.ywan-chungtsiang.top

[D18] 扁平化嵌套数组
来源：http://ysw.smart0.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hpz.fzhhl.top

PHP:  array_merge(...$nested);
来源：http://fim.yj20258888.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hxx.hesvh.cn

TS:   nested.flat();
来源：http://gko.zhijiandao.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gtv.shzxlz.cn

Go:   // 手写双层循环
来源：http://git.jlsjyb.cn

Ruby: nested.flatten
来源：http://kva.guowangkeji.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://lhy.yuanzhike.top

[D19] 按字段分组
来源：http://kqz.nanxinkj.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://alg.xingfuxueyuan.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://iiy.shanyushiyangtech.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hzj.nwbrower.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://zbm.hcnkem.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tpd.zhongyouzk.top

Go:   // 手写 map[string][]T
来源：http://tnm.gzhubu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://fcz.jianghu66.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fgj.yongpay.top

[D20] 统计每个元素出现次数
来源：http://bke.jqgufenzy.top

Py:   Counter(arr)
来源：http://zje.yongpay.top

PHP:  array_count_values($arr);
来源：http://rkc.shangyingyoupin.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qgd.uphjek.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vyw.c1oappe.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dky.hnqzz.top

Go:   // 手写 map[T]int
来源：http://yra.iojbl.cn

Ruby: arr.tally
来源：http://qgc.andypj.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yhl.yuanzhike.top

[D21] 判断是否包含某元素
来源：http://bfi.fanxiaobao.xyz

Py:   x in arr
来源：http://vmj.snrcjt.cn

PHP:  in_array($x, $arr, true);
来源：http://qis.jinyuanbaomall.cn

JS:   arr.includes(x)
来源：http://dfl.cashguo.top

TS:   arr.includes(x)
来源：http://nrw.pengpengdd.cyou

Java: list.contains(x)
来源：http://znk.epnwcf.com

Go:   slices.Contains(arr, x)
来源：http://nmk.yonumen.top

Ruby: arr.include?(x)
来源：http://wqq.zhaomingkeji.xyz

C#:   list.Contains(x)
来源：http://rkw.0kj1m.cn

[D22] 复制数组（避免共享引用）
来源：http://ofx.chenzaomai.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://phl.cucudq.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ldx.cashguo.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kkr.fehbvm.com

TS:   [...arr];
来源：http://bkq.meibo888.top

Java: new ArrayList<>(list);
来源：http://swt.xuetiantiany.cn

Go:   copied := append([]int(nil), arr...)
来源：http://sdv.jianghu66.top

Ruby: arr.dup;  arr.clone
来源：http://nzd.zhengqikj.top

C#:   new List<int>(list);
来源：http://fia.zycfv.cn


<!-- 参考信息 -->