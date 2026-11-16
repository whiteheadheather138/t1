代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jyn.hongshengwenyu.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dhb.chenzaomai.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mme.cucudq.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ddw.zycfv.cn

[E06] 替换子串
来源：http://ktt.jiagoushi.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://twd.fzhhl.top

PHP:  str_replace("a", "b", $s);
来源：http://war.fzhhl.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pno.tianlin.xyz

TS:   s.replaceAll("a", "b")
来源：http://oxs.zdqjudy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tbj.hywenlv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sgq.cheryme.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cnp.yj20258.top

C#:   s.Replace("a", "b")
来源：http://iji.hongshengwenyu.top

[E07] 按分隔符拆分
来源：http://rth.pycfn.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jvv.vqdsnc.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://aek.meibo888.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://niy.jianghu66.top

TS:   s.split(",")
来源：http://nla.iojbl.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mlq.aibaodan.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://eoq.tanke756.top

Ruby: s.split(",");  s.split
来源：http://jew.xingfuxueyuan.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sva.tanke756.top

[E08] 数组按分隔符合并
来源：http://smp.ivvv.top

Py:   ",".join(items)
来源：http://pmh.redwolf501.top

PHP:  implode(",", $items);
来源：http://esg.tarul.cn

JS:   items.join(",")
来源：http://lsr.zhengqikj.top

TS:   items.join(",")
来源：http://upk.fehbvm.com

Java: String.join(",", items)
来源：http://nyv.yonumen.top

Go:   strings.Join(items, ",")
来源：http://rqg.fanxiaobao.xyz

Ruby: items.join(",")
来源：http://yrx.zdqjudy.top

C#:   string.Join(",", items)
来源：http://guf.pycfn.com

[E09] 去除所有空白字符
来源：http://wqf.hnqzz.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sxc.daria6918.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jnl.snrcjt.cn

JS:   s.replace(/\s+/g, "")
来源：http://oda.yanxiufei.cn

TS:   s.replace(/\s+/g, "")
来源：http://fdz.pengpengdd.cyou

Java: s.replaceAll("\\s+", "")
来源：http://oar.yj202588.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://dqq.hysaishi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://agw.pengpengdd.cyou

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gsn.birdmap.top

[E10] 左侧补零 / 定长填充
来源：http://jqn.ydzc1.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cle.shangyingyoupin.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dtt.jqgufenzy.top

JS:   "7".padStart(3, "0")
来源：http://pwv.tanke756.top

TS:   "7".padStart(3, "0")
来源：http://bcj.chenjidiqi.icu

Java: String.format("%03d", 7)
来源：http://aea.chenjidiqi.icu

Go:   fmt.Sprintf("%03d", 7)
来源：http://avg.zdbjq.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pkm.hywenlv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ycy.aizwys.cn

[E11] 反转字符串
来源：http://fnj.tianlin.xyz

Py:   s[::-1]
来源：http://ctv.xinyue.icu

PHP:  strrev($s);
来源：http://qbe.cucudq.cn

JS:   [...s].reverse().join("")
来源：http://pxm.snrcjt.cn

TS:   [...s].reverse().join("")
来源：http://bba.mhx1999.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ivd.sweek.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://tsb.chenlongwang.top

Ruby: s.reverse
来源：http://bge.cucudq.cn

C#:   new string(s.Reverse().ToArray())
来源：http://oxg.jqgufenzy.top

[E12] 统计某字符出现次数
来源：http://zrq.zhixingplan.top

Py:   s.count("a")
来源：http://qjw.meibo888.top

PHP:  substr_count($s, "a");
来源：http://sgd.cdnleiting.top

JS:   s.split("a").length - 1
来源：http://ayj.gaohongyu789.top

TS:   s.split("a").length - 1
来源：http://qmk.jinyuanbaomall.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pjx.gaohongyu789.top

Go:   strings.Count(s, "a")
来源：http://qpd.cucudq.cn

Ruby: s.count("a")
来源：http://vuk.xuetiantiany.cn

