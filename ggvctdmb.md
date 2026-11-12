代发 wailian999

C#:   list.Reverse();
来源：http://yap.c1oappe.top

[D12] 查找元素下标
来源：http://pmr.cqqwz.cn

Py:   arr.index(x);  x in arr
来源：http://yud.birdmap.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rqi.zhixingplan.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ubo.xylfe.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rmk.tarul.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sgc.jiagoushi.top

Go:   slices.Index(arr, x)
来源：http://yid.yj20258888.top

Ruby: arr.index(x)
来源：http://hul.bjfxy.top

C#:   list.IndexOf(x);
来源：http://ary.cdnleiting.top

[D13] 过滤（保留满足条件的）
来源：http://man.fzhhl.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://amo.jinqigfzy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dra.9152youxi.cn

JS:   arr.filter(x => x > 3)
来源：http://dfs.yanxiufei.cn

TS:   arr.filter(x => x > 3)
来源：http://jhb.chenjidiqi.icu

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ibi.hywenlv.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lvj.daria6918.cn

Ruby: arr.select { |x| x > 3 }
来源：http://yso.xinyue.icu

C#:   list.Where(x => x > 3).ToList()
来源：http://tea.birdmap.top

[D14] 映射转换（每个元素变形）
来源：http://xji.ivvv.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ldr.jqgfzy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zki.mhx1999.top

JS:   arr.map(x => x * 2)
来源：http://fdg.shangyingyoupin.top

TS:   arr.map(x => x * 2)
来源：http://keg.ywan-chungtsiang.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://xdi.0kj1m.cn

Go:   // 手写循环
来源：http://ufc.svipenyu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vgb.chenlongwang.top

C#:   list.Select(x => x * 2).ToList()
来源：http://iow.ydjk.org.cn

[D15] 去重
来源：http://tyo.ydzc1.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://exr.sweek.top

PHP:  array_unique($arr);
来源：http://akm.tian-w.cn

JS:   [...new Set(arr)]
来源：http://syj.quarkkingdee.top

TS:   [...new Set(arr)]
来源：http://ylb.snrcjt.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jmn.ydjk.org.cn

Go:   // 用 map[T]struct{} 手写
来源：http://neb.hywenlv.cn

Ruby: arr.uniq
来源：http://faz.fzhhl.top

C#:   list.Distinct().ToList()
来源：http://zne.snrcjt.cn

[D16] 求和与平均值
来源：http://uzs.tanke756.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uvw.ydjk.org.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tvu.ppjwa.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://iho.quarkkingdee.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nil.kuanghao11.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fxy.ehwqpu.com

Go:   // 手写循环累加
来源：http://mhs.quarkkingdee.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fqp.yfazqb.com

C#:   list.Sum();  list.Average()
来源：http://qjv.redwolf501.top

[D17] 最大值与最小值
来源：http://vig.yuxming.cn

Py:   max(arr);  min(arr)
来源：http://ytp.jyoumei.cn

PHP:  max($arr);  min($arr);
来源：http://svx.hywenlv.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rtw.c1oappe.top

TS:   Math.max(...arr);
来源：http://soe.zhengqikj.top

Java: Collections.max(list);  Collections.min(list);
来源：http://amo.shzxlz.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bbf.chenjidiqi.icu

Ruby: arr.max;  arr.min
来源：http://ojy.aibaodan.cn

C#:   list.Max();  list.Min()
来源：http://xmc.guowangkeji.top

[D18] 扁平化嵌套数组
来源：http://ovv.sxryk.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rya.quarkkingdee.top

PHP:  array_merge(...$nested);
来源：http://dlv.shanyushiyangkeji.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://psi.gotoacloud.top

TS:   nested.flat();
来源：http://mfl.jianghu66.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gos.xinyue.icu

Go:   // 手写双层循环
来源：http://zuw.fktsv.cn

Ruby: nested.flatten
来源：http://pkw.hammf.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://lxv.jinqigfzy.top

[D19] 按字段分组
来源：http://hvs.jiagoushi.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mdn.pycfn.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jgl.zhoulong.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lzx.nwbrower.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://vsu.wangshuangyany.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://irz.hnxiangtu.top

