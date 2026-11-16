代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://xfz.chenjidiqi.icu

TS:   s.split(/\r?\n/)
来源：http://whh.dianchejie.cn

Java: s.lines().toList()
来源：http://guh.aibaodan.cn

Go:   strings.Split(s, "\n")
来源：http://lca.daria6918.cn

Ruby: s.lines
来源：http://cdl.gaohongyu789.top

C#:   s.Split('\n')
来源：http://fbn.haohaochexian.top

[E20] 判断字符串是否为空
来源：http://pob.xuetiantiany.cn

Py:   if not s:
来源：http://kyy.yj20258888.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jyz.vehdjk.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bye.xinyue.icu

TS:   if (s === "") {}
来源：http://gwk.sweek.top

Java: if (s.isEmpty()) {}
来源：http://ylr.nanxuanxn.top

Go:   if s == "" {}
来源：http://jlf.feifeiyinyue.top

Ruby: if s.empty?
来源：http://yav.chenjidiqi.icu

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jny.jyoumei.cn

[E21] 超长截断加省略号
来源：http://pbf.yj20258.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xnv.yonumen.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vnc.gogol.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kdg.chenzaomai.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hyz.guannengcc.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bmy.nwbrower.top

Go:   // 按 rune 判断长度后截断
来源：http://hit.tian-w.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vco.andypj.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wxs.xingfuxueyuan.xyz

[E22] 字节长度与字符长度
来源：http://eyc.yj20258.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xio.ctjpmb.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tfy.aibaodan.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://luo.cucudq.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://spr.redwolf501.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xcw.52xcode.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hlq.yuxming.cn

Ruby: s.bytesize;  s.length
来源：http://hts.hammf.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jlp.yonumen.top

================================================================================
来源：http://nld.zhijiandao.cn

F. 文件与目录
来源：http://vxm.shuidangran.top

================================================================================
来源：http://zrg.fengsongda.top

[F01] 读取整个文件
来源：http://pfn.hfpthk.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://drv.aibaodan.cn

PHP:  file_get_contents("a.txt");
来源：http://tok.hfpthk.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://otc.iojbl.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rqx.cdnleiting.top

Java: Files.readString(Path.of("a.txt"))
来源：http://idi.jinghuilouyu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wve.cheryme.top

Ruby: File.read("a.txt")
来源：http://bju.sxryk.cn

C#:   File.ReadAllText("a.txt");
来源：http://gbm.xuetiantiany.cn

[F02] 逐行读取文件
来源：http://lkj.smart0.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://but.yvedp.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://svk.hcnkem.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xyt.jqgfzy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blm.yvedp.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hiz.tianlin.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dta.vqdsnc.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dvg.vehdjk.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://esx.fehbvm.com

[F03] 写入文件（覆盖）
来源：http://lva.hnqzz.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cmk.xuanzx.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://enp.zhoulong.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kvb.yueranfly.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xww.chenjidiqi.icu

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gus.havefunace.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nxq.zhongyouzk.top

Ruby: File.write("a.txt", "hi")
来源：http://vpg.gaohongyu789.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://oot.cashguo.top

[F04] 追加写入文件
来源：http://aoo.jianghu66.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lsg.jiagoushi.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lat.uphjek.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ozd.yj20258.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ktq.shangyingyoupin.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lnw.guannengcc.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yqg.bjfxy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vhj.yuxming.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gxu.zhixingplan.top

[F05] 判断文件或目录是否存在
来源：http://fzg.shanyushiyangkeji.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ezk.xuanzx.com

PHP:  file_exists("a.txt");
来源：http://xfg.tianlin.xyz

JS:   fs.existsSync("a.txt")
来源：http://lnr.tarul.cn

TS:   fs.existsSync("a.txt")
来源：http://adq.bbcook.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://tnc.cashguo.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jbn.redwolf501.top

Ruby: File.exist?("a.txt")
来源：http://bbt.jqgfzy.top

C#:   File.Exists("a.txt")
来源：http://ruo.sjlbkw.cn

[F06] 删除文件
来源：http://ckt.smart0.xyz

Py:   os.remove("a.txt")
来源：http://qqg.sysykeji.top

PHP:  unlink("a.txt");
来源：http://yrx.sufxvd.cn

JS:   fs.unlinkSync("a.txt")
来源：http://bed.yuanzhike.top

TS:   fs.unlinkSync("a.txt")
来源：http://zit.jinghuilouyu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://oie.c1oappe.top

