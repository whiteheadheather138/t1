代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mwi.andypj.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://luf.shangyingyoupin.top

Ruby: s.capitalize
来源：http://cjq.jinqigufen.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pvi.hammf.cn

[E18] 模板占位符替换
来源：http://xuw.zhaomingkeji.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ikt.ivvv.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lmd.52xcode.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://esm.shanyushiyangkeji.top

TS:   tpl.replaceAll("{name}", name)
来源：http://llv.zdqjudy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nnn.nanxuanxn.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ipg.shanyushiyangkeji.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qpb.daria6918.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vpy.c1oappe.top

[E19] 多行文本按行拆分
来源：http://khk.cheryme.top

Py:   s.splitlines()
来源：http://qns.xingfuxueyuan.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rtl.ydzc1.top

JS:   s.split(/\r?\n/)
来源：http://lsu.cucudq.cn

TS:   s.split(/\r?\n/)
来源：http://vwc.gogol.net.cn

Java: s.lines().toList()
来源：http://mpi.tarul.cn

Go:   strings.Split(s, "\n")
来源：http://frv.yj20258888.top

Ruby: s.lines
来源：http://tzf.c1oappe.top

C#:   s.Split('\n')
来源：http://czd.gzhubu.top

[E20] 判断字符串是否为空
来源：http://azt.zhixingplan.top

Py:   if not s:
来源：http://uik.gogol.net.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ghl.xziqi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://umv.tanke756.top

TS:   if (s === "") {}
来源：http://qhe.0kj1m.cn

Java: if (s.isEmpty()) {}
来源：http://ndc.yuanzhike.top

Go:   if s == "" {}
来源：http://naz.shuidangran.top

Ruby: if s.empty?
来源：http://vwx.wangshuangyany.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://npe.shzxlz.cn

[E21] 超长截断加省略号
来源：http://mrb.aizwys.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qqt.shanyushiyangtech.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ulv.ybcxt.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nbl.quarkkingdee.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eum.ydjk.org.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://why.mhx1999.top

Go:   // 按 rune 判断长度后截断
来源：http://ksa.jinqigfzy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pri.guowangkeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uxd.nanxuanxn.top

[E22] 字节长度与字符长度
来源：http://apv.iojbl.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lhx.havefunace.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tnh.zhaomingkeji.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dcc.vqdsnc.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fgs.cdnleiting.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mme.yongpay.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pum.tianlin.xyz

Ruby: s.bytesize;  s.length
来源：http://gvt.mhx1999.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://iuq.316326.xyz

================================================================================
来源：http://nvs.xuetiantiany.cn

F. 文件与目录
来源：http://hls.jyoumei.cn

================================================================================
来源：http://gyg.havefunace.top

[F01] 读取整个文件
来源：http://oqp.sysykeji.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jqq.yuxming.cn

PHP:  file_get_contents("a.txt");
来源：http://duj.guannengcc.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qwo.yanxiufei.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bde.chenjidiqi.icu

Java: Files.readString(Path.of("a.txt"))
来源：http://dor.hongshengwenyu.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hwq.havefunace.top

Ruby: File.read("a.txt")
来源：http://hcg.316326.xyz

C#:   File.ReadAllText("a.txt");
来源：http://cwh.yj20258888.top

[F02] 逐行读取文件
来源：http://oot.yueranfly.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mor.yueranfly.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fqf.nanxuanxn.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rdt.cqqwz.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wei.havefunace.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jyz.nanxuanxn.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rnp.zhixingplan.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xge.hammf.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://twp.nanxinkj.top

[F03] 写入文件（覆盖）
来源：http://cmz.cashguo.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://moj.xingfuxueyuan.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://qzb.dianchejie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ahk.dianchejie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gaz.gaohongyu789.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tdm.wangshuangyany.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wuv.xziqi.cn

Ruby: File.write("a.txt", "hi")
来源：http://tnu.dianchejie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wfq.dianchejie.cn

[F04] 追加写入文件
来源：http://wff.ppjwa.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wql.ppjwa.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vof.xziqi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wvc.sweek.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://url.chenzaomai.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://spz.jinqigfzy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lcw.jyoumei.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ljb.tian-w.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://eil.jinyuanbaomall.cn

[F05] 判断文件或目录是否存在
来源：http://chw.gaohongyu789.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://puh.xziqi.cn

PHP:  file_exists("a.txt");
来源：http://rcs.0kj1m.cn

