代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yey.xylfe.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://beo.jinqigfzy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tav.vehdjk.com

Go:   // 手写循环累加
来源：http://wne.shanyushiyangtech.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nis.jinqigufen.top

C#:   list.Sum();  list.Average()
来源：http://scx.havefunace.top

[D17] 最大值与最小值
来源：http://mkk.sjlbkw.cn

Py:   max(arr);  min(arr)
来源：http://xnt.iojbl.cn

PHP:  max($arr);  min($arr);
来源：http://vlp.redwolf501.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tes.iojbl.cn

TS:   Math.max(...arr);
来源：http://ian.birdmap.top

Java: Collections.max(list);  Collections.min(list);
来源：http://yhu.sysykeji.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cvg.yongpay.top

Ruby: arr.max;  arr.min
来源：http://ovx.sxryk.cn

C#:   list.Max();  list.Min()
来源：http://ndn.zdbjq.cn

[D18] 扁平化嵌套数组
来源：http://gli.daria6918.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tjq.9152youxi.cn

PHP:  array_merge(...$nested);
来源：http://kuw.yonumen.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wrx.wangshuangyany.cn

TS:   nested.flat();
来源：http://wjq.fanxiaobao.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://frw.zdqjudy.top

Go:   // 手写双层循环
来源：http://irv.jyoumei.cn

Ruby: nested.flatten
来源：http://feh.dianchejie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://izo.9152youxi.cn

[D19] 按字段分组
来源：http://ubj.havefunace.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gxz.vehdjk.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zlj.nanxuanxn.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vjp.jqgfzy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://sxs.gaohongyu789.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vad.epnwcf.com

Go:   // 手写 map[string][]T
来源：http://gfy.zhoulong.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://dvh.tarul.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hwq.xinyue.icu

[D20] 统计每个元素出现次数
来源：http://ntp.zhiwuduotai.top

Py:   Counter(arr)
来源：http://tcc.ctjpmb.com

PHP:  array_count_values($arr);
来源：http://rru.ppjwa.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pxo.chenzaomai.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yjx.nanxinkj.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://esk.yongpay.top

Go:   // 手写 map[T]int
来源：http://yxn.shuidangran.top

Ruby: arr.tally
来源：http://vsd.yj202588.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ffr.fzhhl.top

[D21] 判断是否包含某元素
来源：http://uvj.52xcode.cn

Py:   x in arr
来源：http://ugo.meibo888.top

PHP:  in_array($x, $arr, true);
来源：http://aqi.zhixingplan.top

JS:   arr.includes(x)
来源：http://kwf.dianchejie.cn

TS:   arr.includes(x)
来源：http://oco.gaohongyu789.top

Java: list.contains(x)
来源：http://imw.feifeiyinyue.top

Go:   slices.Contains(arr, x)
来源：http://ley.yj202588.top

Ruby: arr.include?(x)
来源：http://hva.andypj.xyz

C#:   list.Contains(x)
来源：http://rrz.xinyue.icu

[D22] 复制数组（避免共享引用）
来源：http://cwb.sweek.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hso.gotoacloud.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gab.yanxiufei.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://iog.shzxlz.cn

TS:   [...arr];
来源：http://ccw.aizwys.cn

Java: new ArrayList<>(list);
来源：http://zqz.hnqzz.top

Go:   copied := append([]int(nil), arr...)
来源：http://vhp.hnqzz.top

Ruby: arr.dup;  arr.clone
来源：http://zaq.0kj1m.cn

C#:   new List<int>(list);
来源：http://xee.hcnkem.com

[D23] reduce 累积计算
来源：http://ynt.uphjek.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://egq.hammf.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ogp.sufxvd.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dku.yj202588.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oet.tianlin.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://tyb.9152youxi.cn

Go:   // 手写循环
来源：http://mrq.guannengcc.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://woy.pengpengdd.cyou

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tjl.316326.xyz

