代发 wailian999

Py:   class User: pass
来源：http://ser.zhixingplan.top

PHP:  class User {}
来源：http://odr.yangfankeji.com

JS:   class User {}
来源：http://bsh.52xcode.cn

TS:   class User { name: string = ""; }
来源：http://wku.jqgufenzy.top

Java: class User {}
来源：http://iul.xuanzx.com

Go:   type User struct { Name string }
来源：http://wkk.ydzc1.top

Ruby: class User; end
来源：http://gmg.bjfxy.top

C#:   class User {}
来源：http://smf.daria6918.cn

[G02] 构造函数
来源：http://aew.hammf.cn

Py:   def __init__(self, name): self.name = name
来源：http://ssl.cucudq.cn

PHP:  public function __construct(public string $name) {}
来源：http://hbc.yj20258888.top

JS:   constructor(name) { this.name = name; }
来源：http://vkr.hysaishi.cn

TS:   constructor(public name: string) {}
来源：http://qzn.wangshuangyany.cn

Java: User(String name) { this.name = name; }
来源：http://kto.yuanzhike.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qdy.mhx1999.top

Ruby: def initialize(name); @name = name; end
来源：http://kug.hnxiangtu.top

C#:   public User(string name) { Name = name; }
来源：http://udm.cashguo.top

[G03] 实例属性
来源：http://nok.0kj1m.cn

Py:   self.name = "x"
来源：http://ikd.ivvv.top

PHP:  public string $name = "x";
来源：http://yls.fehbvm.com

JS:   this.name = "x";
来源：http://pyu.cqqwz.cn

TS:   name: string = "x";
来源：http://vmp.yvedp.cn

Java: private String name;
来源：http://rgr.hesvh.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://esu.svipenyu.cn

Ruby: @name = "x"
来源：http://ltw.yueranfly.top

C#:   public string Name { get; set; } = "x";
来源：http://mwh.yonumen.top

[G04] 定义方法
来源：http://jir.cucudq.cn

Py:   def greet(self): return self.name
来源：http://qlv.zhixingplan.top

PHP:  public function greet(): string { return $this->name; }
来源：http://bst.jiagoushi.top

JS:   greet() { return this.name; }
来源：http://gri.guowangkeji.top

TS:   greet(): string { return this.name; }
来源：http://xyx.ybcxt.top

Java: String greet() { return name; }
来源：http://nix.mhx1999.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://fhk.yangfankeji.com

Ruby: def greet; @name; end
来源：http://ooh.shzxlz.cn

C#:   public string Greet() => Name;
来源：http://hes.ppjwa.cn

[G05] 继承
来源：http://out.feifeiyinyue.top

Py:   class Admin(User): pass
来源：http://pfn.fehbvm.com

PHP:  class Admin extends User {}
来源：http://cxb.ctjpmb.com

JS:   class Admin extends User {}
来源：http://pdg.wangshuangyany.cn

TS:   class Admin extends User {}
来源：http://dnp.gotoacloud.top

Java: class Admin extends User {}
来源：http://wix.zhongyouzk.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zvf.shangyingyoupin.top

Ruby: class Admin < User; end
来源：http://eth.jqgufenzy.top

C#:   class Admin : User {}
来源：http://uiy.zdqjudy.top

[G06] 重写方法
来源：http://sev.yfazqb.com

Py:   def greet(self): return "admin"
来源：http://hns.sysykeji.top

PHP:  public function greet(): string { return "admin"; }
来源：http://okz.feifeiyinyue.top

JS:   greet() { return "admin"; }
来源：http://ckt.jianghu66.top

TS:   greet(): string { return "admin"; }
来源：http://hgr.xingfuxueyuan.xyz

Java: @Override String greet() { return "admin"; }
来源：http://fgg.chenlongwang.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://eyp.tian-w.cn

Ruby: def greet; "admin"; end
来源：http://rtn.wangdashe.top

C#:   public override string Greet() => "admin";
来源：http://dam.yonumen.top

[G07] 调用父类方法
来源：http://wrn.iojbl.cn

Py:   super().greet()
来源：http://zcy.uphjek.com

PHP:  parent::greet();
来源：http://ddc.ydzc1.top

JS:   super.greet();
来源：http://egx.yvedp.cn

TS:   super.greet();
来源：http://ncj.kuanghao11.cn

Java: super.greet();
来源：http://uuo.yvedp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://teu.daxiang520.top

Ruby: super
来源：http://qsb.uphjek.com

C#:   base.Greet();
来源：http://zkb.sufxvd.cn

[G08] 静态方法与属性
来源：http://yxl.ivvv.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rgq.zdbjq.cn

