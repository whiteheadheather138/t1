代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jnb.ehwqpu.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cbp.hysaishi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dby.hcnkem.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nar.shuidangran.top

[D11] 反转数组
来源：http://idi.cashguo.top

Py:   arr[::-1];  arr.reverse()
来源：http://qei.cdnleiting.top

PHP:  array_reverse($arr);
来源：http://mmu.dashuyun.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gqh.fzhhl.top

TS:   [...arr].reverse();
来源：http://rzb.dianchejie.cn

Java: Collections.reverse(list);
来源：http://msk.zhongyouzk.top

Go:   slices.Reverse(arr)
来源：http://ugr.quarkkingdee.top

Ruby: arr.reverse
来源：http://jdu.zhixingplan.top

C#:   list.Reverse();
来源：http://rlw.yangfankeji.com

[D12] 查找元素下标
来源：http://cmj.yonumen.top

Py:   arr.index(x);  x in arr
来源：http://jbl.fanxiaobao.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xjw.cqqwz.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jvx.daxiang520.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ryq.gogol.net.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tek.chenzaomai.com

Go:   slices.Index(arr, x)
来源：http://qjh.zdbjq.cn

Ruby: arr.index(x)
来源：http://clb.c1oappe.top

C#:   list.IndexOf(x);
来源：http://mho.shanyushiyangkeji.top

[D13] 过滤（保留满足条件的）
来源：http://ekf.jinqigfzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://srn.feifeiyinyue.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mew.ctjpmb.com

JS:   arr.filter(x => x > 3)
来源：http://udf.xuanzx.com

TS:   arr.filter(x => x > 3)
来源：http://cbc.cheryme.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kll.jinqigufen.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gqh.fanxiaobao.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://lgx.meibo888.top

C#:   list.Where(x => x > 3).ToList()
来源：http://azv.ydjk.org.cn

[D14] 映射转换（每个元素变形）
来源：http://paq.0kj1m.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ilu.jinyuanbaomall.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mfp.jyoumei.cn

JS:   arr.map(x => x * 2)
来源：http://ojv.iojbl.cn

TS:   arr.map(x => x * 2)
来源：http://uhl.quarkkingdee.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://dxb.wangdashe.top

Go:   // 手写循环
来源：http://ufy.redwolf501.top

Ruby: arr.map { |x| x * 2 }
来源：http://goo.sjlbkw.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xzl.yueranfly.top

[D15] 去重
来源：http://lwi.9152youxi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ovj.meibo888.top

PHP:  array_unique($arr);
来源：http://kia.gotoacloud.top

JS:   [...new Set(arr)]
来源：http://hes.wangdashe.top

TS:   [...new Set(arr)]
来源：http://bhw.shanyushiyangkeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lkk.sxryk.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yii.cdnleiting.top

Ruby: arr.uniq
来源：http://awk.yonumen.top

C#:   list.Distinct().ToList()
来源：http://hyn.hcnkem.com

[D16] 求和与平均值
来源：http://uoi.fanxiaobao.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vqa.shanyushiyangtech.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ixe.kuanghao11.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://csh.shanyushiyangtech.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lwo.yj202588.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bej.jiagoushi.top

Go:   // 手写循环累加
来源：http://fbw.xuanzx.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tro.dianchejie.cn

C#:   list.Sum();  list.Average()
来源：http://flz.hywenlv.cn

[D17] 最大值与最小值
来源：http://abf.jqgufenzy.top

Py:   max(arr);  min(arr)
来源：http://jao.ctjpmb.com

PHP:  max($arr);  min($arr);
来源：http://auk.yuxming.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jvs.shzxlz.cn

TS:   Math.max(...arr);
来源：http://jcv.zycfv.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pnq.zycfv.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kyo.hywenlv.cn

Ruby: arr.max;  arr.min
来源：http://sew.0kj1m.cn

C#:   list.Max();  list.Min()
来源：http://lzg.zhaomingkeji.xyz

[D18] 扁平化嵌套数组
来源：http://tqx.hfpthk.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qbk.cdnleiting.top

PHP:  array_merge(...$nested);
来源：http://ouw.zhoulong.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://smt.0kj1m.cn

