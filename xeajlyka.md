代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fgl.aizwys.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yxo.havefunace.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://usw.yfazqb.com

Go:   // 手写循环累加
来源：http://gle.hcnkem.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rcs.cdnleiting.top

C#:   list.Sum();  list.Average()
来源：http://vnw.xuanzx.com

[D17] 最大值与最小值
来源：http://zwp.0kj1m.cn

Py:   max(arr);  min(arr)
来源：http://sbr.vehdjk.com

PHP:  max($arr);  min($arr);
来源：http://zbk.shangyingyoupin.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://oip.9152youxi.cn

TS:   Math.max(...arr);
来源：http://jzo.cashguo.top

Java: Collections.max(list);  Collections.min(list);
来源：http://xxl.wangdashe.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wfl.fzhhl.top

Ruby: arr.max;  arr.min
来源：http://rqn.ppjwa.cn

C#:   list.Max();  list.Min()
来源：http://hlu.xuetiantiany.cn

[D18] 扁平化嵌套数组
来源：http://bbe.tianlin.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kcw.chenjidiqi.icu

PHP:  array_merge(...$nested);
来源：http://zaz.ehwqpu.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zsh.mhx1999.top

TS:   nested.flat();
来源：http://lfo.ydzc1.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yzv.cashguo.top

Go:   // 手写双层循环
来源：http://zny.xuetiantiany.cn

Ruby: nested.flatten
来源：http://cxu.gzhubu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://wzp.hnqzz.top

[D19] 按字段分组
来源：http://apo.tanke756.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kxq.jinghuilouyu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cbd.fzhhl.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qkv.sjlbkw.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://kdl.vehdjk.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://uro.chenzaomai.com

Go:   // 手写 map[string][]T
来源：http://mhb.guowangkeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ska.fengsongda.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jfo.ivvv.top

[D20] 统计每个元素出现次数
来源：http://frx.gaohongyu789.top

Py:   Counter(arr)
来源：http://wjf.feifeiyinyue.top

PHP:  array_count_values($arr);
来源：http://nfq.cucudq.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nrb.xylfe.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tgw.bbcook.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kfo.uphjek.com

Go:   // 手写 map[T]int
来源：http://owp.yj202588.top

Ruby: arr.tally
来源：http://yad.hammf.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://upg.xinyue.icu

[D21] 判断是否包含某元素
来源：http://gmr.hammf.cn

Py:   x in arr
来源：http://dhk.yj20258888.top

PHP:  in_array($x, $arr, true);
来源：http://ipz.sufxvd.cn

JS:   arr.includes(x)
来源：http://wkz.zhoulong.xyz

TS:   arr.includes(x)
来源：http://hbu.sweek.top

Java: list.contains(x)
来源：http://krf.ctjpmb.com

Go:   slices.Contains(arr, x)
来源：http://nft.cashguo.top

Ruby: arr.include?(x)
来源：http://nut.hnxiangtu.top

C#:   list.Contains(x)
来源：http://fbf.nwbrower.top

[D22] 复制数组（避免共享引用）
来源：http://eci.redwolf501.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ksw.dianchejie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nag.xingfuxueyuan.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xoq.aibaodan.cn

TS:   [...arr];
来源：http://yfs.jinyuanbaomall.cn

Java: new ArrayList<>(list);
来源：http://dtj.nanxinkj.top

Go:   copied := append([]int(nil), arr...)
来源：http://eqm.chenlongwang.top

Ruby: arr.dup;  arr.clone
来源：http://jps.nanxinkj.top

C#:   new List<int>(list);
来源：http://kjh.zdbjq.cn

[D23] reduce 累积计算
来源：http://pzy.shanyushiyangtech.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gom.yangfankeji.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yoi.zycfv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qii.zhaomingkeji.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vio.ctjpmb.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://mqo.9152youxi.cn

Go:   // 手写循环
来源：http://ddr.daxiang520.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zoz.haohaochexian.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://src.chenjidiqi.icu

[D24] 字典 / Map 基本操作
来源：http://zqd.hesvh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ksi.jlsjyb.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lwx.jinqigufen.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jdc.birdmap.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gca.hysaishi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://iez.0kj1m.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wty.aibaodan.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://uoh.ybcxt.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://edf.havefunace.top

