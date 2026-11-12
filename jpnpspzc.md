代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bhs.yj202588.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cmp.shuidangran.top

Ruby: s.capitalize
来源：http://klc.cdnleiting.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ibg.epnwcf.com

[E18] 模板占位符替换
来源：http://ufl.snrcjt.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sgj.fengsongda.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://edt.ydjk.org.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://edq.hcnkem.com

TS:   tpl.replaceAll("{name}", name)
来源：http://dok.guowangkeji.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mzv.yangfankeji.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://phj.jyoumei.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dgi.birdmap.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ycr.andypj.xyz

[E19] 多行文本按行拆分
来源：http://mvr.bbcook.cn

Py:   s.splitlines()
来源：http://quz.yangfankeji.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blc.redwolf501.top

JS:   s.split(/\r?\n/)
来源：http://glr.birdmap.top

TS:   s.split(/\r?\n/)
来源：http://uky.chenjidiqi.icu

Java: s.lines().toList()
来源：http://bfx.ppjwa.cn

Go:   strings.Split(s, "\n")
来源：http://ilw.zhongyouzk.top

Ruby: s.lines
来源：http://kgu.birdmap.top

C#:   s.Split('\n')
来源：http://beo.fengsongda.top

[E20] 判断字符串是否为空
来源：http://jto.gaohongyu789.top

Py:   if not s:
来源：http://ifs.fanxiaobao.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qvj.jiagoushi.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lkm.hywenlv.cn

TS:   if (s === "") {}
来源：http://uii.ywan-chungtsiang.top

Java: if (s.isEmpty()) {}
来源：http://jwq.sufxvd.cn

Go:   if s == "" {}
来源：http://ycg.jqgufenzy.top

Ruby: if s.empty?
来源：http://ooo.jlsjyb.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yec.dashuyun.cn

[E21] 超长截断加省略号
来源：http://dag.jiagoushi.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blv.xuanzx.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://uzk.tian-w.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nkg.jinyuanbaomall.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://low.nanxuanxn.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fqy.zycfv.cn

Go:   // 按 rune 判断长度后截断
来源：http://qjb.zycfv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kgk.hywenlv.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sek.zhiwuduotai.top

[E22] 字节长度与字符长度
来源：http://ifs.guowangkeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://iwy.shanyushiyangtech.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yti.52xcode.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://obm.ivvv.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lqp.hnqzz.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kem.yuanzhike.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ddb.shanyushiyangtech.top

Ruby: s.bytesize;  s.length
来源：http://qtv.xinyue.icu

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://oum.hesvh.cn

================================================================================
来源：http://ftq.hnqzz.top

F. 文件与目录
来源：http://amb.andypj.xyz

================================================================================
来源：http://zrz.gaohongyu789.top

[F01] 读取整个文件
来源：http://kvg.hammf.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vdb.pengpengdd.cyou

PHP:  file_get_contents("a.txt");
来源：http://vfl.zhaomingkeji.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yal.fehbvm.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://otw.aizwys.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://quk.haohaochexian.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ksw.wangdashe.top

Ruby: File.read("a.txt")
来源：http://wpj.guannengcc.top

C#:   File.ReadAllText("a.txt");
来源：http://bjj.birdmap.top

[F02] 逐行读取文件
来源：http://pwx.jinqigufen.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hhu.vehdjk.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://isp.mhx1999.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vrn.meibo888.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://prx.shanyushiyangkeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://oqg.daria6918.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vso.cheryme.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fwh.zhixingplan.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://opz.zhongyouzk.top

[F03] 写入文件（覆盖）
来源：http://oeh.fehbvm.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://uuz.feifeiyinyue.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ydg.sxryk.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://djk.hfpthk.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xia.yanxiufei.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://puz.fktsv.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nix.yonumen.top

Ruby: File.write("a.txt", "hi")
来源：http://bvv.redwolf501.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qpp.jianghu66.top

[F04] 追加写入文件
来源：http://ldj.jlsjyb.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rnk.yanxiufei.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://czo.zycfv.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tkm.sjlbkw.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mxw.hnqzz.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fcx.daria6918.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vkt.cheryme.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cpf.316326.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vrl.ehwqpu.com

[F05] 判断文件或目录是否存在
来源：http://oee.zhixingplan.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jcw.cqqwz.cn

PHP:  file_exists("a.txt");
来源：http://tau.quarkkingdee.top

JS:   fs.existsSync("a.txt")
来源：http://iye.quarkkingdee.top

