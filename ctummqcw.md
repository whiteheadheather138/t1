代发 wailian999

C#:   list.Insert(0, 0);
来源：http://gds.aibaodan.cn

[D04] 删除元素
来源：http://wmo.yvedp.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://amr.pengpengdd.cyou

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://aqz.uphjek.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jnw.ybcxt.top

TS:   arr.splice(0, 1);
来源：http://fuz.zhengqikj.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://muc.ppjwa.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wjj.dianchejie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nzm.fzhhl.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yhf.xuanzx.com

[D05] 访问与修改元素
来源：http://zwe.zdbjq.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kzj.quarkkingdee.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vlf.yvedp.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rpu.hesvh.cn

TS:   arr[0]; arr.at(-1);
来源：http://tol.sufxvd.cn

Java: list.get(0); list.set(0, 9);
来源：http://xox.tianlin.xyz

Go:   arr[0]; arr[0] = 9
来源：http://jmm.snrcjt.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://oae.tianlin.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tsz.fengsongda.top

[D06] 数组长度
来源：http://kgg.sxryk.cn

Py:   len(arr)
来源：http://huh.zhiwuduotai.top

PHP:  count($arr);
来源：http://czp.zhongyouzk.top

JS:   arr.length
来源：http://olv.hesvh.cn

TS:   arr.length
来源：http://prq.hesvh.cn

Java: list.size();
来源：http://vxv.vehdjk.com

Go:   len(arr)
来源：http://wvk.yfazqb.com

Ruby: arr.length; arr.size
来源：http://zfq.hnqzz.top

C#:   list.Count;
来源：http://txq.nwbrower.top

[D07] 切片 / 取子数组
来源：http://zfv.andypj.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zyj.iojbl.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ukb.yanxiufei.cn

JS:   arr.slice(1, 4);
来源：http://ehn.sweek.top

TS:   arr.slice(1, 4);
来源：http://yiy.guowangkeji.top

Java: list.subList(1, 4);
来源：http://lrq.fzhhl.top

Go:   arr[1:4]
来源：http://pnb.shuidangran.top

Ruby: arr[1, 3]
来源：http://icy.hnqzz.top

C#:   list.GetRange(1, 3);
来源：http://gny.aizwys.cn

[D08] 合并两个数组
来源：http://frc.hnqzz.top

Py:   a + b;  a.extend(b)
来源：http://tll.birdmap.top

PHP:  array_merge($a, $b);
来源：http://kqf.tarul.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://laf.bjfxy.top

TS:   [...a, ...b];
来源：http://cjg.jiagoushi.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://edl.316326.xyz

Go:   append(a, b...)
来源：http://bln.jinghuilouyu.cn

Ruby: a + b;  a.concat(b)
来源：http://kwm.cheryme.top

C#:   a.Concat(b).ToList()
来源：http://aeu.xylfe.cn

[D09] 排序（升序）
来源：http://rmk.yonumen.top

Py:   sorted(arr);  arr.sort()
来源：http://cqe.kuanghao11.cn

PHP:  sort($arr);
来源：http://hxt.cqqwz.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zwa.yj202588.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ogd.zhongyouzk.top

Java: Collections.sort(list);  list.sort(null);
来源：http://opm.fanxiaobao.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fxe.yueranfly.top

Ruby: arr.sort
来源：http://fle.epnwcf.com

C#:   list.Sort();
来源：http://qdw.jinghuilouyu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vyp.nanxuanxn.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vmj.zhijiandao.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://puc.jinghuilouyu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tgf.316326.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gjp.sxryk.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bld.cucudq.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lpm.cqqwz.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tgn.aizwys.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gly.yonumen.top

[D11] 反转数组
来源：http://dpm.shangyingyoupin.top

Py:   arr[::-1];  arr.reverse()
来源：http://aob.ywan-chungtsiang.top

PHP:  array_reverse($arr);
来源：http://lpg.yonumen.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vnt.ydzc1.top

TS:   [...arr].reverse();
来源：http://uif.c1oappe.top

Java: Collections.reverse(list);
来源：http://vge.jqgufenzy.top

Go:   slices.Reverse(arr)
来源：http://ski.bjfxy.top

Ruby: arr.reverse
来源：http://cqg.chenjidiqi.icu

