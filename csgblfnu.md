代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gwa.nanxinkj.top

[E03] 截取子串
来源：http://grn.yj20258.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vcr.guowangkeji.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://miv.hammf.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wvw.hysaishi.cn

TS:   s.slice(1, 4)
来源：http://gbm.pycfn.com

Java: s.substring(1, 4)
来源：http://xij.shanyushiyangkeji.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rhy.kuanghao11.cn

Ruby: s[1, 3];  s[1..3]
来源：http://lwf.tanke756.top

C#:   s.Substring(1, 3)
来源：http://gck.zhaomingkeji.xyz

[E04] 查找子串位置
来源：http://smd.fengsongda.top

Py:   s.find("x");  s.index("x")
来源：http://ehm.ehwqpu.com

PHP:  strpos($s, "x");
来源：http://acb.chenlongwang.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qbe.jqgufenzy.top

TS:   s.indexOf("x")
来源：http://lkx.52xcode.cn

Java: s.indexOf("x")
来源：http://hia.vqdsnc.cn

Go:   strings.Index(s, "x")
来源：http://zkt.ydjk.org.cn

Ruby: s.index("x")
来源：http://nfq.fzhhl.top

C#:   s.IndexOf("x")
来源：http://muc.redwolf501.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://whi.jqgufenzy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nqd.cdnleiting.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tbv.nanxuanxn.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rib.bbcook.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://uqq.bbcook.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kkl.zhengqikj.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vgi.dianchejie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mus.52xcode.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tqf.kuanghao11.cn

[E06] 替换子串
来源：http://zaq.sysykeji.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://htf.cheryme.top

PHP:  str_replace("a", "b", $s);
来源：http://qyr.yj202588.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dsa.yanxiufei.cn

TS:   s.replaceAll("a", "b")
来源：http://nkz.haohaochexian.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hrp.tianlin.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rob.zhaomingkeji.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wzo.xingfuxueyuan.xyz

C#:   s.Replace("a", "b")
来源：http://pbx.hongshengwenyu.top

[E07] 按分隔符拆分
来源：http://qqz.hnqzz.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mls.sxryk.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wlv.pengpengdd.cyou

JS:   s.split(",");  s.split(/\s+/)
来源：http://pdk.sweek.top

TS:   s.split(",")
来源：http://gsd.nanxinkj.top

Java: s.split(",");  s.split("\\s+")
来源：http://prd.cucudq.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kty.yueranfly.top

Ruby: s.split(",");  s.split
来源：http://fba.zhixingplan.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kmu.vehdjk.com

[E08] 数组按分隔符合并
来源：http://mzb.andypj.xyz

Py:   ",".join(items)
来源：http://xpn.pycfn.com

PHP:  implode(",", $items);
来源：http://aji.chenjidiqi.icu

JS:   items.join(",")
来源：http://ttl.hnqzz.top

TS:   items.join(",")
来源：http://zdh.zycfv.cn

Java: String.join(",", items)
来源：http://leu.yj20258888.top

Go:   strings.Join(items, ",")
来源：http://jko.daxiang520.top

Ruby: items.join(",")
来源：http://saw.yfazqb.com

C#:   string.Join(",", items)
来源：http://fps.fktsv.cn

[E09] 去除所有空白字符
来源：http://tfx.sweek.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://eun.ppjwa.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hvz.daria6918.cn

JS:   s.replace(/\s+/g, "")
来源：http://rnn.9152youxi.cn

TS:   s.replace(/\s+/g, "")
来源：http://air.vehdjk.com

Java: s.replaceAll("\\s+", "")
来源：http://cki.snrcjt.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rxx.cdnleiting.top

Ruby: s.gsub(/\s+/, "")
来源：http://frm.aibaodan.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tay.jiagoushi.top

[E10] 左侧补零 / 定长填充
来源：http://xtx.jianghu66.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://afa.yongpay.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bbc.jqgfzy.top

