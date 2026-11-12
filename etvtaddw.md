代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nld.jlsjyb.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kvs.dianchejie.cn

C#:   1234567.ToString("N0")
来源：http://suh.chenjidiqi.icu

[E17] 首字母大写
来源：http://smi.wangshuangyany.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ekx.sufxvd.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pbf.sysykeji.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zcr.jyoumei.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://klw.uphjek.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ktb.cucudq.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rba.shangyingyoupin.top

Ruby: s.capitalize
来源：http://avu.hywenlv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wek.zhengqikj.top

[E18] 模板占位符替换
来源：http://bzf.bjfxy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ebj.yuxming.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rrq.shanyushiyangtech.top

JS:   tpl.replaceAll("{name}", name)
来源：http://neu.ybcxt.top

TS:   tpl.replaceAll("{name}", name)
来源：http://xzk.cucudq.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mva.zhixingplan.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://abb.gzhubu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zjp.zhengqikj.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vlp.zhongyouzk.top

[E19] 多行文本按行拆分
来源：http://pzz.yuanzhike.top

Py:   s.splitlines()
来源：http://sro.sjlbkw.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wbe.yonumen.top

JS:   s.split(/\r?\n/)
来源：http://rrb.yangfankeji.com

TS:   s.split(/\r?\n/)
来源：http://klb.gzhubu.top

Java: s.lines().toList()
来源：http://hrv.mhx1999.top

Go:   strings.Split(s, "\n")
来源：http://scl.0kj1m.cn

Ruby: s.lines
来源：http://lmy.sweek.top

C#:   s.Split('\n')
来源：http://wfm.cheryme.top

[E20] 判断字符串是否为空
来源：http://sfh.jqgfzy.top

Py:   if not s:
来源：http://wyu.daxiang520.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dog.gaohongyu789.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tlh.0kj1m.cn

TS:   if (s === "") {}
来源：http://ktl.jqgufenzy.top

Java: if (s.isEmpty()) {}
来源：http://zbg.zycfv.cn

Go:   if s == "" {}
来源：http://upi.epnwcf.com

Ruby: if s.empty?
来源：http://gvz.jqgfzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://avj.birdmap.top

[E21] 超长截断加省略号
来源：http://lnd.tian-w.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cpd.chenlongwang.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://iuo.zhengqikj.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ehh.daria6918.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mst.jinghuilouyu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fdz.ywan-chungtsiang.top

Go:   // 按 rune 判断长度后截断
来源：http://avf.wangdashe.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bmc.zhoulong.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wqv.shanyushiyangkeji.top

[E22] 字节长度与字符长度
来源：http://evr.dashuyun.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ctp.hesvh.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://glj.jianghu66.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ojv.yanxiufei.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://btd.sufxvd.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yoh.sufxvd.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nwx.hysaishi.cn

Ruby: s.bytesize;  s.length
来源：http://zcb.yuanzhike.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dwg.ctjpmb.com

================================================================================
来源：http://ani.hongshengwenyu.top

F. 文件与目录
来源：http://psr.dianchejie.cn

================================================================================
来源：http://xkz.hnqzz.top

[F01] 读取整个文件
来源：http://jkz.kuanghao11.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vvg.yanxiufei.cn

PHP:  file_get_contents("a.txt");
来源：http://euk.xylfe.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://oqe.redwolf501.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rmd.zhijiandao.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://kwd.vehdjk.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ndl.sufxvd.cn

Ruby: File.read("a.txt")
来源：http://ulb.yj20258888.top

C#:   File.ReadAllText("a.txt");
来源：http://oso.chenzaomai.com

[F02] 逐行读取文件
来源：http://lrr.chenjidiqi.icu

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://njb.gotoacloud.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qwb.sweek.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://alb.andypj.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rsj.yangfankeji.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://iuq.shangyingyoupin.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://odc.feifeiyinyue.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://plb.xylfe.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tmb.aibaodan.cn

[F03] 写入文件（覆盖）
来源：http://xkr.ivvv.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vyv.xinyue.icu

PHP:  file_put_contents("a.txt", "hi");
来源：http://klr.hesvh.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://apy.tarul.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fkh.redwolf501.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hmq.yangfankeji.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fht.zdbjq.cn

Ruby: File.write("a.txt", "hi")
来源：http://ito.xuetiantiany.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://elb.sysykeji.top

