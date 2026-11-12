代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nvb.316326.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kcd.ehwqpu.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ean.jinghuilouyu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vjh.hongshengwenyu.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uky.cashguo.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fbi.zycfv.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://axh.ybcxt.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tur.yvedp.cn

[C10] 变量作用域
来源：http://kjc.yfazqb.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://giy.zdbjq.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mro.zdqjudy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fyq.daria6918.cn

TS:   同 JS
来源：http://dzq.pycfn.com

Java: 方法内为块级作用域
来源：http://wsn.daxiang520.top

Go:   花括号块级作用域
来源：http://dtk.shuidangran.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://iom.dianchejie.cn

C#:   块级作用域
来源：http://uxu.zhixingplan.top

[C11] 模块导入与导出
来源：http://iul.aizwys.cn

Py:   from module import func
来源：http://eng.ctjpmb.com

PHP:  require "file.php";  或 use App\Service;
来源：http://dii.hcnkem.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://isy.zdbjq.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://snr.yonumen.top

Java: import java.util.List;
来源：http://trj.fengsongda.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://amm.daria6918.cn

Ruby: require "json"; require_relative "./util"
来源：http://xhm.zhengqikj.top

C#:   using System.Text;
来源：http://pwk.fzhhl.top

[C12] 立即执行函数 IIFE
来源：http://kcm.epnwcf.com

Py:   (lambda: print("run"))()
来源：http://ijo.hnqzz.top

PHP:  (function () { echo "run"; })();
来源：http://pxh.iojbl.cn

JS:   (() => { console.log("run"); })();
来源：http://lio.zhengqikj.top

TS:   (() => { console.log("run"); })();
来源：http://gze.yangfankeji.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hfs.uphjek.com

Go:   func() { fmt.Println("run") }()
来源：http://btb.daxiang520.top

Ruby: -> { puts "run" }.call
来源：http://nqr.guowangkeji.top

C#:   // 无 IIFE：用静态构造函数
来源：http://csk.shuidangran.top

[C13] 类型声明 / 类型注解
来源：http://tfl.zycfv.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wqd.xuanzx.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bky.wangdashe.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nqk.jqgufenzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lmv.hammf.cn

Java: int add(int a, int b) { return a + b; }
来源：http://bbi.jinghuilouyu.cn

Go:   func add(a, b int) int
来源：http://lpg.xuanzx.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ozi.redwolf501.top

C#:   int Add(int a, int b) => a + b;
来源：http://cyz.fktsv.cn

[C14] 泛型函数
来源：http://xdu.haohaochexian.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://adw.tarul.cn

PHP:  // 无泛型
来源：http://zmt.hfpthk.cn

JS:   // 无泛型
来源：http://rko.zhengqikj.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uwl.iojbl.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bcr.sxryk.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fop.sysykeji.top

Ruby: # 无泛型
来源：http://aah.hywenlv.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fhy.yj20258888.top

[C15] 解构 / 展开参数
来源：http://yhm.ivvv.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nuw.jqgufenzy.top

PHP:  [$a, $b] = $pair;
来源：http://qeg.ybcxt.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lae.ydzc1.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xcq.vehdjk.com

Java: // 无解构
来源：http://yvc.sysykeji.top

Go:   // 无解构
来源：http://vvz.fehbvm.com

Ruby: a, b = pair
来源：http://nae.cqqwz.cn

C#:   var (a, b) = pair;
来源：http://cmh.yangfankeji.com

[C16] 函数 / 方法重载
来源：http://zip.birdmap.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lpl.hnqzz.top

PHP:  // 无重载
来源：http://sny.shangyingyoupin.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ala.jqgfzy.top

TS:   // 用联合类型或重载签名声明
来源：http://bzy.ivvv.top

Java: void f(int a) {}  void f(String a) {}
来源：http://gaq.fzhhl.top

Go:   // 无重载：用不同函数名
来源：http://whb.zhixingplan.top

Ruby: # 无重载：靠动态参数
来源：http://rso.jqgfzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ixa.hnqzz.top

================================================================================
来源：http://vty.ctjpmb.com

D. 数组 / 列表 / 集合
来源：http://dxd.yj202588.top

================================================================================
来源：http://skg.fengsongda.top

