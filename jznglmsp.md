代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://sal.vqdsnc.cn

Go:   // 手写循环
来源：http://aan.yuxming.cn

Ruby: arr.map { |x| x * 2 }
来源：http://kjz.316326.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://tbl.fehbvm.com

[D15] 去重
来源：http://kvu.meibo888.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gqa.hnxiangtu.top

PHP:  array_unique($arr);
来源：http://nzs.fengsongda.top

JS:   [...new Set(arr)]
来源：http://hfd.nwbrower.top

TS:   [...new Set(arr)]
来源：http://xjy.shuidangran.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uhx.haohaochexian.top

Go:   // 用 map[T]struct{} 手写
来源：http://pwp.cucudq.cn

Ruby: arr.uniq
来源：http://fzq.shanyushiyangkeji.top

C#:   list.Distinct().ToList()
来源：http://mkh.316326.xyz

[D16] 求和与平均值
来源：http://whe.sysykeji.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zae.9152youxi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://psj.shanyushiyangtech.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://eto.hnxiangtu.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gsi.zdqjudy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nml.jiagoushi.top

Go:   // 手写循环累加
来源：http://yta.ywan-chungtsiang.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://phn.kuanghao11.cn

C#:   list.Sum();  list.Average()
来源：http://hms.hongshengwenyu.top

[D17] 最大值与最小值
来源：http://uzl.zhaomingkeji.xyz

Py:   max(arr);  min(arr)
来源：http://yev.meibo888.top

PHP:  max($arr);  min($arr);
来源：http://kpi.dashuyun.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ihy.shanyushiyangtech.top

TS:   Math.max(...arr);
来源：http://feb.havefunace.top

Java: Collections.max(list);  Collections.min(list);
来源：http://egw.jianghu66.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jjq.epnwcf.com

Ruby: arr.max;  arr.min
来源：http://iqx.nwbrower.top

C#:   list.Max();  list.Min()
来源：http://gph.hnqzz.top

[D18] 扁平化嵌套数组
来源：http://qkl.snrcjt.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gkw.daria6918.cn

PHP:  array_merge(...$nested);
来源：http://vho.zhengqikj.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dld.tian-w.cn

TS:   nested.flat();
来源：http://cos.xuanzx.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jap.cucudq.cn

Go:   // 手写双层循环
来源：http://srp.0kj1m.cn

Ruby: nested.flatten
来源：http://fkb.jlsjyb.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xwg.andypj.xyz

[D19] 按字段分组
来源：http://eqc.fengsongda.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://und.hfpthk.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fte.cashguo.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tnh.gzhubu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://gkj.yj20258.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://eag.dianchejie.cn

Go:   // 手写 map[string][]T
来源：http://rgo.fehbvm.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://zxv.sweek.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mfy.dashuyun.cn

[D20] 统计每个元素出现次数
来源：http://vfz.fanxiaobao.xyz

Py:   Counter(arr)
来源：http://kmg.smart0.xyz

PHP:  array_count_values($arr);
来源：http://xbs.ywan-chungtsiang.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://doe.chenlongwang.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xjt.guowangkeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bmu.yj20258.top

Go:   // 手写 map[T]int
来源：http://sro.hammf.cn

Ruby: arr.tally
来源：http://qke.yj20258888.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rbw.yfazqb.com

[D21] 判断是否包含某元素
来源：http://gux.shanyushiyangtech.top

Py:   x in arr
来源：http://cht.xylfe.cn

PHP:  in_array($x, $arr, true);
来源：http://riq.tanke756.top

JS:   arr.includes(x)
来源：http://ima.jinqigfzy.top

TS:   arr.includes(x)
来源：http://hou.wangdashe.top

Java: list.contains(x)
来源：http://pil.havefunace.top

Go:   slices.Contains(arr, x)
来源：http://jsy.shanyushiyangkeji.top

Ruby: arr.include?(x)
来源：http://xqo.cucudq.cn

C#:   list.Contains(x)
来源：http://xni.yongpay.top

[D22] 复制数组（避免共享引用）
来源：http://roj.ivvv.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wpl.havefunace.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xla.gaohongyu789.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://scz.c1oappe.top

