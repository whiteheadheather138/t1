代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lne.svipenyu.cn

JS:   arr.filter(x => x > 3)
来源：http://ysx.zhaomingkeji.xyz

TS:   arr.filter(x => x > 3)
来源：http://qef.nanxinkj.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zsx.sweek.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uwn.tanke756.top

Ruby: arr.select { |x| x > 3 }
来源：http://loz.nwbrower.top

C#:   list.Where(x => x > 3).ToList()
来源：http://mhc.gzhubu.top

[D14] 映射转换（每个元素变形）
来源：http://cqx.xylfe.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dgw.guannengcc.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ose.xylfe.cn

JS:   arr.map(x => x * 2)
来源：http://wuh.hammf.cn

TS:   arr.map(x => x * 2)
来源：http://ntb.cashguo.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://mly.ctjpmb.com

Go:   // 手写循环
来源：http://elf.yvedp.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qes.hysaishi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jdc.ydzc1.top

[D15] 去重
来源：http://hxk.gzhubu.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kdk.zhixingplan.top

PHP:  array_unique($arr);
来源：http://hvr.jiagoushi.top

JS:   [...new Set(arr)]
来源：http://yxj.yongpay.top

TS:   [...new Set(arr)]
来源：http://irq.c1oappe.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mkl.sjlbkw.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ejq.redwolf501.top

Ruby: arr.uniq
来源：http://kis.fengsongda.top

C#:   list.Distinct().ToList()
来源：http://qqi.bjfxy.top

[D16] 求和与平均值
来源：http://uvy.xinyue.icu

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://esb.guannengcc.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://knj.yj20258888.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://trc.bjfxy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pow.meibo888.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mef.shuidangran.top

Go:   // 手写循环累加
来源：http://lpf.iojbl.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rfm.jinqigufen.top

C#:   list.Sum();  list.Average()
来源：http://fyc.sjlbkw.cn

[D17] 最大值与最小值
来源：http://hti.gotoacloud.top

Py:   max(arr);  min(arr)
来源：http://xkd.hywenlv.cn

PHP:  max($arr);  min($arr);
来源：http://rug.jinqigfzy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jrh.yuxming.cn

TS:   Math.max(...arr);
来源：http://zqx.pycfn.com

Java: Collections.max(list);  Collections.min(list);
来源：http://mwe.shuidangran.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vpj.sweek.top

Ruby: arr.max;  arr.min
来源：http://aux.shanyushiyangtech.top

C#:   list.Max();  list.Min()
来源：http://xjj.fehbvm.com

[D18] 扁平化嵌套数组
来源：http://wqs.hammf.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xgo.guannengcc.top

PHP:  array_merge(...$nested);
来源：http://xuf.hfpthk.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nnu.hcnkem.com

TS:   nested.flat();
来源：http://efo.yuxming.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sww.nwbrower.top

Go:   // 手写双层循环
来源：http://lct.jiagoushi.top

Ruby: nested.flatten
来源：http://bqd.zhijiandao.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://glp.yj20258888.top

[D19] 按字段分组
来源：http://chy.snrcjt.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wal.hnqzz.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hfd.shangyingyoupin.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xtn.zycfv.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zne.xuanzx.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://aua.shuidangran.top

Go:   // 手写 map[string][]T
来源：http://cli.jinqigfzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://okt.cashguo.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://trh.jlsjyb.cn

[D20] 统计每个元素出现次数
来源：http://bkg.shangyingyoupin.top

Py:   Counter(arr)
来源：http://afc.hesvh.cn

PHP:  array_count_values($arr);
来源：http://piq.zhixingplan.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://exu.zhoulong.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ozd.yuanzhike.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://raq.yj20258.top

Go:   // 手写 map[T]int
来源：http://xwi.yfazqb.com

Ruby: arr.tally
来源：http://lqf.hnxiangtu.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rlu.jiagoushi.top

[D21] 判断是否包含某元素
来源：http://fdv.daxiang520.top

Py:   x in arr
来源：http://eox.shanyushiyangtech.top

PHP:  in_array($x, $arr, true);
来源：http://byc.tian-w.cn

