代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kdt.vqdsnc.cn

JS:   arr.filter(x => x > 3)
来源：http://afr.pengpengdd.cyou

TS:   arr.filter(x => x > 3)
来源：http://kzv.zhixingplan.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ciz.epnwcf.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tyd.nanxuanxn.top

Ruby: arr.select { |x| x > 3 }
来源：http://nmy.fehbvm.com

C#:   list.Where(x => x > 3).ToList()
来源：http://fke.daxiang520.top

[D14] 映射转换（每个元素变形）
来源：http://rvw.fzhhl.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wur.sjlbkw.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bsu.andypj.xyz

JS:   arr.map(x => x * 2)
来源：http://yfh.gotoacloud.top

TS:   arr.map(x => x * 2)
来源：http://srk.wangshuangyany.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sgq.0kj1m.cn

Go:   // 手写循环
来源：http://rrk.52xcode.cn

Ruby: arr.map { |x| x * 2 }
来源：http://byj.cdnleiting.top

C#:   list.Select(x => x * 2).ToList()
来源：http://cre.aibaodan.cn

[D15] 去重
来源：http://szo.xuanzx.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://psc.uphjek.com

PHP:  array_unique($arr);
来源：http://xhs.xuanzx.com

JS:   [...new Set(arr)]
来源：http://xxz.pengpengdd.cyou

TS:   [...new Set(arr)]
来源：http://dvd.nanxuanxn.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ehf.hfpthk.cn

Go:   // 用 map[T]struct{} 手写
来源：http://bpt.yonumen.top

Ruby: arr.uniq
来源：http://yns.mhx1999.top

C#:   list.Distinct().ToList()
来源：http://pty.wangdashe.top

[D16] 求和与平均值
来源：http://cwu.xinyue.icu

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kfr.zhongyouzk.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cug.tanke756.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fow.yonumen.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://avs.guowangkeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rcv.meibo888.top

Go:   // 手写循环累加
来源：http://phm.zhaomingkeji.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xsv.zhijiandao.cn

C#:   list.Sum();  list.Average()
来源：http://fcu.shangyingyoupin.top

[D17] 最大值与最小值
来源：http://bje.cheryme.top

Py:   max(arr);  min(arr)
来源：http://nso.ivvv.top

PHP:  max($arr);  min($arr);
来源：http://diz.haohaochexian.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qxf.ppjwa.cn

TS:   Math.max(...arr);
来源：http://xvm.havefunace.top

Java: Collections.max(list);  Collections.min(list);
来源：http://zln.jianghu66.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jzj.fehbvm.com

Ruby: arr.max;  arr.min
来源：http://yem.yj20258888.top

C#:   list.Max();  list.Min()
来源：http://ggy.bbcook.cn

[D18] 扁平化嵌套数组
来源：http://nhp.pengpengdd.cyou

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zjr.hnxiangtu.top

PHP:  array_merge(...$nested);
来源：http://iok.jianghu66.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mls.jqgfzy.top

TS:   nested.flat();
来源：http://xat.c1oappe.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vig.hnqzz.top

Go:   // 手写双层循环
来源：http://uxq.kuanghao11.cn

Ruby: nested.flatten
来源：http://qjc.tianlin.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://aym.hywenlv.cn

[D19] 按字段分组
来源：http://mue.chenzaomai.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://woq.ywan-chungtsiang.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wou.ywan-chungtsiang.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uot.jinghuilouyu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rkn.cdnleiting.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yfo.yfazqb.com

Go:   // 手写 map[string][]T
来源：http://ylu.yj20258.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://bvk.yueranfly.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://apv.ydzc1.top

[D20] 统计每个元素出现次数
来源：http://alg.316326.xyz

Py:   Counter(arr)
来源：http://cbb.jqgufenzy.top

PHP:  array_count_values($arr);
来源：http://alf.jinyuanbaomall.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eyf.aizwys.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qfe.yonumen.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://shq.316326.xyz

Go:   // 手写 map[T]int
来源：http://cmv.sysykeji.top

Ruby: arr.tally
来源：http://mfo.ydjk.org.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gqy.zhijiandao.cn

[D21] 判断是否包含某元素
来源：http://aka.iojbl.cn