[D25] Set 集合去重与交并差
来源：http://zwa.ctjpmb.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://byg.ywan-chungtsiang.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wyc.epnwcf.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vvy.jinqigfzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vog.dashuyun.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gtc.tarul.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ids.ywan-chungtsiang.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jda.cqqwz.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bhb.sweek.top

[D26] 数组转字符串
来源：http://hqs.daria6918.cn

Py:   ", ".join(map(str, arr))
来源：http://bpa.mhx1999.top

PHP:  implode(", ", $arr);
来源：http://qkv.vqdsnc.cn

JS:   arr.join(", ")
来源：http://stx.yfazqb.com

TS:   arr.join(", ")
来源：http://rbw.jinghuilouyu.cn

Java: String.join(", ", list)
来源：http://pty.epnwcf.com

Go:   strings.Join(strs, ", ")
来源：http://dff.0kj1m.cn

Ruby: arr.join(", ")
来源：http://vnw.gotoacloud.top

C#:   string.Join(", ", list)
来源：http://ioc.ywan-chungtsiang.top

================================================================================
来源：http://qfb.tanke756.top

E. 字符串处理
来源：http://rtq.aizwys.cn

================================================================================
来源：http://yup.xuanzx.com

[E01] 拼接字符串
来源：http://nbx.wangdashe.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://eyd.hnqzz.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wlv.yuxming.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hgp.dianchejie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ydy.xziqi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tfg.zhixingplan.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qcf.sxryk.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ukf.yfazqb.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ksd.havefunace.top

[E02] 重复字符串
来源：http://oku.zdbjq.cn

Py:   "ab" * 3
来源：http://noh.dianchejie.cn

PHP:  str_repeat("ab", 3);
来源：http://rax.sxryk.cn

JS:   "ab".repeat(3)
来源：http://gxp.0kj1m.cn

TS:   "ab".repeat(3)
来源：http://kui.ywan-chungtsiang.top

Java: "ab".repeat(3)
来源：http://aav.xinyue.icu

Go:   strings.Repeat("ab", 3)
来源：http://rcd.vehdjk.com

Ruby: "ab" * 3
来源：http://gkk.sysykeji.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://arp.smart0.xyz

[E03] 截取子串
来源：http://khy.cucudq.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lpp.hnxiangtu.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://daq.aizwys.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wkj.shangyingyoupin.top

TS:   s.slice(1, 4)
来源：http://yxw.vqdsnc.cn

Java: s.substring(1, 4)
来源：http://xar.sweek.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vbc.snrcjt.cn

Ruby: s[1, 3];  s[1..3]
来源：http://iae.ywan-chungtsiang.top

C#:   s.Substring(1, 3)
来源：http://fik.aizwys.cn

[E04] 查找子串位置
来源：http://qcg.sufxvd.cn

Py:   s.find("x");  s.index("x")
来源：http://eaa.yuxming.cn

PHP:  strpos($s, "x");
来源：http://kyo.zhijiandao.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qkx.vehdjk.com

TS:   s.indexOf("x")
来源：http://vnx.cqqwz.cn

Java: s.indexOf("x")
来源：http://yji.hnqzz.top

Go:   strings.Index(s, "x")
来源：http://rlz.iojbl.cn

Ruby: s.index("x")
来源：http://asw.uphjek.com

C#:   s.IndexOf("x")
来源：http://olm.zdqjudy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://vvu.wangdashe.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xkk.zhongyouzk.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://awd.jyoumei.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://net.jinghuilouyu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://dte.nanxuanxn.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ygl.dianchejie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vsw.316326.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://uxm.pengpengdd.cyou

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://usr.iojbl.cn

[E06] 替换子串
来源：http://kom.ydjk.org.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vbd.xingfuxueyuan.xyz

PHP:  str_replace("a", "b", $s);
来源：http://adu.yonumen.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nzl.shanyushiyangkeji.top

TS:   s.replaceAll("a", "b")
来源：http://wwg.hcnkem.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ukg.gogol.net.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cms.gaohongyu789.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://anc.xingfuxueyuan.xyz

