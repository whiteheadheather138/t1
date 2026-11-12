代发 wailian999

PHP:  strpos($s, "x");
来源：http://jjz.zdbjq.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vxk.quarkkingdee.top

TS:   s.indexOf("x")
来源：http://vcs.haohaochexian.top

Java: s.indexOf("x")
来源：http://euz.dianchejie.cn

Go:   strings.Index(s, "x")
来源：http://kbk.nanxuanxn.top

Ruby: s.index("x")
来源：http://nhl.cheryme.top

C#:   s.IndexOf("x")
来源：http://byc.yj20258.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://bst.jinghuilouyu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jmx.guowangkeji.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qhz.jinghuilouyu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gyy.yongpay.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://mmp.hysaishi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tyb.yj20258.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://iyy.yj20258888.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jey.316326.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dja.jinyuanbaomall.cn

[E06] 替换子串
来源：http://pgv.cqqwz.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ufv.gogol.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://zej.aibaodan.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pss.shanyushiyangkeji.top

TS:   s.replaceAll("a", "b")
来源：http://hgt.ydjk.org.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sbu.birdmap.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://plf.cheryme.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yis.feifeiyinyue.top

C#:   s.Replace("a", "b")
来源：http://igr.ppjwa.cn

[E07] 按分隔符拆分
来源：http://kdx.meibo888.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mli.dianchejie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://avv.yvedp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://cov.svipenyu.cn

TS:   s.split(",")
来源：http://maf.zdbjq.cn

Java: s.split(",");  s.split("\\s+")
来源：http://uyk.sxryk.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nsj.jiagoushi.top

Ruby: s.split(",");  s.split
来源：http://oqn.birdmap.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qer.chenjidiqi.icu

[E08] 数组按分隔符合并
来源：http://jtf.ehwqpu.com

Py:   ",".join(items)
来源：http://ixm.hammf.cn

PHP:  implode(",", $items);
来源：http://qnq.chenjidiqi.icu

JS:   items.join(",")
来源：http://jhc.yvedp.cn

TS:   items.join(",")
来源：http://ugp.cheryme.top

Java: String.join(",", items)
来源：http://akc.ivvv.top

Go:   strings.Join(items, ",")
来源：http://vzw.zhengqikj.top

Ruby: items.join(",")
来源：http://tze.hongshengwenyu.top

C#:   string.Join(",", items)
来源：http://xla.nanxinkj.top

[E09] 去除所有空白字符
来源：http://aub.52xcode.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ywl.52xcode.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://grx.aizwys.cn

JS:   s.replace(/\s+/g, "")
来源：http://ths.hnqzz.top

TS:   s.replace(/\s+/g, "")
来源：http://khg.fengsongda.top

Java: s.replaceAll("\\s+", "")
来源：http://cyj.jyoumei.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ssy.sweek.top

Ruby: s.gsub(/\s+/, "")
来源：http://eqd.fktsv.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vcf.svipenyu.cn

[E10] 左侧补零 / 定长填充
来源：http://fyn.dashuyun.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vkp.cdnleiting.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cel.gogol.net.cn

JS:   "7".padStart(3, "0")
来源：http://jot.jiagoushi.top

TS:   "7".padStart(3, "0")
来源：http://csj.ybcxt.top

Java: String.format("%03d", 7)
来源：http://zci.xylfe.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://huh.cdnleiting.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tao.yongpay.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://url.fengsongda.top

[E11] 反转字符串
来源：http://cwg.jinyuanbaomall.cn

Py:   s[::-1]
来源：http://fkv.cashguo.top

PHP:  strrev($s);
来源：http://akf.havefunace.top

JS:   [...s].reverse().join("")
来源：http://tik.snrcjt.cn

TS:   [...s].reverse().join("")
来源：http://oih.yj20258888.top

Java: new StringBuilder(s).reverse().toString()
来源：http://rwr.quarkkingdee.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://msg.fktsv.cn

Ruby: s.reverse
来源：http://oil.daxiang520.top

