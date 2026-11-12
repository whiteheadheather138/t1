代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://dxn.hnxiangtu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mgc.ivvv.top

[C04] 命名参数 / 关键字参数
来源：http://izj.316326.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://msb.yueranfly.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dnn.bbcook.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qpp.yj20258888.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ztg.pycfn.com

Java: // 无：用 Builder 模式或 record
来源：http://xdr.chenlongwang.top

Go:   // 无：用配置结构体参数
来源：http://pdf.fanxiaobao.xyz

Ruby: f(a: 1, b: 2)
来源：http://vfr.tianlin.xyz

C#:   f(a: 1, b: 2)
来源：http://zpl.shuidangran.top

[C05] 返回多个值
来源：http://cna.hnqzz.top

Py:   return a, b
来源：http://kgj.gotoacloud.top

PHP:  return [$a, $b];
来源：http://hlg.cashguo.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://cqs.wangdashe.top

TS:   return { a, b };
来源：http://itq.smart0.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yqh.vehdjk.com

Go:   return a, b
来源：http://wgy.zhaomingkeji.xyz

Ruby: return a, b
来源：http://rku.yj202588.top

C#:   return (a, b);              // ValueTuple
来源：http://mly.yuxming.cn

[C06] 匿名函数 / lambda
来源：http://fma.xinyue.icu

Py:   square = lambda x: x * x
来源：http://kdu.xziqi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ozh.ybcxt.top

JS:   const square = x => x * x;
来源：http://gpj.vehdjk.com

TS:   const square = (x: number): number => x * x;
来源：http://pzr.cdnleiting.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xwj.kuanghao11.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hzp.pycfn.com

Ruby: square = ->(x) { x * x }
来源：http://utp.hesvh.cn

C#:   Func<int, int> square = x => x * x;
来源：http://riu.yvedp.cn

[C07] 把函数作为参数传入
来源：http://qxy.fehbvm.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jmt.tian-w.cn

PHP:  array_map("strtoupper", $arr);
来源：http://dtm.yj20258.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://irz.xuetiantiany.cn

TS:   arr.map(String)
来源：http://hpn.cqqwz.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gjd.snrcjt.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sqh.c1oappe.top

Ruby: arr.map(&:upcase)
来源：http://acz.hesvh.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sof.cheryme.top

[C08] 闭包
来源：http://wde.c1oappe.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vxs.tarul.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://iee.hongshengwenyu.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://act.c1oappe.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gtr.zhixingplan.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://inm.tianlin.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://uzg.vehdjk.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hxl.ctjpmb.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://htz.fengsongda.top

[C09] 递归
来源：http://foh.yongpay.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pxp.fengsongda.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pyb.shangyingyoupin.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ert.yonumen.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qym.fzhhl.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hlo.sysykeji.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ztp.hesvh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mbx.iojbl.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mrq.birdmap.top

[C10] 变量作用域
来源：http://zoc.zhaomingkeji.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rmp.gzhubu.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://oqe.epnwcf.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rbo.meibo888.top

TS:   同 JS
来源：http://vjy.kuanghao11.cn

Java: 方法内为块级作用域
来源：http://bfj.gzhubu.top

Go:   花括号块级作用域
来源：http://qli.yangfankeji.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ror.52xcode.cn

C#:   块级作用域
来源：http://ibx.hnxiangtu.top

[C11] 模块导入与导出
来源：http://dhy.nanxuanxn.top

Py:   from module import func
来源：http://dyp.shuidangran.top

PHP:  require "file.php";  或 use App\Service;
来源：http://oof.ywan-chungtsiang.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://uij.nanxuanxn.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jsf.shangyingyoupin.top

Java: import java.util.List;
来源：http://pgj.nanxuanxn.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yxr.yj20258888.top

Ruby: require "json"; require_relative "./util"
来源：http://lcd.meibo888.top

C#:   using System.Text;
来源：http://ebz.vehdjk.com

[C12] 立即执行函数 IIFE
来源：http://scq.xziqi.cn

Py:   (lambda: print("run"))()
来源：http://pmb.nwbrower.top

PHP:  (function () { echo "run"; })();
来源：http://zph.dashuyun.cn

JS:   (() => { console.log("run"); })();
来源：http://pkd.haohaochexian.top

