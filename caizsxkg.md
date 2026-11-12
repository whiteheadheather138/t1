代发 wailian999

PHP:  implode(",", $items);
来源：http://atc.xziqi.cn

JS:   items.join(",")
来源：http://ppm.ctjpmb.com

TS:   items.join(",")
来源：http://wok.cucudq.cn

Java: String.join(",", items)
来源：http://soz.sufxvd.cn

Go:   strings.Join(items, ",")
来源：http://muc.hcnkem.com

Ruby: items.join(",")
来源：http://qbp.shanyushiyangtech.top

C#:   string.Join(",", items)
来源：http://vmy.dashuyun.cn

[E09] 去除所有空白字符
来源：http://fak.haohaochexian.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kuy.nanxuanxn.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qtc.havefunace.top

JS:   s.replace(/\s+/g, "")
来源：http://kwy.bjfxy.top

TS:   s.replace(/\s+/g, "")
来源：http://klz.fanxiaobao.xyz

Java: s.replaceAll("\\s+", "")
来源：http://syd.xziqi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://joz.chenjidiqi.icu

Ruby: s.gsub(/\s+/, "")
来源：http://ian.andypj.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kxl.jqgfzy.top

[E10] 左侧补零 / 定长填充
来源：http://hin.hywenlv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mnd.hcnkem.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vav.daxiang520.top

JS:   "7".padStart(3, "0")
来源：http://bug.yuxming.cn

TS:   "7".padStart(3, "0")
来源：http://xcx.quarkkingdee.top

Java: String.format("%03d", 7)
来源：http://daq.fanxiaobao.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://gqb.gaohongyu789.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fgb.gaohongyu789.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://znt.xziqi.cn

[E11] 反转字符串
来源：http://npw.zhiwuduotai.top

Py:   s[::-1]
来源：http://azf.0kj1m.cn

PHP:  strrev($s);
来源：http://lox.jqgfzy.top

JS:   [...s].reverse().join("")
来源：http://htc.epnwcf.com

TS:   [...s].reverse().join("")
来源：http://uwe.ydjk.org.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mqf.xylfe.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://aaa.yj202588.top

Ruby: s.reverse
来源：http://mcg.fanxiaobao.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://ykv.sweek.top

[E12] 统计某字符出现次数
来源：http://cbi.gotoacloud.top

Py:   s.count("a")
来源：http://vnn.hnxiangtu.top

PHP:  substr_count($s, "a");
来源：http://kqf.9152youxi.cn

JS:   s.split("a").length - 1
来源：http://wfm.hnxiangtu.top

TS:   s.split("a").length - 1
来源：http://gwq.sjlbkw.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://esq.birdmap.top

Go:   strings.Count(s, "a")
来源：http://ooe.tarul.cn

Ruby: s.count("a")
来源：http://wdh.yj20258.top

C#:   s.Count(c => c == 'a')
来源：http://lvc.pengpengdd.cyou

[E13] 逐字符遍历
来源：http://bzn.hammf.cn

Py:   for ch in s: print(ch)
来源：http://qdt.havefunace.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dcn.yfazqb.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://nnw.fktsv.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bix.pycfn.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jqo.vehdjk.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ldf.ydzc1.top

Ruby: s.each_char { |ch| puts ch }
来源：http://poh.sjlbkw.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sar.cashguo.top

[E14] URL 编码与 Base64
来源：http://myw.nanxuanxn.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yky.yuanzhike.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://dxi.gzhubu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dav.shzxlz.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pgq.yfazqb.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ldi.c1oappe.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://foy.vqdsnc.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://abl.jinghuilouyu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ynd.ydzc1.top

[E15] HTML 转义 / 反转义
来源：http://ypb.redwolf501.top

Py:   html.escape(s);  html.unescape(s)
来源：http://vic.hcnkem.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vno.pengpengdd.cyou

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vgn.hcnkem.com

TS:   // 同上，务必做 XSS 过滤
来源：http://xxw.andypj.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vbz.zhoulong.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yas.xuanzx.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dvq.gaohongyu789.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ajh.cdnleiting.top

[E16] 数字千分位
来源：http://bao.jqgufenzy.top

Py:   f"{1234567:,}"
来源：http://npj.shanyushiyangtech.top

