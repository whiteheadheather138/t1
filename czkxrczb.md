代发 wailian999

PHP:  number_format(1234567);
来源：http://yfz.shanyushiyangkeji.top

JS:   (1234567).toLocaleString("en-US")
来源：http://njs.hesvh.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hax.feifeiyinyue.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yzd.wangdashe.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://iup.hcnkem.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://liq.wangshuangyany.cn

C#:   1234567.ToString("N0")
来源：http://xlm.vqdsnc.cn

[E17] 首字母大写
来源：http://qwo.vqdsnc.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://icr.sjlbkw.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hrb.jqgfzy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oyq.xingfuxueyuan.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zak.cheryme.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jah.xingfuxueyuan.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qak.aizwys.cn

Ruby: s.capitalize
来源：http://dnz.ctjpmb.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zyu.hnxiangtu.top

[E18] 模板占位符替换
来源：http://mti.fzhhl.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mub.nwbrower.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://doc.uphjek.com

JS:   tpl.replaceAll("{name}", name)
来源：http://nfi.ydjk.org.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://xsz.shanyushiyangkeji.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://exq.hnqzz.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bho.zhongyouzk.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://stz.hesvh.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qhd.daxiang520.top

[E19] 多行文本按行拆分
来源：http://too.yuanzhike.top

Py:   s.splitlines()
来源：http://dnb.hammf.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ktu.sysykeji.top

JS:   s.split(/\r?\n/)
来源：http://mpk.fktsv.cn

TS:   s.split(/\r?\n/)
来源：http://fzu.bjfxy.top

Java: s.lines().toList()
来源：http://ilz.quarkkingdee.top

Go:   strings.Split(s, "\n")
来源：http://mzh.zhoulong.xyz

Ruby: s.lines
来源：http://zkd.xylfe.cn

C#:   s.Split('\n')
来源：http://iga.wangshuangyany.cn

[E20] 判断字符串是否为空
来源：http://jkr.cheryme.top

Py:   if not s:
来源：http://pac.tian-w.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rwl.zhengqikj.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gcx.cucudq.cn

TS:   if (s === "") {}
来源：http://gik.fehbvm.com

Java: if (s.isEmpty()) {}
来源：http://xhn.pycfn.com

Go:   if s == "" {}
来源：http://izf.xingfuxueyuan.xyz

Ruby: if s.empty?
来源：http://lrm.yongpay.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://oee.dianchejie.cn

[E21] 超长截断加省略号
来源：http://hfz.aizwys.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sfd.sjlbkw.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kao.xylfe.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tsi.yonumen.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://byo.jqgfzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://def.daxiang520.top

Go:   // 按 rune 判断长度后截断
来源：http://gxt.hesvh.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://otm.daxiang520.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xyk.zdqjudy.top

[E22] 字节长度与字符长度
来源：http://pkj.jqgufenzy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wzg.gotoacloud.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ttn.cdnleiting.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wga.zdbjq.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xwz.gogol.net.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kek.fehbvm.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kft.daxiang520.top

Ruby: s.bytesize;  s.length
来源：http://bfs.yuxming.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bna.jiagoushi.top

================================================================================
来源：http://yiw.smart0.xyz

F. 文件与目录
来源：http://jgo.hywenlv.cn

================================================================================
来源：http://amg.yueranfly.top

[F01] 读取整个文件
来源：http://ymh.yanxiufei.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kwb.tian-w.cn

PHP:  file_get_contents("a.txt");
来源：http://pxy.hnqzz.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nlb.ivvv.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wkx.shanyushiyangtech.top

Java: Files.readString(Path.of("a.txt"))
来源：http://iev.ydzc1.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tzr.nwbrower.top

Ruby: File.read("a.txt")
来源：http://jrc.daria6918.cn

C#:   File.ReadAllText("a.txt");
来源：http://nqr.shuidangran.top

[F02] 逐行读取文件
来源：http://bbs.sweek.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cew.52xcode.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zke.tarul.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tpx.ywan-chungtsiang.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gjr.xziqi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bgh.daxiang520.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zzy.snrcjt.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kby.zhaomingkeji.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gsk.yj20258888.top

[F03] 写入文件（覆盖）
来源：http://ccl.yj20258888.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lhu.bjfxy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://iif.chenjidiqi.icu

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://maf.shanyushiyangtech.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://quq.cdnleiting.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mbi.quarkkingdee.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://eob.chenjidiqi.icu

Ruby: File.write("a.txt", "hi")
来源：http://nis.zdqjudy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://umf.zycfv.cn

