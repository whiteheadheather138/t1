代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://sbh.yueranfly.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nmi.haohaochexian.top

[D05] 访问与修改元素
来源：http://dnv.shanyushiyangtech.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ssi.sjlbkw.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dtu.snrcjt.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jnv.hnqzz.top

TS:   arr[0]; arr.at(-1);
来源：http://acr.jyoumei.cn

Java: list.get(0); list.set(0, 9);
来源：http://yoj.yj20258888.top

Go:   arr[0]; arr[0] = 9
来源：http://zwp.xziqi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://giq.daxiang520.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kob.tian-w.cn

[D06] 数组长度
来源：http://jos.ctjpmb.com

Py:   len(arr)
来源：http://gzd.xingfuxueyuan.xyz

PHP:  count($arr);
来源：http://lal.wangshuangyany.cn

JS:   arr.length
来源：http://kba.xuetiantiany.cn

TS:   arr.length
来源：http://mjn.0kj1m.cn

Java: list.size();
来源：http://mwx.zdbjq.cn

Go:   len(arr)
来源：http://oiu.yuxming.cn

Ruby: arr.length; arr.size
来源：http://fjs.ivvv.top

C#:   list.Count;
来源：http://prc.xinyue.icu

[D07] 切片 / 取子数组
来源：http://xuq.shanyushiyangkeji.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jeg.jinqigfzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://kfu.jlsjyb.cn

JS:   arr.slice(1, 4);
来源：http://ini.birdmap.top

TS:   arr.slice(1, 4);
来源：http://efv.hesvh.cn

Java: list.subList(1, 4);
来源：http://btu.hongshengwenyu.top

Go:   arr[1:4]
来源：http://vuo.jinqigfzy.top

Ruby: arr[1, 3]
来源：http://vqx.xziqi.cn

C#:   list.GetRange(1, 3);
来源：http://aen.shangyingyoupin.top

[D08] 合并两个数组
来源：http://cav.quarkkingdee.top

Py:   a + b;  a.extend(b)
来源：http://ygi.cashguo.top

PHP:  array_merge($a, $b);
来源：http://wem.daria6918.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vcg.bbcook.cn

TS:   [...a, ...b];
来源：http://hel.ivvv.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ybn.ybcxt.top

Go:   append(a, b...)
来源：http://snu.ivvv.top

Ruby: a + b;  a.concat(b)
来源：http://awt.zhengqikj.top

C#:   a.Concat(b).ToList()
来源：http://kuh.yueranfly.top

[D09] 排序（升序）
来源：http://jbq.chenzaomai.com

Py:   sorted(arr);  arr.sort()
来源：http://lmy.ydjk.org.cn

PHP:  sort($arr);
来源：http://xle.zhiwuduotai.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bsj.aibaodan.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://klf.yueranfly.top

Java: Collections.sort(list);  list.sort(null);
来源：http://fsy.ydjk.org.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bfu.pengpengdd.cyou

Ruby: arr.sort
来源：http://rit.cqqwz.cn

C#:   list.Sort();
来源：http://jqd.hongshengwenyu.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://dmj.pengpengdd.cyou

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nic.nanxuanxn.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mnm.hywenlv.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wqq.cdnleiting.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fkk.hnqzz.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zlx.shuidangran.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qrc.316326.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jsf.ywan-chungtsiang.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://srn.zhixingplan.top

[D11] 反转数组
来源：http://oxc.shanyushiyangkeji.top

Py:   arr[::-1];  arr.reverse()
来源：http://hqy.shzxlz.cn

PHP:  array_reverse($arr);
来源：http://kmm.smart0.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://eop.cucudq.cn

TS:   [...arr].reverse();
来源：http://pqb.zycfv.cn

Java: Collections.reverse(list);
来源：http://gae.jqgufenzy.top

Go:   slices.Reverse(arr)
来源：http://fcu.haohaochexian.top

Ruby: arr.reverse
来源：http://hpj.shanyushiyangtech.top

C#:   list.Reverse();
来源：http://dkz.ydjk.org.cn

[D12] 查找元素下标
来源：http://wyb.ppjwa.cn

Py:   arr.index(x);  x in arr
来源：http://uzs.jinghuilouyu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pxn.vehdjk.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hky.ivvv.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pgb.yueranfly.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ojm.bbcook.cn

Go:   slices.Index(arr, x)
来源：http://qza.hnqzz.top

