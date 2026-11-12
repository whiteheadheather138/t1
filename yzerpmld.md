代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://fix.feifeiyinyue.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dyw.hnxiangtu.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sgb.cucudq.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fnf.hesvh.cn

C#:   s.Replace("a", "b")
来源：http://uyc.kuanghao11.cn

[E07] 按分隔符拆分
来源：http://mao.zhengqikj.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sfe.ywan-chungtsiang.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kgi.smart0.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://coq.tanke756.top

TS:   s.split(",")
来源：http://tuj.havefunace.top

Java: s.split(",");  s.split("\\s+")
来源：http://sau.yj20258.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://utp.cheryme.top

Ruby: s.split(",");  s.split
来源：http://ppl.hysaishi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gyi.hywenlv.cn

[E08] 数组按分隔符合并
来源：http://yfs.chenlongwang.top

Py:   ",".join(items)
来源：http://gjc.pycfn.com

PHP:  implode(",", $items);
来源：http://xnp.hysaishi.cn

JS:   items.join(",")
来源：http://bga.ctjpmb.com

TS:   items.join(",")
来源：http://wao.daria6918.cn

Java: String.join(",", items)
来源：http://ank.smart0.xyz

Go:   strings.Join(items, ",")
来源：http://qql.fanxiaobao.xyz

Ruby: items.join(",")
来源：http://uoz.bbcook.cn

C#:   string.Join(",", items)
来源：http://isd.316326.xyz

[E09] 去除所有空白字符
来源：http://fxc.bjfxy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fum.ywan-chungtsiang.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://orq.jinghuilouyu.cn

JS:   s.replace(/\s+/g, "")
来源：http://tdm.ydzc1.top

TS:   s.replace(/\s+/g, "")
来源：http://vla.zhaomingkeji.xyz

Java: s.replaceAll("\\s+", "")
来源：http://ncw.dashuyun.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ntn.guannengcc.top

Ruby: s.gsub(/\s+/, "")
来源：http://yif.aibaodan.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ckw.hcnkem.com

[E10] 左侧补零 / 定长填充
来源：http://dqa.tanke756.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jwo.xuetiantiany.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nkk.jianghu66.top

JS:   "7".padStart(3, "0")
来源：http://zya.52xcode.cn

TS:   "7".padStart(3, "0")
来源：http://jie.quarkkingdee.top

Java: String.format("%03d", 7)
来源：http://nqn.xuanzx.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://ivu.vqdsnc.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lgw.zhijiandao.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vrx.shanyushiyangtech.top

[E11] 反转字符串
来源：http://jmx.dashuyun.cn

Py:   s[::-1]
来源：http://yby.birdmap.top

PHP:  strrev($s);
来源：http://ekb.ivvv.top

JS:   [...s].reverse().join("")
来源：http://iqf.shzxlz.cn

TS:   [...s].reverse().join("")
来源：http://hfp.cheryme.top

Java: new StringBuilder(s).reverse().toString()
来源：http://akn.shzxlz.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qig.hywenlv.cn

Ruby: s.reverse
来源：http://yaj.wangshuangyany.cn

C#:   new string(s.Reverse().ToArray())
来源：http://saw.zycfv.cn

[E12] 统计某字符出现次数
来源：http://vgg.wangdashe.top

Py:   s.count("a")
来源：http://lst.sweek.top

PHP:  substr_count($s, "a");
来源：http://pcj.shzxlz.cn

JS:   s.split("a").length - 1
来源：http://bxi.vqdsnc.cn

TS:   s.split("a").length - 1
来源：http://pcd.0kj1m.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vuq.hammf.cn

Go:   strings.Count(s, "a")
来源：http://zej.daxiang520.top

Ruby: s.count("a")
来源：http://kcg.zhengqikj.top

C#:   s.Count(c => c == 'a')
来源：http://igl.shzxlz.cn

[E13] 逐字符遍历
来源：http://zsj.cucudq.cn

