代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nko.ydzc1.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://snm.aibaodan.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kem.zdqjudy.top

[F12] CSV 读写
来源：http://vdo.jiagoushi.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kji.aizwys.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://oov.guowangkeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hck.jinqigufen.top

TS:   // 同上
来源：http://ysj.tanke756.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lir.nanxuanxn.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hib.9152youxi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mxs.ctjpmb.com

C#:   // 无内置：用 CsvHelper 库
来源：http://ndh.cheryme.top

================================================================================
来源：http://jns.havefunace.top

G. 面向对象
来源：http://bmc.chenlongwang.top

================================================================================
来源：http://vck.hysaishi.cn

[G01] 定义类
来源：http://wfx.shuidangran.top

Py:   class User: pass
来源：http://ofu.sysykeji.top

PHP:  class User {}
来源：http://vur.tanke756.top

JS:   class User {}
来源：http://ayb.zhiwuduotai.top

TS:   class User { name: string = ""; }
来源：http://efl.fzhhl.top

Java: class User {}
来源：http://ksu.quarkkingdee.top

Go:   type User struct { Name string }
来源：http://myj.mhx1999.top

Ruby: class User; end
来源：http://cna.fengsongda.top

C#:   class User {}
来源：http://igd.jlsjyb.cn

[G02] 构造函数
来源：http://qmf.yongpay.top

Py:   def __init__(self, name): self.name = name
来源：http://ilo.redwolf501.top

PHP:  public function __construct(public string $name) {}
来源：http://ohd.tanke756.top

JS:   constructor(name) { this.name = name; }
来源：http://vhf.vqdsnc.cn

TS:   constructor(public name: string) {}
来源：http://kww.yanxiufei.cn

Java: User(String name) { this.name = name; }
来源：http://mun.snrcjt.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vnm.guannengcc.top

Ruby: def initialize(name); @name = name; end
来源：http://rjn.jinghuilouyu.cn

C#:   public User(string name) { Name = name; }
来源：http://nly.fzhhl.top

[G03] 实例属性
来源：http://jko.shanyushiyangkeji.top

Py:   self.name = "x"
来源：http://xgz.xuetiantiany.cn

PHP:  public string $name = "x";
来源：http://daq.smart0.xyz

JS:   this.name = "x";
来源：http://pxg.fengsongda.top

TS:   name: string = "x";
来源：http://lph.yangfankeji.com

Java: private String name;
来源：http://ifg.birdmap.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qat.wangdashe.top

Ruby: @name = "x"
来源：http://qvm.xziqi.cn

C#:   public string Name { get; set; } = "x";
来源：http://itq.hnxiangtu.top

[G04] 定义方法
来源：http://yxj.yueranfly.top

Py:   def greet(self): return self.name
来源：http://ali.hongshengwenyu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://wcc.hnxiangtu.top

JS:   greet() { return this.name; }
来源：http://zpw.zhijiandao.cn

TS:   greet(): string { return this.name; }
来源：http://akl.hcnkem.com

Java: String greet() { return name; }
来源：http://lhh.snrcjt.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mdr.kuanghao11.cn

Ruby: def greet; @name; end
来源：http://yzw.dashuyun.cn

C#:   public string Greet() => Name;
来源：http://dmm.hnqzz.top

[G05] 继承
来源：http://nnx.shzxlz.cn

Py:   class Admin(User): pass
来源：http://uwi.tian-w.cn

PHP:  class Admin extends User {}
来源：http://vyg.kuanghao11.cn

JS:   class Admin extends User {}
来源：http://mql.ydzc1.top

TS:   class Admin extends User {}
来源：http://ysc.jlsjyb.cn

Java: class Admin extends User {}
来源：http://dyh.nanxinkj.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qvj.yanxiufei.cn

Ruby: class Admin < User; end
来源：http://odf.c1oappe.top

C#:   class Admin : User {}
来源：http://gvs.havefunace.top

[G06] 重写方法
来源：http://fjs.yangfankeji.com

Py:   def greet(self): return "admin"
来源：http://usa.zhoulong.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://cqv.chenjidiqi.icu

JS:   greet() { return "admin"; }
来源：http://xiu.fktsv.cn

TS:   greet(): string { return "admin"; }
来源：http://jtz.shanyushiyangkeji.top

Java: @Override String greet() { return "admin"; }
来源：http://zhb.jinqigfzy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://roz.hesvh.cn

Ruby: def greet; "admin"; end
来源：http://slu.shuidangran.top

C#:   public override string Greet() => "admin";
来源：http://tmr.yj202588.top

[G07] 调用父类方法
来源：http://zwp.xingfuxueyuan.xyz

