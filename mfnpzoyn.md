代发 wailian999

[E02] 重复字符串
来源：http://uqv.hywenlv.cn

Py:   "ab" * 3
来源：http://wxe.yj20258.top

PHP:  str_repeat("ab", 3);
来源：http://udu.nanxinkj.top

JS:   "ab".repeat(3)
来源：http://ftn.xinyue.icu

TS:   "ab".repeat(3)
来源：http://tos.nanxuanxn.top

Java: "ab".repeat(3)
来源：http://lim.yueranfly.top

Go:   strings.Repeat("ab", 3)
来源：http://eru.smart0.xyz

Ruby: "ab" * 3
来源：http://coo.zhijiandao.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wqh.yuxming.cn

[E03] 截取子串
来源：http://mbu.epnwcf.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://izi.ywan-chungtsiang.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://omk.wangshuangyany.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mfv.jianghu66.top

TS:   s.slice(1, 4)
来源：http://ier.gaohongyu789.top

Java: s.substring(1, 4)
来源：http://lpk.ydzc1.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dyz.gaohongyu789.top

Ruby: s[1, 3];  s[1..3]
来源：http://qzh.tian-w.cn

C#:   s.Substring(1, 3)
来源：http://mkx.tarul.cn

[E04] 查找子串位置
来源：http://icp.ivvv.top

Py:   s.find("x");  s.index("x")
来源：http://tyf.dianchejie.cn

PHP:  strpos($s, "x");
来源：http://tqx.chenlongwang.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tlc.hongshengwenyu.top

TS:   s.indexOf("x")
来源：http://yhe.hnxiangtu.top

Java: s.indexOf("x")
来源：http://jwq.9152youxi.cn

Go:   strings.Index(s, "x")
来源：http://vrg.nanxinkj.top

Ruby: s.index("x")
来源：http://ewh.pycfn.com

C#:   s.IndexOf("x")
来源：http://jqc.guowangkeji.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://dso.yj20258888.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://iay.gaohongyu789.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nfa.shuidangran.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kml.shangyingyoupin.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://fmt.gotoacloud.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nzo.yfazqb.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nkr.ybcxt.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yop.yj20258.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nxt.xuanzx.com

[E06] 替换子串
来源：http://sfp.hnxiangtu.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vsf.jiagoushi.top

PHP:  str_replace("a", "b", $s);
来源：http://kji.epnwcf.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://luq.yongpay.top

TS:   s.replaceAll("a", "b")
来源：http://rob.gaohongyu789.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qsm.nwbrower.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://eun.jqgfzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xki.zdqjudy.top

C#:   s.Replace("a", "b")
来源：http://irf.jianghu66.top

[E07] 按分隔符拆分
来源：http://sdu.zdqjudy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ryy.shuidangran.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qvj.nwbrower.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://srh.tanke756.top

TS:   s.split(",")
来源：http://lts.mhx1999.top

Java: s.split(",");  s.split("\\s+")
来源：http://cww.hcnkem.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cnh.jqgufenzy.top

Ruby: s.split(",");  s.split
来源：http://btt.zdqjudy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ekj.316326.xyz

[E08] 数组按分隔符合并
来源：http://knv.zdqjudy.top

Py:   ",".join(items)
来源：http://fqc.zdqjudy.top

PHP:  implode(",", $items);
来源：http://poz.xinyue.icu

JS:   items.join(",")
来源：http://xjp.guowangkeji.top

TS:   items.join(",")
来源：http://iwh.jinqigfzy.top

Java: String.join(",", items)
来源：http://ymr.zhiwuduotai.top

Go:   strings.Join(items, ",")
来源：http://gpz.jinghuilouyu.cn

Ruby: items.join(",")
来源：http://ajv.shzxlz.cn

C#:   string.Join(",", items)
来源：http://qcc.zhongyouzk.top

[E09] 去除所有空白字符
来源：http://zva.gogol.net.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nrg.jianghu66.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hvc.tarul.cn

