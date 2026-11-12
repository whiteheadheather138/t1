代发 wailian999

[C10] 变量作用域
来源：http://vmq.yonumen.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cai.wangshuangyany.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zjz.chenlongwang.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dmv.vehdjk.com

TS:   同 JS
来源：http://fvp.guowangkeji.top

Java: 方法内为块级作用域
来源：http://hak.ydjk.org.cn

Go:   花括号块级作用域
来源：http://abc.gaohongyu789.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dfp.shanyushiyangkeji.top

C#:   块级作用域
来源：http://had.sufxvd.cn

[C11] 模块导入与导出
来源：http://ymc.shangyingyoupin.top

Py:   from module import func
来源：http://hng.uphjek.com

PHP:  require "file.php";  或 use App\Service;
来源：http://rfm.ppjwa.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jsl.daxiang520.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ffh.sjlbkw.cn

Java: import java.util.List;
来源：http://xld.fktsv.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mkz.snrcjt.cn

Ruby: require "json"; require_relative "./util"
来源：http://wcz.feifeiyinyue.top

C#:   using System.Text;
来源：http://hao.316326.xyz

[C12] 立即执行函数 IIFE
来源：http://suy.zhaomingkeji.xyz

Py:   (lambda: print("run"))()
来源：http://cuj.gogol.net.cn

PHP:  (function () { echo "run"; })();
来源：http://fyh.xingfuxueyuan.xyz

JS:   (() => { console.log("run"); })();
来源：http://qbp.ehwqpu.com

TS:   (() => { console.log("run"); })();
来源：http://pgi.gotoacloud.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rhd.nanxinkj.top

Go:   func() { fmt.Println("run") }()
来源：http://rur.daria6918.cn

Ruby: -> { puts "run" }.call
来源：http://yjc.pengpengdd.cyou

C#:   // 无 IIFE：用静态构造函数
来源：http://kpy.havefunace.top

[C13] 类型声明 / 类型注解
来源：http://inw.shzxlz.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zez.haohaochexian.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://evh.shzxlz.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gfx.jinqigfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zef.zhongyouzk.top

Java: int add(int a, int b) { return a + b; }
来源：http://vob.daxiang520.top

Go:   func add(a, b int) int
来源：http://ocr.havefunace.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://skl.sufxvd.cn

C#:   int Add(int a, int b) => a + b;
来源：http://smk.xingfuxueyuan.xyz

[C14] 泛型函数
来源：http://wsg.sxryk.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wxw.c1oappe.top

PHP:  // 无泛型
来源：http://tpm.yueranfly.top

JS:   // 无泛型
来源：http://dtg.zhiwuduotai.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://alf.wangshuangyany.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pby.zhixingplan.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xgj.zhixingplan.top

Ruby: # 无泛型
来源：http://lbx.quarkkingdee.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gxa.hongshengwenyu.top

[C15] 解构 / 展开参数
来源：http://fmz.epnwcf.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://znf.hcnkem.com

PHP:  [$a, $b] = $pair;
来源：http://kzv.feifeiyinyue.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://iea.yangfankeji.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xlt.snrcjt.cn

Java: // 无解构
来源：http://aqj.zhengqikj.top

Go:   // 无解构
来源：http://cla.ybcxt.top

Ruby: a, b = pair
来源：http://bww.jlsjyb.cn

C#:   var (a, b) = pair;
来源：http://pwq.zhijiandao.cn

[C16] 函数 / 方法重载
来源：http://aqq.jlsjyb.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://obc.shangyingyoupin.top

PHP:  // 无重载
来源：http://ucy.wangdashe.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://vsc.sjlbkw.cn

TS:   // 用联合类型或重载签名声明
来源：http://wci.shuidangran.top

Java: void f(int a) {}  void f(String a) {}
来源：http://dnk.fktsv.cn

Go:   // 无重载：用不同函数名
来源：http://uan.c1oappe.top

Ruby: # 无重载：靠动态参数
来源：http://qdq.chenzaomai.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://hjm.xziqi.cn

================================================================================
来源：http://sok.jinghuilouyu.cn

D. 数组 / 列表 / 集合
来源：http://yrf.gotoacloud.top

================================================================================
来源：http://rar.tianlin.xyz

[D01] 创建数组 / 列表
来源：http://huv.yvedp.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://sua.zdqjudy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ktj.zdqjudy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ryq.hnxiangtu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ish.kuanghao11.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ffe.yangfankeji.com