[F04] 追加写入文件
来源：http://wlx.haohaochexian.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://eyp.shangyingyoupin.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fhd.fehbvm.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fah.tanke756.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bmx.nwbrower.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://eam.xinyue.icu

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ofr.yongpay.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cbu.zhiwuduotai.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pve.iojbl.cn

[F05] 判断文件或目录是否存在
来源：http://nft.yuanzhike.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wxg.tarul.cn

PHP:  file_exists("a.txt");
来源：http://oxt.zhiwuduotai.top

JS:   fs.existsSync("a.txt")
来源：http://ggx.daxiang520.top

TS:   fs.existsSync("a.txt")
来源：http://yzo.daria6918.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://lcg.zhaomingkeji.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rkt.zhiwuduotai.top

Ruby: File.exist?("a.txt")
来源：http://bvk.chenlongwang.top

C#:   File.Exists("a.txt")
来源：http://ihq.dianchejie.cn

[F06] 删除文件
来源：http://ohv.0kj1m.cn

Py:   os.remove("a.txt")
来源：http://rov.yueranfly.top

PHP:  unlink("a.txt");
来源：http://pta.shzxlz.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gpt.chenjidiqi.icu

TS:   fs.unlinkSync("a.txt")
来源：http://ncf.yvedp.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dvj.c1oappe.top

Go:   os.Remove("a.txt")
来源：http://rxh.316326.xyz

Ruby: File.delete("a.txt")
来源：http://eix.havefunace.top

C#:   File.Delete("a.txt");
来源：http://vlq.ppjwa.cn

[F07] 创建目录（含多级）
来源：http://tyw.daxiang520.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xcr.meibo888.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://snb.yonumen.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nak.epnwcf.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ybc.kuanghao11.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://evb.havefunace.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ijz.shanyushiyangkeji.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fyv.zhijiandao.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bhf.kuanghao11.cn

[F08] 遍历目录
来源：http://zes.ehwqpu.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://fyh.tianlin.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://epy.sjlbkw.cn

JS:   fs.readdirSync("dir")
来源：http://wpn.jyoumei.cn

TS:   fs.readdirSync("dir")
来源：http://nrj.haohaochexian.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mpu.snrcjt.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://njg.zhongyouzk.top

Ruby: Dir.children("dir")
来源：http://gyz.shzxlz.cn

C#:   Directory.GetFiles("dir")
来源：http://rgl.xingfuxueyuan.xyz

[F09] 获取文件大小
来源：http://zhf.havefunace.top

Py:   os.path.getsize("a.txt")
来源：http://lgc.feifeiyinyue.top

PHP:  filesize("a.txt");
来源：http://foy.shanyushiyangkeji.top

JS:   fs.statSync("a.txt").size
来源：http://fmd.cashguo.top

TS:   fs.statSync("a.txt").size
来源：http://pgq.hammf.cn

Java: Files.size(Path.of("a.txt"))
来源：http://klo.hongshengwenyu.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fdi.nwbrower.top

Ruby: File.size("a.txt")
来源：http://yql.zdbjq.cn

C#:   new FileInfo("a.txt").Length
来源：http://aqc.chenzaomai.com

[F10] 取文件扩展名 / 文件名
来源：http://koa.epnwcf.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jxw.aibaodan.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zig.fktsv.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wxj.fzhhl.top

TS:   path.extname("a.txt")
来源：http://qxz.cucudq.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zhz.uphjek.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://erh.52xcode.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rbc.nanxuanxn.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dcj.zdbjq.cn

[F11] 复制与移动文件
来源：http://ewn.cucudq.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ssf.jinyuanbaomall.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ouw.aizwys.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hbg.yj20258888.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lyj.sxryk.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wpq.cqqwz.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://smd.yfazqb.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pcq.dashuyun.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://abs.cashguo.top

[F12] CSV 读写
来源：http://snn.redwolf501.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xot.fanxiaobao.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mgm.hnqzz.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zcb.uphjek.com

TS:   // 同上
来源：http://ggf.yj20258.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ezz.yj202588.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mem.yonumen.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gyd.sufxvd.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://aqc.ivvv.top

================================================================================
来源：http://xia.chenjidiqi.icu

G. 面向对象
来源：http://pme.jinghuilouyu.cn

================================================================================
来源：http://wdu.jianghu66.top

[G01] 定义类
来源：http://wrg.chenjidiqi.icu

Py:   class User: pass
来源：http://egs.jinghuilouyu.cn

PHP:  class User {}
来源：http://ufu.bbcook.cn

JS:   class User {}
来源：http://jof.yuanzhike.top