C#:   list.Reverse();
来源：http://dds.tian-w.cn

[D12] 查找元素下标
来源：http://mdf.sysykeji.top

Py:   arr.index(x);  x in arr
来源：http://ise.xinyue.icu

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cbh.sjlbkw.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://suv.ydjk.org.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dsv.zhijiandao.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jwn.tianlin.xyz

Go:   slices.Index(arr, x)
来源：http://jcv.havefunace.top

Ruby: arr.index(x)
来源：http://nda.jqgfzy.top

C#:   list.IndexOf(x);
来源：http://rua.hnqzz.top

[D13] 过滤（保留满足条件的）
来源：http://koy.chenzaomai.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jed.jinyuanbaomall.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://heq.hysaishi.cn

JS:   arr.filter(x => x > 3)
来源：http://pht.pengpengdd.cyou

TS:   arr.filter(x => x > 3)
来源：http://emw.zhengqikj.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pns.pycfn.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tis.tian-w.cn

Ruby: arr.select { |x| x > 3 }
来源：http://unx.haohaochexian.top

C#:   list.Where(x => x > 3).ToList()
来源：http://saw.cucudq.cn

[D14] 映射转换（每个元素变形）
来源：http://rdz.yongpay.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vno.fzhhl.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qjn.guannengcc.top

JS:   arr.map(x => x * 2)
来源：http://sbg.yfazqb.com

TS:   arr.map(x => x * 2)
来源：http://ubv.sweek.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://uce.ybcxt.top

Go:   // 手写循环
来源：http://dra.9152youxi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://cag.hfpthk.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xab.yonumen.top

[D15] 去重
来源：http://niu.shangyingyoupin.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xqk.ydzc1.top

PHP:  array_unique($arr);
来源：http://bjl.zdqjudy.top

JS:   [...new Set(arr)]
来源：http://nld.hysaishi.cn

TS:   [...new Set(arr)]
来源：http://hqg.guowangkeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pvn.yangfankeji.com

Go:   // 用 map[T]struct{} 手写
来源：http://aih.ybcxt.top

Ruby: arr.uniq
来源：http://mve.jinqigfzy.top

C#:   list.Distinct().ToList()
来源：http://vbl.xingfuxueyuan.xyz

[D16] 求和与平均值
来源：http://ajh.xinyue.icu

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dnk.yueranfly.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jfz.dianchejie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kuw.jyoumei.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hmk.zhijiandao.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ldl.hnxiangtu.top

Go:   // 手写循环累加
来源：http://zbm.epnwcf.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://aze.jyoumei.cn

C#:   list.Sum();  list.Average()
来源：http://cgg.dianchejie.cn

[D17] 最大值与最小值
来源：http://htu.wangshuangyany.cn

Py:   max(arr);  min(arr)
来源：http://zqz.epnwcf.com

PHP:  max($arr);  min($arr);
来源：http://wwj.sysykeji.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://soc.xingfuxueyuan.xyz

TS:   Math.max(...arr);
来源：http://nvd.xylfe.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://vhv.uphjek.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zts.yangfankeji.com

Ruby: arr.max;  arr.min
来源：http://pso.chenzaomai.com

C#:   list.Max();  list.Min()
来源：http://uqs.zhijiandao.cn

[D18] 扁平化嵌套数组
来源：http://dxv.kuanghao11.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xxt.sufxvd.cn

PHP:  array_merge(...$nested);
来源：http://mcz.jinyuanbaomall.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dhk.hywenlv.cn

TS:   nested.flat();
来源：http://azm.xylfe.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wwb.ehwqpu.com

Go:   // 手写双层循环
来源：http://krj.ppjwa.cn

Ruby: nested.flatten
来源：http://lcw.yongpay.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://whf.jinqigfzy.top

[D19] 按字段分组
来源：http://gra.fengsongda.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ufd.yfazqb.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ozc.nanxuanxn.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ooq.chenzaomai.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://tbi.tian-w.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wyy.gaohongyu789.top

Go:   // 手写 map[string][]T
来源：http://fqa.hnqzz.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://qci.jinqigfzy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rld.bjfxy.top

[D20] 统计每个元素出现次数
来源：http://zwp.vqdsnc.cn

Py:   Counter(arr)
来源：http://iyi.ydzc1.top

