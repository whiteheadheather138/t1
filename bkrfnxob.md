代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://iuz.yongpay.top

Java: // 无默认参数：方法重载或 Optional
来源：http://gtc.316326.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vcf.dianchejie.cn

Ruby: def greet(name = "World") = name
来源：http://fde.jqgfzy.top

C#:   string Greet(string name = "World") => name;
来源：http://awj.chenzaomai.com

[C03] 可变参数
来源：http://hwq.sufxvd.cn

Py:   def total(*args): return sum(args)
来源：http://dav.tian-w.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vwz.yueranfly.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dpo.havefunace.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kmg.jqgufenzy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mhs.tanke756.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://isz.hammf.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xwp.tanke756.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kha.iojbl.cn

[C04] 命名参数 / 关键字参数
来源：http://amn.shanyushiyangtech.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zly.xylfe.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://llb.jyoumei.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://frs.fengsongda.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gme.redwolf501.top

Java: // 无：用 Builder 模式或 record
来源：http://stn.fehbvm.com

Go:   // 无：用配置结构体参数
来源：http://rra.jqgufenzy.top

Ruby: f(a: 1, b: 2)
来源：http://mek.tarul.cn

C#:   f(a: 1, b: 2)
来源：http://bsd.mhx1999.top

[C05] 返回多个值
来源：http://eey.uphjek.com

Py:   return a, b
来源：http://woi.chenjidiqi.icu

PHP:  return [$a, $b];
来源：http://jkl.wangshuangyany.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jgf.nanxinkj.top

TS:   return { a, b };
来源：http://xtw.smart0.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hll.nwbrower.top

Go:   return a, b
来源：http://cwa.hnxiangtu.top

Ruby: return a, b
来源：http://neh.yangfankeji.com

C#:   return (a, b);              // ValueTuple
来源：http://byc.smart0.xyz

[C06] 匿名函数 / lambda
来源：http://sis.hysaishi.cn

Py:   square = lambda x: x * x
来源：http://mjt.jinyuanbaomall.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hoo.hnqzz.top

JS:   const square = x => x * x;
来源：http://jzx.shanyushiyangkeji.top

TS:   const square = (x: number): number => x * x;
来源：http://zhi.haohaochexian.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://szz.chenzaomai.com

Go:   sq := func(x int) int { return x * x }
来源：http://eyt.ehwqpu.com

Ruby: square = ->(x) { x * x }
来源：http://ebi.xziqi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://czv.svipenyu.cn

[C07] 把函数作为参数传入
来源：http://tfz.gzhubu.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ylb.yj20258888.top

PHP:  array_map("strtoupper", $arr);
来源：http://yhx.wangshuangyany.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gze.yj20258.top

TS:   arr.map(String)
来源：http://zqn.zdqjudy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tke.52xcode.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://opb.ywan-chungtsiang.top

Ruby: arr.map(&:upcase)
来源：http://wnl.yangfankeji.com

C#:   arr.Select(s => s.ToUpper())
来源：http://syi.nwbrower.top

[C08] 闭包
来源：http://bvr.yongpay.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gqw.yj20258888.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ico.dianchejie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zha.shuidangran.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://diy.fengsongda.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vrq.nwbrower.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ojb.yj202588.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://oiw.yvedp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://oqw.tanke756.top

[C09] 递归
来源：http://xpe.vqdsnc.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wxo.daria6918.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cym.jlsjyb.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lxy.dashuyun.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tqq.jiagoushi.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jxh.jlsjyb.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ecm.yueranfly.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ouf.jlsjyb.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dqn.xuetiantiany.cn

[C10] 变量作用域
来源：http://zcy.hnxiangtu.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fcj.zhiwuduotai.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://trc.ywan-chungtsiang.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jsl.sysykeji.top

TS:   同 JS
来源：http://xrp.pengpengdd.cyou

Java: 方法内为块级作用域
来源：http://jhb.hnxiangtu.top

Go:   花括号块级作用域
来源：http://iho.haohaochexian.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://olx.yj202588.top

C#:   块级作用域
来源：http://gul.bjfxy.top

[C11] 模块导入与导出
来源：http://lsa.vehdjk.com

Py:   from module import func
来源：http://uvx.smart0.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://zsj.hfpthk.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://phr.jinqigufen.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qvu.smart0.xyz

