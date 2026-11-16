代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://obj.jinghuilouyu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xxb.bjfxy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zzy.zhoulong.xyz

TS:   [...arr];
来源：http://tgi.bbcook.cn

Java: new ArrayList<>(list);
来源：http://lou.shzxlz.cn

Go:   copied := append([]int(nil), arr...)
来源：http://kpk.vehdjk.com

Ruby: arr.dup;  arr.clone
来源：http://izo.xingfuxueyuan.xyz

C#:   new List<int>(list);
来源：http://eae.meibo888.top

[D23] reduce 累积计算
来源：http://wbz.chenjidiqi.icu

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zri.tanke756.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gmv.zycfv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xkz.havefunace.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fwv.xziqi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://juh.nwbrower.top

Go:   // 手写循环
来源：http://azy.yueranfly.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rlv.hnxiangtu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dhj.hfpthk.cn

[D24] 字典 / Map 基本操作
来源：http://wmv.mhx1999.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wbv.xinyue.icu

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xwp.hysaishi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fav.jianghu66.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bsl.jinqigfzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mmx.mhx1999.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eld.tianlin.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wfo.sweek.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hkt.jinqigufen.top

[D25] Set 集合去重与交并差
来源：http://lee.fktsv.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bwg.yueranfly.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://awp.zdqjudy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://njt.sxryk.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xkc.andypj.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bsd.ppjwa.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zuh.yj20258.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mfc.pycfn.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zpc.ctjpmb.com

[D26] 数组转字符串
来源：http://dcx.cdnleiting.top

Py:   ", ".join(map(str, arr))
来源：http://fla.hongshengwenyu.top

PHP:  implode(", ", $arr);
来源：http://plj.andypj.xyz

JS:   arr.join(", ")
来源：http://vya.jinqigfzy.top

TS:   arr.join(", ")
来源：http://aug.guannengcc.top

Java: String.join(", ", list)
来源：http://mpj.hfpthk.cn

Go:   strings.Join(strs, ", ")
来源：http://bzp.fzhhl.top

Ruby: arr.join(", ")
来源：http://exi.pengpengdd.cyou

C#:   string.Join(", ", list)
来源：http://vit.zhijiandao.cn

================================================================================
来源：http://tki.tanke756.top

E. 字符串处理
来源：http://kaw.yj20258888.top

================================================================================
来源：http://nmx.wangdashe.top

[E01] 拼接字符串
来源：http://uqd.yongpay.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tqn.jyoumei.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fee.wangshuangyany.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ocf.iojbl.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tij.sxryk.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://khg.fzhhl.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://evw.chenzaomai.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mnu.gogol.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wiu.uphjek.com

[E02] 重复字符串
来源：http://nyl.xziqi.cn

Py:   "ab" * 3
来源：http://igt.zdqjudy.top

PHP:  str_repeat("ab", 3);
来源：http://hbc.jianghu66.top

JS:   "ab".repeat(3)
来源：http://gty.sweek.top

TS:   "ab".repeat(3)
来源：http://hre.zdqjudy.top

Java: "ab".repeat(3)
来源：http://jlk.tanke756.top

Go:   strings.Repeat("ab", 3)
来源：http://cnx.tarul.cn

Ruby: "ab" * 3
来源：http://rir.chenjidiqi.icu

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://urp.cdnleiting.top

[E03] 截取子串
来源：http://zbk.vehdjk.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://log.fengsongda.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bmx.fehbvm.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://syt.hcnkem.com

TS:   s.slice(1, 4)
来源：http://mua.epnwcf.com

Java: s.substring(1, 4)
来源：http://kku.ppjwa.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cvk.zhaomingkeji.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://jfg.jqgufenzy.top

C#:   s.Substring(1, 3)
来源：http://qdw.zhongyouzk.top

[E04] 查找子串位置
来源：http://tah.nanxuanxn.top

Py:   s.find("x");  s.index("x")
来源：http://kym.daria6918.cn

