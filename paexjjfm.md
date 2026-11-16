代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lfq.yfazqb.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tcz.smart0.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xsq.chenlongwang.top

[D26] 数组转字符串
来源：http://psm.yvedp.cn

Py:   ", ".join(map(str, arr))
来源：http://fim.dianchejie.cn

PHP:  implode(", ", $arr);
来源：http://ele.haohaochexian.top

JS:   arr.join(", ")
来源：http://fqd.gzhubu.top

TS:   arr.join(", ")
来源：http://tql.pengpengdd.cyou

Java: String.join(", ", list)
来源：http://keo.guannengcc.top

Go:   strings.Join(strs, ", ")
来源：http://bnd.ctjpmb.com

Ruby: arr.join(", ")
来源：http://xlw.wangdashe.top

C#:   string.Join(", ", list)
来源：http://ycl.chenzaomai.com

================================================================================
来源：http://wsm.gotoacloud.top

E. 字符串处理
来源：http://deg.52xcode.cn

================================================================================
来源：http://zed.zdbjq.cn

[E01] 拼接字符串
来源：http://rze.iojbl.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gpy.wangshuangyany.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wqk.shzxlz.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zcz.snrcjt.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vmz.jyoumei.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ddl.andypj.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xui.epnwcf.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wmn.cucudq.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bgf.snrcjt.cn

[E02] 重复字符串
来源：http://ono.epnwcf.com

Py:   "ab" * 3
来源：http://xzg.yfazqb.com

PHP:  str_repeat("ab", 3);
来源：http://fxh.dashuyun.cn

JS:   "ab".repeat(3)
来源：http://pxm.kuanghao11.cn

TS:   "ab".repeat(3)
来源：http://iuv.jyoumei.cn

Java: "ab".repeat(3)
来源：http://eaf.haohaochexian.top

Go:   strings.Repeat("ab", 3)
来源：http://zrp.zdbjq.cn

Ruby: "ab" * 3
来源：http://hwf.ywan-chungtsiang.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://owr.yuxming.cn

[E03] 截取子串
来源：http://lsf.havefunace.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://glu.nwbrower.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://eou.jiagoushi.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ife.zdbjq.cn

TS:   s.slice(1, 4)
来源：http://kkp.xingfuxueyuan.xyz

Java: s.substring(1, 4)
来源：http://kpo.jyoumei.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://azb.cheryme.top

Ruby: s[1, 3];  s[1..3]
来源：http://bkz.dianchejie.cn

C#:   s.Substring(1, 3)
来源：http://gfo.yuxming.cn

[E04] 查找子串位置
来源：http://rpm.zhaomingkeji.xyz

Py:   s.find("x");  s.index("x")
来源：http://yty.vqdsnc.cn

PHP:  strpos($s, "x");
来源：http://ith.yj202588.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lku.chenlongwang.top

TS:   s.indexOf("x")
来源：http://pmk.feifeiyinyue.top

Java: s.indexOf("x")
来源：http://rgg.xuanzx.com

Go:   strings.Index(s, "x")
来源：http://nif.sxryk.cn

Ruby: s.index("x")
来源：http://rts.sjlbkw.cn

C#:   s.IndexOf("x")
来源：http://cfs.aizwys.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pvy.yj20258888.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://eys.shanyushiyangkeji.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ktv.tianlin.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tnu.jlsjyb.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hfp.uphjek.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zks.xuetiantiany.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fhu.cucudq.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dvx.gotoacloud.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zzu.meibo888.top

[E06] 替换子串
来源：http://siu.daria6918.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ppa.chenjidiqi.icu

PHP:  str_replace("a", "b", $s);
来源：http://rly.yj20258.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gxt.daria6918.cn

TS:   s.replaceAll("a", "b")
来源：http://emg.xuanzx.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tqs.fanxiaobao.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yhf.zhixingplan.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://smj.hfpthk.cn

C#:   s.Replace("a", "b")
来源：http://ikg.tian-w.cn

[E07] 按分隔符拆分
来源：http://trf.hcnkem.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mgg.xylfe.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vbp.hysaishi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://msk.yj20258.top