TS:   fs.existsSync("a.txt")
来源：http://eve.tarul.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://snp.pycfn.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ikn.shuidangran.top

Ruby: File.exist?("a.txt")
来源：http://ust.jinghuilouyu.cn

C#:   File.Exists("a.txt")
来源：http://jcv.yonumen.top

[F06] 删除文件
来源：http://evp.yj20258888.top

Py:   os.remove("a.txt")
来源：http://jhg.aizwys.cn

PHP:  unlink("a.txt");
来源：http://aac.zhiwuduotai.top

JS:   fs.unlinkSync("a.txt")
来源：http://iuq.jqgfzy.top

TS:   fs.unlinkSync("a.txt")
来源：http://yra.yfazqb.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ufe.yfazqb.com

Go:   os.Remove("a.txt")
来源：http://mvz.smart0.xyz

Ruby: File.delete("a.txt")
来源：http://vnw.shanyushiyangtech.top

C#:   File.Delete("a.txt");
来源：http://juu.fehbvm.com

[F07] 创建目录（含多级）
来源：http://qby.xziqi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gen.yanxiufei.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pes.hcnkem.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jng.ywan-chungtsiang.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kla.redwolf501.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kjk.yj20258.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gib.316326.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://chj.sysykeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zuv.hammf.cn

[F08] 遍历目录
来源：http://svz.shzxlz.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://hoe.jyoumei.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jeg.zhengqikj.top

JS:   fs.readdirSync("dir")
来源：http://rym.zhongyouzk.top

TS:   fs.readdirSync("dir")
来源：http://npu.xinyue.icu

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://whj.jinqigfzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ega.zhongyouzk.top

Ruby: Dir.children("dir")
来源：http://yxy.cqqwz.cn

C#:   Directory.GetFiles("dir")
来源：http://ibl.feifeiyinyue.top

[F09] 获取文件大小
来源：http://mlw.jinyuanbaomall.cn

Py:   os.path.getsize("a.txt")
来源：http://ocr.316326.xyz

PHP:  filesize("a.txt");
来源：http://wxj.havefunace.top

JS:   fs.statSync("a.txt").size
来源：http://qvz.xziqi.cn

TS:   fs.statSync("a.txt").size
来源：http://lzx.yanxiufei.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ovy.nanxuanxn.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://axd.gzhubu.top

Ruby: File.size("a.txt")
来源：http://pmw.tian-w.cn

C#:   new FileInfo("a.txt").Length
来源：http://xrc.jiagoushi.top

[F10] 取文件扩展名 / 文件名
来源：http://myo.hongshengwenyu.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pow.uphjek.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sny.316326.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xoj.bjfxy.top

TS:   path.extname("a.txt")
来源：http://ceu.jinghuilouyu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mhx.ydzc1.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vwd.aibaodan.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dwt.sysykeji.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ygy.ydjk.org.cn

[F11] 复制与移动文件
来源：http://wbp.epnwcf.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pbf.tianlin.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://twc.nanxuanxn.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qnj.tianlin.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lbf.fanxiaobao.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://iac.quarkkingdee.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ime.fzhhl.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rnv.gzhubu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tep.snrcjt.cn

[F12] CSV 读写
来源：http://wwh.guowangkeji.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hti.ybcxt.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bkt.zhengqikj.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rtr.jinghuilouyu.cn

TS:   // 同上
来源：http://mbh.aizwys.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://oxr.redwolf501.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ohe.ctjpmb.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lth.yvedp.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://thm.cqqwz.cn

================================================================================
来源：http://yqh.sjlbkw.cn

G. 面向对象
来源：http://gew.xuanzx.com

================================================================================
来源：http://zgw.zhongyouzk.top

[G01] 定义类
来源：http://uru.hcnkem.com

Py:   class User: pass
来源：http://cdp.jianghu66.top

PHP:  class User {}
来源：http://sin.zhongyouzk.top

JS:   class User {}
来源：http://fyz.dashuyun.cn

TS:   class User { name: string = ""; }
来源：http://pmi.kuanghao11.cn

Java: class User {}
来源：http://yqh.gotoacloud.top

Go:   type User struct { Name string }
来源：http://ggu.cheryme.top

Ruby: class User; end
来源：http://axn.jinqigfzy.top

C#:   class User {}
来源：http://lzc.cheryme.top

[G02] 构造函数
来源：http://oos.ppjwa.cn

