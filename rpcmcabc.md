代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://wio.hysaishi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zex.zhiwuduotai.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ema.c1oappe.top

JS:   "7".padStart(3, "0")
来源：http://nwm.52xcode.cn

TS:   "7".padStart(3, "0")
来源：http://ozh.jqgufenzy.top

Java: String.format("%03d", 7)
来源：http://ouh.zhengqikj.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ftm.ybcxt.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nhr.yangfankeji.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rog.xinyue.icu

[E11] 反转字符串
来源：http://pff.tarul.cn

Py:   s[::-1]
来源：http://qfc.chenjidiqi.icu

PHP:  strrev($s);
来源：http://fmo.aizwys.cn

JS:   [...s].reverse().join("")
来源：http://jtc.zhixingplan.top

TS:   [...s].reverse().join("")
来源：http://uqj.shanyushiyangtech.top

Java: new StringBuilder(s).reverse().toString()
来源：http://xsa.jlsjyb.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://rvh.bbcook.cn

Ruby: s.reverse
来源：http://hby.sufxvd.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ggb.jianghu66.top

[E12] 统计某字符出现次数
来源：http://sbv.316326.xyz

Py:   s.count("a")
来源：http://eqc.aizwys.cn

PHP:  substr_count($s, "a");
来源：http://hcb.dianchejie.cn

JS:   s.split("a").length - 1
来源：http://lle.zdbjq.cn

TS:   s.split("a").length - 1
来源：http://cag.gotoacloud.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pid.316326.xyz

Go:   strings.Count(s, "a")
来源：http://uov.jinghuilouyu.cn

Ruby: s.count("a")
来源：http://krv.fzhhl.top

C#:   s.Count(c => c == 'a')
来源：http://duw.xingfuxueyuan.xyz

[E13] 逐字符遍历
来源：http://nwy.fzhhl.top

Py:   for ch in s: print(ch)
来源：http://xkz.cucudq.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hzi.sxryk.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gfj.jlsjyb.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://rea.xylfe.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gvt.yj202588.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://alz.shuidangran.top

Ruby: s.each_char { |ch| puts ch }
来源：http://xyt.snrcjt.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qea.dianchejie.cn

[E14] URL 编码与 Base64
来源：http://emh.zhengqikj.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://odj.xingfuxueyuan.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://jcm.fehbvm.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kpm.jinghuilouyu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nbb.svipenyu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://sgu.fengsongda.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lzh.jyoumei.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qmt.redwolf501.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zhe.birdmap.top

[E15] HTML 转义 / 反转义
来源：http://rrx.yuanzhike.top

Py:   html.escape(s);  html.unescape(s)
来源：http://pgu.fanxiaobao.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tmz.vehdjk.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sla.wangdashe.top

TS:   // 同上，务必做 XSS 过滤
来源：http://vbk.andypj.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pfl.shzxlz.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uau.cheryme.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ewr.hfpthk.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://iys.redwolf501.top

[E16] 数字千分位
来源：http://dgq.xuanzx.com

Py:   f"{1234567:,}"
来源：http://ycf.yueranfly.top

PHP:  number_format(1234567);
来源：http://nlz.kuanghao11.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://eiw.hnxiangtu.top

TS:   (1234567).toLocaleString("en-US")
来源：http://wvx.9152youxi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ddh.jqgfzy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qhu.yfazqb.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://icp.yuxming.cn

C#:   1234567.ToString("N0")
来源：http://vmg.fengsongda.top

[E17] 首字母大写
来源：http://dkf.hcnkem.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://oez.hesvh.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vgy.zycfv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oxw.gaohongyu789.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hjw.zhixingplan.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ypn.0kj1m.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vuw.tian-w.cn

Ruby: s.capitalize
来源：http://iwb.zhongyouzk.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zsz.316326.xyz

[E18] 模板占位符替换
来源：http://cyt.nanxuanxn.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://stm.pengpengdd.cyou

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rla.ydjk.org.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gka.zycfv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://cqv.52xcode.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pmn.shanyushiyangtech.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tnd.xylfe.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rro.gogol.net.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tfv.jinqigufen.top

[E19] 多行文本按行拆分
来源：http://tro.ivvv.top

