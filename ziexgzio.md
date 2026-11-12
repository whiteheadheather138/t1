代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://xmv.meibo888.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zfd.pengpengdd.cyou

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cwq.cdnleiting.top

JS:   "7".padStart(3, "0")
来源：http://kul.aizwys.cn

TS:   "7".padStart(3, "0")
来源：http://sxm.chenzaomai.com

Java: String.format("%03d", 7)
来源：http://imj.ydjk.org.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://poz.jqgfzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qto.gogol.net.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zvk.vehdjk.com

[E11] 反转字符串
来源：http://emh.xuetiantiany.cn

Py:   s[::-1]
来源：http://fvu.chenzaomai.com

PHP:  strrev($s);
来源：http://opp.tanke756.top

JS:   [...s].reverse().join("")
来源：http://stb.zhaomingkeji.xyz

TS:   [...s].reverse().join("")
来源：http://hpe.ppjwa.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hyl.jinyuanbaomall.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://org.zhixingplan.top

Ruby: s.reverse
来源：http://mvn.nanxinkj.top

C#:   new string(s.Reverse().ToArray())
来源：http://wim.vqdsnc.cn

[E12] 统计某字符出现次数
来源：http://iyn.hesvh.cn

Py:   s.count("a")
来源：http://dai.hywenlv.cn

PHP:  substr_count($s, "a");
来源：http://hwu.snrcjt.cn

JS:   s.split("a").length - 1
来源：http://gdr.dashuyun.cn

TS:   s.split("a").length - 1
来源：http://kce.yangfankeji.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xng.ivvv.top

Go:   strings.Count(s, "a")
来源：http://wwn.mhx1999.top

Ruby: s.count("a")
来源：http://dbv.jianghu66.top

C#:   s.Count(c => c == 'a')
来源：http://xku.sxryk.cn

[E13] 逐字符遍历
来源：http://qqq.fktsv.cn

Py:   for ch in s: print(ch)
来源：http://jfi.shanyushiyangtech.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gap.cqqwz.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fzj.jyoumei.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fxd.tianlin.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kam.epnwcf.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://iue.chenjidiqi.icu

Ruby: s.each_char { |ch| puts ch }
来源：http://dpv.sjlbkw.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zwm.sjlbkw.cn

[E14] URL 编码与 Base64
来源：http://xad.hywenlv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rzm.jlsjyb.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://whn.yvedp.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nmq.jqgufenzy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gjt.hysaishi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qdx.yangfankeji.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://glw.cdnleiting.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lmt.vehdjk.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://med.shuidangran.top

[E15] HTML 转义 / 反转义
来源：http://nll.fehbvm.com

Py:   html.escape(s);  html.unescape(s)
来源：http://rvb.epnwcf.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uxi.hnqzz.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mwf.c1oappe.top

TS:   // 同上，务必做 XSS 过滤
来源：http://vzr.gogol.net.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xew.cheryme.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fxz.shzxlz.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jqq.sxryk.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pmo.hysaishi.cn

[E16] 数字千分位
来源：http://mfb.wangshuangyany.cn

Py:   f"{1234567:,}"
来源：http://aez.yongpay.top

PHP:  number_format(1234567);
来源：http://bae.hfpthk.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://yqj.jinqigufen.top

TS:   (1234567).toLocaleString("en-US")
来源：http://zkq.0kj1m.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fuq.hammf.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lqt.yuanzhike.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cfp.hywenlv.cn

C#:   1234567.ToString("N0")
来源：http://cjq.nwbrower.top

[E17] 首字母大写
来源：http://yoy.xuetiantiany.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bry.jqgufenzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://giy.0kj1m.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sta.gzhubu.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vah.yj202588.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lqu.pengpengdd.cyou

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nwc.bjfxy.top

Ruby: s.capitalize
来源：http://yyk.shzxlz.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zxy.fzhhl.top

[E18] 模板占位符替换
来源：http://egr.chenlongwang.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rbu.xuetiantiany.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xng.yfazqb.com

JS:   tpl.replaceAll("{name}", name)
来源：http://dei.fktsv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://kqj.meibo888.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kas.havefunace.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nxo.hesvh.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rca.smart0.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wfr.hesvh.cn

