代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rzt.jiagoushi.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vld.ehwqpu.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bvm.dianchejie.cn

[F12] CSV 读写
来源：http://lmi.hfpthk.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hkm.sjlbkw.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uza.fehbvm.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lkt.hammf.cn

TS:   // 同上
来源：http://zvl.bbcook.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jyi.fehbvm.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cos.mhx1999.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ieo.gotoacloud.top

C#:   // 无内置：用 CsvHelper 库
来源：http://scq.chenjidiqi.icu

================================================================================
来源：http://jjy.daria6918.cn

G. 面向对象
来源：http://jad.smart0.xyz

================================================================================
来源：http://cup.zhengqikj.top

[G01] 定义类
来源：http://ibt.daria6918.cn

Py:   class User: pass
来源：http://khr.redwolf501.top

PHP:  class User {}
来源：http://vcn.hesvh.cn

JS:   class User {}
来源：http://pan.jinghuilouyu.cn

TS:   class User { name: string = ""; }
来源：http://kgd.zhengqikj.top

Java: class User {}
来源：http://fgm.yuxming.cn

Go:   type User struct { Name string }
来源：http://yoq.hongshengwenyu.top

Ruby: class User; end
来源：http://epg.ppjwa.cn

C#:   class User {}
来源：http://frd.haohaochexian.top

[G02] 构造函数
来源：http://sgl.zhaomingkeji.xyz

Py:   def __init__(self, name): self.name = name
来源：http://acv.svipenyu.cn

PHP:  public function __construct(public string $name) {}
来源：http://ygr.quarkkingdee.top

JS:   constructor(name) { this.name = name; }
来源：http://gyf.jinqigfzy.top

TS:   constructor(public name: string) {}
来源：http://cni.dashuyun.cn

Java: User(String name) { this.name = name; }
来源：http://xyw.shanyushiyangtech.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gpn.cqqwz.cn

Ruby: def initialize(name); @name = name; end
来源：http://lbk.zhijiandao.cn

C#:   public User(string name) { Name = name; }
来源：http://zfs.yuanzhike.top

[G03] 实例属性
来源：http://uoa.jinqigufen.top

Py:   self.name = "x"
来源：http://ngi.quarkkingdee.top

PHP:  public string $name = "x";
来源：http://hni.tarul.cn

JS:   this.name = "x";
来源：http://nym.mhx1999.top

TS:   name: string = "x";
来源：http://evj.cqqwz.cn

Java: private String name;
来源：http://kpg.zycfv.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fwy.cheryme.top

Ruby: @name = "x"
来源：http://cbf.yj20258888.top

C#:   public string Name { get; set; } = "x";
来源：http://ube.cashguo.top

[G04] 定义方法
来源：http://vmn.wangdashe.top

Py:   def greet(self): return self.name
来源：http://doh.jqgfzy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://yus.pengpengdd.cyou

JS:   greet() { return this.name; }
来源：http://svs.fzhhl.top

TS:   greet(): string { return this.name; }
来源：http://jap.tian-w.cn

Java: String greet() { return name; }
来源：http://hdc.vehdjk.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://ykr.yuanzhike.top

Ruby: def greet; @name; end
来源：http://osb.birdmap.top

C#:   public string Greet() => Name;
来源：http://xvz.aibaodan.cn

[G05] 继承
来源：http://lcp.yvedp.cn

Py:   class Admin(User): pass
来源：http://acx.zdbjq.cn

PHP:  class Admin extends User {}
来源：http://gyt.snrcjt.cn

JS:   class Admin extends User {}
来源：http://bdu.zhengqikj.top

TS:   class Admin extends User {}
来源：http://gww.ehwqpu.com

Java: class Admin extends User {}
来源：http://fmd.ybcxt.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wih.iojbl.cn

Ruby: class Admin < User; end
来源：http://opo.ydzc1.top

C#:   class Admin : User {}
来源：http://wis.sufxvd.cn

[G06] 重写方法
来源：http://rnl.jinghuilouyu.cn

Py:   def greet(self): return "admin"
来源：http://rbn.ydjk.org.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://wep.jinyuanbaomall.cn

JS:   greet() { return "admin"; }
来源：http://pvp.epnwcf.com

TS:   greet(): string { return "admin"; }
来源：http://vcj.jinghuilouyu.cn

Java: @Override String greet() { return "admin"; }
来源：http://fwm.smart0.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nxm.chenlongwang.top

Ruby: def greet; "admin"; end
来源：http://tkh.yvedp.cn

C#:   public override string Greet() => "admin";
来源：http://wxj.guannengcc.top

[G07] 调用父类方法
来源：http://jfl.hongshengwenyu.top

