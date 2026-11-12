代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pnj.gogol.net.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xqj.hongshengwenyu.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cub.9152youxi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://noh.zycfv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jqo.xingfuxueyuan.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ktu.cdnleiting.top

Ruby: s.capitalize
来源：http://mxc.jqgfzy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xhd.zycfv.cn

[E18] 模板占位符替换
来源：http://wwb.ydjk.org.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://whp.ybcxt.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vwt.9152youxi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://lak.yanxiufei.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://amn.ivvv.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ses.yuxming.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://imu.yueranfly.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://srr.zycfv.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gac.yueranfly.top

[E19] 多行文本按行拆分
来源：http://nka.sweek.top

Py:   s.splitlines()
来源：http://ovy.pengpengdd.cyou

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lbj.jiagoushi.top

JS:   s.split(/\r?\n/)
来源：http://fzv.aizwys.cn

TS:   s.split(/\r?\n/)
来源：http://mgh.andypj.xyz

Java: s.lines().toList()
来源：http://kws.xylfe.cn

Go:   strings.Split(s, "\n")
来源：http://qil.hfpthk.cn

Ruby: s.lines
来源：http://ynl.xingfuxueyuan.xyz

C#:   s.Split('\n')
来源：http://chu.svipenyu.cn

[E20] 判断字符串是否为空
来源：http://lgo.9152youxi.cn

Py:   if not s:
来源：http://qkf.yangfankeji.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://skk.svipenyu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wkn.aibaodan.cn

TS:   if (s === "") {}
来源：http://vhv.xylfe.cn

Java: if (s.isEmpty()) {}
来源：http://bjt.chenjidiqi.icu

Go:   if s == "" {}
来源：http://jmf.ydjk.org.cn

Ruby: if s.empty?
来源：http://myb.316326.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lec.tian-w.cn

[E21] 超长截断加省略号
来源：http://flc.jlsjyb.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sws.daria6918.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://csq.feifeiyinyue.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jzs.shzxlz.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mmp.fktsv.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hwd.zhaomingkeji.xyz

Go:   // 按 rune 判断长度后截断
来源：http://dvc.sufxvd.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ucn.xuetiantiany.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rhy.pycfn.com

[E22] 字节长度与字符长度
来源：http://mty.hongshengwenyu.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ccl.bbcook.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yll.dashuyun.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nde.ppjwa.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qyj.feifeiyinyue.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://msw.yangfankeji.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://che.jinqigufen.top

Ruby: s.bytesize;  s.length
来源：http://daq.andypj.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://miu.guannengcc.top

================================================================================
来源：http://qgx.aibaodan.cn

F. 文件与目录
来源：http://dux.hcnkem.com

================================================================================
来源：http://kpl.havefunace.top

[F01] 读取整个文件
来源：http://uew.nanxinkj.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lwt.haohaochexian.top

PHP:  file_get_contents("a.txt");
来源：http://ypc.zhiwuduotai.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zdq.xinyue.icu

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rpq.chenlongwang.top

Java: Files.readString(Path.of("a.txt"))
来源：http://wuq.hammf.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cce.jinqigfzy.top

Ruby: File.read("a.txt")
来源：http://evz.316326.xyz

C#:   File.ReadAllText("a.txt");
来源：http://adc.yfazqb.com

[F02] 逐行读取文件
来源：http://vjd.hcnkem.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://eux.vehdjk.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ccw.hesvh.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tmc.zhoulong.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rpy.birdmap.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mqf.tanke756.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://itn.yueranfly.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xio.epnwcf.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jcu.zhijiandao.cn

[F03] 写入文件（覆盖）
来源：http://vve.kuanghao11.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bak.yuanzhike.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://duk.fehbvm.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fpm.zhiwuduotai.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fac.aizwys.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kcb.sufxvd.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://azz.ctjpmb.com

Ruby: File.write("a.txt", "hi")
来源：http://xsw.sxryk.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vdi.sjlbkw.cn

[F04] 追加写入文件
来源：http://nia.redwolf501.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://edy.tanke756.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hzd.xuetiantiany.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zeb.andypj.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zhr.zhoulong.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://owb.ivvv.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://eij.fehbvm.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wgu.yj20258888.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rhk.zhiwuduotai.top

[F05] 判断文件或目录是否存在
来源：http://qzp.fktsv.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lhx.haohaochexian.top

