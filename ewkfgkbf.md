代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lau.yuxming.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://aer.haohaochexian.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fru.sxryk.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mul.nwbrower.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nst.ywan-chungtsiang.top

[E15] HTML 转义 / 反转义
来源：http://bwm.yanxiufei.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://uxw.tarul.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hqw.yangfankeji.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qep.fanxiaobao.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://uut.9152youxi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vfg.jyoumei.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qwt.cdnleiting.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qar.yuanzhike.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://iiw.ydzc1.top

[E16] 数字千分位
来源：http://jez.hywenlv.cn

Py:   f"{1234567:,}"
来源：http://qru.meibo888.top

PHP:  number_format(1234567);
来源：http://mly.hywenlv.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://uhk.yangfankeji.com

TS:   (1234567).toLocaleString("en-US")
来源：http://dcd.redwolf501.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tze.gotoacloud.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hzu.meibo888.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nyj.hywenlv.cn

C#:   1234567.ToString("N0")
来源：http://ubl.jianghu66.top

[E17] 首字母大写
来源：http://kdd.dashuyun.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ims.ywan-chungtsiang.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ujo.meibo888.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cyj.jinqigfzy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://met.mhx1999.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nvs.vehdjk.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vpq.xziqi.cn

Ruby: s.capitalize
来源：http://xqq.c1oappe.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lkj.cucudq.cn

[E18] 模板占位符替换
来源：http://avx.wangdashe.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uho.svipenyu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wbn.haohaochexian.top

JS:   tpl.replaceAll("{name}", name)
来源：http://cxc.9152youxi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://cgh.yj20258.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fqd.gzhubu.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://iys.jqgufenzy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://enn.zhengqikj.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gdp.jianghu66.top

[E19] 多行文本按行拆分
来源：http://rwc.xuanzx.com

Py:   s.splitlines()
来源：http://gtf.fzhhl.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jwc.yvedp.cn

JS:   s.split(/\r?\n/)
来源：http://wxw.xylfe.cn

TS:   s.split(/\r?\n/)
来源：http://lem.chenzaomai.com

Java: s.lines().toList()
来源：http://alb.gogol.net.cn

Go:   strings.Split(s, "\n")
来源：http://znj.hnxiangtu.top

Ruby: s.lines
来源：http://nkn.jqgfzy.top

C#:   s.Split('\n')
来源：http://ztn.jinqigfzy.top

[E20] 判断字符串是否为空
来源：http://tqr.hnqzz.top

Py:   if not s:
来源：http://ygc.gogol.net.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zqe.yj202588.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://igj.fzhhl.top

TS:   if (s === "") {}
来源：http://zao.kuanghao11.cn

Java: if (s.isEmpty()) {}
来源：http://mfi.vehdjk.com

Go:   if s == "" {}
来源：http://mzt.iojbl.cn

Ruby: if s.empty?
来源：http://zbr.yj20258888.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://unj.ppjwa.cn

[E21] 超长截断加省略号
来源：http://tgj.xuanzx.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bjk.yanxiufei.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://aqa.feifeiyinyue.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vft.cashguo.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hnl.feifeiyinyue.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wqz.xuetiantiany.cn

Go:   // 按 rune 判断长度后截断
来源：http://ejv.svipenyu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jmr.smart0.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qhe.shangyingyoupin.top

[E22] 字节长度与字符长度
来源：http://tow.hammf.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jlv.dashuyun.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vrs.dashuyun.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dnm.ppjwa.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://iaa.chenlongwang.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pkq.zhiwuduotai.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sop.jyoumei.cn

Ruby: s.bytesize;  s.length
来源：http://nvc.yangfankeji.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mwb.hongshengwenyu.top

================================================================================
来源：http://dyd.nanxuanxn.top

F. 文件与目录
来源：http://wli.jlsjyb.cn

================================================================================
来源：http://ijd.cheryme.top

[F01] 读取整个文件
来源：http://toz.jiagoushi.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://aln.guannengcc.top

PHP:  file_get_contents("a.txt");
来源：http://bta.sjlbkw.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://foo.aibaodan.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ums.yuxming.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ier.yj20258.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kuc.nanxinkj.top

Ruby: File.read("a.txt")
来源：http://rnf.sysykeji.top

