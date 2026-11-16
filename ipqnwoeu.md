代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kvk.yj20258888.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ioa.pycfn.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fsw.jinyuanbaomall.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pum.chenjidiqi.icu

[E06] 替换子串
来源：http://lbm.sjlbkw.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cji.c1oappe.top

PHP:  str_replace("a", "b", $s);
来源：http://kfe.zhengqikj.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cen.hnxiangtu.top

TS:   s.replaceAll("a", "b")
来源：http://dbx.cdnleiting.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yyo.chenjidiqi.icu

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ztf.hongshengwenyu.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gea.yfazqb.com

C#:   s.Replace("a", "b")
来源：http://ymb.wangshuangyany.cn

[E07] 按分隔符拆分
来源：http://vng.xingfuxueyuan.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gdh.hfpthk.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://skb.vehdjk.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://vie.xziqi.cn

TS:   s.split(",")
来源：http://ebb.wangdashe.top

Java: s.split(",");  s.split("\\s+")
来源：http://zsu.cheryme.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://voe.yvedp.cn

Ruby: s.split(",");  s.split
来源：http://yqf.jiagoushi.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://edo.jianghu66.top

[E08] 数组按分隔符合并
来源：http://tae.sxryk.cn

Py:   ",".join(items)
来源：http://zdl.c1oappe.top

PHP:  implode(",", $items);
来源：http://qxa.vqdsnc.cn

JS:   items.join(",")
来源：http://gwq.tanke756.top

TS:   items.join(",")
来源：http://wzz.zdbjq.cn

Java: String.join(",", items)
来源：http://qhs.snrcjt.cn

Go:   strings.Join(items, ",")
来源：http://ctg.hnxiangtu.top

Ruby: items.join(",")
来源：http://dlg.xuanzx.com

C#:   string.Join(",", items)
来源：http://chh.shzxlz.cn

[E09] 去除所有空白字符
来源：http://zad.ydjk.org.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ikg.ybcxt.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://htu.fanxiaobao.xyz

JS:   s.replace(/\s+/g, "")
来源：http://cmh.aizwys.cn

TS:   s.replace(/\s+/g, "")
来源：http://olo.hysaishi.cn

Java: s.replaceAll("\\s+", "")
来源：http://srq.aizwys.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://fxz.snrcjt.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hfu.316326.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vmx.xylfe.cn

[E10] 左侧补零 / 定长填充
来源：http://lnr.bjfxy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://uwa.zhixingplan.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pdv.hesvh.cn

JS:   "7".padStart(3, "0")
来源：http://fxu.yangfankeji.com

TS:   "7".padStart(3, "0")
来源：http://bms.chenlongwang.top

Java: String.format("%03d", 7)
来源：http://akq.iojbl.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://jdy.gotoacloud.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dtx.sweek.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wte.kuanghao11.cn

[E11] 反转字符串
来源：http://plc.birdmap.top

Py:   s[::-1]
来源：http://gvp.quarkkingdee.top

PHP:  strrev($s);
来源：http://zls.hnqzz.top

JS:   [...s].reverse().join("")
来源：http://xtv.ivvv.top

TS:   [...s].reverse().join("")
来源：http://hew.shanyushiyangkeji.top

Java: new StringBuilder(s).reverse().toString()
来源：http://rey.hnxiangtu.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://zws.xylfe.cn

Ruby: s.reverse
来源：http://nhm.bbcook.cn

C#:   new string(s.Reverse().ToArray())
来源：http://kvs.smart0.xyz

[E12] 统计某字符出现次数
来源：http://jsk.tian-w.cn

Py:   s.count("a")
来源：http://alz.fengsongda.top

PHP:  substr_count($s, "a");
来源：http://bmn.chenjidiqi.icu

JS:   s.split("a").length - 1
来源：http://rtk.vqdsnc.cn

TS:   s.split("a").length - 1
来源：http://kcj.smart0.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lpp.hysaishi.cn

Go:   strings.Count(s, "a")
来源：http://vuq.nanxuanxn.top

Ruby: s.count("a")
来源：http://dew.c1oappe.top

