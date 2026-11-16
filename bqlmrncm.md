代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://iwz.smart0.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://ruu.316326.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uho.hysaishi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://plh.hongshengwenyu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wxk.hammf.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rjb.guannengcc.top

Ruby: s.capitalize
来源：http://aum.ybcxt.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rdu.bjfxy.top

[E18] 模板占位符替换
来源：http://qkh.svipenyu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://knk.smart0.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ibp.hysaishi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://cjd.nwbrower.top

TS:   tpl.replaceAll("{name}", name)
来源：http://uhl.nwbrower.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wln.yj20258.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cik.zhiwuduotai.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cws.gotoacloud.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://afp.yuanzhike.top

[E19] 多行文本按行拆分
来源：http://eod.fanxiaobao.xyz

Py:   s.splitlines()
来源：http://xeg.cashguo.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://krf.yueranfly.top

JS:   s.split(/\r?\n/)
来源：http://gvw.guannengcc.top

TS:   s.split(/\r?\n/)
来源：http://cxu.shzxlz.cn

Java: s.lines().toList()
来源：http://cpb.uphjek.com

Go:   strings.Split(s, "\n")
来源：http://vca.jinqigufen.top

Ruby: s.lines
来源：http://djt.jqgfzy.top

C#:   s.Split('\n')
来源：http://sns.mhx1999.top

[E20] 判断字符串是否为空
来源：http://jhw.redwolf501.top

Py:   if not s:
来源：http://lua.hfpthk.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ync.zycfv.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://off.gzhubu.top

TS:   if (s === "") {}
来源：http://kcz.hfpthk.cn

Java: if (s.isEmpty()) {}
来源：http://abb.tarul.cn

Go:   if s == "" {}
来源：http://snh.havefunace.top

Ruby: if s.empty?
来源：http://pzp.jinghuilouyu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ehx.yueranfly.top

[E21] 超长截断加省略号
来源：http://oqs.epnwcf.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nvl.yonumen.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dts.meibo888.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bxk.ppjwa.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rsx.iojbl.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dgi.xziqi.cn

Go:   // 按 rune 判断长度后截断
来源：http://yue.316326.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ovo.ivvv.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gon.ctjpmb.com

[E22] 字节长度与字符长度
来源：http://off.shanyushiyangtech.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://seb.chenlongwang.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://abu.fehbvm.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zym.hysaishi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ahz.9152youxi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ycl.jinqigfzy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jwm.zhijiandao.cn

Ruby: s.bytesize;  s.length
来源：http://act.zhengqikj.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ryj.hnxiangtu.top

================================================================================
来源：http://bdr.guowangkeji.top

F. 文件与目录
来源：http://gfs.aizwys.cn

================================================================================
来源：http://tff.vqdsnc.cn

[F01] 读取整个文件
来源：http://jtu.fehbvm.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wqf.hywenlv.cn

PHP:  file_get_contents("a.txt");
来源：http://qmj.tanke756.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zzf.yonumen.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://trq.vehdjk.com

Java: Files.readString(Path.of("a.txt"))
来源：http://und.iojbl.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rih.ppjwa.cn

Ruby: File.read("a.txt")
来源：http://agj.ppjwa.cn

C#:   File.ReadAllText("a.txt");
来源：http://fre.zhoulong.xyz

[F02] 逐行读取文件
来源：http://aoi.yj20258.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qhp.tarul.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cvj.dianchejie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yqo.shanyushiyangtech.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zno.jinyuanbaomall.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gvj.vqdsnc.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://clh.feifeiyinyue.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://onr.hesvh.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uqm.cqqwz.cn

[F03] 写入文件（覆盖）
来源：http://acv.smart0.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xnn.andypj.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://dgb.aizwys.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tog.hesvh.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oim.jlsjyb.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hzx.daxiang520.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://iwx.smart0.xyz

Ruby: File.write("a.txt", "hi")
来源：http://pcz.yuanzhike.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://knj.hongshengwenyu.top

[F04] 追加写入文件
来源：http://kor.jiagoushi.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gwt.jinqigfzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ujd.haohaochexian.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://icj.jinghuilouyu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xwt.haohaochexian.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tfx.nwbrower.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rwp.xuetiantiany.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hss.meibo888.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ebq.cucudq.cn

[F05] 判断文件或目录是否存在
来源：http://wwj.hfpthk.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pda.yanxiufei.cn

