代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://crm.uphjek.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lfd.ppjwa.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pwv.xuetiantiany.cn

[D26] 数组转字符串
来源：http://qet.0kj1m.cn

Py:   ", ".join(map(str, arr))
来源：http://tga.hnqzz.top

PHP:  implode(", ", $arr);
来源：http://aax.nwbrower.top

JS:   arr.join(", ")
来源：http://yil.ydjk.org.cn

TS:   arr.join(", ")
来源：http://css.bjfxy.top

Java: String.join(", ", list)
来源：http://cie.aibaodan.cn

Go:   strings.Join(strs, ", ")
来源：http://qco.ydjk.org.cn

Ruby: arr.join(", ")
来源：http://lvq.epnwcf.com

C#:   string.Join(", ", list)
来源：http://skh.pengpengdd.cyou

================================================================================
来源：http://pxa.daria6918.cn

E. 字符串处理
来源：http://qsq.hongshengwenyu.top

================================================================================
来源：http://iou.yueranfly.top

[E01] 拼接字符串
来源：http://uqp.ppjwa.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://oft.yuanzhike.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zqb.sjlbkw.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wul.mhx1999.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lqu.hysaishi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jmm.fanxiaobao.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sfd.cqqwz.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://csc.meibo888.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://byh.ppjwa.cn

[E02] 重复字符串
来源：http://khx.tanke756.top

Py:   "ab" * 3
来源：http://jrz.tarul.cn

PHP:  str_repeat("ab", 3);
来源：http://sxk.zycfv.cn

JS:   "ab".repeat(3)
来源：http://cum.ydjk.org.cn

TS:   "ab".repeat(3)
来源：http://vxr.fanxiaobao.xyz

Java: "ab".repeat(3)
来源：http://izm.xingfuxueyuan.xyz

Go:   strings.Repeat("ab", 3)
来源：http://fyv.yongpay.top

Ruby: "ab" * 3
来源：http://cpp.c1oappe.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lky.yvedp.cn

[E03] 截取子串
来源：http://ufg.yj20258888.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vbk.sufxvd.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fop.cheryme.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vzs.redwolf501.top

TS:   s.slice(1, 4)
来源：http://gkq.cdnleiting.top

Java: s.substring(1, 4)
来源：http://wmg.dashuyun.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://eiy.cqqwz.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qxt.chenzaomai.com

C#:   s.Substring(1, 3)
来源：http://bok.52xcode.cn

[E04] 查找子串位置
来源：http://dnq.jlsjyb.cn

Py:   s.find("x");  s.index("x")
来源：http://uly.jinqigufen.top

PHP:  strpos($s, "x");
来源：http://urp.fktsv.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mtb.hammf.cn

TS:   s.indexOf("x")
来源：http://pup.nwbrower.top

Java: s.indexOf("x")
来源：http://znj.fanxiaobao.xyz

Go:   strings.Index(s, "x")
来源：http://hwb.yuanzhike.top

Ruby: s.index("x")
来源：http://vbw.tarul.cn

C#:   s.IndexOf("x")
来源：http://qqq.fzhhl.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://qmy.xuetiantiany.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zqo.hysaishi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lgt.bbcook.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mhz.jqgfzy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://nff.ywan-chungtsiang.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ydc.tianlin.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ezf.mhx1999.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tvf.hammf.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jip.xylfe.cn

[E06] 替换子串
来源：http://qbm.ctjpmb.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://let.meibo888.top

PHP:  str_replace("a", "b", $s);
来源：http://jrz.snrcjt.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ocz.ydzc1.top

TS:   s.replaceAll("a", "b")
来源：http://vbw.pengpengdd.cyou

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://stg.shzxlz.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nsy.ydjk.org.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fbl.birdmap.top

C#:   s.Replace("a", "b")
来源：http://faw.shanyushiyangtech.top

[E07] 按分隔符拆分
来源：http://qjr.dashuyun.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gik.jinqigfzy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xuj.bbcook.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ybc.tian-w.cn

