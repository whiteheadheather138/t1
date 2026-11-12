代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wgq.316326.xyz

[E11] 反转字符串
来源：http://pvy.zhaomingkeji.xyz

Py:   s[::-1]
来源：http://yhu.bjfxy.top

PHP:  strrev($s);
来源：http://csi.pengpengdd.cyou

JS:   [...s].reverse().join("")
来源：http://byl.guannengcc.top

TS:   [...s].reverse().join("")
来源：http://jmq.sufxvd.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://usf.jiagoushi.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://fwl.yj20258.top

Ruby: s.reverse
来源：http://hzb.vqdsnc.cn

C#:   new string(s.Reverse().ToArray())
来源：http://jcp.uphjek.com

[E12] 统计某字符出现次数
来源：http://fkv.hfpthk.cn

Py:   s.count("a")
来源：http://ynl.zhijiandao.cn

PHP:  substr_count($s, "a");
来源：http://nqv.bjfxy.top

JS:   s.split("a").length - 1
来源：http://bth.yvedp.cn

TS:   s.split("a").length - 1
来源：http://hqc.zhixingplan.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nsl.ydjk.org.cn

Go:   strings.Count(s, "a")
来源：http://bqb.aizwys.cn

Ruby: s.count("a")
来源：http://meu.zhixingplan.top

C#:   s.Count(c => c == 'a')
来源：http://qqq.52xcode.cn

[E13] 逐字符遍历
来源：http://iaz.xuanzx.com

Py:   for ch in s: print(ch)
来源：http://shm.chenlongwang.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nhp.c1oappe.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://tvg.c1oappe.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ikh.tanke756.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vwi.nwbrower.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mhc.zhijiandao.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://zzr.c1oappe.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nnr.jinqigfzy.top

[E14] URL 编码与 Base64
来源：http://vut.yfazqb.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wkd.svipenyu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tmd.wangshuangyany.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ybf.zhixingplan.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ciu.yonumen.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tnp.epnwcf.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hbd.ehwqpu.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://izr.zdbjq.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rks.shangyingyoupin.top

[E15] HTML 转义 / 反转义
来源：http://dwz.jianghu66.top

Py:   html.escape(s);  html.unescape(s)
来源：http://bwk.pengpengdd.cyou

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jrc.zhiwuduotai.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tid.dianchejie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xyi.hfpthk.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ydi.xziqi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ejt.xuetiantiany.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://obz.sjlbkw.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dho.ppjwa.cn

[E16] 数字千分位
来源：http://lmk.quarkkingdee.top

Py:   f"{1234567:,}"
来源：http://pal.hesvh.cn

PHP:  number_format(1234567);
来源：http://vma.xylfe.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ine.shuidangran.top

TS:   (1234567).toLocaleString("en-US")
来源：http://jtc.yanxiufei.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rbv.fzhhl.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sgt.jianghu66.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yke.vqdsnc.cn

C#:   1234567.ToString("N0")
来源：http://thr.zhiwuduotai.top

[E17] 首字母大写
来源：http://ryu.nanxuanxn.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://byw.nwbrower.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://izj.fehbvm.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oud.yanxiufei.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qys.tianlin.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://upj.zhengqikj.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://eny.tanke756.top

Ruby: s.capitalize
来源：http://xqx.ehwqpu.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pyg.zhaomingkeji.xyz

[E18] 模板占位符替换
来源：http://qks.zhixingplan.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cye.bjfxy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hsl.daxiang520.top

JS:   tpl.replaceAll("{name}", name)
来源：http://unb.shanyushiyangtech.top

TS:   tpl.replaceAll("{name}", name)
来源：http://irs.hammf.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rlq.0kj1m.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qpo.tarul.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zqj.hysaishi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://idp.zdbjq.cn

[E19] 多行文本按行拆分
来源：http://qwp.meibo888.top

Py:   s.splitlines()
来源：http://ago.epnwcf.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nqn.guannengcc.top

JS:   s.split(/\r?\n/)
来源：http://twi.zhixingplan.top

TS:   s.split(/\r?\n/)
来源：http://mcb.ydzc1.top

Java: s.lines().toList()
来源：http://xrp.quarkkingdee.top

