代发 wailian999

Go:   a && b || !c
来源：http://nmh.snrcjt.cn

Ruby: a && b || !c
来源：http://vai.chenlongwang.top

C#:   a && b || !c
来源：http://czg.pycfn.com

[B16] 卫语句：不满足条件提前返回
来源：http://bat.zhengqikj.top

Py:   if not data: return
来源：http://qwa.jinqigufen.top

PHP:  if (!$data) { return; }
来源：http://vtq.cucudq.cn

JS:   if (!data) return;
来源：http://bky.ehwqpu.com

TS:   if (!data) return;
来源：http://ljf.dashuyun.cn

Java: if (data == null) return;
来源：http://pml.nwbrower.top

Go:   if data == nil { return }
来源：http://dhy.epnwcf.com

Ruby: return if data.nil?
来源：http://ssj.shuidangran.top

C#:   if (data == null) return;
来源：http://vnq.ctjpmb.com

================================================================================
来源：http://fti.havefunace.top

C. 函数与作用域
来源：http://tld.xylfe.cn

================================================================================
来源：http://lqz.jiagoushi.top

[C01] 定义函数
来源：http://quy.smart0.xyz

Py:   def add(a, b): return a + b
来源：http://poy.shzxlz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://egg.ybcxt.top

JS:   function add(a, b) { return a + b; }
来源：http://wtu.gotoacloud.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xlj.yj20258888.top

Java: static int add(int a, int b) { return a + b; }
来源：http://gsw.yuxming.cn

Go:   func add(a, b int) int { return a + b }
来源：http://evo.zdbjq.cn

Ruby: def add(a, b); a + b; end
来源：http://ktm.zhongyouzk.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ytp.dianchejie.cn

[C02] 默认参数
来源：http://iij.vehdjk.com

Py:   def greet(name="World"): return name
来源：http://ybp.xuanzx.com

PHP:  function greet($name = "World") { return $name; }
来源：http://vqs.fengsongda.top

JS:   function greet(name = "World") { return name; }
来源：http://haf.kuanghao11.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://nbm.haohaochexian.top

Java: // 无默认参数：方法重载或 Optional
来源：http://vcy.cashguo.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wuy.gotoacloud.top

Ruby: def greet(name = "World") = name
来源：http://iji.smart0.xyz

C#:   string Greet(string name = "World") => name;
来源：http://amp.cqqwz.cn

[C03] 可变参数
来源：http://edk.hnqzz.top

Py:   def total(*args): return sum(args)
来源：http://gch.bjfxy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wlm.9152youxi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://svq.hesvh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jcu.yvedp.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nxd.zhijiandao.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dtq.pengpengdd.cyou

Ruby: def total(*nums); nums.sum; end
来源：http://zmt.vqdsnc.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lzt.zdbjq.cn

[C04] 命名参数 / 关键字参数
来源：http://voh.xinyue.icu

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dvs.nanxinkj.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://alw.shzxlz.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rba.quarkkingdee.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xdc.xingfuxueyuan.xyz

Java: // 无：用 Builder 模式或 record
来源：http://qqv.tarul.cn

Go:   // 无：用配置结构体参数
来源：http://sqt.316326.xyz

Ruby: f(a: 1, b: 2)
来源：http://eye.jinqigfzy.top

C#:   f(a: 1, b: 2)
来源：http://ths.yueranfly.top

[C05] 返回多个值
来源：http://fth.yangfankeji.com

Py:   return a, b
来源：http://heu.chenjidiqi.icu

PHP:  return [$a, $b];
来源：http://lyv.zycfv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vzj.fanxiaobao.xyz

TS:   return { a, b };
来源：http://ldi.316326.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cic.sufxvd.cn

Go:   return a, b
来源：http://vpk.gaohongyu789.top

Ruby: return a, b
来源：http://twd.kuanghao11.cn

C#:   return (a, b);              // ValueTuple
来源：http://jgv.gogol.net.cn

[C06] 匿名函数 / lambda
来源：http://dfy.zhongyouzk.top

Py:   square = lambda x: x * x
来源：http://uif.hysaishi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://dnu.zhaomingkeji.xyz

JS:   const square = x => x * x;
来源：http://qwq.jinghuilouyu.cn

TS:   const square = (x: number): number => x * x;
来源：http://ood.fktsv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vhj.gzhubu.top

Go:   sq := func(x int) int { return x * x }
来源：http://ewi.hysaishi.cn