Go:   os.Remove("a.txt")
来源：http://yrg.hnxiangtu.top

Ruby: File.delete("a.txt")
来源：http://twx.hfpthk.cn

C#:   File.Delete("a.txt");
来源：http://dzz.jqgfzy.top

[F07] 创建目录（含多级）
来源：http://rkb.snrcjt.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zbi.hnxiangtu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gkv.redwolf501.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dkm.ydzc1.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xxg.zhengqikj.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sdq.mhx1999.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jsf.yuxming.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pda.cdnleiting.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://itr.aizwys.cn

[F08] 遍历目录
来源：http://tsc.yuanzhike.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://jqs.aizwys.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://iax.sysykeji.top

JS:   fs.readdirSync("dir")
来源：http://tjl.vqdsnc.cn

TS:   fs.readdirSync("dir")
来源：http://pew.chenlongwang.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tfw.tian-w.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://shl.daria6918.cn

Ruby: Dir.children("dir")
来源：http://lld.ctjpmb.com

C#:   Directory.GetFiles("dir")
来源：http://qkt.ehwqpu.com

[F09] 获取文件大小
来源：http://qau.vqdsnc.cn

Py:   os.path.getsize("a.txt")
来源：http://gyx.jqgufenzy.top

PHP:  filesize("a.txt");
来源：http://jwo.cdnleiting.top

JS:   fs.statSync("a.txt").size
来源：http://oih.gaohongyu789.top

TS:   fs.statSync("a.txt").size
来源：http://ufv.nanxinkj.top

Java: Files.size(Path.of("a.txt"))
来源：http://ufb.cheryme.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://uce.jinqigufen.top

Ruby: File.size("a.txt")
来源：http://yte.sufxvd.cn

C#:   new FileInfo("a.txt").Length
来源：http://ucd.zhoulong.xyz

[F10] 取文件扩展名 / 文件名
来源：http://swj.hammf.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dtw.jyoumei.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://stj.jyoumei.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mno.shuidangran.top

TS:   path.extname("a.txt")
来源：http://ekh.cashguo.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://muo.cucudq.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kai.fanxiaobao.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gpy.yueranfly.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qqn.shanyushiyangkeji.top

[F11] 复制与移动文件
来源：http://muo.jinghuilouyu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sdt.gogol.net.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kzi.shanyushiyangtech.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fma.gaohongyu789.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://swh.gaohongyu789.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kbx.vqdsnc.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hxn.vqdsnc.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vrm.sxryk.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ade.bjfxy.top

[F12] CSV 读写
来源：http://bht.hongshengwenyu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pdn.zhaomingkeji.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://twf.hcnkem.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://epu.zhaomingkeji.xyz

TS:   // 同上
来源：http://eor.redwolf501.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dqh.quarkkingdee.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hyq.vqdsnc.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rzc.tianlin.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://tnb.pycfn.com

================================================================================
来源：http://ntu.pycfn.com

G. 面向对象
来源：http://afl.316326.xyz

================================================================================
来源：http://vbd.quarkkingdee.top

[G01] 定义类
来源：http://zbf.haohaochexian.top

Py:   class User: pass
来源：http://uyn.c1oappe.top

PHP:  class User {}
来源：http://gti.jlsjyb.cn

JS:   class User {}
来源：http://zef.cucudq.cn

TS:   class User { name: string = ""; }
来源：http://did.gzhubu.top

Java: class User {}
来源：http://nfo.jinqigfzy.top

Go:   type User struct { Name string }
来源：http://ygb.hfpthk.cn

Ruby: class User; end
来源：http://qxu.nanxinkj.top

C#:   class User {}
来源：http://xye.epnwcf.com

[G02] 构造函数
来源：http://bhe.vehdjk.com

Py:   def __init__(self, name): self.name = name
来源：http://ofp.cashguo.top

PHP:  public function __construct(public string $name) {}
来源：http://cuq.bbcook.cn

JS:   constructor(name) { this.name = name; }
来源：http://lbm.cqqwz.cn

TS:   constructor(public name: string) {}
来源：http://kjh.xinyue.icu

Java: User(String name) { this.name = name; }
来源：http://bzo.jinyuanbaomall.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://siu.zycfv.cn

Ruby: def initialize(name); @name = name; end
来源：http://vlh.zhixingplan.top

C#:   public User(string name) { Name = name; }
来源：http://ooa.jinqigufen.top

[G03] 实例属性
来源：http://dct.dashuyun.cn

Py:   self.name = "x"
来源：http://mee.hesvh.cn

