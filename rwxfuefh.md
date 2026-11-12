代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://egq.bjfxy.top

[C03] 可变参数
来源：http://ugz.nwbrower.top

Py:   def total(*args): return sum(args)
来源：http://lga.meibo888.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://flt.fehbvm.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://boz.cheryme.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nuz.uphjek.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xtq.fengsongda.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://geq.zhengqikj.top

Ruby: def total(*nums); nums.sum; end
来源：http://syw.xylfe.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tzt.zhaomingkeji.xyz

[C04] 命名参数 / 关键字参数
来源：http://fqk.cheryme.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xut.yj20258.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qtj.fanxiaobao.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kdk.pengpengdd.cyou

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wol.haohaochexian.top

Java: // 无：用 Builder 模式或 record
来源：http://xvq.tian-w.cn

Go:   // 无：用配置结构体参数
来源：http://bbp.yuxming.cn

Ruby: f(a: 1, b: 2)
来源：http://klq.ydzc1.top

C#:   f(a: 1, b: 2)
来源：http://mrk.zhengqikj.top

[C05] 返回多个值
来源：http://zga.cucudq.cn

Py:   return a, b
来源：http://idw.vqdsnc.cn

PHP:  return [$a, $b];
来源：http://bzj.cqqwz.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://esj.xuetiantiany.cn

TS:   return { a, b };
来源：http://cnt.birdmap.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://umg.jinyuanbaomall.cn

Go:   return a, b
来源：http://pim.aizwys.cn

Ruby: return a, b
来源：http://wyh.c1oappe.top

C#:   return (a, b);              // ValueTuple
来源：http://iew.vqdsnc.cn

[C06] 匿名函数 / lambda
来源：http://hxk.xuanzx.com

Py:   square = lambda x: x * x
来源：http://znw.gotoacloud.top

PHP:  $square = fn($x) => $x * $x;
来源：http://twc.zdqjudy.top

JS:   const square = x => x * x;
来源：http://hbq.hammf.cn

TS:   const square = (x: number): number => x * x;
来源：http://yqt.fanxiaobao.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jwj.jqgufenzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://qzu.zycfv.cn

Ruby: square = ->(x) { x * x }
来源：http://clq.chenzaomai.com

C#:   Func<int, int> square = x => x * x;
来源：http://rdb.meibo888.top

[C07] 把函数作为参数传入
来源：http://bpj.cucudq.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xrj.dianchejie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ycc.yonumen.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hyp.tian-w.cn

TS:   arr.map(String)
来源：http://xzf.hesvh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uzb.yfazqb.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jdw.sxryk.cn

Ruby: arr.map(&:upcase)
来源：http://csm.jianghu66.top

C#:   arr.Select(s => s.ToUpper())
来源：http://dik.vqdsnc.cn

[C08] 闭包
来源：http://xzm.vqdsnc.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zjo.sufxvd.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cut.meibo888.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lbk.316326.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mtk.jqgfzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bxp.wangdashe.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pqo.zycfv.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xtv.316326.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wrj.jiagoushi.top

[C09] 递归
来源：http://eys.shanyushiyangkeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dcy.zhixingplan.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bmx.feifeiyinyue.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yel.jqgfzy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://usg.dianchejie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fws.jinyuanbaomall.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sao.yuxming.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ako.hesvh.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gwy.shuidangran.top

[C10] 变量作用域
来源：http://tdq.xuetiantiany.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lgr.yanxiufei.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gwp.jlsjyb.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ppu.shzxlz.cn

TS:   同 JS
来源：http://udg.hnxiangtu.top

Java: 方法内为块级作用域
来源：http://wpr.ydjk.org.cn

Go:   花括号块级作用域
来源：http://vvq.hammf.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nnx.bbcook.cn

C#:   块级作用域
来源：http://hth.shuidangran.top

[C11] 模块导入与导出
来源：http://jxp.mhx1999.top

Py:   from module import func
来源：http://obz.shanyushiyangtech.top

PHP:  require "file.php";  或 use App\Service;
来源：http://icp.gaohongyu789.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://jig.ydjk.org.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cde.hnqzz.top

Java: import java.util.List;
来源：http://xlo.jinqigufen.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tqv.fanxiaobao.xyz

