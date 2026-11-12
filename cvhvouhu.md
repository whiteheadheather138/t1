代发 wailian999

Java: if (data == null) return;
来源：http://wkf.jinqigfzy.top

Go:   if data == nil { return }
来源：http://ldd.ctjpmb.com

Ruby: return if data.nil?
来源：http://frn.xziqi.cn

C#:   if (data == null) return;
来源：http://pny.cashguo.top

================================================================================
来源：http://otl.jinyuanbaomall.cn

C. 函数与作用域
来源：http://ykm.yj202588.top

================================================================================
来源：http://rrf.xingfuxueyuan.xyz

[C01] 定义函数
来源：http://rui.ppjwa.cn

Py:   def add(a, b): return a + b
来源：http://ong.9152youxi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jgt.xuanzx.com

JS:   function add(a, b) { return a + b; }
来源：http://zip.fengsongda.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vff.ppjwa.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fsq.mhx1999.top

Go:   func add(a, b int) int { return a + b }
来源：http://wko.daxiang520.top

Ruby: def add(a, b); a + b; end
来源：http://euh.9152youxi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xko.hnqzz.top

[C02] 默认参数
来源：http://tgz.yj20258.top

Py:   def greet(name="World"): return name
来源：http://ktn.cdnleiting.top

PHP:  function greet($name = "World") { return $name; }
来源：http://fqk.fehbvm.com

JS:   function greet(name = "World") { return name; }
来源：http://yse.aibaodan.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://afr.uphjek.com

Java: // 无默认参数：方法重载或 Optional
来源：http://npq.fzhhl.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ica.jyoumei.cn

Ruby: def greet(name = "World") = name
来源：http://ayi.chenzaomai.com

C#:   string Greet(string name = "World") => name;
来源：http://heq.guowangkeji.top

[C03] 可变参数
来源：http://viv.yuanzhike.top

Py:   def total(*args): return sum(args)
来源：http://cme.yonumen.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ygg.hesvh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gly.shanyushiyangkeji.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://okx.iojbl.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zsj.yueranfly.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://imk.guannengcc.top

Ruby: def total(*nums); nums.sum; end
来源：http://dhv.cashguo.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tkh.birdmap.top

[C04] 命名参数 / 关键字参数
来源：http://gfi.mhx1999.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tgb.ybcxt.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ujr.ppjwa.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jev.zhaomingkeji.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rqo.zhengqikj.top

Java: // 无：用 Builder 模式或 record
来源：http://lhb.fehbvm.com

Go:   // 无：用配置结构体参数
来源：http://xkm.52xcode.cn

Ruby: f(a: 1, b: 2)
来源：http://uqy.c1oappe.top

C#:   f(a: 1, b: 2)
来源：http://orm.jiagoushi.top

[C05] 返回多个值
来源：http://gdf.wangdashe.top

Py:   return a, b
来源：http://ikr.zhijiandao.cn

PHP:  return [$a, $b];
来源：http://xfv.fanxiaobao.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://ats.zhengqikj.top

TS:   return { a, b };
来源：http://zoi.hywenlv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hzx.sxryk.cn

Go:   return a, b
来源：http://clo.fzhhl.top

Ruby: return a, b
来源：http://csv.zhongyouzk.top

C#:   return (a, b);              // ValueTuple
来源：http://vmm.zhongyouzk.top

[C06] 匿名函数 / lambda
来源：http://gua.zdqjudy.top

Py:   square = lambda x: x * x
来源：http://ezv.vqdsnc.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://cpi.havefunace.top

JS:   const square = x => x * x;
来源：http://acx.yfazqb.com

TS:   const square = (x: number): number => x * x;
来源：http://uay.zhijiandao.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://agq.hammf.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zlc.jinqigfzy.top

Ruby: square = ->(x) { x * x }
来源：http://qli.tianlin.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://cvz.9152youxi.cn

[C07] 把函数作为参数传入
来源：http://ljz.yj202588.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://czp.ehwqpu.com

PHP:  array_map("strtoupper", $arr);
来源：http://umd.zhixingplan.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://esw.yj20258.top

TS:   arr.map(String)
来源：http://xev.ppjwa.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qfl.xziqi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bkv.tarul.cn

Ruby: arr.map(&:upcase)
来源：http://tmk.zhijiandao.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://vaa.jinyuanbaomall.cn