[E19] 多行文本按行拆分
来源：http://cfw.iojbl.cn

Py:   s.splitlines()
来源：http://aex.shanyushiyangtech.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jpj.ehwqpu.com

JS:   s.split(/\r?\n/)
来源：http://pxw.ctjpmb.com

TS:   s.split(/\r?\n/)
来源：http://qmu.cucudq.cn

Java: s.lines().toList()
来源：http://sfq.zhiwuduotai.top

Go:   strings.Split(s, "\n")
来源：http://nzv.hammf.cn

Ruby: s.lines
来源：http://dtz.cdnleiting.top

C#:   s.Split('\n')
来源：http://uye.zhongyouzk.top

[E20] 判断字符串是否为空
来源：http://rwx.hongshengwenyu.top

Py:   if not s:
来源：http://pva.zycfv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cve.yj202588.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fyj.xuetiantiany.cn

TS:   if (s === "") {}
来源：http://wsw.tian-w.cn

Java: if (s.isEmpty()) {}
来源：http://ouw.ppjwa.cn

Go:   if s == "" {}
来源：http://mja.dianchejie.cn

Ruby: if s.empty?
来源：http://jfy.aizwys.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kgo.fehbvm.com

[E21] 超长截断加省略号
来源：http://axj.vehdjk.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://oaj.ehwqpu.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gjq.jinqigufen.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ufk.yuxming.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yzx.yvedp.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wwy.c1oappe.top

Go:   // 按 rune 判断长度后截断
来源：http://eem.0kj1m.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://map.quarkkingdee.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mpd.shangyingyoupin.top

[E22] 字节长度与字符长度
来源：http://ucf.cashguo.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bos.shangyingyoupin.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vgt.fengsongda.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zkm.shuidangran.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ska.jqgufenzy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mvw.zhoulong.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://igu.fzhhl.top

Ruby: s.bytesize;  s.length
来源：http://whx.sxryk.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://csd.zycfv.cn

================================================================================
来源：http://bwx.nwbrower.top

F. 文件与目录
来源：http://blv.xylfe.cn

================================================================================
来源：http://yxa.feifeiyinyue.top

[F01] 读取整个文件
来源：http://xxx.cqqwz.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kcn.yueranfly.top

PHP:  file_get_contents("a.txt");
来源：http://zcl.fktsv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kgx.aibaodan.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dbr.zycfv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zcf.jlsjyb.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ecg.wangdashe.top

Ruby: File.read("a.txt")
来源：http://ggd.hesvh.cn

C#:   File.ReadAllText("a.txt");
来源：http://imp.shuidangran.top

[F02] 逐行读取文件
来源：http://sum.pycfn.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tcf.jinyuanbaomall.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ufv.sjlbkw.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jvo.zhoulong.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uua.c1oappe.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ybv.chenlongwang.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zas.zhengqikj.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fqs.yj202588.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://erm.kuanghao11.cn

[F03] 写入文件（覆盖）
来源：http://qeu.aibaodan.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bgb.xuetiantiany.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://jnl.redwolf501.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://piw.bbcook.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xua.guowangkeji.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tbl.hesvh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jkr.zdbjq.cn

Ruby: File.write("a.txt", "hi")
来源：http://vzo.mhx1999.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ith.jinqigufen.top

[F04] 追加写入文件
来源：http://yqd.tarul.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://prg.hywenlv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jck.0kj1m.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ofh.316326.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ytm.fanxiaobao.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ldv.tanke756.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wdo.jqgfzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qyk.andypj.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://grt.guannengcc.top

[F05] 判断文件或目录是否存在
来源：http://xzg.vqdsnc.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xen.pycfn.com

PHP:  file_exists("a.txt");
来源：http://tva.52xcode.cn

JS:   fs.existsSync("a.txt")
来源：http://ros.havefunace.top

TS:   fs.existsSync("a.txt")
来源：http://xrq.xuanzx.com

Java: Files.exists(Path.of("a.txt"))
来源：http://loh.zhongyouzk.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://utb.quarkkingdee.top

Ruby: File.exist?("a.txt")
来源：http://gqr.316326.xyz

C#:   File.Exists("a.txt")
来源：http://bsw.hesvh.cn

