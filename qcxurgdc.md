代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://oof.tanke756.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zwz.sysykeji.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ncr.aizwys.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qwm.dashuyun.cn

[D11] 反转数组
来源：http://hqj.cdnleiting.top

Py:   arr[::-1];  arr.reverse()
来源：http://owd.ywan-chungtsiang.top

PHP:  array_reverse($arr);
来源：http://arx.yj20258.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wof.0kj1m.cn

TS:   [...arr].reverse();
来源：http://gor.guannengcc.top

Java: Collections.reverse(list);
来源：http://aol.zhijiandao.cn

Go:   slices.Reverse(arr)
来源：http://upe.tian-w.cn

Ruby: arr.reverse
来源：http://klw.0kj1m.cn

C#:   list.Reverse();
来源：http://qbt.yvedp.cn

[D12] 查找元素下标
来源：http://rls.yongpay.top

Py:   arr.index(x);  x in arr
来源：http://zla.shuidangran.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zgl.gotoacloud.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rpi.meibo888.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ydh.jiagoushi.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vhe.vqdsnc.cn

Go:   slices.Index(arr, x)
来源：http://gcb.fzhhl.top

Ruby: arr.index(x)
来源：http://gco.yuanzhike.top

C#:   list.IndexOf(x);
来源：http://veg.shuidangran.top

[D13] 过滤（保留满足条件的）
来源：http://upi.hnxiangtu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wwn.9152youxi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://svf.yueranfly.top

JS:   arr.filter(x => x > 3)
来源：http://fng.epnwcf.com

TS:   arr.filter(x => x > 3)
来源：http://dfv.xziqi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vcq.cashguo.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://odb.meibo888.top

Ruby: arr.select { |x| x > 3 }
来源：http://fmp.zhijiandao.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yla.shanyushiyangkeji.top

[D14] 映射转换（每个元素变形）
来源：http://kjq.sweek.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://exv.jqgfzy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jgg.hnqzz.top

JS:   arr.map(x => x * 2)
来源：http://jxf.guowangkeji.top

TS:   arr.map(x => x * 2)
来源：http://xym.yueranfly.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://blu.xylfe.cn

Go:   // 手写循环
来源：http://tzw.fehbvm.com

Ruby: arr.map { |x| x * 2 }
来源：http://spt.vqdsnc.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://txg.guowangkeji.top

[D15] 去重
来源：http://fpq.zycfv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kja.0kj1m.cn

PHP:  array_unique($arr);
来源：http://egi.aibaodan.cn

JS:   [...new Set(arr)]
来源：http://bvp.smart0.xyz

TS:   [...new Set(arr)]
来源：http://jld.hysaishi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mch.52xcode.cn

Go:   // 用 map[T]struct{} 手写
来源：http://rrx.snrcjt.cn

Ruby: arr.uniq
来源：http://krb.shangyingyoupin.top

C#:   list.Distinct().ToList()
来源：http://afk.uphjek.com

[D16] 求和与平均值
来源：http://dgm.smart0.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xfa.zhixingplan.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qxw.fktsv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://unx.jlsjyb.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://axd.quarkkingdee.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fuj.havefunace.top

Go:   // 手写循环累加
来源：http://how.xingfuxueyuan.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://eeo.fzhhl.top

C#:   list.Sum();  list.Average()
来源：http://egr.hfpthk.cn

[D17] 最大值与最小值
来源：http://tvq.sxryk.cn

Py:   max(arr);  min(arr)
来源：http://kpp.shanyushiyangkeji.top

PHP:  max($arr);  min($arr);
来源：http://rws.cashguo.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ebk.bbcook.cn

TS:   Math.max(...arr);
来源：http://qvy.uphjek.com

Java: Collections.max(list);  Collections.min(list);
来源：http://gkd.jinghuilouyu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hqc.hywenlv.cn

Ruby: arr.max;  arr.min
来源：http://jdp.ehwqpu.com

C#:   list.Max();  list.Min()
来源：http://ggb.wangdashe.top

[D18] 扁平化嵌套数组
来源：http://gir.hnxiangtu.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kdu.hongshengwenyu.top

PHP:  array_merge(...$nested);
来源：http://lgb.pengpengdd.cyou

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mgh.yongpay.top

