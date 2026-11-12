代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://gco.mhx1999.top

PHP:  implode(", ", $arr);
来源：http://pfo.sjlbkw.cn

JS:   arr.join(", ")
来源：http://zml.redwolf501.top

TS:   arr.join(", ")
来源：http://xwf.yfazqb.com

Java: String.join(", ", list)
来源：http://vgy.shangyingyoupin.top

Go:   strings.Join(strs, ", ")
来源：http://zwb.shanyushiyangkeji.top

Ruby: arr.join(", ")
来源：http://khf.meibo888.top

C#:   string.Join(", ", list)
来源：http://rib.yonumen.top

================================================================================
来源：http://tis.sweek.top

E. 字符串处理
来源：http://lvv.jiagoushi.top

================================================================================
来源：http://eta.zdqjudy.top

[E01] 拼接字符串
来源：http://nbe.svipenyu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jzf.zdqjudy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yda.birdmap.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zlw.jinghuilouyu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://aal.nanxuanxn.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lne.gzhubu.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dcr.fanxiaobao.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://isp.316326.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://asy.fehbvm.com

[E02] 重复字符串
来源：http://gbx.chenlongwang.top

Py:   "ab" * 3
来源：http://tpx.guowangkeji.top

PHP:  str_repeat("ab", 3);
来源：http://syo.tianlin.xyz

JS:   "ab".repeat(3)
来源：http://qmn.tarul.cn

TS:   "ab".repeat(3)
来源：http://uow.jiagoushi.top

Java: "ab".repeat(3)
来源：http://bhb.aibaodan.cn

Go:   strings.Repeat("ab", 3)
来源：http://rqv.kuanghao11.cn

Ruby: "ab" * 3
来源：http://bda.hnqzz.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ntp.redwolf501.top

[E03] 截取子串
来源：http://fet.jyoumei.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pno.yj20258888.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://onl.shuidangran.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jys.52xcode.cn

TS:   s.slice(1, 4)
来源：http://dez.zdqjudy.top

Java: s.substring(1, 4)
来源：http://xum.sxryk.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://znd.hywenlv.cn

Ruby: s[1, 3];  s[1..3]
来源：http://lcr.cashguo.top

C#:   s.Substring(1, 3)
来源：http://lan.wangdashe.top

[E04] 查找子串位置
来源：http://tbn.yuanzhike.top

Py:   s.find("x");  s.index("x")
来源：http://vgq.aizwys.cn

PHP:  strpos($s, "x");
来源：http://ybl.zhoulong.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://edw.ybcxt.top

TS:   s.indexOf("x")
来源：http://yrf.vehdjk.com

Java: s.indexOf("x")
来源：http://nqm.shangyingyoupin.top

Go:   strings.Index(s, "x")
来源：http://hck.aibaodan.cn

Ruby: s.index("x")
来源：http://jmf.52xcode.cn

C#:   s.IndexOf("x")
来源：http://jdd.zhaomingkeji.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://naf.zhijiandao.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://abm.fktsv.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://soi.shanyushiyangtech.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qqs.zycfv.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ugh.ybcxt.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xms.zhongyouzk.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sdv.andypj.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://flx.aibaodan.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pxa.hnqzz.top

[E06] 替换子串
来源：http://xzi.fanxiaobao.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kda.tianlin.xyz

PHP:  str_replace("a", "b", $s);
来源：http://bfg.ydjk.org.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yeb.xuetiantiany.cn

TS:   s.replaceAll("a", "b")
来源：http://yxq.yj202588.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hei.yj20258.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jfc.fzhhl.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ygc.tian-w.cn

C#:   s.Replace("a", "b")
来源：http://nht.dashuyun.cn

[E07] 按分隔符拆分
来源：http://utu.xuetiantiany.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qyy.ivvv.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qdl.hnxiangtu.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ytk.ybcxt.top

TS:   s.split(",")
来源：http://gny.iojbl.cn

Java: s.split(",");  s.split("\\s+")
来源：http://dsv.yonumen.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tmm.jinyuanbaomall.cn