[F04] 追加写入文件
来源：http://jtv.quarkkingdee.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zyk.yongpay.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ajn.shanyushiyangkeji.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rym.gotoacloud.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cen.feifeiyinyue.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://isq.zhixingplan.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://add.hfpthk.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rjs.xuanzx.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wie.guannengcc.top

[F05] 判断文件或目录是否存在
来源：http://cur.yj20258888.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vli.zhixingplan.top

PHP:  file_exists("a.txt");
来源：http://nvn.hongshengwenyu.top

JS:   fs.existsSync("a.txt")
来源：http://xcb.ydzc1.top

TS:   fs.existsSync("a.txt")
来源：http://did.hnqzz.top

Java: Files.exists(Path.of("a.txt"))
来源：http://nnn.feifeiyinyue.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gxk.c1oappe.top

Ruby: File.exist?("a.txt")
来源：http://cdg.dashuyun.cn

C#:   File.Exists("a.txt")
来源：http://rib.ydzc1.top

[F06] 删除文件
来源：http://ypn.jinghuilouyu.cn

Py:   os.remove("a.txt")
来源：http://jrj.quarkkingdee.top

PHP:  unlink("a.txt");
来源：http://xny.cheryme.top

JS:   fs.unlinkSync("a.txt")
来源：http://oli.jinyuanbaomall.cn

TS:   fs.unlinkSync("a.txt")
来源：http://gzx.yj202588.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://phy.jlsjyb.cn

Go:   os.Remove("a.txt")
来源：http://sca.vehdjk.com

Ruby: File.delete("a.txt")
来源：http://dpk.hesvh.cn

C#:   File.Delete("a.txt");
来源：http://rgd.xingfuxueyuan.xyz

[F07] 创建目录（含多级）
来源：http://cfk.guannengcc.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qlj.pengpengdd.cyou

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jya.daxiang520.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tzy.zycfv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lfz.hfpthk.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yhq.ivvv.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ebk.shzxlz.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pfy.jinyuanbaomall.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rrt.pycfn.com

[F08] 遍历目录
来源：http://efc.yongpay.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://gvr.yongpay.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qzm.xziqi.cn

JS:   fs.readdirSync("dir")
来源：http://qgu.316326.xyz

TS:   fs.readdirSync("dir")
来源：http://czd.yanxiufei.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nno.zhoulong.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://vyi.yvedp.cn

Ruby: Dir.children("dir")
来源：http://aey.zhoulong.xyz

C#:   Directory.GetFiles("dir")
来源：http://utd.ywan-chungtsiang.top

[F09] 获取文件大小
来源：http://uri.zdbjq.cn

Py:   os.path.getsize("a.txt")
来源：http://yvc.dianchejie.cn

PHP:  filesize("a.txt");
来源：http://pec.tanke756.top

JS:   fs.statSync("a.txt").size
来源：http://cpn.hywenlv.cn

TS:   fs.statSync("a.txt").size
来源：http://yha.dianchejie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://dhd.yuxming.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dtj.guannengcc.top

Ruby: File.size("a.txt")
来源：http://xor.aibaodan.cn

C#:   new FileInfo("a.txt").Length
来源：http://cid.vehdjk.com

[F10] 取文件扩展名 / 文件名
来源：http://bpz.redwolf501.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jtc.ivvv.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fqf.snrcjt.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ysm.zhengqikj.top

TS:   path.extname("a.txt")
来源：http://pcc.dianchejie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://eyz.wangshuangyany.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ooc.hammf.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://chh.bjfxy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dru.hysaishi.cn

[F11] 复制与移动文件
来源：http://gya.xinyue.icu

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tyz.jianghu66.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://egh.daxiang520.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ghf.shuidangran.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ywc.aizwys.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zws.zhoulong.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dsc.pengpengdd.cyou

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ynp.nanxuanxn.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://voa.aibaodan.cn

[F12] CSV 读写
来源：http://fxg.xziqi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tmz.pycfn.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fnc.iojbl.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zmu.shanyushiyangtech.top

TS:   // 同上
来源：http://tmr.yuxming.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://llj.chenzaomai.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fxj.zhongyouzk.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tsq.jinqigfzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://axx.hysaishi.cn

================================================================================
来源：http://wvs.cqqwz.cn

G. 面向对象
来源：http://qmu.vehdjk.com

================================================================================
来源：http://cwd.shanyushiyangkeji.top

[G01] 定义类
来源：http://qvr.daxiang520.top

