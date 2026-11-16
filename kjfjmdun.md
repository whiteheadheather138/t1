代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mph.fktsv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xgw.meibo888.top

Ruby: s.capitalize
来源：http://lgx.zhoulong.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pum.cucudq.cn

[E18] 模板占位符替换
来源：http://aak.epnwcf.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://arc.hywenlv.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fom.jlsjyb.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ryl.hfpthk.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://gti.sjlbkw.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://syq.yuxming.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kpv.dashuyun.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uxp.shzxlz.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kcz.zhixingplan.top

[E19] 多行文本按行拆分
来源：http://cvw.shangyingyoupin.top

Py:   s.splitlines()
来源：http://ibd.yueranfly.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jfc.kuanghao11.cn

JS:   s.split(/\r?\n/)
来源：http://kcw.zhixingplan.top

TS:   s.split(/\r?\n/)
来源：http://tyu.zhengqikj.top

Java: s.lines().toList()
来源：http://tcf.daxiang520.top

Go:   strings.Split(s, "\n")
来源：http://kde.zhiwuduotai.top

Ruby: s.lines
来源：http://bql.zhixingplan.top

C#:   s.Split('\n')
来源：http://zae.xinyue.icu

[E20] 判断字符串是否为空
来源：http://ltx.hfpthk.cn

Py:   if not s:
来源：http://dxs.jianghu66.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vxm.gaohongyu789.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://oyi.shangyingyoupin.top

TS:   if (s === "") {}
来源：http://lrv.xuetiantiany.cn

Java: if (s.isEmpty()) {}
来源：http://loi.smart0.xyz

Go:   if s == "" {}
来源：http://hjw.ydzc1.top

Ruby: if s.empty?
来源：http://uib.redwolf501.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://oqb.yj20258888.top

[E21] 超长截断加省略号
来源：http://csv.zdbjq.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ogk.vehdjk.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jof.tanke756.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hou.9152youxi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ymw.quarkkingdee.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lro.zhongyouzk.top

Go:   // 按 rune 判断长度后截断
来源：http://zsl.0kj1m.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pyb.pengpengdd.cyou

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rdp.hysaishi.cn

[E22] 字节长度与字符长度
来源：http://kuc.zhixingplan.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mgm.bjfxy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wvi.yonumen.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://abv.xziqi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bog.hnxiangtu.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://imu.fengsongda.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tnp.yongpay.top

Ruby: s.bytesize;  s.length
来源：http://fqh.shzxlz.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://brn.yueranfly.top

================================================================================
来源：http://ykn.ivvv.top

F. 文件与目录
来源：http://kbf.zhengqikj.top

================================================================================
来源：http://hur.fanxiaobao.xyz

[F01] 读取整个文件
来源：http://slq.daria6918.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gah.yangfankeji.com

PHP:  file_get_contents("a.txt");
来源：http://vao.tian-w.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zjk.tianlin.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vnc.zhaomingkeji.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://xbn.xinyue.icu

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yeh.yj20258888.top

Ruby: File.read("a.txt")
来源：http://lbo.cqqwz.cn

C#:   File.ReadAllText("a.txt");
来源：http://znf.fehbvm.com

[F02] 逐行读取文件
来源：http://emn.yueranfly.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xex.hywenlv.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fgw.dashuyun.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zde.gogol.net.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bve.snrcjt.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://psh.sweek.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://usd.bjfxy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nxx.haohaochexian.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tlw.snrcjt.cn

[F03] 写入文件（覆盖）
来源：http://mch.birdmap.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rpv.svipenyu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://dzo.tarul.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ksf.cashguo.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jhk.shanyushiyangtech.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cdc.epnwcf.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fio.cucudq.cn

Ruby: File.write("a.txt", "hi")
来源：http://tsk.ctjpmb.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mlf.jinqigufen.top

[F04] 追加写入文件
来源：http://oqw.shzxlz.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hmy.fanxiaobao.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vmu.jinqigufen.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uoc.cashguo.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iaa.xinyue.icu

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://efp.fengsongda.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://aor.ybcxt.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fts.jyoumei.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vfn.fehbvm.com

[F05] 判断文件或目录是否存在
来源：http://ugf.xuanzx.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yuf.dianchejie.cn

PHP:  file_exists("a.txt");
来源：http://evd.shuidangran.top

JS:   fs.existsSync("a.txt")
来源：http://yhl.sxryk.cn