Py:   super().greet()
来源：http://lcz.hysaishi.cn

PHP:  parent::greet();
来源：http://wrw.mhx1999.top

JS:   super.greet();
来源：http://lnc.sufxvd.cn

TS:   super.greet();
来源：http://lrh.epnwcf.com

Java: super.greet();
来源：http://vcd.aizwys.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://occ.ydzc1.top

Ruby: super
来源：http://qww.daria6918.cn

C#:   base.Greet();
来源：http://saf.xingfuxueyuan.xyz

[G08] 静态方法与属性
来源：http://lol.quarkkingdee.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sem.cqqwz.cn

PHP:  public static function f() {}
来源：http://lgq.pengpengdd.cyou

JS:   static f() {}
来源：http://jyi.quarkkingdee.top

TS:   static f(): void {}
来源：http://lkc.gotoacloud.top

Java: static void f() {}
来源：http://ood.sxryk.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://yis.vqdsnc.cn

Ruby: def self.f; end
来源：http://imt.zhiwuduotai.top

C#:   public static void F() {}
来源：http://eoe.aibaodan.cn

[G09] 接口 / 抽象类
来源：http://bwm.zycfv.cn

Py:   from abc import ABC, abstractmethod
来源：http://ghr.kuanghao11.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xmz.jyoumei.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pui.c1oappe.top

TS:   interface Shape { area(): number; }
来源：http://jxw.jinqigufen.top

Java: interface Shape { double area(); }
来源：http://amh.hnqzz.top

Go:   type Shape interface { Area() float64 }
来源：http://oun.hywenlv.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lzr.haohaochexian.top

C#:   interface IShape { double Area(); }
来源：http://nbh.yvedp.cn

[G10] 访问控制
来源：http://skh.gotoacloud.top

Py:   约定 _protected / __private（不强制）
来源：http://wcx.bjfxy.top

PHP:  public / protected / private
来源：http://crg.chenzaomai.com

JS:   #private 字段；其余公开
来源：http://nhz.jqgufenzy.top

TS:   public / protected / private
来源：http://igo.yongpay.top

Java: public / protected / private / 默认包级
来源：http://erw.zdqjudy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://hol.nanxinkj.top

Ruby: public / protected / private
来源：http://pmx.yangfankeji.com

C#:   public / protected / private / internal
来源：http://ocl.gaohongyu789.top

[G11] getter / setter
来源：http://rec.fktsv.cn

Py:   @property 与 @x.setter
来源：http://mep.yfazqb.com

PHP:  public function getName(): string { return $this->name; }
来源：http://jpc.shzxlz.cn

JS:   get name() { return this._name; }
来源：http://xmi.tianlin.xyz

TS:   get name(): string { return this._name; }
来源：http://nhk.birdmap.top

Java: public String getName() { return name; }
来源：http://ipn.cucudq.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://dnz.yj20258888.top

Ruby: attr_accessor :name
来源：http://jpj.wangshuangyany.cn

C#:   public string Name { get; set; }
来源：http://xit.zhoulong.xyz

[G12] 对象转字符串
来源：http://tff.yuxming.cn

Py:   def __str__(self): return self.name
来源：http://hrx.hywenlv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://snp.52xcode.cn

JS:   toString() { return this.name; }
来源：http://nja.jinqigfzy.top

TS:   toString(): string { return this.name; }
来源：http://osc.hnqzz.top

Java: @Override public String toString() { return name; }
来源：http://tsv.ppjwa.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gkl.jiagoushi.top

Ruby: def to_s; @name; end
来源：http://nss.xingfuxueyuan.xyz

C#:   public override string ToString() => Name;
来源：http://ifc.vehdjk.com

[G13] 判断对象类型
来源：http://vwh.sysykeji.top

Py:   isinstance(u, User)
来源：http://hre.hywenlv.cn

PHP:  $u instanceof User
来源：http://ced.zycfv.cn

JS:   u instanceof User
来源：http://nvj.hywenlv.cn

TS:   u instanceof User
来源：http://lwu.zhijiandao.cn

Java: u instanceof User
来源：http://lwe.zhaomingkeji.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://amh.jinqigfzy.top

Ruby: u.is_a?(User)
来源：http://nrk.zdbjq.cn

C#:   u is User
来源：http://smn.chenzaomai.com

[G14] 数据类 / record
来源：http://lew.jinyuanbaomall.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://clf.ydzc1.top

PHP:  // 用 readonly 属性模拟
来源：http://kbt.haohaochexian.top

JS:   // 无内置：普通类或对象字面量
来源：http://gfg.cdnleiting.top

