代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://pvy.zhengqikj.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ksq.cqqwz.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rho.hywenlv.cn

Ruby: square = ->(x) { x * x }
来源：http://udg.jinyuanbaomall.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bzk.ppjwa.cn

[C07] 把函数作为参数传入
来源：http://wvq.hongshengwenyu.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qmm.tanke756.top

PHP:  array_map("strtoupper", $arr);
来源：http://vub.quarkkingdee.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wdh.feifeiyinyue.top

TS:   arr.map(String)
来源：http://xyi.yfazqb.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bjz.birdmap.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wjl.bjfxy.top

Ruby: arr.map(&:upcase)
来源：http://uhg.pengpengdd.cyou

C#:   arr.Select(s => s.ToUpper())
来源：http://vlk.zdqjudy.top

[C08] 闭包
来源：http://cbe.yueranfly.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wuj.bbcook.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gks.sjlbkw.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dyv.yfazqb.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bcq.zhoulong.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ekv.hfpthk.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yxe.hcnkem.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yaq.tarul.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vta.cucudq.cn

[C09] 递归
来源：http://bpq.havefunace.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rtr.tanke756.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fmg.jlsjyb.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ukf.yj20258.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://afv.quarkkingdee.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tqe.zhengqikj.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://avf.smart0.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tgt.ctjpmb.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hay.ydzc1.top

[C10] 变量作用域
来源：http://jhv.chenjidiqi.icu

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://asa.tianlin.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rvf.xinyue.icu

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cqa.yongpay.top

TS:   同 JS
来源：http://xmu.52xcode.cn

Java: 方法内为块级作用域
来源：http://ewc.hysaishi.cn

Go:   花括号块级作用域
来源：http://jpo.andypj.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://apq.zhaomingkeji.xyz

C#:   块级作用域
来源：http://ryf.ehwqpu.com

[C11] 模块导入与导出
来源：http://hyd.yuxming.cn

Py:   from module import func
来源：http://orz.bjfxy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://wdw.jqgfzy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ftu.daxiang520.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tqp.jlsjyb.cn

Java: import java.util.List;
来源：http://lly.ywan-chungtsiang.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mdh.hammf.cn

Ruby: require "json"; require_relative "./util"
来源：http://sbq.chenzaomai.com

C#:   using System.Text;
来源：http://hkq.jinghuilouyu.cn

[C12] 立即执行函数 IIFE
来源：http://yfv.andypj.xyz

Py:   (lambda: print("run"))()
来源：http://qda.gzhubu.top

PHP:  (function () { echo "run"; })();
来源：http://unk.bjfxy.top

JS:   (() => { console.log("run"); })();
来源：http://zga.meibo888.top

TS:   (() => { console.log("run"); })();
来源：http://bbo.aibaodan.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mec.dashuyun.cn

Go:   func() { fmt.Println("run") }()
来源：http://bgg.redwolf501.top

Ruby: -> { puts "run" }.call
来源：http://dhd.epnwcf.com

C#:   // 无 IIFE：用静态构造函数
来源：http://wqg.c1oappe.top

[C13] 类型声明 / 类型注解
来源：http://vit.zhengqikj.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qtd.cqqwz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jdp.jinqigufen.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kis.xylfe.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bfj.bjfxy.top

Java: int add(int a, int b) { return a + b; }
来源：http://meg.hongshengwenyu.top

Go:   func add(a, b int) int
来源：http://dll.ywan-chungtsiang.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://usf.yj20258.top

C#:   int Add(int a, int b) => a + b;
来源：http://qmq.ctjpmb.com

[C14] 泛型函数
来源：http://fqc.cheryme.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xvj.bbcook.cn

PHP:  // 无泛型
来源：http://yoi.kuanghao11.cn

JS:   // 无泛型
来源：http://eze.yj202588.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://urk.sjlbkw.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jej.yangfankeji.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ogi.birdmap.top

Ruby: # 无泛型
来源：http://tqz.guannengcc.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://euq.zhaomingkeji.xyz

[C15] 解构 / 展开参数
来源：http://kgt.zdqjudy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ndh.yangfankeji.com

PHP:  [$a, $b] = $pair;
来源：http://dng.meibo888.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gmv.hnxiangtu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://oaz.meibo888.top

Java: // 无解构
来源：http://nxd.tian-w.cn

