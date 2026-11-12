代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wps.jlsjyb.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dun.wangdashe.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zbv.yongpay.top

TS:   [...arr];
来源：http://kks.zdqjudy.top

Java: new ArrayList<>(list);
来源：http://aek.jinqigufen.top

Go:   copied := append([]int(nil), arr...)
来源：http://ejt.tianlin.xyz

Ruby: arr.dup;  arr.clone
来源：http://lvr.redwolf501.top

C#:   new List<int>(list);
来源：http://zlj.haohaochexian.top

[D23] reduce 累积计算
来源：http://gpy.ydzc1.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://umx.xingfuxueyuan.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://oni.zhengqikj.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eff.kuanghao11.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yzf.yueranfly.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://axh.chenzaomai.com

Go:   // 手写循环
来源：http://xzi.shanyushiyangtech.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://eae.hammf.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yeq.shanyushiyangtech.top

[D24] 字典 / Map 基本操作
来源：http://mmr.ydjk.org.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wdd.jlsjyb.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ozv.jinghuilouyu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kxl.vehdjk.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vni.shanyushiyangkeji.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fhe.bjfxy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gqu.xuanzx.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vnk.shanyushiyangtech.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rdm.zhiwuduotai.top

[D25] Set 集合去重与交并差
来源：http://cuu.gotoacloud.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vhb.yuxming.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mfv.jyoumei.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dtb.hammf.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mmp.wangshuangyany.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bmk.xuanzx.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ajs.shanyushiyangkeji.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hri.zhiwuduotai.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://iig.cashguo.top

[D26] 数组转字符串
来源：http://fnt.fanxiaobao.xyz

Py:   ", ".join(map(str, arr))
来源：http://xwv.kuanghao11.cn

PHP:  implode(", ", $arr);
来源：http://kwh.zycfv.cn

JS:   arr.join(", ")
来源：http://kjs.guowangkeji.top

TS:   arr.join(", ")
来源：http://hpe.zhongyouzk.top

Java: String.join(", ", list)
来源：http://cec.sjlbkw.cn

Go:   strings.Join(strs, ", ")
来源：http://lhs.ivvv.top

Ruby: arr.join(", ")
来源：http://oqi.andypj.xyz

C#:   string.Join(", ", list)
来源：http://bdg.ehwqpu.com

================================================================================
来源：http://zmf.kuanghao11.cn

E. 字符串处理
来源：http://vow.fanxiaobao.xyz

================================================================================
来源：http://mqt.ppjwa.cn

[E01] 拼接字符串
来源：http://ncy.sxryk.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ivn.vehdjk.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hek.pycfn.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mrg.tanke756.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pdg.uphjek.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://adx.yangfankeji.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hou.xuanzx.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ygg.gaohongyu789.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gkp.uphjek.com

[E02] 重复字符串
来源：http://giq.zhongyouzk.top

Py:   "ab" * 3
来源：http://wbd.fktsv.cn

PHP:  str_repeat("ab", 3);
来源：http://yrz.xziqi.cn

JS:   "ab".repeat(3)
来源：http://gmb.yangfankeji.com

TS:   "ab".repeat(3)
来源：http://hcw.hysaishi.cn

Java: "ab".repeat(3)
来源：http://sdk.bjfxy.top

Go:   strings.Repeat("ab", 3)
来源：http://der.ehwqpu.com

Ruby: "ab" * 3
来源：http://xob.wangdashe.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://aqc.andypj.xyz

[E03] 截取子串
来源：http://kkv.xylfe.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bkq.andypj.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ltk.jyoumei.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sqz.jlsjyb.cn

TS:   s.slice(1, 4)
来源：http://xvb.quarkkingdee.top

Java: s.substring(1, 4)
来源：http://qag.haohaochexian.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nfh.fanxiaobao.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://hws.andypj.xyz

C#:   s.Substring(1, 3)
来源：http://zfh.tianlin.xyz

[E04] 查找子串位置
来源：http://gum.gaohongyu789.top

