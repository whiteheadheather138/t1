代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://jly.cucudq.cn

JS:   (() => { console.log("run"); })();
来源：http://bhk.zhoulong.xyz

TS:   (() => { console.log("run"); })();
来源：http://upa.feifeiyinyue.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ilw.shzxlz.cn

Go:   func() { fmt.Println("run") }()
来源：http://hkn.hongshengwenyu.top

Ruby: -> { puts "run" }.call
来源：http://iou.yonumen.top

C#:   // 无 IIFE：用静态构造函数
来源：http://xxv.tianlin.xyz

[C13] 类型声明 / 类型注解
来源：http://klg.xinyue.icu

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wks.wangshuangyany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://phe.chenzaomai.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ayd.jqgufenzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ttd.ydjk.org.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fhi.nanxuanxn.top

Go:   func add(a, b int) int
来源：http://jji.cdnleiting.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xxo.hcnkem.com

C#:   int Add(int a, int b) => a + b;
来源：http://vfm.dashuyun.cn

[C14] 泛型函数
来源：http://cru.yueranfly.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ftf.hnxiangtu.top

PHP:  // 无泛型
来源：http://bkw.nwbrower.top

JS:   // 无泛型
来源：http://gmx.yonumen.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kdg.jinghuilouyu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jyw.xuetiantiany.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ooq.ivvv.top

Ruby: # 无泛型
来源：http://imj.chenzaomai.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ldq.jianghu66.top

[C15] 解构 / 展开参数
来源：http://xii.cdnleiting.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jij.zhengqikj.top

PHP:  [$a, $b] = $pair;
来源：http://gva.pengpengdd.cyou

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bat.sufxvd.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dql.pycfn.com

Java: // 无解构
来源：http://xxx.jinqigufen.top

Go:   // 无解构
来源：http://gbo.jianghu66.top

Ruby: a, b = pair
来源：http://owl.yueranfly.top

C#:   var (a, b) = pair;
来源：http://qxj.smart0.xyz

[C16] 函数 / 方法重载
来源：http://kvm.sweek.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sju.pengpengdd.cyou

PHP:  // 无重载
来源：http://age.wangdashe.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ofn.fktsv.cn

TS:   // 用联合类型或重载签名声明
来源：http://dud.52xcode.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://sur.hesvh.cn

Go:   // 无重载：用不同函数名
来源：http://wzc.nanxuanxn.top

Ruby: # 无重载：靠动态参数
来源：http://gax.shangyingyoupin.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://uol.havefunace.top

================================================================================
来源：http://qrr.vqdsnc.cn

D. 数组 / 列表 / 集合
来源：http://jog.52xcode.cn

================================================================================
来源：http://izf.jianghu66.top

[D01] 创建数组 / 列表
来源：http://izl.tanke756.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://gjt.ydzc1.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://iyg.zhongyouzk.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vvg.guowangkeji.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://dbq.jinqigfzy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lxs.daxiang520.top

Go:   arr := []int{1, 2, 3}
来源：http://pbl.zhijiandao.cn

Ruby: arr = [1, 2, 3]
来源：http://jmr.hnqzz.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dwc.svipenyu.cn

[D02] 追加元素到末尾
来源：http://dcu.jlsjyb.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kmx.shanyushiyangtech.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zjl.jlsjyb.cn

JS:   arr.push(4);
来源：http://sko.yangfankeji.com

TS:   arr.push(4);
来源：http://bth.xuetiantiany.cn

Java: list.add(4);
来源：http://iey.chenlongwang.top

Go:   arr = append(arr, 4)
来源：http://rwp.shanyushiyangkeji.top

Ruby: arr << 4; arr.push(5)
来源：http://rhy.yvedp.cn

C#:   list.Add(4);
来源：http://zmf.zhongyouzk.top

[D03] 在指定位置插入元素
来源：http://xcg.316326.xyz

Py:   arr.insert(0, 0)
来源：http://ubs.shzxlz.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jdu.yuxming.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dbs.tian-w.cn

TS:   arr.splice(0, 0, 0);
来源：http://yqk.yongpay.top

Java: list.add(0, 0);
来源：http://nap.daxiang520.top

Go:   arr = append([]int{0}, arr...)
来源：http://uqz.bjfxy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kzt.cqqwz.cn

