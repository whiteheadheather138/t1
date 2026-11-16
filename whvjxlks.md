代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://slc.mhx1999.top

Go:   // 手写双层循环
来源：http://zyh.daxiang520.top

Ruby: nested.flatten
来源：http://fni.tarul.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bgh.mhx1999.top

[D19] 按字段分组
来源：http://dzl.vqdsnc.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jiu.quarkkingdee.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xiy.fktsv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wzm.vqdsnc.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://pev.svipenyu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fvv.yj20258.top

Go:   // 手写 map[string][]T
来源：http://swo.cdnleiting.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://gbd.pycfn.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rqc.yj20258.top

[D20] 统计每个元素出现次数
来源：http://wgo.ctjpmb.com

Py:   Counter(arr)
来源：http://fkf.chenzaomai.com

PHP:  array_count_values($arr);
来源：http://wgp.zhaomingkeji.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pix.haohaochexian.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lof.vehdjk.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bhs.cashguo.top

Go:   // 手写 map[T]int
来源：http://cmq.yuanzhike.top

Ruby: arr.tally
来源：http://ced.jianghu66.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kpj.redwolf501.top

[D21] 判断是否包含某元素
来源：http://ziz.zhaomingkeji.xyz

Py:   x in arr
来源：http://cky.yongpay.top

PHP:  in_array($x, $arr, true);
来源：http://lth.ivvv.top

JS:   arr.includes(x)
来源：http://ubm.hysaishi.cn

TS:   arr.includes(x)
来源：http://fpq.yuanzhike.top

Java: list.contains(x)
来源：http://yaj.feifeiyinyue.top

Go:   slices.Contains(arr, x)
来源：http://lao.jiagoushi.top

Ruby: arr.include?(x)
来源：http://tpz.zhongyouzk.top

C#:   list.Contains(x)
来源：http://noc.vehdjk.com

[D22] 复制数组（避免共享引用）
来源：http://qny.hysaishi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dkt.wangdashe.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jpt.pengpengdd.cyou

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pph.0kj1m.cn

TS:   [...arr];
来源：http://wzp.tian-w.cn

Java: new ArrayList<>(list);
来源：http://fhc.hysaishi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ivz.gogol.net.cn

Ruby: arr.dup;  arr.clone
来源：http://tno.nanxinkj.top

C#:   new List<int>(list);
来源：http://ryq.yvedp.cn

[D23] reduce 累积计算
来源：http://igb.xziqi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://idy.hfpthk.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ybr.cdnleiting.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vvv.meibo888.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qnk.cheryme.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://uyu.zhaomingkeji.xyz

Go:   // 手写循环
来源：http://tec.hongshengwenyu.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mrh.ybcxt.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wox.sysykeji.top

[D24] 字典 / Map 基本操作
来源：http://zlw.fzhhl.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ixn.meibo888.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mri.pengpengdd.cyou

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sym.jyoumei.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ypq.uphjek.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lyd.ywan-chungtsiang.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hty.jqgufenzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jqh.mhx1999.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://iby.zhengqikj.top

[D25] Set 集合去重与交并差
来源：http://roa.zdbjq.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://icl.havefunace.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://uzi.tian-w.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://noi.fengsongda.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fqf.ctjpmb.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dct.vehdjk.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://olp.jianghu66.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ful.52xcode.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qdw.shangyingyoupin.top

[D26] 数组转字符串
来源：http://qhl.birdmap.top

Py:   ", ".join(map(str, arr))
来源：http://yxl.zdbjq.cn

PHP:  implode(", ", $arr);
来源：http://htq.yvedp.cn

JS:   arr.join(", ")
来源：http://iji.dashuyun.cn

TS:   arr.join(", ")
来源：http://rrs.vehdjk.com

Java: String.join(", ", list)
来源：http://hzs.fehbvm.com

Go:   strings.Join(strs, ", ")
来源：http://jjb.ctjpmb.com

Ruby: arr.join(", ")
来源：http://lbt.sweek.top

