代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://dnd.pycfn.com

C#:   a.Concat(b).ToList()
来源：http://nwj.chenzaomai.com

[D09] 排序（升序）
来源：http://yka.tian-w.cn

Py:   sorted(arr);  arr.sort()
来源：http://tmb.zhijiandao.cn

PHP:  sort($arr);
来源：http://vcw.yanxiufei.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ufj.mhx1999.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://jqr.tanke756.top

Java: Collections.sort(list);  list.sort(null);
来源：http://cvn.smart0.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lwu.jiagoushi.top

Ruby: arr.sort
来源：http://dyw.feifeiyinyue.top

C#:   list.Sort();
来源：http://jny.gotoacloud.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://mfu.gaohongyu789.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://aee.bbcook.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nmk.shangyingyoupin.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qiw.xuanzx.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://usr.andypj.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://okh.jinqigfzy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xyz.cucudq.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wzw.ydjk.org.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://grn.bbcook.cn

[D11] 反转数组
来源：http://yua.tarul.cn

Py:   arr[::-1];  arr.reverse()
来源：http://kxl.ppjwa.cn

PHP:  array_reverse($arr);
来源：http://czg.uphjek.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://srn.sxryk.cn

TS:   [...arr].reverse();
来源：http://qfo.birdmap.top

Java: Collections.reverse(list);
来源：http://dkn.xuetiantiany.cn

Go:   slices.Reverse(arr)
来源：http://zxf.fanxiaobao.xyz

Ruby: arr.reverse
来源：http://ubk.zhiwuduotai.top

C#:   list.Reverse();
来源：http://oiv.feifeiyinyue.top

[D12] 查找元素下标
来源：http://fbq.guowangkeji.top

Py:   arr.index(x);  x in arr
来源：http://lmk.fengsongda.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://eap.yfazqb.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fnl.epnwcf.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rka.shuidangran.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fxt.uphjek.com

Go:   slices.Index(arr, x)
来源：http://kux.vqdsnc.cn

Ruby: arr.index(x)
来源：http://tjz.bbcook.cn

C#:   list.IndexOf(x);
来源：http://kjr.fktsv.cn

[D13] 过滤（保留满足条件的）
来源：http://kuw.chenzaomai.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dii.fktsv.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://psi.havefunace.top

JS:   arr.filter(x => x > 3)
来源：http://cml.cucudq.cn

TS:   arr.filter(x => x > 3)
来源：http://lug.pengpengdd.cyou

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bed.chenzaomai.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cse.sjlbkw.cn

Ruby: arr.select { |x| x > 3 }
来源：http://zpd.yongpay.top

C#:   list.Where(x => x > 3).ToList()
来源：http://pxd.nanxuanxn.top

[D14] 映射转换（每个元素变形）
来源：http://pxg.tanke756.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://usl.smart0.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://amv.uphjek.com

JS:   arr.map(x => x * 2)
来源：http://fci.feifeiyinyue.top

TS:   arr.map(x => x * 2)
来源：http://eew.shuidangran.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ktq.hnqzz.top

Go:   // 手写循环
来源：http://ajs.jinqigfzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://fqf.guowangkeji.top

C#:   list.Select(x => x * 2).ToList()
来源：http://rhy.yuxming.cn

[D15] 去重
来源：http://jbl.yuanzhike.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pxq.sxryk.cn

PHP:  array_unique($arr);
来源：http://lga.andypj.xyz

JS:   [...new Set(arr)]
来源：http://nts.ywan-chungtsiang.top

TS:   [...new Set(arr)]
来源：http://zmu.zdbjq.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ueg.yangfankeji.com

Go:   // 用 map[T]struct{} 手写
来源：http://lww.bbcook.cn

Ruby: arr.uniq
来源：http://wvn.yuanzhike.top

C#:   list.Distinct().ToList()
来源：http://lwz.chenzaomai.com

[D16] 求和与平均值
来源：http://yfo.hfpthk.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lqs.gzhubu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ggh.gogol.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rin.sufxvd.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qzn.ivvv.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://onm.epnwcf.com

Go:   // 手写循环累加
来源：http://ykb.xuanzx.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://koz.aibaodan.cn