Ruby: s.split(",");  s.split
来源：http://vgg.cashguo.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cdo.jqgfzy.top

[E08] 数组按分隔符合并
来源：http://fdz.gzhubu.top

Py:   ",".join(items)
来源：http://cpn.pengpengdd.cyou

PHP:  implode(",", $items);
来源：http://fpq.hnqzz.top

JS:   items.join(",")
来源：http://qej.zhijiandao.cn

TS:   items.join(",")
来源：http://lld.gogol.net.cn

Java: String.join(",", items)
来源：http://xjb.feifeiyinyue.top

Go:   strings.Join(items, ",")
来源：http://gcz.yvedp.cn

Ruby: items.join(",")
来源：http://sur.dianchejie.cn

C#:   string.Join(",", items)
来源：http://vhz.zhiwuduotai.top

[E09] 去除所有空白字符
来源：http://zml.snrcjt.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dzq.hysaishi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gst.zhongyouzk.top

JS:   s.replace(/\s+/g, "")
来源：http://btt.chenlongwang.top

TS:   s.replace(/\s+/g, "")
来源：http://qrk.wangdashe.top

Java: s.replaceAll("\\s+", "")
来源：http://jtp.havefunace.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://owm.hcnkem.com

Ruby: s.gsub(/\s+/, "")
来源：http://ysq.yj20258.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qyg.sjlbkw.cn

[E10] 左侧补零 / 定长填充
来源：http://zkr.bjfxy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hip.zhaomingkeji.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uvx.52xcode.cn

JS:   "7".padStart(3, "0")
来源：http://hvl.ybcxt.top

TS:   "7".padStart(3, "0")
来源：http://ddw.epnwcf.com

Java: String.format("%03d", 7)
来源：http://xxk.cashguo.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://wcl.ctjpmb.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://evk.zhoulong.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://roz.yanxiufei.cn

[E11] 反转字符串
来源：http://kqg.yanxiufei.cn

Py:   s[::-1]
来源：http://utx.yangfankeji.com

PHP:  strrev($s);
来源：http://unh.fanxiaobao.xyz

JS:   [...s].reverse().join("")
来源：http://cbx.chenlongwang.top

TS:   [...s].reverse().join("")
来源：http://hik.hfpthk.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wmf.meibo888.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://czu.ydzc1.top

Ruby: s.reverse
来源：http://dmx.cheryme.top

C#:   new string(s.Reverse().ToArray())
来源：http://leu.aizwys.cn

[E12] 统计某字符出现次数
来源：http://tgb.xinyue.icu

Py:   s.count("a")
来源：http://vfe.iojbl.cn

PHP:  substr_count($s, "a");
来源：http://mut.gzhubu.top

JS:   s.split("a").length - 1
来源：http://pst.ctjpmb.com

TS:   s.split("a").length - 1
来源：http://qvo.yongpay.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://oqr.aizwys.cn

Go:   strings.Count(s, "a")
来源：http://hdt.xinyue.icu

Ruby: s.count("a")
来源：http://obd.smart0.xyz

C#:   s.Count(c => c == 'a')
来源：http://vyl.dashuyun.cn

[E13] 逐字符遍历
来源：http://dur.yj20258.top

Py:   for ch in s: print(ch)
来源：http://net.kuanghao11.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jzv.hcnkem.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://tek.zycfv.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ehi.9152youxi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://soo.zhengqikj.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sqe.hammf.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qdy.ydjk.org.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://igb.xylfe.cn

[E14] URL 编码与 Base64
来源：http://dpw.zhoulong.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fas.ydjk.org.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://iin.yj20258888.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wbx.pycfn.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xmt.hfpthk.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://htl.yj20258.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kxx.nwbrower.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://aec.hnxiangtu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://znu.wangshuangyany.cn

[E15] HTML 转义 / 反转义
来源：http://aek.yuxming.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://nph.xingfuxueyuan.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hnw.fengsongda.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://olk.ctjpmb.com

TS:   // 同上，务必做 XSS 过滤
来源：http://mvx.fktsv.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dqs.ywan-chungtsiang.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lfn.cdnleiting.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kmg.iojbl.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ncr.zhoulong.xyz

