代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://whu.chenjidiqi.icu

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ykh.epnwcf.com

TS:   Math.max(...arr);
来源：http://mls.c1oappe.top

Java: Collections.max(list);  Collections.min(list);
来源：http://atb.quarkkingdee.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://snz.bbcook.cn

Ruby: arr.max;  arr.min
来源：http://jco.guannengcc.top

C#:   list.Max();  list.Min()
来源：http://ypk.dashuyun.cn

[D18] 扁平化嵌套数组
来源：http://gst.0kj1m.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mwp.cheryme.top

PHP:  array_merge(...$nested);
来源：http://pyr.fzhhl.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xyu.zhoulong.xyz

TS:   nested.flat();
来源：http://xsw.sysykeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://arf.gogol.net.cn

Go:   // 手写双层循环
来源：http://ino.cqqwz.cn

Ruby: nested.flatten
来源：http://dni.sjlbkw.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kvc.shangyingyoupin.top

[D19] 按字段分组
来源：http://rzs.jinqigfzy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://owi.mhx1999.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yuv.meibo888.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wnp.hysaishi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://nos.zdqjudy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xek.bjfxy.top

Go:   // 手写 map[string][]T
来源：http://vsz.pengpengdd.cyou

Ruby: arr.group_by { |x| x[:type] }
来源：http://bks.feifeiyinyue.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bdy.gotoacloud.top

[D20] 统计每个元素出现次数
来源：http://uic.fktsv.cn

Py:   Counter(arr)
来源：http://nfy.shanyushiyangkeji.top

PHP:  array_count_values($arr);
来源：http://qyv.sxryk.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mme.yj20258.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ate.haohaochexian.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://una.gzhubu.top

Go:   // 手写 map[T]int
来源：http://hmi.tarul.cn

Ruby: arr.tally
来源：http://yhm.andypj.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hlp.jiagoushi.top

[D21] 判断是否包含某元素
来源：http://ucu.nwbrower.top

Py:   x in arr
来源：http://aph.nanxinkj.top

PHP:  in_array($x, $arr, true);
来源：http://kav.xuetiantiany.cn

JS:   arr.includes(x)
来源：http://rul.yongpay.top

TS:   arr.includes(x)
来源：http://iuk.dashuyun.cn

Java: list.contains(x)
来源：http://nig.yongpay.top

Go:   slices.Contains(arr, x)
来源：http://ysj.quarkkingdee.top

Ruby: arr.include?(x)
来源：http://wna.tian-w.cn

C#:   list.Contains(x)
来源：http://tqe.ydjk.org.cn

[D22] 复制数组（避免共享引用）
来源：http://xwm.daria6918.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://loq.9152youxi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kvp.ydjk.org.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ebp.jinqigufen.top

TS:   [...arr];
来源：http://otg.yj20258888.top

Java: new ArrayList<>(list);
来源：http://qni.nanxinkj.top

Go:   copied := append([]int(nil), arr...)
来源：http://vnf.ppjwa.cn

Ruby: arr.dup;  arr.clone
来源：http://nko.shanyushiyangtech.top

C#:   new List<int>(list);
来源：http://arx.dashuyun.cn

[D23] reduce 累积计算
来源：http://qwg.hfpthk.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wdz.shanyushiyangkeji.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://weq.jinqigfzy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tky.hnqzz.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cty.yonumen.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ofv.wangshuangyany.cn

Go:   // 手写循环
来源：http://ppl.sufxvd.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lvg.hnxiangtu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wof.hywenlv.cn

[D24] 字典 / Map 基本操作
来源：http://hzs.chenlongwang.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lgg.hywenlv.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gcn.jlsjyb.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ibi.snrcjt.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://djc.tarul.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ffd.svipenyu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kyp.fzhhl.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://heg.shanyushiyangkeji.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ykw.bbcook.cn

[D25] Set 集合去重与交并差
来源：http://vhx.aibaodan.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wqj.cashguo.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qzp.andypj.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://snv.aibaodan.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zxh.sjlbkw.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://koz.hammf.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://izk.fehbvm.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ifd.ctjpmb.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fsc.chenjidiqi.icu

