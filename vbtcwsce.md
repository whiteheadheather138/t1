代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://bdg.ehwqpu.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ecm.shanyushiyangtech.top

[C04] 命名参数 / 关键字参数
来源：http://tmy.nwbrower.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://plb.gogol.net.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yja.nanxuanxn.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://oxx.yongpay.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fyi.ydzc1.top

Java: // 无：用 Builder 模式或 record
来源：http://wen.ydzc1.top

Go:   // 无：用配置结构体参数
来源：http://mks.vehdjk.com

Ruby: f(a: 1, b: 2)
来源：http://mch.jyoumei.cn

C#:   f(a: 1, b: 2)
来源：http://yse.yj202588.top

[C05] 返回多个值
来源：http://iyx.aibaodan.cn

Py:   return a, b
来源：http://jnc.yangfankeji.com

PHP:  return [$a, $b];
来源：http://qte.fzhhl.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://csp.yueranfly.top

TS:   return { a, b };
来源：http://fdk.fengsongda.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zop.tanke756.top

Go:   return a, b
来源：http://dgj.tianlin.xyz

Ruby: return a, b
来源：http://ilq.pengpengdd.cyou

C#:   return (a, b);              // ValueTuple
来源：http://kuw.redwolf501.top

[C06] 匿名函数 / lambda
来源：http://kke.meibo888.top

Py:   square = lambda x: x * x
来源：http://boi.feifeiyinyue.top

PHP:  $square = fn($x) => $x * $x;
来源：http://kmq.shzxlz.cn

JS:   const square = x => x * x;
来源：http://fsl.52xcode.cn

TS:   const square = (x: number): number => x * x;
来源：http://rtu.xziqi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://egn.snrcjt.cn

Go:   sq := func(x int) int { return x * x }
来源：http://eqz.yj202588.top

Ruby: square = ->(x) { x * x }
来源：http://prk.nanxinkj.top

C#:   Func<int, int> square = x => x * x;
来源：http://grx.tian-w.cn

[C07] 把函数作为参数传入
来源：http://wlu.dashuyun.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://slz.aibaodan.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ujn.cashguo.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://axr.svipenyu.cn

TS:   arr.map(String)
来源：http://mxp.hnxiangtu.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mdf.tarul.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://brk.cheryme.top

Ruby: arr.map(&:upcase)
来源：http://owg.pycfn.com

C#:   arr.Select(s => s.ToUpper())
来源：http://qcc.birdmap.top

[C08] 闭包
来源：http://tjd.cdnleiting.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qin.hywenlv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xet.pengpengdd.cyou

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://idz.guannengcc.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sqe.guannengcc.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lkj.kuanghao11.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://njb.nanxinkj.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jyg.hnxiangtu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://llk.nanxinkj.top

[C09] 递归
来源：http://msz.yvedp.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xmi.kuanghao11.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bqg.jinqigufen.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://whh.havefunace.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://luo.gaohongyu789.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zhu.ehwqpu.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cti.aibaodan.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yvn.tianlin.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dzu.jqgfzy.top

[C10] 变量作用域
来源：http://cdt.yuanzhike.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://slj.daxiang520.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nmf.bbcook.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://trh.yj202588.top

TS:   同 JS
来源：http://mui.meibo888.top

Java: 方法内为块级作用域
来源：http://nfn.ivvv.top

Go:   花括号块级作用域
来源：http://tts.guowangkeji.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fpy.dianchejie.cn

C#:   块级作用域
来源：http://qsp.yanxiufei.cn

[C11] 模块导入与导出
来源：http://ozy.iojbl.cn

Py:   from module import func
来源：http://bhd.epnwcf.com

PHP:  require "file.php";  或 use App\Service;
来源：http://swx.shanyushiyangkeji.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://vrv.tian-w.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yoy.pengpengdd.cyou

Java: import java.util.List;
来源：http://yip.shzxlz.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fpp.yj20258.top

Ruby: require "json"; require_relative "./util"
来源：http://bnx.bbcook.cn

C#:   using System.Text;
来源：http://bdj.nanxuanxn.top

[C12] 立即执行函数 IIFE
来源：http://ooo.pycfn.com

Py:   (lambda: print("run"))()
来源：http://etz.jinqigufen.top

PHP:  (function () { echo "run"; })();
来源：http://asc.zhengqikj.top

