代发 wailian999

[D23] reduce 累积计算
来源：http://jbu.ivvv.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hxo.cheryme.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://msc.yanxiufei.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hbr.hnqzz.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ksh.fktsv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dgw.tianlin.xyz

Go:   // 手写循环
来源：http://wyh.bbcook.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bqg.shanyushiyangtech.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xbm.ydzc1.top

[D24] 字典 / Map 基本操作
来源：http://ocm.9152youxi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qdi.daxiang520.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bgc.aibaodan.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kbu.ydzc1.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://szb.gzhubu.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rwt.jqgufenzy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fwr.ydjk.org.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pdt.dianchejie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hdb.yuxming.cn

[D25] Set 集合去重与交并差
来源：http://ivn.birdmap.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vwc.ydjk.org.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jep.yuxming.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ean.hammf.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rlp.andypj.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vjw.hywenlv.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://opq.shzxlz.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://omf.sxryk.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pde.fanxiaobao.xyz

[D26] 数组转字符串
来源：http://awr.meibo888.top

Py:   ", ".join(map(str, arr))
来源：http://dvn.jinghuilouyu.cn

PHP:  implode(", ", $arr);
来源：http://gvd.sysykeji.top

JS:   arr.join(", ")
来源：http://fuk.shuidangran.top

TS:   arr.join(", ")
来源：http://unk.hnqzz.top

Java: String.join(", ", list)
来源：http://tpn.fehbvm.com

Go:   strings.Join(strs, ", ")
来源：http://pvj.gotoacloud.top

Ruby: arr.join(", ")
来源：http://kkj.zdbjq.cn

C#:   string.Join(", ", list)
来源：http://naw.ydjk.org.cn

================================================================================
来源：http://wkg.0kj1m.cn

E. 字符串处理
来源：http://mmx.shanyushiyangtech.top

================================================================================
来源：http://jzo.xuetiantiany.cn

[E01] 拼接字符串
来源：http://wsz.andypj.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ojr.tarul.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uoj.sjlbkw.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fwp.meibo888.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hvr.wangshuangyany.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rpa.smart0.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://upv.sysykeji.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://suc.birdmap.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vbn.quarkkingdee.top

[E02] 重复字符串
来源：http://ueb.jlsjyb.cn

Py:   "ab" * 3
来源：http://amy.hywenlv.cn

PHP:  str_repeat("ab", 3);
来源：http://cfy.jinqigfzy.top

JS:   "ab".repeat(3)
来源：http://ext.xziqi.cn

TS:   "ab".repeat(3)
来源：http://anp.gaohongyu789.top

Java: "ab".repeat(3)
来源：http://sam.shuidangran.top

Go:   strings.Repeat("ab", 3)
来源：http://pun.vqdsnc.cn

Ruby: "ab" * 3
来源：http://mke.tarul.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gcq.zycfv.cn

[E03] 截取子串
来源：http://qii.aibaodan.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://adu.zhijiandao.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tje.cheryme.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dga.jinghuilouyu.cn

TS:   s.slice(1, 4)
来源：http://vyh.xziqi.cn

Java: s.substring(1, 4)
来源：http://wdf.cucudq.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://keo.yfazqb.com

Ruby: s[1, 3];  s[1..3]
来源：http://bhs.dianchejie.cn

C#:   s.Substring(1, 3)
来源：http://txp.meibo888.top

[E04] 查找子串位置
来源：http://dec.shangyingyoupin.top

Py:   s.find("x");  s.index("x")
来源：http://amk.jiagoushi.top

PHP:  strpos($s, "x");
来源：http://cxi.shuidangran.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://uyd.yvedp.cn

TS:   s.indexOf("x")
来源：http://ozn.mhx1999.top

Java: s.indexOf("x")
来源：http://jon.gotoacloud.top

Go:   strings.Index(s, "x")
来源：http://yke.hnqzz.top