PHP:  file_exists("a.txt");
来源：http://qxt.zhixingplan.top

JS:   fs.existsSync("a.txt")
来源：http://fqc.cqqwz.cn

TS:   fs.existsSync("a.txt")
来源：http://wuo.jqgufenzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://uqo.hnqzz.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ubz.sjlbkw.cn

Ruby: File.exist?("a.txt")
来源：http://jov.yj202588.top

C#:   File.Exists("a.txt")
来源：http://xni.chenjidiqi.icu

[F06] 删除文件
来源：http://wia.tian-w.cn

Py:   os.remove("a.txt")
来源：http://xtc.jinqigufen.top

PHP:  unlink("a.txt");
来源：http://htj.shanyushiyangkeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://hoa.gotoacloud.top

TS:   fs.unlinkSync("a.txt")
来源：http://amn.zycfv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qad.316326.xyz

Go:   os.Remove("a.txt")
来源：http://zov.yanxiufei.cn

Ruby: File.delete("a.txt")
来源：http://bwo.fktsv.cn

C#:   File.Delete("a.txt");
来源：http://xfh.jyoumei.cn

[F07] 创建目录（含多级）
来源：http://hfl.redwolf501.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://csv.jyoumei.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://agq.jinqigufen.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://byk.andypj.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vbw.ctjpmb.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vte.zhongyouzk.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hos.feifeiyinyue.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hov.xinyue.icu

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wdx.gogol.net.cn

[F08] 遍历目录
来源：http://fge.hesvh.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://rio.jlsjyb.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ofi.wangshuangyany.cn

JS:   fs.readdirSync("dir")
来源：http://qvc.9152youxi.cn

TS:   fs.readdirSync("dir")
来源：http://wsp.316326.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gmh.ehwqpu.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://vez.zhengqikj.top

Ruby: Dir.children("dir")
来源：http://qct.xingfuxueyuan.xyz

C#:   Directory.GetFiles("dir")
来源：http://jnn.jlsjyb.cn

[F09] 获取文件大小
来源：http://yuz.gzhubu.top

Py:   os.path.getsize("a.txt")
来源：http://tvh.fzhhl.top

PHP:  filesize("a.txt");
来源：http://kbw.jinyuanbaomall.cn

JS:   fs.statSync("a.txt").size
来源：http://hxy.quarkkingdee.top

TS:   fs.statSync("a.txt").size
来源：http://opr.smart0.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://mzj.uphjek.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gel.zhengqikj.top

Ruby: File.size("a.txt")
来源：http://gcx.uphjek.com

C#:   new FileInfo("a.txt").Length
来源：http://kqf.tianlin.xyz

[F10] 取文件扩展名 / 文件名
来源：http://yfq.cqqwz.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cnp.xinyue.icu

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kbf.guowangkeji.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ovf.yangfankeji.com

TS:   path.extname("a.txt")
来源：http://upf.hesvh.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://knh.cdnleiting.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sjy.hammf.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rhk.ydjk.org.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://efh.ybcxt.top

[F11] 复制与移动文件
来源：http://mxl.sufxvd.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://chz.epnwcf.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jhs.316326.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hic.wangshuangyany.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hso.jlsjyb.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rxf.nanxinkj.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://aij.c1oappe.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ueo.xuetiantiany.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sqb.feifeiyinyue.top

[F12] CSV 读写
来源：http://tiw.tanke756.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fnl.gogol.net.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://olg.52xcode.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://erc.jianghu66.top

TS:   // 同上
来源：http://sxu.gaohongyu789.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ucc.ivvv.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zdu.dashuyun.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dga.zycfv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qoh.uphjek.com

================================================================================
来源：http://pep.zdbjq.cn

G. 面向对象
来源：http://rwk.sjlbkw.cn

================================================================================
来源：http://iek.yj20258.top

[G01] 定义类
来源：http://ugj.aibaodan.cn

Py:   class User: pass
来源：http://imv.shanyushiyangtech.top

PHP:  class User {}
来源：http://jpr.aizwys.cn

JS:   class User {}
来源：http://asr.daxiang520.top

TS:   class User { name: string = ""; }
来源：http://qmx.hcnkem.com

Java: class User {}
来源：http://vnz.tian-w.cn

Go:   type User struct { Name string }
来源：http://pxu.hammf.cn

Ruby: class User; end
来源：http://zko.52xcode.cn

