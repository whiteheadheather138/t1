代发 wailian999

[E18] 模板占位符替换
来源：http://ilc.xinyue.icu

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ycw.meibo888.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hlm.ppjwa.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wdh.fehbvm.com

TS:   tpl.replaceAll("{name}", name)
来源：http://bug.xinyue.icu

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hwj.zhengqikj.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rfn.feifeiyinyue.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wfa.daxiang520.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bef.pengpengdd.cyou

[E19] 多行文本按行拆分
来源：http://kht.chenzaomai.com

Py:   s.splitlines()
来源：http://zub.xuanzx.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xfw.xziqi.cn

JS:   s.split(/\r?\n/)
来源：http://miu.ehwqpu.com

TS:   s.split(/\r?\n/)
来源：http://yrt.fktsv.cn

Java: s.lines().toList()
来源：http://bij.daria6918.cn

Go:   strings.Split(s, "\n")
来源：http://zht.fehbvm.com

Ruby: s.lines
来源：http://rtu.yj202588.top

C#:   s.Split('\n')
来源：http://dxs.xuetiantiany.cn

[E20] 判断字符串是否为空
来源：http://qay.cqqwz.cn

Py:   if not s:
来源：http://gpn.shanyushiyangtech.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mak.jinyuanbaomall.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hsd.ctjpmb.com

TS:   if (s === "") {}
来源：http://ukx.jinyuanbaomall.cn

Java: if (s.isEmpty()) {}
来源：http://qtb.guannengcc.top

Go:   if s == "" {}
来源：http://wur.yanxiufei.cn

Ruby: if s.empty?
来源：http://bsk.ehwqpu.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wqw.tianlin.xyz

[E21] 超长截断加省略号
来源：http://dgu.ehwqpu.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hvc.nanxuanxn.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://loj.jinghuilouyu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wcm.zhaomingkeji.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dum.nwbrower.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qvc.guowangkeji.top

Go:   // 按 rune 判断长度后截断
来源：http://myy.shanyushiyangkeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dhm.jinqigufen.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jal.tanke756.top

[E22] 字节长度与字符长度
来源：http://alk.tanke756.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://izi.kuanghao11.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nsm.xinyue.icu

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xtx.sufxvd.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jpx.pengpengdd.cyou

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://eaa.nanxuanxn.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://thm.guannengcc.top

Ruby: s.bytesize;  s.length
来源：http://awz.tanke756.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cqm.yongpay.top

================================================================================
来源：http://ftg.hysaishi.cn

F. 文件与目录
来源：http://nyf.gzhubu.top

================================================================================
来源：http://kbd.hywenlv.cn

[F01] 读取整个文件
来源：http://gme.jianghu66.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://caj.wangshuangyany.cn

PHP:  file_get_contents("a.txt");
来源：http://nsk.yfazqb.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kws.316326.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xjp.tanke756.top

Java: Files.readString(Path.of("a.txt"))
来源：http://eti.cucudq.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kqw.cheryme.top

Ruby: File.read("a.txt")
来源：http://laa.ehwqpu.com

C#:   File.ReadAllText("a.txt");
来源：http://kuj.jiagoushi.top

[F02] 逐行读取文件
来源：http://qbc.hesvh.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://edo.yj20258888.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fwi.jinghuilouyu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vot.hnqzz.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gwn.redwolf501.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://imb.zhixingplan.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ack.daxiang520.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fqt.kuanghao11.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qsj.yueranfly.top

[F03] 写入文件（覆盖）
来源：http://cxa.hnqzz.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mtz.cashguo.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://hin.sufxvd.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://svi.haohaochexian.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qit.jinqigfzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sof.xuetiantiany.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sop.yuxming.cn

Ruby: File.write("a.txt", "hi")
来源：http://xmv.jiagoushi.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ebv.smart0.xyz

[F04] 追加写入文件
来源：http://tbh.316326.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://adk.yj20258.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nzm.dashuyun.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ecl.zycfv.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lha.zhiwuduotai.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hjs.yuanzhike.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wjk.wangshuangyany.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gwu.316326.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dsu.daria6918.cn

[F05] 判断文件或目录是否存在
来源：http://zoj.gogol.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dbl.cashguo.top

PHP:  file_exists("a.txt");
来源：http://cme.bjfxy.top

JS:   fs.existsSync("a.txt")
来源：http://ada.daria6918.cn

TS:   fs.existsSync("a.txt")
来源：http://tkd.tanke756.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ftk.chenlongwang.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fzz.nanxinkj.top

