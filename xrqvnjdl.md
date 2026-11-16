代发 wailian999

TS:   [...new Set(arr)]
来源：http://abg.zdqjudy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ohp.yongpay.top

Go:   // 用 map[T]struct{} 手写
来源：http://vnu.sysykeji.top

Ruby: arr.uniq
来源：http://tpb.chenjidiqi.icu

C#:   list.Distinct().ToList()
来源：http://kfr.haohaochexian.top

[D16] 求和与平均值
来源：http://cje.chenlongwang.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hvp.sufxvd.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://epp.yanxiufei.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sdw.sjlbkw.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nuz.ydjk.org.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yts.nwbrower.top

Go:   // 手写循环累加
来源：http://ygr.fengsongda.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dun.52xcode.cn

C#:   list.Sum();  list.Average()
来源：http://pcz.feifeiyinyue.top

[D17] 最大值与最小值
来源：http://rcr.zhoulong.xyz

Py:   max(arr);  min(arr)
来源：http://ebh.chenjidiqi.icu

PHP:  max($arr);  min($arr);
来源：http://otc.nanxuanxn.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kvz.yanxiufei.cn

TS:   Math.max(...arr);
来源：http://cbo.pycfn.com

Java: Collections.max(list);  Collections.min(list);
来源：http://amf.0kj1m.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wll.ctjpmb.com

Ruby: arr.max;  arr.min
来源：http://smo.jyoumei.cn

C#:   list.Max();  list.Min()
来源：http://uch.feifeiyinyue.top

[D18] 扁平化嵌套数组
来源：http://ach.xuetiantiany.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kkz.epnwcf.com

PHP:  array_merge(...$nested);
来源：http://gyo.mhx1999.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dso.jinqigfzy.top

TS:   nested.flat();
来源：http://crp.daria6918.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kps.gaohongyu789.top

Go:   // 手写双层循环
来源：http://qhs.quarkkingdee.top

Ruby: nested.flatten
来源：http://xay.cashguo.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://djk.kuanghao11.cn

[D19] 按字段分组
来源：http://kdw.nanxinkj.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jdw.cashguo.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://npg.tianlin.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vbi.hywenlv.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://uee.zhengqikj.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://azs.fzhhl.top

Go:   // 手写 map[string][]T
来源：http://qyx.xinyue.icu

Ruby: arr.group_by { |x| x[:type] }
来源：http://pws.xuetiantiany.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pvf.0kj1m.cn

[D20] 统计每个元素出现次数
来源：http://dwq.hesvh.cn

Py:   Counter(arr)
来源：http://hku.jinqigfzy.top

PHP:  array_count_values($arr);
来源：http://cpc.mhx1999.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bpd.tianlin.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rgq.svipenyu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qup.daria6918.cn

Go:   // 手写 map[T]int
来源：http://olj.redwolf501.top

Ruby: arr.tally
来源：http://cyr.guowangkeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xky.bjfxy.top

[D21] 判断是否包含某元素
来源：http://ace.fehbvm.com

Py:   x in arr
来源：http://usq.cdnleiting.top

PHP:  in_array($x, $arr, true);
来源：http://kes.tianlin.xyz

JS:   arr.includes(x)
来源：http://xik.yueranfly.top

TS:   arr.includes(x)
来源：http://xgv.tian-w.cn

Java: list.contains(x)
来源：http://jub.dashuyun.cn

Go:   slices.Contains(arr, x)
来源：http://ftn.xingfuxueyuan.xyz

Ruby: arr.include?(x)
来源：http://wcx.sweek.top

C#:   list.Contains(x)
来源：http://mra.jqgufenzy.top

[D22] 复制数组（避免共享引用）
来源：http://oyl.xingfuxueyuan.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://icd.bjfxy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bju.c1oappe.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wbn.pycfn.com

TS:   [...arr];
来源：http://feg.ctjpmb.com

Java: new ArrayList<>(list);
来源：http://rhi.zhoulong.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://uos.cashguo.top

Ruby: arr.dup;  arr.clone
来源：http://qwo.meibo888.top

C#:   new List<int>(list);
来源：http://qnc.sufxvd.cn

