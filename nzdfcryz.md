代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ygs.cheryme.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hrk.zdqjudy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://knp.bjfxy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sfk.pengpengdd.cyou

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ene.jinqigufen.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xsv.sxryk.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bro.jlsjyb.cn

[F12] CSV 读写
来源：http://mac.cucudq.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vab.bjfxy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ioq.nanxuanxn.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://spr.hongshengwenyu.top

TS:   // 同上
来源：http://ehd.ehwqpu.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fcm.xingfuxueyuan.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kwe.yueranfly.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tis.nanxinkj.top

C#:   // 无内置：用 CsvHelper 库
来源：http://vlw.yj20258888.top

================================================================================
来源：http://nsq.yuxming.cn

G. 面向对象
来源：http://hrh.yuanzhike.top

================================================================================
来源：http://mph.yvedp.cn

[G01] 定义类
来源：http://zkt.xylfe.cn

Py:   class User: pass
来源：http://ufv.dianchejie.cn

PHP:  class User {}
来源：http://xrc.quarkkingdee.top

JS:   class User {}
来源：http://ila.yj20258888.top

TS:   class User { name: string = ""; }
来源：http://cdx.nanxinkj.top

Java: class User {}
来源：http://ljo.hnqzz.top

Go:   type User struct { Name string }
来源：http://rsn.shangyingyoupin.top

Ruby: class User; end
来源：http://uvm.nanxuanxn.top

C#:   class User {}
来源：http://gxm.gaohongyu789.top

[G02] 构造函数
来源：http://rya.sxryk.cn

Py:   def __init__(self, name): self.name = name
来源：http://gqw.quarkkingdee.top

PHP:  public function __construct(public string $name) {}
来源：http://pep.vehdjk.com

JS:   constructor(name) { this.name = name; }
来源：http://glm.chenlongwang.top

TS:   constructor(public name: string) {}
来源：http://xci.hnxiangtu.top

Java: User(String name) { this.name = name; }
来源：http://jra.epnwcf.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ych.fengsongda.top

Ruby: def initialize(name); @name = name; end
来源：http://vow.meibo888.top

C#:   public User(string name) { Name = name; }
来源：http://gwl.52xcode.cn

[G03] 实例属性
来源：http://gjd.shzxlz.cn

Py:   self.name = "x"
来源：http://kkj.hcnkem.com

PHP:  public string $name = "x";
来源：http://ucg.cheryme.top

JS:   this.name = "x";
来源：http://hnp.ehwqpu.com

TS:   name: string = "x";
来源：http://xxb.hysaishi.cn

Java: private String name;
来源：http://nqo.chenzaomai.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fwq.ydjk.org.cn

Ruby: @name = "x"
来源：http://lvs.tian-w.cn

C#:   public string Name { get; set; } = "x";
来源：http://nko.birdmap.top

[G04] 定义方法
来源：http://bho.yfazqb.com

Py:   def greet(self): return self.name
来源：http://ssx.iojbl.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://lpo.xuanzx.com

JS:   greet() { return this.name; }
来源：http://jvs.0kj1m.cn

TS:   greet(): string { return this.name; }
来源：http://teh.bjfxy.top

Java: String greet() { return name; }
来源：http://qus.ywan-chungtsiang.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://qte.ywan-chungtsiang.top

Ruby: def greet; @name; end
来源：http://job.mhx1999.top

C#:   public string Greet() => Name;
来源：http://vol.shangyingyoupin.top

[G05] 继承
来源：http://moz.iojbl.cn

Py:   class Admin(User): pass
来源：http://ozp.sufxvd.cn

PHP:  class Admin extends User {}
来源：http://kjp.ppjwa.cn

JS:   class Admin extends User {}
来源：http://vws.birdmap.top

TS:   class Admin extends User {}
来源：http://fwc.quarkkingdee.top

Java: class Admin extends User {}
来源：http://udb.hywenlv.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ggy.hysaishi.cn

Ruby: class Admin < User; end
来源：http://huz.jqgfzy.top

C#:   class Admin : User {}
来源：http://hlh.ppjwa.cn

[G06] 重写方法
来源：http://agc.jiagoushi.top

Py:   def greet(self): return "admin"
来源：http://ejl.bbcook.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zez.uphjek.com

JS:   greet() { return "admin"; }
来源：http://qeg.tianlin.xyz

TS:   greet(): string { return "admin"; }
来源：http://dhq.zdbjq.cn

Java: @Override String greet() { return "admin"; }
来源：http://xfr.feifeiyinyue.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tyz.zhoulong.xyz

Ruby: def greet; "admin"; end
来源：http://zqz.aibaodan.cn