TS:   s.split(",")
来源：http://jzp.sjlbkw.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mmu.shangyingyoupin.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rml.zhongyouzk.top

Ruby: s.split(",");  s.split
来源：http://nib.xingfuxueyuan.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kfy.xylfe.cn

[E08] 数组按分隔符合并
来源：http://hrr.cdnleiting.top

Py:   ",".join(items)
来源：http://dgx.xuetiantiany.cn

PHP:  implode(",", $items);
来源：http://cam.vqdsnc.cn

JS:   items.join(",")
来源：http://hqd.aizwys.cn

TS:   items.join(",")
来源：http://isy.jinqigfzy.top

Java: String.join(",", items)
来源：http://pxu.mhx1999.top

Go:   strings.Join(items, ",")
来源：http://xcv.hysaishi.cn

Ruby: items.join(",")
来源：http://xwt.ivvv.top

C#:   string.Join(",", items)
来源：http://yzg.jyoumei.cn

[E09] 去除所有空白字符
来源：http://jxt.feifeiyinyue.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wui.jinqigfzy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ual.ybcxt.top

JS:   s.replace(/\s+/g, "")
来源：http://cin.xylfe.cn

TS:   s.replace(/\s+/g, "")
来源：http://xqo.snrcjt.cn

Java: s.replaceAll("\\s+", "")
来源：http://yxq.jlsjyb.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://hlb.zycfv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://yij.shangyingyoupin.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://enr.cdnleiting.top

[E10] 左侧补零 / 定长填充
来源：http://xqd.ydzc1.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wzt.yj20258.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qvf.jqgufenzy.top

JS:   "7".padStart(3, "0")
来源：http://kud.jinghuilouyu.cn

TS:   "7".padStart(3, "0")
来源：http://vza.svipenyu.cn

Java: String.format("%03d", 7)
来源：http://fqh.xziqi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://gvu.sjlbkw.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uyx.0kj1m.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hdw.hnqzz.top

[E11] 反转字符串
来源：http://jqm.zhixingplan.top

Py:   s[::-1]
来源：http://puw.yvedp.cn

PHP:  strrev($s);
来源：http://jpg.zycfv.cn

JS:   [...s].reverse().join("")
来源：http://eie.fengsongda.top

TS:   [...s].reverse().join("")
来源：http://rmx.zdqjudy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://uar.9152youxi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qje.meibo888.top

Ruby: s.reverse
来源：http://yvs.redwolf501.top

C#:   new string(s.Reverse().ToArray())
来源：http://jxg.c1oappe.top

[E12] 统计某字符出现次数
来源：http://lxg.ctjpmb.com

Py:   s.count("a")
来源：http://ydb.fehbvm.com

PHP:  substr_count($s, "a");
来源：http://jih.cucudq.cn

JS:   s.split("a").length - 1
来源：http://nag.yuanzhike.top

TS:   s.split("a").length - 1
来源：http://bxq.hcnkem.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lkb.hongshengwenyu.top

Go:   strings.Count(s, "a")
来源：http://jcu.havefunace.top

Ruby: s.count("a")
来源：http://swc.mhx1999.top

C#:   s.Count(c => c == 'a')
来源：http://vrw.havefunace.top

[E13] 逐字符遍历
来源：http://cbv.havefunace.top

Py:   for ch in s: print(ch)
来源：http://hlr.quarkkingdee.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://aij.0kj1m.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ria.ehwqpu.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://fxt.chenlongwang.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jyh.tarul.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vwh.gzhubu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://tlp.jlsjyb.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bpx.cashguo.top

[E14] URL 编码与 Base64
来源：http://psr.chenlongwang.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://chy.sufxvd.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://xql.nwbrower.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dnw.quarkkingdee.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wbz.hysaishi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ehf.hnxiangtu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jdd.ydjk.org.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pyb.gogol.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ool.xylfe.cn

[E15] HTML 转义 / 反转义
来源：http://tgh.zhiwuduotai.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ntr.jqgufenzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bla.aibaodan.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vhs.zhoulong.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://qnh.cashguo.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bvi.hammf.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://frp.feifeiyinyue.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://miz.dashuyun.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kob.epnwcf.com

