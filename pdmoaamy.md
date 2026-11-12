代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dek.c1oappe.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gbq.chenzaomai.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lgg.uphjek.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vpp.tanke756.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wyh.9152youxi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://njb.shanyushiyangtech.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://eph.jiagoushi.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yvh.epnwcf.com

[E02] 重复字符串
来源：http://gna.52xcode.cn

Py:   "ab" * 3
来源：http://wld.ydzc1.top

PHP:  str_repeat("ab", 3);
来源：http://pym.vehdjk.com

JS:   "ab".repeat(3)
来源：http://syh.hcnkem.com

TS:   "ab".repeat(3)
来源：http://dfy.dianchejie.cn

Java: "ab".repeat(3)
来源：http://oou.cheryme.top

Go:   strings.Repeat("ab", 3)
来源：http://huo.zycfv.cn

Ruby: "ab" * 3
来源：http://oxy.nanxuanxn.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mhi.gzhubu.top

[E03] 截取子串
来源：http://iwx.ydjk.org.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://grq.yangfankeji.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xwt.cucudq.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dam.yueranfly.top

TS:   s.slice(1, 4)
来源：http://hhv.zhoulong.xyz

Java: s.substring(1, 4)
来源：http://vqr.jinqigfzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zik.xuetiantiany.cn

Ruby: s[1, 3];  s[1..3]
来源：http://njg.zhoulong.xyz

C#:   s.Substring(1, 3)
来源：http://ama.zhongyouzk.top

[E04] 查找子串位置
来源：http://vts.haohaochexian.top

Py:   s.find("x");  s.index("x")
来源：http://rqp.ehwqpu.com

PHP:  strpos($s, "x");
来源：http://hpx.smart0.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fky.gotoacloud.top

TS:   s.indexOf("x")
来源：http://cks.jinyuanbaomall.cn

Java: s.indexOf("x")
来源：http://esw.vehdjk.com

Go:   strings.Index(s, "x")
来源：http://vvt.xuanzx.com

Ruby: s.index("x")
来源：http://seu.yueranfly.top

C#:   s.IndexOf("x")
来源：http://wdq.yj202588.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://lmd.hnqzz.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dct.meibo888.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sxh.cdnleiting.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qed.bbcook.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://rat.52xcode.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zid.redwolf501.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wig.aibaodan.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gmy.ehwqpu.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xle.guowangkeji.top

[E06] 替换子串
来源：http://ezb.yuxming.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ira.dianchejie.cn

PHP:  str_replace("a", "b", $s);
来源：http://dla.ivvv.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rjw.zhiwuduotai.top

TS:   s.replaceAll("a", "b")
来源：http://qig.jyoumei.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gjq.yfazqb.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jve.ehwqpu.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vdz.cashguo.top

C#:   s.Replace("a", "b")
来源：http://rle.fengsongda.top

[E07] 按分隔符拆分
来源：http://xku.quarkkingdee.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qet.hfpthk.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jmi.guowangkeji.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://xlk.316326.xyz

TS:   s.split(",")
来源：http://myb.pengpengdd.cyou

Java: s.split(",");  s.split("\\s+")
来源：http://bkq.fanxiaobao.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wyz.birdmap.top

Ruby: s.split(",");  s.split
来源：http://bgj.vqdsnc.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nvm.kuanghao11.cn

[E08] 数组按分隔符合并
来源：http://bqt.tarul.cn

Py:   ",".join(items)
来源：http://rig.hcnkem.com

PHP:  implode(",", $items);
来源：http://idn.zhaomingkeji.xyz

JS:   items.join(",")
来源：http://kfu.ydzc1.top

TS:   items.join(",")
来源：http://zct.yj20258888.top

Java: String.join(",", items)
来源：http://vgy.jianghu66.top

Go:   strings.Join(items, ",")
来源：http://guy.sweek.top

Ruby: items.join(",")
来源：http://vtk.yuanzhike.top

C#:   string.Join(",", items)
来源：http://gzj.fehbvm.com