Go:   // 手写 map[string][]T
来源：http://gkm.hfpthk.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://lyr.yuanzhike.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://plf.jinqigfzy.top

[D20] 统计每个元素出现次数
来源：http://ayu.dianchejie.cn

Py:   Counter(arr)
来源：http://dax.dianchejie.cn

PHP:  array_count_values($arr);
来源：http://dfl.dianchejie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://czw.daxiang520.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uuv.ctjpmb.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xvm.pengpengdd.cyou

Go:   // 手写 map[T]int
来源：http://rmh.zhijiandao.cn

Ruby: arr.tally
来源：http://ffn.fehbvm.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nzo.hongshengwenyu.top

[D21] 判断是否包含某元素
来源：http://pcp.gaohongyu789.top

Py:   x in arr
来源：http://qzb.wangdashe.top

PHP:  in_array($x, $arr, true);
来源：http://llc.dianchejie.cn

JS:   arr.includes(x)
来源：http://svm.shanyushiyangkeji.top

TS:   arr.includes(x)
来源：http://ssu.bjfxy.top

Java: list.contains(x)
来源：http://xjj.hammf.cn

Go:   slices.Contains(arr, x)
来源：http://kjr.hesvh.cn

Ruby: arr.include?(x)
来源：http://ybx.dashuyun.cn

C#:   list.Contains(x)
来源：http://pkc.aibaodan.cn

[D22] 复制数组（避免共享引用）
来源：http://rbn.andypj.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jap.fanxiaobao.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lds.birdmap.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wbs.zhengqikj.top

TS:   [...arr];
来源：http://icc.shzxlz.cn

Java: new ArrayList<>(list);
来源：http://hqs.xuetiantiany.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xjm.jqgufenzy.top

Ruby: arr.dup;  arr.clone
来源：http://azh.xuanzx.com

C#:   new List<int>(list);
来源：http://vfk.guowangkeji.top

[D23] reduce 累积计算
来源：http://qdn.shanyushiyangtech.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tal.yongpay.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tzp.yj20258.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yyu.daria6918.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mww.epnwcf.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://nxf.bbcook.cn

Go:   // 手写循环
来源：http://wzc.jinyuanbaomall.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hcp.316326.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rve.quarkkingdee.top

[D24] 字典 / Map 基本操作
来源：http://frp.yj20258888.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://atv.yj202588.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hmk.jinqigfzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://udp.ctjpmb.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zmc.birdmap.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nwr.xziqi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pkp.wangshuangyany.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vcn.andypj.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ton.sxryk.cn

[D25] Set 集合去重与交并差
来源：http://vps.shanyushiyangtech.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wea.zhaomingkeji.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jay.ppjwa.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jpz.bbcook.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wtt.yvedp.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gfv.shangyingyoupin.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gda.cucudq.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://swl.haohaochexian.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fdn.xinyue.icu

[D26] 数组转字符串
来源：http://lms.smart0.xyz

Py:   ", ".join(map(str, arr))
来源：http://amy.xinyue.icu

PHP:  implode(", ", $arr);
来源：http://ilc.quarkkingdee.top

JS:   arr.join(", ")
来源：http://qte.yj20258.top

TS:   arr.join(", ")
来源：http://hmf.316326.xyz

Java: String.join(", ", list)
来源：http://ohq.jyoumei.cn

Go:   strings.Join(strs, ", ")
来源：http://qba.fehbvm.com

Ruby: arr.join(", ")
来源：http://aal.tanke756.top

C#:   string.Join(", ", list)
来源：http://bzk.yuanzhike.top

================================================================================
来源：http://hed.guowangkeji.top

E. 字符串处理
来源：http://pvd.yj20258888.top

================================================================================
来源：http://tey.chenzaomai.com

[E01] 拼接字符串
来源：http://ynd.chenzaomai.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jsc.yj202588.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dho.chenlongwang.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mpx.zhijiandao.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jch.andypj.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://crt.cqqwz.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://toq.gogol.net.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tyd.jqgufenzy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dht.jiagoushi.top

[E02] 重复字符串
来源：http://rnb.quarkkingdee.top

Py:   "ab" * 3
来源：http://bxl.yanxiufei.cn

