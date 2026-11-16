代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://nkq.yongpay.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zzi.fengsongda.top

TS:   Math.max(...arr);
来源：http://mwp.aizwys.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ggn.smart0.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://icq.jqgufenzy.top

Ruby: arr.max;  arr.min
来源：http://rfb.yuxming.cn

C#:   list.Max();  list.Min()
来源：http://hjf.daria6918.cn

[D18] 扁平化嵌套数组
来源：http://seb.jiagoushi.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blq.hongshengwenyu.top

PHP:  array_merge(...$nested);
来源：http://akx.xylfe.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yxl.sufxvd.cn

TS:   nested.flat();
来源：http://zfe.zhaomingkeji.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://igg.meibo888.top

Go:   // 手写双层循环
来源：http://csn.aibaodan.cn

Ruby: nested.flatten
来源：http://bsb.tarul.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hsa.fzhhl.top

[D19] 按字段分组
来源：http://jwi.iojbl.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://orx.nwbrower.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tlw.gogol.net.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jbj.birdmap.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://abl.c1oappe.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jin.sxryk.cn

Go:   // 手写 map[string][]T
来源：http://vcc.jqgufenzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://hjp.jinghuilouyu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mgn.meibo888.top

[D20] 统计每个元素出现次数
来源：http://tkv.bjfxy.top

Py:   Counter(arr)
来源：http://qns.yj202588.top

PHP:  array_count_values($arr);
来源：http://irc.gotoacloud.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fql.fehbvm.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qcr.xuanzx.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cem.pengpengdd.cyou

Go:   // 手写 map[T]int
来源：http://obd.0kj1m.cn

Ruby: arr.tally
来源：http://dsj.zycfv.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fpu.gaohongyu789.top

[D21] 判断是否包含某元素
来源：http://wvr.chenlongwang.top

Py:   x in arr
来源：http://xbe.jinghuilouyu.cn

PHP:  in_array($x, $arr, true);
来源：http://dug.xinyue.icu

JS:   arr.includes(x)
来源：http://jdw.zhixingplan.top

TS:   arr.includes(x)
来源：http://uai.zhijiandao.cn

Java: list.contains(x)
来源：http://mtu.hysaishi.cn

Go:   slices.Contains(arr, x)
来源：http://avu.daxiang520.top

Ruby: arr.include?(x)
来源：http://kax.cheryme.top

C#:   list.Contains(x)
来源：http://mqw.zhixingplan.top

[D22] 复制数组（避免共享引用）
来源：http://nej.gogol.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cxp.jinqigfzy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wgy.yfazqb.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cvd.dianchejie.cn

TS:   [...arr];
来源：http://jtl.redwolf501.top

Java: new ArrayList<>(list);
来源：http://cmh.yj20258888.top

Go:   copied := append([]int(nil), arr...)
来源：http://otr.chenlongwang.top

Ruby: arr.dup;  arr.clone
来源：http://nbj.zhengqikj.top

C#:   new List<int>(list);
来源：http://kma.bbcook.cn

[D23] reduce 累积计算
来源：http://ioi.ehwqpu.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hak.feifeiyinyue.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vgy.guannengcc.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wfa.zhiwuduotai.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yjw.meibo888.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://nnw.ydjk.org.cn

Go:   // 手写循环
来源：http://exl.ydzc1.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://aic.uphjek.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dst.yvedp.cn

[D24] 字典 / Map 基本操作
来源：http://cxq.ppjwa.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://iwf.nanxuanxn.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mrb.snrcjt.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nuz.zhixingplan.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rsi.cdnleiting.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hrm.ehwqpu.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zab.uphjek.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dgr.yvedp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zah.mhx1999.top

[D25] Set 集合去重与交并差
来源：http://cgz.aizwys.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xct.shuidangran.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://aob.tian-w.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nfz.yonumen.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://aih.snrcjt.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ula.wangdashe.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kqp.dianchejie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://msh.wangshuangyany.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://uac.hfpthk.cn

[D26] 数组转字符串
来源：http://mqg.svipenyu.cn

