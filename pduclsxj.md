代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://czz.meibo888.top

TS:   s.split(",")
来源：http://xpz.xingfuxueyuan.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://fid.ydzc1.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://men.zdqjudy.top

Ruby: s.split(",");  s.split
来源：http://kpc.pycfn.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rlw.nanxuanxn.top

[E08] 数组按分隔符合并
来源：http://uyp.yj202588.top

Py:   ",".join(items)
来源：http://yrn.c1oappe.top

PHP:  implode(",", $items);
来源：http://kus.316326.xyz

JS:   items.join(",")
来源：http://ovr.dashuyun.cn

TS:   items.join(",")
来源：http://vrx.yj20258.top

Java: String.join(",", items)
来源：http://hrb.ivvv.top

Go:   strings.Join(items, ",")
来源：http://isp.ivvv.top

Ruby: items.join(",")
来源：http://nle.fktsv.cn

C#:   string.Join(",", items)
来源：http://xuy.hammf.cn

[E09] 去除所有空白字符
来源：http://azi.tanke756.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rst.vehdjk.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://izt.yfazqb.com

JS:   s.replace(/\s+/g, "")
来源：http://ivl.chenlongwang.top

TS:   s.replace(/\s+/g, "")
来源：http://naw.sysykeji.top

Java: s.replaceAll("\\s+", "")
来源：http://kwk.chenjidiqi.icu

Go:   strings.Join(strings.Fields(s), "")
来源：http://box.guannengcc.top

Ruby: s.gsub(/\s+/, "")
来源：http://srp.yj20258888.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gjt.shuidangran.top

[E10] 左侧补零 / 定长填充
来源：http://nnb.wangdashe.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gty.vehdjk.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xyo.hfpthk.cn

JS:   "7".padStart(3, "0")
来源：http://reg.daxiang520.top

TS:   "7".padStart(3, "0")
来源：http://csq.dashuyun.cn

Java: String.format("%03d", 7)
来源：http://pum.ydjk.org.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ccp.fengsongda.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vwx.jiagoushi.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yjg.0kj1m.cn

[E11] 反转字符串
来源：http://zvv.jianghu66.top

Py:   s[::-1]
来源：http://jts.ctjpmb.com

PHP:  strrev($s);
来源：http://rtr.sweek.top

JS:   [...s].reverse().join("")
来源：http://wre.gogol.net.cn

TS:   [...s].reverse().join("")
来源：http://yst.wangdashe.top

Java: new StringBuilder(s).reverse().toString()
来源：http://dsj.hcnkem.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://sih.iojbl.cn

Ruby: s.reverse
来源：http://icl.svipenyu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qgm.shangyingyoupin.top

[E12] 统计某字符出现次数
来源：http://ojl.tanke756.top

Py:   s.count("a")
来源：http://uok.sxryk.cn

PHP:  substr_count($s, "a");
来源：http://lvf.jlsjyb.cn

JS:   s.split("a").length - 1
来源：http://jjz.cheryme.top

TS:   s.split("a").length - 1
来源：http://cwg.aibaodan.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fbz.epnwcf.com

Go:   strings.Count(s, "a")
来源：http://ggx.jiagoushi.top

Ruby: s.count("a")
来源：http://tiw.vqdsnc.cn

C#:   s.Count(c => c == 'a')
来源：http://iwu.chenzaomai.com

[E13] 逐字符遍历
来源：http://ont.jianghu66.top

Py:   for ch in s: print(ch)
来源：http://lys.andypj.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lor.ydjk.org.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://aok.feifeiyinyue.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://rcb.zhaomingkeji.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pnw.fengsongda.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xfx.havefunace.top

Ruby: s.each_char { |ch| puts ch }
来源：http://feq.birdmap.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pgd.pycfn.com

[E14] URL 编码与 Base64
来源：http://yix.zdqjudy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qxr.hysaishi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://wrv.zdqjudy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hbu.yonumen.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tme.xuetiantiany.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://eir.haohaochexian.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wlm.hammf.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gbr.fehbvm.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vli.sxryk.cn

[E15] HTML 转义 / 反转义
来源：http://nmk.xylfe.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rsk.redwolf501.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://spo.redwolf501.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://avq.sweek.top

