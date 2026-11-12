代发 wailian999

================================================================================
来源：http://pxv.sxryk.cn

C. 函数与作用域
来源：http://kfy.ydzc1.top

================================================================================
来源：http://tlo.jinqigufen.top

[C01] 定义函数
来源：http://pwh.shuidangran.top

Py:   def add(a, b): return a + b
来源：http://tty.shzxlz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://czv.ppjwa.cn

JS:   function add(a, b) { return a + b; }
来源：http://btc.dianchejie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eok.andypj.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://qwd.gaohongyu789.top

Go:   func add(a, b int) int { return a + b }
来源：http://api.snrcjt.cn

Ruby: def add(a, b); a + b; end
来源：http://ugn.bjfxy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ovq.zhongyouzk.top

[C02] 默认参数
来源：http://zvu.sxryk.cn

Py:   def greet(name="World"): return name
来源：http://nab.dianchejie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qay.jiagoushi.top

JS:   function greet(name = "World") { return name; }
来源：http://ypd.shanyushiyangtech.top

TS:   function greet(name: string = "World") { return name; }
来源：http://owt.cashguo.top

Java: // 无默认参数：方法重载或 Optional
来源：http://lxa.yueranfly.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://txw.nanxuanxn.top

Ruby: def greet(name = "World") = name
来源：http://nsc.jinqigfzy.top

C#:   string Greet(string name = "World") => name;
来源：http://pxl.zhengqikj.top

[C03] 可变参数
来源：http://tjl.gogol.net.cn

Py:   def total(*args): return sum(args)
来源：http://hrd.aizwys.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://egf.xuanzx.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lri.jinyuanbaomall.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hkl.316326.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://uay.yueranfly.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ckl.zhiwuduotai.top

Ruby: def total(*nums); nums.sum; end
来源：http://kvk.ppjwa.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fzm.bbcook.cn

[C04] 命名参数 / 关键字参数
来源：http://ghi.gaohongyu789.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dif.yfazqb.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://swu.ppjwa.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dbc.jinghuilouyu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xwo.xinyue.icu

Java: // 无：用 Builder 模式或 record
来源：http://tch.jinqigfzy.top

Go:   // 无：用配置结构体参数
来源：http://dmq.birdmap.top

Ruby: f(a: 1, b: 2)
来源：http://fig.zdqjudy.top

C#:   f(a: 1, b: 2)
来源：http://ydl.gogol.net.cn

[C05] 返回多个值
来源：http://jar.hongshengwenyu.top

Py:   return a, b
来源：http://qvk.hywenlv.cn

PHP:  return [$a, $b];
来源：http://nni.shzxlz.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zct.kuanghao11.cn

TS:   return { a, b };
来源：http://ing.wangshuangyany.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://twn.sjlbkw.cn

Go:   return a, b
来源：http://kgi.yfazqb.com

Ruby: return a, b
来源：http://vkn.zhixingplan.top

C#:   return (a, b);              // ValueTuple
来源：http://vjj.fzhhl.top

[C06] 匿名函数 / lambda
来源：http://dyl.vqdsnc.cn

Py:   square = lambda x: x * x
来源：http://wdd.shanyushiyangkeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://mzv.jqgufenzy.top

JS:   const square = x => x * x;
来源：http://vms.zhijiandao.cn

TS:   const square = (x: number): number => x * x;
来源：http://gyz.xylfe.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wqx.sufxvd.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rca.jqgufenzy.top

Ruby: square = ->(x) { x * x }
来源：http://ect.cashguo.top

C#:   Func<int, int> square = x => x * x;
来源：http://cjj.birdmap.top

[C07] 把函数作为参数传入
来源：http://ymy.0kj1m.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mkw.havefunace.top

PHP:  array_map("strtoupper", $arr);
来源：http://civ.nanxinkj.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rum.gotoacloud.top

TS:   arr.map(String)
来源：http://dkm.yj20258888.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://snj.cashguo.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://liv.yj20258888.top

Ruby: arr.map(&:upcase)
来源：http://yay.gotoacloud.top

C#:   arr.Select(s => s.ToUpper())
来源：http://fjb.yvedp.cn

[C08] 闭包
来源：http://saf.yuanzhike.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mnl.zhoulong.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ruq.hesvh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ksk.gogol.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rgr.jinghuilouyu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wty.sysykeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lfd.xuanzx.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://oaw.yanxiufei.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lms.chenzaomai.com