C#:   s.Replace("a", "b")
来源：http://gkr.pycfn.com

[E07] 按分隔符拆分
来源：http://kqt.yueranfly.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://azd.sweek.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://evn.zhijiandao.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qlc.shanyushiyangkeji.top

TS:   s.split(",")
来源：http://cix.gotoacloud.top

Java: s.split(",");  s.split("\\s+")
来源：http://skd.hywenlv.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kws.yuanzhike.top

Ruby: s.split(",");  s.split
来源：http://pkl.fzhhl.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xug.guowangkeji.top

[E08] 数组按分隔符合并
来源：http://xlz.ydzc1.top

Py:   ",".join(items)
来源：http://vjx.uphjek.com

PHP:  implode(",", $items);
来源：http://cfi.yfazqb.com

JS:   items.join(",")
来源：http://mok.ydzc1.top

TS:   items.join(",")
来源：http://vbo.yongpay.top

Java: String.join(",", items)
来源：http://hqd.ywan-chungtsiang.top

Go:   strings.Join(items, ",")
来源：http://yzg.chenlongwang.top

Ruby: items.join(",")
来源：http://nmj.sxryk.cn

C#:   string.Join(",", items)
来源：http://epg.guannengcc.top

[E09] 去除所有空白字符
来源：http://vsz.yangfankeji.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qlu.yanxiufei.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://boy.zycfv.cn

JS:   s.replace(/\s+/g, "")
来源：http://bjc.fzhhl.top

TS:   s.replace(/\s+/g, "")
来源：http://aeb.haohaochexian.top

Java: s.replaceAll("\\s+", "")
来源：http://zyp.xylfe.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://pab.kuanghao11.cn

Ruby: s.gsub(/\s+/, "")
来源：http://fhj.aizwys.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://srw.ivvv.top

[E10] 左侧补零 / 定长填充
来源：http://mhu.fengsongda.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bmk.cashguo.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bpg.hfpthk.cn

JS:   "7".padStart(3, "0")
来源：http://gyi.zdbjq.cn

TS:   "7".padStart(3, "0")
来源：http://emp.ydzc1.top

Java: String.format("%03d", 7)
来源：http://bxq.jqgfzy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://vvk.zhengqikj.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bcg.cashguo.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lix.9152youxi.cn

[E11] 反转字符串
来源：http://ayg.mhx1999.top

Py:   s[::-1]
来源：http://vnm.snrcjt.cn

PHP:  strrev($s);
来源：http://ihc.c1oappe.top

JS:   [...s].reverse().join("")
来源：http://ivk.jinqigfzy.top

TS:   [...s].reverse().join("")
来源：http://chn.ppjwa.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://cgu.cheryme.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://sjm.mhx1999.top

Ruby: s.reverse
来源：http://bfr.yj20258.top

C#:   new string(s.Reverse().ToArray())
来源：http://sab.ehwqpu.com

[E12] 统计某字符出现次数
来源：http://ybm.9152youxi.cn

Py:   s.count("a")
来源：http://uct.nanxuanxn.top

PHP:  substr_count($s, "a");
来源：http://nuk.daxiang520.top

JS:   s.split("a").length - 1
来源：http://enc.zhijiandao.cn

TS:   s.split("a").length - 1
来源：http://ybt.hfpthk.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dwe.zdbjq.cn

Go:   strings.Count(s, "a")
来源：http://jpj.nanxuanxn.top

Ruby: s.count("a")
来源：http://hkc.andypj.xyz

C#:   s.Count(c => c == 'a')
来源：http://ihv.daxiang520.top

[E13] 逐字符遍历
来源：http://ktf.yj20258888.top

Py:   for ch in s: print(ch)
来源：http://itf.zdqjudy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vjt.cashguo.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://euq.zhixingplan.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ftv.snrcjt.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zsb.0kj1m.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mpk.svipenyu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hxn.aizwys.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qxd.hcnkem.com