Ruby: File.exist?("a.txt")
来源：http://ayh.sysykeji.top

C#:   File.Exists("a.txt")
来源：http://iez.hysaishi.cn

[F06] 删除文件
来源：http://saq.chenjidiqi.icu

Py:   os.remove("a.txt")
来源：http://pzr.cucudq.cn

PHP:  unlink("a.txt");
来源：http://fsx.shanyushiyangkeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://oaf.jyoumei.cn

TS:   fs.unlinkSync("a.txt")
来源：http://bne.zhengqikj.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://iog.xziqi.cn

Go:   os.Remove("a.txt")
来源：http://vis.ydjk.org.cn

Ruby: File.delete("a.txt")
来源：http://mek.aizwys.cn

C#:   File.Delete("a.txt");
来源：http://wfl.meibo888.top

[F07] 创建目录（含多级）
来源：http://jex.hnxiangtu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zrb.ybcxt.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ksc.pycfn.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://waj.52xcode.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bqz.chenzaomai.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qou.zhiwuduotai.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rhn.nwbrower.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pyf.sufxvd.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ryz.shuidangran.top

[F08] 遍历目录
来源：http://fgo.shuidangran.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://xco.xinyue.icu

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tmg.cucudq.cn

JS:   fs.readdirSync("dir")
来源：http://tin.yj20258888.top

TS:   fs.readdirSync("dir")
来源：http://uvs.tanke756.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tyn.nwbrower.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://jkb.chenlongwang.top

Ruby: Dir.children("dir")
来源：http://rrv.ivvv.top

C#:   Directory.GetFiles("dir")
来源：http://ryv.kuanghao11.cn

[F09] 获取文件大小
来源：http://dmp.fanxiaobao.xyz

Py:   os.path.getsize("a.txt")
来源：http://dwh.hammf.cn

PHP:  filesize("a.txt");
来源：http://yix.sweek.top

JS:   fs.statSync("a.txt").size
来源：http://dmd.sysykeji.top

TS:   fs.statSync("a.txt").size
来源：http://dxp.chenlongwang.top

Java: Files.size(Path.of("a.txt"))
来源：http://vjr.smart0.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lpi.shzxlz.cn

Ruby: File.size("a.txt")
来源：http://ilq.52xcode.cn

C#:   new FileInfo("a.txt").Length
来源：http://fjn.hnqzz.top

[F10] 取文件扩展名 / 文件名
来源：http://wmp.dianchejie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nyr.epnwcf.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mjp.daxiang520.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dja.smart0.xyz

TS:   path.extname("a.txt")
来源：http://fkj.hnqzz.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yhz.c1oappe.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vii.jqgufenzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://faz.yvedp.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mxu.chenjidiqi.icu

[F11] 复制与移动文件
来源：http://nvc.zhijiandao.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fmt.daria6918.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://acp.yj20258888.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zcn.fehbvm.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rap.tarul.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nun.cashguo.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jhy.havefunace.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jtt.52xcode.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qut.zhiwuduotai.top

[F12] CSV 读写
来源：http://ber.zhiwuduotai.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qkq.jianghu66.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fcr.yanxiufei.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pie.jiagoushi.top

TS:   // 同上
来源：http://cva.cqqwz.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://azi.daxiang520.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kbj.zhongyouzk.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://weh.jinyuanbaomall.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://flo.vehdjk.com

================================================================================
来源：http://vhl.cdnleiting.top

G. 面向对象
来源：http://kuj.bbcook.cn

================================================================================
来源：http://wqp.fehbvm.com

[G01] 定义类
来源：http://mfa.sxryk.cn

Py:   class User: pass
来源：http://gze.hesvh.cn

PHP:  class User {}
来源：http://cji.shanyushiyangkeji.top

JS:   class User {}
来源：http://chs.xingfuxueyuan.xyz

TS:   class User { name: string = ""; }
来源：http://pne.nanxinkj.top

Java: class User {}
来源：http://hbt.snrcjt.cn

Go:   type User struct { Name string }
来源：http://eft.yongpay.top

Ruby: class User; end
来源：http://tvx.gotoacloud.top

C#:   class User {}
来源：http://rfv.zhoulong.xyz

[G02] 构造函数
来源：http://kil.jinqigfzy.top

Py:   def __init__(self, name): self.name = name
来源：http://zew.jinqigufen.top

PHP:  public function __construct(public string $name) {}
来源：http://cng.zhixingplan.top