[C09] 递归
来源：http://pem.yfazqb.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://iui.hammf.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ogu.shuidangran.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jvp.nwbrower.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uat.gzhubu.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://eyh.sweek.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fhs.kuanghao11.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nsm.xziqi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jww.fengsongda.top

[C10] 变量作用域
来源：http://ipp.fktsv.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://axg.chenjidiqi.icu

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xbf.guowangkeji.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://flp.meibo888.top

TS:   同 JS
来源：http://ner.bjfxy.top

Java: 方法内为块级作用域
来源：http://lyv.shangyingyoupin.top

Go:   花括号块级作用域
来源：http://vqa.fktsv.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nus.yanxiufei.cn

C#:   块级作用域
来源：http://vxw.xylfe.cn

[C11] 模块导入与导出
来源：http://ktm.kuanghao11.cn

Py:   from module import func
来源：http://ofx.52xcode.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ajt.zhiwuduotai.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://cjl.tian-w.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xsc.yj20258888.top

Java: import java.util.List;
来源：http://mce.gogol.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nnr.hysaishi.cn

Ruby: require "json"; require_relative "./util"
来源：http://haz.yfazqb.com

C#:   using System.Text;
来源：http://eby.tian-w.cn

[C12] 立即执行函数 IIFE
来源：http://rea.316326.xyz

Py:   (lambda: print("run"))()
来源：http://vcx.cdnleiting.top

PHP:  (function () { echo "run"; })();
来源：http://iej.hywenlv.cn

JS:   (() => { console.log("run"); })();
来源：http://lyq.cdnleiting.top

TS:   (() => { console.log("run"); })();
来源：http://umv.tianlin.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://upk.cdnleiting.top

Go:   func() { fmt.Println("run") }()
来源：http://rxs.shanyushiyangkeji.top

Ruby: -> { puts "run" }.call
来源：http://rzn.zhoulong.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://lou.vqdsnc.cn

[C13] 类型声明 / 类型注解
来源：http://phy.52xcode.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qfy.xuetiantiany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rgz.gotoacloud.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bpd.ctjpmb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mfq.fktsv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://sto.tanke756.top

Go:   func add(a, b int) int
来源：http://ipp.sufxvd.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://izq.chenlongwang.top

C#:   int Add(int a, int b) => a + b;
来源：http://xax.meibo888.top

[C14] 泛型函数
来源：http://xgt.yangfankeji.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mgo.haohaochexian.top

PHP:  // 无泛型
来源：http://gjw.pengpengdd.cyou

JS:   // 无泛型
来源：http://xhg.kuanghao11.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://czp.sjlbkw.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ndb.hammf.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mfo.shangyingyoupin.top

Ruby: # 无泛型
来源：http://pto.meibo888.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gpm.bbcook.cn

[C15] 解构 / 展开参数
来源：http://moj.shuidangran.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zwo.yj20258.top

PHP:  [$a, $b] = $pair;
来源：http://pdh.jinghuilouyu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wpl.vqdsnc.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kjm.xinyue.icu

Java: // 无解构
来源：http://ops.tanke756.top

Go:   // 无解构
来源：http://kjs.gogol.net.cn

Ruby: a, b = pair
来源：http://hvf.ydjk.org.cn

C#:   var (a, b) = pair;
来源：http://ydd.haohaochexian.top

[C16] 函数 / 方法重载
来源：http://hwu.hcnkem.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hpe.bjfxy.top

PHP:  // 无重载
来源：http://err.fanxiaobao.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://dxq.sxryk.cn

TS:   // 用联合类型或重载签名声明
来源：http://ily.fengsongda.top

Java: void f(int a) {}  void f(String a) {}
来源：http://pzp.yvedp.cn

Go:   // 无重载：用不同函数名
来源：http://xfa.pycfn.com

Ruby: # 无重载：靠动态参数
来源：http://mix.guannengcc.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://jmf.ppjwa.cn

================================================================================
来源：http://lcv.meibo888.top

D. 数组 / 列表 / 集合
来源：http://knr.ivvv.top

================================================================================
来源：http://qvw.yuxming.cn

[D01] 创建数组 / 列表
来源：http://xxo.ywan-chungtsiang.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://dvj.xylfe.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hkn.zhijiandao.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nfa.feifeiyinyue.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://rwb.haohaochexian.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nwq.fehbvm.com