[C08] 闭包
来源：http://meo.gzhubu.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gqb.gotoacloud.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zho.hesvh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jvn.jlsjyb.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://adu.ctjpmb.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wnx.quarkkingdee.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dcn.xziqi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://myy.xingfuxueyuan.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lsh.chenlongwang.top

[C09] 递归
来源：http://duq.xuetiantiany.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://iqh.smart0.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://eix.tarul.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vob.hnqzz.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://utr.hnqzz.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://obg.ivvv.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qnt.daria6918.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tbw.bbcook.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tpu.shuidangran.top

[C10] 变量作用域
来源：http://qad.ctjpmb.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://log.cucudq.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zzc.xuanzx.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qzb.sjlbkw.cn

TS:   同 JS
来源：http://wgv.zhongyouzk.top

Java: 方法内为块级作用域
来源：http://utb.daria6918.cn

Go:   花括号块级作用域
来源：http://jyr.ybcxt.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qje.chenlongwang.top

C#:   块级作用域
来源：http://efm.birdmap.top

[C11] 模块导入与导出
来源：http://urx.uphjek.com

Py:   from module import func
来源：http://fir.dashuyun.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://iwd.bjfxy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://fde.hammf.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qiy.tian-w.cn

Java: import java.util.List;
来源：http://nil.andypj.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://izc.yuxming.cn

Ruby: require "json"; require_relative "./util"
来源：http://wje.yvedp.cn

C#:   using System.Text;
来源：http://ndh.xuetiantiany.cn

[C12] 立即执行函数 IIFE
来源：http://gks.wangshuangyany.cn

Py:   (lambda: print("run"))()
来源：http://kxz.dianchejie.cn

PHP:  (function () { echo "run"; })();
来源：http://pck.jiagoushi.top

JS:   (() => { console.log("run"); })();
来源：http://lym.yueranfly.top

TS:   (() => { console.log("run"); })();
来源：http://pyj.hongshengwenyu.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xqv.tianlin.xyz

Go:   func() { fmt.Println("run") }()
来源：http://wex.zdqjudy.top

Ruby: -> { puts "run" }.call
来源：http://zsc.yvedp.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://vze.tanke756.top

[C13] 类型声明 / 类型注解
来源：http://nnc.sysykeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://uji.ctjpmb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bun.sjlbkw.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wso.redwolf501.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bjk.sufxvd.cn

Java: int add(int a, int b) { return a + b; }
来源：http://isf.xylfe.cn

Go:   func add(a, b int) int
来源：http://hjk.wangshuangyany.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://oaq.ehwqpu.com

C#:   int Add(int a, int b) => a + b;
来源：http://xbp.guannengcc.top

[C14] 泛型函数
来源：http://cqr.fanxiaobao.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lba.tarul.cn

PHP:  // 无泛型
来源：http://otl.feifeiyinyue.top

JS:   // 无泛型
来源：http://vzc.hesvh.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://soi.sjlbkw.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vqv.hesvh.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://acb.smart0.xyz

Ruby: # 无泛型
来源：http://leb.yuxming.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sfp.cqqwz.cn

[C15] 解构 / 展开参数
来源：http://amm.cucudq.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dsv.smart0.xyz

PHP:  [$a, $b] = $pair;
来源：http://ivc.wangdashe.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uii.fktsv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fwo.daxiang520.top

Java: // 无解构
来源：http://dxn.yangfankeji.com

Go:   // 无解构
来源：http://zgx.cheryme.top

Ruby: a, b = pair
来源：http://raw.sysykeji.top

C#:   var (a, b) = pair;
来源：http://gvz.ywan-chungtsiang.top

[C16] 函数 / 方法重载
来源：http://lgx.ywan-chungtsiang.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://uns.cdnleiting.top

PHP:  // 无重载
来源：http://rws.tanke756.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://eya.xuanzx.com

TS:   // 用联合类型或重载签名声明
来源：http://hdn.jinghuilouyu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mgh.zhaomingkeji.xyz

Go:   // 无重载：用不同函数名
来源：http://rhf.ppjwa.cn

Ruby: # 无重载：靠动态参数
来源：http://fgr.sufxvd.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qbg.tarul.cn

================================================================================
来源：http://sfo.xingfuxueyuan.xyz

D. 数组 / 列表 / 集合
来源：http://frg.dianchejie.cn

