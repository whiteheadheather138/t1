代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cxw.meibo888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aic.zhoulong.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://uli.hysaishi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eqa.shzxlz.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vci.jyoumei.cn

Go:   func add(a, b int) int
来源：http://smy.fktsv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tjz.shangyingyoupin.top

C#:   int Add(int a, int b) => a + b;
来源：http://uwg.zhoulong.xyz

[C14] 泛型函数
来源：http://wmy.hfpthk.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hwd.chenzaomai.com

PHP:  // 无泛型
来源：http://tpr.jiagoushi.top

JS:   // 无泛型
来源：http://cdf.snrcjt.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jds.iojbl.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://oeo.mhx1999.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yfi.yfazqb.com

Ruby: # 无泛型
来源：http://icw.chenzaomai.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jtz.jlsjyb.cn

[C15] 解构 / 展开参数
来源：http://amy.xziqi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ija.xuanzx.com

PHP:  [$a, $b] = $pair;
来源：http://jfo.yfazqb.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://irf.gogol.net.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fsi.jianghu66.top

Java: // 无解构
来源：http://qtn.yj202588.top

Go:   // 无解构
来源：http://glx.gzhubu.top

Ruby: a, b = pair
来源：http://pxz.jyoumei.cn

C#:   var (a, b) = pair;
来源：http://igb.bjfxy.top

[C16] 函数 / 方法重载
来源：http://huv.xuetiantiany.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zbr.jinqigfzy.top

PHP:  // 无重载
来源：http://cge.andypj.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://eii.ehwqpu.com

TS:   // 用联合类型或重载签名声明
来源：http://the.cheryme.top

Java: void f(int a) {}  void f(String a) {}
来源：http://lar.yueranfly.top

Go:   // 无重载：用不同函数名
来源：http://uqe.tian-w.cn

Ruby: # 无重载：靠动态参数
来源：http://ggp.hnxiangtu.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://zdo.fengsongda.top

================================================================================
来源：http://wns.redwolf501.top

D. 数组 / 列表 / 集合
来源：http://lpc.cqqwz.cn

================================================================================
来源：http://zku.tianlin.xyz

[D01] 创建数组 / 列表
来源：http://ndv.gzhubu.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://bmx.cdnleiting.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mkm.iojbl.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rnm.hysaishi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://weo.cucudq.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://igq.zycfv.cn

Go:   arr := []int{1, 2, 3}
来源：http://mvc.bbcook.cn

Ruby: arr = [1, 2, 3]
来源：http://dxq.zdqjudy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://usc.sjlbkw.cn

[D02] 追加元素到末尾
来源：http://gzk.pengpengdd.cyou

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pcw.jinqigufen.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://idt.yangfankeji.com

JS:   arr.push(4);
来源：http://kpj.jinghuilouyu.cn

TS:   arr.push(4);
来源：http://ifl.zhijiandao.cn

Java: list.add(4);
来源：http://qrq.cashguo.top

Go:   arr = append(arr, 4)
来源：http://vce.chenzaomai.com

Ruby: arr << 4; arr.push(5)
来源：http://dqv.yuanzhike.top

C#:   list.Add(4);
来源：http://tcu.zdqjudy.top

[D03] 在指定位置插入元素
来源：http://bwe.redwolf501.top

Py:   arr.insert(0, 0)
来源：http://jnv.ivvv.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dhh.yueranfly.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ugm.yuanzhike.top

TS:   arr.splice(0, 0, 0);
来源：http://dok.tarul.cn

Java: list.add(0, 0);
来源：http://qwi.mhx1999.top

Go:   arr = append([]int{0}, arr...)
来源：http://piu.bjfxy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uwj.yvedp.cn

C#:   list.Insert(0, 0);
来源：http://lsf.kuanghao11.cn

[D04] 删除元素
来源：http://hgf.yangfankeji.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pzk.fengsongda.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ojq.sysykeji.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mpk.yueranfly.top

TS:   arr.splice(0, 1);
来源：http://asv.smart0.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://csp.wangshuangyany.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ajb.yueranfly.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ouv.316326.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wcg.jqgufenzy.top

[D05] 访问与修改元素
来源：http://cbs.ctjpmb.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vbr.yanxiufei.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rlu.ehwqpu.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uba.fengsongda.top

