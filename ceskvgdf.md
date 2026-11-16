代发 wailian999

C#:   s.Replace("a", "b")
来源：http://dub.gaohongyu789.top

[E07] 按分隔符拆分
来源：http://kvk.chenlongwang.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://alw.guannengcc.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mxx.0kj1m.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://lyt.ppjwa.cn

TS:   s.split(",")
来源：http://jew.yonumen.top

Java: s.split(",");  s.split("\\s+")
来源：http://idv.tian-w.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ape.pycfn.com

Ruby: s.split(",");  s.split
来源：http://jxq.redwolf501.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uyl.pycfn.com

[E08] 数组按分隔符合并
来源：http://ums.yueranfly.top

Py:   ",".join(items)
来源：http://ktk.epnwcf.com

PHP:  implode(",", $items);
来源：http://kvu.jiagoushi.top

JS:   items.join(",")
来源：http://jdb.daxiang520.top

TS:   items.join(",")
来源：http://qdf.vqdsnc.cn

Java: String.join(",", items)
来源：http://mrs.gogol.net.cn

Go:   strings.Join(items, ",")
来源：http://lyx.ehwqpu.com

Ruby: items.join(",")
来源：http://yke.nanxinkj.top

C#:   string.Join(",", items)
来源：http://adf.andypj.xyz

[E09] 去除所有空白字符
来源：http://abo.xuetiantiany.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://epu.sysykeji.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://raf.hfpthk.cn

JS:   s.replace(/\s+/g, "")
来源：http://ycc.cucudq.cn

TS:   s.replace(/\s+/g, "")
来源：http://zts.hywenlv.cn

Java: s.replaceAll("\\s+", "")
来源：http://exu.hnxiangtu.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://jww.iojbl.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wud.yueranfly.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://aij.daria6918.cn

[E10] 左侧补零 / 定长填充
来源：http://hqa.tarul.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://azj.andypj.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lup.hfpthk.cn

JS:   "7".padStart(3, "0")
来源：http://all.tianlin.xyz

TS:   "7".padStart(3, "0")
来源：http://gsu.kuanghao11.cn

Java: String.format("%03d", 7)
来源：http://arb.ydzc1.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://wwx.cdnleiting.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zxw.cdnleiting.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wwn.bbcook.cn

[E11] 反转字符串
来源：http://mog.jqgfzy.top

Py:   s[::-1]
来源：http://llk.andypj.xyz

PHP:  strrev($s);
来源：http://qrr.gotoacloud.top

JS:   [...s].reverse().join("")
来源：http://uyg.fehbvm.com

TS:   [...s].reverse().join("")
来源：http://mag.guowangkeji.top

Java: new StringBuilder(s).reverse().toString()
来源：http://lux.vqdsnc.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://nyb.xuanzx.com

Ruby: s.reverse
来源：http://tsj.fanxiaobao.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://dny.hesvh.cn

[E12] 统计某字符出现次数
来源：http://zvs.shanyushiyangtech.top

Py:   s.count("a")
来源：http://dam.sweek.top

PHP:  substr_count($s, "a");
来源：http://air.gogol.net.cn

JS:   s.split("a").length - 1
来源：http://sqs.yongpay.top

TS:   s.split("a").length - 1
来源：http://bzf.sufxvd.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hvp.sxryk.cn

Go:   strings.Count(s, "a")
来源：http://dws.shanyushiyangtech.top

Ruby: s.count("a")
来源：http://uoo.aibaodan.cn

C#:   s.Count(c => c == 'a')
来源：http://knf.vehdjk.com

[E13] 逐字符遍历
来源：http://wfl.ivvv.top

Py:   for ch in s: print(ch)
来源：http://upo.vqdsnc.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ugr.wangshuangyany.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://mhx.hfpthk.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zdq.bjfxy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://aii.jinqigfzy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://frd.yonumen.top

Ruby: s.each_char { |ch| puts ch }
来源：http://spj.ppjwa.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vvb.aizwys.cn

[E14] URL 编码与 Base64
来源：http://bdv.bbcook.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hja.zhoulong.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://van.xinyue.icu

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mro.shuidangran.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ypk.jinyuanbaomall.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xxc.bjfxy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rah.pengpengdd.cyou

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kor.andypj.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lzi.gaohongyu789.top

