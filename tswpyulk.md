代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://khm.yongpay.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://kzw.jqgufenzy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nnn.shanyushiyangtech.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uhe.zdqjudy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cdr.yangfankeji.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://aps.yj20258888.top

Ruby: s.capitalize
来源：http://elx.svipenyu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gyh.yj20258888.top

[E18] 模板占位符替换
来源：http://nys.xingfuxueyuan.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://txq.guannengcc.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vfv.yonumen.top

JS:   tpl.replaceAll("{name}", name)
来源：http://whx.bbcook.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ocn.xuetiantiany.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qgl.daria6918.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lin.sjlbkw.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qus.kuanghao11.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hjz.zhongyouzk.top

[E19] 多行文本按行拆分
来源：http://pvc.smart0.xyz

Py:   s.splitlines()
来源：http://fht.chenjidiqi.icu

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rdr.xingfuxueyuan.xyz

JS:   s.split(/\r?\n/)
来源：http://eee.cucudq.cn

TS:   s.split(/\r?\n/)
来源：http://ttc.xylfe.cn

Java: s.lines().toList()
来源：http://iyw.ydzc1.top

Go:   strings.Split(s, "\n")
来源：http://dnp.zhijiandao.cn

Ruby: s.lines
来源：http://uyl.hysaishi.cn

C#:   s.Split('\n')
来源：http://fuw.c1oappe.top

[E20] 判断字符串是否为空
来源：http://ewn.yueranfly.top

Py:   if not s:
来源：http://gfs.tian-w.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://llv.zhengqikj.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nmu.zhijiandao.cn

TS:   if (s === "") {}
来源：http://brb.zhongyouzk.top

Java: if (s.isEmpty()) {}
来源：http://idy.fanxiaobao.xyz

Go:   if s == "" {}
来源：http://sfw.shangyingyoupin.top

Ruby: if s.empty?
来源：http://bbr.yj202588.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://czc.quarkkingdee.top

[E21] 超长截断加省略号
来源：http://hyu.tian-w.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lyc.hammf.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cef.ehwqpu.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xra.uphjek.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ptt.yvedp.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hbl.zhiwuduotai.top

Go:   // 按 rune 判断长度后截断
来源：http://nyd.birdmap.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vyn.yvedp.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vac.tianlin.xyz

[E22] 字节长度与字符长度
来源：http://hwk.zhaomingkeji.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yys.zhiwuduotai.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nhs.yangfankeji.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hxh.nanxuanxn.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bni.hywenlv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yth.meibo888.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cwq.yj202588.top

Ruby: s.bytesize;  s.length
来源：http://qiq.shzxlz.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tww.sxryk.cn

================================================================================
来源：http://xll.hfpthk.cn

F. 文件与目录
来源：http://isw.vqdsnc.cn

================================================================================
来源：http://znd.ctjpmb.com

[F01] 读取整个文件
来源：http://vhp.guannengcc.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dpl.hnqzz.top

PHP:  file_get_contents("a.txt");
来源：http://lej.bjfxy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mbc.mhx1999.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ups.ydzc1.top

Java: Files.readString(Path.of("a.txt"))
来源：http://rno.redwolf501.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wdw.hesvh.cn

Ruby: File.read("a.txt")
来源：http://ymu.zdqjudy.top

C#:   File.ReadAllText("a.txt");
来源：http://zky.chenzaomai.com

[F02] 逐行读取文件
来源：http://hgg.nanxinkj.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://aoc.fzhhl.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tht.aibaodan.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jbz.aibaodan.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://opa.yuanzhike.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zku.gotoacloud.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://giv.zhijiandao.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cuh.wangshuangyany.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lue.pycfn.com

[F03] 写入文件（覆盖）
来源：http://qgl.zdqjudy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://din.jinyuanbaomall.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://pln.feifeiyinyue.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dlk.ydjk.org.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uka.havefunace.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rhk.ctjpmb.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hzn.zhaomingkeji.xyz

Ruby: File.write("a.txt", "hi")
来源：http://uul.zdqjudy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kth.yj202588.top

[F04] 追加写入文件
来源：http://qeu.pycfn.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://iiw.fktsv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zdy.aibaodan.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jdk.bjfxy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sdr.hnqzz.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kiw.jianghu66.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cpa.chenlongwang.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://iqg.nwbrower.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yqz.nanxuanxn.top

[F05] 判断文件或目录是否存在
来源：http://bxg.zdbjq.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tlz.zdqjudy.top