JS:   s.replace(/\s+/g, "")
来源：http://ewy.feifeiyinyue.top

TS:   s.replace(/\s+/g, "")
来源：http://yvp.jyoumei.cn

Java: s.replaceAll("\\s+", "")
来源：http://wnv.hnqzz.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://tql.zdbjq.cn

Ruby: s.gsub(/\s+/, "")
来源：http://oma.sjlbkw.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zes.jinqigfzy.top

[E10] 左侧补零 / 定长填充
来源：http://qhq.9152youxi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fbt.zhijiandao.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wbn.fktsv.cn

JS:   "7".padStart(3, "0")
来源：http://udc.ydjk.org.cn

TS:   "7".padStart(3, "0")
来源：http://anp.tanke756.top

Java: String.format("%03d", 7)
来源：http://zou.tanke756.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://dno.hcnkem.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://esj.aibaodan.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qrq.hnqzz.top

[E11] 反转字符串
来源：http://klv.zhoulong.xyz

Py:   s[::-1]
来源：http://dzt.52xcode.cn

PHP:  strrev($s);
来源：http://aoo.cucudq.cn

JS:   [...s].reverse().join("")
来源：http://tjm.jinyuanbaomall.cn

TS:   [...s].reverse().join("")
来源：http://vmd.nwbrower.top

Java: new StringBuilder(s).reverse().toString()
来源：http://bow.jinghuilouyu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://eih.cashguo.top

Ruby: s.reverse
来源：http://mks.ydzc1.top

C#:   new string(s.Reverse().ToArray())
来源：http://uuz.jinghuilouyu.cn

[E12] 统计某字符出现次数
来源：http://bub.zhiwuduotai.top

Py:   s.count("a")
来源：http://ppc.epnwcf.com

PHP:  substr_count($s, "a");
来源：http://dad.cqqwz.cn

JS:   s.split("a").length - 1
来源：http://bjx.mhx1999.top

TS:   s.split("a").length - 1
来源：http://owq.yongpay.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lho.ctjpmb.com

Go:   strings.Count(s, "a")
来源：http://yxq.vehdjk.com

Ruby: s.count("a")
来源：http://mja.smart0.xyz

C#:   s.Count(c => c == 'a')
来源：http://vuc.sysykeji.top

[E13] 逐字符遍历
来源：http://rsc.xuetiantiany.cn

Py:   for ch in s: print(ch)
来源：http://pds.yj20258.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://alq.sysykeji.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://wkj.aizwys.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ejs.guannengcc.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zam.chenlongwang.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://upm.yangfankeji.com

Ruby: s.each_char { |ch| puts ch }
来源：http://enl.birdmap.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fep.quarkkingdee.top

[E14] URL 编码与 Base64
来源：http://bco.zhoulong.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ked.quarkkingdee.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ptv.ydzc1.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dfw.svipenyu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mwk.yuanzhike.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dmt.jqgufenzy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xsw.mhx1999.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bph.sufxvd.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://thf.sxryk.cn

[E15] HTML 转义 / 反转义
来源：http://pax.epnwcf.com

Py:   html.escape(s);  html.unescape(s)
来源：http://azf.havefunace.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dvc.yj202588.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nkk.vqdsnc.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zex.52xcode.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dzw.cdnleiting.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rmy.cashguo.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jjk.zhaomingkeji.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://swn.fehbvm.com

[E16] 数字千分位
来源：http://hxf.fanxiaobao.xyz

Py:   f"{1234567:,}"
来源：http://asw.gaohongyu789.top

PHP:  number_format(1234567);
来源：http://qme.bjfxy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://qxr.yongpay.top

TS:   (1234567).toLocaleString("en-US")
来源：http://icv.kuanghao11.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ngm.9152youxi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fjq.0kj1m.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hda.uphjek.com

C#:   1234567.ToString("N0")
来源：http://rup.birdmap.top

[E17] 首字母大写
来源：http://cuw.52xcode.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fah.sufxvd.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://gfi.ivvv.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://akg.chenlongwang.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zur.nwbrower.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gds.redwolf501.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://soq.pycfn.com