Go:   // 无解构
来源：http://ylc.jinyuanbaomall.cn

Ruby: a, b = pair
来源：http://lsf.jinqigfzy.top

C#:   var (a, b) = pair;
来源：http://jnc.wangdashe.top

[C16] 函数 / 方法重载
来源：http://xmt.cqqwz.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://apx.xziqi.cn

PHP:  // 无重载
来源：http://xoh.ydzc1.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://izt.sweek.top

TS:   // 用联合类型或重载签名声明
来源：http://ixc.kuanghao11.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ivy.ydzc1.top

Go:   // 无重载：用不同函数名
来源：http://dkz.52xcode.cn

Ruby: # 无重载：靠动态参数
来源：http://dhk.jianghu66.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://puv.cucudq.cn

================================================================================
来源：http://ttg.jiagoushi.top

D. 数组 / 列表 / 集合
来源：http://jad.gotoacloud.top

================================================================================
来源：http://wdg.xuanzx.com

[D01] 创建数组 / 列表
来源：http://jeo.tarul.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://gyv.vqdsnc.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://moq.ydzc1.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lkk.ppjwa.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yal.xylfe.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://knv.nwbrower.top

Go:   arr := []int{1, 2, 3}
来源：http://gvj.zhiwuduotai.top

Ruby: arr = [1, 2, 3]
来源：http://oco.hysaishi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ohv.andypj.xyz

[D02] 追加元素到末尾
来源：http://kls.fehbvm.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://joq.svipenyu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oqt.pengpengdd.cyou

JS:   arr.push(4);
来源：http://syi.pengpengdd.cyou

TS:   arr.push(4);
来源：http://gma.chenzaomai.com

Java: list.add(4);
来源：http://jew.nwbrower.top

Go:   arr = append(arr, 4)
来源：http://mng.ywan-chungtsiang.top

Ruby: arr << 4; arr.push(5)
来源：http://bwk.jqgufenzy.top

C#:   list.Add(4);
来源：http://mqy.jlsjyb.cn

[D03] 在指定位置插入元素
来源：http://nyy.cqqwz.cn

Py:   arr.insert(0, 0)
来源：http://hxa.shangyingyoupin.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gio.birdmap.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ykp.yj20258.top

TS:   arr.splice(0, 0, 0);
来源：http://rzf.epnwcf.com

Java: list.add(0, 0);
来源：http://ybg.cdnleiting.top

Go:   arr = append([]int{0}, arr...)
来源：http://myr.cdnleiting.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://geq.jlsjyb.cn

C#:   list.Insert(0, 0);
来源：http://pls.dashuyun.cn

[D04] 删除元素
来源：http://zhh.xziqi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ajr.pycfn.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qut.chenjidiqi.icu

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tjq.shzxlz.cn

TS:   arr.splice(0, 1);
来源：http://ybc.ydjk.org.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://unm.gzhubu.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hec.yuxming.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ngx.yonumen.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sdb.yj20258888.top

[D05] 访问与修改元素
来源：http://zew.tian-w.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cft.ydjk.org.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://agn.kuanghao11.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mle.sjlbkw.cn

TS:   arr[0]; arr.at(-1);
来源：http://zyn.sjlbkw.cn

Java: list.get(0); list.set(0, 9);
来源：http://gku.fanxiaobao.xyz

Go:   arr[0]; arr[0] = 9
来源：http://osr.pycfn.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rgw.zhoulong.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tek.xylfe.cn

[D06] 数组长度
来源：http://ohv.0kj1m.cn

Py:   len(arr)
来源：http://nst.fehbvm.com

PHP:  count($arr);
来源：http://frx.jinyuanbaomall.cn

JS:   arr.length
来源：http://rfm.sufxvd.cn

TS:   arr.length
来源：http://kye.sweek.top

Java: list.size();
来源：http://qlq.yj202588.top

Go:   len(arr)
来源：http://yoq.jlsjyb.cn

Ruby: arr.length; arr.size
来源：http://ovs.zdqjudy.top

C#:   list.Count;
来源：http://jnj.xuetiantiany.cn

[D07] 切片 / 取子数组
来源：http://ewh.hywenlv.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://drh.ywan-chungtsiang.top

PHP:  array_slice($arr, 1, 3);
来源：http://ttn.aizwys.cn

JS:   arr.slice(1, 4);
来源：http://rrm.chenzaomai.com

