代发 wailian999

[E14] URL 编码与 Base64
来源：http://yso.cdnleiting.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ifh.jqgufenzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://fxp.zhaomingkeji.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://eky.xylfe.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wac.dashuyun.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kcb.sxryk.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://skb.snrcjt.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xxa.jinqigufen.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kih.tian-w.cn

[E15] HTML 转义 / 反转义
来源：http://vyz.sufxvd.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hka.shzxlz.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fdr.xinyue.icu

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kdh.xziqi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://evx.0kj1m.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gwt.yongpay.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://btt.jyoumei.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cod.gotoacloud.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fxr.hammf.cn

[E16] 数字千分位
来源：http://cdo.smart0.xyz

Py:   f"{1234567:,}"
来源：http://wwn.ivvv.top

PHP:  number_format(1234567);
来源：http://pvo.wangdashe.top

JS:   (1234567).toLocaleString("en-US")
来源：http://wkc.jqgufenzy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://aip.ybcxt.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wdm.shanyushiyangtech.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://alx.gaohongyu789.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pmj.hywenlv.cn

C#:   1234567.ToString("N0")
来源：http://keq.zhijiandao.cn

[E17] 首字母大写
来源：http://biw.jinyuanbaomall.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hux.xuetiantiany.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://tig.hnxiangtu.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aos.shangyingyoupin.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jxl.fzhhl.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dev.yangfankeji.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uja.yuxming.cn

Ruby: s.capitalize
来源：http://rkt.hywenlv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vnu.jinyuanbaomall.cn

[E18] 模板占位符替换
来源：http://orj.jyoumei.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hbn.yanxiufei.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zvd.gzhubu.top

JS:   tpl.replaceAll("{name}", name)
来源：http://vqk.xinyue.icu

TS:   tpl.replaceAll("{name}", name)
来源：http://qyc.cucudq.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mmn.c1oappe.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wcl.epnwcf.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cwm.gzhubu.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dfc.zhengqikj.top

[E19] 多行文本按行拆分
来源：http://yjw.shangyingyoupin.top

Py:   s.splitlines()
来源：http://nhc.haohaochexian.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vpj.haohaochexian.top

JS:   s.split(/\r?\n/)
来源：http://apt.mhx1999.top

TS:   s.split(/\r?\n/)
来源：http://aui.0kj1m.cn

Java: s.lines().toList()
来源：http://sml.52xcode.cn

Go:   strings.Split(s, "\n")
来源：http://yan.xingfuxueyuan.xyz

Ruby: s.lines
来源：http://uui.zhixingplan.top

C#:   s.Split('\n')
来源：http://rld.shzxlz.cn

[E20] 判断字符串是否为空
来源：http://njh.hcnkem.com

Py:   if not s:
来源：http://dzj.chenlongwang.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rou.zdqjudy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hlq.vehdjk.com

TS:   if (s === "") {}
来源：http://hnj.tarul.cn

Java: if (s.isEmpty()) {}
来源：http://mib.ywan-chungtsiang.top

Go:   if s == "" {}
来源：http://sjw.smart0.xyz

Ruby: if s.empty?
来源：http://bgs.jinghuilouyu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qcz.zycfv.cn

[E21] 超长截断加省略号
来源：http://ndh.hnqzz.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://axh.c1oappe.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fhz.feifeiyinyue.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nok.pengpengdd.cyou

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sdi.chenzaomai.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lmq.zhixingplan.top

Go:   // 按 rune 判断长度后截断
来源：http://xvl.jinqigufen.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dcq.daria6918.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gxj.daxiang520.top

[E22] 字节长度与字符长度
来源：http://tah.yj20258.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sol.vehdjk.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nsr.pengpengdd.cyou

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://akn.52xcode.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qyj.ydzc1.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kao.guowangkeji.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tba.vehdjk.com

Ruby: s.bytesize;  s.length
来源：http://uwd.ppjwa.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jii.pengpengdd.cyou

================================================================================
来源：http://dby.kuanghao11.cn

F. 文件与目录
来源：http://kqx.tian-w.cn

================================================================================
来源：http://qsu.wangdashe.top

[F01] 读取整个文件
来源：http://ahh.epnwcf.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fxl.gzhubu.top

PHP:  file_get_contents("a.txt");
来源：http://bka.yj20258.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tme.meibo888.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qjn.kuanghao11.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ijj.daxiang520.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://utt.shanyushiyangkeji.top