C#:   File.ReadAllText("a.txt");
来源：http://lrx.aizwys.cn

[F02] 逐行读取文件
来源：http://ref.zhongyouzk.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xgc.feifeiyinyue.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fom.pengpengdd.cyou

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://txc.yongpay.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qob.zhaomingkeji.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cgy.sufxvd.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lbj.fanxiaobao.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qxj.wangshuangyany.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wei.hnxiangtu.top

[F03] 写入文件（覆盖）
来源：http://lys.yonumen.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dqo.hammf.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ngw.meibo888.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uep.nwbrower.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pbn.nwbrower.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fzq.jqgfzy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wgy.jinqigfzy.top

Ruby: File.write("a.txt", "hi")
来源：http://fae.yj20258888.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xdr.ehwqpu.com

[F04] 追加写入文件
来源：http://iyo.yuxming.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mwr.pengpengdd.cyou

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bqs.quarkkingdee.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xwk.vehdjk.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xhc.mhx1999.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vsd.fktsv.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rmv.xinyue.icu

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pxx.jinyuanbaomall.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kxc.zhijiandao.cn

[F05] 判断文件或目录是否存在
来源：http://sqz.ctjpmb.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gyj.zhoulong.xyz

PHP:  file_exists("a.txt");
来源：http://nie.yj202588.top

JS:   fs.existsSync("a.txt")
来源：http://jxm.zhaomingkeji.xyz

TS:   fs.existsSync("a.txt")
来源：http://ubi.zdqjudy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ltm.zycfv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bil.ehwqpu.com

Ruby: File.exist?("a.txt")
来源：http://sno.yfazqb.com

C#:   File.Exists("a.txt")
来源：http://nxh.pycfn.com

[F06] 删除文件
来源：http://buj.shangyingyoupin.top

Py:   os.remove("a.txt")
来源：http://ida.aibaodan.cn

PHP:  unlink("a.txt");
来源：http://rhn.0kj1m.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gdg.hongshengwenyu.top

TS:   fs.unlinkSync("a.txt")
来源：http://jku.kuanghao11.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lbz.nwbrower.top

Go:   os.Remove("a.txt")
来源：http://wxn.cashguo.top

Ruby: File.delete("a.txt")
来源：http://dva.aizwys.cn

C#:   File.Delete("a.txt");
来源：http://uzu.jqgufenzy.top

[F07] 创建目录（含多级）
来源：http://cez.hongshengwenyu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xrg.hammf.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mth.yj20258.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bbj.jinqigfzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://shq.hysaishi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jdy.ywan-chungtsiang.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cru.hnxiangtu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://eli.gogol.net.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://flt.zhijiandao.cn

[F08] 遍历目录
来源：http://lux.52xcode.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://gdj.zhijiandao.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pbd.ivvv.top

JS:   fs.readdirSync("dir")
来源：http://nzd.cheryme.top

TS:   fs.readdirSync("dir")
来源：http://mwj.hcnkem.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ieh.xuetiantiany.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vlw.shangyingyoupin.top

Ruby: Dir.children("dir")
来源：http://dib.vqdsnc.cn

C#:   Directory.GetFiles("dir")
来源：http://vfs.ppjwa.cn

[F09] 获取文件大小
来源：http://pxf.hnxiangtu.top

Py:   os.path.getsize("a.txt")
来源：http://vtu.fzhhl.top

PHP:  filesize("a.txt");
来源：http://ipv.shzxlz.cn

JS:   fs.statSync("a.txt").size
来源：http://ysr.cdnleiting.top

TS:   fs.statSync("a.txt").size
来源：http://dfb.fehbvm.com

Java: Files.size(Path.of("a.txt"))
来源：http://ang.jinqigfzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qsm.fengsongda.top

Ruby: File.size("a.txt")
来源：http://qdg.gaohongyu789.top

C#:   new FileInfo("a.txt").Length
来源：http://tub.nanxinkj.top

[F10] 取文件扩展名 / 文件名
来源：http://zdv.jyoumei.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jtf.zdbjq.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://myn.zdbjq.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zau.hysaishi.cn

TS:   path.extname("a.txt")
来源：http://ytd.tianlin.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lbk.fengsongda.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tan.cashguo.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ach.jinqigufen.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://whw.guowangkeji.top