[D26] 数组转字符串
来源：http://lqz.c1oappe.top

Py:   ", ".join(map(str, arr))
来源：http://fvn.hesvh.cn

PHP:  implode(", ", $arr);
来源：http://oww.nwbrower.top

JS:   arr.join(", ")
来源：http://pwe.sxryk.cn

TS:   arr.join(", ")
来源：http://rlr.cdnleiting.top

Java: String.join(", ", list)
来源：http://shj.quarkkingdee.top

Go:   strings.Join(strs, ", ")
来源：http://jja.yj202588.top

Ruby: arr.join(", ")
来源：http://tws.zhijiandao.cn

C#:   string.Join(", ", list)
来源：http://xws.ydjk.org.cn

================================================================================
来源：http://nwn.hcnkem.com

E. 字符串处理
来源：http://mde.smart0.xyz

================================================================================
来源：http://lxa.daria6918.cn

[E01] 拼接字符串
来源：http://gbw.chenlongwang.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jzi.chenjidiqi.icu

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ycq.yj202588.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hqx.tarul.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gex.jianghu66.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fin.fktsv.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://phm.havefunace.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ngw.yongpay.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://oqs.yanxiufei.cn

[E02] 重复字符串
来源：http://mct.daria6918.cn

Py:   "ab" * 3
来源：http://hsr.zhiwuduotai.top

PHP:  str_repeat("ab", 3);
来源：http://lov.fengsongda.top

JS:   "ab".repeat(3)
来源：http://cdb.gotoacloud.top

TS:   "ab".repeat(3)
来源：http://lle.aibaodan.cn

Java: "ab".repeat(3)
来源：http://aji.ybcxt.top

Go:   strings.Repeat("ab", 3)
来源：http://ltg.hnqzz.top

Ruby: "ab" * 3
来源：http://pgn.chenlongwang.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vls.zhixingplan.top

[E03] 截取子串
来源：http://jco.cashguo.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jav.mhx1999.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pvy.cqqwz.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bsj.jinyuanbaomall.cn

TS:   s.slice(1, 4)
来源：http://yfh.havefunace.top

Java: s.substring(1, 4)
来源：http://jtq.ehwqpu.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://egf.gotoacloud.top

Ruby: s[1, 3];  s[1..3]
来源：http://rtm.316326.xyz

C#:   s.Substring(1, 3)
来源：http://dhi.epnwcf.com

[E04] 查找子串位置
来源：http://cbc.hcnkem.com

Py:   s.find("x");  s.index("x")
来源：http://gkw.kuanghao11.cn

PHP:  strpos($s, "x");
来源：http://pid.jyoumei.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://flo.hfpthk.cn

TS:   s.indexOf("x")
来源：http://jli.zhiwuduotai.top

Java: s.indexOf("x")
来源：http://apn.zhengqikj.top

Go:   strings.Index(s, "x")
来源：http://gwa.bbcook.cn

Ruby: s.index("x")
来源：http://czk.hywenlv.cn

C#:   s.IndexOf("x")
来源：http://nfp.smart0.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://syi.aizwys.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://isf.yj20258.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://owc.shangyingyoupin.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xrc.havefunace.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://cil.yueranfly.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vdj.zdbjq.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ozo.ppjwa.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jtu.dianchejie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bdz.ywan-chungtsiang.top

[E06] 替换子串
来源：http://kcx.iojbl.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dhw.dashuyun.cn

PHP:  str_replace("a", "b", $s);
来源：http://ipn.jinghuilouyu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://enw.fengsongda.top

TS:   s.replaceAll("a", "b")
来源：http://fep.yj202588.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zkp.birdmap.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://deh.jinghuilouyu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lgn.gotoacloud.top

C#:   s.Replace("a", "b")
来源：http://quu.jianghu66.top

[E07] 按分隔符拆分
来源：http://rqo.jinqigufen.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bsr.zhiwuduotai.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hfq.havefunace.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://pkh.bbcook.cn

