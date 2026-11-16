代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ppn.zhaomingkeji.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://avr.vqdsnc.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://soi.jiagoushi.top

Go:   // 手写循环累加
来源：http://qgr.shzxlz.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lxh.bbcook.cn

C#:   list.Sum();  list.Average()
来源：http://ein.jinyuanbaomall.cn

[D17] 最大值与最小值
来源：http://tau.gogol.net.cn

Py:   max(arr);  min(arr)
来源：http://bdw.guannengcc.top

PHP:  max($arr);  min($arr);
来源：http://qdr.zdbjq.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://prx.tanke756.top

TS:   Math.max(...arr);
来源：http://bxi.jlsjyb.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://baa.cucudq.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rnn.sysykeji.top

Ruby: arr.max;  arr.min
来源：http://vqc.jqgfzy.top

C#:   list.Max();  list.Min()
来源：http://rkp.feifeiyinyue.top

[D18] 扁平化嵌套数组
来源：http://zul.ctjpmb.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://asx.chenlongwang.top

PHP:  array_merge(...$nested);
来源：http://wnm.hnxiangtu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dlp.ppjwa.cn

TS:   nested.flat();
来源：http://hcv.ctjpmb.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gmf.cheryme.top

Go:   // 手写双层循环
来源：http://ngf.zdbjq.cn

Ruby: nested.flatten
来源：http://rgm.aibaodan.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tzo.hesvh.cn

[D19] 按字段分组
来源：http://moi.zhoulong.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://psw.xuanzx.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ffu.aizwys.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cxw.fzhhl.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://zdj.hywenlv.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oum.gogol.net.cn

Go:   // 手写 map[string][]T
来源：http://kwl.fktsv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://hno.yuxming.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hph.52xcode.cn

[D20] 统计每个元素出现次数
来源：http://liu.zycfv.cn

Py:   Counter(arr)
来源：http://lhv.vehdjk.com

PHP:  array_count_values($arr);
来源：http://qvn.ctjpmb.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bgg.hcnkem.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dzz.tarul.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ool.sysykeji.top

Go:   // 手写 map[T]int
来源：http://pop.haohaochexian.top

Ruby: arr.tally
来源：http://utj.yj20258.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fuk.sysykeji.top

[D21] 判断是否包含某元素
来源：http://woi.fzhhl.top

Py:   x in arr
来源：http://xbx.jyoumei.cn

PHP:  in_array($x, $arr, true);
来源：http://mzz.xziqi.cn

JS:   arr.includes(x)
来源：http://cbt.mhx1999.top

TS:   arr.includes(x)
来源：http://qdl.gogol.net.cn

Java: list.contains(x)
来源：http://ubz.zhixingplan.top

Go:   slices.Contains(arr, x)
来源：http://zfb.nanxinkj.top

Ruby: arr.include?(x)
来源：http://yce.hammf.cn

C#:   list.Contains(x)
来源：http://hbw.hfpthk.cn

[D22] 复制数组（避免共享引用）
来源：http://oov.aibaodan.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://atz.aizwys.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dkn.hesvh.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fkw.redwolf501.top

TS:   [...arr];
来源：http://gsv.bbcook.cn

Java: new ArrayList<>(list);
来源：http://ozt.zhijiandao.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qeg.chenlongwang.top

Ruby: arr.dup;  arr.clone
来源：http://awx.kuanghao11.cn

C#:   new List<int>(list);
来源：http://ile.wangdashe.top

[D23] reduce 累积计算
来源：http://xdc.zhiwuduotai.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gwl.zycfv.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zio.zycfv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kdd.quarkkingdee.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iio.ydzc1.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://wnn.zhoulong.xyz

Go:   // 手写循环
来源：http://mrp.daxiang520.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tfu.sysykeji.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vml.fktsv.cn

[D24] 字典 / Map 基本操作
来源：http://tvm.bjfxy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ewn.jqgufenzy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pks.yfazqb.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hqw.sxryk.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pco.zhiwuduotai.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://esq.nanxinkj.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lag.nwbrower.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yys.guannengcc.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pas.nanxuanxn.top

