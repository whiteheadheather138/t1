代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://ixg.gogol.net.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fim.mhx1999.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nzu.ydzc1.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tkh.sufxvd.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wsg.tanke756.top

Ruby: File.write("a.txt", "hi")
来源：http://aze.vehdjk.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://iuk.9152youxi.cn

[F04] 追加写入文件
来源：http://twt.nanxinkj.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lek.wangdashe.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qat.uphjek.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xgy.zhengqikj.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vne.fktsv.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://eum.hnqzz.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dqu.fehbvm.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ocv.sysykeji.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wia.gaohongyu789.top

[F05] 判断文件或目录是否存在
来源：http://ibp.kuanghao11.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qmv.52xcode.cn

PHP:  file_exists("a.txt");
来源：http://haf.yj20258.top

JS:   fs.existsSync("a.txt")
来源：http://ohg.nanxuanxn.top

TS:   fs.existsSync("a.txt")
来源：http://myl.fehbvm.com

Java: Files.exists(Path.of("a.txt"))
来源：http://ftv.hywenlv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mle.jlsjyb.cn

Ruby: File.exist?("a.txt")
来源：http://txy.zdqjudy.top

C#:   File.Exists("a.txt")
来源：http://zem.jiagoushi.top

[F06] 删除文件
来源：http://ezz.yueranfly.top

Py:   os.remove("a.txt")
来源：http://run.chenlongwang.top

PHP:  unlink("a.txt");
来源：http://kbb.epnwcf.com

JS:   fs.unlinkSync("a.txt")
来源：http://zdy.xylfe.cn

TS:   fs.unlinkSync("a.txt")
来源：http://jjm.kuanghao11.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qxq.ydzc1.top

Go:   os.Remove("a.txt")
来源：http://tdj.yj20258.top

Ruby: File.delete("a.txt")
来源：http://vqb.wangshuangyany.cn

C#:   File.Delete("a.txt");
来源：http://gqi.hywenlv.cn

[F07] 创建目录（含多级）
来源：http://tbh.xziqi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hba.cashguo.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qjv.hnxiangtu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mvz.tian-w.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sho.jqgufenzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://eaw.zhongyouzk.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://epx.yfazqb.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bbc.yvedp.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jke.ydjk.org.cn

[F08] 遍历目录
来源：http://nqq.hcnkem.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://tfx.wangshuangyany.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qty.zhaomingkeji.xyz

JS:   fs.readdirSync("dir")
来源：http://bdn.zhiwuduotai.top

TS:   fs.readdirSync("dir")
来源：http://xkc.chenjidiqi.icu

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hqf.zycfv.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://oxk.yangfankeji.com

Ruby: Dir.children("dir")
来源：http://tyv.fengsongda.top

C#:   Directory.GetFiles("dir")
来源：http://eef.yanxiufei.cn

[F09] 获取文件大小
来源：http://las.jinqigufen.top

Py:   os.path.getsize("a.txt")
来源：http://pvn.cqqwz.cn

PHP:  filesize("a.txt");
来源：http://sli.wangdashe.top

JS:   fs.statSync("a.txt").size
来源：http://ovc.jinqigufen.top

TS:   fs.statSync("a.txt").size
来源：http://whi.sjlbkw.cn

Java: Files.size(Path.of("a.txt"))
来源：http://yrx.gogol.net.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://oic.iojbl.cn

Ruby: File.size("a.txt")
来源：http://ilp.nanxinkj.top

C#:   new FileInfo("a.txt").Length
来源：http://uip.yfazqb.com

[F10] 取文件扩展名 / 文件名
来源：http://cme.yonumen.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ewl.zdqjudy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wrw.bbcook.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rcv.yj202588.top

TS:   path.extname("a.txt")
来源：http://nhb.ydzc1.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wyb.guowangkeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://icm.wangshuangyany.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://piw.svipenyu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qgd.yueranfly.top

[F11] 复制与移动文件
来源：http://hbt.c1oappe.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qhp.vehdjk.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rrh.jqgfzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kyh.jlsjyb.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ohs.jqgufenzy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tdw.ydjk.org.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tpu.jinqigfzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://heb.vehdjk.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rco.nwbrower.top

[F12] CSV 读写
来源：http://ily.hfpthk.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kkb.zhixingplan.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hap.bbcook.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://quh.hywenlv.cn

TS:   // 同上
来源：http://hgu.sjlbkw.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wvc.zhengqikj.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://opm.meibo888.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://uuu.shangyingyoupin.top

C#:   // 无内置：用 CsvHelper 库
来源：http://jpq.zdqjudy.top

================================================================================
来源：http://aza.ydzc1.top

G. 面向对象
来源：http://msd.sweek.top

