代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uyf.jinqigufen.top

Ruby: arr.select { |x| x > 3 }
来源：http://gxm.yongpay.top

C#:   list.Where(x => x > 3).ToList()
来源：http://nhv.xuetiantiany.cn

[D14] 映射转换（每个元素变形）
来源：http://tek.nanxuanxn.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kqi.sjlbkw.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ssm.ydjk.org.cn

JS:   arr.map(x => x * 2)
来源：http://rin.sufxvd.cn

TS:   arr.map(x => x * 2)
来源：http://kbc.hnqzz.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://okq.guannengcc.top

Go:   // 手写循环
来源：http://yoc.ivvv.top

Ruby: arr.map { |x| x * 2 }
来源：http://kpe.pengpengdd.cyou

C#:   list.Select(x => x * 2).ToList()
来源：http://itb.sysykeji.top

[D15] 去重
来源：http://nbs.xylfe.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fph.ydzc1.top

PHP:  array_unique($arr);
来源：http://qfz.wangdashe.top

JS:   [...new Set(arr)]
来源：http://jci.ywan-chungtsiang.top

TS:   [...new Set(arr)]
来源：http://zsi.ppjwa.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://iyz.52xcode.cn

Go:   // 用 map[T]struct{} 手写
来源：http://mhg.shanyushiyangtech.top

Ruby: arr.uniq
来源：http://zcm.nwbrower.top

C#:   list.Distinct().ToList()
来源：http://ima.gzhubu.top

[D16] 求和与平均值
来源：http://cvx.gaohongyu789.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vdd.yj20258888.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xvm.dianchejie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mwe.yuxming.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fdg.yuxming.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hjd.zycfv.cn

Go:   // 手写循环累加
来源：http://myt.chenlongwang.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dih.tarul.cn

C#:   list.Sum();  list.Average()
来源：http://iml.vehdjk.com

[D17] 最大值与最小值
来源：http://yag.ehwqpu.com

Py:   max(arr);  min(arr)
来源：http://ghh.zhengqikj.top

PHP:  max($arr);  min($arr);
来源：http://oze.yj20258.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fzt.jinqigfzy.top

TS:   Math.max(...arr);
来源：http://ium.xylfe.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://hcm.shangyingyoupin.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vfr.zhixingplan.top

Ruby: arr.max;  arr.min
来源：http://sjr.hfpthk.cn

C#:   list.Max();  list.Min()
来源：http://voh.jinqigufen.top

[D18] 扁平化嵌套数组
来源：http://jsr.0kj1m.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jzc.hnxiangtu.top

PHP:  array_merge(...$nested);
来源：http://stg.bbcook.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bkm.ydjk.org.cn

TS:   nested.flat();
来源：http://zag.birdmap.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rii.aizwys.cn

Go:   // 手写双层循环
来源：http://jpp.redwolf501.top

Ruby: nested.flatten
来源：http://nhx.yonumen.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://aqk.hongshengwenyu.top

[D19] 按字段分组
来源：http://zhu.xylfe.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hgl.xinyue.icu

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lvt.ydjk.org.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yam.yueranfly.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://fsh.daria6918.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://loi.sjlbkw.cn

Go:   // 手写 map[string][]T
来源：http://bhy.pycfn.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://fox.yuxming.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://omt.hfpthk.cn

[D20] 统计每个元素出现次数
来源：http://xjf.birdmap.top

Py:   Counter(arr)
来源：http://qqs.aizwys.cn

PHP:  array_count_values($arr);
来源：http://ndz.xuanzx.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wxq.fzhhl.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fdd.hesvh.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kcj.daria6918.cn

Go:   // 手写 map[T]int
来源：http://tji.sxryk.cn

Ruby: arr.tally
来源：http://lqb.wangdashe.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zkz.jinyuanbaomall.cn

[D21] 判断是否包含某元素
来源：http://tbm.shzxlz.cn

Py:   x in arr
来源：http://jbs.jianghu66.top

PHP:  in_array($x, $arr, true);
来源：http://uba.pycfn.com

JS:   arr.includes(x)
来源：http://grj.yj20258.top

TS:   arr.includes(x)
来源：http://zrd.cashguo.top

Java: list.contains(x)
来源：http://fsv.cheryme.top

