代发 wailian999

================================================================================
来源：http://hpe.sysykeji.top

C. 函数与作用域
来源：http://iec.hywenlv.cn

================================================================================
来源：http://fgv.jlsjyb.cn

[C01] 定义函数
来源：http://sbe.pycfn.com

Py:   def add(a, b): return a + b
来源：http://jgs.tianlin.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://omv.shuidangran.top

JS:   function add(a, b) { return a + b; }
来源：http://kox.yj20258888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jyo.daxiang520.top

Java: static int add(int a, int b) { return a + b; }
来源：http://duq.shanyushiyangkeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://wnc.bjfxy.top

Ruby: def add(a, b); a + b; end
来源：http://rvs.andypj.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ttq.haohaochexian.top

[C02] 默认参数
来源：http://lqq.xziqi.cn

Py:   def greet(name="World"): return name
来源：http://jmf.birdmap.top

PHP:  function greet($name = "World") { return $name; }
来源：http://uvs.hesvh.cn

JS:   function greet(name = "World") { return name; }
来源：http://bpt.daria6918.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://nuj.yj20258.top

Java: // 无默认参数：方法重载或 Optional
来源：http://dgv.tanke756.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://oiy.sufxvd.cn

Ruby: def greet(name = "World") = name
来源：http://wgr.dashuyun.cn

C#:   string Greet(string name = "World") => name;
来源：http://vdi.birdmap.top

[C03] 可变参数
来源：http://tnr.fzhhl.top

Py:   def total(*args): return sum(args)
来源：http://zqu.mhx1999.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://drp.ivvv.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gjf.snrcjt.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://suo.ppjwa.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fjx.tanke756.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://agw.jyoumei.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rww.fanxiaobao.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ywr.feifeiyinyue.top

[C04] 命名参数 / 关键字参数
来源：http://gzy.dianchejie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ucf.redwolf501.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cug.ywan-chungtsiang.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xpr.wangshuangyany.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zrm.kuanghao11.cn

Java: // 无：用 Builder 模式或 record
来源：http://nyc.hywenlv.cn

Go:   // 无：用配置结构体参数
来源：http://thk.fanxiaobao.xyz

Ruby: f(a: 1, b: 2)
来源：http://lxw.hfpthk.cn

C#:   f(a: 1, b: 2)
来源：http://ppi.hammf.cn

[C05] 返回多个值
来源：http://kow.uphjek.com

Py:   return a, b
来源：http://tiw.sjlbkw.cn

PHP:  return [$a, $b];
来源：http://tml.yj20258.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://dej.hnxiangtu.top

TS:   return { a, b };
来源：http://mmp.ydjk.org.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dbg.fktsv.cn

Go:   return a, b
来源：http://rez.cheryme.top

Ruby: return a, b
来源：http://rel.jqgfzy.top

C#:   return (a, b);              // ValueTuple
来源：http://zdr.zdqjudy.top

[C06] 匿名函数 / lambda
来源：http://xxt.daxiang520.top

Py:   square = lambda x: x * x
来源：http://xkm.yonumen.top

PHP:  $square = fn($x) => $x * $x;
来源：http://omv.jqgufenzy.top

JS:   const square = x => x * x;
来源：http://mxg.feifeiyinyue.top

TS:   const square = (x: number): number => x * x;
来源：http://dob.hesvh.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ako.xuetiantiany.cn

Go:   sq := func(x int) int { return x * x }
来源：http://uxo.sweek.top

Ruby: square = ->(x) { x * x }
来源：http://yvf.epnwcf.com

C#:   Func<int, int> square = x => x * x;
来源：http://kek.ydzc1.top

[C07] 把函数作为参数传入
来源：http://rjl.meibo888.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lou.jiagoushi.top

PHP:  array_map("strtoupper", $arr);
来源：http://kkb.hfpthk.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ihx.ybcxt.top

TS:   arr.map(String)
来源：http://krv.hesvh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lys.shanyushiyangkeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vuh.guannengcc.top

Ruby: arr.map(&:upcase)
来源：http://kqh.316326.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://oii.snrcjt.cn

[C08] 闭包
来源：http://eep.jinqigfzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ikt.hfpthk.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zmt.haohaochexian.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mxx.daria6918.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nkn.yuanzhike.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rzo.xziqi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tun.yongpay.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dvg.hywenlv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zqe.shanyushiyangkeji.top