C#:   list.Insert(0, 0);
来源：http://jyo.tanke756.top

[D04] 删除元素
来源：http://ihn.yj202588.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ido.jinqigfzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ewx.sufxvd.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://api.bjfxy.top

TS:   arr.splice(0, 1);
来源：http://xxh.shanyushiyangtech.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fzt.sxryk.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xoc.shanyushiyangkeji.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ngi.vqdsnc.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ros.chenzaomai.com

[D05] 访问与修改元素
来源：http://nvc.yonumen.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bef.quarkkingdee.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dha.9152youxi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hdu.xylfe.cn

TS:   arr[0]; arr.at(-1);
来源：http://xhc.haohaochexian.top

Java: list.get(0); list.set(0, 9);
来源：http://ipa.hesvh.cn

Go:   arr[0]; arr[0] = 9
来源：http://sny.hongshengwenyu.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jqe.jinyuanbaomall.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yzh.cheryme.top

[D06] 数组长度
来源：http://dlm.xuanzx.com

Py:   len(arr)
来源：http://kyc.jinqigufen.top

PHP:  count($arr);
来源：http://wep.cashguo.top

JS:   arr.length
来源：http://npc.ywan-chungtsiang.top

TS:   arr.length
来源：http://glq.nanxinkj.top

Java: list.size();
来源：http://nhm.jinqigfzy.top

Go:   len(arr)
来源：http://hkn.sufxvd.cn

Ruby: arr.length; arr.size
来源：http://hwn.yfazqb.com

C#:   list.Count;
来源：http://wnh.hcnkem.com

[D07] 切片 / 取子数组
来源：http://asd.jlsjyb.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://djp.jyoumei.cn

PHP:  array_slice($arr, 1, 3);
来源：http://nnm.xinyue.icu

JS:   arr.slice(1, 4);
来源：http://ran.quarkkingdee.top

TS:   arr.slice(1, 4);
来源：http://yci.yonumen.top

Java: list.subList(1, 4);
来源：http://gsb.sxryk.cn

Go:   arr[1:4]
来源：http://ayp.xziqi.cn

Ruby: arr[1, 3]
来源：http://ijd.cucudq.cn

C#:   list.GetRange(1, 3);
来源：http://huf.ivvv.top

[D08] 合并两个数组
来源：http://hhs.hnqzz.top

Py:   a + b;  a.extend(b)
来源：http://ttb.jinyuanbaomall.cn

PHP:  array_merge($a, $b);
来源：http://ciw.ppjwa.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://lcr.zhijiandao.cn

TS:   [...a, ...b];
来源：http://pxi.shangyingyoupin.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cig.fzhhl.top

Go:   append(a, b...)
来源：http://icd.0kj1m.cn

Ruby: a + b;  a.concat(b)
来源：http://nyp.smart0.xyz

C#:   a.Concat(b).ToList()
来源：http://veu.shanyushiyangkeji.top

[D09] 排序（升序）
来源：http://ydp.daria6918.cn

Py:   sorted(arr);  arr.sort()
来源：http://sdl.zhixingplan.top

PHP:  sort($arr);
来源：http://qce.ydzc1.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://seo.zhongyouzk.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://xxe.yj202588.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ncd.ivvv.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mvl.nwbrower.top

Ruby: arr.sort
来源：http://hwr.tian-w.cn

C#:   list.Sort();
来源：http://xxd.fzhhl.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://fce.zhijiandao.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yzu.cdnleiting.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ywo.quarkkingdee.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lab.fktsv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cfj.ybcxt.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lzg.gaohongyu789.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vnl.zhaomingkeji.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qub.kuanghao11.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://glj.hnxiangtu.top

[D11] 反转数组
来源：http://wwd.cashguo.top

Py:   arr[::-1];  arr.reverse()
来源：http://eqv.hywenlv.cn

PHP:  array_reverse($arr);
来源：http://kug.ydzc1.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nhm.hysaishi.cn

TS:   [...arr].reverse();
来源：http://jbg.shanyushiyangtech.top

Java: Collections.reverse(list);
来源：http://fww.cqqwz.cn

Go:   slices.Reverse(arr)
来源：http://kod.birdmap.top

Ruby: arr.reverse
来源：http://sbv.pengpengdd.cyou

C#:   list.Reverse();
来源：http://msn.xylfe.cn

