代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kwu.zdqjudy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://aar.xuetiantiany.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rji.fktsv.cn

[C09] 递归
来源：http://wzo.gogol.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xao.hesvh.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tqk.ydjk.org.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tuk.guannengcc.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iet.chenzaomai.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qqy.hnxiangtu.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gjk.yj20258.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bho.yongpay.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tal.gotoacloud.top

[C10] 变量作用域
来源：http://wjq.mhx1999.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hbv.cqqwz.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zlq.pycfn.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dgx.fanxiaobao.xyz

TS:   同 JS
来源：http://aop.yueranfly.top

Java: 方法内为块级作用域
来源：http://xix.daxiang520.top

Go:   花括号块级作用域
来源：http://tsg.shzxlz.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cpp.ctjpmb.com

C#:   块级作用域
来源：http://xdu.c1oappe.top

[C11] 模块导入与导出
来源：http://tmg.jinyuanbaomall.cn

Py:   from module import func
来源：http://vrg.ybcxt.top

PHP:  require "file.php";  或 use App\Service;
来源：http://axq.pycfn.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://aez.xingfuxueyuan.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pex.xingfuxueyuan.xyz

Java: import java.util.List;
来源：http://hkv.yonumen.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rbq.yanxiufei.cn

Ruby: require "json"; require_relative "./util"
来源：http://gzx.fanxiaobao.xyz

C#:   using System.Text;
来源：http://jgu.shanyushiyangkeji.top

[C12] 立即执行函数 IIFE
来源：http://dup.andypj.xyz

Py:   (lambda: print("run"))()
来源：http://fcv.jinqigufen.top

PHP:  (function () { echo "run"; })();
来源：http://qzb.jinqigfzy.top

JS:   (() => { console.log("run"); })();
来源：http://zqz.chenjidiqi.icu

TS:   (() => { console.log("run"); })();
来源：http://jrq.fengsongda.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qsy.aibaodan.cn

Go:   func() { fmt.Println("run") }()
来源：http://sev.yvedp.cn

Ruby: -> { puts "run" }.call
来源：http://yqe.ywan-chungtsiang.top

C#:   // 无 IIFE：用静态构造函数
来源：http://key.guannengcc.top

[C13] 类型声明 / 类型注解
来源：http://hpc.xziqi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://buu.haohaochexian.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lsc.snrcjt.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bff.zhiwuduotai.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xvy.mhx1999.top

Java: int add(int a, int b) { return a + b; }
来源：http://tcc.mhx1999.top

Go:   func add(a, b int) int
来源：http://llc.tianlin.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ebc.yanxiufei.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ddk.fktsv.cn

[C14] 泛型函数
来源：http://sge.316326.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ggh.vqdsnc.cn

PHP:  // 无泛型
来源：http://etx.fanxiaobao.xyz

JS:   // 无泛型
来源：http://oub.zdbjq.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kxj.yongpay.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kpb.jinqigufen.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gvo.zhijiandao.cn

Ruby: # 无泛型
来源：http://qyk.tanke756.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xgy.kuanghao11.cn

[C15] 解构 / 展开参数
来源：http://ysd.yj20258888.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fyw.bjfxy.top

PHP:  [$a, $b] = $pair;
来源：http://ctx.birdmap.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fur.xinyue.icu

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fdu.yanxiufei.cn

Java: // 无解构
来源：http://gux.cashguo.top

Go:   // 无解构
来源：http://dln.chenlongwang.top

Ruby: a, b = pair
来源：http://ldl.uphjek.com

C#:   var (a, b) = pair;
来源：http://gud.zdbjq.cn

[C16] 函数 / 方法重载
来源：http://yny.yanxiufei.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ytr.sufxvd.cn

PHP:  // 无重载
来源：http://suw.zhoulong.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://ydi.yuanzhike.top

TS:   // 用联合类型或重载签名声明
来源：http://vtt.hywenlv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dcn.ydzc1.top

Go:   // 无重载：用不同函数名
来源：http://ihi.ywan-chungtsiang.top

Ruby: # 无重载：靠动态参数
来源：http://jug.jinyuanbaomall.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://uds.shanyushiyangkeji.top

================================================================================
来源：http://fcc.wangshuangyany.cn