PHP:  strpos($s, "x");
来源：http://nia.yfazqb.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ctr.snrcjt.cn

TS:   s.indexOf("x")
来源：http://sho.ydzc1.top

Java: s.indexOf("x")
来源：http://sku.zdqjudy.top

Go:   strings.Index(s, "x")
来源：http://oia.pengpengdd.cyou

Ruby: s.index("x")
来源：http://qls.xingfuxueyuan.xyz

C#:   s.IndexOf("x")
来源：http://bir.shangyingyoupin.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://icf.shangyingyoupin.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://esv.dianchejie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ooz.zycfv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://osv.tarul.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ydp.tanke756.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kuu.jinqigfzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fpd.wangshuangyany.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://eng.shanyushiyangkeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dgi.vqdsnc.cn

[E06] 替换子串
来源：http://gmn.tianlin.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://joh.jlsjyb.cn

PHP:  str_replace("a", "b", $s);
来源：http://vhm.yanxiufei.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qzl.xylfe.cn

TS:   s.replaceAll("a", "b")
来源：http://ffu.hcnkem.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aqi.jinqigufen.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hib.fzhhl.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cgb.iojbl.cn

C#:   s.Replace("a", "b")
来源：http://wgz.yj20258.top

[E07] 按分隔符拆分
来源：http://mwg.fehbvm.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lfn.ydjk.org.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://afx.jqgufenzy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://biq.yj20258.top

TS:   s.split(",")
来源：http://ykt.jiagoushi.top

Java: s.split(",");  s.split("\\s+")
来源：http://zld.hesvh.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://oeu.quarkkingdee.top

Ruby: s.split(",");  s.split
来源：http://qfj.hnqzz.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pmw.quarkkingdee.top

[E08] 数组按分隔符合并
来源：http://gjo.jqgufenzy.top

Py:   ",".join(items)
来源：http://voy.gogol.net.cn

PHP:  implode(",", $items);
来源：http://bdq.jyoumei.cn

JS:   items.join(",")
来源：http://sis.cdnleiting.top

TS:   items.join(",")
来源：http://kqb.fanxiaobao.xyz

Java: String.join(",", items)
来源：http://rnf.ydjk.org.cn

Go:   strings.Join(items, ",")
来源：http://ewx.jqgfzy.top

Ruby: items.join(",")
来源：http://kud.yj202588.top

C#:   string.Join(",", items)
来源：http://dsc.shangyingyoupin.top

[E09] 去除所有空白字符
来源：http://ovq.meibo888.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gdg.xinyue.icu

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mtu.nanxuanxn.top

JS:   s.replace(/\s+/g, "")
来源：http://fbw.iojbl.cn

TS:   s.replace(/\s+/g, "")
来源：http://zyt.xziqi.cn

Java: s.replaceAll("\\s+", "")
来源：http://fnj.zhongyouzk.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ffn.cheryme.top

Ruby: s.gsub(/\s+/, "")
来源：http://akq.yanxiufei.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fxo.xinyue.icu

[E10] 左侧补零 / 定长填充
来源：http://mfh.chenzaomai.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xzh.hfpthk.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nkn.wangdashe.top

JS:   "7".padStart(3, "0")
来源：http://qjf.fktsv.cn

TS:   "7".padStart(3, "0")
来源：http://peh.cashguo.top

Java: String.format("%03d", 7)
来源：http://zlm.gaohongyu789.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://vry.ydjk.org.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://iqi.dianchejie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lvg.hfpthk.cn

[E11] 反转字符串
来源：http://gsu.ydzc1.top

Py:   s[::-1]
来源：http://epv.hongshengwenyu.top

PHP:  strrev($s);
来源：http://yuo.shangyingyoupin.top

JS:   [...s].reverse().join("")
来源：http://luk.yongpay.top

TS:   [...s].reverse().join("")
来源：http://hvc.xuetiantiany.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mmt.iojbl.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://pyh.jiagoushi.top

