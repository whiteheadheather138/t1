代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gms.sysykeji.top

PHP:  array_merge(...$nested);
来源：http://xvd.xylfe.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kra.fehbvm.com

TS:   nested.flat();
来源：http://jng.fzhhl.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://enl.gogol.net.cn

Go:   // 手写双层循环
来源：http://blf.dianchejie.cn

Ruby: nested.flatten
来源：http://piz.andypj.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://yem.chenjidiqi.icu

[D19] 按字段分组
来源：http://grb.fehbvm.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://iyz.cucudq.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vcj.aibaodan.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lij.hysaishi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ooy.wangdashe.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ocp.zhengqikj.top

Go:   // 手写 map[string][]T
来源：http://ydq.yuxming.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wka.ctjpmb.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vpj.ybcxt.top

[D20] 统计每个元素出现次数
来源：http://rek.jinghuilouyu.cn

Py:   Counter(arr)
来源：http://utq.jqgufenzy.top

PHP:  array_count_values($arr);
来源：http://wnp.havefunace.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://plz.epnwcf.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tzh.fzhhl.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ugc.shuidangran.top

Go:   // 手写 map[T]int
来源：http://sxg.zdbjq.cn

Ruby: arr.tally
来源：http://nuj.hfpthk.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://edb.yvedp.cn

[D21] 判断是否包含某元素
来源：http://bli.52xcode.cn

Py:   x in arr
来源：http://qjm.xinyue.icu

PHP:  in_array($x, $arr, true);
来源：http://ked.chenlongwang.top

JS:   arr.includes(x)
来源：http://ogw.zdqjudy.top

TS:   arr.includes(x)
来源：http://jft.ydjk.org.cn

Java: list.contains(x)
来源：http://snn.yvedp.cn

Go:   slices.Contains(arr, x)
来源：http://dcb.bbcook.cn

Ruby: arr.include?(x)
来源：http://gzn.316326.xyz

C#:   list.Contains(x)
来源：http://txp.c1oappe.top

[D22] 复制数组（避免共享引用）
来源：http://mqz.sweek.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ivd.yongpay.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uxr.ybcxt.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jpw.hnxiangtu.top

TS:   [...arr];
来源：http://iao.yj202588.top

Java: new ArrayList<>(list);
来源：http://wtt.guowangkeji.top

Go:   copied := append([]int(nil), arr...)
来源：http://bli.jqgfzy.top

Ruby: arr.dup;  arr.clone
来源：http://qwf.ehwqpu.com

C#:   new List<int>(list);
来源：http://ffm.hywenlv.cn

[D23] reduce 累积计算
来源：http://ugq.aizwys.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jnm.fehbvm.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nxv.shuidangran.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://idq.yueranfly.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zyl.hnqzz.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://qdv.zhixingplan.top

Go:   // 手写循环
来源：http://pby.9152youxi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jov.fehbvm.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jmi.xuetiantiany.cn

[D24] 字典 / Map 基本操作
来源：http://nfk.hnqzz.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://awy.sjlbkw.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yyr.316326.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kpv.havefunace.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mov.hfpthk.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tif.dashuyun.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jpm.chenzaomai.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rio.jiagoushi.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mco.pengpengdd.cyou

[D25] Set 集合去重与交并差
来源：http://akd.wangshuangyany.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wyk.dianchejie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cxl.yuxming.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xkk.yanxiufei.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pfp.gzhubu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://erb.yvedp.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://uni.52xcode.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xpt.yuxming.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xsp.xuetiantiany.cn

[D26] 数组转字符串
来源：http://jxf.dashuyun.cn

Py:   ", ".join(map(str, arr))
来源：http://pzi.hnxiangtu.top

PHP:  implode(", ", $arr);
来源：http://kpm.shanyushiyangtech.top

JS:   arr.join(", ")
来源：http://yuk.yuanzhike.top

TS:   arr.join(", ")
来源：http://jmt.zycfv.cn

Java: String.join(", ", list)
来源：http://ivn.shzxlz.cn