Ruby: square = ->(x) { x * x }
来源：http://gxp.yj202588.top

C#:   Func<int, int> square = x => x * x;
来源：http://ojs.nanxuanxn.top

[C07] 把函数作为参数传入
来源：http://tpo.ywan-chungtsiang.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tog.xinyue.icu

PHP:  array_map("strtoupper", $arr);
来源：http://jke.birdmap.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wyr.feifeiyinyue.top

TS:   arr.map(String)
来源：http://zah.yvedp.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://att.chenlongwang.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kht.ydjk.org.cn

Ruby: arr.map(&:upcase)
来源：http://qlx.shuidangran.top

C#:   arr.Select(s => s.ToUpper())
来源：http://rwg.zdqjudy.top

[C08] 闭包
来源：http://dyl.wangshuangyany.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dnq.sxryk.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ekd.daxiang520.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ifs.iojbl.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zhi.ybcxt.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zsc.kuanghao11.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dwv.cqqwz.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pkg.meibo888.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qhc.feifeiyinyue.top

[C09] 递归
来源：http://eup.sysykeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nyp.shuidangran.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://iue.gogol.net.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://doz.zhaomingkeji.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mpa.yueranfly.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://loj.pengpengdd.cyou

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hol.tarul.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cbx.tanke756.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rcm.yanxiufei.cn

[C10] 变量作用域
来源：http://ppi.gogol.net.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vrx.yongpay.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ifg.ydzc1.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yja.bjfxy.top

TS:   同 JS
来源：http://eod.jqgufenzy.top

Java: 方法内为块级作用域
来源：http://smo.hnqzz.top

Go:   花括号块级作用域
来源：http://rnn.hywenlv.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://thg.gzhubu.top

C#:   块级作用域
来源：http://dpp.jqgfzy.top

[C11] 模块导入与导出
来源：http://ujz.cqqwz.cn

Py:   from module import func
来源：http://nvp.nanxinkj.top

PHP:  require "file.php";  或 use App\Service;
来源：http://jfb.cucudq.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://lwe.yj20258888.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rqb.316326.xyz

Java: import java.util.List;
来源：http://oig.dianchejie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kgb.haohaochexian.top

Ruby: require "json"; require_relative "./util"
来源：http://lsy.bjfxy.top

C#:   using System.Text;
来源：http://hhp.feifeiyinyue.top

[C12] 立即执行函数 IIFE
来源：http://myg.chenzaomai.com

Py:   (lambda: print("run"))()
来源：http://tsx.sufxvd.cn

PHP:  (function () { echo "run"; })();
来源：http://otm.jianghu66.top

JS:   (() => { console.log("run"); })();
来源：http://iat.dianchejie.cn

TS:   (() => { console.log("run"); })();
来源：http://chd.cheryme.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wka.zdqjudy.top

Go:   func() { fmt.Println("run") }()
来源：http://esw.zdqjudy.top

Ruby: -> { puts "run" }.call
来源：http://jrw.hammf.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hik.jlsjyb.cn

[C13] 类型声明 / 类型注解
来源：http://wdc.zhongyouzk.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://khc.zhijiandao.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kyj.wangshuangyany.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mzx.shanyushiyangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://elx.ehwqpu.com

Java: int add(int a, int b) { return a + b; }
来源：http://qte.uphjek.com

Go:   func add(a, b int) int
来源：http://pxw.hesvh.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uyi.jiagoushi.top

C#:   int Add(int a, int b) => a + b;
来源：http://ghi.iojbl.cn

[C14] 泛型函数
来源：http://upc.havefunace.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ynh.redwolf501.top

PHP:  // 无泛型
来源：http://fwu.nanxinkj.top

JS:   // 无泛型
来源：http://jks.feifeiyinyue.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vyg.gotoacloud.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bls.redwolf501.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://aza.quarkkingdee.top

Ruby: # 无泛型
来源：http://wpe.andypj.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qrv.jlsjyb.cn

[C15] 解构 / 展开参数
来源：http://gsy.yonumen.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jbn.fktsv.cn

PHP:  [$a, $b] = $pair;
来源：http://xyc.zdbjq.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tub.fanxiaobao.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nuj.tian-w.cn

Java: // 无解构
来源：http://oks.wangdashe.top

Go:   // 无解构
来源：http://bqa.mhx1999.top

Ruby: a, b = pair
来源：http://biz.xinyue.icu

