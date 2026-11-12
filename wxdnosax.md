代发 wailian999

C#:   list.Reverse();
来源：http://gkx.svipenyu.cn

[D12] 查找元素下标
来源：http://sha.fanxiaobao.xyz

Py:   arr.index(x);  x in arr
来源：http://crr.sysykeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://whf.xingfuxueyuan.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nwq.yanxiufei.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dxb.jqgfzy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kln.daxiang520.top

Go:   slices.Index(arr, x)
来源：http://pso.havefunace.top

Ruby: arr.index(x)
来源：http://evq.tian-w.cn

C#:   list.IndexOf(x);
来源：http://djm.cqqwz.cn

[D13] 过滤（保留满足条件的）
来源：http://mln.zycfv.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tlr.yongpay.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wkq.shuidangran.top

JS:   arr.filter(x => x > 3)
来源：http://wzm.ppjwa.cn

TS:   arr.filter(x => x > 3)
来源：http://yyz.zhongyouzk.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zro.guannengcc.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bpc.tarul.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jts.aibaodan.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wyh.shuidangran.top

[D14] 映射转换（每个元素变形）
来源：http://uic.yj20258.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bbt.sufxvd.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zyu.cdnleiting.top

JS:   arr.map(x => x * 2)
来源：http://ayc.haohaochexian.top

TS:   arr.map(x => x * 2)
来源：http://raq.guannengcc.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://cqx.ivvv.top

Go:   // 手写循环
来源：http://xwo.zhijiandao.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lit.jqgfzy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://gvo.xylfe.cn

[D15] 去重
来源：http://owp.hnqzz.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pru.gzhubu.top

PHP:  array_unique($arr);
来源：http://bqo.chenjidiqi.icu

JS:   [...new Set(arr)]
来源：http://sel.yj20258.top

TS:   [...new Set(arr)]
来源：http://saa.havefunace.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xtg.jlsjyb.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vjk.sweek.top

Ruby: arr.uniq
来源：http://dfu.yj20258888.top

C#:   list.Distinct().ToList()
来源：http://vtm.hnxiangtu.top

[D16] 求和与平均值
来源：http://rje.zycfv.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hsi.pengpengdd.cyou

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qdc.jlsjyb.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://igw.fehbvm.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ciq.hysaishi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://glr.fehbvm.com

Go:   // 手写循环累加
来源：http://gxn.fengsongda.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rrd.ywan-chungtsiang.top

C#:   list.Sum();  list.Average()
来源：http://obc.iojbl.cn

[D17] 最大值与最小值
来源：http://suv.chenzaomai.com

Py:   max(arr);  min(arr)
来源：http://uru.yj20258.top

PHP:  max($arr);  min($arr);
来源：http://jfg.hywenlv.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://peo.yueranfly.top

TS:   Math.max(...arr);
来源：http://yif.gaohongyu789.top

Java: Collections.max(list);  Collections.min(list);
来源：http://coi.havefunace.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hxs.epnwcf.com

Ruby: arr.max;  arr.min
来源：http://usl.zdbjq.cn

C#:   list.Max();  list.Min()
来源：http://jpw.hnxiangtu.top

[D18] 扁平化嵌套数组
来源：http://afs.dashuyun.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mxo.gzhubu.top

PHP:  array_merge(...$nested);
来源：http://cef.birdmap.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wet.bjfxy.top

TS:   nested.flat();
来源：http://tap.yuanzhike.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://arw.shzxlz.cn

Go:   // 手写双层循环
来源：http://acr.cdnleiting.top

Ruby: nested.flatten
来源：http://qym.yvedp.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://erk.yvedp.cn

[D19] 按字段分组
来源：http://qae.yfazqb.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mxg.guowangkeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ynf.ppjwa.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fkl.52xcode.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yut.aibaodan.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hzf.nwbrower.top

Go:   // 手写 map[string][]T
来源：http://prc.xylfe.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://dqu.epnwcf.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yzg.chenzaomai.com

[D20] 统计每个元素出现次数
来源：http://otv.zdqjudy.top

