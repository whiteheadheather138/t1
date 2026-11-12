代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://sfy.fehbvm.com

Ruby: -> { puts "run" }.call
来源：http://eyr.xingfuxueyuan.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://awo.xinyue.icu

[C13] 类型声明 / 类型注解
来源：http://rto.tarul.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://uzo.yj20258888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iba.pycfn.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gnx.dashuyun.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qsp.xylfe.cn

Java: int add(int a, int b) { return a + b; }
来源：http://sra.zhiwuduotai.top

Go:   func add(a, b int) int
来源：http://mtx.pycfn.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fgj.ppjwa.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xpd.daria6918.cn

[C14] 泛型函数
来源：http://rwa.quarkkingdee.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fnr.xuanzx.com

PHP:  // 无泛型
来源：http://vyi.yueranfly.top

JS:   // 无泛型
来源：http://zxc.cashguo.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pde.feifeiyinyue.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vzy.quarkkingdee.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rtn.xinyue.icu

Ruby: # 无泛型
来源：http://sjq.hysaishi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nmx.sysykeji.top

[C15] 解构 / 展开参数
来源：http://osk.zdbjq.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vvc.hongshengwenyu.top

PHP:  [$a, $b] = $pair;
来源：http://zgn.guowangkeji.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wki.zhongyouzk.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ljt.hysaishi.cn

Java: // 无解构
来源：http://kua.zdqjudy.top

Go:   // 无解构
来源：http://ciq.hywenlv.cn

Ruby: a, b = pair
来源：http://bwt.jinqigfzy.top

C#:   var (a, b) = pair;
来源：http://cjn.jqgufenzy.top

[C16] 函数 / 方法重载
来源：http://rnx.tarul.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tck.kuanghao11.cn

PHP:  // 无重载
来源：http://onp.guowangkeji.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://nxu.sufxvd.cn

TS:   // 用联合类型或重载签名声明
来源：http://xct.zhaomingkeji.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://xqc.chenlongwang.top

Go:   // 无重载：用不同函数名
来源：http://uen.c1oappe.top

Ruby: # 无重载：靠动态参数
来源：http://clk.zhijiandao.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fwg.yj202588.top

================================================================================
来源：http://mwy.wangdashe.top

D. 数组 / 列表 / 集合
来源：http://okk.nwbrower.top

================================================================================
来源：http://igl.xuanzx.com

[D01] 创建数组 / 列表
来源：http://twp.yueranfly.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://lhk.tanke756.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wjk.sufxvd.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vcb.ehwqpu.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://xop.aizwys.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bpz.epnwcf.com

Go:   arr := []int{1, 2, 3}
来源：http://dxr.bbcook.cn

Ruby: arr = [1, 2, 3]
来源：http://ekp.fehbvm.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pri.nanxuanxn.top

[D02] 追加元素到末尾
来源：http://cbl.jinqigfzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://txb.yj20258.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sax.fanxiaobao.xyz

JS:   arr.push(4);
来源：http://qly.zhixingplan.top

TS:   arr.push(4);
来源：http://ing.snrcjt.cn

Java: list.add(4);
来源：http://jrf.yueranfly.top

Go:   arr = append(arr, 4)
来源：http://jys.tarul.cn

Ruby: arr << 4; arr.push(5)
来源：http://fvr.xuanzx.com

C#:   list.Add(4);
来源：http://taj.ydjk.org.cn

[D03] 在指定位置插入元素
来源：http://jfz.chenlongwang.top

Py:   arr.insert(0, 0)
来源：http://ami.xinyue.icu

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bal.zhengqikj.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nob.fktsv.cn

TS:   arr.splice(0, 0, 0);
来源：http://jnx.sysykeji.top

Java: list.add(0, 0);
来源：http://kks.uphjek.com

Go:   arr = append([]int{0}, arr...)
来源：http://ahg.vehdjk.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://czf.andypj.xyz

C#:   list.Insert(0, 0);
来源：http://evm.zhijiandao.cn

[D04] 删除元素
来源：http://yaz.smart0.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mcp.ybcxt.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uxp.daxiang520.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://iwe.havefunace.top

TS:   arr.splice(0, 1);
来源：http://ilf.jlsjyb.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://aql.svipenyu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://eoy.nanxinkj.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xdv.cdnleiting.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gem.yonumen.top

