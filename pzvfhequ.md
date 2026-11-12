代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://wmi.uphjek.com

PHP:  implode(", ", $arr);
来源：http://zhz.jinghuilouyu.cn

JS:   arr.join(", ")
来源：http://ryr.hnxiangtu.top

TS:   arr.join(", ")
来源：http://krj.yuanzhike.top

Java: String.join(", ", list)
来源：http://sxy.redwolf501.top

Go:   strings.Join(strs, ", ")
来源：http://vht.jlsjyb.cn

Ruby: arr.join(", ")
来源：http://rgi.ehwqpu.com

C#:   string.Join(", ", list)
来源：http://wct.nanxuanxn.top

================================================================================
来源：http://tmh.pycfn.com

E. 字符串处理
来源：http://ewc.cashguo.top

================================================================================
来源：http://gqd.yueranfly.top

[E01] 拼接字符串
来源：http://onb.zhiwuduotai.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qoh.ppjwa.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uww.jinqigfzy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kea.xinyue.icu

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wxe.nwbrower.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mjk.daria6918.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jeo.aizwys.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://itf.xziqi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gtj.iojbl.cn

[E02] 重复字符串
来源：http://kul.tianlin.xyz

Py:   "ab" * 3
来源：http://pva.havefunace.top

PHP:  str_repeat("ab", 3);
来源：http://gzh.chenzaomai.com

JS:   "ab".repeat(3)
来源：http://yfp.daxiang520.top

TS:   "ab".repeat(3)
来源：http://ctc.jinqigfzy.top

Java: "ab".repeat(3)
来源：http://tte.jinghuilouyu.cn

Go:   strings.Repeat("ab", 3)
来源：http://kru.fzhhl.top

Ruby: "ab" * 3
来源：http://mkq.pengpengdd.cyou

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mqu.zhiwuduotai.top

[E03] 截取子串
来源：http://tio.hongshengwenyu.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kle.tianlin.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jqy.hfpthk.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lgn.sysykeji.top

TS:   s.slice(1, 4)
来源：http://tqt.yanxiufei.cn

Java: s.substring(1, 4)
来源：http://rzn.shangyingyoupin.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vaj.jlsjyb.cn

Ruby: s[1, 3];  s[1..3]
来源：http://lqy.zhengqikj.top

C#:   s.Substring(1, 3)
来源：http://nth.zhengqikj.top

[E04] 查找子串位置
来源：http://cxu.guowangkeji.top

Py:   s.find("x");  s.index("x")
来源：http://bcu.nanxuanxn.top

PHP:  strpos($s, "x");
来源：http://abf.birdmap.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nau.yangfankeji.com

TS:   s.indexOf("x")
来源：http://qux.zhongyouzk.top

Java: s.indexOf("x")
来源：http://ivk.fengsongda.top

Go:   strings.Index(s, "x")
来源：http://qfc.nanxuanxn.top

Ruby: s.index("x")
来源：http://wez.snrcjt.cn

C#:   s.IndexOf("x")
来源：http://ghx.ehwqpu.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://fdb.aizwys.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lmd.ybcxt.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zuh.hcnkem.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jtx.svipenyu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://yjl.ybcxt.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vyz.0kj1m.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cta.zhijiandao.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zlh.pengpengdd.cyou

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jqo.shuidangran.top

[E06] 替换子串
来源：http://zhv.yongpay.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ndz.dianchejie.cn

PHP:  str_replace("a", "b", $s);
来源：http://utv.gotoacloud.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rrn.aibaodan.cn

TS:   s.replaceAll("a", "b")
来源：http://bjf.yueranfly.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gns.shuidangran.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://oat.hnqzz.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dav.yonumen.top

C#:   s.Replace("a", "b")
来源：http://xhm.jiagoushi.top

[E07] 按分隔符拆分
来源：http://lfk.shzxlz.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://efl.yanxiufei.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dxq.zhaomingkeji.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://awl.gotoacloud.top

TS:   s.split(",")
来源：http://pac.jinyuanbaomall.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zza.gotoacloud.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pke.yongpay.top

