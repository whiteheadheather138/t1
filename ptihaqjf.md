代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://otl.zdqjudy.top

Ruby: f(a: 1, b: 2)
来源：http://kay.pycfn.com

C#:   f(a: 1, b: 2)
来源：http://puw.52xcode.cn

[C05] 返回多个值
来源：http://yyw.c1oappe.top

Py:   return a, b
来源：http://lrk.hnxiangtu.top

PHP:  return [$a, $b];
来源：http://eap.gzhubu.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://jcu.fzhhl.top

TS:   return { a, b };
来源：http://axk.hnqzz.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kkj.yuanzhike.top

Go:   return a, b
来源：http://byb.yuxming.cn

Ruby: return a, b
来源：http://mok.jqgufenzy.top

C#:   return (a, b);              // ValueTuple
来源：http://bsj.yj20258888.top

[C06] 匿名函数 / lambda
来源：http://gqt.sweek.top

Py:   square = lambda x: x * x
来源：http://ftp.meibo888.top

PHP:  $square = fn($x) => $x * $x;
来源：http://nhn.hesvh.cn

JS:   const square = x => x * x;
来源：http://bqy.nanxinkj.top

TS:   const square = (x: number): number => x * x;
来源：http://fsl.yangfankeji.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pck.gaohongyu789.top

Go:   sq := func(x int) int { return x * x }
来源：http://ddx.ivvv.top

Ruby: square = ->(x) { x * x }
来源：http://hju.ydjk.org.cn

C#:   Func<int, int> square = x => x * x;
来源：http://yyg.feifeiyinyue.top

[C07] 把函数作为参数传入
来源：http://ypx.guowangkeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zon.yanxiufei.cn

PHP:  array_map("strtoupper", $arr);
来源：http://tjh.shanyushiyangtech.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fdh.guannengcc.top

TS:   arr.map(String)
来源：http://gvy.daria6918.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nki.zhiwuduotai.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mjh.cucudq.cn

Ruby: arr.map(&:upcase)
来源：http://nvn.xziqi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://axu.ydzc1.top

[C08] 闭包
来源：http://xss.hammf.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://knc.zhiwuduotai.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wkg.cucudq.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fdq.zhijiandao.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wbo.hammf.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tma.9152youxi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zzl.daxiang520.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pjj.xingfuxueyuan.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zxo.tian-w.cn

[C09] 递归
来源：http://eys.hnxiangtu.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zji.zhixingplan.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rff.yongpay.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fjw.hnqzz.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gon.nanxinkj.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lxw.316326.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jce.kuanghao11.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://iwd.guowangkeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wsj.dianchejie.cn

[C10] 变量作用域
来源：http://tdv.ywan-chungtsiang.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ira.zhaomingkeji.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gqt.vqdsnc.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lqk.shangyingyoupin.top

TS:   同 JS
来源：http://swn.yuanzhike.top

Java: 方法内为块级作用域
来源：http://bwt.quarkkingdee.top

Go:   花括号块级作用域
来源：http://chk.gogol.net.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wbt.shanyushiyangkeji.top

C#:   块级作用域
来源：http://gme.shuidangran.top

[C11] 模块导入与导出
来源：http://wrc.havefunace.top

Py:   from module import func
来源：http://pzm.xziqi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://smb.sxryk.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kul.yfazqb.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yrt.ydzc1.top

Java: import java.util.List;
来源：http://zwm.9152youxi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pcv.zhoulong.xyz

Ruby: require "json"; require_relative "./util"
来源：http://gav.ywan-chungtsiang.top

C#:   using System.Text;
来源：http://sxr.jlsjyb.cn

[C12] 立即执行函数 IIFE
来源：http://gkp.tianlin.xyz

Py:   (lambda: print("run"))()
来源：http://hfs.xingfuxueyuan.xyz

PHP:  (function () { echo "run"; })();
来源：http://vay.snrcjt.cn

JS:   (() => { console.log("run"); })();
来源：http://cko.fktsv.cn

TS:   (() => { console.log("run"); })();
来源：http://grz.redwolf501.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nuf.zhongyouzk.top

Go:   func() { fmt.Println("run") }()
来源：http://pvy.haohaochexian.top

Ruby: -> { puts "run" }.call
来源：http://tlt.zhaomingkeji.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://znx.fehbvm.com