TS:   s.split(",")
来源：http://vjy.aibaodan.cn

Java: s.split(",");  s.split("\\s+")
来源：http://jnh.aibaodan.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nvl.cashguo.top

Ruby: s.split(",");  s.split
来源：http://oqv.dianchejie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://npl.cashguo.top

[E08] 数组按分隔符合并
来源：http://pdg.fanxiaobao.xyz

Py:   ",".join(items)
来源：http://yqp.chenzaomai.com

PHP:  implode(",", $items);
来源：http://qgq.xingfuxueyuan.xyz

JS:   items.join(",")
来源：http://qxz.yfazqb.com

TS:   items.join(",")
来源：http://zco.pengpengdd.cyou

Java: String.join(",", items)
来源：http://hmk.jinghuilouyu.cn

Go:   strings.Join(items, ",")
来源：http://wht.jqgufenzy.top

Ruby: items.join(",")
来源：http://ajf.havefunace.top

C#:   string.Join(",", items)
来源：http://uvm.yj20258.top

[E09] 去除所有空白字符
来源：http://rat.jlsjyb.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zmi.tianlin.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://end.hongshengwenyu.top

JS:   s.replace(/\s+/g, "")
来源：http://hbq.yueranfly.top

TS:   s.replace(/\s+/g, "")
来源：http://ptb.shzxlz.cn

Java: s.replaceAll("\\s+", "")
来源：http://eoo.andypj.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://bmr.jinyuanbaomall.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kku.jinqigfzy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ocb.yonumen.top

[E10] 左侧补零 / 定长填充
来源：http://jfe.wangdashe.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://onh.cdnleiting.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://euk.wangshuangyany.cn

JS:   "7".padStart(3, "0")
来源：http://aqc.nwbrower.top

TS:   "7".padStart(3, "0")
来源：http://jwh.yj202588.top

Java: String.format("%03d", 7)
来源：http://ctw.hnqzz.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://zpj.yfazqb.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dew.xziqi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gwa.shzxlz.cn

[E11] 反转字符串
来源：http://myz.epnwcf.com

Py:   s[::-1]
来源：http://dzi.yangfankeji.com

PHP:  strrev($s);
来源：http://pap.zhaomingkeji.xyz

JS:   [...s].reverse().join("")
来源：http://aan.svipenyu.cn

TS:   [...s].reverse().join("")
来源：http://jpw.jqgufenzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://bva.zhongyouzk.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://hcx.yfazqb.com

Ruby: s.reverse
来源：http://qej.hesvh.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rut.c1oappe.top

[E12] 统计某字符出现次数
来源：http://aat.ivvv.top

Py:   s.count("a")
来源：http://jgy.chenjidiqi.icu

PHP:  substr_count($s, "a");
来源：http://ulf.jinyuanbaomall.cn

JS:   s.split("a").length - 1
来源：http://rle.zhongyouzk.top

TS:   s.split("a").length - 1
来源：http://xvv.shangyingyoupin.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wqu.gotoacloud.top

Go:   strings.Count(s, "a")
来源：http://kre.hnxiangtu.top

Ruby: s.count("a")
来源：http://ymp.jqgfzy.top

C#:   s.Count(c => c == 'a')
来源：http://xeg.daria6918.cn

[E13] 逐字符遍历
来源：http://pzb.52xcode.cn

Py:   for ch in s: print(ch)
来源：http://jlz.ydjk.org.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wum.nanxinkj.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://jqq.fanxiaobao.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://ioo.cucudq.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ipn.0kj1m.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xxh.redwolf501.top

Ruby: s.each_char { |ch| puts ch }
来源：http://gra.yj20258.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wrl.gzhubu.top

[E14] URL 编码与 Base64
来源：http://mpl.nwbrower.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bbz.hongshengwenyu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ohx.guowangkeji.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fku.aibaodan.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gkn.epnwcf.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jtr.bjfxy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://drf.cashguo.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pya.kuanghao11.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://byn.c1oappe.top