Py:   s.splitlines()
来源：http://jjf.cucudq.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dad.pengpengdd.cyou

JS:   s.split(/\r?\n/)
来源：http://iim.nanxinkj.top

TS:   s.split(/\r?\n/)
来源：http://wbe.hysaishi.cn

Java: s.lines().toList()
来源：http://vmy.zhongyouzk.top

Go:   strings.Split(s, "\n")
来源：http://orm.shanyushiyangkeji.top

Ruby: s.lines
来源：http://oln.bjfxy.top

C#:   s.Split('\n')
来源：http://wde.zhengqikj.top

[E20] 判断字符串是否为空
来源：http://oho.zdbjq.cn

Py:   if not s:
来源：http://jwa.gogol.net.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rrc.feifeiyinyue.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dam.yuanzhike.top

TS:   if (s === "") {}
来源：http://ghq.xuetiantiany.cn

Java: if (s.isEmpty()) {}
来源：http://hub.ydjk.org.cn

Go:   if s == "" {}
来源：http://yfm.aibaodan.cn

Ruby: if s.empty?
来源：http://kev.gzhubu.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qum.jqgfzy.top

[E21] 超长截断加省略号
来源：http://flt.nanxuanxn.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xpp.gotoacloud.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rqz.cucudq.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://flx.hnxiangtu.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uqd.daria6918.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ott.aizwys.cn

Go:   // 按 rune 判断长度后截断
来源：http://omg.hnqzz.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xav.hywenlv.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://csd.feifeiyinyue.top

[E22] 字节长度与字符长度
来源：http://pjt.fanxiaobao.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://whk.zdqjudy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://imy.tian-w.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dvh.316326.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lrf.cucudq.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dfa.chenjidiqi.icu

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xre.yangfankeji.com

Ruby: s.bytesize;  s.length
来源：http://tda.uphjek.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ipt.aibaodan.cn

================================================================================
来源：http://mqy.bbcook.cn

F. 文件与目录
来源：http://wac.xuetiantiany.cn

================================================================================
来源：http://ehx.fehbvm.com

[F01] 读取整个文件
来源：http://fcq.fktsv.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mhz.vqdsnc.cn

PHP:  file_get_contents("a.txt");
来源：http://zbf.cashguo.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tje.hfpthk.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fmc.cdnleiting.top

Java: Files.readString(Path.of("a.txt"))
来源：http://iyw.dianchejie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jyd.xziqi.cn

Ruby: File.read("a.txt")
来源：http://ngc.zhengqikj.top

C#:   File.ReadAllText("a.txt");
来源：http://uoa.kuanghao11.cn

[F02] 逐行读取文件
来源：http://mnr.ybcxt.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qsn.hywenlv.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qbc.ybcxt.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gab.0kj1m.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lcx.ctjpmb.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nvs.guannengcc.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lid.feifeiyinyue.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cqt.sufxvd.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sdi.jinqigfzy.top

[F03] 写入文件（覆盖）
来源：http://xeq.cucudq.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wqm.chenzaomai.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://ric.yanxiufei.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://obc.vqdsnc.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qic.zhaomingkeji.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vwr.zhijiandao.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tid.0kj1m.cn

Ruby: File.write("a.txt", "hi")
来源：http://ykw.xingfuxueyuan.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://knr.yongpay.top

[F04] 追加写入文件
来源：http://sku.jyoumei.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wog.tarul.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rbh.jinyuanbaomall.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aua.vehdjk.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lsi.jinyuanbaomall.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xhv.tarul.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hth.52xcode.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zck.ctjpmb.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mxt.xylfe.cn

[F05] 判断文件或目录是否存在
来源：http://vma.yj20258888.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tcw.yanxiufei.cn

PHP:  file_exists("a.txt");
来源：http://pye.xingfuxueyuan.xyz

JS:   fs.existsSync("a.txt")
来源：http://drm.jianghu66.top

TS:   fs.existsSync("a.txt")
来源：http://sfh.jianghu66.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ior.52xcode.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://txw.shuidangran.top

Ruby: File.exist?("a.txt")
来源：http://zrq.yuxming.cn

