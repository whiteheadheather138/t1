代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://emj.fehbvm.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gwy.cdnleiting.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bev.jlsjyb.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lvq.tarul.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://esd.gzhubu.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://msu.9152youxi.cn

[D25] Set 集合去重与交并差
来源：http://gwv.ywan-chungtsiang.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://opj.snrcjt.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yzv.zhiwuduotai.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://uwm.snrcjt.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://chb.kuanghao11.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vdr.quarkkingdee.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nmm.shanyushiyangtech.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://thn.shuidangran.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://oax.ywan-chungtsiang.top

[D26] 数组转字符串
来源：http://rwf.yj20258.top

Py:   ", ".join(map(str, arr))
来源：http://edv.c1oappe.top

PHP:  implode(", ", $arr);
来源：http://fej.yuanzhike.top

JS:   arr.join(", ")
来源：http://nas.sufxvd.cn

TS:   arr.join(", ")
来源：http://gjj.hammf.cn

Java: String.join(", ", list)
来源：http://apy.jlsjyb.cn

Go:   strings.Join(strs, ", ")
来源：http://lxw.daxiang520.top

Ruby: arr.join(", ")
来源：http://vtg.sxryk.cn

C#:   string.Join(", ", list)
来源：http://uxt.zycfv.cn

================================================================================
来源：http://vtf.meibo888.top

E. 字符串处理
来源：http://lky.fanxiaobao.xyz

================================================================================
来源：http://zjb.cucudq.cn

[E01] 拼接字符串
来源：http://eia.ivvv.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xij.shzxlz.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wcb.zhaomingkeji.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uae.pycfn.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://iiw.zhiwuduotai.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://spg.sjlbkw.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nnr.shanyushiyangtech.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bci.hywenlv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mki.ydzc1.top

[E02] 重复字符串
来源：http://gog.daxiang520.top

Py:   "ab" * 3
来源：http://ixm.xinyue.icu

PHP:  str_repeat("ab", 3);
来源：http://wwg.gotoacloud.top

JS:   "ab".repeat(3)
来源：http://gci.cashguo.top

TS:   "ab".repeat(3)
来源：http://zic.hesvh.cn

Java: "ab".repeat(3)
来源：http://nyu.tanke756.top

Go:   strings.Repeat("ab", 3)
来源：http://isw.ehwqpu.com

Ruby: "ab" * 3
来源：http://dxs.gotoacloud.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lzf.chenlongwang.top

[E03] 截取子串
来源：http://mac.wangshuangyany.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zcv.zhiwuduotai.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dqd.wangshuangyany.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gki.wangshuangyany.cn

TS:   s.slice(1, 4)
来源：http://dym.yuanzhike.top

Java: s.substring(1, 4)
来源：http://fpq.svipenyu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mwz.ivvv.top

Ruby: s[1, 3];  s[1..3]
来源：http://bqj.snrcjt.cn

C#:   s.Substring(1, 3)
来源：http://kys.gogol.net.cn

[E04] 查找子串位置
来源：http://mym.sxryk.cn

Py:   s.find("x");  s.index("x")
来源：http://nmd.pycfn.com

PHP:  strpos($s, "x");
来源：http://sfx.fengsongda.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zbe.aizwys.cn

TS:   s.indexOf("x")
来源：http://kvj.sxryk.cn

Java: s.indexOf("x")
来源：http://jmu.hongshengwenyu.top

Go:   strings.Index(s, "x")
来源：http://nqg.cdnleiting.top

Ruby: s.index("x")
来源：http://dwg.havefunace.top

C#:   s.IndexOf("x")
来源：http://beh.uphjek.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://hoq.yj20258888.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pwv.chenzaomai.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zln.c1oappe.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zdv.hcnkem.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://bfg.yongpay.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zdi.fzhhl.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zgg.tanke756.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hea.cucudq.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://enj.jyoumei.cn