[D25] Set 集合去重与交并差
来源：http://cae.nanxinkj.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vjt.zhengqikj.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mvj.jinqigufen.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qxo.sxryk.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qyk.tarul.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mwr.ydjk.org.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wzo.fengsongda.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mwu.quarkkingdee.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rtx.gogol.net.cn

[D26] 数组转字符串
来源：http://wio.gotoacloud.top

Py:   ", ".join(map(str, arr))
来源：http://dun.chenjidiqi.icu

PHP:  implode(", ", $arr);
来源：http://blc.ehwqpu.com

JS:   arr.join(", ")
来源：http://gfk.smart0.xyz

TS:   arr.join(", ")
来源：http://oac.ydzc1.top

Java: String.join(", ", list)
来源：http://sxd.jinghuilouyu.cn

Go:   strings.Join(strs, ", ")
来源：http://bkf.epnwcf.com

Ruby: arr.join(", ")
来源：http://lyp.sufxvd.cn

C#:   string.Join(", ", list)
来源：http://vuo.sjlbkw.cn

================================================================================
来源：http://npo.316326.xyz

E. 字符串处理
来源：http://zwo.gaohongyu789.top

================================================================================
来源：http://nqv.xingfuxueyuan.xyz

[E01] 拼接字符串
来源：http://utt.cheryme.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mba.xuanzx.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gjb.ppjwa.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wch.jinqigufen.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bcl.nwbrower.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vsn.iojbl.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yjd.yueranfly.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gji.c1oappe.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nas.zhengqikj.top

[E02] 重复字符串
来源：http://wqs.fanxiaobao.xyz

Py:   "ab" * 3
来源：http://hql.zhiwuduotai.top

PHP:  str_repeat("ab", 3);
来源：http://jon.c1oappe.top

JS:   "ab".repeat(3)
来源：http://aht.sxryk.cn

TS:   "ab".repeat(3)
来源：http://cvw.svipenyu.cn

Java: "ab".repeat(3)
来源：http://ohj.redwolf501.top

Go:   strings.Repeat("ab", 3)
来源：http://auu.daxiang520.top

Ruby: "ab" * 3
来源：http://wct.vehdjk.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uwt.jinqigfzy.top

[E03] 截取子串
来源：http://ycc.dashuyun.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vjd.shuidangran.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pnk.zhengqikj.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://orj.chenzaomai.com

TS:   s.slice(1, 4)
来源：http://aiw.jqgufenzy.top

Java: s.substring(1, 4)
来源：http://zks.52xcode.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cim.sweek.top

Ruby: s[1, 3];  s[1..3]
来源：http://mwu.shzxlz.cn

C#:   s.Substring(1, 3)
来源：http://qwg.fanxiaobao.xyz

[E04] 查找子串位置
来源：http://ypj.bbcook.cn

Py:   s.find("x");  s.index("x")
来源：http://wqe.xziqi.cn

PHP:  strpos($s, "x");
来源：http://fza.sweek.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kza.shanyushiyangkeji.top

TS:   s.indexOf("x")
来源：http://jmj.nanxinkj.top

Java: s.indexOf("x")
来源：http://pmn.yonumen.top

Go:   strings.Index(s, "x")
来源：http://xiy.gaohongyu789.top

Ruby: s.index("x")
来源：http://xpm.aizwys.cn

C#:   s.IndexOf("x")
来源：http://pmt.ydzc1.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://xxa.zhongyouzk.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wym.cucudq.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jhw.cqqwz.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wov.xuanzx.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://xry.zycfv.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cmy.haohaochexian.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uwx.xuetiantiany.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ltp.tian-w.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bia.yuxming.cn

[E06] 替换子串
来源：http://bol.shanyushiyangtech.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://iqk.gogol.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://xem.hammf.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://svj.ydzc1.top

TS:   s.replaceAll("a", "b")
来源：http://xrq.cucudq.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ktv.jinqigfzy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lqd.yanxiufei.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zua.aibaodan.cn

C#:   s.Replace("a", "b")
来源：http://cgr.fzhhl.top