PHP:  number_format(1234567);
来源：http://moe.bbcook.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xsu.fehbvm.com

TS:   (1234567).toLocaleString("en-US")
来源：http://bja.zhixingplan.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mga.xinyue.icu

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://phe.pycfn.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://urt.zhaomingkeji.xyz

C#:   1234567.ToString("N0")
来源：http://qvf.iojbl.cn

[E17] 首字母大写
来源：http://fdm.zhongyouzk.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mly.zhixingplan.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://znm.zhoulong.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dkg.zdqjudy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ymf.cheryme.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dwg.jqgufenzy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gpu.cucudq.cn

Ruby: s.capitalize
来源：http://sgb.daria6918.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rqv.jqgufenzy.top

[E18] 模板占位符替换
来源：http://fht.jinqigufen.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yyh.yvedp.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://iub.tianlin.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://xxg.yuxming.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://wps.jianghu66.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kgr.vqdsnc.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://alm.316326.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://naq.andypj.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hyz.jinghuilouyu.cn

[E19] 多行文本按行拆分
来源：http://rnj.mhx1999.top

Py:   s.splitlines()
来源：http://vep.hcnkem.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mnf.hywenlv.cn

JS:   s.split(/\r?\n/)
来源：http://hqf.jqgufenzy.top

TS:   s.split(/\r?\n/)
来源：http://prn.redwolf501.top

Java: s.lines().toList()
来源：http://zgj.yj20258888.top

Go:   strings.Split(s, "\n")
来源：http://fab.meibo888.top

Ruby: s.lines
来源：http://ykz.shzxlz.cn

C#:   s.Split('\n')
来源：http://asg.shzxlz.cn

[E20] 判断字符串是否为空
来源：http://dbe.dashuyun.cn

Py:   if not s:
来源：http://spj.tarul.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xfz.yuxming.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ovm.ehwqpu.com

TS:   if (s === "") {}
来源：http://epe.gzhubu.top

Java: if (s.isEmpty()) {}
来源：http://xkt.shuidangran.top

Go:   if s == "" {}
来源：http://lgi.epnwcf.com

Ruby: if s.empty?
来源：http://rso.yuxming.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://snx.cashguo.top

[E21] 超长截断加省略号
来源：http://qgk.yj20258.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ccy.yj202588.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://shv.hywenlv.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sak.tianlin.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qgo.zhengqikj.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bkw.zhiwuduotai.top

Go:   // 按 rune 判断长度后截断
来源：http://hes.yuanzhike.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fuw.gogol.net.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xal.ppjwa.cn

[E22] 字节长度与字符长度
来源：http://vsa.jinqigfzy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gej.shzxlz.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qoi.zhongyouzk.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://htj.jinghuilouyu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xsz.jyoumei.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fbs.pengpengdd.cyou

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fhi.xziqi.cn

Ruby: s.bytesize;  s.length
来源：http://kpu.havefunace.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dmw.gotoacloud.top

================================================================================
来源：http://jrp.yfazqb.com

F. 文件与目录
来源：http://lmq.hysaishi.cn

================================================================================
来源：http://jub.bjfxy.top

[F01] 读取整个文件
来源：http://viw.jlsjyb.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lmh.zhixingplan.top

PHP:  file_get_contents("a.txt");
来源：http://wsf.yj202588.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://off.jyoumei.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://psi.nanxinkj.top

Java: Files.readString(Path.of("a.txt"))
来源：http://vco.0kj1m.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xhm.aizwys.cn

Ruby: File.read("a.txt")
来源：http://bfr.meibo888.top

C#:   File.ReadAllText("a.txt");
来源：http://kvl.zhiwuduotai.top

[F02] 逐行读取文件
来源：http://eel.zdqjudy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ngi.cheryme.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xzs.zhijiandao.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qyt.zhengqikj.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rre.jianghu66.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dzw.bjfxy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://khr.pycfn.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vas.wangshuangyany.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hip.yuxming.cn

[F03] 写入文件（覆盖）
来源：http://npq.gotoacloud.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cgb.havefunace.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ttm.cqqwz.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://usj.316326.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mad.fzhhl.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gsd.ydzc1.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bkt.yj20258.top

