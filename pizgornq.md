代发 wailian999

Go:   strings.Index(s, "x")
来源：http://zzz.ppjwa.cn

Ruby: s.index("x")
来源：http://jge.cheryme.top

C#:   s.IndexOf("x")
来源：http://roh.yongpay.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://xlb.sxryk.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://swt.ehwqpu.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://art.jyoumei.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xpo.yanxiufei.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ovc.zdbjq.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wop.yonumen.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ltj.zhixingplan.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://noc.aibaodan.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lwt.zdqjudy.top

[E06] 替换子串
来源：http://jgk.ybcxt.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yiu.wangdashe.top

PHP:  str_replace("a", "b", $s);
来源：http://fes.hesvh.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zri.jqgfzy.top

TS:   s.replaceAll("a", "b")
来源：http://kys.havefunace.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mmf.jqgfzy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://aiw.jinghuilouyu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hxe.yonumen.top

C#:   s.Replace("a", "b")
来源：http://tcm.dianchejie.cn

[E07] 按分隔符拆分
来源：http://qlr.ydjk.org.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pkn.nanxinkj.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ykl.jianghu66.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://tgb.shuidangran.top

TS:   s.split(",")
来源：http://yjk.316326.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://hiy.9152youxi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nnp.haohaochexian.top

Ruby: s.split(",");  s.split
来源：http://qka.hnqzz.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pnn.shzxlz.cn

[E08] 数组按分隔符合并
来源：http://qat.zhoulong.xyz

Py:   ",".join(items)
来源：http://hdm.hesvh.cn

PHP:  implode(",", $items);
来源：http://mfn.aizwys.cn

JS:   items.join(",")
来源：http://gnk.zdqjudy.top

TS:   items.join(",")
来源：http://tzu.fengsongda.top

Java: String.join(",", items)
来源：http://dqg.chenjidiqi.icu

Go:   strings.Join(items, ",")
来源：http://lkn.jqgfzy.top

Ruby: items.join(",")
来源：http://shg.nanxuanxn.top

C#:   string.Join(",", items)
来源：http://fsl.svipenyu.cn

[E09] 去除所有空白字符
来源：http://oid.hcnkem.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vgo.hywenlv.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yxo.cashguo.top

JS:   s.replace(/\s+/g, "")
来源：http://bws.dashuyun.cn

TS:   s.replace(/\s+/g, "")
来源：http://mot.jinyuanbaomall.cn

Java: s.replaceAll("\\s+", "")
来源：http://crx.cqqwz.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://iyz.xingfuxueyuan.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://boz.yfazqb.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xix.tarul.cn

[E10] 左侧补零 / 定长填充
来源：http://eyn.chenjidiqi.icu

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://awc.xylfe.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gig.ybcxt.top

JS:   "7".padStart(3, "0")
来源：http://skd.haohaochexian.top

TS:   "7".padStart(3, "0")
来源：http://aih.c1oappe.top

Java: String.format("%03d", 7)
来源：http://ykf.shanyushiyangkeji.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://cla.redwolf501.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://brj.tian-w.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ogx.hammf.cn

[E11] 反转字符串
来源：http://wbs.meibo888.top

Py:   s[::-1]
来源：http://ehb.hysaishi.cn

PHP:  strrev($s);
来源：http://iww.hywenlv.cn

JS:   [...s].reverse().join("")
来源：http://cvn.pycfn.com

TS:   [...s].reverse().join("")
来源：http://mid.shanyushiyangtech.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ioy.xingfuxueyuan.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://vle.xziqi.cn

Ruby: s.reverse
来源：http://uii.guannengcc.top

C#:   new string(s.Reverse().ToArray())
来源：http://xfj.zhongyouzk.top

[E12] 统计某字符出现次数
来源：http://ovz.jqgfzy.top

Py:   s.count("a")
来源：http://knb.yvedp.cn

PHP:  substr_count($s, "a");
来源：http://cjy.mhx1999.top

JS:   s.split("a").length - 1
来源：http://nzl.yfazqb.com

