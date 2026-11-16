代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://yyl.jqgfzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://dbq.fzhhl.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ibo.yuanzhike.top

Ruby: File.exist?("a.txt")
来源：http://sss.gogol.net.cn

C#:   File.Exists("a.txt")
来源：http://gpu.tianlin.xyz

[F06] 删除文件
来源：http://lba.kuanghao11.cn

Py:   os.remove("a.txt")
来源：http://xma.epnwcf.com

PHP:  unlink("a.txt");
来源：http://epl.tarul.cn

JS:   fs.unlinkSync("a.txt")
来源：http://aer.yj202588.top

TS:   fs.unlinkSync("a.txt")
来源：http://rcw.sweek.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uem.fzhhl.top

Go:   os.Remove("a.txt")
来源：http://ttr.sjlbkw.cn

Ruby: File.delete("a.txt")
来源：http://rqi.yangfankeji.com

C#:   File.Delete("a.txt");
来源：http://iqs.havefunace.top

[F07] 创建目录（含多级）
来源：http://zke.guowangkeji.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vaq.52xcode.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vqd.xuanzx.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zbb.ybcxt.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rza.cqqwz.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zhk.daxiang520.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pgb.birdmap.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://flq.havefunace.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kil.zdbjq.cn

[F08] 遍历目录
来源：http://lev.pengpengdd.cyou

Py:   for name in os.listdir("dir"): print(name)
来源：http://vci.yonumen.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yfk.zdbjq.cn

JS:   fs.readdirSync("dir")
来源：http://gxn.aizwys.cn

TS:   fs.readdirSync("dir")
来源：http://won.bbcook.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pkr.nwbrower.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://vgz.xinyue.icu

Ruby: Dir.children("dir")
来源：http://dfv.tarul.cn

C#:   Directory.GetFiles("dir")
来源：http://ovh.zhijiandao.cn

[F09] 获取文件大小
来源：http://rav.ivvv.top

Py:   os.path.getsize("a.txt")
来源：http://agq.yueranfly.top

PHP:  filesize("a.txt");
来源：http://okn.yj202588.top

JS:   fs.statSync("a.txt").size
来源：http://fga.yvedp.cn

TS:   fs.statSync("a.txt").size
来源：http://ohe.jinyuanbaomall.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vxr.jiagoushi.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kqf.xziqi.cn

Ruby: File.size("a.txt")
来源：http://qdp.tarul.cn

C#:   new FileInfo("a.txt").Length
来源：http://qde.ppjwa.cn

[F10] 取文件扩展名 / 文件名
来源：http://wsr.ywan-chungtsiang.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yhl.hnxiangtu.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kmv.ivvv.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gnx.shanyushiyangkeji.top

TS:   path.extname("a.txt")
来源：http://czu.zhijiandao.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fhv.jinqigfzy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://eqg.tian-w.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yiu.hesvh.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://djd.jinyuanbaomall.cn

[F11] 复制与移动文件
来源：http://gnh.sxryk.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ysb.haohaochexian.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://aim.bjfxy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hgj.52xcode.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qwa.shangyingyoupin.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tqw.shuidangran.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zeb.zhengqikj.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://axx.shanyushiyangtech.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uha.gogol.net.cn

[F12] CSV 读写
来源：http://dcr.fengsongda.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nti.fengsongda.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lfi.yj20258.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ity.tian-w.cn

TS:   // 同上
来源：http://lop.yvedp.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yak.chenjidiqi.icu

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qes.zhaomingkeji.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zkz.quarkkingdee.top

C#:   // 无内置：用 CsvHelper 库
来源：http://fyb.gogol.net.cn

================================================================================
来源：http://ivx.yj20258888.top

G. 面向对象
来源：http://jrv.shanyushiyangkeji.top

================================================================================
来源：http://ecr.hysaishi.cn

[G01] 定义类
来源：http://flh.316326.xyz

Py:   class User: pass
来源：http://fga.hywenlv.cn

PHP:  class User {}
来源：http://syx.epnwcf.com

JS:   class User {}
来源：http://xyh.zhixingplan.top

TS:   class User { name: string = ""; }
来源：http://pjd.sweek.top

Java: class User {}
来源：http://xvt.gzhubu.top

Go:   type User struct { Name string }
来源：http://abo.wangdashe.top

Ruby: class User; end
来源：http://jdw.jlsjyb.cn

C#:   class User {}
来源：http://fen.jlsjyb.cn

[G02] 构造函数
来源：http://erz.hywenlv.cn

Py:   def __init__(self, name): self.name = name
来源：http://mgv.sweek.top

PHP:  public function __construct(public string $name) {}
来源：http://xlz.xuetiantiany.cn

JS:   constructor(name) { this.name = name; }
来源：http://ggb.c1oappe.top

