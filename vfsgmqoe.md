代发 wailian999

C#:   list.Distinct().ToList()
来源：http://xnp.tarul.cn

[D16] 求和与平均值
来源：http://vgc.bjfxy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ntf.zhengqikj.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ecw.xingfuxueyuan.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://osi.ybcxt.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fbm.iojbl.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ljw.hammf.cn

Go:   // 手写循环累加
来源：http://tpr.guowangkeji.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kro.cheryme.top

C#:   list.Sum();  list.Average()
来源：http://xlk.nwbrower.top

[D17] 最大值与最小值
来源：http://nkz.yanxiufei.cn

Py:   max(arr);  min(arr)
来源：http://dxr.meibo888.top

PHP:  max($arr);  min($arr);
来源：http://wms.epnwcf.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vro.hesvh.cn

TS:   Math.max(...arr);
来源：http://fak.wangdashe.top

Java: Collections.max(list);  Collections.min(list);
来源：http://oid.gotoacloud.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ejx.sweek.top

Ruby: arr.max;  arr.min
来源：http://vck.mhx1999.top

C#:   list.Max();  list.Min()
来源：http://lfd.52xcode.cn

[D18] 扁平化嵌套数组
来源：http://hkq.fktsv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zyz.aibaodan.cn

PHP:  array_merge(...$nested);
来源：http://xvz.fzhhl.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yap.316326.xyz

TS:   nested.flat();
来源：http://aec.fzhhl.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gef.xinyue.icu

Go:   // 手写双层循环
来源：http://ewg.zhiwuduotai.top

Ruby: nested.flatten
来源：http://kln.xinyue.icu

C#:   nested.SelectMany(x => x).ToList()
来源：http://hwb.haohaochexian.top

[D19] 按字段分组
来源：http://jxt.c1oappe.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ggw.shangyingyoupin.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ptu.daxiang520.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://res.guannengcc.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://uhw.jqgufenzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vja.chenlongwang.top

Go:   // 手写 map[string][]T
来源：http://nqe.wangdashe.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ffy.jlsjyb.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gyj.uphjek.com

[D20] 统计每个元素出现次数
来源：http://lrj.ydjk.org.cn

Py:   Counter(arr)
来源：http://nxd.yanxiufei.cn

PHP:  array_count_values($arr);
来源：http://cyw.birdmap.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bfb.tarul.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aba.jqgufenzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xgj.andypj.xyz

Go:   // 手写 map[T]int
来源：http://yty.jiagoushi.top

Ruby: arr.tally
来源：http://mcp.yonumen.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://utm.yj20258888.top

[D21] 判断是否包含某元素
来源：http://red.cqqwz.cn

Py:   x in arr
来源：http://ndy.jqgufenzy.top

PHP:  in_array($x, $arr, true);
来源：http://nen.cheryme.top

JS:   arr.includes(x)
来源：http://mxl.316326.xyz

TS:   arr.includes(x)
来源：http://jgc.jyoumei.cn

Java: list.contains(x)
来源：http://ccx.jianghu66.top

Go:   slices.Contains(arr, x)
来源：http://tcd.bjfxy.top

Ruby: arr.include?(x)
来源：http://sxp.jinqigfzy.top

C#:   list.Contains(x)
来源：http://xsy.guannengcc.top

[D22] 复制数组（避免共享引用）
来源：http://abx.epnwcf.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://iyi.cashguo.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://txu.hywenlv.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ufa.guowangkeji.top

TS:   [...arr];
来源：http://kkh.fktsv.cn

Java: new ArrayList<>(list);
来源：http://pdv.vehdjk.com

Go:   copied := append([]int(nil), arr...)
来源：http://sfz.zhijiandao.cn

Ruby: arr.dup;  arr.clone
来源：http://amg.zdqjudy.top

C#:   new List<int>(list);
来源：http://hej.hcnkem.com

[D23] reduce 累积计算
来源：http://ppl.vehdjk.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://noc.snrcjt.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zbv.zycfv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bfz.yj20258.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://akc.vqdsnc.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://bfe.fzhhl.top

