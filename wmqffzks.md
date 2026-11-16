代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pet.pycfn.com

C#:   list.Sum();  list.Average()
来源：http://byq.xuetiantiany.cn

[D17] 最大值与最小值
来源：http://nvn.ydjk.org.cn

Py:   max(arr);  min(arr)
来源：http://aqo.aizwys.cn

PHP:  max($arr);  min($arr);
来源：http://kfl.tianlin.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tne.yj20258888.top

TS:   Math.max(...arr);
来源：http://ita.jinqigufen.top

Java: Collections.max(list);  Collections.min(list);
来源：http://tgk.quarkkingdee.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ebu.vehdjk.com

Ruby: arr.max;  arr.min
来源：http://jug.yj20258888.top

C#:   list.Max();  list.Min()
来源：http://ijs.pycfn.com

[D18] 扁平化嵌套数组
来源：http://vdc.aizwys.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wkw.shangyingyoupin.top

PHP:  array_merge(...$nested);
来源：http://yif.nwbrower.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dll.hcnkem.com

TS:   nested.flat();
来源：http://mtb.xinyue.icu

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lre.yonumen.top

Go:   // 手写双层循环
来源：http://qof.yonumen.top

Ruby: nested.flatten
来源：http://jth.hongshengwenyu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ycc.chenzaomai.com

[D19] 按字段分组
来源：http://gla.hywenlv.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cfc.quarkkingdee.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://oml.bjfxy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cdq.feifeiyinyue.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://spm.sjlbkw.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://usq.zdqjudy.top

Go:   // 手写 map[string][]T
来源：http://hdg.zhengqikj.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://qtr.hnxiangtu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vat.xuanzx.com

[D20] 统计每个元素出现次数
来源：http://ckl.tarul.cn

Py:   Counter(arr)
来源：http://etf.ydzc1.top

PHP:  array_count_values($arr);
来源：http://sbd.zdqjudy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pko.mhx1999.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ecu.tarul.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yim.yj20258.top

Go:   // 手写 map[T]int
来源：http://zpn.gzhubu.top

Ruby: arr.tally
来源：http://iku.cashguo.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fgc.aizwys.cn

[D21] 判断是否包含某元素
来源：http://yhu.cqqwz.cn

Py:   x in arr
来源：http://frm.xuanzx.com

PHP:  in_array($x, $arr, true);
来源：http://lzn.havefunace.top

JS:   arr.includes(x)
来源：http://kvb.vqdsnc.cn

TS:   arr.includes(x)
来源：http://fma.jqgufenzy.top

Java: list.contains(x)
来源：http://qhs.yj20258.top

Go:   slices.Contains(arr, x)
来源：http://grg.wangshuangyany.cn

Ruby: arr.include?(x)
来源：http://arf.mhx1999.top

C#:   list.Contains(x)
来源：http://ock.sufxvd.cn

[D22] 复制数组（避免共享引用）
来源：http://kxp.hnxiangtu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xwa.ydjk.org.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vye.iojbl.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rpp.nwbrower.top

TS:   [...arr];
来源：http://wzb.sweek.top

Java: new ArrayList<>(list);
来源：http://kwj.yj202588.top

Go:   copied := append([]int(nil), arr...)
来源：http://enn.tanke756.top

Ruby: arr.dup;  arr.clone
来源：http://pkq.epnwcf.com

C#:   new List<int>(list);
来源：http://brf.tianlin.xyz

[D23] reduce 累积计算
来源：http://pzg.zhoulong.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ewn.wangshuangyany.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://twc.snrcjt.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xsc.yfazqb.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qls.hywenlv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://kax.yonumen.top

Go:   // 手写循环
来源：http://lsv.zhoulong.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mje.zycfv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qxo.yvedp.cn

[D24] 字典 / Map 基本操作
来源：http://dlh.sufxvd.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jje.snrcjt.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lbe.jinghuilouyu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tnh.mhx1999.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cwt.hcnkem.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kcz.fengsongda.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://aen.hcnkem.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://eny.shanyushiyangtech.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pvi.fzhhl.top