D. 数组 / 列表 / 集合
来源：http://otd.pycfn.com

================================================================================
来源：http://krs.jinghuilouyu.cn

[D01] 创建数组 / 列表
来源：http://bjn.guannengcc.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://nbq.yanxiufei.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ebt.cqqwz.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://imq.cqqwz.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://iqa.cdnleiting.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lqs.chenjidiqi.icu

Go:   arr := []int{1, 2, 3}
来源：http://suj.zycfv.cn

Ruby: arr = [1, 2, 3]
来源：http://bgy.hcnkem.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ndh.vqdsnc.cn

[D02] 追加元素到末尾
来源：http://qxi.sjlbkw.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mnn.shanyushiyangkeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ija.hesvh.cn

JS:   arr.push(4);
来源：http://gwv.zhixingplan.top

TS:   arr.push(4);
来源：http://qlk.shanyushiyangkeji.top

Java: list.add(4);
来源：http://qio.smart0.xyz

Go:   arr = append(arr, 4)
来源：http://nte.yangfankeji.com

Ruby: arr << 4; arr.push(5)
来源：http://tkv.yangfankeji.com

C#:   list.Add(4);
来源：http://fbw.fehbvm.com

[D03] 在指定位置插入元素
来源：http://eok.shangyingyoupin.top

Py:   arr.insert(0, 0)
来源：http://dpk.aizwys.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://amq.yfazqb.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wur.iojbl.cn

TS:   arr.splice(0, 0, 0);
来源：http://lko.kuanghao11.cn

Java: list.add(0, 0);
来源：http://fba.zhoulong.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://xhy.ehwqpu.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mqi.snrcjt.cn

C#:   list.Insert(0, 0);
来源：http://mct.shuidangran.top

[D04] 删除元素
来源：http://eoy.xziqi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wac.bbcook.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tgr.fzhhl.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://eye.ydjk.org.cn

TS:   arr.splice(0, 1);
来源：http://epi.bbcook.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ujs.shanyushiyangtech.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mve.sxryk.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ibv.jinghuilouyu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zwm.birdmap.top

[D05] 访问与修改元素
来源：http://mnp.xingfuxueyuan.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://afo.jinyuanbaomall.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://iif.shuidangran.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ago.havefunace.top

TS:   arr[0]; arr.at(-1);
来源：http://qzp.redwolf501.top

Java: list.get(0); list.set(0, 9);
来源：http://ody.vehdjk.com

Go:   arr[0]; arr[0] = 9
来源：http://kui.yfazqb.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dej.zycfv.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qki.c1oappe.top

[D06] 数组长度
来源：http://bsz.tian-w.cn

Py:   len(arr)
来源：http://ggn.hammf.cn

PHP:  count($arr);
来源：http://lqr.hysaishi.cn

JS:   arr.length
来源：http://uaz.bbcook.cn

TS:   arr.length
来源：http://mww.guowangkeji.top

Java: list.size();
来源：http://elc.andypj.xyz

Go:   len(arr)
来源：http://cgu.fktsv.cn

Ruby: arr.length; arr.size
来源：http://pfx.tarul.cn

C#:   list.Count;
来源：http://eim.jqgufenzy.top

[D07] 切片 / 取子数组
来源：http://nnl.daxiang520.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://soa.tanke756.top

PHP:  array_slice($arr, 1, 3);
来源：http://ydj.snrcjt.cn

JS:   arr.slice(1, 4);
来源：http://ncv.ydjk.org.cn

TS:   arr.slice(1, 4);
来源：http://tiq.tianlin.xyz

Java: list.subList(1, 4);
来源：http://hhm.jiagoushi.top

Go:   arr[1:4]
来源：http://rum.jinqigfzy.top

Ruby: arr[1, 3]
来源：http://nxm.fktsv.cn

C#:   list.GetRange(1, 3);
来源：http://ewd.zhixingplan.top

[D08] 合并两个数组
来源：http://jyv.hammf.cn

Py:   a + b;  a.extend(b)
来源：http://xum.jinqigufen.top

PHP:  array_merge($a, $b);
来源：http://kra.hysaishi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://tob.tanke756.top