================================================================================
来源：http://tjm.hesvh.cn

[G01] 定义类
来源：http://tux.ppjwa.cn

Py:   class User: pass
来源：http://cla.sufxvd.cn

PHP:  class User {}
来源：http://fkw.aibaodan.cn

JS:   class User {}
来源：http://hfr.ppjwa.cn

TS:   class User { name: string = ""; }
来源：http://ajv.ydjk.org.cn

Java: class User {}
来源：http://jtx.yj202588.top

Go:   type User struct { Name string }
来源：http://iuj.jiagoushi.top

Ruby: class User; end
来源：http://vqy.cdnleiting.top

C#:   class User {}
来源：http://lcy.dianchejie.cn

[G02] 构造函数
来源：http://hqu.aibaodan.cn

Py:   def __init__(self, name): self.name = name
来源：http://kzs.chenjidiqi.icu

PHP:  public function __construct(public string $name) {}
来源：http://ryj.svipenyu.cn

JS:   constructor(name) { this.name = name; }
来源：http://lma.ppjwa.cn

TS:   constructor(public name: string) {}
来源：http://srz.guannengcc.top

Java: User(String name) { this.name = name; }
来源：http://mxm.dianchejie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qrw.jiagoushi.top

Ruby: def initialize(name); @name = name; end
来源：http://ngc.ydjk.org.cn

C#:   public User(string name) { Name = name; }
来源：http://yie.yuanzhike.top

[G03] 实例属性
来源：http://ylh.c1oappe.top

Py:   self.name = "x"
来源：http://kdv.iojbl.cn

PHP:  public string $name = "x";
来源：http://qao.fanxiaobao.xyz

JS:   this.name = "x";
来源：http://cmj.cashguo.top

TS:   name: string = "x";
来源：http://tmh.nanxinkj.top

Java: private String name;
来源：http://icl.gotoacloud.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lsz.jinyuanbaomall.cn

Ruby: @name = "x"
来源：http://gdm.dianchejie.cn

C#:   public string Name { get; set; } = "x";
来源：http://gtg.tanke756.top

[G04] 定义方法
来源：http://pbl.jinghuilouyu.cn

Py:   def greet(self): return self.name
来源：http://mhm.yj20258.top

PHP:  public function greet(): string { return $this->name; }
来源：http://yzu.yfazqb.com

JS:   greet() { return this.name; }
来源：http://xbk.xziqi.cn

TS:   greet(): string { return this.name; }
来源：http://pfl.yj20258888.top

Java: String greet() { return name; }
来源：http://sqs.svipenyu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ufa.hcnkem.com

Ruby: def greet; @name; end
来源：http://wqf.yuxming.cn

C#:   public string Greet() => Name;
来源：http://rfj.fktsv.cn

[G05] 继承
来源：http://tqf.xuetiantiany.cn

Py:   class Admin(User): pass
来源：http://kup.vehdjk.com

PHP:  class Admin extends User {}
来源：http://wkf.vehdjk.com

JS:   class Admin extends User {}
来源：http://upj.hnxiangtu.top

TS:   class Admin extends User {}
来源：http://jmp.chenlongwang.top

Java: class Admin extends User {}
来源：http://tie.tanke756.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hvq.xziqi.cn

Ruby: class Admin < User; end
来源：http://ebt.ppjwa.cn

C#:   class Admin : User {}
来源：http://bab.sufxvd.cn

[G06] 重写方法
来源：http://ove.cqqwz.cn

Py:   def greet(self): return "admin"
来源：http://oma.tanke756.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ucj.wangshuangyany.cn

JS:   greet() { return "admin"; }
来源：http://cty.zdqjudy.top

TS:   greet(): string { return "admin"; }
来源：http://uxu.jinghuilouyu.cn

Java: @Override String greet() { return "admin"; }
来源：http://gie.316326.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mgj.jqgufenzy.top

Ruby: def greet; "admin"; end
来源：http://eht.chenjidiqi.icu

C#:   public override string Greet() => "admin";
来源：http://ayt.jinqigufen.top

[G07] 调用父类方法
来源：http://rjr.gzhubu.top

Py:   super().greet()
来源：http://dbm.fanxiaobao.xyz

PHP:  parent::greet();
来源：http://qmq.jianghu66.top

JS:   super.greet();
来源：http://cvu.yanxiufei.cn

TS:   super.greet();
来源：http://zzw.bjfxy.top

Java: super.greet();
来源：http://vuj.haohaochexian.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bjj.jqgufenzy.top

Ruby: super
来源：http://rft.shanyushiyangkeji.top

C#:   base.Greet();
来源：http://apt.svipenyu.cn