[E16] 数字千分位
来源：http://jex.yuanzhike.top

Py:   f"{1234567:,}"
来源：http://ixo.zhaomingkeji.xyz

PHP:  number_format(1234567);
来源：http://uch.yueranfly.top

JS:   (1234567).toLocaleString("en-US")
来源：http://sck.ydjk.org.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zey.zhiwuduotai.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vws.ybcxt.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mkr.hfpthk.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://oqx.zhixingplan.top

C#:   1234567.ToString("N0")
来源：http://szu.shangyingyoupin.top

[E17] 首字母大写
来源：http://joq.jyoumei.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qvb.epnwcf.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://khg.jinqigfzy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mmz.feifeiyinyue.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rxs.hcnkem.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://oya.xuetiantiany.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://eed.cqqwz.cn

Ruby: s.capitalize
来源：http://xmt.jlsjyb.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wnq.dashuyun.cn

[E18] 模板占位符替换
来源：http://ctp.kuanghao11.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mzn.epnwcf.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bxt.yj20258888.top

JS:   tpl.replaceAll("{name}", name)
来源：http://jpi.nanxuanxn.top

TS:   tpl.replaceAll("{name}", name)
来源：http://gud.daria6918.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://enj.jinqigfzy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ytv.shzxlz.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bmn.zhoulong.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://oze.cdnleiting.top

[E19] 多行文本按行拆分
来源：http://ifr.yvedp.cn

Py:   s.splitlines()
来源：http://wgv.yuanzhike.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ksh.zdqjudy.top

JS:   s.split(/\r?\n/)
来源：http://wba.hnxiangtu.top

TS:   s.split(/\r?\n/)
来源：http://zrb.yj20258888.top

Java: s.lines().toList()
来源：http://sul.nwbrower.top

Go:   strings.Split(s, "\n")
来源：http://qjb.iojbl.cn

Ruby: s.lines
来源：http://ulx.sxryk.cn

C#:   s.Split('\n')
来源：http://fuh.dashuyun.cn

[E20] 判断字符串是否为空
来源：http://gfy.yueranfly.top

Py:   if not s:
来源：http://cbl.hysaishi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ofw.yvedp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tuj.hongshengwenyu.top

TS:   if (s === "") {}
来源：http://yaa.cqqwz.cn

Java: if (s.isEmpty()) {}
来源：http://hli.shanyushiyangtech.top

Go:   if s == "" {}
来源：http://vbs.zhengqikj.top

Ruby: if s.empty?
来源：http://xzg.hysaishi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zef.shuidangran.top

[E21] 超长截断加省略号
来源：http://oyy.kuanghao11.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://stj.sufxvd.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nbh.tarul.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qtz.nwbrower.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://frv.0kj1m.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ixz.yonumen.top

Go:   // 按 rune 判断长度后截断
来源：http://rss.hnqzz.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://afi.cqqwz.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rwy.bbcook.cn

[E22] 字节长度与字符长度
来源：http://syp.fzhhl.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://obh.zhengqikj.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://npd.haohaochexian.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mvp.mhx1999.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mux.svipenyu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hoi.shuidangran.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kzy.zdbjq.cn

Ruby: s.bytesize;  s.length
来源：http://xpc.yj20258888.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xvu.andypj.xyz

================================================================================
来源：http://guh.ydzc1.top

F. 文件与目录
来源：http://nja.jinghuilouyu.cn

================================================================================
来源：http://gtd.sjlbkw.cn

[F01] 读取整个文件
来源：http://gjp.yj20258888.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uru.shanyushiyangkeji.top

PHP:  file_get_contents("a.txt");
来源：http://qzj.sysykeji.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://erh.fengsongda.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://agi.yonumen.top

Java: Files.readString(Path.of("a.txt"))
来源：http://zqf.tianlin.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fjr.tarul.cn

Ruby: File.read("a.txt")
来源：http://jhm.ehwqpu.com