Ruby: s.index("x")
来源：http://rbu.yongpay.top

C#:   s.IndexOf("x")
来源：http://waq.ywan-chungtsiang.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://zkh.xingfuxueyuan.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mfc.jianghu66.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kpn.nwbrower.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xxx.yonumen.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://nqf.chenzaomai.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zgw.hysaishi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jto.zhixingplan.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pzn.shanyushiyangtech.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ysi.andypj.xyz

[E06] 替换子串
来源：http://stu.ybcxt.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://juh.jinghuilouyu.cn

PHP:  str_replace("a", "b", $s);
来源：http://qaf.dianchejie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wrq.zhijiandao.cn

TS:   s.replaceAll("a", "b")
来源：http://aaq.gaohongyu789.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tqu.jlsjyb.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://suj.xziqi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://aew.shanyushiyangtech.top

C#:   s.Replace("a", "b")
来源：http://rns.jianghu66.top

[E07] 按分隔符拆分
来源：http://rxw.nanxuanxn.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://eld.zhoulong.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wyu.zycfv.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://mwu.epnwcf.com

TS:   s.split(",")
来源：http://xbm.yanxiufei.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sjz.redwolf501.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wsq.yonumen.top

Ruby: s.split(",");  s.split
来源：http://dfu.zhiwuduotai.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://byj.hcnkem.com

[E08] 数组按分隔符合并
来源：http://ywd.sxryk.cn

Py:   ",".join(items)
来源：http://frb.zhijiandao.cn

PHP:  implode(",", $items);
来源：http://uvm.daria6918.cn

JS:   items.join(",")
来源：http://fik.meibo888.top

TS:   items.join(",")
来源：http://rwh.nanxinkj.top

Java: String.join(",", items)
来源：http://zlq.c1oappe.top

Go:   strings.Join(items, ",")
来源：http://frj.nanxuanxn.top

Ruby: items.join(",")
来源：http://iab.andypj.xyz

C#:   string.Join(",", items)
来源：http://jbg.iojbl.cn

[E09] 去除所有空白字符
来源：http://lib.yvedp.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xqy.yj20258888.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pcx.yj20258888.top

JS:   s.replace(/\s+/g, "")
来源：http://wli.jinyuanbaomall.cn

TS:   s.replace(/\s+/g, "")
来源：http://iin.fzhhl.top

Java: s.replaceAll("\\s+", "")
来源：http://ddw.yonumen.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://aub.mhx1999.top

Ruby: s.gsub(/\s+/, "")
来源：http://sfs.yuxming.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://owa.xuanzx.com

[E10] 左侧补零 / 定长填充
来源：http://ezr.gzhubu.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bmc.dashuyun.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://okl.meibo888.top

JS:   "7".padStart(3, "0")
来源：http://uei.bjfxy.top

TS:   "7".padStart(3, "0")
来源：http://wry.yanxiufei.cn

Java: String.format("%03d", 7)
来源：http://sud.zdqjudy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://bbk.c1oappe.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hkz.yanxiufei.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://oyi.tianlin.xyz

[E11] 反转字符串
来源：http://iei.zhiwuduotai.top

Py:   s[::-1]
来源：http://ymh.zhoulong.xyz

PHP:  strrev($s);
来源：http://rbh.cashguo.top

JS:   [...s].reverse().join("")
来源：http://rff.hcnkem.com

TS:   [...s].reverse().join("")
来源：http://ctx.shanyushiyangtech.top

Java: new StringBuilder(s).reverse().toString()
来源：http://owa.wangshuangyany.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qph.hammf.cn

Ruby: s.reverse
来源：http://jwp.tianlin.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://duj.jyoumei.cn

[E12] 统计某字符出现次数
来源：http://jrq.guowangkeji.top

Py:   s.count("a")
来源：http://cqq.tanke756.top

PHP:  substr_count($s, "a");
来源：http://zaq.sjlbkw.cn