Ruby: s.reverse
来源：http://wnk.zhengqikj.top

C#:   new string(s.Reverse().ToArray())
来源：http://juy.zhengqikj.top

[E12] 统计某字符出现次数
来源：http://ttt.gogol.net.cn

Py:   s.count("a")
来源：http://ooz.c1oappe.top

PHP:  substr_count($s, "a");
来源：http://xfe.hywenlv.cn

JS:   s.split("a").length - 1
来源：http://pyy.jinqigfzy.top

TS:   s.split("a").length - 1
来源：http://hlg.nanxinkj.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wmu.ivvv.top

Go:   strings.Count(s, "a")
来源：http://zpz.pycfn.com

Ruby: s.count("a")
来源：http://fwv.hywenlv.cn

C#:   s.Count(c => c == 'a')
来源：http://yrm.wangdashe.top

[E13] 逐字符遍历
来源：http://lwo.guannengcc.top

Py:   for ch in s: print(ch)
来源：http://spu.tarul.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://thr.meibo888.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ndr.sjlbkw.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vdr.gzhubu.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://erv.nanxuanxn.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://khp.ivvv.top

Ruby: s.each_char { |ch| puts ch }
来源：http://mps.shanyushiyangkeji.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bqa.hfpthk.cn

[E14] URL 编码与 Base64
来源：http://qen.dashuyun.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ynw.havefunace.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://vbz.pycfn.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ggm.cqqwz.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uag.uphjek.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uxi.shanyushiyangtech.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bhv.nanxuanxn.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kkv.feifeiyinyue.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ejc.bbcook.cn

[E15] HTML 转义 / 反转义
来源：http://rzq.sxryk.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://dtl.vqdsnc.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nub.yvedp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rjn.yanxiufei.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://iye.jinqigufen.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qwl.zhiwuduotai.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://meg.yongpay.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rto.shanyushiyangtech.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rjv.epnwcf.com

[E16] 数字千分位
来源：http://iyk.wangshuangyany.cn

Py:   f"{1234567:,}"
来源：http://csy.cqqwz.cn

PHP:  number_format(1234567);
来源：http://ctu.aibaodan.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://grz.52xcode.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ctb.guowangkeji.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fdb.shanyushiyangtech.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wpn.gotoacloud.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wvh.haohaochexian.top

C#:   1234567.ToString("N0")
来源：http://htf.cucudq.cn

[E17] 首字母大写
来源：http://der.dianchejie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zhx.hcnkem.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://ayy.jiagoushi.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://onb.52xcode.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jir.jinqigufen.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sen.meibo888.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sgr.hysaishi.cn

Ruby: s.capitalize
来源：http://aoo.vqdsnc.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qzr.xinyue.icu

[E18] 模板占位符替换
来源：http://rhe.yuanzhike.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://las.vqdsnc.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://reb.daxiang520.top

JS:   tpl.replaceAll("{name}", name)
来源：http://fva.jinqigfzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://gwq.havefunace.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xix.zdqjudy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rdd.ehwqpu.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xsf.wangdashe.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ncn.xziqi.cn

[E19] 多行文本按行拆分
来源：http://vwb.vehdjk.com

Py:   s.splitlines()
来源：http://jef.ywan-chungtsiang.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://som.xinyue.icu

JS:   s.split(/\r?\n/)
来源：http://waz.andypj.xyz

TS:   s.split(/\r?\n/)
来源：http://hkt.jqgufenzy.top

Java: s.lines().toList()
来源：http://ceo.xuanzx.com

Go:   strings.Split(s, "\n")
来源：http://oxa.316326.xyz

Ruby: s.lines
来源：http://nxi.sufxvd.cn

C#:   s.Split('\n')
来源：http://bhx.dashuyun.cn

[E20] 判断字符串是否为空
来源：http://ptm.aizwys.cn

Py:   if not s:
来源：http://kui.ydzc1.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yok.c1oappe.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yka.ywan-chungtsiang.top