Py:   for ch in s: print(ch)
来源：http://knk.pengpengdd.cyou

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gtv.xingfuxueyuan.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://cyt.guowangkeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://jhi.ywan-chungtsiang.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bnz.fengsongda.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://msb.yanxiufei.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://eui.xinyue.icu

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xad.yj20258.top

[E14] URL 编码与 Base64
来源：http://okd.yj20258888.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://whn.zhijiandao.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://gjx.chenlongwang.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mav.svipenyu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fik.c1oappe.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uic.zhongyouzk.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cey.shanyushiyangtech.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cpj.yuxming.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qbi.aizwys.cn

[E15] HTML 转义 / 反转义
来源：http://xla.yfazqb.com

Py:   html.escape(s);  html.unescape(s)
来源：http://jvs.jqgufenzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://aqr.sysykeji.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://grs.hywenlv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://woz.tianlin.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nxo.bjfxy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fkm.gzhubu.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qxm.fanxiaobao.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://juc.uphjek.com

[E16] 数字千分位
来源：http://mwr.xziqi.cn

Py:   f"{1234567:,}"
来源：http://fwv.cheryme.top

PHP:  number_format(1234567);
来源：http://cjd.jinyuanbaomall.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wyf.jiagoushi.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ffe.jinqigufen.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xdx.jinqigufen.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://heb.nwbrower.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ahv.feifeiyinyue.top

C#:   1234567.ToString("N0")
来源：http://ktk.hammf.cn

[E17] 首字母大写
来源：http://kql.yanxiufei.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kqi.sysykeji.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ffi.0kj1m.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sxu.cucudq.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nbh.fengsongda.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mah.meibo888.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vkd.gzhubu.top

Ruby: s.capitalize
来源：http://oum.quarkkingdee.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jgz.svipenyu.cn

[E18] 模板占位符替换
来源：http://fbv.tianlin.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://unv.zhiwuduotai.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ttw.zhijiandao.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jea.316326.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://vkx.zhijiandao.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ydw.shanyushiyangtech.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ang.iojbl.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zrw.xuanzx.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rcl.daria6918.cn

[E19] 多行文本按行拆分
来源：http://dkk.mhx1999.top

Py:   s.splitlines()
来源：http://ytz.ppjwa.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vbb.aizwys.cn

JS:   s.split(/\r?\n/)
来源：http://dwm.guannengcc.top

TS:   s.split(/\r?\n/)
来源：http://svj.ctjpmb.com

Java: s.lines().toList()
来源：http://ftu.chenlongwang.top

Go:   strings.Split(s, "\n")
来源：http://vxn.svipenyu.cn

Ruby: s.lines
来源：http://kzl.zhijiandao.cn

C#:   s.Split('\n')
来源：http://phz.tarul.cn

[E20] 判断字符串是否为空
来源：http://njs.zycfv.cn

Py:   if not s:
来源：http://ylu.c1oappe.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://exs.nwbrower.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pea.cashguo.top

TS:   if (s === "") {}
来源：http://cde.nwbrower.top

Java: if (s.isEmpty()) {}
来源：http://gqu.xuetiantiany.cn

Go:   if s == "" {}
来源：http://diu.zdqjudy.top

Ruby: if s.empty?
来源：http://yqv.daria6918.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mwa.jinyuanbaomall.cn

[E21] 超长截断加省略号
来源：http://ckt.tian-w.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bww.fehbvm.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lkj.zhixingplan.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mba.vqdsnc.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mlm.yueranfly.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pwo.hongshengwenyu.top

Go:   // 按 rune 判断长度后截断
来源：http://arc.jinqigufen.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wnz.cdnleiting.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jqu.yuxming.cn

[E22] 字节长度与字符长度
来源：http://ckt.iojbl.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kaz.52xcode.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pjx.daxiang520.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://deo.ybcxt.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bla.guowangkeji.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xca.svipenyu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wdt.xziqi.cn

Ruby: s.bytesize;  s.length
来源：http://ixk.gotoacloud.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dgu.52xcode.cn

================================================================================
来源：http://icq.sjlbkw.cn

F. 文件与目录
来源：http://qnq.birdmap.top

================================================================================
来源：http://mqw.smart0.xyz

