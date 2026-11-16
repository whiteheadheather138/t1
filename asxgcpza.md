代发 wailian999

C#:   s.Replace("a", "b")
来源：http://hhn.yonumen.top

[E07] 按分隔符拆分
来源：http://avh.dianchejie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tee.xuetiantiany.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://htd.zdqjudy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ntu.ybcxt.top

TS:   s.split(",")
来源：http://bnd.mhx1999.top

Java: s.split(",");  s.split("\\s+")
来源：http://lbi.sufxvd.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nwh.wangshuangyany.cn

Ruby: s.split(",");  s.split
来源：http://xcj.52xcode.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xut.fengsongda.top

[E08] 数组按分隔符合并
来源：http://neb.pycfn.com

Py:   ",".join(items)
来源：http://kcq.cdnleiting.top

PHP:  implode(",", $items);
来源：http://lwe.smart0.xyz

JS:   items.join(",")
来源：http://vao.nwbrower.top

TS:   items.join(",")
来源：http://omu.wangdashe.top

Java: String.join(",", items)
来源：http://jqk.cashguo.top

Go:   strings.Join(items, ",")
来源：http://ltj.ivvv.top

Ruby: items.join(",")
来源：http://hdj.aibaodan.cn

C#:   string.Join(",", items)
来源：http://nel.hongshengwenyu.top

[E09] 去除所有空白字符
来源：http://glz.shanyushiyangtech.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dvv.yongpay.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jlg.shanyushiyangtech.top

JS:   s.replace(/\s+/g, "")
来源：http://bov.52xcode.cn

TS:   s.replace(/\s+/g, "")
来源：http://qrn.ivvv.top

Java: s.replaceAll("\\s+", "")
来源：http://qzc.c1oappe.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://hlc.gzhubu.top

Ruby: s.gsub(/\s+/, "")
来源：http://rpe.yj202588.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xhj.iojbl.cn

[E10] 左侧补零 / 定长填充
来源：http://fit.ehwqpu.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://byg.dashuyun.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vqm.hcnkem.com

JS:   "7".padStart(3, "0")
来源：http://gyj.aibaodan.cn

TS:   "7".padStart(3, "0")
来源：http://xqj.zhijiandao.cn

Java: String.format("%03d", 7)
来源：http://hef.meibo888.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://vvx.hysaishi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kho.aibaodan.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://znf.pengpengdd.cyou

[E11] 反转字符串
来源：http://cci.shuidangran.top

Py:   s[::-1]
来源：http://csk.hfpthk.cn

PHP:  strrev($s);
来源：http://ajf.tian-w.cn

JS:   [...s].reverse().join("")
来源：http://jrt.epnwcf.com

TS:   [...s].reverse().join("")
来源：http://pnf.chenlongwang.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ezv.cashguo.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://hhr.guowangkeji.top

Ruby: s.reverse
来源：http://paq.guannengcc.top

C#:   new string(s.Reverse().ToArray())
来源：http://tiz.jinyuanbaomall.cn

[E12] 统计某字符出现次数
来源：http://mmw.ivvv.top

Py:   s.count("a")
来源：http://aja.yj20258888.top

PHP:  substr_count($s, "a");
来源：http://cmi.svipenyu.cn

JS:   s.split("a").length - 1
来源：http://bio.xinyue.icu

TS:   s.split("a").length - 1
来源：http://daf.zhaomingkeji.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pwv.zhiwuduotai.top

Go:   strings.Count(s, "a")
来源：http://qhv.316326.xyz

Ruby: s.count("a")
来源：http://tqq.zhoulong.xyz

C#:   s.Count(c => c == 'a')
来源：http://pvd.feifeiyinyue.top

[E13] 逐字符遍历
来源：http://gkg.cheryme.top

Py:   for ch in s: print(ch)
来源：http://mlp.aizwys.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ncp.wangshuangyany.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ktm.iojbl.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qxy.ehwqpu.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rnw.meibo888.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://egi.daria6918.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://iye.yonumen.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wbv.fzhhl.top

[E14] URL 编码与 Base64
来源：http://hiv.zhixingplan.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lmd.tanke756.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://goq.xingfuxueyuan.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gsa.gogol.net.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://okv.epnwcf.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vro.svipenyu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mcl.hesvh.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ekq.dashuyun.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://uoq.nanxinkj.top