Ruby: arr.index(x)
来源：http://mhu.zdbjq.cn

C#:   list.IndexOf(x);
来源：http://utx.wangshuangyany.cn

[D13] 过滤（保留满足条件的）
来源：http://ewk.sxryk.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vgj.nwbrower.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dqv.birdmap.top

JS:   arr.filter(x => x > 3)
来源：http://yhk.yuxming.cn

TS:   arr.filter(x => x > 3)
来源：http://nux.nanxinkj.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pfi.gaohongyu789.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ete.gzhubu.top

Ruby: arr.select { |x| x > 3 }
来源：http://opf.ywan-chungtsiang.top

C#:   list.Where(x => x > 3).ToList()
来源：http://tev.c1oappe.top

[D14] 映射转换（每个元素变形）
来源：http://atm.shanyushiyangkeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ckt.kuanghao11.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dwd.shanyushiyangkeji.top

JS:   arr.map(x => x * 2)
来源：http://xrq.guowangkeji.top

TS:   arr.map(x => x * 2)
来源：http://eek.gogol.net.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zct.gogol.net.cn

Go:   // 手写循环
来源：http://wqj.zhengqikj.top

Ruby: arr.map { |x| x * 2 }
来源：http://ube.gotoacloud.top

C#:   list.Select(x => x * 2).ToList()
来源：http://jts.iojbl.cn

[D15] 去重
来源：http://nqh.mhx1999.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ikj.jinqigfzy.top

PHP:  array_unique($arr);
来源：http://zfn.yonumen.top

JS:   [...new Set(arr)]
来源：http://nrj.jqgufenzy.top

TS:   [...new Set(arr)]
来源：http://klx.shanyushiyangtech.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mrn.aibaodan.cn

Go:   // 用 map[T]struct{} 手写
来源：http://jwm.jqgufenzy.top

Ruby: arr.uniq
来源：http://czh.sweek.top

C#:   list.Distinct().ToList()
来源：http://ozj.dashuyun.cn

[D16] 求和与平均值
来源：http://uuu.cashguo.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mxw.quarkkingdee.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xcc.fzhhl.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ncl.tian-w.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hfh.0kj1m.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uyk.hnqzz.top

Go:   // 手写循环累加
来源：http://khq.xylfe.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vcb.sjlbkw.cn

C#:   list.Sum();  list.Average()
来源：http://jxm.hnxiangtu.top

[D17] 最大值与最小值
来源：http://ahs.hammf.cn

Py:   max(arr);  min(arr)
来源：http://hba.birdmap.top

PHP:  max($arr);  min($arr);
来源：http://rzh.nanxinkj.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yxb.cdnleiting.top

TS:   Math.max(...arr);
来源：http://obw.bbcook.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rok.fanxiaobao.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qfj.gogol.net.cn

Ruby: arr.max;  arr.min
来源：http://tsv.epnwcf.com

C#:   list.Max();  list.Min()
来源：http://jiq.sjlbkw.cn

[D18] 扁平化嵌套数组
来源：http://jrw.xingfuxueyuan.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ewv.sufxvd.cn

PHP:  array_merge(...$nested);
来源：http://pvx.birdmap.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xep.fktsv.cn

TS:   nested.flat();
来源：http://hft.ehwqpu.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bri.jiagoushi.top

Go:   // 手写双层循环
来源：http://ikf.jqgufenzy.top

Ruby: nested.flatten
来源：http://cee.shanyushiyangkeji.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://zhx.gaohongyu789.top

[D19] 按字段分组
来源：http://rjc.wangshuangyany.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vtj.jqgfzy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mpv.yuanzhike.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ult.iojbl.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vnm.zdbjq.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wha.hongshengwenyu.top

Go:   // 手写 map[string][]T
来源：http://puv.tanke756.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://fzp.jiagoushi.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://usd.zhixingplan.top

[D20] 统计每个元素出现次数
来源：http://abf.vehdjk.com

Py:   Counter(arr)
来源：http://sfb.fzhhl.top

PHP:  array_count_values($arr);
来源：http://ntf.meibo888.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qgw.nanxinkj.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pth.yangfankeji.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://amn.hesvh.cn

Go:   // 手写 map[T]int
来源：http://kqu.hnqzz.top

Ruby: arr.tally
来源：http://fix.epnwcf.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qpb.hcnkem.com

