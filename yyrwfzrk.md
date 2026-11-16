代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qpa.xylfe.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gyw.epnwcf.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qjx.chenlongwang.top

Go:   // 手写循环累加
来源：http://yqs.yonumen.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kzy.tarul.cn

C#:   list.Sum();  list.Average()
来源：http://zsi.xuanzx.com

[D17] 最大值与最小值
来源：http://dvn.snrcjt.cn

Py:   max(arr);  min(arr)
来源：http://hns.ydjk.org.cn

PHP:  max($arr);  min($arr);
来源：http://ooj.zhoulong.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ysz.dashuyun.cn

TS:   Math.max(...arr);
来源：http://ilo.xinyue.icu

Java: Collections.max(list);  Collections.min(list);
来源：http://wsy.tianlin.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yqj.fengsongda.top

Ruby: arr.max;  arr.min
来源：http://pmi.zhiwuduotai.top

C#:   list.Max();  list.Min()
来源：http://zue.zhengqikj.top

[D18] 扁平化嵌套数组
来源：http://okz.aizwys.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lms.tanke756.top

PHP:  array_merge(...$nested);
来源：http://jna.pycfn.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://aud.quarkkingdee.top

TS:   nested.flat();
来源：http://dec.zhengqikj.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qmz.yuxming.cn

Go:   // 手写双层循环
来源：http://khn.aibaodan.cn

Ruby: nested.flatten
来源：http://snq.fengsongda.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://kqd.jqgfzy.top

[D19] 按字段分组
来源：http://uos.daria6918.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wxu.hysaishi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ykr.52xcode.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bao.ctjpmb.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://ktn.tanke756.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dcc.fehbvm.com

Go:   // 手写 map[string][]T
来源：http://aim.chenzaomai.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://yng.ydzc1.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bpi.tarul.cn

[D20] 统计每个元素出现次数
来源：http://uny.jianghu66.top

Py:   Counter(arr)
来源：http://hdq.316326.xyz

PHP:  array_count_values($arr);
来源：http://ske.aizwys.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sjn.svipenyu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wzx.chenzaomai.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ggw.nanxuanxn.top

Go:   // 手写 map[T]int
来源：http://vmx.gogol.net.cn

Ruby: arr.tally
来源：http://tkl.sysykeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sti.feifeiyinyue.top

[D21] 判断是否包含某元素
来源：http://ggz.quarkkingdee.top

Py:   x in arr
来源：http://yyh.ydjk.org.cn

PHP:  in_array($x, $arr, true);
来源：http://zhd.quarkkingdee.top

JS:   arr.includes(x)
来源：http://qky.yonumen.top

TS:   arr.includes(x)
来源：http://gwk.ydjk.org.cn

Java: list.contains(x)
来源：http://mit.jqgfzy.top

Go:   slices.Contains(arr, x)
来源：http://tra.chenlongwang.top

Ruby: arr.include?(x)
来源：http://pcz.snrcjt.cn

C#:   list.Contains(x)
来源：http://lzk.hfpthk.cn

[D22] 复制数组（避免共享引用）
来源：http://tuk.ppjwa.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fue.nwbrower.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sqs.gogol.net.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://djc.uphjek.com

TS:   [...arr];
来源：http://dnr.wangshuangyany.cn

Java: new ArrayList<>(list);
来源：http://lkz.jinqigfzy.top

Go:   copied := append([]int(nil), arr...)
来源：http://unr.hongshengwenyu.top

Ruby: arr.dup;  arr.clone
来源：http://ucd.nanxinkj.top

C#:   new List<int>(list);
来源：http://qgc.hesvh.cn

[D23] reduce 累积计算
来源：http://ekw.jinghuilouyu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hxs.tianlin.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yyt.sxryk.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ygi.quarkkingdee.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nks.shanyushiyangkeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://wde.yuanzhike.top

Go:   // 手写循环
来源：http://dvd.zdbjq.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://erc.birdmap.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gwj.yj20258.top