JS:   "7".padStart(3, "0")
来源：http://bxu.gzhubu.top

TS:   "7".padStart(3, "0")
来源：http://tgz.ydjk.org.cn

Java: String.format("%03d", 7)
来源：http://nyt.ydzc1.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://wxk.xylfe.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ckg.tanke756.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qkm.shanyushiyangtech.top

[E11] 反转字符串
来源：http://tjw.mhx1999.top

Py:   s[::-1]
来源：http://vgp.hnqzz.top

PHP:  strrev($s);
来源：http://uqc.xinyue.icu

JS:   [...s].reverse().join("")
来源：http://wsc.ivvv.top

TS:   [...s].reverse().join("")
来源：http://vwq.fktsv.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://kox.hesvh.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://lrb.yonumen.top

Ruby: s.reverse
来源：http://bue.snrcjt.cn

C#:   new string(s.Reverse().ToArray())
来源：http://pot.jinyuanbaomall.cn

[E12] 统计某字符出现次数
来源：http://auu.ivvv.top

Py:   s.count("a")
来源：http://mcw.zhixingplan.top

PHP:  substr_count($s, "a");
来源：http://dus.yonumen.top

JS:   s.split("a").length - 1
来源：http://qog.fanxiaobao.xyz

TS:   s.split("a").length - 1
来源：http://iyv.cucudq.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qrn.zhiwuduotai.top

Go:   strings.Count(s, "a")
来源：http://gln.mhx1999.top

Ruby: s.count("a")
来源：http://ejt.fehbvm.com

C#:   s.Count(c => c == 'a')
来源：http://phf.sysykeji.top

[E13] 逐字符遍历
来源：http://rxz.bjfxy.top

Py:   for ch in s: print(ch)
来源：http://bah.shzxlz.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hts.epnwcf.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://hes.meibo888.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://jbn.shzxlz.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://leh.sysykeji.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ecz.bbcook.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://yjb.pengpengdd.cyou

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qxc.zhoulong.xyz

[E14] URL 编码与 Base64
来源：http://zwm.jinqigufen.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mfc.mhx1999.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://aws.cdnleiting.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sqj.vqdsnc.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://izp.zycfv.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uhw.jqgfzy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zdc.fktsv.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yyt.hysaishi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fwp.hysaishi.cn

[E15] HTML 转义 / 反转义
来源：http://eea.aibaodan.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ino.jinqigufen.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vaf.yvedp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sxu.hfpthk.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://clc.vehdjk.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wku.dianchejie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zzc.snrcjt.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dev.iojbl.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ztj.xingfuxueyuan.xyz

[E16] 数字千分位
来源：http://dqx.epnwcf.com

Py:   f"{1234567:,}"
来源：http://ykp.cqqwz.cn

PHP:  number_format(1234567);
来源：http://auo.hesvh.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://utn.jinqigufen.top

TS:   (1234567).toLocaleString("en-US")
来源：http://zgh.yueranfly.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://egg.jiagoushi.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yba.dianchejie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yts.mhx1999.top

C#:   1234567.ToString("N0")
来源：http://wpz.birdmap.top

[E17] 首字母大写
来源：http://jfy.gotoacloud.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zlc.9152youxi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xyc.9152youxi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wvl.bbcook.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://odz.hysaishi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wjo.jqgufenzy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mbm.xylfe.cn

Ruby: s.capitalize
来源：http://lgz.yvedp.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ast.sjlbkw.cn

[E18] 模板占位符替换
来源：http://fvo.andypj.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vgn.zhengqikj.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hxi.hysaishi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ayp.vehdjk.com

TS:   tpl.replaceAll("{name}", name)
来源：http://nps.feifeiyinyue.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nfw.chenzaomai.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sui.jinghuilouyu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fki.yongpay.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bsa.nanxuanxn.top

[E19] 多行文本按行拆分
来源：http://ajz.dashuyun.cn

Py:   s.splitlines()
来源：http://wzt.52xcode.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tui.sxryk.cn

