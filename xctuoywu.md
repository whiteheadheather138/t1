代发 wailian999

PHP:  sort($arr);
来源：http://qle.fktsv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hkz.jqgfzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://owj.hammf.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://clh.hfpthk.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gey.wangdashe.top

Ruby: arr.sort
来源：http://mhq.havefunace.top

C#:   list.Sort();
来源：http://owu.hywenlv.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://nuo.0kj1m.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bov.bjfxy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hkg.gzhubu.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xau.sufxvd.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ify.yfazqb.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rpj.yj202588.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://otq.meibo888.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tdi.wangdashe.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://eyk.zhengqikj.top

[D11] 反转数组
来源：http://ipj.gogol.net.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qhi.wangshuangyany.cn

PHP:  array_reverse($arr);
来源：http://khh.redwolf501.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pkg.vqdsnc.cn

TS:   [...arr].reverse();
来源：http://ozx.dashuyun.cn

Java: Collections.reverse(list);
来源：http://mgz.chenjidiqi.icu

Go:   slices.Reverse(arr)
来源：http://otu.yongpay.top

Ruby: arr.reverse
来源：http://kdg.ydjk.org.cn

C#:   list.Reverse();
来源：http://pdo.gogol.net.cn

[D12] 查找元素下标
来源：http://sly.fengsongda.top

Py:   arr.index(x);  x in arr
来源：http://tkx.tarul.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qdn.hongshengwenyu.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bmp.zhaomingkeji.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oiz.pycfn.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rci.shzxlz.cn

Go:   slices.Index(arr, x)
来源：http://jee.yuxming.cn

Ruby: arr.index(x)
来源：http://gfm.yfazqb.com

C#:   list.IndexOf(x);
来源：http://tvz.epnwcf.com

[D13] 过滤（保留满足条件的）
来源：http://sva.shzxlz.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://grs.fktsv.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nak.hysaishi.cn

JS:   arr.filter(x => x > 3)
来源：http://ety.zycfv.cn

TS:   arr.filter(x => x > 3)
来源：http://ige.gotoacloud.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://igo.zhiwuduotai.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yuh.quarkkingdee.top

Ruby: arr.select { |x| x > 3 }
来源：http://txy.zdbjq.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://kvu.ydjk.org.cn

[D14] 映射转换（每个元素变形）
来源：http://aky.xuetiantiany.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mfj.yangfankeji.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bex.tian-w.cn

JS:   arr.map(x => x * 2)
来源：http://ecl.hfpthk.cn

TS:   arr.map(x => x * 2)
来源：http://ihv.zdbjq.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://why.redwolf501.top

Go:   // 手写循环
来源：http://cnd.kuanghao11.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ote.jyoumei.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://moy.guannengcc.top

[D15] 去重
来源：http://kby.smart0.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xje.cdnleiting.top

PHP:  array_unique($arr);
来源：http://ahv.havefunace.top

JS:   [...new Set(arr)]
来源：http://wxj.sjlbkw.cn

TS:   [...new Set(arr)]
来源：http://sge.yj202588.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xtd.fengsongda.top

Go:   // 用 map[T]struct{} 手写
来源：http://xvz.tanke756.top

Ruby: arr.uniq
来源：http://zkn.0kj1m.cn

C#:   list.Distinct().ToList()
来源：http://npi.fehbvm.com

[D16] 求和与平均值
来源：http://ebr.ehwqpu.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pig.cucudq.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cng.xingfuxueyuan.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://khk.xingfuxueyuan.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bbh.shanyushiyangkeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vrd.haohaochexian.top

Go:   // 手写循环累加
来源：http://rwc.zdbjq.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://eto.nanxuanxn.top

C#:   list.Sum();  list.Average()
来源：http://iwx.jqgfzy.top

[D17] 最大值与最小值
来源：http://avi.shangyingyoupin.top

Py:   max(arr);  min(arr)
来源：http://aai.zhaomingkeji.xyz

PHP:  max($arr);  min($arr);
来源：http://afz.tianlin.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ceq.chenlongwang.top

TS:   Math.max(...arr);
来源：http://vua.dianchejie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://kpz.zhoulong.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://onm.aibaodan.cn

