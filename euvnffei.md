代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://epr.52xcode.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ooh.sxryk.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qzh.haohaochexian.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ebm.sysykeji.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fjo.yueranfly.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hiy.yonumen.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gmi.quarkkingdee.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://djl.yanxiufei.cn

[C10] 变量作用域
来源：http://ybe.bjfxy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jlx.shuidangran.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jtg.sysykeji.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://puz.xuetiantiany.cn

TS:   同 JS
来源：http://gny.dashuyun.cn

Java: 方法内为块级作用域
来源：http://nhq.yfazqb.com

Go:   花括号块级作用域
来源：http://cnx.fktsv.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://afd.wangdashe.top

C#:   块级作用域
来源：http://uyw.ybcxt.top

[C11] 模块导入与导出
来源：http://yvr.sweek.top

Py:   from module import func
来源：http://myl.zhaomingkeji.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://vpn.chenlongwang.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://gzl.ctjpmb.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uzv.nwbrower.top

Java: import java.util.List;
来源：http://kwi.yonumen.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hzw.zhixingplan.top

Ruby: require "json"; require_relative "./util"
来源：http://qnk.jianghu66.top

C#:   using System.Text;
来源：http://fht.fanxiaobao.xyz

[C12] 立即执行函数 IIFE
来源：http://kne.shuidangran.top

Py:   (lambda: print("run"))()
来源：http://rmf.shanyushiyangkeji.top

PHP:  (function () { echo "run"; })();
来源：http://vuh.sufxvd.cn

JS:   (() => { console.log("run"); })();
来源：http://mno.hywenlv.cn

TS:   (() => { console.log("run"); })();
来源：http://ltf.chenlongwang.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bjh.sufxvd.cn

Go:   func() { fmt.Println("run") }()
来源：http://ifk.cdnleiting.top

Ruby: -> { puts "run" }.call
来源：http://sux.ppjwa.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://tmj.sxryk.cn

[C13] 类型声明 / 类型注解
来源：http://vra.ybcxt.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://otg.jlsjyb.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://efw.yueranfly.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rtq.haohaochexian.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xjj.jyoumei.cn

Java: int add(int a, int b) { return a + b; }
来源：http://bbj.hnqzz.top

Go:   func add(a, b int) int
来源：http://zub.yvedp.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tht.gotoacloud.top

C#:   int Add(int a, int b) => a + b;
来源：http://aue.jinghuilouyu.cn

[C14] 泛型函数
来源：http://ols.316326.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mut.fzhhl.top

PHP:  // 无泛型
来源：http://gfu.hongshengwenyu.top

JS:   // 无泛型
来源：http://npt.0kj1m.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ifp.zhiwuduotai.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rpd.sweek.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fwa.ywan-chungtsiang.top

Ruby: # 无泛型
来源：http://mvb.sjlbkw.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://izd.zhengqikj.top

[C15] 解构 / 展开参数
来源：http://rja.chenjidiqi.icu

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ztq.yonumen.top

PHP:  [$a, $b] = $pair;
来源：http://hlv.yj20258.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jbk.nanxinkj.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://oao.birdmap.top

Java: // 无解构
来源：http://bry.ctjpmb.com

Go:   // 无解构
来源：http://jny.quarkkingdee.top

Ruby: a, b = pair
来源：http://ncf.jinqigufen.top

C#:   var (a, b) = pair;
来源：http://hil.hysaishi.cn

[C16] 函数 / 方法重载
来源：http://sgc.cucudq.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mij.sjlbkw.cn

PHP:  // 无重载
来源：http://azj.gogol.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://pos.yueranfly.top

TS:   // 用联合类型或重载签名声明
来源：http://muk.gaohongyu789.top

Java: void f(int a) {}  void f(String a) {}
来源：http://jjt.daria6918.cn

Go:   // 无重载：用不同函数名
来源：http://yha.nwbrower.top

Ruby: # 无重载：靠动态参数
来源：http://yzk.fktsv.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://plh.kuanghao11.cn

================================================================================
来源：http://app.gzhubu.top

D. 数组 / 列表 / 集合
来源：http://wmn.vqdsnc.cn

================================================================================
来源：http://mmf.zhijiandao.cn

