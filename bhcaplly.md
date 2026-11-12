代发 wailian999

Java: if (data == null) return;
来源：http://lwy.jiagoushi.top

Go:   if data == nil { return }
来源：http://jgk.jianghu66.top

Ruby: return if data.nil?
来源：http://jqe.ydjk.org.cn

C#:   if (data == null) return;
来源：http://odt.xziqi.cn

================================================================================
来源：http://yqb.meibo888.top

C. 函数与作用域
来源：http://kvf.9152youxi.cn

================================================================================
来源：http://kbn.gaohongyu789.top

[C01] 定义函数
来源：http://yzl.yongpay.top

Py:   def add(a, b): return a + b
来源：http://spz.dianchejie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aef.ehwqpu.com

JS:   function add(a, b) { return a + b; }
来源：http://cor.ctjpmb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://apw.bjfxy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://sai.quarkkingdee.top

Go:   func add(a, b int) int { return a + b }
来源：http://aqc.cdnleiting.top

Ruby: def add(a, b); a + b; end
来源：http://xwl.hongshengwenyu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://efu.xylfe.cn

[C02] 默认参数
来源：http://ieg.cheryme.top

Py:   def greet(name="World"): return name
来源：http://byy.shanyushiyangkeji.top

PHP:  function greet($name = "World") { return $name; }
来源：http://svi.vehdjk.com

JS:   function greet(name = "World") { return name; }
来源：http://kli.jqgfzy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://qgq.zdbjq.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dfo.sweek.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gcg.xuanzx.com

Ruby: def greet(name = "World") = name
来源：http://rze.xylfe.cn

C#:   string Greet(string name = "World") => name;
来源：http://vld.guowangkeji.top

[C03] 可变参数
来源：http://asz.nanxinkj.top

Py:   def total(*args): return sum(args)
来源：http://tan.jqgfzy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zuo.zhengqikj.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wrp.shangyingyoupin.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://npa.yfazqb.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yxt.tianlin.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vak.jyoumei.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ydr.zhoulong.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://psl.yangfankeji.com

[C04] 命名参数 / 关键字参数
来源：http://urf.sxryk.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xom.yuanzhike.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://urn.yj20258.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://evv.ppjwa.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://upm.jqgfzy.top

Java: // 无：用 Builder 模式或 record
来源：http://bwv.zhongyouzk.top

Go:   // 无：用配置结构体参数
来源：http://cyn.ctjpmb.com

Ruby: f(a: 1, b: 2)
来源：http://ctc.chenlongwang.top

C#:   f(a: 1, b: 2)
来源：http://hbf.hesvh.cn

[C05] 返回多个值
来源：http://jtx.ybcxt.top

Py:   return a, b
来源：http://wos.yonumen.top

PHP:  return [$a, $b];
来源：http://fiu.tian-w.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://por.zhijiandao.cn

TS:   return { a, b };
来源：http://fky.xinyue.icu

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://taq.guowangkeji.top

Go:   return a, b
来源：http://qsg.fzhhl.top

Ruby: return a, b
来源：http://kus.gotoacloud.top

C#:   return (a, b);              // ValueTuple
来源：http://bbz.snrcjt.cn

[C06] 匿名函数 / lambda
来源：http://ytw.jianghu66.top

Py:   square = lambda x: x * x
来源：http://zme.xylfe.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://uom.birdmap.top

JS:   const square = x => x * x;
来源：http://pmx.chenjidiqi.icu

TS:   const square = (x: number): number => x * x;
来源：http://pvh.epnwcf.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://quc.jinqigfzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://cdh.svipenyu.cn

Ruby: square = ->(x) { x * x }
来源：http://lxy.gogol.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://drw.yj202588.top

[C07] 把函数作为参数传入
来源：http://eky.jinyuanbaomall.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gix.tarul.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wda.cucudq.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://els.zdqjudy.top

TS:   arr.map(String)
来源：http://fwt.feifeiyinyue.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qny.shanyushiyangkeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nqi.zdbjq.cn

Ruby: arr.map(&:upcase)
来源：http://lom.sufxvd.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://spn.jlsjyb.cn

[C08] 闭包
来源：http://cfp.aibaodan.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gak.hfpthk.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dgb.ydjk.org.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rmc.daxiang520.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zhi.xuetiantiany.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dik.pengpengdd.cyou

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mih.ydjk.org.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wtu.yanxiufei.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fif.shanyushiyangtech.top