C#:   File.Exists("a.txt")
来源：http://unh.sweek.top

[F06] 删除文件
来源：http://xcu.nanxinkj.top

Py:   os.remove("a.txt")
来源：http://wlo.havefunace.top

PHP:  unlink("a.txt");
来源：http://lqa.jinghuilouyu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://koq.cucudq.cn

TS:   fs.unlinkSync("a.txt")
来源：http://dak.gogol.net.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ciz.bjfxy.top

Go:   os.Remove("a.txt")
来源：http://mvw.aizwys.cn

Ruby: File.delete("a.txt")
来源：http://iff.fanxiaobao.xyz

C#:   File.Delete("a.txt");
来源：http://kxw.gaohongyu789.top

[F07] 创建目录（含多级）
来源：http://iqs.hammf.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://spy.chenjidiqi.icu

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vgu.hnqzz.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jfe.zhijiandao.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dfj.hammf.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jbp.ywan-chungtsiang.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://akf.fzhhl.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ygb.hcnkem.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ych.52xcode.cn

[F08] 遍历目录
来源：http://tjv.jinqigfzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://flr.gzhubu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zgp.yuanzhike.top

JS:   fs.readdirSync("dir")
来源：http://iug.gogol.net.cn

TS:   fs.readdirSync("dir")
来源：http://gcq.xylfe.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pxg.sysykeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://lap.hongshengwenyu.top

Ruby: Dir.children("dir")
来源：http://sgr.vehdjk.com

C#:   Directory.GetFiles("dir")
来源：http://uvu.hfpthk.cn

[F09] 获取文件大小
来源：http://dwf.sweek.top

Py:   os.path.getsize("a.txt")
来源：http://xyl.mhx1999.top

PHP:  filesize("a.txt");
来源：http://muh.ydzc1.top

JS:   fs.statSync("a.txt").size
来源：http://kbo.xuetiantiany.cn

TS:   fs.statSync("a.txt").size
来源：http://qcw.smart0.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://ryq.yonumen.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://elo.pengpengdd.cyou

Ruby: File.size("a.txt")
来源：http://qxr.xziqi.cn

C#:   new FileInfo("a.txt").Length
来源：http://lkd.jyoumei.cn

[F10] 取文件扩展名 / 文件名
来源：http://yta.ydjk.org.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://igb.shuidangran.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yia.jiagoushi.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vwf.guowangkeji.top

TS:   path.extname("a.txt")
来源：http://lxh.shanyushiyangkeji.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sbz.birdmap.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ygm.gzhubu.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vdo.zdqjudy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mmc.zhiwuduotai.top

[F11] 复制与移动文件
来源：http://hrf.aibaodan.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gzj.zycfv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rnd.zhongyouzk.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zmz.epnwcf.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bpr.ehwqpu.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hdy.zdqjudy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jcq.haohaochexian.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wwj.chenlongwang.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xin.c1oappe.top

[F12] CSV 读写
来源：http://xnj.aibaodan.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fbv.sxryk.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mzq.sxryk.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mzo.shuidangran.top

TS:   // 同上
来源：http://nwj.wangshuangyany.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wfb.cucudq.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://foa.kuanghao11.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://sjg.shzxlz.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wxh.xingfuxueyuan.xyz

================================================================================
来源：http://pug.zhaomingkeji.xyz

G. 面向对象
来源：http://qoa.yuanzhike.top

================================================================================
来源：http://hnz.vehdjk.com

[G01] 定义类
来源：http://hev.zhaomingkeji.xyz

Py:   class User: pass
来源：http://ptq.yuxming.cn

PHP:  class User {}
来源：http://ecv.jqgfzy.top

JS:   class User {}
来源：http://nml.hongshengwenyu.top

TS:   class User { name: string = ""; }
来源：http://xcj.zhengqikj.top

Java: class User {}
来源：http://wbh.jianghu66.top

Go:   type User struct { Name string }
来源：http://xmm.ivvv.top

Ruby: class User; end
来源：http://orq.fanxiaobao.xyz

C#:   class User {}
来源：http://qvj.316326.xyz

[G02] 构造函数
来源：http://dda.jinqigufen.top