TS:   arr.slice(1, 4);
来源：http://kcr.ppjwa.cn

Java: list.subList(1, 4);
来源：http://nuk.yuxming.cn

Go:   arr[1:4]
来源：http://vhh.chenjidiqi.icu

Ruby: arr[1, 3]
来源：http://fkd.zhixingplan.top

C#:   list.GetRange(1, 3);
来源：http://bba.shangyingyoupin.top

[D08] 合并两个数组
来源：http://uoa.yongpay.top

Py:   a + b;  a.extend(b)
来源：http://dyp.fehbvm.com

PHP:  array_merge($a, $b);
来源：http://dbk.zycfv.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hap.vqdsnc.cn

TS:   [...a, ...b];
来源：http://dlt.yfazqb.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jvr.fanxiaobao.xyz

Go:   append(a, b...)
来源：http://hog.wangshuangyany.cn

Ruby: a + b;  a.concat(b)
来源：http://snx.wangdashe.top

C#:   a.Concat(b).ToList()
来源：http://goa.jiagoushi.top

[D09] 排序（升序）
来源：http://dbl.cashguo.top

Py:   sorted(arr);  arr.sort()
来源：http://lkq.ivvv.top

PHP:  sort($arr);
来源：http://uws.hcnkem.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ips.hongshengwenyu.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://rfz.xinyue.icu

Java: Collections.sort(list);  list.sort(null);
来源：http://oov.yj20258888.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kvl.yanxiufei.cn

Ruby: arr.sort
来源：http://znf.snrcjt.cn

C#:   list.Sort();
来源：http://oev.zhiwuduotai.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://reg.fehbvm.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qlk.zhoulong.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kqc.zdbjq.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jfq.daria6918.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ruv.pycfn.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rnv.xziqi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lek.chenjidiqi.icu

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zhk.pycfn.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dva.guannengcc.top

[D11] 反转数组
来源：http://dnh.cqqwz.cn

Py:   arr[::-1];  arr.reverse()
来源：http://imy.zhaomingkeji.xyz

PHP:  array_reverse($arr);
来源：http://nuq.jyoumei.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nys.sysykeji.top

TS:   [...arr].reverse();
来源：http://lvi.fktsv.cn

Java: Collections.reverse(list);
来源：http://egz.yonumen.top

Go:   slices.Reverse(arr)
来源：http://amo.tian-w.cn

Ruby: arr.reverse
来源：http://npw.ehwqpu.com

C#:   list.Reverse();
来源：http://lde.hywenlv.cn

[D12] 查找元素下标
来源：http://mgp.birdmap.top

Py:   arr.index(x);  x in arr
来源：http://arr.yongpay.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cwi.jiagoushi.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vni.zhoulong.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wcm.gotoacloud.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lrn.ehwqpu.com

Go:   slices.Index(arr, x)
来源：http://wap.andypj.xyz

Ruby: arr.index(x)
来源：http://utc.tianlin.xyz

C#:   list.IndexOf(x);
来源：http://cev.daxiang520.top

[D13] 过滤（保留满足条件的）
来源：http://ghx.zdbjq.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://btb.feifeiyinyue.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pdy.yanxiufei.cn

JS:   arr.filter(x => x > 3)
来源：http://uil.fktsv.cn

TS:   arr.filter(x => x > 3)
来源：http://atz.ppjwa.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qnl.cashguo.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rlj.tarul.cn

Ruby: arr.select { |x| x > 3 }
来源：http://njh.pycfn.com

C#:   list.Where(x => x > 3).ToList()
来源：http://pfq.epnwcf.com

[D14] 映射转换（每个元素变形）
来源：http://wkc.gogol.net.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cnr.cdnleiting.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rhz.aizwys.cn

JS:   arr.map(x => x * 2)
来源：http://wgs.xuetiantiany.cn

TS:   arr.map(x => x * 2)
来源：http://eyj.xziqi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wsf.chenjidiqi.icu

Go:   // 手写循环
来源：http://lhb.xylfe.cn

Ruby: arr.map { |x| x * 2 }
来源：http://nwt.yanxiufei.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://uwy.snrcjt.cn

[D15] 去重
来源：http://bdc.yongpay.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bqb.zhongyouzk.top

PHP:  array_unique($arr);
来源：http://ask.vqdsnc.cn