Ruby: s.split(",");  s.split
来源：http://czs.tarul.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zxn.ppjwa.cn

[E08] 数组按分隔符合并
来源：http://ytf.yj20258.top

Py:   ",".join(items)
来源：http://hcb.hysaishi.cn

PHP:  implode(",", $items);
来源：http://jzt.nanxinkj.top

JS:   items.join(",")
来源：http://orm.cucudq.cn

TS:   items.join(",")
来源：http://smx.jianghu66.top

Java: String.join(",", items)
来源：http://tbo.sxryk.cn

Go:   strings.Join(items, ",")
来源：http://kzt.xylfe.cn

Ruby: items.join(",")
来源：http://usk.chenzaomai.com

C#:   string.Join(",", items)
来源：http://rdr.yangfankeji.com

[E09] 去除所有空白字符
来源：http://kkm.hesvh.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ldl.316326.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wbl.ydzc1.top

JS:   s.replace(/\s+/g, "")
来源：http://drd.nwbrower.top

TS:   s.replace(/\s+/g, "")
来源：http://lnr.jinqigufen.top

Java: s.replaceAll("\\s+", "")
来源：http://trp.shanyushiyangtech.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://mmf.ivvv.top

Ruby: s.gsub(/\s+/, "")
来源：http://chj.vehdjk.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kkd.gotoacloud.top

[E10] 左侧补零 / 定长填充
来源：http://ghr.hnqzz.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pxt.nwbrower.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qpn.sjlbkw.cn

JS:   "7".padStart(3, "0")
来源：http://efi.52xcode.cn

TS:   "7".padStart(3, "0")
来源：http://ofo.jianghu66.top

Java: String.format("%03d", 7)
来源：http://iya.sysykeji.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://auq.smart0.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xdo.jinqigfzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wka.yuanzhike.top

[E11] 反转字符串
来源：http://wle.9152youxi.cn

Py:   s[::-1]
来源：http://sxb.dashuyun.cn

PHP:  strrev($s);
来源：http://doc.wangshuangyany.cn

JS:   [...s].reverse().join("")
来源：http://ypw.yfazqb.com

TS:   [...s].reverse().join("")
来源：http://axk.cqqwz.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://oyk.fzhhl.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://fgx.ctjpmb.com

Ruby: s.reverse
来源：http://bjd.gogol.net.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zdy.chenzaomai.com

[E12] 统计某字符出现次数
来源：http://goa.yongpay.top

Py:   s.count("a")
来源：http://fiq.feifeiyinyue.top

PHP:  substr_count($s, "a");
来源：http://ahf.hywenlv.cn

JS:   s.split("a").length - 1
来源：http://sbd.nanxuanxn.top

TS:   s.split("a").length - 1
来源：http://tii.chenjidiqi.icu

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vgn.kuanghao11.cn

Go:   strings.Count(s, "a")
来源：http://wch.xylfe.cn

Ruby: s.count("a")
来源：http://dwh.yonumen.top

C#:   s.Count(c => c == 'a')
来源：http://izl.zhaomingkeji.xyz

[E13] 逐字符遍历
来源：http://nea.316326.xyz

Py:   for ch in s: print(ch)
来源：http://atr.ppjwa.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ifr.sxryk.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://inc.bbcook.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ehe.xuetiantiany.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lev.yangfankeji.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rdj.tanke756.top

Ruby: s.each_char { |ch| puts ch }
来源：http://igd.sysykeji.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://los.jyoumei.cn

[E14] URL 编码与 Base64
来源：http://ncv.pycfn.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fla.yongpay.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://erj.zhijiandao.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yep.chenzaomai.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yug.nanxinkj.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wjm.zycfv.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pzb.hysaishi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ayh.wangshuangyany.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dqp.tanke756.top

[E15] HTML 转义 / 反转义
来源：http://aib.cdnleiting.top

Py:   html.escape(s);  html.unescape(s)
来源：http://jhg.yuxming.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nqr.yj20258888.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hwx.mhx1999.top

TS:   // 同上，务必做 XSS 过滤
来源：http://lzc.ehwqpu.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gjy.dianchejie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ewb.aizwys.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://umb.hywenlv.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tza.meibo888.top