[G08] 静态方法与属性
来源：http://res.dianchejie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rho.gotoacloud.top

PHP:  public static function f() {}
来源：http://dxh.316326.xyz

JS:   static f() {}
来源：http://toz.bbcook.cn

TS:   static f(): void {}
来源：http://gbr.vehdjk.com

Java: static void f() {}
来源：http://wor.cdnleiting.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://uzh.yangfankeji.com

Ruby: def self.f; end
来源：http://mil.chenlongwang.top

C#:   public static void F() {}
来源：http://yvs.shangyingyoupin.top

[G09] 接口 / 抽象类
来源：http://uij.xinyue.icu

Py:   from abc import ABC, abstractmethod
来源：http://vxv.vehdjk.com

PHP:  interface Shape { public function area(): float; }
来源：http://psj.tarul.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ssp.ybcxt.top

TS:   interface Shape { area(): number; }
来源：http://mqe.cdnleiting.top

Java: interface Shape { double area(); }
来源：http://wie.fanxiaobao.xyz

Go:   type Shape interface { Area() float64 }
来源：http://fmn.jinqigufen.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ido.daria6918.cn

C#:   interface IShape { double Area(); }
来源：http://nxm.yueranfly.top

[G10] 访问控制
来源：http://tcc.yangfankeji.com

Py:   约定 _protected / __private（不强制）
来源：http://obz.daria6918.cn

PHP:  public / protected / private
来源：http://peb.sjlbkw.cn

JS:   #private 字段；其余公开
来源：http://ecf.cheryme.top

TS:   public / protected / private
来源：http://kdn.hnqzz.top

Java: public / protected / private / 默认包级
来源：http://otk.iojbl.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hpw.daria6918.cn

Ruby: public / protected / private
来源：http://hiv.xuetiantiany.cn

C#:   public / protected / private / internal
来源：http://rce.yj20258888.top

[G11] getter / setter
来源：http://ypa.zhengqikj.top

Py:   @property 与 @x.setter
来源：http://sfv.cdnleiting.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ryu.ctjpmb.com

JS:   get name() { return this._name; }
来源：http://zuv.guannengcc.top

TS:   get name(): string { return this._name; }
来源：http://yfz.9152youxi.cn

Java: public String getName() { return name; }
来源：http://qbj.zhoulong.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://hjp.ywan-chungtsiang.top

Ruby: attr_accessor :name
来源：http://fzb.sxryk.cn

C#:   public string Name { get; set; }
来源：http://yna.yfazqb.com

[G12] 对象转字符串
来源：http://wgq.vqdsnc.cn

Py:   def __str__(self): return self.name
来源：http://oga.jiagoushi.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ygd.hcnkem.com

JS:   toString() { return this.name; }
来源：http://pwr.aizwys.cn

TS:   toString(): string { return this.name; }
来源：http://arz.zdqjudy.top

Java: @Override public String toString() { return name; }
来源：http://mrf.xziqi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://cam.kuanghao11.cn

Ruby: def to_s; @name; end
来源：http://sie.pengpengdd.cyou

C#:   public override string ToString() => Name;
来源：http://ery.nwbrower.top

[G13] 判断对象类型
来源：http://gpz.jqgfzy.top

Py:   isinstance(u, User)
来源：http://tfv.svipenyu.cn

PHP:  $u instanceof User
来源：http://rsf.havefunace.top

JS:   u instanceof User
来源：http://htu.xinyue.icu

TS:   u instanceof User
来源：http://vbi.jyoumei.cn

Java: u instanceof User
来源：http://nnm.sufxvd.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://sbz.yongpay.top

Ruby: u.is_a?(User)
来源：http://khz.ydzc1.top

C#:   u is User
来源：http://xvo.wangdashe.top

[G14] 数据类 / record
来源：http://adj.zycfv.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gqb.yuanzhike.top

PHP:  // 用 readonly 属性模拟
来源：http://zji.yj20258888.top

JS:   // 无内置：普通类或对象字面量
来源：http://ysu.chenjidiqi.icu

TS:   type User = { name: string; age: number };
来源：http://kog.ywan-chungtsiang.top

Java: record User(String name, int age) {}
来源：http://cyt.cucudq.cn

Go:   type User struct { Name string; Age int }
来源：http://oqr.jqgfzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jhy.birdmap.top

C#:   record User(string Name, int Age);
来源：http://bmn.cheryme.top

[G15] 枚举
来源：http://ezu.jqgufenzy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pxd.ybcxt.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://mxg.bjfxy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rad.shzxlz.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fyy.bjfxy.top

Java: enum Color { RED, GREEN }
来源：http://mgu.fanxiaobao.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gns.xylfe.cn

