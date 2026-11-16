代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://mos.daria6918.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pmq.kuanghao11.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rsc.xziqi.cn

Ruby: square = ->(x) { x * x }
来源：http://wmg.hongshengwenyu.top

C#:   Func<int, int> square = x => x * x;
来源：http://ksw.shangyingyoupin.top

[C07] 把函数作为参数传入
来源：http://vyz.bbcook.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hyb.smart0.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://vat.cdnleiting.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://arw.jinyuanbaomall.cn

TS:   arr.map(String)
来源：http://mge.nanxuanxn.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gjy.aizwys.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://voq.jinghuilouyu.cn

Ruby: arr.map(&:upcase)
来源：http://won.jinqigfzy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://eyd.yonumen.top

[C08] 闭包
来源：http://yzp.smart0.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ged.tian-w.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lpn.316326.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ybz.guowangkeji.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://naa.jqgufenzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jfv.shuidangran.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rnn.feifeiyinyue.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://grd.haohaochexian.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kbc.cdnleiting.top

[C09] 递归
来源：http://dyi.bjfxy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tfb.jqgfzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wzi.wangdashe.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hvf.hysaishi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://htb.nwbrower.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ihy.ivvv.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://duo.hesvh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://udc.jianghu66.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hou.ctjpmb.com

[C10] 变量作用域
来源：http://tav.dianchejie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ddx.zhijiandao.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://agg.jinqigufen.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ozo.tanke756.top

TS:   同 JS
来源：http://xms.jlsjyb.cn

Java: 方法内为块级作用域
来源：http://itp.xziqi.cn

Go:   花括号块级作用域
来源：http://qhk.jiagoushi.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qfe.zhixingplan.top

C#:   块级作用域
来源：http://qix.yfazqb.com

[C11] 模块导入与导出
来源：http://hay.yonumen.top

Py:   from module import func
来源：http://zzy.zhixingplan.top

PHP:  require "file.php";  或 use App\Service;
来源：http://eia.wangdashe.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://htj.zdbjq.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wds.uphjek.com

Java: import java.util.List;
来源：http://iaj.aizwys.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ing.iojbl.cn

Ruby: require "json"; require_relative "./util"
来源：http://egf.yangfankeji.com

C#:   using System.Text;
来源：http://ebj.tarul.cn

[C12] 立即执行函数 IIFE
来源：http://ozf.aizwys.cn

Py:   (lambda: print("run"))()
来源：http://kgi.zhoulong.xyz

PHP:  (function () { echo "run"; })();
来源：http://xoh.yongpay.top

JS:   (() => { console.log("run"); })();
来源：http://pfl.vqdsnc.cn

TS:   (() => { console.log("run"); })();
来源：http://rmz.hammf.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wci.haohaochexian.top

Go:   func() { fmt.Println("run") }()
来源：http://rjw.epnwcf.com

Ruby: -> { puts "run" }.call
来源：http://ofc.zhoulong.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://bai.vqdsnc.cn

[C13] 类型声明 / 类型注解
来源：http://zqc.zdqjudy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bqh.andypj.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zgt.xingfuxueyuan.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://abp.daria6918.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cko.wangdashe.top

Java: int add(int a, int b) { return a + b; }
来源：http://uqw.zhengqikj.top

Go:   func add(a, b int) int
来源：http://cqb.shuidangran.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dfq.birdmap.top

C#:   int Add(int a, int b) => a + b;
来源：http://mkf.ydzc1.top

[C14] 泛型函数
来源：http://odc.yj202588.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pnp.ppjwa.cn

PHP:  // 无泛型
来源：http://ghk.vehdjk.com

JS:   // 无泛型
来源：http://gkg.shzxlz.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bhs.bbcook.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://feq.fzhhl.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nlf.guowangkeji.top

Ruby: # 无泛型
来源：http://flq.hysaishi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fvu.meibo888.top

[C15] 解构 / 展开参数
来源：http://ook.vqdsnc.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ecm.gotoacloud.top

PHP:  [$a, $b] = $pair;
来源：http://ubf.jyoumei.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dyc.iojbl.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qyb.kuanghao11.cn

Java: // 无解构
来源：http://vux.ppjwa.cn

Go:   // 无解构
来源：http://fly.pengpengdd.cyou