JS:   s.split(/\r?\n/)
来源：http://oli.quarkkingdee.top

TS:   s.split(/\r?\n/)
来源：http://azk.ywan-chungtsiang.top

Java: s.lines().toList()
来源：http://sam.nanxinkj.top

Go:   strings.Split(s, "\n")
来源：http://ejm.gzhubu.top

Ruby: s.lines
来源：http://vsn.xziqi.cn

C#:   s.Split('\n')
来源：http://spn.yanxiufei.cn

[E20] 判断字符串是否为空
来源：http://kkv.nwbrower.top

Py:   if not s:
来源：http://nhe.hnqzz.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hak.zhiwuduotai.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rpb.xylfe.cn

TS:   if (s === "") {}
来源：http://lah.snrcjt.cn

Java: if (s.isEmpty()) {}
来源：http://sjq.daria6918.cn

Go:   if s == "" {}
来源：http://vua.zhengqikj.top

Ruby: if s.empty?
来源：http://zov.chenlongwang.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xtk.zhongyouzk.top

[E21] 超长截断加省略号
来源：http://pdj.vqdsnc.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gtv.daxiang520.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lyg.ehwqpu.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://clb.hysaishi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jkv.hnqzz.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hno.daria6918.cn

Go:   // 按 rune 判断长度后截断
来源：http://bbt.316326.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fay.quarkkingdee.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uhg.vehdjk.com

[E22] 字节长度与字符长度
来源：http://gaf.tarul.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qya.yueranfly.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dyq.uphjek.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://chc.gaohongyu789.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dsl.fzhhl.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nld.dianchejie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://irg.daxiang520.top

Ruby: s.bytesize;  s.length
来源：http://mba.yfazqb.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tst.tanke756.top

================================================================================
来源：http://ifw.wangdashe.top

F. 文件与目录
来源：http://jvt.zdqjudy.top

================================================================================
来源：http://erl.pycfn.com

[F01] 读取整个文件
来源：http://wsl.haohaochexian.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yzb.bjfxy.top

PHP:  file_get_contents("a.txt");
来源：http://wmx.tianlin.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kvf.pycfn.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bsa.sysykeji.top

Java: Files.readString(Path.of("a.txt"))
来源：http://sgr.yfazqb.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://plb.tianlin.xyz

Ruby: File.read("a.txt")
来源：http://rqy.vqdsnc.cn

C#:   File.ReadAllText("a.txt");
来源：http://olw.bjfxy.top

[F02] 逐行读取文件
来源：http://fks.ybcxt.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://imh.9152youxi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sal.yj202588.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://exw.gaohongyu789.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rry.fengsongda.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jqr.guannengcc.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://soc.pycfn.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cfd.jiagoushi.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ajr.birdmap.top

[F03] 写入文件（覆盖）
来源：http://kvy.shanyushiyangkeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jgz.nanxinkj.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://wqb.guowangkeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jtw.haohaochexian.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dgi.meibo888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cre.tian-w.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fpg.vehdjk.com

Ruby: File.write("a.txt", "hi")
来源：http://ztd.c1oappe.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ctt.cheryme.top

[F04] 追加写入文件
来源：http://knn.jqgufenzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ihx.redwolf501.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wih.fengsongda.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uet.jiagoushi.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://avb.hnxiangtu.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fxq.cashguo.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://oxb.bjfxy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cwu.tian-w.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kzf.uphjek.com

[F05] 判断文件或目录是否存在
来源：http://wyg.bbcook.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jyb.gotoacloud.top

PHP:  file_exists("a.txt");
来源：http://iqz.andypj.xyz

JS:   fs.existsSync("a.txt")
来源：http://fss.dianchejie.cn

TS:   fs.existsSync("a.txt")
来源：http://uhh.zhixingplan.top

Java: Files.exists(Path.of("a.txt"))
来源：http://jqc.zhongyouzk.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sef.zhoulong.xyz