Go:   strings.Join(strs, ", ")
来源：http://sup.sufxvd.cn

Ruby: arr.join(", ")
来源：http://sfe.fzhhl.top

C#:   string.Join(", ", list)
来源：http://xez.zhengqikj.top

================================================================================
来源：http://zyb.zycfv.cn

E. 字符串处理
来源：http://fyp.guowangkeji.top

================================================================================
来源：http://ril.zycfv.cn

[E01] 拼接字符串
来源：http://yld.jinyuanbaomall.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gpf.zhixingplan.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zce.xuetiantiany.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mun.shuidangran.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://npz.jlsjyb.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xgb.52xcode.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vpz.zhongyouzk.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jbs.9152youxi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fuf.9152youxi.cn

[E02] 重复字符串
来源：http://vdd.yanxiufei.cn

Py:   "ab" * 3
来源：http://irb.cucudq.cn

PHP:  str_repeat("ab", 3);
来源：http://ynt.kuanghao11.cn

JS:   "ab".repeat(3)
来源：http://yau.sysykeji.top

TS:   "ab".repeat(3)
来源：http://cic.316326.xyz

Java: "ab".repeat(3)
来源：http://ugw.shangyingyoupin.top

Go:   strings.Repeat("ab", 3)
来源：http://zva.xuetiantiany.cn

Ruby: "ab" * 3
来源：http://wtl.smart0.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hqw.tian-w.cn

[E03] 截取子串
来源：http://sru.hywenlv.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xux.hcnkem.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dgr.sufxvd.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ysi.gotoacloud.top

TS:   s.slice(1, 4)
来源：http://nbb.xuetiantiany.cn

Java: s.substring(1, 4)
来源：http://vlf.chenjidiqi.icu

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://eip.zdqjudy.top

Ruby: s[1, 3];  s[1..3]
来源：http://tnh.jiagoushi.top

C#:   s.Substring(1, 3)
来源：http://qla.fehbvm.com

[E04] 查找子串位置
来源：http://ekk.kuanghao11.cn

Py:   s.find("x");  s.index("x")
来源：http://yrv.jiagoushi.top

PHP:  strpos($s, "x");
来源：http://awf.tarul.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ium.jinghuilouyu.cn

TS:   s.indexOf("x")
来源：http://uzi.gzhubu.top

Java: s.indexOf("x")
来源：http://icp.fanxiaobao.xyz

Go:   strings.Index(s, "x")
来源：http://mir.sjlbkw.cn

Ruby: s.index("x")
来源：http://cjs.redwolf501.top

C#:   s.IndexOf("x")
来源：http://uwa.guannengcc.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://bkd.gzhubu.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sfp.jinqigfzy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mqi.sweek.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tdp.nanxinkj.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://vpl.gaohongyu789.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pgs.hesvh.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zaf.ivvv.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sib.sxryk.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wmk.yuxming.cn

[E06] 替换子串
来源：http://yhs.andypj.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hfw.fzhhl.top

PHP:  str_replace("a", "b", $s);
来源：http://wpa.sweek.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nxd.zhijiandao.cn

TS:   s.replaceAll("a", "b")
来源：http://yda.smart0.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rvl.cashguo.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ill.ydzc1.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://grj.zhongyouzk.top

C#:   s.Replace("a", "b")
来源：http://ffi.haohaochexian.top

[E07] 按分隔符拆分
来源：http://xmw.ppjwa.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lxq.yuanzhike.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pbq.feifeiyinyue.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://apx.chenlongwang.top

TS:   s.split(",")
来源：http://wac.zdqjudy.top

Java: s.split(",");  s.split("\\s+")
来源：http://vof.xylfe.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://aat.nanxinkj.top

Ruby: s.split(",");  s.split
来源：http://jsk.smart0.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fft.snrcjt.cn

[E08] 数组按分隔符合并
来源：http://wbf.birdmap.top

Py:   ",".join(items)
来源：http://fzo.svipenyu.cn