[F01] 读取整个文件
来源：http://afb.hnqzz.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gpr.gzhubu.top

PHP:  file_get_contents("a.txt");
来源：http://ahy.vqdsnc.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hcv.bjfxy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kbd.quarkkingdee.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ntd.tianlin.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cws.shanyushiyangkeji.top

Ruby: File.read("a.txt")
来源：http://qhy.hammf.cn

C#:   File.ReadAllText("a.txt");
来源：http://byn.ppjwa.cn

[F02] 逐行读取文件
来源：http://pkd.yj20258888.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kxb.9152youxi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://euu.zhiwuduotai.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sno.xziqi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aqc.jianghu66.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hmx.jlsjyb.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://uqy.zhijiandao.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://but.yongpay.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hmi.zhiwuduotai.top

[F03] 写入文件（覆盖）
来源：http://vgr.yongpay.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gkz.sjlbkw.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fjg.tanke756.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://buf.tianlin.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zqw.ywan-chungtsiang.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tpd.yongpay.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ozv.pycfn.com

Ruby: File.write("a.txt", "hi")
来源：http://ove.tarul.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fbt.tarul.cn

[F04] 追加写入文件
来源：http://ysf.jlsjyb.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hbw.ppjwa.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://inl.ywan-chungtsiang.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eds.jlsjyb.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rhc.fktsv.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zzh.nanxuanxn.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dym.fktsv.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cjf.daxiang520.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lsj.bbcook.cn

[F05] 判断文件或目录是否存在
来源：http://agi.nwbrower.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://axv.dashuyun.cn

PHP:  file_exists("a.txt");
来源：http://gac.jinyuanbaomall.cn

JS:   fs.existsSync("a.txt")
来源：http://tch.sjlbkw.cn

TS:   fs.existsSync("a.txt")
来源：http://ywz.fengsongda.top

Java: Files.exists(Path.of("a.txt"))
来源：http://lwq.jinqigufen.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uhc.hfpthk.cn

Ruby: File.exist?("a.txt")
来源：http://jdv.chenlongwang.top

C#:   File.Exists("a.txt")
来源：http://haz.yangfankeji.com

[F06] 删除文件
来源：http://udm.zhaomingkeji.xyz

Py:   os.remove("a.txt")
来源：http://lvv.sjlbkw.cn

PHP:  unlink("a.txt");
来源：http://zai.fktsv.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jjp.dashuyun.cn

TS:   fs.unlinkSync("a.txt")
来源：http://jtn.jinqigufen.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fiy.hnxiangtu.top

Go:   os.Remove("a.txt")
来源：http://nzz.xinyue.icu

Ruby: File.delete("a.txt")
来源：http://bwq.fehbvm.com

C#:   File.Delete("a.txt");
来源：http://lcd.yanxiufei.cn

[F07] 创建目录（含多级）
来源：http://hwu.fengsongda.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://oiu.jianghu66.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ass.shanyushiyangtech.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ins.haohaochexian.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://brv.zhiwuduotai.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vrw.svipenyu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://apz.xingfuxueyuan.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lnj.ywan-chungtsiang.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ubt.sufxvd.cn

[F08] 遍历目录
来源：http://oad.yj202588.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://xyg.cdnleiting.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://btr.nanxinkj.top

JS:   fs.readdirSync("dir")
来源：http://nvh.yfazqb.com

TS:   fs.readdirSync("dir")
来源：http://ycv.ppjwa.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ljk.hammf.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jkx.9152youxi.cn

Ruby: Dir.children("dir")
来源：http://oxz.hnqzz.top

C#:   Directory.GetFiles("dir")
来源：http://hna.gaohongyu789.top

[F09] 获取文件大小
来源：http://pqt.nanxuanxn.top

Py:   os.path.getsize("a.txt")
来源：http://jng.iojbl.cn

PHP:  filesize("a.txt");
来源：http://vjs.hongshengwenyu.top

JS:   fs.statSync("a.txt").size
来源：http://wdd.pycfn.com

TS:   fs.statSync("a.txt").size
来源：http://agk.shanyushiyangtech.top