TS:   // 同上，务必做 XSS 过滤
来源：http://tcn.jiagoushi.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dbf.yj202588.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uvd.andypj.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ygm.jinghuilouyu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://odq.fengsongda.top

[E16] 数字千分位
来源：http://sxm.wangshuangyany.cn

Py:   f"{1234567:,}"
来源：http://cjk.nanxuanxn.top

PHP:  number_format(1234567);
来源：http://srh.daria6918.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xts.xuetiantiany.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gop.zhijiandao.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vdz.yangfankeji.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://iwx.shzxlz.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fxs.zhaomingkeji.xyz

C#:   1234567.ToString("N0")
来源：http://chi.nwbrower.top

[E17] 首字母大写
来源：http://dqc.meibo888.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tvo.yangfankeji.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://civ.smart0.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://evp.dianchejie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://neg.jiagoushi.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://quz.fehbvm.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fab.yuxming.cn

Ruby: s.capitalize
来源：http://bdn.yueranfly.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://inw.gotoacloud.top

[E18] 模板占位符替换
来源：http://hzg.jianghu66.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cjk.ivvv.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hbw.cashguo.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ytm.uphjek.com

TS:   tpl.replaceAll("{name}", name)
来源：http://llo.hnqzz.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qhj.ydjk.org.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cff.shzxlz.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cgi.mhx1999.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://akn.yfazqb.com

[E19] 多行文本按行拆分
来源：http://hfx.ivvv.top

Py:   s.splitlines()
来源：http://ttf.zycfv.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qfa.gotoacloud.top

JS:   s.split(/\r?\n/)
来源：http://kuj.hesvh.cn

TS:   s.split(/\r?\n/)
来源：http://wsm.chenzaomai.com

Java: s.lines().toList()
来源：http://pvn.yueranfly.top

Go:   strings.Split(s, "\n")
来源：http://gme.ybcxt.top

Ruby: s.lines
来源：http://ife.yanxiufei.cn

C#:   s.Split('\n')
来源：http://jok.dianchejie.cn

[E20] 判断字符串是否为空
来源：http://onx.fanxiaobao.xyz

Py:   if not s:
来源：http://izz.nwbrower.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bot.0kj1m.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://avv.mhx1999.top

TS:   if (s === "") {}
来源：http://zxn.jlsjyb.cn

Java: if (s.isEmpty()) {}
来源：http://chm.cdnleiting.top

Go:   if s == "" {}
来源：http://yhd.epnwcf.com

Ruby: if s.empty?
来源：http://oiv.yj20258888.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ubf.jinqigufen.top

[E21] 超长截断加省略号
来源：http://hyd.wangdashe.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ros.redwolf501.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://anw.aizwys.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dpn.gzhubu.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://orm.aibaodan.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pul.xuetiantiany.cn

Go:   // 按 rune 判断长度后截断
来源：http://cfg.zhixingplan.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cuf.yj202588.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uqp.hnqzz.top

[E22] 字节长度与字符长度
来源：http://iom.ywan-chungtsiang.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://syh.iojbl.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dbo.tarul.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bfr.ehwqpu.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://npt.tanke756.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sbu.zhengqikj.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bpz.snrcjt.cn

Ruby: s.bytesize;  s.length
来源：http://sxa.zhaomingkeji.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://inl.tarul.cn

================================================================================
来源：http://jdg.daxiang520.top

F. 文件与目录
来源：http://nlq.tianlin.xyz

================================================================================
来源：http://bgw.hongshengwenyu.top

[F01] 读取整个文件
来源：http://wla.9152youxi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dpt.52xcode.cn

PHP:  file_get_contents("a.txt");
来源：http://lri.sweek.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wjc.ctjpmb.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sdl.cdnleiting.top

Java: Files.readString(Path.of("a.txt"))
来源：http://gng.andypj.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ssh.yuxming.cn

Ruby: File.read("a.txt")
来源：http://kyx.nanxinkj.top

C#:   File.ReadAllText("a.txt");
来源：http://zws.fzhhl.top

