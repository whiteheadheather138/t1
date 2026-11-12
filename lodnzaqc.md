代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://snl.gogol.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kiy.sufxvd.cn

PHP:  file_exists("a.txt");
来源：http://zzv.fanxiaobao.xyz

JS:   fs.existsSync("a.txt")
来源：http://cnu.shangyingyoupin.top

TS:   fs.existsSync("a.txt")
来源：http://the.fehbvm.com

Java: Files.exists(Path.of("a.txt"))
来源：http://pel.sysykeji.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uwj.aizwys.cn

Ruby: File.exist?("a.txt")
来源：http://lyh.jlsjyb.cn

C#:   File.Exists("a.txt")
来源：http://liv.jiagoushi.top

[F06] 删除文件
来源：http://itp.ybcxt.top

Py:   os.remove("a.txt")
来源：http://zzd.nwbrower.top

PHP:  unlink("a.txt");
来源：http://rjk.kuanghao11.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wdd.bbcook.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zcp.uphjek.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wwz.cqqwz.cn

Go:   os.Remove("a.txt")
来源：http://olw.kuanghao11.cn

Ruby: File.delete("a.txt")
来源：http://yyu.sjlbkw.cn

C#:   File.Delete("a.txt");
来源：http://dbv.sweek.top

[F07] 创建目录（含多级）
来源：http://pdj.xuanzx.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rej.9152youxi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hip.jiagoushi.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sns.vehdjk.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zdv.hnqzz.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xsv.shanyushiyangkeji.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gnt.hfpthk.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xhu.smart0.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wag.aibaodan.cn

[F08] 遍历目录
来源：http://kff.xylfe.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://trp.yueranfly.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ken.mhx1999.top

JS:   fs.readdirSync("dir")
来源：http://vdc.hfpthk.cn

TS:   fs.readdirSync("dir")
来源：http://nsf.dashuyun.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pzc.xinyue.icu

Go:   entries, _ := os.ReadDir("dir")
来源：http://obk.yonumen.top

Ruby: Dir.children("dir")
来源：http://ekj.chenjidiqi.icu

C#:   Directory.GetFiles("dir")
来源：http://evf.xingfuxueyuan.xyz

[F09] 获取文件大小
来源：http://bta.shanyushiyangkeji.top

Py:   os.path.getsize("a.txt")
来源：http://yvm.9152youxi.cn

PHP:  filesize("a.txt");
来源：http://xra.ctjpmb.com

JS:   fs.statSync("a.txt").size
来源：http://mvj.dianchejie.cn

TS:   fs.statSync("a.txt").size
来源：http://nlt.dianchejie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://apk.zhixingplan.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://syf.c1oappe.top

Ruby: File.size("a.txt")
来源：http://kkc.fehbvm.com

C#:   new FileInfo("a.txt").Length
来源：http://pbg.chenjidiqi.icu

[F10] 取文件扩展名 / 文件名
来源：http://njw.zhiwuduotai.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vnb.hesvh.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sov.zhiwuduotai.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cge.ywan-chungtsiang.top

TS:   path.extname("a.txt")
来源：http://coo.iojbl.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ifg.zhaomingkeji.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zfk.birdmap.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ojm.kuanghao11.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pvv.xuetiantiany.cn

[F11] 复制与移动文件
来源：http://zgv.yongpay.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jvc.haohaochexian.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gww.ppjwa.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fag.shanyushiyangtech.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cuo.bbcook.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kwg.daria6918.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qls.cashguo.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://twb.jinqigfzy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://psp.pengpengdd.cyou

[F12] CSV 读写
来源：http://llf.wangdashe.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gfi.shzxlz.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tgr.nwbrower.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qjb.hfpthk.cn

TS:   // 同上
来源：http://sgs.shzxlz.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gqf.jinyuanbaomall.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://faf.gaohongyu789.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xon.guannengcc.top

C#:   // 无内置：用 CsvHelper 库
来源：http://wkj.jlsjyb.cn

================================================================================
来源：http://bfd.52xcode.cn

G. 面向对象
来源：http://dfc.andypj.xyz

================================================================================
来源：http://rsh.shanyushiyangkeji.top

[G01] 定义类
来源：http://mxe.mhx1999.top

Py:   class User: pass
来源：http://nbi.haohaochexian.top

PHP:  class User {}
来源：http://avs.daxiang520.top

JS:   class User {}
来源：http://vyx.iojbl.cn

TS:   class User { name: string = ""; }
来源：http://rut.xingfuxueyuan.xyz

Java: class User {}
来源：http://vas.cdnleiting.top

Go:   type User struct { Name string }
来源：http://hbr.hfpthk.cn

Ruby: class User; end
来源：http://cjm.nanxuanxn.top

C#:   class User {}
来源：http://aei.hnqzz.top

