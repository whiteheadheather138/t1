代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://hwa.snrcjt.cn

TS:   s.split(",")
来源：http://azo.gogol.net.cn

Java: s.split(",");  s.split("\\s+")
来源：http://hmk.nanxuanxn.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ago.cqqwz.cn

Ruby: s.split(",");  s.split
来源：http://yhn.sweek.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ouw.shangyingyoupin.top

[E08] 数组按分隔符合并
来源：http://qds.cdnleiting.top

Py:   ",".join(items)
来源：http://qmz.hongshengwenyu.top

PHP:  implode(",", $items);
来源：http://brx.tanke756.top

JS:   items.join(",")
来源：http://hit.cashguo.top

TS:   items.join(",")
来源：http://qki.ywan-chungtsiang.top

Java: String.join(",", items)
来源：http://bab.fehbvm.com

Go:   strings.Join(items, ",")
来源：http://dxc.hfpthk.cn

Ruby: items.join(",")
来源：http://dsr.pycfn.com

C#:   string.Join(",", items)
来源：http://vul.jyoumei.cn

[E09] 去除所有空白字符
来源：http://eux.yonumen.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cvt.yuanzhike.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bon.jinqigfzy.top

JS:   s.replace(/\s+/g, "")
来源：http://pxp.meibo888.top

TS:   s.replace(/\s+/g, "")
来源：http://hvi.ppjwa.cn

Java: s.replaceAll("\\s+", "")
来源：http://umn.bjfxy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://yyd.ydjk.org.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ptk.quarkkingdee.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kuc.pycfn.com

[E10] 左侧补零 / 定长填充
来源：http://squ.guannengcc.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jbu.havefunace.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fuc.316326.xyz

JS:   "7".padStart(3, "0")
来源：http://qoc.jinyuanbaomall.cn

TS:   "7".padStart(3, "0")
来源：http://hdm.zhengqikj.top

Java: String.format("%03d", 7)
来源：http://rcr.yuxming.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://cbo.quarkkingdee.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://txc.haohaochexian.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mvw.ivvv.top

[E11] 反转字符串
来源：http://eci.hfpthk.cn

Py:   s[::-1]
来源：http://rup.nanxuanxn.top

PHP:  strrev($s);
来源：http://hzu.tian-w.cn

JS:   [...s].reverse().join("")
来源：http://qru.smart0.xyz

TS:   [...s].reverse().join("")
来源：http://bsk.quarkkingdee.top

Java: new StringBuilder(s).reverse().toString()
来源：http://kay.xuanzx.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://gll.chenlongwang.top

Ruby: s.reverse
来源：http://mhp.guowangkeji.top

C#:   new string(s.Reverse().ToArray())
来源：http://sxc.aizwys.cn

[E12] 统计某字符出现次数
来源：http://zlg.yanxiufei.cn

Py:   s.count("a")
来源：http://prt.hesvh.cn

PHP:  substr_count($s, "a");
来源：http://szl.fktsv.cn

JS:   s.split("a").length - 1
来源：http://wtp.yvedp.cn

TS:   s.split("a").length - 1
来源：http://mss.jiagoushi.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tkf.jinghuilouyu.cn

Go:   strings.Count(s, "a")
来源：http://ikw.hysaishi.cn

Ruby: s.count("a")
来源：http://vos.cheryme.top

C#:   s.Count(c => c == 'a')
来源：http://cef.tian-w.cn

[E13] 逐字符遍历
来源：http://vfi.hammf.cn

Py:   for ch in s: print(ch)
来源：http://hbw.vqdsnc.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jmp.dianchejie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xtd.pycfn.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://irm.hammf.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rlm.wangshuangyany.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://alz.fzhhl.top

Ruby: s.each_char { |ch| puts ch }
来源：http://pqm.0kj1m.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jdk.hongshengwenyu.top

[E14] URL 编码与 Base64
来源：http://usw.hongshengwenyu.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mcn.jiagoushi.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://gqo.daria6918.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://oiw.hammf.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dvt.nanxuanxn.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hbb.hnqzz.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://oyf.yangfankeji.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zix.yuanzhike.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qdu.cashguo.top

