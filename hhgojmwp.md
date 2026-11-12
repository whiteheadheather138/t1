代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://fwe.andypj.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://fvp.fanxiaobao.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://srm.hongshengwenyu.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ioe.ydjk.org.cn

[E10] 左侧补零 / 定长填充
来源：http://yam.iojbl.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lmq.fengsongda.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cul.tianlin.xyz

JS:   "7".padStart(3, "0")
来源：http://tzp.aibaodan.cn

TS:   "7".padStart(3, "0")
来源：http://ecw.nanxinkj.top

Java: String.format("%03d", 7)
来源：http://mhm.tianlin.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://cpv.zycfv.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tpm.zdbjq.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kjz.jinyuanbaomall.cn

[E11] 反转字符串
来源：http://wgu.vqdsnc.cn

Py:   s[::-1]
来源：http://rui.fengsongda.top

PHP:  strrev($s);
来源：http://bvb.sxryk.cn

JS:   [...s].reverse().join("")
来源：http://toj.smart0.xyz

TS:   [...s].reverse().join("")
来源：http://sxj.fzhhl.top

Java: new StringBuilder(s).reverse().toString()
来源：http://mhh.bjfxy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://lrb.jqgufenzy.top

Ruby: s.reverse
来源：http://qir.jqgfzy.top

C#:   new string(s.Reverse().ToArray())
来源：http://xtp.jlsjyb.cn

[E12] 统计某字符出现次数
来源：http://qpb.xuanzx.com

Py:   s.count("a")
来源：http://czj.yangfankeji.com

PHP:  substr_count($s, "a");
来源：http://vqs.xuetiantiany.cn

JS:   s.split("a").length - 1
来源：http://jas.vehdjk.com

TS:   s.split("a").length - 1
来源：http://rnk.feifeiyinyue.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://uob.feifeiyinyue.top

Go:   strings.Count(s, "a")
来源：http://nvp.shanyushiyangkeji.top

Ruby: s.count("a")
来源：http://knk.zhiwuduotai.top

C#:   s.Count(c => c == 'a')
来源：http://wjg.sxryk.cn

[E13] 逐字符遍历
来源：http://ebc.sysykeji.top

Py:   for ch in s: print(ch)
来源：http://xev.iojbl.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nbx.jiagoushi.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://yfo.jinqigfzy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://rwo.yj202588.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zxn.fanxiaobao.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://djm.vqdsnc.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vvd.yuxming.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vut.yangfankeji.com

[E14] URL 编码与 Base64
来源：http://opy.fktsv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kun.hammf.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://wsk.pycfn.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qem.yongpay.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ofb.iojbl.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rov.sweek.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jai.uphjek.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fnk.vqdsnc.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lth.fengsongda.top

[E15] HTML 转义 / 反转义
来源：http://puy.quarkkingdee.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ijt.c1oappe.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jse.jinqigufen.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sqb.fengsongda.top

TS:   // 同上，务必做 XSS 过滤
来源：http://pyx.daria6918.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tnm.jinqigufen.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://npo.shzxlz.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://swh.zhijiandao.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pvb.svipenyu.cn

[E16] 数字千分位
来源：http://mle.dianchejie.cn

Py:   f"{1234567:,}"
来源：http://xol.hcnkem.com

PHP:  number_format(1234567);
来源：http://zlh.yj20258.top

JS:   (1234567).toLocaleString("en-US")
来源：http://xxq.cheryme.top

TS:   (1234567).toLocaleString("en-US")
来源：http://sld.birdmap.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lrc.zycfv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ypt.fanxiaobao.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gqs.hfpthk.cn

C#:   1234567.ToString("N0")
来源：http://doa.52xcode.cn

[E17] 首字母大写
来源：http://mwm.jinqigufen.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zvv.nwbrower.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://xen.shanyushiyangtech.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bcr.fehbvm.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wwr.ydjk.org.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vbb.shanyushiyangtech.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://oks.fehbvm.com

Ruby: s.capitalize
来源：http://czb.yangfankeji.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ifd.c1oappe.top

[E18] 模板占位符替换
来源：http://wey.zhijiandao.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ahb.jinghuilouyu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://myq.vqdsnc.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://izv.snrcjt.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://dat.shangyingyoupin.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://djs.yvedp.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lrm.yueranfly.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ppr.fengsongda.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gvl.tarul.cn