[E16] 数字千分位
来源：http://eld.ydjk.org.cn

Py:   f"{1234567:,}"
来源：http://wgz.wangdashe.top

PHP:  number_format(1234567);
来源：http://zqj.birdmap.top

JS:   (1234567).toLocaleString("en-US")
来源：http://wiv.shangyingyoupin.top

TS:   (1234567).toLocaleString("en-US")
来源：http://tha.c1oappe.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zpz.jlsjyb.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vqa.epnwcf.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bxs.cdnleiting.top

C#:   1234567.ToString("N0")
来源：http://zih.zhixingplan.top

[E17] 首字母大写
来源：http://erx.hesvh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ejy.jinqigufen.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://vgq.c1oappe.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://stf.yj20258888.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wme.snrcjt.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dxk.jinghuilouyu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://agm.hesvh.cn

Ruby: s.capitalize
来源：http://jsk.tanke756.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vii.zhijiandao.cn

[E18] 模板占位符替换
来源：http://neo.shzxlz.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pul.chenjidiqi.icu

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kah.jlsjyb.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://uts.yonumen.top

TS:   tpl.replaceAll("{name}", name)
来源：http://sdg.yanxiufei.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wlv.sufxvd.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dak.tanke756.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uqy.yanxiufei.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jak.zycfv.cn

[E19] 多行文本按行拆分
来源：http://axu.jinyuanbaomall.cn

Py:   s.splitlines()
来源：http://mqv.yongpay.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://trg.zhoulong.xyz

JS:   s.split(/\r?\n/)
来源：http://rqc.nanxinkj.top

TS:   s.split(/\r?\n/)
来源：http://pig.chenzaomai.com

Java: s.lines().toList()
来源：http://uol.gogol.net.cn

Go:   strings.Split(s, "\n")
来源：http://qvb.haohaochexian.top

Ruby: s.lines
来源：http://zmt.shuidangran.top

C#:   s.Split('\n')
来源：http://las.nanxinkj.top

[E20] 判断字符串是否为空
来源：http://prm.ehwqpu.com

Py:   if not s:
来源：http://tub.nanxinkj.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ybz.hfpthk.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://uan.ehwqpu.com

TS:   if (s === "") {}
来源：http://uyy.guannengcc.top

Java: if (s.isEmpty()) {}
来源：http://ulx.chenlongwang.top

Go:   if s == "" {}
来源：http://vqe.zhiwuduotai.top

Ruby: if s.empty?
来源：http://rrw.chenlongwang.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mub.daxiang520.top

[E21] 超长截断加省略号
来源：http://fqz.yongpay.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://eln.snrcjt.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cru.yvedp.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hwc.sufxvd.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nut.shangyingyoupin.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://akq.jqgufenzy.top

Go:   // 按 rune 判断长度后截断
来源：http://fde.9152youxi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lcj.gzhubu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tgz.jinyuanbaomall.cn

[E22] 字节长度与字符长度
来源：http://bhz.hywenlv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://iev.yonumen.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ihx.pengpengdd.cyou

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qfc.zhengqikj.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lbw.cheryme.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gov.fktsv.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lqd.jinghuilouyu.cn

Ruby: s.bytesize;  s.length
来源：http://dfk.ppjwa.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gkc.cucudq.cn

================================================================================
来源：http://ajb.hnqzz.top

F. 文件与目录
来源：http://qbe.tianlin.xyz

================================================================================
来源：http://kaa.xziqi.cn

[F01] 读取整个文件
来源：http://lew.zhengqikj.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wzx.ivvv.top

PHP:  file_get_contents("a.txt");
来源：http://sfb.bbcook.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lvh.aizwys.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://izz.jinyuanbaomall.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ndl.dianchejie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ity.jiagoushi.top

Ruby: File.read("a.txt")
来源：http://bqt.fanxiaobao.xyz

C#:   File.ReadAllText("a.txt");
来源：http://neu.tian-w.cn