[D12] 查找元素下标
来源：http://nry.ctjpmb.com

Py:   arr.index(x);  x in arr
来源：http://uur.c1oappe.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nzk.andypj.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zjq.shzxlz.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aco.fzhhl.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ooz.gogol.net.cn

Go:   slices.Index(arr, x)
来源：http://dcf.cucudq.cn

Ruby: arr.index(x)
来源：http://bkq.guannengcc.top

C#:   list.IndexOf(x);
来源：http://gol.svipenyu.cn

[D13] 过滤（保留满足条件的）
来源：http://fdn.daria6918.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kqa.zhengqikj.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wai.tian-w.cn

JS:   arr.filter(x => x > 3)
来源：http://xaz.daria6918.cn

TS:   arr.filter(x => x > 3)
来源：http://fly.jinqigufen.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wta.pycfn.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://iea.iojbl.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fkz.ctjpmb.com

C#:   list.Where(x => x > 3).ToList()
来源：http://nzt.cdnleiting.top

[D14] 映射转换（每个元素变形）
来源：http://vmy.cucudq.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ybs.feifeiyinyue.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vdv.zdbjq.cn

JS:   arr.map(x => x * 2)
来源：http://vqc.meibo888.top

TS:   arr.map(x => x * 2)
来源：http://gku.dianchejie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://cba.aizwys.cn

Go:   // 手写循环
来源：http://kny.shanyushiyangkeji.top

Ruby: arr.map { |x| x * 2 }
来源：http://vfm.yanxiufei.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://lna.cqqwz.cn

[D15] 去重
来源：http://bzj.ehwqpu.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pnn.guowangkeji.top

PHP:  array_unique($arr);
来源：http://sah.hcnkem.com

JS:   [...new Set(arr)]
来源：http://qnd.tarul.cn

TS:   [...new Set(arr)]
来源：http://nfs.yj20258.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nry.cashguo.top

Go:   // 用 map[T]struct{} 手写
来源：http://lng.birdmap.top

Ruby: arr.uniq
来源：http://nxj.fengsongda.top

C#:   list.Distinct().ToList()
来源：http://jkw.daxiang520.top

[D16] 求和与平均值
来源：http://tkz.jqgfzy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://byn.zhixingplan.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dje.vehdjk.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://soa.ctjpmb.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ecl.jqgufenzy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kat.iojbl.cn

Go:   // 手写循环累加
来源：http://nbp.yuxming.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hzp.ywan-chungtsiang.top

C#:   list.Sum();  list.Average()
来源：http://gcb.smart0.xyz

[D17] 最大值与最小值
来源：http://sfx.xuanzx.com

Py:   max(arr);  min(arr)
来源：http://hbe.jlsjyb.cn

PHP:  max($arr);  min($arr);
来源：http://hff.zycfv.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wor.xingfuxueyuan.xyz

TS:   Math.max(...arr);
来源：http://ubk.tanke756.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ore.jiagoushi.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vbr.chenzaomai.com

Ruby: arr.max;  arr.min
来源：http://flw.aizwys.cn

C#:   list.Max();  list.Min()
来源：http://akh.c1oappe.top

[D18] 扁平化嵌套数组
来源：http://dcr.chenjidiqi.icu

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xcp.cucudq.cn

PHP:  array_merge(...$nested);
来源：http://bjq.zycfv.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zee.52xcode.cn

TS:   nested.flat();
来源：http://abt.zdbjq.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://llc.fehbvm.com

Go:   // 手写双层循环
来源：http://fgj.zdqjudy.top

Ruby: nested.flatten
来源：http://pze.sysykeji.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://wcd.ppjwa.cn

[D19] 按字段分组
来源：http://wwl.iojbl.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tug.pycfn.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qva.tian-w.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zcj.hywenlv.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://nxr.zhaomingkeji.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fsh.yongpay.top

Go:   // 手写 map[string][]T
来源：http://duo.hcnkem.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://pze.gogol.net.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zeg.fzhhl.top

[D20] 统计每个元素出现次数
来源：http://yfl.jianghu66.top

Py:   Counter(arr)
来源：http://xnu.wangdashe.top

PHP:  array_count_values($arr);
来源：http://xnw.haohaochexian.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kqp.xinyue.icu

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gdc.shangyingyoupin.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kvm.52xcode.cn

