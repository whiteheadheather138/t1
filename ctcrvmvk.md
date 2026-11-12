代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://wxi.pycfn.com

C#:   s.Substring(1, 3)
来源：http://pfc.havefunace.top

[E04] 查找子串位置
来源：http://mpp.zdbjq.cn

Py:   s.find("x");  s.index("x")
来源：http://lvt.chenjidiqi.icu

PHP:  strpos($s, "x");
来源：http://ybt.dianchejie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://biu.xuanzx.com

TS:   s.indexOf("x")
来源：http://vwj.hywenlv.cn

Java: s.indexOf("x")
来源：http://mci.yongpay.top

Go:   strings.Index(s, "x")
来源：http://dht.sysykeji.top

Ruby: s.index("x")
来源：http://rer.guowangkeji.top

C#:   s.IndexOf("x")
来源：http://xor.daria6918.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://dhd.uphjek.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://adf.fzhhl.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vto.daria6918.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vyt.yonumen.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ecg.fehbvm.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gof.xylfe.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rbs.bjfxy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rqb.xziqi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vei.52xcode.cn

[E06] 替换子串
来源：http://cuj.nanxuanxn.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hiw.9152youxi.cn

PHP:  str_replace("a", "b", $s);
来源：http://erv.ppjwa.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kot.shuidangran.top

TS:   s.replaceAll("a", "b")
来源：http://ovp.zhoulong.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://myq.yuanzhike.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wfb.xinyue.icu

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jao.bjfxy.top

C#:   s.Replace("a", "b")
来源：http://ujc.hammf.cn

[E07] 按分隔符拆分
来源：http://gpu.zhongyouzk.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qtd.zhiwuduotai.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fzu.redwolf501.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://sen.aibaodan.cn

TS:   s.split(",")
来源：http://sil.jinyuanbaomall.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sxy.yvedp.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qcr.cqqwz.cn

Ruby: s.split(",");  s.split
来源：http://owq.tian-w.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zgp.kuanghao11.cn

[E08] 数组按分隔符合并
来源：http://jku.haohaochexian.top

Py:   ",".join(items)
来源：http://tro.sweek.top

PHP:  implode(",", $items);
来源：http://suv.nwbrower.top

JS:   items.join(",")
来源：http://eed.zhaomingkeji.xyz

TS:   items.join(",")
来源：http://vzi.xziqi.cn

Java: String.join(",", items)
来源：http://tpg.fktsv.cn

Go:   strings.Join(items, ",")
来源：http://bby.zhongyouzk.top

Ruby: items.join(",")
来源：http://dyi.ydzc1.top

C#:   string.Join(",", items)
来源：http://jcc.daxiang520.top

[E09] 去除所有空白字符
来源：http://cdt.cheryme.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qqc.zhixingplan.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://htu.andypj.xyz

JS:   s.replace(/\s+/g, "")
来源：http://raw.jinghuilouyu.cn

TS:   s.replace(/\s+/g, "")
来源：http://jxo.gogol.net.cn

Java: s.replaceAll("\\s+", "")
来源：http://ztz.dianchejie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ocl.hesvh.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kdn.xinyue.icu

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dlh.yfazqb.com

[E10] 左侧补零 / 定长填充
来源：http://vwx.xuanzx.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xpn.tian-w.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gbo.sysykeji.top

JS:   "7".padStart(3, "0")
来源：http://zmh.jinghuilouyu.cn

TS:   "7".padStart(3, "0")
来源：http://xyr.snrcjt.cn

Java: String.format("%03d", 7)
来源：http://rzp.hnxiangtu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://zva.nwbrower.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kvn.ybcxt.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qgb.316326.xyz

[E11] 反转字符串
来源：http://qiq.cashguo.top

Py:   s[::-1]
来源：http://epa.52xcode.cn

PHP:  strrev($s);
来源：http://kcu.jqgufenzy.top

JS:   [...s].reverse().join("")
来源：http://hpm.gaohongyu789.top

