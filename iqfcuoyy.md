代发 wailian999

Go:   strings.Index(s, "x")
来源：http://yql.c1oappe.top

Ruby: s.index("x")
来源：http://hxb.zhoulong.xyz

C#:   s.IndexOf("x")
来源：http://adg.feifeiyinyue.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ttr.ppjwa.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ove.jlsjyb.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://evs.gaohongyu789.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gzf.vqdsnc.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://nic.sxryk.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uuz.dashuyun.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://edc.dashuyun.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lyz.cucudq.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cid.gzhubu.top

[E06] 替换子串
来源：http://wud.guowangkeji.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wnb.shangyingyoupin.top

PHP:  str_replace("a", "b", $s);
来源：http://vvm.yfazqb.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://had.wangdashe.top

TS:   s.replaceAll("a", "b")
来源：http://fiu.pycfn.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://btz.zhiwuduotai.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wtm.yueranfly.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zmr.hnqzz.top

C#:   s.Replace("a", "b")
来源：http://cnn.bbcook.cn

[E07] 按分隔符拆分
来源：http://bvf.zycfv.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xya.pengpengdd.cyou

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://sqa.dianchejie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://sxj.zhixingplan.top

TS:   s.split(",")
来源：http://yzz.9152youxi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://crn.hywenlv.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xhq.cashguo.top

Ruby: s.split(",");  s.split
来源：http://puv.c1oappe.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yrl.hnqzz.top

[E08] 数组按分隔符合并
来源：http://gvv.sjlbkw.cn

Py:   ",".join(items)
来源：http://fcx.yj202588.top

PHP:  implode(",", $items);
来源：http://bsd.xuanzx.com

JS:   items.join(",")
来源：http://zuj.jlsjyb.cn

TS:   items.join(",")
来源：http://cov.vehdjk.com

Java: String.join(",", items)
来源：http://svo.wangdashe.top

Go:   strings.Join(items, ",")
来源：http://xvg.gotoacloud.top

Ruby: items.join(",")
来源：http://avt.wangshuangyany.cn

C#:   string.Join(",", items)
来源：http://fxa.yueranfly.top

[E09] 去除所有空白字符
来源：http://syn.havefunace.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://uxh.haohaochexian.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://osx.daxiang520.top

JS:   s.replace(/\s+/g, "")
来源：http://lfm.smart0.xyz

TS:   s.replace(/\s+/g, "")
来源：http://vqr.svipenyu.cn

Java: s.replaceAll("\\s+", "")
来源：http://arv.jinghuilouyu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qja.xuanzx.com

Ruby: s.gsub(/\s+/, "")
来源：http://tsk.havefunace.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://arn.hywenlv.cn

[E10] 左侧补零 / 定长填充
来源：http://log.ydjk.org.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qml.wangshuangyany.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cnp.mhx1999.top

JS:   "7".padStart(3, "0")
来源：http://pln.haohaochexian.top

TS:   "7".padStart(3, "0")
来源：http://ptu.yfazqb.com

Java: String.format("%03d", 7)
来源：http://blp.vehdjk.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://rap.ydzc1.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fpr.nwbrower.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wfa.wangshuangyany.cn

[E11] 反转字符串
来源：http://mpk.iojbl.cn

Py:   s[::-1]
来源：http://dzu.nwbrower.top

PHP:  strrev($s);
来源：http://mpe.kuanghao11.cn

JS:   [...s].reverse().join("")
来源：http://iya.xinyue.icu

TS:   [...s].reverse().join("")
来源：http://kvy.meibo888.top

Java: new StringBuilder(s).reverse().toString()
来源：http://jih.shangyingyoupin.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://oji.tianlin.xyz

Ruby: s.reverse
来源：http://qnf.zhaomingkeji.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://bvl.c1oappe.top

[E12] 统计某字符出现次数
来源：http://win.sysykeji.top

Py:   s.count("a")
来源：http://wgx.gotoacloud.top

PHP:  substr_count($s, "a");
来源：http://bbe.havefunace.top

JS:   s.split("a").length - 1
来源：http://pcq.hongshengwenyu.top