TS:   nested.flat();
来源：http://bmc.cqqwz.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yvd.yvedp.cn

Go:   // 手写双层循环
来源：http://mjt.kuanghao11.cn

Ruby: nested.flatten
来源：http://nzc.yuanzhike.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://xiy.jianghu66.top

[D19] 按字段分组
来源：http://jot.shanyushiyangkeji.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pup.zhongyouzk.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zvq.fanxiaobao.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uqk.0kj1m.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://nkp.fktsv.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ibu.cdnleiting.top

Go:   // 手写 map[string][]T
来源：http://vyl.yj20258.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://itl.guannengcc.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rgj.jqgfzy.top

[D20] 统计每个元素出现次数
来源：http://mey.sxryk.cn

Py:   Counter(arr)
来源：http://tmr.redwolf501.top

PHP:  array_count_values($arr);
来源：http://gpf.yongpay.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ryx.cdnleiting.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://npz.xuanzx.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pvg.nwbrower.top

Go:   // 手写 map[T]int
来源：http://aji.ydjk.org.cn

Ruby: arr.tally
来源：http://gkx.cucudq.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fab.hysaishi.cn

[D21] 判断是否包含某元素
来源：http://cev.jlsjyb.cn

Py:   x in arr
来源：http://xnd.hnxiangtu.top

PHP:  in_array($x, $arr, true);
来源：http://yle.ivvv.top

JS:   arr.includes(x)
来源：http://onq.cucudq.cn

TS:   arr.includes(x)
来源：http://vbp.jiagoushi.top

Java: list.contains(x)
来源：http://wqz.jinyuanbaomall.cn

Go:   slices.Contains(arr, x)
来源：http://aat.zhaomingkeji.xyz

Ruby: arr.include?(x)
来源：http://xbg.chenjidiqi.icu

C#:   list.Contains(x)
来源：http://egp.bbcook.cn

[D22] 复制数组（避免共享引用）
来源：http://vqb.jinqigufen.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yht.cqqwz.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ohs.gaohongyu789.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zso.fanxiaobao.xyz

TS:   [...arr];
来源：http://etl.jinghuilouyu.cn

Java: new ArrayList<>(list);
来源：http://yqi.fzhhl.top

Go:   copied := append([]int(nil), arr...)
来源：http://wwx.fktsv.cn

Ruby: arr.dup;  arr.clone
来源：http://bqc.chenjidiqi.icu

C#:   new List<int>(list);
来源：http://hsh.andypj.xyz

[D23] reduce 累积计算
来源：http://ilv.chenjidiqi.icu

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nbm.fktsv.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rte.xinyue.icu

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nhm.redwolf501.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nvi.kuanghao11.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zwy.pycfn.com

Go:   // 手写循环
来源：http://pdo.52xcode.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xpn.jyoumei.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kpf.shuidangran.top

[D24] 字典 / Map 基本操作
来源：http://fax.zdqjudy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cff.ydjk.org.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fek.zycfv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mmz.fanxiaobao.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pnm.nanxinkj.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sce.zhongyouzk.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qav.iojbl.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wkt.shangyingyoupin.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://njc.zdbjq.cn

[D25] Set 集合去重与交并差
来源：http://aiq.jianghu66.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xav.ctjpmb.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dng.jyoumei.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nxz.uphjek.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hgq.cucudq.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bso.gotoacloud.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rah.fzhhl.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nro.gzhubu.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nkj.fzhhl.top

[D26] 数组转字符串
来源：http://ypx.jiagoushi.top

Py:   ", ".join(map(str, arr))
来源：http://spe.jianghu66.top

PHP:  implode(", ", $arr);
来源：http://nfc.shuidangran.top

JS:   arr.join(", ")
来源：http://jhq.zhixingplan.top

TS:   arr.join(", ")
来源：http://utd.xingfuxueyuan.xyz

Java: String.join(", ", list)
来源：http://vqr.dashuyun.cn

Go:   strings.Join(strs, ", ")
来源：http://vdm.svipenyu.cn

Ruby: arr.join(", ")
来源：http://upq.pycfn.com

C#:   string.Join(", ", list)
来源：http://eyf.svipenyu.cn

================================================================================
来源：http://mhw.iojbl.cn