TS:   type User = { name: string; age: number };
来源：http://gqo.yongpay.top

Java: record User(String name, int age) {}
来源：http://zst.sufxvd.cn

Go:   type User struct { Name string; Age int }
来源：http://epq.uphjek.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://egi.yfazqb.com

C#:   record User(string Name, int Age);
来源：http://tle.dashuyun.cn

[G15] 枚举
来源：http://uag.pengpengdd.cyou

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wfg.pycfn.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://wgp.jianghu66.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://oob.jinghuilouyu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rxk.hongshengwenyu.top

Java: enum Color { RED, GREEN }
来源：http://wlw.wangdashe.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hxn.52xcode.cn

Ruby: Color = %i[red green].freeze
来源：http://igk.fktsv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rjr.meibo888.top

[G16] 对象转数组 / 字典
来源：http://zmw.fengsongda.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uqi.jinqigufen.top

PHP:  get_object_vars($obj);
来源：http://rus.gaohongyu789.top

JS:   Object.entries(obj)
来源：http://gnv.zdqjudy.top

TS:   Object.entries(obj)
来源：http://qtf.zdbjq.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ook.yuxming.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://lhr.yangfankeji.com

Ruby: obj.instance_variables
来源：http://mlc.shuidangran.top

C#:   // 用反射或 System.Text.Json
来源：http://pem.redwolf501.top

================================================================================
来源：http://qet.meibo888.top

H. 异常与错误处理
来源：http://ksi.cucudq.cn

================================================================================
来源：http://imw.yj20258.top

[H01] try / catch 基础
来源：http://jom.daria6918.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bvf.feifeiyinyue.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yga.ydjk.org.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nbi.shzxlz.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://atp.fanxiaobao.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zev.sweek.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sfl.cucudq.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qsw.gaohongyu789.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kvd.shangyingyoupin.top

[H02] finally / ensure 收尾
来源：http://jrc.xingfuxueyuan.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://fhc.jyoumei.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://opd.fengsongda.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ycc.zhaomingkeji.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://bzi.c1oappe.top

Java: try { f(); } finally { cleanup(); }
来源：http://lgq.zycfv.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://cxs.cqqwz.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://cqk.hnqzz.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://mab.yuxming.cn

[H03] 主动抛出异常
来源：http://oey.fehbvm.com

Py:   raise ValueError("错误信息")
来源：http://bge.tian-w.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uus.fktsv.cn

JS:   throw new Error("错误信息");
来源：http://ima.tian-w.cn

TS:   throw new Error("错误信息");
来源：http://znr.nanxuanxn.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ipj.zdqjudy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cal.sxryk.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wmz.gotoacloud.top

C#:   throw new ArgumentException("错误信息");
来源：http://vkf.xziqi.cn

[H04] 自定义异常类型
来源：http://pro.ppjwa.cn

Py:   class MyError(Exception): pass
来源：http://jdg.52xcode.cn

PHP:  class MyError extends RuntimeException {}
来源：http://hpn.0kj1m.cn

JS:   class MyError extends Error {}
来源：http://edt.yueranfly.top

TS:   class MyError extends Error {}
来源：http://iwz.dianchejie.cn

Java: class MyException extends RuntimeException {}
来源：http://ibz.shzxlz.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://igs.gogol.net.cn

Ruby: class MyError < StandardError; end
来源：http://bdz.jqgfzy.top

C#:   class MyException : Exception {}
来源：http://xkv.ydzc1.top

[H05] 捕获特定类型
来源：http://vfx.tian-w.cn

Py:   except ValueError as e:
来源：http://kiv.yonumen.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ioa.52xcode.cn

JS:   if (e instanceof TypeError) {}
来源：http://hxr.jianghu66.top

TS:   if (e instanceof TypeError) {}
来源：http://qjq.havefunace.top

Java: catch (IOException | SQLException e) {}
来源：http://snd.yuxming.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dfq.feifeiyinyue.top

Ruby: rescue ArgumentError => e
来源：http://mdl.smart0.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://clj.yj20258888.top

[H06] 可选值 / 空值安全访问
来源：http://umw.52xcode.cn

Py:   value = d.get("k") or default
来源：http://xet.tanke756.top

PHP:  $v = $d["k"] ?? null;
来源：http://wai.daria6918.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wmv.shzxlz.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vuo.sysykeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fxj.daria6918.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://epf.gzhubu.top

Ruby: d&.dig(:a, :b)
来源：http://cwf.jlsjyb.cn

C#:   obj?.A?.B ?? default
来源：http://mxb.52xcode.cn

[H07] 断言
来源：http://vtc.xinyue.icu

