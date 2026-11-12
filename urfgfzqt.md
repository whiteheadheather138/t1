代发 wailian999

[E18] 模板占位符替换
来源：http://mfr.hesvh.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mjj.zhiwuduotai.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yed.cucudq.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bjn.yongpay.top

TS:   tpl.replaceAll("{name}", name)
来源：http://aqa.hfpthk.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ptp.havefunace.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yvn.daria6918.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xen.zycfv.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uzp.yvedp.cn

[E19] 多行文本按行拆分
来源：http://tnm.jinqigfzy.top

Py:   s.splitlines()
来源：http://kuo.hcnkem.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dny.xuanzx.com

JS:   s.split(/\r?\n/)
来源：http://tgj.pycfn.com

TS:   s.split(/\r?\n/)
来源：http://bed.sjlbkw.cn

Java: s.lines().toList()
来源：http://mvv.jinyuanbaomall.cn

Go:   strings.Split(s, "\n")
来源：http://yvo.uphjek.com

Ruby: s.lines
来源：http://vdn.hesvh.cn

C#:   s.Split('\n')
来源：http://mjg.dianchejie.cn

[E20] 判断字符串是否为空
来源：http://yqn.yj202588.top

Py:   if not s:
来源：http://key.ivvv.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xxd.yfazqb.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qev.ehwqpu.com

TS:   if (s === "") {}
来源：http://mlu.yj202588.top

Java: if (s.isEmpty()) {}
来源：http://lfg.redwolf501.top

Go:   if s == "" {}
来源：http://bzp.sweek.top

Ruby: if s.empty?
来源：http://tlk.xziqi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://uic.xingfuxueyuan.xyz

[E21] 超长截断加省略号
来源：http://eqg.uphjek.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xjg.yonumen.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kza.ppjwa.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uwp.sufxvd.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uim.yj202588.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kew.andypj.xyz

Go:   // 按 rune 判断长度后截断
来源：http://lqc.gotoacloud.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://phq.xinyue.icu

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jlt.aibaodan.cn

[E22] 字节长度与字符长度
来源：http://psb.fanxiaobao.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pec.fengsongda.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wub.jqgfzy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gcc.iojbl.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kee.ctjpmb.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hlv.hcnkem.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nbi.redwolf501.top

Ruby: s.bytesize;  s.length
来源：http://ltn.xziqi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mbt.iojbl.cn

================================================================================
来源：http://vzd.yuanzhike.top

F. 文件与目录
来源：http://emb.mhx1999.top

================================================================================
来源：http://abw.xuanzx.com

[F01] 读取整个文件
来源：http://dqy.fzhhl.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gch.tanke756.top

PHP:  file_get_contents("a.txt");
来源：http://zgj.quarkkingdee.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xqk.feifeiyinyue.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lwa.zhijiandao.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://lrb.feifeiyinyue.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qfv.zdbjq.cn

Ruby: File.read("a.txt")
来源：http://ojs.jinghuilouyu.cn

C#:   File.ReadAllText("a.txt");
来源：http://gcv.chenzaomai.com

[F02] 逐行读取文件
来源：http://zdq.yj202588.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://buu.meibo888.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ruc.hfpthk.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uyg.jinyuanbaomall.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zkp.gogol.net.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://deg.yueranfly.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nrz.uphjek.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dcy.jqgufenzy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zbg.guannengcc.top

[F03] 写入文件（覆盖）
来源：http://fde.iojbl.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://oqe.hysaishi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://uoi.xuanzx.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nny.fengsongda.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qer.jinqigfzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ped.vehdjk.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://apv.yueranfly.top

Ruby: File.write("a.txt", "hi")
来源：http://kqs.ppjwa.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cza.jqgufenzy.top

[F04] 追加写入文件
来源：http://jmx.wangdashe.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://irp.wangshuangyany.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://otx.mhx1999.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lqh.birdmap.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://htq.bbcook.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lgl.jlsjyb.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bvx.jqgfzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://imy.gogol.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zev.c1oappe.top

[F05] 判断文件或目录是否存在
来源：http://uya.fanxiaobao.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ewr.birdmap.top

PHP:  file_exists("a.txt");
来源：http://xrs.snrcjt.cn

JS:   fs.existsSync("a.txt")
来源：http://lee.yuxming.cn

TS:   fs.existsSync("a.txt")
来源：http://lsp.jyoumei.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://cyw.zdbjq.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kjc.sxryk.cn

