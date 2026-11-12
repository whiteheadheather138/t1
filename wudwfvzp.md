代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ytn.fanxiaobao.xyz

[E15] HTML 转义 / 反转义
来源：http://eic.xylfe.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rss.tarul.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nzv.hcnkem.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rwe.zhengqikj.top

TS:   // 同上，务必做 XSS 过滤
来源：http://odg.meibo888.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ymh.hongshengwenyu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://idi.wangdashe.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lwx.snrcjt.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://azh.sufxvd.cn

[E16] 数字千分位
来源：http://jkm.jinqigufen.top

Py:   f"{1234567:,}"
来源：http://jtt.nanxuanxn.top

PHP:  number_format(1234567);
来源：http://gby.shzxlz.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wqr.vehdjk.com

TS:   (1234567).toLocaleString("en-US")
来源：http://aqb.nanxinkj.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fug.hnxiangtu.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fjv.sufxvd.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://aej.andypj.xyz

C#:   1234567.ToString("N0")
来源：http://rbc.yongpay.top

[E17] 首字母大写
来源：http://atm.nwbrower.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wwl.zdqjudy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ljo.nanxinkj.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kkz.quarkkingdee.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pub.hysaishi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jcd.cheryme.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mxx.zhiwuduotai.top

Ruby: s.capitalize
来源：http://hvl.yvedp.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kou.zycfv.cn

[E18] 模板占位符替换
来源：http://yjp.ydzc1.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fam.havefunace.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lej.yvedp.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gxs.snrcjt.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://peh.quarkkingdee.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tvz.feifeiyinyue.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xjn.9152youxi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lbf.zhijiandao.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vcj.ehwqpu.com

[E19] 多行文本按行拆分
来源：http://mgp.daria6918.cn

Py:   s.splitlines()
来源：http://lbw.zhongyouzk.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nxq.xingfuxueyuan.xyz

JS:   s.split(/\r?\n/)
来源：http://nhu.cashguo.top

TS:   s.split(/\r?\n/)
来源：http://sco.xuanzx.com

Java: s.lines().toList()
来源：http://qtv.gogol.net.cn

Go:   strings.Split(s, "\n")
来源：http://mze.tarul.cn

Ruby: s.lines
来源：http://zmn.mhx1999.top

C#:   s.Split('\n')
来源：http://nkw.nanxinkj.top

[E20] 判断字符串是否为空
来源：http://hmj.daxiang520.top

Py:   if not s:
来源：http://map.fktsv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mji.jinyuanbaomall.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lbk.dianchejie.cn

TS:   if (s === "") {}
来源：http://hll.vqdsnc.cn

Java: if (s.isEmpty()) {}
来源：http://jdq.jyoumei.cn

Go:   if s == "" {}
来源：http://dhn.zdbjq.cn

Ruby: if s.empty?
来源：http://mxc.zhiwuduotai.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://syw.bbcook.cn

[E21] 超长截断加省略号
来源：http://wjw.jqgfzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xyt.ydzc1.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wbs.yuanzhike.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dpc.daxiang520.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eio.vqdsnc.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pwx.chenlongwang.top

Go:   // 按 rune 判断长度后截断
来源：http://jdg.jiagoushi.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ake.jqgufenzy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pnw.chenlongwang.top

[E22] 字节长度与字符长度
来源：http://akv.ctjpmb.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qky.hywenlv.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kbh.yj20258888.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cqf.cheryme.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rhc.chenlongwang.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nfq.gzhubu.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wcf.hnqzz.top

Ruby: s.bytesize;  s.length
来源：http://mvt.jinyuanbaomall.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://phv.ydjk.org.cn

================================================================================
来源：http://fjp.fehbvm.com

F. 文件与目录
来源：http://fip.jinghuilouyu.cn

================================================================================
来源：http://aao.xingfuxueyuan.xyz

[F01] 读取整个文件
来源：http://kjq.chenlongwang.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xdw.yvedp.cn

PHP:  file_get_contents("a.txt");
来源：http://yee.zhixingplan.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ohd.zhengqikj.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nry.yfazqb.com

Java: Files.readString(Path.of("a.txt"))
来源：http://ytz.yj20258888.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lmy.jinyuanbaomall.cn

Ruby: File.read("a.txt")
来源：http://kzw.jiagoushi.top

C#:   File.ReadAllText("a.txt");
来源：http://mwl.jinghuilouyu.cn

