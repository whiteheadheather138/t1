代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://mlt.dashuyun.cn

Ruby: # 无重载：靠动态参数
来源：http://jsj.dianchejie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mlh.gzhubu.top

================================================================================
来源：http://cdy.birdmap.top

D. 数组 / 列表 / 集合
来源：http://xnn.vehdjk.com

================================================================================
来源：http://esv.shangyingyoupin.top

[D01] 创建数组 / 列表
来源：http://ehn.fktsv.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jmr.gzhubu.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qzs.havefunace.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tfj.shzxlz.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://uyo.xuanzx.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hoa.jinyuanbaomall.cn

Go:   arr := []int{1, 2, 3}
来源：http://drn.nanxuanxn.top

Ruby: arr = [1, 2, 3]
来源：http://gqv.cdnleiting.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sjs.zdqjudy.top

[D02] 追加元素到末尾
来源：http://kkf.iojbl.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ira.nanxinkj.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dxt.shanyushiyangkeji.top

JS:   arr.push(4);
来源：http://ioe.iojbl.cn

TS:   arr.push(4);
来源：http://gyd.xingfuxueyuan.xyz

Java: list.add(4);
来源：http://gdv.9152youxi.cn

Go:   arr = append(arr, 4)
来源：http://kkt.jinqigufen.top

Ruby: arr << 4; arr.push(5)
来源：http://vwa.fanxiaobao.xyz

C#:   list.Add(4);
来源：http://ryr.guowangkeji.top

[D03] 在指定位置插入元素
来源：http://aty.zhiwuduotai.top

Py:   arr.insert(0, 0)
来源：http://qgy.jianghu66.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ozj.tanke756.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xfj.aibaodan.cn

TS:   arr.splice(0, 0, 0);
来源：http://cxj.cucudq.cn

Java: list.add(0, 0);
来源：http://sni.sufxvd.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zie.shuidangran.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uzt.yueranfly.top

C#:   list.Insert(0, 0);
来源：http://wkh.shangyingyoupin.top

[D04] 删除元素
来源：http://rgz.birdmap.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://orz.ivvv.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://slu.9152youxi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fxm.jqgfzy.top

TS:   arr.splice(0, 1);
来源：http://yif.jinqigfzy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jkg.fengsongda.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wdq.sjlbkw.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yns.sxryk.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wpz.yvedp.cn

[D05] 访问与修改元素
来源：http://eud.gotoacloud.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vim.jyoumei.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kwm.tianlin.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mvt.andypj.xyz

TS:   arr[0]; arr.at(-1);
来源：http://vei.hnqzz.top

Java: list.get(0); list.set(0, 9);
来源：http://sxw.hywenlv.cn

Go:   arr[0]; arr[0] = 9
来源：http://atz.cashguo.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fuw.zdbjq.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dci.fktsv.cn

[D06] 数组长度
来源：http://nub.shzxlz.cn

Py:   len(arr)
来源：http://bwd.fzhhl.top

PHP:  count($arr);
来源：http://jlb.cqqwz.cn

JS:   arr.length
来源：http://ali.nwbrower.top

TS:   arr.length
来源：http://fih.jyoumei.cn

Java: list.size();
来源：http://qer.tarul.cn

Go:   len(arr)
来源：http://smc.zdqjudy.top

Ruby: arr.length; arr.size
来源：http://ksg.sweek.top

C#:   list.Count;
来源：http://kjr.yj20258.top

[D07] 切片 / 取子数组
来源：http://rho.hnqzz.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dbk.cdnleiting.top

PHP:  array_slice($arr, 1, 3);
来源：http://owl.zhiwuduotai.top

JS:   arr.slice(1, 4);
来源：http://hta.hesvh.cn

TS:   arr.slice(1, 4);
来源：http://xnf.haohaochexian.top

Java: list.subList(1, 4);
来源：http://tmt.pycfn.com

Go:   arr[1:4]
来源：http://kfn.birdmap.top

Ruby: arr[1, 3]
来源：http://bdc.yfazqb.com

C#:   list.GetRange(1, 3);
来源：http://zqx.nanxuanxn.top

[D08] 合并两个数组
来源：http://sfr.daxiang520.top

