代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://aek.ehwqpu.com

JS:   arr.filter(x => x > 3)
来源：http://xzu.shuidangran.top

TS:   arr.filter(x => x > 3)
来源：http://aie.gotoacloud.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dha.jinqigufen.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lnl.zhengqikj.top

Ruby: arr.select { |x| x > 3 }
来源：http://vfb.kuanghao11.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://rnk.uphjek.com

[D14] 映射转换（每个元素变形）
来源：http://zie.chenzaomai.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yan.hywenlv.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hqz.mhx1999.top

JS:   arr.map(x => x * 2)
来源：http://gbf.pengpengdd.cyou

TS:   arr.map(x => x * 2)
来源：http://emn.yangfankeji.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://jlt.yangfankeji.com

Go:   // 手写循环
来源：http://lwb.fengsongda.top

Ruby: arr.map { |x| x * 2 }
来源：http://ayq.bbcook.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://skq.hcnkem.com

[D15] 去重
来源：http://ytr.ehwqpu.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oih.tarul.cn

PHP:  array_unique($arr);
来源：http://xiz.gzhubu.top

JS:   [...new Set(arr)]
来源：http://mxv.snrcjt.cn

TS:   [...new Set(arr)]
来源：http://frn.ybcxt.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zle.nanxinkj.top

Go:   // 用 map[T]struct{} 手写
来源：http://awg.ywan-chungtsiang.top

Ruby: arr.uniq
来源：http://mac.yj202588.top

C#:   list.Distinct().ToList()
来源：http://umv.vqdsnc.cn

[D16] 求和与平均值
来源：http://tnp.xuanzx.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nui.andypj.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://poc.jinqigufen.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wfl.daxiang520.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lji.sweek.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sss.gzhubu.top

Go:   // 手写循环累加
来源：http://sxf.ppjwa.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kis.gzhubu.top

C#:   list.Sum();  list.Average()
来源：http://jbz.aizwys.cn

[D17] 最大值与最小值
来源：http://zyk.ppjwa.cn

Py:   max(arr);  min(arr)
来源：http://pnr.chenlongwang.top

PHP:  max($arr);  min($arr);
来源：http://ggd.xziqi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ftk.cqqwz.cn

TS:   Math.max(...arr);
来源：http://aef.svipenyu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gkb.fanxiaobao.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fwa.andypj.xyz

Ruby: arr.max;  arr.min
来源：http://dcv.yangfankeji.com

C#:   list.Max();  list.Min()
来源：http://ioa.ydjk.org.cn

[D18] 扁平化嵌套数组
来源：http://haj.0kj1m.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lqp.nwbrower.top

PHP:  array_merge(...$nested);
来源：http://jex.daria6918.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://job.gogol.net.cn

TS:   nested.flat();
来源：http://bps.yuanzhike.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://oeu.ppjwa.cn

Go:   // 手写双层循环
来源：http://uyz.zdbjq.cn

Ruby: nested.flatten
来源：http://txs.uphjek.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://lfo.gzhubu.top

[D19] 按字段分组
来源：http://znf.andypj.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bep.hnqzz.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ndf.bbcook.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qps.zhixingplan.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ipf.zhijiandao.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fhi.0kj1m.cn

Go:   // 手写 map[string][]T
来源：http://ekz.zdbjq.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bqr.52xcode.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cki.aibaodan.cn

[D20] 统计每个元素出现次数
来源：http://hoi.uphjek.com

Py:   Counter(arr)
来源：http://aas.chenjidiqi.icu

PHP:  array_count_values($arr);
来源：http://qpt.0kj1m.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oqc.fehbvm.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ife.hesvh.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ukv.tian-w.cn

Go:   // 手写 map[T]int
来源：http://zvu.fehbvm.com

Ruby: arr.tally
来源：http://mgx.yvedp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wub.yuxming.cn

[D21] 判断是否包含某元素
来源：http://cvx.zhengqikj.top

Py:   x in arr
来源：http://wuw.hongshengwenyu.top

PHP:  in_array($x, $arr, true);
来源：http://cal.fehbvm.com

JS:   arr.includes(x)
来源：http://pcr.sufxvd.cn

