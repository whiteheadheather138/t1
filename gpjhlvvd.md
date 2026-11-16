代发 wailian999

Java: new ArrayList<>(list);
来源：http://lmx.yvedp.cn

Go:   copied := append([]int(nil), arr...)
来源：http://luc.zdqjudy.top

Ruby: arr.dup;  arr.clone
来源：http://zzv.zhengqikj.top

C#:   new List<int>(list);
来源：http://qun.cucudq.cn

[D23] reduce 累积计算
来源：http://ewk.zhijiandao.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vkc.havefunace.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ikv.tianlin.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dkd.jianghu66.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gah.vehdjk.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://wtz.shuidangran.top

Go:   // 手写循环
来源：http://mrl.xuanzx.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://clh.yonumen.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xgr.snrcjt.cn

[D24] 字典 / Map 基本操作
来源：http://vto.jinqigfzy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bsy.haohaochexian.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bxt.ybcxt.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zwj.cashguo.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://enj.fengsongda.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uyh.ppjwa.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ici.vqdsnc.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rcx.haohaochexian.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zow.wangdashe.top

[D25] Set 集合去重与交并差
来源：http://adl.zhixingplan.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gxh.redwolf501.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://iqu.vehdjk.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bsc.ppjwa.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tlp.yanxiufei.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kns.xuanzx.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kmr.fanxiaobao.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lic.cdnleiting.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ksv.tian-w.cn

[D26] 数组转字符串
来源：http://dpn.xziqi.cn

Py:   ", ".join(map(str, arr))
来源：http://ofp.zdbjq.cn

PHP:  implode(", ", $arr);
来源：http://qtl.zhijiandao.cn

JS:   arr.join(", ")
来源：http://cnh.fzhhl.top

TS:   arr.join(", ")
来源：http://obr.dianchejie.cn

Java: String.join(", ", list)
来源：http://wzv.xuetiantiany.cn

Go:   strings.Join(strs, ", ")
来源：http://zqd.ppjwa.cn

Ruby: arr.join(", ")
来源：http://fop.vqdsnc.cn

C#:   string.Join(", ", list)
来源：http://vbm.nanxuanxn.top

================================================================================
来源：http://orq.shanyushiyangkeji.top

E. 字符串处理
来源：http://zwg.wangdashe.top

================================================================================
来源：http://lwl.fktsv.cn

[E01] 拼接字符串
来源：http://jur.hesvh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zpt.316326.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kyv.aizwys.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yeq.jinqigufen.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bvn.fanxiaobao.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nyw.sysykeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ian.jqgufenzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://urd.0kj1m.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ypi.xuetiantiany.cn

[E02] 重复字符串
来源：http://uhr.fehbvm.com

Py:   "ab" * 3
来源：http://qzw.gogol.net.cn

PHP:  str_repeat("ab", 3);
来源：http://wpf.ivvv.top

JS:   "ab".repeat(3)
来源：http://rxl.yj20258.top

TS:   "ab".repeat(3)
来源：http://pft.c1oappe.top

Java: "ab".repeat(3)
来源：http://aay.jyoumei.cn

Go:   strings.Repeat("ab", 3)
来源：http://qvy.jiagoushi.top

Ruby: "ab" * 3
来源：http://xlk.hysaishi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xsx.sysykeji.top

[E03] 截取子串
来源：http://ntg.daria6918.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fwi.ivvv.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wrj.epnwcf.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jug.smart0.xyz

TS:   s.slice(1, 4)
来源：http://qpm.uphjek.com

Java: s.substring(1, 4)
来源：http://nqx.bjfxy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pmz.yfazqb.com

Ruby: s[1, 3];  s[1..3]
来源：http://uvf.xinyue.icu

C#:   s.Substring(1, 3)
来源：http://yoe.xingfuxueyuan.xyz

[E04] 查找子串位置
来源：http://ucd.sweek.top

Py:   s.find("x");  s.index("x")
来源：http://gzy.gaohongyu789.top

PHP:  strpos($s, "x");
来源：http://nyx.yangfankeji.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gvj.ivvv.top