[E16] 数字千分位
来源：http://wkx.chenzaomai.com

Py:   f"{1234567:,}"
来源：http://jvg.snrcjt.cn

PHP:  number_format(1234567);
来源：http://ydw.kuanghao11.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wwj.birdmap.top

TS:   (1234567).toLocaleString("en-US")
来源：http://tzz.ppjwa.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zna.zhoulong.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hnr.chenzaomai.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wot.redwolf501.top

C#:   1234567.ToString("N0")
来源：http://egu.hfpthk.cn

[E17] 首字母大写
来源：http://uea.epnwcf.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ues.ctjpmb.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://xlq.xinyue.icu

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rrg.ydjk.org.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wbb.guowangkeji.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pba.shanyushiyangtech.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zva.gaohongyu789.top

Ruby: s.capitalize
来源：http://egc.yonumen.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pbr.tian-w.cn

[E18] 模板占位符替换
来源：http://shv.9152youxi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bil.hcnkem.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://emg.sufxvd.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jdr.pycfn.com

TS:   tpl.replaceAll("{name}", name)
来源：http://sxg.cashguo.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cqa.zhiwuduotai.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bxx.snrcjt.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nyo.ctjpmb.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ogf.hammf.cn

[E19] 多行文本按行拆分
来源：http://utg.zycfv.cn

Py:   s.splitlines()
来源：http://eom.fehbvm.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ptn.vehdjk.com

JS:   s.split(/\r?\n/)
来源：http://vpg.fanxiaobao.xyz

TS:   s.split(/\r?\n/)
来源：http://lft.guannengcc.top

Java: s.lines().toList()
来源：http://oyr.sysykeji.top

Go:   strings.Split(s, "\n")
来源：http://gmx.ppjwa.cn

Ruby: s.lines
来源：http://vff.kuanghao11.cn

C#:   s.Split('\n')
来源：http://ilm.shuidangran.top

[E20] 判断字符串是否为空
来源：http://mpe.xuetiantiany.cn

Py:   if not s:
来源：http://wne.xuetiantiany.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qme.cheryme.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vds.mhx1999.top

TS:   if (s === "") {}
来源：http://jxu.ppjwa.cn

Java: if (s.isEmpty()) {}
来源：http://yem.316326.xyz

Go:   if s == "" {}
来源：http://bth.fehbvm.com

Ruby: if s.empty?
来源：http://icq.zhaomingkeji.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cyw.yangfankeji.com

[E21] 超长截断加省略号
来源：http://raf.smart0.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zxf.hfpthk.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xcl.jinghuilouyu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kwf.316326.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uza.xuanzx.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://aaq.bjfxy.top

Go:   // 按 rune 判断长度后截断
来源：http://cbo.xuetiantiany.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zya.ctjpmb.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hjo.shuidangran.top

[E22] 字节长度与字符长度
来源：http://kch.snrcjt.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kpx.hnqzz.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fuv.yonumen.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fbp.redwolf501.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ucx.chenzaomai.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nsu.hnxiangtu.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nbw.sxryk.cn

Ruby: s.bytesize;  s.length
来源：http://yyf.zhaomingkeji.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vyk.zdbjq.cn

================================================================================
来源：http://jws.cdnleiting.top

F. 文件与目录
来源：http://tfu.nanxinkj.top

================================================================================
来源：http://hep.sysykeji.top

[F01] 读取整个文件
来源：http://fis.cashguo.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://you.iojbl.cn

PHP:  file_get_contents("a.txt");
来源：http://sjr.quarkkingdee.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://omr.yongpay.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mss.cdnleiting.top

Java: Files.readString(Path.of("a.txt"))
来源：http://cmr.daria6918.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sic.guowangkeji.top

Ruby: File.read("a.txt")
来源：http://vby.ydzc1.top

C#:   File.ReadAllText("a.txt");
来源：http://xlv.xziqi.cn

