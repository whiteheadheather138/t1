代发 wailian999

TS:   [...arr].reverse();
来源：http://sac.tanke756.top

Java: Collections.reverse(list);
来源：http://pay.epnwcf.com

Go:   slices.Reverse(arr)
来源：http://tok.cashguo.top

Ruby: arr.reverse
来源：http://gfg.sxryk.cn

C#:   list.Reverse();
来源：http://fwh.xingfuxueyuan.xyz

[D12] 查找元素下标
来源：http://ejf.jiagoushi.top

Py:   arr.index(x);  x in arr
来源：http://juk.snrcjt.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pwl.fanxiaobao.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rmp.yanxiufei.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nkd.xziqi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mnv.hnqzz.top

Go:   slices.Index(arr, x)
来源：http://cxr.xingfuxueyuan.xyz

Ruby: arr.index(x)
来源：http://nbe.epnwcf.com

C#:   list.IndexOf(x);
来源：http://clb.vqdsnc.cn

[D13] 过滤（保留满足条件的）
来源：http://uwv.shangyingyoupin.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zkt.gzhubu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://etk.vehdjk.com

JS:   arr.filter(x => x > 3)
来源：http://vri.ybcxt.top

TS:   arr.filter(x => x > 3)
来源：http://ttn.daria6918.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bpk.pengpengdd.cyou

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ltg.tian-w.cn

Ruby: arr.select { |x| x > 3 }
来源：http://zta.jianghu66.top

C#:   list.Where(x => x > 3).ToList()
来源：http://cyl.shangyingyoupin.top

[D14] 映射转换（每个元素变形）
来源：http://yob.yongpay.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lnu.zhengqikj.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tcc.shzxlz.cn

JS:   arr.map(x => x * 2)
来源：http://gbk.aizwys.cn

TS:   arr.map(x => x * 2)
来源：http://kvn.sxryk.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://kpb.hongshengwenyu.top

Go:   // 手写循环
来源：http://wik.epnwcf.com

Ruby: arr.map { |x| x * 2 }
来源：http://ngp.meibo888.top

C#:   list.Select(x => x * 2).ToList()
来源：http://mka.fktsv.cn

[D15] 去重
来源：http://hyd.epnwcf.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pww.tanke756.top

PHP:  array_unique($arr);
来源：http://pnr.yvedp.cn

JS:   [...new Set(arr)]
来源：http://hap.zdqjudy.top

TS:   [...new Set(arr)]
来源：http://plv.jyoumei.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hfi.uphjek.com

Go:   // 用 map[T]struct{} 手写
来源：http://flp.andypj.xyz

Ruby: arr.uniq
来源：http://toz.quarkkingdee.top

C#:   list.Distinct().ToList()
来源：http://mwz.vehdjk.com

[D16] 求和与平均值
来源：http://oos.vehdjk.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nvb.zhixingplan.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ebv.chenjidiqi.icu

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sqs.ydzc1.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bhv.shanyushiyangkeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://anw.andypj.xyz

Go:   // 手写循环累加
来源：http://mtg.shangyingyoupin.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cfu.jinghuilouyu.cn

C#:   list.Sum();  list.Average()
来源：http://gtd.hnxiangtu.top

[D17] 最大值与最小值
来源：http://rpc.yj20258.top

Py:   max(arr);  min(arr)
来源：http://xjh.sweek.top

PHP:  max($arr);  min($arr);
来源：http://hpl.ydzc1.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://aal.cashguo.top

TS:   Math.max(...arr);
来源：http://kkw.smart0.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://czi.guowangkeji.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hsr.ppjwa.cn

Ruby: arr.max;  arr.min
来源：http://zah.hnxiangtu.top

C#:   list.Max();  list.Min()
来源：http://fqg.fanxiaobao.xyz

[D18] 扁平化嵌套数组
来源：http://zdd.redwolf501.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xox.jinqigfzy.top

PHP:  array_merge(...$nested);
来源：http://acc.cashguo.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ehf.hnxiangtu.top

TS:   nested.flat();
来源：http://kww.havefunace.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cib.bjfxy.top

Go:   // 手写双层循环
来源：http://heo.pycfn.com

Ruby: nested.flatten
来源：http://zfp.gogol.net.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://afd.andypj.xyz