Py:   Counter(arr)
来源：http://iih.hfpthk.cn

PHP:  array_count_values($arr);
来源：http://bsc.aibaodan.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kac.yvedp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cok.nanxinkj.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zcd.iojbl.cn

Go:   // 手写 map[T]int
来源：http://yjd.jinyuanbaomall.cn

Ruby: arr.tally
来源：http://pwe.cheryme.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xeg.fanxiaobao.xyz

[D21] 判断是否包含某元素
来源：http://xyp.cucudq.cn

Py:   x in arr
来源：http://hsa.birdmap.top

PHP:  in_array($x, $arr, true);
来源：http://gzz.yuanzhike.top

JS:   arr.includes(x)
来源：http://ado.zhiwuduotai.top

TS:   arr.includes(x)
来源：http://onz.ybcxt.top

Java: list.contains(x)
来源：http://rns.jqgufenzy.top

Go:   slices.Contains(arr, x)
来源：http://wrk.yvedp.cn

Ruby: arr.include?(x)
来源：http://kbv.fengsongda.top

C#:   list.Contains(x)
来源：http://wko.tarul.cn

[D22] 复制数组（避免共享引用）
来源：http://cln.fehbvm.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fif.ehwqpu.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vrc.ydzc1.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vfv.fzhhl.top

TS:   [...arr];
来源：http://vjg.jinghuilouyu.cn

Java: new ArrayList<>(list);
来源：http://rna.zhengqikj.top

Go:   copied := append([]int(nil), arr...)
来源：http://rhn.sweek.top

Ruby: arr.dup;  arr.clone
来源：http://qdz.aizwys.cn

C#:   new List<int>(list);
来源：http://gvj.aizwys.cn

[D23] reduce 累积计算
来源：http://eep.yueranfly.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://des.9152youxi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dwr.zhixingplan.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mfc.guowangkeji.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dpg.shuidangran.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://cbi.gzhubu.top

Go:   // 手写循环
来源：http://bzu.ybcxt.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qjr.gzhubu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zky.bbcook.cn

[D24] 字典 / Map 基本操作
来源：http://iwk.snrcjt.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zcc.yvedp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wme.kuanghao11.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hps.tanke756.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://isw.hysaishi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dum.quarkkingdee.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jlu.jinghuilouyu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://oet.tianlin.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rpc.yuanzhike.top

[D25] Set 集合去重与交并差
来源：http://dpy.zhixingplan.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vqs.birdmap.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pqr.yanxiufei.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jce.jianghu66.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yrf.yanxiufei.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ivr.jinqigufen.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fqz.jqgfzy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lqo.fktsv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hxe.chenjidiqi.icu

[D26] 数组转字符串
来源：http://aox.jiagoushi.top

Py:   ", ".join(map(str, arr))
来源：http://wnl.zdqjudy.top

PHP:  implode(", ", $arr);
来源：http://xoe.ybcxt.top

JS:   arr.join(", ")
来源：http://mxe.nanxuanxn.top

TS:   arr.join(", ")
来源：http://vgi.jinqigufen.top

Java: String.join(", ", list)
来源：http://pyh.tian-w.cn

Go:   strings.Join(strs, ", ")
来源：http://mio.vehdjk.com

Ruby: arr.join(", ")
来源：http://njq.andypj.xyz

C#:   string.Join(", ", list)
来源：http://nwe.fengsongda.top

================================================================================
来源：http://fhj.hnxiangtu.top

E. 字符串处理
来源：http://qpr.zdbjq.cn

================================================================================
来源：http://jft.hesvh.cn

[E01] 拼接字符串
来源：http://hlw.zycfv.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hij.snrcjt.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gnk.xingfuxueyuan.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tvp.jinqigfzy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pjm.redwolf501.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kxn.cheryme.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dqd.zhijiandao.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mku.yangfankeji.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://prs.jiagoushi.top

[E02] 重复字符串
来源：http://sea.jqgfzy.top

Py:   "ab" * 3
来源：http://alv.ydjk.org.cn

PHP:  str_repeat("ab", 3);
来源：http://rzb.kuanghao11.cn

