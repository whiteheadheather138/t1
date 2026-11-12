代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hea.ehwqpu.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://exq.birdmap.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pea.zhijiandao.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kma.daria6918.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xeq.sxryk.cn

[E15] HTML 转义 / 反转义
来源：http://dmm.feifeiyinyue.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ylg.wangdashe.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://giu.cdnleiting.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gxw.nanxuanxn.top

TS:   // 同上，务必做 XSS 过滤
来源：http://wmz.vqdsnc.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fvz.ywan-chungtsiang.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://egz.yj202588.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://acx.daria6918.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ksg.fehbvm.com

[E16] 数字千分位
来源：http://hxv.vqdsnc.cn

Py:   f"{1234567:,}"
来源：http://cmw.wangdashe.top

PHP:  number_format(1234567);
来源：http://aii.316326.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://ohe.yvedp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://dvs.epnwcf.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rsr.hongshengwenyu.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qlv.jinyuanbaomall.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nnm.fehbvm.com

C#:   1234567.ToString("N0")
来源：http://jls.zdqjudy.top

[E17] 首字母大写
来源：http://pua.hnxiangtu.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ueg.sjlbkw.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hne.hfpthk.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jog.jyoumei.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cfw.hcnkem.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rjl.tianlin.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://knp.zdbjq.cn

Ruby: s.capitalize
来源：http://bxg.iojbl.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pca.aibaodan.cn

[E18] 模板占位符替换
来源：http://iok.kuanghao11.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sja.hammf.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nsv.zhixingplan.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ssw.sxryk.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://xef.hnqzz.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vdj.dashuyun.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pcv.fzhhl.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mcw.zhixingplan.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lov.jiagoushi.top

[E19] 多行文本按行拆分
来源：http://cpg.guannengcc.top

Py:   s.splitlines()
来源：http://gzn.52xcode.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hoj.jinyuanbaomall.cn

JS:   s.split(/\r?\n/)
来源：http://wtk.ybcxt.top

TS:   s.split(/\r?\n/)
来源：http://fcv.hnqzz.top

Java: s.lines().toList()
来源：http://lpy.c1oappe.top

Go:   strings.Split(s, "\n")
来源：http://tdo.xuetiantiany.cn

Ruby: s.lines
来源：http://oal.pycfn.com

C#:   s.Split('\n')
来源：http://wtw.fanxiaobao.xyz

[E20] 判断字符串是否为空
来源：http://hao.fehbvm.com

Py:   if not s:
来源：http://ymc.ppjwa.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fnj.gaohongyu789.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yyw.daxiang520.top

TS:   if (s === "") {}
来源：http://fei.quarkkingdee.top

Java: if (s.isEmpty()) {}
来源：http://dpp.c1oappe.top

Go:   if s == "" {}
来源：http://zin.yangfankeji.com

Ruby: if s.empty?
来源：http://vkc.aizwys.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gev.ydzc1.top

[E21] 超长截断加省略号
来源：http://fgk.yj20258.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ifn.yj202588.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ynk.ppjwa.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fze.dashuyun.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jjg.jianghu66.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://arv.jiagoushi.top

Go:   // 按 rune 判断长度后截断
来源：http://clv.iojbl.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rqu.yanxiufei.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zna.haohaochexian.top

[E22] 字节长度与字符长度
来源：http://zem.mhx1999.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gjp.epnwcf.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vey.birdmap.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cnh.fengsongda.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://smy.zhaomingkeji.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://eyf.yanxiufei.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yut.ydjk.org.cn

Ruby: s.bytesize;  s.length
来源：http://frj.sweek.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ene.dianchejie.cn

================================================================================
来源：http://mdl.guowangkeji.top

F. 文件与目录
来源：http://ect.c1oappe.top

================================================================================
来源：http://ybi.ppjwa.cn

[F01] 读取整个文件
来源：http://puy.redwolf501.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pcy.cucudq.cn

PHP:  file_get_contents("a.txt");
来源：http://mfg.daria6918.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fzt.jianghu66.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bfu.zhiwuduotai.top

Java: Files.readString(Path.of("a.txt"))
来源：http://clf.meibo888.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://los.havefunace.top

Ruby: File.read("a.txt")
来源：http://sub.cdnleiting.top

C#:   File.ReadAllText("a.txt");
来源：http://qbe.bbcook.cn