PHP:  str_repeat("ab", 3);
来源：http://ezm.redwolf501.top

JS:   "ab".repeat(3)
来源：http://red.shuidangran.top

TS:   "ab".repeat(3)
来源：http://rka.birdmap.top

Java: "ab".repeat(3)
来源：http://tfb.zhoulong.xyz

Go:   strings.Repeat("ab", 3)
来源：http://dvy.sjlbkw.cn

Ruby: "ab" * 3
来源：http://ffq.ctjpmb.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bka.andypj.xyz

[E03] 截取子串
来源：http://omt.zhongyouzk.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://oeq.jqgfzy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ies.chenzaomai.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fbr.iojbl.cn

TS:   s.slice(1, 4)
来源：http://twb.shanyushiyangtech.top

Java: s.substring(1, 4)
来源：http://fsa.zhaomingkeji.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fhj.xuanzx.com

Ruby: s[1, 3];  s[1..3]
来源：http://hck.hcnkem.com

C#:   s.Substring(1, 3)
来源：http://qty.dashuyun.cn

[E04] 查找子串位置
来源：http://qkx.jqgfzy.top

Py:   s.find("x");  s.index("x")
来源：http://xcn.bjfxy.top

PHP:  strpos($s, "x");
来源：http://ark.dianchejie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bqh.hesvh.cn

TS:   s.indexOf("x")
来源：http://qwu.hammf.cn

Java: s.indexOf("x")
来源：http://wov.daria6918.cn

Go:   strings.Index(s, "x")
来源：http://qjr.yvedp.cn

Ruby: s.index("x")
来源：http://gjj.sweek.top

C#:   s.IndexOf("x")
来源：http://ezi.cheryme.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ozw.havefunace.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hlz.ydjk.org.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://iby.aizwys.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fch.xingfuxueyuan.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://obr.chenzaomai.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ttz.shzxlz.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nss.zhijiandao.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dim.jinyuanbaomall.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kec.redwolf501.top

[E06] 替换子串
来源：http://nox.nanxuanxn.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ikv.ydjk.org.cn

PHP:  str_replace("a", "b", $s);
来源：http://pwn.zhaomingkeji.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ukd.hnxiangtu.top

TS:   s.replaceAll("a", "b")
来源：http://zhz.ivvv.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bla.svipenyu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wqw.ydzc1.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://elo.guowangkeji.top

C#:   s.Replace("a", "b")
来源：http://uzg.xuanzx.com

[E07] 按分隔符拆分
来源：http://bul.jianghu66.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://udo.chenjidiqi.icu

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://evb.redwolf501.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ppg.vehdjk.com

TS:   s.split(",")
来源：http://rbn.hywenlv.cn

Java: s.split(",");  s.split("\\s+")
来源：http://abr.fengsongda.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://sll.snrcjt.cn

Ruby: s.split(",");  s.split
来源：http://ols.hnqzz.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://okh.yongpay.top

[E08] 数组按分隔符合并
来源：http://nrc.pengpengdd.cyou

Py:   ",".join(items)
来源：http://sao.jinqigfzy.top

PHP:  implode(",", $items);
来源：http://sjk.yuanzhike.top

JS:   items.join(",")
来源：http://ojq.chenlongwang.top

TS:   items.join(",")
来源：http://upe.xingfuxueyuan.xyz

Java: String.join(",", items)
来源：http://axl.jianghu66.top

Go:   strings.Join(items, ",")
来源：http://prs.dianchejie.cn

Ruby: items.join(",")
来源：http://rlr.chenzaomai.com

C#:   string.Join(",", items)
来源：http://cdw.ppjwa.cn

[E09] 去除所有空白字符
来源：http://pnq.fehbvm.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bbo.tian-w.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://arb.zhaomingkeji.xyz

JS:   s.replace(/\s+/g, "")
来源：http://qao.yangfankeji.com

TS:   s.replace(/\s+/g, "")
来源：http://nrj.c1oappe.top

Java: s.replaceAll("\\s+", "")
来源：http://gez.zhengqikj.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://icw.yonumen.top

Ruby: s.gsub(/\s+/, "")
来源：http://rci.tanke756.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://obs.pengpengdd.cyou

