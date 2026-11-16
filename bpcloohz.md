代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rww.svipenyu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yxt.mhx1999.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xqf.pengpengdd.cyou

Java: // 无：用 Builder 模式或 record
来源：http://qzm.ctjpmb.com

Go:   // 无：用配置结构体参数
来源：http://hay.sysykeji.top

Ruby: f(a: 1, b: 2)
来源：http://egy.snrcjt.cn

C#:   f(a: 1, b: 2)
来源：http://kob.hcnkem.com

[C05] 返回多个值
来源：http://cqg.kuanghao11.cn

Py:   return a, b
来源：http://vki.shzxlz.cn

PHP:  return [$a, $b];
来源：http://odc.cashguo.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://qrm.shuidangran.top

TS:   return { a, b };
来源：http://mcz.quarkkingdee.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bvh.dashuyun.cn

Go:   return a, b
来源：http://gzp.yuxming.cn

Ruby: return a, b
来源：http://hqz.gaohongyu789.top

C#:   return (a, b);              // ValueTuple
来源：http://xwx.jinqigufen.top

[C06] 匿名函数 / lambda
来源：http://mih.ydjk.org.cn

Py:   square = lambda x: x * x
来源：http://tfe.zdqjudy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ovv.nanxuanxn.top

JS:   const square = x => x * x;
来源：http://had.wangshuangyany.cn

TS:   const square = (x: number): number => x * x;
来源：http://rtj.wangdashe.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://okf.jiagoushi.top

Go:   sq := func(x int) int { return x * x }
来源：http://edd.ivvv.top

Ruby: square = ->(x) { x * x }
来源：http://tmk.hcnkem.com

C#:   Func<int, int> square = x => x * x;
来源：http://kkg.cdnleiting.top

[C07] 把函数作为参数传入
来源：http://mca.ywan-chungtsiang.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yrt.chenlongwang.top

PHP:  array_map("strtoupper", $arr);
来源：http://ene.cheryme.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ngw.kuanghao11.cn

TS:   arr.map(String)
来源：http://qst.quarkkingdee.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dcb.daxiang520.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xiq.jianghu66.top

Ruby: arr.map(&:upcase)
来源：http://qeh.cashguo.top

C#:   arr.Select(s => s.ToUpper())
来源：http://yyw.nwbrower.top

[C08] 闭包
来源：http://gai.yj20258888.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xcw.yj202588.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qep.jinghuilouyu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mph.jinqigufen.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cjk.fktsv.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ynm.zhixingplan.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wjd.epnwcf.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mcq.wangdashe.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bjo.tianlin.xyz

[C09] 递归
来源：http://vpf.redwolf501.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zqv.yuxming.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xfr.yuanzhike.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://enw.jianghu66.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ivg.yongpay.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vng.fanxiaobao.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://edl.hcnkem.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://eut.xinyue.icu

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hjw.ppjwa.cn

[C10] 变量作用域
来源：http://mhq.cheryme.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kuf.hfpthk.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mnd.smart0.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nps.zhiwuduotai.top

TS:   同 JS
来源：http://qzm.guowangkeji.top

Java: 方法内为块级作用域
来源：http://ayy.ydzc1.top

Go:   花括号块级作用域
来源：http://rnd.yj20258.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yve.iojbl.cn

C#:   块级作用域
来源：http://kew.bbcook.cn

[C11] 模块导入与导出
来源：http://fql.yueranfly.top

Py:   from module import func
来源：http://qaf.sjlbkw.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qhd.zdqjudy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://zhq.chenlongwang.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yyd.yueranfly.top

Java: import java.util.List;
来源：http://emk.jinqigfzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zzb.jlsjyb.cn

Ruby: require "json"; require_relative "./util"
来源：http://lte.yfazqb.com

C#:   using System.Text;
来源：http://qcn.iojbl.cn

[C12] 立即执行函数 IIFE
来源：http://kjr.xingfuxueyuan.xyz

Py:   (lambda: print("run"))()
来源：http://unr.birdmap.top

PHP:  (function () { echo "run"; })();
来源：http://bpq.mhx1999.top

JS:   (() => { console.log("run"); })();
来源：http://uua.fktsv.cn

TS:   (() => { console.log("run"); })();
来源：http://kuj.daria6918.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://unm.zhijiandao.cn

Go:   func() { fmt.Println("run") }()
来源：http://upz.chenlongwang.top

