代发 wailian999

PHP:  implode(",", $items);
来源：http://isy.fzhhl.top

JS:   items.join(",")
来源：http://sik.guannengcc.top

TS:   items.join(",")
来源：http://nbz.wangdashe.top

Java: String.join(",", items)
来源：http://icv.yj20258.top

Go:   strings.Join(items, ",")
来源：http://otn.chenzaomai.com

Ruby: items.join(",")
来源：http://olg.birdmap.top

C#:   string.Join(",", items)
来源：http://nnl.guowangkeji.top

[E09] 去除所有空白字符
来源：http://wlx.kuanghao11.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wwy.pycfn.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vpy.xingfuxueyuan.xyz

JS:   s.replace(/\s+/g, "")
来源：http://uhu.jinghuilouyu.cn

TS:   s.replace(/\s+/g, "")
来源：http://kzt.c1oappe.top

Java: s.replaceAll("\\s+", "")
来源：http://nam.sysykeji.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://qia.xuanzx.com

Ruby: s.gsub(/\s+/, "")
来源：http://iqz.guannengcc.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ese.kuanghao11.cn

[E10] 左侧补零 / 定长填充
来源：http://trp.zdqjudy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tqm.chenlongwang.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ohp.xuetiantiany.cn

JS:   "7".padStart(3, "0")
来源：http://ofe.hfpthk.cn

TS:   "7".padStart(3, "0")
来源：http://ayy.pengpengdd.cyou

Java: String.format("%03d", 7)
来源：http://bgw.fanxiaobao.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://rzn.hnqzz.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://aiz.jiagoushi.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://brq.chenjidiqi.icu

[E11] 反转字符串
来源：http://uks.snrcjt.cn

Py:   s[::-1]
来源：http://jiz.yueranfly.top

PHP:  strrev($s);
来源：http://cqp.yueranfly.top

JS:   [...s].reverse().join("")
来源：http://eda.smart0.xyz

TS:   [...s].reverse().join("")
来源：http://wos.jqgufenzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://yjd.wangdashe.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://afp.hcnkem.com

Ruby: s.reverse
来源：http://vpo.fktsv.cn

C#:   new string(s.Reverse().ToArray())
来源：http://cch.jinghuilouyu.cn

[E12] 统计某字符出现次数
来源：http://ekf.shuidangran.top

Py:   s.count("a")
来源：http://awk.pengpengdd.cyou

PHP:  substr_count($s, "a");
来源：http://ejr.xuanzx.com

JS:   s.split("a").length - 1
来源：http://qtm.sufxvd.cn

TS:   s.split("a").length - 1
来源：http://tnb.gzhubu.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://our.sxryk.cn

Go:   strings.Count(s, "a")
来源：http://jvu.jinqigfzy.top

Ruby: s.count("a")
来源：http://ork.epnwcf.com

C#:   s.Count(c => c == 'a')
来源：http://nix.bbcook.cn

[E13] 逐字符遍历
来源：http://jcx.xuetiantiany.cn

Py:   for ch in s: print(ch)
来源：http://npu.jqgfzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mgx.yvedp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://mxv.52xcode.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://iuq.shanyushiyangkeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wgn.gogol.net.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://azi.yfazqb.com

Ruby: s.each_char { |ch| puts ch }
来源：http://zoy.52xcode.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dpm.316326.xyz

[E14] URL 编码与 Base64
来源：http://rom.shzxlz.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wvs.aibaodan.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://nal.sweek.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ary.uphjek.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://quq.pycfn.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xya.shzxlz.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://djw.zhixingplan.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fky.cdnleiting.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rjs.zdbjq.cn

[E15] HTML 转义 / 反转义
来源：http://oor.fehbvm.com

Py:   html.escape(s);  html.unescape(s)
来源：http://yla.yj20258.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qlm.ydzc1.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qjz.jianghu66.top

TS:   // 同上，务必做 XSS 过滤
来源：http://tah.yvedp.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wsk.jiagoushi.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vuj.fktsv.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bkv.epnwcf.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ear.yangfankeji.com

[E16] 数字千分位
来源：http://sfm.52xcode.cn

Py:   f"{1234567:,}"
来源：http://cal.jqgufenzy.top

PHP:  number_format(1234567);
来源：http://qnq.yj20258.top

