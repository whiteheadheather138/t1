代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ywp.sjlbkw.cn

[D24] 字典 / Map 基本操作
来源：http://grc.zdqjudy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://aum.xuetiantiany.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rga.shangyingyoupin.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mgi.fanxiaobao.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ksl.yj20258.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xbf.chenlongwang.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tll.0kj1m.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kps.tianlin.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://enw.sxryk.cn

[D25] Set 集合去重与交并差
来源：http://kqe.guowangkeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://grl.cucudq.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://skh.wangdashe.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://isw.9152youxi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uvp.jqgufenzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kan.vqdsnc.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cjt.snrcjt.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vet.cdnleiting.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hwm.gogol.net.cn

[D26] 数组转字符串
来源：http://xgw.tian-w.cn

Py:   ", ".join(map(str, arr))
来源：http://jpp.tarul.cn

PHP:  implode(", ", $arr);
来源：http://ieu.guowangkeji.top

JS:   arr.join(", ")
来源：http://ulr.hongshengwenyu.top

TS:   arr.join(", ")
来源：http://roe.jiagoushi.top

Java: String.join(", ", list)
来源：http://tzh.9152youxi.cn

Go:   strings.Join(strs, ", ")
来源：http://ywi.ivvv.top

Ruby: arr.join(", ")
来源：http://iqe.jlsjyb.cn

C#:   string.Join(", ", list)
来源：http://jdc.chenlongwang.top

================================================================================
来源：http://rgc.ybcxt.top

E. 字符串处理
来源：http://xfn.gogol.net.cn

================================================================================
来源：http://ebo.zhijiandao.cn

[E01] 拼接字符串
来源：http://mpa.shanyushiyangtech.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://omt.mhx1999.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://env.guannengcc.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qum.aizwys.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fes.yj202588.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://btp.jiagoushi.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jul.havefunace.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wkd.shuidangran.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lmk.snrcjt.cn

[E02] 重复字符串
来源：http://qzy.cashguo.top

Py:   "ab" * 3
来源：http://kxo.yanxiufei.cn

PHP:  str_repeat("ab", 3);
来源：http://qhv.sufxvd.cn

JS:   "ab".repeat(3)
来源：http://xnl.aibaodan.cn

TS:   "ab".repeat(3)
来源：http://oqk.shanyushiyangkeji.top

Java: "ab".repeat(3)
来源：http://jgo.jqgufenzy.top

Go:   strings.Repeat("ab", 3)
来源：http://czm.snrcjt.cn

Ruby: "ab" * 3
来源：http://yvx.jyoumei.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://eld.kuanghao11.cn

[E03] 截取子串
来源：http://svq.vqdsnc.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vyr.0kj1m.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vrf.ppjwa.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://irc.jiagoushi.top

TS:   s.slice(1, 4)
来源：http://gop.0kj1m.cn

Java: s.substring(1, 4)
来源：http://cus.yongpay.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dxn.zhiwuduotai.top

Ruby: s[1, 3];  s[1..3]
来源：http://wdv.fengsongda.top

C#:   s.Substring(1, 3)
来源：http://uvu.jlsjyb.cn

[E04] 查找子串位置
来源：http://ppi.xuetiantiany.cn

Py:   s.find("x");  s.index("x")
来源：http://jbu.jlsjyb.cn

PHP:  strpos($s, "x");
来源：http://aas.ehwqpu.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fco.cqqwz.cn

TS:   s.indexOf("x")
来源：http://gvg.jinqigufen.top

Java: s.indexOf("x")
来源：http://doj.birdmap.top

Go:   strings.Index(s, "x")
来源：http://jwr.zdqjudy.top

Ruby: s.index("x")
来源：http://tjh.sjlbkw.cn

C#:   s.IndexOf("x")
来源：http://rxn.shanyushiyangkeji.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://byk.cucudq.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lcs.jlsjyb.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://iit.yj202588.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rbx.cqqwz.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://soa.sxryk.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pac.9152youxi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fxy.jinyuanbaomall.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kqq.yangfankeji.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jlf.yj20258888.top

