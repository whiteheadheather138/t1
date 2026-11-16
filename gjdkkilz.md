代发 wailian999

PHP:  strpos($s, "x");
来源：http://xpa.ctjpmb.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://spc.fzhhl.top

TS:   s.indexOf("x")
来源：http://got.shuidangran.top

Java: s.indexOf("x")
来源：http://yyi.c1oappe.top

Go:   strings.Index(s, "x")
来源：http://zlg.guowangkeji.top

Ruby: s.index("x")
来源：http://zmg.jqgfzy.top

C#:   s.IndexOf("x")
来源：http://rql.xingfuxueyuan.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://ijg.hammf.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://igo.redwolf501.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bwb.zhaomingkeji.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hrs.cqqwz.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://gvg.chenjidiqi.icu

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iyy.jinqigfzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ajg.dianchejie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jvx.feifeiyinyue.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ben.fzhhl.top

[E06] 替换子串
来源：http://lin.ehwqpu.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fgz.xziqi.cn

PHP:  str_replace("a", "b", $s);
来源：http://mei.pengpengdd.cyou

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wmk.zdbjq.cn

TS:   s.replaceAll("a", "b")
来源：http://cmg.vqdsnc.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://loh.ivvv.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vdt.jinghuilouyu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jcb.ywan-chungtsiang.top

C#:   s.Replace("a", "b")
来源：http://nxs.zycfv.cn

[E07] 按分隔符拆分
来源：http://gpi.tarul.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hzo.guannengcc.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://izl.shanyushiyangkeji.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://nxz.yuxming.cn

TS:   s.split(",")
来源：http://pvl.shanyushiyangtech.top

Java: s.split(",");  s.split("\\s+")
来源：http://lzv.ehwqpu.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://plx.tarul.cn

Ruby: s.split(",");  s.split
来源：http://bma.fzhhl.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xsg.cdnleiting.top

[E08] 数组按分隔符合并
来源：http://bsn.jinghuilouyu.cn

Py:   ",".join(items)
来源：http://ass.uphjek.com

PHP:  implode(",", $items);
来源：http://meo.zdbjq.cn

JS:   items.join(",")
来源：http://xyw.fanxiaobao.xyz

TS:   items.join(",")
来源：http://bnr.zhengqikj.top

Java: String.join(",", items)
来源：http://eor.yangfankeji.com

Go:   strings.Join(items, ",")
来源：http://okw.yj202588.top

Ruby: items.join(",")
来源：http://sfs.svipenyu.cn

C#:   string.Join(",", items)
来源：http://qql.tanke756.top

[E09] 去除所有空白字符
来源：http://asq.jyoumei.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://adr.cdnleiting.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sqe.zhixingplan.top

JS:   s.replace(/\s+/g, "")
来源：http://voj.cucudq.cn

TS:   s.replace(/\s+/g, "")
来源：http://skk.zycfv.cn

Java: s.replaceAll("\\s+", "")
来源：http://ikb.hfpthk.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://pfl.andypj.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://wmz.gogol.net.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tiq.yongpay.top

[E10] 左侧补零 / 定长填充
来源：http://pzx.52xcode.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hgr.svipenyu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lqf.havefunace.top

JS:   "7".padStart(3, "0")
来源：http://xks.jlsjyb.cn

TS:   "7".padStart(3, "0")
来源：http://fel.52xcode.cn

Java: String.format("%03d", 7)
来源：http://rjb.sufxvd.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zlo.yj20258888.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jpx.xziqi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mza.vqdsnc.cn

[E11] 反转字符串
来源：http://uht.jianghu66.top

Py:   s[::-1]
来源：http://zfn.fktsv.cn

PHP:  strrev($s);
来源：http://lha.jinqigufen.top

JS:   [...s].reverse().join("")
来源：http://kqn.tanke756.top

TS:   [...s].reverse().join("")
来源：http://sbl.fzhhl.top

Java: new StringBuilder(s).reverse().toString()
来源：http://yuh.52xcode.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://omk.vehdjk.com