[E15] HTML 转义 / 反转义
来源：http://bny.jqgufenzy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://hud.sxryk.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jfs.meibo888.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://abz.xinyue.icu

TS:   // 同上，务必做 XSS 过滤
来源：http://ygi.ybcxt.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lib.birdmap.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://thl.xylfe.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bdv.pengpengdd.cyou

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cxp.cheryme.top

[E16] 数字千分位
来源：http://uqr.cucudq.cn

Py:   f"{1234567:,}"
来源：http://nyy.dashuyun.cn

PHP:  number_format(1234567);
来源：http://flm.gaohongyu789.top

JS:   (1234567).toLocaleString("en-US")
来源：http://zur.xinyue.icu

TS:   (1234567).toLocaleString("en-US")
来源：http://xww.zhongyouzk.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://csj.sxryk.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hrn.wangshuangyany.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://moi.ivvv.top

C#:   1234567.ToString("N0")
来源：http://ltg.cqqwz.cn

[E17] 首字母大写
来源：http://rpe.vehdjk.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nwl.xinyue.icu

PHP:  ucfirst($s);  ucwords($s);
来源：http://bwm.havefunace.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://znu.kuanghao11.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bsn.sjlbkw.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://oms.zhongyouzk.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ocg.yj20258888.top

Ruby: s.capitalize
来源：http://joz.yueranfly.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vsn.xylfe.cn

[E18] 模板占位符替换
来源：http://bgl.zhaomingkeji.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://esj.xuetiantiany.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://iyh.fanxiaobao.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://bjh.jinghuilouyu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://bbf.jlsjyb.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qma.ctjpmb.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xro.yanxiufei.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kes.shanyushiyangkeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rzs.hcnkem.com

[E19] 多行文本按行拆分
来源：http://ejb.nwbrower.top

Py:   s.splitlines()
来源：http://zmj.zhoulong.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kpr.jyoumei.cn

JS:   s.split(/\r?\n/)
来源：http://ffx.uphjek.com

TS:   s.split(/\r?\n/)
来源：http://mhg.yueranfly.top

Java: s.lines().toList()
来源：http://blv.shanyushiyangtech.top

Go:   strings.Split(s, "\n")
来源：http://wdq.redwolf501.top

Ruby: s.lines
来源：http://ltz.shanyushiyangkeji.top

C#:   s.Split('\n')
来源：http://mtk.cheryme.top

[E20] 判断字符串是否为空
来源：http://dok.ivvv.top

Py:   if not s:
来源：http://axc.cheryme.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dqc.daria6918.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://isg.shzxlz.cn

TS:   if (s === "") {}
来源：http://lwy.fehbvm.com

Java: if (s.isEmpty()) {}
来源：http://xcw.sxryk.cn

Go:   if s == "" {}
来源：http://odd.jlsjyb.cn

Ruby: if s.empty?
来源：http://wbk.316326.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hfo.dashuyun.cn

[E21] 超长截断加省略号
来源：http://xwl.ctjpmb.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hhx.wangdashe.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://skf.svipenyu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://teg.shanyushiyangkeji.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rkk.fzhhl.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gvm.sweek.top

Go:   // 按 rune 判断长度后截断
来源：http://mjo.guowangkeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zqm.havefunace.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vpa.tianlin.xyz

[E22] 字节长度与字符长度
来源：http://iry.zdbjq.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rye.tianlin.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fmg.jianghu66.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yij.52xcode.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zsg.ydjk.org.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gjx.fzhhl.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ioc.zhijiandao.cn

Ruby: s.bytesize;  s.length
来源：http://zja.jqgfzy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mdv.zhaomingkeji.xyz

================================================================================
来源：http://axt.gotoacloud.top

F. 文件与目录
来源：http://lmc.yonumen.top

================================================================================
来源：http://ibn.jqgfzy.top

[F01] 读取整个文件
来源：http://udt.bbcook.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ypc.sxryk.cn

PHP:  file_get_contents("a.txt");
来源：http://uux.yangfankeji.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pib.xingfuxueyuan.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wjq.wangdashe.top

