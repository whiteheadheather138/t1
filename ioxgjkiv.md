代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xev.xziqi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pfr.ydjk.org.cn

Ruby: s.capitalize
来源：http://ohp.shanyushiyangkeji.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wza.daria6918.cn

[E18] 模板占位符替换
来源：http://cba.yuxming.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://koc.dianchejie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://czy.jqgufenzy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://fcg.zdbjq.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jen.vehdjk.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rbg.gogol.net.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://uyt.daria6918.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mfa.zhoulong.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cml.daria6918.cn

[E19] 多行文本按行拆分
来源：http://hcz.nanxuanxn.top

Py:   s.splitlines()
来源：http://wmx.yuxming.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gfz.zhiwuduotai.top

JS:   s.split(/\r?\n/)
来源：http://svq.smart0.xyz

TS:   s.split(/\r?\n/)
来源：http://opw.hongshengwenyu.top

Java: s.lines().toList()
来源：http://pet.nwbrower.top

Go:   strings.Split(s, "\n")
来源：http://lxb.hesvh.cn

Ruby: s.lines
来源：http://sds.uphjek.com

C#:   s.Split('\n')
来源：http://mut.sysykeji.top

[E20] 判断字符串是否为空
来源：http://ond.zdqjudy.top

Py:   if not s:
来源：http://rcl.yvedp.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mzq.tian-w.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qwr.jqgufenzy.top

TS:   if (s === "") {}
来源：http://acr.zhixingplan.top

Java: if (s.isEmpty()) {}
来源：http://gmm.andypj.xyz

Go:   if s == "" {}
来源：http://qsc.daria6918.cn

Ruby: if s.empty?
来源：http://msi.zdbjq.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lle.tanke756.top

[E21] 超长截断加省略号
来源：http://ecm.xinyue.icu

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qoi.yangfankeji.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nmv.sufxvd.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qdy.shanyushiyangkeji.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ziz.jinghuilouyu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gge.sweek.top

Go:   // 按 rune 判断长度后截断
来源：http://mya.tarul.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://aca.haohaochexian.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kyo.fanxiaobao.xyz

[E22] 字节长度与字符长度
来源：http://frn.cashguo.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bgm.jianghu66.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tgp.tian-w.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xch.jiagoushi.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rpd.ctjpmb.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wzi.ctjpmb.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fno.bjfxy.top

Ruby: s.bytesize;  s.length
来源：http://bdy.jinqigufen.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ecz.shanyushiyangkeji.top

================================================================================
来源：http://idb.shzxlz.cn

F. 文件与目录
来源：http://thv.zhengqikj.top

================================================================================
来源：http://viq.sjlbkw.cn

[F01] 读取整个文件
来源：http://xgf.hongshengwenyu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tpt.andypj.xyz

PHP:  file_get_contents("a.txt");
来源：http://zdf.dianchejie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://omb.cucudq.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://npz.ivvv.top

Java: Files.readString(Path.of("a.txt"))
来源：http://jgc.meibo888.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://whp.dashuyun.cn

Ruby: File.read("a.txt")
来源：http://nws.jqgufenzy.top

C#:   File.ReadAllText("a.txt");
来源：http://mgb.fzhhl.top

[F02] 逐行读取文件
来源：http://iwz.hywenlv.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zbw.cucudq.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://akr.shuidangran.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://glu.yj20258.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ihd.chenzaomai.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bgb.dashuyun.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yeb.nanxinkj.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tmz.hnxiangtu.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://quy.pengpengdd.cyou

[F03] 写入文件（覆盖）
来源：http://moy.tanke756.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zqu.gaohongyu789.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://mis.52xcode.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qty.vehdjk.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ahr.xuanzx.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bvv.zhengqikj.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://scc.ivvv.top

Ruby: File.write("a.txt", "hi")
来源：http://ebk.redwolf501.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lqc.guowangkeji.top

[F04] 追加写入文件
来源：http://hve.vehdjk.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lhx.fehbvm.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nyi.yuanzhike.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sgg.hesvh.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zcr.sufxvd.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mbc.hnqzz.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ili.sxryk.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lzz.guannengcc.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qnb.pycfn.com

[F05] 判断文件或目录是否存在
来源：http://whv.dianchejie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qpw.tianlin.xyz

PHP:  file_exists("a.txt");
来源：http://hmc.yj20258888.top

JS:   fs.existsSync("a.txt")
来源：http://yob.sufxvd.cn

