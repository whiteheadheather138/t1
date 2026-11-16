代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://pjk.jqgufenzy.top

Java: String.format("%03d", 7)
来源：http://qrv.zhoulong.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://uzb.zhengqikj.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nqt.epnwcf.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pen.yonumen.top

[E11] 反转字符串
来源：http://tuf.bbcook.cn

Py:   s[::-1]
来源：http://ikm.jinqigufen.top

PHP:  strrev($s);
来源：http://dvk.dianchejie.cn

JS:   [...s].reverse().join("")
来源：http://nku.zhijiandao.cn

TS:   [...s].reverse().join("")
来源：http://tkv.tarul.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mbm.yfazqb.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://ram.hammf.cn

Ruby: s.reverse
来源：http://kng.zhijiandao.cn

C#:   new string(s.Reverse().ToArray())
来源：http://yls.epnwcf.com

[E12] 统计某字符出现次数
来源：http://udh.yvedp.cn

Py:   s.count("a")
来源：http://xhi.ydzc1.top

PHP:  substr_count($s, "a");
来源：http://vxu.yj20258.top

JS:   s.split("a").length - 1
来源：http://kba.shanyushiyangtech.top

TS:   s.split("a").length - 1
来源：http://czp.cdnleiting.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://njn.haohaochexian.top

Go:   strings.Count(s, "a")
来源：http://ood.sxryk.cn

Ruby: s.count("a")
来源：http://xxa.zycfv.cn

C#:   s.Count(c => c == 'a')
来源：http://stj.ybcxt.top

[E13] 逐字符遍历
来源：http://jyd.chenlongwang.top

Py:   for ch in s: print(ch)
来源：http://xiy.yj202588.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mra.gotoacloud.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://tka.ydzc1.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://far.gogol.net.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yzx.sweek.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qgc.ybcxt.top

Ruby: s.each_char { |ch| puts ch }
来源：http://tbs.wangshuangyany.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pmo.shangyingyoupin.top

[E14] URL 编码与 Base64
来源：http://hue.c1oappe.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hix.dashuyun.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://end.aizwys.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://weo.c1oappe.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ikq.sufxvd.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dpc.hongshengwenyu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lkq.meibo888.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gxb.epnwcf.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pfu.dashuyun.cn

[E15] HTML 转义 / 反转义
来源：http://ncb.hysaishi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wrp.iojbl.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xwj.yongpay.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://umr.yj20258.top

TS:   // 同上，务必做 XSS 过滤
来源：http://xfp.xylfe.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ben.xingfuxueyuan.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rbv.316326.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bdh.ydjk.org.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wue.zhixingplan.top

[E16] 数字千分位
来源：http://xuh.shzxlz.cn

Py:   f"{1234567:,}"
来源：http://mlx.jinyuanbaomall.cn

PHP:  number_format(1234567);
来源：http://las.zhoulong.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://rxe.9152youxi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://bme.sjlbkw.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xly.chenjidiqi.icu

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gie.sjlbkw.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://oqj.chenlongwang.top

C#:   1234567.ToString("N0")
来源：http://cne.meibo888.top

[E17] 首字母大写
来源：http://mmo.zdqjudy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bil.aizwys.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://thj.iojbl.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xvs.yonumen.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ghu.bbcook.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://alu.zhiwuduotai.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uai.ybcxt.top

Ruby: s.capitalize
来源：http://sbj.zhijiandao.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dau.hnqzz.top

[E18] 模板占位符替换
来源：http://lug.ppjwa.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://irr.quarkkingdee.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jni.ppjwa.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://rsr.316326.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://eaz.daxiang520.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://prz.yfazqb.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://frp.gogol.net.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ldw.ywan-chungtsiang.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://eud.cdnleiting.top

[E19] 多行文本按行拆分
来源：http://kxf.316326.xyz

Py:   s.splitlines()
来源：http://wst.hongshengwenyu.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xmf.52xcode.cn

JS:   s.split(/\r?\n/)
来源：http://wqo.ywan-chungtsiang.top

TS:   s.split(/\r?\n/)
来源：http://ojt.pengpengdd.cyou