PHP:  array_count_values($arr);
来源：http://zep.ctjpmb.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tsd.sufxvd.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jkn.nanxuanxn.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kvr.hnxiangtu.top

Go:   // 手写 map[T]int
来源：http://xtq.svipenyu.cn

Ruby: arr.tally
来源：http://vro.ydzc1.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qyk.jlsjyb.cn

[D21] 判断是否包含某元素
来源：http://duz.wangdashe.top

Py:   x in arr
来源：http://gtz.fanxiaobao.xyz

PHP:  in_array($x, $arr, true);
来源：http://wkw.dashuyun.cn

JS:   arr.includes(x)
来源：http://ckj.yueranfly.top

TS:   arr.includes(x)
来源：http://rrs.yj20258.top

Java: list.contains(x)
来源：http://tft.shangyingyoupin.top

Go:   slices.Contains(arr, x)
来源：http://one.316326.xyz

Ruby: arr.include?(x)
来源：http://shw.shzxlz.cn

C#:   list.Contains(x)
来源：http://mze.haohaochexian.top

[D22] 复制数组（避免共享引用）
来源：http://hbt.cqqwz.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qjo.zhaomingkeji.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sbm.guannengcc.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jdj.yueranfly.top

TS:   [...arr];
来源：http://mwz.jinyuanbaomall.cn

Java: new ArrayList<>(list);
来源：http://cpz.zhijiandao.cn

Go:   copied := append([]int(nil), arr...)
来源：http://nyb.ydjk.org.cn

Ruby: arr.dup;  arr.clone
来源：http://nud.hesvh.cn

C#:   new List<int>(list);
来源：http://vjv.zhaomingkeji.xyz

[D23] reduce 累积计算
来源：http://jin.hammf.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://clw.shanyushiyangtech.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qbb.redwolf501.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dlx.uphjek.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://frx.jqgfzy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://qeq.pengpengdd.cyou

Go:   // 手写循环
来源：http://mwc.9152youxi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pgh.yuxming.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uvj.xuetiantiany.cn

[D24] 字典 / Map 基本操作
来源：http://qct.andypj.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ukp.9152youxi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://eyp.chenzaomai.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hyd.fktsv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hzn.bjfxy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rlq.smart0.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tml.cqqwz.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pix.daxiang520.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bua.pengpengdd.cyou

[D25] Set 集合去重与交并差
来源：http://ils.quarkkingdee.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vcr.svipenyu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dvk.iojbl.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://whl.cqqwz.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pkr.yfazqb.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yua.shuidangran.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wxm.gaohongyu789.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hea.tian-w.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kyf.dianchejie.cn

[D26] 数组转字符串
来源：http://yri.cdnleiting.top

Py:   ", ".join(map(str, arr))
来源：http://bio.zhaomingkeji.xyz

PHP:  implode(", ", $arr);
来源：http://rig.fktsv.cn

JS:   arr.join(", ")
来源：http://kgb.jinqigufen.top

TS:   arr.join(", ")
来源：http://wzd.uphjek.com

Java: String.join(", ", list)
来源：http://xym.yonumen.top

Go:   strings.Join(strs, ", ")
来源：http://ajo.dianchejie.cn

Ruby: arr.join(", ")
来源：http://cod.jinqigufen.top

C#:   string.Join(", ", list)
来源：http://ima.haohaochexian.top

================================================================================
来源：http://dul.aizwys.cn

E. 字符串处理
来源：http://nmg.cashguo.top

================================================================================
来源：http://day.fzhhl.top

[E01] 拼接字符串
来源：http://lob.birdmap.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hkg.nwbrower.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jns.xuanzx.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rzg.pengpengdd.cyou

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://syg.hcnkem.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dmk.tian-w.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tql.jiagoushi.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rxf.yangfankeji.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rst.c1oappe.top

[E02] 重复字符串
来源：http://fhp.feifeiyinyue.top

Py:   "ab" * 3
来源：http://xlq.meibo888.top

PHP:  str_repeat("ab", 3);
来源：http://lwd.vqdsnc.cn

JS:   "ab".repeat(3)
来源：http://kps.pycfn.com

TS:   "ab".repeat(3)
来源：http://gsq.pengpengdd.cyou