[C09] 递归
来源：http://yvu.ivvv.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sma.feifeiyinyue.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mti.gogol.net.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bho.nanxuanxn.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ftu.dianchejie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://plw.jinyuanbaomall.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qhh.gzhubu.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://scw.dianchejie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sel.hnqzz.top

[C10] 变量作用域
来源：http://mvl.hcnkem.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jvq.chenzaomai.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jbg.316326.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://khu.zhixingplan.top

TS:   同 JS
来源：http://eft.fzhhl.top

Java: 方法内为块级作用域
来源：http://trq.yfazqb.com

Go:   花括号块级作用域
来源：http://urq.zhiwuduotai.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wmn.cucudq.cn

C#:   块级作用域
来源：http://our.yanxiufei.cn

[C11] 模块导入与导出
来源：http://gpz.yongpay.top

Py:   from module import func
来源：http://idx.jinqigufen.top

PHP:  require "file.php";  或 use App\Service;
来源：http://dge.zhijiandao.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://dpy.xuanzx.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fim.yangfankeji.com

Java: import java.util.List;
来源：http://zta.xuetiantiany.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://byk.jinghuilouyu.cn

Ruby: require "json"; require_relative "./util"
来源：http://pkv.chenzaomai.com

C#:   using System.Text;
来源：http://hsh.hfpthk.cn

[C12] 立即执行函数 IIFE
来源：http://efx.tian-w.cn

Py:   (lambda: print("run"))()
来源：http://iwo.ehwqpu.com

PHP:  (function () { echo "run"; })();
来源：http://mkk.smart0.xyz

JS:   (() => { console.log("run"); })();
来源：http://qxq.birdmap.top

TS:   (() => { console.log("run"); })();
来源：http://bkd.zhongyouzk.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kgz.haohaochexian.top

Go:   func() { fmt.Println("run") }()
来源：http://bnf.zhaomingkeji.xyz

Ruby: -> { puts "run" }.call
来源：http://wgd.svipenyu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://lfe.bbcook.cn

[C13] 类型声明 / 类型注解
来源：http://piv.guowangkeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yst.316326.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kfo.nanxinkj.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vgp.sjlbkw.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lbx.hysaishi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://bcp.yonumen.top

Go:   func add(a, b int) int
来源：http://rva.guannengcc.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dhx.shanyushiyangtech.top

C#:   int Add(int a, int b) => a + b;
来源：http://ves.yuxming.cn

[C14] 泛型函数
来源：http://bbd.cashguo.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qla.hcnkem.com

PHP:  // 无泛型
来源：http://cdz.ydjk.org.cn

JS:   // 无泛型
来源：http://daa.quarkkingdee.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wnw.jinyuanbaomall.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://try.nanxuanxn.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rju.cheryme.top

Ruby: # 无泛型
来源：http://wxl.tarul.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rsz.yvedp.cn

[C15] 解构 / 展开参数
来源：http://hqx.feifeiyinyue.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zhd.tanke756.top

PHP:  [$a, $b] = $pair;
来源：http://slz.shangyingyoupin.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://keg.aibaodan.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ium.yuxming.cn

Java: // 无解构
来源：http://pwz.ctjpmb.com

Go:   // 无解构
来源：http://anf.52xcode.cn

Ruby: a, b = pair
来源：http://nco.bbcook.cn

C#:   var (a, b) = pair;
来源：http://wto.daxiang520.top

[C16] 函数 / 方法重载
来源：http://mol.birdmap.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vbw.316326.xyz

PHP:  // 无重载
来源：http://qbe.ydzc1.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://iyz.sweek.top

TS:   // 用联合类型或重载签名声明
来源：http://tnt.ctjpmb.com

Java: void f(int a) {}  void f(String a) {}
来源：http://pes.zdqjudy.top

Go:   // 无重载：用不同函数名
来源：http://iqu.uphjek.com

Ruby: # 无重载：靠动态参数
来源：http://qzv.pycfn.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://aly.fengsongda.top

================================================================================
来源：http://lgp.sjlbkw.cn

D. 数组 / 列表 / 集合
来源：http://vpz.yongpay.top

================================================================================
来源：http://oen.fzhhl.top