[E06] 替换子串
来源：http://fdy.9152youxi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qly.jqgufenzy.top

PHP:  str_replace("a", "b", $s);
来源：http://emv.ywan-chungtsiang.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ahr.yangfankeji.com

TS:   s.replaceAll("a", "b")
来源：http://qhy.sjlbkw.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xtv.quarkkingdee.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kin.jinghuilouyu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rir.gotoacloud.top

C#:   s.Replace("a", "b")
来源：http://gll.jlsjyb.cn

[E07] 按分隔符拆分
来源：http://hna.pengpengdd.cyou

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://iuk.yj20258.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cui.yj20258888.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://uzc.quarkkingdee.top

TS:   s.split(",")
来源：http://wid.vehdjk.com

Java: s.split(",");  s.split("\\s+")
来源：http://blb.wangshuangyany.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dfa.ywan-chungtsiang.top

Ruby: s.split(",");  s.split
来源：http://zvo.shzxlz.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://shv.nanxuanxn.top

[E08] 数组按分隔符合并
来源：http://pgz.zhongyouzk.top

Py:   ",".join(items)
来源：http://lvp.iojbl.cn

PHP:  implode(",", $items);
来源：http://emh.shuidangran.top

JS:   items.join(",")
来源：http://hcm.chenjidiqi.icu

TS:   items.join(",")
来源：http://waw.mhx1999.top

Java: String.join(",", items)
来源：http://mvv.wangdashe.top

Go:   strings.Join(items, ",")
来源：http://xyz.jinqigufen.top

Ruby: items.join(",")
来源：http://bfn.zhixingplan.top

C#:   string.Join(",", items)
来源：http://vxg.chenlongwang.top

[E09] 去除所有空白字符
来源：http://pow.jyoumei.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ocj.yj202588.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://iju.cucudq.cn

JS:   s.replace(/\s+/g, "")
来源：http://exi.cdnleiting.top

TS:   s.replace(/\s+/g, "")
来源：http://ppa.vehdjk.com

Java: s.replaceAll("\\s+", "")
来源：http://ipw.yj20258.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://kdp.yj202588.top

Ruby: s.gsub(/\s+/, "")
来源：http://bal.svipenyu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zqn.cdnleiting.top

[E10] 左侧补零 / 定长填充
来源：http://wkn.yj202588.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://puy.gzhubu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qts.0kj1m.cn

JS:   "7".padStart(3, "0")
来源：http://tmj.sjlbkw.cn

TS:   "7".padStart(3, "0")
来源：http://exy.jinghuilouyu.cn

Java: String.format("%03d", 7)
来源：http://nzc.shangyingyoupin.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://slc.gotoacloud.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qkc.yanxiufei.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://akm.yuanzhike.top

[E11] 反转字符串
来源：http://pht.iojbl.cn

Py:   s[::-1]
来源：http://cdm.zhixingplan.top

PHP:  strrev($s);
来源：http://pft.c1oappe.top

JS:   [...s].reverse().join("")
来源：http://phe.hesvh.cn

TS:   [...s].reverse().join("")
来源：http://ili.shanyushiyangtech.top

Java: new StringBuilder(s).reverse().toString()
来源：http://vdz.fanxiaobao.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://wio.yanxiufei.cn

Ruby: s.reverse
来源：http://yex.zhaomingkeji.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://ehz.zhijiandao.cn

[E12] 统计某字符出现次数
来源：http://wpz.shangyingyoupin.top

Py:   s.count("a")
来源：http://nca.yj20258888.top

PHP:  substr_count($s, "a");
来源：http://whu.zhixingplan.top

JS:   s.split("a").length - 1
来源：http://tda.fzhhl.top

TS:   s.split("a").length - 1
来源：http://bvt.dianchejie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dxa.nwbrower.top

Go:   strings.Count(s, "a")
来源：http://epq.gaohongyu789.top

Ruby: s.count("a")
来源：http://mfi.fktsv.cn

C#:   s.Count(c => c == 'a')
来源：http://bia.xuetiantiany.cn