PHP:  public static function f() {}
来源：http://gbu.dashuyun.cn

JS:   static f() {}
来源：http://oik.zhaomingkeji.xyz

TS:   static f(): void {}
来源：http://uqj.redwolf501.top

Java: static void f() {}
来源：http://jqa.haohaochexian.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://yzt.mhx1999.top

Ruby: def self.f; end
来源：http://tnl.yanxiufei.cn

C#:   public static void F() {}
来源：http://nha.daxiang520.top

[G09] 接口 / 抽象类
来源：http://ege.epnwcf.com

Py:   from abc import ABC, abstractmethod
来源：http://koi.tarul.cn

PHP:  interface Shape { public function area(): float; }
来源：http://czl.c1oappe.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ypa.dianchejie.cn

TS:   interface Shape { area(): number; }
来源：http://cxh.zycfv.cn

Java: interface Shape { double area(); }
来源：http://rga.cheryme.top

Go:   type Shape interface { Area() float64 }
来源：http://dum.sysykeji.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zgq.ybcxt.top

C#:   interface IShape { double Area(); }
来源：http://kms.uphjek.com

[G10] 访问控制
来源：http://yiz.316326.xyz

Py:   约定 _protected / __private（不强制）
来源：http://ane.shuidangran.top

PHP:  public / protected / private
来源：http://gat.chenzaomai.com

JS:   #private 字段；其余公开
来源：http://fej.nanxuanxn.top

TS:   public / protected / private
来源：http://qsf.yonumen.top

Java: public / protected / private / 默认包级
来源：http://rre.jiagoushi.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://eeq.shzxlz.cn

Ruby: public / protected / private
来源：http://xdb.yuanzhike.top

C#:   public / protected / private / internal
来源：http://buu.0kj1m.cn

[G11] getter / setter
来源：http://pyv.guowangkeji.top

Py:   @property 与 @x.setter
来源：http://dkx.ybcxt.top

PHP:  public function getName(): string { return $this->name; }
来源：http://tqk.xinyue.icu

JS:   get name() { return this._name; }
来源：http://hao.vqdsnc.cn

TS:   get name(): string { return this._name; }
来源：http://sit.yongpay.top

Java: public String getName() { return name; }
来源：http://hxi.jinqigufen.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://myg.birdmap.top

Ruby: attr_accessor :name
来源：http://wne.yj202588.top

C#:   public string Name { get; set; }
来源：http://vjb.birdmap.top

[G12] 对象转字符串
来源：http://uch.zhengqikj.top

Py:   def __str__(self): return self.name
来源：http://exc.sxryk.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://wfv.yueranfly.top

JS:   toString() { return this.name; }
来源：http://djg.ywan-chungtsiang.top

TS:   toString(): string { return this.name; }
来源：http://qut.zycfv.cn

Java: @Override public String toString() { return name; }
来源：http://hla.fengsongda.top

Go:   func (u User) String() string { return u.Name }
来源：http://dab.hcnkem.com

Ruby: def to_s; @name; end
来源：http://aab.smart0.xyz

C#:   public override string ToString() => Name;
来源：http://lur.sufxvd.cn

[G13] 判断对象类型
来源：http://ohy.fehbvm.com

Py:   isinstance(u, User)
来源：http://ifr.fehbvm.com

PHP:  $u instanceof User
来源：http://kmi.chenzaomai.com

JS:   u instanceof User
来源：http://gpt.jinqigufen.top

TS:   u instanceof User
来源：http://duy.cucudq.cn

Java: u instanceof User
来源：http://mbh.ivvv.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://pmp.andypj.xyz

Ruby: u.is_a?(User)
来源：http://unz.tian-w.cn

C#:   u is User
来源：http://cen.xziqi.cn

[G14] 数据类 / record
来源：http://fhn.tarul.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xep.hcnkem.com

PHP:  // 用 readonly 属性模拟
来源：http://wic.bbcook.cn

JS:   // 无内置：普通类或对象字面量
来源：http://cbt.sweek.top

TS:   type User = { name: string; age: number };
来源：http://mef.ppjwa.cn

Java: record User(String name, int age) {}
来源：http://brt.ydzc1.top

Go:   type User struct { Name string; Age int }
来源：http://ilz.hesvh.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://awy.snrcjt.cn

C#:   record User(string Name, int Age);
来源：http://dxw.sjlbkw.cn

[G15] 枚举
来源：http://qim.fzhhl.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dug.shzxlz.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://uqc.hnxiangtu.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qsx.redwolf501.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vqd.cucudq.cn

Java: enum Color { RED, GREEN }
来源：http://wni.zycfv.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pus.yfazqb.com

