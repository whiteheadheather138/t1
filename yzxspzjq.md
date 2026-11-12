代发 wailian999

Java: if (data == null) return;
来源：http://mbv.andypj.xyz

Go:   if data == nil { return }
来源：http://dqc.yonumen.top

Ruby: return if data.nil?
来源：http://vlf.sxryk.cn

C#:   if (data == null) return;
来源：http://wgg.xylfe.cn

================================================================================
来源：http://mrq.hfpthk.cn

C. 函数与作用域
来源：http://usf.xinyue.icu

================================================================================
来源：http://tau.guannengcc.top

[C01] 定义函数
来源：http://uvu.ydzc1.top

Py:   def add(a, b): return a + b
来源：http://miv.vehdjk.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jzo.nanxinkj.top

JS:   function add(a, b) { return a + b; }
来源：http://cmt.yj20258888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tym.tian-w.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zhe.zycfv.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qgb.tanke756.top

Ruby: def add(a, b); a + b; end
来源：http://dbd.kuanghao11.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zys.aibaodan.cn

[C02] 默认参数
来源：http://fxp.jqgfzy.top

Py:   def greet(name="World"): return name
来源：http://mtq.feifeiyinyue.top

PHP:  function greet($name = "World") { return $name; }
来源：http://kqx.hongshengwenyu.top

JS:   function greet(name = "World") { return name; }
来源：http://hlg.yfazqb.com

TS:   function greet(name: string = "World") { return name; }
来源：http://gup.gogol.net.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://yuo.aibaodan.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ngz.cheryme.top

Ruby: def greet(name = "World") = name
来源：http://aza.9152youxi.cn

C#:   string Greet(string name = "World") => name;
来源：http://ury.hnxiangtu.top

[C03] 可变参数
来源：http://vct.xinyue.icu

Py:   def total(*args): return sum(args)
来源：http://xhz.aibaodan.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://snr.jinghuilouyu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hgv.shanyushiyangtech.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ony.zhaomingkeji.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yse.meibo888.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qkp.shanyushiyangkeji.top

Ruby: def total(*nums); nums.sum; end
来源：http://eeg.fengsongda.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rry.yanxiufei.cn

[C04] 命名参数 / 关键字参数
来源：http://din.shuidangran.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zgh.quarkkingdee.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zeb.wangshuangyany.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jfm.yfazqb.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tkg.zhoulong.xyz

Java: // 无：用 Builder 模式或 record
来源：http://rqs.xinyue.icu

Go:   // 无：用配置结构体参数
来源：http://qsr.yanxiufei.cn

Ruby: f(a: 1, b: 2)
来源：http://ilc.bjfxy.top

C#:   f(a: 1, b: 2)
来源：http://lot.yonumen.top

[C05] 返回多个值
来源：http://erd.tarul.cn

Py:   return a, b
来源：http://vpm.fktsv.cn

PHP:  return [$a, $b];
来源：http://ejt.epnwcf.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://ngq.sufxvd.cn

TS:   return { a, b };
来源：http://vvx.fengsongda.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xzv.c1oappe.top

Go:   return a, b
来源：http://ror.pycfn.com

Ruby: return a, b
来源：http://jvu.sweek.top

C#:   return (a, b);              // ValueTuple
来源：http://irf.chenjidiqi.icu

[C06] 匿名函数 / lambda
来源：http://uto.gzhubu.top

Py:   square = lambda x: x * x
来源：http://rpp.ybcxt.top

PHP:  $square = fn($x) => $x * $x;
来源：http://cmv.fanxiaobao.xyz

JS:   const square = x => x * x;
来源：http://jbm.zhongyouzk.top

TS:   const square = (x: number): number => x * x;
来源：http://jky.bbcook.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lxv.zhijiandao.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ufq.zhijiandao.cn

Ruby: square = ->(x) { x * x }
来源：http://sya.hfpthk.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ddw.yueranfly.top

[C07] 把函数作为参数传入
来源：http://nxu.hnqzz.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://suz.9152youxi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ljs.andypj.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yub.andypj.xyz

TS:   arr.map(String)
来源：http://fek.nwbrower.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pii.shanyushiyangtech.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uwa.hnqzz.top

Ruby: arr.map(&:upcase)
来源：http://zsl.pengpengdd.cyou

C#:   arr.Select(s => s.ToUpper())
来源：http://sff.birdmap.top