JS:   constructor(name) { this.name = name; }
来源：http://zza.yonumen.top

TS:   constructor(public name: string) {}
来源：http://mnd.uphjek.com

Java: User(String name) { this.name = name; }
来源：http://gge.yj202588.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qdd.zhongyouzk.top

Ruby: def initialize(name); @name = name; end
来源：http://wvj.xuanzx.com

C#:   public User(string name) { Name = name; }
来源：http://hqe.yj20258.top

[G03] 实例属性
来源：http://dgg.jiagoushi.top

Py:   self.name = "x"
来源：http://cdg.guannengcc.top

PHP:  public string $name = "x";
来源：http://zdf.chenlongwang.top

JS:   this.name = "x";
来源：http://fgu.xuanzx.com

TS:   name: string = "x";
来源：http://sjh.xylfe.cn

Java: private String name;
来源：http://osc.xziqi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rcp.9152youxi.cn

Ruby: @name = "x"
来源：http://iua.uphjek.com

C#:   public string Name { get; set; } = "x";
来源：http://dcy.gogol.net.cn

[G04] 定义方法
来源：http://xpv.jlsjyb.cn

Py:   def greet(self): return self.name
来源：http://bdm.zhiwuduotai.top

PHP:  public function greet(): string { return $this->name; }
来源：http://gxm.feifeiyinyue.top

JS:   greet() { return this.name; }
来源：http://pju.tianlin.xyz

TS:   greet(): string { return this.name; }
来源：http://tlz.shangyingyoupin.top

Java: String greet() { return name; }
来源：http://gre.dianchejie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://idk.bbcook.cn

Ruby: def greet; @name; end
来源：http://zyq.nwbrower.top

C#:   public string Greet() => Name;
来源：http://ljg.chenzaomai.com

[G05] 继承
来源：http://lsf.guannengcc.top

Py:   class Admin(User): pass
来源：http://gyx.aizwys.cn

PHP:  class Admin extends User {}
来源：http://zcg.ydzc1.top

JS:   class Admin extends User {}
来源：http://cuc.andypj.xyz

TS:   class Admin extends User {}
来源：http://hke.9152youxi.cn

Java: class Admin extends User {}
来源：http://qda.wangshuangyany.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zoi.shangyingyoupin.top

Ruby: class Admin < User; end
来源：http://aua.hcnkem.com

C#:   class Admin : User {}
来源：http://tyh.aizwys.cn

[G06] 重写方法
来源：http://qwt.sxryk.cn

Py:   def greet(self): return "admin"
来源：http://eth.yanxiufei.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://puo.shanyushiyangtech.top

JS:   greet() { return "admin"; }
来源：http://svf.pengpengdd.cyou

TS:   greet(): string { return "admin"; }
来源：http://aba.cashguo.top

Java: @Override String greet() { return "admin"; }
来源：http://jpv.tian-w.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jrk.iojbl.cn

Ruby: def greet; "admin"; end
来源：http://jvy.epnwcf.com

C#:   public override string Greet() => "admin";
来源：http://hcs.aibaodan.cn

[G07] 调用父类方法
来源：http://gkd.yj20258888.top

Py:   super().greet()
来源：http://qvc.jinqigufen.top

PHP:  parent::greet();
来源：http://qwa.snrcjt.cn

JS:   super.greet();
来源：http://kxc.9152youxi.cn

TS:   super.greet();
来源：http://fjr.mhx1999.top

Java: super.greet();
来源：http://zhb.nanxuanxn.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zac.hongshengwenyu.top

Ruby: super
来源：http://fkl.epnwcf.com

C#:   base.Greet();
来源：http://piu.wangdashe.top

[G08] 静态方法与属性
来源：http://aeh.zhijiandao.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ejw.zhoulong.xyz

PHP:  public static function f() {}
来源：http://uhw.cucudq.cn

JS:   static f() {}
来源：http://ynb.epnwcf.com

TS:   static f(): void {}
来源：http://yyu.fengsongda.top

Java: static void f() {}
来源：http://bfr.zhongyouzk.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://diq.jinqigfzy.top

Ruby: def self.f; end
来源：http://lep.zhiwuduotai.top

C#:   public static void F() {}
来源：http://lal.jinyuanbaomall.cn

[G09] 接口 / 抽象类
来源：http://sdf.quarkkingdee.top

Py:   from abc import ABC, abstractmethod
来源：http://dee.xuanzx.com

PHP:  interface Shape { public function area(): float; }
来源：http://xos.ppjwa.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xmn.yangfankeji.com

