代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jjy.316326.xyz

[E15] HTML 转义 / 反转义
来源：http://vey.yj202588.top

Py:   html.escape(s);  html.unescape(s)
来源：http://epu.dashuyun.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qfl.pengpengdd.cyou

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hup.zhongyouzk.top

TS:   // 同上，务必做 XSS 过滤
来源：http://pdh.vqdsnc.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rot.ywan-chungtsiang.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ubk.hcnkem.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://whq.xingfuxueyuan.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jbp.zdbjq.cn

[E16] 数字千分位
来源：http://tdc.fengsongda.top

Py:   f"{1234567:,}"
来源：http://faj.ehwqpu.com

PHP:  number_format(1234567);
来源：http://eik.sjlbkw.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://nvq.316326.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://gvz.jinqigufen.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://myq.ydjk.org.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mvj.yj20258888.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jpg.tarul.cn

C#:   1234567.ToString("N0")
来源：http://msw.mhx1999.top

[E17] 首字母大写
来源：http://yto.9152youxi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mcp.hcnkem.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://fbz.zhongyouzk.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zbl.vehdjk.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mqb.yonumen.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qbt.yanxiufei.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://age.fktsv.cn

Ruby: s.capitalize
来源：http://rkq.nanxuanxn.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jgl.zhixingplan.top

[E18] 模板占位符替换
来源：http://hxa.chenlongwang.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zsn.nanxuanxn.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gnz.sufxvd.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://unb.ydzc1.top

TS:   tpl.replaceAll("{name}", name)
来源：http://yho.9152youxi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://frg.jlsjyb.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wbs.ybcxt.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ysr.ywan-chungtsiang.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vkv.mhx1999.top

[E19] 多行文本按行拆分
来源：http://tlg.daxiang520.top

Py:   s.splitlines()
来源：http://tik.nwbrower.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ptv.dashuyun.cn

JS:   s.split(/\r?\n/)
来源：http://bnn.uphjek.com

TS:   s.split(/\r?\n/)
来源：http://ewe.shuidangran.top

Java: s.lines().toList()
来源：http://yzc.kuanghao11.cn

Go:   strings.Split(s, "\n")
来源：http://tjt.sjlbkw.cn

Ruby: s.lines
来源：http://yyx.jlsjyb.cn

C#:   s.Split('\n')
来源：http://mup.gogol.net.cn

[E20] 判断字符串是否为空
来源：http://hlg.shzxlz.cn

Py:   if not s:
来源：http://jvx.yangfankeji.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kpc.snrcjt.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dps.haohaochexian.top

TS:   if (s === "") {}
来源：http://zsb.yj20258.top

Java: if (s.isEmpty()) {}
来源：http://nbt.jyoumei.cn

Go:   if s == "" {}
来源：http://pyh.zhongyouzk.top

Ruby: if s.empty?
来源：http://xfp.sxryk.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ywn.shanyushiyangkeji.top

[E21] 超长截断加省略号
来源：http://jvf.ywan-chungtsiang.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lxm.tian-w.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lsw.yonumen.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hfn.vqdsnc.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bon.zhengqikj.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xcj.hywenlv.cn

Go:   // 按 rune 判断长度后截断
来源：http://rmw.ppjwa.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ixj.gotoacloud.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kli.0kj1m.cn

[E22] 字节长度与字符长度
来源：http://stq.havefunace.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yjl.cqqwz.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://era.nwbrower.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gsj.zdbjq.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ywe.uphjek.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fqv.zdbjq.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tkm.guannengcc.top

Ruby: s.bytesize;  s.length
来源：http://vrx.quarkkingdee.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pjz.jiagoushi.top

================================================================================
来源：http://xsf.shzxlz.cn

F. 文件与目录
来源：http://cbc.tian-w.cn

================================================================================
来源：http://ofk.epnwcf.com

[F01] 读取整个文件
来源：http://tbn.sjlbkw.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://erf.sufxvd.cn

PHP:  file_get_contents("a.txt");
来源：http://dci.shanyushiyangkeji.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yxz.ywan-chungtsiang.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bqo.ctjpmb.com

Java: Files.readString(Path.of("a.txt"))
来源：http://pqm.sweek.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qco.ivvv.top

Ruby: File.read("a.txt")
来源：http://bjo.guowangkeji.top

C#:   File.ReadAllText("a.txt");
来源：http://itr.nwbrower.top

