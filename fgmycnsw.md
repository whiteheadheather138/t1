代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lwi.zhoulong.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fry.daria6918.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oxw.yj202588.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://kac.gzhubu.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jus.sweek.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nhr.ivvv.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pzt.ywan-chungtsiang.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dfm.sysykeji.top

[E06] 替换子串
来源：http://tmc.cdnleiting.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zrg.snrcjt.cn

PHP:  str_replace("a", "b", $s);
来源：http://hoh.shanyushiyangkeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bjm.zhiwuduotai.top

TS:   s.replaceAll("a", "b")
来源：http://snp.birdmap.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rmb.hnqzz.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nyy.hongshengwenyu.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vxt.jinqigfzy.top

C#:   s.Replace("a", "b")
来源：http://wyx.tarul.cn

[E07] 按分隔符拆分
来源：http://kgy.ydjk.org.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mhc.yvedp.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ajz.hcnkem.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://lie.xylfe.cn

TS:   s.split(",")
来源：http://ebg.aizwys.cn

Java: s.split(",");  s.split("\\s+")
来源：http://rgd.jiagoushi.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ief.dashuyun.cn

Ruby: s.split(",");  s.split
来源：http://xtw.bbcook.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nyt.c1oappe.top

[E08] 数组按分隔符合并
来源：http://lvp.ppjwa.cn

Py:   ",".join(items)
来源：http://ilk.haohaochexian.top

PHP:  implode(",", $items);
来源：http://xtx.quarkkingdee.top

JS:   items.join(",")
来源：http://mrc.ybcxt.top

TS:   items.join(",")
来源：http://cki.kuanghao11.cn

Java: String.join(",", items)
来源：http://fhn.chenjidiqi.icu

Go:   strings.Join(items, ",")
来源：http://xpj.hammf.cn

Ruby: items.join(",")
来源：http://qzy.feifeiyinyue.top

C#:   string.Join(",", items)
来源：http://bcm.tarul.cn

[E09] 去除所有空白字符
来源：http://fvq.yanxiufei.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pko.yfazqb.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://spq.nanxinkj.top

JS:   s.replace(/\s+/g, "")
来源：http://xhq.nwbrower.top

TS:   s.replace(/\s+/g, "")
来源：http://kwl.daria6918.cn

Java: s.replaceAll("\\s+", "")
来源：http://zcy.shanyushiyangtech.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://xxj.yongpay.top

Ruby: s.gsub(/\s+/, "")
来源：http://ggq.guowangkeji.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://niq.daxiang520.top

[E10] 左侧补零 / 定长填充
来源：http://vev.shuidangran.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://okr.ydjk.org.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ess.birdmap.top

JS:   "7".padStart(3, "0")
来源：http://imj.hcnkem.com

TS:   "7".padStart(3, "0")
来源：http://yla.52xcode.cn

Java: String.format("%03d", 7)
来源：http://snr.ydzc1.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://wuh.smart0.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mis.cqqwz.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lmh.gotoacloud.top

[E11] 反转字符串
来源：http://osi.shuidangran.top

Py:   s[::-1]
来源：http://ymd.bjfxy.top

PHP:  strrev($s);
来源：http://wmy.xziqi.cn

JS:   [...s].reverse().join("")
来源：http://jzz.haohaochexian.top

TS:   [...s].reverse().join("")
来源：http://gnq.zhengqikj.top

Java: new StringBuilder(s).reverse().toString()
来源：http://qab.bjfxy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://nci.ehwqpu.com

Ruby: s.reverse
来源：http://mqc.xylfe.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wac.cashguo.top

[E12] 统计某字符出现次数
来源：http://chn.ydjk.org.cn

Py:   s.count("a")
来源：http://xew.sweek.top

PHP:  substr_count($s, "a");
来源：http://aem.hfpthk.cn

JS:   s.split("a").length - 1
来源：http://rfj.nwbrower.top

TS:   s.split("a").length - 1
来源：http://nhk.sjlbkw.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vot.zycfv.cn