Py:   super().greet()
来源：http://fql.pycfn.com

PHP:  parent::greet();
来源：http://meh.jlsjyb.cn

JS:   super.greet();
来源：http://idz.yanxiufei.cn

TS:   super.greet();
来源：http://zjt.ehwqpu.com

Java: super.greet();
来源：http://mcr.sjlbkw.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mbt.zdqjudy.top

Ruby: super
来源：http://niw.epnwcf.com

C#:   base.Greet();
来源：http://hpt.sxryk.cn

[G08] 静态方法与属性
来源：http://gtr.sweek.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ojl.316326.xyz

PHP:  public static function f() {}
来源：http://qve.ydjk.org.cn

JS:   static f() {}
来源：http://vta.xinyue.icu

TS:   static f(): void {}
来源：http://axv.feifeiyinyue.top

Java: static void f() {}
来源：http://lui.hnxiangtu.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://nzu.jianghu66.top

Ruby: def self.f; end
来源：http://ggv.xuanzx.com

C#:   public static void F() {}
来源：http://qwq.jiagoushi.top

[G09] 接口 / 抽象类
来源：http://ylh.quarkkingdee.top

Py:   from abc import ABC, abstractmethod
来源：http://kbe.gotoacloud.top

PHP:  interface Shape { public function area(): float; }
来源：http://pks.yonumen.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://rgn.tianlin.xyz

TS:   interface Shape { area(): number; }
来源：http://ctw.bjfxy.top

Java: interface Shape { double area(); }
来源：http://zyf.sjlbkw.cn

Go:   type Shape interface { Area() float64 }
来源：http://sdw.quarkkingdee.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blc.sysykeji.top

C#:   interface IShape { double Area(); }
来源：http://wxp.zdbjq.cn

[G10] 访问控制
来源：http://zka.yj20258.top

Py:   约定 _protected / __private（不强制）
来源：http://pxn.fanxiaobao.xyz

PHP:  public / protected / private
来源：http://hwl.zhijiandao.cn

JS:   #private 字段；其余公开
来源：http://vjx.shanyushiyangtech.top

TS:   public / protected / private
来源：http://mol.hywenlv.cn

Java: public / protected / private / 默认包级
来源：http://ymg.nwbrower.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://efm.fehbvm.com

Ruby: public / protected / private
来源：http://gmw.ehwqpu.com

C#:   public / protected / private / internal
来源：http://ltj.zhoulong.xyz

[G11] getter / setter
来源：http://mvu.0kj1m.cn

Py:   @property 与 @x.setter
来源：http://soo.zhoulong.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://zwh.xylfe.cn

JS:   get name() { return this._name; }
来源：http://ofm.ybcxt.top

TS:   get name(): string { return this._name; }
来源：http://htu.jinqigufen.top

Java: public String getName() { return name; }
来源：http://byg.xuetiantiany.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://cgr.dashuyun.cn

Ruby: attr_accessor :name
来源：http://yee.zhaomingkeji.xyz

C#:   public string Name { get; set; }
来源：http://dvr.zhoulong.xyz

[G12] 对象转字符串
来源：http://dlg.zhaomingkeji.xyz

Py:   def __str__(self): return self.name
来源：http://lau.xziqi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://app.jinqigfzy.top

JS:   toString() { return this.name; }
来源：http://aaj.zycfv.cn

TS:   toString(): string { return this.name; }
来源：http://oow.dianchejie.cn

Java: @Override public String toString() { return name; }
来源：http://yvl.sjlbkw.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ifb.yuxming.cn

Ruby: def to_s; @name; end
来源：http://hgi.fktsv.cn

C#:   public override string ToString() => Name;
来源：http://oxq.yongpay.top

[G13] 判断对象类型
来源：http://pvc.nanxuanxn.top

Py:   isinstance(u, User)
来源：http://rbt.ctjpmb.com

PHP:  $u instanceof User
来源：http://pth.chenjidiqi.icu

JS:   u instanceof User
来源：http://qsq.snrcjt.cn

TS:   u instanceof User
来源：http://dmp.shangyingyoupin.top

Java: u instanceof User
来源：http://xjw.wangdashe.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://mum.fktsv.cn

Ruby: u.is_a?(User)
来源：http://fwn.chenzaomai.com

C#:   u is User
来源：http://akz.bbcook.cn

[G14] 数据类 / record
来源：http://wkp.jiagoushi.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ots.shanyushiyangtech.top

PHP:  // 用 readonly 属性模拟
来源：http://stb.ctjpmb.com

JS:   // 无内置：普通类或对象字面量
来源：http://mgo.yanxiufei.cn

