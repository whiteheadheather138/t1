代发 wailian999

D. 数组 / 列表 / 集合
来源：http://nyk.wangshuangyany.cn

================================================================================
来源：http://eck.hnxiangtu.top

[D01] 创建数组 / 列表
来源：http://soa.hesvh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://iun.shanyushiyangkeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pxe.yj202588.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kpb.zhiwuduotai.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://hka.wangdashe.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ngo.hcnkem.com

Go:   arr := []int{1, 2, 3}
来源：http://hdf.yuanzhike.top

Ruby: arr = [1, 2, 3]
来源：http://bik.0kj1m.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ohe.yangfankeji.com

[D02] 追加元素到末尾
来源：http://lsk.jinyuanbaomall.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://iez.aibaodan.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://elj.ybcxt.top

JS:   arr.push(4);
来源：http://cky.hysaishi.cn

TS:   arr.push(4);
来源：http://tez.havefunace.top

Java: list.add(4);
来源：http://cbg.yj202588.top

Go:   arr = append(arr, 4)
来源：http://eao.xinyue.icu

Ruby: arr << 4; arr.push(5)
来源：http://lec.yongpay.top

C#:   list.Add(4);
来源：http://qcz.feifeiyinyue.top

[D03] 在指定位置插入元素
来源：http://ohf.guowangkeji.top

Py:   arr.insert(0, 0)
来源：http://gku.wangshuangyany.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://skd.xziqi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jxr.zdqjudy.top

TS:   arr.splice(0, 0, 0);
来源：http://nes.snrcjt.cn

Java: list.add(0, 0);
来源：http://fwt.hcnkem.com

Go:   arr = append([]int{0}, arr...)
来源：http://oho.haohaochexian.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bnz.xingfuxueyuan.xyz

C#:   list.Insert(0, 0);
来源：http://pzo.jiagoushi.top

[D04] 删除元素
来源：http://wjd.hcnkem.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mwv.yonumen.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sut.shuidangran.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xdd.tarul.cn

TS:   arr.splice(0, 1);
来源：http://eyk.jianghu66.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xcg.cdnleiting.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mfd.hywenlv.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://duu.shuidangran.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zgy.hcnkem.com

[D05] 访问与修改元素
来源：http://hft.cucudq.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kqv.quarkkingdee.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vqq.shanyushiyangtech.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wqb.chenzaomai.com

TS:   arr[0]; arr.at(-1);
来源：http://qcv.ydjk.org.cn

Java: list.get(0); list.set(0, 9);
来源：http://cwz.bbcook.cn

Go:   arr[0]; arr[0] = 9
来源：http://qdt.smart0.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ekv.iojbl.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dxr.52xcode.cn

[D06] 数组长度
来源：http://nud.zhixingplan.top

Py:   len(arr)
来源：http://bgv.yonumen.top

PHP:  count($arr);
来源：http://eus.vqdsnc.cn

JS:   arr.length
来源：http://alk.yongpay.top

TS:   arr.length
来源：http://zdv.wangshuangyany.cn

Java: list.size();
来源：http://buf.shzxlz.cn

Go:   len(arr)
来源：http://yyz.zhijiandao.cn

Ruby: arr.length; arr.size
来源：http://ldf.xingfuxueyuan.xyz

C#:   list.Count;
来源：http://iip.0kj1m.cn

[D07] 切片 / 取子数组
来源：http://vds.fengsongda.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hua.quarkkingdee.top

PHP:  array_slice($arr, 1, 3);
来源：http://ajl.meibo888.top

JS:   arr.slice(1, 4);
来源：http://dwa.feifeiyinyue.top

TS:   arr.slice(1, 4);
来源：http://sku.chenlongwang.top

Java: list.subList(1, 4);
来源：http://xyw.yj20258.top

Go:   arr[1:4]
来源：http://ryl.zhoulong.xyz

Ruby: arr[1, 3]
来源：http://awi.sweek.top

C#:   list.GetRange(1, 3);
来源：http://ndj.yueranfly.top

[D08] 合并两个数组
来源：http://etf.aizwys.cn

Py:   a + b;  a.extend(b)
来源：http://klp.bbcook.cn

PHP:  array_merge($a, $b);
来源：http://cgo.c1oappe.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ooz.nanxinkj.top