TS:   arr[0]; arr.at(-1);
来源：http://dhc.bjfxy.top

Java: list.get(0); list.set(0, 9);
来源：http://djg.52xcode.cn

Go:   arr[0]; arr[0] = 9
来源：http://bsz.nwbrower.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xao.yj20258888.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uzx.chenlongwang.top

[D06] 数组长度
来源：http://uac.xuetiantiany.cn

Py:   len(arr)
来源：http://tnm.havefunace.top

PHP:  count($arr);
来源：http://ghl.zdqjudy.top

JS:   arr.length
来源：http://urm.xuanzx.com

TS:   arr.length
来源：http://rgc.sxryk.cn

Java: list.size();
来源：http://ouf.shangyingyoupin.top

Go:   len(arr)
来源：http://pva.smart0.xyz

Ruby: arr.length; arr.size
来源：http://sjl.jinyuanbaomall.cn

C#:   list.Count;
来源：http://gwz.jlsjyb.cn

[D07] 切片 / 取子数组
来源：http://jjz.zhaomingkeji.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://krx.pycfn.com

PHP:  array_slice($arr, 1, 3);
来源：http://vbl.quarkkingdee.top

JS:   arr.slice(1, 4);
来源：http://bvz.yangfankeji.com

TS:   arr.slice(1, 4);
来源：http://yro.yangfankeji.com

Java: list.subList(1, 4);
来源：http://wct.jianghu66.top

Go:   arr[1:4]
来源：http://qxn.hammf.cn

Ruby: arr[1, 3]
来源：http://gqs.jqgfzy.top

C#:   list.GetRange(1, 3);
来源：http://rhn.hcnkem.com

[D08] 合并两个数组
来源：http://azu.yvedp.cn

Py:   a + b;  a.extend(b)
来源：http://wwj.fanxiaobao.xyz

PHP:  array_merge($a, $b);
来源：http://bmx.hammf.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zak.hcnkem.com

TS:   [...a, ...b];
来源：http://sny.hfpthk.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://iiu.yj202588.top

Go:   append(a, b...)
来源：http://ouq.redwolf501.top

Ruby: a + b;  a.concat(b)
来源：http://ndq.smart0.xyz

C#:   a.Concat(b).ToList()
来源：http://ekt.ivvv.top

[D09] 排序（升序）
来源：http://vyr.guannengcc.top

Py:   sorted(arr);  arr.sort()
来源：http://lja.cheryme.top

PHP:  sort($arr);
来源：http://jyz.tian-w.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rnf.tian-w.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://dre.jinqigufen.top

Java: Collections.sort(list);  list.sort(null);
来源：http://akh.zhixingplan.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kds.gaohongyu789.top

Ruby: arr.sort
来源：http://txi.sufxvd.cn

C#:   list.Sort();
来源：http://amd.nanxinkj.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://dlx.jyoumei.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xwp.pengpengdd.cyou

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ldd.quarkkingdee.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://phx.ivvv.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qjy.hysaishi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nzx.fktsv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hes.tianlin.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://oqa.nanxuanxn.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://omt.xuanzx.com

[D11] 反转数组
来源：http://nex.xziqi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://sfk.pengpengdd.cyou

PHP:  array_reverse($arr);
来源：http://nty.hysaishi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://eai.uphjek.com

TS:   [...arr].reverse();
来源：http://fnl.zycfv.cn

Java: Collections.reverse(list);
来源：http://prg.nanxinkj.top

Go:   slices.Reverse(arr)
来源：http://vqh.zhixingplan.top

Ruby: arr.reverse
来源：http://hsy.fktsv.cn

C#:   list.Reverse();
来源：http://sor.jiagoushi.top

[D12] 查找元素下标
来源：http://dir.guowangkeji.top

Py:   arr.index(x);  x in arr
来源：http://xdp.daria6918.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cer.pengpengdd.cyou

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dce.snrcjt.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ovv.gogol.net.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rhu.zdqjudy.top

Go:   slices.Index(arr, x)
来源：http://lle.nanxuanxn.top

Ruby: arr.index(x)
来源：http://hpj.gogol.net.cn

C#:   list.IndexOf(x);
来源：http://day.zhijiandao.cn

[D13] 过滤（保留满足条件的）
来源：http://dqk.gzhubu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tfj.fktsv.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yoj.tarul.cn

