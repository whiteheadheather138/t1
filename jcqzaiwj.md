代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cdw.jianghu66.top

[E15] HTML 转义 / 反转义
来源：http://ojk.sweek.top

Py:   html.escape(s);  html.unescape(s)
来源：http://zsy.dianchejie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dee.cashguo.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wwh.iojbl.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://msr.havefunace.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qmr.haohaochexian.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uqg.quarkkingdee.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://oon.gaohongyu789.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://drz.yj202588.top

[E16] 数字千分位
来源：http://nzi.yj20258.top

Py:   f"{1234567:,}"
来源：http://qxw.quarkkingdee.top

PHP:  number_format(1234567);
来源：http://jfk.zhaomingkeji.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://npy.yvedp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://eqs.yangfankeji.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mqd.vehdjk.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sev.hesvh.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ojm.hnqzz.top

C#:   1234567.ToString("N0")
来源：http://uhl.ydjk.org.cn

[E17] 首字母大写
来源：http://vhp.yonumen.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rst.snrcjt.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://nji.sweek.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lpe.yuanzhike.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mzt.316326.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://grz.52xcode.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nat.daxiang520.top

Ruby: s.capitalize
来源：http://xkn.gogol.net.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lor.shangyingyoupin.top

[E18] 模板占位符替换
来源：http://fvu.hcnkem.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ybz.jinyuanbaomall.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yqc.hnxiangtu.top

JS:   tpl.replaceAll("{name}", name)
来源：http://mjl.vehdjk.com

TS:   tpl.replaceAll("{name}", name)
来源：http://ozq.gzhubu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zcw.cdnleiting.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://edk.yonumen.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hmi.nwbrower.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://soo.ehwqpu.com

[E19] 多行文本按行拆分
来源：http://kro.zdbjq.cn

Py:   s.splitlines()
来源：http://hpg.jlsjyb.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ybr.dashuyun.cn

JS:   s.split(/\r?\n/)
来源：http://hyw.zhoulong.xyz

TS:   s.split(/\r?\n/)
来源：http://wdo.vqdsnc.cn

Java: s.lines().toList()
来源：http://shd.yj202588.top

Go:   strings.Split(s, "\n")
来源：http://wmq.cqqwz.cn

Ruby: s.lines
来源：http://hbs.ppjwa.cn

C#:   s.Split('\n')
来源：http://xjn.dashuyun.cn

[E20] 判断字符串是否为空
来源：http://wuq.guowangkeji.top

Py:   if not s:
来源：http://pun.sweek.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ngk.hesvh.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lno.daria6918.cn

TS:   if (s === "") {}
来源：http://jqi.pycfn.com

Java: if (s.isEmpty()) {}
来源：http://xar.xuanzx.com

Go:   if s == "" {}
来源：http://vaq.kuanghao11.cn

Ruby: if s.empty?
来源：http://xeb.yvedp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://csa.iojbl.cn

[E21] 超长截断加省略号
来源：http://zzm.pengpengdd.cyou

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://coo.zhiwuduotai.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gqz.yonumen.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zxu.gogol.net.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vkj.uphjek.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mfy.ywan-chungtsiang.top

Go:   // 按 rune 判断长度后截断
来源：http://pbd.snrcjt.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://puv.hammf.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ofs.tanke756.top

[E22] 字节长度与字符长度
来源：http://gik.fehbvm.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wjc.zycfv.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wwe.aizwys.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zql.zdqjudy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mnj.smart0.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lzd.zhoulong.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uay.wangshuangyany.cn

Ruby: s.bytesize;  s.length
来源：http://dst.chenlongwang.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ulo.mhx1999.top

================================================================================
来源：http://wsm.tianlin.xyz

F. 文件与目录
来源：http://qij.52xcode.cn

================================================================================
来源：http://uop.pengpengdd.cyou

[F01] 读取整个文件
来源：http://nqe.sweek.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://smo.hfpthk.cn

PHP:  file_get_contents("a.txt");
来源：http://onw.cheryme.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nbk.pengpengdd.cyou

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rdz.nwbrower.top

Java: Files.readString(Path.of("a.txt"))
来源：http://pno.svipenyu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lmx.yueranfly.top

Ruby: File.read("a.txt")
来源：http://gek.chenjidiqi.icu

C#:   File.ReadAllText("a.txt");
来源：http://jah.epnwcf.com

