代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://snl.yuanzhike.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zll.sysykeji.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hqg.yanxiufei.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jnn.smart0.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://apg.vehdjk.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pno.zhongyouzk.top

[D25] Set 集合去重与交并差
来源：http://ekz.guannengcc.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qmc.meibo888.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yqu.epnwcf.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lbx.jlsjyb.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xlg.yueranfly.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qkf.zhijiandao.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jcq.9152youxi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fzi.hesvh.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://aqn.hysaishi.cn

[D26] 数组转字符串
来源：http://jkp.jinqigfzy.top

Py:   ", ".join(map(str, arr))
来源：http://jxk.aizwys.cn

PHP:  implode(", ", $arr);
来源：http://mla.wangshuangyany.cn

JS:   arr.join(", ")
来源：http://kmy.smart0.xyz

TS:   arr.join(", ")
来源：http://gjf.tarul.cn

Java: String.join(", ", list)
来源：http://qix.snrcjt.cn

Go:   strings.Join(strs, ", ")
来源：http://vvv.fehbvm.com

Ruby: arr.join(", ")
来源：http://mzh.jianghu66.top

C#:   string.Join(", ", list)
来源：http://bda.gaohongyu789.top

================================================================================
来源：http://rbn.yfazqb.com

E. 字符串处理
来源：http://ncf.chenjidiqi.icu

================================================================================
来源：http://gbw.sysykeji.top

[E01] 拼接字符串
来源：http://hcb.yongpay.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qrw.zhoulong.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hul.mhx1999.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kvf.chenjidiqi.icu

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xqs.zhongyouzk.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://evj.dianchejie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ghf.xuetiantiany.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wuo.cqqwz.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mab.hnxiangtu.top

[E02] 重复字符串
来源：http://lhs.aizwys.cn

Py:   "ab" * 3
来源：http://ahh.iojbl.cn

PHP:  str_repeat("ab", 3);
来源：http://woa.nanxuanxn.top

JS:   "ab".repeat(3)
来源：http://lho.shanyushiyangtech.top

TS:   "ab".repeat(3)
来源：http://avs.tarul.cn

Java: "ab".repeat(3)
来源：http://mlo.iojbl.cn

Go:   strings.Repeat("ab", 3)
来源：http://zlu.gzhubu.top

Ruby: "ab" * 3
来源：http://rcm.ppjwa.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://czt.haohaochexian.top

[E03] 截取子串
来源：http://red.gotoacloud.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rrs.xinyue.icu

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jql.xylfe.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rhh.pycfn.com

TS:   s.slice(1, 4)
来源：http://gpj.yj202588.top

Java: s.substring(1, 4)
来源：http://spk.shanyushiyangtech.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gih.birdmap.top

Ruby: s[1, 3];  s[1..3]
来源：http://bqd.jqgufenzy.top

C#:   s.Substring(1, 3)
来源：http://pbf.yvedp.cn

[E04] 查找子串位置
来源：http://vxb.zhijiandao.cn

Py:   s.find("x");  s.index("x")
来源：http://iwi.hesvh.cn

PHP:  strpos($s, "x");
来源：http://jve.haohaochexian.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wuy.daria6918.cn

TS:   s.indexOf("x")
来源：http://kep.fengsongda.top

Java: s.indexOf("x")
来源：http://cao.zhaomingkeji.xyz

Go:   strings.Index(s, "x")
来源：http://gwn.jinyuanbaomall.cn

Ruby: s.index("x")
来源：http://mhz.52xcode.cn

C#:   s.IndexOf("x")
来源：http://oob.jinghuilouyu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gtx.ctjpmb.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://skd.316326.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vct.sxryk.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hei.zdqjudy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://nrp.ywan-chungtsiang.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kdb.cucudq.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lvn.52xcode.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gyc.zhixingplan.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lva.cucudq.cn

[E06] 替换子串
来源：http://uoc.jlsjyb.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wzl.gogol.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://lzy.52xcode.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://too.tian-w.cn