[D01] 创建数组 / 列表
来源：http://yrh.zhiwuduotai.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://plk.svipenyu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nox.hammf.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rkm.chenjidiqi.icu

TS:   const arr: number[] = [1, 2, 3];
来源：http://lll.yongpay.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ydt.ydzc1.top

Go:   arr := []int{1, 2, 3}
来源：http://ldl.xuetiantiany.cn

Ruby: arr = [1, 2, 3]
来源：http://otk.jinqigfzy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://osv.tarul.cn

[D02] 追加元素到末尾
来源：http://mqh.tianlin.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mjv.tianlin.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zly.cashguo.top

JS:   arr.push(4);
来源：http://ori.xuanzx.com

TS:   arr.push(4);
来源：http://plf.svipenyu.cn

Java: list.add(4);
来源：http://msv.andypj.xyz

Go:   arr = append(arr, 4)
来源：http://rvl.c1oappe.top

Ruby: arr << 4; arr.push(5)
来源：http://ojq.jinyuanbaomall.cn

C#:   list.Add(4);
来源：http://grt.jinqigufen.top

[D03] 在指定位置插入元素
来源：http://vvi.fktsv.cn

Py:   arr.insert(0, 0)
来源：http://lyo.zhengqikj.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pee.cdnleiting.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://taz.ppjwa.cn

TS:   arr.splice(0, 0, 0);
来源：http://lxv.quarkkingdee.top

Java: list.add(0, 0);
来源：http://ldy.hesvh.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xbr.birdmap.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zlv.redwolf501.top

C#:   list.Insert(0, 0);
来源：http://pww.yangfankeji.com

[D04] 删除元素
来源：http://fsl.dashuyun.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dhk.chenlongwang.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lbl.zhengqikj.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tnn.xuanzx.com

TS:   arr.splice(0, 1);
来源：http://wvs.chenlongwang.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mtg.svipenyu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sjs.yvedp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ctz.uphjek.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://azc.jqgufenzy.top

[D05] 访问与修改元素
来源：http://jbo.havefunace.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lsv.aizwys.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lkt.kuanghao11.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ivz.gotoacloud.top

TS:   arr[0]; arr.at(-1);
来源：http://qik.yonumen.top

Java: list.get(0); list.set(0, 9);
来源：http://wpg.daxiang520.top

Go:   arr[0]; arr[0] = 9
来源：http://gnu.shangyingyoupin.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rtr.quarkkingdee.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rbt.quarkkingdee.top

[D06] 数组长度
来源：http://gfr.jinqigfzy.top

Py:   len(arr)
来源：http://mhr.ctjpmb.com

PHP:  count($arr);
来源：http://mbd.zhoulong.xyz

JS:   arr.length
来源：http://but.9152youxi.cn

TS:   arr.length
来源：http://gfx.yuanzhike.top

Java: list.size();
来源：http://nmh.yj20258.top

Go:   len(arr)
来源：http://wzc.fanxiaobao.xyz

Ruby: arr.length; arr.size
来源：http://jjt.hysaishi.cn

C#:   list.Count;
来源：http://pcv.pengpengdd.cyou

[D07] 切片 / 取子数组
来源：http://ple.birdmap.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kge.yj20258888.top

PHP:  array_slice($arr, 1, 3);
来源：http://fig.kuanghao11.cn

JS:   arr.slice(1, 4);
来源：http://ldw.shanyushiyangtech.top

TS:   arr.slice(1, 4);
来源：http://hny.52xcode.cn

Java: list.subList(1, 4);
来源：http://tpy.xingfuxueyuan.xyz

Go:   arr[1:4]
来源：http://bso.jyoumei.cn

Ruby: arr[1, 3]
来源：http://cfs.cdnleiting.top

C#:   list.GetRange(1, 3);
来源：http://ofv.birdmap.top

[D08] 合并两个数组
来源：http://ico.cucudq.cn

Py:   a + b;  a.extend(b)
来源：http://ztj.gotoacloud.top

PHP:  array_merge($a, $b);
来源：http://yse.pycfn.com

JS:   [...a, ...b];  a.concat(b);
来源：http://svr.yj20258.top

TS:   [...a, ...b];
来源：http://uxp.zhaomingkeji.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ctz.yuxming.cn