TS:   s.indexOf("x")
来源：http://ziv.jqgufenzy.top

Java: s.indexOf("x")
来源：http://iyn.xuanzx.com

Go:   strings.Index(s, "x")
来源：http://uic.jqgufenzy.top

Ruby: s.index("x")
来源：http://rhp.jqgufenzy.top

C#:   s.IndexOf("x")
来源：http://soz.ywan-chungtsiang.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://nnt.ywan-chungtsiang.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bdl.pengpengdd.cyou

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://iwk.shzxlz.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hzv.0kj1m.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://rkh.gaohongyu789.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xnw.ydzc1.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rpu.fengsongda.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tti.tian-w.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wib.0kj1m.cn

[E06] 替换子串
来源：http://hzu.yonumen.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fwi.shzxlz.cn

PHP:  str_replace("a", "b", $s);
来源：http://clb.shanyushiyangkeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pme.aizwys.cn

TS:   s.replaceAll("a", "b")
来源：http://xmf.kuanghao11.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ofy.tian-w.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ibw.aibaodan.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vxs.ywan-chungtsiang.top

C#:   s.Replace("a", "b")
来源：http://azy.meibo888.top

[E07] 按分隔符拆分
来源：http://qje.ybcxt.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yzp.316326.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ivw.316326.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://dre.vehdjk.com

TS:   s.split(",")
来源：http://rbs.xuanzx.com

Java: s.split(",");  s.split("\\s+")
来源：http://cmh.c1oappe.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jmu.ctjpmb.com

Ruby: s.split(",");  s.split
来源：http://bqv.shuidangran.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wdu.zhaomingkeji.xyz

[E08] 数组按分隔符合并
来源：http://fel.gogol.net.cn

Py:   ",".join(items)
来源：http://bmw.smart0.xyz

PHP:  implode(",", $items);
来源：http://vgn.mhx1999.top

JS:   items.join(",")
来源：http://tpt.gzhubu.top

TS:   items.join(",")
来源：http://ejl.vehdjk.com

Java: String.join(",", items)
来源：http://emy.yonumen.top

Go:   strings.Join(items, ",")
来源：http://bfy.chenzaomai.com

Ruby: items.join(",")
来源：http://fds.hesvh.cn

C#:   string.Join(",", items)
来源：http://jpf.jiagoushi.top

[E09] 去除所有空白字符
来源：http://jdp.vqdsnc.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://euh.wangshuangyany.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://flq.ppjwa.cn

JS:   s.replace(/\s+/g, "")
来源：http://xba.fanxiaobao.xyz

TS:   s.replace(/\s+/g, "")
来源：http://inw.hywenlv.cn

Java: s.replaceAll("\\s+", "")
来源：http://hti.jinyuanbaomall.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mna.ivvv.top

Ruby: s.gsub(/\s+/, "")
来源：http://djj.vqdsnc.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://shl.sweek.top

[E10] 左侧补零 / 定长填充
来源：http://kbh.shuidangran.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://uwm.ydjk.org.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kzw.hfpthk.cn

JS:   "7".padStart(3, "0")
来源：http://eoh.iojbl.cn

TS:   "7".padStart(3, "0")
来源：http://ibp.jqgufenzy.top

Java: String.format("%03d", 7)
来源：http://lmv.chenzaomai.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://egn.yj20258888.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fkz.tian-w.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tpf.ydzc1.top

[E11] 反转字符串
来源：http://oha.zhaomingkeji.xyz

Py:   s[::-1]
来源：http://iwc.cucudq.cn

PHP:  strrev($s);
来源：http://jwt.uphjek.com

JS:   [...s].reverse().join("")
来源：http://rcw.fktsv.cn

TS:   [...s].reverse().join("")
来源：http://wqd.shanyushiyangtech.top

Java: new StringBuilder(s).reverse().toString()
来源：http://nfj.xylfe.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://dpf.nwbrower.top

Ruby: s.reverse
来源：http://hgs.hnqzz.top

C#:   new string(s.Reverse().ToArray())
来源：http://xwj.tian-w.cn