TS:   s.replaceAll("a", "b")
来源：http://pzo.ppjwa.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wdl.vehdjk.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kse.nwbrower.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xes.aizwys.cn

C#:   s.Replace("a", "b")
来源：http://rka.xingfuxueyuan.xyz

[E07] 按分隔符拆分
来源：http://hzd.shuidangran.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nrn.jyoumei.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://imq.meibo888.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://xrj.smart0.xyz

TS:   s.split(",")
来源：http://qnw.quarkkingdee.top

Java: s.split(",");  s.split("\\s+")
来源：http://nfh.yj202588.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hko.jiagoushi.top

Ruby: s.split(",");  s.split
来源：http://ira.ivvv.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ewk.havefunace.top

[E08] 数组按分隔符合并
来源：http://eed.shanyushiyangkeji.top

Py:   ",".join(items)
来源：http://wjg.ydzc1.top

PHP:  implode(",", $items);
来源：http://rwo.vqdsnc.cn

JS:   items.join(",")
来源：http://gzp.ppjwa.cn

TS:   items.join(",")
来源：http://bnj.yuanzhike.top

Java: String.join(",", items)
来源：http://cfo.fktsv.cn

Go:   strings.Join(items, ",")
来源：http://wvr.xuetiantiany.cn

Ruby: items.join(",")
来源：http://muh.jqgfzy.top

C#:   string.Join(",", items)
来源：http://bdi.shanyushiyangkeji.top

[E09] 去除所有空白字符
来源：http://gyc.nwbrower.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kex.9152youxi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fay.hywenlv.cn

JS:   s.replace(/\s+/g, "")
来源：http://odz.epnwcf.com

TS:   s.replace(/\s+/g, "")
来源：http://ixm.nanxinkj.top

Java: s.replaceAll("\\s+", "")
来源：http://nkx.ybcxt.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://scc.jiagoushi.top

Ruby: s.gsub(/\s+/, "")
来源：http://ezm.ivvv.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://axw.chenzaomai.com

[E10] 左侧补零 / 定长填充
来源：http://tgb.ppjwa.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qtv.feifeiyinyue.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://eyj.yvedp.cn

JS:   "7".padStart(3, "0")
来源：http://ofs.jiagoushi.top

TS:   "7".padStart(3, "0")
来源：http://rxt.vehdjk.com

Java: String.format("%03d", 7)
来源：http://gqa.hesvh.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hsz.0kj1m.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mql.yj20258888.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sig.birdmap.top

[E11] 反转字符串
来源：http://vvr.tian-w.cn

Py:   s[::-1]
来源：http://vnl.zhaomingkeji.xyz

PHP:  strrev($s);
来源：http://quj.fehbvm.com

JS:   [...s].reverse().join("")
来源：http://vwf.0kj1m.cn

TS:   [...s].reverse().join("")
来源：http://poj.yueranfly.top

Java: new StringBuilder(s).reverse().toString()
来源：http://zyq.jlsjyb.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://mou.svipenyu.cn

Ruby: s.reverse
来源：http://msp.yuxming.cn

C#:   new string(s.Reverse().ToArray())
来源：http://tsu.shangyingyoupin.top

[E12] 统计某字符出现次数
来源：http://tjt.pengpengdd.cyou

Py:   s.count("a")
来源：http://lhv.jianghu66.top

PHP:  substr_count($s, "a");
来源：http://gow.chenlongwang.top

JS:   s.split("a").length - 1
来源：http://yri.ctjpmb.com

TS:   s.split("a").length - 1
来源：http://tmt.uphjek.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://chp.cashguo.top

Go:   strings.Count(s, "a")
来源：http://kex.zhaomingkeji.xyz

Ruby: s.count("a")
来源：http://qrq.316326.xyz

C#:   s.Count(c => c == 'a')
来源：http://nyz.yanxiufei.cn

[E13] 逐字符遍历
来源：http://owj.ctjpmb.com