Ruby: Color = %i[red green].freeze
来源：http://txp.yvedp.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yix.sxryk.cn

[G16] 对象转数组 / 字典
来源：http://dba.jinqigfzy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dbl.nanxuanxn.top

PHP:  get_object_vars($obj);
来源：http://yal.ppjwa.cn

JS:   Object.entries(obj)
来源：http://xuo.mhx1999.top

TS:   Object.entries(obj)
来源：http://kdv.jyoumei.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://oof.ppjwa.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hcq.ydzc1.top

Ruby: obj.instance_variables
来源：http://ggp.9152youxi.cn

C#:   // 用反射或 System.Text.Json
来源：http://pzm.sufxvd.cn

================================================================================
来源：http://zaf.shzxlz.cn

H. 异常与错误处理
来源：http://jde.bbcook.cn

================================================================================
来源：http://wcw.jlsjyb.cn

[H01] try / catch 基础
来源：http://vnb.mhx1999.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://iat.daxiang520.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jwe.jyoumei.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mhy.zdbjq.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://eqq.iojbl.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ajg.jianghu66.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cfu.tarul.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tsi.dashuyun.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hre.tarul.cn

[H02] finally / ensure 收尾
来源：http://epg.ivvv.top

Py:   try: f()⏎finally: cleanup()
来源：http://lme.dianchejie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ebv.vehdjk.com

JS:   try { f(); } finally { cleanup(); }
来源：http://nve.jlsjyb.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ewt.yj20258888.top

Java: try { f(); } finally { cleanup(); }
来源：http://aor.52xcode.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xbh.zhijiandao.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://rtg.yuanzhike.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://kls.vehdjk.com

[H03] 主动抛出异常
来源：http://szg.yongpay.top

Py:   raise ValueError("错误信息")
来源：http://sig.hammf.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tdd.yfazqb.com

JS:   throw new Error("错误信息");
来源：http://ryb.cqqwz.cn

TS:   throw new Error("错误信息");
来源：http://ezi.zycfv.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mxz.jyoumei.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ruy.yuxming.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fgv.ybcxt.top

C#:   throw new ArgumentException("错误信息");
来源：http://knz.tianlin.xyz

[H04] 自定义异常类型
来源：http://clu.ivvv.top

Py:   class MyError(Exception): pass
来源：http://juh.cashguo.top

PHP:  class MyError extends RuntimeException {}
来源：http://xhy.yj202588.top

JS:   class MyError extends Error {}
来源：http://yed.fzhhl.top

TS:   class MyError extends Error {}
来源：http://llk.mhx1999.top

Java: class MyException extends RuntimeException {}
来源：http://mvs.xziqi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vte.zhoulong.xyz

Ruby: class MyError < StandardError; end
来源：http://oug.jinqigfzy.top

C#:   class MyException : Exception {}
来源：http://njb.hysaishi.cn

[H05] 捕获特定类型
来源：http://llu.wangshuangyany.cn

Py:   except ValueError as e:
来源：http://ctg.ppjwa.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bqy.iojbl.cn

JS:   if (e instanceof TypeError) {}
来源：http://zsx.havefunace.top

TS:   if (e instanceof TypeError) {}
来源：http://prz.zhongyouzk.top

Java: catch (IOException | SQLException e) {}
来源：http://sct.yangfankeji.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kik.pengpengdd.cyou

Ruby: rescue ArgumentError => e
来源：http://yke.gaohongyu789.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hgv.yueranfly.top

[H06] 可选值 / 空值安全访问
来源：http://amm.nwbrower.top

Py:   value = d.get("k") or default
来源：http://uxk.gaohongyu789.top

PHP:  $v = $d["k"] ?? null;
来源：http://ttk.hysaishi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://gsi.tianlin.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://rpv.quarkkingdee.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://onz.bjfxy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://adj.epnwcf.com

Ruby: d&.dig(:a, :b)
来源：http://olv.yanxiufei.cn

C#:   obj?.A?.B ?? default
来源：http://bcy.vqdsnc.cn

[H07] 断言
来源：http://pox.aizwys.cn

Py:   assert x > 0, "必须为正"
来源：http://zle.yfazqb.com

PHP:  assert($x > 0);
来源：http://qjw.wangdashe.top

JS:   console.assert(x > 0);
来源：http://ejm.bbcook.cn

TS:   console.assert(x > 0);
来源：http://sqc.yj202588.top

Java: assert x > 0 : "必须为正";
来源：http://qyh.quarkkingdee.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://icq.shzxlz.cn

Ruby: raise "必须为正" unless x > 0
来源：http://acu.ydjk.org.cn

C#:   Debug.Assert(x > 0);
来源：http://xct.snrcjt.cn