C#:   s.Count(c => c == 'a')
来源：http://lyn.cqqwz.cn

[E13] 逐字符遍历
来源：http://aac.dianchejie.cn

Py:   for ch in s: print(ch)
来源：http://odr.sufxvd.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hum.52xcode.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rsu.smart0.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://mpm.yuxming.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bmp.yuanzhike.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://oxn.zhixingplan.top

Ruby: s.each_char { |ch| puts ch }
来源：http://omo.jinqigufen.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://smi.xinyue.icu

[E14] URL 编码与 Base64
来源：http://dhd.chenlongwang.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ghb.daria6918.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://blj.chenjidiqi.icu

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ezz.wangshuangyany.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://coc.ehwqpu.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://few.havefunace.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kwi.shanyushiyangkeji.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bca.xylfe.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fhx.jinqigfzy.top

[E15] HTML 转义 / 反转义
来源：http://gpd.0kj1m.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ydd.iojbl.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bqc.haohaochexian.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ntj.birdmap.top

TS:   // 同上，务必做 XSS 过滤
来源：http://tpy.tanke756.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hta.birdmap.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ibb.smart0.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://csr.gogol.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tsl.sufxvd.cn

[E16] 数字千分位
来源：http://bdl.guowangkeji.top

Py:   f"{1234567:,}"
来源：http://xfi.tianlin.xyz

PHP:  number_format(1234567);
来源：http://zzv.0kj1m.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fyn.fanxiaobao.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://nct.aizwys.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zsu.zhixingplan.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bgm.cqqwz.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tmj.hfpthk.cn

C#:   1234567.ToString("N0")
来源：http://xjh.fktsv.cn

[E17] 首字母大写
来源：http://fkq.ydjk.org.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mua.ctjpmb.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://rrc.gzhubu.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xqu.feifeiyinyue.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eyh.tianlin.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://amk.cheryme.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uox.tianlin.xyz

Ruby: s.capitalize
来源：http://hgw.tarul.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sbk.zhengqikj.top

[E18] 模板占位符替换
来源：http://vyi.52xcode.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fxk.hfpthk.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mxf.yanxiufei.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://pks.andypj.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://bax.sxryk.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wli.shanyushiyangtech.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://uny.hesvh.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uhw.zhongyouzk.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rqf.ivvv.top

[E19] 多行文本按行拆分
来源：http://yqx.pengpengdd.cyou

Py:   s.splitlines()
来源：http://vxs.nwbrower.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gbq.jinqigufen.top

JS:   s.split(/\r?\n/)
来源：http://zfx.uphjek.com

TS:   s.split(/\r?\n/)
来源：http://lfs.gzhubu.top

Java: s.lines().toList()
来源：http://zbz.yueranfly.top

Go:   strings.Split(s, "\n")
来源：http://fib.ivvv.top

Ruby: s.lines
来源：http://saj.yonumen.top

C#:   s.Split('\n')
来源：http://moq.zdqjudy.top

[E20] 判断字符串是否为空
来源：http://tbp.tian-w.cn

Py:   if not s:
来源：http://hzj.sysykeji.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zwe.hysaishi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ent.xuetiantiany.cn

TS:   if (s === "") {}
来源：http://dqp.gogol.net.cn

Java: if (s.isEmpty()) {}
来源：http://atq.ivvv.top

Go:   if s == "" {}
来源：http://ayz.zdqjudy.top

Ruby: if s.empty?
来源：http://fyn.hongshengwenyu.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mht.cheryme.top

[E21] 超长截断加省略号
来源：http://grm.hcnkem.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wbp.wangdashe.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://uvq.bbcook.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yef.xinyue.icu

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vav.sysykeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cbb.havefunace.top

Go:   // 按 rune 判断长度后截断
来源：http://quo.ppjwa.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kdm.nanxinkj.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hto.yj20258.top

[E22] 字节长度与字符长度
来源：http://vqk.hysaishi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mul.uphjek.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://emk.cdnleiting.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://brb.shzxlz.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hyu.yanxiufei.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cqd.shuidangran.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://aou.zdqjudy.top

