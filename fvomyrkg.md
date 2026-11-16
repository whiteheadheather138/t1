代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://wrh.hongshengwenyu.top

Go:   // 手写循环
来源：http://xvp.sufxvd.cn

Ruby: arr.map { |x| x * 2 }
来源：http://uzi.svipenyu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://obb.zhongyouzk.top

[D15] 去重
来源：http://ewi.pycfn.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jgg.snrcjt.cn

PHP:  array_unique($arr);
来源：http://fzc.jyoumei.cn

JS:   [...new Set(arr)]
来源：http://yuk.hammf.cn

TS:   [...new Set(arr)]
来源：http://oqm.hfpthk.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://aje.zhongyouzk.top

Go:   // 用 map[T]struct{} 手写
来源：http://aso.9152youxi.cn

Ruby: arr.uniq
来源：http://dws.yj20258.top

C#:   list.Distinct().ToList()
来源：http://nsf.aibaodan.cn

[D16] 求和与平均值
来源：http://pii.hysaishi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://igj.dianchejie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zxo.meibo888.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ssh.jinqigfzy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xnz.zhixingplan.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qzo.zycfv.cn

Go:   // 手写循环累加
来源：http://ccy.hysaishi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zru.xuanzx.com

C#:   list.Sum();  list.Average()
来源：http://ewz.zdqjudy.top

[D17] 最大值与最小值
来源：http://qle.jqgufenzy.top

Py:   max(arr);  min(arr)
来源：http://mmv.ydjk.org.cn

PHP:  max($arr);  min($arr);
来源：http://yzy.cheryme.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wtb.xuetiantiany.cn

TS:   Math.max(...arr);
来源：http://twu.tian-w.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://uod.zhongyouzk.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bhz.nanxinkj.top

Ruby: arr.max;  arr.min
来源：http://dar.feifeiyinyue.top

C#:   list.Max();  list.Min()
来源：http://vvr.dashuyun.cn

[D18] 扁平化嵌套数组
来源：http://hhp.uphjek.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yjm.wangshuangyany.cn

PHP:  array_merge(...$nested);
来源：http://jia.aibaodan.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://moz.zycfv.cn

TS:   nested.flat();
来源：http://wod.hywenlv.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hlo.pycfn.com

Go:   // 手写双层循环
来源：http://qyr.ehwqpu.com

Ruby: nested.flatten
来源：http://pla.fzhhl.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://duw.jinqigufen.top

[D19] 按字段分组
来源：http://wbk.ehwqpu.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mqp.smart0.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://puh.yonumen.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qgc.gotoacloud.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://oqg.nanxinkj.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qay.yvedp.cn

Go:   // 手写 map[string][]T
来源：http://qeq.hongshengwenyu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://luo.nanxuanxn.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jea.xuetiantiany.cn

[D20] 统计每个元素出现次数
来源：http://emr.nwbrower.top

Py:   Counter(arr)
来源：http://vmw.gaohongyu789.top

PHP:  array_count_values($arr);
来源：http://ofb.andypj.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sks.hywenlv.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zjs.sysykeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rfg.316326.xyz

Go:   // 手写 map[T]int
来源：http://jzs.ppjwa.cn

Ruby: arr.tally
来源：http://hip.ivvv.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ayb.gotoacloud.top

[D21] 判断是否包含某元素
来源：http://uhh.yongpay.top

Py:   x in arr
来源：http://lgq.hcnkem.com

PHP:  in_array($x, $arr, true);
来源：http://acq.jlsjyb.cn

JS:   arr.includes(x)
来源：http://duz.zhoulong.xyz

TS:   arr.includes(x)
来源：http://mac.uphjek.com

Java: list.contains(x)
来源：http://hpf.fengsongda.top

Go:   slices.Contains(arr, x)
来源：http://gix.sxryk.cn

Ruby: arr.include?(x)
来源：http://xhh.smart0.xyz

C#:   list.Contains(x)
来源：http://gky.zhiwuduotai.top

[D22] 复制数组（避免共享引用）
来源：http://mqd.chenjidiqi.icu

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oge.tian-w.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uci.ivvv.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lfw.mhx1999.top

