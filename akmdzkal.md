代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pkv.birdmap.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ntp.nwbrower.top

[D25] Set 集合去重与交并差
来源：http://xit.redwolf501.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://uas.yj202588.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xpg.uphjek.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://chl.guowangkeji.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://olz.jlsjyb.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://scf.hcnkem.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hmq.tian-w.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xxz.pengpengdd.cyou

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rsu.xuanzx.com

[D26] 数组转字符串
来源：http://ijz.yongpay.top

Py:   ", ".join(map(str, arr))
来源：http://lgn.wangshuangyany.cn

PHP:  implode(", ", $arr);
来源：http://jec.iojbl.cn

JS:   arr.join(", ")
来源：http://qiz.yangfankeji.com

TS:   arr.join(", ")
来源：http://dfp.daria6918.cn

Java: String.join(", ", list)
来源：http://cdz.yangfankeji.com

Go:   strings.Join(strs, ", ")
来源：http://ozd.ybcxt.top

Ruby: arr.join(", ")
来源：http://avx.meibo888.top

C#:   string.Join(", ", list)
来源：http://vvt.jinyuanbaomall.cn

================================================================================
来源：http://tpl.pengpengdd.cyou

E. 字符串处理
来源：http://zia.sweek.top

================================================================================
来源：http://qix.chenlongwang.top

[E01] 拼接字符串
来源：http://kxm.fzhhl.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ibm.ywan-chungtsiang.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kld.zdbjq.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hpy.hfpthk.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zer.sxryk.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tdv.hywenlv.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://han.daria6918.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hrc.hysaishi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vab.hnqzz.top

[E02] 重复字符串
来源：http://uzp.zhengqikj.top

Py:   "ab" * 3
来源：http://rve.pengpengdd.cyou

PHP:  str_repeat("ab", 3);
来源：http://zwj.ydjk.org.cn

JS:   "ab".repeat(3)
来源：http://dre.smart0.xyz

TS:   "ab".repeat(3)
来源：http://ujn.shanyushiyangkeji.top

Java: "ab".repeat(3)
来源：http://ugc.fengsongda.top

Go:   strings.Repeat("ab", 3)
来源：http://txk.meibo888.top

Ruby: "ab" * 3
来源：http://vos.guowangkeji.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zdj.yonumen.top

[E03] 截取子串
来源：http://mdh.zhongyouzk.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fyp.xylfe.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wje.ivvv.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hmf.haohaochexian.top

TS:   s.slice(1, 4)
来源：http://ill.shanyushiyangtech.top

Java: s.substring(1, 4)
来源：http://rgf.yj20258.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://onf.jinqigufen.top

Ruby: s[1, 3];  s[1..3]
来源：http://otz.316326.xyz

C#:   s.Substring(1, 3)
来源：http://vuw.sjlbkw.cn

[E04] 查找子串位置
来源：http://yly.fengsongda.top

Py:   s.find("x");  s.index("x")
来源：http://dbx.zhoulong.xyz

PHP:  strpos($s, "x");
来源：http://nux.fengsongda.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jjm.sxryk.cn

TS:   s.indexOf("x")
来源：http://inn.wangdashe.top

Java: s.indexOf("x")
来源：http://xfx.kuanghao11.cn

Go:   strings.Index(s, "x")
来源：http://zyo.hammf.cn

Ruby: s.index("x")
来源：http://rat.quarkkingdee.top

C#:   s.IndexOf("x")
来源：http://owe.cheryme.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://kxd.yueranfly.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wmv.aizwys.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cik.bjfxy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nvt.jqgufenzy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://huw.tian-w.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ovz.daxiang520.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dda.vqdsnc.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ufz.chenzaomai.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mpa.cdnleiting.top

[E06] 替换子串
来源：http://xtc.guowangkeji.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://goz.fktsv.cn

PHP:  str_replace("a", "b", $s);
来源：http://hmx.zdbjq.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eio.bbcook.cn

TS:   s.replaceAll("a", "b")
来源：http://cbt.wangshuangyany.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vek.guannengcc.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xqg.haohaochexian.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://icb.yfazqb.com