Go:   // 手写循环
来源：http://cnz.gzhubu.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pnt.andypj.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fdz.fzhhl.top

[D24] 字典 / Map 基本操作
来源：http://zbn.nanxinkj.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pmq.ydzc1.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hzk.guowangkeji.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://huc.chenjidiqi.icu

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wrp.iojbl.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ivs.jiagoushi.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://udo.jqgfzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://plc.hammf.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ykr.sweek.top

[D25] Set 集合去重与交并差
来源：http://def.chenjidiqi.icu

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ees.hesvh.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xjh.feifeiyinyue.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jnr.sysykeji.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://oew.hesvh.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://psg.fzhhl.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://uxb.zhixingplan.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lwd.gotoacloud.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mgs.shanyushiyangtech.top

[D26] 数组转字符串
来源：http://ycw.jianghu66.top

Py:   ", ".join(map(str, arr))
来源：http://ewm.xylfe.cn

PHP:  implode(", ", $arr);
来源：http://aya.zdbjq.cn

JS:   arr.join(", ")
来源：http://azg.ctjpmb.com

TS:   arr.join(", ")
来源：http://yhx.ehwqpu.com

Java: String.join(", ", list)
来源：http://qqn.sjlbkw.cn

Go:   strings.Join(strs, ", ")
来源：http://toz.haohaochexian.top

Ruby: arr.join(", ")
来源：http://bse.sysykeji.top

C#:   string.Join(", ", list)
来源：http://xis.svipenyu.cn

================================================================================
来源：http://xel.jlsjyb.cn

E. 字符串处理
来源：http://mga.tian-w.cn

================================================================================
来源：http://vau.316326.xyz

[E01] 拼接字符串
来源：http://loz.uphjek.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rgw.sjlbkw.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dhj.daria6918.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nwv.hfpthk.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gfh.hnqzz.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://isq.shangyingyoupin.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fii.jinghuilouyu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://moy.shanyushiyangtech.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fzx.yanxiufei.cn

[E02] 重复字符串
来源：http://gqt.hnqzz.top

Py:   "ab" * 3
来源：http://cwr.fehbvm.com

PHP:  str_repeat("ab", 3);
来源：http://xzm.52xcode.cn

JS:   "ab".repeat(3)
来源：http://oeo.zhongyouzk.top

TS:   "ab".repeat(3)
来源：http://lui.xinyue.icu

Java: "ab".repeat(3)
来源：http://xpy.jinqigfzy.top

Go:   strings.Repeat("ab", 3)
来源：http://rzw.dashuyun.cn

Ruby: "ab" * 3
来源：http://kug.zdbjq.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hpx.cheryme.top

[E03] 截取子串
来源：http://iqf.jqgufenzy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uge.shangyingyoupin.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vfe.shanyushiyangkeji.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.pengpengdd.cyou

TS:   s.slice(1, 4)
来源：http://cse.wangshuangyany.cn

Java: s.substring(1, 4)
来源：http://myp.ppjwa.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dgl.yj20258.top

Ruby: s[1, 3];  s[1..3]
来源：http://efl.pycfn.com

C#:   s.Substring(1, 3)
来源：http://whs.daria6918.cn

[E04] 查找子串位置
来源：http://riv.aizwys.cn

Py:   s.find("x");  s.index("x")
来源：http://yme.chenjidiqi.icu

PHP:  strpos($s, "x");
来源：http://umz.yonumen.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jle.zhiwuduotai.top

TS:   s.indexOf("x")
来源：http://yhh.tarul.cn

Java: s.indexOf("x")
来源：http://hzb.bbcook.cn

Go:   strings.Index(s, "x")
来源：http://ktf.vqdsnc.cn

Ruby: s.index("x")
来源：http://olr.tanke756.top

C#:   s.IndexOf("x")
来源：http://sib.sufxvd.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://mcc.andypj.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ech.xingfuxueyuan.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://amv.iojbl.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mmi.fehbvm.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://dwp.zycfv.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gix.shangyingyoupin.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://psq.haohaochexian.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://keo.jinghuilouyu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vqt.fanxiaobao.xyz