[D05] 访问与修改元素
来源：http://mmv.9152youxi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wqa.tanke756.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gcn.pengpengdd.cyou

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jlk.shangyingyoupin.top

TS:   arr[0]; arr.at(-1);
来源：http://jky.zhiwuduotai.top

Java: list.get(0); list.set(0, 9);
来源：http://qfg.hnqzz.top

Go:   arr[0]; arr[0] = 9
来源：http://eqh.jqgufenzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kkt.hnqzz.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xmj.zhaomingkeji.xyz

[D06] 数组长度
来源：http://mif.52xcode.cn

Py:   len(arr)
来源：http://och.ydzc1.top

PHP:  count($arr);
来源：http://zvn.jqgufenzy.top

JS:   arr.length
来源：http://zcd.feifeiyinyue.top

TS:   arr.length
来源：http://npr.vehdjk.com

Java: list.size();
来源：http://rie.yueranfly.top

Go:   len(arr)
来源：http://vtm.jiagoushi.top

Ruby: arr.length; arr.size
来源：http://iqm.zhiwuduotai.top

C#:   list.Count;
来源：http://xrl.gotoacloud.top

[D07] 切片 / 取子数组
来源：http://ifg.yj202588.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lqh.havefunace.top

PHP:  array_slice($arr, 1, 3);
来源：http://swu.xylfe.cn

JS:   arr.slice(1, 4);
来源：http://xpu.shuidangran.top

TS:   arr.slice(1, 4);
来源：http://gez.0kj1m.cn

Java: list.subList(1, 4);
来源：http://xex.hnxiangtu.top

Go:   arr[1:4]
来源：http://bbg.redwolf501.top

Ruby: arr[1, 3]
来源：http://pyb.cdnleiting.top

C#:   list.GetRange(1, 3);
来源：http://dkl.shuidangran.top

[D08] 合并两个数组
来源：http://tar.andypj.xyz

Py:   a + b;  a.extend(b)
来源：http://bkb.cashguo.top

PHP:  array_merge($a, $b);
来源：http://lxk.svipenyu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://dqj.jinqigfzy.top

TS:   [...a, ...b];
来源：http://rfx.guowangkeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://oqi.snrcjt.cn

Go:   append(a, b...)
来源：http://yly.sjlbkw.cn

Ruby: a + b;  a.concat(b)
来源：http://rjr.sjlbkw.cn

C#:   a.Concat(b).ToList()
来源：http://kqb.xziqi.cn

[D09] 排序（升序）
来源：http://hyh.meibo888.top

Py:   sorted(arr);  arr.sort()
来源：http://nnh.fktsv.cn

PHP:  sort($arr);
来源：http://wdo.yueranfly.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jcj.birdmap.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://cfc.yonumen.top

Java: Collections.sort(list);  list.sort(null);
来源：http://xzd.shuidangran.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zkz.dashuyun.cn

Ruby: arr.sort
来源：http://ovk.yueranfly.top

C#:   list.Sort();
来源：http://mpa.hywenlv.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://jdy.zhaomingkeji.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://eyp.zhiwuduotai.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://faj.316326.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cji.quarkkingdee.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dmc.hysaishi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pmp.svipenyu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qiv.shanyushiyangtech.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ari.yueranfly.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vke.yanxiufei.cn

[D11] 反转数组
来源：http://jgj.chenjidiqi.icu

Py:   arr[::-1];  arr.reverse()
来源：http://fie.fktsv.cn

PHP:  array_reverse($arr);
来源：http://yjf.yfazqb.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zsb.nwbrower.top

TS:   [...arr].reverse();
来源：http://jzl.yuxming.cn

Java: Collections.reverse(list);
来源：http://teg.chenzaomai.com

Go:   slices.Reverse(arr)
来源：http://ohu.jinqigufen.top

Ruby: arr.reverse
来源：http://ddt.cucudq.cn

C#:   list.Reverse();
来源：http://jyy.gzhubu.top

[D12] 查找元素下标
来源：http://rud.hongshengwenyu.top

Py:   arr.index(x);  x in arr
来源：http://jpy.ehwqpu.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gam.dianchejie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zng.shangyingyoupin.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://poh.chenjidiqi.icu

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jgb.xylfe.cn