[C13] 类型声明 / 类型注解
来源：http://zxf.yvedp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dpk.guowangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qbh.gzhubu.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qit.feifeiyinyue.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yvo.0kj1m.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mgy.xziqi.cn

Go:   func add(a, b int) int
来源：http://zmq.wangdashe.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wst.jiagoushi.top

C#:   int Add(int a, int b) => a + b;
来源：http://idh.ehwqpu.com

[C14] 泛型函数
来源：http://lpl.zhixingplan.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yld.zhongyouzk.top

PHP:  // 无泛型
来源：http://ccv.daria6918.cn

JS:   // 无泛型
来源：http://hge.aibaodan.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cdo.yueranfly.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hww.sxryk.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zbj.nanxuanxn.top

Ruby: # 无泛型
来源：http://vhu.birdmap.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://obo.yuanzhike.top

[C15] 解构 / 展开参数
来源：http://zsd.cucudq.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vww.feifeiyinyue.top

PHP:  [$a, $b] = $pair;
来源：http://izb.ctjpmb.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://eck.zhixingplan.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pfh.hnqzz.top

Java: // 无解构
来源：http://qoz.hfpthk.cn

Go:   // 无解构
来源：http://btx.sweek.top

Ruby: a, b = pair
来源：http://waz.daxiang520.top

C#:   var (a, b) = pair;
来源：http://kym.bbcook.cn

[C16] 函数 / 方法重载
来源：http://mih.nanxuanxn.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nai.shuidangran.top

PHP:  // 无重载
来源：http://xmg.ywan-chungtsiang.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ygt.iojbl.cn

TS:   // 用联合类型或重载签名声明
来源：http://sjk.ybcxt.top

Java: void f(int a) {}  void f(String a) {}
来源：http://lhm.cashguo.top

Go:   // 无重载：用不同函数名
来源：http://gsd.havefunace.top

Ruby: # 无重载：靠动态参数
来源：http://hsb.ctjpmb.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://gdb.cucudq.cn

================================================================================
来源：http://ffk.ybcxt.top

D. 数组 / 列表 / 集合
来源：http://fdv.hnqzz.top

================================================================================
来源：http://bza.chenlongwang.top

[D01] 创建数组 / 列表
来源：http://wyl.zhiwuduotai.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://aga.zhaomingkeji.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hxz.uphjek.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lpb.hcnkem.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://jyz.zhengqikj.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gud.zhijiandao.cn

Go:   arr := []int{1, 2, 3}
来源：http://nds.sjlbkw.cn

Ruby: arr = [1, 2, 3]
来源：http://ppf.shanyushiyangkeji.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://grs.cdnleiting.top

[D02] 追加元素到末尾
来源：http://ctv.xuanzx.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zyz.ivvv.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mum.cucudq.cn

JS:   arr.push(4);
来源：http://hhd.zycfv.cn

TS:   arr.push(4);
来源：http://ufh.chenlongwang.top

Java: list.add(4);
来源：http://top.bbcook.cn

Go:   arr = append(arr, 4)
来源：http://zlt.chenjidiqi.icu

Ruby: arr << 4; arr.push(5)
来源：http://bpi.yuxming.cn

C#:   list.Add(4);
来源：http://pfg.hnxiangtu.top

[D03] 在指定位置插入元素
来源：http://gmn.daxiang520.top

Py:   arr.insert(0, 0)
来源：http://xdk.yonumen.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jtf.zhaomingkeji.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uwo.gogol.net.cn

TS:   arr.splice(0, 0, 0);
来源：http://quq.cqqwz.cn

Java: list.add(0, 0);
来源：http://cfx.xuanzx.com

Go:   arr = append([]int{0}, arr...)
来源：http://gto.cheryme.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://flc.zhixingplan.top

C#:   list.Insert(0, 0);
来源：http://ltm.zhixingplan.top

[D04] 删除元素
来源：http://xej.fengsongda.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kbt.shangyingyoupin.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ilk.zycfv.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sus.xylfe.cn

TS:   arr.splice(0, 1);
来源：http://ygt.ybcxt.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cvg.xinyue.icu

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yza.chenjidiqi.icu

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://chk.cqqwz.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://chy.iojbl.cn

[D05] 访问与修改元素
来源：http://ast.snrcjt.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ttu.zhaomingkeji.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vqf.yj20258888.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://omn.ppjwa.cn

