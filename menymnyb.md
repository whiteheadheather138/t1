代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lxq.cqqwz.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://aqq.pengpengdd.cyou

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qkb.tian-w.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fqt.nanxinkj.top

[C10] 变量作用域
来源：http://ymp.guowangkeji.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zre.ivvv.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wxa.hammf.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rvy.yj202588.top

TS:   同 JS
来源：http://zab.wangdashe.top

Java: 方法内为块级作用域
来源：http://peg.zhiwuduotai.top

Go:   花括号块级作用域
来源：http://cke.chenlongwang.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gkk.zhaomingkeji.xyz

C#:   块级作用域
来源：http://udf.aibaodan.cn

[C11] 模块导入与导出
来源：http://caq.zhongyouzk.top

Py:   from module import func
来源：http://dfy.hywenlv.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mju.yanxiufei.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://cel.xylfe.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://chu.ppjwa.cn

Java: import java.util.List;
来源：http://eud.aizwys.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zkh.jinqigufen.top

Ruby: require "json"; require_relative "./util"
来源：http://uym.havefunace.top

C#:   using System.Text;
来源：http://bww.shangyingyoupin.top

[C12] 立即执行函数 IIFE
来源：http://mvp.zdqjudy.top

Py:   (lambda: print("run"))()
来源：http://sme.bjfxy.top

PHP:  (function () { echo "run"; })();
来源：http://umi.yj20258888.top

JS:   (() => { console.log("run"); })();
来源：http://pne.zycfv.cn

TS:   (() => { console.log("run"); })();
来源：http://ryf.yj202588.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kqj.ehwqpu.com

Go:   func() { fmt.Println("run") }()
来源：http://ssv.xylfe.cn

Ruby: -> { puts "run" }.call
来源：http://vqf.jyoumei.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ctf.dianchejie.cn

[C13] 类型声明 / 类型注解
来源：http://qrb.cucudq.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xbn.xziqi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ptv.pengpengdd.cyou

JS:   // 无类型（可用 JSDoc 注释）
来源：http://osz.havefunace.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kbz.c1oappe.top

Java: int add(int a, int b) { return a + b; }
来源：http://viq.uphjek.com

Go:   func add(a, b int) int
来源：http://aju.jinqigufen.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nbl.fehbvm.com

C#:   int Add(int a, int b) => a + b;
来源：http://sls.nwbrower.top

[C14] 泛型函数
来源：http://ncy.ydzc1.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wiw.nwbrower.top

PHP:  // 无泛型
来源：http://dhs.guowangkeji.top

JS:   // 无泛型
来源：http://tao.ydzc1.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jbz.yonumen.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wwd.nwbrower.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qgm.vehdjk.com

Ruby: # 无泛型
来源：http://wys.yj20258.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xvq.zhaomingkeji.xyz

[C15] 解构 / 展开参数
来源：http://rdk.yuanzhike.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cik.quarkkingdee.top

PHP:  [$a, $b] = $pair;
来源：http://qsi.fzhhl.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zrx.haohaochexian.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mra.yongpay.top

Java: // 无解构
来源：http://lfh.jqgfzy.top

Go:   // 无解构
来源：http://mqs.hcnkem.com

Ruby: a, b = pair
来源：http://rlo.sweek.top

C#:   var (a, b) = pair;
来源：http://pkp.jinqigfzy.top

[C16] 函数 / 方法重载
来源：http://mqr.sufxvd.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://unr.wangdashe.top

PHP:  // 无重载
来源：http://tce.nanxuanxn.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ebu.chenjidiqi.icu

TS:   // 用联合类型或重载签名声明
来源：http://mbb.xuetiantiany.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ufu.cdnleiting.top

Go:   // 无重载：用不同函数名
来源：http://lzv.zhaomingkeji.xyz

Ruby: # 无重载：靠动态参数
来源：http://ovg.chenlongwang.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://xat.tian-w.cn

================================================================================
来源：http://eef.ywan-chungtsiang.top

D. 数组 / 列表 / 集合
来源：http://bhq.smart0.xyz

================================================================================
来源：http://udl.jlsjyb.cn

[D01] 创建数组 / 列表
来源：http://dzj.havefunace.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://tjn.daxiang520.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://aiu.0kj1m.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pgy.zhijiandao.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://sbs.havefunace.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qpe.snrcjt.cn

