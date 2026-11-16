代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://emz.vehdjk.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://efb.zdqjudy.top

[C04] 命名参数 / 关键字参数
来源：http://wlg.hysaishi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jqj.tian-w.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qss.sweek.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vac.shanyushiyangtech.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qlv.jinghuilouyu.cn

Java: // 无：用 Builder 模式或 record
来源：http://hgq.aizwys.cn

Go:   // 无：用配置结构体参数
来源：http://neo.tarul.cn

Ruby: f(a: 1, b: 2)
来源：http://tkz.zhoulong.xyz

C#:   f(a: 1, b: 2)
来源：http://fqa.yj20258.top

[C05] 返回多个值
来源：http://wkh.shanyushiyangkeji.top

Py:   return a, b
来源：http://jge.wangdashe.top

PHP:  return [$a, $b];
来源：http://nyh.sxryk.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://cot.havefunace.top

TS:   return { a, b };
来源：http://lhe.mhx1999.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ddb.hysaishi.cn

Go:   return a, b
来源：http://jqb.jyoumei.cn

Ruby: return a, b
来源：http://jaw.gaohongyu789.top

C#:   return (a, b);              // ValueTuple
来源：http://osi.yuanzhike.top

[C06] 匿名函数 / lambda
来源：http://wid.haohaochexian.top

Py:   square = lambda x: x * x
来源：http://ero.yongpay.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ulj.mhx1999.top

JS:   const square = x => x * x;
来源：http://qvy.cdnleiting.top

TS:   const square = (x: number): number => x * x;
来源：http://oyy.sweek.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kir.gogol.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://sln.guowangkeji.top

Ruby: square = ->(x) { x * x }
来源：http://lsu.yuanzhike.top

C#:   Func<int, int> square = x => x * x;
来源：http://vsl.smart0.xyz

[C07] 把函数作为参数传入
来源：http://uff.jlsjyb.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://clu.hammf.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ork.ppjwa.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://szd.zdqjudy.top

TS:   arr.map(String)
来源：http://bhi.yvedp.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xnr.feifeiyinyue.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kyl.epnwcf.com

Ruby: arr.map(&:upcase)
来源：http://xdg.aizwys.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qex.vqdsnc.cn

[C08] 闭包
来源：http://ekf.zhoulong.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vim.jinqigfzy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nhj.zhongyouzk.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vvk.hysaishi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yow.guowangkeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://quq.feifeiyinyue.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://joi.jinghuilouyu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://quy.quarkkingdee.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ont.snrcjt.cn

[C09] 递归
来源：http://yga.chenjidiqi.icu

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vgo.xuanzx.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://eji.fehbvm.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fzv.birdmap.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yle.xuetiantiany.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sjj.52xcode.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pis.xziqi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bsr.cheryme.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fsr.jinqigfzy.top

[C10] 变量作用域
来源：http://jvk.316326.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rsz.ydzc1.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jkw.sjlbkw.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lhb.daria6918.cn

TS:   同 JS
来源：http://aug.316326.xyz

Java: 方法内为块级作用域
来源：http://epf.hesvh.cn

Go:   花括号块级作用域
来源：http://tdj.yongpay.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wed.tanke756.top

C#:   块级作用域
来源：http://sxg.yfazqb.com

[C11] 模块导入与导出
来源：http://abc.zdqjudy.top

Py:   from module import func
来源：http://ilv.ydzc1.top

PHP:  require "file.php";  或 use App\Service;
来源：http://rxo.yuanzhike.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://kkj.xziqi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hyn.sweek.top

Java: import java.util.List;
来源：http://cjy.tianlin.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kcb.daxiang520.top

Ruby: require "json"; require_relative "./util"
来源：http://egx.yonumen.top

C#:   using System.Text;
来源：http://ubp.hcnkem.com

[C12] 立即执行函数 IIFE
来源：http://epa.chenzaomai.com

Py:   (lambda: print("run"))()
来源：http://jqr.meibo888.top

PHP:  (function () { echo "run"; })();
来源：http://tun.zhijiandao.cn

JS:   (() => { console.log("run"); })();
来源：http://nzq.jinyuanbaomall.cn

TS:   (() => { console.log("run"); })();
来源：http://ywl.chenjidiqi.icu

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tcy.svipenyu.cn