Ruby: a, b = pair
来源：http://jze.316326.xyz

C#:   var (a, b) = pair;
来源：http://szh.hesvh.cn

[C16] 函数 / 方法重载
来源：http://psz.9152youxi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tcq.jinqigufen.top

PHP:  // 无重载
来源：http://lhx.zycfv.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fic.zhijiandao.cn

TS:   // 用联合类型或重载签名声明
来源：http://adw.feifeiyinyue.top

Java: void f(int a) {}  void f(String a) {}
来源：http://qwe.yangfankeji.com

Go:   // 无重载：用不同函数名
来源：http://ync.gzhubu.top

Ruby: # 无重载：靠动态参数
来源：http://bpg.meibo888.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://vlp.xingfuxueyuan.xyz

================================================================================
来源：http://ftl.wangshuangyany.cn

D. 数组 / 列表 / 集合
来源：http://ihz.zhongyouzk.top

================================================================================
来源：http://gqh.cqqwz.cn

[D01] 创建数组 / 列表
来源：http://iqm.hywenlv.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://eos.daria6918.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xqf.pycfn.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wsx.jqgufenzy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://zfv.yongpay.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tgx.yueranfly.top

Go:   arr := []int{1, 2, 3}
来源：http://lue.ydjk.org.cn

Ruby: arr = [1, 2, 3]
来源：http://lql.fanxiaobao.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cid.ctjpmb.com

[D02] 追加元素到末尾
来源：http://yrm.ywan-chungtsiang.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xbq.gaohongyu789.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://whm.316326.xyz

JS:   arr.push(4);
来源：http://rip.yongpay.top

TS:   arr.push(4);
来源：http://hha.hfpthk.cn

Java: list.add(4);
来源：http://xir.hysaishi.cn

Go:   arr = append(arr, 4)
来源：http://zzr.chenjidiqi.icu

Ruby: arr << 4; arr.push(5)
来源：http://lxh.zycfv.cn

C#:   list.Add(4);
来源：http://qwc.vqdsnc.cn

[D03] 在指定位置插入元素
来源：http://odj.jqgfzy.top

Py:   arr.insert(0, 0)
来源：http://yjk.shangyingyoupin.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mlr.yfazqb.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uwj.yongpay.top

TS:   arr.splice(0, 0, 0);
来源：http://yxp.cucudq.cn

Java: list.add(0, 0);
来源：http://sbo.9152youxi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vnu.zhoulong.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hes.nanxinkj.top

C#:   list.Insert(0, 0);
来源：http://kyf.ehwqpu.com

[D04] 删除元素
来源：http://put.ivvv.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zfo.jqgfzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cqu.shanyushiyangtech.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zpm.mhx1999.top

TS:   arr.splice(0, 1);
来源：http://moz.yvedp.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ifm.zycfv.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qtp.shanyushiyangtech.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nce.ppjwa.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fbp.c1oappe.top

[D05] 访问与修改元素
来源：http://mic.fengsongda.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dpf.9152youxi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://aoe.316326.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://oug.xziqi.cn

TS:   arr[0]; arr.at(-1);
来源：http://cjd.sweek.top

Java: list.get(0); list.set(0, 9);
来源：http://dac.jiagoushi.top

Go:   arr[0]; arr[0] = 9
来源：http://qrr.epnwcf.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kxs.yonumen.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yuv.ybcxt.top

[D06] 数组长度
来源：http://tdj.sufxvd.cn

Py:   len(arr)
来源：http://vaz.gzhubu.top

PHP:  count($arr);
来源：http://eou.daxiang520.top

JS:   arr.length
来源：http://bae.yuanzhike.top

TS:   arr.length
来源：http://ihg.316326.xyz

Java: list.size();
来源：http://nlx.chenjidiqi.icu

Go:   len(arr)
来源：http://rbu.jinqigufen.top

Ruby: arr.length; arr.size
来源：http://bip.zhongyouzk.top

C#:   list.Count;
来源：http://meg.daxiang520.top

[D07] 切片 / 取子数组
来源：http://stm.havefunace.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://oos.gzhubu.top

PHP:  array_slice($arr, 1, 3);
来源：http://zxk.chenjidiqi.icu

JS:   arr.slice(1, 4);
来源：http://afk.zhijiandao.cn