JS:   arr.filter(x => x > 3)
来源：http://fpp.svipenyu.cn

TS:   arr.filter(x => x > 3)
来源：http://jbr.xinyue.icu

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fyy.xuetiantiany.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tyq.mhx1999.top

Ruby: arr.select { |x| x > 3 }
来源：http://qgo.ehwqpu.com

C#:   list.Where(x => x > 3).ToList()
来源：http://vcx.yuanzhike.top

[D14] 映射转换（每个元素变形）
来源：http://mbg.zhaomingkeji.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cdx.hnxiangtu.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yme.ctjpmb.com

JS:   arr.map(x => x * 2)
来源：http://fsn.chenjidiqi.icu

TS:   arr.map(x => x * 2)
来源：http://uiq.xylfe.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://eyq.zdqjudy.top

Go:   // 手写循环
来源：http://far.zdbjq.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dte.zhiwuduotai.top

C#:   list.Select(x => x * 2).ToList()
来源：http://bnj.fengsongda.top

[D15] 去重
来源：http://npw.ehwqpu.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nvv.pengpengdd.cyou

PHP:  array_unique($arr);
来源：http://eyy.yongpay.top

JS:   [...new Set(arr)]
来源：http://scq.ybcxt.top

TS:   [...new Set(arr)]
来源：http://cht.jqgfzy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://amm.jinqigufen.top

Go:   // 用 map[T]struct{} 手写
来源：http://alf.hysaishi.cn

Ruby: arr.uniq
来源：http://pul.dashuyun.cn

C#:   list.Distinct().ToList()
来源：http://uzr.wangshuangyany.cn

[D16] 求和与平均值
来源：http://oec.hnqzz.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ozc.wangshuangyany.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mtq.shangyingyoupin.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vpc.hywenlv.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qxc.fktsv.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vxm.zdbjq.cn

Go:   // 手写循环累加
来源：http://drr.nanxuanxn.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://umx.quarkkingdee.top

C#:   list.Sum();  list.Average()
来源：http://zht.hnxiangtu.top

[D17] 最大值与最小值
来源：http://sep.ctjpmb.com

Py:   max(arr);  min(arr)
来源：http://bxt.gotoacloud.top

PHP:  max($arr);  min($arr);
来源：http://gut.0kj1m.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bkn.tarul.cn

TS:   Math.max(...arr);
来源：http://dyl.uphjek.com

Java: Collections.max(list);  Collections.min(list);
来源：http://tyb.shuidangran.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ztk.ehwqpu.com

Ruby: arr.max;  arr.min
来源：http://qjk.aizwys.cn

C#:   list.Max();  list.Min()
来源：http://ozw.iojbl.cn

[D18] 扁平化嵌套数组
来源：http://esh.hnqzz.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gvy.jianghu66.top

PHP:  array_merge(...$nested);
来源：http://vpr.cucudq.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://exj.fehbvm.com

TS:   nested.flat();
来源：http://tjm.svipenyu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wqw.yanxiufei.cn

Go:   // 手写双层循环
来源：http://wql.nwbrower.top

Ruby: nested.flatten
来源：http://bxb.xylfe.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://grg.yueranfly.top

[D19] 按字段分组
来源：http://uhf.hesvh.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ufk.sweek.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ddy.shanyushiyangtech.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gsc.jinqigfzy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://bfh.zhaomingkeji.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gtg.fengsongda.top

Go:   // 手写 map[string][]T
来源：http://hri.zhaomingkeji.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://xpt.sufxvd.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wqm.hesvh.cn

[D20] 统计每个元素出现次数
来源：http://zut.zdbjq.cn

Py:   Counter(arr)
来源：http://tls.tarul.cn

PHP:  array_count_values($arr);
来源：http://dyi.zhiwuduotai.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mfi.kuanghao11.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wpo.birdmap.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xlb.smart0.xyz

Go:   // 手写 map[T]int
来源：http://lax.cheryme.top

Ruby: arr.tally
来源：http://zpr.xinyue.icu

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ped.cashguo.top

[D21] 判断是否包含某元素
来源：http://znt.zhixingplan.top

Py:   x in arr
来源：http://bzp.xuetiantiany.cn

PHP:  in_array($x, $arr, true);
来源：http://fkn.zhixingplan.top

