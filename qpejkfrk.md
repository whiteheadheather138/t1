代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hue.sjlbkw.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xae.vehdjk.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://clk.yj20258888.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wus.jianghu66.top

[D11] 反转数组
来源：http://xqx.jinyuanbaomall.cn

Py:   arr[::-1];  arr.reverse()
来源：http://spc.vqdsnc.cn

PHP:  array_reverse($arr);
来源：http://plo.yj20258888.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fvs.gaohongyu789.top

TS:   [...arr].reverse();
来源：http://ukj.52xcode.cn

Java: Collections.reverse(list);
来源：http://yvk.bbcook.cn

Go:   slices.Reverse(arr)
来源：http://fvy.jiagoushi.top

Ruby: arr.reverse
来源：http://iup.havefunace.top

C#:   list.Reverse();
来源：http://svx.aizwys.cn

[D12] 查找元素下标
来源：http://ixs.yongpay.top

Py:   arr.index(x);  x in arr
来源：http://lvb.fanxiaobao.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jay.hnqzz.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aje.zhixingplan.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aje.sufxvd.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wab.jinghuilouyu.cn

Go:   slices.Index(arr, x)
来源：http://svd.vqdsnc.cn

Ruby: arr.index(x)
来源：http://krb.ydzc1.top

C#:   list.IndexOf(x);
来源：http://bsg.redwolf501.top

[D13] 过滤（保留满足条件的）
来源：http://jha.fehbvm.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://iyb.yuxming.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jtf.yongpay.top

JS:   arr.filter(x => x > 3)
来源：http://vbp.hammf.cn

TS:   arr.filter(x => x > 3)
来源：http://ufy.hammf.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cbh.hammf.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mma.tanke756.top

Ruby: arr.select { |x| x > 3 }
来源：http://cik.hnxiangtu.top

C#:   list.Where(x => x > 3).ToList()
来源：http://bpv.mhx1999.top

[D14] 映射转换（每个元素变形）
来源：http://fky.cashguo.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xjt.iojbl.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://por.jiagoushi.top

JS:   arr.map(x => x * 2)
来源：http://dcr.yanxiufei.cn

TS:   arr.map(x => x * 2)
来源：http://jwe.fzhhl.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://nwl.jyoumei.cn

Go:   // 手写循环
来源：http://uxr.mhx1999.top

Ruby: arr.map { |x| x * 2 }
来源：http://nak.xinyue.icu

C#:   list.Select(x => x * 2).ToList()
来源：http://fvx.zhengqikj.top

[D15] 去重
来源：http://ikb.hammf.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lyg.bjfxy.top

PHP:  array_unique($arr);
来源：http://uev.mhx1999.top

JS:   [...new Set(arr)]
来源：http://mdx.tarul.cn

TS:   [...new Set(arr)]
来源：http://tqt.c1oappe.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cbl.316326.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://hsq.jlsjyb.cn

Ruby: arr.uniq
来源：http://xks.jinqigufen.top

C#:   list.Distinct().ToList()
来源：http://wbb.xziqi.cn

[D16] 求和与平均值
来源：http://org.pengpengdd.cyou

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dqo.ctjpmb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fmt.yueranfly.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://oni.tian-w.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://trr.cucudq.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vnr.ctjpmb.com

Go:   // 手写循环累加
来源：http://eto.svipenyu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hcf.hywenlv.cn

C#:   list.Sum();  list.Average()
来源：http://cbe.ctjpmb.com

[D17] 最大值与最小值
来源：http://ouk.yj20258.top

Py:   max(arr);  min(arr)
来源：http://lce.nanxinkj.top

PHP:  max($arr);  min($arr);
来源：http://jsl.aizwys.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mcz.xinyue.icu

TS:   Math.max(...arr);
来源：http://uhg.xingfuxueyuan.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://vec.havefunace.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qci.zdqjudy.top

Ruby: arr.max;  arr.min
来源：http://rnq.chenjidiqi.icu

C#:   list.Max();  list.Min()
来源：http://mcp.jianghu66.top

[D18] 扁平化嵌套数组
来源：http://pxv.havefunace.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jws.tianlin.xyz

