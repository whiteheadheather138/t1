代发 wailian999

C#:   File.Exists("a.txt")
来源：http://skr.gaohongyu789.top

[F06] 删除文件
来源：http://bfg.ywan-chungtsiang.top

Py:   os.remove("a.txt")
来源：http://vdz.sysykeji.top

PHP:  unlink("a.txt");
来源：http://ymo.gzhubu.top

JS:   fs.unlinkSync("a.txt")
来源：http://vus.dianchejie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nfz.tarul.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ics.mhx1999.top

Go:   os.Remove("a.txt")
来源：http://kei.chenzaomai.com

Ruby: File.delete("a.txt")
来源：http://ukx.zhijiandao.cn

C#:   File.Delete("a.txt");
来源：http://mbb.chenlongwang.top

[F07] 创建目录（含多级）
来源：http://imf.wangdashe.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mxe.jiagoushi.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gkn.mhx1999.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mdy.0kj1m.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vmo.9152youxi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qcg.yj20258.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jdo.nanxuanxn.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nxr.wangdashe.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uyq.tarul.cn

[F08] 遍历目录
来源：http://bvr.tianlin.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://rak.sufxvd.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xzb.xziqi.cn

JS:   fs.readdirSync("dir")
来源：http://gbb.9152youxi.cn

TS:   fs.readdirSync("dir")
来源：http://oic.jinqigfzy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ocz.havefunace.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ptf.andypj.xyz

Ruby: Dir.children("dir")
来源：http://xvh.ppjwa.cn

C#:   Directory.GetFiles("dir")
来源：http://eau.jinyuanbaomall.cn

[F09] 获取文件大小
来源：http://fxo.zhaomingkeji.xyz

Py:   os.path.getsize("a.txt")
来源：http://dad.hcnkem.com

PHP:  filesize("a.txt");
来源：http://wqe.tanke756.top

JS:   fs.statSync("a.txt").size
来源：http://txa.jinghuilouyu.cn

TS:   fs.statSync("a.txt").size
来源：http://vvp.yangfankeji.com

Java: Files.size(Path.of("a.txt"))
来源：http://phm.ppjwa.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rgb.ctjpmb.com

Ruby: File.size("a.txt")
来源：http://akz.hammf.cn

C#:   new FileInfo("a.txt").Length
来源：http://rzg.yueranfly.top

[F10] 取文件扩展名 / 文件名
来源：http://gdf.hysaishi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xez.sxryk.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fbk.ybcxt.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://czr.bbcook.cn

TS:   path.extname("a.txt")
来源：http://okq.hfpthk.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gju.yvedp.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qhn.jyoumei.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://krq.yfazqb.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xvv.vqdsnc.cn

[F11] 复制与移动文件
来源：http://lil.sweek.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://obh.mhx1999.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wkf.hammf.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vuz.jianghu66.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qjx.fktsv.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zku.0kj1m.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tug.shangyingyoupin.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dkr.ivvv.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://aqr.jiagoushi.top

[F12] CSV 读写
来源：http://und.ehwqpu.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ugv.zhoulong.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zsc.daxiang520.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ejb.vehdjk.com

TS:   // 同上
来源：http://nnx.gotoacloud.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cuh.guowangkeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ype.zhiwuduotai.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://quf.smart0.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://jml.zhongyouzk.top

================================================================================
来源：http://vsp.daxiang520.top

G. 面向对象
来源：http://ufx.sufxvd.cn

================================================================================
来源：http://iet.hesvh.cn

[G01] 定义类
来源：http://fum.yueranfly.top

Py:   class User: pass
来源：http://rdv.daxiang520.top

PHP:  class User {}
来源：http://qvq.vehdjk.com

JS:   class User {}
来源：http://onj.daria6918.cn

TS:   class User { name: string = ""; }
来源：http://zns.zycfv.cn

Java: class User {}
来源：http://ckd.yangfankeji.com

Go:   type User struct { Name string }
来源：http://oxq.ehwqpu.com

Ruby: class User; end
来源：http://ljg.hammf.cn

C#:   class User {}
来源：http://myv.gaohongyu789.top

[G02] 构造函数
来源：http://fiz.daxiang520.top

Py:   def __init__(self, name): self.name = name
来源：http://cll.hnxiangtu.top

PHP:  public function __construct(public string $name) {}
来源：http://ywf.zhaomingkeji.xyz

JS:   constructor(name) { this.name = name; }
来源：http://ypu.chenjidiqi.icu

TS:   constructor(public name: string) {}
来源：http://jrg.sjlbkw.cn

Java: User(String name) { this.name = name; }
来源：http://vst.yuxming.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yfn.yuxming.cn

Ruby: def initialize(name); @name = name; end
来源：http://mcp.yongpay.top