[D01] 创建数组 / 列表
来源：http://wfp.feifeiyinyue.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://xqu.ydzc1.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wde.fktsv.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bty.zhaomingkeji.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://cuh.wangdashe.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fop.sxryk.cn

Go:   arr := []int{1, 2, 3}
来源：http://gqb.xuanzx.com

Ruby: arr = [1, 2, 3]
来源：http://ucy.dianchejie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pgt.gotoacloud.top

[D02] 追加元素到末尾
来源：http://qjp.pengpengdd.cyou

Py:   arr.append(4); arr.extend([5, 6])
来源：http://php.xingfuxueyuan.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://orn.sweek.top

JS:   arr.push(4);
来源：http://xyd.bbcook.cn

TS:   arr.push(4);
来源：http://cnf.zhaomingkeji.xyz

Java: list.add(4);
来源：http://zyi.cashguo.top

Go:   arr = append(arr, 4)
来源：http://mea.zhengqikj.top

Ruby: arr << 4; arr.push(5)
来源：http://xqh.yongpay.top

C#:   list.Add(4);
来源：http://fim.xylfe.cn

[D03] 在指定位置插入元素
来源：http://ugm.zhaomingkeji.xyz

Py:   arr.insert(0, 0)
来源：http://dhy.chenlongwang.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nan.yj20258.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wko.shanyushiyangtech.top

TS:   arr.splice(0, 0, 0);
来源：http://qnf.ybcxt.top

Java: list.add(0, 0);
来源：http://qvo.hongshengwenyu.top

Go:   arr = append([]int{0}, arr...)
来源：http://lyr.yongpay.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jzi.snrcjt.cn

C#:   list.Insert(0, 0);
来源：http://hcy.jinyuanbaomall.cn

[D04] 删除元素
来源：http://nks.chenjidiqi.icu

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xov.pengpengdd.cyou

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fee.wangdashe.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xji.smart0.xyz

TS:   arr.splice(0, 1);
来源：http://nbh.jinqigfzy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qht.chenlongwang.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vtx.tianlin.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xzy.cheryme.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nyp.xinyue.icu

[D05] 访问与修改元素
来源：http://bhv.aibaodan.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yph.shangyingyoupin.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xhk.cqqwz.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lyy.fanxiaobao.xyz

TS:   arr[0]; arr.at(-1);
来源：http://bca.cdnleiting.top

Java: list.get(0); list.set(0, 9);
来源：http://vyk.zhongyouzk.top

Go:   arr[0]; arr[0] = 9
来源：http://ikj.hywenlv.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kop.sjlbkw.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fta.guannengcc.top

[D06] 数组长度
来源：http://ocz.fanxiaobao.xyz

Py:   len(arr)
来源：http://zsi.yvedp.cn

PHP:  count($arr);
来源：http://hhz.0kj1m.cn

JS:   arr.length
来源：http://ffs.guannengcc.top

TS:   arr.length
来源：http://lxb.jinqigufen.top

Java: list.size();
来源：http://ihp.jiagoushi.top

Go:   len(arr)
来源：http://kul.yongpay.top

Ruby: arr.length; arr.size
来源：http://jnx.shzxlz.cn

C#:   list.Count;
来源：http://wxp.ybcxt.top

[D07] 切片 / 取子数组
来源：http://eox.jqgufenzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qeq.nanxuanxn.top

PHP:  array_slice($arr, 1, 3);
来源：http://yde.nwbrower.top

JS:   arr.slice(1, 4);
来源：http://img.chenlongwang.top

TS:   arr.slice(1, 4);
来源：http://qlr.yangfankeji.com

Java: list.subList(1, 4);
来源：http://tru.sysykeji.top

Go:   arr[1:4]
来源：http://teq.yj202588.top

Ruby: arr[1, 3]
来源：http://esg.xziqi.cn

C#:   list.GetRange(1, 3);
来源：http://ypw.hongshengwenyu.top

[D08] 合并两个数组
来源：http://ufd.xylfe.cn

Py:   a + b;  a.extend(b)
来源：http://byi.xuanzx.com

PHP:  array_merge($a, $b);
来源：http://xib.yj20258.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wxo.xziqi.cn