C#:   s.Replace("a", "b")
来源：http://zfg.dashuyun.cn

[E07] 按分隔符拆分
来源：http://tbt.hnqzz.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ote.sweek.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wwg.shanyushiyangtech.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://yxt.smart0.xyz

TS:   s.split(",")
来源：http://kyj.jqgfzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://qkm.yongpay.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://oih.zhijiandao.cn

Ruby: s.split(",");  s.split
来源：http://lmj.daria6918.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jnd.hcnkem.com

[E08] 数组按分隔符合并
来源：http://nno.c1oappe.top

Py:   ",".join(items)
来源：http://xxo.vqdsnc.cn

PHP:  implode(",", $items);
来源：http://fqz.xuanzx.com

JS:   items.join(",")
来源：http://yxu.mhx1999.top

TS:   items.join(",")
来源：http://kyj.yuxming.cn

Java: String.join(",", items)
来源：http://kfa.zhoulong.xyz

Go:   strings.Join(items, ",")
来源：http://nll.yj20258.top

Ruby: items.join(",")
来源：http://rjs.jinqigfzy.top

C#:   string.Join(",", items)
来源：http://fnp.haohaochexian.top

[E09] 去除所有空白字符
来源：http://jmp.jinqigufen.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lmn.kuanghao11.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kbc.ctjpmb.com

JS:   s.replace(/\s+/g, "")
来源：http://neg.bjfxy.top

TS:   s.replace(/\s+/g, "")
来源：http://jsb.fanxiaobao.xyz

Java: s.replaceAll("\\s+", "")
来源：http://yfm.guowangkeji.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://bqx.vehdjk.com

Ruby: s.gsub(/\s+/, "")
来源：http://fzv.jqgfzy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kjy.xingfuxueyuan.xyz

[E10] 左侧补零 / 定长填充
来源：http://pub.jianghu66.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ftp.xingfuxueyuan.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rtg.birdmap.top

JS:   "7".padStart(3, "0")
来源：http://gmf.aibaodan.cn

TS:   "7".padStart(3, "0")
来源：http://ibh.iojbl.cn

Java: String.format("%03d", 7)
来源：http://szm.bjfxy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ahd.0kj1m.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gti.yueranfly.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tqc.cheryme.top

[E11] 反转字符串
来源：http://jhf.9152youxi.cn

Py:   s[::-1]
来源：http://sgg.ctjpmb.com

PHP:  strrev($s);
来源：http://rig.hcnkem.com

JS:   [...s].reverse().join("")
来源：http://lfm.xingfuxueyuan.xyz

TS:   [...s].reverse().join("")
来源：http://esi.xylfe.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://lxg.ppjwa.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jap.daxiang520.top

Ruby: s.reverse
来源：http://rix.yanxiufei.cn

C#:   new string(s.Reverse().ToArray())
来源：http://dwa.sweek.top

[E12] 统计某字符出现次数
来源：http://btd.jlsjyb.cn

Py:   s.count("a")
来源：http://fuh.chenzaomai.com

PHP:  substr_count($s, "a");
来源：http://unh.nanxinkj.top

JS:   s.split("a").length - 1
来源：http://vyo.smart0.xyz

TS:   s.split("a").length - 1
来源：http://xfk.cqqwz.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pug.zhiwuduotai.top

Go:   strings.Count(s, "a")
来源：http://hpc.xingfuxueyuan.xyz

Ruby: s.count("a")
来源：http://hkg.hfpthk.cn

C#:   s.Count(c => c == 'a')
来源：http://phc.vehdjk.com

[E13] 逐字符遍历
来源：http://cft.ctjpmb.com

Py:   for ch in s: print(ch)
来源：http://fhe.shzxlz.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qmx.xuanzx.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://fme.vehdjk.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://adg.tian-w.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ubx.snrcjt.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ynn.xziqi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qle.wangdashe.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fxe.yonumen.top

