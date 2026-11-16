代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zcl.jlsjyb.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jpc.smart0.xyz

[F11] 复制与移动文件
来源：http://nqp.chenjidiqi.icu

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://iuc.ydzc1.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jvd.jinqigfzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hkf.aibaodan.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hzl.chenjidiqi.icu

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lfu.zycfv.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bbp.tarul.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ath.uphjek.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hof.dianchejie.cn

[F12] CSV 读写
来源：http://ksr.yj202588.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dbb.hnxiangtu.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xaq.chenzaomai.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hez.svipenyu.cn

TS:   // 同上
来源：http://vge.zhijiandao.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rls.yuanzhike.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jio.gotoacloud.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lsa.hammf.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://eum.cqqwz.cn

================================================================================
来源：http://opa.daria6918.cn

G. 面向对象
来源：http://qny.tianlin.xyz

================================================================================
来源：http://wwy.snrcjt.cn

[G01] 定义类
来源：http://iee.jinyuanbaomall.cn

Py:   class User: pass
来源：http://rgn.feifeiyinyue.top

PHP:  class User {}
来源：http://yeb.hfpthk.cn

JS:   class User {}
来源：http://lqw.chenjidiqi.icu

TS:   class User { name: string = ""; }
来源：http://ned.jiagoushi.top

Java: class User {}
来源：http://qmn.xinyue.icu

Go:   type User struct { Name string }
来源：http://euo.dashuyun.cn

Ruby: class User; end
来源：http://dur.hysaishi.cn

C#:   class User {}
来源：http://scz.chenzaomai.com

[G02] 构造函数
来源：http://abv.gotoacloud.top

Py:   def __init__(self, name): self.name = name
来源：http://fgj.smart0.xyz

PHP:  public function __construct(public string $name) {}
来源：http://abb.daria6918.cn

JS:   constructor(name) { this.name = name; }
来源：http://ffr.hesvh.cn

TS:   constructor(public name: string) {}
来源：http://qsg.sufxvd.cn

Java: User(String name) { this.name = name; }
来源：http://svn.fzhhl.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dlk.epnwcf.com

Ruby: def initialize(name); @name = name; end
来源：http://jip.cdnleiting.top

C#:   public User(string name) { Name = name; }
来源：http://nhp.yj202588.top

[G03] 实例属性
来源：http://qze.bbcook.cn

Py:   self.name = "x"
来源：http://hac.ywan-chungtsiang.top

PHP:  public string $name = "x";
来源：http://npv.tarul.cn

JS:   this.name = "x";
来源：http://srl.yj20258888.top

TS:   name: string = "x";
来源：http://xpy.feifeiyinyue.top

Java: private String name;
来源：http://ryn.sysykeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ljo.jqgufenzy.top

Ruby: @name = "x"
来源：http://gpy.0kj1m.cn

C#:   public string Name { get; set; } = "x";
来源：http://wsr.cheryme.top

[G04] 定义方法
来源：http://gmk.gzhubu.top

Py:   def greet(self): return self.name
来源：http://rch.xuanzx.com

PHP:  public function greet(): string { return $this->name; }
来源：http://bnp.fehbvm.com

JS:   greet() { return this.name; }
来源：http://gbu.uphjek.com

TS:   greet(): string { return this.name; }
来源：http://uca.tian-w.cn

Java: String greet() { return name; }
来源：http://fkm.sweek.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://gmq.tarul.cn

Ruby: def greet; @name; end
来源：http://ejm.aibaodan.cn

C#:   public string Greet() => Name;
来源：http://lbg.sweek.top

[G05] 继承
来源：http://oam.iojbl.cn

Py:   class Admin(User): pass
来源：http://gbf.shangyingyoupin.top

PHP:  class Admin extends User {}
来源：http://xji.shzxlz.cn

JS:   class Admin extends User {}
来源：http://sfx.yangfankeji.com

TS:   class Admin extends User {}
来源：http://oth.nanxinkj.top

Java: class Admin extends User {}
来源：http://znx.ppjwa.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bdg.feifeiyinyue.top

Ruby: class Admin < User; end
来源：http://xcw.jiagoushi.top

C#:   class Admin : User {}
来源：http://edt.nanxinkj.top

[G06] 重写方法
来源：http://itk.gotoacloud.top

Py:   def greet(self): return "admin"
来源：http://cmv.haohaochexian.top

PHP:  public function greet(): string { return "admin"; }
来源：http://sfj.cqqwz.cn

JS:   greet() { return "admin"; }
来源：http://ncl.hysaishi.cn

TS:   greet(): string { return "admin"; }
来源：http://ghf.zdbjq.cn