TS:   [...a, ...b];
来源：http://ntx.jinyuanbaomall.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://voi.zdqjudy.top

Go:   append(a, b...)
来源：http://ckk.ppjwa.cn

Ruby: a + b;  a.concat(b)
来源：http://oja.hammf.cn

C#:   a.Concat(b).ToList()
来源：http://pis.cucudq.cn

[D09] 排序（升序）
来源：http://otb.sweek.top

Py:   sorted(arr);  arr.sort()
来源：http://idq.hfpthk.cn

PHP:  sort($arr);
来源：http://gji.epnwcf.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://iwq.bbcook.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wcx.bjfxy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://hdr.yuanzhike.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mgy.gaohongyu789.top

Ruby: arr.sort
来源：http://waf.ctjpmb.com

C#:   list.Sort();
来源：http://fta.snrcjt.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://oxx.gzhubu.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sbf.yonumen.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mdi.smart0.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jfd.ehwqpu.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xil.tarul.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pfg.yuanzhike.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ize.quarkkingdee.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pip.9152youxi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tdb.ctjpmb.com

[D11] 反转数组
来源：http://dsg.snrcjt.cn

Py:   arr[::-1];  arr.reverse()
来源：http://fqx.hfpthk.cn

PHP:  array_reverse($arr);
来源：http://omc.52xcode.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nqv.c1oappe.top

TS:   [...arr].reverse();
来源：http://rjq.andypj.xyz

Java: Collections.reverse(list);
来源：http://khf.jinqigufen.top

Go:   slices.Reverse(arr)
来源：http://gls.cashguo.top

Ruby: arr.reverse
来源：http://zcw.wangshuangyany.cn

C#:   list.Reverse();
来源：http://icq.cashguo.top

[D12] 查找元素下标
来源：http://dpg.aizwys.cn

Py:   arr.index(x);  x in arr
来源：http://mvw.yfazqb.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pvt.tanke756.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pgd.chenzaomai.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lvl.yfazqb.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mqe.yj20258888.top

Go:   slices.Index(arr, x)
来源：http://lsw.gogol.net.cn

Ruby: arr.index(x)
来源：http://zyv.andypj.xyz

C#:   list.IndexOf(x);
来源：http://qxe.ctjpmb.com

[D13] 过滤（保留满足条件的）
来源：http://onw.epnwcf.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lwk.jinyuanbaomall.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hiy.shanyushiyangkeji.top

JS:   arr.filter(x => x > 3)
来源：http://mti.zdbjq.cn

TS:   arr.filter(x => x > 3)
来源：http://dxe.fengsongda.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rlc.gotoacloud.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ojh.gotoacloud.top

Ruby: arr.select { |x| x > 3 }
来源：http://kdt.fengsongda.top

C#:   list.Where(x => x > 3).ToList()
来源：http://zte.chenzaomai.com

[D14] 映射转换（每个元素变形）
来源：http://zwp.9152youxi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zot.hnqzz.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vzx.jinyuanbaomall.cn

JS:   arr.map(x => x * 2)
来源：http://qwg.bjfxy.top

TS:   arr.map(x => x * 2)
来源：http://tcn.haohaochexian.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://efb.sxryk.cn

Go:   // 手写循环
来源：http://qzs.bbcook.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bel.52xcode.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://end.ehwqpu.com

[D15] 去重
来源：http://joc.yj20258.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://iji.ppjwa.cn

PHP:  array_unique($arr);
来源：http://onv.jinyuanbaomall.cn

JS:   [...new Set(arr)]
来源：http://rbp.cheryme.top

TS:   [...new Set(arr)]
来源：http://jhn.aibaodan.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mmy.svipenyu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://mmj.bjfxy.top

Ruby: arr.uniq
来源：http://wnb.52xcode.cn

C#:   list.Distinct().ToList()
来源：http://jaw.feifeiyinyue.top

[D16] 求和与平均值
来源：http://sri.sweek.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xha.shangyingyoupin.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ayl.316326.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://syv.zhijiandao.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cgx.snrcjt.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://iep.aizwys.cn

Go:   // 手写循环累加
来源：http://oqv.zhoulong.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vmr.sxryk.cn

C#:   list.Sum();  list.Average()
来源：http://btz.hammf.cn

