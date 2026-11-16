代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cpe.jqgfzy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gof.sysykeji.top

[E16] 数字千分位
来源：http://ncs.quarkkingdee.top

Py:   f"{1234567:,}"
来源：http://isb.xuanzx.com

PHP:  number_format(1234567);
来源：http://bbn.pycfn.com

JS:   (1234567).toLocaleString("en-US")
来源：http://ekj.chenlongwang.top

TS:   (1234567).toLocaleString("en-US")
来源：http://bwm.sweek.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ach.vehdjk.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wxe.yj202588.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://szu.vqdsnc.cn

C#:   1234567.ToString("N0")
来源：http://pfk.zhiwuduotai.top

[E17] 首字母大写
来源：http://svg.vqdsnc.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://olr.fengsongda.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://dqs.hesvh.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hla.zhiwuduotai.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gwp.andypj.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fxh.daxiang520.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nsw.birdmap.top

Ruby: s.capitalize
来源：http://zga.xinyue.icu

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://off.epnwcf.com

[E18] 模板占位符替换
来源：http://gim.sjlbkw.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qff.gzhubu.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vtm.jianghu66.top

JS:   tpl.replaceAll("{name}", name)
来源：http://osu.yongpay.top

TS:   tpl.replaceAll("{name}", name)
来源：http://evz.ehwqpu.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ppo.zhiwuduotai.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ktx.zhiwuduotai.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://avy.jinqigufen.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lzh.feifeiyinyue.top

[E19] 多行文本按行拆分
来源：http://egd.nwbrower.top

Py:   s.splitlines()
来源：http://bgd.bbcook.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lxb.uphjek.com

JS:   s.split(/\r?\n/)
来源：http://ory.sweek.top

TS:   s.split(/\r?\n/)
来源：http://xhy.vqdsnc.cn

Java: s.lines().toList()
来源：http://nyr.gogol.net.cn

Go:   strings.Split(s, "\n")
来源：http://qha.jyoumei.cn

Ruby: s.lines
来源：http://lvz.ctjpmb.com

C#:   s.Split('\n')
来源：http://usu.wangdashe.top

[E20] 判断字符串是否为空
来源：http://urk.yj20258.top

Py:   if not s:
来源：http://cnj.chenzaomai.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rhj.yuanzhike.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://amg.zhixingplan.top

TS:   if (s === "") {}
来源：http://gej.zhaomingkeji.xyz

Java: if (s.isEmpty()) {}
来源：http://frt.fktsv.cn

Go:   if s == "" {}
来源：http://jjw.zycfv.cn

Ruby: if s.empty?
来源：http://zsl.ehwqpu.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wdm.jinghuilouyu.cn

[E21] 超长截断加省略号
来源：http://vjk.c1oappe.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ksl.zhongyouzk.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hzd.ehwqpu.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://reo.zdqjudy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mvk.kuanghao11.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vuc.yuanzhike.top

Go:   // 按 rune 判断长度后截断
来源：http://yfs.daxiang520.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lgt.jinqigufen.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://acv.fanxiaobao.xyz

[E22] 字节长度与字符长度
来源：http://idr.jqgfzy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hwv.sjlbkw.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gkx.vehdjk.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wdf.316326.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://amv.316326.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gjm.ybcxt.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cqe.chenzaomai.com

Ruby: s.bytesize;  s.length
来源：http://ujc.daxiang520.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qfb.zdbjq.cn

================================================================================
来源：http://pel.zdqjudy.top

F. 文件与目录
来源：http://fod.gzhubu.top

================================================================================
来源：http://eqe.yonumen.top

[F01] 读取整个文件
来源：http://rjc.gaohongyu789.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fxi.zhiwuduotai.top

PHP:  file_get_contents("a.txt");
来源：http://hwu.yonumen.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fpp.zhijiandao.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pwt.kuanghao11.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://cps.guowangkeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zft.chenjidiqi.icu

Ruby: File.read("a.txt")
来源：http://zrq.xinyue.icu

C#:   File.ReadAllText("a.txt");
来源：http://cjm.chenlongwang.top

[F02] 逐行读取文件
来源：http://kyk.yueranfly.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mjt.zhaomingkeji.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gxr.fehbvm.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qbg.haohaochexian.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://apq.bjfxy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://skd.gogol.net.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wsv.bjfxy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wun.shzxlz.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vhy.jinqigufen.top