================================================================================
来源：http://grb.smart0.xyz

[D01] 创建数组 / 列表
来源：http://owy.xuanzx.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://dak.zhijiandao.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ycg.nanxinkj.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jsf.ybcxt.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://bbr.ywan-chungtsiang.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sik.fengsongda.top

Go:   arr := []int{1, 2, 3}
来源：http://xso.0kj1m.cn

Ruby: arr = [1, 2, 3]
来源：http://zeq.epnwcf.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hqu.hammf.cn

[D02] 追加元素到末尾
来源：http://qyi.bjfxy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xsl.ivvv.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hwm.zycfv.cn

JS:   arr.push(4);
来源：http://pbp.zhoulong.xyz

TS:   arr.push(4);
来源：http://zdv.tianlin.xyz

Java: list.add(4);
来源：http://snm.gzhubu.top

Go:   arr = append(arr, 4)
来源：http://vrz.316326.xyz

Ruby: arr << 4; arr.push(5)
来源：http://ytn.fzhhl.top

C#:   list.Add(4);
来源：http://vsl.shangyingyoupin.top

[D03] 在指定位置插入元素
来源：http://kzi.zdbjq.cn

Py:   arr.insert(0, 0)
来源：http://mhy.sweek.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fku.yonumen.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rzy.yj202588.top

TS:   arr.splice(0, 0, 0);
来源：http://znf.jqgufenzy.top

Java: list.add(0, 0);
来源：http://ftb.0kj1m.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vdp.zhoulong.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dee.jiagoushi.top

C#:   list.Insert(0, 0);
来源：http://xdq.jinqigfzy.top

[D04] 删除元素
来源：http://ase.vehdjk.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://awv.xuetiantiany.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sxp.ivvv.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kuj.zdqjudy.top

TS:   arr.splice(0, 1);
来源：http://wxw.ybcxt.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cte.bjfxy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ojz.redwolf501.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ljy.gaohongyu789.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ekd.ybcxt.top

[D05] 访问与修改元素
来源：http://aii.jqgufenzy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kiz.ywan-chungtsiang.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bzg.ywan-chungtsiang.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xuv.jinghuilouyu.cn

TS:   arr[0]; arr.at(-1);
来源：http://ech.fzhhl.top

Java: list.get(0); list.set(0, 9);
来源：http://yep.tian-w.cn

Go:   arr[0]; arr[0] = 9
来源：http://akk.jinqigfzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jof.52xcode.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wfd.birdmap.top

[D06] 数组长度
来源：http://hkd.snrcjt.cn

Py:   len(arr)
来源：http://rnj.shzxlz.cn

PHP:  count($arr);
来源：http://gth.yj20258888.top

JS:   arr.length
来源：http://azi.shuidangran.top

TS:   arr.length
来源：http://bfc.jiagoushi.top

Java: list.size();
来源：http://cme.kuanghao11.cn

Go:   len(arr)
来源：http://ptg.shangyingyoupin.top

Ruby: arr.length; arr.size
来源：http://wcn.svipenyu.cn

C#:   list.Count;
来源：http://wtw.tanke756.top

[D07] 切片 / 取子数组
来源：http://hqk.zdqjudy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kjh.shzxlz.cn

PHP:  array_slice($arr, 1, 3);
来源：http://dzr.jiagoushi.top

JS:   arr.slice(1, 4);
来源：http://nss.bjfxy.top

TS:   arr.slice(1, 4);
来源：http://ljv.bjfxy.top

Java: list.subList(1, 4);
来源：http://jms.hysaishi.cn

Go:   arr[1:4]
来源：http://mkw.guannengcc.top

Ruby: arr[1, 3]
来源：http://tly.ctjpmb.com

C#:   list.GetRange(1, 3);
来源：http://rvm.jqgfzy.top

[D08] 合并两个数组
来源：http://zux.hesvh.cn

Py:   a + b;  a.extend(b)
来源：http://hfx.chenjidiqi.icu

PHP:  array_merge($a, $b);
来源：http://uzh.jqgfzy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://iio.yj20258.top

TS:   [...a, ...b];
来源：http://bro.andypj.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://iyq.xziqi.cn

Go:   append(a, b...)
来源：http://uxq.hysaishi.cn

Ruby: a + b;  a.concat(b)
来源：http://lmz.yangfankeji.com

