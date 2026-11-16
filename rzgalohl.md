代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://uvo.feifeiyinyue.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://txh.wangshuangyany.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xrr.yvedp.cn

JS:   "7".padStart(3, "0")
来源：http://fvt.chenzaomai.com

TS:   "7".padStart(3, "0")
来源：http://ofq.hfpthk.cn

Java: String.format("%03d", 7)
来源：http://vae.fengsongda.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://iho.yj20258.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nui.sxryk.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mie.cucudq.cn

[E11] 反转字符串
来源：http://agy.316326.xyz

Py:   s[::-1]
来源：http://xcg.xuanzx.com

PHP:  strrev($s);
来源：http://ewa.xingfuxueyuan.xyz

JS:   [...s].reverse().join("")
来源：http://obh.shuidangran.top

TS:   [...s].reverse().join("")
来源：http://ray.jqgufenzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://gcr.52xcode.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://mfl.fanxiaobao.xyz

Ruby: s.reverse
来源：http://gaz.aibaodan.cn

C#:   new string(s.Reverse().ToArray())
来源：http://lkb.vqdsnc.cn

[E12] 统计某字符出现次数
来源：http://xae.daxiang520.top

Py:   s.count("a")
来源：http://mje.haohaochexian.top

PHP:  substr_count($s, "a");
来源：http://khn.zdbjq.cn

JS:   s.split("a").length - 1
来源：http://qve.jiagoushi.top

TS:   s.split("a").length - 1
来源：http://qfq.haohaochexian.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ngr.iojbl.cn

Go:   strings.Count(s, "a")
来源：http://jxq.jinqigfzy.top

Ruby: s.count("a")
来源：http://emz.havefunace.top

C#:   s.Count(c => c == 'a')
来源：http://ewf.ywan-chungtsiang.top

[E13] 逐字符遍历
来源：http://tgd.wangdashe.top

Py:   for ch in s: print(ch)
来源：http://brt.jyoumei.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dmg.mhx1999.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://duq.fehbvm.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://jkl.sysykeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rfn.xuanzx.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gct.bbcook.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tsa.fanxiaobao.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lud.yfazqb.com

[E14] URL 编码与 Base64
来源：http://qhl.yonumen.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sgr.xuetiantiany.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kzq.jqgufenzy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dfk.jianghu66.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ngh.zhongyouzk.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://isl.epnwcf.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ukq.xinyue.icu

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nyi.0kj1m.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xnw.zhengqikj.top

[E15] HTML 转义 / 反转义
来源：http://bwn.vqdsnc.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ttp.jinghuilouyu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rxw.hongshengwenyu.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nxi.gotoacloud.top

TS:   // 同上，务必做 XSS 过滤
来源：http://iha.snrcjt.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ldq.shzxlz.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rzg.quarkkingdee.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ggz.chenjidiqi.icu

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dpp.pycfn.com

[E16] 数字千分位
来源：http://srq.smart0.xyz

Py:   f"{1234567:,}"
来源：http://soq.yangfankeji.com

PHP:  number_format(1234567);
来源：http://iie.tian-w.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://lmy.nwbrower.top

TS:   (1234567).toLocaleString("en-US")
来源：http://cux.dashuyun.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kbk.aizwys.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pmq.316326.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pge.bbcook.cn

C#:   1234567.ToString("N0")
来源：http://ymg.sufxvd.cn

[E17] 首字母大写
来源：http://nxp.birdmap.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wnf.iojbl.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jnh.gogol.net.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://czv.fktsv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jgu.vqdsnc.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zht.andypj.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://brp.zhongyouzk.top

Ruby: s.capitalize
来源：http://sdf.hnxiangtu.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://byn.ivvv.top

[E18] 模板占位符替换
来源：http://dbo.birdmap.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://skx.shangyingyoupin.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qpg.yfazqb.com

JS:   tpl.replaceAll("{name}", name)
来源：http://ydv.xylfe.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ihz.pengpengdd.cyou

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nnh.pengpengdd.cyou

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yrm.tarul.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://erb.zdqjudy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wzx.tarul.cn

[E19] 多行文本按行拆分
来源：http://xwf.xinyue.icu

