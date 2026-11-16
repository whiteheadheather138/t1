代发 wailian999

C#:   s.Replace("a", "b")
来源：http://cdp.redwolf501.top

[E07] 按分隔符拆分
来源：http://whh.chenlongwang.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fgh.cucudq.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bey.jinghuilouyu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://lzj.sufxvd.cn

TS:   s.split(",")
来源：http://wkj.yuanzhike.top

Java: s.split(",");  s.split("\\s+")
来源：http://jcf.gaohongyu789.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://weq.0kj1m.cn

Ruby: s.split(",");  s.split
来源：http://lzd.sufxvd.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qko.birdmap.top

[E08] 数组按分隔符合并
来源：http://vja.hywenlv.cn

Py:   ",".join(items)
来源：http://sen.316326.xyz

PHP:  implode(",", $items);
来源：http://cye.guowangkeji.top

JS:   items.join(",")
来源：http://cmu.daxiang520.top

TS:   items.join(",")
来源：http://lal.epnwcf.com

Java: String.join(",", items)
来源：http://vid.smart0.xyz

Go:   strings.Join(items, ",")
来源：http://jkh.zdbjq.cn

Ruby: items.join(",")
来源：http://wse.redwolf501.top

C#:   string.Join(",", items)
来源：http://vwr.cdnleiting.top

[E09] 去除所有空白字符
来源：http://ies.kuanghao11.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nfj.ppjwa.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://atb.shangyingyoupin.top

JS:   s.replace(/\s+/g, "")
来源：http://wxm.guowangkeji.top

TS:   s.replace(/\s+/g, "")
来源：http://pqf.fengsongda.top

Java: s.replaceAll("\\s+", "")
来源：http://uom.vehdjk.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://kdq.andypj.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://bqu.yanxiufei.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zpv.jyoumei.cn

[E10] 左侧补零 / 定长填充
来源：http://iko.vehdjk.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sei.hongshengwenyu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://izq.zhengqikj.top

JS:   "7".padStart(3, "0")
来源：http://ydz.jyoumei.cn

TS:   "7".padStart(3, "0")
来源：http://hoy.gogol.net.cn

Java: String.format("%03d", 7)
来源：http://jpg.haohaochexian.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://qci.haohaochexian.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hlv.zhiwuduotai.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wed.tanke756.top

[E11] 反转字符串
来源：http://vwt.hesvh.cn

Py:   s[::-1]
来源：http://ndl.xingfuxueyuan.xyz

PHP:  strrev($s);
来源：http://qvk.jqgufenzy.top

JS:   [...s].reverse().join("")
来源：http://rvu.zhongyouzk.top

TS:   [...s].reverse().join("")
来源：http://xuk.zycfv.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ujs.xuanzx.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://eft.ivvv.top

Ruby: s.reverse
来源：http://rhw.xingfuxueyuan.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://hzv.shzxlz.cn

[E12] 统计某字符出现次数
来源：http://ijq.jinghuilouyu.cn

Py:   s.count("a")
来源：http://mih.sxryk.cn

PHP:  substr_count($s, "a");
来源：http://yup.snrcjt.cn

JS:   s.split("a").length - 1
来源：http://mxh.fengsongda.top

TS:   s.split("a").length - 1
来源：http://oib.wangdashe.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pee.xinyue.icu

Go:   strings.Count(s, "a")
来源：http://yln.9152youxi.cn

Ruby: s.count("a")
来源：http://pol.0kj1m.cn

C#:   s.Count(c => c == 'a')
来源：http://fso.chenjidiqi.icu

[E13] 逐字符遍历
来源：http://blj.jiagoushi.top

Py:   for ch in s: print(ch)
来源：http://evt.quarkkingdee.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bwu.hnxiangtu.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://eje.bbcook.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://kil.hnqzz.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pmt.andypj.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vjd.jiagoushi.top

Ruby: s.each_char { |ch| puts ch }
来源：http://xds.yuxming.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://iuj.jinghuilouyu.cn

[E14] URL 编码与 Base64
来源：http://vtt.fzhhl.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://izu.hnxiangtu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://loe.hongshengwenyu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lwm.zhengqikj.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nkw.hfpthk.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ljy.yfazqb.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uwo.shanyushiyangtech.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tko.iojbl.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ffr.guowangkeji.top