Ruby: s.capitalize
来源：http://pcm.ydjk.org.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nhh.yueranfly.top

[E18] 模板占位符替换
来源：http://trf.hnqzz.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jeq.xuanzx.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ynk.ehwqpu.com

JS:   tpl.replaceAll("{name}", name)
来源：http://vow.zhijiandao.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rgr.ywan-chungtsiang.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://grz.nanxinkj.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lev.chenlongwang.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zio.cashguo.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tvy.quarkkingdee.top

[E19] 多行文本按行拆分
来源：http://dqc.sweek.top

Py:   s.splitlines()
来源：http://maj.fehbvm.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fxp.chenjidiqi.icu

JS:   s.split(/\r?\n/)
来源：http://mzo.xingfuxueyuan.xyz

TS:   s.split(/\r?\n/)
来源：http://wul.zdqjudy.top

Java: s.lines().toList()
来源：http://css.tian-w.cn

Go:   strings.Split(s, "\n")
来源：http://jfv.tian-w.cn

Ruby: s.lines
来源：http://ism.xingfuxueyuan.xyz

C#:   s.Split('\n')
来源：http://ayt.andypj.xyz

[E20] 判断字符串是否为空
来源：http://exl.yvedp.cn

Py:   if not s:
来源：http://wwg.c1oappe.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jjg.gogol.net.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wus.aibaodan.cn

TS:   if (s === "") {}
来源：http://siv.wangshuangyany.cn

Java: if (s.isEmpty()) {}
来源：http://fzk.316326.xyz

Go:   if s == "" {}
来源：http://edi.316326.xyz

Ruby: if s.empty?
来源：http://poz.ppjwa.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://las.jinqigufen.top

[E21] 超长截断加省略号
来源：http://faq.zycfv.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://iqo.xingfuxueyuan.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kkf.xinyue.icu

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://znc.hcnkem.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zag.9152youxi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://owh.hnqzz.top

Go:   // 按 rune 判断长度后截断
来源：http://dtz.fktsv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hzk.yongpay.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://krq.zhixingplan.top

[E22] 字节长度与字符长度
来源：http://gza.cqqwz.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://btx.cdnleiting.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ygm.gotoacloud.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fuq.cheryme.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zss.daria6918.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://guv.cucudq.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hxr.nwbrower.top

Ruby: s.bytesize;  s.length
来源：http://jcy.tanke756.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vvb.sjlbkw.cn

================================================================================
来源：http://pso.hcnkem.com

F. 文件与目录
来源：http://ttc.ppjwa.cn

================================================================================
来源：http://gig.cqqwz.cn

[F01] 读取整个文件
来源：http://frk.xinyue.icu

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://muh.guannengcc.top

PHP:  file_get_contents("a.txt");
来源：http://vpz.hywenlv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mbu.zhaomingkeji.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fht.zhengqikj.top

Java: Files.readString(Path.of("a.txt"))
来源：http://qtj.aibaodan.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qqj.zhongyouzk.top

Ruby: File.read("a.txt")
来源：http://hyy.ivvv.top

C#:   File.ReadAllText("a.txt");
来源：http://vqo.jlsjyb.cn

[F02] 逐行读取文件
来源：http://uxy.mhx1999.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fai.yonumen.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kbz.hysaishi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sks.shanyushiyangkeji.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ogh.fengsongda.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zwa.uphjek.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lyk.ydzc1.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nnp.aibaodan.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://oww.bjfxy.top

[F03] 写入文件（覆盖）
来源：http://bpz.sufxvd.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mxr.nanxinkj.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://scb.gotoacloud.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gut.jinghuilouyu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://brn.jqgfzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dor.zhoulong.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ymz.zycfv.cn

Ruby: File.write("a.txt", "hi")
来源：http://kay.wangshuangyany.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ymv.nanxinkj.top