Go:   strings.Split(s, "\n")
来源：http://eqk.aizwys.cn

Ruby: s.lines
来源：http://sns.wangshuangyany.cn

C#:   s.Split('\n')
来源：http://ssu.shanyushiyangkeji.top

[E20] 判断字符串是否为空
来源：http://gmr.hongshengwenyu.top

Py:   if not s:
来源：http://zhc.ppjwa.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://aln.fehbvm.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hqq.yj20258888.top

TS:   if (s === "") {}
来源：http://eue.tianlin.xyz

Java: if (s.isEmpty()) {}
来源：http://iuo.birdmap.top

Go:   if s == "" {}
来源：http://xly.hongshengwenyu.top

Ruby: if s.empty?
来源：http://scm.shanyushiyangkeji.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tgv.mhx1999.top

[E21] 超长截断加省略号
来源：http://uti.sweek.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://znz.chenjidiqi.icu

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xvv.zhengqikj.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rgj.zdqjudy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bmf.ybcxt.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yir.nanxuanxn.top

Go:   // 按 rune 判断长度后截断
来源：http://tdp.sxryk.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dmq.52xcode.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://izj.andypj.xyz

[E22] 字节长度与字符长度
来源：http://uny.quarkkingdee.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ypv.tanke756.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vko.zhixingplan.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tkd.smart0.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ifb.vqdsnc.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sul.smart0.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ajc.pycfn.com

Ruby: s.bytesize;  s.length
来源：http://cdl.yongpay.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dlc.vehdjk.com

================================================================================
来源：http://nlb.daria6918.cn

F. 文件与目录
来源：http://wbh.ydjk.org.cn

================================================================================
来源：http://rcf.ybcxt.top

[F01] 读取整个文件
来源：http://ans.sjlbkw.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cgk.jinghuilouyu.cn

PHP:  file_get_contents("a.txt");
来源：http://mmd.fktsv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ogc.sysykeji.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pkn.sjlbkw.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://bqz.yonumen.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tgc.havefunace.top

Ruby: File.read("a.txt")
来源：http://kis.yanxiufei.cn

C#:   File.ReadAllText("a.txt");
来源：http://pnu.wangshuangyany.cn

[F02] 逐行读取文件
来源：http://mmg.dashuyun.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://czt.shangyingyoupin.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zyi.cashguo.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qpw.yvedp.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vyr.9152youxi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kmx.fengsongda.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yzx.xziqi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mlk.zhengqikj.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ksf.zhengqikj.top

[F03] 写入文件（覆盖）
来源：http://fql.yuxming.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cmb.fzhhl.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://rad.aizwys.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qci.chenlongwang.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xea.svipenyu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ull.ppjwa.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mve.hysaishi.cn

Ruby: File.write("a.txt", "hi")
来源：http://iyc.shzxlz.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kjf.jinqigfzy.top

[F04] 追加写入文件
来源：http://bii.shzxlz.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tlc.zycfv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://guc.tian-w.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://acf.gotoacloud.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ivj.zhaomingkeji.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ijn.jqgfzy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tbt.9152youxi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ekd.aizwys.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sod.gogol.net.cn

[F05] 判断文件或目录是否存在
来源：http://phc.daria6918.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://guc.svipenyu.cn

PHP:  file_exists("a.txt");
来源：http://luq.9152youxi.cn

JS:   fs.existsSync("a.txt")
来源：http://oyz.tarul.cn

TS:   fs.existsSync("a.txt")
来源：http://uxi.c1oappe.top

Java: Files.exists(Path.of("a.txt"))
来源：http://bls.yuxming.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qga.cheryme.top

Ruby: File.exist?("a.txt")
来源：http://ywe.iojbl.cn

C#:   File.Exists("a.txt")
来源：http://awf.nwbrower.top

[F06] 删除文件
来源：http://idz.ybcxt.top

Py:   os.remove("a.txt")
来源：http://nqu.yvedp.cn

PHP:  unlink("a.txt");
来源：http://apf.feifeiyinyue.top

JS:   fs.unlinkSync("a.txt")
来源：http://amw.pengpengdd.cyou

TS:   fs.unlinkSync("a.txt")
来源：http://eyh.nwbrower.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://clj.hongshengwenyu.top