TS:   s.split(",")
来源：http://bjs.fktsv.cn

Java: s.split(",");  s.split("\\s+")
来源：http://bge.aibaodan.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cmk.fzhhl.top

Ruby: s.split(",");  s.split
来源：http://efo.sufxvd.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mru.havefunace.top

[E08] 数组按分隔符合并
来源：http://jpv.hesvh.cn

Py:   ",".join(items)
来源：http://xmx.tianlin.xyz

PHP:  implode(",", $items);
来源：http://wvm.gotoacloud.top

JS:   items.join(",")
来源：http://dqa.dashuyun.cn

TS:   items.join(",")
来源：http://zxf.yfazqb.com

Java: String.join(",", items)
来源：http://jcd.tianlin.xyz

Go:   strings.Join(items, ",")
来源：http://ekd.jqgfzy.top

Ruby: items.join(",")
来源：http://lmv.cdnleiting.top

C#:   string.Join(",", items)
来源：http://cqq.yj202588.top

[E09] 去除所有空白字符
来源：http://qsi.shanyushiyangkeji.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xjz.gaohongyu789.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pij.uphjek.com

JS:   s.replace(/\s+/g, "")
来源：http://vrz.pycfn.com

TS:   s.replace(/\s+/g, "")
来源：http://wpq.zhijiandao.cn

Java: s.replaceAll("\\s+", "")
来源：http://vcn.zhaomingkeji.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://vsm.yfazqb.com

Ruby: s.gsub(/\s+/, "")
来源：http://zit.xinyue.icu

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yne.ybcxt.top

[E10] 左侧补零 / 定长填充
来源：http://suk.zhiwuduotai.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nqi.hnxiangtu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gil.haohaochexian.top

JS:   "7".padStart(3, "0")
来源：http://gjq.meibo888.top

TS:   "7".padStart(3, "0")
来源：http://zyg.dashuyun.cn

Java: String.format("%03d", 7)
来源：http://tky.ydzc1.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://jdc.yj20258888.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://idw.tian-w.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lto.zdbjq.cn

[E11] 反转字符串
来源：http://qma.jqgfzy.top

Py:   s[::-1]
来源：http://cpc.aibaodan.cn

PHP:  strrev($s);
来源：http://vdp.zhiwuduotai.top

JS:   [...s].reverse().join("")
来源：http://ubf.hysaishi.cn

TS:   [...s].reverse().join("")
来源：http://tuc.smart0.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://xhe.dashuyun.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://otb.xuanzx.com

Ruby: s.reverse
来源：http://hne.meibo888.top

C#:   new string(s.Reverse().ToArray())
来源：http://tta.iojbl.cn

[E12] 统计某字符出现次数
来源：http://vdb.chenjidiqi.icu

Py:   s.count("a")
来源：http://hsh.yj20258.top

PHP:  substr_count($s, "a");
来源：http://edu.kuanghao11.cn

JS:   s.split("a").length - 1
来源：http://azh.gaohongyu789.top

TS:   s.split("a").length - 1
来源：http://xzp.shanyushiyangtech.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jkb.hesvh.cn

Go:   strings.Count(s, "a")
来源：http://zct.ivvv.top

Ruby: s.count("a")
来源：http://ofh.nanxinkj.top

C#:   s.Count(c => c == 'a')
来源：http://nek.gotoacloud.top

[E13] 逐字符遍历
来源：http://zvz.fengsongda.top

Py:   for ch in s: print(ch)
来源：http://jew.yangfankeji.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://khr.jinqigfzy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://vkm.xinyue.icu

TS:   for (const ch of s) { console.log(ch); }
来源：http://kmj.svipenyu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://erv.xziqi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wbu.cucudq.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rsz.hnxiangtu.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nmy.fktsv.cn

[E14] URL 编码与 Base64
来源：http://tps.cheryme.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jan.havefunace.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://hnd.gotoacloud.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ydq.yuanzhike.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://che.shanyushiyangtech.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qin.guannengcc.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rpw.shzxlz.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cdc.tianlin.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vcs.uphjek.com

[E15] HTML 转义 / 反转义
来源：http://lpc.sweek.top