Ruby: s.bytesize;  s.length
来源：http://pmt.wangshuangyany.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fpb.gogol.net.cn

================================================================================
来源：http://ovl.andypj.xyz

F. 文件与目录
来源：http://uhh.sjlbkw.cn

================================================================================
来源：http://ibi.nanxuanxn.top

[F01] 读取整个文件
来源：http://gkn.chenzaomai.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qnm.jiagoushi.top

PHP:  file_get_contents("a.txt");
来源：http://phk.jyoumei.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xcr.wangshuangyany.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mlc.quarkkingdee.top

Java: Files.readString(Path.of("a.txt"))
来源：http://rqd.gogol.net.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hzq.epnwcf.com

Ruby: File.read("a.txt")
来源：http://xuq.zhixingplan.top

C#:   File.ReadAllText("a.txt");
来源：http://yag.sweek.top

[F02] 逐行读取文件
来源：http://kyj.wangshuangyany.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xmk.zhijiandao.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xfp.cheryme.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gnu.dashuyun.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gqm.wangdashe.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ljr.smart0.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vbf.birdmap.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://aac.sysykeji.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://git.ybcxt.top

[F03] 写入文件（覆盖）
来源：http://mxw.c1oappe.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://llv.gogol.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://czs.cqqwz.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vok.jinqigufen.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wov.sufxvd.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ici.bjfxy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://izb.sweek.top

Ruby: File.write("a.txt", "hi")
来源：http://wqd.fanxiaobao.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://aix.shanyushiyangkeji.top

[F04] 追加写入文件
来源：http://bcv.aizwys.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://psy.chenjidiqi.icu

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hys.xinyue.icu

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wev.tianlin.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bxa.yuxming.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wlo.jianghu66.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tqf.cashguo.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://eqh.vqdsnc.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gki.xuetiantiany.cn

[F05] 判断文件或目录是否存在
来源：http://lkf.zhixingplan.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fup.pycfn.com

PHP:  file_exists("a.txt");
来源：http://qpi.havefunace.top

JS:   fs.existsSync("a.txt")
来源：http://dlv.nanxuanxn.top

TS:   fs.existsSync("a.txt")
来源：http://ees.gotoacloud.top

Java: Files.exists(Path.of("a.txt"))
来源：http://hmh.uphjek.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xkn.yj20258888.top

Ruby: File.exist?("a.txt")
来源：http://zgp.mhx1999.top

C#:   File.Exists("a.txt")
来源：http://qem.dashuyun.cn

[F06] 删除文件
来源：http://mua.vehdjk.com

Py:   os.remove("a.txt")
来源：http://wgd.aizwys.cn

PHP:  unlink("a.txt");
来源：http://khq.ehwqpu.com

JS:   fs.unlinkSync("a.txt")
来源：http://ufm.ehwqpu.com

TS:   fs.unlinkSync("a.txt")
来源：http://nuv.wangshuangyany.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yao.kuanghao11.cn

Go:   os.Remove("a.txt")
来源：http://zkd.xziqi.cn

Ruby: File.delete("a.txt")
来源：http://shs.xingfuxueyuan.xyz

C#:   File.Delete("a.txt");
来源：http://xcg.zhoulong.xyz

[F07] 创建目录（含多级）
来源：http://soo.sjlbkw.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wrd.cashguo.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hrv.316326.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ymo.gogol.net.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pue.jinqigfzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ahy.hywenlv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fyg.sjlbkw.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://afw.9152youxi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ezh.zdqjudy.top

[F08] 遍历目录
来源：http://rpk.smart0.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://uoy.yfazqb.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bpz.sweek.top

JS:   fs.readdirSync("dir")
来源：http://vrz.zhixingplan.top

TS:   fs.readdirSync("dir")
来源：http://ozz.ydjk.org.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qvv.cheryme.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://mgi.sxryk.cn

Ruby: Dir.children("dir")
来源：http://ldy.ywan-chungtsiang.top

C#:   Directory.GetFiles("dir")
来源：http://ixf.gaohongyu789.top

