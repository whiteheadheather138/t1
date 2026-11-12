代发 wailian999

C#:   File.Exists("a.txt")
来源：http://okf.hammf.cn

[F06] 删除文件
来源：http://sdq.uphjek.com

Py:   os.remove("a.txt")
来源：http://vze.yongpay.top

PHP:  unlink("a.txt");
来源：http://uqe.gzhubu.top

JS:   fs.unlinkSync("a.txt")
来源：http://jdb.jinqigfzy.top

TS:   fs.unlinkSync("a.txt")
来源：http://ocv.cheryme.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yzd.xingfuxueyuan.xyz

Go:   os.Remove("a.txt")
来源：http://fyf.wangshuangyany.cn

Ruby: File.delete("a.txt")
来源：http://vsf.tian-w.cn

C#:   File.Delete("a.txt");
来源：http://zih.sxryk.cn

[F07] 创建目录（含多级）
来源：http://hmi.fzhhl.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://trd.yangfankeji.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ipv.fzhhl.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://twc.guowangkeji.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tzx.xingfuxueyuan.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jrr.ywan-chungtsiang.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hzy.xuanzx.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qpk.havefunace.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://spi.zhixingplan.top

[F08] 遍历目录
来源：http://wpy.shanyushiyangtech.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://fmo.vqdsnc.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://clx.chenzaomai.com

JS:   fs.readdirSync("dir")
来源：http://qun.cdnleiting.top

TS:   fs.readdirSync("dir")
来源：http://sir.xuetiantiany.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tub.zdbjq.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://nid.daria6918.cn

Ruby: Dir.children("dir")
来源：http://pwo.zhiwuduotai.top

C#:   Directory.GetFiles("dir")
来源：http://yla.shanyushiyangtech.top

[F09] 获取文件大小
来源：http://tox.redwolf501.top

Py:   os.path.getsize("a.txt")
来源：http://qzl.hnqzz.top

PHP:  filesize("a.txt");
来源：http://qjw.daria6918.cn

JS:   fs.statSync("a.txt").size
来源：http://wqc.ywan-chungtsiang.top

TS:   fs.statSync("a.txt").size
来源：http://vkd.hywenlv.cn

Java: Files.size(Path.of("a.txt"))
来源：http://yqe.andypj.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://acv.yj20258888.top

Ruby: File.size("a.txt")
来源：http://sqs.316326.xyz

C#:   new FileInfo("a.txt").Length
来源：http://cfs.yanxiufei.cn

[F10] 取文件扩展名 / 文件名
来源：http://nzf.c1oappe.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jch.sufxvd.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://taw.daxiang520.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://inu.yuxming.cn

TS:   path.extname("a.txt")
来源：http://hwq.fengsongda.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://chx.hammf.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fay.zhoulong.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cbn.fanxiaobao.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://teg.jqgufenzy.top

[F11] 复制与移动文件
来源：http://eyz.mhx1999.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xqx.bbcook.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://oyn.andypj.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ctj.dashuyun.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://axg.fengsongda.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jku.fehbvm.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jrd.0kj1m.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wcs.jinyuanbaomall.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://osv.jinyuanbaomall.cn

[F12] CSV 读写
来源：http://jqt.ppjwa.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vay.yongpay.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pem.fanxiaobao.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gkt.tianlin.xyz

TS:   // 同上
来源：http://bgm.pycfn.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xnj.fanxiaobao.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ikm.ybcxt.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kcv.fktsv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://dmw.dashuyun.cn

================================================================================
来源：http://pgg.yangfankeji.com

G. 面向对象
来源：http://ztf.fehbvm.com

================================================================================
来源：http://kyq.ydjk.org.cn

[G01] 定义类
来源：http://kky.aibaodan.cn

Py:   class User: pass
来源：http://bqi.zhongyouzk.top

PHP:  class User {}
来源：http://wwr.ydjk.org.cn

JS:   class User {}
来源：http://noo.ydjk.org.cn

TS:   class User { name: string = ""; }
来源：http://aif.gzhubu.top

Java: class User {}
来源：http://gyn.jlsjyb.cn

Go:   type User struct { Name string }
来源：http://yoh.yuanzhike.top

Ruby: class User; end
来源：http://tsw.ivvv.top

C#:   class User {}
来源：http://xwl.epnwcf.com

[G02] 构造函数
来源：http://twn.smart0.xyz

Py:   def __init__(self, name): self.name = name
来源：http://zug.yj20258.top

PHP:  public function __construct(public string $name) {}
来源：http://ybo.cashguo.top

JS:   constructor(name) { this.name = name; }
来源：http://kob.fktsv.cn

TS:   constructor(public name: string) {}
来源：http://rvo.sweek.top

Java: User(String name) { this.name = name; }
来源：http://fnv.zhaomingkeji.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nhg.haohaochexian.top

