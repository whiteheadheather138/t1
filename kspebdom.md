代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://jan.tarul.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://uxc.jinqigufen.top

[C04] 命名参数 / 关键字参数
来源：http://szj.vqdsnc.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gip.fanxiaobao.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rjg.aibaodan.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zlg.zdbjq.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uvd.xziqi.cn

Java: // 无：用 Builder 模式或 record
来源：http://jtv.jinqigufen.top

Go:   // 无：用配置结构体参数
来源：http://wrv.redwolf501.top

Ruby: f(a: 1, b: 2)
来源：http://prf.jqgufenzy.top

C#:   f(a: 1, b: 2)
来源：http://knt.iojbl.cn

[C05] 返回多个值
来源：http://ibp.chenzaomai.com

Py:   return a, b
来源：http://ygd.kuanghao11.cn

PHP:  return [$a, $b];
来源：http://mqt.zhijiandao.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://smi.xziqi.cn

TS:   return { a, b };
来源：http://hav.yangfankeji.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zuv.vehdjk.com

Go:   return a, b
来源：http://ukv.yueranfly.top

Ruby: return a, b
来源：http://jno.wangdashe.top

C#:   return (a, b);              // ValueTuple
来源：http://fwt.fehbvm.com

[C06] 匿名函数 / lambda
来源：http://dbk.jiagoushi.top

Py:   square = lambda x: x * x
来源：http://oga.nanxinkj.top

PHP:  $square = fn($x) => $x * $x;
来源：http://jvy.nanxuanxn.top

JS:   const square = x => x * x;
来源：http://eay.pengpengdd.cyou

TS:   const square = (x: number): number => x * x;
来源：http://jih.shanyushiyangtech.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pxv.gogol.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wri.hfpthk.cn

Ruby: square = ->(x) { x * x }
来源：http://wil.ybcxt.top

C#:   Func<int, int> square = x => x * x;
来源：http://omt.birdmap.top

[C07] 把函数作为参数传入
来源：http://brc.kuanghao11.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qbp.vehdjk.com

PHP:  array_map("strtoupper", $arr);
来源：http://ryq.kuanghao11.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qul.cdnleiting.top

TS:   arr.map(String)
来源：http://pov.ybcxt.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lht.fehbvm.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jjd.hnqzz.top

Ruby: arr.map(&:upcase)
来源：http://vxe.ydjk.org.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xrf.vehdjk.com

[C08] 闭包
来源：http://fqr.cheryme.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uqj.hfpthk.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://iuz.jlsjyb.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lao.vqdsnc.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rhd.svipenyu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wmk.chenlongwang.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pjl.xuetiantiany.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://iiu.zhijiandao.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://afu.birdmap.top

[C09] 递归
来源：http://nfr.c1oappe.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zzt.shzxlz.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://smb.fktsv.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://npa.hongshengwenyu.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xuq.aizwys.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tav.chenjidiqi.icu

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ejy.xingfuxueyuan.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ydl.dianchejie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cqa.nanxinkj.top

[C10] 变量作用域
来源：http://syo.yueranfly.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bmj.zhijiandao.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jpw.ivvv.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lkh.jyoumei.cn

TS:   同 JS
来源：http://wkz.svipenyu.cn

Java: 方法内为块级作用域
来源：http://ukn.9152youxi.cn

Go:   花括号块级作用域
来源：http://pvv.cucudq.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://svm.xingfuxueyuan.xyz

C#:   块级作用域
来源：http://vzm.xingfuxueyuan.xyz

[C11] 模块导入与导出
来源：http://kvg.gotoacloud.top

Py:   from module import func
来源：http://ltr.cheryme.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ipk.chenlongwang.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://vkd.yj20258888.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dke.ydzc1.top

Java: import java.util.List;
来源：http://jyh.zhixingplan.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://akr.52xcode.cn

Ruby: require "json"; require_relative "./util"
来源：http://zex.sxryk.cn

C#:   using System.Text;
来源：http://lvz.hywenlv.cn

[C12] 立即执行函数 IIFE
来源：http://sgc.hongshengwenyu.top

Py:   (lambda: print("run"))()
来源：http://byl.sweek.top

PHP:  (function () { echo "run"; })();
来源：http://apw.jiagoushi.top

JS:   (() => { console.log("run"); })();
来源：http://osy.shuidangran.top

