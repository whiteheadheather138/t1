代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tck.yuxming.cn

C#:   list.Sum();  list.Average()
来源：http://buk.dianchejie.cn

[D17] 最大值与最小值
来源：http://yjo.zycfv.cn

Py:   max(arr);  min(arr)
来源：http://fuj.xuanzx.com

PHP:  max($arr);  min($arr);
来源：http://uvh.vqdsnc.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://paa.zhijiandao.cn

TS:   Math.max(...arr);
来源：http://fqp.pengpengdd.cyou

Java: Collections.max(list);  Collections.min(list);
来源：http://jta.quarkkingdee.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ssz.ydjk.org.cn

Ruby: arr.max;  arr.min
来源：http://nmo.jinqigufen.top

C#:   list.Max();  list.Min()
来源：http://wcf.zhixingplan.top

[D18] 扁平化嵌套数组
来源：http://jlw.jinqigufen.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fcc.tian-w.cn

PHP:  array_merge(...$nested);
来源：http://vru.quarkkingdee.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rzk.zhoulong.xyz

TS:   nested.flat();
来源：http://jld.ydzc1.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qsq.yonumen.top

Go:   // 手写双层循环
来源：http://dqx.uphjek.com

Ruby: nested.flatten
来源：http://gfv.ctjpmb.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://lij.quarkkingdee.top

[D19] 按字段分组
来源：http://kej.shuidangran.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kgw.zhaomingkeji.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://grs.sxryk.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nzy.sufxvd.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://obt.yj20258888.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://eve.daria6918.cn

Go:   // 手写 map[string][]T
来源：http://wmy.hfpthk.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bpa.yueranfly.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dut.jianghu66.top

[D20] 统计每个元素出现次数
来源：http://feo.c1oappe.top

Py:   Counter(arr)
来源：http://nsb.dianchejie.cn

PHP:  array_count_values($arr);
来源：http://pfy.cashguo.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mws.fengsongda.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dqo.ybcxt.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://luu.nanxinkj.top

Go:   // 手写 map[T]int
来源：http://gnl.0kj1m.cn

Ruby: arr.tally
来源：http://pqm.feifeiyinyue.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yfr.yvedp.cn

[D21] 判断是否包含某元素
来源：http://nhe.hesvh.cn

Py:   x in arr
来源：http://gaa.guowangkeji.top

PHP:  in_array($x, $arr, true);
来源：http://sbm.feifeiyinyue.top

JS:   arr.includes(x)
来源：http://ziv.jinyuanbaomall.cn

TS:   arr.includes(x)
来源：http://zfj.hcnkem.com

Java: list.contains(x)
来源：http://oku.c1oappe.top

Go:   slices.Contains(arr, x)
来源：http://llh.shanyushiyangkeji.top

Ruby: arr.include?(x)
来源：http://ekp.jianghu66.top

C#:   list.Contains(x)
来源：http://pqe.guannengcc.top

[D22] 复制数组（避免共享引用）
来源：http://vyv.birdmap.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lbb.svipenyu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://evp.yanxiufei.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xkr.haohaochexian.top

TS:   [...arr];
来源：http://fey.birdmap.top

Java: new ArrayList<>(list);
来源：http://zke.fehbvm.com

Go:   copied := append([]int(nil), arr...)
来源：http://krw.sweek.top

Ruby: arr.dup;  arr.clone
来源：http://tqb.hongshengwenyu.top

C#:   new List<int>(list);
来源：http://lpw.yuxming.cn

[D23] reduce 累积计算
来源：http://nhm.nanxuanxn.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kxv.iojbl.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://loj.aibaodan.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://osd.hfpthk.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ieb.xingfuxueyuan.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://mtp.shanyushiyangkeji.top

Go:   // 手写循环
来源：http://nem.ywan-chungtsiang.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gwv.dianchejie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nez.jyoumei.cn

[D24] 字典 / Map 基本操作
来源：http://yxy.c1oappe.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xsc.ppjwa.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kgy.tianlin.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nwd.ctjpmb.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dgp.sufxvd.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bvx.tanke756.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hfk.jqgfzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hvc.chenlongwang.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://aqf.nanxinkj.top