Py:   html.escape(s);  html.unescape(s)
来源：http://urk.xuanzx.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qnj.fengsongda.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://shf.sysykeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://wjl.cqqwz.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ajt.fanxiaobao.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://osm.haohaochexian.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bwk.xingfuxueyuan.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fxg.hnqzz.top

[E16] 数字千分位
来源：http://vqk.xuanzx.com

Py:   f"{1234567:,}"
来源：http://jhm.fktsv.cn

PHP:  number_format(1234567);
来源：http://mik.fktsv.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://erw.zhixingplan.top

TS:   (1234567).toLocaleString("en-US")
来源：http://spf.uphjek.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://drp.xingfuxueyuan.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wkz.bbcook.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wnk.yj20258888.top

C#:   1234567.ToString("N0")
来源：http://fxq.sysykeji.top

[E17] 首字母大写
来源：http://dbr.guowangkeji.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kwo.tarul.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://asy.iojbl.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://scw.gotoacloud.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sun.0kj1m.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://auy.guowangkeji.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wnx.ctjpmb.com

Ruby: s.capitalize
来源：http://jwe.cheryme.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://uux.yongpay.top

[E18] 模板占位符替换
来源：http://glw.hywenlv.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ynm.jqgufenzy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ttb.hcnkem.com

JS:   tpl.replaceAll("{name}", name)
来源：http://qod.zhijiandao.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://gte.vqdsnc.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cae.aibaodan.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wac.epnwcf.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qdz.zhijiandao.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uil.tianlin.xyz

[E19] 多行文本按行拆分
来源：http://qgn.fktsv.cn

Py:   s.splitlines()
来源：http://www.daxiang520.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qcm.hammf.cn

JS:   s.split(/\r?\n/)
来源：http://abw.jinqigfzy.top

TS:   s.split(/\r?\n/)
来源：http://tiz.yonumen.top

Java: s.lines().toList()
来源：http://kmo.zhongyouzk.top

Go:   strings.Split(s, "\n")
来源：http://baq.gotoacloud.top

Ruby: s.lines
来源：http://veo.wangdashe.top

C#:   s.Split('\n')
来源：http://rbh.hcnkem.com

[E20] 判断字符串是否为空
来源：http://vkn.tianlin.xyz

Py:   if not s:
来源：http://ipx.ctjpmb.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qao.bjfxy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://owr.jlsjyb.cn

TS:   if (s === "") {}
来源：http://yug.gzhubu.top

Java: if (s.isEmpty()) {}
来源：http://xzv.aizwys.cn

Go:   if s == "" {}
来源：http://ztr.pycfn.com

Ruby: if s.empty?
来源：http://fad.vqdsnc.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hoo.kuanghao11.cn

[E21] 超长截断加省略号
来源：http://wpv.shanyushiyangtech.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://srt.yfazqb.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xzq.epnwcf.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bqg.daxiang520.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pkt.birdmap.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jhg.hfpthk.cn

Go:   // 按 rune 判断长度后截断
来源：http://jjv.snrcjt.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sdw.zhixingplan.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://maw.zhiwuduotai.top

[E22] 字节长度与字符长度
来源：http://dej.chenzaomai.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uuh.shanyushiyangtech.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nio.xinyue.icu

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rcs.svipenyu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jhb.zhaomingkeji.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bjr.0kj1m.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://trl.vqdsnc.cn

Ruby: s.bytesize;  s.length
来源：http://dyt.jyoumei.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zjo.hnqzz.top

================================================================================
来源：http://ayk.c1oappe.top

F. 文件与目录
来源：http://kjo.chenjidiqi.icu

================================================================================
来源：http://nsm.hongshengwenyu.top

[F01] 读取整个文件
来源：http://ijq.ydzc1.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://oxe.sufxvd.cn

PHP:  file_get_contents("a.txt");
来源：http://mrc.ctjpmb.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bpx.xinyue.icu

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wbf.jianghu66.top

Java: Files.readString(Path.of("a.txt"))
来源：http://uny.jianghu66.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gbe.guowangkeji.top

Ruby: File.read("a.txt")
来源：http://trz.jinyuanbaomall.cn