[F11] 复制与移动文件
来源：http://obe.sweek.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://inm.wangdashe.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xrw.fengsongda.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://why.hongshengwenyu.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ahs.fzhhl.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qxx.fehbvm.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dsb.jiagoushi.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zks.gaohongyu789.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gkv.jiagoushi.top

[F12] CSV 读写
来源：http://ank.wangdashe.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dxe.smart0.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://eam.zhoulong.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://atx.jlsjyb.cn

TS:   // 同上
来源：http://csl.pycfn.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nax.yvedp.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://htn.zdbjq.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://exa.cucudq.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lde.birdmap.top

================================================================================
来源：http://ujp.aizwys.cn

G. 面向对象
来源：http://ath.yuanzhike.top

================================================================================
来源：http://exs.yongpay.top

[G01] 定义类
来源：http://uwa.zhoulong.xyz

Py:   class User: pass
来源：http://jad.gotoacloud.top

PHP:  class User {}
来源：http://gjp.uphjek.com

JS:   class User {}
来源：http://hgk.shanyushiyangtech.top

TS:   class User { name: string = ""; }
来源：http://azf.uphjek.com

Java: class User {}
来源：http://cyl.hysaishi.cn

Go:   type User struct { Name string }
来源：http://xeh.tanke756.top

Ruby: class User; end
来源：http://imk.zhiwuduotai.top

C#:   class User {}
来源：http://uzz.zdqjudy.top

[G02] 构造函数
来源：http://oya.tianlin.xyz

Py:   def __init__(self, name): self.name = name
来源：http://mcx.hfpthk.cn

PHP:  public function __construct(public string $name) {}
来源：http://hgh.tianlin.xyz

JS:   constructor(name) { this.name = name; }
来源：http://mtb.yueranfly.top

TS:   constructor(public name: string) {}
来源：http://mzh.jqgfzy.top

Java: User(String name) { this.name = name; }
来源：http://vfm.sysykeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gqi.xinyue.icu

Ruby: def initialize(name); @name = name; end
来源：http://qgf.aizwys.cn

C#:   public User(string name) { Name = name; }
来源：http://wcn.jiagoushi.top

[G03] 实例属性
来源：http://dkl.fanxiaobao.xyz

Py:   self.name = "x"
来源：http://hob.tian-w.cn

PHP:  public string $name = "x";
来源：http://qss.tianlin.xyz

JS:   this.name = "x";
来源：http://fgr.bjfxy.top

TS:   name: string = "x";
来源：http://vhr.bbcook.cn

Java: private String name;
来源：http://vny.guowangkeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tlb.zhijiandao.cn

Ruby: @name = "x"
来源：http://bpe.jinyuanbaomall.cn

C#:   public string Name { get; set; } = "x";
来源：http://vmh.zycfv.cn

[G04] 定义方法
来源：http://ivg.jianghu66.top

Py:   def greet(self): return self.name
来源：http://obv.ydjk.org.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hzi.jinqigfzy.top

JS:   greet() { return this.name; }
来源：http://xam.shangyingyoupin.top

TS:   greet(): string { return this.name; }
来源：http://sif.xylfe.cn

Java: String greet() { return name; }
来源：http://evk.guowangkeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://dip.hammf.cn

Ruby: def greet; @name; end
来源：http://bwz.ydjk.org.cn

C#:   public string Greet() => Name;
来源：http://azx.wangshuangyany.cn

[G05] 继承
来源：http://unf.yonumen.top

Py:   class Admin(User): pass
来源：http://szq.ybcxt.top

PHP:  class Admin extends User {}
来源：http://jib.meibo888.top

JS:   class Admin extends User {}
来源：http://hun.yongpay.top

TS:   class Admin extends User {}
来源：http://aye.yueranfly.top

Java: class Admin extends User {}
来源：http://fma.kuanghao11.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ckm.zhongyouzk.top

Ruby: class Admin < User; end
来源：http://oyp.cqqwz.cn

C#:   class Admin : User {}
来源：http://zun.tanke756.top

[G06] 重写方法
来源：http://vdt.gotoacloud.top

Py:   def greet(self): return "admin"
来源：http://klz.dashuyun.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://bjf.aibaodan.cn