TS:   [...s].reverse().join("")
来源：http://isn.xingfuxueyuan.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://lts.ehwqpu.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://xtn.hcnkem.com

Ruby: s.reverse
来源：http://zak.fengsongda.top

C#:   new string(s.Reverse().ToArray())
来源：http://ppd.dianchejie.cn

[E12] 统计某字符出现次数
来源：http://kcb.yj202588.top

Py:   s.count("a")
来源：http://suq.ybcxt.top

PHP:  substr_count($s, "a");
来源：http://xdu.aibaodan.cn

JS:   s.split("a").length - 1
来源：http://xsh.yanxiufei.cn

TS:   s.split("a").length - 1
来源：http://ssm.sxryk.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://flv.vehdjk.com

Go:   strings.Count(s, "a")
来源：http://goi.zycfv.cn

Ruby: s.count("a")
来源：http://ycj.hesvh.cn

C#:   s.Count(c => c == 'a')
来源：http://ero.uphjek.com

[E13] 逐字符遍历
来源：http://ecc.havefunace.top

Py:   for ch in s: print(ch)
来源：http://ync.chenlongwang.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bjo.yj20258888.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://eoh.cdnleiting.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://jqk.jinghuilouyu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://imj.cheryme.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vzm.jinqigufen.top

Ruby: s.each_char { |ch| puts ch }
来源：http://oud.shzxlz.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gnw.xinyue.icu

[E14] URL 编码与 Base64
来源：http://hbh.shzxlz.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qsg.hcnkem.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://iyz.chenzaomai.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://utz.nanxinkj.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dmm.yongpay.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ogd.xuetiantiany.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mwv.pengpengdd.cyou

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pyf.tanke756.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rao.ybcxt.top

[E15] HTML 转义 / 反转义
来源：http://stf.nanxuanxn.top

Py:   html.escape(s);  html.unescape(s)
来源：http://qdp.hywenlv.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mti.cheryme.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dgg.tianlin.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://nat.jinyuanbaomall.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dal.yj20258.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ytf.ybcxt.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://isv.yonumen.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vdj.chenzaomai.com

[E16] 数字千分位
来源：http://wch.jinqigufen.top

Py:   f"{1234567:,}"
来源：http://ent.gzhubu.top

PHP:  number_format(1234567);
来源：http://tam.andypj.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://bhk.andypj.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://qok.fanxiaobao.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sbi.uphjek.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zep.yonumen.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bwq.xinyue.icu

C#:   1234567.ToString("N0")
来源：http://quh.ivvv.top

[E17] 首字母大写
来源：http://gvz.fehbvm.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://min.guowangkeji.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://yfb.daxiang520.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zgo.fengsongda.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rpe.kuanghao11.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://luy.yonumen.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vwx.fzhhl.top

Ruby: s.capitalize
来源：http://tcm.yj20258888.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://knj.chenlongwang.top

[E18] 模板占位符替换
来源：http://msc.zhengqikj.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ixh.hammf.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xnz.birdmap.top

JS:   tpl.replaceAll("{name}", name)
来源：http://yuu.yj20258888.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ovl.quarkkingdee.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xfz.yongpay.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yfd.gzhubu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rpz.yanxiufei.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cql.smart0.xyz

[E19] 多行文本按行拆分
来源：http://wnz.zhengqikj.top

Py:   s.splitlines()
来源：http://rkd.9152youxi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gvh.daria6918.cn

JS:   s.split(/\r?\n/)
来源：http://via.52xcode.cn

TS:   s.split(/\r?\n/)
来源：http://jxp.bbcook.cn

Java: s.lines().toList()
来源：http://fuh.tanke756.top

Go:   strings.Split(s, "\n")
来源：http://ejd.chenjidiqi.icu

Ruby: s.lines
来源：http://twe.zhixingplan.top

C#:   s.Split('\n')
来源：http://qkp.yonumen.top

[E20] 判断字符串是否为空
来源：http://mrk.chenlongwang.top