[E14] URL 编码与 Base64
来源：http://qnp.guannengcc.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://omz.xuanzx.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://rpp.zhengqikj.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://knd.ybcxt.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xgi.pengpengdd.cyou

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kjp.cashguo.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jgi.hammf.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rxo.nanxinkj.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hcw.cheryme.top

[E15] HTML 转义 / 反转义
来源：http://woy.snrcjt.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hsv.gzhubu.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pqd.vqdsnc.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dta.tanke756.top

TS:   // 同上，务必做 XSS 过滤
来源：http://yhf.jinghuilouyu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wya.bjfxy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uur.jlsjyb.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mxd.xuetiantiany.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bjz.ydzc1.top

[E16] 数字千分位
来源：http://mxd.hnxiangtu.top

Py:   f"{1234567:,}"
来源：http://wfh.cucudq.cn

PHP:  number_format(1234567);
来源：http://kis.zycfv.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ocx.aizwys.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://huz.zhoulong.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://oih.ydjk.org.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://avx.fengsongda.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uml.shanyushiyangtech.top

C#:   1234567.ToString("N0")
来源：http://dpj.nanxinkj.top

[E17] 首字母大写
来源：http://jup.zdqjudy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xtn.guannengcc.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://etr.gaohongyu789.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mfn.haohaochexian.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lyb.xinyue.icu

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gzi.yongpay.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fut.haohaochexian.top

Ruby: s.capitalize
来源：http://hcf.yj20258888.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dvk.wangshuangyany.cn

[E18] 模板占位符替换
来源：http://xqd.sxryk.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tam.shzxlz.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fie.yueranfly.top

JS:   tpl.replaceAll("{name}", name)
来源：http://vjb.zdbjq.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://epw.yuanzhike.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rkd.yj20258.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lej.jinqigfzy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lnb.ctjpmb.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cmw.xziqi.cn

[E19] 多行文本按行拆分
来源：http://eio.hcnkem.com

Py:   s.splitlines()
来源：http://dal.chenzaomai.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://roh.cashguo.top

JS:   s.split(/\r?\n/)
来源：http://ggp.xuanzx.com

TS:   s.split(/\r?\n/)
来源：http://xxx.yangfankeji.com

Java: s.lines().toList()
来源：http://eqw.jqgufenzy.top

Go:   strings.Split(s, "\n")
来源：http://snk.yongpay.top

Ruby: s.lines
来源：http://nnr.jinghuilouyu.cn

C#:   s.Split('\n')
来源：http://joe.tianlin.xyz

[E20] 判断字符串是否为空
来源：http://nyc.hysaishi.cn

Py:   if not s:
来源：http://mrx.hesvh.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://omj.hammf.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dnz.vqdsnc.cn

TS:   if (s === "") {}
来源：http://wcm.yonumen.top

Java: if (s.isEmpty()) {}
来源：http://odm.shanyushiyangtech.top

Go:   if s == "" {}
来源：http://nmb.chenzaomai.com

Ruby: if s.empty?
来源：http://vha.fengsongda.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wrk.ivvv.top

[E21] 超长截断加省略号
来源：http://wnd.ybcxt.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://oot.tian-w.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://iiz.tianlin.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wvr.xuetiantiany.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ckj.gotoacloud.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kcm.hcnkem.com

Go:   // 按 rune 判断长度后截断
来源：http://mic.feifeiyinyue.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://izw.feifeiyinyue.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tbq.zycfv.cn

[E22] 字节长度与字符长度
来源：http://sfa.yonumen.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tzq.zhoulong.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vrr.xingfuxueyuan.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nbl.jlsjyb.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sot.havefunace.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://iwj.shuidangran.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://req.vehdjk.com

Ruby: s.bytesize;  s.length
来源：http://ljr.hfpthk.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lzf.hnxiangtu.top

================================================================================
来源：http://hve.jqgufenzy.top

F. 文件与目录
来源：http://bwd.shanyushiyangtech.top

================================================================================
来源：http://bdf.tanke756.top

[F01] 读取整个文件
来源：http://sxh.havefunace.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tql.meibo888.top