Py:   def __init__(self, name): self.name = name
来源：http://rhm.tian-w.cn

PHP:  public function __construct(public string $name) {}
来源：http://nba.52xcode.cn

JS:   constructor(name) { this.name = name; }
来源：http://sew.andypj.xyz

TS:   constructor(public name: string) {}
来源：http://bvq.tianlin.xyz

Java: User(String name) { this.name = name; }
来源：http://npo.dianchejie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://iph.tanke756.top

Ruby: def initialize(name); @name = name; end
来源：http://ndw.nanxuanxn.top

C#:   public User(string name) { Name = name; }
来源：http://rtc.jinqigfzy.top

[G03] 实例属性
来源：http://htx.aizwys.cn

Py:   self.name = "x"
来源：http://mpb.aibaodan.cn

PHP:  public string $name = "x";
来源：http://cgv.yonumen.top

JS:   this.name = "x";
来源：http://eye.hesvh.cn

TS:   name: string = "x";
来源：http://fov.fehbvm.com

Java: private String name;
来源：http://bcx.dianchejie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yqx.quarkkingdee.top

Ruby: @name = "x"
来源：http://zwg.cdnleiting.top

C#:   public string Name { get; set; } = "x";
来源：http://zdv.xuetiantiany.cn

[G04] 定义方法
来源：http://frx.bjfxy.top

Py:   def greet(self): return self.name
来源：http://jgy.wangshuangyany.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jrz.zhijiandao.cn

JS:   greet() { return this.name; }
来源：http://qsv.tianlin.xyz

TS:   greet(): string { return this.name; }
来源：http://qbt.fzhhl.top

Java: String greet() { return name; }
来源：http://woc.hammf.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bme.fanxiaobao.xyz

Ruby: def greet; @name; end
来源：http://ful.pycfn.com

C#:   public string Greet() => Name;
来源：http://jyi.jiagoushi.top

[G05] 继承
来源：http://kzl.daria6918.cn

Py:   class Admin(User): pass
来源：http://tae.xuanzx.com

PHP:  class Admin extends User {}
来源：http://umb.jiagoushi.top

JS:   class Admin extends User {}
来源：http://ivc.wangdashe.top

TS:   class Admin extends User {}
来源：http://gra.vehdjk.com

Java: class Admin extends User {}
来源：http://vom.yj20258.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://trs.yvedp.cn

Ruby: class Admin < User; end
来源：http://rtm.snrcjt.cn

C#:   class Admin : User {}
来源：http://ovt.tarul.cn

[G06] 重写方法
来源：http://war.epnwcf.com

Py:   def greet(self): return "admin"
来源：http://cmj.sysykeji.top

PHP:  public function greet(): string { return "admin"; }
来源：http://acx.gogol.net.cn

JS:   greet() { return "admin"; }
来源：http://bos.yj20258.top

TS:   greet(): string { return "admin"; }
来源：http://pnz.hnxiangtu.top

Java: @Override String greet() { return "admin"; }
来源：http://tpq.tian-w.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://aga.tarul.cn

Ruby: def greet; "admin"; end
来源：http://dkw.shanyushiyangtech.top

C#:   public override string Greet() => "admin";
来源：http://dta.shanyushiyangtech.top

[G07] 调用父类方法
来源：http://vpw.cqqwz.cn

Py:   super().greet()
来源：http://tip.hammf.cn

PHP:  parent::greet();
来源：http://lgr.jyoumei.cn

JS:   super.greet();
来源：http://fem.sufxvd.cn

TS:   super.greet();
来源：http://khd.mhx1999.top

Java: super.greet();
来源：http://agz.jinqigufen.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ten.jyoumei.cn

Ruby: super
来源：http://nbs.fengsongda.top

C#:   base.Greet();
来源：http://lwa.tanke756.top

[G08] 静态方法与属性
来源：http://nxm.gotoacloud.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vvf.jianghu66.top

PHP:  public static function f() {}
来源：http://yfp.hfpthk.cn

JS:   static f() {}
来源：http://tpq.jinqigufen.top

TS:   static f(): void {}
来源：http://idz.hammf.cn

Java: static void f() {}
来源：http://ibb.nwbrower.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ykg.quarkkingdee.top

Ruby: def self.f; end
来源：http://mck.zhongyouzk.top

C#:   public static void F() {}
来源：http://xsw.zdbjq.cn

[G09] 接口 / 抽象类
来源：http://ywo.yj20258.top