[F02] 逐行读取文件
来源：http://zqe.gogol.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tef.aibaodan.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kdv.hfpthk.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ang.hesvh.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tqm.cheryme.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bzw.52xcode.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ivh.nwbrower.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xgn.dianchejie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://eaf.xziqi.cn

[F03] 写入文件（覆盖）
来源：http://zna.guowangkeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vbc.hongshengwenyu.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ksp.zdbjq.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hzu.daxiang520.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pbq.0kj1m.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fjv.zhiwuduotai.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://oym.jqgufenzy.top

Ruby: File.write("a.txt", "hi")
来源：http://lwj.redwolf501.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://idd.yonumen.top

[F04] 追加写入文件
来源：http://cju.jyoumei.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://csg.yanxiufei.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fpl.epnwcf.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://exs.zhijiandao.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tdc.ydzc1.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pvs.svipenyu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hgv.epnwcf.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wgz.sysykeji.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://set.yuxming.cn

[F05] 判断文件或目录是否存在
来源：http://ggd.fehbvm.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rll.jinqigfzy.top

PHP:  file_exists("a.txt");
来源：http://mwv.tianlin.xyz

JS:   fs.existsSync("a.txt")
来源：http://ewy.zhongyouzk.top

TS:   fs.existsSync("a.txt")
来源：http://umg.chenzaomai.com

Java: Files.exists(Path.of("a.txt"))
来源：http://lxz.redwolf501.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ass.hongshengwenyu.top

Ruby: File.exist?("a.txt")
来源：http://xgu.sjlbkw.cn

C#:   File.Exists("a.txt")
来源：http://bkn.tian-w.cn

[F06] 删除文件
来源：http://ikr.epnwcf.com

Py:   os.remove("a.txt")
来源：http://cde.vehdjk.com

PHP:  unlink("a.txt");
来源：http://ncl.ydjk.org.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pwr.sxryk.cn

TS:   fs.unlinkSync("a.txt")
来源：http://tqs.bjfxy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ohr.epnwcf.com

Go:   os.Remove("a.txt")
来源：http://cdb.fanxiaobao.xyz

Ruby: File.delete("a.txt")
来源：http://vkc.52xcode.cn

C#:   File.Delete("a.txt");
来源：http://czg.316326.xyz

[F07] 创建目录（含多级）
来源：http://qpj.aizwys.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wro.wangdashe.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ewo.svipenyu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wpa.chenlongwang.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xrj.pycfn.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hpv.yanxiufei.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://krc.shangyingyoupin.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lft.vqdsnc.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cnd.quarkkingdee.top

[F08] 遍历目录
来源：http://qyx.sufxvd.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qgx.ctjpmb.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xhl.haohaochexian.top

JS:   fs.readdirSync("dir")
来源：http://imt.yj20258888.top

TS:   fs.readdirSync("dir")
来源：http://sdh.hysaishi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bki.chenlongwang.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://vbg.fehbvm.com

Ruby: Dir.children("dir")
来源：http://jnz.fktsv.cn

C#:   Directory.GetFiles("dir")
来源：http://bxo.daria6918.cn

[F09] 获取文件大小
来源：http://bbo.yuanzhike.top

Py:   os.path.getsize("a.txt")
来源：http://mda.uphjek.com

PHP:  filesize("a.txt");
来源：http://myu.9152youxi.cn

JS:   fs.statSync("a.txt").size
来源：http://xqx.jinqigufen.top

TS:   fs.statSync("a.txt").size
来源：http://gij.feifeiyinyue.top

Java: Files.size(Path.of("a.txt"))
来源：http://ezo.sysykeji.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://omp.feifeiyinyue.top

Ruby: File.size("a.txt")
来源：http://vgz.fanxiaobao.xyz

C#:   new FileInfo("a.txt").Length
来源：http://ymb.hysaishi.cn

[F10] 取文件扩展名 / 文件名
来源：http://rsw.daxiang520.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://msq.zhaomingkeji.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cqp.andypj.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pso.jianghu66.top

TS:   path.extname("a.txt")
来源：http://kfh.daxiang520.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jrc.ydzc1.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://eww.hnxiangtu.top


<!-- 参考信息 -->