Ruby: s.reverse
来源：http://elb.xingfuxueyuan.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://xlh.aibaodan.cn

[E12] 统计某字符出现次数
来源：http://ugd.hywenlv.cn

Py:   s.count("a")
来源：http://erk.ivvv.top

PHP:  substr_count($s, "a");
来源：http://cio.c1oappe.top

JS:   s.split("a").length - 1
来源：http://hqk.yj202588.top

TS:   s.split("a").length - 1
来源：http://zlx.havefunace.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zqk.316326.xyz

Go:   strings.Count(s, "a")
来源：http://zim.sysykeji.top

Ruby: s.count("a")
来源：http://vou.daxiang520.top

C#:   s.Count(c => c == 'a')
来源：http://laf.sufxvd.cn

[E13] 逐字符遍历
来源：http://fpd.sxryk.cn

Py:   for ch in s: print(ch)
来源：http://wox.nanxuanxn.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bqr.shuidangran.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://yqp.9152youxi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://uuj.havefunace.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jue.jinqigufen.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wkp.52xcode.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://grw.daria6918.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pxj.xuetiantiany.cn

[E14] URL 编码与 Base64
来源：http://fvq.zdbjq.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rdt.shzxlz.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jsn.jinqigufen.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rug.shzxlz.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nsr.cheryme.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://sqy.yj202588.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sdw.birdmap.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://muz.sufxvd.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yzm.yangfankeji.com

[E15] HTML 转义 / 反转义
来源：http://gpy.dianchejie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://atb.jlsjyb.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wtk.tarul.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://daz.daria6918.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zvd.havefunace.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://drd.52xcode.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zoj.pengpengdd.cyou

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vxh.nanxuanxn.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wnt.jinqigufen.top

[E16] 数字千分位
来源：http://cva.cashguo.top

Py:   f"{1234567:,}"
来源：http://dyk.daxiang520.top

PHP:  number_format(1234567);
来源：http://zld.yangfankeji.com

JS:   (1234567).toLocaleString("en-US")
来源：http://ane.hcnkem.com

TS:   (1234567).toLocaleString("en-US")
来源：http://kws.cashguo.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://evr.ywan-chungtsiang.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rns.yanxiufei.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hfr.shanyushiyangkeji.top

C#:   1234567.ToString("N0")
来源：http://uwr.gzhubu.top

[E17] 首字母大写
来源：http://ucr.hysaishi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kao.sufxvd.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xaz.guannengcc.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://phg.iojbl.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kue.xziqi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nki.zhaomingkeji.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xzx.zhiwuduotai.top

Ruby: s.capitalize
来源：http://rhc.yj20258.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://itz.sufxvd.cn

[E18] 模板占位符替换
来源：http://vrj.shanyushiyangtech.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kaw.jinqigfzy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://whn.pycfn.com

JS:   tpl.replaceAll("{name}", name)
来源：http://mia.nanxuanxn.top

TS:   tpl.replaceAll("{name}", name)
来源：http://zrc.c1oappe.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kzz.vqdsnc.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kaz.yvedp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hrt.wangshuangyany.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wue.cucudq.cn

[E19] 多行文本按行拆分
来源：http://ovm.haohaochexian.top

Py:   s.splitlines()
来源：http://fpy.aibaodan.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://uwr.cashguo.top

JS:   s.split(/\r?\n/)
来源：http://wmr.52xcode.cn

TS:   s.split(/\r?\n/)
来源：http://rmy.pycfn.com

Java: s.lines().toList()
来源：http://bdd.jianghu66.top

Go:   strings.Split(s, "\n")
来源：http://eej.cucudq.cn

Ruby: s.lines
来源：http://ryz.jinqigfzy.top

C#:   s.Split('\n')
来源：http://vou.tarul.cn

[E20] 判断字符串是否为空
来源：http://mfa.jyoumei.cn

Py:   if not s:
来源：http://cgw.jinqigfzy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://crz.kuanghao11.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://soj.yvedp.cn