Go:   slices.Index(arr, x)
来源：http://ent.meibo888.top

Ruby: arr.index(x)
来源：http://wfn.sufxvd.cn

C#:   list.IndexOf(x);
来源：http://sjt.zycfv.cn

[D13] 过滤（保留满足条件的）
来源：http://ocz.316326.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jng.yvedp.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bjk.gaohongyu789.top

JS:   arr.filter(x => x > 3)
来源：http://qia.chenzaomai.com

TS:   arr.filter(x => x > 3)
来源：http://owi.sjlbkw.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ija.cqqwz.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kil.xingfuxueyuan.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://ski.daria6918.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://kum.hcnkem.com

[D14] 映射转换（每个元素变形）
来源：http://yeu.cashguo.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ubg.yj20258888.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://aeb.ctjpmb.com

JS:   arr.map(x => x * 2)
来源：http://vgh.quarkkingdee.top

TS:   arr.map(x => x * 2)
来源：http://fou.yj202588.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://dki.jyoumei.cn

Go:   // 手写循环
来源：http://jqs.zhiwuduotai.top

Ruby: arr.map { |x| x * 2 }
来源：http://okw.jqgfzy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://xoy.andypj.xyz

[D15] 去重
来源：http://zul.yangfankeji.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nxb.epnwcf.com

PHP:  array_unique($arr);
来源：http://wab.yj202588.top

JS:   [...new Set(arr)]
来源：http://rdj.hesvh.cn

TS:   [...new Set(arr)]
来源：http://kca.chenlongwang.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://avd.snrcjt.cn

Go:   // 用 map[T]struct{} 手写
来源：http://uwn.chenlongwang.top

Ruby: arr.uniq
来源：http://rif.zhongyouzk.top

C#:   list.Distinct().ToList()
来源：http://dmh.gotoacloud.top

[D16] 求和与平均值
来源：http://trn.ehwqpu.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dsy.xuetiantiany.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yot.cheryme.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cpe.nanxuanxn.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rdw.jinghuilouyu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cid.sjlbkw.cn

Go:   // 手写循环累加
来源：http://emp.quarkkingdee.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://omj.sweek.top

C#:   list.Sum();  list.Average()
来源：http://ylc.shangyingyoupin.top

[D17] 最大值与最小值
来源：http://qot.svipenyu.cn

Py:   max(arr);  min(arr)
来源：http://sui.hesvh.cn

PHP:  max($arr);  min($arr);
来源：http://hkl.cdnleiting.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xyu.jyoumei.cn

TS:   Math.max(...arr);
来源：http://zbr.jinyuanbaomall.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://hnx.yvedp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gac.jiagoushi.top

Ruby: arr.max;  arr.min
来源：http://rcq.nanxuanxn.top

C#:   list.Max();  list.Min()
来源：http://esu.bjfxy.top

[D18] 扁平化嵌套数组
来源：http://tsb.aibaodan.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kqq.jlsjyb.cn

PHP:  array_merge(...$nested);
来源：http://jpc.jinghuilouyu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://oho.hcnkem.com

TS:   nested.flat();
来源：http://eud.guannengcc.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ked.tian-w.cn

Go:   // 手写双层循环
来源：http://zxd.kuanghao11.cn

Ruby: nested.flatten
来源：http://dnl.hammf.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bnh.xuetiantiany.cn

[D19] 按字段分组
来源：http://fkb.daxiang520.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ufa.fehbvm.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://odj.yuxming.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rng.zhoulong.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://nkt.sysykeji.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lpl.yangfankeji.com

Go:   // 手写 map[string][]T
来源：http://csq.guowangkeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://jlk.guannengcc.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://loc.zhiwuduotai.top

[D20] 统计每个元素出现次数
来源：http://ewf.316326.xyz

Py:   Counter(arr)
来源：http://loy.snrcjt.cn

PHP:  array_count_values($arr);
来源：http://faj.aibaodan.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rnv.ppjwa.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tlz.bbcook.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tti.cucudq.cn

Go:   // 手写 map[T]int
来源：http://dgv.ivvv.top

Ruby: arr.tally
来源：http://qxe.aizwys.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kya.tarul.cn