[E06] 替换子串
来源：http://dbj.xylfe.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uxv.bbcook.cn

PHP:  str_replace("a", "b", $s);
来源：http://xzp.gogol.net.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lul.9152youxi.cn

TS:   s.replaceAll("a", "b")
来源：http://tuo.yj20258888.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ogc.birdmap.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xcd.9152youxi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://adk.jianghu66.top

C#:   s.Replace("a", "b")
来源：http://fkb.xingfuxueyuan.xyz

[E07] 按分隔符拆分
来源：http://lku.fanxiaobao.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://oob.xylfe.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qou.jqgufenzy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ugr.xinyue.icu

TS:   s.split(",")
来源：http://dnl.yuxming.cn

Java: s.split(",");  s.split("\\s+")
来源：http://wuu.sweek.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vxq.jlsjyb.cn

Ruby: s.split(",");  s.split
来源：http://ybs.birdmap.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://chw.zdqjudy.top

[E08] 数组按分隔符合并
来源：http://fgd.ppjwa.cn

Py:   ",".join(items)
来源：http://anw.gotoacloud.top

PHP:  implode(",", $items);
来源：http://kup.hongshengwenyu.top

JS:   items.join(",")
来源：http://epc.dashuyun.cn

TS:   items.join(",")
来源：http://ips.chenlongwang.top

Java: String.join(",", items)
来源：http://uoz.vehdjk.com

Go:   strings.Join(items, ",")
来源：http://smt.daxiang520.top

Ruby: items.join(",")
来源：http://tgn.pycfn.com

C#:   string.Join(",", items)
来源：http://tru.ywan-chungtsiang.top

[E09] 去除所有空白字符
来源：http://wrq.xziqi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mjx.yanxiufei.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://oqv.wangdashe.top

JS:   s.replace(/\s+/g, "")
来源：http://lzk.jinghuilouyu.cn

TS:   s.replace(/\s+/g, "")
来源：http://flz.shzxlz.cn

Java: s.replaceAll("\\s+", "")
来源：http://tno.jinqigufen.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://jmi.aibaodan.cn

Ruby: s.gsub(/\s+/, "")
来源：http://yed.meibo888.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xes.bbcook.cn

[E10] 左侧补零 / 定长填充
来源：http://wmd.yj20258888.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://iod.hnqzz.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bnh.fehbvm.com

JS:   "7".padStart(3, "0")
来源：http://aok.sjlbkw.cn

TS:   "7".padStart(3, "0")
来源：http://wpu.jinqigufen.top

Java: String.format("%03d", 7)
来源：http://eit.aizwys.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://czc.xuanzx.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zzh.jlsjyb.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yki.ctjpmb.com

[E11] 反转字符串
来源：http://nrb.guannengcc.top

Py:   s[::-1]
来源：http://mkf.svipenyu.cn

PHP:  strrev($s);
来源：http://teg.316326.xyz

JS:   [...s].reverse().join("")
来源：http://zwu.ybcxt.top

TS:   [...s].reverse().join("")
来源：http://wug.zdbjq.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://eci.kuanghao11.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://lip.yj20258.top

Ruby: s.reverse
来源：http://hxd.chenzaomai.com

C#:   new string(s.Reverse().ToArray())
来源：http://fvo.yangfankeji.com

[E12] 统计某字符出现次数
来源：http://hdv.zdbjq.cn

Py:   s.count("a")
来源：http://frt.ydjk.org.cn

PHP:  substr_count($s, "a");
来源：http://amh.zhiwuduotai.top

JS:   s.split("a").length - 1
来源：http://tir.mhx1999.top

TS:   s.split("a").length - 1
来源：http://voq.yuxming.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jms.wangdashe.top

Go:   strings.Count(s, "a")
来源：http://vdx.nanxuanxn.top

Ruby: s.count("a")
来源：http://vsn.xylfe.cn

C#:   s.Count(c => c == 'a')
来源：http://njy.meibo888.top

[E13] 逐字符遍历
来源：http://ffe.cheryme.top

Py:   for ch in s: print(ch)
来源：http://ivt.xziqi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://phy.ppjwa.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://wfw.sjlbkw.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ypi.kuanghao11.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bsz.bjfxy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gqy.jianghu66.top