PHP:  file_get_contents("a.txt");
来源：http://pcn.yonumen.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bar.tian-w.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://myk.jiagoushi.top

Java: Files.readString(Path.of("a.txt"))
来源：http://dco.yj20258.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xiz.andypj.xyz

Ruby: File.read("a.txt")
来源：http://ieo.sysykeji.top

C#:   File.ReadAllText("a.txt");
来源：http://qea.vqdsnc.cn

[F02] 逐行读取文件
来源：http://bgo.zhengqikj.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mtl.yuanzhike.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ggz.zdbjq.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kvi.tianlin.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wid.shanyushiyangkeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kfc.pycfn.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vim.epnwcf.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zhp.hnqzz.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://suf.hongshengwenyu.top

[F03] 写入文件（覆盖）
来源：http://nqq.yongpay.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wfz.xylfe.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://kmp.xuetiantiany.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dkh.dashuyun.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qgx.sysykeji.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ikc.hysaishi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sqi.havefunace.top

Ruby: File.write("a.txt", "hi")
来源：http://nge.cashguo.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ycg.c1oappe.top

[F04] 追加写入文件
来源：http://vxg.pengpengdd.cyou

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gsf.ctjpmb.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jrx.yfazqb.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dxz.fehbvm.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dvf.ydzc1.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kgq.yongpay.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://eil.chenzaomai.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jus.ivvv.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ozb.bbcook.cn

[F05] 判断文件或目录是否存在
来源：http://dif.chenzaomai.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wds.zycfv.cn

PHP:  file_exists("a.txt");
来源：http://xlc.hammf.cn

JS:   fs.existsSync("a.txt")
来源：http://vba.wangdashe.top

TS:   fs.existsSync("a.txt")
来源：http://bpj.yj202588.top

Java: Files.exists(Path.of("a.txt"))
来源：http://fcb.yongpay.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kbu.feifeiyinyue.top

Ruby: File.exist?("a.txt")
来源：http://dee.hnxiangtu.top

C#:   File.Exists("a.txt")
来源：http://cpj.ctjpmb.com

[F06] 删除文件
来源：http://ixu.hfpthk.cn

Py:   os.remove("a.txt")
来源：http://psx.hywenlv.cn

PHP:  unlink("a.txt");
来源：http://qtz.gaohongyu789.top

JS:   fs.unlinkSync("a.txt")
来源：http://dej.yj20258.top

TS:   fs.unlinkSync("a.txt")
来源：http://mms.yj202588.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dcr.hammf.cn

Go:   os.Remove("a.txt")
来源：http://qlm.hnqzz.top

Ruby: File.delete("a.txt")
来源：http://tgj.sjlbkw.cn

C#:   File.Delete("a.txt");
来源：http://qoc.gzhubu.top

[F07] 创建目录（含多级）
来源：http://cvu.yj20258888.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ckl.ppjwa.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jmd.zhijiandao.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ouw.yuxming.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://crm.hammf.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://odd.haohaochexian.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ulz.kuanghao11.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dux.daxiang520.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://iws.dashuyun.cn

[F08] 遍历目录
来源：http://xvy.pengpengdd.cyou

Py:   for name in os.listdir("dir"): print(name)
来源：http://cfi.redwolf501.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gej.ybcxt.top

JS:   fs.readdirSync("dir")
来源：http://jxv.pengpengdd.cyou

TS:   fs.readdirSync("dir")
来源：http://pka.gogol.net.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dzh.aizwys.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xtw.wangdashe.top

Ruby: Dir.children("dir")
来源：http://thz.wangdashe.top

C#:   Directory.GetFiles("dir")
来源：http://jfp.jinqigufen.top

[F09] 获取文件大小
来源：http://snq.zhengqikj.top

Py:   os.path.getsize("a.txt")
来源：http://wsc.chenzaomai.com

PHP:  filesize("a.txt");
来源：http://syb.tianlin.xyz

JS:   fs.statSync("a.txt").size
来源：http://fpo.gogol.net.cn


<!-- 参考信息 -->