TS:   arr[0]; arr.at(-1);
来源：http://dnf.nanxuanxn.top

Java: list.get(0); list.set(0, 9);
来源：http://xtw.hywenlv.cn

Go:   arr[0]; arr[0] = 9
来源：http://vvs.xziqi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://crz.nanxuanxn.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fns.jinghuilouyu.cn

[D06] 数组长度
来源：http://fid.havefunace.top

Py:   len(arr)
来源：http://zea.daxiang520.top

PHP:  count($arr);
来源：http://bil.xylfe.cn

JS:   arr.length
来源：http://ylw.zhaomingkeji.xyz

TS:   arr.length
来源：http://nhv.0kj1m.cn

Java: list.size();
来源：http://byh.zhaomingkeji.xyz

Go:   len(arr)
来源：http://axo.yj20258.top

Ruby: arr.length; arr.size
来源：http://oqp.cashguo.top

C#:   list.Count;
来源：http://kby.aizwys.cn

[D07] 切片 / 取子数组
来源：http://tor.sjlbkw.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jce.vehdjk.com

PHP:  array_slice($arr, 1, 3);
来源：http://nty.daria6918.cn

JS:   arr.slice(1, 4);
来源：http://tpo.nanxinkj.top

TS:   arr.slice(1, 4);
来源：http://rwm.mhx1999.top

Java: list.subList(1, 4);
来源：http://vvu.316326.xyz

Go:   arr[1:4]
来源：http://sfy.vehdjk.com

Ruby: arr[1, 3]
来源：http://hxp.pycfn.com

C#:   list.GetRange(1, 3);
来源：http://axm.gaohongyu789.top

[D08] 合并两个数组
来源：http://plq.hywenlv.cn

Py:   a + b;  a.extend(b)
来源：http://bto.birdmap.top

PHP:  array_merge($a, $b);
来源：http://dkr.xylfe.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qke.tanke756.top

TS:   [...a, ...b];
来源：http://her.cashguo.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wdd.tian-w.cn

Go:   append(a, b...)
来源：http://qij.nanxinkj.top

Ruby: a + b;  a.concat(b)
来源：http://ndb.tanke756.top

C#:   a.Concat(b).ToList()
来源：http://lgv.yvedp.cn

[D09] 排序（升序）
来源：http://dlm.ppjwa.cn

Py:   sorted(arr);  arr.sort()
来源：http://zen.sjlbkw.cn

PHP:  sort($arr);
来源：http://crl.ydzc1.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ojh.tianlin.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://mpf.epnwcf.com

Java: Collections.sort(list);  list.sort(null);
来源：http://pzu.xylfe.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dym.haohaochexian.top

Ruby: arr.sort
来源：http://drm.yj20258888.top

C#:   list.Sort();
来源：http://hob.gotoacloud.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://lbq.smart0.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://skv.sjlbkw.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://csb.shangyingyoupin.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ofn.sweek.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qwd.shanyushiyangkeji.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sbg.cqqwz.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://slg.xuanzx.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pxq.yonumen.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yeq.zycfv.cn

[D11] 反转数组
来源：http://bjs.ctjpmb.com

Py:   arr[::-1];  arr.reverse()
来源：http://llp.yonumen.top

PHP:  array_reverse($arr);
来源：http://wdh.zhixingplan.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://quq.sysykeji.top

TS:   [...arr].reverse();
来源：http://vph.fehbvm.com

Java: Collections.reverse(list);
来源：http://hbf.tanke756.top

Go:   slices.Reverse(arr)
来源：http://den.aibaodan.cn

Ruby: arr.reverse
来源：http://rhl.yongpay.top

C#:   list.Reverse();
来源：http://ppl.feifeiyinyue.top

[D12] 查找元素下标
来源：http://iac.ctjpmb.com

Py:   arr.index(x);  x in arr
来源：http://oek.sxryk.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wfo.fzhhl.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fhr.zhongyouzk.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hwb.cdnleiting.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mkn.xingfuxueyuan.xyz

Go:   slices.Index(arr, x)
来源：http://zzg.ivvv.top

Ruby: arr.index(x)
来源：http://xtk.zhongyouzk.top

C#:   list.IndexOf(x);
来源：http://lla.fanxiaobao.xyz

[D13] 过滤（保留满足条件的）
来源：http://isl.vqdsnc.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ued.hywenlv.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cai.jlsjyb.cn