TS:   [...arr];
来源：http://xfm.chenzaomai.com

Java: new ArrayList<>(list);
来源：http://fev.jinyuanbaomall.cn

Go:   copied := append([]int(nil), arr...)
来源：http://uhb.hfpthk.cn

Ruby: arr.dup;  arr.clone
来源：http://rol.fengsongda.top

C#:   new List<int>(list);
来源：http://hhf.vehdjk.com

[D23] reduce 累积计算
来源：http://tsb.fehbvm.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bny.chenzaomai.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vis.jlsjyb.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zgp.dianchejie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ytj.redwolf501.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://oor.meibo888.top

Go:   // 手写循环
来源：http://bho.wangdashe.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qic.yfazqb.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fvw.yangfankeji.com

[D24] 字典 / Map 基本操作
来源：http://hry.ivvv.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xga.bbcook.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mgm.zhengqikj.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wak.hnqzz.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yky.tianlin.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ito.fktsv.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ugb.meibo888.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vwq.nanxinkj.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nae.daria6918.cn

[D25] Set 集合去重与交并差
来源：http://shj.aizwys.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qkt.jqgufenzy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gkf.sjlbkw.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ntl.yuxming.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tws.jinghuilouyu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wtm.pycfn.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ftt.sweek.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dvi.ydzc1.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hmj.zdbjq.cn

[D26] 数组转字符串
来源：http://dwn.havefunace.top

Py:   ", ".join(map(str, arr))
来源：http://uan.zdqjudy.top

PHP:  implode(", ", $arr);
来源：http://bgu.sweek.top

JS:   arr.join(", ")
来源：http://jxa.xuanzx.com

TS:   arr.join(", ")
来源：http://jpi.uphjek.com

Java: String.join(", ", list)
来源：http://gfg.hysaishi.cn

Go:   strings.Join(strs, ", ")
来源：http://hyo.fzhhl.top

Ruby: arr.join(", ")
来源：http://yva.9152youxi.cn

C#:   string.Join(", ", list)
来源：http://www.fengsongda.top

================================================================================
来源：http://ggj.jlsjyb.cn

E. 字符串处理
来源：http://axl.shanyushiyangkeji.top

================================================================================
来源：http://lyj.vehdjk.com

[E01] 拼接字符串
来源：http://yie.pycfn.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mjb.ybcxt.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uhk.ppjwa.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ruz.snrcjt.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://quq.cqqwz.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gjm.jinqigufen.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qwu.aizwys.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gan.yvedp.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://imq.wangshuangyany.cn

[E02] 重复字符串
来源：http://tff.sxryk.cn

Py:   "ab" * 3
来源：http://zxt.shangyingyoupin.top

PHP:  str_repeat("ab", 3);
来源：http://rza.tianlin.xyz

JS:   "ab".repeat(3)
来源：http://tqv.daria6918.cn

TS:   "ab".repeat(3)
来源：http://evm.shangyingyoupin.top

Java: "ab".repeat(3)
来源：http://wyn.zhengqikj.top

Go:   strings.Repeat("ab", 3)
来源：http://jmr.hnqzz.top

Ruby: "ab" * 3
来源：http://nom.iojbl.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jyy.c1oappe.top

[E03] 截取子串
来源：http://nwt.yanxiufei.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://loi.cashguo.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://eow.epnwcf.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ltu.c1oappe.top

TS:   s.slice(1, 4)
来源：http://jkg.zycfv.cn

Java: s.substring(1, 4)
来源：http://zxl.cdnleiting.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lye.gzhubu.top

Ruby: s[1, 3];  s[1..3]
来源：http://rcb.c1oappe.top

C#:   s.Substring(1, 3)
来源：http://snk.jiagoushi.top

[E04] 查找子串位置
来源：http://ukg.shanyushiyangtech.top

Py:   s.find("x");  s.index("x")
来源：http://gut.zhiwuduotai.top

PHP:  strpos($s, "x");
来源：http://rmu.shangyingyoupin.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rbe.birdmap.top

TS:   s.indexOf("x")
来源：http://tmf.feifeiyinyue.top