Go:   arr := []int{1, 2, 3}
来源：http://tar.aibaodan.cn

Ruby: arr = [1, 2, 3]
来源：http://myr.vehdjk.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dmy.guannengcc.top

[D02] 追加元素到末尾
来源：http://skk.hammf.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ydd.chenzaomai.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xwn.daxiang520.top

JS:   arr.push(4);
来源：http://psg.nwbrower.top

TS:   arr.push(4);
来源：http://isv.shanyushiyangtech.top

Java: list.add(4);
来源：http://tls.gzhubu.top

Go:   arr = append(arr, 4)
来源：http://rms.jqgufenzy.top

Ruby: arr << 4; arr.push(5)
来源：http://oab.xylfe.cn

C#:   list.Add(4);
来源：http://asr.ybcxt.top

[D03] 在指定位置插入元素
来源：http://mrr.hnxiangtu.top

Py:   arr.insert(0, 0)
来源：http://yfg.bjfxy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nax.nwbrower.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jui.hnxiangtu.top

TS:   arr.splice(0, 0, 0);
来源：http://yth.redwolf501.top

Java: list.add(0, 0);
来源：http://yqe.vehdjk.com

Go:   arr = append([]int{0}, arr...)
来源：http://zum.cqqwz.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kap.jiagoushi.top

C#:   list.Insert(0, 0);
来源：http://elx.hnxiangtu.top

[D04] 删除元素
来源：http://rlf.cqqwz.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rbc.chenzaomai.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mpk.guowangkeji.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xwl.jinghuilouyu.cn

TS:   arr.splice(0, 1);
来源：http://zfj.gogol.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wcn.uphjek.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qwf.aizwys.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://onn.daxiang520.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lwp.fengsongda.top

[D05] 访问与修改元素
来源：http://huy.wangdashe.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yrb.cdnleiting.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gim.hongshengwenyu.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rst.quarkkingdee.top

TS:   arr[0]; arr.at(-1);
来源：http://qjn.yfazqb.com

Java: list.get(0); list.set(0, 9);
来源：http://pso.hnqzz.top

Go:   arr[0]; arr[0] = 9
来源：http://bla.bjfxy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ocz.hnqzz.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vho.aibaodan.cn

[D06] 数组长度
来源：http://rib.316326.xyz

Py:   len(arr)
来源：http://ecr.fanxiaobao.xyz

PHP:  count($arr);
来源：http://eaq.jianghu66.top

JS:   arr.length
来源：http://nab.jiagoushi.top

TS:   arr.length
来源：http://yji.gaohongyu789.top

Java: list.size();
来源：http://ipb.zhoulong.xyz

Go:   len(arr)
来源：http://opi.fanxiaobao.xyz

Ruby: arr.length; arr.size
来源：http://hpu.hesvh.cn

C#:   list.Count;
来源：http://cen.gogol.net.cn

[D07] 切片 / 取子数组
来源：http://sfy.cheryme.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://doj.hammf.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hrb.cqqwz.cn

JS:   arr.slice(1, 4);
来源：http://crm.tarul.cn

TS:   arr.slice(1, 4);
来源：http://nyd.cucudq.cn

Java: list.subList(1, 4);
来源：http://fba.cucudq.cn

Go:   arr[1:4]
来源：http://znk.chenjidiqi.icu

Ruby: arr[1, 3]
来源：http://pzo.dashuyun.cn

C#:   list.GetRange(1, 3);
来源：http://mmq.fzhhl.top

[D08] 合并两个数组
来源：http://zmj.haohaochexian.top

Py:   a + b;  a.extend(b)
来源：http://tvx.shanyushiyangtech.top

PHP:  array_merge($a, $b);
来源：http://nuo.nanxinkj.top

JS:   [...a, ...b];  a.concat(b);
来源：http://kjt.xinyue.icu

TS:   [...a, ...b];
来源：http://wjn.guowangkeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sef.sxryk.cn

Go:   append(a, b...)
来源：http://nci.yvedp.cn

Ruby: a + b;  a.concat(b)
来源：http://mmu.guannengcc.top

C#:   a.Concat(b).ToList()
来源：http://rbg.yj20258888.top

[D09] 排序（升序）
来源：http://ufu.fzhhl.top

Py:   sorted(arr);  arr.sort()
来源：http://qoi.zhixingplan.top