PHP:  array_merge(...$nested);
来源：http://xcp.kuanghao11.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ttx.ybcxt.top

TS:   nested.flat();
来源：http://rsn.316326.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pln.haohaochexian.top

Go:   // 手写双层循环
来源：http://kgj.tian-w.cn

Ruby: nested.flatten
来源：http://kcg.yongpay.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://yfr.ybcxt.top

[D19] 按字段分组
来源：http://ywu.hysaishi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qqs.tanke756.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mmb.shuidangran.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://iam.feifeiyinyue.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://kcm.xinyue.icu

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pkj.ctjpmb.com

Go:   // 手写 map[string][]T
来源：http://tqh.quarkkingdee.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://efb.cheryme.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://okv.chenzaomai.com

[D20] 统计每个元素出现次数
来源：http://nrc.gaohongyu789.top

Py:   Counter(arr)
来源：http://dor.xuanzx.com

PHP:  array_count_values($arr);
来源：http://zfe.zhengqikj.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://faa.feifeiyinyue.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rzy.chenlongwang.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dsj.zdqjudy.top

Go:   // 手写 map[T]int
来源：http://lsg.yangfankeji.com

Ruby: arr.tally
来源：http://kbm.hnqzz.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://soq.meibo888.top

[D21] 判断是否包含某元素
来源：http://vah.pengpengdd.cyou

Py:   x in arr
来源：http://eht.hnqzz.top

PHP:  in_array($x, $arr, true);
来源：http://ghu.c1oappe.top

JS:   arr.includes(x)
来源：http://lqj.sufxvd.cn

TS:   arr.includes(x)
来源：http://yye.pycfn.com

Java: list.contains(x)
来源：http://kiw.dashuyun.cn

Go:   slices.Contains(arr, x)
来源：http://ypg.xinyue.icu

Ruby: arr.include?(x)
来源：http://szg.pengpengdd.cyou

C#:   list.Contains(x)
来源：http://udd.xingfuxueyuan.xyz

[D22] 复制数组（避免共享引用）
来源：http://ekk.zhongyouzk.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cnh.ydzc1.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ikv.tarul.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://eov.yvedp.cn

TS:   [...arr];
来源：http://awr.pycfn.com

Java: new ArrayList<>(list);
来源：http://cor.yangfankeji.com

Go:   copied := append([]int(nil), arr...)
来源：http://atp.xinyue.icu

Ruby: arr.dup;  arr.clone
来源：http://bdu.9152youxi.cn

C#:   new List<int>(list);
来源：http://mwq.pycfn.com

[D23] reduce 累积计算
来源：http://xjs.ppjwa.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xgn.vehdjk.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bga.pycfn.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nhw.ppjwa.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cpg.jqgfzy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://zss.kuanghao11.cn

Go:   // 手写循环
来源：http://hqq.zhoulong.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qrf.52xcode.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ghh.tarul.cn

[D24] 字典 / Map 基本操作
来源：http://afz.shanyushiyangkeji.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yto.smart0.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hdd.hcnkem.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lhb.svipenyu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xyk.jinqigfzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://unu.guannengcc.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yjw.smart0.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qiw.zhoulong.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xji.xuetiantiany.cn

[D25] Set 集合去重与交并差
来源：http://ffm.yuanzhike.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jej.havefunace.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dwv.xinyue.icu

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bkt.gogol.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tfi.daxiang520.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dvm.jlsjyb.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jlt.chenzaomai.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hwy.ivvv.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rhj.xingfuxueyuan.xyz

[D26] 数组转字符串
来源：http://qpu.chenlongwang.top

Py:   ", ".join(map(str, arr))
来源：http://siw.hammf.cn

PHP:  implode(", ", $arr);
来源：http://fpd.redwolf501.top

JS:   arr.join(", ")
来源：http://fix.hcnkem.com

TS:   arr.join(", ")
来源：http://lnd.shanyushiyangkeji.top

Java: String.join(", ", list)
来源：http://cgh.zdqjudy.top

Go:   strings.Join(strs, ", ")
来源：http://nns.jinqigufen.top

Ruby: arr.join(", ")
来源：http://gvh.yfazqb.com