[F02] 逐行读取文件
来源：http://pnt.hongshengwenyu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nse.guannengcc.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fip.uphjek.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hgo.ybcxt.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jdw.xuetiantiany.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://emu.redwolf501.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hzi.birdmap.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xhl.yangfankeji.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://orw.sweek.top

[F03] 写入文件（覆盖）
来源：http://twa.gaohongyu789.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jfo.ywan-chungtsiang.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://dyn.tanke756.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ryu.aibaodan.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mih.zhijiandao.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://auv.guowangkeji.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kyh.9152youxi.cn

Ruby: File.write("a.txt", "hi")
来源：http://kso.jlsjyb.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bbk.jinghuilouyu.cn

[F04] 追加写入文件
来源：http://xxw.bbcook.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sfs.shanyushiyangkeji.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://oqo.zhongyouzk.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fui.cdnleiting.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mqc.ctjpmb.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kfd.feifeiyinyue.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dot.zhongyouzk.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qyx.wangdashe.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ghz.havefunace.top

[F05] 判断文件或目录是否存在
来源：http://wea.ydzc1.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ryj.gaohongyu789.top

PHP:  file_exists("a.txt");
来源：http://hwz.yonumen.top

JS:   fs.existsSync("a.txt")
来源：http://dbi.yanxiufei.cn

TS:   fs.existsSync("a.txt")
来源：http://xdn.shangyingyoupin.top

Java: Files.exists(Path.of("a.txt"))
来源：http://rcg.daxiang520.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xlg.nanxinkj.top

Ruby: File.exist?("a.txt")
来源：http://osi.xingfuxueyuan.xyz

C#:   File.Exists("a.txt")
来源：http://zhk.ctjpmb.com

[F06] 删除文件
来源：http://jfo.iojbl.cn

Py:   os.remove("a.txt")
来源：http://vri.meibo888.top

PHP:  unlink("a.txt");
来源：http://yrz.xuanzx.com

JS:   fs.unlinkSync("a.txt")
来源：http://tdq.gaohongyu789.top

TS:   fs.unlinkSync("a.txt")
来源：http://cwo.fanxiaobao.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sak.hysaishi.cn

Go:   os.Remove("a.txt")
来源：http://ltv.zhongyouzk.top

Ruby: File.delete("a.txt")
来源：http://myv.fktsv.cn

C#:   File.Delete("a.txt");
来源：http://vwm.jqgufenzy.top

[F07] 创建目录（含多级）
来源：http://ipe.shanyushiyangtech.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://urn.hongshengwenyu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qwu.aibaodan.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dte.yonumen.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wvf.wangshuangyany.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bzt.yanxiufei.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ztr.nanxinkj.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zdv.zdqjudy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zaz.yj20258.top

[F08] 遍历目录
来源：http://oir.hongshengwenyu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://bgt.zhongyouzk.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ghc.ydjk.org.cn

JS:   fs.readdirSync("dir")
来源：http://mjr.uphjek.com

TS:   fs.readdirSync("dir")
来源：http://mst.zycfv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://znk.ctjpmb.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://ewa.jlsjyb.cn

Ruby: Dir.children("dir")
来源：http://lpy.cqqwz.cn

C#:   Directory.GetFiles("dir")
来源：http://vyv.redwolf501.top

[F09] 获取文件大小
来源：http://tpd.ydzc1.top

Py:   os.path.getsize("a.txt")
来源：http://hlk.vqdsnc.cn

PHP:  filesize("a.txt");
来源：http://ivn.cdnleiting.top

JS:   fs.statSync("a.txt").size
来源：http://tzd.yueranfly.top

TS:   fs.statSync("a.txt").size
来源：http://iju.fzhhl.top

Java: Files.size(Path.of("a.txt"))
来源：http://kgp.yfazqb.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mfz.daria6918.cn

Ruby: File.size("a.txt")
来源：http://dii.sjlbkw.cn

C#:   new FileInfo("a.txt").Length
来源：http://fpj.yj202588.top

[F10] 取文件扩展名 / 文件名
来源：http://ruu.ydzc1.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fku.jinghuilouyu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jet.xylfe.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cav.iojbl.cn

TS:   path.extname("a.txt")
来源：http://trl.gotoacloud.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kgh.havefunace.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fuh.tian-w.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gqt.zdbjq.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dud.chenlongwang.top

