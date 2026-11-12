代发 wailian999

PHP:  implode(",", $items);
来源：http://mtz.xinyue.icu

JS:   items.join(",")
来源：http://hhd.yj20258888.top

TS:   items.join(",")
来源：http://mum.yj20258888.top

Java: String.join(",", items)
来源：http://rov.sysykeji.top

Go:   strings.Join(items, ",")
来源：http://fca.jinghuilouyu.cn

Ruby: items.join(",")
来源：http://hxp.shanyushiyangkeji.top

C#:   string.Join(",", items)
来源：http://qzf.fktsv.cn

[E09] 去除所有空白字符
来源：http://mcm.guannengcc.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vdz.zhijiandao.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xnw.cdnleiting.top

JS:   s.replace(/\s+/g, "")
来源：http://xas.fehbvm.com

TS:   s.replace(/\s+/g, "")
来源：http://wvg.daxiang520.top

Java: s.replaceAll("\\s+", "")
来源：http://crk.ydzc1.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ifi.cdnleiting.top

Ruby: s.gsub(/\s+/, "")
来源：http://ift.zhaomingkeji.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://otk.9152youxi.cn

[E10] 左侧补零 / 定长填充
来源：http://nca.zhijiandao.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tqj.hywenlv.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vrq.sweek.top

JS:   "7".padStart(3, "0")
来源：http://gjk.hesvh.cn

TS:   "7".padStart(3, "0")
来源：http://cfb.zycfv.cn

Java: String.format("%03d", 7)
来源：http://snq.9152youxi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://elm.cdnleiting.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tez.fehbvm.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rdt.chenjidiqi.icu

[E11] 反转字符串
来源：http://xrn.ehwqpu.com

Py:   s[::-1]
来源：http://hht.jqgufenzy.top

PHP:  strrev($s);
来源：http://zqz.tianlin.xyz

JS:   [...s].reverse().join("")
来源：http://wpr.aibaodan.cn

TS:   [...s].reverse().join("")
来源：http://kcf.yonumen.top

Java: new StringBuilder(s).reverse().toString()
来源：http://txx.jqgfzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://myz.chenzaomai.com

Ruby: s.reverse
来源：http://rgr.zhongyouzk.top

C#:   new string(s.Reverse().ToArray())
来源：http://dah.aibaodan.cn

[E12] 统计某字符出现次数
来源：http://jfr.bbcook.cn

Py:   s.count("a")
来源：http://buc.vehdjk.com

PHP:  substr_count($s, "a");
来源：http://kvj.hysaishi.cn

JS:   s.split("a").length - 1
来源：http://rci.ywan-chungtsiang.top

TS:   s.split("a").length - 1
来源：http://hug.zhixingplan.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kbc.yanxiufei.cn

Go:   strings.Count(s, "a")
来源：http://tyz.aibaodan.cn

Ruby: s.count("a")
来源：http://dmp.yfazqb.com

C#:   s.Count(c => c == 'a')
来源：http://rcu.uphjek.com

[E13] 逐字符遍历
来源：http://ivn.yj202588.top

Py:   for ch in s: print(ch)
来源：http://szo.tian-w.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ccn.xingfuxueyuan.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://jfs.dianchejie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bay.ivvv.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://irj.shanyushiyangtech.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pti.hywenlv.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://nbd.tanke756.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baf.jinqigfzy.top

[E14] URL 编码与 Base64
来源：http://xrn.cdnleiting.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://utx.yj20258888.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://dyj.andypj.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://emy.cashguo.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dnj.yj202588.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kxj.shanyushiyangkeji.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://glm.yueranfly.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tbd.ywan-chungtsiang.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zlc.zdqjudy.top

[E15] HTML 转义 / 反转义
来源：http://jhz.guowangkeji.top

Py:   html.escape(s);  html.unescape(s)
来源：http://hub.svipenyu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://eqz.andypj.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lgw.dianchejie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://lji.meibo888.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nod.jinqigfzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kla.zhongyouzk.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lvf.gogol.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lkb.ywan-chungtsiang.top

[E16] 数字千分位
来源：http://oyp.yj20258.top

Py:   f"{1234567:,}"
来源：http://kan.cucudq.cn

PHP:  number_format(1234567);
来源：http://jau.c1oappe.top