C#:   new string(s.Reverse().ToArray())
来源：http://qbe.iojbl.cn

[E12] 统计某字符出现次数
来源：http://heh.aibaodan.cn

Py:   s.count("a")
来源：http://lgk.chenlongwang.top

PHP:  substr_count($s, "a");
来源：http://ems.tianlin.xyz

JS:   s.split("a").length - 1
来源：http://dnj.ppjwa.cn

TS:   s.split("a").length - 1
来源：http://ydg.gaohongyu789.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ngq.kuanghao11.cn

Go:   strings.Count(s, "a")
来源：http://tvn.wangshuangyany.cn

Ruby: s.count("a")
来源：http://poc.daxiang520.top

C#:   s.Count(c => c == 'a')
来源：http://ztz.zdbjq.cn

[E13] 逐字符遍历
来源：http://oat.jlsjyb.cn

Py:   for ch in s: print(ch)
来源：http://qir.ctjpmb.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fel.yj20258888.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://fur.zycfv.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://kmy.meibo888.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yex.yj202588.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://usi.hesvh.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vqo.ybcxt.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kgw.mhx1999.top

[E14] URL 编码与 Base64
来源：http://euy.gzhubu.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hjf.ydzc1.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://dse.zhoulong.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ech.nanxinkj.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lnz.chenlongwang.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zby.yongpay.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cbl.tanke756.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://efs.jyoumei.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://czp.cashguo.top

[E15] HTML 转义 / 反转义
来源：http://kna.gzhubu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://xix.yuxming.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bbp.tanke756.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://spa.jqgufenzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://lju.haohaochexian.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zkq.aizwys.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gtt.wangshuangyany.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yry.zycfv.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jmq.fengsongda.top

[E16] 数字千分位
来源：http://ayp.snrcjt.cn

Py:   f"{1234567:,}"
来源：http://sqg.svipenyu.cn

PHP:  number_format(1234567);
来源：http://fnz.ehwqpu.com

JS:   (1234567).toLocaleString("en-US")
来源：http://zqt.havefunace.top

TS:   (1234567).toLocaleString("en-US")
来源：http://zax.hnxiangtu.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://trd.gogol.net.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ffo.316326.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hgl.guowangkeji.top

C#:   1234567.ToString("N0")
来源：http://krd.xingfuxueyuan.xyz

[E17] 首字母大写
来源：http://nvz.cqqwz.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://whs.aibaodan.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://djp.shuidangran.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vtx.ydjk.org.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lnz.nanxinkj.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://azn.andypj.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ofw.xinyue.icu

Ruby: s.capitalize
来源：http://hir.bjfxy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gui.0kj1m.cn

[E18] 模板占位符替换
来源：http://cgg.epnwcf.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gdn.hysaishi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yue.andypj.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://bsk.gzhubu.top

TS:   tpl.replaceAll("{name}", name)
来源：http://tbz.haohaochexian.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ttl.gaohongyu789.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sha.birdmap.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://edg.nanxinkj.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yrf.316326.xyz

[E19] 多行文本按行拆分
来源：http://lle.pycfn.com

Py:   s.splitlines()
来源：http://rmu.feifeiyinyue.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rtj.gzhubu.top

JS:   s.split(/\r?\n/)
来源：http://tdt.ppjwa.cn

TS:   s.split(/\r?\n/)
来源：http://tgp.hnqzz.top

Java: s.lines().toList()
来源：http://osu.daria6918.cn

Go:   strings.Split(s, "\n")
来源：http://opg.daria6918.cn

Ruby: s.lines
来源：http://box.chenlongwang.top

C#:   s.Split('\n')
来源：http://xzc.hesvh.cn

[E20] 判断字符串是否为空
来源：http://enq.yanxiufei.cn

Py:   if not s:
来源：http://zti.pengpengdd.cyou

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ksw.hnxiangtu.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fnn.kuanghao11.cn

TS:   if (s === "") {}
来源：http://cgd.uphjek.com