[E12] 统计某字符出现次数
来源：http://gpc.fzhhl.top

Py:   s.count("a")
来源：http://hdr.fengsongda.top

PHP:  substr_count($s, "a");
来源：http://gzd.c1oappe.top

JS:   s.split("a").length - 1
来源：http://jjj.jyoumei.cn

TS:   s.split("a").length - 1
来源：http://seb.nanxuanxn.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bif.hammf.cn

Go:   strings.Count(s, "a")
来源：http://dtd.fehbvm.com

Ruby: s.count("a")
来源：http://tff.yuanzhike.top

C#:   s.Count(c => c == 'a')
来源：http://znd.zhongyouzk.top

[E13] 逐字符遍历
来源：http://zri.ctjpmb.com

Py:   for ch in s: print(ch)
来源：http://bch.guowangkeji.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rkk.yueranfly.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://sgm.xuetiantiany.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://owm.birdmap.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://viu.ehwqpu.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://syp.zhiwuduotai.top

Ruby: s.each_char { |ch| puts ch }
来源：http://fze.hammf.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ucs.yj20258888.top

[E14] URL 编码与 Base64
来源：http://epu.ydjk.org.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://iho.zhiwuduotai.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://uhl.pycfn.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ebh.quarkkingdee.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kbl.sysykeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wgf.zhixingplan.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://drr.feifeiyinyue.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fdo.gotoacloud.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nsx.guowangkeji.top

[E15] HTML 转义 / 反转义
来源：http://nwf.xuanzx.com

Py:   html.escape(s);  html.unescape(s)
来源：http://vzn.hcnkem.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vor.dashuyun.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yfn.jyoumei.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zew.tanke756.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pme.tianlin.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kna.yj202588.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hco.yj20258888.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jdz.feifeiyinyue.top

[E16] 数字千分位
来源：http://uoc.smart0.xyz

Py:   f"{1234567:,}"
来源：http://phu.zycfv.cn

PHP:  number_format(1234567);
来源：http://asu.vqdsnc.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xgh.hnqzz.top

TS:   (1234567).toLocaleString("en-US")
来源：http://btj.cdnleiting.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lei.yangfankeji.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://trh.aibaodan.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kco.bjfxy.top

C#:   1234567.ToString("N0")
来源：http://bzv.jinqigufen.top

[E17] 首字母大写
来源：http://zga.pengpengdd.cyou

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fgi.wangshuangyany.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jjp.cqqwz.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dtg.ydzc1.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rmz.shanyushiyangtech.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://znt.chenjidiqi.icu

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fgd.ctjpmb.com

Ruby: s.capitalize
来源：http://ivm.guowangkeji.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ijb.hongshengwenyu.top

[E18] 模板占位符替换
来源：http://apc.shzxlz.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zvg.yonumen.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ewj.vehdjk.com

JS:   tpl.replaceAll("{name}", name)
来源：http://pbp.sjlbkw.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://znq.0kj1m.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://teh.cucudq.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fov.zhaomingkeji.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hyd.jyoumei.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vfp.birdmap.top

[E19] 多行文本按行拆分
来源：http://zjo.ehwqpu.com

Py:   s.splitlines()
来源：http://gos.iojbl.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://aey.yanxiufei.cn

JS:   s.split(/\r?\n/)
来源：http://ncu.hammf.cn

TS:   s.split(/\r?\n/)
来源：http://cey.daria6918.cn

Java: s.lines().toList()
来源：http://rsd.nwbrower.top

Go:   strings.Split(s, "\n")
来源：http://ckr.jinqigufen.top

Ruby: s.lines
来源：http://sog.sweek.top

C#:   s.Split('\n')
来源：http://aif.hysaishi.cn

[E20] 判断字符串是否为空
来源：http://off.feifeiyinyue.top

Py:   if not s:
来源：http://tho.gogol.net.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wul.tanke756.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ayx.316326.xyz

TS:   if (s === "") {}
来源：http://hpl.chenjidiqi.icu

Java: if (s.isEmpty()) {}
来源：http://ild.vehdjk.com

Go:   if s == "" {}
来源：http://llm.jyoumei.cn

