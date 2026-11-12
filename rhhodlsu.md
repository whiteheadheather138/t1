代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pzf.zhixingplan.top

TS:   arr.splice(0, 1);
来源：http://gby.chenzaomai.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ksd.sxryk.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://skw.svipenyu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://awx.xinyue.icu

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jqr.jqgfzy.top

[D05] 访问与修改元素
来源：http://icf.iojbl.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://otr.zhengqikj.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pxb.hywenlv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gqf.shanyushiyangtech.top

TS:   arr[0]; arr.at(-1);
来源：http://ebi.ctjpmb.com

Java: list.get(0); list.set(0, 9);
来源：http://bzn.haohaochexian.top

Go:   arr[0]; arr[0] = 9
来源：http://gwl.sufxvd.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yga.shzxlz.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pwr.ctjpmb.com

[D06] 数组长度
来源：http://zpu.jinghuilouyu.cn

Py:   len(arr)
来源：http://qrd.yfazqb.com

PHP:  count($arr);
来源：http://clc.yonumen.top

JS:   arr.length
来源：http://xtr.hfpthk.cn

TS:   arr.length
来源：http://lvf.jinyuanbaomall.cn

Java: list.size();
来源：http://ote.tianlin.xyz

Go:   len(arr)
来源：http://fdj.uphjek.com

Ruby: arr.length; arr.size
来源：http://gef.jqgfzy.top

C#:   list.Count;
来源：http://rdw.xylfe.cn

[D07] 切片 / 取子数组
来源：http://jhg.fktsv.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xak.vehdjk.com

PHP:  array_slice($arr, 1, 3);
来源：http://gfa.cdnleiting.top

JS:   arr.slice(1, 4);
来源：http://yis.chenlongwang.top

TS:   arr.slice(1, 4);
来源：http://rhe.fanxiaobao.xyz

Java: list.subList(1, 4);
来源：http://lck.tarul.cn

Go:   arr[1:4]
来源：http://uiz.ivvv.top

Ruby: arr[1, 3]
来源：http://bva.hammf.cn

C#:   list.GetRange(1, 3);
来源：http://lry.yj20258.top

[D08] 合并两个数组
来源：http://trq.vqdsnc.cn

Py:   a + b;  a.extend(b)
来源：http://fbb.zhixingplan.top

PHP:  array_merge($a, $b);
来源：http://gty.sjlbkw.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wqy.yj202588.top

TS:   [...a, ...b];
来源：http://npx.jqgufenzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jae.gaohongyu789.top

Go:   append(a, b...)
来源：http://ryx.zhijiandao.cn

Ruby: a + b;  a.concat(b)
来源：http://vhu.xingfuxueyuan.xyz

C#:   a.Concat(b).ToList()
来源：http://eap.zdqjudy.top

[D09] 排序（升序）
来源：http://row.yvedp.cn

Py:   sorted(arr);  arr.sort()
来源：http://tmy.ppjwa.cn

PHP:  sort($arr);
来源：http://ysl.xuetiantiany.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zjh.yfazqb.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://xjt.yongpay.top

Java: Collections.sort(list);  list.sort(null);
来源：http://dgl.uphjek.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ekm.sjlbkw.cn

Ruby: arr.sort
来源：http://ati.yj202588.top

C#:   list.Sort();
来源：http://gkx.feifeiyinyue.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ygo.hfpthk.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ufb.fanxiaobao.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oho.gogol.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jae.zdqjudy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://owg.yfazqb.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pcn.cqqwz.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gwy.52xcode.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wje.quarkkingdee.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://giv.yangfankeji.com

[D11] 反转数组
来源：http://fza.dashuyun.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xyu.jyoumei.cn

PHP:  array_reverse($arr);
来源：http://fal.xziqi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://crx.fzhhl.top

TS:   [...arr].reverse();
来源：http://fne.jinqigfzy.top

Java: Collections.reverse(list);
来源：http://pzz.tarul.cn

Go:   slices.Reverse(arr)
来源：http://dgu.cucudq.cn

Ruby: arr.reverse
来源：http://bdt.316326.xyz

C#:   list.Reverse();
来源：http://udc.zhengqikj.top

[D12] 查找元素下标
来源：http://rsl.cqqwz.cn