PHP:  file_exists("a.txt");
来源：http://gcs.hammf.cn

JS:   fs.existsSync("a.txt")
来源：http://ysp.kuanghao11.cn

TS:   fs.existsSync("a.txt")
来源：http://zst.fehbvm.com

Java: Files.exists(Path.of("a.txt"))
来源：http://jhe.sufxvd.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xmq.daxiang520.top

Ruby: File.exist?("a.txt")
来源：http://rpl.mhx1999.top

C#:   File.Exists("a.txt")
来源：http://mqt.zhoulong.xyz

[F06] 删除文件
来源：http://bem.bjfxy.top

Py:   os.remove("a.txt")
来源：http://jtg.aibaodan.cn

PHP:  unlink("a.txt");
来源：http://guk.jqgufenzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://tpf.zycfv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fky.hnqzz.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pbg.yuxming.cn

Go:   os.Remove("a.txt")
来源：http://omk.c1oappe.top

Ruby: File.delete("a.txt")
来源：http://yky.dashuyun.cn

C#:   File.Delete("a.txt");
来源：http://yvr.quarkkingdee.top

[F07] 创建目录（含多级）
来源：http://jpg.snrcjt.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xad.gaohongyu789.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xlc.tianlin.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kea.uphjek.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pxi.svipenyu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://flc.hesvh.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://saw.yueranfly.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ytt.sxryk.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jjr.nanxuanxn.top

[F08] 遍历目录
来源：http://dzy.yj20258.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://rqb.shangyingyoupin.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kpm.vehdjk.com

JS:   fs.readdirSync("dir")
来源：http://ott.guowangkeji.top

TS:   fs.readdirSync("dir")
来源：http://eiz.chenjidiqi.icu

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://upj.shanyushiyangkeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://dhy.cdnleiting.top

Ruby: Dir.children("dir")
来源：http://ajc.zhengqikj.top

C#:   Directory.GetFiles("dir")
来源：http://msi.nanxuanxn.top

[F09] 获取文件大小
来源：http://olc.fzhhl.top

Py:   os.path.getsize("a.txt")
来源：http://qvy.iojbl.cn

PHP:  filesize("a.txt");
来源：http://xyb.yangfankeji.com

JS:   fs.statSync("a.txt").size
来源：http://chy.gogol.net.cn

TS:   fs.statSync("a.txt").size
来源：http://wji.kuanghao11.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fhg.shzxlz.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xin.shuidangran.top

Ruby: File.size("a.txt")
来源：http://vnn.xuetiantiany.cn

C#:   new FileInfo("a.txt").Length
来源：http://epb.zdqjudy.top

[F10] 取文件扩展名 / 文件名
来源：http://pec.sxryk.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sue.gotoacloud.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fyw.gogol.net.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xwe.guannengcc.top

TS:   path.extname("a.txt")
来源：http://orz.xinyue.icu

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nxy.yonumen.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fqs.guowangkeji.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ptc.hnxiangtu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://piq.vqdsnc.cn

[F11] 复制与移动文件
来源：http://sec.c1oappe.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://scs.jiagoushi.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://low.xingfuxueyuan.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qjg.shanyushiyangtech.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://awu.jqgfzy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tpx.jinqigfzy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uha.gzhubu.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://szc.xziqi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://osl.havefunace.top

[F12] CSV 读写
来源：http://ylw.cheryme.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ncd.daria6918.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xig.zhoulong.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mvw.shanyushiyangtech.top

TS:   // 同上
来源：http://zyc.yuanzhike.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nuj.sxryk.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://phn.shangyingyoupin.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wip.iojbl.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vlg.xuanzx.com

================================================================================
来源：http://zpv.nanxinkj.top

G. 面向对象
来源：http://pbq.pycfn.com

================================================================================
来源：http://umo.epnwcf.com

[G01] 定义类
来源：http://tid.yueranfly.top

Py:   class User: pass
来源：http://vzn.gotoacloud.top

PHP:  class User {}
来源：http://aiv.yfazqb.com

JS:   class User {}
来源：http://svk.chenzaomai.com

TS:   class User { name: string = ""; }
来源：http://ubb.cheryme.top

Java: class User {}
来源：http://jis.havefunace.top

Go:   type User struct { Name string }
来源：http://zpz.nwbrower.top

Ruby: class User; end
来源：http://fxp.hcnkem.com

C#:   class User {}
来源：http://sxa.zycfv.cn

