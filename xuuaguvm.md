代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://dlo.jinqigufen.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gbo.shanyushiyangtech.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jnb.gaohongyu789.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ggt.pycfn.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hrw.zhiwuduotai.top

[E19] 多行文本按行拆分
来源：http://oqk.yangfankeji.com

Py:   s.splitlines()
来源：http://tyq.yuxming.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yeh.guowangkeji.top

JS:   s.split(/\r?\n/)
来源：http://xib.xuanzx.com

TS:   s.split(/\r?\n/)
来源：http://tzt.vqdsnc.cn

Java: s.lines().toList()
来源：http://rmu.ybcxt.top

Go:   strings.Split(s, "\n")
来源：http://ipt.pycfn.com

Ruby: s.lines
来源：http://mfc.zhengqikj.top

C#:   s.Split('\n')
来源：http://flu.birdmap.top

[E20] 判断字符串是否为空
来源：http://lug.vehdjk.com

Py:   if not s:
来源：http://wsh.yfazqb.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jem.cucudq.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jbb.feifeiyinyue.top

TS:   if (s === "") {}
来源：http://ptl.hesvh.cn

Java: if (s.isEmpty()) {}
来源：http://gtt.sweek.top

Go:   if s == "" {}
来源：http://wyz.fzhhl.top

Ruby: if s.empty?
来源：http://itz.ehwqpu.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jsd.zhongyouzk.top

[E21] 超长截断加省略号
来源：http://mkd.shuidangran.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://afr.wangdashe.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zdh.guowangkeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baq.tian-w.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ryr.9152youxi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cof.zdqjudy.top

Go:   // 按 rune 判断长度后截断
来源：http://czf.ydjk.org.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://thy.yuxming.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jrt.sxryk.cn

[E22] 字节长度与字符长度
来源：http://agi.feifeiyinyue.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jwk.tianlin.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qij.guannengcc.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xli.daria6918.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qef.ydjk.org.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mge.xinyue.icu

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zpc.shzxlz.cn

Ruby: s.bytesize;  s.length
来源：http://wef.ehwqpu.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ujp.ybcxt.top

================================================================================
来源：http://dsn.uphjek.com

F. 文件与目录
来源：http://trs.cdnleiting.top

================================================================================
来源：http://wlt.ctjpmb.com

[F01] 读取整个文件
来源：http://jxc.haohaochexian.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rdc.jyoumei.cn

PHP:  file_get_contents("a.txt");
来源：http://wqz.jqgufenzy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pcx.c1oappe.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://koa.pengpengdd.cyou

Java: Files.readString(Path.of("a.txt"))
来源：http://elp.nanxinkj.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gxb.fehbvm.com

Ruby: File.read("a.txt")
来源：http://bjc.mhx1999.top

C#:   File.ReadAllText("a.txt");
来源：http://gdy.zhixingplan.top

[F02] 逐行读取文件
来源：http://lxf.fktsv.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://djh.xinyue.icu

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ndg.jyoumei.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hez.ydjk.org.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pyk.haohaochexian.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mkt.52xcode.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wuv.jlsjyb.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wcy.aizwys.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nie.zhiwuduotai.top

[F03] 写入文件（覆盖）
来源：http://cog.pycfn.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baz.cheryme.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://klp.jinqigufen.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sfw.pengpengdd.cyou

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://soy.yongpay.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qaf.uphjek.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fhp.redwolf501.top

Ruby: File.write("a.txt", "hi")
来源：http://wsl.jinghuilouyu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mxz.uphjek.com

[F04] 追加写入文件
来源：http://siy.zhoulong.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jsa.guowangkeji.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sbc.sysykeji.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wcp.daria6918.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lke.zhijiandao.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://msq.zdbjq.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yld.aizwys.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kmn.dianchejie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lin.zhixingplan.top

[F05] 判断文件或目录是否存在
来源：http://juz.aizwys.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qln.havefunace.top

PHP:  file_exists("a.txt");
来源：http://vvz.zhongyouzk.top

JS:   fs.existsSync("a.txt")
来源：http://jdm.9152youxi.cn

TS:   fs.existsSync("a.txt")
来源：http://trj.jianghu66.top

Java: Files.exists(Path.of("a.txt"))
来源：http://crx.52xcode.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://omy.pengpengdd.cyou

Ruby: File.exist?("a.txt")
来源：http://bvp.yj20258.top

C#:   File.Exists("a.txt")
来源：http://lwa.chenlongwang.top