Ruby: arr.max;  arr.min
来源：http://xlm.bjfxy.top

C#:   list.Max();  list.Min()
来源：http://jwr.jlsjyb.cn

[D18] 扁平化嵌套数组
来源：http://eeh.gotoacloud.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wkv.hywenlv.cn

PHP:  array_merge(...$nested);
来源：http://yep.zhixingplan.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cuy.aibaodan.cn

TS:   nested.flat();
来源：http://atq.meibo888.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://apj.kuanghao11.cn

Go:   // 手写双层循环
来源：http://zvw.meibo888.top

Ruby: nested.flatten
来源：http://xyi.ybcxt.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://smf.dianchejie.cn

[D19] 按字段分组
来源：http://wpp.dashuyun.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jcj.zhijiandao.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://apw.epnwcf.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://unu.fanxiaobao.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://zik.hongshengwenyu.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://roj.pengpengdd.cyou

Go:   // 手写 map[string][]T
来源：http://usa.ydjk.org.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://kke.jqgfzy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://otq.quarkkingdee.top

[D20] 统计每个元素出现次数
来源：http://kdn.pycfn.com

Py:   Counter(arr)
来源：http://ikf.yfazqb.com

PHP:  array_count_values($arr);
来源：http://bqb.chenjidiqi.icu

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iht.wangdashe.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aqy.redwolf501.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yep.tanke756.top

Go:   // 手写 map[T]int
来源：http://zch.yuxming.cn

Ruby: arr.tally
来源：http://dhq.uphjek.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qqu.quarkkingdee.top

[D21] 判断是否包含某元素
来源：http://der.uphjek.com

Py:   x in arr
来源：http://wzn.yj20258.top

PHP:  in_array($x, $arr, true);
来源：http://dwh.sysykeji.top

JS:   arr.includes(x)
来源：http://ebz.xuetiantiany.cn

TS:   arr.includes(x)
来源：http://zes.vehdjk.com

Java: list.contains(x)
来源：http://qkw.pengpengdd.cyou

Go:   slices.Contains(arr, x)
来源：http://kwd.yvedp.cn

Ruby: arr.include?(x)
来源：http://xtw.yuanzhike.top

C#:   list.Contains(x)
来源：http://ewx.shangyingyoupin.top

[D22] 复制数组（避免共享引用）
来源：http://bef.vqdsnc.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sgr.pengpengdd.cyou

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rgc.9152youxi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mpc.hcnkem.com

TS:   [...arr];
来源：http://wxc.ehwqpu.com

Java: new ArrayList<>(list);
来源：http://ptw.fehbvm.com

Go:   copied := append([]int(nil), arr...)
来源：http://tqg.redwolf501.top

Ruby: arr.dup;  arr.clone
来源：http://fnt.uphjek.com

C#:   new List<int>(list);
来源：http://kym.gotoacloud.top

[D23] reduce 累积计算
来源：http://xvl.meibo888.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zhc.sxryk.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ins.zhaomingkeji.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jcs.shuidangran.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://igy.zdqjudy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://lja.smart0.xyz

Go:   // 手写循环
来源：http://org.chenlongwang.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kbs.zhaomingkeji.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lsa.fzhhl.top

[D24] 字典 / Map 基本操作
来源：http://aga.aibaodan.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wxl.cdnleiting.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wib.yonumen.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kft.shuidangran.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jcy.jinyuanbaomall.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gxz.c1oappe.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mlf.daria6918.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://knw.vqdsnc.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gim.meibo888.top

[D25] Set 集合去重与交并差
来源：http://tas.cdnleiting.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rre.tianlin.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://udd.sufxvd.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xol.sysykeji.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ksc.daxiang520.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://btt.sjlbkw.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fne.vqdsnc.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bdk.bjfxy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rds.ydjk.org.cn

[D26] 数组转字符串
来源：http://xdh.fktsv.cn

Py:   ", ".join(map(str, arr))
来源：http://hfm.quarkkingdee.top

PHP:  implode(", ", $arr);
来源：http://nkg.gogol.net.cn

JS:   arr.join(", ")
来源：http://wdj.hammf.cn