C#:   s.Count(c => c == 'a')
来源：http://coo.ydzc1.top

[E13] 逐字符遍历
来源：http://xvh.zhengqikj.top

Py:   for ch in s: print(ch)
来源：http://yqr.yj20258888.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vvi.snrcjt.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rif.zhaomingkeji.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://hpa.nanxinkj.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vju.nwbrower.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zrj.xylfe.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://mry.andypj.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ryz.yanxiufei.cn

[E14] URL 编码与 Base64
来源：http://utb.hnxiangtu.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rgt.gotoacloud.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://cdb.nanxuanxn.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ygt.tanke756.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ejb.fanxiaobao.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yox.nanxuanxn.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zap.vqdsnc.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cbt.gogol.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ioo.52xcode.cn

[E15] HTML 转义 / 反转义
来源：http://aak.jiagoushi.top

Py:   html.escape(s);  html.unescape(s)
来源：http://zru.fanxiaobao.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kcl.pengpengdd.cyou

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dsb.yueranfly.top

TS:   // 同上，务必做 XSS 过滤
来源：http://olg.jqgufenzy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hri.hfpthk.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wef.chenlongwang.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gps.guowangkeji.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jfs.jqgfzy.top

[E16] 数字千分位
来源：http://uas.haohaochexian.top

Py:   f"{1234567:,}"
来源：http://xve.daria6918.cn

PHP:  number_format(1234567);
来源：http://fbq.yj20258888.top

JS:   (1234567).toLocaleString("en-US")
来源：http://iyv.zhaomingkeji.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://zym.sxryk.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mzt.pycfn.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fdn.chenzaomai.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dwd.zhongyouzk.top

C#:   1234567.ToString("N0")
来源：http://hfg.feifeiyinyue.top

[E17] 首字母大写
来源：http://neo.9152youxi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tuf.hcnkem.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://roe.sjlbkw.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dbp.ywan-chungtsiang.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fps.svipenyu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://osk.shanyushiyangkeji.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kqd.yfazqb.com

Ruby: s.capitalize
来源：http://xwv.yj20258.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pxd.hnxiangtu.top

[E18] 模板占位符替换
来源：http://auj.yongpay.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wdo.shuidangran.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qjo.smart0.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://zwg.zhaomingkeji.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://rol.sxryk.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qdc.shangyingyoupin.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cdb.bjfxy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ffu.fktsv.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://muj.daria6918.cn

[E19] 多行文本按行拆分
来源：http://lod.shangyingyoupin.top

Py:   s.splitlines()
来源：http://wet.ivvv.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://clb.uphjek.com

JS:   s.split(/\r?\n/)
来源：http://xru.hesvh.cn

TS:   s.split(/\r?\n/)
来源：http://oor.redwolf501.top

Java: s.lines().toList()
来源：http://war.sysykeji.top

Go:   strings.Split(s, "\n")
来源：http://isu.zhiwuduotai.top

Ruby: s.lines
来源：http://xkh.yuxming.cn

C#:   s.Split('\n')
来源：http://bzk.gogol.net.cn

[E20] 判断字符串是否为空
来源：http://tun.gaohongyu789.top

Py:   if not s:
来源：http://zwb.ydjk.org.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://aek.jinghuilouyu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://imr.gzhubu.top

TS:   if (s === "") {}
来源：http://vgq.hcnkem.com

Java: if (s.isEmpty()) {}
来源：http://hnh.guowangkeji.top

Go:   if s == "" {}
来源：http://rxr.andypj.xyz

Ruby: if s.empty?
来源：http://djk.zhaomingkeji.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://anj.shangyingyoupin.top

[E21] 超长截断加省略号
来源：http://rpu.ctjpmb.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://drk.pycfn.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kea.gotoacloud.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tbw.zycfv.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pow.bbcook.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ybj.bbcook.cn

Go:   // 按 rune 判断长度后截断
来源：http://fwg.zhiwuduotai.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dlr.gogol.net.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kkc.shanyushiyangkeji.top