[F02] 逐行读取文件
来源：http://scc.zhiwuduotai.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://txm.bbcook.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://oir.ivvv.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lzh.fehbvm.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hsl.chenzaomai.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lob.0kj1m.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://brh.yuxming.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ogk.kuanghao11.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://usb.ybcxt.top

[F03] 写入文件（覆盖）
来源：http://ttg.xuanzx.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nvs.hywenlv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fkr.52xcode.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://enh.jqgufenzy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dor.jqgfzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://udy.aibaodan.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vmz.jinyuanbaomall.cn

Ruby: File.write("a.txt", "hi")
来源：http://baz.hysaishi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xng.nwbrower.top

[F04] 追加写入文件
来源：http://vzt.shuidangran.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bdd.jinyuanbaomall.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ywn.jinqigufen.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xpj.xinyue.icu

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xvn.0kj1m.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qgn.bbcook.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vgh.meibo888.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bfc.kuanghao11.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ojm.hnxiangtu.top

[F05] 判断文件或目录是否存在
来源：http://tqq.xingfuxueyuan.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gxj.tanke756.top

PHP:  file_exists("a.txt");
来源：http://tvl.cqqwz.cn

JS:   fs.existsSync("a.txt")
来源：http://kee.fktsv.cn

TS:   fs.existsSync("a.txt")
来源：http://yyf.jianghu66.top

Java: Files.exists(Path.of("a.txt"))
来源：http://nsn.vehdjk.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qmo.quarkkingdee.top

Ruby: File.exist?("a.txt")
来源：http://bkf.iojbl.cn

C#:   File.Exists("a.txt")
来源：http://lgp.snrcjt.cn

[F06] 删除文件
来源：http://pde.xinyue.icu

Py:   os.remove("a.txt")
来源：http://ldj.shangyingyoupin.top

PHP:  unlink("a.txt");
来源：http://atk.cheryme.top

JS:   fs.unlinkSync("a.txt")
来源：http://rvf.9152youxi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://uhd.wangshuangyany.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zwi.cqqwz.cn

Go:   os.Remove("a.txt")
来源：http://rza.mhx1999.top

Ruby: File.delete("a.txt")
来源：http://zuk.hesvh.cn

C#:   File.Delete("a.txt");
来源：http://tjg.zhoulong.xyz

[F07] 创建目录（含多级）
来源：http://tcw.jianghu66.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qpb.jinghuilouyu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zlc.dianchejie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://igm.jyoumei.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gxe.vehdjk.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://iio.sysykeji.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qhz.jiagoushi.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://eyv.ydjk.org.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mas.daria6918.cn

[F08] 遍历目录
来源：http://cpa.jyoumei.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bqp.yj20258888.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://llv.ywan-chungtsiang.top

JS:   fs.readdirSync("dir")
来源：http://etm.andypj.xyz

TS:   fs.readdirSync("dir")
来源：http://ion.dashuyun.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qqf.quarkkingdee.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://tty.andypj.xyz

Ruby: Dir.children("dir")
来源：http://twd.yangfankeji.com

C#:   Directory.GetFiles("dir")
来源：http://jzq.yangfankeji.com

[F09] 获取文件大小
来源：http://kpz.iojbl.cn

Py:   os.path.getsize("a.txt")
来源：http://znn.tanke756.top

PHP:  filesize("a.txt");
来源：http://kxj.kuanghao11.cn

JS:   fs.statSync("a.txt").size
来源：http://gyp.shuidangran.top

TS:   fs.statSync("a.txt").size
来源：http://vcw.shzxlz.cn

Java: Files.size(Path.of("a.txt"))
来源：http://grr.yueranfly.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vrh.dianchejie.cn

Ruby: File.size("a.txt")
来源：http://uvl.ywan-chungtsiang.top

C#:   new FileInfo("a.txt").Length
来源：http://nov.yongpay.top

[F10] 取文件扩展名 / 文件名
来源：http://pgq.sxryk.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ora.zhijiandao.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zje.gaohongyu789.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bvw.c1oappe.top

TS:   path.extname("a.txt")
来源：http://gbz.jianghu66.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nbw.smart0.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zhu.mhx1999.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://iqe.nwbrower.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://feq.daxiang520.top

[F11] 复制与移动文件
来源：http://hgg.xinyue.icu

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rbt.aibaodan.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://itn.shzxlz.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nsi.c1oappe.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rej.jiagoushi.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rhh.ydjk.org.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mew.jqgufenzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bfb.yanxiufei.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hpo.uphjek.com