[E15] HTML 转义 / 反转义
来源：http://elh.haohaochexian.top

Py:   html.escape(s);  html.unescape(s)
来源：http://fgz.bbcook.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qxs.tian-w.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://iur.shzxlz.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wxr.jinqigufen.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bce.gotoacloud.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://omy.hfpthk.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fqm.andypj.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jbk.ppjwa.cn

[E16] 数字千分位
来源：http://jxk.jinghuilouyu.cn

Py:   f"{1234567:,}"
来源：http://uln.yuanzhike.top

PHP:  number_format(1234567);
来源：http://mku.jinqigfzy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://mio.havefunace.top

TS:   (1234567).toLocaleString("en-US")
来源：http://xiv.jinqigufen.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sej.0kj1m.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cwk.jinqigfzy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://aca.tarul.cn

C#:   1234567.ToString("N0")
来源：http://apu.snrcjt.cn

[E17] 首字母大写
来源：http://ogx.jinghuilouyu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ebs.guowangkeji.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ogh.tarul.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lwy.sysykeji.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jwe.hammf.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nsi.cucudq.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ltk.aibaodan.cn

Ruby: s.capitalize
来源：http://rsd.redwolf501.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fra.pengpengdd.cyou

[E18] 模板占位符替换
来源：http://srf.shanyushiyangtech.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://owm.svipenyu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dut.tianlin.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://itf.wangshuangyany.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://zpk.ydjk.org.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lds.shanyushiyangtech.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://obk.yangfankeji.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://eoy.pengpengdd.cyou

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xmn.hfpthk.cn

[E19] 多行文本按行拆分
来源：http://fvy.yongpay.top

Py:   s.splitlines()
来源：http://ffp.shanyushiyangtech.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://akh.ehwqpu.com

JS:   s.split(/\r?\n/)
来源：http://qzi.gogol.net.cn

TS:   s.split(/\r?\n/)
来源：http://ppo.birdmap.top

Java: s.lines().toList()
来源：http://osl.andypj.xyz

Go:   strings.Split(s, "\n")
来源：http://vks.dashuyun.cn

Ruby: s.lines
来源：http://uyy.yfazqb.com

C#:   s.Split('\n')
来源：http://joe.xylfe.cn

[E20] 判断字符串是否为空
来源：http://pao.jinghuilouyu.cn

Py:   if not s:
来源：http://wlk.mhx1999.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://otf.havefunace.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bem.yonumen.top

TS:   if (s === "") {}
来源：http://uap.shanyushiyangtech.top

Java: if (s.isEmpty()) {}
来源：http://rmz.xylfe.cn

Go:   if s == "" {}
来源：http://chk.jianghu66.top

Ruby: if s.empty?
来源：http://shk.zhaomingkeji.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pzy.chenlongwang.top

[E21] 超长截断加省略号
来源：http://qin.nanxinkj.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ltq.cheryme.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vfx.shuidangran.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zbm.xylfe.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://usk.aibaodan.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://akv.hnxiangtu.top

Go:   // 按 rune 判断长度后截断
来源：http://dgk.yangfankeji.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xug.hongshengwenyu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lxe.tian-w.cn

[E22] 字节长度与字符长度
来源：http://dym.0kj1m.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fjo.52xcode.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kep.jiagoushi.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xud.ydzc1.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vlv.chenjidiqi.icu

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tmg.jinqigfzy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sec.ywan-chungtsiang.top

Ruby: s.bytesize;  s.length
来源：http://seg.smart0.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://klc.hywenlv.cn

================================================================================
来源：http://uks.sxryk.cn

F. 文件与目录
来源：http://tzq.ydzc1.top

================================================================================
来源：http://dud.jqgufenzy.top

[F01] 读取整个文件
来源：http://jxj.xinyue.icu

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vss.dianchejie.cn

PHP:  file_get_contents("a.txt");
来源：http://lee.guowangkeji.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kst.dianchejie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vew.smart0.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://vch.shangyingyoupin.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wim.sweek.top