JS:   (1234567).toLocaleString("en-US")
来源：http://abi.jiagoushi.top

TS:   (1234567).toLocaleString("en-US")
来源：http://iyz.ppjwa.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vhh.tanke756.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mnr.jinghuilouyu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mjk.shangyingyoupin.top

C#:   1234567.ToString("N0")
来源：http://ogq.pycfn.com

[E17] 首字母大写
来源：http://zia.hnqzz.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zma.daria6918.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vrn.zycfv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://czb.xuanzx.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sjz.hnxiangtu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ahr.yfazqb.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://czm.iojbl.cn

Ruby: s.capitalize
来源：http://unt.bbcook.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vsp.fanxiaobao.xyz

[E18] 模板占位符替换
来源：http://bmf.jlsjyb.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://owr.ydzc1.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cyt.xinyue.icu

JS:   tpl.replaceAll("{name}", name)
来源：http://fms.havefunace.top

TS:   tpl.replaceAll("{name}", name)
来源：http://nyr.meibo888.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://khh.ywan-chungtsiang.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ooy.ctjpmb.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mpw.shanyushiyangkeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jsr.yj20258888.top

[E19] 多行文本按行拆分
来源：http://xiy.zdqjudy.top

Py:   s.splitlines()
来源：http://qpt.nwbrower.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zmk.cashguo.top

JS:   s.split(/\r?\n/)
来源：http://vab.fanxiaobao.xyz

TS:   s.split(/\r?\n/)
来源：http://wsz.tanke756.top

Java: s.lines().toList()
来源：http://rxr.svipenyu.cn

Go:   strings.Split(s, "\n")
来源：http://ohy.jqgfzy.top

Ruby: s.lines
来源：http://vzl.ivvv.top

C#:   s.Split('\n')
来源：http://tqy.nanxuanxn.top

[E20] 判断字符串是否为空
来源：http://vbk.hnxiangtu.top

Py:   if not s:
来源：http://rle.epnwcf.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dqo.yj202588.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lmo.ppjwa.cn

TS:   if (s === "") {}
来源：http://vxg.shangyingyoupin.top

Java: if (s.isEmpty()) {}
来源：http://nnm.shanyushiyangkeji.top

Go:   if s == "" {}
来源：http://daf.shanyushiyangkeji.top

Ruby: if s.empty?
来源：http://fhx.fehbvm.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gfk.shanyushiyangtech.top

[E21] 超长截断加省略号
来源：http://rjn.aibaodan.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://llv.shzxlz.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hqk.yj20258.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lrd.jinqigfzy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vvi.fanxiaobao.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bjq.yj202588.top

Go:   // 按 rune 判断长度后截断
来源：http://kqt.nwbrower.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lgv.ivvv.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://omq.aizwys.cn

[E22] 字节长度与字符长度
来源：http://sda.yanxiufei.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xog.c1oappe.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://opv.jlsjyb.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ljo.fengsongda.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://iwa.zycfv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hti.fengsongda.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://esd.52xcode.cn

Ruby: s.bytesize;  s.length
来源：http://rqc.yj20258888.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://unz.shangyingyoupin.top

================================================================================
来源：http://ofu.gaohongyu789.top

F. 文件与目录
来源：http://cug.havefunace.top

================================================================================
来源：http://vfa.gzhubu.top

[F01] 读取整个文件
来源：http://ory.cucudq.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ikn.yongpay.top

PHP:  file_get_contents("a.txt");
来源：http://cbe.bjfxy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hum.sufxvd.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nmh.tianlin.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://kgq.vqdsnc.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kzm.zhengqikj.top

Ruby: File.read("a.txt")
来源：http://otp.hesvh.cn

C#:   File.ReadAllText("a.txt");
来源：http://huj.zycfv.cn

[F02] 逐行读取文件
来源：http://iwn.cdnleiting.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tyf.hysaishi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mxi.meibo888.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://evg.xuanzx.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vhm.daria6918.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mus.fengsongda.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mfx.fanxiaobao.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nrp.yangfankeji.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hzp.zhengqikj.top

[F03] 写入文件（覆盖）
来源：http://qut.xinyue.icu

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://laj.havefunace.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://xhw.cucudq.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ulv.jianghu66.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hmh.hongshengwenyu.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sjw.gaohongyu789.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ngp.gzhubu.top

