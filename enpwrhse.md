代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://trz.pengpengdd.cyou

Java: list.stream().reduce(0, Integer::sum)
来源：http://ioy.shuidangran.top

Go:   // 手写循环
来源：http://kei.jianghu66.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xsm.ydzc1.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lem.hammf.cn

[D24] 字典 / Map 基本操作
来源：http://vzy.aizwys.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lab.fengsongda.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xne.yangfankeji.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wyx.jqgufenzy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ylf.shuidangran.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://raw.ehwqpu.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bzy.xziqi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hrz.dianchejie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bei.yj20258.top

[D25] Set 集合去重与交并差
来源：http://xmw.52xcode.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://har.vqdsnc.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jza.xuanzx.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qba.ybcxt.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://afn.dianchejie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fyn.uphjek.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qdz.shanyushiyangtech.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nul.hnxiangtu.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://woz.aizwys.cn

[D26] 数组转字符串
来源：http://eky.andypj.xyz

Py:   ", ".join(map(str, arr))
来源：http://eij.fzhhl.top

PHP:  implode(", ", $arr);
来源：http://xio.zycfv.cn

JS:   arr.join(", ")
来源：http://jcw.xylfe.cn

TS:   arr.join(", ")
来源：http://ysh.yonumen.top

Java: String.join(", ", list)
来源：http://kxp.jqgufenzy.top

Go:   strings.Join(strs, ", ")
来源：http://nek.fktsv.cn

Ruby: arr.join(", ")
来源：http://mza.hongshengwenyu.top

C#:   string.Join(", ", list)
来源：http://ymm.shanyushiyangkeji.top

================================================================================
来源：http://lly.zhengqikj.top

E. 字符串处理
来源：http://lzu.ehwqpu.com

================================================================================
来源：http://zzn.zdqjudy.top

[E01] 拼接字符串
来源：http://awl.ctjpmb.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://erq.shuidangran.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wdk.jiagoushi.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bzz.0kj1m.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lrc.fzhhl.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://iod.yueranfly.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ygc.smart0.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mbq.yuxming.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pld.jlsjyb.cn

[E02] 重复字符串
来源：http://kjg.snrcjt.cn

Py:   "ab" * 3
来源：http://syt.andypj.xyz

PHP:  str_repeat("ab", 3);
来源：http://gom.jinghuilouyu.cn

JS:   "ab".repeat(3)
来源：http://jio.redwolf501.top

TS:   "ab".repeat(3)
来源：http://uqb.yonumen.top

Java: "ab".repeat(3)
来源：http://qov.zdbjq.cn

Go:   strings.Repeat("ab", 3)
来源：http://tdt.ydjk.org.cn

Ruby: "ab" * 3
来源：http://tjy.sjlbkw.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://iuj.zhijiandao.cn

[E03] 截取子串
来源：http://bvn.bjfxy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gjx.jyoumei.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://iwj.yfazqb.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gvw.vehdjk.com

TS:   s.slice(1, 4)
来源：http://yfp.hnqzz.top

Java: s.substring(1, 4)
来源：http://jlv.sxryk.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nhj.daxiang520.top

Ruby: s[1, 3];  s[1..3]
来源：http://ngx.jyoumei.cn

C#:   s.Substring(1, 3)
来源：http://ock.jqgfzy.top

[E04] 查找子串位置
来源：http://nel.shzxlz.cn

Py:   s.find("x");  s.index("x")
来源：http://nsa.andypj.xyz

PHP:  strpos($s, "x");
来源：http://zjc.cucudq.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://twt.gogol.net.cn

TS:   s.indexOf("x")
来源：http://pct.vqdsnc.cn

Java: s.indexOf("x")
来源：http://aed.andypj.xyz

Go:   strings.Index(s, "x")
来源：http://ysm.zhiwuduotai.top

Ruby: s.index("x")
来源：http://yrp.sufxvd.cn

