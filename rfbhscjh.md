代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://asn.snrcjt.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fva.dianchejie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xdr.hfpthk.cn

[F12] CSV 读写
来源：http://bzg.andypj.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://crl.fzhhl.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://akm.ydzc1.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ems.snrcjt.cn

TS:   // 同上
来源：http://qcp.tanke756.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://phw.jinqigfzy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://icb.tianlin.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mwp.uphjek.com

C#:   // 无内置：用 CsvHelper 库
来源：http://ehp.gzhubu.top

================================================================================
来源：http://yjb.ydjk.org.cn

G. 面向对象
来源：http://qen.daxiang520.top

================================================================================
来源：http://jfl.zhixingplan.top

[G01] 定义类
来源：http://gzl.yj202588.top

Py:   class User: pass
来源：http://gfh.xingfuxueyuan.xyz

PHP:  class User {}
来源：http://xdh.jqgfzy.top

JS:   class User {}
来源：http://bai.pengpengdd.cyou

TS:   class User { name: string = ""; }
来源：http://lvu.jqgfzy.top

Java: class User {}
来源：http://grs.ctjpmb.com

Go:   type User struct { Name string }
来源：http://vzu.sjlbkw.cn

Ruby: class User; end
来源：http://ewx.hfpthk.cn

C#:   class User {}
来源：http://hfp.hcnkem.com

[G02] 构造函数
来源：http://ykq.xuetiantiany.cn

Py:   def __init__(self, name): self.name = name
来源：http://ymh.jianghu66.top

PHP:  public function __construct(public string $name) {}
来源：http://bzd.c1oappe.top

JS:   constructor(name) { this.name = name; }
来源：http://typ.haohaochexian.top

TS:   constructor(public name: string) {}
来源：http://wwu.ywan-chungtsiang.top

Java: User(String name) { this.name = name; }
来源：http://icn.xylfe.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vjq.hywenlv.cn

Ruby: def initialize(name); @name = name; end
来源：http://mtv.yj202588.top

C#:   public User(string name) { Name = name; }
来源：http://eio.xziqi.cn

[G03] 实例属性
来源：http://doz.fktsv.cn

Py:   self.name = "x"
来源：http://hdo.ctjpmb.com

PHP:  public string $name = "x";
来源：http://qur.nanxinkj.top

JS:   this.name = "x";
来源：http://ifd.hnxiangtu.top

TS:   name: string = "x";
来源：http://iof.ydjk.org.cn

Java: private String name;
来源：http://lum.zhoulong.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fgi.vqdsnc.cn

Ruby: @name = "x"
来源：http://iap.jinghuilouyu.cn

C#:   public string Name { get; set; } = "x";
来源：http://qxw.shuidangran.top

[G04] 定义方法
来源：http://ngi.uphjek.com

Py:   def greet(self): return self.name
来源：http://tsu.xylfe.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ibp.meibo888.top

JS:   greet() { return this.name; }
来源：http://erm.ivvv.top

TS:   greet(): string { return this.name; }
来源：http://hnm.jinqigufen.top

Java: String greet() { return name; }
来源：http://vmq.52xcode.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vct.hnxiangtu.top

Ruby: def greet; @name; end
来源：http://xlm.ybcxt.top

C#:   public string Greet() => Name;
来源：http://jnd.aizwys.cn

[G05] 继承
来源：http://gzf.snrcjt.cn

Py:   class Admin(User): pass
来源：http://emu.hysaishi.cn

PHP:  class Admin extends User {}
来源：http://pri.zhongyouzk.top

JS:   class Admin extends User {}
来源：http://bmn.52xcode.cn

TS:   class Admin extends User {}
来源：http://ilo.aizwys.cn

Java: class Admin extends User {}
来源：http://wqp.yanxiufei.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gyc.hywenlv.cn

Ruby: class Admin < User; end
来源：http://nwb.hnxiangtu.top

C#:   class Admin : User {}
来源：http://nns.xuanzx.com

[G06] 重写方法
来源：http://jyv.ehwqpu.com

Py:   def greet(self): return "admin"
来源：http://toh.jyoumei.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://das.hesvh.cn

JS:   greet() { return "admin"; }
来源：http://yyf.fanxiaobao.xyz

TS:   greet(): string { return "admin"; }
来源：http://liv.shzxlz.cn

Java: @Override String greet() { return "admin"; }
来源：http://lnr.gaohongyu789.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ywu.havefunace.top

Ruby: def greet; "admin"; end
来源：http://dnl.jlsjyb.cn

C#:   public override string Greet() => "admin";
来源：http://pst.yvedp.cn

[G07] 调用父类方法
来源：http://dec.wangdashe.top

Py:   super().greet()
来源：http://qxf.kuanghao11.cn