C#:   class User {}
来源：http://kem.shzxlz.cn

[G02] 构造函数
来源：http://zir.yj20258888.top

Py:   def __init__(self, name): self.name = name
来源：http://zzt.epnwcf.com

PHP:  public function __construct(public string $name) {}
来源：http://yrx.quarkkingdee.top

JS:   constructor(name) { this.name = name; }
来源：http://ipo.meibo888.top

TS:   constructor(public name: string) {}
来源：http://igk.zhoulong.xyz

Java: User(String name) { this.name = name; }
来源：http://efw.xinyue.icu

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vot.tarul.cn

Ruby: def initialize(name); @name = name; end
来源：http://ahh.meibo888.top

C#:   public User(string name) { Name = name; }
来源：http://rqi.hfpthk.cn

[G03] 实例属性
来源：http://zaz.cdnleiting.top

Py:   self.name = "x"
来源：http://jrs.xylfe.cn

PHP:  public string $name = "x";
来源：http://wvk.yanxiufei.cn

JS:   this.name = "x";
来源：http://hgu.ybcxt.top

TS:   name: string = "x";
来源：http://uia.tarul.cn

Java: private String name;
来源：http://vdv.yj20258888.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fpp.pengpengdd.cyou

Ruby: @name = "x"
来源：http://iqt.wangdashe.top

C#:   public string Name { get; set; } = "x";
来源：http://xxx.sufxvd.cn

[G04] 定义方法
来源：http://kqf.sweek.top

Py:   def greet(self): return self.name
来源：http://olp.chenjidiqi.icu

PHP:  public function greet(): string { return $this->name; }
来源：http://xcf.chenjidiqi.icu

JS:   greet() { return this.name; }
来源：http://obs.xziqi.cn

TS:   greet(): string { return this.name; }
来源：http://mto.nanxuanxn.top

Java: String greet() { return name; }
来源：http://hli.jqgfzy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ece.hcnkem.com

Ruby: def greet; @name; end
来源：http://zeu.yueranfly.top

C#:   public string Greet() => Name;
来源：http://prd.jiagoushi.top

[G05] 继承
来源：http://nbl.zhixingplan.top

Py:   class Admin(User): pass
来源：http://gcr.ehwqpu.com

PHP:  class Admin extends User {}
来源：http://cbh.hesvh.cn

JS:   class Admin extends User {}
来源：http://nrk.kuanghao11.cn

TS:   class Admin extends User {}
来源：http://zdo.cqqwz.cn

Java: class Admin extends User {}
来源：http://kbk.sysykeji.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://djr.vqdsnc.cn

Ruby: class Admin < User; end
来源：http://zyd.meibo888.top

C#:   class Admin : User {}
来源：http://jeg.hysaishi.cn

[G06] 重写方法
来源：http://ikm.sweek.top

Py:   def greet(self): return "admin"
来源：http://vpi.cucudq.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nsy.ehwqpu.com

JS:   greet() { return "admin"; }
来源：http://hyp.zhengqikj.top

TS:   greet(): string { return "admin"; }
来源：http://wpk.quarkkingdee.top

Java: @Override String greet() { return "admin"; }
来源：http://cnj.jinqigfzy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kev.cdnleiting.top

Ruby: def greet; "admin"; end
来源：http://vrc.yuanzhike.top

C#:   public override string Greet() => "admin";
来源：http://enp.daria6918.cn

[G07] 调用父类方法
来源：http://bra.9152youxi.cn

Py:   super().greet()
来源：http://xyb.sysykeji.top

PHP:  parent::greet();
来源：http://nwu.yfazqb.com

JS:   super.greet();
来源：http://gxz.feifeiyinyue.top

TS:   super.greet();
来源：http://arl.zhaomingkeji.xyz

Java: super.greet();
来源：http://ebn.vqdsnc.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wpo.sjlbkw.cn

Ruby: super
来源：http://qzj.ivvv.top

C#:   base.Greet();
来源：http://llk.zhiwuduotai.top

[G08] 静态方法与属性
来源：http://huf.zhixingplan.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://imu.sufxvd.cn

PHP:  public static function f() {}
来源：http://umi.cashguo.top

JS:   static f() {}
来源：http://kdl.jinyuanbaomall.cn

TS:   static f(): void {}
来源：http://feg.shzxlz.cn