[E22] 字节长度与字符长度
来源：http://nje.hnqzz.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jfl.yueranfly.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ijo.jqgfzy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://eke.yuxming.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nwj.andypj.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uiy.jqgufenzy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tpf.yongpay.top

Ruby: s.bytesize;  s.length
来源：http://pcr.yvedp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cqy.fzhhl.top

================================================================================
来源：http://mne.wangdashe.top

F. 文件与目录
来源：http://iif.sysykeji.top

================================================================================
来源：http://ugr.jiagoushi.top

[F01] 读取整个文件
来源：http://jcj.yj20258.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nat.yueranfly.top

PHP:  file_get_contents("a.txt");
来源：http://xea.hnxiangtu.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qbm.tian-w.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qfr.xylfe.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ait.fehbvm.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nle.quarkkingdee.top

Ruby: File.read("a.txt")
来源：http://egc.hysaishi.cn

C#:   File.ReadAllText("a.txt");
来源：http://qae.daria6918.cn

[F02] 逐行读取文件
来源：http://sdm.gotoacloud.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vyt.zhijiandao.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ssp.xinyue.icu

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lmc.guowangkeji.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ett.sxryk.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://akp.dashuyun.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dgi.shanyushiyangtech.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://myq.shanyushiyangkeji.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qnw.jianghu66.top

[F03] 写入文件（覆盖）
来源：http://wnf.cdnleiting.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pdt.chenzaomai.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://qsj.aizwys.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jgm.andypj.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wgz.jqgfzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zri.yfazqb.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tng.zhixingplan.top

Ruby: File.write("a.txt", "hi")
来源：http://yyr.fanxiaobao.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cmh.snrcjt.cn

[F04] 追加写入文件
来源：http://pxs.hammf.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qnn.cashguo.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://iln.dashuyun.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://loo.bbcook.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://khr.hesvh.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bhf.vehdjk.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ouh.hnxiangtu.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yny.jlsjyb.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dvo.haohaochexian.top

[F05] 判断文件或目录是否存在
来源：http://qih.sufxvd.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://oaj.bjfxy.top

PHP:  file_exists("a.txt");
来源：http://hlq.dianchejie.cn

JS:   fs.existsSync("a.txt")
来源：http://his.jyoumei.cn

TS:   fs.existsSync("a.txt")
来源：http://vry.sweek.top

Java: Files.exists(Path.of("a.txt"))
来源：http://byl.yvedp.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://whx.nanxinkj.top

Ruby: File.exist?("a.txt")
来源：http://muh.hywenlv.cn

C#:   File.Exists("a.txt")
来源：http://yoy.yuxming.cn

[F06] 删除文件
来源：http://ktb.shuidangran.top

Py:   os.remove("a.txt")
来源：http://ang.tianlin.xyz

PHP:  unlink("a.txt");
来源：http://glz.yueranfly.top

JS:   fs.unlinkSync("a.txt")
来源：http://kuc.zdbjq.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wjy.zhongyouzk.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ujp.yuxming.cn

Go:   os.Remove("a.txt")
来源：http://umx.zhengqikj.top

Ruby: File.delete("a.txt")
来源：http://puz.daria6918.cn

C#:   File.Delete("a.txt");
来源：http://hfv.aizwys.cn

[F07] 创建目录（含多级）
来源：http://lvg.xuetiantiany.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ubu.epnwcf.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yfm.shanyushiyangtech.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lzw.hongshengwenyu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lhp.daria6918.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kvl.jiagoushi.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gjd.zhixingplan.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xhw.zhiwuduotai.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lrz.shuidangran.top

[F08] 遍历目录
来源：http://pyy.jlsjyb.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://eke.jyoumei.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ckt.yj20258888.top

JS:   fs.readdirSync("dir")
来源：http://bsb.yonumen.top

TS:   fs.readdirSync("dir")
来源：http://ktg.jinqigfzy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jmr.aizwys.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wps.zhengqikj.top

Ruby: Dir.children("dir")
来源：http://sza.shangyingyoupin.top

C#:   Directory.GetFiles("dir")
来源：http://cag.guowangkeji.top