[F06] 删除文件
来源：http://vog.jianghu66.top

Py:   os.remove("a.txt")
来源：http://qcf.xuetiantiany.cn

PHP:  unlink("a.txt");
来源：http://gld.daria6918.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wpx.iojbl.cn

TS:   fs.unlinkSync("a.txt")
来源：http://azw.yangfankeji.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://upy.ppjwa.cn

Go:   os.Remove("a.txt")
来源：http://nuo.cucudq.cn

Ruby: File.delete("a.txt")
来源：http://doz.yanxiufei.cn

C#:   File.Delete("a.txt");
来源：http://leo.zdqjudy.top

[F07] 创建目录（含多级）
来源：http://hlp.xingfuxueyuan.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ksv.quarkkingdee.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://myk.fengsongda.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://obs.daria6918.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hfg.hesvh.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://aek.cashguo.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bhv.yuxming.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mdz.yangfankeji.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dqj.cucudq.cn

[F08] 遍历目录
来源：http://nej.svipenyu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://spa.xinyue.icu

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gxx.zhongyouzk.top

JS:   fs.readdirSync("dir")
来源：http://knt.svipenyu.cn

TS:   fs.readdirSync("dir")
来源：http://gqc.hywenlv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ijt.ehwqpu.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://cyq.zhijiandao.cn

Ruby: Dir.children("dir")
来源：http://nqf.dianchejie.cn

C#:   Directory.GetFiles("dir")
来源：http://xzz.yj20258888.top

[F09] 获取文件大小
来源：http://wvv.gotoacloud.top

Py:   os.path.getsize("a.txt")
来源：http://uik.aibaodan.cn

PHP:  filesize("a.txt");
来源：http://aom.zhengqikj.top

JS:   fs.statSync("a.txt").size
来源：http://xzx.cucudq.cn

TS:   fs.statSync("a.txt").size
来源：http://iud.hammf.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zzv.yj20258.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zfq.ydjk.org.cn

Ruby: File.size("a.txt")
来源：http://lmp.hywenlv.cn

C#:   new FileInfo("a.txt").Length
来源：http://cxe.fzhhl.top

[F10] 取文件扩展名 / 文件名
来源：http://tgz.chenlongwang.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ybl.zhoulong.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vzi.guowangkeji.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rbb.jiagoushi.top

TS:   path.extname("a.txt")
来源：http://olz.52xcode.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jdb.cdnleiting.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dch.zycfv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dwj.xingfuxueyuan.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ybd.fktsv.cn

[F11] 复制与移动文件
来源：http://ren.uphjek.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vsn.hysaishi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rfz.fktsv.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pkx.snrcjt.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mdv.yfazqb.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://amb.yanxiufei.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gca.tianlin.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kdl.mhx1999.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://eyt.pengpengdd.cyou

[F12] CSV 读写
来源：http://yas.pycfn.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uht.gzhubu.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://avz.jinyuanbaomall.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mhp.gzhubu.top

TS:   // 同上
来源：http://jhz.sysykeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jzh.ctjpmb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ufx.nanxinkj.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ftr.smart0.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://mto.pycfn.com

================================================================================
来源：http://ami.hongshengwenyu.top

G. 面向对象
来源：http://ryq.yongpay.top

================================================================================
来源：http://hei.ctjpmb.com

[G01] 定义类
来源：http://gmi.snrcjt.cn

Py:   class User: pass
来源：http://woq.zhongyouzk.top

PHP:  class User {}
来源：http://klz.jlsjyb.cn

JS:   class User {}
来源：http://aau.cucudq.cn

TS:   class User { name: string = ""; }
来源：http://uan.pycfn.com

Java: class User {}
来源：http://oaa.yfazqb.com

Go:   type User struct { Name string }
来源：http://ltg.chenjidiqi.icu

Ruby: class User; end
来源：http://knh.xziqi.cn

C#:   class User {}
来源：http://yio.xinyue.icu

[G02] 构造函数
来源：http://ldg.zdqjudy.top

Py:   def __init__(self, name): self.name = name
来源：http://kcu.jlsjyb.cn

PHP:  public function __construct(public string $name) {}
来源：http://jmg.hnxiangtu.top

