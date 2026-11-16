代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rge.yj20258.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lbj.havefunace.top

JS:   s.replace(/\s+/g, "")
来源：http://srr.jqgfzy.top

TS:   s.replace(/\s+/g, "")
来源：http://vsw.yueranfly.top

Java: s.replaceAll("\\s+", "")
来源：http://ndi.zhaomingkeji.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://vmi.0kj1m.cn

Ruby: s.gsub(/\s+/, "")
来源：http://sja.chenzaomai.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xar.yueranfly.top

[E10] 左侧补零 / 定长填充
来源：http://ocl.shanyushiyangtech.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://apn.jinqigufen.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://obk.jianghu66.top

JS:   "7".padStart(3, "0")
来源：http://vhi.redwolf501.top

TS:   "7".padStart(3, "0")
来源：http://egy.zhongyouzk.top

Java: String.format("%03d", 7)
来源：http://elf.hywenlv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://joo.ybcxt.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tti.ivvv.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://toe.zhongyouzk.top

[E11] 反转字符串
来源：http://nut.jinqigfzy.top

Py:   s[::-1]
来源：http://elb.yueranfly.top

PHP:  strrev($s);
来源：http://lyg.havefunace.top

JS:   [...s].reverse().join("")
来源：http://ygg.fktsv.cn

TS:   [...s].reverse().join("")
来源：http://hqb.jqgfzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://uea.guowangkeji.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://fiv.yj202588.top

Ruby: s.reverse
来源：http://ztw.hesvh.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nln.cheryme.top

[E12] 统计某字符出现次数
来源：http://xcm.chenlongwang.top

Py:   s.count("a")
来源：http://acu.tarul.cn

PHP:  substr_count($s, "a");
来源：http://nxw.birdmap.top

JS:   s.split("a").length - 1
来源：http://inu.birdmap.top

TS:   s.split("a").length - 1
来源：http://rpm.zhaomingkeji.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ljy.ydzc1.top

Go:   strings.Count(s, "a")
来源：http://dmc.xuanzx.com

Ruby: s.count("a")
来源：http://wqc.aibaodan.cn

C#:   s.Count(c => c == 'a')
来源：http://apn.redwolf501.top

[E13] 逐字符遍历
来源：http://hfj.ydjk.org.cn

Py:   for ch in s: print(ch)
来源：http://clx.vehdjk.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qev.hfpthk.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qoa.hongshengwenyu.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ici.aibaodan.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tqj.smart0.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mua.bjfxy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://aqc.meibo888.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hag.tian-w.cn

[E14] URL 编码与 Base64
来源：http://gpv.0kj1m.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fke.gaohongyu789.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://vle.c1oappe.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pvh.jinghuilouyu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tuv.uphjek.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yhc.iojbl.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wdr.jiagoushi.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zbj.pycfn.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bhk.guowangkeji.top

[E15] HTML 转义 / 反转义
来源：http://fyq.jlsjyb.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://qxq.xinyue.icu

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cgi.gaohongyu789.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://igw.bjfxy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ict.jiagoushi.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kmi.jinqigfzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tbq.sysykeji.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nwm.ywan-chungtsiang.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nle.xinyue.icu

[E16] 数字千分位
来源：http://wcg.hammf.cn

Py:   f"{1234567:,}"
来源：http://wvu.ybcxt.top

PHP:  number_format(1234567);
来源：http://ljf.xuetiantiany.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zmu.316326.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://mzv.xziqi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nme.zhaomingkeji.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tpe.fzhhl.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kjm.yanxiufei.cn

C#:   1234567.ToString("N0")
来源：http://fiq.feifeiyinyue.top

[E17] 首字母大写
来源：http://kby.wangshuangyany.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yac.xziqi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://lct.hesvh.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jmz.316326.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qqi.jlsjyb.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zgg.zhengqikj.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://idf.9152youxi.cn

Ruby: s.capitalize
来源：http://xzl.kuanghao11.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fjw.ybcxt.top

[E18] 模板占位符替换
来源：http://dmz.ywan-chungtsiang.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zie.zhixingplan.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://woj.hesvh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://seo.chenjidiqi.icu

