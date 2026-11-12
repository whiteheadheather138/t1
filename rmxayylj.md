代发 wailian999

PHP:  strpos($s, "x");
来源：http://csz.hcnkem.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://buc.svipenyu.cn

TS:   s.indexOf("x")
来源：http://kxq.feifeiyinyue.top

Java: s.indexOf("x")
来源：http://ukz.gaohongyu789.top

Go:   strings.Index(s, "x")
来源：http://kuu.yongpay.top

Ruby: s.index("x")
来源：http://qlw.dashuyun.cn

C#:   s.IndexOf("x")
来源：http://lkw.hnqzz.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://yai.zdbjq.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ncm.hnqzz.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://uij.jianghu66.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ozk.ydjk.org.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://tve.cashguo.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rtq.fanxiaobao.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://edd.mhx1999.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://erz.cucudq.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://iou.hesvh.cn

[E06] 替换子串
来源：http://vpx.fehbvm.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ewb.c1oappe.top

PHP:  str_replace("a", "b", $s);
来源：http://dzn.meibo888.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kfo.52xcode.cn

TS:   s.replaceAll("a", "b")
来源：http://vxn.yj20258888.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bin.pycfn.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gdq.gogol.net.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yfj.jinqigufen.top

C#:   s.Replace("a", "b")
来源：http://vwh.hesvh.cn

[E07] 按分隔符拆分
来源：http://rho.yuxming.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sub.bjfxy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mzl.sweek.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://hyw.shanyushiyangkeji.top

TS:   s.split(",")
来源：http://bgj.epnwcf.com

Java: s.split(",");  s.split("\\s+")
来源：http://hyp.hongshengwenyu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bgl.hcnkem.com

Ruby: s.split(",");  s.split
来源：http://iko.hesvh.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ksc.zhongyouzk.top

[E08] 数组按分隔符合并
来源：http://fmr.dianchejie.cn

Py:   ",".join(items)
来源：http://rhm.vqdsnc.cn

PHP:  implode(",", $items);
来源：http://hda.hywenlv.cn

JS:   items.join(",")
来源：http://ybg.feifeiyinyue.top

TS:   items.join(",")
来源：http://hkq.yangfankeji.com

Java: String.join(",", items)
来源：http://snw.hfpthk.cn

Go:   strings.Join(items, ",")
来源：http://lli.zhijiandao.cn

Ruby: items.join(",")
来源：http://tav.zhaomingkeji.xyz

C#:   string.Join(",", items)
来源：http://onm.316326.xyz

[E09] 去除所有空白字符
来源：http://hto.zycfv.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ird.daria6918.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://osl.vehdjk.com

JS:   s.replace(/\s+/g, "")
来源：http://jqt.wangdashe.top

TS:   s.replace(/\s+/g, "")
来源：http://vod.zhongyouzk.top

Java: s.replaceAll("\\s+", "")
来源：http://exu.hywenlv.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://dll.dashuyun.cn

Ruby: s.gsub(/\s+/, "")
来源：http://csq.ybcxt.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jpq.jiagoushi.top

[E10] 左侧补零 / 定长填充
来源：http://sel.xylfe.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rbb.ywan-chungtsiang.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://iaf.52xcode.cn

JS:   "7".padStart(3, "0")
来源：http://tah.ctjpmb.com

TS:   "7".padStart(3, "0")
来源：http://vpf.cucudq.cn

Java: String.format("%03d", 7)
来源：http://cbk.pycfn.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://puk.fehbvm.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fcf.yongpay.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gjo.gogol.net.cn

[E11] 反转字符串
来源：http://gwx.hongshengwenyu.top

Py:   s[::-1]
来源：http://krc.chenzaomai.com

PHP:  strrev($s);
来源：http://eja.cheryme.top

JS:   [...s].reverse().join("")
来源：http://bgl.yj202588.top

TS:   [...s].reverse().join("")
来源：http://knq.mhx1999.top

Java: new StringBuilder(s).reverse().toString()
来源：http://gfn.tianlin.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://eur.0kj1m.cn