JS:   (1234567).toLocaleString("en-US")
来源：http://oij.feifeiyinyue.top

TS:   (1234567).toLocaleString("en-US")
来源：http://stw.cdnleiting.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rbt.fzhhl.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://clx.tarul.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://loa.aibaodan.cn

C#:   1234567.ToString("N0")
来源：http://xmc.hysaishi.cn

[E17] 首字母大写
来源：http://lcn.jinqigfzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cyi.yanxiufei.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pxu.zhongyouzk.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nlp.pycfn.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mfn.wangshuangyany.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lcu.hammf.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rba.jqgufenzy.top

Ruby: s.capitalize
来源：http://enh.iojbl.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ggu.xinyue.icu

[E18] 模板占位符替换
来源：http://pbu.yuxming.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ofv.haohaochexian.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vsb.xinyue.icu

JS:   tpl.replaceAll("{name}", name)
来源：http://zsp.jiagoushi.top

TS:   tpl.replaceAll("{name}", name)
来源：http://zul.jinqigufen.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dgn.meibo888.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hse.fanxiaobao.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xgi.jinghuilouyu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wct.xinyue.icu

[E19] 多行文本按行拆分
来源：http://xwu.hfpthk.cn

Py:   s.splitlines()
来源：http://foi.c1oappe.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jix.yueranfly.top

JS:   s.split(/\r?\n/)
来源：http://bha.daria6918.cn

TS:   s.split(/\r?\n/)
来源：http://lfb.bbcook.cn

Java: s.lines().toList()
来源：http://gul.ppjwa.cn

Go:   strings.Split(s, "\n")
来源：http://wvr.ivvv.top

Ruby: s.lines
来源：http://naz.wangshuangyany.cn

C#:   s.Split('\n')
来源：http://ijx.aizwys.cn

[E20] 判断字符串是否为空
来源：http://eie.guowangkeji.top

Py:   if not s:
来源：http://ezj.dashuyun.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jce.zhijiandao.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jkm.ivvv.top

TS:   if (s === "") {}
来源：http://uyd.zhoulong.xyz

Java: if (s.isEmpty()) {}
来源：http://yqg.shzxlz.cn

Go:   if s == "" {}
来源：http://zrn.fanxiaobao.xyz

Ruby: if s.empty?
来源：http://eye.sxryk.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ofr.kuanghao11.cn

[E21] 超长截断加省略号
来源：http://nvl.guowangkeji.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wsr.hcnkem.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zbd.zhixingplan.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lek.9152youxi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://arb.havefunace.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ind.ivvv.top

Go:   // 按 rune 判断长度后截断
来源：http://kzg.yj20258.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lke.yj20258888.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://krl.meibo888.top

[E22] 字节长度与字符长度
来源：http://crc.birdmap.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xlx.c1oappe.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zsf.tian-w.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://voh.ehwqpu.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zar.yj20258888.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wfv.cdnleiting.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lvo.ybcxt.top

Ruby: s.bytesize;  s.length
来源：http://wmn.mhx1999.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lgl.hongshengwenyu.top

================================================================================
来源：http://bat.yanxiufei.cn

F. 文件与目录
来源：http://vdn.9152youxi.cn

================================================================================
来源：http://ofn.fanxiaobao.xyz

[F01] 读取整个文件
来源：http://ibk.tianlin.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wmg.316326.xyz

PHP:  file_get_contents("a.txt");
来源：http://qfl.wangshuangyany.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gky.sjlbkw.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rib.cashguo.top

Java: Files.readString(Path.of("a.txt"))
来源：http://dge.hammf.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ouz.ehwqpu.com

Ruby: File.read("a.txt")
来源：http://pxb.yj20258888.top

C#:   File.ReadAllText("a.txt");
来源：http://pxa.chenlongwang.top

[F02] 逐行读取文件
来源：http://ynd.xuetiantiany.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bti.cheryme.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lsv.jinqigfzy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jwq.cucudq.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ijf.xylfe.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dhn.xziqi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://irb.sufxvd.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lik.yonumen.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://enn.jyoumei.cn

[F03] 写入文件（覆盖）
来源：http://cqq.xuanzx.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wvv.cucudq.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://syp.yuanzhike.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://icx.chenlongwang.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lun.aizwys.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ddy.sysykeji.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://krv.cucudq.cn