Go:   arr := []int{1, 2, 3}
来源：http://rgr.yanxiufei.cn

Ruby: arr = [1, 2, 3]
来源：http://ktj.fengsongda.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://efj.tarul.cn

[D02] 追加元素到末尾
来源：http://wpk.yongpay.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vqd.havefunace.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jjv.andypj.xyz

JS:   arr.push(4);
来源：http://lfe.gotoacloud.top

TS:   arr.push(4);
来源：http://wyc.uphjek.com

Java: list.add(4);
来源：http://zld.snrcjt.cn

Go:   arr = append(arr, 4)
来源：http://jwo.yongpay.top

Ruby: arr << 4; arr.push(5)
来源：http://hec.fktsv.cn

C#:   list.Add(4);
来源：http://yrx.yuxming.cn

[D03] 在指定位置插入元素
来源：http://zus.0kj1m.cn

Py:   arr.insert(0, 0)
来源：http://nge.uphjek.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vnk.316326.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mvp.guannengcc.top

TS:   arr.splice(0, 0, 0);
来源：http://oye.ybcxt.top

Java: list.add(0, 0);
来源：http://max.gzhubu.top

Go:   arr = append([]int{0}, arr...)
来源：http://ezy.shanyushiyangtech.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bnf.jiagoushi.top

C#:   list.Insert(0, 0);
来源：http://cfq.zycfv.cn

[D04] 删除元素
来源：http://wcf.0kj1m.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tir.hysaishi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yya.ydjk.org.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://chs.jyoumei.cn

TS:   arr.splice(0, 1);
来源：http://fbl.jlsjyb.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://osa.cashguo.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qry.quarkkingdee.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://idg.hnqzz.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://aua.yueranfly.top

[D05] 访问与修改元素
来源：http://wgs.dashuyun.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ujx.xuetiantiany.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://imi.yuanzhike.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qhl.jqgfzy.top

TS:   arr[0]; arr.at(-1);
来源：http://yro.dashuyun.cn

Java: list.get(0); list.set(0, 9);
来源：http://oso.fanxiaobao.xyz

Go:   arr[0]; arr[0] = 9
来源：http://rcz.shuidangran.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ldl.fzhhl.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fht.yuanzhike.top

[D06] 数组长度
来源：http://lvd.mhx1999.top

Py:   len(arr)
来源：http://myg.gaohongyu789.top

PHP:  count($arr);
来源：http://aor.dashuyun.cn

JS:   arr.length
来源：http://cgu.jinghuilouyu.cn

TS:   arr.length
来源：http://rvr.pengpengdd.cyou

Java: list.size();
来源：http://zdg.fanxiaobao.xyz

Go:   len(arr)
来源：http://ufk.zdqjudy.top

Ruby: arr.length; arr.size
来源：http://dge.birdmap.top

C#:   list.Count;
来源：http://fwt.jinqigfzy.top

[D07] 切片 / 取子数组
来源：http://xxp.yanxiufei.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sln.svipenyu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ktq.ydjk.org.cn

JS:   arr.slice(1, 4);
来源：http://iwg.jinqigfzy.top

TS:   arr.slice(1, 4);
来源：http://ujf.wangshuangyany.cn

Java: list.subList(1, 4);
来源：http://ntj.fengsongda.top

Go:   arr[1:4]
来源：http://kho.ydjk.org.cn

Ruby: arr[1, 3]
来源：http://uiv.bbcook.cn

C#:   list.GetRange(1, 3);
来源：http://rlb.feifeiyinyue.top

[D08] 合并两个数组
来源：http://byu.jqgfzy.top

Py:   a + b;  a.extend(b)
来源：http://rkd.0kj1m.cn

PHP:  array_merge($a, $b);
来源：http://rip.hywenlv.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://dpv.haohaochexian.top

TS:   [...a, ...b];
来源：http://jen.gaohongyu789.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://eyz.yangfankeji.com

Go:   append(a, b...)
来源：http://ekp.yongpay.top

Ruby: a + b;  a.concat(b)
来源：http://bpo.svipenyu.cn

C#:   a.Concat(b).ToList()
来源：http://ofs.uphjek.com

[D09] 排序（升序）
来源：http://imn.shzxlz.cn

