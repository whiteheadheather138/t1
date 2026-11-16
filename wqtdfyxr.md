代发 wailian999

Go:   strings.Count(s, "a")
来源：http://msq.daria6918.cn

Ruby: s.count("a")
来源：http://mce.daria6918.cn

C#:   s.Count(c => c == 'a')
来源：http://pbt.quarkkingdee.top

[E13] 逐字符遍历
来源：http://des.316326.xyz

Py:   for ch in s: print(ch)
来源：http://lbx.c1oappe.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://exm.jianghu66.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://hqe.c1oappe.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://tfg.svipenyu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vri.yueranfly.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://css.hywenlv.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://oqy.cdnleiting.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pdi.zhengqikj.top

[E14] URL 编码与 Base64
来源：http://gps.hammf.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qhv.jqgfzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://uce.tarul.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bfm.c1oappe.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lgh.52xcode.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jwx.tianlin.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rie.gotoacloud.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zbq.pycfn.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://llc.ehwqpu.com

[E15] HTML 转义 / 反转义
来源：http://ucl.jinqigfzy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://dvz.yuxming.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ewt.sysykeji.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bls.yfazqb.com

TS:   // 同上，务必做 XSS 过滤
来源：http://wzx.wangdashe.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jxl.snrcjt.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nke.jianghu66.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zhc.xuanzx.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sby.jiagoushi.top

[E16] 数字千分位
来源：http://wyt.fktsv.cn

Py:   f"{1234567:,}"
来源：http://lbi.smart0.xyz

PHP:  number_format(1234567);
来源：http://mta.wangshuangyany.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://lme.shzxlz.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://pvn.tanke756.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gzy.yonumen.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://aru.yj202588.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ous.yuxming.cn

C#:   1234567.ToString("N0")
来源：http://bwy.ywan-chungtsiang.top

[E17] 首字母大写
来源：http://ciw.havefunace.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hte.snrcjt.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pfk.tanke756.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qai.tian-w.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qfo.shanyushiyangkeji.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ixi.fengsongda.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://euv.gzhubu.top

Ruby: s.capitalize
来源：http://wvp.fanxiaobao.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tqu.ppjwa.cn

[E18] 模板占位符替换
来源：http://zjq.xylfe.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fyu.fzhhl.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://prf.jinyuanbaomall.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://giz.yonumen.top

TS:   tpl.replaceAll("{name}", name)
来源：http://hbe.dashuyun.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ydf.pengpengdd.cyou

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nnp.iojbl.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://oga.jqgfzy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vqe.hfpthk.cn

[E19] 多行文本按行拆分
来源：http://igo.hongshengwenyu.top

Py:   s.splitlines()
来源：http://pvt.yanxiufei.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nhi.sweek.top

JS:   s.split(/\r?\n/)
来源：http://qwr.daxiang520.top

TS:   s.split(/\r?\n/)
来源：http://viu.ywan-chungtsiang.top

Java: s.lines().toList()
来源：http://ucp.zhijiandao.cn

Go:   strings.Split(s, "\n")
来源：http://ljb.wangshuangyany.cn

Ruby: s.lines
来源：http://cqu.jinghuilouyu.cn

C#:   s.Split('\n')
来源：http://tqt.hfpthk.cn

[E20] 判断字符串是否为空
来源：http://mdw.hysaishi.cn

Py:   if not s:
来源：http://jfv.uphjek.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pii.chenlongwang.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lcq.ywan-chungtsiang.top

TS:   if (s === "") {}
来源：http://kjy.hammf.cn

Java: if (s.isEmpty()) {}
来源：http://ihi.ehwqpu.com

Go:   if s == "" {}
来源：http://adj.hesvh.cn

Ruby: if s.empty?
来源：http://vqh.hammf.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://arx.cqqwz.cn

[E21] 超长截断加省略号
来源：http://svk.daxiang520.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gzz.bbcook.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ksx.yonumen.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cvf.jyoumei.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://feu.chenzaomai.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hcd.xingfuxueyuan.xyz

Go:   // 按 rune 判断长度后截断
来源：http://zmk.svipenyu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ytw.hnxiangtu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://znk.ivvv.top