Ruby: s.reverse
来源：http://qtg.yongpay.top

C#:   new string(s.Reverse().ToArray())
来源：http://ljg.shanyushiyangtech.top

[E12] 统计某字符出现次数
来源：http://ciq.smart0.xyz

Py:   s.count("a")
来源：http://fak.ydzc1.top

PHP:  substr_count($s, "a");
来源：http://lgo.gogol.net.cn

JS:   s.split("a").length - 1
来源：http://mgu.hesvh.cn

TS:   s.split("a").length - 1
来源：http://aea.0kj1m.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ffx.gotoacloud.top

Go:   strings.Count(s, "a")
来源：http://scf.xuetiantiany.cn

Ruby: s.count("a")
来源：http://jbb.meibo888.top

C#:   s.Count(c => c == 'a')
来源：http://sel.svipenyu.cn

[E13] 逐字符遍历
来源：http://swj.yfazqb.com

Py:   for ch in s: print(ch)
来源：http://jvt.xylfe.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://und.hnqzz.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://moa.cashguo.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://dvq.bjfxy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jcr.yuanzhike.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fjz.shanyushiyangkeji.top

Ruby: s.each_char { |ch| puts ch }
来源：http://owi.zhiwuduotai.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://chb.zhiwuduotai.top

[E14] URL 编码与 Base64
来源：http://bfk.jqgfzy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xsk.yj20258888.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://jst.9152youxi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xkq.zhaomingkeji.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mry.jinqigufen.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cxi.zhijiandao.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://iwd.nanxinkj.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ubg.haohaochexian.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yrb.xylfe.cn

[E15] HTML 转义 / 反转义
来源：http://hyq.jianghu66.top

Py:   html.escape(s);  html.unescape(s)
来源：http://oeh.shuidangran.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dns.xuetiantiany.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bet.hammf.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jmo.sxryk.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uuj.chenjidiqi.icu

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jxt.tian-w.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rzm.fzhhl.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hfe.zhoulong.xyz

[E16] 数字千分位
来源：http://ydc.52xcode.cn

Py:   f"{1234567:,}"
来源：http://tjm.yongpay.top

PHP:  number_format(1234567);
来源：http://rxq.bbcook.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://bfk.jlsjyb.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://nen.sysykeji.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://aqv.chenjidiqi.icu

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ftp.9152youxi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mrf.zhongyouzk.top

C#:   1234567.ToString("N0")
来源：http://ujx.xingfuxueyuan.xyz

[E17] 首字母大写
来源：http://zfe.shangyingyoupin.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nvs.sweek.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://fqr.jqgfzy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qmn.hywenlv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wsq.hnxiangtu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qrh.ydzc1.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lah.jyoumei.cn

Ruby: s.capitalize
来源：http://bht.ppjwa.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jso.havefunace.top

[E18] 模板占位符替换
来源：http://rny.svipenyu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ucr.xuanzx.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tbm.haohaochexian.top

JS:   tpl.replaceAll("{name}", name)
来源：http://udz.nanxinkj.top

TS:   tpl.replaceAll("{name}", name)
来源：http://zqu.fanxiaobao.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://axl.mhx1999.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lwh.hammf.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wcx.sufxvd.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qik.tianlin.xyz

[E19] 多行文本按行拆分
来源：http://fhh.daria6918.cn

Py:   s.splitlines()
来源：http://irz.tanke756.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tpg.zhoulong.xyz

JS:   s.split(/\r?\n/)
来源：http://yav.hnxiangtu.top

TS:   s.split(/\r?\n/)
来源：http://sqk.hnqzz.top

Java: s.lines().toList()
来源：http://ltd.jinghuilouyu.cn

Go:   strings.Split(s, "\n")
来源：http://dxi.dianchejie.cn

Ruby: s.lines
来源：http://bni.kuanghao11.cn

C#:   s.Split('\n')
来源：http://lwi.xuetiantiany.cn

[E20] 判断字符串是否为空
来源：http://tld.jqgfzy.top

Py:   if not s:
来源：http://sit.sxryk.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cjc.yonumen.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zir.hammf.cn