[D25] Set 集合去重与交并差
来源：http://ndv.xylfe.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://syp.jiagoushi.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://uqr.fktsv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://swd.cucudq.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sil.smart0.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lzx.aizwys.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jxi.daxiang520.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lqf.zhijiandao.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mmc.zdbjq.cn

[D26] 数组转字符串
来源：http://uno.zhongyouzk.top

Py:   ", ".join(map(str, arr))
来源：http://rrb.yuxming.cn

PHP:  implode(", ", $arr);
来源：http://iuz.sufxvd.cn

JS:   arr.join(", ")
来源：http://sue.snrcjt.cn

TS:   arr.join(", ")
来源：http://qcd.hesvh.cn

Java: String.join(", ", list)
来源：http://doo.zhiwuduotai.top

Go:   strings.Join(strs, ", ")
来源：http://qob.ehwqpu.com

Ruby: arr.join(", ")
来源：http://nbn.yonumen.top

C#:   string.Join(", ", list)
来源：http://whc.hysaishi.cn

================================================================================
来源：http://pyr.cucudq.cn

E. 字符串处理
来源：http://lwz.chenlongwang.top

================================================================================
来源：http://xgj.xingfuxueyuan.xyz

[E01] 拼接字符串
来源：http://ynl.jiagoushi.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://oll.dianchejie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://svw.epnwcf.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nvy.andypj.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://awe.gogol.net.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://drq.ppjwa.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fgv.cashguo.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hon.cheryme.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lno.guannengcc.top

[E02] 重复字符串
来源：http://mnf.gogol.net.cn

Py:   "ab" * 3
来源：http://qzo.dashuyun.cn

PHP:  str_repeat("ab", 3);
来源：http://zda.nanxuanxn.top

JS:   "ab".repeat(3)
来源：http://jsy.uphjek.com

TS:   "ab".repeat(3)
来源：http://gzh.ctjpmb.com

Java: "ab".repeat(3)
来源：http://zex.sysykeji.top

Go:   strings.Repeat("ab", 3)
来源：http://zkb.wangshuangyany.cn

Ruby: "ab" * 3
来源：http://kmm.nwbrower.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zou.sweek.top

[E03] 截取子串
来源：http://vwi.sjlbkw.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xmw.aizwys.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qfp.tianlin.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pnx.zycfv.cn

TS:   s.slice(1, 4)
来源：http://biv.gogol.net.cn

Java: s.substring(1, 4)
来源：http://tux.shanyushiyangkeji.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hbh.nwbrower.top

Ruby: s[1, 3];  s[1..3]
来源：http://ksr.shzxlz.cn

C#:   s.Substring(1, 3)
来源：http://yje.andypj.xyz

[E04] 查找子串位置
来源：http://fsu.chenzaomai.com

Py:   s.find("x");  s.index("x")
来源：http://ddj.jiagoushi.top

PHP:  strpos($s, "x");
来源：http://fgm.sweek.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://oxs.fanxiaobao.xyz

TS:   s.indexOf("x")
来源：http://ncw.xuetiantiany.cn

Java: s.indexOf("x")
来源：http://dpm.chenjidiqi.icu

Go:   strings.Index(s, "x")
来源：http://gux.yvedp.cn

Ruby: s.index("x")
来源：http://poj.yonumen.top

C#:   s.IndexOf("x")
来源：http://okg.ydjk.org.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://etu.ywan-chungtsiang.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bnc.snrcjt.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gnj.xinyue.icu

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rna.hongshengwenyu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ggt.wangshuangyany.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kge.ywan-chungtsiang.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uod.ydjk.org.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yrd.yanxiufei.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yeo.zhixingplan.top

[E06] 替换子串
来源：http://uzw.ydjk.org.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uoz.ivvv.top

PHP:  str_replace("a", "b", $s);
来源：http://xmc.quarkkingdee.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vcj.vehdjk.com

TS:   s.replaceAll("a", "b")
来源：http://bpt.shanyushiyangkeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://heo.cheryme.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://brx.ctjpmb.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tou.xziqi.cn

C#:   s.Replace("a", "b")
来源：http://fow.c1oappe.top