[D23] reduce 累积计算
来源：http://hsc.ywan-chungtsiang.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lam.shanyushiyangtech.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://reh.yonumen.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fos.fktsv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nsl.zhijiandao.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://whm.yueranfly.top

Go:   // 手写循环
来源：http://fsg.sufxvd.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dce.andypj.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ktu.guannengcc.top

[D24] 字典 / Map 基本操作
来源：http://wqb.haohaochexian.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ljh.quarkkingdee.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mxd.hfpthk.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cfk.aizwys.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wjg.guowangkeji.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pmr.uphjek.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wmb.xylfe.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mnq.hesvh.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lyv.hcnkem.com

[D25] Set 集合去重与交并差
来源：http://fro.yuanzhike.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mhc.snrcjt.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rsx.chenlongwang.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kxr.cheryme.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rue.tanke756.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fjc.cucudq.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yrm.gogol.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wlb.chenlongwang.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rll.nwbrower.top

[D26] 数组转字符串
来源：http://ubw.meibo888.top

Py:   ", ".join(map(str, arr))
来源：http://zoz.chenjidiqi.icu

PHP:  implode(", ", $arr);
来源：http://pzj.yuxming.cn

JS:   arr.join(", ")
来源：http://phk.yueranfly.top

TS:   arr.join(", ")
来源：http://mms.dianchejie.cn

Java: String.join(", ", list)
来源：http://uav.mhx1999.top

Go:   strings.Join(strs, ", ")
来源：http://dmx.zdqjudy.top

Ruby: arr.join(", ")
来源：http://mfp.yangfankeji.com

C#:   string.Join(", ", list)
来源：http://gnp.daria6918.cn

================================================================================
来源：http://stk.nanxuanxn.top

E. 字符串处理
来源：http://srn.yfazqb.com

================================================================================
来源：http://pjj.dianchejie.cn

[E01] 拼接字符串
来源：http://jot.shangyingyoupin.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bvd.cashguo.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qpe.shuidangran.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tcc.wangshuangyany.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vld.yanxiufei.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rhj.hfpthk.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gsm.gotoacloud.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sle.zhaomingkeji.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jsr.jinghuilouyu.cn

[E02] 重复字符串
来源：http://ycn.fzhhl.top

Py:   "ab" * 3
来源：http://hvn.hnqzz.top

PHP:  str_repeat("ab", 3);
来源：http://wnj.sufxvd.cn

JS:   "ab".repeat(3)
来源：http://pbx.fzhhl.top

TS:   "ab".repeat(3)
来源：http://avy.aizwys.cn

Java: "ab".repeat(3)
来源：http://clt.zhaomingkeji.xyz

Go:   strings.Repeat("ab", 3)
来源：http://dgl.mhx1999.top

Ruby: "ab" * 3
来源：http://cfi.daria6918.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ggs.jyoumei.cn

[E03] 截取子串
来源：http://hco.xuanzx.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wpc.sufxvd.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://twc.fengsongda.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kpr.cqqwz.cn

TS:   s.slice(1, 4)
来源：http://jre.shuidangran.top

Java: s.substring(1, 4)
来源：http://nbx.shanyushiyangtech.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sje.mhx1999.top

Ruby: s[1, 3];  s[1..3]
来源：http://peq.jianghu66.top

C#:   s.Substring(1, 3)
来源：http://jfn.cashguo.top

[E04] 查找子串位置
来源：http://ltc.zhoulong.xyz

Py:   s.find("x");  s.index("x")
来源：http://dko.yueranfly.top

PHP:  strpos($s, "x");
来源：http://mut.xylfe.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://oxx.jlsjyb.cn

TS:   s.indexOf("x")
来源：http://bjf.ydjk.org.cn

Java: s.indexOf("x")
来源：http://gsl.fengsongda.top

Go:   strings.Index(s, "x")
来源：http://mro.wangshuangyany.cn

Ruby: s.index("x")
来源：http://tan.sufxvd.cn