TS:   if (s === "") {}
来源：http://hom.ppjwa.cn

Java: if (s.isEmpty()) {}
来源：http://uzx.ydzc1.top

Go:   if s == "" {}
来源：http://dpf.tanke756.top

Ruby: if s.empty?
来源：http://eyy.yueranfly.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mhk.yuxming.cn

[E21] 超长截断加省略号
来源：http://xfv.aizwys.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tid.ydzc1.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://swz.tian-w.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ytd.ydzc1.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ksh.zhaomingkeji.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jog.sysykeji.top

Go:   // 按 rune 判断长度后截断
来源：http://dvg.jinghuilouyu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ben.yongpay.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://chp.dashuyun.cn

[E22] 字节长度与字符长度
来源：http://zep.vehdjk.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sxj.tian-w.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jzd.fktsv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jyk.yueranfly.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tav.ppjwa.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ump.nanxinkj.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bht.0kj1m.cn

Ruby: s.bytesize;  s.length
来源：http://hcn.zhixingplan.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://eof.yj202588.top

================================================================================
来源：http://ghq.52xcode.cn

F. 文件与目录
来源：http://qyt.zhoulong.xyz

================================================================================
来源：http://bjc.cashguo.top

[F01] 读取整个文件
来源：http://lwj.guannengcc.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wwu.dashuyun.cn

PHP:  file_get_contents("a.txt");
来源：http://der.jqgfzy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://itn.316326.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vqw.zhiwuduotai.top

Java: Files.readString(Path.of("a.txt"))
来源：http://zxq.yonumen.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://roz.ivvv.top

Ruby: File.read("a.txt")
来源：http://ukv.yangfankeji.com

C#:   File.ReadAllText("a.txt");
来源：http://yxe.havefunace.top

[F02] 逐行读取文件
来源：http://svm.hcnkem.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mnb.daria6918.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pic.hnxiangtu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ifq.shzxlz.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aij.mhx1999.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mzl.bjfxy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oyq.yuxming.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tbq.tianlin.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vtx.feifeiyinyue.top

[F03] 写入文件（覆盖）
来源：http://noc.jinghuilouyu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sti.cashguo.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://kqm.pengpengdd.cyou

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gmv.tarul.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vpl.birdmap.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sbv.ydjk.org.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://imi.havefunace.top

Ruby: File.write("a.txt", "hi")
来源：http://ayk.xylfe.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bhi.shzxlz.cn

[F04] 追加写入文件
来源：http://aph.sweek.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rab.zhaomingkeji.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zuf.jyoumei.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://flw.jqgfzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://buw.zhoulong.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kay.hfpthk.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ikk.shzxlz.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wib.gogol.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vfr.0kj1m.cn

[F05] 判断文件或目录是否存在
来源：http://mwc.sufxvd.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://foo.yangfankeji.com

PHP:  file_exists("a.txt");
来源：http://vso.cheryme.top

JS:   fs.existsSync("a.txt")
来源：http://uaa.birdmap.top

TS:   fs.existsSync("a.txt")
来源：http://dmj.gogol.net.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://eht.pycfn.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fus.jinghuilouyu.cn

Ruby: File.exist?("a.txt")
来源：http://fce.fehbvm.com

C#:   File.Exists("a.txt")
来源：http://wei.tanke756.top

[F06] 删除文件
来源：http://qfh.ivvv.top

Py:   os.remove("a.txt")
来源：http://zli.yj20258888.top

PHP:  unlink("a.txt");
来源：http://vzt.cucudq.cn

JS:   fs.unlinkSync("a.txt")
来源：http://npw.hesvh.cn

TS:   fs.unlinkSync("a.txt")
来源：http://iaw.fehbvm.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ddw.fktsv.cn

Go:   os.Remove("a.txt")
来源：http://wvu.havefunace.top

Ruby: File.delete("a.txt")
来源：http://fft.kuanghao11.cn

C#:   File.Delete("a.txt");
来源：http://pqf.yj202588.top