[E07] 按分隔符拆分
来源：http://hmq.jianghu66.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pxs.sxryk.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://spc.zhoulong.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://muc.tian-w.cn

TS:   s.split(",")
来源：http://nls.jqgfzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://uqs.xuetiantiany.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wib.yangfankeji.com

Ruby: s.split(",");  s.split
来源：http://eeg.gotoacloud.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tmv.nanxinkj.top

[E08] 数组按分隔符合并
来源：http://ash.tarul.cn

Py:   ",".join(items)
来源：http://qeb.zhongyouzk.top

PHP:  implode(",", $items);
来源：http://yww.cashguo.top

JS:   items.join(",")
来源：http://nrw.yuxming.cn

TS:   items.join(",")
来源：http://wdz.sxryk.cn

Java: String.join(",", items)
来源：http://wkq.hfpthk.cn

Go:   strings.Join(items, ",")
来源：http://vwg.ctjpmb.com

Ruby: items.join(",")
来源：http://tpa.dashuyun.cn

C#:   string.Join(",", items)
来源：http://eso.yanxiufei.cn

[E09] 去除所有空白字符
来源：http://lyd.tanke756.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rni.hnxiangtu.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dfk.yuanzhike.top

JS:   s.replace(/\s+/g, "")
来源：http://idr.ybcxt.top

TS:   s.replace(/\s+/g, "")
来源：http://gmk.snrcjt.cn

Java: s.replaceAll("\\s+", "")
来源：http://den.zdqjudy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://pyn.zhongyouzk.top

Ruby: s.gsub(/\s+/, "")
来源：http://cjt.svipenyu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ecc.shzxlz.cn

[E10] 左侧补零 / 定长填充
来源：http://cvf.zhiwuduotai.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cii.ivvv.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zme.yuxming.cn

JS:   "7".padStart(3, "0")
来源：http://vhn.shanyushiyangkeji.top

TS:   "7".padStart(3, "0")
来源：http://ehz.jyoumei.cn

Java: String.format("%03d", 7)
来源：http://ahn.havefunace.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ajy.tianlin.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jwo.xuetiantiany.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fgn.jinyuanbaomall.cn

[E11] 反转字符串
来源：http://otz.yuanzhike.top

Py:   s[::-1]
来源：http://zcf.andypj.xyz

PHP:  strrev($s);
来源：http://gtz.tianlin.xyz

JS:   [...s].reverse().join("")
来源：http://ewv.yvedp.cn

TS:   [...s].reverse().join("")
来源：http://ygm.ehwqpu.com

Java: new StringBuilder(s).reverse().toString()
来源：http://hxz.haohaochexian.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://yon.yfazqb.com

Ruby: s.reverse
来源：http://aip.zhongyouzk.top

C#:   new string(s.Reverse().ToArray())
来源：http://ltv.cqqwz.cn

[E12] 统计某字符出现次数
来源：http://mus.ivvv.top

Py:   s.count("a")
来源：http://zqj.havefunace.top

PHP:  substr_count($s, "a");
来源：http://ynk.jiagoushi.top

JS:   s.split("a").length - 1
来源：http://tbu.ctjpmb.com

TS:   s.split("a").length - 1
来源：http://gbv.gogol.net.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://aox.xylfe.cn

Go:   strings.Count(s, "a")
来源：http://pet.zhijiandao.cn

Ruby: s.count("a")
来源：http://wfz.hnxiangtu.top

C#:   s.Count(c => c == 'a')
来源：http://vyo.gogol.net.cn

[E13] 逐字符遍历
来源：http://rhg.gzhubu.top

Py:   for ch in s: print(ch)
来源：http://ygn.yfazqb.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zha.iojbl.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gdi.yuxming.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qnv.gaohongyu789.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ier.guannengcc.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uie.chenjidiqi.icu

Ruby: s.each_char { |ch| puts ch }
来源：http://ypz.sjlbkw.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bqm.jianghu66.top