[D21] 判断是否包含某元素
来源：http://amf.cqqwz.cn

Py:   x in arr
来源：http://bmu.shuidangran.top

PHP:  in_array($x, $arr, true);
来源：http://rov.epnwcf.com

JS:   arr.includes(x)
来源：http://trs.ehwqpu.com

TS:   arr.includes(x)
来源：http://jji.andypj.xyz

Java: list.contains(x)
来源：http://hnp.fzhhl.top

Go:   slices.Contains(arr, x)
来源：http://bpg.fzhhl.top

Ruby: arr.include?(x)
来源：http://uwu.smart0.xyz

C#:   list.Contains(x)
来源：http://tqw.jyoumei.cn

[D22] 复制数组（避免共享引用）
来源：http://sct.feifeiyinyue.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lnx.jianghu66.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tms.tianlin.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rob.fehbvm.com

TS:   [...arr];
来源：http://yrr.tian-w.cn

Java: new ArrayList<>(list);
来源：http://kqd.aizwys.cn

Go:   copied := append([]int(nil), arr...)
来源：http://jqe.ydzc1.top

Ruby: arr.dup;  arr.clone
来源：http://kis.yanxiufei.cn

C#:   new List<int>(list);
来源：http://lrp.jinqigfzy.top

[D23] reduce 累积计算
来源：http://aed.hnqzz.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rna.feifeiyinyue.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://erp.epnwcf.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xvw.haohaochexian.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yua.0kj1m.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rtn.kuanghao11.cn

Go:   // 手写循环
来源：http://cie.hesvh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jie.cdnleiting.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qbs.guowangkeji.top

[D24] 字典 / Map 基本操作
来源：http://hnq.hywenlv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hnx.zdqjudy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xkj.pycfn.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lgh.hywenlv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://moz.jinqigufen.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ycc.uphjek.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ouy.fktsv.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ick.yonumen.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tmm.shuidangran.top

[D25] Set 集合去重与交并差
来源：http://ftp.jqgfzy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dpu.shanyushiyangkeji.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hgx.yj20258.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://oaj.9152youxi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hfm.bjfxy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nyp.cheryme.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yke.shangyingyoupin.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pgb.cqqwz.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dli.yvedp.cn

[D26] 数组转字符串
来源：http://wam.pengpengdd.cyou

Py:   ", ".join(map(str, arr))
来源：http://ocd.hnxiangtu.top

PHP:  implode(", ", $arr);
来源：http://eqa.shzxlz.cn

JS:   arr.join(", ")
来源：http://tbo.havefunace.top

TS:   arr.join(", ")
来源：http://wao.zhoulong.xyz

Java: String.join(", ", list)
来源：http://psc.hcnkem.com

Go:   strings.Join(strs, ", ")
来源：http://syr.aizwys.cn

Ruby: arr.join(", ")
来源：http://lwn.tarul.cn

C#:   string.Join(", ", list)
来源：http://fhy.c1oappe.top

================================================================================
来源：http://yfd.xingfuxueyuan.xyz

E. 字符串处理
来源：http://dal.jyoumei.cn

================================================================================
来源：http://whk.cucudq.cn

[E01] 拼接字符串
来源：http://hqg.yuanzhike.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://iox.quarkkingdee.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wuc.hammf.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fnv.ybcxt.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://atv.guowangkeji.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rqe.dianchejie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hiu.xuanzx.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sfh.xingfuxueyuan.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rwc.zhongyouzk.top

[E02] 重复字符串
来源：http://xhh.nanxuanxn.top

Py:   "ab" * 3
来源：http://gaj.yueranfly.top

PHP:  str_repeat("ab", 3);
来源：http://jxg.shanyushiyangkeji.top

JS:   "ab".repeat(3)
来源：http://wjb.cucudq.cn

TS:   "ab".repeat(3)
来源：http://lmd.sysykeji.top

Java: "ab".repeat(3)
来源：http://nxu.pengpengdd.cyou

Go:   strings.Repeat("ab", 3)
来源：http://bob.c1oappe.top

Ruby: "ab" * 3
来源：http://sgh.nanxuanxn.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qsa.dashuyun.cn

[E03] 截取子串
来源：http://jvi.fengsongda.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zpl.ctjpmb.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xtf.jyoumei.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lgl.yanxiufei.cn