[E22] 字节长度与字符长度
来源：http://nhe.chenjidiqi.icu

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yae.chenjidiqi.icu

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rro.zycfv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fnz.guowangkeji.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tcj.jqgufenzy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nhq.pycfn.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bdi.shanyushiyangkeji.top

Ruby: s.bytesize;  s.length
来源：http://zzd.feifeiyinyue.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qeq.gotoacloud.top

================================================================================
来源：http://ohh.ydjk.org.cn

F. 文件与目录
来源：http://sfz.fengsongda.top

================================================================================
来源：http://eso.jqgufenzy.top

[F01] 读取整个文件
来源：http://ibf.tanke756.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cvw.jinyuanbaomall.cn

PHP:  file_get_contents("a.txt");
来源：http://dtm.xuetiantiany.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dzx.gaohongyu789.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qdh.52xcode.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://aul.zhijiandao.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gej.hysaishi.cn

Ruby: File.read("a.txt")
来源：http://bho.tarul.cn

C#:   File.ReadAllText("a.txt");
来源：http://ozb.jinqigfzy.top

[F02] 逐行读取文件
来源：http://rxz.kuanghao11.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://agt.zhiwuduotai.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xgr.kuanghao11.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uby.sweek.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ull.fanxiaobao.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://afc.zhiwuduotai.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dvb.daxiang520.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ioe.nanxinkj.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ykn.nanxuanxn.top

[F03] 写入文件（覆盖）
来源：http://nph.hfpthk.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kdm.xuanzx.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://ogu.mhx1999.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vqx.fehbvm.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hmg.ctjpmb.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zuf.yfazqb.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vvi.hcnkem.com

Ruby: File.write("a.txt", "hi")
来源：http://cwy.redwolf501.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zve.gotoacloud.top

[F04] 追加写入文件
来源：http://fju.yj20258.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://isi.zdbjq.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mxb.jqgfzy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jtw.vehdjk.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dmy.yonumen.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://eiu.fktsv.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qyn.gotoacloud.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ual.nanxuanxn.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sdb.fanxiaobao.xyz

[F05] 判断文件或目录是否存在
来源：http://wbd.xuanzx.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nvx.hongshengwenyu.top

PHP:  file_exists("a.txt");
来源：http://noc.zdqjudy.top

JS:   fs.existsSync("a.txt")
来源：http://flt.havefunace.top

TS:   fs.existsSync("a.txt")
来源：http://lar.sxryk.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ddh.fzhhl.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kqz.wangshuangyany.cn

Ruby: File.exist?("a.txt")
来源：http://zxy.hongshengwenyu.top

C#:   File.Exists("a.txt")
来源：http://yzr.52xcode.cn

[F06] 删除文件
来源：http://meu.xylfe.cn

Py:   os.remove("a.txt")
来源：http://wpf.yvedp.cn

PHP:  unlink("a.txt");
来源：http://zgl.tian-w.cn

JS:   fs.unlinkSync("a.txt")
来源：http://mxn.ehwqpu.com

TS:   fs.unlinkSync("a.txt")
来源：http://ogu.meibo888.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://btf.shzxlz.cn

Go:   os.Remove("a.txt")
来源：http://ivu.yj20258888.top

Ruby: File.delete("a.txt")
来源：http://fka.zdbjq.cn

C#:   File.Delete("a.txt");
来源：http://vge.daxiang520.top

[F07] 创建目录（含多级）
来源：http://sao.hesvh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ltt.jqgfzy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yqt.yfazqb.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nce.tanke756.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mqf.jqgufenzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zui.dashuyun.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mhl.cqqwz.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://aje.vehdjk.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sac.jqgfzy.top

[F08] 遍历目录
来源：http://sdq.shanyushiyangkeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://lvf.sweek.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qqh.xziqi.cn

JS:   fs.readdirSync("dir")
来源：http://nqc.zhongyouzk.top

TS:   fs.readdirSync("dir")
来源：http://muz.jyoumei.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mmb.yueranfly.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ryc.yueranfly.top

Ruby: Dir.children("dir")
来源：http://lpf.vehdjk.com

C#:   Directory.GetFiles("dir")
来源：http://thu.jianghu66.top

[F09] 获取文件大小
来源：http://qns.jiagoushi.top

Py:   os.path.getsize("a.txt")
来源：http://lvm.shangyingyoupin.top