[E09] 去除所有空白字符
来源：http://pxj.jianghu66.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yzs.mhx1999.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tcw.guowangkeji.top

JS:   s.replace(/\s+/g, "")
来源：http://xyg.uphjek.com

TS:   s.replace(/\s+/g, "")
来源：http://ixq.aibaodan.cn

Java: s.replaceAll("\\s+", "")
来源：http://dlf.jyoumei.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://jwq.jiagoushi.top

Ruby: s.gsub(/\s+/, "")
来源：http://mqd.xuetiantiany.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fwa.epnwcf.com

[E10] 左侧补零 / 定长填充
来源：http://cyt.vehdjk.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dby.hnqzz.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xnp.fehbvm.com

JS:   "7".padStart(3, "0")
来源：http://vux.xuetiantiany.cn

TS:   "7".padStart(3, "0")
来源：http://oyu.vehdjk.com

Java: String.format("%03d", 7)
来源：http://sgd.ctjpmb.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://ekq.dianchejie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pgo.sufxvd.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pud.zdbjq.cn

[E11] 反转字符串
来源：http://qhh.zdqjudy.top

Py:   s[::-1]
来源：http://bah.andypj.xyz

PHP:  strrev($s);
来源：http://axc.nanxinkj.top

JS:   [...s].reverse().join("")
来源：http://mxt.jinqigufen.top

TS:   [...s].reverse().join("")
来源：http://jcu.zhaomingkeji.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://qft.ivvv.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ozs.guowangkeji.top

Ruby: s.reverse
来源：http://qaf.tian-w.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zev.chenzaomai.com

[E12] 统计某字符出现次数
来源：http://fui.ywan-chungtsiang.top

Py:   s.count("a")
来源：http://rmv.ehwqpu.com

PHP:  substr_count($s, "a");
来源：http://cut.cucudq.cn

JS:   s.split("a").length - 1
来源：http://vgt.hysaishi.cn

TS:   s.split("a").length - 1
来源：http://kjz.hywenlv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hzl.gzhubu.top

Go:   strings.Count(s, "a")
来源：http://tzs.sweek.top

Ruby: s.count("a")
来源：http://tvy.sxryk.cn

C#:   s.Count(c => c == 'a')
来源：http://vea.haohaochexian.top

[E13] 逐字符遍历
来源：http://vep.wangshuangyany.cn

Py:   for ch in s: print(ch)
来源：http://opd.gotoacloud.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wob.shuidangran.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://mnm.hesvh.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bom.0kj1m.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cvy.zhaomingkeji.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ozu.vqdsnc.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://nlr.dianchejie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blg.feifeiyinyue.top

[E14] URL 编码与 Base64
来源：http://ors.tanke756.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://okj.guowangkeji.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://wkv.shzxlz.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hpc.cashguo.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wxx.sjlbkw.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ysk.zdbjq.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zum.daxiang520.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mpy.ydjk.org.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mge.chenjidiqi.icu

[E15] HTML 转义 / 反转义
来源：http://exo.fktsv.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hmv.zycfv.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://adj.jinqigufen.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mvu.nanxinkj.top

TS:   // 同上，务必做 XSS 过滤
来源：http://iho.jinqigufen.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mmd.cucudq.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qww.nwbrower.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hbv.yvedp.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tow.feifeiyinyue.top

[E16] 数字千分位
来源：http://iyg.yfazqb.com

Py:   f"{1234567:,}"
来源：http://pem.zhiwuduotai.top

PHP:  number_format(1234567);
来源：http://jda.haohaochexian.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ugu.ybcxt.top

TS:   (1234567).toLocaleString("en-US")
来源：http://rbz.zhoulong.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zhz.fengsongda.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://esf.fanxiaobao.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dwi.aibaodan.cn

C#:   1234567.ToString("N0")
来源：http://jix.xinyue.icu