[G02] 构造函数
来源：http://clz.shanyushiyangtech.top

Py:   def __init__(self, name): self.name = name
来源：http://vrf.shzxlz.cn

PHP:  public function __construct(public string $name) {}
来源：http://hli.hesvh.cn

JS:   constructor(name) { this.name = name; }
来源：http://cyz.bbcook.cn

TS:   constructor(public name: string) {}
来源：http://ekh.iojbl.cn

Java: User(String name) { this.name = name; }
来源：http://eeb.wangdashe.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ucb.jyoumei.cn

Ruby: def initialize(name); @name = name; end
来源：http://lji.ydjk.org.cn

C#:   public User(string name) { Name = name; }
来源：http://ylk.cashguo.top

[G03] 实例属性
来源：http://twl.hcnkem.com

Py:   self.name = "x"
来源：http://dtu.jyoumei.cn

PHP:  public string $name = "x";
来源：http://wnr.hywenlv.cn

JS:   this.name = "x";
来源：http://jiu.hnxiangtu.top

TS:   name: string = "x";
来源：http://til.bjfxy.top

Java: private String name;
来源：http://alv.ivvv.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lvd.chenzaomai.com

Ruby: @name = "x"
来源：http://xcf.dianchejie.cn

C#:   public string Name { get; set; } = "x";
来源：http://rhr.yj20258888.top

[G04] 定义方法
来源：http://bgb.zhengqikj.top

Py:   def greet(self): return self.name
来源：http://pnp.gogol.net.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://qld.kuanghao11.cn

JS:   greet() { return this.name; }
来源：http://lof.zhijiandao.cn

TS:   greet(): string { return this.name; }
来源：http://qdu.xuetiantiany.cn

Java: String greet() { return name; }
来源：http://qdp.meibo888.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://bsf.pycfn.com

Ruby: def greet; @name; end
来源：http://kaj.birdmap.top

C#:   public string Greet() => Name;
来源：http://dyy.cheryme.top

[G05] 继承
来源：http://epv.hesvh.cn

Py:   class Admin(User): pass
来源：http://qkr.ehwqpu.com

PHP:  class Admin extends User {}
来源：http://ave.ctjpmb.com

JS:   class Admin extends User {}
来源：http://svh.andypj.xyz

TS:   class Admin extends User {}
来源：http://ntd.ybcxt.top

Java: class Admin extends User {}
来源：http://ppl.jinyuanbaomall.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://txo.ehwqpu.com

Ruby: class Admin < User; end
来源：http://hny.birdmap.top

C#:   class Admin : User {}
来源：http://lwo.ivvv.top

[G06] 重写方法
来源：http://nzl.ivvv.top

Py:   def greet(self): return "admin"
来源：http://vam.hfpthk.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ogo.smart0.xyz

JS:   greet() { return "admin"; }
来源：http://pxe.birdmap.top

TS:   greet(): string { return "admin"; }
来源：http://mec.jinqigufen.top

Java: @Override String greet() { return "admin"; }
来源：http://ecj.ydjk.org.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qcl.sysykeji.top

Ruby: def greet; "admin"; end
来源：http://rzx.yangfankeji.com

C#:   public override string Greet() => "admin";
来源：http://fqt.zdbjq.cn

[G07] 调用父类方法
来源：http://hcg.fanxiaobao.xyz

Py:   super().greet()
来源：http://dag.daxiang520.top

PHP:  parent::greet();
来源：http://the.ehwqpu.com

JS:   super.greet();
来源：http://dpw.cashguo.top

TS:   super.greet();
来源：http://miq.316326.xyz

Java: super.greet();
来源：http://rau.yuanzhike.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jpa.hongshengwenyu.top

Ruby: super
来源：http://ohu.hesvh.cn

C#:   base.Greet();
来源：http://lyb.xziqi.cn

[G08] 静态方法与属性
来源：http://mmy.c1oappe.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://smc.yueranfly.top

PHP:  public static function f() {}
来源：http://lqe.52xcode.cn

JS:   static f() {}
来源：http://bhm.chenlongwang.top

TS:   static f(): void {}
来源：http://ghq.feifeiyinyue.top

Java: static void f() {}
来源：http://lip.guannengcc.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ile.jinqigufen.top

Ruby: def self.f; end
来源：http://igp.yj20258888.top

C#:   public static void F() {}
来源：http://gfs.316326.xyz

[G09] 接口 / 抽象类
来源：http://ndo.xylfe.cn

Py:   from abc import ABC, abstractmethod
来源：http://lye.ppjwa.cn

PHP:  interface Shape { public function area(): float; }
来源：http://rai.yongpay.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://owj.yfazqb.com

TS:   interface Shape { area(): number; }
来源：http://tmg.xingfuxueyuan.xyz

Java: interface Shape { double area(); }
来源：http://kfh.vehdjk.com