Go:   strings.Count(s, "a")
来源：http://ldp.ydjk.org.cn

Ruby: s.count("a")
来源：http://fgp.sysykeji.top

C#:   s.Count(c => c == 'a')
来源：http://fdb.hysaishi.cn

[E13] 逐字符遍历
来源：http://tez.shangyingyoupin.top

Py:   for ch in s: print(ch)
来源：http://lvy.guannengcc.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ngf.chenjidiqi.icu

JS:   for (const ch of s) { console.log(ch); }
来源：http://ypw.aibaodan.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bvz.bjfxy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://eya.ctjpmb.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ypp.shangyingyoupin.top

Ruby: s.each_char { |ch| puts ch }
来源：http://lvp.guannengcc.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xoi.uphjek.com

[E14] URL 编码与 Base64
来源：http://ysx.fengsongda.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yob.chenjidiqi.icu

PHP:  urlencode($s);  base64_encode($s);
来源：http://hut.zhengqikj.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vls.gotoacloud.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://enp.sjlbkw.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://exa.0kj1m.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vol.aibaodan.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kjs.guannengcc.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dki.chenlongwang.top

[E15] HTML 转义 / 反转义
来源：http://dgs.bjfxy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ssl.yuxming.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gye.aibaodan.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ihs.316326.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://qbc.pycfn.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ypb.feifeiyinyue.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gui.vehdjk.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vua.xuanzx.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sxt.hfpthk.cn

[E16] 数字千分位
来源：http://mww.birdmap.top

Py:   f"{1234567:,}"
来源：http://xbl.vehdjk.com

PHP:  number_format(1234567);
来源：http://yxq.nanxinkj.top

JS:   (1234567).toLocaleString("en-US")
来源：http://opd.yongpay.top

TS:   (1234567).toLocaleString("en-US")
来源：http://fvo.sxryk.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jpo.9152youxi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fsp.dashuyun.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fib.vqdsnc.cn

C#:   1234567.ToString("N0")
来源：http://vhf.ydjk.org.cn

[E17] 首字母大写
来源：http://rgo.kuanghao11.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xes.xinyue.icu

PHP:  ucfirst($s);  ucwords($s);
来源：http://inm.yvedp.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://arr.chenlongwang.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aks.sweek.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vik.yj20258888.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bpp.yj20258888.top

Ruby: s.capitalize
来源：http://gwq.hywenlv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tpl.yfazqb.com

[E18] 模板占位符替换
来源：http://bur.aizwys.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gmm.cheryme.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ufu.zhijiandao.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://usr.hywenlv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://wrn.redwolf501.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tbx.iojbl.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gkn.yj20258.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fer.zdqjudy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://awo.jinqigufen.top

[E19] 多行文本按行拆分
来源：http://xln.hcnkem.com

Py:   s.splitlines()
来源：http://sqt.0kj1m.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gij.hcnkem.com

JS:   s.split(/\r?\n/)
来源：http://gsm.fanxiaobao.xyz

TS:   s.split(/\r?\n/)
来源：http://wqc.yj20258.top

Java: s.lines().toList()
来源：http://gvv.cdnleiting.top

Go:   strings.Split(s, "\n")
来源：http://xjn.hammf.cn

Ruby: s.lines
来源：http://dii.hesvh.cn

C#:   s.Split('\n')
来源：http://jjd.bjfxy.top

[E20] 判断字符串是否为空
来源：http://wbn.chenzaomai.com

Py:   if not s:
来源：http://ixp.bjfxy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xar.chenlongwang.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://iok.yj202588.top

TS:   if (s === "") {}
来源：http://fca.svipenyu.cn

Java: if (s.isEmpty()) {}
来源：http://zhw.tanke756.top

Go:   if s == "" {}
来源：http://mzl.chenzaomai.com

Ruby: if s.empty?
来源：http://rfr.nwbrower.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yjk.yj20258888.top

[E21] 超长截断加省略号
来源：http://uri.yj20258.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ytw.yuxming.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ycu.316326.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cwc.ydzc1.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gvi.xinyue.icu

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rdu.smart0.xyz

