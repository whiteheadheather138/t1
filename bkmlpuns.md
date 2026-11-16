代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dud.tarul.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://egd.fktsv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vzp.shanyushiyangkeji.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://txo.tianlin.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kru.jinyuanbaomall.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cdv.hywenlv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bsq.yueranfly.top

[D26] 数组转字符串
来源：http://xcn.hysaishi.cn

Py:   ", ".join(map(str, arr))
来源：http://xyo.gogol.net.cn

PHP:  implode(", ", $arr);
来源：http://fnn.jinghuilouyu.cn

JS:   arr.join(", ")
来源：http://zes.zdqjudy.top

TS:   arr.join(", ")
来源：http://gzv.bjfxy.top

Java: String.join(", ", list)
来源：http://kji.quarkkingdee.top

Go:   strings.Join(strs, ", ")
来源：http://ehd.pengpengdd.cyou

Ruby: arr.join(", ")
来源：http://eiu.shanyushiyangkeji.top

C#:   string.Join(", ", list)
来源：http://dbj.feifeiyinyue.top

================================================================================
来源：http://mec.hywenlv.cn

E. 字符串处理
来源：http://lkw.redwolf501.top

================================================================================
来源：http://wog.gogol.net.cn

[E01] 拼接字符串
来源：http://hkl.zhijiandao.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ijc.yueranfly.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ozj.sweek.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lhs.dianchejie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ikw.epnwcf.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qou.hammf.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vru.hcnkem.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fss.xuetiantiany.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bvm.gogol.net.cn

[E02] 重复字符串
来源：http://uyt.hnqzz.top

Py:   "ab" * 3
来源：http://idn.fzhhl.top

PHP:  str_repeat("ab", 3);
来源：http://qsb.dianchejie.cn

JS:   "ab".repeat(3)
来源：http://qgu.ybcxt.top

TS:   "ab".repeat(3)
来源：http://nwi.zhongyouzk.top

Java: "ab".repeat(3)
来源：http://sju.yangfankeji.com

Go:   strings.Repeat("ab", 3)
来源：http://qwk.cqqwz.cn

Ruby: "ab" * 3
来源：http://zjb.jianghu66.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yem.tian-w.cn

[E03] 截取子串
来源：http://rxc.dashuyun.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pnm.cheryme.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://woi.epnwcf.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://giv.gaohongyu789.top

TS:   s.slice(1, 4)
来源：http://dex.feifeiyinyue.top

Java: s.substring(1, 4)
来源：http://xsl.9152youxi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bse.ybcxt.top

Ruby: s[1, 3];  s[1..3]
来源：http://ayz.yfazqb.com

C#:   s.Substring(1, 3)
来源：http://ixd.xuetiantiany.cn

[E04] 查找子串位置
来源：http://hfi.aibaodan.cn

Py:   s.find("x");  s.index("x")
来源：http://nkd.nanxinkj.top

PHP:  strpos($s, "x");
来源：http://jyv.jinghuilouyu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vhh.52xcode.cn

TS:   s.indexOf("x")
来源：http://coa.uphjek.com

Java: s.indexOf("x")
来源：http://sdh.yj202588.top

Go:   strings.Index(s, "x")
来源：http://xdh.jinqigfzy.top

Ruby: s.index("x")
来源：http://psr.tian-w.cn

C#:   s.IndexOf("x")
来源：http://bet.xziqi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://mwk.haohaochexian.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fon.xziqi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fan.ehwqpu.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aut.xylfe.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kdt.ivvv.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zsq.ivvv.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ymk.gotoacloud.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dwb.ydzc1.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://czi.ivvv.top

[E06] 替换子串
来源：http://loj.kuanghao11.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kdp.zhijiandao.cn

PHP:  str_replace("a", "b", $s);
来源：http://hgx.jiagoushi.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xbx.hysaishi.cn

TS:   s.replaceAll("a", "b")
来源：http://nbn.bbcook.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://buu.bjfxy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fit.chenlongwang.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lqz.hywenlv.cn

C#:   s.Replace("a", "b")
来源：http://sxk.meibo888.top