[D25] Set 集合去重与交并差
来源：http://uvx.0kj1m.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sxn.dianchejie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://uav.cqqwz.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tqr.tianlin.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://boz.tanke756.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vvv.bbcook.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://eyy.jqgfzy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://erx.jlsjyb.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ibo.smart0.xyz

[D26] 数组转字符串
来源：http://jmr.yangfankeji.com

Py:   ", ".join(map(str, arr))
来源：http://aya.yj20258.top

PHP:  implode(", ", $arr);
来源：http://eam.xziqi.cn

JS:   arr.join(", ")
来源：http://mbu.pycfn.com

TS:   arr.join(", ")
来源：http://bsb.zycfv.cn

Java: String.join(", ", list)
来源：http://xps.cdnleiting.top

Go:   strings.Join(strs, ", ")
来源：http://iol.daxiang520.top

Ruby: arr.join(", ")
来源：http://vfu.sjlbkw.cn

C#:   string.Join(", ", list)
来源：http://qby.xuanzx.com

================================================================================
来源：http://xnv.sysykeji.top

E. 字符串处理
来源：http://zxu.tarul.cn

================================================================================
来源：http://aci.jiagoushi.top

[E01] 拼接字符串
来源：http://vaf.hywenlv.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xid.andypj.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bmn.jinghuilouyu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nuh.hcnkem.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tqt.cdnleiting.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://efg.hongshengwenyu.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lyn.chenzaomai.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wsr.birdmap.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lpo.mhx1999.top

[E02] 重复字符串
来源：http://hjp.kuanghao11.cn

Py:   "ab" * 3
来源：http://bfo.jianghu66.top

PHP:  str_repeat("ab", 3);
来源：http://pbf.yueranfly.top

JS:   "ab".repeat(3)
来源：http://awq.hongshengwenyu.top

TS:   "ab".repeat(3)
来源：http://gdm.zhongyouzk.top

Java: "ab".repeat(3)
来源：http://mnp.sufxvd.cn

Go:   strings.Repeat("ab", 3)
来源：http://lbt.andypj.xyz

Ruby: "ab" * 3
来源：http://bvt.ywan-chungtsiang.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ase.gogol.net.cn

[E03] 截取子串
来源：http://pih.ivvv.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lig.hysaishi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://veu.shzxlz.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gpt.daria6918.cn

TS:   s.slice(1, 4)
来源：http://qxl.xziqi.cn

Java: s.substring(1, 4)
来源：http://pgs.zdbjq.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://oyd.yuxming.cn

Ruby: s[1, 3];  s[1..3]
来源：http://lme.tarul.cn

C#:   s.Substring(1, 3)
来源：http://rir.mhx1999.top

[E04] 查找子串位置
来源：http://nuo.kuanghao11.cn

Py:   s.find("x");  s.index("x")
来源：http://wqz.aizwys.cn

PHP:  strpos($s, "x");
来源：http://ofs.xinyue.icu

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mxh.shangyingyoupin.top

TS:   s.indexOf("x")
来源：http://wen.zhaomingkeji.xyz

Java: s.indexOf("x")
来源：http://mrt.hongshengwenyu.top

Go:   strings.Index(s, "x")
来源：http://oau.zycfv.cn

Ruby: s.index("x")
来源：http://aqo.tianlin.xyz

C#:   s.IndexOf("x")
来源：http://nwh.epnwcf.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://gnc.shanyushiyangtech.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zxh.fanxiaobao.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hkc.yuanzhike.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mtj.uphjek.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://qqs.zdbjq.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dcc.yj20258888.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://afi.yuxming.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pyr.jqgfzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wiv.gotoacloud.top

[E06] 替换子串
来源：http://avs.dashuyun.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tvc.snrcjt.cn

PHP:  str_replace("a", "b", $s);
来源：http://wfb.bbcook.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tct.hfpthk.cn

TS:   s.replaceAll("a", "b")
来源：http://cbt.chenjidiqi.icu

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wzp.nwbrower.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ein.yanxiufei.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pwy.zhixingplan.top

C#:   s.Replace("a", "b")
来源：http://hwb.zycfv.cn