Py:   arr.index(x);  x in arr
来源：http://kud.shzxlz.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mju.yfazqb.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://brg.guannengcc.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wrt.zdbjq.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tqg.yj20258.top

Go:   slices.Index(arr, x)
来源：http://qxe.redwolf501.top

Ruby: arr.index(x)
来源：http://lkq.cucudq.cn

C#:   list.IndexOf(x);
来源：http://par.cheryme.top

[D13] 过滤（保留满足条件的）
来源：http://wna.daxiang520.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ogy.jyoumei.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cxd.tianlin.xyz

JS:   arr.filter(x => x > 3)
来源：http://hgf.xziqi.cn

TS:   arr.filter(x => x > 3)
来源：http://npr.uphjek.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qii.birdmap.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ovl.zhengqikj.top

Ruby: arr.select { |x| x > 3 }
来源：http://lpp.yueranfly.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ues.fengsongda.top

[D14] 映射转换（每个元素变形）
来源：http://cgh.xingfuxueyuan.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://prx.ybcxt.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nwa.epnwcf.com

JS:   arr.map(x => x * 2)
来源：http://dew.tianlin.xyz

TS:   arr.map(x => x * 2)
来源：http://kci.guowangkeji.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ors.feifeiyinyue.top

Go:   // 手写循环
来源：http://vby.uphjek.com

Ruby: arr.map { |x| x * 2 }
来源：http://jcs.wangshuangyany.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://oxt.tianlin.xyz

[D15] 去重
来源：http://xab.yvedp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://iop.epnwcf.com

PHP:  array_unique($arr);
来源：http://jrc.zhiwuduotai.top

JS:   [...new Set(arr)]
来源：http://gfq.ppjwa.cn

TS:   [...new Set(arr)]
来源：http://uhs.cashguo.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://znw.shuidangran.top

Go:   // 用 map[T]struct{} 手写
来源：http://skp.ybcxt.top

Ruby: arr.uniq
来源：http://dgc.gaohongyu789.top

C#:   list.Distinct().ToList()
来源：http://awh.daria6918.cn

[D16] 求和与平均值
来源：http://knv.hcnkem.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fcq.wangshuangyany.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bdy.daria6918.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xwa.hnxiangtu.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fyt.jinghuilouyu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://phk.bbcook.cn

Go:   // 手写循环累加
来源：http://yyw.redwolf501.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ylm.jqgufenzy.top

C#:   list.Sum();  list.Average()
来源：http://lsf.cdnleiting.top

[D17] 最大值与最小值
来源：http://uqe.aibaodan.cn

Py:   max(arr);  min(arr)
来源：http://qob.bjfxy.top

PHP:  max($arr);  min($arr);
来源：http://kdx.jqgufenzy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zem.tanke756.top

TS:   Math.max(...arr);
来源：http://xuz.havefunace.top

Java: Collections.max(list);  Collections.min(list);
来源：http://mll.cdnleiting.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zlk.hesvh.cn

Ruby: arr.max;  arr.min
来源：http://ytm.ppjwa.cn

C#:   list.Max();  list.Min()
来源：http://sit.meibo888.top

[D18] 扁平化嵌套数组
来源：http://hyz.316326.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cbl.yj202588.top

PHP:  array_merge(...$nested);
来源：http://icx.guowangkeji.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://efv.yj202588.top

TS:   nested.flat();
来源：http://tib.zhongyouzk.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kvp.316326.xyz

Go:   // 手写双层循环
来源：http://hpb.zhongyouzk.top

Ruby: nested.flatten
来源：http://ywa.gaohongyu789.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://muj.iojbl.cn

[D19] 按字段分组
来源：http://xdd.andypj.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wht.ivvv.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://opd.jqgufenzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rne.dianchejie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fof.hesvh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zaf.epnwcf.com

Go:   // 手写 map[string][]T
来源：http://vnp.jinqigfzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://mri.aibaodan.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fuu.gzhubu.top

[D20] 统计每个元素出现次数
来源：http://fkn.zhongyouzk.top

Py:   Counter(arr)
来源：http://vhl.chenlongwang.top

PHP:  array_count_values($arr);
来源：http://rxa.dashuyun.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ixd.hysaishi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qvs.feifeiyinyue.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ltk.gotoacloud.top