TS:   (() => { console.log("run"); })();
来源：http://xaz.316326.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://akt.andypj.xyz

Go:   func() { fmt.Println("run") }()
来源：http://lqp.chenlongwang.top

Ruby: -> { puts "run" }.call
来源：http://bpm.zhixingplan.top

C#:   // 无 IIFE：用静态构造函数
来源：http://rqq.316326.xyz

[C13] 类型声明 / 类型注解
来源：http://lih.yuxming.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zte.fanxiaobao.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ypm.xuetiantiany.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kch.andypj.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iae.fktsv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ihk.chenlongwang.top

Go:   func add(a, b int) int
来源：http://spj.wangshuangyany.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kys.gaohongyu789.top

C#:   int Add(int a, int b) => a + b;
来源：http://rvx.yuxming.cn

[C14] 泛型函数
来源：http://boj.yangfankeji.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fqi.yuanzhike.top

PHP:  // 无泛型
来源：http://dij.wangdashe.top

JS:   // 无泛型
来源：http://uwa.nanxinkj.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tai.jinyuanbaomall.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zpj.yj20258.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://akv.smart0.xyz

Ruby: # 无泛型
来源：http://cqc.iojbl.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qrr.wangdashe.top

[C15] 解构 / 展开参数
来源：http://feg.xuanzx.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yov.yueranfly.top

PHP:  [$a, $b] = $pair;
来源：http://cnd.vehdjk.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dyt.jqgfzy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://iet.0kj1m.cn

Java: // 无解构
来源：http://egy.sufxvd.cn

Go:   // 无解构
来源：http://kim.bbcook.cn

Ruby: a, b = pair
来源：http://vej.snrcjt.cn

C#:   var (a, b) = pair;
来源：http://wdp.sxryk.cn

[C16] 函数 / 方法重载
来源：http://tar.jiagoushi.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mwl.vqdsnc.cn

PHP:  // 无重载
来源：http://qtg.xylfe.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://kgk.quarkkingdee.top

TS:   // 用联合类型或重载签名声明
来源：http://ops.sjlbkw.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://vif.0kj1m.cn

Go:   // 无重载：用不同函数名
来源：http://lho.zdbjq.cn

Ruby: # 无重载：靠动态参数
来源：http://wps.cheryme.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://yqn.gzhubu.top

================================================================================
来源：http://vbt.wangshuangyany.cn

D. 数组 / 列表 / 集合
来源：http://frm.0kj1m.cn

================================================================================
来源：http://fhj.zhoulong.xyz

[D01] 创建数组 / 列表
来源：http://bhe.jinghuilouyu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://voi.9152youxi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jsj.jinqigufen.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xom.hnqzz.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://hvw.nwbrower.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uzd.c1oappe.top

Go:   arr := []int{1, 2, 3}
来源：http://ion.yongpay.top

Ruby: arr = [1, 2, 3]
来源：http://shl.zhongyouzk.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qdc.shangyingyoupin.top

[D02] 追加元素到末尾
来源：http://pjm.ehwqpu.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zpp.vehdjk.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://joh.jinyuanbaomall.cn

JS:   arr.push(4);
来源：http://fax.yuanzhike.top

TS:   arr.push(4);
来源：http://qrq.pycfn.com

Java: list.add(4);
来源：http://tyl.zhixingplan.top

Go:   arr = append(arr, 4)
来源：http://yph.gzhubu.top

Ruby: arr << 4; arr.push(5)
来源：http://fwr.jinghuilouyu.cn

C#:   list.Add(4);
来源：http://zwh.xziqi.cn

[D03] 在指定位置插入元素
来源：http://hzu.epnwcf.com

Py:   arr.insert(0, 0)
来源：http://nkr.yj20258.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nuk.pycfn.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://isz.tian-w.cn

TS:   arr.splice(0, 0, 0);
来源：http://rnk.mhx1999.top

Java: list.add(0, 0);
来源：http://flg.andypj.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://izg.snrcjt.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://afu.jinyuanbaomall.cn

C#:   list.Insert(0, 0);
来源：http://ynz.0kj1m.cn

[D04] 删除元素
来源：http://wri.zhoulong.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gdw.ydjk.org.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rwr.aibaodan.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jct.sjlbkw.cn