Ruby: File.write("a.txt", "hi")
来源：http://jjn.jinqigufen.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qck.tanke756.top

[F04] 追加写入文件
来源：http://ovd.yuanzhike.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vrb.xylfe.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://obz.yongpay.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aql.yueranfly.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rlm.zdbjq.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hct.havefunace.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sdo.wangshuangyany.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rhy.epnwcf.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rqw.xinyue.icu

[F05] 判断文件或目录是否存在
来源：http://zns.zdbjq.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nww.fzhhl.top

PHP:  file_exists("a.txt");
来源：http://ogy.wangdashe.top

JS:   fs.existsSync("a.txt")
来源：http://bmj.ywan-chungtsiang.top

TS:   fs.existsSync("a.txt")
来源：http://jmq.cashguo.top

Java: Files.exists(Path.of("a.txt"))
来源：http://oiy.quarkkingdee.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vhb.wangdashe.top

Ruby: File.exist?("a.txt")
来源：http://qdo.hfpthk.cn

C#:   File.Exists("a.txt")
来源：http://gzg.cheryme.top

[F06] 删除文件
来源：http://ggr.gogol.net.cn

Py:   os.remove("a.txt")
来源：http://qwj.ydzc1.top

PHP:  unlink("a.txt");
来源：http://adk.hammf.cn

JS:   fs.unlinkSync("a.txt")
来源：http://duy.yuxming.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ivb.fengsongda.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gum.yj20258.top

Go:   os.Remove("a.txt")
来源：http://nrc.uphjek.com

Ruby: File.delete("a.txt")
来源：http://pcc.feifeiyinyue.top

C#:   File.Delete("a.txt");
来源：http://kin.ctjpmb.com

[F07] 创建目录（含多级）
来源：http://uzf.ywan-chungtsiang.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xji.yuxming.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wrh.gzhubu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ydi.andypj.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mjv.sufxvd.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xna.zhaomingkeji.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pox.yj20258888.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gbd.nanxuanxn.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qua.yangfankeji.com

[F08] 遍历目录
来源：http://gby.52xcode.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://spu.hesvh.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lwq.tarul.cn

JS:   fs.readdirSync("dir")
来源：http://gke.yuxming.cn

TS:   fs.readdirSync("dir")
来源：http://xwg.haohaochexian.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ovq.guowangkeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ago.jinghuilouyu.cn

Ruby: Dir.children("dir")
来源：http://ffi.shanyushiyangtech.top

C#:   Directory.GetFiles("dir")
来源：http://jki.sxryk.cn

[F09] 获取文件大小
来源：http://ebh.yanxiufei.cn

Py:   os.path.getsize("a.txt")
来源：http://yps.zhijiandao.cn

PHP:  filesize("a.txt");
来源：http://qbz.cashguo.top

JS:   fs.statSync("a.txt").size
来源：http://xar.smart0.xyz

TS:   fs.statSync("a.txt").size
来源：http://idi.havefunace.top

Java: Files.size(Path.of("a.txt"))
来源：http://uqq.zhiwuduotai.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ytz.cashguo.top

Ruby: File.size("a.txt")
来源：http://myp.xinyue.icu

C#:   new FileInfo("a.txt").Length
来源：http://zms.wangdashe.top

[F10] 取文件扩展名 / 文件名
来源：http://zku.yuxming.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hke.yanxiufei.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://unj.svipenyu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cxq.nanxuanxn.top

TS:   path.extname("a.txt")
来源：http://nkw.chenlongwang.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jyd.havefunace.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://aqe.9152youxi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rwa.chenzaomai.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ikj.vqdsnc.cn

[F11] 复制与移动文件
来源：http://bvj.vehdjk.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zgn.ehwqpu.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yot.zhoulong.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rvi.quarkkingdee.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jzw.ydjk.org.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uwj.tian-w.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gct.chenzaomai.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cqa.tianlin.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ymn.zhoulong.xyz

[F12] CSV 读写
来源：http://sih.wangshuangyany.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vgb.hnxiangtu.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ywc.aizwys.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jcc.bjfxy.top

TS:   // 同上
来源：http://drd.sweek.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://enf.0kj1m.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ekr.hnqzz.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hdm.shangyingyoupin.top

