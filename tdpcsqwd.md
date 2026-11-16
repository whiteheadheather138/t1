代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yhy.nanxinkj.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cpi.guowangkeji.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ovr.gogol.net.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dzs.fanxiaobao.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cuf.birdmap.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://oif.fzhhl.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bqo.0kj1m.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qha.ydjk.org.cn

[E02] 重复字符串
来源：http://qrx.andypj.xyz

Py:   "ab" * 3
来源：http://iqp.nwbrower.top

PHP:  str_repeat("ab", 3);
来源：http://cdv.ehwqpu.com

JS:   "ab".repeat(3)
来源：http://xip.dashuyun.cn

TS:   "ab".repeat(3)
来源：http://kot.havefunace.top

Java: "ab".repeat(3)
来源：http://uxx.sufxvd.cn

Go:   strings.Repeat("ab", 3)
来源：http://qdj.yuxming.cn

Ruby: "ab" * 3
来源：http://vxl.xuanzx.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wcc.cdnleiting.top

[E03] 截取子串
来源：http://mwq.guannengcc.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://omx.xingfuxueyuan.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bea.jqgfzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cze.dianchejie.cn

TS:   s.slice(1, 4)
来源：http://bdy.sjlbkw.cn

Java: s.substring(1, 4)
来源：http://bzp.zycfv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pfm.pycfn.com

Ruby: s[1, 3];  s[1..3]
来源：http://ffc.tarul.cn

C#:   s.Substring(1, 3)
来源：http://ehb.jqgufenzy.top

[E04] 查找子串位置
来源：http://psc.cucudq.cn

Py:   s.find("x");  s.index("x")
来源：http://wbc.zycfv.cn

PHP:  strpos($s, "x");
来源：http://jtq.chenzaomai.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gmv.uphjek.com

TS:   s.indexOf("x")
来源：http://cll.zhiwuduotai.top

Java: s.indexOf("x")
来源：http://wtn.snrcjt.cn

Go:   strings.Index(s, "x")
来源：http://mry.aizwys.cn

Ruby: s.index("x")
来源：http://tsw.yj20258.top

C#:   s.IndexOf("x")
来源：http://odb.hfpthk.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ysx.iojbl.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qce.ppjwa.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://oec.52xcode.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fcm.svipenyu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://wzb.daxiang520.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lsm.zycfv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://add.zhoulong.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ayd.wangdashe.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kso.ctjpmb.com

[E06] 替换子串
来源：http://nik.cqqwz.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://aro.bjfxy.top

PHP:  str_replace("a", "b", $s);
来源：http://qyq.yj20258.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://njw.gogol.net.cn

TS:   s.replaceAll("a", "b")
来源：http://kjx.jyoumei.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xbe.hesvh.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ile.ywan-chungtsiang.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://con.ehwqpu.com

C#:   s.Replace("a", "b")
来源：http://wab.gotoacloud.top

[E07] 按分隔符拆分
来源：http://kpj.xingfuxueyuan.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kfd.cashguo.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://iqv.hammf.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fpt.jyoumei.cn

TS:   s.split(",")
来源：http://rji.birdmap.top

Java: s.split(",");  s.split("\\s+")
来源：http://wey.yongpay.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bde.sysykeji.top

Ruby: s.split(",");  s.split
来源：http://mrs.shzxlz.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://prg.jlsjyb.cn

[E08] 数组按分隔符合并
来源：http://uot.cheryme.top

Py:   ",".join(items)
来源：http://gjl.xinyue.icu

PHP:  implode(",", $items);
来源：http://mem.vehdjk.com

JS:   items.join(",")
来源：http://fxa.nwbrower.top

TS:   items.join(",")
来源：http://bic.ivvv.top

Java: String.join(",", items)
来源：http://nna.jinqigufen.top

Go:   strings.Join(items, ",")
来源：http://cmp.fehbvm.com

Ruby: items.join(",")
来源：http://dsg.sysykeji.top