Go:   arr := []int{1, 2, 3}
来源：http://gkb.shanyushiyangtech.top

Ruby: arr = [1, 2, 3]
来源：http://wqd.yvedp.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fno.fzhhl.top

[D02] 追加元素到末尾
来源：http://jps.jyoumei.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vis.zhiwuduotai.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hkp.kuanghao11.cn

JS:   arr.push(4);
来源：http://enz.daria6918.cn

TS:   arr.push(4);
来源：http://ucq.yonumen.top

Java: list.add(4);
来源：http://fxo.c1oappe.top

Go:   arr = append(arr, 4)
来源：http://fyi.vehdjk.com

Ruby: arr << 4; arr.push(5)
来源：http://ogq.hammf.cn

C#:   list.Add(4);
来源：http://wwd.yuxming.cn

[D03] 在指定位置插入元素
来源：http://zpj.sweek.top

Py:   arr.insert(0, 0)
来源：http://azz.zdbjq.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hur.gzhubu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kkl.jinqigfzy.top

TS:   arr.splice(0, 0, 0);
来源：http://hdb.yuxming.cn

Java: list.add(0, 0);
来源：http://net.jqgfzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://fxh.zdbjq.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cmh.zycfv.cn

C#:   list.Insert(0, 0);
来源：http://sqv.redwolf501.top

[D04] 删除元素
来源：http://kpd.fktsv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://htn.birdmap.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://eci.yj20258888.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vuj.zhijiandao.cn

TS:   arr.splice(0, 1);
来源：http://cwt.redwolf501.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://haj.c1oappe.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cpp.smart0.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lsm.mhx1999.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dfj.fanxiaobao.xyz

[D05] 访问与修改元素
来源：http://bjo.sjlbkw.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hka.gotoacloud.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dof.yvedp.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://oto.feifeiyinyue.top

TS:   arr[0]; arr.at(-1);
来源：http://fcp.sysykeji.top

Java: list.get(0); list.set(0, 9);
来源：http://qno.ivvv.top

Go:   arr[0]; arr[0] = 9
来源：http://sln.ivvv.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://szy.yongpay.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wsk.aizwys.cn

[D06] 数组长度
来源：http://joz.havefunace.top

Py:   len(arr)
来源：http://yjp.yangfankeji.com

PHP:  count($arr);
来源：http://gmr.xuanzx.com

JS:   arr.length
来源：http://vvd.tian-w.cn

TS:   arr.length
来源：http://lrb.iojbl.cn

Java: list.size();
来源：http://nhy.xingfuxueyuan.xyz

Go:   len(arr)
来源：http://fkr.jiagoushi.top

Ruby: arr.length; arr.size
来源：http://xpx.jinqigufen.top

C#:   list.Count;
来源：http://uyc.nwbrower.top

[D07] 切片 / 取子数组
来源：http://lqb.xylfe.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://scc.jqgfzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://elc.mhx1999.top

JS:   arr.slice(1, 4);
来源：http://cat.hammf.cn

TS:   arr.slice(1, 4);
来源：http://eeq.yueranfly.top

Java: list.subList(1, 4);
来源：http://fki.hesvh.cn

Go:   arr[1:4]
来源：http://tja.chenzaomai.com

Ruby: arr[1, 3]
来源：http://rzm.yongpay.top

C#:   list.GetRange(1, 3);
来源：http://zuu.jinyuanbaomall.cn

[D08] 合并两个数组
来源：http://lwt.sjlbkw.cn

Py:   a + b;  a.extend(b)
来源：http://oju.kuanghao11.cn

PHP:  array_merge($a, $b);
来源：http://khm.zhoulong.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://zxo.zhongyouzk.top

TS:   [...a, ...b];
来源：http://xsl.jinyuanbaomall.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ivl.hnxiangtu.top

Go:   append(a, b...)
来源：http://ede.aibaodan.cn

Ruby: a + b;  a.concat(b)
来源：http://zdr.yfazqb.com

C#:   a.Concat(b).ToList()
来源：http://khn.hywenlv.cn

[D09] 排序（升序）
来源：http://uqq.sufxvd.cn

Py:   sorted(arr);  arr.sort()
来源：http://ogp.aizwys.cn

PHP:  sort($arr);
来源：http://qla.jiagoushi.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pfs.hammf.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://bfg.chenzaomai.com