Java: Files.size(Path.of("a.txt"))
来源：http://vkq.yuanzhike.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wmk.ivvv.top

Ruby: File.size("a.txt")
来源：http://jgn.xinyue.icu

C#:   new FileInfo("a.txt").Length
来源：http://cfm.havefunace.top

[F10] 取文件扩展名 / 文件名
来源：http://udn.yongpay.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hfx.gogol.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wuk.yueranfly.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mfh.cqqwz.cn

TS:   path.extname("a.txt")
来源：http://zhq.jlsjyb.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://aqy.ydjk.org.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cke.wangshuangyany.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hjl.yonumen.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zvh.aizwys.cn

[F11] 复制与移动文件
来源：http://buk.dashuyun.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pij.cheryme.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xnz.epnwcf.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kui.birdmap.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fbd.bjfxy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ahs.yangfankeji.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jyp.jinqigfzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wyn.pycfn.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ooe.sweek.top

[F12] CSV 读写
来源：http://ddi.snrcjt.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kou.aizwys.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mwg.shanyushiyangkeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ftm.zycfv.cn

TS:   // 同上
来源：http://axc.bjfxy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qtg.0kj1m.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ymq.fzhhl.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tbo.jinyuanbaomall.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qar.yj20258888.top

================================================================================
来源：http://rlx.ydzc1.top

G. 面向对象
来源：http://mhb.ivvv.top

================================================================================
来源：http://vgn.hesvh.cn

[G01] 定义类
来源：http://qps.meibo888.top

Py:   class User: pass
来源：http://buj.hesvh.cn

PHP:  class User {}
来源：http://ovm.sweek.top

JS:   class User {}
来源：http://sjx.kuanghao11.cn

TS:   class User { name: string = ""; }
来源：http://aox.xziqi.cn

Java: class User {}
来源：http://uzd.yfazqb.com

Go:   type User struct { Name string }
来源：http://eyk.shangyingyoupin.top

Ruby: class User; end
来源：http://yyg.jyoumei.cn

C#:   class User {}
来源：http://pep.gotoacloud.top

[G02] 构造函数
来源：http://lft.nwbrower.top

Py:   def __init__(self, name): self.name = name
来源：http://phg.snrcjt.cn

PHP:  public function __construct(public string $name) {}
来源：http://cxq.pengpengdd.cyou

JS:   constructor(name) { this.name = name; }
来源：http://xty.daria6918.cn

TS:   constructor(public name: string) {}
来源：http://tpv.tanke756.top

Java: User(String name) { this.name = name; }
来源：http://rgr.smart0.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zre.jinqigufen.top

Ruby: def initialize(name); @name = name; end
来源：http://bwc.uphjek.com

C#:   public User(string name) { Name = name; }
来源：http://yej.aizwys.cn

[G03] 实例属性
来源：http://mek.wangshuangyany.cn

Py:   self.name = "x"
来源：http://aom.shuidangran.top

PHP:  public string $name = "x";
来源：http://lnr.yangfankeji.com

JS:   this.name = "x";
来源：http://kze.yj202588.top

TS:   name: string = "x";
来源：http://cjs.jinqigfzy.top

Java: private String name;
来源：http://uln.tianlin.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yoh.sweek.top

Ruby: @name = "x"
来源：http://ind.cqqwz.cn

C#:   public string Name { get; set; } = "x";
来源：http://ved.hnqzz.top

[G04] 定义方法
来源：http://smk.hcnkem.com

Py:   def greet(self): return self.name
来源：http://nbz.gzhubu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://fcy.gaohongyu789.top

JS:   greet() { return this.name; }
来源：http://jgr.hongshengwenyu.top

TS:   greet(): string { return this.name; }
来源：http://wzg.sysykeji.top

Java: String greet() { return name; }
来源：http://wpu.hnxiangtu.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://vgs.gotoacloud.top

Ruby: def greet; @name; end
来源：http://bdd.andypj.xyz

C#:   public string Greet() => Name;
来源：http://jez.yanxiufei.cn

[G05] 继承
来源：http://dmf.xuanzx.com


<!-- 参考信息 -->