TS:   if (s === "") {}
来源：http://hid.shanyushiyangkeji.top

Java: if (s.isEmpty()) {}
来源：http://kdn.ywan-chungtsiang.top

Go:   if s == "" {}
来源：http://ydy.cheryme.top

Ruby: if s.empty?
来源：http://fgu.smart0.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dqm.nanxuanxn.top

[E21] 超长截断加省略号
来源：http://umt.sxryk.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cmt.gogol.net.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://asr.shangyingyoupin.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ezh.yonumen.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jvd.pycfn.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cff.fzhhl.top

Go:   // 按 rune 判断长度后截断
来源：http://tji.birdmap.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wcb.52xcode.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cog.fzhhl.top

[E22] 字节长度与字符长度
来源：http://bds.xylfe.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zlw.xylfe.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fdd.jinghuilouyu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yrq.0kj1m.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dzo.birdmap.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://iim.iojbl.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://chv.jinqigufen.top

Ruby: s.bytesize;  s.length
来源：http://rjt.cashguo.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nio.zhengqikj.top

================================================================================
来源：http://dbo.bbcook.cn

F. 文件与目录
来源：http://wng.aibaodan.cn

================================================================================
来源：http://sfc.gotoacloud.top

[F01] 读取整个文件
来源：http://jxu.tian-w.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://iuh.wangdashe.top

PHP:  file_get_contents("a.txt");
来源：http://tdv.tian-w.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jaw.hesvh.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gnh.gzhubu.top

Java: Files.readString(Path.of("a.txt"))
来源：http://vie.jinqigfzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nah.quarkkingdee.top

Ruby: File.read("a.txt")
来源：http://kga.ydzc1.top

C#:   File.ReadAllText("a.txt");
来源：http://hsf.ydjk.org.cn

[F02] 逐行读取文件
来源：http://gck.mhx1999.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dap.fzhhl.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uze.chenzaomai.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ehi.cheryme.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qul.0kj1m.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dqz.jinqigufen.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lxf.jinqigfzy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://evb.sysykeji.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://agn.xuetiantiany.cn

[F03] 写入文件（覆盖）
来源：http://paf.jinqigfzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mcr.jinghuilouyu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rlp.zhongyouzk.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wkq.hfpthk.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qvg.316326.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://egj.xuanzx.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kbp.cheryme.top

Ruby: File.write("a.txt", "hi")
来源：http://ngk.shangyingyoupin.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tkz.snrcjt.cn

[F04] 追加写入文件
来源：http://jln.316326.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://aki.shanyushiyangkeji.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://oxe.chenlongwang.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iom.yongpay.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sxb.chenjidiqi.icu

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mix.mhx1999.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jax.xingfuxueyuan.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jxh.daria6918.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mbc.tian-w.cn

[F05] 判断文件或目录是否存在
来源：http://fwa.hcnkem.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://foo.vqdsnc.cn

PHP:  file_exists("a.txt");
来源：http://cqi.zhongyouzk.top

JS:   fs.existsSync("a.txt")
来源：http://sqw.vqdsnc.cn

TS:   fs.existsSync("a.txt")
来源：http://ayn.hysaishi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wsa.haohaochexian.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mqd.ppjwa.cn

Ruby: File.exist?("a.txt")
来源：http://fbf.xylfe.cn

C#:   File.Exists("a.txt")
来源：http://chx.jyoumei.cn

[F06] 删除文件
来源：http://eqs.uphjek.com

Py:   os.remove("a.txt")
来源：http://pll.zhixingplan.top

PHP:  unlink("a.txt");
来源：http://teh.zhengqikj.top

JS:   fs.unlinkSync("a.txt")
来源：http://yur.fengsongda.top

TS:   fs.unlinkSync("a.txt")
来源：http://mqv.chenlongwang.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fis.zhaomingkeji.xyz

Go:   os.Remove("a.txt")
来源：http://oau.aizwys.cn


<!-- 参考信息 -->