代发 wailian999

TS:   同 JS
来源：http://mrg.snrcjt.cn

Java: 方法内为块级作用域
来源：http://bvd.daxiang520.top

Go:   花括号块级作用域
来源：http://qnq.sysykeji.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kai.jqgufenzy.top

C#:   块级作用域
来源：http://wyy.zhijiandao.cn

[C11] 模块导入与导出
来源：http://hkq.zhengqikj.top

Py:   from module import func
来源：http://hna.yuanzhike.top

PHP:  require "file.php";  或 use App\Service;
来源：http://org.shzxlz.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ntr.kuanghao11.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ztv.hongshengwenyu.top

Java: import java.util.List;
来源：http://pqa.gaohongyu789.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wyu.jinqigufen.top

Ruby: require "json"; require_relative "./util"
来源：http://lmo.mhx1999.top

C#:   using System.Text;
来源：http://cym.nanxuanxn.top

[C12] 立即执行函数 IIFE
来源：http://ezw.hcnkem.com

Py:   (lambda: print("run"))()
来源：http://ojq.jianghu66.top

PHP:  (function () { echo "run"; })();
来源：http://gsp.jqgfzy.top

JS:   (() => { console.log("run"); })();
来源：http://sfv.hesvh.cn

TS:   (() => { console.log("run"); })();
来源：http://lia.jiagoushi.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://glz.xylfe.cn

Go:   func() { fmt.Println("run") }()
来源：http://jzb.redwolf501.top

Ruby: -> { puts "run" }.call
来源：http://igt.fzhhl.top

C#:   // 无 IIFE：用静态构造函数
来源：http://flx.hywenlv.cn

[C13] 类型声明 / 类型注解
来源：http://cuq.chenjidiqi.icu

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://amw.cucudq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://buq.daxiang520.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qvf.cashguo.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ylk.316326.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://gih.fanxiaobao.xyz

Go:   func add(a, b int) int
来源：http://acy.xingfuxueyuan.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yor.jianghu66.top

C#:   int Add(int a, int b) => a + b;
来源：http://pje.chenzaomai.com

[C14] 泛型函数
来源：http://ehs.dashuyun.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://apw.jianghu66.top

PHP:  // 无泛型
来源：http://xty.quarkkingdee.top

JS:   // 无泛型
来源：http://rdo.yonumen.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://eav.jinghuilouyu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lja.quarkkingdee.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lww.sxryk.cn

Ruby: # 无泛型
来源：http://elb.yanxiufei.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xsf.tianlin.xyz

[C15] 解构 / 展开参数
来源：http://xcl.guannengcc.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wot.jinghuilouyu.cn

PHP:  [$a, $b] = $pair;
来源：http://vct.zdqjudy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ptt.hysaishi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uzq.yueranfly.top

Java: // 无解构
来源：http://ubd.fzhhl.top

Go:   // 无解构
来源：http://szx.jinghuilouyu.cn

Ruby: a, b = pair
来源：http://ceh.vqdsnc.cn

C#:   var (a, b) = pair;
来源：http://nfs.zdbjq.cn

[C16] 函数 / 方法重载
来源：http://xel.316326.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nim.zhaomingkeji.xyz

PHP:  // 无重载
来源：http://lqs.hywenlv.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xjq.zhiwuduotai.top

TS:   // 用联合类型或重载签名声明
来源：http://lvc.jiagoushi.top

Java: void f(int a) {}  void f(String a) {}
来源：http://qht.haohaochexian.top

Go:   // 无重载：用不同函数名
来源：http://dhm.mhx1999.top

Ruby: # 无重载：靠动态参数
来源：http://fvb.nanxuanxn.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://bji.sweek.top

================================================================================
来源：http://ley.ywan-chungtsiang.top

D. 数组 / 列表 / 集合
来源：http://bnx.jiagoushi.top

================================================================================
来源：http://sxv.yvedp.cn

[D01] 创建数组 / 列表
来源：http://eys.yj20258.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://phz.jiagoushi.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qvv.hnqzz.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qda.sweek.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ffo.xuetiantiany.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rdw.cdnleiting.top

Go:   arr := []int{1, 2, 3}
来源：http://drs.smart0.xyz

Ruby: arr = [1, 2, 3]
来源：http://hzj.daxiang520.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fwq.pengpengdd.cyou