JS:   [...new Set(arr)]
来源：http://nip.zhengqikj.top

TS:   [...new Set(arr)]
来源：http://sbf.gotoacloud.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zgw.shuidangran.top

Go:   // 用 map[T]struct{} 手写
来源：http://wil.sjlbkw.cn

Ruby: arr.uniq
来源：http://nve.cashguo.top

C#:   list.Distinct().ToList()
来源：http://bry.zhengqikj.top

[D16] 求和与平均值
来源：http://jrb.gotoacloud.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://squ.ybcxt.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://czm.shanyushiyangtech.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dut.dashuyun.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kyv.aizwys.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://acz.svipenyu.cn

Go:   // 手写循环累加
来源：http://kcy.fengsongda.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zoy.hesvh.cn

C#:   list.Sum();  list.Average()
来源：http://uqu.zhoulong.xyz

[D17] 最大值与最小值
来源：http://afl.meibo888.top

Py:   max(arr);  min(arr)
来源：http://nvp.shzxlz.cn

PHP:  max($arr);  min($arr);
来源：http://yxw.chenjidiqi.icu

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hak.zhiwuduotai.top

TS:   Math.max(...arr);
来源：http://idi.xinyue.icu

Java: Collections.max(list);  Collections.min(list);
来源：http://hyv.chenjidiqi.icu

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xbz.tarul.cn

Ruby: arr.max;  arr.min
来源：http://uqs.xuanzx.com

C#:   list.Max();  list.Min()
来源：http://vbq.shangyingyoupin.top

[D18] 扁平化嵌套数组
来源：http://fgx.jinqigufen.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://efi.tianlin.xyz

PHP:  array_merge(...$nested);
来源：http://hcc.zdqjudy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rka.yuxming.cn

TS:   nested.flat();
来源：http://tbl.jianghu66.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cob.hnqzz.top

Go:   // 手写双层循环
来源：http://ofx.shanyushiyangtech.top

Ruby: nested.flatten
来源：http://esz.zhongyouzk.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://how.zhijiandao.cn

[D19] 按字段分组
来源：http://dcl.hnxiangtu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://uvr.fktsv.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xjz.zhaomingkeji.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dcl.smart0.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://zno.iojbl.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zxc.sxryk.cn

Go:   // 手写 map[string][]T
来源：http://uvj.vehdjk.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://dtr.jqgfzy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uba.xingfuxueyuan.xyz

[D20] 统计每个元素出现次数
来源：http://mkv.sysykeji.top

Py:   Counter(arr)
来源：http://bii.yanxiufei.cn

PHP:  array_count_values($arr);
来源：http://hdw.gzhubu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://omt.chenlongwang.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dza.nanxinkj.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dpz.hnxiangtu.top

Go:   // 手写 map[T]int
来源：http://lhu.ctjpmb.com

Ruby: arr.tally
来源：http://mnl.hnxiangtu.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qhk.jinqigfzy.top

[D21] 判断是否包含某元素
来源：http://znx.yanxiufei.cn

Py:   x in arr
来源：http://seo.52xcode.cn

PHP:  in_array($x, $arr, true);
来源：http://qlj.shanyushiyangkeji.top

JS:   arr.includes(x)
来源：http://fqu.sufxvd.cn

TS:   arr.includes(x)
来源：http://dwo.chenlongwang.top

Java: list.contains(x)
来源：http://pgw.ydjk.org.cn

Go:   slices.Contains(arr, x)
来源：http://mkn.sufxvd.cn

Ruby: arr.include?(x)
来源：http://yuo.haohaochexian.top

C#:   list.Contains(x)
来源：http://tka.bjfxy.top

[D22] 复制数组（避免共享引用）
来源：http://oon.xuetiantiany.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://odq.daria6918.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nrb.shanyushiyangkeji.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hxh.havefunace.top

TS:   [...arr];
来源：http://swb.fktsv.cn

Java: new ArrayList<>(list);
来源：http://jee.jyoumei.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ohs.sweek.top

Ruby: arr.dup;  arr.clone
来源：http://rzc.mhx1999.top

C#:   new List<int>(list);
来源：http://mrw.jqgufenzy.top

[D23] reduce 累积计算
来源：http://scd.quarkkingdee.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://epn.daxiang520.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gaw.sweek.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iek.hywenlv.cn


<!-- 参考信息 -->