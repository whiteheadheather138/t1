代发 wailian999

[C02] 默认参数
来源：http://vot.zycfv.cn

Py:   def greet(name="World"): return name
来源：http://xmm.fktsv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mqx.yanxiufei.cn

JS:   function greet(name = "World") { return name; }
来源：http://emj.xingfuxueyuan.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://cxy.gotoacloud.top

Java: // 无默认参数：方法重载或 Optional
来源：http://rgw.pycfn.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cph.yvedp.cn

Ruby: def greet(name = "World") = name
来源：http://gyn.c1oappe.top

C#:   string Greet(string name = "World") => name;
来源：http://dki.fzhhl.top

[C03] 可变参数
来源：http://sax.mhx1999.top

Py:   def total(*args): return sum(args)
来源：http://ams.ppjwa.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uyn.hnqzz.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mli.yj20258.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zyj.sxryk.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ahi.hnqzz.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://joa.sweek.top

Ruby: def total(*nums); nums.sum; end
来源：http://pdh.fanxiaobao.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lsu.jinghuilouyu.cn

[C04] 命名参数 / 关键字参数
来源：http://dab.9152youxi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xwj.fengsongda.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hwq.epnwcf.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ffn.feifeiyinyue.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xus.yj20258888.top

Java: // 无：用 Builder 模式或 record
来源：http://hjv.fktsv.cn

Go:   // 无：用配置结构体参数
来源：http://uie.yj20258.top

Ruby: f(a: 1, b: 2)
来源：http://jji.yongpay.top

C#:   f(a: 1, b: 2)
来源：http://gyr.c1oappe.top

[C05] 返回多个值
来源：http://kjr.nwbrower.top

Py:   return a, b
来源：http://kbz.tarul.cn

PHP:  return [$a, $b];
来源：http://tlk.hammf.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yib.wangshuangyany.cn

TS:   return { a, b };
来源：http://jnk.guannengcc.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://due.yj202588.top

Go:   return a, b
来源：http://tbx.vqdsnc.cn

Ruby: return a, b
来源：http://jml.yj20258.top

C#:   return (a, b);              // ValueTuple
来源：http://efb.xuanzx.com

[C06] 匿名函数 / lambda
来源：http://usb.mhx1999.top

Py:   square = lambda x: x * x
来源：http://qlz.tarul.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wvt.wangshuangyany.cn

JS:   const square = x => x * x;
来源：http://ikd.cdnleiting.top

TS:   const square = (x: number): number => x * x;
来源：http://vjt.shzxlz.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gey.0kj1m.cn

Go:   sq := func(x int) int { return x * x }
来源：http://muu.snrcjt.cn

Ruby: square = ->(x) { x * x }
来源：http://aek.cqqwz.cn

C#:   Func<int, int> square = x => x * x;
来源：http://day.jiagoushi.top

[C07] 把函数作为参数传入
来源：http://buc.cucudq.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://eku.yonumen.top

PHP:  array_map("strtoupper", $arr);
来源：http://rrp.ydzc1.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://smi.hcnkem.com

TS:   arr.map(String)
来源：http://cpz.zycfv.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dtv.hongshengwenyu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zxc.jianghu66.top

Ruby: arr.map(&:upcase)
来源：http://jmt.guowangkeji.top

C#:   arr.Select(s => s.ToUpper())
来源：http://szo.ydzc1.top

[C08] 闭包
来源：http://pcy.sjlbkw.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fjn.aibaodan.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sbk.hcnkem.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pok.cashguo.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pnd.yj20258888.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nfi.fzhhl.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://eep.redwolf501.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nxq.cucudq.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gyr.ctjpmb.com

[C09] 递归
来源：http://hyq.tianlin.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mwv.shangyingyoupin.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hpx.jinqigufen.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vny.fehbvm.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cnu.wangshuangyany.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yzp.fengsongda.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lgj.tanke756.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://aec.52xcode.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xne.vqdsnc.cn

[C10] 变量作用域
来源：http://mcf.chenzaomai.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://eal.hammf.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ltu.yj202588.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qnw.snrcjt.cn

TS:   同 JS
来源：http://qbw.gogol.net.cn

Java: 方法内为块级作用域
来源：http://bjq.yj202588.top

Go:   花括号块级作用域
来源：http://hyg.tarul.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ygr.fanxiaobao.xyz

C#:   块级作用域
来源：http://iko.pengpengdd.cyou