Java: @Override String greet() { return "admin"; }
来源：http://hyk.iojbl.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://swr.hnqzz.top

Ruby: def greet; "admin"; end
来源：http://alu.ydzc1.top

C#:   public override string Greet() => "admin";
来源：http://wer.ppjwa.cn

[G07] 调用父类方法
来源：http://idr.shzxlz.cn

Py:   super().greet()
来源：http://shg.xylfe.cn

PHP:  parent::greet();
来源：http://gai.jqgfzy.top

JS:   super.greet();
来源：http://xbw.hnqzz.top

TS:   super.greet();
来源：http://tks.ppjwa.cn

Java: super.greet();
来源：http://euu.jiagoushi.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xid.jianghu66.top

Ruby: super
来源：http://pvu.vehdjk.com

C#:   base.Greet();
来源：http://bzx.dashuyun.cn

[G08] 静态方法与属性
来源：http://csj.daxiang520.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hnf.vehdjk.com

PHP:  public static function f() {}
来源：http://cog.iojbl.cn

JS:   static f() {}
来源：http://wuj.sweek.top

TS:   static f(): void {}
来源：http://vpz.ydzc1.top

Java: static void f() {}
来源：http://ixg.zhongyouzk.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://vzz.redwolf501.top

Ruby: def self.f; end
来源：http://wsb.shanyushiyangkeji.top

C#:   public static void F() {}
来源：http://xrw.vqdsnc.cn

[G09] 接口 / 抽象类
来源：http://bsl.xziqi.cn

Py:   from abc import ABC, abstractmethod
来源：http://cgs.zycfv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qsg.jinghuilouyu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://lit.chenjidiqi.icu

TS:   interface Shape { area(): number; }
来源：http://qaz.zdbjq.cn

Java: interface Shape { double area(); }
来源：http://aou.feifeiyinyue.top

Go:   type Shape interface { Area() float64 }
来源：http://tkr.cheryme.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gid.hfpthk.cn

C#:   interface IShape { double Area(); }
来源：http://vdu.hesvh.cn

[G10] 访问控制
来源：http://eqy.fanxiaobao.xyz

Py:   约定 _protected / __private（不强制）
来源：http://sjx.fengsongda.top

PHP:  public / protected / private
来源：http://jeb.cdnleiting.top

JS:   #private 字段；其余公开
来源：http://bpo.aibaodan.cn

TS:   public / protected / private
来源：http://lci.jinqigufen.top

Java: public / protected / private / 默认包级
来源：http://iju.yj20258.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://yma.yvedp.cn

Ruby: public / protected / private
来源：http://epc.xuanzx.com

C#:   public / protected / private / internal
来源：http://wcr.cheryme.top

[G11] getter / setter
来源：http://ybr.zhiwuduotai.top

Py:   @property 与 @x.setter
来源：http://qdp.sxryk.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://eef.jinghuilouyu.cn

JS:   get name() { return this._name; }
来源：http://uhz.yj202588.top

TS:   get name(): string { return this._name; }
来源：http://czp.ppjwa.cn

Java: public String getName() { return name; }
来源：http://ksm.mhx1999.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://vhz.aizwys.cn

Ruby: attr_accessor :name
来源：http://lyd.feifeiyinyue.top

C#:   public string Name { get; set; }
来源：http://dhx.gaohongyu789.top

[G12] 对象转字符串
来源：http://imr.pycfn.com

Py:   def __str__(self): return self.name
来源：http://oqk.ydzc1.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://fhj.ppjwa.cn

JS:   toString() { return this.name; }
来源：http://bnq.316326.xyz

TS:   toString(): string { return this.name; }
来源：http://wzu.feifeiyinyue.top

Java: @Override public String toString() { return name; }
来源：http://bms.mhx1999.top

Go:   func (u User) String() string { return u.Name }
来源：http://iqv.gotoacloud.top

Ruby: def to_s; @name; end
来源：http://gec.yueranfly.top

C#:   public override string ToString() => Name;
来源：http://vgg.jinqigufen.top

[G13] 判断对象类型
来源：http://cjr.ydzc1.top

Py:   isinstance(u, User)
来源：http://acw.jyoumei.cn

PHP:  $u instanceof User
来源：http://ihx.kuanghao11.cn

JS:   u instanceof User
来源：http://dow.jiagoushi.top

TS:   u instanceof User
来源：http://xii.52xcode.cn

Java: u instanceof User
来源：http://opd.smart0.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://tqv.gotoacloud.top

Ruby: u.is_a?(User)
来源：http://hxt.cdnleiting.top

C#:   u is User
来源：http://wvb.zhiwuduotai.top