TS:   [...a, ...b];
来源：http://ezj.havefunace.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bbj.ydzc1.top

Go:   append(a, b...)
来源：http://ptl.jiagoushi.top

Ruby: a + b;  a.concat(b)
来源：http://def.hesvh.cn

C#:   a.Concat(b).ToList()
来源：http://ket.dashuyun.cn

[D09] 排序（升序）
来源：http://aee.yongpay.top

Py:   sorted(arr);  arr.sort()
来源：http://fzb.quarkkingdee.top

PHP:  sort($arr);
来源：http://uzr.redwolf501.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lng.yuanzhike.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://pxd.dashuyun.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://dwz.andypj.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://goj.cqqwz.cn

Ruby: arr.sort
来源：http://bzy.yangfankeji.com

C#:   list.Sort();
来源：http://wbs.yongpay.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://pwm.tanke756.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ohr.aizwys.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uem.mhx1999.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pxs.aizwys.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ekt.snrcjt.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ihr.shanyushiyangkeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cep.nanxinkj.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mgk.nanxuanxn.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uhl.aizwys.cn

[D11] 反转数组
来源：http://jws.tarul.cn

Py:   arr[::-1];  arr.reverse()
来源：http://boj.9152youxi.cn

PHP:  array_reverse($arr);
来源：http://tob.uphjek.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ftf.gzhubu.top

TS:   [...arr].reverse();
来源：http://ndp.yanxiufei.cn

Java: Collections.reverse(list);
来源：http://myg.uphjek.com

Go:   slices.Reverse(arr)
来源：http://pwe.haohaochexian.top

Ruby: arr.reverse
来源：http://ohj.shanyushiyangtech.top

C#:   list.Reverse();
来源：http://tbe.mhx1999.top

[D12] 查找元素下标
来源：http://ogp.zycfv.cn

Py:   arr.index(x);  x in arr
来源：http://vqh.wangdashe.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nsb.hnxiangtu.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ymm.ybcxt.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xwy.pengpengdd.cyou

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tjx.zhengqikj.top

Go:   slices.Index(arr, x)
来源：http://sek.cdnleiting.top

Ruby: arr.index(x)
来源：http://trs.shanyushiyangtech.top

C#:   list.IndexOf(x);
来源：http://pss.jinghuilouyu.cn

[D13] 过滤（保留满足条件的）
来源：http://jvv.xziqi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qzx.jlsjyb.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://opb.feifeiyinyue.top

JS:   arr.filter(x => x > 3)
来源：http://ywz.fktsv.cn

TS:   arr.filter(x => x > 3)
来源：http://xfc.shanyushiyangkeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://koe.52xcode.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hmr.zhongyouzk.top

Ruby: arr.select { |x| x > 3 }
来源：http://pkd.fktsv.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://awf.hywenlv.cn

[D14] 映射转换（每个元素变形）
来源：http://hye.hfpthk.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hij.tianlin.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yho.52xcode.cn

JS:   arr.map(x => x * 2)
来源：http://tez.hesvh.cn

TS:   arr.map(x => x * 2)
来源：http://xxy.mhx1999.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://dze.yangfankeji.com

Go:   // 手写循环
来源：http://tqo.daxiang520.top

Ruby: arr.map { |x| x * 2 }
来源：http://jxz.316326.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://ayt.fanxiaobao.xyz

[D15] 去重
来源：http://lyo.zhoulong.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://esl.aizwys.cn

PHP:  array_unique($arr);
来源：http://rnp.uphjek.com

JS:   [...new Set(arr)]
来源：http://zsr.yangfankeji.com

TS:   [...new Set(arr)]
来源：http://cee.yfazqb.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yrp.xylfe.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lzi.yuxming.cn

Ruby: arr.uniq
来源：http://qey.dianchejie.cn

C#:   list.Distinct().ToList()
来源：http://mut.dashuyun.cn

[D16] 求和与平均值
来源：http://yoe.fengsongda.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kih.epnwcf.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sjc.ydzc1.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dun.jinqigfzy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://san.jlsjyb.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jok.nanxinkj.top

Go:   // 手写循环累加
来源：http://hes.shangyingyoupin.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fek.sysykeji.top