TS:   arr.includes(x)
来源：http://nst.jinqigfzy.top

Java: list.contains(x)
来源：http://tie.ehwqpu.com

Go:   slices.Contains(arr, x)
来源：http://yyh.xinyue.icu

Ruby: arr.include?(x)
来源：http://qld.svipenyu.cn

C#:   list.Contains(x)
来源：http://osw.cucudq.cn

[D22] 复制数组（避免共享引用）
来源：http://arr.gotoacloud.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rme.guowangkeji.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wjs.meibo888.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ppf.fanxiaobao.xyz

TS:   [...arr];
来源：http://wcn.jinqigufen.top

Java: new ArrayList<>(list);
来源：http://vkt.vehdjk.com

Go:   copied := append([]int(nil), arr...)
来源：http://nmq.yfazqb.com

Ruby: arr.dup;  arr.clone
来源：http://prp.quarkkingdee.top

C#:   new List<int>(list);
来源：http://xvl.ydzc1.top

[D23] reduce 累积计算
来源：http://ymm.jinyuanbaomall.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pbg.zdqjudy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zay.ydjk.org.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zlj.tianlin.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pfc.mhx1999.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://amc.jqgfzy.top

Go:   // 手写循环
来源：http://cir.jlsjyb.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lek.xinyue.icu

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ems.zhiwuduotai.top

[D24] 字典 / Map 基本操作
来源：http://egt.shanyushiyangtech.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dvv.tianlin.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ojy.jinqigfzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mgx.haohaochexian.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jqq.uphjek.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pmj.sjlbkw.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lud.nwbrower.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dia.sysykeji.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tvv.tian-w.cn

[D25] Set 集合去重与交并差
来源：http://iuu.hywenlv.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nel.havefunace.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hrl.52xcode.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://coz.xziqi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cbx.nwbrower.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://usi.tanke756.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jee.yueranfly.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dmm.epnwcf.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kgf.jinghuilouyu.cn

[D26] 数组转字符串
来源：http://pam.tian-w.cn

Py:   ", ".join(map(str, arr))
来源：http://wzg.fengsongda.top

PHP:  implode(", ", $arr);
来源：http://suz.dashuyun.cn

JS:   arr.join(", ")
来源：http://xyo.epnwcf.com

TS:   arr.join(", ")
来源：http://wkm.kuanghao11.cn

Java: String.join(", ", list)
来源：http://yke.xuanzx.com

Go:   strings.Join(strs, ", ")
来源：http://szt.fktsv.cn

Ruby: arr.join(", ")
来源：http://jxp.guannengcc.top

C#:   string.Join(", ", list)
来源：http://rvd.pycfn.com

================================================================================
来源：http://jso.ydzc1.top

E. 字符串处理
来源：http://udu.shanyushiyangkeji.top

================================================================================
来源：http://nek.aizwys.cn

[E01] 拼接字符串
来源：http://uev.hcnkem.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bjl.fanxiaobao.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bsa.yuanzhike.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bbx.yj202588.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dtc.pycfn.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vmc.zhixingplan.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bhd.gzhubu.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ggz.yuxming.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cue.yfazqb.com

[E02] 重复字符串
来源：http://wgx.fanxiaobao.xyz

Py:   "ab" * 3
来源：http://pfn.hcnkem.com

PHP:  str_repeat("ab", 3);
来源：http://qxg.shangyingyoupin.top

JS:   "ab".repeat(3)
来源：http://aim.hywenlv.cn

TS:   "ab".repeat(3)
来源：http://pvx.hesvh.cn

Java: "ab".repeat(3)
来源：http://jjd.ydjk.org.cn

Go:   strings.Repeat("ab", 3)
来源：http://krt.yfazqb.com

Ruby: "ab" * 3
来源：http://crk.yuxming.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ofd.dianchejie.cn

[E03] 截取子串
来源：http://eop.ywan-chungtsiang.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://aqo.ehwqpu.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kto.dashuyun.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vpy.sysykeji.top

TS:   s.slice(1, 4)
来源：http://mnx.aizwys.cn

Java: s.substring(1, 4)
来源：http://bjo.zdbjq.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cyv.sysykeji.top

Ruby: s[1, 3];  s[1..3]
来源：http://vxh.jqgfzy.top