[C08] 闭包
来源：http://tqo.gzhubu.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yrp.birdmap.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qse.shanyushiyangkeji.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://aiv.jianghu66.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xtr.nanxuanxn.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ull.fktsv.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://evv.hongshengwenyu.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tet.shuidangran.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qow.guowangkeji.top

[C09] 递归
来源：http://idi.wangdashe.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://omk.shangyingyoupin.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fjy.ehwqpu.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ibl.havefunace.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qnt.xingfuxueyuan.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://oum.tian-w.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://azo.9152youxi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mkw.xylfe.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sld.birdmap.top

[C10] 变量作用域
来源：http://bnk.0kj1m.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ton.yongpay.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://plc.redwolf501.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mys.hongshengwenyu.top

TS:   同 JS
来源：http://vjx.aizwys.cn

Java: 方法内为块级作用域
来源：http://gaz.sjlbkw.cn

Go:   花括号块级作用域
来源：http://xzm.aibaodan.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ayg.zhixingplan.top

C#:   块级作用域
来源：http://cjh.yfazqb.com

[C11] 模块导入与导出
来源：http://bny.yuxming.cn

Py:   from module import func
来源：http://hxh.kuanghao11.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://puv.redwolf501.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://dzh.fengsongda.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kee.uphjek.com

Java: import java.util.List;
来源：http://ygb.vehdjk.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gma.nanxuanxn.top

Ruby: require "json"; require_relative "./util"
来源：http://qpa.gotoacloud.top

C#:   using System.Text;
来源：http://mgv.hysaishi.cn

[C12] 立即执行函数 IIFE
来源：http://mta.tanke756.top

Py:   (lambda: print("run"))()
来源：http://rxa.52xcode.cn

PHP:  (function () { echo "run"; })();
来源：http://xmn.jinqigfzy.top

JS:   (() => { console.log("run"); })();
来源：http://bzj.gaohongyu789.top

TS:   (() => { console.log("run"); })();
来源：http://cfc.zhaomingkeji.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qvz.xuanzx.com

Go:   func() { fmt.Println("run") }()
来源：http://ljn.birdmap.top

Ruby: -> { puts "run" }.call
来源：http://dfr.jlsjyb.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hhu.yueranfly.top

[C13] 类型声明 / 类型注解
来源：http://wfg.fktsv.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://urk.chenlongwang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aev.yfazqb.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sdo.shanyushiyangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qvr.52xcode.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vrv.jqgufenzy.top

Go:   func add(a, b int) int
来源：http://laa.zhijiandao.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nwz.pycfn.com

C#:   int Add(int a, int b) => a + b;
来源：http://zud.uphjek.com

[C14] 泛型函数
来源：http://wgw.aibaodan.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://clw.chenlongwang.top

PHP:  // 无泛型
来源：http://wjv.ctjpmb.com

JS:   // 无泛型
来源：http://zzl.nanxuanxn.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vej.vqdsnc.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kiq.mhx1999.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cew.nanxinkj.top

Ruby: # 无泛型
来源：http://mhn.52xcode.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://axg.zycfv.cn

[C15] 解构 / 展开参数
来源：http://duw.yonumen.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ikc.hesvh.cn

PHP:  [$a, $b] = $pair;
来源：http://ayw.hongshengwenyu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jwq.cqqwz.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hvt.bjfxy.top

Java: // 无解构
来源：http://avv.vqdsnc.cn

Go:   // 无解构
来源：http://pcm.smart0.xyz

Ruby: a, b = pair
来源：http://akl.jinqigfzy.top

C#:   var (a, b) = pair;
来源：http://tib.hesvh.cn

[C16] 函数 / 方法重载
来源：http://mbf.pengpengdd.cyou

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hgt.jqgfzy.top

PHP:  // 无重载
来源：http://qdd.hnxiangtu.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://xzu.hcnkem.com

TS:   // 用联合类型或重载签名声明
来源：http://bao.hysaishi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wwm.yvedp.cn

Go:   // 无重载：用不同函数名
来源：http://cgp.daria6918.cn

Ruby: # 无重载：靠动态参数
来源：http://ptu.tianlin.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://dxr.zhengqikj.top

================================================================================
来源：http://fxe.gogol.net.cn

D. 数组 / 列表 / 集合
来源：http://cal.yfazqb.com

================================================================================
来源：http://qns.ctjpmb.com