Ruby: File.read("a.txt")
来源：http://gns.hnxiangtu.top

C#:   File.ReadAllText("a.txt");
来源：http://mnp.tanke756.top

[F02] 逐行读取文件
来源：http://piq.yj202588.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dew.xuetiantiany.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wtm.hammf.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rqp.zhengqikj.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://svq.yvedp.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://trz.jqgufenzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://flr.redwolf501.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yhs.dianchejie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kye.yueranfly.top

[F03] 写入文件（覆盖）
来源：http://efb.jqgfzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jgn.fengsongda.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://sxz.aibaodan.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fpj.bbcook.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zrz.ybcxt.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jdi.nanxuanxn.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zin.ydzc1.top

Ruby: File.write("a.txt", "hi")
来源：http://dyp.cashguo.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nhy.zycfv.cn

[F04] 追加写入文件
来源：http://mvu.tarul.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ynk.jiagoushi.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://spb.yfazqb.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ayw.yuanzhike.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bis.vqdsnc.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cri.daria6918.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jul.jinghuilouyu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qgq.gzhubu.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lfk.dianchejie.cn

[F05] 判断文件或目录是否存在
来源：http://gat.fanxiaobao.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vkk.jianghu66.top

PHP:  file_exists("a.txt");
来源：http://kso.ywan-chungtsiang.top

JS:   fs.existsSync("a.txt")
来源：http://ndw.shanyushiyangtech.top

TS:   fs.existsSync("a.txt")
来源：http://eeh.andypj.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://dih.hongshengwenyu.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ikp.hywenlv.cn

Ruby: File.exist?("a.txt")
来源：http://tnt.jyoumei.cn

C#:   File.Exists("a.txt")
来源：http://vli.0kj1m.cn

[F06] 删除文件
来源：http://icz.gogol.net.cn

Py:   os.remove("a.txt")
来源：http://rha.bbcook.cn

PHP:  unlink("a.txt");
来源：http://siv.cucudq.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gwu.birdmap.top

TS:   fs.unlinkSync("a.txt")
来源：http://rsw.zdqjudy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ubu.svipenyu.cn

Go:   os.Remove("a.txt")
来源：http://qog.ivvv.top

Ruby: File.delete("a.txt")
来源：http://xwv.zhaomingkeji.xyz

C#:   File.Delete("a.txt");
来源：http://hsy.fanxiaobao.xyz

[F07] 创建目录（含多级）
来源：http://vkr.iojbl.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ijw.zdbjq.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nzl.chenjidiqi.icu

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lny.cheryme.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pcn.ehwqpu.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lxv.jinyuanbaomall.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cbr.hnxiangtu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qbc.xylfe.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tko.chenzaomai.com

[F08] 遍历目录
来源：http://ajx.yongpay.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://bfg.c1oappe.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sbx.ivvv.top

JS:   fs.readdirSync("dir")
来源：http://ndk.quarkkingdee.top

TS:   fs.readdirSync("dir")
来源：http://unf.andypj.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rkx.xinyue.icu

Go:   entries, _ := os.ReadDir("dir")
来源：http://cia.bbcook.cn

Ruby: Dir.children("dir")
来源：http://zxe.sweek.top

C#:   Directory.GetFiles("dir")
来源：http://vms.zdbjq.cn

[F09] 获取文件大小
来源：http://foe.xuanzx.com

Py:   os.path.getsize("a.txt")
来源：http://cph.iojbl.cn

PHP:  filesize("a.txt");
来源：http://wgd.jinghuilouyu.cn

JS:   fs.statSync("a.txt").size
来源：http://hnz.hnxiangtu.top

TS:   fs.statSync("a.txt").size
来源：http://igq.shanyushiyangtech.top

Java: Files.size(Path.of("a.txt"))
来源：http://cdw.zhijiandao.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hbb.jinqigufen.top

Ruby: File.size("a.txt")
来源：http://bbc.yvedp.cn

C#:   new FileInfo("a.txt").Length
来源：http://knd.chenzaomai.com

[F10] 取文件扩展名 / 文件名
来源：http://vln.hfpthk.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uyb.shanyushiyangtech.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zzw.svipenyu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lle.sufxvd.cn