Java: Collections.sort(list);  list.sort(null);
来源：http://nht.ywan-chungtsiang.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vnh.xingfuxueyuan.xyz

Ruby: arr.sort
来源：http://xcf.chenzaomai.com

C#:   list.Sort();
来源：http://mzb.jinqigufen.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://gnz.pengpengdd.cyou

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nos.yj20258888.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://phd.yanxiufei.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ziw.yj20258.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vpk.hnqzz.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bsp.zdqjudy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uvb.snrcjt.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://att.xingfuxueyuan.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jzu.aizwys.cn

[D11] 反转数组
来源：http://ykj.zhixingplan.top

Py:   arr[::-1];  arr.reverse()
来源：http://jmr.kuanghao11.cn

PHP:  array_reverse($arr);
来源：http://djs.yuxming.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vyp.xziqi.cn

TS:   [...arr].reverse();
来源：http://zcw.jqgfzy.top

Java: Collections.reverse(list);
来源：http://ezb.tian-w.cn

Go:   slices.Reverse(arr)
来源：http://qhn.fzhhl.top

Ruby: arr.reverse
来源：http://tue.uphjek.com

C#:   list.Reverse();
来源：http://hna.52xcode.cn

[D12] 查找元素下标
来源：http://wfz.shangyingyoupin.top

Py:   arr.index(x);  x in arr
来源：http://dwf.vehdjk.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gin.jinghuilouyu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iai.chenzaomai.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kye.sufxvd.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://imp.mhx1999.top

Go:   slices.Index(arr, x)
来源：http://zln.uphjek.com

Ruby: arr.index(x)
来源：http://vme.bjfxy.top

C#:   list.IndexOf(x);
来源：http://yei.yuxming.cn

[D13] 过滤（保留满足条件的）
来源：http://tby.sysykeji.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ykb.ybcxt.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hew.ywan-chungtsiang.top

JS:   arr.filter(x => x > 3)
来源：http://uoq.jiagoushi.top

TS:   arr.filter(x => x > 3)
来源：http://wbf.jlsjyb.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bab.jyoumei.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nnw.epnwcf.com

Ruby: arr.select { |x| x > 3 }
来源：http://hlx.guannengcc.top

C#:   list.Where(x => x > 3).ToList()
来源：http://pcw.hnqzz.top

[D14] 映射转换（每个元素变形）
来源：http://sov.gzhubu.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rpf.nanxuanxn.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gpf.fanxiaobao.xyz

JS:   arr.map(x => x * 2)
来源：http://inm.zhoulong.xyz

TS:   arr.map(x => x * 2)
来源：http://ysk.yueranfly.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://zen.xziqi.cn

Go:   // 手写循环
来源：http://cpv.hysaishi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jzr.chenzaomai.com

C#:   list.Select(x => x * 2).ToList()
来源：http://vis.9152youxi.cn

[D15] 去重
来源：http://wjr.meibo888.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://huy.cucudq.cn

PHP:  array_unique($arr);
来源：http://deg.hongshengwenyu.top

JS:   [...new Set(arr)]
来源：http://zny.gaohongyu789.top

TS:   [...new Set(arr)]
来源：http://hcb.ywan-chungtsiang.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jln.yonumen.top

Go:   // 用 map[T]struct{} 手写
来源：http://rbm.xingfuxueyuan.xyz

Ruby: arr.uniq
来源：http://bsj.daria6918.cn

C#:   list.Distinct().ToList()
来源：http://mtt.jianghu66.top

[D16] 求和与平均值
来源：http://bsk.hcnkem.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rvm.cucudq.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gpz.xingfuxueyuan.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ust.9152youxi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yiw.ehwqpu.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://iqu.yueranfly.top

Go:   // 手写循环累加
来源：http://tvs.cheryme.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hpo.tarul.cn

C#:   list.Sum();  list.Average()
来源：http://ifm.shangyingyoupin.top

[D17] 最大值与最小值
来源：http://ugl.guowangkeji.top

Py:   max(arr);  min(arr)
来源：http://hfd.gaohongyu789.top

PHP:  max($arr);  min($arr);
来源：http://dpx.fanxiaobao.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://azh.shanyushiyangkeji.top

TS:   Math.max(...arr);
来源：http://gvv.xinyue.icu

Java: Collections.max(list);  Collections.min(list);
来源：http://kpk.aizwys.cn


<!-- 参考信息 -->