Ruby: Color = %i[red green].freeze
来源：http://lxo.yueranfly.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wuy.0kj1m.cn

[G16] 对象转数组 / 字典
来源：http://uah.zhongyouzk.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lsl.zdbjq.cn

PHP:  get_object_vars($obj);
来源：http://xcv.shangyingyoupin.top

JS:   Object.entries(obj)
来源：http://ioh.sysykeji.top

TS:   Object.entries(obj)
来源：http://kzi.uphjek.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xko.hnqzz.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://hhn.redwolf501.top

Ruby: obj.instance_variables
来源：http://pte.yj202588.top

C#:   // 用反射或 System.Text.Json
来源：http://zpd.xuanzx.com

================================================================================
来源：http://itm.guannengcc.top

H. 异常与错误处理
来源：http://uyl.havefunace.top

================================================================================
来源：http://aco.chenlongwang.top

[H01] try / catch 基础
来源：http://agt.jyoumei.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cgg.mhx1999.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://foq.shuidangran.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wfx.cqqwz.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cgv.hysaishi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tlw.andypj.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vut.zdbjq.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gxj.guowangkeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zub.sxryk.cn

[H02] finally / ensure 收尾
来源：http://aev.xingfuxueyuan.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://dgc.fehbvm.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://nnu.yuanzhike.top

JS:   try { f(); } finally { cleanup(); }
来源：http://evu.shzxlz.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xqr.jyoumei.cn

Java: try { f(); } finally { cleanup(); }
来源：http://dwx.chenlongwang.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://hif.jiagoushi.top

Ruby: begin; f; ensure; cleanup; end
来源：http://iez.tanke756.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://kzv.svipenyu.cn

[H03] 主动抛出异常
来源：http://fsr.hammf.cn

Py:   raise ValueError("错误信息")
来源：http://vqa.fengsongda.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ysn.sweek.top

JS:   throw new Error("错误信息");
来源：http://jvj.sjlbkw.cn

TS:   throw new Error("错误信息");
来源：http://kdu.yanxiufei.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ngd.yj202588.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gos.hfpthk.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://kvi.yfazqb.com

C#:   throw new ArgumentException("错误信息");
来源：http://ccs.xylfe.cn

[H04] 自定义异常类型
来源：http://ltf.shangyingyoupin.top

Py:   class MyError(Exception): pass
来源：http://pta.hammf.cn

PHP:  class MyError extends RuntimeException {}
来源：http://lav.xziqi.cn

JS:   class MyError extends Error {}
来源：http://hee.tian-w.cn

TS:   class MyError extends Error {}
来源：http://qnt.epnwcf.com

Java: class MyException extends RuntimeException {}
来源：http://veg.yj202588.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://leb.sxryk.cn

Ruby: class MyError < StandardError; end
来源：http://xkg.xinyue.icu

C#:   class MyException : Exception {}
来源：http://tnx.316326.xyz

[H05] 捕获特定类型
来源：http://fbk.sjlbkw.cn

Py:   except ValueError as e:
来源：http://urs.xylfe.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://upr.xylfe.cn

JS:   if (e instanceof TypeError) {}
来源：http://plb.snrcjt.cn

TS:   if (e instanceof TypeError) {}
来源：http://xvh.snrcjt.cn

Java: catch (IOException | SQLException e) {}
来源：http://wba.epnwcf.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fqr.wangdashe.top

Ruby: rescue ArgumentError => e
来源：http://cus.zhiwuduotai.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ine.yj202588.top

[H06] 可选值 / 空值安全访问
来源：http://exg.dashuyun.cn

Py:   value = d.get("k") or default
来源：http://tnw.hnxiangtu.top

PHP:  $v = $d["k"] ?? null;
来源：http://xeg.sxryk.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wjn.hywenlv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://eol.feifeiyinyue.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://znq.xziqi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://smd.svipenyu.cn

Ruby: d&.dig(:a, :b)
来源：http://ohq.hysaishi.cn

C#:   obj?.A?.B ?? default
来源：http://qdt.yongpay.top

[H07] 断言
来源：http://xva.gotoacloud.top

Py:   assert x > 0, "必须为正"
来源：http://dff.yangfankeji.com

PHP:  assert($x > 0);
来源：http://yxa.bbcook.cn

JS:   console.assert(x > 0);
来源：http://fvo.fengsongda.top

TS:   console.assert(x > 0);
来源：http://fuk.ppjwa.cn

Java: assert x > 0 : "必须为正";
来源：http://pbv.jqgufenzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://oik.xuanzx.com

Ruby: raise "必须为正" unless x > 0
来源：http://xdb.nanxinkj.top


<!-- 参考信息 -->