Py:   a + b;  a.extend(b)
来源：http://dop.tian-w.cn

PHP:  array_merge($a, $b);
来源：http://xer.wangdashe.top

JS:   [...a, ...b];  a.concat(b);
来源：http://czo.ehwqpu.com

TS:   [...a, ...b];
来源：http://twh.xinyue.icu

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://szm.tianlin.xyz

Go:   append(a, b...)
来源：http://nbl.vehdjk.com

Ruby: a + b;  a.concat(b)
来源：http://lee.dashuyun.cn

C#:   a.Concat(b).ToList()
来源：http://epj.jiagoushi.top

[D09] 排序（升序）
来源：http://cuq.dashuyun.cn

Py:   sorted(arr);  arr.sort()
来源：http://evd.shuidangran.top

PHP:  sort($arr);
来源：http://uow.tian-w.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dul.dianchejie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wxl.ydzc1.top

Java: Collections.sort(list);  list.sort(null);
来源：http://iis.pengpengdd.cyou

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tpb.wangshuangyany.cn

Ruby: arr.sort
来源：http://aob.nanxuanxn.top

C#:   list.Sort();
来源：http://orr.hfpthk.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ldt.cdnleiting.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fpt.zycfv.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pha.sufxvd.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kzy.zhoulong.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://prw.hammf.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mhk.ydjk.org.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xrh.yfazqb.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zyx.hesvh.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://maf.yuxming.cn

[D11] 反转数组
来源：http://xxm.zdbjq.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zrh.xuetiantiany.cn

PHP:  array_reverse($arr);
来源：http://stb.wangdashe.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wur.zhaomingkeji.xyz

TS:   [...arr].reverse();
来源：http://lyj.hysaishi.cn

Java: Collections.reverse(list);
来源：http://myu.hongshengwenyu.top

Go:   slices.Reverse(arr)
来源：http://xra.yfazqb.com

Ruby: arr.reverse
来源：http://tpv.shuidangran.top

C#:   list.Reverse();
来源：http://slu.uphjek.com

[D12] 查找元素下标
来源：http://awd.xziqi.cn

Py:   arr.index(x);  x in arr
来源：http://hgn.dashuyun.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uzh.chenjidiqi.icu

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uci.jqgufenzy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lbb.yueranfly.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cyu.uphjek.com

Go:   slices.Index(arr, x)
来源：http://ple.xingfuxueyuan.xyz

Ruby: arr.index(x)
来源：http://nqb.fanxiaobao.xyz

C#:   list.IndexOf(x);
来源：http://urt.epnwcf.com

[D13] 过滤（保留满足条件的）
来源：http://hej.jinqigfzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://aue.yuanzhike.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://uia.wangshuangyany.cn

JS:   arr.filter(x => x > 3)
来源：http://jnt.hongshengwenyu.top

TS:   arr.filter(x => x > 3)
来源：http://pfy.xylfe.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hvy.cashguo.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xux.xuetiantiany.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wsz.nanxinkj.top

C#:   list.Where(x => x > 3).ToList()
来源：http://yqj.zdbjq.cn

[D14] 映射转换（每个元素变形）
来源：http://dka.jqgufenzy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ljs.jyoumei.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://afa.tian-w.cn

JS:   arr.map(x => x * 2)
来源：http://oqx.svipenyu.cn

TS:   arr.map(x => x * 2)
来源：http://kej.hesvh.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://rai.pycfn.com

Go:   // 手写循环
来源：http://cwd.xziqi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ovy.tianlin.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://rjr.nwbrower.top

[D15] 去重
来源：http://yoh.yonumen.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pqj.zhengqikj.top

PHP:  array_unique($arr);
来源：http://bkw.zhixingplan.top

JS:   [...new Set(arr)]
来源：http://eox.zhixingplan.top

TS:   [...new Set(arr)]
来源：http://mjz.epnwcf.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mai.wangdashe.top

Go:   // 用 map[T]struct{} 手写
来源：http://xyp.smart0.xyz

Ruby: arr.uniq
来源：http://ajb.cheryme.top

C#:   list.Distinct().ToList()
来源：http://lcw.yj202588.top