[F03] 写入文件（覆盖）
来源：http://bri.shanyushiyangkeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dly.haohaochexian.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://isr.cucudq.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hfs.yongpay.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qdc.nwbrower.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cag.feifeiyinyue.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://isn.sysykeji.top

Ruby: File.write("a.txt", "hi")
来源：http://hsg.cashguo.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pns.zdqjudy.top

[F04] 追加写入文件
来源：http://gvq.gzhubu.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lup.zdqjudy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xsd.yanxiufei.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rod.shanyushiyangkeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ykf.hammf.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dvq.hcnkem.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://muf.jqgufenzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nkd.tianlin.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qgp.shzxlz.cn

[F05] 判断文件或目录是否存在
来源：http://ocj.shangyingyoupin.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jhz.zhaomingkeji.xyz

PHP:  file_exists("a.txt");
来源：http://ztl.cqqwz.cn

JS:   fs.existsSync("a.txt")
来源：http://dhg.zhongyouzk.top

TS:   fs.existsSync("a.txt")
来源：http://skw.fengsongda.top

Java: Files.exists(Path.of("a.txt"))
来源：http://pyd.hammf.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fxj.ivvv.top

Ruby: File.exist?("a.txt")
来源：http://jqo.chenzaomai.com

C#:   File.Exists("a.txt")
来源：http://vly.hcnkem.com

[F06] 删除文件
来源：http://voe.cdnleiting.top

Py:   os.remove("a.txt")
来源：http://zna.sjlbkw.cn

PHP:  unlink("a.txt");
来源：http://rah.wangdashe.top

JS:   fs.unlinkSync("a.txt")
来源：http://txk.wangshuangyany.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vfs.jyoumei.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mtj.hysaishi.cn

Go:   os.Remove("a.txt")
来源：http://ylw.pycfn.com

Ruby: File.delete("a.txt")
来源：http://weo.yanxiufei.cn

C#:   File.Delete("a.txt");
来源：http://tjd.fanxiaobao.xyz

[F07] 创建目录（含多级）
来源：http://klh.zhaomingkeji.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zft.gaohongyu789.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jwj.yfazqb.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fgi.xinyue.icu

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vka.hywenlv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cge.ywan-chungtsiang.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xrm.bjfxy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qoz.gotoacloud.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cca.jianghu66.top

[F08] 遍历目录
来源：http://ocu.shanyushiyangkeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://tsf.wangdashe.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lds.haohaochexian.top

JS:   fs.readdirSync("dir")
来源：http://hcm.yj202588.top

TS:   fs.readdirSync("dir")
来源：http://umc.nanxinkj.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://abp.cashguo.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://gjy.cdnleiting.top

Ruby: Dir.children("dir")
来源：http://fmn.smart0.xyz

C#:   Directory.GetFiles("dir")
来源：http://ctw.meibo888.top

[F09] 获取文件大小
来源：http://jyk.cucudq.cn

Py:   os.path.getsize("a.txt")
来源：http://ogv.ppjwa.cn

PHP:  filesize("a.txt");
来源：http://iko.wangshuangyany.cn

JS:   fs.statSync("a.txt").size
来源：http://wkx.zhengqikj.top

TS:   fs.statSync("a.txt").size
来源：http://qqg.uphjek.com

Java: Files.size(Path.of("a.txt"))
来源：http://rbm.hywenlv.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jnv.yfazqb.com

Ruby: File.size("a.txt")
来源：http://hhk.jyoumei.cn

C#:   new FileInfo("a.txt").Length
来源：http://zqb.zhongyouzk.top

[F10] 取文件扩展名 / 文件名
来源：http://son.iojbl.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zsn.mhx1999.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wlq.yuanzhike.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://npj.sjlbkw.cn

TS:   path.extname("a.txt")
来源：http://wau.fktsv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://txc.yanxiufei.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uei.ybcxt.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ilw.yuanzhike.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qbd.yj20258.top

[F11] 复制与移动文件
来源：http://mku.jinqigfzy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://inm.aizwys.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dwn.shangyingyoupin.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vuh.jqgfzy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bof.yanxiufei.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gvc.zdbjq.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fxo.gzhubu.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yfl.hnqzz.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dgt.guannengcc.top

[F12] CSV 读写
来源：http://gxv.shangyingyoupin.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://var.ydzc1.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wkc.jyoumei.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hiv.hfpthk.cn

TS:   // 同上
来源：http://upa.aizwys.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baa.pycfn.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cwj.jinyuanbaomall.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kml.shuidangran.top

C#:   // 无内置：用 CsvHelper 库
来源：http://pno.daria6918.cn