[D19] 按字段分组
来源：http://qrt.yj20258.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mxz.zhixingplan.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://sog.daxiang520.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rbl.ydjk.org.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://sja.hnqzz.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fic.sufxvd.cn

Go:   // 手写 map[string][]T
来源：http://cna.haohaochexian.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://egs.chenlongwang.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gog.redwolf501.top

[D20] 统计每个元素出现次数
来源：http://rlo.zhongyouzk.top

Py:   Counter(arr)
来源：http://vck.ybcxt.top

PHP:  array_count_values($arr);
来源：http://gcm.shanyushiyangtech.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pzr.yj20258.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bxj.ctjpmb.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gzn.nanxuanxn.top

Go:   // 手写 map[T]int
来源：http://mza.ydjk.org.cn

Ruby: arr.tally
来源：http://ghj.guannengcc.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://scm.xuanzx.com

[D21] 判断是否包含某元素
来源：http://lfa.gaohongyu789.top

Py:   x in arr
来源：http://sdb.xylfe.cn

PHP:  in_array($x, $arr, true);
来源：http://oxh.zhongyouzk.top

JS:   arr.includes(x)
来源：http://wlp.daxiang520.top

TS:   arr.includes(x)
来源：http://ihq.yvedp.cn

Java: list.contains(x)
来源：http://hss.tianlin.xyz

Go:   slices.Contains(arr, x)
来源：http://owr.fzhhl.top

Ruby: arr.include?(x)
来源：http://ozk.cashguo.top

C#:   list.Contains(x)
来源：http://oyd.shangyingyoupin.top

[D22] 复制数组（避免共享引用）
来源：http://aqn.fehbvm.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sqe.tian-w.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pfq.meibo888.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ltx.nanxinkj.top

TS:   [...arr];
来源：http://cqw.yuanzhike.top

Java: new ArrayList<>(list);
来源：http://fdf.zhaomingkeji.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://axp.cucudq.cn

Ruby: arr.dup;  arr.clone
来源：http://rhv.yanxiufei.cn

C#:   new List<int>(list);
来源：http://gbs.zdbjq.cn

[D23] reduce 累积计算
来源：http://zan.bjfxy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://unu.birdmap.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ggx.yuanzhike.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rrd.fengsongda.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ptp.sjlbkw.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ncx.chenjidiqi.icu

Go:   // 手写循环
来源：http://jmw.dianchejie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dsg.chenzaomai.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mug.svipenyu.cn

[D24] 字典 / Map 基本操作
来源：http://fyb.316326.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xvf.gzhubu.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ytv.hesvh.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zzl.zycfv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://iah.0kj1m.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ofb.shzxlz.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://syh.fktsv.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vfb.uphjek.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://amn.zhixingplan.top

[D25] Set 集合去重与交并差
来源：http://bpb.jinyuanbaomall.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xzk.jinqigufen.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qvz.daria6918.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gfo.iojbl.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qhq.ppjwa.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zvo.gogol.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cjf.uphjek.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ruf.jiagoushi.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ppo.quarkkingdee.top

[D26] 数组转字符串
来源：http://rni.zhixingplan.top

Py:   ", ".join(map(str, arr))
来源：http://iko.ywan-chungtsiang.top

PHP:  implode(", ", $arr);
来源：http://ewx.daria6918.cn

JS:   arr.join(", ")
来源：http://hlu.fzhhl.top

TS:   arr.join(", ")
来源：http://ier.gaohongyu789.top

Java: String.join(", ", list)
来源：http://xwo.jqgufenzy.top

Go:   strings.Join(strs, ", ")
来源：http://ivz.smart0.xyz

Ruby: arr.join(", ")
来源：http://pgo.zhiwuduotai.top

C#:   string.Join(", ", list)
来源：http://gmn.yongpay.top

================================================================================
来源：http://ulg.cdnleiting.top

E. 字符串处理
来源：http://uoz.redwolf501.top

================================================================================
来源：http://lpq.shzxlz.cn

[E01] 拼接字符串
来源：http://oog.gogol.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fsb.chenjidiqi.icu

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xie.jianghu66.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vrs.yj20258888.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pwf.xuetiantiany.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dvx.yongpay.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mml.hcnkem.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://leb.yuxming.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zsu.quarkkingdee.top

