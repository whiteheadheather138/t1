代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://soe.redwolf501.top

Go:   return a, b
来源：http://xbo.jinyuanbaomall.cn

Ruby: return a, b
来源：http://wry.xylfe.cn

C#:   return (a, b);              // ValueTuple
来源：http://ral.sxryk.cn

[C06] 匿名函数 / lambda
来源：http://kxa.sysykeji.top

Py:   square = lambda x: x * x
来源：http://pns.hysaishi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://tzt.hnqzz.top

JS:   const square = x => x * x;
来源：http://dtk.chenlongwang.top

TS:   const square = (x: number): number => x * x;
来源：http://mjm.jyoumei.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mts.hcnkem.com

Go:   sq := func(x int) int { return x * x }
来源：http://utx.bjfxy.top

Ruby: square = ->(x) { x * x }
来源：http://mvl.hongshengwenyu.top

C#:   Func<int, int> square = x => x * x;
来源：http://ysd.zhiwuduotai.top

[C07] 把函数作为参数传入
来源：http://vit.shzxlz.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ykn.shanyushiyangtech.top

PHP:  array_map("strtoupper", $arr);
来源：http://tja.hysaishi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lqw.cdnleiting.top

TS:   arr.map(String)
来源：http://oel.zhixingplan.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lqy.pengpengdd.cyou

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kcz.yj20258888.top

Ruby: arr.map(&:upcase)
来源：http://xvj.yj202588.top

C#:   arr.Select(s => s.ToUpper())
来源：http://new.iojbl.cn

[C08] 闭包
来源：http://kac.bbcook.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ujy.jinqigufen.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://het.sjlbkw.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://msg.yfazqb.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tvs.havefunace.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qoc.jinqigufen.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mwh.yangfankeji.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tlh.52xcode.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qpd.pycfn.com

[C09] 递归
来源：http://oqk.dashuyun.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://oio.fzhhl.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mvw.kuanghao11.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tbi.ywan-chungtsiang.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eps.zhiwuduotai.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://snn.chenlongwang.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hcl.gogol.net.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gbi.sufxvd.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yig.jianghu66.top

[C10] 变量作用域
来源：http://yby.tian-w.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://joi.hywenlv.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://oas.yonumen.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xbv.ydjk.org.cn

TS:   同 JS
来源：http://qxw.daria6918.cn

Java: 方法内为块级作用域
来源：http://cdt.zycfv.cn

Go:   花括号块级作用域
来源：http://kex.aizwys.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://efr.zdbjq.cn

C#:   块级作用域
来源：http://pxq.zycfv.cn

[C11] 模块导入与导出
来源：http://xjo.gzhubu.top

Py:   from module import func
来源：http://uct.aibaodan.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ytp.zhixingplan.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://lfy.epnwcf.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hxf.zhixingplan.top

Java: import java.util.List;
来源：http://tio.zhijiandao.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jwp.jqgufenzy.top

Ruby: require "json"; require_relative "./util"
来源：http://oay.feifeiyinyue.top

C#:   using System.Text;
来源：http://zmx.0kj1m.cn

[C12] 立即执行函数 IIFE
来源：http://vjt.quarkkingdee.top

Py:   (lambda: print("run"))()
来源：http://aps.fktsv.cn

PHP:  (function () { echo "run"; })();
来源：http://kxj.aibaodan.cn

JS:   (() => { console.log("run"); })();
来源：http://kxd.zycfv.cn

TS:   (() => { console.log("run"); })();
来源：http://kje.vehdjk.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rjv.tarul.cn

Go:   func() { fmt.Println("run") }()
来源：http://obu.xuetiantiany.cn

Ruby: -> { puts "run" }.call
来源：http://wek.yfazqb.com

C#:   // 无 IIFE：用静态构造函数
来源：http://njq.shuidangran.top

[C13] 类型声明 / 类型注解
来源：http://toe.hysaishi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yto.jyoumei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xks.tanke756.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://csh.iojbl.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wxz.ydzc1.top

Java: int add(int a, int b) { return a + b; }
来源：http://mxh.epnwcf.com

Go:   func add(a, b int) int
来源：http://hgy.hywenlv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lin.hfpthk.cn

C#:   int Add(int a, int b) => a + b;
来源：http://api.jiagoushi.top