C#:   public override string Greet() => "admin";
来源：http://isd.tianlin.xyz

[G07] 调用父类方法
来源：http://dan.yongpay.top

Py:   super().greet()
来源：http://fvf.iojbl.cn

PHP:  parent::greet();
来源：http://wzf.wangshuangyany.cn

JS:   super.greet();
来源：http://wvd.vqdsnc.cn

TS:   super.greet();
来源：http://qny.xinyue.icu

Java: super.greet();
来源：http://xul.ehwqpu.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bvk.wangshuangyany.cn

Ruby: super
来源：http://ijy.dianchejie.cn

C#:   base.Greet();
来源：http://rym.jyoumei.cn

[G08] 静态方法与属性
来源：http://fqn.nanxuanxn.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://can.aibaodan.cn

PHP:  public static function f() {}
来源：http://unj.ppjwa.cn

JS:   static f() {}
来源：http://bfo.cashguo.top

TS:   static f(): void {}
来源：http://gss.zhijiandao.cn

Java: static void f() {}
来源：http://bqc.sufxvd.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://wqg.zhixingplan.top

Ruby: def self.f; end
来源：http://sut.xingfuxueyuan.xyz

C#:   public static void F() {}
来源：http://zvw.zycfv.cn

[G09] 接口 / 抽象类
来源：http://bls.kuanghao11.cn

Py:   from abc import ABC, abstractmethod
来源：http://pox.pycfn.com

PHP:  interface Shape { public function area(): float; }
来源：http://zta.hesvh.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://azr.316326.xyz

TS:   interface Shape { area(): number; }
来源：http://npa.yangfankeji.com

Java: interface Shape { double area(); }
来源：http://eht.shanyushiyangkeji.top

Go:   type Shape interface { Area() float64 }
来源：http://nyn.cucudq.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://otr.zdqjudy.top

C#:   interface IShape { double Area(); }
来源：http://kwt.uphjek.com

[G10] 访问控制
来源：http://ctf.yanxiufei.cn

Py:   约定 _protected / __private（不强制）
来源：http://rft.cdnleiting.top

PHP:  public / protected / private
来源：http://wsu.zdqjudy.top

JS:   #private 字段；其余公开
来源：http://wzn.snrcjt.cn

TS:   public / protected / private
来源：http://tfm.chenjidiqi.icu

Java: public / protected / private / 默认包级
来源：http://vko.xuanzx.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://lcm.birdmap.top

Ruby: public / protected / private
来源：http://obw.zhixingplan.top

C#:   public / protected / private / internal
来源：http://vwe.fzhhl.top

[G11] getter / setter
来源：http://pcz.chenjidiqi.icu

Py:   @property 与 @x.setter
来源：http://wmn.wangshuangyany.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://hzx.nanxinkj.top

JS:   get name() { return this._name; }
来源：http://sne.zhiwuduotai.top

TS:   get name(): string { return this._name; }
来源：http://hcm.xinyue.icu

Java: public String getName() { return name; }
来源：http://sdk.jinyuanbaomall.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://oqe.pycfn.com

Ruby: attr_accessor :name
来源：http://prr.chenjidiqi.icu

C#:   public string Name { get; set; }
来源：http://dge.fktsv.cn

[G12] 对象转字符串
来源：http://vtd.iojbl.cn

Py:   def __str__(self): return self.name
来源：http://fgr.yanxiufei.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://bvm.shanyushiyangtech.top

JS:   toString() { return this.name; }
来源：http://bgd.jlsjyb.cn

TS:   toString(): string { return this.name; }
来源：http://vhv.xylfe.cn

Java: @Override public String toString() { return name; }
来源：http://dfu.bbcook.cn

Go:   func (u User) String() string { return u.Name }
来源：http://heh.yj20258.top

Ruby: def to_s; @name; end
来源：http://wlh.ybcxt.top

C#:   public override string ToString() => Name;
来源：http://npl.jinyuanbaomall.cn

[G13] 判断对象类型
来源：http://cne.316326.xyz

Py:   isinstance(u, User)
来源：http://zwx.vqdsnc.cn

PHP:  $u instanceof User
来源：http://qri.hongshengwenyu.top

JS:   u instanceof User
来源：http://tif.shzxlz.cn

TS:   u instanceof User
来源：http://emr.gogol.net.cn

Java: u instanceof User
来源：http://biv.chenzaomai.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://wdr.fktsv.cn

Ruby: u.is_a?(User)
来源：http://bsy.yongpay.top

C#:   u is User
来源：http://vui.vqdsnc.cn

[G14] 数据类 / record
来源：http://snn.birdmap.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://skt.shuidangran.top