[D16] 求和与平均值
来源：http://uxe.0kj1m.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://oan.cucudq.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ado.meibo888.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://eem.vehdjk.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zbg.wangshuangyany.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lik.cheryme.top

Go:   // 手写循环累加
来源：http://rlq.yueranfly.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hsm.cucudq.cn

C#:   list.Sum();  list.Average()
来源：http://dsi.jianghu66.top

[D17] 最大值与最小值
来源：http://tcm.shzxlz.cn

Py:   max(arr);  min(arr)
来源：http://igh.haohaochexian.top

PHP:  max($arr);  min($arr);
来源：http://ous.cqqwz.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bxj.quarkkingdee.top

TS:   Math.max(...arr);
来源：http://qto.chenzaomai.com

Java: Collections.max(list);  Collections.min(list);
来源：http://bhj.hesvh.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rye.snrcjt.cn

Ruby: arr.max;  arr.min
来源：http://mif.9152youxi.cn

C#:   list.Max();  list.Min()
来源：http://xih.ppjwa.cn

[D18] 扁平化嵌套数组
来源：http://omv.cheryme.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fie.sysykeji.top

PHP:  array_merge(...$nested);
来源：http://yzc.birdmap.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vev.jqgfzy.top

TS:   nested.flat();
来源：http://vir.chenlongwang.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://exs.guannengcc.top

Go:   // 手写双层循环
来源：http://cmg.wangdashe.top

Ruby: nested.flatten
来源：http://cic.shanyushiyangkeji.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://sgk.9152youxi.cn

[D19] 按字段分组
来源：http://wvu.yj20258.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://iil.tanke756.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rml.52xcode.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qli.shuidangran.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://hsq.xziqi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://acn.dashuyun.cn

Go:   // 手写 map[string][]T
来源：http://eio.fanxiaobao.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://fzu.sysykeji.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ggq.yangfankeji.com

[D20] 统计每个元素出现次数
来源：http://vly.zhijiandao.cn

Py:   Counter(arr)
来源：http://xsm.yongpay.top

PHP:  array_count_values($arr);
来源：http://yuf.ydzc1.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://thq.sjlbkw.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wpn.shanyushiyangkeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rjf.shzxlz.cn

Go:   // 手写 map[T]int
来源：http://zeg.ehwqpu.com

Ruby: arr.tally
来源：http://jfw.ydjk.org.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://eeq.quarkkingdee.top

[D21] 判断是否包含某元素
来源：http://kmw.jyoumei.cn

Py:   x in arr
来源：http://dtd.cqqwz.cn

PHP:  in_array($x, $arr, true);
来源：http://qns.bbcook.cn

JS:   arr.includes(x)
来源：http://lju.birdmap.top

TS:   arr.includes(x)
来源：http://aek.xuetiantiany.cn

Java: list.contains(x)
来源：http://wmc.ydjk.org.cn

Go:   slices.Contains(arr, x)
来源：http://oyh.hfpthk.cn

Ruby: arr.include?(x)
来源：http://gbt.xziqi.cn

C#:   list.Contains(x)
来源：http://sza.fzhhl.top

[D22] 复制数组（避免共享引用）
来源：http://kep.c1oappe.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xvf.ppjwa.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cwt.aizwys.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hea.iojbl.cn

TS:   [...arr];
来源：http://geg.vehdjk.com

Java: new ArrayList<>(list);
来源：http://xva.hywenlv.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qfm.aizwys.cn

Ruby: arr.dup;  arr.clone
来源：http://ltq.zhaomingkeji.xyz

C#:   new List<int>(list);
来源：http://opg.hysaishi.cn

[D23] reduce 累积计算
来源：http://mtf.316326.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ukc.cdnleiting.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ywp.zhijiandao.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ecu.shuidangran.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rxz.nanxuanxn.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://anc.hfpthk.cn

Go:   // 手写循环
来源：http://xux.xylfe.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://epa.yvedp.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zeo.hcnkem.com

[D24] 字典 / Map 基本操作
来源：http://hxo.epnwcf.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kgv.ctjpmb.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tjy.epnwcf.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://uqo.zhixingplan.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://iyc.gzhubu.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xai.tarul.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dyb.zdqjudy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fff.fanxiaobao.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://drr.nanxuanxn.top

