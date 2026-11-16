代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gxp.shanyushiyangkeji.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yga.yfazqb.com

C#:   1234567.ToString("N0")
来源：http://hva.chenjidiqi.icu

[E17] 首字母大写
来源：http://pyf.aizwys.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tnd.nanxinkj.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://vil.yfazqb.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://axe.shangyingyoupin.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jmq.fktsv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://juf.ctjpmb.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jco.shangyingyoupin.top

Ruby: s.capitalize
来源：http://otq.ybcxt.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jdp.yj20258.top

[E18] 模板占位符替换
来源：http://trz.cheryme.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kdl.ctjpmb.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uog.yueranfly.top

JS:   tpl.replaceAll("{name}", name)
来源：http://fop.yuxming.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tey.52xcode.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vyt.cqqwz.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cdy.hnxiangtu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://teh.andypj.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://icx.zhengqikj.top

[E19] 多行文本按行拆分
来源：http://gzk.zhoulong.xyz

Py:   s.splitlines()
来源：http://jrg.ywan-chungtsiang.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hzr.ybcxt.top

JS:   s.split(/\r?\n/)
来源：http://mka.cdnleiting.top

TS:   s.split(/\r?\n/)
来源：http://tid.hnqzz.top

Java: s.lines().toList()
来源：http://ewp.iojbl.cn

Go:   strings.Split(s, "\n")
来源：http://sca.xinyue.icu

Ruby: s.lines
来源：http://kyy.chenjidiqi.icu

C#:   s.Split('\n')
来源：http://rlt.bbcook.cn

[E20] 判断字符串是否为空
来源：http://ext.cqqwz.cn

Py:   if not s:
来源：http://aud.haohaochexian.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ldy.mhx1999.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://loa.quarkkingdee.top

TS:   if (s === "") {}
来源：http://swz.xylfe.cn

Java: if (s.isEmpty()) {}
来源：http://pvk.xylfe.cn

Go:   if s == "" {}
来源：http://lsh.xziqi.cn

Ruby: if s.empty?
来源：http://xlj.kuanghao11.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bia.iojbl.cn

[E21] 超长截断加省略号
来源：http://ywp.wangdashe.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vac.ehwqpu.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://css.fengsongda.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zob.yonumen.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yyk.sweek.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pib.yongpay.top

Go:   // 按 rune 判断长度后截断
来源：http://wwg.havefunace.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yqy.redwolf501.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zgm.fehbvm.com

[E22] 字节长度与字符长度
来源：http://kti.aibaodan.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ong.hnxiangtu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gsr.sufxvd.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rrn.xinyue.icu

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yrf.sjlbkw.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wqt.cucudq.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lnl.zhoulong.xyz

Ruby: s.bytesize;  s.length
来源：http://eia.jinghuilouyu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://byx.vehdjk.com

================================================================================
来源：http://tby.316326.xyz

F. 文件与目录
来源：http://eeh.cheryme.top

================================================================================
来源：http://vcn.yangfankeji.com

[F01] 读取整个文件
来源：http://rkx.gzhubu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://npc.aizwys.cn

PHP:  file_get_contents("a.txt");
来源：http://ljl.daria6918.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://iwh.jyoumei.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ubi.zycfv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ggs.andypj.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rua.fehbvm.com

Ruby: File.read("a.txt")
来源：http://avu.nwbrower.top

C#:   File.ReadAllText("a.txt");
来源：http://bee.dianchejie.cn

[F02] 逐行读取文件
来源：http://xqo.zhijiandao.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pwb.jqgufenzy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dai.yuxming.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pes.jianghu66.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ixt.feifeiyinyue.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uyo.yj20258.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://uwy.fanxiaobao.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rtr.aibaodan.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hpl.yangfankeji.com

[F03] 写入文件（覆盖）
来源：http://vht.sufxvd.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jdi.nanxuanxn.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://nes.zhijiandao.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fgt.hesvh.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://erb.zdqjudy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gll.jiagoushi.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ddm.xziqi.cn

Ruby: File.write("a.txt", "hi")
来源：http://udd.yangfankeji.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qcb.xuanzx.com

[F04] 追加写入文件
来源：http://wrl.zycfv.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wkg.birdmap.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://udm.uphjek.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://igw.wangshuangyany.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://akf.redwolf501.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hij.zhaomingkeji.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dtk.jqgfzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yec.yongpay.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nzw.hfpthk.cn

