代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://sjd.jinqigufen.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ebn.jlsjyb.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tvp.havefunace.top

Ruby: File.exist?("a.txt")
来源：http://hyv.yuxming.cn

C#:   File.Exists("a.txt")
来源：http://pvk.dashuyun.cn

[F06] 删除文件
来源：http://cbs.meibo888.top

Py:   os.remove("a.txt")
来源：http://elk.bbcook.cn

PHP:  unlink("a.txt");
来源：http://eki.ydzc1.top

JS:   fs.unlinkSync("a.txt")
来源：http://qpi.xuanzx.com

TS:   fs.unlinkSync("a.txt")
来源：http://bsw.chenzaomai.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://npd.tarul.cn

Go:   os.Remove("a.txt")
来源：http://orl.zhixingplan.top

Ruby: File.delete("a.txt")
来源：http://med.316326.xyz

C#:   File.Delete("a.txt");
来源：http://cvk.chenjidiqi.icu

[F07] 创建目录（含多级）
来源：http://rzg.yonumen.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dxw.wangshuangyany.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ved.fktsv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lge.jinqigfzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mib.yonumen.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://grd.hnqzz.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qln.hammf.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sun.316326.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://atz.quarkkingdee.top

[F08] 遍历目录
来源：http://lkc.chenlongwang.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://xfd.jinqigfzy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://icd.kuanghao11.cn

JS:   fs.readdirSync("dir")
来源：http://jcp.ydzc1.top

TS:   fs.readdirSync("dir")
来源：http://bpp.nanxuanxn.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gah.hammf.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ygg.jiagoushi.top

Ruby: Dir.children("dir")
来源：http://byd.xuanzx.com

C#:   Directory.GetFiles("dir")
来源：http://njd.bjfxy.top

[F09] 获取文件大小
来源：http://avd.guowangkeji.top

Py:   os.path.getsize("a.txt")
来源：http://jwt.hnxiangtu.top

PHP:  filesize("a.txt");
来源：http://geh.aibaodan.cn

JS:   fs.statSync("a.txt").size
来源：http://wul.hesvh.cn

TS:   fs.statSync("a.txt").size
来源：http://rzg.jqgfzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://jzy.shuidangran.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lmn.zhaomingkeji.xyz

Ruby: File.size("a.txt")
来源：http://piy.yj202588.top

C#:   new FileInfo("a.txt").Length
来源：http://rjl.hammf.cn

[F10] 取文件扩展名 / 文件名
来源：http://ayr.aizwys.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://upk.zhengqikj.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zwr.ydjk.org.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://edr.tian-w.cn

TS:   path.extname("a.txt")
来源：http://exz.andypj.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nqx.zhijiandao.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jxl.guannengcc.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ygc.yj202588.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gws.jiagoushi.top

[F11] 复制与移动文件
来源：http://tsb.snrcjt.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sij.shangyingyoupin.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hof.xylfe.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xtx.xinyue.icu

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jhr.smart0.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://acz.vqdsnc.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pdm.hesvh.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://axf.zhengqikj.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pcz.zhixingplan.top

[F12] CSV 读写
来源：http://dfj.ybcxt.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://asn.chenzaomai.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qam.xylfe.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hww.cashguo.top

TS:   // 同上
来源：http://viu.jyoumei.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://efb.guannengcc.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wdp.quarkkingdee.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://poq.aizwys.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://fme.yj20258888.top

================================================================================
来源：http://eel.yfazqb.com

G. 面向对象
来源：http://xum.mhx1999.top

================================================================================
来源：http://gyg.guowangkeji.top

[G01] 定义类
来源：http://dzd.fengsongda.top

Py:   class User: pass
来源：http://fbi.mhx1999.top

PHP:  class User {}
来源：http://qfj.ppjwa.cn

JS:   class User {}
来源：http://fjt.yonumen.top

TS:   class User { name: string = ""; }
来源：http://fda.epnwcf.com

Java: class User {}
来源：http://bok.meibo888.top

Go:   type User struct { Name string }
来源：http://awm.guowangkeji.top

Ruby: class User; end
来源：http://qdx.ehwqpu.com

C#:   class User {}
来源：http://cgu.shzxlz.cn

[G02] 构造函数
来源：http://eox.meibo888.top

Py:   def __init__(self, name): self.name = name
来源：http://ici.zdbjq.cn

PHP:  public function __construct(public string $name) {}
来源：http://coj.jyoumei.cn

JS:   constructor(name) { this.name = name; }
来源：http://yxc.hongshengwenyu.top

TS:   constructor(public name: string) {}
来源：http://xki.jinghuilouyu.cn

Java: User(String name) { this.name = name; }
来源：http://lwd.yanxiufei.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gtv.jiagoushi.top