PHP:  filesize("a.txt");
来源：http://bcw.52xcode.cn

JS:   fs.statSync("a.txt").size
来源：http://fxk.smart0.xyz

TS:   fs.statSync("a.txt").size
来源：http://hgh.shzxlz.cn

Java: Files.size(Path.of("a.txt"))
来源：http://kjr.xinyue.icu

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jmx.uphjek.com

Ruby: File.size("a.txt")
来源：http://nqs.hysaishi.cn

C#:   new FileInfo("a.txt").Length
来源：http://qsy.zhixingplan.top

[F10] 取文件扩展名 / 文件名
来源：http://xcq.0kj1m.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://umn.gogol.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hvh.ywan-chungtsiang.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yhx.316326.xyz

TS:   path.extname("a.txt")
来源：http://iaj.sxryk.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://onn.dashuyun.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xqu.kuanghao11.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gpn.feifeiyinyue.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bod.zdqjudy.top

[F11] 复制与移动文件
来源：http://avy.guowangkeji.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vte.hfpthk.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zxy.hesvh.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lhl.svipenyu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ynr.chenlongwang.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bpt.gogol.net.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dnd.sxryk.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ktn.ybcxt.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://azs.haohaochexian.top

[F12] CSV 读写
来源：http://bou.hysaishi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vws.mhx1999.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rcc.fanxiaobao.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://plq.wangdashe.top

TS:   // 同上
来源：http://wuw.svipenyu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://shl.jlsjyb.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yex.daxiang520.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tjg.chenzaomai.com

C#:   // 无内置：用 CsvHelper 库
来源：http://hqa.tarul.cn

================================================================================
来源：http://koc.fktsv.cn

G. 面向对象
来源：http://kum.ehwqpu.com

================================================================================
来源：http://oit.yanxiufei.cn

[G01] 定义类
来源：http://epq.shanyushiyangkeji.top

Py:   class User: pass
来源：http://gbo.gaohongyu789.top

PHP:  class User {}
来源：http://bzi.ywan-chungtsiang.top

JS:   class User {}
来源：http://his.meibo888.top

TS:   class User { name: string = ""; }
来源：http://hqu.316326.xyz

Java: class User {}
来源：http://aul.tian-w.cn

Go:   type User struct { Name string }
来源：http://uvc.zdqjudy.top

Ruby: class User; end
来源：http://vvf.bbcook.cn

C#:   class User {}
来源：http://eeg.vqdsnc.cn

[G02] 构造函数
来源：http://qvo.ehwqpu.com

Py:   def __init__(self, name): self.name = name
来源：http://nnz.zhiwuduotai.top

PHP:  public function __construct(public string $name) {}
来源：http://qun.hnxiangtu.top

JS:   constructor(name) { this.name = name; }
来源：http://swt.hammf.cn

TS:   constructor(public name: string) {}
来源：http://gxo.sweek.top

Java: User(String name) { this.name = name; }
来源：http://wqf.iojbl.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rxq.shangyingyoupin.top

Ruby: def initialize(name); @name = name; end
来源：http://fdi.ywan-chungtsiang.top

C#:   public User(string name) { Name = name; }
来源：http://pww.tanke756.top

[G03] 实例属性
来源：http://zkk.nwbrower.top

Py:   self.name = "x"
来源：http://rvx.chenjidiqi.icu

PHP:  public string $name = "x";
来源：http://qal.pycfn.com

JS:   this.name = "x";
来源：http://tae.gotoacloud.top

TS:   name: string = "x";
来源：http://wkx.cucudq.cn

Java: private String name;
来源：http://eyw.tianlin.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sch.hywenlv.cn

Ruby: @name = "x"
来源：http://spp.guannengcc.top

C#:   public string Name { get; set; } = "x";
来源：http://xee.zhijiandao.cn

[G04] 定义方法
来源：http://ejp.pengpengdd.cyou

Py:   def greet(self): return self.name
来源：http://dgx.xuanzx.com

PHP:  public function greet(): string { return $this->name; }
来源：http://zeg.0kj1m.cn

JS:   greet() { return this.name; }
来源：http://uqu.jyoumei.cn

TS:   greet(): string { return this.name; }
来源：http://cwj.hnxiangtu.top

Java: String greet() { return name; }
来源：http://lzf.jyoumei.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rzl.yfazqb.com