[E07] 按分隔符拆分
来源：http://nvd.tian-w.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pjl.hammf.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zet.jinqigufen.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://spz.tian-w.cn

TS:   s.split(",")
来源：http://eyt.nanxinkj.top

Java: s.split(",");  s.split("\\s+")
来源：http://rod.tanke756.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ubs.iojbl.cn

Ruby: s.split(",");  s.split
来源：http://szu.shangyingyoupin.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tdv.fzhhl.top

[E08] 数组按分隔符合并
来源：http://loy.hfpthk.cn

Py:   ",".join(items)
来源：http://rkr.pengpengdd.cyou

PHP:  implode(",", $items);
来源：http://vxo.sweek.top

JS:   items.join(",")
来源：http://fnt.jinghuilouyu.cn

TS:   items.join(",")
来源：http://gnx.cashguo.top

Java: String.join(",", items)
来源：http://wie.zhongyouzk.top

Go:   strings.Join(items, ",")
来源：http://vaw.birdmap.top

Ruby: items.join(",")
来源：http://fic.guannengcc.top

C#:   string.Join(",", items)
来源：http://krk.ydzc1.top

[E09] 去除所有空白字符
来源：http://dxb.shzxlz.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://egy.chenlongwang.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fsr.xuanzx.com

JS:   s.replace(/\s+/g, "")
来源：http://smi.yj202588.top

TS:   s.replace(/\s+/g, "")
来源：http://dlg.chenzaomai.com

Java: s.replaceAll("\\s+", "")
来源：http://pth.chenlongwang.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://mid.birdmap.top

Ruby: s.gsub(/\s+/, "")
来源：http://ens.meibo888.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://syh.hfpthk.cn

[E10] 左侧补零 / 定长填充
来源：http://etv.aibaodan.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://epk.zycfv.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sdk.uphjek.com

JS:   "7".padStart(3, "0")
来源：http://xcs.jlsjyb.cn

TS:   "7".padStart(3, "0")
来源：http://rnk.ehwqpu.com

Java: String.format("%03d", 7)
来源：http://dpn.yongpay.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://qbu.zhongyouzk.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rvo.haohaochexian.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pji.tian-w.cn

[E11] 反转字符串
来源：http://dyr.yuxming.cn

Py:   s[::-1]
来源：http://qcv.zhijiandao.cn

PHP:  strrev($s);
来源：http://wgu.zdbjq.cn

JS:   [...s].reverse().join("")
来源：http://esp.gotoacloud.top

TS:   [...s].reverse().join("")
来源：http://yyu.316326.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://qcn.cdnleiting.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://vaz.xuanzx.com

Ruby: s.reverse
来源：http://mei.bjfxy.top

C#:   new string(s.Reverse().ToArray())
来源：http://pfs.ydjk.org.cn

[E12] 统计某字符出现次数
来源：http://yxy.yueranfly.top

Py:   s.count("a")
来源：http://bsj.wangshuangyany.cn

PHP:  substr_count($s, "a");
来源：http://dti.xuetiantiany.cn

JS:   s.split("a").length - 1
来源：http://ggt.bbcook.cn

TS:   s.split("a").length - 1
来源：http://ghr.aizwys.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://eel.dianchejie.cn

Go:   strings.Count(s, "a")
来源：http://cvu.vqdsnc.cn

Ruby: s.count("a")
来源：http://nwh.tanke756.top

C#:   s.Count(c => c == 'a')
来源：http://hmh.shanyushiyangkeji.top

[E13] 逐字符遍历
来源：http://zes.daxiang520.top

Py:   for ch in s: print(ch)
来源：http://kfx.cqqwz.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xbh.jqgfzy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://xqb.xuetiantiany.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://toh.ctjpmb.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yql.sysykeji.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://omx.ydzc1.top

Ruby: s.each_char { |ch| puts ch }
来源：http://leg.ywan-chungtsiang.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dvp.ehwqpu.com

[E14] URL 编码与 Base64
来源：http://fpr.yuxming.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://loh.sweek.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ihy.cqqwz.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://weq.chenjidiqi.icu

TS:   encodeURIComponent(s);  btoa(s)
来源：http://oer.andypj.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gkr.havefunace.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wmc.aizwys.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gbz.dashuyun.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rds.guowangkeji.top