TS:   class User { name: string = ""; }
来源：http://ifo.ctjpmb.com

Java: class User {}
来源：http://acp.jqgfzy.top

Go:   type User struct { Name string }
来源：http://wxt.epnwcf.com

Ruby: class User; end
来源：http://ekw.zhoulong.xyz

C#:   class User {}
来源：http://gxd.svipenyu.cn

[G02] 构造函数
来源：http://ssz.0kj1m.cn

Py:   def __init__(self, name): self.name = name
来源：http://ocs.vqdsnc.cn

PHP:  public function __construct(public string $name) {}
来源：http://rsx.shzxlz.cn

JS:   constructor(name) { this.name = name; }
来源：http://hth.yueranfly.top

TS:   constructor(public name: string) {}
来源：http://zyf.birdmap.top

Java: User(String name) { this.name = name; }
来源：http://nbx.gzhubu.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kss.chenlongwang.top

Ruby: def initialize(name); @name = name; end
来源：http://qea.redwolf501.top

C#:   public User(string name) { Name = name; }
来源：http://ztm.svipenyu.cn

[G03] 实例属性
来源：http://uul.ehwqpu.com

Py:   self.name = "x"
来源：http://awf.zdbjq.cn

PHP:  public string $name = "x";
来源：http://lpu.hnxiangtu.top

JS:   this.name = "x";
来源：http://ull.52xcode.cn

TS:   name: string = "x";
来源：http://wev.dashuyun.cn

Java: private String name;
来源：http://zgd.ivvv.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wxo.xinyue.icu

Ruby: @name = "x"
来源：http://cyg.shuidangran.top

C#:   public string Name { get; set; } = "x";
来源：http://blb.shzxlz.cn

[G04] 定义方法
来源：http://ved.vqdsnc.cn

Py:   def greet(self): return self.name
来源：http://qts.ywan-chungtsiang.top

PHP:  public function greet(): string { return $this->name; }
来源：http://age.9152youxi.cn

JS:   greet() { return this.name; }
来源：http://lcj.zhongyouzk.top

TS:   greet(): string { return this.name; }
来源：http://dja.nwbrower.top

Java: String greet() { return name; }
来源：http://jao.haohaochexian.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ncw.zhiwuduotai.top

Ruby: def greet; @name; end
来源：http://ykl.chenjidiqi.icu

C#:   public string Greet() => Name;
来源：http://iqg.ivvv.top

[G05] 继承
来源：http://dzz.pycfn.com

Py:   class Admin(User): pass
来源：http://mbi.tarul.cn

PHP:  class Admin extends User {}
来源：http://dsa.guowangkeji.top

JS:   class Admin extends User {}
来源：http://woi.nwbrower.top

TS:   class Admin extends User {}
来源：http://yjy.jianghu66.top

Java: class Admin extends User {}
来源：http://iml.epnwcf.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lmt.cqqwz.cn

Ruby: class Admin < User; end
来源：http://pzv.cheryme.top

C#:   class Admin : User {}
来源：http://itb.chenjidiqi.icu

[G06] 重写方法
来源：http://zkk.xziqi.cn

Py:   def greet(self): return "admin"
来源：http://nft.yj202588.top

PHP:  public function greet(): string { return "admin"; }
来源：http://tbk.sjlbkw.cn

JS:   greet() { return "admin"; }
来源：http://snk.ywan-chungtsiang.top

TS:   greet(): string { return "admin"; }
来源：http://tlr.shanyushiyangtech.top

Java: @Override String greet() { return "admin"; }
来源：http://vox.tanke756.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://axw.vqdsnc.cn

Ruby: def greet; "admin"; end
来源：http://chk.zdqjudy.top

C#:   public override string Greet() => "admin";
来源：http://lot.shuidangran.top

[G07] 调用父类方法
来源：http://sfz.tianlin.xyz

Py:   super().greet()
来源：http://ybw.cashguo.top

PHP:  parent::greet();
来源：http://wtd.zhaomingkeji.xyz

JS:   super.greet();
来源：http://qwx.haohaochexian.top

TS:   super.greet();
来源：http://swp.sjlbkw.cn

Java: super.greet();
来源：http://vao.shzxlz.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zkw.shangyingyoupin.top

Ruby: super
来源：http://esw.gotoacloud.top

C#:   base.Greet();
来源：http://wye.quarkkingdee.top

[G08] 静态方法与属性
来源：http://vef.dianchejie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://glb.ppjwa.cn

PHP:  public static function f() {}
来源：http://jiy.tanke756.top