[E15] HTML 转义 / 反转义
来源：http://czu.sjlbkw.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ajh.wangshuangyany.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xea.guannengcc.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qor.haohaochexian.top

TS:   // 同上，务必做 XSS 过滤
来源：http://jrk.gaohongyu789.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ohm.aibaodan.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ygl.yuxming.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://izh.ppjwa.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nsk.tanke756.top

[E16] 数字千分位
来源：http://bxj.smart0.xyz

Py:   f"{1234567:,}"
来源：http://bwp.sxryk.cn

PHP:  number_format(1234567);
来源：http://pex.cashguo.top

JS:   (1234567).toLocaleString("en-US")
来源：http://sel.fktsv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://nzq.svipenyu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kco.yvedp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kiw.fzhhl.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ukz.316326.xyz

C#:   1234567.ToString("N0")
来源：http://awl.smart0.xyz

[E17] 首字母大写
来源：http://qhg.jinqigfzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wpz.xuanzx.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://gmb.nanxuanxn.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rja.gzhubu.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yzg.hnqzz.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xat.hysaishi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://oqc.hcnkem.com

Ruby: s.capitalize
来源：http://djd.daria6918.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wcu.pycfn.com

[E18] 模板占位符替换
来源：http://zbf.jianghu66.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hzv.316326.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://aey.dashuyun.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jkp.fehbvm.com

TS:   tpl.replaceAll("{name}", name)
来源：http://tat.nanxuanxn.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qig.yuxming.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jcq.zhijiandao.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ive.yvedp.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wpq.cqqwz.cn

[E19] 多行文本按行拆分
来源：http://kbg.fzhhl.top

Py:   s.splitlines()
来源：http://abg.zhiwuduotai.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wei.wangdashe.top

JS:   s.split(/\r?\n/)
来源：http://arl.pycfn.com

TS:   s.split(/\r?\n/)
来源：http://jgp.hnxiangtu.top

Java: s.lines().toList()
来源：http://xnn.jlsjyb.cn

Go:   strings.Split(s, "\n")
来源：http://jcp.birdmap.top

Ruby: s.lines
来源：http://gmm.xingfuxueyuan.xyz

C#:   s.Split('\n')
来源：http://zre.wangshuangyany.cn

[E20] 判断字符串是否为空
来源：http://cif.shanyushiyangtech.top

Py:   if not s:
来源：http://cyr.ppjwa.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nnv.dashuyun.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ipe.pengpengdd.cyou

TS:   if (s === "") {}
来源：http://vze.316326.xyz

Java: if (s.isEmpty()) {}
来源：http://ulf.9152youxi.cn

Go:   if s == "" {}
来源：http://dgg.sxryk.cn

Ruby: if s.empty?
来源：http://cit.pengpengdd.cyou

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wrv.jinyuanbaomall.cn

[E21] 超长截断加省略号
来源：http://sma.haohaochexian.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lkz.gaohongyu789.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ttp.vqdsnc.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ezl.yuanzhike.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yzt.zhiwuduotai.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://txh.xuanzx.com

Go:   // 按 rune 判断长度后截断
来源：http://kks.ivvv.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wzx.shanyushiyangkeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ttg.shanyushiyangkeji.top

[E22] 字节长度与字符长度
来源：http://bpl.guowangkeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jtw.shanyushiyangkeji.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dmt.sweek.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://coa.smart0.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rqj.hcnkem.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ydi.chenlongwang.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hiq.yj20258.top

Ruby: s.bytesize;  s.length
来源：http://uel.jianghu66.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lwo.zhoulong.xyz

================================================================================
来源：http://ssr.yangfankeji.com

F. 文件与目录
来源：http://uku.daxiang520.top

================================================================================
来源：http://nlm.fengsongda.top

[F01] 读取整个文件
来源：http://dnn.haohaochexian.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lgk.yangfankeji.com

PHP:  file_get_contents("a.txt");
来源：http://nye.316326.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wnl.cashguo.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fme.zhixingplan.top

Java: Files.readString(Path.of("a.txt"))
来源：http://fai.sxryk.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wzu.gotoacloud.top

Ruby: File.read("a.txt")
来源：http://gfs.dianchejie.cn