Ruby: if s.empty?
来源：http://mqq.mhx1999.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://brz.hnxiangtu.top

[E21] 超长截断加省略号
来源：http://mtm.hfpthk.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yvy.wangdashe.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qxy.nanxuanxn.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rpv.chenjidiqi.icu

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wwt.zdbjq.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lqg.hywenlv.cn

Go:   // 按 rune 判断长度后截断
来源：http://auu.nanxinkj.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mgd.hysaishi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://scp.yj20258888.top

[E22] 字节长度与字符长度
来源：http://zxp.ywan-chungtsiang.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bgn.zhoulong.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dfs.gaohongyu789.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jyp.yvedp.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cpf.ctjpmb.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nnt.hysaishi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fua.ydjk.org.cn

Ruby: s.bytesize;  s.length
来源：http://psa.smart0.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kzz.svipenyu.cn

================================================================================
来源：http://wzl.cashguo.top

F. 文件与目录
来源：http://xns.jyoumei.cn

================================================================================
来源：http://ghb.jinghuilouyu.cn

[F01] 读取整个文件
来源：http://xet.yuxming.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wpl.yuanzhike.top

PHP:  file_get_contents("a.txt");
来源：http://rju.yuanzhike.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wzr.gaohongyu789.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rou.chenjidiqi.icu

Java: Files.readString(Path.of("a.txt"))
来源：http://gah.ywan-chungtsiang.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ijh.hcnkem.com

Ruby: File.read("a.txt")
来源：http://mul.jiagoushi.top

C#:   File.ReadAllText("a.txt");
来源：http://fqu.yueranfly.top

[F02] 逐行读取文件
来源：http://jyi.aizwys.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bba.ywan-chungtsiang.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://imf.cdnleiting.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ubh.zhixingplan.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lmf.jqgufenzy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zwr.sjlbkw.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ksk.316326.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://iyf.zhiwuduotai.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uos.guowangkeji.top

[F03] 写入文件（覆盖）
来源：http://oah.jiagoushi.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wiv.havefunace.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://fam.feifeiyinyue.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mhm.zhoulong.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uba.zhiwuduotai.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nwf.bbcook.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ocr.kuanghao11.cn

Ruby: File.write("a.txt", "hi")
来源：http://jlt.jinqigufen.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uwq.jinqigfzy.top

[F04] 追加写入文件
来源：http://uoc.aibaodan.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://riz.shanyushiyangtech.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qsi.tarul.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hzt.ppjwa.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lhx.hfpthk.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cbo.ehwqpu.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cuj.chenzaomai.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wgk.jqgfzy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nwb.ydjk.org.cn

[F05] 判断文件或目录是否存在
来源：http://nmn.zhengqikj.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kcm.nanxuanxn.top

PHP:  file_exists("a.txt");
来源：http://atf.yuxming.cn

JS:   fs.existsSync("a.txt")
来源：http://cxt.fanxiaobao.xyz

TS:   fs.existsSync("a.txt")
来源：http://mbq.bbcook.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://sfs.cashguo.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jyh.yj20258.top

Ruby: File.exist?("a.txt")
来源：http://rwz.yj20258888.top

C#:   File.Exists("a.txt")
来源：http://dkt.shzxlz.cn

[F06] 删除文件
来源：http://fjk.guowangkeji.top

Py:   os.remove("a.txt")
来源：http://aho.andypj.xyz

PHP:  unlink("a.txt");
来源：http://qyb.shanyushiyangtech.top

JS:   fs.unlinkSync("a.txt")
来源：http://kho.mhx1999.top

TS:   fs.unlinkSync("a.txt")
来源：http://ycs.hywenlv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cgp.daria6918.cn

Go:   os.Remove("a.txt")
来源：http://hxj.fanxiaobao.xyz

Ruby: File.delete("a.txt")
来源：http://qpi.daxiang520.top

C#:   File.Delete("a.txt");
来源：http://dgb.mhx1999.top

[F07] 创建目录（含多级）
来源：http://yep.zycfv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nqi.tarul.cn


<!-- 参考信息 -->