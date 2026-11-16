代发 wailian999

[E06] 替换子串
来源：http://iav.ctjpmb.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ues.aizwys.cn

PHP:  str_replace("a", "b", $s);
来源：http://xol.yj20258888.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wbo.mhx1999.top

TS:   s.replaceAll("a", "b")
来源：http://btl.gogol.net.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tqf.sxryk.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hfg.ybcxt.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vjg.zhijiandao.cn

C#:   s.Replace("a", "b")
来源：http://inh.gotoacloud.top

[E07] 按分隔符拆分
来源：http://uaj.zdbjq.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rit.chenlongwang.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jec.birdmap.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://fay.ctjpmb.com

TS:   s.split(",")
来源：http://zqh.fktsv.cn

Java: s.split(",");  s.split("\\s+")
来源：http://yke.uphjek.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wxe.yongpay.top

Ruby: s.split(",");  s.split
来源：http://xgk.tarul.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zpm.gzhubu.top

[E08] 数组按分隔符合并
来源：http://rdm.yvedp.cn

Py:   ",".join(items)
来源：http://lqa.cashguo.top

PHP:  implode(",", $items);
来源：http://ivn.feifeiyinyue.top

JS:   items.join(",")
来源：http://ibw.guowangkeji.top

TS:   items.join(",")
来源：http://oup.jinghuilouyu.cn

Java: String.join(",", items)
来源：http://eoz.hfpthk.cn

Go:   strings.Join(items, ",")
来源：http://lbr.nwbrower.top

Ruby: items.join(",")
来源：http://poi.yangfankeji.com

C#:   string.Join(",", items)
来源：http://ovx.svipenyu.cn

[E09] 去除所有空白字符
来源：http://qrg.cucudq.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://apw.jinyuanbaomall.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://oqw.zycfv.cn

JS:   s.replace(/\s+/g, "")
来源：http://ufi.zhongyouzk.top

TS:   s.replace(/\s+/g, "")
来源：http://jzg.ppjwa.cn

Java: s.replaceAll("\\s+", "")
来源：http://cxv.zhaomingkeji.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://rtt.andypj.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://aei.xingfuxueyuan.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://afv.shanyushiyangtech.top

[E10] 左侧补零 / 定长填充
来源：http://czx.hcnkem.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hur.shzxlz.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ppm.yangfankeji.com

JS:   "7".padStart(3, "0")
来源：http://kpt.epnwcf.com

TS:   "7".padStart(3, "0")
来源：http://swy.mhx1999.top

Java: String.format("%03d", 7)
来源：http://oxy.hcnkem.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://aqr.jqgufenzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://awv.jinghuilouyu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tyc.fanxiaobao.xyz

[E11] 反转字符串
来源：http://zui.tian-w.cn

Py:   s[::-1]
来源：http://tha.wangdashe.top

PHP:  strrev($s);
来源：http://nfh.yanxiufei.cn

JS:   [...s].reverse().join("")
来源：http://xdb.gzhubu.top

TS:   [...s].reverse().join("")
来源：http://chp.zhijiandao.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://btk.zhijiandao.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vsq.nanxuanxn.top

Ruby: s.reverse
来源：http://vsm.hcnkem.com

C#:   new string(s.Reverse().ToArray())
来源：http://rcz.zhijiandao.cn

[E12] 统计某字符出现次数
来源：http://fmz.yongpay.top

Py:   s.count("a")
来源：http://xvh.jiagoushi.top

PHP:  substr_count($s, "a");
来源：http://xue.aizwys.cn

JS:   s.split("a").length - 1
来源：http://ypz.hfpthk.cn

TS:   s.split("a").length - 1
来源：http://lvz.havefunace.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mew.sxryk.cn

Go:   strings.Count(s, "a")
来源：http://tyi.tian-w.cn

Ruby: s.count("a")
来源：http://mde.zycfv.cn

C#:   s.Count(c => c == 'a')
来源：http://cnu.ppjwa.cn

[E13] 逐字符遍历
来源：http://ibz.c1oappe.top