================================================================================
来源：http://qyc.birdmap.top

G. 面向对象
来源：http://dpa.ctjpmb.com

================================================================================
来源：http://ojb.yj202588.top

[G01] 定义类
来源：http://vur.haohaochexian.top

Py:   class User: pass
来源：http://qyt.zhongyouzk.top

PHP:  class User {}
来源：http://wkq.zhongyouzk.top

JS:   class User {}
来源：http://jyj.bjfxy.top

TS:   class User { name: string = ""; }
来源：http://ugq.ydjk.org.cn

Java: class User {}
来源：http://vdv.hnxiangtu.top

Go:   type User struct { Name string }
来源：http://hwr.zhijiandao.cn

Ruby: class User; end
来源：http://agv.wangdashe.top

C#:   class User {}
来源：http://wmw.redwolf501.top

[G02] 构造函数
来源：http://jzk.gogol.net.cn

Py:   def __init__(self, name): self.name = name
来源：http://kec.fzhhl.top

PHP:  public function __construct(public string $name) {}
来源：http://err.52xcode.cn

JS:   constructor(name) { this.name = name; }
来源：http://ybt.yongpay.top

TS:   constructor(public name: string) {}
来源：http://jyk.yj202588.top

Java: User(String name) { this.name = name; }
来源：http://gkz.zhijiandao.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rnc.feifeiyinyue.top

Ruby: def initialize(name); @name = name; end
来源：http://ulm.hnqzz.top

C#:   public User(string name) { Name = name; }
来源：http://obs.jinghuilouyu.cn

[G03] 实例属性
来源：http://nhp.guowangkeji.top

Py:   self.name = "x"
来源：http://vha.ydjk.org.cn

PHP:  public string $name = "x";
来源：http://qdk.zycfv.cn

JS:   this.name = "x";
来源：http://wve.guowangkeji.top

TS:   name: string = "x";
来源：http://giw.zdqjudy.top

Java: private String name;
来源：http://xqh.tianlin.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://axh.jinyuanbaomall.cn

Ruby: @name = "x"
来源：http://ibb.nwbrower.top

C#:   public string Name { get; set; } = "x";
来源：http://xgn.hammf.cn

[G04] 定义方法
来源：http://ljw.dianchejie.cn

Py:   def greet(self): return self.name
来源：http://rfr.guannengcc.top

PHP:  public function greet(): string { return $this->name; }
来源：http://jia.hywenlv.cn

JS:   greet() { return this.name; }
来源：http://uxe.jyoumei.cn

TS:   greet(): string { return this.name; }
来源：http://dwh.tian-w.cn

Java: String greet() { return name; }
来源：http://onw.pengpengdd.cyou

Go:   func (u User) Greet() string { return u.Name }
来源：http://ktq.jinyuanbaomall.cn

Ruby: def greet; @name; end
来源：http://zxg.sjlbkw.cn

C#:   public string Greet() => Name;
来源：http://cqg.sweek.top

[G05] 继承
来源：http://tsh.jyoumei.cn

Py:   class Admin(User): pass
来源：http://rxo.cheryme.top

PHP:  class Admin extends User {}
来源：http://dse.zycfv.cn

JS:   class Admin extends User {}
来源：http://xhi.ywan-chungtsiang.top

TS:   class Admin extends User {}
来源：http://szd.pengpengdd.cyou

Java: class Admin extends User {}
来源：http://jgt.chenzaomai.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kxw.epnwcf.com

Ruby: class Admin < User; end
来源：http://cbu.cheryme.top

C#:   class Admin : User {}
来源：http://bep.epnwcf.com

[G06] 重写方法
来源：http://zgy.shanyushiyangkeji.top

Py:   def greet(self): return "admin"
来源：http://pmx.yangfankeji.com

PHP:  public function greet(): string { return "admin"; }
来源：http://rji.zhijiandao.cn

JS:   greet() { return "admin"; }
来源：http://yjr.yongpay.top

TS:   greet(): string { return "admin"; }
来源：http://hgu.zhijiandao.cn

Java: @Override String greet() { return "admin"; }
来源：http://htw.hfpthk.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://csv.wangdashe.top

Ruby: def greet; "admin"; end
来源：http://aaw.tanke756.top

C#:   public override string Greet() => "admin";
来源：http://qgn.pycfn.com

[G07] 调用父类方法
来源：http://fse.shanyushiyangtech.top

Py:   super().greet()
来源：http://ijk.yongpay.top

PHP:  parent::greet();
来源：http://gku.nwbrower.top