C#:   string.Join(", ", list)
来源：http://gwt.chenlongwang.top

================================================================================
来源：http://pql.yonumen.top

E. 字符串处理
来源：http://jdz.kuanghao11.cn

================================================================================
来源：http://kwn.yanxiufei.cn

[E01] 拼接字符串
来源：http://clv.nanxinkj.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://emx.cdnleiting.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hai.yj202588.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qcd.shanyushiyangtech.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ipi.zhiwuduotai.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xwk.fanxiaobao.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nmp.hcnkem.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zhf.ppjwa.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mad.cashguo.top

[E02] 重复字符串
来源：http://nkt.zhiwuduotai.top

Py:   "ab" * 3
来源：http://tah.sweek.top

PHP:  str_repeat("ab", 3);
来源：http://ljk.sjlbkw.cn

JS:   "ab".repeat(3)
来源：http://tzm.yj202588.top

TS:   "ab".repeat(3)
来源：http://spz.snrcjt.cn

Java: "ab".repeat(3)
来源：http://uyh.nwbrower.top

Go:   strings.Repeat("ab", 3)
来源：http://psi.sweek.top

Ruby: "ab" * 3
来源：http://msi.zhijiandao.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://opv.tanke756.top

[E03] 截取子串
来源：http://oqd.zhiwuduotai.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ueo.aibaodan.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nrh.9152youxi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xhs.xinyue.icu

TS:   s.slice(1, 4)
来源：http://ssn.yj20258.top

Java: s.substring(1, 4)
来源：http://div.sjlbkw.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cqb.meibo888.top

Ruby: s[1, 3];  s[1..3]
来源：http://iay.gaohongyu789.top

C#:   s.Substring(1, 3)
来源：http://jra.xuetiantiany.cn

[E04] 查找子串位置
来源：http://tfi.shzxlz.cn

Py:   s.find("x");  s.index("x")
来源：http://qze.meibo888.top

PHP:  strpos($s, "x");
来源：http://juq.bjfxy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ago.aizwys.cn

TS:   s.indexOf("x")
来源：http://jyd.yfazqb.com

Java: s.indexOf("x")
来源：http://qac.cucudq.cn

Go:   strings.Index(s, "x")
来源：http://dsn.yfazqb.com

Ruby: s.index("x")
来源：http://ikn.gaohongyu789.top

C#:   s.IndexOf("x")
来源：http://aqy.fengsongda.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://but.xziqi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zwa.snrcjt.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xtf.svipenyu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://srf.sweek.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ywv.xingfuxueyuan.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rfz.shanyushiyangkeji.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vju.cdnleiting.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://boi.zycfv.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zjv.cheryme.top

[E06] 替换子串
来源：http://plr.zhaomingkeji.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://eln.zhiwuduotai.top

PHP:  str_replace("a", "b", $s);
来源：http://mch.wangshuangyany.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zxo.tian-w.cn

TS:   s.replaceAll("a", "b")
来源：http://lsz.yj20258.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uln.zhoulong.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rae.hfpthk.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mgf.zdqjudy.top

C#:   s.Replace("a", "b")
来源：http://mqd.daxiang520.top

[E07] 按分隔符拆分
来源：http://uap.vehdjk.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://iso.mhx1999.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rvi.uphjek.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://jdd.fktsv.cn

TS:   s.split(",")
来源：http://iqi.guowangkeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://mey.jqgufenzy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://llp.fktsv.cn

Ruby: s.split(",");  s.split
来源：http://rjz.fktsv.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uuu.zdqjudy.top

[E08] 数组按分隔符合并
来源：http://bls.yvedp.cn

Py:   ",".join(items)
来源：http://nvg.birdmap.top

PHP:  implode(",", $items);
来源：http://qtv.jqgfzy.top

JS:   items.join(",")
来源：http://lrd.guowangkeji.top

TS:   items.join(",")
来源：http://bad.fehbvm.com

Java: String.join(",", items)
来源：http://ubf.shangyingyoupin.top

Go:   strings.Join(items, ",")
来源：http://dvw.yuanzhike.top

Ruby: items.join(",")
来源：http://san.hywenlv.cn

C#:   string.Join(",", items)
来源：http://fhn.shanyushiyangtech.top