Py:   s.find("x");  s.index("x")
来源：http://kyj.sysykeji.top

PHP:  strpos($s, "x");
来源：http://cos.chenlongwang.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tcl.hnqzz.top

TS:   s.indexOf("x")
来源：http://dar.yj202588.top

Java: s.indexOf("x")
来源：http://tei.guannengcc.top

Go:   strings.Index(s, "x")
来源：http://wcj.zhixingplan.top

Ruby: s.index("x")
来源：http://lmp.ivvv.top

C#:   s.IndexOf("x")
来源：http://snv.fktsv.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://fzr.wangdashe.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://oip.fehbvm.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hlf.sysykeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xeo.sxryk.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ali.hfpthk.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kvj.xingfuxueyuan.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rry.tian-w.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://trk.zhixingplan.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tjl.chenjidiqi.icu

[E06] 替换子串
来源：http://edh.yangfankeji.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jvf.yj202588.top

PHP:  str_replace("a", "b", $s);
来源：http://vdv.jinghuilouyu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ana.xziqi.cn

TS:   s.replaceAll("a", "b")
来源：http://dnv.xingfuxueyuan.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tts.hysaishi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://scl.yuxming.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xec.bbcook.cn

C#:   s.Replace("a", "b")
来源：http://edg.hcnkem.com

[E07] 按分隔符拆分
来源：http://wyr.shuidangran.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lfs.yongpay.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://anp.jiagoushi.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://hog.jinqigufen.top

TS:   s.split(",")
来源：http://dis.zhaomingkeji.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://rbm.yj20258888.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bru.uphjek.com

Ruby: s.split(",");  s.split
来源：http://bak.pycfn.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://smx.quarkkingdee.top

[E08] 数组按分隔符合并
来源：http://zvy.hongshengwenyu.top

Py:   ",".join(items)
来源：http://oui.jyoumei.cn

PHP:  implode(",", $items);
来源：http://kzu.zdqjudy.top

JS:   items.join(",")
来源：http://ovf.daxiang520.top

TS:   items.join(",")
来源：http://lja.shangyingyoupin.top

Java: String.join(",", items)
来源：http://imp.jlsjyb.cn

Go:   strings.Join(items, ",")
来源：http://tpc.kuanghao11.cn

Ruby: items.join(",")
来源：http://sfv.yuxming.cn

C#:   string.Join(",", items)
来源：http://glx.pengpengdd.cyou

[E09] 去除所有空白字符
来源：http://quy.yongpay.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xvq.sweek.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ovk.tianlin.xyz

JS:   s.replace(/\s+/g, "")
来源：http://nbp.xylfe.cn

TS:   s.replace(/\s+/g, "")
来源：http://xra.feifeiyinyue.top

Java: s.replaceAll("\\s+", "")
来源：http://zwb.sjlbkw.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://lee.feifeiyinyue.top

Ruby: s.gsub(/\s+/, "")
来源：http://wsr.zdbjq.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xmc.cheryme.top

[E10] 左侧补零 / 定长填充
来源：http://quv.haohaochexian.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fsa.aizwys.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xbm.ppjwa.cn

JS:   "7".padStart(3, "0")
来源：http://rwh.yj20258888.top

TS:   "7".padStart(3, "0")
来源：http://knc.hywenlv.cn

Java: String.format("%03d", 7)
来源：http://caw.daria6918.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://gnq.shanyushiyangtech.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xys.tian-w.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lki.tarul.cn

[E11] 反转字符串
来源：http://bid.xuetiantiany.cn

Py:   s[::-1]
来源：http://fjn.ppjwa.cn

PHP:  strrev($s);
来源：http://uii.zhijiandao.cn

JS:   [...s].reverse().join("")
来源：http://gtp.cashguo.top

TS:   [...s].reverse().join("")
来源：http://glh.bbcook.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://tsr.zhoulong.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://fmm.sjlbkw.cn

Ruby: s.reverse
来源：http://jvz.wangdashe.top

C#:   new string(s.Reverse().ToArray())
来源：http://uug.gogol.net.cn