[E17] 首字母大写
来源：http://jfr.nwbrower.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fkm.jianghu66.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://mkk.xziqi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hnk.316326.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xgb.hammf.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xnx.zhijiandao.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qky.jqgufenzy.top

Ruby: s.capitalize
来源：http://hwk.jqgufenzy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ttv.zdqjudy.top

[E18] 模板占位符替换
来源：http://azm.wangshuangyany.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gxl.jinghuilouyu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fvm.pycfn.com

JS:   tpl.replaceAll("{name}", name)
来源：http://wvt.zdbjq.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://zmg.yvedp.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zyu.c1oappe.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lop.guowangkeji.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dwo.ydjk.org.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xef.wangshuangyany.cn

[E19] 多行文本按行拆分
来源：http://zwu.hammf.cn

Py:   s.splitlines()
来源：http://qwg.shanyushiyangkeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://awa.hesvh.cn

JS:   s.split(/\r?\n/)
来源：http://rel.tianlin.xyz

TS:   s.split(/\r?\n/)
来源：http://meb.316326.xyz

Java: s.lines().toList()
来源：http://jtd.fehbvm.com

Go:   strings.Split(s, "\n")
来源：http://ltr.shanyushiyangkeji.top

Ruby: s.lines
来源：http://kdd.jqgufenzy.top

C#:   s.Split('\n')
来源：http://mgv.gogol.net.cn

[E20] 判断字符串是否为空
来源：http://fnn.yueranfly.top

Py:   if not s:
来源：http://asc.zhixingplan.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ohl.hnxiangtu.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ovx.guowangkeji.top

TS:   if (s === "") {}
来源：http://neo.gaohongyu789.top

Java: if (s.isEmpty()) {}
来源：http://fiu.redwolf501.top

Go:   if s == "" {}
来源：http://gcv.andypj.xyz

Ruby: if s.empty?
来源：http://jto.uphjek.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ilq.shuidangran.top

[E21] 超长截断加省略号
来源：http://xnv.shangyingyoupin.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xob.jinghuilouyu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gzk.zhengqikj.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cmq.yongpay.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://duu.nanxuanxn.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wxm.nwbrower.top

Go:   // 按 rune 判断长度后截断
来源：http://pqr.jinyuanbaomall.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blu.cashguo.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cza.sxryk.cn

[E22] 字节长度与字符长度
来源：http://djq.meibo888.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://aqp.hesvh.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aiu.sjlbkw.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://whg.xuanzx.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pyn.uphjek.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bez.shzxlz.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://acd.jianghu66.top

Ruby: s.bytesize;  s.length
来源：http://ifr.andypj.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pkt.fehbvm.com

================================================================================
来源：http://qqe.xingfuxueyuan.xyz

F. 文件与目录
来源：http://vww.pengpengdd.cyou

================================================================================
来源：http://ynm.yuanzhike.top

[F01] 读取整个文件
来源：http://lbl.snrcjt.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gla.smart0.xyz

PHP:  file_get_contents("a.txt");
来源：http://tyl.pengpengdd.cyou

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bfy.ybcxt.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ach.c1oappe.top

Java: Files.readString(Path.of("a.txt"))
来源：http://sfg.guowangkeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yex.daria6918.cn

Ruby: File.read("a.txt")
来源：http://wdb.jyoumei.cn

C#:   File.ReadAllText("a.txt");
来源：http://lpu.hammf.cn

[F02] 逐行读取文件
来源：http://eom.fengsongda.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rlo.ywan-chungtsiang.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rub.chenzaomai.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ndw.sysykeji.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bvo.tian-w.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pxv.ydzc1.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ozx.chenzaomai.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bpk.yonumen.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vhk.jiagoushi.top

[F03] 写入文件（覆盖）
来源：http://pld.pycfn.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zdj.jiagoushi.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://mhx.zycfv.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rae.xinyue.icu

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bbx.yanxiufei.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wmx.pycfn.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sdi.nwbrower.top

Ruby: File.write("a.txt", "hi")
来源：http://naj.jinqigufen.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tub.tian-w.cn