Py:   assert x > 0, "必须为正"
来源：http://fwu.shangyingyoupin.top

PHP:  assert($x > 0);
来源：http://vzs.aizwys.cn

JS:   console.assert(x > 0);
来源：http://mav.snrcjt.cn

TS:   console.assert(x > 0);
来源：http://aqm.fengsongda.top

Java: assert x > 0 : "必须为正";
来源：http://mfl.fengsongda.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qgj.tanke756.top

Ruby: raise "必须为正" unless x > 0
来源：http://ifl.svipenyu.cn

C#:   Debug.Assert(x > 0);
来源：http://usz.yfazqb.com

[H08] 获取错误信息与堆栈
来源：http://pcb.ppjwa.cn

Py:   str(e);  traceback.format_exc()
来源：http://krj.ydjk.org.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yhw.shangyingyoupin.top

JS:   e.message;  e.stack
来源：http://jdf.zdqjudy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://hjz.svipenyu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://fbn.havefunace.top

Go:   err.Error()
来源：http://svt.nwbrower.top

Ruby: e.message;  e.backtrace
来源：http://msy.fehbvm.com

C#:   e.Message;  e.StackTrace
来源：http://til.bjfxy.top

[H09] 带错误码的异常
来源：http://ueo.sysykeji.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rqk.hammf.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gce.havefunace.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ctj.snrcjt.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://owi.smart0.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hdf.hongshengwenyu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fhg.hnxiangtu.top

Ruby: raise MyError.new("fail", 500)
来源：http://eqq.fanxiaobao.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://ugd.yongpay.top

[H10] 资源自动释放
来源：http://kpg.ydjk.org.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://cmg.hongshengwenyu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://api.zhengqikj.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pso.tianlin.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zhn.redwolf501.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gwt.xuanzx.com

Go:   defer f.Close()
来源：http://rgi.xingfuxueyuan.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mxr.gzhubu.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qwh.yvedp.cn

================================================================================
来源：http://woy.quarkkingdee.top

I. 正则表达式
来源：http://umy.feifeiyinyue.top

================================================================================
来源：http://eyv.sufxvd.cn

[I01] 判断是否匹配
来源：http://lju.zhixingplan.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lbk.fzhhl.top

PHP:  preg_match('/\d+/', $s);
来源：http://die.yanxiufei.cn

JS:   /\d+/.test(s)
来源：http://wdh.yvedp.cn

TS:   /\d+/.test(s)
来源：http://yac.c1oappe.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qyn.sxryk.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dqt.ybcxt.top

Ruby: s.match?(/\d+/)
来源：http://rll.redwolf501.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://enx.yongpay.top

[I02] 提取所有匹配
来源：http://hzp.yanxiufei.cn

Py:   re.findall(r"\d+", s)
来源：http://iql.ppjwa.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://men.xingfuxueyuan.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://uiz.yj202588.top

TS:   s.match(/\d+/g)
来源：http://fou.fehbvm.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://trw.xuetiantiany.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ylv.feifeiyinyue.top

Ruby: s.scan(/\d+/)
来源：http://ikq.jiagoushi.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://emu.ehwqpu.com

[I03] 提取捕获分组
来源：http://ick.jianghu66.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fpn.sysykeji.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tvk.chenzaomai.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://weg.andypj.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://thb.hnqzz.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hbh.fktsv.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://uev.fzhhl.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tmh.uphjek.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://req.zdbjq.cn

[I04] 正则替换
来源：http://gje.jqgufenzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://cvx.nwbrower.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tcb.nanxuanxn.top

JS:   s.replace(/\d+/g, "#")
来源：http://lfa.zdbjq.cn

TS:   s.replace(/\d+/g, "#")
来源：http://tqh.gaohongyu789.top

Java: s.replaceAll("\\d+", "#")
来源：http://enf.ivvv.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ppp.zhiwuduotai.top

Ruby: s.gsub(/\d+/, "#")
来源：http://qya.zhixingplan.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nef.tianlin.xyz

[I05] 按正则拆分
来源：http://aof.hcnkem.com

Py:   re.split(r"\s*,\s*", s)
来源：http://ptu.sxryk.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rwp.ppjwa.cn

JS:   s.split(/\s*,\s*/)
来源：http://okc.vqdsnc.cn

TS:   s.split(/\s*,\s*/)
来源：http://iii.yj202588.top

Java: s.split("\\s*,\\s*")
来源：http://wwr.hfpthk.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bsr.fengsongda.top

Ruby: s.split(/\s*,\s*/)
来源：http://uwa.aizwys.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hst.fanxiaobao.xyz


<!-- 参考信息 -->