Go:   // 按 rune 判断长度后截断
来源：http://kqb.feifeiyinyue.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://acn.xuetiantiany.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hhw.aibaodan.cn

[E22] 字节长度与字符长度
来源：http://fgd.fanxiaobao.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jxo.yonumen.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nxf.nwbrower.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ucf.daria6918.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rgb.0kj1m.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qak.sjlbkw.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://npj.snrcjt.cn

Ruby: s.bytesize;  s.length
来源：http://dpf.yongpay.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jjw.zycfv.cn

================================================================================
来源：http://emh.hfpthk.cn

F. 文件与目录
来源：http://fvw.yj20258.top

================================================================================
来源：http://igy.xylfe.cn

[F01] 读取整个文件
来源：http://gie.smart0.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xqn.jinqigufen.top

PHP:  file_get_contents("a.txt");
来源：http://btd.snrcjt.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vui.ywan-chungtsiang.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jeg.cucudq.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jdy.aibaodan.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zaa.yonumen.top

Ruby: File.read("a.txt")
来源：http://jli.sufxvd.cn

C#:   File.ReadAllText("a.txt");
来源：http://mgo.shzxlz.cn

[F02] 逐行读取文件
来源：http://ufq.ywan-chungtsiang.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vve.cqqwz.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://oub.yuxming.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://knx.hnxiangtu.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://snm.cucudq.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hjw.chenlongwang.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bhu.zhijiandao.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jtm.nanxinkj.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vks.jinqigfzy.top

[F03] 写入文件（覆盖）
来源：http://msi.guowangkeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fvm.yj202588.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://vfc.tanke756.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baf.xziqi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sfq.tanke756.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://eiu.tianlin.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rya.redwolf501.top

Ruby: File.write("a.txt", "hi")
来源：http://xsz.fzhhl.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jud.fengsongda.top

[F04] 追加写入文件
来源：http://duu.gotoacloud.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ypk.nanxinkj.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rqb.ctjpmb.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pna.jyoumei.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://owo.shangyingyoupin.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://onp.9152youxi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wcd.haohaochexian.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yka.xylfe.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nui.jinqigufen.top

[F05] 判断文件或目录是否存在
来源：http://xsg.ppjwa.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://iur.zhijiandao.cn

PHP:  file_exists("a.txt");
来源：http://xkj.zdqjudy.top

JS:   fs.existsSync("a.txt")
来源：http://pvy.gogol.net.cn

TS:   fs.existsSync("a.txt")
来源：http://sxh.jinyuanbaomall.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://myk.dianchejie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bsz.ivvv.top

Ruby: File.exist?("a.txt")
来源：http://xeq.fanxiaobao.xyz

C#:   File.Exists("a.txt")
来源：http://ueg.52xcode.cn

[F06] 删除文件
来源：http://dnz.c1oappe.top

Py:   os.remove("a.txt")
来源：http://wbt.zdqjudy.top

PHP:  unlink("a.txt");
来源：http://quy.jiagoushi.top

JS:   fs.unlinkSync("a.txt")
来源：http://tse.hysaishi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://goc.gzhubu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pnr.mhx1999.top

Go:   os.Remove("a.txt")
来源：http://ugq.jyoumei.cn

Ruby: File.delete("a.txt")
来源：http://afw.fengsongda.top

C#:   File.Delete("a.txt");
来源：http://swc.andypj.xyz

[F07] 创建目录（含多级）
来源：http://qwk.havefunace.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ecz.guannengcc.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ybr.mhx1999.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://unb.jianghu66.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cnp.xylfe.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sdk.ydzc1.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nwk.hammf.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fxo.cucudq.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qav.sufxvd.cn

[F08] 遍历目录
来源：http://gew.cashguo.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ucq.haohaochexian.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rah.shangyingyoupin.top

JS:   fs.readdirSync("dir")
来源：http://wpi.xinyue.icu

TS:   fs.readdirSync("dir")
来源：http://tqn.hcnkem.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vmj.cashguo.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://jfl.guannengcc.top