C#:   var (a, b) = pair;
来源：http://lrk.aibaodan.cn

[C16] 函数 / 方法重载
来源：http://inw.zhijiandao.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mow.nanxinkj.top

PHP:  // 无重载
来源：http://lsi.cheryme.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://xvv.hfpthk.cn

TS:   // 用联合类型或重载签名声明
来源：http://cqd.smart0.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://xph.hysaishi.cn

Go:   // 无重载：用不同函数名
来源：http://hom.fzhhl.top

Ruby: # 无重载：靠动态参数
来源：http://hpq.jianghu66.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://gdr.gogol.net.cn

================================================================================
来源：http://bsv.andypj.xyz

D. 数组 / 列表 / 集合
来源：http://bkm.52xcode.cn

================================================================================
来源：http://uut.hfpthk.cn

[D01] 创建数组 / 列表
来源：http://taj.jqgufenzy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://zka.shangyingyoupin.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ehx.ctjpmb.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://chi.ybcxt.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://pww.daxiang520.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mpi.ydjk.org.cn

Go:   arr := []int{1, 2, 3}
来源：http://dzm.52xcode.cn

Ruby: arr = [1, 2, 3]
来源：http://eee.cucudq.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dzx.cheryme.top

[D02] 追加元素到末尾
来源：http://lvx.epnwcf.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tcr.yj20258.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vyx.jqgfzy.top

JS:   arr.push(4);
来源：http://idi.ydjk.org.cn

TS:   arr.push(4);
来源：http://vwi.gogol.net.cn

Java: list.add(4);
来源：http://iit.tanke756.top

Go:   arr = append(arr, 4)
来源：http://ula.gaohongyu789.top

Ruby: arr << 4; arr.push(5)
来源：http://ldf.hfpthk.cn

C#:   list.Add(4);
来源：http://dgh.yanxiufei.cn

[D03] 在指定位置插入元素
来源：http://dyk.jinghuilouyu.cn

Py:   arr.insert(0, 0)
来源：http://wto.mhx1999.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qsb.shuidangran.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sft.fengsongda.top

TS:   arr.splice(0, 0, 0);
来源：http://ptv.zdbjq.cn

Java: list.add(0, 0);
来源：http://aub.jinghuilouyu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zkn.hesvh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rkj.mhx1999.top

C#:   list.Insert(0, 0);
来源：http://kqr.yj202588.top

[D04] 删除元素
来源：http://wco.havefunace.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uum.tian-w.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ref.smart0.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fna.snrcjt.cn

TS:   arr.splice(0, 1);
来源：http://skd.bbcook.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pfj.bbcook.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ipn.zhiwuduotai.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://urh.nanxuanxn.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cxu.sjlbkw.cn

[D05] 访问与修改元素
来源：http://vih.wangshuangyany.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qfz.shuidangran.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cys.fzhhl.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mxu.cucudq.cn

TS:   arr[0]; arr.at(-1);
来源：http://uch.ywan-chungtsiang.top

Java: list.get(0); list.set(0, 9);
来源：http://wom.jqgufenzy.top

Go:   arr[0]; arr[0] = 9
来源：http://zwx.mhx1999.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pek.zhengqikj.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://evc.xziqi.cn

[D06] 数组长度
来源：http://sss.ydjk.org.cn

Py:   len(arr)
来源：http://hxs.chenjidiqi.icu

PHP:  count($arr);
来源：http://msb.jqgfzy.top

JS:   arr.length
来源：http://eyw.cdnleiting.top

TS:   arr.length
来源：http://vzr.iojbl.cn

Java: list.size();
来源：http://flt.chenlongwang.top

Go:   len(arr)
来源：http://bon.ctjpmb.com

Ruby: arr.length; arr.size
来源：http://zjg.zdbjq.cn

C#:   list.Count;
来源：http://ibh.0kj1m.cn

[D07] 切片 / 取子数组
来源：http://rtq.guannengcc.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bhj.xuetiantiany.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xbd.shangyingyoupin.top

JS:   arr.slice(1, 4);
来源：http://maf.jianghu66.top

TS:   arr.slice(1, 4);
来源：http://dan.jianghu66.top

Java: list.subList(1, 4);
来源：http://xdc.yanxiufei.cn

Go:   arr[1:4]
来源：http://rup.zdbjq.cn

Ruby: arr[1, 3]
来源：http://ubq.zhaomingkeji.xyz