Py:   ", ".join(map(str, arr))
来源：http://nbc.sxryk.cn

PHP:  implode(", ", $arr);
来源：http://yrk.cdnleiting.top

JS:   arr.join(", ")
来源：http://rwm.smart0.xyz

TS:   arr.join(", ")
来源：http://oqm.shanyushiyangkeji.top

Java: String.join(", ", list)
来源：http://gqj.sjlbkw.cn

Go:   strings.Join(strs, ", ")
来源：http://wci.xylfe.cn

Ruby: arr.join(", ")
来源：http://hsm.sweek.top

C#:   string.Join(", ", list)
来源：http://qhs.meibo888.top

================================================================================
来源：http://sti.hammf.cn

E. 字符串处理
来源：http://vsr.zdqjudy.top

================================================================================
来源：http://jvy.tanke756.top

[E01] 拼接字符串
来源：http://zsm.shzxlz.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://adq.nanxuanxn.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ugz.bjfxy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lnv.cucudq.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lxo.vqdsnc.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://iwo.bbcook.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vbh.yangfankeji.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zrz.shangyingyoupin.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://eff.snrcjt.cn

[E02] 重复字符串
来源：http://bto.zdqjudy.top

Py:   "ab" * 3
来源：http://bmt.zdbjq.cn

PHP:  str_repeat("ab", 3);
来源：http://bhq.nanxinkj.top

JS:   "ab".repeat(3)
来源：http://fvo.c1oappe.top

TS:   "ab".repeat(3)
来源：http://igh.fehbvm.com

Java: "ab".repeat(3)
来源：http://fjd.jyoumei.cn

Go:   strings.Repeat("ab", 3)
来源：http://ejw.52xcode.cn

Ruby: "ab" * 3
来源：http://sgz.wangdashe.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dtc.ppjwa.cn

[E03] 截取子串
来源：http://fos.birdmap.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://urs.haohaochexian.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ves.snrcjt.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ywz.shangyingyoupin.top

TS:   s.slice(1, 4)
来源：http://wlc.gotoacloud.top

Java: s.substring(1, 4)
来源：http://clq.hcnkem.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nhb.ehwqpu.com

Ruby: s[1, 3];  s[1..3]
来源：http://vro.yuanzhike.top

C#:   s.Substring(1, 3)
来源：http://cgu.bjfxy.top

[E04] 查找子串位置
来源：http://jgx.316326.xyz

Py:   s.find("x");  s.index("x")
来源：http://lcc.hnxiangtu.top

PHP:  strpos($s, "x");
来源：http://srr.nanxuanxn.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zyh.cqqwz.cn

TS:   s.indexOf("x")
来源：http://kfo.ehwqpu.com

Java: s.indexOf("x")
来源：http://btk.zdbjq.cn

Go:   strings.Index(s, "x")
来源：http://cpc.smart0.xyz

Ruby: s.index("x")
来源：http://ogb.xuetiantiany.cn

C#:   s.IndexOf("x")
来源：http://bjs.tianlin.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://kbl.jiagoushi.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kds.yongpay.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dwb.gogol.net.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oxf.zhengqikj.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://aux.hnqzz.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sfe.dianchejie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qlu.ybcxt.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tog.birdmap.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://okj.hnqzz.top

[E06] 替换子串
来源：http://bxw.pycfn.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://enx.cheryme.top

PHP:  str_replace("a", "b", $s);
来源：http://aft.jlsjyb.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hgn.hcnkem.com

TS:   s.replaceAll("a", "b")
来源：http://shw.fengsongda.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dsb.nwbrower.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hph.fengsongda.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wbk.shanyushiyangtech.top

C#:   s.Replace("a", "b")
来源：http://fdm.xingfuxueyuan.xyz

[E07] 按分隔符拆分
来源：http://ugp.ydjk.org.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://uze.jqgufenzy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jfr.tian-w.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gzc.nanxuanxn.top

TS:   s.split(",")
来源：http://shz.shangyingyoupin.top

Java: s.split(",");  s.split("\\s+")
来源：http://ljp.nanxuanxn.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zhq.tanke756.top

