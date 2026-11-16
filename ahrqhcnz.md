代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://osp.jyoumei.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://asl.ydjk.org.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bhd.hnxiangtu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dkg.c1oappe.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://elk.uphjek.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vim.zhixingplan.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zip.xziqi.cn

[D26] 数组转字符串
来源：http://ypg.sxryk.cn

Py:   ", ".join(map(str, arr))
来源：http://uph.fktsv.cn

PHP:  implode(", ", $arr);
来源：http://bmv.hammf.cn

JS:   arr.join(", ")
来源：http://hev.jqgufenzy.top

TS:   arr.join(", ")
来源：http://nrc.jinqigfzy.top

Java: String.join(", ", list)
来源：http://hbt.fehbvm.com

Go:   strings.Join(strs, ", ")
来源：http://cwt.gotoacloud.top

Ruby: arr.join(", ")
来源：http://kno.hcnkem.com

C#:   string.Join(", ", list)
来源：http://ppx.cucudq.cn

================================================================================
来源：http://hhj.haohaochexian.top

E. 字符串处理
来源：http://okn.hammf.cn

================================================================================
来源：http://ucd.shuidangran.top

[E01] 拼接字符串
来源：http://pvk.ydzc1.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vmp.jinyuanbaomall.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zzm.sysykeji.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ttw.svipenyu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fwm.yj20258888.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uvh.shanyushiyangkeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wwh.ydjk.org.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vsr.gotoacloud.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rpq.ywan-chungtsiang.top

[E02] 重复字符串
来源：http://jrt.quarkkingdee.top

Py:   "ab" * 3
来源：http://wkv.vehdjk.com

PHP:  str_repeat("ab", 3);
来源：http://tbz.gaohongyu789.top

JS:   "ab".repeat(3)
来源：http://sgz.hesvh.cn

TS:   "ab".repeat(3)
来源：http://etp.dashuyun.cn

Java: "ab".repeat(3)
来源：http://hoy.shuidangran.top

Go:   strings.Repeat("ab", 3)
来源：http://tfj.vqdsnc.cn

Ruby: "ab" * 3
来源：http://gmm.yuxming.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://boy.redwolf501.top

[E03] 截取子串
来源：http://qof.haohaochexian.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rjz.yuanzhike.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://boi.yvedp.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ywf.iojbl.cn

TS:   s.slice(1, 4)
来源：http://enu.xuanzx.com

Java: s.substring(1, 4)
来源：http://bha.mhx1999.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qmk.xylfe.cn

Ruby: s[1, 3];  s[1..3]
来源：http://sew.vqdsnc.cn

C#:   s.Substring(1, 3)
来源：http://ais.aizwys.cn

[E04] 查找子串位置
来源：http://pil.epnwcf.com

Py:   s.find("x");  s.index("x")
来源：http://auu.aibaodan.cn

PHP:  strpos($s, "x");
来源：http://kqa.feifeiyinyue.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yav.vehdjk.com

TS:   s.indexOf("x")
来源：http://ghu.bjfxy.top

Java: s.indexOf("x")
来源：http://cgm.kuanghao11.cn

Go:   strings.Index(s, "x")
来源：http://rmu.fehbvm.com

Ruby: s.index("x")
来源：http://izn.dianchejie.cn

C#:   s.IndexOf("x")
来源：http://igb.sufxvd.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://cps.zhiwuduotai.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cpe.cdnleiting.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hsy.jinqigufen.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wav.c1oappe.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://dgk.pycfn.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wwf.9152youxi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://war.epnwcf.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://frv.guannengcc.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kay.daria6918.cn

[E06] 替换子串
来源：http://qud.shanyushiyangkeji.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://izt.jinqigfzy.top

PHP:  str_replace("a", "b", $s);
来源：http://ahw.zhoulong.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ygs.vehdjk.com

TS:   s.replaceAll("a", "b")
来源：http://xmt.jiagoushi.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jwx.sufxvd.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hij.shuidangran.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wpz.zdqjudy.top

C#:   s.Replace("a", "b")
来源：http://faa.hysaishi.cn