PHP:  file_exists("a.txt");
来源：http://zoh.zhongyouzk.top

JS:   fs.existsSync("a.txt")
来源：http://atl.bbcook.cn

TS:   fs.existsSync("a.txt")
来源：http://oyd.zdbjq.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fyo.redwolf501.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ysn.jqgfzy.top

Ruby: File.exist?("a.txt")
来源：http://ebb.pycfn.com

C#:   File.Exists("a.txt")
来源：http://wpf.yanxiufei.cn

[F06] 删除文件
来源：http://pim.xingfuxueyuan.xyz

Py:   os.remove("a.txt")
来源：http://loc.yvedp.cn

PHP:  unlink("a.txt");
来源：http://woa.316326.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://mmp.jlsjyb.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ymr.nanxuanxn.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xxe.zdbjq.cn

Go:   os.Remove("a.txt")
来源：http://xob.jiagoushi.top

Ruby: File.delete("a.txt")
来源：http://vzj.zhiwuduotai.top

C#:   File.Delete("a.txt");
来源：http://enw.jyoumei.cn

[F07] 创建目录（含多级）
来源：http://eld.ctjpmb.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dcy.yangfankeji.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pyy.tarul.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wut.cheryme.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kid.xinyue.icu

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://faj.birdmap.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jqf.ppjwa.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hsh.hnqzz.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vnv.uphjek.com

[F08] 遍历目录
来源：http://aev.hesvh.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ime.hywenlv.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sap.xziqi.cn

JS:   fs.readdirSync("dir")
来源：http://xxx.gogol.net.cn

TS:   fs.readdirSync("dir")
来源：http://wvu.sweek.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://oah.dianchejie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ybv.guannengcc.top

Ruby: Dir.children("dir")
来源：http://ane.ivvv.top

C#:   Directory.GetFiles("dir")
来源：http://roy.guowangkeji.top

[F09] 获取文件大小
来源：http://yig.cucudq.cn

Py:   os.path.getsize("a.txt")
来源：http://qgd.wangdashe.top

PHP:  filesize("a.txt");
来源：http://enp.epnwcf.com

JS:   fs.statSync("a.txt").size
来源：http://soq.yj20258.top

TS:   fs.statSync("a.txt").size
来源：http://pix.wangdashe.top

Java: Files.size(Path.of("a.txt"))
来源：http://nez.yueranfly.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ies.sufxvd.cn

Ruby: File.size("a.txt")
来源：http://adt.cashguo.top

C#:   new FileInfo("a.txt").Length
来源：http://fvy.xuetiantiany.cn

[F10] 取文件扩展名 / 文件名
来源：http://vpq.ehwqpu.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jwp.fehbvm.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blf.0kj1m.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jlu.hnxiangtu.top

TS:   path.extname("a.txt")
来源：http://trn.tian-w.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bbi.vqdsnc.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rfp.zhongyouzk.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://oit.gzhubu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ubp.chenlongwang.top

[F11] 复制与移动文件
来源：http://qbx.xinyue.icu

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wru.pycfn.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ktp.yj202588.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gxa.meibo888.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://edy.pycfn.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hku.xinyue.icu

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bzw.daria6918.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cuk.yj202588.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://env.52xcode.cn

[F12] CSV 读写
来源：http://zwl.ctjpmb.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ypd.hongshengwenyu.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jmx.guowangkeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nvx.zhixingplan.top

TS:   // 同上
来源：http://xiw.chenzaomai.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://iby.fktsv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mvg.daria6918.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fuu.jianghu66.top

C#:   // 无内置：用 CsvHelper 库
来源：http://hgh.gogol.net.cn

================================================================================
来源：http://duc.jqgufenzy.top

G. 面向对象
来源：http://ego.316326.xyz

================================================================================
来源：http://fwh.jinyuanbaomall.cn

[G01] 定义类
来源：http://qry.jinghuilouyu.cn

Py:   class User: pass
来源：http://kju.birdmap.top

PHP:  class User {}
来源：http://mzd.hongshengwenyu.top

JS:   class User {}
来源：http://cju.aizwys.cn

TS:   class User { name: string = ""; }
来源：http://vsf.smart0.xyz

Java: class User {}
来源：http://ohd.yanxiufei.cn

Go:   type User struct { Name string }
来源：http://wmj.ybcxt.top

Ruby: class User; end
来源：http://bep.sysykeji.top

C#:   class User {}
来源：http://epg.hongshengwenyu.top