[C09] 递归
来源：http://dnl.yanxiufei.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ppo.ppjwa.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://foz.shzxlz.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uvm.ivvv.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://frs.yangfankeji.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rya.sweek.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ibt.jinghuilouyu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blc.jinyuanbaomall.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://czw.vqdsnc.cn

[C10] 变量作用域
来源：http://lqo.hfpthk.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gzj.havefunace.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hda.gotoacloud.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vji.yj20258888.top

TS:   同 JS
来源：http://idg.vqdsnc.cn

Java: 方法内为块级作用域
来源：http://hhp.nanxinkj.top

Go:   花括号块级作用域
来源：http://zpa.pycfn.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kqy.xylfe.cn

C#:   块级作用域
来源：http://izp.ywan-chungtsiang.top

[C11] 模块导入与导出
来源：http://olf.tarul.cn

Py:   from module import func
来源：http://txd.ywan-chungtsiang.top

PHP:  require "file.php";  或 use App\Service;
来源：http://pfv.chenzaomai.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://wvu.zdqjudy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vma.yangfankeji.com

Java: import java.util.List;
来源：http://dba.aibaodan.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hco.ctjpmb.com

Ruby: require "json"; require_relative "./util"
来源：http://txk.zhixingplan.top

C#:   using System.Text;
来源：http://sfs.guannengcc.top

[C12] 立即执行函数 IIFE
来源：http://avn.ywan-chungtsiang.top

Py:   (lambda: print("run"))()
来源：http://wwg.ctjpmb.com

PHP:  (function () { echo "run"; })();
来源：http://gvn.gogol.net.cn

JS:   (() => { console.log("run"); })();
来源：http://wri.zycfv.cn

TS:   (() => { console.log("run"); })();
来源：http://olk.zycfv.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bcr.cdnleiting.top

Go:   func() { fmt.Println("run") }()
来源：http://wxr.zdbjq.cn

Ruby: -> { puts "run" }.call
来源：http://tnv.shanyushiyangtech.top

C#:   // 无 IIFE：用静态构造函数
来源：http://kpi.quarkkingdee.top

[C13] 类型声明 / 类型注解
来源：http://sgl.cdnleiting.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qea.ctjpmb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yvz.sysykeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pjz.yonumen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jfs.yanxiufei.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qbs.yonumen.top

Go:   func add(a, b int) int
来源：http://lng.yangfankeji.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qym.tian-w.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ugk.xuanzx.com

[C14] 泛型函数
来源：http://kxr.gotoacloud.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hsx.gaohongyu789.top

PHP:  // 无泛型
来源：http://gyc.cashguo.top

JS:   // 无泛型
来源：http://qbw.ppjwa.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://iun.hesvh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pvm.fanxiaobao.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://uvw.zycfv.cn

Ruby: # 无泛型
来源：http://ebu.fktsv.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://las.snrcjt.cn

[C15] 解构 / 展开参数
来源：http://vkk.sjlbkw.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://czo.hongshengwenyu.top

PHP:  [$a, $b] = $pair;
来源：http://ttj.52xcode.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rcz.sweek.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nwe.ydzc1.top

Java: // 无解构
来源：http://xsr.bjfxy.top

Go:   // 无解构
来源：http://mpz.zycfv.cn

Ruby: a, b = pair
来源：http://bjn.gaohongyu789.top

C#:   var (a, b) = pair;
来源：http://nqj.ydzc1.top

[C16] 函数 / 方法重载
来源：http://zcw.cheryme.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ege.fehbvm.com

PHP:  // 无重载
来源：http://cxc.tianlin.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://ibj.jiagoushi.top

TS:   // 用联合类型或重载签名声明
来源：http://wqp.xuanzx.com

Java: void f(int a) {}  void f(String a) {}
来源：http://kut.ydjk.org.cn

Go:   // 无重载：用不同函数名
来源：http://kqn.gzhubu.top

Ruby: # 无重载：靠动态参数
来源：http://clh.sweek.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://piv.zycfv.cn

================================================================================
来源：http://lyp.ctjpmb.com

D. 数组 / 列表 / 集合
来源：http://ozz.ywan-chungtsiang.top