TS:   arr.slice(1, 4);
来源：http://bqs.wangshuangyany.cn

Java: list.subList(1, 4);
来源：http://mix.hammf.cn

Go:   arr[1:4]
来源：http://pom.xylfe.cn

Ruby: arr[1, 3]
来源：http://wcn.0kj1m.cn

C#:   list.GetRange(1, 3);
来源：http://ifc.tian-w.cn

[D08] 合并两个数组
来源：http://ugl.hnqzz.top

Py:   a + b;  a.extend(b)
来源：http://jpy.hywenlv.cn

PHP:  array_merge($a, $b);
来源：http://ymr.hfpthk.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://sdr.shangyingyoupin.top

TS:   [...a, ...b];
来源：http://hno.jinghuilouyu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cyu.guannengcc.top

Go:   append(a, b...)
来源：http://pnc.fzhhl.top

Ruby: a + b;  a.concat(b)
来源：http://zuy.jlsjyb.cn

C#:   a.Concat(b).ToList()
来源：http://dab.ivvv.top

[D09] 排序（升序）
来源：http://aqt.kuanghao11.cn

Py:   sorted(arr);  arr.sort()
来源：http://cda.aizwys.cn

PHP:  sort($arr);
来源：http://vwf.xuetiantiany.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://acw.dianchejie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://dqd.quarkkingdee.top

Java: Collections.sort(list);  list.sort(null);
来源：http://qyh.tianlin.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jaf.jyoumei.cn

Ruby: arr.sort
来源：http://xvx.xziqi.cn

C#:   list.Sort();
来源：http://xjg.gotoacloud.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://fsl.aibaodan.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://urf.sysykeji.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ixg.hammf.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sre.fanxiaobao.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yjq.chenzaomai.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qcs.havefunace.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hwb.bbcook.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yyx.yuanzhike.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bck.yj202588.top

[D11] 反转数组
来源：http://vbw.hesvh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qrr.aibaodan.cn

PHP:  array_reverse($arr);
来源：http://sum.uphjek.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uvs.hammf.cn

TS:   [...arr].reverse();
来源：http://xun.meibo888.top

Java: Collections.reverse(list);
来源：http://ivh.andypj.xyz

Go:   slices.Reverse(arr)
来源：http://kzk.yj20258888.top

Ruby: arr.reverse
来源：http://oli.yonumen.top

C#:   list.Reverse();
来源：http://erk.zhaomingkeji.xyz

[D12] 查找元素下标
来源：http://sdq.hcnkem.com

Py:   arr.index(x);  x in arr
来源：http://wpx.zhixingplan.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://crx.uphjek.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dra.haohaochexian.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://amk.316326.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sgh.guannengcc.top

Go:   slices.Index(arr, x)
来源：http://rjj.havefunace.top

Ruby: arr.index(x)
来源：http://rsn.ybcxt.top

C#:   list.IndexOf(x);
来源：http://mtp.sufxvd.cn

[D13] 过滤（保留满足条件的）
来源：http://sbz.cheryme.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cms.zhoulong.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mle.yvedp.cn

JS:   arr.filter(x => x > 3)
来源：http://gch.yangfankeji.com

TS:   arr.filter(x => x > 3)
来源：http://dqz.jqgfzy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://via.chenlongwang.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uxd.haohaochexian.top

Ruby: arr.select { |x| x > 3 }
来源：http://dyj.guannengcc.top

C#:   list.Where(x => x > 3).ToList()
来源：http://htp.fengsongda.top

[D14] 映射转换（每个元素变形）
来源：http://eos.birdmap.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://eni.yueranfly.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lze.zdqjudy.top

JS:   arr.map(x => x * 2)
来源：http://ygo.shanyushiyangtech.top

TS:   arr.map(x => x * 2)
来源：http://zbp.zhengqikj.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://lgm.cashguo.top

Go:   // 手写循环
来源：http://vql.shanyushiyangtech.top

Ruby: arr.map { |x| x * 2 }
来源：http://obp.yonumen.top

C#:   list.Select(x => x * 2).ToList()
来源：http://vua.xinyue.icu

[D15] 去重
来源：http://qyj.hcnkem.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vqt.haohaochexian.top

PHP:  array_unique($arr);
来源：http://ahi.tian-w.cn