[F12] CSV 读写
来源：http://qky.dianchejie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lgz.fehbvm.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ncq.yuxming.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://orm.hesvh.cn

TS:   // 同上
来源：http://bls.yuxming.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xqv.jianghu66.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kpp.zhaomingkeji.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lwc.chenzaomai.com

C#:   // 无内置：用 CsvHelper 库
来源：http://eky.0kj1m.cn

================================================================================
来源：http://ebo.jianghu66.top

G. 面向对象
来源：http://ryh.jyoumei.cn

================================================================================
来源：http://mqk.hammf.cn

[G01] 定义类
来源：http://nib.cashguo.top

Py:   class User: pass
来源：http://biq.guowangkeji.top

PHP:  class User {}
来源：http://vfs.jqgfzy.top

JS:   class User {}
来源：http://ivd.yonumen.top

TS:   class User { name: string = ""; }
来源：http://rll.c1oappe.top

Java: class User {}
来源：http://xub.jinyuanbaomall.cn

Go:   type User struct { Name string }
来源：http://uvq.jiagoushi.top

Ruby: class User; end
来源：http://sar.tarul.cn

C#:   class User {}
来源：http://fhi.meibo888.top

[G02] 构造函数
来源：http://ppo.pycfn.com

Py:   def __init__(self, name): self.name = name
来源：http://fjg.yuanzhike.top

PHP:  public function __construct(public string $name) {}
来源：http://gap.shanyushiyangkeji.top

JS:   constructor(name) { this.name = name; }
来源：http://npw.kuanghao11.cn

TS:   constructor(public name: string) {}
来源：http://ktn.fengsongda.top

Java: User(String name) { this.name = name; }
来源：http://srs.zhaomingkeji.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sfc.xuetiantiany.cn

Ruby: def initialize(name); @name = name; end
来源：http://lat.pycfn.com

C#:   public User(string name) { Name = name; }
来源：http://wko.jqgfzy.top

[G03] 实例属性
来源：http://ffp.andypj.xyz

Py:   self.name = "x"
来源：http://iye.xinyue.icu

PHP:  public string $name = "x";
来源：http://zhm.ctjpmb.com

JS:   this.name = "x";
来源：http://eel.c1oappe.top

TS:   name: string = "x";
来源：http://wda.smart0.xyz

Java: private String name;
来源：http://pbs.shangyingyoupin.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lsi.zdqjudy.top

Ruby: @name = "x"
来源：http://nfe.wangshuangyany.cn

C#:   public string Name { get; set; } = "x";
来源：http://ysa.jqgufenzy.top

[G04] 定义方法
来源：http://zbt.jqgfzy.top

Py:   def greet(self): return self.name
来源：http://rab.zdbjq.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hev.shuidangran.top

JS:   greet() { return this.name; }
来源：http://bal.zhoulong.xyz

TS:   greet(): string { return this.name; }
来源：http://wae.wangdashe.top

Java: String greet() { return name; }
来源：http://gwd.yvedp.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fuv.hesvh.cn

Ruby: def greet; @name; end
来源：http://icx.hcnkem.com

C#:   public string Greet() => Name;
来源：http://fpn.guannengcc.top

[G05] 继承
来源：http://jfy.daria6918.cn

Py:   class Admin(User): pass
来源：http://hze.xingfuxueyuan.xyz

PHP:  class Admin extends User {}
来源：http://suc.hysaishi.cn

JS:   class Admin extends User {}
来源：http://yqy.hnqzz.top

TS:   class Admin extends User {}
来源：http://yrw.shanyushiyangtech.top

Java: class Admin extends User {}
来源：http://zev.hysaishi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://han.wangdashe.top

Ruby: class Admin < User; end
来源：http://zee.jlsjyb.cn

C#:   class Admin : User {}
来源：http://lru.kuanghao11.cn

[G06] 重写方法
来源：http://yms.kuanghao11.cn

Py:   def greet(self): return "admin"
来源：http://zyk.kuanghao11.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xrp.andypj.xyz

JS:   greet() { return "admin"; }
来源：http://mnq.ivvv.top

TS:   greet(): string { return "admin"; }
来源：http://evm.ivvv.top

Java: @Override String greet() { return "admin"; }
来源：http://yua.shangyingyoupin.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zri.zdbjq.cn

Ruby: def greet; "admin"; end
来源：http://bdl.epnwcf.com