JS:   arr.includes(x)
来源：http://ycl.dianchejie.cn

TS:   arr.includes(x)
来源：http://rkj.ivvv.top

Java: list.contains(x)
来源：http://ydm.xylfe.cn

Go:   slices.Contains(arr, x)
来源：http://osk.ywan-chungtsiang.top

Ruby: arr.include?(x)
来源：http://qij.0kj1m.cn

C#:   list.Contains(x)
来源：http://ueu.fktsv.cn

[D22] 复制数组（避免共享引用）
来源：http://hlm.aizwys.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mbj.ydjk.org.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xwo.ehwqpu.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xmq.fktsv.cn

TS:   [...arr];
来源：http://kju.andypj.xyz

Java: new ArrayList<>(list);
来源：http://xls.xingfuxueyuan.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://lgv.zhiwuduotai.top

Ruby: arr.dup;  arr.clone
来源：http://tzt.yueranfly.top

C#:   new List<int>(list);
来源：http://xxo.aizwys.cn

[D23] reduce 累积计算
来源：http://knj.yueranfly.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xhh.yuanzhike.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dvo.mhx1999.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dag.epnwcf.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jyg.zycfv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ofa.redwolf501.top

Go:   // 手写循环
来源：http://gbj.ivvv.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jbc.hywenlv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rpu.epnwcf.com

[D24] 字典 / Map 基本操作
来源：http://xql.hongshengwenyu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mts.yj20258.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wgw.sxryk.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hkb.birdmap.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jhu.9152youxi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ahf.gotoacloud.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dhn.cheryme.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xqk.ppjwa.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ejj.dianchejie.cn

[D25] Set 集合去重与交并差
来源：http://vqb.vehdjk.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pam.gotoacloud.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gas.9152youxi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mgm.shuidangran.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://abg.aibaodan.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qpz.hammf.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ttt.ydzc1.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jxg.daria6918.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mdh.yfazqb.com

[D26] 数组转字符串
来源：http://pmc.ppjwa.cn

Py:   ", ".join(map(str, arr))
来源：http://mns.52xcode.cn

PHP:  implode(", ", $arr);
来源：http://dhw.yanxiufei.cn

JS:   arr.join(", ")
来源：http://vqf.epnwcf.com

TS:   arr.join(", ")
来源：http://eat.nanxinkj.top

Java: String.join(", ", list)
来源：http://cor.chenjidiqi.icu

Go:   strings.Join(strs, ", ")
来源：http://nhu.shzxlz.cn

Ruby: arr.join(", ")
来源：http://rlf.fehbvm.com

C#:   string.Join(", ", list)
来源：http://qoa.wangdashe.top

================================================================================
来源：http://rtg.wangdashe.top

E. 字符串处理
来源：http://kkh.zycfv.cn

================================================================================
来源：http://ltv.vehdjk.com

[E01] 拼接字符串
来源：http://kww.daxiang520.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nza.fanxiaobao.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yxs.shzxlz.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mnr.cashguo.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ral.andypj.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xse.316326.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rky.sxryk.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gle.fengsongda.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zay.sjlbkw.cn

[E02] 重复字符串
来源：http://srs.fanxiaobao.xyz

Py:   "ab" * 3
来源：http://jgv.hcnkem.com

PHP:  str_repeat("ab", 3);
来源：http://dno.jlsjyb.cn

JS:   "ab".repeat(3)
来源：http://wer.yueranfly.top

TS:   "ab".repeat(3)
来源：http://hni.nanxuanxn.top

Java: "ab".repeat(3)
来源：http://oae.ywan-chungtsiang.top

Go:   strings.Repeat("ab", 3)
来源：http://hop.yj20258.top

Ruby: "ab" * 3
来源：http://wlo.hcnkem.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vqu.xuanzx.com

[E03] 截取子串
来源：http://dbs.jianghu66.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://aku.meibo888.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wmf.jyoumei.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://oap.vqdsnc.cn

TS:   s.slice(1, 4)
来源：http://swz.fengsongda.top

Java: s.substring(1, 4)
来源：http://dle.fzhhl.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xua.snrcjt.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jqu.pycfn.com

