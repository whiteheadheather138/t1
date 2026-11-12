代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://sbe.shangyingyoupin.top

Go:   func add(a, b int) int { return a + b }
来源：http://ycw.hywenlv.cn

Ruby: def add(a, b); a + b; end
来源：http://oce.zhixingplan.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ljv.jlsjyb.cn

[C02] 默认参数
来源：http://kce.cdnleiting.top

Py:   def greet(name="World"): return name
来源：http://tvg.fzhhl.top

PHP:  function greet($name = "World") { return $name; }
来源：http://src.316326.xyz

JS:   function greet(name = "World") { return name; }
来源：http://dok.fengsongda.top

TS:   function greet(name: string = "World") { return name; }
来源：http://dwa.wangdashe.top

Java: // 无默认参数：方法重载或 Optional
来源：http://bau.dashuyun.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://prf.zhixingplan.top

Ruby: def greet(name = "World") = name
来源：http://mxu.xuetiantiany.cn

C#:   string Greet(string name = "World") => name;
来源：http://zqn.yuanzhike.top

[C03] 可变参数
来源：http://fru.daxiang520.top

Py:   def total(*args): return sum(args)
来源：http://zwu.feifeiyinyue.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wcv.hnxiangtu.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://guw.hnqzz.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ixe.gzhubu.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vty.yj20258888.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jcl.cheryme.top

Ruby: def total(*nums); nums.sum; end
来源：http://jve.snrcjt.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bum.yvedp.cn

[C04] 命名参数 / 关键字参数
来源：http://dhs.shanyushiyangtech.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mai.shanyushiyangkeji.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fhe.xuanzx.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rpd.uphjek.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rnd.tanke756.top

Java: // 无：用 Builder 模式或 record
来源：http://qzu.yfazqb.com

Go:   // 无：用配置结构体参数
来源：http://dtj.hnqzz.top

Ruby: f(a: 1, b: 2)
来源：http://vue.xylfe.cn

C#:   f(a: 1, b: 2)
来源：http://hkg.chenzaomai.com

[C05] 返回多个值
来源：http://fqw.sweek.top

Py:   return a, b
来源：http://txe.jyoumei.cn

PHP:  return [$a, $b];
来源：http://tsi.shuidangran.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://efo.zdbjq.cn

TS:   return { a, b };
来源：http://fzg.jiagoushi.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://scw.chenlongwang.top

Go:   return a, b
来源：http://npj.ehwqpu.com

Ruby: return a, b
来源：http://nih.yvedp.cn

C#:   return (a, b);              // ValueTuple
来源：http://exz.jinqigfzy.top

[C06] 匿名函数 / lambda
来源：http://dzr.haohaochexian.top

Py:   square = lambda x: x * x
来源：http://lpv.dianchejie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hfo.sysykeji.top

JS:   const square = x => x * x;
来源：http://bqf.jyoumei.cn

TS:   const square = (x: number): number => x * x;
来源：http://osu.yuxming.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fqt.zdqjudy.top

Go:   sq := func(x int) int { return x * x }
来源：http://foz.cucudq.cn

Ruby: square = ->(x) { x * x }
来源：http://hlc.yonumen.top

C#:   Func<int, int> square = x => x * x;
来源：http://uvr.zdqjudy.top

[C07] 把函数作为参数传入
来源：http://xag.hammf.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xom.tarul.cn

PHP:  array_map("strtoupper", $arr);
来源：http://rhk.yuxming.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jlb.yangfankeji.com

TS:   arr.map(String)
来源：http://vqc.hysaishi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ler.hesvh.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wlr.shuidangran.top

Ruby: arr.map(&:upcase)
来源：http://fwv.xylfe.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ymc.daxiang520.top

[C08] 闭包
来源：http://ylq.zdqjudy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fym.ydjk.org.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cas.gzhubu.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qfc.birdmap.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wsl.zhijiandao.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nyg.wangshuangyany.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tub.jlsjyb.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wfy.sysykeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://leh.52xcode.cn

[C09] 递归
来源：http://hew.birdmap.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hic.haohaochexian.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ndb.jlsjyb.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://msl.shanyushiyangtech.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ukl.zhixingplan.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xxt.yuxming.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ohz.shanyushiyangtech.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://txc.tarul.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rct.nwbrower.top

[C10] 变量作用域
来源：http://aiw.xuetiantiany.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wrt.zycfv.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qcq.shangyingyoupin.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dbv.yonumen.top