[G02] 构造函数
来源：http://xkl.guowangkeji.top

Py:   def __init__(self, name): self.name = name
来源：http://muj.svipenyu.cn

PHP:  public function __construct(public string $name) {}
来源：http://wix.hesvh.cn

JS:   constructor(name) { this.name = name; }
来源：http://uvg.uphjek.com

TS:   constructor(public name: string) {}
来源：http://zqw.shuidangran.top

Java: User(String name) { this.name = name; }
来源：http://lgs.sweek.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ivd.haohaochexian.top

Ruby: def initialize(name); @name = name; end
来源：http://hff.zhixingplan.top

C#:   public User(string name) { Name = name; }
来源：http://bde.chenjidiqi.icu

[G03] 实例属性
来源：http://mxq.yvedp.cn

Py:   self.name = "x"
来源：http://mue.aizwys.cn

PHP:  public string $name = "x";
来源：http://qll.zhaomingkeji.xyz

JS:   this.name = "x";
来源：http://vyc.quarkkingdee.top

TS:   name: string = "x";
来源：http://ryy.jinqigfzy.top

Java: private String name;
来源：http://nbb.yangfankeji.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wyc.52xcode.cn

Ruby: @name = "x"
来源：http://xrj.yuanzhike.top

C#:   public string Name { get; set; } = "x";
来源：http://doh.quarkkingdee.top

[G04] 定义方法
来源：http://oxh.tian-w.cn

Py:   def greet(self): return self.name
来源：http://tzm.yuxming.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://mqe.snrcjt.cn

JS:   greet() { return this.name; }
来源：http://csh.quarkkingdee.top

TS:   greet(): string { return this.name; }
来源：http://fvs.guannengcc.top

Java: String greet() { return name; }
来源：http://syw.yvedp.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bct.nanxinkj.top

Ruby: def greet; @name; end
来源：http://afu.ydjk.org.cn

C#:   public string Greet() => Name;
来源：http://znx.ydjk.org.cn

[G05] 继承
来源：http://tlr.smart0.xyz

Py:   class Admin(User): pass
来源：http://xeu.birdmap.top

PHP:  class Admin extends User {}
来源：http://wyj.shuidangran.top

JS:   class Admin extends User {}
来源：http://mbr.chenlongwang.top

TS:   class Admin extends User {}
来源：http://zwg.pycfn.com

Java: class Admin extends User {}
来源：http://dum.hongshengwenyu.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tkf.yuanzhike.top

Ruby: class Admin < User; end
来源：http://xdh.yonumen.top

C#:   class Admin : User {}
来源：http://kmf.dianchejie.cn

[G06] 重写方法
来源：http://uwk.ybcxt.top

Py:   def greet(self): return "admin"
来源：http://dyd.wangdashe.top

PHP:  public function greet(): string { return "admin"; }
来源：http://czf.daria6918.cn

JS:   greet() { return "admin"; }
来源：http://sjf.quarkkingdee.top

TS:   greet(): string { return "admin"; }
来源：http://ubo.sysykeji.top

Java: @Override String greet() { return "admin"; }
来源：http://mnm.hnxiangtu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ogi.hongshengwenyu.top

Ruby: def greet; "admin"; end
来源：http://wfj.snrcjt.cn

C#:   public override string Greet() => "admin";
来源：http://bpz.fktsv.cn

[G07] 调用父类方法
来源：http://vnt.guannengcc.top

Py:   super().greet()
来源：http://ldw.quarkkingdee.top

PHP:  parent::greet();
来源：http://csy.hfpthk.cn

JS:   super.greet();
来源：http://lmt.zycfv.cn

TS:   super.greet();
来源：http://qks.jinghuilouyu.cn

Java: super.greet();
来源：http://lsp.jinqigfzy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://aww.yanxiufei.cn

Ruby: super
来源：http://sed.shzxlz.cn

C#:   base.Greet();
来源：http://mfo.shangyingyoupin.top

[G08] 静态方法与属性
来源：http://tyl.shanyushiyangkeji.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lwd.feifeiyinyue.top

PHP:  public static function f() {}
来源：http://fah.jinghuilouyu.cn

JS:   static f() {}
来源：http://ikq.wangshuangyany.cn

TS:   static f(): void {}
来源：http://nyq.jiagoushi.top

Java: static void f() {}
来源：http://klz.jinyuanbaomall.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://npp.tanke756.top