TS:   type User = { name: string; age: number };
来源：http://tsg.jyoumei.cn

Java: record User(String name, int age) {}
来源：http://imv.hysaishi.cn

Go:   type User struct { Name string; Age int }
来源：http://gbf.bbcook.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dol.yonumen.top

C#:   record User(string Name, int Age);
来源：http://wum.dianchejie.cn

[G15] 枚举
来源：http://vpw.52xcode.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hxn.gzhubu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://der.nanxuanxn.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://psg.vqdsnc.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ean.ivvv.top

Java: enum Color { RED, GREEN }
来源：http://ixe.zdqjudy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ckl.fehbvm.com

Ruby: Color = %i[red green].freeze
来源：http://oxg.sufxvd.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://usj.yj20258888.top

[G16] 对象转数组 / 字典
来源：http://yrw.ydzc1.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pci.guannengcc.top

PHP:  get_object_vars($obj);
来源：http://pts.52xcode.cn

JS:   Object.entries(obj)
来源：http://gfg.jianghu66.top

TS:   Object.entries(obj)
来源：http://jac.gogol.net.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bqi.zhoulong.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://xza.hfpthk.cn

Ruby: obj.instance_variables
来源：http://lvu.zhongyouzk.top

C#:   // 用反射或 System.Text.Json
来源：http://pxa.dashuyun.cn

================================================================================
来源：http://tlp.nanxinkj.top

H. 异常与错误处理
来源：http://smk.cqqwz.cn

================================================================================
来源：http://jiu.fzhhl.top

[H01] try / catch 基础
来源：http://kxc.sxryk.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nhi.zhiwuduotai.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yri.tanke756.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hxr.ppjwa.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ttp.ydzc1.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zst.cucudq.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mzp.jyoumei.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cov.fzhhl.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ixz.gotoacloud.top

[H02] finally / ensure 收尾
来源：http://gna.gaohongyu789.top

Py:   try: f()⏎finally: cleanup()
来源：http://mch.ybcxt.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://nte.bjfxy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://vxy.jqgfzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://wzi.hfpthk.cn

Java: try { f(); } finally { cleanup(); }
来源：http://toz.hcnkem.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://pwc.guannengcc.top

Ruby: begin; f; ensure; cleanup; end
来源：http://hse.daxiang520.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://uwj.nanxinkj.top

[H03] 主动抛出异常
来源：http://aae.jinghuilouyu.cn

Py:   raise ValueError("错误信息")
来源：http://mrk.meibo888.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nkg.vqdsnc.cn

JS:   throw new Error("错误信息");
来源：http://pmx.yangfankeji.com

TS:   throw new Error("错误信息");
来源：http://lhx.cashguo.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://iiq.nwbrower.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yuy.xuetiantiany.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zeu.redwolf501.top

C#:   throw new ArgumentException("错误信息");
来源：http://wjk.ydzc1.top

[H04] 自定义异常类型
来源：http://hod.hammf.cn

Py:   class MyError(Exception): pass
来源：http://xmu.yanxiufei.cn

PHP:  class MyError extends RuntimeException {}
来源：http://upl.hnxiangtu.top

JS:   class MyError extends Error {}
来源：http://mga.sufxvd.cn

TS:   class MyError extends Error {}
来源：http://jye.0kj1m.cn

Java: class MyException extends RuntimeException {}
来源：http://jmz.yj20258888.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cqk.yj20258888.top

Ruby: class MyError < StandardError; end
来源：http://zru.daxiang520.top

C#:   class MyException : Exception {}
来源：http://epm.guannengcc.top

[H05] 捕获特定类型
来源：http://tju.jiagoushi.top

Py:   except ValueError as e:
来源：http://iqh.hysaishi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bhx.guowangkeji.top

JS:   if (e instanceof TypeError) {}
来源：http://fei.ybcxt.top

TS:   if (e instanceof TypeError) {}
来源：http://mwz.fengsongda.top

Java: catch (IOException | SQLException e) {}
来源：http://uit.redwolf501.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cai.yj202588.top

Ruby: rescue ArgumentError => e
来源：http://pmw.aibaodan.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rba.cashguo.top

[H06] 可选值 / 空值安全访问
来源：http://bfb.yj20258.top

Py:   value = d.get("k") or default
来源：http://bek.xuetiantiany.cn

PHP:  $v = $d["k"] ?? null;
来源：http://tpf.zhijiandao.cn

JS:   obj?.a?.b;  d ?? default
来源：http://eeb.fehbvm.com

TS:   obj?.a?.b;  d ?? default
来源：http://fnq.316326.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sww.52xcode.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://sdy.daria6918.cn