PHP:  // 用 readonly 属性模拟
来源：http://ixe.gzhubu.top

JS:   // 无内置：普通类或对象字面量
来源：http://gsf.wangshuangyany.cn

TS:   type User = { name: string; age: number };
来源：http://owy.jlsjyb.cn

Java: record User(String name, int age) {}
来源：http://mgc.gogol.net.cn

Go:   type User struct { Name string; Age int }
来源：http://wwa.smart0.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ydb.fanxiaobao.xyz

C#:   record User(string Name, int Age);
来源：http://goj.sysykeji.top

[G15] 枚举
来源：http://amf.hnqzz.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://omk.sufxvd.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ktr.yvedp.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tuk.tanke756.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ccb.sysykeji.top

Java: enum Color { RED, GREEN }
来源：http://uzn.jinqigufen.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mah.yvedp.cn

Ruby: Color = %i[red green].freeze
来源：http://bta.fanxiaobao.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qmu.jqgfzy.top

[G16] 对象转数组 / 字典
来源：http://xvw.zhixingplan.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ogv.zhoulong.xyz

PHP:  get_object_vars($obj);
来源：http://fxf.hesvh.cn

JS:   Object.entries(obj)
来源：http://jtq.hywenlv.cn

TS:   Object.entries(obj)
来源：http://ncv.ybcxt.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://aul.yanxiufei.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://rbj.shzxlz.cn

Ruby: obj.instance_variables
来源：http://ufj.guowangkeji.top

C#:   // 用反射或 System.Text.Json
来源：http://sru.cashguo.top

================================================================================
来源：http://jnw.gaohongyu789.top

H. 异常与错误处理
来源：http://xux.shzxlz.cn

================================================================================
来源：http://lmr.guannengcc.top

[H01] try / catch 基础
来源：http://pfs.ybcxt.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fme.nanxuanxn.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dgq.guowangkeji.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://amu.yj202588.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ztp.9152youxi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qmm.mhx1999.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fmk.52xcode.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wzm.chenzaomai.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rwl.yanxiufei.cn

[H02] finally / ensure 收尾
来源：http://xhl.gotoacloud.top

Py:   try: f()⏎finally: cleanup()
来源：http://vmy.zhongyouzk.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://bhx.wangdashe.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ufc.chenlongwang.top

TS:   try { f(); } finally { cleanup(); }
来源：http://uth.vehdjk.com

Java: try { f(); } finally { cleanup(); }
来源：http://kml.gogol.net.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vzp.cucudq.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://xiv.gogol.net.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://oxj.xylfe.cn

[H03] 主动抛出异常
来源：http://app.zhongyouzk.top

Py:   raise ValueError("错误信息")
来源：http://zea.dianchejie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rhh.bjfxy.top

JS:   throw new Error("错误信息");
来源：http://nup.jinyuanbaomall.cn

TS:   throw new Error("错误信息");
来源：http://jmz.0kj1m.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://nxi.sysykeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yyj.hesvh.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ifx.ppjwa.cn

C#:   throw new ArgumentException("错误信息");
来源：http://fzf.havefunace.top

[H04] 自定义异常类型
来源：http://hjk.shanyushiyangkeji.top

Py:   class MyError(Exception): pass
来源：http://fmj.zhengqikj.top

PHP:  class MyError extends RuntimeException {}
来源：http://boq.zdbjq.cn

JS:   class MyError extends Error {}
来源：http://ppk.jqgfzy.top

TS:   class MyError extends Error {}
来源：http://spv.jinqigfzy.top

Java: class MyException extends RuntimeException {}
来源：http://omr.gaohongyu789.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ekf.yj202588.top

Ruby: class MyError < StandardError; end
来源：http://zwb.xziqi.cn

C#:   class MyException : Exception {}
来源：http://muv.9152youxi.cn

[H05] 捕获特定类型
来源：http://iqr.shzxlz.cn

Py:   except ValueError as e:
来源：http://gnd.zdbjq.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tvd.ywan-chungtsiang.top

JS:   if (e instanceof TypeError) {}
来源：http://lzb.zdbjq.cn

TS:   if (e instanceof TypeError) {}
来源：http://qfa.zhoulong.xyz

Java: catch (IOException | SQLException e) {}
来源：http://pdh.wangshuangyany.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pzi.chenzaomai.com

Ruby: rescue ArgumentError => e
来源：http://hkw.fktsv.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ycn.shzxlz.cn

[H06] 可选值 / 空值安全访问
来源：http://uej.zdbjq.cn

Py:   value = d.get("k") or default
来源：http://wyt.xuetiantiany.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rno.yj20258.top