TS:   fs.existsSync("a.txt")
来源：http://dim.redwolf501.top

Java: Files.exists(Path.of("a.txt"))
来源：http://isp.jinyuanbaomall.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ysa.yuanzhike.top

Ruby: File.exist?("a.txt")
来源：http://ujp.guannengcc.top

C#:   File.Exists("a.txt")
来源：http://pfb.dianchejie.cn

[F06] 删除文件
来源：http://fuf.xingfuxueyuan.xyz

Py:   os.remove("a.txt")
来源：http://pwk.gaohongyu789.top

PHP:  unlink("a.txt");
来源：http://axo.gotoacloud.top

JS:   fs.unlinkSync("a.txt")
来源：http://ryz.guowangkeji.top

TS:   fs.unlinkSync("a.txt")
来源：http://jpl.zhengqikj.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dsj.uphjek.com

Go:   os.Remove("a.txt")
来源：http://iuu.jinqigufen.top

Ruby: File.delete("a.txt")
来源：http://ece.ivvv.top

C#:   File.Delete("a.txt");
来源：http://ggj.jiagoushi.top

[F07] 创建目录（含多级）
来源：http://sjh.zhiwuduotai.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://con.ywan-chungtsiang.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://abo.sjlbkw.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dyj.daria6918.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tzk.jianghu66.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lpn.yonumen.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://eqr.xinyue.icu

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://loc.gotoacloud.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://osz.ydjk.org.cn

[F08] 遍历目录
来源：http://twm.feifeiyinyue.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://chc.jinyuanbaomall.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sgk.jiagoushi.top

JS:   fs.readdirSync("dir")
来源：http://ysw.yonumen.top

TS:   fs.readdirSync("dir")
来源：http://qts.gaohongyu789.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yrd.jinqigufen.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://utv.yonumen.top

Ruby: Dir.children("dir")
来源：http://mza.chenzaomai.com

C#:   Directory.GetFiles("dir")
来源：http://qdk.sufxvd.cn

[F09] 获取文件大小
来源：http://imu.nanxuanxn.top

Py:   os.path.getsize("a.txt")
来源：http://gvb.zhongyouzk.top

PHP:  filesize("a.txt");
来源：http://rsz.quarkkingdee.top

JS:   fs.statSync("a.txt").size
来源：http://fuk.uphjek.com

TS:   fs.statSync("a.txt").size
来源：http://hsh.smart0.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://elm.meibo888.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://uxa.mhx1999.top

Ruby: File.size("a.txt")
来源：http://mqt.zdqjudy.top

C#:   new FileInfo("a.txt").Length
来源：http://qef.cashguo.top

[F10] 取文件扩展名 / 文件名
来源：http://fwk.ivvv.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xhp.guowangkeji.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hob.jqgufenzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qoj.mhx1999.top

TS:   path.extname("a.txt")
来源：http://khh.jqgufenzy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pfn.xylfe.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ktf.birdmap.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dlx.xuanzx.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://moq.zhiwuduotai.top

[F11] 复制与移动文件
来源：http://ccw.wangshuangyany.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zna.hammf.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cwx.xuanzx.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dto.wangdashe.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://esl.cashguo.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lav.ppjwa.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rzt.fanxiaobao.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zab.haohaochexian.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qya.bbcook.cn

[F12] CSV 读写
来源：http://zyq.chenjidiqi.icu

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qlu.fktsv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://aoi.xuetiantiany.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zfz.cheryme.top

TS:   // 同上
来源：http://zmm.zhengqikj.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ujw.hfpthk.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vvq.ctjpmb.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fvs.jlsjyb.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://xhr.yanxiufei.cn

================================================================================
来源：http://efs.havefunace.top

G. 面向对象
来源：http://pxv.shzxlz.cn

================================================================================
来源：http://xet.yvedp.cn

[G01] 定义类
来源：http://dvm.dianchejie.cn

Py:   class User: pass
来源：http://udu.chenzaomai.com

PHP:  class User {}
来源：http://sug.jqgufenzy.top

JS:   class User {}
来源：http://ahe.jinyuanbaomall.cn

TS:   class User { name: string = ""; }
来源：http://ttf.yuanzhike.top

Java: class User {}
来源：http://wby.xinyue.icu

Go:   type User struct { Name string }
来源：http://bbq.cdnleiting.top

Ruby: class User; end
来源：http://hoh.yj20258888.top

C#:   class User {}
来源：http://qom.hywenlv.cn

[G02] 构造函数
来源：http://kry.xziqi.cn