[E02] 重复字符串
来源：http://mmd.fehbvm.com

Py:   "ab" * 3
来源：http://pgv.jiagoushi.top

PHP:  str_repeat("ab", 3);
来源：http://mts.jyoumei.cn

JS:   "ab".repeat(3)
来源：http://wwz.yj20258888.top

TS:   "ab".repeat(3)
来源：http://tds.0kj1m.cn

Java: "ab".repeat(3)
来源：http://ilx.epnwcf.com

Go:   strings.Repeat("ab", 3)
来源：http://amr.yanxiufei.cn

Ruby: "ab" * 3
来源：http://ncr.xingfuxueyuan.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ncb.c1oappe.top

[E03] 截取子串
来源：http://yzf.haohaochexian.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xxk.haohaochexian.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ixh.hywenlv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://spd.zhongyouzk.top

TS:   s.slice(1, 4)
来源：http://fzx.fanxiaobao.xyz

Java: s.substring(1, 4)
来源：http://gsz.yuxming.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://meg.zhengqikj.top

Ruby: s[1, 3];  s[1..3]
来源：http://cpd.meibo888.top

C#:   s.Substring(1, 3)
来源：http://cax.ivvv.top

[E04] 查找子串位置
来源：http://zkv.uphjek.com

Py:   s.find("x");  s.index("x")
来源：http://gpq.snrcjt.cn

PHP:  strpos($s, "x");
来源：http://pta.shanyushiyangkeji.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dcq.shuidangran.top

TS:   s.indexOf("x")
来源：http://eqx.gaohongyu789.top

Java: s.indexOf("x")
来源：http://elf.sjlbkw.cn

Go:   strings.Index(s, "x")
来源：http://srf.shanyushiyangtech.top

Ruby: s.index("x")
来源：http://udy.hnxiangtu.top

C#:   s.IndexOf("x")
来源：http://kyd.shanyushiyangtech.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://hch.guowangkeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gse.yuxming.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ykb.jinghuilouyu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://eth.yonumen.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://urv.gzhubu.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ftx.xuanzx.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ccv.sufxvd.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kjt.aibaodan.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fgz.epnwcf.com

[E06] 替换子串
来源：http://ijm.smart0.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lyv.nwbrower.top

PHP:  str_replace("a", "b", $s);
来源：http://jjr.yj202588.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://omb.yfazqb.com

TS:   s.replaceAll("a", "b")
来源：http://nsr.dashuyun.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://skq.shuidangran.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mqv.xylfe.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bwg.zycfv.cn

C#:   s.Replace("a", "b")
来源：http://drz.jinqigfzy.top

[E07] 按分隔符拆分
来源：http://oki.zhoulong.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://err.dianchejie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rev.hfpthk.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://niv.c1oappe.top

TS:   s.split(",")
来源：http://uwc.uphjek.com

Java: s.split(",");  s.split("\\s+")
来源：http://tor.redwolf501.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xae.ybcxt.top

Ruby: s.split(",");  s.split
来源：http://ltq.jinqigfzy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fna.daxiang520.top

[E08] 数组按分隔符合并
来源：http://soq.hcnkem.com

Py:   ",".join(items)
来源：http://ugq.yuxming.cn

PHP:  implode(",", $items);
来源：http://lhr.cucudq.cn

JS:   items.join(",")
来源：http://sja.tanke756.top

TS:   items.join(",")
来源：http://gsx.sjlbkw.cn

Java: String.join(",", items)
来源：http://zpy.yj202588.top

Go:   strings.Join(items, ",")
来源：http://jce.tian-w.cn

Ruby: items.join(",")
来源：http://tgq.mhx1999.top

C#:   string.Join(",", items)
来源：http://rhf.nanxinkj.top

[E09] 去除所有空白字符
来源：http://lbg.chenjidiqi.icu

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://udb.shangyingyoupin.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://quu.xinyue.icu

JS:   s.replace(/\s+/g, "")
来源：http://sey.sysykeji.top

TS:   s.replace(/\s+/g, "")
来源：http://knu.hywenlv.cn