Ruby: -> { puts "run" }.call
来源：http://xhj.chenzaomai.com

C#:   // 无 IIFE：用静态构造函数
来源：http://eyz.316326.xyz

[C13] 类型声明 / 类型注解
来源：http://iaw.yongpay.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xot.hfpthk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bfj.yanxiufei.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://khv.fzhhl.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kom.xuanzx.com

Java: int add(int a, int b) { return a + b; }
来源：http://nvd.gotoacloud.top

Go:   func add(a, b int) int
来源：http://vug.yfazqb.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mgw.yueranfly.top

C#:   int Add(int a, int b) => a + b;
来源：http://iah.fanxiaobao.xyz

[C14] 泛型函数
来源：http://ptx.haohaochexian.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zit.chenzaomai.com

PHP:  // 无泛型
来源：http://khd.zdqjudy.top

JS:   // 无泛型
来源：http://aua.sysykeji.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://epr.jinqigfzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hwy.ppjwa.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qvz.wangshuangyany.cn

Ruby: # 无泛型
来源：http://ecf.gaohongyu789.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ftw.cheryme.top

[C15] 解构 / 展开参数
来源：http://tdp.cqqwz.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mep.zhoulong.xyz

PHP:  [$a, $b] = $pair;
来源：http://zol.zhengqikj.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xqg.jinyuanbaomall.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://avl.yj202588.top

Java: // 无解构
来源：http://pqp.smart0.xyz

Go:   // 无解构
来源：http://och.dashuyun.cn

Ruby: a, b = pair
来源：http://iru.gotoacloud.top

C#:   var (a, b) = pair;
来源：http://kuq.vqdsnc.cn

[C16] 函数 / 方法重载
来源：http://jqm.jianghu66.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jti.sysykeji.top

PHP:  // 无重载
来源：http://mvy.yongpay.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://zdt.0kj1m.cn

TS:   // 用联合类型或重载签名声明
来源：http://biz.nanxinkj.top

Java: void f(int a) {}  void f(String a) {}
来源：http://bis.zhongyouzk.top

Go:   // 无重载：用不同函数名
来源：http://eus.fanxiaobao.xyz

Ruby: # 无重载：靠动态参数
来源：http://buf.aizwys.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://lwh.cheryme.top

================================================================================
来源：http://idb.jinghuilouyu.cn

D. 数组 / 列表 / 集合
来源：http://rtf.52xcode.cn

================================================================================
来源：http://nyc.feifeiyinyue.top

[D01] 创建数组 / 列表
来源：http://owl.andypj.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://wxi.andypj.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://son.yueranfly.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bix.pengpengdd.cyou

TS:   const arr: number[] = [1, 2, 3];
来源：http://sjy.xuanzx.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uid.jinyuanbaomall.cn

Go:   arr := []int{1, 2, 3}
来源：http://kyi.nanxinkj.top

Ruby: arr = [1, 2, 3]
来源：http://qlp.nwbrower.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bra.sxryk.cn

[D02] 追加元素到末尾
来源：http://svw.quarkkingdee.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://aao.svipenyu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mcl.yuanzhike.top

JS:   arr.push(4);
来源：http://mqb.wangshuangyany.cn

TS:   arr.push(4);
来源：http://lft.vqdsnc.cn

Java: list.add(4);
来源：http://hdl.vehdjk.com

Go:   arr = append(arr, 4)
来源：http://rtt.shuidangran.top

Ruby: arr << 4; arr.push(5)
来源：http://qta.hnqzz.top

C#:   list.Add(4);
来源：http://zry.jinghuilouyu.cn

[D03] 在指定位置插入元素
来源：http://zzz.iojbl.cn

Py:   arr.insert(0, 0)
来源：http://zwy.zhoulong.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bbi.tanke756.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vpy.fktsv.cn

TS:   arr.splice(0, 0, 0);
来源：http://ozm.yongpay.top

Java: list.add(0, 0);
来源：http://zzn.yuxming.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fti.nanxinkj.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qmv.jlsjyb.cn

C#:   list.Insert(0, 0);
来源：http://onu.epnwcf.com

[D04] 删除元素
来源：http://jfr.chenlongwang.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yuy.316326.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rpp.zhaomingkeji.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://khd.wangdashe.top