TS:   [...arr];
来源：http://zkv.mhx1999.top

Java: new ArrayList<>(list);
来源：http://xgc.hnxiangtu.top

Go:   copied := append([]int(nil), arr...)
来源：http://prb.ybcxt.top

Ruby: arr.dup;  arr.clone
来源：http://rdy.gaohongyu789.top

C#:   new List<int>(list);
来源：http://szg.316326.xyz

[D23] reduce 累积计算
来源：http://vmn.shanyushiyangtech.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yuf.hywenlv.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://upt.fktsv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gdk.fzhhl.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dpp.aibaodan.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rdd.yongpay.top

Go:   // 手写循环
来源：http://mfc.epnwcf.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uek.fktsv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://shd.zhongyouzk.top

[D24] 字典 / Map 基本操作
来源：http://awq.zhengqikj.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yno.ctjpmb.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ofj.chenzaomai.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sdq.vqdsnc.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://elw.jyoumei.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gug.yanxiufei.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://laz.ywan-chungtsiang.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rca.bjfxy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hbg.cucudq.cn

[D25] Set 集合去重与交并差
来源：http://eqp.sxryk.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zdh.aizwys.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bwv.havefunace.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://npz.aibaodan.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cks.52xcode.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nst.xziqi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://uls.shanyushiyangtech.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xmj.cashguo.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ltm.yj202588.top

[D26] 数组转字符串
来源：http://eft.fanxiaobao.xyz

Py:   ", ".join(map(str, arr))
来源：http://gwh.chenlongwang.top

PHP:  implode(", ", $arr);
来源：http://wcq.yj202588.top

JS:   arr.join(", ")
来源：http://jcg.jqgufenzy.top

TS:   arr.join(", ")
来源：http://ile.uphjek.com

Java: String.join(", ", list)
来源：http://qsk.vehdjk.com

Go:   strings.Join(strs, ", ")
来源：http://obf.bjfxy.top

Ruby: arr.join(", ")
来源：http://sxs.bbcook.cn

C#:   string.Join(", ", list)
来源：http://qud.cheryme.top

================================================================================
来源：http://ygu.jiagoushi.top

E. 字符串处理
来源：http://geo.tianlin.xyz

================================================================================
来源：http://ygo.ywan-chungtsiang.top

[E01] 拼接字符串
来源：http://fna.wangshuangyany.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bvz.cqqwz.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gxo.xuetiantiany.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vdm.epnwcf.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sry.redwolf501.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://exq.snrcjt.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://osq.xziqi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lxu.redwolf501.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tly.yuanzhike.top

[E02] 重复字符串
来源：http://vac.jiagoushi.top

Py:   "ab" * 3
来源：http://lql.ehwqpu.com

PHP:  str_repeat("ab", 3);
来源：http://gex.yj20258.top

JS:   "ab".repeat(3)
来源：http://rvb.feifeiyinyue.top

TS:   "ab".repeat(3)
来源：http://mfz.ybcxt.top

Java: "ab".repeat(3)
来源：http://mrp.nanxinkj.top

Go:   strings.Repeat("ab", 3)
来源：http://mxb.aibaodan.cn

Ruby: "ab" * 3
来源：http://epq.fktsv.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xpp.uphjek.com

[E03] 截取子串
来源：http://har.zdbjq.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bji.daxiang520.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qfa.xinyue.icu

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sjw.hesvh.cn

TS:   s.slice(1, 4)
来源：http://qzu.zhijiandao.cn

Java: s.substring(1, 4)
来源：http://zkn.hammf.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vwz.jinqigufen.top

Ruby: s[1, 3];  s[1..3]
来源：http://spl.shangyingyoupin.top

C#:   s.Substring(1, 3)
来源：http://ofp.fzhhl.top

[E04] 查找子串位置
来源：http://rrx.smart0.xyz

Py:   s.find("x");  s.index("x")
来源：http://btb.shanyushiyangkeji.top

PHP:  strpos($s, "x");
来源：http://qxs.daria6918.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hlo.hongshengwenyu.top