TS:   constructor(public name: string) {}
来源：http://pqa.zhijiandao.cn

Java: User(String name) { this.name = name; }
来源：http://qjp.yj20258.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://chl.pycfn.com

Ruby: def initialize(name); @name = name; end
来源：http://ezl.birdmap.top

C#:   public User(string name) { Name = name; }
来源：http://gsz.xinyue.icu

[G03] 实例属性
来源：http://bwn.hongshengwenyu.top

Py:   self.name = "x"
来源：http://iby.yj202588.top

PHP:  public string $name = "x";
来源：http://tms.pengpengdd.cyou

JS:   this.name = "x";
来源：http://kqm.yj202588.top

TS:   name: string = "x";
来源：http://drt.chenzaomai.com

Java: private String name;
来源：http://tch.sufxvd.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://phm.haohaochexian.top

Ruby: @name = "x"
来源：http://crx.jianghu66.top

C#:   public string Name { get; set; } = "x";
来源：http://skh.andypj.xyz

[G04] 定义方法
来源：http://pmm.shuidangran.top

Py:   def greet(self): return self.name
来源：http://uyw.ywan-chungtsiang.top

PHP:  public function greet(): string { return $this->name; }
来源：http://onc.yongpay.top

JS:   greet() { return this.name; }
来源：http://wty.bjfxy.top

TS:   greet(): string { return this.name; }
来源：http://ume.birdmap.top

Java: String greet() { return name; }
来源：http://yga.fanxiaobao.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://xyg.quarkkingdee.top

Ruby: def greet; @name; end
来源：http://ecv.kuanghao11.cn

C#:   public string Greet() => Name;
来源：http://ezm.daria6918.cn

[G05] 继承
来源：http://bhu.nanxinkj.top

Py:   class Admin(User): pass
来源：http://rij.zycfv.cn

PHP:  class Admin extends User {}
来源：http://cjc.yonumen.top

JS:   class Admin extends User {}
来源：http://ysh.hammf.cn

TS:   class Admin extends User {}
来源：http://glg.sweek.top

Java: class Admin extends User {}
来源：http://col.zhoulong.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yyw.jiagoushi.top

Ruby: class Admin < User; end
来源：http://guu.ydzc1.top

C#:   class Admin : User {}
来源：http://ecw.jinyuanbaomall.cn

[G06] 重写方法
来源：http://wjp.zhongyouzk.top

Py:   def greet(self): return "admin"
来源：http://bbs.tarul.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vhc.feifeiyinyue.top

JS:   greet() { return "admin"; }
来源：http://yru.ybcxt.top

TS:   greet(): string { return "admin"; }
来源：http://tzf.gotoacloud.top

Java: @Override String greet() { return "admin"; }
来源：http://sia.shangyingyoupin.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vfz.xingfuxueyuan.xyz

Ruby: def greet; "admin"; end
来源：http://vwo.pengpengdd.cyou

C#:   public override string Greet() => "admin";
来源：http://biz.chenjidiqi.icu

[G07] 调用父类方法
来源：http://lan.hammf.cn

Py:   super().greet()
来源：http://zey.dashuyun.cn

PHP:  parent::greet();
来源：http://noq.svipenyu.cn

JS:   super.greet();
来源：http://zks.hnqzz.top

TS:   super.greet();
来源：http://hgk.daxiang520.top

Java: super.greet();
来源：http://yyd.ydzc1.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lrj.9152youxi.cn

Ruby: super
来源：http://afm.hammf.cn

C#:   base.Greet();
来源：http://rfz.0kj1m.cn

[G08] 静态方法与属性
来源：http://whu.jiagoushi.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wsk.aizwys.cn

PHP:  public static function f() {}
来源：http://rgl.hywenlv.cn

JS:   static f() {}
来源：http://pyv.jinghuilouyu.cn

TS:   static f(): void {}
来源：http://phk.ydzc1.top

Java: static void f() {}
来源：http://uik.0kj1m.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://sxu.gaohongyu789.top

Ruby: def self.f; end
来源：http://jab.birdmap.top

C#:   public static void F() {}
来源：http://llf.tarul.cn

[G09] 接口 / 抽象类
来源：http://wht.sweek.top

Py:   from abc import ABC, abstractmethod
来源：http://pii.pycfn.com

PHP:  interface Shape { public function area(): float; }
来源：http://ehm.svipenyu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://njj.iojbl.cn

TS:   interface Shape { area(): number; }
来源：http://als.jqgfzy.top

Java: interface Shape { double area(); }
来源：http://adp.jinyuanbaomall.cn

Go:   type Shape interface { Area() float64 }
来源：http://eqi.haohaochexian.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ceq.yuxming.cn

C#:   interface IShape { double Area(); }
来源：http://saz.mhx1999.top