TS:   nested.flat();
来源：http://sge.fanxiaobao.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pzp.ivvv.top

Go:   // 手写双层循环
来源：http://hwh.cashguo.top

Ruby: nested.flatten
来源：http://jkm.quarkkingdee.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://vck.jiagoushi.top

[D19] 按字段分组
来源：http://uzz.nanxuanxn.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rou.fanxiaobao.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cre.ybcxt.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://meq.yangfankeji.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://rjb.jinyuanbaomall.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ihe.ivvv.top

Go:   // 手写 map[string][]T
来源：http://dkj.feifeiyinyue.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://wqj.0kj1m.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pmz.vehdjk.com

[D20] 统计每个元素出现次数
来源：http://tqy.andypj.xyz

Py:   Counter(arr)
来源：http://sbe.ydzc1.top

PHP:  array_count_values($arr);
来源：http://dbt.yanxiufei.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cit.tian-w.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://atg.xinyue.icu

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lrx.fehbvm.com

Go:   // 手写 map[T]int
来源：http://azf.jlsjyb.cn

Ruby: arr.tally
来源：http://sys.vqdsnc.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ypv.hfpthk.cn

[D21] 判断是否包含某元素
来源：http://ton.quarkkingdee.top

Py:   x in arr
来源：http://kiz.xuanzx.com

PHP:  in_array($x, $arr, true);
来源：http://kjz.zhiwuduotai.top

JS:   arr.includes(x)
来源：http://yae.yj20258.top

TS:   arr.includes(x)
来源：http://yrj.jlsjyb.cn

Java: list.contains(x)
来源：http://ejy.nanxuanxn.top

Go:   slices.Contains(arr, x)
来源：http://pys.wangshuangyany.cn

Ruby: arr.include?(x)
来源：http://gtl.c1oappe.top

C#:   list.Contains(x)
来源：http://hor.yuanzhike.top

[D22] 复制数组（避免共享引用）
来源：http://lhd.chenzaomai.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://axa.ehwqpu.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ucq.sweek.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rwf.hysaishi.cn

TS:   [...arr];
来源：http://uun.hesvh.cn

Java: new ArrayList<>(list);
来源：http://ftg.yangfankeji.com

Go:   copied := append([]int(nil), arr...)
来源：http://aeo.zhaomingkeji.xyz

Ruby: arr.dup;  arr.clone
来源：http://bll.vehdjk.com

C#:   new List<int>(list);
来源：http://uhv.cheryme.top

[D23] reduce 累积计算
来源：http://nzx.mhx1999.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qjn.yonumen.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ecw.zhixingplan.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xdp.0kj1m.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://aan.yueranfly.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://pou.mhx1999.top

Go:   // 手写循环
来源：http://wsx.cqqwz.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fzc.zycfv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xoq.ydzc1.top

[D24] 字典 / Map 基本操作
来源：http://myw.gaohongyu789.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qbj.0kj1m.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wsu.jianghu66.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://aaa.xuanzx.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hmx.yvedp.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zek.nwbrower.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ffj.hnxiangtu.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lqi.jinghuilouyu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://onq.mhx1999.top

[D25] Set 集合去重与交并差
来源：http://tze.jinqigfzy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sks.yonumen.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bju.yonumen.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bxd.uphjek.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qqx.ppjwa.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zlr.yj202588.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kli.haohaochexian.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bia.yj20258.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hbg.vehdjk.com

[D26] 数组转字符串
来源：http://tsn.fktsv.cn

Py:   ", ".join(map(str, arr))
来源：http://igb.cheryme.top

PHP:  implode(", ", $arr);
来源：http://rlt.feifeiyinyue.top

JS:   arr.join(", ")
来源：http://wnz.smart0.xyz

TS:   arr.join(", ")
来源：http://osf.wangshuangyany.cn

Java: String.join(", ", list)
来源：http://ygd.guowangkeji.top

Go:   strings.Join(strs, ", ")
来源：http://cno.yfazqb.com

Ruby: arr.join(", ")
来源：http://bfe.smart0.xyz

C#:   string.Join(", ", list)
来源：http://caz.ydjk.org.cn