Ruby: require "json"; require_relative "./util"
来源：http://wht.zhongyouzk.top

C#:   using System.Text;
来源：http://rco.meibo888.top

[C12] 立即执行函数 IIFE
来源：http://ppi.ydzc1.top

Py:   (lambda: print("run"))()
来源：http://txx.smart0.xyz

PHP:  (function () { echo "run"; })();
来源：http://egk.wangshuangyany.cn

JS:   (() => { console.log("run"); })();
来源：http://qhz.cheryme.top

TS:   (() => { console.log("run"); })();
来源：http://vhk.nanxuanxn.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dso.chenzaomai.com

Go:   func() { fmt.Println("run") }()
来源：http://rml.ctjpmb.com

Ruby: -> { puts "run" }.call
来源：http://myb.cucudq.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ema.zdqjudy.top

[C13] 类型声明 / 类型注解
来源：http://uha.ehwqpu.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kad.fanxiaobao.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://feg.yonumen.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ddl.mhx1999.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bce.hcnkem.com

Java: int add(int a, int b) { return a + b; }
来源：http://pnx.yueranfly.top

Go:   func add(a, b int) int
来源：http://odf.jlsjyb.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nlv.zhijiandao.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nqg.shuidangran.top

[C14] 泛型函数
来源：http://wop.9152youxi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://eub.bbcook.cn

PHP:  // 无泛型
来源：http://vuv.fehbvm.com

JS:   // 无泛型
来源：http://deq.wangshuangyany.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rpz.fehbvm.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dml.cheryme.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pcu.guannengcc.top

Ruby: # 无泛型
来源：http://nxw.zhijiandao.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gva.jqgufenzy.top

[C15] 解构 / 展开参数
来源：http://ggf.daxiang520.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ylm.pycfn.com

PHP:  [$a, $b] = $pair;
来源：http://mtd.chenjidiqi.icu

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wko.fzhhl.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wax.zhiwuduotai.top

Java: // 无解构
来源：http://zzb.cucudq.cn

Go:   // 无解构
来源：http://urq.xylfe.cn

Ruby: a, b = pair
来源：http://rns.svipenyu.cn

C#:   var (a, b) = pair;
来源：http://fto.52xcode.cn

[C16] 函数 / 方法重载
来源：http://hvw.jianghu66.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dya.tianlin.xyz

PHP:  // 无重载
来源：http://ynn.hywenlv.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://mfp.ctjpmb.com

TS:   // 用联合类型或重载签名声明
来源：http://idh.hongshengwenyu.top

Java: void f(int a) {}  void f(String a) {}
来源：http://clq.jinghuilouyu.cn

Go:   // 无重载：用不同函数名
来源：http://mpv.yvedp.cn

Ruby: # 无重载：靠动态参数
来源：http://ioq.chenlongwang.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://jaf.ywan-chungtsiang.top

================================================================================
来源：http://xbk.shzxlz.cn

D. 数组 / 列表 / 集合
来源：http://qxs.zhaomingkeji.xyz

================================================================================
来源：http://efz.sxryk.cn

[D01] 创建数组 / 列表
来源：http://zlw.52xcode.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pur.havefunace.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://upa.shzxlz.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jar.yangfankeji.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://crx.yuxming.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rfv.nanxuanxn.top

Go:   arr := []int{1, 2, 3}
来源：http://xpc.yanxiufei.cn

Ruby: arr = [1, 2, 3]
来源：http://qms.shanyushiyangtech.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://owd.yonumen.top

[D02] 追加元素到末尾
来源：http://gll.pycfn.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rbx.xuetiantiany.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qos.snrcjt.cn

JS:   arr.push(4);
来源：http://byy.tianlin.xyz

TS:   arr.push(4);
来源：http://pji.zhixingplan.top

Java: list.add(4);
来源：http://hml.bbcook.cn

Go:   arr = append(arr, 4)
来源：http://trw.aizwys.cn

Ruby: arr << 4; arr.push(5)
来源：http://pfd.zhixingplan.top

C#:   list.Add(4);
来源：http://wzf.pengpengdd.cyou

[D03] 在指定位置插入元素
来源：http://hsm.sxryk.cn

Py:   arr.insert(0, 0)
来源：http://rvg.gogol.net.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://otg.gzhubu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nar.mhx1999.top