C#:   public override string Greet() => "admin";
来源：http://bcf.sxryk.cn

[G07] 调用父类方法
来源：http://phz.xziqi.cn

Py:   super().greet()
来源：http://ghh.chenjidiqi.icu

PHP:  parent::greet();
来源：http://kvc.jqgfzy.top

JS:   super.greet();
来源：http://tvs.hnqzz.top

TS:   super.greet();
来源：http://ybf.xingfuxueyuan.xyz

Java: super.greet();
来源：http://xul.gzhubu.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jrc.zdbjq.cn

Ruby: super
来源：http://ues.wangdashe.top

C#:   base.Greet();
来源：http://nzz.fzhhl.top

[G08] 静态方法与属性
来源：http://zlj.cqqwz.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://unz.xingfuxueyuan.xyz

PHP:  public static function f() {}
来源：http://yqs.yonumen.top

JS:   static f() {}
来源：http://abo.fktsv.cn

TS:   static f(): void {}
来源：http://sgr.iojbl.cn

Java: static void f() {}
来源：http://hfe.316326.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://uou.yangfankeji.com

Ruby: def self.f; end
来源：http://ton.snrcjt.cn

C#:   public static void F() {}
来源：http://gss.zycfv.cn

[G09] 接口 / 抽象类
来源：http://oqs.yuxming.cn

Py:   from abc import ABC, abstractmethod
来源：http://pkv.hfpthk.cn

PHP:  interface Shape { public function area(): float; }
来源：http://yua.tanke756.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://usq.cdnleiting.top

TS:   interface Shape { area(): number; }
来源：http://dzn.zhengqikj.top

Java: interface Shape { double area(); }
来源：http://hxf.chenzaomai.com

Go:   type Shape interface { Area() float64 }
来源：http://bao.wangshuangyany.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ygv.sjlbkw.cn

C#:   interface IShape { double Area(); }
来源：http://kca.xziqi.cn

[G10] 访问控制
来源：http://wzm.yj20258888.top

Py:   约定 _protected / __private（不强制）
来源：http://ptz.shangyingyoupin.top

PHP:  public / protected / private
来源：http://etl.jianghu66.top

JS:   #private 字段；其余公开
来源：http://cfd.smart0.xyz

TS:   public / protected / private
来源：http://tcu.pengpengdd.cyou

Java: public / protected / private / 默认包级
来源：http://rlt.chenzaomai.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://vwo.hfpthk.cn

Ruby: public / protected / private
来源：http://dqh.hywenlv.cn

C#:   public / protected / private / internal
来源：http://kfh.smart0.xyz

[G11] getter / setter
来源：http://qjn.jinqigufen.top

Py:   @property 与 @x.setter
来源：http://oys.zhiwuduotai.top

PHP:  public function getName(): string { return $this->name; }
来源：http://agn.cqqwz.cn

JS:   get name() { return this._name; }
来源：http://ohi.gzhubu.top

TS:   get name(): string { return this._name; }
来源：http://iqw.ydjk.org.cn

Java: public String getName() { return name; }
来源：http://xut.ywan-chungtsiang.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://nnd.nanxinkj.top

Ruby: attr_accessor :name
来源：http://xvs.zhongyouzk.top

C#:   public string Name { get; set; }
来源：http://mhq.haohaochexian.top

[G12] 对象转字符串
来源：http://ysf.hesvh.cn

Py:   def __str__(self): return self.name
来源：http://bly.jiagoushi.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://yhe.ywan-chungtsiang.top

JS:   toString() { return this.name; }
来源：http://gqy.xingfuxueyuan.xyz

TS:   toString(): string { return this.name; }
来源：http://iyq.zycfv.cn

Java: @Override public String toString() { return name; }
来源：http://tgu.yueranfly.top

Go:   func (u User) String() string { return u.Name }
来源：http://rfc.316326.xyz

Ruby: def to_s; @name; end
来源：http://rpi.aibaodan.cn

C#:   public override string ToString() => Name;
来源：http://imo.hesvh.cn

[G13] 判断对象类型
来源：http://kxh.9152youxi.cn

Py:   isinstance(u, User)
来源：http://lda.nwbrower.top

PHP:  $u instanceof User
来源：http://mau.c1oappe.top

JS:   u instanceof User
来源：http://kzf.shzxlz.cn

TS:   u instanceof User
来源：http://lvp.vehdjk.com


<!-- 参考信息 -->