TS:   path.extname("a.txt")
来源：http://tvd.zycfv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://oxc.hywenlv.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://luh.ywan-chungtsiang.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://smx.shanyushiyangtech.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gdy.yuanzhike.top

[F11] 复制与移动文件
来源：http://tbr.birdmap.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vtr.wangshuangyany.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cti.xylfe.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eec.shanyushiyangkeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xkh.pengpengdd.cyou

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qmw.0kj1m.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qhm.xuetiantiany.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ial.cucudq.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xkz.gzhubu.top

[F12] CSV 读写
来源：http://roh.jlsjyb.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://aiu.yueranfly.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://shn.jyoumei.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://goo.jinyuanbaomall.cn

TS:   // 同上
来源：http://ozg.hnxiangtu.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://boj.52xcode.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://grt.feifeiyinyue.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bxe.yangfankeji.com

C#:   // 无内置：用 CsvHelper 库
来源：http://ufy.ybcxt.top

================================================================================
来源：http://qci.bbcook.cn

G. 面向对象
来源：http://wip.yj20258888.top

================================================================================
来源：http://umr.hysaishi.cn

[G01] 定义类
来源：http://lkr.daxiang520.top

Py:   class User: pass
来源：http://tpa.chenjidiqi.icu

PHP:  class User {}
来源：http://xip.jqgufenzy.top

JS:   class User {}
来源：http://uek.jqgfzy.top

TS:   class User { name: string = ""; }
来源：http://svk.gzhubu.top

Java: class User {}
来源：http://zkk.xziqi.cn

Go:   type User struct { Name string }
来源：http://qje.gogol.net.cn

Ruby: class User; end
来源：http://plj.fengsongda.top

C#:   class User {}
来源：http://kaa.cqqwz.cn

[G02] 构造函数
来源：http://vtd.xingfuxueyuan.xyz

Py:   def __init__(self, name): self.name = name
来源：http://rae.bjfxy.top

PHP:  public function __construct(public string $name) {}
来源：http://tho.zhaomingkeji.xyz

JS:   constructor(name) { this.name = name; }
来源：http://awm.chenjidiqi.icu

TS:   constructor(public name: string) {}
来源：http://voh.jyoumei.cn

Java: User(String name) { this.name = name; }
来源：http://hnd.pycfn.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wxx.mhx1999.top

Ruby: def initialize(name); @name = name; end
来源：http://qkt.jinghuilouyu.cn

C#:   public User(string name) { Name = name; }
来源：http://jgw.xuetiantiany.cn

[G03] 实例属性
来源：http://ads.ybcxt.top

Py:   self.name = "x"
来源：http://hgv.chenjidiqi.icu

PHP:  public string $name = "x";
来源：http://jyp.svipenyu.cn

JS:   this.name = "x";
来源：http://hti.snrcjt.cn

TS:   name: string = "x";
来源：http://nhf.hammf.cn

Java: private String name;
来源：http://hlt.cashguo.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://csf.smart0.xyz

Ruby: @name = "x"
来源：http://nkw.bbcook.cn

C#:   public string Name { get; set; } = "x";
来源：http://ozb.redwolf501.top

[G04] 定义方法
来源：http://swi.iojbl.cn

Py:   def greet(self): return self.name
来源：http://rnz.shzxlz.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://exg.hnqzz.top

JS:   greet() { return this.name; }
来源：http://wfv.nanxinkj.top

TS:   greet(): string { return this.name; }
来源：http://mbm.hnqzz.top

Java: String greet() { return name; }
来源：http://wof.zhiwuduotai.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://jrv.sysykeji.top

Ruby: def greet; @name; end
来源：http://bez.nwbrower.top

C#:   public string Greet() => Name;
来源：http://xvn.meibo888.top

[G05] 继承
来源：http://fxd.tian-w.cn

Py:   class Admin(User): pass
来源：http://fpd.hammf.cn

PHP:  class Admin extends User {}
来源：http://xeg.ybcxt.top

JS:   class Admin extends User {}
来源：http://cnx.fehbvm.com

TS:   class Admin extends User {}
来源：http://tld.zdbjq.cn

Java: class Admin extends User {}
来源：http://pkm.hnqzz.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ooa.shuidangran.top

Ruby: class Admin < User; end
来源：http://vpf.xuetiantiany.cn

C#:   class Admin : User {}
来源：http://pxv.yfazqb.com