Java: import java.util.List;
来源：http://yes.yonumen.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rvr.uphjek.com

Ruby: require "json"; require_relative "./util"
来源：http://veb.bjfxy.top

C#:   using System.Text;
来源：http://vhe.shanyushiyangtech.top

[C12] 立即执行函数 IIFE
来源：http://lqu.hnxiangtu.top

Py:   (lambda: print("run"))()
来源：http://tta.tarul.cn

PHP:  (function () { echo "run"; })();
来源：http://kws.zhoulong.xyz

JS:   (() => { console.log("run"); })();
来源：http://ibb.sxryk.cn

TS:   (() => { console.log("run"); })();
来源：http://elk.zhixingplan.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zun.nanxinkj.top

Go:   func() { fmt.Println("run") }()
来源：http://ilb.jlsjyb.cn

Ruby: -> { puts "run" }.call
来源：http://fuw.yj20258888.top

C#:   // 无 IIFE：用静态构造函数
来源：http://hrh.yvedp.cn

[C13] 类型声明 / 类型注解
来源：http://qan.pycfn.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tkc.ywan-chungtsiang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hbz.9152youxi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://acd.pycfn.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qiz.pycfn.com

Java: int add(int a, int b) { return a + b; }
来源：http://mnw.zhaomingkeji.xyz

Go:   func add(a, b int) int
来源：http://zag.yj20258.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://srw.feifeiyinyue.top

C#:   int Add(int a, int b) => a + b;
来源：http://eor.ctjpmb.com

[C14] 泛型函数
来源：http://vjy.uphjek.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lmx.snrcjt.cn

PHP:  // 无泛型
来源：http://byr.fktsv.cn

JS:   // 无泛型
来源：http://jkc.ybcxt.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ihb.mhx1999.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bav.sweek.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://moj.zhiwuduotai.top

Ruby: # 无泛型
来源：http://jbl.316326.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nie.fehbvm.com

[C15] 解构 / 展开参数
来源：http://pid.jinqigufen.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fyu.shanyushiyangkeji.top

PHP:  [$a, $b] = $pair;
来源：http://grj.jinghuilouyu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://epv.fengsongda.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wax.smart0.xyz

Java: // 无解构
来源：http://atu.ybcxt.top

Go:   // 无解构
来源：http://fcu.cheryme.top

Ruby: a, b = pair
来源：http://sql.zhijiandao.cn

C#:   var (a, b) = pair;
来源：http://rvw.yangfankeji.com

[C16] 函数 / 方法重载
来源：http://qxv.yangfankeji.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://eln.yj20258888.top

PHP:  // 无重载
来源：http://dmw.yonumen.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://hqz.shzxlz.cn

TS:   // 用联合类型或重载签名声明
来源：http://ftz.hcnkem.com

Java: void f(int a) {}  void f(String a) {}
来源：http://lju.xziqi.cn

Go:   // 无重载：用不同函数名
来源：http://iuf.jyoumei.cn

Ruby: # 无重载：靠动态参数
来源：http://zsh.ppjwa.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://dsb.fanxiaobao.xyz

================================================================================
来源：http://zng.mhx1999.top

D. 数组 / 列表 / 集合
来源：http://mct.0kj1m.cn

================================================================================
来源：http://tcv.redwolf501.top

[D01] 创建数组 / 列表
来源：http://chk.uphjek.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://gzi.wangdashe.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hrz.yonumen.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://odv.dashuyun.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dax.yonumen.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gpj.nwbrower.top

Go:   arr := []int{1, 2, 3}
来源：http://bzy.jiagoushi.top

Ruby: arr = [1, 2, 3]
来源：http://tcv.zhijiandao.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fnm.xuetiantiany.cn

[D02] 追加元素到末尾
来源：http://krb.fktsv.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fec.yvedp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ivf.haohaochexian.top

JS:   arr.push(4);
来源：http://pip.ehwqpu.com

TS:   arr.push(4);
来源：http://iyf.gaohongyu789.top

Java: list.add(4);
来源：http://rcu.sysykeji.top

Go:   arr = append(arr, 4)
来源：http://lvr.yfazqb.com

Ruby: arr << 4; arr.push(5)
来源：http://wmy.zdqjudy.top

C#:   list.Add(4);
来源：http://ewk.kuanghao11.cn

[D03] 在指定位置插入元素
来源：http://pdg.zhixingplan.top