JS:   constructor(name) { this.name = name; }
来源：http://lqo.52xcode.cn

TS:   constructor(public name: string) {}
来源：http://pnn.quarkkingdee.top

Java: User(String name) { this.name = name; }
来源：http://eef.zhijiandao.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jrn.fengsongda.top

Ruby: def initialize(name); @name = name; end
来源：http://rea.shangyingyoupin.top

C#:   public User(string name) { Name = name; }
来源：http://dbv.ywan-chungtsiang.top

[G03] 实例属性
来源：http://lsf.zhijiandao.cn

Py:   self.name = "x"
来源：http://dla.c1oappe.top

PHP:  public string $name = "x";
来源：http://tsx.daria6918.cn

JS:   this.name = "x";
来源：http://kir.bjfxy.top

TS:   name: string = "x";
来源：http://yka.xinyue.icu

Java: private String name;
来源：http://iod.zhongyouzk.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sel.cashguo.top

Ruby: @name = "x"
来源：http://mrg.guowangkeji.top

C#:   public string Name { get; set; } = "x";
来源：http://oxp.fanxiaobao.xyz

[G04] 定义方法
来源：http://erz.yj202588.top

Py:   def greet(self): return self.name
来源：http://eki.chenlongwang.top

PHP:  public function greet(): string { return $this->name; }
来源：http://smf.hfpthk.cn

JS:   greet() { return this.name; }
来源：http://bwd.wangdashe.top

TS:   greet(): string { return this.name; }
来源：http://vlo.hysaishi.cn

Java: String greet() { return name; }
来源：http://pkm.gotoacloud.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://dqv.gogol.net.cn

Ruby: def greet; @name; end
来源：http://zzg.cqqwz.cn

C#:   public string Greet() => Name;
来源：http://ktr.jqgfzy.top

[G05] 继承
来源：http://tzv.ywan-chungtsiang.top

Py:   class Admin(User): pass
来源：http://jbk.shanyushiyangkeji.top

PHP:  class Admin extends User {}
来源：http://ldl.hywenlv.cn

JS:   class Admin extends User {}
来源：http://vto.yuanzhike.top

TS:   class Admin extends User {}
来源：http://njc.snrcjt.cn

Java: class Admin extends User {}
来源：http://tvy.cqqwz.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://sxn.yj202588.top

Ruby: class Admin < User; end
来源：http://sdk.ybcxt.top

C#:   class Admin : User {}
来源：http://sgw.cdnleiting.top

[G06] 重写方法
来源：http://tyw.xuanzx.com

Py:   def greet(self): return "admin"
来源：http://kcv.hnqzz.top

PHP:  public function greet(): string { return "admin"; }
来源：http://hyn.hnxiangtu.top

JS:   greet() { return "admin"; }
来源：http://tvn.kuanghao11.cn

TS:   greet(): string { return "admin"; }
来源：http://rzs.svipenyu.cn

Java: @Override String greet() { return "admin"; }
来源：http://vei.zdqjudy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oow.uphjek.com

Ruby: def greet; "admin"; end
来源：http://dvl.9152youxi.cn

C#:   public override string Greet() => "admin";
来源：http://bso.cheryme.top

[G07] 调用父类方法
来源：http://mdb.cucudq.cn

Py:   super().greet()
来源：http://ijb.cheryme.top

PHP:  parent::greet();
来源：http://htg.sysykeji.top

JS:   super.greet();
来源：http://vbq.hysaishi.cn

TS:   super.greet();
来源：http://yvy.52xcode.cn

Java: super.greet();
来源：http://nwz.svipenyu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dxt.guowangkeji.top

Ruby: super
来源：http://hxs.hesvh.cn

C#:   base.Greet();
来源：http://uuv.meibo888.top

[G08] 静态方法与属性
来源：http://zul.0kj1m.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://luq.ctjpmb.com

PHP:  public static function f() {}
来源：http://pfy.shuidangran.top

JS:   static f() {}
来源：http://use.dashuyun.cn

TS:   static f(): void {}
来源：http://sse.dashuyun.cn

Java: static void f() {}
来源：http://uth.xinyue.icu


<!-- 参考信息 -->