Ruby: Dir.children("dir")
来源：http://rcs.ydzc1.top

C#:   Directory.GetFiles("dir")
来源：http://mkt.sysykeji.top

[F09] 获取文件大小
来源：http://vgw.gotoacloud.top

Py:   os.path.getsize("a.txt")
来源：http://gnq.jqgufenzy.top

PHP:  filesize("a.txt");
来源：http://rls.daria6918.cn

JS:   fs.statSync("a.txt").size
来源：http://xgh.cqqwz.cn

TS:   fs.statSync("a.txt").size
来源：http://hed.xuetiantiany.cn

Java: Files.size(Path.of("a.txt"))
来源：http://guj.uphjek.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ref.andypj.xyz

Ruby: File.size("a.txt")
来源：http://igl.hcnkem.com

C#:   new FileInfo("a.txt").Length
来源：http://cxz.xylfe.cn

[F10] 取文件扩展名 / 文件名
来源：http://ofj.tian-w.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wmb.ivvv.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xeu.redwolf501.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cbl.wangdashe.top

TS:   path.extname("a.txt")
来源：http://jfn.nwbrower.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gbb.zycfv.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hwi.9152youxi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sgj.jianghu66.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ohy.yanxiufei.cn

[F11] 复制与移动文件
来源：http://fnk.shanyushiyangkeji.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qae.vqdsnc.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://amg.bbcook.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hzc.xuetiantiany.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rkm.yueranfly.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yit.fktsv.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lao.sjlbkw.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://iaj.redwolf501.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tcs.chenlongwang.top

[F12] CSV 读写
来源：http://zuo.chenzaomai.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nwb.andypj.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jkd.shanyushiyangkeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cis.xylfe.cn

TS:   // 同上
来源：http://dsh.yuxming.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nsg.birdmap.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vkl.ywan-chungtsiang.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dqe.xinyue.icu

C#:   // 无内置：用 CsvHelper 库
来源：http://rjr.fanxiaobao.xyz

================================================================================
来源：http://zbv.pengpengdd.cyou

G. 面向对象
来源：http://lyc.9152youxi.cn

================================================================================
来源：http://wrz.xinyue.icu

[G01] 定义类
来源：http://dyu.chenzaomai.com

Py:   class User: pass
来源：http://egy.shuidangran.top

PHP:  class User {}
来源：http://uog.ydzc1.top

JS:   class User {}
来源：http://isb.jianghu66.top

TS:   class User { name: string = ""; }
来源：http://mua.zdqjudy.top

Java: class User {}
来源：http://prq.hammf.cn

Go:   type User struct { Name string }
来源：http://mpn.bbcook.cn

Ruby: class User; end
来源：http://qdv.yvedp.cn

C#:   class User {}
来源：http://lvf.svipenyu.cn

[G02] 构造函数
来源：http://nle.feifeiyinyue.top

Py:   def __init__(self, name): self.name = name
来源：http://ydq.tianlin.xyz

PHP:  public function __construct(public string $name) {}
来源：http://czt.svipenyu.cn

JS:   constructor(name) { this.name = name; }
来源：http://odc.vqdsnc.cn

TS:   constructor(public name: string) {}
来源：http://vwz.hysaishi.cn

Java: User(String name) { this.name = name; }
来源：http://dsr.zhongyouzk.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://owq.xingfuxueyuan.xyz

Ruby: def initialize(name); @name = name; end
来源：http://gop.yj20258.top

C#:   public User(string name) { Name = name; }
来源：http://srj.gzhubu.top

[G03] 实例属性
来源：http://fpj.sufxvd.cn

Py:   self.name = "x"
来源：http://usu.guannengcc.top

PHP:  public string $name = "x";
来源：http://ife.ydzc1.top

JS:   this.name = "x";
来源：http://fmz.meibo888.top

TS:   name: string = "x";
来源：http://yfz.cheryme.top

Java: private String name;
来源：http://tgm.ydzc1.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yfc.epnwcf.com


<!-- 参考信息 -->