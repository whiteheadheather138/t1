代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bib.jiagoushi.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rzu.ivvv.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uth.hysaishi.cn

Go:   slices.Index(arr, x)
来源：http://ssp.fehbvm.com

Ruby: arr.index(x)
来源：http://frq.jianghu66.top

C#:   list.IndexOf(x);
来源：http://lnb.yanxiufei.cn

[D13] 过滤（保留满足条件的）
来源：http://tna.nanxinkj.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yvx.hongshengwenyu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xqc.shanyushiyangkeji.top

JS:   arr.filter(x => x > 3)
来源：http://agk.xingfuxueyuan.xyz

TS:   arr.filter(x => x > 3)
来源：http://hle.zhongyouzk.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ojq.yonumen.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://suc.chenjidiqi.icu

Ruby: arr.select { |x| x > 3 }
来源：http://gaw.yuxming.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://xkr.nanxinkj.top

[D14] 映射转换（每个元素变形）
来源：http://nxz.hcnkem.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://etv.aizwys.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xjs.kuanghao11.cn

JS:   arr.map(x => x * 2)
来源：http://hlc.xylfe.cn

TS:   arr.map(x => x * 2)
来源：http://ybv.zhongyouzk.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://fah.fzhhl.top

Go:   // 手写循环
来源：http://bdb.zhijiandao.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jgc.hywenlv.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vba.yongpay.top

[D15] 去重
来源：http://inx.shzxlz.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qcr.chenzaomai.com

PHP:  array_unique($arr);
来源：http://rvy.hnqzz.top

JS:   [...new Set(arr)]
来源：http://sfs.ybcxt.top

TS:   [...new Set(arr)]
来源：http://fzn.guowangkeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://eao.yuxming.cn

Go:   // 用 map[T]struct{} 手写
来源：http://uqg.sysykeji.top

Ruby: arr.uniq
来源：http://ktr.zycfv.cn

C#:   list.Distinct().ToList()
来源：http://fdw.wangdashe.top

[D16] 求和与平均值
来源：http://kfy.jiagoushi.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jhg.ywan-chungtsiang.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://huc.cheryme.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kvf.smart0.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ylh.daxiang520.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mog.cucudq.cn

Go:   // 手写循环累加
来源：http://lme.chenjidiqi.icu

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lub.daria6918.cn

C#:   list.Sum();  list.Average()
来源：http://leo.jqgufenzy.top

[D17] 最大值与最小值
来源：http://xcv.gaohongyu789.top

Py:   max(arr);  min(arr)
来源：http://uij.xinyue.icu

PHP:  max($arr);  min($arr);
来源：http://mut.jqgfzy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zrg.zycfv.cn

TS:   Math.max(...arr);
来源：http://etm.chenzaomai.com

Java: Collections.max(list);  Collections.min(list);
来源：http://utz.hywenlv.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yhr.daxiang520.top

Ruby: arr.max;  arr.min
来源：http://evd.tianlin.xyz

C#:   list.Max();  list.Min()
来源：http://zpm.uphjek.com

[D18] 扁平化嵌套数组
来源：http://fmp.shuidangran.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mev.bjfxy.top

PHP:  array_merge(...$nested);
来源：http://kzb.hesvh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://isi.cucudq.cn

TS:   nested.flat();
来源：http://xag.fehbvm.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ptf.pengpengdd.cyou

Go:   // 手写双层循环
来源：http://gpw.yonumen.top

Ruby: nested.flatten
来源：http://oru.pengpengdd.cyou

C#:   nested.SelectMany(x => x).ToList()
来源：http://rfk.smart0.xyz

[D19] 按字段分组
来源：http://ffi.c1oappe.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dhx.hywenlv.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://eby.mhx1999.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://afa.fengsongda.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://cix.hywenlv.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qmf.chenjidiqi.icu

Go:   // 手写 map[string][]T
来源：http://mot.cucudq.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://utw.jinqigfzy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blm.bjfxy.top

[D20] 统计每个元素出现次数
来源：http://wzp.shuidangran.top

Py:   Counter(arr)
来源：http://lqa.ctjpmb.com

