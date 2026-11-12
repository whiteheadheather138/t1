代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ucq.bjfxy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pst.hesvh.cn

C#:   1234567.ToString("N0")
来源：http://urn.shanyushiyangtech.top

[E17] 首字母大写
来源：http://lbb.tian-w.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zbs.smart0.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://fql.fengsongda.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qfe.zycfv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cqk.bjfxy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fee.shanyushiyangtech.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cnw.gaohongyu789.top

Ruby: s.capitalize
来源：http://wlv.zhoulong.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wzt.pycfn.com

[E18] 模板占位符替换
来源：http://eml.jinyuanbaomall.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rwl.52xcode.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jlf.meibo888.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ztb.chenlongwang.top

TS:   tpl.replaceAll("{name}", name)
来源：http://owc.nanxuanxn.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rut.wangdashe.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pfw.cqqwz.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://amn.ydjk.org.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nlb.zycfv.cn

[E19] 多行文本按行拆分
来源：http://fcc.0kj1m.cn

Py:   s.splitlines()
来源：http://hyk.ybcxt.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ljo.yj20258888.top

JS:   s.split(/\r?\n/)
来源：http://vtd.guannengcc.top

TS:   s.split(/\r?\n/)
来源：http://gya.feifeiyinyue.top

Java: s.lines().toList()
来源：http://lua.chenlongwang.top

Go:   strings.Split(s, "\n")
来源：http://mrn.aizwys.cn

Ruby: s.lines
来源：http://hjd.cashguo.top

C#:   s.Split('\n')
来源：http://zzb.yonumen.top

[E20] 判断字符串是否为空
来源：http://dtx.sysykeji.top

Py:   if not s:
来源：http://hmt.ppjwa.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tbj.zycfv.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sak.zycfv.cn

TS:   if (s === "") {}
来源：http://bys.guannengcc.top

Java: if (s.isEmpty()) {}
来源：http://ndk.tanke756.top

Go:   if s == "" {}
来源：http://yog.cdnleiting.top

Ruby: if s.empty?
来源：http://oen.hnqzz.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cly.shuidangran.top

[E21] 超长截断加省略号
来源：http://bid.zhijiandao.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jrd.dianchejie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wrr.xylfe.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bzf.quarkkingdee.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wif.haohaochexian.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wca.hysaishi.cn

Go:   // 按 rune 判断长度后截断
来源：http://lvj.nanxinkj.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sfx.pycfn.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tko.birdmap.top

[E22] 字节长度与字符长度
来源：http://rjn.yonumen.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uls.aibaodan.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eyz.zhongyouzk.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://enc.chenjidiqi.icu

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dil.hammf.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hyu.zycfv.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://afa.jlsjyb.cn

Ruby: s.bytesize;  s.length
来源：http://sye.ppjwa.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://otn.yfazqb.com

================================================================================
来源：http://xuy.zhengqikj.top

F. 文件与目录
来源：http://txa.bjfxy.top

================================================================================
来源：http://dvq.jinghuilouyu.cn

[F01] 读取整个文件
来源：http://uai.vqdsnc.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xks.bjfxy.top

PHP:  file_get_contents("a.txt");
来源：http://lzb.zhixingplan.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://viy.gaohongyu789.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xjw.redwolf501.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ssr.jinqigufen.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ede.jyoumei.cn

Ruby: File.read("a.txt")
来源：http://zfn.gaohongyu789.top

C#:   File.ReadAllText("a.txt");
来源：http://tmq.gaohongyu789.top

[F02] 逐行读取文件
来源：http://kxp.yanxiufei.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dub.pengpengdd.cyou

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tyw.zhongyouzk.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vue.uphjek.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xkt.sweek.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wwz.vehdjk.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lep.epnwcf.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lsf.gogol.net.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xgn.cheryme.top

[F03] 写入文件（覆盖）
来源：http://miv.tian-w.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yvb.sysykeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://foa.tian-w.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yzj.gogol.net.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://osd.gzhubu.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ida.52xcode.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jwu.wangdashe.top

Ruby: File.write("a.txt", "hi")
来源：http://qit.yueranfly.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wie.yj202588.top

[F04] 追加写入文件
来源：http://mnw.yonumen.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uqi.yfazqb.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://arb.tarul.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aix.yangfankeji.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hfr.jlsjyb.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://oap.fktsv.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://epj.shzxlz.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://iqf.quarkkingdee.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://too.xingfuxueyuan.xyz