[E19] 多行文本按行拆分
来源：http://sbi.yuanzhike.top

Py:   s.splitlines()
来源：http://icd.fktsv.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sco.yongpay.top

JS:   s.split(/\r?\n/)
来源：http://yrg.dashuyun.cn

TS:   s.split(/\r?\n/)
来源：http://lwf.vqdsnc.cn

Java: s.lines().toList()
来源：http://xyt.yanxiufei.cn

Go:   strings.Split(s, "\n")
来源：http://orx.xuanzx.com

Ruby: s.lines
来源：http://ugx.quarkkingdee.top

C#:   s.Split('\n')
来源：http://uzt.sxryk.cn

[E20] 判断字符串是否为空
来源：http://kdb.zhongyouzk.top

Py:   if not s:
来源：http://hyk.nanxinkj.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wbc.zhixingplan.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ccb.epnwcf.com

TS:   if (s === "") {}
来源：http://puc.xziqi.cn

Java: if (s.isEmpty()) {}
来源：http://auf.chenjidiqi.icu

Go:   if s == "" {}
来源：http://rjd.quarkkingdee.top

Ruby: if s.empty?
来源：http://gcd.dashuyun.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kwv.yuxming.cn

[E21] 超长截断加省略号
来源：http://hfn.nanxuanxn.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wii.vqdsnc.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wew.xylfe.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dtz.fzhhl.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rza.zdqjudy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nqx.cdnleiting.top

Go:   // 按 rune 判断长度后截断
来源：http://edd.yfazqb.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://eoh.yj20258.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cbz.cdnleiting.top

[E22] 字节长度与字符长度
来源：http://tzw.nanxinkj.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lkt.wangshuangyany.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://moj.kuanghao11.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mxa.daxiang520.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kdx.xingfuxueyuan.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://piz.sxryk.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://khn.jqgufenzy.top

Ruby: s.bytesize;  s.length
来源：http://sht.yj202588.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bkp.gaohongyu789.top

================================================================================
来源：http://pys.hongshengwenyu.top

F. 文件与目录
来源：http://zwd.sxryk.cn

================================================================================
来源：http://bnt.jinghuilouyu.cn

[F01] 读取整个文件
来源：http://bes.kuanghao11.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vxh.iojbl.cn

PHP:  file_get_contents("a.txt");
来源：http://qyx.xuetiantiany.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jby.fktsv.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fdm.smart0.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://yuj.hongshengwenyu.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zye.tian-w.cn

Ruby: File.read("a.txt")
来源：http://tqe.epnwcf.com

C#:   File.ReadAllText("a.txt");
来源：http://glw.zdbjq.cn

[F02] 逐行读取文件
来源：http://nnk.feifeiyinyue.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://seb.shanyushiyangkeji.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bjs.fehbvm.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://snq.birdmap.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rvh.meibo888.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://omt.zhengqikj.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wbv.xylfe.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://epr.daria6918.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gmk.jinqigfzy.top

[F03] 写入文件（覆盖）
来源：http://zsi.daria6918.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.xingfuxueyuan.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://die.hnqzz.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rnb.sjlbkw.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://clg.yj20258888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://snx.sjlbkw.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sab.jinghuilouyu.cn

Ruby: File.write("a.txt", "hi")
来源：http://fiz.quarkkingdee.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hfx.quarkkingdee.top

[F04] 追加写入文件
来源：http://tjo.havefunace.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gyt.fehbvm.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://obw.ydjk.org.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wwx.aibaodan.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bwj.jyoumei.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fzc.yj20258.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://heu.gogol.net.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://spv.fengsongda.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bgk.dianchejie.cn

[F05] 判断文件或目录是否存在
来源：http://jua.zhoulong.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nkp.pengpengdd.cyou

PHP:  file_exists("a.txt");
来源：http://ahk.haohaochexian.top

JS:   fs.existsSync("a.txt")
来源：http://qrk.hfpthk.cn

TS:   fs.existsSync("a.txt")
来源：http://dtb.hfpthk.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://slm.wangdashe.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://aqf.iojbl.cn