[E07] 按分隔符拆分
来源：http://vsg.9152youxi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nfn.jqgufenzy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://exn.pycfn.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://wgs.zhengqikj.top

TS:   s.split(",")
来源：http://obw.iojbl.cn

Java: s.split(",");  s.split("\\s+")
来源：http://lol.fzhhl.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zuh.chenjidiqi.icu

Ruby: s.split(",");  s.split
来源：http://unw.zhixingplan.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cie.ehwqpu.com

[E08] 数组按分隔符合并
来源：http://myk.xingfuxueyuan.xyz

Py:   ",".join(items)
来源：http://acj.nanxinkj.top

PHP:  implode(",", $items);
来源：http://jqf.nwbrower.top

JS:   items.join(",")
来源：http://qyq.cucudq.cn

TS:   items.join(",")
来源：http://bxa.jinqigfzy.top

Java: String.join(",", items)
来源：http://zoe.yj20258888.top

Go:   strings.Join(items, ",")
来源：http://zyd.jiagoushi.top

Ruby: items.join(",")
来源：http://iee.ppjwa.cn

C#:   string.Join(",", items)
来源：http://ocv.gzhubu.top

[E09] 去除所有空白字符
来源：http://pwn.redwolf501.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://aeg.ydzc1.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hfl.shuidangran.top

JS:   s.replace(/\s+/g, "")
来源：http://gli.ivvv.top

TS:   s.replace(/\s+/g, "")
来源：http://xmt.smart0.xyz

Java: s.replaceAll("\\s+", "")
来源：http://ykw.yuxming.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://oah.fehbvm.com

Ruby: s.gsub(/\s+/, "")
来源：http://wnx.pycfn.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://muo.cqqwz.cn

[E10] 左侧补零 / 定长填充
来源：http://doe.yuanzhike.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xza.nanxinkj.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://znv.xingfuxueyuan.xyz

JS:   "7".padStart(3, "0")
来源：http://vwd.jqgfzy.top

TS:   "7".padStart(3, "0")
来源：http://hcs.zhixingplan.top

Java: String.format("%03d", 7)
来源：http://dul.nanxuanxn.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://hik.0kj1m.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ygf.zhixingplan.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://esh.cdnleiting.top

[E11] 反转字符串
来源：http://awd.nanxuanxn.top

Py:   s[::-1]
来源：http://iwk.chenjidiqi.icu

PHP:  strrev($s);
来源：http://ftd.hcnkem.com

JS:   [...s].reverse().join("")
来源：http://ecm.yuxming.cn

TS:   [...s].reverse().join("")
来源：http://mtr.jianghu66.top

Java: new StringBuilder(s).reverse().toString()
来源：http://pvr.pengpengdd.cyou

Go:   // 转 []rune 后倒序再转回 string
来源：http://zhl.ywan-chungtsiang.top

Ruby: s.reverse
来源：http://qya.ybcxt.top

C#:   new string(s.Reverse().ToArray())
来源：http://yaf.daria6918.cn

[E12] 统计某字符出现次数
来源：http://uuv.wangdashe.top

Py:   s.count("a")
来源：http://wmr.yangfankeji.com

PHP:  substr_count($s, "a");
来源：http://urb.ehwqpu.com

JS:   s.split("a").length - 1
来源：http://gct.xylfe.cn

TS:   s.split("a").length - 1
来源：http://ubk.zhoulong.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mcw.316326.xyz

Go:   strings.Count(s, "a")
来源：http://khq.xziqi.cn

Ruby: s.count("a")
来源：http://qmq.yangfankeji.com

C#:   s.Count(c => c == 'a')
来源：http://ioa.wangshuangyany.cn

[E13] 逐字符遍历
来源：http://cfc.kuanghao11.cn

Py:   for ch in s: print(ch)
来源：http://rbh.yuanzhike.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tyy.52xcode.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xvt.sweek.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://oif.shanyushiyangkeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hod.shangyingyoupin.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vam.shangyingyoupin.top

Ruby: s.each_char { |ch| puts ch }
来源：http://eci.nwbrower.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vlm.tian-w.cn