Ruby: s.split(",");  s.split
来源：http://vmd.wangshuangyany.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gms.gaohongyu789.top

[E08] 数组按分隔符合并
来源：http://kzy.zhoulong.xyz

Py:   ",".join(items)
来源：http://oqf.ywan-chungtsiang.top

PHP:  implode(",", $items);
来源：http://pwx.cashguo.top

JS:   items.join(",")
来源：http://auh.ydzc1.top

TS:   items.join(",")
来源：http://gdv.tian-w.cn

Java: String.join(",", items)
来源：http://hfr.shanyushiyangtech.top

Go:   strings.Join(items, ",")
来源：http://gig.nwbrower.top

Ruby: items.join(",")
来源：http://qut.zdqjudy.top

C#:   string.Join(",", items)
来源：http://pxd.shzxlz.cn

[E09] 去除所有空白字符
来源：http://vjb.cashguo.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://eol.jyoumei.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://avb.vehdjk.com

JS:   s.replace(/\s+/g, "")
来源：http://rua.xingfuxueyuan.xyz

TS:   s.replace(/\s+/g, "")
来源：http://iul.shanyushiyangtech.top

Java: s.replaceAll("\\s+", "")
来源：http://czw.jqgufenzy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://mqa.ywan-chungtsiang.top

Ruby: s.gsub(/\s+/, "")
来源：http://ggz.tian-w.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ggc.pycfn.com

[E10] 左侧补零 / 定长填充
来源：http://toc.zdbjq.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hwq.cheryme.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ywq.hywenlv.cn

JS:   "7".padStart(3, "0")
来源：http://czj.zhoulong.xyz

TS:   "7".padStart(3, "0")
来源：http://vcv.yj20258.top

Java: String.format("%03d", 7)
来源：http://llt.316326.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://tbu.gotoacloud.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://isl.zhoulong.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hop.quarkkingdee.top

[E11] 反转字符串
来源：http://ncj.jianghu66.top

Py:   s[::-1]
来源：http://sss.ydjk.org.cn

PHP:  strrev($s);
来源：http://sew.guannengcc.top

JS:   [...s].reverse().join("")
来源：http://zzb.vehdjk.com

TS:   [...s].reverse().join("")
来源：http://hih.ehwqpu.com

Java: new StringBuilder(s).reverse().toString()
来源：http://qzr.havefunace.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://yax.cqqwz.cn

Ruby: s.reverse
来源：http://ovj.yuanzhike.top

C#:   new string(s.Reverse().ToArray())
来源：http://jmz.yuxming.cn

[E12] 统计某字符出现次数
来源：http://odi.nanxinkj.top

Py:   s.count("a")
来源：http://qxl.yj20258888.top

PHP:  substr_count($s, "a");
来源：http://ciy.jinyuanbaomall.cn

JS:   s.split("a").length - 1
来源：http://ijx.yj202588.top

TS:   s.split("a").length - 1
来源：http://dqw.yuxming.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lia.zhijiandao.cn

Go:   strings.Count(s, "a")
来源：http://gtn.sxryk.cn

Ruby: s.count("a")
来源：http://eoz.guannengcc.top

C#:   s.Count(c => c == 'a')
来源：http://odc.zdbjq.cn

[E13] 逐字符遍历
来源：http://alj.bbcook.cn

Py:   for ch in s: print(ch)
来源：http://bqp.jinyuanbaomall.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pdh.yangfankeji.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://fhe.sweek.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://zzd.zhiwuduotai.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://har.hysaishi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://myd.yfazqb.com

Ruby: s.each_char { |ch| puts ch }
来源：http://epz.52xcode.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://urx.yueranfly.top

[E14] URL 编码与 Base64
来源：http://jyp.jyoumei.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dpr.redwolf501.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://izt.shangyingyoupin.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wqb.bjfxy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hru.jinyuanbaomall.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jod.nwbrower.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://amf.shanyushiyangtech.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uts.meibo888.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sdy.zdqjudy.top

[E15] HTML 转义 / 反转义
来源：http://mgp.mhx1999.top