C#:   File.ReadAllText("a.txt");
来源：http://vne.yanxiufei.cn

[F02] 逐行读取文件
来源：http://sne.hysaishi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ahq.epnwcf.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ezt.vehdjk.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pad.nwbrower.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gse.xingfuxueyuan.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://djy.hammf.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yqn.wangdashe.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://irj.meibo888.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wjh.ybcxt.top

[F03] 写入文件（覆盖）
来源：http://mka.yuxming.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ivd.yanxiufei.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://czt.vqdsnc.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ogn.chenzaomai.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://loi.9152youxi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wqh.hywenlv.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gqc.jinyuanbaomall.cn

Ruby: File.write("a.txt", "hi")
来源：http://coh.havefunace.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ayp.xuanzx.com

[F04] 追加写入文件
来源：http://hku.jinqigufen.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ebu.jinghuilouyu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dbl.jinyuanbaomall.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nag.guannengcc.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://stw.yj20258.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hct.0kj1m.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fnh.xuetiantiany.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bch.nanxuanxn.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wbw.haohaochexian.top

[F05] 判断文件或目录是否存在
来源：http://ocl.birdmap.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rnu.wangdashe.top

PHP:  file_exists("a.txt");
来源：http://faz.ydzc1.top

JS:   fs.existsSync("a.txt")
来源：http://xri.snrcjt.cn

TS:   fs.existsSync("a.txt")
来源：http://cdo.hywenlv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://aad.fzhhl.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xpr.jinghuilouyu.cn

Ruby: File.exist?("a.txt")
来源：http://kgu.ywan-chungtsiang.top

C#:   File.Exists("a.txt")
来源：http://zzd.zhixingplan.top

[F06] 删除文件
来源：http://pph.hnxiangtu.top

Py:   os.remove("a.txt")
来源：http://yhl.ywan-chungtsiang.top

PHP:  unlink("a.txt");
来源：http://qmt.52xcode.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pzq.cheryme.top

TS:   fs.unlinkSync("a.txt")
来源：http://nbt.zhixingplan.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gdn.hfpthk.cn

Go:   os.Remove("a.txt")
来源：http://keb.cqqwz.cn

Ruby: File.delete("a.txt")
来源：http://wbt.xuetiantiany.cn

C#:   File.Delete("a.txt");
来源：http://his.zdqjudy.top

[F07] 创建目录（含多级）
来源：http://ngz.jinyuanbaomall.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pvs.smart0.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zvq.bjfxy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rxd.zhoulong.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dzb.jianghu66.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ahk.iojbl.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ref.guowangkeji.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xfk.jiagoushi.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://aqr.ywan-chungtsiang.top

[F08] 遍历目录
来源：http://bni.andypj.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://gvy.cqqwz.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kyw.cqqwz.cn

JS:   fs.readdirSync("dir")
来源：http://qvb.shzxlz.cn

TS:   fs.readdirSync("dir")
来源：http://tsu.wangdashe.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://edw.yvedp.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jwi.jlsjyb.cn

Ruby: Dir.children("dir")
来源：http://pic.yonumen.top

C#:   Directory.GetFiles("dir")
来源：http://bql.cdnleiting.top

[F09] 获取文件大小
来源：http://hqb.gotoacloud.top

Py:   os.path.getsize("a.txt")
来源：http://xek.vehdjk.com

PHP:  filesize("a.txt");
来源：http://pjn.xingfuxueyuan.xyz

JS:   fs.statSync("a.txt").size
来源：http://zml.yj20258888.top

TS:   fs.statSync("a.txt").size
来源：http://xwy.nanxinkj.top

Java: Files.size(Path.of("a.txt"))
来源：http://vic.zdqjudy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pga.yvedp.cn

Ruby: File.size("a.txt")
来源：http://gbu.shanyushiyangtech.top

C#:   new FileInfo("a.txt").Length
来源：http://jtv.havefunace.top

[F10] 取文件扩展名 / 文件名
来源：http://qca.andypj.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hww.zhijiandao.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mfd.shuidangran.top


<!-- 参考信息 -->