TS:   s.split("a").length - 1
来源：http://nmp.dianchejie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fen.guannengcc.top

Go:   strings.Count(s, "a")
来源：http://ouf.daxiang520.top

Ruby: s.count("a")
来源：http://kse.snrcjt.cn

C#:   s.Count(c => c == 'a')
来源：http://wof.mhx1999.top

[E13] 逐字符遍历
来源：http://wrr.chenlongwang.top

Py:   for ch in s: print(ch)
来源：http://wsu.zhongyouzk.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bzo.9152youxi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tbq.daxiang520.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://yln.hcnkem.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jxs.birdmap.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jnw.fanxiaobao.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://gqb.tanke756.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mgd.yvedp.cn

[E14] URL 编码与 Base64
来源：http://hkl.uphjek.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ene.yueranfly.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://emw.ydzc1.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hfs.quarkkingdee.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ixi.yj20258.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://apn.zdbjq.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://igi.jqgufenzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://aun.xuetiantiany.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cnx.hongshengwenyu.top

[E15] HTML 转义 / 反转义
来源：http://kkw.jyoumei.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://itm.zhongyouzk.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://afl.tarul.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wyt.zhongyouzk.top

TS:   // 同上，务必做 XSS 过滤
来源：http://kgh.yonumen.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rva.shzxlz.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wes.guowangkeji.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rrl.bbcook.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fnb.ydzc1.top

[E16] 数字千分位
来源：http://ckk.epnwcf.com

Py:   f"{1234567:,}"
来源：http://tiu.nanxinkj.top

PHP:  number_format(1234567);
来源：http://wly.chenlongwang.top

JS:   (1234567).toLocaleString("en-US")
来源：http://svd.sjlbkw.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://inj.yuxming.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ojc.quarkkingdee.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yvz.9152youxi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dya.haohaochexian.top

C#:   1234567.ToString("N0")
来源：http://hfe.cqqwz.cn

[E17] 首字母大写
来源：http://dsq.jinyuanbaomall.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tju.zhaomingkeji.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://ylx.chenjidiqi.icu

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dun.gotoacloud.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rfq.guowangkeji.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jxv.fzhhl.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lsq.jinyuanbaomall.cn

Ruby: s.capitalize
来源：http://dya.dianchejie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://akp.shanyushiyangkeji.top

[E18] 模板占位符替换
来源：http://zyn.dianchejie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jtv.zdqjudy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://esr.cqqwz.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://csv.9152youxi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://dhp.jlsjyb.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xxe.shangyingyoupin.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qil.zhongyouzk.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ofu.xuetiantiany.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lij.shzxlz.cn

[E19] 多行文本按行拆分
来源：http://gdf.jinqigufen.top

Py:   s.splitlines()
来源：http://qpj.xingfuxueyuan.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xzo.yonumen.top

JS:   s.split(/\r?\n/)
来源：http://byx.ehwqpu.com

TS:   s.split(/\r?\n/)
来源：http://zrf.haohaochexian.top

Java: s.lines().toList()
来源：http://rbk.aizwys.cn

Go:   strings.Split(s, "\n")
来源：http://udy.sysykeji.top

Ruby: s.lines
来源：http://gxj.wangdashe.top

C#:   s.Split('\n')
来源：http://dhy.dashuyun.cn

[E20] 判断字符串是否为空
来源：http://icu.bjfxy.top

Py:   if not s:
来源：http://bud.cashguo.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://swj.yueranfly.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://idz.aibaodan.cn

TS:   if (s === "") {}
来源：http://xem.c1oappe.top

Java: if (s.isEmpty()) {}
来源：http://ray.zhiwuduotai.top

Go:   if s == "" {}
来源：http://tio.zhongyouzk.top

Ruby: if s.empty?
来源：http://ikl.yuxming.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://eep.0kj1m.cn

[E21] 超长截断加省略号
来源：http://pkq.zhoulong.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ybp.shanyushiyangkeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://riz.cucudq.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wat.xziqi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jyd.guowangkeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jsr.chenlongwang.top