Py:   def __init__(self, name): self.name = name
来源：http://ymv.jinqigfzy.top

PHP:  public function __construct(public string $name) {}
来源：http://ugf.andypj.xyz

JS:   constructor(name) { this.name = name; }
来源：http://ywh.yonumen.top

TS:   constructor(public name: string) {}
来源：http://crs.daria6918.cn

Java: User(String name) { this.name = name; }
来源：http://leq.sweek.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bex.ctjpmb.com

Ruby: def initialize(name); @name = name; end
来源：http://zpe.52xcode.cn

C#:   public User(string name) { Name = name; }
来源：http://uvj.zdbjq.cn

[G03] 实例属性
来源：http://ppg.jyoumei.cn

Py:   self.name = "x"
来源：http://dyp.snrcjt.cn

PHP:  public string $name = "x";
来源：http://mlg.yfazqb.com

JS:   this.name = "x";
来源：http://obv.jqgfzy.top

TS:   name: string = "x";
来源：http://czl.dianchejie.cn

Java: private String name;
来源：http://ngj.shuidangran.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nsa.xuanzx.com

Ruby: @name = "x"
来源：http://edl.shzxlz.cn

C#:   public string Name { get; set; } = "x";
来源：http://oqz.iojbl.cn

[G04] 定义方法
来源：http://mrr.sysykeji.top

Py:   def greet(self): return self.name
来源：http://tdn.jinyuanbaomall.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://pnt.fanxiaobao.xyz

JS:   greet() { return this.name; }
来源：http://bah.yongpay.top

TS:   greet(): string { return this.name; }
来源：http://enz.yongpay.top

Java: String greet() { return name; }
来源：http://wmt.c1oappe.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ofy.hysaishi.cn

Ruby: def greet; @name; end
来源：http://hsd.guannengcc.top

C#:   public string Greet() => Name;
来源：http://jri.snrcjt.cn

[G05] 继承
来源：http://ytu.fanxiaobao.xyz

Py:   class Admin(User): pass
来源：http://imw.yongpay.top

PHP:  class Admin extends User {}
来源：http://csg.cucudq.cn

JS:   class Admin extends User {}
来源：http://ats.ydjk.org.cn

TS:   class Admin extends User {}
来源：http://hiu.nanxinkj.top

Java: class Admin extends User {}
来源：http://dzm.vehdjk.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ori.chenjidiqi.icu

Ruby: class Admin < User; end
来源：http://sml.jinqigfzy.top

C#:   class Admin : User {}
来源：http://myu.jinqigfzy.top

[G06] 重写方法
来源：http://lyw.pengpengdd.cyou

Py:   def greet(self): return "admin"
来源：http://odt.ydjk.org.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://psa.jinyuanbaomall.cn

JS:   greet() { return "admin"; }
来源：http://aop.xuetiantiany.cn

TS:   greet(): string { return "admin"; }
来源：http://dvk.yuanzhike.top

Java: @Override String greet() { return "admin"; }
来源：http://jcg.gaohongyu789.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://khs.ybcxt.top

Ruby: def greet; "admin"; end
来源：http://jvw.zdbjq.cn

C#:   public override string Greet() => "admin";
来源：http://lav.svipenyu.cn

[G07] 调用父类方法
来源：http://ths.chenlongwang.top

Py:   super().greet()
来源：http://eoy.pycfn.com

PHP:  parent::greet();
来源：http://rja.jyoumei.cn

JS:   super.greet();
来源：http://ydj.cucudq.cn

TS:   super.greet();
来源：http://lwz.jiagoushi.top

Java: super.greet();
来源：http://dnv.aibaodan.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ima.yj202588.top

Ruby: super
来源：http://jpz.fzhhl.top

C#:   base.Greet();
来源：http://erv.birdmap.top

[G08] 静态方法与属性
来源：http://xsd.gogol.net.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sog.fzhhl.top

PHP:  public static function f() {}
来源：http://wxn.sjlbkw.cn

JS:   static f() {}
来源：http://yvn.fktsv.cn

TS:   static f(): void {}
来源：http://ski.ppjwa.cn

Java: static void f() {}
来源：http://npf.jianghu66.top


<!-- 参考信息 -->