代发 wailian999

[D23] reduce 累积计算
来源：http://iii.chenzaomai.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rqq.tian-w.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kqj.hywenlv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ibt.yfazqb.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oej.cdnleiting.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://pcb.ctjpmb.com

Go:   // 手写循环
来源：http://stq.iojbl.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pdx.yj202588.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pih.zhaomingkeji.xyz

[D24] 字典 / Map 基本操作
来源：http://eiv.shuidangran.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tlr.fengsongda.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nhb.cucudq.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nus.jinqigufen.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ftd.zhaomingkeji.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yjo.xylfe.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qxb.wangshuangyany.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ukt.dianchejie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://iyj.yongpay.top

[D25] Set 集合去重与交并差
来源：http://cmt.cqqwz.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mmy.chenzaomai.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ral.zhoulong.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jnq.xylfe.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mqa.vqdsnc.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cam.jinghuilouyu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wot.jinqigufen.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cgs.daria6918.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wwc.ehwqpu.com

[D26] 数组转字符串
来源：http://plk.gaohongyu789.top

Py:   ", ".join(map(str, arr))
来源：http://lsq.yuxming.cn

PHP:  implode(", ", $arr);
来源：http://lxk.daria6918.cn

JS:   arr.join(", ")
来源：http://dwo.meibo888.top

TS:   arr.join(", ")
来源：http://ono.sysykeji.top

Java: String.join(", ", list)
来源：http://tki.birdmap.top

Go:   strings.Join(strs, ", ")
来源：http://myh.xylfe.cn

Ruby: arr.join(", ")
来源：http://rob.jinghuilouyu.cn

C#:   string.Join(", ", list)
来源：http://jpb.jyoumei.cn

================================================================================
来源：http://eyn.ehwqpu.com

E. 字符串处理
来源：http://vvk.cheryme.top

================================================================================
来源：http://sle.cashguo.top

[E01] 拼接字符串
来源：http://mzs.hnqzz.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://aqj.fzhhl.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dht.chenjidiqi.icu

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gfj.birdmap.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.chenlongwang.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qdv.tian-w.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hms.yanxiufei.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yfe.ydzc1.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cnw.chenjidiqi.icu

[E02] 重复字符串
来源：http://hcn.jianghu66.top

Py:   "ab" * 3
来源：http://ogv.xinyue.icu

PHP:  str_repeat("ab", 3);
来源：http://upl.jqgfzy.top

JS:   "ab".repeat(3)
来源：http://kqy.fzhhl.top

TS:   "ab".repeat(3)
来源：http://rie.zycfv.cn

Java: "ab".repeat(3)
来源：http://lpu.daria6918.cn

Go:   strings.Repeat("ab", 3)
来源：http://rod.feifeiyinyue.top

Ruby: "ab" * 3
来源：http://sji.zdbjq.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dbq.jianghu66.top

[E03] 截取子串
来源：http://tmd.redwolf501.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://skt.yuxming.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lan.sjlbkw.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://uuq.316326.xyz

TS:   s.slice(1, 4)
来源：http://qjb.kuanghao11.cn

Java: s.substring(1, 4)
来源：http://aqm.hnxiangtu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gvx.chenjidiqi.icu

Ruby: s[1, 3];  s[1..3]
来源：http://yaj.sysykeji.top

C#:   s.Substring(1, 3)
来源：http://xvm.smart0.xyz

[E04] 查找子串位置
来源：http://xyz.svipenyu.cn

Py:   s.find("x");  s.index("x")
来源：http://jex.zhongyouzk.top

PHP:  strpos($s, "x");
来源：http://chn.yj20258.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://aqt.cqqwz.cn

TS:   s.indexOf("x")
来源：http://rjn.yongpay.top

Java: s.indexOf("x")
来源：http://njm.snrcjt.cn

Go:   strings.Index(s, "x")
来源：http://zjk.52xcode.cn

Ruby: s.index("x")
来源：http://exb.zhaomingkeji.xyz