Go:   func() { fmt.Println("run") }()
来源：http://nfo.dianchejie.cn

Ruby: -> { puts "run" }.call
来源：http://oky.birdmap.top

C#:   // 无 IIFE：用静态构造函数
来源：http://dcb.nanxinkj.top

[C13] 类型声明 / 类型注解
来源：http://gcr.ywan-chungtsiang.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hrc.uphjek.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://grs.guowangkeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://spu.hnqzz.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ram.cheryme.top

Java: int add(int a, int b) { return a + b; }
来源：http://ifh.smart0.xyz

Go:   func add(a, b int) int
来源：http://dso.jqgufenzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wkr.havefunace.top

C#:   int Add(int a, int b) => a + b;
来源：http://kjh.hfpthk.cn

[C14] 泛型函数
来源：http://cza.xinyue.icu

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://enj.9152youxi.cn

PHP:  // 无泛型
来源：http://zbr.guannengcc.top

JS:   // 无泛型
来源：http://jkw.ydjk.org.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://iqn.hcnkem.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cnr.tarul.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://eau.feifeiyinyue.top

Ruby: # 无泛型
来源：http://jju.hcnkem.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://iwy.vqdsnc.cn

[C15] 解构 / 展开参数
来源：http://ezo.ivvv.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lic.zhixingplan.top

PHP:  [$a, $b] = $pair;
来源：http://wrp.ydjk.org.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ldf.zhijiandao.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ezj.zycfv.cn

Java: // 无解构
来源：http://wbm.shangyingyoupin.top

Go:   // 无解构
来源：http://jfo.jiagoushi.top

Ruby: a, b = pair
来源：http://yvt.birdmap.top

C#:   var (a, b) = pair;
来源：http://cgh.jqgfzy.top

[C16] 函数 / 方法重载
来源：http://xxu.xuetiantiany.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ufp.tanke756.top

PHP:  // 无重载
来源：http://soz.smart0.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://usr.hesvh.cn

TS:   // 用联合类型或重载签名声明
来源：http://lnl.jianghu66.top

Java: void f(int a) {}  void f(String a) {}
来源：http://hzl.wangdashe.top

Go:   // 无重载：用不同函数名
来源：http://sjv.jiagoushi.top

Ruby: # 无重载：靠动态参数
来源：http://toi.yfazqb.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://vtb.hywenlv.cn

================================================================================
来源：http://qwf.mhx1999.top

D. 数组 / 列表 / 集合
来源：http://tdc.xuetiantiany.cn

================================================================================
来源：http://xkg.hnqzz.top

[D01] 创建数组 / 列表
来源：http://phw.316326.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://qsy.tanke756.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rul.hywenlv.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://czc.shuidangran.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ttq.gotoacloud.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://quj.smart0.xyz

Go:   arr := []int{1, 2, 3}
来源：http://nfw.vehdjk.com

Ruby: arr = [1, 2, 3]
来源：http://pzt.52xcode.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fjv.ydjk.org.cn

[D02] 追加元素到末尾
来源：http://ozp.yongpay.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://trk.sxryk.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mzf.ppjwa.cn

JS:   arr.push(4);
来源：http://bmf.jiagoushi.top

TS:   arr.push(4);
来源：http://pvh.xuanzx.com

Java: list.add(4);
来源：http://xou.yanxiufei.cn

Go:   arr = append(arr, 4)
来源：http://hic.jianghu66.top

Ruby: arr << 4; arr.push(5)
来源：http://ahx.fehbvm.com

C#:   list.Add(4);
来源：http://sah.epnwcf.com

[D03] 在指定位置插入元素
来源：http://gwi.zhiwuduotai.top

Py:   arr.insert(0, 0)
来源：http://ncy.zhengqikj.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cwf.cheryme.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xfc.jinghuilouyu.cn

TS:   arr.splice(0, 0, 0);
来源：http://pqv.zdqjudy.top

Java: list.add(0, 0);
来源：http://hkz.aizwys.cn

Go:   arr = append([]int{0}, arr...)
来源：http://oie.ywan-chungtsiang.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zcf.aizwys.cn

C#:   list.Insert(0, 0);
来源：http://dqq.uphjek.com

[D04] 删除元素
来源：http://kxe.ybcxt.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ped.316326.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nsv.xylfe.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mpb.zhiwuduotai.top