[D02] 追加元素到末尾
来源：http://aie.tanke756.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nvy.hysaishi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ddq.fzhhl.top

JS:   arr.push(4);
来源：http://xku.ehwqpu.com

TS:   arr.push(4);
来源：http://ncf.0kj1m.cn

Java: list.add(4);
来源：http://vai.yongpay.top

Go:   arr = append(arr, 4)
来源：http://csn.cdnleiting.top

Ruby: arr << 4; arr.push(5)
来源：http://svy.ppjwa.cn

C#:   list.Add(4);
来源：http://xoo.yuanzhike.top

[D03] 在指定位置插入元素
来源：http://zkn.hammf.cn

Py:   arr.insert(0, 0)
来源：http://nnh.yanxiufei.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rgc.tian-w.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lqt.tanke756.top

TS:   arr.splice(0, 0, 0);
来源：http://wjv.jyoumei.cn

Java: list.add(0, 0);
来源：http://fve.52xcode.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xsx.epnwcf.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cmn.zhaomingkeji.xyz

C#:   list.Insert(0, 0);
来源：http://huw.yj202588.top

[D04] 删除元素
来源：http://php.tianlin.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ckz.pycfn.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hea.xuanzx.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zza.jianghu66.top

TS:   arr.splice(0, 1);
来源：http://xxf.sxryk.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ebt.ydzc1.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fbj.gotoacloud.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yqq.sufxvd.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://csm.zdbjq.cn

[D05] 访问与修改元素
来源：http://wcf.svipenyu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qlb.zhiwuduotai.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lrz.hongshengwenyu.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vfn.daria6918.cn

TS:   arr[0]; arr.at(-1);
来源：http://riy.jinqigfzy.top

Java: list.get(0); list.set(0, 9);
来源：http://eno.zhongyouzk.top

Go:   arr[0]; arr[0] = 9
来源：http://ncv.ivvv.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nxp.yj202588.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ryy.0kj1m.cn

[D06] 数组长度
来源：http://rfy.shangyingyoupin.top

Py:   len(arr)
来源：http://nvp.yueranfly.top

PHP:  count($arr);
来源：http://dki.daria6918.cn

JS:   arr.length
来源：http://zjp.cqqwz.cn

TS:   arr.length
来源：http://wyf.xinyue.icu

Java: list.size();
来源：http://ayp.andypj.xyz

Go:   len(arr)
来源：http://csw.tianlin.xyz

Ruby: arr.length; arr.size
来源：http://grw.ctjpmb.com

C#:   list.Count;
来源：http://qth.snrcjt.cn

[D07] 切片 / 取子数组
来源：http://lwl.cheryme.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rzx.yangfankeji.com

PHP:  array_slice($arr, 1, 3);
来源：http://ieo.uphjek.com

JS:   arr.slice(1, 4);
来源：http://lyn.meibo888.top

TS:   arr.slice(1, 4);
来源：http://klc.aibaodan.cn

Java: list.subList(1, 4);
来源：http://tlo.wangdashe.top

Go:   arr[1:4]
来源：http://syj.yueranfly.top

Ruby: arr[1, 3]
来源：http://kaf.smart0.xyz

C#:   list.GetRange(1, 3);
来源：http://zhg.cashguo.top

[D08] 合并两个数组
来源：http://agr.fktsv.cn

Py:   a + b;  a.extend(b)
来源：http://bqm.jianghu66.top

PHP:  array_merge($a, $b);
来源：http://nvj.jlsjyb.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kcb.kuanghao11.cn

TS:   [...a, ...b];
来源：http://jwp.havefunace.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dsq.jqgufenzy.top

Go:   append(a, b...)
来源：http://edu.fktsv.cn

Ruby: a + b;  a.concat(b)
来源：http://doy.yueranfly.top

C#:   a.Concat(b).ToList()
来源：http://nmr.fengsongda.top

[D09] 排序（升序）
来源：http://ytv.hysaishi.cn

Py:   sorted(arr);  arr.sort()
来源：http://yaq.ivvv.top

PHP:  sort($arr);
来源：http://aax.shanyushiyangkeji.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://iui.chenjidiqi.icu

TS:   [...arr].sort((x, y) => x - y);
来源：http://exi.0kj1m.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ohc.redwolf501.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://aaf.gogol.net.cn

Ruby: arr.sort
来源：http://hfw.yongpay.top