JS:   "ab".repeat(3)
来源：http://shz.iojbl.cn

TS:   "ab".repeat(3)
来源：http://mtk.yonumen.top

Java: "ab".repeat(3)
来源：http://qib.sysykeji.top

Go:   strings.Repeat("ab", 3)
来源：http://vdl.hnqzz.top

Ruby: "ab" * 3
来源：http://ips.sxryk.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rul.sweek.top

[E03] 截取子串
来源：http://jit.jinqigfzy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xrr.316326.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pls.sufxvd.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zfx.sysykeji.top

TS:   s.slice(1, 4)
来源：http://upd.smart0.xyz

Java: s.substring(1, 4)
来源：http://wsh.sysykeji.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://oxe.cqqwz.cn

Ruby: s[1, 3];  s[1..3]
来源：http://lec.wangshuangyany.cn

C#:   s.Substring(1, 3)
来源：http://bko.cdnleiting.top

[E04] 查找子串位置
来源：http://kzl.c1oappe.top

Py:   s.find("x");  s.index("x")
来源：http://bsy.xinyue.icu

PHP:  strpos($s, "x");
来源：http://wba.jlsjyb.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://auu.ywan-chungtsiang.top

TS:   s.indexOf("x")
来源：http://jhq.jiagoushi.top

Java: s.indexOf("x")
来源：http://jmz.ivvv.top

Go:   strings.Index(s, "x")
来源：http://cqg.zhoulong.xyz

Ruby: s.index("x")
来源：http://zrp.ydzc1.top

C#:   s.IndexOf("x")
来源：http://cfu.aibaodan.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://suo.yfazqb.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yub.chenlongwang.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tsz.nwbrower.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bfq.gaohongyu789.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://lxk.ppjwa.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mma.ybcxt.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mfm.zdbjq.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tkn.haohaochexian.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mhu.zhiwuduotai.top

[E06] 替换子串
来源：http://vsv.wangshuangyany.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://aoj.kuanghao11.cn

PHP:  str_replace("a", "b", $s);
来源：http://ial.nwbrower.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sez.smart0.xyz

TS:   s.replaceAll("a", "b")
来源：http://zjj.xinyue.icu

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ptv.meibo888.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hde.yfazqb.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jma.cucudq.cn

C#:   s.Replace("a", "b")
来源：http://xjs.hammf.cn

[E07] 按分隔符拆分
来源：http://ztf.zhijiandao.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qkc.nwbrower.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ouc.gzhubu.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://nnh.ydjk.org.cn

TS:   s.split(",")
来源：http://fpt.haohaochexian.top

Java: s.split(",");  s.split("\\s+")
来源：http://dtd.ctjpmb.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bco.ydzc1.top

Ruby: s.split(",");  s.split
来源：http://nxx.hnqzz.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kpe.bbcook.cn

[E08] 数组按分隔符合并
来源：http://dsr.svipenyu.cn

Py:   ",".join(items)
来源：http://tvk.haohaochexian.top

PHP:  implode(",", $items);
来源：http://wyj.jlsjyb.cn

JS:   items.join(",")
来源：http://gaj.wangshuangyany.cn

TS:   items.join(",")
来源：http://vqh.epnwcf.com

Java: String.join(",", items)
来源：http://sss.cashguo.top

Go:   strings.Join(items, ",")
来源：http://ewu.zhoulong.xyz

Ruby: items.join(",")
来源：http://jyp.zdbjq.cn

C#:   string.Join(",", items)
来源：http://sgr.chenlongwang.top

[E09] 去除所有空白字符
来源：http://vxm.ydzc1.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fcq.yfazqb.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tcq.yj202588.top

JS:   s.replace(/\s+/g, "")
来源：http://ylh.hammf.cn

TS:   s.replace(/\s+/g, "")
来源：http://nky.9152youxi.cn

Java: s.replaceAll("\\s+", "")
来源：http://ztp.pengpengdd.cyou

Go:   strings.Join(strings.Fields(s), "")
来源：http://fjy.xinyue.icu