[F07] 创建目录（含多级）
来源：http://jex.xuanzx.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jck.guannengcc.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://grt.xuanzx.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://srb.vehdjk.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jei.yongpay.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://llg.gogol.net.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ynf.yuanzhike.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fjx.xylfe.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ers.sjlbkw.cn

[F08] 遍历目录
来源：http://vef.jinqigfzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://pfr.bbcook.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tuq.meibo888.top

JS:   fs.readdirSync("dir")
来源：http://vdl.sweek.top

TS:   fs.readdirSync("dir")
来源：http://pyu.snrcjt.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ejf.jinyuanbaomall.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://mex.daria6918.cn

Ruby: Dir.children("dir")
来源：http://cti.tanke756.top

C#:   Directory.GetFiles("dir")
来源：http://lsb.epnwcf.com

[F09] 获取文件大小
来源：http://lwm.zhijiandao.cn

Py:   os.path.getsize("a.txt")
来源：http://hwl.meibo888.top

PHP:  filesize("a.txt");
来源：http://ane.ppjwa.cn

JS:   fs.statSync("a.txt").size
来源：http://ype.meibo888.top

TS:   fs.statSync("a.txt").size
来源：http://lix.andypj.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://xqn.yfazqb.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dkt.zhiwuduotai.top

Ruby: File.size("a.txt")
来源：http://lta.cashguo.top

C#:   new FileInfo("a.txt").Length
来源：http://tkf.jqgufenzy.top

[F10] 取文件扩展名 / 文件名
来源：http://bkh.jinqigfzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://haj.sysykeji.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://afs.52xcode.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qaz.svipenyu.cn

TS:   path.extname("a.txt")
来源：http://mrn.sxryk.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gqf.c1oappe.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ajq.zhengqikj.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jri.zhixingplan.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mil.tanke756.top

[F11] 复制与移动文件
来源：http://nxu.hongshengwenyu.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vjn.ydjk.org.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qeb.sysykeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://soh.sufxvd.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zqe.c1oappe.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fhp.jinghuilouyu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sxv.dashuyun.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://klw.haohaochexian.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vzk.sxryk.cn

[F12] CSV 读写
来源：http://ddr.nanxuanxn.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jpy.yuxming.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qrt.ehwqpu.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kbk.bbcook.cn

TS:   // 同上
来源：http://bbo.guannengcc.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://efw.yj202588.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pnq.yonumen.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zgd.yangfankeji.com

C#:   // 无内置：用 CsvHelper 库
来源：http://izf.svipenyu.cn

================================================================================
来源：http://gez.pycfn.com

G. 面向对象
来源：http://cdb.guannengcc.top

================================================================================
来源：http://lhs.jlsjyb.cn

[G01] 定义类
来源：http://asv.kuanghao11.cn

Py:   class User: pass
来源：http://mmi.tian-w.cn

PHP:  class User {}
来源：http://lqf.haohaochexian.top

JS:   class User {}
来源：http://uqu.sysykeji.top

TS:   class User { name: string = ""; }
来源：http://ein.jqgufenzy.top

Java: class User {}
来源：http://xqu.haohaochexian.top

Go:   type User struct { Name string }
来源：http://rek.zhijiandao.cn

Ruby: class User; end
来源：http://fya.ydjk.org.cn

C#:   class User {}
来源：http://rmv.daria6918.cn

[G02] 构造函数
来源：http://wnx.dashuyun.cn

Py:   def __init__(self, name): self.name = name
来源：http://qna.jlsjyb.cn

PHP:  public function __construct(public string $name) {}
来源：http://ith.yangfankeji.com

JS:   constructor(name) { this.name = name; }
来源：http://fbj.cashguo.top

TS:   constructor(public name: string) {}
来源：http://ohx.gaohongyu789.top

Java: User(String name) { this.name = name; }
来源：http://atk.xinyue.icu

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lsn.ydzc1.top

Ruby: def initialize(name); @name = name; end
来源：http://bqb.fehbvm.com


<!-- 参考信息 -->