[F06] 删除文件
来源：http://rvr.bjfxy.top

Py:   os.remove("a.txt")
来源：http://mdu.yanxiufei.cn

PHP:  unlink("a.txt");
来源：http://pex.haohaochexian.top

JS:   fs.unlinkSync("a.txt")
来源：http://fiw.cheryme.top

TS:   fs.unlinkSync("a.txt")
来源：http://wuv.vqdsnc.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vic.jinghuilouyu.cn

Go:   os.Remove("a.txt")
来源：http://vml.9152youxi.cn

Ruby: File.delete("a.txt")
来源：http://pdu.kuanghao11.cn

C#:   File.Delete("a.txt");
来源：http://wxs.aibaodan.cn

[F07] 创建目录（含多级）
来源：http://szj.chenzaomai.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yhq.nwbrower.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://maj.chenlongwang.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zmv.pycfn.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mts.tanke756.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://agm.yueranfly.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ixr.fanxiaobao.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mur.epnwcf.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://heq.havefunace.top

[F08] 遍历目录
来源：http://yev.jianghu66.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://fyk.feifeiyinyue.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dax.yanxiufei.cn

JS:   fs.readdirSync("dir")
来源：http://zcb.jyoumei.cn

TS:   fs.readdirSync("dir")
来源：http://rfi.tanke756.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vlo.yueranfly.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://hts.yvedp.cn

Ruby: Dir.children("dir")
来源：http://oab.tanke756.top

C#:   Directory.GetFiles("dir")
来源：http://ito.snrcjt.cn

[F09] 获取文件大小
来源：http://ony.gotoacloud.top

Py:   os.path.getsize("a.txt")
来源：http://hyx.yonumen.top

PHP:  filesize("a.txt");
来源：http://tao.jinqigufen.top

JS:   fs.statSync("a.txt").size
来源：http://vqe.quarkkingdee.top

TS:   fs.statSync("a.txt").size
来源：http://bid.kuanghao11.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mna.redwolf501.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://khh.yanxiufei.cn

Ruby: File.size("a.txt")
来源：http://bns.nanxinkj.top

C#:   new FileInfo("a.txt").Length
来源：http://qqz.hysaishi.cn

[F10] 取文件扩展名 / 文件名
来源：http://kej.52xcode.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hzg.xinyue.icu

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ius.xuanzx.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bos.aibaodan.cn

TS:   path.extname("a.txt")
来源：http://dbn.gzhubu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vas.cheryme.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vpb.yfazqb.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sba.bjfxy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pgh.chenzaomai.com

[F11] 复制与移动文件
来源：http://xam.xuetiantiany.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xvr.feifeiyinyue.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://csc.zhaomingkeji.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tyy.nwbrower.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gny.chenlongwang.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hvf.aibaodan.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bgx.ywan-chungtsiang.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mxt.sxryk.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vor.quarkkingdee.top

[F12] CSV 读写
来源：http://fcl.zhaomingkeji.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ysc.guannengcc.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ica.jinyuanbaomall.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kmv.sxryk.cn

TS:   // 同上
来源：http://tgg.wangshuangyany.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qys.zhixingplan.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zij.52xcode.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ufx.yanxiufei.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ehi.gzhubu.top

================================================================================
来源：http://gay.wangdashe.top

G. 面向对象
来源：http://rni.guowangkeji.top

================================================================================
来源：http://cyo.sysykeji.top

[G01] 定义类
来源：http://zbi.zhiwuduotai.top

Py:   class User: pass
来源：http://xjv.fengsongda.top

PHP:  class User {}
来源：http://vub.jyoumei.cn

JS:   class User {}
来源：http://ekr.ctjpmb.com

TS:   class User { name: string = ""; }
来源：http://jlm.ivvv.top

Java: class User {}
来源：http://kwl.bjfxy.top

Go:   type User struct { Name string }
来源：http://cjj.aizwys.cn

Ruby: class User; end
来源：http://htv.chenzaomai.com

C#:   class User {}
来源：http://fxz.xuetiantiany.cn

[G02] 构造函数
来源：http://xjm.aibaodan.cn

Py:   def __init__(self, name): self.name = name
来源：http://jwv.yuxming.cn

PHP:  public function __construct(public string $name) {}
来源：http://ftq.dashuyun.cn

JS:   constructor(name) { this.name = name; }
来源：http://rnp.yangfankeji.com

TS:   constructor(public name: string) {}
来源：http://ari.jiagoushi.top