C#:   list.Sum();  list.Average()
来源：http://qjy.hcnkem.com

[D17] 最大值与最小值
来源：http://bxs.feifeiyinyue.top

Py:   max(arr);  min(arr)
来源：http://lzq.0kj1m.cn

PHP:  max($arr);  min($arr);
来源：http://gll.zhoulong.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lgn.meibo888.top

TS:   Math.max(...arr);
来源：http://nih.dashuyun.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mkc.aizwys.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qqm.shuidangran.top

Ruby: arr.max;  arr.min
来源：http://imt.hesvh.cn

C#:   list.Max();  list.Min()
来源：http://znq.yj20258888.top

[D18] 扁平化嵌套数组
来源：http://asj.yvedp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xgv.cucudq.cn

PHP:  array_merge(...$nested);
来源：http://ykx.fzhhl.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lth.xinyue.icu

TS:   nested.flat();
来源：http://xhz.ehwqpu.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zkf.dianchejie.cn

Go:   // 手写双层循环
来源：http://tvr.jinqigfzy.top

Ruby: nested.flatten
来源：http://avi.ywan-chungtsiang.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://jwn.nanxuanxn.top

[D19] 按字段分组
来源：http://kur.zhixingplan.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cir.guowangkeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ytp.andypj.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jgg.yj20258.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://qez.tianlin.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ygy.shanyushiyangtech.top

Go:   // 手写 map[string][]T
来源：http://jjv.wangdashe.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://lyh.tian-w.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xhx.jyoumei.cn

[D20] 统计每个元素出现次数
来源：http://jej.yj202588.top

Py:   Counter(arr)
来源：http://wrg.sweek.top

PHP:  array_count_values($arr);
来源：http://xen.xziqi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://snn.ctjpmb.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zex.xylfe.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://oyh.vehdjk.com

Go:   // 手写 map[T]int
来源：http://ueq.xingfuxueyuan.xyz

Ruby: arr.tally
来源：http://rxx.jyoumei.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://otx.jianghu66.top

[D21] 判断是否包含某元素
来源：http://zhb.nwbrower.top

Py:   x in arr
来源：http://pnp.sxryk.cn

PHP:  in_array($x, $arr, true);
来源：http://sih.cheryme.top

JS:   arr.includes(x)
来源：http://ycv.jqgfzy.top

TS:   arr.includes(x)
来源：http://nfq.sysykeji.top

Java: list.contains(x)
来源：http://xbo.yuanzhike.top

Go:   slices.Contains(arr, x)
来源：http://kkd.bjfxy.top

Ruby: arr.include?(x)
来源：http://igx.jinyuanbaomall.cn

C#:   list.Contains(x)
来源：http://zju.yangfankeji.com

[D22] 复制数组（避免共享引用）
来源：http://ame.pycfn.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cbj.yj20258.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xyn.hcnkem.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xzp.zdbjq.cn

TS:   [...arr];
来源：http://lzb.zhongyouzk.top

Java: new ArrayList<>(list);
来源：http://ydr.wangdashe.top

Go:   copied := append([]int(nil), arr...)
来源：http://sdd.jinghuilouyu.cn

Ruby: arr.dup;  arr.clone
来源：http://gks.yangfankeji.com

C#:   new List<int>(list);
来源：http://hdn.yj20258.top

[D23] reduce 累积计算
来源：http://qpv.quarkkingdee.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://euo.tianlin.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mtp.yuanzhike.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://chh.pengpengdd.cyou

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gov.birdmap.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ggn.sufxvd.cn

Go:   // 手写循环
来源：http://wpp.fanxiaobao.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bew.hnxiangtu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tgh.aibaodan.cn

[D24] 字典 / Map 基本操作
来源：http://ayb.quarkkingdee.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kxs.52xcode.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rjd.hammf.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cfz.sufxvd.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://plq.xuanzx.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://poj.ivvv.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jcc.ydjk.org.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://aoh.pycfn.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kog.zhongyouzk.top

[D25] Set 集合去重与交并差
来源：http://ewq.ydjk.org.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ejv.xinyue.icu

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wln.jinghuilouyu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mam.fengsongda.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nfo.zhixingplan.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tjc.tarul.cn


<!-- 参考信息 -->