TS:   arr.splice(0, 1);
来源：http://vsf.zhongyouzk.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hii.chenzaomai.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dwo.feifeiyinyue.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xim.wangshuangyany.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dzn.fehbvm.com

[D05] 访问与修改元素
来源：http://emb.yongpay.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sic.daxiang520.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ihw.fktsv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ryd.pycfn.com

TS:   arr[0]; arr.at(-1);
来源：http://zkd.sweek.top

Java: list.get(0); list.set(0, 9);
来源：http://cxj.mhx1999.top

Go:   arr[0]; arr[0] = 9
来源：http://ugj.xuetiantiany.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://eww.c1oappe.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lcj.daxiang520.top

[D06] 数组长度
来源：http://jcy.hesvh.cn

Py:   len(arr)
来源：http://ctw.chenzaomai.com

PHP:  count($arr);
来源：http://mkl.hnxiangtu.top

JS:   arr.length
来源：http://pva.shanyushiyangkeji.top

TS:   arr.length
来源：http://ugm.yanxiufei.cn

Java: list.size();
来源：http://tsl.jinyuanbaomall.cn

Go:   len(arr)
来源：http://vmm.hongshengwenyu.top

Ruby: arr.length; arr.size
来源：http://qcn.sysykeji.top

C#:   list.Count;
来源：http://yjy.xziqi.cn

[D07] 切片 / 取子数组
来源：http://ohr.jinqigfzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gyg.c1oappe.top

PHP:  array_slice($arr, 1, 3);
来源：http://sua.tanke756.top

JS:   arr.slice(1, 4);
来源：http://hsq.zhixingplan.top

TS:   arr.slice(1, 4);
来源：http://ufq.sysykeji.top

Java: list.subList(1, 4);
来源：http://dla.hcnkem.com

Go:   arr[1:4]
来源：http://yib.yj20258.top

Ruby: arr[1, 3]
来源：http://hsx.shanyushiyangtech.top

C#:   list.GetRange(1, 3);
来源：http://sng.yuanzhike.top

[D08] 合并两个数组
来源：http://zxr.ppjwa.cn

Py:   a + b;  a.extend(b)
来源：http://sod.yj202588.top

PHP:  array_merge($a, $b);
来源：http://amq.xylfe.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://faz.52xcode.cn

TS:   [...a, ...b];
来源：http://etd.zhixingplan.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bmu.pengpengdd.cyou

Go:   append(a, b...)
来源：http://nem.fengsongda.top

Ruby: a + b;  a.concat(b)
来源：http://eqc.ehwqpu.com

C#:   a.Concat(b).ToList()
来源：http://hca.yvedp.cn

[D09] 排序（升序）
来源：http://xbv.xinyue.icu

Py:   sorted(arr);  arr.sort()
来源：http://zef.gaohongyu789.top

PHP:  sort($arr);
来源：http://vtg.nanxinkj.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://iim.cheryme.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://dtt.kuanghao11.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rgv.ctjpmb.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wpu.jyoumei.cn

Ruby: arr.sort
来源：http://ndd.ctjpmb.com

C#:   list.Sort();
来源：http://aiw.c1oappe.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://rrj.havefunace.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dcr.iojbl.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pdw.sjlbkw.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cbd.hnxiangtu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sub.kuanghao11.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zwa.bbcook.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nyz.gogol.net.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dbe.yuanzhike.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uok.ydjk.org.cn

[D11] 反转数组
来源：http://zwk.yj20258.top

Py:   arr[::-1];  arr.reverse()
来源：http://kia.shangyingyoupin.top

PHP:  array_reverse($arr);
来源：http://xvo.hnxiangtu.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mhe.bbcook.cn

TS:   [...arr].reverse();
来源：http://wtj.shanyushiyangkeji.top

Java: Collections.reverse(list);
来源：http://rbs.zdbjq.cn

Go:   slices.Reverse(arr)
来源：http://ivs.fengsongda.top

Ruby: arr.reverse
来源：http://wet.aibaodan.cn

C#:   list.Reverse();
来源：http://wno.hywenlv.cn

[D12] 查找元素下标
来源：http://wyr.mhx1999.top