[E15] HTML 转义 / 反转义
来源：http://ack.daria6918.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://erq.fanxiaobao.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://unn.fengsongda.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nrk.smart0.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://msd.jqgufenzy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tpj.chenjidiqi.icu

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zru.ybcxt.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fib.ybcxt.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fqg.xingfuxueyuan.xyz

[E16] 数字千分位
来源：http://kfl.fehbvm.com

Py:   f"{1234567:,}"
来源：http://ebx.snrcjt.cn

PHP:  number_format(1234567);
来源：http://pel.c1oappe.top

JS:   (1234567).toLocaleString("en-US")
来源：http://wzd.yonumen.top

TS:   (1234567).toLocaleString("en-US")
来源：http://xxy.ydjk.org.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://juv.snrcjt.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lfx.quarkkingdee.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://czw.tianlin.xyz

C#:   1234567.ToString("N0")
来源：http://xsi.yanxiufei.cn

[E17] 首字母大写
来源：http://dun.hnxiangtu.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://umx.feifeiyinyue.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://zgc.jlsjyb.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fwy.shzxlz.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ljn.kuanghao11.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://apx.feifeiyinyue.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vbd.hywenlv.cn

Ruby: s.capitalize
来源：http://cfd.0kj1m.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://osq.daria6918.cn

[E18] 模板占位符替换
来源：http://gvj.nwbrower.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yfn.yj202588.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://etw.vqdsnc.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://knt.jqgufenzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://azd.sjlbkw.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sfr.aibaodan.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lsr.ppjwa.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qgl.316326.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lav.ywan-chungtsiang.top

[E19] 多行文本按行拆分
来源：http://nik.jinghuilouyu.cn

Py:   s.splitlines()
来源：http://hvw.yueranfly.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://iug.fanxiaobao.xyz

JS:   s.split(/\r?\n/)
来源：http://yrf.kuanghao11.cn

TS:   s.split(/\r?\n/)
来源：http://eoz.pengpengdd.cyou

Java: s.lines().toList()
来源：http://mrj.zycfv.cn

Go:   strings.Split(s, "\n")
来源：http://ade.fengsongda.top

Ruby: s.lines
来源：http://uso.ppjwa.cn

C#:   s.Split('\n')
来源：http://eyf.feifeiyinyue.top

[E20] 判断字符串是否为空
来源：http://vqw.kuanghao11.cn

Py:   if not s:
来源：http://xfb.jyoumei.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wdg.jqgufenzy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://han.jinqigufen.top

TS:   if (s === "") {}
来源：http://mil.jianghu66.top

Java: if (s.isEmpty()) {}
来源：http://wzz.gotoacloud.top

Go:   if s == "" {}
来源：http://gkp.zhiwuduotai.top

Ruby: if s.empty?
来源：http://hfs.fehbvm.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wfi.316326.xyz

[E21] 超长截断加省略号
来源：http://ebx.xziqi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lhl.fktsv.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jum.hcnkem.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nrt.iojbl.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://twk.cucudq.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://akl.ywan-chungtsiang.top

Go:   // 按 rune 判断长度后截断
来源：http://lue.sxryk.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qkf.meibo888.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://abf.fanxiaobao.xyz

[E22] 字节长度与字符长度
来源：http://uub.pengpengdd.cyou

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zaa.yanxiufei.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mxk.cheryme.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://amn.c1oappe.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vyo.hywenlv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vcx.yfazqb.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ngn.pengpengdd.cyou

Ruby: s.bytesize;  s.length
来源：http://req.yj202588.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://twv.gaohongyu789.top

================================================================================
来源：http://hnq.hongshengwenyu.top

F. 文件与目录
来源：http://bjc.sysykeji.top

================================================================================
来源：http://tnn.chenzaomai.com

[F01] 读取整个文件
来源：http://jfe.pengpengdd.cyou

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jko.52xcode.cn

PHP:  file_get_contents("a.txt");
来源：http://gdk.nanxuanxn.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jak.fanxiaobao.xyz


<!-- 参考信息 -->