C#:   public User(string name) { Name = name; }
来源：http://qdv.epnwcf.com

[G03] 实例属性
来源：http://ngc.0kj1m.cn

Py:   self.name = "x"
来源：http://fjj.jianghu66.top

PHP:  public string $name = "x";
来源：http://wed.yj202588.top

JS:   this.name = "x";
来源：http://yjn.birdmap.top

TS:   name: string = "x";
来源：http://wpl.jinqigufen.top

Java: private String name;
来源：http://jpv.sufxvd.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ldo.yfazqb.com

Ruby: @name = "x"
来源：http://fom.uphjek.com

C#:   public string Name { get; set; } = "x";
来源：http://dmt.jqgfzy.top

[G04] 定义方法
来源：http://hov.tanke756.top

Py:   def greet(self): return self.name
来源：http://iid.xinyue.icu

PHP:  public function greet(): string { return $this->name; }
来源：http://byp.hysaishi.cn

JS:   greet() { return this.name; }
来源：http://zsx.yanxiufei.cn

TS:   greet(): string { return this.name; }
来源：http://pbl.fktsv.cn

Java: String greet() { return name; }
来源：http://bfc.ctjpmb.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://pfv.xingfuxueyuan.xyz

Ruby: def greet; @name; end
来源：http://dyl.ppjwa.cn

C#:   public string Greet() => Name;
来源：http://jjq.hammf.cn

[G05] 继承
来源：http://cbj.ydzc1.top

Py:   class Admin(User): pass
来源：http://vrn.iojbl.cn

PHP:  class Admin extends User {}
来源：http://toa.yj20258.top

JS:   class Admin extends User {}
来源：http://dsh.sjlbkw.cn

TS:   class Admin extends User {}
来源：http://lfe.ctjpmb.com

Java: class Admin extends User {}
来源：http://vxp.tanke756.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hga.meibo888.top

Ruby: class Admin < User; end
来源：http://ooc.hammf.cn

C#:   class Admin : User {}
来源：http://ypf.shanyushiyangtech.top

[G06] 重写方法
来源：http://csw.jiagoushi.top

Py:   def greet(self): return "admin"
来源：http://rpy.zhoulong.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://bha.guowangkeji.top

JS:   greet() { return "admin"; }
来源：http://voc.sjlbkw.cn

TS:   greet(): string { return "admin"; }
来源：http://hpw.shanyushiyangkeji.top

Java: @Override String greet() { return "admin"; }
来源：http://qlt.c1oappe.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vbg.tarul.cn

Ruby: def greet; "admin"; end
来源：http://aod.hnqzz.top

C#:   public override string Greet() => "admin";
来源：http://zfk.yvedp.cn

[G07] 调用父类方法
来源：http://loq.ybcxt.top

Py:   super().greet()
来源：http://erb.ivvv.top

PHP:  parent::greet();
来源：http://tli.chenlongwang.top

JS:   super.greet();
来源：http://ble.tanke756.top

TS:   super.greet();
来源：http://acm.jinyuanbaomall.cn

Java: super.greet();
来源：http://fbc.tianlin.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://oxi.cucudq.cn

Ruby: super
来源：http://spd.chenlongwang.top

C#:   base.Greet();
来源：http://cxe.cqqwz.cn

[G08] 静态方法与属性
来源：http://dzq.guowangkeji.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jkp.zhaomingkeji.xyz

PHP:  public static function f() {}
来源：http://vie.kuanghao11.cn

JS:   static f() {}
来源：http://mib.9152youxi.cn

TS:   static f(): void {}
来源：http://aye.mhx1999.top

Java: static void f() {}
来源：http://wwr.redwolf501.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://pkf.yuxming.cn

Ruby: def self.f; end
来源：http://qbg.zhiwuduotai.top

C#:   public static void F() {}
来源：http://njo.yonumen.top

[G09] 接口 / 抽象类
来源：http://llz.zhixingplan.top

Py:   from abc import ABC, abstractmethod
来源：http://kjd.hywenlv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bhp.gotoacloud.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://gig.shanyushiyangtech.top

TS:   interface Shape { area(): number; }
来源：http://qtf.ivvv.top

Java: interface Shape { double area(); }
来源：http://wur.gzhubu.top

Go:   type Shape interface { Area() float64 }
来源：http://kcd.meibo888.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pvf.chenlongwang.top

C#:   interface IShape { double Area(); }
来源：http://zal.daria6918.cn

[G10] 访问控制
来源：http://vlx.nanxinkj.top

Py:   约定 _protected / __private（不强制）
来源：http://eos.sxryk.cn

PHP:  public / protected / private
来源：http://kgr.hcnkem.com

JS:   #private 字段；其余公开
来源：http://mpx.ywan-chungtsiang.top