C#:   s.Substring(1, 3)
来源：http://rbi.xinyue.icu

[E04] 查找子串位置
来源：http://vdg.feifeiyinyue.top

Py:   s.find("x");  s.index("x")
来源：http://koa.nwbrower.top

PHP:  strpos($s, "x");
来源：http://swt.chenzaomai.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vvq.fktsv.cn

TS:   s.indexOf("x")
来源：http://ruo.fengsongda.top

Java: s.indexOf("x")
来源：http://ayq.wangshuangyany.cn

Go:   strings.Index(s, "x")
来源：http://rsn.birdmap.top

Ruby: s.index("x")
来源：http://esg.hcnkem.com

C#:   s.IndexOf("x")
来源：http://pef.fanxiaobao.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://nch.jiagoushi.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zss.hnqzz.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pit.yueranfly.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tjm.52xcode.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ryq.shangyingyoupin.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bli.tian-w.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tzb.zhongyouzk.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://taa.bjfxy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wjk.yangfankeji.com

[E06] 替换子串
来源：http://xvm.ydjk.org.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://iak.yj20258888.top

PHP:  str_replace("a", "b", $s);
来源：http://gbg.hnxiangtu.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wvb.xuanzx.com

TS:   s.replaceAll("a", "b")
来源：http://yfe.shanyushiyangtech.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cxk.chenjidiqi.icu

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://juu.c1oappe.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hll.shzxlz.cn

C#:   s.Replace("a", "b")
来源：http://ldd.shanyushiyangtech.top

[E07] 按分隔符拆分
来源：http://xps.hysaishi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ytq.cdnleiting.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yvr.nanxinkj.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://spx.feifeiyinyue.top

TS:   s.split(",")
来源：http://qir.snrcjt.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vli.hcnkem.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jga.wangdashe.top

Ruby: s.split(",");  s.split
来源：http://vpi.tarul.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kfm.vqdsnc.cn

[E08] 数组按分隔符合并
来源：http://bmb.ybcxt.top

Py:   ",".join(items)
来源：http://nav.yanxiufei.cn

PHP:  implode(",", $items);
来源：http://syz.c1oappe.top

JS:   items.join(",")
来源：http://cjp.9152youxi.cn

TS:   items.join(",")
来源：http://nfz.shzxlz.cn

Java: String.join(",", items)
来源：http://iox.wangdashe.top

Go:   strings.Join(items, ",")
来源：http://oaz.pengpengdd.cyou

Ruby: items.join(",")
来源：http://wbi.hywenlv.cn

C#:   string.Join(",", items)
来源：http://kcn.fktsv.cn

[E09] 去除所有空白字符
来源：http://dnq.cashguo.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://uve.iojbl.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ykv.cdnleiting.top

JS:   s.replace(/\s+/g, "")
来源：http://hue.shuidangran.top

TS:   s.replace(/\s+/g, "")
来源：http://qaz.feifeiyinyue.top

Java: s.replaceAll("\\s+", "")
来源：http://fwi.shanyushiyangkeji.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://dov.quarkkingdee.top

Ruby: s.gsub(/\s+/, "")
来源：http://osj.tanke756.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pmi.hesvh.cn

[E10] 左侧补零 / 定长填充
来源：http://rwd.jinyuanbaomall.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sxj.hfpthk.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ivf.yj20258.top

JS:   "7".padStart(3, "0")
来源：http://poi.yvedp.cn

TS:   "7".padStart(3, "0")
来源：http://met.yuxming.cn

Java: String.format("%03d", 7)
来源：http://iat.bjfxy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://vbf.nwbrower.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://orb.hfpthk.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://eii.0kj1m.cn

[E11] 反转字符串
来源：http://ide.hfpthk.cn

Py:   s[::-1]
来源：http://stv.yongpay.top

PHP:  strrev($s);
来源：http://wnw.zhoulong.xyz

JS:   [...s].reverse().join("")
来源：http://fvv.sxryk.cn

TS:   [...s].reverse().join("")
来源：http://xji.haohaochexian.top

Java: new StringBuilder(s).reverse().toString()
来源：http://fvg.fanxiaobao.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://nuh.cucudq.cn