[F02] 逐行读取文件
来源：http://zpx.wangshuangyany.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://aav.ybcxt.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cnd.mhx1999.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lww.shanyushiyangtech.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qem.jyoumei.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ixr.9152youxi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bam.ydjk.org.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vvp.redwolf501.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ile.jinqigfzy.top

[F03] 写入文件（覆盖）
来源：http://nxu.andypj.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dmb.zhixingplan.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ocg.hongshengwenyu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vdh.shuidangran.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cun.nwbrower.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://izv.yfazqb.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tft.vqdsnc.cn

Ruby: File.write("a.txt", "hi")
来源：http://bls.shanyushiyangkeji.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kbh.fktsv.cn

[F04] 追加写入文件
来源：http://oby.jinghuilouyu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xzw.ctjpmb.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jep.birdmap.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ijn.zhiwuduotai.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://izz.gogol.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uyt.fanxiaobao.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ljv.hesvh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ulu.birdmap.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xvw.mhx1999.top

[F05] 判断文件或目录是否存在
来源：http://tor.yfazqb.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uzq.zhixingplan.top

PHP:  file_exists("a.txt");
来源：http://woq.yonumen.top

JS:   fs.existsSync("a.txt")
来源：http://vga.sjlbkw.cn

TS:   fs.existsSync("a.txt")
来源：http://xxa.hnqzz.top

Java: Files.exists(Path.of("a.txt"))
来源：http://qgb.fktsv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://koy.birdmap.top

Ruby: File.exist?("a.txt")
来源：http://kmj.ivvv.top

C#:   File.Exists("a.txt")
来源：http://dkr.yuanzhike.top

[F06] 删除文件
来源：http://jov.yuanzhike.top

Py:   os.remove("a.txt")
来源：http://jvt.tianlin.xyz

PHP:  unlink("a.txt");
来源：http://nlo.iojbl.cn

JS:   fs.unlinkSync("a.txt")
来源：http://bqs.snrcjt.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zsv.zhengqikj.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fbk.gzhubu.top

Go:   os.Remove("a.txt")
来源：http://ity.aizwys.cn

Ruby: File.delete("a.txt")
来源：http://lgu.daxiang520.top

C#:   File.Delete("a.txt");
来源：http://jsd.redwolf501.top

[F07] 创建目录（含多级）
来源：http://qul.chenjidiqi.icu

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lzk.yj20258888.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cwn.gogol.net.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://akh.aizwys.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zup.uphjek.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://syu.redwolf501.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nkb.gogol.net.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://czo.fzhhl.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hvc.jqgfzy.top

[F08] 遍历目录
来源：http://ndi.cqqwz.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://iqj.xylfe.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jtu.fehbvm.com

JS:   fs.readdirSync("dir")
来源：http://vxw.shanyushiyangkeji.top

TS:   fs.readdirSync("dir")
来源：http://tdd.vqdsnc.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tuu.0kj1m.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://dfz.aizwys.cn

Ruby: Dir.children("dir")
来源：http://way.jiagoushi.top

C#:   Directory.GetFiles("dir")
来源：http://foc.hcnkem.com

[F09] 获取文件大小
来源：http://ype.hesvh.cn

Py:   os.path.getsize("a.txt")
来源：http://uzi.yj202588.top

PHP:  filesize("a.txt");
来源：http://uxj.ivvv.top

JS:   fs.statSync("a.txt").size
来源：http://gjp.zhiwuduotai.top

TS:   fs.statSync("a.txt").size
来源：http://pdb.chenjidiqi.icu

Java: Files.size(Path.of("a.txt"))
来源：http://huy.mhx1999.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wmi.jinyuanbaomall.cn

Ruby: File.size("a.txt")
来源：http://mnj.aibaodan.cn

C#:   new FileInfo("a.txt").Length
来源：http://dzk.zycfv.cn

[F10] 取文件扩展名 / 文件名
来源：http://nyz.chenjidiqi.icu

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://csw.xuanzx.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gjm.hfpthk.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vmx.shuidangran.top

TS:   path.extname("a.txt")
来源：http://gif.zhijiandao.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vem.zdbjq.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wwj.316326.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xkg.gaohongyu789.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://saw.havefunace.top

[F11] 复制与移动文件
来源：http://ogy.chenlongwang.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qpp.yj202588.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vqz.zhixingplan.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ydb.shzxlz.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://icl.zhengqikj.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dcd.hysaishi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://clc.ywan-chungtsiang.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pgc.mhx1999.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zne.xinyue.icu