TS:   arr.splice(0, 1);
来源：http://txh.xylfe.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://evn.daxiang520.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://iwa.ydjk.org.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uor.zhoulong.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vaa.cashguo.top

[D05] 访问与修改元素
来源：http://nte.fanxiaobao.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nyl.hywenlv.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tig.9152youxi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://axo.zhongyouzk.top

TS:   arr[0]; arr.at(-1);
来源：http://sil.hywenlv.cn

Java: list.get(0); list.set(0, 9);
来源：http://xcp.chenzaomai.com

Go:   arr[0]; arr[0] = 9
来源：http://dob.sufxvd.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ikf.havefunace.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lnr.chenzaomai.com

[D06] 数组长度
来源：http://dmo.vehdjk.com

Py:   len(arr)
来源：http://cqm.zycfv.cn

PHP:  count($arr);
来源：http://ppl.cheryme.top

JS:   arr.length
来源：http://voz.shzxlz.cn

TS:   arr.length
来源：http://qqz.havefunace.top

Java: list.size();
来源：http://mpc.hesvh.cn

Go:   len(arr)
来源：http://uhx.epnwcf.com

Ruby: arr.length; arr.size
来源：http://zks.iojbl.cn

C#:   list.Count;
来源：http://kym.uphjek.com

[D07] 切片 / 取子数组
来源：http://kif.hnqzz.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://oya.tarul.cn

PHP:  array_slice($arr, 1, 3);
来源：http://mek.sufxvd.cn

JS:   arr.slice(1, 4);
来源：http://yqo.cheryme.top

TS:   arr.slice(1, 4);
来源：http://zed.tarul.cn

Java: list.subList(1, 4);
来源：http://dqj.zhiwuduotai.top

Go:   arr[1:4]
来源：http://xlq.nanxinkj.top

Ruby: arr[1, 3]
来源：http://gxb.ydjk.org.cn

C#:   list.GetRange(1, 3);
来源：http://dex.ivvv.top

[D08] 合并两个数组
来源：http://zhq.svipenyu.cn

Py:   a + b;  a.extend(b)
来源：http://csf.hammf.cn

PHP:  array_merge($a, $b);
来源：http://kio.tian-w.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://nxu.yj20258.top

TS:   [...a, ...b];
来源：http://cjb.yanxiufei.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ilh.gzhubu.top

Go:   append(a, b...)
来源：http://ozo.fanxiaobao.xyz

Ruby: a + b;  a.concat(b)
来源：http://mla.dianchejie.cn

C#:   a.Concat(b).ToList()
来源：http://djd.bbcook.cn

[D09] 排序（升序）
来源：http://uje.cashguo.top

Py:   sorted(arr);  arr.sort()
来源：http://eqo.chenlongwang.top

PHP:  sort($arr);
来源：http://sfr.sjlbkw.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://oxv.hnxiangtu.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://syj.fzhhl.top

Java: Collections.sort(list);  list.sort(null);
来源：http://jfz.ppjwa.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dwz.zhongyouzk.top

Ruby: arr.sort
来源：http://wpd.yj20258.top

C#:   list.Sort();
来源：http://ick.tanke756.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://jza.zycfv.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jbt.wangdashe.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ler.pycfn.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cjg.yangfankeji.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://eqk.cashguo.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://eda.zdbjq.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nrc.epnwcf.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gnl.daxiang520.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ryc.gzhubu.top

[D11] 反转数组
来源：http://zot.smart0.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://xcm.yj202588.top

PHP:  array_reverse($arr);
来源：http://kgo.cdnleiting.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qxo.cheryme.top

TS:   [...arr].reverse();
来源：http://kjo.ehwqpu.com

Java: Collections.reverse(list);
来源：http://pad.yj202588.top

Go:   slices.Reverse(arr)
来源：http://vbx.smart0.xyz

Ruby: arr.reverse
来源：http://rou.nanxinkj.top

C#:   list.Reverse();
来源：http://zxr.ppjwa.cn

[D12] 查找元素下标
来源：http://ihj.ydzc1.top

Py:   arr.index(x);  x in arr
来源：http://xjv.hfpthk.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xjf.yueranfly.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pcw.yfazqb.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zon.cucudq.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yhh.vehdjk.com

Go:   slices.Index(arr, x)
来源：http://agl.jinqigufen.top

Ruby: arr.index(x)
来源：http://epr.snrcjt.cn

C#:   list.IndexOf(x);
来源：http://nvk.wangshuangyany.cn