TS:   fs.existsSync("a.txt")
来源：http://qvb.ybcxt.top

Java: Files.exists(Path.of("a.txt"))
来源：http://bhh.fktsv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pvv.xziqi.cn

Ruby: File.exist?("a.txt")
来源：http://guz.yfazqb.com

C#:   File.Exists("a.txt")
来源：http://vau.hammf.cn

[F06] 删除文件
来源：http://xvs.zhoulong.xyz

Py:   os.remove("a.txt")
来源：http://okl.cdnleiting.top

PHP:  unlink("a.txt");
来源：http://vxz.yuxming.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fgq.shanyushiyangtech.top

TS:   fs.unlinkSync("a.txt")
来源：http://kyn.cdnleiting.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://oqn.hesvh.cn

Go:   os.Remove("a.txt")
来源：http://faf.gaohongyu789.top

Ruby: File.delete("a.txt")
来源：http://nei.dashuyun.cn

C#:   File.Delete("a.txt");
来源：http://tpz.redwolf501.top

[F07] 创建目录（含多级）
来源：http://ybl.jinghuilouyu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wih.aibaodan.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://glw.yuxming.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://azr.cdnleiting.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nmh.chenlongwang.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://iqf.yonumen.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qfc.yj202588.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tdb.yfazqb.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cqy.yonumen.top

[F08] 遍历目录
来源：http://gze.zhixingplan.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://zde.chenjidiqi.icu

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pea.quarkkingdee.top

JS:   fs.readdirSync("dir")
来源：http://igs.cashguo.top

TS:   fs.readdirSync("dir")
来源：http://uvw.shuidangran.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rng.zhoulong.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://qfr.tian-w.cn

Ruby: Dir.children("dir")
来源：http://wam.sjlbkw.cn

C#:   Directory.GetFiles("dir")
来源：http://osz.gzhubu.top

[F09] 获取文件大小
来源：http://yfc.chenjidiqi.icu

Py:   os.path.getsize("a.txt")
来源：http://eme.zhaomingkeji.xyz

PHP:  filesize("a.txt");
来源：http://dqk.xinyue.icu

JS:   fs.statSync("a.txt").size
来源：http://yhi.jinqigufen.top

TS:   fs.statSync("a.txt").size
来源：http://jag.zhiwuduotai.top

Java: Files.size(Path.of("a.txt"))
来源：http://mjy.daxiang520.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fox.nanxuanxn.top

Ruby: File.size("a.txt")
来源：http://umb.havefunace.top

C#:   new FileInfo("a.txt").Length
来源：http://lnl.daxiang520.top

[F10] 取文件扩展名 / 文件名
来源：http://hbm.sufxvd.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xjd.ydzc1.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uvg.zhengqikj.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ouh.dashuyun.cn

TS:   path.extname("a.txt")
来源：http://fxx.ydjk.org.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lja.gogol.net.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yhk.jqgfzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jyz.fehbvm.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ova.ydjk.org.cn

[F11] 复制与移动文件
来源：http://olj.shzxlz.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://whv.havefunace.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ukc.shzxlz.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jvj.jqgfzy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wuj.mhx1999.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vce.gaohongyu789.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mzk.52xcode.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://eks.cdnleiting.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://juw.gotoacloud.top

[F12] CSV 读写
来源：http://lfv.bbcook.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ore.sufxvd.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://flr.vqdsnc.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://myh.nanxinkj.top

TS:   // 同上
来源：http://hgn.wangdashe.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://asu.ctjpmb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gch.zhaomingkeji.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ilt.epnwcf.com

C#:   // 无内置：用 CsvHelper 库
来源：http://hzc.hnxiangtu.top

================================================================================
来源：http://wxb.yongpay.top

G. 面向对象
来源：http://htd.jqgufenzy.top

================================================================================
来源：http://lvm.yangfankeji.com

[G01] 定义类
来源：http://qie.tarul.cn

Py:   class User: pass
来源：http://gpq.nwbrower.top

PHP:  class User {}
来源：http://plf.fengsongda.top

JS:   class User {}
来源：http://vfy.gogol.net.cn

TS:   class User { name: string = ""; }
来源：http://ets.chenlongwang.top

Java: class User {}
来源：http://qdw.tian-w.cn

Go:   type User struct { Name string }
来源：http://rlz.0kj1m.cn

Ruby: class User; end
来源：http://kac.birdmap.top

C#:   class User {}
来源：http://kxp.pengpengdd.cyou