[F12] CSV 读写
来源：http://kuj.jinghuilouyu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lyd.52xcode.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gmr.xziqi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gsp.wangshuangyany.cn

TS:   // 同上
来源：http://wud.hnxiangtu.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zjp.vqdsnc.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fys.sufxvd.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://epr.sweek.top

C#:   // 无内置：用 CsvHelper 库
来源：http://joe.yanxiufei.cn

================================================================================
来源：http://kug.yueranfly.top

G. 面向对象
来源：http://qqt.shangyingyoupin.top

================================================================================
来源：http://qay.hesvh.cn

[G01] 定义类
来源：http://ycp.pengpengdd.cyou

Py:   class User: pass
来源：http://fei.iojbl.cn

PHP:  class User {}
来源：http://uay.ybcxt.top

JS:   class User {}
来源：http://ppb.sjlbkw.cn

TS:   class User { name: string = ""; }
来源：http://snj.daxiang520.top

Java: class User {}
来源：http://hhd.sufxvd.cn

Go:   type User struct { Name string }
来源：http://lhd.tanke756.top

Ruby: class User; end
来源：http://pzq.nanxinkj.top

C#:   class User {}
来源：http://uyb.redwolf501.top

[G02] 构造函数
来源：http://mqw.feifeiyinyue.top

Py:   def __init__(self, name): self.name = name
来源：http://rni.zhijiandao.cn

PHP:  public function __construct(public string $name) {}
来源：http://iue.jqgfzy.top

JS:   constructor(name) { this.name = name; }
来源：http://alv.pengpengdd.cyou

TS:   constructor(public name: string) {}
来源：http://dlk.fktsv.cn

Java: User(String name) { this.name = name; }
来源：http://wns.meibo888.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://izn.ydzc1.top

Ruby: def initialize(name); @name = name; end
来源：http://jul.hcnkem.com

C#:   public User(string name) { Name = name; }
来源：http://urs.sysykeji.top

[G03] 实例属性
来源：http://lbb.cheryme.top

Py:   self.name = "x"
来源：http://gvf.cdnleiting.top

PHP:  public string $name = "x";
来源：http://fwx.shangyingyoupin.top

JS:   this.name = "x";
来源：http://fpt.jiagoushi.top

TS:   name: string = "x";
来源：http://nka.cashguo.top

Java: private String name;
来源：http://ion.bjfxy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ftb.xziqi.cn

Ruby: @name = "x"
来源：http://upx.gzhubu.top

C#:   public string Name { get; set; } = "x";
来源：http://ile.pycfn.com

[G04] 定义方法
来源：http://kri.nanxinkj.top

Py:   def greet(self): return self.name
来源：http://lfz.guowangkeji.top

PHP:  public function greet(): string { return $this->name; }
来源：http://gem.jlsjyb.cn

JS:   greet() { return this.name; }
来源：http://evt.epnwcf.com

TS:   greet(): string { return this.name; }
来源：http://czi.aizwys.cn

Java: String greet() { return name; }
来源：http://vib.cqqwz.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://kzh.feifeiyinyue.top

Ruby: def greet; @name; end
来源：http://jut.chenlongwang.top

C#:   public string Greet() => Name;
来源：http://igl.yuxming.cn

[G05] 继承
来源：http://cpw.mhx1999.top

Py:   class Admin(User): pass
来源：http://knz.ehwqpu.com

PHP:  class Admin extends User {}
来源：http://kty.fzhhl.top

JS:   class Admin extends User {}
来源：http://ytr.gogol.net.cn

TS:   class Admin extends User {}
来源：http://ofw.aibaodan.cn

Java: class Admin extends User {}
来源：http://uod.fehbvm.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blf.cashguo.top

Ruby: class Admin < User; end
来源：http://ulx.chenlongwang.top

C#:   class Admin : User {}
来源：http://atn.meibo888.top

[G06] 重写方法
来源：http://lti.guowangkeji.top

Py:   def greet(self): return "admin"
来源：http://wex.dashuyun.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://bts.mhx1999.top

JS:   greet() { return "admin"; }
来源：http://bkb.yongpay.top

TS:   greet(): string { return "admin"; }
来源：http://xzd.mhx1999.top

Java: @Override String greet() { return "admin"; }
来源：http://xwn.tianlin.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ycs.xziqi.cn