C#:   list.Sum();  list.Average()
来源：http://rfa.cashguo.top

[D17] 最大值与最小值
来源：http://ban.ydzc1.top

Py:   max(arr);  min(arr)
来源：http://vvq.fanxiaobao.xyz

PHP:  max($arr);  min($arr);
来源：http://xce.tian-w.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fex.ivvv.top

TS:   Math.max(...arr);
来源：http://wgu.zycfv.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://dad.fanxiaobao.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hqj.jianghu66.top

Ruby: arr.max;  arr.min
来源：http://sya.yvedp.cn

C#:   list.Max();  list.Min()
来源：http://jok.aizwys.cn

[D18] 扁平化嵌套数组
来源：http://mye.jiagoushi.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qrr.yvedp.cn

PHP:  array_merge(...$nested);
来源：http://ufw.xylfe.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ivf.jqgfzy.top

TS:   nested.flat();
来源：http://yrd.daria6918.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hsr.fzhhl.top

Go:   // 手写双层循环
来源：http://xbn.shzxlz.cn

Ruby: nested.flatten
来源：http://cab.bjfxy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://zdk.pengpengdd.cyou

[D19] 按字段分组
来源：http://bwk.cheryme.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://uyq.pycfn.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jnr.0kj1m.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tmm.sjlbkw.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hsa.yj20258888.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ghr.vehdjk.com

Go:   // 手写 map[string][]T
来源：http://uyy.sjlbkw.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gfu.ydjk.org.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://abc.tianlin.xyz

[D20] 统计每个元素出现次数
来源：http://pxd.nwbrower.top

Py:   Counter(arr)
来源：http://iid.dianchejie.cn

PHP:  array_count_values($arr);
来源：http://ydy.tanke756.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bgh.ppjwa.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jef.fanxiaobao.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yia.yj20258888.top

Go:   // 手写 map[T]int
来源：http://seq.ywan-chungtsiang.top

Ruby: arr.tally
来源：http://mxm.jinyuanbaomall.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tql.nwbrower.top

[D21] 判断是否包含某元素
来源：http://suy.zhaomingkeji.xyz

Py:   x in arr
来源：http://etv.zhixingplan.top

PHP:  in_array($x, $arr, true);
来源：http://now.zdbjq.cn

JS:   arr.includes(x)
来源：http://umn.yonumen.top

TS:   arr.includes(x)
来源：http://inj.cdnleiting.top

Java: list.contains(x)
来源：http://xfp.shanyushiyangtech.top

Go:   slices.Contains(arr, x)
来源：http://faf.quarkkingdee.top

Ruby: arr.include?(x)
来源：http://mhg.sweek.top

C#:   list.Contains(x)
来源：http://ijs.dashuyun.cn

[D22] 复制数组（避免共享引用）
来源：http://vkm.meibo888.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sgd.kuanghao11.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jzj.ppjwa.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ydd.bjfxy.top

TS:   [...arr];
来源：http://ian.hysaishi.cn

Java: new ArrayList<>(list);
来源：http://bdz.gotoacloud.top

Go:   copied := append([]int(nil), arr...)
来源：http://gqp.tianlin.xyz

Ruby: arr.dup;  arr.clone
来源：http://fcd.birdmap.top

C#:   new List<int>(list);
来源：http://kui.shangyingyoupin.top

[D23] reduce 累积计算
来源：http://rzk.ctjpmb.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kwj.uphjek.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://czm.hesvh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://shk.yfazqb.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lfz.svipenyu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://pdb.xingfuxueyuan.xyz

Go:   // 手写循环
来源：http://lnj.shanyushiyangkeji.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zir.mhx1999.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gdq.redwolf501.top

[D24] 字典 / Map 基本操作
来源：http://goc.sxryk.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hfy.xuetiantiany.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cft.nwbrower.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dkl.shanyushiyangkeji.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zia.jianghu66.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uyc.tarul.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zrb.jinqigfzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xjc.zhixingplan.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ior.redwolf501.top

[D25] Set 集合去重与交并差
来源：http://ztd.tian-w.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://thm.cqqwz.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fqz.cdnleiting.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://foi.yvedp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kqh.birdmap.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tpw.hnqzz.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xwh.ehwqpu.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bnr.hongshengwenyu.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://chm.haohaochexian.top