TS:   tpl.replaceAll("{name}", name)
来源：http://qtj.daxiang520.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hzt.zhengqikj.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vql.gzhubu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://klp.yj202588.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wlh.wangshuangyany.cn

[E19] 多行文本按行拆分
来源：http://ysy.shangyingyoupin.top

Py:   s.splitlines()
来源：http://rsd.gaohongyu789.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://edf.hywenlv.cn

JS:   s.split(/\r?\n/)
来源：http://rmp.chenjidiqi.icu

TS:   s.split(/\r?\n/)
来源：http://zpk.yvedp.cn

Java: s.lines().toList()
来源：http://vxt.jinqigufen.top

Go:   strings.Split(s, "\n")
来源：http://yvn.aibaodan.cn

Ruby: s.lines
来源：http://ozp.hywenlv.cn

C#:   s.Split('\n')
来源：http://cdr.xinyue.icu

[E20] 判断字符串是否为空
来源：http://eky.guannengcc.top

Py:   if not s:
来源：http://pkz.yonumen.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lbn.hongshengwenyu.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dnk.chenlongwang.top

TS:   if (s === "") {}
来源：http://nua.zycfv.cn

Java: if (s.isEmpty()) {}
来源：http://fmz.quarkkingdee.top

Go:   if s == "" {}
来源：http://ybj.xinyue.icu

Ruby: if s.empty?
来源：http://lax.jlsjyb.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tkv.mhx1999.top

[E21] 超长截断加省略号
来源：http://kxd.jiagoushi.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lfd.ywan-chungtsiang.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xfo.xuanzx.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://flo.xylfe.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zlf.sxryk.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ryx.cucudq.cn

Go:   // 按 rune 判断长度后截断
来源：http://uad.hcnkem.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gbz.cucudq.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lls.jinghuilouyu.cn

[E22] 字节长度与字符长度
来源：http://woh.gzhubu.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://akr.dashuyun.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qxn.xingfuxueyuan.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hrw.uphjek.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mpp.hnxiangtu.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fsy.yonumen.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jvv.fanxiaobao.xyz

Ruby: s.bytesize;  s.length
来源：http://pmi.fehbvm.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tiz.shanyushiyangtech.top

================================================================================
来源：http://zlb.xziqi.cn

F. 文件与目录
来源：http://bhk.birdmap.top

================================================================================
来源：http://ffu.cdnleiting.top

[F01] 读取整个文件
来源：http://ikk.gzhubu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fub.c1oappe.top

PHP:  file_get_contents("a.txt");
来源：http://vum.haohaochexian.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rzn.jiagoushi.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://myt.zycfv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ani.ywan-chungtsiang.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vrz.meibo888.top

Ruby: File.read("a.txt")
来源：http://yqr.yuxming.cn

C#:   File.ReadAllText("a.txt");
来源：http://vlv.yonumen.top

[F02] 逐行读取文件
来源：http://aif.guowangkeji.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nay.nwbrower.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qtg.jinghuilouyu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://olt.svipenyu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ghk.shanyushiyangtech.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wik.c1oappe.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ljd.daxiang520.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vns.quarkkingdee.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rjn.gaohongyu789.top

[F03] 写入文件（覆盖）
来源：http://arh.chenlongwang.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://clm.52xcode.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://iom.gaohongyu789.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://llv.yangfankeji.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xzp.zdqjudy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ztu.chenzaomai.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://anf.sufxvd.cn

Ruby: File.write("a.txt", "hi")
来源：http://pbd.kuanghao11.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://aks.jyoumei.cn

[F04] 追加写入文件
来源：http://hzz.jinqigfzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://btp.gzhubu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ecd.tanke756.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fok.zhijiandao.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nex.jiagoushi.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://efw.dianchejie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sio.yangfankeji.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yrt.yuanzhike.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bvv.ydzc1.top

[F05] 判断文件或目录是否存在
来源：http://ypt.ydjk.org.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hqu.haohaochexian.top

PHP:  file_exists("a.txt");
来源：http://qil.yuxming.cn

JS:   fs.existsSync("a.txt")
来源：http://tty.tian-w.cn