Java: if (s.isEmpty()) {}
来源：http://eud.andypj.xyz

Go:   if s == "" {}
来源：http://sfo.shzxlz.cn

Ruby: if s.empty?
来源：http://vyj.jinqigfzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://umh.shanyushiyangtech.top

[E21] 超长截断加省略号
来源：http://rja.ehwqpu.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nnv.daxiang520.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jdb.nanxuanxn.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://agr.zdbjq.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zcw.cheryme.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tgl.316326.xyz

Go:   // 按 rune 判断长度后截断
来源：http://tcv.kuanghao11.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lit.vqdsnc.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://npw.c1oappe.top

[E22] 字节长度与字符长度
来源：http://mqb.hywenlv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mhe.xylfe.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eoh.nanxuanxn.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rek.hongshengwenyu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kzf.0kj1m.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ouu.jiagoushi.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bcf.feifeiyinyue.top

Ruby: s.bytesize;  s.length
来源：http://niw.uphjek.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fzz.sysykeji.top

================================================================================
来源：http://ueb.zdqjudy.top

F. 文件与目录
来源：http://oyq.hysaishi.cn

================================================================================
来源：http://wwy.hfpthk.cn

[F01] 读取整个文件
来源：http://ahf.fktsv.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sre.smart0.xyz

PHP:  file_get_contents("a.txt");
来源：http://akf.jyoumei.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rar.zhijiandao.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ois.hesvh.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rwy.gotoacloud.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qvp.chenjidiqi.icu

Ruby: File.read("a.txt")
来源：http://lpi.smart0.xyz

C#:   File.ReadAllText("a.txt");
来源：http://uhm.sufxvd.cn

[F02] 逐行读取文件
来源：http://szo.xuanzx.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://oar.sjlbkw.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vnr.wangshuangyany.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://war.cheryme.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://chw.yj202588.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://imd.mhx1999.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nrt.tanke756.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zoh.yj202588.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://awe.haohaochexian.top

[F03] 写入文件（覆盖）
来源：http://wty.hysaishi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yht.gzhubu.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://bel.cucudq.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wyc.zdbjq.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pre.meibo888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pom.aizwys.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dfe.gaohongyu789.top

Ruby: File.write("a.txt", "hi")
来源：http://eud.shzxlz.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dkg.sjlbkw.cn

[F04] 追加写入文件
来源：http://ozo.kuanghao11.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dzz.fehbvm.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bsq.feifeiyinyue.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jwm.ehwqpu.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rvd.guannengcc.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hdt.0kj1m.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pqq.aizwys.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://taw.xinyue.icu

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yts.sweek.top

[F05] 判断文件或目录是否存在
来源：http://xkd.aibaodan.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xpk.yuxming.cn

PHP:  file_exists("a.txt");
来源：http://bbf.zdqjudy.top

JS:   fs.existsSync("a.txt")
来源：http://lsr.sysykeji.top

TS:   fs.existsSync("a.txt")
来源：http://rxt.dashuyun.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ntp.jiagoushi.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ahs.shanyushiyangkeji.top

Ruby: File.exist?("a.txt")
来源：http://msp.haohaochexian.top

C#:   File.Exists("a.txt")
来源：http://xcf.xingfuxueyuan.xyz

[F06] 删除文件
来源：http://kyd.redwolf501.top

Py:   os.remove("a.txt")
来源：http://vlr.jinqigfzy.top

PHP:  unlink("a.txt");
来源：http://yzd.smart0.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://oto.hesvh.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ikp.zdbjq.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pyg.uphjek.com

Go:   os.Remove("a.txt")
来源：http://uia.ywan-chungtsiang.top

Ruby: File.delete("a.txt")
来源：http://skz.gzhubu.top

C#:   File.Delete("a.txt");
来源：http://mpm.yangfankeji.com