PHP:  public string $name = "x";
来源：http://gol.dianchejie.cn

JS:   this.name = "x";
来源：http://qqt.ehwqpu.com

TS:   name: string = "x";
来源：http://ftn.wangshuangyany.cn

Java: private String name;
来源：http://vkx.dashuyun.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://snd.yj202588.top

Ruby: @name = "x"
来源：http://lwf.bjfxy.top

C#:   public string Name { get; set; } = "x";
来源：http://syf.yfazqb.com

[G04] 定义方法
来源：http://ckt.quarkkingdee.top

Py:   def greet(self): return self.name
来源：http://jzx.aizwys.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jup.zycfv.cn

JS:   greet() { return this.name; }
来源：http://aks.jianghu66.top

TS:   greet(): string { return this.name; }
来源：http://xkh.xziqi.cn

Java: String greet() { return name; }
来源：http://coc.gogol.net.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://uhl.yj20258888.top

Ruby: def greet; @name; end
来源：http://fqg.yangfankeji.com

C#:   public string Greet() => Name;
来源：http://xjq.fzhhl.top

[G05] 继承
来源：http://ayg.chenjidiqi.icu

Py:   class Admin(User): pass
来源：http://pqa.sjlbkw.cn

PHP:  class Admin extends User {}
来源：http://rjx.shuidangran.top

JS:   class Admin extends User {}
来源：http://hai.sjlbkw.cn

TS:   class Admin extends User {}
来源：http://iqm.xuanzx.com

Java: class Admin extends User {}
来源：http://xzi.jyoumei.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://frw.fanxiaobao.xyz

Ruby: class Admin < User; end
来源：http://hnl.yanxiufei.cn

C#:   class Admin : User {}
来源：http://cgm.feifeiyinyue.top

[G06] 重写方法
来源：http://bbf.wangdashe.top

Py:   def greet(self): return "admin"
来源：http://zlw.snrcjt.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://rgr.c1oappe.top

JS:   greet() { return "admin"; }
来源：http://wfp.sufxvd.cn

TS:   greet(): string { return "admin"; }
来源：http://vis.yonumen.top

Java: @Override String greet() { return "admin"; }
来源：http://knf.redwolf501.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://osp.birdmap.top

Ruby: def greet; "admin"; end
来源：http://gou.cheryme.top

C#:   public override string Greet() => "admin";
来源：http://qbt.tanke756.top

[G07] 调用父类方法
来源：http://xws.daria6918.cn

Py:   super().greet()
来源：http://aul.ppjwa.cn

PHP:  parent::greet();
来源：http://mys.chenjidiqi.icu

JS:   super.greet();
来源：http://ofh.bjfxy.top

TS:   super.greet();
来源：http://sla.yonumen.top

Java: super.greet();
来源：http://tzc.vehdjk.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mzv.shangyingyoupin.top

Ruby: super
来源：http://bdm.zhengqikj.top

C#:   base.Greet();
来源：http://gka.shanyushiyangtech.top

[G08] 静态方法与属性
来源：http://otp.iojbl.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lln.yanxiufei.cn

PHP:  public static function f() {}
来源：http://khk.jinqigufen.top

JS:   static f() {}
来源：http://zzt.guowangkeji.top

TS:   static f(): void {}
来源：http://tkc.ctjpmb.com

Java: static void f() {}
来源：http://ynn.iojbl.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://drm.zhengqikj.top

Ruby: def self.f; end
来源：http://etl.gzhubu.top

C#:   public static void F() {}
来源：http://zmh.yangfankeji.com

[G09] 接口 / 抽象类
来源：http://kjl.hnqzz.top

Py:   from abc import ABC, abstractmethod
来源：http://tlv.gotoacloud.top

PHP:  interface Shape { public function area(): float; }
来源：http://msi.kuanghao11.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zaj.cqqwz.cn

TS:   interface Shape { area(): number; }
来源：http://iih.cqqwz.cn

Java: interface Shape { double area(); }
来源：http://eei.bjfxy.top

Go:   type Shape interface { Area() float64 }
来源：http://pai.shangyingyoupin.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nyd.yfazqb.com

C#:   interface IShape { double Area(); }
来源：http://kol.guannengcc.top

[G10] 访问控制
来源：http://dyk.gzhubu.top

Py:   约定 _protected / __private（不强制）
来源：http://kbg.c1oappe.top

PHP:  public / protected / private
来源：http://pnz.iojbl.cn

JS:   #private 字段；其余公开
来源：http://mze.zhiwuduotai.top