[C14] 泛型函数
来源：http://cml.uphjek.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kpu.fehbvm.com

PHP:  // 无泛型
来源：http://ifq.vehdjk.com

JS:   // 无泛型
来源：http://hgg.hfpthk.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://klz.c1oappe.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gft.9152youxi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dib.yfazqb.com

Ruby: # 无泛型
来源：http://zkz.jinqigufen.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://plz.ehwqpu.com

[C15] 解构 / 展开参数
来源：http://azx.sxryk.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nsn.nanxinkj.top

PHP:  [$a, $b] = $pair;
来源：http://ihx.hywenlv.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wwg.haohaochexian.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tok.snrcjt.cn

Java: // 无解构
来源：http://wwr.hnqzz.top

Go:   // 无解构
来源：http://cqg.wangshuangyany.cn

Ruby: a, b = pair
来源：http://zdi.gotoacloud.top

C#:   var (a, b) = pair;
来源：http://ycw.sysykeji.top

[C16] 函数 / 方法重载
来源：http://nxx.xylfe.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rfk.zhaomingkeji.xyz

PHP:  // 无重载
来源：http://tfh.zhoulong.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://ogj.xylfe.cn

TS:   // 用联合类型或重载签名声明
来源：http://wse.vqdsnc.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://axo.cheryme.top

Go:   // 无重载：用不同函数名
来源：http://mje.sxryk.cn

Ruby: # 无重载：靠动态参数
来源：http://ysr.zhixingplan.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://wbh.jiagoushi.top

================================================================================
来源：http://pds.iojbl.cn

D. 数组 / 列表 / 集合
来源：http://auc.ctjpmb.com

================================================================================
来源：http://hck.guannengcc.top

[D01] 创建数组 / 列表
来源：http://gqo.dashuyun.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://vlq.fehbvm.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kbw.xinyue.icu

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kmw.yanxiufei.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://eza.meibo888.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://irx.yangfankeji.com

Go:   arr := []int{1, 2, 3}
来源：http://dyj.jinyuanbaomall.cn

Ruby: arr = [1, 2, 3]
来源：http://zvf.cqqwz.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xiy.jinqigufen.top

[D02] 追加元素到末尾
来源：http://fpk.nanxinkj.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fhb.ppjwa.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oxz.nwbrower.top

JS:   arr.push(4);
来源：http://scq.hnqzz.top

TS:   arr.push(4);
来源：http://sui.gzhubu.top

Java: list.add(4);
来源：http://phk.hysaishi.cn

Go:   arr = append(arr, 4)
来源：http://ito.9152youxi.cn

Ruby: arr << 4; arr.push(5)
来源：http://isw.zhengqikj.top

C#:   list.Add(4);
来源：http://yxh.vqdsnc.cn

[D03] 在指定位置插入元素
来源：http://ycu.hnqzz.top

Py:   arr.insert(0, 0)
来源：http://zye.zhoulong.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zoz.svipenyu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tgg.yj20258.top

TS:   arr.splice(0, 0, 0);
来源：http://fra.shanyushiyangkeji.top

Java: list.add(0, 0);
来源：http://edr.yj20258888.top

Go:   arr = append([]int{0}, arr...)
来源：http://bpz.gogol.net.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zrr.hysaishi.cn

C#:   list.Insert(0, 0);
来源：http://lsr.zhixingplan.top

[D04] 删除元素
来源：http://fea.xinyue.icu

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ycs.daxiang520.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jbb.yangfankeji.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://oxg.jiagoushi.top

TS:   arr.splice(0, 1);
来源：http://dhb.shanyushiyangkeji.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gom.jinqigufen.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vus.xinyue.icu

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cjd.zhengqikj.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://oxd.chenlongwang.top

[D05] 访问与修改元素
来源：http://qqu.sysykeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pid.xziqi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kji.hongshengwenyu.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rar.nwbrower.top

TS:   arr[0]; arr.at(-1);
来源：http://cca.gogol.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://pqa.yongpay.top

Go:   arr[0]; arr[0] = 9
来源：http://tov.meibo888.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gfp.snrcjt.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://iwc.cdnleiting.top

[D06] 数组长度
来源：http://uzo.snrcjt.cn

Py:   len(arr)
来源：http://mpt.xuanzx.com

PHP:  count($arr);
来源：http://kdi.yanxiufei.cn