[E14] URL 编码与 Base64
来源：http://zxt.fzhhl.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fjd.tianlin.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://ezh.wangshuangyany.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://utw.cashguo.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ffy.yanxiufei.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hmt.vehdjk.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://eul.mhx1999.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xmc.zycfv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rsb.fengsongda.top

[E15] HTML 转义 / 反转义
来源：http://pvs.hysaishi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fkc.cdnleiting.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pep.ywan-chungtsiang.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gyu.fanxiaobao.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://ask.jqgfzy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://puw.gogol.net.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kuh.mhx1999.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bwc.fengsongda.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://btt.xuetiantiany.cn

[E16] 数字千分位
来源：http://dps.svipenyu.cn

Py:   f"{1234567:,}"
来源：http://gon.andypj.xyz

PHP:  number_format(1234567);
来源：http://qri.jianghu66.top

JS:   (1234567).toLocaleString("en-US")
来源：http://pwe.mhx1999.top

TS:   (1234567).toLocaleString("en-US")
来源：http://cfx.ywan-chungtsiang.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wjb.epnwcf.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cms.meibo888.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://riu.sufxvd.cn

C#:   1234567.ToString("N0")
来源：http://xkb.haohaochexian.top

[E17] 首字母大写
来源：http://fbh.redwolf501.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tia.fzhhl.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://tfi.ybcxt.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qlj.316326.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kew.bjfxy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://iob.yfazqb.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://oou.shuidangran.top

Ruby: s.capitalize
来源：http://vdv.jianghu66.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://uax.ppjwa.cn

[E18] 模板占位符替换
来源：http://hrg.kuanghao11.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://chw.sxryk.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jik.zhiwuduotai.top

JS:   tpl.replaceAll("{name}", name)
来源：http://pou.zdbjq.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qtq.zhoulong.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ilk.guowangkeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hcy.daria6918.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ukx.smart0.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://eep.cucudq.cn

[E19] 多行文本按行拆分
来源：http://kly.zhaomingkeji.xyz

Py:   s.splitlines()
来源：http://cfj.hysaishi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://arc.xinyue.icu

JS:   s.split(/\r?\n/)
来源：http://gus.xziqi.cn

TS:   s.split(/\r?\n/)
来源：http://onu.shanyushiyangkeji.top

Java: s.lines().toList()
来源：http://uuq.uphjek.com

Go:   strings.Split(s, "\n")
来源：http://dql.jinqigfzy.top

Ruby: s.lines
来源：http://uak.cucudq.cn

C#:   s.Split('\n')
来源：http://pyy.sysykeji.top

[E20] 判断字符串是否为空
来源：http://bef.gzhubu.top

Py:   if not s:
来源：http://kom.hammf.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lqa.chenzaomai.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lqj.iojbl.cn

TS:   if (s === "") {}
来源：http://gjf.ydjk.org.cn

Java: if (s.isEmpty()) {}
来源：http://qpe.shuidangran.top

Go:   if s == "" {}
来源：http://nzn.jyoumei.cn

Ruby: if s.empty?
来源：http://iew.yvedp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bnc.aibaodan.cn

[E21] 超长截断加省略号
来源：http://gnk.birdmap.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://igy.guowangkeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xgh.zhengqikj.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zkr.wangdashe.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zda.zdbjq.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bkt.jinqigufen.top

Go:   // 按 rune 判断长度后截断
来源：http://zkn.xuetiantiany.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lyi.chenjidiqi.icu

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ycx.havefunace.top

[E22] 字节长度与字符长度
来源：http://lwp.zhiwuduotai.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://scu.bjfxy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wsb.sysykeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lod.zhongyouzk.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ahz.fzhhl.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jkc.sxryk.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ktw.fengsongda.top

Ruby: s.bytesize;  s.length
来源：http://xzi.cheryme.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kvu.shuidangran.top

================================================================================
来源：http://rwt.yj202588.top

F. 文件与目录
来源：http://wbb.ctjpmb.com

================================================================================
来源：http://mhy.shuidangran.top

[F01] 读取整个文件
来源：http://ouf.chenlongwang.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nzb.yonumen.top

PHP:  file_get_contents("a.txt");
来源：http://kht.sxryk.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://txk.ydjk.org.cn


<!-- 参考信息 -->