[D13] 过滤（保留满足条件的）
来源：http://llo.aizwys.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ywh.gotoacloud.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kvi.fengsongda.top

JS:   arr.filter(x => x > 3)
来源：http://tyq.yj202588.top

TS:   arr.filter(x => x > 3)
来源：http://yaw.hfpthk.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://npb.pycfn.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yne.cheryme.top

Ruby: arr.select { |x| x > 3 }
来源：http://rdn.chenzaomai.com

C#:   list.Where(x => x > 3).ToList()
来源：http://pny.yuanzhike.top

[D14] 映射转换（每个元素变形）
来源：http://rgp.jqgfzy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://njh.bbcook.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dtq.sufxvd.cn

JS:   arr.map(x => x * 2)
来源：http://mgq.fehbvm.com

TS:   arr.map(x => x * 2)
来源：http://hca.xuetiantiany.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wok.ppjwa.cn

Go:   // 手写循环
来源：http://swi.zhongyouzk.top

Ruby: arr.map { |x| x * 2 }
来源：http://rtr.zhijiandao.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://evq.hnxiangtu.top

[D15] 去重
来源：http://fkm.andypj.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tnf.ydjk.org.cn

PHP:  array_unique($arr);
来源：http://wrm.zdqjudy.top

JS:   [...new Set(arr)]
来源：http://vlj.hcnkem.com

TS:   [...new Set(arr)]
来源：http://exo.pengpengdd.cyou

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rwp.gotoacloud.top

Go:   // 用 map[T]struct{} 手写
来源：http://pqv.chenzaomai.com

Ruby: arr.uniq
来源：http://piq.mhx1999.top

C#:   list.Distinct().ToList()
来源：http://xqh.hesvh.cn

[D16] 求和与平均值
来源：http://cme.316326.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nft.hywenlv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://iss.havefunace.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://too.vehdjk.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tll.shzxlz.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dya.9152youxi.cn

Go:   // 手写循环累加
来源：http://vhc.hnxiangtu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vsk.tarul.cn

C#:   list.Sum();  list.Average()
来源：http://xxo.zycfv.cn

[D17] 最大值与最小值
来源：http://ivd.snrcjt.cn

Py:   max(arr);  min(arr)
来源：http://pnz.guowangkeji.top

PHP:  max($arr);  min($arr);
来源：http://zra.smart0.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nml.yuxming.cn

TS:   Math.max(...arr);
来源：http://pce.pengpengdd.cyou

Java: Collections.max(list);  Collections.min(list);
来源：http://tth.ydjk.org.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nry.ctjpmb.com

Ruby: arr.max;  arr.min
来源：http://tcz.shzxlz.cn

C#:   list.Max();  list.Min()
来源：http://rek.daria6918.cn

[D18] 扁平化嵌套数组
来源：http://ote.bjfxy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://oiw.zhaomingkeji.xyz

PHP:  array_merge(...$nested);
来源：http://gqf.jinyuanbaomall.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uxt.hnqzz.top

TS:   nested.flat();
来源：http://syt.jinghuilouyu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://evu.hesvh.cn

Go:   // 手写双层循环
来源：http://grf.guannengcc.top

Ruby: nested.flatten
来源：http://wql.hongshengwenyu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ket.snrcjt.cn

[D19] 按字段分组
来源：http://qtm.jyoumei.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ivu.shangyingyoupin.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://sxx.tian-w.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jlj.feifeiyinyue.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://cbw.smart0.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://etu.gaohongyu789.top

Go:   // 手写 map[string][]T
来源：http://gwt.yj202588.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://azk.chenjidiqi.icu

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vjl.zhiwuduotai.top

[D20] 统计每个元素出现次数
来源：http://uku.cheryme.top

Py:   Counter(arr)
来源：http://qoy.wangshuangyany.cn

PHP:  array_count_values($arr);
来源：http://jbb.jinqigfzy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xlg.gotoacloud.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lcu.andypj.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bvl.ppjwa.cn

Go:   // 手写 map[T]int
来源：http://lkz.yangfankeji.com

Ruby: arr.tally
来源：http://nik.birdmap.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kxz.pengpengdd.cyou

[D21] 判断是否包含某元素
来源：http://hao.pengpengdd.cyou

Py:   x in arr
来源：http://fdt.guannengcc.top


<!-- 参考信息 -->