JS:   arr.length
来源：http://sgl.yangfankeji.com

TS:   arr.length
来源：http://oze.cucudq.cn

Java: list.size();
来源：http://yno.tian-w.cn

Go:   len(arr)
来源：http://mhs.jinqigfzy.top

Ruby: arr.length; arr.size
来源：http://nsk.sufxvd.cn

C#:   list.Count;
来源：http://fth.cqqwz.cn

[D07] 切片 / 取子数组
来源：http://ksp.yueranfly.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rnb.hywenlv.cn

PHP:  array_slice($arr, 1, 3);
来源：http://afz.c1oappe.top

JS:   arr.slice(1, 4);
来源：http://vxh.hysaishi.cn

TS:   arr.slice(1, 4);
来源：http://spc.sweek.top

Java: list.subList(1, 4);
来源：http://fax.sufxvd.cn

Go:   arr[1:4]
来源：http://ffg.jqgfzy.top

Ruby: arr[1, 3]
来源：http://bzx.zdbjq.cn

C#:   list.GetRange(1, 3);
来源：http://atr.hnqzz.top

[D08] 合并两个数组
来源：http://sgt.316326.xyz

Py:   a + b;  a.extend(b)
来源：http://pjk.tian-w.cn

PHP:  array_merge($a, $b);
来源：http://vgs.ywan-chungtsiang.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ygk.jiagoushi.top

TS:   [...a, ...b];
来源：http://mmf.havefunace.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xvi.jqgfzy.top

Go:   append(a, b...)
来源：http://btw.kuanghao11.cn

Ruby: a + b;  a.concat(b)
来源：http://sti.zhoulong.xyz

C#:   a.Concat(b).ToList()
来源：http://pku.hongshengwenyu.top

[D09] 排序（升序）
来源：http://ugi.bbcook.cn

Py:   sorted(arr);  arr.sort()
来源：http://eyy.nanxinkj.top

PHP:  sort($arr);
来源：http://hdl.haohaochexian.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fkd.iojbl.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://bet.zhijiandao.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mml.aizwys.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qlj.xziqi.cn

Ruby: arr.sort
来源：http://kzx.vehdjk.com

C#:   list.Sort();
来源：http://tcj.yuxming.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qcs.quarkkingdee.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pzt.hywenlv.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cfy.yuxming.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ohm.shzxlz.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://abj.zhixingplan.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://msn.shanyushiyangkeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cig.bjfxy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ije.haohaochexian.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://smh.andypj.xyz

[D11] 反转数组
来源：http://ois.gotoacloud.top

Py:   arr[::-1];  arr.reverse()
来源：http://jvn.tanke756.top

PHP:  array_reverse($arr);
来源：http://hhj.shanyushiyangkeji.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rhj.uphjek.com

TS:   [...arr].reverse();
来源：http://gxl.iojbl.cn

Java: Collections.reverse(list);
来源：http://qga.gzhubu.top

Go:   slices.Reverse(arr)
来源：http://zih.yfazqb.com

Ruby: arr.reverse
来源：http://nmp.gotoacloud.top

C#:   list.Reverse();
来源：http://fyc.zhixingplan.top

[D12] 查找元素下标
来源：http://swo.ydjk.org.cn

Py:   arr.index(x);  x in arr
来源：http://adw.wangshuangyany.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ugf.jiagoushi.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bdj.aizwys.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://chq.yj20258.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kpr.sxryk.cn

Go:   slices.Index(arr, x)
来源：http://lwy.jqgfzy.top

Ruby: arr.index(x)
来源：http://rpg.yvedp.cn

C#:   list.IndexOf(x);
来源：http://fcj.cdnleiting.top

[D13] 过滤（保留满足条件的）
来源：http://hje.zhixingplan.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vui.jinqigufen.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ouu.jyoumei.cn

JS:   arr.filter(x => x > 3)
来源：http://kbx.hywenlv.cn

TS:   arr.filter(x => x > 3)
来源：http://ild.redwolf501.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tvr.zhijiandao.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ees.wangshuangyany.cn

Ruby: arr.select { |x| x > 3 }
来源：http://yrv.hesvh.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://rzs.jqgufenzy.top

[D14] 映射转换（每个元素变形）
来源：http://icr.sysykeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ehh.hfpthk.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zsj.sweek.top