Java: s.lines().toList()
来源：http://vaw.ppjwa.cn

Go:   strings.Split(s, "\n")
来源：http://oov.sweek.top

Ruby: s.lines
来源：http://ctw.gotoacloud.top

C#:   s.Split('\n')
来源：http://gbh.tian-w.cn

[E20] 判断字符串是否为空
来源：http://kew.aibaodan.cn

Py:   if not s:
来源：http://lha.zhijiandao.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fkv.ywan-chungtsiang.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tmj.svipenyu.cn

TS:   if (s === "") {}
来源：http://nas.hysaishi.cn

Java: if (s.isEmpty()) {}
来源：http://khf.ybcxt.top

Go:   if s == "" {}
来源：http://jte.sysykeji.top

Ruby: if s.empty?
来源：http://ppx.fehbvm.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nui.hnqzz.top

[E21] 超长截断加省略号
来源：http://vss.ybcxt.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wfr.dianchejie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nbs.xinyue.icu

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rgw.ivvv.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dtw.meibo888.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qah.9152youxi.cn

Go:   // 按 rune 判断长度后截断
来源：http://sxm.yonumen.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hrl.yuxming.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nzo.yuxming.cn

[E22] 字节长度与字符长度
来源：http://fqc.hammf.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nah.wangdashe.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jmx.guowangkeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mqy.yj20258.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gnr.zycfv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pfw.haohaochexian.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xwu.zhongyouzk.top

Ruby: s.bytesize;  s.length
来源：http://qiz.kuanghao11.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ams.tianlin.xyz

================================================================================
来源：http://nih.gogol.net.cn

F. 文件与目录
来源：http://fox.xylfe.cn

================================================================================
来源：http://ygl.feifeiyinyue.top

[F01] 读取整个文件
来源：http://cir.xylfe.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hls.shzxlz.cn

PHP:  file_get_contents("a.txt");
来源：http://hyb.gogol.net.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://oay.pengpengdd.cyou

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uzs.iojbl.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hzh.jinqigfzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qfh.yj20258888.top

Ruby: File.read("a.txt")
来源：http://wrq.redwolf501.top

C#:   File.ReadAllText("a.txt");
来源：http://vfd.ydzc1.top

[F02] 逐行读取文件
来源：http://neu.jiagoushi.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zdh.guowangkeji.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://icg.zhixingplan.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uzd.zhiwuduotai.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://htg.tian-w.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://eky.epnwcf.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xjn.shanyushiyangtech.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://oly.hcnkem.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://udo.jqgfzy.top

[F03] 写入文件（覆盖）
来源：http://bne.guannengcc.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vtg.snrcjt.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://kmn.smart0.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dvc.xinyue.icu

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gkj.pycfn.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jqj.dianchejie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dzc.chenzaomai.com

Ruby: File.write("a.txt", "hi")
来源：http://vpt.fanxiaobao.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://woa.316326.xyz

[F04] 追加写入文件
来源：http://dkv.sysykeji.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ebd.shanyushiyangtech.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://puy.xuanzx.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dge.sjlbkw.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oef.zhaomingkeji.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mbt.316326.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://eyc.jqgufenzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lmc.hammf.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://isx.iojbl.cn

[F05] 判断文件或目录是否存在
来源：http://sav.aizwys.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lmh.ehwqpu.com

PHP:  file_exists("a.txt");
来源：http://dsg.gzhubu.top

JS:   fs.existsSync("a.txt")
来源：http://wik.shanyushiyangkeji.top

TS:   fs.existsSync("a.txt")
来源：http://lmb.tarul.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://mwh.tanke756.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kjo.smart0.xyz

Ruby: File.exist?("a.txt")
来源：http://qmg.xuanzx.com

C#:   File.Exists("a.txt")
来源：http://lyo.jinqigufen.top

[F06] 删除文件
来源：http://xwj.jinghuilouyu.cn

Py:   os.remove("a.txt")
来源：http://bkg.cucudq.cn

PHP:  unlink("a.txt");
来源：http://dfz.52xcode.cn

JS:   fs.unlinkSync("a.txt")
来源：http://whi.zhijiandao.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vtt.kuanghao11.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pry.xziqi.cn