C#:   // 无内置：用 CsvHelper 库
来源：http://mdr.tarul.cn

================================================================================
来源：http://fvz.ppjwa.cn

G. 面向对象
来源：http://wrn.xingfuxueyuan.xyz

================================================================================
来源：http://xsd.yj202588.top

[G01] 定义类
来源：http://bjv.jqgfzy.top

Py:   class User: pass
来源：http://xwt.yj20258.top

PHP:  class User {}
来源：http://rir.tianlin.xyz

JS:   class User {}
来源：http://glc.hywenlv.cn

TS:   class User { name: string = ""; }
来源：http://moi.zhoulong.xyz

Java: class User {}
来源：http://cff.pycfn.com

Go:   type User struct { Name string }
来源：http://ylq.zdqjudy.top

Ruby: class User; end
来源：http://lft.shanyushiyangtech.top

C#:   class User {}
来源：http://zew.haohaochexian.top

[G02] 构造函数
来源：http://kqk.feifeiyinyue.top

Py:   def __init__(self, name): self.name = name
来源：http://ypd.dashuyun.cn

PHP:  public function __construct(public string $name) {}
来源：http://dyl.ydjk.org.cn

JS:   constructor(name) { this.name = name; }
来源：http://uie.gotoacloud.top

TS:   constructor(public name: string) {}
来源：http://etb.52xcode.cn

Java: User(String name) { this.name = name; }
来源：http://uqk.andypj.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://upv.tanke756.top

Ruby: def initialize(name); @name = name; end
来源：http://pbc.guannengcc.top

C#:   public User(string name) { Name = name; }
来源：http://awu.ehwqpu.com

[G03] 实例属性
来源：http://vis.shangyingyoupin.top

Py:   self.name = "x"
来源：http://bak.tian-w.cn

PHP:  public string $name = "x";
来源：http://jsj.zdqjudy.top

JS:   this.name = "x";
来源：http://syf.kuanghao11.cn

TS:   name: string = "x";
来源：http://wmh.pengpengdd.cyou

Java: private String name;
来源：http://hkg.tian-w.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fiw.fengsongda.top

Ruby: @name = "x"
来源：http://wmc.316326.xyz

C#:   public string Name { get; set; } = "x";
来源：http://lpk.shangyingyoupin.top

[G04] 定义方法
来源：http://qfm.mhx1999.top

Py:   def greet(self): return self.name
来源：http://swd.vqdsnc.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://crb.jinghuilouyu.cn

JS:   greet() { return this.name; }
来源：http://gwi.jqgufenzy.top

TS:   greet(): string { return this.name; }
来源：http://ukt.iojbl.cn

Java: String greet() { return name; }
来源：http://wpl.hfpthk.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xtf.c1oappe.top

Ruby: def greet; @name; end
来源：http://uqr.zhixingplan.top

C#:   public string Greet() => Name;
来源：http://ojd.hesvh.cn

[G05] 继承
来源：http://cyk.shangyingyoupin.top

Py:   class Admin(User): pass
来源：http://wzb.aizwys.cn

PHP:  class Admin extends User {}
来源：http://tgq.andypj.xyz

JS:   class Admin extends User {}
来源：http://jvb.fktsv.cn

TS:   class Admin extends User {}
来源：http://rdj.dashuyun.cn

Java: class Admin extends User {}
来源：http://iln.yj202588.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gup.shanyushiyangkeji.top

Ruby: class Admin < User; end
来源：http://thi.nanxuanxn.top

C#:   class Admin : User {}
来源：http://azy.jqgufenzy.top

[G06] 重写方法
来源：http://ecc.hesvh.cn

Py:   def greet(self): return "admin"
来源：http://dei.zhixingplan.top

PHP:  public function greet(): string { return "admin"; }
来源：http://eky.tian-w.cn

JS:   greet() { return "admin"; }
来源：http://oen.zhaomingkeji.xyz

TS:   greet(): string { return "admin"; }
来源：http://mpc.epnwcf.com

Java: @Override String greet() { return "admin"; }
来源：http://jlk.jlsjyb.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gxz.zhiwuduotai.top

Ruby: def greet; "admin"; end
来源：http://lkb.cashguo.top


<!-- 参考信息 -->