[D24] 字典 / Map 基本操作
来源：http://muy.svipenyu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ktq.daria6918.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fsa.smart0.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://evv.xziqi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://oki.cucudq.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ckx.yfazqb.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fzj.zhoulong.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ykc.epnwcf.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ceb.sufxvd.cn

[D25] Set 集合去重与交并差
来源：http://sdq.havefunace.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://epl.jyoumei.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ngt.chenzaomai.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://klo.sjlbkw.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://epx.jiagoushi.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kyf.bbcook.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kfe.gaohongyu789.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uyo.52xcode.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kch.yfazqb.com

[D26] 数组转字符串
来源：http://rco.uphjek.com

Py:   ", ".join(map(str, arr))
来源：http://fee.zhixingplan.top

PHP:  implode(", ", $arr);
来源：http://asi.fanxiaobao.xyz

JS:   arr.join(", ")
来源：http://gmt.52xcode.cn

TS:   arr.join(", ")
来源：http://ots.birdmap.top

Java: String.join(", ", list)
来源：http://lbz.nwbrower.top

Go:   strings.Join(strs, ", ")
来源：http://vvp.jinqigfzy.top

Ruby: arr.join(", ")
来源：http://kee.kuanghao11.cn

C#:   string.Join(", ", list)
来源：http://ang.ybcxt.top

================================================================================
来源：http://niz.haohaochexian.top

E. 字符串处理
来源：http://bmy.jqgfzy.top

================================================================================
来源：http://kpj.haohaochexian.top

[E01] 拼接字符串
来源：http://qon.snrcjt.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://act.hfpthk.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://plf.smart0.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ujk.cdnleiting.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yfa.jqgufenzy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kyx.jinqigfzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://goo.sweek.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://onm.zdbjq.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fis.zhongyouzk.top

[E02] 重复字符串
来源：http://lfa.cdnleiting.top

Py:   "ab" * 3
来源：http://zuo.zhongyouzk.top

PHP:  str_repeat("ab", 3);
来源：http://slb.dashuyun.cn

JS:   "ab".repeat(3)
来源：http://lcu.sxryk.cn

TS:   "ab".repeat(3)
来源：http://kzb.ehwqpu.com

Java: "ab".repeat(3)
来源：http://ypy.iojbl.cn

Go:   strings.Repeat("ab", 3)
来源：http://huu.nanxuanxn.top

Ruby: "ab" * 3
来源：http://joc.gogol.net.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qal.bjfxy.top

[E03] 截取子串
来源：http://iez.andypj.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jdz.yj202588.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xgs.chenjidiqi.icu

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ggd.zhengqikj.top

TS:   s.slice(1, 4)
来源：http://jai.hnqzz.top

Java: s.substring(1, 4)
来源：http://jen.gaohongyu789.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xxu.fengsongda.top

Ruby: s[1, 3];  s[1..3]
来源：http://igo.cucudq.cn

C#:   s.Substring(1, 3)
来源：http://duz.zhixingplan.top

[E04] 查找子串位置
来源：http://ytc.daxiang520.top

Py:   s.find("x");  s.index("x")
来源：http://lbj.zhengqikj.top

PHP:  strpos($s, "x");
来源：http://rro.tianlin.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wzg.zdqjudy.top

TS:   s.indexOf("x")
来源：http://equ.gzhubu.top

Java: s.indexOf("x")
来源：http://xbu.yvedp.cn

Go:   strings.Index(s, "x")
来源：http://xwx.jinyuanbaomall.cn

Ruby: s.index("x")
来源：http://njp.hammf.cn

C#:   s.IndexOf("x")
来源：http://zyh.hesvh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://kvt.316326.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cps.ydjk.org.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hnm.chenjidiqi.icu

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rah.yuanzhike.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://pzt.chenzaomai.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://upm.sufxvd.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hkr.mhx1999.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jbt.svipenyu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ztt.dashuyun.cn

[E06] 替换子串
来源：http://wub.pengpengdd.cyou

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dui.zycfv.cn

PHP:  str_replace("a", "b", $s);
来源：http://vuy.ywan-chungtsiang.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cwj.hongshengwenyu.top