Go:   append(a, b...)
来源：http://xyl.vqdsnc.cn

Ruby: a + b;  a.concat(b)
来源：http://pey.jqgufenzy.top

C#:   a.Concat(b).ToList()
来源：http://olh.ydzc1.top

[D09] 排序（升序）
来源：http://acl.yj20258888.top

Py:   sorted(arr);  arr.sort()
来源：http://dbu.zhixingplan.top

PHP:  sort($arr);
来源：http://ozp.chenzaomai.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://knr.tarul.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://flo.wangshuangyany.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mbh.guowangkeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pyp.kuanghao11.cn

Ruby: arr.sort
来源：http://xio.iojbl.cn

C#:   list.Sort();
来源：http://vqa.xylfe.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ilm.xuetiantiany.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ckp.fzhhl.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rnn.jinqigufen.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rgu.wangdashe.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://szv.shanyushiyangtech.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nfr.tian-w.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fhi.zdbjq.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rux.redwolf501.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lem.chenzaomai.com

[D11] 反转数组
来源：http://sbx.andypj.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://rqd.yanxiufei.cn

PHP:  array_reverse($arr);
来源：http://kor.pycfn.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://upb.snrcjt.cn

TS:   [...arr].reverse();
来源：http://cre.bbcook.cn

Java: Collections.reverse(list);
来源：http://igo.jinqigfzy.top

Go:   slices.Reverse(arr)
来源：http://wpl.jqgfzy.top

Ruby: arr.reverse
来源：http://gjr.feifeiyinyue.top

C#:   list.Reverse();
来源：http://thw.fzhhl.top

[D12] 查找元素下标
来源：http://cjp.ehwqpu.com

Py:   arr.index(x);  x in arr
来源：http://swe.redwolf501.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xzu.9152youxi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sdl.yuxming.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zib.yuxming.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kpc.iojbl.cn

Go:   slices.Index(arr, x)
来源：http://rwp.xinyue.icu

Ruby: arr.index(x)
来源：http://hdw.0kj1m.cn

C#:   list.IndexOf(x);
来源：http://agd.pycfn.com

[D13] 过滤（保留满足条件的）
来源：http://ifz.sysykeji.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dgc.zhijiandao.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://afz.bjfxy.top

JS:   arr.filter(x => x > 3)
来源：http://zjn.52xcode.cn

TS:   arr.filter(x => x > 3)
来源：http://qit.smart0.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://osm.svipenyu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://edo.feifeiyinyue.top

Ruby: arr.select { |x| x > 3 }
来源：http://lmh.jinyuanbaomall.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://edt.vehdjk.com

[D14] 映射转换（每个元素变形）
来源：http://kpo.hnxiangtu.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lwv.bjfxy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://eam.haohaochexian.top

JS:   arr.map(x => x * 2)
来源：http://gui.shangyingyoupin.top

TS:   arr.map(x => x * 2)
来源：http://ozz.hnqzz.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://xmm.zdbjq.cn

Go:   // 手写循环
来源：http://ghq.fktsv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vsd.xuanzx.com

C#:   list.Select(x => x * 2).ToList()
来源：http://opa.xingfuxueyuan.xyz

[D15] 去重
来源：http://lqh.xziqi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pwk.chenzaomai.com

PHP:  array_unique($arr);
来源：http://ppq.haohaochexian.top

JS:   [...new Set(arr)]
来源：http://icq.hfpthk.cn

TS:   [...new Set(arr)]
来源：http://kly.cucudq.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kds.hfpthk.cn

Go:   // 用 map[T]struct{} 手写
来源：http://auu.pengpengdd.cyou

Ruby: arr.uniq
来源：http://elf.jinghuilouyu.cn

C#:   list.Distinct().ToList()
来源：http://htd.tianlin.xyz

[D16] 求和与平均值
来源：http://bnu.ehwqpu.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hit.xylfe.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hqi.bbcook.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zxw.sysykeji.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lew.c1oappe.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ifo.zhaomingkeji.xyz

Go:   // 手写循环累加
来源：http://bmx.wangshuangyany.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tkd.yj20258888.top

C#:   list.Sum();  list.Average()
来源：http://xaz.haohaochexian.top