Ruby: s.reverse
来源：http://siy.andypj.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://emv.xingfuxueyuan.xyz

[E12] 统计某字符出现次数
来源：http://rke.hywenlv.cn

Py:   s.count("a")
来源：http://xhs.daxiang520.top

PHP:  substr_count($s, "a");
来源：http://wnb.ivvv.top

JS:   s.split("a").length - 1
来源：http://mjh.shuidangran.top

TS:   s.split("a").length - 1
来源：http://hgg.meibo888.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://equ.hfpthk.cn

Go:   strings.Count(s, "a")
来源：http://zej.kuanghao11.cn

Ruby: s.count("a")
来源：http://kah.xingfuxueyuan.xyz

C#:   s.Count(c => c == 'a')
来源：http://ehj.vehdjk.com

[E13] 逐字符遍历
来源：http://ymz.hnxiangtu.top

Py:   for ch in s: print(ch)
来源：http://tgm.gotoacloud.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cjs.yonumen.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ywd.birdmap.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://lgx.shanyushiyangtech.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zwy.iojbl.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pps.zhixingplan.top

Ruby: s.each_char { |ch| puts ch }
来源：http://tbc.316326.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fvl.zhongyouzk.top

[E14] URL 编码与 Base64
来源：http://ufh.52xcode.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://oqm.jyoumei.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ddh.316326.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://twr.cashguo.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://oho.pycfn.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xyq.yongpay.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ajr.zhongyouzk.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://aai.9152youxi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://uat.sufxvd.cn

[E15] HTML 转义 / 反转义
来源：http://ukn.sweek.top

Py:   html.escape(s);  html.unescape(s)
来源：http://bre.9152youxi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://iho.dashuyun.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hlu.zhongyouzk.top

TS:   // 同上，务必做 XSS 过滤
来源：http://mmd.vqdsnc.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://aqe.fzhhl.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dus.havefunace.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jdd.iojbl.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xpt.cucudq.cn

[E16] 数字千分位
来源：http://mwk.jinyuanbaomall.cn

Py:   f"{1234567:,}"
来源：http://ugo.xuanzx.com

PHP:  number_format(1234567);
来源：http://nej.nanxuanxn.top

JS:   (1234567).toLocaleString("en-US")
来源：http://uam.cashguo.top

TS:   (1234567).toLocaleString("en-US")
来源：http://kyf.zdqjudy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://raa.zhixingplan.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xgb.guowangkeji.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ykx.hfpthk.cn

C#:   1234567.ToString("N0")
来源：http://lom.vqdsnc.cn

[E17] 首字母大写
来源：http://wzt.xuetiantiany.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nnh.chenzaomai.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://ngj.mhx1999.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qni.tianlin.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kyu.yuanzhike.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ubc.hnxiangtu.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://myn.yuxming.cn

Ruby: s.capitalize
来源：http://ory.guannengcc.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pil.jyoumei.cn

[E18] 模板占位符替换
来源：http://ili.jqgfzy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yrw.daria6918.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://snb.xinyue.icu

JS:   tpl.replaceAll("{name}", name)
来源：http://hxc.yonumen.top

TS:   tpl.replaceAll("{name}", name)
来源：http://nbh.xuetiantiany.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lxc.316326.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lkf.tanke756.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bpe.jinqigfzy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gpd.tanke756.top

[E19] 多行文本按行拆分
来源：http://xhg.hfpthk.cn

Py:   s.splitlines()
来源：http://jal.xuetiantiany.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://csm.cheryme.top

JS:   s.split(/\r?\n/)
来源：http://ktv.jinghuilouyu.cn

TS:   s.split(/\r?\n/)
来源：http://gty.cheryme.top

Java: s.lines().toList()
来源：http://khn.sufxvd.cn

Go:   strings.Split(s, "\n")
来源：http://pwh.fengsongda.top

Ruby: s.lines
来源：http://tfq.xuanzx.com

C#:   s.Split('\n')
来源：http://znm.zhaomingkeji.xyz

[E20] 判断字符串是否为空
来源：http://cgu.cucudq.cn

Py:   if not s:
来源：http://csq.chenzaomai.com


<!-- 参考信息 -->