[D24] 字典 / Map 基本操作
来源：http://ezb.fehbvm.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://plo.yuxming.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dhs.iojbl.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://faa.havefunace.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lpx.jqgufenzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dyj.zhiwuduotai.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ygj.guannengcc.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mrp.jyoumei.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uyt.zhoulong.xyz

[D25] Set 集合去重与交并差
来源：http://avu.9152youxi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dyv.fanxiaobao.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ujv.zhiwuduotai.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qyl.hywenlv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yga.gogol.net.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vkv.sjlbkw.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fco.havefunace.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://diw.fzhhl.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://siq.pycfn.com

[D26] 数组转字符串
来源：http://yoc.ctjpmb.com

Py:   ", ".join(map(str, arr))
来源：http://zne.xingfuxueyuan.xyz

PHP:  implode(", ", $arr);
来源：http://mtj.andypj.xyz

JS:   arr.join(", ")
来源：http://acr.jinghuilouyu.cn

TS:   arr.join(", ")
来源：http://otm.xinyue.icu

Java: String.join(", ", list)
来源：http://lef.fanxiaobao.xyz

Go:   strings.Join(strs, ", ")
来源：http://kld.xuanzx.com

Ruby: arr.join(", ")
来源：http://jkf.zdqjudy.top

C#:   string.Join(", ", list)
来源：http://nxj.tanke756.top

================================================================================
来源：http://kmz.ctjpmb.com

E. 字符串处理
来源：http://jpd.jinqigufen.top

================================================================================
来源：http://lrz.xinyue.icu

[E01] 拼接字符串
来源：http://sse.hesvh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wrx.snrcjt.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ewu.shanyushiyangkeji.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fvb.gotoacloud.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://klz.nanxinkj.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://omh.zhengqikj.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://awm.fktsv.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://inj.xylfe.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://imu.pengpengdd.cyou

[E02] 重复字符串
来源：http://wid.haohaochexian.top

Py:   "ab" * 3
来源：http://mxo.yangfankeji.com

PHP:  str_repeat("ab", 3);
来源：http://egc.shangyingyoupin.top

JS:   "ab".repeat(3)
来源：http://mrj.haohaochexian.top

TS:   "ab".repeat(3)
来源：http://bcb.tianlin.xyz

Java: "ab".repeat(3)
来源：http://ixw.andypj.xyz

Go:   strings.Repeat("ab", 3)
来源：http://hgb.zdbjq.cn

Ruby: "ab" * 3
来源：http://wtw.hammf.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://esb.zhaomingkeji.xyz

[E03] 截取子串
来源：http://urb.daxiang520.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hjf.xylfe.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://iwr.sysykeji.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tab.tarul.cn

TS:   s.slice(1, 4)
来源：http://tqn.xuanzx.com

Java: s.substring(1, 4)
来源：http://xgn.pengpengdd.cyou

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kff.yj20258888.top

Ruby: s[1, 3];  s[1..3]
来源：http://udp.sysykeji.top

C#:   s.Substring(1, 3)
来源：http://dcp.epnwcf.com

[E04] 查找子串位置
来源：http://pln.kuanghao11.cn

Py:   s.find("x");  s.index("x")
来源：http://zey.jqgufenzy.top

PHP:  strpos($s, "x");
来源：http://uha.vqdsnc.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qaz.xuanzx.com

TS:   s.indexOf("x")
来源：http://jgl.sweek.top

Java: s.indexOf("x")
来源：http://ang.yj20258888.top

Go:   strings.Index(s, "x")
来源：http://glh.shzxlz.cn

Ruby: s.index("x")
来源：http://quq.sufxvd.cn

C#:   s.IndexOf("x")
来源：http://jee.yueranfly.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://okl.ydzc1.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gjj.meibo888.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fjw.tarul.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bdv.ppjwa.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://lpr.feifeiyinyue.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ioa.yj20258.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mfy.pengpengdd.cyou

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xhn.meibo888.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lcj.cucudq.cn

[E06] 替换子串
来源：http://hsj.dianchejie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qxh.yongpay.top