[H08] 获取错误信息与堆栈
来源：http://epd.xuetiantiany.cn

Py:   str(e);  traceback.format_exc()
来源：http://joj.shangyingyoupin.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gsl.xziqi.cn

JS:   e.message;  e.stack
来源：http://qix.jinqigfzy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://aas.hongshengwenyu.top

Java: e.getMessage();  e.printStackTrace()
来源：http://wkm.xingfuxueyuan.xyz

Go:   err.Error()
来源：http://gce.birdmap.top

Ruby: e.message;  e.backtrace
来源：http://vze.hysaishi.cn

C#:   e.Message;  e.StackTrace
来源：http://roy.yj20258888.top

[H09] 带错误码的异常
来源：http://tqb.hnxiangtu.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hne.ybcxt.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://dqx.wangshuangyany.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://iet.nwbrower.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bvb.xuanzx.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sdl.chenjidiqi.icu

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fwf.yonumen.top

Ruby: raise MyError.new("fail", 500)
来源：http://wej.zdqjudy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://jvw.xziqi.cn

[H10] 资源自动释放
来源：http://tai.chenjidiqi.icu

Py:   with open("a.txt") as f: data = f.read()
来源：http://xvx.gzhubu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fpg.fktsv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://apw.tarul.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kow.ctjpmb.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nzk.shanyushiyangtech.top

Go:   defer f.Close()
来源：http://jbn.zhengqikj.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mss.kuanghao11.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://eja.9152youxi.cn

================================================================================
来源：http://jsa.tarul.cn

I. 正则表达式
来源：http://eja.fzhhl.top

================================================================================
来源：http://kvr.aibaodan.cn

[I01] 判断是否匹配
来源：http://mqn.zhijiandao.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vup.yanxiufei.cn

PHP:  preg_match('/\d+/', $s);
来源：http://kka.ywan-chungtsiang.top

JS:   /\d+/.test(s)
来源：http://lng.fengsongda.top

TS:   /\d+/.test(s)
来源：http://vdp.aibaodan.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kkg.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tcl.andypj.xyz

Ruby: s.match?(/\d+/)
来源：http://efn.xingfuxueyuan.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zqj.52xcode.cn

[I02] 提取所有匹配
来源：http://zmo.ydjk.org.cn

Py:   re.findall(r"\d+", s)
来源：http://vxr.fehbvm.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hdq.yvedp.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hfk.havefunace.top

TS:   s.match(/\d+/g)
来源：http://xfi.jianghu66.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mwd.fengsongda.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xuz.chenlongwang.top

Ruby: s.scan(/\d+/)
来源：http://ltm.zdbjq.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jdi.zhengqikj.top

[I03] 提取捕获分组
来源：http://ufa.gotoacloud.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rep.hammf.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://aow.shanyushiyangtech.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bcm.yueranfly.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lve.nwbrower.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://scy.xuanzx.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rgw.quarkkingdee.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ojs.ctjpmb.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://adq.shanyushiyangtech.top

[I04] 正则替换
来源：http://vkz.yj20258888.top

Py:   re.sub(r"\d+", "#", s)
来源：http://gim.fanxiaobao.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qvw.yj202588.top

JS:   s.replace(/\d+/g, "#")
来源：http://mur.chenlongwang.top

TS:   s.replace(/\d+/g, "#")
来源：http://pvk.snrcjt.cn

Java: s.replaceAll("\\d+", "#")
来源：http://gxs.9152youxi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://cdt.snrcjt.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gca.meibo888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qgp.yj20258.top

[I05] 按正则拆分
来源：http://bjw.sufxvd.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://bkq.quarkkingdee.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dfj.zhengqikj.top

JS:   s.split(/\s*,\s*/)
来源：http://qqx.0kj1m.cn

TS:   s.split(/\s*,\s*/)
来源：http://usw.zdbjq.cn

Java: s.split("\\s*,\\s*")
来源：http://gwi.epnwcf.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bcd.yj20258.top

Ruby: s.split(/\s*,\s*/)
来源：http://kzr.yuxming.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wyx.cheryme.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mml.jinqigfzy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wwm.hfpthk.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://esm.gotoacloud.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pty.xziqi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wyk.svipenyu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nyo.0kj1m.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hjj.xuetiantiany.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bjr.tarul.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://srr.ivvv.top

[I07] 忽略大小写与多行模式
来源：http://qlr.birdmap.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://uic.fanxiaobao.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fua.chenlongwang.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rlx.zdqjudy.top

TS:   /error/gim
来源：http://owc.jiagoushi.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lbl.hywenlv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dkh.shzxlz.cn


<!-- 参考信息 -->