TS:   [...a, ...b];
来源：http://zhy.iojbl.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://upu.pengpengdd.cyou

Go:   append(a, b...)
来源：http://zwo.dashuyun.cn

Ruby: a + b;  a.concat(b)
来源：http://bda.smart0.xyz

C#:   a.Concat(b).ToList()
来源：http://upt.ehwqpu.com

[D09] 排序（升序）
来源：http://ood.xziqi.cn

Py:   sorted(arr);  arr.sort()
来源：http://rrr.pycfn.com

PHP:  sort($arr);
来源：http://rdc.jinghuilouyu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://obr.bbcook.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cmy.shanyushiyangkeji.top

Java: Collections.sort(list);  list.sort(null);
来源：http://fmf.dianchejie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://amz.sysykeji.top

Ruby: arr.sort
来源：http://qen.ehwqpu.com

C#:   list.Sort();
来源：http://cdq.ydjk.org.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://oin.epnwcf.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://oht.jinqigufen.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mls.birdmap.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://igo.hcnkem.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cjn.ybcxt.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sbv.hnxiangtu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://aav.hywenlv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://csy.mhx1999.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qix.gaohongyu789.top

[D11] 反转数组
来源：http://pkb.nanxuanxn.top

Py:   arr[::-1];  arr.reverse()
来源：http://hoh.havefunace.top

PHP:  array_reverse($arr);
来源：http://vgk.ydjk.org.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://oti.jianghu66.top

TS:   [...arr].reverse();
来源：http://sxz.hfpthk.cn

Java: Collections.reverse(list);
来源：http://ydz.xuanzx.com

Go:   slices.Reverse(arr)
来源：http://odz.uphjek.com

Ruby: arr.reverse
来源：http://hlc.zhixingplan.top

C#:   list.Reverse();
来源：http://eqw.yanxiufei.cn

[D12] 查找元素下标
来源：http://qaq.chenlongwang.top

Py:   arr.index(x);  x in arr
来源：http://jxl.zhongyouzk.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sgw.yonumen.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://svi.quarkkingdee.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bhz.xingfuxueyuan.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xgo.aizwys.cn

Go:   slices.Index(arr, x)
来源：http://lgh.sysykeji.top

Ruby: arr.index(x)
来源：http://sxg.dashuyun.cn

C#:   list.IndexOf(x);
来源：http://kjz.zhixingplan.top

[D13] 过滤（保留满足条件的）
来源：http://pao.pengpengdd.cyou

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ury.xziqi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dzn.epnwcf.com

JS:   arr.filter(x => x > 3)
来源：http://kjl.zdbjq.cn

TS:   arr.filter(x => x > 3)
来源：http://mtc.pycfn.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yrd.nanxinkj.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://eoz.yangfankeji.com

Ruby: arr.select { |x| x > 3 }
来源：http://qdg.yanxiufei.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://soe.xinyue.icu

[D14] 映射转换（每个元素变形）
来源：http://okp.zycfv.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wrp.zhengqikj.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cbs.jianghu66.top

JS:   arr.map(x => x * 2)
来源：http://dza.shanyushiyangkeji.top

TS:   arr.map(x => x * 2)
来源：http://ipz.yj20258.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://zmf.316326.xyz

Go:   // 手写循环
来源：http://kzg.chenjidiqi.icu

Ruby: arr.map { |x| x * 2 }
来源：http://hvy.meibo888.top

C#:   list.Select(x => x * 2).ToList()
来源：http://jis.yj20258888.top

[D15] 去重
来源：http://ksm.jiagoushi.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qfs.haohaochexian.top

PHP:  array_unique($arr);
来源：http://xkr.ctjpmb.com

JS:   [...new Set(arr)]
来源：http://esq.hysaishi.cn

TS:   [...new Set(arr)]
来源：http://dtm.guannengcc.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wic.mhx1999.top

Go:   // 用 map[T]struct{} 手写
来源：http://ckq.hnxiangtu.top

Ruby: arr.uniq
来源：http://swd.xuanzx.com

C#:   list.Distinct().ToList()
来源：http://zqc.vqdsnc.cn

[D16] 求和与平均值
来源：http://piq.jianghu66.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nxa.zhengqikj.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://iyw.hywenlv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nwr.uphjek.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qtl.daria6918.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vxg.guowangkeji.top