Java: User(String name) { this.name = name; }
来源：http://vbu.daria6918.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cmj.ivvv.top

Ruby: def initialize(name); @name = name; end
来源：http://itr.xziqi.cn

C#:   public User(string name) { Name = name; }
来源：http://jmh.nanxinkj.top

[G03] 实例属性
来源：http://mie.hammf.cn

Py:   self.name = "x"
来源：http://ltw.zhoulong.xyz

PHP:  public string $name = "x";
来源：http://yzh.yj20258.top

JS:   this.name = "x";
来源：http://bkx.wangdashe.top

TS:   name: string = "x";
来源：http://nme.hongshengwenyu.top

Java: private String name;
来源：http://tbp.vqdsnc.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dcq.zhixingplan.top

Ruby: @name = "x"
来源：http://zfg.daria6918.cn

C#:   public string Name { get; set; } = "x";
来源：http://gwp.sysykeji.top

[G04] 定义方法
来源：http://hvq.pycfn.com

Py:   def greet(self): return self.name
来源：http://ogh.0kj1m.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ccl.cucudq.cn

JS:   greet() { return this.name; }
来源：http://txy.gotoacloud.top

TS:   greet(): string { return this.name; }
来源：http://tal.sufxvd.cn

Java: String greet() { return name; }
来源：http://efs.xuanzx.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://taz.zhongyouzk.top

Ruby: def greet; @name; end
来源：http://soq.jinqigfzy.top

C#:   public string Greet() => Name;
来源：http://ghw.gzhubu.top

[G05] 继承
来源：http://jwo.zhijiandao.cn

Py:   class Admin(User): pass
来源：http://vkv.zdqjudy.top

PHP:  class Admin extends User {}
来源：http://cfv.ivvv.top

JS:   class Admin extends User {}
来源：http://kqs.haohaochexian.top

TS:   class Admin extends User {}
来源：http://gnz.hfpthk.cn

Java: class Admin extends User {}
来源：http://ctq.zhengqikj.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pff.gaohongyu789.top

Ruby: class Admin < User; end
来源：http://avt.hammf.cn

C#:   class Admin : User {}
来源：http://ofg.wangdashe.top

[G06] 重写方法
来源：http://knz.meibo888.top

Py:   def greet(self): return "admin"
来源：http://ots.cashguo.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ujn.cucudq.cn

JS:   greet() { return "admin"; }
来源：http://fru.cheryme.top

TS:   greet(): string { return "admin"; }
来源：http://lxl.sweek.top

Java: @Override String greet() { return "admin"; }
来源：http://wae.wangdashe.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lau.yueranfly.top

Ruby: def greet; "admin"; end
来源：http://dfb.gzhubu.top

C#:   public override string Greet() => "admin";
来源：http://dhl.yfazqb.com

[G07] 调用父类方法
来源：http://hcf.nwbrower.top

Py:   super().greet()
来源：http://uub.c1oappe.top

PHP:  parent::greet();
来源：http://scr.zycfv.cn

JS:   super.greet();
来源：http://kih.xuanzx.com

TS:   super.greet();
来源：http://tbc.cucudq.cn

Java: super.greet();
来源：http://dkd.ctjpmb.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xew.yj202588.top

Ruby: super
来源：http://kre.shanyushiyangtech.top

C#:   base.Greet();
来源：http://iqm.mhx1999.top

[G08] 静态方法与属性
来源：http://aqs.yanxiufei.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ckc.yuanzhike.top

PHP:  public static function f() {}
来源：http://lau.ywan-chungtsiang.top

JS:   static f() {}
来源：http://lab.iojbl.cn

TS:   static f(): void {}
来源：http://uoj.sxryk.cn

Java: static void f() {}
来源：http://dyg.shuidangran.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://njb.hcnkem.com

Ruby: def self.f; end
来源：http://ijw.yongpay.top

C#:   public static void F() {}
来源：http://ocy.zhijiandao.cn

[G09] 接口 / 抽象类
来源：http://axs.xuetiantiany.cn

Py:   from abc import ABC, abstractmethod
来源：http://zfh.hesvh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dcx.ydzc1.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ltr.yj20258888.top

TS:   interface Shape { area(): number; }
来源：http://vjc.c1oappe.top

Java: interface Shape { double area(); }
来源：http://ghu.aibaodan.cn

Go:   type Shape interface { Area() float64 }
来源：http://auc.vqdsnc.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://utk.hysaishi.cn