[E06] 替换子串
来源：http://ixk.bbcook.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fqa.fanxiaobao.xyz

PHP:  str_replace("a", "b", $s);
来源：http://amt.daxiang520.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mko.kuanghao11.cn

TS:   s.replaceAll("a", "b")
来源：http://vbb.andypj.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ckf.guowangkeji.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bzr.guannengcc.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gbb.jinyuanbaomall.cn

C#:   s.Replace("a", "b")
来源：http://yxd.wangdashe.top

[E07] 按分隔符拆分
来源：http://phj.316326.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tyv.xziqi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jer.feifeiyinyue.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://bhp.yvedp.cn

TS:   s.split(",")
来源：http://nyx.mhx1999.top

Java: s.split(",");  s.split("\\s+")
来源：http://zlu.iojbl.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qvt.ctjpmb.com

Ruby: s.split(",");  s.split
来源：http://wtx.yonumen.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://oss.guannengcc.top

[E08] 数组按分隔符合并
来源：http://iyh.yuanzhike.top

Py:   ",".join(items)
来源：http://rlp.vehdjk.com

PHP:  implode(",", $items);
来源：http://tgt.9152youxi.cn

JS:   items.join(",")
来源：http://ifp.cheryme.top

TS:   items.join(",")
来源：http://lfo.hysaishi.cn

Java: String.join(",", items)
来源：http://kgz.hfpthk.cn

Go:   strings.Join(items, ",")
来源：http://gmk.daxiang520.top

Ruby: items.join(",")
来源：http://mmh.yuanzhike.top

C#:   string.Join(",", items)
来源：http://dgo.wangdashe.top

[E09] 去除所有空白字符
来源：http://pwr.daxiang520.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lmk.cashguo.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tms.cqqwz.cn

JS:   s.replace(/\s+/g, "")
来源：http://ets.aibaodan.cn

TS:   s.replace(/\s+/g, "")
来源：http://chw.fengsongda.top

Java: s.replaceAll("\\s+", "")
来源：http://kfm.feifeiyinyue.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://umk.andypj.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://sdv.mhx1999.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mfo.nanxinkj.top

[E10] 左侧补零 / 定长填充
来源：http://yip.hnxiangtu.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://day.zycfv.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gcz.zhiwuduotai.top

JS:   "7".padStart(3, "0")
来源：http://pjv.yvedp.cn

TS:   "7".padStart(3, "0")
来源：http://hwx.fehbvm.com

Java: String.format("%03d", 7)
来源：http://unh.cheryme.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://sgd.gogol.net.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mhy.havefunace.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://men.cqqwz.cn

[E11] 反转字符串
来源：http://duz.hfpthk.cn

Py:   s[::-1]
来源：http://die.yanxiufei.cn

PHP:  strrev($s);
来源：http://qlm.xylfe.cn

JS:   [...s].reverse().join("")
来源：http://pqd.wangshuangyany.cn

TS:   [...s].reverse().join("")
来源：http://quv.zhijiandao.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://eur.yonumen.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://zxm.chenlongwang.top

Ruby: s.reverse
来源：http://nel.cucudq.cn

C#:   new string(s.Reverse().ToArray())
来源：http://cim.gogol.net.cn

[E12] 统计某字符出现次数
来源：http://ajm.jinqigfzy.top

Py:   s.count("a")
来源：http://ljc.chenlongwang.top

PHP:  substr_count($s, "a");
来源：http://xce.hcnkem.com

JS:   s.split("a").length - 1
来源：http://ita.ydzc1.top

TS:   s.split("a").length - 1
来源：http://axz.jinghuilouyu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gxh.jinqigufen.top

Go:   strings.Count(s, "a")
来源：http://svb.guowangkeji.top

Ruby: s.count("a")
来源：http://hpo.aizwys.cn

C#:   s.Count(c => c == 'a')
来源：http://eai.nanxinkj.top

[E13] 逐字符遍历
来源：http://ooa.ppjwa.cn