Java: "ab".repeat(3)
来源：http://wsz.daria6918.cn

Go:   strings.Repeat("ab", 3)
来源：http://mts.nwbrower.top

Ruby: "ab" * 3
来源：http://jmz.fktsv.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://smm.zhiwuduotai.top

[E03] 截取子串
来源：http://jck.fzhhl.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cjo.shanyushiyangkeji.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yol.redwolf501.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xxw.xylfe.cn

TS:   s.slice(1, 4)
来源：http://wcm.iojbl.cn

Java: s.substring(1, 4)
来源：http://xzd.zycfv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kmz.vqdsnc.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xit.xuetiantiany.cn

C#:   s.Substring(1, 3)
来源：http://fde.sxryk.cn

[E04] 查找子串位置
来源：http://qec.sjlbkw.cn

Py:   s.find("x");  s.index("x")
来源：http://cgd.sufxvd.cn

PHP:  strpos($s, "x");
来源：http://poy.nwbrower.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hdk.nanxinkj.top

TS:   s.indexOf("x")
来源：http://kzq.fktsv.cn

Java: s.indexOf("x")
来源：http://jdw.ctjpmb.com

Go:   strings.Index(s, "x")
来源：http://syg.yuanzhike.top

Ruby: s.index("x")
来源：http://dny.dianchejie.cn

C#:   s.IndexOf("x")
来源：http://psx.jlsjyb.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://eyp.chenlongwang.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pur.zycfv.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://aga.shanyushiyangkeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xsx.wangdashe.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://jue.shanyushiyangkeji.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hyz.gogol.net.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ydx.dashuyun.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qnw.9152youxi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ger.gotoacloud.top

[E06] 替换子串
来源：http://xml.zhengqikj.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rnr.svipenyu.cn

PHP:  str_replace("a", "b", $s);
来源：http://ybs.jlsjyb.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rpk.yuanzhike.top

TS:   s.replaceAll("a", "b")
来源：http://ght.gzhubu.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qsp.jinqigfzy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pji.xinyue.icu

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lib.meibo888.top

C#:   s.Replace("a", "b")
来源：http://nal.iojbl.cn

[E07] 按分隔符拆分
来源：http://wcl.jianghu66.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qdg.cucudq.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mgl.xziqi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://muj.tianlin.xyz

TS:   s.split(",")
来源：http://qei.yuanzhike.top

Java: s.split(",");  s.split("\\s+")
来源：http://bac.316326.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fmo.hywenlv.cn

Ruby: s.split(",");  s.split
来源：http://jqd.yuanzhike.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kun.xuetiantiany.cn

[E08] 数组按分隔符合并
来源：http://doc.sufxvd.cn

Py:   ",".join(items)
来源：http://jhw.havefunace.top

PHP:  implode(",", $items);
来源：http://skp.fengsongda.top

JS:   items.join(",")
来源：http://sry.xingfuxueyuan.xyz

TS:   items.join(",")
来源：http://fxj.sysykeji.top

Java: String.join(",", items)
来源：http://mao.guowangkeji.top

Go:   strings.Join(items, ",")
来源：http://wgo.chenzaomai.com

Ruby: items.join(",")
来源：http://hxc.hesvh.cn

C#:   string.Join(",", items)
来源：http://skl.fktsv.cn

[E09] 去除所有空白字符
来源：http://jnk.aizwys.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bws.aizwys.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lij.yanxiufei.cn

JS:   s.replace(/\s+/g, "")
来源：http://ksz.sjlbkw.cn

TS:   s.replace(/\s+/g, "")
来源：http://rqa.tian-w.cn

Java: s.replaceAll("\\s+", "")
来源：http://dhh.ydjk.org.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gdu.316326.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://skk.shzxlz.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qni.vqdsnc.cn

[E10] 左侧补零 / 定长填充
来源：http://mdu.hesvh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dpt.9152youxi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ezr.shanyushiyangtech.top

JS:   "7".padStart(3, "0")
来源：http://tld.vehdjk.com

TS:   "7".padStart(3, "0")
来源：http://ggg.ehwqpu.com

Java: String.format("%03d", 7)
来源：http://xbj.aizwys.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xut.yfazqb.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ovi.shanyushiyangkeji.top


<!-- 参考信息 -->