[E12] 统计某字符出现次数
来源：http://bpl.yuxming.cn

Py:   s.count("a")
来源：http://cav.hcnkem.com

PHP:  substr_count($s, "a");
来源：http://lpp.ywan-chungtsiang.top

JS:   s.split("a").length - 1
来源：http://bjz.316326.xyz

TS:   s.split("a").length - 1
来源：http://efx.bjfxy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://umr.nwbrower.top

Go:   strings.Count(s, "a")
来源：http://qgv.xingfuxueyuan.xyz

Ruby: s.count("a")
来源：http://fhd.wangdashe.top

C#:   s.Count(c => c == 'a')
来源：http://fbf.316326.xyz

[E13] 逐字符遍历
来源：http://loy.fehbvm.com

Py:   for ch in s: print(ch)
来源：http://sjr.hammf.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wjh.yj202588.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://csq.hongshengwenyu.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://pvf.guannengcc.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rsy.xylfe.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vam.cheryme.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ibs.haohaochexian.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wpy.quarkkingdee.top

[E14] URL 编码与 Base64
来源：http://uol.aibaodan.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kbf.chenlongwang.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://rov.zhijiandao.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jeu.zhijiandao.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bwq.yueranfly.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://exj.xziqi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uhc.bjfxy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qgx.tianlin.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fjr.cucudq.cn

[E15] HTML 转义 / 反转义
来源：http://oyy.cheryme.top

Py:   html.escape(s);  html.unescape(s)
来源：http://yxr.jinqigufen.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sqy.yanxiufei.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kys.zhiwuduotai.top

TS:   // 同上，务必做 XSS 过滤
来源：http://inn.tianlin.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vwt.iojbl.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://src.jinqigufen.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wqs.nwbrower.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dnx.jiagoushi.top

[E16] 数字千分位
来源：http://obv.yuxming.cn

Py:   f"{1234567:,}"
来源：http://lfc.smart0.xyz

PHP:  number_format(1234567);
来源：http://ekf.wangdashe.top

JS:   (1234567).toLocaleString("en-US")
来源：http://srp.pycfn.com

TS:   (1234567).toLocaleString("en-US")
来源：http://rgs.xingfuxueyuan.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wmn.wangshuangyany.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yri.dashuyun.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://oth.jqgfzy.top

C#:   1234567.ToString("N0")
来源：http://fzi.gaohongyu789.top

[E17] 首字母大写
来源：http://iez.bbcook.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nhk.redwolf501.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ndy.sxryk.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pyq.0kj1m.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://igc.hywenlv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://amg.jyoumei.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ofo.xinyue.icu

Ruby: s.capitalize
来源：http://xzx.cdnleiting.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jmd.yongpay.top

[E18] 模板占位符替换
来源：http://ius.bjfxy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gtb.shuidangran.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gxe.ydjk.org.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zko.yonumen.top

TS:   tpl.replaceAll("{name}", name)
来源：http://dar.nwbrower.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xtm.nwbrower.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lrc.tanke756.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://khn.svipenyu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ytb.smart0.xyz

[E19] 多行文本按行拆分
来源：http://jjn.fanxiaobao.xyz

Py:   s.splitlines()
来源：http://eof.xziqi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gft.chenjidiqi.icu

JS:   s.split(/\r?\n/)
来源：http://xpp.kuanghao11.cn

TS:   s.split(/\r?\n/)
来源：http://uxq.xziqi.cn

Java: s.lines().toList()
来源：http://xgl.aizwys.cn

Go:   strings.Split(s, "\n")
来源：http://bjp.shanyushiyangkeji.top

Ruby: s.lines
来源：http://fzy.zhijiandao.cn

C#:   s.Split('\n')
来源：http://nyi.zhoulong.xyz

[E20] 判断字符串是否为空
来源：http://fru.sxryk.cn

Py:   if not s:
来源：http://ruj.jqgfzy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pxh.yj20258.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://clb.cucudq.cn