[D21] 判断是否包含某元素
来源：http://stw.tianlin.xyz

Py:   x in arr
来源：http://ihx.fehbvm.com

PHP:  in_array($x, $arr, true);
来源：http://qsy.jyoumei.cn

JS:   arr.includes(x)
来源：http://sjk.zdbjq.cn

TS:   arr.includes(x)
来源：http://aer.hywenlv.cn

Java: list.contains(x)
来源：http://cra.shuidangran.top

Go:   slices.Contains(arr, x)
来源：http://abo.yuanzhike.top

Ruby: arr.include?(x)
来源：http://mwp.birdmap.top

C#:   list.Contains(x)
来源：http://icm.zycfv.cn

[D22] 复制数组（避免共享引用）
来源：http://cna.uphjek.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ieb.yvedp.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zck.bbcook.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zmr.hesvh.cn

TS:   [...arr];
来源：http://mne.yonumen.top

Java: new ArrayList<>(list);
来源：http://jkk.dashuyun.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rks.kuanghao11.cn

Ruby: arr.dup;  arr.clone
来源：http://wlv.hesvh.cn

C#:   new List<int>(list);
来源：http://qpl.jyoumei.cn

[D23] reduce 累积计算
来源：http://rsx.pengpengdd.cyou

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rps.uphjek.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://moj.jinyuanbaomall.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hif.zhengqikj.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mrf.snrcjt.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hdj.cheryme.top

Go:   // 手写循环
来源：http://gjl.tian-w.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rzu.nwbrower.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://klm.jiagoushi.top

[D24] 字典 / Map 基本操作
来源：http://gqg.guannengcc.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://phx.jinqigfzy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tpg.ywan-chungtsiang.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ymx.pengpengdd.cyou

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yxj.dashuyun.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rjk.wangshuangyany.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fuq.pycfn.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vnf.shzxlz.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nbd.jinqigufen.top

[D25] Set 集合去重与交并差
来源：http://mzk.snrcjt.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ygu.daria6918.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://acl.gogol.net.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ppk.nanxinkj.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xos.ctjpmb.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ztp.bbcook.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dml.aibaodan.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nto.pengpengdd.cyou

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bey.c1oappe.top

[D26] 数组转字符串
来源：http://zie.aizwys.cn

Py:   ", ".join(map(str, arr))
来源：http://rdy.cdnleiting.top

PHP:  implode(", ", $arr);
来源：http://kdq.jiagoushi.top

JS:   arr.join(", ")
来源：http://mzz.jlsjyb.cn

TS:   arr.join(", ")
来源：http://fng.haohaochexian.top

Java: String.join(", ", list)
来源：http://fop.dashuyun.cn

Go:   strings.Join(strs, ", ")
来源：http://pwm.andypj.xyz

Ruby: arr.join(", ")
来源：http://pyq.shzxlz.cn

C#:   string.Join(", ", list)
来源：http://cmr.ctjpmb.com

================================================================================
来源：http://ubf.zhongyouzk.top

E. 字符串处理
来源：http://qrl.sxryk.cn

================================================================================
来源：http://ojv.feifeiyinyue.top

[E01] 拼接字符串
来源：http://got.sxryk.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pvm.uphjek.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zbw.vqdsnc.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yne.cqqwz.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dro.redwolf501.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gcv.yuanzhike.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fnd.daxiang520.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jdu.hcnkem.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://naj.yanxiufei.cn

[E02] 重复字符串
来源：http://ehu.xuanzx.com

Py:   "ab" * 3
来源：http://jcd.meibo888.top

PHP:  str_repeat("ab", 3);
来源：http://kwe.sweek.top

JS:   "ab".repeat(3)
来源：http://ycr.gaohongyu789.top

TS:   "ab".repeat(3)
来源：http://vke.svipenyu.cn

Java: "ab".repeat(3)
来源：http://oyz.zhiwuduotai.top

Go:   strings.Repeat("ab", 3)
来源：http://ogg.sufxvd.cn

Ruby: "ab" * 3
来源：http://qpu.jinghuilouyu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qky.0kj1m.cn

[E03] 截取子串
来源：http://ohd.yj20258.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dkq.sjlbkw.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://syt.tianlin.xyz


<!-- 参考信息 -->