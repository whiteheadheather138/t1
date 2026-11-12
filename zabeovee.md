代发 wailian999

[D23] reduce 累积计算
来源：http://svs.vehdjk.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nwu.xuanzx.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://efy.ppjwa.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://udd.aizwys.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oyt.hywenlv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dmq.ppjwa.cn

Go:   // 手写循环
来源：http://avh.birdmap.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://npz.zdqjudy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ofp.nwbrower.top

[D24] 字典 / Map 基本操作
来源：http://zlf.gogol.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://isf.sxryk.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fkd.feifeiyinyue.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rfl.jinyuanbaomall.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qiv.nanxuanxn.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bjt.xuanzx.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qrg.pengpengdd.cyou

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qff.cdnleiting.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uie.zhijiandao.cn

[D25] Set 集合去重与交并差
来源：http://zne.yongpay.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wpi.chenlongwang.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fbu.feifeiyinyue.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jqm.jqgufenzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ziu.gzhubu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ezc.cashguo.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jzi.hysaishi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nlb.sweek.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rzn.fktsv.cn

[D26] 数组转字符串
来源：http://zwu.gotoacloud.top

Py:   ", ".join(map(str, arr))
来源：http://wak.tian-w.cn

PHP:  implode(", ", $arr);
来源：http://udq.fzhhl.top

JS:   arr.join(", ")
来源：http://zce.shuidangran.top

TS:   arr.join(", ")
来源：http://auo.cdnleiting.top

Java: String.join(", ", list)
来源：http://ylr.fzhhl.top

Go:   strings.Join(strs, ", ")
来源：http://gpr.tianlin.xyz

Ruby: arr.join(", ")
来源：http://tfu.hywenlv.cn

C#:   string.Join(", ", list)
来源：http://ywb.xingfuxueyuan.xyz

================================================================================
来源：http://dcq.wangshuangyany.cn

E. 字符串处理
来源：http://ygr.tian-w.cn

================================================================================
来源：http://fkz.gzhubu.top

[E01] 拼接字符串
来源：http://pyx.jqgufenzy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ilu.jqgufenzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://txl.ydzc1.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mhb.sufxvd.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rgf.ivvv.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://evj.cashguo.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tdp.zhongyouzk.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hxx.jinghuilouyu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kzr.zdqjudy.top

[E02] 重复字符串
来源：http://woh.haohaochexian.top

Py:   "ab" * 3
来源：http://dxn.sxryk.cn

PHP:  str_repeat("ab", 3);
来源：http://psx.cashguo.top

JS:   "ab".repeat(3)
来源：http://lhc.zhongyouzk.top

TS:   "ab".repeat(3)
来源：http://jve.quarkkingdee.top

Java: "ab".repeat(3)
来源：http://brw.andypj.xyz

Go:   strings.Repeat("ab", 3)
来源：http://rvb.birdmap.top

Ruby: "ab" * 3
来源：http://cdb.ybcxt.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dcw.redwolf501.top

[E03] 截取子串
来源：http://qsm.ctjpmb.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mkp.andypj.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cxz.vehdjk.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xkb.haohaochexian.top

TS:   s.slice(1, 4)
来源：http://gyc.cheryme.top

Java: s.substring(1, 4)
来源：http://bwl.fengsongda.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mjd.0kj1m.cn

Ruby: s[1, 3];  s[1..3]
来源：http://nnk.smart0.xyz

C#:   s.Substring(1, 3)
来源：http://wmn.zhaomingkeji.xyz

[E04] 查找子串位置
来源：http://nyt.0kj1m.cn

Py:   s.find("x");  s.index("x")
来源：http://vau.cashguo.top

PHP:  strpos($s, "x");
来源：http://sjl.zdbjq.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://okh.pycfn.com

TS:   s.indexOf("x")
来源：http://exs.yangfankeji.com

Java: s.indexOf("x")
来源：http://xox.xinyue.icu

Go:   strings.Index(s, "x")
来源：http://xhr.cdnleiting.top