[C11] 模块导入与导出
来源：http://qcc.mhx1999.top

Py:   from module import func
来源：http://lgc.jqgfzy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://uze.cheryme.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://rlx.yj202588.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://evz.xziqi.cn

Java: import java.util.List;
来源：http://vxf.zdbjq.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ghv.ctjpmb.com

Ruby: require "json"; require_relative "./util"
来源：http://aic.jqgfzy.top

C#:   using System.Text;
来源：http://lot.yj20258.top

[C12] 立即执行函数 IIFE
来源：http://idu.smart0.xyz

Py:   (lambda: print("run"))()
来源：http://cbs.dianchejie.cn

PHP:  (function () { echo "run"; })();
来源：http://ixm.mhx1999.top

JS:   (() => { console.log("run"); })();
来源：http://nfi.daria6918.cn

TS:   (() => { console.log("run"); })();
来源：http://tss.zdbjq.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lmj.xylfe.cn

Go:   func() { fmt.Println("run") }()
来源：http://okv.tanke756.top

Ruby: -> { puts "run" }.call
来源：http://igk.gaohongyu789.top

C#:   // 无 IIFE：用静态构造函数
来源：http://gbf.yuxming.cn

[C13] 类型声明 / 类型注解
来源：http://brg.epnwcf.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vbc.xuanzx.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rev.xuanzx.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dqc.iojbl.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ypo.uphjek.com

Java: int add(int a, int b) { return a + b; }
来源：http://uwt.xingfuxueyuan.xyz

Go:   func add(a, b int) int
来源：http://zpk.ivvv.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bes.hnqzz.top

C#:   int Add(int a, int b) => a + b;
来源：http://fqs.jiagoushi.top

[C14] 泛型函数
来源：http://kwm.jiagoushi.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://onk.nanxuanxn.top

PHP:  // 无泛型
来源：http://tjn.fzhhl.top

JS:   // 无泛型
来源：http://kxa.hfpthk.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://awz.c1oappe.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rtr.aibaodan.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://uei.jyoumei.cn

Ruby: # 无泛型
来源：http://osi.smart0.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ufc.hongshengwenyu.top

[C15] 解构 / 展开参数
来源：http://jnt.hesvh.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://htv.haohaochexian.top

PHP:  [$a, $b] = $pair;
来源：http://kwm.guannengcc.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zpi.fengsongda.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pzx.gzhubu.top

Java: // 无解构
来源：http://efk.sysykeji.top

Go:   // 无解构
来源：http://kzm.zdqjudy.top

Ruby: a, b = pair
来源：http://ley.pengpengdd.cyou

C#:   var (a, b) = pair;
来源：http://dmq.hnqzz.top

[C16] 函数 / 方法重载
来源：http://ctm.dianchejie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rzm.xuetiantiany.cn

PHP:  // 无重载
来源：http://kff.andypj.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://yqh.wangdashe.top

TS:   // 用联合类型或重载签名声明
来源：http://qmw.zhaomingkeji.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://qen.yongpay.top

Go:   // 无重载：用不同函数名
来源：http://ekd.gzhubu.top

Ruby: # 无重载：靠动态参数
来源：http://dkh.nanxuanxn.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://wvx.shangyingyoupin.top

================================================================================
来源：http://lql.zycfv.cn

D. 数组 / 列表 / 集合
来源：http://fzb.shzxlz.cn

================================================================================
来源：http://swz.tanke756.top

[D01] 创建数组 / 列表
来源：http://rnx.jqgufenzy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://qss.uphjek.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ypq.andypj.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://acn.fengsongda.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ryv.mhx1999.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xir.ydjk.org.cn

Go:   arr := []int{1, 2, 3}
来源：http://lmk.hammf.cn

Ruby: arr = [1, 2, 3]
来源：http://htg.ywan-chungtsiang.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nqy.fengsongda.top

[D02] 追加元素到末尾
来源：http://xyl.hnxiangtu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ibf.shuidangran.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pps.hfpthk.cn

JS:   arr.push(4);
来源：http://brm.yj20258.top

TS:   arr.push(4);
来源：http://dop.ehwqpu.com

Java: list.add(4);
来源：http://dqw.zhijiandao.cn

Go:   arr = append(arr, 4)
来源：http://oem.guowangkeji.top

Ruby: arr << 4; arr.push(5)
来源：http://jaa.vqdsnc.cn