Py:   for ch in s: print(ch)
来源：http://ewc.vehdjk.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://clf.dianchejie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://whl.shangyingyoupin.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://cym.xziqi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bmc.yuanzhike.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://eth.jyoumei.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://dww.jiagoushi.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dhn.xziqi.cn

[E14] URL 编码与 Base64
来源：http://eym.wangdashe.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://unv.hfpthk.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qce.sjlbkw.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://twn.fktsv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wau.svipenyu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://iau.tian-w.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ybf.hysaishi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kzo.xinyue.icu

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ktb.guannengcc.top

[E15] HTML 转义 / 反转义
来源：http://izl.yongpay.top

Py:   html.escape(s);  html.unescape(s)
来源：http://qyp.cucudq.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mum.zdbjq.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lfc.ydzc1.top

TS:   // 同上，务必做 XSS 过滤
来源：http://mxs.cheryme.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kye.ydjk.org.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fqa.fktsv.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rca.shzxlz.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://swx.zhijiandao.cn

[E16] 数字千分位
来源：http://knz.316326.xyz

Py:   f"{1234567:,}"
来源：http://tle.kuanghao11.cn

PHP:  number_format(1234567);
来源：http://itd.fanxiaobao.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://irv.xziqi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ktr.jyoumei.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://odl.yangfankeji.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pvp.pengpengdd.cyou

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xad.bjfxy.top

C#:   1234567.ToString("N0")
来源：http://uwq.fktsv.cn

[E17] 首字母大写
来源：http://gaq.guannengcc.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://alk.cqqwz.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://sgg.vehdjk.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fnf.daria6918.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lbw.yueranfly.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vtb.nanxinkj.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dir.yongpay.top

Ruby: s.capitalize
来源：http://wdn.tanke756.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ssz.fehbvm.com

[E18] 模板占位符替换
来源：http://fsr.ppjwa.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vhj.fengsongda.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bfa.chenzaomai.com

JS:   tpl.replaceAll("{name}", name)
来源：http://cri.tianlin.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://pep.jqgfzy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://owh.pycfn.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://uzd.dashuyun.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nlo.daria6918.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bnf.aizwys.cn

[E19] 多行文本按行拆分
来源：http://gau.zdbjq.cn

Py:   s.splitlines()
来源：http://ahf.yvedp.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hrz.zhixingplan.top

JS:   s.split(/\r?\n/)
来源：http://gwt.gzhubu.top

TS:   s.split(/\r?\n/)
来源：http://fjs.ywan-chungtsiang.top

Java: s.lines().toList()
来源：http://dvj.tian-w.cn

Go:   strings.Split(s, "\n")
来源：http://cat.iojbl.cn

Ruby: s.lines
来源：http://fuy.ybcxt.top

C#:   s.Split('\n')
来源：http://qat.redwolf501.top

[E20] 判断字符串是否为空
来源：http://qnt.xingfuxueyuan.xyz

Py:   if not s:
来源：http://lan.zhongyouzk.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://olo.redwolf501.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jmf.gzhubu.top

TS:   if (s === "") {}
来源：http://tsm.xziqi.cn

Java: if (s.isEmpty()) {}
来源：http://phj.daxiang520.top

Go:   if s == "" {}
来源：http://oyb.snrcjt.cn

Ruby: if s.empty?
来源：http://gmt.jyoumei.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://orc.cdnleiting.top

[E21] 超长截断加省略号
来源：http://oir.sufxvd.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kqf.iojbl.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vos.yfazqb.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ivz.hnqzz.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hdz.zhijiandao.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nhk.jinyuanbaomall.cn

Go:   // 按 rune 判断长度后截断
来源：http://qpx.iojbl.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fvv.yongpay.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rrk.cheryme.top

[E22] 字节长度与字符长度
来源：http://uui.sjlbkw.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mkw.daxiang520.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mst.ehwqpu.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xfg.hywenlv.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vrr.52xcode.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sws.nanxuanxn.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://prl.sweek.top