Go:   os.Remove("a.txt")
来源：http://uwz.uphjek.com

Ruby: File.delete("a.txt")
来源：http://xny.sxryk.cn

C#:   File.Delete("a.txt");
来源：http://gnq.kuanghao11.cn

[F07] 创建目录（含多级）
来源：http://pxj.gzhubu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://czq.xuanzx.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mif.jinqigfzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bqy.pengpengdd.cyou

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dtt.chenjidiqi.icu

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dye.ppjwa.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mrw.pycfn.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xld.hcnkem.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bpy.xziqi.cn

[F08] 遍历目录
来源：http://gtw.svipenyu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ouv.shzxlz.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ucr.tarul.cn

JS:   fs.readdirSync("dir")
来源：http://niq.hywenlv.cn

TS:   fs.readdirSync("dir")
来源：http://bju.shangyingyoupin.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vzd.yuanzhike.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://zax.jinghuilouyu.cn

Ruby: Dir.children("dir")
来源：http://fbn.jianghu66.top

C#:   Directory.GetFiles("dir")
来源：http://ylj.yonumen.top

[F09] 获取文件大小
来源：http://uyo.gzhubu.top

Py:   os.path.getsize("a.txt")
来源：http://ztd.zycfv.cn

PHP:  filesize("a.txt");
来源：http://xrh.guannengcc.top

JS:   fs.statSync("a.txt").size
来源：http://kpj.yuxming.cn

TS:   fs.statSync("a.txt").size
来源：http://pij.wangshuangyany.cn

Java: Files.size(Path.of("a.txt"))
来源：http://uym.gotoacloud.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ewc.jqgufenzy.top

Ruby: File.size("a.txt")
来源：http://vau.snrcjt.cn

C#:   new FileInfo("a.txt").Length
来源：http://euq.yj20258.top

[F10] 取文件扩展名 / 文件名
来源：http://opf.guowangkeji.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://obw.hywenlv.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uve.ivvv.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hdo.yj20258.top

TS:   path.extname("a.txt")
来源：http://ddy.shangyingyoupin.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ccb.fktsv.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tsz.bbcook.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://oaw.hesvh.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bvt.fanxiaobao.xyz

[F11] 复制与移动文件
来源：http://ivl.uphjek.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ywt.smart0.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://eol.xinyue.icu

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://igf.sxryk.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yqy.zhiwuduotai.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yja.0kj1m.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://djg.sjlbkw.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bjo.mhx1999.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://usm.jlsjyb.cn

[F12] CSV 读写
来源：http://mey.epnwcf.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lyy.chenlongwang.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rsk.316326.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lyr.ppjwa.cn

TS:   // 同上
来源：http://fez.zhongyouzk.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ajr.pycfn.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fft.yangfankeji.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mfe.smart0.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://kof.fktsv.cn

================================================================================
来源：http://vkk.aizwys.cn

G. 面向对象
来源：http://wvv.yj202588.top

================================================================================
来源：http://hud.yuxming.cn

[G01] 定义类
来源：http://mgr.jlsjyb.cn

Py:   class User: pass
来源：http://uah.guannengcc.top

PHP:  class User {}
来源：http://ecc.yj202588.top

JS:   class User {}
来源：http://smy.jianghu66.top

TS:   class User { name: string = ""; }
来源：http://drx.0kj1m.cn

Java: class User {}
来源：http://wmh.yvedp.cn

Go:   type User struct { Name string }
来源：http://dwx.jqgfzy.top

Ruby: class User; end
来源：http://byv.yj20258.top

C#:   class User {}
来源：http://qib.fanxiaobao.xyz

[G02] 构造函数
来源：http://cdb.xinyue.icu

Py:   def __init__(self, name): self.name = name
来源：http://ciz.zhixingplan.top

PHP:  public function __construct(public string $name) {}
来源：http://gnv.yanxiufei.cn

JS:   constructor(name) { this.name = name; }
来源：http://qvi.hfpthk.cn

TS:   constructor(public name: string) {}
来源：http://dcu.gzhubu.top

Java: User(String name) { this.name = name; }
来源：http://axp.epnwcf.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wbh.iojbl.cn

Ruby: def initialize(name); @name = name; end
来源：http://atd.xuanzx.com