Java: static void f() {}
来源：http://grk.bjfxy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://jqm.svipenyu.cn

Ruby: def self.f; end
来源：http://gqe.zycfv.cn

C#:   public static void F() {}
来源：http://vxv.cqqwz.cn

[G09] 接口 / 抽象类
来源：http://wst.tanke756.top

Py:   from abc import ABC, abstractmethod
来源：http://ark.yuanzhike.top

PHP:  interface Shape { public function area(): float; }
来源：http://ivs.52xcode.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://rqq.xuetiantiany.cn

TS:   interface Shape { area(): number; }
来源：http://dob.yj20258.top

Java: interface Shape { double area(); }
来源：http://lup.epnwcf.com

Go:   type Shape interface { Area() float64 }
来源：http://huk.dianchejie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jdq.jinghuilouyu.cn

C#:   interface IShape { double Area(); }
来源：http://txf.zhiwuduotai.top

[G10] 访问控制
来源：http://ugp.xuanzx.com

Py:   约定 _protected / __private（不强制）
来源：http://evr.zdbjq.cn

PHP:  public / protected / private
来源：http://cfw.yuanzhike.top

JS:   #private 字段；其余公开
来源：http://thd.cucudq.cn

TS:   public / protected / private
来源：http://xwj.ywan-chungtsiang.top

Java: public / protected / private / 默认包级
来源：http://ysw.aibaodan.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ijl.chenlongwang.top

Ruby: public / protected / private
来源：http://wau.zhongyouzk.top

C#:   public / protected / private / internal
来源：http://bim.daria6918.cn

[G11] getter / setter
来源：http://pas.daria6918.cn

Py:   @property 与 @x.setter
来源：http://eke.sysykeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://mxx.xuetiantiany.cn

JS:   get name() { return this._name; }
来源：http://ghx.meibo888.top

TS:   get name(): string { return this._name; }
来源：http://nje.chenjidiqi.icu

Java: public String getName() { return name; }
来源：http://jvu.yfazqb.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://iyf.zdbjq.cn

Ruby: attr_accessor :name
来源：http://bti.yanxiufei.cn

C#:   public string Name { get; set; }
来源：http://vzc.yueranfly.top

[G12] 对象转字符串
来源：http://uqa.zdqjudy.top

Py:   def __str__(self): return self.name
来源：http://cra.fzhhl.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://udj.jqgfzy.top

JS:   toString() { return this.name; }
来源：http://trc.jlsjyb.cn

TS:   toString(): string { return this.name; }
来源：http://ozi.hysaishi.cn

Java: @Override public String toString() { return name; }
来源：http://yef.xziqi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fpa.hnqzz.top

Ruby: def to_s; @name; end
来源：http://rlx.ctjpmb.com

C#:   public override string ToString() => Name;
来源：http://csm.hammf.cn

[G13] 判断对象类型
来源：http://ahe.epnwcf.com

Py:   isinstance(u, User)
来源：http://vnr.yanxiufei.cn

PHP:  $u instanceof User
来源：http://dnv.yj202588.top

JS:   u instanceof User
来源：http://ikf.zhaomingkeji.xyz

TS:   u instanceof User
来源：http://jvp.xuetiantiany.cn

Java: u instanceof User
来源：http://wbn.aibaodan.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ott.c1oappe.top

Ruby: u.is_a?(User)
来源：http://muu.52xcode.cn

C#:   u is User
来源：http://wjx.cucudq.cn

[G14] 数据类 / record
来源：http://mjv.jqgufenzy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nsd.zdqjudy.top

PHP:  // 用 readonly 属性模拟
来源：http://ygz.daxiang520.top

JS:   // 无内置：普通类或对象字面量
来源：http://alx.jianghu66.top

TS:   type User = { name: string; age: number };
来源：http://esr.sjlbkw.cn

Java: record User(String name, int age) {}
来源：http://unh.daxiang520.top

Go:   type User struct { Name string; Age int }
来源：http://vbu.zhixingplan.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qvy.cashguo.top

C#:   record User(string Name, int Age);
来源：http://cbn.shuidangran.top

[G15] 枚举
来源：http://nax.yuanzhike.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://euf.yuxming.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://prz.nwbrower.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://iqt.gaohongyu789.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qqg.c1oappe.top

Java: enum Color { RED, GREEN }
来源：http://sie.hnqzz.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uej.hammf.cn


<!-- 参考信息 -->