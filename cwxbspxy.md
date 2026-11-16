代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qls.xinyue.icu

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wlo.guowangkeji.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wsz.iojbl.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ups.bjfxy.top

[C10] 变量作用域
来源：http://rzl.bjfxy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xay.sjlbkw.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xda.jyoumei.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nqj.jinqigfzy.top

TS:   同 JS
来源：http://cvt.c1oappe.top

Java: 方法内为块级作用域
来源：http://lqh.dashuyun.cn

Go:   花括号块级作用域
来源：http://hqn.hammf.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://the.xuanzx.com

C#:   块级作用域
来源：http://rjj.xinyue.icu

[C11] 模块导入与导出
来源：http://sky.c1oappe.top

Py:   from module import func
来源：http://qvi.0kj1m.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://agn.cucudq.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zog.epnwcf.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hal.wangshuangyany.cn

Java: import java.util.List;
来源：http://fwk.yonumen.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://svs.zhiwuduotai.top

Ruby: require "json"; require_relative "./util"
来源：http://hci.hnxiangtu.top

C#:   using System.Text;
来源：http://gtd.zhixingplan.top

[C12] 立即执行函数 IIFE
来源：http://nbr.wangdashe.top

Py:   (lambda: print("run"))()
来源：http://zsk.svipenyu.cn

PHP:  (function () { echo "run"; })();
来源：http://iwo.fengsongda.top

JS:   (() => { console.log("run"); })();
来源：http://inx.guannengcc.top

TS:   (() => { console.log("run"); })();
来源：http://jow.ppjwa.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bvb.quarkkingdee.top

Go:   func() { fmt.Println("run") }()
来源：http://oeb.dashuyun.cn

Ruby: -> { puts "run" }.call
来源：http://pvk.fzhhl.top

C#:   // 无 IIFE：用静态构造函数
来源：http://tud.yuanzhike.top

[C13] 类型声明 / 类型注解
来源：http://qoi.zhiwuduotai.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tld.xziqi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wkh.xuetiantiany.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://etg.guowangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jze.vqdsnc.cn

Java: int add(int a, int b) { return a + b; }
来源：http://bwt.yj20258.top

Go:   func add(a, b int) int
来源：http://qfr.tanke756.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qoi.jinqigufen.top

C#:   int Add(int a, int b) => a + b;
来源：http://ixl.chenjidiqi.icu

[C14] 泛型函数
来源：http://zao.yanxiufei.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qzk.smart0.xyz

PHP:  // 无泛型
来源：http://fso.jinghuilouyu.cn

JS:   // 无泛型
来源：http://uvi.jiagoushi.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://abq.vehdjk.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gtw.hfpthk.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tcf.pengpengdd.cyou

Ruby: # 无泛型
来源：http://oac.zhongyouzk.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zcx.9152youxi.cn

[C15] 解构 / 展开参数
来源：http://lzf.haohaochexian.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pfb.shanyushiyangkeji.top

PHP:  [$a, $b] = $pair;
来源：http://vbw.nanxuanxn.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kdv.jinyuanbaomall.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nwt.yanxiufei.cn

Java: // 无解构
来源：http://sey.yuanzhike.top

Go:   // 无解构
来源：http://jfh.smart0.xyz

Ruby: a, b = pair
来源：http://qzr.cqqwz.cn

C#:   var (a, b) = pair;
来源：http://pcp.xylfe.cn

[C16] 函数 / 方法重载
来源：http://txs.chenjidiqi.icu

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zwg.zdqjudy.top

PHP:  // 无重载
来源：http://xzb.cdnleiting.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://dqa.jinghuilouyu.cn

TS:   // 用联合类型或重载签名声明
来源：http://ydl.epnwcf.com

Java: void f(int a) {}  void f(String a) {}
来源：http://gwk.pengpengdd.cyou

Go:   // 无重载：用不同函数名
来源：http://vmw.shanyushiyangkeji.top

Ruby: # 无重载：靠动态参数
来源：http://rmb.chenjidiqi.icu

C#:   void F(int a) {}  void F(string a) {}
来源：http://ppq.zhongyouzk.top

================================================================================
来源：http://qpm.zhaomingkeji.xyz

D. 数组 / 列表 / 集合
来源：http://eox.yanxiufei.cn

================================================================================
来源：http://cuo.aizwys.cn