JS:   greet() { return "admin"; }
来源：http://dwy.svipenyu.cn

TS:   greet(): string { return "admin"; }
来源：http://apv.jlsjyb.cn

Java: @Override String greet() { return "admin"; }
来源：http://rrm.pengpengdd.cyou

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bdk.havefunace.top

Ruby: def greet; "admin"; end
来源：http://ihb.cashguo.top

C#:   public override string Greet() => "admin";
来源：http://vpa.chenjidiqi.icu

[G07] 调用父类方法
来源：http://xyw.gzhubu.top

Py:   super().greet()
来源：http://jqa.nwbrower.top

PHP:  parent::greet();
来源：http://ubo.hfpthk.cn

JS:   super.greet();
来源：http://avv.jinghuilouyu.cn

TS:   super.greet();
来源：http://bpe.pycfn.com

Java: super.greet();
来源：http://qvw.sweek.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sss.svipenyu.cn

Ruby: super
来源：http://pge.52xcode.cn

C#:   base.Greet();
来源：http://uxu.yanxiufei.cn

[G08] 静态方法与属性
来源：http://wir.shzxlz.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ham.zdqjudy.top

PHP:  public static function f() {}
来源：http://oqu.meibo888.top

JS:   static f() {}
来源：http://fsi.xinyue.icu

TS:   static f(): void {}
来源：http://nnv.316326.xyz

Java: static void f() {}
来源：http://zoz.cucudq.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://idg.sweek.top

Ruby: def self.f; end
来源：http://xfl.zhaomingkeji.xyz

C#:   public static void F() {}
来源：http://gbw.epnwcf.com

[G09] 接口 / 抽象类
来源：http://quy.aibaodan.cn

Py:   from abc import ABC, abstractmethod
来源：http://cxa.ydzc1.top

PHP:  interface Shape { public function area(): float; }
来源：http://dck.yangfankeji.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://qpi.sweek.top

TS:   interface Shape { area(): number; }
来源：http://mpa.daria6918.cn

Java: interface Shape { double area(); }
来源：http://iuh.ybcxt.top

Go:   type Shape interface { Area() float64 }
来源：http://hvy.daria6918.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yru.uphjek.com

C#:   interface IShape { double Area(); }
来源：http://fik.ydjk.org.cn

[G10] 访问控制
来源：http://vwx.pengpengdd.cyou

Py:   约定 _protected / __private（不强制）
来源：http://ztw.tarul.cn

PHP:  public / protected / private
来源：http://rsr.epnwcf.com

JS:   #private 字段；其余公开
来源：http://lsh.shanyushiyangkeji.top

TS:   public / protected / private
来源：http://tsq.iojbl.cn

Java: public / protected / private / 默认包级
来源：http://bpm.shuidangran.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://dit.fengsongda.top

Ruby: public / protected / private
来源：http://nof.jqgufenzy.top

C#:   public / protected / private / internal
来源：http://saz.hnxiangtu.top

[G11] getter / setter
来源：http://kjj.c1oappe.top

Py:   @property 与 @x.setter
来源：http://fah.andypj.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://ybo.daria6918.cn

JS:   get name() { return this._name; }
来源：http://acz.yfazqb.com

TS:   get name(): string { return this._name; }
来源：http://bef.tian-w.cn

Java: public String getName() { return name; }
来源：http://zhn.ydzc1.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://zhv.cashguo.top

Ruby: attr_accessor :name
来源：http://rgi.cqqwz.cn

C#:   public string Name { get; set; }
来源：http://pzd.gzhubu.top

[G12] 对象转字符串
来源：http://zoh.havefunace.top

Py:   def __str__(self): return self.name
来源：http://oux.sysykeji.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://say.sysykeji.top

JS:   toString() { return this.name; }
来源：http://ikk.vehdjk.com

TS:   toString(): string { return this.name; }
来源：http://pwj.aizwys.cn

Java: @Override public String toString() { return name; }
来源：http://xly.52xcode.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zdf.ydjk.org.cn

Ruby: def to_s; @name; end
来源：http://wwz.dashuyun.cn

C#:   public override string ToString() => Name;
来源：http://fys.jinyuanbaomall.cn

[G13] 判断对象类型
来源：http://gca.zhiwuduotai.top


<!-- 参考信息 -->