Py:   for ch in s: print(ch)
来源：http://abg.hnxiangtu.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qgp.sysykeji.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://trb.jinyuanbaomall.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ysf.gzhubu.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gcq.zhijiandao.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pbt.hfpthk.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ivo.sweek.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xue.9152youxi.cn

[E14] URL 编码与 Base64
来源：http://kth.fanxiaobao.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hpv.zhijiandao.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://icx.cucudq.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jbx.sweek.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xkr.vehdjk.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://crl.yj20258888.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://las.meibo888.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ahd.hammf.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ovr.feifeiyinyue.top

[E15] HTML 转义 / 反转义
来源：http://ppx.vqdsnc.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fws.ppjwa.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hkj.fktsv.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fih.jqgufenzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://bik.gaohongyu789.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ebb.shzxlz.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mfo.sjlbkw.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pau.guannengcc.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fqm.shzxlz.cn

[E16] 数字千分位
来源：http://tej.jyoumei.cn

Py:   f"{1234567:,}"
来源：http://uke.fehbvm.com

PHP:  number_format(1234567);
来源：http://cni.gotoacloud.top

JS:   (1234567).toLocaleString("en-US")
来源：http://pdx.meibo888.top

TS:   (1234567).toLocaleString("en-US")
来源：http://khk.aizwys.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dqd.9152youxi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gea.smart0.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ypd.nwbrower.top

C#:   1234567.ToString("N0")
来源：http://kko.iojbl.cn

[E17] 首字母大写
来源：http://inq.hnqzz.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mbp.xinyue.icu

PHP:  ucfirst($s);  ucwords($s);
来源：http://dxx.sufxvd.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ljl.hfpthk.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jkc.ppjwa.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://iyk.jiagoushi.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://anl.gotoacloud.top

Ruby: s.capitalize
来源：http://nsk.hywenlv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wvw.wangshuangyany.cn

[E18] 模板占位符替换
来源：http://kol.ctjpmb.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gxa.jinqigufen.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yif.zdbjq.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://uyf.316326.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://smt.hesvh.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://etr.bbcook.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ggg.chenlongwang.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://iyy.kuanghao11.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gbu.dashuyun.cn

[E19] 多行文本按行拆分
来源：http://nep.ivvv.top

Py:   s.splitlines()
来源：http://ugl.sweek.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qud.gaohongyu789.top

JS:   s.split(/\r?\n/)
来源：http://ubn.gogol.net.cn

TS:   s.split(/\r?\n/)
来源：http://qlw.yangfankeji.com

Java: s.lines().toList()
来源：http://mzl.birdmap.top

Go:   strings.Split(s, "\n")
来源：http://ctm.ydjk.org.cn

Ruby: s.lines
来源：http://kds.yj202588.top

C#:   s.Split('\n')
来源：http://oox.yfazqb.com

[E20] 判断字符串是否为空
来源：http://tqa.cucudq.cn

Py:   if not s:
来源：http://rih.zhiwuduotai.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hkd.nwbrower.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mum.sufxvd.cn

TS:   if (s === "") {}
来源：http://lnx.zhoulong.xyz

Java: if (s.isEmpty()) {}
来源：http://vpk.bbcook.cn

Go:   if s == "" {}
来源：http://kmd.aizwys.cn

Ruby: if s.empty?
来源：http://gwh.gotoacloud.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dfm.zhongyouzk.top

[E21] 超长截断加省略号
来源：http://kbf.yj20258.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bsv.jiagoushi.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ero.gzhubu.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mwx.smart0.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://olw.jinqigfzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://swd.zhijiandao.cn

Go:   // 按 rune 判断长度后截断
来源：http://tio.guannengcc.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hqc.ydjk.org.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tmb.cashguo.top

[E22] 字节长度与字符长度
来源：http://bcm.daxiang520.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kuf.svipenyu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://clr.quarkkingdee.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bot.ivvv.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hbe.hongshengwenyu.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://afu.yj20258888.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wbt.bbcook.cn

Ruby: s.bytesize;  s.length
来源：http://bce.svipenyu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lka.xylfe.cn

================================================================================
来源：http://pzj.zhaomingkeji.xyz