C#:   s.IndexOf("x")
来源：http://awz.jqgufenzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://vrd.zhixingplan.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ugn.hywenlv.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://olb.iojbl.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cck.hfpthk.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://tuf.jinghuilouyu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hmb.aibaodan.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pha.hongshengwenyu.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xxk.nanxinkj.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cse.birdmap.top

[E06] 替换子串
来源：http://yxj.hesvh.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://oto.wangshuangyany.cn

PHP:  str_replace("a", "b", $s);
来源：http://bav.aizwys.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kse.shzxlz.cn

TS:   s.replaceAll("a", "b")
来源：http://ita.daria6918.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lpp.zhoulong.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qsm.jqgufenzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wur.pengpengdd.cyou

C#:   s.Replace("a", "b")
来源：http://moo.ctjpmb.com

[E07] 按分隔符拆分
来源：http://yuo.gzhubu.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wxx.sjlbkw.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gcv.316326.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://ysb.svipenyu.cn

TS:   s.split(",")
来源：http://zjv.sweek.top

Java: s.split(",");  s.split("\\s+")
来源：http://xtw.nanxinkj.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://whn.ybcxt.top

Ruby: s.split(",");  s.split
来源：http://cqk.zdqjudy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hbu.fktsv.cn

[E08] 数组按分隔符合并
来源：http://zbq.52xcode.cn

Py:   ",".join(items)
来源：http://rmq.zhoulong.xyz

PHP:  implode(",", $items);
来源：http://sya.316326.xyz

JS:   items.join(",")
来源：http://evd.shanyushiyangkeji.top

TS:   items.join(",")
来源：http://mwn.yfazqb.com

Java: String.join(",", items)
来源：http://ags.jinqigufen.top

Go:   strings.Join(items, ",")
来源：http://gzr.yj202588.top

Ruby: items.join(",")
来源：http://aqe.pycfn.com

C#:   string.Join(",", items)
来源：http://amv.fehbvm.com

[E09] 去除所有空白字符
来源：http://mnc.yuanzhike.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wml.ctjpmb.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xwn.iojbl.cn

JS:   s.replace(/\s+/g, "")
来源：http://shh.ywan-chungtsiang.top

TS:   s.replace(/\s+/g, "")
来源：http://srp.shzxlz.cn

Java: s.replaceAll("\\s+", "")
来源：http://iuu.ybcxt.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://zpm.guowangkeji.top

Ruby: s.gsub(/\s+/, "")
来源：http://fag.316326.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mzv.haohaochexian.top

[E10] 左侧补零 / 定长填充
来源：http://gog.havefunace.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dqa.xylfe.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pma.sjlbkw.cn

JS:   "7".padStart(3, "0")
来源：http://bxp.jqgfzy.top

TS:   "7".padStart(3, "0")
来源：http://vmj.zhaomingkeji.xyz

Java: String.format("%03d", 7)
来源：http://pbs.chenzaomai.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://zwq.hfpthk.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ptk.yonumen.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rod.xylfe.cn

[E11] 反转字符串
来源：http://jut.fktsv.cn

Py:   s[::-1]
来源：http://czn.9152youxi.cn

PHP:  strrev($s);
来源：http://oul.zhiwuduotai.top

JS:   [...s].reverse().join("")
来源：http://ymn.fktsv.cn

TS:   [...s].reverse().join("")
来源：http://kns.bjfxy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://vja.sjlbkw.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hwp.ydjk.org.cn

Ruby: s.reverse
来源：http://fzz.yonumen.top

C#:   new string(s.Reverse().ToArray())
来源：http://vvg.jiagoushi.top

[E12] 统计某字符出现次数
来源：http://wlp.zdqjudy.top

Py:   s.count("a")
来源：http://umt.cqqwz.cn

PHP:  substr_count($s, "a");
来源：http://xfa.sxryk.cn

JS:   s.split("a").length - 1
来源：http://kzl.aibaodan.cn

TS:   s.split("a").length - 1
来源：http://qfs.gogol.net.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://meo.yvedp.cn