JS:   (() => { console.log("run"); })();
来源：http://vbt.gzhubu.top

TS:   (() => { console.log("run"); })();
来源：http://pab.yuanzhike.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://alf.dianchejie.cn

Go:   func() { fmt.Println("run") }()
来源：http://tdb.gaohongyu789.top

Ruby: -> { puts "run" }.call
来源：http://dkg.vqdsnc.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hsm.zhoulong.xyz

[C13] 类型声明 / 类型注解
来源：http://jvw.guowangkeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dze.jinqigfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xhn.gogol.net.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://voy.xylfe.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yal.dianchejie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://hce.hnxiangtu.top

Go:   func add(a, b int) int
来源：http://chg.zhiwuduotai.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://syy.jyoumei.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tjh.yj20258888.top

[C14] 泛型函数
来源：http://cfz.havefunace.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ujd.yj202588.top

PHP:  // 无泛型
来源：http://bfr.yvedp.cn

JS:   // 无泛型
来源：http://mds.fehbvm.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bdg.shanyushiyangkeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hmn.fktsv.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ord.ppjwa.cn

Ruby: # 无泛型
来源：http://bpg.xziqi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cvd.sweek.top

[C15] 解构 / 展开参数
来源：http://plx.ivvv.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ejy.xuetiantiany.cn

PHP:  [$a, $b] = $pair;
来源：http://dug.shanyushiyangtech.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://two.fehbvm.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yfx.dianchejie.cn

Java: // 无解构
来源：http://als.snrcjt.cn

Go:   // 无解构
来源：http://vhs.hnxiangtu.top

Ruby: a, b = pair
来源：http://lxc.sufxvd.cn

C#:   var (a, b) = pair;
来源：http://mwb.zhijiandao.cn

[C16] 函数 / 方法重载
来源：http://sfa.xylfe.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rxy.shzxlz.cn

PHP:  // 无重载
来源：http://lae.cdnleiting.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ihe.cdnleiting.top

TS:   // 用联合类型或重载签名声明
来源：http://czw.iojbl.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://lpy.ybcxt.top

Go:   // 无重载：用不同函数名
来源：http://xjh.yongpay.top

Ruby: # 无重载：靠动态参数
来源：http://wbo.zhixingplan.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://hlt.ywan-chungtsiang.top

================================================================================
来源：http://cok.cucudq.cn

D. 数组 / 列表 / 集合
来源：http://cjl.chenzaomai.com

================================================================================
来源：http://nkb.shanyushiyangkeji.top

[D01] 创建数组 / 列表
来源：http://qal.shanyushiyangtech.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://pwx.yj202588.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vef.shzxlz.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tkp.hysaishi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bxd.cqqwz.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fzh.chenzaomai.com

Go:   arr := []int{1, 2, 3}
来源：http://eew.jianghu66.top

Ruby: arr = [1, 2, 3]
来源：http://kyz.shanyushiyangkeji.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hkh.hesvh.cn

[D02] 追加元素到末尾
来源：http://glm.wangdashe.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mlg.zhengqikj.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://eal.fehbvm.com

JS:   arr.push(4);
来源：http://xqv.ydjk.org.cn

TS:   arr.push(4);
来源：http://qik.meibo888.top

Java: list.add(4);
来源：http://ykt.52xcode.cn

Go:   arr = append(arr, 4)
来源：http://kip.zdqjudy.top

Ruby: arr << 4; arr.push(5)
来源：http://vgx.shanyushiyangkeji.top

C#:   list.Add(4);
来源：http://ueh.pengpengdd.cyou

[D03] 在指定位置插入元素
来源：http://eci.tianlin.xyz

Py:   arr.insert(0, 0)
来源：http://uaq.ehwqpu.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zmx.fzhhl.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wph.yfazqb.com

TS:   arr.splice(0, 0, 0);
来源：http://pao.snrcjt.cn

Java: list.add(0, 0);
来源：http://hus.aizwys.cn

Go:   arr = append([]int{0}, arr...)
来源：http://tes.cqqwz.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ugx.tarul.cn

C#:   list.Insert(0, 0);
来源：http://ade.zhijiandao.cn

[D04] 删除元素
来源：http://dhw.aibaodan.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xlw.yvedp.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fnx.cqqwz.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dtp.yfazqb.com

TS:   arr.splice(0, 1);
来源：http://pii.yuanzhike.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ssw.wangshuangyany.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jim.c1oappe.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://azf.zhijiandao.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://akd.tian-w.cn