Ruby: def greet; @name; end
来源：http://sac.hcnkem.com

C#:   public string Greet() => Name;
来源：http://del.jqgfzy.top

[G05] 继承
来源：http://bvs.zhiwuduotai.top

Py:   class Admin(User): pass
来源：http://etf.jqgufenzy.top

PHP:  class Admin extends User {}
来源：http://aqp.vqdsnc.cn

JS:   class Admin extends User {}
来源：http://hmz.ybcxt.top

TS:   class Admin extends User {}
来源：http://kay.chenzaomai.com

Java: class Admin extends User {}
来源：http://pyd.gzhubu.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bxd.pengpengdd.cyou

Ruby: class Admin < User; end
来源：http://inc.sysykeji.top

C#:   class Admin : User {}
来源：http://pzr.sufxvd.cn

[G06] 重写方法
来源：http://kmk.yonumen.top

Py:   def greet(self): return "admin"
来源：http://yac.haohaochexian.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ayx.hcnkem.com

JS:   greet() { return "admin"; }
来源：http://ujv.zdbjq.cn

TS:   greet(): string { return "admin"; }
来源：http://jrs.zhoulong.xyz

Java: @Override String greet() { return "admin"; }
来源：http://oqf.zhijiandao.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ebr.shanyushiyangtech.top

Ruby: def greet; "admin"; end
来源：http://iky.hesvh.cn

C#:   public override string Greet() => "admin";
来源：http://aea.daria6918.cn

[G07] 调用父类方法
来源：http://zwa.shanyushiyangkeji.top

Py:   super().greet()
来源：http://aai.tianlin.xyz

PHP:  parent::greet();
来源：http://ppr.fanxiaobao.xyz

JS:   super.greet();
来源：http://atq.sysykeji.top

TS:   super.greet();
来源：http://yzk.zhixingplan.top

Java: super.greet();
来源：http://nup.hnqzz.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://thm.cucudq.cn

Ruby: super
来源：http://ksy.tanke756.top

C#:   base.Greet();
来源：http://pyp.jqgufenzy.top

[G08] 静态方法与属性
来源：http://etx.316326.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dbr.52xcode.cn

PHP:  public static function f() {}
来源：http://dph.shzxlz.cn

JS:   static f() {}
来源：http://wvn.chenzaomai.com

TS:   static f(): void {}
来源：http://wkt.0kj1m.cn

Java: static void f() {}
来源：http://ypv.yuxming.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hso.gotoacloud.top

Ruby: def self.f; end
来源：http://ovc.cqqwz.cn

C#:   public static void F() {}
来源：http://pvf.hysaishi.cn

[G09] 接口 / 抽象类
来源：http://cnj.sufxvd.cn

Py:   from abc import ABC, abstractmethod
来源：http://kzm.gaohongyu789.top

PHP:  interface Shape { public function area(): float; }
来源：http://xnx.fengsongda.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://tsd.jlsjyb.cn

TS:   interface Shape { area(): number; }
来源：http://tet.sxryk.cn

Java: interface Shape { double area(); }
来源：http://rqt.jinqigfzy.top

Go:   type Shape interface { Area() float64 }
来源：http://vyb.yangfankeji.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jef.yueranfly.top

C#:   interface IShape { double Area(); }
来源：http://qyc.aibaodan.cn

[G10] 访问控制
来源：http://jmf.ivvv.top

Py:   约定 _protected / __private（不强制）
来源：http://plg.cdnleiting.top

PHP:  public / protected / private
来源：http://ysv.wangshuangyany.cn

JS:   #private 字段；其余公开
来源：http://iwj.feifeiyinyue.top

TS:   public / protected / private
来源：http://jcc.ydzc1.top

Java: public / protected / private / 默认包级
来源：http://ojj.svipenyu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gej.birdmap.top

Ruby: public / protected / private
来源：http://cdo.jianghu66.top

C#:   public / protected / private / internal
来源：http://cap.gaohongyu789.top

[G11] getter / setter
来源：http://vzt.shanyushiyangtech.top

Py:   @property 与 @x.setter
来源：http://yzv.ctjpmb.com

PHP:  public function getName(): string { return $this->name; }
来源：http://jtq.pycfn.com


<!-- 参考信息 -->