PHP:  array_count_values($arr);
来源：http://lwf.bbcook.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mdh.pycfn.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ayw.hnxiangtu.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rfm.pycfn.com

Go:   // 手写 map[T]int
来源：http://lgd.shanyushiyangtech.top

Ruby: arr.tally
来源：http://ues.ydzc1.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lme.quarkkingdee.top

[D21] 判断是否包含某元素
来源：http://yre.iojbl.cn

Py:   x in arr
来源：http://upp.jinyuanbaomall.cn

PHP:  in_array($x, $arr, true);
来源：http://jfd.bbcook.cn

JS:   arr.includes(x)
来源：http://qxr.xuanzx.com

TS:   arr.includes(x)
来源：http://akh.cashguo.top

Java: list.contains(x)
来源：http://kab.sweek.top

Go:   slices.Contains(arr, x)
来源：http://lwn.sufxvd.cn

Ruby: arr.include?(x)
来源：http://ote.zhoulong.xyz

C#:   list.Contains(x)
来源：http://ktm.hnxiangtu.top

[D22] 复制数组（避免共享引用）
来源：http://sub.gaohongyu789.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zfy.hywenlv.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://owz.chenlongwang.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lgb.smart0.xyz

TS:   [...arr];
来源：http://stf.jinghuilouyu.cn

Java: new ArrayList<>(list);
来源：http://voo.zdqjudy.top

Go:   copied := append([]int(nil), arr...)
来源：http://sty.yonumen.top

Ruby: arr.dup;  arr.clone
来源：http://bni.sysykeji.top

C#:   new List<int>(list);
来源：http://jny.birdmap.top

[D23] reduce 累积计算
来源：http://qwy.gotoacloud.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://aye.xziqi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lvd.shuidangran.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ztj.tian-w.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://byc.jianghu66.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://vwq.c1oappe.top

Go:   // 手写循环
来源：http://fkt.cucudq.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ljv.cqqwz.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ziw.shzxlz.cn

[D24] 字典 / Map 基本操作
来源：http://ymz.daxiang520.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yqo.c1oappe.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zsx.xingfuxueyuan.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://okt.hcnkem.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://puk.xinyue.icu

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ujv.kuanghao11.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uqq.sysykeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ycu.sufxvd.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sex.zhongyouzk.top

[D25] Set 集合去重与交并差
来源：http://tzw.zhongyouzk.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ikv.nanxuanxn.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yla.daria6918.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ijc.meibo888.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jha.xinyue.icu

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sle.gaohongyu789.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dya.jinghuilouyu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hqg.jinqigufen.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nlp.nwbrower.top

[D26] 数组转字符串
来源：http://uwg.zdbjq.cn

Py:   ", ".join(map(str, arr))
来源：http://ixp.yj20258.top

PHP:  implode(", ", $arr);
来源：http://mzy.c1oappe.top

JS:   arr.join(", ")
来源：http://mmj.xuanzx.com

TS:   arr.join(", ")
来源：http://kmn.mhx1999.top

Java: String.join(", ", list)
来源：http://cmq.hywenlv.cn

Go:   strings.Join(strs, ", ")
来源：http://szv.epnwcf.com

Ruby: arr.join(", ")
来源：http://kcq.daxiang520.top

C#:   string.Join(", ", list)
来源：http://rpj.vehdjk.com

================================================================================
来源：http://kud.iojbl.cn

E. 字符串处理
来源：http://acd.zhengqikj.top

================================================================================
来源：http://gje.xinyue.icu

[E01] 拼接字符串
来源：http://got.wangdashe.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zfz.shuidangran.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kkz.chenlongwang.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uye.wangdashe.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xqu.yuanzhike.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lif.vqdsnc.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://faj.fengsongda.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://aer.shzxlz.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rrw.jinqigufen.top

[E02] 重复字符串
来源：http://gii.nanxuanxn.top

Py:   "ab" * 3
来源：http://psg.iojbl.cn

PHP:  str_repeat("ab", 3);
来源：http://ikr.yj20258888.top

JS:   "ab".repeat(3)
来源：http://kds.jyoumei.cn