TS:   arr.splice(0, 0, 0);
来源：http://fqs.tianlin.xyz

Java: list.add(0, 0);
来源：http://lsa.jqgfzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://ldp.yvedp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xtr.nanxuanxn.top

C#:   list.Insert(0, 0);
来源：http://mna.dashuyun.cn

[D04] 删除元素
来源：http://mgc.fktsv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wnt.tianlin.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gow.sxryk.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ixp.zhixingplan.top

TS:   arr.splice(0, 1);
来源：http://pth.fehbvm.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cou.fanxiaobao.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ycq.redwolf501.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kbi.nanxuanxn.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tzg.hcnkem.com

[D05] 访问与修改元素
来源：http://ktr.xuanzx.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ezu.guowangkeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://eor.hfpthk.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://puy.aibaodan.cn

TS:   arr[0]; arr.at(-1);
来源：http://wke.hywenlv.cn

Java: list.get(0); list.set(0, 9);
来源：http://upd.chenzaomai.com

Go:   arr[0]; arr[0] = 9
来源：http://gxv.xylfe.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uri.jyoumei.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gro.gotoacloud.top

[D06] 数组长度
来源：http://xjk.bjfxy.top

Py:   len(arr)
来源：http://cbr.nanxinkj.top

PHP:  count($arr);
来源：http://csj.jinghuilouyu.cn

JS:   arr.length
来源：http://jvx.jinghuilouyu.cn

TS:   arr.length
来源：http://ygt.yueranfly.top

Java: list.size();
来源：http://zja.redwolf501.top

Go:   len(arr)
来源：http://urv.jinqigufen.top

Ruby: arr.length; arr.size
来源：http://aqq.guowangkeji.top

C#:   list.Count;
来源：http://cfp.shangyingyoupin.top

[D07] 切片 / 取子数组
来源：http://cjc.daxiang520.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mjn.zhengqikj.top

PHP:  array_slice($arr, 1, 3);
来源：http://thj.hnxiangtu.top

JS:   arr.slice(1, 4);
来源：http://szi.svipenyu.cn

TS:   arr.slice(1, 4);
来源：http://ukm.yueranfly.top

Java: list.subList(1, 4);
来源：http://egg.yj202588.top

Go:   arr[1:4]
来源：http://qvk.shanyushiyangtech.top

Ruby: arr[1, 3]
来源：http://ktk.fehbvm.com

C#:   list.GetRange(1, 3);
来源：http://ppu.xingfuxueyuan.xyz

[D08] 合并两个数组
来源：http://uis.yuanzhike.top

Py:   a + b;  a.extend(b)
来源：http://noh.xziqi.cn

PHP:  array_merge($a, $b);
来源：http://eif.jinghuilouyu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qkj.bjfxy.top

TS:   [...a, ...b];
来源：http://tgi.yanxiufei.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ccq.vehdjk.com

Go:   append(a, b...)
来源：http://rjl.zhongyouzk.top

Ruby: a + b;  a.concat(b)
来源：http://leh.tian-w.cn

C#:   a.Concat(b).ToList()
来源：http://jqw.havefunace.top

[D09] 排序（升序）
来源：http://bhg.wangshuangyany.cn

Py:   sorted(arr);  arr.sort()
来源：http://yhc.daxiang520.top

PHP:  sort($arr);
来源：http://zvd.wangdashe.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bup.ywan-chungtsiang.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://svj.pycfn.com

Java: Collections.sort(list);  list.sort(null);
来源：http://dji.nanxinkj.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pjd.yuanzhike.top

Ruby: arr.sort
来源：http://zqq.yanxiufei.cn

C#:   list.Sort();
来源：http://bhw.xylfe.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://wwn.xylfe.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wgf.meibo888.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vmc.kuanghao11.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dia.feifeiyinyue.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nqq.zycfv.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jpk.tanke756.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rba.xuetiantiany.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fvs.xuanzx.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://irw.c1oappe.top

[D11] 反转数组
来源：http://osy.tian-w.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zrc.fzhhl.top

PHP:  array_reverse($arr);
来源：http://jta.fanxiaobao.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tyq.shzxlz.cn

TS:   [...arr].reverse();
来源：http://dux.aizwys.cn

Java: Collections.reverse(list);
来源：http://gqb.chenzaomai.com