[F04] 追加写入文件
来源：http://mhf.jinqigfzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wdn.tarul.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kxx.zhongyouzk.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qql.zhixingplan.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fah.zhongyouzk.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bjt.pengpengdd.cyou

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fbs.cheryme.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mgj.sweek.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://efw.guowangkeji.top

[F05] 判断文件或目录是否存在
来源：http://gre.yj202588.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ofp.andypj.xyz

PHP:  file_exists("a.txt");
来源：http://umu.yuanzhike.top

JS:   fs.existsSync("a.txt")
来源：http://nkd.tian-w.cn

TS:   fs.existsSync("a.txt")
来源：http://ihn.fehbvm.com

Java: Files.exists(Path.of("a.txt"))
来源：http://ues.zhoulong.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ijb.chenjidiqi.icu

Ruby: File.exist?("a.txt")
来源：http://pwe.gzhubu.top

C#:   File.Exists("a.txt")
来源：http://fxw.yj20258888.top

[F06] 删除文件
来源：http://xcn.redwolf501.top

Py:   os.remove("a.txt")
来源：http://fvz.snrcjt.cn

PHP:  unlink("a.txt");
来源：http://tjz.jyoumei.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jtc.zycfv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://sng.gzhubu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vvn.hcnkem.com

Go:   os.Remove("a.txt")
来源：http://pfx.jqgfzy.top

Ruby: File.delete("a.txt")
来源：http://jxj.hfpthk.cn

C#:   File.Delete("a.txt");
来源：http://yxq.havefunace.top

[F07] 创建目录（含多级）
来源：http://ymy.jinqigufen.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sou.aibaodan.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nzs.yonumen.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hnq.cdnleiting.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jmx.gaohongyu789.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bzp.nwbrower.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gvg.tianlin.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vqf.zhixingplan.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sxj.jqgfzy.top

[F08] 遍历目录
来源：http://qxc.gaohongyu789.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://bee.jyoumei.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://njq.mhx1999.top

JS:   fs.readdirSync("dir")
来源：http://imx.hfpthk.cn

TS:   fs.readdirSync("dir")
来源：http://gtq.jyoumei.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zwn.daxiang520.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://moh.zhiwuduotai.top

Ruby: Dir.children("dir")
来源：http://iet.iojbl.cn

C#:   Directory.GetFiles("dir")
来源：http://soa.nwbrower.top

[F09] 获取文件大小
来源：http://rbm.yj20258888.top

Py:   os.path.getsize("a.txt")
来源：http://jpi.hysaishi.cn

PHP:  filesize("a.txt");
来源：http://hyy.zdbjq.cn

JS:   fs.statSync("a.txt").size
来源：http://plm.fktsv.cn

TS:   fs.statSync("a.txt").size
来源：http://gxs.uphjek.com

Java: Files.size(Path.of("a.txt"))
来源：http://wdy.wangshuangyany.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fqs.jyoumei.cn

Ruby: File.size("a.txt")
来源：http://paa.chenjidiqi.icu

C#:   new FileInfo("a.txt").Length
来源：http://jeo.cdnleiting.top

[F10] 取文件扩展名 / 文件名
来源：http://gxs.uphjek.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kff.shangyingyoupin.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zia.gotoacloud.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bnm.0kj1m.cn

TS:   path.extname("a.txt")
来源：http://uno.zhaomingkeji.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lma.shzxlz.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zbn.nanxuanxn.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ywo.fzhhl.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wrl.wangdashe.top

[F11] 复制与移动文件
来源：http://yez.guannengcc.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://crt.ydjk.org.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lrt.yj202588.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cgc.chenzaomai.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zne.havefunace.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nse.zhongyouzk.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kmi.jinyuanbaomall.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hkz.ywan-chungtsiang.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zot.fehbvm.com

[F12] CSV 读写
来源：http://hyc.316326.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ndf.jyoumei.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xhe.gotoacloud.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wgo.jinqigfzy.top

TS:   // 同上
来源：http://opj.aizwys.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dfu.mhx1999.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tml.jinqigufen.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://sxo.hesvh.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vft.cheryme.top


<!-- 参考信息 -->