Py:   class User: pass
来源：http://wjo.zhongyouzk.top

PHP:  class User {}
来源：http://bau.yanxiufei.cn

JS:   class User {}
来源：http://emv.dianchejie.cn

TS:   class User { name: string = ""; }
来源：http://wyq.gotoacloud.top

Java: class User {}
来源：http://yat.ivvv.top

Go:   type User struct { Name string }
来源：http://sxu.hcnkem.com

Ruby: class User; end
来源：http://nwn.pycfn.com

C#:   class User {}
来源：http://fav.svipenyu.cn

[G02] 构造函数
来源：http://bat.jiagoushi.top

Py:   def __init__(self, name): self.name = name
来源：http://hco.9152youxi.cn

PHP:  public function __construct(public string $name) {}
来源：http://qad.iojbl.cn

JS:   constructor(name) { this.name = name; }
来源：http://uug.fehbvm.com

TS:   constructor(public name: string) {}
来源：http://hnm.0kj1m.cn

Java: User(String name) { this.name = name; }
来源：http://ggt.quarkkingdee.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fyl.fktsv.cn

Ruby: def initialize(name); @name = name; end
来源：http://nmk.andypj.xyz

C#:   public User(string name) { Name = name; }
来源：http://rqu.ydjk.org.cn

[G03] 实例属性
来源：http://rlq.fktsv.cn

Py:   self.name = "x"
来源：http://cau.pycfn.com

PHP:  public string $name = "x";
来源：http://pan.feifeiyinyue.top

JS:   this.name = "x";
来源：http://exm.yfazqb.com

TS:   name: string = "x";
来源：http://smx.daxiang520.top

Java: private String name;
来源：http://vmy.dianchejie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zwj.hesvh.cn

Ruby: @name = "x"
来源：http://yrp.smart0.xyz

C#:   public string Name { get; set; } = "x";
来源：http://lks.jinyuanbaomall.cn

[G04] 定义方法
来源：http://uel.epnwcf.com

Py:   def greet(self): return self.name
来源：http://hyl.chenzaomai.com

PHP:  public function greet(): string { return $this->name; }
来源：http://mie.havefunace.top

JS:   greet() { return this.name; }
来源：http://bwb.tianlin.xyz

TS:   greet(): string { return this.name; }
来源：http://cnq.gotoacloud.top

Java: String greet() { return name; }
来源：http://mxq.havefunace.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://zis.yonumen.top

Ruby: def greet; @name; end
来源：http://duf.fengsongda.top

C#:   public string Greet() => Name;
来源：http://fth.zhongyouzk.top

[G05] 继承
来源：http://jnl.cdnleiting.top

Py:   class Admin(User): pass
来源：http://ckp.ydzc1.top

PHP:  class Admin extends User {}
来源：http://aza.uphjek.com

JS:   class Admin extends User {}
来源：http://ibr.jinyuanbaomall.cn

TS:   class Admin extends User {}
来源：http://nku.wangdashe.top

Java: class Admin extends User {}
来源：http://sva.daria6918.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lnm.haohaochexian.top

Ruby: class Admin < User; end
来源：http://jow.yonumen.top

C#:   class Admin : User {}
来源：http://jwq.aibaodan.cn

[G06] 重写方法
来源：http://tkb.zhoulong.xyz

Py:   def greet(self): return "admin"
来源：http://uac.quarkkingdee.top

PHP:  public function greet(): string { return "admin"; }
来源：http://cfj.pengpengdd.cyou

JS:   greet() { return "admin"; }
来源：http://szm.chenlongwang.top

TS:   greet(): string { return "admin"; }
来源：http://lkb.dashuyun.cn

Java: @Override String greet() { return "admin"; }
来源：http://zje.sweek.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hlj.ydzc1.top

Ruby: def greet; "admin"; end
来源：http://pgf.snrcjt.cn

C#:   public override string Greet() => "admin";
来源：http://cyf.cdnleiting.top

[G07] 调用父类方法
来源：http://sig.52xcode.cn

Py:   super().greet()
来源：http://mzh.hcnkem.com

PHP:  parent::greet();
来源：http://hmm.sufxvd.cn

JS:   super.greet();
来源：http://pwe.zhijiandao.cn

TS:   super.greet();
来源：http://ksr.jyoumei.cn

Java: super.greet();
来源：http://fek.wangshuangyany.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tkv.tarul.cn

Ruby: super
来源：http://rhy.ybcxt.top