Java: s.replaceAll("\\s+", "")
来源：http://exl.zhijiandao.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://eyv.nanxuanxn.top

Ruby: s.gsub(/\s+/, "")
来源：http://fva.dianchejie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://quo.cqqwz.cn

[E10] 左侧补零 / 定长填充
来源：http://jwr.yonumen.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nuu.shanyushiyangtech.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rze.jianghu66.top

JS:   "7".padStart(3, "0")
来源：http://tku.haohaochexian.top

TS:   "7".padStart(3, "0")
来源：http://gtl.ywan-chungtsiang.top

Java: String.format("%03d", 7)
来源：http://xlx.hesvh.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ugb.ydzc1.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vbb.zycfv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rwq.hysaishi.cn

[E11] 反转字符串
来源：http://ptf.andypj.xyz

Py:   s[::-1]
来源：http://xoz.ydjk.org.cn

PHP:  strrev($s);
来源：http://wuy.aibaodan.cn

JS:   [...s].reverse().join("")
来源：http://abo.dashuyun.cn

TS:   [...s].reverse().join("")
来源：http://isc.hfpthk.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://sjv.zhengqikj.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://goj.dianchejie.cn

Ruby: s.reverse
来源：http://emf.dianchejie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wuk.chenzaomai.com

[E12] 统计某字符出现次数
来源：http://snl.jinghuilouyu.cn

Py:   s.count("a")
来源：http://nia.guannengcc.top

PHP:  substr_count($s, "a");
来源：http://iay.bbcook.cn

JS:   s.split("a").length - 1
来源：http://agt.zycfv.cn

TS:   s.split("a").length - 1
来源：http://pas.shuidangran.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://emb.zhijiandao.cn

Go:   strings.Count(s, "a")
来源：http://qam.meibo888.top

Ruby: s.count("a")
来源：http://ijn.chenjidiqi.icu

C#:   s.Count(c => c == 'a')
来源：http://xwc.fanxiaobao.xyz

[E13] 逐字符遍历
来源：http://tlg.cqqwz.cn

Py:   for ch in s: print(ch)
来源：http://alc.zhijiandao.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tav.sufxvd.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ooa.dianchejie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://piz.iojbl.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ylc.jinqigufen.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://neq.redwolf501.top

Ruby: s.each_char { |ch| puts ch }
来源：http://yxb.vqdsnc.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://muo.pycfn.com

[E14] URL 编码与 Base64
来源：http://bul.tarul.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qxi.hywenlv.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zlj.jinqigfzy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ork.snrcjt.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://htq.hesvh.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tmf.dianchejie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uhp.c1oappe.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vix.jinqigufen.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://quo.gotoacloud.top

[E15] HTML 转义 / 反转义
来源：http://anf.nanxinkj.top

Py:   html.escape(s);  html.unescape(s)
来源：http://axw.xziqi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uvc.tanke756.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hcr.shanyushiyangtech.top

TS:   // 同上，务必做 XSS 过滤
来源：http://idw.jlsjyb.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kbw.gzhubu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pos.bbcook.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://udg.hnxiangtu.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zzn.shanyushiyangkeji.top

[E16] 数字千分位
来源：http://lpi.tian-w.cn

Py:   f"{1234567:,}"
来源：http://ixy.sufxvd.cn

PHP:  number_format(1234567);
来源：http://rxo.xinyue.icu

JS:   (1234567).toLocaleString("en-US")
来源：http://vpg.vqdsnc.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ykl.daxiang520.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://scx.daria6918.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jbf.sysykeji.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tmk.jinghuilouyu.cn

C#:   1234567.ToString("N0")
来源：http://sbf.kuanghao11.cn

[E17] 首字母大写
来源：http://tlq.52xcode.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kfr.cucudq.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ctw.xingfuxueyuan.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uuf.cqqwz.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://van.zycfv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kke.zhengqikj.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fcy.jinqigufen.top

Ruby: s.capitalize
来源：http://pxo.meibo888.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qsy.ywan-chungtsiang.top

[E18] 模板占位符替换
来源：http://tdc.ywan-chungtsiang.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hww.316326.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://phk.daxiang520.top

JS:   tpl.replaceAll("{name}", name)
来源：http://fds.zycfv.cn


<!-- 参考信息 -->