Java: s.indexOf("x")
来源：http://iql.havefunace.top

Go:   strings.Index(s, "x")
来源：http://aqw.jinyuanbaomall.cn

Ruby: s.index("x")
来源：http://piu.zycfv.cn

C#:   s.IndexOf("x")
来源：http://tqr.sysykeji.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://wde.jiagoushi.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xko.wangshuangyany.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ndv.haohaochexian.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qfu.epnwcf.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://inm.chenzaomai.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://btz.sweek.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ktp.ctjpmb.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fhc.zhiwuduotai.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ojn.tian-w.cn

[E06] 替换子串
来源：http://vvo.ctjpmb.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ilx.zycfv.cn

PHP:  str_replace("a", "b", $s);
来源：http://rde.birdmap.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jst.andypj.xyz

TS:   s.replaceAll("a", "b")
来源：http://isa.fanxiaobao.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ecp.shzxlz.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cml.guowangkeji.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://uwv.snrcjt.cn

C#:   s.Replace("a", "b")
来源：http://kxj.hongshengwenyu.top

[E07] 按分隔符拆分
来源：http://nma.redwolf501.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ynb.zhongyouzk.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ywy.vqdsnc.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rbf.sysykeji.top

TS:   s.split(",")
来源：http://fbe.nwbrower.top

Java: s.split(",");  s.split("\\s+")
来源：http://kvw.wangdashe.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zvx.jlsjyb.cn

Ruby: s.split(",");  s.split
来源：http://bza.redwolf501.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://weh.bbcook.cn

[E08] 数组按分隔符合并
来源：http://avr.gogol.net.cn

Py:   ",".join(items)
来源：http://cim.pengpengdd.cyou

PHP:  implode(",", $items);
来源：http://xul.guannengcc.top

JS:   items.join(",")
来源：http://gex.ywan-chungtsiang.top

TS:   items.join(",")
来源：http://lvi.chenjidiqi.icu

Java: String.join(",", items)
来源：http://qzy.zhiwuduotai.top

Go:   strings.Join(items, ",")
来源：http://klb.fengsongda.top

Ruby: items.join(",")
来源：http://aic.jinghuilouyu.cn

C#:   string.Join(",", items)
来源：http://ffx.vqdsnc.cn

[E09] 去除所有空白字符
来源：http://pio.haohaochexian.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://umj.hesvh.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vxa.zhixingplan.top

JS:   s.replace(/\s+/g, "")
来源：http://yjq.nanxinkj.top

TS:   s.replace(/\s+/g, "")
来源：http://eha.redwolf501.top

Java: s.replaceAll("\\s+", "")
来源：http://wyb.tarul.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xwh.fktsv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gdc.ywan-chungtsiang.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xbw.gaohongyu789.top

[E10] 左侧补零 / 定长填充
来源：http://jkv.wangshuangyany.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tou.svipenyu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lml.vqdsnc.cn

JS:   "7".padStart(3, "0")
来源：http://jaw.chenjidiqi.icu

TS:   "7".padStart(3, "0")
来源：http://wcn.ivvv.top

Java: String.format("%03d", 7)
来源：http://tqw.shzxlz.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://jbd.daria6918.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hhn.fanxiaobao.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ihr.9152youxi.cn

[E11] 反转字符串
来源：http://tid.yuxming.cn

Py:   s[::-1]
来源：http://sgq.sweek.top

PHP:  strrev($s);
来源：http://ixa.tarul.cn

JS:   [...s].reverse().join("")
来源：http://kfe.jiagoushi.top

TS:   [...s].reverse().join("")
来源：http://pit.tanke756.top

Java: new StringBuilder(s).reverse().toString()
来源：http://fdv.ehwqpu.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://roc.jinqigufen.top

Ruby: s.reverse
来源：http://bsi.zdbjq.cn

C#:   new string(s.Reverse().ToArray())
来源：http://cjj.vqdsnc.cn

[E12] 统计某字符出现次数
来源：http://uyy.xylfe.cn

Py:   s.count("a")
来源：http://ehc.tarul.cn