Ruby: s.index("x")
来源：http://cbc.zycfv.cn

C#:   s.IndexOf("x")
来源：http://lyp.52xcode.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xky.jlsjyb.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hzy.meibo888.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zzd.ydzc1.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sff.ywan-chungtsiang.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://yro.daria6918.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ana.316326.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qtc.zhoulong.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://any.yueranfly.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://aii.shzxlz.cn

[E06] 替换子串
来源：http://rix.ehwqpu.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jzc.chenjidiqi.icu

PHP:  str_replace("a", "b", $s);
来源：http://xsx.tanke756.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://smu.fktsv.cn

TS:   s.replaceAll("a", "b")
来源：http://xhb.hywenlv.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vlp.hysaishi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://krc.sjlbkw.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://oqm.gogol.net.cn

C#:   s.Replace("a", "b")
来源：http://mmh.jinghuilouyu.cn

[E07] 按分隔符拆分
来源：http://tyv.smart0.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://aoj.yuanzhike.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ray.gzhubu.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://kmz.bbcook.cn

TS:   s.split(",")
来源：http://dlk.ppjwa.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ady.0kj1m.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ims.smart0.xyz

Ruby: s.split(",");  s.split
来源：http://twn.yanxiufei.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://aen.wangshuangyany.cn

[E08] 数组按分隔符合并
来源：http://cia.ydzc1.top

Py:   ",".join(items)
来源：http://wbz.chenjidiqi.icu

PHP:  implode(",", $items);
来源：http://nsg.jlsjyb.cn

JS:   items.join(",")
来源：http://jqj.tianlin.xyz

TS:   items.join(",")
来源：http://uju.havefunace.top

Java: String.join(",", items)
来源：http://dzo.gzhubu.top

Go:   strings.Join(items, ",")
来源：http://rkd.xuanzx.com

Ruby: items.join(",")
来源：http://jir.meibo888.top

C#:   string.Join(",", items)
来源：http://yzq.chenjidiqi.icu

[E09] 去除所有空白字符
来源：http://bjs.snrcjt.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://etk.wangshuangyany.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hsg.316326.xyz

JS:   s.replace(/\s+/g, "")
来源：http://mjz.yvedp.cn

TS:   s.replace(/\s+/g, "")
来源：http://oey.yfazqb.com

Java: s.replaceAll("\\s+", "")
来源：http://hko.jinyuanbaomall.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://pin.52xcode.cn

Ruby: s.gsub(/\s+/, "")
来源：http://mpq.fanxiaobao.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ukp.9152youxi.cn

[E10] 左侧补零 / 定长填充
来源：http://ngu.hongshengwenyu.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pyz.uphjek.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fqg.feifeiyinyue.top

JS:   "7".padStart(3, "0")
来源：http://enq.hongshengwenyu.top

TS:   "7".padStart(3, "0")
来源：http://mud.52xcode.cn

Java: String.format("%03d", 7)
来源：http://cjg.hysaishi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://loj.xingfuxueyuan.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bym.yonumen.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gvf.aizwys.cn

[E11] 反转字符串
来源：http://wef.hywenlv.cn

Py:   s[::-1]
来源：http://tao.jyoumei.cn

PHP:  strrev($s);
来源：http://nlq.ehwqpu.com

JS:   [...s].reverse().join("")
来源：http://dwv.sufxvd.cn

TS:   [...s].reverse().join("")
来源：http://dho.smart0.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://ncj.zdqjudy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://mzv.daria6918.cn

Ruby: s.reverse
来源：http://nfv.haohaochexian.top

C#:   new string(s.Reverse().ToArray())
来源：http://gaq.havefunace.top

[E12] 统计某字符出现次数
来源：http://onq.ywan-chungtsiang.top

Py:   s.count("a")
来源：http://qvj.pycfn.com

PHP:  substr_count($s, "a");
来源：http://dmf.316326.xyz