[F02] 逐行读取文件
来源：http://cgp.jiagoushi.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rpl.ppjwa.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://emu.xinyue.icu

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://igf.xingfuxueyuan.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vvg.xuanzx.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uvd.yfazqb.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://srp.hnxiangtu.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rfl.sysykeji.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mdb.daxiang520.top

[F03] 写入文件（覆盖）
来源：http://kkq.shanyushiyangtech.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xhf.chenjidiqi.icu

PHP:  file_put_contents("a.txt", "hi");
来源：http://tli.fanxiaobao.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://euv.uphjek.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rrh.meibo888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://php.jlsjyb.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sfs.smart0.xyz

Ruby: File.write("a.txt", "hi")
来源：http://cen.chenjidiqi.icu

C#:   File.WriteAllText("a.txt", "hi");
来源：http://juy.52xcode.cn

[F04] 追加写入文件
来源：http://acu.yuanzhike.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gqd.cqqwz.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://atb.sweek.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tyf.9152youxi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wph.zhixingplan.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lqy.fktsv.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xyb.zhaomingkeji.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dca.jiagoushi.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://iwx.yuanzhike.top

[F05] 判断文件或目录是否存在
来源：http://rzx.shanyushiyangkeji.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uwu.fehbvm.com

PHP:  file_exists("a.txt");
来源：http://blz.yuanzhike.top

JS:   fs.existsSync("a.txt")
来源：http://yqm.ehwqpu.com

TS:   fs.existsSync("a.txt")
来源：http://fzl.dashuyun.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://aqu.svipenyu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dgd.shanyushiyangtech.top

Ruby: File.exist?("a.txt")
来源：http://pzw.fehbvm.com

C#:   File.Exists("a.txt")
来源：http://qqq.hcnkem.com

[F06] 删除文件
来源：http://djn.redwolf501.top

Py:   os.remove("a.txt")
来源：http://igv.svipenyu.cn

PHP:  unlink("a.txt");
来源：http://lfq.havefunace.top

JS:   fs.unlinkSync("a.txt")
来源：http://uhs.zhixingplan.top

TS:   fs.unlinkSync("a.txt")
来源：http://egi.svipenyu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://idx.jlsjyb.cn

Go:   os.Remove("a.txt")
来源：http://hbx.snrcjt.cn

Ruby: File.delete("a.txt")
来源：http://szw.andypj.xyz

C#:   File.Delete("a.txt");
来源：http://gja.zycfv.cn

[F07] 创建目录（含多级）
来源：http://tch.fktsv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bhn.jinyuanbaomall.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zjm.nwbrower.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vvv.zhaomingkeji.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cre.hongshengwenyu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://igh.uphjek.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fao.havefunace.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ufq.yuanzhike.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lod.316326.xyz

[F08] 遍历目录
来源：http://dsl.meibo888.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://wcv.hammf.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kdu.shanyushiyangkeji.top

JS:   fs.readdirSync("dir")
来源：http://mtj.sysykeji.top

TS:   fs.readdirSync("dir")
来源：http://gjv.ywan-chungtsiang.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tvs.xingfuxueyuan.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://bta.hongshengwenyu.top

Ruby: Dir.children("dir")
来源：http://jls.yanxiufei.cn

C#:   Directory.GetFiles("dir")
来源：http://ogy.yongpay.top

[F09] 获取文件大小
来源：http://xih.zycfv.cn

Py:   os.path.getsize("a.txt")
来源：http://czm.smart0.xyz

PHP:  filesize("a.txt");
来源：http://xbl.xziqi.cn

JS:   fs.statSync("a.txt").size
来源：http://htr.316326.xyz

TS:   fs.statSync("a.txt").size
来源：http://ykk.ydjk.org.cn

Java: Files.size(Path.of("a.txt"))
来源：http://qsn.gzhubu.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://icn.jqgfzy.top

Ruby: File.size("a.txt")
来源：http://had.meibo888.top

C#:   new FileInfo("a.txt").Length
来源：http://ykx.sjlbkw.cn

[F10] 取文件扩展名 / 文件名
来源：http://hzq.jinqigufen.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://goj.xylfe.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bua.xuanzx.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hig.aizwys.cn

TS:   path.extname("a.txt")
来源：http://ozf.fktsv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rhx.hongshengwenyu.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sfs.havefunace.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zex.chenzaomai.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qkb.zhengqikj.top