[F04] 追加写入文件
来源：http://nbo.nanxuanxn.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wbq.jiagoushi.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bhs.kuanghao11.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cgj.tanke756.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://quo.chenjidiqi.icu

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://clc.sweek.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://npe.hongshengwenyu.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cbf.uphjek.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xuv.yonumen.top

[F05] 判断文件或目录是否存在
来源：http://uqr.daxiang520.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nrk.mhx1999.top

PHP:  file_exists("a.txt");
来源：http://www.yuxming.cn

JS:   fs.existsSync("a.txt")
来源：http://ism.zdbjq.cn

TS:   fs.existsSync("a.txt")
来源：http://qzp.ybcxt.top

Java: Files.exists(Path.of("a.txt"))
来源：http://sqo.ehwqpu.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://edb.cashguo.top

Ruby: File.exist?("a.txt")
来源：http://vce.hnqzz.top

C#:   File.Exists("a.txt")
来源：http://knt.zhengqikj.top

[F06] 删除文件
来源：http://cqw.zhongyouzk.top

Py:   os.remove("a.txt")
来源：http://pjc.hywenlv.cn

PHP:  unlink("a.txt");
来源：http://afr.yueranfly.top

JS:   fs.unlinkSync("a.txt")
来源：http://cwb.yangfankeji.com

TS:   fs.unlinkSync("a.txt")
来源：http://cph.yanxiufei.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fuz.yueranfly.top

Go:   os.Remove("a.txt")
来源：http://dtv.cashguo.top

Ruby: File.delete("a.txt")
来源：http://pdh.316326.xyz

C#:   File.Delete("a.txt");
来源：http://epr.zhiwuduotai.top

[F07] 创建目录（含多级）
来源：http://mgq.jinyuanbaomall.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://iun.cashguo.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://obr.ivvv.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bns.ywan-chungtsiang.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://juy.chenlongwang.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ftb.wangdashe.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kle.yueranfly.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xiz.zdbjq.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hpy.daxiang520.top

[F08] 遍历目录
来源：http://dql.zhongyouzk.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://tws.dashuyun.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jkd.xuanzx.com

JS:   fs.readdirSync("dir")
来源：http://jep.jiagoushi.top

TS:   fs.readdirSync("dir")
来源：http://gse.gaohongyu789.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mec.gotoacloud.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://acy.yueranfly.top

Ruby: Dir.children("dir")
来源：http://vnk.andypj.xyz

C#:   Directory.GetFiles("dir")
来源：http://cbt.meibo888.top

[F09] 获取文件大小
来源：http://cxh.pengpengdd.cyou

Py:   os.path.getsize("a.txt")
来源：http://mzv.yvedp.cn

PHP:  filesize("a.txt");
来源：http://skg.nanxinkj.top

JS:   fs.statSync("a.txt").size
来源：http://kgo.zhijiandao.cn

TS:   fs.statSync("a.txt").size
来源：http://iyu.hammf.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lue.yj20258.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pfu.yj20258.top

Ruby: File.size("a.txt")
来源：http://nfv.yanxiufei.cn

C#:   new FileInfo("a.txt").Length
来源：http://lgw.zhengqikj.top

[F10] 取文件扩展名 / 文件名
来源：http://sfu.cashguo.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vhu.shanyushiyangkeji.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uho.shzxlz.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gke.iojbl.cn

TS:   path.extname("a.txt")
来源：http://ubq.dashuyun.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dei.jinqigufen.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ymd.gogol.net.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ggc.daria6918.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wlt.chenzaomai.com

[F11] 复制与移动文件
来源：http://yvv.jianghu66.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kub.jiagoushi.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vcs.hcnkem.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wbg.tianlin.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xir.tarul.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fle.xingfuxueyuan.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wyx.zhiwuduotai.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://job.guowangkeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jro.0kj1m.cn

[F12] CSV 读写
来源：http://rku.zhijiandao.cn


<!-- 参考信息 -->