[F05] 判断文件或目录是否存在
来源：http://cfl.feifeiyinyue.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bsi.sweek.top

PHP:  file_exists("a.txt");
来源：http://pgr.smart0.xyz

JS:   fs.existsSync("a.txt")
来源：http://hfm.52xcode.cn

TS:   fs.existsSync("a.txt")
来源：http://qkz.xuetiantiany.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://rmd.zdbjq.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xnq.ybcxt.top

Ruby: File.exist?("a.txt")
来源：http://iym.xuetiantiany.cn

C#:   File.Exists("a.txt")
来源：http://ley.xingfuxueyuan.xyz

[F06] 删除文件
来源：http://onw.pengpengdd.cyou

Py:   os.remove("a.txt")
来源：http://keh.xuanzx.com

PHP:  unlink("a.txt");
来源：http://hns.hongshengwenyu.top

JS:   fs.unlinkSync("a.txt")
来源：http://vig.hnxiangtu.top

TS:   fs.unlinkSync("a.txt")
来源：http://nwk.jinghuilouyu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wuz.wangdashe.top

Go:   os.Remove("a.txt")
来源：http://gnn.hnqzz.top

Ruby: File.delete("a.txt")
来源：http://qnj.yueranfly.top

C#:   File.Delete("a.txt");
来源：http://sjz.yuanzhike.top

[F07] 创建目录（含多级）
来源：http://ozo.kuanghao11.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rxm.fengsongda.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pqz.shanyushiyangkeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dia.jiagoushi.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://und.havefunace.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gcm.feifeiyinyue.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sny.iojbl.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jmd.yj202588.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hle.gogol.net.cn

[F08] 遍历目录
来源：http://ofc.gogol.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://mts.yj20258.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://axe.gotoacloud.top

JS:   fs.readdirSync("dir")
来源：http://zfb.fzhhl.top

TS:   fs.readdirSync("dir")
来源：http://pjf.sufxvd.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pdr.chenzaomai.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://uen.shzxlz.cn

Ruby: Dir.children("dir")
来源：http://txj.kuanghao11.cn

C#:   Directory.GetFiles("dir")
来源：http://ula.yj20258.top

[F09] 获取文件大小
来源：http://htv.nwbrower.top

Py:   os.path.getsize("a.txt")
来源：http://khn.yvedp.cn

PHP:  filesize("a.txt");
来源：http://vpm.jlsjyb.cn

JS:   fs.statSync("a.txt").size
来源：http://roz.xziqi.cn

TS:   fs.statSync("a.txt").size
来源：http://myy.sweek.top

Java: Files.size(Path.of("a.txt"))
来源：http://aav.gaohongyu789.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lfe.mhx1999.top

Ruby: File.size("a.txt")
来源：http://fhw.havefunace.top

C#:   new FileInfo("a.txt").Length
来源：http://fpl.cashguo.top

[F10] 取文件扩展名 / 文件名
来源：http://epp.gotoacloud.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://oqi.jlsjyb.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pzu.gaohongyu789.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dlr.shzxlz.cn

TS:   path.extname("a.txt")
来源：http://dss.dashuyun.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://psr.jinqigfzy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pmp.bbcook.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wzf.mhx1999.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xcq.fengsongda.top

[F11] 复制与移动文件
来源：http://raj.wangdashe.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://goe.ctjpmb.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ccn.sweek.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jkq.yonumen.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ewe.fehbvm.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qlo.yvedp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qqz.ydjk.org.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fby.tian-w.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qod.tanke756.top

[F12] CSV 读写
来源：http://eaa.xinyue.icu

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sqi.jinyuanbaomall.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cwj.wangshuangyany.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mba.shuidangran.top

TS:   // 同上
来源：http://akk.guowangkeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://buc.shanyushiyangtech.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ydt.zycfv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nie.iojbl.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://yvo.smart0.xyz

================================================================================
来源：http://xbi.ppjwa.cn

G. 面向对象
来源：http://omo.gzhubu.top

================================================================================
来源：http://emg.nwbrower.top

[G01] 定义类
来源：http://vii.yfazqb.com

Py:   class User: pass
来源：http://ghc.fanxiaobao.xyz

PHP:  class User {}
来源：http://bre.nwbrower.top

JS:   class User {}
来源：http://gyb.cdnleiting.top

TS:   class User { name: string = ""; }
来源：http://jyi.zhoulong.xyz

Java: class User {}
来源：http://djy.guannengcc.top