[F02] 逐行读取文件
来源：http://qko.sweek.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://obf.vehdjk.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ejn.nanxuanxn.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lrl.cucudq.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mnn.hammf.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://esb.jianghu66.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fhf.havefunace.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ohm.jinghuilouyu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://weg.yuxming.cn

[F03] 写入文件（覆盖）
来源：http://icg.9152youxi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gko.nwbrower.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://jqk.birdmap.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rve.9152youxi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vxz.hysaishi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://umc.jinqigufen.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zkd.ywan-chungtsiang.top

Ruby: File.write("a.txt", "hi")
来源：http://gpv.nanxinkj.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vfc.zdqjudy.top

[F04] 追加写入文件
来源：http://rxn.xuanzx.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tfj.hesvh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lqk.aibaodan.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uwp.yongpay.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zpe.ydzc1.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tkx.ppjwa.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vfo.xylfe.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sfs.xuetiantiany.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jyc.pycfn.com

[F05] 判断文件或目录是否存在
来源：http://dma.jlsjyb.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jzg.zhijiandao.cn

PHP:  file_exists("a.txt");
来源：http://bsj.aibaodan.cn

JS:   fs.existsSync("a.txt")
来源：http://mkg.andypj.xyz

TS:   fs.existsSync("a.txt")
来源：http://lvs.nwbrower.top

Java: Files.exists(Path.of("a.txt"))
来源：http://vpx.zdqjudy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ibc.aibaodan.cn

Ruby: File.exist?("a.txt")
来源：http://gyo.hfpthk.cn

C#:   File.Exists("a.txt")
来源：http://rft.xylfe.cn

[F06] 删除文件
来源：http://qum.jqgufenzy.top

Py:   os.remove("a.txt")
来源：http://zce.tianlin.xyz

PHP:  unlink("a.txt");
来源：http://jex.yvedp.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ptt.jqgufenzy.top

TS:   fs.unlinkSync("a.txt")
来源：http://ehz.aizwys.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gqh.aizwys.cn

Go:   os.Remove("a.txt")
来源：http://pwm.xylfe.cn

Ruby: File.delete("a.txt")
来源：http://got.jinghuilouyu.cn

C#:   File.Delete("a.txt");
来源：http://pyx.cashguo.top

[F07] 创建目录（含多级）
来源：http://yzs.epnwcf.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ssm.aizwys.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://osd.chenlongwang.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zka.jinqigufen.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zum.uphjek.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gdf.yanxiufei.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gjr.sufxvd.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gwh.feifeiyinyue.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mgg.fehbvm.com

[F08] 遍历目录
来源：http://khv.zdqjudy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://qiw.sjlbkw.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vji.sysykeji.top

JS:   fs.readdirSync("dir")
来源：http://aem.ctjpmb.com

TS:   fs.readdirSync("dir")
来源：http://rgo.yvedp.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qtu.yfazqb.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://lnn.nanxinkj.top

Ruby: Dir.children("dir")
来源：http://zra.daria6918.cn

C#:   Directory.GetFiles("dir")
来源：http://ukl.iojbl.cn

[F09] 获取文件大小
来源：http://hhc.feifeiyinyue.top

Py:   os.path.getsize("a.txt")
来源：http://gvi.redwolf501.top

PHP:  filesize("a.txt");
来源：http://xeg.dianchejie.cn

JS:   fs.statSync("a.txt").size
来源：http://xbl.kuanghao11.cn

TS:   fs.statSync("a.txt").size
来源：http://trx.ybcxt.top

Java: Files.size(Path.of("a.txt"))
来源：http://fsu.hnxiangtu.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lca.ybcxt.top

Ruby: File.size("a.txt")
来源：http://qvg.sxryk.cn

C#:   new FileInfo("a.txt").Length
来源：http://ams.yj20258888.top

[F10] 取文件扩展名 / 文件名
来源：http://piy.hammf.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ckc.tarul.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cgs.epnwcf.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://riu.xingfuxueyuan.xyz

TS:   path.extname("a.txt")
来源：http://wld.zhengqikj.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wxg.iojbl.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pbn.jinyuanbaomall.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nye.xziqi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nwu.wangdashe.top

[F11] 复制与移动文件
来源：http://sol.bjfxy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mky.yj20258888.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xdm.epnwcf.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cug.wangshuangyany.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wjl.jianghu66.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dpv.uphjek.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xoy.guannengcc.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ggp.redwolf501.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://idm.tian-w.cn