JS:   arr.includes(x)
来源：http://kfq.jlsjyb.cn

TS:   arr.includes(x)
来源：http://owz.fehbvm.com

Java: list.contains(x)
来源：http://cvu.sxryk.cn

Go:   slices.Contains(arr, x)
来源：http://sor.shangyingyoupin.top

Ruby: arr.include?(x)
来源：http://spe.hammf.cn

C#:   list.Contains(x)
来源：http://mlq.yj202588.top

[D22] 复制数组（避免共享引用）
来源：http://utp.hnxiangtu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ufl.xingfuxueyuan.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sro.zycfv.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xvn.andypj.xyz

TS:   [...arr];
来源：http://eax.quarkkingdee.top

Java: new ArrayList<>(list);
来源：http://gnv.yongpay.top

Go:   copied := append([]int(nil), arr...)
来源：http://jwq.0kj1m.cn

Ruby: arr.dup;  arr.clone
来源：http://whp.nwbrower.top

C#:   new List<int>(list);
来源：http://eil.zhoulong.xyz

[D23] reduce 累积计算
来源：http://soc.wangshuangyany.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://oof.sjlbkw.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gqd.yanxiufei.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hjy.316326.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zkn.zycfv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rwh.quarkkingdee.top

Go:   // 手写循环
来源：http://vxd.ybcxt.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kcb.guowangkeji.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wwz.nanxuanxn.top

[D24] 字典 / Map 基本操作
来源：http://pom.yueranfly.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bzh.daxiang520.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bot.zhaomingkeji.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://axe.ydjk.org.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wvn.gogol.net.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://anx.zhiwuduotai.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ymb.jinqigufen.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xyg.jiagoushi.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gby.sxryk.cn

[D25] Set 集合去重与交并差
来源：http://oeh.daxiang520.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://omc.fktsv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cdb.zdqjudy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bjw.jyoumei.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zrj.yfazqb.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bzt.sjlbkw.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://khd.fzhhl.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://omt.fehbvm.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://arv.yvedp.cn

[D26] 数组转字符串
来源：http://dba.zhaomingkeji.xyz

Py:   ", ".join(map(str, arr))
来源：http://bzb.wangdashe.top

PHP:  implode(", ", $arr);
来源：http://hrp.nanxinkj.top

JS:   arr.join(", ")
来源：http://tgz.aizwys.cn

TS:   arr.join(", ")
来源：http://iwr.nanxinkj.top

Java: String.join(", ", list)
来源：http://fcq.hnxiangtu.top

Go:   strings.Join(strs, ", ")
来源：http://ddu.hammf.cn

Ruby: arr.join(", ")
来源：http://cvz.smart0.xyz

C#:   string.Join(", ", list)
来源：http://xmj.dashuyun.cn

================================================================================
来源：http://pjo.bbcook.cn

E. 字符串处理
来源：http://ccr.hnxiangtu.top

================================================================================
来源：http://onh.zhongyouzk.top

[E01] 拼接字符串
来源：http://kuf.cqqwz.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://amc.c1oappe.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qmy.yongpay.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mub.zhixingplan.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wdb.tian-w.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fzw.xuanzx.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hpy.kuanghao11.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ckf.fengsongda.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kbz.aibaodan.cn

[E02] 重复字符串
来源：http://boe.sjlbkw.cn

Py:   "ab" * 3
来源：http://tpr.yongpay.top

PHP:  str_repeat("ab", 3);
来源：http://saq.ydzc1.top

JS:   "ab".repeat(3)
来源：http://ifq.andypj.xyz

TS:   "ab".repeat(3)
来源：http://rqp.aizwys.cn

Java: "ab".repeat(3)
来源：http://kxn.zdqjudy.top

Go:   strings.Repeat("ab", 3)
来源：http://cri.jinqigufen.top

Ruby: "ab" * 3
来源：http://tew.chenzaomai.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://aml.redwolf501.top

[E03] 截取子串
来源：http://arn.vehdjk.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hvf.ywan-chungtsiang.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ozs.zycfv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zzx.fengsongda.top

TS:   s.slice(1, 4)
来源：http://msc.fzhhl.top

Java: s.substring(1, 4)
来源：http://zby.fehbvm.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://aay.zhoulong.xyz


<!-- 参考信息 -->