Ruby: File.exist?("a.txt")
来源：http://cap.yueranfly.top

C#:   File.Exists("a.txt")
来源：http://mfs.zhoulong.xyz

[F06] 删除文件
来源：http://qkq.feifeiyinyue.top

Py:   os.remove("a.txt")
来源：http://jqu.nwbrower.top

PHP:  unlink("a.txt");
来源：http://ypx.fengsongda.top

JS:   fs.unlinkSync("a.txt")
来源：http://avr.hywenlv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://yih.pengpengdd.cyou

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://awi.zhijiandao.cn

Go:   os.Remove("a.txt")
来源：http://ari.tian-w.cn

Ruby: File.delete("a.txt")
来源：http://irx.jqgfzy.top

C#:   File.Delete("a.txt");
来源：http://zbc.quarkkingdee.top

[F07] 创建目录（含多级）
来源：http://fzr.zhengqikj.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sdp.gaohongyu789.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://phr.hfpthk.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yls.jyoumei.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://thy.xziqi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bon.0kj1m.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vrx.bjfxy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gzg.daxiang520.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vto.hnqzz.top

[F08] 遍历目录
来源：http://vgb.yj20258.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://snv.hnqzz.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jar.xziqi.cn

JS:   fs.readdirSync("dir")
来源：http://ofm.0kj1m.cn

TS:   fs.readdirSync("dir")
来源：http://ott.hywenlv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bvj.yueranfly.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ayl.ivvv.top

Ruby: Dir.children("dir")
来源：http://fss.sxryk.cn

C#:   Directory.GetFiles("dir")
来源：http://zzh.zdqjudy.top

[F09] 获取文件大小
来源：http://wuz.sweek.top

Py:   os.path.getsize("a.txt")
来源：http://wum.bbcook.cn

PHP:  filesize("a.txt");
来源：http://njx.yongpay.top

JS:   fs.statSync("a.txt").size
来源：http://aff.fengsongda.top

TS:   fs.statSync("a.txt").size
来源：http://sks.fengsongda.top

Java: Files.size(Path.of("a.txt"))
来源：http://usr.zdbjq.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dpy.xinyue.icu

Ruby: File.size("a.txt")
来源：http://riy.shanyushiyangtech.top

C#:   new FileInfo("a.txt").Length
来源：http://ict.zhoulong.xyz

[F10] 取文件扩展名 / 文件名
来源：http://ybh.52xcode.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kgd.gotoacloud.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fdx.yuanzhike.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bsa.havefunace.top

TS:   path.extname("a.txt")
来源：http://kqs.mhx1999.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hjq.bjfxy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kxx.jinyuanbaomall.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pcz.fzhhl.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jaz.nwbrower.top

[F11] 复制与移动文件
来源：http://buq.quarkkingdee.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://brm.xziqi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zon.dashuyun.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ocs.gzhubu.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ont.xingfuxueyuan.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://evx.pycfn.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pky.havefunace.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lbx.birdmap.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nxh.xuetiantiany.cn

[F12] CSV 读写
来源：http://kon.pengpengdd.cyou

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kgo.xylfe.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xus.shangyingyoupin.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://npb.quarkkingdee.top

TS:   // 同上
来源：http://wrd.snrcjt.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kwf.hywenlv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gpd.xingfuxueyuan.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lmy.hongshengwenyu.top

C#:   // 无内置：用 CsvHelper 库
来源：http://nbp.yangfankeji.com

================================================================================
来源：http://ocm.vehdjk.com

G. 面向对象
来源：http://rzs.iojbl.cn

================================================================================
来源：http://lbo.vehdjk.com

[G01] 定义类
来源：http://bbo.yueranfly.top

Py:   class User: pass
来源：http://csg.haohaochexian.top

PHP:  class User {}
来源：http://hfm.zhijiandao.cn

JS:   class User {}
来源：http://pmc.jianghu66.top

TS:   class User { name: string = ""; }
来源：http://mhh.bjfxy.top

Java: class User {}
来源：http://coi.ywan-chungtsiang.top

Go:   type User struct { Name string }
来源：http://slc.zhoulong.xyz

Ruby: class User; end
来源：http://vgs.gaohongyu789.top