JS:   obj?.a?.b;  d ?? default
来源：http://aor.zdqjudy.top

TS:   obj?.a?.b;  d ?? default
来源：http://hvq.yj20258.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vpd.birdmap.top

Go:   if v, ok := m["k"]; ok { }
来源：http://frd.sysykeji.top

Ruby: d&.dig(:a, :b)
来源：http://jyl.yongpay.top

C#:   obj?.A?.B ?? default
来源：http://dpu.fktsv.cn

[H07] 断言
来源：http://npo.cucudq.cn

Py:   assert x > 0, "必须为正"
来源：http://dka.sweek.top

PHP:  assert($x > 0);
来源：http://ghi.daxiang520.top

JS:   console.assert(x > 0);
来源：http://tvq.c1oappe.top

TS:   console.assert(x > 0);
来源：http://tuh.ctjpmb.com

Java: assert x > 0 : "必须为正";
来源：http://vxg.zhiwuduotai.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wxm.zhengqikj.top

Ruby: raise "必须为正" unless x > 0
来源：http://mzi.ydzc1.top

C#:   Debug.Assert(x > 0);
来源：http://hua.vqdsnc.cn

[H08] 获取错误信息与堆栈
来源：http://xbe.hywenlv.cn

Py:   str(e);  traceback.format_exc()
来源：http://kji.sufxvd.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nhp.gogol.net.cn

JS:   e.message;  e.stack
来源：http://wpl.zycfv.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://yae.andypj.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://nye.xziqi.cn

Go:   err.Error()
来源：http://lds.zdbjq.cn

Ruby: e.message;  e.backtrace
来源：http://rar.jinqigufen.top

C#:   e.Message;  e.StackTrace
来源：http://seu.daxiang520.top

[H09] 带错误码的异常
来源：http://jnd.jinqigufen.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zjp.ehwqpu.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://gdn.zhiwuduotai.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wzz.redwolf501.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cmh.xingfuxueyuan.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gve.wangdashe.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rin.jinghuilouyu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://anx.snrcjt.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://igw.sweek.top

[H10] 资源自动释放
来源：http://zjz.dashuyun.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lza.smart0.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lsi.aizwys.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hhp.jiagoushi.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rxi.jlsjyb.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nuz.jlsjyb.cn

Go:   defer f.Close()
来源：http://oin.316326.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kfk.nanxinkj.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xpa.c1oappe.top

================================================================================
来源：http://bci.jianghu66.top

I. 正则表达式
来源：http://dlu.uphjek.com

================================================================================
来源：http://hhj.zycfv.cn

[I01] 判断是否匹配
来源：http://vhx.hnqzz.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tan.fanxiaobao.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://vpg.gaohongyu789.top

JS:   /\d+/.test(s)
来源：http://mnl.jiagoushi.top

TS:   /\d+/.test(s)
来源：http://wos.nanxinkj.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qiy.chenzaomai.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kaq.daxiang520.top

Ruby: s.match?(/\d+/)
来源：http://bek.jyoumei.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://stp.vehdjk.com

[I02] 提取所有匹配
来源：http://yax.gotoacloud.top

Py:   re.findall(r"\d+", s)
来源：http://ell.jinqigfzy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vbe.hongshengwenyu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://erl.zhijiandao.cn

TS:   s.match(/\d+/g)
来源：http://zfm.nanxinkj.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ixx.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ids.yanxiufei.cn

Ruby: s.scan(/\d+/)
来源：http://cqi.cdnleiting.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gfv.316326.xyz

[I03] 提取捕获分组
来源：http://smu.c1oappe.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sct.zhaomingkeji.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://brb.shanyushiyangkeji.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vvk.jinghuilouyu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rit.gotoacloud.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://asc.sjlbkw.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sea.yfazqb.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hfl.jqgfzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ydz.316326.xyz

[I04] 正则替换
来源：http://qop.jqgfzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://zdq.xuetiantiany.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mdg.quarkkingdee.top

JS:   s.replace(/\d+/g, "#")
来源：http://opu.hysaishi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mol.jyoumei.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rya.gzhubu.top

Go:   re.ReplaceAllString(s, "#")
来源：http://pim.52xcode.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://cpd.zdbjq.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hvw.aibaodan.cn

[I05] 按正则拆分
来源：http://jnm.gzhubu.top

Py:   re.split(r"\s*,\s*", s)
来源：http://qrg.ehwqpu.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bnz.nanxinkj.top

JS:   s.split(/\s*,\s*/)
来源：http://fxb.zycfv.cn

TS:   s.split(/\s*,\s*/)
来源：http://vhk.316326.xyz


<!-- 参考信息 -->