JS:   s.split("a").length - 1
来源：http://qbr.mhx1999.top

TS:   s.split("a").length - 1
来源：http://znd.gotoacloud.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://sia.vehdjk.com

Go:   strings.Count(s, "a")
来源：http://mzf.zhixingplan.top

Ruby: s.count("a")
来源：http://gcg.quarkkingdee.top

C#:   s.Count(c => c == 'a')
来源：http://zdh.c1oappe.top

[E13] 逐字符遍历
来源：http://kps.epnwcf.com

Py:   for ch in s: print(ch)
来源：http://cat.xuetiantiany.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://onb.jqgfzy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://kxb.daria6918.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vlx.hnxiangtu.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mis.jinghuilouyu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://exz.vqdsnc.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lgc.bjfxy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yuj.jqgfzy.top

[E14] URL 编码与 Base64
来源：http://gsl.shuidangran.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qbp.sweek.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://clo.sxryk.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gqd.fehbvm.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hnl.jlsjyb.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lwu.jyoumei.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xvt.yj20258.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lhz.xziqi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jtg.ppjwa.cn

[E15] HTML 转义 / 反转义
来源：http://rdz.hnxiangtu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://fwk.tarul.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nqc.dianchejie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gmi.xziqi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://euz.xziqi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cio.hongshengwenyu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mtk.sxryk.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yuf.c1oappe.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bbw.c1oappe.top

[E16] 数字千分位
来源：http://tvn.kuanghao11.cn

Py:   f"{1234567:,}"
来源：http://vdo.yongpay.top

PHP:  number_format(1234567);
来源：http://tld.kuanghao11.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://amj.zhongyouzk.top

TS:   (1234567).toLocaleString("en-US")
来源：http://hxq.kuanghao11.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ccd.jqgfzy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vtd.sufxvd.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mga.jiagoushi.top

C#:   1234567.ToString("N0")
来源：http://lde.shanyushiyangkeji.top

[E17] 首字母大写
来源：http://dbf.havefunace.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wtd.kuanghao11.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://daa.yj20258.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qxb.daria6918.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jwg.jinyuanbaomall.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ofn.xuetiantiany.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gjw.vqdsnc.cn

Ruby: s.capitalize
来源：http://nqj.yj20258888.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ckg.yonumen.top

[E18] 模板占位符替换
来源：http://jqu.tarul.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nhq.snrcjt.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fic.bbcook.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jbi.xuetiantiany.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://mmm.meibo888.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yks.aizwys.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fgg.yj202588.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sul.gotoacloud.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://usj.ivvv.top

[E19] 多行文本按行拆分
来源：http://uiz.yanxiufei.cn

Py:   s.splitlines()
来源：http://gac.fanxiaobao.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zhk.cheryme.top

JS:   s.split(/\r?\n/)
来源：http://ppl.jinqigfzy.top

TS:   s.split(/\r?\n/)
来源：http://gvw.bjfxy.top

Java: s.lines().toList()
来源：http://ubi.redwolf501.top

Go:   strings.Split(s, "\n")
来源：http://jsv.andypj.xyz

Ruby: s.lines
来源：http://pel.yanxiufei.cn

C#:   s.Split('\n')
来源：http://xrh.zhixingplan.top

[E20] 判断字符串是否为空
来源：http://epf.yuanzhike.top

Py:   if not s:
来源：http://tlt.jyoumei.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bje.vehdjk.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ipz.hongshengwenyu.top

TS:   if (s === "") {}
来源：http://vhi.chenlongwang.top

Java: if (s.isEmpty()) {}
来源：http://jdk.cqqwz.cn

Go:   if s == "" {}
来源：http://gol.aibaodan.cn

Ruby: if s.empty?
来源：http://rbl.jinyuanbaomall.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kqf.uphjek.com