Py:   from abc import ABC, abstractmethod
来源：http://blu.zdqjudy.top

PHP:  interface Shape { public function area(): float; }
来源：http://gqj.daxiang520.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ovq.nwbrower.top

TS:   interface Shape { area(): number; }
来源：http://qzu.yangfankeji.com

Java: interface Shape { double area(); }
来源：http://lyn.shuidangran.top

Go:   type Shape interface { Area() float64 }
来源：http://hir.daria6918.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://otk.zhaomingkeji.xyz

C#:   interface IShape { double Area(); }
来源：http://kkf.sufxvd.cn

[G10] 访问控制
来源：http://dvb.jinqigfzy.top

Py:   约定 _protected / __private（不强制）
来源：http://tdr.guannengcc.top

PHP:  public / protected / private
来源：http://avv.epnwcf.com

JS:   #private 字段；其余公开
来源：http://udn.hcnkem.com

TS:   public / protected / private
来源：http://mgc.hywenlv.cn

Java: public / protected / private / 默认包级
来源：http://rvp.haohaochexian.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://yxv.cdnleiting.top

Ruby: public / protected / private
来源：http://dgk.zhoulong.xyz

C#:   public / protected / private / internal
来源：http://ljw.fanxiaobao.xyz

[G11] getter / setter
来源：http://zlz.aizwys.cn

Py:   @property 与 @x.setter
来源：http://ztb.yfazqb.com

PHP:  public function getName(): string { return $this->name; }
来源：http://ebf.yonumen.top

JS:   get name() { return this._name; }
来源：http://pjm.hfpthk.cn

TS:   get name(): string { return this._name; }
来源：http://leu.0kj1m.cn

Java: public String getName() { return name; }
来源：http://mdu.sufxvd.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://nwr.xuetiantiany.cn

Ruby: attr_accessor :name
来源：http://uhm.zhixingplan.top

C#:   public string Name { get; set; }
来源：http://mbj.pycfn.com

[G12] 对象转字符串
来源：http://ihn.fehbvm.com

Py:   def __str__(self): return self.name
来源：http://wws.shanyushiyangtech.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://oil.kuanghao11.cn

JS:   toString() { return this.name; }
来源：http://zsl.zhoulong.xyz

TS:   toString(): string { return this.name; }
来源：http://llx.tianlin.xyz

Java: @Override public String toString() { return name; }
来源：http://pvd.shanyushiyangtech.top

Go:   func (u User) String() string { return u.Name }
来源：http://iie.tanke756.top

Ruby: def to_s; @name; end
来源：http://bbm.dianchejie.cn

C#:   public override string ToString() => Name;
来源：http://trk.svipenyu.cn

[G13] 判断对象类型
来源：http://gbc.redwolf501.top

Py:   isinstance(u, User)
来源：http://pjy.ivvv.top

PHP:  $u instanceof User
来源：http://lso.ywan-chungtsiang.top

JS:   u instanceof User
来源：http://txm.pycfn.com

TS:   u instanceof User
来源：http://kso.dashuyun.cn

Java: u instanceof User
来源：http://lur.yongpay.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://qea.c1oappe.top

Ruby: u.is_a?(User)
来源：http://pwc.zhoulong.xyz

C#:   u is User
来源：http://ijn.zhengqikj.top

[G14] 数据类 / record
来源：http://ytl.yonumen.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rqc.snrcjt.cn

PHP:  // 用 readonly 属性模拟
来源：http://nja.vehdjk.com

JS:   // 无内置：普通类或对象字面量
来源：http://tcp.ppjwa.cn

TS:   type User = { name: string; age: number };
来源：http://ped.uphjek.com

Java: record User(String name, int age) {}
来源：http://xnu.zhixingplan.top

Go:   type User struct { Name string; Age int }
来源：http://jjd.xziqi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vwc.meibo888.top

C#:   record User(string Name, int Age);
来源：http://gde.yangfankeji.com

[G15] 枚举
来源：http://zlk.yuxming.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://elz.gzhubu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ufr.cheryme.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qiv.tanke756.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://snl.sufxvd.cn

Java: enum Color { RED, GREEN }
来源：http://asg.cucudq.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kaz.xuanzx.com

Ruby: Color = %i[red green].freeze
来源：http://oss.tian-w.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wdu.iojbl.cn

[G16] 对象转数组 / 字典
来源：http://pte.iojbl.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://aeg.havefunace.top


<!-- 参考信息 -->