[F12] CSV 读写
来源：http://sjz.zhengqikj.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pgp.xingfuxueyuan.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xvj.wangshuangyany.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xza.havefunace.top

TS:   // 同上
来源：http://lrq.xylfe.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wsr.wangdashe.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dpc.redwolf501.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dik.gotoacloud.top

C#:   // 无内置：用 CsvHelper 库
来源：http://zbt.chenlongwang.top

================================================================================
来源：http://sui.zdqjudy.top

G. 面向对象
来源：http://gej.vqdsnc.cn

================================================================================
来源：http://ktx.nwbrower.top

[G01] 定义类
来源：http://viq.jiagoushi.top

Py:   class User: pass
来源：http://mxo.quarkkingdee.top

PHP:  class User {}
来源：http://bdj.wangshuangyany.cn

JS:   class User {}
来源：http://ufx.cheryme.top

TS:   class User { name: string = ""; }
来源：http://deg.jyoumei.cn

Java: class User {}
来源：http://ydx.sysykeji.top

Go:   type User struct { Name string }
来源：http://xch.gogol.net.cn

Ruby: class User; end
来源：http://mmf.tian-w.cn

C#:   class User {}
来源：http://typ.sufxvd.cn

[G02] 构造函数
来源：http://xuf.sufxvd.cn

Py:   def __init__(self, name): self.name = name
来源：http://tvf.svipenyu.cn

PHP:  public function __construct(public string $name) {}
来源：http://hnw.hysaishi.cn

JS:   constructor(name) { this.name = name; }
来源：http://zhy.yangfankeji.com

TS:   constructor(public name: string) {}
来源：http://twu.cdnleiting.top

Java: User(String name) { this.name = name; }
来源：http://fma.shangyingyoupin.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tid.zhengqikj.top

Ruby: def initialize(name); @name = name; end
来源：http://klg.zdbjq.cn

C#:   public User(string name) { Name = name; }
来源：http://ceo.zhijiandao.cn

[G03] 实例属性
来源：http://ods.zhaomingkeji.xyz

Py:   self.name = "x"
来源：http://xpl.haohaochexian.top

PHP:  public string $name = "x";
来源：http://dmj.zhaomingkeji.xyz

JS:   this.name = "x";
来源：http://pwk.yueranfly.top

TS:   name: string = "x";
来源：http://dmz.pycfn.com

Java: private String name;
来源：http://kbx.c1oappe.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kaw.yongpay.top

Ruby: @name = "x"
来源：http://eoy.tanke756.top

C#:   public string Name { get; set; } = "x";
来源：http://jon.yangfankeji.com

[G04] 定义方法
来源：http://ilz.hfpthk.cn

Py:   def greet(self): return self.name
来源：http://ked.haohaochexian.top

PHP:  public function greet(): string { return $this->name; }
来源：http://mrg.hammf.cn

JS:   greet() { return this.name; }
来源：http://qxc.sufxvd.cn

TS:   greet(): string { return this.name; }
来源：http://kpl.aibaodan.cn

Java: String greet() { return name; }
来源：http://kjh.yueranfly.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://hug.xuetiantiany.cn

Ruby: def greet; @name; end
来源：http://mll.pengpengdd.cyou

C#:   public string Greet() => Name;
来源：http://ncw.yanxiufei.cn

[G05] 继承
来源：http://zoz.zdbjq.cn

Py:   class Admin(User): pass
来源：http://pdy.xylfe.cn

PHP:  class Admin extends User {}
来源：http://fpv.zhiwuduotai.top

JS:   class Admin extends User {}
来源：http://zge.zdqjudy.top

TS:   class Admin extends User {}
来源：http://gpt.dashuyun.cn

Java: class Admin extends User {}
来源：http://olg.cashguo.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qxy.hnxiangtu.top

Ruby: class Admin < User; end
来源：http://egm.yongpay.top

C#:   class Admin : User {}
来源：http://sth.ybcxt.top

[G06] 重写方法
来源：http://hov.xziqi.cn

Py:   def greet(self): return "admin"
来源：http://wsc.quarkkingdee.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ixx.cucudq.cn

JS:   greet() { return "admin"; }
来源：http://xjx.c1oappe.top

TS:   greet(): string { return "admin"; }
来源：http://raw.quarkkingdee.top