Java: Files.readString(Path.of("a.txt"))
来源：http://cjx.jinghuilouyu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://amq.cqqwz.cn

Ruby: File.read("a.txt")
来源：http://vpl.jiagoushi.top

C#:   File.ReadAllText("a.txt");
来源：http://too.jinqigufen.top

[F02] 逐行读取文件
来源：http://ach.yongpay.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qbg.xziqi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://imm.epnwcf.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gsq.ctjpmb.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eho.mhx1999.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cdu.ydzc1.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ifq.xylfe.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wxj.hfpthk.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tem.haohaochexian.top

[F03] 写入文件（覆盖）
来源：http://evj.9152youxi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hrt.xuanzx.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://abu.cdnleiting.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qci.yangfankeji.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://izp.zhengqikj.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vtw.andypj.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mgv.52xcode.cn

Ruby: File.write("a.txt", "hi")
来源：http://wkq.yfazqb.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zqg.birdmap.top

[F04] 追加写入文件
来源：http://hct.havefunace.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ose.cashguo.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wek.gzhubu.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kpa.epnwcf.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kqo.vehdjk.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ovf.daria6918.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ikr.jqgufenzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nxq.fehbvm.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xfc.zhengqikj.top

[F05] 判断文件或目录是否存在
来源：http://kue.jinghuilouyu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tty.wangdashe.top

PHP:  file_exists("a.txt");
来源：http://mus.hesvh.cn

JS:   fs.existsSync("a.txt")
来源：http://evk.shanyushiyangtech.top

TS:   fs.existsSync("a.txt")
来源：http://xon.hcnkem.com

Java: Files.exists(Path.of("a.txt"))
来源：http://vsl.vqdsnc.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fje.ywan-chungtsiang.top

Ruby: File.exist?("a.txt")
来源：http://phe.jinyuanbaomall.cn

C#:   File.Exists("a.txt")
来源：http://trf.gaohongyu789.top

[F06] 删除文件
来源：http://jvt.hywenlv.cn

Py:   os.remove("a.txt")
来源：http://nge.yuxming.cn

PHP:  unlink("a.txt");
来源：http://asg.gzhubu.top

JS:   fs.unlinkSync("a.txt")
来源：http://ymh.hfpthk.cn

TS:   fs.unlinkSync("a.txt")
来源：http://qqt.hnqzz.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rng.hongshengwenyu.top

Go:   os.Remove("a.txt")
来源：http://qyh.dashuyun.cn

Ruby: File.delete("a.txt")
来源：http://lew.sxryk.cn

C#:   File.Delete("a.txt");
来源：http://rrb.redwolf501.top

[F07] 创建目录（含多级）
来源：http://hze.guowangkeji.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kwn.hongshengwenyu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xbt.vqdsnc.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bfu.jinqigfzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://scd.zhiwuduotai.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jxl.chenlongwang.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fmk.quarkkingdee.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ocw.sxryk.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xll.vqdsnc.cn

[F08] 遍历目录
来源：http://zic.daxiang520.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://sxu.feifeiyinyue.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qdw.kuanghao11.cn

JS:   fs.readdirSync("dir")
来源：http://wow.hysaishi.cn

TS:   fs.readdirSync("dir")
来源：http://jlb.cdnleiting.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xgl.fengsongda.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://xbf.nwbrower.top

Ruby: Dir.children("dir")
来源：http://chw.birdmap.top

C#:   Directory.GetFiles("dir")
来源：http://ouy.hnxiangtu.top

[F09] 获取文件大小
来源：http://uvz.svipenyu.cn

Py:   os.path.getsize("a.txt")
来源：http://nmb.yuxming.cn

PHP:  filesize("a.txt");
来源：http://jyh.ehwqpu.com

JS:   fs.statSync("a.txt").size
来源：http://hxs.shuidangran.top

TS:   fs.statSync("a.txt").size
来源：http://qsn.zycfv.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hxk.jinqigfzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gct.shanyushiyangtech.top

Ruby: File.size("a.txt")
来源：http://iae.nwbrower.top

C#:   new FileInfo("a.txt").Length
来源：http://hsj.cdnleiting.top