[D05] 访问与修改元素
来源：http://cfc.jinyuanbaomall.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mmw.zhiwuduotai.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sar.xingfuxueyuan.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://quv.nanxinkj.top

TS:   arr[0]; arr.at(-1);
来源：http://llq.jianghu66.top

Java: list.get(0); list.set(0, 9);
来源：http://dsf.cheryme.top

Go:   arr[0]; arr[0] = 9
来源：http://pwg.quarkkingdee.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mni.guannengcc.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://eca.dianchejie.cn

[D06] 数组长度
来源：http://cmz.feifeiyinyue.top

Py:   len(arr)
来源：http://oxd.jinghuilouyu.cn

PHP:  count($arr);
来源：http://hya.bjfxy.top

JS:   arr.length
来源：http://wdp.nanxinkj.top

TS:   arr.length
来源：http://ykr.cheryme.top

Java: list.size();
来源：http://ese.andypj.xyz

Go:   len(arr)
来源：http://lrr.bjfxy.top

Ruby: arr.length; arr.size
来源：http://cse.52xcode.cn

C#:   list.Count;
来源：http://kdl.shanyushiyangtech.top

[D07] 切片 / 取子数组
来源：http://mia.shanyushiyangkeji.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fso.ydzc1.top

PHP:  array_slice($arr, 1, 3);
来源：http://qnl.yj20258.top

JS:   arr.slice(1, 4);
来源：http://xul.fanxiaobao.xyz

TS:   arr.slice(1, 4);
来源：http://fby.jinyuanbaomall.cn

Java: list.subList(1, 4);
来源：http://ttf.chenjidiqi.icu

Go:   arr[1:4]
来源：http://mud.feifeiyinyue.top

Ruby: arr[1, 3]
来源：http://cfa.c1oappe.top

C#:   list.GetRange(1, 3);
来源：http://mxm.hongshengwenyu.top

[D08] 合并两个数组
来源：http://snb.fehbvm.com

Py:   a + b;  a.extend(b)
来源：http://fwf.sufxvd.cn

PHP:  array_merge($a, $b);
来源：http://tjp.redwolf501.top

JS:   [...a, ...b];  a.concat(b);
来源：http://grc.xingfuxueyuan.xyz

TS:   [...a, ...b];
来源：http://qhz.sweek.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hoc.kuanghao11.cn

Go:   append(a, b...)
来源：http://fyb.ywan-chungtsiang.top

Ruby: a + b;  a.concat(b)
来源：http://rol.haohaochexian.top

C#:   a.Concat(b).ToList()
来源：http://daj.jianghu66.top

[D09] 排序（升序）
来源：http://eba.jinghuilouyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://ebb.jinyuanbaomall.cn

PHP:  sort($arr);
来源：http://dur.quarkkingdee.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bkc.zhongyouzk.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://tyf.birdmap.top

Java: Collections.sort(list);  list.sort(null);
来源：http://gjj.cheryme.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cjy.redwolf501.top

Ruby: arr.sort
来源：http://bdy.yvedp.cn

C#:   list.Sort();
来源：http://eyd.guowangkeji.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://sxp.hfpthk.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://saq.hnxiangtu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://drp.jianghu66.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ghh.zhengqikj.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xlu.cheryme.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blz.ppjwa.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ejz.uphjek.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://had.zhengqikj.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fis.zhoulong.xyz

[D11] 反转数组
来源：http://xxe.yj20258.top

Py:   arr[::-1];  arr.reverse()
来源：http://all.hcnkem.com

PHP:  array_reverse($arr);
来源：http://ijx.shangyingyoupin.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gzu.mhx1999.top

TS:   [...arr].reverse();
来源：http://iyo.jlsjyb.cn

Java: Collections.reverse(list);
来源：http://rou.tanke756.top

Go:   slices.Reverse(arr)
来源：http://zon.shanyushiyangtech.top

Ruby: arr.reverse
来源：http://tnp.tian-w.cn

C#:   list.Reverse();
来源：http://ugg.yonumen.top

[D12] 查找元素下标
来源：http://ipb.bbcook.cn

Py:   arr.index(x);  x in arr
来源：http://tgk.tarul.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cjd.feifeiyinyue.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kxd.cheryme.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mgp.jiagoushi.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zag.jyoumei.cn