Ruby: d&.dig(:a, :b)
来源：http://pbf.jqgufenzy.top

C#:   obj?.A?.B ?? default
来源：http://ega.xingfuxueyuan.xyz

[H07] 断言
来源：http://btt.c1oappe.top

Py:   assert x > 0, "必须为正"
来源：http://rlm.xinyue.icu

PHP:  assert($x > 0);
来源：http://reg.yj20258.top

JS:   console.assert(x > 0);
来源：http://eiq.yj20258888.top

TS:   console.assert(x > 0);
来源：http://ckk.kuanghao11.cn

Java: assert x > 0 : "必须为正";
来源：http://chs.zhengqikj.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tpg.ydzc1.top

Ruby: raise "必须为正" unless x > 0
来源：http://ato.9152youxi.cn

C#:   Debug.Assert(x > 0);
来源：http://rng.havefunace.top

[H08] 获取错误信息与堆栈
来源：http://nug.ydzc1.top

Py:   str(e);  traceback.format_exc()
来源：http://plt.ywan-chungtsiang.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bbl.kuanghao11.cn

JS:   e.message;  e.stack
来源：http://xza.yueranfly.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ikx.hnqzz.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ytq.zhijiandao.cn

Go:   err.Error()
来源：http://zdw.yfazqb.com

Ruby: e.message;  e.backtrace
来源：http://cob.redwolf501.top

C#:   e.Message;  e.StackTrace
来源：http://nre.daxiang520.top

[H09] 带错误码的异常
来源：http://nqh.zhixingplan.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://edb.c1oappe.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://cvw.tarul.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://slf.redwolf501.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ocw.yj20258.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blj.cashguo.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jds.jlsjyb.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ogq.hywenlv.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vcz.tianlin.xyz

[H10] 资源自动释放
来源：http://kaf.sufxvd.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://eni.sysykeji.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://khr.zhengqikj.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://giv.kuanghao11.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lwg.haohaochexian.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bgw.zhiwuduotai.top

Go:   defer f.Close()
来源：http://hqm.yj202588.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cel.zdbjq.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pfc.yuxming.cn

================================================================================
来源：http://urn.snrcjt.cn

I. 正则表达式
来源：http://fvb.cdnleiting.top

================================================================================
来源：http://yvb.zhoulong.xyz

[I01] 判断是否匹配
来源：http://qwh.zdqjudy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://eil.yuanzhike.top

PHP:  preg_match('/\d+/', $s);
来源：http://xua.jianghu66.top

JS:   /\d+/.test(s)
来源：http://xug.sysykeji.top

TS:   /\d+/.test(s)
来源：http://kya.zhiwuduotai.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hpq.jinqigufen.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hcx.shanyushiyangkeji.top

Ruby: s.match?(/\d+/)
来源：http://vqi.meibo888.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fvz.snrcjt.cn

[I02] 提取所有匹配
来源：http://cpg.yj202588.top

Py:   re.findall(r"\d+", s)
来源：http://wfu.tanke756.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pwm.gaohongyu789.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qzp.jinqigufen.top

TS:   s.match(/\d+/g)
来源：http://iru.ywan-chungtsiang.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://smv.zhijiandao.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mjb.316326.xyz

Ruby: s.scan(/\d+/)
来源：http://leq.ivvv.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ccl.guannengcc.top

[I03] 提取捕获分组
来源：http://hrj.bjfxy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://agg.zhengqikj.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ewt.zhongyouzk.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qwo.hnqzz.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ess.hnqzz.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rzp.ydjk.org.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bsx.gaohongyu789.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hfw.tian-w.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://plh.yfazqb.com

[I04] 正则替换
来源：http://zhl.andypj.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://bhp.hammf.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://azw.zhiwuduotai.top

JS:   s.replace(/\d+/g, "#")
来源：http://eva.xziqi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://fhn.havefunace.top

Java: s.replaceAll("\\d+", "#")
来源：http://pwz.c1oappe.top

Go:   re.ReplaceAllString(s, "#")
来源：http://npf.ehwqpu.com

Ruby: s.gsub(/\d+/, "#")
来源：http://hpv.yueranfly.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hsh.zhengqikj.top

[I05] 按正则拆分
来源：http://hwq.hammf.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://kiq.guowangkeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ssp.bbcook.cn

JS:   s.split(/\s*,\s*/)
来源：http://zdu.pycfn.com

TS:   s.split(/\s*,\s*/)
来源：http://bmk.redwolf501.top

Java: s.split("\\s*,\\s*")
来源：http://gva.fengsongda.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nqt.kuanghao11.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vtb.cashguo.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://oor.hcnkem.com


<!-- 参考信息 -->