C#:   string.Join(", ", list)
来源：http://vnu.vqdsnc.cn

================================================================================
来源：http://quh.shanyushiyangkeji.top

E. 字符串处理
来源：http://upo.yj20258888.top

================================================================================
来源：http://vib.cdnleiting.top

[E01] 拼接字符串
来源：http://poo.meibo888.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wsc.dianchejie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nxd.tian-w.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://puh.sjlbkw.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ano.gzhubu.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ccn.zhixingplan.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dab.jlsjyb.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lbr.yfazqb.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sro.andypj.xyz

[E02] 重复字符串
来源：http://lcu.svipenyu.cn

Py:   "ab" * 3
来源：http://jby.xuetiantiany.cn

PHP:  str_repeat("ab", 3);
来源：http://srp.guannengcc.top

JS:   "ab".repeat(3)
来源：http://jin.jyoumei.cn

TS:   "ab".repeat(3)
来源：http://wsu.sysykeji.top

Java: "ab".repeat(3)
来源：http://bzh.yuanzhike.top

Go:   strings.Repeat("ab", 3)
来源：http://rwp.jinyuanbaomall.cn

Ruby: "ab" * 3
来源：http://kmg.fktsv.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kmx.bbcook.cn

[E03] 截取子串
来源：http://snm.tian-w.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hxv.zdqjudy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tkx.wangshuangyany.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://seq.yuanzhike.top

TS:   s.slice(1, 4)
来源：http://joa.xuanzx.com

Java: s.substring(1, 4)
来源：http://cin.zhengqikj.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cml.aibaodan.cn

Ruby: s[1, 3];  s[1..3]
来源：http://uqg.ybcxt.top

C#:   s.Substring(1, 3)
来源：http://zrc.jqgfzy.top

[E04] 查找子串位置
来源：http://zdw.xuetiantiany.cn

Py:   s.find("x");  s.index("x")
来源：http://teo.zhengqikj.top

PHP:  strpos($s, "x");
来源：http://ois.feifeiyinyue.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lvh.bjfxy.top

TS:   s.indexOf("x")
来源：http://mcv.gzhubu.top

Java: s.indexOf("x")
来源：http://sva.zhongyouzk.top

Go:   strings.Index(s, "x")
来源：http://psh.xuanzx.com

Ruby: s.index("x")
来源：http://iim.zhixingplan.top

C#:   s.IndexOf("x")
来源：http://pln.feifeiyinyue.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://vjq.guowangkeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lhq.shangyingyoupin.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dzr.yongpay.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gni.yj20258888.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ekz.xuanzx.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tub.feifeiyinyue.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://grw.meibo888.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pdf.svipenyu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vhh.yuanzhike.top

[E06] 替换子串
来源：http://xqt.zhiwuduotai.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rnk.havefunace.top

PHP:  str_replace("a", "b", $s);
来源：http://ilp.316326.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sbe.sweek.top

TS:   s.replaceAll("a", "b")
来源：http://qrf.birdmap.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ari.dashuyun.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uky.xingfuxueyuan.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mah.guowangkeji.top

C#:   s.Replace("a", "b")
来源：http://arz.yj202588.top

[E07] 按分隔符拆分
来源：http://jue.shzxlz.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ynz.jinqigufen.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ymm.hongshengwenyu.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://lck.chenzaomai.com

TS:   s.split(",")
来源：http://gyk.yuanzhike.top

Java: s.split(",");  s.split("\\s+")
来源：http://kyn.hongshengwenyu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ayf.aizwys.cn

Ruby: s.split(",");  s.split
来源：http://tzd.uphjek.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qeh.hfpthk.cn

[E08] 数组按分隔符合并
来源：http://txk.ydjk.org.cn

Py:   ",".join(items)
来源：http://vsx.sjlbkw.cn

PHP:  implode(",", $items);
来源：http://tgg.hfpthk.cn

JS:   items.join(",")
来源：http://uwr.jinqigfzy.top

TS:   items.join(",")
来源：http://wbn.daxiang520.top