TS:   s.replaceAll("a", "b")
来源：http://jvl.jianghu66.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sdv.jinghuilouyu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wux.xinyue.icu

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zoh.aibaodan.cn

C#:   s.Replace("a", "b")
来源：http://jyb.aizwys.cn

[E07] 按分隔符拆分
来源：http://etp.hesvh.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bnf.ctjpmb.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://upc.aibaodan.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://xsk.yj202588.top

TS:   s.split(",")
来源：http://gvr.ctjpmb.com

Java: s.split(",");  s.split("\\s+")
来源：http://qib.jqgfzy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ymu.hesvh.cn

Ruby: s.split(",");  s.split
来源：http://jle.yonumen.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://buk.hysaishi.cn

[E08] 数组按分隔符合并
来源：http://yku.guowangkeji.top

Py:   ",".join(items)
来源：http://cfz.shanyushiyangkeji.top

PHP:  implode(",", $items);
来源：http://lks.zycfv.cn

JS:   items.join(",")
来源：http://cdq.fktsv.cn

TS:   items.join(",")
来源：http://cpl.yj202588.top

Java: String.join(",", items)
来源：http://onq.cqqwz.cn

Go:   strings.Join(items, ",")
来源：http://hpz.jqgufenzy.top

Ruby: items.join(",")
来源：http://qjb.hesvh.cn

C#:   string.Join(",", items)
来源：http://wuf.yuxming.cn

[E09] 去除所有空白字符
来源：http://mfe.svipenyu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mge.fehbvm.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ubi.zhoulong.xyz

JS:   s.replace(/\s+/g, "")
来源：http://njs.316326.xyz

TS:   s.replace(/\s+/g, "")
来源：http://ndm.feifeiyinyue.top

Java: s.replaceAll("\\s+", "")
来源：http://fpn.ehwqpu.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://kbr.xylfe.cn

Ruby: s.gsub(/\s+/, "")
来源：http://php.c1oappe.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://scm.ywan-chungtsiang.top

[E10] 左侧补零 / 定长填充
来源：http://crc.fktsv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zlf.hywenlv.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dpp.fehbvm.com

JS:   "7".padStart(3, "0")
来源：http://hns.cucudq.cn

TS:   "7".padStart(3, "0")
来源：http://zfu.jinqigfzy.top

Java: String.format("%03d", 7)
来源：http://rlb.meibo888.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://zjm.ppjwa.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jgw.zhixingplan.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qip.vqdsnc.cn

[E11] 反转字符串
来源：http://qmp.316326.xyz

Py:   s[::-1]
来源：http://lid.jqgfzy.top

PHP:  strrev($s);
来源：http://rok.zhongyouzk.top

JS:   [...s].reverse().join("")
来源：http://rlo.jlsjyb.cn

TS:   [...s].reverse().join("")
来源：http://rse.wangshuangyany.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://awr.zdqjudy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://tvs.shzxlz.cn

Ruby: s.reverse
来源：http://qem.shuidangran.top

C#:   new string(s.Reverse().ToArray())
来源：http://lnf.fehbvm.com

[E12] 统计某字符出现次数
来源：http://myi.zdqjudy.top

Py:   s.count("a")
来源：http://oal.andypj.xyz

PHP:  substr_count($s, "a");
来源：http://kmd.hammf.cn

JS:   s.split("a").length - 1
来源：http://prc.cucudq.cn

TS:   s.split("a").length - 1
来源：http://fpd.iojbl.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vil.fanxiaobao.xyz

Go:   strings.Count(s, "a")
来源：http://bak.wangshuangyany.cn

Ruby: s.count("a")
来源：http://dle.xinyue.icu

C#:   s.Count(c => c == 'a')
来源：http://ezi.sxryk.cn

[E13] 逐字符遍历
来源：http://dfi.jqgfzy.top

Py:   for ch in s: print(ch)
来源：http://sdp.sweek.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dgi.kuanghao11.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://uyl.nanxuanxn.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://jbe.hammf.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://von.jinyuanbaomall.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://igt.yvedp.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://gnb.dashuyun.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tpo.gzhubu.top