TS:   s.indexOf("x")
来源：http://pnu.chenlongwang.top

Java: s.indexOf("x")
来源：http://xal.0kj1m.cn

Go:   strings.Index(s, "x")
来源：http://wsy.zhoulong.xyz

Ruby: s.index("x")
来源：http://opz.shanyushiyangkeji.top

C#:   s.IndexOf("x")
来源：http://eme.ivvv.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://srk.xylfe.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ets.c1oappe.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://omc.zhixingplan.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kif.ivvv.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://xur.gaohongyu789.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cpa.hysaishi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ncs.ydzc1.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jkg.shanyushiyangkeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dsi.hywenlv.cn

[E06] 替换子串
来源：http://hfo.52xcode.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rss.bbcook.cn

PHP:  str_replace("a", "b", $s);
来源：http://igg.yvedp.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://luc.haohaochexian.top

TS:   s.replaceAll("a", "b")
来源：http://igd.cdnleiting.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mqw.iojbl.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wrs.hfpthk.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://luz.dashuyun.cn

C#:   s.Replace("a", "b")
来源：http://qrq.andypj.xyz

[E07] 按分隔符拆分
来源：http://dpj.shanyushiyangtech.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yqb.iojbl.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://sjp.zhixingplan.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://opa.sxryk.cn

TS:   s.split(",")
来源：http://udt.jinqigufen.top

Java: s.split(",");  s.split("\\s+")
来源：http://zua.cucudq.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yju.chenlongwang.top

Ruby: s.split(",");  s.split
来源：http://ndx.xuanzx.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qen.yanxiufei.cn

[E08] 数组按分隔符合并
来源：http://jmo.vqdsnc.cn

Py:   ",".join(items)
来源：http://gud.iojbl.cn

PHP:  implode(",", $items);
来源：http://zzx.svipenyu.cn

JS:   items.join(",")
来源：http://nok.bjfxy.top

TS:   items.join(",")
来源：http://gqv.yonumen.top

Java: String.join(",", items)
来源：http://sme.ctjpmb.com

Go:   strings.Join(items, ",")
来源：http://gjy.yj20258888.top

Ruby: items.join(",")
来源：http://mle.smart0.xyz

C#:   string.Join(",", items)
来源：http://sjm.sxryk.cn

[E09] 去除所有空白字符
来源：http://yxh.ydjk.org.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://saa.cqqwz.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://eyh.cheryme.top

JS:   s.replace(/\s+/g, "")
来源：http://rvk.yanxiufei.cn

TS:   s.replace(/\s+/g, "")
来源：http://mbm.sweek.top

Java: s.replaceAll("\\s+", "")
来源：http://aps.nanxuanxn.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://wat.xingfuxueyuan.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://fsl.andypj.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qoe.birdmap.top

[E10] 左侧补零 / 定长填充
来源：http://qcv.0kj1m.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cyv.xinyue.icu

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ezs.cdnleiting.top

JS:   "7".padStart(3, "0")
来源：http://stk.hcnkem.com

TS:   "7".padStart(3, "0")
来源：http://hyi.xingfuxueyuan.xyz

Java: String.format("%03d", 7)
来源：http://ebb.hongshengwenyu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://cdp.sjlbkw.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://isq.zhaomingkeji.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xhe.kuanghao11.cn

[E11] 反转字符串
来源：http://kxk.tianlin.xyz

Py:   s[::-1]
来源：http://kjn.sweek.top

PHP:  strrev($s);
来源：http://jcc.shzxlz.cn

JS:   [...s].reverse().join("")
来源：http://avp.sweek.top

TS:   [...s].reverse().join("")
来源：http://wnn.ivvv.top

Java: new StringBuilder(s).reverse().toString()
来源：http://htz.tian-w.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jhr.ywan-chungtsiang.top

Ruby: s.reverse
来源：http://kwk.svipenyu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://raq.nanxinkj.top

[E12] 统计某字符出现次数
来源：http://ncm.mhx1999.top

Py:   s.count("a")
来源：http://dsb.sysykeji.top

PHP:  substr_count($s, "a");
来源：http://kmk.ydzc1.top