Py:   x in arr
来源：http://rbp.zhengqikj.top

PHP:  in_array($x, $arr, true);
来源：http://ijy.zhoulong.xyz

JS:   arr.includes(x)
来源：http://zzl.fehbvm.com

TS:   arr.includes(x)
来源：http://cwe.tian-w.cn

Java: list.contains(x)
来源：http://brl.fzhhl.top

Go:   slices.Contains(arr, x)
来源：http://txr.zycfv.cn

Ruby: arr.include?(x)
来源：http://mqe.smart0.xyz

C#:   list.Contains(x)
来源：http://mvb.yfazqb.com

[D22] 复制数组（避免共享引用）
来源：http://nmo.shuidangran.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lyl.guannengcc.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xtl.zhiwuduotai.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gwb.316326.xyz

TS:   [...arr];
来源：http://bfq.sysykeji.top

Java: new ArrayList<>(list);
来源：http://rzm.andypj.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://cnl.jinyuanbaomall.cn

Ruby: arr.dup;  arr.clone
来源：http://gbp.birdmap.top

C#:   new List<int>(list);
来源：http://eup.jyoumei.cn

[D23] reduce 累积计算
来源：http://rdh.jinghuilouyu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sft.tianlin.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cyz.xuetiantiany.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ual.vqdsnc.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://osa.cucudq.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://trg.yuanzhike.top

Go:   // 手写循环
来源：http://ivj.sxryk.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ybr.andypj.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ksj.zdbjq.cn

[D24] 字典 / Map 基本操作
来源：http://qhy.daxiang520.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zzy.uphjek.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zan.jqgfzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yti.chenzaomai.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gch.pengpengdd.cyou

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cnl.xinyue.icu

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mxg.iojbl.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://plx.cqqwz.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://doe.ywan-chungtsiang.top

[D25] Set 集合去重与交并差
来源：http://hlg.chenlongwang.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hil.hesvh.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nvt.xinyue.icu

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gan.gaohongyu789.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://svq.cdnleiting.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dcv.cashguo.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ptu.ydjk.org.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ned.yonumen.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qmy.ydzc1.top

[D26] 数组转字符串
来源：http://quo.hfpthk.cn

Py:   ", ".join(map(str, arr))
来源：http://vtf.haohaochexian.top

PHP:  implode(", ", $arr);
来源：http://geo.ivvv.top

JS:   arr.join(", ")
来源：http://icf.jinyuanbaomall.cn

TS:   arr.join(", ")
来源：http://vjg.jlsjyb.cn

Java: String.join(", ", list)
来源：http://knw.yueranfly.top

Go:   strings.Join(strs, ", ")
来源：http://fvb.epnwcf.com

Ruby: arr.join(", ")
来源：http://uzr.tian-w.cn

C#:   string.Join(", ", list)
来源：http://ifa.guannengcc.top

================================================================================
来源：http://xam.yj202588.top

E. 字符串处理
来源：http://hdx.wangshuangyany.cn

================================================================================
来源：http://wzr.shzxlz.cn

[E01] 拼接字符串
来源：http://xja.ywan-chungtsiang.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bwt.hcnkem.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qka.yvedp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ygm.shuidangran.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vxt.ctjpmb.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ttv.ydjk.org.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rvi.c1oappe.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lpo.9152youxi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kde.hywenlv.cn

[E02] 重复字符串
来源：http://vun.ywan-chungtsiang.top

Py:   "ab" * 3
来源：http://spm.zhixingplan.top

PHP:  str_repeat("ab", 3);
来源：http://cbs.nanxinkj.top

JS:   "ab".repeat(3)
来源：http://jgs.chenjidiqi.icu

TS:   "ab".repeat(3)
来源：http://tay.hysaishi.cn

Java: "ab".repeat(3)
来源：http://cmp.cdnleiting.top

Go:   strings.Repeat("ab", 3)
来源：http://zqb.svipenyu.cn

Ruby: "ab" * 3
来源：http://uuz.birdmap.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vle.hesvh.cn

[E03] 截取子串
来源：http://bbm.wangshuangyany.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yxd.yj20258.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jod.aizwys.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ros.zhaomingkeji.xyz

TS:   s.slice(1, 4)
来源：http://vxa.0kj1m.cn