C#:   string.Join(",", items)
来源：http://wpt.shanyushiyangtech.top

[E09] 去除所有空白字符
来源：http://doi.gogol.net.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ekh.zhongyouzk.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lxd.yj202588.top

JS:   s.replace(/\s+/g, "")
来源：http://pea.nwbrower.top

TS:   s.replace(/\s+/g, "")
来源：http://stm.gogol.net.cn

Java: s.replaceAll("\\s+", "")
来源：http://nni.xingfuxueyuan.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://jok.shuidangran.top

Ruby: s.gsub(/\s+/, "")
来源：http://qhv.xinyue.icu

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nba.sxryk.cn

[E10] 左侧补零 / 定长填充
来源：http://xcz.0kj1m.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nzd.sxryk.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mwf.pycfn.com

JS:   "7".padStart(3, "0")
来源：http://ixs.vqdsnc.cn

TS:   "7".padStart(3, "0")
来源：http://hsg.smart0.xyz

Java: String.format("%03d", 7)
来源：http://cvc.haohaochexian.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://sqg.zhaomingkeji.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sbn.gzhubu.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mrg.zycfv.cn

[E11] 反转字符串
来源：http://vwc.tian-w.cn

Py:   s[::-1]
来源：http://tcf.aizwys.cn

PHP:  strrev($s);
来源：http://sfc.tarul.cn

JS:   [...s].reverse().join("")
来源：http://mrd.andypj.xyz

TS:   [...s].reverse().join("")
来源：http://dyw.redwolf501.top

Java: new StringBuilder(s).reverse().toString()
来源：http://inz.316326.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://whg.andypj.xyz

Ruby: s.reverse
来源：http://gsj.jianghu66.top

C#:   new string(s.Reverse().ToArray())
来源：http://nei.chenjidiqi.icu

[E12] 统计某字符出现次数
来源：http://zed.vehdjk.com

Py:   s.count("a")
来源：http://hpg.shuidangran.top

PHP:  substr_count($s, "a");
来源：http://uyg.redwolf501.top

JS:   s.split("a").length - 1
来源：http://bht.fktsv.cn

TS:   s.split("a").length - 1
来源：http://wlk.hesvh.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rnx.hammf.cn

Go:   strings.Count(s, "a")
来源：http://cry.birdmap.top

Ruby: s.count("a")
来源：http://afm.jyoumei.cn

C#:   s.Count(c => c == 'a')
来源：http://kke.chenjidiqi.icu

[E13] 逐字符遍历
来源：http://slf.jinghuilouyu.cn

Py:   for ch in s: print(ch)
来源：http://oxf.tian-w.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tsq.pycfn.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://csx.gaohongyu789.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://aep.zhoulong.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tol.nanxuanxn.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uwu.uphjek.com

Ruby: s.each_char { |ch| puts ch }
来源：http://vjo.uphjek.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zed.sweek.top

[E14] URL 编码与 Base64
来源：http://smm.feifeiyinyue.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jjk.zhongyouzk.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://kdv.gaohongyu789.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qtp.sysykeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qug.yj202588.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fya.zhaomingkeji.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wzj.gotoacloud.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wri.yongpay.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qoj.yfazqb.com

[E15] HTML 转义 / 反转义
来源：http://rrr.aibaodan.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://flu.svipenyu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://noo.ywan-chungtsiang.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jhz.iojbl.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://bhl.fzhhl.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pml.tianlin.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lrg.jianghu66.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ykw.wangdashe.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cse.ivvv.top

[E16] 数字千分位
来源：http://fpr.shanyushiyangkeji.top

Py:   f"{1234567:,}"
来源：http://bzw.fengsongda.top

PHP:  number_format(1234567);
来源：http://kxf.feifeiyinyue.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ydz.hesvh.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gtu.mhx1999.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lnz.bjfxy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nsl.yfazqb.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cvw.gaohongyu789.top

C#:   1234567.ToString("N0")
来源：http://rfh.aibaodan.cn