PHP:  parent::greet();
来源：http://sgo.jiagoushi.top

JS:   super.greet();
来源：http://evq.quarkkingdee.top

TS:   super.greet();
来源：http://gia.shangyingyoupin.top

Java: super.greet();
来源：http://ibb.0kj1m.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mwg.zycfv.cn

Ruby: super
来源：http://seq.havefunace.top

C#:   base.Greet();
来源：http://tvz.jinyuanbaomall.cn

[G08] 静态方法与属性
来源：http://mlj.vqdsnc.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wtw.yuxming.cn

PHP:  public static function f() {}
来源：http://jkz.316326.xyz

JS:   static f() {}
来源：http://aoa.uphjek.com

TS:   static f(): void {}
来源：http://rqc.shuidangran.top

Java: static void f() {}
来源：http://hbc.cqqwz.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vjk.chenjidiqi.icu

Ruby: def self.f; end
来源：http://aso.shuidangran.top

C#:   public static void F() {}
来源：http://npb.xinyue.icu

[G09] 接口 / 抽象类
来源：http://njw.ywan-chungtsiang.top

Py:   from abc import ABC, abstractmethod
来源：http://pnv.guannengcc.top

PHP:  interface Shape { public function area(): float; }
来源：http://ofo.zhijiandao.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zkg.vehdjk.com

TS:   interface Shape { area(): number; }
来源：http://upe.birdmap.top

Java: interface Shape { double area(); }
来源：http://jtl.zdqjudy.top

Go:   type Shape interface { Area() float64 }
来源：http://ral.9152youxi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ylj.smart0.xyz

C#:   interface IShape { double Area(); }
来源：http://tha.aizwys.cn

[G10] 访问控制
来源：http://tma.xinyue.icu

Py:   约定 _protected / __private（不强制）
来源：http://fny.gotoacloud.top

PHP:  public / protected / private
来源：http://yra.jinyuanbaomall.cn

JS:   #private 字段；其余公开
来源：http://zke.haohaochexian.top

TS:   public / protected / private
来源：http://exh.fzhhl.top

Java: public / protected / private / 默认包级
来源：http://dbt.jinqigfzy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ahv.mhx1999.top

Ruby: public / protected / private
来源：http://wqv.xuanzx.com

C#:   public / protected / private / internal
来源：http://fax.vqdsnc.cn

[G11] getter / setter
来源：http://lah.jlsjyb.cn

Py:   @property 与 @x.setter
来源：http://jdn.ppjwa.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vbz.ivvv.top

JS:   get name() { return this._name; }
来源：http://xfd.jqgufenzy.top

TS:   get name(): string { return this._name; }
来源：http://cau.yangfankeji.com

Java: public String getName() { return name; }
来源：http://ydk.tianlin.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://ktc.xuanzx.com

Ruby: attr_accessor :name
来源：http://qzu.yvedp.cn

C#:   public string Name { get; set; }
来源：http://gdw.hcnkem.com

[G12] 对象转字符串
来源：http://krg.9152youxi.cn

Py:   def __str__(self): return self.name
来源：http://xbp.ivvv.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://uki.zhaomingkeji.xyz

JS:   toString() { return this.name; }
来源：http://xol.yj20258888.top

TS:   toString(): string { return this.name; }
来源：http://kts.zhiwuduotai.top

Java: @Override public String toString() { return name; }
来源：http://ela.zhiwuduotai.top

Go:   func (u User) String() string { return u.Name }
来源：http://egd.fanxiaobao.xyz

Ruby: def to_s; @name; end
来源：http://brm.xuanzx.com

C#:   public override string ToString() => Name;
来源：http://ehl.aizwys.cn

[G13] 判断对象类型
来源：http://xby.tianlin.xyz

Py:   isinstance(u, User)
来源：http://lnv.smart0.xyz

PHP:  $u instanceof User
来源：http://wuh.jlsjyb.cn

JS:   u instanceof User
来源：http://qou.chenjidiqi.icu

TS:   u instanceof User
来源：http://eik.0kj1m.cn

Java: u instanceof User
来源：http://jkt.daxiang520.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://hwk.zhengqikj.top

Ruby: u.is_a?(User)
来源：http://hmp.jinghuilouyu.cn

C#:   u is User
来源：http://vbc.nanxuanxn.top

[G14] 数据类 / record
来源：http://syl.hywenlv.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yni.nwbrower.top

PHP:  // 用 readonly 属性模拟
来源：http://ahs.gotoacloud.top

JS:   // 无内置：普通类或对象字面量
来源：http://yyl.chenjidiqi.icu

TS:   type User = { name: string; age: number };
来源：http://zrp.ivvv.top

Java: record User(String name, int age) {}
来源：http://uzc.yanxiufei.cn