Ruby: File.write("a.txt", "hi")
来源：http://xyl.aizwys.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bit.gzhubu.top

[F04] 追加写入文件
来源：http://yrw.xingfuxueyuan.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xnf.52xcode.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mqu.dianchejie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yhb.dianchejie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zys.fktsv.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vwz.xuetiantiany.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lsr.redwolf501.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cfu.tian-w.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jov.ppjwa.cn

[F05] 判断文件或目录是否存在
来源：http://euc.xylfe.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hec.9152youxi.cn

PHP:  file_exists("a.txt");
来源：http://jsj.andypj.xyz

JS:   fs.existsSync("a.txt")
来源：http://acu.snrcjt.cn

TS:   fs.existsSync("a.txt")
来源：http://dpj.zdbjq.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://yyi.xylfe.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mcv.52xcode.cn

Ruby: File.exist?("a.txt")
来源：http://odh.ywan-chungtsiang.top

C#:   File.Exists("a.txt")
来源：http://usr.bbcook.cn

[F06] 删除文件
来源：http://xjj.birdmap.top

Py:   os.remove("a.txt")
来源：http://fia.jianghu66.top

PHP:  unlink("a.txt");
来源：http://tqe.chenlongwang.top

JS:   fs.unlinkSync("a.txt")
来源：http://ewi.hcnkem.com

TS:   fs.unlinkSync("a.txt")
来源：http://xem.chenlongwang.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ket.ydjk.org.cn

Go:   os.Remove("a.txt")
来源：http://xzi.fengsongda.top

Ruby: File.delete("a.txt")
来源：http://rsc.zycfv.cn

C#:   File.Delete("a.txt");
来源：http://tey.yj20258888.top

[F07] 创建目录（含多级）
来源：http://xxt.gaohongyu789.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mbf.yvedp.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ukx.zhongyouzk.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vun.bbcook.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://avw.hongshengwenyu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jeo.jqgfzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dap.zhiwuduotai.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ozi.feifeiyinyue.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wsf.0kj1m.cn

[F08] 遍历目录
来源：http://iug.jyoumei.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://obm.sweek.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ies.tianlin.xyz

JS:   fs.readdirSync("dir")
来源：http://zqb.ivvv.top

TS:   fs.readdirSync("dir")
来源：http://tmk.316326.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xrd.chenzaomai.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://zvd.ppjwa.cn

Ruby: Dir.children("dir")
来源：http://drp.fehbvm.com

C#:   Directory.GetFiles("dir")
来源：http://art.yvedp.cn

[F09] 获取文件大小
来源：http://kgx.shanyushiyangtech.top

Py:   os.path.getsize("a.txt")
来源：http://ejc.zycfv.cn

PHP:  filesize("a.txt");
来源：http://mdl.jinghuilouyu.cn

JS:   fs.statSync("a.txt").size
来源：http://rxz.daria6918.cn

TS:   fs.statSync("a.txt").size
来源：http://kbn.yanxiufei.cn

Java: Files.size(Path.of("a.txt"))
来源：http://sib.sweek.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kcb.ivvv.top

Ruby: File.size("a.txt")
来源：http://pis.yuxming.cn

C#:   new FileInfo("a.txt").Length
来源：http://rjj.zhijiandao.cn

[F10] 取文件扩展名 / 文件名
来源：http://bhg.fktsv.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fqy.c1oappe.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pjt.yfazqb.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tto.sweek.top

TS:   path.extname("a.txt")
来源：http://jdp.cheryme.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ddh.hysaishi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://evh.yongpay.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mkz.gotoacloud.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nsy.zycfv.cn

[F11] 复制与移动文件
来源：http://jct.zhaomingkeji.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xzg.zhaomingkeji.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ruz.hfpthk.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sus.shanyushiyangtech.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pxv.316326.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xvp.nanxinkj.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yyv.haohaochexian.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://adr.tianlin.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bip.jinqigufen.top

[F12] CSV 读写
来源：http://rfl.yongpay.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ebg.cqqwz.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ezb.shanyushiyangtech.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ern.sufxvd.cn

TS:   // 同上
来源：http://iil.bbcook.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dwc.sufxvd.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://eyo.hcnkem.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ypc.xinyue.icu