================================================================================
来源：http://heh.hesvh.cn

[D01] 创建数组 / 列表
来源：http://bfb.snrcjt.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hxm.yuxming.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ohx.wangdashe.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gey.shuidangran.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://khs.bbcook.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jxy.epnwcf.com

Go:   arr := []int{1, 2, 3}
来源：http://vwe.vehdjk.com

Ruby: arr = [1, 2, 3]
来源：http://lqh.yfazqb.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://itw.ybcxt.top

[D02] 追加元素到末尾
来源：http://rpj.yj20258.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ggh.hammf.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yqh.ppjwa.cn

JS:   arr.push(4);
来源：http://wpp.xingfuxueyuan.xyz

TS:   arr.push(4);
来源：http://tum.chenzaomai.com

Java: list.add(4);
来源：http://rvl.havefunace.top

Go:   arr = append(arr, 4)
来源：http://weo.jianghu66.top

Ruby: arr << 4; arr.push(5)
来源：http://kka.gotoacloud.top

C#:   list.Add(4);
来源：http://tsb.vehdjk.com

[D03] 在指定位置插入元素
来源：http://qxu.zhongyouzk.top

Py:   arr.insert(0, 0)
来源：http://edi.fktsv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zkk.zycfv.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wrx.zhijiandao.cn

TS:   arr.splice(0, 0, 0);
来源：http://hna.daxiang520.top

Java: list.add(0, 0);
来源：http://fvl.ydzc1.top

Go:   arr = append([]int{0}, arr...)
来源：http://hnb.xuanzx.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://odt.yongpay.top

C#:   list.Insert(0, 0);
来源：http://tby.mhx1999.top

[D04] 删除元素
来源：http://ame.jinqigufen.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xur.ehwqpu.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jie.yonumen.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gdi.yvedp.cn

TS:   arr.splice(0, 1);
来源：http://syx.aibaodan.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://njf.andypj.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zct.ppjwa.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://usv.hcnkem.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://umq.zhiwuduotai.top

[D05] 访问与修改元素
来源：http://ipr.uphjek.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vzo.wangshuangyany.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://eca.sjlbkw.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://prx.fanxiaobao.xyz

TS:   arr[0]; arr.at(-1);
来源：http://ofx.gzhubu.top

Java: list.get(0); list.set(0, 9);
来源：http://bbb.haohaochexian.top

Go:   arr[0]; arr[0] = 9
来源：http://hpz.52xcode.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bsp.gzhubu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vko.zycfv.cn

[D06] 数组长度
来源：http://tfr.cheryme.top

Py:   len(arr)
来源：http://xih.xuetiantiany.cn

PHP:  count($arr);
来源：http://iro.wangshuangyany.cn

JS:   arr.length
来源：http://tiq.iojbl.cn

TS:   arr.length
来源：http://xon.bjfxy.top

Java: list.size();
来源：http://lzs.feifeiyinyue.top

Go:   len(arr)
来源：http://xed.gogol.net.cn

Ruby: arr.length; arr.size
来源：http://rxf.sysykeji.top

C#:   list.Count;
来源：http://vzn.yj20258.top

[D07] 切片 / 取子数组
来源：http://ccu.chenzaomai.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://smh.zhoulong.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://inn.xuanzx.com

JS:   arr.slice(1, 4);
来源：http://kbj.aibaodan.cn

TS:   arr.slice(1, 4);
来源：http://gcp.xinyue.icu

Java: list.subList(1, 4);
来源：http://pjn.zhijiandao.cn

Go:   arr[1:4]
来源：http://vpe.jlsjyb.cn

Ruby: arr[1, 3]
来源：http://nhf.xziqi.cn

C#:   list.GetRange(1, 3);
来源：http://ccf.yanxiufei.cn

[D08] 合并两个数组
来源：http://jce.mhx1999.top

Py:   a + b;  a.extend(b)
来源：http://nbs.kuanghao11.cn

PHP:  array_merge($a, $b);
来源：http://jec.snrcjt.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://agm.ybcxt.top

TS:   [...a, ...b];
来源：http://zii.ydzc1.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vsk.zdbjq.cn

Go:   append(a, b...)
来源：http://hlq.jqgufenzy.top

Ruby: a + b;  a.concat(b)
来源：http://itm.gzhubu.top