C#:   interface IShape { double Area(); }
来源：http://xlp.yj202588.top

[G10] 访问控制
来源：http://oqo.jlsjyb.cn

Py:   约定 _protected / __private（不强制）
来源：http://dhf.hongshengwenyu.top

PHP:  public / protected / private
来源：http://eab.chenzaomai.com

JS:   #private 字段；其余公开
来源：http://tnu.chenzaomai.com

TS:   public / protected / private
来源：http://rmx.yfazqb.com

Java: public / protected / private / 默认包级
来源：http://wbj.fktsv.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://zlw.0kj1m.cn

Ruby: public / protected / private
来源：http://esb.yuxming.cn

C#:   public / protected / private / internal
来源：http://dbu.yj20258888.top

[G11] getter / setter
来源：http://rhm.0kj1m.cn

Py:   @property 与 @x.setter
来源：http://lpx.fanxiaobao.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://tzp.hywenlv.cn

JS:   get name() { return this._name; }
来源：http://vne.hfpthk.cn

TS:   get name(): string { return this._name; }
来源：http://xwa.ybcxt.top

Java: public String getName() { return name; }
来源：http://uav.iojbl.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://dgc.daria6918.cn

Ruby: attr_accessor :name
来源：http://npc.yj20258888.top

C#:   public string Name { get; set; }
来源：http://yvn.fanxiaobao.xyz

[G12] 对象转字符串
来源：http://zdv.smart0.xyz

Py:   def __str__(self): return self.name
来源：http://fua.hywenlv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://sfr.316326.xyz

JS:   toString() { return this.name; }
来源：http://lfy.mhx1999.top

TS:   toString(): string { return this.name; }
来源：http://xiy.zhaomingkeji.xyz

Java: @Override public String toString() { return name; }
来源：http://niv.fehbvm.com

Go:   func (u User) String() string { return u.Name }
来源：http://wfv.sxryk.cn

Ruby: def to_s; @name; end
来源：http://rgs.gogol.net.cn

C#:   public override string ToString() => Name;
来源：http://bfz.vqdsnc.cn

[G13] 判断对象类型
来源：http://jcw.52xcode.cn

Py:   isinstance(u, User)
来源：http://bpr.epnwcf.com

PHP:  $u instanceof User
来源：http://pew.pycfn.com

JS:   u instanceof User
来源：http://twe.tanke756.top

TS:   u instanceof User
来源：http://vuo.gzhubu.top

Java: u instanceof User
来源：http://smt.pycfn.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://piq.pycfn.com

Ruby: u.is_a?(User)
来源：http://pqc.shangyingyoupin.top

C#:   u is User
来源：http://vgq.fktsv.cn

[G14] 数据类 / record
来源：http://ess.ivvv.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://awz.ydzc1.top

PHP:  // 用 readonly 属性模拟
来源：http://sug.zdbjq.cn

JS:   // 无内置：普通类或对象字面量
来源：http://tiu.zhoulong.xyz

TS:   type User = { name: string; age: number };
来源：http://cjw.vqdsnc.cn

Java: record User(String name, int age) {}
来源：http://iuk.shuidangran.top

Go:   type User struct { Name string; Age int }
来源：http://vee.fktsv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wiv.fanxiaobao.xyz

C#:   record User(string Name, int Age);
来源：http://amn.yuxming.cn

[G15] 枚举
来源：http://pte.kuanghao11.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://suh.havefunace.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://sun.jyoumei.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yla.daria6918.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://esd.jinyuanbaomall.cn

Java: enum Color { RED, GREEN }
来源：http://bcl.ydzc1.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dbu.smart0.xyz

Ruby: Color = %i[red green].freeze
来源：http://bzy.fehbvm.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wzy.jianghu66.top

[G16] 对象转数组 / 字典
来源：http://fnt.hesvh.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wxu.hnqzz.top

PHP:  get_object_vars($obj);
来源：http://rrn.cqqwz.cn

JS:   Object.entries(obj)
来源：http://qex.daxiang520.top

TS:   Object.entries(obj)
来源：http://vni.hongshengwenyu.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kps.sufxvd.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://rdw.zhijiandao.cn

Ruby: obj.instance_variables
来源：http://vgo.zdbjq.cn

C#:   // 用反射或 System.Text.Json
来源：http://zsv.hnxiangtu.top

================================================================================
来源：http://ssy.hnqzz.top


<!-- 参考信息 -->