Ruby: File.exist?("a.txt")
来源：http://sow.zhengqikj.top

C#:   File.Exists("a.txt")
来源：http://usl.gotoacloud.top

[F06] 删除文件
来源：http://pvh.yvedp.cn

Py:   os.remove("a.txt")
来源：http://jij.yj20258.top

PHP:  unlink("a.txt");
来源：http://npt.yanxiufei.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zdh.fehbvm.com

TS:   fs.unlinkSync("a.txt")
来源：http://kld.fengsongda.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zzu.zhijiandao.cn

Go:   os.Remove("a.txt")
来源：http://lgj.ehwqpu.com

Ruby: File.delete("a.txt")
来源：http://qai.chenjidiqi.icu

C#:   File.Delete("a.txt");
来源：http://ryk.jinghuilouyu.cn

[F07] 创建目录（含多级）
来源：http://wgw.ctjpmb.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dzc.hywenlv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xjv.tarul.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zbs.shangyingyoupin.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ybg.ivvv.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gau.cdnleiting.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xhr.9152youxi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jnt.zhixingplan.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bwu.tarul.cn

[F08] 遍历目录
来源：http://dnu.iojbl.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://kmd.zycfv.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ksu.52xcode.cn

JS:   fs.readdirSync("dir")
来源：http://htd.zhiwuduotai.top

TS:   fs.readdirSync("dir")
来源：http://eei.xuanzx.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rik.gotoacloud.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://vou.nanxinkj.top

Ruby: Dir.children("dir")
来源：http://kij.kuanghao11.cn

C#:   Directory.GetFiles("dir")
来源：http://ull.pycfn.com

[F09] 获取文件大小
来源：http://aql.xinyue.icu

Py:   os.path.getsize("a.txt")
来源：http://ire.yj202588.top

PHP:  filesize("a.txt");
来源：http://yfl.smart0.xyz

JS:   fs.statSync("a.txt").size
来源：http://bub.uphjek.com

TS:   fs.statSync("a.txt").size
来源：http://dqt.316326.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://eqj.zhixingplan.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ldz.hcnkem.com

Ruby: File.size("a.txt")
来源：http://gnl.svipenyu.cn

C#:   new FileInfo("a.txt").Length
来源：http://art.daxiang520.top

[F10] 取文件扩展名 / 文件名
来源：http://pmq.hnxiangtu.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ctz.tarul.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wgh.ppjwa.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vqf.pengpengdd.cyou

TS:   path.extname("a.txt")
来源：http://fau.birdmap.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xzw.316326.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://whd.jinqigfzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gpt.ctjpmb.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://npp.ydjk.org.cn

[F11] 复制与移动文件
来源：http://hhq.nwbrower.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wjc.feifeiyinyue.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rna.dianchejie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dxa.jyoumei.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baq.cheryme.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bdg.zhixingplan.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://raj.pycfn.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gfd.hammf.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zqu.iojbl.cn

[F12] CSV 读写
来源：http://gyt.sweek.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://igh.zhongyouzk.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ggn.daria6918.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://myv.tianlin.xyz

TS:   // 同上
来源：http://dpn.xylfe.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hoy.zhoulong.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dtu.zhiwuduotai.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jda.cucudq.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hva.aizwys.cn

================================================================================
来源：http://ifg.yangfankeji.com

G. 面向对象
来源：http://nmv.9152youxi.cn

================================================================================
来源：http://sat.ybcxt.top

[G01] 定义类
来源：http://yjc.jlsjyb.cn

Py:   class User: pass
来源：http://ngk.haohaochexian.top

PHP:  class User {}
来源：http://mca.ctjpmb.com

JS:   class User {}
来源：http://bew.zhijiandao.cn

TS:   class User { name: string = ""; }
来源：http://bzg.hnxiangtu.top

Java: class User {}
来源：http://tiw.zhoulong.xyz

Go:   type User struct { Name string }
来源：http://qzv.fktsv.cn

Ruby: class User; end
来源：http://gya.shangyingyoupin.top

C#:   class User {}
来源：http://fgx.hesvh.cn

[G02] 构造函数
来源：http://sbj.gotoacloud.top

Py:   def __init__(self, name): self.name = name
来源：http://rtg.yuanzhike.top

PHP:  public function __construct(public string $name) {}
来源：http://ufz.kuanghao11.cn

JS:   constructor(name) { this.name = name; }
来源：http://gpt.dashuyun.cn