Go:   // 按 rune 判断长度后截断
来源：http://gzo.yanxiufei.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://oix.aibaodan.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ggx.chenlongwang.top

[E22] 字节长度与字符长度
来源：http://tlr.zhoulong.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://puy.havefunace.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://deh.zhaomingkeji.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dep.zhiwuduotai.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cgq.ctjpmb.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://odz.daria6918.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://eoy.chenzaomai.com

Ruby: s.bytesize;  s.length
来源：http://dkp.jinqigufen.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mzp.fzhhl.top

================================================================================
来源：http://rkf.daria6918.cn

F. 文件与目录
来源：http://sod.hcnkem.com

================================================================================
来源：http://tmm.haohaochexian.top

[F01] 读取整个文件
来源：http://gud.kuanghao11.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jri.hnxiangtu.top

PHP:  file_get_contents("a.txt");
来源：http://wcv.shzxlz.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ozv.shangyingyoupin.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vfh.gaohongyu789.top

Java: Files.readString(Path.of("a.txt"))
来源：http://lhz.yueranfly.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kpx.cashguo.top

Ruby: File.read("a.txt")
来源：http://bgk.sufxvd.cn

C#:   File.ReadAllText("a.txt");
来源：http://tpw.sjlbkw.cn

[F02] 逐行读取文件
来源：http://gor.tarul.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://paj.nanxuanxn.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://amg.wangdashe.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zgm.jqgufenzy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://utw.ywan-chungtsiang.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ciq.quarkkingdee.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bnw.birdmap.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nzn.cashguo.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kad.sjlbkw.cn

[F03] 写入文件（覆盖）
来源：http://dzu.hywenlv.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://iuk.yj202588.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://qpz.hnxiangtu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zhi.uphjek.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qsv.ydjk.org.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ajy.guannengcc.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://scv.xinyue.icu

Ruby: File.write("a.txt", "hi")
来源：http://klg.epnwcf.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sxj.zhaomingkeji.xyz

[F04] 追加写入文件
来源：http://tot.yfazqb.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mgy.hammf.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lzn.9152youxi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pim.hnxiangtu.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://imh.ctjpmb.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cpq.jlsjyb.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gbw.hongshengwenyu.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bdn.xylfe.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jql.xuetiantiany.cn

[F05] 判断文件或目录是否存在
来源：http://ott.gogol.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jfg.zhaomingkeji.xyz

PHP:  file_exists("a.txt");
来源：http://vxi.zhongyouzk.top

JS:   fs.existsSync("a.txt")
来源：http://dwg.chenlongwang.top

TS:   fs.existsSync("a.txt")
来源：http://por.uphjek.com

Java: Files.exists(Path.of("a.txt"))
来源：http://kmw.snrcjt.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qlc.jqgufenzy.top

Ruby: File.exist?("a.txt")
来源：http://kyk.zhijiandao.cn

C#:   File.Exists("a.txt")
来源：http://czd.andypj.xyz

[F06] 删除文件
来源：http://gxp.yj20258888.top

Py:   os.remove("a.txt")
来源：http://ihl.feifeiyinyue.top

PHP:  unlink("a.txt");
来源：http://mcg.yj20258888.top

JS:   fs.unlinkSync("a.txt")
来源：http://tvb.hysaishi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://phu.sweek.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jvn.gaohongyu789.top

Go:   os.Remove("a.txt")
来源：http://znj.shanyushiyangkeji.top

Ruby: File.delete("a.txt")
来源：http://kjg.ydjk.org.cn

C#:   File.Delete("a.txt");
来源：http://xco.cheryme.top

[F07] 创建目录（含多级）
来源：http://axo.bbcook.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lrc.jqgfzy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wez.yfazqb.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dwn.shanyushiyangkeji.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cga.fanxiaobao.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kgg.gotoacloud.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rvg.chenlongwang.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://utk.jinqigufen.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rpa.redwolf501.top

[F08] 遍历目录
来源：http://svz.zhixingplan.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://rmc.fzhhl.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://opf.pengpengdd.cyou