TS:   public / protected / private
来源：http://lfe.zhengqikj.top

Java: public / protected / private / 默认包级
来源：http://wbk.yongpay.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://jwu.yj202588.top

Ruby: public / protected / private
来源：http://nte.hesvh.cn

C#:   public / protected / private / internal
来源：http://jpx.guannengcc.top

[G11] getter / setter
来源：http://qbm.daxiang520.top

Py:   @property 与 @x.setter
来源：http://mes.9152youxi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fqh.cqqwz.cn

JS:   get name() { return this._name; }
来源：http://sqr.feifeiyinyue.top

TS:   get name(): string { return this._name; }
来源：http://hil.jqgufenzy.top

Java: public String getName() { return name; }
来源：http://bzk.andypj.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://gny.quarkkingdee.top

Ruby: attr_accessor :name
来源：http://lrk.shuidangran.top

C#:   public string Name { get; set; }
来源：http://szv.uphjek.com

[G12] 对象转字符串
来源：http://ixt.cqqwz.cn

Py:   def __str__(self): return self.name
来源：http://txz.kuanghao11.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://uhv.wangshuangyany.cn

JS:   toString() { return this.name; }
来源：http://vmr.xinyue.icu

TS:   toString(): string { return this.name; }
来源：http://kdv.vqdsnc.cn

Java: @Override public String toString() { return name; }
来源：http://pmw.nanxuanxn.top

Go:   func (u User) String() string { return u.Name }
来源：http://qdv.chenzaomai.com

Ruby: def to_s; @name; end
来源：http://ohv.sysykeji.top

C#:   public override string ToString() => Name;
来源：http://wya.jiagoushi.top

[G13] 判断对象类型
来源：http://dav.hcnkem.com

Py:   isinstance(u, User)
来源：http://hdi.hysaishi.cn

PHP:  $u instanceof User
来源：http://brt.yuxming.cn

JS:   u instanceof User
来源：http://csw.jinyuanbaomall.cn

TS:   u instanceof User
来源：http://slr.yanxiufei.cn

Java: u instanceof User
来源：http://ela.yj20258.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://wmt.daria6918.cn

Ruby: u.is_a?(User)
来源：http://ksq.hnqzz.top

C#:   u is User
来源：http://vcj.tanke756.top

[G14] 数据类 / record
来源：http://vnx.ywan-chungtsiang.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://oju.wangshuangyany.cn

PHP:  // 用 readonly 属性模拟
来源：http://rvv.jqgufenzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://lct.shanyushiyangtech.top

TS:   type User = { name: string; age: number };
来源：http://moc.c1oappe.top

Java: record User(String name, int age) {}
来源：http://klj.bbcook.cn

Go:   type User struct { Name string; Age int }
来源：http://vjm.aibaodan.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fif.uphjek.com

C#:   record User(string Name, int Age);
来源：http://hpa.ehwqpu.com

[G15] 枚举
来源：http://phr.zhongyouzk.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mlu.jqgfzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://qfg.redwolf501.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ywq.bbcook.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jgb.chenzaomai.com

Java: enum Color { RED, GREEN }
来源：http://rlm.cdnleiting.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zkw.pengpengdd.cyou

Ruby: Color = %i[red green].freeze
来源：http://xfw.ydjk.org.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ddj.hywenlv.cn

[G16] 对象转数组 / 字典
来源：http://lzz.nanxinkj.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cib.chenlongwang.top

PHP:  get_object_vars($obj);
来源：http://vuk.wangdashe.top

JS:   Object.entries(obj)
来源：http://cjo.ydjk.org.cn

TS:   Object.entries(obj)
来源：http://waq.jlsjyb.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://znv.snrcjt.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gyy.haohaochexian.top

Ruby: obj.instance_variables
来源：http://hbe.yj202588.top

C#:   // 用反射或 System.Text.Json
来源：http://ewh.xingfuxueyuan.xyz

================================================================================
来源：http://pio.yj20258888.top

H. 异常与错误处理
来源：http://jqy.yuanzhike.top

================================================================================
来源：http://ygd.cheryme.top

[H01] try / catch 基础
来源：http://wzg.hongshengwenyu.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://aja.ydjk.org.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ojh.hongshengwenyu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lfw.aibaodan.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uvp.smart0.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dkt.zhoulong.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yus.aizwys.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lkn.guowangkeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ana.chenzaomai.com

[H02] finally / ensure 收尾
来源：http://bbm.cdnleiting.top

Py:   try: f()⏎finally: cleanup()
来源：http://sxq.hnqzz.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://lob.xinyue.icu

JS:   try { f(); } finally { cleanup(); }
来源：http://nrz.aizwys.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mui.uphjek.com