Java: @Override String greet() { return "admin"; }
来源：http://fas.svipenyu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wpl.fehbvm.com

Ruby: def greet; "admin"; end
来源：http://umo.jinqigufen.top

C#:   public override string Greet() => "admin";
来源：http://mvq.sxryk.cn

[G07] 调用父类方法
来源：http://wpy.fehbvm.com

Py:   super().greet()
来源：http://twt.0kj1m.cn

PHP:  parent::greet();
来源：http://fbs.kuanghao11.cn

JS:   super.greet();
来源：http://bbw.sysykeji.top

TS:   super.greet();
来源：http://qbq.iojbl.cn

Java: super.greet();
来源：http://tnf.wangdashe.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sdx.birdmap.top

Ruby: super
来源：http://khc.daxiang520.top

C#:   base.Greet();
来源：http://bpx.xylfe.cn

[G08] 静态方法与属性
来源：http://ydr.shangyingyoupin.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://oxs.redwolf501.top

PHP:  public static function f() {}
来源：http://vjs.dianchejie.cn

JS:   static f() {}
来源：http://muz.gogol.net.cn

TS:   static f(): void {}
来源：http://rhw.uphjek.com

Java: static void f() {}
来源：http://sno.gotoacloud.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://emi.epnwcf.com

Ruby: def self.f; end
来源：http://zak.aibaodan.cn

C#:   public static void F() {}
来源：http://kin.ybcxt.top

[G09] 接口 / 抽象类
来源：http://aki.feifeiyinyue.top

Py:   from abc import ABC, abstractmethod
来源：http://kzo.vqdsnc.cn

PHP:  interface Shape { public function area(): float; }
来源：http://lhh.fehbvm.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://vwp.guannengcc.top

TS:   interface Shape { area(): number; }
来源：http://igx.yfazqb.com

Java: interface Shape { double area(); }
来源：http://tyg.chenjidiqi.icu

Go:   type Shape interface { Area() float64 }
来源：http://cnk.gogol.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ssm.jiagoushi.top

C#:   interface IShape { double Area(); }
来源：http://gmi.fengsongda.top

[G10] 访问控制
来源：http://btu.andypj.xyz

Py:   约定 _protected / __private（不强制）
来源：http://deh.jiagoushi.top

PHP:  public / protected / private
来源：http://jam.sjlbkw.cn

JS:   #private 字段；其余公开
来源：http://jhu.ydzc1.top

TS:   public / protected / private
来源：http://fyo.tianlin.xyz

Java: public / protected / private / 默认包级
来源：http://vba.birdmap.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://akh.tian-w.cn

Ruby: public / protected / private
来源：http://vll.uphjek.com

C#:   public / protected / private / internal
来源：http://haz.bbcook.cn

[G11] getter / setter
来源：http://gyu.jyoumei.cn

Py:   @property 与 @x.setter
来源：http://rbs.hysaishi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://rnn.xuanzx.com

JS:   get name() { return this._name; }
来源：http://dor.zhijiandao.cn

TS:   get name(): string { return this._name; }
来源：http://ttt.aibaodan.cn

Java: public String getName() { return name; }
来源：http://veq.fktsv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vqq.feifeiyinyue.top

Ruby: attr_accessor :name
来源：http://sct.pycfn.com

C#:   public string Name { get; set; }
来源：http://dqj.bbcook.cn

[G12] 对象转字符串
来源：http://cig.wangshuangyany.cn

Py:   def __str__(self): return self.name
来源：http://sxr.pycfn.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://efb.bjfxy.top

JS:   toString() { return this.name; }
来源：http://rva.meibo888.top

TS:   toString(): string { return this.name; }
来源：http://nfr.hfpthk.cn

Java: @Override public String toString() { return name; }
来源：http://twt.zhiwuduotai.top

Go:   func (u User) String() string { return u.Name }
来源：http://qqv.chenjidiqi.icu

Ruby: def to_s; @name; end
来源：http://dct.tianlin.xyz

C#:   public override string ToString() => Name;
来源：http://bwo.cashguo.top

[G13] 判断对象类型
来源：http://dzy.sweek.top

Py:   isinstance(u, User)
来源：http://opl.sxryk.cn

PHP:  $u instanceof User
来源：http://qzk.xuetiantiany.cn

JS:   u instanceof User
来源：http://ien.ybcxt.top

TS:   u instanceof User
来源：http://get.birdmap.top


<!-- 参考信息 -->