Java: String.join(",", items)
来源：http://dpg.pycfn.com

Go:   strings.Join(items, ",")
来源：http://tcd.jqgufenzy.top

Ruby: items.join(",")
来源：http://hmv.havefunace.top

C#:   string.Join(",", items)
来源：http://hyv.smart0.xyz

[E09] 去除所有空白字符
来源：http://snd.jyoumei.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rpp.xingfuxueyuan.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://oiv.hongshengwenyu.top

JS:   s.replace(/\s+/g, "")
来源：http://heu.hnxiangtu.top

TS:   s.replace(/\s+/g, "")
来源：http://dgv.shanyushiyangkeji.top

Java: s.replaceAll("\\s+", "")
来源：http://fmk.yj202588.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://aaj.zhongyouzk.top

Ruby: s.gsub(/\s+/, "")
来源：http://dtq.zhijiandao.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ivc.tarul.cn

[E10] 左侧补零 / 定长填充
来源：http://hje.ivvv.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://neg.pycfn.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bjb.chenjidiqi.icu

JS:   "7".padStart(3, "0")
来源：http://zxi.xinyue.icu

TS:   "7".padStart(3, "0")
来源：http://rfq.yuanzhike.top

Java: String.format("%03d", 7)
来源：http://mii.yj20258888.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ekh.ppjwa.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vvk.havefunace.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ewe.ehwqpu.com

[E11] 反转字符串
来源：http://wbd.meibo888.top

Py:   s[::-1]
来源：http://qfu.chenjidiqi.icu

PHP:  strrev($s);
来源：http://zpu.ctjpmb.com

JS:   [...s].reverse().join("")
来源：http://yzz.nwbrower.top

TS:   [...s].reverse().join("")
来源：http://cho.jinghuilouyu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://yca.bbcook.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://nor.yj20258.top

Ruby: s.reverse
来源：http://jgi.hfpthk.cn

C#:   new string(s.Reverse().ToArray())
来源：http://smk.svipenyu.cn

[E12] 统计某字符出现次数
来源：http://rcb.guannengcc.top

Py:   s.count("a")
来源：http://ful.shuidangran.top

PHP:  substr_count($s, "a");
来源：http://adn.jqgfzy.top

JS:   s.split("a").length - 1
来源：http://wmh.quarkkingdee.top

TS:   s.split("a").length - 1
来源：http://nhq.wangshuangyany.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bsb.xuetiantiany.cn

Go:   strings.Count(s, "a")
来源：http://xxu.zhiwuduotai.top

Ruby: s.count("a")
来源：http://tep.fehbvm.com

C#:   s.Count(c => c == 'a')
来源：http://zgb.ybcxt.top

[E13] 逐字符遍历
来源：http://kcr.cdnleiting.top

Py:   for ch in s: print(ch)
来源：http://ovk.hywenlv.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vaa.hnqzz.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ewm.tarul.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xnt.ybcxt.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vcx.shanyushiyangtech.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tak.fehbvm.com

Ruby: s.each_char { |ch| puts ch }
来源：http://tar.zdqjudy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jmy.tanke756.top

[E14] URL 编码与 Base64
来源：http://mgp.daria6918.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fhw.redwolf501.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://nwo.pengpengdd.cyou

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xzj.zhixingplan.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lop.xingfuxueyuan.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yyz.hysaishi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fij.yfazqb.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vkq.daria6918.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bnz.jyoumei.cn

[E15] HTML 转义 / 反转义
来源：http://kxu.bjfxy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://qsw.gaohongyu789.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tdq.sweek.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cvd.xziqi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://vbw.ywan-chungtsiang.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nss.jinyuanbaomall.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rhn.hysaishi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://muh.chenzaomai.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hgr.pycfn.com

[E16] 数字千分位
来源：http://yjj.jinqigfzy.top

Py:   f"{1234567:,}"
来源：http://ycx.gotoacloud.top

PHP:  number_format(1234567);
来源：http://bcf.ywan-chungtsiang.top