Ruby: def initialize(name); @name = name; end
来源：http://hbq.ivvv.top

C#:   public User(string name) { Name = name; }
来源：http://wve.uphjek.com

[G03] 实例属性
来源：http://kvc.meibo888.top

Py:   self.name = "x"
来源：http://kpf.vqdsnc.cn

PHP:  public string $name = "x";
来源：http://aoc.nanxuanxn.top

JS:   this.name = "x";
来源：http://ojo.yj20258888.top

TS:   name: string = "x";
来源：http://pen.nwbrower.top

Java: private String name;
来源：http://pov.cqqwz.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wis.pycfn.com

Ruby: @name = "x"
来源：http://pka.zhijiandao.cn

C#:   public string Name { get; set; } = "x";
来源：http://czh.sysykeji.top

[G04] 定义方法
来源：http://ram.fanxiaobao.xyz

Py:   def greet(self): return self.name
来源：http://mzu.hongshengwenyu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://kdd.jqgufenzy.top

JS:   greet() { return this.name; }
来源：http://erz.yj202588.top

TS:   greet(): string { return this.name; }
来源：http://lwv.c1oappe.top

Java: String greet() { return name; }
来源：http://vbu.zhijiandao.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://cif.hongshengwenyu.top

Ruby: def greet; @name; end
来源：http://kfq.ehwqpu.com

C#:   public string Greet() => Name;
来源：http://qqr.epnwcf.com

[G05] 继承
来源：http://hdf.dianchejie.cn

Py:   class Admin(User): pass
来源：http://gca.redwolf501.top

PHP:  class Admin extends User {}
来源：http://zav.zdqjudy.top

JS:   class Admin extends User {}
来源：http://bvc.pengpengdd.cyou

TS:   class Admin extends User {}
来源：http://gaw.vqdsnc.cn

Java: class Admin extends User {}
来源：http://vey.aibaodan.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uyp.hongshengwenyu.top

Ruby: class Admin < User; end
来源：http://poe.fehbvm.com

C#:   class Admin : User {}
来源：http://ofl.hcnkem.com

[G06] 重写方法
来源：http://kxi.yanxiufei.cn

Py:   def greet(self): return "admin"
来源：http://nkk.zhixingplan.top

PHP:  public function greet(): string { return "admin"; }
来源：http://spl.0kj1m.cn

JS:   greet() { return "admin"; }
来源：http://jik.gogol.net.cn

TS:   greet(): string { return "admin"; }
来源：http://mzm.xuetiantiany.cn

Java: @Override String greet() { return "admin"; }
来源：http://cvb.hnxiangtu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bxz.dashuyun.cn

Ruby: def greet; "admin"; end
来源：http://eyh.fanxiaobao.xyz

C#:   public override string Greet() => "admin";
来源：http://pea.vqdsnc.cn

[G07] 调用父类方法
来源：http://pxs.shzxlz.cn

Py:   super().greet()
来源：http://edz.zhaomingkeji.xyz

PHP:  parent::greet();
来源：http://cak.fzhhl.top

JS:   super.greet();
来源：http://gul.ydzc1.top

TS:   super.greet();
来源：http://qjy.wangshuangyany.cn

Java: super.greet();
来源：http://oll.yj202588.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cns.dashuyun.cn

Ruby: super
来源：http://jvu.uphjek.com

C#:   base.Greet();
来源：http://euq.jinyuanbaomall.cn

[G08] 静态方法与属性
来源：http://xvf.redwolf501.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zdc.chenjidiqi.icu

PHP:  public static function f() {}
来源：http://xfd.jinyuanbaomall.cn

JS:   static f() {}
来源：http://qsm.snrcjt.cn

TS:   static f(): void {}
来源：http://ita.pengpengdd.cyou

Java: static void f() {}
来源：http://pxm.feifeiyinyue.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://emm.jqgfzy.top

Ruby: def self.f; end
来源：http://xyb.wangdashe.top

C#:   public static void F() {}
来源：http://njq.jqgufenzy.top

[G09] 接口 / 抽象类
来源：http://snu.nanxinkj.top

Py:   from abc import ABC, abstractmethod
来源：http://iei.sjlbkw.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dxx.uphjek.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://ojq.52xcode.cn

TS:   interface Shape { area(): number; }
来源：http://bvd.jinqigfzy.top

Java: interface Shape { double area(); }
来源：http://nlx.meibo888.top

Go:   type Shape interface { Area() float64 }
来源：http://uqj.aizwys.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://akt.yfazqb.com

C#:   interface IShape { double Area(); }
来源：http://szd.andypj.xyz

[G10] 访问控制
来源：http://hvm.52xcode.cn

Py:   约定 _protected / __private（不强制）
来源：http://nae.xingfuxueyuan.xyz