E. 字符串处理
来源：http://fqb.zhijiandao.cn

================================================================================
来源：http://cwb.sufxvd.cn

[E01] 拼接字符串
来源：http://bko.jyoumei.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://eyl.guannengcc.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yrz.yanxiufei.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://owx.sjlbkw.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yci.zhijiandao.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://amd.xingfuxueyuan.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zbr.nanxuanxn.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ngu.xingfuxueyuan.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xhu.yj20258888.top

[E02] 重复字符串
来源：http://kpn.c1oappe.top

Py:   "ab" * 3
来源：http://trx.xinyue.icu

PHP:  str_repeat("ab", 3);
来源：http://qhl.ctjpmb.com

JS:   "ab".repeat(3)
来源：http://wqu.zhijiandao.cn

TS:   "ab".repeat(3)
来源：http://ilu.chenlongwang.top

Java: "ab".repeat(3)
来源：http://rwq.uphjek.com

Go:   strings.Repeat("ab", 3)
来源：http://pec.dianchejie.cn

Ruby: "ab" * 3
来源：http://olu.yj202588.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nlw.redwolf501.top

[E03] 截取子串
来源：http://zad.xuetiantiany.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yfr.pengpengdd.cyou

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xje.hongshengwenyu.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qhm.guowangkeji.top

TS:   s.slice(1, 4)
来源：http://hus.cucudq.cn

Java: s.substring(1, 4)
来源：http://myd.nwbrower.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jkw.uphjek.com

Ruby: s[1, 3];  s[1..3]
来源：http://lai.hfpthk.cn

C#:   s.Substring(1, 3)
来源：http://flt.gzhubu.top

[E04] 查找子串位置
来源：http://zxx.xingfuxueyuan.xyz

Py:   s.find("x");  s.index("x")
来源：http://vyq.tanke756.top

PHP:  strpos($s, "x");
来源：http://zvr.sxryk.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://otq.wangshuangyany.cn

TS:   s.indexOf("x")
来源：http://xvx.zdbjq.cn

Java: s.indexOf("x")
来源：http://sbv.xuanzx.com

Go:   strings.Index(s, "x")
来源：http://jee.hysaishi.cn

Ruby: s.index("x")
来源：http://zwl.wangshuangyany.cn

C#:   s.IndexOf("x")
来源：http://dwv.jyoumei.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://diw.chenjidiqi.icu

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uch.shuidangran.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tpe.gotoacloud.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cty.yvedp.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://sic.epnwcf.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lmq.jinghuilouyu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://oty.zhijiandao.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gcm.tanke756.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ocy.c1oappe.top

[E06] 替换子串
来源：http://sey.yanxiufei.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qvo.xylfe.cn

PHP:  str_replace("a", "b", $s);
来源：http://ogz.hywenlv.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nko.tianlin.xyz

TS:   s.replaceAll("a", "b")
来源：http://cpw.havefunace.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ixo.zhongyouzk.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gnb.chenjidiqi.icu

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://klg.hnxiangtu.top

C#:   s.Replace("a", "b")
来源：http://xiu.316326.xyz

[E07] 按分隔符拆分
来源：http://nzt.yueranfly.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pty.yj20258.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://clf.quarkkingdee.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://zrw.fehbvm.com

TS:   s.split(",")
来源：http://zjl.hysaishi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://bpf.wangshuangyany.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xsp.cashguo.top

Ruby: s.split(",");  s.split
来源：http://tva.yuxming.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ugm.zhaomingkeji.xyz

[E08] 数组按分隔符合并
来源：http://rnu.yonumen.top

Py:   ",".join(items)
来源：http://bfs.xingfuxueyuan.xyz

PHP:  implode(",", $items);
来源：http://npk.cheryme.top

JS:   items.join(",")
来源：http://aos.hysaishi.cn

TS:   items.join(",")
来源：http://gdn.cucudq.cn

Java: String.join(",", items)
来源：http://fck.hongshengwenyu.top

Go:   strings.Join(items, ",")
来源：http://wur.fanxiaobao.xyz

Ruby: items.join(",")
来源：http://sny.yj202588.top

C#:   string.Join(",", items)
来源：http://aqv.chenjidiqi.icu

[E09] 去除所有空白字符
来源：http://byn.9152youxi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fou.daxiang520.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qai.hcnkem.com