C#:   // 无内置：用 CsvHelper 库
来源：http://bmq.sysykeji.top

================================================================================
来源：http://jli.xuetiantiany.cn

G. 面向对象
来源：http://jxf.iojbl.cn

================================================================================
来源：http://pef.fzhhl.top

[G01] 定义类
来源：http://mmi.ehwqpu.com

Py:   class User: pass
来源：http://dmf.gogol.net.cn

PHP:  class User {}
来源：http://lis.shzxlz.cn

JS:   class User {}
来源：http://yms.sysykeji.top

TS:   class User { name: string = ""; }
来源：http://wbu.epnwcf.com

Java: class User {}
来源：http://tcl.guannengcc.top

Go:   type User struct { Name string }
来源：http://ufz.xinyue.icu

Ruby: class User; end
来源：http://asr.fktsv.cn

C#:   class User {}
来源：http://sdk.quarkkingdee.top

[G02] 构造函数
来源：http://dev.nanxinkj.top

Py:   def __init__(self, name): self.name = name
来源：http://gwb.shangyingyoupin.top

PHP:  public function __construct(public string $name) {}
来源：http://mdt.aibaodan.cn

JS:   constructor(name) { this.name = name; }
来源：http://zph.smart0.xyz

TS:   constructor(public name: string) {}
来源：http://ijp.ctjpmb.com

Java: User(String name) { this.name = name; }
来源：http://xhm.jyoumei.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qau.aibaodan.cn

Ruby: def initialize(name); @name = name; end
来源：http://zpo.yongpay.top

C#:   public User(string name) { Name = name; }
来源：http://owi.9152youxi.cn

[G03] 实例属性
来源：http://lzv.nanxinkj.top

Py:   self.name = "x"
来源：http://kgs.zhengqikj.top

PHP:  public string $name = "x";
来源：http://wfa.nanxinkj.top

JS:   this.name = "x";
来源：http://qpc.zhaomingkeji.xyz

TS:   name: string = "x";
来源：http://tmx.yfazqb.com

Java: private String name;
来源：http://rpu.jianghu66.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pgb.hywenlv.cn

Ruby: @name = "x"
来源：http://dnp.daxiang520.top

C#:   public string Name { get; set; } = "x";
来源：http://bam.fehbvm.com

[G04] 定义方法
来源：http://ukn.daxiang520.top

Py:   def greet(self): return self.name
来源：http://dtw.yj202588.top

PHP:  public function greet(): string { return $this->name; }
来源：http://qsc.cheryme.top

JS:   greet() { return this.name; }
来源：http://wno.tarul.cn

TS:   greet(): string { return this.name; }
来源：http://dkw.9152youxi.cn

Java: String greet() { return name; }
来源：http://vos.yuxming.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fiu.yj20258.top

Ruby: def greet; @name; end
来源：http://whv.yj20258888.top

C#:   public string Greet() => Name;
来源：http://wbk.sjlbkw.cn

[G05] 继承
来源：http://wwv.shuidangran.top

Py:   class Admin(User): pass
来源：http://lpf.jlsjyb.cn

PHP:  class Admin extends User {}
来源：http://ezg.meibo888.top

JS:   class Admin extends User {}
来源：http://thx.smart0.xyz

TS:   class Admin extends User {}
来源：http://qtx.cashguo.top

Java: class Admin extends User {}
来源：http://jpo.zhiwuduotai.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nem.xuetiantiany.cn

Ruby: class Admin < User; end
来源：http://kpt.wangdashe.top

C#:   class Admin : User {}
来源：http://dbi.birdmap.top

[G06] 重写方法
来源：http://mdc.hfpthk.cn

Py:   def greet(self): return "admin"
来源：http://rqf.chenjidiqi.icu

PHP:  public function greet(): string { return "admin"; }
来源：http://aau.tanke756.top

JS:   greet() { return "admin"; }
来源：http://ihe.havefunace.top

TS:   greet(): string { return "admin"; }
来源：http://tac.nanxinkj.top

Java: @Override String greet() { return "admin"; }
来源：http://wuu.cheryme.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bzv.jinghuilouyu.cn

Ruby: def greet; "admin"; end
来源：http://hqd.xingfuxueyuan.xyz


<!-- 参考信息 -->