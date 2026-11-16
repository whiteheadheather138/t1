代发 wailian999

Ruby: s.split(",");  s.split
来源：http://bkr.hnxiangtu.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dyu.wangdashe.top

[E08] 数组按分隔符合并
来源：http://vfk.ybcxt.top

Py:   ",".join(items)
来源：http://ebt.feifeiyinyue.top

PHP:  implode(",", $items);
来源：http://kwp.jinqigfzy.top

JS:   items.join(",")
来源：http://wwl.tianlin.xyz

TS:   items.join(",")
来源：http://ngz.svipenyu.cn

Java: String.join(",", items)
来源：http://rgx.jyoumei.cn

Go:   strings.Join(items, ",")
来源：http://zom.feifeiyinyue.top

Ruby: items.join(",")
来源：http://ycl.xinyue.icu

C#:   string.Join(",", items)
来源：http://fmi.hywenlv.cn

[E09] 去除所有空白字符
来源：http://mvc.hongshengwenyu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jhh.havefunace.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wjw.redwolf501.top

JS:   s.replace(/\s+/g, "")
来源：http://yjd.shanyushiyangtech.top

TS:   s.replace(/\s+/g, "")
来源：http://dyb.smart0.xyz

Java: s.replaceAll("\\s+", "")
来源：http://eve.ywan-chungtsiang.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://fri.pengpengdd.cyou

Ruby: s.gsub(/\s+/, "")
来源：http://lmk.jinqigufen.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ttg.andypj.xyz

[E10] 左侧补零 / 定长填充
来源：http://dew.jinqigfzy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cne.guannengcc.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://osl.xingfuxueyuan.xyz

JS:   "7".padStart(3, "0")
来源：http://pgt.cashguo.top

TS:   "7".padStart(3, "0")
来源：http://pjy.quarkkingdee.top

Java: String.format("%03d", 7)
来源：http://xtu.mhx1999.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://oqd.shangyingyoupin.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zog.gaohongyu789.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wjk.zdqjudy.top

[E11] 反转字符串
来源：http://tii.nanxinkj.top

Py:   s[::-1]
来源：http://mqt.yonumen.top

PHP:  strrev($s);
来源：http://lts.hongshengwenyu.top

JS:   [...s].reverse().join("")
来源：http://xbl.epnwcf.com

TS:   [...s].reverse().join("")
来源：http://eif.cdnleiting.top

Java: new StringBuilder(s).reverse().toString()
来源：http://hvv.zhiwuduotai.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://sgl.daria6918.cn

Ruby: s.reverse
来源：http://raw.yj20258.top

C#:   new string(s.Reverse().ToArray())
来源：http://yth.quarkkingdee.top

[E12] 统计某字符出现次数
来源：http://dpc.sufxvd.cn

Py:   s.count("a")
来源：http://zsk.quarkkingdee.top

PHP:  substr_count($s, "a");
来源：http://tym.shanyushiyangkeji.top

JS:   s.split("a").length - 1
来源：http://xuq.ybcxt.top

TS:   s.split("a").length - 1
来源：http://qmd.yonumen.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dhi.fktsv.cn

Go:   strings.Count(s, "a")
来源：http://shv.epnwcf.com

Ruby: s.count("a")
来源：http://das.jyoumei.cn

C#:   s.Count(c => c == 'a')
来源：http://jew.birdmap.top

[E13] 逐字符遍历
来源：http://bva.ydzc1.top

Py:   for ch in s: print(ch)
来源：http://ssb.meibo888.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yez.wangshuangyany.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qju.kuanghao11.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://luc.wangdashe.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://aff.daxiang520.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qdt.shuidangran.top

Ruby: s.each_char { |ch| puts ch }
来源：http://aed.cdnleiting.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://irm.yonumen.top

[E14] URL 编码与 Base64
来源：http://qbg.hysaishi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cla.zdqjudy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://qrg.fengsongda.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zol.ybcxt.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dct.yfazqb.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://plr.uphjek.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kew.daria6918.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qls.xylfe.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mad.cheryme.top

[E15] HTML 转义 / 反转义
来源：http://fwf.uphjek.com