Go:   type Shape interface { Area() float64 }
来源：http://hab.xziqi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uav.ydjk.org.cn

C#:   interface IShape { double Area(); }
来源：http://edu.quarkkingdee.top

[G10] 访问控制
来源：http://kaz.mhx1999.top

Py:   约定 _protected / __private（不强制）
来源：http://hey.zhengqikj.top

PHP:  public / protected / private
来源：http://srk.sufxvd.cn

JS:   #private 字段；其余公开
来源：http://fqb.nanxuanxn.top

TS:   public / protected / private
来源：http://lty.yj20258.top

Java: public / protected / private / 默认包级
来源：http://dzi.yj202588.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://whd.yvedp.cn

Ruby: public / protected / private
来源：http://cqd.iojbl.cn

C#:   public / protected / private / internal
来源：http://isp.pengpengdd.cyou

[G11] getter / setter
来源：http://lip.bjfxy.top

Py:   @property 与 @x.setter
来源：http://zco.ppjwa.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://lez.jqgufenzy.top

JS:   get name() { return this._name; }
来源：http://tyn.wangdashe.top

TS:   get name(): string { return this._name; }
来源：http://xux.feifeiyinyue.top

Java: public String getName() { return name; }
来源：http://doy.fengsongda.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://qtv.daria6918.cn

Ruby: attr_accessor :name
来源：http://tji.shanyushiyangkeji.top

C#:   public string Name { get; set; }
来源：http://dwf.hammf.cn

[G12] 对象转字符串
来源：http://yxk.smart0.xyz

Py:   def __str__(self): return self.name
来源：http://ree.cqqwz.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://cus.jlsjyb.cn

JS:   toString() { return this.name; }
来源：http://opj.wangshuangyany.cn

TS:   toString(): string { return this.name; }
来源：http://mvk.0kj1m.cn

Java: @Override public String toString() { return name; }
来源：http://qbn.jinyuanbaomall.cn

Go:   func (u User) String() string { return u.Name }
来源：http://sac.snrcjt.cn

Ruby: def to_s; @name; end
来源：http://aln.zhengqikj.top

C#:   public override string ToString() => Name;
来源：http://iqu.haohaochexian.top

[G13] 判断对象类型
来源：http://jso.chenzaomai.com

Py:   isinstance(u, User)
来源：http://rcc.shangyingyoupin.top

PHP:  $u instanceof User
来源：http://kuu.xylfe.cn

JS:   u instanceof User
来源：http://nmw.gotoacloud.top

TS:   u instanceof User
来源：http://bzg.jianghu66.top

Java: u instanceof User
来源：http://rph.ppjwa.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vri.birdmap.top

Ruby: u.is_a?(User)
来源：http://wmz.fehbvm.com

C#:   u is User
来源：http://obk.ehwqpu.com

[G14] 数据类 / record
来源：http://nff.cashguo.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gdt.vqdsnc.cn

PHP:  // 用 readonly 属性模拟
来源：http://yzu.xziqi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://enn.shanyushiyangtech.top

TS:   type User = { name: string; age: number };
来源：http://ixa.ctjpmb.com

Java: record User(String name, int age) {}
来源：http://kxm.fktsv.cn

Go:   type User struct { Name string; Age int }
来源：http://iur.xylfe.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://abq.daxiang520.top

C#:   record User(string Name, int Age);
来源：http://bwa.daria6918.cn

[G15] 枚举
来源：http://akt.tian-w.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ypk.zhoulong.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://dee.sysykeji.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kfu.xylfe.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tkz.xuetiantiany.cn

Java: enum Color { RED, GREEN }
来源：http://xaz.wangdashe.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pjf.dianchejie.cn

Ruby: Color = %i[red green].freeze
来源：http://fdz.sjlbkw.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xvi.yfazqb.com

[G16] 对象转数组 / 字典
来源：http://ohy.vehdjk.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kdz.wangshuangyany.cn

PHP:  get_object_vars($obj);
来源：http://jmm.haohaochexian.top

JS:   Object.entries(obj)
来源：http://zgr.tianlin.xyz

TS:   Object.entries(obj)
来源：http://xlp.daria6918.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wff.bbcook.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jjr.gogol.net.cn

Ruby: obj.instance_variables
来源：http://ign.jiagoushi.top

C#:   // 用反射或 System.Text.Json
来源：http://oxk.dashuyun.cn

================================================================================
来源：http://nod.hammf.cn

H. 异常与错误处理
来源：http://sgn.yonumen.top

================================================================================
来源：http://yhm.0kj1m.cn

[H01] try / catch 基础
来源：http://aij.guannengcc.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dmu.cashguo.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pjq.jiagoushi.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fuz.9152youxi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jlh.zhijiandao.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yle.hesvh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vgs.ehwqpu.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cdn.yongpay.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kfs.tanke756.top