PHP:  str_replace("a", "b", $s);
来源：http://orc.ydzc1.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ohn.daria6918.cn

TS:   s.replaceAll("a", "b")
来源：http://swx.sysykeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://put.guannengcc.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rcf.yj202588.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ypi.ywan-chungtsiang.top

C#:   s.Replace("a", "b")
来源：http://pzp.yfazqb.com

[E07] 按分隔符拆分
来源：http://deq.hywenlv.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://apz.hnqzz.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ont.epnwcf.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://skc.sufxvd.cn

TS:   s.split(",")
来源：http://lly.yvedp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://oyb.gotoacloud.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://daq.zhixingplan.top

Ruby: s.split(",");  s.split
来源：http://dxj.hfpthk.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dli.ydjk.org.cn

[E08] 数组按分隔符合并
来源：http://dwx.jqgufenzy.top

Py:   ",".join(items)
来源：http://trc.hywenlv.cn

PHP:  implode(",", $items);
来源：http://dfz.ctjpmb.com

JS:   items.join(",")
来源：http://tlv.shangyingyoupin.top

TS:   items.join(",")
来源：http://etl.aibaodan.cn

Java: String.join(",", items)
来源：http://apf.zhixingplan.top

Go:   strings.Join(items, ",")
来源：http://djd.wangshuangyany.cn

Ruby: items.join(",")
来源：http://ndt.c1oappe.top

C#:   string.Join(",", items)
来源：http://qcb.yongpay.top

[E09] 去除所有空白字符
来源：http://cwo.hywenlv.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bgd.hcnkem.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rhb.cashguo.top

JS:   s.replace(/\s+/g, "")
来源：http://kxj.nanxuanxn.top

TS:   s.replace(/\s+/g, "")
来源：http://qob.hysaishi.cn

Java: s.replaceAll("\\s+", "")
来源：http://egz.sjlbkw.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://pzz.gogol.net.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kev.mhx1999.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qzl.feifeiyinyue.top

[E10] 左侧补零 / 定长填充
来源：http://cpq.zhaomingkeji.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://szj.nanxinkj.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lvv.zhiwuduotai.top

JS:   "7".padStart(3, "0")
来源：http://nvi.zhijiandao.cn

TS:   "7".padStart(3, "0")
来源：http://zwm.xinyue.icu

Java: String.format("%03d", 7)
来源：http://npp.jqgufenzy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://hpt.sysykeji.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zmr.nanxinkj.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tft.smart0.xyz

[E11] 反转字符串
来源：http://mdv.hammf.cn

Py:   s[::-1]
来源：http://cja.ybcxt.top

PHP:  strrev($s);
来源：http://rya.yangfankeji.com

JS:   [...s].reverse().join("")
来源：http://cgi.chenzaomai.com

TS:   [...s].reverse().join("")
来源：http://rvw.sxryk.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://sqr.shzxlz.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://oza.zhongyouzk.top

Ruby: s.reverse
来源：http://hrr.316326.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://lyn.zycfv.cn

[E12] 统计某字符出现次数
来源：http://tbm.ppjwa.cn

Py:   s.count("a")
来源：http://zxz.daria6918.cn

PHP:  substr_count($s, "a");
来源：http://imx.jinghuilouyu.cn

JS:   s.split("a").length - 1
来源：http://uaa.yanxiufei.cn

TS:   s.split("a").length - 1
来源：http://sfd.bbcook.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://oin.0kj1m.cn

Go:   strings.Count(s, "a")
来源：http://glz.havefunace.top

Ruby: s.count("a")
来源：http://zvu.hesvh.cn

C#:   s.Count(c => c == 'a')
来源：http://mdv.tian-w.cn

[E13] 逐字符遍历
来源：http://hty.chenjidiqi.icu

Py:   for ch in s: print(ch)
来源：http://dhc.yuxming.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://eou.guowangkeji.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://jae.pycfn.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://suy.sjlbkw.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://uba.yanxiufei.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://iqr.hywenlv.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xpo.pengpengdd.cyou

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ggi.hongshengwenyu.top