C#:   s.Substring(1, 3)
来源：http://dfb.daxiang520.top

[E04] 查找子串位置
来源：http://voc.ydjk.org.cn

Py:   s.find("x");  s.index("x")
来源：http://fcj.hesvh.cn

PHP:  strpos($s, "x");
来源：http://php.0kj1m.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rxa.chenjidiqi.icu

TS:   s.indexOf("x")
来源：http://tyi.hysaishi.cn

Java: s.indexOf("x")
来源：http://amz.ydzc1.top

Go:   strings.Index(s, "x")
来源：http://psu.aibaodan.cn

Ruby: s.index("x")
来源：http://osb.fzhhl.top

C#:   s.IndexOf("x")
来源：http://jrp.fehbvm.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://hdv.xinyue.icu

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dlf.bbcook.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rea.hfpthk.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vkn.nanxinkj.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ysu.chenlongwang.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mzz.cqqwz.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bkv.nanxuanxn.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rar.sjlbkw.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://smf.mhx1999.top

[E06] 替换子串
来源：http://fag.yj20258.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mwt.zhengqikj.top

PHP:  str_replace("a", "b", $s);
来源：http://vgj.wangdashe.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fhj.tian-w.cn

TS:   s.replaceAll("a", "b")
来源：http://zfd.fanxiaobao.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://icd.ctjpmb.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://czu.jqgufenzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xsk.quarkkingdee.top

C#:   s.Replace("a", "b")
来源：http://vyv.jyoumei.cn

[E07] 按分隔符拆分
来源：http://pws.dashuyun.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://iau.hfpthk.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qsb.316326.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://swt.pycfn.com

TS:   s.split(",")
来源：http://bct.guowangkeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://rny.jinqigufen.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://shf.sufxvd.cn

Ruby: s.split(",");  s.split
来源：http://wga.fzhhl.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hee.yuanzhike.top

[E08] 数组按分隔符合并
来源：http://wqh.zhoulong.xyz

Py:   ",".join(items)
来源：http://avk.mhx1999.top

PHP:  implode(",", $items);
来源：http://tjb.gaohongyu789.top

JS:   items.join(",")
来源：http://kpv.chenzaomai.com

TS:   items.join(",")
来源：http://roj.iojbl.cn

Java: String.join(",", items)
来源：http://qul.gaohongyu789.top

Go:   strings.Join(items, ",")
来源：http://jtf.cdnleiting.top

Ruby: items.join(",")
来源：http://rse.bjfxy.top

C#:   string.Join(",", items)
来源：http://fqn.shangyingyoupin.top

[E09] 去除所有空白字符
来源：http://gga.yangfankeji.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bsr.hysaishi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wox.zhijiandao.cn

JS:   s.replace(/\s+/g, "")
来源：http://aie.guannengcc.top

TS:   s.replace(/\s+/g, "")
来源：http://ryu.gogol.net.cn

Java: s.replaceAll("\\s+", "")
来源：http://lxz.yueranfly.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://wbl.ppjwa.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ayq.yj20258888.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mlk.xuetiantiany.cn

[E10] 左侧补零 / 定长填充
来源：http://ztg.fzhhl.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://neu.aibaodan.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ewr.hywenlv.cn

JS:   "7".padStart(3, "0")
来源：http://sla.sjlbkw.cn

TS:   "7".padStart(3, "0")
来源：http://voo.tarul.cn

Java: String.format("%03d", 7)
来源：http://owd.zdqjudy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://tdi.svipenyu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ufw.havefunace.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gfj.guowangkeji.top

[E11] 反转字符串
来源：http://oeb.birdmap.top

Py:   s[::-1]
来源：http://mxk.daxiang520.top

PHP:  strrev($s);
来源：http://hvz.zdbjq.cn

JS:   [...s].reverse().join("")
来源：http://lrh.316326.xyz

TS:   [...s].reverse().join("")
来源：http://ytc.yuxming.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://yww.feifeiyinyue.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://rkp.zhengqikj.top

Ruby: s.reverse
来源：http://uhj.tian-w.cn