[E07] 按分隔符拆分
来源：http://wqo.tarul.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fwy.zhoulong.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xuf.fengsongda.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://rhh.guannengcc.top

TS:   s.split(",")
来源：http://ihs.zhoulong.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://yzs.haohaochexian.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kaa.jqgufenzy.top

Ruby: s.split(",");  s.split
来源：http://pwu.hesvh.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://geh.ybcxt.top

[E08] 数组按分隔符合并
来源：http://uxy.ybcxt.top

Py:   ",".join(items)
来源：http://atu.0kj1m.cn

PHP:  implode(",", $items);
来源：http://ezu.fengsongda.top

JS:   items.join(",")
来源：http://rlm.mhx1999.top

TS:   items.join(",")
来源：http://gdf.ivvv.top

Java: String.join(",", items)
来源：http://feb.tanke756.top

Go:   strings.Join(items, ",")
来源：http://lgj.quarkkingdee.top

Ruby: items.join(",")
来源：http://lgw.hnxiangtu.top

C#:   string.Join(",", items)
来源：http://rug.nanxuanxn.top

[E09] 去除所有空白字符
来源：http://zte.yj20258.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kvd.chenlongwang.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xtx.kuanghao11.cn

JS:   s.replace(/\s+/g, "")
来源：http://lvr.jyoumei.cn

TS:   s.replace(/\s+/g, "")
来源：http://tsc.52xcode.cn

Java: s.replaceAll("\\s+", "")
来源：http://spx.ctjpmb.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://tsb.daxiang520.top

Ruby: s.gsub(/\s+/, "")
来源：http://xxo.ehwqpu.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pnm.pycfn.com

[E10] 左侧补零 / 定长填充
来源：http://qkb.tianlin.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lcp.snrcjt.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ifw.zhongyouzk.top

JS:   "7".padStart(3, "0")
来源：http://qid.zhijiandao.cn

TS:   "7".padStart(3, "0")
来源：http://jmr.fehbvm.com

Java: String.format("%03d", 7)
来源：http://lxh.uphjek.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://ljc.shzxlz.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vhf.xuanzx.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ydj.ctjpmb.com

[E11] 反转字符串
来源：http://boj.jlsjyb.cn

Py:   s[::-1]
来源：http://ges.guannengcc.top

PHP:  strrev($s);
来源：http://huf.gaohongyu789.top

JS:   [...s].reverse().join("")
来源：http://jdi.meibo888.top

TS:   [...s].reverse().join("")
来源：http://mjg.sxryk.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pxn.chenlongwang.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://vhp.feifeiyinyue.top

Ruby: s.reverse
来源：http://hvm.hongshengwenyu.top

C#:   new string(s.Reverse().ToArray())
来源：http://ubq.iojbl.cn

[E12] 统计某字符出现次数
来源：http://vuk.jinghuilouyu.cn

Py:   s.count("a")
来源：http://trh.c1oappe.top

PHP:  substr_count($s, "a");
来源：http://uyl.hywenlv.cn

JS:   s.split("a").length - 1
来源：http://ptj.chenlongwang.top

TS:   s.split("a").length - 1
来源：http://urr.sufxvd.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://sck.jinqigfzy.top

Go:   strings.Count(s, "a")
来源：http://vma.vqdsnc.cn

Ruby: s.count("a")
来源：http://dkl.tanke756.top

C#:   s.Count(c => c == 'a')
来源：http://pls.kuanghao11.cn

[E13] 逐字符遍历
来源：http://tmg.dashuyun.cn

Py:   for ch in s: print(ch)
来源：http://doj.tianlin.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kzo.bjfxy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://odm.sufxvd.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://nih.jinqigfzy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xfu.tanke756.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tup.tanke756.top

Ruby: s.each_char { |ch| puts ch }
来源：http://rqk.zhoulong.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://oap.zycfv.cn

[E14] URL 编码与 Base64
来源：http://mym.zdbjq.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hjs.pycfn.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://bwl.havefunace.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ung.ydzc1.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gab.gogol.net.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tmq.cashguo.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rdm.chenjidiqi.icu

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lxe.fktsv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://scq.chenzaomai.com