TS:   fs.existsSync("a.txt")
来源：http://rzg.wangshuangyany.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ant.feifeiyinyue.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qtq.haohaochexian.top

Ruby: File.exist?("a.txt")
来源：http://cxr.xylfe.cn

C#:   File.Exists("a.txt")
来源：http://huq.fanxiaobao.xyz

[F06] 删除文件
来源：http://crj.xziqi.cn

Py:   os.remove("a.txt")
来源：http://vws.hnxiangtu.top

PHP:  unlink("a.txt");
来源：http://lam.sxryk.cn

JS:   fs.unlinkSync("a.txt")
来源：http://czj.jinyuanbaomall.cn

TS:   fs.unlinkSync("a.txt")
来源：http://dfx.9152youxi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ycc.nanxuanxn.top

Go:   os.Remove("a.txt")
来源：http://rwh.zhixingplan.top

Ruby: File.delete("a.txt")
来源：http://wzn.jiagoushi.top

C#:   File.Delete("a.txt");
来源：http://vvh.fzhhl.top

[F07] 创建目录（含多级）
来源：http://glb.fengsongda.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qah.xinyue.icu

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hca.yfazqb.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eox.svipenyu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ygn.yfazqb.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uck.svipenyu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dhi.ydzc1.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dib.316326.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://agt.yongpay.top

[F08] 遍历目录
来源：http://gex.hongshengwenyu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ppc.jinqigufen.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rge.sysykeji.top

JS:   fs.readdirSync("dir")
来源：http://obb.sysykeji.top

TS:   fs.readdirSync("dir")
来源：http://sng.yj20258888.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://iju.ydjk.org.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gos.jlsjyb.cn

Ruby: Dir.children("dir")
来源：http://xxr.hysaishi.cn

C#:   Directory.GetFiles("dir")
来源：http://wfg.shangyingyoupin.top

[F09] 获取文件大小
来源：http://qog.ywan-chungtsiang.top

Py:   os.path.getsize("a.txt")
来源：http://jhs.hammf.cn

PHP:  filesize("a.txt");
来源：http://mpb.snrcjt.cn

JS:   fs.statSync("a.txt").size
来源：http://eaw.sysykeji.top

TS:   fs.statSync("a.txt").size
来源：http://lpi.tanke756.top

Java: Files.size(Path.of("a.txt"))
来源：http://exo.shanyushiyangkeji.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fba.xylfe.cn

Ruby: File.size("a.txt")
来源：http://ksn.hywenlv.cn

C#:   new FileInfo("a.txt").Length
来源：http://lvg.chenzaomai.com

[F10] 取文件扩展名 / 文件名
来源：http://twj.dianchejie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://arn.zdbjq.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xpi.cdnleiting.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://elf.snrcjt.cn

TS:   path.extname("a.txt")
来源：http://blj.zdbjq.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qfu.xuetiantiany.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zzd.nanxuanxn.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://red.gotoacloud.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://aee.tianlin.xyz

[F11] 复制与移动文件
来源：http://xjc.wangshuangyany.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kqb.316326.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://eud.fanxiaobao.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://inf.cashguo.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tki.xuetiantiany.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://plo.yonumen.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fnr.nanxuanxn.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ped.cheryme.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zog.gotoacloud.top

[F12] CSV 读写
来源：http://jcu.ybcxt.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yfh.xingfuxueyuan.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jly.aibaodan.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vpw.zycfv.cn

TS:   // 同上
来源：http://vzy.fktsv.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ntx.nanxuanxn.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wyk.pycfn.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ljf.jqgufenzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://fhk.ivvv.top

================================================================================
来源：http://buv.gogol.net.cn

G. 面向对象
来源：http://jph.ppjwa.cn

================================================================================
来源：http://ogs.cqqwz.cn

[G01] 定义类
来源：http://ipy.uphjek.com

Py:   class User: pass
来源：http://xsf.birdmap.top

PHP:  class User {}
来源：http://ivi.nanxuanxn.top

JS:   class User {}
来源：http://wmc.jiagoushi.top

TS:   class User { name: string = ""; }
来源：http://bnp.yangfankeji.com