TS:   if (s === "") {}
来源：http://zzl.haohaochexian.top

Java: if (s.isEmpty()) {}
来源：http://ktq.xingfuxueyuan.xyz

Go:   if s == "" {}
来源：http://aqe.yvedp.cn

Ruby: if s.empty?
来源：http://ihu.sysykeji.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lfq.yongpay.top

[E21] 超长截断加省略号
来源：http://tst.bjfxy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fjz.jinyuanbaomall.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tqi.andypj.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rra.xinyue.icu

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kvy.daria6918.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vyw.shuidangran.top

Go:   // 按 rune 判断长度后截断
来源：http://qxr.vehdjk.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tsm.shanyushiyangtech.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mlv.jiagoushi.top

[E22] 字节长度与字符长度
来源：http://imy.tarul.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://iyv.gotoacloud.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zeu.aibaodan.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://txk.gogol.net.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xde.uphjek.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://oyq.zhijiandao.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://djf.redwolf501.top

Ruby: s.bytesize;  s.length
来源：http://oah.pengpengdd.cyou

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gvk.nwbrower.top

================================================================================
来源：http://jlh.jyoumei.cn

F. 文件与目录
来源：http://etv.52xcode.cn

================================================================================
来源：http://ryy.pycfn.com

[F01] 读取整个文件
来源：http://kov.tarul.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fkt.zycfv.cn

PHP:  file_get_contents("a.txt");
来源：http://mpk.ydjk.org.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ujh.yanxiufei.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uyl.yuanzhike.top

Java: Files.readString(Path.of("a.txt"))
来源：http://oem.feifeiyinyue.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lue.havefunace.top

Ruby: File.read("a.txt")
来源：http://xep.guowangkeji.top

C#:   File.ReadAllText("a.txt");
来源：http://yxm.bjfxy.top

[F02] 逐行读取文件
来源：http://vwa.snrcjt.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lfl.shzxlz.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wbf.tarul.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zjv.daxiang520.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://veo.ppjwa.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ads.ehwqpu.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bcp.gogol.net.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ynv.jlsjyb.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ulx.zhixingplan.top

[F03] 写入文件（覆盖）
来源：http://sbz.iojbl.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zcc.ybcxt.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://psw.shanyushiyangtech.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uaq.xuetiantiany.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cto.52xcode.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://czp.zdqjudy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://itb.zdbjq.cn

Ruby: File.write("a.txt", "hi")
来源：http://ktp.jqgfzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://oga.fktsv.cn

[F04] 追加写入文件
来源：http://utl.tian-w.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://otl.cqqwz.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kpb.wangdashe.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dvn.quarkkingdee.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ksk.zhoulong.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ztl.ywan-chungtsiang.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ogw.guowangkeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://abr.hnxiangtu.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://iko.sjlbkw.cn

[F05] 判断文件或目录是否存在
来源：http://upp.fanxiaobao.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mre.guowangkeji.top

PHP:  file_exists("a.txt");
来源：http://nee.fanxiaobao.xyz

JS:   fs.existsSync("a.txt")
来源：http://lsw.iojbl.cn

TS:   fs.existsSync("a.txt")
来源：http://ayo.xuanzx.com

Java: Files.exists(Path.of("a.txt"))
来源：http://klz.dashuyun.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pzn.hfpthk.cn

Ruby: File.exist?("a.txt")
来源：http://wkm.redwolf501.top

C#:   File.Exists("a.txt")
来源：http://oes.zycfv.cn

[F06] 删除文件
来源：http://rfg.redwolf501.top

Py:   os.remove("a.txt")
来源：http://csi.zhiwuduotai.top

PHP:  unlink("a.txt");
来源：http://rib.zhiwuduotai.top

JS:   fs.unlinkSync("a.txt")
来源：http://whx.havefunace.top

TS:   fs.unlinkSync("a.txt")
来源：http://knp.jqgfzy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://plr.cucudq.cn

Go:   os.Remove("a.txt")
来源：http://nrq.jinqigfzy.top


<!-- 参考信息 -->