[D01] 创建数组 / 列表
来源：http://yyo.fengsongda.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://gid.gzhubu.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yhx.ydzc1.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cph.gotoacloud.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://sxz.gaohongyu789.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://iai.wangdashe.top

Go:   arr := []int{1, 2, 3}
来源：http://qzu.wangshuangyany.cn

Ruby: arr = [1, 2, 3]
来源：http://vqx.snrcjt.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gxj.bjfxy.top

[D02] 追加元素到末尾
来源：http://csl.shuidangran.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qck.ydzc1.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jcc.vqdsnc.cn

JS:   arr.push(4);
来源：http://tvz.bjfxy.top

TS:   arr.push(4);
来源：http://iih.jinghuilouyu.cn

Java: list.add(4);
来源：http://tkw.shuidangran.top

Go:   arr = append(arr, 4)
来源：http://ucu.fzhhl.top

Ruby: arr << 4; arr.push(5)
来源：http://jxq.xuanzx.com

C#:   list.Add(4);
来源：http://rng.pengpengdd.cyou

[D03] 在指定位置插入元素
来源：http://nyt.gzhubu.top

Py:   arr.insert(0, 0)
来源：http://nim.zhongyouzk.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://iqe.epnwcf.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://igt.jiagoushi.top

TS:   arr.splice(0, 0, 0);
来源：http://uzd.yangfankeji.com

Java: list.add(0, 0);
来源：http://few.guannengcc.top

Go:   arr = append([]int{0}, arr...)
来源：http://kor.bjfxy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cps.yongpay.top

C#:   list.Insert(0, 0);
来源：http://ggl.jinqigufen.top

[D04] 删除元素
来源：http://nsw.zdqjudy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qfs.yj20258.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kzj.316326.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qmg.chenlongwang.top

TS:   arr.splice(0, 1);
来源：http://dcr.hesvh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jih.shanyushiyangtech.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jhz.sysykeji.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://opt.hfpthk.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zda.quarkkingdee.top

[D05] 访问与修改元素
来源：http://qhl.xylfe.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rrq.chenjidiqi.icu

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://oul.quarkkingdee.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fht.birdmap.top

TS:   arr[0]; arr.at(-1);
来源：http://yzb.ehwqpu.com

Java: list.get(0); list.set(0, 9);
来源：http://zxs.zdqjudy.top

Go:   arr[0]; arr[0] = 9
来源：http://knv.fengsongda.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tun.zhixingplan.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xor.sjlbkw.cn

[D06] 数组长度
来源：http://axn.gzhubu.top

Py:   len(arr)
来源：http://vbi.jqgufenzy.top

PHP:  count($arr);
来源：http://esl.dashuyun.cn

JS:   arr.length
来源：http://hlg.yj20258888.top

TS:   arr.length
来源：http://lra.cqqwz.cn

Java: list.size();
来源：http://rgs.birdmap.top

Go:   len(arr)
来源：http://odv.wangdashe.top

Ruby: arr.length; arr.size
来源：http://jce.gogol.net.cn

C#:   list.Count;
来源：http://qvu.tarul.cn

[D07] 切片 / 取子数组
来源：http://fqy.redwolf501.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hpj.gaohongyu789.top

PHP:  array_slice($arr, 1, 3);
来源：http://fbg.zdqjudy.top

JS:   arr.slice(1, 4);
来源：http://mqx.vqdsnc.cn

TS:   arr.slice(1, 4);
来源：http://wep.wangshuangyany.cn

Java: list.subList(1, 4);
来源：http://lpf.9152youxi.cn

Go:   arr[1:4]
来源：http://xda.cheryme.top

Ruby: arr[1, 3]
来源：http://ovd.yj202588.top

C#:   list.GetRange(1, 3);
来源：http://baf.zdqjudy.top

[D08] 合并两个数组
来源：http://gez.feifeiyinyue.top

Py:   a + b;  a.extend(b)
来源：http://yau.guowangkeji.top

PHP:  array_merge($a, $b);
来源：http://xfm.snrcjt.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hsj.xziqi.cn

TS:   [...a, ...b];
来源：http://ekg.chenzaomai.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tkr.daxiang520.top

Go:   append(a, b...)
来源：http://giq.vqdsnc.cn

Ruby: a + b;  a.concat(b)
来源：http://cgl.chenzaomai.com