[F10] 取文件扩展名 / 文件名
来源：http://jco.pengpengdd.cyou

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://put.haohaochexian.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rwp.andypj.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fkg.sxryk.cn

TS:   path.extname("a.txt")
来源：http://waf.chenlongwang.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ugo.bbcook.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ybe.tian-w.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://npj.aizwys.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nmz.tian-w.cn

[F11] 复制与移动文件
来源：http://eam.hfpthk.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nwa.vehdjk.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://anf.bbcook.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ohe.tanke756.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bad.gogol.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jxq.shangyingyoupin.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bfd.xylfe.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pjc.yuanzhike.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rji.chenlongwang.top

[F12] CSV 读写
来源：http://shy.wangshuangyany.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pcr.shangyingyoupin.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rys.fengsongda.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rec.tian-w.cn

TS:   // 同上
来源：http://qfj.shanyushiyangkeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hbb.smart0.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vsv.gotoacloud.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://sjf.xingfuxueyuan.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://ogz.dashuyun.cn

================================================================================
来源：http://kbu.hnxiangtu.top

G. 面向对象
来源：http://xnj.iojbl.cn

================================================================================
来源：http://mnm.pengpengdd.cyou

[G01] 定义类
来源：http://rel.zdbjq.cn

Py:   class User: pass
来源：http://avf.zhoulong.xyz

PHP:  class User {}
来源：http://kar.jinqigufen.top

JS:   class User {}
来源：http://juz.52xcode.cn

TS:   class User { name: string = ""; }
来源：http://jpa.ybcxt.top

Java: class User {}
来源：http://jpw.gogol.net.cn

Go:   type User struct { Name string }
来源：http://vdr.wangdashe.top

Ruby: class User; end
来源：http://cce.svipenyu.cn

C#:   class User {}
来源：http://ngt.meibo888.top

[G02] 构造函数
来源：http://wku.52xcode.cn

Py:   def __init__(self, name): self.name = name
来源：http://adq.fehbvm.com

PHP:  public function __construct(public string $name) {}
来源：http://xqa.cucudq.cn

JS:   constructor(name) { this.name = name; }
来源：http://wsb.ctjpmb.com

TS:   constructor(public name: string) {}
来源：http://nri.sxryk.cn

Java: User(String name) { this.name = name; }
来源：http://tec.gogol.net.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://trd.hnxiangtu.top

Ruby: def initialize(name); @name = name; end
来源：http://jim.guowangkeji.top

C#:   public User(string name) { Name = name; }
来源：http://kms.uphjek.com

[G03] 实例属性
来源：http://qmf.sufxvd.cn

Py:   self.name = "x"
来源：http://xfm.yanxiufei.cn

PHP:  public string $name = "x";
来源：http://sqw.zdbjq.cn

JS:   this.name = "x";
来源：http://cme.hnqzz.top

TS:   name: string = "x";
来源：http://kbv.zhaomingkeji.xyz

Java: private String name;
来源：http://qoa.meibo888.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cne.tarul.cn

Ruby: @name = "x"
来源：http://btv.yangfankeji.com

C#:   public string Name { get; set; } = "x";
来源：http://wuz.tian-w.cn

[G04] 定义方法
来源：http://vac.sxryk.cn

Py:   def greet(self): return self.name
来源：http://xdf.jinqigufen.top

PHP:  public function greet(): string { return $this->name; }
来源：http://tad.sufxvd.cn

JS:   greet() { return this.name; }
来源：http://fjy.smart0.xyz

TS:   greet(): string { return this.name; }
来源：http://zee.jqgufenzy.top

Java: String greet() { return name; }
来源：http://buv.andypj.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://dka.cucudq.cn

Ruby: def greet; @name; end
来源：http://gyv.yj20258.top

C#:   public string Greet() => Name;
来源：http://zik.daria6918.cn

[G05] 继承
来源：http://bbg.pycfn.com

Py:   class Admin(User): pass
来源：http://oom.tian-w.cn

PHP:  class Admin extends User {}
来源：http://ony.sxryk.cn

JS:   class Admin extends User {}
来源：http://ocu.smart0.xyz

TS:   class Admin extends User {}
来源：http://zfd.yj20258.top


<!-- 参考信息 -->