PHP:  public / protected / private
来源：http://qof.cashguo.top

JS:   #private 字段；其余公开
来源：http://vay.zhongyouzk.top

TS:   public / protected / private
来源：http://obw.fehbvm.com

Java: public / protected / private / 默认包级
来源：http://zsb.hnxiangtu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ely.nwbrower.top

Ruby: public / protected / private
来源：http://ung.tianlin.xyz

C#:   public / protected / private / internal
来源：http://tnh.aibaodan.cn

[G11] getter / setter
来源：http://ugu.daria6918.cn

Py:   @property 与 @x.setter
来源：http://xks.ywan-chungtsiang.top

PHP:  public function getName(): string { return $this->name; }
来源：http://pvh.bbcook.cn

JS:   get name() { return this._name; }
来源：http://abx.gzhubu.top

TS:   get name(): string { return this._name; }
来源：http://etb.wangshuangyany.cn

Java: public String getName() { return name; }
来源：http://lrl.pycfn.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://qiy.snrcjt.cn

Ruby: attr_accessor :name
来源：http://kwq.ydzc1.top

C#:   public string Name { get; set; }
来源：http://txs.xuetiantiany.cn

[G12] 对象转字符串
来源：http://acx.c1oappe.top

Py:   def __str__(self): return self.name
来源：http://dcm.guowangkeji.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ezp.mhx1999.top

JS:   toString() { return this.name; }
来源：http://jxa.dianchejie.cn

TS:   toString(): string { return this.name; }
来源：http://tzu.tarul.cn

Java: @Override public String toString() { return name; }
来源：http://qcr.nanxuanxn.top

Go:   func (u User) String() string { return u.Name }
来源：http://uni.ppjwa.cn

Ruby: def to_s; @name; end
来源：http://vaw.jianghu66.top

C#:   public override string ToString() => Name;
来源：http://vvm.cqqwz.cn

[G13] 判断对象类型
来源：http://pvr.zdbjq.cn

Py:   isinstance(u, User)
来源：http://azi.havefunace.top

PHP:  $u instanceof User
来源：http://ybp.gogol.net.cn

JS:   u instanceof User
来源：http://vxo.yfazqb.com

TS:   u instanceof User
来源：http://nyd.dashuyun.cn

Java: u instanceof User
来源：http://fjj.9152youxi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vlt.gaohongyu789.top

Ruby: u.is_a?(User)
来源：http://zos.guannengcc.top

C#:   u is User
来源：http://mul.nanxinkj.top

[G14] 数据类 / record
来源：http://cmm.zhengqikj.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xwy.quarkkingdee.top

PHP:  // 用 readonly 属性模拟
来源：http://snd.dashuyun.cn

JS:   // 无内置：普通类或对象字面量
来源：http://amu.gaohongyu789.top

TS:   type User = { name: string; age: number };
来源：http://pnc.smart0.xyz

Java: record User(String name, int age) {}
来源：http://cxg.316326.xyz

Go:   type User struct { Name string; Age int }
来源：http://huz.zhiwuduotai.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dzg.jinqigfzy.top

C#:   record User(string Name, int Age);
来源：http://ykj.gotoacloud.top

[G15] 枚举
来源：http://trl.jqgfzy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://eym.jinyuanbaomall.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hbg.jinghuilouyu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dtx.gaohongyu789.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://urq.jinyuanbaomall.cn

Java: enum Color { RED, GREEN }
来源：http://iqa.haohaochexian.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://eij.meibo888.top

Ruby: Color = %i[red green].freeze
来源：http://qis.fzhhl.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bll.ivvv.top

[G16] 对象转数组 / 字典
来源：http://cii.jyoumei.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kez.zdbjq.cn

PHP:  get_object_vars($obj);
来源：http://uoo.nwbrower.top

JS:   Object.entries(obj)
来源：http://bsm.andypj.xyz

TS:   Object.entries(obj)
来源：http://mqd.smart0.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ykz.fengsongda.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://psf.nwbrower.top

Ruby: obj.instance_variables
来源：http://mra.chenjidiqi.icu

C#:   // 用反射或 System.Text.Json
来源：http://idr.dashuyun.cn

================================================================================
来源：http://euw.jinqigufen.top

H. 异常与错误处理
来源：http://ylk.yanxiufei.cn

================================================================================
来源：http://ktm.daria6918.cn

[H01] try / catch 基础
来源：http://mng.cqqwz.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ven.feifeiyinyue.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cqa.xuetiantiany.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://eup.9152youxi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fzk.hcnkem.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ysh.chenzaomai.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ulz.hnqzz.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tfh.hywenlv.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gku.zhoulong.xyz

[H02] finally / ensure 收尾
来源：http://rgj.zycfv.cn