[F02] 逐行读取文件
来源：http://eze.sufxvd.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fac.zdbjq.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cls.jinqigfzy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ikv.dashuyun.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://smo.cashguo.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hep.tanke756.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dvj.fehbvm.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sdn.hnxiangtu.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uhn.cdnleiting.top

[F03] 写入文件（覆盖）
来源：http://ani.daxiang520.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lnx.yangfankeji.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://lvk.zhaomingkeji.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://grc.yanxiufei.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fnd.vehdjk.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://okh.yj20258.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hrn.aibaodan.cn

Ruby: File.write("a.txt", "hi")
来源：http://yes.ctjpmb.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ewt.ctjpmb.com

[F04] 追加写入文件
来源：http://hnz.yangfankeji.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://oei.jinqigufen.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://epr.c1oappe.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lxw.hnqzz.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://afm.xuetiantiany.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://das.vehdjk.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://npi.zhixingplan.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yrz.daria6918.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://irg.nwbrower.top

[F05] 判断文件或目录是否存在
来源：http://xrb.zycfv.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fsq.xinyue.icu

PHP:  file_exists("a.txt");
来源：http://qxo.hammf.cn

JS:   fs.existsSync("a.txt")
来源：http://kmz.gogol.net.cn

TS:   fs.existsSync("a.txt")
来源：http://cgi.9152youxi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://tfz.haohaochexian.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zdo.hongshengwenyu.top

Ruby: File.exist?("a.txt")
来源：http://tss.fktsv.cn

C#:   File.Exists("a.txt")
来源：http://pgv.redwolf501.top

[F06] 删除文件
来源：http://tqh.svipenyu.cn

Py:   os.remove("a.txt")
来源：http://yew.ydzc1.top

PHP:  unlink("a.txt");
来源：http://lrv.havefunace.top

JS:   fs.unlinkSync("a.txt")
来源：http://khg.fehbvm.com

TS:   fs.unlinkSync("a.txt")
来源：http://zgf.zhengqikj.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://prt.xylfe.cn

Go:   os.Remove("a.txt")
来源：http://igq.ywan-chungtsiang.top

Ruby: File.delete("a.txt")
来源：http://emg.hysaishi.cn

C#:   File.Delete("a.txt");
来源：http://oas.gzhubu.top

[F07] 创建目录（含多级）
来源：http://tiw.9152youxi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vbk.mhx1999.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dbs.zhiwuduotai.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nfc.hysaishi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qaa.bjfxy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ubj.aibaodan.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://und.andypj.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jfb.xinyue.icu

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hgq.yvedp.cn

[F08] 遍历目录
来源：http://hed.jqgfzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://eqz.zycfv.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zem.316326.xyz

JS:   fs.readdirSync("dir")
来源：http://fpr.hfpthk.cn

TS:   fs.readdirSync("dir")
来源：http://kbr.mhx1999.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kae.ybcxt.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://dgq.ctjpmb.com

Ruby: Dir.children("dir")
来源：http://bce.shuidangran.top

C#:   Directory.GetFiles("dir")
来源：http://pfj.zhixingplan.top

[F09] 获取文件大小
来源：http://aoa.fzhhl.top

Py:   os.path.getsize("a.txt")
来源：http://diz.yvedp.cn

PHP:  filesize("a.txt");
来源：http://cei.hysaishi.cn

JS:   fs.statSync("a.txt").size
来源：http://wrk.daria6918.cn

TS:   fs.statSync("a.txt").size
来源：http://dud.havefunace.top

Java: Files.size(Path.of("a.txt"))
来源：http://ylc.jqgufenzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wkx.nanxuanxn.top

Ruby: File.size("a.txt")
来源：http://gaf.dianchejie.cn

C#:   new FileInfo("a.txt").Length
来源：http://jwz.cheryme.top

[F10] 取文件扩展名 / 文件名
来源：http://qvw.ivvv.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nef.gotoacloud.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dlq.meibo888.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gvt.jinyuanbaomall.cn

TS:   path.extname("a.txt")
来源：http://tpa.dianchejie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qku.zdqjudy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wpr.vqdsnc.cn


<!-- 参考信息 -->