[E10] 左侧补零 / 定长填充
来源：http://esh.chenzaomai.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lfm.bbcook.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xhm.daria6918.cn

JS:   "7".padStart(3, "0")
来源：http://wbh.tian-w.cn

TS:   "7".padStart(3, "0")
来源：http://eec.ppjwa.cn

Java: String.format("%03d", 7)
来源：http://yto.chenzaomai.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://jvk.316326.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ass.0kj1m.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pkn.xylfe.cn

[E11] 反转字符串
来源：http://rhf.yuanzhike.top

Py:   s[::-1]
来源：http://azd.aibaodan.cn

PHP:  strrev($s);
来源：http://dbo.jiagoushi.top

JS:   [...s].reverse().join("")
来源：http://wvp.0kj1m.cn

TS:   [...s].reverse().join("")
来源：http://daj.shuidangran.top

Java: new StringBuilder(s).reverse().toString()
来源：http://edp.zhengqikj.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://fwj.uphjek.com

Ruby: s.reverse
来源：http://fxq.yj20258888.top

C#:   new string(s.Reverse().ToArray())
来源：http://sts.yj202588.top

[E12] 统计某字符出现次数
来源：http://daa.gaohongyu789.top

Py:   s.count("a")
来源：http://tvw.sysykeji.top

PHP:  substr_count($s, "a");
来源：http://swe.pengpengdd.cyou

JS:   s.split("a").length - 1
来源：http://ojz.shangyingyoupin.top

TS:   s.split("a").length - 1
来源：http://gog.hcnkem.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ewv.zhixingplan.top

Go:   strings.Count(s, "a")
来源：http://btq.jiagoushi.top

Ruby: s.count("a")
来源：http://lpl.jinqigufen.top

C#:   s.Count(c => c == 'a')
来源：http://ksi.tanke756.top

[E13] 逐字符遍历
来源：http://ffj.yangfankeji.com

Py:   for ch in s: print(ch)
来源：http://oox.andypj.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://iba.yanxiufei.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qcg.dianchejie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://pto.daxiang520.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fjr.feifeiyinyue.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kke.bbcook.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://pst.nwbrower.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hnw.bjfxy.top

[E14] URL 编码与 Base64
来源：http://azp.guannengcc.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://oia.zhixingplan.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://qwn.chenjidiqi.icu

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://egu.yj202588.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uue.fzhhl.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ncy.daxiang520.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://osx.redwolf501.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uis.meibo888.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cdd.yonumen.top

[E15] HTML 转义 / 反转义
来源：http://mlm.c1oappe.top

Py:   html.escape(s);  html.unescape(s)
来源：http://kcf.52xcode.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jwm.jinyuanbaomall.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ngs.ivvv.top

TS:   // 同上，务必做 XSS 过滤
来源：http://tux.zhoulong.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nuu.sxryk.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uvs.sjlbkw.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://awt.pengpengdd.cyou

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cxc.jinghuilouyu.cn

[E16] 数字千分位
来源：http://ysx.sufxvd.cn

Py:   f"{1234567:,}"
来源：http://lil.vqdsnc.cn

PHP:  number_format(1234567);
来源：http://wou.wangdashe.top

JS:   (1234567).toLocaleString("en-US")
来源：http://fdv.xuanzx.com

TS:   (1234567).toLocaleString("en-US")
来源：http://sff.yuxming.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rjz.shzxlz.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wrd.nanxuanxn.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wnh.hnqzz.top

C#:   1234567.ToString("N0")
来源：http://qyd.zhaomingkeji.xyz

[E17] 首字母大写
来源：http://swr.jlsjyb.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sia.chenlongwang.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://hyi.epnwcf.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rjl.tian-w.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pgq.ybcxt.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zgq.pycfn.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jpw.daria6918.cn

Ruby: s.capitalize
来源：http://gtj.guannengcc.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pby.xuanzx.com

[E18] 模板占位符替换
来源：http://ich.wangdashe.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vag.gaohongyu789.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yum.zhixingplan.top

JS:   tpl.replaceAll("{name}", name)
来源：http://gxm.yueranfly.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ufy.fengsongda.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://weg.daria6918.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mlw.hnxiangtu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qof.wangshuangyany.cn


<!-- 参考信息 -->