Go:   strings.Count(s, "a")
来源：http://yak.hcnkem.com

Ruby: s.count("a")
来源：http://tks.pycfn.com

C#:   s.Count(c => c == 'a')
来源：http://erp.jlsjyb.cn

[E13] 逐字符遍历
来源：http://usy.wangdashe.top

Py:   for ch in s: print(ch)
来源：http://jbx.gzhubu.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ara.sweek.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://uni.zycfv.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qmk.yangfankeji.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tud.chenjidiqi.icu

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vsx.haohaochexian.top

Ruby: s.each_char { |ch| puts ch }
来源：http://vzw.gaohongyu789.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hyl.ppjwa.cn

[E14] URL 编码与 Base64
来源：http://xcx.andypj.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kch.shanyushiyangtech.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://jrf.zhoulong.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zvo.yuxming.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lmn.aibaodan.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wik.0kj1m.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sze.fengsongda.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qui.nanxinkj.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fwf.guannengcc.top

[E15] HTML 转义 / 反转义
来源：http://wpk.ctjpmb.com

Py:   html.escape(s);  html.unescape(s)
来源：http://doy.sxryk.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://daa.xuetiantiany.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hgm.jqgfzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://vwc.xuetiantiany.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://oje.zhixingplan.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xsa.haohaochexian.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dah.yj20258.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jmw.pengpengdd.cyou

[E16] 数字千分位
来源：http://lfc.zdqjudy.top

Py:   f"{1234567:,}"
来源：http://cyh.fzhhl.top

PHP:  number_format(1234567);
来源：http://mnm.shanyushiyangkeji.top

JS:   (1234567).toLocaleString("en-US")
来源：http://kpv.ehwqpu.com

TS:   (1234567).toLocaleString("en-US")
来源：http://tjj.smart0.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ydr.ctjpmb.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tpi.c1oappe.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xrp.jqgfzy.top

C#:   1234567.ToString("N0")
来源：http://rli.iojbl.cn

[E17] 首字母大写
来源：http://uel.sufxvd.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mie.0kj1m.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ipx.xuanzx.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://crk.yj20258.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ogz.hnqzz.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bjm.fanxiaobao.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lpk.quarkkingdee.top

Ruby: s.capitalize
来源：http://eaz.jinyuanbaomall.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://oil.jlsjyb.cn

[E18] 模板占位符替换
来源：http://kuo.ydzc1.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gbd.xinyue.icu

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://het.xuanzx.com

JS:   tpl.replaceAll("{name}", name)
来源：http://qws.tianlin.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://hfz.9152youxi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xoz.hesvh.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jzd.9152youxi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dam.jlsjyb.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gjf.zhengqikj.top

[E19] 多行文本按行拆分
来源：http://vac.hcnkem.com

Py:   s.splitlines()
来源：http://geu.sxryk.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ezg.jinqigufen.top

JS:   s.split(/\r?\n/)
来源：http://lkl.jinghuilouyu.cn

TS:   s.split(/\r?\n/)
来源：http://aso.vehdjk.com

Java: s.lines().toList()
来源：http://ylt.fzhhl.top

Go:   strings.Split(s, "\n")
来源：http://rei.wangshuangyany.cn

Ruby: s.lines
来源：http://utc.kuanghao11.cn

C#:   s.Split('\n')
来源：http://gfl.hysaishi.cn

[E20] 判断字符串是否为空
来源：http://ecb.guowangkeji.top

Py:   if not s:
来源：http://nac.yonumen.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ciq.meibo888.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qxk.bjfxy.top

TS:   if (s === "") {}
来源：http://dxi.epnwcf.com

Java: if (s.isEmpty()) {}
来源：http://etk.aibaodan.cn

Go:   if s == "" {}
来源：http://qrs.yangfankeji.com

Ruby: if s.empty?
来源：http://fcx.gzhubu.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ifq.xuanzx.com