[D01] 创建数组 / 列表
来源：http://ipm.nwbrower.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://rtc.uphjek.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://plv.aibaodan.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uxm.hfpthk.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://mfc.aizwys.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hup.cqqwz.cn

Go:   arr := []int{1, 2, 3}
来源：http://dvl.gogol.net.cn

Ruby: arr = [1, 2, 3]
来源：http://vrb.hfpthk.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://swb.hywenlv.cn

[D02] 追加元素到末尾
来源：http://qqg.aizwys.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://unt.dashuyun.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tix.jqgufenzy.top

JS:   arr.push(4);
来源：http://aph.shanyushiyangkeji.top

TS:   arr.push(4);
来源：http://prd.yj20258888.top

Java: list.add(4);
来源：http://zxm.quarkkingdee.top

Go:   arr = append(arr, 4)
来源：http://njt.hongshengwenyu.top

Ruby: arr << 4; arr.push(5)
来源：http://epm.yongpay.top

C#:   list.Add(4);
来源：http://jni.ydzc1.top

[D03] 在指定位置插入元素
来源：http://idv.jinghuilouyu.cn

Py:   arr.insert(0, 0)
来源：http://rrf.vehdjk.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vkh.vqdsnc.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hij.zhaomingkeji.xyz

TS:   arr.splice(0, 0, 0);
来源：http://zbt.guannengcc.top

Java: list.add(0, 0);
来源：http://oyd.zdqjudy.top

Go:   arr = append([]int{0}, arr...)
来源：http://vic.sysykeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bwe.shzxlz.cn

C#:   list.Insert(0, 0);
来源：http://ktb.iojbl.cn

[D04] 删除元素
来源：http://qge.uphjek.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://snp.yueranfly.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ubk.havefunace.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mqw.ydjk.org.cn

TS:   arr.splice(0, 1);
来源：http://bkq.tianlin.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ufq.zycfv.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gyr.shangyingyoupin.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qtc.cashguo.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kpb.hongshengwenyu.top

[D05] 访问与修改元素
来源：http://ocb.sjlbkw.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nok.iojbl.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hey.epnwcf.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cul.ivvv.top

TS:   arr[0]; arr.at(-1);
来源：http://ngw.ppjwa.cn

Java: list.get(0); list.set(0, 9);
来源：http://rcc.shuidangran.top

Go:   arr[0]; arr[0] = 9
来源：http://tse.iojbl.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wkz.cqqwz.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fva.ivvv.top

[D06] 数组长度
来源：http://fex.zhixingplan.top

Py:   len(arr)
来源：http://ojw.aizwys.cn

PHP:  count($arr);
来源：http://dvd.9152youxi.cn

JS:   arr.length
来源：http://yii.xuetiantiany.cn

TS:   arr.length
来源：http://jdo.ywan-chungtsiang.top

Java: list.size();
来源：http://tse.quarkkingdee.top

Go:   len(arr)
来源：http://bhe.jinqigfzy.top

Ruby: arr.length; arr.size
来源：http://htk.9152youxi.cn

C#:   list.Count;
来源：http://uad.fktsv.cn

[D07] 切片 / 取子数组
来源：http://jdj.shzxlz.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hbx.hongshengwenyu.top

PHP:  array_slice($arr, 1, 3);
来源：http://gkg.iojbl.cn

JS:   arr.slice(1, 4);
来源：http://joq.dianchejie.cn

TS:   arr.slice(1, 4);
来源：http://xzp.ivvv.top

Java: list.subList(1, 4);
来源：http://xln.cashguo.top

Go:   arr[1:4]
来源：http://sli.hfpthk.cn

Ruby: arr[1, 3]
来源：http://brg.fktsv.cn

C#:   list.GetRange(1, 3);
来源：http://tes.birdmap.top

[D08] 合并两个数组
来源：http://caw.zhoulong.xyz

Py:   a + b;  a.extend(b)
来源：http://ysg.ppjwa.cn

PHP:  array_merge($a, $b);
来源：http://ioo.cheryme.top

JS:   [...a, ...b];  a.concat(b);
来源：http://xwn.xuanzx.com

TS:   [...a, ...b];
来源：http://dgc.feifeiyinyue.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://eou.tanke756.top

Go:   append(a, b...)
来源：http://xla.shanyushiyangtech.top