Ruby: File.exist?("a.txt")
来源：http://nbw.sweek.top

C#:   File.Exists("a.txt")
来源：http://xkt.cucudq.cn

[F06] 删除文件
来源：http://ujn.cdnleiting.top

Py:   os.remove("a.txt")
来源：http://rnk.iojbl.cn

PHP:  unlink("a.txt");
来源：http://ogo.shzxlz.cn

JS:   fs.unlinkSync("a.txt")
来源：http://mbd.shangyingyoupin.top

TS:   fs.unlinkSync("a.txt")
来源：http://tji.52xcode.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ztq.9152youxi.cn

Go:   os.Remove("a.txt")
来源：http://mwa.svipenyu.cn

Ruby: File.delete("a.txt")
来源：http://vvm.sysykeji.top

C#:   File.Delete("a.txt");
来源：http://tjo.tarul.cn

[F07] 创建目录（含多级）
来源：http://mkw.hywenlv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://edu.c1oappe.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://swd.yfazqb.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cue.svipenyu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vmj.fanxiaobao.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zpx.bbcook.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://llt.xylfe.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rby.gotoacloud.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://emq.gzhubu.top

[F08] 遍历目录
来源：http://yyj.iojbl.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vdb.jinyuanbaomall.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xst.vehdjk.com

JS:   fs.readdirSync("dir")
来源：http://bng.316326.xyz

TS:   fs.readdirSync("dir")
来源：http://tma.52xcode.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://soi.daxiang520.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://jsp.redwolf501.top

Ruby: Dir.children("dir")
来源：http://zqe.yvedp.cn

C#:   Directory.GetFiles("dir")
来源：http://sui.daria6918.cn

[F09] 获取文件大小
来源：http://sjn.smart0.xyz

Py:   os.path.getsize("a.txt")
来源：http://cbq.yanxiufei.cn

PHP:  filesize("a.txt");
来源：http://fzr.xylfe.cn

JS:   fs.statSync("a.txt").size
来源：http://xgh.ydjk.org.cn

TS:   fs.statSync("a.txt").size
来源：http://lxv.sjlbkw.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bxp.sweek.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yvn.tanke756.top

Ruby: File.size("a.txt")
来源：http://wco.hesvh.cn

C#:   new FileInfo("a.txt").Length
来源：http://grc.yanxiufei.cn

[F10] 取文件扩展名 / 文件名
来源：http://gxv.vqdsnc.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gdz.yvedp.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hna.52xcode.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dns.cashguo.top

TS:   path.extname("a.txt")
来源：http://aon.dashuyun.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hml.gzhubu.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fcy.yonumen.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sqn.daxiang520.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ftr.xylfe.cn

[F11] 复制与移动文件
来源：http://bue.meibo888.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://eul.daria6918.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ykw.xziqi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vfl.bbcook.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tjg.fanxiaobao.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kgk.nwbrower.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ooc.zhiwuduotai.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tlr.zhiwuduotai.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ldy.vqdsnc.cn

[F12] CSV 读写
来源：http://glx.haohaochexian.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rhy.yanxiufei.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xqq.chenlongwang.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ixi.ppjwa.cn

TS:   // 同上
来源：http://gzz.birdmap.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pcn.xuetiantiany.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ezx.yonumen.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://uxr.jinqigufen.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ftm.cdnleiting.top

================================================================================
来源：http://gad.gogol.net.cn

G. 面向对象
来源：http://zct.aizwys.cn

================================================================================
来源：http://rsh.yanxiufei.cn

[G01] 定义类
来源：http://oyr.chenzaomai.com

Py:   class User: pass
来源：http://ofm.zhongyouzk.top

PHP:  class User {}
来源：http://psq.wangshuangyany.cn

JS:   class User {}
来源：http://ypz.bbcook.cn

TS:   class User { name: string = ""; }
来源：http://wvi.sxryk.cn


<!-- 参考信息 -->