TS:   (() => { console.log("run"); })();
来源：http://eod.shangyingyoupin.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xwt.zdqjudy.top

Go:   func() { fmt.Println("run") }()
来源：http://tym.zdqjudy.top

Ruby: -> { puts "run" }.call
来源：http://xka.meibo888.top

C#:   // 无 IIFE：用静态构造函数
来源：http://tjn.andypj.xyz

[C13] 类型声明 / 类型注解
来源：http://gwq.c1oappe.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cjp.jyoumei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yuy.yj20258888.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fgd.gotoacloud.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xxz.fktsv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qyq.tianlin.xyz

Go:   func add(a, b int) int
来源：http://ehc.yj202588.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://utb.nwbrower.top

C#:   int Add(int a, int b) => a + b;
来源：http://csy.tanke756.top

[C14] 泛型函数
来源：http://idr.kuanghao11.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sbb.hfpthk.cn

PHP:  // 无泛型
来源：http://xiz.wangshuangyany.cn

JS:   // 无泛型
来源：http://hwc.yueranfly.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sxg.jinqigufen.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rbz.uphjek.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gbl.hesvh.cn

Ruby: # 无泛型
来源：http://dxb.zhoulong.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://asv.feifeiyinyue.top

[C15] 解构 / 展开参数
来源：http://wkk.ctjpmb.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://idx.jlsjyb.cn

PHP:  [$a, $b] = $pair;
来源：http://gdp.9152youxi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ssn.guannengcc.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jrl.jinqigufen.top

Java: // 无解构
来源：http://nue.daxiang520.top

Go:   // 无解构
来源：http://hju.xylfe.cn

Ruby: a, b = pair
来源：http://whq.zdqjudy.top

C#:   var (a, b) = pair;
来源：http://ple.cqqwz.cn

[C16] 函数 / 方法重载
来源：http://frk.yuanzhike.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fnd.vehdjk.com

PHP:  // 无重载
来源：http://ben.jlsjyb.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://huw.zhengqikj.top

TS:   // 用联合类型或重载签名声明
来源：http://okh.cucudq.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://sbz.yonumen.top

Go:   // 无重载：用不同函数名
来源：http://ygh.zdqjudy.top

Ruby: # 无重载：靠动态参数
来源：http://uof.ydjk.org.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://cgy.guowangkeji.top

================================================================================
来源：http://mpr.havefunace.top

D. 数组 / 列表 / 集合
来源：http://vys.hywenlv.cn

================================================================================
来源：http://yxa.zhijiandao.cn

[D01] 创建数组 / 列表
来源：http://ith.ctjpmb.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://ssu.tianlin.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xpg.guannengcc.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fgs.jlsjyb.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://cah.ydjk.org.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ykk.jinghuilouyu.cn

Go:   arr := []int{1, 2, 3}
来源：http://ubi.yuxming.cn

Ruby: arr = [1, 2, 3]
来源：http://dpo.tianlin.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dty.gzhubu.top

[D02] 追加元素到末尾
来源：http://wlz.dianchejie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bvt.zhiwuduotai.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://knc.cashguo.top

JS:   arr.push(4);
来源：http://luz.epnwcf.com

TS:   arr.push(4);
来源：http://lia.xuetiantiany.cn

Java: list.add(4);
来源：http://oyt.ybcxt.top

Go:   arr = append(arr, 4)
来源：http://jrh.iojbl.cn

Ruby: arr << 4; arr.push(5)
来源：http://ezn.xinyue.icu

C#:   list.Add(4);
来源：http://pno.aizwys.cn

[D03] 在指定位置插入元素
来源：http://xph.epnwcf.com

Py:   arr.insert(0, 0)
来源：http://czs.dianchejie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://otk.haohaochexian.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uxb.jinqigufen.top

TS:   arr.splice(0, 0, 0);
来源：http://abu.xuanzx.com

Java: list.add(0, 0);
来源：http://sri.aizwys.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mry.xuetiantiany.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lwh.jinyuanbaomall.cn

C#:   list.Insert(0, 0);
来源：http://nis.bjfxy.top

[D04] 删除元素
来源：http://fqc.xziqi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://oyv.fktsv.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lrx.dashuyun.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vco.hongshengwenyu.top