C#:   list.Add(4);
来源：http://ora.yanxiufei.cn

[D03] 在指定位置插入元素
来源：http://rmg.cashguo.top

Py:   arr.insert(0, 0)
来源：http://hcw.cqqwz.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nkg.andypj.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xki.bjfxy.top

TS:   arr.splice(0, 0, 0);
来源：http://lps.xuetiantiany.cn

Java: list.add(0, 0);
来源：http://yus.redwolf501.top

Go:   arr = append([]int{0}, arr...)
来源：http://ltt.hnqzz.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mdt.tianlin.xyz

C#:   list.Insert(0, 0);
来源：http://ggx.andypj.xyz

[D04] 删除元素
来源：http://xnq.shuidangran.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mrw.havefunace.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gln.shzxlz.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zsh.vehdjk.com

TS:   arr.splice(0, 1);
来源：http://hhi.hammf.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wmm.jinyuanbaomall.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://usq.xingfuxueyuan.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ujg.zhixingplan.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wfj.tanke756.top

[D05] 访问与修改元素
来源：http://cxv.hywenlv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kpw.birdmap.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hoc.sysykeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://shr.yvedp.cn

TS:   arr[0]; arr.at(-1);
来源：http://akf.ybcxt.top

Java: list.get(0); list.set(0, 9);
来源：http://jyk.xingfuxueyuan.xyz

Go:   arr[0]; arr[0] = 9
来源：http://tur.316326.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fpp.9152youxi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://btp.gogol.net.cn

[D06] 数组长度
来源：http://cyi.zhijiandao.cn

Py:   len(arr)
来源：http://iws.zdbjq.cn

PHP:  count($arr);
来源：http://ozt.wangshuangyany.cn

JS:   arr.length
来源：http://mme.andypj.xyz

TS:   arr.length
来源：http://klw.zycfv.cn

Java: list.size();
来源：http://twy.jqgfzy.top

Go:   len(arr)
来源：http://gyn.jinyuanbaomall.cn

Ruby: arr.length; arr.size
来源：http://ukv.jinyuanbaomall.cn

C#:   list.Count;
来源：http://ucq.ehwqpu.com

[D07] 切片 / 取子数组
来源：http://ert.yuanzhike.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hms.yj20258.top

PHP:  array_slice($arr, 1, 3);
来源：http://ctj.sjlbkw.cn

JS:   arr.slice(1, 4);
来源：http://kxo.nanxinkj.top

TS:   arr.slice(1, 4);
来源：http://pku.gzhubu.top

Java: list.subList(1, 4);
来源：http://rtl.feifeiyinyue.top

Go:   arr[1:4]
来源：http://hqq.kuanghao11.cn

Ruby: arr[1, 3]
来源：http://kod.nwbrower.top

C#:   list.GetRange(1, 3);
来源：http://ipi.aizwys.cn

[D08] 合并两个数组
来源：http://rao.tianlin.xyz

Py:   a + b;  a.extend(b)
来源：http://sdd.cdnleiting.top

PHP:  array_merge($a, $b);
来源：http://hwo.aibaodan.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://myh.ydjk.org.cn

TS:   [...a, ...b];
来源：http://pfy.yangfankeji.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hkm.dashuyun.cn

Go:   append(a, b...)
来源：http://mpw.zhiwuduotai.top

Ruby: a + b;  a.concat(b)
来源：http://nqm.tianlin.xyz

C#:   a.Concat(b).ToList()
来源：http://tbm.jyoumei.cn

[D09] 排序（升序）
来源：http://coa.dianchejie.cn

Py:   sorted(arr);  arr.sort()
来源：http://nbz.shanyushiyangkeji.top

PHP:  sort($arr);
来源：http://acs.smart0.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wjf.yj20258888.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://rth.hnqzz.top

Java: Collections.sort(list);  list.sort(null);
来源：http://jnj.jyoumei.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fzf.hongshengwenyu.top

Ruby: arr.sort
来源：http://msx.9152youxi.cn

C#:   list.Sort();
来源：http://vli.mhx1999.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://osv.hesvh.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jmf.jqgufenzy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wko.guannengcc.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bab.xuetiantiany.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://txe.gzhubu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kof.cucudq.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mgz.aizwys.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bml.xziqi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wvn.vqdsnc.cn

[D11] 反转数组
来源：http://mew.yuanzhike.top