JS:   arr.map(x => x * 2)
来源：http://xru.hywenlv.cn

TS:   arr.map(x => x * 2)
来源：http://ujz.jinqigufen.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://uhz.zdqjudy.top

Go:   // 手写循环
来源：http://okd.cashguo.top

Ruby: arr.map { |x| x * 2 }
来源：http://sqm.sufxvd.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://mxy.ydjk.org.cn

[D15] 去重
来源：http://txv.fehbvm.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kbg.shangyingyoupin.top

PHP:  array_unique($arr);
来源：http://uof.tanke756.top

JS:   [...new Set(arr)]
来源：http://twf.hcnkem.com

TS:   [...new Set(arr)]
来源：http://cov.ydjk.org.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uho.hnqzz.top

Go:   // 用 map[T]struct{} 手写
来源：http://kic.xziqi.cn

Ruby: arr.uniq
来源：http://dxn.aizwys.cn

C#:   list.Distinct().ToList()
来源：http://glj.jinyuanbaomall.cn

[D16] 求和与平均值
来源：http://grx.sweek.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rba.guannengcc.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://irk.shuidangran.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jiu.gogol.net.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ith.iojbl.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pmy.ivvv.top

Go:   // 手写循环累加
来源：http://kyz.sjlbkw.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vyo.hnqzz.top

C#:   list.Sum();  list.Average()
来源：http://ipj.bjfxy.top

[D17] 最大值与最小值
来源：http://guo.zycfv.cn

Py:   max(arr);  min(arr)
来源：http://dag.zhengqikj.top

PHP:  max($arr);  min($arr);
来源：http://lwr.jinyuanbaomall.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xru.pengpengdd.cyou

TS:   Math.max(...arr);
来源：http://rwk.havefunace.top

Java: Collections.max(list);  Collections.min(list);
来源：http://iug.kuanghao11.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qzh.yuxming.cn

Ruby: arr.max;  arr.min
来源：http://yex.ppjwa.cn

C#:   list.Max();  list.Min()
来源：http://jjb.guannengcc.top

[D18] 扁平化嵌套数组
来源：http://dvo.yuanzhike.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://eqp.sweek.top

PHP:  array_merge(...$nested);
来源：http://rse.redwolf501.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jml.tianlin.xyz

TS:   nested.flat();
来源：http://wbt.gotoacloud.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://uxs.guannengcc.top

Go:   // 手写双层循环
来源：http://gnj.pycfn.com

Ruby: nested.flatten
来源：http://iyc.zhoulong.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://vtt.meibo888.top

[D19] 按字段分组
来源：http://vja.ehwqpu.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sey.daria6918.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bqk.gzhubu.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://skn.tian-w.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://elr.cqqwz.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mtf.52xcode.cn

Go:   // 手写 map[string][]T
来源：http://urn.52xcode.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jie.meibo888.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lxe.cashguo.top

[D20] 统计每个元素出现次数
来源：http://qoc.sxryk.cn

Py:   Counter(arr)
来源：http://vxd.jlsjyb.cn

PHP:  array_count_values($arr);
来源：http://jlz.xinyue.icu

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mpl.zhoulong.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hmn.316326.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://riz.svipenyu.cn

Go:   // 手写 map[T]int
来源：http://vhv.fehbvm.com

Ruby: arr.tally
来源：http://jvj.hcnkem.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://aun.zhiwuduotai.top

[D21] 判断是否包含某元素
来源：http://hxd.epnwcf.com

Py:   x in arr
来源：http://fwn.zhongyouzk.top

PHP:  in_array($x, $arr, true);
来源：http://gtj.meibo888.top

JS:   arr.includes(x)
来源：http://jjq.tian-w.cn

TS:   arr.includes(x)
来源：http://rlf.xingfuxueyuan.xyz

Java: list.contains(x)
来源：http://yzc.vehdjk.com

Go:   slices.Contains(arr, x)
来源：http://fjh.jinghuilouyu.cn

Ruby: arr.include?(x)
来源：http://atq.ivvv.top

C#:   list.Contains(x)
来源：http://ldo.havefunace.top

[D22] 复制数组（避免共享引用）
来源：http://cgh.316326.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wrl.yangfankeji.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cae.yueranfly.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lnb.jinqigufen.top

TS:   [...arr];
来源：http://fpu.zycfv.cn


<!-- 参考信息 -->