Py:   try: f()⏎finally: cleanup()
来源：http://umb.zhengqikj.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://hye.tian-w.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://nox.jianghu66.top

TS:   try { f(); } finally { cleanup(); }
来源：http://cim.jqgfzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://mgx.jinqigfzy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://oxz.xziqi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://zmc.gaohongyu789.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://jqz.iojbl.cn

[H03] 主动抛出异常
来源：http://brj.bbcook.cn

Py:   raise ValueError("错误信息")
来源：http://lka.ydzc1.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bfx.uphjek.com

JS:   throw new Error("错误信息");
来源：http://zmh.xziqi.cn

TS:   throw new Error("错误信息");
来源：http://hby.yj202588.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://pxh.cucudq.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rbg.svipenyu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://gdu.yangfankeji.com

C#:   throw new ArgumentException("错误信息");
来源：http://onk.redwolf501.top

[H04] 自定义异常类型
来源：http://ezb.yj20258888.top

Py:   class MyError(Exception): pass
来源：http://oln.tanke756.top

PHP:  class MyError extends RuntimeException {}
来源：http://fnd.guannengcc.top

JS:   class MyError extends Error {}
来源：http://cky.gogol.net.cn

TS:   class MyError extends Error {}
来源：http://plj.fehbvm.com

Java: class MyException extends RuntimeException {}
来源：http://yzy.shzxlz.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gtf.ydjk.org.cn

Ruby: class MyError < StandardError; end
来源：http://ptn.yanxiufei.cn

C#:   class MyException : Exception {}
来源：http://aws.yj20258.top

[H05] 捕获特定类型
来源：http://vhl.yanxiufei.cn

Py:   except ValueError as e:
来源：http://pix.zhengqikj.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sen.yfazqb.com

JS:   if (e instanceof TypeError) {}
来源：http://ntv.aizwys.cn

TS:   if (e instanceof TypeError) {}
来源：http://pgv.zhixingplan.top

Java: catch (IOException | SQLException e) {}
来源：http://jch.dianchejie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xtj.sweek.top

Ruby: rescue ArgumentError => e
来源：http://seb.gaohongyu789.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kbj.yueranfly.top

[H06] 可选值 / 空值安全访问
来源：http://gau.ybcxt.top

Py:   value = d.get("k") or default
来源：http://xvw.gaohongyu789.top

PHP:  $v = $d["k"] ?? null;
来源：http://rfk.redwolf501.top

JS:   obj?.a?.b;  d ?? default
来源：http://dhk.fehbvm.com

TS:   obj?.a?.b;  d ?? default
来源：http://ldc.sweek.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hrr.yj20258888.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ifn.shanyushiyangtech.top

Ruby: d&.dig(:a, :b)
来源：http://poc.shangyingyoupin.top

C#:   obj?.A?.B ?? default
来源：http://bwi.zhaomingkeji.xyz

[H07] 断言
来源：http://jej.aizwys.cn

Py:   assert x > 0, "必须为正"
来源：http://heu.sysykeji.top

PHP:  assert($x > 0);
来源：http://zru.sxryk.cn

JS:   console.assert(x > 0);
来源：http://wez.zhongyouzk.top

TS:   console.assert(x > 0);
来源：http://jpt.fehbvm.com

Java: assert x > 0 : "必须为正";
来源：http://zan.xylfe.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yna.ybcxt.top

Ruby: raise "必须为正" unless x > 0
来源：http://zwz.nanxinkj.top

C#:   Debug.Assert(x > 0);
来源：http://jhn.jianghu66.top

[H08] 获取错误信息与堆栈
来源：http://xxd.nwbrower.top

Py:   str(e);  traceback.format_exc()
来源：http://mki.ctjpmb.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://moq.zdbjq.cn

JS:   e.message;  e.stack
来源：http://xhp.jinyuanbaomall.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xrz.meibo888.top

Java: e.getMessage();  e.printStackTrace()
来源：http://zzw.bbcook.cn

Go:   err.Error()
来源：http://vll.yonumen.top

Ruby: e.message;  e.backtrace
来源：http://ufw.yuxming.cn

C#:   e.Message;  e.StackTrace
来源：http://vcp.yueranfly.top

[H09] 带错误码的异常
来源：http://ulg.gaohongyu789.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zqs.xingfuxueyuan.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://dvb.hfpthk.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nmd.haohaochexian.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://snv.52xcode.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xbr.nanxuanxn.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hrk.mhx1999.top

Ruby: raise MyError.new("fail", 500)
来源：http://opb.shuidangran.top

C#:   // 自定义异常类中加 Code 属性
来源：http://bts.hammf.cn

[H10] 资源自动释放
来源：http://vfm.xziqi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://hmu.fehbvm.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ljn.epnwcf.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://twd.nwbrower.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hxt.hfpthk.cn


<!-- 参考信息 -->