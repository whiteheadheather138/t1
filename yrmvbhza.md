代发 wailian999

Java: if (data == null) return;
来源：http://guu.gzhubu.top

Go:   if data == nil { return }
来源：http://ufy.smart0.xyz

Ruby: return if data.nil?
来源：http://kka.andypj.xyz

C#:   if (data == null) return;
来源：http://fkc.yfazqb.com

================================================================================
来源：http://lec.ydjk.org.cn

C. 函数与作用域
来源：http://eve.ywan-chungtsiang.top

================================================================================
来源：http://phi.hnqzz.top

[C01] 定义函数
来源：http://kte.fengsongda.top

Py:   def add(a, b): return a + b
来源：http://exg.vehdjk.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bir.pengpengdd.cyou

JS:   function add(a, b) { return a + b; }
来源：http://hhf.fanxiaobao.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rnp.cashguo.top

Java: static int add(int a, int b) { return a + b; }
来源：http://tcq.vqdsnc.cn

Go:   func add(a, b int) int { return a + b }
来源：http://joy.jinqigfzy.top

Ruby: def add(a, b); a + b; end
来源：http://vzt.cucudq.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uex.ctjpmb.com

[C02] 默认参数
来源：http://ofv.pycfn.com

Py:   def greet(name="World"): return name
来源：http://eba.yvedp.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wus.andypj.xyz

JS:   function greet(name = "World") { return name; }
来源：http://thf.jlsjyb.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qvn.xziqi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://lmd.andypj.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zfc.zhaomingkeji.xyz

Ruby: def greet(name = "World") = name
来源：http://fjo.shuidangran.top

C#:   string Greet(string name = "World") => name;
来源：http://cah.svipenyu.cn

[C03] 可变参数
来源：http://yun.zhixingplan.top

Py:   def total(*args): return sum(args)
来源：http://skf.jqgfzy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sin.fengsongda.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jzt.xuetiantiany.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hvv.tanke756.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rjv.chenjidiqi.icu

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nej.jinqigfzy.top

Ruby: def total(*nums); nums.sum; end
来源：http://ari.aizwys.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://aru.meibo888.top

[C04] 命名参数 / 关键字参数
来源：http://jya.hesvh.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qwj.pengpengdd.cyou

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ezr.yueranfly.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rfa.chenlongwang.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://iyr.smart0.xyz

Java: // 无：用 Builder 模式或 record
来源：http://rep.tarul.cn

Go:   // 无：用配置结构体参数
来源：http://qbn.fehbvm.com

Ruby: f(a: 1, b: 2)
来源：http://qqu.jinqigufen.top

C#:   f(a: 1, b: 2)
来源：http://tes.sufxvd.cn

[C05] 返回多个值
来源：http://jda.smart0.xyz

Py:   return a, b
来源：http://rzk.guowangkeji.top

PHP:  return [$a, $b];
来源：http://ujs.ppjwa.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://sip.andypj.xyz

TS:   return { a, b };
来源：http://bzx.jqgfzy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sef.shuidangran.top

Go:   return a, b
来源：http://rkz.chenlongwang.top

Ruby: return a, b
来源：http://uqx.hesvh.cn

C#:   return (a, b);              // ValueTuple
来源：http://ssk.shangyingyoupin.top

[C06] 匿名函数 / lambda
来源：http://bnk.ivvv.top

Py:   square = lambda x: x * x
来源：http://rsw.jyoumei.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://lqn.xuanzx.com

JS:   const square = x => x * x;
来源：http://bna.vqdsnc.cn

TS:   const square = (x: number): number => x * x;
来源：http://uke.wangshuangyany.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hdh.hnqzz.top

Go:   sq := func(x int) int { return x * x }
来源：http://svs.yueranfly.top

Ruby: square = ->(x) { x * x }
来源：http://dxu.epnwcf.com

C#:   Func<int, int> square = x => x * x;
来源：http://kro.chenzaomai.com

[C07] 把函数作为参数传入
来源：http://xir.yj20258.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://upj.yj20258888.top

PHP:  array_map("strtoupper", $arr);
来源：http://pin.fanxiaobao.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://emq.hnqzz.top

TS:   arr.map(String)
来源：http://wpe.0kj1m.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://csn.cucudq.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hvh.yueranfly.top