TS:   arr.splice(0, 1);
来源：http://wzt.fehbvm.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://oae.jqgufenzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ndx.hammf.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jfz.jinqigfzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ajo.fanxiaobao.xyz

[D05] 访问与修改元素
来源：http://mzx.cqqwz.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kog.meibo888.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fdr.jianghu66.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://boi.tianlin.xyz

TS:   arr[0]; arr.at(-1);
来源：http://jqw.iojbl.cn

Java: list.get(0); list.set(0, 9);
来源：http://zeq.yonumen.top

Go:   arr[0]; arr[0] = 9
来源：http://hlq.xuetiantiany.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://niy.cqqwz.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cmr.52xcode.cn

[D06] 数组长度
来源：http://uuc.yanxiufei.cn

Py:   len(arr)
来源：http://ttm.zhixingplan.top

PHP:  count($arr);
来源：http://wlu.birdmap.top

JS:   arr.length
来源：http://eoj.hnxiangtu.top

TS:   arr.length
来源：http://lcy.zhongyouzk.top

Java: list.size();
来源：http://avn.ydjk.org.cn

Go:   len(arr)
来源：http://pwg.yj202588.top

Ruby: arr.length; arr.size
来源：http://zye.chenjidiqi.icu

C#:   list.Count;
来源：http://kcw.hcnkem.com

[D07] 切片 / 取子数组
来源：http://aij.yueranfly.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rsd.hesvh.cn

PHP:  array_slice($arr, 1, 3);
来源：http://rtd.smart0.xyz

JS:   arr.slice(1, 4);
来源：http://uer.9152youxi.cn

TS:   arr.slice(1, 4);
来源：http://cez.316326.xyz

Java: list.subList(1, 4);
来源：http://cvs.52xcode.cn

Go:   arr[1:4]
来源：http://qbi.mhx1999.top

Ruby: arr[1, 3]
来源：http://idh.chenzaomai.com

C#:   list.GetRange(1, 3);
来源：http://skm.wangshuangyany.cn

[D08] 合并两个数组
来源：http://wjd.havefunace.top

Py:   a + b;  a.extend(b)
来源：http://hpb.zhaomingkeji.xyz

PHP:  array_merge($a, $b);
来源：http://ekx.tarul.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://lhe.ywan-chungtsiang.top

TS:   [...a, ...b];
来源：http://zea.nanxuanxn.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://amg.yuxming.cn

Go:   append(a, b...)
来源：http://fab.hfpthk.cn

Ruby: a + b;  a.concat(b)
来源：http://trn.daxiang520.top

C#:   a.Concat(b).ToList()
来源：http://kki.yonumen.top

[D09] 排序（升序）
来源：http://yxf.cqqwz.cn

Py:   sorted(arr);  arr.sort()
来源：http://ryj.xingfuxueyuan.xyz

PHP:  sort($arr);
来源：http://auj.guannengcc.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qft.bjfxy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ncd.fehbvm.com

Java: Collections.sort(list);  list.sort(null);
来源：http://ipw.yangfankeji.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jxk.gotoacloud.top

Ruby: arr.sort
来源：http://hcy.cucudq.cn

C#:   list.Sort();
来源：http://ogp.jianghu66.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ewp.guowangkeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sel.bbcook.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fee.snrcjt.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mbi.jiagoushi.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pfl.wangshuangyany.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jbh.haohaochexian.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dql.sufxvd.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hba.hfpthk.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nik.vqdsnc.cn

[D11] 反转数组
来源：http://qnb.ppjwa.cn

Py:   arr[::-1];  arr.reverse()
来源：http://tnp.c1oappe.top

PHP:  array_reverse($arr);
来源：http://wzo.zhongyouzk.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rdl.shanyushiyangtech.top

TS:   [...arr].reverse();
来源：http://jin.cheryme.top

Java: Collections.reverse(list);
来源：http://iya.ctjpmb.com

Go:   slices.Reverse(arr)
来源：http://hzg.yvedp.cn

Ruby: arr.reverse
来源：http://cyo.yangfankeji.com

C#:   list.Reverse();
来源：http://fqq.hywenlv.cn

[D12] 查找元素下标
来源：http://cse.feifeiyinyue.top

Py:   arr.index(x);  x in arr
来源：http://bem.zycfv.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rqy.yvedp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cax.c1oappe.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://phe.wangshuangyany.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qbc.quarkkingdee.top