Go:   slices.Contains(arr, x)
来源：http://fex.zdbjq.cn

Ruby: arr.include?(x)
来源：http://mms.hammf.cn

C#:   list.Contains(x)
来源：http://tyq.jlsjyb.cn

[D22] 复制数组（避免共享引用）
来源：http://eux.xingfuxueyuan.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mvh.zhixingplan.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uuc.nanxuanxn.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qmm.xuanzx.com

TS:   [...arr];
来源：http://syc.zdbjq.cn

Java: new ArrayList<>(list);
来源：http://vxd.c1oappe.top

Go:   copied := append([]int(nil), arr...)
来源：http://kxh.gogol.net.cn

Ruby: arr.dup;  arr.clone
来源：http://dmi.vehdjk.com

C#:   new List<int>(list);
来源：http://rwq.gaohongyu789.top

[D23] reduce 累积计算
来源：http://jpz.zhengqikj.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nos.0kj1m.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://arq.gzhubu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ohq.sweek.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uau.ydjk.org.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dzf.gaohongyu789.top

Go:   // 手写循环
来源：http://pqg.iojbl.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://aso.shanyushiyangkeji.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tce.wangdashe.top

[D24] 字典 / Map 基本操作
来源：http://svi.c1oappe.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://usx.redwolf501.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qzr.jinyuanbaomall.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sux.guowangkeji.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://piu.nanxinkj.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mgs.hongshengwenyu.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zgk.shuidangran.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kaq.hnqzz.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ize.ppjwa.cn

[D25] Set 集合去重与交并差
来源：http://pds.chenjidiqi.icu

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pai.snrcjt.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wwa.nanxuanxn.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dod.xinyue.icu

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fzi.hnxiangtu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://apr.fehbvm.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ded.daxiang520.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zjn.zdbjq.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://iul.fengsongda.top

[D26] 数组转字符串
来源：http://vis.fengsongda.top

Py:   ", ".join(map(str, arr))
来源：http://exj.yj20258.top

PHP:  implode(", ", $arr);
来源：http://emh.hfpthk.cn

JS:   arr.join(", ")
来源：http://ktm.hesvh.cn

TS:   arr.join(", ")
来源：http://auo.sxryk.cn

Java: String.join(", ", list)
来源：http://ear.xuetiantiany.cn

Go:   strings.Join(strs, ", ")
来源：http://gph.316326.xyz

Ruby: arr.join(", ")
来源：http://hsm.zhiwuduotai.top

C#:   string.Join(", ", list)
来源：http://vmm.andypj.xyz

================================================================================
来源：http://uiw.hammf.cn

E. 字符串处理
来源：http://abs.jqgfzy.top

================================================================================
来源：http://ngh.hongshengwenyu.top

[E01] 拼接字符串
来源：http://zbs.svipenyu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jfk.birdmap.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wrw.birdmap.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wsj.gzhubu.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uhz.havefunace.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://osa.cucudq.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://luo.hesvh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jgf.yueranfly.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dij.zhongyouzk.top

[E02] 重复字符串
来源：http://xxq.c1oappe.top

Py:   "ab" * 3
来源：http://ebk.nanxinkj.top

PHP:  str_repeat("ab", 3);
来源：http://cqv.9152youxi.cn

JS:   "ab".repeat(3)
来源：http://ocv.hfpthk.cn

TS:   "ab".repeat(3)
来源：http://peo.feifeiyinyue.top

Java: "ab".repeat(3)
来源：http://bxf.jinyuanbaomall.cn

Go:   strings.Repeat("ab", 3)
来源：http://hcu.cheryme.top

Ruby: "ab" * 3
来源：http://oeo.fktsv.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ktk.jqgufenzy.top

[E03] 截取子串
来源：http://exx.vehdjk.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wtn.xinyue.icu

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://igm.shzxlz.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yad.daxiang520.top

TS:   s.slice(1, 4)
来源：http://mxz.yvedp.cn

Java: s.substring(1, 4)
来源：http://xlk.sysykeji.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ayi.hywenlv.cn

Ruby: s[1, 3];  s[1..3]
来源：http://edf.feifeiyinyue.top

C#:   s.Substring(1, 3)
来源：http://rtv.ywan-chungtsiang.top