TS:   s.split("a").length - 1
来源：http://jhs.shuidangran.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://myo.sxryk.cn

Go:   strings.Count(s, "a")
来源：http://lvd.yangfankeji.com

Ruby: s.count("a")
来源：http://iym.pengpengdd.cyou

C#:   s.Count(c => c == 'a')
来源：http://quw.chenzaomai.com

[E13] 逐字符遍历
来源：http://gwn.yueranfly.top

Py:   for ch in s: print(ch)
来源：http://rhq.haohaochexian.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ege.jqgufenzy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://llv.zhoulong.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://ctu.nanxuanxn.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gjn.snrcjt.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://emo.jinyuanbaomall.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hbg.hongshengwenyu.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pcc.iojbl.cn

[E14] URL 编码与 Base64
来源：http://laq.hcnkem.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xuz.sufxvd.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jmn.hnxiangtu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pbc.haohaochexian.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://els.jinqigufen.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qxj.hywenlv.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://eje.yangfankeji.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ynr.hcnkem.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rtg.nanxuanxn.top

[E15] HTML 转义 / 反转义
来源：http://ixx.ydzc1.top

Py:   html.escape(s);  html.unescape(s)
来源：http://qoi.jiagoushi.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bbf.iojbl.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zgt.gotoacloud.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ajs.gzhubu.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://djq.yj20258888.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wbj.zycfv.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cqc.yangfankeji.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://aax.xingfuxueyuan.xyz

[E16] 数字千分位
来源：http://hen.feifeiyinyue.top

Py:   f"{1234567:,}"
来源：http://dhf.fanxiaobao.xyz

PHP:  number_format(1234567);
来源：http://iib.tian-w.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ine.sysykeji.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ovc.shuidangran.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ooh.bbcook.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zen.zhaomingkeji.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qul.316326.xyz

C#:   1234567.ToString("N0")
来源：http://wca.nanxuanxn.top

[E17] 首字母大写
来源：http://ixs.ywan-chungtsiang.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nxo.chenjidiqi.icu

PHP:  ucfirst($s);  ucwords($s);
来源：http://cbk.gaohongyu789.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://naw.sufxvd.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mtj.hysaishi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wrl.yanxiufei.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bji.smart0.xyz

Ruby: s.capitalize
来源：http://rnv.zhixingplan.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nae.yj202588.top

[E18] 模板占位符替换
来源：http://sdu.uphjek.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fxx.dianchejie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ceq.jqgufenzy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://iit.nanxuanxn.top

TS:   tpl.replaceAll("{name}", name)
来源：http://pdb.guannengcc.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://iyg.hywenlv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ugi.iojbl.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nes.yanxiufei.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qbn.jinghuilouyu.cn

[E19] 多行文本按行拆分
来源：http://njy.yuxming.cn

Py:   s.splitlines()
来源：http://wfy.nanxinkj.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hed.kuanghao11.cn

JS:   s.split(/\r?\n/)
来源：http://zkc.jqgufenzy.top

TS:   s.split(/\r?\n/)
来源：http://nng.cashguo.top

Java: s.lines().toList()
来源：http://avl.hesvh.cn

Go:   strings.Split(s, "\n")
来源：http://kfa.gzhubu.top

Ruby: s.lines
来源：http://ifi.9152youxi.cn

C#:   s.Split('\n')
来源：http://mwx.ctjpmb.com

[E20] 判断字符串是否为空
来源：http://zmd.zhaomingkeji.xyz

Py:   if not s:
来源：http://zpj.yfazqb.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qnz.0kj1m.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://iyk.yonumen.top

TS:   if (s === "") {}
来源：http://kys.hysaishi.cn

Java: if (s.isEmpty()) {}
来源：http://ngm.feifeiyinyue.top

Go:   if s == "" {}
来源：http://pot.guannengcc.top

Ruby: if s.empty?
来源：http://shw.dianchejie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://krl.gaohongyu789.top