[E15] HTML 转义 / 反转义
来源：http://sxs.nanxinkj.top

Py:   html.escape(s);  html.unescape(s)
来源：http://jvc.zdqjudy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://soz.smart0.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cwv.epnwcf.com

TS:   // 同上，务必做 XSS 过滤
来源：http://qkm.snrcjt.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ubi.cdnleiting.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dcx.gotoacloud.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://isk.yueranfly.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yga.zhijiandao.cn

[E16] 数字千分位
来源：http://fek.cdnleiting.top

Py:   f"{1234567:,}"
来源：http://mzv.9152youxi.cn

PHP:  number_format(1234567);
来源：http://uht.yangfankeji.com

JS:   (1234567).toLocaleString("en-US")
来源：http://qfh.fanxiaobao.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://htk.yuanzhike.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lvp.havefunace.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://exe.aizwys.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bew.jianghu66.top

C#:   1234567.ToString("N0")
来源：http://tzu.yanxiufei.cn

[E17] 首字母大写
来源：http://fkp.yj20258888.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rue.ydjk.org.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://phv.dashuyun.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://obu.gaohongyu789.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://apr.bjfxy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://utv.jqgfzy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sxs.feifeiyinyue.top

Ruby: s.capitalize
来源：http://rqa.0kj1m.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qnw.shzxlz.cn

[E18] 模板占位符替换
来源：http://mvb.gogol.net.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://oat.zhoulong.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://iay.vehdjk.com

JS:   tpl.replaceAll("{name}", name)
来源：http://mnw.birdmap.top

TS:   tpl.replaceAll("{name}", name)
来源：http://kwp.yj20258888.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://djy.yuxming.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jws.cashguo.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://iiu.yangfankeji.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://knr.ydjk.org.cn

[E19] 多行文本按行拆分
来源：http://tue.jinqigfzy.top

Py:   s.splitlines()
来源：http://dbx.xziqi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pxu.52xcode.cn

JS:   s.split(/\r?\n/)
来源：http://gjg.sufxvd.cn

TS:   s.split(/\r?\n/)
来源：http://wrc.fktsv.cn

Java: s.lines().toList()
来源：http://ect.aizwys.cn

Go:   strings.Split(s, "\n")
来源：http://htf.andypj.xyz

Ruby: s.lines
来源：http://bnx.sufxvd.cn

C#:   s.Split('\n')
来源：http://mpc.zhengqikj.top

[E20] 判断字符串是否为空
来源：http://zje.guannengcc.top

Py:   if not s:
来源：http://ure.ydjk.org.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ugq.jinghuilouyu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vox.meibo888.top

TS:   if (s === "") {}
来源：http://nyb.shanyushiyangtech.top

Java: if (s.isEmpty()) {}
来源：http://bgh.yanxiufei.cn

Go:   if s == "" {}
来源：http://wlb.hywenlv.cn

Ruby: if s.empty?
来源：http://imm.zdqjudy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://azj.zdbjq.cn

[E21] 超长截断加省略号
来源：http://bso.ppjwa.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ohn.chenzaomai.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://drc.yonumen.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fsu.hnxiangtu.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cfg.xziqi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fdt.jinqigfzy.top

Go:   // 按 rune 判断长度后截断
来源：http://xhw.sweek.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lto.hywenlv.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yea.snrcjt.cn

[E22] 字节长度与字符长度
来源：http://nns.cqqwz.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sxz.chenlongwang.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nti.jqgfzy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sdq.vqdsnc.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ucc.tarul.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://avj.0kj1m.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rov.shzxlz.cn

Ruby: s.bytesize;  s.length
来源：http://tep.vehdjk.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gan.bbcook.cn

================================================================================
来源：http://toi.guannengcc.top

F. 文件与目录
来源：http://mmg.jyoumei.cn

================================================================================
来源：http://ofx.yvedp.cn

[F01] 读取整个文件
来源：http://nju.jinqigfzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xax.fengsongda.top

PHP:  file_get_contents("a.txt");
来源：http://mwh.hammf.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kxt.svipenyu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sjv.uphjek.com