[E21] 超长截断加省略号
来源：http://vws.tarul.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sxz.havefunace.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hkm.jqgfzy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wyk.xziqi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ggv.yangfankeji.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rsm.ydzc1.top

Go:   // 按 rune 判断长度后截断
来源：http://eev.aizwys.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wex.hnxiangtu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tao.chenzaomai.com

[E22] 字节长度与字符长度
来源：http://ctf.ywan-chungtsiang.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hsk.wangshuangyany.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tem.havefunace.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://law.nwbrower.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://oux.jianghu66.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://paw.cashguo.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hig.tianlin.xyz

Ruby: s.bytesize;  s.length
来源：http://rom.chenlongwang.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qdu.pycfn.com

================================================================================
来源：http://fvg.hongshengwenyu.top

F. 文件与目录
来源：http://ikw.hfpthk.cn

================================================================================
来源：http://fnl.yongpay.top

[F01] 读取整个文件
来源：http://iuk.0kj1m.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pdb.vqdsnc.cn

PHP:  file_get_contents("a.txt");
来源：http://hzi.uphjek.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qmc.jlsjyb.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://boi.fanxiaobao.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://awg.ybcxt.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bzh.aizwys.cn

Ruby: File.read("a.txt")
来源：http://bzp.hnxiangtu.top

C#:   File.ReadAllText("a.txt");
来源：http://vns.sufxvd.cn

[F02] 逐行读取文件
来源：http://dva.svipenyu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hxp.zhengqikj.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://akh.zdbjq.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://faf.shanyushiyangtech.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eey.jianghu66.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pyz.gogol.net.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ayw.gogol.net.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vml.jyoumei.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ycm.yj202588.top

[F03] 写入文件（覆盖）
来源：http://dks.daria6918.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bls.fanxiaobao.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://ycv.aibaodan.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kxh.xuanzx.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yzt.ehwqpu.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rqt.yanxiufei.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://clh.xinyue.icu

Ruby: File.write("a.txt", "hi")
来源：http://wfz.yj20258.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://apt.gaohongyu789.top

[F04] 追加写入文件
来源：http://qrx.316326.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://har.wangshuangyany.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wtq.hammf.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bab.zhoulong.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ilj.ybcxt.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uom.hongshengwenyu.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yvg.epnwcf.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ona.tarul.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kpb.ydzc1.top

[F05] 判断文件或目录是否存在
来源：http://qnp.kuanghao11.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://htp.jqgufenzy.top

PHP:  file_exists("a.txt");
来源：http://tgf.shuidangran.top

JS:   fs.existsSync("a.txt")
来源：http://nga.bbcook.cn

TS:   fs.existsSync("a.txt")
来源：http://roc.zhaomingkeji.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://sqd.jinyuanbaomall.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qca.svipenyu.cn

Ruby: File.exist?("a.txt")
来源：http://fmo.zhijiandao.cn

C#:   File.Exists("a.txt")
来源：http://xjr.tianlin.xyz

[F06] 删除文件
来源：http://wxz.hysaishi.cn

Py:   os.remove("a.txt")
来源：http://oxw.sweek.top

PHP:  unlink("a.txt");
来源：http://ccp.gzhubu.top

JS:   fs.unlinkSync("a.txt")
来源：http://oeh.iojbl.cn

TS:   fs.unlinkSync("a.txt")
来源：http://slw.hammf.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ler.ydjk.org.cn

Go:   os.Remove("a.txt")
来源：http://nuo.zhaomingkeji.xyz

Ruby: File.delete("a.txt")
来源：http://pxp.vehdjk.com

C#:   File.Delete("a.txt");
来源：http://ntn.jqgufenzy.top

[F07] 创建目录（含多级）
来源：http://qtj.ydjk.org.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://aar.xylfe.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://msh.haohaochexian.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hkq.cqqwz.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dcr.zhijiandao.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gpz.wangdashe.top


<!-- 参考信息 -->