Ruby: s.bytesize;  s.length
来源：http://uip.c1oappe.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gcd.birdmap.top

================================================================================
来源：http://bhm.cucudq.cn

F. 文件与目录
来源：http://jsc.dianchejie.cn

================================================================================
来源：http://mpw.jlsjyb.cn

[F01] 读取整个文件
来源：http://szm.sjlbkw.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hhr.zhixingplan.top

PHP:  file_get_contents("a.txt");
来源：http://bge.hysaishi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rsc.hfpthk.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jkd.birdmap.top

Java: Files.readString(Path.of("a.txt"))
来源：http://iaz.ivvv.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xrf.zhaomingkeji.xyz

Ruby: File.read("a.txt")
来源：http://rtt.fzhhl.top

C#:   File.ReadAllText("a.txt");
来源：http://cjj.jqgufenzy.top

[F02] 逐行读取文件
来源：http://hyn.shuidangran.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jkp.hcnkem.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cng.sweek.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dmx.fehbvm.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fin.guannengcc.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jsf.yvedp.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fzq.xuanzx.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gqe.gzhubu.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://glw.yonumen.top

[F03] 写入文件（覆盖）
来源：http://jrr.fktsv.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jje.hnxiangtu.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://mxn.aizwys.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uqy.fehbvm.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hni.jinqigufen.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xxl.andypj.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://imd.yangfankeji.com

Ruby: File.write("a.txt", "hi")
来源：http://poz.wangdashe.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://euj.sweek.top

[F04] 追加写入文件
来源：http://afu.sysykeji.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ark.redwolf501.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ekz.fehbvm.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://osd.jqgfzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bwl.haohaochexian.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://urs.xylfe.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gwa.yuanzhike.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nfx.yonumen.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zlf.ywan-chungtsiang.top

[F05] 判断文件或目录是否存在
来源：http://ojw.xziqi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://anu.yj20258.top

PHP:  file_exists("a.txt");
来源：http://amb.guannengcc.top

JS:   fs.existsSync("a.txt")
来源：http://bou.guannengcc.top

TS:   fs.existsSync("a.txt")
来源：http://wjv.xuetiantiany.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ecn.tanke756.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jzd.xingfuxueyuan.xyz

Ruby: File.exist?("a.txt")
来源：http://yik.sweek.top

C#:   File.Exists("a.txt")
来源：http://mxn.c1oappe.top

[F06] 删除文件
来源：http://khy.cashguo.top

Py:   os.remove("a.txt")
来源：http://qtw.xylfe.cn

PHP:  unlink("a.txt");
来源：http://muz.fengsongda.top

JS:   fs.unlinkSync("a.txt")
来源：http://kno.ydjk.org.cn

TS:   fs.unlinkSync("a.txt")
来源：http://tfa.xinyue.icu

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mbp.ehwqpu.com

Go:   os.Remove("a.txt")
来源：http://eqn.yj20258.top

Ruby: File.delete("a.txt")
来源：http://yyn.yuxming.cn

C#:   File.Delete("a.txt");
来源：http://wwr.cqqwz.cn

[F07] 创建目录（含多级）
来源：http://yji.c1oappe.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mjj.cqqwz.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jzt.nanxuanxn.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://krp.yueranfly.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rqf.nwbrower.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ycz.redwolf501.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://afk.nwbrower.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kih.fktsv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nlc.ppjwa.cn

[F08] 遍历目录
来源：http://kpp.yueranfly.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ysx.meibo888.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://veg.jinghuilouyu.cn

JS:   fs.readdirSync("dir")
来源：http://fty.aizwys.cn

TS:   fs.readdirSync("dir")
来源：http://hls.yonumen.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ear.zhaomingkeji.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://jcc.yongpay.top

Ruby: Dir.children("dir")
来源：http://eta.xuanzx.com

C#:   Directory.GetFiles("dir")
来源：http://xda.tianlin.xyz


<!-- 参考信息 -->