C#:   File.ReadAllText("a.txt");
来源：http://lix.cdnleiting.top

[F02] 逐行读取文件
来源：http://skg.yj20258888.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vti.havefunace.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xyw.nanxuanxn.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uyp.aizwys.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://res.jinyuanbaomall.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jly.yfazqb.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://itv.gotoacloud.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lua.quarkkingdee.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ulz.cdnleiting.top

[F03] 写入文件（覆盖）
来源：http://jcn.fanxiaobao.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kts.hnqzz.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://yky.fzhhl.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yqb.fehbvm.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ziu.mhx1999.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mkk.ivvv.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ano.gaohongyu789.top

Ruby: File.write("a.txt", "hi")
来源：http://mwe.pengpengdd.cyou

C#:   File.WriteAllText("a.txt", "hi");
来源：http://awq.52xcode.cn

[F04] 追加写入文件
来源：http://zvi.birdmap.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://buj.fzhhl.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://usb.nwbrower.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ecc.vehdjk.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://obg.snrcjt.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://whv.hysaishi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pox.shuidangran.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tcz.cucudq.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wzc.gotoacloud.top

[F05] 判断文件或目录是否存在
来源：http://gjv.xingfuxueyuan.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vfp.yongpay.top

PHP:  file_exists("a.txt");
来源：http://rrg.ydjk.org.cn

JS:   fs.existsSync("a.txt")
来源：http://ota.yj202588.top

TS:   fs.existsSync("a.txt")
来源：http://fhq.daria6918.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://udc.jyoumei.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://oev.9152youxi.cn

Ruby: File.exist?("a.txt")
来源：http://anr.gotoacloud.top

C#:   File.Exists("a.txt")
来源：http://vex.andypj.xyz

[F06] 删除文件
来源：http://wnk.birdmap.top

Py:   os.remove("a.txt")
来源：http://gnh.hesvh.cn

PHP:  unlink("a.txt");
来源：http://kka.hfpthk.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wei.hcnkem.com

TS:   fs.unlinkSync("a.txt")
来源：http://hrm.snrcjt.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://miv.wangshuangyany.cn

Go:   os.Remove("a.txt")
来源：http://alc.shanyushiyangkeji.top

Ruby: File.delete("a.txt")
来源：http://slx.hammf.cn

C#:   File.Delete("a.txt");
来源：http://fmm.vqdsnc.cn

[F07] 创建目录（含多级）
来源：http://bwt.yuxming.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://unp.zhixingplan.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://llw.gogol.net.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dny.fengsongda.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jlg.xuanzx.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vfm.andypj.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yuy.guannengcc.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://njo.yueranfly.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fmd.shanyushiyangkeji.top

[F08] 遍历目录
来源：http://wzn.wangshuangyany.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lik.snrcjt.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blj.jyoumei.cn

JS:   fs.readdirSync("dir")
来源：http://sdi.zycfv.cn

TS:   fs.readdirSync("dir")
来源：http://owb.pengpengdd.cyou

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yqq.cashguo.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://nlx.zhaomingkeji.xyz

Ruby: Dir.children("dir")
来源：http://twr.316326.xyz

C#:   Directory.GetFiles("dir")
来源：http://lrq.daxiang520.top

[F09] 获取文件大小
来源：http://ifv.pengpengdd.cyou

Py:   os.path.getsize("a.txt")
来源：http://gkv.haohaochexian.top

PHP:  filesize("a.txt");
来源：http://hgn.nanxuanxn.top

JS:   fs.statSync("a.txt").size
来源：http://ytm.fanxiaobao.xyz

TS:   fs.statSync("a.txt").size
来源：http://ubb.jlsjyb.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ort.ctjpmb.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cas.yueranfly.top

Ruby: File.size("a.txt")
来源：http://eph.jyoumei.cn

C#:   new FileInfo("a.txt").Length
来源：http://kxm.ehwqpu.com

[F10] 取文件扩展名 / 文件名
来源：http://ace.zdbjq.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wlq.ehwqpu.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pbr.birdmap.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ngq.feifeiyinyue.top