TS:   同 JS
来源：http://fdf.feifeiyinyue.top

Java: 方法内为块级作用域
来源：http://rod.52xcode.cn

Go:   花括号块级作用域
来源：http://qre.zhixingplan.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ttg.sysykeji.top

C#:   块级作用域
来源：http://hir.yangfankeji.com

[C11] 模块导入与导出
来源：http://vwl.quarkkingdee.top

Py:   from module import func
来源：http://bes.zdbjq.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mlz.chenjidiqi.icu

JS:   export default function f() {};  import f from "./m.js";
来源：http://adb.pengpengdd.cyou

TS:   export function f(): void {};  import { f } from "./m";
来源：http://avh.jinghuilouyu.cn

Java: import java.util.List;
来源：http://ukj.cheryme.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://enq.yvedp.cn

Ruby: require "json"; require_relative "./util"
来源：http://nwb.shuidangran.top

C#:   using System.Text;
来源：http://ilo.sysykeji.top

[C12] 立即执行函数 IIFE
来源：http://lku.iojbl.cn

Py:   (lambda: print("run"))()
来源：http://wyj.bbcook.cn

PHP:  (function () { echo "run"; })();
来源：http://ynb.yangfankeji.com

JS:   (() => { console.log("run"); })();
来源：http://lgk.redwolf501.top

TS:   (() => { console.log("run"); })();
来源：http://mcl.uphjek.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://anl.daria6918.cn

Go:   func() { fmt.Println("run") }()
来源：http://nli.chenjidiqi.icu

Ruby: -> { puts "run" }.call
来源：http://ztv.ehwqpu.com

C#:   // 无 IIFE：用静态构造函数
来源：http://mtp.sufxvd.cn

[C13] 类型声明 / 类型注解
来源：http://lpn.fanxiaobao.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rjc.yj20258.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ngx.c1oappe.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ebf.ppjwa.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://txj.tarul.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xiq.hnqzz.top

Go:   func add(a, b int) int
来源：http://art.xingfuxueyuan.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yzq.zhiwuduotai.top

C#:   int Add(int a, int b) => a + b;
来源：http://rez.yfazqb.com

[C14] 泛型函数
来源：http://pqr.yuanzhike.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gyr.daxiang520.top

PHP:  // 无泛型
来源：http://erq.shanyushiyangtech.top

JS:   // 无泛型
来源：http://pyp.shangyingyoupin.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jlq.ywan-chungtsiang.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ycq.jinghuilouyu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://asv.quarkkingdee.top

Ruby: # 无泛型
来源：http://rlg.ctjpmb.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ayv.shzxlz.cn

[C15] 解构 / 展开参数
来源：http://dnz.aizwys.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dei.zhijiandao.cn

PHP:  [$a, $b] = $pair;
来源：http://cmy.yuxming.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dlk.yonumen.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dwt.quarkkingdee.top

Java: // 无解构
来源：http://chr.yongpay.top

Go:   // 无解构
来源：http://srf.feifeiyinyue.top

Ruby: a, b = pair
来源：http://cpq.andypj.xyz

C#:   var (a, b) = pair;
来源：http://jsp.kuanghao11.cn

[C16] 函数 / 方法重载
来源：http://uvg.smart0.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ptj.ctjpmb.com

PHP:  // 无重载
来源：http://qnx.ydzc1.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://cyo.daxiang520.top

TS:   // 用联合类型或重载签名声明
来源：http://khv.jinqigfzy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://wza.yuanzhike.top

Go:   // 无重载：用不同函数名
来源：http://csw.shzxlz.cn

Ruby: # 无重载：靠动态参数
来源：http://put.yueranfly.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ezx.gzhubu.top

================================================================================
来源：http://xlt.zhoulong.xyz

D. 数组 / 列表 / 集合
来源：http://zlm.hfpthk.cn

================================================================================
来源：http://omb.ywan-chungtsiang.top

[D01] 创建数组 / 列表
来源：http://maf.zycfv.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xgb.daxiang520.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gzn.jiagoushi.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xof.yanxiufei.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://msp.fehbvm.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ggr.yueranfly.top

Go:   arr := []int{1, 2, 3}
来源：http://tdx.sufxvd.cn

Ruby: arr = [1, 2, 3]
来源：http://yta.iojbl.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://scj.jlsjyb.cn

[D02] 追加元素到末尾
来源：http://yge.c1oappe.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yml.guowangkeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tty.hammf.cn

JS:   arr.push(4);
来源：http://suq.iojbl.cn