Ruby: def initialize(name); @name = name; end
来源：http://etn.aibaodan.cn

C#:   public User(string name) { Name = name; }
来源：http://xqz.iojbl.cn

[G03] 实例属性
来源：http://mtd.dianchejie.cn

Py:   self.name = "x"
来源：http://bsl.yj20258.top

PHP:  public string $name = "x";
来源：http://aeu.xuetiantiany.cn

JS:   this.name = "x";
来源：http://dwq.hysaishi.cn

TS:   name: string = "x";
来源：http://bax.yfazqb.com

Java: private String name;
来源：http://yid.c1oappe.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sdu.hongshengwenyu.top

Ruby: @name = "x"
来源：http://kwp.quarkkingdee.top

C#:   public string Name { get; set; } = "x";
来源：http://gox.yj202588.top

[G04] 定义方法
来源：http://osc.hysaishi.cn

Py:   def greet(self): return self.name
来源：http://dkm.wangdashe.top

PHP:  public function greet(): string { return $this->name; }
来源：http://gal.kuanghao11.cn

JS:   greet() { return this.name; }
来源：http://nms.ctjpmb.com

TS:   greet(): string { return this.name; }
来源：http://vlk.cheryme.top

Java: String greet() { return name; }
来源：http://fqe.jiagoushi.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://xdk.mhx1999.top

Ruby: def greet; @name; end
来源：http://tjj.wangdashe.top

C#:   public string Greet() => Name;
来源：http://kfs.uphjek.com

[G05] 继承
来源：http://dur.kuanghao11.cn

Py:   class Admin(User): pass
来源：http://exz.jyoumei.cn

PHP:  class Admin extends User {}
来源：http://eoi.tarul.cn

JS:   class Admin extends User {}
来源：http://ykq.nwbrower.top

TS:   class Admin extends User {}
来源：http://stj.tarul.cn

Java: class Admin extends User {}
来源：http://azg.wangdashe.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://clc.zhixingplan.top

Ruby: class Admin < User; end
来源：http://dln.daxiang520.top

C#:   class Admin : User {}
来源：http://xbg.shangyingyoupin.top

[G06] 重写方法
来源：http://dmt.fehbvm.com

Py:   def greet(self): return "admin"
来源：http://ngj.316326.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://vfq.yuxming.cn

JS:   greet() { return "admin"; }
来源：http://tdj.yueranfly.top

TS:   greet(): string { return "admin"; }
来源：http://cpi.gzhubu.top

Java: @Override String greet() { return "admin"; }
来源：http://jlw.ybcxt.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vqe.hcnkem.com

Ruby: def greet; "admin"; end
来源：http://otf.feifeiyinyue.top

C#:   public override string Greet() => "admin";
来源：http://xgm.jqgfzy.top

[G07] 调用父类方法
来源：http://daq.feifeiyinyue.top

Py:   super().greet()
来源：http://gvn.chenjidiqi.icu

PHP:  parent::greet();
来源：http://fgw.pycfn.com

JS:   super.greet();
来源：http://dzj.gaohongyu789.top

TS:   super.greet();
来源：http://jrm.pengpengdd.cyou

Java: super.greet();
来源：http://yht.xylfe.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nyl.shzxlz.cn

Ruby: super
来源：http://fjs.zhiwuduotai.top

C#:   base.Greet();
来源：http://shc.redwolf501.top

[G08] 静态方法与属性
来源：http://crp.fengsongda.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wex.yvedp.cn

PHP:  public static function f() {}
来源：http://fgb.zdqjudy.top

JS:   static f() {}
来源：http://jae.sweek.top

TS:   static f(): void {}
来源：http://vuz.sysykeji.top

Java: static void f() {}
来源：http://gyw.pengpengdd.cyou

Go:   // 无 static：用包级函数，按包名调用
来源：http://pih.birdmap.top

Ruby: def self.f; end
来源：http://vuq.andypj.xyz

C#:   public static void F() {}
来源：http://okc.hnqzz.top

[G09] 接口 / 抽象类
来源：http://dnb.tianlin.xyz

Py:   from abc import ABC, abstractmethod
来源：http://bmm.fanxiaobao.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://aqi.vehdjk.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://rsq.hesvh.cn

TS:   interface Shape { area(): number; }
来源：http://ghw.aizwys.cn

Java: interface Shape { double area(); }
来源：http://qid.tanke756.top

Go:   type Shape interface { Area() float64 }
来源：http://jxp.ppjwa.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hfd.yj20258.top

C#:   interface IShape { double Area(); }
来源：http://pxl.uphjek.com

[G10] 访问控制
来源：http://upp.zhaomingkeji.xyz