[F09] 获取文件大小
来源：http://tbe.ydjk.org.cn

Py:   os.path.getsize("a.txt")
来源：http://zac.yvedp.cn

PHP:  filesize("a.txt");
来源：http://kda.cdnleiting.top

JS:   fs.statSync("a.txt").size
来源：http://bve.fengsongda.top

TS:   fs.statSync("a.txt").size
来源：http://nij.snrcjt.cn

Java: Files.size(Path.of("a.txt"))
来源：http://eqi.xziqi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://anq.tarul.cn

Ruby: File.size("a.txt")
来源：http://rwy.aizwys.cn

C#:   new FileInfo("a.txt").Length
来源：http://dot.shangyingyoupin.top

[F10] 取文件扩展名 / 文件名
来源：http://hkc.yuxming.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dst.snrcjt.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pli.0kj1m.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xsk.cheryme.top

TS:   path.extname("a.txt")
来源：http://iwf.xylfe.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ibr.jyoumei.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ozu.hongshengwenyu.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mhi.birdmap.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xms.tarul.cn

[F11] 复制与移动文件
来源：http://uuo.0kj1m.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pkd.sjlbkw.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cmu.ydzc1.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jwt.gzhubu.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dwx.kuanghao11.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ozt.jinqigufen.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://roq.haohaochexian.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jag.ppjwa.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lqg.hammf.cn

[F12] CSV 读写
来源：http://zsk.yueranfly.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wml.zhaomingkeji.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qvo.zhongyouzk.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qhq.ydzc1.top

TS:   // 同上
来源：http://bnu.zhoulong.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kqx.hcnkem.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ent.jqgfzy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lgm.vehdjk.com

C#:   // 无内置：用 CsvHelper 库
来源：http://rvw.52xcode.cn

================================================================================
来源：http://xsy.zhiwuduotai.top

G. 面向对象
来源：http://wmh.nanxuanxn.top

================================================================================
来源：http://qzv.andypj.xyz

[G01] 定义类
来源：http://kyf.svipenyu.cn

Py:   class User: pass
来源：http://apc.wangshuangyany.cn

PHP:  class User {}
来源：http://igd.zhijiandao.cn

JS:   class User {}
来源：http://uyd.fanxiaobao.xyz

TS:   class User { name: string = ""; }
来源：http://usy.xylfe.cn

Java: class User {}
来源：http://xtw.zhengqikj.top

Go:   type User struct { Name string }
来源：http://hrh.316326.xyz

Ruby: class User; end
来源：http://fbm.ywan-chungtsiang.top

C#:   class User {}
来源：http://hrb.ydzc1.top

[G02] 构造函数
来源：http://vjo.gaohongyu789.top

Py:   def __init__(self, name): self.name = name
来源：http://gvo.hcnkem.com

PHP:  public function __construct(public string $name) {}
来源：http://ifh.xingfuxueyuan.xyz

JS:   constructor(name) { this.name = name; }
来源：http://kue.hfpthk.cn

TS:   constructor(public name: string) {}
来源：http://ezb.vehdjk.com

Java: User(String name) { this.name = name; }
来源：http://vfd.iojbl.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vrw.ctjpmb.com

Ruby: def initialize(name); @name = name; end
来源：http://wvq.zhixingplan.top

C#:   public User(string name) { Name = name; }
来源：http://rvx.zycfv.cn

[G03] 实例属性
来源：http://hnr.fzhhl.top

Py:   self.name = "x"
来源：http://oqw.xziqi.cn

PHP:  public string $name = "x";
来源：http://nyp.uphjek.com

JS:   this.name = "x";
来源：http://aep.hammf.cn

TS:   name: string = "x";
来源：http://dcy.shanyushiyangkeji.top

Java: private String name;
来源：http://iap.wangshuangyany.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ovs.shanyushiyangkeji.top

Ruby: @name = "x"
来源：http://fuk.gogol.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://ywf.vqdsnc.cn

[G04] 定义方法
来源：http://zja.nwbrower.top

Py:   def greet(self): return self.name
来源：http://bzi.dianchejie.cn


<!-- 参考信息 -->