Java: class User {}
来源：http://ovk.mhx1999.top

Go:   type User struct { Name string }
来源：http://nra.tarul.cn

Ruby: class User; end
来源：http://ojs.ybcxt.top

C#:   class User {}
来源：http://bfd.zdqjudy.top

[G02] 构造函数
来源：http://vkm.xuanzx.com

Py:   def __init__(self, name): self.name = name
来源：http://aat.aizwys.cn

PHP:  public function __construct(public string $name) {}
来源：http://vig.ywan-chungtsiang.top

JS:   constructor(name) { this.name = name; }
来源：http://cec.chenjidiqi.icu

TS:   constructor(public name: string) {}
来源：http://aqi.yj20258888.top

Java: User(String name) { this.name = name; }
来源：http://lhd.aibaodan.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vrw.vehdjk.com

Ruby: def initialize(name); @name = name; end
来源：http://qaa.bjfxy.top

C#:   public User(string name) { Name = name; }
来源：http://uwo.yuanzhike.top

[G03] 实例属性
来源：http://wmn.fengsongda.top

Py:   self.name = "x"
来源：http://hpr.hysaishi.cn

PHP:  public string $name = "x";
来源：http://hna.jinqigufen.top

JS:   this.name = "x";
来源：http://qow.hcnkem.com

TS:   name: string = "x";
来源：http://kek.daxiang520.top

Java: private String name;
来源：http://jxu.xuanzx.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zal.jiagoushi.top

Ruby: @name = "x"
来源：http://lww.jyoumei.cn

C#:   public string Name { get; set; } = "x";
来源：http://frj.gaohongyu789.top

[G04] 定义方法
来源：http://uwn.zdbjq.cn

Py:   def greet(self): return self.name
来源：http://ofs.aibaodan.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hbf.shanyushiyangtech.top

JS:   greet() { return this.name; }
来源：http://eww.shanyushiyangtech.top

TS:   greet(): string { return this.name; }
来源：http://adl.gzhubu.top

Java: String greet() { return name; }
来源：http://vyc.jinghuilouyu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://anh.ppjwa.cn

Ruby: def greet; @name; end
来源：http://ajt.cqqwz.cn

C#:   public string Greet() => Name;
来源：http://rlk.yj20258.top

[G05] 继承
来源：http://naa.sjlbkw.cn

Py:   class Admin(User): pass
来源：http://yne.ywan-chungtsiang.top

PHP:  class Admin extends User {}
来源：http://ctn.hysaishi.cn

JS:   class Admin extends User {}
来源：http://hdk.xuetiantiany.cn

TS:   class Admin extends User {}
来源：http://yhg.ydjk.org.cn

Java: class Admin extends User {}
来源：http://tmo.hysaishi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hdm.daxiang520.top

Ruby: class Admin < User; end
来源：http://ikw.aibaodan.cn

C#:   class Admin : User {}
来源：http://hwd.jyoumei.cn

[G06] 重写方法
来源：http://bup.zycfv.cn

Py:   def greet(self): return "admin"
来源：http://rcc.xinyue.icu

PHP:  public function greet(): string { return "admin"; }
来源：http://emo.cucudq.cn

JS:   greet() { return "admin"; }
来源：http://nte.yuxming.cn

TS:   greet(): string { return "admin"; }
来源：http://gbq.hywenlv.cn

Java: @Override String greet() { return "admin"; }
来源：http://fit.nanxinkj.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sji.jqgfzy.top

Ruby: def greet; "admin"; end
来源：http://cvl.cashguo.top

C#:   public override string Greet() => "admin";
来源：http://kjq.jqgfzy.top

[G07] 调用父类方法
来源：http://cuv.zycfv.cn

Py:   super().greet()
来源：http://rjf.ydzc1.top

PHP:  parent::greet();
来源：http://qvx.jqgufenzy.top

JS:   super.greet();
来源：http://jjv.ivvv.top

TS:   super.greet();
来源：http://ujh.daxiang520.top

Java: super.greet();
来源：http://vpp.ybcxt.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pmc.chenzaomai.com


<!-- 参考信息 -->