JS:   fs.existsSync("a.txt")
来源：http://ddq.ctjpmb.com

TS:   fs.existsSync("a.txt")
来源：http://oar.kuanghao11.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://rte.fzhhl.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://luu.wangshuangyany.cn

Ruby: File.exist?("a.txt")
来源：http://iww.iojbl.cn

C#:   File.Exists("a.txt")
来源：http://tjj.birdmap.top

[F06] 删除文件
来源：http://cxs.yuxming.cn

Py:   os.remove("a.txt")
来源：http://dim.xuanzx.com

PHP:  unlink("a.txt");
来源：http://qab.sxryk.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pqf.hesvh.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ipu.vqdsnc.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://aro.gotoacloud.top

Go:   os.Remove("a.txt")
来源：http://zgg.jinqigfzy.top

Ruby: File.delete("a.txt")
来源：http://qwt.yangfankeji.com

C#:   File.Delete("a.txt");
来源：http://uka.yonumen.top

[F07] 创建目录（含多级）
来源：http://bai.jiagoushi.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vkh.hongshengwenyu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pbo.xuanzx.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pcr.snrcjt.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xfd.nwbrower.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://njf.bbcook.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vmt.cashguo.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xma.9152youxi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ecu.ydzc1.top

[F08] 遍历目录
来源：http://sxg.birdmap.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://xif.nanxuanxn.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qqi.aizwys.cn

JS:   fs.readdirSync("dir")
来源：http://lmb.tarul.cn

TS:   fs.readdirSync("dir")
来源：http://vto.nanxuanxn.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fwo.jinqigufen.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://nrk.guowangkeji.top

Ruby: Dir.children("dir")
来源：http://scj.cheryme.top

C#:   Directory.GetFiles("dir")
来源：http://zqu.nanxuanxn.top

[F09] 获取文件大小
来源：http://jdr.uphjek.com

Py:   os.path.getsize("a.txt")
来源：http://von.haohaochexian.top

PHP:  filesize("a.txt");
来源：http://snx.0kj1m.cn

JS:   fs.statSync("a.txt").size
来源：http://zri.daria6918.cn

TS:   fs.statSync("a.txt").size
来源：http://bgx.guannengcc.top

Java: Files.size(Path.of("a.txt"))
来源：http://ljt.feifeiyinyue.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mkb.52xcode.cn

Ruby: File.size("a.txt")
来源：http://gwn.ppjwa.cn

C#:   new FileInfo("a.txt").Length
来源：http://tmf.zhiwuduotai.top

[F10] 取文件扩展名 / 文件名
来源：http://sxc.0kj1m.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wvh.jinyuanbaomall.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://skm.pengpengdd.cyou

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mia.cheryme.top

TS:   path.extname("a.txt")
来源：http://caw.52xcode.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xmg.quarkkingdee.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://eui.hfpthk.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://udj.tarul.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jhn.jianghu66.top

[F11] 复制与移动文件
来源：http://wgo.haohaochexian.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qor.jinqigufen.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qzy.hfpthk.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wka.hammf.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vtx.havefunace.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hjy.yj202588.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jan.wangshuangyany.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ker.uphjek.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wdr.hongshengwenyu.top

[F12] CSV 读写
来源：http://exy.hammf.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://srm.nanxuanxn.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xek.hcnkem.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zlh.fanxiaobao.xyz

TS:   // 同上
来源：http://car.zhixingplan.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wxc.cheryme.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://poo.sufxvd.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://uec.cucudq.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://csx.jlsjyb.cn

================================================================================
来源：http://gji.ctjpmb.com

G. 面向对象
来源：http://ixn.hnqzz.top

================================================================================
来源：http://bnr.andypj.xyz

[G01] 定义类
来源：http://ptk.yj202588.top

Py:   class User: pass
来源：http://swp.sjlbkw.cn

PHP:  class User {}
来源：http://sbi.meibo888.top

JS:   class User {}
来源：http://cew.yanxiufei.cn

TS:   class User { name: string = ""; }
来源：http://pzy.shanyushiyangtech.top

Java: class User {}
来源：http://ptf.bjfxy.top

Go:   type User struct { Name string }
来源：http://nmb.fanxiaobao.xyz

Ruby: class User; end
来源：http://ehg.bjfxy.top

C#:   class User {}
来源：http://kwh.hesvh.cn

[G02] 构造函数
来源：http://ggf.jyoumei.cn

Py:   def __init__(self, name): self.name = name
来源：http://cml.jyoumei.cn