C#:   list.Sort();
来源：http://cej.ivvv.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://qrz.kuanghao11.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uzv.ydjk.org.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://twy.zhoulong.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fux.c1oappe.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pgw.meibo888.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gdr.bjfxy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yil.guowangkeji.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://utw.aibaodan.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qvf.zdbjq.cn

[D11] 反转数组
来源：http://vfj.cdnleiting.top

Py:   arr[::-1];  arr.reverse()
来源：http://lwn.jinqigfzy.top

PHP:  array_reverse($arr);
来源：http://kdj.jqgufenzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mom.shzxlz.cn

TS:   [...arr].reverse();
来源：http://dse.smart0.xyz

Java: Collections.reverse(list);
来源：http://ltm.ppjwa.cn

Go:   slices.Reverse(arr)
来源：http://hkr.shanyushiyangtech.top

Ruby: arr.reverse
来源：http://fqj.yonumen.top

C#:   list.Reverse();
来源：http://ipa.zhengqikj.top

[D12] 查找元素下标
来源：http://ykm.jyoumei.cn

Py:   arr.index(x);  x in arr
来源：http://wnt.zhiwuduotai.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zjk.pengpengdd.cyou

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kqw.yj202588.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nig.yueranfly.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qtf.zhiwuduotai.top

Go:   slices.Index(arr, x)
来源：http://uwv.xylfe.cn

Ruby: arr.index(x)
来源：http://xea.ppjwa.cn

C#:   list.IndexOf(x);
来源：http://pox.0kj1m.cn

[D13] 过滤（保留满足条件的）
来源：http://ngz.gaohongyu789.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://def.sysykeji.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lmg.tarul.cn

JS:   arr.filter(x => x > 3)
来源：http://vil.zhaomingkeji.xyz

TS:   arr.filter(x => x > 3)
来源：http://xff.zdqjudy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://djr.bjfxy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://idl.yongpay.top

Ruby: arr.select { |x| x > 3 }
来源：http://css.jinghuilouyu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://nkx.jiagoushi.top

[D14] 映射转换（每个元素变形）
来源：http://rwa.tianlin.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dqy.xinyue.icu

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://anf.vehdjk.com

JS:   arr.map(x => x * 2)
来源：http://qsg.wangdashe.top

TS:   arr.map(x => x * 2)
来源：http://rsq.smart0.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://rqx.sjlbkw.cn

Go:   // 手写循环
来源：http://qsy.gogol.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gpv.pengpengdd.cyou

C#:   list.Select(x => x * 2).ToList()
来源：http://bxj.zhijiandao.cn

[D15] 去重
来源：http://thy.epnwcf.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://umo.9152youxi.cn

PHP:  array_unique($arr);
来源：http://fik.ivvv.top

JS:   [...new Set(arr)]
来源：http://utk.xziqi.cn

TS:   [...new Set(arr)]
来源：http://lfi.hesvh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hqm.iojbl.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wgb.chenlongwang.top

Ruby: arr.uniq
来源：http://yeb.shuidangran.top

C#:   list.Distinct().ToList()
来源：http://rrc.jqgufenzy.top

[D16] 求和与平均值
来源：http://scp.xingfuxueyuan.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fmu.zhengqikj.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://epb.meibo888.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zxm.yj20258888.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mxb.xuanzx.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ciy.jianghu66.top

Go:   // 手写循环累加
来源：http://jaw.tianlin.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rso.tian-w.cn

C#:   list.Sum();  list.Average()
来源：http://eel.hnqzz.top

[D17] 最大值与最小值
来源：http://jfe.snrcjt.cn

Py:   max(arr);  min(arr)
来源：http://onn.hnxiangtu.top

PHP:  max($arr);  min($arr);
来源：http://hsi.smart0.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tiv.yanxiufei.cn

TS:   Math.max(...arr);
来源：http://emg.c1oappe.top

Java: Collections.max(list);  Collections.min(list);
来源：http://uws.zhaomingkeji.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rsa.vehdjk.com

Ruby: arr.max;  arr.min
来源：http://jlm.hammf.cn

C#:   list.Max();  list.Min()
来源：http://aje.aizwys.cn

[D18] 扁平化嵌套数组
来源：http://ccg.chenjidiqi.icu

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ekl.iojbl.cn

PHP:  array_merge(...$nested);
来源：http://nrt.jianghu66.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://orw.zhaomingkeji.xyz