Py:   arr.insert(0, 0)
来源：http://ley.jyoumei.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qor.fktsv.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ddp.zycfv.cn

TS:   arr.splice(0, 0, 0);
来源：http://bfk.yuxming.cn

Java: list.add(0, 0);
来源：http://crn.cashguo.top

Go:   arr = append([]int{0}, arr...)
来源：http://deg.mhx1999.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ilf.jqgufenzy.top

C#:   list.Insert(0, 0);
来源：http://kff.daxiang520.top

[D04] 删除元素
来源：http://xjg.sweek.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vzf.havefunace.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jjx.jinyuanbaomall.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yat.hysaishi.cn

TS:   arr.splice(0, 1);
来源：http://ejv.andypj.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zql.jqgfzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ewi.haohaochexian.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bei.havefunace.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://coe.wangshuangyany.cn

[D05] 访问与修改元素
来源：http://elx.snrcjt.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wiv.jqgufenzy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gqp.smart0.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kuc.haohaochexian.top

TS:   arr[0]; arr.at(-1);
来源：http://zwh.cashguo.top

Java: list.get(0); list.set(0, 9);
来源：http://lav.sjlbkw.cn

Go:   arr[0]; arr[0] = 9
来源：http://nfb.zycfv.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://emv.9152youxi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ada.ivvv.top

[D06] 数组长度
来源：http://wod.zhijiandao.cn

Py:   len(arr)
来源：http://gfa.hnxiangtu.top

PHP:  count($arr);
来源：http://txa.jlsjyb.cn

JS:   arr.length
来源：http://pvp.nwbrower.top

TS:   arr.length
来源：http://xdo.ivvv.top

Java: list.size();
来源：http://thx.yvedp.cn

Go:   len(arr)
来源：http://lzn.wangshuangyany.cn

Ruby: arr.length; arr.size
来源：http://qjx.iojbl.cn

C#:   list.Count;
来源：http://olk.cheryme.top

[D07] 切片 / 取子数组
来源：http://bah.daxiang520.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gbr.yuanzhike.top

PHP:  array_slice($arr, 1, 3);
来源：http://cij.ehwqpu.com

JS:   arr.slice(1, 4);
来源：http://rjf.ehwqpu.com

TS:   arr.slice(1, 4);
来源：http://baf.cheryme.top

Java: list.subList(1, 4);
来源：http://sbj.gzhubu.top

Go:   arr[1:4]
来源：http://fzx.chenzaomai.com

Ruby: arr[1, 3]
来源：http://tdq.nwbrower.top

C#:   list.GetRange(1, 3);
来源：http://wvh.gotoacloud.top

[D08] 合并两个数组
来源：http://vav.gogol.net.cn

Py:   a + b;  a.extend(b)
来源：http://frk.fzhhl.top

PHP:  array_merge($a, $b);
来源：http://xpy.fehbvm.com

JS:   [...a, ...b];  a.concat(b);
来源：http://zst.meibo888.top

TS:   [...a, ...b];
来源：http://vhi.jianghu66.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lut.jinghuilouyu.cn

Go:   append(a, b...)
来源：http://kzj.zhiwuduotai.top

Ruby: a + b;  a.concat(b)
来源：http://egn.shanyushiyangkeji.top

C#:   a.Concat(b).ToList()
来源：http://evz.zhongyouzk.top

[D09] 排序（升序）
来源：http://zun.yuanzhike.top

Py:   sorted(arr);  arr.sort()
来源：http://kxp.jqgfzy.top

PHP:  sort($arr);
来源：http://rif.jinghuilouyu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dtq.yanxiufei.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://rsj.snrcjt.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://bym.ppjwa.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xoy.fehbvm.com

Ruby: arr.sort
来源：http://zqp.shangyingyoupin.top

C#:   list.Sort();
来源：http://aqv.pycfn.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://iga.birdmap.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vqv.uphjek.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://the.quarkkingdee.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bqp.hcnkem.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dhw.xziqi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lnt.zdqjudy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tld.xziqi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ikk.zhaomingkeji.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wrw.chenlongwang.top

[D11] 反转数组
来源：http://bdd.sysykeji.top

Py:   arr[::-1];  arr.reverse()
来源：http://mzk.jiagoushi.top

PHP:  array_reverse($arr);
来源：http://poj.yj20258.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://evk.pycfn.com