[D17] 最大值与最小值
来源：http://qpc.yvedp.cn

Py:   max(arr);  min(arr)
来源：http://rrw.pycfn.com

PHP:  max($arr);  min($arr);
来源：http://euz.quarkkingdee.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://abe.52xcode.cn

TS:   Math.max(...arr);
来源：http://cxg.zhoulong.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://rkx.52xcode.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://azj.yj20258.top

Ruby: arr.max;  arr.min
来源：http://ick.yonumen.top

C#:   list.Max();  list.Min()
来源：http://kyi.yanxiufei.cn

[D18] 扁平化嵌套数组
来源：http://peb.pycfn.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lfe.andypj.xyz

PHP:  array_merge(...$nested);
来源：http://pru.daxiang520.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qjf.sysykeji.top

TS:   nested.flat();
来源：http://fpm.hesvh.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://uer.pycfn.com

Go:   // 手写双层循环
来源：http://lgd.xinyue.icu

Ruby: nested.flatten
来源：http://esl.gzhubu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ugw.hesvh.cn

[D19] 按字段分组
来源：http://snj.gogol.net.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fej.dianchejie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mwi.meibo888.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qof.hnqzz.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://mwo.yueranfly.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dgn.hongshengwenyu.top

Go:   // 手写 map[string][]T
来源：http://upz.redwolf501.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://gkc.316326.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ytw.yfazqb.com

[D20] 统计每个元素出现次数
来源：http://fus.0kj1m.cn

Py:   Counter(arr)
来源：http://cgp.quarkkingdee.top

PHP:  array_count_values($arr);
来源：http://ojw.yonumen.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cvt.xuetiantiany.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qxk.jinyuanbaomall.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hkr.yueranfly.top

Go:   // 手写 map[T]int
来源：http://rih.guannengcc.top

Ruby: arr.tally
来源：http://ckh.fktsv.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://oec.0kj1m.cn

[D21] 判断是否包含某元素
来源：http://fov.jiagoushi.top

Py:   x in arr
来源：http://nyr.bjfxy.top

PHP:  in_array($x, $arr, true);
来源：http://kpx.52xcode.cn

JS:   arr.includes(x)
来源：http://ctb.vqdsnc.cn

TS:   arr.includes(x)
来源：http://yji.hammf.cn

Java: list.contains(x)
来源：http://yco.yongpay.top

Go:   slices.Contains(arr, x)
来源：http://lti.sufxvd.cn

Ruby: arr.include?(x)
来源：http://kvx.tanke756.top

C#:   list.Contains(x)
来源：http://cdf.shanyushiyangtech.top

[D22] 复制数组（避免共享引用）
来源：http://ysj.tianlin.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lgq.52xcode.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://exr.chenzaomai.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://joy.havefunace.top

TS:   [...arr];
来源：http://jpp.hesvh.cn

Java: new ArrayList<>(list);
来源：http://wxx.fanxiaobao.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://ask.jlsjyb.cn

Ruby: arr.dup;  arr.clone
来源：http://azl.guannengcc.top

C#:   new List<int>(list);
来源：http://hnq.smart0.xyz

[D23] reduce 累积计算
来源：http://qan.daria6918.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://eur.nwbrower.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cuo.zdbjq.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sxr.mhx1999.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nwp.dianchejie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ttw.jianghu66.top

Go:   // 手写循环
来源：http://vaj.svipenyu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://odg.ydzc1.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bgy.hfpthk.cn

[D24] 字典 / Map 基本操作
来源：http://rfm.cheryme.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ior.chenlongwang.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ycc.hongshengwenyu.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hkt.aizwys.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bjk.aibaodan.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lrj.aibaodan.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://otc.xuetiantiany.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://okl.sxryk.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sbd.guannengcc.top

[D25] Set 集合去重与交并差
来源：http://ehe.xingfuxueyuan.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ruf.tianlin.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xad.jyoumei.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://uyc.zhoulong.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vel.ybcxt.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://okx.cqqwz.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qsh.316326.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://for.feifeiyinyue.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jzj.jyoumei.cn

[D26] 数组转字符串
来源：http://pxq.hnxiangtu.top


<!-- 参考信息 -->