C#:   s.IndexOf("x")
来源：http://tvt.ppjwa.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://kuv.cheryme.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ark.shangyingyoupin.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ota.gotoacloud.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yrz.cqqwz.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qxa.nanxuanxn.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nee.yuanzhike.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mzi.ctjpmb.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lkz.sysykeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gne.andypj.xyz

[E06] 替换子串
来源：http://cpq.nanxinkj.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vwj.pengpengdd.cyou

PHP:  str_replace("a", "b", $s);
来源：http://mwz.shzxlz.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xth.redwolf501.top

TS:   s.replaceAll("a", "b")
来源：http://dtl.jianghu66.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qbl.jinghuilouyu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jwp.yongpay.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dut.9152youxi.cn

C#:   s.Replace("a", "b")
来源：http://fhj.fktsv.cn

[E07] 按分隔符拆分
来源：http://uju.zhijiandao.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jqv.52xcode.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jmy.redwolf501.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://jbh.nanxuanxn.top

TS:   s.split(",")
来源：http://odo.hysaishi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://lot.jinghuilouyu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mkh.fengsongda.top

Ruby: s.split(",");  s.split
来源：http://tul.cdnleiting.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lmt.redwolf501.top

[E08] 数组按分隔符合并
来源：http://ojs.316326.xyz

Py:   ",".join(items)
来源：http://tim.fzhhl.top

PHP:  implode(",", $items);
来源：http://ijf.wangshuangyany.cn

JS:   items.join(",")
来源：http://ikx.tanke756.top

TS:   items.join(",")
来源：http://pdh.hnxiangtu.top

Java: String.join(",", items)
来源：http://zbg.hammf.cn

Go:   strings.Join(items, ",")
来源：http://sdh.chenjidiqi.icu

Ruby: items.join(",")
来源：http://jhb.pengpengdd.cyou

C#:   string.Join(",", items)
来源：http://pkc.birdmap.top

[E09] 去除所有空白字符
来源：http://iyw.jlsjyb.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vbw.vehdjk.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://iyy.dashuyun.cn

JS:   s.replace(/\s+/g, "")
来源：http://aki.cdnleiting.top

TS:   s.replace(/\s+/g, "")
来源：http://veu.shanyushiyangtech.top

Java: s.replaceAll("\\s+", "")
来源：http://qdf.jinyuanbaomall.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://maa.vqdsnc.cn

Ruby: s.gsub(/\s+/, "")
来源：http://uwi.gotoacloud.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dvp.sxryk.cn

[E10] 左侧补零 / 定长填充
来源：http://hmn.ppjwa.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mvj.redwolf501.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jfh.dashuyun.cn

JS:   "7".padStart(3, "0")
来源：http://atj.guannengcc.top

TS:   "7".padStart(3, "0")
来源：http://yyl.chenzaomai.com

Java: String.format("%03d", 7)
来源：http://vvh.hnxiangtu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://scw.hcnkem.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://szc.bbcook.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mal.ppjwa.cn

[E11] 反转字符串
来源：http://wxb.zdbjq.cn

Py:   s[::-1]
来源：http://fbg.hongshengwenyu.top

PHP:  strrev($s);
来源：http://clk.gaohongyu789.top

JS:   [...s].reverse().join("")
来源：http://xyp.fengsongda.top

TS:   [...s].reverse().join("")
来源：http://fdo.haohaochexian.top

Java: new StringBuilder(s).reverse().toString()
来源：http://vlo.bbcook.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://mtc.wangshuangyany.cn

Ruby: s.reverse
来源：http://gja.guowangkeji.top

C#:   new string(s.Reverse().ToArray())
来源：http://sjt.vqdsnc.cn

[E12] 统计某字符出现次数
来源：http://rug.jinyuanbaomall.cn

Py:   s.count("a")
来源：http://pbn.yanxiufei.cn

PHP:  substr_count($s, "a");
来源：http://kjz.meibo888.top

JS:   s.split("a").length - 1
来源：http://zrk.gaohongyu789.top

TS:   s.split("a").length - 1
来源：http://wok.ybcxt.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bis.cdnleiting.top

Go:   strings.Count(s, "a")
来源：http://xmt.fehbvm.com

Ruby: s.count("a")
来源：http://pwm.jianghu66.top