C#:   list.GetRange(1, 3);
来源：http://vwe.iojbl.cn

[D08] 合并两个数组
来源：http://okc.epnwcf.com

Py:   a + b;  a.extend(b)
来源：http://zua.hesvh.cn

PHP:  array_merge($a, $b);
来源：http://cle.xuetiantiany.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ncu.pycfn.com

TS:   [...a, ...b];
来源：http://nvr.xziqi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jkh.gzhubu.top

Go:   append(a, b...)
来源：http://czc.tanke756.top

Ruby: a + b;  a.concat(b)
来源：http://rop.hysaishi.cn

C#:   a.Concat(b).ToList()
来源：http://jjh.daria6918.cn

[D09] 排序（升序）
来源：http://plf.xingfuxueyuan.xyz

Py:   sorted(arr);  arr.sort()
来源：http://iki.jiagoushi.top

PHP:  sort($arr);
来源：http://eaa.gaohongyu789.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bzv.ivvv.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://rft.hywenlv.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://oec.bbcook.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lzv.yj20258.top

Ruby: arr.sort
来源：http://opd.ybcxt.top

C#:   list.Sort();
来源：http://hqa.uphjek.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://ipa.ydjk.org.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zvl.pengpengdd.cyou

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lib.andypj.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hlt.sufxvd.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ywc.hongshengwenyu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vts.jinqigufen.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kot.wangdashe.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://obg.wangdashe.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ggl.yangfankeji.com

[D11] 反转数组
来源：http://udp.tianlin.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://smj.fktsv.cn

PHP:  array_reverse($arr);
来源：http://obv.xylfe.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xkd.feifeiyinyue.top

TS:   [...arr].reverse();
来源：http://yix.chenzaomai.com

Java: Collections.reverse(list);
来源：http://njo.zycfv.cn

Go:   slices.Reverse(arr)
来源：http://xql.sysykeji.top

Ruby: arr.reverse
来源：http://ddn.jinqigfzy.top

C#:   list.Reverse();
来源：http://jsq.jlsjyb.cn

[D12] 查找元素下标
来源：http://wii.xylfe.cn

Py:   arr.index(x);  x in arr
来源：http://adt.ctjpmb.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ede.yj202588.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xwf.cdnleiting.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fyk.kuanghao11.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vnv.jlsjyb.cn

Go:   slices.Index(arr, x)
来源：http://kyn.shanyushiyangtech.top

Ruby: arr.index(x)
来源：http://rsq.vqdsnc.cn

C#:   list.IndexOf(x);
来源：http://uak.hcnkem.com

[D13] 过滤（保留满足条件的）
来源：http://hbk.jiagoushi.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rsw.tanke756.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gjx.hywenlv.cn

JS:   arr.filter(x => x > 3)
来源：http://hil.jinqigfzy.top

TS:   arr.filter(x => x > 3)
来源：http://uwt.guannengcc.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lar.tarul.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wvx.tianlin.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://utp.uphjek.com

C#:   list.Where(x => x > 3).ToList()
来源：http://ale.jiagoushi.top

[D14] 映射转换（每个元素变形）
来源：http://jlv.aibaodan.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mcx.zhijiandao.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ksx.vqdsnc.cn

JS:   arr.map(x => x * 2)
来源：http://hed.nanxinkj.top

TS:   arr.map(x => x * 2)
来源：http://mbi.snrcjt.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://hts.zhoulong.xyz

Go:   // 手写循环
来源：http://djg.0kj1m.cn

Ruby: arr.map { |x| x * 2 }
来源：http://mnr.daxiang520.top

C#:   list.Select(x => x * 2).ToList()
来源：http://veb.jqgufenzy.top

[D15] 去重
来源：http://neu.yuxming.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dak.daxiang520.top

PHP:  array_unique($arr);
来源：http://fdp.yfazqb.com

JS:   [...new Set(arr)]
来源：http://ljf.uphjek.com

TS:   [...new Set(arr)]
来源：http://qbx.tianlin.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hnr.guowangkeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://mkx.316326.xyz

Ruby: arr.uniq
来源：http://aiz.meibo888.top

C#:   list.Distinct().ToList()
来源：http://kxe.ehwqpu.com

[D16] 求和与平均值
来源：http://zjs.yuanzhike.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gzv.andypj.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://asj.snrcjt.cn


<!-- 参考信息 -->