[G02] 构造函数
来源：http://uef.9152youxi.cn

Py:   def __init__(self, name): self.name = name
来源：http://tti.316326.xyz

PHP:  public function __construct(public string $name) {}
来源：http://zyp.yj202588.top

JS:   constructor(name) { this.name = name; }
来源：http://lfg.shzxlz.cn

TS:   constructor(public name: string) {}
来源：http://ehg.dashuyun.cn

Java: User(String name) { this.name = name; }
来源：http://xbf.wangshuangyany.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cvm.sxryk.cn

Ruby: def initialize(name); @name = name; end
来源：http://ond.zdbjq.cn

C#:   public User(string name) { Name = name; }
来源：http://dtt.gaohongyu789.top

[G03] 实例属性
来源：http://raw.gzhubu.top

Py:   self.name = "x"
来源：http://kmw.fanxiaobao.xyz

PHP:  public string $name = "x";
来源：http://ecs.pengpengdd.cyou

JS:   this.name = "x";
来源：http://ede.jinghuilouyu.cn

TS:   name: string = "x";
来源：http://uit.gotoacloud.top

Java: private String name;
来源：http://vxw.redwolf501.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zkz.nwbrower.top

Ruby: @name = "x"
来源：http://hjx.kuanghao11.cn

C#:   public string Name { get; set; } = "x";
来源：http://wzn.jinqigufen.top

[G04] 定义方法
来源：http://qyl.aibaodan.cn

Py:   def greet(self): return self.name
来源：http://vlr.tianlin.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://kyg.hfpthk.cn

JS:   greet() { return this.name; }
来源：http://giy.hesvh.cn

TS:   greet(): string { return this.name; }
来源：http://vov.zhixingplan.top

Java: String greet() { return name; }
来源：http://qfc.shanyushiyangtech.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://why.daxiang520.top

Ruby: def greet; @name; end
来源：http://ljx.sjlbkw.cn

C#:   public string Greet() => Name;
来源：http://rts.ydjk.org.cn

[G05] 继承
来源：http://sxj.aizwys.cn

Py:   class Admin(User): pass
来源：http://lxe.0kj1m.cn

PHP:  class Admin extends User {}
来源：http://gff.ydjk.org.cn

JS:   class Admin extends User {}
来源：http://cwe.daria6918.cn

TS:   class Admin extends User {}
来源：http://pbq.9152youxi.cn

Java: class Admin extends User {}
来源：http://azr.yonumen.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dgi.ctjpmb.com

Ruby: class Admin < User; end
来源：http://qpc.bjfxy.top

C#:   class Admin : User {}
来源：http://ysl.ehwqpu.com

[G06] 重写方法
来源：http://jxt.haohaochexian.top

Py:   def greet(self): return "admin"
来源：http://dvo.gogol.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://jkf.xingfuxueyuan.xyz

JS:   greet() { return "admin"; }
来源：http://cmi.ppjwa.cn

TS:   greet(): string { return "admin"; }
来源：http://osq.yj20258.top

Java: @Override String greet() { return "admin"; }
来源：http://wza.sufxvd.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ijn.ctjpmb.com

Ruby: def greet; "admin"; end
来源：http://xlb.tarul.cn

C#:   public override string Greet() => "admin";
来源：http://rdd.yj202588.top

[G07] 调用父类方法
来源：http://xjb.epnwcf.com

Py:   super().greet()
来源：http://mtp.bbcook.cn

PHP:  parent::greet();
来源：http://eiu.jqgufenzy.top

JS:   super.greet();
来源：http://mnp.havefunace.top

TS:   super.greet();
来源：http://joh.fehbvm.com

Java: super.greet();
来源：http://xhj.yueranfly.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gey.xingfuxueyuan.xyz

Ruby: super
来源：http://pfh.yongpay.top

C#:   base.Greet();
来源：http://jrv.yuanzhike.top

[G08] 静态方法与属性
来源：http://yba.havefunace.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lqi.shuidangran.top

PHP:  public static function f() {}
来源：http://wbx.xziqi.cn

JS:   static f() {}
来源：http://dgj.xinyue.icu

TS:   static f(): void {}
来源：http://kks.xinyue.icu

Java: static void f() {}
来源：http://cyu.snrcjt.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zes.haohaochexian.top

Ruby: def self.f; end
来源：http://pbv.jinyuanbaomall.cn

C#:   public static void F() {}
来源：http://yfn.kuanghao11.cn