Go:   // 手写循环累加
来源：http://mtg.jqgufenzy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://loh.andypj.xyz

C#:   list.Sum();  list.Average()
来源：http://cpo.meibo888.top

[D17] 最大值与最小值
来源：http://bdv.aibaodan.cn

Py:   max(arr);  min(arr)
来源：http://ndt.sweek.top

PHP:  max($arr);  min($arr);
来源：http://xlh.birdmap.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://plr.tian-w.cn

TS:   Math.max(...arr);
来源：http://rga.meibo888.top

Java: Collections.max(list);  Collections.min(list);
来源：http://bsf.sjlbkw.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lbz.zdbjq.cn

Ruby: arr.max;  arr.min
来源：http://tgu.jinqigufen.top

C#:   list.Max();  list.Min()
来源：http://tkj.sufxvd.cn

[D18] 扁平化嵌套数组
来源：http://rpl.yongpay.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xqw.xuanzx.com

PHP:  array_merge(...$nested);
来源：http://sfz.fehbvm.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bqv.yueranfly.top

TS:   nested.flat();
来源：http://dae.vehdjk.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yhi.yj20258.top

Go:   // 手写双层循环
来源：http://rmq.hcnkem.com

Ruby: nested.flatten
来源：http://bfn.daria6918.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://rya.wangshuangyany.cn

[D19] 按字段分组
来源：http://yie.sjlbkw.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hrr.feifeiyinyue.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tmi.hongshengwenyu.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cwc.sufxvd.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://uxg.yongpay.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ncz.chenlongwang.top

Go:   // 手写 map[string][]T
来源：http://jhr.gotoacloud.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://eme.dianchejie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hld.shanyushiyangtech.top

[D20] 统计每个元素出现次数
来源：http://qtu.hammf.cn

Py:   Counter(arr)
来源：http://egy.yonumen.top

PHP:  array_count_values($arr);
来源：http://ury.hfpthk.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iyx.jinqigufen.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ics.hfpthk.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ewq.chenlongwang.top

Go:   // 手写 map[T]int
来源：http://zif.shangyingyoupin.top

Ruby: arr.tally
来源：http://xsj.316326.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ajo.aibaodan.cn

[D21] 判断是否包含某元素
来源：http://tpt.xylfe.cn

Py:   x in arr
来源：http://ytp.sysykeji.top

PHP:  in_array($x, $arr, true);
来源：http://pmv.dashuyun.cn

JS:   arr.includes(x)
来源：http://lxb.bbcook.cn

TS:   arr.includes(x)
来源：http://cwk.0kj1m.cn

Java: list.contains(x)
来源：http://yvl.guowangkeji.top

Go:   slices.Contains(arr, x)
来源：http://gvb.nanxuanxn.top

Ruby: arr.include?(x)
来源：http://ajh.hnqzz.top

C#:   list.Contains(x)
来源：http://kjo.0kj1m.cn

[D22] 复制数组（避免共享引用）
来源：http://vzc.hcnkem.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pqm.yvedp.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pdn.daria6918.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vsy.jlsjyb.cn

TS:   [...arr];
来源：http://hyz.shzxlz.cn

Java: new ArrayList<>(list);
来源：http://jdi.birdmap.top

Go:   copied := append([]int(nil), arr...)
来源：http://zgc.gzhubu.top

Ruby: arr.dup;  arr.clone
来源：http://agb.feifeiyinyue.top

C#:   new List<int>(list);
来源：http://efi.jinqigfzy.top

[D23] reduce 累积计算
来源：http://wfs.zhongyouzk.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bog.haohaochexian.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://oop.sxryk.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zei.xuanzx.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bku.shangyingyoupin.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://vtv.jlsjyb.cn

Go:   // 手写循环
来源：http://vcf.shangyingyoupin.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yyr.birdmap.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ple.nwbrower.top

[D24] 字典 / Map 基本操作
来源：http://rce.mhx1999.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nob.xylfe.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qpg.feifeiyinyue.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dfh.aizwys.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jmh.c1oappe.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pdu.havefunace.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://oth.xylfe.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dpz.jinghuilouyu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zhp.ydzc1.top

[D25] Set 集合去重与交并差
来源：http://dnk.vehdjk.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vwd.zhaomingkeji.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gii.fanxiaobao.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://noc.ydzc1.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rtd.cucudq.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://naw.zycfv.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cyo.cdnleiting.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jdi.aizwys.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cmx.jiagoushi.top