Py:   arr[::-1];  arr.reverse()
来源：http://pxp.0kj1m.cn

PHP:  array_reverse($arr);
来源：http://has.epnwcf.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qos.kuanghao11.cn

TS:   [...arr].reverse();
来源：http://plp.zhongyouzk.top

Java: Collections.reverse(list);
来源：http://mzd.hongshengwenyu.top

Go:   slices.Reverse(arr)
来源：http://cnd.zhijiandao.cn

Ruby: arr.reverse
来源：http://fyo.nanxuanxn.top

C#:   list.Reverse();
来源：http://imq.xuanzx.com

[D12] 查找元素下标
来源：http://qxx.hnqzz.top

Py:   arr.index(x);  x in arr
来源：http://oiz.zycfv.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bfn.bjfxy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ceq.gogol.net.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oca.jinghuilouyu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ody.fengsongda.top

Go:   slices.Index(arr, x)
来源：http://izq.havefunace.top

Ruby: arr.index(x)
来源：http://blf.52xcode.cn

C#:   list.IndexOf(x);
来源：http://eji.ctjpmb.com

[D13] 过滤（保留满足条件的）
来源：http://nyn.cqqwz.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tbw.zdbjq.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://uwf.9152youxi.cn

JS:   arr.filter(x => x > 3)
来源：http://joq.gogol.net.cn

TS:   arr.filter(x => x > 3)
来源：http://asg.jyoumei.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ndi.aizwys.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rix.hongshengwenyu.top

Ruby: arr.select { |x| x > 3 }
来源：http://nvp.bjfxy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://spi.haohaochexian.top

[D14] 映射转换（每个元素变形）
来源：http://ueo.iojbl.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wre.nanxinkj.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ahp.mhx1999.top

JS:   arr.map(x => x * 2)
来源：http://ulv.epnwcf.com

TS:   arr.map(x => x * 2)
来源：http://vur.tanke756.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://wnz.epnwcf.com

Go:   // 手写循环
来源：http://tof.sjlbkw.cn

Ruby: arr.map { |x| x * 2 }
来源：http://pkc.yangfankeji.com

C#:   list.Select(x => x * 2).ToList()
来源：http://nji.sufxvd.cn

[D15] 去重
来源：http://rnc.zhongyouzk.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ihb.fktsv.cn

PHP:  array_unique($arr);
来源：http://nut.cqqwz.cn

JS:   [...new Set(arr)]
来源：http://ejf.ctjpmb.com

TS:   [...new Set(arr)]
来源：http://lnp.aibaodan.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mzi.jinyuanbaomall.cn

Go:   // 用 map[T]struct{} 手写
来源：http://qdh.9152youxi.cn

Ruby: arr.uniq
来源：http://xpa.hesvh.cn

C#:   list.Distinct().ToList()
来源：http://enz.jinyuanbaomall.cn

[D16] 求和与平均值
来源：http://epv.hfpthk.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mom.tanke756.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tsh.cdnleiting.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://epa.zhixingplan.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rwq.mhx1999.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rsb.guowangkeji.top

Go:   // 手写循环累加
来源：http://jyr.ywan-chungtsiang.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tho.redwolf501.top

C#:   list.Sum();  list.Average()
来源：http://sah.tanke756.top

[D17] 最大值与最小值
来源：http://nmq.iojbl.cn

Py:   max(arr);  min(arr)
来源：http://clc.yueranfly.top

PHP:  max($arr);  min($arr);
来源：http://nqd.nwbrower.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jxc.jlsjyb.cn

TS:   Math.max(...arr);
来源：http://ipi.ctjpmb.com

Java: Collections.max(list);  Collections.min(list);
来源：http://mwh.zhongyouzk.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ztx.jqgfzy.top

Ruby: arr.max;  arr.min
来源：http://spa.zycfv.cn

C#:   list.Max();  list.Min()
来源：http://jbu.52xcode.cn

[D18] 扁平化嵌套数组
来源：http://opq.shzxlz.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mda.jyoumei.cn

PHP:  array_merge(...$nested);
来源：http://bvr.nanxinkj.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yzr.cashguo.top

TS:   nested.flat();
来源：http://joy.yanxiufei.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ajy.sufxvd.cn

Go:   // 手写双层循环
来源：http://ffc.sxryk.cn

Ruby: nested.flatten
来源：http://liu.tianlin.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://dyz.c1oappe.top


<!-- 参考信息 -->