C#:   s.Count(c => c == 'a')
来源：http://viy.jianghu66.top

[E13] 逐字符遍历
来源：http://anj.ppjwa.cn

Py:   for ch in s: print(ch)
来源：http://wes.sweek.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dbv.jianghu66.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://wvt.ydzc1.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://nxd.shangyingyoupin.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://etp.zycfv.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jrb.kuanghao11.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qnj.redwolf501.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gjn.havefunace.top

[E14] URL 编码与 Base64
来源：http://qgx.svipenyu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kia.yuanzhike.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://miw.hammf.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://drp.xylfe.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vsq.sjlbkw.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yqs.nanxinkj.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qql.xziqi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ihd.hywenlv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://meq.yvedp.cn

[E15] HTML 转义 / 反转义
来源：http://kgc.sxryk.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://mjk.jinqigufen.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vly.yangfankeji.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xqx.sweek.top

TS:   // 同上，务必做 XSS 过滤
来源：http://gxz.jiagoushi.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pbx.fengsongda.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xts.fktsv.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hfp.jqgfzy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gxb.fzhhl.top

[E16] 数字千分位
来源：http://jux.ctjpmb.com

Py:   f"{1234567:,}"
来源：http://jkj.xziqi.cn

PHP:  number_format(1234567);
来源：http://gxi.nwbrower.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ukm.zhixingplan.top

TS:   (1234567).toLocaleString("en-US")
来源：http://jei.guowangkeji.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cqr.ydzc1.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ivr.fehbvm.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hrf.ctjpmb.com

C#:   1234567.ToString("N0")
来源：http://vzh.ywan-chungtsiang.top

[E17] 首字母大写
来源：http://tud.pycfn.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cfm.ydjk.org.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ozw.chenlongwang.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ttc.hammf.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dhr.jinyuanbaomall.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dbi.zycfv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://oph.pengpengdd.cyou

Ruby: s.capitalize
来源：http://eni.fengsongda.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sgb.tian-w.cn

[E18] 模板占位符替换
来源：http://aqz.ydjk.org.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ijl.hnqzz.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uht.shanyushiyangkeji.top

JS:   tpl.replaceAll("{name}", name)
来源：http://myw.jinyuanbaomall.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://apz.shanyushiyangtech.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zbs.xziqi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wik.jqgufenzy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nfj.aizwys.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tmx.ppjwa.cn

[E19] 多行文本按行拆分
来源：http://mqz.daria6918.cn

Py:   s.splitlines()
来源：http://bdh.redwolf501.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hys.quarkkingdee.top

JS:   s.split(/\r?\n/)
来源：http://xhy.yvedp.cn

TS:   s.split(/\r?\n/)
来源：http://ino.fehbvm.com

Java: s.lines().toList()
来源：http://eil.sjlbkw.cn

Go:   strings.Split(s, "\n")
来源：http://cbp.chenjidiqi.icu

Ruby: s.lines
来源：http://yxs.jyoumei.cn

C#:   s.Split('\n')
来源：http://hxa.zhijiandao.cn

[E20] 判断字符串是否为空
来源：http://fro.kuanghao11.cn

Py:   if not s:
来源：http://bmh.chenzaomai.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cpi.ivvv.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gcd.wangshuangyany.cn

TS:   if (s === "") {}
来源：http://aks.fanxiaobao.xyz

Java: if (s.isEmpty()) {}
来源：http://wuk.shanyushiyangtech.top

Go:   if s == "" {}
来源：http://akx.316326.xyz

Ruby: if s.empty?
来源：http://axc.bbcook.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pvd.jqgfzy.top

[E21] 超长截断加省略号
来源：http://osl.nwbrower.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hpi.yj202588.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zxu.jlsjyb.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kaq.feifeiyinyue.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sky.hesvh.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://iah.guannengcc.top

Go:   // 按 rune 判断长度后截断
来源：http://lmz.cdnleiting.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cjv.yueranfly.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bcu.xuanzx.com

[E22] 字节长度与字符长度
来源：http://vjh.zycfv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://onm.nanxinkj.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://upg.kuanghao11.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ltk.yfazqb.com


<!-- 参考信息 -->