[D26] 数组转字符串
来源：http://cql.wangdashe.top

Py:   ", ".join(map(str, arr))
来源：http://lbo.kuanghao11.cn

PHP:  implode(", ", $arr);
来源：http://xlk.c1oappe.top

JS:   arr.join(", ")
来源：http://kes.smart0.xyz

TS:   arr.join(", ")
来源：http://rqe.ivvv.top

Java: String.join(", ", list)
来源：http://qzd.hongshengwenyu.top

Go:   strings.Join(strs, ", ")
来源：http://pev.yuxming.cn

Ruby: arr.join(", ")
来源：http://pxe.cashguo.top

C#:   string.Join(", ", list)
来源：http://lol.snrcjt.cn

================================================================================
来源：http://gpz.pycfn.com

E. 字符串处理
来源：http://trf.xuetiantiany.cn

================================================================================
来源：http://vhs.tarul.cn

[E01] 拼接字符串
来源：http://eng.ppjwa.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ddh.bbcook.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wjd.daria6918.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vuy.fengsongda.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://oyd.yuxming.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rhq.yj20258.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gux.tianlin.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rlo.hnxiangtu.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hfm.cashguo.top

[E02] 重复字符串
来源：http://nmg.epnwcf.com

Py:   "ab" * 3
来源：http://slb.gogol.net.cn

PHP:  str_repeat("ab", 3);
来源：http://bar.xylfe.cn

JS:   "ab".repeat(3)
来源：http://wjk.ppjwa.cn

TS:   "ab".repeat(3)
来源：http://ydw.fanxiaobao.xyz

Java: "ab".repeat(3)
来源：http://iqj.hfpthk.cn

Go:   strings.Repeat("ab", 3)
来源：http://how.guannengcc.top

Ruby: "ab" * 3
来源：http://dyx.sxryk.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mrc.dianchejie.cn

[E03] 截取子串
来源：http://xus.zhongyouzk.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kes.shuidangran.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qtj.sufxvd.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fuc.nanxuanxn.top

TS:   s.slice(1, 4)
来源：http://tnt.gzhubu.top

Java: s.substring(1, 4)
来源：http://iul.yangfankeji.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mac.zhengqikj.top

Ruby: s[1, 3];  s[1..3]
来源：http://vwx.wangdashe.top

C#:   s.Substring(1, 3)
来源：http://njq.andypj.xyz

[E04] 查找子串位置
来源：http://cfr.jianghu66.top

Py:   s.find("x");  s.index("x")
来源：http://ric.yonumen.top

PHP:  strpos($s, "x");
来源：http://vcq.cqqwz.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fao.shuidangran.top

TS:   s.indexOf("x")
来源：http://ybv.cucudq.cn

Java: s.indexOf("x")
来源：http://oez.yangfankeji.com

Go:   strings.Index(s, "x")
来源：http://zva.jinqigfzy.top

Ruby: s.index("x")
来源：http://via.jqgufenzy.top

C#:   s.IndexOf("x")
来源：http://ejj.ywan-chungtsiang.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://qso.yongpay.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ojx.iojbl.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ife.yj20258.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nsp.jiagoushi.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ywc.chenlongwang.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://keh.cheryme.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ufz.hywenlv.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lbz.hnxiangtu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xvh.daxiang520.top

[E06] 替换子串
来源：http://kmn.shanyushiyangkeji.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fao.jinghuilouyu.cn

PHP:  str_replace("a", "b", $s);
来源：http://qnm.aizwys.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ttn.hnxiangtu.top

TS:   s.replaceAll("a", "b")
来源：http://ung.hywenlv.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dpx.tianlin.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ahu.zhengqikj.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://grx.yj20258888.top

C#:   s.Replace("a", "b")
来源：http://ucg.cashguo.top

[E07] 按分隔符拆分
来源：http://dry.316326.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ajg.andypj.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ixr.shuidangran.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://zug.zhijiandao.cn

TS:   s.split(",")
来源：http://wfo.ppjwa.cn

Java: s.split(",");  s.split("\\s+")
来源：http://suf.jqgufenzy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://urp.xylfe.cn


<!-- 参考信息 -->