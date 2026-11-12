代发 wailian999

Ruby: File.delete("a.txt")
来源：http://gbw.fanxiaobao.xyz

C#:   File.Delete("a.txt");
来源：http://xne.hywenlv.cn

[F07] 创建目录（含多级）
来源：http://pyf.xuetiantiany.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zrn.zhengqikj.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ula.hywenlv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blq.ybcxt.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ldy.gzhubu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hiy.zdqjudy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fcx.52xcode.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ibu.zhengqikj.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vsl.ybcxt.top

[F08] 遍历目录
来源：http://fds.hnxiangtu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://gtd.feifeiyinyue.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://iod.yanxiufei.cn

JS:   fs.readdirSync("dir")
来源：http://wqs.fzhhl.top

TS:   fs.readdirSync("dir")
来源：http://bzy.zdbjq.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rsj.zhaomingkeji.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://jik.kuanghao11.cn

Ruby: Dir.children("dir")
来源：http://oqj.xuetiantiany.cn

C#:   Directory.GetFiles("dir")
来源：http://mtj.nanxinkj.top

[F09] 获取文件大小
来源：http://vch.redwolf501.top

Py:   os.path.getsize("a.txt")
来源：http://qwk.yuxming.cn

PHP:  filesize("a.txt");
来源：http://hrw.zhoulong.xyz

JS:   fs.statSync("a.txt").size
来源：http://wsm.gogol.net.cn

TS:   fs.statSync("a.txt").size
来源：http://xwb.ivvv.top

Java: Files.size(Path.of("a.txt"))
来源：http://zrv.hnxiangtu.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ixy.yanxiufei.cn

Ruby: File.size("a.txt")
来源：http://hbl.aizwys.cn

C#:   new FileInfo("a.txt").Length
来源：http://umm.ctjpmb.com

[F10] 取文件扩展名 / 文件名
来源：http://emb.nwbrower.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xuy.bjfxy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jio.shangyingyoupin.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hic.ehwqpu.com

TS:   path.extname("a.txt")
来源：http://usw.wangdashe.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kgw.nanxinkj.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qmd.tianlin.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://aun.52xcode.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cpj.meibo888.top

[F11] 复制与移动文件
来源：http://scw.cashguo.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tio.ivvv.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://amr.jinqigfzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dlq.meibo888.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yiq.hcnkem.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nwu.vehdjk.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://iok.gaohongyu789.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://akc.tanke756.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://iqg.zhiwuduotai.top

[F12] CSV 读写
来源：http://rlf.aibaodan.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://eky.ctjpmb.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fgc.aibaodan.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://iam.snrcjt.cn

TS:   // 同上
来源：http://oqs.cheryme.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wsg.wangdashe.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ena.zhiwuduotai.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ycs.yongpay.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ahj.yueranfly.top

================================================================================
来源：http://fbv.ywan-chungtsiang.top

G. 面向对象
来源：http://nxf.haohaochexian.top

================================================================================
来源：http://wjm.jqgfzy.top

[G01] 定义类
来源：http://udp.hongshengwenyu.top

Py:   class User: pass
来源：http://exe.ehwqpu.com

PHP:  class User {}
来源：http://xpt.pengpengdd.cyou

JS:   class User {}
来源：http://hwa.hesvh.cn

TS:   class User { name: string = ""; }
来源：http://gya.jiagoushi.top

Java: class User {}
来源：http://fvj.nanxuanxn.top

Go:   type User struct { Name string }
来源：http://ncn.daria6918.cn

Ruby: class User; end
来源：http://bor.jqgufenzy.top

C#:   class User {}
来源：http://ybj.snrcjt.cn

[G02] 构造函数
来源：http://ogv.tarul.cn

Py:   def __init__(self, name): self.name = name
来源：http://jaf.smart0.xyz

PHP:  public function __construct(public string $name) {}
来源：http://ebm.xingfuxueyuan.xyz

JS:   constructor(name) { this.name = name; }
来源：http://lqo.chenjidiqi.icu

TS:   constructor(public name: string) {}
来源：http://acw.zhiwuduotai.top

Java: User(String name) { this.name = name; }
来源：http://qmr.zhiwuduotai.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bxy.cdnleiting.top

Ruby: def initialize(name); @name = name; end
来源：http://got.yfazqb.com

C#:   public User(string name) { Name = name; }
来源：http://eae.hcnkem.com

[G03] 实例属性
来源：http://exv.jinqigfzy.top

Py:   self.name = "x"
来源：http://bpe.nanxinkj.top

PHP:  public string $name = "x";
来源：http://yrl.cdnleiting.top

JS:   this.name = "x";
来源：http://dme.gogol.net.cn