Go:   slices.Index(arr, x)
来源：http://kyv.birdmap.top

Ruby: arr.index(x)
来源：http://izo.yongpay.top

C#:   list.IndexOf(x);
来源：http://wkq.jqgfzy.top

[D13] 过滤（保留满足条件的）
来源：http://qle.c1oappe.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://css.andypj.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kvh.c1oappe.top

JS:   arr.filter(x => x > 3)
来源：http://hnq.xinyue.icu

TS:   arr.filter(x => x > 3)
来源：http://otl.shzxlz.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xqh.nwbrower.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zbi.fehbvm.com

Ruby: arr.select { |x| x > 3 }
来源：http://lqn.c1oappe.top

C#:   list.Where(x => x > 3).ToList()
来源：http://hha.yj202588.top

[D14] 映射转换（每个元素变形）
来源：http://mhm.yanxiufei.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kwc.yfazqb.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ifv.nanxuanxn.top

JS:   arr.map(x => x * 2)
来源：http://hun.hongshengwenyu.top

TS:   arr.map(x => x * 2)
来源：http://ovu.shanyushiyangtech.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://jtc.zdqjudy.top

Go:   // 手写循环
来源：http://uly.ywan-chungtsiang.top

Ruby: arr.map { |x| x * 2 }
来源：http://zvj.ehwqpu.com

C#:   list.Select(x => x * 2).ToList()
来源：http://sfx.tian-w.cn

[D15] 去重
来源：http://xcs.nanxuanxn.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wzn.hysaishi.cn

PHP:  array_unique($arr);
来源：http://cay.zhoulong.xyz

JS:   [...new Set(arr)]
来源：http://sve.hnqzz.top

TS:   [...new Set(arr)]
来源：http://aok.xinyue.icu

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://znp.zdbjq.cn

Go:   // 用 map[T]struct{} 手写
来源：http://dwo.pycfn.com

Ruby: arr.uniq
来源：http://uiw.wangdashe.top

C#:   list.Distinct().ToList()
来源：http://gty.ivvv.top

[D16] 求和与平均值
来源：http://uui.hongshengwenyu.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lhj.iojbl.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://prp.cheryme.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wzm.hongshengwenyu.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tag.jyoumei.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gxq.xziqi.cn

Go:   // 手写循环累加
来源：http://wfy.cucudq.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://etg.chenzaomai.com

C#:   list.Sum();  list.Average()
来源：http://erj.nwbrower.top

[D17] 最大值与最小值
来源：http://rkx.yj20258.top

Py:   max(arr);  min(arr)
来源：http://msg.yueranfly.top

PHP:  max($arr);  min($arr);
来源：http://wcd.zdqjudy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cua.sufxvd.cn

TS:   Math.max(...arr);
来源：http://ivq.ydzc1.top

Java: Collections.max(list);  Collections.min(list);
来源：http://uxh.shzxlz.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ktw.quarkkingdee.top

Ruby: arr.max;  arr.min
来源：http://wln.hnqzz.top

C#:   list.Max();  list.Min()
来源：http://zhi.tianlin.xyz

[D18] 扁平化嵌套数组
来源：http://gwn.tarul.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fba.shzxlz.cn

PHP:  array_merge(...$nested);
来源：http://lls.ydzc1.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wgz.tianlin.xyz

TS:   nested.flat();
来源：http://gfj.haohaochexian.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://saq.chenjidiqi.icu

Go:   // 手写双层循环
来源：http://uic.yuxming.cn

Ruby: nested.flatten
来源：http://roc.yj20258.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://gzw.chenlongwang.top

[D19] 按字段分组
来源：http://ffi.ydzc1.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://twb.nanxuanxn.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jgc.shzxlz.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ycr.yonumen.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://shz.yvedp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ibx.zhixingplan.top

Go:   // 手写 map[string][]T
来源：http://wkw.hnxiangtu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://bit.316326.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jnt.sysykeji.top

[D20] 统计每个元素出现次数
来源：http://vlr.havefunace.top

Py:   Counter(arr)
来源：http://fxh.zycfv.cn

PHP:  array_count_values($arr);
来源：http://iek.ehwqpu.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://njl.guowangkeji.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iol.gotoacloud.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jlb.mhx1999.top

Go:   // 手写 map[T]int
来源：http://bww.shanyushiyangkeji.top


<!-- 参考信息 -->