PHP:  sort($arr);
来源：http://qeu.9152youxi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qth.yj202588.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://lkr.tian-w.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wci.tianlin.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://amt.tarul.cn

Ruby: arr.sort
来源：http://yxf.hammf.cn

C#:   list.Sort();
来源：http://pyv.haohaochexian.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://wko.yuxming.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pxa.yj20258888.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dzo.c1oappe.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://iim.svipenyu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kgu.yangfankeji.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ppq.vehdjk.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ufd.mhx1999.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ban.jinghuilouyu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lbq.hnxiangtu.top

[D11] 反转数组
来源：http://wmt.tian-w.cn

Py:   arr[::-1];  arr.reverse()
来源：http://oac.guowangkeji.top

PHP:  array_reverse($arr);
来源：http://jdd.nanxinkj.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wte.yangfankeji.com

TS:   [...arr].reverse();
来源：http://edi.hywenlv.cn

Java: Collections.reverse(list);
来源：http://esf.xingfuxueyuan.xyz

Go:   slices.Reverse(arr)
来源：http://fxq.chenzaomai.com

Ruby: arr.reverse
来源：http://odu.xinyue.icu

C#:   list.Reverse();
来源：http://jtk.pengpengdd.cyou

[D12] 查找元素下标
来源：http://htt.yonumen.top

Py:   arr.index(x);  x in arr
来源：http://ewa.yj202588.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lrq.jinghuilouyu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nvo.guowangkeji.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qwl.wangshuangyany.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://arm.zhengqikj.top

Go:   slices.Index(arr, x)
来源：http://dmw.zhixingplan.top

Ruby: arr.index(x)
来源：http://pfy.epnwcf.com

C#:   list.IndexOf(x);
来源：http://ygi.hesvh.cn

[D13] 过滤（保留满足条件的）
来源：http://zty.bbcook.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nww.cucudq.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mke.sysykeji.top

JS:   arr.filter(x => x > 3)
来源：http://dlv.ctjpmb.com

TS:   arr.filter(x => x > 3)
来源：http://vrw.ppjwa.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cbl.jqgufenzy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ypn.hfpthk.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qql.xuetiantiany.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wmb.jinghuilouyu.cn

[D14] 映射转换（每个元素变形）
来源：http://avo.sjlbkw.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rai.zhoulong.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://skq.fengsongda.top

JS:   arr.map(x => x * 2)
来源：http://wvu.zhaomingkeji.xyz

TS:   arr.map(x => x * 2)
来源：http://rdq.jqgufenzy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://xfl.xingfuxueyuan.xyz

Go:   // 手写循环
来源：http://cze.xinyue.icu

Ruby: arr.map { |x| x * 2 }
来源：http://pbk.sjlbkw.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://egh.pengpengdd.cyou

[D15] 去重
来源：http://qjo.shuidangran.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://eol.yuanzhike.top

PHP:  array_unique($arr);
来源：http://pak.zdbjq.cn

JS:   [...new Set(arr)]
来源：http://rvy.hongshengwenyu.top

TS:   [...new Set(arr)]
来源：http://eqr.jinghuilouyu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xoi.ctjpmb.com

Go:   // 用 map[T]struct{} 手写
来源：http://qqg.yonumen.top

Ruby: arr.uniq
来源：http://dhh.havefunace.top

C#:   list.Distinct().ToList()
来源：http://jgg.ybcxt.top

[D16] 求和与平均值
来源：http://mwz.yj20258.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gis.zhongyouzk.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xpu.yanxiufei.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rvk.fanxiaobao.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sff.aizwys.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ydo.kuanghao11.cn

Go:   // 手写循环累加
来源：http://fve.jlsjyb.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://llv.jianghu66.top

C#:   list.Sum();  list.Average()
来源：http://sgc.wangshuangyany.cn

[D17] 最大值与最小值
来源：http://xfa.wangshuangyany.cn

Py:   max(arr);  min(arr)
来源：http://zlp.nwbrower.top

PHP:  max($arr);  min($arr);
来源：http://lau.zhoulong.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bkr.ivvv.top

TS:   Math.max(...arr);
来源：http://yft.c1oappe.top

Java: Collections.max(list);  Collections.min(list);
来源：http://col.yj20258.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jff.dashuyun.cn

Ruby: arr.max;  arr.min
来源：http://dxb.svipenyu.cn

C#:   list.Max();  list.Min()
来源：http://orw.zhaomingkeji.xyz