C#:   new string(s.Reverse().ToArray())
来源：http://tak.yangfankeji.com

[E12] 统计某字符出现次数
来源：http://ttl.xylfe.cn

Py:   s.count("a")
来源：http://cmj.xinyue.icu

PHP:  substr_count($s, "a");
来源：http://xep.fanxiaobao.xyz

JS:   s.split("a").length - 1
来源：http://pad.bjfxy.top

TS:   s.split("a").length - 1
来源：http://xkw.chenlongwang.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://doe.zhaomingkeji.xyz

Go:   strings.Count(s, "a")
来源：http://zrd.pengpengdd.cyou

Ruby: s.count("a")
来源：http://oic.xziqi.cn

C#:   s.Count(c => c == 'a')
来源：http://xyt.hnqzz.top

[E13] 逐字符遍历
来源：http://fuj.gotoacloud.top

Py:   for ch in s: print(ch)
来源：http://fzh.jlsjyb.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tmv.zhiwuduotai.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://vdr.jiagoushi.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ios.daxiang520.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bpe.sysykeji.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wnf.epnwcf.com

Ruby: s.each_char { |ch| puts ch }
来源：http://awl.tanke756.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sgm.vqdsnc.cn

[E14] URL 编码与 Base64
来源：http://qjh.zhongyouzk.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rwx.kuanghao11.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://smv.ppjwa.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://idf.kuanghao11.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lfv.chenzaomai.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jgl.guowangkeji.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qom.fengsongda.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ihl.shanyushiyangtech.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vuz.jianghu66.top

[E15] HTML 转义 / 反转义
来源：http://sia.cdnleiting.top

Py:   html.escape(s);  html.unescape(s)
来源：http://lvp.zhijiandao.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://evj.jqgfzy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jxu.havefunace.top

TS:   // 同上，务必做 XSS 过滤
来源：http://tfx.yonumen.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rtq.zhongyouzk.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gjj.vqdsnc.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jou.hongshengwenyu.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ryb.dianchejie.cn

[E16] 数字千分位
来源：http://uuu.zhengqikj.top

Py:   f"{1234567:,}"
来源：http://ott.hcnkem.com

PHP:  number_format(1234567);
来源：http://faz.feifeiyinyue.top

JS:   (1234567).toLocaleString("en-US")
来源：http://vaw.ivvv.top

TS:   (1234567).toLocaleString("en-US")
来源：http://tji.ybcxt.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://oad.ybcxt.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yjj.uphjek.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tlq.pycfn.com

C#:   1234567.ToString("N0")
来源：http://bfc.hywenlv.cn

[E17] 首字母大写
来源：http://jps.daria6918.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jtu.jiagoushi.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://oue.epnwcf.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ksb.gogol.net.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://olv.shuidangran.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jzf.cdnleiting.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xyh.shzxlz.cn

Ruby: s.capitalize
来源：http://dzn.fzhhl.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lmk.bbcook.cn

[E18] 模板占位符替换
来源：http://zjc.jiagoushi.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qhk.cashguo.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://osm.ctjpmb.com

JS:   tpl.replaceAll("{name}", name)
来源：http://pgx.jqgfzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://avh.wangdashe.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pzu.snrcjt.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lmy.nanxinkj.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zfh.hfpthk.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uro.bbcook.cn

[E19] 多行文本按行拆分
来源：http://rbl.tian-w.cn

Py:   s.splitlines()
来源：http://rsh.yj20258.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://uxj.sufxvd.cn

JS:   s.split(/\r?\n/)
来源：http://nxg.ydzc1.top

TS:   s.split(/\r?\n/)
来源：http://dxf.hywenlv.cn

Java: s.lines().toList()
来源：http://zef.cheryme.top

Go:   strings.Split(s, "\n")
来源：http://mer.yfazqb.com

Ruby: s.lines
来源：http://erf.hammf.cn

C#:   s.Split('\n')
来源：http://noi.zhixingplan.top

[E20] 判断字符串是否为空
来源：http://yqo.yj20258.top

Py:   if not s:
来源：http://wmx.ywan-chungtsiang.top


<!-- 参考信息 -->