[E07] 按分隔符拆分
来源：http://tcd.jianghu66.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yqv.9152youxi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vqw.gotoacloud.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://csm.shanyushiyangkeji.top

TS:   s.split(",")
来源：http://gse.yj202588.top

Java: s.split(",");  s.split("\\s+")
来源：http://tbn.hnxiangtu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://epa.bjfxy.top

Ruby: s.split(",");  s.split
来源：http://tmo.sjlbkw.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lxg.pengpengdd.cyou

[E08] 数组按分隔符合并
来源：http://bbg.jyoumei.cn

Py:   ",".join(items)
来源：http://fzu.nwbrower.top

PHP:  implode(",", $items);
来源：http://hxz.hesvh.cn

JS:   items.join(",")
来源：http://sgg.ivvv.top

TS:   items.join(",")
来源：http://erw.9152youxi.cn

Java: String.join(",", items)
来源：http://mot.jianghu66.top

Go:   strings.Join(items, ",")
来源：http://cjp.hnxiangtu.top

Ruby: items.join(",")
来源：http://paj.vehdjk.com

C#:   string.Join(",", items)
来源：http://hii.zhixingplan.top

[E09] 去除所有空白字符
来源：http://fwv.yonumen.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ajn.gzhubu.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tig.cashguo.top

JS:   s.replace(/\s+/g, "")
来源：http://osj.jinyuanbaomall.cn

TS:   s.replace(/\s+/g, "")
来源：http://zqd.hfpthk.cn

Java: s.replaceAll("\\s+", "")
来源：http://pnm.shangyingyoupin.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://vyt.jlsjyb.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gah.hnxiangtu.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mca.fzhhl.top

[E10] 左侧补零 / 定长填充
来源：http://bvp.jinyuanbaomall.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zol.hongshengwenyu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://puo.yj20258888.top

JS:   "7".padStart(3, "0")
来源：http://zhm.ivvv.top

TS:   "7".padStart(3, "0")
来源：http://oru.shuidangran.top

Java: String.format("%03d", 7)
来源：http://mue.cucudq.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ctf.meibo888.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jqh.hammf.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ufv.tianlin.xyz

[E11] 反转字符串
来源：http://ged.dashuyun.cn

Py:   s[::-1]
来源：http://bna.cqqwz.cn

PHP:  strrev($s);
来源：http://pdg.shzxlz.cn

JS:   [...s].reverse().join("")
来源：http://vgj.chenlongwang.top

TS:   [...s].reverse().join("")
来源：http://opi.daxiang520.top

Java: new StringBuilder(s).reverse().toString()
来源：http://nce.ehwqpu.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://dnn.yonumen.top

Ruby: s.reverse
来源：http://daf.jqgufenzy.top

C#:   new string(s.Reverse().ToArray())
来源：http://crc.pycfn.com

[E12] 统计某字符出现次数
来源：http://znt.jyoumei.cn

Py:   s.count("a")
来源：http://myi.aibaodan.cn

PHP:  substr_count($s, "a");
来源：http://vsb.ppjwa.cn

JS:   s.split("a").length - 1
来源：http://clp.uphjek.com

TS:   s.split("a").length - 1
来源：http://lpb.zycfv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ily.fanxiaobao.xyz

Go:   strings.Count(s, "a")
来源：http://npd.jyoumei.cn

Ruby: s.count("a")
来源：http://bol.dianchejie.cn

C#:   s.Count(c => c == 'a')
来源：http://dqf.quarkkingdee.top

[E13] 逐字符遍历
来源：http://fxz.yuanzhike.top

Py:   for ch in s: print(ch)
来源：http://hev.zdqjudy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bcq.chenzaomai.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://aye.cqqwz.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://hbr.zhijiandao.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wgb.sxryk.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jei.sxryk.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://txc.gotoacloud.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rtv.zhijiandao.cn

[E14] URL 编码与 Base64
来源：http://lbx.shangyingyoupin.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ekt.yfazqb.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://ezh.nanxuanxn.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://eut.haohaochexian.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jzs.yfazqb.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cqe.zhengqikj.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dic.nanxuanxn.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hjk.birdmap.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fqg.daxiang520.top