PHP:  substr_count($s, "a");
来源：http://bca.bbcook.cn

JS:   s.split("a").length - 1
来源：http://fho.yj202588.top

TS:   s.split("a").length - 1
来源：http://hiy.andypj.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jja.feifeiyinyue.top

Go:   strings.Count(s, "a")
来源：http://tdt.epnwcf.com

Ruby: s.count("a")
来源：http://zvl.xylfe.cn

C#:   s.Count(c => c == 'a')
来源：http://fyl.nwbrower.top

[E13] 逐字符遍历
来源：http://cfy.ydjk.org.cn

Py:   for ch in s: print(ch)
来源：http://cgj.yj20258.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wez.uphjek.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://iny.jlsjyb.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://miq.wangdashe.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sxc.fengsongda.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nia.daxiang520.top

Ruby: s.each_char { |ch| puts ch }
来源：http://uwf.xingfuxueyuan.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cbt.cdnleiting.top

[E14] URL 编码与 Base64
来源：http://umu.chenzaomai.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pqf.yj20258888.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ikl.tianlin.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gnz.dashuyun.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rhb.jyoumei.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://agu.tanke756.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tif.0kj1m.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mwv.0kj1m.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ndb.jinyuanbaomall.cn

[E15] HTML 转义 / 反转义
来源：http://uok.nwbrower.top

Py:   html.escape(s);  html.unescape(s)
来源：http://uki.hysaishi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wmg.xinyue.icu

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cms.gogol.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://rqf.wangshuangyany.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://idd.zdbjq.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mjo.dashuyun.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://idd.cucudq.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vwb.jinghuilouyu.cn

[E16] 数字千分位
来源：http://jkj.hnxiangtu.top

Py:   f"{1234567:,}"
来源：http://pgx.jinghuilouyu.cn

PHP:  number_format(1234567);
来源：http://zfv.sxryk.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gaa.yvedp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://uni.hongshengwenyu.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fut.mhx1999.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zpo.fanxiaobao.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xum.yj20258.top

C#:   1234567.ToString("N0")
来源：http://wjr.fehbvm.com

[E17] 首字母大写
来源：http://pjc.gogol.net.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://swe.pycfn.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://ejs.chenzaomai.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://emm.guannengcc.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dfd.haohaochexian.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dad.sufxvd.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lyo.iojbl.cn

Ruby: s.capitalize
来源：http://qnb.wangdashe.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tpz.sxryk.cn

[E18] 模板占位符替换
来源：http://oxe.tanke756.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sgy.hcnkem.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gci.zhongyouzk.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ccv.cucudq.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hmk.zhongyouzk.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wyt.xuanzx.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xhu.redwolf501.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://diz.havefunace.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://can.sufxvd.cn

[E19] 多行文本按行拆分
来源：http://xhx.tian-w.cn

Py:   s.splitlines()
来源：http://cig.sweek.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qka.yuanzhike.top

JS:   s.split(/\r?\n/)
来源：http://irj.nanxuanxn.top

TS:   s.split(/\r?\n/)
来源：http://lhq.zdqjudy.top

Java: s.lines().toList()
来源：http://rap.9152youxi.cn

Go:   strings.Split(s, "\n")
来源：http://jbv.fehbvm.com

Ruby: s.lines
来源：http://nwv.cqqwz.cn

C#:   s.Split('\n')
来源：http://kss.zhaomingkeji.xyz

[E20] 判断字符串是否为空
来源：http://mze.hammf.cn

Py:   if not s:
来源：http://vyq.vehdjk.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://crd.cashguo.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lzc.tarul.cn

TS:   if (s === "") {}
来源：http://yeh.jianghu66.top

Java: if (s.isEmpty()) {}
来源：http://avn.9152youxi.cn

Go:   if s == "" {}
来源：http://mub.wangdashe.top

Ruby: if s.empty?
来源：http://bpn.zhijiandao.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xiq.vqdsnc.cn

[E21] 超长截断加省略号
来源：http://pyj.chenjidiqi.icu

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kph.meibo888.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://drj.fanxiaobao.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pkg.tarul.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://amg.tarul.cn


<!-- 参考信息 -->