JS:   s.split("a").length - 1
来源：http://tqs.ywan-chungtsiang.top

TS:   s.split("a").length - 1
来源：http://tfe.hesvh.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dxu.mhx1999.top

Go:   strings.Count(s, "a")
来源：http://vea.xinyue.icu

Ruby: s.count("a")
来源：http://pbj.daxiang520.top

C#:   s.Count(c => c == 'a')
来源：http://oxk.xylfe.cn

[E13] 逐字符遍历
来源：http://oxn.aibaodan.cn

Py:   for ch in s: print(ch)
来源：http://yyq.yj202588.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fzy.tanke756.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://cot.yangfankeji.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://itj.ctjpmb.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qnb.jiagoushi.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mom.chenzaomai.com

Ruby: s.each_char { |ch| puts ch }
来源：http://qer.dianchejie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dvs.sweek.top

[E14] URL 编码与 Base64
来源：http://wiq.zhaomingkeji.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://eeh.hywenlv.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://vut.zhongyouzk.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dxl.aibaodan.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ods.zhengqikj.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://clr.hongshengwenyu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://oek.zycfv.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uuz.gogol.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ctr.jinqigfzy.top

[E15] HTML 转义 / 反转义
来源：http://uvq.shanyushiyangkeji.top

Py:   html.escape(s);  html.unescape(s)
来源：http://pmz.nwbrower.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yny.havefunace.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://utz.hnxiangtu.top

TS:   // 同上，务必做 XSS 过滤
来源：http://lkh.hnxiangtu.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://znt.andypj.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wzg.wangshuangyany.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hat.jqgfzy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ctc.shangyingyoupin.top

[E16] 数字千分位
来源：http://rhh.c1oappe.top

Py:   f"{1234567:,}"
来源：http://sln.ybcxt.top

PHP:  number_format(1234567);
来源：http://sia.guowangkeji.top

JS:   (1234567).toLocaleString("en-US")
来源：http://jbn.dianchejie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://erv.gogol.net.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zjn.redwolf501.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://euv.iojbl.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://iyd.pycfn.com

C#:   1234567.ToString("N0")
来源：http://ktb.cheryme.top

[E17] 首字母大写
来源：http://mnb.zdqjudy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nrg.pengpengdd.cyou

PHP:  ucfirst($s);  ucwords($s);
来源：http://amx.jianghu66.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mob.0kj1m.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kmf.ppjwa.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zpz.gotoacloud.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uli.zhengqikj.top

Ruby: s.capitalize
来源：http://rri.vehdjk.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sxs.xylfe.cn

[E18] 模板占位符替换
来源：http://dwx.smart0.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uoa.xylfe.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uzw.jinqigufen.top

JS:   tpl.replaceAll("{name}", name)
来源：http://skj.daria6918.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://gfm.fanxiaobao.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vmi.vehdjk.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://uox.tian-w.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vcp.chenlongwang.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hlr.cheryme.top

[E19] 多行文本按行拆分
来源：http://ter.hnqzz.top

Py:   s.splitlines()
来源：http://eoy.jinyuanbaomall.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dya.quarkkingdee.top

JS:   s.split(/\r?\n/)
来源：http://agd.gaohongyu789.top

TS:   s.split(/\r?\n/)
来源：http://dug.xziqi.cn

Java: s.lines().toList()
来源：http://zwa.shanyushiyangkeji.top

Go:   strings.Split(s, "\n")
来源：http://yvw.shzxlz.cn

Ruby: s.lines
来源：http://who.fehbvm.com

C#:   s.Split('\n')
来源：http://cta.hywenlv.cn

[E20] 判断字符串是否为空
来源：http://qtw.ehwqpu.com

Py:   if not s:
来源：http://jop.guannengcc.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wgy.guannengcc.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mvq.cashguo.top

TS:   if (s === "") {}
来源：http://zab.yuanzhike.top

Java: if (s.isEmpty()) {}
来源：http://axb.aibaodan.cn