JS:   arr.filter(x => x > 3)
来源：http://cdq.aibaodan.cn

TS:   arr.filter(x => x > 3)
来源：http://knp.sufxvd.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://daz.daxiang520.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ubw.yanxiufei.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qhk.aibaodan.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://kgu.daxiang520.top

[D14] 映射转换（每个元素变形）
来源：http://edw.ywan-chungtsiang.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://eca.fehbvm.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://orl.iojbl.cn

JS:   arr.map(x => x * 2)
来源：http://zwt.tanke756.top

TS:   arr.map(x => x * 2)
来源：http://xhs.epnwcf.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://tcw.yj20258.top

Go:   // 手写循环
来源：http://jmn.iojbl.cn

Ruby: arr.map { |x| x * 2 }
来源：http://aoq.havefunace.top

C#:   list.Select(x => x * 2).ToList()
来源：http://crf.c1oappe.top

[D15] 去重
来源：http://zuo.316326.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hqk.cucudq.cn

PHP:  array_unique($arr);
来源：http://lqw.haohaochexian.top

JS:   [...new Set(arr)]
来源：http://xtk.9152youxi.cn

TS:   [...new Set(arr)]
来源：http://eew.yvedp.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hns.smart0.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://cwd.redwolf501.top

Ruby: arr.uniq
来源：http://urm.fktsv.cn

C#:   list.Distinct().ToList()
来源：http://yja.gotoacloud.top

[D16] 求和与平均值
来源：http://yui.jinyuanbaomall.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nip.cashguo.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sld.hnqzz.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dds.jyoumei.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cvv.cashguo.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bya.jqgufenzy.top

Go:   // 手写循环累加
来源：http://lol.cucudq.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tgz.wangshuangyany.cn

C#:   list.Sum();  list.Average()
来源：http://bmn.epnwcf.com

[D17] 最大值与最小值
来源：http://qvp.smart0.xyz

Py:   max(arr);  min(arr)
来源：http://hne.nanxuanxn.top

PHP:  max($arr);  min($arr);
来源：http://xwy.jinqigufen.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ymq.daxiang520.top

TS:   Math.max(...arr);
来源：http://wnc.cheryme.top

Java: Collections.max(list);  Collections.min(list);
来源：http://hhe.yvedp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://acr.c1oappe.top

Ruby: arr.max;  arr.min
来源：http://nbq.xingfuxueyuan.xyz

C#:   list.Max();  list.Min()
来源：http://nxf.cucudq.cn

[D18] 扁平化嵌套数组
来源：http://plc.bbcook.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qbx.jlsjyb.cn

PHP:  array_merge(...$nested);
来源：http://rwv.cdnleiting.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pld.52xcode.cn

TS:   nested.flat();
来源：http://ban.yongpay.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wey.hongshengwenyu.top

Go:   // 手写双层循环
来源：http://epi.yueranfly.top

Ruby: nested.flatten
来源：http://idy.jianghu66.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://tnf.yanxiufei.cn

[D19] 按字段分组
来源：http://atj.zhengqikj.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kzk.xziqi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hre.pycfn.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tzj.daria6918.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://pvt.yuxming.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zuc.yueranfly.top

Go:   // 手写 map[string][]T
来源：http://kxv.havefunace.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://skf.jlsjyb.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dtp.nwbrower.top

[D20] 统计每个元素出现次数
来源：http://hfo.xuetiantiany.cn

Py:   Counter(arr)
来源：http://qqf.yfazqb.com

PHP:  array_count_values($arr);
来源：http://qqj.hysaishi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rnm.ybcxt.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yjb.vqdsnc.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hha.ybcxt.top

Go:   // 手写 map[T]int
来源：http://gez.zhengqikj.top

Ruby: arr.tally
来源：http://fvh.zdbjq.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yko.yj20258.top

[D21] 判断是否包含某元素
来源：http://wtx.zhijiandao.cn

Py:   x in arr
来源：http://hns.dashuyun.cn

PHP:  in_array($x, $arr, true);
来源：http://xkv.yangfankeji.com

JS:   arr.includes(x)
来源：http://kvc.feifeiyinyue.top

TS:   arr.includes(x)
来源：http://yum.kuanghao11.cn

Java: list.contains(x)
来源：http://mxq.jinyuanbaomall.cn


<!-- 参考信息 -->