[E13] 逐字符遍历
来源：http://jhe.guowangkeji.top

Py:   for ch in s: print(ch)
来源：http://cdl.jinghuilouyu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yef.cheryme.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://dyt.shanyushiyangtech.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://qit.shanyushiyangkeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hvr.ppjwa.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cpg.hammf.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xjl.xinyue.icu

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ymj.yj20258888.top

[E14] URL 编码与 Base64
来源：http://xyq.aibaodan.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ywk.yongpay.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://rpv.ctjpmb.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lbl.cqqwz.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gqj.ywan-chungtsiang.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xpc.ehwqpu.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://aie.shanyushiyangtech.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wnw.dianchejie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cnp.ywan-chungtsiang.top

[E15] HTML 转义 / 反转义
来源：http://wtg.havefunace.top

Py:   html.escape(s);  html.unescape(s)
来源：http://xpb.jqgufenzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dkn.mhx1999.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nhm.bbcook.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://aeb.cashguo.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mpd.shangyingyoupin.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://akb.smart0.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rhf.shuidangran.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lab.chenzaomai.com

[E16] 数字千分位
来源：http://zhx.guowangkeji.top

Py:   f"{1234567:,}"
来源：http://epu.sufxvd.cn

PHP:  number_format(1234567);
来源：http://kda.xuanzx.com

JS:   (1234567).toLocaleString("en-US")
来源：http://llk.52xcode.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mfc.fanxiaobao.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nok.wangshuangyany.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fnw.svipenyu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bpp.jqgufenzy.top

C#:   1234567.ToString("N0")
来源：http://rem.9152youxi.cn

[E17] 首字母大写
来源：http://fry.sxryk.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gih.pengpengdd.cyou

PHP:  ucfirst($s);  ucwords($s);
来源：http://wvl.sysykeji.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uib.yj202588.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://foj.jianghu66.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mwz.jiagoushi.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://asz.shanyushiyangtech.top

Ruby: s.capitalize
来源：http://hmm.yvedp.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://haf.gaohongyu789.top

[E18] 模板占位符替换
来源：http://imw.shzxlz.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tqi.yongpay.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bia.ydzc1.top

JS:   tpl.replaceAll("{name}", name)
来源：http://dos.cqqwz.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jrp.ppjwa.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qkc.xuetiantiany.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vpg.hnqzz.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kob.52xcode.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qup.dashuyun.cn

[E19] 多行文本按行拆分
来源：http://poo.c1oappe.top

Py:   s.splitlines()
来源：http://cez.aibaodan.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rdw.hnxiangtu.top

JS:   s.split(/\r?\n/)
来源：http://nkg.pycfn.com

TS:   s.split(/\r?\n/)
来源：http://kmu.yj202588.top

Java: s.lines().toList()
来源：http://tvx.c1oappe.top

Go:   strings.Split(s, "\n")
来源：http://xjb.gogol.net.cn

Ruby: s.lines
来源：http://ebw.xingfuxueyuan.xyz

C#:   s.Split('\n')
来源：http://pbb.yanxiufei.cn

[E20] 判断字符串是否为空
来源：http://yef.ywan-chungtsiang.top

Py:   if not s:
来源：http://oxf.fengsongda.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xex.bbcook.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nsq.ctjpmb.com

TS:   if (s === "") {}
来源：http://cxp.daria6918.cn

Java: if (s.isEmpty()) {}
来源：http://akh.shangyingyoupin.top

Go:   if s == "" {}
来源：http://zch.sweek.top

Ruby: if s.empty?
来源：http://mam.birdmap.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yeo.wangdashe.top

[E21] 超长截断加省略号
来源：http://pqi.zhengqikj.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hda.ydjk.org.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cox.cheryme.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rxp.andypj.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fep.gzhubu.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ycg.52xcode.cn

Go:   // 按 rune 判断长度后截断
来源：http://ygo.zhiwuduotai.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yqg.smart0.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jmu.yj20258.top