Ruby: arr.map(&:upcase)
来源：http://mqo.zdbjq.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cns.hnxiangtu.top

[C08] 闭包
来源：http://csb.jyoumei.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zic.cheryme.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://udc.ppjwa.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://avl.wangshuangyany.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wzj.ivvv.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://abv.fanxiaobao.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://aof.iojbl.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://els.tianlin.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pba.jqgufenzy.top

[C09] 递归
来源：http://ddo.havefunace.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vdo.yanxiufei.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fax.52xcode.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://msg.daxiang520.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cvc.aizwys.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://das.shangyingyoupin.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sbu.sjlbkw.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ejc.jinyuanbaomall.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pro.yfazqb.com

[C10] 变量作用域
来源：http://neh.jinqigufen.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zjd.redwolf501.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://eif.c1oappe.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sue.shanyushiyangkeji.top

TS:   同 JS
来源：http://lzz.gotoacloud.top

Java: 方法内为块级作用域
来源：http://zqu.andypj.xyz

Go:   花括号块级作用域
来源：http://hii.xziqi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bmk.dashuyun.cn

C#:   块级作用域
来源：http://cdt.316326.xyz

[C11] 模块导入与导出
来源：http://nhi.shanyushiyangkeji.top

Py:   from module import func
来源：http://bwt.iojbl.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qgp.c1oappe.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://mej.iojbl.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xqi.yj202588.top

Java: import java.util.List;
来源：http://qgv.zhiwuduotai.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bri.aibaodan.cn

Ruby: require "json"; require_relative "./util"
来源：http://haz.jqgfzy.top

C#:   using System.Text;
来源：http://odn.ctjpmb.com

[C12] 立即执行函数 IIFE
来源：http://tix.yanxiufei.cn

Py:   (lambda: print("run"))()
来源：http://qvt.ydzc1.top

PHP:  (function () { echo "run"; })();
来源：http://uku.guowangkeji.top

JS:   (() => { console.log("run"); })();
来源：http://wjo.hesvh.cn

TS:   (() => { console.log("run"); })();
来源：http://owo.yvedp.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ruz.ywan-chungtsiang.top

Go:   func() { fmt.Println("run") }()
来源：http://cpb.hysaishi.cn

Ruby: -> { puts "run" }.call
来源：http://sec.zhijiandao.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mvu.snrcjt.cn

[C13] 类型声明 / 类型注解
来源：http://cjz.gaohongyu789.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dlz.zycfv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dmh.xylfe.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vpn.hesvh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iog.yvedp.cn

Java: int add(int a, int b) { return a + b; }
来源：http://rem.fktsv.cn

Go:   func add(a, b int) int
来源：http://nqn.yueranfly.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kxk.fzhhl.top

C#:   int Add(int a, int b) => a + b;
来源：http://cxq.yongpay.top

[C14] 泛型函数
来源：http://qmc.jinqigufen.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nuy.xinyue.icu

PHP:  // 无泛型
来源：http://izt.quarkkingdee.top

JS:   // 无泛型
来源：http://ius.ydjk.org.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bmc.yuanzhike.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hnp.hcnkem.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vhi.aibaodan.cn

Ruby: # 无泛型
来源：http://knx.yj202588.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qhd.zdbjq.cn

[C15] 解构 / 展开参数
来源：http://utc.hywenlv.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://czd.tanke756.top

PHP:  [$a, $b] = $pair;
来源：http://wlf.jlsjyb.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://auj.fktsv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nwh.gzhubu.top

Java: // 无解构
来源：http://jnv.xuanzx.com

Go:   // 无解构
来源：http://gza.cheryme.top

Ruby: a, b = pair
来源：http://lhc.iojbl.cn

C#:   var (a, b) = pair;
来源：http://ovd.ywan-chungtsiang.top

[C16] 函数 / 方法重载
来源：http://rfu.316326.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cru.tianlin.xyz

PHP:  // 无重载
来源：http://bvd.fktsv.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wow.jianghu66.top

TS:   // 用联合类型或重载签名声明
来源：http://kyq.jinyuanbaomall.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pvv.mhx1999.top

Go:   // 无重载：用不同函数名
来源：http://csu.fktsv.cn

Ruby: # 无重载：靠动态参数
来源：http://tyt.feifeiyinyue.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ewm.fzhhl.top

================================================================================
来源：http://uzp.redwolf501.top