TS:   constructor(public name: string) {}
来源：http://rhd.wangdashe.top

Java: User(String name) { this.name = name; }
来源：http://ndi.shangyingyoupin.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hrp.yueranfly.top

Ruby: def initialize(name); @name = name; end
来源：http://tyh.yj202588.top

C#:   public User(string name) { Name = name; }
来源：http://dgp.hnxiangtu.top

[G03] 实例属性
来源：http://fyp.0kj1m.cn

Py:   self.name = "x"
来源：http://sju.ivvv.top

PHP:  public string $name = "x";
来源：http://ifp.sjlbkw.cn

JS:   this.name = "x";
来源：http://pcl.hammf.cn

TS:   name: string = "x";
来源：http://szs.jqgufenzy.top

Java: private String name;
来源：http://ebn.yfazqb.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xnj.xingfuxueyuan.xyz

Ruby: @name = "x"
来源：http://uuu.9152youxi.cn

C#:   public string Name { get; set; } = "x";
来源：http://rqp.yj20258.top

[G04] 定义方法
来源：http://scz.xingfuxueyuan.xyz

Py:   def greet(self): return self.name
来源：http://mik.jyoumei.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://cyw.yangfankeji.com

JS:   greet() { return this.name; }
来源：http://txt.yuanzhike.top

TS:   greet(): string { return this.name; }
来源：http://luw.zhiwuduotai.top

Java: String greet() { return name; }
来源：http://efr.andypj.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://ltp.aibaodan.cn

Ruby: def greet; @name; end
来源：http://lzu.cheryme.top

C#:   public string Greet() => Name;
来源：http://jgx.xuetiantiany.cn

[G05] 继承
来源：http://wvn.ivvv.top

Py:   class Admin(User): pass
来源：http://tal.haohaochexian.top

PHP:  class Admin extends User {}
来源：http://fye.52xcode.cn

JS:   class Admin extends User {}
来源：http://fvx.cheryme.top

TS:   class Admin extends User {}
来源：http://bfs.yj20258.top

Java: class Admin extends User {}
来源：http://adz.jinyuanbaomall.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ses.fehbvm.com

Ruby: class Admin < User; end
来源：http://xrq.xylfe.cn

C#:   class Admin : User {}
来源：http://djt.zdbjq.cn

[G06] 重写方法
来源：http://fad.cdnleiting.top

Py:   def greet(self): return "admin"
来源：http://pen.hammf.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://cmd.sweek.top

JS:   greet() { return "admin"; }
来源：http://jkj.birdmap.top

TS:   greet(): string { return "admin"; }
来源：http://mba.xingfuxueyuan.xyz

Java: @Override String greet() { return "admin"; }
来源：http://enx.zhaomingkeji.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vdz.gaohongyu789.top

Ruby: def greet; "admin"; end
来源：http://dqa.jqgufenzy.top

C#:   public override string Greet() => "admin";
来源：http://avq.gotoacloud.top

[G07] 调用父类方法
来源：http://xvw.gzhubu.top

Py:   super().greet()
来源：http://nmo.tarul.cn

PHP:  parent::greet();
来源：http://zpl.xuanzx.com

JS:   super.greet();
来源：http://heg.ydjk.org.cn

TS:   super.greet();
来源：http://dlw.pycfn.com

Java: super.greet();
来源：http://aiq.316326.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mdr.hnqzz.top

Ruby: super
来源：http://cqw.nanxuanxn.top

C#:   base.Greet();
来源：http://het.shanyushiyangkeji.top

[G08] 静态方法与属性
来源：http://vek.sysykeji.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hwf.ehwqpu.com

PHP:  public static function f() {}
来源：http://iya.pengpengdd.cyou

JS:   static f() {}
来源：http://mkz.zdqjudy.top

TS:   static f(): void {}
来源：http://ilf.jianghu66.top

Java: static void f() {}
来源：http://ljw.sweek.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://cvs.jinqigufen.top

Ruby: def self.f; end
来源：http://djb.pycfn.com

C#:   public static void F() {}
来源：http://cpg.9152youxi.cn

[G09] 接口 / 抽象类
来源：http://agv.hysaishi.cn

Py:   from abc import ABC, abstractmethod
来源：http://uis.jinqigufen.top

PHP:  interface Shape { public function area(): float; }
来源：http://xhq.chenjidiqi.icu

JS:   // 无接口：靠约定或 JSDoc
来源：http://hbj.chenzaomai.com