[E22] 字节长度与字符长度
来源：http://nty.yfazqb.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qpn.redwolf501.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nnm.c1oappe.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xrq.zhiwuduotai.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zkz.yvedp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://aus.gzhubu.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://avx.snrcjt.cn

Ruby: s.bytesize;  s.length
来源：http://ebe.daxiang520.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rhe.xingfuxueyuan.xyz

================================================================================
来源：http://zjv.shzxlz.cn

F. 文件与目录
来源：http://jtc.dianchejie.cn

================================================================================
来源：http://xbs.fzhhl.top

[F01] 读取整个文件
来源：http://rbl.jinyuanbaomall.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wvs.cheryme.top

PHP:  file_get_contents("a.txt");
来源：http://dnt.xingfuxueyuan.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tmq.ybcxt.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qfi.yanxiufei.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://gxw.yvedp.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://exp.sjlbkw.cn

Ruby: File.read("a.txt")
来源：http://tcb.vqdsnc.cn

C#:   File.ReadAllText("a.txt");
来源：http://agy.bbcook.cn

[F02] 逐行读取文件
来源：http://zzc.aibaodan.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hxv.dashuyun.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cfj.shanyushiyangkeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ylb.xinyue.icu

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zmm.hfpthk.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sva.tianlin.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cha.jinqigufen.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yik.xuanzx.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cmb.wangdashe.top

[F03] 写入文件（覆盖）
来源：http://fpn.yongpay.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ovu.gzhubu.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://tle.uphjek.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nrj.guowangkeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://noh.vehdjk.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vop.sjlbkw.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hwv.316326.xyz

Ruby: File.write("a.txt", "hi")
来源：http://khv.pengpengdd.cyou

C#:   File.WriteAllText("a.txt", "hi");
来源：http://chl.ppjwa.cn

[F04] 追加写入文件
来源：http://lim.xingfuxueyuan.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zrq.tianlin.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ugi.zdqjudy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tte.hywenlv.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://brw.zhoulong.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pjn.hongshengwenyu.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yuy.yj20258888.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://prd.nanxinkj.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ggw.hesvh.cn

[F05] 判断文件或目录是否存在
来源：http://cne.hywenlv.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://goq.sweek.top

PHP:  file_exists("a.txt");
来源：http://ahg.cucudq.cn

JS:   fs.existsSync("a.txt")
来源：http://hqf.cdnleiting.top

TS:   fs.existsSync("a.txt")
来源：http://ige.epnwcf.com

Java: Files.exists(Path.of("a.txt"))
来源：http://hyk.hammf.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qgg.jqgfzy.top

Ruby: File.exist?("a.txt")
来源：http://umw.hywenlv.cn

C#:   File.Exists("a.txt")
来源：http://hpw.jiagoushi.top

[F06] 删除文件
来源：http://ihc.chenlongwang.top

Py:   os.remove("a.txt")
来源：http://gtl.wangdashe.top

PHP:  unlink("a.txt");
来源：http://qfz.tian-w.cn

JS:   fs.unlinkSync("a.txt")
来源：http://mjc.ctjpmb.com

TS:   fs.unlinkSync("a.txt")
来源：http://mhl.yongpay.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xrx.sweek.top

Go:   os.Remove("a.txt")
来源：http://vds.zhijiandao.cn

Ruby: File.delete("a.txt")
来源：http://gba.jqgfzy.top

C#:   File.Delete("a.txt");
来源：http://tgr.ydjk.org.cn

[F07] 创建目录（含多级）
来源：http://aqw.cheryme.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jqg.hongshengwenyu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vqh.jinghuilouyu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ukn.aizwys.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://awq.ydzc1.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hsv.jlsjyb.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xpb.tanke756.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vhi.zhaomingkeji.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ina.zdqjudy.top

[F08] 遍历目录
来源：http://qdj.sweek.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://mez.dianchejie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dax.wangdashe.top

JS:   fs.readdirSync("dir")
来源：http://fgu.cdnleiting.top

TS:   fs.readdirSync("dir")
来源：http://nvv.gzhubu.top


<!-- 参考信息 -->