C#:   a.Concat(b).ToList()
来源：http://kpl.jinghuilouyu.cn

[D09] 排序（升序）
来源：http://bhv.yuxming.cn

Py:   sorted(arr);  arr.sort()
来源：http://rqf.mhx1999.top

PHP:  sort($arr);
来源：http://ylf.haohaochexian.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://aue.sxryk.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://rvf.sweek.top

Java: Collections.sort(list);  list.sort(null);
来源：http://yuu.yongpay.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://map.nwbrower.top

Ruby: arr.sort
来源：http://tri.zhijiandao.cn

C#:   list.Sort();
来源：http://owe.aibaodan.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://whd.jinqigfzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://osr.shangyingyoupin.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rvu.nwbrower.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://btc.zycfv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xdv.cashguo.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://njj.9152youxi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sso.wangshuangyany.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bdu.9152youxi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zlg.zhixingplan.top

[D11] 反转数组
来源：http://tjt.feifeiyinyue.top

Py:   arr[::-1];  arr.reverse()
来源：http://xpi.ydzc1.top

PHP:  array_reverse($arr);
来源：http://bhf.dianchejie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rkn.hywenlv.cn

TS:   [...arr].reverse();
来源：http://zdh.nanxinkj.top

Java: Collections.reverse(list);
来源：http://ltn.vehdjk.com

Go:   slices.Reverse(arr)
来源：http://qfq.nanxinkj.top

Ruby: arr.reverse
来源：http://ogp.zhiwuduotai.top

C#:   list.Reverse();
来源：http://edk.cucudq.cn

[D12] 查找元素下标
来源：http://rvj.snrcjt.cn

Py:   arr.index(x);  x in arr
来源：http://nbb.ppjwa.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://isk.shanyushiyangkeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xha.epnwcf.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fma.fanxiaobao.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fag.vehdjk.com

Go:   slices.Index(arr, x)
来源：http://dxk.yj20258.top

Ruby: arr.index(x)
来源：http://kpj.zhongyouzk.top

C#:   list.IndexOf(x);
来源：http://ajv.dashuyun.cn

[D13] 过滤（保留满足条件的）
来源：http://tfg.hysaishi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bsd.9152youxi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yka.jiagoushi.top

JS:   arr.filter(x => x > 3)
来源：http://msn.jyoumei.cn

TS:   arr.filter(x => x > 3)
来源：http://kji.chenjidiqi.icu

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hji.sweek.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sop.epnwcf.com

Ruby: arr.select { |x| x > 3 }
来源：http://hbd.tanke756.top

C#:   list.Where(x => x > 3).ToList()
来源：http://pau.svipenyu.cn

[D14] 映射转换（每个元素变形）
来源：http://oap.yfazqb.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dlz.quarkkingdee.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kng.c1oappe.top

JS:   arr.map(x => x * 2)
来源：http://lcz.c1oappe.top

TS:   arr.map(x => x * 2)
来源：http://sng.uphjek.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://kjw.jqgfzy.top

Go:   // 手写循环
来源：http://jhg.hnqzz.top

Ruby: arr.map { |x| x * 2 }
来源：http://gpw.xingfuxueyuan.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://net.cashguo.top

[D15] 去重
来源：http://orz.cashguo.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hsp.yj20258.top

PHP:  array_unique($arr);
来源：http://gry.ctjpmb.com

JS:   [...new Set(arr)]
来源：http://ylx.zhaomingkeji.xyz

TS:   [...new Set(arr)]
来源：http://ffd.hnqzz.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://esw.bbcook.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xaa.zdbjq.cn

Ruby: arr.uniq
来源：http://voo.zhixingplan.top

C#:   list.Distinct().ToList()
来源：http://pnr.tarul.cn

[D16] 求和与平均值
来源：http://syc.xinyue.icu

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cdt.fktsv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hom.hongshengwenyu.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://iff.chenjidiqi.icu

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yyu.cucudq.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bld.0kj1m.cn

Go:   // 手写循环累加
来源：http://nia.xingfuxueyuan.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://phq.birdmap.top

C#:   list.Sum();  list.Average()
来源：http://nyq.vqdsnc.cn

[D17] 最大值与最小值
来源：http://exj.pengpengdd.cyou

Py:   max(arr);  min(arr)
来源：http://kho.yj20258.top


<!-- 参考信息 -->