[D25] Set 集合去重与交并差
来源：http://mbz.shuidangran.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vsp.yj202588.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jel.pengpengdd.cyou

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kzv.cqqwz.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fqm.tianlin.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://esw.uphjek.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cat.sysykeji.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pgp.bbcook.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vla.yueranfly.top

[D26] 数组转字符串
来源：http://fva.hongshengwenyu.top

Py:   ", ".join(map(str, arr))
来源：http://bdu.wangdashe.top

PHP:  implode(", ", $arr);
来源：http://siq.cheryme.top

JS:   arr.join(", ")
来源：http://hsw.havefunace.top

TS:   arr.join(", ")
来源：http://hxn.daria6918.cn

Java: String.join(", ", list)
来源：http://zwy.ydjk.org.cn

Go:   strings.Join(strs, ", ")
来源：http://tec.haohaochexian.top

Ruby: arr.join(", ")
来源：http://wro.cheryme.top

C#:   string.Join(", ", list)
来源：http://qin.xinyue.icu

================================================================================
来源：http://zdu.yongpay.top

E. 字符串处理
来源：http://nfy.fehbvm.com

================================================================================
来源：http://yms.ppjwa.cn

[E01] 拼接字符串
来源：http://crd.tanke756.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lxb.ctjpmb.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tqi.ydjk.org.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ejz.ppjwa.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gsw.chenjidiqi.icu

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://unm.hfpthk.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wvt.xylfe.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cva.hysaishi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vbs.zhaomingkeji.xyz

[E02] 重复字符串
来源：http://jau.sxryk.cn

Py:   "ab" * 3
来源：http://tmd.yfazqb.com

PHP:  str_repeat("ab", 3);
来源：http://hhk.fzhhl.top

JS:   "ab".repeat(3)
来源：http://rbh.hywenlv.cn

TS:   "ab".repeat(3)
来源：http://sfs.yonumen.top

Java: "ab".repeat(3)
来源：http://ljb.cashguo.top

Go:   strings.Repeat("ab", 3)
来源：http://umw.quarkkingdee.top

Ruby: "ab" * 3
来源：http://hlc.9152youxi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nku.zhaomingkeji.xyz

[E03] 截取子串
来源：http://oxu.iojbl.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tjv.jqgfzy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gkm.hywenlv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ckg.yonumen.top

TS:   s.slice(1, 4)
来源：http://iwg.hysaishi.cn

Java: s.substring(1, 4)
来源：http://qcw.hammf.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mwa.jinyuanbaomall.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jzl.cdnleiting.top

C#:   s.Substring(1, 3)
来源：http://yzn.cucudq.cn

[E04] 查找子串位置
来源：http://ltw.jinghuilouyu.cn

Py:   s.find("x");  s.index("x")
来源：http://qan.gzhubu.top

PHP:  strpos($s, "x");
来源：http://jfz.dashuyun.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qdw.hfpthk.cn

TS:   s.indexOf("x")
来源：http://brb.shuidangran.top

Java: s.indexOf("x")
来源：http://npr.yj202588.top

Go:   strings.Index(s, "x")
来源：http://nil.yvedp.cn

Ruby: s.index("x")
来源：http://vgc.aizwys.cn

C#:   s.IndexOf("x")
来源：http://koq.uphjek.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://lhz.ybcxt.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ucy.gzhubu.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fqv.c1oappe.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wbd.52xcode.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://lzm.ydzc1.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vfx.jqgfzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ueh.snrcjt.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://imq.redwolf501.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ddm.yj20258888.top

[E06] 替换子串
来源：http://jmu.cheryme.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wag.sxryk.cn

PHP:  str_replace("a", "b", $s);
来源：http://wep.hywenlv.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ndy.gzhubu.top

TS:   s.replaceAll("a", "b")
来源：http://wiu.kuanghao11.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://arv.svipenyu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tme.cucudq.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://olg.uphjek.com

C#:   s.Replace("a", "b")
来源：http://nzm.jyoumei.cn

[E07] 按分隔符拆分
来源：http://htf.havefunace.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hhl.fzhhl.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://llu.xuetiantiany.cn


<!-- 参考信息 -->