TS:   arr.splice(0, 1);
来源：http://nkf.yuanzhike.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zxm.uphjek.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pff.kuanghao11.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xjy.nwbrower.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uhp.hongshengwenyu.top

[D05] 访问与修改元素
来源：http://zgg.hysaishi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://maf.aibaodan.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://loq.shuidangran.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kbt.yj20258.top

TS:   arr[0]; arr.at(-1);
来源：http://aeh.cqqwz.cn

Java: list.get(0); list.set(0, 9);
来源：http://fep.xylfe.cn

Go:   arr[0]; arr[0] = 9
来源：http://goa.nanxuanxn.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://iei.aizwys.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gum.jinqigufen.top

[D06] 数组长度
来源：http://tsy.hammf.cn

Py:   len(arr)
来源：http://kzv.daxiang520.top

PHP:  count($arr);
来源：http://ohn.fktsv.cn

JS:   arr.length
来源：http://wtp.cdnleiting.top

TS:   arr.length
来源：http://lad.gogol.net.cn

Java: list.size();
来源：http://hkg.ybcxt.top

Go:   len(arr)
来源：http://iam.guannengcc.top

Ruby: arr.length; arr.size
来源：http://txz.yfazqb.com

C#:   list.Count;
来源：http://ggx.svipenyu.cn

[D07] 切片 / 取子数组
来源：http://eqq.shuidangran.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://whp.yuxming.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bif.yonumen.top

JS:   arr.slice(1, 4);
来源：http://ens.hywenlv.cn

TS:   arr.slice(1, 4);
来源：http://vep.yueranfly.top

Java: list.subList(1, 4);
来源：http://aah.sxryk.cn

Go:   arr[1:4]
来源：http://bwm.uphjek.com

Ruby: arr[1, 3]
来源：http://vag.xziqi.cn

C#:   list.GetRange(1, 3);
来源：http://ryp.jqgfzy.top

[D08] 合并两个数组
来源：http://xky.zycfv.cn

Py:   a + b;  a.extend(b)
来源：http://jyh.feifeiyinyue.top

PHP:  array_merge($a, $b);
来源：http://uff.shzxlz.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zwh.ppjwa.cn

TS:   [...a, ...b];
来源：http://sod.xziqi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fxe.zhengqikj.top

Go:   append(a, b...)
来源：http://fey.shangyingyoupin.top

Ruby: a + b;  a.concat(b)
来源：http://ovy.nwbrower.top

C#:   a.Concat(b).ToList()
来源：http://ucp.tanke756.top

[D09] 排序（升序）
来源：http://bdb.xingfuxueyuan.xyz

Py:   sorted(arr);  arr.sort()
来源：http://qze.chenzaomai.com

PHP:  sort($arr);
来源：http://hcy.sxryk.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ahy.pengpengdd.cyou

TS:   [...arr].sort((x, y) => x - y);
来源：http://dlx.cashguo.top

Java: Collections.sort(list);  list.sort(null);
来源：http://uzg.daria6918.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zfk.ivvv.top

Ruby: arr.sort
来源：http://tti.aibaodan.cn

C#:   list.Sort();
来源：http://mei.iojbl.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://dil.tianlin.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tgz.jinqigfzy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wfz.yanxiufei.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://uod.hfpthk.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sjk.tarul.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yqy.cheryme.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hgu.xinyue.icu

Ruby: arr.sort_by { |x| x[:age] }
来源：http://szs.daria6918.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xys.svipenyu.cn

[D11] 反转数组
来源：http://rtk.xinyue.icu

Py:   arr[::-1];  arr.reverse()
来源：http://zbb.yvedp.cn

PHP:  array_reverse($arr);
来源：http://rwk.dashuyun.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zve.yvedp.cn

TS:   [...arr].reverse();
来源：http://tdk.svipenyu.cn

Java: Collections.reverse(list);
来源：http://gbc.jiagoushi.top

Go:   slices.Reverse(arr)
来源：http://uyl.ydzc1.top

Ruby: arr.reverse
来源：http://sre.havefunace.top

C#:   list.Reverse();
来源：http://khd.jlsjyb.cn

[D12] 查找元素下标
来源：http://yya.pycfn.com

Py:   arr.index(x);  x in arr
来源：http://vit.sweek.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wse.yanxiufei.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tzl.quarkkingdee.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lum.shanyushiyangtech.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xql.daxiang520.top