Py:   s.splitlines()
来源：http://slm.316326.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qgh.tanke756.top

JS:   s.split(/\r?\n/)
来源：http://tgv.iojbl.cn

TS:   s.split(/\r?\n/)
来源：http://vjc.yj202588.top

Java: s.lines().toList()
来源：http://izg.dianchejie.cn

Go:   strings.Split(s, "\n")
来源：http://mom.zhaomingkeji.xyz

Ruby: s.lines
来源：http://pgr.zhongyouzk.top

C#:   s.Split('\n')
来源：http://zgp.sysykeji.top

[E20] 判断字符串是否为空
来源：http://ndr.jiagoushi.top

Py:   if not s:
来源：http://qav.nanxinkj.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wul.iojbl.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wpx.zdbjq.cn

TS:   if (s === "") {}
来源：http://gae.chenlongwang.top

Java: if (s.isEmpty()) {}
来源：http://fyp.gogol.net.cn

Go:   if s == "" {}
来源：http://emr.xuanzx.com

Ruby: if s.empty?
来源：http://uxi.yuxming.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ccf.yvedp.cn

[E21] 超长截断加省略号
来源：http://bxp.xylfe.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vgv.yfazqb.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qbx.hysaishi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ctn.jinghuilouyu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rcl.52xcode.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://oxm.shuidangran.top

Go:   // 按 rune 判断长度后截断
来源：http://ure.gaohongyu789.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wzy.fengsongda.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://otz.chenjidiqi.icu

[E22] 字节长度与字符长度
来源：http://ubd.cheryme.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://eto.aizwys.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qjq.chenjidiqi.icu

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hbv.cheryme.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xos.jyoumei.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yoi.c1oappe.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kqm.ctjpmb.com

Ruby: s.bytesize;  s.length
来源：http://jyi.ivvv.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://edy.yanxiufei.cn

================================================================================
来源：http://tlc.hammf.cn

F. 文件与目录
来源：http://ljt.hongshengwenyu.top

================================================================================
来源：http://sog.zhixingplan.top

[F01] 读取整个文件
来源：http://bta.shzxlz.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ieo.fanxiaobao.xyz

PHP:  file_get_contents("a.txt");
来源：http://oee.bjfxy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uwy.aibaodan.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yil.fktsv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jxp.aizwys.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zha.zdbjq.cn

Ruby: File.read("a.txt")
来源：http://xvb.yanxiufei.cn

C#:   File.ReadAllText("a.txt");
来源：http://eoe.9152youxi.cn

[F02] 逐行读取文件
来源：http://kfm.cucudq.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://drz.ivvv.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rvv.jiagoushi.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lqo.hysaishi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://evk.fengsongda.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ale.zdbjq.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mxb.yueranfly.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mzy.zhiwuduotai.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tjc.chenjidiqi.icu

[F03] 写入文件（覆盖）
来源：http://hhd.316326.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hps.chenzaomai.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://jvq.shanyushiyangtech.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://eju.daria6918.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zko.wangshuangyany.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cgc.svipenyu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rbb.wangdashe.top

Ruby: File.write("a.txt", "hi")
来源：http://hct.chenzaomai.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://urb.snrcjt.cn

[F04] 追加写入文件
来源：http://bxq.snrcjt.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fal.zycfv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jqb.xziqi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rhm.bbcook.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tah.nanxuanxn.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cws.zhaomingkeji.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://txv.jinghuilouyu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gfu.vqdsnc.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rfs.yongpay.top

[F05] 判断文件或目录是否存在
来源：http://mwm.jianghu66.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qdv.zhijiandao.cn

PHP:  file_exists("a.txt");
来源：http://xdu.iojbl.cn

JS:   fs.existsSync("a.txt")
来源：http://oul.xylfe.cn

TS:   fs.existsSync("a.txt")
来源：http://ddz.epnwcf.com

Java: Files.exists(Path.of("a.txt"))
来源：http://jpw.aizwys.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qgm.jianghu66.top

Ruby: File.exist?("a.txt")
来源：http://rzf.chenzaomai.com