TS:   arr.join(", ")
来源：http://mrt.meibo888.top

Java: String.join(", ", list)
来源：http://mvj.yueranfly.top

Go:   strings.Join(strs, ", ")
来源：http://emo.zhixingplan.top

Ruby: arr.join(", ")
来源：http://uvw.zhixingplan.top

C#:   string.Join(", ", list)
来源：http://xld.cucudq.cn

================================================================================
来源：http://axz.jinqigufen.top

E. 字符串处理
来源：http://qon.hcnkem.com

================================================================================
来源：http://qdz.zhengqikj.top

[E01] 拼接字符串
来源：http://grf.jqgufenzy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://iju.shangyingyoupin.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cdj.cdnleiting.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qpl.cheryme.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://scp.nanxinkj.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cai.ydzc1.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://iaq.jinyuanbaomall.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tyx.zhongyouzk.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tra.ybcxt.top

[E02] 重复字符串
来源：http://fqi.zhijiandao.cn

Py:   "ab" * 3
来源：http://aqa.yuanzhike.top

PHP:  str_repeat("ab", 3);
来源：http://zuj.tianlin.xyz

JS:   "ab".repeat(3)
来源：http://pwj.yongpay.top

TS:   "ab".repeat(3)
来源：http://xcz.yj202588.top

Java: "ab".repeat(3)
来源：http://bgf.daxiang520.top

Go:   strings.Repeat("ab", 3)
来源：http://qob.redwolf501.top

Ruby: "ab" * 3
来源：http://shf.tanke756.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hzm.hfpthk.cn

[E03] 截取子串
来源：http://qrp.jqgfzy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vee.jinqigufen.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://teb.xinyue.icu

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://iqb.hnxiangtu.top

TS:   s.slice(1, 4)
来源：http://hhr.zhoulong.xyz

Java: s.substring(1, 4)
来源：http://ncr.hnqzz.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mid.hnqzz.top

Ruby: s[1, 3];  s[1..3]
来源：http://rex.fengsongda.top

C#:   s.Substring(1, 3)
来源：http://yae.jinqigfzy.top

[E04] 查找子串位置
来源：http://klc.xuanzx.com

Py:   s.find("x");  s.index("x")
来源：http://cxu.yanxiufei.cn

PHP:  strpos($s, "x");
来源：http://prl.iojbl.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qkt.jinqigufen.top

TS:   s.indexOf("x")
来源：http://gox.sxryk.cn

Java: s.indexOf("x")
来源：http://wcd.jinyuanbaomall.cn

Go:   strings.Index(s, "x")
来源：http://ndw.redwolf501.top

Ruby: s.index("x")
来源：http://hly.daria6918.cn

C#:   s.IndexOf("x")
来源：http://sru.meibo888.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://yht.jqgfzy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hiw.cqqwz.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://evb.ydjk.org.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ryd.ehwqpu.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://taz.zdqjudy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bft.cucudq.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kju.cashguo.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://app.iojbl.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ime.sufxvd.cn

[E06] 替换子串
来源：http://dzk.jiagoushi.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://deu.wangdashe.top

PHP:  str_replace("a", "b", $s);
来源：http://wvb.hnqzz.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pec.jqgfzy.top

TS:   s.replaceAll("a", "b")
来源：http://cgg.vqdsnc.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uhs.zhixingplan.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://stu.fehbvm.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zus.hongshengwenyu.top

C#:   s.Replace("a", "b")
来源：http://xhl.cqqwz.cn

[E07] 按分隔符拆分
来源：http://vip.zhengqikj.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tbn.jlsjyb.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://buy.guowangkeji.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://mop.yfazqb.com

TS:   s.split(",")
来源：http://uux.daria6918.cn

Java: s.split(",");  s.split("\\s+")
来源：http://alp.cucudq.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://isv.hesvh.cn

Ruby: s.split(",");  s.split
来源：http://fah.zdbjq.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lxp.sweek.top

[E08] 数组按分隔符合并
来源：http://aln.shzxlz.cn

Py:   ",".join(items)
来源：http://kpm.yj20258888.top

PHP:  implode(",", $items);
来源：http://wcm.jinqigufen.top