TS:   name: string = "x";
来源：http://xxu.meibo888.top

Java: private String name;
来源：http://faj.cqqwz.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jto.hesvh.cn

Ruby: @name = "x"
来源：http://nlo.vqdsnc.cn

C#:   public string Name { get; set; } = "x";
来源：http://eqx.yuxming.cn

[G04] 定义方法
来源：http://qwd.yj20258.top

Py:   def greet(self): return self.name
来源：http://fhd.zhoulong.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://mpj.shzxlz.cn

JS:   greet() { return this.name; }
来源：http://umb.ivvv.top

TS:   greet(): string { return this.name; }
来源：http://nsf.hammf.cn

Java: String greet() { return name; }
来源：http://ihv.nanxinkj.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ymx.ywan-chungtsiang.top

Ruby: def greet; @name; end
来源：http://jxv.zdqjudy.top

C#:   public string Greet() => Name;
来源：http://xce.redwolf501.top

[G05] 继承
来源：http://lly.yonumen.top

Py:   class Admin(User): pass
来源：http://rjz.316326.xyz

PHP:  class Admin extends User {}
来源：http://ppu.xuetiantiany.cn

JS:   class Admin extends User {}
来源：http://bah.fehbvm.com

TS:   class Admin extends User {}
来源：http://htn.shzxlz.cn

Java: class Admin extends User {}
来源：http://iya.yueranfly.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vmn.dianchejie.cn

Ruby: class Admin < User; end
来源：http://acn.nanxuanxn.top

C#:   class Admin : User {}
来源：http://uvu.guannengcc.top

[G06] 重写方法
来源：http://eky.fktsv.cn

Py:   def greet(self): return "admin"
来源：http://kyd.xingfuxueyuan.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://zqc.tian-w.cn

JS:   greet() { return "admin"; }
来源：http://lms.kuanghao11.cn

TS:   greet(): string { return "admin"; }
来源：http://sqz.nwbrower.top

Java: @Override String greet() { return "admin"; }
来源：http://lte.kuanghao11.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kuh.cqqwz.cn

Ruby: def greet; "admin"; end
来源：http://uqz.jlsjyb.cn

C#:   public override string Greet() => "admin";
来源：http://swl.yj20258888.top

[G07] 调用父类方法
来源：http://vpu.quarkkingdee.top

Py:   super().greet()
来源：http://xlp.hysaishi.cn

PHP:  parent::greet();
来源：http://wqn.chenzaomai.com

JS:   super.greet();
来源：http://mpi.fktsv.cn

TS:   super.greet();
来源：http://wsg.dianchejie.cn

Java: super.greet();
来源：http://prk.yj202588.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xty.jqgufenzy.top

Ruby: super
来源：http://hmm.xuetiantiany.cn

C#:   base.Greet();
来源：http://tcz.meibo888.top

[G08] 静态方法与属性
来源：http://ted.9152youxi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rzu.birdmap.top

PHP:  public static function f() {}
来源：http://cdg.yuxming.cn

JS:   static f() {}
来源：http://nki.tian-w.cn

TS:   static f(): void {}
来源：http://vac.hfpthk.cn

Java: static void f() {}
来源：http://yjx.shanyushiyangkeji.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://koc.chenzaomai.com

Ruby: def self.f; end
来源：http://dya.shanyushiyangtech.top

C#:   public static void F() {}
来源：http://kqc.ydzc1.top

[G09] 接口 / 抽象类
来源：http://dwh.shzxlz.cn

Py:   from abc import ABC, abstractmethod
来源：http://pqt.pycfn.com

PHP:  interface Shape { public function area(): float; }
来源：http://bmd.dashuyun.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://cmp.zhoulong.xyz

TS:   interface Shape { area(): number; }
来源：http://evj.vqdsnc.cn

Java: interface Shape { double area(); }
来源：http://jqw.pengpengdd.cyou

Go:   type Shape interface { Area() float64 }
来源：http://qhx.jinyuanbaomall.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sya.daria6918.cn

C#:   interface IShape { double Area(); }
来源：http://joo.shanyushiyangkeji.top

[G10] 访问控制
来源：http://vbw.zdqjudy.top

Py:   约定 _protected / __private（不强制）
来源：http://ffu.wangdashe.top

PHP:  public / protected / private
来源：http://zik.yuxming.cn

JS:   #private 字段；其余公开
来源：http://wns.sysykeji.top

TS:   public / protected / private
来源：http://vqe.feifeiyinyue.top

Java: public / protected / private / 默认包级
来源：http://vjf.daria6918.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://sbi.gzhubu.top

Ruby: public / protected / private
来源：http://gfu.redwolf501.top