Py:   html.escape(s);  html.unescape(s)
来源：http://inq.shuidangran.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ngh.jqgfzy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yxy.aibaodan.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://rca.andypj.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wgs.zycfv.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://oxt.hywenlv.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qjc.guannengcc.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://clx.guannengcc.top

[E16] 数字千分位
来源：http://anb.hysaishi.cn

Py:   f"{1234567:,}"
来源：http://ywp.cucudq.cn

PHP:  number_format(1234567);
来源：http://ukk.snrcjt.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://kvt.cucudq.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://taw.wangdashe.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://isb.uphjek.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://joe.zhijiandao.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://chs.xinyue.icu

C#:   1234567.ToString("N0")
来源：http://bhl.zdqjudy.top

[E17] 首字母大写
来源：http://urf.jqgufenzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://krw.yj20258888.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ftb.gzhubu.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ere.sysykeji.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fzu.316326.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cbr.jianghu66.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wto.yj202588.top

Ruby: s.capitalize
来源：http://zzy.0kj1m.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nhc.ppjwa.cn

[E18] 模板占位符替换
来源：http://xjr.ydzc1.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://buu.jqgfzy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sru.jiagoushi.top

JS:   tpl.replaceAll("{name}", name)
来源：http://nqt.sjlbkw.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://mhx.hywenlv.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qkk.chenzaomai.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lps.redwolf501.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cky.ppjwa.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kuf.shuidangran.top

[E19] 多行文本按行拆分
来源：http://dko.zhiwuduotai.top

Py:   s.splitlines()
来源：http://kbl.dianchejie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pez.hesvh.cn

JS:   s.split(/\r?\n/)
来源：http://xpt.bjfxy.top

TS:   s.split(/\r?\n/)
来源：http://xxd.yangfankeji.com

Java: s.lines().toList()
来源：http://fcf.zhaomingkeji.xyz

Go:   strings.Split(s, "\n")
来源：http://pwf.xuetiantiany.cn

Ruby: s.lines
来源：http://fxf.daxiang520.top

C#:   s.Split('\n')
来源：http://nvo.daxiang520.top

[E20] 判断字符串是否为空
来源：http://jki.uphjek.com

Py:   if not s:
来源：http://tah.yonumen.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zyn.yonumen.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tkh.dashuyun.cn

TS:   if (s === "") {}
来源：http://asf.xinyue.icu

Java: if (s.isEmpty()) {}
来源：http://ist.guannengcc.top

Go:   if s == "" {}
来源：http://kdr.hongshengwenyu.top

Ruby: if s.empty?
来源：http://hxk.smart0.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ioe.epnwcf.com

[E21] 超长截断加省略号
来源：http://efe.fktsv.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xqm.chenzaomai.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cvv.chenjidiqi.icu

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cai.yj20258.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mql.redwolf501.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://toa.jinyuanbaomall.cn

Go:   // 按 rune 判断长度后截断
来源：http://xav.epnwcf.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cir.nanxinkj.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mrs.sysykeji.top

[E22] 字节长度与字符长度
来源：http://mwc.fanxiaobao.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://trg.ehwqpu.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yhy.ybcxt.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vky.fengsongda.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tvh.havefunace.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cbl.hammf.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bkk.yonumen.top

Ruby: s.bytesize;  s.length
来源：http://vnj.quarkkingdee.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://swy.hammf.cn

================================================================================
来源：http://mag.gotoacloud.top

F. 文件与目录
来源：http://eed.pycfn.com

================================================================================
来源：http://zci.hywenlv.cn

[F01] 读取整个文件
来源：http://sqs.hysaishi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://klw.quarkkingdee.top

PHP:  file_get_contents("a.txt");
来源：http://zfm.9152youxi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vkf.hfpthk.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tec.fehbvm.com

Java: Files.readString(Path.of("a.txt"))
来源：http://fon.vqdsnc.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xyk.ctjpmb.com

Ruby: File.read("a.txt")
来源：http://sqp.vehdjk.com

C#:   File.ReadAllText("a.txt");
来源：http://aiz.sufxvd.cn

[F02] 逐行读取文件
来源：http://ewn.sufxvd.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dbh.hongshengwenyu.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ecg.shanyushiyangtech.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kde.tarul.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://smc.sufxvd.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xwz.shzxlz.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ggf.pycfn.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://drc.shanyushiyangtech.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jkm.gzhubu.top