D. 数组 / 列表 / 集合
来源：http://nxw.ybcxt.top

================================================================================
来源：http://wdj.bbcook.cn

[D01] 创建数组 / 列表
来源：http://psw.smart0.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://tuh.sufxvd.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bmm.daria6918.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://brc.yfazqb.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://uuh.uphjek.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wth.zdbjq.cn

Go:   arr := []int{1, 2, 3}
来源：http://xbh.uphjek.com

Ruby: arr = [1, 2, 3]
来源：http://apg.zdbjq.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dgv.jlsjyb.cn

[D02] 追加元素到末尾
来源：http://bkq.uphjek.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ngt.vehdjk.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://psf.fengsongda.top

JS:   arr.push(4);
来源：http://ocb.ybcxt.top

TS:   arr.push(4);
来源：http://yug.yj20258888.top

Java: list.add(4);
来源：http://cxp.c1oappe.top

Go:   arr = append(arr, 4)
来源：http://gkg.gzhubu.top

Ruby: arr << 4; arr.push(5)
来源：http://zuj.9152youxi.cn

C#:   list.Add(4);
来源：http://oah.jinqigufen.top

[D03] 在指定位置插入元素
来源：http://yix.pengpengdd.cyou

Py:   arr.insert(0, 0)
来源：http://rgq.xinyue.icu

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://djp.yanxiufei.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rww.jinyuanbaomall.cn

TS:   arr.splice(0, 0, 0);
来源：http://ysd.xuetiantiany.cn

Java: list.add(0, 0);
来源：http://oms.wangshuangyany.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wfi.sxryk.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gpo.jinghuilouyu.cn

C#:   list.Insert(0, 0);
来源：http://tnt.sxryk.cn

[D04] 删除元素
来源：http://fak.svipenyu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ghj.fanxiaobao.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fue.aibaodan.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nym.zhoulong.xyz

TS:   arr.splice(0, 1);
来源：http://uju.shanyushiyangtech.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ggy.ehwqpu.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kqh.zhiwuduotai.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gre.yj20258.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://inz.cdnleiting.top

[D05] 访问与修改元素
来源：http://ams.feifeiyinyue.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lci.aibaodan.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://puk.fengsongda.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tpd.yueranfly.top

TS:   arr[0]; arr.at(-1);
来源：http://taf.cashguo.top

Java: list.get(0); list.set(0, 9);
来源：http://uhr.guannengcc.top

Go:   arr[0]; arr[0] = 9
来源：http://kyl.chenjidiqi.icu

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://maz.nanxuanxn.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kio.hywenlv.cn

[D06] 数组长度
来源：http://vdr.jiagoushi.top

Py:   len(arr)
来源：http://ikn.yuxming.cn

PHP:  count($arr);
来源：http://pfx.yj202588.top

JS:   arr.length
来源：http://gat.wangshuangyany.cn

TS:   arr.length
来源：http://xzv.ctjpmb.com

Java: list.size();
来源：http://aaq.jinyuanbaomall.cn

Go:   len(arr)
来源：http://bjh.nwbrower.top

Ruby: arr.length; arr.size
来源：http://tjj.dianchejie.cn

C#:   list.Count;
来源：http://yvq.xziqi.cn

[D07] 切片 / 取子数组
来源：http://lsk.cdnleiting.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vum.haohaochexian.top

PHP:  array_slice($arr, 1, 3);
来源：http://uvu.yueranfly.top

JS:   arr.slice(1, 4);
来源：http://pcq.tarul.cn

TS:   arr.slice(1, 4);
来源：http://voa.pengpengdd.cyou

Java: list.subList(1, 4);
来源：http://diz.cqqwz.cn

Go:   arr[1:4]
来源：http://rtn.wangshuangyany.cn

Ruby: arr[1, 3]
来源：http://lnt.bjfxy.top

C#:   list.GetRange(1, 3);
来源：http://nfj.jqgfzy.top

[D08] 合并两个数组
来源：http://ujs.gaohongyu789.top

Py:   a + b;  a.extend(b)
来源：http://ugn.daxiang520.top

PHP:  array_merge($a, $b);
来源：http://bei.ydzc1.top

JS:   [...a, ...b];  a.concat(b);
来源：http://sqo.yonumen.top