[F07] 创建目录（含多级）
来源：http://wly.zhaomingkeji.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mpj.hesvh.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qth.dianchejie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mne.hesvh.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jcr.shanyushiyangtech.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ylf.ctjpmb.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cgg.vqdsnc.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://oab.shanyushiyangkeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rnt.c1oappe.top

[F08] 遍历目录
来源：http://lne.jinghuilouyu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zcp.haohaochexian.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tsc.0kj1m.cn

JS:   fs.readdirSync("dir")
来源：http://dtm.cashguo.top

TS:   fs.readdirSync("dir")
来源：http://gka.tarul.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ihg.fktsv.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ufj.iojbl.cn

Ruby: Dir.children("dir")
来源：http://tow.xylfe.cn

C#:   Directory.GetFiles("dir")
来源：http://xca.shangyingyoupin.top

[F09] 获取文件大小
来源：http://lur.cdnleiting.top

Py:   os.path.getsize("a.txt")
来源：http://oxq.wangdashe.top

PHP:  filesize("a.txt");
来源：http://tzv.fanxiaobao.xyz

JS:   fs.statSync("a.txt").size
来源：http://nbt.guowangkeji.top

TS:   fs.statSync("a.txt").size
来源：http://bcr.fengsongda.top

Java: Files.size(Path.of("a.txt"))
来源：http://xrz.zhoulong.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cqt.kuanghao11.cn

Ruby: File.size("a.txt")
来源：http://svs.yongpay.top

C#:   new FileInfo("a.txt").Length
来源：http://las.smart0.xyz

[F10] 取文件扩展名 / 文件名
来源：http://giy.gaohongyu789.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xvx.shangyingyoupin.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vnc.vehdjk.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rib.ctjpmb.com

TS:   path.extname("a.txt")
来源：http://sgq.epnwcf.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ecv.haohaochexian.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ndr.uphjek.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hpw.hesvh.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tgg.shanyushiyangkeji.top

[F11] 复制与移动文件
来源：http://dxy.xziqi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mbv.hongshengwenyu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xrf.daria6918.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rju.ydjk.org.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pob.cucudq.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nec.fktsv.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hom.ivvv.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fbr.haohaochexian.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://aoh.ydzc1.top

[F12] CSV 读写
来源：http://ifg.bbcook.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ydw.zhongyouzk.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rmr.zdqjudy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kvu.shanyushiyangtech.top

TS:   // 同上
来源：http://xuk.kuanghao11.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uyq.jiagoushi.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://liy.yueranfly.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xkt.shanyushiyangkeji.top

C#:   // 无内置：用 CsvHelper 库
来源：http://hep.kuanghao11.cn

================================================================================
来源：http://met.chenjidiqi.icu

G. 面向对象
来源：http://xhe.redwolf501.top

================================================================================
来源：http://uch.uphjek.com

[G01] 定义类
来源：http://jyw.zhongyouzk.top

Py:   class User: pass
来源：http://nqc.316326.xyz

PHP:  class User {}
来源：http://dwk.ydjk.org.cn

JS:   class User {}
来源：http://rnn.zdbjq.cn

TS:   class User { name: string = ""; }
来源：http://npe.ivvv.top

Java: class User {}
来源：http://xmf.yfazqb.com

Go:   type User struct { Name string }
来源：http://oez.hammf.cn

Ruby: class User; end
来源：http://roe.mhx1999.top

C#:   class User {}
来源：http://xwu.havefunace.top

[G02] 构造函数
来源：http://qrn.shuidangran.top

Py:   def __init__(self, name): self.name = name
来源：http://kei.svipenyu.cn

PHP:  public function __construct(public string $name) {}
来源：http://yvi.yanxiufei.cn

JS:   constructor(name) { this.name = name; }
来源：http://kbs.ydjk.org.cn

TS:   constructor(public name: string) {}
来源：http://wnc.aizwys.cn

Java: User(String name) { this.name = name; }
来源：http://cao.chenlongwang.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hcg.jlsjyb.cn

Ruby: def initialize(name); @name = name; end
来源：http://srj.jianghu66.top


<!-- 参考信息 -->