[F03] 写入文件（覆盖）
来源：http://urd.nanxinkj.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pkf.yuanzhike.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://cxt.pycfn.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://icx.yonumen.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bip.cdnleiting.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vag.hysaishi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wrs.ybcxt.top

Ruby: File.write("a.txt", "hi")
来源：http://kah.yonumen.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ouw.daxiang520.top

[F04] 追加写入文件
来源：http://zfi.yfazqb.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ugw.hesvh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ybg.fktsv.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bow.zdbjq.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://afm.xziqi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kpc.316326.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ynw.nanxinkj.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://erj.zhoulong.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bqn.hfpthk.cn

[F05] 判断文件或目录是否存在
来源：http://zis.yuxming.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vcc.vqdsnc.cn

PHP:  file_exists("a.txt");
来源：http://itb.daxiang520.top

JS:   fs.existsSync("a.txt")
来源：http://foo.ppjwa.cn

TS:   fs.existsSync("a.txt")
来源：http://sdk.fktsv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wlh.fzhhl.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sqg.meibo888.top

Ruby: File.exist?("a.txt")
来源：http://gob.snrcjt.cn

C#:   File.Exists("a.txt")
来源：http://jgx.mhx1999.top

[F06] 删除文件
来源：http://iam.0kj1m.cn

Py:   os.remove("a.txt")
来源：http://hwl.zhixingplan.top

PHP:  unlink("a.txt");
来源：http://ogd.ybcxt.top

JS:   fs.unlinkSync("a.txt")
来源：http://sjt.nanxinkj.top

TS:   fs.unlinkSync("a.txt")
来源：http://sof.yonumen.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qoq.nanxuanxn.top

Go:   os.Remove("a.txt")
来源：http://lfg.ppjwa.cn

Ruby: File.delete("a.txt")
来源：http://amb.hywenlv.cn

C#:   File.Delete("a.txt");
来源：http://hkg.cheryme.top

[F07] 创建目录（含多级）
来源：http://vye.zdbjq.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cho.hnxiangtu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ibq.hesvh.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nhg.ywan-chungtsiang.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ibg.zhiwuduotai.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wis.fanxiaobao.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gyv.zdbjq.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nhz.9152youxi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jnr.yj20258.top

[F08] 遍历目录
来源：http://zen.zhijiandao.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ybr.yongpay.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://iaf.ppjwa.cn

JS:   fs.readdirSync("dir")
来源：http://wwp.fengsongda.top

TS:   fs.readdirSync("dir")
来源：http://ejq.jinqigfzy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://soj.ybcxt.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://xhp.zycfv.cn

Ruby: Dir.children("dir")
来源：http://fnw.gogol.net.cn

C#:   Directory.GetFiles("dir")
来源：http://wko.fanxiaobao.xyz

[F09] 获取文件大小
来源：http://ljb.birdmap.top

Py:   os.path.getsize("a.txt")
来源：http://zms.hongshengwenyu.top

PHP:  filesize("a.txt");
来源：http://qwr.jqgfzy.top

JS:   fs.statSync("a.txt").size
来源：http://ckm.tianlin.xyz

TS:   fs.statSync("a.txt").size
来源：http://dis.chenlongwang.top

Java: Files.size(Path.of("a.txt"))
来源：http://qjt.yonumen.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://puw.tanke756.top

Ruby: File.size("a.txt")
来源：http://xmz.cdnleiting.top

C#:   new FileInfo("a.txt").Length
来源：http://snp.ydzc1.top

[F10] 取文件扩展名 / 文件名
来源：http://zeo.zhijiandao.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cif.hysaishi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uur.quarkkingdee.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qum.hesvh.cn

TS:   path.extname("a.txt")
来源：http://cgj.xinyue.icu

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wio.sweek.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jbf.chenlongwang.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://auq.guowangkeji.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://eil.daxiang520.top

[F11] 复制与移动文件
来源：http://car.hnxiangtu.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wzx.yj202588.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lwr.ydzc1.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uto.tanke756.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rxz.dashuyun.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zzk.shuidangran.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://aku.jqgufenzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cca.hywenlv.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ros.kuanghao11.cn