JS:   (1234567).toLocaleString("en-US")
来源：http://gsc.hnqzz.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ydp.yfazqb.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sip.xylfe.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://umo.yongpay.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bos.yangfankeji.com

C#:   1234567.ToString("N0")
来源：http://yrg.yueranfly.top

[E17] 首字母大写
来源：http://dgd.snrcjt.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jqf.9152youxi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ufg.jlsjyb.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kmz.cashguo.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gbi.daria6918.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rll.52xcode.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ocp.yj20258.top

Ruby: s.capitalize
来源：http://gkf.zdqjudy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://spj.nanxinkj.top

[E18] 模板占位符替换
来源：http://gaz.sufxvd.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kex.yfazqb.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cjr.yangfankeji.com

JS:   tpl.replaceAll("{name}", name)
来源：http://cra.andypj.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://yiu.hfpthk.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pou.zycfv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hqp.wangdashe.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://joh.yfazqb.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kus.meibo888.top

[E19] 多行文本按行拆分
来源：http://hti.yj20258.top

Py:   s.splitlines()
来源：http://dgt.ydjk.org.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bsy.fehbvm.com

JS:   s.split(/\r?\n/)
来源：http://mjz.feifeiyinyue.top

TS:   s.split(/\r?\n/)
来源：http://qvi.hcnkem.com

Java: s.lines().toList()
来源：http://ulg.wangdashe.top

Go:   strings.Split(s, "\n")
来源：http://uwg.nanxinkj.top

Ruby: s.lines
来源：http://hxu.jyoumei.cn

C#:   s.Split('\n')
来源：http://apd.wangshuangyany.cn

[E20] 判断字符串是否为空
来源：http://nqd.jinghuilouyu.cn

Py:   if not s:
来源：http://quu.daria6918.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://feh.meibo888.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dah.meibo888.top

TS:   if (s === "") {}
来源：http://lix.gotoacloud.top

Java: if (s.isEmpty()) {}
来源：http://uqw.zhengqikj.top

Go:   if s == "" {}
来源：http://xyb.zhixingplan.top

Ruby: if s.empty?
来源：http://usr.cheryme.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://joy.zhengqikj.top

[E21] 超长截断加省略号
来源：http://mjm.xuetiantiany.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://klq.cdnleiting.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pcw.yj20258.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ezu.hysaishi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sca.zhongyouzk.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rta.hysaishi.cn

Go:   // 按 rune 判断长度后截断
来源：http://bnp.hammf.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://omh.sjlbkw.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mcp.uphjek.com

[E22] 字节长度与字符长度
来源：http://iok.gogol.net.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bhg.tianlin.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mub.snrcjt.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ujc.ppjwa.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ymj.nanxuanxn.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gaf.zdqjudy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ouk.yj202588.top

Ruby: s.bytesize;  s.length
来源：http://buk.smart0.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pgg.316326.xyz

================================================================================
来源：http://ace.chenlongwang.top

F. 文件与目录
来源：http://mjv.ydjk.org.cn

================================================================================
来源：http://glh.9152youxi.cn

[F01] 读取整个文件
来源：http://sno.quarkkingdee.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yjh.cheryme.top

PHP:  file_get_contents("a.txt");
来源：http://wqu.guannengcc.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gmo.xinyue.icu

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hli.ivvv.top

Java: Files.readString(Path.of("a.txt"))
来源：http://fps.fktsv.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gmm.52xcode.cn

Ruby: File.read("a.txt")
来源：http://cba.shanyushiyangtech.top

C#:   File.ReadAllText("a.txt");
来源：http://xvn.0kj1m.cn

[F02] 逐行读取文件
来源：http://szh.vqdsnc.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://glt.jinqigfzy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://awq.zhijiandao.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pja.epnwcf.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tyx.hesvh.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://alp.jqgufenzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hpd.ydjk.org.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nis.guowangkeji.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jso.sufxvd.cn

[F03] 写入文件（覆盖）
来源：http://dmw.redwolf501.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tsx.hfpthk.cn


<!-- 参考信息 -->