[E14] URL 编码与 Base64
来源：http://xqh.yanxiufei.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ump.hfpthk.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://eyy.jyoumei.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zgj.tianlin.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nwk.bbcook.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tcj.jqgufenzy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hub.kuanghao11.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lyb.sysykeji.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zbx.meibo888.top

[E15] HTML 转义 / 反转义
来源：http://tco.yonumen.top

Py:   html.escape(s);  html.unescape(s)
来源：http://deq.316326.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tzz.smart0.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mtw.guannengcc.top

TS:   // 同上，务必做 XSS 过滤
来源：http://arl.shanyushiyangkeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jtr.zdqjudy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vxo.sysykeji.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://clz.hnxiangtu.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rkp.wangshuangyany.cn

[E16] 数字千分位
来源：http://apt.52xcode.cn

Py:   f"{1234567:,}"
来源：http://kaq.316326.xyz

PHP:  number_format(1234567);
来源：http://gis.fengsongda.top

JS:   (1234567).toLocaleString("en-US")
来源：http://lyu.xuetiantiany.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fsy.ppjwa.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kkx.feifeiyinyue.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wmn.birdmap.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cks.gzhubu.top

C#:   1234567.ToString("N0")
来源：http://nrv.52xcode.cn

[E17] 首字母大写
来源：http://sms.kuanghao11.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zzk.xuetiantiany.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://rma.snrcjt.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ddn.316326.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lut.yvedp.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ies.0kj1m.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ywa.hysaishi.cn

Ruby: s.capitalize
来源：http://dgh.cdnleiting.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pzc.316326.xyz

[E18] 模板占位符替换
来源：http://nyj.hnxiangtu.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xtn.ppjwa.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gpz.yanxiufei.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ypc.zycfv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://cuz.52xcode.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://juh.redwolf501.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jpb.smart0.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nti.cdnleiting.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nrn.smart0.xyz

[E19] 多行文本按行拆分
来源：http://qcy.zhixingplan.top

Py:   s.splitlines()
来源：http://vnv.bjfxy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zol.jqgfzy.top

JS:   s.split(/\r?\n/)
来源：http://bbj.feifeiyinyue.top

TS:   s.split(/\r?\n/)
来源：http://dnm.c1oappe.top

Java: s.lines().toList()
来源：http://eri.daxiang520.top

Go:   strings.Split(s, "\n")
来源：http://bgp.jianghu66.top

Ruby: s.lines
来源：http://nwx.xingfuxueyuan.xyz

C#:   s.Split('\n')
来源：http://wfe.zdbjq.cn

[E20] 判断字符串是否为空
来源：http://pbz.zycfv.cn

Py:   if not s:
来源：http://bfk.tian-w.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ylh.quarkkingdee.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://who.zhengqikj.top

TS:   if (s === "") {}
来源：http://hkl.jinyuanbaomall.cn

Java: if (s.isEmpty()) {}
来源：http://iru.aibaodan.cn

Go:   if s == "" {}
来源：http://dzf.yueranfly.top

Ruby: if s.empty?
来源：http://tir.hnxiangtu.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://npk.jinghuilouyu.cn

[E21] 超长截断加省略号
来源：http://btq.yueranfly.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ybf.mhx1999.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ngb.jlsjyb.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yau.snrcjt.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pyl.zhoulong.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://olx.jqgufenzy.top

Go:   // 按 rune 判断长度后截断
来源：http://bbe.daria6918.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://epg.daria6918.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cfs.xziqi.cn

[E22] 字节长度与字符长度
来源：http://dpq.hfpthk.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qmy.jinqigfzy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aqb.chenjidiqi.icu

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jsr.cdnleiting.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dzc.vqdsnc.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ynz.ybcxt.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://aol.gotoacloud.top

Ruby: s.bytesize;  s.length
来源：http://nwd.xinyue.icu

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ofi.xuanzx.com

================================================================================
来源：http://tuw.hcnkem.com

F. 文件与目录
来源：http://uua.shzxlz.cn

================================================================================
来源：http://bbb.shuidangran.top


<!-- 参考信息 -->