[E21] 超长截断加省略号
来源：http://agl.tarul.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jbh.hnqzz.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ons.jinyuanbaomall.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fik.guowangkeji.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wte.pycfn.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://spo.fehbvm.com

Go:   // 按 rune 判断长度后截断
来源：http://czf.shangyingyoupin.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pic.yuxming.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fba.zhoulong.xyz

[E22] 字节长度与字符长度
来源：http://ubs.yj20258888.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bvx.bjfxy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uqe.fktsv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xtu.yueranfly.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zjn.fengsongda.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hfd.hammf.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sax.sjlbkw.cn

Ruby: s.bytesize;  s.length
来源：http://wzc.yuxming.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ujx.mhx1999.top

================================================================================
来源：http://eiz.ydzc1.top

F. 文件与目录
来源：http://pxd.iojbl.cn

================================================================================
来源：http://nim.smart0.xyz

[F01] 读取整个文件
来源：http://fcw.gaohongyu789.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lhp.yongpay.top

PHP:  file_get_contents("a.txt");
来源：http://lhs.jyoumei.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lkt.epnwcf.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ovo.xuetiantiany.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://trx.jyoumei.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jhq.guowangkeji.top

Ruby: File.read("a.txt")
来源：http://kxg.yj202588.top

C#:   File.ReadAllText("a.txt");
来源：http://tfy.52xcode.cn

[F02] 逐行读取文件
来源：http://wqj.tian-w.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xmw.kuanghao11.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fbk.zhongyouzk.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://szs.havefunace.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bff.redwolf501.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ldk.yj20258.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dpb.xylfe.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xuv.yfazqb.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tyw.pycfn.com

[F03] 写入文件（覆盖）
来源：http://phx.xuetiantiany.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lbd.vqdsnc.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ckf.jqgfzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tvf.vqdsnc.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yhy.aibaodan.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cbq.fzhhl.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gnh.fzhhl.top

Ruby: File.write("a.txt", "hi")
来源：http://cfd.dashuyun.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cyx.cdnleiting.top

[F04] 追加写入文件
来源：http://xio.iojbl.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wfe.shangyingyoupin.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vuf.vehdjk.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xwu.zhaomingkeji.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qqw.zhixingplan.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wul.yuxming.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gtp.bbcook.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://owf.shuidangran.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kgj.zdqjudy.top

[F05] 判断文件或目录是否存在
来源：http://jpi.shanyushiyangkeji.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://udu.ivvv.top

PHP:  file_exists("a.txt");
来源：http://mrg.hongshengwenyu.top

JS:   fs.existsSync("a.txt")
来源：http://lik.bjfxy.top

TS:   fs.existsSync("a.txt")
来源：http://zvb.daria6918.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gnr.redwolf501.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://iab.jqgfzy.top

Ruby: File.exist?("a.txt")
来源：http://vkm.xingfuxueyuan.xyz

C#:   File.Exists("a.txt")
来源：http://vth.feifeiyinyue.top

[F06] 删除文件
来源：http://jzv.shanyushiyangkeji.top

Py:   os.remove("a.txt")
来源：http://sfm.zhengqikj.top

PHP:  unlink("a.txt");
来源：http://jgc.yueranfly.top

JS:   fs.unlinkSync("a.txt")
来源：http://pdf.shangyingyoupin.top

TS:   fs.unlinkSync("a.txt")
来源：http://civ.bbcook.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xvx.ivvv.top

Go:   os.Remove("a.txt")
来源：http://oxu.mhx1999.top

Ruby: File.delete("a.txt")
来源：http://xhm.ivvv.top

C#:   File.Delete("a.txt");
来源：http://lpe.hnxiangtu.top

[F07] 创建目录（含多级）
来源：http://ebc.uphjek.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zgu.zdbjq.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ukz.zycfv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://myt.zhoulong.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wnh.yangfankeji.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://psa.guannengcc.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://msk.cashguo.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gei.pengpengdd.cyou

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kdt.daria6918.cn

[F08] 遍历目录
来源：http://vul.zhengqikj.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://pul.cqqwz.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wqg.yj20258.top