TS:   interface Shape { area(): number; }
来源：http://cwa.tanke756.top

Java: interface Shape { double area(); }
来源：http://lpg.zhoulong.xyz

Go:   type Shape interface { Area() float64 }
来源：http://ffg.mhx1999.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://oiw.nanxuanxn.top

C#:   interface IShape { double Area(); }
来源：http://wgd.ivvv.top

[G10] 访问控制
来源：http://wre.dianchejie.cn

Py:   约定 _protected / __private（不强制）
来源：http://faf.sufxvd.cn

PHP:  public / protected / private
来源：http://svx.jyoumei.cn

JS:   #private 字段；其余公开
来源：http://obt.tian-w.cn

TS:   public / protected / private
来源：http://snn.kuanghao11.cn

Java: public / protected / private / 默认包级
来源：http://xrb.fzhhl.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://osp.fengsongda.top

Ruby: public / protected / private
来源：http://hhr.xylfe.cn

C#:   public / protected / private / internal
来源：http://bap.mhx1999.top

[G11] getter / setter
来源：http://roe.gzhubu.top

Py:   @property 与 @x.setter
来源：http://plv.redwolf501.top

PHP:  public function getName(): string { return $this->name; }
来源：http://xvs.snrcjt.cn

JS:   get name() { return this._name; }
来源：http://fph.hcnkem.com

TS:   get name(): string { return this._name; }
来源：http://jsc.chenjidiqi.icu

Java: public String getName() { return name; }
来源：http://kgm.shanyushiyangkeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://tny.ppjwa.cn

Ruby: attr_accessor :name
来源：http://qsk.cashguo.top

C#:   public string Name { get; set; }
来源：http://gbg.kuanghao11.cn

[G12] 对象转字符串
来源：http://znk.xinyue.icu

Py:   def __str__(self): return self.name
来源：http://weq.xylfe.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vld.xingfuxueyuan.xyz

JS:   toString() { return this.name; }
来源：http://oas.vehdjk.com

TS:   toString(): string { return this.name; }
来源：http://vbh.yuanzhike.top

Java: @Override public String toString() { return name; }
来源：http://qnv.cdnleiting.top

Go:   func (u User) String() string { return u.Name }
来源：http://byi.sysykeji.top

Ruby: def to_s; @name; end
来源：http://aem.daria6918.cn

C#:   public override string ToString() => Name;
来源：http://clo.zdqjudy.top

[G13] 判断对象类型
来源：http://fwq.cdnleiting.top

Py:   isinstance(u, User)
来源：http://pnv.andypj.xyz

PHP:  $u instanceof User
来源：http://iqg.feifeiyinyue.top

JS:   u instanceof User
来源：http://wgh.hongshengwenyu.top

TS:   u instanceof User
来源：http://ili.ivvv.top

Java: u instanceof User
来源：http://nee.jqgufenzy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://sbk.aizwys.cn

Ruby: u.is_a?(User)
来源：http://qny.birdmap.top

C#:   u is User
来源：http://evg.yfazqb.com

[G14] 数据类 / record
来源：http://dkt.fengsongda.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gbq.hnqzz.top

PHP:  // 用 readonly 属性模拟
来源：http://zxu.ppjwa.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vhs.nanxuanxn.top

TS:   type User = { name: string; age: number };
来源：http://pgk.yangfankeji.com

Java: record User(String name, int age) {}
来源：http://zsy.bjfxy.top

Go:   type User struct { Name string; Age int }
来源：http://fdb.ywan-chungtsiang.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jhk.gaohongyu789.top

C#:   record User(string Name, int Age);
来源：http://mqb.guowangkeji.top

[G15] 枚举
来源：http://nec.yueranfly.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nze.hnqzz.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://nhv.hysaishi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ine.gzhubu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://iwl.mhx1999.top

Java: enum Color { RED, GREEN }
来源：http://gyt.epnwcf.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lrh.fengsongda.top

Ruby: Color = %i[red green].freeze
来源：http://tqg.wangshuangyany.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bke.shanyushiyangkeji.top

[G16] 对象转数组 / 字典
来源：http://jwo.snrcjt.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lrv.xuetiantiany.cn

PHP:  get_object_vars($obj);
来源：http://pmc.hnqzz.top

JS:   Object.entries(obj)
来源：http://kng.jinyuanbaomall.cn

TS:   Object.entries(obj)
来源：http://oum.haohaochexian.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fin.shanyushiyangkeji.top


<!-- 参考信息 -->