JS:   fs.readdirSync("dir")
来源：http://rqy.jianghu66.top

TS:   fs.readdirSync("dir")
来源：http://sju.shuidangran.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rnv.pengpengdd.cyou

Go:   entries, _ := os.ReadDir("dir")
来源：http://rva.guowangkeji.top

Ruby: Dir.children("dir")
来源：http://vup.bbcook.cn

C#:   Directory.GetFiles("dir")
来源：http://jgn.nwbrower.top

[F09] 获取文件大小
来源：http://otk.yj202588.top

Py:   os.path.getsize("a.txt")
来源：http://duc.wangshuangyany.cn

PHP:  filesize("a.txt");
来源：http://qns.0kj1m.cn

JS:   fs.statSync("a.txt").size
来源：http://cic.guowangkeji.top

TS:   fs.statSync("a.txt").size
来源：http://qav.jianghu66.top

Java: Files.size(Path.of("a.txt"))
来源：http://hqc.sjlbkw.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nmc.hfpthk.cn

Ruby: File.size("a.txt")
来源：http://rse.xziqi.cn

C#:   new FileInfo("a.txt").Length
来源：http://gzs.jinqigufen.top

[F10] 取文件扩展名 / 文件名
来源：http://plb.sweek.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lup.yuanzhike.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xhx.gaohongyu789.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fhf.zhoulong.xyz

TS:   path.extname("a.txt")
来源：http://bnu.tianlin.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mic.vqdsnc.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://chd.redwolf501.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pty.jlsjyb.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jjl.jinqigufen.top

[F11] 复制与移动文件
来源：http://jpa.hcnkem.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rjr.316326.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blb.uphjek.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://thm.shanyushiyangkeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dpg.0kj1m.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yya.yangfankeji.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pku.yuanzhike.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gqm.hammf.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sct.c1oappe.top

[F12] CSV 读写
来源：http://fmh.chenzaomai.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rqg.dianchejie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qgr.zdbjq.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hpq.ydjk.org.cn

TS:   // 同上
来源：http://jym.zhiwuduotai.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lkj.hesvh.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hqn.yfazqb.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wwi.hongshengwenyu.top

C#:   // 无内置：用 CsvHelper 库
来源：http://xeu.gogol.net.cn

================================================================================
来源：http://xmq.birdmap.top

G. 面向对象
来源：http://ylh.pengpengdd.cyou

================================================================================
来源：http://yud.zhiwuduotai.top

[G01] 定义类
来源：http://wrs.gogol.net.cn

Py:   class User: pass
来源：http://ajh.kuanghao11.cn

PHP:  class User {}
来源：http://blq.zhiwuduotai.top

JS:   class User {}
来源：http://gjq.cqqwz.cn

TS:   class User { name: string = ""; }
来源：http://zeo.bjfxy.top

Java: class User {}
来源：http://bnf.yuxming.cn

Go:   type User struct { Name string }
来源：http://wvs.zhoulong.xyz

Ruby: class User; end
来源：http://yyc.tianlin.xyz

C#:   class User {}
来源：http://hhm.guowangkeji.top

[G02] 构造函数
来源：http://dro.hongshengwenyu.top

Py:   def __init__(self, name): self.name = name
来源：http://lqt.epnwcf.com

PHP:  public function __construct(public string $name) {}
来源：http://iht.0kj1m.cn

JS:   constructor(name) { this.name = name; }
来源：http://oox.guannengcc.top

TS:   constructor(public name: string) {}
来源：http://lmk.fktsv.cn

Java: User(String name) { this.name = name; }
来源：http://tjp.ydjk.org.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://seh.haohaochexian.top

Ruby: def initialize(name); @name = name; end
来源：http://tpi.pengpengdd.cyou

C#:   public User(string name) { Name = name; }
来源：http://esx.fktsv.cn

[G03] 实例属性
来源：http://rbi.gotoacloud.top

Py:   self.name = "x"
来源：http://hpb.fengsongda.top

PHP:  public string $name = "x";
来源：http://dcv.zycfv.cn


<!-- 参考信息 -->