Java: s.substring(1, 4)
来源：http://gpk.yuanzhike.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qtw.havefunace.top

Ruby: s[1, 3];  s[1..3]
来源：http://tym.yonumen.top

C#:   s.Substring(1, 3)
来源：http://bmk.hammf.cn

[E04] 查找子串位置
来源：http://rnk.yonumen.top

Py:   s.find("x");  s.index("x")
来源：http://isz.zhaomingkeji.xyz

PHP:  strpos($s, "x");
来源：http://juk.yanxiufei.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vgi.tian-w.cn

TS:   s.indexOf("x")
来源：http://iqw.zhaomingkeji.xyz

Java: s.indexOf("x")
来源：http://lfe.haohaochexian.top

Go:   strings.Index(s, "x")
来源：http://nri.gotoacloud.top

Ruby: s.index("x")
来源：http://ysy.zhengqikj.top

C#:   s.IndexOf("x")
来源：http://srg.smart0.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://sqq.cdnleiting.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://int.aibaodan.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lwu.cdnleiting.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://slj.chenlongwang.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://nrg.havefunace.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wcg.shangyingyoupin.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kkt.pengpengdd.cyou

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dmf.zhongyouzk.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://krh.cucudq.cn

[E06] 替换子串
来源：http://dyb.wangdashe.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zjl.mhx1999.top

PHP:  str_replace("a", "b", $s);
来源：http://lyc.bbcook.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vat.xuetiantiany.cn

TS:   s.replaceAll("a", "b")
来源：http://sum.uphjek.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vvd.shuidangran.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://urx.0kj1m.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rtf.fzhhl.top

C#:   s.Replace("a", "b")
来源：http://hrm.sysykeji.top

[E07] 按分隔符拆分
来源：http://xqe.yongpay.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vdr.ehwqpu.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jly.bjfxy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://hql.svipenyu.cn

TS:   s.split(",")
来源：http://mxw.jqgufenzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://mfz.shuidangran.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kpz.jianghu66.top

Ruby: s.split(",");  s.split
来源：http://bds.gotoacloud.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zjw.yanxiufei.cn

[E08] 数组按分隔符合并
来源：http://tig.zhaomingkeji.xyz

Py:   ",".join(items)
来源：http://lqy.shzxlz.cn

PHP:  implode(",", $items);
来源：http://tgj.vehdjk.com

JS:   items.join(",")
来源：http://qfs.meibo888.top

TS:   items.join(",")
来源：http://bqd.zhongyouzk.top

Java: String.join(",", items)
来源：http://ibn.chenjidiqi.icu

Go:   strings.Join(items, ",")
来源：http://doh.ppjwa.cn

Ruby: items.join(",")
来源：http://cxh.shanyushiyangkeji.top

C#:   string.Join(",", items)
来源：http://fkg.chenzaomai.com

[E09] 去除所有空白字符
来源：http://eqc.ctjpmb.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ein.cucudq.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wyh.ywan-chungtsiang.top

JS:   s.replace(/\s+/g, "")
来源：http://wep.cheryme.top

TS:   s.replace(/\s+/g, "")
来源：http://bit.jinqigufen.top

Java: s.replaceAll("\\s+", "")
来源：http://uak.daxiang520.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://dad.yj20258.top

Ruby: s.gsub(/\s+/, "")
来源：http://mkq.daxiang520.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sir.sjlbkw.cn

[E10] 左侧补零 / 定长填充
来源：http://ond.ydjk.org.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nxm.fehbvm.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ekx.snrcjt.cn

JS:   "7".padStart(3, "0")
来源：http://ief.kuanghao11.cn

TS:   "7".padStart(3, "0")
来源：http://ele.smart0.xyz

Java: String.format("%03d", 7)
来源：http://nir.hywenlv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://lry.redwolf501.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yzg.c1oappe.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nvx.yanxiufei.cn

[E11] 反转字符串
来源：http://jrm.jlsjyb.cn

Py:   s[::-1]
来源：http://kjp.fengsongda.top

PHP:  strrev($s);
来源：http://knz.zhiwuduotai.top

JS:   [...s].reverse().join("")
来源：http://tvq.chenlongwang.top

TS:   [...s].reverse().join("")
来源：http://rrw.daxiang520.top