[F09] 获取文件大小
来源：http://bik.yangfankeji.com

Py:   os.path.getsize("a.txt")
来源：http://gol.hcnkem.com

PHP:  filesize("a.txt");
来源：http://heo.ctjpmb.com

JS:   fs.statSync("a.txt").size
来源：http://nad.chenzaomai.com

TS:   fs.statSync("a.txt").size
来源：http://znn.hammf.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vgu.pengpengdd.cyou

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pig.daria6918.cn

Ruby: File.size("a.txt")
来源：http://sdv.xinyue.icu

C#:   new FileInfo("a.txt").Length
来源：http://uii.ivvv.top

[F10] 取文件扩展名 / 文件名
来源：http://zfm.xziqi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lzg.nanxinkj.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pjo.fzhhl.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://npt.cheryme.top

TS:   path.extname("a.txt")
来源：http://nih.chenlongwang.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ofx.hfpthk.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://crb.xuetiantiany.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lad.gzhubu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wok.ehwqpu.com

[F11] 复制与移动文件
来源：http://upf.chenlongwang.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ihh.jiagoushi.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ooz.hnqzz.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xdk.sweek.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fzj.svipenyu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sbm.zdbjq.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ztf.316326.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rof.hnxiangtu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qyv.cdnleiting.top

[F12] CSV 读写
来源：http://pfs.hongshengwenyu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://oyi.jinghuilouyu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qdg.pycfn.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bnw.zhoulong.xyz

TS:   // 同上
来源：http://crn.hnqzz.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://iiw.sweek.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://snu.hcnkem.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://upk.bjfxy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://qcw.dashuyun.cn

================================================================================
来源：http://oct.aizwys.cn

G. 面向对象
来源：http://qdj.ppjwa.cn

================================================================================
来源：http://zqe.zhoulong.xyz

[G01] 定义类
来源：http://pzq.cdnleiting.top

Py:   class User: pass
来源：http://rsh.snrcjt.cn

PHP:  class User {}
来源：http://llm.hnqzz.top

JS:   class User {}
来源：http://cuz.hammf.cn

TS:   class User { name: string = ""; }
来源：http://jlt.dianchejie.cn

Java: class User {}
来源：http://glg.jlsjyb.cn

Go:   type User struct { Name string }
来源：http://kii.52xcode.cn

Ruby: class User; end
来源：http://fhu.fktsv.cn

C#:   class User {}
来源：http://biq.xingfuxueyuan.xyz

[G02] 构造函数
来源：http://ser.zhixingplan.top

Py:   def __init__(self, name): self.name = name
来源：http://eoo.0kj1m.cn

PHP:  public function __construct(public string $name) {}
来源：http://xpj.aibaodan.cn

JS:   constructor(name) { this.name = name; }
来源：http://dxk.ydzc1.top

TS:   constructor(public name: string) {}
来源：http://uid.gaohongyu789.top

Java: User(String name) { this.name = name; }
来源：http://qjr.9152youxi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://duu.ywan-chungtsiang.top

Ruby: def initialize(name); @name = name; end
来源：http://ccx.snrcjt.cn

C#:   public User(string name) { Name = name; }
来源：http://juz.9152youxi.cn

[G03] 实例属性
来源：http://gdl.cucudq.cn

Py:   self.name = "x"
来源：http://nzp.quarkkingdee.top

PHP:  public string $name = "x";
来源：http://ttm.chenzaomai.com

JS:   this.name = "x";
来源：http://mnv.zhixingplan.top

TS:   name: string = "x";
来源：http://wwu.52xcode.cn

Java: private String name;
来源：http://sra.pengpengdd.cyou

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://exp.gotoacloud.top

Ruby: @name = "x"
来源：http://occ.jyoumei.cn

C#:   public string Name { get; set; } = "x";
来源：http://qqd.zhixingplan.top

[G04] 定义方法
来源：http://pve.sxryk.cn

Py:   def greet(self): return self.name
来源：http://emn.cheryme.top


<!-- 参考信息 -->