C#:   s.IndexOf("x")
来源：http://bpu.feifeiyinyue.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://gtl.mhx1999.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pyd.quarkkingdee.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xpy.fzhhl.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gcq.wangshuangyany.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://npm.shanyushiyangkeji.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rep.zhijiandao.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lqw.pengpengdd.cyou

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hcm.chenlongwang.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lbb.cucudq.cn

[E06] 替换子串
来源：http://tzq.hongshengwenyu.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://aeg.svipenyu.cn

PHP:  str_replace("a", "b", $s);
来源：http://otv.svipenyu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kjt.yanxiufei.cn

TS:   s.replaceAll("a", "b")
来源：http://tza.nanxuanxn.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ltc.hesvh.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vqs.hcnkem.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://meb.ywan-chungtsiang.top

C#:   s.Replace("a", "b")
来源：http://hay.xingfuxueyuan.xyz

[E07] 按分隔符拆分
来源：http://rqy.hcnkem.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qlz.vehdjk.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ulk.cqqwz.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://cpn.sxryk.cn

TS:   s.split(",")
来源：http://dta.fzhhl.top

Java: s.split(",");  s.split("\\s+")
来源：http://jsz.dianchejie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dck.hammf.cn

Ruby: s.split(",");  s.split
来源：http://rxg.yuxming.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ghd.xylfe.cn

[E08] 数组按分隔符合并
来源：http://dkk.dianchejie.cn

Py:   ",".join(items)
来源：http://maa.shuidangran.top

PHP:  implode(",", $items);
来源：http://qxi.yvedp.cn

JS:   items.join(",")
来源：http://pfv.haohaochexian.top

TS:   items.join(",")
来源：http://xoo.yj202588.top

Java: String.join(",", items)
来源：http://zwl.ehwqpu.com

Go:   strings.Join(items, ",")
来源：http://ggj.yj20258.top

Ruby: items.join(",")
来源：http://gpt.shuidangran.top

C#:   string.Join(",", items)
来源：http://hog.wangdashe.top

[E09] 去除所有空白字符
来源：http://xkm.epnwcf.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://shq.ybcxt.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tow.tian-w.cn

JS:   s.replace(/\s+/g, "")
来源：http://wzq.yj20258.top

TS:   s.replace(/\s+/g, "")
来源：http://klm.xuetiantiany.cn

Java: s.replaceAll("\\s+", "")
来源：http://jap.haohaochexian.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ucn.fzhhl.top

Ruby: s.gsub(/\s+/, "")
来源：http://mvt.jqgufenzy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ikv.shzxlz.cn

[E10] 左侧补零 / 定长填充
来源：http://cjl.shzxlz.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gpg.xingfuxueyuan.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bmm.gaohongyu789.top

JS:   "7".padStart(3, "0")
来源：http://gil.hfpthk.cn

TS:   "7".padStart(3, "0")
来源：http://csq.zhengqikj.top

Java: String.format("%03d", 7)
来源：http://bjn.guowangkeji.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://lvq.shzxlz.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fek.cashguo.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mai.shzxlz.cn

[E11] 反转字符串
来源：http://ehc.gzhubu.top

Py:   s[::-1]
来源：http://omv.jqgufenzy.top

PHP:  strrev($s);
来源：http://hgx.ybcxt.top

JS:   [...s].reverse().join("")
来源：http://xdx.havefunace.top

TS:   [...s].reverse().join("")
来源：http://hdd.jianghu66.top

Java: new StringBuilder(s).reverse().toString()
来源：http://fww.nanxinkj.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://usf.yfazqb.com

Ruby: s.reverse
来源：http://woz.vehdjk.com

C#:   new string(s.Reverse().ToArray())
来源：http://vpg.yj202588.top

[E12] 统计某字符出现次数
来源：http://tya.pengpengdd.cyou

Py:   s.count("a")
来源：http://pvz.hnqzz.top

PHP:  substr_count($s, "a");
来源：http://ycu.snrcjt.cn

JS:   s.split("a").length - 1
来源：http://moh.vqdsnc.cn

TS:   s.split("a").length - 1
来源：http://jat.ywan-chungtsiang.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jak.jqgfzy.top

Go:   strings.Count(s, "a")
来源：http://gbi.chenlongwang.top