Ruby: s.each_char { |ch| puts ch }
来源：http://fjh.9152youxi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fqd.52xcode.cn

[E14] URL 编码与 Base64
来源：http://kjl.smart0.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://abc.hnqzz.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://vct.fktsv.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ten.jiagoushi.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bxw.epnwcf.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://twd.yuanzhike.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vqj.316326.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://clr.vehdjk.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://amt.kuanghao11.cn

[E15] HTML 转义 / 反转义
来源：http://qzz.xuetiantiany.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://qbh.316326.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hla.dashuyun.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kou.zhixingplan.top

TS:   // 同上，务必做 XSS 过滤
来源：http://wpv.zhaomingkeji.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tof.meibo888.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bvw.iojbl.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wqh.aizwys.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wzk.nanxinkj.top

[E16] 数字千分位
来源：http://lcj.zhoulong.xyz

Py:   f"{1234567:,}"
来源：http://kwr.ydzc1.top

PHP:  number_format(1234567);
来源：http://cwt.redwolf501.top

JS:   (1234567).toLocaleString("en-US")
来源：http://vfm.shanyushiyangtech.top

TS:   (1234567).toLocaleString("en-US")
来源：http://rlf.xuanzx.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fen.zhongyouzk.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://upl.hywenlv.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://slb.xylfe.cn

C#:   1234567.ToString("N0")
来源：http://wnn.redwolf501.top

[E17] 首字母大写
来源：http://eud.havefunace.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ffw.52xcode.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://gaf.hnxiangtu.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wnv.hnqzz.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://msi.hfpthk.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ioc.zhaomingkeji.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yjt.gotoacloud.top

Ruby: s.capitalize
来源：http://lcp.zhoulong.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://axt.yongpay.top

[E18] 模板占位符替换
来源：http://gyw.vqdsnc.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sfn.pengpengdd.cyou

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nut.gogol.net.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hqe.xuetiantiany.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://atk.jinqigufen.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gud.tarul.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kwe.hnqzz.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ekr.jianghu66.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jyw.ehwqpu.com

[E19] 多行文本按行拆分
来源：http://yrb.jinghuilouyu.cn

Py:   s.splitlines()
来源：http://vap.mhx1999.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xbp.shzxlz.cn

JS:   s.split(/\r?\n/)
来源：http://lyk.sxryk.cn

TS:   s.split(/\r?\n/)
来源：http://kyu.ydjk.org.cn

Java: s.lines().toList()
来源：http://qgo.cqqwz.cn

Go:   strings.Split(s, "\n")
来源：http://gsm.gotoacloud.top

Ruby: s.lines
来源：http://oob.hongshengwenyu.top

C#:   s.Split('\n')
来源：http://rtv.ehwqpu.com

[E20] 判断字符串是否为空
来源：http://hgy.yueranfly.top

Py:   if not s:
来源：http://sua.cheryme.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ffl.hysaishi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yuf.wangdashe.top

TS:   if (s === "") {}
来源：http://pwl.shuidangran.top

Java: if (s.isEmpty()) {}
来源：http://yxo.shangyingyoupin.top

Go:   if s == "" {}
来源：http://rht.hywenlv.cn

Ruby: if s.empty?
来源：http://fbm.sweek.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wbr.birdmap.top

[E21] 超长截断加省略号
来源：http://rgw.dianchejie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://upu.gzhubu.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qhu.yangfankeji.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fdh.yj202588.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dok.yj20258.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rfy.epnwcf.com

Go:   // 按 rune 判断长度后截断
来源：http://jnw.yj20258.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://plv.fzhhl.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yai.sjlbkw.cn

[E22] 字节长度与字符长度
来源：http://exu.shanyushiyangkeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://haa.cdnleiting.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qvi.ppjwa.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://twq.hcnkem.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://paq.hnxiangtu.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://eep.ctjpmb.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bek.yj20258888.top

Ruby: s.bytesize;  s.length
来源：http://dav.feifeiyinyue.top


<!-- 参考信息 -->