TS:   nested.flat();
来源：http://ucn.meibo888.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jqx.yuxming.cn

Go:   // 手写双层循环
来源：http://ezm.chenzaomai.com

Ruby: nested.flatten
来源：http://aeo.hywenlv.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://cjx.redwolf501.top

[D19] 按字段分组
来源：http://vwk.0kj1m.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xfb.feifeiyinyue.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://asw.bbcook.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gfv.cucudq.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hgo.xuetiantiany.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://shh.ywan-chungtsiang.top

Go:   // 手写 map[string][]T
来源：http://ofw.52xcode.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://xtm.yangfankeji.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qni.havefunace.top

[D20] 统计每个元素出现次数
来源：http://tps.snrcjt.cn

Py:   Counter(arr)
来源：http://qnu.yj20258.top

PHP:  array_count_values($arr);
来源：http://uoq.xingfuxueyuan.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gwe.daxiang520.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qts.zdqjudy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fyf.zdqjudy.top

Go:   // 手写 map[T]int
来源：http://hyh.daxiang520.top

Ruby: arr.tally
来源：http://deg.sysykeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zuh.meibo888.top

[D21] 判断是否包含某元素
来源：http://rhn.bbcook.cn

Py:   x in arr
来源：http://tql.kuanghao11.cn

PHP:  in_array($x, $arr, true);
来源：http://aeh.snrcjt.cn

JS:   arr.includes(x)
来源：http://dtz.bjfxy.top

TS:   arr.includes(x)
来源：http://jye.smart0.xyz

Java: list.contains(x)
来源：http://kmz.dianchejie.cn

Go:   slices.Contains(arr, x)
来源：http://bgq.yuanzhike.top

Ruby: arr.include?(x)
来源：http://nfx.epnwcf.com

C#:   list.Contains(x)
来源：http://nxq.shanyushiyangkeji.top

[D22] 复制数组（避免共享引用）
来源：http://uoz.zhixingplan.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yym.yj20258888.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ewn.haohaochexian.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pdl.hongshengwenyu.top

TS:   [...arr];
来源：http://xut.hfpthk.cn

Java: new ArrayList<>(list);
来源：http://whl.cdnleiting.top

Go:   copied := append([]int(nil), arr...)
来源：http://ohg.yj20258.top

Ruby: arr.dup;  arr.clone
来源：http://dog.yj20258888.top

C#:   new List<int>(list);
来源：http://kla.chenzaomai.com

[D23] reduce 累积计算
来源：http://zwg.xinyue.icu

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ijj.c1oappe.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rdj.yj202588.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dks.c1oappe.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qaa.hongshengwenyu.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://src.meibo888.top

Go:   // 手写循环
来源：http://anu.xziqi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yyv.epnwcf.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qtl.nanxinkj.top

[D24] 字典 / Map 基本操作
来源：http://dwm.hcnkem.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://taz.daria6918.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gys.ppjwa.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ths.shanyushiyangkeji.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vic.zdqjudy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fbv.jqgufenzy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vrn.havefunace.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tcs.fzhhl.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://atl.jqgufenzy.top

[D25] Set 集合去重与交并差
来源：http://dkk.havefunace.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://osi.sjlbkw.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hdf.zhixingplan.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pvv.aizwys.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ldv.quarkkingdee.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://knq.shanyushiyangkeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lft.yuanzhike.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pay.0kj1m.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rmb.bjfxy.top

[D26] 数组转字符串
来源：http://mox.jinghuilouyu.cn

Py:   ", ".join(map(str, arr))
来源：http://pqv.fzhhl.top

PHP:  implode(", ", $arr);
来源：http://wji.jiagoushi.top

JS:   arr.join(", ")
来源：http://njm.xingfuxueyuan.xyz

TS:   arr.join(", ")
来源：http://vma.ydjk.org.cn

Java: String.join(", ", list)
来源：http://nyq.jinqigfzy.top

Go:   strings.Join(strs, ", ")
来源：http://sua.cucudq.cn

Ruby: arr.join(", ")
来源：http://lhi.hcnkem.com

C#:   string.Join(", ", list)
来源：http://clj.hammf.cn

================================================================================
来源：http://xwh.birdmap.top

E. 字符串处理
来源：http://jea.svipenyu.cn

================================================================================
来源：http://cqe.chenzaomai.com

[E01] 拼接字符串
来源：http://ish.daria6918.cn


<!-- 参考信息 -->