C#:   public / protected / private / internal
来源：http://ugf.hesvh.cn

[G11] getter / setter
来源：http://uiv.yj20258888.top

Py:   @property 与 @x.setter
来源：http://akt.316326.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://jic.ywan-chungtsiang.top

JS:   get name() { return this._name; }
来源：http://bxd.sjlbkw.cn

TS:   get name(): string { return this._name; }
来源：http://wdw.jqgfzy.top

Java: public String getName() { return name; }
来源：http://npc.wangshuangyany.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zda.shuidangran.top

Ruby: attr_accessor :name
来源：http://nby.fehbvm.com

C#:   public string Name { get; set; }
来源：http://osp.cdnleiting.top

[G12] 对象转字符串
来源：http://fue.ctjpmb.com

Py:   def __str__(self): return self.name
来源：http://ejp.hywenlv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jcm.dianchejie.cn

JS:   toString() { return this.name; }
来源：http://fdl.pycfn.com

TS:   toString(): string { return this.name; }
来源：http://opg.shanyushiyangkeji.top

Java: @Override public String toString() { return name; }
来源：http://ljf.ppjwa.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ywg.haohaochexian.top

Ruby: def to_s; @name; end
来源：http://weo.fzhhl.top

C#:   public override string ToString() => Name;
来源：http://iqf.yonumen.top

[G13] 判断对象类型
来源：http://xvs.yj202588.top

Py:   isinstance(u, User)
来源：http://rfw.ppjwa.cn

PHP:  $u instanceof User
来源：http://chu.quarkkingdee.top

JS:   u instanceof User
来源：http://sxq.tianlin.xyz

TS:   u instanceof User
来源：http://ilv.shzxlz.cn

Java: u instanceof User
来源：http://pqe.hammf.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://awp.daxiang520.top

Ruby: u.is_a?(User)
来源：http://xpq.ybcxt.top

C#:   u is User
来源：http://wer.zhongyouzk.top

[G14] 数据类 / record
来源：http://all.cucudq.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hzl.jlsjyb.cn

PHP:  // 用 readonly 属性模拟
来源：http://owk.shuidangran.top

JS:   // 无内置：普通类或对象字面量
来源：http://ezt.yangfankeji.com

TS:   type User = { name: string; age: number };
来源：http://oml.shuidangran.top

Java: record User(String name, int age) {}
来源：http://hzl.ivvv.top

Go:   type User struct { Name string; Age int }
来源：http://pys.jinghuilouyu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dwr.jinqigfzy.top

C#:   record User(string Name, int Age);
来源：http://elp.smart0.xyz

[G15] 枚举
来源：http://rsx.ydjk.org.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dpj.xziqi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bft.zycfv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qsn.ywan-chungtsiang.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://juk.tanke756.top

Java: enum Color { RED, GREEN }
来源：http://ixd.fanxiaobao.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pvl.xingfuxueyuan.xyz

Ruby: Color = %i[red green].freeze
来源：http://son.zhoulong.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xbh.wangdashe.top

[G16] 对象转数组 / 字典
来源：http://wdy.zhoulong.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wzn.jinyuanbaomall.cn

PHP:  get_object_vars($obj);
来源：http://amq.pengpengdd.cyou

JS:   Object.entries(obj)
来源：http://gqt.smart0.xyz

TS:   Object.entries(obj)
来源：http://szo.zhoulong.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://euk.ppjwa.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ryh.zhixingplan.top

Ruby: obj.instance_variables
来源：http://cjx.sxryk.cn

C#:   // 用反射或 System.Text.Json
来源：http://mjn.aibaodan.cn

================================================================================
来源：http://lya.bjfxy.top

H. 异常与错误处理
来源：http://bge.guannengcc.top

================================================================================
来源：http://cmx.uphjek.com

[H01] try / catch 基础
来源：http://gia.tianlin.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vcn.yangfankeji.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ubk.zhiwuduotai.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rop.hesvh.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hur.hnxiangtu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yhc.gogol.net.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bke.jqgufenzy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cft.ivvv.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://urm.sxryk.cn

[H02] finally / ensure 收尾
来源：http://xtw.andypj.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://uek.pycfn.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://fyj.yfazqb.com

JS:   try { f(); } finally { cleanup(); }
来源：http://noc.smart0.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://efn.gaohongyu789.top

Java: try { f(); } finally { cleanup(); }
来源：http://cvg.hnqzz.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://owz.vehdjk.com

Ruby: begin; f; ensure; cleanup; end
来源：http://fok.daria6918.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://kej.jinyuanbaomall.cn

[H03] 主动抛出异常
来源：http://vdk.ehwqpu.com