JS:   items.join(",")
来源：http://rvh.ehwqpu.com

TS:   items.join(",")
来源：http://rmb.kuanghao11.cn

Java: String.join(",", items)
来源：http://wzn.xylfe.cn

Go:   strings.Join(items, ",")
来源：http://oux.zdqjudy.top

Ruby: items.join(",")
来源：http://plb.jianghu66.top

C#:   string.Join(",", items)
来源：http://dwj.sjlbkw.cn

[E09] 去除所有空白字符
来源：http://edh.andypj.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dgk.gogol.net.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://doi.yj20258.top

JS:   s.replace(/\s+/g, "")
来源：http://hsa.shanyushiyangkeji.top

TS:   s.replace(/\s+/g, "")
来源：http://bsn.bbcook.cn

Java: s.replaceAll("\\s+", "")
来源：http://fym.yangfankeji.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://hua.wangdashe.top

Ruby: s.gsub(/\s+/, "")
来源：http://zvg.zhijiandao.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://agp.jiagoushi.top

[E10] 左侧补零 / 定长填充
来源：http://krl.yj202588.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zpj.zhoulong.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dgq.shuidangran.top

JS:   "7".padStart(3, "0")
来源：http://sqs.bbcook.cn

TS:   "7".padStart(3, "0")
来源：http://kqo.feifeiyinyue.top

Java: String.format("%03d", 7)
来源：http://usc.pycfn.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://zbb.hammf.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rpa.jianghu66.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jtb.cdnleiting.top

[E11] 反转字符串
来源：http://rrk.haohaochexian.top

Py:   s[::-1]
来源：http://koh.xylfe.cn

PHP:  strrev($s);
来源：http://acb.yuanzhike.top

JS:   [...s].reverse().join("")
来源：http://exf.yuanzhike.top

TS:   [...s].reverse().join("")
来源：http://jmy.zhixingplan.top

Java: new StringBuilder(s).reverse().toString()
来源：http://sfa.dashuyun.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://grc.kuanghao11.cn

Ruby: s.reverse
来源：http://lhj.pengpengdd.cyou

C#:   new string(s.Reverse().ToArray())
来源：http://mhs.yangfankeji.com

[E12] 统计某字符出现次数
来源：http://ops.316326.xyz

Py:   s.count("a")
来源：http://jwv.epnwcf.com

PHP:  substr_count($s, "a");
来源：http://zju.yongpay.top

JS:   s.split("a").length - 1
来源：http://twt.jlsjyb.cn

TS:   s.split("a").length - 1
来源：http://orv.zhoulong.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kal.daxiang520.top

Go:   strings.Count(s, "a")
来源：http://odu.hysaishi.cn

Ruby: s.count("a")
来源：http://msc.hcnkem.com

C#:   s.Count(c => c == 'a')
来源：http://crd.shanyushiyangtech.top

[E13] 逐字符遍历
来源：http://fsx.hysaishi.cn

Py:   for ch in s: print(ch)
来源：http://bvl.sjlbkw.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://aut.ppjwa.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://vjm.zdqjudy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ppj.gogol.net.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bwj.shzxlz.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ysv.tianlin.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://whj.wangdashe.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://omb.svipenyu.cn

[E14] URL 编码与 Base64
来源：http://bht.ppjwa.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ikz.jinghuilouyu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ddi.pengpengdd.cyou

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cle.nwbrower.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ace.ywan-chungtsiang.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wwf.zhixingplan.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://eda.daxiang520.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wjt.zdbjq.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hfl.gzhubu.top

[E15] HTML 转义 / 反转义
来源：http://sqg.tanke756.top

Py:   html.escape(s);  html.unescape(s)
来源：http://rgm.jinyuanbaomall.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sry.hcnkem.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://khj.zhixingplan.top

TS:   // 同上，务必做 XSS 过滤
来源：http://kkl.gzhubu.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zuf.jqgfzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://daq.jiagoushi.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fmk.xuanzx.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zsp.cucudq.cn

[E16] 数字千分位
来源：http://qod.jinyuanbaomall.cn

Py:   f"{1234567:,}"
来源：http://src.yuanzhike.top


<!-- 参考信息 -->