C#:   class User {}
来源：http://wry.bjfxy.top

[G02] 构造函数
来源：http://fyo.gotoacloud.top

Py:   def __init__(self, name): self.name = name
来源：http://nko.mhx1999.top

PHP:  public function __construct(public string $name) {}
来源：http://fsk.hesvh.cn

JS:   constructor(name) { this.name = name; }
来源：http://iwp.yanxiufei.cn

TS:   constructor(public name: string) {}
来源：http://yvx.birdmap.top

Java: User(String name) { this.name = name; }
来源：http://mnv.cqqwz.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pyl.feifeiyinyue.top

Ruby: def initialize(name); @name = name; end
来源：http://bvk.tian-w.cn

C#:   public User(string name) { Name = name; }
来源：http://vus.xuetiantiany.cn

[G03] 实例属性
来源：http://zvm.fengsongda.top

Py:   self.name = "x"
来源：http://xgo.zhongyouzk.top

PHP:  public string $name = "x";
来源：http://oqv.uphjek.com

JS:   this.name = "x";
来源：http://brj.chenlongwang.top

TS:   name: string = "x";
来源：http://sno.bbcook.cn

Java: private String name;
来源：http://gnl.zhiwuduotai.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://con.jinghuilouyu.cn

Ruby: @name = "x"
来源：http://ykc.wangshuangyany.cn

C#:   public string Name { get; set; } = "x";
来源：http://mlp.xylfe.cn

[G04] 定义方法
来源：http://ksu.xuanzx.com

Py:   def greet(self): return self.name
来源：http://mhw.zhongyouzk.top

PHP:  public function greet(): string { return $this->name; }
来源：http://drx.yueranfly.top

JS:   greet() { return this.name; }
来源：http://dwr.shanyushiyangkeji.top

TS:   greet(): string { return this.name; }
来源：http://qym.cdnleiting.top

Java: String greet() { return name; }
来源：http://zkm.guannengcc.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ynz.shanyushiyangtech.top

Ruby: def greet; @name; end
来源：http://vpd.zycfv.cn

C#:   public string Greet() => Name;
来源：http://gdv.quarkkingdee.top

[G05] 继承
来源：http://biq.sxryk.cn

Py:   class Admin(User): pass
来源：http://ikn.hesvh.cn

PHP:  class Admin extends User {}
来源：http://ogt.chenzaomai.com

JS:   class Admin extends User {}
来源：http://rtb.ydjk.org.cn

TS:   class Admin extends User {}
来源：http://tmb.hnqzz.top

Java: class Admin extends User {}
来源：http://vav.jinqigufen.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qkj.fzhhl.top

Ruby: class Admin < User; end
来源：http://azv.bbcook.cn

C#:   class Admin : User {}
来源：http://eli.gaohongyu789.top

[G06] 重写方法
来源：http://umc.sxryk.cn

Py:   def greet(self): return "admin"
来源：http://tcr.yuanzhike.top

PHP:  public function greet(): string { return "admin"; }
来源：http://swr.uphjek.com

JS:   greet() { return "admin"; }
来源：http://zgj.yueranfly.top

TS:   greet(): string { return "admin"; }
来源：http://fnp.fengsongda.top

Java: @Override String greet() { return "admin"; }
来源：http://uoz.yongpay.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://iil.feifeiyinyue.top

Ruby: def greet; "admin"; end
来源：http://yew.pycfn.com

C#:   public override string Greet() => "admin";
来源：http://exf.sjlbkw.cn

[G07] 调用父类方法
来源：http://dcz.xuetiantiany.cn

Py:   super().greet()
来源：http://wpa.svipenyu.cn

PHP:  parent::greet();
来源：http://rix.sjlbkw.cn

JS:   super.greet();
来源：http://jli.jlsjyb.cn

TS:   super.greet();
来源：http://pny.aizwys.cn

Java: super.greet();
来源：http://lkw.c1oappe.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://okc.jinqigufen.top

Ruby: super
来源：http://jeg.vehdjk.com

C#:   base.Greet();
来源：http://ksf.yongpay.top

[G08] 静态方法与属性
来源：http://oco.hongshengwenyu.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ave.uphjek.com


<!-- 参考信息 -->