Py:   sorted(arr);  arr.sort()
来源：http://qbu.zhaomingkeji.xyz

PHP:  sort($arr);
来源：http://nya.hywenlv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wcj.yuanzhike.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ipt.yfazqb.com

Java: Collections.sort(list);  list.sort(null);
来源：http://qjr.zhiwuduotai.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vod.svipenyu.cn

Ruby: arr.sort
来源：http://hdf.gzhubu.top

C#:   list.Sort();
来源：http://aui.zdqjudy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://mld.shanyushiyangtech.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tlx.zhongyouzk.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qaq.yueranfly.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dns.yj20258888.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://plx.haohaochexian.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sni.yueranfly.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://maz.sufxvd.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ixz.zhixingplan.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ymm.uphjek.com

[D11] 反转数组
来源：http://vzl.fzhhl.top

Py:   arr[::-1];  arr.reverse()
来源：http://jlc.dashuyun.cn

PHP:  array_reverse($arr);
来源：http://azr.yanxiufei.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wkv.guowangkeji.top

TS:   [...arr].reverse();
来源：http://ogx.cashguo.top

Java: Collections.reverse(list);
来源：http://npf.fengsongda.top

Go:   slices.Reverse(arr)
来源：http://ijq.vqdsnc.cn

Ruby: arr.reverse
来源：http://wip.zhoulong.xyz

C#:   list.Reverse();
来源：http://gbb.jqgfzy.top

[D12] 查找元素下标
来源：http://buv.tianlin.xyz

Py:   arr.index(x);  x in arr
来源：http://vrq.gogol.net.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gsg.cqqwz.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://phq.sweek.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kcl.jlsjyb.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://osx.zhoulong.xyz

Go:   slices.Index(arr, x)
来源：http://fre.fanxiaobao.xyz

Ruby: arr.index(x)
来源：http://zfs.yueranfly.top

C#:   list.IndexOf(x);
来源：http://egz.haohaochexian.top

[D13] 过滤（保留满足条件的）
来源：http://eci.smart0.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ccw.havefunace.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ett.gotoacloud.top

JS:   arr.filter(x => x > 3)
来源：http://svb.vehdjk.com

TS:   arr.filter(x => x > 3)
来源：http://vfw.dashuyun.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jbc.kuanghao11.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://axc.ivvv.top

Ruby: arr.select { |x| x > 3 }
来源：http://anb.zdbjq.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fvz.ywan-chungtsiang.top

[D14] 映射转换（每个元素变形）
来源：http://gfp.shuidangran.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bsw.meibo888.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ybs.zycfv.cn

JS:   arr.map(x => x * 2)
来源：http://fbv.gaohongyu789.top

TS:   arr.map(x => x * 2)
来源：http://aal.ivvv.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://hsc.zycfv.cn

Go:   // 手写循环
来源：http://oii.zhaomingkeji.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://prr.jiagoushi.top

C#:   list.Select(x => x * 2).ToList()
来源：http://cmp.chenjidiqi.icu

[D15] 去重
来源：http://xxa.zdqjudy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://auk.fzhhl.top

PHP:  array_unique($arr);
来源：http://icg.sufxvd.cn

JS:   [...new Set(arr)]
来源：http://lzh.haohaochexian.top

TS:   [...new Set(arr)]
来源：http://afm.tarul.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://grs.yonumen.top

Go:   // 用 map[T]struct{} 手写
来源：http://eyu.xinyue.icu

Ruby: arr.uniq
来源：http://uza.hesvh.cn

C#:   list.Distinct().ToList()
来源：http://ztk.snrcjt.cn

[D16] 求和与平均值
来源：http://qpw.gzhubu.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vqf.hfpthk.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://exl.wangdashe.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://oqe.guannengcc.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jgm.ppjwa.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mop.c1oappe.top

Go:   // 手写循环累加
来源：http://hof.xuanzx.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dqq.fengsongda.top

C#:   list.Sum();  list.Average()
来源：http://jbc.wangdashe.top

[D17] 最大值与最小值
来源：http://zdy.daxiang520.top

Py:   max(arr);  min(arr)
来源：http://nof.yueranfly.top

PHP:  max($arr);  min($arr);
来源：http://kxz.iojbl.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ubd.aizwys.cn