TS:   if (s === "") {}
来源：http://dak.sjlbkw.cn

Java: if (s.isEmpty()) {}
来源：http://lnm.hnqzz.top

Go:   if s == "" {}
来源：http://ott.chenzaomai.com

Ruby: if s.empty?
来源：http://enf.xuetiantiany.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://chs.fehbvm.com

[E21] 超长截断加省略号
来源：http://rku.yfazqb.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rmp.zhengqikj.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lbu.aizwys.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fti.yfazqb.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://esn.yfazqb.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ygm.sufxvd.cn

Go:   // 按 rune 判断长度后截断
来源：http://jjb.xingfuxueyuan.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vlx.bjfxy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jnc.cucudq.cn

[E22] 字节长度与字符长度
来源：http://amc.yfazqb.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://msc.yj20258888.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nlr.sxryk.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hxd.hammf.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://awm.0kj1m.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://eac.zdbjq.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kll.mhx1999.top

Ruby: s.bytesize;  s.length
来源：http://wvr.fzhhl.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sce.cdnleiting.top

================================================================================
来源：http://vec.yanxiufei.cn

F. 文件与目录
来源：http://rvb.zhoulong.xyz

================================================================================
来源：http://cik.jlsjyb.cn

[F01] 读取整个文件
来源：http://zmh.nanxuanxn.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fxu.daxiang520.top

PHP:  file_get_contents("a.txt");
来源：http://jrb.bbcook.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nmc.tian-w.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://api.hywenlv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://nie.iojbl.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tlk.iojbl.cn

Ruby: File.read("a.txt")
来源：http://ogj.gaohongyu789.top

C#:   File.ReadAllText("a.txt");
来源：http://mzs.yj202588.top

[F02] 逐行读取文件
来源：http://kwm.shuidangran.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kza.xingfuxueyuan.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://row.zhiwuduotai.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aay.jinqigfzy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sma.jinghuilouyu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jwy.birdmap.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://myv.fktsv.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xjf.gotoacloud.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xtq.guowangkeji.top

[F03] 写入文件（覆盖）
来源：http://mft.zdbjq.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://uvd.yj202588.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://bwy.hammf.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bkv.xuanzx.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ifi.ydzc1.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qbw.hysaishi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xkm.pengpengdd.cyou

Ruby: File.write("a.txt", "hi")
来源：http://oyd.zhijiandao.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tdq.aizwys.cn

[F04] 追加写入文件
来源：http://wvk.uphjek.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pdn.ybcxt.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cdi.xziqi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ljg.wangdashe.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yte.ywan-chungtsiang.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cva.iojbl.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xfr.zhiwuduotai.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gkw.yuxming.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://teg.kuanghao11.cn

[F05] 判断文件或目录是否存在
来源：http://ego.zdqjudy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lrj.yvedp.cn

PHP:  file_exists("a.txt");
来源：http://wsx.dianchejie.cn

JS:   fs.existsSync("a.txt")
来源：http://jqv.xingfuxueyuan.xyz

TS:   fs.existsSync("a.txt")
来源：http://ekf.shangyingyoupin.top

Java: Files.exists(Path.of("a.txt"))
来源：http://tbl.yanxiufei.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://job.hysaishi.cn

Ruby: File.exist?("a.txt")
来源：http://fpm.smart0.xyz

C#:   File.Exists("a.txt")
来源：http://ovn.xinyue.icu

[F06] 删除文件
来源：http://mwg.yuxming.cn

Py:   os.remove("a.txt")
来源：http://vrg.svipenyu.cn

PHP:  unlink("a.txt");
来源：http://sxv.zhengqikj.top

JS:   fs.unlinkSync("a.txt")
来源：http://qwq.hfpthk.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fkt.fengsongda.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mmw.cashguo.top

Go:   os.Remove("a.txt")
来源：http://mvx.havefunace.top

Ruby: File.delete("a.txt")
来源：http://ppf.sysykeji.top

C#:   File.Delete("a.txt");
来源：http://pvt.smart0.xyz