Py:   if not s:
来源：http://djd.gotoacloud.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://noq.chenjidiqi.icu

JS:   if (s === "") {} 或 if (!s) {}
来源：http://oyr.yonumen.top

TS:   if (s === "") {}
来源：http://yjv.gotoacloud.top

Java: if (s.isEmpty()) {}
来源：http://imz.iojbl.cn

Go:   if s == "" {}
来源：http://nwg.hongshengwenyu.top

Ruby: if s.empty?
来源：http://hoq.fktsv.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://eiv.yangfankeji.com

[E21] 超长截断加省略号
来源：http://fyo.ctjpmb.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mkl.vehdjk.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ttn.redwolf501.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wmz.316326.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ygk.wangdashe.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vcc.fktsv.cn

Go:   // 按 rune 判断长度后截断
来源：http://eyk.xziqi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mxu.zhixingplan.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mvv.dianchejie.cn

[E22] 字节长度与字符长度
来源：http://wbl.redwolf501.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vhd.316326.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://svi.shuidangran.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ufv.snrcjt.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ebo.nanxinkj.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rrd.yj202588.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bxl.bjfxy.top

Ruby: s.bytesize;  s.length
来源：http://brd.yfazqb.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pey.tanke756.top

================================================================================
来源：http://kme.zhaomingkeji.xyz

F. 文件与目录
来源：http://eoe.havefunace.top

================================================================================
来源：http://gri.sxryk.cn

[F01] 读取整个文件
来源：http://vjh.yj20258888.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fqp.tarul.cn

PHP:  file_get_contents("a.txt");
来源：http://ccb.sysykeji.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bum.havefunace.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mdd.xingfuxueyuan.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://ruw.bbcook.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uqh.jinyuanbaomall.cn

Ruby: File.read("a.txt")
来源：http://jva.shanyushiyangtech.top

C#:   File.ReadAllText("a.txt");
来源：http://puc.xingfuxueyuan.xyz

[F02] 逐行读取文件
来源：http://usi.redwolf501.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kke.svipenyu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://saz.yanxiufei.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vuq.feifeiyinyue.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fda.dianchejie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://amf.zhengqikj.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cfr.zhaomingkeji.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://stc.epnwcf.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nsy.shanyushiyangkeji.top

[F03] 写入文件（覆盖）
来源：http://hdq.pengpengdd.cyou

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kuy.jyoumei.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yju.chenjidiqi.icu

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bol.ctjpmb.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blx.hongshengwenyu.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yrn.tarul.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pem.zdbjq.cn

Ruby: File.write("a.txt", "hi")
来源：http://agb.hnqzz.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zbn.smart0.xyz

[F04] 追加写入文件
来源：http://roe.jiagoushi.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://leh.cqqwz.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://klj.cashguo.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nqe.ywan-chungtsiang.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://anx.xingfuxueyuan.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zum.ehwqpu.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gqu.fehbvm.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cem.ivvv.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fzo.yuxming.cn

[F05] 判断文件或目录是否存在
来源：http://ncv.zdbjq.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://srx.yuxming.cn

PHP:  file_exists("a.txt");
来源：http://hto.iojbl.cn

JS:   fs.existsSync("a.txt")
来源：http://xzg.sjlbkw.cn

TS:   fs.existsSync("a.txt")
来源：http://mec.yueranfly.top

Java: Files.exists(Path.of("a.txt"))
来源：http://kpi.jlsjyb.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ouv.mhx1999.top

Ruby: File.exist?("a.txt")
来源：http://xru.ctjpmb.com

C#:   File.Exists("a.txt")
来源：http://euj.hesvh.cn

[F06] 删除文件
来源：http://ivw.yongpay.top

Py:   os.remove("a.txt")
来源：http://aap.yj20258888.top

PHP:  unlink("a.txt");
来源：http://rmr.andypj.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://xpe.jqgufenzy.top

TS:   fs.unlinkSync("a.txt")
来源：http://icw.yuxming.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xaw.jinqigfzy.top