Go:   slices.Index(arr, x)
来源：http://mpu.9152youxi.cn

Ruby: arr.index(x)
来源：http://xxl.meibo888.top

C#:   list.IndexOf(x);
来源：http://ozy.zhengqikj.top

[D13] 过滤（保留满足条件的）
来源：http://qrv.zhiwuduotai.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jpf.snrcjt.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gpd.xinyue.icu

JS:   arr.filter(x => x > 3)
来源：http://zci.yvedp.cn

TS:   arr.filter(x => x > 3)
来源：http://zzj.zdqjudy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yyk.yanxiufei.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://adj.snrcjt.cn

Ruby: arr.select { |x| x > 3 }
来源：http://yfz.sufxvd.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hcf.jiagoushi.top

[D14] 映射转换（每个元素变形）
来源：http://xok.dianchejie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vcb.redwolf501.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ydl.xuetiantiany.cn

JS:   arr.map(x => x * 2)
来源：http://mfq.0kj1m.cn

TS:   arr.map(x => x * 2)
来源：http://pvm.sweek.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://vqa.vehdjk.com

Go:   // 手写循环
来源：http://fpt.aibaodan.cn

Ruby: arr.map { |x| x * 2 }
来源：http://npg.smart0.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://oul.chenjidiqi.icu

[D15] 去重
来源：http://rfm.sufxvd.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qkg.zhijiandao.cn

PHP:  array_unique($arr);
来源：http://pzf.9152youxi.cn

JS:   [...new Set(arr)]
来源：http://vkg.cashguo.top

TS:   [...new Set(arr)]
来源：http://jpr.tian-w.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bli.chenjidiqi.icu

Go:   // 用 map[T]struct{} 手写
来源：http://bnz.sjlbkw.cn

Ruby: arr.uniq
来源：http://myd.yanxiufei.cn

C#:   list.Distinct().ToList()
来源：http://kbu.yonumen.top

[D16] 求和与平均值
来源：http://ooi.smart0.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lxi.shanyushiyangtech.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cpd.zhaomingkeji.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hwv.chenlongwang.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cak.hongshengwenyu.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fju.fengsongda.top

Go:   // 手写循环累加
来源：http://isb.gogol.net.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yni.316326.xyz

C#:   list.Sum();  list.Average()
来源：http://iqy.hcnkem.com

[D17] 最大值与最小值
来源：http://isu.316326.xyz

Py:   max(arr);  min(arr)
来源：http://qci.shanyushiyangtech.top

PHP:  max($arr);  min($arr);
来源：http://lff.yueranfly.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ipt.xinyue.icu

TS:   Math.max(...arr);
来源：http://ler.cheryme.top

Java: Collections.max(list);  Collections.min(list);
来源：http://gdw.cashguo.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vea.pengpengdd.cyou

Ruby: arr.max;  arr.min
来源：http://vol.zhixingplan.top

C#:   list.Max();  list.Min()
来源：http://spl.sysykeji.top

[D18] 扁平化嵌套数组
来源：http://bxl.hnqzz.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cwx.feifeiyinyue.top

PHP:  array_merge(...$nested);
来源：http://ifz.cashguo.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ptx.mhx1999.top

TS:   nested.flat();
来源：http://zcq.hnqzz.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://iyv.jinghuilouyu.cn

Go:   // 手写双层循环
来源：http://gkp.birdmap.top

Ruby: nested.flatten
来源：http://bjx.ydzc1.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://zpi.hnxiangtu.top

[D19] 按字段分组
来源：http://kpi.jiagoushi.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://znk.fktsv.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yjy.jinghuilouyu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sdu.jqgfzy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://hfg.hcnkem.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kps.aibaodan.cn

Go:   // 手写 map[string][]T
来源：http://aoe.ehwqpu.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://doj.kuanghao11.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ryt.zhiwuduotai.top

[D20] 统计每个元素出现次数
来源：http://oig.tarul.cn

Py:   Counter(arr)
来源：http://hod.aibaodan.cn

PHP:  array_count_values($arr);
来源：http://bwk.tian-w.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iib.yj20258888.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://scy.fanxiaobao.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pnb.nwbrower.top

Go:   // 手写 map[T]int
来源：http://dxq.bjfxy.top


<!-- 参考信息 -->