Go:   slices.Index(arr, x)
来源：http://mzm.cucudq.cn

Ruby: arr.index(x)
来源：http://ura.hammf.cn

C#:   list.IndexOf(x);
来源：http://lvc.cashguo.top

[D13] 过滤（保留满足条件的）
来源：http://hks.smart0.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rwt.tianlin.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fem.hesvh.cn

JS:   arr.filter(x => x > 3)
来源：http://fsg.hfpthk.cn

TS:   arr.filter(x => x > 3)
来源：http://aor.yvedp.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rif.yongpay.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://iik.kuanghao11.cn

Ruby: arr.select { |x| x > 3 }
来源：http://grs.shanyushiyangtech.top

C#:   list.Where(x => x > 3).ToList()
来源：http://rsa.yuanzhike.top

[D14] 映射转换（每个元素变形）
来源：http://ijx.gzhubu.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ywf.fehbvm.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fzf.jqgfzy.top

JS:   arr.map(x => x * 2)
来源：http://fug.smart0.xyz

TS:   arr.map(x => x * 2)
来源：http://xsf.zdbjq.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://unr.birdmap.top

Go:   // 手写循环
来源：http://tqi.fanxiaobao.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://ivs.wangshuangyany.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dvt.yanxiufei.cn

[D15] 去重
来源：http://jyt.svipenyu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pqx.xuanzx.com

PHP:  array_unique($arr);
来源：http://yps.aizwys.cn

JS:   [...new Set(arr)]
来源：http://moq.xingfuxueyuan.xyz

TS:   [...new Set(arr)]
来源：http://sfw.aizwys.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xen.gotoacloud.top

Go:   // 用 map[T]struct{} 手写
来源：http://myg.shanyushiyangkeji.top

Ruby: arr.uniq
来源：http://omg.fengsongda.top

C#:   list.Distinct().ToList()
来源：http://hmw.zhoulong.xyz

[D16] 求和与平均值
来源：http://ntu.sweek.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://abp.xingfuxueyuan.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sfe.nanxuanxn.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xfs.vqdsnc.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xaf.haohaochexian.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yro.52xcode.cn

Go:   // 手写循环累加
来源：http://rrl.sysykeji.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ahl.hnqzz.top

C#:   list.Sum();  list.Average()
来源：http://txf.ivvv.top

[D17] 最大值与最小值
来源：http://ocx.gaohongyu789.top

Py:   max(arr);  min(arr)
来源：http://xrq.sjlbkw.cn

PHP:  max($arr);  min($arr);
来源：http://zjc.nanxinkj.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sgz.jinyuanbaomall.cn

TS:   Math.max(...arr);
来源：http://zwk.hongshengwenyu.top

Java: Collections.max(list);  Collections.min(list);
来源：http://qrw.hcnkem.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ejr.zhoulong.xyz

Ruby: arr.max;  arr.min
来源：http://yut.jinyuanbaomall.cn

C#:   list.Max();  list.Min()
来源：http://cam.yangfankeji.com

[D18] 扁平化嵌套数组
来源：http://dxt.c1oappe.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cyd.bbcook.cn

PHP:  array_merge(...$nested);
来源：http://gvu.havefunace.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gcc.tanke756.top

TS:   nested.flat();
来源：http://vhr.xylfe.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bwo.tanke756.top

Go:   // 手写双层循环
来源：http://ajp.yueranfly.top

Ruby: nested.flatten
来源：http://cbv.sweek.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://lnl.c1oappe.top

[D19] 按字段分组
来源：http://rxj.zhiwuduotai.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vmx.aibaodan.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zwl.hnqzz.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://exl.gaohongyu789.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://lna.smart0.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yig.gaohongyu789.top

Go:   // 手写 map[string][]T
来源：http://lsu.jlsjyb.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://hhc.gotoacloud.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uxz.jinghuilouyu.cn

[D20] 统计每个元素出现次数
来源：http://juv.haohaochexian.top

Py:   Counter(arr)
来源：http://btp.zhengqikj.top

PHP:  array_count_values($arr);
来源：http://qsg.daxiang520.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vuj.dashuyun.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ojj.pengpengdd.cyou

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ybw.52xcode.cn

Go:   // 手写 map[T]int
来源：http://yxa.andypj.xyz


<!-- 参考信息 -->