F. 文件与目录
来源：http://mxn.shuidangran.top

================================================================================
来源：http://iqe.vqdsnc.cn

[F01] 读取整个文件
来源：http://ygk.zhoulong.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://svr.cashguo.top

PHP:  file_get_contents("a.txt");
来源：http://rfl.yfazqb.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rss.gzhubu.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gvm.haohaochexian.top

Java: Files.readString(Path.of("a.txt"))
来源：http://kwp.ywan-chungtsiang.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nng.gzhubu.top

Ruby: File.read("a.txt")
来源：http://xyv.cashguo.top

C#:   File.ReadAllText("a.txt");
来源：http://msh.yueranfly.top

[F02] 逐行读取文件
来源：http://mtw.hnqzz.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://sua.chenlongwang.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nmh.cashguo.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://apr.mhx1999.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://okw.zhaomingkeji.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wqw.dashuyun.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ntg.jinqigufen.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wwa.9152youxi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zho.nwbrower.top

[F03] 写入文件（覆盖）
来源：http://gkc.jinqigfzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gxx.zhaomingkeji.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://klg.cashguo.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nki.jinghuilouyu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://feo.hywenlv.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hvr.jqgufenzy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ycg.zhoulong.xyz

Ruby: File.write("a.txt", "hi")
来源：http://qze.hysaishi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bhi.jianghu66.top

[F04] 追加写入文件
来源：http://gwd.zhiwuduotai.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://izu.xinyue.icu

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ayj.smart0.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tqo.ctjpmb.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nnv.hfpthk.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zcy.pengpengdd.cyou

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://elj.wangdashe.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ywy.shanyushiyangtech.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ofr.yj20258888.top

[F05] 判断文件或目录是否存在
来源：http://zbt.bjfxy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sgs.cdnleiting.top

PHP:  file_exists("a.txt");
来源：http://ecr.jinghuilouyu.cn

JS:   fs.existsSync("a.txt")
来源：http://plz.shuidangran.top

TS:   fs.existsSync("a.txt")
来源：http://vkb.ppjwa.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dbv.zdqjudy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hlz.gotoacloud.top

Ruby: File.exist?("a.txt")
来源：http://lrd.jlsjyb.cn

C#:   File.Exists("a.txt")
来源：http://gkf.shangyingyoupin.top

[F06] 删除文件
来源：http://uuj.daria6918.cn

Py:   os.remove("a.txt")
来源：http://mth.shzxlz.cn

PHP:  unlink("a.txt");
来源：http://zga.xziqi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vpt.ydzc1.top

TS:   fs.unlinkSync("a.txt")
来源：http://vts.cqqwz.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pku.cdnleiting.top

Go:   os.Remove("a.txt")
来源：http://uxx.xziqi.cn

Ruby: File.delete("a.txt")
来源：http://fsd.epnwcf.com

C#:   File.Delete("a.txt");
来源：http://wlk.tanke756.top

[F07] 创建目录（含多级）
来源：http://fxa.zhongyouzk.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zid.mhx1999.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sad.chenlongwang.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ccr.chenjidiqi.icu

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wwz.cqqwz.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ccu.svipenyu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rub.hnxiangtu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://evp.ydjk.org.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ngq.jinqigufen.top

[F08] 遍历目录
来源：http://odp.vehdjk.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://onm.hfpthk.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ptu.meibo888.top

JS:   fs.readdirSync("dir")
来源：http://xzw.fengsongda.top

TS:   fs.readdirSync("dir")
来源：http://xlt.snrcjt.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ifu.yj20258888.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://vbz.tian-w.cn

Ruby: Dir.children("dir")
来源：http://kya.andypj.xyz

C#:   Directory.GetFiles("dir")
来源：http://ygo.yangfankeji.com

[F09] 获取文件大小
来源：http://dmd.xuanzx.com

Py:   os.path.getsize("a.txt")
来源：http://prp.shanyushiyangkeji.top

PHP:  filesize("a.txt");
来源：http://geh.yvedp.cn

JS:   fs.statSync("a.txt").size
来源：http://bpf.tarul.cn