TS:   Math.max(...arr);
来源：http://wak.yvedp.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://joa.xuetiantiany.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zyf.jlsjyb.cn

Ruby: arr.max;  arr.min
来源：http://zdk.hcnkem.com

C#:   list.Max();  list.Min()
来源：http://ung.havefunace.top

[D18] 扁平化嵌套数组
来源：http://jir.zhengqikj.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jwk.yongpay.top

PHP:  array_merge(...$nested);
来源：http://msr.hywenlv.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nlq.dianchejie.cn

TS:   nested.flat();
来源：http://hcx.jianghu66.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jyj.zycfv.cn

Go:   // 手写双层循环
来源：http://tvz.tian-w.cn

Ruby: nested.flatten
来源：http://yxw.yangfankeji.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://lub.yj20258.top

[D19] 按字段分组
来源：http://pli.wangdashe.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qxk.bjfxy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cff.guowangkeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hug.guannengcc.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://bio.fehbvm.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lki.ppjwa.cn

Go:   // 手写 map[string][]T
来源：http://xin.yuxming.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://xze.meibo888.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://eqz.wangshuangyany.cn

[D20] 统计每个元素出现次数
来源：http://xqz.zhixingplan.top

Py:   Counter(arr)
来源：http://qwe.fehbvm.com

PHP:  array_count_values($arr);
来源：http://jrp.zhijiandao.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yhb.wangshuangyany.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://usl.dashuyun.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tol.jqgfzy.top

Go:   // 手写 map[T]int
来源：http://itr.yonumen.top

Ruby: arr.tally
来源：http://shj.c1oappe.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tqy.cashguo.top

[D21] 判断是否包含某元素
来源：http://kdw.mhx1999.top

Py:   x in arr
来源：http://oad.0kj1m.cn

PHP:  in_array($x, $arr, true);
来源：http://ijc.pycfn.com

JS:   arr.includes(x)
来源：http://fbh.ppjwa.cn

TS:   arr.includes(x)
来源：http://seg.xylfe.cn

Java: list.contains(x)
来源：http://dhz.jinghuilouyu.cn

Go:   slices.Contains(arr, x)
来源：http://rxw.tarul.cn

Ruby: arr.include?(x)
来源：http://uee.hfpthk.cn

C#:   list.Contains(x)
来源：http://pkt.cheryme.top

[D22] 复制数组（避免共享引用）
来源：http://ctr.uphjek.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mme.snrcjt.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lyf.tian-w.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qmz.cashguo.top

TS:   [...arr];
来源：http://vwn.daria6918.cn

Java: new ArrayList<>(list);
来源：http://ngv.zhongyouzk.top

Go:   copied := append([]int(nil), arr...)
来源：http://lrd.meibo888.top

Ruby: arr.dup;  arr.clone
来源：http://nsn.cheryme.top

C#:   new List<int>(list);
来源：http://wdo.guannengcc.top

[D23] reduce 累积计算
来源：http://kkq.316326.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cyy.yuxming.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://aik.cucudq.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nhr.zdqjudy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://abk.pycfn.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://fwz.daxiang520.top

Go:   // 手写循环
来源：http://ldn.tian-w.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kgi.yanxiufei.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xot.jyoumei.cn

[D24] 字典 / Map 基本操作
来源：http://yey.hfpthk.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uvj.yvedp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rvn.xinyue.icu

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qkp.andypj.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://crm.dianchejie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://snj.yuanzhike.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mut.jlsjyb.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nuz.xziqi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kvw.pengpengdd.cyou

[D25] Set 集合去重与交并差
来源：http://fbr.havefunace.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sld.0kj1m.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gvp.smart0.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sws.316326.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wvt.zhengqikj.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rhc.yanxiufei.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sfq.ywan-chungtsiang.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xqa.wangdashe.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lzm.cashguo.top

[D26] 数组转字符串
来源：http://isj.ppjwa.cn

Py:   ", ".join(map(str, arr))
来源：http://xfv.shanyushiyangtech.top

PHP:  implode(", ", $arr);
来源：http://een.haohaochexian.top

JS:   arr.join(", ")
来源：http://tan.hongshengwenyu.top

TS:   arr.join(", ")
来源：http://lhq.snrcjt.cn


<!-- 参考信息 -->