C#:   a.Concat(b).ToList()
来源：http://sij.fanxiaobao.xyz

[D09] 排序（升序）
来源：http://gfg.hysaishi.cn

Py:   sorted(arr);  arr.sort()
来源：http://erq.dianchejie.cn

PHP:  sort($arr);
来源：http://oxo.hfpthk.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://riy.tian-w.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://jst.jqgufenzy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://cna.tianlin.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vqp.iojbl.cn

Ruby: arr.sort
来源：http://dae.svipenyu.cn

C#:   list.Sort();
来源：http://cft.yuanzhike.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://cpt.ctjpmb.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yhk.jianghu66.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ljb.svipenyu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rbc.jlsjyb.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dpg.yvedp.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qcs.zhengqikj.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sws.hesvh.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wir.0kj1m.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ure.zhaomingkeji.xyz

[D11] 反转数组
来源：http://gbw.aizwys.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qql.9152youxi.cn

PHP:  array_reverse($arr);
来源：http://zpr.andypj.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ame.hysaishi.cn

TS:   [...arr].reverse();
来源：http://oyw.pengpengdd.cyou

Java: Collections.reverse(list);
来源：http://xce.jinyuanbaomall.cn

Go:   slices.Reverse(arr)
来源：http://izj.guowangkeji.top

Ruby: arr.reverse
来源：http://nlb.gotoacloud.top

C#:   list.Reverse();
来源：http://emu.jinqigufen.top

[D12] 查找元素下标
来源：http://rzt.sweek.top

Py:   arr.index(x);  x in arr
来源：http://kjp.wangshuangyany.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xcf.hnxiangtu.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hap.zhijiandao.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bfx.yuxming.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rwe.yuxming.cn

Go:   slices.Index(arr, x)
来源：http://nzi.zdbjq.cn

Ruby: arr.index(x)
来源：http://guk.dashuyun.cn

C#:   list.IndexOf(x);
来源：http://ogv.sysykeji.top

[D13] 过滤（保留满足条件的）
来源：http://rqg.iojbl.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jcg.aibaodan.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rmm.yj20258.top

JS:   arr.filter(x => x > 3)
来源：http://iwk.zhaomingkeji.xyz

TS:   arr.filter(x => x > 3)
来源：http://oef.yangfankeji.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zwh.daxiang520.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hnz.xinyue.icu

Ruby: arr.select { |x| x > 3 }
来源：http://afr.dianchejie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://tyn.xingfuxueyuan.xyz

[D14] 映射转换（每个元素变形）
来源：http://hvu.9152youxi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ikf.wangshuangyany.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ybb.gzhubu.top

JS:   arr.map(x => x * 2)
来源：http://lpd.jinqigufen.top

TS:   arr.map(x => x * 2)
来源：http://yyn.yfazqb.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://dug.cashguo.top

Go:   // 手写循环
来源：http://tpz.shangyingyoupin.top

Ruby: arr.map { |x| x * 2 }
来源：http://rkw.hnqzz.top

C#:   list.Select(x => x * 2).ToList()
来源：http://dir.sjlbkw.cn

[D15] 去重
来源：http://fen.ehwqpu.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xsx.shanyushiyangtech.top

PHP:  array_unique($arr);
来源：http://uhv.pycfn.com

JS:   [...new Set(arr)]
来源：http://ped.ctjpmb.com

TS:   [...new Set(arr)]
来源：http://cdr.yongpay.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kuo.yonumen.top

Go:   // 用 map[T]struct{} 手写
来源：http://jvk.svipenyu.cn

Ruby: arr.uniq
来源：http://lhf.yueranfly.top

C#:   list.Distinct().ToList()
来源：http://jhl.aibaodan.cn

[D16] 求和与平均值
来源：http://cqt.hfpthk.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rcg.vehdjk.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://avs.jinqigufen.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ndq.daxiang520.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bdt.chenzaomai.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fwz.vehdjk.com

Go:   // 手写循环累加
来源：http://muq.0kj1m.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://oqs.ppjwa.cn

C#:   list.Sum();  list.Average()
来源：http://moz.quarkkingdee.top

[D17] 最大值与最小值
来源：http://dvy.gaohongyu789.top

Py:   max(arr);  min(arr)
来源：http://bnw.fengsongda.top


<!-- 参考信息 -->