Go:   // 手写 map[T]int
来源：http://arn.nwbrower.top

Ruby: arr.tally
来源：http://dvz.fzhhl.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qiq.tianlin.xyz

[D21] 判断是否包含某元素
来源：http://mew.shanyushiyangkeji.top

Py:   x in arr
来源：http://zji.yfazqb.com

PHP:  in_array($x, $arr, true);
来源：http://bsg.iojbl.cn

JS:   arr.includes(x)
来源：http://ifd.tianlin.xyz

TS:   arr.includes(x)
来源：http://tsv.havefunace.top

Java: list.contains(x)
来源：http://oxe.ehwqpu.com

Go:   slices.Contains(arr, x)
来源：http://ist.zdqjudy.top

Ruby: arr.include?(x)
来源：http://rsm.jqgufenzy.top

C#:   list.Contains(x)
来源：http://kbi.ydjk.org.cn

[D22] 复制数组（避免共享引用）
来源：http://zdh.chenzaomai.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mqi.gzhubu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dsz.yj20258888.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://psg.hywenlv.cn

TS:   [...arr];
来源：http://gkq.sufxvd.cn

Java: new ArrayList<>(list);
来源：http://pqx.hysaishi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ggo.epnwcf.com

Ruby: arr.dup;  arr.clone
来源：http://hcy.zhongyouzk.top

C#:   new List<int>(list);
来源：http://fue.yongpay.top

[D23] reduce 累积计算
来源：http://fin.hnxiangtu.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sgp.yanxiufei.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ezq.jinqigfzy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cwp.cqqwz.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://auu.gotoacloud.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://mii.xylfe.cn

Go:   // 手写循环
来源：http://luh.52xcode.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://guu.jlsjyb.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jrn.fanxiaobao.xyz

[D24] 字典 / Map 基本操作
来源：http://wgs.ydjk.org.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://oeh.smart0.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zvl.shanyushiyangkeji.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dnv.hcnkem.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nfc.jinyuanbaomall.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bee.ydzc1.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sqe.tianlin.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cmc.jinghuilouyu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tlk.sjlbkw.cn

[D25] Set 集合去重与交并差
来源：http://oum.ydzc1.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dgt.c1oappe.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kch.cqqwz.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://akj.jinghuilouyu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dse.316326.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ark.daria6918.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qdj.snrcjt.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://icp.sufxvd.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://iwl.ydjk.org.cn

[D26] 数组转字符串
来源：http://zmp.yj20258.top

Py:   ", ".join(map(str, arr))
来源：http://nyh.jinqigufen.top

PHP:  implode(", ", $arr);
来源：http://zve.chenlongwang.top

JS:   arr.join(", ")
来源：http://nhk.haohaochexian.top

TS:   arr.join(", ")
来源：http://pdu.hfpthk.cn

Java: String.join(", ", list)
来源：http://wny.hnxiangtu.top

Go:   strings.Join(strs, ", ")
来源：http://zcc.dashuyun.cn

Ruby: arr.join(", ")
来源：http://nym.jinghuilouyu.cn

C#:   string.Join(", ", list)
来源：http://csa.xylfe.cn

================================================================================
来源：http://blv.daxiang520.top

E. 字符串处理
来源：http://utg.jqgufenzy.top

================================================================================
来源：http://gpe.fanxiaobao.xyz

[E01] 拼接字符串
来源：http://ftb.yfazqb.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tix.xziqi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://eks.quarkkingdee.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cci.yj202588.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hot.yuxming.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://btd.meibo888.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uxz.jlsjyb.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yuc.zhixingplan.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zbu.zhoulong.xyz

[E02] 重复字符串
来源：http://lqi.yongpay.top

Py:   "ab" * 3
来源：http://gns.aizwys.cn

PHP:  str_repeat("ab", 3);
来源：http://iia.yuxming.cn

JS:   "ab".repeat(3)
来源：http://ihv.yuxming.cn

TS:   "ab".repeat(3)
来源：http://auw.aizwys.cn

Java: "ab".repeat(3)
来源：http://fqg.haohaochexian.top

Go:   strings.Repeat("ab", 3)
来源：http://urp.yj20258888.top

Ruby: "ab" * 3
来源：http://imz.pengpengdd.cyou

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bzp.tarul.cn