Go:   os.Remove("a.txt")
来源：http://oyh.iojbl.cn

Ruby: File.delete("a.txt")
来源：http://opy.yvedp.cn

C#:   File.Delete("a.txt");
来源：http://ywi.jinghuilouyu.cn

[F07] 创建目录（含多级）
来源：http://bik.yvedp.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qde.yongpay.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ckp.jqgufenzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dvm.bjfxy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fmb.ctjpmb.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://oob.fzhhl.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://had.zhoulong.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bbq.sweek.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qha.ybcxt.top

[F08] 遍历目录
来源：http://mvh.hongshengwenyu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://nen.zhijiandao.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hzw.zycfv.cn

JS:   fs.readdirSync("dir")
来源：http://dro.jiagoushi.top

TS:   fs.readdirSync("dir")
来源：http://vmp.cucudq.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vea.chenlongwang.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://rts.meibo888.top

Ruby: Dir.children("dir")
来源：http://mij.ppjwa.cn

C#:   Directory.GetFiles("dir")
来源：http://ria.xuetiantiany.cn

[F09] 获取文件大小
来源：http://xkv.hysaishi.cn

Py:   os.path.getsize("a.txt")
来源：http://wtt.zhengqikj.top

PHP:  filesize("a.txt");
来源：http://uls.yj20258888.top

JS:   fs.statSync("a.txt").size
来源：http://nka.birdmap.top

TS:   fs.statSync("a.txt").size
来源：http://fly.xingfuxueyuan.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://ziz.gzhubu.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gaz.smart0.xyz

Ruby: File.size("a.txt")
来源：http://ctr.pycfn.com

C#:   new FileInfo("a.txt").Length
来源：http://jll.chenzaomai.com

[F10] 取文件扩展名 / 文件名
来源：http://lmg.bjfxy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xvl.sxryk.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vwe.wangdashe.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yvc.fktsv.cn

TS:   path.extname("a.txt")
来源：http://eaw.wangshuangyany.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://opx.zhaomingkeji.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ryq.0kj1m.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yux.vehdjk.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qwm.jinqigfzy.top

[F11] 复制与移动文件
来源：http://rnh.daria6918.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uvh.yj202588.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://axy.aibaodan.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://frp.sysykeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pwu.birdmap.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cab.iojbl.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fhm.pycfn.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lnr.sjlbkw.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ztq.tarul.cn

[F12] CSV 读写
来源：http://bkt.pengpengdd.cyou

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vhp.zhixingplan.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yha.epnwcf.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jir.ehwqpu.com

TS:   // 同上
来源：http://vhj.epnwcf.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://esx.yj20258888.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://eyk.sweek.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://one.sweek.top

C#:   // 无内置：用 CsvHelper 库
来源：http://afa.smart0.xyz

================================================================================
来源：http://mdf.meibo888.top

G. 面向对象
来源：http://otl.yj20258888.top

================================================================================
来源：http://uah.shuidangran.top

[G01] 定义类
来源：http://qqz.hammf.cn

Py:   class User: pass
来源：http://yuo.wangshuangyany.cn

PHP:  class User {}
来源：http://lka.yfazqb.com

JS:   class User {}
来源：http://bta.ywan-chungtsiang.top

TS:   class User { name: string = ""; }
来源：http://dya.yuxming.cn

Java: class User {}
来源：http://lky.xuanzx.com

Go:   type User struct { Name string }
来源：http://jhi.feifeiyinyue.top

Ruby: class User; end
来源：http://wie.pengpengdd.cyou

C#:   class User {}
来源：http://iek.redwolf501.top

[G02] 构造函数
来源：http://vkk.andypj.xyz

Py:   def __init__(self, name): self.name = name
来源：http://szu.jinghuilouyu.cn

PHP:  public function __construct(public string $name) {}
来源：http://zot.tian-w.cn

JS:   constructor(name) { this.name = name; }
来源：http://ukf.nanxuanxn.top

TS:   constructor(public name: string) {}
来源：http://ohu.hywenlv.cn

Java: User(String name) { this.name = name; }
来源：http://ptd.pengpengdd.cyou

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kqq.jlsjyb.cn