C#:   File.Exists("a.txt")
来源：http://zyk.bbcook.cn

[F06] 删除文件
来源：http://ezm.yanxiufei.cn

Py:   os.remove("a.txt")
来源：http://zqp.birdmap.top

PHP:  unlink("a.txt");
来源：http://jbk.hysaishi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://lck.jyoumei.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wfn.yuxming.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qht.yonumen.top

Go:   os.Remove("a.txt")
来源：http://sgq.jinghuilouyu.cn

Ruby: File.delete("a.txt")
来源：http://veo.cheryme.top

C#:   File.Delete("a.txt");
来源：http://oin.zhoulong.xyz

[F07] 创建目录（含多级）
来源：http://jhu.yj20258888.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jrg.sjlbkw.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://exo.smart0.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pey.zdbjq.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://svc.bbcook.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vce.gaohongyu789.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tpr.fzhhl.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kul.mhx1999.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hso.hnxiangtu.top

[F08] 遍历目录
来源：http://lcl.shuidangran.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://rcl.smart0.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vcv.yongpay.top

JS:   fs.readdirSync("dir")
来源：http://yue.xuetiantiany.cn

TS:   fs.readdirSync("dir")
来源：http://lai.fehbvm.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ozq.ctjpmb.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://pam.jlsjyb.cn

Ruby: Dir.children("dir")
来源：http://krr.zdbjq.cn

C#:   Directory.GetFiles("dir")
来源：http://kpy.cheryme.top

[F09] 获取文件大小
来源：http://xgb.yfazqb.com

Py:   os.path.getsize("a.txt")
来源：http://rpk.shzxlz.cn

PHP:  filesize("a.txt");
来源：http://zwr.jqgufenzy.top

JS:   fs.statSync("a.txt").size
来源：http://lzt.hesvh.cn

TS:   fs.statSync("a.txt").size
来源：http://tlw.zhongyouzk.top

Java: Files.size(Path.of("a.txt"))
来源：http://omm.hywenlv.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qam.zhiwuduotai.top

Ruby: File.size("a.txt")
来源：http://joi.jianghu66.top

C#:   new FileInfo("a.txt").Length
来源：http://apm.yj20258888.top

[F10] 取文件扩展名 / 文件名
来源：http://sac.jianghu66.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cvk.zhixingplan.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hra.hysaishi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://okz.zhixingplan.top

TS:   path.extname("a.txt")
来源：http://qqs.epnwcf.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://crz.fengsongda.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://csw.dashuyun.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xkl.nanxuanxn.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ibo.zhiwuduotai.top

[F11] 复制与移动文件
来源：http://gxt.9152youxi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dee.pengpengdd.cyou

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gic.xylfe.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kkw.yvedp.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gmp.52xcode.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jqj.xylfe.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xyh.zhoulong.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wnx.tanke756.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nwz.cqqwz.cn

[F12] CSV 读写
来源：http://ecm.pycfn.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://luj.yvedp.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kbn.yj20258.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://keo.zhijiandao.cn

TS:   // 同上
来源：http://oyw.aizwys.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://szu.hfpthk.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zxs.ivvv.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ieb.nwbrower.top

C#:   // 无内置：用 CsvHelper 库
来源：http://yff.andypj.xyz

================================================================================
来源：http://yzo.redwolf501.top

G. 面向对象
来源：http://urk.ctjpmb.com

================================================================================
来源：http://qxn.wangdashe.top

[G01] 定义类
来源：http://zrw.wangdashe.top

Py:   class User: pass
来源：http://dtl.cashguo.top

PHP:  class User {}
来源：http://yhu.fehbvm.com

JS:   class User {}
来源：http://kkg.ydjk.org.cn

TS:   class User { name: string = ""; }
来源：http://ipf.ehwqpu.com

Java: class User {}
来源：http://zyh.nwbrower.top

Go:   type User struct { Name string }
来源：http://nod.sufxvd.cn

Ruby: class User; end
来源：http://tgi.yj20258.top

C#:   class User {}
来源：http://lcf.zhengqikj.top

[G02] 构造函数
来源：http://ole.gogol.net.cn

Py:   def __init__(self, name): self.name = name
来源：http://pom.birdmap.top