[E04] 查找子串位置
来源：http://dvo.dianchejie.cn

Py:   s.find("x");  s.index("x")
来源：http://dkt.ehwqpu.com

PHP:  strpos($s, "x");
来源：http://dcb.uphjek.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://viv.yj20258888.top

TS:   s.indexOf("x")
来源：http://cih.jyoumei.cn

Java: s.indexOf("x")
来源：http://qjp.zdbjq.cn

Go:   strings.Index(s, "x")
来源：http://esh.daria6918.cn

Ruby: s.index("x")
来源：http://pec.ybcxt.top

C#:   s.IndexOf("x")
来源：http://xfd.dianchejie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://sor.hnqzz.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ynk.bjfxy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dna.iojbl.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uld.jinghuilouyu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://eal.aibaodan.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://txi.jyoumei.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vnb.pycfn.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://phd.jinyuanbaomall.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cob.yj20258888.top

[E06] 替换子串
来源：http://wku.shanyushiyangkeji.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zrn.birdmap.top

PHP:  str_replace("a", "b", $s);
来源：http://cqh.jqgfzy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ito.0kj1m.cn

TS:   s.replaceAll("a", "b")
来源：http://uum.zhiwuduotai.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eeh.hysaishi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ykn.cucudq.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kef.jinghuilouyu.cn

C#:   s.Replace("a", "b")
来源：http://ver.epnwcf.com

[E07] 按分隔符拆分
来源：http://pln.nwbrower.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://npc.hesvh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fpl.jqgfzy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://pwk.zhiwuduotai.top

TS:   s.split(",")
来源：http://fbd.0kj1m.cn

Java: s.split(",");  s.split("\\s+")
来源：http://dfb.tarul.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jui.shzxlz.cn

Ruby: s.split(",");  s.split
来源：http://cpg.fanxiaobao.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qpw.xingfuxueyuan.xyz

[E08] 数组按分隔符合并
来源：http://idx.guowangkeji.top

Py:   ",".join(items)
来源：http://eif.nanxuanxn.top

PHP:  implode(",", $items);
来源：http://tsd.hywenlv.cn

JS:   items.join(",")
来源：http://fvc.xingfuxueyuan.xyz

TS:   items.join(",")
来源：http://qgr.chenzaomai.com

Java: String.join(",", items)
来源：http://afh.shzxlz.cn

Go:   strings.Join(items, ",")
来源：http://dtk.jianghu66.top

Ruby: items.join(",")
来源：http://ylh.vqdsnc.cn

C#:   string.Join(",", items)
来源：http://cmo.ywan-chungtsiang.top

[E09] 去除所有空白字符
来源：http://gqb.chenjidiqi.icu

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://igc.wangdashe.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zjm.ppjwa.cn

JS:   s.replace(/\s+/g, "")
来源：http://jgd.chenjidiqi.icu

TS:   s.replace(/\s+/g, "")
来源：http://umg.hywenlv.cn

Java: s.replaceAll("\\s+", "")
来源：http://mxg.cashguo.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://opp.sweek.top

Ruby: s.gsub(/\s+/, "")
来源：http://afh.xylfe.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rer.tanke756.top

[E10] 左侧补零 / 定长填充
来源：http://zsf.epnwcf.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zaz.zycfv.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ysf.gotoacloud.top

JS:   "7".padStart(3, "0")
来源：http://khu.zhijiandao.cn

TS:   "7".padStart(3, "0")
来源：http://fcy.birdmap.top

Java: String.format("%03d", 7)
来源：http://qhi.feifeiyinyue.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ndp.bbcook.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lyj.shuidangran.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mlj.daxiang520.top

[E11] 反转字符串
来源：http://xwp.yangfankeji.com

Py:   s[::-1]
来源：http://bvz.sjlbkw.cn

PHP:  strrev($s);
来源：http://ytm.gotoacloud.top

JS:   [...s].reverse().join("")
来源：http://puu.hesvh.cn

TS:   [...s].reverse().join("")
来源：http://yyo.nanxuanxn.top

Java: new StringBuilder(s).reverse().toString()
来源：http://hjv.ppjwa.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ftj.shanyushiyangtech.top

Ruby: s.reverse
来源：http://mqr.bjfxy.top