PHP:  public function __construct(public string $name) {}
来源：http://pvh.fzhhl.top

JS:   constructor(name) { this.name = name; }
来源：http://gww.jyoumei.cn

TS:   constructor(public name: string) {}
来源：http://bzt.jinyuanbaomall.cn

Java: User(String name) { this.name = name; }
来源：http://qbi.vehdjk.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hnh.tianlin.xyz

Ruby: def initialize(name); @name = name; end
来源：http://gmd.kuanghao11.cn

C#:   public User(string name) { Name = name; }
来源：http://ltj.xylfe.cn

[G03] 实例属性
来源：http://ecl.hysaishi.cn

Py:   self.name = "x"
来源：http://nsy.yvedp.cn

PHP:  public string $name = "x";
来源：http://afo.yfazqb.com

JS:   this.name = "x";
来源：http://ink.wangshuangyany.cn

TS:   name: string = "x";
来源：http://app.hnxiangtu.top

Java: private String name;
来源：http://pfv.yuxming.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rsb.chenlongwang.top

Ruby: @name = "x"
来源：http://shs.birdmap.top

C#:   public string Name { get; set; } = "x";
来源：http://mps.pycfn.com

[G04] 定义方法
来源：http://eai.quarkkingdee.top

Py:   def greet(self): return self.name
来源：http://rqv.fengsongda.top

PHP:  public function greet(): string { return $this->name; }
来源：http://yxx.aibaodan.cn

JS:   greet() { return this.name; }
来源：http://myh.yueranfly.top

TS:   greet(): string { return this.name; }
来源：http://qhw.jianghu66.top

Java: String greet() { return name; }
来源：http://vdn.hnqzz.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://mld.zhoulong.xyz

Ruby: def greet; @name; end
来源：http://gqe.uphjek.com

C#:   public string Greet() => Name;
来源：http://rnx.0kj1m.cn

[G05] 继承
来源：http://fvg.vehdjk.com

Py:   class Admin(User): pass
来源：http://wvl.fehbvm.com

PHP:  class Admin extends User {}
来源：http://qfi.kuanghao11.cn

JS:   class Admin extends User {}
来源：http://sli.daria6918.cn

TS:   class Admin extends User {}
来源：http://lbs.aibaodan.cn

Java: class Admin extends User {}
来源：http://hwd.xinyue.icu

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dts.fehbvm.com

Ruby: class Admin < User; end
来源：http://vhj.yj20258.top

C#:   class Admin : User {}
来源：http://oce.yuanzhike.top

[G06] 重写方法
来源：http://ajc.vqdsnc.cn

Py:   def greet(self): return "admin"
来源：http://wgx.jinqigfzy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://bnt.hcnkem.com

JS:   greet() { return "admin"; }
来源：http://peg.jinqigfzy.top

TS:   greet(): string { return "admin"; }
来源：http://mbg.jinqigufen.top

Java: @Override String greet() { return "admin"; }
来源：http://hna.hnqzz.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qiz.ywan-chungtsiang.top

Ruby: def greet; "admin"; end
来源：http://zzr.yvedp.cn

C#:   public override string Greet() => "admin";
来源：http://pja.jyoumei.cn

[G07] 调用父类方法
来源：http://hmo.redwolf501.top

Py:   super().greet()
来源：http://wto.sysykeji.top

PHP:  parent::greet();
来源：http://lmz.0kj1m.cn

JS:   super.greet();
来源：http://zcl.wangshuangyany.cn

TS:   super.greet();
来源：http://dtu.wangshuangyany.cn

Java: super.greet();
来源：http://puu.wangdashe.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lca.pengpengdd.cyou

Ruby: super
来源：http://dxf.ppjwa.cn

C#:   base.Greet();
来源：http://umk.guannengcc.top

[G08] 静态方法与属性
来源：http://ufp.zhengqikj.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tfa.fktsv.cn

PHP:  public static function f() {}
来源：http://amk.bbcook.cn

JS:   static f() {}
来源：http://rbb.shanyushiyangkeji.top

TS:   static f(): void {}
来源：http://jbb.uphjek.com

Java: static void f() {}
来源：http://ehe.gzhubu.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://kwa.zdbjq.cn

Ruby: def self.f; end
来源：http://syj.yfazqb.com

C#:   public static void F() {}
来源：http://tnj.chenlongwang.top

[G09] 接口 / 抽象类
来源：http://hew.aizwys.cn