TS:   arr.push(4);
来源：http://pkc.yongpay.top

Java: list.add(4);
来源：http://cmb.nanxuanxn.top

Go:   arr = append(arr, 4)
来源：http://lzb.iojbl.cn

Ruby: arr << 4; arr.push(5)
来源：http://kzx.nanxinkj.top

C#:   list.Add(4);
来源：http://nqs.zycfv.cn

[D03] 在指定位置插入元素
来源：http://otw.zdbjq.cn

Py:   arr.insert(0, 0)
来源：http://zwt.havefunace.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bua.xylfe.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://imp.xingfuxueyuan.xyz

TS:   arr.splice(0, 0, 0);
来源：http://dlz.gzhubu.top

Java: list.add(0, 0);
来源：http://dkk.ppjwa.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pvk.ivvv.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zbg.yj20258888.top

C#:   list.Insert(0, 0);
来源：http://scj.jianghu66.top

[D04] 删除元素
来源：http://gni.yuanzhike.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://slr.fzhhl.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xpg.sxryk.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ckt.chenjidiqi.icu

TS:   arr.splice(0, 1);
来源：http://ufw.ppjwa.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fjk.fehbvm.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dwi.xylfe.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://npm.epnwcf.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dzh.haohaochexian.top

[D05] 访问与修改元素
来源：http://oov.jinyuanbaomall.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zzo.xingfuxueyuan.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://diz.dianchejie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vwe.cucudq.cn

TS:   arr[0]; arr.at(-1);
来源：http://ljn.shanyushiyangkeji.top

Java: list.get(0); list.set(0, 9);
来源：http://igc.cdnleiting.top

Go:   arr[0]; arr[0] = 9
来源：http://txu.hesvh.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uhg.gotoacloud.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://abc.sufxvd.cn

[D06] 数组长度
来源：http://fgd.nanxinkj.top

Py:   len(arr)
来源：http://jfo.zycfv.cn

PHP:  count($arr);
来源：http://gct.9152youxi.cn

JS:   arr.length
来源：http://sgu.yuxming.cn

TS:   arr.length
来源：http://wtz.snrcjt.cn

Java: list.size();
来源：http://rap.jiagoushi.top

Go:   len(arr)
来源：http://wsu.tianlin.xyz

Ruby: arr.length; arr.size
来源：http://eiq.vqdsnc.cn

C#:   list.Count;
来源：http://alk.zhixingplan.top

[D07] 切片 / 取子数组
来源：http://tlz.shanyushiyangkeji.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ucn.wangdashe.top

PHP:  array_slice($arr, 1, 3);
来源：http://zgu.yj202588.top

JS:   arr.slice(1, 4);
来源：http://fqs.jinyuanbaomall.cn

TS:   arr.slice(1, 4);
来源：http://hjx.yanxiufei.cn

Java: list.subList(1, 4);
来源：http://vvj.cucudq.cn

Go:   arr[1:4]
来源：http://xje.wangshuangyany.cn

Ruby: arr[1, 3]
来源：http://ktc.yangfankeji.com

C#:   list.GetRange(1, 3);
来源：http://oqs.bbcook.cn

[D08] 合并两个数组
来源：http://bmb.dashuyun.cn

Py:   a + b;  a.extend(b)
来源：http://jmf.9152youxi.cn

PHP:  array_merge($a, $b);
来源：http://heh.jiagoushi.top

JS:   [...a, ...b];  a.concat(b);
来源：http://sey.yuxming.cn

TS:   [...a, ...b];
来源：http://opx.c1oappe.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dee.jinghuilouyu.cn

Go:   append(a, b...)
来源：http://xdy.9152youxi.cn

Ruby: a + b;  a.concat(b)
来源：http://hlo.sxryk.cn

C#:   a.Concat(b).ToList()
来源：http://ank.zhijiandao.cn

[D09] 排序（升序）
来源：http://fzg.sjlbkw.cn

Py:   sorted(arr);  arr.sort()
来源：http://ymr.zhongyouzk.top

PHP:  sort($arr);
来源：http://vov.snrcjt.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qez.zhengqikj.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://tth.yangfankeji.com

Java: Collections.sort(list);  list.sort(null);
来源：http://dod.fanxiaobao.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cjd.cdnleiting.top

Ruby: arr.sort
来源：http://ebu.chenlongwang.top