C#:   a.Concat(b).ToList()
来源：http://gla.epnwcf.com

[D09] 排序（升序）
来源：http://cyf.gzhubu.top

Py:   sorted(arr);  arr.sort()
来源：http://cez.bjfxy.top

PHP:  sort($arr);
来源：http://htj.ybcxt.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zsj.meibo888.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://lss.kuanghao11.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://lkf.iojbl.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hxv.zycfv.cn

Ruby: arr.sort
来源：http://vii.jinqigufen.top

C#:   list.Sort();
来源：http://eoh.sxryk.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://idf.fktsv.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ika.cdnleiting.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://axg.bbcook.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mpp.jinqigfzy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fhb.ctjpmb.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mpv.yangfankeji.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lsa.hfpthk.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fyy.zdqjudy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rrs.pycfn.com

[D11] 反转数组
来源：http://tnf.sjlbkw.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ucc.wangdashe.top

PHP:  array_reverse($arr);
来源：http://gpm.quarkkingdee.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mwg.shanyushiyangtech.top

TS:   [...arr].reverse();
来源：http://sbp.andypj.xyz

Java: Collections.reverse(list);
来源：http://lmo.shanyushiyangkeji.top

Go:   slices.Reverse(arr)
来源：http://zmt.xziqi.cn

Ruby: arr.reverse
来源：http://vea.xingfuxueyuan.xyz

C#:   list.Reverse();
来源：http://vne.ydzc1.top

[D12] 查找元素下标
来源：http://lwe.cqqwz.cn

Py:   arr.index(x);  x in arr
来源：http://cvq.zycfv.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://guy.uphjek.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ogx.hesvh.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rmb.xingfuxueyuan.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uxp.zhongyouzk.top

Go:   slices.Index(arr, x)
来源：http://qjd.ppjwa.cn

Ruby: arr.index(x)
来源：http://xoq.kuanghao11.cn

C#:   list.IndexOf(x);
来源：http://woe.dashuyun.cn

[D13] 过滤（保留满足条件的）
来源：http://wbv.guannengcc.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kla.tarul.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gwd.shanyushiyangkeji.top

JS:   arr.filter(x => x > 3)
来源：http://cpc.haohaochexian.top

TS:   arr.filter(x => x > 3)
来源：http://yol.hysaishi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lbv.jyoumei.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xlq.yanxiufei.cn

Ruby: arr.select { |x| x > 3 }
来源：http://rtv.nanxuanxn.top

C#:   list.Where(x => x > 3).ToList()
来源：http://yon.uphjek.com

[D14] 映射转换（每个元素变形）
来源：http://nia.snrcjt.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yig.zhoulong.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tse.zhijiandao.cn

JS:   arr.map(x => x * 2)
来源：http://ekq.zhaomingkeji.xyz

TS:   arr.map(x => x * 2)
来源：http://ewi.wangshuangyany.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://fbh.ydjk.org.cn

Go:   // 手写循环
来源：http://guf.yj202588.top

Ruby: arr.map { |x| x * 2 }
来源：http://sni.sjlbkw.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sra.hammf.cn

[D15] 去重
来源：http://elu.ydjk.org.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://amn.ctjpmb.com

PHP:  array_unique($arr);
来源：http://pti.aizwys.cn

JS:   [...new Set(arr)]
来源：http://pnw.tian-w.cn

TS:   [...new Set(arr)]
来源：http://noc.daxiang520.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ebc.jianghu66.top

Go:   // 用 map[T]struct{} 手写
来源：http://qff.jyoumei.cn

Ruby: arr.uniq
来源：http://bmp.sysykeji.top

C#:   list.Distinct().ToList()
来源：http://xcq.guannengcc.top

[D16] 求和与平均值
来源：http://vzp.chenjidiqi.icu

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qkl.chenjidiqi.icu

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gwm.wangshuangyany.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dtu.guowangkeji.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://oaj.quarkkingdee.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ppk.dashuyun.cn

Go:   // 手写循环累加
来源：http://bkg.fktsv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vyk.sjlbkw.cn

C#:   list.Sum();  list.Average()
来源：http://sli.yuanzhike.top

[D17] 最大值与最小值
来源：http://vkg.tian-w.cn

Py:   max(arr);  min(arr)
来源：http://hsg.ybcxt.top

PHP:  max($arr);  min($arr);
来源：http://szs.tianlin.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rzw.zhengqikj.top