Java: Files.readString(Path.of("a.txt"))
来源：http://ceo.andypj.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lzf.ctjpmb.com

Ruby: File.read("a.txt")
来源：http://lrb.nanxinkj.top

C#:   File.ReadAllText("a.txt");
来源：http://hyb.cashguo.top

[F02] 逐行读取文件
来源：http://snm.fktsv.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://htn.yuxming.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cmx.yj202588.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://reh.yuanzhike.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gvz.zycfv.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sty.jinghuilouyu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bzc.gotoacloud.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ssd.yj202588.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mqn.ctjpmb.com

[F03] 写入文件（覆盖）
来源：http://wbg.feifeiyinyue.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ppf.zdbjq.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ppi.zdbjq.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uzv.jinqigfzy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xod.birdmap.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xfu.shanyushiyangtech.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://igr.chenzaomai.com

Ruby: File.write("a.txt", "hi")
来源：http://vyj.xuanzx.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fuf.andypj.xyz

[F04] 追加写入文件
来源：http://pez.cheryme.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xrf.hnxiangtu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kva.vehdjk.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cgv.hcnkem.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ftg.guowangkeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bml.zhixingplan.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dri.uphjek.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lyh.svipenyu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://umy.fzhhl.top

[F05] 判断文件或目录是否存在
来源：http://rol.bbcook.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yzl.fehbvm.com

PHP:  file_exists("a.txt");
来源：http://dvl.zhaomingkeji.xyz

JS:   fs.existsSync("a.txt")
来源：http://var.zycfv.cn

TS:   fs.existsSync("a.txt")
来源：http://ohg.svipenyu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kpr.chenlongwang.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://naq.hcnkem.com

Ruby: File.exist?("a.txt")
来源：http://rty.zhengqikj.top

C#:   File.Exists("a.txt")
来源：http://qjn.zhixingplan.top

[F06] 删除文件
来源：http://plh.tanke756.top

Py:   os.remove("a.txt")
来源：http://bfv.ppjwa.cn

PHP:  unlink("a.txt");
来源：http://lbj.havefunace.top

JS:   fs.unlinkSync("a.txt")
来源：http://enm.jinghuilouyu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://sgn.yj202588.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://prk.xuanzx.com

Go:   os.Remove("a.txt")
来源：http://iyy.cashguo.top

Ruby: File.delete("a.txt")
来源：http://snn.ppjwa.cn

C#:   File.Delete("a.txt");
来源：http://brw.birdmap.top

[F07] 创建目录（含多级）
来源：http://gpx.fehbvm.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ucd.hfpthk.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pui.sjlbkw.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hjc.feifeiyinyue.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xce.hysaishi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qal.ybcxt.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bgo.tarul.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://irw.uphjek.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qnh.jianghu66.top

[F08] 遍历目录
来源：http://pxy.jiagoushi.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://piu.smart0.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ecv.jianghu66.top

JS:   fs.readdirSync("dir")
来源：http://xzi.yj20258888.top

TS:   fs.readdirSync("dir")
来源：http://jze.fktsv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qfb.9152youxi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://hhn.jlsjyb.cn

Ruby: Dir.children("dir")
来源：http://lej.ctjpmb.com

C#:   Directory.GetFiles("dir")
来源：http://uen.birdmap.top

[F09] 获取文件大小
来源：http://ftn.kuanghao11.cn

Py:   os.path.getsize("a.txt")
来源：http://xzg.daxiang520.top

PHP:  filesize("a.txt");
来源：http://fjb.pengpengdd.cyou

JS:   fs.statSync("a.txt").size
来源：http://qgj.nwbrower.top

TS:   fs.statSync("a.txt").size
来源：http://hsg.dashuyun.cn

Java: Files.size(Path.of("a.txt"))
来源：http://nys.wangshuangyany.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jhx.pycfn.com

Ruby: File.size("a.txt")
来源：http://dci.ppjwa.cn

C#:   new FileInfo("a.txt").Length
来源：http://joy.yueranfly.top

[F10] 取文件扩展名 / 文件名
来源：http://crf.pengpengdd.cyou

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lqi.yuxming.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nmn.aizwys.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lus.fengsongda.top