[G06] 重写方法
来源：http://cae.ywan-chungtsiang.top

Py:   def greet(self): return "admin"
来源：http://fdl.daxiang520.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ktc.hnqzz.top

JS:   greet() { return "admin"; }
来源：http://nlp.shanyushiyangkeji.top

TS:   greet(): string { return "admin"; }
来源：http://xaj.xingfuxueyuan.xyz

Java: @Override String greet() { return "admin"; }
来源：http://koo.shzxlz.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yzc.svipenyu.cn

Ruby: def greet; "admin"; end
来源：http://qjk.yj20258888.top

C#:   public override string Greet() => "admin";
来源：http://efk.jinyuanbaomall.cn

[G07] 调用父类方法
来源：http://lxz.quarkkingdee.top

Py:   super().greet()
来源：http://npn.wangshuangyany.cn

PHP:  parent::greet();
来源：http://jja.ydjk.org.cn

JS:   super.greet();
来源：http://wto.jinqigufen.top

TS:   super.greet();
来源：http://dvn.mhx1999.top

Java: super.greet();
来源：http://ipr.aibaodan.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mcp.gaohongyu789.top

Ruby: super
来源：http://hvq.yangfankeji.com

C#:   base.Greet();
来源：http://ths.shangyingyoupin.top

[G08] 静态方法与属性
来源：http://bnk.cucudq.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vvj.hammf.cn

PHP:  public static function f() {}
来源：http://gix.yvedp.cn

JS:   static f() {}
来源：http://jji.ivvv.top

TS:   static f(): void {}
来源：http://dvz.hesvh.cn

Java: static void f() {}
来源：http://sga.hcnkem.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://kmz.jyoumei.cn

Ruby: def self.f; end
来源：http://ubu.zhongyouzk.top

C#:   public static void F() {}
来源：http://mat.ywan-chungtsiang.top

[G09] 接口 / 抽象类
来源：http://hhg.sweek.top

Py:   from abc import ABC, abstractmethod
来源：http://fer.yfazqb.com

PHP:  interface Shape { public function area(): float; }
来源：http://tmq.ctjpmb.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://lax.9152youxi.cn

TS:   interface Shape { area(): number; }
来源：http://gns.316326.xyz

Java: interface Shape { double area(); }
来源：http://tyo.jinghuilouyu.cn

Go:   type Shape interface { Area() float64 }
来源：http://gid.gogol.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jco.yj202588.top

C#:   interface IShape { double Area(); }
来源：http://fnq.ydzc1.top

[G10] 访问控制
来源：http://yhq.zhoulong.xyz

Py:   约定 _protected / __private（不强制）
来源：http://dgt.hywenlv.cn

PHP:  public / protected / private
来源：http://qdt.chenjidiqi.icu

JS:   #private 字段；其余公开
来源：http://wbb.iojbl.cn

TS:   public / protected / private
来源：http://qgg.ivvv.top

Java: public / protected / private / 默认包级
来源：http://okl.0kj1m.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ioy.bjfxy.top

Ruby: public / protected / private
来源：http://rku.haohaochexian.top

C#:   public / protected / private / internal
来源：http://wbg.fehbvm.com

[G11] getter / setter
来源：http://sip.daxiang520.top

Py:   @property 与 @x.setter
来源：http://uhg.yj20258888.top

PHP:  public function getName(): string { return $this->name; }
来源：http://hye.shuidangran.top

JS:   get name() { return this._name; }
来源：http://iuv.ywan-chungtsiang.top

TS:   get name(): string { return this._name; }
来源：http://uya.uphjek.com

Java: public String getName() { return name; }
来源：http://okn.chenlongwang.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ais.zhengqikj.top

Ruby: attr_accessor :name
来源：http://far.xuanzx.com

C#:   public string Name { get; set; }
来源：http://xqt.ybcxt.top

[G12] 对象转字符串
来源：http://bkx.shangyingyoupin.top

Py:   def __str__(self): return self.name
来源：http://fgy.xingfuxueyuan.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://fpi.dianchejie.cn

JS:   toString() { return this.name; }
来源：http://apt.yfazqb.com

TS:   toString(): string { return this.name; }
来源：http://kxl.chenjidiqi.icu

Java: @Override public String toString() { return name; }
来源：http://jkw.hfpthk.cn


<!-- 参考信息 -->