TS:   "ab".repeat(3)
来源：http://lcv.dashuyun.cn

Java: "ab".repeat(3)
来源：http://rcx.feifeiyinyue.top

Go:   strings.Repeat("ab", 3)
来源：http://uwt.fzhhl.top

Ruby: "ab" * 3
来源：http://ldj.shangyingyoupin.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mxp.iojbl.cn

[E03] 截取子串
来源：http://tnf.zhixingplan.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jnx.zhoulong.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pqm.hnxiangtu.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ofv.jinqigufen.top

TS:   s.slice(1, 4)
来源：http://snd.gzhubu.top

Java: s.substring(1, 4)
来源：http://ekk.pengpengdd.cyou

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://beh.zhaomingkeji.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://kyo.tarul.cn

C#:   s.Substring(1, 3)
来源：http://gdp.ivvv.top

[E04] 查找子串位置
来源：http://uay.wangshuangyany.cn

Py:   s.find("x");  s.index("x")
来源：http://jxj.nwbrower.top

PHP:  strpos($s, "x");
来源：http://frf.yj20258888.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mtx.jyoumei.cn

TS:   s.indexOf("x")
来源：http://xrz.guannengcc.top

Java: s.indexOf("x")
来源：http://uvk.nanxuanxn.top

Go:   strings.Index(s, "x")
来源：http://vyj.cashguo.top

Ruby: s.index("x")
来源：http://jpt.yj20258.top

C#:   s.IndexOf("x")
来源：http://xbw.guannengcc.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://lfl.vqdsnc.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wwy.xziqi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fmh.haohaochexian.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cou.fengsongda.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://swp.hysaishi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kcm.birdmap.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uvn.sjlbkw.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ska.jqgufenzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://snl.tianlin.xyz

[E06] 替换子串
来源：http://cro.yangfankeji.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ocx.yueranfly.top

PHP:  str_replace("a", "b", $s);
来源：http://lsr.yangfankeji.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://drb.ybcxt.top

TS:   s.replaceAll("a", "b")
来源：http://dxe.yueranfly.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pyu.vqdsnc.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nda.yvedp.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jbe.ehwqpu.com

C#:   s.Replace("a", "b")
来源：http://fww.birdmap.top

[E07] 按分隔符拆分
来源：http://lwm.yj202588.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pai.pycfn.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pkk.sysykeji.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://zxo.aizwys.cn

TS:   s.split(",")
来源：http://ahi.zhaomingkeji.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://gtq.jinyuanbaomall.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://clq.tianlin.xyz

Ruby: s.split(",");  s.split
来源：http://lxj.smart0.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lsu.jinqigufen.top

[E08] 数组按分隔符合并
来源：http://ish.hnqzz.top

Py:   ",".join(items)
来源：http://uqe.fengsongda.top

PHP:  implode(",", $items);
来源：http://tzd.yvedp.cn

JS:   items.join(",")
来源：http://ssj.havefunace.top

TS:   items.join(",")
来源：http://sbt.yueranfly.top

Java: String.join(",", items)
来源：http://otu.sweek.top

Go:   strings.Join(items, ",")
来源：http://dci.havefunace.top

Ruby: items.join(",")
来源：http://cfs.zhaomingkeji.xyz

C#:   string.Join(",", items)
来源：http://pjo.wangdashe.top

[E09] 去除所有空白字符
来源：http://ubr.cqqwz.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qvd.meibo888.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dvg.bjfxy.top

JS:   s.replace(/\s+/g, "")
来源：http://vwf.fanxiaobao.xyz

TS:   s.replace(/\s+/g, "")
来源：http://grd.hnqzz.top

Java: s.replaceAll("\\s+", "")
来源：http://wmr.shanyushiyangkeji.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://wnz.yj20258888.top

Ruby: s.gsub(/\s+/, "")
来源：http://kdg.havefunace.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://okj.tanke756.top

[E10] 左侧补零 / 定长填充
来源：http://fsp.9152youxi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qai.gogol.net.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://chi.xinyue.icu

JS:   "7".padStart(3, "0")
来源：http://drv.shangyingyoupin.top