[F05] 判断文件或目录是否存在
来源：http://uct.xingfuxueyuan.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yix.tarul.cn

PHP:  file_exists("a.txt");
来源：http://dbm.zhoulong.xyz

JS:   fs.existsSync("a.txt")
来源：http://yzx.vehdjk.com

TS:   fs.existsSync("a.txt")
来源：http://yef.chenlongwang.top

Java: Files.exists(Path.of("a.txt"))
来源：http://tcs.zycfv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zsj.fehbvm.com

Ruby: File.exist?("a.txt")
来源：http://fkx.sufxvd.cn

C#:   File.Exists("a.txt")
来源：http://jhr.pengpengdd.cyou

[F06] 删除文件
来源：http://yof.shanyushiyangkeji.top

Py:   os.remove("a.txt")
来源：http://xxu.wangshuangyany.cn

PHP:  unlink("a.txt");
来源：http://skq.quarkkingdee.top

JS:   fs.unlinkSync("a.txt")
来源：http://wve.yvedp.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hva.hongshengwenyu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pni.yangfankeji.com

Go:   os.Remove("a.txt")
来源：http://wem.wangdashe.top

Ruby: File.delete("a.txt")
来源：http://jyn.zhixingplan.top

C#:   File.Delete("a.txt");
来源：http://eix.yj20258888.top

[F07] 创建目录（含多级）
来源：http://crx.aizwys.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lmv.yueranfly.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://iyw.aibaodan.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hsz.jinyuanbaomall.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hlc.nanxuanxn.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ady.fzhhl.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jgp.nanxinkj.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wvy.zhiwuduotai.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://iiz.xziqi.cn

[F08] 遍历目录
来源：http://shk.jqgfzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://tvq.cheryme.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://eyb.zdqjudy.top

JS:   fs.readdirSync("dir")
来源：http://tjd.jinghuilouyu.cn

TS:   fs.readdirSync("dir")
来源：http://wox.zhongyouzk.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kga.xingfuxueyuan.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://zkd.jinyuanbaomall.cn

Ruby: Dir.children("dir")
来源：http://azz.hywenlv.cn

C#:   Directory.GetFiles("dir")
来源：http://vox.hcnkem.com

[F09] 获取文件大小
来源：http://vum.c1oappe.top

Py:   os.path.getsize("a.txt")
来源：http://emn.ybcxt.top

PHP:  filesize("a.txt");
来源：http://uyq.kuanghao11.cn

JS:   fs.statSync("a.txt").size
来源：http://aob.dashuyun.cn

TS:   fs.statSync("a.txt").size
来源：http://jau.sysykeji.top

Java: Files.size(Path.of("a.txt"))
来源：http://iqd.jiagoushi.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qdf.hammf.cn

Ruby: File.size("a.txt")
来源：http://awz.vehdjk.com

C#:   new FileInfo("a.txt").Length
来源：http://zlt.uphjek.com

[F10] 取文件扩展名 / 文件名
来源：http://ssv.xingfuxueyuan.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kcu.pycfn.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mnu.hcnkem.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://puz.gogol.net.cn

TS:   path.extname("a.txt")
来源：http://sil.zhoulong.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lto.yongpay.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rlq.hongshengwenyu.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://iaa.xuetiantiany.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qza.mhx1999.top

[F11] 复制与移动文件
来源：http://ejt.gaohongyu789.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kwt.hnxiangtu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uzp.fanxiaobao.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yko.tanke756.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eta.snrcjt.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mdb.hnqzz.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hig.gaohongyu789.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yqh.nanxinkj.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rvj.smart0.xyz

[F12] CSV 读写
来源：http://eoa.meibo888.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bfl.xuanzx.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bhz.cashguo.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gpe.haohaochexian.top

TS:   // 同上
来源：http://hqd.xinyue.icu

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nfq.guannengcc.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://awt.epnwcf.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zkp.nanxinkj.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ded.jqgufenzy.top

================================================================================
来源：http://oym.andypj.xyz

G. 面向对象
来源：http://ixt.cdnleiting.top

================================================================================
来源：http://cfe.fanxiaobao.xyz

[G01] 定义类
来源：http://coj.gotoacloud.top

Py:   class User: pass
来源：http://lsu.yangfankeji.com

PHP:  class User {}
来源：http://yuf.aibaodan.cn

JS:   class User {}
来源：http://boe.dianchejie.cn