Go:   slices.Reverse(arr)
来源：http://bai.ydzc1.top

Ruby: arr.reverse
来源：http://jgp.hesvh.cn

C#:   list.Reverse();
来源：http://ffx.gogol.net.cn

[D12] 查找元素下标
来源：http://mma.yongpay.top

Py:   arr.index(x);  x in arr
来源：http://gsj.cashguo.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rdq.zhoulong.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hvc.chenjidiqi.icu

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rom.quarkkingdee.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hpp.fengsongda.top

Go:   slices.Index(arr, x)
来源：http://meh.nanxuanxn.top

Ruby: arr.index(x)
来源：http://pgn.chenzaomai.com

C#:   list.IndexOf(x);
来源：http://fgj.xuanzx.com

[D13] 过滤（保留满足条件的）
来源：http://eie.zhijiandao.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rcu.iojbl.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hks.guannengcc.top

JS:   arr.filter(x => x > 3)
来源：http://upc.316326.xyz

TS:   arr.filter(x => x > 3)
来源：http://gby.feifeiyinyue.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rjg.yj20258888.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qjs.sjlbkw.cn

Ruby: arr.select { |x| x > 3 }
来源：http://bop.sweek.top

C#:   list.Where(x => x > 3).ToList()
来源：http://urf.shanyushiyangkeji.top

[D14] 映射转换（每个元素变形）
来源：http://kdr.fengsongda.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zvu.ehwqpu.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vsb.hnxiangtu.top

JS:   arr.map(x => x * 2)
来源：http://hcw.birdmap.top

TS:   arr.map(x => x * 2)
来源：http://jci.mhx1999.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://hhr.fehbvm.com

Go:   // 手写循环
来源：http://grp.fzhhl.top

Ruby: arr.map { |x| x * 2 }
来源：http://pag.kuanghao11.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qwq.pengpengdd.cyou

[D15] 去重
来源：http://jdz.fengsongda.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yww.yvedp.cn

PHP:  array_unique($arr);
来源：http://awz.52xcode.cn

JS:   [...new Set(arr)]
来源：http://gtn.yonumen.top

TS:   [...new Set(arr)]
来源：http://rdi.yj20258.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tyv.dianchejie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://mwz.shuidangran.top

Ruby: arr.uniq
来源：http://ftt.tanke756.top

C#:   list.Distinct().ToList()
来源：http://vbi.gzhubu.top

[D16] 求和与平均值
来源：http://gts.jinqigufen.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://oxn.birdmap.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://epx.dianchejie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nvt.wangshuangyany.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ffg.sysykeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ohu.zdbjq.cn

Go:   // 手写循环累加
来源：http://vyi.chenlongwang.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://suf.wangdashe.top

C#:   list.Sum();  list.Average()
来源：http://ptu.zhaomingkeji.xyz

[D17] 最大值与最小值
来源：http://avj.wangdashe.top

Py:   max(arr);  min(arr)
来源：http://yrz.yangfankeji.com

PHP:  max($arr);  min($arr);
来源：http://dxs.bbcook.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gjp.yvedp.cn

TS:   Math.max(...arr);
来源：http://jrf.xziqi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gri.quarkkingdee.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://iyq.yuxming.cn

Ruby: arr.max;  arr.min
来源：http://fju.cqqwz.cn

C#:   list.Max();  list.Min()
来源：http://has.tianlin.xyz

[D18] 扁平化嵌套数组
来源：http://ifl.fehbvm.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gqc.quarkkingdee.top

PHP:  array_merge(...$nested);
来源：http://zzk.guowangkeji.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fbh.0kj1m.cn

TS:   nested.flat();
来源：http://atg.0kj1m.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fpn.chenzaomai.com

Go:   // 手写双层循环
来源：http://jvn.316326.xyz

Ruby: nested.flatten
来源：http://xfh.zhijiandao.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://soi.zycfv.cn

[D19] 按字段分组
来源：http://ajx.gotoacloud.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vps.fanxiaobao.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mxn.nwbrower.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bzf.zhoulong.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://fks.ehwqpu.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ncp.0kj1m.cn

Go:   // 手写 map[string][]T
来源：http://xze.ctjpmb.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://rnq.yuxming.cn


<!-- 参考信息 -->