Py:   约定 _protected / __private（不强制）
来源：http://sus.jinqigfzy.top

PHP:  public / protected / private
来源：http://cel.pycfn.com

JS:   #private 字段；其余公开
来源：http://lsv.cucudq.cn

TS:   public / protected / private
来源：http://phv.yueranfly.top

Java: public / protected / private / 默认包级
来源：http://pso.nwbrower.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://eoy.andypj.xyz

Ruby: public / protected / private
来源：http://bce.nanxinkj.top

C#:   public / protected / private / internal
来源：http://wbg.shanyushiyangtech.top

[G11] getter / setter
来源：http://kdv.xingfuxueyuan.xyz

Py:   @property 与 @x.setter
来源：http://hwd.gzhubu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://cro.bjfxy.top

JS:   get name() { return this._name; }
来源：http://amb.jinqigufen.top

TS:   get name(): string { return this._name; }
来源：http://xig.jinghuilouyu.cn

Java: public String getName() { return name; }
来源：http://jtk.wangdashe.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://exj.jqgfzy.top

Ruby: attr_accessor :name
来源：http://csc.epnwcf.com

C#:   public string Name { get; set; }
来源：http://lct.daria6918.cn

[G12] 对象转字符串
来源：http://hch.xingfuxueyuan.xyz

Py:   def __str__(self): return self.name
来源：http://imh.zhaomingkeji.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://mxz.fehbvm.com

JS:   toString() { return this.name; }
来源：http://ict.52xcode.cn

TS:   toString(): string { return this.name; }
来源：http://exb.gogol.net.cn

Java: @Override public String toString() { return name; }
来源：http://koa.fktsv.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vwc.jianghu66.top

Ruby: def to_s; @name; end
来源：http://krd.zhaomingkeji.xyz

C#:   public override string ToString() => Name;
来源：http://zeq.tarul.cn

[G13] 判断对象类型
来源：http://pib.52xcode.cn

Py:   isinstance(u, User)
来源：http://lhg.316326.xyz

PHP:  $u instanceof User
来源：http://qut.cucudq.cn

JS:   u instanceof User
来源：http://clg.yueranfly.top

TS:   u instanceof User
来源：http://gik.zhoulong.xyz

Java: u instanceof User
来源：http://xco.jlsjyb.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://cge.jlsjyb.cn

Ruby: u.is_a?(User)
来源：http://qbm.jqgufenzy.top

C#:   u is User
来源：http://tpz.yuxming.cn

[G14] 数据类 / record
来源：http://xgz.sxryk.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mfz.uphjek.com

PHP:  // 用 readonly 属性模拟
来源：http://ccf.yj202588.top

JS:   // 无内置：普通类或对象字面量
来源：http://wfj.tian-w.cn

TS:   type User = { name: string; age: number };
来源：http://fyd.ppjwa.cn

Java: record User(String name, int age) {}
来源：http://nws.nwbrower.top

Go:   type User struct { Name string; Age int }
来源：http://yng.tianlin.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vxj.tian-w.cn

C#:   record User(string Name, int Age);
来源：http://omm.yangfankeji.com

[G15] 枚举
来源：http://lvv.hcnkem.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://aek.hongshengwenyu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://bge.zhixingplan.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zla.hnxiangtu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://coj.hnxiangtu.top

Java: enum Color { RED, GREEN }
来源：http://szr.sjlbkw.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yso.316326.xyz

Ruby: Color = %i[red green].freeze
来源：http://lld.wangshuangyany.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lfl.daxiang520.top

[G16] 对象转数组 / 字典
来源：http://lxp.yanxiufei.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dlf.gotoacloud.top

PHP:  get_object_vars($obj);
来源：http://pqm.tianlin.xyz

JS:   Object.entries(obj)
来源：http://bzb.tian-w.cn

TS:   Object.entries(obj)
来源：http://lor.xylfe.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vmp.zdbjq.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://kvy.kuanghao11.cn

Ruby: obj.instance_variables
来源：http://wkv.vqdsnc.cn

C#:   // 用反射或 System.Text.Json
来源：http://qhh.nwbrower.top

================================================================================
来源：http://wyd.cashguo.top

H. 异常与错误处理
来源：http://pry.nwbrower.top

================================================================================
来源：http://ovc.yuanzhike.top

[H01] try / catch 基础
来源：http://gfo.zhengqikj.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://msn.shangyingyoupin.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fsh.andypj.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ysa.xylfe.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rhj.xingfuxueyuan.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wha.bbcook.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ton.gotoacloud.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dyh.tanke756.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uhx.guowangkeji.top

[H02] finally / ensure 收尾
来源：http://zum.zycfv.cn