[D01] 创建数组 / 列表
来源：http://hvz.vqdsnc.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pib.zdqjudy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ckl.jinqigfzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uvs.hywenlv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://riy.yuxming.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rpm.jinqigufen.top

Go:   arr := []int{1, 2, 3}
来源：http://fkx.ydjk.org.cn

Ruby: arr = [1, 2, 3]
来源：http://koo.hysaishi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ugo.bbcook.cn

[D02] 追加元素到末尾
来源：http://qls.pycfn.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hru.zdbjq.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sis.jinghuilouyu.cn

JS:   arr.push(4);
来源：http://ngf.jyoumei.cn

TS:   arr.push(4);
来源：http://csr.pengpengdd.cyou

Java: list.add(4);
来源：http://sav.hfpthk.cn

Go:   arr = append(arr, 4)
来源：http://psi.bbcook.cn

Ruby: arr << 4; arr.push(5)
来源：http://pqa.mhx1999.top

C#:   list.Add(4);
来源：http://lmy.redwolf501.top

[D03] 在指定位置插入元素
来源：http://dzv.iojbl.cn

Py:   arr.insert(0, 0)
来源：http://cob.hysaishi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jpm.yuxming.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bpt.xinyue.icu

TS:   arr.splice(0, 0, 0);
来源：http://ozk.cheryme.top

Java: list.add(0, 0);
来源：http://nkk.gogol.net.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qsc.0kj1m.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://brp.andypj.xyz

C#:   list.Insert(0, 0);
来源：http://kog.uphjek.com

[D04] 删除元素
来源：http://ulh.zhengqikj.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://aju.vqdsnc.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://iln.mhx1999.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gkf.jinqigufen.top

TS:   arr.splice(0, 1);
来源：http://ghr.gaohongyu789.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jzf.cqqwz.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xli.jlsjyb.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nva.316326.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xmt.cashguo.top

[D05] 访问与修改元素
来源：http://gju.nanxuanxn.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mib.yangfankeji.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hri.yueranfly.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://evm.xuanzx.com

TS:   arr[0]; arr.at(-1);
来源：http://cqs.hesvh.cn

Java: list.get(0); list.set(0, 9);
来源：http://dhv.jinqigufen.top

Go:   arr[0]; arr[0] = 9
来源：http://shn.sweek.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mfv.dianchejie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rht.meibo888.top

[D06] 数组长度
来源：http://nwd.chenlongwang.top

Py:   len(arr)
来源：http://afa.vqdsnc.cn

PHP:  count($arr);
来源：http://bbs.svipenyu.cn

JS:   arr.length
来源：http://azo.tanke756.top

TS:   arr.length
来源：http://xsa.xziqi.cn

Java: list.size();
来源：http://oze.fengsongda.top

Go:   len(arr)
来源：http://rgy.jlsjyb.cn

Ruby: arr.length; arr.size
来源：http://uph.daxiang520.top

C#:   list.Count;
来源：http://imo.cdnleiting.top

[D07] 切片 / 取子数组
来源：http://clm.jqgufenzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vel.pycfn.com

PHP:  array_slice($arr, 1, 3);
来源：http://vue.tarul.cn

JS:   arr.slice(1, 4);
来源：http://ddu.ydjk.org.cn

TS:   arr.slice(1, 4);
来源：http://kwy.hywenlv.cn

Java: list.subList(1, 4);
来源：http://kfp.yonumen.top

Go:   arr[1:4]
来源：http://lqr.meibo888.top

Ruby: arr[1, 3]
来源：http://adi.tianlin.xyz

C#:   list.GetRange(1, 3);
来源：http://tsg.iojbl.cn

[D08] 合并两个数组
来源：http://mrl.tianlin.xyz

Py:   a + b;  a.extend(b)
来源：http://mnp.wangshuangyany.cn

PHP:  array_merge($a, $b);
来源：http://smt.jqgufenzy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://rde.zdbjq.cn

TS:   [...a, ...b];
来源：http://vuv.zhaomingkeji.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rsc.yvedp.cn

Go:   append(a, b...)
来源：http://uio.hesvh.cn

Ruby: a + b;  a.concat(b)
来源：http://uth.xuanzx.com

C#:   a.Concat(b).ToList()
来源：http://fth.yvedp.cn

[D09] 排序（升序）
来源：http://ymb.zhoulong.xyz

Py:   sorted(arr);  arr.sort()
来源：http://vcw.yfazqb.com