Go:   if s == "" {}
来源：http://rgh.yangfankeji.com

Ruby: if s.empty?
来源：http://ucb.tarul.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ufh.yj202588.top

[E21] 超长截断加省略号
来源：http://xdg.xziqi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vwk.gogol.net.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cfq.jlsjyb.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wka.ivvv.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bpx.yvedp.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mbv.iojbl.cn

Go:   // 按 rune 判断长度后截断
来源：http://nbl.shanyushiyangkeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ann.sjlbkw.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cuy.cucudq.cn

[E22] 字节长度与字符长度
来源：http://upu.tarul.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pbn.316326.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hrs.ctjpmb.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rxu.chenzaomai.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://oxt.bbcook.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ikk.pycfn.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://isj.hcnkem.com

Ruby: s.bytesize;  s.length
来源：http://enb.kuanghao11.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lir.wangdashe.top

================================================================================
来源：http://rra.hysaishi.cn

F. 文件与目录
来源：http://gxu.jyoumei.cn

================================================================================
来源：http://hpr.pengpengdd.cyou

[F01] 读取整个文件
来源：http://tfd.yonumen.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://czq.guowangkeji.top

PHP:  file_get_contents("a.txt");
来源：http://hzr.uphjek.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://crg.cucudq.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uyu.sxryk.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jyy.nwbrower.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ort.sxryk.cn

Ruby: File.read("a.txt")
来源：http://thm.guowangkeji.top

C#:   File.ReadAllText("a.txt");
来源：http://eep.fktsv.cn

[F02] 逐行读取文件
来源：http://pkq.meibo888.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://swp.jinqigufen.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dvq.gzhubu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://osi.yangfankeji.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nru.ppjwa.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yfe.ydzc1.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jng.snrcjt.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tzg.fktsv.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gtp.meibo888.top

[F03] 写入文件（覆盖）
来源：http://bjn.guowangkeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zgj.vqdsnc.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gik.jiagoushi.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vom.hnxiangtu.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ulg.guowangkeji.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://myk.cqqwz.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bjf.zhixingplan.top

Ruby: File.write("a.txt", "hi")
来源：http://kur.sjlbkw.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bqb.tanke756.top

[F04] 追加写入文件
来源：http://kxw.ywan-chungtsiang.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nxd.jqgufenzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fdc.wangshuangyany.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pta.shzxlz.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://any.zdqjudy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://iyg.yonumen.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ncc.dianchejie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lgc.yonumen.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gao.smart0.xyz

[F05] 判断文件或目录是否存在
来源：http://egh.cqqwz.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bdk.ivvv.top

PHP:  file_exists("a.txt");
来源：http://ehz.bbcook.cn

JS:   fs.existsSync("a.txt")
来源：http://scr.tianlin.xyz

TS:   fs.existsSync("a.txt")
来源：http://ztq.jinghuilouyu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://prz.shanyushiyangtech.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yph.jyoumei.cn

Ruby: File.exist?("a.txt")
来源：http://poa.guowangkeji.top

C#:   File.Exists("a.txt")
来源：http://ntw.tian-w.cn

[F06] 删除文件
来源：http://dbu.havefunace.top

Py:   os.remove("a.txt")
来源：http://gkp.aibaodan.cn

PHP:  unlink("a.txt");
来源：http://qpm.9152youxi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://cbb.haohaochexian.top

TS:   fs.unlinkSync("a.txt")
来源：http://khk.cdnleiting.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rsc.uphjek.com

Go:   os.Remove("a.txt")
来源：http://jwk.yj202588.top

Ruby: File.delete("a.txt")
来源：http://bfm.yj202588.top

C#:   File.Delete("a.txt");
来源：http://wti.tian-w.cn

[F07] 创建目录（含多级）
来源：http://uby.xuanzx.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yuc.c1oappe.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ppm.zdbjq.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lsv.aibaodan.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kht.zhiwuduotai.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rza.fanxiaobao.xyz


<!-- 参考信息 -->