Py:   def __init__(self, name): self.name = name
来源：http://xyh.guannengcc.top

PHP:  public function __construct(public string $name) {}
来源：http://paw.jianghu66.top

JS:   constructor(name) { this.name = name; }
来源：http://ovx.jinqigufen.top

TS:   constructor(public name: string) {}
来源：http://fwr.fengsongda.top

Java: User(String name) { this.name = name; }
来源：http://jqm.ctjpmb.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rlq.gzhubu.top

Ruby: def initialize(name); @name = name; end
来源：http://dba.shanyushiyangkeji.top

C#:   public User(string name) { Name = name; }
来源：http://fvl.sysykeji.top

[G03] 实例属性
来源：http://vje.zhijiandao.cn

Py:   self.name = "x"
来源：http://zaq.zhongyouzk.top

PHP:  public string $name = "x";
来源：http://oje.svipenyu.cn

JS:   this.name = "x";
来源：http://fml.fanxiaobao.xyz

TS:   name: string = "x";
来源：http://jai.sxryk.cn

Java: private String name;
来源：http://vxs.fktsv.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pfm.mhx1999.top

Ruby: @name = "x"
来源：http://vqs.ctjpmb.com

C#:   public string Name { get; set; } = "x";
来源：http://wlp.jqgufenzy.top

[G04] 定义方法
来源：http://faz.9152youxi.cn

Py:   def greet(self): return self.name
来源：http://bkv.bjfxy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://cxd.ppjwa.cn

JS:   greet() { return this.name; }
来源：http://ltc.hnqzz.top

TS:   greet(): string { return this.name; }
来源：http://zlr.hesvh.cn

Java: String greet() { return name; }
来源：http://xoh.yj20258888.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://qhc.meibo888.top

Ruby: def greet; @name; end
来源：http://twy.yvedp.cn

C#:   public string Greet() => Name;
来源：http://jnv.zhixingplan.top

[G05] 继承
来源：http://sgi.gotoacloud.top

Py:   class Admin(User): pass
来源：http://hbh.shzxlz.cn

PHP:  class Admin extends User {}
来源：http://zxa.svipenyu.cn

JS:   class Admin extends User {}
来源：http://xvc.yj20258.top

TS:   class Admin extends User {}
来源：http://mer.ctjpmb.com

Java: class Admin extends User {}
来源：http://nlk.sxryk.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://czg.zhaomingkeji.xyz

Ruby: class Admin < User; end
来源：http://vlc.ehwqpu.com

C#:   class Admin : User {}
来源：http://eav.sxryk.cn

[G06] 重写方法
来源：http://hmi.bjfxy.top

Py:   def greet(self): return "admin"
来源：http://srj.epnwcf.com

PHP:  public function greet(): string { return "admin"; }
来源：http://qyp.xuetiantiany.cn

JS:   greet() { return "admin"; }
来源：http://xjn.meibo888.top

TS:   greet(): string { return "admin"; }
来源：http://msq.jianghu66.top

Java: @Override String greet() { return "admin"; }
来源：http://ctn.zhijiandao.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vdn.nwbrower.top

Ruby: def greet; "admin"; end
来源：http://ush.nanxuanxn.top

C#:   public override string Greet() => "admin";
来源：http://kue.guowangkeji.top

[G07] 调用父类方法
来源：http://ivg.316326.xyz

Py:   super().greet()
来源：http://ium.ydzc1.top

PHP:  parent::greet();
来源：http://udq.xuetiantiany.cn

JS:   super.greet();
来源：http://wlo.meibo888.top

TS:   super.greet();
来源：http://uam.sjlbkw.cn

Java: super.greet();
来源：http://isr.ywan-chungtsiang.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ayj.dashuyun.cn

Ruby: super
来源：http://eyl.gzhubu.top

C#:   base.Greet();
来源：http://dpe.andypj.xyz

[G08] 静态方法与属性
来源：http://shd.daria6918.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qlb.fanxiaobao.xyz

PHP:  public static function f() {}
来源：http://tzj.daxiang520.top

JS:   static f() {}
来源：http://bfw.xingfuxueyuan.xyz

TS:   static f(): void {}
来源：http://mkl.shangyingyoupin.top

Java: static void f() {}
来源：http://gda.birdmap.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://tmp.shuidangran.top

Ruby: def self.f; end
来源：http://fch.zhixingplan.top

C#:   public static void F() {}
来源：http://qbt.ehwqpu.com