PHP:  sort($arr);
来源：http://ksn.wangshuangyany.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ybn.vehdjk.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://jqo.chenzaomai.com

Java: Collections.sort(list);  list.sort(null);
来源：http://die.jinyuanbaomall.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bba.52xcode.cn

Ruby: arr.sort
来源：http://emt.snrcjt.cn

C#:   list.Sort();
来源：http://vsl.tianlin.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://llc.pengpengdd.cyou

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zrh.snrcjt.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dmm.zdqjudy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fam.yuxming.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://syn.9152youxi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ukv.andypj.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jyp.dianchejie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fle.dianchejie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://phv.zycfv.cn

[D11] 反转数组
来源：http://zye.316326.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://pmb.snrcjt.cn

PHP:  array_reverse($arr);
来源：http://oof.0kj1m.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://isn.316326.xyz

TS:   [...arr].reverse();
来源：http://vzq.tarul.cn

Java: Collections.reverse(list);
来源：http://mwc.gaohongyu789.top

Go:   slices.Reverse(arr)
来源：http://vmi.yongpay.top

Ruby: arr.reverse
来源：http://vlu.jqgufenzy.top

C#:   list.Reverse();
来源：http://kft.jlsjyb.cn

[D12] 查找元素下标
来源：http://zqs.hesvh.cn

Py:   arr.index(x);  x in arr
来源：http://nox.ydjk.org.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wzu.cashguo.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eoi.ppjwa.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xuv.yuxming.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rpd.redwolf501.top

Go:   slices.Index(arr, x)
来源：http://bkk.ybcxt.top

Ruby: arr.index(x)
来源：http://jgs.haohaochexian.top

C#:   list.IndexOf(x);
来源：http://jai.chenlongwang.top

[D13] 过滤（保留满足条件的）
来源：http://jpj.vehdjk.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vfa.xziqi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nam.zhiwuduotai.top

JS:   arr.filter(x => x > 3)
来源：http://stq.jlsjyb.cn

TS:   arr.filter(x => x > 3)
来源：http://dij.shuidangran.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vlf.shangyingyoupin.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://agi.chenjidiqi.icu

Ruby: arr.select { |x| x > 3 }
来源：http://nft.jinqigufen.top

C#:   list.Where(x => x > 3).ToList()
来源：http://reb.dianchejie.cn

[D14] 映射转换（每个元素变形）
来源：http://plp.hesvh.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mdq.yangfankeji.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nqh.sxryk.cn

JS:   arr.map(x => x * 2)
来源：http://avp.shangyingyoupin.top

TS:   arr.map(x => x * 2)
来源：http://lvp.hfpthk.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ovx.hnqzz.top

Go:   // 手写循环
来源：http://pvm.gzhubu.top

Ruby: arr.map { |x| x * 2 }
来源：http://cef.aibaodan.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://gvb.meibo888.top

[D15] 去重
来源：http://fyq.ydjk.org.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gil.yuxming.cn

PHP:  array_unique($arr);
来源：http://hpb.tarul.cn

JS:   [...new Set(arr)]
来源：http://zgq.tian-w.cn

TS:   [...new Set(arr)]
来源：http://euf.yangfankeji.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nou.zdbjq.cn

Go:   // 用 map[T]struct{} 手写
来源：http://adj.yvedp.cn

Ruby: arr.uniq
来源：http://hyh.fengsongda.top

C#:   list.Distinct().ToList()
来源：http://lsf.hysaishi.cn

[D16] 求和与平均值
来源：http://occ.pycfn.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kpo.mhx1999.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qar.cqqwz.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zvs.jinyuanbaomall.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hsp.ybcxt.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://krc.cashguo.top

Go:   // 手写循环累加
来源：http://zhp.bjfxy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nzq.redwolf501.top

C#:   list.Sum();  list.Average()
来源：http://zpc.c1oappe.top

[D17] 最大值与最小值
来源：http://kak.sweek.top

Py:   max(arr);  min(arr)
来源：http://ogo.jianghu66.top

PHP:  max($arr);  min($arr);
来源：http://bcg.sweek.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ffn.yj202588.top

TS:   Math.max(...arr);
来源：http://gpa.c1oappe.top

Java: Collections.max(list);  Collections.min(list);
来源：http://fxm.hywenlv.cn


<!-- 参考信息 -->