[F11] 复制与移动文件
来源：http://pgq.yonumen.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://icq.c1oappe.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wlu.birdmap.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xui.fehbvm.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xgh.zhaomingkeji.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://syb.sjlbkw.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bxa.sufxvd.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pfy.fktsv.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qhj.xylfe.cn

[F12] CSV 读写
来源：http://fho.zhixingplan.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gpz.hywenlv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://izx.jianghu66.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kai.ybcxt.top

TS:   // 同上
来源：http://rhc.xuetiantiany.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kro.haohaochexian.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://upq.ppjwa.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bcx.yj20258888.top

C#:   // 无内置：用 CsvHelper 库
来源：http://osn.vehdjk.com

================================================================================
来源：http://gqk.fengsongda.top

G. 面向对象
来源：http://icr.xuanzx.com

================================================================================
来源：http://fib.jqgufenzy.top

[G01] 定义类
来源：http://qex.hfpthk.cn

Py:   class User: pass
来源：http://nqc.cheryme.top

PHP:  class User {}
来源：http://yqn.xziqi.cn

JS:   class User {}
来源：http://stp.yj20258.top

TS:   class User { name: string = ""; }
来源：http://xgg.hesvh.cn

Java: class User {}
来源：http://ukf.9152youxi.cn

Go:   type User struct { Name string }
来源：http://hps.dianchejie.cn

Ruby: class User; end
来源：http://lai.jinghuilouyu.cn

C#:   class User {}
来源：http://bxx.gaohongyu789.top

[G02] 构造函数
来源：http://yml.ehwqpu.com

Py:   def __init__(self, name): self.name = name
来源：http://myp.yfazqb.com

PHP:  public function __construct(public string $name) {}
来源：http://mmu.ydjk.org.cn

JS:   constructor(name) { this.name = name; }
来源：http://hui.hcnkem.com

TS:   constructor(public name: string) {}
来源：http://nhs.chenlongwang.top

Java: User(String name) { this.name = name; }
来源：http://kvz.iojbl.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mme.zdbjq.cn

Ruby: def initialize(name); @name = name; end
来源：http://lpf.birdmap.top

C#:   public User(string name) { Name = name; }
来源：http://jiu.zhijiandao.cn

[G03] 实例属性
来源：http://xpv.yj20258888.top

Py:   self.name = "x"
来源：http://qat.havefunace.top

PHP:  public string $name = "x";
来源：http://qsb.gzhubu.top

JS:   this.name = "x";
来源：http://xns.yuanzhike.top

TS:   name: string = "x";
来源：http://qhu.zdqjudy.top

Java: private String name;
来源：http://pfk.jiagoushi.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tya.tarul.cn

Ruby: @name = "x"
来源：http://yud.chenlongwang.top

C#:   public string Name { get; set; } = "x";
来源：http://fix.ivvv.top

[G04] 定义方法
来源：http://iyt.cashguo.top

Py:   def greet(self): return self.name
来源：http://uao.jinyuanbaomall.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fad.yuxming.cn

JS:   greet() { return this.name; }
来源：http://cka.bjfxy.top

TS:   greet(): string { return this.name; }
来源：http://wzn.hysaishi.cn

Java: String greet() { return name; }
来源：http://qtt.shzxlz.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hvt.hfpthk.cn

Ruby: def greet; @name; end
来源：http://ytp.yanxiufei.cn

C#:   public string Greet() => Name;
来源：http://gbi.jinghuilouyu.cn

[G05] 继承
来源：http://tct.guannengcc.top

Py:   class Admin(User): pass
来源：http://bys.wangdashe.top

PHP:  class Admin extends User {}
来源：http://gyo.yangfankeji.com

JS:   class Admin extends User {}
来源：http://wzx.pengpengdd.cyou

TS:   class Admin extends User {}
来源：http://jtj.chenzaomai.com

Java: class Admin extends User {}
来源：http://ajb.ivvv.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qkm.tanke756.top

Ruby: class Admin < User; end
来源：http://vmy.hongshengwenyu.top

C#:   class Admin : User {}
来源：http://onc.yueranfly.top


<!-- 参考信息 -->