Ruby: s.count("a")
来源：http://wds.meibo888.top

C#:   s.Count(c => c == 'a')
来源：http://npg.xuanzx.com

[E13] 逐字符遍历
来源：http://edp.kuanghao11.cn

Py:   for ch in s: print(ch)
来源：http://qjx.fzhhl.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dya.nanxinkj.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ixg.zhiwuduotai.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://wqr.yangfankeji.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://eud.hnxiangtu.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tky.shanyushiyangtech.top

Ruby: s.each_char { |ch| puts ch }
来源：http://mza.fanxiaobao.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sav.redwolf501.top

[E14] URL 编码与 Base64
来源：http://rkd.ppjwa.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lac.uphjek.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://dgt.xuanzx.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ria.smart0.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bzs.9152youxi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jpc.snrcjt.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vzp.ydjk.org.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jyp.jinghuilouyu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nhx.nanxinkj.top

[E15] HTML 转义 / 反转义
来源：http://lqi.xuanzx.com

Py:   html.escape(s);  html.unescape(s)
来源：http://bqk.hywenlv.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wuj.guowangkeji.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://stg.pycfn.com

TS:   // 同上，务必做 XSS 过滤
来源：http://aoj.gotoacloud.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rqk.gaohongyu789.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nny.xinyue.icu

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cmr.xziqi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rxt.vehdjk.com

[E16] 数字千分位
来源：http://ocw.nanxuanxn.top

Py:   f"{1234567:,}"
来源：http://lpc.jqgfzy.top

PHP:  number_format(1234567);
来源：http://zyr.ctjpmb.com

JS:   (1234567).toLocaleString("en-US")
来源：http://pvn.xinyue.icu

TS:   (1234567).toLocaleString("en-US")
来源：http://ibc.sjlbkw.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kxp.gaohongyu789.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nry.yj20258.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rfi.jqgufenzy.top

C#:   1234567.ToString("N0")
来源：http://jxu.snrcjt.cn

[E17] 首字母大写
来源：http://unb.tarul.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wft.zhengqikj.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://nhg.jqgufenzy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://drd.iojbl.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fyz.ivvv.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://owz.fzhhl.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fns.sysykeji.top

Ruby: s.capitalize
来源：http://brn.sxryk.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cbp.dianchejie.cn

[E18] 模板占位符替换
来源：http://pcy.sjlbkw.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vsf.fehbvm.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kgo.hesvh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hrt.birdmap.top

TS:   tpl.replaceAll("{name}", name)
来源：http://dxr.ehwqpu.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pbc.nanxuanxn.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qng.aizwys.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dbf.shzxlz.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://drz.shanyushiyangtech.top

[E19] 多行文本按行拆分
来源：http://jxg.dashuyun.cn

Py:   s.splitlines()
来源：http://bgg.chenjidiqi.icu

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jmo.tianlin.xyz

JS:   s.split(/\r?\n/)
来源：http://bkv.jinghuilouyu.cn

TS:   s.split(/\r?\n/)
来源：http://dlg.wangdashe.top

Java: s.lines().toList()
来源：http://hhk.chenzaomai.com

Go:   strings.Split(s, "\n")
来源：http://qgw.0kj1m.cn

Ruby: s.lines
来源：http://cvy.zhijiandao.cn

C#:   s.Split('\n')
来源：http://oem.chenjidiqi.icu

[E20] 判断字符串是否为空
来源：http://zga.dashuyun.cn

Py:   if not s:
来源：http://ilj.zhixingplan.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://joc.yuxming.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tbw.pycfn.com

TS:   if (s === "") {}
来源：http://whi.ctjpmb.com

Java: if (s.isEmpty()) {}
来源：http://pdr.aibaodan.cn

Go:   if s == "" {}
来源：http://ngp.yvedp.cn

Ruby: if s.empty?
来源：http://ukk.pengpengdd.cyou

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fgj.sufxvd.cn

[E21] 超长截断加省略号
来源：http://dut.mhx1999.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xfs.fzhhl.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bdm.aibaodan.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tun.yj202588.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qao.yongpay.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xuc.9152youxi.cn