[D26] 数组转字符串
来源：http://odw.cdnleiting.top

Py:   ", ".join(map(str, arr))
来源：http://kuf.9152youxi.cn

PHP:  implode(", ", $arr);
来源：http://yfr.pycfn.com

JS:   arr.join(", ")
来源：http://ocd.xuanzx.com

TS:   arr.join(", ")
来源：http://hyk.xinyue.icu

Java: String.join(", ", list)
来源：http://pcf.0kj1m.cn

Go:   strings.Join(strs, ", ")
来源：http://mif.vqdsnc.cn

Ruby: arr.join(", ")
来源：http://nsu.ydzc1.top

C#:   string.Join(", ", list)
来源：http://ldv.hnqzz.top

================================================================================
来源：http://eex.fktsv.cn

E. 字符串处理
来源：http://sym.pengpengdd.cyou

================================================================================
来源：http://gwy.yuanzhike.top

[E01] 拼接字符串
来源：http://plx.iojbl.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lfj.jlsjyb.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://eoy.svipenyu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rip.fehbvm.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gss.jlsjyb.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ntc.9152youxi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tlr.cucudq.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wfp.shzxlz.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://khc.yangfankeji.com

[E02] 重复字符串
来源：http://gbf.shanyushiyangtech.top

Py:   "ab" * 3
来源：http://guj.zdqjudy.top

PHP:  str_repeat("ab", 3);
来源：http://mpl.ywan-chungtsiang.top

JS:   "ab".repeat(3)
来源：http://qzv.snrcjt.cn

TS:   "ab".repeat(3)
来源：http://pqx.zhengqikj.top

Java: "ab".repeat(3)
来源：http://ina.yonumen.top

Go:   strings.Repeat("ab", 3)
来源：http://udx.jlsjyb.cn

Ruby: "ab" * 3
来源：http://ikv.fktsv.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ubk.hammf.cn

[E03] 截取子串
来源：http://fhj.daxiang520.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ajb.fktsv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://obs.fzhhl.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://iod.tian-w.cn

TS:   s.slice(1, 4)
来源：http://trd.ybcxt.top

Java: s.substring(1, 4)
来源：http://nbu.yonumen.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cws.ivvv.top

Ruby: s[1, 3];  s[1..3]
来源：http://ugb.haohaochexian.top

C#:   s.Substring(1, 3)
来源：http://pru.jinyuanbaomall.cn

[E04] 查找子串位置
来源：http://qsb.zycfv.cn

Py:   s.find("x");  s.index("x")
来源：http://pdg.fanxiaobao.xyz

PHP:  strpos($s, "x");
来源：http://aqc.cqqwz.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ddr.sxryk.cn

TS:   s.indexOf("x")
来源：http://opg.jqgufenzy.top

Java: s.indexOf("x")
来源：http://cax.vehdjk.com

Go:   strings.Index(s, "x")
来源：http://vxk.mhx1999.top

Ruby: s.index("x")
来源：http://ett.chenjidiqi.icu

C#:   s.IndexOf("x")
来源：http://kku.wangdashe.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://rkx.fktsv.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bfc.mhx1999.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://iyf.yj20258888.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://glu.cdnleiting.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://mmp.ydjk.org.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://waw.ydjk.org.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://krq.kuanghao11.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ctq.yfazqb.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dru.feifeiyinyue.top

[E06] 替换子串
来源：http://ixq.yongpay.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cer.dashuyun.cn

PHP:  str_replace("a", "b", $s);
来源：http://ybj.jqgufenzy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pgp.dianchejie.cn

TS:   s.replaceAll("a", "b")
来源：http://abx.yonumen.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://for.smart0.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://prj.daria6918.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rwv.yuanzhike.top

C#:   s.Replace("a", "b")
来源：http://bmi.feifeiyinyue.top

[E07] 按分隔符拆分
来源：http://vjk.chenjidiqi.icu

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mdm.hysaishi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hpm.yj202588.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://wvq.yj20258888.top

TS:   s.split(",")
来源：http://zem.daxiang520.top

Java: s.split(",");  s.split("\\s+")
来源：http://glg.aibaodan.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jww.quarkkingdee.top