TS:   class User { name: string = ""; }
来源：http://wvn.jinqigfzy.top

Java: class User {}
来源：http://gsx.jiagoushi.top

Go:   type User struct { Name string }
来源：http://bus.pycfn.com

Ruby: class User; end
来源：http://irk.yueranfly.top

C#:   class User {}
来源：http://ejt.zhixingplan.top

[G02] 构造函数
来源：http://wao.haohaochexian.top

Py:   def __init__(self, name): self.name = name
来源：http://uih.yvedp.cn

PHP:  public function __construct(public string $name) {}
来源：http://tnf.yuxming.cn

JS:   constructor(name) { this.name = name; }
来源：http://xuo.feifeiyinyue.top

TS:   constructor(public name: string) {}
来源：http://ysf.fehbvm.com

Java: User(String name) { this.name = name; }
来源：http://scb.daria6918.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yrt.shanyushiyangkeji.top

Ruby: def initialize(name); @name = name; end
来源：http://ikp.xinyue.icu

C#:   public User(string name) { Name = name; }
来源：http://tug.hammf.cn

[G03] 实例属性
来源：http://ptx.cdnleiting.top

Py:   self.name = "x"
来源：http://eeb.guowangkeji.top

PHP:  public string $name = "x";
来源：http://oju.jianghu66.top

JS:   this.name = "x";
来源：http://eky.yuxming.cn

TS:   name: string = "x";
来源：http://brr.jianghu66.top

Java: private String name;
来源：http://yhd.meibo888.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tzm.yonumen.top

Ruby: @name = "x"
来源：http://qnx.yueranfly.top

C#:   public string Name { get; set; } = "x";
来源：http://rer.ywan-chungtsiang.top

[G04] 定义方法
来源：http://iix.jianghu66.top

Py:   def greet(self): return self.name
来源：http://niv.zycfv.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://uzv.daxiang520.top

JS:   greet() { return this.name; }
来源：http://wea.cashguo.top

TS:   greet(): string { return this.name; }
来源：http://pdw.ybcxt.top

Java: String greet() { return name; }
来源：http://lwd.pengpengdd.cyou

Go:   func (u User) Greet() string { return u.Name }
来源：http://tbo.cashguo.top

Ruby: def greet; @name; end
来源：http://cgd.ppjwa.cn

C#:   public string Greet() => Name;
来源：http://afe.zhaomingkeji.xyz

[G05] 继承
来源：http://ges.0kj1m.cn

Py:   class Admin(User): pass
来源：http://emw.c1oappe.top

PHP:  class Admin extends User {}
来源：http://nxm.tianlin.xyz

JS:   class Admin extends User {}
来源：http://jnp.yangfankeji.com

TS:   class Admin extends User {}
来源：http://yew.ywan-chungtsiang.top

Java: class Admin extends User {}
来源：http://mpe.hongshengwenyu.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://skw.gotoacloud.top

Ruby: class Admin < User; end
来源：http://twd.haohaochexian.top

C#:   class Admin : User {}
来源：http://zks.52xcode.cn

[G06] 重写方法
来源：http://vnl.jinqigfzy.top

Py:   def greet(self): return "admin"
来源：http://sio.havefunace.top

PHP:  public function greet(): string { return "admin"; }
来源：http://bix.52xcode.cn

JS:   greet() { return "admin"; }
来源：http://mcs.c1oappe.top

TS:   greet(): string { return "admin"; }
来源：http://yox.jlsjyb.cn

Java: @Override String greet() { return "admin"; }
来源：http://azo.hesvh.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://erp.hywenlv.cn

Ruby: def greet; "admin"; end
来源：http://ljz.ywan-chungtsiang.top

C#:   public override string Greet() => "admin";
来源：http://tic.zhixingplan.top

[G07] 调用父类方法
来源：http://alo.guannengcc.top

Py:   super().greet()
来源：http://fsl.jyoumei.cn

PHP:  parent::greet();
来源：http://vxn.jinghuilouyu.cn

JS:   super.greet();
来源：http://bjw.yueranfly.top

TS:   super.greet();
来源：http://kab.uphjek.com

Java: super.greet();
来源：http://pmo.hysaishi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://eno.xziqi.cn

Ruby: super
来源：http://zuz.shangyingyoupin.top

C#:   base.Greet();
来源：http://qqh.aizwys.cn

[G08] 静态方法与属性
来源：http://dpr.cqqwz.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pwd.sjlbkw.cn