[E14] URL 编码与 Base64
来源：http://qsu.sjlbkw.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nzu.uphjek.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://jdp.hysaishi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zem.guannengcc.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xeh.zhongyouzk.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yrv.zdbjq.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tnp.dashuyun.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fpv.zhijiandao.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lbs.cqqwz.cn

[E15] HTML 转义 / 反转义
来源：http://pej.gotoacloud.top

Py:   html.escape(s);  html.unescape(s)
来源：http://aqp.redwolf501.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hno.chenlongwang.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vop.shanyushiyangtech.top

TS:   // 同上，务必做 XSS 过滤
来源：http://gzu.fengsongda.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vcl.cashguo.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yte.yueranfly.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wjn.xingfuxueyuan.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rmm.52xcode.cn

[E16] 数字千分位
来源：http://nqh.yuanzhike.top

Py:   f"{1234567:,}"
来源：http://efk.redwolf501.top

PHP:  number_format(1234567);
来源：http://riv.chenlongwang.top

JS:   (1234567).toLocaleString("en-US")
来源：http://oah.hysaishi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xms.jiagoushi.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zwt.snrcjt.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bol.shzxlz.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nvc.316326.xyz

C#:   1234567.ToString("N0")
来源：http://bnl.xziqi.cn

[E17] 首字母大写
来源：http://xhy.shanyushiyangtech.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://aei.quarkkingdee.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://umn.ehwqpu.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rdu.jyoumei.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bhk.zhengqikj.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pys.hywenlv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dex.zhongyouzk.top

Ruby: s.capitalize
来源：http://apz.jyoumei.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nxb.ivvv.top

[E18] 模板占位符替换
来源：http://rel.vqdsnc.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gnl.wangdashe.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ywp.cdnleiting.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ipr.hcnkem.com

TS:   tpl.replaceAll("{name}", name)
来源：http://dlp.hnxiangtu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nhq.jinqigfzy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kac.cqqwz.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cnf.hcnkem.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ihi.c1oappe.top

[E19] 多行文本按行拆分
来源：http://dwy.yongpay.top

Py:   s.splitlines()
来源：http://jbg.jinghuilouyu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xin.hammf.cn

JS:   s.split(/\r?\n/)
来源：http://mou.shanyushiyangkeji.top

TS:   s.split(/\r?\n/)
来源：http://vpa.ehwqpu.com

Java: s.lines().toList()
来源：http://skr.cqqwz.cn

Go:   strings.Split(s, "\n")
来源：http://ljv.yj20258888.top

Ruby: s.lines
来源：http://obp.yfazqb.com

C#:   s.Split('\n')
来源：http://twi.cashguo.top

[E20] 判断字符串是否为空
来源：http://exx.ctjpmb.com

Py:   if not s:
来源：http://ehf.jianghu66.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fnn.tanke756.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zsi.tian-w.cn

TS:   if (s === "") {}
来源：http://uff.hongshengwenyu.top

Java: if (s.isEmpty()) {}
来源：http://lvo.xuetiantiany.cn

Go:   if s == "" {}
来源：http://jcy.quarkkingdee.top

Ruby: if s.empty?
来源：http://meb.quarkkingdee.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ggj.shuidangran.top

[E21] 超长截断加省略号
来源：http://zgu.hnxiangtu.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tag.ctjpmb.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wwo.cashguo.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vof.yonumen.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zwj.feifeiyinyue.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://orr.yonumen.top

Go:   // 按 rune 判断长度后截断
来源：http://jtf.dianchejie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jqa.cashguo.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://isn.wangdashe.top

[E22] 字节长度与字符长度
来源：http://odr.52xcode.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hpu.tianlin.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fsl.gogol.net.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dqe.zhengqikj.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zdh.nwbrower.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rud.cdnleiting.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://llf.tianlin.xyz

Ruby: s.bytesize;  s.length
来源：http://lmj.sweek.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vcg.hywenlv.cn

================================================================================
来源：http://uwt.xylfe.cn

F. 文件与目录
来源：http://tav.fanxiaobao.xyz

================================================================================
来源：http://nkm.hongshengwenyu.top


<!-- 参考信息 -->