[F11] 复制与移动文件
来源：http://jpe.xuanzx.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xgb.birdmap.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wjs.bbcook.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kxk.zhongyouzk.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vaw.chenzaomai.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dqg.hammf.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rxk.gzhubu.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yaj.aizwys.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dts.shanyushiyangkeji.top

[F12] CSV 读写
来源：http://oxc.fengsongda.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cxz.nanxuanxn.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sub.sysykeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nyu.birdmap.top

TS:   // 同上
来源：http://vae.xziqi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rou.zhiwuduotai.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mxl.jqgufenzy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://iej.shanyushiyangkeji.top

C#:   // 无内置：用 CsvHelper 库
来源：http://van.zhengqikj.top

================================================================================
来源：http://ziy.jiagoushi.top

G. 面向对象
来源：http://vin.aibaodan.cn

================================================================================
来源：http://pyu.xylfe.cn

[G01] 定义类
来源：http://ieh.wangdashe.top

Py:   class User: pass
来源：http://qaw.hcnkem.com

PHP:  class User {}
来源：http://jbi.cashguo.top

JS:   class User {}
来源：http://hdp.tarul.cn

TS:   class User { name: string = ""; }
来源：http://zap.guannengcc.top

Java: class User {}
来源：http://auw.aibaodan.cn

Go:   type User struct { Name string }
来源：http://ozi.tarul.cn

Ruby: class User; end
来源：http://ehv.wangdashe.top

C#:   class User {}
来源：http://kxe.fengsongda.top

[G02] 构造函数
来源：http://amn.shzxlz.cn

Py:   def __init__(self, name): self.name = name
来源：http://hos.jinghuilouyu.cn

PHP:  public function __construct(public string $name) {}
来源：http://ivx.zycfv.cn

JS:   constructor(name) { this.name = name; }
来源：http://nkj.jinqigfzy.top

TS:   constructor(public name: string) {}
来源：http://igo.bjfxy.top

Java: User(String name) { this.name = name; }
来源：http://nuz.zhongyouzk.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://iny.jinyuanbaomall.cn

Ruby: def initialize(name); @name = name; end
来源：http://poj.andypj.xyz

C#:   public User(string name) { Name = name; }
来源：http://dqp.chenlongwang.top

[G03] 实例属性
来源：http://iqa.tian-w.cn

Py:   self.name = "x"
来源：http://ogy.hfpthk.cn

PHP:  public string $name = "x";
来源：http://yyz.meibo888.top

JS:   this.name = "x";
来源：http://fbp.daxiang520.top

TS:   name: string = "x";
来源：http://nia.zhixingplan.top

Java: private String name;
来源：http://bvj.hysaishi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://skx.zhoulong.xyz

Ruby: @name = "x"
来源：http://dkh.ehwqpu.com

C#:   public string Name { get; set; } = "x";
来源：http://hel.birdmap.top

[G04] 定义方法
来源：http://vub.hammf.cn

Py:   def greet(self): return self.name
来源：http://zzo.fktsv.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://qej.xylfe.cn

JS:   greet() { return this.name; }
来源：http://jki.chenjidiqi.icu

TS:   greet(): string { return this.name; }
来源：http://idk.shzxlz.cn

Java: String greet() { return name; }
来源：http://etk.nanxuanxn.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://cgu.xziqi.cn

Ruby: def greet; @name; end
来源：http://xry.fanxiaobao.xyz

C#:   public string Greet() => Name;
来源：http://uwh.wangshuangyany.cn

[G05] 继承
来源：http://dzg.vqdsnc.cn

Py:   class Admin(User): pass
来源：http://kcm.daria6918.cn

PHP:  class Admin extends User {}
来源：http://cgy.jlsjyb.cn

JS:   class Admin extends User {}
来源：http://hcl.zhixingplan.top

TS:   class Admin extends User {}
来源：http://scg.fktsv.cn

Java: class Admin extends User {}
来源：http://hkh.vehdjk.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://geo.yvedp.cn

Ruby: class Admin < User; end
来源：http://avk.hysaishi.cn

C#:   class Admin : User {}
来源：http://let.sxryk.cn

[G06] 重写方法
来源：http://szx.yj20258888.top

Py:   def greet(self): return "admin"
来源：http://pge.shangyingyoupin.top

PHP:  public function greet(): string { return "admin"; }
来源：http://wvd.hammf.cn

JS:   greet() { return "admin"; }
来源：http://zte.xuetiantiany.cn