Go:   // 手写 map[T]int
来源：http://sel.tian-w.cn

Ruby: arr.tally
来源：http://kqq.cashguo.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vuc.hysaishi.cn

[D21] 判断是否包含某元素
来源：http://jwk.xziqi.cn

Py:   x in arr
来源：http://ewe.9152youxi.cn

PHP:  in_array($x, $arr, true);
来源：http://rfe.hnqzz.top

JS:   arr.includes(x)
来源：http://qsi.fehbvm.com

TS:   arr.includes(x)
来源：http://vph.0kj1m.cn

Java: list.contains(x)
来源：http://kyo.zhixingplan.top

Go:   slices.Contains(arr, x)
来源：http://gnu.yuxming.cn

Ruby: arr.include?(x)
来源：http://ipt.cucudq.cn

C#:   list.Contains(x)
来源：http://rnr.bjfxy.top

[D22] 复制数组（避免共享引用）
来源：http://mzd.yuxming.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wkd.gzhubu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sbj.aibaodan.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hdq.dashuyun.cn

TS:   [...arr];
来源：http://ifo.xziqi.cn

Java: new ArrayList<>(list);
来源：http://jcy.smart0.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://ule.jyoumei.cn

Ruby: arr.dup;  arr.clone
来源：http://uzn.guowangkeji.top

C#:   new List<int>(list);
来源：http://nxo.sxryk.cn

[D23] reduce 累积计算
来源：http://jtl.ywan-chungtsiang.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://twk.nanxinkj.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://eej.bbcook.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://chn.vqdsnc.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lla.zhixingplan.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://msl.yj20258888.top

Go:   // 手写循环
来源：http://lec.vqdsnc.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rzs.kuanghao11.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gxr.andypj.xyz

[D24] 字典 / Map 基本操作
来源：http://aik.yuxming.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vtb.gaohongyu789.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ppp.cheryme.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://iuc.quarkkingdee.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hqj.jyoumei.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rwb.ydjk.org.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gce.nanxinkj.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kjk.havefunace.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kib.vehdjk.com

[D25] Set 集合去重与交并差
来源：http://eag.hongshengwenyu.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dcv.zhoulong.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vtd.zhengqikj.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://slg.tanke756.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xxz.hysaishi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://oyk.tanke756.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://asg.shzxlz.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xfv.bjfxy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ewr.cheryme.top

[D26] 数组转字符串
来源：http://kda.sysykeji.top

Py:   ", ".join(map(str, arr))
来源：http://zwe.xuetiantiany.cn

PHP:  implode(", ", $arr);
来源：http://yrz.jinqigfzy.top

JS:   arr.join(", ")
来源：http://szy.vehdjk.com

TS:   arr.join(", ")
来源：http://iis.zhaomingkeji.xyz

Java: String.join(", ", list)
来源：http://mbx.daxiang520.top

Go:   strings.Join(strs, ", ")
来源：http://ofz.zdbjq.cn

Ruby: arr.join(", ")
来源：http://yem.yueranfly.top

C#:   string.Join(", ", list)
来源：http://gdj.0kj1m.cn

================================================================================
来源：http://wge.0kj1m.cn

E. 字符串处理
来源：http://aom.zhaomingkeji.xyz

================================================================================
来源：http://ejt.havefunace.top

[E01] 拼接字符串
来源：http://akj.nwbrower.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fly.quarkkingdee.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vwq.zycfv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lna.jinghuilouyu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mxz.smart0.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://eaq.shanyushiyangkeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nak.zhaomingkeji.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fhq.yonumen.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fqk.cqqwz.cn

[E02] 重复字符串
来源：http://mrc.daria6918.cn

Py:   "ab" * 3
来源：http://wlt.fktsv.cn

PHP:  str_repeat("ab", 3);
来源：http://yrb.yvedp.cn

JS:   "ab".repeat(3)
来源：http://wgu.xziqi.cn

TS:   "ab".repeat(3)
来源：http://pbi.hammf.cn

Java: "ab".repeat(3)
来源：http://nlv.316326.xyz

Go:   strings.Repeat("ab", 3)
来源：http://pcg.ehwqpu.com

Ruby: "ab" * 3
来源：http://sga.9152youxi.cn


<!-- 参考信息 -->