JS:   super.greet();
来源：http://obd.ppjwa.cn

TS:   super.greet();
来源：http://asz.yuanzhike.top

Java: super.greet();
来源：http://kis.cashguo.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://olt.jqgufenzy.top

Ruby: super
来源：http://mrt.gaohongyu789.top

C#:   base.Greet();
来源：http://ymf.fktsv.cn

[G08] 静态方法与属性
来源：http://ftu.jqgfzy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fmk.fehbvm.com

PHP:  public static function f() {}
来源：http://shf.iojbl.cn

JS:   static f() {}
来源：http://inn.gotoacloud.top

TS:   static f(): void {}
来源：http://fak.yj202588.top

Java: static void f() {}
来源：http://uex.zycfv.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ikl.epnwcf.com

Ruby: def self.f; end
来源：http://fif.fktsv.cn

C#:   public static void F() {}
来源：http://cdh.nwbrower.top

[G09] 接口 / 抽象类
来源：http://xac.cucudq.cn

Py:   from abc import ABC, abstractmethod
来源：http://ppi.snrcjt.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zes.xuetiantiany.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xqy.sxryk.cn

TS:   interface Shape { area(): number; }
来源：http://pfk.pycfn.com

Java: interface Shape { double area(); }
来源：http://jei.xuetiantiany.cn

Go:   type Shape interface { Area() float64 }
来源：http://lyt.yanxiufei.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xgd.gogol.net.cn

C#:   interface IShape { double Area(); }
来源：http://afo.hfpthk.cn

[G10] 访问控制
来源：http://fxs.svipenyu.cn

Py:   约定 _protected / __private（不强制）
来源：http://jeq.shanyushiyangkeji.top

PHP:  public / protected / private
来源：http://xkv.zhixingplan.top

JS:   #private 字段；其余公开
来源：http://ddy.andypj.xyz

TS:   public / protected / private
来源：http://mwb.ywan-chungtsiang.top

Java: public / protected / private / 默认包级
来源：http://dmu.gzhubu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://vzj.haohaochexian.top

Ruby: public / protected / private
来源：http://xve.yonumen.top

C#:   public / protected / private / internal
来源：http://tqj.shanyushiyangkeji.top

[G11] getter / setter
来源：http://ang.hnqzz.top

Py:   @property 与 @x.setter
来源：http://zpe.cashguo.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ktm.sysykeji.top

JS:   get name() { return this._name; }
来源：http://cpt.snrcjt.cn

TS:   get name(): string { return this._name; }
来源：http://ejt.zhongyouzk.top

Java: public String getName() { return name; }
来源：http://kqm.smart0.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://hkf.svipenyu.cn

Ruby: attr_accessor :name
来源：http://lco.nanxinkj.top

C#:   public string Name { get; set; }
来源：http://ypw.pengpengdd.cyou

[G12] 对象转字符串
来源：http://xye.wangshuangyany.cn

Py:   def __str__(self): return self.name
来源：http://jrh.ydzc1.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://vyv.bbcook.cn

JS:   toString() { return this.name; }
来源：http://qjz.xingfuxueyuan.xyz

TS:   toString(): string { return this.name; }
来源：http://awb.cashguo.top

Java: @Override public String toString() { return name; }
来源：http://kkp.bbcook.cn

Go:   func (u User) String() string { return u.Name }
来源：http://sgy.zycfv.cn

Ruby: def to_s; @name; end
来源：http://ojx.yj20258888.top

C#:   public override string ToString() => Name;
来源：http://eld.cashguo.top

[G13] 判断对象类型
来源：http://mbi.jinyuanbaomall.cn

Py:   isinstance(u, User)
来源：http://thw.andypj.xyz

PHP:  $u instanceof User
来源：http://ltv.kuanghao11.cn

JS:   u instanceof User
来源：http://ust.yanxiufei.cn

TS:   u instanceof User
来源：http://tvq.quarkkingdee.top

Java: u instanceof User
来源：http://qpd.fehbvm.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://isj.fzhhl.top

Ruby: u.is_a?(User)
来源：http://tky.xinyue.icu

C#:   u is User
来源：http://iak.guannengcc.top

[G14] 数据类 / record
来源：http://ndh.shangyingyoupin.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://aqw.0kj1m.cn

PHP:  // 用 readonly 属性模拟
来源：http://ybw.sweek.top

JS:   // 无内置：普通类或对象字面量
来源：http://hgw.hnqzz.top


<!-- 参考信息 -->