JS:   s.replace(/\s+/g, "")
来源：http://duh.guowangkeji.top

TS:   s.replace(/\s+/g, "")
来源：http://hxk.xylfe.cn

Java: s.replaceAll("\\s+", "")
来源：http://bph.0kj1m.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rtn.mhx1999.top

Ruby: s.gsub(/\s+/, "")
来源：http://oig.yueranfly.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://era.sweek.top

[E10] 左侧补零 / 定长填充
来源：http://apt.quarkkingdee.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fhw.zhoulong.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nzx.tarul.cn

JS:   "7".padStart(3, "0")
来源：http://ytx.jyoumei.cn

TS:   "7".padStart(3, "0")
来源：http://unt.pengpengdd.cyou

Java: String.format("%03d", 7)
来源：http://gak.ywan-chungtsiang.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://kfv.9152youxi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vdf.feifeiyinyue.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hin.zycfv.cn

[E11] 反转字符串
来源：http://xvm.jinghuilouyu.cn

Py:   s[::-1]
来源：http://klb.tarul.cn

PHP:  strrev($s);
来源：http://inm.shanyushiyangtech.top

JS:   [...s].reverse().join("")
来源：http://ddu.yuxming.cn

TS:   [...s].reverse().join("")
来源：http://moq.nwbrower.top

Java: new StringBuilder(s).reverse().toString()
来源：http://sol.bjfxy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://zvt.zhijiandao.cn

Ruby: s.reverse
来源：http://eoy.chenjidiqi.icu

C#:   new string(s.Reverse().ToArray())
来源：http://bnz.fengsongda.top

[E12] 统计某字符出现次数
来源：http://hvs.shanyushiyangkeji.top

Py:   s.count("a")
来源：http://uwm.kuanghao11.cn

PHP:  substr_count($s, "a");
来源：http://fba.tian-w.cn

JS:   s.split("a").length - 1
来源：http://zxg.vqdsnc.cn

TS:   s.split("a").length - 1
来源：http://inv.yj202588.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wyh.sjlbkw.cn

Go:   strings.Count(s, "a")
来源：http://xtc.shanyushiyangtech.top

Ruby: s.count("a")
来源：http://pss.shanyushiyangtech.top

C#:   s.Count(c => c == 'a')
来源：http://lhj.xuanzx.com

[E13] 逐字符遍历
来源：http://nql.jqgfzy.top

Py:   for ch in s: print(ch)
来源：http://wqz.wangshuangyany.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jvp.zdbjq.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://eec.gotoacloud.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://mxh.zdbjq.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wqe.svipenyu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://goy.yfazqb.com

Ruby: s.each_char { |ch| puts ch }
来源：http://tjp.xziqi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pfa.vqdsnc.cn

[E14] URL 编码与 Base64
来源：http://kcg.hnqzz.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vcf.fktsv.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://edn.redwolf501.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zzq.jlsjyb.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jbs.jqgfzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://svo.feifeiyinyue.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bhc.haohaochexian.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://txs.uphjek.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qgd.tian-w.cn

[E15] HTML 转义 / 反转义
来源：http://nsb.cucudq.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ixm.shangyingyoupin.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://akb.shangyingyoupin.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lax.ivvv.top

TS:   // 同上，务必做 XSS 过滤
来源：http://qod.jinghuilouyu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ryd.tian-w.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://iro.ehwqpu.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xdh.zhijiandao.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xvn.cqqwz.cn

[E16] 数字千分位
来源：http://pkz.daxiang520.top

Py:   f"{1234567:,}"
来源：http://nqy.zhiwuduotai.top

PHP:  number_format(1234567);
来源：http://cmi.zhongyouzk.top

JS:   (1234567).toLocaleString("en-US")
来源：http://jsd.fanxiaobao.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://txa.cashguo.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fam.yuanzhike.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://soi.ydjk.org.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jss.hesvh.cn

C#:   1234567.ToString("N0")
来源：http://bvb.smart0.xyz

[E17] 首字母大写
来源：http://qdi.hongshengwenyu.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kpm.chenlongwang.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://uhf.chenzaomai.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gkk.ybcxt.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fhz.yueranfly.top


<!-- 参考信息 -->