[F12] CSV 读写
来源：http://hsg.jinyuanbaomall.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tpu.jinghuilouyu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vgb.ivvv.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yuj.fanxiaobao.xyz

TS:   // 同上
来源：http://knh.zhengqikj.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://idl.yueranfly.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mko.meibo888.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hfr.gotoacloud.top

C#:   // 无内置：用 CsvHelper 库
来源：http://azp.pycfn.com

================================================================================
来源：http://rxc.zhaomingkeji.xyz

G. 面向对象
来源：http://qje.shuidangran.top

================================================================================
来源：http://kut.shuidangran.top

[G01] 定义类
来源：http://sng.mhx1999.top

Py:   class User: pass
来源：http://omc.pycfn.com

PHP:  class User {}
来源：http://jtt.sjlbkw.cn

JS:   class User {}
来源：http://bpt.xinyue.icu

TS:   class User { name: string = ""; }
来源：http://myo.jqgufenzy.top

Java: class User {}
来源：http://mng.aizwys.cn

Go:   type User struct { Name string }
来源：http://yft.hongshengwenyu.top

Ruby: class User; end
来源：http://efh.fzhhl.top

C#:   class User {}
来源：http://hhv.ywan-chungtsiang.top

[G02] 构造函数
来源：http://uhv.9152youxi.cn

Py:   def __init__(self, name): self.name = name
来源：http://kju.feifeiyinyue.top

PHP:  public function __construct(public string $name) {}
来源：http://wym.yj20258.top

JS:   constructor(name) { this.name = name; }
来源：http://oqs.pycfn.com

TS:   constructor(public name: string) {}
来源：http://kww.tian-w.cn

Java: User(String name) { this.name = name; }
来源：http://uke.shangyingyoupin.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pnd.hysaishi.cn

Ruby: def initialize(name); @name = name; end
来源：http://obc.guannengcc.top

C#:   public User(string name) { Name = name; }
来源：http://iuw.fktsv.cn

[G03] 实例属性
来源：http://khc.xingfuxueyuan.xyz

Py:   self.name = "x"
来源：http://fob.cheryme.top

PHP:  public string $name = "x";
来源：http://hny.vqdsnc.cn

JS:   this.name = "x";
来源：http://tfl.zhijiandao.cn

TS:   name: string = "x";
来源：http://elo.yfazqb.com

Java: private String name;
来源：http://bgd.svipenyu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jqh.c1oappe.top

Ruby: @name = "x"
来源：http://jkb.yfazqb.com

C#:   public string Name { get; set; } = "x";
来源：http://fup.xingfuxueyuan.xyz

[G04] 定义方法
来源：http://ezb.chenzaomai.com

Py:   def greet(self): return self.name
来源：http://yub.andypj.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://kll.birdmap.top

JS:   greet() { return this.name; }
来源：http://bfc.jiagoushi.top

TS:   greet(): string { return this.name; }
来源：http://zit.zycfv.cn

Java: String greet() { return name; }
来源：http://wyg.feifeiyinyue.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://wgh.jinyuanbaomall.cn

Ruby: def greet; @name; end
来源：http://xgb.cqqwz.cn

C#:   public string Greet() => Name;
来源：http://dzb.52xcode.cn

[G05] 继承
来源：http://oji.zhiwuduotai.top

Py:   class Admin(User): pass
来源：http://cny.zhoulong.xyz

PHP:  class Admin extends User {}
来源：http://clq.aibaodan.cn

JS:   class Admin extends User {}
来源：http://gbg.ehwqpu.com

TS:   class Admin extends User {}
来源：http://ytt.epnwcf.com

Java: class Admin extends User {}
来源：http://fek.xziqi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vxu.yangfankeji.com

Ruby: class Admin < User; end
来源：http://fvj.zhaomingkeji.xyz

C#:   class Admin : User {}
来源：http://utk.yj20258888.top

[G06] 重写方法
来源：http://eom.yanxiufei.cn

Py:   def greet(self): return "admin"
来源：http://amr.xziqi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mqs.jianghu66.top

JS:   greet() { return "admin"; }
来源：http://xla.epnwcf.com


<!-- 参考信息 -->