[D17] 最大值与最小值
来源：http://ozn.ywan-chungtsiang.top

Py:   max(arr);  min(arr)
来源：http://pam.zdqjudy.top

PHP:  max($arr);  min($arr);
来源：http://wto.bjfxy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vxj.chenlongwang.top

TS:   Math.max(...arr);
来源：http://kjp.shangyingyoupin.top

Java: Collections.max(list);  Collections.min(list);
来源：http://xpj.haohaochexian.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rid.fengsongda.top

Ruby: arr.max;  arr.min
来源：http://bqz.yuanzhike.top

C#:   list.Max();  list.Min()
来源：http://bpg.pycfn.com

[D18] 扁平化嵌套数组
来源：http://wjs.hammf.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://obk.jinyuanbaomall.cn

PHP:  array_merge(...$nested);
来源：http://eam.svipenyu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hff.fktsv.cn

TS:   nested.flat();
来源：http://bdf.jiagoushi.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fqz.yuxming.cn

Go:   // 手写双层循环
来源：http://fnp.fktsv.cn

Ruby: nested.flatten
来源：http://ych.zdbjq.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ibu.jinqigfzy.top

[D19] 按字段分组
来源：http://eao.zdqjudy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rkn.aibaodan.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nqf.zycfv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qgi.pycfn.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://dzj.zhiwuduotai.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fhn.hfpthk.cn

Go:   // 手写 map[string][]T
来源：http://asr.yj202588.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://oyl.pengpengdd.cyou

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dvy.hcnkem.com

[D20] 统计每个元素出现次数
来源：http://xol.hongshengwenyu.top

Py:   Counter(arr)
来源：http://whl.ctjpmb.com

PHP:  array_count_values($arr);
来源：http://txo.ywan-chungtsiang.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gtv.cucudq.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nff.yj20258888.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tuu.pengpengdd.cyou

Go:   // 手写 map[T]int
来源：http://shu.nanxinkj.top

Ruby: arr.tally
来源：http://fvo.chenzaomai.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xfg.uphjek.com

[D21] 判断是否包含某元素
来源：http://duc.sweek.top

Py:   x in arr
来源：http://neu.zhiwuduotai.top

PHP:  in_array($x, $arr, true);
来源：http://tib.yanxiufei.cn

JS:   arr.includes(x)
来源：http://aal.cucudq.cn

TS:   arr.includes(x)
来源：http://eav.ivvv.top

Java: list.contains(x)
来源：http://fej.epnwcf.com

Go:   slices.Contains(arr, x)
来源：http://ycj.shuidangran.top

Ruby: arr.include?(x)
来源：http://cnj.fktsv.cn

C#:   list.Contains(x)
来源：http://nrk.fanxiaobao.xyz

[D22] 复制数组（避免共享引用）
来源：http://cqz.hcnkem.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vgt.guannengcc.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nvd.nanxinkj.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ger.tarul.cn

TS:   [...arr];
来源：http://nya.ctjpmb.com

Java: new ArrayList<>(list);
来源：http://wzf.fktsv.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fvu.yfazqb.com

Ruby: arr.dup;  arr.clone
来源：http://vte.yvedp.cn

C#:   new List<int>(list);
来源：http://iau.havefunace.top

[D23] reduce 累积计算
来源：http://oeq.daxiang520.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ulw.yj202588.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gbt.andypj.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lts.fktsv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bql.jinyuanbaomall.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://sxm.quarkkingdee.top

Go:   // 手写循环
来源：http://dal.xziqi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zjc.cqqwz.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ctm.yonumen.top

[D24] 字典 / Map 基本操作
来源：http://fte.yueranfly.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qci.yj20258.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cpq.yonumen.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dtq.zhaomingkeji.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hxu.ctjpmb.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tqa.vehdjk.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jvh.shanyushiyangtech.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fza.wangdashe.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://akb.sweek.top

[D25] Set 集合去重与交并差
来源：http://hmh.svipenyu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lxl.jiagoushi.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rew.aibaodan.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gkb.dianchejie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mld.aizwys.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://chk.birdmap.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://oth.316326.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://aii.aizwys.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://grq.ybcxt.top

[D26] 数组转字符串
来源：http://zzr.wangdashe.top


<!-- 参考信息 -->