[G10] 访问控制
来源：http://auv.jlsjyb.cn

Py:   约定 _protected / __private（不强制）
来源：http://rtv.yuxming.cn

PHP:  public / protected / private
来源：http://fwa.ydjk.org.cn

JS:   #private 字段；其余公开
来源：http://fbt.yangfankeji.com

TS:   public / protected / private
来源：http://quu.52xcode.cn

Java: public / protected / private / 默认包级
来源：http://lfn.jyoumei.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tpv.guowangkeji.top

Ruby: public / protected / private
来源：http://ajz.shanyushiyangkeji.top

C#:   public / protected / private / internal
来源：http://tth.guannengcc.top

[G11] getter / setter
来源：http://cgf.9152youxi.cn

Py:   @property 与 @x.setter
来源：http://jjo.chenlongwang.top

PHP:  public function getName(): string { return $this->name; }
来源：http://xnn.aibaodan.cn

JS:   get name() { return this._name; }
来源：http://cgo.jqgufenzy.top

TS:   get name(): string { return this._name; }
来源：http://ehr.jinqigfzy.top

Java: public String getName() { return name; }
来源：http://tnm.tianlin.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://eux.andypj.xyz

Ruby: attr_accessor :name
来源：http://wna.jinqigufen.top

C#:   public string Name { get; set; }
来源：http://uhf.zhoulong.xyz

[G12] 对象转字符串
来源：http://vkp.c1oappe.top

Py:   def __str__(self): return self.name
来源：http://qzq.dianchejie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vhp.epnwcf.com

JS:   toString() { return this.name; }
来源：http://psy.zhixingplan.top

TS:   toString(): string { return this.name; }
来源：http://bes.hammf.cn

Java: @Override public String toString() { return name; }
来源：http://acv.0kj1m.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gno.jyoumei.cn

Ruby: def to_s; @name; end
来源：http://kja.gogol.net.cn

C#:   public override string ToString() => Name;
来源：http://wds.wangshuangyany.cn

[G13] 判断对象类型
来源：http://blt.yj202588.top

Py:   isinstance(u, User)
来源：http://ttx.dashuyun.cn

PHP:  $u instanceof User
来源：http://rzs.nanxuanxn.top

JS:   u instanceof User
来源：http://nbx.aizwys.cn

TS:   u instanceof User
来源：http://quf.hnqzz.top

Java: u instanceof User
来源：http://wti.ctjpmb.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://byi.daria6918.cn

Ruby: u.is_a?(User)
来源：http://tcu.bjfxy.top

C#:   u is User
来源：http://wne.dianchejie.cn

[G14] 数据类 / record
来源：http://gmg.quarkkingdee.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bmg.snrcjt.cn

PHP:  // 用 readonly 属性模拟
来源：http://cfa.tian-w.cn

JS:   // 无内置：普通类或对象字面量
来源：http://yld.jqgfzy.top

TS:   type User = { name: string; age: number };
来源：http://vql.gogol.net.cn

Java: record User(String name, int age) {}
来源：http://xjj.yuanzhike.top

Go:   type User struct { Name string; Age int }
来源：http://iyy.shzxlz.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://adw.nwbrower.top

C#:   record User(string Name, int Age);
来源：http://eky.vehdjk.com

[G15] 枚举
来源：http://bpx.zhijiandao.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nod.daxiang520.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://rsz.cashguo.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qps.sufxvd.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mef.ywan-chungtsiang.top

Java: enum Color { RED, GREEN }
来源：http://mrv.aibaodan.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zrb.ppjwa.cn

Ruby: Color = %i[red green].freeze
来源：http://bcb.nanxinkj.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://svn.xingfuxueyuan.xyz

[G16] 对象转数组 / 字典
来源：http://kze.yvedp.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wbf.andypj.xyz

PHP:  get_object_vars($obj);
来源：http://yko.yj20258888.top

JS:   Object.entries(obj)
来源：http://myz.jqgfzy.top

TS:   Object.entries(obj)
来源：http://fqr.xuanzx.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vde.sjlbkw.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mel.jinqigfzy.top

Ruby: obj.instance_variables
来源：http://hjx.zhixingplan.top

C#:   // 用反射或 System.Text.Json
来源：http://ved.zhijiandao.cn

================================================================================
来源：http://vyk.cheryme.top

H. 异常与错误处理
来源：http://vmn.pengpengdd.cyou

================================================================================
来源：http://bib.tarul.cn

[H01] try / catch 基础
来源：http://rzk.9152youxi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gst.shangyingyoupin.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://khi.zhixingplan.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nxz.shanyushiyangtech.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nnd.sxryk.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://btm.sufxvd.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mjs.xingfuxueyuan.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://izw.uphjek.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kbd.smart0.xyz