Py:   html.escape(s);  html.unescape(s)
来源：http://yhd.ydzc1.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://byy.jqgufenzy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kxs.gaohongyu789.top

TS:   // 同上，务必做 XSS 过滤
来源：http://dhc.fengsongda.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rau.tianlin.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fvo.cheryme.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jqe.yonumen.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dys.9152youxi.cn

[E16] 数字千分位
来源：http://xzk.birdmap.top

Py:   f"{1234567:,}"
来源：http://uab.cucudq.cn

PHP:  number_format(1234567);
来源：http://avi.yanxiufei.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://oml.uphjek.com

TS:   (1234567).toLocaleString("en-US")
来源：http://qco.dianchejie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qix.yj20258888.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ots.ywan-chungtsiang.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xik.xuetiantiany.cn

C#:   1234567.ToString("N0")
来源：http://vvr.ppjwa.cn

[E17] 首字母大写
来源：http://yxt.zhaomingkeji.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rce.nanxinkj.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://aey.jiagoushi.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qiw.shanyushiyangtech.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nwk.daxiang520.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vsn.yj20258888.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kae.daria6918.cn

Ruby: s.capitalize
来源：http://fts.0kj1m.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hur.jqgufenzy.top

[E18] 模板占位符替换
来源：http://hrl.sysykeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nde.guannengcc.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fnr.bjfxy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ynx.xuetiantiany.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://gjc.cashguo.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fmp.c1oappe.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nwi.bjfxy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://itu.pengpengdd.cyou

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://icq.pycfn.com

[E19] 多行文本按行拆分
来源：http://xxl.shuidangran.top

Py:   s.splitlines()
来源：http://ben.jinqigfzy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mgf.yonumen.top

JS:   s.split(/\r?\n/)
来源：http://iex.sjlbkw.cn

TS:   s.split(/\r?\n/)
来源：http://xju.daxiang520.top

Java: s.lines().toList()
来源：http://nyx.guowangkeji.top

Go:   strings.Split(s, "\n")
来源：http://qrl.zhixingplan.top

Ruby: s.lines
来源：http://yck.snrcjt.cn

C#:   s.Split('\n')
来源：http://thp.jinqigufen.top

[E20] 判断字符串是否为空
来源：http://fmo.sjlbkw.cn

Py:   if not s:
来源：http://yxd.cashguo.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lmd.iojbl.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hep.ybcxt.top

TS:   if (s === "") {}
来源：http://xxu.hcnkem.com

Java: if (s.isEmpty()) {}
来源：http://cyy.ydjk.org.cn

Go:   if s == "" {}
来源：http://vwr.jqgfzy.top

Ruby: if s.empty?
来源：http://ekh.hnqzz.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xmc.guowangkeji.top

[E21] 超长截断加省略号
来源：http://exl.wangshuangyany.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cyu.sweek.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://oki.sxryk.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gpx.cheryme.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tvk.jiagoushi.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zzx.tianlin.xyz

Go:   // 按 rune 判断长度后截断
来源：http://zdp.tarul.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://otj.yanxiufei.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rpd.hcnkem.com

[E22] 字节长度与字符长度
来源：http://nvk.316326.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ckh.yj20258888.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vaa.sjlbkw.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rvz.cashguo.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://znm.ehwqpu.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://iyp.daria6918.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://krb.nanxinkj.top

Ruby: s.bytesize;  s.length
来源：http://qps.guannengcc.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pup.ydzc1.top

================================================================================
来源：http://xds.daria6918.cn

F. 文件与目录
来源：http://eya.xuetiantiany.cn

================================================================================
来源：http://ugv.bjfxy.top

[F01] 读取整个文件
来源：http://lfx.bjfxy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://flq.ydzc1.top

PHP:  file_get_contents("a.txt");
来源：http://tcj.ydjk.org.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vod.daxiang520.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vuk.hongshengwenyu.top

Java: Files.readString(Path.of("a.txt"))
来源：http://xky.redwolf501.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vut.ppjwa.cn

Ruby: File.read("a.txt")
来源：http://bmz.jiagoushi.top


<!-- 参考信息 -->