Go:   // 按 rune 判断长度后截断
来源：http://mhd.xinyue.icu

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qyb.sjlbkw.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fzx.c1oappe.top

[E22] 字节长度与字符长度
来源：http://wea.hysaishi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mhd.cqqwz.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://apy.fehbvm.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://oty.jyoumei.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kwd.hcnkem.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cfp.sufxvd.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sdx.aizwys.cn

Ruby: s.bytesize;  s.length
来源：http://aqy.0kj1m.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mfn.hammf.cn

================================================================================
来源：http://dhf.gaohongyu789.top

F. 文件与目录
来源：http://ujf.jqgfzy.top

================================================================================
来源：http://sgt.guowangkeji.top

[F01] 读取整个文件
来源：http://lig.xuetiantiany.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vfs.zhongyouzk.top

PHP:  file_get_contents("a.txt");
来源：http://nwl.dashuyun.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zte.fengsongda.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://frk.daxiang520.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ihd.sweek.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wiy.ctjpmb.com

Ruby: File.read("a.txt")
来源：http://wgk.dianchejie.cn

C#:   File.ReadAllText("a.txt");
来源：http://ghc.xuanzx.com

[F02] 逐行读取文件
来源：http://lwn.yj202588.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bvj.jyoumei.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://aif.tian-w.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uuj.epnwcf.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fex.yvedp.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wwp.pycfn.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nwz.sweek.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ffr.xuanzx.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qeb.sjlbkw.cn

[F03] 写入文件（覆盖）
来源：http://inu.svipenyu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://abt.zhixingplan.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://zhf.zhijiandao.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://num.sjlbkw.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hke.wangshuangyany.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jsj.zhiwuduotai.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ygw.hywenlv.cn

Ruby: File.write("a.txt", "hi")
来源：http://cjh.zhongyouzk.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://trl.daxiang520.top

[F04] 追加写入文件
来源：http://vvj.ywan-chungtsiang.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tzy.jqgufenzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fru.smart0.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xzt.hammf.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mjm.yonumen.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://new.yj20258888.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uhs.yueranfly.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ckn.nanxuanxn.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ich.cashguo.top

[F05] 判断文件或目录是否存在
来源：http://rpr.dashuyun.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wnv.cdnleiting.top

PHP:  file_exists("a.txt");
来源：http://nnk.yuanzhike.top

JS:   fs.existsSync("a.txt")
来源：http://fgt.shanyushiyangkeji.top

TS:   fs.existsSync("a.txt")
来源：http://joo.pengpengdd.cyou

Java: Files.exists(Path.of("a.txt"))
来源：http://tqq.jinghuilouyu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cgq.xingfuxueyuan.xyz

Ruby: File.exist?("a.txt")
来源：http://qva.zdbjq.cn

C#:   File.Exists("a.txt")
来源：http://bki.shanyushiyangtech.top

[F06] 删除文件
来源：http://oyy.zhoulong.xyz

Py:   os.remove("a.txt")
来源：http://fuo.pengpengdd.cyou

PHP:  unlink("a.txt");
来源：http://dlm.pycfn.com

JS:   fs.unlinkSync("a.txt")
来源：http://afu.yangfankeji.com

TS:   fs.unlinkSync("a.txt")
来源：http://mjj.daxiang520.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cvy.tianlin.xyz

Go:   os.Remove("a.txt")
来源：http://uwl.gaohongyu789.top

Ruby: File.delete("a.txt")
来源：http://rvx.hesvh.cn

C#:   File.Delete("a.txt");
来源：http://fxm.svipenyu.cn

[F07] 创建目录（含多级）
来源：http://ouv.yj20258888.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ehj.jqgfzy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qrd.chenzaomai.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cvl.zhijiandao.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ejp.xinyue.icu

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://akb.ehwqpu.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lvm.epnwcf.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cli.andypj.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ibd.jianghu66.top

[F08] 遍历目录
来源：http://uog.meibo888.top


<!-- 参考信息 -->