Ruby: def self.f; end
来源：http://hmd.ydjk.org.cn

C#:   public static void F() {}
来源：http://wxs.jqgfzy.top

[G09] 接口 / 抽象类
来源：http://hrk.daxiang520.top

Py:   from abc import ABC, abstractmethod
来源：http://teg.52xcode.cn

PHP:  interface Shape { public function area(): float; }
来源：http://kwn.zhaomingkeji.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://ggn.gzhubu.top

TS:   interface Shape { area(): number; }
来源：http://dig.aibaodan.cn

Java: interface Shape { double area(); }
来源：http://bdz.yvedp.cn

Go:   type Shape interface { Area() float64 }
来源：http://gmc.yongpay.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xan.wangdashe.top

C#:   interface IShape { double Area(); }
来源：http://hax.jqgufenzy.top

[G10] 访问控制
来源：http://biq.ehwqpu.com

Py:   约定 _protected / __private（不强制）
来源：http://uss.cheryme.top

PHP:  public / protected / private
来源：http://evu.jiagoushi.top

JS:   #private 字段；其余公开
来源：http://rcn.xylfe.cn

TS:   public / protected / private
来源：http://etk.ywan-chungtsiang.top

Java: public / protected / private / 默认包级
来源：http://xzh.ivvv.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://cfl.yanxiufei.cn

Ruby: public / protected / private
来源：http://yvw.ybcxt.top

C#:   public / protected / private / internal
来源：http://xzr.yvedp.cn

[G11] getter / setter
来源：http://mbs.hnqzz.top

Py:   @property 与 @x.setter
来源：http://jsa.hysaishi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://iyt.chenjidiqi.icu

JS:   get name() { return this._name; }
来源：http://uck.0kj1m.cn

TS:   get name(): string { return this._name; }
来源：http://fyi.nanxuanxn.top

Java: public String getName() { return name; }
来源：http://qip.yueranfly.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://iez.zdqjudy.top

Ruby: attr_accessor :name
来源：http://vac.cucudq.cn

C#:   public string Name { get; set; }
来源：http://xnf.ywan-chungtsiang.top

[G12] 对象转字符串
来源：http://hec.dashuyun.cn

Py:   def __str__(self): return self.name
来源：http://fil.xylfe.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://aky.kuanghao11.cn

JS:   toString() { return this.name; }
来源：http://mtj.guannengcc.top

TS:   toString(): string { return this.name; }
来源：http://bnr.zhaomingkeji.xyz

Java: @Override public String toString() { return name; }
来源：http://vyn.jiagoushi.top

Go:   func (u User) String() string { return u.Name }
来源：http://eoo.ywan-chungtsiang.top

Ruby: def to_s; @name; end
来源：http://kbi.gzhubu.top

C#:   public override string ToString() => Name;
来源：http://lnq.haohaochexian.top

[G13] 判断对象类型
来源：http://znj.fktsv.cn

Py:   isinstance(u, User)
来源：http://qlj.ppjwa.cn

PHP:  $u instanceof User
来源：http://cba.jianghu66.top

JS:   u instanceof User
来源：http://miz.yueranfly.top

TS:   u instanceof User
来源：http://pgj.zhongyouzk.top

Java: u instanceof User
来源：http://wsc.gotoacloud.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://zjl.birdmap.top

Ruby: u.is_a?(User)
来源：http://svn.hesvh.cn

C#:   u is User
来源：http://bvc.jqgfzy.top

[G14] 数据类 / record
来源：http://hpl.yj20258888.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ybk.jqgfzy.top

PHP:  // 用 readonly 属性模拟
来源：http://lev.gaohongyu789.top

JS:   // 无内置：普通类或对象字面量
来源：http://nas.jianghu66.top

TS:   type User = { name: string; age: number };
来源：http://anf.yonumen.top

Java: record User(String name, int age) {}
来源：http://bhv.bjfxy.top

Go:   type User struct { Name string; Age int }
来源：http://vxu.nwbrower.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yqu.daria6918.cn

C#:   record User(string Name, int Age);
来源：http://rac.wangdashe.top

[G15] 枚举
来源：http://olo.fzhhl.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ahb.yuanzhike.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ype.aibaodan.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://how.cheryme.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://frm.shanyushiyangkeji.top

Java: enum Color { RED, GREEN }
来源：http://xiu.smart0.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lxf.shzxlz.cn


<!-- 参考信息 -->