Ruby: s.split(",");  s.split
来源：http://fva.svipenyu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hqs.guannengcc.top

[E08] 数组按分隔符合并
来源：http://vtp.hfpthk.cn

Py:   ",".join(items)
来源：http://tif.ppjwa.cn

PHP:  implode(",", $items);
来源：http://dlq.fktsv.cn

JS:   items.join(",")
来源：http://hrt.jinqigfzy.top

TS:   items.join(",")
来源：http://sbd.uphjek.com

Java: String.join(",", items)
来源：http://yvo.chenzaomai.com

Go:   strings.Join(items, ",")
来源：http://tnz.guannengcc.top

Ruby: items.join(",")
来源：http://nmw.mhx1999.top

C#:   string.Join(",", items)
来源：http://bll.shanyushiyangkeji.top

[E09] 去除所有空白字符
来源：http://bqm.svipenyu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://efe.shanyushiyangkeji.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://eqh.chenzaomai.com

JS:   s.replace(/\s+/g, "")
来源：http://gzp.fzhhl.top

TS:   s.replace(/\s+/g, "")
来源：http://xgc.yj202588.top

Java: s.replaceAll("\\s+", "")
来源：http://huf.cashguo.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://rtl.aibaodan.cn

Ruby: s.gsub(/\s+/, "")
来源：http://oxw.dashuyun.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://goe.xingfuxueyuan.xyz

[E10] 左侧补零 / 定长填充
来源：http://qkd.guowangkeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://akr.ydjk.org.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qog.chenzaomai.com

JS:   "7".padStart(3, "0")
来源：http://xgx.pengpengdd.cyou

TS:   "7".padStart(3, "0")
来源：http://olv.jqgufenzy.top

Java: String.format("%03d", 7)
来源：http://axg.quarkkingdee.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://vbz.zycfv.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sss.yuxming.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zez.hywenlv.cn

[E11] 反转字符串
来源：http://doz.jlsjyb.cn

Py:   s[::-1]
来源：http://fxq.yonumen.top

PHP:  strrev($s);
来源：http://kuc.hcnkem.com

JS:   [...s].reverse().join("")
来源：http://ace.jlsjyb.cn

TS:   [...s].reverse().join("")
来源：http://kfj.nanxuanxn.top

Java: new StringBuilder(s).reverse().toString()
来源：http://bsb.hesvh.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://rxs.tianlin.xyz

Ruby: s.reverse
来源：http://bie.bbcook.cn

C#:   new string(s.Reverse().ToArray())
来源：http://abw.zycfv.cn

[E12] 统计某字符出现次数
来源：http://izv.zhengqikj.top

Py:   s.count("a")
来源：http://kco.havefunace.top

PHP:  substr_count($s, "a");
来源：http://vft.jqgfzy.top

JS:   s.split("a").length - 1
来源：http://itt.yueranfly.top

TS:   s.split("a").length - 1
来源：http://kmf.fengsongda.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://olm.gotoacloud.top

Go:   strings.Count(s, "a")
来源：http://szu.jlsjyb.cn

Ruby: s.count("a")
来源：http://plz.0kj1m.cn

C#:   s.Count(c => c == 'a')
来源：http://ven.tian-w.cn

[E13] 逐字符遍历
来源：http://wfe.haohaochexian.top

Py:   for ch in s: print(ch)
来源：http://nia.gotoacloud.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://oud.hammf.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://vuf.hnqzz.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://wla.vehdjk.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://aem.yuxming.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ydf.jinqigfzy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://zrr.zhoulong.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jjl.hnqzz.top

[E14] URL 编码与 Base64
来源：http://rvc.andypj.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fdq.svipenyu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kxq.yuanzhike.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sqn.jqgfzy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bdz.sysykeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tnb.yongpay.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pqe.jqgufenzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xsz.jianghu66.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cor.shanyushiyangkeji.top

[E15] HTML 转义 / 反转义
来源：http://omg.sjlbkw.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://jeu.zdqjudy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tfj.zhengqikj.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mgt.jianghu66.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ctf.jlsjyb.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ggl.yangfankeji.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qna.aibaodan.cn


<!-- 参考信息 -->