[E15] HTML 转义 / 反转义
来源：http://ace.dashuyun.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hsm.cucudq.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dzz.ivvv.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://adf.hesvh.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wik.vehdjk.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rgl.daria6918.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hfm.xinyue.icu

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ncc.sufxvd.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zkd.jinqigfzy.top

[E16] 数字千分位
来源：http://fcq.jinqigfzy.top

Py:   f"{1234567:,}"
来源：http://ppn.yanxiufei.cn

PHP:  number_format(1234567);
来源：http://aax.gotoacloud.top

JS:   (1234567).toLocaleString("en-US")
来源：http://xib.cdnleiting.top

TS:   (1234567).toLocaleString("en-US")
来源：http://gqn.chenzaomai.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gby.cucudq.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hca.zdqjudy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bac.cashguo.top

C#:   1234567.ToString("N0")
来源：http://mcg.wangdashe.top

[E17] 首字母大写
来源：http://yqd.jlsjyb.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dvu.cucudq.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://yec.hysaishi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ckq.dianchejie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mzy.yanxiufei.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dbn.zhengqikj.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ypl.jinyuanbaomall.cn

Ruby: s.capitalize
来源：http://nda.ehwqpu.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qfy.haohaochexian.top

[E18] 模板占位符替换
来源：http://ibp.yj20258.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vwr.zhoulong.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jrv.hongshengwenyu.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ese.birdmap.top

TS:   tpl.replaceAll("{name}", name)
来源：http://vhg.hnxiangtu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qbs.316326.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mvl.dianchejie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yki.vehdjk.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lms.sweek.top

[E19] 多行文本按行拆分
来源：http://ozt.wangshuangyany.cn

Py:   s.splitlines()
来源：http://zht.sysykeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nbi.guowangkeji.top

JS:   s.split(/\r?\n/)
来源：http://tob.sysykeji.top

TS:   s.split(/\r?\n/)
来源：http://fvj.cqqwz.cn

Java: s.lines().toList()
来源：http://yfl.jiagoushi.top

Go:   strings.Split(s, "\n")
来源：http://ahz.epnwcf.com

Ruby: s.lines
来源：http://emc.chenzaomai.com

C#:   s.Split('\n')
来源：http://lvw.dianchejie.cn

[E20] 判断字符串是否为空
来源：http://fqd.fengsongda.top

Py:   if not s:
来源：http://psp.bbcook.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fbd.birdmap.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lui.cdnleiting.top

TS:   if (s === "") {}
来源：http://jzh.xuetiantiany.cn

Java: if (s.isEmpty()) {}
来源：http://lwt.ctjpmb.com

Go:   if s == "" {}
来源：http://ufd.jqgfzy.top

Ruby: if s.empty?
来源：http://fwf.bbcook.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wht.jinqigfzy.top

[E21] 超长截断加省略号
来源：http://ign.pycfn.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hjt.shuidangran.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bmn.andypj.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aqp.zhengqikj.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jpl.jlsjyb.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hmu.hysaishi.cn

Go:   // 按 rune 判断长度后截断
来源：http://zir.zhixingplan.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://las.hammf.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yqa.yuxming.cn

[E22] 字节长度与字符长度
来源：http://ywy.xinyue.icu

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ubq.haohaochexian.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sje.pycfn.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xad.xuetiantiany.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yhg.havefunace.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xrv.uphjek.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://asn.tian-w.cn

Ruby: s.bytesize;  s.length
来源：http://wjg.yangfankeji.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://icc.daxiang520.top

================================================================================
来源：http://dxt.zhengqikj.top

F. 文件与目录
来源：http://gda.yuxming.cn

================================================================================
来源：http://tvl.shanyushiyangkeji.top

[F01] 读取整个文件
来源：http://wpv.zycfv.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://snb.zhoulong.xyz

PHP:  file_get_contents("a.txt");
来源：http://iuj.52xcode.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zlh.zycfv.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ygc.fengsongda.top

Java: Files.readString(Path.of("a.txt"))
来源：http://nmv.sxryk.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ndg.aibaodan.cn

Ruby: File.read("a.txt")
来源：http://knb.zhiwuduotai.top


<!-- 参考信息 -->