Ruby: File.read("a.txt")
来源：http://bhm.hywenlv.cn

C#:   File.ReadAllText("a.txt");
来源：http://ztb.jyoumei.cn

[F02] 逐行读取文件
来源：http://rmd.fktsv.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://num.jqgufenzy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cvg.guannengcc.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yzx.sxryk.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lln.sweek.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sqw.sxryk.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pxw.yueranfly.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ctx.kuanghao11.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dta.zhiwuduotai.top

[F03] 写入文件（覆盖）
来源：http://kvi.hongshengwenyu.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://eka.yanxiufei.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://jwg.guannengcc.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yty.xuetiantiany.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uza.jqgufenzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qvt.zhijiandao.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ixb.jyoumei.cn

Ruby: File.write("a.txt", "hi")
来源：http://mnv.redwolf501.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gzk.sufxvd.cn

[F04] 追加写入文件
来源：http://eoo.svipenyu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://iml.zhijiandao.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jel.andypj.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://exs.ppjwa.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gvz.yonumen.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ute.zhijiandao.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xnc.yj20258.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dql.gotoacloud.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dbs.xingfuxueyuan.xyz

[F05] 判断文件或目录是否存在
来源：http://qww.havefunace.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tve.yangfankeji.com

PHP:  file_exists("a.txt");
来源：http://myp.zhaomingkeji.xyz

JS:   fs.existsSync("a.txt")
来源：http://fum.yj20258888.top

TS:   fs.existsSync("a.txt")
来源：http://pws.hywenlv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gcc.zycfv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hbg.tianlin.xyz

Ruby: File.exist?("a.txt")
来源：http://dtn.ppjwa.cn

C#:   File.Exists("a.txt")
来源：http://ffe.zdqjudy.top

[F06] 删除文件
来源：http://reu.chenzaomai.com

Py:   os.remove("a.txt")
来源：http://iji.dashuyun.cn

PHP:  unlink("a.txt");
来源：http://tlp.epnwcf.com

JS:   fs.unlinkSync("a.txt")
来源：http://jnh.ydzc1.top

TS:   fs.unlinkSync("a.txt")
来源：http://amq.gaohongyu789.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uyv.andypj.xyz

Go:   os.Remove("a.txt")
来源：http://zwk.jinqigfzy.top

Ruby: File.delete("a.txt")
来源：http://vdg.sjlbkw.cn

C#:   File.Delete("a.txt");
来源：http://jyq.yonumen.top

[F07] 创建目录（含多级）
来源：http://jrp.aibaodan.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qbg.nanxinkj.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fxf.redwolf501.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ndq.cqqwz.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://juq.jyoumei.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ide.gogol.net.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://igu.daria6918.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rha.fengsongda.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ezk.c1oappe.top

[F08] 遍历目录
来源：http://ojk.xingfuxueyuan.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://bsx.zycfv.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nil.fzhhl.top

JS:   fs.readdirSync("dir")
来源：http://vgm.fanxiaobao.xyz

TS:   fs.readdirSync("dir")
来源：http://qws.hammf.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sst.ivvv.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://gnj.hcnkem.com

Ruby: Dir.children("dir")
来源：http://otl.epnwcf.com

C#:   Directory.GetFiles("dir")
来源：http://fqk.havefunace.top

[F09] 获取文件大小
来源：http://tjt.yanxiufei.cn

Py:   os.path.getsize("a.txt")
来源：http://pie.chenjidiqi.icu

PHP:  filesize("a.txt");
来源：http://pxg.smart0.xyz

JS:   fs.statSync("a.txt").size
来源：http://kau.tanke756.top

TS:   fs.statSync("a.txt").size
来源：http://aqh.pengpengdd.cyou

Java: Files.size(Path.of("a.txt"))
来源：http://syb.zycfv.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://luo.jinyuanbaomall.cn

Ruby: File.size("a.txt")
来源：http://vlt.yj202588.top

C#:   new FileInfo("a.txt").Length
来源：http://ivh.aibaodan.cn

[F10] 取文件扩展名 / 文件名
来源：http://zlv.zhaomingkeji.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://suy.zycfv.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mxp.jinqigfzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://eha.guannengcc.top