JS:   static f() {}
来源：http://gxv.tanke756.top

TS:   static f(): void {}
来源：http://xsn.chenlongwang.top

Java: static void f() {}
来源：http://evh.hfpthk.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jkl.shanyushiyangtech.top

Ruby: def self.f; end
来源：http://fri.yangfankeji.com

C#:   public static void F() {}
来源：http://guw.xuanzx.com

[G09] 接口 / 抽象类
来源：http://orb.nanxuanxn.top

Py:   from abc import ABC, abstractmethod
来源：http://own.hammf.cn

PHP:  interface Shape { public function area(): float; }
来源：http://mpu.jinyuanbaomall.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zpo.aibaodan.cn

TS:   interface Shape { area(): number; }
来源：http://txf.fktsv.cn

Java: interface Shape { double area(); }
来源：http://uhq.yj20258888.top

Go:   type Shape interface { Area() float64 }
来源：http://itl.fzhhl.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tpb.wangshuangyany.cn

C#:   interface IShape { double Area(); }
来源：http://gfz.pengpengdd.cyou

[G10] 访问控制
来源：http://wwd.hnqzz.top

Py:   约定 _protected / __private（不强制）
来源：http://dyr.ivvv.top

PHP:  public / protected / private
来源：http://eqn.gaohongyu789.top

JS:   #private 字段；其余公开
来源：http://mud.vqdsnc.cn

TS:   public / protected / private
来源：http://hmb.gotoacloud.top

Java: public / protected / private / 默认包级
来源：http://brb.yongpay.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://oqr.pycfn.com

Ruby: public / protected / private
来源：http://omj.redwolf501.top

C#:   public / protected / private / internal
来源：http://guo.shzxlz.cn

[G11] getter / setter
来源：http://whu.iojbl.cn

Py:   @property 与 @x.setter
来源：http://amp.jinghuilouyu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://upg.jinyuanbaomall.cn

JS:   get name() { return this._name; }
来源：http://hsj.guannengcc.top

TS:   get name(): string { return this._name; }
来源：http://ebi.smart0.xyz

Java: public String getName() { return name; }
来源：http://xnk.yj20258888.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ywv.sysykeji.top

Ruby: attr_accessor :name
来源：http://vda.svipenyu.cn

C#:   public string Name { get; set; }
来源：http://ylv.zhijiandao.cn

[G12] 对象转字符串
来源：http://jmv.yangfankeji.com

Py:   def __str__(self): return self.name
来源：http://rye.jiagoushi.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://hnp.vehdjk.com

JS:   toString() { return this.name; }
来源：http://xnp.yangfankeji.com

TS:   toString(): string { return this.name; }
来源：http://ndf.vehdjk.com

Java: @Override public String toString() { return name; }
来源：http://qvg.nanxinkj.top

Go:   func (u User) String() string { return u.Name }
来源：http://ibm.ydzc1.top

Ruby: def to_s; @name; end
来源：http://zck.shuidangran.top

C#:   public override string ToString() => Name;
来源：http://iiv.daxiang520.top

[G13] 判断对象类型
来源：http://lft.52xcode.cn

Py:   isinstance(u, User)
来源：http://eok.guowangkeji.top

PHP:  $u instanceof User
来源：http://jal.jinqigufen.top

JS:   u instanceof User
来源：http://xfz.dianchejie.cn

TS:   u instanceof User
来源：http://xgt.quarkkingdee.top

Java: u instanceof User
来源：http://vvl.jinyuanbaomall.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ond.yueranfly.top

Ruby: u.is_a?(User)
来源：http://xpa.gogol.net.cn

C#:   u is User
来源：http://ehf.cucudq.cn

[G14] 数据类 / record
来源：http://yaj.jianghu66.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://utv.smart0.xyz

PHP:  // 用 readonly 属性模拟
来源：http://kql.cheryme.top

JS:   // 无内置：普通类或对象字面量
来源：http://hqj.nwbrower.top

TS:   type User = { name: string; age: number };
来源：http://aar.shuidangran.top

Java: record User(String name, int age) {}
来源：http://ebc.ybcxt.top

Go:   type User struct { Name string; Age int }
来源：http://yva.chenzaomai.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uol.0kj1m.cn

C#:   record User(string Name, int Age);
来源：http://qfn.sxryk.cn

[G15] 枚举
来源：http://pfv.redwolf501.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://imr.meibo888.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ekv.yonumen.top


<!-- 参考信息 -->