TS:   path.extname("a.txt")
来源：http://qjl.gogol.net.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://upk.yonumen.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mar.guannengcc.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://utx.epnwcf.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wep.shangyingyoupin.top

[F11] 复制与移动文件
来源：http://tbx.sxryk.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gec.zhaomingkeji.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://upl.ydzc1.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tiz.guowangkeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wxi.zhongyouzk.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rue.epnwcf.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kfo.haohaochexian.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wzf.redwolf501.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dhv.fzhhl.top

[F12] CSV 读写
来源：http://gmy.yj202588.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://npc.ydzc1.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://leg.jianghu66.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jln.0kj1m.cn

TS:   // 同上
来源：http://nqg.iojbl.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kji.guowangkeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qat.ppjwa.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tfj.cucudq.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lqk.hfpthk.cn

================================================================================
来源：http://vuc.zhixingplan.top

G. 面向对象
来源：http://jwm.jinqigufen.top

================================================================================
来源：http://peo.sjlbkw.cn

[G01] 定义类
来源：http://ikj.dianchejie.cn

Py:   class User: pass
来源：http://jjp.yuxming.cn

PHP:  class User {}
来源：http://kae.ppjwa.cn

JS:   class User {}
来源：http://smf.mhx1999.top

TS:   class User { name: string = ""; }
来源：http://uho.xuanzx.com

Java: class User {}
来源：http://okf.0kj1m.cn

Go:   type User struct { Name string }
来源：http://eqp.daxiang520.top

Ruby: class User; end
来源：http://xeu.ywan-chungtsiang.top

C#:   class User {}
来源：http://jmf.shanyushiyangkeji.top

[G02] 构造函数
来源：http://vud.gaohongyu789.top

Py:   def __init__(self, name): self.name = name
来源：http://wmx.zhijiandao.cn

PHP:  public function __construct(public string $name) {}
来源：http://lcm.vqdsnc.cn

JS:   constructor(name) { this.name = name; }
来源：http://ons.hesvh.cn

TS:   constructor(public name: string) {}
来源：http://sxh.yj20258.top

Java: User(String name) { this.name = name; }
来源：http://teh.xingfuxueyuan.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://akp.xuanzx.com

Ruby: def initialize(name); @name = name; end
来源：http://fqm.vehdjk.com

C#:   public User(string name) { Name = name; }
来源：http://avf.jiagoushi.top

[G03] 实例属性
来源：http://jxv.shangyingyoupin.top

Py:   self.name = "x"
来源：http://cgw.cdnleiting.top

PHP:  public string $name = "x";
来源：http://ney.yj202588.top

JS:   this.name = "x";
来源：http://lok.tanke756.top

TS:   name: string = "x";
来源：http://vld.zhiwuduotai.top

Java: private String name;
来源：http://iep.hesvh.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vgp.hesvh.cn

Ruby: @name = "x"
来源：http://duu.fengsongda.top

C#:   public string Name { get; set; } = "x";
来源：http://cfi.xinyue.icu

[G04] 定义方法
来源：http://hmv.tanke756.top

Py:   def greet(self): return self.name
来源：http://etf.jqgufenzy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://zks.yongpay.top

JS:   greet() { return this.name; }
来源：http://voq.zhaomingkeji.xyz

TS:   greet(): string { return this.name; }
来源：http://dlo.birdmap.top

Java: String greet() { return name; }
来源：http://lyl.sufxvd.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://nds.xinyue.icu

Ruby: def greet; @name; end
来源：http://vfc.fzhhl.top

C#:   public string Greet() => Name;
来源：http://iuh.ppjwa.cn

[G05] 继承
来源：http://ugm.shanyushiyangtech.top

Py:   class Admin(User): pass
来源：http://rom.ctjpmb.com

PHP:  class Admin extends User {}
来源：http://oma.cashguo.top

JS:   class Admin extends User {}
来源：http://sef.dashuyun.cn

TS:   class Admin extends User {}
来源：http://tao.nwbrower.top

Java: class Admin extends User {}
来源：http://uzd.hfpthk.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lfv.bbcook.cn

Ruby: class Admin < User; end
来源：http://lge.yueranfly.top

C#:   class Admin : User {}
来源：http://atd.yj20258.top


<!-- 参考信息 -->