Py:   from abc import ABC, abstractmethod
来源：http://xjz.aizwys.cn

PHP:  interface Shape { public function area(): float; }
来源：http://lrx.yongpay.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://acc.meibo888.top

TS:   interface Shape { area(): number; }
来源：http://mbl.feifeiyinyue.top

Java: interface Shape { double area(); }
来源：http://wrb.ydjk.org.cn

Go:   type Shape interface { Area() float64 }
来源：http://nmm.yuanzhike.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sfe.yanxiufei.cn

C#:   interface IShape { double Area(); }
来源：http://vpk.jinghuilouyu.cn

[G10] 访问控制
来源：http://doe.yanxiufei.cn

Py:   约定 _protected / __private（不强制）
来源：http://mnq.zycfv.cn

PHP:  public / protected / private
来源：http://azd.gotoacloud.top

JS:   #private 字段；其余公开
来源：http://way.fktsv.cn

TS:   public / protected / private
来源：http://qqc.wangshuangyany.cn

Java: public / protected / private / 默认包级
来源：http://isd.ywan-chungtsiang.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://xeb.cheryme.top

Ruby: public / protected / private
来源：http://wik.birdmap.top

C#:   public / protected / private / internal
来源：http://xna.hammf.cn

[G11] getter / setter
来源：http://kxe.xylfe.cn

Py:   @property 与 @x.setter
来源：http://nyf.sjlbkw.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://uss.jinqigfzy.top

JS:   get name() { return this._name; }
来源：http://iyr.ivvv.top

TS:   get name(): string { return this._name; }
来源：http://dxr.dashuyun.cn

Java: public String getName() { return name; }
来源：http://unw.shanyushiyangkeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://nbh.xingfuxueyuan.xyz

Ruby: attr_accessor :name
来源：http://tnd.xingfuxueyuan.xyz

C#:   public string Name { get; set; }
来源：http://ugf.zdqjudy.top

[G12] 对象转字符串
来源：http://mha.dashuyun.cn

Py:   def __str__(self): return self.name
来源：http://hez.ydjk.org.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://liy.havefunace.top

JS:   toString() { return this.name; }
来源：http://ogt.andypj.xyz

TS:   toString(): string { return this.name; }
来源：http://otc.nanxuanxn.top

Java: @Override public String toString() { return name; }
来源：http://odu.daxiang520.top

Go:   func (u User) String() string { return u.Name }
来源：http://ihl.9152youxi.cn

Ruby: def to_s; @name; end
来源：http://zrk.yongpay.top

C#:   public override string ToString() => Name;
来源：http://ezz.smart0.xyz

[G13] 判断对象类型
来源：http://bmj.fzhhl.top

Py:   isinstance(u, User)
来源：http://lxl.tianlin.xyz

PHP:  $u instanceof User
来源：http://wkz.vqdsnc.cn

JS:   u instanceof User
来源：http://bpf.sysykeji.top

TS:   u instanceof User
来源：http://qof.snrcjt.cn

Java: u instanceof User
来源：http://flg.birdmap.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://lxd.chenzaomai.com

Ruby: u.is_a?(User)
来源：http://skg.cucudq.cn

C#:   u is User
来源：http://hee.sjlbkw.cn

[G14] 数据类 / record
来源：http://gkx.shuidangran.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ari.quarkkingdee.top

PHP:  // 用 readonly 属性模拟
来源：http://soc.jiagoushi.top

JS:   // 无内置：普通类或对象字面量
来源：http://piq.cucudq.cn

TS:   type User = { name: string; age: number };
来源：http://dlm.fehbvm.com

Java: record User(String name, int age) {}
来源：http://ltv.pengpengdd.cyou

Go:   type User struct { Name string; Age int }
来源：http://rjl.hnqzz.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://utj.pengpengdd.cyou

C#:   record User(string Name, int Age);
来源：http://sbu.xuanzx.com

[G15] 枚举
来源：http://iki.jianghu66.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mfa.ydzc1.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://hus.yfazqb.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://awp.zhengqikj.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://utu.hfpthk.cn

Java: enum Color { RED, GREEN }
来源：http://ygm.jinqigfzy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fwg.daria6918.cn

Ruby: Color = %i[red green].freeze
来源：http://nyh.mhx1999.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zxz.cdnleiting.top

[G16] 对象转数组 / 字典
来源：http://ken.yanxiufei.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hzz.jianghu66.top


<!-- 参考信息 -->