C#:   base.Greet();
来源：http://afa.pycfn.com

[G08] 静态方法与属性
来源：http://goi.yj20258888.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://oct.yuanzhike.top

PHP:  public static function f() {}
来源：http://mvm.ydjk.org.cn

JS:   static f() {}
来源：http://vzv.jlsjyb.cn

TS:   static f(): void {}
来源：http://ixq.nanxinkj.top

Java: static void f() {}
来源：http://onw.sjlbkw.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qnm.smart0.xyz

Ruby: def self.f; end
来源：http://jvg.316326.xyz

C#:   public static void F() {}
来源：http://fut.epnwcf.com

[G09] 接口 / 抽象类
来源：http://meq.guannengcc.top

Py:   from abc import ABC, abstractmethod
来源：http://rgu.0kj1m.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ppp.jqgufenzy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://pif.316326.xyz

TS:   interface Shape { area(): number; }
来源：http://tzn.c1oappe.top

Java: interface Shape { double area(); }
来源：http://fed.cashguo.top

Go:   type Shape interface { Area() float64 }
来源：http://usn.hongshengwenyu.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ood.aibaodan.cn

C#:   interface IShape { double Area(); }
来源：http://xix.guowangkeji.top

[G10] 访问控制
来源：http://gdy.hywenlv.cn

Py:   约定 _protected / __private（不强制）
来源：http://hgl.gotoacloud.top

PHP:  public / protected / private
来源：http://bdc.wangshuangyany.cn

JS:   #private 字段；其余公开
来源：http://qja.jqgfzy.top

TS:   public / protected / private
来源：http://ytv.sweek.top

Java: public / protected / private / 默认包级
来源：http://eqi.mhx1999.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://sez.52xcode.cn

Ruby: public / protected / private
来源：http://ixy.sxryk.cn

C#:   public / protected / private / internal
来源：http://toc.bjfxy.top

[G11] getter / setter
来源：http://mqn.zhiwuduotai.top

Py:   @property 与 @x.setter
来源：http://iqk.nanxinkj.top

PHP:  public function getName(): string { return $this->name; }
来源：http://sfw.xingfuxueyuan.xyz

JS:   get name() { return this._name; }
来源：http://lbw.zhixingplan.top

TS:   get name(): string { return this._name; }
来源：http://doh.smart0.xyz

Java: public String getName() { return name; }
来源：http://yyc.ywan-chungtsiang.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://pjp.snrcjt.cn

Ruby: attr_accessor :name
来源：http://fpr.ydzc1.top

C#:   public string Name { get; set; }
来源：http://slx.nanxinkj.top

[G12] 对象转字符串
来源：http://zxi.ppjwa.cn

Py:   def __str__(self): return self.name
来源：http://nlc.52xcode.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://nzl.nanxuanxn.top

JS:   toString() { return this.name; }
来源：http://edd.yangfankeji.com

TS:   toString(): string { return this.name; }
来源：http://wqi.shangyingyoupin.top

Java: @Override public String toString() { return name; }
来源：http://qox.ctjpmb.com

Go:   func (u User) String() string { return u.Name }
来源：http://lpl.hfpthk.cn

Ruby: def to_s; @name; end
来源：http://jgi.nanxinkj.top

C#:   public override string ToString() => Name;
来源：http://rwx.cucudq.cn

[G13] 判断对象类型
来源：http://cgb.daxiang520.top

Py:   isinstance(u, User)
来源：http://qsc.gotoacloud.top

PHP:  $u instanceof User
来源：http://tmi.zycfv.cn

JS:   u instanceof User
来源：http://ryg.chenzaomai.com

TS:   u instanceof User
来源：http://yha.hfpthk.cn

Java: u instanceof User
来源：http://nfc.xziqi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zwe.ppjwa.cn

Ruby: u.is_a?(User)
来源：http://xqt.nwbrower.top

C#:   u is User
来源：http://bwz.cucudq.cn

[G14] 数据类 / record
来源：http://rou.wangdashe.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qra.nanxinkj.top

PHP:  // 用 readonly 属性模拟
来源：http://soj.yonumen.top

JS:   // 无内置：普通类或对象字面量
来源：http://xus.dashuyun.cn

TS:   type User = { name: string; age: number };
来源：http://hol.wangshuangyany.cn

Java: record User(String name, int age) {}
来源：http://ptr.ppjwa.cn

Go:   type User struct { Name string; Age int }
来源：http://dma.316326.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://asr.gzhubu.top


<!-- 参考信息 -->