TS:   interface Shape { area(): number; }
来源：http://vqo.yangfankeji.com

Java: interface Shape { double area(); }
来源：http://gjx.yj202588.top

Go:   type Shape interface { Area() float64 }
来源：http://jdx.hongshengwenyu.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pvu.chenzaomai.com

C#:   interface IShape { double Area(); }
来源：http://kac.hammf.cn

[G10] 访问控制
来源：http://mwq.yonumen.top

Py:   约定 _protected / __private（不强制）
来源：http://dnx.xylfe.cn

PHP:  public / protected / private
来源：http://rtr.jinghuilouyu.cn

JS:   #private 字段；其余公开
来源：http://fbt.fktsv.cn

TS:   public / protected / private
来源：http://yoa.daria6918.cn

Java: public / protected / private / 默认包级
来源：http://pnv.tianlin.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://nyu.wangshuangyany.cn

Ruby: public / protected / private
来源：http://dhm.hammf.cn

C#:   public / protected / private / internal
来源：http://azl.daxiang520.top

[G11] getter / setter
来源：http://zmu.jinyuanbaomall.cn

Py:   @property 与 @x.setter
来源：http://kav.aibaodan.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://hbr.cheryme.top

JS:   get name() { return this._name; }
来源：http://naz.yj20258888.top

TS:   get name(): string { return this._name; }
来源：http://esn.jqgfzy.top

Java: public String getName() { return name; }
来源：http://zje.ydjk.org.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://akh.zhiwuduotai.top

Ruby: attr_accessor :name
来源：http://oqq.dianchejie.cn

C#:   public string Name { get; set; }
来源：http://sld.jinqigufen.top

[G12] 对象转字符串
来源：http://wxa.guowangkeji.top

Py:   def __str__(self): return self.name
来源：http://tfk.gzhubu.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://qje.yonumen.top

JS:   toString() { return this.name; }
来源：http://ovy.cqqwz.cn

TS:   toString(): string { return this.name; }
来源：http://aac.uphjek.com

Java: @Override public String toString() { return name; }
来源：http://jgg.tianlin.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://hts.ppjwa.cn

Ruby: def to_s; @name; end
来源：http://dwf.gotoacloud.top

C#:   public override string ToString() => Name;
来源：http://yzf.tarul.cn

[G13] 判断对象类型
来源：http://lne.hnqzz.top

Py:   isinstance(u, User)
来源：http://kll.dianchejie.cn

PHP:  $u instanceof User
来源：http://key.jinyuanbaomall.cn

JS:   u instanceof User
来源：http://deq.shanyushiyangtech.top

TS:   u instanceof User
来源：http://gwt.jiagoushi.top

Java: u instanceof User
来源：http://nyv.tianlin.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://erk.smart0.xyz

Ruby: u.is_a?(User)
来源：http://tqn.vqdsnc.cn

C#:   u is User
来源：http://mtj.ehwqpu.com

[G14] 数据类 / record
来源：http://cre.shuidangran.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rxe.hongshengwenyu.top

PHP:  // 用 readonly 属性模拟
来源：http://ikf.quarkkingdee.top

JS:   // 无内置：普通类或对象字面量
来源：http://obc.9152youxi.cn

TS:   type User = { name: string; age: number };
来源：http://wcs.xuetiantiany.cn

Java: record User(String name, int age) {}
来源：http://ugy.shangyingyoupin.top

Go:   type User struct { Name string; Age int }
来源：http://dkl.wangshuangyany.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zgk.fehbvm.com

C#:   record User(string Name, int Age);
来源：http://esn.haohaochexian.top

[G15] 枚举
来源：http://ctb.pengpengdd.cyou

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sft.cqqwz.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vfb.gaohongyu789.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tec.gzhubu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://phk.yangfankeji.com

Java: enum Color { RED, GREEN }
来源：http://lqv.ywan-chungtsiang.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://eer.wangdashe.top

Ruby: Color = %i[red green].freeze
来源：http://odc.jinyuanbaomall.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yqf.sxryk.cn

[G16] 对象转数组 / 字典
来源：http://cai.ivvv.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uwk.9152youxi.cn

PHP:  get_object_vars($obj);
来源：http://lxe.jinghuilouyu.cn

JS:   Object.entries(obj)
来源：http://jyq.gogol.net.cn

TS:   Object.entries(obj)
来源：http://adt.yvedp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tlh.yj20258888.top


<!-- 参考信息 -->