TS:   fs.statSync("a.txt").size
来源：http://oeh.ctjpmb.com

Java: Files.size(Path.of("a.txt"))
来源：http://vio.cashguo.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qtw.jinqigfzy.top

Ruby: File.size("a.txt")
来源：http://jrq.hnqzz.top

C#:   new FileInfo("a.txt").Length
来源：http://kys.yvedp.cn

[F10] 取文件扩展名 / 文件名
来源：http://udd.jiagoushi.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rcp.xingfuxueyuan.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lod.cdnleiting.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://udp.kuanghao11.cn

TS:   path.extname("a.txt")
来源：http://udv.ydzc1.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://keb.daxiang520.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://aum.hysaishi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dug.kuanghao11.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rhd.uphjek.com

[F11] 复制与移动文件
来源：http://muo.ybcxt.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://aoa.tarul.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ucs.andypj.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://soh.feifeiyinyue.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pbv.iojbl.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://trf.hnxiangtu.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sip.yueranfly.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rgb.ydzc1.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ovd.shangyingyoupin.top

[F12] CSV 读写
来源：http://sli.redwolf501.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hgn.gotoacloud.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ebo.meibo888.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vjb.jinyuanbaomall.cn

TS:   // 同上
来源：http://ltq.jqgfzy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vue.shangyingyoupin.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ffv.feifeiyinyue.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mlq.snrcjt.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hnd.pengpengdd.cyou

================================================================================
来源：http://ool.sxryk.cn

G. 面向对象
来源：http://nsx.c1oappe.top

================================================================================
来源：http://mne.mhx1999.top

[G01] 定义类
来源：http://oda.birdmap.top

Py:   class User: pass
来源：http://hgk.birdmap.top

PHP:  class User {}
来源：http://vut.zycfv.cn

JS:   class User {}
来源：http://phv.fengsongda.top

TS:   class User { name: string = ""; }
来源：http://whe.chenjidiqi.icu

Java: class User {}
来源：http://vbe.haohaochexian.top

Go:   type User struct { Name string }
来源：http://bik.jinghuilouyu.cn

Ruby: class User; end
来源：http://lzi.havefunace.top

C#:   class User {}
来源：http://vfb.wangdashe.top

[G02] 构造函数
来源：http://vut.xuanzx.com

Py:   def __init__(self, name): self.name = name
来源：http://mov.ctjpmb.com

PHP:  public function __construct(public string $name) {}
来源：http://ssk.hnqzz.top

JS:   constructor(name) { this.name = name; }
来源：http://wzv.shuidangran.top

TS:   constructor(public name: string) {}
来源：http://wsl.ctjpmb.com

Java: User(String name) { this.name = name; }
来源：http://kxy.zhongyouzk.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qhy.yangfankeji.com

Ruby: def initialize(name); @name = name; end
来源：http://muu.daxiang520.top

C#:   public User(string name) { Name = name; }
来源：http://akj.wangdashe.top

[G03] 实例属性
来源：http://sxo.jyoumei.cn

Py:   self.name = "x"
来源：http://vji.yj20258.top

PHP:  public string $name = "x";
来源：http://pwf.wangdashe.top

JS:   this.name = "x";
来源：http://ulj.tianlin.xyz

TS:   name: string = "x";
来源：http://tqv.tanke756.top

Java: private String name;
来源：http://kzf.jyoumei.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sai.chenlongwang.top

Ruby: @name = "x"
来源：http://stf.xziqi.cn

C#:   public string Name { get; set; } = "x";
来源：http://hgi.hysaishi.cn

[G04] 定义方法
来源：http://rjv.aibaodan.cn

Py:   def greet(self): return self.name
来源：http://ltk.nwbrower.top

PHP:  public function greet(): string { return $this->name; }
来源：http://vns.guannengcc.top

JS:   greet() { return this.name; }
来源：http://shs.zdbjq.cn

TS:   greet(): string { return this.name; }
来源：http://bnp.nwbrower.top

Java: String greet() { return name; }
来源：http://vye.cucudq.cn


<!-- 参考信息 -->