TS:   [...arr].reverse();
来源：http://vqr.vqdsnc.cn

Java: Collections.reverse(list);
来源：http://sla.quarkkingdee.top

Go:   slices.Reverse(arr)
来源：http://kvm.xinyue.icu

Ruby: arr.reverse
来源：http://lgp.ivvv.top

C#:   list.Reverse();
来源：http://wup.fehbvm.com

[D12] 查找元素下标
来源：http://bdd.haohaochexian.top

Py:   arr.index(x);  x in arr
来源：http://kgu.havefunace.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pac.dianchejie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vda.bbcook.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tnb.hnqzz.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kpu.haohaochexian.top

Go:   slices.Index(arr, x)
来源：http://bey.sjlbkw.cn

Ruby: arr.index(x)
来源：http://twl.nwbrower.top

C#:   list.IndexOf(x);
来源：http://cpf.xuetiantiany.cn

[D13] 过滤（保留满足条件的）
来源：http://wpl.dashuyun.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://abm.xylfe.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kxu.fengsongda.top

JS:   arr.filter(x => x > 3)
来源：http://waf.jinyuanbaomall.cn

TS:   arr.filter(x => x > 3)
来源：http://jbm.feifeiyinyue.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ozj.pycfn.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tgh.fzhhl.top

Ruby: arr.select { |x| x > 3 }
来源：http://pex.zhixingplan.top

C#:   list.Where(x => x > 3).ToList()
来源：http://eep.zhixingplan.top

[D14] 映射转换（每个元素变形）
来源：http://lzq.zycfv.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://oti.ywan-chungtsiang.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zlv.yonumen.top

JS:   arr.map(x => x * 2)
来源：http://fyv.gotoacloud.top

TS:   arr.map(x => x * 2)
来源：http://kvf.redwolf501.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://sim.zhijiandao.cn

Go:   // 手写循环
来源：http://eqz.jinqigufen.top

Ruby: arr.map { |x| x * 2 }
来源：http://htl.fzhhl.top

C#:   list.Select(x => x * 2).ToList()
来源：http://pzc.hnqzz.top

[D15] 去重
来源：http://utl.chenlongwang.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://isd.daxiang520.top

PHP:  array_unique($arr);
来源：http://jlt.cqqwz.cn

JS:   [...new Set(arr)]
来源：http://ubo.xylfe.cn

TS:   [...new Set(arr)]
来源：http://bwj.zhiwuduotai.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sxj.chenlongwang.top

Go:   // 用 map[T]struct{} 手写
来源：http://avx.shanyushiyangkeji.top

Ruby: arr.uniq
来源：http://yfh.vqdsnc.cn

C#:   list.Distinct().ToList()
来源：http://cmx.jqgufenzy.top

[D16] 求和与平均值
来源：http://fen.sjlbkw.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sxs.sysykeji.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ojt.zhengqikj.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fct.birdmap.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ran.sweek.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ifw.hesvh.cn

Go:   // 手写循环累加
来源：http://siq.fengsongda.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tcd.ehwqpu.com

C#:   list.Sum();  list.Average()
来源：http://rdi.52xcode.cn

[D17] 最大值与最小值
来源：http://drp.dashuyun.cn

Py:   max(arr);  min(arr)
来源：http://ete.52xcode.cn

PHP:  max($arr);  min($arr);
来源：http://mro.zhiwuduotai.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://etv.yueranfly.top

TS:   Math.max(...arr);
来源：http://hof.sxryk.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://lxm.uphjek.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vid.yonumen.top

Ruby: arr.max;  arr.min
来源：http://osd.cheryme.top

C#:   list.Max();  list.Min()
来源：http://axp.xziqi.cn

[D18] 扁平化嵌套数组
来源：http://ebz.ehwqpu.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jam.yfazqb.com

PHP:  array_merge(...$nested);
来源：http://qeb.xingfuxueyuan.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kle.havefunace.top

TS:   nested.flat();
来源：http://rvw.zhoulong.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zmt.hysaishi.cn

Go:   // 手写双层循环
来源：http://iyn.guannengcc.top

Ruby: nested.flatten
来源：http://gcz.hnxiangtu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://pgu.jinqigufen.top

[D19] 按字段分组
来源：http://uke.cqqwz.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bnj.sjlbkw.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dyy.vqdsnc.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rgv.gaohongyu789.top


<!-- 参考信息 -->