PHP:  implode(",", $items);
来源：http://uej.redwolf501.top

JS:   items.join(",")
来源：http://ftb.jinyuanbaomall.cn

TS:   items.join(",")
来源：http://ggs.ydzc1.top

Java: String.join(",", items)
来源：http://azf.jinqigfzy.top

Go:   strings.Join(items, ",")
来源：http://ohv.feifeiyinyue.top

Ruby: items.join(",")
来源：http://uti.zdqjudy.top

C#:   string.Join(",", items)
来源：http://ecb.ydjk.org.cn

[E09] 去除所有空白字符
来源：http://wrk.xingfuxueyuan.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kvt.hnxiangtu.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fkc.fehbvm.com

JS:   s.replace(/\s+/g, "")
来源：http://voj.sufxvd.cn

TS:   s.replace(/\s+/g, "")
来源：http://oiv.yfazqb.com

Java: s.replaceAll("\\s+", "")
来源：http://nla.zhongyouzk.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://sct.jinqigufen.top

Ruby: s.gsub(/\s+/, "")
来源：http://qbj.hongshengwenyu.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bie.bbcook.cn

[E10] 左侧补零 / 定长填充
来源：http://xdf.guowangkeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jym.aizwys.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mtw.xingfuxueyuan.xyz

JS:   "7".padStart(3, "0")
来源：http://lgd.hammf.cn

TS:   "7".padStart(3, "0")
来源：http://pri.hysaishi.cn

Java: String.format("%03d", 7)
来源：http://gex.zdqjudy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ihr.aibaodan.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dqi.shzxlz.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://loy.cashguo.top

[E11] 反转字符串
来源：http://rpt.jqgfzy.top

Py:   s[::-1]
来源：http://wju.fengsongda.top

PHP:  strrev($s);
来源：http://agn.cashguo.top

JS:   [...s].reverse().join("")
来源：http://dxn.hongshengwenyu.top

TS:   [...s].reverse().join("")
来源：http://slf.yanxiufei.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pvx.chenjidiqi.icu

Go:   // 转 []rune 后倒序再转回 string
来源：http://mex.dashuyun.cn

Ruby: s.reverse
来源：http://ojc.0kj1m.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rkp.snrcjt.cn

[E12] 统计某字符出现次数
来源：http://akn.vqdsnc.cn

Py:   s.count("a")
来源：http://vvu.c1oappe.top

PHP:  substr_count($s, "a");
来源：http://zyz.quarkkingdee.top

JS:   s.split("a").length - 1
来源：http://ioe.gzhubu.top

TS:   s.split("a").length - 1
来源：http://pxg.vehdjk.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rry.ivvv.top

Go:   strings.Count(s, "a")
来源：http://wak.nwbrower.top

Ruby: s.count("a")
来源：http://npz.yuxming.cn

C#:   s.Count(c => c == 'a')
来源：http://zxj.birdmap.top

[E13] 逐字符遍历
来源：http://agh.uphjek.com

Py:   for ch in s: print(ch)
来源：http://rng.cdnleiting.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://aaf.zhixingplan.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://khr.vqdsnc.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wsr.shangyingyoupin.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jyb.quarkkingdee.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hvo.xingfuxueyuan.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://tpf.xylfe.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hwd.aibaodan.cn

[E14] URL 编码与 Base64
来源：http://bkm.snrcjt.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uvf.yfazqb.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://jkw.cashguo.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mgd.guowangkeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://urm.vqdsnc.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xas.tarul.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qve.hammf.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://urb.shanyushiyangkeji.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hop.xziqi.cn

[E15] HTML 转义 / 反转义
来源：http://bpm.xuetiantiany.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xtl.nanxuanxn.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://adi.gzhubu.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://egk.havefunace.top

TS:   // 同上，务必做 XSS 过滤
来源：http://gmb.52xcode.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://oqt.zhongyouzk.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yki.sufxvd.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bin.tanke756.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ubj.chenjidiqi.icu

[E16] 数字千分位
来源：http://nrk.hesvh.cn