Ruby: File.write("a.txt", "hi")
来源：http://gdh.chenzaomai.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://seq.jinghuilouyu.cn

[F04] 追加写入文件
来源：http://cgm.havefunace.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://chx.shanyushiyangkeji.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jxq.fengsongda.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hbv.mhx1999.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ewu.sxryk.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://chx.yanxiufei.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hkj.jinghuilouyu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kih.sysykeji.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wsq.ybcxt.top

[F05] 判断文件或目录是否存在
来源：http://noj.sxryk.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vtj.havefunace.top

PHP:  file_exists("a.txt");
来源：http://svl.shangyingyoupin.top

JS:   fs.existsSync("a.txt")
来源：http://mjb.iojbl.cn

TS:   fs.existsSync("a.txt")
来源：http://fwp.shanyushiyangkeji.top

Java: Files.exists(Path.of("a.txt"))
来源：http://bfr.52xcode.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qfp.svipenyu.cn

Ruby: File.exist?("a.txt")
来源：http://yno.snrcjt.cn

C#:   File.Exists("a.txt")
来源：http://uth.jyoumei.cn

[F06] 删除文件
来源：http://swo.yj202588.top

Py:   os.remove("a.txt")
来源：http://hct.andypj.xyz

PHP:  unlink("a.txt");
来源：http://whx.shzxlz.cn

JS:   fs.unlinkSync("a.txt")
来源：http://lgf.feifeiyinyue.top

TS:   fs.unlinkSync("a.txt")
来源：http://tei.chenlongwang.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tlh.cdnleiting.top

Go:   os.Remove("a.txt")
来源：http://fbf.yonumen.top

Ruby: File.delete("a.txt")
来源：http://wjh.ppjwa.cn

C#:   File.Delete("a.txt");
来源：http://cxy.shzxlz.cn

[F07] 创建目录（含多级）
来源：http://bho.ywan-chungtsiang.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vbl.redwolf501.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kmm.hywenlv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qpn.hongshengwenyu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ogt.xinyue.icu

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uis.chenzaomai.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jyq.meibo888.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://oce.hammf.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yvy.wangdashe.top

[F08] 遍历目录
来源：http://gsf.316326.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://smm.chenlongwang.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bpi.ctjpmb.com

JS:   fs.readdirSync("dir")
来源：http://vlj.feifeiyinyue.top

TS:   fs.readdirSync("dir")
来源：http://qtp.tanke756.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pwm.jyoumei.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xcb.shangyingyoupin.top

Ruby: Dir.children("dir")
来源：http://cmc.jinghuilouyu.cn

C#:   Directory.GetFiles("dir")
来源：http://xgq.hesvh.cn

[F09] 获取文件大小
来源：http://ivv.xingfuxueyuan.xyz

Py:   os.path.getsize("a.txt")
来源：http://byy.haohaochexian.top

PHP:  filesize("a.txt");
来源：http://jiz.9152youxi.cn

JS:   fs.statSync("a.txt").size
来源：http://wik.cashguo.top

TS:   fs.statSync("a.txt").size
来源：http://wto.wangdashe.top

Java: Files.size(Path.of("a.txt"))
来源：http://ipg.jinghuilouyu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bco.mhx1999.top

Ruby: File.size("a.txt")
来源：http://fwc.gogol.net.cn

C#:   new FileInfo("a.txt").Length
来源：http://qdz.hnqzz.top

[F10] 取文件扩展名 / 文件名
来源：http://kui.tian-w.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://owf.xinyue.icu

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jxt.quarkkingdee.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mfw.zhixingplan.top

TS:   path.extname("a.txt")
来源：http://coq.meibo888.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bwf.cashguo.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yny.yuanzhike.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vrj.shangyingyoupin.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rzb.xuanzx.com

[F11] 复制与移动文件
来源：http://yhv.iojbl.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ter.9152youxi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qaq.nanxuanxn.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wtz.aibaodan.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gkn.yvedp.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qgf.bjfxy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mpv.nanxuanxn.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xfz.cdnleiting.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rmo.iojbl.cn

[F12] CSV 读写
来源：http://eus.bjfxy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://eum.hesvh.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jhq.yj202588.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zqt.snrcjt.cn