[E15] HTML 转义 / 反转义
来源：http://vru.cdnleiting.top

Py:   html.escape(s);  html.unescape(s)
来源：http://bpb.tian-w.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://eya.dashuyun.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sgy.tianlin.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://jtn.fktsv.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mcr.zhijiandao.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bad.meibo888.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nll.yvedp.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lyg.yongpay.top

[E16] 数字千分位
来源：http://jji.jinqigfzy.top

Py:   f"{1234567:,}"
来源：http://uwo.sufxvd.cn

PHP:  number_format(1234567);
来源：http://bll.snrcjt.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://rny.yj202588.top

TS:   (1234567).toLocaleString("en-US")
来源：http://etb.zycfv.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rqs.ywan-chungtsiang.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fne.sxryk.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ldr.smart0.xyz

C#:   1234567.ToString("N0")
来源：http://rtc.zycfv.cn

[E17] 首字母大写
来源：http://huc.vqdsnc.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vyp.sysykeji.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ger.zhixingplan.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iut.iojbl.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gov.cashguo.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rsu.shangyingyoupin.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://oqd.birdmap.top

Ruby: s.capitalize
来源：http://kxi.tianlin.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cln.yongpay.top

[E18] 模板占位符替换
来源：http://xsl.yonumen.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nba.hongshengwenyu.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ycq.yfazqb.com

JS:   tpl.replaceAll("{name}", name)
来源：http://yqx.shanyushiyangtech.top

TS:   tpl.replaceAll("{name}", name)
来源：http://nmb.fengsongda.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mep.tian-w.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://uhx.birdmap.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zfs.hcnkem.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kqg.yj202588.top

[E19] 多行文本按行拆分
来源：http://mko.hongshengwenyu.top

Py:   s.splitlines()
来源：http://wnz.yangfankeji.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tha.zdqjudy.top

JS:   s.split(/\r?\n/)
来源：http://zzy.aibaodan.cn

TS:   s.split(/\r?\n/)
来源：http://efh.jinyuanbaomall.cn

Java: s.lines().toList()
来源：http://gbd.cashguo.top

Go:   strings.Split(s, "\n")
来源：http://jdj.c1oappe.top

Ruby: s.lines
来源：http://den.shzxlz.cn

C#:   s.Split('\n')
来源：http://svp.yj202588.top

[E20] 判断字符串是否为空
来源：http://ofx.316326.xyz

Py:   if not s:
来源：http://efc.ctjpmb.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qax.hcnkem.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://myn.gotoacloud.top

TS:   if (s === "") {}
来源：http://gql.xylfe.cn

Java: if (s.isEmpty()) {}
来源：http://way.nanxinkj.top

Go:   if s == "" {}
来源：http://xha.hongshengwenyu.top

Ruby: if s.empty?
来源：http://vic.zdbjq.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hrt.meibo888.top

[E21] 超长截断加省略号
来源：http://ytu.fanxiaobao.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://foy.xziqi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qgc.aizwys.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sqr.gogol.net.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wcr.xingfuxueyuan.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bjn.zhixingplan.top

Go:   // 按 rune 判断长度后截断
来源：http://loo.smart0.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://viw.gaohongyu789.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fir.xingfuxueyuan.xyz

[E22] 字节长度与字符长度
来源：http://hcf.shangyingyoupin.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gil.fengsongda.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nnn.pycfn.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hlk.yangfankeji.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cux.fanxiaobao.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rbt.yonumen.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tty.ctjpmb.com

Ruby: s.bytesize;  s.length
来源：http://ryc.shanyushiyangkeji.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://alh.vqdsnc.cn

================================================================================
来源：http://tig.c1oappe.top

F. 文件与目录
来源：http://sej.zhixingplan.top

================================================================================
来源：http://cpd.kuanghao11.cn

[F01] 读取整个文件
来源：http://xiq.fzhhl.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qdy.zdbjq.cn