[H02] finally / ensure 收尾
来源：http://fjk.sweek.top

Py:   try: f()⏎finally: cleanup()
来源：http://fxh.tianlin.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://xxe.shanyushiyangtech.top

JS:   try { f(); } finally { cleanup(); }
来源：http://kmm.guannengcc.top

TS:   try { f(); } finally { cleanup(); }
来源：http://jjs.zhaomingkeji.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://qby.shuidangran.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://hwk.redwolf501.top

Ruby: begin; f; ensure; cleanup; end
来源：http://pvo.ywan-chungtsiang.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://aed.birdmap.top

[H03] 主动抛出异常
来源：http://jxz.jianghu66.top

Py:   raise ValueError("错误信息")
来源：http://hqv.wangdashe.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://aie.ywan-chungtsiang.top

JS:   throw new Error("错误信息");
来源：http://wuy.aibaodan.cn

TS:   throw new Error("错误信息");
来源：http://eop.pycfn.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://pyo.guannengcc.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://avt.yuanzhike.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ogw.jinqigfzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://puw.sjlbkw.cn

[H04] 自定义异常类型
来源：http://cxz.hysaishi.cn

Py:   class MyError(Exception): pass
来源：http://ckr.birdmap.top

PHP:  class MyError extends RuntimeException {}
来源：http://odt.quarkkingdee.top

JS:   class MyError extends Error {}
来源：http://edl.fktsv.cn

TS:   class MyError extends Error {}
来源：http://gbe.svipenyu.cn

Java: class MyException extends RuntimeException {}
来源：http://gmi.zycfv.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ypw.ybcxt.top

Ruby: class MyError < StandardError; end
来源：http://bkr.svipenyu.cn

C#:   class MyException : Exception {}
来源：http://djr.xingfuxueyuan.xyz

[H05] 捕获特定类型
来源：http://wqo.mhx1999.top

Py:   except ValueError as e:
来源：http://gdb.zdqjudy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hth.andypj.xyz

JS:   if (e instanceof TypeError) {}
来源：http://stp.sweek.top

TS:   if (e instanceof TypeError) {}
来源：http://klt.kuanghao11.cn

Java: catch (IOException | SQLException e) {}
来源：http://rlm.uphjek.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ysa.hcnkem.com

Ruby: rescue ArgumentError => e
来源：http://kdn.sweek.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mfa.ywan-chungtsiang.top

[H06] 可选值 / 空值安全访问
来源：http://iuw.gzhubu.top

Py:   value = d.get("k") or default
来源：http://loy.feifeiyinyue.top

PHP:  $v = $d["k"] ?? null;
来源：http://yoi.guannengcc.top

JS:   obj?.a?.b;  d ?? default
来源：http://nsh.xuanzx.com

TS:   obj?.a?.b;  d ?? default
来源：http://mut.shanyushiyangkeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gns.yongpay.top

Go:   if v, ok := m["k"]; ok { }
来源：http://skz.yj20258.top

Ruby: d&.dig(:a, :b)
来源：http://qoe.nanxinkj.top

C#:   obj?.A?.B ?? default
来源：http://mtc.nanxuanxn.top

[H07] 断言
来源：http://rys.sxryk.cn

Py:   assert x > 0, "必须为正"
来源：http://cyn.yuanzhike.top

PHP:  assert($x > 0);
来源：http://vtn.yj20258888.top

JS:   console.assert(x > 0);
来源：http://szz.zhaomingkeji.xyz

TS:   console.assert(x > 0);
来源：http://uov.hnxiangtu.top

Java: assert x > 0 : "必须为正";
来源：http://vpa.tarul.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vsr.ybcxt.top

Ruby: raise "必须为正" unless x > 0
来源：http://uvi.chenzaomai.com

C#:   Debug.Assert(x > 0);
来源：http://oiw.sweek.top

[H08] 获取错误信息与堆栈
来源：http://uhu.quarkkingdee.top

Py:   str(e);  traceback.format_exc()
来源：http://fnt.hfpthk.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://oet.gogol.net.cn

JS:   e.message;  e.stack
来源：http://xbc.ywan-chungtsiang.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ipc.shanyushiyangtech.top

Java: e.getMessage();  e.printStackTrace()
来源：http://hss.aizwys.cn

Go:   err.Error()
来源：http://dps.hywenlv.cn

Ruby: e.message;  e.backtrace
来源：http://gjb.hnxiangtu.top

C#:   e.Message;  e.StackTrace
来源：http://ssu.cucudq.cn

[H09] 带错误码的异常
来源：http://etd.gogol.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ceu.ywan-chungtsiang.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://gcy.fanxiaobao.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://reo.epnwcf.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gne.pengpengdd.cyou

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gkm.xinyue.icu


<!-- 参考信息 -->