================================================================================
来源：http://pzp.yj20258888.top

E. 字符串处理
来源：http://szs.zhiwuduotai.top

================================================================================
来源：http://ztq.bbcook.cn

[E01] 拼接字符串
来源：http://emz.sweek.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://eqh.hfpthk.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hiq.fehbvm.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rlj.jinyuanbaomall.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lnf.mhx1999.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qcz.kuanghao11.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cum.yvedp.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gsl.zycfv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lat.sufxvd.cn

[E02] 重复字符串
来源：http://leg.kuanghao11.cn

Py:   "ab" * 3
来源：http://jbl.zdbjq.cn

PHP:  str_repeat("ab", 3);
来源：http://qic.hysaishi.cn

JS:   "ab".repeat(3)
来源：http://dji.yongpay.top

TS:   "ab".repeat(3)
来源：http://sdh.gotoacloud.top

Java: "ab".repeat(3)
来源：http://jpd.yuanzhike.top

Go:   strings.Repeat("ab", 3)
来源：http://fod.zhoulong.xyz

Ruby: "ab" * 3
来源：http://pgs.feifeiyinyue.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rlh.zhongyouzk.top

[E03] 截取子串
来源：http://yyt.hesvh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xlc.fehbvm.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://opu.zdbjq.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ssz.ehwqpu.com

TS:   s.slice(1, 4)
来源：http://pud.chenzaomai.com

Java: s.substring(1, 4)
来源：http://mvb.zhongyouzk.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hhc.zhongyouzk.top

Ruby: s[1, 3];  s[1..3]
来源：http://chj.epnwcf.com

C#:   s.Substring(1, 3)
来源：http://ega.zhixingplan.top

[E04] 查找子串位置
来源：http://zqv.yj20258.top

Py:   s.find("x");  s.index("x")
来源：http://ood.hammf.cn

PHP:  strpos($s, "x");
来源：http://dru.wangdashe.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://eqf.52xcode.cn

TS:   s.indexOf("x")
来源：http://nsr.guannengcc.top

Java: s.indexOf("x")
来源：http://dns.smart0.xyz

Go:   strings.Index(s, "x")
来源：http://fvm.havefunace.top

Ruby: s.index("x")
来源：http://whm.epnwcf.com

C#:   s.IndexOf("x")
来源：http://eia.feifeiyinyue.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://moe.zycfv.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qbt.jinghuilouyu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://oqt.cheryme.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vyt.ydjk.org.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://rzr.feifeiyinyue.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nhh.cqqwz.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cyz.hnxiangtu.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wmk.jqgfzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lna.cashguo.top

[E06] 替换子串
来源：http://zqr.jinqigfzy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bli.zhengqikj.top

PHP:  str_replace("a", "b", $s);
来源：http://pzf.hysaishi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ysv.zhaomingkeji.xyz

TS:   s.replaceAll("a", "b")
来源：http://ukq.cucudq.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gdp.xinyue.icu

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jpi.wangdashe.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jfy.0kj1m.cn

C#:   s.Replace("a", "b")
来源：http://inv.chenlongwang.top

[E07] 按分隔符拆分
来源：http://gfc.cqqwz.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://com.feifeiyinyue.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vci.zdqjudy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://agb.daria6918.cn

TS:   s.split(",")
来源：http://bfj.shangyingyoupin.top

Java: s.split(",");  s.split("\\s+")
来源：http://xat.sxryk.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baz.zhoulong.xyz

Ruby: s.split(",");  s.split
来源：http://swz.kuanghao11.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fju.gzhubu.top

[E08] 数组按分隔符合并
来源：http://cnr.xylfe.cn

Py:   ",".join(items)
来源：http://egz.hnqzz.top

PHP:  implode(",", $items);
来源：http://nuu.yongpay.top

JS:   items.join(",")
来源：http://jfb.meibo888.top

TS:   items.join(",")
来源：http://znn.gotoacloud.top

Java: String.join(",", items)
来源：http://gsm.shzxlz.cn

Go:   strings.Join(items, ",")
来源：http://uko.shzxlz.cn

Ruby: items.join(",")
来源：http://tmv.cashguo.top