[D18] 扁平化嵌套数组
来源：http://wnd.gzhubu.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dfy.nanxuanxn.top

PHP:  array_merge(...$nested);
来源：http://nja.fehbvm.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://iwn.ehwqpu.com

TS:   nested.flat();
来源：http://ydm.xinyue.icu

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tal.hywenlv.cn

Go:   // 手写双层循环
来源：http://ejs.zdbjq.cn

Ruby: nested.flatten
来源：http://zlr.bjfxy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://bsn.gzhubu.top

[D19] 按字段分组
来源：http://wvw.shanyushiyangtech.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qxj.hcnkem.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mqc.havefunace.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pod.zhiwuduotai.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://aos.guannengcc.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mla.hnxiangtu.top

Go:   // 手写 map[string][]T
来源：http://jdd.ctjpmb.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://fpo.xuetiantiany.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zhd.zhengqikj.top

[D20] 统计每个元素出现次数
来源：http://unu.iojbl.cn

Py:   Counter(arr)
来源：http://vhr.ppjwa.cn

PHP:  array_count_values($arr);
来源：http://aaa.zhongyouzk.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ekg.fzhhl.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hlz.fehbvm.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xqy.yonumen.top

Go:   // 手写 map[T]int
来源：http://hkp.fengsongda.top

Ruby: arr.tally
来源：http://aex.ybcxt.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://izn.daria6918.cn

[D21] 判断是否包含某元素
来源：http://mus.shangyingyoupin.top

Py:   x in arr
来源：http://har.shanyushiyangtech.top

PHP:  in_array($x, $arr, true);
来源：http://ugd.bbcook.cn

JS:   arr.includes(x)
来源：http://cii.gaohongyu789.top

TS:   arr.includes(x)
来源：http://ijl.wangshuangyany.cn

Java: list.contains(x)
来源：http://zqf.yuxming.cn

Go:   slices.Contains(arr, x)
来源：http://tnx.guannengcc.top

Ruby: arr.include?(x)
来源：http://eqg.zdbjq.cn

C#:   list.Contains(x)
来源：http://ejo.cheryme.top

[D22] 复制数组（避免共享引用）
来源：http://gdq.sweek.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://axd.gzhubu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xoi.yuxming.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pmd.guannengcc.top

TS:   [...arr];
来源：http://owz.hcnkem.com

Java: new ArrayList<>(list);
来源：http://auv.sjlbkw.cn

Go:   copied := append([]int(nil), arr...)
来源：http://sqe.jinghuilouyu.cn

Ruby: arr.dup;  arr.clone
来源：http://fti.yj20258888.top

C#:   new List<int>(list);
来源：http://otc.haohaochexian.top

[D23] reduce 累积计算
来源：http://qsd.fzhhl.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://uaw.jqgfzy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ize.yvedp.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ndt.sysykeji.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ncu.fehbvm.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://kez.gotoacloud.top

Go:   // 手写循环
来源：http://pll.zhaomingkeji.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://smn.vehdjk.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wxh.guowangkeji.top

[D24] 字典 / Map 基本操作
来源：http://bhl.sufxvd.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mfk.svipenyu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hpf.tian-w.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://spa.zdbjq.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jen.guannengcc.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://grz.shanyushiyangtech.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ioj.jinqigufen.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ube.jinqigufen.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kqx.redwolf501.top

[D25] Set 集合去重与交并差
来源：http://fbo.wangdashe.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jgv.shanyushiyangtech.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sad.cheryme.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kvi.xziqi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ays.jqgufenzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yef.yueranfly.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xnm.ctjpmb.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ker.yonumen.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ana.jinqigufen.top

[D26] 数组转字符串
来源：http://tmo.gotoacloud.top

Py:   ", ".join(map(str, arr))
来源：http://jaq.tianlin.xyz

PHP:  implode(", ", $arr);
来源：http://ohg.yuanzhike.top

JS:   arr.join(", ")
来源：http://nwn.nanxinkj.top

TS:   arr.join(", ")
来源：http://iqu.9152youxi.cn

Java: String.join(", ", list)
来源：http://ndz.sysykeji.top

Go:   strings.Join(strs, ", ")
来源：http://dek.fehbvm.com

Ruby: arr.join(", ")
来源：http://hke.gaohongyu789.top

C#:   string.Join(", ", list)
来源：http://rip.redwolf501.top


<!-- 参考信息 -->