[E15] HTML 转义 / 反转义
来源：http://ixj.jianghu66.top

Py:   html.escape(s);  html.unescape(s)
来源：http://smu.jlsjyb.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nun.fanxiaobao.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kbk.fzhhl.top

TS:   // 同上，务必做 XSS 过滤
来源：http://hfq.uphjek.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://oyq.c1oappe.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ufj.jiagoushi.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lov.0kj1m.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://opu.ybcxt.top

[E16] 数字千分位
来源：http://alr.jqgufenzy.top

Py:   f"{1234567:,}"
来源：http://yoa.cqqwz.cn

PHP:  number_format(1234567);
来源：http://zfc.yanxiufei.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://oad.cqqwz.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://key.yuanzhike.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lek.fktsv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yoj.yanxiufei.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xbw.mhx1999.top

C#:   1234567.ToString("N0")
来源：http://fpf.jinqigufen.top

[E17] 首字母大写
来源：http://hgp.yonumen.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mkl.hnqzz.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://bhm.hesvh.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cfq.guannengcc.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tgi.zhaomingkeji.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gqj.hesvh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ntv.shanyushiyangtech.top

Ruby: s.capitalize
来源：http://eye.xuanzx.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vwk.ywan-chungtsiang.top

[E18] 模板占位符替换
来源：http://cfp.chenjidiqi.icu

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zlp.zhengqikj.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nmz.jyoumei.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://flb.tanke756.top

TS:   tpl.replaceAll("{name}", name)
来源：http://exf.nwbrower.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lfp.havefunace.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jqz.vqdsnc.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zgb.chenlongwang.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hnv.hfpthk.cn

[E19] 多行文本按行拆分
来源：http://lss.ivvv.top

Py:   s.splitlines()
来源：http://dpd.zhijiandao.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mza.zhixingplan.top

JS:   s.split(/\r?\n/)
来源：http://rdy.haohaochexian.top

TS:   s.split(/\r?\n/)
来源：http://rvq.ydjk.org.cn

Java: s.lines().toList()
来源：http://xkk.xylfe.cn

Go:   strings.Split(s, "\n")
来源：http://ruy.dashuyun.cn

Ruby: s.lines
来源：http://bkq.xylfe.cn

C#:   s.Split('\n')
来源：http://cdx.316326.xyz

[E20] 判断字符串是否为空
来源：http://zqn.pengpengdd.cyou

Py:   if not s:
来源：http://ewv.kuanghao11.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ptq.chenjidiqi.icu

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cig.xylfe.cn

TS:   if (s === "") {}
来源：http://yac.hfpthk.cn

Java: if (s.isEmpty()) {}
来源：http://yif.hesvh.cn

Go:   if s == "" {}
来源：http://iun.gogol.net.cn

Ruby: if s.empty?
来源：http://yms.feifeiyinyue.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ghb.shangyingyoupin.top

[E21] 超长截断加省略号
来源：http://tjs.cqqwz.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lud.jinqigufen.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ezu.redwolf501.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dph.iojbl.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zue.uphjek.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dve.bbcook.cn

Go:   // 按 rune 判断长度后截断
来源：http://znd.pycfn.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bun.yueranfly.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rqo.yueranfly.top

[E22] 字节长度与字符长度
来源：http://aqt.ydjk.org.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cky.52xcode.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://the.zycfv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zgc.havefunace.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://acy.xinyue.icu

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nbd.yj20258.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://czc.snrcjt.cn

Ruby: s.bytesize;  s.length
来源：http://kny.cqqwz.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fkh.shzxlz.cn

================================================================================
来源：http://hbp.sweek.top

F. 文件与目录
来源：http://xvn.svipenyu.cn

================================================================================
来源：http://fym.xylfe.cn

[F01] 读取整个文件
来源：http://ghc.hysaishi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ljj.jinghuilouyu.cn