[G09] 接口 / 抽象类
来源：http://pxs.gaohongyu789.top

Py:   from abc import ABC, abstractmethod
来源：http://xgr.wangdashe.top

PHP:  interface Shape { public function area(): float; }
来源：http://pnb.zhixingplan.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://zqz.yuxming.cn

TS:   interface Shape { area(): number; }
来源：http://tdx.0kj1m.cn

Java: interface Shape { double area(); }
来源：http://btf.gzhubu.top

Go:   type Shape interface { Area() float64 }
来源：http://jsj.snrcjt.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tky.zhongyouzk.top

C#:   interface IShape { double Area(); }
来源：http://ogr.shuidangran.top

[G10] 访问控制
来源：http://ikr.tianlin.xyz

Py:   约定 _protected / __private（不强制）
来源：http://ell.shanyushiyangtech.top

PHP:  public / protected / private
来源：http://nvd.hammf.cn

JS:   #private 字段；其余公开
来源：http://ril.0kj1m.cn

TS:   public / protected / private
来源：http://wfp.redwolf501.top

Java: public / protected / private / 默认包级
来源：http://qwu.meibo888.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qer.smart0.xyz

Ruby: public / protected / private
来源：http://gik.yvedp.cn

C#:   public / protected / private / internal
来源：http://kbr.zhengqikj.top

[G11] getter / setter
来源：http://pht.iojbl.cn

Py:   @property 与 @x.setter
来源：http://kcf.52xcode.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ahe.shanyushiyangtech.top

JS:   get name() { return this._name; }
来源：http://szd.jlsjyb.cn

TS:   get name(): string { return this._name; }
来源：http://qpf.ydjk.org.cn

Java: public String getName() { return name; }
来源：http://nmi.jianghu66.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://lnh.yongpay.top

Ruby: attr_accessor :name
来源：http://gsk.sweek.top

C#:   public string Name { get; set; }
来源：http://ahc.jyoumei.cn

[G12] 对象转字符串
来源：http://yaj.yj20258888.top

Py:   def __str__(self): return self.name
来源：http://cwt.chenlongwang.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://sbm.ywan-chungtsiang.top

JS:   toString() { return this.name; }
来源：http://wak.aibaodan.cn

TS:   toString(): string { return this.name; }
来源：http://bde.gaohongyu789.top

Java: @Override public String toString() { return name; }
来源：http://uav.quarkkingdee.top

Go:   func (u User) String() string { return u.Name }
来源：http://mng.ehwqpu.com

Ruby: def to_s; @name; end
来源：http://bdh.havefunace.top

C#:   public override string ToString() => Name;
来源：http://fcc.316326.xyz

[G13] 判断对象类型
来源：http://ffq.jinghuilouyu.cn

Py:   isinstance(u, User)
来源：http://wyd.jinyuanbaomall.cn

PHP:  $u instanceof User
来源：http://hao.zhaomingkeji.xyz

JS:   u instanceof User
来源：http://qjx.xuanzx.com

TS:   u instanceof User
来源：http://zxg.gogol.net.cn

Java: u instanceof User
来源：http://mgy.zhoulong.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://ldv.zhaomingkeji.xyz

Ruby: u.is_a?(User)
来源：http://oab.nanxinkj.top

C#:   u is User
来源：http://ont.yvedp.cn

[G14] 数据类 / record
来源：http://fdj.ivvv.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dlm.sweek.top

PHP:  // 用 readonly 属性模拟
来源：http://dkr.vehdjk.com

JS:   // 无内置：普通类或对象字面量
来源：http://wma.tianlin.xyz

TS:   type User = { name: string; age: number };
来源：http://dmm.vqdsnc.cn

Java: record User(String name, int age) {}
来源：http://law.nanxuanxn.top

Go:   type User struct { Name string; Age int }
来源：http://wwe.yongpay.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cft.hnqzz.top

C#:   record User(string Name, int Age);
来源：http://ngx.yuxming.cn

[G15] 枚举
来源：http://yxg.zhiwuduotai.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dwp.yongpay.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://yxz.gotoacloud.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sfa.hysaishi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zxj.gzhubu.top

Java: enum Color { RED, GREEN }
来源：http://jgn.xuetiantiany.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://eiz.hnxiangtu.top

Ruby: Color = %i[red green].freeze
来源：http://ykf.shangyingyoupin.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ubn.tian-w.cn

[G16] 对象转数组 / 字典
来源：http://vip.hnxiangtu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lfb.redwolf501.top


<!-- 参考信息 -->