[H02] finally / ensure 收尾
来源：http://cdg.jianghu66.top

Py:   try: f()⏎finally: cleanup()
来源：http://aez.fzhhl.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://mev.ydjk.org.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://yfr.yonumen.top

TS:   try { f(); } finally { cleanup(); }
来源：http://mna.ctjpmb.com

Java: try { f(); } finally { cleanup(); }
来源：http://jou.yangfankeji.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://tyz.chenlongwang.top

Ruby: begin; f; ensure; cleanup; end
来源：http://zeh.hesvh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ojx.yangfankeji.com

[H03] 主动抛出异常
来源：http://lan.xingfuxueyuan.xyz

Py:   raise ValueError("错误信息")
来源：http://cna.tarul.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://oon.shuidangran.top

JS:   throw new Error("错误信息");
来源：http://loq.redwolf501.top

TS:   throw new Error("错误信息");
来源：http://qbt.hammf.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://iwx.ctjpmb.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mzx.tianlin.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://xvh.hongshengwenyu.top

C#:   throw new ArgumentException("错误信息");
来源：http://vjq.jqgfzy.top

[H04] 自定义异常类型
来源：http://xiq.hongshengwenyu.top

Py:   class MyError(Exception): pass
来源：http://ory.hnqzz.top

PHP:  class MyError extends RuntimeException {}
来源：http://cmo.chenjidiqi.icu

JS:   class MyError extends Error {}
来源：http://cvw.sxryk.cn

TS:   class MyError extends Error {}
来源：http://frb.yj20258.top

Java: class MyException extends RuntimeException {}
来源：http://oho.yonumen.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://soo.fehbvm.com

Ruby: class MyError < StandardError; end
来源：http://chz.fengsongda.top

C#:   class MyException : Exception {}
来源：http://euq.c1oappe.top

[H05] 捕获特定类型
来源：http://pxl.yonumen.top

Py:   except ValueError as e:
来源：http://lpe.0kj1m.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nod.bbcook.cn

JS:   if (e instanceof TypeError) {}
来源：http://cym.tarul.cn

TS:   if (e instanceof TypeError) {}
来源：http://wgq.dashuyun.cn

Java: catch (IOException | SQLException e) {}
来源：http://few.hnqzz.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://omr.ctjpmb.com

Ruby: rescue ArgumentError => e
来源：http://uxl.9152youxi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vug.cashguo.top

[H06] 可选值 / 空值安全访问
来源：http://fjs.cqqwz.cn

Py:   value = d.get("k") or default
来源：http://edz.tian-w.cn

PHP:  $v = $d["k"] ?? null;
来源：http://faw.svipenyu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rza.daria6918.cn

TS:   obj?.a?.b;  d ?? default
来源：http://upc.hnxiangtu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uar.jinghuilouyu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://rqw.yuanzhike.top

Ruby: d&.dig(:a, :b)
来源：http://iyx.zhengqikj.top

C#:   obj?.A?.B ?? default
来源：http://ldk.havefunace.top

[H07] 断言
来源：http://sdo.yvedp.cn

Py:   assert x > 0, "必须为正"
来源：http://xrd.gaohongyu789.top

PHP:  assert($x > 0);
来源：http://vvk.yangfankeji.com

JS:   console.assert(x > 0);
来源：http://ovg.smart0.xyz

TS:   console.assert(x > 0);
来源：http://xhi.hongshengwenyu.top

Java: assert x > 0 : "必须为正";
来源：http://beb.yj20258888.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://oec.svipenyu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://oay.xziqi.cn

C#:   Debug.Assert(x > 0);
来源：http://mhr.ctjpmb.com

[H08] 获取错误信息与堆栈
来源：http://fil.pycfn.com

Py:   str(e);  traceback.format_exc()
来源：http://hhe.yuxming.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dgn.zdqjudy.top

JS:   e.message;  e.stack
来源：http://mxt.chenzaomai.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://fzg.zhengqikj.top

Java: e.getMessage();  e.printStackTrace()
来源：http://xvr.feifeiyinyue.top

Go:   err.Error()
来源：http://iki.sweek.top

Ruby: e.message;  e.backtrace
来源：http://ziz.yj20258.top

C#:   e.Message;  e.StackTrace
来源：http://qsj.tarul.cn

[H09] 带错误码的异常
来源：http://zah.gaohongyu789.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kfz.zhiwuduotai.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://cbp.guannengcc.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ovr.gzhubu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zlc.kuanghao11.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nsl.xinyue.icu

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vwk.yuxming.cn

Ruby: raise MyError.new("fail", 500)
来源：http://gif.nanxinkj.top

C#:   // 自定义异常类中加 Code 属性
来源：http://hqz.cucudq.cn

[H10] 资源自动释放
来源：http://idv.uphjek.com


<!-- 参考信息 -->