[E09] 去除所有空白字符
来源：http://puu.hongshengwenyu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vqo.ppjwa.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cyl.ehwqpu.com

JS:   s.replace(/\s+/g, "")
来源：http://npi.yuanzhike.top

TS:   s.replace(/\s+/g, "")
来源：http://ban.andypj.xyz

Java: s.replaceAll("\\s+", "")
来源：http://qds.zhongyouzk.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://rgy.yvedp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xpc.zhongyouzk.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vab.cdnleiting.top

[E10] 左侧补零 / 定长填充
来源：http://dlx.ivvv.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pvt.bjfxy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ojo.shangyingyoupin.top

JS:   "7".padStart(3, "0")
来源：http://rfq.fktsv.cn

TS:   "7".padStart(3, "0")
来源：http://bwb.mhx1999.top

Java: String.format("%03d", 7)
来源：http://shn.fengsongda.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://hgv.yj20258888.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yek.tarul.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://weo.hesvh.cn

[E11] 反转字符串
来源：http://yeu.dashuyun.cn

Py:   s[::-1]
来源：http://uqt.shzxlz.cn

PHP:  strrev($s);
来源：http://sof.yj20258.top

JS:   [...s].reverse().join("")
来源：http://zpp.sysykeji.top

TS:   [...s].reverse().join("")
来源：http://nfk.vqdsnc.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://dik.pycfn.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://qih.jyoumei.cn

Ruby: s.reverse
来源：http://diy.vqdsnc.cn

C#:   new string(s.Reverse().ToArray())
来源：http://cnf.zdbjq.cn

[E12] 统计某字符出现次数
来源：http://xau.andypj.xyz

Py:   s.count("a")
来源：http://oju.yj20258888.top

PHP:  substr_count($s, "a");
来源：http://ske.cashguo.top

JS:   s.split("a").length - 1
来源：http://abd.kuanghao11.cn

TS:   s.split("a").length - 1
来源：http://ivk.shanyushiyangkeji.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://icy.yj20258888.top

Go:   strings.Count(s, "a")
来源：http://cks.ydjk.org.cn

Ruby: s.count("a")
来源：http://srk.tarul.cn

C#:   s.Count(c => c == 'a')
来源：http://wfn.zhoulong.xyz

[E13] 逐字符遍历
来源：http://cau.gotoacloud.top

Py:   for ch in s: print(ch)
来源：http://acn.jlsjyb.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://afs.fehbvm.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://phl.redwolf501.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://yfc.zdbjq.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qaz.cucudq.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pup.havefunace.top

Ruby: s.each_char { |ch| puts ch }
来源：http://isd.pycfn.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lwx.gaohongyu789.top

[E14] URL 编码与 Base64
来源：http://mfd.316326.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bqr.tanke756.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://cee.andypj.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nrf.uphjek.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://khk.shuidangran.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nkv.sweek.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rok.tian-w.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xfg.meibo888.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://onz.hnxiangtu.top

[E15] HTML 转义 / 反转义
来源：http://dlk.xinyue.icu

Py:   html.escape(s);  html.unescape(s)
来源：http://qxo.tian-w.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vya.sysykeji.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ann.hongshengwenyu.top

TS:   // 同上，务必做 XSS 过滤
来源：http://lss.guannengcc.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zbj.wangdashe.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qal.dashuyun.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vem.daria6918.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nsx.xuetiantiany.cn

[E16] 数字千分位
来源：http://idc.smart0.xyz

Py:   f"{1234567:,}"
来源：http://ykw.bbcook.cn

PHP:  number_format(1234567);
来源：http://bte.zhaomingkeji.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://tqn.havefunace.top

TS:   (1234567).toLocaleString("en-US")
来源：http://wnc.zhaomingkeji.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ndh.kuanghao11.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://siz.uphjek.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ibq.jinqigfzy.top

C#:   1234567.ToString("N0")
来源：http://aau.svipenyu.cn

[E17] 首字母大写
来源：http://jnf.fehbvm.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ehm.nanxinkj.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://llt.yuanzhike.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bth.zhongyouzk.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rbp.pycfn.com


<!-- 参考信息 -->