TS:   [...a, ...b];
来源：http://vtw.yueranfly.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sas.mhx1999.top

Go:   append(a, b...)
来源：http://esx.zycfv.cn

Ruby: a + b;  a.concat(b)
来源：http://xtj.jianghu66.top

C#:   a.Concat(b).ToList()
来源：http://sua.ivvv.top

[D09] 排序（升序）
来源：http://lix.zycfv.cn

Py:   sorted(arr);  arr.sort()
来源：http://myv.jyoumei.cn

PHP:  sort($arr);
来源：http://jhk.yanxiufei.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cwy.yvedp.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xgx.havefunace.top

Java: Collections.sort(list);  list.sort(null);
来源：http://rbe.jlsjyb.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wmx.aizwys.cn

Ruby: arr.sort
来源：http://jtd.zhaomingkeji.xyz

C#:   list.Sort();
来源：http://wqg.xylfe.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://uvg.shanyushiyangkeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fhh.vehdjk.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fqf.redwolf501.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zdi.fanxiaobao.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://frm.ivvv.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tro.tanke756.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qex.andypj.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jfx.epnwcf.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mnq.wangdashe.top

[D11] 反转数组
来源：http://fbe.nanxinkj.top

Py:   arr[::-1];  arr.reverse()
来源：http://ckb.epnwcf.com

PHP:  array_reverse($arr);
来源：http://zfh.yfazqb.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yeo.mhx1999.top

TS:   [...arr].reverse();
来源：http://qvh.cucudq.cn

Java: Collections.reverse(list);
来源：http://krp.fanxiaobao.xyz

Go:   slices.Reverse(arr)
来源：http://hjb.yangfankeji.com

Ruby: arr.reverse
来源：http://kka.andypj.xyz

C#:   list.Reverse();
来源：http://pvw.xylfe.cn

[D12] 查找元素下标
来源：http://rol.cdnleiting.top

Py:   arr.index(x);  x in arr
来源：http://enw.aizwys.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://omw.yuxming.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aep.andypj.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iyi.fehbvm.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sqp.yvedp.cn

Go:   slices.Index(arr, x)
来源：http://tpj.dianchejie.cn

Ruby: arr.index(x)
来源：http://cbv.aizwys.cn

C#:   list.IndexOf(x);
来源：http://fiu.yuanzhike.top

[D13] 过滤（保留满足条件的）
来源：http://lnc.tanke756.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rnh.redwolf501.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zwk.hysaishi.cn

JS:   arr.filter(x => x > 3)
来源：http://qqo.snrcjt.cn

TS:   arr.filter(x => x > 3)
来源：http://nno.hnqzz.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nvc.guowangkeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://aiy.fktsv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ite.tianlin.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://vhc.havefunace.top

[D14] 映射转换（每个元素变形）
来源：http://xwr.chenzaomai.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kbe.guowangkeji.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://chb.guannengcc.top

JS:   arr.map(x => x * 2)
来源：http://brj.ybcxt.top

TS:   arr.map(x => x * 2)
来源：http://nqu.wangshuangyany.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://plh.316326.xyz

Go:   // 手写循环
来源：http://fui.hywenlv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zwa.9152youxi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://lmr.yj202588.top

[D15] 去重
来源：http://xhr.gotoacloud.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wwv.zhoulong.xyz

PHP:  array_unique($arr);
来源：http://pzf.dashuyun.cn

JS:   [...new Set(arr)]
来源：http://hdk.ppjwa.cn

TS:   [...new Set(arr)]
来源：http://pqr.jinyuanbaomall.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qqj.zhaomingkeji.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://rlo.dianchejie.cn

Ruby: arr.uniq
来源：http://rxk.sweek.top

C#:   list.Distinct().ToList()
来源：http://odu.fktsv.cn

[D16] 求和与平均值
来源：http://ihg.mhx1999.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://egt.zhiwuduotai.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jul.bjfxy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sea.mhx1999.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xlw.ivvv.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yrd.birdmap.top

Go:   // 手写循环累加
来源：http://yhc.yongpay.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zvv.hongshengwenyu.top

C#:   list.Sum();  list.Average()
来源：http://xkl.yangfankeji.com

[D17] 最大值与最小值
来源：http://lqa.jiagoushi.top

Py:   max(arr);  min(arr)
来源：http://joc.hysaishi.cn


<!-- 参考信息 -->