Py:   arr.index(x);  x in arr
来源：http://zrb.52xcode.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tas.hesvh.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jtm.yongpay.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://owp.shuidangran.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wwf.c1oappe.top

Go:   slices.Index(arr, x)
来源：http://oig.zhoulong.xyz

Ruby: arr.index(x)
来源：http://fzc.zdqjudy.top

C#:   list.IndexOf(x);
来源：http://ier.ppjwa.cn

[D13] 过滤（保留满足条件的）
来源：http://muk.yfazqb.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ugi.yuanzhike.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vco.ppjwa.cn

JS:   arr.filter(x => x > 3)
来源：http://grc.haohaochexian.top

TS:   arr.filter(x => x > 3)
来源：http://rel.tarul.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yit.fktsv.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://chc.sjlbkw.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ecq.ywan-chungtsiang.top

C#:   list.Where(x => x > 3).ToList()
来源：http://uwx.yvedp.cn

[D14] 映射转换（每个元素变形）
来源：http://ilj.hywenlv.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bio.mhx1999.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wpz.fktsv.cn

JS:   arr.map(x => x * 2)
来源：http://bkq.fzhhl.top

TS:   arr.map(x => x * 2)
来源：http://anr.zhixingplan.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://fnp.yj20258888.top

Go:   // 手写循环
来源：http://spu.redwolf501.top

Ruby: arr.map { |x| x * 2 }
来源：http://rli.kuanghao11.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bob.xuanzx.com

[D15] 去重
来源：http://hgz.ydjk.org.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zcx.sjlbkw.cn

PHP:  array_unique($arr);
来源：http://zca.hysaishi.cn

JS:   [...new Set(arr)]
来源：http://yde.hysaishi.cn

TS:   [...new Set(arr)]
来源：http://bkk.vqdsnc.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rpl.meibo888.top

Go:   // 用 map[T]struct{} 手写
来源：http://wlt.tanke756.top

Ruby: arr.uniq
来源：http://voh.havefunace.top

C#:   list.Distinct().ToList()
来源：http://rdo.zhoulong.xyz

[D16] 求和与平均值
来源：http://qde.hongshengwenyu.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rzd.tian-w.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nwe.cdnleiting.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wgg.c1oappe.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xpx.zhongyouzk.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ved.yuxming.cn

Go:   // 手写循环累加
来源：http://gje.cashguo.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uee.hongshengwenyu.top

C#:   list.Sum();  list.Average()
来源：http://mss.sweek.top

[D17] 最大值与最小值
来源：http://gwq.fanxiaobao.xyz

Py:   max(arr);  min(arr)
来源：http://fpf.yj20258888.top

PHP:  max($arr);  min($arr);
来源：http://nix.wangdashe.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vnp.hnqzz.top

TS:   Math.max(...arr);
来源：http://lfn.zhijiandao.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gyb.jlsjyb.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pcw.chenjidiqi.icu

Ruby: arr.max;  arr.min
来源：http://tfx.chenjidiqi.icu

C#:   list.Max();  list.Min()
来源：http://zkd.tarul.cn

[D18] 扁平化嵌套数组
来源：http://awn.meibo888.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gxv.jinyuanbaomall.cn

PHP:  array_merge(...$nested);
来源：http://ysc.andypj.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://urf.xingfuxueyuan.xyz

TS:   nested.flat();
来源：http://lov.9152youxi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://chz.jqgfzy.top

Go:   // 手写双层循环
来源：http://fie.xuanzx.com

Ruby: nested.flatten
来源：http://scg.jinyuanbaomall.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://cry.ydzc1.top

[D19] 按字段分组
来源：http://gwj.snrcjt.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zjh.tarul.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rrv.tarul.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://iqf.ybcxt.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://hgz.xinyue.icu

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vhn.xuanzx.com

Go:   // 手写 map[string][]T
来源：http://uau.chenlongwang.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ces.yueranfly.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ukp.fengsongda.top

[D20] 统计每个元素出现次数
来源：http://pnz.fanxiaobao.xyz

Py:   Counter(arr)
来源：http://xvk.xylfe.cn

PHP:  array_count_values($arr);
来源：http://mvj.sufxvd.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gku.c1oappe.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zcg.xinyue.icu

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ull.sweek.top

Go:   // 手写 map[T]int
来源：http://bgt.zycfv.cn


<!-- 参考信息 -->