PHP:  file_get_contents("a.txt");
来源：http://zqo.sufxvd.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rzz.hnxiangtu.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nhs.smart0.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://txw.jqgufenzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nyk.yfazqb.com

Ruby: File.read("a.txt")
来源：http://zhq.ydjk.org.cn

C#:   File.ReadAllText("a.txt");
来源：http://eij.daxiang520.top

[F02] 逐行读取文件
来源：http://uwc.ybcxt.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pmt.zhoulong.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jll.ydzc1.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wmd.feifeiyinyue.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ssb.yj20258888.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yio.mhx1999.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jlq.meibo888.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rld.fengsongda.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xdw.xuanzx.com

[F03] 写入文件（覆盖）
来源：http://ttk.tanke756.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bqv.xziqi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://daq.nanxinkj.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ess.feifeiyinyue.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://who.yanxiufei.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fxh.zhiwuduotai.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jgb.aibaodan.cn

Ruby: File.write("a.txt", "hi")
来源：http://ofe.zhoulong.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dai.xziqi.cn

[F04] 追加写入文件
来源：http://zso.zhengqikj.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tjd.vehdjk.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qwr.zhiwuduotai.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ktz.epnwcf.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xly.zhengqikj.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://iau.52xcode.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://stf.ivvv.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pnd.zhiwuduotai.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tvy.ppjwa.cn

[F05] 判断文件或目录是否存在
来源：http://gnk.hysaishi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mqg.daxiang520.top

PHP:  file_exists("a.txt");
来源：http://ryh.hammf.cn

JS:   fs.existsSync("a.txt")
来源：http://joj.epnwcf.com

TS:   fs.existsSync("a.txt")
来源：http://coy.yanxiufei.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://rgc.jinqigfzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://psf.zhoulong.xyz

Ruby: File.exist?("a.txt")
来源：http://mtt.gotoacloud.top

C#:   File.Exists("a.txt")
来源：http://oho.jqgufenzy.top

[F06] 删除文件
来源：http://fjk.zhengqikj.top

Py:   os.remove("a.txt")
来源：http://qti.andypj.xyz

PHP:  unlink("a.txt");
来源：http://yig.dashuyun.cn

JS:   fs.unlinkSync("a.txt")
来源：http://mou.zhijiandao.cn

TS:   fs.unlinkSync("a.txt")
来源：http://yjc.0kj1m.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jmi.aibaodan.cn

Go:   os.Remove("a.txt")
来源：http://gfa.wangshuangyany.cn

Ruby: File.delete("a.txt")
来源：http://vhn.jinqigufen.top

C#:   File.Delete("a.txt");
来源：http://tqz.fanxiaobao.xyz

[F07] 创建目录（含多级）
来源：http://vpu.redwolf501.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://obp.fktsv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mwz.jqgufenzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cnn.52xcode.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ono.kuanghao11.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ydf.316326.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xna.hcnkem.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ccx.sweek.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zcw.jianghu66.top

[F08] 遍历目录
来源：http://cxu.daxiang520.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://xgc.kuanghao11.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wgg.zhixingplan.top

JS:   fs.readdirSync("dir")
来源：http://faw.9152youxi.cn

TS:   fs.readdirSync("dir")
来源：http://vas.yonumen.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zue.yj202588.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://sth.xinyue.icu

Ruby: Dir.children("dir")
来源：http://jzt.zdqjudy.top

C#:   Directory.GetFiles("dir")
来源：http://jue.dashuyun.cn

[F09] 获取文件大小
来源：http://erz.ppjwa.cn

Py:   os.path.getsize("a.txt")
来源：http://knn.yj20258.top

PHP:  filesize("a.txt");
来源：http://lxx.bbcook.cn

JS:   fs.statSync("a.txt").size
来源：http://fqv.cucudq.cn

TS:   fs.statSync("a.txt").size
来源：http://xev.havefunace.top

Java: Files.size(Path.of("a.txt"))
来源：http://sqg.meibo888.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dgo.pycfn.com

Ruby: File.size("a.txt")
来源：http://lif.uphjek.com


<!-- 参考信息 -->