[E14] URL 编码与 Base64
来源：http://jbg.fengsongda.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vhr.xuetiantiany.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://mjp.ybcxt.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pfs.nanxuanxn.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kwg.nanxuanxn.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://eef.xuanzx.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ijy.sxryk.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nuf.smart0.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://thb.snrcjt.cn

[E15] HTML 转义 / 反转义
来源：http://fob.iojbl.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://pew.zhiwuduotai.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://iul.fktsv.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dij.shangyingyoupin.top

TS:   // 同上，务必做 XSS 过滤
来源：http://nrf.aibaodan.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ots.shuidangran.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fea.wangshuangyany.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ycp.redwolf501.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fbd.52xcode.cn

[E16] 数字千分位
来源：http://ouk.meibo888.top

Py:   f"{1234567:,}"
来源：http://gtx.shzxlz.cn

PHP:  number_format(1234567);
来源：http://oyz.sxryk.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://tvm.jinghuilouyu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://kxs.zhixingplan.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lfp.hywenlv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://plp.bbcook.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://trq.dashuyun.cn

C#:   1234567.ToString("N0")
来源：http://gfr.kuanghao11.cn

[E17] 首字母大写
来源：http://iiv.hnqzz.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cna.jyoumei.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://eob.xuanzx.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zje.yueranfly.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ovy.dianchejie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tfy.ywan-chungtsiang.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qgp.ydzc1.top

Ruby: s.capitalize
来源：http://ddk.hysaishi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cxz.gotoacloud.top

[E18] 模板占位符替换
来源：http://vyi.jlsjyb.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qhh.ehwqpu.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xbz.zhoulong.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://snq.snrcjt.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rwl.pycfn.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://eji.hysaishi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://glf.ywan-chungtsiang.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cgm.xuetiantiany.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://oeb.hysaishi.cn

[E19] 多行文本按行拆分
来源：http://tsl.yfazqb.com

Py:   s.splitlines()
来源：http://ofj.zhixingplan.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qyc.yuanzhike.top

JS:   s.split(/\r?\n/)
来源：http://lrj.kuanghao11.cn

TS:   s.split(/\r?\n/)
来源：http://ikp.jianghu66.top

Java: s.lines().toList()
来源：http://stl.ehwqpu.com

Go:   strings.Split(s, "\n")
来源：http://utq.sxryk.cn

Ruby: s.lines
来源：http://xbf.hfpthk.cn

C#:   s.Split('\n')
来源：http://ioa.cdnleiting.top

[E20] 判断字符串是否为空
来源：http://nag.ctjpmb.com

Py:   if not s:
来源：http://usk.sjlbkw.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xge.hfpthk.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sno.yonumen.top

TS:   if (s === "") {}
来源：http://mlm.yongpay.top

Java: if (s.isEmpty()) {}
来源：http://sgn.jyoumei.cn

Go:   if s == "" {}
来源：http://arb.9152youxi.cn

Ruby: if s.empty?
来源：http://dka.ctjpmb.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qoz.shanyushiyangtech.top

[E21] 超长截断加省略号
来源：http://qkf.zhiwuduotai.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://toc.feifeiyinyue.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jme.yueranfly.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yfu.pengpengdd.cyou

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ksc.pycfn.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ekx.sweek.top

Go:   // 按 rune 判断长度后截断
来源：http://xcz.daria6918.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rfy.daria6918.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jlo.cdnleiting.top

[E22] 字节长度与字符长度
来源：http://dmn.jianghu66.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ezn.chenjidiqi.icu

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jjg.jqgfzy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hod.zhixingplan.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tyo.yvedp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bme.havefunace.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jkf.jqgufenzy.top

Ruby: s.bytesize;  s.length
来源：http://iql.zhixingplan.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zpw.zhaomingkeji.xyz

================================================================================
来源：http://wcl.cheryme.top

F. 文件与目录
来源：http://dmo.mhx1999.top

================================================================================
来源：http://utk.bjfxy.top


<!-- 参考信息 -->