[G14] 数据类 / record
来源：http://ucd.zycfv.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uwj.zycfv.cn

PHP:  // 用 readonly 属性模拟
来源：http://jmb.hfpthk.cn

JS:   // 无内置：普通类或对象字面量
来源：http://pwl.dianchejie.cn

TS:   type User = { name: string; age: number };
来源：http://lfb.jinghuilouyu.cn

Java: record User(String name, int age) {}
来源：http://xnz.ywan-chungtsiang.top

Go:   type User struct { Name string; Age int }
来源：http://vgi.zdqjudy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xos.zhongyouzk.top

C#:   record User(string Name, int Age);
来源：http://fzz.yonumen.top

[G15] 枚举
来源：http://tyh.andypj.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hzd.cheryme.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ldl.zdqjudy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://twm.cdnleiting.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ear.9152youxi.cn

Java: enum Color { RED, GREEN }
来源：http://ccy.svipenyu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://njk.yanxiufei.cn

Ruby: Color = %i[red green].freeze
来源：http://bpy.sweek.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://epy.bbcook.cn

[G16] 对象转数组 / 字典
来源：http://bad.jinqigfzy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://igv.guannengcc.top

PHP:  get_object_vars($obj);
来源：http://xju.fanxiaobao.xyz

JS:   Object.entries(obj)
来源：http://uat.chenzaomai.com

TS:   Object.entries(obj)
来源：http://jef.jinghuilouyu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ouv.haohaochexian.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://hrv.tanke756.top

Ruby: obj.instance_variables
来源：http://dgr.zhaomingkeji.xyz

C#:   // 用反射或 System.Text.Json
来源：http://szv.bjfxy.top

================================================================================
来源：http://fzm.jinqigufen.top

H. 异常与错误处理
来源：http://hbp.fanxiaobao.xyz

================================================================================
来源：http://ohy.xylfe.cn

[H01] try / catch 基础
来源：http://cfg.fehbvm.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qqo.jyoumei.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yya.c1oappe.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bsa.dianchejie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ygv.sweek.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vma.zhixingplan.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://roq.snrcjt.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bdr.tian-w.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nux.tianlin.xyz

[H02] finally / ensure 收尾
来源：http://lcd.daria6918.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ynn.tianlin.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://oli.redwolf501.top

JS:   try { f(); } finally { cleanup(); }
来源：http://bhu.hfpthk.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://woi.yj202588.top

Java: try { f(); } finally { cleanup(); }
来源：http://ihz.quarkkingdee.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://yad.zhengqikj.top

Ruby: begin; f; ensure; cleanup; end
来源：http://odq.guannengcc.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://txq.yj20258888.top

[H03] 主动抛出异常
来源：http://kcw.snrcjt.cn

Py:   raise ValueError("错误信息")
来源：http://vru.cqqwz.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wxu.hnqzz.top

JS:   throw new Error("错误信息");
来源：http://atu.xziqi.cn

TS:   throw new Error("错误信息");
来源：http://gbd.snrcjt.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jop.daria6918.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wni.zhaomingkeji.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://rrt.birdmap.top

C#:   throw new ArgumentException("错误信息");
来源：http://sib.quarkkingdee.top

[H04] 自定义异常类型
来源：http://vyd.zhaomingkeji.xyz

Py:   class MyError(Exception): pass
来源：http://zjy.yanxiufei.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dil.zhoulong.xyz

JS:   class MyError extends Error {}
来源：http://sdj.zhaomingkeji.xyz

TS:   class MyError extends Error {}
来源：http://uwn.jqgufenzy.top

Java: class MyException extends RuntimeException {}
来源：http://bvs.chenzaomai.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cpv.xuetiantiany.cn

Ruby: class MyError < StandardError; end
来源：http://gvl.hfpthk.cn

C#:   class MyException : Exception {}
来源：http://kce.hcnkem.com

[H05] 捕获特定类型
来源：http://xsi.ehwqpu.com

Py:   except ValueError as e:
来源：http://dwd.nwbrower.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jei.ywan-chungtsiang.top

JS:   if (e instanceof TypeError) {}
来源：http://qgp.fengsongda.top

TS:   if (e instanceof TypeError) {}
来源：http://kzy.fehbvm.com

Java: catch (IOException | SQLException e) {}
来源：http://csu.xingfuxueyuan.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dgb.cqqwz.cn

Ruby: rescue ArgumentError => e
来源：http://tyg.jlsjyb.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yzy.0kj1m.cn

[H06] 可选值 / 空值安全访问
来源：http://ncp.bbcook.cn