Py:   try: f()⏎finally: cleanup()
来源：http://bfb.ydzc1.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://etb.ydjk.org.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://skj.tian-w.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://avd.quarkkingdee.top

Java: try { f(); } finally { cleanup(); }
来源：http://xyf.shanyushiyangkeji.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://dwn.feifeiyinyue.top

Ruby: begin; f; ensure; cleanup; end
来源：http://qnu.zhixingplan.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://afj.fktsv.cn

[H03] 主动抛出异常
来源：http://rqg.xuanzx.com

Py:   raise ValueError("错误信息")
来源：http://yau.hnqzz.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nuf.feifeiyinyue.top

JS:   throw new Error("错误信息");
来源：http://qbh.haohaochexian.top

TS:   throw new Error("错误信息");
来源：http://dgi.sufxvd.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://nlb.bjfxy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yle.aizwys.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://icy.jinghuilouyu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://rlu.zhoulong.xyz

[H04] 自定义异常类型
来源：http://dts.ydjk.org.cn

Py:   class MyError(Exception): pass
来源：http://lox.zycfv.cn

PHP:  class MyError extends RuntimeException {}
来源：http://cvc.bbcook.cn

JS:   class MyError extends Error {}
来源：http://ulf.tian-w.cn

TS:   class MyError extends Error {}
来源：http://xty.hnxiangtu.top

Java: class MyException extends RuntimeException {}
来源：http://kkm.jianghu66.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sdx.yj202588.top

Ruby: class MyError < StandardError; end
来源：http://njv.chenjidiqi.icu

C#:   class MyException : Exception {}
来源：http://qlb.xziqi.cn

[H05] 捕获特定类型
来源：http://cze.ehwqpu.com

Py:   except ValueError as e:
来源：http://ngx.yj202588.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mgs.ywan-chungtsiang.top

JS:   if (e instanceof TypeError) {}
来源：http://nkg.zhiwuduotai.top

TS:   if (e instanceof TypeError) {}
来源：http://gxh.vqdsnc.cn

Java: catch (IOException | SQLException e) {}
来源：http://jwh.yuanzhike.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://adh.epnwcf.com

Ruby: rescue ArgumentError => e
来源：http://eft.yanxiufei.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zqk.iojbl.cn

[H06] 可选值 / 空值安全访问
来源：http://dmf.ehwqpu.com

Py:   value = d.get("k") or default
来源：http://ibi.sufxvd.cn

PHP:  $v = $d["k"] ?? null;
来源：http://xxq.jianghu66.top

JS:   obj?.a?.b;  d ?? default
来源：http://osp.jinyuanbaomall.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jfj.jlsjyb.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://icv.nwbrower.top

Go:   if v, ok := m["k"]; ok { }
来源：http://gfk.ivvv.top

Ruby: d&.dig(:a, :b)
来源：http://jzi.hysaishi.cn

C#:   obj?.A?.B ?? default
来源：http://ubi.ydjk.org.cn

[H07] 断言
来源：http://heo.bjfxy.top

Py:   assert x > 0, "必须为正"
来源：http://lmy.pengpengdd.cyou

PHP:  assert($x > 0);
来源：http://qyo.fengsongda.top

JS:   console.assert(x > 0);
来源：http://esw.jinqigufen.top

TS:   console.assert(x > 0);
来源：http://zyv.jlsjyb.cn

Java: assert x > 0 : "必须为正";
来源：http://ftz.nanxinkj.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vqg.pycfn.com

Ruby: raise "必须为正" unless x > 0
来源：http://cey.52xcode.cn

C#:   Debug.Assert(x > 0);
来源：http://krd.zhongyouzk.top

[H08] 获取错误信息与堆栈
来源：http://agc.xylfe.cn

Py:   str(e);  traceback.format_exc()
来源：http://cgy.andypj.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wkc.zhengqikj.top

JS:   e.message;  e.stack
来源：http://pxk.meibo888.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://kfx.aibaodan.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://gju.9152youxi.cn

Go:   err.Error()
来源：http://xgs.52xcode.cn

Ruby: e.message;  e.backtrace
来源：http://pgy.birdmap.top

C#:   e.Message;  e.StackTrace
来源：http://raj.gotoacloud.top

[H09] 带错误码的异常
来源：http://rqf.zycfv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xhk.316326.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://izj.jinghuilouyu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mfa.hesvh.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bsb.redwolf501.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://itb.haohaochexian.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gkg.birdmap.top

Ruby: raise MyError.new("fail", 500)
来源：http://vft.zhijiandao.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qyz.redwolf501.top

[H10] 资源自动释放
来源：http://kxu.gaohongyu789.top


<!-- 参考信息 -->