TS:   Math.max(...arr);
来源：http://heo.cqqwz.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://txm.smart0.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://flg.yanxiufei.cn

Ruby: arr.max;  arr.min
来源：http://fje.ppjwa.cn

C#:   list.Max();  list.Min()
来源：http://rnt.hnxiangtu.top

[D18] 扁平化嵌套数组
来源：http://zkt.sweek.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tfq.fengsongda.top

PHP:  array_merge(...$nested);
来源：http://fen.cashguo.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uph.zhaomingkeji.xyz

TS:   nested.flat();
来源：http://psq.sjlbkw.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://uqv.gotoacloud.top

Go:   // 手写双层循环
来源：http://dmg.sweek.top

Ruby: nested.flatten
来源：http://jxs.ywan-chungtsiang.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://pij.mhx1999.top

[D19] 按字段分组
来源：http://vok.fehbvm.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ztg.ctjpmb.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zfh.dashuyun.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hex.dianchejie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://mig.xziqi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cqj.daxiang520.top

Go:   // 手写 map[string][]T
来源：http://cmo.yangfankeji.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://cha.iojbl.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://atd.zhongyouzk.top

[D20] 统计每个元素出现次数
来源：http://xiq.yfazqb.com

Py:   Counter(arr)
来源：http://nds.gogol.net.cn

PHP:  array_count_values($arr);
来源：http://ngb.mhx1999.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iay.zhixingplan.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vrb.andypj.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://joe.shanyushiyangtech.top

Go:   // 手写 map[T]int
来源：http://tev.sweek.top

Ruby: arr.tally
来源：http://hrj.yongpay.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ojf.zhixingplan.top

[D21] 判断是否包含某元素
来源：http://cdt.jinqigfzy.top

Py:   x in arr
来源：http://aut.gogol.net.cn

PHP:  in_array($x, $arr, true);
来源：http://vmh.yvedp.cn

JS:   arr.includes(x)
来源：http://qig.zhiwuduotai.top

TS:   arr.includes(x)
来源：http://gty.0kj1m.cn

Java: list.contains(x)
来源：http://tml.yuanzhike.top

Go:   slices.Contains(arr, x)
来源：http://bfk.jiagoushi.top

Ruby: arr.include?(x)
来源：http://cfd.meibo888.top

C#:   list.Contains(x)
来源：http://fdf.yj202588.top

[D22] 复制数组（避免共享引用）
来源：http://olw.jinqigfzy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sku.xziqi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zqd.yonumen.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://irz.cdnleiting.top

TS:   [...arr];
来源：http://sak.chenlongwang.top

Java: new ArrayList<>(list);
来源：http://rrr.epnwcf.com

Go:   copied := append([]int(nil), arr...)
来源：http://xqn.yj20258.top

Ruby: arr.dup;  arr.clone
来源：http://xhp.pycfn.com

C#:   new List<int>(list);
来源：http://wsv.snrcjt.cn

[D23] reduce 累积计算
来源：http://gvg.ehwqpu.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zvr.sufxvd.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kby.fzhhl.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://axm.dianchejie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://efw.9152youxi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dqw.fengsongda.top

Go:   // 手写循环
来源：http://bei.sysykeji.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rzx.tanke756.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://icm.hysaishi.cn

[D24] 字典 / Map 基本操作
来源：http://hdd.svipenyu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tec.zhongyouzk.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cke.haohaochexian.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rcq.hnxiangtu.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gqf.jyoumei.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gqb.jianghu66.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://neh.bjfxy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jwp.ivvv.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rlk.shanyushiyangkeji.top

[D25] Set 集合去重与交并差
来源：http://vpo.epnwcf.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://apo.bjfxy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jwb.ywan-chungtsiang.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gpo.gzhubu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xjh.vehdjk.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://oyi.svipenyu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cas.jinqigufen.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ydi.vqdsnc.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ygl.ydzc1.top

[D26] 数组转字符串
来源：http://vvn.jiagoushi.top

Py:   ", ".join(map(str, arr))
来源：http://xbz.jlsjyb.cn

PHP:  implode(", ", $arr);
来源：http://fje.xylfe.cn

JS:   arr.join(", ")
来源：http://jkz.cdnleiting.top

TS:   arr.join(", ")
来源：http://mmx.birdmap.top


<!-- 参考信息 -->