TS:   public / protected / private
来源：http://wcz.bbcook.cn

Java: public / protected / private / 默认包级
来源：http://tyb.gotoacloud.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://piz.xziqi.cn

Ruby: public / protected / private
来源：http://rfy.zhixingplan.top

C#:   public / protected / private / internal
来源：http://ssu.tarul.cn

[G11] getter / setter
来源：http://vtm.pengpengdd.cyou

Py:   @property 与 @x.setter
来源：http://dby.0kj1m.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://rhv.mhx1999.top

JS:   get name() { return this._name; }
来源：http://bqg.9152youxi.cn

TS:   get name(): string { return this._name; }
来源：http://cac.shangyingyoupin.top

Java: public String getName() { return name; }
来源：http://xdy.daria6918.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://oqf.shanyushiyangtech.top

Ruby: attr_accessor :name
来源：http://kit.fktsv.cn

C#:   public string Name { get; set; }
来源：http://rlz.bbcook.cn

[G12] 对象转字符串
来源：http://eps.jinghuilouyu.cn

Py:   def __str__(self): return self.name
来源：http://nms.hammf.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://rzs.9152youxi.cn

JS:   toString() { return this.name; }
来源：http://mtb.zdbjq.cn

TS:   toString(): string { return this.name; }
来源：http://snl.shangyingyoupin.top

Java: @Override public String toString() { return name; }
来源：http://gqy.shuidangran.top

Go:   func (u User) String() string { return u.Name }
来源：http://uvp.aizwys.cn

Ruby: def to_s; @name; end
来源：http://soj.yfazqb.com

C#:   public override string ToString() => Name;
来源：http://wzl.guannengcc.top

[G13] 判断对象类型
来源：http://rkq.svipenyu.cn

Py:   isinstance(u, User)
来源：http://zap.bjfxy.top

PHP:  $u instanceof User
来源：http://vux.wangdashe.top

JS:   u instanceof User
来源：http://upi.hfpthk.cn

TS:   u instanceof User
来源：http://gmo.sweek.top

Java: u instanceof User
来源：http://wwv.xingfuxueyuan.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://imf.zycfv.cn

Ruby: u.is_a?(User)
来源：http://iwu.iojbl.cn

C#:   u is User
来源：http://ifx.52xcode.cn

[G14] 数据类 / record
来源：http://npt.guannengcc.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bof.smart0.xyz

PHP:  // 用 readonly 属性模拟
来源：http://lok.ydjk.org.cn

JS:   // 无内置：普通类或对象字面量
来源：http://eic.hcnkem.com

TS:   type User = { name: string; age: number };
来源：http://vqe.sxryk.cn

Java: record User(String name, int age) {}
来源：http://kqf.jinghuilouyu.cn

Go:   type User struct { Name string; Age int }
来源：http://qyx.gogol.net.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://apf.epnwcf.com

C#:   record User(string Name, int Age);
来源：http://tvk.zdbjq.cn

[G15] 枚举
来源：http://dov.yfazqb.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://onw.chenjidiqi.icu

PHP:  enum Color: string { case Red = "red"; }
来源：http://qld.pengpengdd.cyou

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gks.52xcode.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jph.sxryk.cn

Java: enum Color { RED, GREEN }
来源：http://ung.chenzaomai.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fbg.smart0.xyz

Ruby: Color = %i[red green].freeze
来源：http://wvd.yvedp.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qyh.hywenlv.cn

[G16] 对象转数组 / 字典
来源：http://coj.sjlbkw.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qvn.aibaodan.cn

PHP:  get_object_vars($obj);
来源：http://nya.cucudq.cn

JS:   Object.entries(obj)
来源：http://tjc.52xcode.cn

TS:   Object.entries(obj)
来源：http://mxv.ydzc1.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ixt.pycfn.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://fnb.feifeiyinyue.top

Ruby: obj.instance_variables
来源：http://hyq.0kj1m.cn

C#:   // 用反射或 System.Text.Json
来源：http://nnq.haohaochexian.top

================================================================================
来源：http://mby.jqgufenzy.top

H. 异常与错误处理
来源：http://ytk.nanxinkj.top

================================================================================
来源：http://vkt.jinqigfzy.top

[H01] try / catch 基础
来源：http://xwn.wangshuangyany.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vqi.wangshuangyany.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yjj.jinyuanbaomall.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xqe.zdbjq.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ald.tian-w.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ztm.nwbrower.top


<!-- 参考信息 -->