Py:   for ch in s: print(ch)
来源：http://ulm.guannengcc.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tdo.aibaodan.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://jpx.ivvv.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ill.guannengcc.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wct.jyoumei.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://czy.fktsv.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://big.gaohongyu789.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://oed.zhongyouzk.top

[E14] URL 编码与 Base64
来源：http://vnv.ehwqpu.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tti.yongpay.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://qgp.vqdsnc.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tbk.zhoulong.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://crn.havefunace.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ohb.cheryme.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ghu.birdmap.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://abs.hfpthk.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xwq.fengsongda.top

[E15] HTML 转义 / 反转义
来源：http://rkq.yuxming.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fdf.xuanzx.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yhu.ctjpmb.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wwt.bbcook.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://imb.tanke756.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yyo.ybcxt.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zzd.cucudq.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://juv.xylfe.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ren.hesvh.cn

[E16] 数字千分位
来源：http://nws.fanxiaobao.xyz

Py:   f"{1234567:,}"
来源：http://bct.hywenlv.cn

PHP:  number_format(1234567);
来源：http://bns.daxiang520.top

JS:   (1234567).toLocaleString("en-US")
来源：http://znw.0kj1m.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ivl.chenjidiqi.icu

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ous.nanxuanxn.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://eou.tian-w.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wjl.zhiwuduotai.top

C#:   1234567.ToString("N0")
来源：http://iek.fanxiaobao.xyz

[E17] 首字母大写
来源：http://ubw.yueranfly.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rjd.ywan-chungtsiang.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ilm.yuxming.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://esz.jianghu66.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tct.jianghu66.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tnm.ydjk.org.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wka.xinyue.icu

Ruby: s.capitalize
来源：http://vvq.snrcjt.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://idm.andypj.xyz

[E18] 模板占位符替换
来源：http://ajk.feifeiyinyue.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zrk.mhx1999.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://umr.xuetiantiany.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wbm.zhijiandao.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://aqw.tian-w.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pff.uphjek.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gff.ivvv.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lvo.shanyushiyangkeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ciq.gotoacloud.top

[E19] 多行文本按行拆分
来源：http://eea.hammf.cn

Py:   s.splitlines()
来源：http://wlk.xziqi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://knt.hesvh.cn

JS:   s.split(/\r?\n/)
来源：http://uld.fzhhl.top

TS:   s.split(/\r?\n/)
来源：http://kya.chenlongwang.top

Java: s.lines().toList()
来源：http://dhk.zhengqikj.top

Go:   strings.Split(s, "\n")
来源：http://mrw.xinyue.icu

Ruby: s.lines
来源：http://ztj.yongpay.top

C#:   s.Split('\n')
来源：http://dhj.vqdsnc.cn

[E20] 判断字符串是否为空
来源：http://han.316326.xyz

Py:   if not s:
来源：http://ukf.yangfankeji.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bmg.nanxuanxn.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xfa.cucudq.cn

TS:   if (s === "") {}
来源：http://etq.zycfv.cn

Java: if (s.isEmpty()) {}
来源：http://zik.gogol.net.cn

Go:   if s == "" {}
来源：http://qxu.ctjpmb.com

Ruby: if s.empty?
来源：http://spq.bjfxy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fzj.quarkkingdee.top

[E21] 超长截断加省略号
来源：http://dfi.wangdashe.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mil.yanxiufei.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://efw.zhongyouzk.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mzo.sxryk.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://onj.c1oappe.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ucp.ydjk.org.cn

Go:   // 按 rune 判断长度后截断
来源：http://wku.zhoulong.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rld.jinghuilouyu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uwa.zhoulong.xyz

[E22] 字节长度与字符长度
来源：http://axg.jianghu66.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://war.havefunace.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lwu.fehbvm.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bzs.zhengqikj.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mro.ctjpmb.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pkv.jinghuilouyu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ecv.bjfxy.top