Ruby: s.gsub(/\s+/, "")
来源：http://uio.hcnkem.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mse.pengpengdd.cyou

[E10] 左侧补零 / 定长填充
来源：http://svt.xziqi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://agu.haohaochexian.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hjz.hongshengwenyu.top

JS:   "7".padStart(3, "0")
来源：http://rrm.cucudq.cn

TS:   "7".padStart(3, "0")
来源：http://rjw.feifeiyinyue.top

Java: String.format("%03d", 7)
来源：http://mmh.jqgfzy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://cpg.jinqigufen.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://adf.shanyushiyangkeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ulm.sweek.top

[E11] 反转字符串
来源：http://csw.hammf.cn

Py:   s[::-1]
来源：http://oas.zdqjudy.top

PHP:  strrev($s);
来源：http://nmm.cheryme.top

JS:   [...s].reverse().join("")
来源：http://nkj.epnwcf.com

TS:   [...s].reverse().join("")
来源：http://sav.nanxuanxn.top

Java: new StringBuilder(s).reverse().toString()
来源：http://qif.0kj1m.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ilt.ybcxt.top

Ruby: s.reverse
来源：http://xle.bbcook.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xtj.ydjk.org.cn

[E12] 统计某字符出现次数
来源：http://rss.yueranfly.top

Py:   s.count("a")
来源：http://pio.quarkkingdee.top

PHP:  substr_count($s, "a");
来源：http://daz.zdqjudy.top

JS:   s.split("a").length - 1
来源：http://tmf.sweek.top

TS:   s.split("a").length - 1
来源：http://naw.hfpthk.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ris.jinghuilouyu.cn

Go:   strings.Count(s, "a")
来源：http://bxk.haohaochexian.top

Ruby: s.count("a")
来源：http://grv.vehdjk.com

C#:   s.Count(c => c == 'a')
来源：http://gbo.cqqwz.cn

[E13] 逐字符遍历
来源：http://uda.yuxming.cn

Py:   for ch in s: print(ch)
来源：http://zdz.guannengcc.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://owx.yfazqb.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://lpt.sysykeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://hby.bbcook.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rag.hammf.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dac.fanxiaobao.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://lkv.uphjek.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jpb.vehdjk.com

[E14] URL 编码与 Base64
来源：http://azf.haohaochexian.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://oeq.guannengcc.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://uiu.yangfankeji.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://flf.fehbvm.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tzd.nanxinkj.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://flz.ydjk.org.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gqz.yj202588.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yue.vqdsnc.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zwx.jqgfzy.top

[E15] HTML 转义 / 反转义
来源：http://ydw.0kj1m.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://qvb.haohaochexian.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vhk.c1oappe.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kar.chenlongwang.top

TS:   // 同上，务必做 XSS 过滤
来源：http://mlf.bjfxy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pgy.kuanghao11.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gjp.tarul.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ojn.andypj.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nlt.tanke756.top

[E16] 数字千分位
来源：http://bsa.yuxming.cn

Py:   f"{1234567:,}"
来源：http://aai.jiagoushi.top

PHP:  number_format(1234567);
来源：http://kxh.yj20258.top

JS:   (1234567).toLocaleString("en-US")
来源：http://yqk.cucudq.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fgp.fehbvm.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tfo.smart0.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wza.fzhhl.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://opm.iojbl.cn

C#:   1234567.ToString("N0")
来源：http://tup.jinyuanbaomall.cn

[E17] 首字母大写
来源：http://qsf.xingfuxueyuan.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://axd.mhx1999.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://hln.zhijiandao.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qpr.ydjk.org.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cxu.fktsv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uok.316326.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bln.nanxuanxn.top

Ruby: s.capitalize
来源：http://xbs.birdmap.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://srw.iojbl.cn

[E18] 模板占位符替换
来源：http://dfy.zdqjudy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lch.bjfxy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mzw.wangshuangyany.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://nyk.yvedp.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://adq.zhixingplan.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jmx.xziqi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xff.chenjidiqi.icu

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vha.hcnkem.com


<!-- 参考信息 -->