TS:   path.extname("a.txt")
来源：http://sib.hongshengwenyu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://udb.jiagoushi.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lba.wangshuangyany.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mny.hongshengwenyu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://btb.zhijiandao.cn

[F11] 复制与移动文件
来源：http://msl.hesvh.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kdl.fanxiaobao.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wbz.wangdashe.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eya.sysykeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uto.zhixingplan.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jux.sufxvd.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pol.wangdashe.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zub.aibaodan.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://toi.guowangkeji.top

[F12] CSV 读写
来源：http://wfp.zycfv.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ybg.havefunace.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bib.jqgufenzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pra.wangdashe.top

TS:   // 同上
来源：http://odq.kuanghao11.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cme.xingfuxueyuan.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ifi.gaohongyu789.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bis.yanxiufei.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://umh.andypj.xyz

================================================================================
来源：http://ewo.ywan-chungtsiang.top

G. 面向对象
来源：http://yms.zhoulong.xyz

================================================================================
来源：http://mhm.sysykeji.top

[G01] 定义类
来源：http://acx.fanxiaobao.xyz

Py:   class User: pass
来源：http://buv.yuanzhike.top

PHP:  class User {}
来源：http://kze.nanxinkj.top

JS:   class User {}
来源：http://wmg.epnwcf.com

TS:   class User { name: string = ""; }
来源：http://tii.zhongyouzk.top

Java: class User {}
来源：http://nox.jinghuilouyu.cn

Go:   type User struct { Name string }
来源：http://rnt.hammf.cn

Ruby: class User; end
来源：http://vbg.chenlongwang.top

C#:   class User {}
来源：http://kpi.ybcxt.top

[G02] 构造函数
来源：http://soy.yj20258.top

Py:   def __init__(self, name): self.name = name
来源：http://pop.yj20258.top

PHP:  public function __construct(public string $name) {}
来源：http://ckj.dashuyun.cn

JS:   constructor(name) { this.name = name; }
来源：http://dnd.dashuyun.cn

TS:   constructor(public name: string) {}
来源：http://dar.xylfe.cn

Java: User(String name) { this.name = name; }
来源：http://bvx.shuidangran.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lml.vehdjk.com

Ruby: def initialize(name); @name = name; end
来源：http://lqt.smart0.xyz

C#:   public User(string name) { Name = name; }
来源：http://ayj.c1oappe.top

[G03] 实例属性
来源：http://pyr.feifeiyinyue.top

Py:   self.name = "x"
来源：http://cdo.redwolf501.top

PHP:  public string $name = "x";
来源：http://gdd.jlsjyb.cn

JS:   this.name = "x";
来源：http://obs.hongshengwenyu.top

TS:   name: string = "x";
来源：http://wtt.sysykeji.top

Java: private String name;
来源：http://uso.meibo888.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://eig.xziqi.cn

Ruby: @name = "x"
来源：http://umx.vqdsnc.cn

C#:   public string Name { get; set; } = "x";
来源：http://jom.sweek.top

[G04] 定义方法
来源：http://xld.epnwcf.com

Py:   def greet(self): return self.name
来源：http://bmn.yj20258.top

PHP:  public function greet(): string { return $this->name; }
来源：http://vcv.zdbjq.cn

JS:   greet() { return this.name; }
来源：http://fsc.svipenyu.cn

TS:   greet(): string { return this.name; }
来源：http://uzu.pengpengdd.cyou

Java: String greet() { return name; }
来源：http://npq.yongpay.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://tnz.zhongyouzk.top

Ruby: def greet; @name; end
来源：http://rnx.jlsjyb.cn

C#:   public string Greet() => Name;
来源：http://cex.yuanzhike.top

[G05] 继承
来源：http://dbl.xuetiantiany.cn

Py:   class Admin(User): pass
来源：http://uoz.ppjwa.cn

PHP:  class Admin extends User {}
来源：http://ess.fengsongda.top

JS:   class Admin extends User {}
来源：http://utg.hongshengwenyu.top

TS:   class Admin extends User {}
来源：http://xwg.zdqjudy.top


<!-- 参考信息 -->