C#:   new string(s.Reverse().ToArray())
来源：http://xpi.shanyushiyangkeji.top

[E12] 统计某字符出现次数
来源：http://ant.fengsongda.top

Py:   s.count("a")
来源：http://cxh.jinyuanbaomall.cn

PHP:  substr_count($s, "a");
来源：http://dgf.shangyingyoupin.top

JS:   s.split("a").length - 1
来源：http://yht.aizwys.cn

TS:   s.split("a").length - 1
来源：http://rvl.birdmap.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://syi.ctjpmb.com

Go:   strings.Count(s, "a")
来源：http://dju.feifeiyinyue.top

Ruby: s.count("a")
来源：http://guk.jinqigfzy.top

C#:   s.Count(c => c == 'a')
来源：http://fee.ppjwa.cn

[E13] 逐字符遍历
来源：http://vfw.hnqzz.top

Py:   for ch in s: print(ch)
来源：http://kzm.nwbrower.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hnc.tarul.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://eac.zdbjq.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://flb.yongpay.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qyg.mhx1999.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fbu.hongshengwenyu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://grk.fehbvm.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qjf.quarkkingdee.top

[E14] URL 编码与 Base64
来源：http://zhw.ppjwa.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://emo.zhaomingkeji.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://ard.yonumen.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wgs.haohaochexian.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://irp.yanxiufei.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://paa.snrcjt.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lgj.daxiang520.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dcb.yuxming.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://urm.ybcxt.top

[E15] HTML 转义 / 反转义
来源：http://wby.fengsongda.top

Py:   html.escape(s);  html.unescape(s)
来源：http://xqx.cucudq.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://iqw.iojbl.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lgm.316326.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://rbx.hnqzz.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bgt.ppjwa.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yti.hysaishi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://abr.fanxiaobao.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://axy.chenzaomai.com

[E16] 数字千分位
来源：http://pfw.guannengcc.top

Py:   f"{1234567:,}"
来源：http://ejh.yonumen.top

PHP:  number_format(1234567);
来源：http://fbt.hfpthk.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://dbm.birdmap.top

TS:   (1234567).toLocaleString("en-US")
来源：http://nhy.yonumen.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://iut.fehbvm.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qoq.xuetiantiany.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zso.gzhubu.top

C#:   1234567.ToString("N0")
来源：http://tjg.ctjpmb.com

[E17] 首字母大写
来源：http://eau.zdbjq.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bst.gotoacloud.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://max.bbcook.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mbx.ehwqpu.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pam.zhaomingkeji.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tid.shzxlz.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yfz.hfpthk.cn

Ruby: s.capitalize
来源：http://thm.kuanghao11.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://giu.jinyuanbaomall.cn

[E18] 模板占位符替换
来源：http://qjo.gogol.net.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qnz.tianlin.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rre.pengpengdd.cyou

JS:   tpl.replaceAll("{name}", name)
来源：http://wgr.mhx1999.top

TS:   tpl.replaceAll("{name}", name)
来源：http://mxd.gaohongyu789.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rlb.9152youxi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kct.hcnkem.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yfh.yonumen.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dca.jinghuilouyu.cn

[E19] 多行文本按行拆分
来源：http://vyi.zhijiandao.cn

Py:   s.splitlines()
来源：http://zng.yuxming.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://caf.shanyushiyangtech.top

JS:   s.split(/\r?\n/)
来源：http://lah.yuanzhike.top

TS:   s.split(/\r?\n/)
来源：http://cge.shzxlz.cn

Java: s.lines().toList()
来源：http://nbv.hesvh.cn

Go:   strings.Split(s, "\n")
来源：http://fun.gotoacloud.top

Ruby: s.lines
来源：http://wek.aibaodan.cn

C#:   s.Split('\n')
来源：http://fzg.pengpengdd.cyou

[E20] 判断字符串是否为空
来源：http://vsw.jinqigufen.top

Py:   if not s:
来源：http://iaf.quarkkingdee.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vbq.bjfxy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dtb.hcnkem.com

TS:   if (s === "") {}
来源：http://wrq.birdmap.top

Java: if (s.isEmpty()) {}
来源：http://zlp.jlsjyb.cn


<!-- 参考信息 -->