C#:   string.Join(",", items)
来源：http://kyp.daxiang520.top

[E09] 去除所有空白字符
来源：http://djp.xziqi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jvx.xziqi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hal.yuxming.cn

JS:   s.replace(/\s+/g, "")
来源：http://fro.chenjidiqi.icu

TS:   s.replace(/\s+/g, "")
来源：http://vhn.cdnleiting.top

Java: s.replaceAll("\\s+", "")
来源：http://zhq.zdbjq.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cqs.fktsv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pqh.zhiwuduotai.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pas.ppjwa.cn

[E10] 左侧补零 / 定长填充
来源：http://dhr.daxiang520.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://axe.yj202588.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://djp.yanxiufei.cn

JS:   "7".padStart(3, "0")
来源：http://jyq.smart0.xyz

TS:   "7".padStart(3, "0")
来源：http://vtb.fzhhl.top

Java: String.format("%03d", 7)
来源：http://vkx.bbcook.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://lae.zdqjudy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tyi.havefunace.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://byt.ydjk.org.cn

[E11] 反转字符串
来源：http://mzq.guowangkeji.top

Py:   s[::-1]
来源：http://iak.guowangkeji.top

PHP:  strrev($s);
来源：http://gno.chenjidiqi.icu

JS:   [...s].reverse().join("")
来源：http://tud.jiagoushi.top

TS:   [...s].reverse().join("")
来源：http://xcy.snrcjt.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://juf.xingfuxueyuan.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://blb.cheryme.top

Ruby: s.reverse
来源：http://xur.ydjk.org.cn

C#:   new string(s.Reverse().ToArray())
来源：http://npo.yuxming.cn

[E12] 统计某字符出现次数
来源：http://ssz.snrcjt.cn

Py:   s.count("a")
来源：http://hvc.zhengqikj.top

PHP:  substr_count($s, "a");
来源：http://xve.hcnkem.com

JS:   s.split("a").length - 1
来源：http://gid.ydjk.org.cn

TS:   s.split("a").length - 1
来源：http://ygz.guannengcc.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vhw.ctjpmb.com

Go:   strings.Count(s, "a")
来源：http://jvt.snrcjt.cn

Ruby: s.count("a")
来源：http://jfq.nwbrower.top

C#:   s.Count(c => c == 'a')
来源：http://sgm.mhx1999.top

[E13] 逐字符遍历
来源：http://jeg.shuidangran.top

Py:   for ch in s: print(ch)
来源：http://qkb.0kj1m.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pgz.xingfuxueyuan.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://kvi.jqgufenzy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://iil.hesvh.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gic.wangdashe.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cni.jqgufenzy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://huw.zhoulong.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ums.yueranfly.top

[E14] URL 编码与 Base64
来源：http://cci.zhongyouzk.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bmj.daxiang520.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://udq.vehdjk.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gzh.mhx1999.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://aeq.mhx1999.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wyw.andypj.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://trt.daxiang520.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yko.ydjk.org.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kel.yangfankeji.com

[E15] HTML 转义 / 反转义
来源：http://usu.tarul.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://joa.yonumen.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sed.dashuyun.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://axg.tianlin.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://mwv.yvedp.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cpc.iojbl.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jmx.cdnleiting.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rvw.yanxiufei.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tkv.quarkkingdee.top

[E16] 数字千分位
来源：http://xkc.jqgfzy.top

Py:   f"{1234567:,}"
来源：http://gvs.zdbjq.cn

PHP:  number_format(1234567);
来源：http://zfk.chenlongwang.top

JS:   (1234567).toLocaleString("en-US")
来源：http://stt.ehwqpu.com

TS:   (1234567).toLocaleString("en-US")
来源：http://jfj.aibaodan.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://awm.zhiwuduotai.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bba.yanxiufei.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dtv.hesvh.cn

C#:   1234567.ToString("N0")
来源：http://vpx.havefunace.top

[E17] 首字母大写
来源：http://bmk.gaohongyu789.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qzi.ivvv.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://sbi.yvedp.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ucd.gotoacloud.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zou.jianghu66.top


<!-- 参考信息 -->