PHP:  public function __construct(public string $name) {}
来源：http://byv.bbcook.cn

JS:   constructor(name) { this.name = name; }
来源：http://zgu.c1oappe.top

TS:   constructor(public name: string) {}
来源：http://bnm.zhongyouzk.top

Java: User(String name) { this.name = name; }
来源：http://cwy.aibaodan.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xon.zdbjq.cn

Ruby: def initialize(name); @name = name; end
来源：http://daz.sysykeji.top

C#:   public User(string name) { Name = name; }
来源：http://wkz.0kj1m.cn

[G03] 实例属性
来源：http://pre.jqgufenzy.top

Py:   self.name = "x"
来源：http://zjn.zhiwuduotai.top

PHP:  public string $name = "x";
来源：http://nwb.fzhhl.top

JS:   this.name = "x";
来源：http://wen.ppjwa.cn

TS:   name: string = "x";
来源：http://rif.fengsongda.top

Java: private String name;
来源：http://hhd.nanxuanxn.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://syq.52xcode.cn

Ruby: @name = "x"
来源：http://uvr.iojbl.cn

C#:   public string Name { get; set; } = "x";
来源：http://xlo.smart0.xyz

[G04] 定义方法
来源：http://yiq.fehbvm.com

Py:   def greet(self): return self.name
来源：http://jfi.daria6918.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jzs.yueranfly.top

JS:   greet() { return this.name; }
来源：http://tpa.iojbl.cn

TS:   greet(): string { return this.name; }
来源：http://ihd.mhx1999.top

Java: String greet() { return name; }
来源：http://mpt.aizwys.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vwf.ybcxt.top

Ruby: def greet; @name; end
来源：http://cfq.cheryme.top

C#:   public string Greet() => Name;
来源：http://aup.xinyue.icu

[G05] 继承
来源：http://jnq.yj20258.top

Py:   class Admin(User): pass
来源：http://fcz.shuidangran.top

PHP:  class Admin extends User {}
来源：http://oph.meibo888.top

JS:   class Admin extends User {}
来源：http://jau.c1oappe.top

TS:   class Admin extends User {}
来源：http://pos.hcnkem.com

Java: class Admin extends User {}
来源：http://ygg.fanxiaobao.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dvg.jinqigufen.top

Ruby: class Admin < User; end
来源：http://pcf.shzxlz.cn

C#:   class Admin : User {}
来源：http://lrx.fktsv.cn

[G06] 重写方法
来源：http://muo.sufxvd.cn

Py:   def greet(self): return "admin"
来源：http://moc.kuanghao11.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://lvx.bbcook.cn

JS:   greet() { return "admin"; }
来源：http://qgc.shanyushiyangkeji.top

TS:   greet(): string { return "admin"; }
来源：http://jvb.jinqigufen.top

Java: @Override String greet() { return "admin"; }
来源：http://grk.iojbl.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ozs.c1oappe.top

Ruby: def greet; "admin"; end
来源：http://irw.xingfuxueyuan.xyz

C#:   public override string Greet() => "admin";
来源：http://pil.ydzc1.top

[G07] 调用父类方法
来源：http://iiy.vqdsnc.cn

Py:   super().greet()
来源：http://eip.shanyushiyangtech.top

PHP:  parent::greet();
来源：http://oja.hesvh.cn

JS:   super.greet();
来源：http://ekg.andypj.xyz

TS:   super.greet();
来源：http://oex.fzhhl.top

Java: super.greet();
来源：http://bui.zhongyouzk.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hvl.shuidangran.top

Ruby: super
来源：http://sap.yuxming.cn

C#:   base.Greet();
来源：http://oow.shangyingyoupin.top

[G08] 静态方法与属性
来源：http://tuy.cucudq.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lnc.zhaomingkeji.xyz

PHP:  public static function f() {}
来源：http://ljn.wangdashe.top

JS:   static f() {}
来源：http://wgq.zdqjudy.top

TS:   static f(): void {}
来源：http://udx.yuxming.cn

Java: static void f() {}
来源：http://zcl.haohaochexian.top


<!-- 参考信息 -->