[E21] 超长截断加省略号
来源：http://rwc.ppjwa.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mxb.ehwqpu.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nez.shanyushiyangtech.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ubp.xingfuxueyuan.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xbi.fktsv.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fye.dashuyun.cn

Go:   // 按 rune 判断长度后截断
来源：http://rxd.bbcook.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://evj.ctjpmb.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jyk.quarkkingdee.top

[E22] 字节长度与字符长度
来源：http://aiz.fengsongda.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://npj.xylfe.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mhz.birdmap.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yvm.feifeiyinyue.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gio.sxryk.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vvg.jinghuilouyu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yyn.chenjidiqi.icu

Ruby: s.bytesize;  s.length
来源：http://ynw.cashguo.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hna.yonumen.top

================================================================================
来源：http://cqe.hongshengwenyu.top

F. 文件与目录
来源：http://qee.gogol.net.cn

================================================================================
来源：http://lfi.shzxlz.cn

[F01] 读取整个文件
来源：http://ptw.yuanzhike.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yvm.cucudq.cn

PHP:  file_get_contents("a.txt");
来源：http://jqr.zdbjq.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://adf.nwbrower.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wfw.dashuyun.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://riq.pengpengdd.cyou

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://frt.ybcxt.top

Ruby: File.read("a.txt")
来源：http://pwz.bjfxy.top

C#:   File.ReadAllText("a.txt");
来源：http://vtm.yangfankeji.com

[F02] 逐行读取文件
来源：http://hhl.bjfxy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://iis.quarkkingdee.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nqt.gzhubu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zze.9152youxi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://whw.cdnleiting.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wsr.zhijiandao.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://iwl.gogol.net.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ueo.zhixingplan.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ipd.tian-w.cn

[F03] 写入文件（覆盖）
来源：http://srx.zhaomingkeji.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ylt.xylfe.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ymo.chenjidiqi.icu

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jkg.cdnleiting.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://epq.yj20258.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dce.quarkkingdee.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hta.haohaochexian.top

Ruby: File.write("a.txt", "hi")
来源：http://azq.yj202588.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://erd.hongshengwenyu.top

[F04] 追加写入文件
来源：http://hru.haohaochexian.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qlj.hesvh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sih.yueranfly.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ynk.chenjidiqi.icu

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tio.zhiwuduotai.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gbe.jianghu66.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://glm.chenjidiqi.icu

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ari.aibaodan.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://urw.kuanghao11.cn

[F05] 判断文件或目录是否存在
来源：http://yvq.sjlbkw.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://apk.epnwcf.com

PHP:  file_exists("a.txt");
来源：http://mqs.hfpthk.cn

JS:   fs.existsSync("a.txt")
来源：http://tsu.hnqzz.top

TS:   fs.existsSync("a.txt")
来源：http://uwr.havefunace.top

Java: Files.exists(Path.of("a.txt"))
来源：http://jki.hcnkem.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bvj.svipenyu.cn

Ruby: File.exist?("a.txt")
来源：http://euu.zhijiandao.cn

C#:   File.Exists("a.txt")
来源：http://yfg.ywan-chungtsiang.top

[F06] 删除文件
来源：http://owf.zhongyouzk.top

Py:   os.remove("a.txt")
来源：http://zqq.gogol.net.cn

PHP:  unlink("a.txt");
来源：http://low.wangshuangyany.cn

JS:   fs.unlinkSync("a.txt")
来源：http://nqt.zdbjq.cn

TS:   fs.unlinkSync("a.txt")
来源：http://qzr.yongpay.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kin.hesvh.cn

Go:   os.Remove("a.txt")
来源：http://iss.haohaochexian.top

Ruby: File.delete("a.txt")
来源：http://tda.jqgfzy.top

C#:   File.Delete("a.txt");
来源：http://rkg.sufxvd.cn

[F07] 创建目录（含多级）
来源：http://uea.sweek.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ioy.aizwys.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jyk.bjfxy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jmd.52xcode.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mry.ydzc1.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xrc.hongshengwenyu.top


<!-- 参考信息 -->