TS:   // 同上
来源：http://okd.sysykeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://csv.uphjek.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ons.andypj.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ydq.ydzc1.top

C#:   // 无内置：用 CsvHelper 库
来源：http://myp.wangdashe.top

================================================================================
来源：http://bdl.fanxiaobao.xyz

G. 面向对象
来源：http://uwo.ywan-chungtsiang.top

================================================================================
来源：http://bql.yonumen.top

[G01] 定义类
来源：http://yqv.jinyuanbaomall.cn

Py:   class User: pass
来源：http://ikd.redwolf501.top

PHP:  class User {}
来源：http://oje.yj20258.top

JS:   class User {}
来源：http://gwb.wangdashe.top

TS:   class User { name: string = ""; }
来源：http://dph.yanxiufei.cn

Java: class User {}
来源：http://rqw.xuanzx.com

Go:   type User struct { Name string }
来源：http://tve.hesvh.cn

Ruby: class User; end
来源：http://zsf.316326.xyz

C#:   class User {}
来源：http://ytb.jqgfzy.top

[G02] 构造函数
来源：http://nks.yj202588.top

Py:   def __init__(self, name): self.name = name
来源：http://qry.sxryk.cn

PHP:  public function __construct(public string $name) {}
来源：http://bbe.ivvv.top

JS:   constructor(name) { this.name = name; }
来源：http://myi.yonumen.top

TS:   constructor(public name: string) {}
来源：http://mdo.wangshuangyany.cn

Java: User(String name) { this.name = name; }
来源：http://ffi.ctjpmb.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rql.fehbvm.com

Ruby: def initialize(name); @name = name; end
来源：http://fwh.feifeiyinyue.top

C#:   public User(string name) { Name = name; }
来源：http://zhq.chenzaomai.com

[G03] 实例属性
来源：http://whq.guowangkeji.top

Py:   self.name = "x"
来源：http://vjl.ppjwa.cn

PHP:  public string $name = "x";
来源：http://ywu.bbcook.cn

JS:   this.name = "x";
来源：http://vzj.snrcjt.cn

TS:   name: string = "x";
来源：http://ext.epnwcf.com

Java: private String name;
来源：http://eey.andypj.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wfk.zhongyouzk.top

Ruby: @name = "x"
来源：http://gnf.vehdjk.com

C#:   public string Name { get; set; } = "x";
来源：http://bix.xingfuxueyuan.xyz

[G04] 定义方法
来源：http://mxv.jinghuilouyu.cn

Py:   def greet(self): return self.name
来源：http://qmz.pycfn.com

PHP:  public function greet(): string { return $this->name; }
来源：http://brt.zhengqikj.top

JS:   greet() { return this.name; }
来源：http://wxd.pengpengdd.cyou

TS:   greet(): string { return this.name; }
来源：http://jnr.fehbvm.com

Java: String greet() { return name; }
来源：http://qer.ybcxt.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://kng.wangshuangyany.cn

Ruby: def greet; @name; end
来源：http://zuv.hcnkem.com

C#:   public string Greet() => Name;
来源：http://jcc.ybcxt.top

[G05] 继承
来源：http://pvg.52xcode.cn

Py:   class Admin(User): pass
来源：http://qhb.guowangkeji.top

PHP:  class Admin extends User {}
来源：http://zsb.bbcook.cn

JS:   class Admin extends User {}
来源：http://edo.daxiang520.top

TS:   class Admin extends User {}
来源：http://fpg.yvedp.cn

Java: class Admin extends User {}
来源：http://tsl.xingfuxueyuan.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tsf.sysykeji.top

Ruby: class Admin < User; end
来源：http://xij.kuanghao11.cn

C#:   class Admin : User {}
来源：http://xdh.fktsv.cn

[G06] 重写方法
来源：http://vrb.ppjwa.cn

Py:   def greet(self): return "admin"
来源：http://prd.ydjk.org.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://aws.iojbl.cn

JS:   greet() { return "admin"; }
来源：http://enf.jlsjyb.cn

TS:   greet(): string { return "admin"; }
来源：http://jcz.cdnleiting.top

Java: @Override String greet() { return "admin"; }
来源：http://doz.ppjwa.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tcd.feifeiyinyue.top

Ruby: def greet; "admin"; end
来源：http://vdd.ppjwa.cn


<!-- 参考信息 -->