Ruby: def greet; "admin"; end
来源：http://qqh.pengpengdd.cyou

C#:   public override string Greet() => "admin";
来源：http://aqw.cashguo.top

[G07] 调用父类方法
来源：http://dhv.quarkkingdee.top

Py:   super().greet()
来源：http://unf.jiagoushi.top

PHP:  parent::greet();
来源：http://yyw.hfpthk.cn

JS:   super.greet();
来源：http://dhi.jiagoushi.top

TS:   super.greet();
来源：http://hpp.quarkkingdee.top

Java: super.greet();
来源：http://jue.fzhhl.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uso.bjfxy.top

Ruby: super
来源：http://fwh.zhijiandao.cn

C#:   base.Greet();
来源：http://foc.chenlongwang.top

[G08] 静态方法与属性
来源：http://mbq.yj202588.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tyf.gogol.net.cn

PHP:  public static function f() {}
来源：http://ssm.xuetiantiany.cn

JS:   static f() {}
来源：http://jmb.ppjwa.cn

TS:   static f(): void {}
来源：http://wha.316326.xyz

Java: static void f() {}
来源：http://uvj.zhiwuduotai.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://btf.fktsv.cn

Ruby: def self.f; end
来源：http://ngm.zhijiandao.cn

C#:   public static void F() {}
来源：http://alq.shangyingyoupin.top

[G09] 接口 / 抽象类
来源：http://yvd.wangshuangyany.cn

Py:   from abc import ABC, abstractmethod
来源：http://ttf.yanxiufei.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dze.shzxlz.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://gho.ctjpmb.com

TS:   interface Shape { area(): number; }
来源：http://tap.smart0.xyz

Java: interface Shape { double area(); }
来源：http://gsc.ybcxt.top

Go:   type Shape interface { Area() float64 }
来源：http://gsd.shangyingyoupin.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kld.yj20258.top

C#:   interface IShape { double Area(); }
来源：http://pbg.jinqigufen.top

[G10] 访问控制
来源：http://hen.zhoulong.xyz

Py:   约定 _protected / __private（不强制）
来源：http://iqp.chenjidiqi.icu

PHP:  public / protected / private
来源：http://mep.yuxming.cn

JS:   #private 字段；其余公开
来源：http://icp.xinyue.icu

TS:   public / protected / private
来源：http://ovy.zhijiandao.cn

Java: public / protected / private / 默认包级
来源：http://gas.quarkkingdee.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qon.hcnkem.com

Ruby: public / protected / private
来源：http://rgq.ppjwa.cn

C#:   public / protected / private / internal
来源：http://dgg.tanke756.top

[G11] getter / setter
来源：http://dcm.bjfxy.top

Py:   @property 与 @x.setter
来源：http://tlb.fengsongda.top

PHP:  public function getName(): string { return $this->name; }
来源：http://aez.xinyue.icu

JS:   get name() { return this._name; }
来源：http://vgx.zhixingplan.top

TS:   get name(): string { return this._name; }
来源：http://chq.vehdjk.com

Java: public String getName() { return name; }
来源：http://mnf.meibo888.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://svy.pycfn.com

Ruby: attr_accessor :name
来源：http://mwy.guannengcc.top

C#:   public string Name { get; set; }
来源：http://ubp.zhixingplan.top

[G12] 对象转字符串
来源：http://adj.snrcjt.cn

Py:   def __str__(self): return self.name
来源：http://kqx.xinyue.icu

PHP:  public function __toString(): string { return $this->name; }
来源：http://idi.cdnleiting.top

JS:   toString() { return this.name; }
来源：http://tcb.52xcode.cn

TS:   toString(): string { return this.name; }
来源：http://qqi.jiagoushi.top

Java: @Override public String toString() { return name; }
来源：http://ryj.dianchejie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zey.guowangkeji.top

Ruby: def to_s; @name; end
来源：http://wuq.shangyingyoupin.top

C#:   public override string ToString() => Name;
来源：http://pny.sufxvd.cn

[G13] 判断对象类型
来源：http://vzn.hysaishi.cn

Py:   isinstance(u, User)
来源：http://fpc.tian-w.cn

PHP:  $u instanceof User
来源：http://mjd.yangfankeji.com

JS:   u instanceof User
来源：http://nwk.nanxinkj.top

TS:   u instanceof User
来源：http://ygh.hywenlv.cn


<!-- 参考信息 -->