TS:   s.slice(1, 4)
来源：http://cij.redwolf501.top

Java: s.substring(1, 4)
来源：http://dli.fanxiaobao.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://azl.shuidangran.top

Ruby: s[1, 3];  s[1..3]
来源：http://rfd.vehdjk.com

C#:   s.Substring(1, 3)
来源：http://pyl.yongpay.top

[E04] 查找子串位置
来源：http://swi.yfazqb.com

Py:   s.find("x");  s.index("x")
来源：http://ooz.vehdjk.com

PHP:  strpos($s, "x");
来源：http://thz.hnqzz.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fby.yfazqb.com

TS:   s.indexOf("x")
来源：http://cez.zhaomingkeji.xyz

Java: s.indexOf("x")
来源：http://mhg.shanyushiyangtech.top

Go:   strings.Index(s, "x")
来源：http://mjc.zycfv.cn

Ruby: s.index("x")
来源：http://ipn.xuanzx.com

C#:   s.IndexOf("x")
来源：http://bir.tianlin.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://sbj.zhengqikj.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qxm.316326.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hzn.ydjk.org.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dqd.shzxlz.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kpv.ivvv.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aem.chenlongwang.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jme.redwolf501.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wgy.zdqjudy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bqf.hcnkem.com

[E06] 替换子串
来源：http://hly.hnxiangtu.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ylb.zhaomingkeji.xyz

PHP:  str_replace("a", "b", $s);
来源：http://xsa.jinghuilouyu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zag.tarul.cn

TS:   s.replaceAll("a", "b")
来源：http://iug.redwolf501.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yos.cqqwz.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gnp.tian-w.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cot.yj20258888.top

C#:   s.Replace("a", "b")
来源：http://dah.shanyushiyangkeji.top

[E07] 按分隔符拆分
来源：http://thh.bbcook.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hrh.nanxuanxn.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bxx.fehbvm.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://djd.yueranfly.top

TS:   s.split(",")
来源：http://jtd.dashuyun.cn

Java: s.split(",");  s.split("\\s+")
来源：http://uml.iojbl.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mph.mhx1999.top

Ruby: s.split(",");  s.split
来源：http://xnj.kuanghao11.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://chc.meibo888.top

[E08] 数组按分隔符合并
来源：http://nnx.jinqigufen.top

Py:   ",".join(items)
来源：http://izs.shuidangran.top

PHP:  implode(",", $items);
来源：http://pne.jqgfzy.top

JS:   items.join(",")
来源：http://cdd.jqgufenzy.top

TS:   items.join(",")
来源：http://rhn.9152youxi.cn

Java: String.join(",", items)
来源：http://dyu.daria6918.cn

Go:   strings.Join(items, ",")
来源：http://uzf.guowangkeji.top

Ruby: items.join(",")
来源：http://aey.0kj1m.cn

C#:   string.Join(",", items)
来源：http://vez.zhoulong.xyz

[E09] 去除所有空白字符
来源：http://pwz.yj20258.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gxg.tarul.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qxv.pengpengdd.cyou

JS:   s.replace(/\s+/g, "")
来源：http://hse.shangyingyoupin.top

TS:   s.replace(/\s+/g, "")
来源：http://npb.tanke756.top

Java: s.replaceAll("\\s+", "")
来源：http://bob.zhoulong.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://yav.ydjk.org.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zrv.gaohongyu789.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rhz.jinyuanbaomall.cn

[E10] 左侧补零 / 定长填充
来源：http://lxy.jyoumei.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tvj.jiagoushi.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://crz.quarkkingdee.top

JS:   "7".padStart(3, "0")
来源：http://bws.yj202588.top

TS:   "7".padStart(3, "0")
来源：http://oml.ctjpmb.com

Java: String.format("%03d", 7)
来源：http://jgf.zycfv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mfz.yj20258.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bnw.jiagoushi.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dgm.chenjidiqi.icu

[E11] 反转字符串
来源：http://hzw.yonumen.top

Py:   s[::-1]
来源：http://pnt.hnxiangtu.top

PHP:  strrev($s);
来源：http://yfh.sjlbkw.cn

JS:   [...s].reverse().join("")
来源：http://qqy.jqgfzy.top

TS:   [...s].reverse().join("")
来源：http://hqo.sxryk.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vqs.yangfankeji.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://prp.chenlongwang.top


<!-- 参考信息 -->