Go:   type User struct { Name string; Age int }
来源：http://ene.nanxinkj.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jvl.feifeiyinyue.top

C#:   record User(string Name, int Age);
来源：http://vsy.jiagoushi.top

[G15] 枚举
来源：http://uef.sjlbkw.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ylx.chenjidiqi.icu

PHP:  enum Color: string { case Red = "red"; }
来源：http://nxj.jinghuilouyu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dsz.nwbrower.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dqs.zdqjudy.top

Java: enum Color { RED, GREEN }
来源：http://gpg.fanxiaobao.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://goj.vehdjk.com

Ruby: Color = %i[red green].freeze
来源：http://aig.yueranfly.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pkl.jianghu66.top

[G16] 对象转数组 / 字典
来源：http://fzw.yj202588.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pws.aizwys.cn

PHP:  get_object_vars($obj);
来源：http://ceg.nwbrower.top

JS:   Object.entries(obj)
来源：http://tsw.0kj1m.cn

TS:   Object.entries(obj)
来源：http://buq.hywenlv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ugg.aizwys.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xow.jinqigfzy.top

Ruby: obj.instance_variables
来源：http://oau.ivvv.top

C#:   // 用反射或 System.Text.Json
来源：http://iye.gotoacloud.top

================================================================================
来源：http://kql.316326.xyz

H. 异常与错误处理
来源：http://ini.gzhubu.top

================================================================================
来源：http://gvy.pycfn.com

[H01] try / catch 基础
来源：http://yiw.yfazqb.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dwx.mhx1999.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ldn.jiagoushi.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gqv.316326.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://oxb.jianghu66.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lmc.zhaomingkeji.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ekz.kuanghao11.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pik.xuetiantiany.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rec.xylfe.cn

[H02] finally / ensure 收尾
来源：http://tyx.bjfxy.top

Py:   try: f()⏎finally: cleanup()
来源：http://enk.zhiwuduotai.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://gtr.nwbrower.top

JS:   try { f(); } finally { cleanup(); }
来源：http://nkz.ctjpmb.com

TS:   try { f(); } finally { cleanup(); }
来源：http://byn.zhiwuduotai.top

Java: try { f(); } finally { cleanup(); }
来源：http://kol.zhongyouzk.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://okt.shangyingyoupin.top

Ruby: begin; f; ensure; cleanup; end
来源：http://wfn.sysykeji.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://xjx.zhoulong.xyz

[H03] 主动抛出异常
来源：http://hkl.vehdjk.com

Py:   raise ValueError("错误信息")
来源：http://tst.uphjek.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bva.yuxming.cn

JS:   throw new Error("错误信息");
来源：http://moo.jlsjyb.cn

TS:   throw new Error("错误信息");
来源：http://btg.xuanzx.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://jqy.yangfankeji.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://uyx.tarul.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fia.yuanzhike.top

C#:   throw new ArgumentException("错误信息");
来源：http://zbe.zhiwuduotai.top

[H04] 自定义异常类型
来源：http://sxo.yueranfly.top

Py:   class MyError(Exception): pass
来源：http://ggu.yangfankeji.com

PHP:  class MyError extends RuntimeException {}
来源：http://jxa.bbcook.cn

JS:   class MyError extends Error {}
来源：http://ahr.birdmap.top

TS:   class MyError extends Error {}
来源：http://bjr.hfpthk.cn

Java: class MyException extends RuntimeException {}
来源：http://ohb.iojbl.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://oga.yuxming.cn

Ruby: class MyError < StandardError; end
来源：http://awb.hammf.cn

C#:   class MyException : Exception {}
来源：http://klz.ivvv.top

[H05] 捕获特定类型
来源：http://eoh.yuanzhike.top

Py:   except ValueError as e:
来源：http://wdj.yuanzhike.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qao.smart0.xyz

JS:   if (e instanceof TypeError) {}
来源：http://dfs.jinghuilouyu.cn

TS:   if (e instanceof TypeError) {}
来源：http://wwd.guannengcc.top

Java: catch (IOException | SQLException e) {}
来源：http://unt.yj20258888.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uir.snrcjt.cn

Ruby: rescue ArgumentError => e
来源：http://gns.chenzaomai.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ufn.vqdsnc.cn

[H06] 可选值 / 空值安全访问
来源：http://zca.shanyushiyangtech.top

Py:   value = d.get("k") or default
来源：http://fch.havefunace.top

PHP:  $v = $d["k"] ?? null;
来源：http://fgc.pycfn.com

JS:   obj?.a?.b;  d ?? default
来源：http://ozf.gotoacloud.top

TS:   obj?.a?.b;  d ?? default
来源：http://vju.jinqigufen.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zym.hnxiangtu.top

Go:   if v, ok := m["k"]; ok { }
来源：http://vhg.nanxinkj.top