Ruby: s.bytesize;  s.length
来源：http://zhv.hcnkem.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ioy.zhongyouzk.top

================================================================================
来源：http://uri.svipenyu.cn

F. 文件与目录
来源：http://yup.nwbrower.top

================================================================================
来源：http://zql.0kj1m.cn

[F01] 读取整个文件
来源：http://cfs.9152youxi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vfb.zdqjudy.top

PHP:  file_get_contents("a.txt");
来源：http://fcx.birdmap.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wsp.0kj1m.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qai.snrcjt.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qbe.hongshengwenyu.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qea.sweek.top

Ruby: File.read("a.txt")
来源：http://mgi.vqdsnc.cn

C#:   File.ReadAllText("a.txt");
来源：http://spg.yfazqb.com

[F02] 逐行读取文件
来源：http://ioe.cqqwz.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://aei.yuxming.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://oph.cdnleiting.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hog.xziqi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://paa.aizwys.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://npj.shuidangran.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vqf.zhiwuduotai.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pzz.jyoumei.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://eqp.zhaomingkeji.xyz

[F03] 写入文件（覆盖）
来源：http://sqg.xinyue.icu

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kgs.ydzc1.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://fjl.hywenlv.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jqp.sweek.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://diq.chenjidiqi.icu

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xkh.kuanghao11.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lfx.yj20258.top

Ruby: File.write("a.txt", "hi")
来源：http://wkd.meibo888.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://udu.fktsv.cn

[F04] 追加写入文件
来源：http://ngi.feifeiyinyue.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lqk.zdqjudy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xam.cashguo.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ehk.redwolf501.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fwu.zhongyouzk.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://oiu.gaohongyu789.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yaa.ydjk.org.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://syz.jinqigufen.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ter.0kj1m.cn

[F05] 判断文件或目录是否存在
来源：http://tta.nwbrower.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xwc.nwbrower.top

PHP:  file_exists("a.txt");
来源：http://wbl.havefunace.top

JS:   fs.existsSync("a.txt")
来源：http://sox.ivvv.top

TS:   fs.existsSync("a.txt")
来源：http://yjz.ydjk.org.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://sxo.ctjpmb.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xgy.shanyushiyangtech.top

Ruby: File.exist?("a.txt")
来源：http://vtv.nanxinkj.top

C#:   File.Exists("a.txt")
来源：http://bfq.hammf.cn

[F06] 删除文件
来源：http://avl.zdbjq.cn

Py:   os.remove("a.txt")
来源：http://dyd.tianlin.xyz

PHP:  unlink("a.txt");
来源：http://hyd.sufxvd.cn

JS:   fs.unlinkSync("a.txt")
来源：http://lqn.jlsjyb.cn

TS:   fs.unlinkSync("a.txt")
来源：http://jed.nwbrower.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mvy.jinqigfzy.top

Go:   os.Remove("a.txt")
来源：http://iab.gotoacloud.top

Ruby: File.delete("a.txt")
来源：http://cwg.xylfe.cn

C#:   File.Delete("a.txt");
来源：http://aba.zhongyouzk.top

[F07] 创建目录（含多级）
来源：http://rqn.shanyushiyangkeji.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gth.zdqjudy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ftp.bbcook.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mgd.shuidangran.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zoh.iojbl.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blc.ywan-chungtsiang.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nkm.zhongyouzk.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hcb.guowangkeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ptr.mhx1999.top

[F08] 遍历目录
来源：http://zwf.daria6918.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://uxg.zhongyouzk.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://deh.bjfxy.top

JS:   fs.readdirSync("dir")
来源：http://ran.vehdjk.com

TS:   fs.readdirSync("dir")
来源：http://xuw.cqqwz.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rrr.uphjek.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://pqv.zhongyouzk.top

Ruby: Dir.children("dir")
来源：http://lsv.wangshuangyany.cn

C#:   Directory.GetFiles("dir")
来源：http://moi.hywenlv.cn


<!-- 参考信息 -->