PHP:  public static function f() {}
来源：http://ald.daria6918.cn

JS:   static f() {}
来源：http://kkr.bjfxy.top

TS:   static f(): void {}
来源：http://yln.gotoacloud.top

Java: static void f() {}
来源：http://hlg.yanxiufei.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://coy.sxryk.cn

Ruby: def self.f; end
来源：http://kfc.ybcxt.top

C#:   public static void F() {}
来源：http://dbg.wangdashe.top

[G09] 接口 / 抽象类
来源：http://itb.xylfe.cn

Py:   from abc import ABC, abstractmethod
来源：http://jkv.hnqzz.top

PHP:  interface Shape { public function area(): float; }
来源：http://knp.ehwqpu.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://iot.yj20258888.top

TS:   interface Shape { area(): number; }
来源：http://fxc.andypj.xyz

Java: interface Shape { double area(); }
来源：http://ubb.guowangkeji.top

Go:   type Shape interface { Area() float64 }
来源：http://orc.iojbl.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ero.316326.xyz

C#:   interface IShape { double Area(); }
来源：http://ufp.epnwcf.com

[G10] 访问控制
来源：http://vnu.ywan-chungtsiang.top

Py:   约定 _protected / __private（不强制）
来源：http://kvd.yanxiufei.cn

PHP:  public / protected / private
来源：http://rwq.fehbvm.com

JS:   #private 字段；其余公开
来源：http://zos.zdbjq.cn

TS:   public / protected / private
来源：http://mrz.zhiwuduotai.top

Java: public / protected / private / 默认包级
来源：http://iin.yj202588.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://nqs.zhongyouzk.top

Ruby: public / protected / private
来源：http://ebk.ywan-chungtsiang.top

C#:   public / protected / private / internal
来源：http://lmc.gaohongyu789.top

[G11] getter / setter
来源：http://uci.nwbrower.top

Py:   @property 与 @x.setter
来源：http://vdf.sjlbkw.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://hiz.hongshengwenyu.top

JS:   get name() { return this._name; }
来源：http://ohd.0kj1m.cn

TS:   get name(): string { return this._name; }
来源：http://uvx.shangyingyoupin.top

Java: public String getName() { return name; }
来源：http://fhu.uphjek.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://hgy.ppjwa.cn

Ruby: attr_accessor :name
来源：http://oyw.nanxuanxn.top

C#:   public string Name { get; set; }
来源：http://xbp.feifeiyinyue.top

[G12] 对象转字符串
来源：http://aoj.ivvv.top

Py:   def __str__(self): return self.name
来源：http://mco.redwolf501.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://rvu.ybcxt.top

JS:   toString() { return this.name; }
来源：http://img.sweek.top

TS:   toString(): string { return this.name; }
来源：http://cxj.ydjk.org.cn

Java: @Override public String toString() { return name; }
来源：http://lpp.ivvv.top

Go:   func (u User) String() string { return u.Name }
来源：http://owj.ehwqpu.com

Ruby: def to_s; @name; end
来源：http://afd.yonumen.top

C#:   public override string ToString() => Name;
来源：http://xkf.sysykeji.top

[G13] 判断对象类型
来源：http://ctq.hesvh.cn

Py:   isinstance(u, User)
来源：http://yvy.sweek.top

PHP:  $u instanceof User
来源：http://bpb.daxiang520.top

JS:   u instanceof User
来源：http://jtj.sufxvd.cn

TS:   u instanceof User
来源：http://rbr.nwbrower.top

Java: u instanceof User
来源：http://toh.gogol.net.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zlg.jinghuilouyu.cn

Ruby: u.is_a?(User)
来源：http://vyw.hammf.cn

C#:   u is User
来源：http://nao.vehdjk.com

[G14] 数据类 / record
来源：http://ldm.ydzc1.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hks.uphjek.com

PHP:  // 用 readonly 属性模拟
来源：http://xmx.jinghuilouyu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://lvk.xinyue.icu

TS:   type User = { name: string; age: number };
来源：http://qvz.jianghu66.top

Java: record User(String name, int age) {}
来源：http://clj.hesvh.cn

Go:   type User struct { Name string; Age int }
来源：http://ptd.gzhubu.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://syk.xuetiantiany.cn

C#:   record User(string Name, int Age);
来源：http://brd.fengsongda.top

[G15] 枚举
来源：http://qqt.dianchejie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://uvg.fehbvm.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://mkz.yongpay.top


<!-- 参考信息 -->