Java: try { f(); } finally { cleanup(); }
来源：http://fwu.yongpay.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://svj.zhoulong.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://vaw.yj20258888.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://mew.xinyue.icu

[H03] 主动抛出异常
来源：http://dkp.gzhubu.top

Py:   raise ValueError("错误信息")
来源：http://xpc.shangyingyoupin.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mdj.316326.xyz

JS:   throw new Error("错误信息");
来源：http://omv.xuanzx.com

TS:   throw new Error("错误信息");
来源：http://yqh.shanyushiyangkeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://cjg.shanyushiyangkeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kdf.hnqzz.top

Ruby: raise ArgumentError, "错误信息"
来源：http://gry.ybcxt.top

C#:   throw new ArgumentException("错误信息");
来源：http://roe.hfpthk.cn

[H04] 自定义异常类型
来源：http://wue.andypj.xyz

Py:   class MyError(Exception): pass
来源：http://heu.nwbrower.top

PHP:  class MyError extends RuntimeException {}
来源：http://jat.zhaomingkeji.xyz

JS:   class MyError extends Error {}
来源：http://rgv.zhengqikj.top

TS:   class MyError extends Error {}
来源：http://nkx.xuetiantiany.cn

Java: class MyException extends RuntimeException {}
来源：http://stv.sufxvd.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qcp.yuanzhike.top

Ruby: class MyError < StandardError; end
来源：http://uev.xinyue.icu

C#:   class MyException : Exception {}
来源：http://hhx.snrcjt.cn

[H05] 捕获特定类型
来源：http://mfe.dashuyun.cn

Py:   except ValueError as e:
来源：http://inw.zhoulong.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xgn.dianchejie.cn

JS:   if (e instanceof TypeError) {}
来源：http://svl.tianlin.xyz

TS:   if (e instanceof TypeError) {}
来源：http://nqv.yuanzhike.top

Java: catch (IOException | SQLException e) {}
来源：http://ern.jiagoushi.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vid.zdbjq.cn

Ruby: rescue ArgumentError => e
来源：http://lpk.kuanghao11.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cwp.tanke756.top

[H06] 可选值 / 空值安全访问
来源：http://vdk.zhijiandao.cn

Py:   value = d.get("k") or default
来源：http://uqo.cdnleiting.top

PHP:  $v = $d["k"] ?? null;
来源：http://aka.zdbjq.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mhn.haohaochexian.top

TS:   obj?.a?.b;  d ?? default
来源：http://wuw.ywan-chungtsiang.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dio.yfazqb.com

Go:   if v, ok := m["k"]; ok { }
来源：http://qwq.ydzc1.top

Ruby: d&.dig(:a, :b)
来源：http://fds.nanxinkj.top

C#:   obj?.A?.B ?? default
来源：http://qnq.yangfankeji.com

[H07] 断言
来源：http://dnl.0kj1m.cn

Py:   assert x > 0, "必须为正"
来源：http://pda.cashguo.top

PHP:  assert($x > 0);
来源：http://ucp.c1oappe.top

JS:   console.assert(x > 0);
来源：http://lym.jlsjyb.cn

TS:   console.assert(x > 0);
来源：http://mrd.yuxming.cn

Java: assert x > 0 : "必须为正";
来源：http://dek.sjlbkw.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rtn.haohaochexian.top

Ruby: raise "必须为正" unless x > 0
来源：http://eel.sysykeji.top

C#:   Debug.Assert(x > 0);
来源：http://dht.pengpengdd.cyou

[H08] 获取错误信息与堆栈
来源：http://xho.yj202588.top

Py:   str(e);  traceback.format_exc()
来源：http://zep.yongpay.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tms.chenzaomai.com

JS:   e.message;  e.stack
来源：http://qza.jiagoushi.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://iep.cashguo.top

Java: e.getMessage();  e.printStackTrace()
来源：http://bug.vqdsnc.cn

Go:   err.Error()
来源：http://bku.hywenlv.cn

Ruby: e.message;  e.backtrace
来源：http://xuc.yj20258888.top

C#:   e.Message;  e.StackTrace
来源：http://uhh.hcnkem.com

[H09] 带错误码的异常
来源：http://bsl.feifeiyinyue.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://uwz.zhiwuduotai.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://iqq.quarkkingdee.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mui.cashguo.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yhq.ehwqpu.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bdu.jianghu66.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://iyu.jqgfzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://nnu.wangdashe.top

C#:   // 自定义异常类中加 Code 属性
来源：http://lxh.zhijiandao.cn

[H10] 资源自动释放
来源：http://lgu.chenzaomai.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://mop.fengsongda.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sky.nanxuanxn.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://udz.hongshengwenyu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tth.shzxlz.cn


<!-- 参考信息 -->