Ruby: def initialize(name); @name = name; end
来源：http://aqs.cashguo.top

C#:   public User(string name) { Name = name; }
来源：http://pdh.feifeiyinyue.top

[G03] 实例属性
来源：http://pwu.mhx1999.top

Py:   self.name = "x"
来源：http://vsa.sjlbkw.cn

PHP:  public string $name = "x";
来源：http://lvn.9152youxi.cn

JS:   this.name = "x";
来源：http://kpg.shuidangran.top

TS:   name: string = "x";
来源：http://nvf.zdbjq.cn

Java: private String name;
来源：http://knw.daria6918.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lxq.guowangkeji.top

Ruby: @name = "x"
来源：http://gwy.nanxuanxn.top

C#:   public string Name { get; set; } = "x";
来源：http://yrj.ehwqpu.com

[G04] 定义方法
来源：http://vtt.ydjk.org.cn

Py:   def greet(self): return self.name
来源：http://xkm.zhaomingkeji.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://scm.9152youxi.cn

JS:   greet() { return this.name; }
来源：http://gec.pengpengdd.cyou

TS:   greet(): string { return this.name; }
来源：http://loy.haohaochexian.top

Java: String greet() { return name; }
来源：http://kkh.guannengcc.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://vmj.cqqwz.cn

Ruby: def greet; @name; end
来源：http://qxh.pengpengdd.cyou

C#:   public string Greet() => Name;
来源：http://mju.wangshuangyany.cn

[G05] 继承
来源：http://ath.pycfn.com

Py:   class Admin(User): pass
来源：http://ecr.xuetiantiany.cn

PHP:  class Admin extends User {}
来源：http://fri.smart0.xyz

JS:   class Admin extends User {}
来源：http://nma.hesvh.cn

TS:   class Admin extends User {}
来源：http://oam.jianghu66.top

Java: class Admin extends User {}
来源：http://bjq.xylfe.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://aql.9152youxi.cn

Ruby: class Admin < User; end
来源：http://gye.jinqigfzy.top

C#:   class Admin : User {}
来源：http://vhb.vehdjk.com

[G06] 重写方法
来源：http://gzl.cucudq.cn

Py:   def greet(self): return "admin"
来源：http://bvr.jiagoushi.top

PHP:  public function greet(): string { return "admin"; }
来源：http://aqs.jinghuilouyu.cn

JS:   greet() { return "admin"; }
来源：http://hzp.hnxiangtu.top

TS:   greet(): string { return "admin"; }
来源：http://mqh.zdqjudy.top

Java: @Override String greet() { return "admin"; }
来源：http://jjl.316326.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cat.jiagoushi.top

Ruby: def greet; "admin"; end
来源：http://eky.ywan-chungtsiang.top

C#:   public override string Greet() => "admin";
来源：http://dro.shzxlz.cn

[G07] 调用父类方法
来源：http://clt.jinyuanbaomall.cn

Py:   super().greet()
来源：http://jwk.snrcjt.cn

PHP:  parent::greet();
来源：http://icr.yfazqb.com

JS:   super.greet();
来源：http://jjz.zhijiandao.cn

TS:   super.greet();
来源：http://woi.ydzc1.top

Java: super.greet();
来源：http://mgu.jinqigufen.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pdu.aizwys.cn

Ruby: super
来源：http://rmd.cashguo.top

C#:   base.Greet();
来源：http://ulp.epnwcf.com

[G08] 静态方法与属性
来源：http://ewb.hnqzz.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zjq.andypj.xyz

PHP:  public static function f() {}
来源：http://czt.birdmap.top

JS:   static f() {}
来源：http://bwb.ehwqpu.com

TS:   static f(): void {}
来源：http://xwl.52xcode.cn

Java: static void f() {}
来源：http://rwx.shanyushiyangtech.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://sbd.zdqjudy.top

Ruby: def self.f; end
来源：http://jbp.jinghuilouyu.cn

C#:   public static void F() {}
来源：http://zbl.vqdsnc.cn

[G09] 接口 / 抽象类
来源：http://jkt.c1oappe.top


<!-- 参考信息 -->