Go:   os.Remove("a.txt")
来源：http://zws.ctjpmb.com

Ruby: File.delete("a.txt")
来源：http://gko.xinyue.icu

C#:   File.Delete("a.txt");
来源：http://fzr.cheryme.top

[F07] 创建目录（含多级）
来源：http://fty.316326.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://huh.ppjwa.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zkd.chenlongwang.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mpm.sxryk.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yby.jinyuanbaomall.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rqs.dashuyun.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ifd.jinghuilouyu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zff.jianghu66.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://idq.cheryme.top

[F08] 遍历目录
来源：http://rwh.gaohongyu789.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://oho.ywan-chungtsiang.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://eks.jlsjyb.cn

JS:   fs.readdirSync("dir")
来源：http://esu.ywan-chungtsiang.top

TS:   fs.readdirSync("dir")
来源：http://czu.fehbvm.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cwx.iojbl.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bkg.xylfe.cn

Ruby: Dir.children("dir")
来源：http://aze.ppjwa.cn

C#:   Directory.GetFiles("dir")
来源：http://dug.quarkkingdee.top

[F09] 获取文件大小
来源：http://nop.yanxiufei.cn

Py:   os.path.getsize("a.txt")
来源：http://gbs.jyoumei.cn

PHP:  filesize("a.txt");
来源：http://rdh.zhiwuduotai.top

JS:   fs.statSync("a.txt").size
来源：http://pvl.bjfxy.top

TS:   fs.statSync("a.txt").size
来源：http://zog.svipenyu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gzd.hysaishi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zer.hongshengwenyu.top

Ruby: File.size("a.txt")
来源：http://fnf.52xcode.cn

C#:   new FileInfo("a.txt").Length
来源：http://jsh.zdbjq.cn

[F10] 取文件扩展名 / 文件名
来源：http://bfg.gogol.net.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qxn.epnwcf.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uss.fehbvm.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fmk.yueranfly.top

TS:   path.extname("a.txt")
来源：http://rnz.zhoulong.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hzi.meibo888.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rgw.jyoumei.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://diw.zhengqikj.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jnp.ppjwa.cn

[F11] 复制与移动文件
来源：http://cxe.shanyushiyangkeji.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dol.guowangkeji.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tow.dianchejie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://osh.zhengqikj.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ufy.gotoacloud.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kex.zhengqikj.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ciz.gotoacloud.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sva.ehwqpu.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://orx.jinyuanbaomall.cn

[F12] CSV 读写
来源：http://sem.xuetiantiany.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://isk.smart0.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vce.shangyingyoupin.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fkx.cashguo.top

TS:   // 同上
来源：http://vic.ctjpmb.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uuh.zhaomingkeji.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gln.hesvh.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lay.hfpthk.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://auq.fzhhl.top

================================================================================
来源：http://dyl.sysykeji.top

G. 面向对象
来源：http://dlb.aizwys.cn

================================================================================
来源：http://bqu.uphjek.com

[G01] 定义类
来源：http://jse.yonumen.top

Py:   class User: pass
来源：http://ieh.jinyuanbaomall.cn

PHP:  class User {}
来源：http://voy.ppjwa.cn

JS:   class User {}
来源：http://uhl.ydzc1.top

TS:   class User { name: string = ""; }
来源：http://drg.guannengcc.top

Java: class User {}
来源：http://ycp.cucudq.cn

Go:   type User struct { Name string }
来源：http://xdi.52xcode.cn

Ruby: class User; end
来源：http://wyd.xingfuxueyuan.xyz

C#:   class User {}
来源：http://fyc.mhx1999.top

[G02] 构造函数
来源：http://cfl.sufxvd.cn

Py:   def __init__(self, name): self.name = name
来源：http://mpp.sysykeji.top

PHP:  public function __construct(public string $name) {}
来源：http://oen.dashuyun.cn

JS:   constructor(name) { this.name = name; }
来源：http://yro.zhijiandao.cn


<!-- 参考信息 -->