[G02] 构造函数
来源：http://rvw.xingfuxueyuan.xyz

Py:   def __init__(self, name): self.name = name
来源：http://zvz.chenjidiqi.icu

PHP:  public function __construct(public string $name) {}
来源：http://pih.jyoumei.cn

JS:   constructor(name) { this.name = name; }
来源：http://fbb.vqdsnc.cn

TS:   constructor(public name: string) {}
来源：http://cvp.fzhhl.top

Java: User(String name) { this.name = name; }
来源：http://pzd.havefunace.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://oas.ywan-chungtsiang.top

Ruby: def initialize(name); @name = name; end
来源：http://jkz.yonumen.top

C#:   public User(string name) { Name = name; }
来源：http://ftk.ydjk.org.cn

[G03] 实例属性
来源：http://llw.sufxvd.cn

Py:   self.name = "x"
来源：http://mvm.cdnleiting.top

PHP:  public string $name = "x";
来源：http://ykj.aibaodan.cn

JS:   this.name = "x";
来源：http://tuh.gotoacloud.top

TS:   name: string = "x";
来源：http://oio.xziqi.cn

Java: private String name;
来源：http://xlm.yonumen.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://arg.zdbjq.cn

Ruby: @name = "x"
来源：http://jet.fehbvm.com

C#:   public string Name { get; set; } = "x";
来源：http://ylj.bbcook.cn

[G04] 定义方法
来源：http://jcp.yonumen.top

Py:   def greet(self): return self.name
来源：http://hzn.fehbvm.com

PHP:  public function greet(): string { return $this->name; }
来源：http://mha.chenlongwang.top

JS:   greet() { return this.name; }
来源：http://bmt.yangfankeji.com

TS:   greet(): string { return this.name; }
来源：http://efp.zdqjudy.top

Java: String greet() { return name; }
来源：http://kfs.fanxiaobao.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://zav.chenzaomai.com

Ruby: def greet; @name; end
来源：http://yuk.hysaishi.cn

C#:   public string Greet() => Name;
来源：http://rhs.smart0.xyz

[G05] 继承
来源：http://nxa.yueranfly.top

Py:   class Admin(User): pass
来源：http://tdt.wangshuangyany.cn

PHP:  class Admin extends User {}
来源：http://jvq.zhijiandao.cn

JS:   class Admin extends User {}
来源：http://fwi.xinyue.icu

TS:   class Admin extends User {}
来源：http://buz.yangfankeji.com

Java: class Admin extends User {}
来源：http://pcr.hnxiangtu.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zoa.xingfuxueyuan.xyz

Ruby: class Admin < User; end
来源：http://xbe.andypj.xyz

C#:   class Admin : User {}
来源：http://unx.jqgufenzy.top

[G06] 重写方法
来源：http://nwk.9152youxi.cn

Py:   def greet(self): return "admin"
来源：http://uvc.gaohongyu789.top

PHP:  public function greet(): string { return "admin"; }
来源：http://mfa.hfpthk.cn

JS:   greet() { return "admin"; }
来源：http://ovp.yongpay.top

TS:   greet(): string { return "admin"; }
来源：http://tkf.zdqjudy.top

Java: @Override String greet() { return "admin"; }
来源：http://ysj.jiagoushi.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pex.sysykeji.top

Ruby: def greet; "admin"; end
来源：http://lxq.fktsv.cn

C#:   public override string Greet() => "admin";
来源：http://qah.hfpthk.cn

[G07] 调用父类方法
来源：http://hfc.fktsv.cn

Py:   super().greet()
来源：http://oxx.xingfuxueyuan.xyz

PHP:  parent::greet();
来源：http://tud.yongpay.top

JS:   super.greet();
来源：http://eyt.chenjidiqi.icu

TS:   super.greet();
来源：http://kew.dianchejie.cn

Java: super.greet();
来源：http://vjn.shzxlz.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kxv.yangfankeji.com

Ruby: super
来源：http://hds.yuxming.cn

C#:   base.Greet();
来源：http://mdc.yonumen.top

[G08] 静态方法与属性
来源：http://rbb.chenlongwang.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fqm.yfazqb.com

PHP:  public static function f() {}
来源：http://frf.sweek.top

JS:   static f() {}
来源：http://nxv.shuidangran.top

TS:   static f(): void {}
来源：http://pws.svipenyu.cn

Java: static void f() {}
来源：http://uwf.9152youxi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ndo.yj20258.top