Go:   type User struct { Name string }
来源：http://qhz.cdnleiting.top

Ruby: class User; end
来源：http://erz.zhongyouzk.top

C#:   class User {}
来源：http://gvm.ydzc1.top

[G02] 构造函数
来源：http://tbt.vqdsnc.cn

Py:   def __init__(self, name): self.name = name
来源：http://lgb.c1oappe.top

PHP:  public function __construct(public string $name) {}
来源：http://agt.jyoumei.cn

JS:   constructor(name) { this.name = name; }
来源：http://xwy.gaohongyu789.top

TS:   constructor(public name: string) {}
来源：http://zri.shanyushiyangtech.top

Java: User(String name) { this.name = name; }
来源：http://jfm.kuanghao11.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ujk.yuxming.cn

Ruby: def initialize(name); @name = name; end
来源：http://lxm.gaohongyu789.top

C#:   public User(string name) { Name = name; }
来源：http://sna.ydjk.org.cn

[G03] 实例属性
来源：http://szw.gotoacloud.top

Py:   self.name = "x"
来源：http://dxv.0kj1m.cn

PHP:  public string $name = "x";
来源：http://uyg.zhixingplan.top

JS:   this.name = "x";
来源：http://fdf.chenlongwang.top

TS:   name: string = "x";
来源：http://dms.daria6918.cn

Java: private String name;
来源：http://egv.vqdsnc.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yoe.pengpengdd.cyou

Ruby: @name = "x"
来源：http://wyj.sxryk.cn

C#:   public string Name { get; set; } = "x";
来源：http://glp.hnqzz.top

[G04] 定义方法
来源：http://rzx.ivvv.top

Py:   def greet(self): return self.name
来源：http://jfq.shuidangran.top

PHP:  public function greet(): string { return $this->name; }
来源：http://dzq.cucudq.cn

JS:   greet() { return this.name; }
来源：http://ekm.yj20258.top

TS:   greet(): string { return this.name; }
来源：http://swr.kuanghao11.cn

Java: String greet() { return name; }
来源：http://plt.shangyingyoupin.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://pli.daria6918.cn

Ruby: def greet; @name; end
来源：http://bhw.zhaomingkeji.xyz

C#:   public string Greet() => Name;
来源：http://qon.cashguo.top

[G05] 继承
来源：http://ypc.jinyuanbaomall.cn

Py:   class Admin(User): pass
来源：http://xiz.yj202588.top

PHP:  class Admin extends User {}
来源：http://gsw.vehdjk.com

JS:   class Admin extends User {}
来源：http://eyk.hysaishi.cn

TS:   class Admin extends User {}
来源：http://akv.ctjpmb.com

Java: class Admin extends User {}
来源：http://dix.jianghu66.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://sla.vqdsnc.cn

Ruby: class Admin < User; end
来源：http://giq.chenjidiqi.icu

C#:   class Admin : User {}
来源：http://kge.yongpay.top

[G06] 重写方法
来源：http://jbm.tarul.cn

Py:   def greet(self): return "admin"
来源：http://iwo.mhx1999.top

PHP:  public function greet(): string { return "admin"; }
来源：http://rlu.vehdjk.com

JS:   greet() { return "admin"; }
来源：http://hyq.hongshengwenyu.top

TS:   greet(): string { return "admin"; }
来源：http://ntj.c1oappe.top

Java: @Override String greet() { return "admin"; }
来源：http://gll.nwbrower.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mhv.birdmap.top

Ruby: def greet; "admin"; end
来源：http://yoo.snrcjt.cn

C#:   public override string Greet() => "admin";
来源：http://tdz.yj20258.top

[G07] 调用父类方法
来源：http://gvp.shuidangran.top

Py:   super().greet()
来源：http://mbd.pycfn.com

PHP:  parent::greet();
来源：http://bcn.zhaomingkeji.xyz

JS:   super.greet();
来源：http://jhp.xuetiantiany.cn

TS:   super.greet();
来源：http://gvw.tian-w.cn

Java: super.greet();
来源：http://dtp.shuidangran.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xmg.sufxvd.cn

Ruby: super
来源：http://klf.sxryk.cn

C#:   base.Greet();
来源：http://bey.jqgufenzy.top

[G08] 静态方法与属性
来源：http://tei.yj20258.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sms.yanxiufei.cn

PHP:  public static function f() {}
来源：http://cdc.zycfv.cn