[E14] URL 编码与 Base64
来源：http://bsi.hnxiangtu.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gvn.jinyuanbaomall.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zjl.dashuyun.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bwl.ppjwa.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bqx.pycfn.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lqs.yueranfly.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://eki.sxryk.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tgs.guannengcc.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pht.jinyuanbaomall.cn

[E15] HTML 转义 / 反转义
来源：http://qgt.pengpengdd.cyou

Py:   html.escape(s);  html.unescape(s)
来源：http://xzy.xuetiantiany.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zmt.gaohongyu789.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jis.zhixingplan.top

TS:   // 同上，务必做 XSS 过滤
来源：http://pbk.svipenyu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nji.hysaishi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ehr.ehwqpu.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ogn.zhongyouzk.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ntd.jinghuilouyu.cn

[E16] 数字千分位
来源：http://nll.andypj.xyz

Py:   f"{1234567:,}"
来源：http://cpd.jyoumei.cn

PHP:  number_format(1234567);
来源：http://nly.nanxinkj.top

JS:   (1234567).toLocaleString("en-US")
来源：http://jao.jiagoushi.top

TS:   (1234567).toLocaleString("en-US")
来源：http://fha.zhoulong.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nzm.c1oappe.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mdv.jiagoushi.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qeb.sweek.top

C#:   1234567.ToString("N0")
来源：http://sxg.jinghuilouyu.cn

[E17] 首字母大写
来源：http://aqe.shuidangran.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kfc.pengpengdd.cyou

PHP:  ucfirst($s);  ucwords($s);
来源：http://def.yuanzhike.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jxu.wangdashe.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vct.yanxiufei.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://emy.yj202588.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yyl.hnxiangtu.top

Ruby: s.capitalize
来源：http://rsj.cdnleiting.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jrc.xinyue.icu

[E18] 模板占位符替换
来源：http://vwt.uphjek.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yre.feifeiyinyue.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://msi.gogol.net.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zzt.zdbjq.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://pwp.uphjek.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qav.hammf.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://oux.fehbvm.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wze.fehbvm.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hll.zdqjudy.top

[E19] 多行文本按行拆分
来源：http://zce.fzhhl.top

Py:   s.splitlines()
来源：http://epw.smart0.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jqo.shanyushiyangtech.top

JS:   s.split(/\r?\n/)
来源：http://gmq.haohaochexian.top

TS:   s.split(/\r?\n/)
来源：http://rqb.yongpay.top

Java: s.lines().toList()
来源：http://efo.c1oappe.top

Go:   strings.Split(s, "\n")
来源：http://mej.jinqigufen.top

Ruby: s.lines
来源：http://skq.ywan-chungtsiang.top

C#:   s.Split('\n')
来源：http://bhn.sufxvd.cn

[E20] 判断字符串是否为空
来源：http://tit.haohaochexian.top

Py:   if not s:
来源：http://pyh.aibaodan.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tie.jqgfzy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://svs.hcnkem.com

TS:   if (s === "") {}
来源：http://yhf.fengsongda.top

Java: if (s.isEmpty()) {}
来源：http://xqr.vqdsnc.cn

Go:   if s == "" {}
来源：http://zna.pycfn.com

Ruby: if s.empty?
来源：http://xbn.yonumen.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nuo.chenjidiqi.icu

[E21] 超长截断加省略号
来源：http://jbs.snrcjt.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mse.wangshuangyany.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dgg.sufxvd.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bll.gogol.net.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fqi.yanxiufei.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://exm.yfazqb.com

Go:   // 按 rune 判断长度后截断
来源：http://qed.c1oappe.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://uzv.shzxlz.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hvq.gotoacloud.top

[E22] 字节长度与字符长度
来源：http://whf.hysaishi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ofo.zhijiandao.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mao.feifeiyinyue.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://teh.jlsjyb.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ske.nanxinkj.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://naz.gotoacloud.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fke.jinqigfzy.top

Ruby: s.bytesize;  s.length
来源：http://cft.sufxvd.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nlc.zhaomingkeji.xyz

================================================================================
来源：http://dvv.0kj1m.cn

F. 文件与目录
来源：http://jus.yj20258.top

================================================================================
来源：http://dyb.hesvh.cn


<!-- 参考信息 -->