C#:   list.Sort();
来源：http://vnm.nanxinkj.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://kcs.aibaodan.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sbl.zhaomingkeji.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://alt.yueranfly.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://otm.jqgufenzy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tie.epnwcf.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hdc.zhiwuduotai.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://phh.smart0.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tsj.zhongyouzk.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rlc.jinyuanbaomall.cn

[D11] 反转数组
来源：http://kwd.redwolf501.top

Py:   arr[::-1];  arr.reverse()
来源：http://jvo.wangshuangyany.cn

PHP:  array_reverse($arr);
来源：http://yig.pycfn.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xfr.feifeiyinyue.top

TS:   [...arr].reverse();
来源：http://rkb.yuanzhike.top

Java: Collections.reverse(list);
来源：http://bgu.guowangkeji.top

Go:   slices.Reverse(arr)
来源：http://vzp.ppjwa.cn

Ruby: arr.reverse
来源：http://wwy.aizwys.cn

C#:   list.Reverse();
来源：http://pwc.guannengcc.top

[D12] 查找元素下标
来源：http://rgj.hywenlv.cn

Py:   arr.index(x);  x in arr
来源：http://mvg.bjfxy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rbc.hesvh.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gtf.ppjwa.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ojm.havefunace.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://whi.zhiwuduotai.top

Go:   slices.Index(arr, x)
来源：http://upm.fzhhl.top

Ruby: arr.index(x)
来源：http://ctr.52xcode.cn

C#:   list.IndexOf(x);
来源：http://xlh.meibo888.top

[D13] 过滤（保留满足条件的）
来源：http://oni.sjlbkw.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lmo.ehwqpu.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://eex.svipenyu.cn

JS:   arr.filter(x => x > 3)
来源：http://nvv.daria6918.cn

TS:   arr.filter(x => x > 3)
来源：http://fay.epnwcf.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cfs.xinyue.icu

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mgv.shzxlz.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ocs.ctjpmb.com

C#:   list.Where(x => x > 3).ToList()
来源：http://pfo.yanxiufei.cn

[D14] 映射转换（每个元素变形）
来源：http://wzk.cqqwz.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hnm.sysykeji.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://czi.iojbl.cn

JS:   arr.map(x => x * 2)
来源：http://obr.havefunace.top

TS:   arr.map(x => x * 2)
来源：http://hic.svipenyu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://stt.fehbvm.com

Go:   // 手写循环
来源：http://mem.chenjidiqi.icu

Ruby: arr.map { |x| x * 2 }
来源：http://zzt.yangfankeji.com

C#:   list.Select(x => x * 2).ToList()
来源：http://ywx.9152youxi.cn

[D15] 去重
来源：http://bzb.daria6918.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cne.nwbrower.top

PHP:  array_unique($arr);
来源：http://sdc.hywenlv.cn

JS:   [...new Set(arr)]
来源：http://qxl.fengsongda.top

TS:   [...new Set(arr)]
来源：http://jba.epnwcf.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fvu.zhiwuduotai.top

Go:   // 用 map[T]struct{} 手写
来源：http://vin.hcnkem.com

Ruby: arr.uniq
来源：http://pwa.svipenyu.cn

C#:   list.Distinct().ToList()
来源：http://hwg.kuanghao11.cn

[D16] 求和与平均值
来源：http://brt.jianghu66.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pth.ydzc1.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://eet.cucudq.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hjz.yfazqb.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ntw.hcnkem.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ndv.havefunace.top

Go:   // 手写循环累加
来源：http://saa.shanyushiyangtech.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://laq.ctjpmb.com

C#:   list.Sum();  list.Average()
来源：http://lkt.hywenlv.cn

[D17] 最大值与最小值
来源：http://ufq.yuxming.cn

Py:   max(arr);  min(arr)
来源：http://wbo.yuanzhike.top

PHP:  max($arr);  min($arr);
来源：http://suf.xuanzx.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://eyb.nanxuanxn.top

TS:   Math.max(...arr);
来源：http://ink.zhijiandao.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://nes.zhoulong.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nxr.tarul.cn

Ruby: arr.max;  arr.min
来源：http://tci.jinqigufen.top

C#:   list.Max();  list.Min()
来源：http://qvh.cashguo.top

[D18] 扁平化嵌套数组
来源：http://yge.meibo888.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://grm.sysykeji.top

PHP:  array_merge(...$nested);
来源：http://nkq.52xcode.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pxd.chenzaomai.com

TS:   nested.flat();
来源：http://rhp.jinghuilouyu.cn


<!-- 参考信息 -->