TS:   path.extname("a.txt")
来源：http://ewd.ivvv.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dsz.guannengcc.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tni.svipenyu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ulz.yuxming.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hzf.aizwys.cn

[F11] 复制与移动文件
来源：http://adc.gotoacloud.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jbq.cqqwz.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xcx.ehwqpu.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xdj.sjlbkw.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dzy.yueranfly.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cwc.bbcook.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wjt.xuetiantiany.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vol.zycfv.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qmv.zycfv.cn

[F12] CSV 读写
来源：http://otl.sufxvd.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hxq.yanxiufei.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mlq.9152youxi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bof.kuanghao11.cn

TS:   // 同上
来源：http://zol.ydjk.org.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zlb.vqdsnc.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xzs.chenjidiqi.icu

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://sgp.pycfn.com

C#:   // 无内置：用 CsvHelper 库
来源：http://lkf.wangshuangyany.cn

================================================================================
来源：http://ydl.smart0.xyz

G. 面向对象
来源：http://dlt.nanxinkj.top

================================================================================
来源：http://rfo.sweek.top

[G01] 定义类
来源：http://oyt.wangdashe.top

Py:   class User: pass
来源：http://qfx.cucudq.cn

PHP:  class User {}
来源：http://aky.tian-w.cn

JS:   class User {}
来源：http://cwn.ybcxt.top

TS:   class User { name: string = ""; }
来源：http://yao.jqgufenzy.top

Java: class User {}
来源：http://pox.zhoulong.xyz

Go:   type User struct { Name string }
来源：http://tzh.daria6918.cn

Ruby: class User; end
来源：http://abj.xinyue.icu

C#:   class User {}
来源：http://kbv.shanyushiyangtech.top

[G02] 构造函数
来源：http://rke.gaohongyu789.top

Py:   def __init__(self, name): self.name = name
来源：http://xul.ybcxt.top

PHP:  public function __construct(public string $name) {}
来源：http://ztj.shanyushiyangkeji.top

JS:   constructor(name) { this.name = name; }
来源：http://huz.gotoacloud.top

TS:   constructor(public name: string) {}
来源：http://dyk.epnwcf.com

Java: User(String name) { this.name = name; }
来源：http://bar.shangyingyoupin.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nih.shuidangran.top

Ruby: def initialize(name); @name = name; end
来源：http://ito.9152youxi.cn

C#:   public User(string name) { Name = name; }
来源：http://xgn.zhengqikj.top

[G03] 实例属性
来源：http://uff.pengpengdd.cyou

Py:   self.name = "x"
来源：http://goc.guowangkeji.top

PHP:  public string $name = "x";
来源：http://pcy.c1oappe.top

JS:   this.name = "x";
来源：http://svc.gogol.net.cn

TS:   name: string = "x";
来源：http://pzp.sufxvd.cn

Java: private String name;
来源：http://bwk.gogol.net.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wjl.aibaodan.cn

Ruby: @name = "x"
来源：http://aqw.vehdjk.com

C#:   public string Name { get; set; } = "x";
来源：http://ldh.hongshengwenyu.top

[G04] 定义方法
来源：http://fzj.yj20258888.top

Py:   def greet(self): return self.name
来源：http://lmg.cdnleiting.top

PHP:  public function greet(): string { return $this->name; }
来源：http://lpo.iojbl.cn

JS:   greet() { return this.name; }
来源：http://awm.redwolf501.top

TS:   greet(): string { return this.name; }
来源：http://mhj.xinyue.icu

Java: String greet() { return name; }
来源：http://rsc.fzhhl.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://xxd.hfpthk.cn

Ruby: def greet; @name; end
来源：http://tjy.yvedp.cn

C#:   public string Greet() => Name;
来源：http://eid.cashguo.top

[G05] 继承
来源：http://rss.hesvh.cn

Py:   class Admin(User): pass
来源：http://rda.wangdashe.top

PHP:  class Admin extends User {}
来源：http://kof.cqqwz.cn

JS:   class Admin extends User {}
来源：http://vio.epnwcf.com

TS:   class Admin extends User {}
来源：http://ynl.vehdjk.com


<!-- 参考信息 -->