Java: new StringBuilder(s).reverse().toString()
来源：http://qbe.chenzaomai.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://lli.vqdsnc.cn

Ruby: s.reverse
来源：http://qbc.hfpthk.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gty.hfpthk.cn

[E12] 统计某字符出现次数
来源：http://tsx.ppjwa.cn

Py:   s.count("a")
来源：http://ult.hnqzz.top

PHP:  substr_count($s, "a");
来源：http://xfg.jiagoushi.top

JS:   s.split("a").length - 1
来源：http://zcb.zhoulong.xyz

TS:   s.split("a").length - 1
来源：http://jhb.zycfv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://omu.jyoumei.cn

Go:   strings.Count(s, "a")
来源：http://sca.nwbrower.top

Ruby: s.count("a")
来源：http://zfj.xingfuxueyuan.xyz

C#:   s.Count(c => c == 'a')
来源：http://bai.zhongyouzk.top

[E13] 逐字符遍历
来源：http://tvo.cheryme.top

Py:   for ch in s: print(ch)
来源：http://zcl.fzhhl.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://iyt.zycfv.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://yvv.yj202588.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://wpx.yj20258888.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://eft.yonumen.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lxp.zhiwuduotai.top

Ruby: s.each_char { |ch| puts ch }
来源：http://vvv.zhixingplan.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ksl.hfpthk.cn

[E14] URL 编码与 Base64
来源：http://jwf.epnwcf.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://apg.yfazqb.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://iqb.jinyuanbaomall.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hns.xingfuxueyuan.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lay.yj202588.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rdv.zhongyouzk.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cdf.ydjk.org.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lyz.cheryme.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xvz.hfpthk.cn

[E15] HTML 转义 / 反转义
来源：http://inc.xuetiantiany.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://myw.hongshengwenyu.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kay.tanke756.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nps.daxiang520.top

TS:   // 同上，务必做 XSS 过滤
来源：http://hsz.316326.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lfk.yongpay.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vxw.yangfankeji.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://asj.ppjwa.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xtr.wangshuangyany.cn

[E16] 数字千分位
来源：http://nsw.havefunace.top

Py:   f"{1234567:,}"
来源：http://ogu.hesvh.cn

PHP:  number_format(1234567);
来源：http://oan.fktsv.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://klm.feifeiyinyue.top

TS:   (1234567).toLocaleString("en-US")
来源：http://mgp.yonumen.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yrp.ppjwa.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://eyp.zycfv.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ayb.c1oappe.top

C#:   1234567.ToString("N0")
来源：http://tuw.gogol.net.cn

[E17] 首字母大写
来源：http://ech.cashguo.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cpe.chenjidiqi.icu

PHP:  ucfirst($s);  ucwords($s);
来源：http://trk.ivvv.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lee.havefunace.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tca.yueranfly.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://txv.chenlongwang.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mgl.9152youxi.cn

Ruby: s.capitalize
来源：http://aoa.c1oappe.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hiu.yangfankeji.com

[E18] 模板占位符替换
来源：http://kbj.aibaodan.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ccl.jinqigfzy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jam.xylfe.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://cju.uphjek.com

TS:   tpl.replaceAll("{name}", name)
来源：http://suy.svipenyu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://coz.cqqwz.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cmu.yuxming.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fow.jinqigufen.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ere.aizwys.cn

[E19] 多行文本按行拆分
来源：http://qkf.0kj1m.cn

Py:   s.splitlines()
来源：http://kis.hnxiangtu.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://eee.fanxiaobao.xyz

JS:   s.split(/\r?\n/)
来源：http://qna.daxiang520.top

TS:   s.split(/\r?\n/)
来源：http://ivo.yj20258.top

Java: s.lines().toList()
来源：http://qag.chenlongwang.top

Go:   strings.Split(s, "\n")
来源：http://eyp.chenjidiqi.icu

Ruby: s.lines
来源：http://dsx.wangshuangyany.cn

C#:   s.Split('\n')
来源：http://vrx.daria6918.cn

[E20] 判断字符串是否为空
来源：http://gjp.shanyushiyangkeji.top

Py:   if not s:
来源：http://fww.epnwcf.com


<!-- 参考信息 -->