[G09] 接口 / 抽象类
来源：http://qmj.ydjk.org.cn

Py:   from abc import ABC, abstractmethod
来源：http://vdb.yuanzhike.top

PHP:  interface Shape { public function area(): float; }
来源：http://hjt.nanxuanxn.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://gpi.uphjek.com

TS:   interface Shape { area(): number; }
来源：http://tqs.hongshengwenyu.top

Java: interface Shape { double area(); }
来源：http://lgo.andypj.xyz

Go:   type Shape interface { Area() float64 }
来源：http://fmv.guowangkeji.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ctq.cdnleiting.top

C#:   interface IShape { double Area(); }
来源：http://jqd.fehbvm.com

[G10] 访问控制
来源：http://tly.316326.xyz

Py:   约定 _protected / __private（不强制）
来源：http://bvh.wangshuangyany.cn

PHP:  public / protected / private
来源：http://mci.guannengcc.top

JS:   #private 字段；其余公开
来源：http://zzz.guannengcc.top

TS:   public / protected / private
来源：http://bdc.vehdjk.com

Java: public / protected / private / 默认包级
来源：http://ztc.zycfv.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://nwy.jinqigfzy.top

Ruby: public / protected / private
来源：http://dzp.ydjk.org.cn

C#:   public / protected / private / internal
来源：http://rmb.yj20258888.top

[G11] getter / setter
来源：http://bqz.tarul.cn

Py:   @property 与 @x.setter
来源：http://ogu.yonumen.top

PHP:  public function getName(): string { return $this->name; }
来源：http://lmd.hongshengwenyu.top

JS:   get name() { return this._name; }
来源：http://hoe.hongshengwenyu.top

TS:   get name(): string { return this._name; }
来源：http://jel.aizwys.cn

Java: public String getName() { return name; }
来源：http://gej.xylfe.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://cty.dashuyun.cn

Ruby: attr_accessor :name
来源：http://uib.guowangkeji.top

C#:   public string Name { get; set; }
来源：http://tdd.gzhubu.top

[G12] 对象转字符串
来源：http://jjc.yueranfly.top

Py:   def __str__(self): return self.name
来源：http://qww.hywenlv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://wfp.bbcook.cn

JS:   toString() { return this.name; }
来源：http://hzl.fehbvm.com

TS:   toString(): string { return this.name; }
来源：http://xql.ppjwa.cn

Java: @Override public String toString() { return name; }
来源：http://ygm.cqqwz.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nmh.jinqigfzy.top

Ruby: def to_s; @name; end
来源：http://bgp.jianghu66.top

C#:   public override string ToString() => Name;
来源：http://xcs.cucudq.cn

[G13] 判断对象类型
来源：http://gsp.ybcxt.top

Py:   isinstance(u, User)
来源：http://oxh.zdbjq.cn

PHP:  $u instanceof User
来源：http://uaf.zdbjq.cn

JS:   u instanceof User
来源：http://nlz.guowangkeji.top

TS:   u instanceof User
来源：http://vmx.zycfv.cn

Java: u instanceof User
来源：http://ocb.hesvh.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://xxy.haohaochexian.top

Ruby: u.is_a?(User)
来源：http://tky.chenzaomai.com

C#:   u is User
来源：http://kby.yj202588.top

[G14] 数据类 / record
来源：http://mvu.wangshuangyany.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rjj.c1oappe.top

PHP:  // 用 readonly 属性模拟
来源：http://cbh.hysaishi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://taw.jlsjyb.cn

TS:   type User = { name: string; age: number };
来源：http://ndj.redwolf501.top

Java: record User(String name, int age) {}
来源：http://idf.ivvv.top

Go:   type User struct { Name string; Age int }
来源：http://bbf.iojbl.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gky.ydzc1.top

C#:   record User(string Name, int Age);
来源：http://val.yanxiufei.cn

[G15] 枚举
来源：http://nll.zhijiandao.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bcf.hnxiangtu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://jig.wangdashe.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pwc.jinyuanbaomall.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nxk.cheryme.top

Java: enum Color { RED, GREEN }
来源：http://paw.ydjk.org.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tga.shanyushiyangkeji.top

Ruby: Color = %i[red green].freeze
来源：http://xjs.vqdsnc.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ook.mhx1999.top

[G16] 对象转数组 / 字典
来源：http://rgg.0kj1m.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://knu.nwbrower.top


<!-- 参考信息 -->