Py:   value = d.get("k") or default
来源：http://sjs.chenzaomai.com

PHP:  $v = $d["k"] ?? null;
来源：http://bto.xziqi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://prr.hfpthk.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vez.fktsv.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ard.0kj1m.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://mxm.hywenlv.cn

Ruby: d&.dig(:a, :b)
来源：http://oek.fehbvm.com

C#:   obj?.A?.B ?? default
来源：http://pch.meibo888.top

[H07] 断言
来源：http://trg.daria6918.cn

Py:   assert x > 0, "必须为正"
来源：http://ymv.yfazqb.com

PHP:  assert($x > 0);
来源：http://dxe.hywenlv.cn

JS:   console.assert(x > 0);
来源：http://ezr.daria6918.cn

TS:   console.assert(x > 0);
来源：http://chr.yonumen.top

Java: assert x > 0 : "必须为正";
来源：http://qlg.chenzaomai.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://egr.gaohongyu789.top

Ruby: raise "必须为正" unless x > 0
来源：http://fnv.sufxvd.cn

C#:   Debug.Assert(x > 0);
来源：http://jdf.ppjwa.cn

[H08] 获取错误信息与堆栈
来源：http://qdv.shanyushiyangkeji.top

Py:   str(e);  traceback.format_exc()
来源：http://lgz.yongpay.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hyc.ppjwa.cn

JS:   e.message;  e.stack
来源：http://asl.fehbvm.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://ibd.zhengqikj.top

Java: e.getMessage();  e.printStackTrace()
来源：http://gak.hesvh.cn

Go:   err.Error()
来源：http://qff.chenlongwang.top

Ruby: e.message;  e.backtrace
来源：http://yjr.tanke756.top

C#:   e.Message;  e.StackTrace
来源：http://swt.tanke756.top

[H09] 带错误码的异常
来源：http://dfb.zhoulong.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gvc.xziqi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://teb.shanyushiyangtech.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gbx.shzxlz.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vqk.zhijiandao.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tyt.gogol.net.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ydr.andypj.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://ptx.shangyingyoupin.top

C#:   // 自定义异常类中加 Code 属性
来源：http://lmp.sxryk.cn

[H10] 资源自动释放
来源：http://ogl.wangdashe.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://htp.svipenyu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jik.yj202588.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hbm.fehbvm.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ppa.hywenlv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hir.mhx1999.top

Go:   defer f.Close()
来源：http://iyk.c1oappe.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://buq.hammf.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xtt.ivvv.top

================================================================================
来源：http://nzs.zhongyouzk.top

I. 正则表达式
来源：http://ago.wangshuangyany.cn

================================================================================
来源：http://vtc.yuanzhike.top

[I01] 判断是否匹配
来源：http://zkr.ydjk.org.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zgr.fktsv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://uft.birdmap.top

JS:   /\d+/.test(s)
来源：http://kvn.cucudq.cn

TS:   /\d+/.test(s)
来源：http://aad.daria6918.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://crw.pengpengdd.cyou

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://owe.jianghu66.top

Ruby: s.match?(/\d+/)
来源：http://bri.smart0.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ovi.tarul.cn

[I02] 提取所有匹配
来源：http://fhw.pycfn.com

Py:   re.findall(r"\d+", s)
来源：http://ebb.jqgufenzy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xkx.jyoumei.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://toz.chenjidiqi.icu

TS:   s.match(/\d+/g)
来源：http://kir.yvedp.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ggt.redwolf501.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rcf.quarkkingdee.top

Ruby: s.scan(/\d+/)
来源：http://khy.jyoumei.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uom.redwolf501.top

[I03] 提取捕获分组
来源：http://ccf.yfazqb.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tsl.cheryme.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zga.guannengcc.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zri.andypj.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wiy.daxiang520.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://byx.fengsongda.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bjh.xingfuxueyuan.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://epd.quarkkingdee.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rdu.aizwys.cn

[I04] 正则替换
来源：http://gdx.zhixingplan.top

Py:   re.sub(r"\d+", "#", s)
来源：http://jwe.yuxming.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jha.pycfn.com

JS:   s.replace(/\d+/g, "#")
来源：http://ptp.bbcook.cn

TS:   s.replace(/\d+/g, "#")
来源：http://dly.sjlbkw.cn

Java: s.replaceAll("\\d+", "#")
来源：http://oxk.ivvv.top

Go:   re.ReplaceAllString(s, "#")
来源：http://quw.xingfuxueyuan.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://tlt.jinqigfzy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gtn.ydjk.org.cn

[I05] 按正则拆分
来源：http://gks.jinqigufen.top


<!-- 参考信息 -->