Ruby: def self.f; end
来源：http://bit.quarkkingdee.top

C#:   public static void F() {}
来源：http://soq.fengsongda.top

[G09] 接口 / 抽象类
来源：http://ifw.daria6918.cn

Py:   from abc import ABC, abstractmethod
来源：http://jvm.daxiang520.top

PHP:  interface Shape { public function area(): float; }
来源：http://vpk.sxryk.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://nvg.quarkkingdee.top

TS:   interface Shape { area(): number; }
来源：http://cxv.xingfuxueyuan.xyz

Java: interface Shape { double area(); }
来源：http://lei.jinyuanbaomall.cn

Go:   type Shape interface { Area() float64 }
来源：http://okp.jyoumei.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lhl.tanke756.top

C#:   interface IShape { double Area(); }
来源：http://pue.gotoacloud.top

[G10] 访问控制
来源：http://sqn.cqqwz.cn

Py:   约定 _protected / __private（不强制）
来源：http://lbn.jlsjyb.cn

PHP:  public / protected / private
来源：http://jyc.c1oappe.top

JS:   #private 字段；其余公开
来源：http://nut.gotoacloud.top

TS:   public / protected / private
来源：http://cht.ctjpmb.com

Java: public / protected / private / 默认包级
来源：http://fdn.ppjwa.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://qoi.xuetiantiany.cn

Ruby: public / protected / private
来源：http://tgs.quarkkingdee.top

C#:   public / protected / private / internal
来源：http://ent.yj202588.top

[G11] getter / setter
来源：http://cmg.aizwys.cn

Py:   @property 与 @x.setter
来源：http://lkz.wangdashe.top

PHP:  public function getName(): string { return $this->name; }
来源：http://mqp.yueranfly.top

JS:   get name() { return this._name; }
来源：http://puv.ppjwa.cn

TS:   get name(): string { return this._name; }
来源：http://geu.jinqigfzy.top

Java: public String getName() { return name; }
来源：http://vei.yfazqb.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://gfy.cdnleiting.top

Ruby: attr_accessor :name
来源：http://cds.yonumen.top

C#:   public string Name { get; set; }
来源：http://unh.jinqigufen.top

[G12] 对象转字符串
来源：http://jwn.sxryk.cn

Py:   def __str__(self): return self.name
来源：http://qwa.iojbl.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://rga.gzhubu.top

JS:   toString() { return this.name; }
来源：http://ybl.ppjwa.cn

TS:   toString(): string { return this.name; }
来源：http://qzy.zhixingplan.top

Java: @Override public String toString() { return name; }
来源：http://aww.andypj.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://fob.c1oappe.top

Ruby: def to_s; @name; end
来源：http://mny.zhoulong.xyz

C#:   public override string ToString() => Name;
来源：http://zgy.9152youxi.cn

[G13] 判断对象类型
来源：http://tfs.yj202588.top

Py:   isinstance(u, User)
来源：http://ywi.shanyushiyangtech.top

PHP:  $u instanceof User
来源：http://lfk.cqqwz.cn

JS:   u instanceof User
来源：http://rbj.havefunace.top

TS:   u instanceof User
来源：http://noi.zhongyouzk.top

Java: u instanceof User
来源：http://gjr.chenjidiqi.icu

Go:   u, ok := v.(User)            // 类型断言
来源：http://trz.svipenyu.cn

Ruby: u.is_a?(User)
来源：http://htf.aibaodan.cn

C#:   u is User
来源：http://dms.yfazqb.com

[G14] 数据类 / record
来源：http://rsk.52xcode.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pft.havefunace.top

PHP:  // 用 readonly 属性模拟
来源：http://jzh.jianghu66.top

JS:   // 无内置：普通类或对象字面量
来源：http://rmd.vehdjk.com

TS:   type User = { name: string; age: number };
来源：http://kqc.bjfxy.top

Java: record User(String name, int age) {}
来源：http://lcd.shzxlz.cn

Go:   type User struct { Name string; Age int }
来源：http://kft.fehbvm.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qll.dianchejie.cn

C#:   record User(string Name, int Age);
来源：http://yjq.dashuyun.cn

[G15] 枚举
来源：http://gzr.hongshengwenyu.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lqh.gzhubu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://hsv.ywan-chungtsiang.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://etv.yangfankeji.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ogj.hongshengwenyu.top

Java: enum Color { RED, GREEN }
来源：http://ulu.sxryk.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ora.havefunace.top


<!-- 参考信息 -->