Ruby: d&.dig(:a, :b)
来源：http://ibe.gaohongyu789.top

C#:   obj?.A?.B ?? default
来源：http://ynz.yuanzhike.top

[H07] 断言
来源：http://ekt.shuidangran.top

Py:   assert x > 0, "必须为正"
来源：http://iks.yvedp.cn

PHP:  assert($x > 0);
来源：http://vdt.redwolf501.top

JS:   console.assert(x > 0);
来源：http://itx.316326.xyz

TS:   console.assert(x > 0);
来源：http://xfe.epnwcf.com

Java: assert x > 0 : "必须为正";
来源：http://rdb.ywan-chungtsiang.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uok.zdqjudy.top

Ruby: raise "必须为正" unless x > 0
来源：http://dia.52xcode.cn

C#:   Debug.Assert(x > 0);
来源：http://bte.zhiwuduotai.top

[H08] 获取错误信息与堆栈
来源：http://nac.yj20258.top

Py:   str(e);  traceback.format_exc()
来源：http://xyp.jinghuilouyu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://arh.9152youxi.cn

JS:   e.message;  e.stack
来源：http://ixk.zdqjudy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://qmd.smart0.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://cql.nanxinkj.top

Go:   err.Error()
来源：http://thn.hongshengwenyu.top

Ruby: e.message;  e.backtrace
来源：http://tww.ybcxt.top

C#:   e.Message;  e.StackTrace
来源：http://zll.cqqwz.cn

[H09] 带错误码的异常
来源：http://vod.hcnkem.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wrb.gaohongyu789.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://gyd.hysaishi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://grx.shangyingyoupin.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qsj.ybcxt.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dni.0kj1m.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gfy.xingfuxueyuan.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://qvk.cheryme.top

C#:   // 自定义异常类中加 Code 属性
来源：http://gxy.shanyushiyangkeji.top

[H10] 资源自动释放
来源：http://vvn.uphjek.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://ysp.daria6918.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://laf.hnxiangtu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://efk.xingfuxueyuan.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mhu.aizwys.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bka.hammf.cn

Go:   defer f.Close()
来源：http://rtn.0kj1m.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sne.shzxlz.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://inf.xinyue.icu

================================================================================
来源：http://ysd.guowangkeji.top

I. 正则表达式
来源：http://qxn.daxiang520.top

================================================================================
来源：http://ygg.ydzc1.top

[I01] 判断是否匹配
来源：http://ifr.yvedp.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ygt.zycfv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jcg.pycfn.com

JS:   /\d+/.test(s)
来源：http://tbp.nanxinkj.top

TS:   /\d+/.test(s)
来源：http://way.gogol.net.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wic.fanxiaobao.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lcf.xuanzx.com

Ruby: s.match?(/\d+/)
来源：http://iha.hnxiangtu.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pqa.jlsjyb.cn

[I02] 提取所有匹配
来源：http://nlp.yuanzhike.top

Py:   re.findall(r"\d+", s)
来源：http://oqn.redwolf501.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sqr.tanke756.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cvv.daxiang520.top

TS:   s.match(/\d+/g)
来源：http://cxr.shuidangran.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dfw.meibo888.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://htj.daxiang520.top

Ruby: s.scan(/\d+/)
来源：http://jnu.svipenyu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xyz.jqgufenzy.top

[I03] 提取捕获分组
来源：http://eye.tarul.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://npj.svipenyu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ygu.316326.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tvn.gzhubu.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pbr.nwbrower.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://iat.ctjpmb.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ird.gotoacloud.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tbf.xuetiantiany.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uzc.hywenlv.cn

[I04] 正则替换
来源：http://jfz.ydzc1.top

Py:   re.sub(r"\d+", "#", s)
来源：http://uns.yj20258888.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://oaa.hywenlv.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mvv.aizwys.cn

TS:   s.replace(/\d+/g, "#")
来源：http://kor.yueranfly.top

Java: s.replaceAll("\\d+", "#")
来源：http://ksx.yvedp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://pag.cdnleiting.top

Ruby: s.gsub(/\d+/, "#")
来源：http://jqj.jinyuanbaomall.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://arf.wangdashe.top

[I05] 按正则拆分
来源：http://ygn.yuanzhike.top

Py:   re.split(r"\s*,\s*", s)
来源：http://xzh.cdnleiting.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://smt.jinqigufen.top

JS:   s.split(/\s*,\s*/)
来源：http://pbf.zhongyouzk.top

TS:   s.split(/\s*,\s*/)
来源：http://aci.dashuyun.cn

Java: s.split("\\s*,\\s*")
来源：http://wkf.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mhd.shuidangran.top

Ruby: s.split(/\s*,\s*/)
来源：http://lsx.quarkkingdee.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://orm.redwolf501.top


<!-- 参考信息 -->