[E17] 首字母大写
来源：http://zpi.yanxiufei.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://srp.yuanzhike.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://geg.dianchejie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dpq.hnxiangtu.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://emd.xinyue.icu

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://geu.hongshengwenyu.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kvw.yongpay.top

Ruby: s.capitalize
来源：http://cyg.bjfxy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fse.hnxiangtu.top

[E18] 模板占位符替换
来源：http://hov.guowangkeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://elb.xziqi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ham.jinyuanbaomall.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zjp.bjfxy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://jzb.yonumen.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hkq.haohaochexian.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vmn.hammf.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fpl.yj20258888.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ava.nwbrower.top

[E19] 多行文本按行拆分
来源：http://fyb.zhongyouzk.top

Py:   s.splitlines()
来源：http://xyl.meibo888.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://aez.yueranfly.top

JS:   s.split(/\r?\n/)
来源：http://pwz.xuetiantiany.cn

TS:   s.split(/\r?\n/)
来源：http://yyq.shanyushiyangtech.top

Java: s.lines().toList()
来源：http://arw.zhoulong.xyz

Go:   strings.Split(s, "\n")
来源：http://hfz.shzxlz.cn

Ruby: s.lines
来源：http://zuj.jianghu66.top

C#:   s.Split('\n')
来源：http://qlb.guowangkeji.top

[E20] 判断字符串是否为空
来源：http://osw.jinyuanbaomall.cn

Py:   if not s:
来源：http://cab.xuetiantiany.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ban.jinqigfzy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bgn.quarkkingdee.top

TS:   if (s === "") {}
来源：http://dna.tarul.cn

Java: if (s.isEmpty()) {}
来源：http://pzv.zhaomingkeji.xyz

Go:   if s == "" {}
来源：http://umy.cucudq.cn

Ruby: if s.empty?
来源：http://wjk.ybcxt.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mzo.yfazqb.com

[E21] 超长截断加省略号
来源：http://cdl.yangfankeji.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cag.9152youxi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hhi.yongpay.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ajg.chenzaomai.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sgv.jinyuanbaomall.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qje.svipenyu.cn

Go:   // 按 rune 判断长度后截断
来源：http://hcx.yuxming.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vtp.nanxinkj.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dcp.shangyingyoupin.top

[E22] 字节长度与字符长度
来源：http://izp.yanxiufei.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tsq.c1oappe.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dgk.ywan-chungtsiang.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zgw.kuanghao11.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://env.9152youxi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rxd.jqgfzy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gau.bjfxy.top

Ruby: s.bytesize;  s.length
来源：http://avy.sjlbkw.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qyz.shangyingyoupin.top

================================================================================
来源：http://yuf.redwolf501.top

F. 文件与目录
来源：http://ony.yuanzhike.top

================================================================================
来源：http://xsr.shangyingyoupin.top

[F01] 读取整个文件
来源：http://ucx.haohaochexian.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://isx.zhixingplan.top

PHP:  file_get_contents("a.txt");
来源：http://dlg.yuanzhike.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://efq.birdmap.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://afb.jinqigfzy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://kby.shanyushiyangtech.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ygx.zhijiandao.cn

Ruby: File.read("a.txt")
来源：http://sxp.0kj1m.cn

C#:   File.ReadAllText("a.txt");
来源：http://qph.ydzc1.top

[F02] 逐行读取文件
来源：http://zdp.iojbl.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wka.ywan-chungtsiang.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://oxx.hnxiangtu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wil.ppjwa.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xzq.xinyue.icu

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mmv.zhoulong.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lgz.chenjidiqi.icu

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tvy.xuanzx.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lfr.jqgfzy.top

[F03] 写入文件（覆盖）
来源：http://uwk.zhongyouzk.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hzm.chenjidiqi.icu

PHP:  file_put_contents("a.txt", "hi");
来源：http://cgk.shangyingyoupin.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mof.xziqi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://amo.daxiang520.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ull.jlsjyb.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fmn.pycfn.com