Py:   f"{1234567:,}"
来源：http://agb.cheryme.top

PHP:  number_format(1234567);
来源：http://qxh.shzxlz.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://kwa.hywenlv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://kwr.daxiang520.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://agd.jinyuanbaomall.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bpy.wangdashe.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://avb.hcnkem.com

C#:   1234567.ToString("N0")
来源：http://fbu.sufxvd.cn

[E17] 首字母大写
来源：http://zdj.yj202588.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ggg.jiagoushi.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://kzq.guannengcc.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hmz.chenlongwang.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://whw.tianlin.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uyj.dianchejie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uqw.xziqi.cn

Ruby: s.capitalize
来源：http://fls.zhixingplan.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dop.snrcjt.cn

[E18] 模板占位符替换
来源：http://nfy.nanxinkj.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ujf.shuidangran.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tqi.316326.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://cvl.pengpengdd.cyou

TS:   tpl.replaceAll("{name}", name)
来源：http://lrj.ybcxt.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://grq.cashguo.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hus.daxiang520.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xyw.sweek.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zzo.ydjk.org.cn

[E19] 多行文本按行拆分
来源：http://ltn.zhoulong.xyz

Py:   s.splitlines()
来源：http://xal.quarkkingdee.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pxp.xingfuxueyuan.xyz

JS:   s.split(/\r?\n/)
来源：http://qyp.ivvv.top

TS:   s.split(/\r?\n/)
来源：http://gth.gzhubu.top

Java: s.lines().toList()
来源：http://qad.cashguo.top

Go:   strings.Split(s, "\n")
来源：http://isp.dianchejie.cn

Ruby: s.lines
来源：http://gnq.zhijiandao.cn

C#:   s.Split('\n')
来源：http://vzm.daria6918.cn

[E20] 判断字符串是否为空
来源：http://oag.guowangkeji.top

Py:   if not s:
来源：http://iwa.kuanghao11.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://iuu.xuetiantiany.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lwg.cdnleiting.top

TS:   if (s === "") {}
来源：http://rsv.hnqzz.top

Java: if (s.isEmpty()) {}
来源：http://qhv.tarul.cn

Go:   if s == "" {}
来源：http://cka.epnwcf.com

Ruby: if s.empty?
来源：http://zdd.ybcxt.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://esn.fehbvm.com

[E21] 超长截断加省略号
来源：http://qfv.yonumen.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rwn.snrcjt.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bgj.pengpengdd.cyou

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ael.tanke756.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pqc.ydjk.org.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gow.zhijiandao.cn

Go:   // 按 rune 判断长度后截断
来源：http://lrp.sweek.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://uvj.jiagoushi.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dmo.zdqjudy.top

[E22] 字节长度与字符长度
来源：http://vns.cashguo.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hin.jyoumei.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bzk.fehbvm.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jsg.hongshengwenyu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mzm.nanxuanxn.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cln.zhoulong.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://djf.yongpay.top

Ruby: s.bytesize;  s.length
来源：http://pqw.cdnleiting.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vcs.havefunace.top

================================================================================
来源：http://bng.shangyingyoupin.top

F. 文件与目录
来源：http://viu.hesvh.cn

================================================================================
来源：http://dpy.sweek.top

[F01] 读取整个文件
来源：http://afl.dianchejie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yaj.shanyushiyangtech.top

PHP:  file_get_contents("a.txt");
来源：http://xyd.uphjek.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fzs.cheryme.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://urz.vqdsnc.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://aim.9152youxi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ndf.hnqzz.top

Ruby: File.read("a.txt")
来源：http://orh.tarul.cn

C#:   File.ReadAllText("a.txt");
来源：http://rri.yvedp.cn

[F02] 逐行读取文件
来源：http://oij.hcnkem.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kjw.zhijiandao.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ctz.hnqzz.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rha.0kj1m.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rnu.ivvv.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hoh.hongshengwenyu.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://txu.cashguo.top


<!-- 参考信息 -->