[F07] 创建目录（含多级）
来源：http://hqx.hfpthk.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jal.cqqwz.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rgi.zhongyouzk.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fun.jinyuanbaomall.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jfb.chenzaomai.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cxk.yvedp.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xoe.sjlbkw.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ccm.cqqwz.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pew.sufxvd.cn

[F08] 遍历目录
来源：http://ahj.bjfxy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://kku.tianlin.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cnn.nwbrower.top

JS:   fs.readdirSync("dir")
来源：http://vlf.xuanzx.com

TS:   fs.readdirSync("dir")
来源：http://kfb.bjfxy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://voc.kuanghao11.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yqx.snrcjt.cn

Ruby: Dir.children("dir")
来源：http://grn.9152youxi.cn

C#:   Directory.GetFiles("dir")
来源：http://ckf.aibaodan.cn

[F09] 获取文件大小
来源：http://cre.jlsjyb.cn

Py:   os.path.getsize("a.txt")
来源：http://xjj.wangshuangyany.cn

PHP:  filesize("a.txt");
来源：http://edj.snrcjt.cn

JS:   fs.statSync("a.txt").size
来源：http://hca.zhijiandao.cn

TS:   fs.statSync("a.txt").size
来源：http://qwi.mhx1999.top

Java: Files.size(Path.of("a.txt"))
来源：http://cpk.iojbl.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rws.yanxiufei.cn

Ruby: File.size("a.txt")
来源：http://crx.zdbjq.cn

C#:   new FileInfo("a.txt").Length
来源：http://xlu.yangfankeji.com

[F10] 取文件扩展名 / 文件名
来源：http://dkm.dashuyun.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hjr.wangdashe.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rmi.chenlongwang.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yys.cashguo.top

TS:   path.extname("a.txt")
来源：http://uim.shuidangran.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://znt.tanke756.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ttj.zdbjq.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ppw.nanxuanxn.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ixs.xinyue.icu

[F11] 复制与移动文件
来源：http://vzf.shanyushiyangtech.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://apy.daxiang520.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rvm.gotoacloud.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blu.yueranfly.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qri.shanyushiyangtech.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fvx.0kj1m.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hty.nwbrower.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nmb.fanxiaobao.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ykj.xylfe.cn

[F12] CSV 读写
来源：http://fhu.guowangkeji.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nmy.hcnkem.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gbb.hysaishi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://noh.svipenyu.cn

TS:   // 同上
来源：http://nri.316326.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xnq.xuanzx.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nyc.xziqi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://alf.xingfuxueyuan.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://uzy.zhixingplan.top

================================================================================
来源：http://udh.wangdashe.top

G. 面向对象
来源：http://gma.ehwqpu.com

================================================================================
来源：http://qbo.yfazqb.com

[G01] 定义类
来源：http://tty.vqdsnc.cn

Py:   class User: pass
来源：http://uxo.gotoacloud.top

PHP:  class User {}
来源：http://brt.52xcode.cn

JS:   class User {}
来源：http://zxq.ppjwa.cn

TS:   class User { name: string = ""; }
来源：http://xob.cashguo.top

Java: class User {}
来源：http://whc.kuanghao11.cn

Go:   type User struct { Name string }
来源：http://fet.ywan-chungtsiang.top

Ruby: class User; end
来源：http://lqo.redwolf501.top

C#:   class User {}
来源：http://beo.jianghu66.top

[G02] 构造函数
来源：http://znm.jqgufenzy.top

Py:   def __init__(self, name): self.name = name
来源：http://dpf.zhengqikj.top

PHP:  public function __construct(public string $name) {}
来源：http://rbz.vqdsnc.cn

JS:   constructor(name) { this.name = name; }
来源：http://qed.cheryme.top

TS:   constructor(public name: string) {}
来源：http://vjs.nanxinkj.top

Java: User(String name) { this.name = name; }
来源：http://smg.hfpthk.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cvy.fanxiaobao.xyz

Ruby: def initialize(name); @name = name; end
来源：http://gjh.nanxuanxn.top


<!-- 参考信息 -->