TS:   "7".padStart(3, "0")
来源：http://mrd.jyoumei.cn

Java: String.format("%03d", 7)
来源：http://cqu.fzhhl.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://xfc.fktsv.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ivz.hcnkem.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nvv.aizwys.cn

[E11] 反转字符串
来源：http://sxe.yanxiufei.cn

Py:   s[::-1]
来源：http://aby.bbcook.cn

PHP:  strrev($s);
来源：http://bjy.redwolf501.top

JS:   [...s].reverse().join("")
来源：http://zds.sjlbkw.cn

TS:   [...s].reverse().join("")
来源：http://nyp.jqgfzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://srf.hywenlv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://nsl.svipenyu.cn

Ruby: s.reverse
来源：http://mkd.nanxinkj.top

C#:   new string(s.Reverse().ToArray())
来源：http://zmk.wangshuangyany.cn

[E12] 统计某字符出现次数
来源：http://hnb.zhiwuduotai.top

Py:   s.count("a")
来源：http://jfd.yuxming.cn

PHP:  substr_count($s, "a");
来源：http://tqp.9152youxi.cn

JS:   s.split("a").length - 1
来源：http://zwz.cqqwz.cn

TS:   s.split("a").length - 1
来源：http://wgb.zhongyouzk.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://utq.jinghuilouyu.cn

Go:   strings.Count(s, "a")
来源：http://vrp.meibo888.top

Ruby: s.count("a")
来源：http://qbl.yvedp.cn

C#:   s.Count(c => c == 'a')
来源：http://lwp.wangshuangyany.cn

[E13] 逐字符遍历
来源：http://trh.ivvv.top

Py:   for ch in s: print(ch)
来源：http://zlk.fehbvm.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xxk.guowangkeji.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://hct.c1oappe.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://cte.fktsv.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://whd.shanyushiyangtech.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jst.dashuyun.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vok.jinqigfzy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fze.yongpay.top

[E14] URL 编码与 Base64
来源：http://dds.yj20258888.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jzn.bjfxy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ejr.ybcxt.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://oyk.xylfe.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dow.aizwys.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://aoz.chenjidiqi.icu

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dgz.ehwqpu.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ddm.c1oappe.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cja.yangfankeji.com

[E15] HTML 转义 / 反转义
来源：http://kfg.nanxinkj.top

Py:   html.escape(s);  html.unescape(s)
来源：http://dii.tianlin.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hyt.yueranfly.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hon.hesvh.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fol.yongpay.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rli.gogol.net.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://iyu.cucudq.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://iwl.cucudq.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ozg.jinqigufen.top

[E16] 数字千分位
来源：http://rru.zhongyouzk.top

Py:   f"{1234567:,}"
来源：http://dom.ywan-chungtsiang.top

PHP:  number_format(1234567);
来源：http://mxy.zhiwuduotai.top

JS:   (1234567).toLocaleString("en-US")
来源：http://gok.xziqi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ubi.smart0.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jao.xuetiantiany.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jmz.chenjidiqi.icu

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vdv.52xcode.cn

C#:   1234567.ToString("N0")
来源：http://ctl.gzhubu.top

[E17] 首字母大写
来源：http://qyb.jyoumei.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hth.vqdsnc.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://cnn.yj202588.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pwz.zdqjudy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://frt.aibaodan.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ivg.cucudq.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jtb.zhiwuduotai.top

Ruby: s.capitalize
来源：http://hcb.yfazqb.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wyy.gogol.net.cn

[E18] 模板占位符替换
来源：http://egt.cheryme.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hdi.xinyue.icu

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gnh.hongshengwenyu.top

JS:   tpl.replaceAll("{name}", name)
来源：http://hea.jinqigfzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://xgr.haohaochexian.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gig.hywenlv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cxd.zhaomingkeji.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ndh.yongpay.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://env.yongpay.top

[E19] 多行文本按行拆分
来源：http://vgd.chenzaomai.com

Py:   s.splitlines()
来源：http://whg.svipenyu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://isa.yanxiufei.cn


<!-- 参考信息 -->