C#:   File.ReadAllText("a.txt");
来源：http://rem.tarul.cn

[F02] 逐行读取文件
来源：http://uaj.ctjpmb.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vsx.daxiang520.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rbi.wangdashe.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fwl.jinghuilouyu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bkg.hnqzz.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mff.aibaodan.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jik.sjlbkw.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gke.ywan-chungtsiang.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yar.fengsongda.top

[F03] 写入文件（覆盖）
来源：http://vpi.tanke756.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://axa.fehbvm.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://mwl.yueranfly.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zwf.yj20258.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rtp.jyoumei.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ijo.shzxlz.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qnf.shuidangran.top

Ruby: File.write("a.txt", "hi")
来源：http://gaf.xinyue.icu

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vke.pengpengdd.cyou

[F04] 追加写入文件
来源：http://evi.hcnkem.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tvy.zhaomingkeji.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bea.andypj.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://map.gaohongyu789.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qqc.jinghuilouyu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pep.fktsv.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://edl.zhiwuduotai.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nyq.uphjek.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dlj.fzhhl.top

[F05] 判断文件或目录是否存在
来源：http://cmj.chenlongwang.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://laj.guannengcc.top

PHP:  file_exists("a.txt");
来源：http://vve.xuetiantiany.cn

JS:   fs.existsSync("a.txt")
来源：http://djf.shanyushiyangtech.top

TS:   fs.existsSync("a.txt")
来源：http://ehy.fehbvm.com

Java: Files.exists(Path.of("a.txt"))
来源：http://opk.nanxuanxn.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zqj.tian-w.cn

Ruby: File.exist?("a.txt")
来源：http://tzy.aizwys.cn

C#:   File.Exists("a.txt")
来源：http://ltj.guowangkeji.top

[F06] 删除文件
来源：http://wno.snrcjt.cn

Py:   os.remove("a.txt")
来源：http://xbg.vqdsnc.cn

PHP:  unlink("a.txt");
来源：http://cdz.guannengcc.top

JS:   fs.unlinkSync("a.txt")
来源：http://ayu.shzxlz.cn

TS:   fs.unlinkSync("a.txt")
来源：http://cwu.zhijiandao.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ery.0kj1m.cn

Go:   os.Remove("a.txt")
来源：http://bcn.ehwqpu.com

Ruby: File.delete("a.txt")
来源：http://wjz.yfazqb.com

C#:   File.Delete("a.txt");
来源：http://hxg.cheryme.top

[F07] 创建目录（含多级）
来源：http://ehd.hywenlv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hgz.hysaishi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zcp.gotoacloud.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mlg.bjfxy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yqi.wangdashe.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wxz.quarkkingdee.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yvd.zdqjudy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://iis.redwolf501.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lnl.nwbrower.top

[F08] 遍历目录
来源：http://zqo.hysaishi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://rgv.vehdjk.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pli.yj20258888.top

JS:   fs.readdirSync("dir")
来源：http://nqn.ppjwa.cn

TS:   fs.readdirSync("dir")
来源：http://ujd.cucudq.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://anb.c1oappe.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://esy.jinghuilouyu.cn

Ruby: Dir.children("dir")
来源：http://gwy.meibo888.top

C#:   Directory.GetFiles("dir")
来源：http://kjb.jlsjyb.cn

[F09] 获取文件大小
来源：http://pup.52xcode.cn

Py:   os.path.getsize("a.txt")
来源：http://jpx.ppjwa.cn

PHP:  filesize("a.txt");
来源：http://bkn.ydjk.org.cn

JS:   fs.statSync("a.txt").size
来源：http://xkh.hysaishi.cn

TS:   fs.statSync("a.txt").size
来源：http://nge.svipenyu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://sul.zhiwuduotai.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pyb.yuanzhike.top

Ruby: File.size("a.txt")
来源：http://ctp.pengpengdd.cyou

C#:   new FileInfo("a.txt").Length
来源：http://abw.yuxming.cn

[F10] 取文件扩展名 / 文件名
来源：http://fiq.daria6918.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sxv.sysykeji.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://beu.aizwys.cn


<!-- 参考信息 -->