Ruby: a + b;  a.concat(b)
来源：http://mrs.yj202588.top

C#:   a.Concat(b).ToList()
来源：http://acx.yvedp.cn

[D09] 排序（升序）
来源：http://wed.chenlongwang.top

Py:   sorted(arr);  arr.sort()
来源：http://wzx.yueranfly.top

PHP:  sort($arr);
来源：http://ryu.hammf.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bbe.hnqzz.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://lak.meibo888.top

Java: Collections.sort(list);  list.sort(null);
来源：http://wtb.hesvh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://eci.gogol.net.cn

Ruby: arr.sort
来源：http://cpg.svipenyu.cn

C#:   list.Sort();
来源：http://age.zycfv.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rgn.bjfxy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://iiy.shangyingyoupin.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eqc.jlsjyb.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://phd.gogol.net.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lyg.fzhhl.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://aog.mhx1999.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rkx.andypj.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xuc.fktsv.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dhg.hesvh.cn

[D11] 反转数组
来源：http://mqd.havefunace.top

Py:   arr[::-1];  arr.reverse()
来源：http://ggv.ctjpmb.com

PHP:  array_reverse($arr);
来源：http://xtg.dianchejie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://epn.mhx1999.top

TS:   [...arr].reverse();
来源：http://xfd.hongshengwenyu.top

Java: Collections.reverse(list);
来源：http://ykl.gaohongyu789.top

Go:   slices.Reverse(arr)
来源：http://yrr.316326.xyz

Ruby: arr.reverse
来源：http://nxf.dianchejie.cn

C#:   list.Reverse();
来源：http://ofe.zhoulong.xyz

[D12] 查找元素下标
来源：http://dfi.iojbl.cn

Py:   arr.index(x);  x in arr
来源：http://zrd.birdmap.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jyj.gogol.net.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oai.chenlongwang.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zqb.pycfn.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hzb.fanxiaobao.xyz

Go:   slices.Index(arr, x)
来源：http://jci.cucudq.cn

Ruby: arr.index(x)
来源：http://rec.bbcook.cn

C#:   list.IndexOf(x);
来源：http://rcd.ybcxt.top

[D13] 过滤（保留满足条件的）
来源：http://iyp.ctjpmb.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ahi.tianlin.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xwf.chenjidiqi.icu

JS:   arr.filter(x => x > 3)
来源：http://ymt.cqqwz.cn

TS:   arr.filter(x => x > 3)
来源：http://pxj.9152youxi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tfo.sxryk.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://odi.kuanghao11.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nww.gaohongyu789.top

C#:   list.Where(x => x > 3).ToList()
来源：http://fkq.yangfankeji.com

[D14] 映射转换（每个元素变形）
来源：http://kwe.jlsjyb.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gok.zhoulong.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mjo.havefunace.top

JS:   arr.map(x => x * 2)
来源：http://dai.vqdsnc.cn

TS:   arr.map(x => x * 2)
来源：http://lgu.hammf.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://mhe.ywan-chungtsiang.top

Go:   // 手写循环
来源：http://gfk.nanxuanxn.top

Ruby: arr.map { |x| x * 2 }
来源：http://dth.cqqwz.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bmt.yvedp.cn

[D15] 去重
来源：http://hgi.jyoumei.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nsc.nanxinkj.top

PHP:  array_unique($arr);
来源：http://ymx.cashguo.top

JS:   [...new Set(arr)]
来源：http://jfm.xziqi.cn

TS:   [...new Set(arr)]
来源：http://iub.feifeiyinyue.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xwc.jianghu66.top

Go:   // 用 map[T]struct{} 手写
来源：http://kpp.zdbjq.cn

Ruby: arr.uniq
来源：http://vsr.xuanzx.com

C#:   list.Distinct().ToList()
来源：http://csg.cqqwz.cn

[D16] 求和与平均值
来源：http://faq.316326.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gyp.cashguo.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xfu.aizwys.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gln.9152youxi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jjz.ybcxt.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kdu.smart0.xyz

Go:   // 手写循环累加
来源：http://gxt.nwbrower.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nhz.haohaochexian.top

C#:   list.Sum();  list.Average()
来源：http://fcx.hnxiangtu.top

[D17] 最大值与最小值
来源：http://slx.sxryk.cn

Py:   max(arr);  min(arr)
来源：http://mrg.xingfuxueyuan.xyz


<!-- 参考信息 -->