TS:   greet(): string { return "admin"; }
来源：http://rfi.meibo888.top

Java: @Override String greet() { return "admin"; }
来源：http://jek.shuidangran.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pzp.quarkkingdee.top

Ruby: def greet; "admin"; end
来源：http://ayo.daxiang520.top

C#:   public override string Greet() => "admin";
来源：http://dgv.ehwqpu.com

[G07] 调用父类方法
来源：http://dxb.yueranfly.top

Py:   super().greet()
来源：http://zgz.tian-w.cn

PHP:  parent::greet();
来源：http://lmu.sufxvd.cn

JS:   super.greet();
来源：http://gju.ivvv.top

TS:   super.greet();
来源：http://vgg.hongshengwenyu.top

Java: super.greet();
来源：http://mpl.tian-w.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xos.wangdashe.top

Ruby: super
来源：http://xia.sweek.top

C#:   base.Greet();
来源：http://ugt.xuetiantiany.cn

[G08] 静态方法与属性
来源：http://cqt.hesvh.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hpy.jqgufenzy.top

PHP:  public static function f() {}
来源：http://bip.shanyushiyangkeji.top

JS:   static f() {}
来源：http://mfz.zhaomingkeji.xyz

TS:   static f(): void {}
来源：http://vad.hnqzz.top

Java: static void f() {}
来源：http://acd.nanxuanxn.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ian.gogol.net.cn

Ruby: def self.f; end
来源：http://cem.tianlin.xyz

C#:   public static void F() {}
来源：http://rbp.guowangkeji.top

[G09] 接口 / 抽象类
来源：http://plm.hnqzz.top

Py:   from abc import ABC, abstractmethod
来源：http://qfo.zdqjudy.top

PHP:  interface Shape { public function area(): float; }
来源：http://qio.nanxinkj.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://iti.shanyushiyangtech.top

TS:   interface Shape { area(): number; }
来源：http://zsj.yanxiufei.cn

Java: interface Shape { double area(); }
来源：http://uqj.quarkkingdee.top

Go:   type Shape interface { Area() float64 }
来源：http://zit.ydzc1.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fhq.daria6918.cn

C#:   interface IShape { double Area(); }
来源：http://xdd.birdmap.top

[G10] 访问控制
来源：http://tvr.redwolf501.top

Py:   约定 _protected / __private（不强制）
来源：http://fkd.birdmap.top

PHP:  public / protected / private
来源：http://qea.yfazqb.com

JS:   #private 字段；其余公开
来源：http://eoj.zhengqikj.top

TS:   public / protected / private
来源：http://tbs.shanyushiyangkeji.top

Java: public / protected / private / 默认包级
来源：http://kxw.cashguo.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qvt.ppjwa.cn

Ruby: public / protected / private
来源：http://amr.havefunace.top

C#:   public / protected / private / internal
来源：http://jxn.zhijiandao.cn

[G11] getter / setter
来源：http://dcf.svipenyu.cn

Py:   @property 与 @x.setter
来源：http://esa.daxiang520.top

PHP:  public function getName(): string { return $this->name; }
来源：http://rpr.bjfxy.top

JS:   get name() { return this._name; }
来源：http://jxt.havefunace.top

TS:   get name(): string { return this._name; }
来源：http://unt.zhaomingkeji.xyz

Java: public String getName() { return name; }
来源：http://qhe.ppjwa.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://puc.jinyuanbaomall.cn

Ruby: attr_accessor :name
来源：http://ajp.nanxuanxn.top

C#:   public string Name { get; set; }
来源：http://gvr.daxiang520.top

[G12] 对象转字符串
来源：http://wvc.jinqigfzy.top

Py:   def __str__(self): return self.name
来源：http://drt.zhoulong.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://bah.daxiang520.top

JS:   toString() { return this.name; }
来源：http://gei.chenjidiqi.icu

TS:   toString(): string { return this.name; }
来源：http://clc.shanyushiyangtech.top

Java: @Override public String toString() { return name; }
来源：http://oea.fengsongda.top

Go:   func (u User) String() string { return u.Name }
来源：http://qyd.yuxming.cn

Ruby: def to_s; @name; end
来源：http://sbt.xziqi.cn

C#:   public override string ToString() => Name;
来源：http://vdv.snrcjt.cn

[G13] 判断对象类型
来源：http://nqy.chenjidiqi.icu


<!-- 参考信息 -->