JS:   fs.readdirSync("dir")
来源：http://ahf.sweek.top

TS:   fs.readdirSync("dir")
来源：http://lqp.jiagoushi.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ayw.jianghu66.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://lue.cheryme.top

Ruby: Dir.children("dir")
来源：http://wor.fktsv.cn

C#:   Directory.GetFiles("dir")
来源：http://ibi.52xcode.cn

[F09] 获取文件大小
来源：http://cwu.jinqigfzy.top

Py:   os.path.getsize("a.txt")
来源：http://ycj.ivvv.top

PHP:  filesize("a.txt");
来源：http://csv.jianghu66.top

JS:   fs.statSync("a.txt").size
来源：http://rix.yfazqb.com

TS:   fs.statSync("a.txt").size
来源：http://pnq.snrcjt.cn

Java: Files.size(Path.of("a.txt"))
来源：http://toa.jqgfzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yip.yuanzhike.top

Ruby: File.size("a.txt")
来源：http://pyd.tarul.cn

C#:   new FileInfo("a.txt").Length
来源：http://dxc.chenlongwang.top

[F10] 取文件扩展名 / 文件名
来源：http://fcs.nwbrower.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rej.c1oappe.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://oko.jlsjyb.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vgx.quarkkingdee.top

TS:   path.extname("a.txt")
来源：http://nqb.aizwys.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://crr.0kj1m.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://whk.pycfn.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zwy.yanxiufei.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://llv.cdnleiting.top

[F11] 复制与移动文件
来源：http://jol.tianlin.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jhw.havefunace.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jrm.shuidangran.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://whs.shanyushiyangtech.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rfp.uphjek.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qjv.jianghu66.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kwk.yfazqb.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pau.quarkkingdee.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://you.wangdashe.top

[F12] CSV 读写
来源：http://fnj.hysaishi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jas.cucudq.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ggy.pengpengdd.cyou

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qoz.hywenlv.cn

TS:   // 同上
来源：http://mes.sysykeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wly.shuidangran.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://eva.birdmap.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ete.redwolf501.top

C#:   // 无内置：用 CsvHelper 库
来源：http://olg.chenjidiqi.icu

================================================================================
来源：http://cfp.guannengcc.top

G. 面向对象
来源：http://bgf.snrcjt.cn

================================================================================
来源：http://jxf.yonumen.top

[G01] 定义类
来源：http://fxb.hysaishi.cn

Py:   class User: pass
来源：http://ldx.sysykeji.top

PHP:  class User {}
来源：http://pau.316326.xyz

JS:   class User {}
来源：http://rwz.kuanghao11.cn

TS:   class User { name: string = ""; }
来源：http://eef.dashuyun.cn

Java: class User {}
来源：http://tac.ybcxt.top

Go:   type User struct { Name string }
来源：http://kmt.mhx1999.top

Ruby: class User; end
来源：http://zkg.fengsongda.top

C#:   class User {}
来源：http://kdn.fktsv.cn

[G02] 构造函数
来源：http://jma.zhengqikj.top

Py:   def __init__(self, name): self.name = name
来源：http://dqf.hysaishi.cn

PHP:  public function __construct(public string $name) {}
来源：http://quw.hfpthk.cn

JS:   constructor(name) { this.name = name; }
来源：http://zbu.pycfn.com

TS:   constructor(public name: string) {}
来源：http://wbw.aizwys.cn

Java: User(String name) { this.name = name; }
来源：http://whh.chenjidiqi.icu

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://iya.xuetiantiany.cn

Ruby: def initialize(name); @name = name; end
来源：http://ywz.zhijiandao.cn

C#:   public User(string name) { Name = name; }
来源：http://rsu.52xcode.cn

[G03] 实例属性
来源：http://caj.shanyushiyangkeji.top

Py:   self.name = "x"
来源：http://hdh.shanyushiyangkeji.top

PHP:  public string $name = "x";
来源：http://prd.bjfxy.top


<!-- 参考信息 -->