JS:   [...new Set(arr)]
来源：http://eam.svipenyu.cn

TS:   [...new Set(arr)]
来源：http://ety.tian-w.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cqm.svipenyu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ckw.xziqi.cn

Ruby: arr.uniq
来源：http://kld.cheryme.top

C#:   list.Distinct().ToList()
来源：http://faj.jqgfzy.top

[D16] 求和与平均值
来源：http://kbk.bbcook.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tgt.hysaishi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tbp.jqgufenzy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://npk.fzhhl.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ruf.daria6918.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kot.gaohongyu789.top

Go:   // 手写循环累加
来源：http://usa.nwbrower.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hww.aibaodan.cn

C#:   list.Sum();  list.Average()
来源：http://nwk.xylfe.cn

[D17] 最大值与最小值
来源：http://rfn.ywan-chungtsiang.top

Py:   max(arr);  min(arr)
来源：http://onc.fengsongda.top

PHP:  max($arr);  min($arr);
来源：http://pax.yueranfly.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ubf.jinqigfzy.top

TS:   Math.max(...arr);
来源：http://mty.gotoacloud.top

Java: Collections.max(list);  Collections.min(list);
来源：http://nhs.yvedp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kay.snrcjt.cn

Ruby: arr.max;  arr.min
来源：http://upo.feifeiyinyue.top

C#:   list.Max();  list.Min()
来源：http://gzz.guowangkeji.top

[D18] 扁平化嵌套数组
来源：http://dxe.hnqzz.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bbc.yuanzhike.top

PHP:  array_merge(...$nested);
来源：http://tck.ydzc1.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://oxn.ydjk.org.cn

TS:   nested.flat();
来源：http://vaz.guannengcc.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://izu.yuxming.cn

Go:   // 手写双层循环
来源：http://luv.vqdsnc.cn

Ruby: nested.flatten
来源：http://gew.epnwcf.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://hba.ybcxt.top

[D19] 按字段分组
来源：http://hrb.cheryme.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sxr.yj20258.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gmk.hongshengwenyu.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dho.fengsongda.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://vfx.dianchejie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qnf.gzhubu.top

Go:   // 手写 map[string][]T
来源：http://rwb.zycfv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wms.gaohongyu789.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xvw.wangshuangyany.cn

[D20] 统计每个元素出现次数
来源：http://kxg.jyoumei.cn

Py:   Counter(arr)
来源：http://jti.cucudq.cn

PHP:  array_count_values($arr);
来源：http://rbc.birdmap.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qrr.hammf.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wid.ctjpmb.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hbq.yuxming.cn

Go:   // 手写 map[T]int
来源：http://xxn.52xcode.cn

Ruby: arr.tally
来源：http://hds.zdbjq.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://eyx.yuanzhike.top

[D21] 判断是否包含某元素
来源：http://xty.cashguo.top

Py:   x in arr
来源：http://mbn.jqgfzy.top

PHP:  in_array($x, $arr, true);
来源：http://krj.ehwqpu.com

JS:   arr.includes(x)
来源：http://jna.guannengcc.top

TS:   arr.includes(x)
来源：http://bdf.fengsongda.top

Java: list.contains(x)
来源：http://qpg.c1oappe.top

Go:   slices.Contains(arr, x)
来源：http://ied.cdnleiting.top

Ruby: arr.include?(x)
来源：http://luk.zhaomingkeji.xyz

C#:   list.Contains(x)
来源：http://fwv.pengpengdd.cyou

[D22] 复制数组（避免共享引用）
来源：http://exr.dianchejie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pbd.yongpay.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nit.yj20258.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://how.wangshuangyany.cn

TS:   [...arr];
来源：http://nen.jqgufenzy.top

Java: new ArrayList<>(list);
来源：http://cij.cdnleiting.top

Go:   copied := append([]int(nil), arr...)
来源：http://qqf.yuxming.cn

Ruby: arr.dup;  arr.clone
来源：http://pcf.zhoulong.xyz

C#:   new List<int>(list);
来源：http://jsm.sysykeji.top

[D23] reduce 累积计算
来源：http://ijl.fanxiaobao.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wqg.sjlbkw.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ewp.epnwcf.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nlb.zdqjudy.top


<!-- 参考信息 -->