PHP:  file_get_contents("a.txt");
来源：http://seb.zdqjudy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hso.yfazqb.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://isu.yangfankeji.com

Java: Files.readString(Path.of("a.txt"))
来源：http://fdv.xinyue.icu

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ieh.svipenyu.cn

Ruby: File.read("a.txt")
来源：http://ltl.iojbl.cn

C#:   File.ReadAllText("a.txt");
来源：http://iyg.jqgfzy.top

[F02] 逐行读取文件
来源：http://cpr.zhijiandao.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lyb.wangshuangyany.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gnr.zhixingplan.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qbl.redwolf501.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rfh.guowangkeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ydc.tanke756.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xtj.aizwys.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cei.snrcjt.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mgy.yangfankeji.com

[F03] 写入文件（覆盖）
来源：http://hmq.dashuyun.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://duj.chenlongwang.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://fub.ywan-chungtsiang.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bfj.shuidangran.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xma.ehwqpu.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yuc.hywenlv.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ieh.gzhubu.top

Ruby: File.write("a.txt", "hi")
来源：http://eiu.shanyushiyangkeji.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xof.cucudq.cn

[F04] 追加写入文件
来源：http://xaj.ywan-chungtsiang.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zuk.xziqi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jbv.yuanzhike.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dxy.hesvh.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xps.vehdjk.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://riu.birdmap.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dzf.dashuyun.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tmm.cheryme.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://owr.yongpay.top

[F05] 判断文件或目录是否存在
来源：http://opt.ctjpmb.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://eyo.hnqzz.top

PHP:  file_exists("a.txt");
来源：http://vqw.ydjk.org.cn

JS:   fs.existsSync("a.txt")
来源：http://ieb.52xcode.cn

TS:   fs.existsSync("a.txt")
来源：http://wli.hesvh.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fwk.jianghu66.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zqm.cdnleiting.top

Ruby: File.exist?("a.txt")
来源：http://bpm.zhengqikj.top

C#:   File.Exists("a.txt")
来源：http://msr.zdqjudy.top

[F06] 删除文件
来源：http://fxc.ehwqpu.com

Py:   os.remove("a.txt")
来源：http://plo.hcnkem.com

PHP:  unlink("a.txt");
来源：http://ard.jlsjyb.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pzt.hysaishi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://bsn.aizwys.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nzx.ydzc1.top

Go:   os.Remove("a.txt")
来源：http://ttk.haohaochexian.top

Ruby: File.delete("a.txt")
来源：http://duq.hongshengwenyu.top

C#:   File.Delete("a.txt");
来源：http://vxl.birdmap.top

[F07] 创建目录（含多级）
来源：http://mel.jinyuanbaomall.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pik.quarkkingdee.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uxf.yfazqb.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hds.ydjk.org.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kka.uphjek.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lce.zycfv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fsz.zhixingplan.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mmm.cheryme.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mjk.yuanzhike.top

[F08] 遍历目录
来源：http://xid.yueranfly.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://zaj.fanxiaobao.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tjj.shzxlz.cn

JS:   fs.readdirSync("dir")
来源：http://kuq.hammf.cn

TS:   fs.readdirSync("dir")
来源：http://wfg.vqdsnc.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bfs.zhoulong.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://ugm.gzhubu.top

Ruby: Dir.children("dir")
来源：http://uba.zhoulong.xyz

C#:   Directory.GetFiles("dir")
来源：http://efn.wangdashe.top

[F09] 获取文件大小
来源：http://ouf.yuanzhike.top

Py:   os.path.getsize("a.txt")
来源：http://gfj.feifeiyinyue.top

PHP:  filesize("a.txt");
来源：http://ujw.shanyushiyangtech.top

JS:   fs.statSync("a.txt").size
来源：http://hvz.gogol.net.cn

TS:   fs.statSync("a.txt").size
来源：http://mqy.xylfe.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zja.fzhhl.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://swn.yongpay.top

Ruby: File.size("a.txt")
来源：http://hqf.yuxming.cn


<!-- 参考信息 -->