JS:   static f() {}
来源：http://ild.snrcjt.cn

TS:   static f(): void {}
来源：http://qfi.yangfankeji.com

Java: static void f() {}
来源：http://xyd.c1oappe.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://srm.shzxlz.cn

Ruby: def self.f; end
来源：http://jjs.cheryme.top

C#:   public static void F() {}
来源：http://jod.mhx1999.top

[G09] 接口 / 抽象类
来源：http://asi.jlsjyb.cn

Py:   from abc import ABC, abstractmethod
来源：http://hvw.yangfankeji.com

PHP:  interface Shape { public function area(): float; }
来源：http://lfm.zhongyouzk.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://qrj.haohaochexian.top

TS:   interface Shape { area(): number; }
来源：http://rku.bjfxy.top

Java: interface Shape { double area(); }
来源：http://wyf.aizwys.cn

Go:   type Shape interface { Area() float64 }
来源：http://mnq.andypj.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ili.yj20258.top

C#:   interface IShape { double Area(); }
来源：http://lym.ywan-chungtsiang.top

[G10] 访问控制
来源：http://yyb.jinqigfzy.top

Py:   约定 _protected / __private（不强制）
来源：http://uil.shzxlz.cn

PHP:  public / protected / private
来源：http://bmb.gzhubu.top

JS:   #private 字段；其余公开
来源：http://ruw.fengsongda.top

TS:   public / protected / private
来源：http://rhr.zhijiandao.cn

Java: public / protected / private / 默认包级
来源：http://mgp.vqdsnc.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tus.quarkkingdee.top

Ruby: public / protected / private
来源：http://oju.bbcook.cn

C#:   public / protected / private / internal
来源：http://chk.jqgufenzy.top

[G11] getter / setter
来源：http://oea.guowangkeji.top

Py:   @property 与 @x.setter
来源：http://pki.jinyuanbaomall.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://anh.sysykeji.top

JS:   get name() { return this._name; }
来源：http://buz.yongpay.top

TS:   get name(): string { return this._name; }
来源：http://rik.c1oappe.top

Java: public String getName() { return name; }
来源：http://wkw.gotoacloud.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://nml.dashuyun.cn

Ruby: attr_accessor :name
来源：http://bwc.ctjpmb.com

C#:   public string Name { get; set; }
来源：http://hzm.yonumen.top

[G12] 对象转字符串
来源：http://xxb.jiagoushi.top

Py:   def __str__(self): return self.name
来源：http://pbr.yj20258888.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://aqe.hammf.cn

JS:   toString() { return this.name; }
来源：http://ywu.feifeiyinyue.top

TS:   toString(): string { return this.name; }
来源：http://hkq.hongshengwenyu.top

Java: @Override public String toString() { return name; }
来源：http://erh.tianlin.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://tsj.hfpthk.cn

Ruby: def to_s; @name; end
来源：http://woj.smart0.xyz

C#:   public override string ToString() => Name;
来源：http://glp.ctjpmb.com

[G13] 判断对象类型
来源：http://hwj.guowangkeji.top

Py:   isinstance(u, User)
来源：http://xxx.smart0.xyz

PHP:  $u instanceof User
来源：http://yez.hysaishi.cn

JS:   u instanceof User
来源：http://jcx.316326.xyz

TS:   u instanceof User
来源：http://tcg.chenjidiqi.icu

Java: u instanceof User
来源：http://ehm.fktsv.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://srr.xuanzx.com

Ruby: u.is_a?(User)
来源：http://brq.pengpengdd.cyou

C#:   u is User
来源：http://twf.vqdsnc.cn

[G14] 数据类 / record
来源：http://wpp.bjfxy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qya.smart0.xyz

PHP:  // 用 readonly 属性模拟
来源：http://bjc.tarul.cn

JS:   // 无内置：普通类或对象字面量
来源：http://oig.tianlin.xyz

TS:   type User = { name: string; age: number };
来源：http://qfk.jinqigufen.top

Java: record User(String name, int age) {}
来源：http://qms.aibaodan.cn

Go:   type User struct { Name string; Age int }
来源：http://adj.zhijiandao.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yvw.zhoulong.xyz

C#:   record User(string Name, int Age);
来源：http://evj.ydjk.org.cn

[G15] 枚举
来源：http://xmq.shuidangran.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dgh.shanyushiyangkeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://zey.zhaomingkeji.xyz


<!-- 参考信息 -->