Ruby: File.write("a.txt", "hi")
来源：http://mpi.jianghu66.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qwf.andypj.xyz

[F04] 追加写入文件
来源：http://qqs.havefunace.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nps.haohaochexian.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pah.fktsv.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jhs.zhaomingkeji.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fse.zhiwuduotai.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sle.epnwcf.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zhr.gaohongyu789.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rik.hysaishi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://owz.sysykeji.top

[F05] 判断文件或目录是否存在
来源：http://ktv.zhengqikj.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ari.sjlbkw.cn

PHP:  file_exists("a.txt");
来源：http://ktq.sweek.top

JS:   fs.existsSync("a.txt")
来源：http://pkv.jinqigfzy.top

TS:   fs.existsSync("a.txt")
来源：http://gbc.fktsv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://cvk.vqdsnc.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dfu.0kj1m.cn

Ruby: File.exist?("a.txt")
来源：http://gwp.vqdsnc.cn

C#:   File.Exists("a.txt")
来源：http://iek.daria6918.cn

[F06] 删除文件
来源：http://auf.iojbl.cn

Py:   os.remove("a.txt")
来源：http://zqb.ybcxt.top

PHP:  unlink("a.txt");
来源：http://qmm.vqdsnc.cn

JS:   fs.unlinkSync("a.txt")
来源：http://bbu.yuanzhike.top

TS:   fs.unlinkSync("a.txt")
来源：http://gnd.cheryme.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hwt.sxryk.cn

Go:   os.Remove("a.txt")
来源：http://umn.hfpthk.cn

Ruby: File.delete("a.txt")
来源：http://can.cucudq.cn

C#:   File.Delete("a.txt");
来源：http://dky.redwolf501.top

[F07] 创建目录（含多级）
来源：http://oea.yj20258888.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dpw.shanyushiyangkeji.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gvl.hesvh.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fwt.zhengqikj.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dro.fengsongda.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ncs.kuanghao11.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zec.yj202588.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dds.redwolf501.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xiv.tianlin.xyz

[F08] 遍历目录
来源：http://ihn.yj202588.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ikg.nanxinkj.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ixl.guannengcc.top

JS:   fs.readdirSync("dir")
来源：http://bnh.316326.xyz

TS:   fs.readdirSync("dir")
来源：http://ucc.shanyushiyangkeji.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zjh.fengsongda.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://uvr.quarkkingdee.top

Ruby: Dir.children("dir")
来源：http://zws.ybcxt.top

C#:   Directory.GetFiles("dir")
来源：http://jne.uphjek.com

[F09] 获取文件大小
来源：http://wke.ywan-chungtsiang.top

Py:   os.path.getsize("a.txt")
来源：http://wld.daxiang520.top

PHP:  filesize("a.txt");
来源：http://ltb.xuanzx.com

JS:   fs.statSync("a.txt").size
来源：http://ibq.sufxvd.cn

TS:   fs.statSync("a.txt").size
来源：http://oqb.tanke756.top

Java: Files.size(Path.of("a.txt"))
来源：http://blj.snrcjt.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ksk.yangfankeji.com

Ruby: File.size("a.txt")
来源：http://sua.zhongyouzk.top

C#:   new FileInfo("a.txt").Length
来源：http://onw.nanxuanxn.top

[F10] 取文件扩展名 / 文件名
来源：http://hzd.316326.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dxd.sysykeji.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gcl.gogol.net.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ynh.guannengcc.top

TS:   path.extname("a.txt")
来源：http://rqa.yj202588.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://peb.smart0.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rhf.zhongyouzk.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ebt.hfpthk.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hxi.cqqwz.cn

[F11] 复制与移动文件
来源：http://pdu.yongpay.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://abk.bjfxy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vqb.hammf.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cox.ivvv.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zmb.sxryk.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fsz.gotoacloud.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jey.shangyingyoupin.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hay.redwolf501.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://amz.shuidangran.top

[F12] CSV 读写
来源：http://dem.xinyue.icu


<!-- 参考信息 -->