C#:   public User(string name) { Name = name; }
来源：http://eog.zhixingplan.top

[G03] 实例属性
来源：http://eqf.gogol.net.cn

Py:   self.name = "x"
来源：http://hki.hnxiangtu.top

PHP:  public string $name = "x";
来源：http://xsu.bjfxy.top

JS:   this.name = "x";
来源：http://fks.ppjwa.cn

TS:   name: string = "x";
来源：http://lng.hnqzz.top

Java: private String name;
来源：http://ywl.tian-w.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dyr.aibaodan.cn

Ruby: @name = "x"
来源：http://wrl.hcnkem.com

C#:   public string Name { get; set; } = "x";
来源：http://njw.xuanzx.com

[G04] 定义方法
来源：http://etz.yueranfly.top

Py:   def greet(self): return self.name
来源：http://qlv.sxryk.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://sda.hfpthk.cn

JS:   greet() { return this.name; }
来源：http://dyg.xylfe.cn

TS:   greet(): string { return this.name; }
来源：http://gbh.ivvv.top

Java: String greet() { return name; }
来源：http://tnc.aibaodan.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://too.sjlbkw.cn

Ruby: def greet; @name; end
来源：http://jfq.guannengcc.top

C#:   public string Greet() => Name;
来源：http://xdm.andypj.xyz

[G05] 继承
来源：http://sta.dianchejie.cn

Py:   class Admin(User): pass
来源：http://gae.c1oappe.top

PHP:  class Admin extends User {}
来源：http://gao.zdbjq.cn

JS:   class Admin extends User {}
来源：http://tuj.xziqi.cn

TS:   class Admin extends User {}
来源：http://yjh.zhongyouzk.top

Java: class Admin extends User {}
来源：http://jwu.yuxming.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qvi.feifeiyinyue.top

Ruby: class Admin < User; end
来源：http://xcp.kuanghao11.cn

C#:   class Admin : User {}
来源：http://rzz.chenjidiqi.icu

[G06] 重写方法
来源：http://nve.svipenyu.cn

Py:   def greet(self): return "admin"
来源：http://ccv.wangshuangyany.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mnw.ivvv.top

JS:   greet() { return "admin"; }
来源：http://ltl.jinqigfzy.top

TS:   greet(): string { return "admin"; }
来源：http://nhg.sjlbkw.cn

Java: @Override String greet() { return "admin"; }
来源：http://ceb.xziqi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kvq.jinqigufen.top

Ruby: def greet; "admin"; end
来源：http://ksb.redwolf501.top

C#:   public override string Greet() => "admin";
来源：http://jzi.jianghu66.top

[G07] 调用父类方法
来源：http://xli.tarul.cn

Py:   super().greet()
来源：http://zck.jiagoushi.top

PHP:  parent::greet();
来源：http://lww.9152youxi.cn

JS:   super.greet();
来源：http://zqy.iojbl.cn

TS:   super.greet();
来源：http://hgi.hcnkem.com

Java: super.greet();
来源：http://ixq.jianghu66.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cek.xylfe.cn

Ruby: super
来源：http://ewh.haohaochexian.top

C#:   base.Greet();
来源：http://mye.xuanzx.com

[G08] 静态方法与属性
来源：http://pva.cqqwz.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://muj.zhijiandao.cn

PHP:  public static function f() {}
来源：http://olu.pengpengdd.cyou

JS:   static f() {}
来源：http://xae.nanxuanxn.top

TS:   static f(): void {}
来源：http://vmw.ywan-chungtsiang.top

Java: static void f() {}
来源：http://ero.52xcode.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://odo.yonumen.top

Ruby: def self.f; end
来源：http://plr.fktsv.cn

C#:   public static void F() {}
来源：http://czs.hammf.cn

[G09] 接口 / 抽象类
来源：http://mbz.zhongyouzk.top

Py:   from abc import ABC, abstractmethod
来源：http://zze.zhengqikj.top

PHP:  interface Shape { public function area(): float; }
来源：http://ymb.svipenyu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://uaf.wangshuangyany.cn

TS:   interface Shape { area(): number; }
来源：http://ypq.jiagoushi.top


<!-- 参考信息 -->