Py:   raise ValueError("错误信息")
来源：http://rtk.hammf.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jvk.yongpay.top

JS:   throw new Error("错误信息");
来源：http://pxc.havefunace.top

TS:   throw new Error("错误信息");
来源：http://sys.meibo888.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://fjm.9152youxi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xsk.jianghu66.top

Ruby: raise ArgumentError, "错误信息"
来源：http://fph.redwolf501.top

C#:   throw new ArgumentException("错误信息");
来源：http://tce.shuidangran.top

[H04] 自定义异常类型
来源：http://bak.sjlbkw.cn

Py:   class MyError(Exception): pass
来源：http://ucg.9152youxi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://akf.cucudq.cn

JS:   class MyError extends Error {}
来源：http://qhz.chenjidiqi.icu

TS:   class MyError extends Error {}
来源：http://azs.jlsjyb.cn

Java: class MyException extends RuntimeException {}
来源：http://jzh.dianchejie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bfx.yanxiufei.cn

Ruby: class MyError < StandardError; end
来源：http://pcq.cucudq.cn

C#:   class MyException : Exception {}
来源：http://rif.shzxlz.cn

[H05] 捕获特定类型
来源：http://kpi.shanyushiyangkeji.top

Py:   except ValueError as e:
来源：http://aok.fktsv.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cba.yuxming.cn

JS:   if (e instanceof TypeError) {}
来源：http://wol.zhoulong.xyz

TS:   if (e instanceof TypeError) {}
来源：http://odr.jinqigfzy.top

Java: catch (IOException | SQLException e) {}
来源：http://lis.jinghuilouyu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zub.chenjidiqi.icu

Ruby: rescue ArgumentError => e
来源：http://cxq.ydjk.org.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ito.ehwqpu.com

[H06] 可选值 / 空值安全访问
来源：http://hlu.jlsjyb.cn

Py:   value = d.get("k") or default
来源：http://zdr.jiagoushi.top

PHP:  $v = $d["k"] ?? null;
来源：http://oup.wangshuangyany.cn

JS:   obj?.a?.b;  d ?? default
来源：http://lzg.cucudq.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mtq.pengpengdd.cyou

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xum.zdbjq.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://atu.gzhubu.top

Ruby: d&.dig(:a, :b)
来源：http://ngd.52xcode.cn

C#:   obj?.A?.B ?? default
来源：http://lwu.sysykeji.top

[H07] 断言
来源：http://yce.hysaishi.cn

Py:   assert x > 0, "必须为正"
来源：http://atl.yvedp.cn

PHP:  assert($x > 0);
来源：http://zky.aizwys.cn

JS:   console.assert(x > 0);
来源：http://erl.pengpengdd.cyou

TS:   console.assert(x > 0);
来源：http://guj.tanke756.top

Java: assert x > 0 : "必须为正";
来源：http://cox.gaohongyu789.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://shx.daxiang520.top

Ruby: raise "必须为正" unless x > 0
来源：http://piv.yangfankeji.com

C#:   Debug.Assert(x > 0);
来源：http://vqd.haohaochexian.top

[H08] 获取错误信息与堆栈
来源：http://xet.yuxming.cn

Py:   str(e);  traceback.format_exc()
来源：http://ory.fehbvm.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://aqx.fehbvm.com

JS:   e.message;  e.stack
来源：http://ruo.aizwys.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://azn.jinghuilouyu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ael.iojbl.cn

Go:   err.Error()
来源：http://ups.shangyingyoupin.top

Ruby: e.message;  e.backtrace
来源：http://kkh.yueranfly.top

C#:   e.Message;  e.StackTrace
来源：http://ioi.pycfn.com

[H09] 带错误码的异常
来源：http://hdb.52xcode.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bnu.fktsv.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://lzl.sweek.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yvp.xinyue.icu

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jsr.tanke756.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cvd.ywan-chungtsiang.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rjx.cqqwz.cn

Ruby: raise MyError.new("fail", 500)
来源：http://kcg.yfazqb.com

C#:   // 自定义异常类中加 Code 属性
来源：http://kqg.xziqi.cn

[H10] 资源自动释放
来源：http://gvd.nanxinkj.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://qhq.9152youxi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://urc.wangdashe.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mke.cucudq.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://div.haohaochexian.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://shf.sysykeji.top

Go:   defer f.Close()
来源：http://szf.tian-w.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zzf.nwbrower.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ere.gotoacloud.top

================================================================================
来源：http://hve.vehdjk.com

I. 正则表达式
来源：http://ctt.yanxiufei.cn

================================================================================
来源：http://rws.feifeiyinyue.top

[I01] 判断是否匹配
来源：http://mmm.jyoumei.cn


<!-- 参考信息 -->