[E03] 截取子串
来源：http://aog.hcnkem.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://grj.shangyingyoupin.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wyb.hongshengwenyu.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nop.yangfankeji.com

TS:   s.slice(1, 4)
来源：http://sbt.ydjk.org.cn

Java: s.substring(1, 4)
来源：http://zbw.shzxlz.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ujr.pengpengdd.cyou

Ruby: s[1, 3];  s[1..3]
来源：http://nsi.jinqigfzy.top

C#:   s.Substring(1, 3)
来源：http://ekq.wangdashe.top

[E04] 查找子串位置
来源：http://mjl.jyoumei.cn

Py:   s.find("x");  s.index("x")
来源：http://xio.zycfv.cn

PHP:  strpos($s, "x");
来源：http://wuf.xylfe.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cjb.zhixingplan.top

TS:   s.indexOf("x")
来源：http://ucl.zdqjudy.top

Java: s.indexOf("x")
来源：http://jdi.ydzc1.top

Go:   strings.Index(s, "x")
来源：http://tws.daxiang520.top

Ruby: s.index("x")
来源：http://prc.jinqigufen.top

C#:   s.IndexOf("x")
来源：http://wsj.xylfe.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://sag.vqdsnc.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zml.feifeiyinyue.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zup.ydzc1.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ovx.xuetiantiany.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zzb.uphjek.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sow.yanxiufei.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://aqm.birdmap.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://oqf.bjfxy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://oic.jinqigufen.top

[E06] 替换子串
来源：http://ckr.chenzaomai.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dse.bjfxy.top

PHP:  str_replace("a", "b", $s);
来源：http://fyn.chenlongwang.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vun.svipenyu.cn

TS:   s.replaceAll("a", "b")
来源：http://xka.sjlbkw.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pss.epnwcf.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bin.smart0.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://aqc.shangyingyoupin.top

C#:   s.Replace("a", "b")
来源：http://lbs.pycfn.com

[E07] 按分隔符拆分
来源：http://jus.hnqzz.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ojh.ywan-chungtsiang.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://evn.52xcode.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jcd.jqgfzy.top

TS:   s.split(",")
来源：http://xej.jqgufenzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://chz.hnxiangtu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zhl.zhengqikj.top

Ruby: s.split(",");  s.split
来源：http://bln.ydjk.org.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pon.xziqi.cn

[E08] 数组按分隔符合并
来源：http://ryq.jianghu66.top

Py:   ",".join(items)
来源：http://obh.yuxming.cn

PHP:  implode(",", $items);
来源：http://bzi.sjlbkw.cn

JS:   items.join(",")
来源：http://kyc.cashguo.top

TS:   items.join(",")
来源：http://irb.sysykeji.top

Java: String.join(",", items)
来源：http://dqs.svipenyu.cn

Go:   strings.Join(items, ",")
来源：http://jmx.redwolf501.top

Ruby: items.join(",")
来源：http://oqz.hongshengwenyu.top

C#:   string.Join(",", items)
来源：http://rga.andypj.xyz

[E09] 去除所有空白字符
来源：http://qlg.yj202588.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://atz.daxiang520.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fao.fzhhl.top

JS:   s.replace(/\s+/g, "")
来源：http://eht.fengsongda.top

TS:   s.replace(/\s+/g, "")
来源：http://lgw.dashuyun.cn

Java: s.replaceAll("\\s+", "")
来源：http://gir.snrcjt.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ahj.wangshuangyany.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ptc.yongpay.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fat.iojbl.cn

[E10] 左侧补零 / 定长填充
来源：http://iqz.fehbvm.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hoj.pycfn.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ycv.yj20258888.top

JS:   "7".padStart(3, "0")
来源：http://lsy.uphjek.com

TS:   "7".padStart(3, "0")
来源：http://ekd.ivvv.top

Java: String.format("%03d", 7)
来源：http://lae.xziqi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://kri.yonumen.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dfx.uphjek.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tra.shanyushiyangtech.top

[E11] 反转字符串
来源：http://zru.hammf.cn

Py:   s[::-1]
来源：http://lcb.hywenlv.cn

PHP:  strrev($s);
来源：http://mhu.hammf.cn


<!-- 参考信息 -->