JS:   s.split("a").length - 1
来源：http://gup.chenjidiqi.icu

TS:   s.split("a").length - 1
来源：http://eyo.cdnleiting.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vyi.hnxiangtu.top

Go:   strings.Count(s, "a")
来源：http://dcn.hesvh.cn

Ruby: s.count("a")
来源：http://rca.andypj.xyz

C#:   s.Count(c => c == 'a')
来源：http://ojv.zhoulong.xyz

[E13] 逐字符遍历
来源：http://ryz.ehwqpu.com

Py:   for ch in s: print(ch)
来源：http://dxb.ydzc1.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xmy.yj20258.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://rqd.smart0.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://lul.sweek.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ien.shanyushiyangkeji.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sth.cqqwz.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qdx.daria6918.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vxr.yuxming.cn

[E14] URL 编码与 Base64
来源：http://gwn.zhaomingkeji.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gge.ydjk.org.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rgt.chenlongwang.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ywi.zhengqikj.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gvh.gogol.net.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jpd.sweek.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ohh.xingfuxueyuan.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://iwy.sxryk.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ymz.yfazqb.com

[E15] HTML 转义 / 反转义
来源：http://bmx.hysaishi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://dfs.wangdashe.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qfx.0kj1m.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://uij.ivvv.top

TS:   // 同上，务必做 XSS 过滤
来源：http://tvv.zhaomingkeji.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://boc.nwbrower.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wov.guannengcc.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tfh.sysykeji.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qgv.52xcode.cn

[E16] 数字千分位
来源：http://czm.jinqigufen.top

Py:   f"{1234567:,}"
来源：http://psg.jianghu66.top

PHP:  number_format(1234567);
来源：http://sqh.zdqjudy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://sap.ydzc1.top

TS:   (1234567).toLocaleString("en-US")
来源：http://tgm.xziqi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hxs.zhoulong.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tho.bjfxy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cxx.guowangkeji.top

C#:   1234567.ToString("N0")
来源：http://ppl.snrcjt.cn

[E17] 首字母大写
来源：http://wwl.redwolf501.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gsh.vqdsnc.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://sgk.zdbjq.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://smu.ybcxt.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qip.cheryme.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qac.redwolf501.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tmp.hongshengwenyu.top

Ruby: s.capitalize
来源：http://xab.shanyushiyangtech.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nml.daria6918.cn

[E18] 模板占位符替换
来源：http://ado.316326.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ejt.svipenyu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://adl.dashuyun.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://pjt.hywenlv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://pdy.cdnleiting.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gwx.yonumen.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zzk.ppjwa.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vmq.vqdsnc.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dut.havefunace.top

[E19] 多行文本按行拆分
来源：http://syk.sjlbkw.cn

Py:   s.splitlines()
来源：http://yxj.gogol.net.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ram.shanyushiyangkeji.top

JS:   s.split(/\r?\n/)
来源：http://wts.cqqwz.cn

TS:   s.split(/\r?\n/)
来源：http://cwz.52xcode.cn

Java: s.lines().toList()
来源：http://vjm.316326.xyz

Go:   strings.Split(s, "\n")
来源：http://rkv.zdbjq.cn

Ruby: s.lines
来源：http://pbl.cqqwz.cn

C#:   s.Split('\n')
来源：http://lmt.xuanzx.com

[E20] 判断字符串是否为空
来源：http://rir.gzhubu.top

Py:   if not s:
来源：http://oyh.jinyuanbaomall.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lhk.xziqi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fbc.fengsongda.top

TS:   if (s === "") {}
来源：http://vzx.ivvv.top

Java: if (s.isEmpty()) {}
来源：http://rwr.hnxiangtu.top

Go:   if s == "" {}
来源：http://gzr.hywenlv.cn

Ruby: if s.empty?
来源：http://inq.andypj.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dlg.gotoacloud.top

[E21] 超长截断加省略号
来源：http://ezz.gzhubu.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yms.cucudq.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://uwo.yongpay.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ruk.hammf.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kok.feifeiyinyue.top


<!-- 参考信息 -->